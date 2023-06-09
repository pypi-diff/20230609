# Comparing `tmp/ellar-0.4.0.tar.gz` & `tmp/ellar-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ellar-0.4.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "ellar-0.4.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ellar-0.4.0.tar` & `ellar-0.4.2.tar`

### file list

```diff
@@ -1,535 +1,544 @@
--rw-r--r--   0        0        0      270 2023-05-29 23:22:51.594828 ellar-0.4.0/.coveragerc
--rw-r--r--   0        0        0       65 2023-05-29 23:22:51.594828 ellar-0.4.0/.dockerignore
--rw-r--r--   0        0        0      146 2023-05-29 23:22:51.594828 ellar-0.4.0/.flake8
--rw-r--r--   0        0        0      205 2023-05-29 23:22:51.594828 ellar-0.4.0/.github/dependabot.yml
--rw-r--r--   0        0        0      635 2023-05-29 23:22:51.594828 ellar-0.4.0/.github/workflows/publish.yml
--rw-r--r--   0        0        0      545 2023-05-29 23:22:51.594828 ellar-0.4.0/.github/workflows/test.yml
--rw-r--r--   0        0        0     1122 2023-05-29 23:22:51.594828 ellar-0.4.0/.github/workflows/test_full.yml
--rw-r--r--   0        0        0     1891 2023-05-29 23:22:51.594828 ellar-0.4.0/.gitignore
--rw-r--r--   0        0        0       53 2023-05-29 23:22:51.594828 ellar-0.4.0/.isort.cfg
--rw-r--r--   0        0        0     1073 2023-05-29 23:22:51.594828 ellar-0.4.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1083 2023-05-29 23:22:51.594828 ellar-0.4.0/LICENSE
--rw-r--r--   0        0        0     1166 2023-05-29 23:22:51.594828 ellar-0.4.0/Makefile
--rw-r--r--   0        0        0    10596 2023-05-29 23:22:51.594828 ellar-0.4.0/README.md
--rw-r--r--   0        0        0     2289 2023-05-29 23:22:51.594828 ellar-0.4.0/docs/background-task.md
--rw-r--r--   0        0        0       15 2023-05-29 23:22:51.594828 ellar-0.4.0/docs/basics/api-docs.md
--rw-r--r--   0        0        0        0 2023-05-29 23:22:51.594828 ellar-0.4.0/docs/basics/custom-providers.md
--rw-r--r--   0        0        0       15 2023-05-29 23:22:51.594828 ellar-0.4.0/docs/basics/events.md
--rw-r--r--   0        0        0    10686 2023-05-29 23:22:51.594828 ellar-0.4.0/docs/basics/execution-context.md
--rw-r--r--   0        0        0        0 2023-05-29 23:22:51.594828 ellar-0.4.0/docs/basics/file-streaming.md
--rw-r--r--   0        0        0        0 2023-05-29 23:22:51.594828 ellar-0.4.0/docs/basics/injection-scope.md
--rw-r--r--   0        0        0        0 2023-05-29 23:22:51.594828 ellar-0.4.0/docs/basics/model-view-controller.md
--rw-r--r--   0        0        0    14852 2023-05-29 23:22:51.594828 ellar-0.4.0/docs/basics/testing.md
--rw-r--r--   0        0        0     7874 2023-05-29 23:22:51.594828 ellar-0.4.0/docs/basics/versioning.md
--rw-r--r--   0        0        0    21109 2023-05-29 23:22:51.594828 ellar-0.4.0/docs/caching.md
--rw-r--r--   0        0        0     1177 2023-05-29 23:22:51.594828 ellar-0.4.0/docs/commands/command-grouping.md
--rw-r--r--   0        0        0     6586 2023-05-29 23:22:51.594828 ellar-0.4.0/docs/commands/create-module-command.md
--rw-r--r--   0        0        0      388 2023-05-29 23:22:51.594828 ellar-0.4.0/docs/commands/create-project-command.md
--rw-r--r--   0        0        0     2755 2023-05-29 23:22:51.594828 ellar-0.4.0/docs/commands/custom-commands.md
--rw-r--r--   0        0        0     1340 2023-05-29 23:22:51.594828 ellar-0.4.0/docs/commands/index.md
--rw-r--r--   0        0        0     1206 2023-05-29 23:22:51.594828 ellar-0.4.0/docs/commands/new-command.md
--rw-r--r--   0        0        0      803 2023-05-29 23:22:51.594828 ellar-0.4.0/docs/commands/runserver-command.md
--rw-r--r--   0        0        0     9081 2023-05-29 23:22:51.594828 ellar-0.4.0/docs/configurations.md
--rw-r--r--   0        0        0     1765 2023-05-29 23:22:51.594828 ellar-0.4.0/docs/custom-setup.md
--rw-r--r--   0        0        0     6521 2023-05-29 23:22:51.594828 ellar-0.4.0/docs/handling-response/response-model.md
--rw-r--r--   0        0        0     6571 2023-05-29 23:22:51.594828 ellar-0.4.0/docs/handling-response/response.md
--rwxr-xr-x   0        0        0    25915 2023-05-29 23:22:51.598828 ellar-0.4.0/docs/img/EllarLogoB.png
--rwxr-xr-x   0        0        0    36744 2023-05-29 23:22:51.598828 ellar-0.4.0/docs/img/EllarLogoIconOnly.png
--rwxr-xr-x   0        0        0    26456 2023-05-29 23:22:51.598828 ellar-0.4.0/docs/img/EllarLogoW.png
--rwxr-xr-x   0        0        0     3888 2023-05-29 23:22:51.598828 ellar-0.4.0/docs/img/Icon.svg
--rwxr-xr-x   0        0        0     4781 2023-05-29 23:22:51.598828 ellar-0.4.0/docs/img/Logo.svg
--rw-r--r--   0        0        0    92094 2023-05-29 23:22:51.598828 ellar-0.4.0/docs/img/ModuleDescription.png
--rw-r--r--   0        0        0    71483 2023-05-29 23:22:51.598828 ellar-0.4.0/docs/img/body-schema-doc.png
--rw-r--r--   0        0        0   233058 2023-05-29 23:22:51.598828 ellar-0.4.0/docs/img/body-schema-doc2.png
--rw-r--r--   0        0        0   196608 2023-05-29 23:22:51.598828 ellar-0.4.0/docs/img/body-schema-doc3.png
--rwxr-xr-x   0        0        0    54689 2023-05-29 23:22:51.598828 ellar-0.4.0/docs/img/car_api.png
--rw-r--r--   0        0        0  1632661 2023-05-29 23:22:51.610828 ellar-0.4.0/docs/img/car_controller.gif
--rw-r--r--   0        0        0    50364 2023-05-29 23:22:51.610828 ellar-0.4.0/docs/img/controller_description.png
--rw-r--r--   0        0        0    45273 2023-05-29 23:22:51.614828 ellar-0.4.0/docs/img/create-car-schema.png
--rw-r--r--   0        0        0    19519 2023-05-29 23:22:51.614828 ellar-0.4.0/docs/img/create-dog-schema.png
--rwxr-xr-x   0        0        0  1326350 2023-05-29 23:22:51.618828 ellar-0.4.0/docs/img/ellar_demo.gif
--rwxr-xr-x   0        0        0    69977 2023-05-29 23:22:51.618828 ellar-0.4.0/docs/img/ellar_framework.png
--rw-r--r--   0        0        0   244178 2023-05-29 23:22:51.622828 ellar-0.4.0/docs/img/enum_docs_swagger.png
--rw-r--r--   0        0        0   168505 2023-05-29 23:22:51.622828 ellar-0.4.0/docs/img/event_docs_swagger.png
--rw-r--r--   0        0        0   253271 2023-05-29 23:22:51.622828 ellar-0.4.0/docs/img/form-schema-doc.png
--rw-r--r--   0        0        0   170683 2023-05-29 23:22:51.622828 ellar-0.4.0/docs/img/json_api_response_model.png
--rw-r--r--   0        0        0    71548 2023-05-29 23:22:51.622828 ellar-0.4.0/docs/img/live_support_websocket.gif
--rw-r--r--   0        0        0   121361 2023-05-29 23:22:51.626828 ellar-0.4.0/docs/img/live_support_websocket_3.gif
--rw-r--r--   0        0        0   216500 2023-05-29 23:22:51.626828 ellar-0.4.0/docs/img/math_router.png
--rw-r--r--   0        0        0   280669 2023-05-29 23:22:51.626828 ellar-0.4.0/docs/img/math_router_with_request_object.png
--rw-r--r--   0        0        0    52280 2023-05-29 23:22:51.626828 ellar-0.4.0/docs/img/middleware.png
--rw-r--r--   0        0        0   267982 2023-05-29 23:22:51.630828 ellar-0.4.0/docs/img/query_filter_swagger.png
--rw-r--r--   0        0        0   208787 2023-05-29 23:22:51.630828 ellar-0.4.0/docs/img/response_description.png
--rw-r--r--   0        0        0     4486 2023-05-29 23:22:51.630828 ellar-0.4.0/docs/index.md
--rw-r--r--   0        0        0     2028 2023-05-29 23:22:51.630828 ellar-0.4.0/docs/mount.md
--rw-r--r--   0        0        0    12559 2023-05-29 23:22:51.630828 ellar-0.4.0/docs/overview/controllers.md
--rw-r--r--   0        0        0    22477 2023-05-29 23:22:51.630828 ellar-0.4.0/docs/overview/custom_decorators.md
--rw-r--r--   0        0        0     7997 2023-05-29 23:22:51.630828 ellar-0.4.0/docs/overview/exception_handling.md
--rw-r--r--   0        0        0     8976 2023-05-29 23:22:51.630828 ellar-0.4.0/docs/overview/guards.md
--rw-r--r--   0        0        0     7695 2023-05-29 23:22:51.630828 ellar-0.4.0/docs/overview/index.md
--rw-r--r--   0        0        0     6521 2023-05-29 23:22:51.630828 ellar-0.4.0/docs/overview/interceptors.md
--rw-r--r--   0        0        0     9258 2023-05-29 23:22:51.630828 ellar-0.4.0/docs/overview/middleware.md
--rw-r--r--   0        0        0     4497 2023-05-29 23:22:51.630828 ellar-0.4.0/docs/overview/module-router.md
--rw-r--r--   0        0        0    15337 2023-05-29 23:22:51.630828 ellar-0.4.0/docs/overview/modules.md
--rw-r--r--   0        0        0     9391 2023-05-29 23:22:51.630828 ellar-0.4.0/docs/overview/providers.md
--rw-r--r--   0        0        0     8879 2023-05-29 23:22:51.630828 ellar-0.4.0/docs/parsing-inputs/body.md
--rw-r--r--   0        0        0     1371 2023-05-29 23:22:51.630828 ellar-0.4.0/docs/parsing-inputs/cookie-params.md
--rw-r--r--   0        0        0     6588 2023-05-29 23:22:51.630828 ellar-0.4.0/docs/parsing-inputs/file-params.md
--rw-r--r--   0        0        0     4096 2023-05-29 23:22:51.630828 ellar-0.4.0/docs/parsing-inputs/form-params.md
--rw-r--r--   0        0        0     3795 2023-05-29 23:22:51.630828 ellar-0.4.0/docs/parsing-inputs/header-params.md
--rw-r--r--   0        0        0     1560 2023-05-29 23:22:51.630828 ellar-0.4.0/docs/parsing-inputs/index.md
--rw-r--r--   0        0        0     6749 2023-05-29 23:22:51.630828 ellar-0.4.0/docs/parsing-inputs/path-params.md
--rw-r--r--   0        0        0     4920 2023-05-29 23:22:51.630828 ellar-0.4.0/docs/parsing-inputs/query-params.md
--rw-r--r--   0        0        0        0 2023-05-29 23:22:51.630828 ellar-0.4.0/docs/release-notes.md
--rw-r--r--   0        0        0       69 2023-05-29 23:22:51.630828 ellar-0.4.0/docs/stylesheets/extra.css
--rw-r--r--   0        0        0     4130 2023-05-29 23:22:51.630828 ellar-0.4.0/docs/templating/staticfiles.md
--rw-r--r--   0        0        0    13707 2023-05-29 23:22:51.630828 ellar-0.4.0/docs/templating/templating.md
--rw-r--r--   0        0        0     7368 2023-05-29 23:22:51.630828 ellar-0.4.0/docs/throttling.md
--rw-r--r--   0        0        0    12692 2023-05-29 23:22:51.630828 ellar-0.4.0/docs/websockets/index.md
--rw-r--r--   0        0        0    12912 2023-05-29 23:22:51.630828 ellar-0.4.0/docs/websockets/socketio.md
--rw-r--r--   0        0        0      143 2023-05-29 23:22:51.630828 ellar-0.4.0/ellar/__init__.py
--rw-r--r--   0        0        0      257 2023-05-29 23:22:51.630828 ellar-0.4.0/ellar/cache/__init__.py
--rw-r--r--   0        0        0      109 2023-05-29 23:22:51.630828 ellar-0.4.0/ellar/cache/backends/__init__.py
--rw-r--r--   0        0        0     4841 2023-05-29 23:22:51.630828 ellar-0.4.0/ellar/cache/backends/_aio_cache.py.ellar
--rw-r--r--   0        0        0     4361 2023-05-29 23:22:51.630828 ellar-0.4.0/ellar/cache/backends/base.py
--rw-r--r--   0        0        0     5145 2023-05-29 23:22:51.630828 ellar-0.4.0/ellar/cache/backends/local_cache.py
--rw-r--r--   0        0        0      944 2023-05-29 23:22:51.630828 ellar-0.4.0/ellar/cache/backends/pylib_cache.py
--rw-r--r--   0        0        0     2215 2023-05-29 23:22:51.630828 ellar-0.4.0/ellar/cache/backends/pymem_cache.py
--rw-r--r--   0        0        0       72 2023-05-29 23:22:51.630828 ellar-0.4.0/ellar/cache/backends/redis/__init__.py
--rw-r--r--   0        0        0     6548 2023-05-29 23:22:51.630828 ellar-0.4.0/ellar/cache/backends/redis/backend.py
--rw-r--r--   0        0        0     1397 2023-05-29 23:22:51.630828 ellar-0.4.0/ellar/cache/backends/serializer.py
--rw-r--r--   0        0        0     2923 2023-05-29 23:22:51.630828 ellar-0.4.0/ellar/cache/decorator.py
--rw-r--r--   0        0        0    10943 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/cache/interface.py
--rw-r--r--   0        0        0     2027 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/cache/make_key_decorator.py
--rw-r--r--   0        0        0     2501 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/cache/model.py
--rw-r--r--   0        0        0     1859 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/cache/module.py
--rw-r--r--   0        0        0      852 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/cache/schema.py
--rw-r--r--   0        0        0     4489 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/cache/service.py
--rw-r--r--   0        0        0     3958 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/__init__.py
--rw-r--r--   0        0        0      108 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/commands/__init__.py
--rw-r--r--   0        0        0     2254 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/commands/base.py
--rw-r--r--   0        0        0     1537 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/commands/decorator.py
--rw-r--r--   0        0        0      270 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/compatible/__init__.py
--rw-r--r--   0        0        0     1166 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/compatible/cache_properties.py
--rw-r--r--   0        0        0     1511 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/compatible/dict.py
--rw-r--r--   0        0        0      637 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/compatible/emails.py
--rw-r--r--   0        0        0     4768 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/constants.py
--rw-r--r--   0        0        0     1670 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/converters.py
--rw-r--r--   0        0        0      809 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/datastructures.py
--rw-r--r--   0        0        0      865 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/decorators/__init__.py
--rw-r--r--   0        0        0      485 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/decorators/base.py
--rw-r--r--   0        0        0     7141 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/decorators/controller.py
--rw-r--r--   0        0        0     1036 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/decorators/exception.py
--rw-r--r--   0        0        0      610 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/decorators/extra_args.py
--rw-r--r--   0        0        0     2528 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/decorators/file.py
--rw-r--r--   0        0        0     1025 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/decorators/guards.py
--rw-r--r--   0        0        0     4748 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/decorators/html.py
--rw-r--r--   0        0        0     1084 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/decorators/interceptor.py
--rw-r--r--   0        0        0      648 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/decorators/middleware.py
--rw-r--r--   0        0        0     3105 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/decorators/modules.py
--rw-r--r--   0        0        0      932 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/decorators/openapi.py
--rw-r--r--   0        0        0     1295 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/decorators/serializer.py
--rw-r--r--   0        0        0      402 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/decorators/versioning.py
--rw-r--r--   0        0        0      840 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/exceptions/__init__.py
--rw-r--r--   0        0        0      472 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/exceptions/api/__init__.py
--rw-r--r--   0        0        0     1447 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/exceptions/api/base.py
--rw-r--r--   0        0        0     1239 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/exceptions/api/exceptions_types.py
--rw-r--r--   0        0        0     2498 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/exceptions/callable_exceptions.py
--rw-r--r--   0        0        0      103 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/exceptions/context.py
--rw-r--r--   0        0        0     2517 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/exceptions/handlers.py
--rw-r--r--   0        0        0      598 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/exceptions/validation.py
--rw-r--r--   0        0        0     1485 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/helper/__init__.py
--rw-r--r--   0        0        0      658 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/helper/enums.py
--rw-r--r--   0        0        0      389 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/helper/event_loop.py
--rw-r--r--   0        0        0     2137 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/helper/importer.py
--rw-r--r--   0        0        0     1272 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/helper/modelfield.py
--rw-r--r--   0        0        0      703 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/helper/module_loading.py
--rw-r--r--   0        0        0      952 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/interfaces/__init__.py
--rw-r--r--   0        0        0     3560 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/interfaces/context.py
--rw-r--r--   0        0        0      278 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/interfaces/controller_factory.py
--rw-r--r--   0        0        0     1356 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/interfaces/exceptions.py
--rw-r--r--   0        0        0      400 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/interfaces/guard_consumer.py
--rw-r--r--   0        0        0      406 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/interfaces/interceptor_consumer.py
--rw-r--r--   0        0        0     1771 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/interfaces/module.py
--rw-r--r--   0        0        0      749 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/interfaces/response_model.py
--rw-r--r--   0        0        0      908 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/interfaces/templating.py
--rw-r--r--   0        0        0       52 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/logger.py
--rw-r--r--   0        0        0      340 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/models/__init__.py
--rw-r--r--   0        0        0      923 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/models/controller.py
--rw-r--r--   0        0        0     4258 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/models/guard.py
--rw-r--r--   0        0        0      320 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/models/interceptor.py
--rw-r--r--   0        0        0      476 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/params/__init__.py
--rw-r--r--   0        0        0      365 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/params/args/__init__.py
--rw-r--r--   0        0        0    14227 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/params/args/base.py
--rw-r--r--   0        0        0     1615 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/params/args/extra_args.py
--rw-r--r--   0        0        0     2045 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/params/args/factory.py
--rw-r--r--   0        0        0     4252 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/params/args/request_model.py
--rw-r--r--   0        0        0     5893 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/params/args/resolver_generators.py
--rw-r--r--   0        0        0     2457 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/params/args/websocket_model.py
--rw-r--r--   0        0        0    10559 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/params/decorators.py
--rw-r--r--   0        0        0     1235 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/params/helpers.py
--rw-r--r--   0        0        0     9342 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/params/params.py
--rw-r--r--   0        0        0     1083 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/params/resolvers/__init__.py
--rw-r--r--   0        0        0     1678 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/params/resolvers/base.py
--rw-r--r--   0        0        0     4460 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/params/resolvers/bulk_parameter.py
--rw-r--r--   0        0        0      768 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/params/resolvers/non_parameter/__init__.py
--rw-r--r--   0        0        0      868 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/params/resolvers/non_parameter/background.py
--rw-r--r--   0        0        0     2961 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/params/resolvers/non_parameter/base.py
--rw-r--r--   0        0        0      391 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/params/resolvers/non_parameter/connection.py
--rw-r--r--   0        0        0      328 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/params/resolvers/non_parameter/context.py
--rw-r--r--   0        0        0     1660 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/params/resolvers/non_parameter/inject.py
--rw-r--r--   0        0        0      387 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/params/resolvers/non_parameter/request.py
--rw-r--r--   0        0        0      394 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/params/resolvers/non_parameter/response.py
--rw-r--r--   0        0        0      524 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/params/resolvers/non_parameter/session.py
--rw-r--r--   0        0        0      386 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/params/resolvers/non_parameter/websocket.py
--rw-r--r--   0        0        0     9544 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/params/resolvers/parameter.py
--rw-r--r--   0        0        0      415 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/responses/__init__.py
--rw-r--r--   0        0        0      925 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/responses/models/__init__.py
--rw-r--r--   0        0        0     6157 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/responses/models/base.py
--rw-r--r--   0        0        0       50 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/responses/models/exceptions.py
--rw-r--r--   0        0        0     3129 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/responses/models/file.py
--rw-r--r--   0        0        0      691 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/responses/models/helper.py
--rw-r--r--   0        0        0     1952 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/responses/models/html.py
--rw-r--r--   0        0        0     2383 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/responses/models/json.py
--rw-r--r--   0        0        0     4392 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/responses/models/route.py
--rw-r--r--   0        0        0     2167 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/responses/models/type_converter.py
--rw-r--r--   0        0        0      995 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/responses/response_types.py
--rw-r--r--   0        0        0     1181 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/routing/__init__.py
--rw-r--r--   0        0        0     4511 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/common/routing/base.py
--rw-r--r--   0        0        0      272 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/common/routing/controller/__init__.py
--rw-r--r--   0        0        0      877 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/common/routing/controller/base.py
--rw-r--r--   0        0        0      689 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/common/routing/controller/route.py
--rw-r--r--   0        0        0      190 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/common/routing/controller/websocket/__init__.py
--rw-r--r--   0        0        0     1424 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/common/routing/controller/websocket/handler.py
--rw-r--r--   0        0        0     1260 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/common/routing/controller/websocket/route.py
--rw-r--r--   0        0        0     6589 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/common/routing/mount.py
--rw-r--r--   0        0        0    10048 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/common/routing/operation_definitions.py
--rw-r--r--   0        0        0     4799 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/common/routing/route.py
--rw-r--r--   0        0        0     2985 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/common/routing/route_collections.py
--rw-r--r--   0        0        0     3689 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/common/routing/schema.py
--rw-r--r--   0        0        0      161 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/common/routing/websocket/__init__.py
--rw-r--r--   0        0        0     5680 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/common/routing/websocket/handler.py
--rw-r--r--   0        0        0     5158 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/common/routing/websocket/route.py
--rw-r--r--   0        0        0      499 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/common/serializer/__init__.py
--rw-r--r--   0        0        0     4960 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/common/serializer/base.py
--rw-r--r--   0        0        0      194 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/common/serializer/guard.py
--rw-r--r--   0        0        0      453 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/common/shortcuts.py
--rw-r--r--   0        0        0      613 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/common/templating/__init__.py
--rw-r--r--   0        0        0      472 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/common/templating/environment.py
--rw-r--r--   0        0        0     1634 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/common/templating/loader.py
--rw-r--r--   0        0        0     2895 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/common/templating/model.py
--rw-r--r--   0        0        0     2482 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/common/templating/renderer.py
--rw-r--r--   0        0        0      110 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/common/templating/schema.py
--rw-r--r--   0        0        0      585 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/common/types.py
--rw-r--r--   0        0        0      925 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/core/__init__.py
--rw-r--r--   0        0        0      120 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/core/conf/__init__.py
--rw-r--r--   0        0        0     4914 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/core/conf/app_settings_models.py
--rw-r--r--   0        0        0     2177 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/core/conf/config.py
--rw-r--r--   0        0        0     5122 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/core/conf/mixins.py
--rw-r--r--   0        0        0      470 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/core/connection/__init__.py
--rw-r--r--   0        0        0      688 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/core/connection/http.py
--rw-r--r--   0        0        0      245 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/core/connection/websocket.py
--rw-r--r--   0        0        0      458 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/core/context/__init__.py
--rw-r--r--   0        0        0     1315 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/core/context/execution.py
--rw-r--r--   0        0        0     2607 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/core/context/factory.py
--rw-r--r--   0        0        0     2091 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/core/context/host.py
--rw-r--r--   0        0        0     2122 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/core/context/http.py
--rw-r--r--   0        0        0      817 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/core/context/websocket.py
--rw-r--r--   0        0        0     1829 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/core/core_service_registration.py
--rw-r--r--   0        0        0       97 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/core/exceptions/__init__.py
--rw-r--r--   0        0        0     2273 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/core/exceptions/service.py
--rw-r--r--   0        0        0     7616 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/core/factory.py
--rw-r--r--   0        0        0      320 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/core/guard/__init__.py
--rw-r--r--   0        0        0      744 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/core/guard/apikey.py
--rw-r--r--   0        0        0     1729 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/core/guard/consumer.py
--rw-r--r--   0        0        0     3318 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/core/guard/http.py
--rw-r--r--   0        0        0       87 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/core/interceptors/__init__.py
--rw-r--r--   0        0        0     2083 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/core/interceptors/consumer.py
--rw-r--r--   0        0        0     9940 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/core/main.py
--rw-r--r--   0        0        0     1159 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/core/middleware/__init__.py
--rw-r--r--   0        0        0     2600 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/core/middleware/di.py
--rw-r--r--   0        0        0     2704 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/core/middleware/exceptions.py
--rw-r--r--   0        0        0     2256 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/core/middleware/function.py
--rw-r--r--   0        0        0      121 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/core/middleware/sessions.py
--rw-r--r--   0        0        0     1095 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/core/middleware/versioning.py
--rw-r--r--   0        0        0      321 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/core/modules/__init__.py
--rw-r--r--   0        0        0     1287 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/core/modules/base.py
--rw-r--r--   0        0        0     3143 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/core/modules/builder.py
--rw-r--r--   0        0        0     5827 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/core/modules/config.py
--rw-r--r--   0        0        0      787 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/core/modules/helper.py
--rw-r--r--   0        0        0     9876 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/core/modules/ref.py
--rw-r--r--   0        0        0      351 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/core/routing/__init__.py
--rw-r--r--   0        0        0     3661 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/core/routing/app.py
--rw-r--r--   0        0        0     1865 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/core/routing/builder.py
--rw-r--r--   0        0        0     1862 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/core/routing/factory.py
--rw-r--r--   0        0        0     1971 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/core/routing/helper.py
--rw-r--r--   0        0        0      794 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/core/routing/module_router.py
--rw-r--r--   0        0        0       58 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/core/services/__init__.py
--rw-r--r--   0        0        0     1951 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/core/services/reflector.py
--rw-r--r--   0        0        0     1718 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/core/staticfiles.py
--rw-r--r--   0        0        0       67 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/core/templating/__init__.py
--rw-r--r--   0        0        0     3978 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/core/templating/app.py
--rw-r--r--   0        0        0      563 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/core/versioning/__init__.py
--rw-r--r--   0        0        0     2526 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/core/versioning/base.py
--rw-r--r--   0        0        0     6040 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/core/versioning/resolver.py
--rw-r--r--   0        0        0      915 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/di/__init__.py
--rw-r--r--   0        0        0      344 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/di/asgi_args.py
--rw-r--r--   0        0        0     1073 2023-05-29 23:22:51.642828 ellar-0.4.0/ellar/di/constants.py
--rw-r--r--   0        0        0      400 2023-05-29 23:22:51.642828 ellar-0.4.0/ellar/di/exceptions.py
--rw-r--r--   0        0        0      117 2023-05-29 23:22:51.642828 ellar-0.4.0/ellar/di/injector/__init__.py
--rw-r--r--   0        0        0     7619 2023-05-29 23:22:51.642828 ellar-0.4.0/ellar/di/injector/container.py
--rw-r--r--   0        0        0     5268 2023-05-29 23:22:51.642828 ellar-0.4.0/ellar/di/injector/ellar_injector.py
--rw-r--r--   0        0        0      845 2023-05-29 23:22:51.642828 ellar-0.4.0/ellar/di/providers.py
--rw-r--r--   0        0        0     2247 2023-05-29 23:22:51.642828 ellar-0.4.0/ellar/di/scopes.py
--rw-r--r--   0        0        0     4533 2023-05-29 23:22:51.642828 ellar-0.4.0/ellar/di/service_config.py
--rw-r--r--   0        0        0       39 2023-05-29 23:22:51.642828 ellar-0.4.0/ellar/di/types.py
--rw-r--r--   0        0        0      244 2023-05-29 23:22:51.642828 ellar-0.4.0/ellar/di/utils.py
--rw-r--r--   0        0        0     2052 2023-05-29 23:22:51.642828 ellar-0.4.0/ellar/events.py
--rw-r--r--   0        0        0      573 2023-05-29 23:22:51.642828 ellar-0.4.0/ellar/openapi/__init__.py
--rw-r--r--   0        0        0     8069 2023-05-29 23:22:51.642828 ellar-0.4.0/ellar/openapi/builder.py
--rw-r--r--   0        0        0      239 2023-05-29 23:22:51.642828 ellar-0.4.0/ellar/openapi/docs_generators/__init__.py
--rw-r--r--   0        0        0      530 2023-05-29 23:22:51.642828 ellar-0.4.0/ellar/openapi/docs_generators/base.py
--rw-r--r--   0        0        0      959 2023-05-29 23:22:51.642828 ellar-0.4.0/ellar/openapi/docs_generators/redocs.py
--rw-r--r--   0        0        0     1025 2023-05-29 23:22:51.642828 ellar-0.4.0/ellar/openapi/docs_generators/swagger.py
--rw-r--r--   0        0        0     2937 2023-05-29 23:22:51.642828 ellar-0.4.0/ellar/openapi/module.py
--rw-r--r--   0        0        0    10611 2023-05-29 23:22:51.642828 ellar-0.4.0/ellar/openapi/openapi_v3.py
--rw-r--r--   0        0        0    15879 2023-05-29 23:22:51.642828 ellar-0.4.0/ellar/openapi/route_doc_models.py
--rw-r--r--   0        0        0      115 2023-05-29 23:22:51.642828 ellar-0.4.0/ellar/openapi/schemas/__init__.py
--rw-r--r--   0        0        0      342 2023-05-29 23:22:51.642828 ellar-0.4.0/ellar/openapi/schemas/validation.py
--rw-r--r--   0        0        0      702 2023-05-29 23:22:51.642828 ellar-0.4.0/ellar/openapi/templates/redocs.html
--rw-r--r--   0        0        0      758 2023-05-29 23:22:51.642828 ellar-0.4.0/ellar/openapi/templates/swagger.html
--rw-r--r--   0        0        0        0 2023-05-29 23:22:51.642828 ellar-0.4.0/ellar/py.typed
--rw-r--r--   0        0        0      180 2023-05-29 23:22:51.642828 ellar-0.4.0/ellar/reflect/__init__.py
--rw-r--r--   0        0        0     5356 2023-05-29 23:22:51.642828 ellar-0.4.0/ellar/reflect/_reflect.py
--rw-r--r--   0        0        0       34 2023-05-29 23:22:51.642828 ellar-0.4.0/ellar/reflect/constants.py
--rw-r--r--   0        0        0      238 2023-05-29 23:22:51.642828 ellar-0.4.0/ellar/reflect/contextmanager_fix.py
--rw-r--r--   0        0        0       58 2023-05-29 23:22:51.642828 ellar-0.4.0/ellar/samples/__init__.py
--rw-r--r--   0        0        0        0 2023-05-29 23:22:51.642828 ellar-0.4.0/ellar/samples/controllers/__init__.py
--rw-r--r--   0        0        0      381 2023-05-29 23:22:51.642828 ellar-0.4.0/ellar/samples/controllers/home.py
--rw-r--r--   0        0        0      211 2023-05-29 23:22:51.642828 ellar-0.4.0/ellar/samples/modules.py
--rw-r--r--   0        0        0   155845 2023-05-29 23:22:51.642828 ellar-0.4.0/ellar/samples/static/css/bootstrap.min.css
--rwxr-xr-x   0        0        0    25915 2023-05-29 23:22:51.642828 ellar-0.4.0/ellar/samples/static/img/EllarLogoB.png
--rwxr-xr-x   0        0        0    36744 2023-05-29 23:22:51.642828 ellar-0.4.0/ellar/samples/static/img/EllarLogoIconOnly.png
--rwxr-xr-x   0        0        0     3888 2023-05-29 23:22:51.642828 ellar-0.4.0/ellar/samples/static/img/Icon.svg
--rw-r--r--   0        0        0     1312 2023-05-29 23:22:51.642828 ellar-0.4.0/ellar/samples/templates/home/index.html
--rw-r--r--   0        0        0      596 2023-05-29 23:22:51.642828 ellar-0.4.0/ellar/socket_io/__init__.py
--rw-r--r--   0        0        0      423 2023-05-29 23:22:51.642828 ellar-0.4.0/ellar/socket_io/adapter.py
--rw-r--r--   0        0        0      524 2023-05-29 23:22:51.642828 ellar-0.4.0/ellar/socket_io/constants.py
--rw-r--r--   0        0        0     1659 2023-05-29 23:22:51.642828 ellar-0.4.0/ellar/socket_io/context.py
--rw-r--r--   0        0        0      225 2023-05-29 23:22:51.642828 ellar-0.4.0/ellar/socket_io/decorators/__init__.py
--rw-r--r--   0        0        0      667 2023-05-29 23:22:51.642828 ellar-0.4.0/ellar/socket_io/decorators/events.py
--rw-r--r--   0        0        0     3846 2023-05-29 23:22:51.642828 ellar-0.4.0/ellar/socket_io/decorators/gateway.py
--rw-r--r--   0        0        0      578 2023-05-29 23:22:51.642828 ellar-0.4.0/ellar/socket_io/decorators/subscribe_message.py
--rw-r--r--   0        0        0     2511 2023-05-29 23:22:51.642828 ellar-0.4.0/ellar/socket_io/factory.py
--rw-r--r--   0        0        0     9627 2023-05-29 23:22:51.642828 ellar-0.4.0/ellar/socket_io/gateway.py
--rw-r--r--   0        0        0      144 2023-05-29 23:22:51.642828 ellar-0.4.0/ellar/socket_io/model.py
--rw-r--r--   0        0        0      465 2023-05-29 23:22:51.642828 ellar-0.4.0/ellar/socket_io/responses.py
--rw-r--r--   0        0        0      107 2023-05-29 23:22:51.642828 ellar-0.4.0/ellar/socket_io/testing/__init__.py
--rw-r--r--   0        0        0     1704 2023-05-29 23:22:51.642828 ellar-0.4.0/ellar/socket_io/testing/module.py
--rw-r--r--   0        0        0      129 2023-05-29 23:22:51.642828 ellar-0.4.0/ellar/testing/__init__.py
--rw-r--r--   0        0        0     4074 2023-05-29 23:22:51.642828 ellar-0.4.0/ellar/testing/module.py
--rw-r--r--   0        0        0     1215 2023-05-29 23:22:51.642828 ellar-0.4.0/ellar/testing/uvicorn_server.py
--rw-r--r--   0        0        0      509 2023-05-29 23:22:51.642828 ellar-0.4.0/examples/01-carapp/README.md
--rw-r--r--   0        0        0        0 2023-05-29 23:22:51.642828 ellar-0.4.0/examples/01-carapp/carapp/__init__.py
--rw-r--r--   0        0        0        0 2023-05-29 23:22:51.642828 ellar-0.4.0/examples/01-carapp/carapp/apps/__init__.py
--rw-r--r--   0        0        0        0 2023-05-29 23:22:51.642828 ellar-0.4.0/examples/01-carapp/carapp/apps/car/__init__.py
--rw-r--r--   0        0        0     1659 2023-05-29 23:22:51.642828 ellar-0.4.0/examples/01-carapp/carapp/apps/car/controllers.py
--rw-r--r--   0        0        0     1077 2023-05-29 23:22:51.642828 ellar-0.4.0/examples/01-carapp/carapp/apps/car/module.py
--rw-r--r--   0        0        0     1146 2023-05-29 23:22:51.642828 ellar-0.4.0/examples/01-carapp/carapp/apps/car/routers.py
--rw-r--r--   0        0        0      629 2023-05-29 23:22:51.642828 ellar-0.4.0/examples/01-carapp/carapp/apps/car/schemas.py
--rw-r--r--   0        0        0      666 2023-05-29 23:22:51.642828 ellar-0.4.0/examples/01-carapp/carapp/apps/car/services.py
--rw-r--r--   0        0        0     1708 2023-05-29 23:22:51.642828 ellar-0.4.0/examples/01-carapp/carapp/apps/car/statics/blog/blog.css
--rw-r--r--   0        0        0     1586 2023-05-29 23:22:51.642828 ellar-0.4.0/examples/01-carapp/carapp/apps/car/statics/blog/blog.rtl.css
--rw-r--r--   0        0        0     1008 2023-05-29 23:22:51.642828 ellar-0.4.0/examples/01-carapp/carapp/apps/car/statics/brand/bootstrap-logo-white.svg
--rw-r--r--   0        0        0     2047 2023-05-29 23:22:51.642828 ellar-0.4.0/examples/01-carapp/carapp/apps/car/statics/brand/bootstrap-logo.svg
--rw-r--r--   0        0        0        0 2023-05-29 23:22:51.642828 ellar-0.4.0/examples/01-carapp/carapp/apps/car/tests/__init__.py
--rw-r--r--   0        0        0     2900 2023-05-29 23:22:51.642828 ellar-0.4.0/examples/01-carapp/carapp/apps/car/tests/test_controllers.py
--rw-r--r--   0        0        0     1604 2023-05-29 23:22:51.642828 ellar-0.4.0/examples/01-carapp/carapp/apps/car/tests/test_routers.py
--rw-r--r--   0        0        0        0 2023-05-29 23:22:51.642828 ellar-0.4.0/examples/01-carapp/carapp/apps/car/tests/test_services.py
--rw-r--r--   0        0        0      202 2023-05-29 23:22:51.646828 ellar-0.4.0/examples/01-carapp/carapp/apps/car/views/car/list.html
--rw-r--r--   0        0        0      202 2023-05-29 23:22:51.646828 ellar-0.4.0/examples/01-carapp/carapp/apps/car/views/cat/list.html
--rw-r--r--   0        0        0    15257 2023-05-29 23:22:51.646828 ellar-0.4.0/examples/01-carapp/carapp/apps/car/views/index.html
--rw-r--r--   0        0        0      216 2023-05-29 23:22:51.646828 ellar-0.4.0/examples/01-carapp/carapp/commands.py
--rw-r--r--   0        0        0      187 2023-05-29 23:22:51.646828 ellar-0.4.0/examples/01-carapp/carapp/config.py
--rw-r--r--   0        0        0      598 2023-05-29 23:22:51.646828 ellar-0.4.0/examples/01-carapp/carapp/root_module.py
--rw-r--r--   0        0        0      954 2023-05-29 23:22:51.646828 ellar-0.4.0/examples/01-carapp/carapp/server.py
--rw-r--r--   0        0        0      134 2023-05-29 23:22:51.646828 ellar-0.4.0/examples/01-carapp/carapp/tests/conftest.py
--rw-r--r--   0        0        0      241 2023-05-29 23:22:51.646828 ellar-0.4.0/examples/01-carapp/pyproject.toml
--rw-r--r--   0        0        0      264 2023-05-29 23:22:51.646828 ellar-0.4.0/examples/02-socketio-app/README.md
--rw-r--r--   0        0        0      283 2023-05-29 23:22:51.646828 ellar-0.4.0/examples/02-socketio-app/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-29 23:22:51.646828 ellar-0.4.0/examples/02-socketio-app/socketio_app/__init__.py
--rw-r--r--   0        0        0        0 2023-05-29 23:22:51.646828 ellar-0.4.0/examples/02-socketio-app/socketio_app/apps/__init__.py
--rw-r--r--   0        0        0        0 2023-05-29 23:22:51.646828 ellar-0.4.0/examples/02-socketio-app/socketio_app/apps/events/__init__.py
--rw-r--r--   0        0        0      455 2023-05-29 23:22:51.646828 ellar-0.4.0/examples/02-socketio-app/socketio_app/apps/events/controllers.py
--rw-r--r--   0        0        0     2182 2023-05-29 23:22:51.646828 ellar-0.4.0/examples/02-socketio-app/socketio_app/apps/events/gateways.py
--rw-r--r--   0        0        0     1005 2023-05-29 23:22:51.646828 ellar-0.4.0/examples/02-socketio-app/socketio_app/apps/events/module.py
--rw-r--r--   0        0        0      295 2023-05-29 23:22:51.646828 ellar-0.4.0/examples/02-socketio-app/socketio_app/apps/events/routers.py
--rw-r--r--   0        0        0      542 2023-05-29 23:22:51.646828 ellar-0.4.0/examples/02-socketio-app/socketio_app/apps/events/schemas.py
--rw-r--r--   0        0        0      179 2023-05-29 23:22:51.646828 ellar-0.4.0/examples/02-socketio-app/socketio_app/apps/events/services.py
--rw-r--r--   0        0        0     3829 2023-05-29 23:22:51.646828 ellar-0.4.0/examples/02-socketio-app/socketio_app/apps/events/templates/events/index.html
--rw-r--r--   0        0        0        0 2023-05-29 23:22:51.646828 ellar-0.4.0/examples/02-socketio-app/socketio_app/apps/events/tests/test_controllers.py
--rw-r--r--   0        0        0        0 2023-05-29 23:22:51.646828 ellar-0.4.0/examples/02-socketio-app/socketio_app/apps/events/tests/test_routers.py
--rw-r--r--   0        0        0        0 2023-05-29 23:22:51.646828 ellar-0.4.0/examples/02-socketio-app/socketio_app/apps/events/tests/test_services.py
--rw-r--r--   0        0        0     2602 2023-05-29 23:22:51.646828 ellar-0.4.0/examples/02-socketio-app/socketio_app/config.py
--rw-r--r--   0        0        0        0 2023-05-29 23:22:51.646828 ellar-0.4.0/examples/02-socketio-app/socketio_app/core/__init__.py
--rw-r--r--   0        0        0        0 2023-05-29 23:22:51.646828 ellar-0.4.0/examples/02-socketio-app/socketio_app/domain/__init__.py
--rw-r--r--   0        0        0      480 2023-05-29 23:22:51.646828 ellar-0.4.0/examples/02-socketio-app/socketio_app/root_module.py
--rw-r--r--   0        0        0     1045 2023-05-29 23:22:51.646828 ellar-0.4.0/examples/02-socketio-app/socketio_app/server.py
--rw-r--r--   0        0        0       43 2023-05-29 23:22:51.646828 ellar-0.4.0/examples/02-socketio-app/tests/conftest.py
--rw-r--r--   0        0        0     3872 2023-05-29 23:22:51.646828 ellar-0.4.0/mkdocs.yml
--rw-r--r--   0        0        0      597 2023-05-29 23:22:51.646828 ellar-0.4.0/mypy.ini
--rw-r--r--   0        0        0     3037 2023-05-29 23:22:51.646828 ellar-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      207 2023-05-29 23:22:51.646828 ellar-0.4.0/pytest.ini
--rw-r--r--   0        0        0        0 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/__init__.py
--rw-r--r--   0        0        0     1022 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/conftest.py
--rw-r--r--   0        0        0      616 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/injector_module.py
--rw-r--r--   0        0        0     5249 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/main.py
--rw-r--r--   0        0        0       23 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/private/test.css
--rw-r--r--   0        0        0      748 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/schema.py
--rw-r--r--   0        0        0        4 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/statics/example.txt
--rw-r--r--   0        0        0      160 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/templates/ellar/index.html
--rw-r--r--   0        0        0      102 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/templates/ellar/list.html
--rw-r--r--   0        0        0      129 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/templates/index.html
--rw-r--r--   0        0        0      128 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/templates/list.html
--rw-r--r--   0        0        0       65 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/templates/render_string.html
--rw-r--r--   0        0        0        0 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_application/__init__.py
--rw-r--r--   0        0        0       84 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_application/config.py
--rw-r--r--   0        0        0     2854 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_application/sample.py
--rw-r--r--   0        0        0     3548 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_application/test_application_factory.py
--rw-r--r--   0        0        0    15855 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_application/test_application_functions.py
--rw-r--r--   0        0        0    18052 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_application/test_cors.py
--rw-r--r--   0        0        0     4352 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_application/test_replacing_app_services.py
--rw-r--r--   0        0        0     2329 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_application/test_trusted_host.py
--rw-r--r--   0        0        0      862 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_attribute_dict.py
--rw-r--r--   0        0        0        0 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_cache/__init__.py
--rw-r--r--   0        0        0     3625 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_cache/_test_aio_memcache.py.ellar
--rw-r--r--   0        0        0     1893 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_cache/pylib_mock.py
--rw-r--r--   0        0        0     2592 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_cache/redis_mock.py
--rw-r--r--   0        0        0     2764 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_cache/test_cache_decorator.py
--rw-r--r--   0        0        0     1744 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_cache/test_cache_many_config.py
--rw-r--r--   0        0        0     4772 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_cache/test_cache_service.py
--rw-r--r--   0        0        0     4995 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_cache/test_local_cache.py
--rw-r--r--   0        0        0      596 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_cache/test_module_setup.py
--rw-r--r--   0        0        0     9973 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_cache/test_pylibmc_cache.py
--rw-r--r--   0        0        0     6093 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_cache/test_redis_cache.py
--rw-r--r--   0        0        0      577 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_cache/test_schema.py
--rw-r--r--   0        0        0        0 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_conf/__init__.py
--rw-r--r--   0        0        0     5223 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_conf/test_default_conf.py
--rw-r--r--   0        0        0     1151 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_conf/test_mixins.py
--rw-r--r--   0        0        0        0 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_controller/__init__.py
--rw-r--r--   0        0        0      387 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_controller/sample.py
--rw-r--r--   0        0        0        0 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_controller/test_application_router.py
--rw-r--r--   0        0        0     4448 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_controller/test_controller_decorator.py
--rw-r--r--   0        0        0     2872 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_controller/test_controller_inheritance.py
--rw-r--r--   0        0        0     2722 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_controller/test_module_router.py
--rw-r--r--   0        0        0     7186 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_controller/test_route_collection.py
--rw-r--r--   0        0        0        0 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_decorators/__init__.py
--rw-r--r--   0        0        0     3366 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_decorators/test_controller.py
--rw-r--r--   0        0        0      789 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_decorators/test_exception.py
--rw-r--r--   0        0        0     3508 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_decorators/test_file.py
--rw-r--r--   0        0        0     1059 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_decorators/test_guards.py
--rw-r--r--   0        0        0     4082 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_decorators/test_html.py
--rw-r--r--   0        0        0      554 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_decorators/test_middleware.py
--rw-r--r--   0        0        0     2061 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_decorators/test_modules.py
--rw-r--r--   0        0        0      915 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_decorators/test_openapi.py
--rw-r--r--   0        0        0     1311 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_decorators/test_serializer.py
--rw-r--r--   0        0        0      475 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_decorators/test_versioning.py
--rw-r--r--   0        0        0        0 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_di/__init__.py
--rw-r--r--   0        0        0     1332 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_di/examples.py
--rw-r--r--   0        0        0     2078 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_di/test_injectable_resolving.py
--rw-r--r--   0        0        0     6275 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_di/test_injector.py
--rw-r--r--   0        0        0     3508 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_di/test_provider_scopes.py
--rw-r--r--   0        0        0     3993 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_di/test_providers.py
--rw-r--r--   0        0        0     2094 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_events.py
--rw-r--r--   0        0        0        0 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_exceptions/__init__.py
--rw-r--r--   0        0        0      206 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_exceptions/exception_runner.py
--rw-r--r--   0        0        0     2562 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_exceptions/test_api_exception.py
--rw-r--r--   0        0        0     8609 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_exceptions/test_custom_exceptions.py
--rw-r--r--   0        0        0     1195 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_exceptions/test_error_details.py
--rw-r--r--   0        0        0     3722 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_exceptions/test_validation_exception.py
--rw-r--r--   0        0        0     7585 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_guard.py
--rw-r--r--   0        0        0        0 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_helper/__init__.py
--rw-r--r--   0        0        0      571 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_helper/test_enum.py
--rw-r--r--   0        0        0        0 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_helper/test_importer.py
--rw-r--r--   0        0        0      795 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_helper/test_model_field.py
--rw-r--r--   0        0        0      298 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_helper/test_module_loading.py
--rw-r--r--   0        0        0        0 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_interceptors/__init__.py
--rw-r--r--   0        0        0     2945 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_interceptors/test_interceptor.py
--rw-r--r--   0        0        0        0 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_middleware/__init__.py
--rw-r--r--   0        0        0     3100 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_middleware/test_functional_middleware.py
--rw-r--r--   0        0        0     4243 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_middleware/test_service_provider_middleware.py
--rw-r--r--   0        0        0     2168 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_middleware/test_versioning_middleware.py
--rw-r--r--   0        0        0        0 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_modules/__init__.py
--rw-r--r--   0        0        0     1847 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_modules/sample.py
--rw-r--r--   0        0        0     6760 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_modules/test_module_config.py
--rw-r--r--   0        0        0    10234 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_modules/test_module_ref.py
--rw-r--r--   0        0        0        0 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_openapi/__init__.py
--rw-r--r--   0        0        0     8341 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_openapi/test_builder.py
--rw-r--r--   0        0        0     6680 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_openapi/test_module.py
--rw-r--r--   0        0        0    16536 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_openapi/test_open_api_route_documentation.py
--rw-r--r--   0        0        0     5571 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_reflect.py
--rw-r--r--   0        0        0     2287 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_reflector.py
--rw-r--r--   0        0        0        0 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_response/__init__.py
--rw-r--r--   0        0        0     2486 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_response/test_defined_response_model.py
--rw-r--r--   0        0        0     4562 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_response/test_pydantic_response_model.py
--rw-r--r--   0        0        0     3393 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_response/test_response_file.py
--rw-r--r--   0        0        0     5063 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_response/test_response_html.py
--rw-r--r--   0        0        0     3228 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_response/test_response_streaming.py
--rw-r--r--   0        0        0     3902 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_response/test_response_type_definition_converter.py
--rw-r--r--   0        0        0     3524 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_response/test_route_response_model.py
--rw-r--r--   0        0        0        0 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_routing/__init__.py
--rw-r--r--   0        0        0     1126 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_routing/sample.py
--rw-r--r--   0        0        0     2757 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_routing/test_background_tasks.py
--rw-r--r--   0        0        0     3605 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_routing/test_body_schema.py
--rw-r--r--   0        0        0     3666 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_routing/test_body_schema_extra_properties.py
--rw-r--r--   0        0        0     4142 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_routing/test_body_union_schema.py
--rw-r--r--   0        0        0     4066 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_routing/test_cookie_schema.py
--rw-r--r--   0        0        0     6854 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_routing/test_extra_args.py
--rw-r--r--   0        0        0     2457 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_routing/test_form_schema.py
--rw-r--r--   0        0        0    10018 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_routing/test_formparsers.py
--rw-r--r--   0        0        0     1282 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_routing/test_forms.py
--rw-r--r--   0        0        0     1296 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_routing/test_forms_from_non_typing_sequences.py
--rw-r--r--   0        0        0     3633 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_routing/test_header_schema.py
--rw-r--r--   0        0        0     1887 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_routing/test_invalid_path_param.py
--rw-r--r--   0        0        0     2006 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_routing/test_invalid_sequence_param.py
--rw-r--r--   0        0        0     5205 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_routing/test_multi_body_errors.py
--rw-r--r--   0        0        0     3783 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_routing/test_multi_query_errors.py
--rw-r--r--   0        0        0     9423 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_routing/test_path.py
--rw-r--r--   0        0        0     2933 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_routing/test_path_with_schema.py
--rw-r--r--   0        0        0     3333 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_routing/test_put_with_no_body_schema.py
--rw-r--r--   0        0        0     2242 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_routing/test_query.py
--rw-r--r--   0        0        0     3699 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_routing/test_query_schema.py
--rw-r--r--   0        0        0     1987 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_routing/test_request.py
--rw-r--r--   0        0        0     3415 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_routing/test_route_endpoint_params.py
--rw-r--r--   0        0        0      451 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_sample_project.py
--rw-r--r--   0        0        0     2712 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_schema.py
--rw-r--r--   0        0        0     6379 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_serializer.py
--rw-r--r--   0        0        0      775 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_shortcuts.py
--rw-r--r--   0        0        0        0 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_socket_io/__init__.py
--rw-r--r--   0        0        0     4116 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_socket_io/sample.py
--rw-r--r--   0        0        0      718 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_socket_io/test_decorators/test_events.py
--rw-r--r--   0        0        0     3598 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_socket_io/test_decorators/test_gateway.py
--rw-r--r--   0        0        0      719 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_socket_io/test_decorators/test_subcribe_message.py
--rw-r--r--   0        0        0      859 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_socket_io/test_gateway.py
--rw-r--r--   0        0        0     8889 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_socket_io/test_operation.py
--rw-r--r--   0        0        0    14104 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_staticfiles.py
--rw-r--r--   0        0        0        0 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_templating/__init__.py
--rw-r--r--   0        0        0        0 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_templating/module_statics/watever.txt
--rw-r--r--   0        0        0        0 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_templating/static/watever.txt
--rw-r--r--   0        0        0      167 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_templating/templates/watever.html
--rw-r--r--   0        0        0     2904 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_templating/test_module_templating.py
--rw-r--r--   0        0        0     2718 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_templating/test_renderer.py
--rw-r--r--   0        0        0        0 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_templating/views/watever.html
--rw-r--r--   0        0        0     2425 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_testing.py
--rw-r--r--   0        0        0        0 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_versioning/__init__.py
--rw-r--r--   0        0        0     1968 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_versioning/operations.py
--rw-r--r--   0        0        0     2138 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_versioning/test_default_versioning.py
--rw-r--r--   0        0        0     4449 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_versioning/test_default_versioning_for_controllers.py
--rw-r--r--   0        0        0     4475 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_versioning/test_header_versioning.py
--rw-r--r--   0        0        0     7820 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_versioning/test_header_versioning_controller.py
--rw-r--r--   0        0        0     3823 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_versioning/test_host_versioning.py
--rw-r--r--   0        0        0     3227 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_versioning/test_query_versioning.py
--rw-r--r--   0        0        0     2865 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_versioning/test_url_versioning.py
--rw-r--r--   0        0        0    17496 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_websocket.py
--rw-r--r--   0        0        0    11181 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_websocket_handler.py
--rw-r--r--   0        0        0    14698 1970-01-01 00:00:00.000000 ellar-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      270 2023-06-09 10:14:33.613593 ellar-0.4.2/.coveragerc
+-rw-r--r--   0        0        0       65 2023-06-09 10:14:33.613593 ellar-0.4.2/.dockerignore
+-rw-r--r--   0        0        0      146 2023-06-09 10:14:33.613593 ellar-0.4.2/.flake8
+-rw-r--r--   0        0        0      205 2023-06-09 10:14:33.613593 ellar-0.4.2/.github/dependabot.yml
+-rw-r--r--   0        0        0      635 2023-06-09 10:14:33.613593 ellar-0.4.2/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      545 2023-06-09 10:14:33.613593 ellar-0.4.2/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1122 2023-06-09 10:14:33.613593 ellar-0.4.2/.github/workflows/test_full.yml
+-rw-r--r--   0        0        0     1891 2023-06-09 10:14:33.613593 ellar-0.4.2/.gitignore
+-rw-r--r--   0        0        0       53 2023-06-09 10:14:33.613593 ellar-0.4.2/.isort.cfg
+-rw-r--r--   0        0        0     1073 2023-06-09 10:14:33.613593 ellar-0.4.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1083 2023-06-09 10:14:33.613593 ellar-0.4.2/LICENSE
+-rw-r--r--   0        0        0     1166 2023-06-09 10:14:33.613593 ellar-0.4.2/Makefile
+-rw-r--r--   0        0        0    10596 2023-06-09 10:14:33.613593 ellar-0.4.2/README.md
+-rw-r--r--   0        0        0       15 2023-06-09 10:14:33.613593 ellar-0.4.2/docs/basics/api-docs.md
+-rw-r--r--   0        0        0     6367 2023-06-09 10:14:33.613593 ellar-0.4.2/docs/basics/dynamic-modules.md
+-rw-r--r--   0        0        0    10690 2023-06-09 10:14:33.613593 ellar-0.4.2/docs/basics/execution-context.md
+-rw-r--r--   0        0        0        0 2023-06-09 10:14:33.613593 ellar-0.4.2/docs/basics/file-streaming.md
+-rw-r--r--   0        0        0     2852 2023-06-09 10:14:33.613593 ellar-0.4.2/docs/basics/injector-scopes.md
+-rw-r--r--   0        0        0     3252 2023-06-09 10:14:33.613593 ellar-0.4.2/docs/basics/lifespan.md
+-rw-r--r--   0        0        0        0 2023-06-09 10:14:33.613593 ellar-0.4.2/docs/basics/model-view-controller.md
+-rw-r--r--   0        0        0    14869 2023-06-09 10:14:33.613593 ellar-0.4.2/docs/basics/testing.md
+-rw-r--r--   0        0        0     1177 2023-06-09 10:14:33.613593 ellar-0.4.2/docs/cli/command-grouping.md
+-rw-r--r--   0        0        0     6586 2023-06-09 10:14:33.613593 ellar-0.4.2/docs/cli/create-module-command.md
+-rw-r--r--   0        0        0      388 2023-06-09 10:14:33.613593 ellar-0.4.2/docs/cli/create-project-command.md
+-rw-r--r--   0        0        0     2755 2023-06-09 10:14:33.613593 ellar-0.4.2/docs/cli/custom-commands.md
+-rw-r--r--   0        0        0     1340 2023-06-09 10:14:33.613593 ellar-0.4.2/docs/cli/index.md
+-rw-r--r--   0        0        0     1206 2023-06-09 10:14:33.613593 ellar-0.4.2/docs/cli/new-command.md
+-rw-r--r--   0        0        0      803 2023-06-09 10:14:33.613593 ellar-0.4.2/docs/cli/runserver-command.md
+-rw-r--r--   0        0        0       14 2023-06-09 10:14:33.613593 ellar-0.4.2/docs/contribution.md
+-rw-r--r--   0        0        0     1765 2023-06-09 10:14:33.613593 ellar-0.4.2/docs/custom-setup.md
+-rwxr-xr-x   0        0        0    25915 2023-06-09 10:14:33.613593 ellar-0.4.2/docs/img/EllarLogoB.png
+-rwxr-xr-x   0        0        0    36744 2023-06-09 10:14:33.617593 ellar-0.4.2/docs/img/EllarLogoIconOnly.png
+-rwxr-xr-x   0        0        0    26456 2023-06-09 10:14:33.617593 ellar-0.4.2/docs/img/EllarLogoW.png
+-rwxr-xr-x   0        0        0     3888 2023-06-09 10:14:33.617593 ellar-0.4.2/docs/img/Icon.svg
+-rwxr-xr-x   0        0        0     4781 2023-06-09 10:14:33.617593 ellar-0.4.2/docs/img/Logo.svg
+-rw-r--r--   0        0        0    92094 2023-06-09 10:14:33.617593 ellar-0.4.2/docs/img/ModuleDescription.png
+-rw-r--r--   0        0        0    71483 2023-06-09 10:14:33.617593 ellar-0.4.2/docs/img/body-schema-doc.png
+-rw-r--r--   0        0        0   233058 2023-06-09 10:14:33.617593 ellar-0.4.2/docs/img/body-schema-doc2.png
+-rw-r--r--   0        0        0   196608 2023-06-09 10:14:33.617593 ellar-0.4.2/docs/img/body-schema-doc3.png
+-rwxr-xr-x   0        0        0    54689 2023-06-09 10:14:33.621593 ellar-0.4.2/docs/img/car_api.png
+-rw-r--r--   0        0        0  1632661 2023-06-09 10:14:33.629593 ellar-0.4.2/docs/img/car_controller.gif
+-rw-r--r--   0        0        0    50364 2023-06-09 10:14:33.629593 ellar-0.4.2/docs/img/controller_description.png
+-rw-r--r--   0        0        0    45273 2023-06-09 10:14:33.629593 ellar-0.4.2/docs/img/create-car-schema.png
+-rw-r--r--   0        0        0    19519 2023-06-09 10:14:33.629593 ellar-0.4.2/docs/img/create-dog-schema.png
+-rwxr-xr-x   0        0        0  1326350 2023-06-09 10:14:33.637593 ellar-0.4.2/docs/img/ellar_demo.gif
+-rwxr-xr-x   0        0        0    69977 2023-06-09 10:14:33.641593 ellar-0.4.2/docs/img/ellar_framework.png
+-rw-r--r--   0        0        0   244178 2023-06-09 10:14:33.641593 ellar-0.4.2/docs/img/enum_docs_swagger.png
+-rw-r--r--   0        0        0   168505 2023-06-09 10:14:33.641593 ellar-0.4.2/docs/img/event_docs_swagger.png
+-rw-r--r--   0        0        0   253271 2023-06-09 10:14:33.641593 ellar-0.4.2/docs/img/form-schema-doc.png
+-rw-r--r--   0        0        0   170683 2023-06-09 10:14:33.645593 ellar-0.4.2/docs/img/json_api_response_model.png
+-rw-r--r--   0        0        0    71548 2023-06-09 10:14:33.645593 ellar-0.4.2/docs/img/live_support_websocket.gif
+-rw-r--r--   0        0        0   121361 2023-06-09 10:14:33.645593 ellar-0.4.2/docs/img/live_support_websocket_3.gif
+-rw-r--r--   0        0        0   216500 2023-06-09 10:14:33.645593 ellar-0.4.2/docs/img/math_router.png
+-rw-r--r--   0        0        0   280669 2023-06-09 10:14:33.649593 ellar-0.4.2/docs/img/math_router_with_request_object.png
+-rw-r--r--   0        0        0    52280 2023-06-09 10:14:33.649593 ellar-0.4.2/docs/img/middleware.png
+-rw-r--r--   0        0        0   267982 2023-06-09 10:14:33.649593 ellar-0.4.2/docs/img/query_filter_swagger.png
+-rw-r--r--   0        0        0   208787 2023-06-09 10:14:33.649593 ellar-0.4.2/docs/img/response_description.png
+-rw-r--r--   0        0        0     4464 2023-06-09 10:14:33.649593 ellar-0.4.2/docs/index.md
+-rw-r--r--   0        0        0    12559 2023-06-09 10:14:33.653593 ellar-0.4.2/docs/overview/controllers.md
+-rw-r--r--   0        0        0    22647 2023-06-09 10:14:33.653593 ellar-0.4.2/docs/overview/custom_decorators.md
+-rw-r--r--   0        0        0     8031 2023-06-09 10:14:33.653593 ellar-0.4.2/docs/overview/exception_handling.md
+-rw-r--r--   0        0        0     8976 2023-06-09 10:14:33.653593 ellar-0.4.2/docs/overview/guards.md
+-rw-r--r--   0        0        0     7780 2023-06-09 10:14:33.653593 ellar-0.4.2/docs/overview/index.md
+-rw-r--r--   0        0        0     6559 2023-06-09 10:14:33.653593 ellar-0.4.2/docs/overview/interceptors.md
+-rw-r--r--   0        0        0     9377 2023-06-09 10:14:33.653593 ellar-0.4.2/docs/overview/middleware.md
+-rw-r--r--   0        0        0     4501 2023-06-09 10:14:33.653593 ellar-0.4.2/docs/overview/module-router.md
+-rw-r--r--   0        0        0     9117 2023-06-09 10:14:33.653593 ellar-0.4.2/docs/overview/modules.md
+-rw-r--r--   0        0        0     6683 2023-06-09 10:14:33.653593 ellar-0.4.2/docs/overview/providers.md
+-rw-r--r--   0        0        0        0 2023-06-09 10:14:33.653593 ellar-0.4.2/docs/release-notes.md
+-rw-r--r--   0        0        0       14 2023-06-09 10:14:33.653593 ellar-0.4.2/docs/security/authentication.md
+-rw-r--r--   0        0        0       14 2023-06-09 10:14:33.653593 ellar-0.4.2/docs/security/authorization.md
+-rw-r--r--   0        0        0       14 2023-06-09 10:14:33.653593 ellar-0.4.2/docs/security/csrf.md
+-rw-r--r--   0        0        0       14 2023-06-09 10:14:33.653593 ellar-0.4.2/docs/security/sessions.md
+-rw-r--r--   0        0        0     7385 2023-06-09 10:14:33.653593 ellar-0.4.2/docs/security/throttling.md
+-rw-r--r--   0        0        0       69 2023-06-09 10:14:33.653593 ellar-0.4.2/docs/stylesheets/extra.css
+-rw-r--r--   0        0        0     2279 2023-06-09 10:14:33.653593 ellar-0.4.2/docs/techniques/background-task.md
+-rw-r--r--   0        0        0    21194 2023-06-09 10:14:33.653593 ellar-0.4.2/docs/techniques/caching.md
+-rw-r--r--   0        0        0    10775 2023-06-09 10:14:33.653593 ellar-0.4.2/docs/techniques/configurations.md
+-rw-r--r--   0        0        0     2028 2023-06-09 10:14:33.653593 ellar-0.4.2/docs/techniques/mount.md
+-rw-r--r--   0        0        0     6541 2023-06-09 10:14:33.653593 ellar-0.4.2/docs/techniques/response-model.md
+-rw-r--r--   0        0        0     6590 2023-06-09 10:14:33.653593 ellar-0.4.2/docs/techniques/serializers.md
+-rw-r--r--   0        0        0     4130 2023-06-09 10:14:33.653593 ellar-0.4.2/docs/techniques/staticfiles.md
+-rw-r--r--   0        0        0    13755 2023-06-09 10:14:33.653593 ellar-0.4.2/docs/techniques/templating.md
+-rw-r--r--   0        0        0     8919 2023-06-09 10:14:33.653593 ellar-0.4.2/docs/techniques/validations/body.md
+-rw-r--r--   0        0        0     1386 2023-06-09 10:14:33.653593 ellar-0.4.2/docs/techniques/validations/cookie-params.md
+-rw-r--r--   0        0        0     6612 2023-06-09 10:14:33.653593 ellar-0.4.2/docs/techniques/validations/file-params.md
+-rw-r--r--   0        0        0     4116 2023-06-09 10:14:33.653593 ellar-0.4.2/docs/techniques/validations/form-params.md
+-rw-r--r--   0        0        0     3818 2023-06-09 10:14:33.653593 ellar-0.4.2/docs/techniques/validations/header-params.md
+-rw-r--r--   0        0        0     1588 2023-06-09 10:14:33.653593 ellar-0.4.2/docs/techniques/validations/index.md
+-rw-r--r--   0        0        0     6772 2023-06-09 10:14:33.653593 ellar-0.4.2/docs/techniques/validations/path-params.md
+-rw-r--r--   0        0        0     4936 2023-06-09 10:14:33.653593 ellar-0.4.2/docs/techniques/validations/query-params.md
+-rw-r--r--   0        0        0     7891 2023-06-09 10:14:33.653593 ellar-0.4.2/docs/techniques/versioning.md
+-rw-r--r--   0        0        0    12692 2023-06-09 10:14:33.653593 ellar-0.4.2/docs/websockets/index.md
+-rw-r--r--   0        0        0    12912 2023-06-09 10:14:33.653593 ellar-0.4.2/docs/websockets/socketio.md
+-rw-r--r--   0        0        0      143 2023-06-09 10:14:33.653593 ellar-0.4.2/ellar/__init__.py
+-rw-r--r--   0        0        0      257 2023-06-09 10:14:33.653593 ellar-0.4.2/ellar/cache/__init__.py
+-rw-r--r--   0        0        0      109 2023-06-09 10:14:33.653593 ellar-0.4.2/ellar/cache/backends/__init__.py
+-rw-r--r--   0        0        0     4841 2023-06-09 10:14:33.653593 ellar-0.4.2/ellar/cache/backends/_aio_cache.py.ellar
+-rw-r--r--   0        0        0     4361 2023-06-09 10:14:33.653593 ellar-0.4.2/ellar/cache/backends/base.py
+-rw-r--r--   0        0        0     5145 2023-06-09 10:14:33.653593 ellar-0.4.2/ellar/cache/backends/local_cache.py
+-rw-r--r--   0        0        0      944 2023-06-09 10:14:33.653593 ellar-0.4.2/ellar/cache/backends/pylib_cache.py
+-rw-r--r--   0        0        0     2215 2023-06-09 10:14:33.653593 ellar-0.4.2/ellar/cache/backends/pymem_cache.py
+-rw-r--r--   0        0        0       72 2023-06-09 10:14:33.653593 ellar-0.4.2/ellar/cache/backends/redis/__init__.py
+-rw-r--r--   0        0        0     6548 2023-06-09 10:14:33.653593 ellar-0.4.2/ellar/cache/backends/redis/backend.py
+-rw-r--r--   0        0        0     1397 2023-06-09 10:14:33.653593 ellar-0.4.2/ellar/cache/backends/serializer.py
+-rw-r--r--   0        0        0     2923 2023-06-09 10:14:33.653593 ellar-0.4.2/ellar/cache/decorator.py
+-rw-r--r--   0        0        0    10943 2023-06-09 10:14:33.653593 ellar-0.4.2/ellar/cache/interface.py
+-rw-r--r--   0        0        0     2027 2023-06-09 10:14:33.653593 ellar-0.4.2/ellar/cache/make_key_decorator.py
+-rw-r--r--   0        0        0     2501 2023-06-09 10:14:33.653593 ellar-0.4.2/ellar/cache/model.py
+-rw-r--r--   0        0        0     1859 2023-06-09 10:14:33.653593 ellar-0.4.2/ellar/cache/module.py
+-rw-r--r--   0        0        0      852 2023-06-09 10:14:33.653593 ellar-0.4.2/ellar/cache/schema.py
+-rw-r--r--   0        0        0     4489 2023-06-09 10:14:33.653593 ellar-0.4.2/ellar/cache/service.py
+-rw-r--r--   0        0        0     4064 2023-06-09 10:14:33.653593 ellar-0.4.2/ellar/common/__init__.py
+-rw-r--r--   0        0        0      108 2023-06-09 10:14:33.653593 ellar-0.4.2/ellar/common/commands/__init__.py
+-rw-r--r--   0        0        0     2254 2023-06-09 10:14:33.653593 ellar-0.4.2/ellar/common/commands/base.py
+-rw-r--r--   0        0        0     1537 2023-06-09 10:14:33.653593 ellar-0.4.2/ellar/common/commands/decorator.py
+-rw-r--r--   0        0        0      270 2023-06-09 10:14:33.653593 ellar-0.4.2/ellar/common/compatible/__init__.py
+-rw-r--r--   0        0        0     1166 2023-06-09 10:14:33.653593 ellar-0.4.2/ellar/common/compatible/cache_properties.py
+-rw-r--r--   0        0        0     1511 2023-06-09 10:14:33.653593 ellar-0.4.2/ellar/common/compatible/dict.py
+-rw-r--r--   0        0        0      637 2023-06-09 10:14:33.653593 ellar-0.4.2/ellar/common/compatible/emails.py
+-rw-r--r--   0        0        0     4768 2023-06-09 10:14:33.653593 ellar-0.4.2/ellar/common/constants.py
+-rw-r--r--   0        0        0     1670 2023-06-09 10:14:33.653593 ellar-0.4.2/ellar/common/converters.py
+-rw-r--r--   0        0        0      809 2023-06-09 10:14:33.653593 ellar-0.4.2/ellar/common/datastructures.py
+-rw-r--r--   0        0        0      865 2023-06-09 10:14:33.653593 ellar-0.4.2/ellar/common/decorators/__init__.py
+-rw-r--r--   0        0        0      485 2023-06-09 10:14:33.653593 ellar-0.4.2/ellar/common/decorators/base.py
+-rw-r--r--   0        0        0     7141 2023-06-09 10:14:33.653593 ellar-0.4.2/ellar/common/decorators/controller.py
+-rw-r--r--   0        0        0     1036 2023-06-09 10:14:33.653593 ellar-0.4.2/ellar/common/decorators/exception.py
+-rw-r--r--   0        0        0      610 2023-06-09 10:14:33.653593 ellar-0.4.2/ellar/common/decorators/extra_args.py
+-rw-r--r--   0        0        0     2528 2023-06-09 10:14:33.653593 ellar-0.4.2/ellar/common/decorators/file.py
+-rw-r--r--   0        0        0     1025 2023-06-09 10:14:33.653593 ellar-0.4.2/ellar/common/decorators/guards.py
+-rw-r--r--   0        0        0     4748 2023-06-09 10:14:33.653593 ellar-0.4.2/ellar/common/decorators/html.py
+-rw-r--r--   0        0        0     1084 2023-06-09 10:14:33.653593 ellar-0.4.2/ellar/common/decorators/interceptor.py
+-rw-r--r--   0        0        0      648 2023-06-09 10:14:33.653593 ellar-0.4.2/ellar/common/decorators/middleware.py
+-rw-r--r--   0        0        0     3105 2023-06-09 10:14:33.653593 ellar-0.4.2/ellar/common/decorators/modules.py
+-rw-r--r--   0        0        0      932 2023-06-09 10:14:33.653593 ellar-0.4.2/ellar/common/decorators/openapi.py
+-rw-r--r--   0        0        0     1295 2023-06-09 10:14:33.653593 ellar-0.4.2/ellar/common/decorators/serializer.py
+-rw-r--r--   0        0        0      402 2023-06-09 10:14:33.653593 ellar-0.4.2/ellar/common/decorators/versioning.py
+-rw-r--r--   0        0        0      840 2023-06-09 10:14:33.653593 ellar-0.4.2/ellar/common/exceptions/__init__.py
+-rw-r--r--   0        0        0      472 2023-06-09 10:14:33.653593 ellar-0.4.2/ellar/common/exceptions/api/__init__.py
+-rw-r--r--   0        0        0     1447 2023-06-09 10:14:33.653593 ellar-0.4.2/ellar/common/exceptions/api/base.py
+-rw-r--r--   0        0        0     1239 2023-06-09 10:14:33.653593 ellar-0.4.2/ellar/common/exceptions/api/exceptions_types.py
+-rw-r--r--   0        0        0     2498 2023-06-09 10:14:33.653593 ellar-0.4.2/ellar/common/exceptions/callable_exceptions.py
+-rw-r--r--   0        0        0      103 2023-06-09 10:14:33.653593 ellar-0.4.2/ellar/common/exceptions/context.py
+-rw-r--r--   0        0        0     2517 2023-06-09 10:14:33.657593 ellar-0.4.2/ellar/common/exceptions/handlers.py
+-rw-r--r--   0        0        0      598 2023-06-09 10:14:33.657593 ellar-0.4.2/ellar/common/exceptions/validation.py
+-rw-r--r--   0        0        0     1485 2023-06-09 10:14:33.657593 ellar-0.4.2/ellar/common/helper/__init__.py
+-rw-r--r--   0        0        0      658 2023-06-09 10:14:33.657593 ellar-0.4.2/ellar/common/helper/enums.py
+-rw-r--r--   0        0        0      389 2023-06-09 10:14:33.657593 ellar-0.4.2/ellar/common/helper/event_loop.py
+-rw-r--r--   0        0        0     2137 2023-06-09 10:14:33.657593 ellar-0.4.2/ellar/common/helper/importer.py
+-rw-r--r--   0        0        0     1272 2023-06-09 10:14:33.657593 ellar-0.4.2/ellar/common/helper/modelfield.py
+-rw-r--r--   0        0        0      703 2023-06-09 10:14:33.657593 ellar-0.4.2/ellar/common/helper/module_loading.py
+-rw-r--r--   0        0        0     1074 2023-06-09 10:14:33.657593 ellar-0.4.2/ellar/common/interfaces/__init__.py
+-rw-r--r--   0        0        0      399 2023-06-09 10:14:33.657593 ellar-0.4.2/ellar/common/interfaces/application.py
+-rw-r--r--   0        0        0     3560 2023-06-09 10:14:33.657593 ellar-0.4.2/ellar/common/interfaces/context.py
+-rw-r--r--   0        0        0      278 2023-06-09 10:14:33.657593 ellar-0.4.2/ellar/common/interfaces/controller_factory.py
+-rw-r--r--   0        0        0     1356 2023-06-09 10:14:33.657593 ellar-0.4.2/ellar/common/interfaces/exceptions.py
+-rw-r--r--   0        0        0      400 2023-06-09 10:14:33.657593 ellar-0.4.2/ellar/common/interfaces/guard_consumer.py
+-rw-r--r--   0        0        0      406 2023-06-09 10:14:33.657593 ellar-0.4.2/ellar/common/interfaces/interceptor_consumer.py
+-rw-r--r--   0        0        0     1771 2023-06-09 10:14:33.657593 ellar-0.4.2/ellar/common/interfaces/module.py
+-rw-r--r--   0        0        0      749 2023-06-09 10:14:33.657593 ellar-0.4.2/ellar/common/interfaces/response_model.py
+-rw-r--r--   0        0        0      908 2023-06-09 10:14:33.657593 ellar-0.4.2/ellar/common/interfaces/templating.py
+-rw-r--r--   0        0        0       52 2023-06-09 10:14:33.657593 ellar-0.4.2/ellar/common/logger.py
+-rw-r--r--   0        0        0      340 2023-06-09 10:14:33.657593 ellar-0.4.2/ellar/common/models/__init__.py
+-rw-r--r--   0        0        0      923 2023-06-09 10:14:33.657593 ellar-0.4.2/ellar/common/models/controller.py
+-rw-r--r--   0        0        0     4258 2023-06-09 10:14:33.657593 ellar-0.4.2/ellar/common/models/guard.py
+-rw-r--r--   0        0        0      320 2023-06-09 10:14:33.657593 ellar-0.4.2/ellar/common/models/interceptor.py
+-rw-r--r--   0        0        0      476 2023-06-09 10:14:33.657593 ellar-0.4.2/ellar/common/params/__init__.py
+-rw-r--r--   0        0        0      365 2023-06-09 10:14:33.657593 ellar-0.4.2/ellar/common/params/args/__init__.py
+-rw-r--r--   0        0        0    14227 2023-06-09 10:14:33.657593 ellar-0.4.2/ellar/common/params/args/base.py
+-rw-r--r--   0        0        0     1615 2023-06-09 10:14:33.657593 ellar-0.4.2/ellar/common/params/args/extra_args.py
+-rw-r--r--   0        0        0     2045 2023-06-09 10:14:33.657593 ellar-0.4.2/ellar/common/params/args/factory.py
+-rw-r--r--   0        0        0     4252 2023-06-09 10:14:33.657593 ellar-0.4.2/ellar/common/params/args/request_model.py
+-rw-r--r--   0        0        0     5893 2023-06-09 10:14:33.657593 ellar-0.4.2/ellar/common/params/args/resolver_generators.py
+-rw-r--r--   0        0        0     2457 2023-06-09 10:14:33.657593 ellar-0.4.2/ellar/common/params/args/websocket_model.py
+-rw-r--r--   0        0        0    10559 2023-06-09 10:14:33.657593 ellar-0.4.2/ellar/common/params/decorators.py
+-rw-r--r--   0        0        0     1235 2023-06-09 10:14:33.657593 ellar-0.4.2/ellar/common/params/helpers.py
+-rw-r--r--   0        0        0     9342 2023-06-09 10:14:33.657593 ellar-0.4.2/ellar/common/params/params.py
+-rw-r--r--   0        0        0     1083 2023-06-09 10:14:33.657593 ellar-0.4.2/ellar/common/params/resolvers/__init__.py
+-rw-r--r--   0        0        0     1678 2023-06-09 10:14:33.657593 ellar-0.4.2/ellar/common/params/resolvers/base.py
+-rw-r--r--   0        0        0     4460 2023-06-09 10:14:33.657593 ellar-0.4.2/ellar/common/params/resolvers/bulk_parameter.py
+-rw-r--r--   0        0        0      768 2023-06-09 10:14:33.657593 ellar-0.4.2/ellar/common/params/resolvers/non_parameter/__init__.py
+-rw-r--r--   0        0        0      868 2023-06-09 10:14:33.657593 ellar-0.4.2/ellar/common/params/resolvers/non_parameter/background.py
+-rw-r--r--   0        0        0     2961 2023-06-09 10:14:33.657593 ellar-0.4.2/ellar/common/params/resolvers/non_parameter/base.py
+-rw-r--r--   0        0        0      391 2023-06-09 10:14:33.657593 ellar-0.4.2/ellar/common/params/resolvers/non_parameter/connection.py
+-rw-r--r--   0        0        0      328 2023-06-09 10:14:33.657593 ellar-0.4.2/ellar/common/params/resolvers/non_parameter/context.py
+-rw-r--r--   0        0        0     1660 2023-06-09 10:14:33.657593 ellar-0.4.2/ellar/common/params/resolvers/non_parameter/inject.py
+-rw-r--r--   0        0        0      387 2023-06-09 10:14:33.657593 ellar-0.4.2/ellar/common/params/resolvers/non_parameter/request.py
+-rw-r--r--   0        0        0      394 2023-06-09 10:14:33.657593 ellar-0.4.2/ellar/common/params/resolvers/non_parameter/response.py
+-rw-r--r--   0        0        0      524 2023-06-09 10:14:33.657593 ellar-0.4.2/ellar/common/params/resolvers/non_parameter/session.py
+-rw-r--r--   0        0        0      386 2023-06-09 10:14:33.657593 ellar-0.4.2/ellar/common/params/resolvers/non_parameter/websocket.py
+-rw-r--r--   0        0        0     9544 2023-06-09 10:14:33.657593 ellar-0.4.2/ellar/common/params/resolvers/parameter.py
+-rw-r--r--   0        0        0      415 2023-06-09 10:14:33.657593 ellar-0.4.2/ellar/common/responses/__init__.py
+-rw-r--r--   0        0        0      925 2023-06-09 10:14:33.657593 ellar-0.4.2/ellar/common/responses/models/__init__.py
+-rw-r--r--   0        0        0     6157 2023-06-09 10:14:33.657593 ellar-0.4.2/ellar/common/responses/models/base.py
+-rw-r--r--   0        0        0       50 2023-06-09 10:14:33.657593 ellar-0.4.2/ellar/common/responses/models/exceptions.py
+-rw-r--r--   0        0        0     3129 2023-06-09 10:14:33.657593 ellar-0.4.2/ellar/common/responses/models/file.py
+-rw-r--r--   0        0        0      691 2023-06-09 10:14:33.657593 ellar-0.4.2/ellar/common/responses/models/helper.py
+-rw-r--r--   0        0        0     1952 2023-06-09 10:14:33.657593 ellar-0.4.2/ellar/common/responses/models/html.py
+-rw-r--r--   0        0        0     2383 2023-06-09 10:14:33.657593 ellar-0.4.2/ellar/common/responses/models/json.py
+-rw-r--r--   0        0        0     4392 2023-06-09 10:14:33.657593 ellar-0.4.2/ellar/common/responses/models/route.py
+-rw-r--r--   0        0        0     2167 2023-06-09 10:14:33.657593 ellar-0.4.2/ellar/common/responses/models/type_converter.py
+-rw-r--r--   0        0        0      995 2023-06-09 10:14:33.657593 ellar-0.4.2/ellar/common/responses/response_types.py
+-rw-r--r--   0        0        0     1249 2023-06-09 10:14:33.657593 ellar-0.4.2/ellar/common/routing/__init__.py
+-rw-r--r--   0        0        0     4511 2023-06-09 10:14:33.657593 ellar-0.4.2/ellar/common/routing/base.py
+-rw-r--r--   0        0        0      272 2023-06-09 10:14:33.657593 ellar-0.4.2/ellar/common/routing/controller/__init__.py
+-rw-r--r--   0        0        0      877 2023-06-09 10:14:33.657593 ellar-0.4.2/ellar/common/routing/controller/base.py
+-rw-r--r--   0        0        0      689 2023-06-09 10:14:33.657593 ellar-0.4.2/ellar/common/routing/controller/route.py
+-rw-r--r--   0        0        0      190 2023-06-09 10:14:33.657593 ellar-0.4.2/ellar/common/routing/controller/websocket/__init__.py
+-rw-r--r--   0        0        0     1424 2023-06-09 10:14:33.657593 ellar-0.4.2/ellar/common/routing/controller/websocket/handler.py
+-rw-r--r--   0        0        0     1260 2023-06-09 10:14:33.657593 ellar-0.4.2/ellar/common/routing/controller/websocket/route.py
+-rw-r--r--   0        0        0     6589 2023-06-09 10:14:33.657593 ellar-0.4.2/ellar/common/routing/mount.py
+-rw-r--r--   0        0        0    10048 2023-06-09 10:14:33.657593 ellar-0.4.2/ellar/common/routing/operation_definitions.py
+-rw-r--r--   0        0        0     4799 2023-06-09 10:14:33.657593 ellar-0.4.2/ellar/common/routing/route.py
+-rw-r--r--   0        0        0     2985 2023-06-09 10:14:33.657593 ellar-0.4.2/ellar/common/routing/route_collections.py
+-rw-r--r--   0        0        0     3689 2023-06-09 10:14:33.657593 ellar-0.4.2/ellar/common/routing/schema.py
+-rw-r--r--   0        0        0      161 2023-06-09 10:14:33.657593 ellar-0.4.2/ellar/common/routing/websocket/__init__.py
+-rw-r--r--   0        0        0     5680 2023-06-09 10:14:33.657593 ellar-0.4.2/ellar/common/routing/websocket/handler.py
+-rw-r--r--   0        0        0     5158 2023-06-09 10:14:33.657593 ellar-0.4.2/ellar/common/routing/websocket/route.py
+-rw-r--r--   0        0        0      499 2023-06-09 10:14:33.657593 ellar-0.4.2/ellar/common/serializer/__init__.py
+-rw-r--r--   0        0        0     4960 2023-06-09 10:14:33.657593 ellar-0.4.2/ellar/common/serializer/base.py
+-rw-r--r--   0        0        0      194 2023-06-09 10:14:33.657593 ellar-0.4.2/ellar/common/serializer/guard.py
+-rw-r--r--   0        0        0      453 2023-06-09 10:14:33.657593 ellar-0.4.2/ellar/common/shortcuts.py
+-rw-r--r--   0        0        0      613 2023-06-09 10:14:33.657593 ellar-0.4.2/ellar/common/templating/__init__.py
+-rw-r--r--   0        0        0      472 2023-06-09 10:14:33.657593 ellar-0.4.2/ellar/common/templating/environment.py
+-rw-r--r--   0        0        0     1634 2023-06-09 10:14:33.657593 ellar-0.4.2/ellar/common/templating/loader.py
+-rw-r--r--   0        0        0     2895 2023-06-09 10:14:33.657593 ellar-0.4.2/ellar/common/templating/model.py
+-rw-r--r--   0        0        0     2482 2023-06-09 10:14:33.657593 ellar-0.4.2/ellar/common/templating/renderer.py
+-rw-r--r--   0        0        0      110 2023-06-09 10:14:33.657593 ellar-0.4.2/ellar/common/templating/schema.py
+-rw-r--r--   0        0        0      585 2023-06-09 10:14:33.657593 ellar-0.4.2/ellar/common/types.py
+-rw-r--r--   0        0        0      925 2023-06-09 10:14:33.657593 ellar-0.4.2/ellar/core/__init__.py
+-rw-r--r--   0        0        0      120 2023-06-09 10:14:33.657593 ellar-0.4.2/ellar/core/conf/__init__.py
+-rw-r--r--   0        0        0     4914 2023-06-09 10:14:33.657593 ellar-0.4.2/ellar/core/conf/app_settings_models.py
+-rw-r--r--   0        0        0     2409 2023-06-09 10:14:33.657593 ellar-0.4.2/ellar/core/conf/config.py
+-rw-r--r--   0        0        0     5122 2023-06-09 10:14:33.657593 ellar-0.4.2/ellar/core/conf/mixins.py
+-rw-r--r--   0        0        0      470 2023-06-09 10:14:33.657593 ellar-0.4.2/ellar/core/connection/__init__.py
+-rw-r--r--   0        0        0      688 2023-06-09 10:14:33.657593 ellar-0.4.2/ellar/core/connection/http.py
+-rw-r--r--   0        0        0      245 2023-06-09 10:14:33.657593 ellar-0.4.2/ellar/core/connection/websocket.py
+-rw-r--r--   0        0        0      458 2023-06-09 10:14:33.657593 ellar-0.4.2/ellar/core/context/__init__.py
+-rw-r--r--   0        0        0     1315 2023-06-09 10:14:33.657593 ellar-0.4.2/ellar/core/context/execution.py
+-rw-r--r--   0        0        0     2607 2023-06-09 10:14:33.657593 ellar-0.4.2/ellar/core/context/factory.py
+-rw-r--r--   0        0        0     2091 2023-06-09 10:14:33.657593 ellar-0.4.2/ellar/core/context/host.py
+-rw-r--r--   0        0        0     2122 2023-06-09 10:14:33.657593 ellar-0.4.2/ellar/core/context/http.py
+-rw-r--r--   0        0        0      817 2023-06-09 10:14:33.657593 ellar-0.4.2/ellar/core/context/websocket.py
+-rw-r--r--   0        0        0     1829 2023-06-09 10:14:33.657593 ellar-0.4.2/ellar/core/core_service_registration.py
+-rw-r--r--   0        0        0       97 2023-06-09 10:14:33.657593 ellar-0.4.2/ellar/core/exceptions/__init__.py
+-rw-r--r--   0        0        0     2273 2023-06-09 10:14:33.657593 ellar-0.4.2/ellar/core/exceptions/service.py
+-rw-r--r--   0        0        0     7616 2023-06-09 10:14:33.657593 ellar-0.4.2/ellar/core/factory.py
+-rw-r--r--   0        0        0      320 2023-06-09 10:14:33.657593 ellar-0.4.2/ellar/core/guard/__init__.py
+-rw-r--r--   0        0        0      744 2023-06-09 10:14:33.657593 ellar-0.4.2/ellar/core/guard/apikey.py
+-rw-r--r--   0        0        0     1729 2023-06-09 10:14:33.657593 ellar-0.4.2/ellar/core/guard/consumer.py
+-rw-r--r--   0        0        0     3318 2023-06-09 10:14:33.657593 ellar-0.4.2/ellar/core/guard/http.py
+-rw-r--r--   0        0        0       87 2023-06-09 10:14:33.657593 ellar-0.4.2/ellar/core/interceptors/__init__.py
+-rw-r--r--   0        0        0     2083 2023-06-09 10:14:33.657593 ellar-0.4.2/ellar/core/interceptors/consumer.py
+-rw-r--r--   0        0        0     2027 2023-06-09 10:14:33.661593 ellar-0.4.2/ellar/core/lifespan.py
+-rw-r--r--   0        0        0    10088 2023-06-09 10:14:33.661593 ellar-0.4.2/ellar/core/main.py
+-rw-r--r--   0        0        0     1159 2023-06-09 10:14:33.661593 ellar-0.4.2/ellar/core/middleware/__init__.py
+-rw-r--r--   0        0        0     2600 2023-06-09 10:14:33.661593 ellar-0.4.2/ellar/core/middleware/di.py
+-rw-r--r--   0        0        0     2704 2023-06-09 10:14:33.661593 ellar-0.4.2/ellar/core/middleware/exceptions.py
+-rw-r--r--   0        0        0     2256 2023-06-09 10:14:33.661593 ellar-0.4.2/ellar/core/middleware/function.py
+-rw-r--r--   0        0        0      121 2023-06-09 10:14:33.661593 ellar-0.4.2/ellar/core/middleware/sessions.py
+-rw-r--r--   0        0        0     1095 2023-06-09 10:14:33.661593 ellar-0.4.2/ellar/core/middleware/versioning.py
+-rw-r--r--   0        0        0      321 2023-06-09 10:14:33.661593 ellar-0.4.2/ellar/core/modules/__init__.py
+-rw-r--r--   0        0        0     1287 2023-06-09 10:14:33.661593 ellar-0.4.2/ellar/core/modules/base.py
+-rw-r--r--   0        0        0     3143 2023-06-09 10:14:33.661593 ellar-0.4.2/ellar/core/modules/builder.py
+-rw-r--r--   0        0        0     5827 2023-06-09 10:14:33.661593 ellar-0.4.2/ellar/core/modules/config.py
+-rw-r--r--   0        0        0      787 2023-06-09 10:14:33.661593 ellar-0.4.2/ellar/core/modules/helper.py
+-rw-r--r--   0        0        0     9876 2023-06-09 10:14:33.661593 ellar-0.4.2/ellar/core/modules/ref.py
+-rw-r--r--   0        0        0      351 2023-06-09 10:14:33.661593 ellar-0.4.2/ellar/core/routing/__init__.py
+-rw-r--r--   0        0        0     3661 2023-06-09 10:14:33.661593 ellar-0.4.2/ellar/core/routing/app.py
+-rw-r--r--   0        0        0     1865 2023-06-09 10:14:33.661593 ellar-0.4.2/ellar/core/routing/builder.py
+-rw-r--r--   0        0        0     1862 2023-06-09 10:14:33.661593 ellar-0.4.2/ellar/core/routing/factory.py
+-rw-r--r--   0        0        0     1971 2023-06-09 10:14:33.661593 ellar-0.4.2/ellar/core/routing/helper.py
+-rw-r--r--   0        0        0      794 2023-06-09 10:14:33.661593 ellar-0.4.2/ellar/core/routing/module_router.py
+-rw-r--r--   0        0        0       58 2023-06-09 10:14:33.661593 ellar-0.4.2/ellar/core/services/__init__.py
+-rw-r--r--   0        0        0     1951 2023-06-09 10:14:33.661593 ellar-0.4.2/ellar/core/services/reflector.py
+-rw-r--r--   0        0        0     1718 2023-06-09 10:14:33.661593 ellar-0.4.2/ellar/core/staticfiles.py
+-rw-r--r--   0        0        0       67 2023-06-09 10:14:33.661593 ellar-0.4.2/ellar/core/templating/__init__.py
+-rw-r--r--   0        0        0     3978 2023-06-09 10:14:33.661593 ellar-0.4.2/ellar/core/templating/app.py
+-rw-r--r--   0        0        0      563 2023-06-09 10:14:33.661593 ellar-0.4.2/ellar/core/versioning/__init__.py
+-rw-r--r--   0        0        0     2526 2023-06-09 10:14:33.661593 ellar-0.4.2/ellar/core/versioning/base.py
+-rw-r--r--   0        0        0     6040 2023-06-09 10:14:33.661593 ellar-0.4.2/ellar/core/versioning/resolver.py
+-rw-r--r--   0        0        0      915 2023-06-09 10:14:33.661593 ellar-0.4.2/ellar/di/__init__.py
+-rw-r--r--   0        0        0      344 2023-06-09 10:14:33.661593 ellar-0.4.2/ellar/di/asgi_args.py
+-rw-r--r--   0        0        0     1073 2023-06-09 10:14:33.661593 ellar-0.4.2/ellar/di/constants.py
+-rw-r--r--   0        0        0      400 2023-06-09 10:14:33.661593 ellar-0.4.2/ellar/di/exceptions.py
+-rw-r--r--   0        0        0      117 2023-06-09 10:14:33.661593 ellar-0.4.2/ellar/di/injector/__init__.py
+-rw-r--r--   0        0        0     7568 2023-06-09 10:14:33.661593 ellar-0.4.2/ellar/di/injector/container.py
+-rw-r--r--   0        0        0     5268 2023-06-09 10:14:33.661593 ellar-0.4.2/ellar/di/injector/ellar_injector.py
+-rw-r--r--   0        0        0      845 2023-06-09 10:14:33.661593 ellar-0.4.2/ellar/di/providers.py
+-rw-r--r--   0        0        0     2247 2023-06-09 10:14:33.661593 ellar-0.4.2/ellar/di/scopes.py
+-rw-r--r--   0        0        0     4533 2023-06-09 10:14:33.661593 ellar-0.4.2/ellar/di/service_config.py
+-rw-r--r--   0        0        0       39 2023-06-09 10:14:33.661593 ellar-0.4.2/ellar/di/types.py
+-rw-r--r--   0        0        0      244 2023-06-09 10:14:33.661593 ellar-0.4.2/ellar/di/utils.py
+-rw-r--r--   0        0        0     2052 2023-06-09 10:14:33.661593 ellar-0.4.2/ellar/events.py
+-rw-r--r--   0        0        0      573 2023-06-09 10:14:33.661593 ellar-0.4.2/ellar/openapi/__init__.py
+-rw-r--r--   0        0        0     8069 2023-06-09 10:14:33.661593 ellar-0.4.2/ellar/openapi/builder.py
+-rw-r--r--   0        0        0      239 2023-06-09 10:14:33.661593 ellar-0.4.2/ellar/openapi/docs_generators/__init__.py
+-rw-r--r--   0        0        0      530 2023-06-09 10:14:33.661593 ellar-0.4.2/ellar/openapi/docs_generators/base.py
+-rw-r--r--   0        0        0      959 2023-06-09 10:14:33.661593 ellar-0.4.2/ellar/openapi/docs_generators/redocs.py
+-rw-r--r--   0        0        0     1025 2023-06-09 10:14:33.661593 ellar-0.4.2/ellar/openapi/docs_generators/swagger.py
+-rw-r--r--   0        0        0     2937 2023-06-09 10:14:33.661593 ellar-0.4.2/ellar/openapi/module.py
+-rw-r--r--   0        0        0    10611 2023-06-09 10:14:33.661593 ellar-0.4.2/ellar/openapi/openapi_v3.py
+-rw-r--r--   0        0        0    15879 2023-06-09 10:14:33.661593 ellar-0.4.2/ellar/openapi/route_doc_models.py
+-rw-r--r--   0        0        0      115 2023-06-09 10:14:33.661593 ellar-0.4.2/ellar/openapi/schemas/__init__.py
+-rw-r--r--   0        0        0      342 2023-06-09 10:14:33.661593 ellar-0.4.2/ellar/openapi/schemas/validation.py
+-rw-r--r--   0        0        0      702 2023-06-09 10:14:33.661593 ellar-0.4.2/ellar/openapi/templates/redocs.html
+-rw-r--r--   0        0        0      758 2023-06-09 10:14:33.661593 ellar-0.4.2/ellar/openapi/templates/swagger.html
+-rw-r--r--   0        0        0        0 2023-06-09 10:14:33.661593 ellar-0.4.2/ellar/py.typed
+-rw-r--r--   0        0        0      180 2023-06-09 10:14:33.661593 ellar-0.4.2/ellar/reflect/__init__.py
+-rw-r--r--   0        0        0     5356 2023-06-09 10:14:33.661593 ellar-0.4.2/ellar/reflect/_reflect.py
+-rw-r--r--   0        0        0       34 2023-06-09 10:14:33.661593 ellar-0.4.2/ellar/reflect/constants.py
+-rw-r--r--   0        0        0      238 2023-06-09 10:14:33.661593 ellar-0.4.2/ellar/reflect/contextmanager_fix.py
+-rw-r--r--   0        0        0       58 2023-06-09 10:14:33.661593 ellar-0.4.2/ellar/samples/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-09 10:14:33.661593 ellar-0.4.2/ellar/samples/controllers/__init__.py
+-rw-r--r--   0        0        0      381 2023-06-09 10:14:33.661593 ellar-0.4.2/ellar/samples/controllers/home.py
+-rw-r--r--   0        0        0      211 2023-06-09 10:14:33.661593 ellar-0.4.2/ellar/samples/modules.py
+-rw-r--r--   0        0        0   155845 2023-06-09 10:14:33.661593 ellar-0.4.2/ellar/samples/static/css/bootstrap.min.css
+-rwxr-xr-x   0        0        0    25915 2023-06-09 10:14:33.661593 ellar-0.4.2/ellar/samples/static/img/EllarLogoB.png
+-rwxr-xr-x   0        0        0    36744 2023-06-09 10:14:33.661593 ellar-0.4.2/ellar/samples/static/img/EllarLogoIconOnly.png
+-rwxr-xr-x   0        0        0     3888 2023-06-09 10:14:33.661593 ellar-0.4.2/ellar/samples/static/img/Icon.svg
+-rw-r--r--   0        0        0     1312 2023-06-09 10:14:33.661593 ellar-0.4.2/ellar/samples/templates/home/index.html
+-rw-r--r--   0        0        0      596 2023-06-09 10:14:33.661593 ellar-0.4.2/ellar/socket_io/__init__.py
+-rw-r--r--   0        0        0      423 2023-06-09 10:14:33.661593 ellar-0.4.2/ellar/socket_io/adapter.py
+-rw-r--r--   0        0        0      524 2023-06-09 10:14:33.661593 ellar-0.4.2/ellar/socket_io/constants.py
+-rw-r--r--   0        0        0     1659 2023-06-09 10:14:33.661593 ellar-0.4.2/ellar/socket_io/context.py
+-rw-r--r--   0        0        0      225 2023-06-09 10:14:33.661593 ellar-0.4.2/ellar/socket_io/decorators/__init__.py
+-rw-r--r--   0        0        0      667 2023-06-09 10:14:33.661593 ellar-0.4.2/ellar/socket_io/decorators/events.py
+-rw-r--r--   0        0        0     3846 2023-06-09 10:14:33.661593 ellar-0.4.2/ellar/socket_io/decorators/gateway.py
+-rw-r--r--   0        0        0      578 2023-06-09 10:14:33.661593 ellar-0.4.2/ellar/socket_io/decorators/subscribe_message.py
+-rw-r--r--   0        0        0     2511 2023-06-09 10:14:33.661593 ellar-0.4.2/ellar/socket_io/factory.py
+-rw-r--r--   0        0        0     9627 2023-06-09 10:14:33.661593 ellar-0.4.2/ellar/socket_io/gateway.py
+-rw-r--r--   0        0        0      144 2023-06-09 10:14:33.661593 ellar-0.4.2/ellar/socket_io/model.py
+-rw-r--r--   0        0        0      465 2023-06-09 10:14:33.661593 ellar-0.4.2/ellar/socket_io/responses.py
+-rw-r--r--   0        0        0      107 2023-06-09 10:14:33.661593 ellar-0.4.2/ellar/socket_io/testing/__init__.py
+-rw-r--r--   0        0        0     1704 2023-06-09 10:14:33.665593 ellar-0.4.2/ellar/socket_io/testing/module.py
+-rw-r--r--   0        0        0      129 2023-06-09 10:14:33.665593 ellar-0.4.2/ellar/testing/__init__.py
+-rw-r--r--   0        0        0     4074 2023-06-09 10:14:33.665593 ellar-0.4.2/ellar/testing/module.py
+-rw-r--r--   0        0        0     1215 2023-06-09 10:14:33.665593 ellar-0.4.2/ellar/testing/uvicorn_server.py
+-rw-r--r--   0        0        0      509 2023-06-09 10:14:33.665593 ellar-0.4.2/examples/01-carapp/README.md
+-rw-r--r--   0        0        0        0 2023-06-09 10:14:33.665593 ellar-0.4.2/examples/01-carapp/carapp/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-09 10:14:33.665593 ellar-0.4.2/examples/01-carapp/carapp/apps/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-09 10:14:33.665593 ellar-0.4.2/examples/01-carapp/carapp/apps/car/__init__.py
+-rw-r--r--   0        0        0     1659 2023-06-09 10:14:33.665593 ellar-0.4.2/examples/01-carapp/carapp/apps/car/controllers.py
+-rw-r--r--   0        0        0     1077 2023-06-09 10:14:33.665593 ellar-0.4.2/examples/01-carapp/carapp/apps/car/module.py
+-rw-r--r--   0        0        0     1146 2023-06-09 10:14:33.665593 ellar-0.4.2/examples/01-carapp/carapp/apps/car/routers.py
+-rw-r--r--   0        0        0      629 2023-06-09 10:14:33.665593 ellar-0.4.2/examples/01-carapp/carapp/apps/car/schemas.py
+-rw-r--r--   0        0        0      666 2023-06-09 10:14:33.665593 ellar-0.4.2/examples/01-carapp/carapp/apps/car/services.py
+-rw-r--r--   0        0        0     1708 2023-06-09 10:14:33.665593 ellar-0.4.2/examples/01-carapp/carapp/apps/car/statics/blog/blog.css
+-rw-r--r--   0        0        0     1586 2023-06-09 10:14:33.665593 ellar-0.4.2/examples/01-carapp/carapp/apps/car/statics/blog/blog.rtl.css
+-rw-r--r--   0        0        0     1008 2023-06-09 10:14:33.665593 ellar-0.4.2/examples/01-carapp/carapp/apps/car/statics/brand/bootstrap-logo-white.svg
+-rw-r--r--   0        0        0     2047 2023-06-09 10:14:33.665593 ellar-0.4.2/examples/01-carapp/carapp/apps/car/statics/brand/bootstrap-logo.svg
+-rw-r--r--   0        0        0        0 2023-06-09 10:14:33.665593 ellar-0.4.2/examples/01-carapp/carapp/apps/car/tests/__init__.py
+-rw-r--r--   0        0        0     2900 2023-06-09 10:14:33.665593 ellar-0.4.2/examples/01-carapp/carapp/apps/car/tests/test_controllers.py
+-rw-r--r--   0        0        0     1604 2023-06-09 10:14:33.665593 ellar-0.4.2/examples/01-carapp/carapp/apps/car/tests/test_routers.py
+-rw-r--r--   0        0        0        0 2023-06-09 10:14:33.665593 ellar-0.4.2/examples/01-carapp/carapp/apps/car/tests/test_services.py
+-rw-r--r--   0        0        0      202 2023-06-09 10:14:33.665593 ellar-0.4.2/examples/01-carapp/carapp/apps/car/views/car/list.html
+-rw-r--r--   0        0        0      202 2023-06-09 10:14:33.665593 ellar-0.4.2/examples/01-carapp/carapp/apps/car/views/cat/list.html
+-rw-r--r--   0        0        0    15257 2023-06-09 10:14:33.665593 ellar-0.4.2/examples/01-carapp/carapp/apps/car/views/index.html
+-rw-r--r--   0        0        0      216 2023-06-09 10:14:33.665593 ellar-0.4.2/examples/01-carapp/carapp/commands.py
+-rw-r--r--   0        0        0      187 2023-06-09 10:14:33.665593 ellar-0.4.2/examples/01-carapp/carapp/config.py
+-rw-r--r--   0        0        0      598 2023-06-09 10:14:33.665593 ellar-0.4.2/examples/01-carapp/carapp/root_module.py
+-rw-r--r--   0        0        0      954 2023-06-09 10:14:33.665593 ellar-0.4.2/examples/01-carapp/carapp/server.py
+-rw-r--r--   0        0        0      134 2023-06-09 10:14:33.665593 ellar-0.4.2/examples/01-carapp/carapp/tests/conftest.py
+-rw-r--r--   0        0        0      241 2023-06-09 10:14:33.665593 ellar-0.4.2/examples/01-carapp/pyproject.toml
+-rw-r--r--   0        0        0      264 2023-06-09 10:14:33.665593 ellar-0.4.2/examples/02-socketio-app/README.md
+-rw-r--r--   0        0        0      283 2023-06-09 10:14:33.665593 ellar-0.4.2/examples/02-socketio-app/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-09 10:14:33.665593 ellar-0.4.2/examples/02-socketio-app/socketio_app/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-09 10:14:33.665593 ellar-0.4.2/examples/02-socketio-app/socketio_app/apps/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-09 10:14:33.665593 ellar-0.4.2/examples/02-socketio-app/socketio_app/apps/events/__init__.py
+-rw-r--r--   0        0        0      455 2023-06-09 10:14:33.665593 ellar-0.4.2/examples/02-socketio-app/socketio_app/apps/events/controllers.py
+-rw-r--r--   0        0        0     2182 2023-06-09 10:14:33.665593 ellar-0.4.2/examples/02-socketio-app/socketio_app/apps/events/gateways.py
+-rw-r--r--   0        0        0     1005 2023-06-09 10:14:33.665593 ellar-0.4.2/examples/02-socketio-app/socketio_app/apps/events/module.py
+-rw-r--r--   0        0        0      295 2023-06-09 10:14:33.665593 ellar-0.4.2/examples/02-socketio-app/socketio_app/apps/events/routers.py
+-rw-r--r--   0        0        0      542 2023-06-09 10:14:33.665593 ellar-0.4.2/examples/02-socketio-app/socketio_app/apps/events/schemas.py
+-rw-r--r--   0        0        0      179 2023-06-09 10:14:33.665593 ellar-0.4.2/examples/02-socketio-app/socketio_app/apps/events/services.py
+-rw-r--r--   0        0        0     3829 2023-06-09 10:14:33.665593 ellar-0.4.2/examples/02-socketio-app/socketio_app/apps/events/templates/events/index.html
+-rw-r--r--   0        0        0        0 2023-06-09 10:14:33.665593 ellar-0.4.2/examples/02-socketio-app/socketio_app/apps/events/tests/test_controllers.py
+-rw-r--r--   0        0        0        0 2023-06-09 10:14:33.665593 ellar-0.4.2/examples/02-socketio-app/socketio_app/apps/events/tests/test_routers.py
+-rw-r--r--   0        0        0        0 2023-06-09 10:14:33.665593 ellar-0.4.2/examples/02-socketio-app/socketio_app/apps/events/tests/test_services.py
+-rw-r--r--   0        0        0     2602 2023-06-09 10:14:33.665593 ellar-0.4.2/examples/02-socketio-app/socketio_app/config.py
+-rw-r--r--   0        0        0        0 2023-06-09 10:14:33.665593 ellar-0.4.2/examples/02-socketio-app/socketio_app/core/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-09 10:14:33.665593 ellar-0.4.2/examples/02-socketio-app/socketio_app/domain/__init__.py
+-rw-r--r--   0        0        0      480 2023-06-09 10:14:33.665593 ellar-0.4.2/examples/02-socketio-app/socketio_app/root_module.py
+-rw-r--r--   0        0        0     1045 2023-06-09 10:14:33.665593 ellar-0.4.2/examples/02-socketio-app/socketio_app/server.py
+-rw-r--r--   0        0        0       43 2023-06-09 10:14:33.665593 ellar-0.4.2/examples/02-socketio-app/tests/conftest.py
+-rw-r--r--   0        0        0     4506 2023-06-09 10:14:33.665593 ellar-0.4.2/mkdocs.yml
+-rw-r--r--   0        0        0      597 2023-06-09 10:14:33.665593 ellar-0.4.2/mypy.ini
+-rw-r--r--   0        0        0     3038 2023-06-09 10:14:33.665593 ellar-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0      207 2023-06-09 10:14:33.665593 ellar-0.4.2/pytest.ini
+-rw-r--r--   0        0        0        0 2023-06-09 10:14:33.665593 ellar-0.4.2/tests/__init__.py
+-rw-r--r--   0        0        0     1022 2023-06-09 10:14:33.665593 ellar-0.4.2/tests/conftest.py
+-rw-r--r--   0        0        0      616 2023-06-09 10:14:33.665593 ellar-0.4.2/tests/injector_module.py
+-rw-r--r--   0        0        0     5249 2023-06-09 10:14:33.665593 ellar-0.4.2/tests/main.py
+-rw-r--r--   0        0        0       23 2023-06-09 10:14:33.665593 ellar-0.4.2/tests/private/test.css
+-rw-r--r--   0        0        0      748 2023-06-09 10:14:33.665593 ellar-0.4.2/tests/schema.py
+-rw-r--r--   0        0        0        4 2023-06-09 10:14:33.665593 ellar-0.4.2/tests/statics/example.txt
+-rw-r--r--   0        0        0      160 2023-06-09 10:14:33.665593 ellar-0.4.2/tests/templates/ellar/index.html
+-rw-r--r--   0        0        0      102 2023-06-09 10:14:33.665593 ellar-0.4.2/tests/templates/ellar/list.html
+-rw-r--r--   0        0        0      129 2023-06-09 10:14:33.665593 ellar-0.4.2/tests/templates/index.html
+-rw-r--r--   0        0        0      128 2023-06-09 10:14:33.665593 ellar-0.4.2/tests/templates/list.html
+-rw-r--r--   0        0        0       65 2023-06-09 10:14:33.665593 ellar-0.4.2/tests/templates/render_string.html
+-rw-r--r--   0        0        0        0 2023-06-09 10:14:33.665593 ellar-0.4.2/tests/test_application/__init__.py
+-rw-r--r--   0        0        0       84 2023-06-09 10:14:33.665593 ellar-0.4.2/tests/test_application/config.py
+-rw-r--r--   0        0        0     2854 2023-06-09 10:14:33.665593 ellar-0.4.2/tests/test_application/sample.py
+-rw-r--r--   0        0        0     3548 2023-06-09 10:14:33.665593 ellar-0.4.2/tests/test_application/test_application_factory.py
+-rw-r--r--   0        0        0    15855 2023-06-09 10:14:33.665593 ellar-0.4.2/tests/test_application/test_application_functions.py
+-rw-r--r--   0        0        0    18052 2023-06-09 10:14:33.665593 ellar-0.4.2/tests/test_application/test_cors.py
+-rw-r--r--   0        0        0     4352 2023-06-09 10:14:33.665593 ellar-0.4.2/tests/test_application/test_replacing_app_services.py
+-rw-r--r--   0        0        0     2329 2023-06-09 10:14:33.665593 ellar-0.4.2/tests/test_application/test_trusted_host.py
+-rw-r--r--   0        0        0      862 2023-06-09 10:14:33.665593 ellar-0.4.2/tests/test_attribute_dict.py
+-rw-r--r--   0        0        0        0 2023-06-09 10:14:33.665593 ellar-0.4.2/tests/test_cache/__init__.py
+-rw-r--r--   0        0        0     3625 2023-06-09 10:14:33.665593 ellar-0.4.2/tests/test_cache/_test_aio_memcache.py.ellar
+-rw-r--r--   0        0        0     1893 2023-06-09 10:14:33.665593 ellar-0.4.2/tests/test_cache/pylib_mock.py
+-rw-r--r--   0        0        0     2592 2023-06-09 10:14:33.665593 ellar-0.4.2/tests/test_cache/redis_mock.py
+-rw-r--r--   0        0        0     2764 2023-06-09 10:14:33.665593 ellar-0.4.2/tests/test_cache/test_cache_decorator.py
+-rw-r--r--   0        0        0     1744 2023-06-09 10:14:33.665593 ellar-0.4.2/tests/test_cache/test_cache_many_config.py
+-rw-r--r--   0        0        0     4772 2023-06-09 10:14:33.665593 ellar-0.4.2/tests/test_cache/test_cache_service.py
+-rw-r--r--   0        0        0     4995 2023-06-09 10:14:33.665593 ellar-0.4.2/tests/test_cache/test_local_cache.py
+-rw-r--r--   0        0        0      596 2023-06-09 10:14:33.665593 ellar-0.4.2/tests/test_cache/test_module_setup.py
+-rw-r--r--   0        0        0     9973 2023-06-09 10:14:33.665593 ellar-0.4.2/tests/test_cache/test_pylibmc_cache.py
+-rw-r--r--   0        0        0     6093 2023-06-09 10:14:33.665593 ellar-0.4.2/tests/test_cache/test_redis_cache.py
+-rw-r--r--   0        0        0      577 2023-06-09 10:14:33.665593 ellar-0.4.2/tests/test_cache/test_schema.py
+-rw-r--r--   0        0        0        0 2023-06-09 10:14:33.665593 ellar-0.4.2/tests/test_conf/__init__.py
+-rw-r--r--   0        0        0      900 2023-06-09 10:14:33.665593 ellar-0.4.2/tests/test_conf/test_config_prefix.py
+-rw-r--r--   0        0        0     5223 2023-06-09 10:14:33.665593 ellar-0.4.2/tests/test_conf/test_default_conf.py
+-rw-r--r--   0        0        0     1151 2023-06-09 10:14:33.665593 ellar-0.4.2/tests/test_conf/test_mixins.py
+-rw-r--r--   0        0        0        0 2023-06-09 10:14:33.665593 ellar-0.4.2/tests/test_controller/__init__.py
+-rw-r--r--   0        0        0      387 2023-06-09 10:14:33.665593 ellar-0.4.2/tests/test_controller/sample.py
+-rw-r--r--   0        0        0        0 2023-06-09 10:14:33.665593 ellar-0.4.2/tests/test_controller/test_application_router.py
+-rw-r--r--   0        0        0     4448 2023-06-09 10:14:33.665593 ellar-0.4.2/tests/test_controller/test_controller_decorator.py
+-rw-r--r--   0        0        0     2872 2023-06-09 10:14:33.665593 ellar-0.4.2/tests/test_controller/test_controller_inheritance.py
+-rw-r--r--   0        0        0     2722 2023-06-09 10:14:33.665593 ellar-0.4.2/tests/test_controller/test_module_router.py
+-rw-r--r--   0        0        0     7186 2023-06-09 10:14:33.665593 ellar-0.4.2/tests/test_controller/test_route_collection.py
+-rw-r--r--   0        0        0        0 2023-06-09 10:14:33.665593 ellar-0.4.2/tests/test_decorators/__init__.py
+-rw-r--r--   0        0        0     3366 2023-06-09 10:14:33.665593 ellar-0.4.2/tests/test_decorators/test_controller.py
+-rw-r--r--   0        0        0      789 2023-06-09 10:14:33.665593 ellar-0.4.2/tests/test_decorators/test_exception.py
+-rw-r--r--   0        0        0     3508 2023-06-09 10:14:33.665593 ellar-0.4.2/tests/test_decorators/test_file.py
+-rw-r--r--   0        0        0     1059 2023-06-09 10:14:33.665593 ellar-0.4.2/tests/test_decorators/test_guards.py
+-rw-r--r--   0        0        0     4082 2023-06-09 10:14:33.665593 ellar-0.4.2/tests/test_decorators/test_html.py
+-rw-r--r--   0        0        0      554 2023-06-09 10:14:33.665593 ellar-0.4.2/tests/test_decorators/test_middleware.py
+-rw-r--r--   0        0        0     2061 2023-06-09 10:14:33.665593 ellar-0.4.2/tests/test_decorators/test_modules.py
+-rw-r--r--   0        0        0      915 2023-06-09 10:14:33.665593 ellar-0.4.2/tests/test_decorators/test_openapi.py
+-rw-r--r--   0        0        0     1311 2023-06-09 10:14:33.665593 ellar-0.4.2/tests/test_decorators/test_serializer.py
+-rw-r--r--   0        0        0      475 2023-06-09 10:14:33.665593 ellar-0.4.2/tests/test_decorators/test_versioning.py
+-rw-r--r--   0        0        0        0 2023-06-09 10:14:33.665593 ellar-0.4.2/tests/test_di/__init__.py
+-rw-r--r--   0        0        0     1332 2023-06-09 10:14:33.665593 ellar-0.4.2/tests/test_di/examples.py
+-rw-r--r--   0        0        0     2078 2023-06-09 10:14:33.665593 ellar-0.4.2/tests/test_di/test_injectable_resolving.py
+-rw-r--r--   0        0        0     6600 2023-06-09 10:14:33.665593 ellar-0.4.2/tests/test_di/test_injector.py
+-rw-r--r--   0        0        0     3508 2023-06-09 10:14:33.665593 ellar-0.4.2/tests/test_di/test_provider_scopes.py
+-rw-r--r--   0        0        0     3993 2023-06-09 10:14:33.665593 ellar-0.4.2/tests/test_di/test_providers.py
+-rw-r--r--   0        0        0     2094 2023-06-09 10:14:33.669593 ellar-0.4.2/tests/test_events.py
+-rw-r--r--   0        0        0        0 2023-06-09 10:14:33.669593 ellar-0.4.2/tests/test_exceptions/__init__.py
+-rw-r--r--   0        0        0      206 2023-06-09 10:14:33.669593 ellar-0.4.2/tests/test_exceptions/exception_runner.py
+-rw-r--r--   0        0        0     2562 2023-06-09 10:14:33.669593 ellar-0.4.2/tests/test_exceptions/test_api_exception.py
+-rw-r--r--   0        0        0     8609 2023-06-09 10:14:33.669593 ellar-0.4.2/tests/test_exceptions/test_custom_exceptions.py
+-rw-r--r--   0        0        0     1195 2023-06-09 10:14:33.669593 ellar-0.4.2/tests/test_exceptions/test_error_details.py
+-rw-r--r--   0        0        0     3722 2023-06-09 10:14:33.669593 ellar-0.4.2/tests/test_exceptions/test_validation_exception.py
+-rw-r--r--   0        0        0     7585 2023-06-09 10:14:33.669593 ellar-0.4.2/tests/test_guard.py
+-rw-r--r--   0        0        0        0 2023-06-09 10:14:33.669593 ellar-0.4.2/tests/test_helper/__init__.py
+-rw-r--r--   0        0        0      571 2023-06-09 10:14:33.669593 ellar-0.4.2/tests/test_helper/test_enum.py
+-rw-r--r--   0        0        0        0 2023-06-09 10:14:33.669593 ellar-0.4.2/tests/test_helper/test_importer.py
+-rw-r--r--   0        0        0      795 2023-06-09 10:14:33.669593 ellar-0.4.2/tests/test_helper/test_model_field.py
+-rw-r--r--   0        0        0      298 2023-06-09 10:14:33.669593 ellar-0.4.2/tests/test_helper/test_module_loading.py
+-rw-r--r--   0        0        0        0 2023-06-09 10:14:33.669593 ellar-0.4.2/tests/test_interceptors/__init__.py
+-rw-r--r--   0        0        0     2945 2023-06-09 10:14:33.669593 ellar-0.4.2/tests/test_interceptors/test_interceptor.py
+-rw-r--r--   0        0        0        0 2023-06-09 10:14:33.669593 ellar-0.4.2/tests/test_middleware/__init__.py
+-rw-r--r--   0        0        0     3100 2023-06-09 10:14:33.669593 ellar-0.4.2/tests/test_middleware/test_functional_middleware.py
+-rw-r--r--   0        0        0     4243 2023-06-09 10:14:33.669593 ellar-0.4.2/tests/test_middleware/test_service_provider_middleware.py
+-rw-r--r--   0        0        0     2168 2023-06-09 10:14:33.669593 ellar-0.4.2/tests/test_middleware/test_versioning_middleware.py
+-rw-r--r--   0        0        0        0 2023-06-09 10:14:33.669593 ellar-0.4.2/tests/test_modules/__init__.py
+-rw-r--r--   0        0        0     1847 2023-06-09 10:14:33.669593 ellar-0.4.2/tests/test_modules/sample.py
+-rw-r--r--   0        0        0     6760 2023-06-09 10:14:33.669593 ellar-0.4.2/tests/test_modules/test_module_config.py
+-rw-r--r--   0        0        0    10234 2023-06-09 10:14:33.669593 ellar-0.4.2/tests/test_modules/test_module_ref.py
+-rw-r--r--   0        0        0     1497 2023-06-09 10:14:33.669593 ellar-0.4.2/tests/test_modules/test_module_startup_shutdown.py
+-rw-r--r--   0        0        0        0 2023-06-09 10:14:33.669593 ellar-0.4.2/tests/test_openapi/__init__.py
+-rw-r--r--   0        0        0     8341 2023-06-09 10:14:33.669593 ellar-0.4.2/tests/test_openapi/test_builder.py
+-rw-r--r--   0        0        0     6680 2023-06-09 10:14:33.669593 ellar-0.4.2/tests/test_openapi/test_module.py
+-rw-r--r--   0        0        0    16536 2023-06-09 10:14:33.669593 ellar-0.4.2/tests/test_openapi/test_open_api_route_documentation.py
+-rw-r--r--   0        0        0     5571 2023-06-09 10:14:33.669593 ellar-0.4.2/tests/test_reflect.py
+-rw-r--r--   0        0        0     2287 2023-06-09 10:14:33.669593 ellar-0.4.2/tests/test_reflector.py
+-rw-r--r--   0        0        0        0 2023-06-09 10:14:33.669593 ellar-0.4.2/tests/test_response/__init__.py
+-rw-r--r--   0        0        0     2486 2023-06-09 10:14:33.669593 ellar-0.4.2/tests/test_response/test_defined_response_model.py
+-rw-r--r--   0        0        0     4562 2023-06-09 10:14:33.669593 ellar-0.4.2/tests/test_response/test_pydantic_response_model.py
+-rw-r--r--   0        0        0     3393 2023-06-09 10:14:33.669593 ellar-0.4.2/tests/test_response/test_response_file.py
+-rw-r--r--   0        0        0     5063 2023-06-09 10:14:33.669593 ellar-0.4.2/tests/test_response/test_response_html.py
+-rw-r--r--   0        0        0     3228 2023-06-09 10:14:33.669593 ellar-0.4.2/tests/test_response/test_response_streaming.py
+-rw-r--r--   0        0        0     3902 2023-06-09 10:14:33.669593 ellar-0.4.2/tests/test_response/test_response_type_definition_converter.py
+-rw-r--r--   0        0        0     3524 2023-06-09 10:14:33.669593 ellar-0.4.2/tests/test_response/test_route_response_model.py
+-rw-r--r--   0        0        0        0 2023-06-09 10:14:33.669593 ellar-0.4.2/tests/test_routing/__init__.py
+-rw-r--r--   0        0        0     1126 2023-06-09 10:14:33.669593 ellar-0.4.2/tests/test_routing/sample.py
+-rw-r--r--   0        0        0     2757 2023-06-09 10:14:33.669593 ellar-0.4.2/tests/test_routing/test_background_tasks.py
+-rw-r--r--   0        0        0     3605 2023-06-09 10:14:33.669593 ellar-0.4.2/tests/test_routing/test_body_schema.py
+-rw-r--r--   0        0        0     3666 2023-06-09 10:14:33.669593 ellar-0.4.2/tests/test_routing/test_body_schema_extra_properties.py
+-rw-r--r--   0        0        0     4142 2023-06-09 10:14:33.669593 ellar-0.4.2/tests/test_routing/test_body_union_schema.py
+-rw-r--r--   0        0        0     4066 2023-06-09 10:14:33.669593 ellar-0.4.2/tests/test_routing/test_cookie_schema.py
+-rw-r--r--   0        0        0     6854 2023-06-09 10:14:33.669593 ellar-0.4.2/tests/test_routing/test_extra_args.py
+-rw-r--r--   0        0        0     2457 2023-06-09 10:14:33.669593 ellar-0.4.2/tests/test_routing/test_form_schema.py
+-rw-r--r--   0        0        0    10018 2023-06-09 10:14:33.669593 ellar-0.4.2/tests/test_routing/test_formparsers.py
+-rw-r--r--   0        0        0     1282 2023-06-09 10:14:33.669593 ellar-0.4.2/tests/test_routing/test_forms.py
+-rw-r--r--   0        0        0     1296 2023-06-09 10:14:33.669593 ellar-0.4.2/tests/test_routing/test_forms_from_non_typing_sequences.py
+-rw-r--r--   0        0        0     3633 2023-06-09 10:14:33.669593 ellar-0.4.2/tests/test_routing/test_header_schema.py
+-rw-r--r--   0        0        0     1887 2023-06-09 10:14:33.669593 ellar-0.4.2/tests/test_routing/test_invalid_path_param.py
+-rw-r--r--   0        0        0     2006 2023-06-09 10:14:33.669593 ellar-0.4.2/tests/test_routing/test_invalid_sequence_param.py
+-rw-r--r--   0        0        0     5205 2023-06-09 10:14:33.669593 ellar-0.4.2/tests/test_routing/test_multi_body_errors.py
+-rw-r--r--   0        0        0     3783 2023-06-09 10:14:33.669593 ellar-0.4.2/tests/test_routing/test_multi_query_errors.py
+-rw-r--r--   0        0        0     9423 2023-06-09 10:14:33.669593 ellar-0.4.2/tests/test_routing/test_path.py
+-rw-r--r--   0        0        0     2933 2023-06-09 10:14:33.669593 ellar-0.4.2/tests/test_routing/test_path_with_schema.py
+-rw-r--r--   0        0        0     3333 2023-06-09 10:14:33.669593 ellar-0.4.2/tests/test_routing/test_put_with_no_body_schema.py
+-rw-r--r--   0        0        0     2242 2023-06-09 10:14:33.669593 ellar-0.4.2/tests/test_routing/test_query.py
+-rw-r--r--   0        0        0     3699 2023-06-09 10:14:33.669593 ellar-0.4.2/tests/test_routing/test_query_schema.py
+-rw-r--r--   0        0        0     1987 2023-06-09 10:14:33.669593 ellar-0.4.2/tests/test_routing/test_request.py
+-rw-r--r--   0        0        0     3415 2023-06-09 10:14:33.669593 ellar-0.4.2/tests/test_routing/test_route_endpoint_params.py
+-rw-r--r--   0        0        0      451 2023-06-09 10:14:33.669593 ellar-0.4.2/tests/test_sample_project.py
+-rw-r--r--   0        0        0     2712 2023-06-09 10:14:33.669593 ellar-0.4.2/tests/test_schema.py
+-rw-r--r--   0        0        0     6379 2023-06-09 10:14:33.669593 ellar-0.4.2/tests/test_serializer.py
+-rw-r--r--   0        0        0      775 2023-06-09 10:14:33.669593 ellar-0.4.2/tests/test_shortcuts.py
+-rw-r--r--   0        0        0        0 2023-06-09 10:14:33.669593 ellar-0.4.2/tests/test_socket_io/__init__.py
+-rw-r--r--   0        0        0     4116 2023-06-09 10:14:33.669593 ellar-0.4.2/tests/test_socket_io/sample.py
+-rw-r--r--   0        0        0      718 2023-06-09 10:14:33.669593 ellar-0.4.2/tests/test_socket_io/test_decorators/test_events.py
+-rw-r--r--   0        0        0     3598 2023-06-09 10:14:33.669593 ellar-0.4.2/tests/test_socket_io/test_decorators/test_gateway.py
+-rw-r--r--   0        0        0      719 2023-06-09 10:14:33.669593 ellar-0.4.2/tests/test_socket_io/test_decorators/test_subcribe_message.py
+-rw-r--r--   0        0        0      859 2023-06-09 10:14:33.669593 ellar-0.4.2/tests/test_socket_io/test_gateway.py
+-rw-r--r--   0        0        0     8889 2023-06-09 10:14:33.669593 ellar-0.4.2/tests/test_socket_io/test_operation.py
+-rw-r--r--   0        0        0    14104 2023-06-09 10:14:33.669593 ellar-0.4.2/tests/test_staticfiles.py
+-rw-r--r--   0        0        0        0 2023-06-09 10:14:33.669593 ellar-0.4.2/tests/test_templating/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-09 10:14:33.669593 ellar-0.4.2/tests/test_templating/module_statics/watever.txt
+-rw-r--r--   0        0        0        0 2023-06-09 10:14:33.669593 ellar-0.4.2/tests/test_templating/static/watever.txt
+-rw-r--r--   0        0        0      167 2023-06-09 10:14:33.669593 ellar-0.4.2/tests/test_templating/templates/watever.html
+-rw-r--r--   0        0        0     2904 2023-06-09 10:14:33.669593 ellar-0.4.2/tests/test_templating/test_module_templating.py
+-rw-r--r--   0        0        0     2718 2023-06-09 10:14:33.669593 ellar-0.4.2/tests/test_templating/test_renderer.py
+-rw-r--r--   0        0        0        0 2023-06-09 10:14:33.669593 ellar-0.4.2/tests/test_templating/views/watever.html
+-rw-r--r--   0        0        0     2425 2023-06-09 10:14:33.669593 ellar-0.4.2/tests/test_testing.py
+-rw-r--r--   0        0        0        0 2023-06-09 10:14:33.669593 ellar-0.4.2/tests/test_versioning/__init__.py
+-rw-r--r--   0        0        0     1968 2023-06-09 10:14:33.669593 ellar-0.4.2/tests/test_versioning/operations.py
+-rw-r--r--   0        0        0     2138 2023-06-09 10:14:33.669593 ellar-0.4.2/tests/test_versioning/test_default_versioning.py
+-rw-r--r--   0        0        0     4449 2023-06-09 10:14:33.669593 ellar-0.4.2/tests/test_versioning/test_default_versioning_for_controllers.py
+-rw-r--r--   0        0        0     4475 2023-06-09 10:14:33.669593 ellar-0.4.2/tests/test_versioning/test_header_versioning.py
+-rw-r--r--   0        0        0     7820 2023-06-09 10:14:33.669593 ellar-0.4.2/tests/test_versioning/test_header_versioning_controller.py
+-rw-r--r--   0        0        0     3823 2023-06-09 10:14:33.669593 ellar-0.4.2/tests/test_versioning/test_host_versioning.py
+-rw-r--r--   0        0        0     3227 2023-06-09 10:14:33.669593 ellar-0.4.2/tests/test_versioning/test_query_versioning.py
+-rw-r--r--   0        0        0     2865 2023-06-09 10:14:33.669593 ellar-0.4.2/tests/test_versioning/test_url_versioning.py
+-rw-r--r--   0        0        0    17496 2023-06-09 10:14:33.669593 ellar-0.4.2/tests/test_websocket.py
+-rw-r--r--   0        0        0    11181 2023-06-09 10:14:33.669593 ellar-0.4.2/tests/test_websocket_handler.py
+-rw-r--r--   0        0        0    14699 1970-01-01 00:00:00.000000 ellar-0.4.2/PKG-INFO
```

