# Comparing `tmp/bokeh-3.2.0.dev3.tar.gz` & `tmp/bokeh-3.2.0.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bokeh-3.2.0.dev3.tar", last modified: Tue May 30 22:10:12 2023, max compression
+gzip compressed data, was "bokeh-3.2.0.dev4.tar", last modified: Fri Jun  9 10:33:29 2023, max compression
```

## Comparing `bokeh-3.2.0.dev3.tar` & `bokeh-3.2.0.dev4.tar`

### file list

```diff
@@ -1,1205 +1,1205 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 22:10:12.946560 bokeh-3.2.0.dev3/
--rw-r--r--   0 runner    (1001) docker     (122)     1494 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      881 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    12082 2023-05-30 22:10:12.946560 bokeh-3.2.0.dev3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     8603 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/README.md
--rw-r--r--   0 runner    (1001) docker     (122)    10430 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-30 22:10:12.946560 bokeh-3.2.0.dev3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     6745 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 22:10:12.794561 bokeh-3.2.0.dev3/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 22:10:12.802561 bokeh-3.2.0.dev3/src/bokeh/
--rw-r--r--   0 runner    (1001) docker     (122)     1494 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)     3750 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2136 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)    73110 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/_sri.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 22:10:12.802561 bokeh-3.2.0.dev3/src/bokeh/application/
--rw-r--r--   0 runner    (1001) docker     (122)     2145 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/application/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11549 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/application/application.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 22:10:12.806561 bokeh-3.2.0.dev3/src/bokeh/application/handlers/
--rw-r--r--   0 runner    (1001) docker     (122)     2194 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/application/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6919 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/application/handlers/code.py
--rw-r--r--   0 runner    (1001) docker     (122)     7818 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/application/handlers/code_runner.py
--rw-r--r--   0 runner    (1001) docker     (122)    10926 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/application/handlers/directory.py
--rw-r--r--   0 runner    (1001) docker     (122)     2882 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/application/handlers/document_lifecycle.py
--rw-r--r--   0 runner    (1001) docker     (122)     4943 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/application/handlers/function.py
--rw-r--r--   0 runner    (1001) docker     (122)     7975 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/application/handlers/handler.py
--rw-r--r--   0 runner    (1001) docker     (122)     4705 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/application/handlers/lifecycle.py
--rw-r--r--   0 runner    (1001) docker     (122)     5180 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/application/handlers/notebook.py
--rw-r--r--   0 runner    (1001) docker     (122)     2921 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/application/handlers/request_handler.py
--rw-r--r--   0 runner    (1001) docker     (122)     3348 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/application/handlers/script.py
--rw-r--r--   0 runner    (1001) docker     (122)     5035 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/application/handlers/server_lifecycle.py
--rw-r--r--   0 runner    (1001) docker     (122)     4339 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/application/handlers/server_request_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 22:10:12.806561 bokeh-3.2.0.dev3/src/bokeh/client/
--rw-r--r--   0 runner    (1001) docker     (122)     2373 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    16199 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/client/connection.py
--rw-r--r--   0 runner    (1001) docker     (122)    21727 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/client/session.py
--rw-r--r--   0 runner    (1001) docker     (122)     5334 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/client/states.py
--rw-r--r--   0 runner    (1001) docker     (122)     3299 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/client/util.py
--rw-r--r--   0 runner    (1001) docker     (122)     3252 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/client/websocket.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 22:10:12.806561 bokeh-3.2.0.dev3/src/bokeh/colors/
--rw-r--r--   0 runner    (1001) docker     (122)     1948 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/colors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    14039 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/colors/color.py
--rw-r--r--   0 runner    (1001) docker     (122)     9825 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/colors/groups.py
--rw-r--r--   0 runner    (1001) docker     (122)    13046 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/colors/named.py
--rw-r--r--   0 runner    (1001) docker     (122)     5432 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/colors/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 22:10:12.806561 bokeh-3.2.0.dev3/src/bokeh/command/
--rw-r--r--   0 runner    (1001) docker     (122)      901 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3965 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/command/bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (122)     5822 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/command/subcommand.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 22:10:12.806561 bokeh-3.2.0.dev3/src/bokeh/command/subcommands/
--rw-r--r--   0 runner    (1001) docker     (122)     2802 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/command/subcommands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2567 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/command/subcommands/build.py
--rw-r--r--   0 runner    (1001) docker     (122)     7336 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/command/subcommands/file_output.py
--rw-r--r--   0 runner    (1001) docker     (122)     4658 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/command/subcommands/info.py
--rw-r--r--   0 runner    (1001) docker     (122)     2765 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/command/subcommands/init.py
--rw-r--r--   0 runner    (1001) docker     (122)     3592 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/command/subcommands/json.py
--rw-r--r--   0 runner    (1001) docker     (122)     2564 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/command/subcommands/sampledata.py
--rw-r--r--   0 runner    (1001) docker     (122)     2775 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/command/subcommands/secret.py
--rw-r--r--   0 runner    (1001) docker     (122)    37703 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/command/subcommands/serve.py
--rw-r--r--   0 runner    (1001) docker     (122)     3764 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/command/subcommands/static.py
--rw-r--r--   0 runner    (1001) docker     (122)     7996 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/command/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 22:10:12.810561 bokeh-3.2.0.dev3/src/bokeh/core/
--rw-r--r--   0 runner    (1001) docker     (122)     2140 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 22:10:12.810561 bokeh-3.2.0.dev3/src/bokeh/core/_templates/
--rw-r--r--   0 runner    (1001) docker     (122)     4349 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/core/_templates/autoload_js.js
--rw-r--r--   0 runner    (1001) docker     (122)     6450 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/core/_templates/autoload_nb_js.js
--rw-r--r--   0 runner    (1001) docker     (122)     1393 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/core/_templates/autoload_request_tag.html
--rw-r--r--   0 runner    (1001) docker     (122)      815 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/core/_templates/autoload_tag.html
--rw-r--r--   0 runner    (1001) docker     (122)      469 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/core/_templates/css_resources.html
--rw-r--r--   0 runner    (1001) docker     (122)      314 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/core/_templates/doc_js.js
--rw-r--r--   0 runner    (1001) docker     (122)      213 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/core/_templates/doc_nb_js.js
--rw-r--r--   0 runner    (1001) docker     (122)     1606 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/core/_templates/file.html
--rw-r--r--   0 runner    (1001) docker     (122)      586 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/core/_templates/js_resources.html
--rw-r--r--   0 runner    (1001) docker     (122)      158 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/core/_templates/macros.html
--rw-r--r--   0 runner    (1001) docker     (122)     3933 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/core/_templates/notebook_load.html
--rw-r--r--   0 runner    (1001) docker     (122)      356 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/core/_templates/plot_div.html
--rw-r--r--   0 runner    (1001) docker     (122)       49 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/core/_templates/root_div.html
--rw-r--r--   0 runner    (1001) docker     (122)      260 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/core/_templates/script_tag.html
--rw-r--r--   0 runner    (1001) docker     (122)      591 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/core/_templates/try_run.js
--rw-r--r--   0 runner    (1001) docker     (122)    16751 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/core/enums.py
--rw-r--r--   0 runner    (1001) docker     (122)    29845 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/core/has_props.py
--rw-r--r--   0 runner    (1001) docker     (122)     7133 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/core/json_encoder.py
--rw-r--r--   0 runner    (1001) docker     (122)    11533 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/core/properties.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 22:10:12.814561 bokeh-3.2.0.dev3/src/bokeh/core/property/
--rw-r--r--   0 runner    (1001) docker     (122)     1658 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/core/property/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2782 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/core/property/_sphinx.py
--rw-r--r--   0 runner    (1001) docker     (122)     3646 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/core/property/alias.py
--rw-r--r--   0 runner    (1001) docker     (122)     1906 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/core/property/aliases.py
--rw-r--r--   0 runner    (1001) docker     (122)     3156 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/core/property/any.py
--rw-r--r--   0 runner    (1001) docker     (122)     2499 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/core/property/auto.py
--rw-r--r--   0 runner    (1001) docker     (122)    20064 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/core/property/bases.py
--rw-r--r--   0 runner    (1001) docker     (122)     6436 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/core/property/color.py
--rw-r--r--   0 runner    (1001) docker     (122)    12052 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/core/property/container.py
--rw-r--r--   0 runner    (1001) docker     (122)    22696 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/core/property/dataspec.py
--rw-r--r--   0 runner    (1001) docker     (122)     6091 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/core/property/datetime.py
--rw-r--r--   0 runner    (1001) docker     (122)     5123 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/core/property/descriptor_factory.py
--rw-r--r--   0 runner    (1001) docker     (122)    34998 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/core/property/descriptors.py
--rw-r--r--   0 runner    (1001) docker     (122)     4198 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/core/property/either.py
--rw-r--r--   0 runner    (1001) docker     (122)     3989 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/core/property/enum.py
--rw-r--r--   0 runner    (1001) docker     (122)     3021 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/core/property/factors.py
--rw-r--r--   0 runner    (1001) docker     (122)     2879 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/core/property/include.py
--rw-r--r--   0 runner    (1001) docker     (122)     6521 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/core/property/instance.py
--rw-r--r--   0 runner    (1001) docker     (122)     2743 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/core/property/json.py
--rw-r--r--   0 runner    (1001) docker     (122)     2139 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/core/property/nothing.py
--rw-r--r--   0 runner    (1001) docker     (122)     3745 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/core/property/nullable.py
--rw-r--r--   0 runner    (1001) docker     (122)     9631 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/core/property/numeric.py
--rw-r--r--   0 runner    (1001) docker     (122)     3458 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/core/property/override.py
--rw-r--r--   0 runner    (1001) docker     (122)     3251 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/core/property/pd.py
--rw-r--r--   0 runner    (1001) docker     (122)     7166 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/core/property/primitive.py
--rw-r--r--   0 runner    (1001) docker     (122)     2255 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/core/property/readonly.py
--rw-r--r--   0 runner    (1001) docker     (122)     2494 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/core/property/required.py
--rw-r--r--   0 runner    (1001) docker     (122)     2536 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/core/property/serialized.py
--rw-r--r--   0 runner    (1001) docker     (122)     2351 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/core/property/singletons.py
--rw-r--r--   0 runner    (1001) docker     (122)     3465 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/core/property/string.py
--rw-r--r--   0 runner    (1001) docker     (122)     3896 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/core/property/struct.py
--rw-r--r--   0 runner    (1001) docker     (122)     2481 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/core/property/text_like.py
--rw-r--r--   0 runner    (1001) docker     (122)     3378 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/core/property/validation.py
--rw-r--r--   0 runner    (1001) docker     (122)     5977 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/core/property/vectorization.py
--rw-r--r--   0 runner    (1001) docker     (122)     8905 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/core/property/visual.py
--rw-r--r--   0 runner    (1001) docker     (122)    17517 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/core/property/wrappers.py
--rw-r--r--   0 runner    (1001) docker     (122)     3508 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/core/property_aliases.py
--rw-r--r--   0 runner    (1001) docker     (122)    12260 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/core/property_mixins.py
--rw-r--r--   0 runner    (1001) docker     (122)    10171 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/core/query.py
--rw-r--r--   0 runner    (1001) docker     (122)    23292 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/core/serialization.py
--rw-r--r--   0 runner    (1001) docker     (122)     4892 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/core/templates.py
--rw-r--r--   0 runner    (1001) docker     (122)     3025 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/core/types.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 22:10:12.814561 bokeh-3.2.0.dev3/src/bokeh/core/validation/
--rw-r--r--   0 runner    (1001) docker     (122)     3502 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/core/validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7168 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/core/validation/check.py
--rw-r--r--   0 runner    (1001) docker     (122)     6555 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/core/validation/decorators.py
--rw-r--r--   0 runner    (1001) docker     (122)     9259 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/core/validation/errors.py
--rw-r--r--   0 runner    (1001) docker     (122)     2983 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/core/validation/issue.py
--rw-r--r--   0 runner    (1001) docker     (122)     3082 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/core/validation/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 22:10:12.814561 bokeh-3.2.0.dev3/src/bokeh/document/
--rw-r--r--   0 runner    (1001) docker     (122)     2435 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/document/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    16657 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/document/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (122)    27922 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/document/document.py
--rw-r--r--   0 runner    (1001) docker     (122)    29934 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/document/events.py
--rw-r--r--   0 runner    (1001) docker     (122)     3419 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/document/json.py
--rw-r--r--   0 runner    (1001) docker     (122)     4978 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/document/locking.py
--rw-r--r--   0 runner    (1001) docker     (122)     9341 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/document/models.py
--rw-r--r--   0 runner    (1001) docker     (122)     5026 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/document/modules.py
--rw-r--r--   0 runner    (1001) docker     (122)     6344 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/driving.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 22:10:12.818561 bokeh-3.2.0.dev3/src/bokeh/embed/
--rw-r--r--   0 runner    (1001) docker     (122)     2074 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/embed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    14666 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/embed/bundle.py
--rw-r--r--   0 runner    (1001) docker     (122)     6464 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/embed/elements.py
--rw-r--r--   0 runner    (1001) docker     (122)     3968 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/embed/notebook.py
--rw-r--r--   0 runner    (1001) docker     (122)    12506 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/embed/server.py
--rw-r--r--   0 runner    (1001) docker     (122)    17716 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/embed/standalone.py
--rw-r--r--   0 runner    (1001) docker     (122)    14837 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/embed/util.py
--rw-r--r--   0 runner    (1001) docker     (122)     2453 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/embed/wrappers.py
--rw-r--r--   0 runner    (1001) docker     (122)    23182 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/events.py
--rw-r--r--   0 runner    (1001) docker     (122)     3844 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/ext.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 22:10:12.818561 bokeh-3.2.0.dev3/src/bokeh/io/
--rw-r--r--   0 runner    (1001) docker     (122)     2208 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3375 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/io/doc.py
--rw-r--r--   0 runner    (1001) docker     (122)    19285 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/io/export.py
--rw-r--r--   0 runner    (1001) docker     (122)    21518 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/io/notebook.py
--rw-r--r--   0 runner    (1001) docker     (122)     5047 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/io/output.py
--rw-r--r--   0 runner    (1001) docker     (122)     6251 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/io/saving.py
--rw-r--r--   0 runner    (1001) docker     (122)     8278 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/io/showing.py
--rw-r--r--   0 runner    (1001) docker     (122)     8360 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/io/state.py
--rw-r--r--   0 runner    (1001) docker     (122)     4155 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/io/util.py
--rw-r--r--   0 runner    (1001) docker     (122)     6093 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/io/webdriver.py
--rw-r--r--   0 runner    (1001) docker     (122)    23032 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/layouts.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 22:10:12.818561 bokeh-3.2.0.dev3/src/bokeh/model/
--rw-r--r--   0 runner    (1001) docker     (122)     1876 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2053 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/model/data_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     4140 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/model/docs.py
--rw-r--r--   0 runner    (1001) docker     (122)    21253 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/model/model.py
--rw-r--r--   0 runner    (1001) docker     (122)     7839 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/model/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 22:10:12.822561 bokeh-3.2.0.dev3/src/bokeh/models/
--rw-r--r--   0 runner    (1001) docker     (122)     4057 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 22:10:12.822561 bokeh-3.2.0.dev3/src/bokeh/models/annotations/
--rw-r--r--   0 runner    (1001) docker     (122)     2109 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/models/annotations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2590 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/models/annotations/annotation.py
--rw-r--r--   0 runner    (1001) docker     (122)     5564 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/models/annotations/arrows.py
--rw-r--r--   0 runner    (1001) docker     (122)    13775 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/models/annotations/geometry.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 22:10:12.822561 bokeh-3.2.0.dev3/src/bokeh/models/annotations/html/
--rw-r--r--   0 runner    (1001) docker     (122)     1950 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/models/annotations/html/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2265 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/models/annotations/html/html_annotation.py
--rw-r--r--   0 runner    (1001) docker     (122)    10444 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/models/annotations/html/labels.py
--rw-r--r--   0 runner    (1001) docker     (122)     2093 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/models/annotations/html/toolbars.py
--rw-r--r--   0 runner    (1001) docker     (122)     9340 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/models/annotations/labels.py
--rw-r--r--   0 runner    (1001) docker     (122)    16806 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/models/annotations/legends.py
--rw-r--r--   0 runner    (1001) docker     (122)    12456 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/models/axes.py
--rw-r--r--   0 runner    (1001) docker     (122)     5629 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/models/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (122)     2363 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/models/canvas.py
--rw-r--r--   0 runner    (1001) docker     (122)     3154 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/models/coordinates.py
--rw-r--r--   0 runner    (1001) docker     (122)    16739 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/models/css.py
--rw-r--r--   0 runner    (1001) docker     (122)     6881 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/models/dom.py
--rw-r--r--   0 runner    (1001) docker     (122)     9495 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/models/expressions.py
--rw-r--r--   0 runner    (1001) docker     (122)     8487 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/models/filters.py
--rw-r--r--   0 runner    (1001) docker     (122)    24516 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/models/formatters.py
--rw-r--r--   0 runner    (1001) docker     (122)     4197 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/models/glyph.py
--rw-r--r--   0 runner    (1001) docker     (122)    54279 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/models/glyphs.py
--rw-r--r--   0 runner    (1001) docker     (122)     2616 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/models/graphics.py
--rw-r--r--   0 runner    (1001) docker     (122)     6435 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/models/graphs.py
--rw-r--r--   0 runner    (1001) docker     (122)     4263 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/models/grids.py
--rw-r--r--   0 runner    (1001) docker     (122)     4008 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/models/labeling.py
--rw-r--r--   0 runner    (1001) docker     (122)    23128 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/models/layouts.py
--rw-r--r--   0 runner    (1001) docker     (122)     7304 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/models/map_plots.py
--rw-r--r--   0 runner    (1001) docker     (122)    12636 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/models/mappers.py
--rw-r--r--   0 runner    (1001) docker     (122)    33674 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/models/plots.py
--rw-r--r--   0 runner    (1001) docker     (122)    17571 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/models/ranges.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 22:10:12.822561 bokeh-3.2.0.dev3/src/bokeh/models/renderers/
--rw-r--r--   0 runner    (1001) docker     (122)     2101 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/models/renderers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4996 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/models/renderers/contour_renderer.py
--rw-r--r--   0 runner    (1001) docker     (122)     8796 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/models/renderers/glyph_renderer.py
--rw-r--r--   0 runner    (1001) docker     (122)     4366 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/models/renderers/graph_renderer.py
--rw-r--r--   0 runner    (1001) docker     (122)     4219 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/models/renderers/renderer.py
--rw-r--r--   0 runner    (1001) docker     (122)     2613 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/models/renderers/tile_renderer.py
--rw-r--r--   0 runner    (1001) docker     (122)     3815 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/models/scales.py
--rw-r--r--   0 runner    (1001) docker     (122)     4923 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/models/selections.py
--rw-r--r--   0 runner    (1001) docker     (122)     3711 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/models/selectors.py
--rw-r--r--   0 runner    (1001) docker     (122)    33223 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/models/sources.py
--rw-r--r--   0 runner    (1001) docker     (122)     4673 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/models/text.py
--rw-r--r--   0 runner    (1001) docker     (122)     2827 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/models/textures.py
--rw-r--r--   0 runner    (1001) docker     (122)    11476 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/models/tickers.py
--rw-r--r--   0 runner    (1001) docker     (122)     6596 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/models/tiles.py
--rw-r--r--   0 runner    (1001) docker     (122)    72345 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/models/tools.py
--rw-r--r--   0 runner    (1001) docker     (122)     9422 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/models/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 22:10:12.822561 bokeh-3.2.0.dev3/src/bokeh/models/ui/
--rw-r--r--   0 runner    (1001) docker     (122)     2153 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/models/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2548 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/models/ui/dialogs.py
--rw-r--r--   0 runner    (1001) docker     (122)     2275 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/models/ui/examiner.py
--rw-r--r--   0 runner    (1001) docker     (122)     4930 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/models/ui/icons.py
--rw-r--r--   0 runner    (1001) docker     (122)     3706 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/models/ui/menus.py
--rw-r--r--   0 runner    (1001) docker     (122)     2095 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/models/ui/panes.py
--rw-r--r--   0 runner    (1001) docker     (122)     3913 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/models/ui/tooltips.py
--rw-r--r--   0 runner    (1001) docker     (122)     3068 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/models/ui/ui_element.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 22:10:12.826561 bokeh-3.2.0.dev3/src/bokeh/models/util/
--rw-r--r--   0 runner    (1001) docker     (122)      876 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/models/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12432 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/models/util/structure.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 22:10:12.826561 bokeh-3.2.0.dev3/src/bokeh/models/widgets/
--rw-r--r--   0 runner    (1001) docker     (122)     2137 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/models/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7089 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/models/widgets/buttons.py
--rw-r--r--   0 runner    (1001) docker     (122)     4612 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/models/widgets/groups.py
--rw-r--r--   0 runner    (1001) docker     (122)    16135 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/models/widgets/inputs.py
--rw-r--r--   0 runner    (1001) docker     (122)     4680 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/models/widgets/markups.py
--rw-r--r--   0 runner    (1001) docker     (122)    11229 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/models/widgets/pickers.py
--rw-r--r--   0 runner    (1001) docker     (122)    10242 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/models/widgets/sliders.py
--rw-r--r--   0 runner    (1001) docker     (122)    28151 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/models/widgets/tables.py
--rw-r--r--   0 runner    (1001) docker     (122)     2355 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/models/widgets/widget.py
--rw-r--r--   0 runner    (1001) docker     (122)   113099 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/palettes.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 22:10:12.826561 bokeh-3.2.0.dev3/src/bokeh/plotting/
--rw-r--r--   0 runner    (1001) docker     (122)     2533 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3921 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/plotting/_decorators.py
--rw-r--r--   0 runner    (1001) docker     (122)     8267 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/plotting/_docstring.py
--rw-r--r--   0 runner    (1001) docker     (122)    32388 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/plotting/_figure.py
--rw-r--r--   0 runner    (1001) docker     (122)     6603 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/plotting/_graph.py
--rw-r--r--   0 runner    (1001) docker     (122)     5002 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/plotting/_legends.py
--rw-r--r--   0 runner    (1001) docker     (122)     6567 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/plotting/_plot.py
--rw-r--r--   0 runner    (1001) docker     (122)    12625 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/plotting/_renderer.py
--rw-r--r--   0 runner    (1001) docker     (122)     3813 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/plotting/_stack.py
--rw-r--r--   0 runner    (1001) docker     (122)     8078 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/plotting/_tools.py
--rw-r--r--   0 runner    (1001) docker     (122)    14637 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/plotting/contour.py
--rw-r--r--   0 runner    (1001) docker     (122)    27693 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/plotting/glyph_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     4939 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/plotting/gmap.py
--rw-r--r--   0 runner    (1001) docker     (122)     5836 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/plotting/graph.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 22:10:12.826561 bokeh-3.2.0.dev3/src/bokeh/protocol/
--rw-r--r--   0 runner    (1001) docker     (122)     5428 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/protocol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2485 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/protocol/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)    11813 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/protocol/message.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 22:10:12.826561 bokeh-3.2.0.dev3/src/bokeh/protocol/messages/
--rw-r--r--   0 runner    (1001) docker     (122)     2138 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/protocol/messages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2309 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/protocol/messages/ack.py
--rw-r--r--   0 runner    (1001) docker     (122)     3307 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/protocol/messages/error.py
--rw-r--r--   0 runner    (1001) docker     (122)     2467 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/protocol/messages/ok.py
--rw-r--r--   0 runner    (1001) docker     (122)     3754 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/protocol/messages/patch_doc.py
--rw-r--r--   0 runner    (1001) docker     (122)     3176 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/protocol/messages/pull_doc_reply.py
--rw-r--r--   0 runner    (1001) docker     (122)     2334 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/protocol/messages/pull_doc_req.py
--rw-r--r--   0 runner    (1001) docker     (122)     2799 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/protocol/messages/push_doc.py
--rw-r--r--   0 runner    (1001) docker     (122)     3072 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/protocol/messages/server_info_reply.py
--rw-r--r--   0 runner    (1001) docker     (122)     2380 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/protocol/messages/server_info_req.py
--rw-r--r--   0 runner    (1001) docker     (122)     6987 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/protocol/receiver.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)    23830 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 22:10:12.830561 bokeh-3.2.0.dev3/src/bokeh/sampledata/
--rw-r--r--   0 runner    (1001) docker     (122)     2643 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/sampledata/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 22:10:12.834561 bokeh-3.2.0.dev3/src/bokeh/sampledata/_data/
--rw-r--r--   0 runner    (1001) docker     (122)    79935 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/sampledata/_data/USHolidays.ics
--rw-r--r--   0 runner    (1001) docker     (122)   106201 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/sampledata/_data/US_Regions_State_Boundaries.csv.gz
--rw-r--r--   0 runner    (1001) docker     (122)    17444 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/sampledata/_data/auto-mpg.csv
--rw-r--r--   0 runner    (1001) docker     (122)    17345 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/sampledata/_data/auto-mpg2.csv
--rw-r--r--   0 runner    (1001) docker     (122)     2296 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/sampledata/_data/browsers_nov_2013.csv
--rw-r--r--   0 runner    (1001) docker     (122)    25491 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/sampledata/_data/commits.txt.gz
--rw-r--r--   0 runner    (1001) docker     (122)    11342 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/sampledata/_data/daylight_warsaw_2013.csv
--rw-r--r--   0 runner    (1001) docker     (122)    14487 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/sampledata/_data/elements.csv
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 22:10:12.834561 bokeh-3.2.0.dev3/src/bokeh/sampledata/_data/icons/
--rw-r--r--   0 runner    (1001) docker     (122)     1985 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/sampledata/_data/icons/chrome_32x32.png
--rw-r--r--   0 runner    (1001) docker     (122)     2443 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/sampledata/_data/icons/firefox_32x32.png
--rw-r--r--   0 runner    (1001) docker     (122)     2293 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/sampledata/_data/icons/ie_32x32.png
--rw-r--r--   0 runner    (1001) docker     (122)     1666 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/sampledata/_data/icons/opera_32x32.png
--rw-r--r--   0 runner    (1001) docker     (122)     2552 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/sampledata/_data/icons/safari_32x32.png
--rw-r--r--   0 runner    (1001) docker     (122)     3858 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/sampledata/_data/iris.csv
--rw-r--r--   0 runner    (1001) docker     (122)    11536 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/sampledata/_data/les_mis.json
--rw-r--r--   0 runner    (1001) docker     (122)     1390 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/sampledata/_data/numberly.csv
--rw-r--r--   0 runner    (1001) docker     (122)    33264 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/sampledata/_data/obiszow_mtb_xcm.csv
--rw-r--r--   0 runner    (1001) docker     (122)     8630 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/sampledata/_data/olympics2014.json
--rw-r--r--   0 runner    (1001) docker     (122)    13478 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/sampledata/_data/penguins.csv
--rw-r--r--   0 runner    (1001) docker     (122)     5682 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/sampledata/_data/percent-bachelors-degrees-women-usa.csv
--rw-r--r--   0 runner    (1001) docker     (122)     2465 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/sampledata/_data/probly.csv
--rw-r--r--   0 runner    (1001) docker     (122)    14494 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/sampledata/_data/sample_geojson.geojson
--rw-r--r--   0 runner    (1001) docker     (122)    76453 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/sampledata/_data/sea_surface_temperature.csv.gz
--rw-r--r--   0 runner    (1001) docker     (122)     5332 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/sampledata/_data/sprint.csv
--rw-r--r--   0 runner    (1001) docker     (122)     4003 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/sampledata/_data/unemployment1948.csv
--rw-r--r--   0 runner    (1001) docker     (122)     5387 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/sampledata/_data/us_marriages_divorces.csv
--rw-r--r--   0 runner    (1001) docker     (122)     2285 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/sampledata/airport_routes.py
--rw-r--r--   0 runner    (1001) docker     (122)     2761 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/sampledata/airports.py
--rw-r--r--   0 runner    (1001) docker     (122)     3122 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/sampledata/anscombe.py
--rw-r--r--   0 runner    (1001) docker     (122)     3780 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/sampledata/antibiotics.py
--rw-r--r--   0 runner    (1001) docker     (122)     3038 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/sampledata/autompg.py
--rw-r--r--   0 runner    (1001) docker     (122)     2607 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/sampledata/autompg2.py
--rw-r--r--   0 runner    (1001) docker     (122)     3112 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/sampledata/browsers.py
--rw-r--r--   0 runner    (1001) docker     (122)     2498 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/sampledata/commits.py
--rw-r--r--   0 runner    (1001) docker     (122)     2648 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/sampledata/daylight.py
--rw-r--r--   0 runner    (1001) docker     (122)     2192 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/sampledata/degrees.py
--rw-r--r--   0 runner    (1001) docker     (122)     4599 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/sampledata/gapminder.py
--rw-r--r--   0 runner    (1001) docker     (122)     2022 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/sampledata/glucose.py
--rw-r--r--   0 runner    (1001) docker     (122)     2200 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/sampledata/haar_cascade.py
--rw-r--r--   0 runner    (1001) docker     (122)     2371 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/sampledata/iris.py
--rw-r--r--   0 runner    (1001) docker     (122)     2367 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/sampledata/les_mis.py
--rw-r--r--   0 runner    (1001) docker     (122)     2102 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/sampledata/movies_data.py
--rw-r--r--   0 runner    (1001) docker     (122)     2096 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/sampledata/mtb.py
--rw-r--r--   0 runner    (1001) docker     (122)     2224 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/sampledata/olympics2014.py
--rw-r--r--   0 runner    (1001) docker     (122)     2212 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/sampledata/penguins.py
--rw-r--r--   0 runner    (1001) docker     (122)     2270 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/sampledata/perceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     2041 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/sampledata/periodic_table.py
--rw-r--r--   0 runner    (1001) docker     (122)     2548 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/sampledata/population.py
--rw-r--r--   0 runner    (1001) docker     (122)     2071 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/sampledata/sample_geojson.py
--rw-r--r--   0 runner    (1001) docker     (122)     2109 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/sampledata/sample_superstore.py
--rw-r--r--   0 runner    (1001) docker     (122)     2706 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/sampledata/sea_surface_temperature.py
--rw-r--r--   0 runner    (1001) docker     (122)     2066 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/sampledata/sprint.py
--rw-r--r--   0 runner    (1001) docker     (122)     3520 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/sampledata/stocks.py
--rw-r--r--   0 runner    (1001) docker     (122)     2777 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/sampledata/unemployment.py
--rw-r--r--   0 runner    (1001) docker     (122)     2099 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/sampledata/unemployment1948.py
--rw-r--r--   0 runner    (1001) docker     (122)     2116 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/sampledata/us_cities.py
--rw-r--r--   0 runner    (1001) docker     (122)     4032 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/sampledata/us_counties.py
--rw-r--r--   0 runner    (1001) docker     (122)     2888 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/sampledata/us_holidays.py
--rw-r--r--   0 runner    (1001) docker     (122)     2382 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/sampledata/us_marriages_divorces.py
--rw-r--r--   0 runner    (1001) docker     (122)     3703 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/sampledata/us_states.py
--rw-r--r--   0 runner    (1001) docker     (122)     2132 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/sampledata/world_cities.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 22:10:12.834561 bokeh-3.2.0.dev3/src/bokeh/server/
--rw-r--r--   0 runner    (1001) docker     (122)     1468 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9579 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/server/auth_provider.py
--rw-r--r--   0 runner    (1001) docker     (122)     6721 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/server/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (122)     3939 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/server/connection.py
--rw-r--r--   0 runner    (1001) docker     (122)    14606 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/server/contexts.py
--rw-r--r--   0 runner    (1001) docker     (122)     4096 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/server/protocol_handler.py
--rw-r--r--   0 runner    (1001) docker     (122)    20849 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/server/server.py
--rw-r--r--   0 runner    (1001) docker     (122)    11852 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/server/session.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 22:10:12.798561 bokeh-3.2.0.dev3/src/bokeh/server/static/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 22:10:12.846561 bokeh-3.2.0.dev3/src/bokeh/server/static/js/
--rw-r--r--   0 runner    (1001) docker     (122)   211364 2023-05-30 22:09:24.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/bokeh-api.js
--rw-r--r--   0 runner    (1001) docker     (122)   118620 2023-05-30 22:09:24.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/bokeh-api.min.js
--rw-r--r--   0 runner    (1001) docker     (122)   535945 2023-05-30 22:09:24.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/bokeh-gl.js
--rw-r--r--   0 runner    (1001) docker     (122)   198503 2023-05-30 22:09:24.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/bokeh-gl.min.js
--rw-r--r--   0 runner    (1001) docker     (122)  2750420 2023-05-30 22:09:24.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/bokeh-mathjax.js
--rw-r--r--   0 runner    (1001) docker     (122)  1785923 2023-05-30 22:09:24.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/bokeh-mathjax.min.js
--rw-r--r--   0 runner    (1001) docker     (122)   949266 2023-05-30 22:09:24.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/bokeh-tables.js
--rw-r--r--   0 runner    (1001) docker     (122)   302644 2023-05-30 22:09:24.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/bokeh-tables.min.js
--rw-r--r--   0 runner    (1001) docker     (122)   799356 2023-05-30 22:09:24.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/bokeh-widgets.js
--rw-r--r--   0 runner    (1001) docker     (122)   301323 2023-05-30 22:09:24.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/bokeh-widgets.min.js
--rw-r--r--   0 runner    (1001) docker     (122)  2250908 2023-05-30 22:09:24.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/bokeh.js
--rw-r--r--   0 runner    (1001) docker     (122)   956539 2023-05-30 22:09:24.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/bokeh.min.js
--rw-r--r--   0 runner    (1001) docker     (122) 20427536 2023-05-30 22:09:37.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/compiler.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 22:10:12.866561 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 22:10:12.866561 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/api/
--rw-r--r--   0 runner    (1001) docker     (122)     1042 2023-05-30 22:08:51.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/api/charts.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      508 2023-05-30 22:08:52.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/api/expr.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     4471 2023-05-30 22:08:52.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/api/figure.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)    19794 2023-05-30 22:08:52.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/api/glyph_api.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      924 2023-05-30 22:08:52.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/api/gridplot.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      448 2023-05-30 22:08:52.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/api/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      739 2023-05-30 22:08:52.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/api/io.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     3346 2023-05-30 22:08:51.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/api/linalg.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)       59 2023-05-30 22:08:52.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/api/main.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)       63 2023-05-30 22:08:51.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/api/models.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)    63941 2023-05-30 22:08:51.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/api/palettes.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     5394 2023-05-30 22:08:52.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/api/parser.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      206 2023-05-30 22:08:52.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/api/plotting.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      844 2023-05-30 22:08:52.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/api/themes.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      255 2023-05-30 22:08:48.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/base.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      260 2023-05-30 22:08:53.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/bokeh.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 22:10:12.870561 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/client/
--rw-r--r--   0 runner    (1001) docker     (122)     2380 2023-05-30 22:08:48.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/client/connection.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1106 2023-05-30 22:08:48.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/client/session.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 22:10:12.870561 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/
--rw-r--r--   0 runner    (1001) docker     (122)     5846 2023-05-30 22:08:40.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/bokeh_events.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      820 2023-05-30 22:08:43.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/build_views.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      274 2023-05-30 22:08:39.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/class.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)    42976 2023-05-30 22:08:41.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/css.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      334 2023-05-30 22:08:48.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/diagnostics.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     5953 2023-05-30 22:08:41.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/dom.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1548 2023-05-30 22:08:42.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/dom_view.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)    11975 2023-05-30 22:08:40.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/enums.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1062 2023-05-30 22:08:40.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/geometry.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     3638 2023-05-30 22:08:45.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/graphics.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     5113 2023-05-30 22:08:48.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/has_props.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      966 2023-05-30 22:08:43.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/hittest.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     8908 2023-05-30 22:08:40.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/kinds.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 22:10:12.870561 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/layout/
--rw-r--r--   0 runner    (1001) docker     (122)      894 2023-05-30 22:08:42.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/layout/alignments.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      835 2023-05-30 22:08:45.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/layout/border.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     3050 2023-05-30 22:08:42.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/layout/grid.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      321 2023-05-30 22:08:42.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/layout/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1764 2023-05-30 22:08:42.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/layout/layoutable.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1143 2023-05-30 22:08:45.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/layout/side_panel.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1595 2023-05-30 22:08:42.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/layout/types.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1139 2023-05-30 22:08:40.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/logging.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      861 2023-05-30 22:08:47.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/patching.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     9618 2023-05-30 22:08:48.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/properties.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     6764 2023-05-30 22:08:42.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/property_mixins.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      497 2023-05-30 22:08:48.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/resolvers.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      839 2023-05-30 22:08:44.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/selection_manager.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 22:10:12.874560 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/serialization/
--rw-r--r--   0 runner    (1001) docker     (122)      409 2023-05-30 22:08:40.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/serialization/buffer.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2491 2023-05-30 22:08:48.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/serialization/deserializer.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      201 2023-05-30 22:08:40.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/serialization/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2038 2023-05-30 22:08:40.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/serialization/reps.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1766 2023-05-30 22:08:40.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/serialization/serializer.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      376 2023-05-30 22:08:43.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/settings.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1442 2023-05-30 22:08:40.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/signaling.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2971 2023-05-30 22:08:39.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/types.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     6931 2023-05-30 22:08:47.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/ui_events.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1746 2023-05-30 22:08:43.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/uniforms.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 22:10:12.878560 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/util/
--rw-r--r--   0 runner    (1001) docker     (122)     1565 2023-05-30 22:08:41.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/util/affine.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      754 2023-05-30 22:08:49.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/util/algorithms.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2365 2023-05-30 22:08:40.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/util/array.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     4300 2023-05-30 22:08:40.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/util/arrayable.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      243 2023-05-30 22:08:39.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/util/assert.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     3261 2023-05-30 22:08:41.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/util/bbox.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1486 2023-05-30 22:08:39.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/util/bitset.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      298 2023-05-30 22:08:40.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/util/buffer.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1006 2023-05-30 22:08:41.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/util/canvas.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      592 2023-05-30 22:08:48.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/util/cloneable.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      918 2023-05-30 22:08:40.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/util/color.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      236 2023-05-30 22:08:40.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/util/defer.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1275 2023-05-30 22:08:39.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/util/eq.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      152 2023-05-30 22:08:43.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/util/flip_step_mode.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      562 2023-05-30 22:08:45.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/util/image.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      234 2023-05-30 22:08:50.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/util/interpolation.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1332 2023-05-30 22:08:40.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/util/iterator.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1763 2023-05-30 22:08:40.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/util/math.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      737 2023-05-30 22:08:52.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/util/matrix.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1884 2023-05-30 22:08:43.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/util/menus.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      163 2023-05-30 22:08:45.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/util/modules.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     6794 2023-05-30 22:08:44.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/util/ndarray.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2324 2023-05-30 22:08:40.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/util/object.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      287 2023-05-30 22:08:40.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/util/platform.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      865 2023-05-30 22:08:48.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/util/pretty.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1027 2023-05-30 22:08:43.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/util/projections.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      963 2023-05-30 22:08:39.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/util/ragged_array.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      831 2023-05-30 22:08:41.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/util/random.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      253 2023-05-30 22:08:40.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/util/refs.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      254 2023-05-30 22:08:42.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/util/set.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      507 2023-05-30 22:08:47.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/util/slice.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      492 2023-05-30 22:08:43.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/util/spatial.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      499 2023-05-30 22:08:45.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/util/string.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)    11070 2023-05-30 22:08:41.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/util/svg.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     3602 2023-05-30 22:08:39.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/util/svg_colors.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1813 2023-05-30 22:08:46.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/util/templating.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      560 2023-05-30 22:08:45.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/util/text.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      189 2023-05-30 22:08:45.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/util/throttle.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      185 2023-05-30 22:08:47.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/util/typed_array.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1756 2023-05-30 22:08:39.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/util/types.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      101 2023-05-30 22:08:48.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/util/version.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      253 2023-05-30 22:08:43.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/util/wheel.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      713 2023-05-30 22:08:45.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/util/zoom.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1427 2023-05-30 22:08:48.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/vectorization.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2375 2023-05-30 22:08:48.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/view.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 22:10:12.878560 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/visuals/
--rw-r--r--   0 runner    (1001) docker     (122)     1355 2023-05-30 22:08:42.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/visuals/fill.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2400 2023-05-30 22:08:42.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/visuals/hatch.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1165 2023-05-30 22:08:42.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/visuals/image.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      959 2023-05-30 22:08:42.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/visuals/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1947 2023-05-30 22:08:42.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/visuals/line.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      472 2023-05-30 22:08:41.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/visuals/patterns.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2167 2023-05-30 22:08:42.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/visuals/text.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1262 2023-05-30 22:08:42.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/visuals/visual.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 22:10:12.878560 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/document/
--rw-r--r--   0 runner    (1001) docker     (122)     1161 2023-05-30 22:08:48.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/document/defs.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     4788 2023-05-30 22:08:48.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/document/document.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     6205 2023-05-30 22:08:48.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/document/events.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)       89 2023-05-30 22:08:48.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/document/index.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 22:10:12.878560 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/embed/
--rw-r--r--   0 runner    (1001) docker     (122)      287 2023-05-30 22:08:48.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/embed/dom.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      843 2023-05-30 22:08:48.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/embed/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      482 2023-05-30 22:08:48.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/embed/json.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      254 2023-05-30 22:08:48.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/embed/notebook.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      308 2023-05-30 22:08:48.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/embed/server.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      441 2023-05-30 22:08:48.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/embed/standalone.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      446 2023-05-30 22:08:48.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)       83 2023-05-30 22:08:51.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/main.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2140 2023-05-30 22:08:41.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/model.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 22:10:12.878560 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 22:10:12.882560 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/annotations/
--rw-r--r--   0 runner    (1001) docker     (122)     1133 2023-05-30 22:08:45.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/annotations/annotation.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2176 2023-05-30 22:08:48.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/annotations/arrow.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     3573 2023-05-30 22:08:48.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/annotations/arrow_head.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      900 2023-05-30 22:08:48.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/annotations/band.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     4220 2023-05-30 22:08:48.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/annotations/base_color_bar.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     4135 2023-05-30 22:08:46.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/annotations/box_annotation.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2099 2023-05-30 22:08:49.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/annotations/color_bar.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1398 2023-05-30 22:08:49.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/annotations/contour_color_bar.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1100 2023-05-30 22:08:48.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/annotations/data_annotation.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 22:10:12.882560 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/annotations/html/
--rw-r--r--   0 runner    (1001) docker     (122)      153 2023-05-30 22:08:49.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/annotations/html/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1369 2023-05-30 22:08:49.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/annotations/html/label.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2245 2023-05-30 22:08:49.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/annotations/html/label_set.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1191 2023-05-30 22:08:49.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/annotations/html/text_annotation.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1357 2023-05-30 22:08:49.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/annotations/html/title.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1004 2023-05-30 22:08:49.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/annotations/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1145 2023-05-30 22:08:49.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/annotations/label.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1970 2023-05-30 22:08:49.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/annotations/label_set.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     3924 2023-05-30 22:08:49.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/annotations/legend.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      948 2023-05-30 22:08:49.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/annotations/legend_item.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     3650 2023-05-30 22:08:46.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/annotations/poly_annotation.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1159 2023-05-30 22:08:49.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/annotations/slope.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2146 2023-05-30 22:08:46.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/annotations/span.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1699 2023-05-30 22:08:45.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/annotations/text_annotation.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1175 2023-05-30 22:08:45.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/annotations/title.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1283 2023-05-30 22:08:45.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/annotations/toolbar_panel.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1586 2023-05-30 22:08:48.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/annotations/upper_lower.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1443 2023-05-30 22:08:49.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/annotations/whisker.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 22:10:12.882560 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/axes/
--rw-r--r--   0 runner    (1001) docker     (122)     4950 2023-05-30 22:08:47.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/axes/axis.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2312 2023-05-30 22:08:47.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/axes/categorical_axis.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      600 2023-05-30 22:08:47.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/axes/continuous_axis.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      834 2023-05-30 22:08:47.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/axes/datetime_axis.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      350 2023-05-30 22:08:47.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/axes/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      816 2023-05-30 22:08:47.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/axes/linear_axis.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      754 2023-05-30 22:08:47.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/axes/log_axis.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      823 2023-05-30 22:08:47.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/axes/mercator_axis.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 22:10:12.882560 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/callbacks/
--rw-r--r--   0 runner    (1001) docker     (122)      916 2023-05-30 22:08:40.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/callbacks/callback.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      705 2023-05-30 22:08:49.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/callbacks/customjs.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      152 2023-05-30 22:08:49.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/callbacks/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      696 2023-05-30 22:08:49.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/callbacks/open_url.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      604 2023-05-30 22:08:49.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/callbacks/set_value.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 22:10:12.882560 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/canvas/
--rw-r--r--   0 runner    (1001) docker     (122)     2146 2023-05-30 22:08:47.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/canvas/canvas.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1852 2023-05-30 22:08:44.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/canvas/cartesian_frame.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      122 2023-05-30 22:08:49.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/canvas/index.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 22:10:12.882560 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/common/
--rw-r--r--   0 runner    (1001) docker     (122)     3477 2023-05-30 22:08:45.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/common/kinds.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      256 2023-05-30 22:08:46.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/common/painting.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      565 2023-05-30 22:08:45.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/common/resolve.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 22:10:12.882560 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/coordinates/
--rw-r--r--   0 runner    (1001) docker     (122)     2253 2023-05-30 22:08:45.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/coordinates/coordinate_mapping.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)       93 2023-05-30 22:08:49.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/coordinates/index.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 22:10:12.886560 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/dom/
--rw-r--r--   0 runner    (1001) docker     (122)      819 2023-05-30 22:08:46.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/dom/action.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      932 2023-05-30 22:08:51.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/dom/color_ref.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1081 2023-05-30 22:08:46.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/dom/dom_element.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      605 2023-05-30 22:08:46.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/dom/dom_node.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1609 2023-05-30 22:08:51.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/dom/elements.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      936 2023-05-30 22:08:46.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/dom/html.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      708 2023-05-30 22:08:51.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/dom/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      762 2023-05-30 22:08:51.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/dom/index_.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      872 2023-05-30 22:08:46.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/dom/placeholder.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)    16289 2023-05-30 22:08:42.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/dom/styles.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2288 2023-05-30 22:08:42.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/dom/stylesheets.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1050 2023-05-30 22:08:46.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/dom/template.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      641 2023-05-30 22:08:50.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/dom/text.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      902 2023-05-30 22:08:51.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/dom/toggle_group.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      729 2023-05-30 22:08:51.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/dom/value_of.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      836 2023-05-30 22:08:51.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/dom/value_ref.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 22:10:12.886560 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/expressions/
--rw-r--r--   0 runner    (1001) docker     (122)     1972 2023-05-30 22:08:43.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/expressions/coordinate_transform.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      699 2023-05-30 22:08:49.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/expressions/cumsum.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      894 2023-05-30 22:08:49.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/expressions/customjs_expr.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1308 2023-05-30 22:08:43.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/expressions/expression.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      424 2023-05-30 22:08:49.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/expressions/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      662 2023-05-30 22:08:49.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/expressions/maximum.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      662 2023-05-30 22:08:49.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/expressions/minimum.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      850 2023-05-30 22:08:49.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/expressions/polar.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      652 2023-05-30 22:08:49.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/expressions/stack.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 22:10:12.886560 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/filters/
--rw-r--r--   0 runner    (1001) docker     (122)      607 2023-05-30 22:08:44.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/filters/all_indices.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      681 2023-05-30 22:08:49.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/filters/boolean_filter.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      827 2023-05-30 22:08:49.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/filters/customjs_filter.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      694 2023-05-30 22:08:49.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/filters/difference_filter.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      571 2023-05-30 22:08:44.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/filters/filter.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      695 2023-05-30 22:08:49.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/filters/group_filter.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      599 2023-05-30 22:08:49.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/filters/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      725 2023-05-30 22:08:49.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/filters/index_filter.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      708 2023-05-30 22:08:44.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/filters/intersection_filter.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      689 2023-05-30 22:08:49.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/filters/inversion_filter.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      758 2023-05-30 22:08:49.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/filters/symmetric_difference_filter.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      659 2023-05-30 22:08:49.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/filters/union_filter.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 22:10:12.890560 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/formatters/
--rw-r--r--   0 runner    (1001) docker     (122)     1189 2023-05-30 22:08:47.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/formatters/basic_tick_formatter.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      631 2023-05-30 22:08:47.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/formatters/categorical_tick_formatter.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      813 2023-05-30 22:08:48.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/formatters/customjs_tick_formatter.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2021 2023-05-30 22:08:47.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/formatters/datetime_tick_formatter.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      605 2023-05-30 22:08:48.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/formatters/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1078 2023-05-30 22:08:47.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/formatters/log_tick_formatter.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      729 2023-05-30 22:08:47.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/formatters/mercator_tick_formatter.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      820 2023-05-30 22:08:48.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/formatters/numeral_tick_formatter.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      642 2023-05-30 22:08:48.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/formatters/printf_tick_formatter.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      878 2023-05-30 22:08:47.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/formatters/tick_formatter.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 22:10:12.894560 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/
--rw-r--r--   0 runner    (1001) docker     (122)     2365 2023-05-30 22:08:47.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/annular_wedge.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1970 2023-05-30 22:08:47.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/annulus.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1757 2023-05-30 22:08:49.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/arc.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1141 2023-05-30 22:08:43.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/area.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2002 2023-05-30 22:08:49.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/bezier.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1295 2023-05-30 22:08:49.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/block.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1712 2023-05-30 22:08:47.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/center_rotatable.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2604 2023-05-30 22:08:47.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/circle.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      499 2023-05-30 22:08:47.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/defs.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1293 2023-05-30 22:08:49.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/ellipse.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     4094 2023-05-30 22:08:44.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/glyph.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1472 2023-05-30 22:08:43.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/harea.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1747 2023-05-30 22:08:43.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/harea_step.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1286 2023-05-30 22:08:49.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/hbar.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2711 2023-05-30 22:08:47.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/hex_tile.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2076 2023-05-30 22:08:49.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/hspan.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2480 2023-05-30 22:08:49.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/hstrip.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1043 2023-05-30 22:08:50.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/image.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2888 2023-05-30 22:08:46.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/image_base.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      922 2023-05-30 22:08:50.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/image_rgba.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1160 2023-05-30 22:08:50.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/image_stack.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2425 2023-05-30 22:08:45.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/image_url.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1396 2023-05-30 22:08:50.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1591 2023-05-30 22:08:43.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/line.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2559 2023-05-30 22:08:49.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/lrtb.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2220 2023-05-30 22:08:47.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/marker.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2032 2023-05-30 22:08:44.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/multi_line.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2290 2023-05-30 22:08:49.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/multi_polygons.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1478 2023-05-30 22:08:43.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/patch.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2116 2023-05-30 22:08:44.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/patches.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1169 2023-05-30 22:08:50.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/quad.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1892 2023-05-30 22:08:50.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/quadratic.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1379 2023-05-30 22:08:50.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/ray.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2202 2023-05-30 22:08:47.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/rect.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1161 2023-05-30 22:08:47.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/scatter.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2090 2023-05-30 22:08:50.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/segment.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1365 2023-05-30 22:08:50.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/spline.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1399 2023-05-30 22:08:47.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/step.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2543 2023-05-30 22:08:50.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/text.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1307 2023-05-30 22:08:43.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/utils.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1472 2023-05-30 22:08:43.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/varea.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1747 2023-05-30 22:08:43.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/varea_step.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1284 2023-05-30 22:08:50.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/vbar.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2076 2023-05-30 22:08:50.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/vspan.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2480 2023-05-30 22:08:50.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/vstrip.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 22:10:12.898560 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/webgl/
--rw-r--r--   0 runner    (1001) docker     (122)      668 2023-05-30 22:08:47.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/webgl/annular_wedge.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      595 2023-05-30 22:08:47.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/webgl/annulus.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      944 2023-05-30 22:08:43.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/webgl/base.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1553 2023-05-30 22:08:43.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/webgl/base_line.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2179 2023-05-30 22:08:47.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/webgl/base_marker.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1920 2023-05-30 22:08:43.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/webgl/buffer.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      542 2023-05-30 22:08:47.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/webgl/circle.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      552 2023-05-30 22:08:43.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/webgl/dash_cache.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      472 2023-05-30 22:08:47.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/webgl/hex_tile.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      438 2023-05-30 22:08:47.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/webgl/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      700 2023-05-30 22:08:43.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/webgl/line_gl.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      825 2023-05-30 22:08:47.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/webgl/lrtb.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)       52 2023-05-30 22:08:51.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/webgl/main.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)       53 2023-05-30 22:08:37.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/webgl/marker.frag.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)       53 2023-05-30 22:08:37.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/webgl/marker.vert.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      853 2023-05-30 22:08:47.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/webgl/multi_marker.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      452 2023-05-30 22:08:47.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/webgl/rect.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)       53 2023-05-30 22:08:37.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/webgl/regl_line.frag.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)       53 2023-05-30 22:08:37.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/webgl/regl_line.vert.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1310 2023-05-30 22:08:43.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/webgl/regl_wrap.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      930 2023-05-30 22:08:47.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/webgl/single_marker.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      703 2023-05-30 22:08:47.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/webgl/step.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      562 2023-05-30 22:08:47.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/webgl/sxsy.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     3538 2023-05-30 22:08:43.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/webgl/types.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 22:10:12.898560 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/webgl/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      143 2023-05-30 22:08:43.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/webgl/utils/math.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      697 2023-05-30 22:08:43.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/webgl/webgl_utils.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      612 2023-05-30 22:08:47.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/webgl/wedge.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2052 2023-05-30 22:08:47.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/wedge.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1144 2023-05-30 22:08:43.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/xy_glyph.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 22:10:12.898560 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/graphics/
--rw-r--r--   0 runner    (1001) docker     (122)     1123 2023-05-30 22:08:44.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/graphics/decoration.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      115 2023-05-30 22:08:50.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/graphics/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1239 2023-05-30 22:08:44.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/graphics/marking.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 22:10:12.898560 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/graphs/
--rw-r--r--   0 runner    (1001) docker     (122)     5351 2023-05-30 22:08:43.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/graphs/graph_hit_test_policy.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      153 2023-05-30 22:08:50.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/graphs/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2330 2023-05-30 22:08:43.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/graphs/layout_provider.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      933 2023-05-30 22:08:50.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/graphs/static_layout_provider.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 22:10:12.898560 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/grids/
--rw-r--r--   0 runner    (1001) docker     (122)     1926 2023-05-30 22:08:47.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/grids/grid.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)       66 2023-05-30 22:08:50.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/grids/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      875 2023-05-30 22:08:51.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/index.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 22:10:12.898560 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/layouts/
--rw-r--r--   0 runner    (1001) docker     (122)      636 2023-05-30 22:08:50.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/layouts/alignments.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      556 2023-05-30 22:08:50.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/layouts/column.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1190 2023-05-30 22:08:50.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/layouts/css_grid_box.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      981 2023-05-30 22:08:50.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/layouts/flex_box.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1032 2023-05-30 22:08:50.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/layouts/grid_box.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1019 2023-05-30 22:08:50.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/layouts/group_box.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1087 2023-05-30 22:08:50.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/layouts/hbox.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      467 2023-05-30 22:08:50.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/layouts/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     4125 2023-05-30 22:08:43.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/layouts/layout_dom.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      523 2023-05-30 22:08:50.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/layouts/row.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1010 2023-05-30 22:08:50.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/layouts/scroll_box.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      660 2023-05-30 22:08:50.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/layouts/spacer.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      618 2023-05-30 22:08:50.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/layouts/tab_panel.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1288 2023-05-30 22:08:50.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/layouts/tabs.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1087 2023-05-30 22:08:50.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/layouts/vbox.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)       45 2023-05-30 22:08:51.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/main.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 22:10:12.902560 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/mappers/
--rw-r--r--   0 runner    (1001) docker     (122)      891 2023-05-30 22:08:48.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/mappers/categorical_color_mapper.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      866 2023-05-30 22:08:48.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/mappers/categorical_mapper.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      977 2023-05-30 22:08:48.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/mappers/categorical_marker_mapper.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1003 2023-05-30 22:08:48.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/mappers/categorical_pattern_mapper.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1659 2023-05-30 22:08:48.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/mappers/color_mapper.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1888 2023-05-30 22:08:48.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/mappers/continuous_color_mapper.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      807 2023-05-30 22:08:48.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/mappers/eqhist_color_mapper.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      726 2023-05-30 22:08:49.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/mappers/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      892 2023-05-30 22:08:48.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/mappers/linear_color_mapper.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      830 2023-05-30 22:08:48.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/mappers/log_color_mapper.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      668 2023-05-30 22:08:48.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/mappers/mapper.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      993 2023-05-30 22:08:48.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/mappers/scanning_color_mapper.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      498 2023-05-30 22:08:48.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/mappers/stack_color_mapper.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1307 2023-05-30 22:08:49.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/mappers/weighted_stack_color_mapper.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 22:10:12.902560 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/menus/
--rw-r--r--   0 runner    (1001) docker     (122)      819 2023-05-30 22:08:50.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/menus/action.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      612 2023-05-30 22:08:50.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/menus/check_action.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      556 2023-05-30 22:08:50.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/menus/divider.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      221 2023-05-30 22:08:50.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/menus/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1057 2023-05-30 22:08:43.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/menus/menu.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      666 2023-05-30 22:08:43.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/menus/menu_item.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      605 2023-05-30 22:08:50.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/menus/section.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 22:10:12.902560 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/plots/
--rw-r--r--   0 runner    (1001) docker     (122)      604 2023-05-30 22:08:50.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/plots/figure.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      609 2023-05-30 22:08:50.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/plots/gmap.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1568 2023-05-30 22:08:50.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/plots/gmap_plot.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1531 2023-05-30 22:08:50.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/plots/gmap_plot_canvas.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1954 2023-05-30 22:08:50.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/plots/grid_plot.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      297 2023-05-30 22:08:50.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/plots/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     4499 2023-05-30 22:08:47.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/plots/plot.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     4940 2023-05-30 22:08:46.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/plots/plot_canvas.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1234 2023-05-30 22:08:45.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/plots/range_manager.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1274 2023-05-30 22:08:45.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/plots/state_manager.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 22:10:12.902560 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/policies/
--rw-r--r--   0 runner    (1001) docker     (122)       63 2023-05-30 22:08:50.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/policies/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2207 2023-05-30 22:08:47.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/policies/labeling.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 22:10:12.902560 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/random/
--rw-r--r--   0 runner    (1001) docker     (122)       86 2023-05-30 22:08:50.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/random/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      630 2023-05-30 22:08:50.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/random/park_miller_lcg.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      573 2023-05-30 22:08:50.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/random/random_generator.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 22:10:12.902560 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/ranges/
--rw-r--r--   0 runner    (1001) docker     (122)      553 2023-05-30 22:08:44.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/ranges/data_range.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2363 2023-05-30 22:08:44.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/ranges/data_range1d.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     3167 2023-05-30 22:08:48.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/ranges/factor_range.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      239 2023-05-30 22:08:48.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/ranges/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      956 2023-05-30 22:08:48.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/ranges/range.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      826 2023-05-30 22:08:43.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/ranges/range1d.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 22:10:12.902560 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/renderers/
--rw-r--r--   0 runner    (1001) docker     (122)     1467 2023-05-30 22:08:50.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/renderers/contour_renderer.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1306 2023-05-30 22:08:44.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/renderers/data_renderer.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2946 2023-05-30 22:08:44.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/renderers/glyph_renderer.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1809 2023-05-30 22:08:44.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/renderers/graph_renderer.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      687 2023-05-30 22:08:47.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/renderers/guide_renderer.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      293 2023-05-30 22:08:50.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/renderers/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2714 2023-05-30 22:08:47.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/renderers/renderer.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 22:10:12.906560 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/scales/
--rw-r--r--   0 runner    (1001) docker     (122)      669 2023-05-30 22:08:43.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/scales/categorical_scale.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      473 2023-05-30 22:08:43.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/scales/continuous_scale.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      337 2023-05-30 22:08:48.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/scales/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1069 2023-05-30 22:08:48.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/scales/linear_interpolation_scale.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      604 2023-05-30 22:08:43.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/scales/linear_scale.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      679 2023-05-30 22:08:43.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/scales/log_scale.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1109 2023-05-30 22:08:43.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/scales/scale.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 22:10:12.906560 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/selections/
--rw-r--r--   0 runner    (1001) docker     (122)      114 2023-05-30 22:08:50.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/selections/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      982 2023-05-30 22:08:44.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/selections/interaction_policy.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1607 2023-05-30 22:08:43.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/selections/selection.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 22:10:12.906560 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/selectors/
--rw-r--r--   0 runner    (1001) docker     (122)      459 2023-05-30 22:08:50.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/selectors/by_class.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      445 2023-05-30 22:08:50.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/selectors/by_css.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      438 2023-05-30 22:08:50.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/selectors/by_id.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      459 2023-05-30 22:08:50.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/selectors/by_xpath.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      177 2023-05-30 22:08:50.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/selectors/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      520 2023-05-30 22:08:46.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/selectors/selector.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 22:10:12.906560 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/sources/
--rw-r--r--   0 runner    (1001) docker     (122)     1212 2023-05-30 22:08:50.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/sources/ajax_data_source.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1525 2023-05-30 22:08:44.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/sources/cds_view.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      901 2023-05-30 22:08:47.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/sources/column_data_source.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1541 2023-05-30 22:08:44.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/sources/columnar_data_source.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      558 2023-05-30 22:08:44.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/sources/data_source.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1179 2023-05-30 22:08:50.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/sources/geojson_data_source.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      464 2023-05-30 22:08:50.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/sources/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      582 2023-05-30 22:08:50.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/sources/server_sent_data_source.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1138 2023-05-30 22:08:50.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/sources/web_data_source.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 22:10:12.906560 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/text/
--rw-r--r--   0 runner    (1001) docker     (122)      797 2023-05-30 22:08:45.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/text/base_text.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      137 2023-05-30 22:08:50.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/text/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     4357 2023-05-30 22:08:45.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/text/math_text.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 22:10:12.906560 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/text/mathjax/
--rw-r--r--   0 runner    (1001) docker     (122)      361 2023-05-30 22:08:45.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/text/mathjax/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)       52 2023-05-30 22:08:53.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/text/mathjax/main.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      666 2023-05-30 22:08:45.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/text/plain_text.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      839 2023-05-30 22:08:45.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/text/providers.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      152 2023-05-30 22:08:45.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/text/utils.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 22:10:12.906560 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/textures/
--rw-r--r--   0 runner    (1001) docker     (122)      719 2023-05-30 22:08:50.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/textures/canvas_texture.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      771 2023-05-30 22:08:50.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/textures/image_url_texture.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      177 2023-05-30 22:08:50.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/textures/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      766 2023-05-30 22:08:41.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/textures/texture.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 22:10:12.910560 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tickers/
--rw-r--r--   0 runner    (1001) docker     (122)      905 2023-05-30 22:08:47.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tickers/adaptive_ticker.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      465 2023-05-30 22:08:47.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tickers/basic_ticker.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      817 2023-05-30 22:08:48.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tickers/binned_ticker.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      797 2023-05-30 22:08:47.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tickers/categorical_ticker.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1051 2023-05-30 22:08:47.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tickers/composite_ticker.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1170 2023-05-30 22:08:47.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tickers/continuous_ticker.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      490 2023-05-30 22:08:47.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tickers/datetime_ticker.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      757 2023-05-30 22:08:47.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tickers/days_ticker.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      959 2023-05-30 22:08:48.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tickers/fixed_ticker.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      779 2023-05-30 22:08:48.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tickers/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      620 2023-05-30 22:08:47.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tickers/log_ticker.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      999 2023-05-30 22:08:47.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tickers/mercator_ticker.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      773 2023-05-30 22:08:47.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tickers/months_ticker.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1222 2023-05-30 22:08:47.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tickers/single_interval_ticker.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      623 2023-05-30 22:08:47.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tickers/ticker.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      495 2023-05-30 22:08:47.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tickers/util.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      787 2023-05-30 22:08:47.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tickers/years_ticker.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 22:10:12.910560 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tiles/
--rw-r--r--   0 runner    (1001) docker     (122)      615 2023-05-30 22:08:50.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tiles/bbox_tile_source.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      404 2023-05-30 22:08:50.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tiles/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2788 2023-05-30 22:08:50.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tiles/mercator_tile_source.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      585 2023-05-30 22:08:50.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tiles/quadkey_tile_source.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2434 2023-05-30 22:08:50.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tiles/tile_renderer.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2277 2023-05-30 22:08:50.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tiles/tile_source.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      486 2023-05-30 22:08:50.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tiles/tile_utils.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      557 2023-05-30 22:08:50.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tiles/tms_tile_source.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      564 2023-05-30 22:08:50.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tiles/wmts_tile_source.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 22:10:12.910560 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tools/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 22:10:12.914560 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tools/actions/
--rw-r--r--   0 runner    (1001) docker     (122)      903 2023-05-30 22:08:44.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tools/actions/action_tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      653 2023-05-30 22:08:51.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tools/actions/copy_tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      805 2023-05-30 22:08:51.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tools/actions/custom_action.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      867 2023-05-30 22:08:51.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tools/actions/examine_tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      686 2023-05-30 22:08:51.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tools/actions/fullscreen_tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      674 2023-05-30 22:08:44.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tools/actions/help_tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      559 2023-05-30 22:08:51.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tools/actions/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      760 2023-05-30 22:08:46.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tools/actions/plot_action_tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      680 2023-05-30 22:08:46.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tools/actions/redo_tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      661 2023-05-30 22:08:46.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tools/actions/reset_tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      864 2023-05-30 22:08:46.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tools/actions/save_tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      680 2023-05-30 22:08:46.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tools/actions/undo_tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      913 2023-05-30 22:08:46.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tools/actions/zoom_base_tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      552 2023-05-30 22:08:46.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tools/actions/zoom_in_tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      766 2023-05-30 22:08:46.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tools/actions/zoom_out_tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      748 2023-05-30 22:08:44.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tools/click_button.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 22:10:12.914560 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tools/edit/
--rw-r--r--   0 runner    (1001) docker     (122)     1820 2023-05-30 22:08:51.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tools/edit/box_edit_tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1873 2023-05-30 22:08:51.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tools/edit/edit_tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1098 2023-05-30 22:08:51.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tools/edit/freehand_draw_tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      417 2023-05-30 22:08:51.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tools/edit/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1466 2023-05-30 22:08:51.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tools/edit/line_edit_tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1038 2023-05-30 22:08:51.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tools/edit/line_tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1303 2023-05-30 22:08:51.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tools/edit/point_draw_tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1621 2023-05-30 22:08:51.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tools/edit/poly_draw_tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1574 2023-05-30 22:08:51.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tools/edit/poly_edit_tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1288 2023-05-30 22:08:51.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tools/edit/poly_tool.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 22:10:12.914560 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tools/gestures/
--rw-r--r--   0 runner    (1001) docker     (122)     2019 2023-05-30 22:08:46.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tools/gestures/box_select_tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1944 2023-05-30 22:08:46.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tools/gestures/box_zoom_tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      928 2023-05-30 22:08:44.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tools/gestures/gesture_tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      549 2023-05-30 22:08:51.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tools/gestures/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1770 2023-05-30 22:08:46.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tools/gestures/lasso_select_tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1586 2023-05-30 22:08:45.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tools/gestures/pan_tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1900 2023-05-30 22:08:46.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tools/gestures/poly_select_tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1294 2023-05-30 22:08:51.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tools/gestures/range_tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1343 2023-05-30 22:08:46.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tools/gestures/region_select_tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1778 2023-05-30 22:08:46.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tools/gestures/select_tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2003 2023-05-30 22:08:46.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tools/gestures/tap_tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1009 2023-05-30 22:08:45.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tools/gestures/wheel_pan_tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1124 2023-05-30 22:08:45.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tools/gestures/wheel_zoom_tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      391 2023-05-30 22:08:51.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tools/index.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 22:10:12.914560 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tools/inspectors/
--rw-r--r--   0 runner    (1001) docker     (122)     1459 2023-05-30 22:08:46.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tools/inspectors/crosshair_tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      792 2023-05-30 22:08:46.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tools/inspectors/customjs_hover.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     4159 2023-05-30 22:08:46.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tools/inspectors/hover_tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      223 2023-05-30 22:08:51.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tools/inspectors/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      841 2023-05-30 22:08:44.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tools/inspectors/inspect_tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      709 2023-05-30 22:08:44.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tools/on_off_button.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     4774 2023-05-30 22:08:46.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tools/tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1225 2023-05-30 22:08:45.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tools/tool_button.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1492 2023-05-30 22:08:44.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tools/tool_proxy.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     4551 2023-05-30 22:08:45.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tools/toolbar.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 22:10:12.918560 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/transforms/
--rw-r--r--   0 runner    (1001) docker     (122)      978 2023-05-30 22:08:50.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/transforms/customjs_transform.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      510 2023-05-30 22:08:50.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/transforms/dodge.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      365 2023-05-30 22:08:50.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/transforms/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1012 2023-05-30 22:08:50.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/transforms/interpolator.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1192 2023-05-30 22:08:50.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/transforms/jitter.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      537 2023-05-30 22:08:50.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/transforms/linear_interpolator.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      831 2023-05-30 22:08:50.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/transforms/range_transform.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      614 2023-05-30 22:08:50.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/transforms/step_interpolator.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      628 2023-05-30 22:08:43.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/transforms/transform.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 22:10:12.918560 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/ui/
--rw-r--r--   0 runner    (1001) docker     (122)     1317 2023-05-30 22:08:50.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/ui/dialog.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1685 2023-05-30 22:08:51.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/ui/examiner.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 22:10:12.918560 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/ui/icons/
--rw-r--r--   0 runner    (1001) docker     (122)      905 2023-05-30 22:08:50.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/ui/icons/builtin_icon.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      623 2023-05-30 22:08:50.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/ui/icons/icon.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      163 2023-05-30 22:08:50.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/ui/icons/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      775 2023-05-30 22:08:50.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/ui/icons/svg_icon.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1067 2023-05-30 22:08:50.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/ui/icons/tabler_icon.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      244 2023-05-30 22:08:51.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/ui/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1107 2023-05-30 22:08:51.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/ui/pane.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1754 2023-05-30 22:08:46.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/ui/tooltip.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2704 2023-05-30 22:08:43.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/ui/ui_element.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      208 2023-05-30 22:08:44.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/util.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 22:10:12.922560 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/
--rw-r--r--   0 runner    (1001) docker     (122)     1432 2023-05-30 22:08:52.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/abstract_button.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2666 2023-05-30 22:08:52.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/abstract_slider.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1826 2023-05-30 22:08:52.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/autocomplete_input.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1648 2023-05-30 22:08:52.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/base_date_picker.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1166 2023-05-30 22:08:52.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/base_datetime_picker.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      752 2023-05-30 22:08:52.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/button.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      946 2023-05-30 22:08:52.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/checkbox.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      866 2023-05-30 22:08:52.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/checkbox_button_group.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      810 2023-05-30 22:08:52.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/checkbox_group.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      761 2023-05-30 22:08:52.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/color_picker.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      655 2023-05-30 22:08:52.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/control.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      798 2023-05-30 22:08:52.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/date_picker.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      861 2023-05-30 22:08:52.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/date_range_picker.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      952 2023-05-30 22:08:52.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/date_range_slider.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      890 2023-05-30 22:08:52.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/date_slider.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      904 2023-05-30 22:08:52.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/datetime_picker.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      962 2023-05-30 22:08:52.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/datetime_range_picker.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      901 2023-05-30 22:08:52.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/datetime_range_slider.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      558 2023-05-30 22:08:52.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/div.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1188 2023-05-30 22:08:52.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/dropdown.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1057 2023-05-30 22:08:52.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/file_input.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      940 2023-05-30 22:08:52.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/help_button.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1884 2023-05-30 22:08:53.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1454 2023-05-30 22:08:52.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/input_widget.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)       90 2023-05-30 22:08:53.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/main.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      998 2023-05-30 22:08:52.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/markup.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1311 2023-05-30 22:08:52.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/multi_choice.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      923 2023-05-30 22:08:52.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/multiple_date_picker.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1024 2023-05-30 22:08:52.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/multiple_datetime_picker.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      873 2023-05-30 22:08:52.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/multiselect.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1403 2023-05-30 22:08:52.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/numeric_input.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      732 2023-05-30 22:08:52.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/oriented_control.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      563 2023-05-30 22:08:52.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/paragraph.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      742 2023-05-30 22:08:52.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/password_input.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1246 2023-05-30 22:08:52.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/picker_base.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      543 2023-05-30 22:08:52.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/pretext.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      810 2023-05-30 22:08:52.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/radio_button_group.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      754 2023-05-30 22:08:52.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/radio_group.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      820 2023-05-30 22:08:52.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/range_slider.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      969 2023-05-30 22:08:52.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/selectbox.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      758 2023-05-30 22:08:52.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/slider.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1492 2023-05-30 22:08:52.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/spinner.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      833 2023-05-30 22:08:53.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/switch.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 22:10:12.926560 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/tables/
--rw-r--r--   0 runner    (1001) docker     (122)     6181 2023-05-30 22:08:53.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/tables/cell_editors.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     4072 2023-05-30 22:08:53.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/tables/cell_formatters.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2397 2023-05-30 22:08:53.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/tables/data_cube.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     3920 2023-05-30 22:08:53.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/tables/data_table.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      355 2023-05-30 22:08:53.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/tables/definitions.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      386 2023-05-30 22:08:53.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/tables/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)       88 2023-05-30 22:08:53.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/tables/main.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1697 2023-05-30 22:08:53.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/tables/row_aggregators.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      980 2023-05-30 22:08:53.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/tables/table_column.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      646 2023-05-30 22:08:53.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/tables/table_widget.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      859 2023-05-30 22:08:52.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/text_input.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1013 2023-05-30 22:08:52.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/text_like_input.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      834 2023-05-30 22:08:53.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/textarea_input.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1457 2023-05-30 22:08:52.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/time_picker.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      715 2023-05-30 22:08:53.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/toggle.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1199 2023-05-30 22:08:52.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/toggle_button_group.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      792 2023-05-30 22:08:52.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/toggle_input.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      996 2023-05-30 22:08:52.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/toggle_input_group.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      879 2023-05-30 22:08:52.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/widget.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 22:10:12.926560 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/protocol/
--rw-r--r--   0 runner    (1001) docker     (122)       90 2023-05-30 22:08:48.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/protocol/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      975 2023-05-30 22:08:48.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/protocol/message.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      736 2023-05-30 22:08:48.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/protocol/receiver.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      117 2023-05-30 22:08:48.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/safely.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 22:10:12.926560 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/styles/
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-05-30 22:08:37.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/styles/attribution.css.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-05-30 22:08:37.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/styles/base.css.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      396 2023-05-30 22:08:37.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/styles/buttons.css.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)       73 2023-05-30 22:08:37.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/styles/canvas.css.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      148 2023-05-30 22:08:37.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/styles/caret.css.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)       48 2023-05-30 22:08:37.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/styles/clearfix.css.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      130 2023-05-30 22:08:37.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/styles/dialogs.css.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      155 2023-05-30 22:08:37.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/styles/dropdown.css.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-05-30 22:08:37.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/styles/examiner.css.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-05-30 22:08:37.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/styles/group_box.css.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2067 2023-05-30 22:08:37.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/styles/icons.css.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      102 2023-05-30 22:08:37.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/styles/logo.css.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      168 2023-05-30 22:08:37.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/styles/menus.css.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)       46 2023-05-30 22:08:37.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/styles/plots.css.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      263 2023-05-30 22:08:37.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/styles/tabs.css.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      248 2023-05-30 22:08:37.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/styles/tool_button.css.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      332 2023-05-30 22:08:37.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/styles/toolbar.css.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      380 2023-05-30 22:08:37.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/styles/tooltips.css.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-05-30 22:08:37.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/styles/ui.css.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 22:10:12.926560 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/styles/widgets/
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-05-30 22:08:37.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/styles/widgets/checkbox.css.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-05-30 22:08:37.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/styles/widgets/choices.css.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-05-30 22:08:37.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/styles/widgets/flatpickr.css.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      430 2023-05-30 22:08:37.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/styles/widgets/inputs.css.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-05-30 22:08:37.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/styles/widgets/nouislider.css.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      102 2023-05-30 22:08:37.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/styles/widgets/password_input.css.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-05-30 22:08:37.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/styles/widgets/slickgrid.css.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)       86 2023-05-30 22:08:37.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/styles/widgets/sliders.css.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-05-30 22:08:37.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/styles/widgets/switch.css.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      269 2023-05-30 22:08:37.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/styles/widgets/tables.css.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      303 2023-05-30 22:08:48.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/testing.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-30 22:08:37.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/version.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 22:10:12.938560 bokeh-3.2.0.dev3/src/bokeh/server/static/lib/
--rw-r--r--   0 runner    (1001) docker     (122)    12714 2023-05-30 22:10:12.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.decorators.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1326 2023-05-30 22:10:12.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.decorators.legacy.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)   824027 2023-05-30 22:10:12.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.dom.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)    16886 2023-05-30 22:10:12.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.dom.iterable.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     5203 2023-05-30 22:10:12.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2015.collection.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)    21204 2023-05-30 22:10:12.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2015.core.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1241 2023-05-30 22:10:12.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2015.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2552 2023-05-30 22:10:12.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2015.generator.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)    14892 2023-05-30 22:10:12.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2015.iterable.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     3199 2023-05-30 22:10:12.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2015.promise.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     5251 2023-05-30 22:10:12.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2015.proxy.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     6493 2023-05-30 22:10:12.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2015.reflect.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1648 2023-05-30 22:10:12.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2015.symbol.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)    10621 2023-05-30 22:10:12.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2015.symbol.wellknown.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     4861 2023-05-30 22:10:12.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2016.array.include.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      928 2023-05-30 22:10:12.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2016.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1031 2023-05-30 22:10:12.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2016.full.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1083 2023-05-30 22:10:12.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2017.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1031 2023-05-30 22:10:12.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2017.full.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1439 2023-05-30 22:10:12.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2017.intl.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2451 2023-05-30 22:10:12.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2017.object.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     6227 2023-05-30 22:10:12.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2017.sharedmemory.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2378 2023-05-30 22:10:12.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2017.string.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1425 2023-05-30 22:10:12.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2017.typedarrays.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2687 2023-05-30 22:10:12.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2018.asyncgenerator.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1753 2023-05-30 22:10:12.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2018.asynciterable.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1088 2023-05-30 22:10:12.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2018.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1031 2023-05-30 22:10:12.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2018.full.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     3076 2023-05-30 22:10:12.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2018.intl.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1352 2023-05-30 22:10:12.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2018.promise.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1227 2023-05-30 22:10:12.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2018.regexp.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     3173 2023-05-30 22:10:12.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2019.array.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1071 2023-05-30 22:10:12.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2019.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1032 2023-05-30 22:10:12.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2019.full.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      955 2023-05-30 22:10:12.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2019.intl.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1472 2023-05-30 22:10:12.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2019.object.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1528 2023-05-30 22:10:12.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2019.string.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1006 2023-05-30 22:10:12.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2019.symbol.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)    35366 2023-05-30 22:10:12.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2020.bigint.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1201 2023-05-30 22:10:12.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2020.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2955 2023-05-30 22:10:12.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2020.date.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1032 2023-05-30 22:10:12.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2020.full.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)    20994 2023-05-30 22:10:12.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2020.intl.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1587 2023-05-30 22:10:12.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2020.number.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1802 2023-05-30 22:10:12.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2020.promise.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     4749 2023-05-30 22:10:12.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2020.sharedmemory.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1237 2023-05-30 22:10:12.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2020.string.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1455 2023-05-30 22:10:12.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2020.symbol.wellknown.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1036 2023-05-30 22:10:12.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2021.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1032 2023-05-30 22:10:12.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2021.full.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     8378 2023-05-30 22:10:12.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2021.intl.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2259 2023-05-30 22:10:12.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2021.promise.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1592 2023-05-30 22:10:12.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2021.string.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2739 2023-05-30 22:10:12.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2021.weakref.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     4258 2023-05-30 22:10:12.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2022.array.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1152 2023-05-30 22:10:12.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2022.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2337 2023-05-30 22:10:12.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2022.error.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1032 2023-05-30 22:10:12.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2022.full.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     5563 2023-05-30 22:10:12.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2022.intl.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1085 2023-05-30 22:10:12.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2022.object.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1336 2023-05-30 22:10:12.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2022.regexp.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2081 2023-05-30 22:10:12.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2022.sharedmemory.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1155 2023-05-30 22:10:12.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2022.string.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)    21108 2023-05-30 22:10:12.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2023.array.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      921 2023-05-30 22:10:12.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2023.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1032 2023-05-30 22:10:12.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2023.full.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)   212834 2023-05-30 22:10:12.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es5.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1032 2023-05-30 22:10:12.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es6.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      920 2023-05-30 22:10:12.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.esnext.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1031 2023-05-30 22:10:12.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.esnext.full.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1192 2023-05-30 22:10:12.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.esnext.intl.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     9453 2023-05-30 22:10:12.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.scripthost.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)   273794 2023-05-30 22:10:12.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.webworker.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1042 2023-05-30 22:10:12.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.webworker.importscripts.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)    12132 2023-05-30 22:10:12.000000 bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.webworker.iterable.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)    31831 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/server/tornado.py
--rw-r--r--   0 runner    (1001) docker     (122)     4014 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/server/urls.py
--rw-r--r--   0 runner    (1001) docker     (122)     7787 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/server/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 22:10:12.938560 bokeh-3.2.0.dev3/src/bokeh/server/views/
--rw-r--r--   0 runner    (1001) docker     (122)      331 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/server/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7033 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/server/views/app_index.html
--rw-r--r--   0 runner    (1001) docker     (122)     3207 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/server/views/auth_request_handler.py
--rw-r--r--   0 runner    (1001) docker     (122)     3817 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/server/views/autoload_js_handler.py
--rw-r--r--   0 runner    (1001) docker     (122)    15086 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/server/views/bokeh-dev.ico
--rw-r--r--   0 runner    (1001) docker     (122)    15086 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/server/views/bokeh.ico
--rw-r--r--   0 runner    (1001) docker     (122)     2631 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/server/views/doc_handler.py
--rw-r--r--   0 runner    (1001) docker     (122)     2239 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/server/views/ico_handler.py
--rw-r--r--   0 runner    (1001) docker     (122)     2571 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/server/views/metadata_handler.py
--rw-r--r--   0 runner    (1001) docker     (122)     2871 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/server/views/multi_root_static_handler.py
--rw-r--r--   0 runner    (1001) docker     (122)     2840 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/server/views/root_handler.py
--rw-r--r--   0 runner    (1001) docker     (122)     6493 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/server/views/session_handler.py
--rw-r--r--   0 runner    (1001) docker     (122)     3205 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/server/views/static_handler.py
--rw-r--r--   0 runner    (1001) docker     (122)    13576 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/server/views/ws.py
--rw-r--r--   0 runner    (1001) docker     (122)    26346 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 22:10:12.942560 bokeh-3.2.0.dev3/src/bokeh/sphinxext/
--rw-r--r--   0 runner    (1001) docker     (122)      929 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/sphinxext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 22:10:12.942560 bokeh-3.2.0.dev3/src/bokeh/sphinxext/_templates/
--rw-r--r--   0 runner    (1001) docker     (122)     2608 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/sphinxext/_templates/bokehjs_codepen_init.html
--rw-r--r--   0 runner    (1001) docker     (122)      383 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/sphinxext/_templates/bokehjs_content_epilogue.html
--rw-r--r--   0 runner    (1001) docker     (122)       95 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/sphinxext/_templates/bokehjs_content_prologue.html
--rw-r--r--   0 runner    (1001) docker     (122)      480 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/sphinxext/_templates/bokehjs_html_template.html
--rw-r--r--   0 runner    (1001) docker     (122)      204 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/sphinxext/_templates/color_detail.html
--rw-r--r--   0 runner    (1001) docker     (122)      417 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/sphinxext/_templates/enum_detail.rst
--rw-r--r--   0 runner    (1001) docker     (122)      230 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/sphinxext/_templates/example_metadata.rst
--rw-r--r--   0 runner    (1001) docker     (122)      199 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/sphinxext/_templates/gallery_detail.rst
--rw-r--r--   0 runner    (1001) docker     (122)      641 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/sphinxext/_templates/gallery_page.rst
--rw-r--r--   0 runner    (1001) docker     (122)      314 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/sphinxext/_templates/jinja_detail.rst
--rw-r--r--   0 runner    (1001) docker     (122)      325 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/sphinxext/_templates/model_detail.rst
--rw-r--r--   0 runner    (1001) docker     (122)      153 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/sphinxext/_templates/options_detail.rst
--rw-r--r--   0 runner    (1001) docker     (122)      243 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/sphinxext/_templates/palette_detail.html
--rw-r--r--   0 runner    (1001) docker     (122)      481 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/sphinxext/_templates/palette_group_detail.html
--rw-r--r--   0 runner    (1001) docker     (122)      171 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/sphinxext/_templates/prop_detail.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1269 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/sphinxext/_templates/release_detail.rst
--rw-r--r--   0 runner    (1001) docker     (122)      302 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/sphinxext/_templates/settings_detail.rst
--rw-r--r--   0 runner    (1001) docker     (122)     4320 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/sphinxext/bokeh_autodoc.py
--rw-r--r--   0 runner    (1001) docker     (122)     2912 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/sphinxext/bokeh_color.py
--rw-r--r--   0 runner    (1001) docker     (122)     3465 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/sphinxext/bokeh_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (122)     2725 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/sphinxext/bokeh_directive.py
--rw-r--r--   0 runner    (1001) docker     (122)     4423 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/sphinxext/bokeh_enum.py
--rw-r--r--   0 runner    (1001) docker     (122)     4784 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/sphinxext/bokeh_example_metadata.py
--rw-r--r--   0 runner    (1001) docker     (122)     6570 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/sphinxext/bokeh_gallery.py
--rw-r--r--   0 runner    (1001) docker     (122)     3964 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/sphinxext/bokeh_jinja.py
--rw-r--r--   0 runner    (1001) docker     (122)     6135 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/sphinxext/bokeh_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     4828 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/sphinxext/bokeh_options.py
--rw-r--r--   0 runner    (1001) docker     (122)     4784 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/sphinxext/bokeh_palette.py
--rw-r--r--   0 runner    (1001) docker     (122)     4099 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/sphinxext/bokeh_palette_group.py
--rw-r--r--   0 runner    (1001) docker     (122)    12661 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/sphinxext/bokeh_plot.py
--rw-r--r--   0 runner    (1001) docker     (122)     4988 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/sphinxext/bokeh_prop.py
--rw-r--r--   0 runner    (1001) docker     (122)     3398 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/sphinxext/bokeh_releases.py
--rw-r--r--   0 runner    (1001) docker     (122)     8083 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/sphinxext/bokeh_roles.py
--rw-r--r--   0 runner    (1001) docker     (122)     7577 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/sphinxext/bokeh_sampledata_xref.py
--rw-r--r--   0 runner    (1001) docker     (122)     4275 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/sphinxext/bokeh_settings.py
--rw-r--r--   0 runner    (1001) docker     (122)     3791 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/sphinxext/bokeh_sitemap.py
--rw-r--r--   0 runner    (1001) docker     (122)     9589 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/sphinxext/bokehjs_content.py
--rw-r--r--   0 runner    (1001) docker     (122)     4630 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/sphinxext/example_handler.py
--rw-r--r--   0 runner    (1001) docker     (122)     2600 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/sphinxext/sample.py
--rw-r--r--   0 runner    (1001) docker     (122)     3247 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/sphinxext/templates.py
--rw-r--r--   0 runner    (1001) docker     (122)     3004 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/sphinxext/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 22:10:12.942560 bokeh-3.2.0.dev3/src/bokeh/themes/
--rw-r--r--   0 runner    (1001) docker     (122)     2904 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/themes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2243 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/themes/_caliber.py
--rw-r--r--   0 runner    (1001) docker     (122)     2382 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/themes/_contrast.py
--rw-r--r--   0 runner    (1001) docker     (122)     2382 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/themes/_dark_minimal.py
--rw-r--r--   0 runner    (1001) docker     (122)     1970 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/themes/_light_minimal.py
--rw-r--r--   0 runner    (1001) docker     (122)     2382 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/themes/_night_sky.py
--rw-r--r--   0 runner    (1001) docker     (122)     9267 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/themes/theme.py
--rw-r--r--   0 runner    (1001) docker     (122)     8284 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/tile_providers.py
--rw-r--r--   0 runner    (1001) docker     (122)    14776 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 22:10:12.946560 bokeh-3.2.0.dev3/src/bokeh/util/
--rw-r--r--   0 runner    (1001) docker     (122)     2528 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4707 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/util/browser.py
--rw-r--r--   0 runner    (1001) docker     (122)     7856 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/util/callback_manager.py
--rw-r--r--   0 runner    (1001) docker     (122)    18959 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/util/compiler.py
--rw-r--r--   0 runner    (1001) docker     (122)     2711 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/util/dataclasses.py
--rw-r--r--   0 runner    (1001) docker     (122)     3827 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/util/datatypes.py
--rw-r--r--   0 runner    (1001) docker     (122)     2924 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/util/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (122)     3121 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/util/deprecation.py
--rw-r--r--   0 runner    (1001) docker     (122)     2303 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/util/functions.py
--rw-r--r--   0 runner    (1001) docker     (122)     8426 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/util/hex.py
--rw-r--r--   0 runner    (1001) docker     (122)     3600 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/util/logconfig.py
--rw-r--r--   0 runner    (1001) docker     (122)     3043 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/util/options.py
--rw-r--r--   0 runner    (1001) docker     (122)     4391 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/util/package.py
--rw-r--r--   0 runner    (1001) docker     (122)     2505 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/util/paths.py
--rw-r--r--   0 runner    (1001) docker     (122)     1872 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/util/sampledata.json
--rw-r--r--   0 runner    (1001) docker     (122)     7969 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/util/sampledata.py
--rw-r--r--   0 runner    (1001) docker     (122)    11396 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/util/serialization.py
--rw-r--r--   0 runner    (1001) docker     (122)     5419 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/util/strings.py
--rw-r--r--   0 runner    (1001) docker     (122)     3646 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/util/terminal.py
--rw-r--r--   0 runner    (1001) docker     (122)    12872 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/util/token.py
--rw-r--r--   0 runner    (1001) docker     (122)    11285 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/util/tornado.py
--rw-r--r--   0 runner    (1001) docker     (122)     2944 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/util/version.py
--rw-r--r--   0 runner    (1001) docker     (122)     3153 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/src/bokeh/util/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 22:10:12.802561 bokeh-3.2.0.dev3/src/bokeh.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    12082 2023-05-30 22:10:12.000000 bokeh-3.2.0.dev3/src/bokeh.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    55013 2023-05-30 22:10:12.000000 bokeh-3.2.0.dev3/src/bokeh.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-30 22:10:12.000000 bokeh-3.2.0.dev3/src/bokeh.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       46 2023-05-30 22:10:12.000000 bokeh-3.2.0.dev3/src/bokeh.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      128 2023-05-30 22:10:12.000000 bokeh-3.2.0.dev3/src/bokeh.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       14 2023-05-30 22:10:12.000000 bokeh-3.2.0.dev3/src/bokeh.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 22:10:12.946560 bokeh-3.2.0.dev3/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     2002 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/tests/test_bokehjs.py
--rw-r--r--   0 runner    (1001) docker     (122)     6178 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/tests/test_cross.py
--rw-r--r--   0 runner    (1001) docker     (122)     2588 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/tests/test_defaults.py
--rw-r--r--   0 runner    (1001) docker     (122)    10468 2023-05-30 22:01:46.000000 bokeh-3.2.0.dev3/tests/test_examples.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:29.010450 bokeh-3.2.0.dev4/
+-rw-r--r--   0 runner    (1001) docker     (122)     1494 2023-06-09 10:22:42.000000 bokeh-3.2.0.dev4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      881 2023-06-09 10:22:42.000000 bokeh-3.2.0.dev4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    12082 2023-06-09 10:33:29.010450 bokeh-3.2.0.dev4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     8603 2023-06-09 10:22:42.000000 bokeh-3.2.0.dev4/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)    10430 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-09 10:33:29.010450 bokeh-3.2.0.dev4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     6745 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.822447 bokeh-3.2.0.dev4/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.834447 bokeh-3.2.0.dev4/src/bokeh/
+-rw-r--r--   0 runner    (1001) docker     (122)     1494 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     3750 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2136 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    73110 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/_sri.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.834447 bokeh-3.2.0.dev4/src/bokeh/application/
+-rw-r--r--   0 runner    (1001) docker     (122)     2145 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/application/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11549 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/application/application.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.838447 bokeh-3.2.0.dev4/src/bokeh/application/handlers/
+-rw-r--r--   0 runner    (1001) docker     (122)     2194 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/application/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6919 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/application/handlers/code.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7818 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/application/handlers/code_runner.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10926 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/application/handlers/directory.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2882 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/application/handlers/document_lifecycle.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4943 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/application/handlers/function.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7975 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/application/handlers/handler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4705 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/application/handlers/lifecycle.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5180 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/application/handlers/notebook.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2921 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/application/handlers/request_handler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3348 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/application/handlers/script.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5035 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/application/handlers/server_lifecycle.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4339 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/application/handlers/server_request_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.838447 bokeh-3.2.0.dev4/src/bokeh/client/
+-rw-r--r--   0 runner    (1001) docker     (122)     2373 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16199 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/client/connection.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21727 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/client/session.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5334 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/client/states.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3299 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/client/util.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3252 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/client/websocket.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.838447 bokeh-3.2.0.dev4/src/bokeh/colors/
+-rw-r--r--   0 runner    (1001) docker     (122)     1948 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/colors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14039 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/colors/color.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9825 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/colors/groups.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13046 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/colors/named.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5432 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/colors/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.838447 bokeh-3.2.0.dev4/src/bokeh/command/
+-rw-r--r--   0 runner    (1001) docker     (122)      901 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3965 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/command/bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5822 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/command/subcommand.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.838447 bokeh-3.2.0.dev4/src/bokeh/command/subcommands/
+-rw-r--r--   0 runner    (1001) docker     (122)     2802 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/command/subcommands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2567 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/command/subcommands/build.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7336 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/command/subcommands/file_output.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4658 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/command/subcommands/info.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2765 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/command/subcommands/init.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3592 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/command/subcommands/json.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2564 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/command/subcommands/sampledata.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2775 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/command/subcommands/secret.py
+-rw-r--r--   0 runner    (1001) docker     (122)    37703 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/command/subcommands/serve.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3764 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/command/subcommands/static.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7996 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/command/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.842447 bokeh-3.2.0.dev4/src/bokeh/core/
+-rw-r--r--   0 runner    (1001) docker     (122)     2140 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.842447 bokeh-3.2.0.dev4/src/bokeh/core/_templates/
+-rw-r--r--   0 runner    (1001) docker     (122)     4349 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/_templates/autoload_js.js
+-rw-r--r--   0 runner    (1001) docker     (122)     6450 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/_templates/autoload_nb_js.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1393 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/_templates/autoload_request_tag.html
+-rw-r--r--   0 runner    (1001) docker     (122)      815 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/_templates/autoload_tag.html
+-rw-r--r--   0 runner    (1001) docker     (122)      469 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/_templates/css_resources.html
+-rw-r--r--   0 runner    (1001) docker     (122)      314 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/_templates/doc_js.js
+-rw-r--r--   0 runner    (1001) docker     (122)      213 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/_templates/doc_nb_js.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1634 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/_templates/file.html
+-rw-r--r--   0 runner    (1001) docker     (122)      586 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/_templates/js_resources.html
+-rw-r--r--   0 runner    (1001) docker     (122)      158 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/_templates/macros.html
+-rw-r--r--   0 runner    (1001) docker     (122)     3933 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/_templates/notebook_load.html
+-rw-r--r--   0 runner    (1001) docker     (122)      356 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/_templates/plot_div.html
+-rw-r--r--   0 runner    (1001) docker     (122)       49 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/_templates/root_div.html
+-rw-r--r--   0 runner    (1001) docker     (122)      260 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/_templates/script_tag.html
+-rw-r--r--   0 runner    (1001) docker     (122)      591 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/_templates/try_run.js
+-rw-r--r--   0 runner    (1001) docker     (122)    16751 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/enums.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29845 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/has_props.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7133 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/json_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11533 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/properties.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.846447 bokeh-3.2.0.dev4/src/bokeh/core/property/
+-rw-r--r--   0 runner    (1001) docker     (122)     1658 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/property/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2782 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/property/_sphinx.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3646 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/property/alias.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1906 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/property/aliases.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3156 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/property/any.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2499 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/property/auto.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20064 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/property/bases.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6436 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/property/color.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12052 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/property/container.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22696 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/property/dataspec.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6091 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/property/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5123 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/property/descriptor_factory.py
+-rw-r--r--   0 runner    (1001) docker     (122)    35217 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/property/descriptors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4198 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/property/either.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3989 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/property/enum.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3021 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/property/factors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2879 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/property/include.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6521 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/property/instance.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2743 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/property/json.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2139 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/property/nothing.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3745 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/property/nullable.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9631 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/property/numeric.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3458 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/property/override.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3251 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/property/pd.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7166 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/property/primitive.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2255 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/property/readonly.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2494 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/property/required.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2536 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/property/serialized.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2351 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/property/singletons.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3465 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/property/string.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3896 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/property/struct.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2481 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/property/text_like.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3378 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/property/validation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5977 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/property/vectorization.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8905 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/property/visual.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17517 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/property/wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3508 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/property_aliases.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12260 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/property_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10171 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/query.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23292 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4892 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/templates.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3025 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/types.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.850448 bokeh-3.2.0.dev4/src/bokeh/core/validation/
+-rw-r--r--   0 runner    (1001) docker     (122)     3502 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7168 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/validation/check.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6555 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/validation/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9259 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/validation/errors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2983 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/validation/issue.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3082 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/core/validation/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.850448 bokeh-3.2.0.dev4/src/bokeh/document/
+-rw-r--r--   0 runner    (1001) docker     (122)     2435 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/document/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16657 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/document/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27922 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/document/document.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29934 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/document/events.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3419 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/document/json.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4978 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/document/locking.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9341 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/document/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5026 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/document/modules.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6344 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/driving.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.850448 bokeh-3.2.0.dev4/src/bokeh/embed/
+-rw-r--r--   0 runner    (1001) docker     (122)     2074 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/embed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14666 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/embed/bundle.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6464 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/embed/elements.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3968 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/embed/notebook.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12506 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/embed/server.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17807 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/embed/standalone.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14837 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/embed/util.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2453 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/embed/wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23182 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/events.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3844 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/ext.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.854447 bokeh-3.2.0.dev4/src/bokeh/io/
+-rw-r--r--   0 runner    (1001) docker     (122)     2208 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3375 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/io/doc.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19390 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/io/export.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21518 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/io/notebook.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5047 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/io/output.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6261 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/io/saving.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8278 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/io/showing.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8360 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/io/state.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4155 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/io/util.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6093 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/io/webdriver.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23032 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/layouts.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.854447 bokeh-3.2.0.dev4/src/bokeh/model/
+-rw-r--r--   0 runner    (1001) docker     (122)     1876 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2053 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/model/data_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4140 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/model/docs.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21302 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/model/model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7839 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/model/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.858448 bokeh-3.2.0.dev4/src/bokeh/models/
+-rw-r--r--   0 runner    (1001) docker     (122)     4057 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.858448 bokeh-3.2.0.dev4/src/bokeh/models/annotations/
+-rw-r--r--   0 runner    (1001) docker     (122)     2109 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/annotations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2590 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/annotations/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5564 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/annotations/arrows.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13775 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/annotations/geometry.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.858448 bokeh-3.2.0.dev4/src/bokeh/models/annotations/html/
+-rw-r--r--   0 runner    (1001) docker     (122)     1950 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/annotations/html/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2265 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/annotations/html/html_annotation.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10444 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/annotations/html/labels.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2093 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/annotations/html/toolbars.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9340 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/annotations/labels.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16806 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/annotations/legends.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12456 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/axes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7795 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2363 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/canvas.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3154 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16739 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/css.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6881 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/dom.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9495 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/expressions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8487 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/filters.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24509 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/formatters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4197 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/glyph.py
+-rw-r--r--   0 runner    (1001) docker     (122)    54279 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/glyphs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2616 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/graphics.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6435 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/graphs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4263 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/grids.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4008 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/labeling.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23128 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/layouts.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7304 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/map_plots.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12636 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/mappers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    33674 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/plots.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17571 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/ranges.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.858448 bokeh-3.2.0.dev4/src/bokeh/models/renderers/
+-rw-r--r--   0 runner    (1001) docker     (122)     2101 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/renderers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4996 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/renderers/contour_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8796 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/renderers/glyph_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4366 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/renderers/graph_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4219 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/renderers/renderer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2613 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/renderers/tile_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3815 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/scales.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4923 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/selections.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3711 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/selectors.py
+-rw-r--r--   0 runner    (1001) docker     (122)    33223 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/sources.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4673 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/text.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2827 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/textures.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11476 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/tickers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6596 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/tiles.py
+-rw-r--r--   0 runner    (1001) docker     (122)    73516 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/tools.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9422 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.862448 bokeh-3.2.0.dev4/src/bokeh/models/ui/
+-rw-r--r--   0 runner    (1001) docker     (122)     2153 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2548 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/ui/dialogs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2275 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/ui/examiner.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4930 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/ui/icons.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3706 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/ui/menus.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2095 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/ui/panes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3913 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/ui/tooltips.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3068 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/ui/ui_element.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.862448 bokeh-3.2.0.dev4/src/bokeh/models/util/
+-rw-r--r--   0 runner    (1001) docker     (122)      876 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12432 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/util/structure.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.862448 bokeh-3.2.0.dev4/src/bokeh/models/widgets/
+-rw-r--r--   0 runner    (1001) docker     (122)     2137 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7089 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/widgets/buttons.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4612 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/widgets/groups.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16135 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/widgets/inputs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4680 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/widgets/markups.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11229 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/widgets/pickers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10242 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/widgets/sliders.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28151 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/widgets/tables.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2429 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/models/widgets/widget.py
+-rw-r--r--   0 runner    (1001) docker     (122)   113099 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/palettes.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.862448 bokeh-3.2.0.dev4/src/bokeh/plotting/
+-rw-r--r--   0 runner    (1001) docker     (122)     2533 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3921 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/plotting/_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8267 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/plotting/_docstring.py
+-rw-r--r--   0 runner    (1001) docker     (122)    32388 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/plotting/_figure.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6603 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/plotting/_graph.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5002 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/plotting/_legends.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6567 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/plotting/_plot.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12625 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/plotting/_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3813 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/plotting/_stack.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8078 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/plotting/_tools.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14637 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/plotting/contour.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27693 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/plotting/glyph_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4939 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/plotting/gmap.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5836 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/plotting/graph.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.866448 bokeh-3.2.0.dev4/src/bokeh/protocol/
+-rw-r--r--   0 runner    (1001) docker     (122)     5428 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/protocol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2485 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/protocol/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11813 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/protocol/message.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.866448 bokeh-3.2.0.dev4/src/bokeh/protocol/messages/
+-rw-r--r--   0 runner    (1001) docker     (122)     2138 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/protocol/messages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2309 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/protocol/messages/ack.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3307 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/protocol/messages/error.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2467 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/protocol/messages/ok.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3754 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/protocol/messages/patch_doc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3176 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/protocol/messages/pull_doc_reply.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2334 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/protocol/messages/pull_doc_req.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2799 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/protocol/messages/push_doc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3072 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/protocol/messages/server_info_reply.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2380 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/protocol/messages/server_info_req.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6987 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/protocol/receiver.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)    24107 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.870448 bokeh-3.2.0.dev4/src/bokeh/sampledata/
+-rw-r--r--   0 runner    (1001) docker     (122)     2643 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.874448 bokeh-3.2.0.dev4/src/bokeh/sampledata/_data/
+-rw-r--r--   0 runner    (1001) docker     (122)    79935 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/_data/USHolidays.ics
+-rw-r--r--   0 runner    (1001) docker     (122)   106201 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/_data/US_Regions_State_Boundaries.csv.gz
+-rw-r--r--   0 runner    (1001) docker     (122)    17444 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/_data/auto-mpg.csv
+-rw-r--r--   0 runner    (1001) docker     (122)    17345 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/_data/auto-mpg2.csv
+-rw-r--r--   0 runner    (1001) docker     (122)     2296 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/_data/browsers_nov_2013.csv
+-rw-r--r--   0 runner    (1001) docker     (122)    25491 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/_data/commits.txt.gz
+-rw-r--r--   0 runner    (1001) docker     (122)    11342 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/_data/daylight_warsaw_2013.csv
+-rw-r--r--   0 runner    (1001) docker     (122)    14487 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/_data/elements.csv
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.874448 bokeh-3.2.0.dev4/src/bokeh/sampledata/_data/icons/
+-rw-r--r--   0 runner    (1001) docker     (122)     1985 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/_data/icons/chrome_32x32.png
+-rw-r--r--   0 runner    (1001) docker     (122)     2443 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/_data/icons/firefox_32x32.png
+-rw-r--r--   0 runner    (1001) docker     (122)     2293 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/_data/icons/ie_32x32.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1666 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/_data/icons/opera_32x32.png
+-rw-r--r--   0 runner    (1001) docker     (122)     2552 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/_data/icons/safari_32x32.png
+-rw-r--r--   0 runner    (1001) docker     (122)     3858 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/_data/iris.csv
+-rw-r--r--   0 runner    (1001) docker     (122)    11536 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/_data/les_mis.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1390 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/_data/numberly.csv
+-rw-r--r--   0 runner    (1001) docker     (122)    33264 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/_data/obiszow_mtb_xcm.csv
+-rw-r--r--   0 runner    (1001) docker     (122)     8630 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/_data/olympics2014.json
+-rw-r--r--   0 runner    (1001) docker     (122)    13478 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/_data/penguins.csv
+-rw-r--r--   0 runner    (1001) docker     (122)     5682 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/_data/percent-bachelors-degrees-women-usa.csv
+-rw-r--r--   0 runner    (1001) docker     (122)     2465 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/_data/probly.csv
+-rw-r--r--   0 runner    (1001) docker     (122)    14494 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/_data/sample_geojson.geojson
+-rw-r--r--   0 runner    (1001) docker     (122)    76453 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/_data/sea_surface_temperature.csv.gz
+-rw-r--r--   0 runner    (1001) docker     (122)     5332 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/_data/sprint.csv
+-rw-r--r--   0 runner    (1001) docker     (122)     4003 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/_data/unemployment1948.csv
+-rw-r--r--   0 runner    (1001) docker     (122)     5387 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/_data/us_marriages_divorces.csv
+-rw-r--r--   0 runner    (1001) docker     (122)     2285 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/airport_routes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2761 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/airports.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3122 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/anscombe.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3780 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/antibiotics.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3038 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/autompg.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2607 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/autompg2.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3112 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/browsers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2498 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/commits.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2648 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/daylight.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2192 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/degrees.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4599 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/gapminder.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2022 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/glucose.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2200 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/haar_cascade.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2371 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/iris.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2367 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/les_mis.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2102 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/movies_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2096 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/mtb.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2224 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/olympics2014.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2212 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/penguins.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2270 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/perceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2041 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/periodic_table.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2548 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/population.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2071 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/sample_geojson.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2109 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/sample_superstore.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2706 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/sea_surface_temperature.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2066 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/sprint.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3520 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/stocks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2777 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/unemployment.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2099 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/unemployment1948.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2116 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/us_cities.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4032 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/us_counties.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2888 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/us_holidays.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2382 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/us_marriages_divorces.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3703 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/us_states.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2132 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sampledata/world_cities.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.874448 bokeh-3.2.0.dev4/src/bokeh/server/
+-rw-r--r--   0 runner    (1001) docker     (122)     1468 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9579 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/auth_provider.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6721 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3939 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/connection.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14606 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/contexts.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4096 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/protocol_handler.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20849 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/server.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11852 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/session.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.830447 bokeh-3.2.0.dev4/src/bokeh/server/static/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.890448 bokeh-3.2.0.dev4/src/bokeh/server/static/js/
+-rw-r--r--   0 runner    (1001) docker     (122)   211364 2023-06-09 10:32:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/bokeh-api.js
+-rw-r--r--   0 runner    (1001) docker     (122)   118620 2023-06-09 10:32:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/bokeh-api.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)   535981 2023-06-09 10:32:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/bokeh-gl.js
+-rw-r--r--   0 runner    (1001) docker     (122)   198524 2023-06-09 10:32:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/bokeh-gl.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)  2750420 2023-06-09 10:32:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/bokeh-mathjax.js
+-rw-r--r--   0 runner    (1001) docker     (122)  1785923 2023-06-09 10:32:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/bokeh-mathjax.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)   949247 2023-06-09 10:32:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/bokeh-tables.js
+-rw-r--r--   0 runner    (1001) docker     (122)   302599 2023-06-09 10:32:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/bokeh-tables.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)   799629 2023-06-09 10:32:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/bokeh-widgets.js
+-rw-r--r--   0 runner    (1001) docker     (122)   301352 2023-06-09 10:32:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/bokeh-widgets.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)  2257234 2023-06-09 10:32:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/bokeh.js
+-rw-r--r--   0 runner    (1001) docker     (122)   959268 2023-06-09 10:32:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/bokeh.min.js
+-rw-r--r--   0 runner    (1001) docker     (122) 20427534 2023-06-09 10:32:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/compiler.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.914449 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.914449 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/api/
+-rw-r--r--   0 runner    (1001) docker     (122)     1042 2023-06-09 10:31:47.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/api/charts.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      508 2023-06-09 10:31:47.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/api/expr.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     4471 2023-06-09 10:31:47.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/api/figure.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)    19794 2023-06-09 10:31:47.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/api/glyph_api.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      924 2023-06-09 10:31:47.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/api/gridplot.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      448 2023-06-09 10:31:47.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/api/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      739 2023-06-09 10:31:47.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/api/io.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     3346 2023-06-09 10:31:46.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/api/linalg.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)       59 2023-06-09 10:31:47.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/api/main.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)       63 2023-06-09 10:31:47.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/api/models.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)    63941 2023-06-09 10:31:47.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/api/palettes.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     5394 2023-06-09 10:31:47.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/api/parser.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      206 2023-06-09 10:31:47.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/api/plotting.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      844 2023-06-09 10:31:47.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/api/themes.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      255 2023-06-09 10:31:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/base.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      260 2023-06-09 10:31:49.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/bokeh.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.914449 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/client/
+-rw-r--r--   0 runner    (1001) docker     (122)     2380 2023-06-09 10:31:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/client/connection.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1106 2023-06-09 10:31:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/client/session.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.918449 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/
+-rw-r--r--   0 runner    (1001) docker     (122)     5846 2023-06-09 10:31:33.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/bokeh_events.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      820 2023-06-09 10:31:36.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/build_views.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      274 2023-06-09 10:31:32.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/class.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)    42976 2023-06-09 10:31:34.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/css.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      334 2023-06-09 10:31:42.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/diagnostics.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     5953 2023-06-09 10:31:34.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/dom.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1548 2023-06-09 10:31:36.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/dom_view.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)    11975 2023-06-09 10:31:33.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/enums.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1062 2023-06-09 10:31:33.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/geometry.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     3638 2023-06-09 10:31:39.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/graphics.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     5113 2023-06-09 10:31:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/has_props.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      966 2023-06-09 10:31:36.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/hittest.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     8908 2023-06-09 10:31:33.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/kinds.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.918449 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/layout/
+-rw-r--r--   0 runner    (1001) docker     (122)      894 2023-06-09 10:31:36.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/layout/alignments.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      835 2023-06-09 10:31:39.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/layout/border.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     3050 2023-06-09 10:31:36.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/layout/grid.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      321 2023-06-09 10:31:36.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/layout/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1764 2023-06-09 10:31:36.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/layout/layoutable.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1143 2023-06-09 10:31:39.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/layout/side_panel.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1595 2023-06-09 10:31:35.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/layout/types.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1139 2023-06-09 10:31:33.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/logging.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      861 2023-06-09 10:31:42.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/patching.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     9618 2023-06-09 10:31:42.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/properties.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     6764 2023-06-09 10:31:35.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/property_mixins.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      497 2023-06-09 10:31:42.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/resolvers.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      839 2023-06-09 10:31:37.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/selection_manager.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.918449 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/serialization/
+-rw-r--r--   0 runner    (1001) docker     (122)      409 2023-06-09 10:31:33.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/serialization/buffer.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2491 2023-06-09 10:31:42.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/serialization/deserializer.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      201 2023-06-09 10:31:33.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/serialization/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2038 2023-06-09 10:31:33.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/serialization/reps.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1766 2023-06-09 10:31:33.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/serialization/serializer.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      376 2023-06-09 10:31:36.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/settings.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1442 2023-06-09 10:31:33.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/signaling.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     3051 2023-06-09 10:31:32.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/types.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     6931 2023-06-09 10:31:41.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/ui_events.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1746 2023-06-09 10:31:37.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/uniforms.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.926449 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/
+-rw-r--r--   0 runner    (1001) docker     (122)     1565 2023-06-09 10:31:34.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/affine.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      754 2023-06-09 10:31:44.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/algorithms.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2365 2023-06-09 10:31:33.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/array.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     4300 2023-06-09 10:31:33.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/arrayable.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      243 2023-06-09 10:31:32.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/assert.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     3261 2023-06-09 10:31:34.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/bbox.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1486 2023-06-09 10:31:32.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/bitset.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      298 2023-06-09 10:31:33.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/buffer.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1006 2023-06-09 10:31:34.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/canvas.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      592 2023-06-09 10:31:42.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/cloneable.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      918 2023-06-09 10:31:32.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/color.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      236 2023-06-09 10:31:33.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/defer.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1275 2023-06-09 10:31:32.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/eq.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      152 2023-06-09 10:31:37.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/flip_step_mode.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      562 2023-06-09 10:31:39.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/image.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      234 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/interpolation.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1332 2023-06-09 10:31:33.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/iterator.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1763 2023-06-09 10:31:33.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/math.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      737 2023-06-09 10:31:47.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/matrix.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1884 2023-06-09 10:31:36.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/menus.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      163 2023-06-09 10:31:39.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/modules.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     6794 2023-06-09 10:31:38.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/ndarray.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2324 2023-06-09 10:31:33.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/object.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      287 2023-06-09 10:31:33.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/platform.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      865 2023-06-09 10:31:42.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/pretty.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1027 2023-06-09 10:31:36.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/projections.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      963 2023-06-09 10:31:32.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/ragged_array.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      831 2023-06-09 10:31:34.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/random.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      253 2023-06-09 10:31:33.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/refs.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      254 2023-06-09 10:31:35.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/set.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      507 2023-06-09 10:31:42.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/slice.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      492 2023-06-09 10:31:36.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/spatial.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      499 2023-06-09 10:31:39.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/string.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)    11070 2023-06-09 10:31:34.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/svg.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     3602 2023-06-09 10:31:32.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/svg_colors.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1813 2023-06-09 10:31:40.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/templating.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      560 2023-06-09 10:31:39.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/text.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      189 2023-06-09 10:31:39.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/throttle.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      185 2023-06-09 10:31:42.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/typed_array.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1756 2023-06-09 10:31:32.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/types.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      101 2023-06-09 10:31:42.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/version.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      253 2023-06-09 10:31:36.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/wheel.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      770 2023-06-09 10:31:39.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/zoom.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1427 2023-06-09 10:31:42.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/vectorization.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2375 2023-06-09 10:31:42.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/view.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.926449 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/visuals/
+-rw-r--r--   0 runner    (1001) docker     (122)     1355 2023-06-09 10:31:35.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/visuals/fill.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2414 2023-06-09 10:31:35.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/visuals/hatch.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1165 2023-06-09 10:31:35.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/visuals/image.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      959 2023-06-09 10:31:35.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/visuals/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1947 2023-06-09 10:31:35.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/visuals/line.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      472 2023-06-09 10:31:34.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/visuals/patterns.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2167 2023-06-09 10:31:35.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/visuals/text.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1262 2023-06-09 10:31:35.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/visuals/visual.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.926449 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/document/
+-rw-r--r--   0 runner    (1001) docker     (122)     1161 2023-06-09 10:31:42.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/document/defs.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     4788 2023-06-09 10:31:42.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/document/document.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     6205 2023-06-09 10:31:42.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/document/events.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)       89 2023-06-09 10:31:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/document/index.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.926449 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/embed/
+-rw-r--r--   0 runner    (1001) docker     (122)      287 2023-06-09 10:31:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/embed/dom.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      843 2023-06-09 10:31:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/embed/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      482 2023-06-09 10:31:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/embed/json.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      254 2023-06-09 10:31:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/embed/notebook.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      308 2023-06-09 10:31:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/embed/server.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      441 2023-06-09 10:31:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/embed/standalone.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      446 2023-06-09 10:31:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)       83 2023-06-09 10:31:46.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/main.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2140 2023-06-09 10:31:34.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/model.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.926449 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.930449 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/annotations/
+-rw-r--r--   0 runner    (1001) docker     (122)     1133 2023-06-09 10:31:39.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/annotations/annotation.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2176 2023-06-09 10:31:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/annotations/arrow.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     3573 2023-06-09 10:31:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/annotations/arrow_head.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      900 2023-06-09 10:31:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/annotations/band.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     4220 2023-06-09 10:31:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/annotations/base_color_bar.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     4135 2023-06-09 10:31:40.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/annotations/box_annotation.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2099 2023-06-09 10:31:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/annotations/color_bar.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1398 2023-06-09 10:31:44.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/annotations/contour_color_bar.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1100 2023-06-09 10:31:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/annotations/data_annotation.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.930449 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/annotations/html/
+-rw-r--r--   0 runner    (1001) docker     (122)      153 2023-06-09 10:31:44.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/annotations/html/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1369 2023-06-09 10:31:44.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/annotations/html/label.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2245 2023-06-09 10:31:44.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/annotations/html/label_set.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1191 2023-06-09 10:31:44.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/annotations/html/text_annotation.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1357 2023-06-09 10:31:44.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/annotations/html/title.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1004 2023-06-09 10:31:44.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/annotations/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1145 2023-06-09 10:31:44.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/annotations/label.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1970 2023-06-09 10:31:44.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/annotations/label_set.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     3890 2023-06-09 10:31:44.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/annotations/legend.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      948 2023-06-09 10:31:44.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/annotations/legend_item.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     3650 2023-06-09 10:31:40.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/annotations/poly_annotation.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1159 2023-06-09 10:31:44.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/annotations/slope.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2146 2023-06-09 10:31:40.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/annotations/span.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1699 2023-06-09 10:31:39.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/annotations/text_annotation.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1175 2023-06-09 10:31:39.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/annotations/title.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1283 2023-06-09 10:31:39.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/annotations/toolbar_panel.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1586 2023-06-09 10:31:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/annotations/upper_lower.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1443 2023-06-09 10:31:44.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/annotations/whisker.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.934449 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/axes/
+-rw-r--r--   0 runner    (1001) docker     (122)     5022 2023-06-09 10:31:41.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/axes/axis.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2312 2023-06-09 10:31:41.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/axes/categorical_axis.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      600 2023-06-09 10:31:41.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/axes/continuous_axis.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      834 2023-06-09 10:31:42.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/axes/datetime_axis.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      350 2023-06-09 10:31:42.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/axes/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      816 2023-06-09 10:31:42.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/axes/linear_axis.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      754 2023-06-09 10:31:42.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/axes/log_axis.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      823 2023-06-09 10:31:42.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/axes/mercator_axis.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.934449 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (122)      982 2023-06-09 10:31:33.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/callbacks/callback.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1311 2023-06-09 10:31:44.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/callbacks/customjs.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      152 2023-06-09 10:31:44.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/callbacks/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      696 2023-06-09 10:31:44.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/callbacks/open_url.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      604 2023-06-09 10:31:44.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/callbacks/set_value.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.934449 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/canvas/
+-rw-r--r--   0 runner    (1001) docker     (122)     2146 2023-06-09 10:31:41.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/canvas/canvas.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1852 2023-06-09 10:31:38.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/canvas/cartesian_frame.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      122 2023-06-09 10:31:44.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/canvas/index.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.934449 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/common/
+-rw-r--r--   0 runner    (1001) docker     (122)     3477 2023-06-09 10:31:39.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/common/kinds.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      256 2023-06-09 10:31:40.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/common/painting.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      565 2023-06-09 10:31:39.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/common/resolve.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.934449 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/coordinates/
+-rw-r--r--   0 runner    (1001) docker     (122)     2253 2023-06-09 10:31:39.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/coordinates/coordinate_mapping.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)       93 2023-06-09 10:31:44.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/coordinates/index.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.938449 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/dom/
+-rw-r--r--   0 runner    (1001) docker     (122)      819 2023-06-09 10:31:40.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/dom/action.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      932 2023-06-09 10:31:46.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/dom/color_ref.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1081 2023-06-09 10:31:40.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/dom/dom_element.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      605 2023-06-09 10:31:40.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/dom/dom_node.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1609 2023-06-09 10:31:46.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/dom/elements.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      936 2023-06-09 10:31:40.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/dom/html.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      708 2023-06-09 10:31:46.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/dom/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      762 2023-06-09 10:31:46.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/dom/index_.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      872 2023-06-09 10:31:40.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/dom/placeholder.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)    16289 2023-06-09 10:31:35.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/dom/styles.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2288 2023-06-09 10:31:35.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/dom/stylesheets.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1050 2023-06-09 10:31:40.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/dom/template.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      641 2023-06-09 10:31:46.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/dom/text.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      902 2023-06-09 10:31:46.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/dom/toggle_group.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      729 2023-06-09 10:31:46.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/dom/value_of.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      836 2023-06-09 10:31:46.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/dom/value_ref.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.938449 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/expressions/
+-rw-r--r--   0 runner    (1001) docker     (122)     1972 2023-06-09 10:31:37.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/expressions/coordinate_transform.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      699 2023-06-09 10:31:44.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/expressions/cumsum.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      894 2023-06-09 10:31:44.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/expressions/customjs_expr.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1308 2023-06-09 10:31:37.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/expressions/expression.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      424 2023-06-09 10:31:44.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/expressions/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      662 2023-06-09 10:31:44.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/expressions/maximum.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      662 2023-06-09 10:31:44.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/expressions/minimum.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      850 2023-06-09 10:31:44.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/expressions/polar.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      652 2023-06-09 10:31:44.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/expressions/stack.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.938449 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/filters/
+-rw-r--r--   0 runner    (1001) docker     (122)      607 2023-06-09 10:31:38.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/filters/all_indices.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      681 2023-06-09 10:31:44.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/filters/boolean_filter.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      827 2023-06-09 10:31:44.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/filters/customjs_filter.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      694 2023-06-09 10:31:44.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/filters/difference_filter.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      571 2023-06-09 10:31:38.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/filters/filter.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      695 2023-06-09 10:31:44.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/filters/group_filter.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      599 2023-06-09 10:31:44.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/filters/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      725 2023-06-09 10:31:44.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/filters/index_filter.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      708 2023-06-09 10:31:38.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/filters/intersection_filter.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      689 2023-06-09 10:31:44.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/filters/inversion_filter.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      758 2023-06-09 10:31:44.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/filters/symmetric_difference_filter.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      659 2023-06-09 10:31:44.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/filters/union_filter.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.942449 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/formatters/
+-rw-r--r--   0 runner    (1001) docker     (122)     1189 2023-06-09 10:31:42.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/formatters/basic_tick_formatter.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      631 2023-06-09 10:31:41.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/formatters/categorical_tick_formatter.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      813 2023-06-09 10:31:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/formatters/customjs_tick_formatter.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2021 2023-06-09 10:31:42.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/formatters/datetime_tick_formatter.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      605 2023-06-09 10:31:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/formatters/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1078 2023-06-09 10:31:42.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/formatters/log_tick_formatter.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      729 2023-06-09 10:31:42.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/formatters/mercator_tick_formatter.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      820 2023-06-09 10:31:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/formatters/numeral_tick_formatter.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      642 2023-06-09 10:31:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/formatters/printf_tick_formatter.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      878 2023-06-09 10:31:41.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/formatters/tick_formatter.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.946449 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/
+-rw-r--r--   0 runner    (1001) docker     (122)     2365 2023-06-09 10:31:41.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/annular_wedge.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1970 2023-06-09 10:31:41.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/annulus.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1757 2023-06-09 10:31:44.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/arc.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1141 2023-06-09 10:31:37.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/area.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2002 2023-06-09 10:31:44.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/bezier.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1295 2023-06-09 10:31:44.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/block.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1712 2023-06-09 10:31:41.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/center_rotatable.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2604 2023-06-09 10:31:41.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/circle.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      499 2023-06-09 10:31:41.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/defs.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1293 2023-06-09 10:31:44.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/ellipse.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     4094 2023-06-09 10:31:38.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/glyph.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1472 2023-06-09 10:31:37.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/harea.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1747 2023-06-09 10:31:37.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/harea_step.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1286 2023-06-09 10:31:44.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/hbar.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2711 2023-06-09 10:31:41.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/hex_tile.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2076 2023-06-09 10:31:44.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/hspan.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2480 2023-06-09 10:31:44.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/hstrip.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1043 2023-06-09 10:31:44.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/image.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2979 2023-06-09 10:31:40.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/image_base.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      922 2023-06-09 10:31:44.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/image_rgba.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1160 2023-06-09 10:31:44.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/image_stack.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2425 2023-06-09 10:31:39.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/image_url.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1396 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1591 2023-06-09 10:31:37.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/line.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2559 2023-06-09 10:31:44.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/lrtb.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2220 2023-06-09 10:31:41.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/marker.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2032 2023-06-09 10:31:37.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/multi_line.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2290 2023-06-09 10:31:44.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/multi_polygons.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1478 2023-06-09 10:31:37.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/patch.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2116 2023-06-09 10:31:37.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/patches.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1169 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/quad.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1892 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/quadratic.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1379 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/ray.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2202 2023-06-09 10:31:41.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/rect.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1161 2023-06-09 10:31:41.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/scatter.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2090 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/segment.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1365 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/spline.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1399 2023-06-09 10:31:41.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/step.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2543 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/text.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1307 2023-06-09 10:31:36.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/utils.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1472 2023-06-09 10:31:37.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/varea.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1747 2023-06-09 10:31:37.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/varea_step.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1284 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/vbar.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2076 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/vspan.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2480 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/vstrip.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.950449 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/webgl/
+-rw-r--r--   0 runner    (1001) docker     (122)      668 2023-06-09 10:31:41.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/webgl/annular_wedge.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      595 2023-06-09 10:31:41.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/webgl/annulus.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      944 2023-06-09 10:31:37.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/webgl/base.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1560 2023-06-09 10:31:37.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/webgl/base_line.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2179 2023-06-09 10:31:41.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/webgl/base_marker.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1920 2023-06-09 10:31:37.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/webgl/buffer.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      542 2023-06-09 10:31:41.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/webgl/circle.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      552 2023-06-09 10:31:37.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/webgl/dash_cache.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      472 2023-06-09 10:31:41.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/webgl/hex_tile.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      438 2023-06-09 10:31:41.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/webgl/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      700 2023-06-09 10:31:37.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/webgl/line_gl.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      825 2023-06-09 10:31:41.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/webgl/lrtb.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)       52 2023-06-09 10:31:46.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/webgl/main.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)       53 2023-06-09 10:31:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/webgl/marker.frag.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)       53 2023-06-09 10:31:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/webgl/marker.vert.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      853 2023-06-09 10:31:41.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/webgl/multi_marker.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      452 2023-06-09 10:31:41.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/webgl/rect.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)       53 2023-06-09 10:31:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/webgl/regl_line.frag.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)       53 2023-06-09 10:31:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/webgl/regl_line.vert.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1310 2023-06-09 10:31:37.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/webgl/regl_wrap.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      930 2023-06-09 10:31:41.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/webgl/single_marker.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      703 2023-06-09 10:31:41.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/webgl/step.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      562 2023-06-09 10:31:41.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/webgl/sxsy.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     3538 2023-06-09 10:31:37.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/webgl/types.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.950449 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/webgl/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      143 2023-06-09 10:31:37.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/webgl/utils/math.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      697 2023-06-09 10:31:36.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/webgl/webgl_utils.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      612 2023-06-09 10:31:41.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/webgl/wedge.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2052 2023-06-09 10:31:41.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/wedge.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1144 2023-06-09 10:31:36.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/xy_glyph.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.950449 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/graphics/
+-rw-r--r--   0 runner    (1001) docker     (122)     1123 2023-06-09 10:31:38.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/graphics/decoration.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      115 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/graphics/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1239 2023-06-09 10:31:38.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/graphics/marking.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.950449 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/graphs/
+-rw-r--r--   0 runner    (1001) docker     (122)     5351 2023-06-09 10:31:37.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/graphs/graph_hit_test_policy.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      153 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/graphs/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2330 2023-06-09 10:31:37.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/graphs/layout_provider.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      933 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/graphs/static_layout_provider.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.950449 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/grids/
+-rw-r--r--   0 runner    (1001) docker     (122)     1926 2023-06-09 10:31:42.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/grids/grid.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)       66 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/grids/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      875 2023-06-09 10:31:46.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/index.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.954449 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/layouts/
+-rw-r--r--   0 runner    (1001) docker     (122)      636 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/layouts/alignments.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      556 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/layouts/column.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1190 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/layouts/css_grid_box.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      981 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/layouts/flex_box.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1032 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/layouts/grid_box.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1019 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/layouts/group_box.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1087 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/layouts/hbox.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      467 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/layouts/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     4125 2023-06-09 10:31:36.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/layouts/layout_dom.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      523 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/layouts/row.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1010 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/layouts/scroll_box.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      660 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/layouts/spacer.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      618 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/layouts/tab_panel.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1288 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/layouts/tabs.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1087 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/layouts/vbox.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)       45 2023-06-09 10:31:46.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/main.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.954449 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/mappers/
+-rw-r--r--   0 runner    (1001) docker     (122)      891 2023-06-09 10:31:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/mappers/categorical_color_mapper.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      866 2023-06-09 10:31:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/mappers/categorical_mapper.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      977 2023-06-09 10:31:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/mappers/categorical_marker_mapper.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1003 2023-06-09 10:31:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/mappers/categorical_pattern_mapper.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1659 2023-06-09 10:31:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/mappers/color_mapper.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1888 2023-06-09 10:31:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/mappers/continuous_color_mapper.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      807 2023-06-09 10:31:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/mappers/eqhist_color_mapper.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      726 2023-06-09 10:31:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/mappers/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      892 2023-06-09 10:31:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/mappers/linear_color_mapper.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      830 2023-06-09 10:31:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/mappers/log_color_mapper.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      668 2023-06-09 10:31:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/mappers/mapper.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      993 2023-06-09 10:31:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/mappers/scanning_color_mapper.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      498 2023-06-09 10:31:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/mappers/stack_color_mapper.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1307 2023-06-09 10:31:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/mappers/weighted_stack_color_mapper.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.954449 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/menus/
+-rw-r--r--   0 runner    (1001) docker     (122)      819 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/menus/action.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      612 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/menus/check_action.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      556 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/menus/divider.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      221 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/menus/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1057 2023-06-09 10:31:36.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/menus/menu.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      666 2023-06-09 10:31:36.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/menus/menu_item.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      605 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/menus/section.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.958449 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/plots/
+-rw-r--r--   0 runner    (1001) docker     (122)      604 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/plots/figure.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      609 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/plots/gmap.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1568 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/plots/gmap_plot.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1531 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/plots/gmap_plot_canvas.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1954 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/plots/grid_plot.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      297 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/plots/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     4499 2023-06-09 10:31:42.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/plots/plot.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     4933 2023-06-09 10:31:39.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/plots/plot_canvas.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1227 2023-06-09 10:31:39.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/plots/range_manager.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1274 2023-06-09 10:31:39.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/plots/state_manager.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.958449 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/policies/
+-rw-r--r--   0 runner    (1001) docker     (122)       63 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/policies/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2207 2023-06-09 10:31:41.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/policies/labeling.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.958449 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/random/
+-rw-r--r--   0 runner    (1001) docker     (122)       86 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/random/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      630 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/random/park_miller_lcg.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      573 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/random/random_generator.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.958449 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/ranges/
+-rw-r--r--   0 runner    (1001) docker     (122)      553 2023-06-09 10:31:38.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/ranges/data_range.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2363 2023-06-09 10:31:38.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/ranges/data_range1d.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     3167 2023-06-09 10:31:42.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/ranges/factor_range.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      239 2023-06-09 10:31:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/ranges/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      956 2023-06-09 10:31:42.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/ranges/range.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      826 2023-06-09 10:31:36.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/ranges/range1d.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.958449 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/renderers/
+-rw-r--r--   0 runner    (1001) docker     (122)     1467 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/renderers/contour_renderer.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1306 2023-06-09 10:31:38.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/renderers/data_renderer.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2946 2023-06-09 10:31:38.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/renderers/glyph_renderer.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1809 2023-06-09 10:31:37.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/renderers/graph_renderer.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      687 2023-06-09 10:31:41.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/renderers/guide_renderer.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      293 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/renderers/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2714 2023-06-09 10:31:41.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/renderers/renderer.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.962449 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/scales/
+-rw-r--r--   0 runner    (1001) docker     (122)      669 2023-06-09 10:31:36.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/scales/categorical_scale.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      473 2023-06-09 10:31:36.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/scales/continuous_scale.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      337 2023-06-09 10:31:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/scales/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1069 2023-06-09 10:31:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/scales/linear_interpolation_scale.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      604 2023-06-09 10:31:36.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/scales/linear_scale.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      679 2023-06-09 10:31:36.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/scales/log_scale.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1109 2023-06-09 10:31:36.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/scales/scale.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.962449 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/selections/
+-rw-r--r--   0 runner    (1001) docker     (122)      114 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/selections/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      982 2023-06-09 10:31:38.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/selections/interaction_policy.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1607 2023-06-09 10:31:36.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/selections/selection.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.962449 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/selectors/
+-rw-r--r--   0 runner    (1001) docker     (122)      459 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/selectors/by_class.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      445 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/selectors/by_css.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      438 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/selectors/by_id.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      459 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/selectors/by_xpath.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      177 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/selectors/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      520 2023-06-09 10:31:40.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/selectors/selector.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.962449 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/sources/
+-rw-r--r--   0 runner    (1001) docker     (122)     1221 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/sources/ajax_data_source.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1525 2023-06-09 10:31:38.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/sources/cds_view.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      901 2023-06-09 10:31:42.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/sources/column_data_source.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1541 2023-06-09 10:31:38.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/sources/columnar_data_source.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      558 2023-06-09 10:31:38.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/sources/data_source.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1179 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/sources/geojson_data_source.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      464 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/sources/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      582 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/sources/server_sent_data_source.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1147 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/sources/web_data_source.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.962449 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/text/
+-rw-r--r--   0 runner    (1001) docker     (122)      797 2023-06-09 10:31:39.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/text/base_text.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      137 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/text/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     4357 2023-06-09 10:31:39.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/text/math_text.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.962449 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/text/mathjax/
+-rw-r--r--   0 runner    (1001) docker     (122)      361 2023-06-09 10:31:39.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/text/mathjax/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)       52 2023-06-09 10:31:49.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/text/mathjax/main.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      666 2023-06-09 10:31:39.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/text/plain_text.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      839 2023-06-09 10:31:39.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/text/providers.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      152 2023-06-09 10:31:39.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/text/utils.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.966450 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/textures/
+-rw-r--r--   0 runner    (1001) docker     (122)      719 2023-06-09 10:31:46.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/textures/canvas_texture.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      771 2023-06-09 10:31:46.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/textures/image_url_texture.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      177 2023-06-09 10:31:46.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/textures/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      766 2023-06-09 10:31:35.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/textures/texture.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.966450 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tickers/
+-rw-r--r--   0 runner    (1001) docker     (122)      905 2023-06-09 10:31:42.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tickers/adaptive_ticker.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      465 2023-06-09 10:31:42.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tickers/basic_ticker.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      817 2023-06-09 10:31:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tickers/binned_ticker.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      797 2023-06-09 10:31:41.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tickers/categorical_ticker.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1051 2023-06-09 10:31:42.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tickers/composite_ticker.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1170 2023-06-09 10:31:42.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tickers/continuous_ticker.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      490 2023-06-09 10:31:42.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tickers/datetime_ticker.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      757 2023-06-09 10:31:42.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tickers/days_ticker.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      959 2023-06-09 10:31:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tickers/fixed_ticker.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      779 2023-06-09 10:31:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tickers/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      620 2023-06-09 10:31:42.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tickers/log_ticker.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      999 2023-06-09 10:31:42.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tickers/mercator_ticker.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      773 2023-06-09 10:31:42.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tickers/months_ticker.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1222 2023-06-09 10:31:42.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tickers/single_interval_ticker.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      623 2023-06-09 10:31:41.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tickers/ticker.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      495 2023-06-09 10:31:41.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tickers/util.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      787 2023-06-09 10:31:42.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tickers/years_ticker.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.966450 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tiles/
+-rw-r--r--   0 runner    (1001) docker     (122)      615 2023-06-09 10:31:46.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tiles/bbox_tile_source.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      404 2023-06-09 10:31:46.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tiles/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2788 2023-06-09 10:31:46.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tiles/mercator_tile_source.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      585 2023-06-09 10:31:46.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tiles/quadkey_tile_source.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2434 2023-06-09 10:31:46.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tiles/tile_renderer.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2277 2023-06-09 10:31:46.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tiles/tile_source.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      486 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tiles/tile_utils.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      557 2023-06-09 10:31:46.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tiles/tms_tile_source.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      564 2023-06-09 10:31:46.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tiles/wmts_tile_source.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.970450 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.970450 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/actions/
+-rw-r--r--   0 runner    (1001) docker     (122)      903 2023-06-09 10:31:38.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/actions/action_tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      653 2023-06-09 10:31:46.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/actions/copy_tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      805 2023-06-09 10:31:46.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/actions/custom_action.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      867 2023-06-09 10:31:46.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/actions/examine_tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      686 2023-06-09 10:31:46.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/actions/fullscreen_tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      674 2023-06-09 10:31:38.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/actions/help_tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      559 2023-06-09 10:31:46.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/actions/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      760 2023-06-09 10:31:39.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/actions/plot_action_tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      680 2023-06-09 10:31:40.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/actions/redo_tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      661 2023-06-09 10:31:40.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/actions/reset_tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      864 2023-06-09 10:31:40.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/actions/save_tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      680 2023-06-09 10:31:40.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/actions/undo_tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1031 2023-06-09 10:31:39.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/actions/zoom_base_tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      552 2023-06-09 10:31:39.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/actions/zoom_in_tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      766 2023-06-09 10:31:39.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/actions/zoom_out_tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      748 2023-06-09 10:31:38.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/click_button.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.974450 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/edit/
+-rw-r--r--   0 runner    (1001) docker     (122)     1820 2023-06-09 10:31:46.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/edit/box_edit_tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1873 2023-06-09 10:31:46.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/edit/edit_tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1098 2023-06-09 10:31:46.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/edit/freehand_draw_tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      417 2023-06-09 10:31:46.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/edit/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1466 2023-06-09 10:31:46.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/edit/line_edit_tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1038 2023-06-09 10:31:46.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/edit/line_tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1303 2023-06-09 10:31:46.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/edit/point_draw_tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1621 2023-06-09 10:31:46.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/edit/poly_draw_tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1574 2023-06-09 10:31:46.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/edit/poly_edit_tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1288 2023-06-09 10:31:46.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/edit/poly_tool.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.974450 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/gestures/
+-rw-r--r--   0 runner    (1001) docker     (122)     2019 2023-06-09 10:31:40.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/gestures/box_select_tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1944 2023-06-09 10:31:40.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/gestures/box_zoom_tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      928 2023-06-09 10:31:38.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/gestures/gesture_tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      549 2023-06-09 10:31:46.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/gestures/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1770 2023-06-09 10:31:40.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/gestures/lasso_select_tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1586 2023-06-09 10:31:39.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/gestures/pan_tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1900 2023-06-09 10:31:40.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/gestures/poly_select_tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1294 2023-06-09 10:31:46.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/gestures/range_tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1343 2023-06-09 10:31:40.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/gestures/region_select_tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1778 2023-06-09 10:31:39.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/gestures/select_tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2003 2023-06-09 10:31:40.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/gestures/tap_tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1009 2023-06-09 10:31:39.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/gestures/wheel_pan_tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1324 2023-06-09 10:31:39.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/gestures/wheel_zoom_tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      391 2023-06-09 10:31:46.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/index.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.974450 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/inspectors/
+-rw-r--r--   0 runner    (1001) docker     (122)     1459 2023-06-09 10:31:40.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/inspectors/crosshair_tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      792 2023-06-09 10:31:40.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/inspectors/customjs_hover.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     4159 2023-06-09 10:31:40.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/inspectors/hover_tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      223 2023-06-09 10:31:46.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/inspectors/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      841 2023-06-09 10:31:38.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/inspectors/inspect_tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      709 2023-06-09 10:31:38.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/on_off_button.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     4774 2023-06-09 10:31:41.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1225 2023-06-09 10:31:39.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/tool_button.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1492 2023-06-09 10:31:38.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/tool_proxy.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     4551 2023-06-09 10:31:38.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/toolbar.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.974450 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/transforms/
+-rw-r--r--   0 runner    (1001) docker     (122)      978 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/transforms/customjs_transform.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      510 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/transforms/dodge.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      365 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/transforms/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1012 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/transforms/interpolator.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1192 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/transforms/jitter.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      537 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/transforms/linear_interpolator.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      831 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/transforms/range_transform.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      614 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/transforms/step_interpolator.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      628 2023-06-09 10:31:36.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/transforms/transform.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.978450 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/ui/
+-rw-r--r--   0 runner    (1001) docker     (122)     1317 2023-06-09 10:31:46.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/ui/dialog.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1685 2023-06-09 10:31:46.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/ui/examiner.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.978450 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/ui/icons/
+-rw-r--r--   0 runner    (1001) docker     (122)      905 2023-06-09 10:31:46.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/ui/icons/builtin_icon.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      623 2023-06-09 10:31:45.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/ui/icons/icon.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      163 2023-06-09 10:31:46.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/ui/icons/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      775 2023-06-09 10:31:46.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/ui/icons/svg_icon.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1067 2023-06-09 10:31:46.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/ui/icons/tabler_icon.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      244 2023-06-09 10:31:46.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/ui/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1107 2023-06-09 10:31:46.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/ui/pane.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1754 2023-06-09 10:31:40.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/ui/tooltip.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2704 2023-06-09 10:31:36.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/ui/ui_element.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      208 2023-06-09 10:31:38.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/util.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.982450 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/
+-rw-r--r--   0 runner    (1001) docker     (122)     1432 2023-06-09 10:31:47.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/abstract_button.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2666 2023-06-09 10:31:48.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/abstract_slider.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1826 2023-06-09 10:31:47.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/autocomplete_input.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1648 2023-06-09 10:31:48.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/base_date_picker.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1166 2023-06-09 10:31:48.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/base_datetime_picker.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      752 2023-06-09 10:31:47.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/button.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      946 2023-06-09 10:31:48.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/checkbox.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      866 2023-06-09 10:31:48.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/checkbox_button_group.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      810 2023-06-09 10:31:48.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/checkbox_group.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      761 2023-06-09 10:31:48.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/color_picker.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      655 2023-06-09 10:31:47.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/control.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      798 2023-06-09 10:31:48.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/date_picker.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      861 2023-06-09 10:31:48.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/date_range_picker.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      952 2023-06-09 10:31:48.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/date_range_slider.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      890 2023-06-09 10:31:48.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/date_slider.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      904 2023-06-09 10:31:48.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/datetime_picker.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      962 2023-06-09 10:31:48.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/datetime_range_picker.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      901 2023-06-09 10:31:48.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/datetime_range_slider.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      558 2023-06-09 10:31:48.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/div.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1188 2023-06-09 10:31:48.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/dropdown.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1057 2023-06-09 10:31:48.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/file_input.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      940 2023-06-09 10:31:48.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/help_button.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1884 2023-06-09 10:31:48.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1454 2023-06-09 10:31:47.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/input_widget.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)       90 2023-06-09 10:31:48.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/main.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      998 2023-06-09 10:31:48.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/markup.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1311 2023-06-09 10:31:48.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/multi_choice.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      923 2023-06-09 10:31:48.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/multiple_date_picker.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1024 2023-06-09 10:31:48.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/multiple_datetime_picker.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      873 2023-06-09 10:31:48.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/multiselect.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1403 2023-06-09 10:31:48.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/numeric_input.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      732 2023-06-09 10:31:47.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/oriented_control.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      563 2023-06-09 10:31:48.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/paragraph.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      742 2023-06-09 10:31:48.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/password_input.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1246 2023-06-09 10:31:48.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/picker_base.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      543 2023-06-09 10:31:48.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/pretext.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      810 2023-06-09 10:31:48.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/radio_button_group.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      754 2023-06-09 10:31:48.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/radio_group.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      820 2023-06-09 10:31:48.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/range_slider.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      969 2023-06-09 10:31:48.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/selectbox.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      758 2023-06-09 10:31:48.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/slider.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1492 2023-06-09 10:31:48.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/spinner.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      833 2023-06-09 10:31:48.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/switch.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.986450 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/tables/
+-rw-r--r--   0 runner    (1001) docker     (122)     6181 2023-06-09 10:31:48.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/tables/cell_editors.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     4072 2023-06-09 10:31:48.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/tables/cell_formatters.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2397 2023-06-09 10:31:49.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/tables/data_cube.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     3920 2023-06-09 10:31:49.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/tables/data_table.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      355 2023-06-09 10:31:48.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/tables/definitions.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      386 2023-06-09 10:31:49.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/tables/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)       88 2023-06-09 10:31:49.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/tables/main.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1697 2023-06-09 10:31:49.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/tables/row_aggregators.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      980 2023-06-09 10:31:48.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/tables/table_column.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      646 2023-06-09 10:31:48.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/tables/table_widget.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      859 2023-06-09 10:31:47.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/text_input.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1013 2023-06-09 10:31:47.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/text_like_input.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      834 2023-06-09 10:31:48.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/textarea_input.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1457 2023-06-09 10:31:48.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/time_picker.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      715 2023-06-09 10:31:48.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/toggle.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1199 2023-06-09 10:31:48.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/toggle_button_group.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      792 2023-06-09 10:31:48.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/toggle_input.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      996 2023-06-09 10:31:48.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/toggle_input_group.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      853 2023-06-09 10:31:47.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/widget.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.986450 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/protocol/
+-rw-r--r--   0 runner    (1001) docker     (122)       90 2023-06-09 10:31:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/protocol/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      975 2023-06-09 10:31:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/protocol/message.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      736 2023-06-09 10:31:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/protocol/receiver.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      117 2023-06-09 10:31:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/safely.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.986450 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/styles/
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-06-09 10:31:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/styles/attribution.css.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-06-09 10:31:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/styles/base.css.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      396 2023-06-09 10:31:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/styles/buttons.css.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)       73 2023-06-09 10:31:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/styles/canvas.css.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      148 2023-06-09 10:31:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/styles/caret.css.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)       48 2023-06-09 10:31:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/styles/clearfix.css.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      130 2023-06-09 10:31:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/styles/dialogs.css.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      155 2023-06-09 10:31:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/styles/dropdown.css.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-06-09 10:31:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/styles/examiner.css.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-06-09 10:31:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/styles/group_box.css.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2067 2023-06-09 10:31:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/styles/icons.css.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      102 2023-06-09 10:31:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/styles/logo.css.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      168 2023-06-09 10:31:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/styles/menus.css.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)       46 2023-06-09 10:31:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/styles/plots.css.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      263 2023-06-09 10:31:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/styles/tabs.css.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      248 2023-06-09 10:31:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/styles/tool_button.css.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      332 2023-06-09 10:31:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/styles/toolbar.css.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      380 2023-06-09 10:31:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/styles/tooltips.css.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-06-09 10:31:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/styles/ui.css.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.990450 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/styles/widgets/
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-06-09 10:31:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/styles/widgets/checkbox.css.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-06-09 10:31:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/styles/widgets/choices.css.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-06-09 10:31:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/styles/widgets/flatpickr.css.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      430 2023-06-09 10:31:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/styles/widgets/inputs.css.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-06-09 10:31:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/styles/widgets/nouislider.css.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      102 2023-06-09 10:31:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/styles/widgets/password_input.css.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-06-09 10:31:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/styles/widgets/slickgrid.css.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)       86 2023-06-09 10:31:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/styles/widgets/sliders.css.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-06-09 10:31:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/styles/widgets/switch.css.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      269 2023-06-09 10:31:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/styles/widgets/tables.css.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      303 2023-06-09 10:31:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/testing.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-09 10:31:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/version.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.998450 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/
+-rw-r--r--   0 runner    (1001) docker     (122)    12714 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.decorators.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1326 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.decorators.legacy.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)   824027 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.dom.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)    16886 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.dom.iterable.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     5203 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2015.collection.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)    21204 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2015.core.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1241 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2015.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2552 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2015.generator.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)    14892 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2015.iterable.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     3199 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2015.promise.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     5251 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2015.proxy.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     6493 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2015.reflect.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1648 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2015.symbol.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)    10621 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2015.symbol.wellknown.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     4861 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2016.array.include.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      928 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2016.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1031 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2016.full.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1083 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2017.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1031 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2017.full.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1439 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2017.intl.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2451 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2017.object.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     6227 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2017.sharedmemory.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2378 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2017.string.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1425 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2017.typedarrays.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2687 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2018.asyncgenerator.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1753 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2018.asynciterable.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1088 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2018.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1031 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2018.full.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     3076 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2018.intl.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1352 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2018.promise.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1227 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2018.regexp.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     3173 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2019.array.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1071 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2019.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1032 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2019.full.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      955 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2019.intl.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1472 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2019.object.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1528 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2019.string.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1006 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2019.symbol.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)    35366 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2020.bigint.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1201 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2020.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2955 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2020.date.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1032 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2020.full.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)    20994 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2020.intl.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1587 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2020.number.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1802 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2020.promise.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     4749 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2020.sharedmemory.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1237 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2020.string.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1455 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2020.symbol.wellknown.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1036 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2021.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1032 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2021.full.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     8378 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2021.intl.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2259 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2021.promise.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1592 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2021.string.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2739 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2021.weakref.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     4258 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2022.array.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1152 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2022.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2337 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2022.error.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1032 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2022.full.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     5563 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2022.intl.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1085 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2022.object.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1336 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2022.regexp.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2081 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2022.sharedmemory.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1155 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2022.string.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)    21108 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2023.array.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      921 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2023.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1032 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2023.full.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)   212834 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es5.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1032 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es6.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      920 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.esnext.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1031 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.esnext.full.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1192 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.esnext.intl.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     9453 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.scripthost.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)   273794 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.webworker.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1042 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.webworker.importscripts.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)    12132 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.webworker.iterable.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)    31831 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/tornado.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4014 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/urls.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7787 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:29.002450 bokeh-3.2.0.dev4/src/bokeh/server/views/
+-rw-r--r--   0 runner    (1001) docker     (122)      331 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7033 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/views/app_index.html
+-rw-r--r--   0 runner    (1001) docker     (122)     3207 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/views/auth_request_handler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3817 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/views/autoload_js_handler.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15086 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/views/bokeh-dev.ico
+-rw-r--r--   0 runner    (1001) docker     (122)    15086 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/views/bokeh.ico
+-rw-r--r--   0 runner    (1001) docker     (122)     2631 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/views/doc_handler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2239 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/views/ico_handler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2571 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/views/metadata_handler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2871 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/views/multi_root_static_handler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2840 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/views/root_handler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6493 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/views/session_handler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3205 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/views/static_handler.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13576 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/server/views/ws.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26423 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:29.006450 bokeh-3.2.0.dev4/src/bokeh/sphinxext/
+-rw-r--r--   0 runner    (1001) docker     (122)      929 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sphinxext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:29.006450 bokeh-3.2.0.dev4/src/bokeh/sphinxext/_templates/
+-rw-r--r--   0 runner    (1001) docker     (122)     2608 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sphinxext/_templates/bokehjs_codepen_init.html
+-rw-r--r--   0 runner    (1001) docker     (122)      383 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sphinxext/_templates/bokehjs_content_epilogue.html
+-rw-r--r--   0 runner    (1001) docker     (122)       95 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sphinxext/_templates/bokehjs_content_prologue.html
+-rw-r--r--   0 runner    (1001) docker     (122)      480 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sphinxext/_templates/bokehjs_html_template.html
+-rw-r--r--   0 runner    (1001) docker     (122)      204 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sphinxext/_templates/color_detail.html
+-rw-r--r--   0 runner    (1001) docker     (122)      417 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sphinxext/_templates/enum_detail.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      230 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sphinxext/_templates/example_metadata.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      199 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sphinxext/_templates/gallery_detail.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      641 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sphinxext/_templates/gallery_page.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      314 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sphinxext/_templates/jinja_detail.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      325 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sphinxext/_templates/model_detail.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      153 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sphinxext/_templates/options_detail.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      243 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sphinxext/_templates/palette_detail.html
+-rw-r--r--   0 runner    (1001) docker     (122)      481 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sphinxext/_templates/palette_group_detail.html
+-rw-r--r--   0 runner    (1001) docker     (122)      171 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sphinxext/_templates/prop_detail.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1269 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sphinxext/_templates/release_detail.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      302 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sphinxext/_templates/settings_detail.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     4320 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sphinxext/bokeh_autodoc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2912 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sphinxext/bokeh_color.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3465 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sphinxext/bokeh_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2725 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sphinxext/bokeh_directive.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4423 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sphinxext/bokeh_enum.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4784 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sphinxext/bokeh_example_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6570 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sphinxext/bokeh_gallery.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3964 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sphinxext/bokeh_jinja.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6135 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sphinxext/bokeh_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4828 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sphinxext/bokeh_options.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4784 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sphinxext/bokeh_palette.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4099 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sphinxext/bokeh_palette_group.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12661 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sphinxext/bokeh_plot.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4988 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sphinxext/bokeh_prop.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3398 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sphinxext/bokeh_releases.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8083 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sphinxext/bokeh_roles.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7577 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sphinxext/bokeh_sampledata_xref.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4275 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sphinxext/bokeh_settings.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3791 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sphinxext/bokeh_sitemap.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9589 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sphinxext/bokehjs_content.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4630 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sphinxext/example_handler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2600 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sphinxext/sample.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3247 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sphinxext/templates.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3004 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/sphinxext/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:29.006450 bokeh-3.2.0.dev4/src/bokeh/themes/
+-rw-r--r--   0 runner    (1001) docker     (122)     2904 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/themes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2243 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/themes/_caliber.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2382 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/themes/_contrast.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2382 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/themes/_dark_minimal.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1970 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/themes/_light_minimal.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2382 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/themes/_night_sky.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9267 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/themes/theme.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8284 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/tile_providers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14776 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:29.010450 bokeh-3.2.0.dev4/src/bokeh/util/
+-rw-r--r--   0 runner    (1001) docker     (122)     2528 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4707 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/util/browser.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7856 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/util/callback_manager.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18959 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/util/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2711 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/util/dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3827 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/util/datatypes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2924 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/util/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3121 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/util/deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2303 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/util/functions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8426 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/util/hex.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3600 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/util/logconfig.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3043 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/util/options.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4391 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/util/package.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2505 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/util/paths.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1872 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/util/sampledata.json
+-rw-r--r--   0 runner    (1001) docker     (122)     7969 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/util/sampledata.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11396 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/util/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5419 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/util/strings.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3646 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/util/terminal.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12872 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/util/token.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11285 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/util/tornado.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2944 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/util/version.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3153 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/src/bokeh/util/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:28.834447 bokeh-3.2.0.dev4/src/bokeh.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    12082 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    55013 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       46 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      128 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       14 2023-06-09 10:33:28.000000 bokeh-3.2.0.dev4/src/bokeh.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 10:33:29.010450 bokeh-3.2.0.dev4/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     2002 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/tests/test_bokehjs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6178 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/tests/test_cross.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2588 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/tests/test_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10468 2023-06-09 10:22:43.000000 bokeh-3.2.0.dev4/tests/test_examples.py
```

### Comparing `bokeh-3.2.0.dev3/LICENSE.txt` & `bokeh-3.2.0.dev4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/MANIFEST.in` & `bokeh-3.2.0.dev4/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/PKG-INFO` & `bokeh-3.2.0.dev4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bokeh
-Version: 3.2.0.dev3
+Version: 3.2.0.dev4
 Summary: Interactive plots and applications in the browser from Python
 Author: Bokeh Team
 Author-email: info@bokeh.org
 License: Copyright (c) 2012 - 2023, Anaconda, Inc., and Bokeh Contributors
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without modification,
```

### Comparing `bokeh-3.2.0.dev3/README.md` & `bokeh-3.2.0.dev4/README.md`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/pyproject.toml` & `bokeh-3.2.0.dev4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/setup.py` & `bokeh-3.2.0.dev4/setup.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/LICENSE.txt` & `bokeh-3.2.0.dev4/src/bokeh/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/__init__.py` & `bokeh-3.2.0.dev4/src/bokeh/__init__.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/__main__.py` & `bokeh-3.2.0.dev4/src/bokeh/__main__.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/_sri.json` & `bokeh-3.2.0.dev4/src/bokeh/_sri.json`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/application/__init__.py` & `bokeh-3.2.0.dev4/src/bokeh/application/__init__.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/application/application.py` & `bokeh-3.2.0.dev4/src/bokeh/application/application.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/application/handlers/__init__.py` & `bokeh-3.2.0.dev4/src/bokeh/application/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/application/handlers/code.py` & `bokeh-3.2.0.dev4/src/bokeh/application/handlers/code.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/application/handlers/code_runner.py` & `bokeh-3.2.0.dev4/src/bokeh/application/handlers/code_runner.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/application/handlers/directory.py` & `bokeh-3.2.0.dev4/src/bokeh/application/handlers/directory.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/application/handlers/document_lifecycle.py` & `bokeh-3.2.0.dev4/src/bokeh/application/handlers/document_lifecycle.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/application/handlers/function.py` & `bokeh-3.2.0.dev4/src/bokeh/application/handlers/function.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/application/handlers/handler.py` & `bokeh-3.2.0.dev4/src/bokeh/application/handlers/handler.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/application/handlers/lifecycle.py` & `bokeh-3.2.0.dev4/src/bokeh/application/handlers/lifecycle.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/application/handlers/notebook.py` & `bokeh-3.2.0.dev4/src/bokeh/application/handlers/notebook.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/application/handlers/request_handler.py` & `bokeh-3.2.0.dev4/src/bokeh/application/handlers/request_handler.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/application/handlers/script.py` & `bokeh-3.2.0.dev4/src/bokeh/application/handlers/script.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/application/handlers/server_lifecycle.py` & `bokeh-3.2.0.dev4/src/bokeh/application/handlers/server_lifecycle.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/application/handlers/server_request_handler.py` & `bokeh-3.2.0.dev4/src/bokeh/application/handlers/server_request_handler.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/client/__init__.py` & `bokeh-3.2.0.dev4/src/bokeh/client/__init__.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/client/connection.py` & `bokeh-3.2.0.dev4/src/bokeh/client/connection.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/client/session.py` & `bokeh-3.2.0.dev4/src/bokeh/client/session.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/client/states.py` & `bokeh-3.2.0.dev4/src/bokeh/client/states.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/client/util.py` & `bokeh-3.2.0.dev4/src/bokeh/client/util.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/client/websocket.py` & `bokeh-3.2.0.dev4/src/bokeh/client/websocket.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/colors/__init__.py` & `bokeh-3.2.0.dev4/src/bokeh/colors/__init__.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/colors/color.py` & `bokeh-3.2.0.dev4/src/bokeh/colors/color.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/colors/groups.py` & `bokeh-3.2.0.dev4/src/bokeh/colors/groups.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/colors/named.py` & `bokeh-3.2.0.dev4/src/bokeh/colors/named.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/colors/util.py` & `bokeh-3.2.0.dev4/src/bokeh/colors/util.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/command/__init__.py` & `bokeh-3.2.0.dev4/src/bokeh/command/__init__.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/command/bootstrap.py` & `bokeh-3.2.0.dev4/src/bokeh/command/bootstrap.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/command/subcommand.py` & `bokeh-3.2.0.dev4/src/bokeh/command/subcommand.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/command/subcommands/__init__.py` & `bokeh-3.2.0.dev4/src/bokeh/command/subcommands/__init__.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/command/subcommands/build.py` & `bokeh-3.2.0.dev4/src/bokeh/command/subcommands/build.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/command/subcommands/file_output.py` & `bokeh-3.2.0.dev4/src/bokeh/command/subcommands/file_output.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/command/subcommands/info.py` & `bokeh-3.2.0.dev4/src/bokeh/command/subcommands/info.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/command/subcommands/init.py` & `bokeh-3.2.0.dev4/src/bokeh/command/subcommands/init.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/command/subcommands/json.py` & `bokeh-3.2.0.dev4/src/bokeh/command/subcommands/json.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/command/subcommands/sampledata.py` & `bokeh-3.2.0.dev4/src/bokeh/command/subcommands/sampledata.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/command/subcommands/secret.py` & `bokeh-3.2.0.dev4/src/bokeh/command/subcommands/secret.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/command/subcommands/serve.py` & `bokeh-3.2.0.dev4/src/bokeh/command/subcommands/serve.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/command/subcommands/static.py` & `bokeh-3.2.0.dev4/src/bokeh/command/subcommands/static.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/command/util.py` & `bokeh-3.2.0.dev4/src/bokeh/command/util.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/core/__init__.py` & `bokeh-3.2.0.dev4/src/bokeh/core/__init__.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/core/_templates/autoload_js.js` & `bokeh-3.2.0.dev4/src/bokeh/core/_templates/autoload_js.js`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/core/_templates/autoload_nb_js.js` & `bokeh-3.2.0.dev4/src/bokeh/core/_templates/autoload_nb_js.js`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/core/_templates/autoload_request_tag.html` & `bokeh-3.2.0.dev4/src/bokeh/core/_templates/autoload_request_tag.html`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/core/_templates/autoload_tag.html` & `bokeh-3.2.0.dev4/src/bokeh/core/_templates/autoload_tag.html`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/core/_templates/file.html` & `bokeh-3.2.0.dev4/src/bokeh/core/_templates/file.html`

 * *Files 0% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     <meta charset="utf-8">
     <title>{% block title %}{{ title | e if title else "Bokeh Plot" }}{% endblock %}</title>
   {%  block preamble -%}{%- endblock %}
   {%  block resources %}
     <style>
       html, body {
         box-sizing: border-box;
+        display: flow-root;
         height: 100%;
         margin: 0;
         padding: 0;
       }
     </style>
   {%   block css_resources -%}
     {{- bokeh_css if bokeh_css }}
```

### Comparing `bokeh-3.2.0.dev3/src/bokeh/core/_templates/js_resources.html` & `bokeh-3.2.0.dev4/src/bokeh/core/_templates/js_resources.html`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/core/_templates/notebook_load.html` & `bokeh-3.2.0.dev4/src/bokeh/core/_templates/notebook_load.html`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/core/_templates/try_run.js` & `bokeh-3.2.0.dev4/src/bokeh/core/_templates/try_run.js`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/core/enums.py` & `bokeh-3.2.0.dev4/src/bokeh/core/enums.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/core/has_props.py` & `bokeh-3.2.0.dev4/src/bokeh/core/has_props.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/core/json_encoder.py` & `bokeh-3.2.0.dev4/src/bokeh/core/json_encoder.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/core/properties.py` & `bokeh-3.2.0.dev4/src/bokeh/core/properties.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/core/property/__init__.py` & `bokeh-3.2.0.dev4/src/bokeh/core/property/__init__.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/core/property/_sphinx.py` & `bokeh-3.2.0.dev4/src/bokeh/core/property/_sphinx.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/core/property/alias.py` & `bokeh-3.2.0.dev4/src/bokeh/core/property/alias.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/core/property/aliases.py` & `bokeh-3.2.0.dev4/src/bokeh/core/property/aliases.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/core/property/any.py` & `bokeh-3.2.0.dev4/src/bokeh/core/property/any.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/core/property/auto.py` & `bokeh-3.2.0.dev4/src/bokeh/core/property/auto.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/core/property/bases.py` & `bokeh-3.2.0.dev4/src/bokeh/core/property/bases.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/core/property/color.py` & `bokeh-3.2.0.dev4/src/bokeh/core/property/color.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/core/property/container.py` & `bokeh-3.2.0.dev4/src/bokeh/core/property/container.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/core/property/dataspec.py` & `bokeh-3.2.0.dev4/src/bokeh/core/property/dataspec.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/core/property/datetime.py` & `bokeh-3.2.0.dev4/src/bokeh/core/property/datetime.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/core/property/descriptor_factory.py` & `bokeh-3.2.0.dev4/src/bokeh/core/property/descriptor_factory.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/core/property/descriptors.py` & `bokeh-3.2.0.dev4/src/bokeh/core/property/descriptors.py`

 * *Files 1% similar despite different names*

```diff
@@ -526,21 +526,24 @@
         if self.name in obj._property_values:
             # this shouldn't happen because we should have checked before _get_default()
             raise RuntimeError("Bokeh internal error, does not handle the case of self.name already in _property_values")
 
         themed_values = obj.themed_values()
         is_themed = themed_values is not None and self.name in themed_values
 
-        default = self.instance_default(obj)
-
         unstable_dict = obj._unstable_themed_values if is_themed else obj._unstable_default_values
 
         if self.name in unstable_dict:
             return unstable_dict[self.name]
 
+        # Ensure we do not look up the default until after we check if it already present
+        # in the unstable_dict because it is a very expensive operation
+        # Ref: https://github.com/bokeh/bokeh/pull/13174
+        default = self.instance_default(obj)
+
         if self.has_unstable_default(obj):
             if isinstance(default, PropertyValueContainer):
                 default._register_owner(obj, self)
             unstable_dict[self.name] = default
 
         return default
```

### Comparing `bokeh-3.2.0.dev3/src/bokeh/core/property/either.py` & `bokeh-3.2.0.dev4/src/bokeh/core/property/either.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/core/property/enum.py` & `bokeh-3.2.0.dev4/src/bokeh/core/property/enum.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/core/property/factors.py` & `bokeh-3.2.0.dev4/src/bokeh/core/property/factors.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/core/property/include.py` & `bokeh-3.2.0.dev4/src/bokeh/core/property/include.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/core/property/instance.py` & `bokeh-3.2.0.dev4/src/bokeh/core/property/instance.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/core/property/json.py` & `bokeh-3.2.0.dev4/src/bokeh/core/property/json.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/core/property/nothing.py` & `bokeh-3.2.0.dev4/src/bokeh/core/property/nothing.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/core/property/nullable.py` & `bokeh-3.2.0.dev4/src/bokeh/core/property/nullable.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/core/property/numeric.py` & `bokeh-3.2.0.dev4/src/bokeh/core/property/numeric.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/core/property/override.py` & `bokeh-3.2.0.dev4/src/bokeh/core/property/override.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/core/property/pd.py` & `bokeh-3.2.0.dev4/src/bokeh/core/property/pd.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/core/property/primitive.py` & `bokeh-3.2.0.dev4/src/bokeh/core/property/primitive.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/core/property/readonly.py` & `bokeh-3.2.0.dev4/src/bokeh/core/property/readonly.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/core/property/required.py` & `bokeh-3.2.0.dev4/src/bokeh/core/property/required.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/core/property/serialized.py` & `bokeh-3.2.0.dev4/src/bokeh/core/property/serialized.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/core/property/singletons.py` & `bokeh-3.2.0.dev4/src/bokeh/core/property/singletons.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/core/property/string.py` & `bokeh-3.2.0.dev4/src/bokeh/core/property/string.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/core/property/struct.py` & `bokeh-3.2.0.dev4/src/bokeh/core/property/struct.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/core/property/text_like.py` & `bokeh-3.2.0.dev4/src/bokeh/core/property/text_like.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/core/property/validation.py` & `bokeh-3.2.0.dev4/src/bokeh/core/property/validation.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/core/property/vectorization.py` & `bokeh-3.2.0.dev4/src/bokeh/core/property/vectorization.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/core/property/visual.py` & `bokeh-3.2.0.dev4/src/bokeh/core/property/visual.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/core/property/wrappers.py` & `bokeh-3.2.0.dev4/src/bokeh/core/property/wrappers.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/core/property_aliases.py` & `bokeh-3.2.0.dev4/src/bokeh/core/property_aliases.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/core/property_mixins.py` & `bokeh-3.2.0.dev4/src/bokeh/core/property_mixins.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/core/query.py` & `bokeh-3.2.0.dev4/src/bokeh/core/query.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/core/serialization.py` & `bokeh-3.2.0.dev4/src/bokeh/core/serialization.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/core/templates.py` & `bokeh-3.2.0.dev4/src/bokeh/core/templates.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/core/types.py` & `bokeh-3.2.0.dev4/src/bokeh/core/types.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/core/validation/__init__.py` & `bokeh-3.2.0.dev4/src/bokeh/core/validation/__init__.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/core/validation/check.py` & `bokeh-3.2.0.dev4/src/bokeh/core/validation/check.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/core/validation/decorators.py` & `bokeh-3.2.0.dev4/src/bokeh/core/validation/decorators.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/core/validation/errors.py` & `bokeh-3.2.0.dev4/src/bokeh/core/validation/errors.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/core/validation/issue.py` & `bokeh-3.2.0.dev4/src/bokeh/core/validation/issue.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/core/validation/warnings.py` & `bokeh-3.2.0.dev4/src/bokeh/core/validation/warnings.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/document/__init__.py` & `bokeh-3.2.0.dev4/src/bokeh/document/__init__.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/document/callbacks.py` & `bokeh-3.2.0.dev4/src/bokeh/document/callbacks.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/document/document.py` & `bokeh-3.2.0.dev4/src/bokeh/document/document.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/document/events.py` & `bokeh-3.2.0.dev4/src/bokeh/document/events.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/document/json.py` & `bokeh-3.2.0.dev4/src/bokeh/document/json.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/document/locking.py` & `bokeh-3.2.0.dev4/src/bokeh/document/locking.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/document/models.py` & `bokeh-3.2.0.dev4/src/bokeh/document/models.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/document/modules.py` & `bokeh-3.2.0.dev4/src/bokeh/document/modules.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/driving.py` & `bokeh-3.2.0.dev4/src/bokeh/driving.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/embed/__init__.py` & `bokeh-3.2.0.dev4/src/bokeh/embed/__init__.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/embed/bundle.py` & `bokeh-3.2.0.dev4/src/bokeh/embed/bundle.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/embed/elements.py` & `bokeh-3.2.0.dev4/src/bokeh/embed/elements.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/embed/notebook.py` & `bokeh-3.2.0.dev4/src/bokeh/embed/notebook.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/embed/server.py` & `bokeh-3.2.0.dev4/src/bokeh/embed/server.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/embed/standalone.py` & `bokeh-3.2.0.dev4/src/bokeh/embed/standalone.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     AUTOLOAD_TAG,
     FILE,
     MACROS,
     ROOT_DIV,
 )
 from ..document.document import DEFAULT_TITLE, Document
 from ..model import Model
-from ..resources import Resources
+from ..resources import Resources, ResourcesLike
 from ..themes import Theme
 from .bundle import Script, bundle_for_objs_and_resources
 from .elements import html_page_for_render_items, script_for_render_items
 from .util import (
     FromCurdoc,
     OutputDocumentFor,
     RenderRoot,
@@ -288,16 +288,17 @@
         result = dict_type(zip(model_keys, results))
     else:
         result = tuple(results)
 
     return script, result
 
 def file_html(models: Model | Document | Sequence[Model],
-              resources: Resources | None,
+              resources: ResourcesLike | None = None,
               title: str | None = None,
+              *,
               template: Template | str = FILE,
               template_variables: dict[str, Any] = {},
               theme: ThemeLike = None,
               suppress_callback_warning: bool = False,
               _always_new: bool = False) -> str:
     ''' Return an HTML document that embeds Bokeh Model or Document objects.
 
@@ -305,16 +306,16 @@
     support for customizing the JS/CSS resources independently and
     customizing the jinja2 template.
 
     Args:
         models (Model or Document or seq[Model]) : Bokeh object or objects to render
             typically a Model or Document
 
-        resources (Resources) :
-            A resource configuration for Bokeh JS & CSS assets.
+        resources (ResourcesLike) :
+            A resources configuration for Bokeh JS & CSS assets.
 
         title (str, optional) :
             A title for the HTML document ``<title>`` tags or None. (default: None)
 
             If None, attempt to automatically find the Document title from the given
             plot objects.
 
@@ -338,25 +339,26 @@
             cannot function. However, this warning can be suppressed by setting
             this value to True (default: False)
 
     Returns:
         UTF-8 encoded HTML
 
     '''
-
     models_seq: Sequence[Model] = []
     if isinstance(models, Model):
         models_seq = [models]
     elif isinstance(models, Document):
         if len(models.roots) == 0:
             raise ValueError("Document has no root Models")
         models_seq = models.roots
     else:
         models_seq = models
 
+    resources = Resources.build(resources)
+
     with OutputDocumentFor(models_seq, apply_theme=theme, always_new=_always_new) as doc:
         (docs_json, render_items) = standalone_docs_json_and_render_items(models_seq, suppress_callback_warning=suppress_callback_warning)
         title = _title_from_models(models_seq, title)
         bundle = bundle_for_objs_and_resources([doc], resources)
         return html_page_for_render_items(bundle, docs_json, render_items, title=title,
                                           template=template, template_variables=template_variables)
```

### Comparing `bokeh-3.2.0.dev3/src/bokeh/embed/util.py` & `bokeh-3.2.0.dev4/src/bokeh/embed/util.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/embed/wrappers.py` & `bokeh-3.2.0.dev4/src/bokeh/embed/wrappers.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/events.py` & `bokeh-3.2.0.dev4/src/bokeh/events.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/ext.py` & `bokeh-3.2.0.dev4/src/bokeh/ext.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/io/__init__.py` & `bokeh-3.2.0.dev4/src/bokeh/io/__init__.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/io/doc.py` & `bokeh-3.2.0.dev4/src/bokeh/io/doc.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/io/export.py` & `bokeh-3.2.0.dev4/src/bokeh/io/export.py`

 * *Files 0% similar despite different names*

```diff
@@ -314,15 +314,23 @@
             overflow: hidden;
         }
     </style>
     {% endblock %}
     """
 
     def html() -> str:
-        return file_html(obj, resources, title="", template=template, theme=theme, suppress_callback_warning=True, _always_new=True)
+        return file_html(
+            obj,
+            resources=resources,
+            title="",
+            template=template,
+            theme=theme,
+            suppress_callback_warning=True,
+            _always_new=True,
+        )
 
     if width is not None or height is not None:
         # Defer this import, it is expensive
         from ..models.plots import Plot
         if not isinstance(obj, Plot):
             warn("Export method called with width or height argument on a non-Plot model. The size values will be ignored.")
         else:
```

### Comparing `bokeh-3.2.0.dev3/src/bokeh/io/notebook.py` & `bokeh-3.2.0.dev4/src/bokeh/io/notebook.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/io/output.py` & `bokeh-3.2.0.dev4/src/bokeh/io/output.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/io/saving.py` & `bokeh-3.2.0.dev4/src/bokeh/io/saving.py`

 * *Files 1% similar despite different names*

```diff
@@ -157,15 +157,15 @@
 
 def _save_helper(obj: UIElement | Sequence[UIElement], filename: PathLike, resources: Resources | None,
         title: str | None, template: Template | str | None, theme: Theme | None = None) -> None:
     '''
 
     '''
     from ..embed import file_html
-    html = file_html(obj, resources, title=title, template=template or FILE, theme=theme)
+    html = file_html(obj, resources=resources, title=title, template=template or FILE, theme=theme)
 
     with open(filename, mode="w", encoding="utf-8") as f:
         f.write(html)
 
 #-----------------------------------------------------------------------------
 # Code
 #-----------------------------------------------------------------------------
```

### Comparing `bokeh-3.2.0.dev3/src/bokeh/io/showing.py` & `bokeh-3.2.0.dev4/src/bokeh/io/showing.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/io/state.py` & `bokeh-3.2.0.dev4/src/bokeh/io/state.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/io/util.py` & `bokeh-3.2.0.dev4/src/bokeh/io/util.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/io/webdriver.py` & `bokeh-3.2.0.dev4/src/bokeh/io/webdriver.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/layouts.py` & `bokeh-3.2.0.dev4/src/bokeh/layouts.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/model/__init__.py` & `bokeh-3.2.0.dev4/src/bokeh/model/__init__.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/model/data_model.py` & `bokeh-3.2.0.dev4/src/bokeh/model/data_model.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/model/docs.py` & `bokeh-3.2.0.dev4/src/bokeh/model/docs.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/model/model.py` & `bokeh-3.2.0.dev4/src/bokeh/model/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 from .util import HasDocumentRef, collect_models, visit_value_and_its_immediate_references
 
 if TYPE_CHECKING:
     from ..core.has_props import Setter
     from ..core.query import SelectorType
     from ..document import Document
     from ..document.events import DocumentPatchedEvent
-    from ..models.callbacks import Callback as JSEventCallback
+    from ..models.callbacks import Callback as JSEventCallback, CustomCode as JSChangeCallback
     from ..util.callback_manager import PropertyCallback
 
 #-----------------------------------------------------------------------------
 # Globals and constants
 #-----------------------------------------------------------------------------
 
 __all__ = (
@@ -394,15 +394,15 @@
         from bokeh.models import CustomJS
 
         selector = f"[{attr_selector!r}]" if attr_selector is not None else ""
         cb = CustomJS(args=dict(other=other), code=f"other.{other_descriptor.name} = this.{descriptor.name}{selector}")
 
         self.js_on_change(attr, cb)
 
-    def js_on_change(self, event: str, *callbacks: JSEventCallback) -> None:
+    def js_on_change(self, event: str, *callbacks: JSChangeCallback) -> None:
         ''' Attach a :class:`~bokeh.models.CustomJS` callback to an arbitrary
         BokehJS model event.
 
         On the BokehJS side, change events for model properties have the
         form ``"change:property_name"``. As a convenience, if the event name
         passed to this method is also the name of a property on the model,
         then it will be prefixed with ``"change:"`` automatically:
@@ -423,17 +423,17 @@
             source.js_on_change('streaming', callback)
 
         '''
         if len(callbacks) == 0:
             raise ValueError("js_on_change takes an event name and one or more callbacks, got only one parameter")
 
         # handle any CustomJS callbacks here
-        from bokeh.models import CustomJS
-        if not all(isinstance(x, CustomJS) for x in callbacks):
-            raise ValueError("not all callback values are CustomJS instances")
+        from bokeh.models.callbacks import CustomCode
+        if not all(isinstance(x, CustomCode) for x in callbacks):
+            raise ValueError("not all callback values are CustomCode instances")
 
         descriptor = self.lookup(event, raises=False)
         if descriptor is not None:
             event = f"change:{descriptor.name}"
 
         old = {k: [cb for cb in cbs] for k, cbs in self.js_property_callbacks.items()}
         if event not in self.js_property_callbacks:
```

### Comparing `bokeh-3.2.0.dev3/src/bokeh/model/util.py` & `bokeh-3.2.0.dev4/src/bokeh/model/util.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/models/__init__.py` & `bokeh-3.2.0.dev4/src/bokeh/models/__init__.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/models/annotations/__init__.py` & `bokeh-3.2.0.dev4/src/bokeh/models/annotations/__init__.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/models/annotations/annotation.py` & `bokeh-3.2.0.dev4/src/bokeh/models/annotations/annotation.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/models/annotations/arrows.py` & `bokeh-3.2.0.dev4/src/bokeh/models/annotations/arrows.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/models/annotations/geometry.py` & `bokeh-3.2.0.dev4/src/bokeh/models/annotations/geometry.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/models/annotations/html/__init__.py` & `bokeh-3.2.0.dev4/src/bokeh/models/annotations/html/__init__.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/models/annotations/html/html_annotation.py` & `bokeh-3.2.0.dev4/src/bokeh/models/annotations/html/html_annotation.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/models/annotations/html/labels.py` & `bokeh-3.2.0.dev4/src/bokeh/models/annotations/html/labels.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/models/annotations/html/toolbars.py` & `bokeh-3.2.0.dev4/src/bokeh/models/annotations/html/toolbars.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/models/annotations/labels.py` & `bokeh-3.2.0.dev4/src/bokeh/models/annotations/labels.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/models/annotations/legends.py` & `bokeh-3.2.0.dev4/src/bokeh/models/annotations/legends.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/models/axes.py` & `bokeh-3.2.0.dev4/src/bokeh/models/axes.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/models/callbacks.py` & `bokeh-3.2.0.dev4/src/bokeh/models/callbacks.py`

 * *Files 19% similar despite different names*

```diff
@@ -17,33 +17,39 @@
 log = logging.getLogger(__name__)
 
 #-----------------------------------------------------------------------------
 # Imports
 #-----------------------------------------------------------------------------
 
 # Standard library imports
-from typing import Any as any
+import pathlib
+from typing import TYPE_CHECKING, Any as any
 
 # Bokeh imports
 from ..core.has_props import HasProps, abstract
 from ..core.properties import (
     Any,
     AnyRef,
+    Auto,
     Bool,
     Dict,
+    Either,
     Instance,
     Required,
     String,
 )
 from ..core.property.bases import Init
 from ..core.property.singletons import Intrinsic
 from ..core.validation import error
 from ..core.validation.errors import INVALID_PROPERTY_VALUE, NOT_A_PROPERTY_OF
 from ..model import Model
 
+if TYPE_CHECKING:
+    from ..core.types import PathLike
+
 #-----------------------------------------------------------------------------
 # Globals and constants
 #-----------------------------------------------------------------------------
 
 __all__ = (
     'Callback',
     'OpenURL',
@@ -61,15 +67,14 @@
 
     '''
 
     # explicit __init__ to support Init signatures
     def __init__(self, *args, **kwargs) -> None:
         super().__init__(*args, **kwargs)
 
-
 class OpenURL(Callback):
     ''' Open a URL in a new or current tab or window.
 
     '''
 
     # explicit __init__ to support Init signatures
     def __init__(self, *args, **kwargs) -> None:
@@ -82,44 +87,109 @@
 
     same_tab = Bool(False, help="""
     Open URL in a new (`False`, default) or current (`True`) tab or window.
     For `same_tab=False`, whether tab or window will be opened is browser
     dependent.
     """)
 
-class CustomJS(Callback):
+class CustomCode(Callback):
+    """ """
+
+    # explicit __init__ to support Init signatures
+    def __init__(self, *args, **kwargs) -> None:
+        super().__init__(*args, **kwargs)
+
+class CustomJS(CustomCode):
     ''' Execute a JavaScript function.
 
     .. warning::
         The explicit purpose of this Bokeh Model is to embed *raw JavaScript
         code* for a browser to execute. If any part of the code is derived
         from untrusted user inputs, then you must take appropriate care to
         sanitize the user input prior to passing to Bokeh.
 
     '''
 
     # explicit __init__ to support Init signatures
     def __init__(self, *args, **kwargs) -> None:
         super().__init__(*args, **kwargs)
 
-    args = Dict(String, AnyRef, help="""
+    args = Dict(String, AnyRef)(default={}, help="""
     A mapping of names to Python objects. In particular those can be bokeh's models.
     These objects are made available to the callback's code snippet as the values of
     named parameters to the callback.
     """)
 
-    code = String(default="", help="""
-    A snippet of JavaScript code to execute in the browser. The
-    code is made into the body of a function, and all of of the named objects in
+    code = Required(String)(help="""
+    A snippet of JavaScript code to execute in the browser.
+
+    This can be interpreted either as a JavaScript function or a module, depending
+    on the ``module`` property:
+
+    1. A JS function.
+
+    The code is made into the body of a function, and all of of the named objects in
     ``args`` are available as parameters that the code can use. Additionally,
     a ``cb_obj`` parameter contains the object that triggered the callback
     and an optional ``cb_data`` parameter that contains any tool-specific data
     (i.e. mouse coordinates and hovered glyph indices for the ``HoverTool``).
+
+    2. An ES module.
+
+    A JavaScript module (ESM) exporting a default function with the following
+    signature:
+
+    .. code-block: javascript
+
+        export default function(args, obj, data) {
+            // program logic
+        }
+
+    where ``args`` is a key-value mapping of user-provided parameters, ``obj``
+    refers to the object that triggered the callback, and ``data`` is a key-value
+    mapping of optional parameters provided by the caller.
+
+    This function can be an asynchronous function (``async function``).
     """)
 
+    module = Either(Auto, Bool, default="auto", help="""
+    Whether to interpret the code as a JS function or ES module. If set to
+    ``"auto"``, the this will be inferred from the code.
+    """)
+
+    @classmethod
+    def from_file(cls, path: PathLike, **args: any) -> CustomJS:
+        """
+        Construct a ``CustomJS`` instance from a ``*.js`` or ``*.mjs`` file.
+
+        For example, if we want to construct a ``CustomJS`` instance from
+        a JavaScript module ``my_module.mjs``, that takes a single argument
+        ``source``, then we would use:
+
+        .. code-block: python
+
+            from bokeh.models import ColumnDataSrouce, CustomJS
+            source = ColumnDataSource(data=dict(x=[1, 2, 3]))
+            CustomJS.from_file("./my_module.mjs", source=source)
+
+        """
+        path = pathlib.Path(path)
+
+        if path.suffix == ".js":
+            module = False
+        elif path.suffix == ".mjs":
+            module = True
+        else:
+            raise RuntimeError(f"expected a *.js or *.mjs file, got {path}")
+
+        with open(path, encoding="utf-8") as file:
+            code = file.read()
+
+        return CustomJS(code=code, args=args, module=module)
+
 class SetValue(Callback):
     """ Allows to update a property of an object. """
 
     # explicit __init__ to support Init signatures
     def __init__(self, obj: Init[HasProps] = Intrinsic, attr: Init[str] = Intrinsic, value: Init[any] = Intrinsic, **kwargs) -> None:
         super().__init__(obj=obj, attr=attr, value=value, **kwargs)
```

### Comparing `bokeh-3.2.0.dev3/src/bokeh/models/canvas.py` & `bokeh-3.2.0.dev4/src/bokeh/models/canvas.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/models/coordinates.py` & `bokeh-3.2.0.dev4/src/bokeh/models/coordinates.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/models/css.py` & `bokeh-3.2.0.dev4/src/bokeh/models/css.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/models/dom.py` & `bokeh-3.2.0.dev4/src/bokeh/models/dom.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/models/expressions.py` & `bokeh-3.2.0.dev4/src/bokeh/models/expressions.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/models/filters.py` & `bokeh-3.2.0.dev4/src/bokeh/models/filters.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/models/formatters.py` & `bokeh-3.2.0.dev4/src/bokeh/models/formatters.py`

 * *Files 0% similar despite different names*

```diff
@@ -399,15 +399,15 @@
 
 class DatetimeTickFormatter(TickFormatter):
     ''' A ``TickFormatter`` for displaying datetime values nicely across a
     range of scales.
 
     ``DatetimeTickFormatter`` has the following properties (listed together
     with their default values) that can be used to control the formatting
-    of axis ticks at different scales scales:
+    of axis ticks at different scales:
 
     .. code-block:: python
 
         {defaults}
 
     Each scale property can be set to format or list of formats to use for
     formatting datetime tick values that fall in in that "time scale".
```

### Comparing `bokeh-3.2.0.dev3/src/bokeh/models/glyph.py` & `bokeh-3.2.0.dev4/src/bokeh/models/glyph.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/models/glyphs.py` & `bokeh-3.2.0.dev4/src/bokeh/models/glyphs.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/models/graphics.py` & `bokeh-3.2.0.dev4/src/bokeh/models/graphics.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/models/graphs.py` & `bokeh-3.2.0.dev4/src/bokeh/models/graphs.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/models/grids.py` & `bokeh-3.2.0.dev4/src/bokeh/models/grids.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/models/labeling.py` & `bokeh-3.2.0.dev4/src/bokeh/models/labeling.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/models/layouts.py` & `bokeh-3.2.0.dev4/src/bokeh/models/layouts.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/models/map_plots.py` & `bokeh-3.2.0.dev4/src/bokeh/models/map_plots.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/models/mappers.py` & `bokeh-3.2.0.dev4/src/bokeh/models/mappers.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/models/plots.py` & `bokeh-3.2.0.dev4/src/bokeh/models/plots.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/models/ranges.py` & `bokeh-3.2.0.dev4/src/bokeh/models/ranges.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/models/renderers/__init__.py` & `bokeh-3.2.0.dev4/src/bokeh/models/renderers/__init__.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/models/renderers/contour_renderer.py` & `bokeh-3.2.0.dev4/src/bokeh/models/renderers/contour_renderer.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/models/renderers/glyph_renderer.py` & `bokeh-3.2.0.dev4/src/bokeh/models/renderers/glyph_renderer.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/models/renderers/graph_renderer.py` & `bokeh-3.2.0.dev4/src/bokeh/models/renderers/graph_renderer.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/models/renderers/renderer.py` & `bokeh-3.2.0.dev4/src/bokeh/models/renderers/renderer.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/models/renderers/tile_renderer.py` & `bokeh-3.2.0.dev4/src/bokeh/models/renderers/tile_renderer.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/models/scales.py` & `bokeh-3.2.0.dev4/src/bokeh/models/scales.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/models/selections.py` & `bokeh-3.2.0.dev4/src/bokeh/models/selections.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/models/selectors.py` & `bokeh-3.2.0.dev4/src/bokeh/models/selectors.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/models/sources.py` & `bokeh-3.2.0.dev4/src/bokeh/models/sources.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/models/text.py` & `bokeh-3.2.0.dev4/src/bokeh/models/text.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/models/textures.py` & `bokeh-3.2.0.dev4/src/bokeh/models/textures.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/models/tickers.py` & `bokeh-3.2.0.dev4/src/bokeh/models/tickers.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/models/tiles.py` & `bokeh-3.2.0.dev4/src/bokeh/models/tiles.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/models/tools.py` & `bokeh-3.2.0.dev4/src/bokeh/models/tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -544,15 +544,28 @@
     further zooming all dimensions. If False, zooming can continue
     independently in any dimension that has not yet reached its bounds, even if
     that causes overall focus or aspect ratio to change.
     """)
 
     zoom_on_axis = Bool(default=True, help="""
     Whether scrolling on an axis (outside the central plot area) should zoom
-    that dimension.
+    that dimension. If enabled, the behavior of this feature can be configured
+    with ``zoom_together`` property.
+    """)
+
+    zoom_together = Enum("none", "cross", "all", default="all", help="""
+    Defines the behavior of the tool when zooming on an axis:
+
+    - ``"none"`` - zoom only the axis that's being interacted with. Any cross
+    axes, nor any other axes in the dimension of this axis will be affected.
+    - ``"cross"`` - zoom the axis that's being interactd with and its cross
+    axis, if configured. No other axes in this or cross dimension will be
+    affected.
+    - ``"all"`` - zoom all axes in the dimension of the axis that's being
+    interacted with. All cross axes will be unaffected.
     """)
 
     speed = Float(default=1/600, help="""
     Speed at which the wheel zooms. Default is 1/600. Optimal range is between
     0.001 and 0.09. High values will be clipped. Speed may very between browsers.
     """)
 
@@ -861,15 +874,28 @@
     """)
 
     origin = Enum("corner", "center", default="corner", help="""
     Indicates whether the rectangular zoom area should originate from a corner
     (top-left or bottom-right depending on direction) or the center of the box.
     """)
 
-class ZoomInTool(PlotActionTool):
+@abstract
+class ZoomBaseTool(PlotActionTool):
+    """ Abstract base class for zoom action tools. """
+
+    # explicit __init__ to support Init signatures
+    def __init__(self, *args, **kwargs) -> None:
+        super().__init__(*args, **kwargs)
+
+    renderers = Either(Auto, List(Instance(DataRenderer)), default="auto", help="""
+    Restrict zoom to ranges used by the provided data renderers. If ``"auto"``
+    then all ranges provided by the cartesian frame will be used.
+    """)
+
+class ZoomInTool(ZoomBaseTool):
     ''' *toolbar icon*: |zoom_in_icon|
 
     The zoom-in tool allows users to click a button to zoom in
     by a fixed amount.
 
     .. |zoom_in_icon| image:: /_images/icons/ZoomIn.png
         :height: 24px
@@ -889,15 +915,15 @@
     height of the plot.
     """)
 
     factor = Percent(default=0.1, help="""
     Percentage to zoom for each click of the zoom-in tool.
     """)
 
-class ZoomOutTool(PlotActionTool):
+class ZoomOutTool(ZoomBaseTool):
     ''' *toolbar icon*: |zoom_out_icon|
 
     The zoom-out tool allows users to click a button to zoom out
     by a fixed amount.
 
     .. |zoom_out_icon| image:: /_images/icons/ZoomOut.png
         :height: 24px
```

### Comparing `bokeh-3.2.0.dev3/src/bokeh/models/transforms.py` & `bokeh-3.2.0.dev4/src/bokeh/models/transforms.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/models/ui/__init__.py` & `bokeh-3.2.0.dev4/src/bokeh/models/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/models/ui/dialogs.py` & `bokeh-3.2.0.dev4/src/bokeh/models/ui/dialogs.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/models/ui/examiner.py` & `bokeh-3.2.0.dev4/src/bokeh/models/ui/examiner.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/models/ui/icons.py` & `bokeh-3.2.0.dev4/src/bokeh/models/ui/icons.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/models/ui/menus.py` & `bokeh-3.2.0.dev4/src/bokeh/models/ui/menus.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/models/ui/panes.py` & `bokeh-3.2.0.dev4/src/bokeh/models/ui/panes.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/models/ui/tooltips.py` & `bokeh-3.2.0.dev4/src/bokeh/models/ui/tooltips.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/models/ui/ui_element.py` & `bokeh-3.2.0.dev4/src/bokeh/models/ui/ui_element.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/models/util/__init__.py` & `bokeh-3.2.0.dev4/src/bokeh/models/util/__init__.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/models/util/structure.py` & `bokeh-3.2.0.dev4/src/bokeh/models/util/structure.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/models/widgets/__init__.py` & `bokeh-3.2.0.dev4/src/bokeh/models/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/models/widgets/buttons.py` & `bokeh-3.2.0.dev4/src/bokeh/models/widgets/buttons.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/models/widgets/groups.py` & `bokeh-3.2.0.dev4/src/bokeh/models/widgets/groups.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/models/widgets/inputs.py` & `bokeh-3.2.0.dev4/src/bokeh/models/widgets/inputs.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/models/widgets/markups.py` & `bokeh-3.2.0.dev4/src/bokeh/models/widgets/markups.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/models/widgets/pickers.py` & `bokeh-3.2.0.dev4/src/bokeh/models/widgets/pickers.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/models/widgets/sliders.py` & `bokeh-3.2.0.dev4/src/bokeh/models/widgets/sliders.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/models/widgets/tables.py` & `bokeh-3.2.0.dev4/src/bokeh/models/widgets/tables.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/models/widgets/widget.py` & `bokeh-3.2.0.dev4/src/bokeh/models/widgets/widget.py`

 * *Files 15% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 
 #-----------------------------------------------------------------------------
 # Imports
 #-----------------------------------------------------------------------------
 
 # Bokeh imports
 from ...core.has_props import abstract
+from ...core.properties import Override
 from ..layouts import LayoutDOM
 
 #-----------------------------------------------------------------------------
 # Globals and constants
 #-----------------------------------------------------------------------------
 
 __all__ = (
@@ -51,14 +52,16 @@
 
     '''
 
     # explicit __init__ to support Init signatures
     def __init__(self, *args, **kwargs) -> None:
         super().__init__(*args, **kwargs)
 
+    margin = Override(default=5)
+
 #-----------------------------------------------------------------------------
 # Private API
 #-----------------------------------------------------------------------------
 
 #-----------------------------------------------------------------------------
 # Code
 #-----------------------------------------------------------------------------
```

### Comparing `bokeh-3.2.0.dev3/src/bokeh/palettes.py` & `bokeh-3.2.0.dev4/src/bokeh/palettes.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/plotting/__init__.py` & `bokeh-3.2.0.dev4/src/bokeh/plotting/__init__.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/plotting/_decorators.py` & `bokeh-3.2.0.dev4/src/bokeh/plotting/_decorators.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/plotting/_docstring.py` & `bokeh-3.2.0.dev4/src/bokeh/plotting/_docstring.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/plotting/_figure.py` & `bokeh-3.2.0.dev4/src/bokeh/plotting/_figure.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/plotting/_graph.py` & `bokeh-3.2.0.dev4/src/bokeh/plotting/_graph.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/plotting/_legends.py` & `bokeh-3.2.0.dev4/src/bokeh/plotting/_legends.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/plotting/_plot.py` & `bokeh-3.2.0.dev4/src/bokeh/plotting/_plot.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/plotting/_renderer.py` & `bokeh-3.2.0.dev4/src/bokeh/plotting/_renderer.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/plotting/_stack.py` & `bokeh-3.2.0.dev4/src/bokeh/plotting/_stack.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/plotting/_tools.py` & `bokeh-3.2.0.dev4/src/bokeh/plotting/_tools.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/plotting/contour.py` & `bokeh-3.2.0.dev4/src/bokeh/plotting/contour.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/plotting/glyph_api.py` & `bokeh-3.2.0.dev4/src/bokeh/plotting/glyph_api.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/plotting/gmap.py` & `bokeh-3.2.0.dev4/src/bokeh/plotting/gmap.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/plotting/graph.py` & `bokeh-3.2.0.dev4/src/bokeh/plotting/graph.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/protocol/__init__.py` & `bokeh-3.2.0.dev4/src/bokeh/protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/protocol/exceptions.py` & `bokeh-3.2.0.dev4/src/bokeh/protocol/exceptions.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/protocol/message.py` & `bokeh-3.2.0.dev4/src/bokeh/protocol/message.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/protocol/messages/__init__.py` & `bokeh-3.2.0.dev4/src/bokeh/protocol/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/protocol/messages/ack.py` & `bokeh-3.2.0.dev4/src/bokeh/protocol/messages/ack.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/protocol/messages/error.py` & `bokeh-3.2.0.dev4/src/bokeh/protocol/messages/error.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/protocol/messages/ok.py` & `bokeh-3.2.0.dev4/src/bokeh/protocol/messages/ok.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/protocol/messages/patch_doc.py` & `bokeh-3.2.0.dev4/src/bokeh/protocol/messages/patch_doc.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/protocol/messages/pull_doc_reply.py` & `bokeh-3.2.0.dev4/src/bokeh/protocol/messages/pull_doc_reply.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/protocol/messages/pull_doc_req.py` & `bokeh-3.2.0.dev4/src/bokeh/protocol/messages/pull_doc_req.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/protocol/messages/push_doc.py` & `bokeh-3.2.0.dev4/src/bokeh/protocol/messages/push_doc.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/protocol/messages/server_info_reply.py` & `bokeh-3.2.0.dev4/src/bokeh/protocol/messages/server_info_reply.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/protocol/messages/server_info_req.py` & `bokeh-3.2.0.dev4/src/bokeh/protocol/messages/server_info_req.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/protocol/receiver.py` & `bokeh-3.2.0.dev4/src/bokeh/protocol/receiver.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/resources.py` & `bokeh-3.2.0.dev4/src/bokeh/resources.py`

 * *Files 2% similar despite different names*

```diff
@@ -411,14 +411,21 @@
             args.append("dev=True")
         if self.components != self._default_components:
             args.append(f"components={self.components!r}")
         return f"Resources({', '.join(args)})"
 
     __str__ = __repr__
 
+    @classmethod
+    def build(cls, resources: ResourcesLike | None = None) -> Resources:
+        if isinstance(resources, Resources):
+            return resources
+        else:
+            return Resources(mode=settings.resources(resources))
+
     # Properties --------------------------------------------------------------
 
     @property
     def log_level(self) -> LogLevel:
         return self._log_level
 
     @log_level.setter
@@ -636,16 +643,19 @@
         result.hashes = lambda components, kind: {
             mk_url(component, kind): sri_hashes[mk_filename(component, kind)] for component in components
         }
 
     return result
 
 
-def _get_server_urls(root_url: str, minified: bool = True,
-        path_versioner: PathVersioner | None = None) -> Urls:
+def _get_server_urls(
+    root_url: str = DEFAULT_SERVER_HTTP_URL,
+    minified: bool = True,
+    path_versioner: PathVersioner | None = None,
+) -> Urls:
     _minified = ".min" if minified else ""
 
     def mk_url(comp: str, kind: Kind) -> str:
         path = f"{kind}/{comp}{_minified}.{kind}"
         if path_versioner is not None:
             path = path_versioner(path)
         return f"{root_url}static/{path}"
```

### Comparing `bokeh-3.2.0.dev3/src/bokeh/sampledata/__init__.py` & `bokeh-3.2.0.dev4/src/bokeh/sampledata/__init__.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/sampledata/_data/USHolidays.ics` & `bokeh-3.2.0.dev4/src/bokeh/sampledata/_data/USHolidays.ics`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/sampledata/_data/US_Regions_State_Boundaries.csv.gz` & `bokeh-3.2.0.dev4/src/bokeh/sampledata/_data/US_Regions_State_Boundaries.csv.gz`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/sampledata/_data/auto-mpg.csv` & `bokeh-3.2.0.dev4/src/bokeh/sampledata/_data/auto-mpg.csv`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/sampledata/_data/auto-mpg2.csv` & `bokeh-3.2.0.dev4/src/bokeh/sampledata/_data/auto-mpg2.csv`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/sampledata/_data/browsers_nov_2013.csv` & `bokeh-3.2.0.dev4/src/bokeh/sampledata/_data/browsers_nov_2013.csv`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/sampledata/_data/commits.txt.gz` & `bokeh-3.2.0.dev4/src/bokeh/sampledata/_data/commits.txt.gz`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/sampledata/_data/daylight_warsaw_2013.csv` & `bokeh-3.2.0.dev4/src/bokeh/sampledata/_data/daylight_warsaw_2013.csv`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/sampledata/_data/elements.csv` & `bokeh-3.2.0.dev4/src/bokeh/sampledata/_data/elements.csv`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/sampledata/_data/icons/chrome_32x32.png` & `bokeh-3.2.0.dev4/src/bokeh/sampledata/_data/icons/chrome_32x32.png`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/sampledata/_data/icons/firefox_32x32.png` & `bokeh-3.2.0.dev4/src/bokeh/sampledata/_data/icons/firefox_32x32.png`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/sampledata/_data/icons/ie_32x32.png` & `bokeh-3.2.0.dev4/src/bokeh/sampledata/_data/icons/ie_32x32.png`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/sampledata/_data/icons/opera_32x32.png` & `bokeh-3.2.0.dev4/src/bokeh/sampledata/_data/icons/opera_32x32.png`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/sampledata/_data/icons/safari_32x32.png` & `bokeh-3.2.0.dev4/src/bokeh/sampledata/_data/icons/safari_32x32.png`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/sampledata/_data/iris.csv` & `bokeh-3.2.0.dev4/src/bokeh/sampledata/_data/iris.csv`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/sampledata/_data/les_mis.json` & `bokeh-3.2.0.dev4/src/bokeh/sampledata/_data/les_mis.json`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/sampledata/_data/numberly.csv` & `bokeh-3.2.0.dev4/src/bokeh/sampledata/_data/numberly.csv`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/sampledata/_data/obiszow_mtb_xcm.csv` & `bokeh-3.2.0.dev4/src/bokeh/sampledata/_data/obiszow_mtb_xcm.csv`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/sampledata/_data/olympics2014.json` & `bokeh-3.2.0.dev4/src/bokeh/sampledata/_data/olympics2014.json`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/sampledata/_data/penguins.csv` & `bokeh-3.2.0.dev4/src/bokeh/sampledata/_data/penguins.csv`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/sampledata/_data/percent-bachelors-degrees-women-usa.csv` & `bokeh-3.2.0.dev4/src/bokeh/sampledata/_data/percent-bachelors-degrees-women-usa.csv`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/sampledata/_data/probly.csv` & `bokeh-3.2.0.dev4/src/bokeh/sampledata/_data/probly.csv`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/sampledata/_data/sample_geojson.geojson` & `bokeh-3.2.0.dev4/src/bokeh/sampledata/_data/sample_geojson.geojson`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/sampledata/_data/sea_surface_temperature.csv.gz` & `bokeh-3.2.0.dev4/src/bokeh/sampledata/_data/sea_surface_temperature.csv.gz`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/sampledata/_data/sprint.csv` & `bokeh-3.2.0.dev4/src/bokeh/sampledata/_data/sprint.csv`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/sampledata/_data/unemployment1948.csv` & `bokeh-3.2.0.dev4/src/bokeh/sampledata/_data/unemployment1948.csv`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/sampledata/_data/us_marriages_divorces.csv` & `bokeh-3.2.0.dev4/src/bokeh/sampledata/_data/us_marriages_divorces.csv`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/sampledata/airport_routes.py` & `bokeh-3.2.0.dev4/src/bokeh/sampledata/airport_routes.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/sampledata/airports.py` & `bokeh-3.2.0.dev4/src/bokeh/sampledata/airports.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/sampledata/anscombe.py` & `bokeh-3.2.0.dev4/src/bokeh/sampledata/anscombe.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/sampledata/antibiotics.py` & `bokeh-3.2.0.dev4/src/bokeh/sampledata/antibiotics.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/sampledata/autompg.py` & `bokeh-3.2.0.dev4/src/bokeh/sampledata/autompg.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/sampledata/autompg2.py` & `bokeh-3.2.0.dev4/src/bokeh/sampledata/autompg2.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/sampledata/browsers.py` & `bokeh-3.2.0.dev4/src/bokeh/sampledata/browsers.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/sampledata/commits.py` & `bokeh-3.2.0.dev4/src/bokeh/sampledata/commits.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/sampledata/daylight.py` & `bokeh-3.2.0.dev4/src/bokeh/sampledata/daylight.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/sampledata/degrees.py` & `bokeh-3.2.0.dev4/src/bokeh/sampledata/degrees.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/sampledata/gapminder.py` & `bokeh-3.2.0.dev4/src/bokeh/sampledata/gapminder.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/sampledata/glucose.py` & `bokeh-3.2.0.dev4/src/bokeh/sampledata/glucose.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/sampledata/haar_cascade.py` & `bokeh-3.2.0.dev4/src/bokeh/sampledata/haar_cascade.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/sampledata/iris.py` & `bokeh-3.2.0.dev4/src/bokeh/sampledata/iris.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/sampledata/les_mis.py` & `bokeh-3.2.0.dev4/src/bokeh/sampledata/les_mis.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/sampledata/movies_data.py` & `bokeh-3.2.0.dev4/src/bokeh/sampledata/movies_data.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/sampledata/mtb.py` & `bokeh-3.2.0.dev4/src/bokeh/sampledata/mtb.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/sampledata/olympics2014.py` & `bokeh-3.2.0.dev4/src/bokeh/sampledata/olympics2014.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/sampledata/penguins.py` & `bokeh-3.2.0.dev4/src/bokeh/sampledata/penguins.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/sampledata/perceptions.py` & `bokeh-3.2.0.dev4/src/bokeh/sampledata/perceptions.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/sampledata/periodic_table.py` & `bokeh-3.2.0.dev4/src/bokeh/sampledata/periodic_table.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/sampledata/population.py` & `bokeh-3.2.0.dev4/src/bokeh/sampledata/population.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/sampledata/sample_geojson.py` & `bokeh-3.2.0.dev4/src/bokeh/sampledata/sample_geojson.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/sampledata/sample_superstore.py` & `bokeh-3.2.0.dev4/src/bokeh/sampledata/sample_superstore.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/sampledata/sea_surface_temperature.py` & `bokeh-3.2.0.dev4/src/bokeh/sampledata/sea_surface_temperature.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/sampledata/sprint.py` & `bokeh-3.2.0.dev4/src/bokeh/sampledata/sprint.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/sampledata/stocks.py` & `bokeh-3.2.0.dev4/src/bokeh/sampledata/stocks.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/sampledata/unemployment.py` & `bokeh-3.2.0.dev4/src/bokeh/sampledata/unemployment.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/sampledata/unemployment1948.py` & `bokeh-3.2.0.dev4/src/bokeh/sampledata/unemployment1948.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/sampledata/us_cities.py` & `bokeh-3.2.0.dev4/src/bokeh/sampledata/us_cities.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/sampledata/us_counties.py` & `bokeh-3.2.0.dev4/src/bokeh/sampledata/us_counties.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/sampledata/us_holidays.py` & `bokeh-3.2.0.dev4/src/bokeh/sampledata/us_holidays.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/sampledata/us_marriages_divorces.py` & `bokeh-3.2.0.dev4/src/bokeh/sampledata/us_marriages_divorces.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/sampledata/us_states.py` & `bokeh-3.2.0.dev4/src/bokeh/sampledata/us_states.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/sampledata/world_cities.py` & `bokeh-3.2.0.dev4/src/bokeh/sampledata/world_cities.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/__init__.py` & `bokeh-3.2.0.dev4/src/bokeh/server/__init__.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/auth_provider.py` & `bokeh-3.2.0.dev4/src/bokeh/server/auth_provider.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/callbacks.py` & `bokeh-3.2.0.dev4/src/bokeh/server/callbacks.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/connection.py` & `bokeh-3.2.0.dev4/src/bokeh/server/connection.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/contexts.py` & `bokeh-3.2.0.dev4/src/bokeh/server/contexts.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/protocol_handler.py` & `bokeh-3.2.0.dev4/src/bokeh/server/protocol_handler.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/server.py` & `bokeh-3.2.0.dev4/src/bokeh/server/server.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/session.py` & `bokeh-3.2.0.dev4/src/bokeh/server/session.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/bokeh-api.js` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/bokeh-api.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -25,15 +25,15 @@
  * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
  * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
  * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
  * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF
  * THE POSSIBILITY OF SUCH DAMAGE.
  */
 (function(root, factory) {
-    factory(root["Bokeh"], "3.2.0-dev.3");
+    factory(root["Bokeh"], "3.2.0-dev.4");
 })(this, function(Bokeh, version) {
     let define;
     return (function(modules, entry, aliases, externals) {
             const bokeh = typeof Bokeh !== "undefined" && (version != null ? Bokeh[version] : Bokeh);
             if (bokeh != null) {
                 return bokeh.register_plugin(modules, entry, aliases);
             } else {
```

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/bokeh-api.min.js` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/bokeh-api.min.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -25,15 +25,15 @@
  * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
  * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
  * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
  * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF
  * THE POSSIBILITY OF SUCH DAMAGE.
  */
 (function(root, factory) {
-    factory(root["Bokeh"], "3.2.0-dev.3");
+    factory(root["Bokeh"], "3.2.0-dev.4");
 })(this, function(Bokeh, version) {
     let define;
     return (function(modules, entry, aliases, externals) {
             const bokeh = typeof Bokeh !== "undefined" && (version != null ? Bokeh[version] : Bokeh);
             if (bokeh != null) {
                 return bokeh.register_plugin(modules, entry, aliases);
             } else {
```

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/bokeh-gl.js` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/bokeh-gl.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -25,15 +25,15 @@
  * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
  * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
  * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
  * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF
  * THE POSSIBILITY OF SUCH DAMAGE.
  */
 (function(root, factory) {
-    factory(root["Bokeh"], "3.2.0-dev.3");
+    factory(root["Bokeh"], "3.2.0-dev.4");
 })(this, function(Bokeh, version) {
     let define;
     return (function(modules, entry, aliases, externals) {
             const bokeh = typeof Bokeh !== "undefined" && (version != null ? Bokeh[version] : Bokeh);
             if (bokeh != null) {
                 return bokeh.register_plugin(modules, entry, aliases);
             } else {
@@ -11408,14 +11408,15 @@
                 const buffer_1 = require(525) /* ./buffer */ ;
                 const webgl_utils_1 = require(526) /* ./webgl_utils */ ;
                 const color_1 = require(21) /* ../../../core/util/color */ ;
                 const line_1 = require(76) /* ../../../core/visuals/line */ ;
                 class BaseLineGL extends base_1.BaseGLGlyph {
                     constructor(regl_wrapper, glyph) {
                         super(regl_wrapper, glyph);
+                        this._line_dash = null;
                         this.glyph = glyph;
                         this._antialias = 1.5; // Make this larger to test antialiasing at edges.
                         this._miter_limit = 10.0; // Threshold for miters to be replaced by bevels.
                     }
                     _draw_impl(indices, transform, main_gl_glyph) {
                         if (this.visuals_changed) {
                             this._set_visuals();
```

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/bokeh-gl.min.js` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/bokeh-gl.min.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -25,15 +25,15 @@
  * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
  * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
  * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
  * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF
  * THE POSSIBILITY OF SUCH DAMAGE.
  */
 (function(root, factory) {
-    factory(root["Bokeh"], "3.2.0-dev.3");
+    factory(root["Bokeh"], "3.2.0-dev.4");
 })(this, function(Bokeh, version) {
     let define;
     return (function(modules, entry, aliases, externals) {
             const bokeh = typeof Bokeh !== "undefined" && (version != null ? Bokeh[version] : Bokeh);
             if (bokeh != null) {
                 return bokeh.register_plugin(modules, entry, aliases);
             } else {
@@ -5243,15 +5243,15 @@
                 const h = s(524),
                     a = s(525),
                     l = s(526),
                     n = s(21),
                     o = s(76);
                 class r extends h.BaseGLGlyph {
                     constructor(s, i) {
-                        super(s, i), this.glyph = i, this._antialias = 1.5, this._miter_limit = 10
+                        super(s, i), this._line_dash = null, this.glyph = i, this._antialias = 1.5, this._miter_limit = 10
                     }
                     _draw_impl(s, i, t) {
                         this.visuals_changed && (this._set_visuals(), this.visuals_changed = !1), t.data_changed && (t._set_data(), t.data_changed = !1);
                         const _ = this._get_visuals().line,
                             e = l.cap_lookup[_.line_cap.value],
                             h = l.join_lookup[_.line_join.value],
                             a = t._points,
```

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/bokeh-mathjax.js` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/bokeh-mathjax.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -25,15 +25,15 @@
  * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
  * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
  * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
  * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF
  * THE POSSIBILITY OF SUCH DAMAGE.
  */
 (function(root, factory) {
-    factory(root["Bokeh"], "3.2.0-dev.3");
+    factory(root["Bokeh"], "3.2.0-dev.4");
 })(this, function(Bokeh, version) {
     let define;
     return (function(modules, entry, aliases, externals) {
             const bokeh = typeof Bokeh !== "undefined" && (version != null ? Bokeh[version] : Bokeh);
             if (bokeh != null) {
                 return bokeh.register_plugin(modules, entry, aliases);
             } else {
```

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/bokeh-mathjax.min.js` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/bokeh-mathjax.min.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -25,15 +25,15 @@
  * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
  * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
  * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
  * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF
  * THE POSSIBILITY OF SUCH DAMAGE.
  */
 (function(root, factory) {
-    factory(root["Bokeh"], "3.2.0-dev.3");
+    factory(root["Bokeh"], "3.2.0-dev.4");
 })(this, function(Bokeh, version) {
     let define;
     return (function(modules, entry, aliases, externals) {
             const bokeh = typeof Bokeh !== "undefined" && (version != null ? Bokeh[version] : Bokeh);
             if (bokeh != null) {
                 return bokeh.register_plugin(modules, entry, aliases);
             } else {
```

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/bokeh-tables.js` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/bokeh-tables.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -25,15 +25,15 @@
  * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
  * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
  * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
  * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF
  * THE POSSIBILITY OF SUCH DAMAGE.
  */
 (function(root, factory) {
-    factory(root["Bokeh"], "3.2.0-dev.3");
+    factory(root["Bokeh"], "3.2.0-dev.4");
 })(this, function(Bokeh, version) {
     let define;
     return (function(modules, entry, aliases, externals) {
             const bokeh = typeof Bokeh !== "undefined" && (version != null ? Bokeh[version] : Bokeh);
             if (bokeh != null) {
                 return bokeh.register_plugin(modules, entry, aliases);
             } else {
@@ -20657,24 +20657,19 @@
                     };
                 }
                 module.exports = {
                     GroupItemMetadataProvider: GroupItemMetadataProvider
                 };
             },
             651: /* models/widgets/widget.js */ function _(require, module, exports, __esModule, __esExport) {
+                var _a;
                 __esModule();
                 const layout_dom_1 = require(367) /* ../layouts/layout_dom */ ;
                 const providers_1 = require(154) /* ../text/providers */ ;
                 class WidgetView extends layout_dom_1.LayoutDOMView {
-                    update_style() {
-                        super.update_style();
-                        this.style.append(":host", {
-                            margin: "5px"
-                        });
-                    }
                     get child_models() {
                         return [];
                     }
                     get provider() {
                         return providers_1.default_provider;
                     }
                     async lazy_initialize() {
@@ -20714,15 +20709,21 @@
                 WidgetView.__name__ = "WidgetView";
                 class Widget extends layout_dom_1.LayoutDOM {
                     constructor(attrs) {
                         super(attrs);
                     }
                 }
                 exports.Widget = Widget;
+                _a = Widget;
                 Widget.__name__ = "Widget";
+                (() => {
+                    _a.override({
+                        margin: 5,
+                    });
+                })();
             },
             652: /* models/widgets/tables/table_widget.js */ function _(require, module, exports, __esModule, __esExport) {
                 var _a;
                 __esModule();
                 const widget_1 = require(651) /* ../widget */ ;
                 const column_data_source_1 = require(104) /* ../../sources/column_data_source */ ;
                 const cds_view_1 = require(218) /* ../../sources/cds_view */ ;
```

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/bokeh-tables.min.js` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/bokeh-tables.min.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -25,15 +25,15 @@
  * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
  * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
  * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
  * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF
  * THE POSSIBILITY OF SUCH DAMAGE.
  */
 (function(root, factory) {
-    factory(root["Bokeh"], "3.2.0-dev.3");
+    factory(root["Bokeh"], "3.2.0-dev.4");
 })(this, function(Bokeh, version) {
     let define;
     return (function(modules, entry, aliases, externals) {
             const bokeh = typeof Bokeh !== "undefined" && (version != null ? Bokeh[version] : Bokeh);
             if (bokeh != null) {
                 return bokeh.register_plugin(modules, entry, aliases);
             } else {
@@ -9203,57 +9203,55 @@
                             setOptions: function(e) {
                                 a.extend(!0, o, e)
                             }
                         }
                     }
                 }
             },
-            651: function _(t, e, i, s, r) {
-                s();
-                const a = t(367),
-                    n = t(154);
-                class d extends a.LayoutDOMView {
-                    update_style() {
-                        super.update_style(), this.style.append(":host", {
-                            margin: "5px"
-                        })
-                    }
+            651: function _(t, e, i, r, s) {
+                var a;
+                r();
+                const n = t(367),
+                    o = t(154);
+                class d extends n.LayoutDOMView {
                     get child_models() {
                         return []
                     }
                     get provider() {
-                        return n.default_provider
+                        return o.default_provider
                     }
                     async lazy_initialize() {
                         await super.lazy_initialize(), "not_started" == this.provider.status && await this.provider.fetch()
                     }
                     _after_layout() {
                         super._after_layout(), "loading" == this.provider.status && (this._has_finished = !1)
                     }
                     process_tex(t) {
                         if (null == this.provider.MathJax) return t;
                         const e = this.provider.MathJax.find_tex(t),
                             i = [];
-                        let s = 0;
-                        for (const r of e) i.push(t.slice(s, r.start.n)), i.push(this.provider.MathJax.tex2svg(r.math, {
-                            display: r.display
-                        }).outerHTML), s = r.end.n;
-                        return s < t.length && i.push(t.slice(s)), i.join("")
+                        let r = 0;
+                        for (const s of e) i.push(t.slice(r, s.start.n)), i.push(this.provider.MathJax.tex2svg(s.math, {
+                            display: s.display
+                        }).outerHTML), r = s.end.n;
+                        return r < t.length && i.push(t.slice(r)), i.join("")
                     }
                     contains_tex_string(t) {
                         return null != this.provider.MathJax && this.provider.MathJax.find_tex(t).length > 0
                     }
                 }
                 i.WidgetView = d, d.__name__ = "WidgetView";
-                class o extends a.LayoutDOM {
+                class _ extends n.LayoutDOM {
                     constructor(t) {
                         super(t)
                     }
                 }
-                i.Widget = o, o.__name__ = "Widget"
+                i.Widget = _, a = _, _.__name__ = "Widget", a.override({
+                    margin: 5
+                })
             },
             652: function _(e, n, t, a, o) {
                 var c;
                 a();
                 const i = e(651),
                     u = e(104),
                     r = e(218);
```

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/bokeh-widgets.js` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/bokeh-widgets.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -25,15 +25,15 @@
  * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
  * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
  * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
  * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF
  * THE POSSIBILITY OF SUCH DAMAGE.
  */
 (function(root, factory) {
-    factory(root["Bokeh"], "3.2.0-dev.3");
+    factory(root["Bokeh"], "3.2.0-dev.4");
 })(this, function(Bokeh, version) {
     let define;
     return (function(modules, entry, aliases, externals) {
             const bokeh = typeof Bokeh !== "undefined" && (version != null ? Bokeh[version] : Bokeh);
             if (bokeh != null) {
                 return bokeh.register_plugin(modules, entry, aliases);
             } else {
@@ -241,24 +241,19 @@
                         super(attrs);
                     }
                 }
                 exports.Control = Control;
                 Control.__name__ = "Control";
             },
             651: /* models/widgets/widget.js */ function _(require, module, exports, __esModule, __esExport) {
+                var _a;
                 __esModule();
                 const layout_dom_1 = require(367) /* ../layouts/layout_dom */ ;
                 const providers_1 = require(154) /* ../text/providers */ ;
                 class WidgetView extends layout_dom_1.LayoutDOMView {
-                    update_style() {
-                        super.update_style();
-                        this.style.append(":host", {
-                            margin: "5px"
-                        });
-                    }
                     get child_models() {
                         return [];
                     }
                     get provider() {
                         return providers_1.default_provider;
                     }
                     async lazy_initialize() {
@@ -298,15 +293,21 @@
                 WidgetView.__name__ = "WidgetView";
                 class Widget extends layout_dom_1.LayoutDOM {
                     constructor(attrs) {
                         super(attrs);
                     }
                 }
                 exports.Widget = Widget;
+                _a = Widget;
                 Widget.__name__ = "Widget";
+                (() => {
+                    _a.override({
+                        margin: 5,
+                    });
+                })();
             },
             558: /* styles/buttons.css.js */ function _(require, module, exports, __esModule, __esExport) {
                 __esModule();
                 exports.btn = "bk-btn";
                 exports.active = "bk-active";
                 exports.btn_default = "bk-btn-default";
                 exports.btn_primary = "bk-btn-primary";
@@ -1367,21 +1368,28 @@
                         });
                         this.connect(min_date.change, () => this.picker.set("minDate", this.model.min_date));
                         this.connect(max_date.change, () => this.picker.set("maxDate", this.model.max_date));
                         this.connect(disabled_dates.change, () => {
                             const {
                                 disabled_dates
                             } = this.model;
-                            this.picker.set("disable", disabled_dates != null ? this._convert_date_list(disabled_dates) : undefined);
+                            this.picker.set("disable", disabled_dates != null ? this._convert_date_list(disabled_dates) : []);
                         });
                         this.connect(enabled_dates.change, () => {
                             const {
                                 enabled_dates
                             } = this.model;
-                            this.picker.set("enable", enabled_dates != null ? this._convert_date_list(enabled_dates) : undefined);
+                            if (enabled_dates != null) {
+                                this.picker.set("enable", this._convert_date_list(enabled_dates));
+                            } else {
+                                // this reimplements `set()` for the `undefined` case
+                                this.picker.config._enable = undefined;
+                                this.picker.redraw();
+                                this.picker.updateValue(true);
+                            }
                         });
                         this.connect(date_format.change, () => this.picker.set("altFormat", this.model.date_format));
                     }
                     get flatpickr_options() {
                         const {
                             value,
                             min_date,
```

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/bokeh-widgets.min.js` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/bokeh-widgets.min.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -25,15 +25,15 @@
  * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
  * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
  * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
  * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF
  * THE POSSIBILITY OF SUCH DAMAGE.
  */
 (function(root, factory) {
-    factory(root["Bokeh"], "3.2.0-dev.3");
+    factory(root["Bokeh"], "3.2.0-dev.4");
 })(this, function(Bokeh, version) {
     let define;
     return (function(modules, entry, aliases, externals) {
             const bokeh = typeof Bokeh !== "undefined" && (version != null ? Bokeh[version] : Bokeh);
             if (bokeh != null) {
                 return bokeh.register_plugin(modules, entry, aliases);
             } else {
@@ -134,57 +134,55 @@
                 class _ extends c.Widget {
                     constructor(t) {
                         super(t)
                     }
                 }
                 o.Control = _, _.__name__ = "Control"
             },
-            651: function _(t, e, i, s, r) {
-                s();
-                const a = t(367),
-                    n = t(154);
-                class d extends a.LayoutDOMView {
-                    update_style() {
-                        super.update_style(), this.style.append(":host", {
-                            margin: "5px"
-                        })
-                    }
+            651: function _(t, e, i, r, s) {
+                var a;
+                r();
+                const n = t(367),
+                    o = t(154);
+                class d extends n.LayoutDOMView {
                     get child_models() {
                         return []
                     }
                     get provider() {
-                        return n.default_provider
+                        return o.default_provider
                     }
                     async lazy_initialize() {
                         await super.lazy_initialize(), "not_started" == this.provider.status && await this.provider.fetch()
                     }
                     _after_layout() {
                         super._after_layout(), "loading" == this.provider.status && (this._has_finished = !1)
                     }
                     process_tex(t) {
                         if (null == this.provider.MathJax) return t;
                         const e = this.provider.MathJax.find_tex(t),
                             i = [];
-                        let s = 0;
-                        for (const r of e) i.push(t.slice(s, r.start.n)), i.push(this.provider.MathJax.tex2svg(r.math, {
-                            display: r.display
-                        }).outerHTML), s = r.end.n;
-                        return s < t.length && i.push(t.slice(s)), i.join("")
+                        let r = 0;
+                        for (const s of e) i.push(t.slice(r, s.start.n)), i.push(this.provider.MathJax.tex2svg(s.math, {
+                            display: s.display
+                        }).outerHTML), r = s.end.n;
+                        return r < t.length && i.push(t.slice(r)), i.join("")
                     }
                     contains_tex_string(t) {
                         return null != this.provider.MathJax && this.provider.MathJax.find_tex(t).length > 0
                     }
                 }
                 i.WidgetView = d, d.__name__ = "WidgetView";
-                class o extends a.LayoutDOM {
+                class _ extends n.LayoutDOM {
                     constructor(t) {
                         super(t)
                     }
                 }
-                i.Widget = o, o.__name__ = "Widget"
+                i.Widget = _, a = _, _.__name__ = "Widget", a.override({
+                    margin: 5
+                })
             },
             558: function _(b, o, r, e, t) {
                 e(), r.btn = "bk-btn", r.active = "bk-active", r.btn_default = "bk-btn-default", r.btn_primary = "bk-btn-primary", r.btn_success = "bk-btn-success", r.btn_warning = "bk-btn-warning", r.btn_danger = "bk-btn-danger", r.btn_light = "bk-btn-light", r.btn_group = "bk-btn-group", r.vertical = "bk-vertical", r.horizontal = "bk-horizontal", r.dropdown_toggle = "bk-dropdown-toggle", r.default = ".bk-btn,::file-selector-button{height:100%;display:inline-block;text-align:center;vertical-align:middle;white-space:nowrap;cursor:pointer;padding:var(--padding-vertical) var(--padding-horizontal);font-size:var(--font-size);border:1px solid transparent;border-radius:var(--border-radius);outline:0;outline-offset:-5px;user-select:none;-webkit-user-select:none;}.bk-btn:hover,::file-selector-button:hover,.bk-btn:focus,::file-selector-button:focus{text-decoration:none;}.bk-btn:active,::file-selector-button:active,.bk-active.bk-btn,.bk-active::file-selector-button{background-image:none;box-shadow:inset 0 3px 5px rgba(0, 0, 0, 0.125);}.bk-btn[disabled]{cursor:not-allowed;pointer-events:none;opacity:0.65;box-shadow:none;}::file-selector-button{color:#333;background-color:#fff;border-color:#ccc;}::file-selector-button:hover{background-color:#f5f5f5;border-color:#b8b8b8;}.bk-active::file-selector-button{background-color:#ebebeb;border-color:#adadad;}::file-selector-button[disabled],::file-selector-button[disabled]:hover,::file-selector-button[disabled]:focus,::file-selector-button[disabled]:active,.bk-active::file-selector-button[disabled]{background-color:#e6e6e6;border-color:#ccc;}::file-selector-button:focus,::file-selector-button:active{outline:1px dotted #ccc;}.bk-btn-default{color:#333;background-color:#fff;border-color:#ccc;}.bk-btn-default:hover{background-color:#f5f5f5;border-color:#b8b8b8;}.bk-active.bk-btn-default{background-color:#ebebeb;border-color:#adadad;}.bk-btn-default[disabled],.bk-btn-default[disabled]:hover,.bk-btn-default[disabled]:focus,.bk-btn-default[disabled]:active,.bk-active.bk-btn-default[disabled]{background-color:#e6e6e6;border-color:#ccc;}.bk-btn-default:focus,.bk-btn-default:active{outline:1px dotted #ccc;}.bk-btn-primary{color:#fff;background-color:#428bca;border-color:#357ebd;}.bk-btn-primary:hover{background-color:#3681c1;border-color:#2c699e;}.bk-active.bk-btn-primary{background-color:#3276b1;border-color:#285e8e;}.bk-btn-primary[disabled],.bk-btn-primary[disabled]:hover,.bk-btn-primary[disabled]:focus,.bk-btn-primary[disabled]:active,.bk-active.bk-btn-primary[disabled]{background-color:#506f89;border-color:#357ebd;}.bk-btn-primary:focus,.bk-btn-primary:active{outline:1px dotted #ccc;}.bk-btn-success{color:#fff;background-color:#5cb85c;border-color:#4cae4c;}.bk-btn-success:hover{background-color:#4eb24e;border-color:#409240;}.bk-active.bk-btn-success{background-color:#47a447;border-color:#398439;}.bk-btn-success[disabled],.bk-btn-success[disabled]:hover,.bk-btn-success[disabled]:focus,.bk-btn-success[disabled]:active,.bk-active.bk-btn-success[disabled]{background-color:#667b66;border-color:#4cae4c;}.bk-btn-success:focus,.bk-btn-success:active{outline:1px dotted #ccc;}.bk-btn-warning{color:#fff;background-color:#f0ad4e;border-color:#eea236;}.bk-btn-warning:hover{background-color:#eea43b;border-color:#e89014;}.bk-active.bk-btn-warning{background-color:#ed9c28;border-color:#d58512;}.bk-btn-warning[disabled],.bk-btn-warning[disabled]:hover,.bk-btn-warning[disabled]:focus,.bk-btn-warning[disabled]:active,.bk-active.bk-btn-warning[disabled]{background-color:#c89143;border-color:#eea236;}.bk-btn-warning:focus,.bk-btn-warning:active{outline:1px dotted #ccc;}.bk-btn-danger{color:#fff;background-color:#d9534f;border-color:#d43f3a;}.bk-btn-danger:hover{background-color:#d5433e;border-color:#bd2d29;}.bk-active.bk-btn-danger{background-color:#d2322d;border-color:#ac2925;}.bk-btn-danger[disabled],.bk-btn-danger[disabled]:hover,.bk-btn-danger[disabled]:focus,.bk-btn-danger[disabled]:active,.bk-active.bk-btn-danger[disabled]{background-color:#a55350;border-color:#d43f3a;}.bk-btn-danger:focus,.bk-btn-danger:active{outline:1px dotted #ccc;}.bk-btn-light{color:#333;background-color:#fff;border-color:#ccc;border-color:transparent;}.bk-btn-light:hover{background-color:#f5f5f5;border-color:#b8b8b8;}.bk-active.bk-btn-light{background-color:#ebebeb;border-color:#adadad;}.bk-btn-light[disabled],.bk-btn-light[disabled]:hover,.bk-btn-light[disabled]:focus,.bk-btn-light[disabled]:active,.bk-active.bk-btn-light[disabled]{background-color:#e6e6e6;border-color:#ccc;}.bk-btn-light:focus,.bk-btn-light:active{outline:1px dotted #ccc;}.bk-btn-group{height:100%;display:flex;flex-wrap:nowrap;align-items:center;}.bk-btn-group:not(.bk-vertical),.bk-btn-group.bk-horizontal{flex-direction:row;}.bk-btn-group.bk-vertical{flex-direction:column;}.bk-btn-group > .bk-btn{flex-grow:1;}.bk-btn-group:not(.bk-vertical) > .bk-btn + .bk-btn{margin-left:-1px;}.bk-btn-group.bk-vertical > .bk-btn + .bk-btn{margin-top:-1px;}.bk-btn-group:not(.bk-vertical) > .bk-btn:first-child:not(:last-child){border-bottom-right-radius:0;border-top-right-radius:0;}.bk-btn-group.bk-vertical > .bk-btn:first-child:not(:last-child){border-bottom-left-radius:0;border-bottom-right-radius:0;}.bk-btn-group:not(.bk-vertical) > .bk-btn:not(:first-child):last-child{border-bottom-left-radius:0;border-top-left-radius:0;}.bk-btn-group.bk-vertical > .bk-btn:not(:first-child):last-child{border-top-left-radius:0;border-top-right-radius:0;}.bk-btn-group > .bk-btn:not(:first-child):not(:last-child){border-radius:0;}.bk-btn-group.bk-vertical > .bk-btn{width:100%;}.bk-btn-group .bk-dropdown-toggle{flex:0 0 0;padding:var(--padding-vertical) calc(var(--padding-horizontal)/2);}"
             },
             559: function _(e, t, s, n, i) {
                 var h;
                 n();
@@ -931,17 +929,17 @@
                 }
                 a.DatePicker = o, n = o, o.__name__ = "DatePicker", n.prototype.default_view = r, n.define((({
                     Nullable: e
                 }) => ({
                     value: [e(l.DateLike), null]
                 })))
             },
-            576: function _(e, t, a, s, i) {
+            576: function _(e, t, a, i, s) {
                 var n;
-                s();
+                i();
                 const l = e(577),
                     c = e(8),
                     r = e(20);
                 a.DateLike = (0, r.Or)((0, r.Ref)(Date), r.String, r.Number), a.DateLikeList = (0, r.Array)((0, r.Or)(a.DateLike, (0, r.Tuple)(a.DateLike, a.DateLike), (0, r.Struct)({
                     from: a.DateLike,
                     to: a.DateLike
                 })));
@@ -954,54 +952,54 @@
                     }
                     connect_signals() {
                         super.connect_signals();
                         const {
                             value: e,
                             min_date: t,
                             max_date: a,
-                            disabled_dates: s,
-                            enabled_dates: i,
+                            disabled_dates: i,
+                            enabled_dates: s,
                             date_format: n
                         } = this.model.properties;
                         this.connect(e.change, (() => {
                             const {
                                 value: e
                             } = this.model;
                             null != e ? this.picker.setDate(e) : this.picker.clear()
-                        })), this.connect(t.change, (() => this.picker.set("minDate", this.model.min_date))), this.connect(a.change, (() => this.picker.set("maxDate", this.model.max_date))), this.connect(s.change, (() => {
+                        })), this.connect(t.change, (() => this.picker.set("minDate", this.model.min_date))), this.connect(a.change, (() => this.picker.set("maxDate", this.model.max_date))), this.connect(i.change, (() => {
                             const {
                                 disabled_dates: e
                             } = this.model;
-                            this.picker.set("disable", null != e ? this._convert_date_list(e) : void 0)
-                        })), this.connect(i.change, (() => {
+                            this.picker.set("disable", null != e ? this._convert_date_list(e) : [])
+                        })), this.connect(s.change, (() => {
                             const {
                                 enabled_dates: e
                             } = this.model;
-                            this.picker.set("enable", null != e ? this._convert_date_list(e) : void 0)
+                            null != e ? this.picker.set("enable", this._convert_date_list(e)) : (this.picker.config._enable = void 0, this.picker.redraw(), this.picker.updateValue(!0))
                         })), this.connect(n.change, (() => this.picker.set("altFormat", this.model.date_format)))
                     }
                     get flatpickr_options() {
                         const {
                             value: e,
                             min_date: t,
                             max_date: a,
-                            disabled_dates: s,
-                            enabled_dates: i,
+                            disabled_dates: i,
+                            enabled_dates: s,
                             date_format: n
                         } = this.model, l = super.flatpickr_options;
-                        return l.altInput = !0, l.altFormat = n, l.dateFormat = "Y-m-d", null != e && (l.defaultDate = e), null != t && (l.minDate = t), null != a && (l.maxDate = a), null != s && (l.disable = this._convert_date_list(s)), null != i && (l.enable = this._convert_date_list(i)), l
+                        return l.altInput = !0, l.altFormat = n, l.dateFormat = "Y-m-d", null != e && (l.defaultDate = e), null != t && (l.minDate = t), null != a && (l.maxDate = a), null != i && (l.disable = this._convert_date_list(i)), null != s && (l.enable = this._convert_date_list(s)), l
                     }
                     _convert_date_list(e) {
                         const t = [];
                         for (const a of e)
                             if ((0, c.isArray)(a)) {
-                                const [e, s] = a;
+                                const [e, i] = a;
                                 t.push({
                                     from: e,
-                                    to: s
+                                    to: i
                                 })
                             } else t.push(a);
                         return t
                     }
                 }
                 a.BaseDatePickerView = d, d.__name__ = "BaseDatePickerView";
                 class o extends l.PickerBase {
```

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/bokeh.js` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/bokeh.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -748,15 +748,15 @@
                 __esExport("documents", document_1.documents);
                 var safely_1 = require(69) /* ./safely */ ;
                 __esExport("safely", safely_1.safely);
             },
             /* version.js */
             function _(require, module, exports, __esModule, __esExport) {
                 __esModule();
-                exports.version = "3.2.0-dev.3";
+                exports.version = "3.2.0-dev.4";
             },
             /* embed/index.js */
             function _(require, module, exports, __esModule, __esExport) {
                 __esModule();
                 const document_1 = require(5) /* ../document */ ;
                 const settings_1 = require(28) /* ../core/settings */ ;
                 const logging_1 = require(18) /* ../core/logging */ ;
@@ -1418,15 +1418,23 @@
                 function isPrimitive(obj) {
                     return obj === null || isBoolean(obj) || isNumber(obj) || isString(obj) || isSymbol(obj);
                 }
                 exports.isPrimitive = isPrimitive;
 
                 function isFunction(obj) {
                     const rep = toString.call(obj);
-                    return rep === "[object Function]" || rep === "[object AsyncFunction]";
+                    switch (rep) {
+                        case "[object Function]":
+                        case "[object AsyncFunction]":
+                        case "[object GeneratorFunction]":
+                        case "[object AsyncGeneratorFunction]":
+                            return true;
+                        default:
+                            return false;
+                    }
                 }
                 exports.isFunction = isFunction;
 
                 function isArray(obj) {
                     return Array.isArray(obj);
                 }
                 exports.isArray = isArray;
@@ -1658,14 +1666,17 @@
                     }
                     return result;
                 }
                 exports.zip = zip;
 
                 function unzip(array) {
                     const n = array.length;
+                    if (n == 0) {
+                        return [];
+                    }
                     const k = (0, arrayable_1.min)(array.map((a) => a.length));
                     const results = Array(k);
                     for (let j = 0; j < k; j++)
                         results[j] = new Array(n);
                     for (let i = 0; i < n; i++) {
                         for (let j = 0; j < k; j++)
                             results[j][i] = array[i][j];
@@ -5176,15 +5187,19 @@
                     return color in exports.named_colors;
                 }
                 exports.is_named_color = is_named_color;
             },
             /* core/types.js */
             function _(require, module, exports, __esModule, __esExport) {
                 __esModule();
+                const tslib_1 = require(1) /* tslib */ ;
                 exports.GeneratorFunction = Object.getPrototypeOf(function*() {}).constructor;
+                exports.AsyncGeneratorFunction = Object.getPrototypeOf(function() {
+                    return tslib_1.__asyncGenerator(this, arguments, function*() {});
+                }).constructor;
                 exports.ColorArray = Uint32Array;
                 exports.RGBAArray = Uint8ClampedArray;
 
                 function infer_type(a0, a1) {
                     if (a0 instanceof Float64Array || a0 instanceof Array)
                         return Float64Array;
                     if (a1 instanceof Float64Array || a1 instanceof Array)
@@ -9584,27 +9599,21 @@
                     get y_range() {
                         return {
                             start: this.y0,
                             end: this.y1
                         };
                     }
                     get h_range() {
-                        return {
-                            start: this.x0,
-                            end: this.x1
-                        };
+                        return this.x_range;
                     }
                     get v_range() {
-                        return {
-                            start: this.y0,
-                            end: this.y1
-                        };
+                        return this.y_range;
                     }
                     get ranges() {
-                        return [this.h_range, this.v_range];
+                        return [this.x_range, this.y_range];
                     }
                     get aspect() {
                         return this.width / this.height;
                     }
                     get hcenter() {
                         return (this.left + this.right) / 2;
                     }
@@ -10888,14 +10897,15 @@
                 var _a, _b;
                 __esModule();
                 const tslib_1 = require(1) /* tslib */ ;
                 const view_1 = require(54) /* ../../core/view */ ;
                 const visuals = tslib_1.__importStar(require(75) /* ../../core/visuals */ );
                 const enums_1 = require(19) /* ../../core/enums */ ;
                 const model_1 = require(50) /* ../../model */ ;
+                const assert_1 = require(12) /* ../../core/util/assert */ ;
                 const coordinate_mapping_1 = require(84) /* ../coordinates/coordinate_mapping */ ;
                 class RendererGroup extends model_1.Model {
                     constructor(attrs) {
                         super(attrs);
                     }
                 }
                 exports.RendererGroup = RendererGroup;
@@ -10951,14 +10961,16 @@
                         } else {
                             const {
                                 x_range_name,
                                 y_range_name
                             } = this.model;
                             const x_scale = frame.x_scales.get(x_range_name);
                             const y_scale = frame.y_scales.get(y_range_name);
+                            (0, assert_1.assert)(x_scale != null, `missing '${x_range_name}' range`);
+                            (0, assert_1.assert)(y_scale != null, `missing '${y_range_name}' range`);
                             return new coordinate_mapping_1.CoordinateTransform(x_scale, y_scale);
                         }
                     }
                     get plot_view() {
                         return this.parent;
                     }
                     get plot_model() {
@@ -11903,15 +11915,15 @@
                         this._static_doit = false;
                         this._update_iteration = 0;
                     }
                     _compute_static_doit() {
                         const color = this.hatch_color.value;
                         const alpha = this.hatch_alpha.value;
                         const pattern = this.hatch_pattern.value;
-                        return !(color == null || alpha == 0 || pattern == " " || pattern == "blank" || pattern == null);
+                        return !(color == 0 || alpha == 0 || pattern == " " || pattern == "blank" || pattern == null);
                     }
                     update() {
                         this._update_iteration++;
                         const n = this.hatch_color.length;
                         this._hatch_image = new p.UniformScalar(null, n);
                         this._static_doit = this._compute_static_doit();
                         if (!this._static_doit)
@@ -11969,29 +11981,30 @@
                         if (image == null)
                             return null;
                         else
                             return ctx.createPattern(image, this.repetition());
                     }
                     repetition() {
                         const pattern = this.hatch_pattern.value;
-                        const texture = this.hatch_extra.value[pattern];
-                        if (texture == null)
-                            return "repeat";
-                        else {
-                            switch (texture.repetition) {
-                                case "repeat":
-                                    return "repeat";
-                                case "repeat_x":
-                                    return "repeat-x";
-                                case "repeat_y":
-                                    return "repeat-y";
-                                case "no_repeat":
-                                    return "no-repeat";
+                        if (pattern != null) {
+                            const texture = this.hatch_extra.value[pattern];
+                            if (texture != null) {
+                                switch (texture.repetition) {
+                                    case "repeat":
+                                        return "repeat";
+                                    case "repeat_x":
+                                        return "repeat-x";
+                                    case "repeat_y":
+                                        return "repeat-y";
+                                    case "no_repeat":
+                                        return "no-repeat";
+                                }
                             }
                         }
+                        return "repeat";
                     }
                 }
                 exports.HatchScalar = HatchScalar;
                 HatchScalar.__name__ = "HatchScalar";
                 class HatchVector extends visual_1.VisualUniforms {
                     constructor() {
                         super(...arguments);
@@ -12111,29 +12124,30 @@
                         if (image == null)
                             return null;
                         else
                             return ctx.createPattern(image, this.repetition(i));
                     }
                     repetition(i) {
                         const pattern = this.hatch_pattern.get(i);
-                        const texture = this.hatch_extra.value[pattern];
-                        if (texture == null)
-                            return "repeat";
-                        else {
-                            switch (texture.repetition) {
-                                case "repeat":
-                                    return "repeat";
-                                case "repeat_x":
-                                    return "repeat-x";
-                                case "repeat_y":
-                                    return "repeat-y";
-                                case "no_repeat":
-                                    return "no-repeat";
+                        if (pattern != null) {
+                            const texture = this.hatch_extra.value[pattern];
+                            if (texture != null) {
+                                switch (texture.repetition) {
+                                    case "repeat":
+                                        return "repeat";
+                                    case "repeat_x":
+                                        return "repeat-x";
+                                    case "repeat_y":
+                                        return "repeat-y";
+                                    case "no_repeat":
+                                        return "no-repeat";
+                                }
                             }
                         }
+                        return "repeat";
                     }
                 }
                 exports.HatchVector = HatchVector;
                 HatchVector.__name__ = "HatchVector";
                 Hatch.prototype.type = "hatch";
                 Hatch.prototype.attrs = Object.keys(mixins.Hatch);
                 HatchScalar.prototype.type = "hatch";
@@ -20674,19 +20688,22 @@
                 const types_3 = require(8) /* ../../core/util/types */ ;
                 const utils_1 = require(148) /* ../text/utils */ ;
                 const {
                     abs
                 } = Math;
                 class AxisView extends guide_renderer_1.GuideRendererView {
                     constructor() {
-                            super(...arguments);
-                            /*private*/
-                            this._axis_label_view = null;
-                            /*private*/
-                            this._major_label_views = new Map();
+                        super(...arguments);
+                        /*private*/
+                        this._axis_label_view = null;
+                        /*private*/
+                        this._major_label_views = new Map();
+                    }
+                    get bbox() {
+                            return this.layout.bbox;
                         }
                         * children() {
                             yield* super.children();
                             if (this._axis_label_view != null)
                                 yield this._axis_label_view;
                             yield* this._major_label_views.values();
                         }
@@ -25331,24 +25348,35 @@
                                         return index;
                                 }
                             }
                         }
                         return 0;
                     }
                     draw_legend(ctx, x0, x1, y0, y1, field, label, index) {
-                        if (this.glyph.data_size == 0)
+                        if (this.glyph.data_size == 0) {
                             return;
-                        if (index == null)
-                            index = this.get_reference_point(field, label);
-                        this.glyph.draw_legend_for_index(ctx, {
-                            x0,
-                            x1,
-                            y0,
-                            y1
-                        }, index);
+                        }
+                        const subset_index = (() => {
+                            if (index == null)
+                                return this.get_reference_point(field, label);
+                            else {
+                                const {
+                                    indices_map
+                                } = this.model.view;
+                                return index in indices_map ? indices_map[index] : null;
+                            }
+                        })();
+                        if (subset_index != null) {
+                            this.glyph.draw_legend_for_index(ctx, {
+                                x0,
+                                x1,
+                                y0,
+                                y1
+                            }, subset_index);
+                        }
                     }
                     hit_test(geometry) {
                         if (!this.model.visible)
                             return null;
                         const hit_test_result = this.glyph.hit_test(geometry);
                         // glyphs that don't have hit-testing implemented will return null
                         if (hit_test_result == null)
@@ -31520,18 +31548,15 @@
                         if (panel != null)
                             this.layout = new side_panel_1.SideLayout(panel, () => this.get_size());
                         else
                             this.layout = undefined;
                     }
                     connect_signals() {
                         super.connect_signals();
-                        const rerender = () => {
-                            this.update_geometry();
-                            this.request_render();
-                        };
+                        const rerender = () => this.request_render();
                         this.connect(this.model.change, rerender);
                         this.connect(this.model.item_change, rerender);
                     }
                     get padding() {
                         return this.model.border_line_color != null ? this.model.padding : 0;
                     }
                     update_geometry() {
@@ -31793,14 +31818,18 @@
                                 fn(renderer);
                             }
                             return true;
                         }
                         return false;
                     }
                     _render() {
+                        // It would be better to update geometry (the internal layout) only when
+                        // necessary, but conditions for that are not clear, so for now update
+                        // at every render.
+                        this.update_geometry();
                         this.compute_geometry();
                         if (this.model.items.length == 0)
                             return;
                         if (!(0, array_1.some)(this.model.items, (item) => item.visible))
                             return;
                         const {
                             ctx
@@ -31944,22 +31973,14 @@
                     constructor(attrs) {
                         super(attrs);
                     }
                     initialize() {
                         super.initialize();
                         this.item_change = new signaling_1.Signal0(this, "item_change");
                     }
-                    get_legend_names() {
-                        const legend_names = [];
-                        for (const item of this.items) {
-                            const labels = item.get_labels_list_from_label_prop();
-                            legend_names.push(...labels);
-                        }
-                        return legend_names;
-                    }
                 }
                 exports.Legend = Legend;
                 _a = Legend;
                 Legend.__name__ = "Legend";
                 (() => {
                     _a.prototype.default_view = LegendView;
                     _a.mixins([
@@ -32083,16 +32104,24 @@
                     get_field_from_label_prop() {
                         const {
                             label
                         } = this;
                         return (0, vectorization_1.isField)(label) ? label.field : null;
                     }
                     get_labels_list_from_label_prop() {
-                        if (!this.visible)
+                        if (!this.visible) {
                             return [];
+                        }
+                        const {
+                            index
+                        } = this;
+                        if (index != null && this.renderers.every((r) => !(index in r.view.indices_map))) {
+                            // this index points to nowhere, so skip this item altogether from its legend
+                            return [];
+                        }
                         if ((0, vectorization_1.isValue)(this.label)) {
                             const {
                                 value
                             } = this.label;
                             return value != null ? [value] : [];
                         }
                         const field = this.get_field_from_label_prop();
@@ -37272,44 +37301,112 @@
             },
             /* models/callbacks/customjs.js */
             function _(require, module, exports, __esModule, __esExport) {
                 var _a;
                 __esModule();
                 const callback_1 = require(290) /* ./callback */ ;
                 const object_1 = require(9) /* ../../core/util/object */ ;
+                const array_1 = require(10) /* ../../core/util/array */ ;
                 const string_1 = require(38) /* ../../core/util/string */ ;
+                const logging_1 = require(18) /* ../../core/logging */ ;
+                const types_1 = require(8) /* ../../core/util/types */ ;
                 class CustomJS extends callback_1.Callback {
                     constructor(attrs) {
                         super(attrs);
+                        this._state = null;
                     }
-                    get names() {
-                        return (0, object_1.keys)(this.args);
+                    connect_signals() {
+                        super.connect_signals();
+                        const {
+                            args,
+                            code,
+                            module
+                        } = this.properties;
+                        this.on_change([args, code, module], () => this._state = null);
                     }
-                    get values() {
-                        return (0, object_1.values)(this.args);
+                    async _compile_module() {
+                        const url = URL.createObjectURL(new Blob([this.code], {
+                            type: "text/javascript"
+                        }));
+                        try {
+                            // XXX: eval() to work around transpilation to require()
+                            // https://github.com/microsoft/TypeScript/issues/43329
+                            const module = await eval(`import("${url}")`);
+                            if ((0, types_1.isFunction)(module.default)) {
+                                return module.default;
+                            } else {
+                                logging_1.logger.warn("custom ES module didn't export a default function");
+                                return () => undefined;
+                            }
+                        } finally {
+                            URL.revokeObjectURL(url);
+                        }
                     }
-                    get func() {
+                    async _compile_function() {
+                        const [names = [], values = []] = (0, array_1.unzip)((0, object_1.entries)(this.args));
                         const code = (0, string_1.use_strict)(this.code);
-                        return new Function(...this.names, "cb_obj", "cb_data", code);
+                        const func = new Function(...names, "cb_obj", "cb_data", code);
+                        return func.bind(undefined, ...values);
                     }
-                    execute(cb_obj, cb_data = {}) {
-                        return this.func.apply(cb_obj, this.values.concat(cb_obj, cb_data));
+                    _is_es_module(code) {
+                        return code.split("\n").some((line) => line.trimStart().startsWith("export default"));
+                    }
+                    async _compile() {
+                        const module = (() => {
+                            if (this.module == "auto") {
+                                return this._is_es_module(this.code);
+                            } else {
+                                return this.module;
+                            }
+                        })();
+                        if (module) {
+                            return {
+                                func: await this._compile_module(),
+                                module
+                            };
+                        } else {
+                            return {
+                                func: await this._compile_function(),
+                                module
+                            };
+                        }
+                    }
+                    async state() {
+                        if (this._state == null) {
+                            this._state = await this._compile();
+                        }
+                        return this._state;
+                    }
+                    async execute(obj, data = {}) {
+                        const {
+                            func,
+                            module
+                        } = await this.state();
+                        if (module) {
+                            return func(this.args, obj, data);
+                        } else {
+                            return func.call(obj, obj, data);
+                        }
                     }
                 }
                 exports.CustomJS = CustomJS;
                 _a = CustomJS;
                 CustomJS.__name__ = "CustomJS";
                 (() => {
                     _a.define(({
                         Unknown,
                         String,
-                        Dict
+                        Dict,
+                        Auto,
+                        Or,
+                        Boolean
                     }) => ({
                         args: [Dict(Unknown), {}],
-                        code: [String, ""],
+                        code: [String],
+                        module: [Or(Auto, Boolean), "auto"],
                     }));
                 })();
             },
             /* models/callbacks/callback.js */
             function _(require, module, exports, __esModule, __esExport) {
                 __esModule();
                 const model_1 = require(50) /* ../../model */ ;
@@ -43742,15 +43839,15 @@
                 class ImageView extends image_base_1.ImageBaseView {
                     connect_signals() {
                         super.connect_signals();
                         this.connect(this.model.color_mapper.change, () => this._update_image());
                     }
                     _update_image() {
                         // Only reset image_data if already initialized
-                        if (this.image_data != null) {
+                        if (this._image_data != null) {
                             this._set_data(null);
                             this.renderer.request_render();
                         }
                     }
                     _flat_img_to_buf8(img) {
                         const cmap = this.model.color_mapper.rgba_mapper;
                         return cmap.v_compute(img);
@@ -43790,14 +43887,22 @@
                 const p = tslib_1.__importStar(require(17) /* ../../core/properties */ );
                 const mixins = tslib_1.__importStar(require(78) /* ../../core/property_mixins */ );
                 const selection_1 = require(101) /* ../selections/selection */ ;
                 const assert_1 = require(12) /* ../../core/util/assert */ ;
                 const kinds_1 = require(236) /* ../common/kinds */ ;
                 const resolve_1 = require(238) /* ../common/resolve */ ;
                 class ImageBaseView extends xy_glyph_1.XYGlyphView {
+                    constructor() {
+                        super(...arguments);
+                        this._image_data = null;
+                    }
+                    get image_data() {
+                        (0, assert_1.assert)(this._image_data != null, "data not set");
+                        return this._image_data;
+                    }
                     connect_signals() {
                         super.connect_signals();
                         this.connect(this.model.properties.global_alpha.change, () => this.renderer.request_render());
                     }
                     get image_dimension() {
                         return 2;
                     }
@@ -43886,25 +43991,31 @@
                                 ctx.drawImage(image_data_i, -xy_offset.x * sw_i, -xy_offset.y * sh_i, sw_i, sh_i);
                                 ctx.restore();
                             }
                         }
                         ctx.restore();
                     }
                     _set_data(indices) {
-                        this._set_width_height_data();
+                        const n = this.data_size;
+                        if (this._image_data == null || this._image_data.length != n) {
+                            this._image_data = new Array(n).fill(null);
+                            this._width = new Uint32Array(n);
+                            this._height = new Uint32Array(n);
+                        }
                         const {
                             image_dimension
                         } = this;
-                        for (let i = 0, end = this.image.length; i < end; i++) {
-                            if (indices != null && indices.indexOf(i) < 0)
+                        for (let i = 0; i < n; i++) {
+                            if (indices != null && !indices.includes(i))
                                 continue;
                             const img = this.image.get(i);
                             (0, assert_1.assert)(img.dimension == image_dimension, `expected a ${image_dimension}D array, not ${img.dimension}D`);
-                            this._height[i] = img.shape[0];
-                            this._width[i] = img.shape[1];
+                            const [width, height] = img.shape;
+                            this._height[i] = width;
+                            this._width[i] = height;
                             const buf8 = this._flat_img_to_buf8(img);
                             this._set_image_data_from_buffer(i, buf8);
                         }
                     }
                     _index_data(index) {
                         const {
                             data_size
@@ -43924,27 +44035,19 @@
                         } = this;
                         const [x0, x1] = [x_i - xy_anchor.x * dw_i, x_i + (1 - xy_anchor.x) * dw_i];
                         const [y0, y1] = [y_i + xy_anchor.y * dh_i, y_i - (1 - xy_anchor.y) * dh_i];
                         const [l, r] = x0 <= x1 ? [x0, x1] : [x1, x0];
                         const [b, t] = y0 <= y1 ? [y0, y1] : [y1, y0];
                         return [l, r, t, b];
                     }
-                    _set_width_height_data() {
-                        if (this.image_data == null || this.image_data.length != this.image.length)
-                            this.image_data = new Array(this.image.length);
-                        if (this._width == null || this._width.length != this.image.length)
-                            this._width = new Uint32Array(this.image.length);
-                        if (this._height == null || this._height.length != this.image.length)
-                            this._height = new Uint32Array(this.image.length);
-                    }
                     _get_or_create_canvas(i) {
-                        const _image_data = this.image_data[i];
-                        if (_image_data != null && _image_data.width == this._width[i] &&
-                            _image_data.height == this._height[i])
-                            return _image_data;
+                        const image_data_i = this.image_data[i];
+                        if (image_data_i != null && image_data_i.width == this._width[i] &&
+                            image_data_i.height == this._height[i])
+                            return image_data_i;
                         else {
                             const canvas = document.createElement("canvas");
                             canvas.width = this._width[i];
                             canvas.height = this._height[i];
                             return canvas;
                         }
                     }
@@ -44078,15 +44181,15 @@
                         this.connect(this.model.color_mapper.change, () => this._update_image());
                     }
                     get image_dimension() {
                         return 3;
                     }
                     _update_image() {
                         // Only reset image_data if already initialized
-                        if (this.image_data != null) {
+                        if (this._image_data != null) {
                             this._set_data(null);
                             this.renderer.request_render();
                         }
                     }
                     _flat_img_to_buf8(img) {
                         const cmap = this.model.color_mapper.rgba_mapper;
                         return cmap.v_compute(img);
@@ -51419,15 +51522,17 @@
                     }
                     update_range(range_info, options) {
                         this.pause();
                         this._range_manager.update(range_info, options);
                         this.unpause();
                     }
                     reset_range() {
-                        this.update_range(null);
+                        this.pause();
+                        this._range_manager.reset();
+                        this.unpause();
                         this.trigger_ranges_update_event();
                     }
                     trigger_ranges_update_event() {
                         const {
                             x_range,
                             y_range
                         } = this.model;
@@ -51965,38 +52070,38 @@
                     }
                     update(range_info, options = {}) {
                         var _a;
                         const {
                             x_ranges,
                             y_ranges
                         } = this.frame;
-                        if (range_info == null) {
-                            for (const [, range] of x_ranges) {
-                                range.reset();
-                            }
-                            for (const [, range] of y_ranges) {
-                                range.reset();
-                            }
-                            this.update_dataranges();
-                        } else {
-                            const range_info_iter = [];
-                            for (const [name, range] of x_ranges) {
-                                range_info_iter.push([range, range_info.xrs.get(name)]);
-                            }
-                            for (const [name, range] of y_ranges) {
-                                range_info_iter.push([range, range_info.yrs.get(name)]);
-                            }
-                            if ((_a = options.scrolling) !== null && _a !== void 0 ? _a : false) {
-                                this._update_ranges_together(range_info_iter); // apply interval bounds while keeping aspect
-                            }
-                            this._update_ranges_individually(range_info_iter, options);
+                        const range_info_iter = [];
+                        for (const [name, interval] of range_info.xrs) {
+                            range_info_iter.push([x_ranges.get(name), interval]);
+                        }
+                        for (const [name, interval] of range_info.yrs) {
+                            range_info_iter.push([y_ranges.get(name), interval]);
                         }
+                        if ((_a = options.scrolling) !== null && _a !== void 0 ? _a : false) {
+                            this._update_ranges_together(range_info_iter); // apply interval bounds while keeping aspect
+                        }
+                        this._update_ranges_individually(range_info_iter, options);
                     }
                     reset() {
-                        this.update(null);
+                        const {
+                            x_ranges,
+                            y_ranges
+                        } = this.frame;
+                        for (const range of x_ranges.values()) {
+                            range.reset();
+                        }
+                        for (const range of y_ranges.values()) {
+                            range.reset();
+                        }
+                        this.update_dataranges();
                     }
                     _update_dataranges(frame) {
                         // Update any DataRange1ds here
                         const bounds = new Map();
                         const log_bounds = new Map();
                         let calculate_log_bounds = false;
                         for (const [, xr] of frame.x_ranges) {
@@ -52394,15 +52499,15 @@
                             this.map.setCenter({
                                 lat: this.initial_lat,
                                 lng: this.initial_lng
                             });
                             this.map.setOptions({
                                 zoom: this.initial_zoom
                             });
-                            super.update_range(null, options);
+                            super.reset_range();
                             // PAN ----------------------------
                         } else if (range_info.sdx != null || range_info.sdy != null) {
                             this.map.panBy((_a = range_info.sdx) !== null && _a !== void 0 ? _a : 0, (_b = range_info.sdy) !== null && _b !== void 0 ? _b : 0);
                             super.update_range(range_info, options);
                             // ZOOM ---------------------------
                         } else if (range_info.factor != null) {
                             // The zoom count decreases the sensitivity of the zoom. (We could make this user configurable)
@@ -53198,17 +53303,17 @@
                         super(attrs);
                         this.initialized = false;
                     }
                     setup() {
                         if (!this.initialized) {
                             this.initialized = true;
                             const source = new EventSource(this.data_url);
-                            source.onmessage = (event) => {
+                            source.onmessage = async (event) => {
                                 var _a;
-                                this.load_data(JSON.parse(event.data), this.mode, (_a = this.max_size) !== null && _a !== void 0 ? _a : undefined);
+                                await this.load_data(JSON.parse(event.data), this.mode, (_a = this.max_size) !== null && _a !== void 0 ? _a : undefined);
                             };
                         }
                     }
                 }
                 exports.ServerSentDataSource = ServerSentDataSource;
                 ServerSentDataSource.__name__ = "ServerSentDataSource";
             },
@@ -53229,21 +53334,21 @@
                         var _b;
                         return (_b = super.get_length()) !== null && _b !== void 0 ? _b : 0;
                     }
                     initialize() {
                         super.initialize();
                         this.setup();
                     }
-                    load_data(raw_data, mode, max_size) {
+                    async load_data(raw_data, mode, max_size) {
                         const {
                             adapter
                         } = this;
                         let data;
                         if (adapter != null)
-                            data = adapter.execute(this, {
+                            data = await adapter.execute(this, {
                                 response: raw_data
                             });
                         else
                             data = raw_data;
                         switch (mode) {
                             case "replace": {
                                 this.data = data;
@@ -53324,18 +53429,18 @@
                         xhr.setRequestHeader("Content-Type", this.content_type);
                         const http_headers = this.http_headers;
                         for (const [name, value] of(0, object_1.entries)(http_headers)) {
                             xhr.setRequestHeader(name, value);
                         }
                         return xhr;
                     }
-                    do_load(xhr, mode, max_size) {
-                        if (xhr.status === 200) {
+                    async do_load(xhr, mode, max_size) {
+                        if (xhr.status == 200) {
                             const raw_data = JSON.parse(xhr.responseText);
-                            this.load_data(raw_data, mode, max_size);
+                            await this.load_data(raw_data, mode, max_size);
                         }
                     }
                     do_error(xhr) {
                         logging_1.logger.error(`Failed to fetch JSON from ${this.data_url} with code ${xhr.status}`);
                     }
                 }
                 exports.AjaxDataSource = AjaxDataSource;
@@ -56357,27 +56462,28 @@
             },
             /* models/tools/actions/zoom_in_tool.js */
             function _(require, module, exports, __esModule, __esExport) {
                 var _a;
                 __esModule();
                 const zoom_base_tool_1 = require(470) /* ./zoom_base_tool */ ;
                 const icons_css_1 = require(272) /* ../../../styles/icons.css */ ;
-                class ZoomInToolView extends zoom_base_tool_1.ZoomBaseToolView {}
+                class ZoomInToolView extends zoom_base_tool_1.ZoomBaseToolView {
+                    get factor() {
+                        return this.model.factor;
+                    }
+                }
                 exports.ZoomInToolView = ZoomInToolView;
                 ZoomInToolView.__name__ = "ZoomInToolView";
                 class ZoomInTool extends zoom_base_tool_1.ZoomBaseTool {
                     constructor(attrs) {
                         super(attrs);
                         this.maintain_focus = true;
                         this.tool_name = "Zoom In";
                         this.tool_icon = icons_css_1.tool_icon_zoom_in;
                     }
-                    get_factor() {
-                        return this.factor;
-                    }
                 }
                 exports.ZoomInTool = ZoomInTool;
                 _a = ZoomInTool;
                 ZoomInTool.__name__ = "ZoomInTool";
                 (() => {
                     _a.prototype.default_view = ZoomInToolView;
                     _a.register_alias("zoom_in", () => new ZoomInTool({
@@ -56392,26 +56498,55 @@
                 })();
             },
             /* models/tools/actions/zoom_base_tool.js */
             function _(require, module, exports, __esModule, __esExport) {
                 var _a;
                 __esModule();
                 const plot_action_tool_1 = require(465) /* ./plot_action_tool */ ;
+                const data_renderer_1 = require(200) /* ../../renderers/data_renderer */ ;
                 const enums_1 = require(19) /* ../../../core/enums */ ;
                 const zoom_1 = require(471) /* ../../../core/util/zoom */ ;
                 class ZoomBaseToolView extends plot_action_tool_1.PlotActionToolView {
                     doit() {
                         var _b;
-                        const frame = this.plot_view.frame;
-                        const dims = this.model.dimensions;
                         // restrict to axis configured in tool's dimensions property
-                        const h_axis = dims == "width" || dims == "both";
-                        const v_axis = dims == "height" || dims == "both";
-                        const factor = this.model.get_factor();
-                        const zoom_info = (0, zoom_1.scale_range)(frame, factor, h_axis, v_axis);
+                        const {
+                            dimensions
+                        } = this.model;
+                        const x_axis = dimensions == "width" || dimensions == "both";
+                        const y_axis = dimensions == "height" || dimensions == "both";
+                        const {
+                            frame
+                        } = this.plot_view;
+                        const {
+                            x_range,
+                            y_range
+                        } = frame.bbox;
+                        const x_scales = new Map(frame.x_scales);
+                        const y_scales = new Map(frame.y_scales);
+                        const {
+                            renderers
+                        } = this.model;
+                        if (renderers != "auto") {
+                            const x_range_names = new Set();
+                            const y_range_names = new Set();
+                            for (const renderer of renderers) {
+                                x_range_names.add(renderer.x_range_name);
+                                y_range_names.add(renderer.y_range_name);
+                            }
+                            for (const name of x_scales.keys()) {
+                                if (!x_range_names.has(name))
+                                    x_scales.delete(name);
+                            }
+                            for (const name of y_scales.keys()) {
+                                if (!y_range_names.has(name))
+                                    y_scales.delete(name);
+                            }
+                        }
+                        const zoom_info = (0, zoom_1.scale_range)(x_scales, y_scales, x_range, y_range, this.factor, x_axis, y_axis);
                         this.plot_view.state.push("zoom_out", {
                             range: zoom_info
                         });
                         this.plot_view.update_range(zoom_info, {
                             scrolling: true,
                             maintain_focus: this.model.maintain_focus
                         });
@@ -56430,28 +56565,33 @@
                     }
                 }
                 exports.ZoomBaseTool = ZoomBaseTool;
                 _a = ZoomBaseTool;
                 ZoomBaseTool.__name__ = "ZoomBaseTool";
                 (() => {
                     _a.define(({
-                        Percent
+                        Percent,
+                        Or,
+                        Array,
+                        Ref,
+                        Auto
                     }) => ({
                         factor: [Percent, 0.1],
                         dimensions: [enums_1.Dimensions, "both"],
+                        renderers: [Or(Array(Ref(data_renderer_1.DataRenderer)), Auto), "auto"],
                     }));
                 })();
             },
             /* core/util/zoom.js */
             function _(require, module, exports, __esModule, __esExport) {
                 __esModule();
-                // Module for zoom-related functions
+
                 function scale_highlow(range, factor, center) {
                     const [low, high] = [range.start, range.end];
-                    const x = center != null ? center : (high + low) / 2.0;
+                    const x = center !== null && center !== void 0 ? center : (high + low) / 2.0;
                     const x0 = low - (low - x) * factor;
                     const x1 = high - (high - x) * factor;
                     return [x0, x1];
                 }
                 exports.scale_highlow = scale_highlow;
 
                 function get_info(scales, [sxy0, sxy1]) {
@@ -56463,38 +56603,25 @@
                             end
                         });
                     }
                     return info;
                 }
                 exports.get_info = get_info;
 
-                function scale_range(frame, factor, h_axis = true, v_axis = true, center) {
+                function scale_range(x_scales, y_scales, x_range, y_range, factor, x_axis = true, y_axis = true, center) {
                     /*
                      * Utility function for zoom tools to calculate/create the zoom_info object
-                     * of the form required by ``PlotView.update_range``
-                     *
-                     * Parameters:
-                     *   frame : CartesianFrame
-                     *   factor : Number
-                     *   h_axis : Boolean, optional
-                     *     whether to zoom the horizontal axis (default = true)
-                     *   v_axis : Boolean, optional
-                     *     whether to zoom the horizontal axis (default = true)
-                     *   center : object, optional
-                     *     of form {'x': Number, 'y', Number}
-                     *
-                     * Returns:
-                     *   ScaleRange
+                     * of the form required by `PlotView.update_range`.
                      */
-                    const hfactor = h_axis ? factor : 0;
-                    const [sx0, sx1] = scale_highlow(frame.bbox.h_range, hfactor, center != null ? center.x : undefined);
-                    const xrs = get_info(frame.x_scales, [sx0, sx1]);
-                    const vfactor = v_axis ? factor : 0;
-                    const [sy0, sy1] = scale_highlow(frame.bbox.v_range, vfactor, center != null ? center.y : undefined);
-                    const yrs = get_info(frame.y_scales, [sy0, sy1]);
+                    const x_factor = x_axis ? factor : 0;
+                    const [sx0, sx1] = scale_highlow(x_range, x_factor, center === null || center === void 0 ? void 0 : center.x);
+                    const xrs = get_info(x_scales, [sx0, sx1]);
+                    const y_factor = y_axis ? factor : 0;
+                    const [sy0, sy1] = scale_highlow(y_range, y_factor, center === null || center === void 0 ? void 0 : center.y);
+                    const yrs = get_info(y_scales, [sy0, sy1]);
                     // OK this sucks we can't set factor independently in each direction. It is used
                     // for GMap plots, and GMap plots always preserve aspect, so effective the value
                     // of 'dimensions' is ignored.
                     return {
                         xrs,
                         yrs,
                         factor
@@ -56504,26 +56631,30 @@
             },
             /* models/tools/actions/zoom_out_tool.js */
             function _(require, module, exports, __esModule, __esExport) {
                 var _a;
                 __esModule();
                 const zoom_base_tool_1 = require(470) /* ./zoom_base_tool */ ;
                 const icons_css_1 = require(272) /* ../../../styles/icons.css */ ;
-                class ZoomOutToolView extends zoom_base_tool_1.ZoomBaseToolView {}
+                class ZoomOutToolView extends zoom_base_tool_1.ZoomBaseToolView {
+                    get factor() {
+                        const {
+                            factor
+                        } = this.model;
+                        return -factor / (1 - factor);
+                    }
+                }
                 exports.ZoomOutToolView = ZoomOutToolView;
                 ZoomOutToolView.__name__ = "ZoomOutToolView";
                 class ZoomOutTool extends zoom_base_tool_1.ZoomBaseTool {
                     constructor(attrs) {
                         super(attrs);
                         this.tool_name = "Zoom Out";
                         this.tool_icon = icons_css_1.tool_icon_zoom_out;
                     }
-                    get_factor() {
-                        return -this.factor / (1 - this.factor);
-                    }
                 }
                 exports.ZoomOutTool = ZoomOutTool;
                 _a = ZoomOutTool;
                 ZoomOutTool.__name__ = "ZoomOutTool";
                 (() => {
                     _a.prototype.default_view = ZoomOutToolView;
                     _a.define(({
@@ -59735,14 +59866,16 @@
                 var _a;
                 __esModule();
                 const gesture_tool_1 = require(274) /* ./gesture_tool */ ;
                 const zoom_1 = require(471) /* ../../../core/util/zoom */ ;
                 const enums_1 = require(19) /* ../../../core/enums */ ;
                 const platform_1 = require(26) /* ../../../core/util/platform */ ;
                 const icons_css_1 = require(272) /* ../../../styles/icons.css */ ;
+                const kinds_1 = require(20) /* ../../../core/kinds */ ;
+                const ZoomTogether = (0, kinds_1.Enum)("none", "cross", "all");
                 class WheelZoomToolView extends gesture_tool_1.GestureToolView {
                     _pinch(ev) {
                         // TODO (bev) this can probably be done much better
                         const {
                             sx,
                             sy,
                             scale,
@@ -59760,35 +59893,125 @@
                             delta,
                             modifiers
                         });
                     }
                     _scroll(ev) {
                         var _b;
                         const {
-                            frame
-                        } = this.plot_view;
-                        const hr = frame.bbox.h_range;
-                        const vr = frame.bbox.v_range;
-                        const {
                             sx,
                             sy
                         } = ev;
-                        const dims = this.model.dimensions;
-                        // restrict to axis configured in tool's dimensions property and if
-                        // zoom origin is inside of frame range/domain
-                        const h_axis = (dims == "width" || dims == "both") && hr.start < sx && sx < hr.end;
-                        const v_axis = (dims == "height" || dims == "both") && vr.start < sy && sy < vr.end;
-                        if ((!h_axis || !v_axis) && !this.model.zoom_on_axis) {
+                        const axis_view = this.plot_view.axis_views.find((view) => view.layout.bbox.contains(sx, sy));
+                        if (axis_view != null && !this.model.zoom_on_axis) {
                             return;
                         }
+                        const {
+                            frame
+                        } = this.plot_view;
+                        if (axis_view == null && !frame.bbox.contains(sx, sy)) {
+                            return;
+                        }
+                        // restrict to axis configured in tool's dimensions property and if
+                        // zoom origin is inside of frame range/domain
+                        const dims = this.model.dimensions;
+                        const x_axis = dims == "width" || dims == "both";
+                        const y_axis = dims == "height" || dims == "both";
+                        const {
+                            x_range,
+                            y_range
+                        } = frame.bbox;
+                        const {
+                            x_scales,
+                            y_scales,
+                            center
+                        } = (() => {
+                            if (axis_view != null) {
+                                const center = axis_view.dimension == 0 ? {
+                                    x: sx,
+                                    y: null
+                                } : {
+                                    x: null,
+                                    y: sy
+                                };
+                                const {
+                                    zoom_together
+                                } = this.model;
+                                if (zoom_together == "all") {
+                                    const {
+                                        x_scales,
+                                        y_scales
+                                    } = frame;
+                                    if (axis_view.dimension == 0)
+                                        return {
+                                            x_scales,
+                                            y_scales: new Map(),
+                                            center
+                                        };
+                                    else
+                                        return {
+                                            x_scales: new Map(),
+                                            y_scales,
+                                            center
+                                        };
+                                } else {
+                                    const {
+                                        x_range_name,
+                                        y_range_name
+                                    } = axis_view.model;
+                                    const {
+                                        x_scale,
+                                        y_scale
+                                    } = axis_view.coordinates;
+                                    const x_scales = new Map([
+                                        [x_range_name, x_scale]
+                                    ]);
+                                    const y_scales = new Map([
+                                        [y_range_name, y_scale]
+                                    ]);
+                                    switch (zoom_together) {
+                                        case "cross": {
+                                            return {
+                                                x_scales,
+                                                y_scales,
+                                                center
+                                            };
+                                        }
+                                        case "none": {
+                                            if (axis_view.dimension == 0)
+                                                return {
+                                                    x_scales,
+                                                    y_scales: new Map(),
+                                                    center
+                                                };
+                                            else
+                                                return {
+                                                    x_scales: new Map(),
+                                                    y_scales,
+                                                    center
+                                                };
+                                        }
+                                    }
+                                }
+                            } else {
+                                const {
+                                    x_scales,
+                                    y_scales
+                                } = frame;
+                                return {
+                                    x_scales,
+                                    y_scales,
+                                    center: {
+                                        x: sx,
+                                        y: sy
+                                    }
+                                };
+                            }
+                        })();
                         const factor = this.model.speed * ev.delta;
-                        const zoom_info = (0, zoom_1.scale_range)(frame, factor, h_axis, v_axis, {
-                            x: sx,
-                            y: sy
-                        });
+                        const zoom_info = (0, zoom_1.scale_range)(x_scales, y_scales, x_range, y_range, factor, x_axis, y_axis, center);
                         this.plot_view.state.push("wheel_zoom", {
                             range: zoom_info
                         });
                         const {
                             maintain_focus
                         } = this.model;
                         this.plot_view.update_range(zoom_info, {
@@ -59820,14 +60043,15 @@
                     _a.define(({
                         Boolean,
                         Number
                     }) => ({
                         dimensions: [enums_1.Dimensions, "both"],
                         maintain_focus: [Boolean, true],
                         zoom_on_axis: [Boolean, true],
+                        zoom_together: [ZoomTogether, "all"],
                         speed: [Number, 1 / 600],
                     }));
                     _a.register_alias("wheel_zoom", () => new WheelZoomTool({
                         dimensions: "both"
                     }));
                     _a.register_alias("xwheel_zoom", () => new WheelZoomTool({
                         dimensions: "width"
```

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/bokeh.min.js` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/bokeh.min.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -533,15 +533,15 @@
                 s();
                 const r = e(1);
                 l("version", e(3).version), l("index", e(4).index), o.embed = r.__importStar(e(4)), o.protocol = r.__importStar(e(67)), o._testing = r.__importStar(e(68));
                 var _ = e(18);
                 l("logger", _.logger), l("set_log_level", _.set_log_level), l("settings", e(28).settings), l("Models", e(7).default_resolver), l("documents", e(5).documents), l("safely", e(69).safely)
             },
             function _(n, e, i, o, v) {
-                o(), i.version = "3.2.0-dev.3"
+                o(), i.version = "3.2.0-dev.4"
             },
             function _(e, o, t, n, r) {
                 n();
                 const s = e(5),
                     d = e(28),
                     i = e(18),
                     _ = e(38),
@@ -949,34 +949,34 @@
                     a = e(14),
                     f = e(45);
                 r.default_resolver = new f.ModelResolver(null), r.register_models = function(e, o = !1) {
                     for (const t of (0, l.isArray)(e) ? e : (0, n.values)(e)) s = t, (0, l.isObject)(s) && s.prototype instanceof a.HasProps && r.default_resolver.register(t, o);
                     var s
                 }
             },
-            function _(n, t, r, i, o) {
-                i();
+            function _(n, t, r, e, i) {
+                e();
                 //     (c) 2009-2015 Jeremy Ashkenas, DocumentCloud and Investigative Reporters & Editors
                 //     Underscore may be freely distributed under the MIT license.
-                const u = Object.prototype.toString;
+                const o = Object.prototype.toString;
 
-                function e(n) {
+                function u(n) {
                     return null == n
                 }
 
                 function c(n) {
-                    return !0 === n || !1 === n || "[object Boolean]" === u.call(n)
+                    return !0 === n || !1 === n || "[object Boolean]" === o.call(n)
                 }
 
-                function f(n) {
-                    return "[object Number]" === u.call(n)
+                function s(n) {
+                    return "[object Number]" === o.call(n)
                 }
 
-                function s(n) {
-                    return "[object String]" === u.call(n)
+                function f(n) {
+                    return "[object String]" === o.call(n)
                 }
 
                 function l(n) {
                     return "symbol" == typeof n
                 }
 
                 function a(n) {
@@ -987,41 +987,48 @@
                 function b(n) {
                     return a(n) && Symbol.iterator in n
                 }
                 r.is_undefined = function(n) {
                     return void 0 === n
                 }, r.is_defined = function(n) {
                     return void 0 !== n
-                }, r.is_nullish = e, r.isNull = function(n) {
+                }, r.is_nullish = u, r.isNull = function(n) {
                     return null == n
                 }, r.isNotNull = function(n) {
                     return null != n
-                }, r.isBoolean = c, r.isNumber = f, r.isInteger = function(n) {
-                    return f(n) && Number.isInteger(n)
-                }, r.isString = s, r.isSymbol = l, r.isPrimitive = function(n) {
-                    return null === n || c(n) || f(n) || s(n) || l(n)
+                }, r.isBoolean = c, r.isNumber = s, r.isInteger = function(n) {
+                    return s(n) && Number.isInteger(n)
+                }, r.isString = f, r.isSymbol = l, r.isPrimitive = function(n) {
+                    return null === n || c(n) || s(n) || f(n) || l(n)
                 }, r.isFunction = function(n) {
-                    const t = u.call(n);
-                    return "[object Function]" === t || "[object AsyncFunction]" === t
+                    switch (o.call(n)) {
+                        case "[object Function]":
+                        case "[object AsyncFunction]":
+                        case "[object GeneratorFunction]":
+                        case "[object AsyncGeneratorFunction]":
+                            return !0;
+                        default:
+                            return !1
+                    }
                 }, r.isArray = function(n) {
                     return Array.isArray(n)
                 }, r.isArrayOf = function(n, t) {
                     for (const r of n)
                         if (!t(r)) return !1;
                     return !0
                 }, r.isArrayableOf = function(n, t) {
                     for (const r of n)
                         if (!t(r)) return !1;
                     return !0
                 }, r.isTypedArray = function(n) {
                     return ArrayBuffer.isView(n) && !(n instanceof DataView)
                 }, r.isObject = a, r.isBasicObject = function(n) {
-                    return a(n) && e(n.constructor)
+                    return a(n) && u(n.constructor)
                 }, r.isPlainObject = function(n) {
-                    return a(n) && (e(n.constructor) || n.constructor === Object)
+                    return a(n) && (u(n.constructor) || n.constructor === Object)
                 }, r.isIterable = b, r.isArrayable = function(n) {
                     return b(n) && "length" in n
                 }
             },
             function _(t, e, s, n, i) {
                 var o;
                 n();
@@ -1141,16 +1148,17 @@
                         r = new Array(t);
                     for (let o = 0; o < t; o++) {
                         r[o] = new Array(e);
                         for (let t = 0; t < e; t++) r[o][t] = n[t][o]
                     }
                     return r
                 }, e.unzip = function(n) {
-                    const t = n.length,
-                        e = (0, s.min)(n.map((n => n.length))),
+                    const t = n.length;
+                    if (0 == t) return [];
+                    const e = (0, s.min)(n.map((n => n.length))),
                         r = Array(e);
                     for (let n = 0; n < e; n++) r[n] = new Array(t);
                     for (let o = 0; o < t; o++)
                         for (let t = 0; t < e; t++) r[t][o] = n[o][t];
                     return r
                 }, e.range = m, e.linspace = function(n, t, e = 100) {
                     const r = 1 == e ? 0 : (t - n) / (e - 1),
@@ -3428,20 +3436,24 @@
                     whitesmoke: 4126537215,
                     yellow: 4294902015,
                     yellowgreen: 2597139199
                 }, l.is_named_color = function(e) {
                     return e in l.named_colors
                 }
             },
-            function _(r, t, n, a, o) {
-                a(), n.GeneratorFunction = Object.getPrototypeOf((function*() {})).constructor, n.ColorArray = Uint32Array, n.RGBAArray = Uint8ClampedArray, n.infer_type = function(r, t) {
+            function _(r, t, n, o, a) {
+                o();
+                const e = r(1);
+                n.GeneratorFunction = Object.getPrototypeOf((function*() {})).constructor, n.AsyncGeneratorFunction = Object.getPrototypeOf((function() {
+                    return e.__asyncGenerator(this, arguments, (function*() {}))
+                })).constructor, n.ColorArray = Uint32Array, n.RGBAArray = Uint8ClampedArray, n.infer_type = function(r, t) {
                     return r instanceof Float64Array || r instanceof Array || t instanceof Float64Array || t instanceof Array ? Float64Array : Float32Array
                 }, n.ScreenArray = Float32Array, n.to_screen = function(r) {
                     return r instanceof Float32Array ? r : Float32Array.from(r)
-                }, o("Indices", r(24).BitSet)
+                }, a("Indices", r(24).BitSet)
             },
             function _(t, s, r, e, i) {
                 var n;
                 e();
                 const o = t(25),
                     _ = t(12);
                 class h {
@@ -6367,27 +6379,21 @@
                     get y_range() {
                         return {
                             start: this.y0,
                             end: this.y1
                         }
                     }
                     get h_range() {
-                        return {
-                            start: this.x0,
-                            end: this.x1
-                        }
+                        return this.x_range
                     }
                     get v_range() {
-                        return {
-                            start: this.y0,
-                            end: this.y1
-                        }
+                        return this.y_range
                     }
                     get ranges() {
-                        return [this.h_range, this.v_range]
+                        return [this.x_range, this.y_range]
                     }
                     get aspect() {
                         return this.width / this.height
                     }
                     get hcenter() {
                         return (this.left + this.right) / 2
                     }
@@ -7204,41 +7210,42 @@
                     }
                 }
                 i.Annotation = a, o = a, a.__name__ = "Annotation", o.override({
                     level: "annotation"
                 })
             },
             function _(e, t, i, n, s) {
-                var r, o;
+                var r, a;
                 n();
-                const a = e(1),
-                    _ = e(54),
-                    l = a.__importStar(e(75)),
+                const o = e(1),
+                    l = e(54),
+                    _ = o.__importStar(e(75)),
                     d = e(19),
                     h = e(50),
-                    u = e(84);
-                class c extends h.Model {
+                    u = e(12),
+                    c = e(84);
+                class p extends h.Model {
                     constructor(e) {
                         super(e)
                     }
                 }
-                i.RendererGroup = c, r = c, c.__name__ = "RendererGroup", r.define((({
+                i.RendererGroup = p, r = p, p.__name__ = "RendererGroup", r.define((({
                     Boolean: e
                 }) => ({
                     visible: [e, !0]
                 })));
-                class p extends _.View {
+                class g extends l.View {
                     get coordinates() {
                         const {
                             _coordinates: e
                         } = this;
                         return null != e ? e : this._coordinates = this._initialize_coordinates()
                     }
                     initialize() {
-                        super.initialize(), this.visuals = new l.Visuals(this)
+                        super.initialize(), this.visuals = new _.Visuals(this)
                     }
                     connect_signals() {
                         super.connect_signals();
                         const {
                             group: e
                         } = this.model;
                         null != e && this.on_change(e.properties.visible, (() => {
@@ -7257,15 +7264,15 @@
                             frame: t
                         } = this.plot_view;
                         if (null != e) return e.get_transform(t); {
                             const {
                                 x_range_name: e,
                                 y_range_name: i
                             } = this.model, n = t.x_scales.get(e), s = t.y_scales.get(i);
-                            return new u.CoordinateTransform(n, s)
+                            return (0, u.assert)(null != n, `missing '${e}' range`), (0, u.assert)(null != s, `missing '${i}' range`), new c.CoordinateTransform(n, s)
                         }
                     }
                     get plot_view() {
                         return this.parent
                     }
                     get plot_model() {
                         return this.parent.model
@@ -7307,32 +7314,32 @@
                     render() {
                         this.displayed && this._render(), this._has_finished = !0
                     }
                     renderer_view(e) {}
                     update_geometry() {}
                     compute_geometry() {}
                 }
-                i.RendererView = p, p.__name__ = "RendererView";
-                class g extends h.Model {
+                i.RendererView = g, g.__name__ = "RendererView";
+                class m extends h.Model {
                     constructor(e) {
                         super(e)
                     }
                 }
-                i.Renderer = g, o = g, g.__name__ = "Renderer", o.define((({
+                i.Renderer = m, a = m, m.__name__ = "Renderer", a.define((({
                     Boolean: e,
                     String: t,
                     Ref: i,
                     Nullable: n
                 }) => ({
-                    group: [n(i(c)), null],
+                    group: [n(i(p)), null],
                     level: [d.RenderLevel, "image"],
                     visible: [e, !0],
                     x_range_name: [t, "default"],
                     y_range_name: [t, "default"],
-                    coordinates: [n(i(u.CoordinateMapping)), null],
+                    coordinates: [n(i(c.CoordinateMapping)), null],
                     propagate_hover: [e, !1]
                 })))
             },
             function _(e, a, r, t, c) {
                 t();
                 const n = e(1),
                     l = e(76);
@@ -7901,50 +7908,50 @@
                     }
                     font_value(t) {
                         return `${this.text_font_style.get(t)} ${this.text_font_size.get(t)} ${this.text_font.get(t)}`
                     }
                 }
                 l.TextVector = c, c.__name__ = "TextVector", u.prototype.type = "text", u.prototype.attrs = Object.keys(a.Text), x.prototype.type = "text", x.prototype.attrs = Object.keys(a.TextScalar), c.prototype.type = "text", c.prototype.attrs = Object.keys(a.TextVector)
             },
-            function _(t, e, a, r, h) {
+            function _(t, e, a, r, i) {
                 r();
-                const i = t(1),
+                const h = t(1),
                     s = t(77),
                     n = t(82),
-                    c = i.__importStar(t(17)),
-                    _ = i.__importStar(t(78));
+                    c = h.__importStar(t(17)),
+                    _ = h.__importStar(t(78));
                 class l extends s.VisualProperties {
                     constructor() {
                         super(...arguments), this._update_iteration = 0
                     }
                     update() {
                         if (this._update_iteration++, this._hatch_image = null, !this.doit) return;
                         const t = this.hatch_color.get_value(),
                             e = this.hatch_alpha.get_value(),
                             a = this.hatch_scale.get_value(),
                             r = this.hatch_pattern.get_value(),
-                            h = this.hatch_weight.get_value(),
-                            i = t => {
+                            i = this.hatch_weight.get_value(),
+                            h = t => {
                                 this._hatch_image = t
                             },
                             s = this.hatch_extra.get_value()[r];
                         if (null != s) {
-                            const r = s.get_pattern(t, e, a, h);
+                            const r = s.get_pattern(t, e, a, i);
                             if (r instanceof Promise) {
                                 const {
                                     _update_iteration: t
                                 } = this;
                                 r.then((e => {
-                                    this._update_iteration == t && (i(e), this.obj.request_render())
+                                    this._update_iteration == t && (h(e), this.obj.request_render())
                                 }))
-                            } else i(r)
+                            } else h(r)
                         } else {
                             const s = this.obj.canvas.create_layer(),
-                                c = (0, n.get_pattern)(s, r, t, e, a, h);
-                            i(c)
+                                c = (0, n.get_pattern)(s, r, t, e, a, i);
+                            h(c)
                         }
                     }
                     get doit() {
                         const t = this.hatch_color.get_value(),
                             e = this.hatch_alpha.get_value(),
                             a = this.hatch_pattern.get_value();
                         return !(null == t || 0 == e || " " == a || "blank" == a || null == a)
@@ -7984,42 +7991,42 @@
                     constructor() {
                         super(...arguments), this._static_doit = !1, this._update_iteration = 0
                     }
                     _compute_static_doit() {
                         const t = this.hatch_color.value,
                             e = this.hatch_alpha.value,
                             a = this.hatch_pattern.value;
-                        return !(null == t || 0 == e || " " == a || "blank" == a || null == a)
+                        return !(0 == t || 0 == e || " " == a || "blank" == a || null == a)
                     }
                     update() {
                         this._update_iteration++;
                         const t = this.hatch_color.length;
                         if (this._hatch_image = new c.UniformScalar(null, t), this._static_doit = this._compute_static_doit(), !this._static_doit) return;
                         const e = this.hatch_color.value,
                             a = this.hatch_alpha.value,
                             r = this.hatch_scale.value,
-                            h = this.hatch_pattern.value,
-                            i = this.hatch_weight.value,
+                            i = this.hatch_pattern.value,
+                            h = this.hatch_weight.value,
                             s = e => {
                                 this._hatch_image = new c.UniformScalar(e, t)
                             },
-                            _ = this.hatch_extra.value[h];
+                            _ = this.hatch_extra.value[i];
                         if (null != _) {
-                            const t = _.get_pattern(e, a, r, i);
+                            const t = _.get_pattern(e, a, r, h);
                             if (t instanceof Promise) {
                                 const {
                                     _update_iteration: e
                                 } = this;
                                 t.then((t => {
                                     this._update_iteration == e && (s(t), this.obj.request_render())
                                 }))
                             } else s(t)
                         } else {
                             const t = this.obj.canvas.create_layer(),
-                                c = (0, n.get_pattern)(t, h, e, a, r, i);
+                                c = (0, n.get_pattern)(t, i, e, a, r, h);
                             s(c)
                         }
                     }
                     get doit() {
                         return this._static_doit
                     }
                     apply(t, e) {
@@ -8033,27 +8040,29 @@
                         t.fillStyle = null !== (e = this.pattern(t)) && void 0 !== e ? e : "transparent"
                     }
                     pattern(t) {
                         const e = this._hatch_image.value;
                         return null == e ? null : t.createPattern(e, this.repetition())
                     }
                     repetition() {
-                        const t = this.hatch_pattern.value,
-                            e = this.hatch_extra.value[t];
-                        if (null == e) return "repeat";
-                        switch (e.repetition) {
-                            case "repeat":
-                                return "repeat";
-                            case "repeat_x":
-                                return "repeat-x";
-                            case "repeat_y":
-                                return "repeat-y";
-                            case "no_repeat":
-                                return "no-repeat"
+                        const t = this.hatch_pattern.value;
+                        if (null != t) {
+                            const e = this.hatch_extra.value[t];
+                            if (null != e) switch (e.repetition) {
+                                case "repeat":
+                                    return "repeat";
+                                case "repeat_x":
+                                    return "repeat-x";
+                                case "repeat_y":
+                                    return "repeat-y";
+                                case "no_repeat":
+                                    return "no-repeat"
+                            }
                         }
+                        return "repeat"
                     }
                 }
                 a.HatchScalar = o, o.__name__ = "HatchScalar";
                 class u extends s.VisualUniforms {
                     constructor() {
                         super(...arguments), this._static_doit = !1, this._update_iteration = 0
                     }
@@ -8075,47 +8084,47 @@
                         }
                         return !0
                     }
                     update() {
                         this._update_iteration++;
                         const t = this.hatch_color.length;
                         if (this._hatch_image = new c.UniformScalar(null, t), this._static_doit = this._compute_static_doit(), !this._static_doit) return;
-                        const e = (t, e, a, r, h, i) => {
+                        const e = (t, e, a, r, i, h) => {
                             const s = this.hatch_extra.value[t];
                             if (null != s) {
-                                const t = s.get_pattern(e, a, r, h);
+                                const t = s.get_pattern(e, a, r, i);
                                 if (t instanceof Promise) {
                                     const {
                                         _update_iteration: e
                                     } = this;
                                     t.then((t => {
-                                        this._update_iteration == e && (i(t), this.obj.request_render())
+                                        this._update_iteration == e && (h(t), this.obj.request_render())
                                     }))
-                                } else i(t)
+                                } else h(t)
                             } else {
                                 const s = this.obj.canvas.create_layer(),
-                                    c = (0, n.get_pattern)(s, t, e, a, r, h);
-                                i(c)
+                                    c = (0, n.get_pattern)(s, t, e, a, r, i);
+                                h(c)
                             }
                         };
                         if (this.hatch_color.is_Scalar() && this.hatch_alpha.is_Scalar() && this.hatch_scale.is_Scalar() && this.hatch_pattern.is_Scalar() && this.hatch_weight.is_Scalar()) {
                             const a = this.hatch_color.value,
                                 r = this.hatch_alpha.value,
-                                h = this.hatch_scale.value;
-                            e(this.hatch_pattern.value, a, r, h, this.hatch_weight.value, (e => {
+                                i = this.hatch_scale.value;
+                            e(this.hatch_pattern.value, a, r, i, this.hatch_weight.value, (e => {
                                 this._hatch_image = new c.UniformScalar(e, t)
                             }))
                         } else {
                             const a = new Array(t);
                             a.fill(null), this._hatch_image = new c.UniformVector(a);
                             for (let r = 0; r < t; r++) {
                                 const t = this.hatch_color.get(r),
-                                    h = this.hatch_alpha.get(r),
-                                    i = this.hatch_scale.get(r);
-                                e(this.hatch_pattern.get(r), t, h, i, this.hatch_weight.get(r), (t => {
+                                    i = this.hatch_alpha.get(r),
+                                    h = this.hatch_scale.get(r);
+                                e(this.hatch_pattern.get(r), t, i, h, this.hatch_weight.get(r), (t => {
                                     a[r] = t
                                 }))
                             }
                         }
                     }
                     get doit() {
                         return this._static_doit
@@ -8136,27 +8145,29 @@
                         t.fillStyle = null !== (a = this.pattern(t, e)) && void 0 !== a ? a : "transparent"
                     }
                     pattern(t, e) {
                         const a = this._hatch_image.get(e);
                         return null == a ? null : t.createPattern(a, this.repetition(e))
                     }
                     repetition(t) {
-                        const e = this.hatch_pattern.get(t),
-                            a = this.hatch_extra.value[e];
-                        if (null == a) return "repeat";
-                        switch (a.repetition) {
-                            case "repeat":
-                                return "repeat";
-                            case "repeat_x":
-                                return "repeat-x";
-                            case "repeat_y":
-                                return "repeat-y";
-                            case "no_repeat":
-                                return "no-repeat"
+                        const e = this.hatch_pattern.get(t);
+                        if (null != e) {
+                            const t = this.hatch_extra.value[e];
+                            if (null != t) switch (t.repetition) {
+                                case "repeat":
+                                    return "repeat";
+                                case "repeat_x":
+                                    return "repeat-x";
+                                case "repeat_y":
+                                    return "repeat-y";
+                                case "no_repeat":
+                                    return "no-repeat"
+                            }
                         }
+                        return "repeat"
                     }
                 }
                 a.HatchVector = u, u.__name__ = "HatchVector", l.prototype.type = "hatch", l.prototype.attrs = Object.keys(_.Hatch), o.prototype.type = "hatch", o.prototype.attrs = Object.keys(_.HatchScalar), u.prototype.type = "hatch", u.prototype.attrs = Object.keys(_.HatchVector)
             },
             function _(e, o, a, r, s) {
                 r();
                 const i = e(18),
@@ -13855,14 +13866,17 @@
                     y = t(148),
                     {
                         abs: z
                     } = Math;
                 class M extends n.GuideRendererView {
                     constructor() {
                         super(...arguments), this._axis_label_view = null, this._major_label_views = new Map
+                    }
+                    get bbox() {
+                        return this.layout.bbox
                     }* children() {
                         yield* super.children(), null != this._axis_label_view && (yield this._axis_label_view), yield* this._major_label_views.values()
                     }
                     async lazy_initialize() {
                         await super.lazy_initialize(), await this._init_axis_label(), await this._init_major_labels()
                     }
                     async _init_axis_label() {
@@ -16454,18 +16468,18 @@
                 n.Mapper = t, t.__name__ = "Mapper"
             },
             function _(e, t, i, s, l) {
                 var h;
                 s();
                 const n = e(200),
                     o = e(201),
-                    a = e(211),
-                    c = e(212),
-                    _ = e(215),
-                    d = e(216),
+                    c = e(211),
+                    a = e(212),
+                    d = e(215),
+                    _ = e(216),
                     r = e(217),
                     p = e(203),
                     g = e(99),
                     y = e(218),
                     u = e(23),
                     m = e(13),
                     v = e(9),
@@ -16529,21 +16543,21 @@
                                 fill: {},
                                 line: {}
                             })
                         }
                         delete l.id;
                         let {
                             selection_glyph: o,
-                            nonselection_glyph: a,
-                            hover_glyph: c,
-                            muted_glyph: _
+                            nonselection_glyph: c,
+                            hover_glyph: a,
+                            muted_glyph: d
                         } = this.model;
-                        o = n(G, o), this.selection_glyph = await this.build_glyph_view(o), a = n(R, a), this.nonselection_glyph = await this.build_glyph_view(a), null != c && (this.hover_glyph = await this.build_glyph_view(c)), _ = n(k, _), this.muted_glyph = await this.build_glyph_view(_);
-                        const d = n(x, "auto");
-                        this.decimated_glyph = await this.build_glyph_view(d), this.selection_glyph.set_base(this.glyph), this.nonselection_glyph.set_base(this.glyph), null === (e = this.hover_glyph) || void 0 === e || e.set_base(this.glyph), this.muted_glyph.set_base(this.glyph), this.decimated_glyph.set_base(this.glyph), this.set_data()
+                        o = n(G, o), this.selection_glyph = await this.build_glyph_view(o), c = n(R, c), this.nonselection_glyph = await this.build_glyph_view(c), null != a && (this.hover_glyph = await this.build_glyph_view(a)), d = n(k, d), this.muted_glyph = await this.build_glyph_view(d);
+                        const _ = n(x, "auto");
+                        this.decimated_glyph = await this.build_glyph_view(_), this.selection_glyph.set_base(this.glyph), this.nonselection_glyph.set_base(this.glyph), null === (e = this.hover_glyph) || void 0 === e || e.set_base(this.glyph), this.muted_glyph.set_base(this.glyph), this.decimated_glyph.set_base(this.glyph), this.set_data()
                     }
                     async build_glyph_view(e) {
                         return (0, f.build_view)(e, {
                             parent: this
                         })
                     }
                     remove() {
@@ -16644,15 +16658,15 @@
                         if (null != this.model.document && this.model.document.interactive_duration() > 0 && !e && null != y && t.length > y ? (i = [...this.decimated], u = this.decimated_glyph, v = this.decimated_glyph, f = this.selection_glyph) : (u = this.model.muted ? this.muted_glyph : this.glyph, v = this.nonselection_glyph, f = this.selection_glyph), null != this.hover_glyph && 0 != g.length) {
                             const e = new Set(i);
                             for (const t of g) e.delete(t);
                             i = [...e]
                         }
                         if (0 == h.length)
                             if (this.glyph instanceof o.LineView) null != this.hover_glyph && 0 != g.length ? this.hover_glyph.render(s, this.model.view.convert_indices_from_subset(g)) : u.render(s, t);
-                            else if (this.glyph instanceof a.PatchView || this.glyph instanceof _.HAreaView || this.glyph instanceof r.VAreaView || this.glyph instanceof d.VAreaStepView || this.glyph instanceof c.HAreaStepView)
+                            else if (this.glyph instanceof c.PatchView || this.glyph instanceof d.HAreaView || this.glyph instanceof r.VAreaView || this.glyph instanceof _.VAreaStepView || this.glyph instanceof a.HAreaStepView)
                             if (0 == n.selected_glyphs.length || null == this.hover_glyph) u.render(s, t);
                             else
                                 for (const e of n.selected_glyphs) e == this.glyph.model && this.hover_glyph.render(s, t);
                         else u.render(s, i), null != this.hover_glyph && 0 != g.length && this.hover_glyph.render(s, g);
                         else {
                             const e = new Set(h),
                                 l = new Array,
@@ -16671,20 +16685,29 @@
                             if (null != i)
                                 for (const [e, s] of(0, v.entries)(this.model.view.indices_map))
                                     if (i[parseInt(e)] == t) return s
                         }
                         return 0
                     }
                     draw_legend(e, t, i, s, l, h, n, o) {
-                        0 != this.glyph.data_size && (null == o && (o = this.get_reference_point(h, n)), this.glyph.draw_legend_for_index(e, {
+                        if (0 == this.glyph.data_size) return;
+                        const c = (() => {
+                            if (null == o) return this.get_reference_point(h, n); {
+                                const {
+                                    indices_map: e
+                                } = this.model.view;
+                                return o in e ? e[o] : null
+                            }
+                        })();
+                        null != c && this.glyph.draw_legend_for_index(e, {
                             x0: t,
                             x1: i,
                             y0: s,
                             y1: l
-                        }, o))
+                        }, c)
                     }
                     hit_test(e) {
                         if (!this.model.visible) return null;
                         const t = this.glyph.hit_test(e);
                         return null == t ? null : this.model.view.convert_selection_from_subset(t)
                     }
                 }
@@ -21053,23 +21076,23 @@
                         value: 0
                     }]
                 }))), n.override({
                     background_fill_color: null,
                     border_line_color: null
                 })
             },
-            function _(t, e, i, s, n) {
+            function _(t, e, i, n, s) {
                 var o;
-                s();
+                n();
                 const l = t(1),
                     r = t(73),
                     a = t(254),
-                    _ = t(19),
-                    c = l.__importStar(t(78)),
-                    h = t(15),
+                    c = t(19),
+                    h = l.__importStar(t(78)),
+                    _ = t(15),
                     d = t(144),
                     u = t(57),
                     b = t(10),
                     g = t(32),
                     p = t(8),
                     m = t(151),
                     f = t(229),
@@ -21083,30 +21106,30 @@
                     }
                     _content_size() {
                         return new f.Sizeable(this.text.size())
                     }
                 }
                 y.__name__ = "TextLayout";
                 class v extends f.ContentLayoutable {
-                    constructor(t, e, i, s) {
-                        super(), this.item = t, this.label = e, this.text = i, this.settings = s
+                    constructor(t, e, i, n) {
+                        super(), this.item = t, this.label = e, this.text = i, this.settings = n
                     }
                     get field() {
                         return this.item.get_field_from_label_prop()
                     }
                     _content_size() {
                         const t = this.text.size(),
                             {
                                 glyph_width: e,
                                 glyph_height: i,
-                                label_standoff: s,
-                                label_width: n,
+                                label_standoff: n,
+                                label_width: s,
                                 label_height: o
                             } = this.settings,
-                            l = e + s + x(t.width, n),
+                            l = e + n + x(t.width, s),
                             r = x(i, t.height, o);
                         return new f.Sizeable({
                             width: l,
                             height: r
                         })
                     }
                 }
@@ -21132,84 +21155,82 @@
                         const {
                             panel: t
                         } = this;
                         this.layout = null != t ? new d.SideLayout(t, (() => this.get_size())) : void 0
                     }
                     connect_signals() {
                         super.connect_signals();
-                        const t = () => {
-                            this.update_geometry(), this.request_render()
-                        };
+                        const t = () => this.request_render();
                         this.connect(this.model.change, t), this.connect(this.model.item_change, t)
                     }
                     get padding() {
                         return null != this.model.border_line_color ? this.model.padding : 0
                     }
                     update_geometry() {
                         super.update_geometry();
                         const {
                             spacing: t,
                             orientation: e
                         } = this.model, i = "vertical" == e, {
-                            padding: s
-                        } = this, n = s, o = s, {
+                            padding: n
+                        } = this, s = n, o = n, {
                             title: l
                         } = this.model, r = new m.TextBox({
                             text: null != l ? l : ""
                         });
                         r.position = {
                             sx: 0,
                             sy: 0,
                             x_anchor: "left",
                             y_anchor: "top"
                         }, r.visuals = this.visuals.title_text.values();
                         const a = new d.Panel(this.model.title_location);
                         r.angle = a.get_label_angle_heuristic("parallel");
-                        const _ = [];
+                        const c = [];
                         for (const t of this.model.items) {
                             t.legend = this.model;
                             const e = t.get_labels_list_from_label_prop();
                             for (const i of e) {
                                 const e = new m.TextBox({
                                     text: `${i}`
                                 });
                                 e.position = {
                                     sx: 0,
                                     sy: 0,
                                     x_anchor: "left",
                                     y_anchor: "center"
                                 }, e.visuals = this.visuals.label_text.values();
-                                const s = new v(t, i, e, this.model);
-                                s.set_sizing({
+                                const n = new v(t, i, e, this.model);
+                                n.set_sizing({
                                     visible: t.visible
-                                }), _.push({
-                                    layout: s,
+                                }), c.push({
+                                    layout: n,
                                     row: 0,
                                     col: 0
                                 })
                             }
                         }
                         const {
-                            ncols: c,
-                            nrows: h
+                            ncols: h,
+                            nrows: _
                         } = (() => {
                             let {
                                 ncols: t,
                                 nrows: e
                             } = this.model;
-                            const s = _.length;
-                            return i ? ("auto" != e || (e = "auto" != t ? w(s / t) : 1 / 0), t = 1 / 0) : ("auto" != t || (t = "auto" != e ? w(s / e) : 1 / 0), e = 1 / 0), {
+                            const n = c.length;
+                            return i ? ("auto" != e || (e = "auto" != t ? w(n / t) : 1 / 0), t = 1 / 0) : ("auto" != t || (t = "auto" != e ? w(n / e) : 1 / 0), e = 1 / 0), {
                                 ncols: t,
                                 nrows: e
                             }
                         })();
                         let b = 0,
                             g = 0;
-                        for (const t of _) t.row = b, t.col = g, i ? (b += 1, b >= h && (b = 0, g += 1)) : (g += 1, g >= c && (g = 0, b += 1));
-                        const p = new f.Grid(_);
+                        for (const t of c) t.row = b, t.col = g, i ? (b += 1, b >= _ && (b = 0, g += 1)) : (g += 1, g >= h && (g = 0, b += 1));
+                        const p = new f.Grid(c);
                         this.grid = p, p.spacing = t, p.set_sizing();
                         const x = new y(r);
                         this.title_panel = x;
                         const k = "" != r.text && this.visuals.title_text.doit;
                         x.set_sizing({
                             visible: k
                         });
@@ -21223,88 +21244,88 @@
                                 case "left":
                                     return new f.Row([x, p]);
                                 case "right":
                                     return new f.Row([p, x])
                             }
                         })();
                         this.border_box = z, z.position = {
-                            left: n,
+                            left: s,
                             top: o
                         }, z.spacing = this.model.title_standoff, z.set_sizing(), z.compute();
-                        const L = s + z.bbox.width + s,
-                            B = s + z.bbox.height + s;
+                        const L = n + z.bbox.width + n,
+                            B = n + z.bbox.height + n;
                         this.bbox = new u.BBox({
                             left: 0,
                             top: 0,
                             width: L,
                             height: B
                         })
                     }
                     compute_geometry() {
                         super.compute_geometry();
                         const {
                             margin: t,
                             location: e
                         } = this.model, {
                             width: i,
-                            height: s
-                        } = this.bbox, n = null != this.layout ? this.layout : this.plot_view.frame, [o, l] = n.bbox.ranges;
+                            height: n
+                        } = this.bbox, s = null != this.layout ? this.layout : this.plot_view.frame, [o, l] = s.bbox.ranges;
                         let r, a;
                         if ((0, p.isString)(e)) switch (e) {
                             case "top_left":
                                 r = o.start + t, a = l.start + t;
                                 break;
                             case "top":
                             case "top_center":
                                 r = (o.end + o.start) / 2 - i / 2, a = l.start + t;
                                 break;
                             case "top_right":
                                 r = o.end - t - i, a = l.start + t;
                                 break;
                             case "bottom_right":
-                                r = o.end - t - i, a = l.end - t - s;
+                                r = o.end - t - i, a = l.end - t - n;
                                 break;
                             case "bottom":
                             case "bottom_center":
-                                r = (o.end + o.start) / 2 - i / 2, a = l.end - t - s;
+                                r = (o.end + o.start) / 2 - i / 2, a = l.end - t - n;
                                 break;
                             case "bottom_left":
-                                r = o.start + t, a = l.end - t - s;
+                                r = o.start + t, a = l.end - t - n;
                                 break;
                             case "left":
                             case "center_left":
-                                r = o.start + t, a = (l.end + l.start) / 2 - s / 2;
+                                r = o.start + t, a = (l.end + l.start) / 2 - n / 2;
                                 break;
                             case "center":
                             case "center_center":
-                                r = (o.end + o.start) / 2 - i / 2, a = (l.end + l.start) / 2 - s / 2;
+                                r = (o.end + o.start) / 2 - i / 2, a = (l.end + l.start) / 2 - n / 2;
                                 break;
                             case "right":
                             case "center_right":
-                                r = o.end - t - i, a = (l.end + l.start) / 2 - s / 2
+                                r = o.end - t - i, a = (l.end + l.start) / 2 - n / 2
                         } else {
                             const [t, i] = e;
-                            r = n.bbox.xview.compute(t), a = n.bbox.yview.compute(i) - s
+                            r = s.bbox.xview.compute(t), a = s.bbox.yview.compute(i) - n
                         }
                         this.bbox = new u.BBox({
                             left: r,
                             top: a,
                             width: i,
-                            height: s
+                            height: n
                         })
                     }
                     interactive_hit(t, e) {
                         return this.bbox.contains(t, e)
                     }
                     _hit_test(t, e) {
                         const {
                             left: i,
-                            top: s
+                            top: n
                         } = this.bbox;
-                        t -= i + this.grid.bbox.left, e -= s + this.grid.bbox.top;
+                        t -= i + this.grid.bbox.left, e -= n + this.grid.bbox.top;
                         for (const i of this.grid)
                             if (i.bbox.contains(t, e)) return {
                                 type: "entry",
                                 entry: i
                             };
                         return null
                     }
@@ -21318,51 +21339,51 @@
                                         return t => t.visible = !t.visible;
                                     case "mute":
                                         return t => t.muted = !t.muted;
                                     case "none":
                                         return t => {}
                                 }
                             })(),
-                            s = this._hit_test(t, e);
-                        if (null != s) {
+                            n = this._hit_test(t, e);
+                        if (null != n) {
                             const {
                                 renderers: t
-                            } = s.entry.item;
+                            } = n.entry.item;
                             for (const e of t) i(e);
                             return !0
                         }
                         return !1
                     }
                     _render() {
-                        if (this.compute_geometry(), 0 == this.model.items.length) return;
+                        if (this.update_geometry(), this.compute_geometry(), 0 == this.model.items.length) return;
                         if (!(0, b.some)(this.model.items, (t => t.visible))) return;
                         const {
                             ctx: t
                         } = this.layer;
                         t.save(), this._draw_legend_box(t), this._draw_legend_items(t), this._draw_title(t), t.restore()
                     }
                     _draw_legend_box(t) {
                         const {
                             x: e,
                             y: i,
-                            width: s,
-                            height: n
+                            width: n,
+                            height: s
                         } = this.bbox;
-                        t.beginPath(), t.rect(e, i, s, n), this.visuals.background_fill.apply(t), this.visuals.border_line.apply(t)
+                        t.beginPath(), t.rect(e, i, n, s), this.visuals.background_fill.apply(t), this.visuals.border_line.apply(t)
                     }
                     _draw_title(t) {
                         const {
                             title: e
                         } = this.model;
                         if (null == e || 0 == e.length || !this.visuals.title_text.doit) return;
                         const {
                             left: i,
-                            top: s
+                            top: n
                         } = this.bbox;
-                        switch (t.save(), t.translate(i, s), t.translate(this.title_panel.bbox.left, this.title_panel.bbox.top), this.model.title_location) {
+                        switch (t.save(), t.translate(i, n), t.translate(this.title_panel.bbox.left, this.title_panel.bbox.top), this.model.title_location) {
                             case "left":
                                 t.translate(0, this.title_panel.bbox.height);
                                 break;
                             case "right":
                                 t.translate(this.title_panel.bbox.width, 0)
                         }
                         this.title_panel.text.paint(t), t.restore()
@@ -21388,109 +21409,101 @@
                                     case "odd":
                                         return e % 2 == 0 != (i % 2 == 0);
                                     case "none":
                                         return !1
                                 }
                             },
                             {
-                                left: s,
-                                top: n
+                                left: n,
+                                top: s
                             } = this.bbox;
-                        t.translate(s, n), t.translate(this.grid.bbox.left, this.grid.bbox.top);
+                        t.translate(n, s), t.translate(this.grid.bbox.left, this.grid.bbox.top);
                         for (const [{
-                                layout: s,
-                                row: n,
+                                layout: n,
+                                row: s,
                                 col: o
                             }, l] of(0, g.enumerate)(this.grid.items)) {
                             const {
                                 bbox: l,
                                 text: r,
                                 item: a,
-                                label: _,
-                                field: c,
-                                settings: h
-                            } = s, {
+                                label: c,
+                                field: h,
+                                settings: _
+                            } = n, {
                                 glyph_width: d,
                                 glyph_height: u,
                                 label_standoff: b
-                            } = h, {
+                            } = _, {
                                 left: g,
                                 top: p,
                                 width: m,
                                 height: f
                             } = l;
-                            t.translate(g, p), i(0, n, o) && (t.beginPath(), t.rect(0, 0, m, f), this.visuals.item_background_fill.apply(t));
+                            t.translate(g, p), i(0, s, o) && (t.beginPath(), t.rect(0, 0, m, f), this.visuals.item_background_fill.apply(t));
                             const x = f / 2,
                                 w = 0,
                                 y = x - u / 2,
                                 v = w + d,
                                 k = y + u;
                             for (const e of a.renderers) {
                                 const i = this.plot_view.renderer_view(e);
-                                null == i || i.draw_legend(t, w, v, y, k, c, _, a.index)
+                                null == i || i.draw_legend(t, w, v, y, k, h, c, a.index)
                             }
                             t.translate(v + b, x), r.paint(t), t.translate(-v - b, -x), e(a) || (t.beginPath(), t.rect(0, 0, m, f), this.visuals.inactive_fill.set_value(t), t.fill()), t.translate(-g, -p)
                         }
-                        t.translate(-this.grid.bbox.left, -this.grid.bbox.top), t.translate(-s, -n)
+                        t.translate(-this.grid.bbox.left, -this.grid.bbox.top), t.translate(-n, -s)
                     }
                 }
                 i.LegendView = k, k.__name__ = "LegendView";
                 class z extends r.Annotation {
                     constructor(t) {
                         super(t)
                     }
                     initialize() {
-                        super.initialize(), this.item_change = new h.Signal0(this, "item_change")
-                    }
-                    get_legend_names() {
-                        const t = [];
-                        for (const e of this.items) {
-                            const i = e.get_labels_list_from_label_prop();
-                            t.push(...i)
-                        }
-                        return t
+                        super.initialize(), this.item_change = new _.Signal0(this, "item_change")
                     }
                 }
                 i.Legend = z, o = z, z.__name__ = "Legend", o.prototype.default_view = k, o.mixins([
-                    ["label_", c.Text],
-                    ["title_", c.Text],
-                    ["inactive_", c.Fill],
-                    ["border_", c.Line],
-                    ["background_", c.Fill],
-                    ["item_background_", c.Fill]
+                    ["label_", h.Text],
+                    ["title_", h.Text],
+                    ["inactive_", h.Fill],
+                    ["border_", h.Line],
+                    ["background_", h.Fill],
+                    ["item_background_", h.Fill]
                 ]), o.define((({
                     Number: t,
                     Int: e,
                     String: i,
-                    Array: s,
-                    Tuple: n,
+                    Array: n,
+                    Tuple: s,
                     Or: o,
                     Ref: l,
                     Nullable: r,
-                    Positive: c,
-                    Auto: h
+                    Positive: h,
+                    Auto: _
                 }) => ({
-                    orientation: [_.Orientation, "vertical"],
-                    ncols: [o(c(e), h), "auto"],
-                    nrows: [o(c(e), h), "auto"],
-                    location: [o(_.LegendLocation, n(t, t)), "top_right"],
+                    orientation: [c.Orientation, "vertical"],
+                    ncols: [o(h(e), _), "auto"],
+                    nrows: [o(h(e), _), "auto"],
+                    location: [o(c.LegendLocation, s(t, t)), "top_right"],
                     title: [r(i), null],
-                    title_location: [_.Location, "above"],
+                    title_location: [c.Location, "above"],
                     title_standoff: [t, 5],
                     label_standoff: [t, 5],
                     glyph_height: [t, 20],
                     glyph_width: [t, 20],
                     label_height: [t, 20],
                     label_width: [t, 20],
                     margin: [t, 10],
                     padding: [t, 10],
                     spacing: [t, 3],
-                    items: [s(l(a.LegendItem)), []],
-                    click_policy: [_.LegendClickPolicy, "none"],
-                    item_background_policy: [_.AlternationPolicy, "none"]
+                    items: [n(l(a.LegendItem)), []],
+                    click_policy: [c.LegendClickPolicy, "none"],
+                    item_background_policy: [c.AlternationPolicy, "none"]
                 }))), o.override({
                     border_line_color: "#e5e5e5",
                     border_line_alpha: .5,
                     border_line_width: 1,
                     background_fill_color: "#ffffff",
                     background_fill_alpha: .95,
                     item_background_fill_color: "#f1f1f1",
@@ -21499,26 +21512,26 @@
                     inactive_fill_alpha: .7,
                     label_text_font_size: "13px",
                     label_text_baseline: "middle",
                     title_text_font_size: "13px",
                     title_text_font_style: "italic"
                 })
             },
-            function _(e, r, l, n, t) {
+            function _(e, r, n, l, t) {
                 var i;
-                n();
+                l();
                 const s = e(1),
                     o = e(50),
                     _ = e(199),
                     a = e(99),
                     u = e(27),
                     d = s.__importStar(e(17)),
                     c = e(18),
-                    f = e(10);
-                class h extends o.Model {
+                    h = e(10);
+                class f extends o.Model {
                     constructor(e) {
                         super(e)
                     }
                     _check_data_sources_on_renderers() {
                         if (null != this.get_field_from_label_prop()) {
                             if (this.renderers.length < 1) return !1;
                             const e = this.renderers[0].data_source;
@@ -21528,15 +21541,15 @@
                         return !0
                     }
                     _check_field_label_on_data_source() {
                         const e = this.get_field_from_label_prop();
                         if (null != e) {
                             if (this.renderers.length < 1) return !1;
                             const r = this.renderers[0].data_source;
-                            if (!(0, f.includes)(r.columns(), e)) return !1
+                            if (!(0, h.includes)(r.columns(), e)) return !1
                         }
                         return !0
                     }
                     initialize() {
                         super.initialize(), this.legend = null, this.connect(this.change, (() => {
                             var e;
                             return null === (e = this.legend) || void 0 === e ? void 0 : e.item_change.emit()
@@ -21548,41 +21561,45 @@
                         const {
                             label: e
                         } = this;
                         return (0, u.isField)(e) ? e.field : null
                     }
                     get_labels_list_from_label_prop() {
                         if (!this.visible) return [];
+                        const {
+                            index: e
+                        } = this;
+                        if (null != e && this.renderers.every((r => !(e in r.view.indices_map)))) return [];
                         if ((0, u.isValue)(this.label)) {
                             const {
                                 value: e
                             } = this.label;
                             return null != e ? [e] : []
                         }
-                        const e = this.get_field_from_label_prop();
-                        if (null != e) {
-                            let r;
+                        const r = this.get_field_from_label_prop();
+                        if (null != r) {
+                            let e;
                             if (0 == this.renderers.length) return ["No source found"];
-                            if (r = this.renderers[0].data_source, r instanceof a.ColumnarDataSource) {
-                                const l = r.get_column(e);
-                                return null != l ? (0, f.uniq)(Array.from(l)) : ["Invalid field"]
+                            if (e = this.renderers[0].data_source, e instanceof a.ColumnarDataSource) {
+                                const n = e.get_column(r);
+                                return null != n ? (0, h.uniq)(Array.from(n)) : ["Invalid field"]
                             }
                         }
                         return []
                     }
                 }
-                l.LegendItem = h, i = h, h.__name__ = "LegendItem", i.define((({
+                n.LegendItem = f, i = f, f.__name__ = "LegendItem", i.define((({
                     Boolean: e,
                     Int: r,
-                    Array: l,
-                    Ref: n,
+                    Array: n,
+                    Ref: l,
                     Nullable: t
                 }) => ({
                     label: [d.NullStringSpec, null],
-                    renderers: [l(n(_.GlyphRenderer)), []],
+                    renderers: [n(l(_.GlyphRenderer)), []],
                     index: [t(r), null],
                     visible: [e, !0]
                 })))
             },
             function _(t, e, s, n, i) {
                 var o, a;
                 n();
@@ -25220,45 +25237,86 @@
                     background_fill_color: null,
                     border_line_color: null
                 })
             },
             function _(e, t, u, n, S) {
                 n(), S("CustomJS", e(289).CustomJS), S("OpenURL", e(291).OpenURL), S("SetValue", e(292).SetValue)
             },
-            function _(t, e, s, n, c) {
-                var a;
-                n();
-                const r = t(290),
-                    u = t(9),
-                    o = t(38);
-                class i extends r.Callback {
+            function _(require, module, exports, __esModule, __esExport) {
+                var _a;
+                __esModule();
+                const callback_1 = require(290),
+                    object_1 = require(9),
+                    array_1 = require(10),
+                    string_1 = require(38),
+                    logging_1 = require(18),
+                    types_1 = require(8);
+                class CustomJS extends callback_1.Callback {
                     constructor(t) {
-                        super(t)
+                        super(t), this._state = null
                     }
-                    get names() {
-                        return (0, u.keys)(this.args)
+                    connect_signals() {
+                        super.connect_signals();
+                        const {
+                            args: t,
+                            code: e,
+                            module: s
+                        } = this.properties;
+                        this.on_change([t, e, s], (() => this._state = null))
                     }
-                    get values() {
-                        return (0, u.values)(this.args)
+                    async _compile_module() {
+                        const url = URL.createObjectURL(new Blob([this.code], {
+                            type: "text/javascript"
+                        }));
+                        try {
+                            const module = await eval(`import("${url}")`);
+                            return (0, types_1.isFunction)(module.default) ? module.default : (logging_1.logger.warn("custom ES module didn't export a default function"), () => {})
+                        } finally {
+                            URL.revokeObjectURL(url)
+                        }
                     }
-                    get func() {
-                        const t = (0, o.use_strict)(this.code);
-                        return new Function(...this.names, "cb_obj", "cb_data", t)
+                    async _compile_function() {
+                        const [t = [], e = []] = (0, array_1.unzip)((0, object_1.entries)(this.args)), s = (0, string_1.use_strict)(this.code);
+                        return new Function(...t, "cb_obj", "cb_data", s).bind(void 0, ...e)
                     }
-                    execute(t, e = {}) {
-                        return this.func.apply(t, this.values.concat(t, e))
+                    _is_es_module(t) {
+                        return t.split("\n").some((t => t.trimStart().startsWith("export default")))
+                    }
+                    async _compile() {
+                        const t = (() => "auto" == this.module ? this._is_es_module(this.code) : this.module)();
+                        return t ? {
+                            func: await this._compile_module(),
+                            module: t
+                        } : {
+                            func: await this._compile_function(),
+                            module: t
+                        }
+                    }
+                    async state() {
+                        return null == this._state && (this._state = await this._compile()), this._state
+                    }
+                    async execute(t, e = {}) {
+                        const {
+                            func: s,
+                            module: o
+                        } = await this.state();
+                        return o ? s(this.args, t, e) : s.call(t, t, e)
                     }
                 }
-                s.CustomJS = i, a = i, i.__name__ = "CustomJS", a.define((({
+                exports.CustomJS = CustomJS, _a = CustomJS, CustomJS.__name__ = "CustomJS", _a.define((({
                     Unknown: t,
                     String: e,
-                    Dict: s
+                    Dict: s,
+                    Auto: o,
+                    Or: i,
+                    Boolean: n
                 }) => ({
                     args: [s(t), {}],
-                    code: [e, ""]
+                    code: [e],
+                    module: [i(o, n), "auto"]
                 })))
             },
             function _(c, a, l, n, s) {
                 n();
                 const e = c(50);
                 class o extends e.Model {
                     constructor(c) {
@@ -29127,15 +29185,15 @@
                     o = e(197),
                     i = e(245);
                 class p extends s.ImageBaseView {
                     connect_signals() {
                         super.connect_signals(), this.connect(this.model.color_mapper.change, (() => this._update_image()))
                     }
                     _update_image() {
-                        null != this.image_data && (this._set_data(null), this.renderer.request_render())
+                        null != this._image_data && (this._set_data(null), this.renderer.request_render())
                     }
                     _flat_img_to_buf8(e) {
                         return this.model.color_mapper.rgba_mapper.v_compute(e)
                     }
                 }
                 t.ImageView = p, p.__name__ = "ImageView";
                 class m extends s.ImageBase {
@@ -29147,28 +29205,34 @@
                     Ref: e
                 }) => ({
                     color_mapper: [e(o.ColorMapper), () => new i.LinearColorMapper({
                         palette: ["#000000", "#252525", "#525252", "#737373", "#969696", "#bdbdbd", "#d9d9d9", "#f0f0f0", "#ffffff"]
                     })]
                 })))
             },
-            function _(e, t, i, s, a) {
-                var h;
-                s();
-                const r = e(1),
-                    n = e(202),
+            function _(e, t, s, i, a) {
+                var r;
+                i();
+                const n = e(1),
+                    h = e(202),
                     _ = e(23),
                     o = e(19),
-                    d = r.__importStar(e(17)),
-                    g = r.__importStar(e(78)),
-                    c = e(101),
-                    l = e(12),
+                    d = n.__importStar(e(17)),
+                    c = n.__importStar(e(78)),
+                    l = e(101),
+                    g = e(12),
                     m = e(236),
-                    x = e(238);
-                class u extends n.XYGlyphView {
+                    u = e(238);
+                class x extends h.XYGlyphView {
+                    constructor() {
+                        super(...arguments), this._image_data = null
+                    }
+                    get image_data() {
+                        return (0, g.assert)(null != this._image_data, "data not set"), this._image_data
+                    }
                     connect_signals() {
                         super.connect_signals(), this.connect(this.model.properties.global_alpha.change, (() => this.renderer.request_render()))
                     }
                     get image_dimension() {
                         return 2
                     }
                     get xy_scale() {
@@ -29208,138 +29272,138 @@
                             case "top_right":
                                 return {
                                     x: 1, y: 0
                                 }
                         }
                     }
                     get xy_anchor() {
-                        return (0, x.anchor)(this.model.anchor)
+                        return (0, u.anchor)(this.model.anchor)
                     }
                     get xy_sign() {
                         const e = this.renderer.xscale.source_range,
                             t = this.renderer.yscale.source_range;
                         return {
                             x: e.is_reversed ? -1 : 1,
                             y: t.is_reversed ? -1 : 1
                         }
                     }
-                    _render(e, t, i) {
+                    _render(e, t, s) {
                         const {
-                            image_data: s,
+                            image_data: i,
                             sx: a,
-                            sy: h,
-                            sw: r,
-                            sh: n
-                        } = null != i ? i : this, {
+                            sy: r,
+                            sw: n,
+                            sh: h
+                        } = null != s ? s : this, {
                             xy_sign: _,
                             xy_scale: o,
                             xy_offset: d,
-                            xy_anchor: g
+                            xy_anchor: c
                         } = this;
                         if (e.save(), e.imageSmoothingEnabled = !1, this.visuals.image.doit)
-                            for (const i of t) {
-                                const t = s[i],
-                                    c = a[i],
-                                    l = h[i],
-                                    m = r[i],
-                                    x = n[i];
-                                if (null == t || !isFinite(c + l + m + x)) continue;
-                                const u = _.x * g.x * m,
-                                    y = _.y * g.y * x;
-                                e.save(), e.translate(c - u, l - y), e.scale(_.x * o.x, _.y * o.y), this.visuals.image.set_vectorize(e, i), e.drawImage(t, -d.x * m, -d.y * x, m, x), e.restore()
+                            for (const s of t) {
+                                const t = i[s],
+                                    l = a[s],
+                                    g = r[s],
+                                    m = n[s],
+                                    u = h[s];
+                                if (null == t || !isFinite(l + g + m + u)) continue;
+                                const x = _.x * c.x * m,
+                                    y = _.y * c.y * u;
+                                e.save(), e.translate(l - x, g - y), e.scale(_.x * o.x, _.y * o.y), this.visuals.image.set_vectorize(e, s), e.drawImage(t, -d.x * m, -d.y * u, m, u), e.restore()
                             }
                         e.restore()
                     }
                     _set_data(e) {
-                        this._set_width_height_data();
+                        const t = this.data_size;
+                        null != this._image_data && this._image_data.length == t || (this._image_data = new Array(t).fill(null), this._width = new Uint32Array(t), this._height = new Uint32Array(t));
                         const {
-                            image_dimension: t
+                            image_dimension: s
                         } = this;
-                        for (let i = 0, s = this.image.length; i < s; i++) {
-                            if (null != e && e.indexOf(i) < 0) continue;
-                            const s = this.image.get(i);
-                            (0, l.assert)(s.dimension == t, `expected a ${t}D array, not ${s.dimension}D`), this._height[i] = s.shape[0], this._width[i] = s.shape[1];
-                            const a = this._flat_img_to_buf8(s);
-                            this._set_image_data_from_buffer(i, a)
+                        for (let i = 0; i < t; i++) {
+                            if (null != e && !e.includes(i)) continue;
+                            const t = this.image.get(i);
+                            (0, g.assert)(t.dimension == s, `expected a ${s}D array, not ${t.dimension}D`);
+                            const [a, r] = t.shape;
+                            this._height[i] = a, this._width[i] = r;
+                            const n = this._flat_img_to_buf8(t);
+                            this._set_image_data_from_buffer(i, n)
                         }
                     }
                     _index_data(e) {
                         const {
                             data_size: t
                         } = this;
-                        for (let i = 0; i < t; i++) {
-                            const [t, s, a, h] = this._lrtb(i);
-                            e.add_rect(t, h, s, a)
+                        for (let s = 0; s < t; s++) {
+                            const [t, i, a, r] = this._lrtb(s);
+                            e.add_rect(t, r, i, a)
                         }
                     }
                     _lrtb(e) {
                         const t = this.dw.get(e),
-                            i = this.dh.get(e),
-                            s = this._x[e],
+                            s = this.dh.get(e),
+                            i = this._x[e],
                             a = this._y[e],
                             {
-                                xy_anchor: h
+                                xy_anchor: r
                             } = this,
-                            [r, n] = [s - h.x * t, s + (1 - h.x) * t],
-                            [_, o] = [a + h.y * i, a - (1 - h.y) * i],
-                            [d, g] = r <= n ? [r, n] : [n, r],
-                            [c, l] = _ <= o ? [_, o] : [o, _];
-                        return [d, g, l, c]
-                    }
-                    _set_width_height_data() {
-                        null != this.image_data && this.image_data.length == this.image.length || (this.image_data = new Array(this.image.length)), null != this._width && this._width.length == this.image.length || (this._width = new Uint32Array(this.image.length)), null != this._height && this._height.length == this.image.length || (this._height = new Uint32Array(this.image.length))
+                            [n, h] = [i - r.x * t, i + (1 - r.x) * t],
+                            [_, o] = [a + r.y * s, a - (1 - r.y) * s],
+                            [d, c] = n <= h ? [n, h] : [h, n],
+                            [l, g] = _ <= o ? [_, o] : [o, _];
+                        return [d, c, g, l]
                     }
                     _get_or_create_canvas(e) {
                         const t = this.image_data[e];
                         if (null != t && t.width == this._width[e] && t.height == this._height[e]) return t; {
                             const t = document.createElement("canvas");
                             return t.width = this._width[e], t.height = this._height[e], t
                         }
                     }
                     _set_image_data_from_buffer(e, t) {
-                        const i = this._get_or_create_canvas(e),
-                            s = i.getContext("2d"),
-                            a = s.getImageData(0, 0, this._width[e], this._height[e]);
-                        a.data.set(t), s.putImageData(a, 0, 0), this.image_data[e] = i
+                        const s = this._get_or_create_canvas(e),
+                            i = s.getContext("2d"),
+                            a = i.getImageData(0, 0, this._width[e], this._height[e]);
+                        a.data.set(t), i.putImageData(a, 0, 0), this.image_data[e] = s
                     }
                     _map_data() {
                         "data" == this.model.properties.dw.units ? this.sw = this.sdist(this.renderer.xscale, this._x, this.dw, "edge", this.model.dilate) : this.sw = (0, _.to_screen)(this.dw), "data" == this.model.properties.dh.units ? this.sh = this.sdist(this.renderer.yscale, this._y, this.dh, "edge", this.model.dilate) : this.sh = (0, _.to_screen)(this.dh)
                     }
-                    _image_index(e, t, i) {
-                        const [s, a, h, r] = this._lrtb(e), n = this._width[e], _ = this._height[e], o = (a - s) / n, d = (h - r) / _;
-                        let g = Math.floor((t - s) / o),
-                            c = Math.floor((i - r) / d);
-                        return this.renderer.xscale.source_range.is_reversed && (g = n - g - 1), this.renderer.yscale.source_range.is_reversed && (c = _ - c - 1), {
+                    _image_index(e, t, s) {
+                        const [i, a, r, n] = this._lrtb(e), h = this._width[e], _ = this._height[e], o = (a - i) / h, d = (r - n) / _;
+                        let c = Math.floor((t - i) / o),
+                            l = Math.floor((s - n) / d);
+                        return this.renderer.xscale.source_range.is_reversed && (c = h - c - 1), this.renderer.yscale.source_range.is_reversed && (l = _ - l - 1), {
                             index: e,
-                            i: g,
-                            j: c,
-                            flat_index: c * n + g
+                            i: c,
+                            j: l,
+                            flat_index: l * h + c
                         }
                     }
                     _hit_point(e) {
                         const {
                             sx: t,
-                            sy: i
-                        } = e, s = this.renderer.xscale.invert(t), a = this.renderer.yscale.invert(i), h = this.index.indices({
-                            x0: s,
-                            x1: s,
+                            sy: s
+                        } = e, i = this.renderer.xscale.invert(t), a = this.renderer.yscale.invert(s), r = this.index.indices({
+                            x0: i,
+                            x1: i,
                             y0: a,
                             y1: a
-                        }), r = new c.Selection, n = [];
-                        for (const e of h) t != 1 / 0 && i != 1 / 0 && (n.push(e), r.image_indices.push(this._image_index(e, s, a)));
-                        return r.indices = n, r
+                        }), n = new l.Selection, h = [];
+                        for (const e of r) t != 1 / 0 && s != 1 / 0 && (h.push(e), n.image_indices.push(this._image_index(e, i, a)));
+                        return n.indices = h, n
                     }
                 }
-                i.ImageBaseView = u, u.__name__ = "ImageBaseView";
-                class y extends n.XYGlyph {
+                s.ImageBaseView = x, x.__name__ = "ImageBaseView";
+                class y extends h.XYGlyph {
                     constructor(e) {
                         super(e)
                     }
                 }
-                i.ImageBase = y, h = y, y.__name__ = "ImageBase", h.mixins(g.ImageVector), h.define((({
+                s.ImageBase = y, r = y, y.__name__ = "ImageBase", r.mixins(c.ImageVector), r.define((({
                     Boolean: e
                 }) => ({
                     image: [d.NDArraySpec, {
                         field: "image"
                     }],
                     dw: [d.DistanceSpec, {
                         field: "dw"
@@ -29380,15 +29444,15 @@
                     connect_signals() {
                         super.connect_signals(), this.connect(this.model.color_mapper.change, (() => this._update_image()))
                     }
                     get image_dimension() {
                         return 3
                     }
                     _update_image() {
-                        null != this.image_data && (this._set_data(null), this.renderer.request_render())
+                        null != this._image_data && (this._set_data(null), this.renderer.request_render())
                     }
                     _flat_img_to_buf8(e) {
                         return this.model.color_mapper.rgba_mapper.v_compute(e)
                     }
                 }
                 t.ImageStackView = i, i.__name__ = "ImageStackView";
                 class o extends s.ImageBase {
@@ -34744,15 +34808,15 @@
                         for (const [, t] of this.renderer_views) t instanceof c.AxisView && e.push(t);
                         return e
                     }
                     update_range(e, t) {
                         this.pause(), this._range_manager.update(e, t), this.unpause()
                     }
                     reset_range() {
-                        this.update_range(null), this.trigger_ranges_update_event()
+                        this.pause(), this._range_manager.reset(), this.unpause(), this.trigger_ranges_update_event()
                     }
                     trigger_ranges_update_event() {
                         const {
                             x_range: e,
                             y_range: t
                         } = this.model, i = new Set([...e.plots, ...t.plots]);
                         for (const e of i) {
@@ -35069,28 +35133,27 @@
                         return this.parent.frame
                     }
                     update(t, n = {}) {
                         var a;
                         const {
                             x_ranges: e,
                             y_ranges: s
-                        } = this.frame;
-                        if (null == t) {
-                            for (const [, t] of e) t.reset();
-                            for (const [, t] of s) t.reset();
-                            this.update_dataranges()
-                        } else {
-                            const o = [];
-                            for (const [n, a] of e) o.push([a, t.xrs.get(n)]);
-                            for (const [n, a] of s) o.push([a, t.yrs.get(n)]);
-                            null !== (a = n.scrolling) && void 0 !== a && a && this._update_ranges_together(o), this._update_ranges_individually(o, n)
-                        }
+                        } = this.frame, o = [];
+                        for (const [n, a] of t.xrs) o.push([e.get(n), a]);
+                        for (const [n, a] of t.yrs) o.push([s.get(n), a]);
+                        null !== (a = n.scrolling) && void 0 !== a && a && this._update_ranges_together(o), this._update_ranges_individually(o, n)
                     }
                     reset() {
-                        this.update(null)
+                        const {
+                            x_ranges: t,
+                            y_ranges: n
+                        } = this.frame;
+                        for (const n of t.values()) n.reset();
+                        for (const t of n.values()) t.reset();
+                        this.update_dataranges()
                     }
                     _update_dataranges(t) {
                         const n = new Map,
                             a = new Map;
                         let e = !1;
                         for (const [, n] of t.x_ranges) n instanceof o.DataRange1d && "log" == n.scale_hint && (e = !0);
                         for (const [, n] of t.y_ranges) n instanceof o.DataRange1d && "log" == n.scale_hint && (e = !0);
@@ -35101,27 +35164,27 @@
                                 a.set(t.model, n)
                             }
                         }
                         let s = !1,
                             l = !1;
                         const i = t.x_target.span,
                             d = t.y_target.span;
-                        let u;
-                        !1 !== this.parent.model.match_aspect && 0 != i && 0 != d && (u = 1 / this.parent.model.aspect_scale * (i / d));
+                        let _;
+                        !1 !== this.parent.model.match_aspect && 0 != i && 0 != d && (_ = 1 / this.parent.model.aspect_scale * (i / d));
                         for (const [, e] of t.x_ranges) {
                             if (e instanceof o.DataRange1d) {
                                 const t = "log" == e.scale_hint ? a : n;
-                                e.update(t, 0, this.parent, u), null != e.follow && (s = !0)
+                                e.update(t, 0, this.parent, _), null != e.follow && (s = !0)
                             }
                             null != e.bounds && (l = !0)
                         }
                         for (const [, e] of t.y_ranges) {
                             if (e instanceof o.DataRange1d) {
                                 const t = "log" == e.scale_hint ? a : n;
-                                e.update(t, 1, this.parent, u), null != e.follow && (s = !0)
+                                e.update(t, 1, this.parent, _), null != e.follow && (s = !0)
                             }
                             null != e.bounds && (l = !0)
                         }
                         if (s && l) {
                             r.logger.warn("Follow enabled so bounds are unset.");
                             for (const [, n] of t.x_ranges) n.bounds = null;
                             for (const [, n] of t.y_ranges) n.bounds = null
@@ -35286,15 +35349,15 @@
                 i();
                 const a = t(18),
                     n = t(15),
                     p = t(56),
                     _ = t(105),
                     l = t(402);
                 const h = new n.Signal0({}, "gmaps_ready");
-                class d extends l.PlotView {
+                class m extends l.PlotView {
                     initialize() {
                         super.initialize(), this._tiles_loaded = !1, this.zoom_count = 0;
                         const {
                             zoom: t,
                             lat: e,
                             lng: s
                         } = this.model.map_options;
@@ -35333,15 +35396,15 @@
                     update_range(t, e) {
                         var s, i;
                         if (null == t) this.map.setCenter({
                             lat: this.initial_lat,
                             lng: this.initial_lng
                         }), this.map.setOptions({
                             zoom: this.initial_zoom
-                        }), super.update_range(null, e);
+                        }), super.reset_range();
                         else if (null != t.sdx || null != t.sdy) this.map.panBy(null !== (s = t.sdx) && void 0 !== s ? s : 0, null !== (i = t.sdy) && void 0 !== i ? i : 0), super.update_range(t, e);
                         else if (null != t.factor) {
                             if (10 !== this.zoom_count) return void(this.zoom_count += 1);
                             this.zoom_count = 0, this.pause(), super.update_range(t, e);
                             const s = t.factor < 0 ? -1 : 1,
                                 i = this.map.getZoom();
                             if (null != i) {
@@ -35446,15 +35509,15 @@
                             top: e,
                             width: s,
                             height: i
                         } = this.frame.bbox;
                         this.map_el.style.top = `${e}px`, this.map_el.style.left = `${t}px`, this.map_el.style.width = `${s}px`, this.map_el.style.height = `${i}px`
                     }
                 }
-                s.GMapPlotView = d, d.__name__ = "GMapPlotView"
+                s.GMapPlotView = m, m.__name__ = "GMapPlotView"
             },
             function _(e, a, t, s, n) {
                 var p;
                 s();
                 const _ = e(400);
                 class i extends _.GMapPlotView {
                     serializable_state() {
@@ -35908,87 +35971,87 @@
                     }
                 }
                 n.ByXPath = o, o.__name__ = "ByXPath"
             },
             function _(a, e, S, o, r) {
                 o(), r("ServerSentDataSource", a(425).ServerSentDataSource), r("AjaxDataSource", a(427).AjaxDataSource), r("ColumnDataSource", a(104).ColumnDataSource), r("ColumnarDataSource", a(99).ColumnarDataSource), r("CDSView", a(218).CDSView), r("DataSource", a(103).DataSource), r("GeoJSONDataSource", a(428).GeoJSONDataSource), r("WebDataSource", a(426).WebDataSource)
             },
-            function _(e, t, i, a, s) {
-                a();
+            function _(e, t, a, i, s) {
+                i();
                 const n = e(426);
                 class r extends n.WebDataSource {
                     constructor(e) {
                         super(e), this.initialized = !1
                     }
                     setup() {
                         if (!this.initialized) {
                             this.initialized = !0;
-                            new EventSource(this.data_url).onmessage = e => {
+                            new EventSource(this.data_url).onmessage = async e => {
                                 var t;
-                                this.load_data(JSON.parse(e.data), this.mode, null !== (t = this.max_size) && void 0 !== t ? t : void 0)
+                                await this.load_data(JSON.parse(e.data), this.mode, null !== (t = this.max_size) && void 0 !== t ? t : void 0)
                             }
                         }
                     }
                 }
-                i.ServerSentDataSource = r, r.__name__ = "ServerSentDataSource"
+                a.ServerSentDataSource = r, r.__name__ = "ServerSentDataSource"
             },
-            function _(t, e, a, n, r) {
-                var s;
+            function _(t, a, e, n, s) {
+                var r;
                 n();
                 const l = t(104),
                     i = t(19);
-                class o extends l.ColumnDataSource {
+                class c extends l.ColumnDataSource {
                     constructor(t) {
                         super(t)
                     }
                     get_column(t) {
                         return t in this.data ? this.data[t] : []
                     }
                     get_length() {
                         var t;
                         return null !== (t = super.get_length()) && void 0 !== t ? t : 0
                     }
                     initialize() {
                         super.initialize(), this.setup()
                     }
-                    load_data(t, e, a) {
+                    async load_data(t, a, e) {
                         const {
                             adapter: n
                         } = this;
-                        let r;
-                        switch (r = null != n ? n.execute(this, {
+                        let s;
+                        switch (s = null != n ? await n.execute(this, {
                                 response: t
-                            }) : t, e) {
+                            }) : t, a) {
                             case "replace":
-                                this.data = r;
+                                this.data = s;
                                 break;
                             case "append": {
                                 const t = this.data;
-                                for (const e of this.columns()) {
-                                    const n = Array.from(t[e]),
-                                        s = Array.from(r[e]),
-                                        l = n.concat(s);
-                                    r[e] = null != a ? l.slice(-a) : l
+                                for (const a of this.columns()) {
+                                    const n = Array.from(t[a]),
+                                        r = Array.from(s[a]),
+                                        l = n.concat(r);
+                                    s[a] = null != e ? l.slice(-e) : l
                                 }
-                                this.data = r;
+                                this.data = s;
                                 break
                             }
                         }
                     }
                 }
-                a.WebDataSource = o, s = o, o.__name__ = "WebDataSource", s.define((({
+                e.WebDataSource = c, r = c, c.__name__ = "WebDataSource", r.define((({
                     Any: t,
-                    Int: e,
-                    String: a,
+                    Int: a,
+                    String: e,
                     Nullable: n
                 }) => ({
-                    max_size: [n(e), null],
+                    max_size: [n(a), null],
                     mode: [i.UpdateMode, "replace"],
                     adapter: [n(t), null],
-                    data_url: [a]
+                    data_url: [e]
                 })))
             },
             function _(t, e, i, s, a) {
                 var n;
                 s();
                 const r = t(426),
                     o = t(19),
@@ -36014,18 +36077,18 @@
                     prepare_request() {
                         const t = new XMLHttpRequest;
                         t.open(this.method, this.data_url, !0), t.withCredentials = !1, t.setRequestHeader("Content-Type", this.content_type);
                         const e = this.http_headers;
                         for (const [i, s] of(0, d.entries)(e)) t.setRequestHeader(i, s);
                         return t
                     }
-                    do_load(t, e, i) {
-                        if (200 === t.status) {
+                    async do_load(t, e, i) {
+                        if (200 == t.status) {
                             const s = JSON.parse(t.responseText);
-                            this.load_data(s, e, i)
+                            await this.load_data(s, e, i)
                         }
                     }
                     do_error(t) {
                         l.logger.error(`Failed to fetch JSON from ${this.data_url} with code ${t.status}`)
                     }
                 }
                 i.AjaxDataSource = h, n = h, h.__name__ = "AjaxDataSource", n.define((({
@@ -38141,120 +38204,143 @@
                         super(o), this.tool_name = "Undo", this.tool_icon = _.tool_icon_undo
                     }
                 }
                 e.UndoTool = a, s = a, a.__name__ = "UndoTool", s.prototype.default_view = d, s.override({
                     disabled: !0
                 }), s.register_alias("undo", (() => new a))
             },
-            function _(o, n, e, i, s) {
+            function _(o, e, n, i, s) {
                 var t;
                 i();
                 const _ = o(470),
                     a = o(272);
-                class m extends _.ZoomBaseToolView {}
-                e.ZoomInToolView = m, m.__name__ = "ZoomInToolView";
+                class m extends _.ZoomBaseToolView {
+                    get factor() {
+                        return this.model.factor
+                    }
+                }
+                n.ZoomInToolView = m, m.__name__ = "ZoomInToolView";
                 class l extends _.ZoomBaseTool {
                     constructor(o) {
                         super(o), this.maintain_focus = !0, this.tool_name = "Zoom In", this.tool_icon = a.tool_icon_zoom_in
                     }
-                    get_factor() {
-                        return this.factor
-                    }
                 }
-                e.ZoomInTool = l, t = l, l.__name__ = "ZoomInTool", t.prototype.default_view = m, t.register_alias("zoom_in", (() => new l({
+                n.ZoomInTool = l, t = l, l.__name__ = "ZoomInTool", t.prototype.default_view = m, t.register_alias("zoom_in", (() => new l({
                     dimensions: "both"
                 }))), t.register_alias("xzoom_in", (() => new l({
                     dimensions: "width"
                 }))), t.register_alias("yzoom_in", (() => new l({
                     dimensions: "height"
                 })))
             },
-            function _(o, t, e, i, s) {
-                var n;
-                i();
-                const a = o(465),
-                    l = o(19),
-                    _ = o(471);
-                class m extends a.PlotActionToolView {
+            function _(e, o, t, s, n) {
+                var i;
+                s();
+                const a = e(465),
+                    r = e(200),
+                    _ = e(19),
+                    l = e(471);
+                class d extends a.PlotActionToolView {
                     doit() {
-                        var o;
-                        const t = this.plot_view.frame,
-                            e = this.model.dimensions,
-                            i = "width" == e || "both" == e,
-                            s = "height" == e || "both" == e,
-                            n = this.model.get_factor(),
-                            a = (0, _.scale_range)(t, n, i, s);
+                        var e;
+                        const {
+                            dimensions: o
+                        } = this.model, t = "width" == o || "both" == o, s = "height" == o || "both" == o, {
+                            frame: n
+                        } = this.plot_view, {
+                            x_range: i,
+                            y_range: a
+                        } = n.bbox, r = new Map(n.x_scales), _ = new Map(n.y_scales), {
+                            renderers: d
+                        } = this.model;
+                        if ("auto" != d) {
+                            const e = new Set,
+                                o = new Set;
+                            for (const t of d) e.add(t.x_range_name), o.add(t.y_range_name);
+                            for (const o of r.keys()) e.has(o) || r.delete(o);
+                            for (const e of _.keys()) o.has(e) || _.delete(e)
+                        }
+                        const c = (0, l.scale_range)(r, _, i, a, this.factor, t, s);
                         this.plot_view.state.push("zoom_out", {
-                            range: a
-                        }), this.plot_view.update_range(a, {
+                            range: c
+                        }), this.plot_view.update_range(c, {
                             scrolling: !0,
                             maintain_focus: this.model.maintain_focus
-                        }), null === (o = this.model.document) || void 0 === o || o.interactive_start(this.plot_view.model), this.plot_view.trigger_ranges_update_event()
+                        }), null === (e = this.model.document) || void 0 === e || e.interactive_start(this.plot_view.model), this.plot_view.trigger_ranges_update_event()
                     }
                 }
-                e.ZoomBaseToolView = m, m.__name__ = "ZoomBaseToolView";
-                class r extends a.PlotActionTool {
-                    constructor(o) {
-                        super(o)
+                t.ZoomBaseToolView = d, d.__name__ = "ZoomBaseToolView";
+                class c extends a.PlotActionTool {
+                    constructor(e) {
+                        super(e)
                     }
                     get tooltip() {
                         return this._get_dim_tooltip(this.dimensions)
                     }
                 }
-                e.ZoomBaseTool = r, n = r, r.__name__ = "ZoomBaseTool", n.define((({
-                    Percent: o
+                t.ZoomBaseTool = c, i = c, c.__name__ = "ZoomBaseTool", i.define((({
+                    Percent: e,
+                    Or: o,
+                    Array: t,
+                    Ref: s,
+                    Auto: n
                 }) => ({
-                    factor: [o, .1],
-                    dimensions: [l.Dimensions, "both"]
+                    factor: [e, .1],
+                    dimensions: [_.Dimensions, "both"],
+                    renderers: [o(t(s(r.DataRenderer)), n), "auto"]
                 })))
             },
-            function _(n, t, o, r, e) {
-                function s(n, t, o) {
-                    const [r, e] = [n.start, n.end], s = null != o ? o : (e + r) / 2;
-                    return [r - (r - s) * t, e - (e - s) * t]
+            function _(n, t, o, r, c) {
+                function e(n, t, o) {
+                    const [r, c] = [n.start, n.end], e = null != o ? o : (c + r) / 2;
+                    return [r - (r - e) * t, c - (c - e) * t]
                 }
 
-                function c(n, [t, o]) {
+                function s(n, [t, o]) {
                     const r = new Map;
-                    for (const [e, s] of n) {
-                        const [n, c] = s.r_invert(t, o);
-                        r.set(e, {
+                    for (const [c, e] of n) {
+                        const [n, s] = e.r_invert(t, o);
+                        r.set(c, {
                             start: n,
-                            end: c
+                            end: s
                         })
                     }
                     return r
                 }
-                r(), o.scale_highlow = s, o.get_info = c, o.scale_range = function(n, t, o = !0, r = !0, e) {
-                    const a = o ? t : 0,
-                        [l, u] = s(n.bbox.h_range, a, null != e ? e.x : void 0),
-                        i = c(n.x_scales, [l, u]),
-                        _ = r ? t : 0,
-                        [f, g] = s(n.bbox.v_range, _, null != e ? e.y : void 0);
+                r(), o.scale_highlow = e, o.get_info = s, o.scale_range = function(n, t, o, r, c, u = !0, i = !0, l) {
+                    const f = u ? c : 0,
+                        [a, _] = e(o, f, null == l ? void 0 : l.x),
+                        d = s(n, [a, _]),
+                        g = i ? c : 0,
+                        [v, h] = e(r, g, null == l ? void 0 : l.y);
                     return {
-                        xrs: i,
-                        yrs: c(n.y_scales, [f, g]),
-                        factor: t
+                        xrs: d,
+                        yrs: s(t, [v, h]),
+                        factor: c
                     }
                 }
             },
-            function _(o, t, e, i, s) {
+            function _(o, t, e, s, i) {
                 var n;
-                i();
+                s();
                 const _ = o(470),
                     a = o(272);
-                class m extends _.ZoomBaseToolView {}
+                class m extends _.ZoomBaseToolView {
+                    get factor() {
+                        const {
+                            factor: o
+                        } = this.model;
+                        return -o / (1 - o)
+                    }
+                }
                 e.ZoomOutToolView = m, m.__name__ = "ZoomOutToolView";
                 class l extends _.ZoomBaseTool {
                     constructor(o) {
                         super(o), this.tool_name = "Zoom Out", this.tool_icon = a.tool_icon_zoom_out
                     }
-                    get_factor() {
-                        return -this.factor / (1 - this.factor)
-                    }
                 }
                 e.ZoomOutTool = l, n = l, l.__name__ = "ZoomOutTool", n.prototype.default_view = m, n.define((({
                     Boolean: o
                 }) => ({
                     maintain_focus: [o, !0]
                 }))), n.register_alias("zoom_out", (() => new l({
                     dimensions: "both"
@@ -40410,87 +40496,169 @@
                     speed: [e, .001]
                 }))), o.register_alias("xwheel_pan", (() => new d({
                     dimension: "width"
                 }))), o.register_alias("ywheel_pan", (() => new d({
                     dimension: "height"
                 })))
             },
-            function _(e, o, t, s, i) {
-                var n;
-                s();
+            function _(e, s, o, t, n) {
+                var i;
+                t();
                 const l = e(274),
-                    _ = e(471),
-                    a = e(19),
-                    h = e(26),
-                    r = e(272);
-                class m extends l.GestureToolView {
+                    a = e(471),
+                    _ = e(19),
+                    c = e(26),
+                    r = e(272),
+                    m = (0, e(20).Enum)("none", "cross", "all");
+                class h extends l.GestureToolView {
                     _pinch(e) {
                         const {
-                            sx: o,
-                            sy: t,
-                            scale: s,
-                            modifiers: i
+                            sx: s,
+                            sy: o,
+                            scale: t,
+                            modifiers: n
                         } = e;
-                        let n;
-                        n = s >= 1 ? 20 * (s - 1) : -20 / s, this._scroll({
+                        let i;
+                        i = t >= 1 ? 20 * (t - 1) : -20 / t, this._scroll({
                             type: "wheel",
-                            sx: o,
-                            sy: t,
-                            delta: n,
-                            modifiers: i
+                            sx: s,
+                            sy: o,
+                            delta: i,
+                            modifiers: n
                         })
                     }
                     _scroll(e) {
-                        var o;
+                        var s;
                         const {
-                            frame: t
-                        } = this.plot_view, s = t.bbox.h_range, i = t.bbox.v_range, {
-                            sx: n,
-                            sy: l
-                        } = e, a = this.model.dimensions, h = ("width" == a || "both" == a) && s.start < n && n < s.end, r = ("height" == a || "both" == a) && i.start < l && l < i.end;
-                        if (!(h && r || this.model.zoom_on_axis)) return;
-                        const m = this.model.speed * e.delta,
-                            d = (0, _.scale_range)(t, m, h, r, {
-                                x: n,
-                                y: l
-                            });
+                            sx: o,
+                            sy: t
+                        } = e, n = this.plot_view.axis_views.find((e => e.layout.bbox.contains(o, t)));
+                        if (null != n && !this.model.zoom_on_axis) return;
+                        const {
+                            frame: i
+                        } = this.plot_view;
+                        if (null == n && !i.bbox.contains(o, t)) return;
+                        const l = this.model.dimensions,
+                            _ = "width" == l || "both" == l,
+                            c = "height" == l || "both" == l,
+                            {
+                                x_range: r,
+                                y_range: m
+                            } = i.bbox,
+                            {
+                                x_scales: h,
+                                y_scales: d,
+                                center: u
+                            } = (() => {
+                                if (null == n) {
+                                    const {
+                                        x_scales: e,
+                                        y_scales: s
+                                    } = i;
+                                    return {
+                                        x_scales: e,
+                                        y_scales: s,
+                                        center: {
+                                            x: o,
+                                            y: t
+                                        }
+                                    }
+                                } {
+                                    const e = 0 == n.dimension ? {
+                                            x: o,
+                                            y: null
+                                        } : {
+                                            x: null,
+                                            y: t
+                                        },
+                                        {
+                                            zoom_together: s
+                                        } = this.model;
+                                    if ("all" == s) {
+                                        const {
+                                            x_scales: s,
+                                            y_scales: o
+                                        } = i;
+                                        return 0 == n.dimension ? {
+                                            x_scales: s,
+                                            y_scales: new Map,
+                                            center: e
+                                        } : {
+                                            x_scales: new Map,
+                                            y_scales: o,
+                                            center: e
+                                        }
+                                    } {
+                                        const {
+                                            x_range_name: o,
+                                            y_range_name: t
+                                        } = n.model, {
+                                            x_scale: i,
+                                            y_scale: l
+                                        } = n.coordinates, a = new Map([
+                                            [o, i]
+                                        ]), _ = new Map([
+                                            [t, l]
+                                        ]);
+                                        switch (s) {
+                                            case "cross":
+                                                return {
+                                                    x_scales: a, y_scales: _, center: e
+                                                };
+                                            case "none":
+                                                return 0 == n.dimension ? {
+                                                    x_scales: a,
+                                                    y_scales: new Map,
+                                                    center: e
+                                                } : {
+                                                    x_scales: new Map,
+                                                    y_scales: _,
+                                                    center: e
+                                                }
+                                        }
+                                    }
+                                }
+                            })(),
+                            w = this.model.speed * e.delta,
+                            x = (0, a.scale_range)(h, d, r, m, w, _, c, u);
                         this.plot_view.state.push("wheel_zoom", {
-                            range: d
+                            range: x
                         });
                         const {
-                            maintain_focus: c
+                            maintain_focus: p
                         } = this.model;
-                        this.plot_view.update_range(d, {
+                        this.plot_view.update_range(x, {
                             scrolling: !0,
-                            maintain_focus: c
-                        }), null === (o = this.model.document) || void 0 === o || o.interactive_start(this.plot_view.model, (() => this.plot_view.trigger_ranges_update_event()))
+                            maintain_focus: p
+                        }), null === (s = this.model.document) || void 0 === s || s.interactive_start(this.plot_view.model, (() => this.plot_view.trigger_ranges_update_event()))
                     }
                 }
-                t.WheelZoomToolView = m, m.__name__ = "WheelZoomToolView";
+                o.WheelZoomToolView = h, h.__name__ = "WheelZoomToolView";
                 class d extends l.GestureTool {
                     constructor(e) {
-                        super(e), this.tool_name = "Wheel Zoom", this.tool_icon = r.tool_icon_wheel_zoom, this.event_type = h.is_mobile ? "pinch" : "scroll", this.default_order = 10
+                        super(e), this.tool_name = "Wheel Zoom", this.tool_icon = r.tool_icon_wheel_zoom, this.event_type = c.is_mobile ? "pinch" : "scroll", this.default_order = 10
                     }
                     get tooltip() {
                         return this._get_dim_tooltip(this.dimensions)
                     }
                 }
-                t.WheelZoomTool = d, n = d, d.__name__ = "WheelZoomTool", n.prototype.default_view = m, n.define((({
+                o.WheelZoomTool = d, i = d, d.__name__ = "WheelZoomTool", i.prototype.default_view = h, i.define((({
                     Boolean: e,
-                    Number: o
+                    Number: s
                 }) => ({
-                    dimensions: [a.Dimensions, "both"],
+                    dimensions: [_.Dimensions, "both"],
                     maintain_focus: [e, !0],
                     zoom_on_axis: [e, !0],
-                    speed: [o, 1 / 600]
-                }))), n.register_alias("wheel_zoom", (() => new d({
+                    zoom_together: [m, "all"],
+                    speed: [s, 1 / 600]
+                }))), i.register_alias("wheel_zoom", (() => new d({
                     dimensions: "both"
-                }))), n.register_alias("xwheel_zoom", (() => new d({
+                }))), i.register_alias("xwheel_zoom", (() => new d({
                     dimensions: "width"
-                }))), n.register_alias("ywheel_zoom", (() => new d({
+                }))), i.register_alias("ywheel_zoom", (() => new d({
                     dimensions: "height"
                 })))
             },
             function _(o, r, s, e, l) {
                 e(), l("CrosshairTool", o(496).CrosshairTool), l("CustomJSHover", o(497).CustomJSHover), l("HoverTool", o(498).HoverTool), l("InspectTool", o(276).InspectTool)
             },
             function _(s, e, i, t, o) {
```

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/compiler.js` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/compiler.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -178161,15 +178161,15 @@
                             print(`Compiling TypeScript (${magenta(`${files.length} files`)})`);
                             const tsoutput = (0, compiler_1.compile_files)(files, options, transformers, host);
                             if ((0, compiler_1.is_failed)(tsoutput)) {
                                 print((0, compiler_1.report_diagnostics)(tsoutput.diagnostics).text);
                                 if (options.noEmitOnError ?? false)
                                     return false;
                             }
-                            const lint_config = (0, path_1.join)(base_dir, "eslint.json");
+                            const lint_config = (0, path_1.join)(base_dir, "eslint.js");
                             if ((0, sys_1.file_exists)(lint_config)) {
                                 print("Linting sources");
                                 lint(lint_config, files);
                             }
                             const artifact = (0, path_1.basename)(base_dir);
                             const bases = [lib_dir];
                             if (is_package)
```

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/api/charts.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/api/charts.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/api/figure.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/api/figure.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/api/glyph_api.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/api/glyph_api.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/api/gridplot.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/api/gridplot.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/api/io.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/api/io.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/api/linalg.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/api/linalg.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/api/palettes.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/api/palettes.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/api/parser.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/api/parser.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/api/themes.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/api/themes.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/client/connection.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/client/connection.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/client/session.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/client/session.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/bokeh_events.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/bokeh_events.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/build_views.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/build_views.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/css.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/css.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/dom.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/dom.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/dom_view.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/dom_view.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/enums.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/enums.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/geometry.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/geometry.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/graphics.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/graphics.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/has_props.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/has_props.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/hittest.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/hittest.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/kinds.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/kinds.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/layout/alignments.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/layout/alignments.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/layout/border.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/layout/border.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/layout/grid.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/layout/grid.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/layout/layoutable.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/layout/layoutable.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/layout/side_panel.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/layout/side_panel.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/layout/types.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/layout/types.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/logging.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/logging.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/patching.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/patching.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/properties.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/properties.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/property_mixins.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/property_mixins.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/selection_manager.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/selection_manager.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/serialization/deserializer.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/serialization/deserializer.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/serialization/reps.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/serialization/reps.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/serialization/serializer.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/serialization/serializer.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/signaling.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/signaling.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/types.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/types.d.ts`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 export declare const GeneratorFunction: GeneratorFunctionConstructor;
+export declare const AsyncGeneratorFunction: AsyncGeneratorFunctionConstructor;
 export type uint8 = number;
 export type uint16 = number;
 export type uint32 = number;
 export type ByteOrder = "little" | "big";
 export type ID = string;
 export type Color = string | [name: string, alpha: number] | uint32 | [R: uint8, G: uint8, B: uint8, A?: number];
 export type ColorArray = Uint32Array;
```

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/ui_events.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/ui_events.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/uniforms.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/uniforms.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/util/affine.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/affine.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/util/algorithms.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/algorithms.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/util/array.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/array.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/util/arrayable.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/arrayable.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/util/bbox.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/bbox.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/util/bitset.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/bitset.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/util/canvas.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/canvas.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/util/cloneable.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/cloneable.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/util/color.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/color.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/util/eq.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/eq.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/util/image.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/image.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/util/iterator.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/iterator.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/util/math.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/math.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/util/matrix.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/matrix.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/util/menus.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/menus.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/util/ndarray.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/ndarray.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/util/object.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/object.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/util/pretty.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/pretty.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/util/projections.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/projections.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/util/ragged_array.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/ragged_array.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/util/random.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/random.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/util/svg.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/svg.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/util/svg_colors.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/svg_colors.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/util/templating.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/templating.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/util/text.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/text.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/util/types.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/util/types.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/vectorization.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/vectorization.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/view.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/view.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/visuals/fill.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/visuals/fill.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/visuals/hatch.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/visuals/hatch.d.ts`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     pattern(ctx: Context2d): CanvasPattern | null;
     repetition(): CanvasPatternRepetition;
 }
 export declare class HatchScalar extends VisualUniforms {
     readonly hatch_color: p.UniformScalar<uint32>;
     readonly hatch_alpha: p.UniformScalar<number>;
     readonly hatch_scale: p.UniformScalar<number>;
-    readonly hatch_pattern: p.UniformScalar<string>;
+    readonly hatch_pattern: p.UniformScalar<string | null>;
     readonly hatch_weight: p.UniformScalar<number>;
     readonly hatch_extra: p.UniformScalar<mixins.HatchExtra>;
     protected _hatch_image: p.UniformScalar<CanvasImageSource | null>;
     protected _static_doit: boolean;
     protected _compute_static_doit(): boolean;
     protected _update_iteration: number;
     update(): void;
@@ -33,15 +33,15 @@
     pattern(ctx: Context2d): CanvasPattern | null;
     repetition(): CanvasPatternRepetition;
 }
 export declare class HatchVector extends VisualUniforms {
     readonly hatch_color: p.Uniform<uint32>;
     readonly hatch_alpha: p.Uniform<number>;
     readonly hatch_scale: p.Uniform<number>;
-    readonly hatch_pattern: p.Uniform<string>;
+    readonly hatch_pattern: p.Uniform<string | null>;
     readonly hatch_weight: p.Uniform<number>;
     readonly hatch_extra: p.UniformScalar<mixins.HatchExtra>;
     protected _hatch_image: p.Uniform<CanvasImageSource | null>;
     protected _static_doit: boolean;
     protected _compute_static_doit(): boolean;
     protected _update_iteration: number;
     update(): void;
```

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/visuals/image.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/visuals/image.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/visuals/index.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/visuals/index.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/visuals/line.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/visuals/line.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/visuals/text.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/visuals/text.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/core/visuals/visual.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/core/visuals/visual.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/document/defs.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/document/defs.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/document/document.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/document/document.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/document/events.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/document/events.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/embed/index.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/embed/index.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/model.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/model.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/annotations/annotation.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/annotations/annotation.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/annotations/arrow.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/annotations/arrow.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/annotations/arrow_head.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/annotations/arrow_head.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/annotations/band.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/annotations/band.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/annotations/base_color_bar.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/annotations/base_color_bar.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/annotations/box_annotation.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/annotations/box_annotation.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/annotations/color_bar.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/annotations/color_bar.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/annotations/contour_color_bar.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/annotations/contour_color_bar.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/annotations/data_annotation.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/annotations/data_annotation.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/annotations/html/label.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/annotations/html/label.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/annotations/html/label_set.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/annotations/html/label_set.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/annotations/html/text_annotation.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/annotations/html/text_annotation.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/annotations/html/title.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/annotations/html/title.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/annotations/index.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/annotations/index.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/annotations/label.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/annotations/label.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/annotations/label_set.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/annotations/label_set.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/annotations/legend.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/annotations/legend.d.ts`

 * *Files 2% similar despite different names*

```diff
@@ -93,11 +93,10 @@
 }
 export declare class Legend extends Annotation {
     properties: Legend.Props;
     __view_type__: LegendView;
     item_change: Signal0<this>;
     constructor(attrs?: Partial<Legend.Attrs>);
     initialize(): void;
-    get_legend_names(): string[];
 }
 export {};
 //# sourceMappingURL=legend.d.ts.map
```

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/annotations/legend_item.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/annotations/legend_item.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/annotations/poly_annotation.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/annotations/poly_annotation.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/annotations/slope.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/annotations/slope.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/annotations/span.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/annotations/span.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/annotations/text_annotation.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/annotations/text_annotation.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/annotations/title.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/annotations/title.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/annotations/toolbar_panel.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/annotations/toolbar_panel.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/annotations/upper_lower.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/annotations/upper_lower.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/annotations/whisker.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/annotations/whisker.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/axes/axis.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/axes/axis.d.ts`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 import type { Panel, Orient } from "../../core/layout/side_panel";
 import type { Context2d } from "../../core/util/canvas";
 import { GraphicsBoxes } from "../../core/graphics";
 import type { Factor } from "../ranges/factor_range";
 import type { BaseTextView } from "../text/base_text";
 import { BaseText } from "../text/base_text";
 import type { IterViews } from "../../core/build_views";
+import type { BBox } from "../../core/util/bbox";
 export type Extents = {
     tick: number;
     tick_labels: number[];
     tick_label: number;
     axis_label: number;
 };
 export type Coords = [number[], number[]];
@@ -29,14 +30,15 @@
     minor: Coords;
 }
 export declare class AxisView extends GuideRendererView {
     model: Axis;
     visuals: Axis.Visuals;
     panel: Panel;
     layout: Layoutable;
+    get bbox(): BBox;
     _axis_label_view: BaseTextView | null;
     _major_label_views: Map<string | number, BaseTextView>;
     children(): IterViews;
     lazy_initialize(): Promise<void>;
     protected _init_axis_label(): Promise<void>;
     protected _init_major_labels(): Promise<void>;
     update_layout(): void;
```

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/axes/categorical_axis.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/axes/categorical_axis.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/axes/continuous_axis.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/axes/continuous_axis.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/axes/datetime_axis.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/axes/datetime_axis.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/axes/linear_axis.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/axes/linear_axis.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/axes/log_axis.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/axes/log_axis.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/axes/mercator_axis.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/axes/mercator_axis.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/callbacks/callback.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/callbacks/callback.d.ts`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import { Model } from "../../model";
 import type * as p from "../../core/properties";
 export type CallbackFn<Obj, Args extends any[], Ret = void> = (obj: Obj, ...args: Args) => Ret;
 export type CallbackLike<Obj, Args extends any[], Ret = void> = {
-    execute: CallbackFn<Obj, Args, Ret>;
+    execute: CallbackFn<Obj, Args, Ret> | CallbackFn<Obj, Args, Promise<Ret>>;
 };
 export type CallbackLike0<Obj, Ret = void> = CallbackLike<Obj, [], Ret>;
 export type CallbackLike1<Obj, Arg, Ret = void> = CallbackLike<Obj, [Arg], Ret>;
 export declare namespace Callback {
     type Attrs = p.AttrsOf<Props>;
     type Props = Model.Props;
 }
 export interface Callback extends Callback.Attrs {
 }
-export declare abstract class Callback extends Model implements CallbackLike<unknown, any> {
+export declare abstract class Callback extends Model implements CallbackLike<unknown, any, unknown> {
     properties: Callback.Props;
     constructor(attrs?: Partial<Callback.Attrs>);
     abstract execute(cb_obj: unknown, cb_data?: {
         [key: string]: unknown;
-    }): unknown;
+    }): unknown | Promise<unknown>;
 }
 //# sourceMappingURL=callback.d.ts.map
```

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/callbacks/customjs.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/expressions/customjs_expr.d.ts`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,25 @@
-import { Callback } from "./callback";
+import { Expression } from "./expression";
+import type { ColumnarDataSource } from "../sources/columnar_data_source";
 import type * as p from "../../core/properties";
-export declare namespace CustomJS {
+import type { Arrayable } from "../../core/types";
+export declare namespace CustomJSExpr {
     type Attrs = p.AttrsOf<Props>;
-    type Props = Callback.Props & {
+    type Props = Expression.Props & {
         args: p.Property<{
             [key: string]: unknown;
         }>;
         code: p.Property<string>;
     };
 }
-export interface CustomJS extends CustomJS.Attrs {
+export interface CustomJSExpr extends CustomJSExpr.Attrs {
 }
-export declare class CustomJS extends Callback {
-    properties: CustomJS.Props;
-    constructor(attrs?: Partial<CustomJS.Attrs>);
+export declare class CustomJSExpr extends Expression {
+    properties: CustomJSExpr.Props;
+    constructor(attrs?: Partial<CustomJSExpr.Attrs>);
+    connect_signals(): void;
     get names(): string[];
-    get values(): any[];
-    get func(): Function;
-    execute(cb_obj: unknown, cb_data?: {
-        [key: string]: unknown;
-    }): unknown;
+    get values(): unknown[];
+    get func(): GeneratorFunction;
+    protected _v_compute(source: ColumnarDataSource): Arrayable<unknown>;
 }
-//# sourceMappingURL=customjs.d.ts.map
+//# sourceMappingURL=customjs_expr.d.ts.map
```

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/callbacks/open_url.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/callbacks/open_url.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/callbacks/set_value.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/callbacks/set_value.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/canvas/canvas.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/canvas/canvas.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/canvas/cartesian_frame.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/canvas/cartesian_frame.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/common/kinds.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/common/kinds.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/common/resolve.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/common/resolve.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/coordinates/coordinate_mapping.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/coordinates/coordinate_mapping.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/dom/action.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/dom/action.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/dom/color_ref.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/dom/color_ref.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/dom/dom_element.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/dom/dom_element.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/dom/dom_node.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/dom/dom_node.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/dom/elements.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/dom/elements.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/dom/html.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/dom/html.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/dom/index.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/dom/index.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/dom/index_.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/dom/index_.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/dom/placeholder.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/dom/placeholder.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/dom/styles.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/dom/styles.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/dom/stylesheets.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/dom/stylesheets.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/dom/template.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/dom/template.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/dom/text.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/dom/text.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/dom/toggle_group.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/dom/toggle_group.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/dom/value_of.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/dom/value_of.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/dom/value_ref.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/dom/value_ref.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/expressions/coordinate_transform.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/expressions/coordinate_transform.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/expressions/cumsum.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/expressions/cumsum.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/expressions/customjs_expr.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/markup.d.ts`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,30 @@
-import { Expression } from "./expression";
-import type { ColumnarDataSource } from "../sources/columnar_data_source";
+import type { StyleSheetLike } from "../../core/dom";
 import type * as p from "../../core/properties";
-import type { Arrayable } from "../../core/types";
-export declare namespace CustomJSExpr {
+import { Widget, WidgetView } from "./widget";
+export declare abstract class MarkupView extends WidgetView {
+    model: Markup;
+    protected markup_el: HTMLElement;
+    protected readonly _auto_width = "fit-content";
+    protected readonly _auto_height = "auto";
+    lazy_initialize(): Promise<void>;
+    has_math_disabled(): boolean;
+    protected rerender(): void;
+    connect_signals(): void;
+    stylesheets(): StyleSheetLike[];
+    render(): void;
+}
+export declare namespace Markup {
     type Attrs = p.AttrsOf<Props>;
-    type Props = Expression.Props & {
-        args: p.Property<{
-            [key: string]: unknown;
-        }>;
-        code: p.Property<string>;
+    type Props = Widget.Props & {
+        text: p.Property<string>;
+        disable_math: p.Property<boolean>;
     };
 }
-export interface CustomJSExpr extends CustomJSExpr.Attrs {
+export interface Markup extends Markup.Attrs {
 }
-export declare class CustomJSExpr extends Expression {
-    properties: CustomJSExpr.Props;
-    constructor(attrs?: Partial<CustomJSExpr.Attrs>);
-    connect_signals(): void;
-    get names(): string[];
-    get values(): unknown[];
-    get func(): GeneratorFunction;
-    protected _v_compute(source: ColumnarDataSource): Arrayable<unknown>;
+export declare abstract class Markup extends Widget {
+    properties: Markup.Props;
+    __view_type__: MarkupView;
+    constructor(attrs?: Partial<Markup.Attrs>);
 }
-//# sourceMappingURL=customjs_expr.d.ts.map
+//# sourceMappingURL=markup.d.ts.map
```

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/expressions/expression.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/expressions/expression.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/expressions/maximum.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/expressions/maximum.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/expressions/minimum.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/expressions/minimum.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/expressions/polar.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/expressions/polar.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/expressions/stack.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/expressions/stack.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/filters/all_indices.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/filters/all_indices.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/filters/boolean_filter.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/filters/boolean_filter.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/filters/customjs_filter.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/filters/customjs_filter.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/filters/difference_filter.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/filters/difference_filter.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/filters/filter.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/filters/filter.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/filters/group_filter.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/filters/group_filter.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/filters/index.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/filters/index.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/filters/index_filter.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/filters/index_filter.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/filters/intersection_filter.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/filters/intersection_filter.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/filters/inversion_filter.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/filters/inversion_filter.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/filters/symmetric_difference_filter.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/filters/symmetric_difference_filter.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/filters/union_filter.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/filters/union_filter.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/formatters/basic_tick_formatter.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/formatters/basic_tick_formatter.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/formatters/categorical_tick_formatter.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/formatters/categorical_tick_formatter.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/formatters/customjs_tick_formatter.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/formatters/customjs_tick_formatter.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/formatters/datetime_tick_formatter.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/formatters/datetime_tick_formatter.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/formatters/index.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/formatters/index.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/formatters/log_tick_formatter.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/formatters/log_tick_formatter.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/formatters/mercator_tick_formatter.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/formatters/mercator_tick_formatter.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/formatters/numeral_tick_formatter.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/formatters/numeral_tick_formatter.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/formatters/printf_tick_formatter.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/formatters/printf_tick_formatter.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/formatters/tick_formatter.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/formatters/tick_formatter.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/annular_wedge.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/annular_wedge.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/annulus.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/annulus.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/arc.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/arc.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/area.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/area.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/bezier.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/bezier.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/block.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/block.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/center_rotatable.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/center_rotatable.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/circle.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/circle.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/ellipse.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/ellipse.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/glyph.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/glyph.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/harea.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/harea.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/harea_step.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/harea_step.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/hbar.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/hbar.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/hex_tile.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/hex_tile.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/hspan.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/hspan.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/hstrip.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/hstrip.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/image.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/image.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/image_base.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/image_base.d.ts`

 * *Files 4% similar despite different names*

```diff
@@ -9,41 +9,43 @@
 import type { ImageIndex } from "../selections/selection";
 import { Selection } from "../selections/selection";
 import type { PointGeometry } from "../../core/geometry";
 import type { SpatialIndex } from "../../core/util/spatial";
 import type { NDArrayType } from "../../core/util/ndarray";
 import type { XY } from "../../core/util/bbox";
 import { Anchor } from "../common/kinds";
+type ImageData = HTMLCanvasElement | null;
 export type ImageDataBase = XYGlyphData & {
-    image_data: HTMLCanvasElement[];
+    readonly image_data: ImageData[];
     readonly image: p.Uniform<NDArrayType<number>>;
     readonly dw: p.Uniform<number>;
     readonly dh: p.Uniform<number>;
     sw: ScreenArray;
     sh: ScreenArray;
 };
 export interface ImageBaseView extends ImageDataBase {
 }
 export declare abstract class ImageBaseView extends XYGlyphView {
     model: ImageBase;
     visuals: ImageBase.Visuals;
+    protected _image_data: ImageData[] | null;
+    get image_data(): ImageData[];
     protected _width: Uint32Array;
     protected _height: Uint32Array;
     connect_signals(): void;
     get image_dimension(): number;
     get xy_scale(): XY<number>;
     get xy_offset(): XY<number>;
     get xy_anchor(): XY<number>;
     get xy_sign(): XY<number>;
     protected _render(ctx: Context2d, indices: number[], data?: ImageDataBase): void;
     protected abstract _flat_img_to_buf8(img: NDArrayType<number>): Uint8ClampedArray;
     protected _set_data(indices: number[] | null): void;
     protected _index_data(index: SpatialIndex): void;
     _lrtb(i: number): [number, number, number, number];
-    protected _set_width_height_data(): void;
     protected _get_or_create_canvas(i: number): HTMLCanvasElement;
     protected _set_image_data_from_buffer(i: number, buf8: Uint8ClampedArray): void;
     protected _map_data(): void;
     _image_index(index: number, x: number, y: number): ImageIndex;
     _hit_point(geometry: PointGeometry): Selection;
 }
 export declare namespace ImageBase {
@@ -64,8 +66,9 @@
 export interface ImageBase extends ImageBase.Attrs {
 }
 export declare abstract class ImageBase extends XYGlyph {
     properties: ImageBase.Props;
     __view_type__: ImageBaseView;
     constructor(attrs?: Partial<ImageBase.Attrs>);
 }
+export {};
 //# sourceMappingURL=image_base.d.ts.map
```

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/image_rgba.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/image_rgba.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/image_stack.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/image_stack.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/image_url.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/image_url.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/index.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/index.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/line.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/line.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/lrtb.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/lrtb.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/marker.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/marker.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/multi_line.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/multi_line.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/multi_polygons.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/multi_polygons.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/patch.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/patch.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/patches.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/patches.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/quad.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/quad.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/quadratic.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/quadratic.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/ray.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/ray.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/rect.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/rect.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/scatter.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/scatter.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/segment.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/segment.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/spline.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/spline.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/step.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/step.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/text.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/text.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/utils.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/utils.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/varea.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/varea.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/varea_step.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/varea_step.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/vbar.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/vbar.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/vspan.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/vspan.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/vstrip.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/vstrip.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/webgl/annular_wedge.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/webgl/annular_wedge.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/webgl/annulus.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/webgl/annulus.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/webgl/base.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/webgl/base.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/webgl/base_line.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/webgl/base_line.d.ts`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     readonly glyph: GlyphView;
     protected _points?: Float32Buffer;
     protected _show?: Uint8Buffer;
     private _antialias;
     private _miter_limit;
     protected _color: number[];
     protected _linewidth: number;
-    protected _line_dash: number[];
+    protected _line_dash: number[] | null;
     protected _is_closed: boolean;
     protected _length_so_far?: Float32Buffer;
     protected _dash_tex?: Texture2D;
     protected _dash_tex_info?: number[];
     protected _dash_scale?: number;
     protected _dash_offset?: number;
     constructor(regl_wrapper: ReglWrapper, glyph: GlyphView);
```

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/webgl/base_marker.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/webgl/base_marker.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/webgl/buffer.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/webgl/buffer.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/webgl/circle.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/webgl/circle.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/webgl/dash_cache.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/webgl/dash_cache.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/webgl/line_gl.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/webgl/line_gl.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/webgl/lrtb.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/webgl/lrtb.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/webgl/multi_marker.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/webgl/multi_marker.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/webgl/regl_wrap.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/webgl/regl_wrap.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/webgl/single_marker.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/webgl/single_marker.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/webgl/step.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/webgl/step.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/webgl/sxsy.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/webgl/sxsy.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/webgl/types.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/webgl/types.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/webgl/webgl_utils.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/webgl/webgl_utils.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/webgl/wedge.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/webgl/wedge.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/wedge.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/wedge.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/glyphs/xy_glyph.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/glyphs/xy_glyph.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/graphics/decoration.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/graphics/decoration.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/graphics/marking.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/graphics/marking.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/graphs/graph_hit_test_policy.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/graphs/graph_hit_test_policy.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/graphs/layout_provider.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/graphs/layout_provider.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/graphs/static_layout_provider.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/graphs/static_layout_provider.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/grids/grid.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/grids/grid.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/index.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/index.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/layouts/alignments.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/layouts/alignments.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/layouts/column.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/layouts/column.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/layouts/css_grid_box.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/layouts/css_grid_box.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/layouts/flex_box.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/layouts/flex_box.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/layouts/grid_box.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/layouts/grid_box.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/layouts/group_box.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/layouts/group_box.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/layouts/hbox.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/layouts/hbox.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/layouts/layout_dom.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/layouts/layout_dom.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/layouts/row.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/layouts/row.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/layouts/scroll_box.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/layouts/scroll_box.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/layouts/spacer.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/layouts/spacer.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/layouts/tab_panel.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/layouts/tab_panel.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/layouts/tabs.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/layouts/tabs.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/layouts/vbox.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/layouts/vbox.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/mappers/categorical_color_mapper.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/mappers/categorical_color_mapper.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/mappers/categorical_mapper.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/mappers/categorical_mapper.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/mappers/categorical_marker_mapper.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/mappers/categorical_marker_mapper.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/mappers/categorical_pattern_mapper.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/mappers/categorical_pattern_mapper.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/mappers/color_mapper.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/mappers/color_mapper.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/mappers/continuous_color_mapper.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/mappers/continuous_color_mapper.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/mappers/eqhist_color_mapper.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/mappers/eqhist_color_mapper.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/mappers/index.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/mappers/index.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/mappers/linear_color_mapper.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/mappers/linear_color_mapper.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/mappers/log_color_mapper.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/mappers/log_color_mapper.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/mappers/mapper.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/mappers/mapper.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/mappers/scanning_color_mapper.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/mappers/scanning_color_mapper.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/mappers/weighted_stack_color_mapper.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/mappers/weighted_stack_color_mapper.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/menus/action.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/menus/action.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/menus/check_action.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/menus/check_action.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/menus/divider.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/menus/divider.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/menus/menu.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/menus/menu.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/menus/menu_item.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/menus/menu_item.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/menus/section.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/menus/section.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/plots/figure.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/plots/figure.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/plots/gmap.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/plots/gmap.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/plots/gmap_plot.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/plots/gmap_plot.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/plots/gmap_plot_canvas.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/plots/gmap_plot_canvas.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/plots/grid_plot.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/plots/grid_plot.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/plots/plot.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/plots/plot.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/plots/plot_canvas.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/plots/plot_canvas.d.ts`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
     initialize(): void;
     lazy_initialize(): Promise<void>;
     box_sizing(): DOMBoxSizing;
     protected _intrinsic_display(): FullDisplay;
     _update_layout(): void;
     protected _measure_layout(): void;
     get axis_views(): AxisView[];
-    update_range(range_info: RangeInfo | null, options?: RangeOptions): void;
+    update_range(range_info: RangeInfo, options?: RangeOptions): void;
     reset_range(): void;
     trigger_ranges_update_event(): void;
     get_selection(): Map<DataRenderer, Selection>;
     update_selection(selections: Map<DataRenderer, Selection> | null): void;
     reset_selection(): void;
     protected _invalidate_layout_if_needed(): void;
     get_renderer_views(): RendererView[];
```

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/plots/range_manager.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/plots/range_manager.d.ts`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     maintain_focus?: boolean;
 };
 export declare class RangeManager {
     readonly parent: PlotView;
     constructor(parent: PlotView);
     get frame(): CartesianFrame;
     invalidate_dataranges: boolean;
-    update(range_info: RangeInfo | null, options?: RangeOptions): void;
+    update(range_info: RangeInfo, options?: RangeOptions): void;
     reset(): void;
     protected _update_dataranges(frame: CartesianFrame | CoordinateMapping): void;
     update_dataranges(): void;
     compute_initial(): RangeInfo | null;
     protected _update_ranges_together(range_info_iter: [Range, Interval][]): void;
     protected _update_ranges_individually(range_info_iter: [Range, Interval][], options?: RangeOptions): void;
     protected _get_weight_to_constrain_interval(rng: Range, range_info: Interval): number;
```

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/plots/state_manager.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/plots/state_manager.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/policies/labeling.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/policies/labeling.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/random/park_miller_lcg.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/random/park_miller_lcg.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/random/random_generator.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/random/random_generator.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/ranges/data_range.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/ranges/data_range.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/ranges/data_range1d.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/ranges/data_range1d.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/ranges/factor_range.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/ranges/factor_range.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/ranges/range.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/ranges/range.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/ranges/range1d.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/ranges/range1d.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/renderers/contour_renderer.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/renderers/contour_renderer.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/renderers/data_renderer.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/renderers/data_renderer.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/renderers/glyph_renderer.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/renderers/glyph_renderer.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/renderers/graph_renderer.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/renderers/graph_renderer.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/renderers/guide_renderer.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/renderers/guide_renderer.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/renderers/renderer.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/renderers/renderer.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/scales/categorical_scale.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/scales/categorical_scale.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/scales/linear_interpolation_scale.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/scales/linear_interpolation_scale.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/scales/linear_scale.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/scales/linear_scale.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/scales/log_scale.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/scales/log_scale.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/scales/scale.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/scales/scale.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/selections/interaction_policy.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/selections/interaction_policy.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/selections/selection.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/selections/selection.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/selectors/selector.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/selectors/selector.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/sources/ajax_data_source.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/sources/ajax_data_source.d.ts`

 * *Files 8% similar despite different names*

```diff
@@ -21,11 +21,11 @@
     constructor(attrs?: Partial<AjaxDataSource.Attrs>);
     protected interval: number | null;
     protected initialized: boolean;
     destroy(): void;
     setup(): void;
     get_data(mode: UpdateMode, max_size?: number | null, _if_modified?: boolean): void;
     prepare_request(): XMLHttpRequest;
-    do_load(xhr: XMLHttpRequest, mode: UpdateMode, max_size?: number): void;
+    do_load(xhr: XMLHttpRequest, mode: UpdateMode, max_size?: number): Promise<void>;
     do_error(xhr: XMLHttpRequest): void;
 }
 //# sourceMappingURL=ajax_data_source.d.ts.map
```

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/sources/cds_view.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/sources/cds_view.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/sources/column_data_source.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/sources/column_data_source.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/sources/columnar_data_source.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/sources/columnar_data_source.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/sources/data_source.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/sources/data_source.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/sources/geojson_data_source.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/sources/geojson_data_source.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/sources/server_sent_data_source.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/sources/server_sent_data_source.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/sources/web_data_source.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/sources/web_data_source.d.ts`

 * *Files 20% similar despite different names*

```diff
@@ -20,10 +20,10 @@
 export declare abstract class WebDataSource extends ColumnDataSource {
     properties: WebDataSource.Props;
     constructor(attrs?: Partial<WebDataSource.Attrs>);
     get_column(name: string): Arrayable;
     get_length(): number;
     abstract setup(): void;
     initialize(): void;
-    load_data(raw_data: any, mode: UpdateMode, max_size?: number): void;
+    load_data(raw_data: any, mode: UpdateMode, max_size?: number): Promise<void>;
 }
 //# sourceMappingURL=web_data_source.d.ts.map
```

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/text/base_text.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/text/base_text.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/text/math_text.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/text/math_text.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/text/plain_text.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/text/plain_text.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/text/providers.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/text/providers.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/textures/canvas_texture.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/textures/canvas_texture.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/textures/image_url_texture.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/textures/image_url_texture.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/textures/texture.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/textures/texture.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tickers/adaptive_ticker.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tickers/adaptive_ticker.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tickers/binned_ticker.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tickers/binned_ticker.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tickers/categorical_ticker.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tickers/categorical_ticker.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tickers/composite_ticker.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tickers/composite_ticker.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tickers/continuous_ticker.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tickers/continuous_ticker.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tickers/days_ticker.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tickers/days_ticker.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tickers/fixed_ticker.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tickers/fixed_ticker.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tickers/index.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tickers/index.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tickers/log_ticker.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tickers/log_ticker.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tickers/mercator_ticker.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tickers/mercator_ticker.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tickers/months_ticker.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tickers/months_ticker.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tickers/single_interval_ticker.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tickers/single_interval_ticker.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tickers/ticker.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tickers/ticker.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tickers/years_ticker.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tickers/years_ticker.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tiles/bbox_tile_source.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tiles/bbox_tile_source.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tiles/mercator_tile_source.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tiles/mercator_tile_source.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tiles/quadkey_tile_source.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tiles/quadkey_tile_source.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tiles/tile_renderer.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tiles/tile_renderer.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tiles/tile_source.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tiles/tile_source.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tiles/tms_tile_source.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tiles/tms_tile_source.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tiles/wmts_tile_source.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tiles/wmts_tile_source.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tools/actions/action_tool.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/actions/action_tool.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tools/actions/copy_tool.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/actions/copy_tool.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tools/actions/custom_action.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/actions/custom_action.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tools/actions/examine_tool.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/actions/examine_tool.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tools/actions/fullscreen_tool.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/actions/fullscreen_tool.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tools/actions/help_tool.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/actions/help_tool.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tools/actions/index.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/actions/index.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tools/actions/plot_action_tool.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/actions/plot_action_tool.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tools/actions/redo_tool.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/actions/redo_tool.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tools/actions/reset_tool.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/actions/reset_tool.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tools/actions/save_tool.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/actions/save_tool.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tools/actions/undo_tool.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/actions/undo_tool.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tools/actions/zoom_base_tool.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/actions/zoom_out_tool.d.ts`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,23 @@
-import { PlotActionTool, PlotActionToolView } from "./plot_action_tool";
-import { Dimensions } from "../../../core/enums";
+import { ZoomBaseTool, ZoomBaseToolView } from "./zoom_base_tool";
 import type * as p from "../../../core/properties";
-export declare abstract class ZoomBaseToolView extends PlotActionToolView {
+export declare class ZoomOutToolView extends ZoomBaseToolView {
     model: ZoomBaseTool;
-    doit(): void;
+    get factor(): number;
 }
-export declare namespace ZoomBaseTool {
+export declare namespace ZoomOutTool {
     type Attrs = p.AttrsOf<Props>;
-    type Props = PlotActionTool.Props & {
-        factor: p.Property<number>;
-        dimensions: p.Property<Dimensions>;
+    type Props = ZoomBaseTool.Props & {
+        maintain_focus: p.Property<boolean>;
     };
 }
-export interface ZoomBaseTool extends ZoomBaseTool.Attrs {
+export interface ZoomOutTool extends ZoomBaseTool.Attrs {
 }
-export declare abstract class ZoomBaseTool extends PlotActionTool {
-    properties: ZoomBaseTool.Props;
+export declare class ZoomOutTool extends ZoomBaseTool {
+    properties: ZoomOutTool.Props;
     __view_type__: ZoomBaseToolView;
+    maintain_focus: boolean;
     constructor(attrs?: Partial<ZoomBaseTool.Attrs>);
-    get tooltip(): string;
-    abstract readonly maintain_focus: boolean;
-    abstract get_factor(): number;
+    tool_name: string;
+    tool_icon: string;
 }
-//# sourceMappingURL=zoom_base_tool.d.ts.map
+//# sourceMappingURL=zoom_out_tool.d.ts.map
```

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tools/actions/zoom_in_tool.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/actions/zoom_in_tool.d.ts`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import { ZoomBaseTool, ZoomBaseToolView } from "./zoom_base_tool";
 export declare class ZoomInToolView extends ZoomBaseToolView {
     model: ZoomBaseTool;
+    get factor(): number;
 }
 export interface ZoomInTool extends ZoomBaseTool.Attrs {
 }
 export declare class ZoomInTool extends ZoomBaseTool {
     properties: ZoomBaseTool.Props;
     __view_type__: ZoomBaseToolView;
     readonly maintain_focus: boolean;
     constructor(attrs?: Partial<ZoomBaseTool.Attrs>);
-    get_factor(): number;
     tool_name: string;
     tool_icon: string;
 }
 //# sourceMappingURL=zoom_in_tool.d.ts.map
```

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tools/click_button.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/click_button.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tools/edit/box_edit_tool.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/edit/box_edit_tool.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tools/edit/edit_tool.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/edit/edit_tool.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tools/edit/freehand_draw_tool.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/edit/freehand_draw_tool.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tools/edit/line_edit_tool.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/edit/line_edit_tool.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tools/edit/line_tool.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/edit/line_tool.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tools/edit/point_draw_tool.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/edit/point_draw_tool.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tools/edit/poly_draw_tool.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/edit/poly_draw_tool.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tools/edit/poly_edit_tool.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/edit/poly_edit_tool.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tools/edit/poly_tool.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/edit/poly_tool.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tools/gestures/box_select_tool.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/gestures/box_select_tool.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tools/gestures/box_zoom_tool.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/gestures/box_zoom_tool.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tools/gestures/gesture_tool.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/gestures/gesture_tool.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tools/gestures/index.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/gestures/index.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tools/gestures/lasso_select_tool.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/gestures/lasso_select_tool.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tools/gestures/pan_tool.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/gestures/pan_tool.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tools/gestures/poly_select_tool.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/gestures/poly_select_tool.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tools/gestures/range_tool.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/gestures/range_tool.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tools/gestures/region_select_tool.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/gestures/region_select_tool.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tools/gestures/select_tool.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/gestures/select_tool.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tools/gestures/tap_tool.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/gestures/tap_tool.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tools/gestures/wheel_pan_tool.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/gestures/wheel_pan_tool.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tools/gestures/wheel_zoom_tool.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/gestures/wheel_zoom_tool.d.ts`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 import { GestureTool, GestureToolView } from "./gesture_tool";
 import type * as p from "../../../core/properties";
 import type { PinchEvent, ScrollEvent } from "../../../core/ui_events";
 import { Dimensions } from "../../../core/enums";
+declare const ZoomTogether: import("core/kinds").Kinds.Enum<"none" | "all" | "cross">;
+type ZoomTogether = typeof ZoomTogether["__type__"];
 export declare class WheelZoomToolView extends GestureToolView {
     model: WheelZoomTool;
     _pinch(ev: PinchEvent): void;
     _scroll(ev: ScrollEvent): void;
 }
 export declare namespace WheelZoomTool {
     type Attrs = p.AttrsOf<Props>;
     type Props = GestureTool.Props & {
         dimensions: p.Property<Dimensions>;
         maintain_focus: p.Property<boolean>;
         zoom_on_axis: p.Property<boolean>;
+        zoom_together: p.Property<ZoomTogether>;
         speed: p.Property<number>;
     };
 }
 export interface WheelZoomTool extends WheelZoomTool.Attrs {
 }
 export declare class WheelZoomTool extends GestureTool {
     properties: WheelZoomTool.Props;
@@ -24,8 +27,9 @@
     constructor(attrs?: Partial<WheelZoomTool.Attrs>);
     tool_name: string;
     tool_icon: string;
     event_type: "pinch" | "scroll";
     default_order: number;
     get tooltip(): string;
 }
+export {};
 //# sourceMappingURL=wheel_zoom_tool.d.ts.map
```

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tools/inspectors/crosshair_tool.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/inspectors/crosshair_tool.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tools/inspectors/customjs_hover.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/inspectors/customjs_hover.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tools/inspectors/hover_tool.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/inspectors/hover_tool.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tools/inspectors/inspect_tool.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/inspectors/inspect_tool.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tools/on_off_button.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/on_off_button.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tools/tool.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/tool.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tools/tool_button.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/tool_button.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tools/tool_proxy.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/tool_proxy.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/tools/toolbar.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/tools/toolbar.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/transforms/customjs_transform.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/transforms/customjs_transform.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/transforms/interpolator.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/transforms/interpolator.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/transforms/jitter.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/transforms/jitter.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/transforms/linear_interpolator.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/transforms/linear_interpolator.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/transforms/range_transform.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/transforms/range_transform.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/transforms/step_interpolator.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/transforms/step_interpolator.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/transforms/transform.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/transforms/transform.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/ui/dialog.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/ui/dialog.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/ui/examiner.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/ui/examiner.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/ui/icons/builtin_icon.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/ui/icons/builtin_icon.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/ui/icons/icon.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/ui/icons/icon.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/ui/icons/svg_icon.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/ui/icons/svg_icon.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/ui/icons/tabler_icon.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/ui/icons/tabler_icon.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/ui/pane.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/ui/pane.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/ui/tooltip.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/ui/tooltip.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/ui/ui_element.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/ui/ui_element.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/abstract_button.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/abstract_button.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/abstract_slider.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/abstract_slider.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/autocomplete_input.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/autocomplete_input.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/base_date_picker.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/base_date_picker.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/base_datetime_picker.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/base_datetime_picker.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/button.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/button.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/checkbox.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/checkbox.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/checkbox_button_group.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/checkbox_button_group.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/checkbox_group.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/checkbox_group.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/color_picker.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/color_picker.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/control.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/control.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/date_picker.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/date_picker.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/date_range_picker.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/date_range_picker.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/date_range_slider.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/date_range_slider.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/date_slider.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/date_slider.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/datetime_picker.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/datetime_picker.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/datetime_range_picker.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/datetime_range_picker.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/datetime_range_slider.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/datetime_range_slider.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/div.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/div.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/dropdown.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/dropdown.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/file_input.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/file_input.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/help_button.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/help_button.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/index.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/index.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/input_widget.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/input_widget.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/markup.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/toggle_button_group.d.ts`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,31 @@
+import { OrientedControl, OrientedControlView } from "./oriented_control";
+import { ButtonType } from "../../core/enums";
 import type { StyleSheetLike } from "../../core/dom";
 import type * as p from "../../core/properties";
-import { Widget, WidgetView } from "./widget";
-export declare abstract class MarkupView extends WidgetView {
-    model: Markup;
-    protected markup_el: HTMLElement;
-    protected readonly _auto_width = "fit-content";
-    protected readonly _auto_height = "auto";
-    lazy_initialize(): Promise<void>;
-    has_math_disabled(): boolean;
-    protected rerender(): void;
+export declare abstract class ToggleButtonGroupView extends OrientedControlView {
+    model: ToggleButtonGroup;
+    protected _buttons: HTMLElement[];
+    controls(): Generator<any, void, any>;
     connect_signals(): void;
     stylesheets(): StyleSheetLike[];
     render(): void;
+    abstract change_active(i: number): void;
+    protected abstract _update_active(): void;
 }
-export declare namespace Markup {
+export declare namespace ToggleButtonGroup {
     type Attrs = p.AttrsOf<Props>;
-    type Props = Widget.Props & {
-        text: p.Property<string>;
-        disable_math: p.Property<boolean>;
+    type Props = OrientedControl.Props & {
+        labels: p.Property<string[]>;
+        button_type: p.Property<ButtonType>;
     };
 }
-export interface Markup extends Markup.Attrs {
+export interface ToggleButtonGroup extends ToggleButtonGroup.Attrs {
 }
-export declare abstract class Markup extends Widget {
-    properties: Markup.Props;
-    __view_type__: MarkupView;
-    constructor(attrs?: Partial<Markup.Attrs>);
+export declare abstract class ToggleButtonGroup extends OrientedControl {
+    properties: ToggleButtonGroup.Props & {
+        active: p.Property<unknown>;
+    };
+    __view_type__: ToggleButtonGroupView;
+    constructor(attrs?: Partial<ToggleButtonGroup.Attrs>);
 }
-//# sourceMappingURL=markup.d.ts.map
+//# sourceMappingURL=toggle_button_group.d.ts.map
```

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/multi_choice.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/multi_choice.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/multiple_date_picker.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/multiple_date_picker.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/multiple_datetime_picker.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/multiple_datetime_picker.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/multiselect.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/multiselect.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/numeric_input.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/numeric_input.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/oriented_control.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/oriented_control.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/paragraph.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/paragraph.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/password_input.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/password_input.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/picker_base.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/picker_base.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/pretext.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/pretext.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/radio_button_group.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/radio_button_group.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/radio_group.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/radio_group.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/range_slider.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/range_slider.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/selectbox.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/selectbox.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/slider.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/slider.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/spinner.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/spinner.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/switch.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/switch.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/tables/cell_editors.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/tables/cell_editors.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/tables/cell_formatters.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/tables/cell_formatters.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/tables/data_cube.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/tables/data_cube.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/tables/data_table.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/tables/data_table.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/tables/row_aggregators.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/tables/row_aggregators.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/tables/table_column.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/tables/table_column.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/tables/table_widget.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/tables/table_widget.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/text_input.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/text_input.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/text_like_input.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/text_like_input.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/textarea_input.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/textarea_input.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/time_picker.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/time_picker.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/toggle.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/toggle.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/toggle_button_group.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/toggle_input_group.d.ts`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,27 @@
-import { OrientedControl, OrientedControlView } from "./oriented_control";
-import { ButtonType } from "../../core/enums";
+import { Control, ControlView } from "./control";
 import type { StyleSheetLike } from "../../core/dom";
 import type * as p from "../../core/properties";
-export declare abstract class ToggleButtonGroupView extends OrientedControlView {
-    model: ToggleButtonGroup;
-    protected _buttons: HTMLElement[];
-    controls(): Generator<any, void, any>;
+export declare abstract class ToggleInputGroupView extends ControlView {
+    model: ToggleInputGroup;
+    protected _inputs: HTMLInputElement[];
+    controls(): Generator<HTMLInputElement, void, undefined>;
     connect_signals(): void;
     stylesheets(): StyleSheetLike[];
-    render(): void;
-    abstract change_active(i: number): void;
-    protected abstract _update_active(): void;
 }
-export declare namespace ToggleButtonGroup {
+export declare namespace ToggleInputGroup {
     type Attrs = p.AttrsOf<Props>;
-    type Props = OrientedControl.Props & {
+    type Props = Control.Props & {
         labels: p.Property<string[]>;
-        button_type: p.Property<ButtonType>;
+        inline: p.Property<boolean>;
     };
 }
-export interface ToggleButtonGroup extends ToggleButtonGroup.Attrs {
+export interface ToggleInputGroup extends ToggleInputGroup.Attrs {
 }
-export declare abstract class ToggleButtonGroup extends OrientedControl {
-    properties: ToggleButtonGroup.Props & {
+export declare abstract class ToggleInputGroup extends Control {
+    properties: ToggleInputGroup.Props & {
         active: p.Property<unknown>;
     };
-    __view_type__: ToggleButtonGroupView;
-    constructor(attrs?: Partial<ToggleButtonGroup.Attrs>);
+    __view_type__: ToggleInputGroupView;
+    constructor(attrs?: Partial<ToggleInputGroup.Attrs>);
 }
-//# sourceMappingURL=toggle_button_group.d.ts.map
+//# sourceMappingURL=toggle_input_group.d.ts.map
```

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/toggle_input.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/toggle_input.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/models/widgets/widget.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/models/widgets/widget.d.ts`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import { LayoutDOM, LayoutDOMView } from "../layouts/layout_dom";
 import type { MathJaxProvider } from "../text/providers";
 import type * as p from "../../core/properties";
 export declare abstract class WidgetView extends LayoutDOMView {
     model: Widget;
-    update_style(): void;
     get child_models(): LayoutDOM[];
     get provider(): MathJaxProvider;
     lazy_initialize(): Promise<void>;
     _after_layout(): void;
     process_tex(text: string): string;
     protected contains_tex_string(text: string): boolean;
 }
```

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/protocol/message.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/protocol/message.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/protocol/receiver.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/protocol/receiver.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/js/lib/styles/icons.css.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/js/lib/styles/icons.css.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.decorators.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.decorators.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.decorators.legacy.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.decorators.legacy.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.dom.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.dom.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.dom.iterable.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.dom.iterable.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2015.collection.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2015.collection.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2015.core.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2015.core.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2015.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2015.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2015.generator.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2015.generator.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2015.iterable.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2015.iterable.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2015.promise.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2015.promise.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2015.proxy.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2015.proxy.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2015.reflect.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2015.reflect.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2015.symbol.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2015.symbol.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2015.symbol.wellknown.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2015.symbol.wellknown.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2016.array.include.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2016.array.include.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2016.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2016.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2016.full.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2016.full.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2017.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2017.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2017.full.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2017.full.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2017.intl.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2017.intl.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2017.object.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2017.object.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2017.sharedmemory.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2017.sharedmemory.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2017.string.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2017.string.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2017.typedarrays.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2017.typedarrays.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2018.asyncgenerator.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2018.asyncgenerator.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2018.asynciterable.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2018.asynciterable.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2018.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2018.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2018.full.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2018.full.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2018.intl.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2018.intl.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2018.promise.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2018.promise.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2018.regexp.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2018.regexp.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2019.array.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2019.array.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2019.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2019.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2019.full.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2019.full.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2019.intl.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2019.intl.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2019.object.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2019.object.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2019.string.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2019.string.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2019.symbol.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2019.symbol.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2020.bigint.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2020.bigint.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2020.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2020.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2020.date.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2020.date.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2020.full.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2020.full.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2020.intl.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2020.intl.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2020.number.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2020.number.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2020.promise.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2020.promise.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2020.sharedmemory.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2020.sharedmemory.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2020.string.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2020.string.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2020.symbol.wellknown.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2020.symbol.wellknown.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2021.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2021.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2021.full.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2021.full.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2021.intl.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2021.intl.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2021.promise.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2021.promise.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2021.string.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2021.string.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2021.weakref.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2021.weakref.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2022.array.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2022.array.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2022.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2022.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2022.error.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2022.error.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2022.full.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2022.full.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2022.intl.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2022.intl.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2022.object.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2022.object.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2022.regexp.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2022.regexp.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2022.sharedmemory.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2022.sharedmemory.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2022.string.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2022.string.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2023.array.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2023.array.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2023.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2023.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es2023.full.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es2023.full.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es5.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es5.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.es6.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.es6.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.esnext.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.esnext.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.esnext.full.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.esnext.full.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.esnext.intl.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.esnext.intl.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.scripthost.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.scripthost.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.webworker.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.webworker.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.webworker.importscripts.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.webworker.importscripts.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/static/lib/lib.webworker.iterable.d.ts` & `bokeh-3.2.0.dev4/src/bokeh/server/static/lib/lib.webworker.iterable.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/tornado.py` & `bokeh-3.2.0.dev4/src/bokeh/server/tornado.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/urls.py` & `bokeh-3.2.0.dev4/src/bokeh/server/urls.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/util.py` & `bokeh-3.2.0.dev4/src/bokeh/server/util.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/views/app_index.html` & `bokeh-3.2.0.dev4/src/bokeh/server/views/app_index.html`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/views/auth_request_handler.py` & `bokeh-3.2.0.dev4/src/bokeh/server/views/auth_request_handler.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/views/autoload_js_handler.py` & `bokeh-3.2.0.dev4/src/bokeh/server/views/autoload_js_handler.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/views/bokeh-dev.ico` & `bokeh-3.2.0.dev4/src/bokeh/server/views/bokeh-dev.ico`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/views/bokeh.ico` & `bokeh-3.2.0.dev4/src/bokeh/server/views/bokeh.ico`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/views/doc_handler.py` & `bokeh-3.2.0.dev4/src/bokeh/server/views/doc_handler.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/views/ico_handler.py` & `bokeh-3.2.0.dev4/src/bokeh/server/views/ico_handler.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/views/metadata_handler.py` & `bokeh-3.2.0.dev4/src/bokeh/server/views/metadata_handler.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/views/multi_root_static_handler.py` & `bokeh-3.2.0.dev4/src/bokeh/server/views/multi_root_static_handler.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/views/root_handler.py` & `bokeh-3.2.0.dev4/src/bokeh/server/views/root_handler.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/views/session_handler.py` & `bokeh-3.2.0.dev4/src/bokeh/server/views/session_handler.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/views/static_handler.py` & `bokeh-3.2.0.dev4/src/bokeh/server/views/static_handler.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/server/views/ws.py` & `bokeh-3.2.0.dev4/src/bokeh/server/views/ws.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/settings.py` & `bokeh-3.2.0.dev4/src/bokeh/settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -434,14 +434,17 @@
 
     def __get__(self, instance: Any, owner: type[Any]) -> PrioritizedSetting[T]:
         return self
 
     def __set__(self, instance: Any, value: str | T) -> None:
         self.set_value(value)
 
+    def __delete__(self, instance: Any) -> None:
+        self.unset_value()
+
     def set_value(self, value: str | T) -> None:
         ''' Specify a value for this setting programmatically.
 
         A value set this way takes precedence over all other methods except
         immediate values.
 
         Args:
```

### Comparing `bokeh-3.2.0.dev3/src/bokeh/sphinxext/__init__.py` & `bokeh-3.2.0.dev4/src/bokeh/sphinxext/__init__.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/sphinxext/_templates/bokehjs_codepen_init.html` & `bokeh-3.2.0.dev4/src/bokeh/sphinxext/_templates/bokehjs_codepen_init.html`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/sphinxext/_templates/gallery_page.rst` & `bokeh-3.2.0.dev4/src/bokeh/sphinxext/_templates/gallery_page.rst`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/sphinxext/_templates/release_detail.rst` & `bokeh-3.2.0.dev4/src/bokeh/sphinxext/_templates/release_detail.rst`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/sphinxext/bokeh_autodoc.py` & `bokeh-3.2.0.dev4/src/bokeh/sphinxext/bokeh_autodoc.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/sphinxext/bokeh_color.py` & `bokeh-3.2.0.dev4/src/bokeh/sphinxext/bokeh_color.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/sphinxext/bokeh_dataframe.py` & `bokeh-3.2.0.dev4/src/bokeh/sphinxext/bokeh_dataframe.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/sphinxext/bokeh_directive.py` & `bokeh-3.2.0.dev4/src/bokeh/sphinxext/bokeh_directive.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/sphinxext/bokeh_enum.py` & `bokeh-3.2.0.dev4/src/bokeh/sphinxext/bokeh_enum.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/sphinxext/bokeh_example_metadata.py` & `bokeh-3.2.0.dev4/src/bokeh/sphinxext/bokeh_example_metadata.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/sphinxext/bokeh_gallery.py` & `bokeh-3.2.0.dev4/src/bokeh/sphinxext/bokeh_gallery.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/sphinxext/bokeh_jinja.py` & `bokeh-3.2.0.dev4/src/bokeh/sphinxext/bokeh_jinja.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/sphinxext/bokeh_model.py` & `bokeh-3.2.0.dev4/src/bokeh/sphinxext/bokeh_model.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/sphinxext/bokeh_options.py` & `bokeh-3.2.0.dev4/src/bokeh/sphinxext/bokeh_options.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/sphinxext/bokeh_palette.py` & `bokeh-3.2.0.dev4/src/bokeh/sphinxext/bokeh_palette.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/sphinxext/bokeh_palette_group.py` & `bokeh-3.2.0.dev4/src/bokeh/sphinxext/bokeh_palette_group.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/sphinxext/bokeh_plot.py` & `bokeh-3.2.0.dev4/src/bokeh/sphinxext/bokeh_plot.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/sphinxext/bokeh_prop.py` & `bokeh-3.2.0.dev4/src/bokeh/sphinxext/bokeh_prop.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/sphinxext/bokeh_releases.py` & `bokeh-3.2.0.dev4/src/bokeh/sphinxext/bokeh_releases.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/sphinxext/bokeh_roles.py` & `bokeh-3.2.0.dev4/src/bokeh/sphinxext/bokeh_roles.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/sphinxext/bokeh_sampledata_xref.py` & `bokeh-3.2.0.dev4/src/bokeh/sphinxext/bokeh_sampledata_xref.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/sphinxext/bokeh_settings.py` & `bokeh-3.2.0.dev4/src/bokeh/sphinxext/bokeh_settings.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/sphinxext/bokeh_sitemap.py` & `bokeh-3.2.0.dev4/src/bokeh/sphinxext/bokeh_sitemap.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/sphinxext/bokehjs_content.py` & `bokeh-3.2.0.dev4/src/bokeh/sphinxext/bokehjs_content.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/sphinxext/example_handler.py` & `bokeh-3.2.0.dev4/src/bokeh/sphinxext/example_handler.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/sphinxext/sample.py` & `bokeh-3.2.0.dev4/src/bokeh/sphinxext/sample.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/sphinxext/templates.py` & `bokeh-3.2.0.dev4/src/bokeh/sphinxext/templates.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/sphinxext/util.py` & `bokeh-3.2.0.dev4/src/bokeh/sphinxext/util.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/themes/__init__.py` & `bokeh-3.2.0.dev4/src/bokeh/themes/__init__.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/themes/_caliber.py` & `bokeh-3.2.0.dev4/src/bokeh/themes/_caliber.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/themes/_contrast.py` & `bokeh-3.2.0.dev4/src/bokeh/themes/_contrast.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/themes/_dark_minimal.py` & `bokeh-3.2.0.dev4/src/bokeh/themes/_dark_minimal.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/themes/_light_minimal.py` & `bokeh-3.2.0.dev4/src/bokeh/themes/_light_minimal.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/themes/_night_sky.py` & `bokeh-3.2.0.dev4/src/bokeh/themes/_night_sky.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/themes/theme.py` & `bokeh-3.2.0.dev4/src/bokeh/themes/theme.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/tile_providers.py` & `bokeh-3.2.0.dev4/src/bokeh/tile_providers.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/transform.py` & `bokeh-3.2.0.dev4/src/bokeh/transform.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/util/__init__.py` & `bokeh-3.2.0.dev4/src/bokeh/util/__init__.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/util/browser.py` & `bokeh-3.2.0.dev4/src/bokeh/util/browser.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/util/callback_manager.py` & `bokeh-3.2.0.dev4/src/bokeh/util/callback_manager.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/util/compiler.py` & `bokeh-3.2.0.dev4/src/bokeh/util/compiler.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/util/dataclasses.py` & `bokeh-3.2.0.dev4/src/bokeh/util/dataclasses.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/util/datatypes.py` & `bokeh-3.2.0.dev4/src/bokeh/util/datatypes.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/util/dependencies.py` & `bokeh-3.2.0.dev4/src/bokeh/util/dependencies.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/util/deprecation.py` & `bokeh-3.2.0.dev4/src/bokeh/util/deprecation.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/util/functions.py` & `bokeh-3.2.0.dev4/src/bokeh/util/functions.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/util/hex.py` & `bokeh-3.2.0.dev4/src/bokeh/util/hex.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/util/logconfig.py` & `bokeh-3.2.0.dev4/src/bokeh/util/logconfig.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/util/options.py` & `bokeh-3.2.0.dev4/src/bokeh/util/options.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/util/package.py` & `bokeh-3.2.0.dev4/src/bokeh/util/package.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/util/paths.py` & `bokeh-3.2.0.dev4/src/bokeh/util/paths.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/util/sampledata.json` & `bokeh-3.2.0.dev4/src/bokeh/util/sampledata.json`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/util/sampledata.py` & `bokeh-3.2.0.dev4/src/bokeh/util/sampledata.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/util/serialization.py` & `bokeh-3.2.0.dev4/src/bokeh/util/serialization.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/util/strings.py` & `bokeh-3.2.0.dev4/src/bokeh/util/strings.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/util/terminal.py` & `bokeh-3.2.0.dev4/src/bokeh/util/terminal.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/util/token.py` & `bokeh-3.2.0.dev4/src/bokeh/util/token.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/util/tornado.py` & `bokeh-3.2.0.dev4/src/bokeh/util/tornado.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/util/version.py` & `bokeh-3.2.0.dev4/src/bokeh/util/version.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh/util/warnings.py` & `bokeh-3.2.0.dev4/src/bokeh/util/warnings.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/src/bokeh.egg-info/PKG-INFO` & `bokeh-3.2.0.dev4/src/bokeh.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bokeh
-Version: 3.2.0.dev3
+Version: 3.2.0.dev4
 Summary: Interactive plots and applications in the browser from Python
 Author: Bokeh Team
 Author-email: info@bokeh.org
 License: Copyright (c) 2012 - 2023, Anaconda, Inc., and Bokeh Contributors
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without modification,
```

### Comparing `bokeh-3.2.0.dev3/src/bokeh.egg-info/SOURCES.txt` & `bokeh-3.2.0.dev4/src/bokeh.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/tests/test_bokehjs.py` & `bokeh-3.2.0.dev4/tests/test_bokehjs.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/tests/test_cross.py` & `bokeh-3.2.0.dev4/tests/test_cross.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/tests/test_defaults.py` & `bokeh-3.2.0.dev4/tests/test_defaults.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.0.dev3/tests/test_examples.py` & `bokeh-3.2.0.dev4/tests/test_examples.py`

 * *Files identical despite different names*