### Comparing `ellar-0.4.0/.github/workflows/publish.yml` & `ellar-0.4.2/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/.github/workflows/test.yml` & `ellar-0.4.2/.github/workflows/test.yml`

 * *Files 0% similar despite different names*

```diff
@@ -18,8 +18,8 @@
       - name: Install Flit
         run: pip install flit
       - name: Install Dependencies
         run: flit install --symlink
       - name: Test
         run: make test-cov
       - name: Coverage
-        uses: codecov/codecov-action@v3.1.3
+        uses: codecov/codecov-action@v3.1.4
```

### Comparing `ellar-0.4.0/.github/workflows/test_full.yml` & `ellar-0.4.2/.github/workflows/test_full.yml`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/.gitignore` & `ellar-0.4.2/.gitignore`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/.pre-commit-config.yaml` & `ellar-0.4.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/LICENSE` & `ellar-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/Makefile` & `ellar-0.4.2/Makefile`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/README.md` & `ellar-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/docs/background-task.md` & `ellar-0.4.2/docs/techniques/background-task.md`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 ## **Using BackgroundTasks**
 `BackgroundTasks` is another class from Starlette useful for adding multiple background tasks to a response. 
 Unlike the previous construct, `BackgroundTasks` can be injected into your route function by type annotation.
 
 For example:
 ```python
 from starlette.background import BackgroundTasks
-from ellar.common import ModuleRouter, get, Res
+from ellar.common import ModuleRouter
 
 router = ModuleRouter('/background-test')
 
 def another_background_task(parameter):
     print(f'Another Background task called with "{parameter}"')
     
 async def send_welcome_email(email):
```

### Comparing `ellar-0.4.0/docs/basics/execution-context.md` & `ellar-0.4.2/docs/basics/execution-context.md`

 * *Files 0% similar despite different names*

```diff
@@ -159,15 +159,15 @@
     def get_handler(self) -> typing.Callable:
         pass
 
 ```
 
 These extra information are necessary for reading `metadata` properties set on controllers or the route handler function.
 
-### How to access the current execution context
+### **How to access the current execution context**
 You can access the current execution context using the `Context()` function. 
 This decorator can be applied to a parameter of a controller or service method, 
 and it will inject the current `ExecutionContext` object into the method.
 
 For example, consider the following controller method:
 ```python
 from ellar.common import Context, get, Controller
```

### Comparing `ellar-0.4.0/docs/basics/testing.md` & `ellar-0.4.2/docs/basics/testing.md`

 * *Files 0% similar despite different names*

```diff
@@ -286,15 +286,15 @@
 which is where automated e2e testing becomes essential in validating that the system's overall behavior is correct and 
 aligned with project requirements. 
 
 To execute e2e tests, we adopt a similar configuration to that of unit testing, 
 and Ellar's use of **TestClient**, a tool provided by Starlette, to facilitates the simulation of HTTP requests
 
 ### **TestClient**
-Starlette provides a [TestClient](https://www.starlette.io/testclient/) for making requests ASGI Applications, and it's based on [httpx](https://www.python-httpx.org/) library similar to requests.
+Starlette provides a [TestClient](https://www.starlette.io/testclient/){target="_blank"} for making requests ASGI Applications, and it's based on [httpx](https://www.python-httpx.org/) library similar to requests.
 ```python
 from starlette.responses import HTMLResponse
 from starlette.testclient import TestClient
 
 
 async def app(scope, receive, send):
     assert scope['type'] == 'http'
```

### Comparing `ellar-0.4.0/docs/basics/versioning.md` & `ellar-0.4.2/docs/techniques/versioning.md`

 * *Files 0% similar despite different names*

```diff
@@ -166,15 +166,15 @@
 ```regexp
 ^([a-zA-Z0-9]+)\.[a-zA-Z0-9]+\.[a-zA-Z0-9]+$
 ```
 
 Note that the first group is enclosed in brackets, indicating that this is the matched portion of the hostname.
 
 The `HostNameVersioning` scheme can be awkward to use in debug mode as you will typically be accessing a raw IP address such as 127.0.0.1. 
-There are various online tutorials on how to [access localhost with a custom subdomain](https://reinteractive.net/posts/199-developing-and-testing-rails-applications-with-subdomains) which you may find helpful in this case.
+There are various online tutorials on how to [access localhost with a custom subdomain](https://reinteractive.net/posts/199-developing-and-testing-rails-applications-with-subdomains){target="_blank"} which you may find helpful in this case.
 
 Hostname based versioning can be particularly useful if you have requirements to route incoming requests to different servers based on the version, as you can configure different DNS records for different API versions.
 
 ## **Controller Versions**
 A version can be applied to a controller by using `Version` decorator from `ellar.common` package.
 
 To add a version to a controller do the following:
```

### Comparing `ellar-0.4.0/docs/caching.md` & `ellar-0.4.2/docs/techniques/caching.md`

 * *Files 2% similar despite different names*

```diff
@@ -64,22 +64,22 @@
     class ApplicationModule:
         pass
     ```
     In CacheModule.`setup`, the `default` parameter must be provided and other cache 
     backends will be defined as keyword-arguments just like `local` and `others` incase you want to set up more than one cache backend.
 
 ### **Memcached**
-[Memcached](https://memcached.org/) is an entirely memory-based cache server, originally developed to handle high loads at LiveJournal.com and subsequently open-sourced by Danga Interactive.
+[Memcached](https://memcached.org/){target="_blank"} is an entirely memory-based cache server, originally developed to handle high loads at LiveJournal.com and subsequently open-sourced by Danga Interactive.
 
 Memcached runs as a daemon and is allotted a specified amount of RAM. All it does is provide a fast interface for adding, retrieving and deleting data in the cache. All data is stored directly in memory.
 
 After installing Memcached itself, you’ll need to install a Memcached binding. 
 There are several Python Memcached bindings available; 
 
-Ellar supports are [pylibmc](https://pypi.org/project/pylibmc/) and [pymemcache](https://pypi.org/project/pymemcache/)
+Ellar supports are [pylibmc](https://pypi.org/project/pylibmc/){target="_blank"} and [pymemcache](https://pypi.org/project/pymemcache/){target="_blank"}
 
 For an example, lets assume you have a Memcached is running on localhost (127.0.0.1) port 11211, using the `pymemcache` or `pylibmc` binding:
 
 === "pymemcache"
     ```python
     # project_name/config.py
     
@@ -192,19 +192,19 @@
             '172.19.26.242:11212',
             '172.19.26.244:11213',
         ], options={'default_noreply': True})
     }
 ```
 
 ### **Redis**
-[Redis](https://redis.io/) is a high-performance, in-memory database that is commonly used for caching data. 
+[Redis](https://redis.io/){target="_blank"} is a high-performance, in-memory database that is commonly used for caching data. 
 To get started with Redis, you will need to have a Redis server running on either your local machine or a remote server.
 
 Once you have set up the Redis server, 
-you will need to install the [Redis](https://pypi.org/project/redis/) Python client library to be able 
+you will need to install the [Redis](https://pypi.org/project/redis/){target="_blank"} Python client library to be able 
 to communicate with Redis from your Python code. 
 
 To use redis in Ellar, you need to import RedisCacheBackend from `ellar.cache.backend.redis`.
 
 Let's assume after setting up your redis server and it's running on localhost (127.0.0.1) port 6379:
 
 === "Redis"
```

### Comparing `ellar-0.4.0/docs/commands/command-grouping.md` & `ellar-0.4.2/docs/cli/command-grouping.md`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/docs/commands/create-module-command.md` & `ellar-0.4.2/docs/cli/create-module-command.md`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/docs/commands/custom-commands.md` & `ellar-0.4.2/docs/cli/custom-commands.md`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/docs/commands/index.md` & `ellar-0.4.2/docs/cli/index.md`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/docs/commands/new-command.md` & `ellar-0.4.2/docs/cli/new-command.md`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/docs/commands/runserver-command.md` & `ellar-0.4.2/docs/cli/runserver-command.md`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/docs/configurations.md` & `ellar-0.4.2/docs/techniques/configurations.md`

 * *Files 9% similar despite different names*

```diff
@@ -35,16 +35,16 @@
 ### **DEFAULT_JSON_CLASS**
 Default: `JSONResponse` - (`starlette.common.JSONResponse`)
 
 **DEFAULT_JSON_CLASS** is used when sending JSON response to the client.
 
 There are other options for JSON available in Ellar:
 
-- **UJSONResponse**(`ellar.common.UJSONResponse`):  renders JSON response using [ujson](https://pypi.python.org/pypi/ujson). 
-- **ORJSONResponse**(`ellar.common.ORJSONResponse`):  renders JSON response using [orjson](https://pypi.org/project/orjson/). 
+- **UJSONResponse**(`ellar.common.UJSONResponse`):  renders JSON response using [ujson](https://pypi.python.org/pypi/ujson){target="_blank"}. 
+- **ORJSONResponse**(`ellar.common.ORJSONResponse`):  renders JSON response using [orjson](https://pypi.org/project/orjson/){target="_blank"}. 
 
 ### **JINJA_TEMPLATES_OPTIONS**
 Default: `{}`
 
 Default is an empty dictionary object. It defines options used when creating `Jinja2` Environment for templating.
 
 Different keys available:
@@ -69,15 +69,15 @@
 - `loader` (Optional[BaseLoader]) –
 - `cache_size` (int) –
 - `auto_reload` (bool) –
 - `bytecode_cache` (Optional[BytecodeCache]) –
 - `enable_async` (bool)
 
 !!! info
-    Check Jinja2 [environment option](https://jinja.palletsprojects.com/en/3.0.x/api/#high-level-api) for more information.
+    Check Jinja2 [environment option](https://jinja.palletsprojects.com/en/3.0.x/api/#high-level-api){target="_blank"} for more information.
 
 ### **VERSIONING_SCHEME**
 Default: `DefaultAPIVersioning()`
 
 **VERSIONING_SCHEME** defined the versioning scheme for the application.  
 The **DefaultAPIVersioning** is placeHolder object for versioning scheme.
 
@@ -247,7 +247,52 @@
 
 To allow any hostname either use `allowed_hosts=["*"]` or omit the middleware.
 
 ### **REDIRECT_HOST**
 Default: `True`
 
 Indicates whether to append `www.` when redirecting host in `TrustedHostMiddleware`
+
+
+## **Configuration with prefix**
+Ellar configuration module also support loading of its configurations with appended prefix. for instance,
+we can have a file `my_settings.py` with some ellar's configurations set to it with some prefix `API_` as shown below.
+
+```python
+# my_settings.py
+API_DEBUG = True
+API_SECRET_KEY = "your-secret-key-changed"
+API_INJECTOR_AUTO_BIND = True
+API_JINJA_TEMPLATES_OPTIONS = {"auto_reload": True}
+
+OTHER_XYZ_CONFIGS_1 ='whatever'
+OTHER_XYZ_CONFIGS_2 ='whatever2'
+```
+To apply these configurations without having to load everything, you have to provide the prefix to be used to load configurations that
+belongs to ellar. For example,
+
+```python
+from ellar.core.factory import AppFactory
+from .root_module import ApplicationModule
+
+application = AppFactory.create_from_app_module(ApplicationModule, config_module=dict(
+    config_module='project_name:my_settings',
+    config_prefix='api_',
+))
+```
+In the above construct, we used a dict object to define the configuration module(`'project_name:my_settings'`) and prefix `api_`. 
+This will be applied to the configuration instance when the application is ready.
+
+## **Defining Configurations directly**
+During application bootstrapping with `AppFactory`, you can define app configurations directly under `config_module` as a dict object as some below.
+
+```python
+from ellar.core.factory import AppFactory
+from .root_module import ApplicationModule
+
+application = AppFactory.create_from_app_module(ApplicationModule, config_module=dict(
+    SECRET_KEY = "your-secret-key-changed",
+    INJECTOR_AUTO_BIND = True,
+    MIDDLEWARE=[],
+    EXCEPTION_HANDLERS=[]
+))
+```
```

### Comparing `ellar-0.4.0/docs/custom-setup.md` & `ellar-0.4.2/docs/custom-setup.md`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/docs/handling-response/response-model.md` & `ellar-0.4.2/docs/techniques/response-model.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Response Model
+# **Response Models**
 
 Each route handler has key-value pair of status codes and a response model. 
 This response model holds information on the type of response to be returned.
 
 ```python
 # project_name/apps/items/controllers.py
 
@@ -58,15 +58,15 @@
 
 ![response description](../img/response_description.png)
 
 !!! info
     Each route handler has its own `ResponseModel` computation and validation. If there is no response definition, Ellar default the route handler model to `EmptyAPIResponseModel`.
 
 
-## Override Response Type
+## **Override Response Type**
 
 When you use a `Response` class as response, a `ResponseModel` is used and the `response_type` is replaced with applied response class.
 
 For example:
 
 ```python
 # project_name/apps/items/controllers.py
@@ -92,15 +92,15 @@
 ```python
 from ellar.common.responses.models import ResponseModel, JSONResponseModel
 from ellar.common import PlainTextResponse
 
 response = {200: ResponseModel(response_type=PlainTextResponse), 201: JSONResponseModel(model_field_or_schema=UserSchema)}
 ```
 
-## Response Model Properties
+## **Response Model Properties**
 
 All response model follows `IResponseModel` contract.
 
 ```python
 import typing as t
 
 from pydantic.fields import ModelField
@@ -125,15 +125,15 @@
 
 They include:
 
 - `response_type`: Response classes eg. JSONResponse, PlainResponse, HTMLResponse. etc. Default: `Response`. **Required**
 - `model_field_or_schema`: `Optional` property. For return data validation. Default: `None` **Optional**
 
 
-## Different Response Models 
+## **Different Response Models**
 Let's see different `ResponseModel` available in Ellar and how you can create one too.
 
 ### **ResponseModel** 
 Response model that manages rendering of other response types.
 
 - Location: `ellar.common.responses.models.ResponseModel`
 - response_type: `Response`
@@ -179,15 +179,15 @@
 Default `ResponseModel` applied when no response is defined.
 
 - Location: `ellar.common.responses.models.json.EmptyAPIResponseModel`
 - response_type: `JSONResponse` OR `config.DEFAULT_JSON_CLASS`
 - model_field_or_schema: `dict`
 - media_type: `application/json`
 
-## Custom Response Model
+## **Custom Response Model**
 
 Lets create a new JSON response model.
 
 ```python
 # project_name/apps/items/controllers.py
 
 import typing as t
```

### Comparing `ellar-0.4.0/docs/handling-response/response.md` & `ellar-0.4.2/docs/techniques/serializers.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-## Introduction
+# **Serializers**
 The `Serializer` class in the Ellar, is a custom class based on `pydantic` models, which provides additional functionality specific to Ellar's requirements.
 
 To use `Serializer` in Ellar, you simply need to create a class that inherits from `Serializer` and define your data model using pydantic fields. 
 Here's an example of how you could define a serializer class for a user model:
 
 ```python
 from ellar.common import Serializer
@@ -13,15 +13,15 @@
     age: int
 
 ```
 
 With this setup, you can use the `UserSerializer` class to validate incoming data and or serialize outgoing response data, 
 ensuring that it matches the expected format before saving it to the database or returning it to the client.
 
-## Handling Responses
+## **Handling Responses**
 
 Let's see how we can use **Serializer** as a responses schema which will help us validate out data output and also provide documentation on route function response.
 
 The response schema is defined on the HTTP method decorator.
 
 For example:
 ```python
@@ -64,18 +64,18 @@
 This code sets up a User model and a `UserSerializer` class based on the `Serializer` class. 
 The User model represents a user with a `username`, `email`, `first_name`, and `last_name`. 
 The `UserSerializer` class is used to define the expected format of the response data in the `/me` endpoint.
 
 When the `/me` endpoint is called, it returns the `current_user` object as the response. 
 The `UserSerializer` is then used to parse and validate the `current_user` object, converting it into a dictionary representation 
 that can be easily serialized to JSON. 
-The resulting dictionary is then passed to the [`JSONResponseModel`](./response-model/#jsonresponsemodel) for serialization to a 
+The resulting dictionary is then passed to the [`JSONResponseModel`](../response-model/#jsonresponsemodel) for serialization to a 
 JSON string and sending the response to the client.
 
-## Using Dataclass as Response Schema
+## **Using Dataclass as Response Schema**
 We can utilize the `dataclasses` feature as a response schema by utilizing the `DataclassSerializer` a base class. 
 
 For instance, we can convert the `UserSchema` to a dataclass by defining `UserDataclass` as follows:
 
 ```python
 from dataclasses import dataclass
 from ellar.common import DataclassSerializer
@@ -88,15 +88,15 @@
     first_name: str = None
     last_name: str = None
 
 ```
 
 By replacing the `UserSchema` with `UserDataclass`, we can expect the same outcomes in the returned response, response validation, and documentation.
 
-### Multiple Response Types
+### **Multiple Response Types**
 
 The `response` parameter takes different shape. Let's see how to return a different response if the user is not authenticated.
 
 ```python
 # project_name/apps/items/controllers.py
 
 from ellar.common import Controller, get, ControllerBase, Serializer
@@ -152,15 +152,15 @@
 Here, the `response` parameter takes a KeyValuePair of the `status` and response `Schema`.
 
 !!! info
     Note that we returned a tuple of status code and response data (`403, {"message": "Please sign in first"}`) to specify the response validation to use.
 
 
 
-## Using Response Type/Object As Response
+## **Using Response Type/Object As Response**
 
 You can use `Response` type to change the format of data returned from endpoint functions.
 
 ```python
 # project_name/apps/items/controllers.py
 
 from ellar.common import Controller, get, ControllerBase, PlainTextResponse
```

### Comparing `ellar-0.4.0/docs/img/EllarLogoB.png` & `ellar-0.4.2/docs/img/EllarLogoB.png`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/docs/img/EllarLogoIconOnly.png` & `ellar-0.4.2/docs/img/EllarLogoIconOnly.png`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/docs/img/EllarLogoW.png` & `ellar-0.4.2/docs/img/EllarLogoW.png`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/docs/img/Icon.svg` & `ellar-0.4.2/docs/img/Icon.svg`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/docs/img/Logo.svg` & `ellar-0.4.2/docs/img/Logo.svg`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/docs/img/ModuleDescription.png` & `ellar-0.4.2/docs/img/ModuleDescription.png`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/docs/img/body-schema-doc.png` & `ellar-0.4.2/docs/img/body-schema-doc.png`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/docs/img/body-schema-doc2.png` & `ellar-0.4.2/docs/img/body-schema-doc2.png`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/docs/img/body-schema-doc3.png` & `ellar-0.4.2/docs/img/body-schema-doc3.png`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/docs/img/car_api.png` & `ellar-0.4.2/docs/img/car_api.png`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/docs/img/car_controller.gif` & `ellar-0.4.2/docs/img/car_controller.gif`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/docs/img/controller_description.png` & `ellar-0.4.2/docs/img/controller_description.png`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/docs/img/create-car-schema.png` & `ellar-0.4.2/docs/img/create-car-schema.png`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/docs/img/create-dog-schema.png` & `ellar-0.4.2/docs/img/create-dog-schema.png`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/docs/img/ellar_demo.gif` & `ellar-0.4.2/docs/img/ellar_demo.gif`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/docs/img/ellar_framework.png` & `ellar-0.4.2/docs/img/ellar_framework.png`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/docs/img/enum_docs_swagger.png` & `ellar-0.4.2/docs/img/enum_docs_swagger.png`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/docs/img/event_docs_swagger.png` & `ellar-0.4.2/docs/img/event_docs_swagger.png`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/docs/img/form-schema-doc.png` & `ellar-0.4.2/docs/img/form-schema-doc.png`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/docs/img/json_api_response_model.png` & `ellar-0.4.2/docs/img/json_api_response_model.png`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/docs/img/live_support_websocket.gif` & `ellar-0.4.2/docs/img/live_support_websocket.gif`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/docs/img/live_support_websocket_3.gif` & `ellar-0.4.2/docs/img/live_support_websocket_3.gif`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/docs/img/math_router.png` & `ellar-0.4.2/docs/img/math_router.png`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/docs/img/math_router_with_request_object.png` & `ellar-0.4.2/docs/img/math_router_with_request_object.png`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/docs/img/middleware.png` & `ellar-0.4.2/docs/img/middleware.png`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/docs/img/query_filter_swagger.png` & `ellar-0.4.2/docs/img/query_filter_swagger.png`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/docs/img/response_description.png` & `ellar-0.4.2/docs/img/response_description.png`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/docs/index.md` & `ellar-0.4.2/docs/index.md`

 * *Files 3% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 [![PyPI version](https://img.shields.io/pypi/pyversions/ellar.svg)](https://pypi.python.org/pypi/ellar)
 
 ---
 ## **Introduction**
 Ellar is a lightweight ASGI framework for building efficient and scalable server-side python applications.
 It supports both OOP (Object-Oriented Programming) and FP (Functional Programming)
 
-Ellar is also a higher level of abstraction of [Starlette (ASGI toolkit)](https://www.starlette.io/), a lightweight ASGI framework/toolkit well-suited for developing asynchronous web services in Python.
+Ellar is also a higher level of abstraction of [Starlette (ASGI toolkit)](https://www.starlette.io/){target="_blank"}, a lightweight ASGI framework/toolkit well-suited for developing asynchronous web services in Python.
 
 ## **Inspiration**
-Ellar was deeply influenced by [NestJS](https://docs.nestjs.com/) for its ease of use, project structures and patterns that aids in building small or complex project applications.
-Also, Ellar took some concepts from [FastAPI](https://fastapi.tiangolo.com/) in terms of request parameter handling and data serialization with Pydantic. 
+Ellar was deeply influenced by [NestJS](https://docs.nestjs.com/){target="_blank"} for its ease of use, project structures and patterns that aids in building small or complex project applications.
+Also, Ellar took some concepts from [FastAPI](https://fastapi.tiangolo.com/){target="_blank"} in terms of request parameter handling and data serialization with Pydantic. 
 
 The objective of Ellar is to provide a high level of abstracted interface to the web, along with a well-structured project setup, give room for object-oriented approach to web application design, 
 allow you chose your desired application architecture, and ultimately, deliver speedy handling to requests.
 
 As developers, we never know how big a project can become or evolve over time but following some design patterns and architecture makes it easier to build a more testable and maintainable application.
 
 
@@ -38,15 +38,15 @@
 - **OpenAPI Documentation**: It comes with built-in support for OpenAPI documentation, making it easy to generate `Swagger` or `ReDoc` documentation for your API. And more can be added with ease if necessary.
 - **Controller (MVC) Architecture**: Ellar's controller architecture follows the Model-View-Controller (MVC) pattern, making it easy to organize your code.
 - **Guards for Authentication and Authorization**: It provides built-in support for guards, allowing you to easily implement authentication and authorization in your application.
 - **Modularity**: Ellar follows a modular architecture inspired by NestJS, making it easy to organize your code into reusable modules.
 - **Asynchronous programming**: It allows you to takes advantage of Python's `async/await` feature to write efficient and fast code that can handle large numbers of concurrent requests
 
 ## **Installation**
-To get started, you need to scaffold a project using [Ellar-CLI](https://eadwincode.github.io/ellar-cli/) toolkit. This is recommended for a first-time user.
+To get started, you need to scaffold a project using [Ellar-CLI](https://eadwincode.github.io/ellar-cli/){target="_blank"} toolkit. This is recommended for a first-time user.
 The scaffolded project is more like a guide to project setup.
 
 ```shell
 $(venv) pip install ellar
 ```
 
 After that, lets create a new project. 
@@ -56,23 +56,22 @@
 ```
 
 then, start the app with:
 ```shell
 $(venv) ellar runserver --reload
 ```
 
-Open your browser and navigate to [`http://localhost:8000/`](http://localhost:8000/).
+Open your browser and navigate to [`http://localhost:8000/`](http://localhost:8000/){target="_blank"}.
 ![Swagger UI](img/ellar_framework.png)
 
 ## **Dependency Summary**
 - `Python >= 3.7`
 - `Starlette`
 - `Pydantic`
 - `Injector`
 
 ## **Status**
 
 Project is still in development
 
 - Documentation - in progress
-- Interceptors  -  [Aspect Oriented Programming](https://en.wikipedia.org/wiki/Aspect-oriented_programming) (AOP) technique
-- Database Plugin with [Encode/ORM](https://github.com/encode/orm)
+- Database Plugin with [Encode/ORM](https://github.com/encode/orm){target="_blank"}
```

#### html2text {}

```diff
@@ -8,52 +8,53 @@
 badge.fury.io/py/ellar) [![PyPI version](https://img.shields.io/pypi/v/
 ellar.svg)](https://pypi.python.org/pypi/ellar) [![PyPI version](https://
 img.shields.io/pypi/pyversions/ellar.svg)](https://pypi.python.org/pypi/ellar)
 --- ## **Introduction** Ellar is a lightweight ASGI framework for building
 efficient and scalable server-side python applications. It supports both OOP
 (Object-Oriented Programming) and FP (Functional Programming) Ellar is also a
 higher level of abstraction of [Starlette (ASGI toolkit)](https://
-www.starlette.io/), a lightweight ASGI framework/toolkit well-suited for
-developing asynchronous web services in Python. ## **Inspiration** Ellar was
-deeply influenced by [NestJS](https://docs.nestjs.com/) for its ease of use,
-project structures and patterns that aids in building small or complex project
-applications. Also, Ellar took some concepts from [FastAPI](https://
-fastapi.tiangolo.com/) in terms of request parameter handling and data
-serialization with Pydantic. The objective of Ellar is to provide a high level
-of abstracted interface to the web, along with a well-structured project setup,
-give room for object-oriented approach to web application design, allow you
-chose your desired application architecture, and ultimately, deliver speedy
-handling to requests. As developers, we never know how big a project can become
-or evolve over time but following some design patterns and architecture makes
-it easier to build a more testable and maintainable application. ## **Features
-Summary** - **Easy to Use**: Ellar has a simple and intuitive API that makes it
-easy to get started with building a fast and scalable web applications or web
-APIs with Python. - **Dependency Injection (DI)**: It comes with DI system
-makes it easy to manage dependencies and reduce coupling between components. -
-**Pydantic Integration**: It is properly integrated with Pydantic, a popular
-Python library for data validation, to ensure that input data is valid. -
-**Templating with Jinja2**: Ellar provides built-in support for Jinja2
-templates, making it easy to create dynamic web pages. - **OpenAPI
-Documentation**: It comes with built-in support for OpenAPI documentation,
-making it easy to generate `Swagger` or `ReDoc` documentation for your API. And
-more can be added with ease if necessary. - **Controller (MVC) Architecture**:
-Ellar's controller architecture follows the Model-View-Controller (MVC)
-pattern, making it easy to organize your code. - **Guards for Authentication
-and Authorization**: It provides built-in support for guards, allowing you to
-easily implement authentication and authorization in your application. -
-**Modularity**: Ellar follows a modular architecture inspired by NestJS, making
-it easy to organize your code into reusable modules. - **Asynchronous
-programming**: It allows you to takes advantage of Python's `async/await`
-feature to write efficient and fast code that can handle large numbers of
-concurrent requests ## **Installation** To get started, you need to scaffold a
-project using [Ellar-CLI](https://eadwincode.github.io/ellar-cli/) toolkit.
-This is recommended for a first-time user. The scaffolded project is more like
-a guide to project setup. ```shell $(venv) pip install ellar ``` After that,
-lets create a new project. Run the command below and change the `project-name`
-with whatever name you decide. ```shell $(venv) ellar new project-name ```
-then, start the app with: ```shell $(venv) ellar runserver --reload ``` Open
-your browser and navigate to [`http://localhost:8000/`](http://localhost:8000/
-). ![Swagger UI](img/ellar_framework.png) ## **Dependency Summary** - `Python
->= 3.7` - `Starlette` - `Pydantic` - `Injector` ## **Status** Project is still
-in development - Documentation - in progress - Interceptors - [Aspect Oriented
-Programming](https://en.wikipedia.org/wiki/Aspect-oriented_programming) (AOP)
-technique - Database Plugin with [Encode/ORM](https://github.com/encode/orm)
+www.starlette.io/){target="_blank"}, a lightweight ASGI framework/toolkit well-
+suited for developing asynchronous web services in Python. ## **Inspiration**
+Ellar was deeply influenced by [NestJS](https://docs.nestjs.com/)
+{target="_blank"} for its ease of use, project structures and patterns that
+aids in building small or complex project applications. Also, Ellar took some
+concepts from [FastAPI](https://fastapi.tiangolo.com/){target="_blank"} in
+terms of request parameter handling and data serialization with Pydantic. The
+objective of Ellar is to provide a high level of abstracted interface to the
+web, along with a well-structured project setup, give room for object-oriented
+approach to web application design, allow you chose your desired application
+architecture, and ultimately, deliver speedy handling to requests. As
+developers, we never know how big a project can become or evolve over time but
+following some design patterns and architecture makes it easier to build a more
+testable and maintainable application. ## **Features Summary** - **Easy to
+Use**: Ellar has a simple and intuitive API that makes it easy to get started
+with building a fast and scalable web applications or web APIs with Python. -
+**Dependency Injection (DI)**: It comes with DI system makes it easy to manage
+dependencies and reduce coupling between components. - **Pydantic
+Integration**: It is properly integrated with Pydantic, a popular Python
+library for data validation, to ensure that input data is valid. - **Templating
+with Jinja2**: Ellar provides built-in support for Jinja2 templates, making it
+easy to create dynamic web pages. - **OpenAPI Documentation**: It comes with
+built-in support for OpenAPI documentation, making it easy to generate
+`Swagger` or `ReDoc` documentation for your API. And more can be added with
+ease if necessary. - **Controller (MVC) Architecture**: Ellar's controller
+architecture follows the Model-View-Controller (MVC) pattern, making it easy to
+organize your code. - **Guards for Authentication and Authorization**: It
+provides built-in support for guards, allowing you to easily implement
+authentication and authorization in your application. - **Modularity**: Ellar
+follows a modular architecture inspired by NestJS, making it easy to organize
+your code into reusable modules. - **Asynchronous programming**: It allows you
+to takes advantage of Python's `async/await` feature to write efficient and
+fast code that can handle large numbers of concurrent requests ##
+**Installation** To get started, you need to scaffold a project using [Ellar-
+CLI](https://eadwincode.github.io/ellar-cli/){target="_blank"} toolkit. This is
+recommended for a first-time user. The scaffolded project is more like a guide
+to project setup. ```shell $(venv) pip install ellar ``` After that, lets
+create a new project. Run the command below and change the `project-name` with
+whatever name you decide. ```shell $(venv) ellar new project-name ``` then,
+start the app with: ```shell $(venv) ellar runserver --reload ``` Open your
+browser and navigate to [`http://localhost:8000/`](http://localhost:8000/)
+{target="_blank"}. ![Swagger UI](img/ellar_framework.png) ## **Dependency
+Summary** - `Python >= 3.7` - `Starlette` - `Pydantic` - `Injector` ##
+**Status** Project is still in development - Documentation - in progress -
+Database Plugin with [Encode/ORM](https://github.com/encode/orm)
+{target="_blank"}
```

### Comparing `ellar-0.4.0/docs/mount.md` & `ellar-0.4.2/docs/techniques/mount.md`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/docs/overview/controllers.md` & `ellar-0.4.2/docs/overview/controllers.md`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/docs/overview/custom_decorators.md` & `ellar-0.4.2/docs/overview/custom_decorators.md`

 * *Files 3% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 - `Form(..., embed=True)`
 - `Query(...)`
 - `File(...)`
 - `Path(...)`
 - `Header(...)`
 - `Cookie(...)`
 
-Please refer to the "How-to-Guide" on parsing inputs [here](/ellar/parsing-inputs/) to see how this input decorators work. 
+Please refer to the "How-to-Guide" on parsing inputs [here](../../techniques/validations){target="_blank"} to see how this input decorators work. 
 
 ### **WsBody(..., embed=False)**
 
 `WsBody(...)` is a decorator that defines the message format that should be transmitted from the client in a WebSocket when there is a successful connection. 
 This decorator can be used to specify the structure of the message that is sent over the WebSocket, and to validate the message against a specified schema
 but for only `use_extra_handler=True`.
 
@@ -92,15 +92,15 @@
 It also makes the code more modular and easier to test.
 
 !!! info
     Only types registered in the application can be resolved, but you can set `INJECTOR_AUTO_BIND = True` in configuration for the injector to register automatically that are not found. 
     please note that this automatic registration will be scoped to singleton by the `EllarInjector`.
 
 ### **Context**
-The **Context()** decorator injects the current `IExecutionContext` to route function parameter. See [ExecutionContext](/basics/execution-context)
+The **Context()** decorator injects the current `IExecutionContext` to route function parameter. See [ExecutionContext](../../basics/execution-context){target="_blank"}
 
 For example:
 ```python
 from ellar.common import ModuleRouter, Context
 
 router = ModuleRouter('/test-context')
 
@@ -172,15 +172,15 @@
 ```
 The above code creates a WebSocket route '/test-ws' and when a client connects to this route, 
 the `example_endpoint` function is executed. The `Ws` decorator injects the current `WebSocket` object to the `ws` parameter of the function, which can then be used to interact with the WebSocket connection, such as accepting the connection and sending data to the client.
 
 The same conditions and examples applies for:
 
 - **Host()** decorator injects current client host address to route function parameter.
-- **Session()** decorator injects current Session object to route function parameter. This requires [SessionMiddleware](https://www.starlette.io/middleware/#sessionmiddleware) module from Starlette added in application middleware and also `SessionMiddleware` module depends on [itsdangerous](https://pypi.org/project/itsdangerous/) package.
+- **Session()** decorator injects current Session object to route function parameter. This requires [SessionMiddleware](https://www.starlette.io/middleware/#sessionmiddleware){target="_blank"} module from Starlette added in application middleware and also `SessionMiddleware` module depends on [itsdangerous](https://pypi.org/project/itsdangerous/){target="_blank"} package.
 - **Http()** decorator injects current HTTP connection object to route function parameter.
 
 ## **Creating a Custom Parameter Decorators**
 You can still create your own route parameter decorators that suits your need. You simply need to follow a contract, `NonParameterResolver`, and override the resolve function.
 
 The `NonParameterResolver` has two attribute, `type_annotation` and `parameter_name`, that are provided automatically when computing route parameter dependencies. 
 They are gotten from the application of the NonParameterResolver, like so - `def s(parameter_name:type_annotation = NonParameterResolver())`.
@@ -238,15 +238,15 @@
 
 In the example, the index function is decorated with the `render` decorator, 
 which will return a 200 status code and HTML content from my_template. 
 
 The return object from the index function will be used as the templating context for `my_template` during the template rendering process. 
 This allows the function to pass data to the template and have it rendered with the provided context, the rendered template will be the response body.
 
-See [HTML Templating](/ellar/templating/templating) for more information on `render` and HTML templating with Ellar.
+See [HTML Templating](../../templating/templating){target="_blank"} for more information on `render` and HTML templating with Ellar.
 
 ### **FILE**
 **@file()** decorator converts a route function response to file or streaming response type. 
 Based on the value of `streaming` parameter, file decorator creates `FileResponseModel` or `StreamingResponseModel`.
 
 #### FileResponseModel as file(streaming=False)
 When `streaming` parameter in `@file(streaming=False)` decorator is set to `False`, a `FileResponseModel` is created as the response model for the decorated route function. 
@@ -374,22 +374,22 @@
 @get("/serialize-filter-1", response=UserSchema)
 @serializer_filter(exclude_none=True, exclude={'password'})
 def serialized_output_1(self):
     return dict(username='python', password='secret', first_name='ellar')
 
 ```
 In example, `serializer_filter` to filter values that are `None` and also excluded `password` property from been returned.
-See [Pydantic Model Export](https://docs.pydantic.dev/usage/exporting_models/#modeldict) for more examples.
+See [Pydantic Model Export](https://docs.pydantic.dev/usage/exporting_models/#modeldict){target="_blank"} for more examples.
 
 ### **VERSION**
 **@version()**  is a decorator that provides endpoint versioning for a route function. 
 This decorator allows you to specify the version of the endpoint that the function is associated with. 
 
 Based on the versioning scheme configuration in the application, versioned route functions are called. This can be useful for maintaining backward compatibility, or for rolling out new features to different versions of an application. 
-More information on how to use this decorator can be found in the [Versioning documentation]()
+More information on how to use this decorator can be found in the [Versioning documentation](../../techniques/versioning){target="_blank"}
 
 A quick example on how to use `version` decorator:
 ```python
 from ellar.common import post, Version
 
 @post("/create", name='v2_v3_list')
 @Version('2', '3')
@@ -404,15 +404,15 @@
 ### **UseGuards**
 **@UseGuards()**  is a decorator that applies a protection class of type `GuardCanActivate` to a route function. 
 These protection classes have a `can_execute` function that is called to determine whether a route function should be executed. 
 
 This decorator allows you to apply certain conditions or checks before a route function is executed, such as `authentication` or `authorization` checks. 
 This can help to ensure that only authorized users can access certain resources. 
 
-More information on how to use this decorator can be found in the [Guard Documentation]()
+More information on how to use this decorator can be found in the [Guard Documentation](../guards){target="_blank"}
 
 A quick example on how to use `UseGuards` decorator:
 ```python
 import typing as t
 from ellar.common import get, UseGuards
 from ellar.core import APIKeyQuery, HTTPConnection
 
@@ -437,21 +437,21 @@
 
 Each guard class has a `can_execute` function that is called in the order specified by the decorator, if any of the guard's `can_execute` function returns False, the route function will not be executed.
 
 ## **Command Decorators**
 The `command` decorator is used to convert a decorated function into a command that can be executed through the Ellar command-line interface (CLI) actions. 
 This allows you to define custom commands that can be run from the command-line, which can be useful for tasks such as running database migrations, generating code, or other tasks that can be automated.
 
-See [Ellar-CLI Custom Commands](https://eadwincode.github.io/ellar-cli/custom-commands/)
+See [Ellar-CLI Custom Commands](../../cli){target="_blank"}
 
 ## **Module Function Decorators**
 
 - `@exception_handler`: This decorator is used to register a function as an exception handler. This function will be called when an unhandled exception occurs during a request. It should take the exception instance as its only argument and return a response object.
 
 - `@middleware`: This decorator is used to register a function as a middleware. Middlewares are called for each incoming request and can be used to modify the request or response, or perform any other actions before or after the request is handled.
 
 - `@template_filter`: This decorator is used to register a function as a Jinja2 template filter. The function should take one or more arguments and return a modified value.
 
 - `@template_global`: This decorator is used to register a function as a global variable available in all Jinja2 templates. The function can be called without any arguments and should return a value.
 
 These decorators can be used to define functions that will be executed at specific points in the application's lifecycle. 
-They provide a way to separate and organize the different parts of an application. See [Module Additional Configuration](../modules/#additional-module-configurations) for examples on how these decorator functions are used.
+They provide a way to separate and organize the different parts of an application. See [Module Additional Configuration](../modules/#additional-module-configurations){target="_blank"} for examples on how these decorator functions are used.
```

### Comparing `ellar-0.4.0/docs/overview/exception_handling.md` & `ellar-0.4.2/docs/overview/exception_handling.md`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 ## **WebSocketException**
 
 You can use the `WebSocketException` class to raise errors inside WebSocket endpoints.
 
 * `WebSocketException(code=1008, reason=None)`
 
-You can set any code valid as defined [in the specification](https://tools.ietf.org/html/rfc6455#section-7.4.1).
+You can set any code valid as defined [in the specification](https://tools.ietf.org/html/rfc6455#section-7.4.1){target="_blank"}.
 
 ## **APIException**
 It is a type of exception for REST API based applications. It gives more concept to error and provides a simple interface for creating other custom exception needs in your application without having to create an extra exception handler.
 
 For example,
 
 ```python
@@ -56,15 +56,15 @@
 # project_name/apps/car/controllers.py
 
 @get()
 def get_all(self):
     raise ServiceUnavailableException()
 
 ```
-Now, when you visit [http://127.0.0.1/car/](http://127.0.0.1/car/), you will get a JSON response.
+Now, when you visit [http://127.0.0.1/car/](http://127.0.0.1/car/){target="_blank"}, you will get a JSON response.
 ```json
 {
   "detail": "Service Unavailable"
 }
 ```
 
 When we raise the `ServiceUnavailableException` exception type, it produces a `JSON` response because `Ellar` has implemented an exception handler for any `APIException` exception type.
```

### Comparing `ellar-0.4.0/docs/overview/guards.md` & `ellar-0.4.2/docs/overview/guards.md`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/docs/overview/index.md` & `ellar-0.4.2/docs/overview/index.md`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,15 @@
 )
 ```
 
 There are two ways to create an Ellar application using the `AppFactory`, `create_from_app_module` and `create_app`.
 Both provides all necessary parameter for creating Ellar application
 
 ## **Run your project**
-Ellar runs [UVICORN - ASGI Server](https://www.uvicorn.org/) under the hood.
+Ellar runs [UVICORN - ASGI Server](https://www.uvicorn.org/){target="_blank"} under the hood.
 
 ```shell
 $(venv) cd project-name
 $(venv) ellar runserver --reload
 ```
 `--reload` is to watch for file changes
 
@@ -86,18 +86,18 @@
 INFO:     Started reloader process [2934815] using WatchFiles
 INFO:     APP SETTINGS MODULE: project_name.config:DevelopmentConfig
 INFO:     Started server process [2934818]
 INFO:     Waiting for application startup.
 INFO:     Application startup complete.
 ```
 
-Now go to [http://127.0.0.1:8000](http://127.0.0.1:8000)
+Now go to [http://127.0.0.1:8000](http://127.0.0.1:8000){target="_blank"}
 ![Swagger UI](../img/ellar_framework.png)
 
-For more info on Ellar CLI, click [here](https://github.com/eadwinCode/ellar-cli)
+For more info on Ellar CLI, click [here](https://github.com/eadwinCode/ellar-cli){target="_blank"}
 
 To run the application with a different configuration,
 In `project_name/config`, Add a `ProductionConfig`
 
 ```python
 ...
 
@@ -163,15 +163,15 @@
 class ApplicationModule(ModuleBase):
     @exception_handler(404)
     def exception_404_handler(cls, request: Request, exc: Exception) -> Response:
         return JSONResponse(dict(detail="Resource not found."))
 ```
 That's it.
 
-Goto your browser and visit: [http://localhost:8000/car/](http://localhost:8000/car/)
+Goto your browser and visit: [http://localhost:8000/car/](http://localhost:8000/car/){target="_blank"}
 ```json
 {
   "detail": "Welcome Car Resource"
 }
 ```
 
 ## **Enabling OpenAPI Docs**
@@ -204,8 +204,8 @@
     document_generator=SwaggerDocumentGenerator(),
     document=document,
     guards=[]
 )
 application.install_module(module_config)
 ```
 
-Goto your browser and visit: [http://localhost:8000/docs/](http://localhost:8000/docs)
+Goto your browser and visit: [http://localhost:8000/docs/](http://localhost:8000/docs){target="_blank"}
```

### Comparing `ellar-0.4.0/docs/overview/interceptors.md` & `ellar-0.4.2/docs/overview/interceptors.md`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 - transform the result returned from a function
 - transform the exception thrown from a function
 - extend the basic function behavior
 - completely override a function depending on specific conditions (e.g., for caching purposes)
 
 ## **Basic**
 Each interceptor implements the `intercept()` method, which takes two arguments. 
-The first one is the `ExecutionContext` instance (exactly the same object as for [guards](./guards)) and 
+The first one is the `ExecutionContext` instance (exactly the same object as for [guards](../guards){target="_blank"}) and 
 `next_interceptor` awaitable function that executes the next interceptor in the execution chain.
 
 ```python
 import typing as t
 from abc import ABC, abstractmethod
 from ellar.common import IExecutionContext
 
@@ -32,15 +32,15 @@
 ```
 !!! note
     `intercept` function of interceptor class is an asynchronous function.
 
 ## **Execution context**
 The `ExecutionContext` adds several new helper methods that provide additional details about the current execution process. 
 These details can be helpful in building more generic interceptors that can work across a broad set of controllers, methods, and execution contexts. 
-Learn more about `ExecutionContext` [here](../basics/execution-context).
+Learn more about `ExecutionContext` [here](../../basics/execution-context){target="_blank"}.
 
 ## **Next Interceptor Handler**
 The second argument, `next_interceptor`,  in `intercept` of EllarInterceptor class is used to invoke the route handler method at some point in your interceptor.
 If you don't call the `next_interceptor` method in your implementation of the `intercept()` method, the route handler method won't be executed at all.
 
 This approach means that the `intercept()` method effectively wraps the request/response cycle. 
 As a result, you may implement custom logic **both before and after** the execution of the final route handler.
```

### Comparing `ellar-0.4.0/docs/overview/middleware.md` & `ellar-0.4.2/docs/overview/middleware.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # **Middlewares**
 Middlewares are functions that are called during requests before hitting a specific route handler.
 Middleware functions can modify **request** and **response** objects during the `HTTP` or `WebSocket` connection. 
 
 ![middleware description image](../img/middleware.png)
 
-Ellar Middlewares follows the [`Starlette ASGI Middleware`](https://www.starlette.io/middleware/) contract. The middlewares are set up in a pipeline fashion that creates a chain of request-response cycles.
+Ellar Middlewares follows the [`Starlette ASGI Middleware`](https://www.starlette.io/middleware/){target="_blank"} contract. The middlewares are set up in a pipeline fashion that creates a chain of request-response cycles.
 
 During request, each `ASGI` Middleware must call another ASGI `app` passed to it during the middlewares instantiation and `await` its response. 
 
 !!!info
     An `ASGI` type is any callable that takes `scope`, `receive` and `send` as arguments
     ```python
     
@@ -161,15 +161,15 @@
 `ALLOWED_HOSTS` - A list of domain names that should be allowed as hostnames. 
 Wildcard domains such as `*.example.com` are supported for matching subdomains. 
 To allow any hostname either use `allowed_hosts=["*"]` or omit the middleware.
 
 If an incoming request does not validate correctly then a `400` response will be sent.
 
 ### **`CORSMiddleware`**
-Adds appropriate [`CORS headers`](https://developer.mozilla.org/en-US/docs/Web/HTTP/CORS) to outgoing responses in order to allow cross-origin requests from browsers.
+Adds appropriate [`CORS headers`](https://developer.mozilla.org/en-US/docs/Web/HTTP/CORS){target="_blank"} to outgoing responses in order to allow cross-origin requests from browsers.
 
 Since `CORSMiddleware` is part of default application middleware, let's see how to configure CORS arguments in ellar application.
 
 ```python
 # project_name/config.py
 import typing as t
 ...
@@ -212,15 +212,15 @@
 
 
 ### **`Other Middlewares`**
 
 There are many other ASGI middlewares.
 For example:
 
-- [Sentry](https://docs.sentry.io/platforms/python/asgi/)
-- [Uvicorn's ProxyHeadersMiddleware](https://github.com/encode/uvicorn/blob/master/uvicorn/middleware/proxy_headers.py)
-- [MessagePack](https://github.com/florimondmanca/msgpack-asgi)
+- [Sentry](https://docs.sentry.io/platforms/python/asgi/){target="_blank"}
+- [Uvicorn's ProxyHeadersMiddleware](https://github.com/encode/uvicorn/blob/master/uvicorn/middleware/proxy_headers.py){target="_blank"}
+- [MessagePack](https://github.com/florimondmanca/msgpack-asgi){target="_blank"}
 
-To see other available middlewares check [Starlette's Middleware docs](https://www.starlette.io/middleware/)  and the [ASGI Awesome List](https://github.com/florimondmanca/awesome-asgi).
+To see other available middlewares check [Starlette's Middleware docs](https://www.starlette.io/middleware/){target="_blank"}  and the [ASGI Awesome List](https://github.com/florimondmanca/awesome-asgi){target="_blank"}.
 
 !!! note "Technical Details"
     Most of the available middlewares come directly from Starlette. Ellar provides few required for its basic functionalities
```

### Comparing `ellar-0.4.0/docs/overview/module-router.md` & `ellar-0.4.2/docs/overview/module-router.md`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 
 ![math_router.png](../img/math_router.png)
 
 
 ## **Accessing Other Request Object**
 In functional route handle, we can access request object and response object through custom decorators or type annotation as shown below.
 
-### By Type Annotation
+### **By Type Annotation**
 Let's inject request and response object in `addition` route handler function from our previous example
 
 ```python
 from ellar.core import Request
 from ellar.common import ModuleRouter, Response
```

### Comparing `ellar-0.4.0/docs/overview/providers.md` & `ellar-0.4.2/docs/overview/modules.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,343 +1,241 @@
-# **Providers**
-A provider is any class or object that is **injectable** as a dependency to another class, and it's required when creating an instance of that class.
+# **Modules**
 
-Providers are like services, repositories services, factories, etc., classes that manage complex tasks. These providers can be made available to a controller, a route handler, or to another provider as a dependency. This concept is known as [Dependency Injector](https://en.wikipedia.org/wiki/Dependency_injection)
+A module is a class annotated with a `@Module()` decorator.
+The `@Module()` decorator provides **metadata** that exports a `Module` data and defines the module structure.
 
-You can easily create a provider class by decorating that class with the `@injectable()` mark and stating the scope.
+![middleware description image](../img/ModuleDescription.png)
 
-```python
-from ellar.di import injectable, singleton_scope
-
-
-@injectable(scope=singleton_scope)
-class UserRepository:
-    pass
-```
-
-We have created a `UserRepository` provider that will help manage the loading and saving of user data to the database.
-
-Let's add this service to a controller.
-
-```python
-from ellar.di import injectable, singleton_scope
-from ellar.common import Controller, ControllerBase
-
-
-@injectable(scope=singleton_scope)
-class UserRepository:
-    pass
-
-
-@Controller()
-class UserController(ControllerBase):
-    def __init__(self, user_repo: UserRepository) -> None:
-        self.user_repo = user_repo
-```
-Let's refactor our `CarController` and move some actions to a service.
-
-```python
-# project_name/apps/car/services.py
-import typing as t
-from ellar.di import injectable, singleton_scope
-from .schemas import CreateCarSerializer, CarSerializer
-
-
-@injectable(scope=singleton_scope)
-class CarRepository:
-    def __init__(self):
-        self._cars: t.List[CarSerializer] = []
-
-    def create_car(self, data: CreateCarSerializer) -> dict:
-        data = CarSerializer(id=len(self._cars) + 1, **data.dict())
-        self._cars.append(data)
-        return data.dict()
-
-
-    def get_all(self) -> t.List[CarSerializer]:
-        return self._cars
-
-```
-
-We have successfully created a `CarRepository` with a `singleton` scope.
-
-Let's wire it up to `CarController`. And rewrite some route handles.
-
-```python
-# project_name/apps/car/controllers.py
-
-from ellar.common import Body, Controller, get, post, Query, ControllerBase
-from .schemas import CreateCarSerializer, CarListFilter
-from .services import CarRepository
-
-
-@Controller('/car')
-class CarController(ControllerBase):
-    def __init__(self, repo: CarRepository):
-        self.repo = repo
-    
-    @post()
-    async def create(self, payload: CreateCarSerializer = Body()):
-        result = self.repo.create_car(payload)
-        result.update(message='This action adds a new car')
-        return result
-
-    @get()
-    async def get_all(self, query: CarListFilter = Query()):
-        res = dict(
-            cars=self.repo.get_all(), 
-            message=f'This action returns all cars at limit={query.limit}, offset={query.offset}')
-        return res
+The best way to organize your components is to build your projects as `Modules`.
 
-    ...
-```
-
-We have defined `CarRepository` as a dependency to `CarController` and Ellar will resolve the `CarRepository` instance when creating the `CarController` instance.
+The `ApplicationModule` is the entry-point/root module to building the application module tree -
+the internal data structure used to resolve `module` and `provider` relationships and dependencies.
 
-!!! info
-    Every class dependency should be defined in the class **constructor**  as a type annotation or Ellar won't be aware of the dependencies required for an object instantiation.
+Thus, the architecture resulting from most applications will include multiple modules with closely related **functionality**.
 
-## **Provider Registration**
-To get this working, we need to expose the `CarRepository` to the `CarModule` module just like we did for the `CarController`.
+## **Feature modules**
+Building an application as a group of feature modules bundled together helps to manage complexity, have a maintainable, extendable, and testable code base, and encourage development using SOLID principles.
 
+A typical example of a feature module is the **car** project. The `CarModule` wraps all the services and controller that manages the `car` resource which makes it easy to maintain, extend, and testable.
 ```python
 # project_name/apps/car/module.py
 
 from ellar.common import Module
 from ellar.core import ModuleBase
 from ellar.di import Container
 from .services import CarRepository
 from .controllers import CarController
 
 
 @Module(
     controllers=[CarController],
     providers=[CarRepository],
-    routers=[],
 )
 class CarModule(ModuleBase):
     def register_providers(self, container: Container) -> None:
         # for more complicated provider registrations
         # container.register_instance(...)
         pass
 ```
 
-## **Provider Scopes**
-There are different scope which defines different ways a service is instantiated.
-
-### **`transient_scope`**: 
-Whenever a transient scoped provider is required, a new instance of the provider is created
+## **Module Parameters**
+Let's create a Module and take a quick overview of its parameters.
 
 ```python
-# main.py
-
-from ellar.di import EllarInjector, transient_scope, injectable
-
-injector = EllarInjector(auto_bind=False)
-
+from ellar.common import Module
+from ellar.core import ModuleBase
 
-@injectable(scope=transient_scope)
-class ATransientClass:
+@Module(
+    name='', 
+    modules=[], 
+    providers=[],
+    controllers=[],
+    routers=[],
+    commands=[],
+    base_directory=None, 
+    static_folder='static', 
+    template_folder='templates'
+)
+class BookModule(ModuleBase):
     pass
 
-injector.container.register(ATransientClass)
-# OR
-# injector.container.register_transient(ATransientClass)
-
-def validate_transient_scope():
-    a_transient_instance_1 = injector.get(ATransientClass)
-    a_transient_instance_2 = injector.get(ATransientClass)
-    
-    assert a_transient_instance_2 != a_transient_instance_1 # True
-
-    
-if __name__ == "__main__":
-    validate_transient_scope()
 ```
 
-### **`singleton_scope`**: 
-A singleton scoped provider is created once throughout the lifespan of the Container instance.
-
-For example:
-```python
-# main.py
+|                   |                                                                                                                              |
+|-------------------|------------------------------------------------------------------------------------------------------------------------------|
+| `name`            | name of the module - it's irrelevant at the moment.                                                                          |
+| `modules`         | List of Module dependencies                                                                                                  |
+| `providers`       | the providers that will be instantiated by the Ellar injector and that may be shared at least across this module             |
+| `controllers`     | the set of controllers defined in this module which have to be instantiated                                                  |
+| `routers`         | the set of `ModuleRouter` defined in this module                                                                             |
+| `commands`        | the set of `EllarTyper` or `command` decorated functions                                                                     |
+| `base_directory`  | root directory for this module to read `static_folder` and `template_folder`. Default is the root folder of the Module Class |
+| `static_folder`   | defines the static folder for this module - default: `static`                                                                |
+| `template_folder` | defines the template folder for this module - default: `templates`                                                           |
 
-from ellar.di import EllarInjector, singleton_scope, injectable
 
-injector = EllarInjector(auto_bind=False)
-# OR
+## **Additional Module Configurations**
 
-@injectable(scope=singleton_scope)
-class ASingletonClass:
-    pass
+### **Module Events**
+Every registered Module receives two event calls during its instantiation and when the application is ready.
 
-injector.container.register(ASingletonClass)
-# OR
-# injector.container.register_singleton(ASingletonClass)
-
-def validate_singleton_scope():
-    a_singleton_instance_1 = injector.get(ASingletonClass)
-    a_singleton_instance_2 = injector.get(ASingletonClass)
+```python
+from ellar.common import Module
+from ellar.core import ModuleBase, Config, App
 
-    assert a_singleton_instance_2 == a_singleton_instance_1 # True
+@Module()
+class ModuleEventSample(ModuleBase):
+    @classmethod
+    def before_init(cls, config: Config) -> None:
+        """Called before creating Module object"""
+    
+    def application_ready(self, app: App) -> None:
+        """Called when application is ready - this is similar to @on_startup event"""
 
-if __name__ == "__main__":
-    validate_singleton_scope()
 ```
+`before_init` receives current app `Config` as a parameter and `application_ready` function receives `App` instance as parameter.
 
-### **`request_scope`**: 
-A request scoped provider is instantiated once during the scope of the request. And it's destroyed once the request is complete.
-It is important to note that `request_scope` behaves like a `singleton_scope` during HTTPConnection mode and behaves like a `transient_scope` outside HTTPConnection mode.
+### **Module Exceptions**
+Custom exception handlers can be registered through modules.
 
 ```python
-# main.py
-
-import uvicorn
-from ellar.di import EllarInjector, request_scope, injectable
-
-injector = EllarInjector(auto_bind=False)
-
-
-@injectable(scope=request_scope)
-class ARequestScopeClass:
-    pass
-
-
-injector.container.register(ARequestScopeClass)
+from ellar.common import Module, exception_handler, JSONResponse, Response, IHostContext
+from ellar.core import ModuleBase
 
+@Module()
+class ModuleExceptionSample(ModuleBase):
+    @exception_handler(404)
+    def exception_404_handler(cls, context: IHostContext, exc: Exception) -> Response:
+        return JSONResponse(dict(detail="Resource not found."))
+```
+`exception_404_handler` will be register to the application at runtime during `ModuleExceptionSample` computation.
 
-async def scoped_request(scope, receive, send):
-    async with injector.create_asgi_args(scope, receive, send) as request_injector:
-        request_instance_1 = request_injector.get(ARequestScopeClass)
-        request_instance_2 = request_injector.get(ARequestScopeClass)
-        assert request_instance_2 == request_instance_1
+### **Module Templating Filters**
+We can also define `Jinja2` templating filters in project Modules or any `@Module()` module.
+The defined filters are be passed down to `Jinja2` **environment** instance alongside the `template_folder` 
+value when creating **TemplateLoader**.
 
-    request_instance_1 = injector.get(ARequestScopeClass)
-    request_instance_2 = injector.get(ARequestScopeClass)
+```python
 
-    assert request_instance_2 != request_instance_1
+from ellar.common import Module, template_global, template_filter
+from ellar.core import ModuleBase
 
+@Module()
+class ModuleTemplateFilterSample(ModuleBase):
+    @template_filter()
+    def double_filter(cls, n):
+        return n * 2
 
-if __name__ == "__main__":
-    uvicorn.run("main:scoped_request", port=5000, log_level="info")
+    @template_global()
+    def double_global(cls, n):
+        return n * 2
 
+    @template_filter(name="dec_filter")
+    def double_filter_dec(cls, n):
+        return n * 2
 ```
 
-## **Provider Configurations**
-There are two ways we can configure providers that are required in EllarInjector IoC.
+## **Dependency Injection**
+A module class can inject providers as well (e.g., for configuration purposes):
 
-### **`ProviderConfig`**:
-With `ProviderConfig`, we can register a `base_type` against a `concrete_type` OR register a `base_type` against a value type.
+For example, from our sample project, the can inject `Config` to the `CarModule`
 
-For example:
 ```python
-# main.py
+# project_name/apps/car/module.py
 
 from ellar.common import Module
-from ellar.core import ModuleBase, Config
-from ellar.di import ProviderConfig, injectable, EllarInjector
-from ellar.core.modules.ref import create_module_ref_factor
-
-injector = EllarInjector(auto_bind=False)
-
-
-class IFoo:
-    pass
-
-
-class IFooB:
-    pass
-
-
-@injectable
-class AFooClass(IFoo, IFooB):
-    pass
-
-
-a_foo_instance = AFooClass()
+from ellar.core import Config, ModuleBase
+from ellar.di import Container
+from .services import CarRepository
+from .controllers import CarController
 
 
 @Module(
-    providers=[
-        ProviderConfig(IFoo, use_class=AFooClass),
-        ProviderConfig(IFooB, use_value=a_foo_instance)
-    ]
+    controllers=[CarController],
+    providers=[CarRepository],
 )
-class AModule(ModuleBase):
-    def __init__(self, ifoo: IFoo, ifoo_b: IFooB):
-        self.ifoo = ifoo
-        self.ifoo_b = ifoo_b
-
-
-def validate_provider_config():
-    module_ref = create_module_ref_factor(
-    AModule, container=injector.container, config=Config(),
-    )
-    module_ref.run_module_register_services()
-    a_module_instance: AModule = injector.get(AModule)
-    
-    assert isinstance(a_module_instance.ifoo, AFooClass)
-    assert isinstance(a_module_instance.ifoo_b, AFooClass)
-    assert a_module_instance.ifoo_b == a_foo_instance
-
+class CarModule(ModuleBase):
+    def __init__(self, config: Config):
+        self.config = config
     
-if __name__ == "__main__":
-    validate_provider_config()
+    def register_providers(self, container: Container) -> None:
+        # for more complicated provider registrations
+        # container.register_instance(...)
+        pass
 ```
-In above example, we used `ProviderConfig` as a value type as in the case of `IFooB` type and 
-as a concrete type as in the case of `IFoo` type.
 
-### **`register_providers`**:
-We can also achieve the same by overriding `register_providers` in any Module class.
+## **Module Middleware**
+
+Middlewares functions can be defined at Module level with `@middleware()` function decorator.
 
 For example:
+
 ```python
-# main.py
+from ellar.common import Module, middleware, IHostContext, PlainTextResponse
+from ellar.core import ModuleBase
 
-from ellar.common import Module
-from ellar.core import ModuleBase, Config
-from ellar.di import Container, EllarInjector, injectable
-from ellar.core.modules.ref import create_module_ref_factor
 
-injector = EllarInjector(auto_bind=False)
+@Module()
+class ModuleMiddlewareSample(ModuleBase):
+    @middleware()
+    async def my_middleware_function_1(cls, context: IHostContext, call_next):
+        request = context.switch_to_http_connection().get_request() # for http response only
+        request.state.my_middleware_function_1 = True
+        await call_next()
+    
+    @middleware()
+    async def my_middleware_function_2(cls, context: IHostContext, call_next):
+        if context.get_type() == 'websocket':
+            websocket = context.switch_to_websocket().get_client()
+            websocket.state.my_middleware_function_2 = True
+        await call_next()
+
+    @middleware()
+    async def my_middleware_function_3(cls, context: IHostContext, call_next):
+        connection = context.switch_to_http_connection().get_client() # for http response only
+        if connection.headers['somekey']:
+            # response = context.get_response() -> use the `response` to add extra definitions to things you want to see on
+            return PlainTextResponse('Header is not allowed.')
+        await call_next()
+```
+Things to note:
+
+- middleware functions must be `async`.
+- middleware functions can return a `response` or modify a `response` returned
+- middleware functions must call `call_next` and `await` its actions as shown above.
 
+## **Injector Module**
+`EllarInjector` is based on a python library [injector](https://injector.readthedocs.io/en/latest/index.html). Both share similar `Module` features with few distinct features. 
 
-class IFoo:
-    pass
+As an added support, you can create or reuse modules from `injector` Modules.
 
+!!! info
+    This type of module is used to configure `injector` **bindings** and **providers** for dependency injection purposes.
 
-class IFooB:
-    pass
+```python
+from ellar.core import ModuleBase
+from ellar.di import Container
+from injector import provider
 
 
-@injectable  # default scope=singleton_scope
-class AFooClass(IFoo, IFooB):
+class Name(str):
     pass
 
 
-a_foo_instance = AFooClass()
+class Description(str):
+    pass
 
 
-@Module()
-class AModule(ModuleBase):
+class ExampleModule(ModuleBase):
     def register_services(self, container: Container) -> None:
-        container.register_singleton(IFoo, AFooClass)
-        container.register(IFooB, a_foo_instance)
+        container.bind(Name, to='Sherlock')
 
+    @provider
+    def describe(self, name: Name) -> Description:
+        return Description('%s is a man of astounding insight' % name)
 
-def validate_register_services():
-    module_ref = create_module_ref_factor(
-    AModule, container=injector.container, config=Config(),
-    )
-    module_ref.run_module_register_services()
-    
-    ifoo_b = injector.get(IFooB)
-    ifoo = injector.get(IFoo)
-    
-    assert isinstance(ifoo_b, AFooClass)
-    assert isinstance(ifoo, AFooClass)
-    assert ifoo_b == a_foo_instance
+```
+The `ExampleModule` has registered `Description` and `Name` type to the injector and can be resolved respectively if required by any object.
 
-if __name__ == "__main__":
-    validate_register_services()
+Read more on injector module use cases - [Here](https://injector.readthedocs.io/en/latest/terminology.html#module).
 
-```
+## **Module and Application Lifespan**
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ellar-0.4.0/docs/parsing-inputs/body.md` & `ellar-0.4.2/docs/techniques/validations/body.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-# Request Body
+# **Request Body**
 
 Request bodies are typically used with “create” and “update” operations (POST, PUT, PATCH).
 For example, when creating a resource using POST or PUT, the request body usually contains the representation of the resource to be created.
 
 To declare a **request body**, you need to use **Ellar `Serializer`**.
 
 !!! info
     Under the hood **Ellar** uses <a href="https://pydantic-docs.helpmanual.io/" class="external-link" target="_blank">Pydantic</a> models with all their power and benefits.
 
-## Import Serializer
+## **Import Serializer**
 
 First, you need to import `Serializer` from `ella.serializer`:
 
 ```python
 # project_name/apps/items/controllers.py
 from ellar.common import Serializer
 
@@ -20,15 +20,15 @@
 #     name: str
 #     description: str = None
 #     price: float
 #     quantity: int
 
 ```
 
-## Create your data model
+## **Create your data model**
 
 Then you declare your data model as a class that inherits from `Serializer`.
 
 Use standard Python types for all the attributes:
 
 ```python
 # project_name/apps/items/controllers.py
@@ -67,15 +67,15 @@
 {
     "name": "Alexis",
     "price": 200.00,
     "quantity": 12
 }
 ```
 
-## Declare it as a parameter
+## **Declare it as a parameter**
 
 To add it to your *path operation*, declare it the same way you declared the path and query parameters:
 
 ```python
 # project_name/apps/items/controllers.py
 
 from ellar.common import Serializer, Controller, post, ControllerBase
@@ -93,41 +93,41 @@
     @post("/")
     def create(self, item: Item):
         return item
 ```
 
 ... and declare its type as the model you created, `Item`.
 
-## Results
+## **Results**
 
 With just that Python type declaration, **Ellar** will:
 
 * Read the body of the request as JSON.
 * Convert the corresponding types (if needed).
 * Validate the data.
     * If the data is invalid, it will return a nice and meaningful error, indicating exactly where and what the incorrect data was.
 * Give you the received data in the parameter `item`.
     * Because you declared it in the function to be of type `Item`, you will also have all the editor support
       (completion, etc.) for all the attributes and their types.
 * Generate <a href="https://json-schema.org" class="external-link" target="_blank">JSON Schema</a> definitions for
   your models, and you can also use them anywhere else you like if it makes sense for your project.
 * Those schemas will be part of the generated OpenAPI schema, and used by the automatic documentation <abbr title="User Interfaces">UI's</abbr>.
 
-## Automatic Docs
+## **Automatic Docs**
 
 The JSON Schemas of your models will be part of your OpenAPI generated schema, and will be shown in the interactive API docs:
 
 ![Openapi schema](../img/body-schema-doc.png)
 
 ... and they will be also used in the API docs inside each *path operation* that needs them:
 
 ![Openapi schema](../img/body-schema-doc2.png)
 
 
-## Request Body + Path parameters
+## **Request Body + Path parameters**
 
 You can declare path parameters **and** body requests at the same time.
 
 **Ellar** will recognize that the function parameters that match path parameters should be **taken from the path**, and that function parameters that are declared with `Serializer` should be **taken from the request body**.
 
 ```python
 # project_name/apps/items/controllers.py
@@ -148,15 +148,15 @@
         return item
     
     @put("/items/{item_id}")
     def update(self, item_id: int, item: Item):
         return {"item_id": item_id, "item": item.dict()}
 ```
 
-## Request Body + Path + Query parameters
+## **Request Body + Path + Query parameters**
 
 You can also declare **body**, **path** and **query** parameters, all at the same time.
 
 **Ellar** will recognize each of them and take the data from the correct place.
 
 ```python
 # project_name/apps/items/controllers.py
@@ -187,15 +187,15 @@
 * If the parameter is of a **singular type** (like `int`, `float`, `str`, `bool`, etc.), it will be interpreted as a **query** parameter.
 * If the parameter is declared to be of the type of **Serializer** (or Pydantic `BaseModel`), it will be interpreted as a request **body**.
 
 !!! info
     In here, we have combined both `Serializers` and `Controllers` in one file. This is for the convenience of writing this documentation.
     It's advised to have all your serializers in `schemas.py` and then import them over to `controllers.py` if needed.
 
-## Singular values in body
+## **Singular values in body**
 The same way there is a `Query` and `Path` to define extra data for query and path parameters, 
 **Ellar** provides an equivalent `Body`.
 
 For example, extending the previous model, you could decide that you want to have another key `importance` in the same body, besides the `item` and `user`.
 
 If you declare it as is, because it is a singular value, **Ellar** will assume that it is a query parameter.
 
@@ -249,15 +249,15 @@
         "username": "dave",
         "full_name": "Dave Grohl"
     },
     "importance": 5
 }
 ```
 
-## Multiple body params and query
+## **Multiple body params and query**
 Of course, you can also declare additional `query` parameters whenever you need, additional to anybody parameters.
 
 As, by default, singular values are interpreted as query parameters, you don't have to explicitly add a `Query`, you can just do:
 
 For example:
 
 ```python
```

### Comparing `ellar-0.4.0/docs/parsing-inputs/cookie-params.md` & `ellar-0.4.2/docs/techniques/validations/cookie-params.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-# Cookie Parameters
+# **Cookie Parameters**
 
 You can define Cookie parameters the same way you define `Path` parameters.
 
-## Import `Cookie`
+## **Import `Cookie`**
 
 First import `Cookie` from `ellar.common` module
 
-## Declare `Cookie` parameters
+## **Declare `Cookie` parameters**
 
 Then declare the cookie parameters using the same structure as with `Path` and `Query`.
 
 The first value is the default value, you can pass all the extra validation or annotation parameters:
 
 ```python
 # project_name/apps/items/controllers.py
@@ -25,15 +25,15 @@
     async def read_items(self, ads_id: Optional[str] = Cookie(default=None)):
         return {"ads_id": ads_id}
 ```
 
 !!! info
     To declare cookies, you need to use `Cookie`, because otherwise the parameters would be interpreted as `query` parameters.
 
-### Using Schema
+## **Using Schema**
 
 You can also use Schema to encapsulate `Cookies` parameters:
 
 ```python
 # project_name/apps/items/controllers.py
 
 from ellar.common import Serializer, get, Controller, Cookie, ControllerBase
```

### Comparing `ellar-0.4.0/docs/parsing-inputs/file-params.md` & `ellar-0.4.2/docs/techniques/validations/file-params.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-# File uploads
+# **File Uploads**
 
 Handling files are no different from other parameters.
 You can define files to be uploaded by using `File`.
 
 !!! info
     To receive uploaded files, first install <a href="https://andrew-d.github.io/python-multipart/" class="external-link" target="_blank">`python-multipart`</a>.
 
     E.g. `pip install python-multipart`.
 
     This is because uploaded files are sent as "form data".
 
-## Import `File`
+## **Import `File`**
 
 First import `File` from `ellar.common` module
 
-## Define `File` parameters
+## **Define `File` parameters**
 
 Create file parameters the same way you would for `Body` or `Form`:
 
 ```python
 # project_name/apps/items/controllers.py
 from ellar.common import File, Controller, post, ControllerBase
 
@@ -34,15 +34,15 @@
 
 If you declare the type of your *path operation function* parameter as `bytes`, **Ellar** will read the file for you and you will receive the contents as `bytes`.
 
 Have in mind that this means that the whole contents will be stored in memory. This will work well for small files.
 
 But there are several cases in which you might benefit from using `UploadFile`.
 
-## `File` parameters with `UploadFile`
+## **`File` parameters with `UploadFile`**
 
 Define a `File` parameter with a type of `UploadFile`:
 
 ```python
 # project_name/apps/items/controllers.py
 from ellar.common import File, UploadFile, Controller, post, ControllerBase
 
@@ -102,15 +102,15 @@
 !!! note "`async` Technical Details"
     When you use the `async` methods, **Ellar** runs the file methods in a threadpool and awaits for them.
 
 !!! note "Starlette Technical Details"
     **Ellar**'s `UploadFile` inherits directly from **Starlette**'s `UploadFile`, but adds some necessary parts to make it compatible with **Pydantic** and the other parts of Ellar.
 
 
-## Uploading array of files
+## **Uploading array of files**
 
 To **upload several files** at the same time, just declare a `List` of `UploadFile`:
 
 
 ```python
 # project_name/apps/items/controllers.py
 from typing import List
@@ -120,15 +120,15 @@
 @Controller
 class ItemsController(ControllerBase):
     @post("/upload-many")
     def upload_many(self, files: List[UploadFile] = File()):
         return [f.filename for f in files]
 ```
 
-## Uploading files with extra fields
+## **Uploading files with extra fields**
 
 Note: HTTP protocol does not allow you to send files in application/json format by default (unless you encode it somehow to JSON on client side)
 
 To send files along with some extra attributes you need to send bodies in multipart/form-data encoding. You can do it by simply marking fields with `Form`:
 
 ```python
 # project_name/apps/items/controllers.py
```

### Comparing `ellar-0.4.0/docs/parsing-inputs/form-params.md` & `ellar-0.4.2/docs/techniques/validations/form-params.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-# Form data
+# **Form Data**
 
 **Ellar** also allows you to parse and validate `request.POST` data
 (aka `application x-www-form-urlencoded` or `multipart/form-data`).
 When you need to receive form fields instead of JSON, you can use `Form`.
 
 !!! info
     To use forms, first install [python-multipart](https://andrew-d.github.io/python-multipart/).
 
     E.g. `pip install python-multipart`.
 
 
-## Form Data as params 
+## **Form Data as params** 
 
 ```python
 # project_name/apps/items/controllers.py
 
 from ellar.common import Controller, Form, post, ControllerBase
 
 
@@ -35,15 +35,15 @@
 2) Use `Form` as default value for your parameter:
 ```python
 from ellar.common import Form
 
 username: str = Form()
 ```
 
-## Using a Schema
+## **Using a Schema**
 
 In a similar manner to [Body](../body/#declare-it-as-a-parameter), you can use
 a Schema to organize your parameters.
 
 ```python
 # project_name/apps/items/controllers.py
 
@@ -62,15 +62,15 @@
     @post("/")
     def create(self, item: Item = Form()):
         return item
 ```
 
 ![Openapi schema](../img/form-schema-doc.png)
 
-## Request form + path + query parameters
+## **Request form + path + query parameters**
 
 In a similar manner to [Body](../body/#request-body-path-query-parameters), you can use
 Form data in combination with other parameter sources.
 
 You can declare query **and** path **and** form field, **and** etc... parameters at the same time.
 
 **Ellar** will recognize that the function parameters that match path
@@ -97,15 +97,15 @@
         return item
     
     @put("/{item_id}")
     def update(self, item_id: int, q: str, item: Item=Form()):
         return {"item_id": item_id, "item": item.dict(), "q": q}
 ```
 
-## Mapping Empty Form Field to Default
+## **Mapping Empty Form Field to Default**
 
 Form fields that are optional, are often sent with an empty value. This value is
 interpreted as an empty string, and thus may fail validation for fields such as `int` or `bool`.
 
 This can be fixed, as described in the Pydantic docs, by using
 [Generic Classes as Types](https://pydantic-docs.helpmanual.io/usage/types/#generic-classes-as-types).
```

### Comparing `ellar-0.4.0/docs/parsing-inputs/header-params.md` & `ellar-0.4.2/docs/techniques/validations/header-params.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-# Header Parameters
+# **Header Parameters**
 
 You can define Header parameters the same way you define `Query`, `Path` and `Cookie` parameters.
 
 To query this operation, you use a URL like:
 
-## Import `Header`
+## **Import `Header`**
 
 First import `Header` from `ellar.common` module
 
-## Declare `Header` parameters
+## **Declare `Header` parameters**
 
 Then declare the header parameters using the same structure as with `Path`, `Query` and `Cookie`.
 
 The first value is the default value, you can pass all the extra validation or annotation parameters:
 
 ```python
 # project_name/apps/items/controllers.py
@@ -27,15 +27,15 @@
     async def read_items(self, user_agent: Optional[str] = Header(default=None)):
         return {"User-Agent": user_agent}
 ```
 
 !!! info
     To declare headers, you need to use `Header`, because otherwise the parameters would be interpreted as query parameters.
 
-## Automatic conversion
+## **Automatic conversion**
 
 `Header` has a little extra functionality.
 
 Most of the standard headers are separated by a "hyphen" character, also known as the "minus symbol" (`-`).
 
 But a variable like `user-agent` is not valid in Python.
 
@@ -63,15 +63,15 @@
         return {"strange_header": strange_header}
 ```
 
 !!! warning
     Before setting `convert_underscores` to `False`, bear in mind that some HTTP proxies and servers disallow the usage of headers with underscores.
 
 
-## Duplicate headers
+## **Duplicate headers**
 
 It is possible to receive duplicate headers. That means, the same header with multiple values.
 
 You can define those cases using a list in the type declaration.
 
 You will receive all the values from the duplicate header as a Python `list`.
 
@@ -105,15 +105,15 @@
     "X-Token values": [
         "bar",
         "foo"
     ]
 }
 ```
 
-### Using Schema
+## **Using Schema**
 
 You can also use Schema to encapsulate `Header` parameters:
 
 ```python
 # project_name/apps/items/controllers.py
 
 from typing import List
```

### Comparing `ellar-0.4.0/docs/parsing-inputs/index.md` & `ellar-0.4.2/docs/techniques/validations/index.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Intro
+# **Input Validation Tutorial**
 
 In this section, we are going to learn how inputs are parsed in the Ellar route handle functions.
 
 To get started, we need to create another module for this tutorial.
 
 Open the terminal, navigate to the root level of the project and run the command that scaffolds a new module to your project.
 
@@ -40,15 +40,15 @@
   "detail": "Welcome Items Resource"
 }
 ```
 
 All code example will be done on the `ItemController` in `project_name/apps/items/controllers.py`. 
 Please keep it open.
 
-## Tutorial
+## **Tutorial**
 You are going to learn how to use the following route handler parameter:
 
 - [Path](./path-params)
 - [Query](./query-params/)
 - [Header](./header-params/)
 - [Cookie](./cookie-params/)
 - [Body](./body/)
```

### Comparing `ellar-0.4.0/docs/parsing-inputs/path-params.md` & `ellar-0.4.2/docs/techniques/validations/path-params.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Path parameters
+# **Path Parameters**
 You can declare path "parameters" with the same syntax used by Python format-strings 
 which is similar to [OpenAPI path parameters](https://swagger.io/docs/specification/describing-parameters/#path-parameters)
 
 
 ```python
 # project_name/apps/items/controllers.py
 
@@ -22,15 +22,15 @@
 
 ```JSON
 {
   "item_id":"foo"
 }
 ```
 
-### Path parameters with types
+## **Path parameters with types**
 You can declare the type of path parameter in the function using standard Python type annotations:
 
 ```python
 # project_name/apps/items/controllers.py
 
 from ellar.common import get, Controller, ControllerBase
 
@@ -52,15 +52,15 @@
 ```
 
 !!! tip
     Notice that the value your function received (and returned) is **3**, as a Python `int` - not a string `"3"`.
     So, with just that type declaration, **Ellar** gives you automatic request "parsing" and validation.
 
 
-### Data validation
+## **Data validation**
 On the other hand, if you go to the browser at [http://localhost:8000/items/foo](http://localhost:8000/items/foo), you will see an HTTP error like this:
 
 ```JSON
 {
     "detail": [
         {
             "loc": [
@@ -74,15 +74,15 @@
 }
 ```
 that is because the path parameter `item_id` had a value of `"foo"`, which is not an `int`.
 
 The same error would appear if you provided a `float` instead of an `int`, as in:
 [http://localhost:8000/items/4.2](http://localhost:8000/items/4.2)
 
-### Path Converters
+## **Path Converters**
 
 You can use [Starlette Path Converters](https://www.starlette.io/routing/#path-parameters) to help parse the path:
 
 ```python
 # project_name/apps/items/controllers.py
 
 from ellar.common import get, Controller, ControllerBase
@@ -106,15 +106,15 @@
     ```python
     ...
     @get("/items/{int:item_id}")
     def read_item(self, item_id:int):
         return {"item_id": item_id}
     ```
  
-#### Path params with slashes
+### Path params with slashes
 
 Starlette `path` converter allows you to handle path-like parameters:
 
 For example, lets another route handler `some_view` and give it a path `/dir/{value:path}`.
 What this means is that the parameter is `value`, and the last part, `:path`, tells it that the parameter should match any path.
 
 ```python
@@ -128,15 +128,15 @@
     @get('/dir/{value:path}')
     def some_view(self, value: str):
         return value
 ```
 You can query this operation with [http://localhost:8000/items/dir/some/path/with-slashes](http://localhost:8000/items/dir/some/path/with-slashes) 
 and your `value` will be equal to `"some/path/with-slashes"`
 
-### Multiple parameters
+## **Multiple parameters**
 
 You can pass as many variables as you want into `path`, just remember to have unique names and don't forget to use the same names in the function arguments.
 
 ```Python
 # project_name/apps/items/controllers.py
 
 from ellar.common import get, Controller, ControllerBase
@@ -146,15 +146,15 @@
 class ItemsController(ControllerBase):
     @get("/events/{year}/{month}/{day}")
     def events(self, year: int, month: int, day: int):
         return {"date": [year, month, day]}
 ```
 
 
-### Using Schema
+## **Using Schema**
 
 You can also use Schema to encapsulate path parameters that depend on each other (and validate them as a group):
 
 ```python
 # project_name/apps/items/controllers.py
 
 import datetime
@@ -176,19 +176,19 @@
     def events(self, date: PathDate = Path()):
         return {"date": date.value()}
 ```
 
 !!! note
     Notice that here we used a `Path` source hint to let **Ellar** know that this schema will be applied to path parameters.
 
-### Documentation
+## **Documentation**
 Now, when you open your browser at [http://localhost:8000/docs](http://localhost:8000/docs), you will see the automatic, interactive, API documentation.
 ![events Swagger doc](../img/event_docs_swagger.png)
 
-### Using Enum
+## **Using Enum**
 
 If you have a path operation that receives a path parameter, 
 but you want the possible valid path parameter values to be predefined, you can use a standard Python `Enum`.
 
 For an example:
 
 ```python
@@ -212,11 +212,11 @@
     
         if model_name.value == "lenet":
             return {"model_name": model_name, "message": "LeCNN all the images"}
     
         return {"model_name": model_name, "message": "Have some residuals"}
 ```
 
-#### Check the docs
+### Check the docs
 Because the available values for the path parameter are predefined, the interactive docs can show them nicely:
 
 ![enum Swagger doc](../img/enum_docs_swagger.png)
```

### Comparing `ellar-0.4.0/docs/parsing-inputs/query-params.md` & `ellar-0.4.2/docs/techniques/validations/query-params.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Query parameters
+# **Query Parameters**
 
 When you declare other function parameters that are not part of the path parameters, they are automatically interpreted as "query" parameters.
 
 ```python
 # project_name/apps/items/controllers.py
 
 from ellar.common import get, Controller, ControllerBase
@@ -47,15 +47,15 @@
     @get('/weapons')
     def list_weapons(self, limit, offset):
         assert type(limit) == str
         assert type(offset) == str
         return fake_items_db[offset: int(offset) + int(limit)]
 ```
 
-### Defaults
+## **Defaults**
 
 As query parameters are not a fixed part of a path, they are optional and can have default values:
 
 ```python
 # project_name/apps/items/controllers.py
 
 from ellar.common import get, Controller, ControllerBase
@@ -87,15 +87,15 @@
 
 the parameter values in your function will be:
 
  - `offset=20`  (because you set it in the URL)
  - `limit=10`  (because that was the default value)
 
 
-### Required and optional parameters
+## **Required and optional parameters**
 
 You can declare required or optional GET parameters in the same way as declaring Python function arguments:
 
 ```python
 # project_name/apps/items/controllers.py
 
 from ellar.common import get, Controller, ControllerBase
@@ -110,15 +110,15 @@
         results = [w for w in weapons if q in w.lower()]
         print(q, results)
         return results[offset: offset + 10]
 ```
 
 In this case, **Ellar** will always validate that you pass the `q` param in the GET, and the `offset` param is an optional integer.
 
-### GET parameters type conversion
+## **GET parameters type conversion**
 
 Let's declare multiple type arguments:
 ```python
 # project_name/apps/items/controllers.py
 
 from ellar.common import get, Controller, ControllerBase
 from datetime import date
@@ -147,15 +147,15 @@
 ```
 http://localhost:8000/items/example?d=1672286800
 # same as 2022-12-29
 
 http://localhost:8000/items/example?d=2022-12-29
 ```
 
-### Using Schema
+## **Using Schema**
 
 You can also use Schema to encapsulate GET parameters:
 
 ```python
 # project_name/apps/items/controllers.py
 
 from typing import List
```

### Comparing `ellar-0.4.0/docs/templating/staticfiles.md` & `ellar-0.4.2/docs/techniques/staticfiles.md`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/docs/templating/templating.md` & `ellar-0.4.2/docs/techniques/templating.md`

 * *Files 2% similar despite different names*

```diff
@@ -168,19 +168,19 @@
 if __name__ == "__main__":
     uvicorn.run("main:app", port=5000, log_level="info")
 ```
 
 !!! info
     `Jinja2` supports async template rendering, however as a general rule we'd recommend that you keep your templates free from logic that invokes database lookups, or other I/O operations.
     Instead, we'd recommend that you ensure that your endpoints perform all I/O, for example, strictly evaluate any database queries within the view and include the final results in the context.'
-    - [`Starlette Recommendation`](https://www.starlette.io/templates/#asynchronous-template-rendering)
+    - [`Starlette Recommendation`](https://www.starlette.io/templates/#asynchronous-template-rendering){target="_blank"}
 
 
 ## **Jinja2 Configurations**
-If there are specific configurations you want to apply to your Jinja2 Environment, you can look at [JINJA_TEMPLATE_OPTIONS](https://eadwincode.github.io/ellar/configurations/#jinja_templates_options) configuration.
+If there are specific configurations you want to apply to your Jinja2 Environment, you can look at [JINJA_TEMPLATE_OPTIONS](../../techniques/configurations/#jinja_templates_options){target="_blank"} configuration.
 
 ## **Default Jinja Template Context**
 
 Every jinja template in ellar receives two context, `url_for`, `config`, `request` object and other specific context defined to render a template.
 
 - `url_for` is a utility function that helps to resolve path to files and url(reversing url)
 - `config` is current application configuration object.
@@ -201,15 +201,15 @@
 </head>
 ```
 
 The `url_for` takes `path` parameter, in the case of `static` files, to match the **directory** and **filename** to be resolved.
 This `url_for('static', path='img/Icon.svg')` will search for `img/Icon.svg` in all registered static folders.
 
 
-### Reversing Controllers URLs
+### **Reversing Controllers URLs**
 It is common to need to generate URLs for specific routes, particularly when returning a redirect response. 
 This can be achieved by using the `request.url_for` method in the request object, or in the case of templating, by using the `url_for()` function.
 
 The `request.url_for` method generates a URL based on the current request context, while in template `{{url_for()}}` function generates a URL based on the current routing configuration.
 Both of them will generate a URL for a specific route, allowing the server to redirect the client to the correct location.
 
 In controllers, urls are reversed by joining the **controller_name** and **route handler** name like so `controller_name:function_name`.
@@ -281,15 +281,15 @@
 In the example `request.url_for('templateexample:index', parameter_a='ellar')`, 
 we can see that the `parameter_a` is used as a keyword argument to satisfy the dependency on the `parameter_a` parameter in the URL being generated.
 
 !!! info
     If the `url_for` function is called with a path that does not exist or with insufficient parameters to resolve an existing URL, 
     it will raise a `starlette.routing.NoMatchFound` exception.
 
-### Reversing Module Router URLs
+### **Reversing Module Router URLs**
 
 Just like in controller, we can also reverse URLs that belongs to `ModuleRouter`. 
 
 ```python
 # main.py
 import uvicorn
 from ellar.common import ModuleRouter, Req
@@ -334,15 +334,15 @@
     profile_url = request.url_for('profile', user_id=user_id)
     return profile_url
 ```
 
 It's worth noting that providing a unique name to a router is useful if you have multiple routes with the same function name, or to make the URL reversing more readable or meaningful.
 
 
-### Overriding Reversing URL Function Name
+### **Overriding Reversing URL Function Name**
 You can override the `function_name` part of reversing the URL by providing a `name` on the **route method** decorator.
 Each route method has an optional name parameter, which, when set, is used in place of the function name when reversing the URL.
 For example, you could have the following code:
 
 ```python
 router = ModuleRouter('/template-reversing', name='users')
 
@@ -354,9 +354,9 @@
 
 In this case, when reversing the URL, you would use `request.url_for('users:user_profile', user_id=user_id)`
 which will generate `http://127.0.0.1:5000/template-reversing/profile/value_of_user_id` based on routing configuration.
 
 This allows for greater control and readability when reversing URLs, and makes it less prone to error if the function name of the route were to change in the future.
 
 
-### Adding template filters and template globals.
-Jinja template filter and global functions can be defined at module level as shown here: [Module Templating Filters](/ellar/overview/modules/#module-templating-filters)
+### **Adding template filters and template globals.**
+Jinja template filter and global functions can be defined at module level as shown here: [Module Templating Filters](../../overview/modules/#module-templating-filters){target="_blank"}
```

### Comparing `ellar-0.4.0/docs/throttling.md` & `ellar-0.4.2/docs/security/throttling.md`

 * *Files 1% similar despite different names*

```diff
@@ -171,15 +171,15 @@
 ])
 class ApplicationModule:
     pass
 ```
 
 ### **Proxies**
 If you are working with multiple proxies, you can override the `get_tracker()` method to pull the value from the header or install 
-[`ProxyHeadersMiddleware`](https://github.com/encode/uvicorn/blob/master/uvicorn/middleware/proxy_headers.py)
+[`ProxyHeadersMiddleware`](https://github.com/encode/uvicorn/blob/master/uvicorn/middleware/proxy_headers.py){target="_blank"}
 
 ```python
 # throttler_behind_proxy.guard.py
 from ellar_throttler import ThrottlerGuard
 from ellar.di import injectable
 from ellar.core.connection import HTTPConnection
```

### Comparing `ellar-0.4.0/docs/websockets/index.md` & `ellar-0.4.2/docs/websockets/index.md`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/docs/websockets/socketio.md` & `ellar-0.4.2/docs/websockets/socketio.md`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/cache/backends/_aio_cache.py.ellar` & `ellar-0.4.2/ellar/cache/backends/_aio_cache.py.ellar`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/cache/backends/base.py` & `ellar-0.4.2/ellar/cache/backends/base.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/cache/backends/local_cache.py` & `ellar-0.4.2/ellar/cache/backends/local_cache.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/cache/backends/pylib_cache.py` & `ellar-0.4.2/ellar/cache/backends/pylib_cache.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/cache/backends/pymem_cache.py` & `ellar-0.4.2/ellar/cache/backends/pymem_cache.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/cache/backends/redis/backend.py` & `ellar-0.4.2/ellar/cache/backends/redis/backend.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/cache/backends/serializer.py` & `ellar-0.4.2/ellar/cache/backends/serializer.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/cache/decorator.py` & `ellar-0.4.2/ellar/cache/decorator.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/cache/interface.py` & `ellar-0.4.2/ellar/cache/interface.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/cache/make_key_decorator.py` & `ellar-0.4.2/ellar/cache/make_key_decorator.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/cache/model.py` & `ellar-0.4.2/ellar/cache/model.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/cache/module.py` & `ellar-0.4.2/ellar/cache/module.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/cache/schema.py` & `ellar-0.4.2/ellar/cache/schema.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/cache/service.py` & `ellar-0.4.2/ellar/cache/service.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/common/__init__.py` & `ellar-0.4.2/ellar/common/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,14 +29,16 @@
     NotAcceptable,
     NotAuthenticated,
     NotFound,
     PermissionDenied,
     UnsupportedMediaType,
 )
 from .interfaces import (
+    IApplicationShutdown,
+    IApplicationStartup,
     IExceptionHandler,
     IExceptionMiddlewareService,
     IExecutionContext,
     IExecutionContextFactory,
     IGuardsConsumer,
     IHostContext,
     IHostContextFactory,
@@ -195,12 +197,14 @@
     "IModuleSetup",
     "IResponseModel",
     "IModuleTemplateLoader",
     "IInterceptorsConsumer",
     "IGuardsConsumer",
     "EllarInterceptor",
     "UseInterceptors",
+    "IApplicationStartup",
+    "IApplicationShutdown",
 ]
 
 
 def __dir__() -> t.List[str]:
     return sorted(__all__)  # pragma: no cover
```

### Comparing `ellar-0.4.0/ellar/common/commands/base.py` & `ellar-0.4.2/ellar/common/commands/base.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/common/commands/decorator.py` & `ellar-0.4.2/ellar/common/commands/decorator.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/common/compatible/cache_properties.py` & `ellar-0.4.2/ellar/common/compatible/cache_properties.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/common/compatible/dict.py` & `ellar-0.4.2/ellar/common/compatible/dict.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/common/compatible/emails.py` & `ellar-0.4.2/ellar/common/compatible/emails.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/common/constants.py` & `ellar-0.4.2/ellar/common/constants.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/common/converters.py` & `ellar-0.4.2/ellar/common/converters.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/common/datastructures.py` & `ellar-0.4.2/ellar/common/datastructures.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/common/decorators/__init__.py` & `ellar-0.4.2/ellar/common/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/common/decorators/controller.py` & `ellar-0.4.2/ellar/common/decorators/controller.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/common/decorators/exception.py` & `ellar-0.4.2/ellar/common/decorators/exception.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/common/decorators/extra_args.py` & `ellar-0.4.2/ellar/common/decorators/extra_args.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/common/decorators/file.py` & `ellar-0.4.2/ellar/common/decorators/file.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/common/decorators/guards.py` & `ellar-0.4.2/ellar/common/decorators/guards.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/common/decorators/html.py` & `ellar-0.4.2/ellar/common/decorators/html.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/common/decorators/interceptor.py` & `ellar-0.4.2/ellar/common/decorators/interceptor.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/common/decorators/middleware.py` & `ellar-0.4.2/ellar/common/decorators/middleware.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/common/decorators/modules.py` & `ellar-0.4.2/ellar/common/decorators/modules.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/common/decorators/openapi.py` & `ellar-0.4.2/ellar/common/decorators/openapi.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/common/decorators/serializer.py` & `ellar-0.4.2/ellar/common/decorators/serializer.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/common/exceptions/__init__.py` & `ellar-0.4.2/ellar/common/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/common/exceptions/api/base.py` & `ellar-0.4.2/ellar/common/exceptions/api/base.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/common/exceptions/api/exceptions_types.py` & `ellar-0.4.2/ellar/common/exceptions/api/exceptions_types.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/common/exceptions/callable_exceptions.py` & `ellar-0.4.2/ellar/common/exceptions/callable_exceptions.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/common/exceptions/handlers.py` & `ellar-0.4.2/ellar/common/exceptions/handlers.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/common/exceptions/validation.py` & `ellar-0.4.2/ellar/common/exceptions/validation.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/common/helper/__init__.py` & `ellar-0.4.2/ellar/common/helper/__init__.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/common/helper/enums.py` & `ellar-0.4.2/ellar/common/helper/enums.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/common/helper/importer.py` & `ellar-0.4.2/ellar/common/helper/importer.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/common/helper/modelfield.py` & `ellar-0.4.2/ellar/common/helper/modelfield.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/common/helper/module_loading.py` & `ellar-0.4.2/ellar/common/helper/module_loading.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/common/interfaces/__init__.py` & `ellar-0.4.2/ellar/common/interfaces/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from .application import IApplicationShutdown, IApplicationStartup
 from .context import (
     IExecutionContext,
     IExecutionContextFactory,
     IHostContext,
     IHostContextFactory,
     IHTTPConnectionContextFactory,
     IHTTPHostContext,
@@ -27,8 +28,10 @@
     "IExceptionMiddlewareService",
     "IExceptionHandler",
     "IModuleSetup",
     "IResponseModel",
     "IModuleTemplateLoader",
     "IInterceptorsConsumer",
     "IGuardsConsumer",
+    "IApplicationShutdown",
+    "IApplicationStartup",
 ]
```

### Comparing `ellar-0.4.0/ellar/common/interfaces/context.py` & `ellar-0.4.2/ellar/common/interfaces/context.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/common/interfaces/exceptions.py` & `ellar-0.4.2/ellar/common/interfaces/exceptions.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/common/interfaces/module.py` & `ellar-0.4.2/ellar/common/interfaces/module.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/common/interfaces/response_model.py` & `ellar-0.4.2/ellar/common/interfaces/response_model.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/common/interfaces/templating.py` & `ellar-0.4.2/ellar/common/interfaces/templating.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/common/models/controller.py` & `ellar-0.4.2/ellar/common/models/controller.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/common/models/guard.py` & `ellar-0.4.2/ellar/common/models/guard.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/common/params/args/base.py` & `ellar-0.4.2/ellar/common/params/args/base.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/common/params/args/extra_args.py` & `ellar-0.4.2/ellar/common/params/args/extra_args.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/common/params/args/factory.py` & `ellar-0.4.2/ellar/common/params/args/factory.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/common/params/args/request_model.py` & `ellar-0.4.2/ellar/common/params/args/request_model.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/common/params/args/resolver_generators.py` & `ellar-0.4.2/ellar/common/params/args/resolver_generators.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/common/params/args/websocket_model.py` & `ellar-0.4.2/ellar/common/params/args/websocket_model.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/common/params/decorators.py` & `ellar-0.4.2/ellar/common/params/decorators.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/common/params/helpers.py` & `ellar-0.4.2/ellar/common/params/helpers.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/common/params/params.py` & `ellar-0.4.2/ellar/common/params/params.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/common/params/resolvers/__init__.py` & `ellar-0.4.2/ellar/common/params/resolvers/__init__.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/common/params/resolvers/base.py` & `ellar-0.4.2/ellar/common/params/resolvers/base.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/common/params/resolvers/bulk_parameter.py` & `ellar-0.4.2/ellar/common/params/resolvers/bulk_parameter.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/common/params/resolvers/non_parameter/__init__.py` & `ellar-0.4.2/ellar/common/params/resolvers/non_parameter/__init__.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/common/params/resolvers/non_parameter/background.py` & `ellar-0.4.2/ellar/common/params/resolvers/non_parameter/background.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/common/params/resolvers/non_parameter/base.py` & `ellar-0.4.2/ellar/common/params/resolvers/non_parameter/base.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/common/params/resolvers/non_parameter/inject.py` & `ellar-0.4.2/ellar/common/params/resolvers/non_parameter/inject.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/common/params/resolvers/non_parameter/session.py` & `ellar-0.4.2/ellar/common/params/resolvers/non_parameter/session.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/common/params/resolvers/parameter.py` & `ellar-0.4.2/ellar/common/params/resolvers/parameter.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/common/responses/models/__init__.py` & `ellar-0.4.2/ellar/common/responses/models/__init__.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/common/responses/models/base.py` & `ellar-0.4.2/ellar/common/responses/models/base.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/common/responses/models/file.py` & `ellar-0.4.2/ellar/common/responses/models/file.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/common/responses/models/helper.py` & `ellar-0.4.2/ellar/common/responses/models/helper.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/common/responses/models/html.py` & `ellar-0.4.2/ellar/common/responses/models/html.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/common/responses/models/json.py` & `ellar-0.4.2/ellar/common/responses/models/json.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/common/responses/models/route.py` & `ellar-0.4.2/ellar/common/responses/models/route.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/common/responses/models/type_converter.py` & `ellar-0.4.2/ellar/common/responses/models/type_converter.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/common/responses/response_types.py` & `ellar-0.4.2/ellar/common/responses/response_types.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/common/routing/__init__.py` & `ellar-0.4.2/ellar/common/routing/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import typing as t
 
+from starlette.routing import Host, Mount
+
 from ellar.common.params.params import ParamFieldInfo as Param, ParamTypes
 
 from .base import RouteOperationBase
 from .mount import ModuleMount, ModuleRouter
 from .operation_definitions import OperationDefinitions
 from .route import RouteOperation
 from .route_collections import RouteCollection
@@ -42,12 +44,14 @@
     "RouteCollection",
     "ModuleRouter",
     "ModuleMount",
     "RouteOperation",
     "RouteOperationBase",
     "OperationDefinitions",
     "WebsocketRouteOperation",
+    "Host",
+    "Mount",
 ]
 
 
 def __dir__() -> t.List[str]:
     return sorted(__all__)  # pragma: no cover
```

### Comparing `ellar-0.4.0/ellar/common/routing/base.py` & `ellar-0.4.2/ellar/common/routing/base.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/common/routing/controller/base.py` & `ellar-0.4.2/ellar/common/routing/controller/base.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/common/routing/controller/route.py` & `ellar-0.4.2/ellar/common/routing/controller/route.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/common/routing/controller/websocket/handler.py` & `ellar-0.4.2/ellar/common/routing/controller/websocket/handler.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/common/routing/controller/websocket/route.py` & `ellar-0.4.2/ellar/common/routing/controller/websocket/route.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/common/routing/mount.py` & `ellar-0.4.2/ellar/common/routing/mount.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/common/routing/operation_definitions.py` & `ellar-0.4.2/ellar/common/routing/operation_definitions.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/common/routing/route.py` & `ellar-0.4.2/ellar/common/routing/route.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/common/routing/route_collections.py` & `ellar-0.4.2/ellar/common/routing/route_collections.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/common/routing/schema.py` & `ellar-0.4.2/ellar/common/routing/schema.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/common/routing/websocket/handler.py` & `ellar-0.4.2/ellar/common/routing/websocket/handler.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/common/routing/websocket/route.py` & `ellar-0.4.2/ellar/common/routing/websocket/route.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/common/serializer/base.py` & `ellar-0.4.2/ellar/common/serializer/base.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/common/templating/__init__.py` & `ellar-0.4.2/ellar/common/templating/__init__.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/common/templating/loader.py` & `ellar-0.4.2/ellar/common/templating/loader.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/common/templating/model.py` & `ellar-0.4.2/ellar/common/templating/model.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/common/templating/renderer.py` & `ellar-0.4.2/ellar/common/templating/renderer.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/common/types.py` & `ellar-0.4.2/ellar/common/types.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/core/__init__.py` & `ellar-0.4.2/ellar/core/__init__.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/core/conf/app_settings_models.py` & `ellar-0.4.2/ellar/core/conf/app_settings_models.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/core/conf/config.py` & `ellar-0.4.2/ellar/core/conf/config.py`

 * *Files 13% similar despite different names*

```diff
@@ -17,38 +17,43 @@
 
 class Config(DataMutableMapper, AttributeDictAccessMixin, ConfigDefaultTypesMixin):
     __slots__ = ("config_module", "_data")
 
     def __init__(
         self,
         config_module: str = None,
+        config_prefix: str = None,
         **mapping: t.Any,
     ):
         """
         Creates a new instance of Configuration object with the given values.
         """
         super().__init__()
         self.config_module = config_module or environ.get(ELLAR_CONFIG_MODULE, None)
 
         self._data.clear()
 
+        self._load_config_module(config_prefix or "")
+
+        self._data.update(**mapping)
+
+        validate_config = ConfigValidationSchema.parse_obj(self._data)
+        self._data.update(validate_config.serialize())
+
+    def _load_config_module(self, prefix: str) -> None:
+        _prefix = prefix.upper()
         if self.config_module:
             try:
                 mod = import_from_string(self.config_module)
                 for setting in dir(mod):
-                    if setting.isupper():
-                        self._data[setting] = getattr(mod, setting)
+                    if setting.isupper() and setting.startswith(_prefix):
+                        self._data[setting.replace(_prefix, "")] = getattr(mod, setting)
             except Exception as ex:
                 raise ConfigRuntimeError(str(ex))
 
-        self._data.update(**mapping)
-
-        validate_config = ConfigValidationSchema.parse_obj(self._data)
-        self._data.update(validate_config.serialize())
-
     def set_defaults(self, **kwargs: t.Any) -> "Config":
         for k, v in kwargs.items():
             self._data.setdefault(k, v)
         return self
 
     def __repr__(self) -> str:  # pragma: no cover
         hidden_values = {key: "..." for key in self._data.keys()}
```

### Comparing `ellar-0.4.0/ellar/core/conf/mixins.py` & `ellar-0.4.2/ellar/core/conf/mixins.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/core/connection/http.py` & `ellar-0.4.2/ellar/core/connection/http.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/core/context/execution.py` & `ellar-0.4.2/ellar/core/context/execution.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/core/context/factory.py` & `ellar-0.4.2/ellar/core/context/factory.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/core/context/host.py` & `ellar-0.4.2/ellar/core/context/host.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/core/context/http.py` & `ellar-0.4.2/ellar/core/context/http.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/core/context/websocket.py` & `ellar-0.4.2/ellar/core/context/websocket.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/core/core_service_registration.py` & `ellar-0.4.2/ellar/core/core_service_registration.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/core/exceptions/service.py` & `ellar-0.4.2/ellar/core/exceptions/service.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/core/factory.py` & `ellar-0.4.2/ellar/core/factory.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/core/guard/apikey.py` & `ellar-0.4.2/ellar/core/guard/apikey.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/core/guard/consumer.py` & `ellar-0.4.2/ellar/core/guard/consumer.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/core/guard/http.py` & `ellar-0.4.2/ellar/core/guard/http.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/core/interceptors/consumer.py` & `ellar-0.4.2/ellar/core/interceptors/consumer.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/core/main.py` & `ellar-0.4.2/ellar/core/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from ellar.common.constants import LOG_LEVELS
 from ellar.common.datastructures import State, URLPath
 from ellar.common.interfaces import IExceptionHandler, IExceptionMiddlewareService
 from ellar.common.logger import logger
 from ellar.common.models import EllarInterceptor, GuardCanActivate
 from ellar.common.templating import Environment
 from ellar.common.types import ASGIApp, T, TReceive, TScope, TSend
+from ellar.core.lifespan import EllarApplicationLifespan
 from ellar.core.middleware import (
     CORSMiddleware,
     ExceptionMiddleware,
     Middleware,
     RequestServiceProviderMiddleware,
     RequestVersioningMiddleware,
     TrustedHostMiddleware,
@@ -67,15 +68,17 @@
         self.config.DEFAULT_LIFESPAN_HANDLER = (
             lifespan or self.config.DEFAULT_LIFESPAN_HANDLER
         )
         self.router = ApplicationRouter(
             routes=self._get_module_routes(),
             redirect_slashes=self.config.REDIRECT_SLASHES,
             default=self.config.DEFAULT_NOT_FOUND_HANDLER,  # type: ignore
-            lifespan=self.config.DEFAULT_LIFESPAN_HANDLER,
+            lifespan=EllarApplicationLifespan(
+                self.config.DEFAULT_LIFESPAN_HANDLER  # type: ignore[arg-type]
+            ).lifespan,
         )
         self.middleware_stack = self.build_middleware_stack()
         self._finalize_app_initialization()
         self._config_logging()
 
     def _config_logging(self) -> None:
         log_level = (
```

### Comparing `ellar-0.4.0/ellar/core/middleware/__init__.py` & `ellar-0.4.2/ellar/core/middleware/__init__.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/core/middleware/di.py` & `ellar-0.4.2/ellar/core/middleware/di.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/core/middleware/exceptions.py` & `ellar-0.4.2/ellar/core/middleware/exceptions.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/core/middleware/function.py` & `ellar-0.4.2/ellar/core/middleware/function.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/core/middleware/versioning.py` & `ellar-0.4.2/ellar/core/middleware/versioning.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/core/modules/base.py` & `ellar-0.4.2/ellar/core/modules/base.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/core/modules/builder.py` & `ellar-0.4.2/ellar/core/modules/builder.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/core/modules/config.py` & `ellar-0.4.2/ellar/core/modules/config.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/core/modules/helper.py` & `ellar-0.4.2/ellar/core/modules/helper.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/core/modules/ref.py` & `ellar-0.4.2/ellar/core/modules/ref.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/core/routing/app.py` & `ellar-0.4.2/ellar/core/routing/app.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/core/routing/builder.py` & `ellar-0.4.2/ellar/core/routing/builder.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/core/routing/factory.py` & `ellar-0.4.2/ellar/core/routing/factory.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/core/routing/helper.py` & `ellar-0.4.2/ellar/core/routing/helper.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/core/routing/module_router.py` & `ellar-0.4.2/ellar/core/routing/module_router.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/core/services/reflector.py` & `ellar-0.4.2/ellar/core/services/reflector.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/core/staticfiles.py` & `ellar-0.4.2/ellar/core/staticfiles.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/core/templating/app.py` & `ellar-0.4.2/ellar/core/templating/app.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/core/versioning/__init__.py` & `ellar-0.4.2/ellar/core/versioning/__init__.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/core/versioning/base.py` & `ellar-0.4.2/ellar/core/versioning/base.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/core/versioning/resolver.py` & `ellar-0.4.2/ellar/core/versioning/resolver.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/di/__init__.py` & `ellar-0.4.2/ellar/di/__init__.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/di/constants.py` & `ellar-0.4.2/ellar/di/constants.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/di/injector/container.py` & `ellar-0.4.2/ellar/di/injector/container.py`

 * *Files 1% similar despite different names*

```diff
@@ -234,16 +234,16 @@
 
         instance = t.cast(t.Union[t.Type["ModuleBase"], "ModuleBase"], module)
 
         if isinstance(instance, type) and issubclass(
             t.cast(type, instance), InjectorModule
         ):
             instance = t.cast(type, instance)(**init_kwargs)
-        elif isinstance(instance, type) and not isinstance(instance, InjectorModule):
+        elif isinstance(instance, type):
             return self.injector.get(t.cast(type, instance))
         elif not isinstance(instance, type) and not isinstance(
-            type(instance), InjectorModule
+            instance, InjectorModule
         ):
             return instance
 
         instance(self)
         return instance
```

### Comparing `ellar-0.4.0/ellar/di/injector/ellar_injector.py` & `ellar-0.4.2/ellar/di/injector/ellar_injector.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/di/providers.py` & `ellar-0.4.2/ellar/di/providers.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/di/scopes.py` & `ellar-0.4.2/ellar/di/scopes.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/di/service_config.py` & `ellar-0.4.2/ellar/di/service_config.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/events.py` & `ellar-0.4.2/ellar/events.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/openapi/__init__.py` & `ellar-0.4.2/ellar/openapi/__init__.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/openapi/builder.py` & `ellar-0.4.2/ellar/openapi/builder.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/openapi/docs_generators/base.py` & `ellar-0.4.2/ellar/openapi/docs_generators/base.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/openapi/docs_generators/redocs.py` & `ellar-0.4.2/ellar/openapi/docs_generators/redocs.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/openapi/docs_generators/swagger.py` & `ellar-0.4.2/ellar/openapi/docs_generators/swagger.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/openapi/module.py` & `ellar-0.4.2/ellar/openapi/module.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/openapi/openapi_v3.py` & `ellar-0.4.2/ellar/openapi/openapi_v3.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/openapi/route_doc_models.py` & `ellar-0.4.2/ellar/openapi/route_doc_models.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/openapi/templates/redocs.html` & `ellar-0.4.2/ellar/openapi/templates/redocs.html`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/openapi/templates/swagger.html` & `ellar-0.4.2/ellar/openapi/templates/swagger.html`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/reflect/_reflect.py` & `ellar-0.4.2/ellar/reflect/_reflect.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/samples/static/css/bootstrap.min.css` & `ellar-0.4.2/ellar/samples/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/samples/static/img/EllarLogoB.png` & `ellar-0.4.2/ellar/samples/static/img/EllarLogoB.png`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/samples/static/img/EllarLogoIconOnly.png` & `ellar-0.4.2/ellar/samples/static/img/EllarLogoIconOnly.png`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/samples/static/img/Icon.svg` & `ellar-0.4.2/ellar/samples/static/img/Icon.svg`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/samples/templates/home/index.html` & `ellar-0.4.2/ellar/samples/templates/home/index.html`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/socket_io/__init__.py` & `ellar-0.4.2/ellar/socket_io/__init__.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/socket_io/constants.py` & `ellar-0.4.2/ellar/socket_io/constants.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/socket_io/context.py` & `ellar-0.4.2/ellar/socket_io/context.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/socket_io/decorators/events.py` & `ellar-0.4.2/ellar/socket_io/decorators/events.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/socket_io/decorators/gateway.py` & `ellar-0.4.2/ellar/socket_io/decorators/gateway.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/socket_io/decorators/subscribe_message.py` & `ellar-0.4.2/ellar/socket_io/decorators/subscribe_message.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/socket_io/factory.py` & `ellar-0.4.2/ellar/socket_io/factory.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/socket_io/gateway.py` & `ellar-0.4.2/ellar/socket_io/gateway.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/socket_io/testing/module.py` & `ellar-0.4.2/ellar/socket_io/testing/module.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/testing/module.py` & `ellar-0.4.2/ellar/testing/module.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/ellar/testing/uvicorn_server.py` & `ellar-0.4.2/ellar/testing/uvicorn_server.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/examples/01-carapp/carapp/apps/car/controllers.py` & `ellar-0.4.2/examples/01-carapp/carapp/apps/car/controllers.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/examples/01-carapp/carapp/apps/car/module.py` & `ellar-0.4.2/examples/01-carapp/carapp/apps/car/module.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/examples/01-carapp/carapp/apps/car/routers.py` & `ellar-0.4.2/examples/01-carapp/carapp/apps/car/routers.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/examples/01-carapp/carapp/apps/car/schemas.py` & `ellar-0.4.2/examples/01-carapp/carapp/apps/car/schemas.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/examples/01-carapp/carapp/apps/car/services.py` & `ellar-0.4.2/examples/01-carapp/carapp/apps/car/services.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/examples/01-carapp/carapp/apps/car/statics/blog/blog.css` & `ellar-0.4.2/examples/01-carapp/carapp/apps/car/statics/blog/blog.css`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/examples/01-carapp/carapp/apps/car/statics/blog/blog.rtl.css` & `ellar-0.4.2/examples/01-carapp/carapp/apps/car/statics/blog/blog.rtl.css`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/examples/01-carapp/carapp/apps/car/statics/brand/bootstrap-logo-white.svg` & `ellar-0.4.2/examples/01-carapp/carapp/apps/car/statics/brand/bootstrap-logo-white.svg`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/examples/01-carapp/carapp/apps/car/statics/brand/bootstrap-logo.svg` & `ellar-0.4.2/examples/01-carapp/carapp/apps/car/statics/brand/bootstrap-logo.svg`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/examples/01-carapp/carapp/apps/car/tests/test_controllers.py` & `ellar-0.4.2/examples/01-carapp/carapp/apps/car/tests/test_controllers.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/examples/01-carapp/carapp/apps/car/tests/test_routers.py` & `ellar-0.4.2/examples/01-carapp/carapp/apps/car/tests/test_routers.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/examples/01-carapp/carapp/apps/car/views/index.html` & `ellar-0.4.2/examples/01-carapp/carapp/apps/car/views/index.html`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/examples/01-carapp/carapp/root_module.py` & `ellar-0.4.2/examples/01-carapp/carapp/root_module.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/examples/01-carapp/carapp/server.py` & `ellar-0.4.2/examples/01-carapp/carapp/server.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/examples/02-socketio-app/socketio_app/apps/events/gateways.py` & `ellar-0.4.2/examples/02-socketio-app/socketio_app/apps/events/gateways.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/examples/02-socketio-app/socketio_app/apps/events/module.py` & `ellar-0.4.2/examples/02-socketio-app/socketio_app/apps/events/module.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/examples/02-socketio-app/socketio_app/apps/events/schemas.py` & `ellar-0.4.2/examples/02-socketio-app/socketio_app/apps/events/schemas.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/examples/02-socketio-app/socketio_app/apps/events/templates/events/index.html` & `ellar-0.4.2/examples/02-socketio-app/socketio_app/apps/events/templates/events/index.html`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/examples/02-socketio-app/socketio_app/config.py` & `ellar-0.4.2/examples/02-socketio-app/socketio_app/config.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/examples/02-socketio-app/socketio_app/server.py` & `ellar-0.4.2/examples/02-socketio-app/socketio_app/server.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/mypy.ini` & `ellar-0.4.2/mypy.ini`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/pyproject.toml` & `ellar-0.4.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -38,19 +38,19 @@
     "Framework :: AsyncIO",
     "Topic :: Internet :: WWW/HTTP :: HTTP Servers",
     "Topic :: Internet :: WWW/HTTP",
 ]
 
 dependencies = [
     "injector == 0.20.1",
-    "starlette == 0.26.1",
+    "starlette == 0.27.0",
     "pydantic >=1.6.2,!=1.7,!=1.7.1,!=1.7.2,!=1.7.3,!=1.8,!=1.8.1,<2.0.0",
     "jinja2",
     # cli
-    "typer >=0.6.1,<0.8.0",
+    "typer >=0.6.1,<0.10.0",
     # testing
     "httpx >= 0.22.0"
 ]
 
 [project.urls]
 Documentation = "https://github.com/eadwinCode/ellar"
 Source = "https://github.com/eadwinCode/ellar"
@@ -78,15 +78,15 @@
     "redis",
     "itsdangerous >=1.1.0,<3.0.0",
     # types
     "types-ujson ==5.7.0.5",
     "types-orjson ==3.6.2",
     "types-dataclasses ==0.6.6",
     "python-socketio",
-    "uvicorn[standard] == 0.20.0",
+    "uvicorn[standard] == 0.22.0",
     "aiohttp == 3.8.4",
 ]
 dev = [
     "pre-commit"
 ]
 
 all = [
```

### Comparing `ellar-0.4.0/tests/conftest.py` & `ellar-0.4.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/tests/injector_module.py` & `ellar-0.4.2/tests/injector_module.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/tests/main.py` & `ellar-0.4.2/tests/main.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/tests/schema.py` & `ellar-0.4.2/tests/schema.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/tests/test_application/sample.py` & `ellar-0.4.2/tests/test_application/sample.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/tests/test_application/test_application_factory.py` & `ellar-0.4.2/tests/test_application/test_application_factory.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/tests/test_application/test_application_functions.py` & `ellar-0.4.2/tests/test_application/test_application_functions.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/tests/test_application/test_cors.py` & `ellar-0.4.2/tests/test_application/test_cors.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/tests/test_application/test_replacing_app_services.py` & `ellar-0.4.2/tests/test_application/test_replacing_app_services.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/tests/test_application/test_trusted_host.py` & `ellar-0.4.2/tests/test_application/test_trusted_host.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/tests/test_attribute_dict.py` & `ellar-0.4.2/tests/test_attribute_dict.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/tests/test_cache/_test_aio_memcache.py.ellar` & `ellar-0.4.2/tests/test_cache/_test_aio_memcache.py.ellar`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/tests/test_cache/pylib_mock.py` & `ellar-0.4.2/tests/test_cache/pylib_mock.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/tests/test_cache/redis_mock.py` & `ellar-0.4.2/tests/test_cache/redis_mock.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/tests/test_cache/test_cache_decorator.py` & `ellar-0.4.2/tests/test_cache/test_cache_decorator.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/tests/test_cache/test_cache_many_config.py` & `ellar-0.4.2/tests/test_cache/test_cache_many_config.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/tests/test_cache/test_cache_service.py` & `ellar-0.4.2/tests/test_cache/test_cache_service.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/tests/test_cache/test_local_cache.py` & `ellar-0.4.2/tests/test_cache/test_local_cache.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/tests/test_cache/test_module_setup.py` & `ellar-0.4.2/tests/test_cache/test_module_setup.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/tests/test_cache/test_pylibmc_cache.py` & `ellar-0.4.2/tests/test_cache/test_pylibmc_cache.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/tests/test_cache/test_redis_cache.py` & `ellar-0.4.2/tests/test_cache/test_redis_cache.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/tests/test_cache/test_schema.py` & `ellar-0.4.2/tests/test_cache/test_schema.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/tests/test_conf/test_default_conf.py` & `ellar-0.4.2/tests/test_conf/test_default_conf.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/tests/test_conf/test_mixins.py` & `ellar-0.4.2/tests/test_conf/test_mixins.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/tests/test_controller/test_controller_decorator.py` & `ellar-0.4.2/tests/test_controller/test_controller_decorator.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/tests/test_controller/test_controller_inheritance.py` & `ellar-0.4.2/tests/test_controller/test_controller_inheritance.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/tests/test_controller/test_module_router.py` & `ellar-0.4.2/tests/test_controller/test_module_router.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/tests/test_controller/test_route_collection.py` & `ellar-0.4.2/tests/test_controller/test_route_collection.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/tests/test_decorators/test_controller.py` & `ellar-0.4.2/tests/test_decorators/test_controller.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/tests/test_decorators/test_exception.py` & `ellar-0.4.2/tests/test_decorators/test_exception.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/tests/test_decorators/test_file.py` & `ellar-0.4.2/tests/test_decorators/test_file.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/tests/test_decorators/test_guards.py` & `ellar-0.4.2/tests/test_decorators/test_guards.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/tests/test_decorators/test_html.py` & `ellar-0.4.2/tests/test_decorators/test_html.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/tests/test_decorators/test_middleware.py` & `ellar-0.4.2/tests/test_decorators/test_middleware.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/tests/test_decorators/test_modules.py` & `ellar-0.4.2/tests/test_decorators/test_modules.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/tests/test_decorators/test_openapi.py` & `ellar-0.4.2/tests/test_decorators/test_openapi.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/tests/test_decorators/test_serializer.py` & `ellar-0.4.2/tests/test_decorators/test_serializer.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/tests/test_di/examples.py` & `ellar-0.4.2/tests/test_di/examples.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/tests/test_di/test_injectable_resolving.py` & `ellar-0.4.2/tests/test_di/test_injectable_resolving.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/tests/test_di/test_injector.py` & `ellar-0.4.2/tests/test_di/test_injector.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,35 +21,44 @@
     pass
 
 
 def test_container_install_module_case_1():
     called = False
     app_container = EllarInjector().container
 
-    class FakeModule(ModuleBase):
+    class PlainModule(ModuleBase):
         def register_services(self, container: Container) -> None:
             nonlocal called
             called = True
 
     @Module()
     class DecoratedModuleWithBase(ModuleBase):
         def register_services(self, container: Container) -> None:
             nonlocal called
             called = True
 
-    fake_module = app_container.install(FakeModule)
+    plain_module = app_container.install(PlainModule)
     assert called
-    assert isinstance(fake_module, FakeModule)
+    assert isinstance(plain_module, PlainModule)
 
     called = False
 
     decorated_module = app_container.install(DecoratedModuleWithBase)
     assert called
     assert isinstance(decorated_module, DecoratedModuleWithBase)
 
+    called = False
+    app_container.install(PlainModule())
+    assert called
+
+    called = False
+
+    app_container.install(DecoratedModuleWithBase())
+    assert called
+
 
 def test_container_install_module_return_case_2():
     called = False
     app_container = EllarInjector().container
 
     @Module()
     class DecoratedModule:
@@ -57,14 +66,18 @@
             nonlocal called
             called = True
 
     decorated_module = app_container.install(DecoratedModule)
     assert called is False
     assert isinstance(decorated_module, DecoratedModule)
 
+    decorated_module = app_container.install(DecoratedModule())
+    assert called is False
+    assert isinstance(decorated_module, DecoratedModule)
+
 
 def test_default_container_registration():
     injector = EllarInjector(auto_bind=False)
     assert isinstance(injector.get(Container), Container)
     assert isinstance(injector.get(EllarInjector), EllarInjector)
     assert isinstance(injector.get(EllarInjector), EllarInjector)
```

### Comparing `ellar-0.4.0/tests/test_di/test_provider_scopes.py` & `ellar-0.4.2/tests/test_di/test_provider_scopes.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/tests/test_di/test_providers.py` & `ellar-0.4.2/tests/test_di/test_providers.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/tests/test_events.py` & `ellar-0.4.2/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/tests/test_exceptions/test_api_exception.py` & `ellar-0.4.2/tests/test_exceptions/test_api_exception.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/tests/test_exceptions/test_custom_exceptions.py` & `ellar-0.4.2/tests/test_exceptions/test_custom_exceptions.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/tests/test_exceptions/test_error_details.py` & `ellar-0.4.2/tests/test_exceptions/test_error_details.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/tests/test_exceptions/test_validation_exception.py` & `ellar-0.4.2/tests/test_exceptions/test_validation_exception.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/tests/test_guard.py` & `ellar-0.4.2/tests/test_guard.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/tests/test_helper/test_enum.py` & `ellar-0.4.2/tests/test_helper/test_enum.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/tests/test_helper/test_model_field.py` & `ellar-0.4.2/tests/test_helper/test_model_field.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/tests/test_interceptors/test_interceptor.py` & `ellar-0.4.2/tests/test_interceptors/test_interceptor.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/tests/test_middleware/test_functional_middleware.py` & `ellar-0.4.2/tests/test_middleware/test_functional_middleware.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/tests/test_middleware/test_service_provider_middleware.py` & `ellar-0.4.2/tests/test_middleware/test_service_provider_middleware.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/tests/test_middleware/test_versioning_middleware.py` & `ellar-0.4.2/tests/test_middleware/test_versioning_middleware.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/tests/test_modules/sample.py` & `ellar-0.4.2/tests/test_modules/sample.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/tests/test_modules/test_module_config.py` & `ellar-0.4.2/tests/test_modules/test_module_config.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/tests/test_modules/test_module_ref.py` & `ellar-0.4.2/tests/test_modules/test_module_ref.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/tests/test_openapi/test_builder.py` & `ellar-0.4.2/tests/test_openapi/test_builder.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/tests/test_openapi/test_module.py` & `ellar-0.4.2/tests/test_openapi/test_module.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/tests/test_openapi/test_open_api_route_documentation.py` & `ellar-0.4.2/tests/test_openapi/test_open_api_route_documentation.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/tests/test_reflect.py` & `ellar-0.4.2/tests/test_reflect.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/tests/test_reflector.py` & `ellar-0.4.2/tests/test_reflector.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/tests/test_response/test_defined_response_model.py` & `ellar-0.4.2/tests/test_response/test_defined_response_model.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/tests/test_response/test_pydantic_response_model.py` & `ellar-0.4.2/tests/test_response/test_pydantic_response_model.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/tests/test_response/test_response_file.py` & `ellar-0.4.2/tests/test_response/test_response_file.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/tests/test_response/test_response_html.py` & `ellar-0.4.2/tests/test_response/test_response_html.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/tests/test_response/test_response_streaming.py` & `ellar-0.4.2/tests/test_response/test_response_streaming.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/tests/test_response/test_response_type_definition_converter.py` & `ellar-0.4.2/tests/test_response/test_response_type_definition_converter.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/tests/test_response/test_route_response_model.py` & `ellar-0.4.2/tests/test_response/test_route_response_model.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/tests/test_routing/sample.py` & `ellar-0.4.2/tests/test_routing/sample.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/tests/test_routing/test_background_tasks.py` & `ellar-0.4.2/tests/test_routing/test_background_tasks.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/tests/test_routing/test_body_schema.py` & `ellar-0.4.2/tests/test_routing/test_body_schema.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/tests/test_routing/test_body_schema_extra_properties.py` & `ellar-0.4.2/tests/test_routing/test_body_schema_extra_properties.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/tests/test_routing/test_body_union_schema.py` & `ellar-0.4.2/tests/test_routing/test_body_union_schema.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/tests/test_routing/test_cookie_schema.py` & `ellar-0.4.2/tests/test_routing/test_cookie_schema.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/tests/test_routing/test_extra_args.py` & `ellar-0.4.2/tests/test_routing/test_extra_args.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/tests/test_routing/test_form_schema.py` & `ellar-0.4.2/tests/test_routing/test_form_schema.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/tests/test_routing/test_formparsers.py` & `ellar-0.4.2/tests/test_routing/test_formparsers.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/tests/test_routing/test_forms.py` & `ellar-0.4.2/tests/test_routing/test_forms.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/tests/test_routing/test_forms_from_non_typing_sequences.py` & `ellar-0.4.2/tests/test_routing/test_forms_from_non_typing_sequences.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/tests/test_routing/test_header_schema.py` & `ellar-0.4.2/tests/test_routing/test_header_schema.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/tests/test_routing/test_invalid_path_param.py` & `ellar-0.4.2/tests/test_routing/test_invalid_path_param.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/tests/test_routing/test_invalid_sequence_param.py` & `ellar-0.4.2/tests/test_routing/test_invalid_sequence_param.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/tests/test_routing/test_multi_body_errors.py` & `ellar-0.4.2/tests/test_routing/test_multi_body_errors.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/tests/test_routing/test_multi_query_errors.py` & `ellar-0.4.2/tests/test_routing/test_multi_query_errors.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/tests/test_routing/test_path.py` & `ellar-0.4.2/tests/test_routing/test_path.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/tests/test_routing/test_path_with_schema.py` & `ellar-0.4.2/tests/test_routing/test_path_with_schema.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/tests/test_routing/test_put_with_no_body_schema.py` & `ellar-0.4.2/tests/test_routing/test_put_with_no_body_schema.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/tests/test_routing/test_query.py` & `ellar-0.4.2/tests/test_routing/test_query.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/tests/test_routing/test_query_schema.py` & `ellar-0.4.2/tests/test_routing/test_query_schema.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/tests/test_routing/test_request.py` & `ellar-0.4.2/tests/test_routing/test_request.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/tests/test_routing/test_route_endpoint_params.py` & `ellar-0.4.2/tests/test_routing/test_route_endpoint_params.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/tests/test_schema.py` & `ellar-0.4.2/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/tests/test_serializer.py` & `ellar-0.4.2/tests/test_serializer.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/tests/test_shortcuts.py` & `ellar-0.4.2/tests/test_shortcuts.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/tests/test_socket_io/sample.py` & `ellar-0.4.2/tests/test_socket_io/sample.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/tests/test_socket_io/test_decorators/test_events.py` & `ellar-0.4.2/tests/test_socket_io/test_decorators/test_events.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/tests/test_socket_io/test_decorators/test_gateway.py` & `ellar-0.4.2/tests/test_socket_io/test_decorators/test_gateway.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/tests/test_socket_io/test_decorators/test_subcribe_message.py` & `ellar-0.4.2/tests/test_socket_io/test_decorators/test_subcribe_message.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/tests/test_socket_io/test_gateway.py` & `ellar-0.4.2/tests/test_socket_io/test_gateway.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/tests/test_socket_io/test_operation.py` & `ellar-0.4.2/tests/test_socket_io/test_operation.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/tests/test_staticfiles.py` & `ellar-0.4.2/tests/test_staticfiles.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/tests/test_templating/test_module_templating.py` & `ellar-0.4.2/tests/test_templating/test_module_templating.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/tests/test_templating/test_renderer.py` & `ellar-0.4.2/tests/test_templating/test_renderer.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/tests/test_testing.py` & `ellar-0.4.2/tests/test_testing.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/tests/test_versioning/operations.py` & `ellar-0.4.2/tests/test_versioning/operations.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/tests/test_versioning/test_default_versioning.py` & `ellar-0.4.2/tests/test_versioning/test_default_versioning.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/tests/test_versioning/test_default_versioning_for_controllers.py` & `ellar-0.4.2/tests/test_versioning/test_default_versioning_for_controllers.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/tests/test_versioning/test_header_versioning.py` & `ellar-0.4.2/tests/test_versioning/test_header_versioning.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/tests/test_versioning/test_header_versioning_controller.py` & `ellar-0.4.2/tests/test_versioning/test_header_versioning_controller.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/tests/test_versioning/test_host_versioning.py` & `ellar-0.4.2/tests/test_versioning/test_host_versioning.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/tests/test_versioning/test_query_versioning.py` & `ellar-0.4.2/tests/test_versioning/test_query_versioning.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/tests/test_versioning/test_url_versioning.py` & `ellar-0.4.2/tests/test_versioning/test_url_versioning.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/tests/test_websocket.py` & `ellar-0.4.2/tests/test_websocket.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/tests/test_websocket_handler.py` & `ellar-0.4.2/tests/test_websocket_handler.py`

 * *Files identical despite different names*

### Comparing `ellar-0.4.0/PKG-INFO` & `ellar-0.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ellar
-Version: 0.4.0
+Version: 0.4.2
 Summary: Ellar - Python ASGI web framework for building fast, efficient and scalable RESTAPIs and server-side application.
 Author-email: Ezeudoh Tochukwu <tochukwu.ezeudoh@gmail.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: OS Independent
@@ -24,18 +24,18 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Framework :: AsyncIO
 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
 Classifier: Topic :: Internet :: WWW/HTTP
 Requires-Dist: injector == 0.20.1
-Requires-Dist: starlette == 0.26.1
+Requires-Dist: starlette == 0.27.0
 Requires-Dist: pydantic >=1.6.2,!=1.7,!=1.7.1,!=1.7.2,!=1.7.3,!=1.8,!=1.8.1,<2.0.0
 Requires-Dist: jinja2
-Requires-Dist: typer >=0.6.1,<0.8.0
+Requires-Dist: typer >=0.6.1,<0.10.0
 Requires-Dist: httpx >= 0.22.0
 Requires-Dist: python-multipart >=0.0.5,<0.0.7 ; extra == "all"
 Requires-Dist: itsdangerous >=1.1.0,<3.0.0 ; extra == "all"
 Requires-Dist: pyyaml >=5.3.1,<7.0.0 ; extra == "all"
 Requires-Dist: ujson >=4.0.1,!=4.0.2,!=4.1.0,!=4.2.0,!=4.3.0,!=5.0.0,!=5.1.0,<6.0.0 ; extra == "all"
 Requires-Dist: orjson >=3.2.1,<4.0.0 ; extra == "all"
 Requires-Dist: email_validator >=1.1.1,<3.0.0 ; extra == "all"
@@ -67,15 +67,15 @@
 Requires-Dist: aiomcache ; extra == "test"
 Requires-Dist: redis ; extra == "test"
 Requires-Dist: itsdangerous >=1.1.0,<3.0.0 ; extra == "test"
 Requires-Dist: types-ujson ==5.7.0.5 ; extra == "test"
 Requires-Dist: types-orjson ==3.6.2 ; extra == "test"
 Requires-Dist: types-dataclasses ==0.6.6 ; extra == "test"
 Requires-Dist: python-socketio ; extra == "test"
-Requires-Dist: uvicorn[standard] == 0.20.0 ; extra == "test"
+Requires-Dist: uvicorn[standard] == 0.22.0 ; extra == "test"
 Requires-Dist: aiohttp == 3.8.4 ; extra == "test"
 Project-URL: Documentation, https://github.com/eadwinCode/ellar
 Project-URL: Homepage, https://eadwincode.github.io/ellar/
 Project-URL: Source, https://github.com/eadwinCode/ellar
 Provides-Extra: all
 Provides-Extra: dev
 Provides-Extra: doc
```

