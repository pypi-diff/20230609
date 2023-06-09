# Comparing `tmp/orwynn-1.0.0b4.tar.gz` & `tmp/orwynn-1.0.0b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orwynn-1.0.0b4.tar", max compression
+gzip compressed data, was "orwynn-1.0.0b5.tar", max compression
```

## Comparing `orwynn-1.0.0b4.tar` & `orwynn-1.0.0b5.tar`

### file list

```diff
@@ -1,260 +1,251 @@
--rw-r--r--   0        0        0     1072 2022-12-08 10:08:41.917165 orwynn-1.0.0b4/LICENSE
--rw-r--r--   0        0        0      307 2023-05-22 08:29:05.173562 orwynn-1.0.0b4/README.md
--rw-r--r--   0        0        0       65 2023-03-07 08:24:06.640906 orwynn-1.0.0b4/orwynn/__init__.py
--rw-r--r--   0        0        0       63 2022-12-11 09:09:39.933971 orwynn-1.0.0b4/orwynn/_di/Acceptor.py
--rw-r--r--   0        0        0      500 2023-03-06 12:12:57.645660 orwynn-1.0.0b4/orwynn/_di/BUILTIN_ACCEPTORS.py
--rw-r--r--   0        0        0      399 2023-02-28 05:48:16.657065 orwynn-1.0.0b4/orwynn/_di/BUILTIN_PROVIDERS.py
--rw-r--r--   0        0        0     4726 2023-04-03 14:59:49.701980 orwynn-1.0.0b4/orwynn/_di/Di.py
--rw-r--r--   0        0        0     6038 2023-04-03 14:59:49.636980 orwynn-1.0.0b4/orwynn/_di/DiContainer.py
--rw-r--r--   0        0        0      140 2023-02-15 12:49:24.369340 orwynn-1.0.0b4/orwynn/_di/DiObject.py
--rw-r--r--   0        0        0      119 2023-03-06 11:23:49.043895 orwynn-1.0.0b4/orwynn/_di/DiObjectAlreadyInitializedInContainerError.py
--rw-r--r--   0        0        0      132 2023-03-06 11:23:49.043895 orwynn-1.0.0b4/orwynn/_di/FinalizedDiContainerError.py
--rw-r--r--   0        0        0       51 2023-03-06 11:23:49.043895 orwynn-1.0.0b4/orwynn/_di/MissingDiObjectError.py
--rw-r--r--   0        0        0       96 2023-03-06 11:23:49.043895 orwynn-1.0.0b4/orwynn/_di/NoAnnotationError.py
--rw-r--r--   0        0        0      291 2023-03-06 11:23:49.043895 orwynn-1.0.0b4/orwynn/_di/NotProviderError.py
--rw-r--r--   0        0        0       39 2022-12-11 09:09:05.931124 orwynn-1.0.0b4/orwynn/_di/Provider.py
--rw-r--r--   0        0        0      579 2023-03-06 11:30:55.552595 orwynn-1.0.0b4/orwynn/_di/ProviderAvailabilityError.py
--rw-r--r--   0        0        0      101 2023-03-06 14:58:11.412882 orwynn-1.0.0b4/orwynn/_di/__init__.py
--rw-r--r--   0        0        0     1733 2023-03-06 14:58:30.471950 orwynn-1.0.0b4/orwynn/_di/_collect_dependencies_for_acceptor.py
--rw-r--r--   0        0        0     3856 2023-02-28 05:48:16.658066 orwynn-1.0.0b4/orwynn/_di/check_availability.py
--rw-r--r--   0        0        0     3232 2023-04-03 14:59:49.701980 orwynn-1.0.0b4/orwynn/_di/collecting/ModuleCollector.py
--rw-r--r--   0        0        0      459 2023-03-06 11:30:55.551595 orwynn-1.0.0b4/orwynn/_di/collecting/ProviderAlreadyInitializedForMapError.py
--rw-r--r--   0        0        0     1086 2023-04-03 14:59:49.701980 orwynn-1.0.0b4/orwynn/_di/collecting/collect_modules_test.py
--rw-r--r--   0        0        0     3305 2023-04-03 14:59:49.702980 orwynn-1.0.0b4/orwynn/_di/collecting/collect_provider_dependencies.py
--rw-r--r--   0        0        0     1709 2023-02-28 06:25:30.262229 orwynn-1.0.0b4/orwynn/_di/collecting/collect_provider_dependencies_test.py
--rw-r--r--   0        0        0     3210 2023-02-28 05:48:16.648064 orwynn-1.0.0b4/orwynn/_di/collecting/get_parameters_for_provider.py
--rw-r--r--   0        0        0      324 2023-03-06 11:30:55.551595 orwynn-1.0.0b4/orwynn/_di/collecting/no_dependencies_for_given_provider_error.py
--rw-r--r--   0        0        0     2523 2023-02-27 12:30:57.696823 orwynn-1.0.0b4/orwynn/_di/collecting/provider_dependencies_map.py
--rw-r--r--   0        0        0      138 2023-03-06 11:23:49.055894 orwynn-1.0.0b4/orwynn/_di/collecting/provider_keyword_attribute_error.py
--rw-r--r--   0        0        0      376 2023-03-06 11:30:55.550595 orwynn-1.0.0b4/orwynn/_di/collecting/provider_not_found_in_map_error.py
--rw-r--r--   0        0        0      519 2023-02-28 05:48:16.651064 orwynn-1.0.0b4/orwynn/_di/di_test.py
--rw-r--r--   0        0        0     6771 2023-04-03 14:59:49.705980 orwynn-1.0.0b4/orwynn/_di/init/init_other_acceptors.py
--rw-r--r--   0        0        0     2907 2023-04-03 14:59:49.704980 orwynn-1.0.0b4/orwynn/_di/init/init_other_acceptors_test.py
--rw-r--r--   0        0        0     4157 2023-04-03 14:59:49.702980 orwynn-1.0.0b4/orwynn/_di/init/init_providers.py
--rw-r--r--   0        0        0      628 2023-02-28 05:48:16.657065 orwynn-1.0.0b4/orwynn/_di/init/init_providers_test.py
--rw-r--r--   0        0        0      336 2023-02-27 12:30:57.666822 orwynn-1.0.0b4/orwynn/_di/is_acceptor.py
--rw-r--r--   0        0        0      334 2023-02-27 12:30:57.666822 orwynn-1.0.0b4/orwynn/_di/is_provider.py
--rw-r--r--   0        0        0     1106 2023-05-22 08:13:58.515604 orwynn-1.0.0b4/orwynn/_testingtools/__init__.py
--rw-r--r--   0        0        0     1920 2023-04-03 14:59:49.716980 orwynn-1.0.0b4/orwynn/apiversion/_ApiVersion.py
--rw-r--r--   0        0        0       36 2023-02-23 07:25:38.261308 orwynn-1.0.0b4/orwynn/apiversion/__init__.py
--rw-r--r--   0        0        0     4559 2023-04-03 14:59:49.716980 orwynn-1.0.0b4/orwynn/apiversion/api_version_test.py
--rw-r--r--   0        0        0       54 2023-03-06 11:23:49.055894 orwynn-1.0.0b4/orwynn/apiversion/errors.py
--rw-r--r--   0        0        0      401 2023-03-07 07:20:52.198703 orwynn-1.0.0b4/orwynn/app/_ApiRouter.py
--rw-r--r--   0        0        0     1493 2023-03-07 07:21:08.188882 orwynn-1.0.0b4/orwynn/app/_ApiWebsocketRoute.py
--rw-r--r--   0        0        0     1619 2023-05-22 08:53:59.970818 orwynn-1.0.0b4/orwynn/app/_App.py
--rw-r--r--   0        0        0      120 2023-04-07 10:01:45.607493 orwynn-1.0.0b4/orwynn/app/_AppConfig.py
--rw-r--r--   0        0        0       97 2023-02-27 12:42:05.392452 orwynn-1.0.0b4/orwynn/app/_AppMode.py
--rw-r--r--   0        0        0     1561 2023-03-07 07:20:52.199703 orwynn-1.0.0b4/orwynn/app/_CoreApp.py
--rw-r--r--   0        0        0       86 2023-04-07 10:06:55.137728 orwynn-1.0.0b4/orwynn/app/__init__.py
--rw-r--r--   0        0        0     2885 2023-03-07 07:26:27.308262 orwynn-1.0.0b4/orwynn/app/_get_dependant.py
--rw-r--r--   0        0        0     2207 2023-04-07 10:05:51.094748 orwynn-1.0.0b4/orwynn/app/app_test.py
--rw-r--r--   0        0        0      190 2023-02-27 12:42:54.819951 orwynn-1.0.0b4/orwynn/apprc/_APP_RC_MODE_NESTING.py
--rw-r--r--   0        0        0       13 2023-02-27 06:15:50.756268 orwynn-1.0.0b4/orwynn/apprc/_AppRc.py
--rw-r--r--   0        0        0       47 2023-03-06 11:23:49.055894 orwynn-1.0.0b4/orwynn/apprc/_AppRcSearchError.py
--rw-r--r--   0        0        0       64 2023-02-27 06:16:07.584011 orwynn-1.0.0b4/orwynn/apprc/__init__.py
--rw-r--r--   0        0        0     3516 2023-04-07 09:56:47.710126 orwynn-1.0.0b4/orwynn/apprc/_parse_apprc.py
--rw-r--r--   0        0        0     2608 2023-04-03 14:59:49.734980 orwynn-1.0.0b4/orwynn/apprc/apprc_test.py
--rw-r--r--   0        0        0      374 2023-03-07 08:25:49.974896 orwynn-1.0.0b4/orwynn/base/__init__.py
--rw-r--r--   0        0        0     1116 2023-04-03 14:59:49.383979 orwynn-1.0.0b4/orwynn/base/config/_Config.py
--rw-r--r--   0        0        0       28 2023-02-27 06:19:37.641319 orwynn-1.0.0b4/orwynn/base/config/__init__.py
--rw-r--r--   0        0        0        0 2022-12-18 22:39:38.591866 orwynn-1.0.0b4/orwynn/base/config/config_test.py
--rw-r--r--   0        0        0     2201 2023-04-07 10:26:00.405258 orwynn-1.0.0b4/orwynn/base/controller/_Controller.py
--rw-r--r--   0        0        0       36 2023-02-27 09:39:20.802918 orwynn-1.0.0b4/orwynn/base/controller/__init__.py
--rw-r--r--   0        0        0      179 2023-03-06 11:23:49.043895 orwynn-1.0.0b4/orwynn/base/controller/errors.py
--rw-r--r--   0        0        0      630 2023-02-27 07:44:54.968991 orwynn-1.0.0b4/orwynn/base/database/_Database.py
--rw-r--r--   0        0        0       32 2023-02-27 07:35:06.448928 orwynn-1.0.0b4/orwynn/base/database/__init__.py
--rw-r--r--   0        0        0      528 2023-03-06 11:23:49.038895 orwynn-1.0.0b4/orwynn/base/database/errors.py
--rw-r--r--   0        0        0       86 2023-03-06 11:24:23.455706 orwynn-1.0.0b4/orwynn/base/error/_ErrorValueSchema.py
--rw-r--r--   0        0        0      128 2023-03-06 11:23:49.035894 orwynn-1.0.0b4/orwynn/base/error/_ExceptionAlreadyHandledError.py
--rw-r--r--   0        0        0      157 2023-03-06 11:29:08.008168 orwynn-1.0.0b4/orwynn/base/error/_MalfunctionError.py
--rw-r--r--   0        0        0      403 2023-04-07 09:57:35.357451 orwynn-1.0.0b4/orwynn/base/error/__init__.py
--rw-r--r--   0        0        0     1009 2023-04-07 09:58:09.846657 orwynn-1.0.0b4/orwynn/base/error/_errcode.py
--rw-r--r--   0        0        0     1777 2023-02-20 12:03:03.462649 orwynn-1.0.0b4/orwynn/base/error/_find_detailed_class_for_exception.py
--rw-r--r--   0        0        0      227 2023-03-06 11:29:02.964195 orwynn-1.0.0b4/orwynn/base/error/_get_exception_direct_subclasses.py
--rw-r--r--   0        0        0      871 2023-04-07 09:57:35.360451 orwynn-1.0.0b4/orwynn/base/error/errcode_test.py
--rw-r--r--   0        0        0      340 2023-03-06 11:30:55.547595 orwynn-1.0.0b4/orwynn/base/error/error_test.py
--rw-r--r--   0        0        0      465 2023-03-06 11:30:05.054864 orwynn-1.0.0b4/orwynn/base/error/find_detailed_class_test.py
--rw-r--r--   0        0        0     2381 2023-05-22 08:32:39.088446 orwynn-1.0.0b4/orwynn/base/errorhandler/_ErrorHandler.py
--rw-r--r--   0        0        0       40 2023-03-06 12:10:21.521111 orwynn-1.0.0b4/orwynn/base/errorhandler/__init__.py
--rw-r--r--   0        0        0       95 2023-02-27 07:44:23.453495 orwynn-1.0.0b4/orwynn/base/middleware/_GlobalMiddlewareSetup.py
--rw-r--r--   0        0        0     2919 2023-04-21 09:59:20.018394 orwynn-1.0.0b4/orwynn/base/middleware/_Middleware.py
--rw-r--r--   0        0        0       94 2023-02-27 09:39:25.885954 orwynn-1.0.0b4/orwynn/base/middleware/__init__.py
--rw-r--r--   0        0        0     1188 2023-04-03 14:59:49.566980 orwynn-1.0.0b4/orwynn/base/middleware/global_middleware_test.py
--rw-r--r--   0        0        0     1437 2023-04-03 14:59:49.469979 orwynn-1.0.0b4/orwynn/base/model/_Model.py
--rw-r--r--   0        0        0       26 2023-02-27 07:44:01.168434 orwynn-1.0.0b4/orwynn/base/model/__init__.py
--rw-r--r--   0        0        0      805 2023-02-28 05:48:16.658066 orwynn-1.0.0b4/orwynn/base/model/model_test.py
--rw-r--r--   0        0        0     7191 2023-04-03 14:59:49.092978 orwynn-1.0.0b4/orwynn/base/module/_Module.py
--rw-r--r--   0        0        0       28 2023-02-27 08:27:08.818056 orwynn-1.0.0b4/orwynn/base/module/__init__.py
--rw-r--r--   0        0        0      308 2023-04-03 14:39:07.523996 orwynn-1.0.0b4/orwynn/base/module/errors.py
--rw-r--r--   0        0        0      951 2023-04-03 14:59:49.134978 orwynn-1.0.0b4/orwynn/base/module/module_test.py
--rw-r--r--   0        0        0      397 2023-02-27 07:44:37.638169 orwynn-1.0.0b4/orwynn/base/service/_FrameworkService.py
--rw-r--r--   0        0        0      286 2023-01-10 09:51:48.349126 orwynn-1.0.0b4/orwynn/base/service/_Service.py
--rw-r--r--   0        0        0       78 2023-02-28 05:48:16.655065 orwynn-1.0.0b4/orwynn/base/service/__init__.py
--rw-r--r--   0        0        0      213 2023-02-27 08:21:58.741307 orwynn-1.0.0b4/orwynn/base/worker/_Worker.py
--rw-r--r--   0        0        0       28 2023-02-27 08:22:18.356515 orwynn-1.0.0b4/orwynn/base/worker/__init__.py
--rw-r--r--   0        0        0    10694 2023-05-22 08:56:00.400479 orwynn-1.0.0b4/orwynn/boot/_Boot.py
--rw-r--r--   0        0        0      723 2023-02-28 05:48:16.655065 orwynn-1.0.0b4/orwynn/boot/_BootConfig.py
--rw-r--r--   0        0        0       50 2023-03-06 11:23:49.055894 orwynn-1.0.0b4/orwynn/boot/_UnknownBootModeError.py
--rw-r--r--   0        0        0       49 2023-03-06 11:23:49.055894 orwynn-1.0.0b4/orwynn/boot/_UnknownSourceError.py
--rw-r--r--   0        0        0       60 2023-02-27 12:41:46.281489 orwynn-1.0.0b4/orwynn/boot/__init__.py
--rw-r--r--   0        0        0     4765 2023-04-07 09:56:47.709126 orwynn-1.0.0b4/orwynn/boot/boot_test.py
--rw-r--r--   0        0        0      232 2023-03-06 14:58:11.414882 orwynn-1.0.0b4/orwynn/bootscript/_Bootscript.py
--rw-r--r--   0        0        0       70 2023-03-06 14:58:11.412882 orwynn-1.0.0b4/orwynn/bootscript/_BootscriptCallable.py
--rw-r--r--   0        0        0     2309 2023-03-07 08:22:34.928871 orwynn-1.0.0b4/orwynn/bootscript/_BootscriptWorker.py
--rw-r--r--   0        0        0      240 2023-03-06 13:38:38.458249 orwynn-1.0.0b4/orwynn/bootscript/_CallTime.py
--rw-r--r--   0        0        0      167 2023-03-06 14:58:11.415882 orwynn-1.0.0b4/orwynn/bootscript/__init__.py
--rw-r--r--   0        0        0      863 2023-04-03 14:59:49.716980 orwynn-1.0.0b4/orwynn/bootscript/bootscript_test.py
--rw-r--r--   0        0        0      220 2023-03-06 14:11:14.410261 orwynn-1.0.0b4/orwynn/bootscript/errors.py
--rw-r--r--   0        0        0     2657 2023-04-03 14:59:49.734980 orwynn-1.0.0b4/orwynn/context/_ContextStorage.py
--rw-r--r--   0        0        0       90 2023-02-27 06:44:46.522437 orwynn-1.0.0b4/orwynn/context/__init__.py
--rw-r--r--   0        0        0      651 2023-04-03 14:59:49.734980 orwynn-1.0.0b4/orwynn/context/_context_manager.py
--rw-r--r--   0        0        0      318 2023-03-06 11:23:49.055894 orwynn-1.0.0b4/orwynn/context/errors.py
--rw-r--r--   0        0        0      197 2023-05-22 08:56:00.400479 orwynn-1.0.0b4/orwynn/helpers/ENVIRONS.py
--rw-r--r--   0        0        0      683 2023-04-03 14:59:49.716980 orwynn-1.0.0b4/orwynn/helpers/SUBCLASSABLES.py
--rw-r--r--   0        0        0     1140 2023-04-03 15:28:01.351294 orwynn-1.0.0b4/orwynn/helpers/web.py
--rw-r--r--   0        0        0      581 2023-03-06 12:13:17.936738 orwynn-1.0.0b4/orwynn/http/_BUILTIN_HTTP_MIDDLEWARE.py
--rw-r--r--   0        0        0      392 2023-05-15 09:41:13.740171 orwynn-1.0.0b4/orwynn/http/_DEFAULT_HTTP_ERROR_HANDLERS.py
--rw-r--r--   0        0        0     1288 2023-05-22 08:13:58.524603 orwynn-1.0.0b4/orwynn/http/__init__.py
--rw-r--r--   0        0        0      638 2023-02-27 13:18:48.601279 orwynn-1.0.0b4/orwynn/http/_context/ContextBuiltinMiddleware.py
--rw-r--r--   0        0        0      785 2023-04-21 10:02:27.264870 orwynn-1.0.0b4/orwynn/http/_context/HttpRequestContextBuiltinMiddleware.py
--rw-r--r--   0        0        0      959 2023-04-03 14:59:49.717980 orwynn-1.0.0b4/orwynn/http/_context/HttpRequestContextId.py
--rw-r--r--   0        0        0      986 2023-04-03 14:59:49.717980 orwynn-1.0.0b4/orwynn/http/_context/context_test.py
--rw-r--r--   0        0        0     5455 2023-04-03 15:31:36.939282 orwynn-1.0.0b4/orwynn/http/_controller/HttpController.py
--rw-r--r--   0        0        0     1239 2023-02-28 05:48:16.650064 orwynn-1.0.0b4/orwynn/http/_controller/endpoint/Endpoint.py
--rw-r--r--   0        0        0     1130 2023-04-03 14:59:49.717980 orwynn-1.0.0b4/orwynn/http/_controller/endpoint/EndpointContainer.py
--rw-r--r--   0        0        0      217 2023-05-15 09:51:42.051574 orwynn-1.0.0b4/orwynn/http/_controller/endpoint/EndpointResponse.py
--rw-r--r--   0        0        0     2234 2023-04-03 14:59:49.717980 orwynn-1.0.0b4/orwynn/http/_controller/endpoint/endpoint_test.py
--rw-r--r--   0        0        0       64 2023-03-06 11:23:49.055894 orwynn-1.0.0b4/orwynn/http/_controller/errors.py
--rw-r--r--   0        0        0     7269 2023-04-21 10:06:19.025210 orwynn-1.0.0b4/orwynn/http/_controller/http_controller_test.py
--rw-r--r--   0        0        0      408 2023-02-27 07:44:23.427494 orwynn-1.0.0b4/orwynn/http/_cors/Cors.py
--rw-r--r--   0        0        0     1926 2023-02-28 05:48:16.656065 orwynn-1.0.0b4/orwynn/http/_cors/cors_test.py
--rw-r--r--   0        0        0     1107 2023-04-21 09:55:44.471980 orwynn-1.0.0b4/orwynn/http/_errorhandler/ErrorHandlerHttpMiddleware.py
--rw-r--r--   0        0        0     1211 2023-05-22 08:13:58.518604 orwynn-1.0.0b4/orwynn/http/_errorhandler/default.py
--rw-r--r--   0        0        0     6159 2023-04-03 14:59:49.717980 orwynn-1.0.0b4/orwynn/http/_errorhandler/error_handler_test.py
--rw-r--r--   0        0        0     4527 2023-05-22 08:37:52.772943 orwynn-1.0.0b4/orwynn/http/_log/HttpLogger.py
--rw-r--r--   0        0        0     1181 2023-02-28 05:54:49.627064 orwynn-1.0.0b4/orwynn/http/_log/LogMiddleware.py
--rw-r--r--   0        0        0      279 2023-02-27 12:24:09.544983 orwynn-1.0.0b4/orwynn/http/_middleware/BuiltinHttpMiddleware.py
--rw-r--r--   0        0        0      659 2023-04-21 09:58:22.708552 orwynn-1.0.0b4/orwynn/http/_middleware/HttpMiddleware.py
--rw-r--r--   0        0        0      329 2023-02-27 12:23:41.962432 orwynn-1.0.0b4/orwynn/http/_middleware/HttpNextCall.py
--rw-r--r--   0        0        0     2153 2023-02-28 05:48:16.654065 orwynn-1.0.0b4/orwynn/http/_middleware/http_middleware_test.py
--rw-r--r--   0        0        0       76 2023-02-21 09:41:40.933060 orwynn-1.0.0b4/orwynn/http/_requests.py
--rw-r--r--   0        0        0      577 2023-05-22 07:24:03.129227 orwynn-1.0.0b4/orwynn/http/_responses.py
--rw-r--r--   0        0        0      120 2023-03-06 11:39:26.483900 orwynn-1.0.0b4/orwynn/http/_schema/HttpExceptionValueSchema.py
--rw-r--r--   0        0        0      149 2023-03-06 11:39:39.812830 orwynn-1.0.0b4/orwynn/http/_schema/RequestValidationExceptionValueSchema.py
--rw-r--r--   0        0        0      220 2023-03-06 11:30:55.550595 orwynn-1.0.0b4/orwynn/http/errors.py
--rw-r--r--   0        0        0      878 2023-05-22 08:37:12.679129 orwynn-1.0.0b4/orwynn/http/responses_test.py
--rw-r--r--   0        0        0      126 2023-02-27 07:08:40.302249 orwynn-1.0.0b4/orwynn/http/testing.py
--rw-r--r--   0        0        0      187 2023-03-06 11:37:56.740371 orwynn-1.0.0b4/orwynn/indication/_Indicatable.py
--rw-r--r--   0        0        0    11582 2023-05-15 09:44:55.514487 orwynn-1.0.0b4/orwynn/indication/_Indication.py
--rw-r--r--   0        0        0      491 2023-02-10 07:37:36.270095 orwynn-1.0.0b4/orwynn/indication/_IndicationType.py
--rw-r--r--   0        0        0      373 2023-02-10 07:31:06.809383 orwynn-1.0.0b4/orwynn/indication/_Indicator.py
--rw-r--r--   0        0        0      174 2023-02-28 05:48:16.652064 orwynn-1.0.0b4/orwynn/indication/__init__.py
--rw-r--r--   0        0        0      233 2023-02-27 08:17:22.419985 orwynn-1.0.0b4/orwynn/indication/_default_api_indication.py
--rw-r--r--   0        0        0      213 2023-03-06 11:23:49.055894 orwynn-1.0.0b4/orwynn/indication/errors.py
--rw-r--r--   0        0        0     3449 2023-05-15 09:48:05.804030 orwynn-1.0.0b4/orwynn/indication/indication_test.py
--rw-r--r--   0        0        0      114 2023-02-13 09:24:59.764293 orwynn-1.0.0b4/orwynn/log/_LOG_EXTRA_RESERVED_FIELDS.py
--rw-r--r--   0        0        0       35 2023-02-14 07:07:42.021607 orwynn-1.0.0b4/orwynn/log/_Log.py
--rw-r--r--   0        0        0      156 2023-02-27 09:57:55.608936 orwynn-1.0.0b4/orwynn/log/_LogConfig.py
--rw-r--r--   0        0        0      746 2023-02-27 07:44:23.427494 orwynn-1.0.0b4/orwynn/log/_LogHandler.py
--rw-r--r--   0        0        0      134 2023-02-27 08:12:14.243641 orwynn-1.0.0b4/orwynn/log/__init__.py
--rw-r--r--   0        0        0     1984 2023-02-27 12:51:28.284483 orwynn-1.0.0b4/orwynn/log/_configure_log.py
--rw-r--r--   0        0        0       99 2023-03-06 11:23:49.055894 orwynn-1.0.0b4/orwynn/log/errors.py
--rw-r--r--   0        0        0      541 2023-05-22 08:50:13.691363 orwynn-1.0.0b4/orwynn/log/helpers.py
--rw-r--r--   0        0        0     3688 2023-05-22 08:22:24.475022 orwynn-1.0.0b4/orwynn/log/log_middleware_test.py
--rw-r--r--   0        0        0     1779 2023-05-22 08:20:37.035811 orwynn-1.0.0b4/orwynn/log/log_test.py
--rw-r--r--   0        0        0     1460 2023-02-28 05:48:16.662067 orwynn-1.0.0b4/orwynn/log/log_websocket_middleware_test.py
--rw-r--r--   0        0        0     1560 2023-04-03 14:59:49.734980 orwynn-1.0.0b4/orwynn/mapping/_Mapping.py
--rw-r--r--   0        0        0       30 2023-02-27 08:33:14.996815 orwynn-1.0.0b4/orwynn/mapping/__init__.py
--rw-r--r--   0        0        0      281 2023-03-06 11:23:49.055894 orwynn-1.0.0b4/orwynn/mapping/errors.py
--rw-r--r--   0        0        0      179 2023-02-27 08:32:55.043879 orwynn-1.0.0b4/orwynn/mapping/mapping_test.py
--rw-r--r--   0        0        0      111 2022-12-25 22:05:28.493755 orwynn-1.0.0b4/orwynn/mongo/_ClientSession.py
--rw-r--r--   0        0        0     6048 2023-04-03 14:59:49.734980 orwynn-1.0.0b4/orwynn/mongo/_Document.py
--rw-r--r--   0        0        0     3579 2023-04-03 14:59:49.734980 orwynn-1.0.0b4/orwynn/mongo/_Mongo.py
--rw-r--r--   0        0        0      133 2023-02-27 09:58:10.560648 orwynn-1.0.0b4/orwynn/mongo/_MongoConfig.py
--rw-r--r--   0        0        0       19 2022-12-25 11:43:30.248664 orwynn-1.0.0b4/orwynn/mongo/_MongoEntity.py
--rw-r--r--   0        0        0      224 2023-02-28 05:48:16.650064 orwynn-1.0.0b4/orwynn/mongo/__init__.py
--rw-r--r--   0        0        0     3300 2023-04-03 14:59:49.734980 orwynn-1.0.0b4/orwynn/mongo/document_test.py
--rw-r--r--   0        0        0      445 2023-03-06 11:30:55.548595 orwynn-1.0.0b4/orwynn/mongo/errors.py
--rw-r--r--   0        0        0     1361 2023-04-03 14:59:49.734980 orwynn-1.0.0b4/orwynn/mongo/mongo_test.py
--rw-r--r--   0        0        0      310 2023-03-07 08:22:29.576929 orwynn-1.0.0b4/orwynn/proxy/ApiIndicationOnlyProxy.py
--rw-r--r--   0        0        0     2841 2023-05-15 10:17:07.786310 orwynn-1.0.0b4/orwynn/proxy/BootProxy.py
--rw-r--r--   0        0        0    14266 2023-05-15 09:53:21.180789 orwynn-1.0.0b4/orwynn/router/_ControllerRegister.py
--rw-r--r--   0        0        0     3952 2023-04-03 14:59:49.711980 orwynn-1.0.0b4/orwynn/router/_ErrorHandlerManager.py
--rw-r--r--   0        0        0    10362 2023-05-22 08:08:57.588603 orwynn-1.0.0b4/orwynn/router/_MiddlewareRegister.py
--rw-r--r--   0        0        0     2697 2023-03-07 08:22:34.931871 orwynn-1.0.0b4/orwynn/router/_Router.py
--rw-r--r--   0        0        0       28 2023-02-27 13:24:49.469241 orwynn-1.0.0b4/orwynn/router/__init__.py
--rw-r--r--   0        0        0      116 2023-03-06 11:23:49.055894 orwynn-1.0.0b4/orwynn/router/errors.py
--rw-r--r--   0        0        0     2465 2023-02-28 05:48:16.660066 orwynn-1.0.0b4/orwynn/router/global_http_route_test.py
--rw-r--r--   0        0        0     1306 2023-01-10 10:10:51.782079 orwynn-1.0.0b4/orwynn/singleton/_Singleton.py
--rw-r--r--   0        0        0       34 2023-02-27 08:21:14.680585 orwynn-1.0.0b4/orwynn/singleton/__init__.py
--rw-r--r--   0        0        0       65 2023-02-28 06:53:56.326285 orwynn-1.0.0b4/orwynn/sql/_PoolclassStr.py
--rw-r--r--   0        0        0     3888 2023-05-15 09:39:14.553897 orwynn-1.0.0b4/orwynn/sql/_Sql.py
--rw-r--r--   0        0        0     1972 2023-05-15 09:35:55.577896 orwynn-1.0.0b4/orwynn/sql/_SqlConfig.py
--rw-r--r--   0        0        0      105 2023-01-19 15:20:28.442785 orwynn-1.0.0b4/orwynn/sql/_SqlDatabaseKind.py
--rw-r--r--   0        0        0     2636 2023-05-22 08:54:47.949687 orwynn-1.0.0b4/orwynn/sql/_Table.py
--rw-r--r--   0        0        0      210 2023-02-28 05:15:28.490194 orwynn-1.0.0b4/orwynn/sql/__init__.py
--rw-r--r--   0        0        0     5865 2023-04-03 14:59:49.751980 orwynn-1.0.0b4/orwynn/sql/sql_test.py
--rw-r--r--   0        0        0    11258 2023-04-03 14:59:49.717980 orwynn-1.0.0b4/orwynn/testing/_Client.py
--rw-r--r--   0        0        0      101 2022-12-29 09:50:50.883906 orwynn-1.0.0b4/orwynn/testing/_EmbeddedTestClient.py
--rw-r--r--   0        0        0      727 2023-02-28 05:48:16.655065 orwynn-1.0.0b4/orwynn/testing/__init__.py
--rw-r--r--   0        0        0     2049 2023-05-22 07:37:27.975231 orwynn-1.0.0b4/orwynn/testing/client_test.py
--rw-r--r--   0        0        0       24 2022-12-22 07:52:56.312366 orwynn-1.0.0b4/orwynn/utils/BaseSubclassable.py
--rw-r--r--   0        0        0      133 2023-02-17 07:27:38.315341 orwynn-1.0.0b4/orwynn/utils/Protocol.py
--rw-r--r--   0        0        0      866 2023-04-03 14:59:49.716980 orwynn-1.0.0b4/orwynn/utils/crypto/__init__.py
--rw-r--r--   0        0        0      448 2023-04-03 14:59:49.716980 orwynn-1.0.0b4/orwynn/utils/dt/__init__.py
--rw-r--r--   0        0        0     1746 2023-02-23 07:22:44.852890 orwynn-1.0.0b4/orwynn/utils/fmt/__init__.py
--rw-r--r--   0        0        0     1312 2023-04-03 14:59:49.716980 orwynn-1.0.0b4/orwynn/utils/fmt/fmt_test.py
--rw-r--r--   0        0        0     1974 2023-04-03 14:59:49.716980 orwynn-1.0.0b4/orwynn/utils/klass/__init__.py
--rw-r--r--   0        0        0       46 2023-03-07 05:33:50.925367 orwynn-1.0.0b4/orwynn/utils/klass/_errors.py
--rw-r--r--   0        0        0      522 2023-04-07 10:26:52.657368 orwynn-1.0.0b4/orwynn/utils/klass/klass_test.py
--rw-r--r--   0        0        0     2545 2023-04-03 14:59:49.716980 orwynn-1.0.0b4/orwynn/utils/mp/__init__.py
--rw-r--r--   0        0        0       98 2023-01-11 10:48:59.268124 orwynn-1.0.0b4/orwynn/utils/mp/_dictpp.py
--rw-r--r--   0        0        0     2448 2023-03-06 11:30:55.553595 orwynn-1.0.0b4/orwynn/utils/mp/location.py
--rw-r--r--   0        0        0     1738 2023-04-03 14:59:49.716980 orwynn-1.0.0b4/orwynn/utils/mp/mp_test.py
--rw-r--r--   0        0        0      131 2023-02-21 10:53:24.615257 orwynn-1.0.0b4/orwynn/utils/rnd/__init__.py
--rw-r--r--   0        0        0       90 2023-04-03 14:59:49.716980 orwynn-1.0.0b4/orwynn/utils/rnd/rnd_test.py
--rw-r--r--   0        0        0      176 2023-02-17 07:26:21.447070 orwynn-1.0.0b4/orwynn/utils/types.py
--rw-r--r--   0        0        0      307 2023-03-07 05:31:01.650091 orwynn-1.0.0b4/orwynn/utils/uio.py
--rw-r--r--   0        0        0       79 2023-02-22 12:14:57.519901 orwynn-1.0.0b4/orwynn/utils/url/_Url.py
--rw-r--r--   0        0        0      254 2023-04-03 14:59:49.716980 orwynn-1.0.0b4/orwynn/utils/url/_UrlVars.py
--rw-r--r--   0        0        0      697 2023-04-03 14:59:49.716980 orwynn-1.0.0b4/orwynn/utils/url/__init__.py
--rw-r--r--   0        0        0     1934 2023-04-03 14:59:49.716980 orwynn-1.0.0b4/orwynn/utils/url/_get_vars.py
--rw-r--r--   0        0        0      419 2023-03-06 13:33:43.023337 orwynn-1.0.0b4/orwynn/utils/url/_match_routes.py
--rw-r--r--   0        0        0     1412 2023-04-03 14:59:49.716980 orwynn-1.0.0b4/orwynn/utils/url/get_vars_test.py
--rw-r--r--   0        0        0     9151 2023-04-03 15:00:11.231062 orwynn-1.0.0b4/orwynn/utils/validation/__init__.py
--rw-r--r--   0        0        0      216 2022-12-16 11:42:54.126673 orwynn-1.0.0b4/orwynn/utils/validation/_validator.py
--rw-r--r--   0        0        0     1796 2023-03-07 05:27:06.425420 orwynn-1.0.0b4/orwynn/utils/validation/errors.py
--rw-r--r--   0        0        0     1743 2023-04-03 14:59:49.716980 orwynn-1.0.0b4/orwynn/utils/yml/__init__.py
--rw-r--r--   0        0        0       42 2023-03-06 11:23:49.055894 orwynn-1.0.0b4/orwynn/utils/yml/errors.py
--rw-r--r--   0        0        0      864 2023-03-06 12:13:17.936738 orwynn-1.0.0b4/orwynn/websocket/_BUILTIN_WEBSOCKET_MIDDLEWARE.py
--rw-r--r--   0        0        0      248 2023-03-06 12:13:17.936738 orwynn-1.0.0b4/orwynn/websocket/_DEFAULT_WEBSOCKET_ERROR_HANDLERS.py
--rw-r--r--   0        0        0       82 2022-12-25 23:39:24.206537 orwynn-1.0.0b4/orwynn/websocket/_Websocket.py
--rw-r--r--   0        0        0      836 2023-03-06 12:13:17.936738 orwynn-1.0.0b4/orwynn/websocket/__init__.py
--rw-r--r--   0        0        0      579 2023-02-28 05:55:07.500801 orwynn-1.0.0b4/orwynn/websocket/_context/ContextBuiltinWebsocketMiddleware.py
--rw-r--r--   0        0        0      824 2023-02-28 05:48:16.654065 orwynn-1.0.0b4/orwynn/websocket/_context/RequestContextBuiltinWebsocketMiddleware.py
--rw-r--r--   0        0        0     1028 2023-04-03 14:59:49.717980 orwynn-1.0.0b4/orwynn/websocket/_context/WebsocketRequestContextId.py
--rw-r--r--   0        0        0     1291 2023-04-03 14:59:49.717980 orwynn-1.0.0b4/orwynn/websocket/_context/websocket_context_test.py
--rw-r--r--   0        0        0     3977 2023-04-07 10:11:54.671319 orwynn-1.0.0b4/orwynn/websocket/_controller/WebsocketController.py
--rw-r--r--   0        0        0      902 2023-04-07 10:21:27.442702 orwynn-1.0.0b4/orwynn/websocket/_controller/WebsocketController_test.py
--rw-r--r--   0        0        0      147 2023-02-27 07:44:23.427494 orwynn-1.0.0b4/orwynn/websocket/_controller/WebsocketEventHandlerMethod.py
--rw-r--r--   0        0        0     2900 2023-02-28 05:48:16.658066 orwynn-1.0.0b4/orwynn/websocket/_controller/global_websocket_route_test.py
--rw-r--r--   0        0        0     3026 2023-03-06 13:33:04.085558 orwynn-1.0.0b4/orwynn/websocket/_controller/websocket_controller_test.py
--rw-r--r--   0        0        0      417 2023-03-06 12:12:57.645660 orwynn-1.0.0b4/orwynn/websocket/_errorhandler/DefaultWebsocketErrorHandler.py
--rw-r--r--   0        0        0     3620 2023-04-03 14:59:49.717980 orwynn-1.0.0b4/orwynn/websocket/_errorhandler/ErrorHandlerWebsocketMiddleware.py
--rw-r--r--   0        0        0     1707 2023-04-03 14:59:49.717980 orwynn-1.0.0b4/orwynn/websocket/_errorhandler/error_handler_websocket_test.py
--rw-r--r--   0        0        0      920 2023-02-28 05:48:16.653065 orwynn-1.0.0b4/orwynn/websocket/_log/LogWebsocketMiddleware.py
--rw-r--r--   0        0        0     1708 2023-04-03 14:59:49.717980 orwynn-1.0.0b4/orwynn/websocket/_log/WebsocketLogger.py
--rw-r--r--   0        0        0      313 2023-02-28 05:48:16.648064 orwynn-1.0.0b4/orwynn/websocket/_middleware/BuiltinWebsocketMiddleware.py
--rw-r--r--   0        0        0      887 2023-02-28 05:48:16.653065 orwynn-1.0.0b4/orwynn/websocket/_middleware/ConnectionBuiltinWebsocketMiddleware.py
--rw-r--r--   0        0        0      748 2023-02-28 05:48:16.653065 orwynn-1.0.0b4/orwynn/websocket/_middleware/WebsocketMiddleware.py
--rw-r--r--   0        0        0      280 2023-02-27 13:14:10.637743 orwynn-1.0.0b4/orwynn/websocket/_middleware/WebsocketNextCall.py
--rw-r--r--   0        0        0     1056 2023-02-28 05:48:16.647063 orwynn-1.0.0b4/orwynn/websocket/_middleware/websocket_middleware_test.py
--rw-r--r--   0        0        0     1893 2023-04-03 14:59:49.717980 orwynn-1.0.0b4/orwynn/websocket/_routing/NextCallHandler.py
--rw-r--r--   0        0        0     6084 2023-04-03 14:59:49.717980 orwynn-1.0.0b4/orwynn/websocket/_routing/WebsocketStack.py
--rw-r--r--   0        0        0      231 2023-02-28 05:55:25.292122 orwynn-1.0.0b4/orwynn/websocket/_routing/_DispatchWebsocketFn.py
--rw-r--r--   0        0        0       92 2023-02-15 09:24:37.556326 orwynn-1.0.0b4/orwynn/websocket/_routing/_GenericWebsocketFn.py
--rw-r--r--   0        0        0     5547 2023-04-03 14:59:49.717980 orwynn-1.0.0b4/orwynn/websocket/_routing/_get_handler_kwargs.py
--rw-r--r--   0        0        0      448 2023-02-28 05:48:16.646063 orwynn-1.0.0b4/orwynn/websocket/_routing/handlers.py
--rw-r--r--   0        0        0      823 2023-05-22 09:00:24.425657 orwynn-1.0.0b4/pyproject.toml
--rw-r--r--   0        0        0     2650 1970-01-01 00:00:00.000000 orwynn-1.0.0b4/setup.py
--rw-r--r--   0        0        0     1280 1970-01-01 00:00:00.000000 orwynn-1.0.0b4/PKG-INFO
+-rw-r--r--   0        0        0     1072 2022-12-08 10:08:41.917165 orwynn-1.0.0b5/LICENSE
+-rw-r--r--   0        0        0      307 2023-05-22 08:29:05.173562 orwynn-1.0.0b5/README.md
+-rw-r--r--   0        0        0       65 2023-03-07 08:24:06.640906 orwynn-1.0.0b5/orwynn/__init__.py
+-rw-r--r--   0        0        0     1920 2023-06-08 13:46:47.770769 orwynn-1.0.0b5/orwynn/apiversion/__init__.py
+-rw-r--r--   0        0        0       54 2023-03-06 11:23:49.055894 orwynn-1.0.0b5/orwynn/apiversion/errors.py
+-rw-r--r--   0        0        0     4546 2023-06-09 12:16:54.007732 orwynn-1.0.0b5/orwynn/apiversion/test_main.py
+-rw-r--r--   0        0        0       77 2023-06-08 13:47:49.293428 orwynn-1.0.0b5/orwynn/app/__init__.py
+-rw-r--r--   0        0        0      400 2023-06-08 13:48:58.389784 orwynn-1.0.0b5/orwynn/app/apirouter.py
+-rw-r--r--   0        0        0     1484 2023-06-08 13:47:28.661538 orwynn-1.0.0b5/orwynn/app/apiwebsocketroute.py
+-rw-r--r--   0        0        0     2594 2023-06-09 12:20:44.292995 orwynn-1.0.0b5/orwynn/app/app.py
+-rw-r--r--   0        0        0      188 2023-06-09 10:55:27.417944 orwynn-1.0.0b5/orwynn/app/config.py
+-rw-r--r--   0        0        0     1560 2023-06-08 13:47:12.703403 orwynn-1.0.0b5/orwynn/app/core.py
+-rw-r--r--   0        0        0       97 2023-02-27 12:42:05.392452 orwynn-1.0.0b5/orwynn/app/mode.py
+-rw-r--r--   0        0        0     2206 2023-06-08 13:47:49.295428 orwynn-1.0.0b5/orwynn/app/test_main.py
+-rw-r--r--   0        0        0       98 2023-06-09 11:05:03.703488 orwynn-1.0.0b5/orwynn/app/types.py
+-rw-r--r--   0        0        0     2885 2023-03-07 07:26:27.308262 orwynn-1.0.0b5/orwynn/app/utils.py
+-rw-r--r--   0        0        0       56 2023-06-08 13:49:42.996486 orwynn-1.0.0b5/orwynn/apprc/__init__.py
+-rw-r--r--   0        0        0       13 2023-02-27 06:15:50.756268 orwynn-1.0.0b5/orwynn/apprc/apprc.py
+-rw-r--r--   0        0        0      190 2023-02-27 12:42:54.819951 orwynn-1.0.0b5/orwynn/apprc/constants.py
+-rw-r--r--   0        0        0       47 2023-03-06 11:23:49.055894 orwynn-1.0.0b5/orwynn/apprc/errors.py
+-rw-r--r--   0        0        0     3493 2023-06-08 13:49:43.002486 orwynn-1.0.0b5/orwynn/apprc/parse.py
+-rw-r--r--   0        0        0     2604 2023-06-09 06:20:20.107768 orwynn-1.0.0b5/orwynn/apprc/test_main.py
+-rw-r--r--   0        0        0      374 2023-03-07 08:25:49.974896 orwynn-1.0.0b5/orwynn/base/__init__.py
+-rw-r--r--   0        0        0       27 2023-06-08 13:49:50.224117 orwynn-1.0.0b5/orwynn/base/config/__init__.py
+-rw-r--r--   0        0        0     1109 2023-06-09 05:54:54.979178 orwynn-1.0.0b5/orwynn/base/config/config.py
+-rw-r--r--   0        0        0        0 2022-12-18 22:39:38.591866 orwynn-1.0.0b5/orwynn/base/config/test_config.py
+-rw-r--r--   0        0        0       35 2023-06-08 13:50:00.474596 orwynn-1.0.0b5/orwynn/base/controller/__init__.py
+-rw-r--r--   0        0        0     2201 2023-04-07 10:26:00.405258 orwynn-1.0.0b5/orwynn/base/controller/controller.py
+-rw-r--r--   0        0        0      179 2023-03-06 11:23:49.043895 orwynn-1.0.0b5/orwynn/base/controller/errors.py
+-rw-r--r--   0        0        0       31 2023-06-08 13:50:07.129259 orwynn-1.0.0b5/orwynn/base/database/__init__.py
+-rw-r--r--   0        0        0      629 2023-06-08 13:55:40.340226 orwynn-1.0.0b5/orwynn/base/database/database.py
+-rw-r--r--   0        0        0      528 2023-03-06 11:23:49.038895 orwynn-1.0.0b5/orwynn/base/database/errors.py
+-rw-r--r--   0        0        0      203 2023-06-09 06:20:20.113767 orwynn-1.0.0b5/orwynn/base/error/__init__.py
+-rw-r--r--   0        0        0     1009 2023-04-07 09:58:09.846657 orwynn-1.0.0b5/orwynn/base/error/code.py
+-rw-r--r--   0        0        0      284 2023-06-08 13:54:00.170896 orwynn-1.0.0b5/orwynn/base/error/errors.py
+-rw-r--r--   0        0        0     1204 2023-06-09 06:20:20.112767 orwynn-1.0.0b5/orwynn/base/error/test_main.py
+-rw-r--r--   0        0        0      436 2023-06-08 13:50:50.520080 orwynn-1.0.0b5/orwynn/base/error/test_utils.py
+-rw-r--r--   0        0        0     2006 2023-06-08 13:54:17.686071 orwynn-1.0.0b5/orwynn/base/error/utils.py
+-rw-r--r--   0        0        0       86 2023-03-06 11:24:23.455706 orwynn-1.0.0b5/orwynn/base/error/valueschema.py
+-rw-r--r--   0        0        0       39 2023-06-08 13:54:42.338917 orwynn-1.0.0b5/orwynn/base/errorhandler/__init__.py
+-rw-r--r--   0        0        0     2365 2023-06-09 06:03:10.090856 orwynn-1.0.0b5/orwynn/base/errorhandler/errorhandler.py
+-rw-r--r--   0        0        0       82 2023-06-08 13:55:03.438934 orwynn-1.0.0b5/orwynn/base/middleware/__init__.py
+-rw-r--r--   0        0        0       94 2023-06-08 13:55:03.438934 orwynn-1.0.0b5/orwynn/base/middleware/globalsetup.py
+-rw-r--r--   0        0        0     2919 2023-04-21 09:59:20.018394 orwynn-1.0.0b5/orwynn/base/middleware/middleware.py
+-rw-r--r--   0        0        0     1186 2023-06-09 06:20:20.112767 orwynn-1.0.0b5/orwynn/base/middleware/test_main.py
+-rw-r--r--   0        0        0       25 2023-06-08 13:55:11.806546 orwynn-1.0.0b5/orwynn/base/model/__init__.py
+-rw-r--r--   0        0        0     1429 2023-06-09 05:54:50.487357 orwynn-1.0.0b5/orwynn/base/model/model.py
+-rw-r--r--   0        0        0      791 2023-06-09 06:20:20.110767 orwynn-1.0.0b5/orwynn/base/model/test_model.py
+-rw-r--r--   0        0        0       27 2023-06-08 13:55:21.285106 orwynn-1.0.0b5/orwynn/base/module/__init__.py
+-rw-r--r--   0        0        0      308 2023-04-03 14:39:07.523996 orwynn-1.0.0b5/orwynn/base/module/errors.py
+-rw-r--r--   0        0        0     7183 2023-06-08 13:55:37.034379 orwynn-1.0.0b5/orwynn/base/module/module.py
+-rw-r--r--   0        0        0      950 2023-06-08 13:55:21.291106 orwynn-1.0.0b5/orwynn/base/module/test_module.py
+-rw-r--r--   0        0        0       69 2023-06-08 13:55:40.340226 orwynn-1.0.0b5/orwynn/base/service/__init__.py
+-rw-r--r--   0        0        0      396 2023-06-08 13:55:40.342226 orwynn-1.0.0b5/orwynn/base/service/framework.py
+-rw-r--r--   0        0        0      286 2023-01-10 09:51:48.349126 orwynn-1.0.0b5/orwynn/base/service/service.py
+-rw-r--r--   0        0        0       27 2023-06-08 13:55:46.418946 orwynn-1.0.0b5/orwynn/base/worker/__init__.py
+-rw-r--r--   0        0        0      212 2023-06-09 05:57:10.064779 orwynn-1.0.0b5/orwynn/base/worker/worker.py
+-rw-r--r--   0        0        0       54 2023-06-08 13:56:30.127942 orwynn-1.0.0b5/orwynn/boot/__init__.py
+-rw-r--r--   0        0        0    10355 2023-06-09 12:09:03.948090 orwynn-1.0.0b5/orwynn/boot/boot.py
+-rw-r--r--   0        0        0      716 2023-06-09 05:54:54.987177 orwynn-1.0.0b5/orwynn/boot/config.py
+-rw-r--r--   0        0        0       95 2023-06-08 13:58:33.909354 orwynn-1.0.0b5/orwynn/boot/errors.py
+-rw-r--r--   0        0        0     4754 2023-06-09 06:27:59.920644 orwynn-1.0.0b5/orwynn/boot/test_main.py
+-rw-r--r--   0        0        0      154 2023-06-09 06:20:20.102768 orwynn-1.0.0b5/orwynn/bootscript/__init__.py
+-rw-r--r--   0        0        0      220 2023-06-08 13:59:21.194248 orwynn-1.0.0b5/orwynn/bootscript/bootscript.py
+-rw-r--r--   0        0        0       70 2023-03-06 14:58:11.412882 orwynn-1.0.0b5/orwynn/bootscript/callable.py
+-rw-r--r--   0        0        0      240 2023-03-06 13:38:38.458249 orwynn-1.0.0b5/orwynn/bootscript/calltime.py
+-rw-r--r--   0        0        0      220 2023-03-06 14:11:14.410261 orwynn-1.0.0b5/orwynn/bootscript/errors.py
+-rw-r--r--   0        0        0      860 2023-06-09 06:20:20.107768 orwynn-1.0.0b5/orwynn/bootscript/test_main.py
+-rw-r--r--   0        0        0     2300 2023-06-09 06:20:20.107768 orwynn-1.0.0b5/orwynn/bootscript/worker.py
+-rw-r--r--   0        0        0       73 2023-06-08 13:59:41.390353 orwynn-1.0.0b5/orwynn/context/__init__.py
+-rw-r--r--   0        0        0      318 2023-03-06 11:23:49.055894 orwynn-1.0.0b5/orwynn/context/errors.py
+-rw-r--r--   0        0        0      643 2023-06-08 13:59:41.391353 orwynn-1.0.0b5/orwynn/context/manager.py
+-rw-r--r--   0        0        0     2656 2023-06-08 13:55:46.418946 orwynn-1.0.0b5/orwynn/context/storage.py
+-rw-r--r--   0        0        0       97 2023-06-08 14:06:22.928960 orwynn-1.0.0b5/orwynn/di/__init__.py
+-rw-r--r--   0        0        0       63 2022-12-11 09:09:39.933971 orwynn-1.0.0b5/orwynn/di/acceptor.py
+-rw-r--r--   0        0        0     3780 2023-06-09 06:21:27.250456 orwynn-1.0.0b5/orwynn/di/availability.py
+-rw-r--r--   0        0        0     1719 2023-06-09 06:20:20.108768 orwynn-1.0.0b5/orwynn/di/collecting/acceptordependencies.py
+-rw-r--r--   0        0        0     1219 2023-06-08 14:24:49.757165 orwynn-1.0.0b5/orwynn/di/collecting/errors.py
+-rw-r--r--   0        0        0     3128 2023-06-09 06:20:20.113767 orwynn-1.0.0b5/orwynn/di/collecting/helpers.py
+-rw-r--r--   0        0        0     3232 2023-04-03 14:59:49.701980 orwynn-1.0.0b5/orwynn/di/collecting/modulecollector.py
+-rw-r--r--   0        0        0        0 2023-06-09 06:31:34.417910 orwynn-1.0.0b5/orwynn/di/collecting/providerdependencies/__init__.py
+-rw-r--r--   0        0        0     3229 2023-06-09 06:20:20.111767 orwynn-1.0.0b5/orwynn/di/collecting/providerdependencies/collect.py
+-rw-r--r--   0        0        0     2341 2023-06-09 07:32:02.380043 orwynn-1.0.0b5/orwynn/di/collecting/providerdependencies/map.py
+-rw-r--r--   0        0        0     1765 2023-06-09 06:20:20.109768 orwynn-1.0.0b5/orwynn/di/collecting/providerdependencies/test_main.py
+-rw-r--r--   0        0        0     1084 2023-06-09 06:20:20.103768 orwynn-1.0.0b5/orwynn/di/collecting/test_modules.py
+-rw-r--r--   0        0        0      840 2023-06-08 14:24:49.775165 orwynn-1.0.0b5/orwynn/di/constants.py
+-rw-r--r--   0        0        0     5895 2023-06-09 07:32:02.385042 orwynn-1.0.0b5/orwynn/di/container.py
+-rw-r--r--   0        0        0     4694 2023-06-09 06:20:20.104768 orwynn-1.0.0b5/orwynn/di/di.py
+-rw-r--r--   0        0        0     1260 2023-06-08 14:25:37.475430 orwynn-1.0.0b5/orwynn/di/errors.py
+-rw-r--r--   0        0        0     6756 2023-06-09 06:20:20.110767 orwynn-1.0.0b5/orwynn/di/init/acceptors.py
+-rw-r--r--   0        0        0     4115 2023-06-09 06:22:50.702901 orwynn-1.0.0b5/orwynn/di/init/providers.py
+-rw-r--r--   0        0        0     2871 2023-06-09 06:20:20.106768 orwynn-1.0.0b5/orwynn/di/init/test_acceptors.py
+-rw-r--r--   0        0        0      615 2023-06-09 06:23:04.561666 orwynn-1.0.0b5/orwynn/di/init/test_providers.py
+-rw-r--r--   0        0        0      327 2023-06-08 14:06:45.172014 orwynn-1.0.0b5/orwynn/di/isacceptor.py
+-rw-r--r--   0        0        0      325 2023-06-08 14:09:24.648261 orwynn-1.0.0b5/orwynn/di/isprovider.py
+-rw-r--r--   0        0        0      140 2023-02-15 12:49:24.369340 orwynn-1.0.0b5/orwynn/di/object.py
+-rw-r--r--   0        0        0       39 2022-12-11 09:09:05.931124 orwynn-1.0.0b5/orwynn/di/provider.py
+-rw-r--r--   0        0        0      506 2023-06-09 06:20:20.105768 orwynn-1.0.0b5/orwynn/di/testing.py
+-rw-r--r--   0        0        0      877 2023-06-09 06:03:05.647671 orwynn-1.0.0b5/orwynn/helpers/constants.py
+-rw-r--r--   0        0        0     1140 2023-06-09 06:03:10.090856 orwynn-1.0.0b5/orwynn/helpers/web.py
+-rw-r--r--   0        0        0     1118 2023-06-09 06:20:20.105768 orwynn-1.0.0b5/orwynn/http/__init__.py
+-rw-r--r--   0        0        0      922 2023-06-09 06:20:20.109768 orwynn-1.0.0b5/orwynn/http/constants.py
+-rw-r--r--   0        0        0        0 2023-06-09 06:36:32.323279 orwynn-1.0.0b5/orwynn/http/context/__init__.py
+-rw-r--r--   0        0        0      959 2023-04-03 14:59:49.717980 orwynn-1.0.0b5/orwynn/http/context/id.py
+-rw-r--r--   0        0        0      617 2023-06-09 05:50:36.441513 orwynn-1.0.0b5/orwynn/http/context/middleware/builtin.py
+-rw-r--r--   0        0        0      754 2023-06-09 05:50:36.430513 orwynn-1.0.0b5/orwynn/http/context/middleware/contextbuiltin.py
+-rw-r--r--   0        0        0      984 2023-06-09 06:27:59.920644 orwynn-1.0.0b5/orwynn/http/context/test_main.py
+-rw-r--r--   0        0        0        0 2023-06-09 06:36:14.697646 orwynn-1.0.0b5/orwynn/http/controller/__init__.py
+-rw-r--r--   0        0        0     5446 2023-06-09 06:03:10.090856 orwynn-1.0.0b5/orwynn/http/controller/controller.py
+-rw-r--r--   0        0        0        0 2023-06-09 06:36:46.319189 orwynn-1.0.0b5/orwynn/http/controller/endpoint/__init__.py
+-rw-r--r--   0        0        0     1130 2023-06-09 05:49:31.580107 orwynn-1.0.0b5/orwynn/http/controller/endpoint/container.py
+-rw-r--r--   0        0        0     1231 2023-06-09 05:49:40.023769 orwynn-1.0.0b5/orwynn/http/controller/endpoint/endpoint.py
+-rw-r--r--   0        0        0      215 2023-06-09 05:51:12.418075 orwynn-1.0.0b5/orwynn/http/controller/endpoint/response.py
+-rw-r--r--   0        0        0     2231 2023-06-08 13:56:18.457476 orwynn-1.0.0b5/orwynn/http/controller/endpoint/test_main.py
+-rw-r--r--   0        0        0       64 2023-03-06 11:23:49.055894 orwynn-1.0.0b5/orwynn/http/controller/errors.py
+-rw-r--r--   0        0        0     7262 2023-06-09 06:20:20.111767 orwynn-1.0.0b5/orwynn/http/controller/test_main.py
+-rw-r--r--   0        0        0        0 2023-06-09 12:19:12.185278 orwynn-1.0.0b5/orwynn/http/cors/__init__.py
+-rw-r--r--   0        0        0      429 2023-06-09 11:03:10.108801 orwynn-1.0.0b5/orwynn/http/cors/cors.py
+-rw-r--r--   0        0        0     3491 2023-06-09 12:32:20.369783 orwynn-1.0.0b5/orwynn/http/cors/test_main.py
+-rw-r--r--   0        0        0        0 2023-06-09 06:37:51.749042 orwynn-1.0.0b5/orwynn/http/errorhandler/__init__.py
+-rw-r--r--   0        0        0     1204 2023-06-09 06:20:20.110767 orwynn-1.0.0b5/orwynn/http/errorhandler/default.py
+-rw-r--r--   0        0        0     1094 2023-06-09 05:50:36.426514 orwynn-1.0.0b5/orwynn/http/errorhandler/middleware.py
+-rw-r--r--   0        0        0     6129 2023-06-09 07:32:02.382043 orwynn-1.0.0b5/orwynn/http/errorhandler/test_main.py
+-rw-r--r--   0        0        0      220 2023-03-06 11:30:55.550595 orwynn-1.0.0b5/orwynn/http/errors.py
+-rw-r--r--   0        0        0     4525 2023-06-09 05:47:03.116046 orwynn-1.0.0b5/orwynn/http/log/logger.py
+-rw-r--r--   0        0        0     1145 2023-06-09 05:50:42.043289 orwynn-1.0.0b5/orwynn/http/log/middleware.py
+-rw-r--r--   0        0        0        0 2023-06-09 06:38:13.602306 orwynn-1.0.0b5/orwynn/http/middleware/__init__.py
+-rw-r--r--   0        0        0      274 2023-06-09 05:50:36.430513 orwynn-1.0.0b5/orwynn/http/middleware/builtinmiddleware.py
+-rw-r--r--   0        0        0      652 2023-06-09 05:50:36.430513 orwynn-1.0.0b5/orwynn/http/middleware/middleware.py
+-rw-r--r--   0        0        0      327 2023-06-09 05:47:03.114046 orwynn-1.0.0b5/orwynn/http/middleware/nextcall.py
+-rw-r--r--   0        0        0     2150 2023-06-09 06:00:41.008691 orwynn-1.0.0b5/orwynn/http/middleware/test_main.py
+-rw-r--r--   0        0        0       76 2023-02-21 09:41:40.933060 orwynn-1.0.0b5/orwynn/http/requests.py
+-rw-r--r--   0        0        0      577 2023-05-22 07:24:03.129227 orwynn-1.0.0b5/orwynn/http/responses.py
+-rw-r--r--   0        0        0      149 2023-03-06 11:39:39.812830 orwynn-1.0.0b5/orwynn/http/schema/validationvalue.py
+-rw-r--r--   0        0        0      120 2023-03-06 11:39:26.483900 orwynn-1.0.0b5/orwynn/http/schema/value.py
+-rw-r--r--   0        0        0      873 2023-06-09 05:50:36.425514 orwynn-1.0.0b5/orwynn/http/test_responses.py
+-rw-r--r--   0        0        0      126 2023-02-27 07:08:40.302249 orwynn-1.0.0b5/orwynn/http/testing.py
+-rw-r--r--   0        0        0      145 2023-06-09 06:20:20.111767 orwynn-1.0.0b5/orwynn/indication/__init__.py
+-rw-r--r--   0        0        0      231 2023-06-09 05:51:42.027891 orwynn-1.0.0b5/orwynn/indication/default.py
+-rw-r--r--   0        0        0      213 2023-03-06 11:23:49.055894 orwynn-1.0.0b5/orwynn/indication/errors.py
+-rw-r--r--   0        0        0      186 2023-06-08 13:55:11.806546 orwynn-1.0.0b5/orwynn/indication/indicatable.py
+-rw-r--r--   0        0        0    11518 2023-06-09 07:31:49.349629 orwynn-1.0.0b5/orwynn/indication/indication.py
+-rw-r--r--   0        0        0      373 2023-02-10 07:31:06.809383 orwynn-1.0.0b5/orwynn/indication/indicator.py
+-rw-r--r--   0        0        0     3422 2023-06-09 07:31:58.353224 orwynn-1.0.0b5/orwynn/indication/test_main.py
+-rw-r--r--   0        0        0      491 2023-02-10 07:37:36.270095 orwynn-1.0.0b5/orwynn/indication/type.py
+-rw-r--r--   0        0        0      120 2023-06-09 06:20:20.115767 orwynn-1.0.0b5/orwynn/log/__init__.py
+-rw-r--r--   0        0        0      152 2023-06-09 05:51:55.299360 orwynn-1.0.0b5/orwynn/log/config.py
+-rw-r--r--   0        0        0     1972 2023-06-09 07:45:46.128730 orwynn-1.0.0b5/orwynn/log/configure.py
+-rw-r--r--   0        0        0      114 2023-02-13 09:24:59.764293 orwynn-1.0.0b5/orwynn/log/constants.py
+-rw-r--r--   0        0        0       99 2023-03-06 11:23:49.055894 orwynn-1.0.0b5/orwynn/log/errors.py
+-rw-r--r--   0        0        0      870 2023-06-09 07:50:28.243651 orwynn-1.0.0b5/orwynn/log/handler.py
+-rw-r--r--   0        0        0      540 2023-06-09 05:52:01.299120 orwynn-1.0.0b5/orwynn/log/helpers.py
+-rw-r--r--   0        0        0       35 2023-02-14 07:07:42.021607 orwynn-1.0.0b5/orwynn/log/log.py
+-rw-r--r--   0        0        0     1767 2023-06-09 07:50:09.129655 orwynn-1.0.0b5/orwynn/log/test_main.py
+-rw-r--r--   0        0        0     3679 2023-06-09 06:00:41.008691 orwynn-1.0.0b5/orwynn/log/test_middleware.py
+-rw-r--r--   0        0        0     1443 2023-06-09 06:20:10.150480 orwynn-1.0.0b5/orwynn/log/test_websocketmiddleware.py
+-rw-r--r--   0        0        0       83 2023-06-09 07:50:59.221569 orwynn-1.0.0b5/orwynn/log/types.py
+-rw-r--r--   0        0        0       29 2023-06-09 05:52:49.668187 orwynn-1.0.0b5/orwynn/mapping/__init__.py
+-rw-r--r--   0        0        0      281 2023-03-06 11:23:49.055894 orwynn-1.0.0b5/orwynn/mapping/errors.py
+-rw-r--r--   0        0        0     1559 2023-06-08 13:55:11.826545 orwynn-1.0.0b5/orwynn/mapping/mapping.py
+-rw-r--r--   0        0        0      178 2023-06-09 05:52:49.667187 orwynn-1.0.0b5/orwynn/mapping/test_main.py
+-rw-r--r--   0        0        0      216 2023-06-09 06:20:20.112767 orwynn-1.0.0b5/orwynn/mongo/__init__.py
+-rw-r--r--   0        0        0      111 2022-12-25 22:05:28.493755 orwynn-1.0.0b5/orwynn/mongo/clientsession.py
+-rw-r--r--   0        0        0      133 2023-02-27 09:58:10.560648 orwynn-1.0.0b5/orwynn/mongo/config.py
+-rw-r--r--   0        0        0     6038 2023-06-09 06:20:20.110767 orwynn-1.0.0b5/orwynn/mongo/document.py
+-rw-r--r--   0        0        0       19 2022-12-25 11:43:30.248664 orwynn-1.0.0b5/orwynn/mongo/entity.py
+-rw-r--r--   0        0        0      445 2023-03-06 11:30:55.548595 orwynn-1.0.0b5/orwynn/mongo/errors.py
+-rw-r--r--   0        0        0     3567 2023-06-09 05:54:25.941338 orwynn-1.0.0b5/orwynn/mongo/mongo.py
+-rw-r--r--   0        0        0     3298 2023-06-09 07:04:54.571539 orwynn-1.0.0b5/orwynn/mongo/test_document.py
+-rw-r--r--   0        0        0     1354 2023-06-09 06:00:41.028688 orwynn-1.0.0b5/orwynn/mongo/test_main.py
+-rw-r--r--   0        0        0     2839 2023-06-09 06:03:10.133848 orwynn-1.0.0b5/orwynn/proxy/boot.py
+-rw-r--r--   0        0        0      310 2023-03-07 08:22:29.576929 orwynn-1.0.0b5/orwynn/proxy/indicationonly.py
+-rw-r--r--   0        0        0       27 2023-06-09 05:56:44.921784 orwynn-1.0.0b5/orwynn/router/__init__.py
+-rw-r--r--   0        0        0     3966 2023-06-09 06:23:57.815708 orwynn-1.0.0b5/orwynn/router/errorhandlermanager.py
+-rw-r--r--   0        0        0      116 2023-03-06 11:23:49.055894 orwynn-1.0.0b5/orwynn/router/errors.py
+-rw-r--r--   0        0        0    14259 2023-06-09 06:03:10.133848 orwynn-1.0.0b5/orwynn/router/register/controller.py
+-rw-r--r--   0        0        0     9656 2023-06-09 11:05:03.703488 orwynn-1.0.0b5/orwynn/router/register/middleware.py
+-rw-r--r--   0        0        0     2565 2023-06-09 11:05:03.696488 orwynn-1.0.0b5/orwynn/router/router.py
+-rw-r--r--   0        0        0     2465 2023-02-28 05:48:16.660066 orwynn-1.0.0b5/orwynn/router/test_globalroute.py
+-rw-r--r--   0        0        0       33 2023-06-09 05:57:10.064779 orwynn-1.0.0b5/orwynn/singleton/__init__.py
+-rw-r--r--   0        0        0     1318 2023-06-09 06:27:33.730658 orwynn-1.0.0b5/orwynn/singleton/singleton.py
+-rw-r--r--   0        0        0      203 2023-06-09 06:20:20.112767 orwynn-1.0.0b5/orwynn/sql/__init__.py
+-rw-r--r--   0        0        0     1964 2023-06-09 06:00:27.751246 orwynn-1.0.0b5/orwynn/sql/config.py
+-rw-r--r--   0        0        0      105 2023-01-19 15:20:28.442785 orwynn-1.0.0b5/orwynn/sql/databasekind.py
+-rw-r--r--   0        0        0       65 2023-02-28 06:53:56.326285 orwynn-1.0.0b5/orwynn/sql/poolclass.py
+-rw-r--r--   0        0        0     3878 2023-06-09 06:00:31.786840 orwynn-1.0.0b5/orwynn/sql/sql.py
+-rw-r--r--   0        0        0     2636 2023-05-22 08:54:47.949687 orwynn-1.0.0b5/orwynn/sql/table.py
+-rw-r--r--   0        0        0     5855 2023-06-09 06:20:20.114767 orwynn-1.0.0b5/orwynn/sql/test_main.py
+-rw-r--r--   0        0        0      721 2023-06-09 06:00:51.915024 orwynn-1.0.0b5/orwynn/testing/__init__.py
+-rw-r--r--   0        0        0    11299 2023-06-09 07:32:18.165326 orwynn-1.0.0b5/orwynn/testing/client.py
+-rw-r--r--   0        0        0      101 2022-12-29 09:50:50.883906 orwynn-1.0.0b5/orwynn/testing/embeddedclient.py
+-rw-r--r--   0        0        0     2046 2023-06-09 06:20:20.111767 orwynn-1.0.0b5/orwynn/testing/test_main.py
+-rw-r--r--   0        0        0     1106 2023-05-22 08:13:58.515604 orwynn-1.0.0b5/orwynn/testingtools/__init__.py
+-rw-r--r--   0        0        0       24 2022-12-22 07:52:56.312366 orwynn-1.0.0b5/orwynn/utils/basesubclassable.py
+-rw-r--r--   0        0        0      866 2023-04-03 14:59:49.716980 orwynn-1.0.0b5/orwynn/utils/crypto/__init__.py
+-rw-r--r--   0        0        0      508 2023-06-09 07:42:13.220704 orwynn-1.0.0b5/orwynn/utils/dt/__init__.py
+-rw-r--r--   0        0        0     1746 2023-02-23 07:22:44.852890 orwynn-1.0.0b5/orwynn/utils/fmt/__init__.py
+-rw-r--r--   0        0        0     1312 2023-04-03 14:59:49.716980 orwynn-1.0.0b5/orwynn/utils/fmt/test_main.py
+-rw-r--r--   0        0        0     1973 2023-06-09 06:01:29.753531 orwynn-1.0.0b5/orwynn/utils/klass/__init__.py
+-rw-r--r--   0        0        0       46 2023-03-07 05:33:50.925367 orwynn-1.0.0b5/orwynn/utils/klass/errors.py
+-rw-r--r--   0        0        0      522 2023-04-07 10:26:52.657368 orwynn-1.0.0b5/orwynn/utils/klass/test_klass.py
+-rw-r--r--   0        0        0     2544 2023-06-09 06:01:41.912390 orwynn-1.0.0b5/orwynn/utils/mp/__init__.py
+-rw-r--r--   0        0        0       98 2023-01-11 10:48:59.268124 orwynn-1.0.0b5/orwynn/utils/mp/dictpp.py
+-rw-r--r--   0        0        0     2448 2023-03-06 11:30:55.553595 orwynn-1.0.0b5/orwynn/utils/mp/location.py
+-rw-r--r--   0        0        0     1737 2023-06-09 06:01:41.912390 orwynn-1.0.0b5/orwynn/utils/mp/test_main.py
+-rw-r--r--   0        0        0      133 2023-02-17 07:27:38.315341 orwynn-1.0.0b5/orwynn/utils/protocol.py
+-rw-r--r--   0        0        0      131 2023-02-21 10:53:24.615257 orwynn-1.0.0b5/orwynn/utils/rnd/__init__.py
+-rw-r--r--   0        0        0       90 2023-04-03 14:59:49.716980 orwynn-1.0.0b5/orwynn/utils/rnd/test_main.py
+-rw-r--r--   0        0        0      341 2023-06-09 07:45:34.941367 orwynn-1.0.0b5/orwynn/utils/types.py
+-rw-r--r--   0        0        0      307 2023-03-07 05:31:01.650091 orwynn-1.0.0b5/orwynn/utils/uio.py
+-rw-r--r--   0        0        0      682 2023-06-09 06:02:47.709865 orwynn-1.0.0b5/orwynn/utils/url/__init__.py
+-rw-r--r--   0        0        0     1921 2023-06-09 06:20:20.108768 orwynn-1.0.0b5/orwynn/utils/url/helpers.py
+-rw-r--r--   0        0        0     1405 2023-06-09 06:02:47.710864 orwynn-1.0.0b5/orwynn/utils/url/test_utils.py
+-rw-r--r--   0        0        0       79 2023-02-22 12:14:57.519901 orwynn-1.0.0b5/orwynn/utils/url/url.py
+-rw-r--r--   0        0        0      419 2023-06-09 06:02:30.816698 orwynn-1.0.0b5/orwynn/utils/url/utils.py
+-rw-r--r--   0        0        0      253 2023-06-09 06:02:47.709865 orwynn-1.0.0b5/orwynn/utils/url/vars.py
+-rw-r--r--   0        0        0     9150 2023-06-09 06:02:55.428511 orwynn-1.0.0b5/orwynn/utils/validation/__init__.py
+-rw-r--r--   0        0        0     1796 2023-03-07 05:27:06.425420 orwynn-1.0.0b5/orwynn/utils/validation/errors.py
+-rw-r--r--   0        0        0      216 2022-12-16 11:42:54.126673 orwynn-1.0.0b5/orwynn/utils/validation/validator.py
+-rw-r--r--   0        0        0     1743 2023-04-03 14:59:49.716980 orwynn-1.0.0b5/orwynn/utils/yml/__init__.py
+-rw-r--r--   0        0        0       42 2023-03-06 11:23:49.055894 orwynn-1.0.0b5/orwynn/utils/yml/errors.py
+-rw-r--r--   0        0        0      638 2023-06-09 06:20:20.115767 orwynn-1.0.0b5/orwynn/websocket/__init__.py
+-rw-r--r--   0        0        0      995 2023-06-09 06:20:20.113767 orwynn-1.0.0b5/orwynn/websocket/constants.py
+-rw-r--r--   0        0        0        0 2023-06-09 06:40:48.176846 orwynn-1.0.0b5/orwynn/websocket/context/__init__.py
+-rw-r--r--   0        0        0     1028 2023-04-03 14:59:49.717980 orwynn-1.0.0b5/orwynn/websocket/context/id.py
+-rw-r--r--   0        0        0      550 2023-06-09 06:20:10.146480 orwynn-1.0.0b5/orwynn/websocket/context/middleware/builtin.py
+-rw-r--r--   0        0        0      768 2023-06-09 06:20:10.146480 orwynn-1.0.0b5/orwynn/websocket/context/middleware/contextbuiltin.py
+-rw-r--r--   0        0        0     1241 2023-06-09 06:27:59.917644 orwynn-1.0.0b5/orwynn/websocket/context/test_main.py
+-rw-r--r--   0        0        0     3966 2023-06-09 06:20:10.146480 orwynn-1.0.0b5/orwynn/websocket/controller/controller.py
+-rw-r--r--   0        0        0      146 2023-06-08 13:55:11.806546 orwynn-1.0.0b5/orwynn/websocket/controller/eventhandlermethod.py
+-rw-r--r--   0        0        0     3806 2023-06-09 07:21:01.679769 orwynn-1.0.0b5/orwynn/websocket/controller/test_controller.py
+-rw-r--r--   0        0        0     2888 2023-06-09 06:20:10.147480 orwynn-1.0.0b5/orwynn/websocket/controller/test_globalroute.py
+-rw-r--r--   0        0        0      410 2023-06-09 06:16:27.158191 orwynn-1.0.0b5/orwynn/websocket/errorhandler/default.py
+-rw-r--r--   0        0        0     3514 2023-06-09 06:20:20.115767 orwynn-1.0.0b5/orwynn/websocket/errorhandler/middleware.py
+-rw-r--r--   0        0        0     1699 2023-06-09 06:03:10.090856 orwynn-1.0.0b5/orwynn/websocket/errorhandler/test_default.py
+-rw-r--r--   0        0        0     1706 2023-06-09 06:16:27.191193 orwynn-1.0.0b5/orwynn/websocket/log/logger.py
+-rw-r--r--   0        0        0      910 2023-06-09 06:20:10.150480 orwynn-1.0.0b5/orwynn/websocket/log/middleware.py
+-rw-r--r--   0        0        0      303 2023-06-09 06:20:10.150480 orwynn-1.0.0b5/orwynn/websocket/middleware/builtin.py
+-rw-r--r--   0        0        0      856 2023-06-09 06:20:10.150480 orwynn-1.0.0b5/orwynn/websocket/middleware/connectionbuiltin.py
+-rw-r--r--   0        0        0      737 2023-06-09 06:20:10.149480 orwynn-1.0.0b5/orwynn/websocket/middleware/middleware.py
+-rw-r--r--   0        0        0      279 2023-06-09 06:16:27.159191 orwynn-1.0.0b5/orwynn/websocket/middleware/nextcall.py
+-rw-r--r--   0        0        0     1053 2023-06-09 06:27:59.918644 orwynn-1.0.0b5/orwynn/websocket/middleware/test_main.py
+-rw-r--r--   0        0        0      220 2023-06-09 06:16:27.190193 orwynn-1.0.0b5/orwynn/websocket/routing/dispatchfn.py
+-rw-r--r--   0        0        0       92 2023-02-15 09:24:37.556326 orwynn-1.0.0b5/orwynn/websocket/routing/genericfn.py
+-rw-r--r--   0        0        0      427 2023-06-09 06:15:15.485170 orwynn-1.0.0b5/orwynn/websocket/routing/handlers.py
+-rw-r--r--   0        0        0     5607 2023-06-09 07:32:02.386042 orwynn-1.0.0b5/orwynn/websocket/routing/helpers.py
+-rw-r--r--   0        0        0     1880 2023-06-09 06:20:20.114767 orwynn-1.0.0b5/orwynn/websocket/routing/nextcall.py
+-rw-r--r--   0        0        0     6065 2023-06-09 06:16:27.192193 orwynn-1.0.0b5/orwynn/websocket/routing/stack.py
+-rw-r--r--   0        0        0       82 2022-12-25 23:39:24.206537 orwynn-1.0.0b5/orwynn/websocket/websocket.py
+-rw-r--r--   0        0        0      823 2023-06-09 12:35:51.507901 orwynn-1.0.0b5/pyproject.toml
+-rw-r--r--   0        0        0     1280 1970-01-01 00:00:00.000000 orwynn-1.0.0b5/PKG-INFO
```

### Comparing `orwynn-1.0.0b4/LICENSE` & `orwynn-1.0.0b5/LICENSE`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b4/orwynn/_di/Di.py` & `orwynn-1.0.0b5/orwynn/di/di.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from orwynn._di.collecting.collect_provider_dependencies import (
+from orwynn.app.app import App
+from orwynn.base.controller.controller import Controller
+from orwynn.base.errorhandler.errorhandler import ErrorHandler
+from orwynn.base.middleware import GlobalMiddlewareSetup, Middleware
+from orwynn.base.module.module import Module
+from orwynn.base.worker.worker import Worker
+from orwynn.di.collecting.modulecollector import ModuleCollector
+from orwynn.di.collecting.providerdependencies.collect import (
     collect_provider_dependencies,
 )
-from orwynn._di.collecting.ModuleCollector import ModuleCollector
-from orwynn._di.DiContainer import DiContainer
-from orwynn._di.DiObject import DiObject
-from orwynn._di.init.init_other_acceptors import init_other_acceptors
-from orwynn._di.init.init_providers import init_providers
-from orwynn.app._App import App
-from orwynn.base.controller._Controller import Controller
-from orwynn.base.errorhandler._ErrorHandler import ErrorHandler
-from orwynn.base.middleware import GlobalMiddlewareSetup, Middleware
-from orwynn.base.module._Module import Module
-from orwynn.base.worker._Worker import Worker
+from orwynn.di.container import DiContainer
+from orwynn.di.init.acceptors import init_other_acceptors
+from orwynn.di.init.providers import init_providers
+from orwynn.di.object import DiObject
 from orwynn.log import LogConfig
 from orwynn.utils import validation
 
 
 class Di(Worker):
     """Resolves Dependency-injection related tasks for an application.
```

### Comparing `orwynn-1.0.0b4/orwynn/_di/DiContainer.py` & `orwynn-1.0.0b5/orwynn/di/container.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import re
 from typing import TypeVar
 
-from orwynn._di.DiObject import DiObject
-from orwynn._di.DiObjectAlreadyInitializedInContainerError import (
-    DiObjectAlreadyInitializedInContainerError,
-)
-from orwynn._di.FinalizedDiContainerError import FinalizedDiContainerError
-from orwynn._di.is_provider import is_provider
-from orwynn._di.MissingDiObjectError import MissingDiObjectError
 from orwynn.base.config import Config
-from orwynn.base.controller._Controller import Controller
-from orwynn.base.error._MalfunctionError import MalfunctionError
-from orwynn.base.errorhandler._ErrorHandler import ErrorHandler
+from orwynn.base.controller.controller import Controller
+from orwynn.base.error.errors import MalfunctionError
+from orwynn.base.errorhandler.errorhandler import ErrorHandler
 from orwynn.base.middleware import Middleware
-from orwynn.base.model._Model import Model
-from orwynn.helpers.SUBCLASSABLES import SUBCLASSABLES
+from orwynn.base.model.model import Model
+from orwynn.di.errors import (
+    DiObjectAlreadyInitializedInContainerError,
+    FinalizedDiContainerError,
+    MissingDiObjectError,
+)
+from orwynn.di.isprovider import is_provider
+from orwynn.di.object import DiObject
+from orwynn.helpers.constants import SUBCLASSABLES
 from orwynn.utils.validation import validate
 
 _InnerObj = TypeVar("_InnerObj")
 
 
 class DiContainer:
     """Holds data about initialized di objects."""
```

### Comparing `orwynn-1.0.0b4/orwynn/_di/_collect_dependencies_for_acceptor.py` & `orwynn-1.0.0b5/orwynn/di/collecting/acceptordependencies.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import inspect
 from typing import Callable
 
-from orwynn._di.check_availability import check_availability
-from orwynn._di.DiContainer import DiContainer
-from orwynn._di.DiObject import DiObject
-from orwynn._di.Provider import Provider
 from orwynn.base.middleware import Middleware
 from orwynn.base.module import Module
+from orwynn.di.availability import check_availability
+from orwynn.di.container import DiContainer
+from orwynn.di.object import DiObject
+from orwynn.di.provider import Provider
 
 
 def collect_dependencies_for_acceptor(
     acceptor_callable: Callable,
     container: DiContainer,
     acceptor_module: Module | None
 ) -> dict[str, Provider]:
```

### Comparing `orwynn-1.0.0b4/orwynn/_di/check_availability.py` & `orwynn-1.0.0b5/orwynn/di/availability.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,14 @@
-
-
-from orwynn._di.DiObject import DiObject
-from orwynn._di.is_provider import is_provider
-from orwynn._di.NotProviderError import NotProviderError
-from orwynn._di.Provider import Provider
-from orwynn._di.ProviderAvailabilityError import ProviderAvailabilityError
 from orwynn.base.config import Config
-from orwynn.base.module._Module import Module
-from orwynn.base.service._FrameworkService import FrameworkService
+from orwynn.base.module.module import Module
+from orwynn.base.service.framework import FrameworkService
+from orwynn.di.errors import NotProviderError, ProviderAvailabilityError
+from orwynn.di.isprovider import is_provider
+from orwynn.di.object import DiObject
+from orwynn.di.provider import Provider
 
 
 def check_availability(
     Requestor: type[DiObject],
     Target: type[Provider],
     requestor_module: Module | None
 ) -> Module | None:
```

### Comparing `orwynn-1.0.0b4/orwynn/_di/collecting/ModuleCollector.py` & `orwynn-1.0.0b5/orwynn/di/collecting/modulecollector.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b4/orwynn/_di/collecting/collect_modules_test.py` & `orwynn-1.0.0b5/orwynn/di/collecting/test_modules.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from pytest import fixture
 
-from orwynn._di.collecting.ModuleCollector import ModuleCollector
-from orwynn.base.module._Module import Module
 from orwynn.base.module.errors import CircularDependencyError
+from orwynn.base.module.module import Module
+from orwynn.di.collecting.modulecollector import ModuleCollector
 from orwynn.utils.validation import expect
-from tests.std.Assertion import Assertion
+from tests.std.assertion import Assertion
 
 
 @fixture
 def std_modules(std_struct: Module) -> list[Module]:
     return ModuleCollector(std_struct).collected_modules
```

### Comparing `orwynn-1.0.0b4/orwynn/_di/collecting/collect_provider_dependencies.py` & `orwynn-1.0.0b5/orwynn/di/collecting/providerdependencies/collect.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-from orwynn._di.check_availability import check_availability
-from orwynn._di.collecting.get_parameters_for_provider import (
+from orwynn.base.config import Config
+from orwynn.base.module import Module
+from orwynn.base.module.errors import CircularDependencyError
+from orwynn.di.availability import check_availability
+from orwynn.di.collecting.errors import (
+    ProviderAlreadyInitializedForMapError,
+)
+from orwynn.di.collecting.helpers import (
     get_parameters_for_provider,
 )
-from orwynn._di.collecting.provider_dependencies_map import (
+from orwynn.di.collecting.providerdependencies.map import (
     ProviderDependenciesMap,
 )
-from orwynn._di.collecting.ProviderAlreadyInitializedForMapError import (
-    ProviderAlreadyInitializedForMapError,
-)
-from orwynn._di.is_provider import is_provider
-from orwynn._di.NotProviderError import NotProviderError
-from orwynn._di.Provider import Provider
-from orwynn.base.config import Config
-from orwynn.base.module import Module
-from orwynn.base.module.errors import CircularDependencyError
+from orwynn.di.errors import NotProviderError
+from orwynn.di.isprovider import is_provider
+from orwynn.di.provider import Provider
 from orwynn.utils.fmt import format_chain
 
 
 def collect_provider_dependencies(
     modules: list[Module]
 ) -> ProviderDependenciesMap:
     """Collects providers and their dependencies from given modules.
```

### Comparing `orwynn-1.0.0b4/orwynn/_di/collecting/collect_provider_dependencies_test.py` & `orwynn-1.0.0b5/orwynn/di/collecting/providerdependencies/test_main.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 import inspect
 
 from pytest import fixture
 
-from orwynn._di.collecting.collect_provider_dependencies import (
-    ProviderDependenciesMap,
-    collect_provider_dependencies,
-)
-from orwynn._di.collecting.ModuleCollector import ModuleCollector
-from orwynn._di.is_provider import is_provider
-from orwynn._di.Provider import Provider
 from orwynn.base.config import Config
 from orwynn.base.module import Module
+from orwynn.di.collecting.modulecollector import ModuleCollector
+from orwynn.di.collecting.providerdependencies.collect import (
+    collect_provider_dependencies,
+)
+from orwynn.di.collecting.providerdependencies.map import (
+    ProviderDependenciesMap,
+)
+from orwynn.di.isprovider import is_provider
+from orwynn.di.provider import Provider
 from orwynn.log import LogConfig
-from tests.std.Assertion import Assertion
+from tests.std.assertion import Assertion
 
 
 @fixture
 def std_provider_dependencies_map(
     std_modules: list[Module]
 ) -> ProviderDependenciesMap:
     return collect_provider_dependencies(std_modules)
```

### Comparing `orwynn-1.0.0b4/orwynn/_di/collecting/get_parameters_for_provider.py` & `orwynn-1.0.0b5/orwynn/di/collecting/helpers.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import inspect
 
-from orwynn._di.collecting.provider_keyword_attribute_error import (
+from orwynn.base.config import Config
+from orwynn.base.model.model import Model
+from orwynn.di.collecting.errors import (
     ProviderKeywordAttributeError,
 )
-from orwynn._di.is_provider import is_provider
-from orwynn._di.NoAnnotationError import NoAnnotationError
-from orwynn._di.NotProviderError import NotProviderError
-from orwynn._di.Provider import Provider
-from orwynn.base.config import Config
-from orwynn.base.model._Model import Model
+from orwynn.di.errors import NoAnnotationError, NotProviderError
+from orwynn.di.isprovider import is_provider
+from orwynn.di.provider import Provider
 
 ProviderParameters = list["ProviderParameter"]
 
 
 class ProviderParameter(Model):
     name: str
     DependencyProvider: type[Provider]
```

### Comparing `orwynn-1.0.0b4/orwynn/_di/collecting/provider_dependencies_map.py` & `orwynn-1.0.0b5/orwynn/di/collecting/providerdependencies/map.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,13 @@
-from orwynn._di.collecting.no_dependencies_for_given_provider_error import (
+from orwynn.di.collecting.errors import (
     NoDependenciesForGivenProviderError,
-)
-from orwynn._di.collecting.provider_not_found_in_map_error import (
-    ProviderNotFoundInMapError,
-)
-from orwynn._di.collecting.ProviderAlreadyInitializedForMapError import (
     ProviderAlreadyInitializedForMapError,
+    ProviderNotFoundInMapError,
 )
-from orwynn._di.Provider import Provider
+from orwynn.di.provider import Provider
 
 
 class ProviderDependenciesMap:
     """Maps Providers and their requested dependencies.
 
     Since providers can request only other providers, it's a representation of
     Provider to Provider map.
```

### Comparing `orwynn-1.0.0b4/orwynn/_di/init/init_other_acceptors.py` & `orwynn-1.0.0b5/orwynn/di/init/acceptors.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 
-from orwynn._di._collect_dependencies_for_acceptor import (
+from orwynn.base.controller.controller import Controller
+from orwynn.base.middleware import GlobalMiddlewareSetup, Middleware
+from orwynn.base.model.model import Model
+from orwynn.base.module.module import Module
+from orwynn.di.collecting.acceptordependencies import (
     collect_dependencies_for_acceptor,
 )
-from orwynn._di.DiContainer import DiContainer
-from orwynn.base.controller._Controller import Controller
-from orwynn.base.middleware import GlobalMiddlewareSetup, Middleware
-from orwynn.base.model._Model import Model
-from orwynn.base.module._Module import Module
+from orwynn.di.container import DiContainer
 from orwynn.http import HttpController, HttpMiddleware
-from orwynn.proxy.BootProxy import BootProxy
+from orwynn.proxy.boot import BootProxy
 from orwynn.utils import validation
 from orwynn.utils.url import join_routes
 from orwynn.utils.validation import validate
 from orwynn.websocket import WebsocketController, WebsocketMiddleware
 
 
 class __CoveredRoutes(Model):
```

### Comparing `orwynn-1.0.0b4/orwynn/_di/init/init_other_acceptors_test.py` & `orwynn-1.0.0b5/orwynn/di/init/test_acceptors.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-from orwynn._di.DiContainer import DiContainer
-from orwynn._di.init.init_other_acceptors import init_other_acceptors
-from orwynn._di.ProviderAvailabilityError import ProviderAvailabilityError
 from orwynn.base.module import Module
 from orwynn.base.service import Service
-from orwynn.boot._Boot import Boot
+from orwynn.boot.boot import Boot
+from orwynn.di.container import DiContainer
+from orwynn.di.errors import ProviderAvailabilityError
+from orwynn.di.init.acceptors import init_other_acceptors
 from orwynn.http import Endpoint, HttpController, HttpMiddleware
 from orwynn.utils import validation
-from tests.std.Assertion import Assertion
+from tests.std.assertion import Assertion
 
 
 def test_std(
     std_di_container: DiContainer,
     std_modules: list[Module]
 ):
     init_other_acceptors(std_di_container, std_modules)
```

### Comparing `orwynn-1.0.0b4/orwynn/_di/init/init_providers.py` & `orwynn-1.0.0b5/orwynn/di/init/providers.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import inspect
 
-from orwynn._di.collecting.no_dependencies_for_given_provider_error import (
+from orwynn.base.config import Config
+from orwynn.base.module.errors import CircularDependencyError
+from orwynn.di.collecting.errors import (
     NoDependenciesForGivenProviderError,
 )
-from orwynn._di.collecting.provider_dependencies_map import (
+from orwynn.di.collecting.providerdependencies.map import (
     ProviderDependenciesMap,
 )
-from orwynn._di.DiContainer import DiContainer
-from orwynn._di.is_provider import is_provider
-from orwynn._di.MissingDiObjectError import MissingDiObjectError
-from orwynn._di.Provider import Provider
-from orwynn.base.config import Config
-from orwynn.base.module.errors import CircularDependencyError
+from orwynn.di.container import DiContainer
+from orwynn.di.errors import MissingDiObjectError
+from orwynn.di.isprovider import is_provider
+from orwynn.di.provider import Provider
 from orwynn.utils.fmt import format_chain
 
 
 def init_providers(
     provider_dependencies_map: ProviderDependenciesMap
 ) -> DiContainer:
     """Traverses through given providers and dependencies initializing them.
@@ -114,11 +114,11 @@
                     param.annotation.__name__
                 )
 
         result_provider = StarterProvider.load(extra=provider_kwargs)
     else:
         result_provider = StarterProvider(
             *already_initialized_dependencies
-        )
+        )  # type: ignore
 
     container.add(result_provider)
     return result_provider
```

### Comparing `orwynn-1.0.0b4/orwynn/_di/init/init_providers_test.py` & `orwynn-1.0.0b5/orwynn/di/init/test_providers.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from orwynn._di.collecting.provider_dependencies_map import (
+from orwynn.base.module.module import Module
+from orwynn.boot.boot import Boot
+from orwynn.di.collecting.providerdependencies.map import (
     ProviderDependenciesMap,
 )
-from orwynn._di.DiContainer import DiContainer
-from orwynn._di.init.init_providers import init_providers
-from orwynn.base.module._Module import Module
-from orwynn.boot._Boot import Boot
-from tests.std.Assertion import Assertion
+from orwynn.di.container import DiContainer
+from orwynn.di.init.providers import init_providers
+from tests.std.assertion import Assertion
 
 
 def test_std(
     std_struct: Module,
     std_provider_dependencies_map: ProviderDependenciesMap
 ):
     Boot(std_struct)
```

### Comparing `orwynn-1.0.0b4/orwynn/_testingtools/__init__.py` & `orwynn-1.0.0b5/orwynn/testingtools/__init__.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b4/orwynn/apiversion/_ApiVersion.py` & `orwynn-1.0.0b5/orwynn/apiversion/__init__.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b4/orwynn/apiversion/api_version_test.py` & `orwynn-1.0.0b5/orwynn/apiversion/test_main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from orwynn.base.module._Module import Module
-from orwynn.boot._Boot import Boot
+from orwynn.base.module.module import Module
+from orwynn.boot.boot import Boot
 from orwynn.http import Endpoint, HttpController
 from orwynn.utils import validation
 
-from ._ApiVersion import ApiVersion
+from . import ApiVersion
 from .errors import UnsupportedVersionError
 
 # NOTE: By default there is no global route for backwards compatiblity.
 
 def test_versioned_global_route():
     class C(HttpController):
         ROUTE = "/message"
```

### Comparing `orwynn-1.0.0b4/orwynn/app/_ApiWebsocketRoute.py` & `orwynn-1.0.0b5/orwynn/app/apiwebsocketroute.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from fastapi.routing import get_websocket_app
 from starlette.routing import (
     compile_path,
     get_name,
     websocket_session,
 )
 
-from orwynn.app._get_dependant import get_dependant
+from orwynn.app.utils import get_dependant
 
 
 class ApiWebsocketRoute(_NativeWebsocketRoute):
     def __init__(
         self,
         path: str,
         endpoint: Callable[..., Any],
```

### Comparing `orwynn-1.0.0b4/orwynn/app/_CoreApp.py` & `orwynn-1.0.0b5/orwynn/app/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from fastapi import FastAPI
 from fastapi.middleware.asyncexitstack import AsyncExitStackMiddleware
 from starlette.middleware import Middleware
 from starlette.middleware.errors import ServerErrorMiddleware
 from starlette.middleware.exceptions import ExceptionMiddleware
 from starlette.types import ASGIApp
 
-from orwynn.app._ApiRouter import ApiRouter
+from orwynn.app.apirouter import ApiRouter
 
 
 class CoreApp(FastAPI):
     def __init__(self, **kwargs) -> None:
         with patch("fastapi.routing.APIRouter", new=ApiRouter):
             super().__init__(**kwargs)
```

### Comparing `orwynn-1.0.0b4/orwynn/app/_get_dependant.py` & `orwynn-1.0.0b5/orwynn/app/utils.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b4/orwynn/app/app_test.py` & `orwynn-1.0.0b5/orwynn/app/test_main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from pytest import fixture
 
-from orwynn.app._App import App
+from orwynn.app.app import App
 from orwynn.base.module import Module
 from orwynn.boot import Boot
 from orwynn.websocket import Websocket, WebsocketController
 
 
 @fixture
 def std_app(std_boot: Boot) -> App:
```

### Comparing `orwynn-1.0.0b4/orwynn/apprc/_parse_apprc.py` & `orwynn-1.0.0b5/orwynn/apprc/parse.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import contextlib
 import os
 from pathlib import Path
 from types import NoneType
 
 from orwynn.app import AppMode
-from orwynn.apprc._AppRc import AppRc
+from orwynn.apprc.apprc import AppRc
 from orwynn.utils import validation
 from orwynn.utils.mp import patch as mp_patch
 from orwynn.utils.yml import load_yml
 
-from ._APP_RC_MODE_NESTING import APP_RC_MODE_NESTING
-from ._AppRcSearchError import AppRcSearchError
+from .constants import APP_RC_MODE_NESTING
+from .errors import AppRcSearchError
 
 
 def parse_apprc(
     root_dir: Path,
     mode: AppMode,
     direct_apprc: AppRc | None
 ) -> AppRc:
```

### Comparing `orwynn-1.0.0b4/orwynn/apprc/apprc_test.py` & `orwynn-1.0.0b5/orwynn/apprc/test_main.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import pytest
 
-from orwynn._di.Di import Di
 from orwynn.app import AppMode
-from orwynn.apprc._AppRc import AppRc
+from orwynn.apprc.apprc import AppRc
 from orwynn.base.config import Config
-from orwynn.base.model._Model import Model
-from orwynn.base.module._Module import Module
+from orwynn.base.model.model import Model
+from orwynn.base.module.module import Module
 from orwynn.boot import Boot
+from orwynn.di.di import Di
 from orwynn.utils import validation
 from orwynn.utils.mp import find as mp_find
 
 
 class Menu(Model):
     __root__: dict[str, float]
```

### Comparing `orwynn-1.0.0b4/orwynn/base/config/_Config.py` & `orwynn-1.0.0b5/orwynn/base/config/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import re
 from typing import TYPE_CHECKING, Any, Self
 
-from orwynn.base.model._Model import Model
-from orwynn.proxy.BootProxy import BootProxy
+from orwynn.base.model.model import Model
+from orwynn.proxy.boot import BootProxy
 from orwynn.utils import validation
 
 if TYPE_CHECKING:
-    from orwynn.apprc._AppRc import AppRc
+    from orwynn.apprc.apprc import AppRc
 
 
 class Config(Model):
     """Object holding configuration which can be injected to any requesting
     entity.
     """
     @classmethod
```

### Comparing `orwynn-1.0.0b4/orwynn/base/controller/_Controller.py` & `orwynn-1.0.0b5/orwynn/base/controller/controller.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b4/orwynn/base/database/_Database.py` & `orwynn-1.0.0b5/orwynn/base/database/database.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-from orwynn.base.service._Service import Service
+from orwynn.base.service.service import Service
 
 
 class Database(Service):
     """Represents a connection to database as well as set of actions with this
     database.
 
     This is an abstract class and defines core methods which should present on
```

### Comparing `orwynn-1.0.0b4/orwynn/base/database/errors.py` & `orwynn-1.0.0b5/orwynn/base/database/errors.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b4/orwynn/base/error/_errcode.py` & `orwynn-1.0.0b5/orwynn/base/error/code.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b4/orwynn/base/error/_find_detailed_class_for_exception.py` & `orwynn-1.0.0b5/orwynn/base/error/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,7 +54,15 @@
     Returns True if an Exception1 has more detail level than Exception2 and
     False otherwise. Also returns False if both given exception classes have
     the same level of detail.
     """
     mro1: list[type] = Exception1.mro()
 
     return (Exception2 in mro1)
+
+
+def get_exception_direct_subclasses() -> list[type[Exception]]:
+    """
+    Returns all base Exception direct subclasses.
+    """
+    all_exceptions: list[type[Exception]] = Exception.__subclasses__()
+    return all_exceptions
```

### Comparing `orwynn-1.0.0b4/orwynn/base/errorhandler/_ErrorHandler.py` & `orwynn-1.0.0b5/orwynn/base/errorhandler/errorhandler.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import os
 from typing import ClassVar
 
-from orwynn.base.error._MalfunctionError import MalfunctionError
+from orwynn.base.error.errors import MalfunctionError
 from orwynn.helpers.web import GenericRequest, GenericResponse
 from orwynn.log.helpers import catch_error
-from orwynn.proxy.BootProxy import BootProxy
+from orwynn.proxy.boot import BootProxy
 from orwynn.utils import validation
-from orwynn.utils.Protocol import Protocol
+from orwynn.utils.protocol import Protocol
 
 
 class ErrorHandler:
     """Handles outcoming errors from the application.
     Method handle(...) should be redefined in subclass in order to work.
 
     Class-Attributes:
```

### Comparing `orwynn-1.0.0b4/orwynn/base/middleware/_Middleware.py` & `orwynn-1.0.0b5/orwynn/base/middleware/middleware.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b4/orwynn/base/middleware/global_middleware_test.py` & `orwynn-1.0.0b5/orwynn/base/middleware/test_main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from orwynn._di.Di import Di
 from orwynn.base.module import Module
-from orwynn.boot._Boot import Boot
+from orwynn.boot.boot import Boot
+from orwynn.di.di import Di
 from orwynn.http import HttpMiddleware
 from orwynn.utils import validation
 from orwynn.websocket import WebsocketMiddleware
 
 
 def test_http():
     """
```

### Comparing `orwynn-1.0.0b4/orwynn/base/model/_Model.py` & `orwynn-1.0.0b5/orwynn/base/model/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import TYPE_CHECKING, Any, ClassVar, Self, TypeVar, Union
 
 import pydantic
 
-from orwynn.proxy.ApiIndicationOnlyProxy import ApiIndicationOnlyProxy
+from orwynn.proxy.indicationonly import ApiIndicationOnlyProxy
 from orwynn.utils import validation
 
 if TYPE_CHECKING:
     from orwynn.indication import IndicationType
 
 RecoverType = TypeVar("RecoverType", bound="Model")
```

### Comparing `orwynn-1.0.0b4/orwynn/base/model/model_test.py` & `orwynn-1.0.0b5/orwynn/base/model/test_model.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from orwynn.base.model._Model import Model
-from orwynn.indication._Indication import Indication
-from orwynn.indication._IndicationType import IndicationType
-from orwynn.indication._Indicator import Indicator
+from orwynn.base.model.model import Model
+from orwynn.indication.indication import Indication
+from orwynn.indication.indicator import Indicator
+from orwynn.indication.type import IndicationType
 
 
 def test_default_indication_type():
     class Item(Model):
         name: str
         price: float
```

### Comparing `orwynn-1.0.0b4/orwynn/base/module/_Module.py` & `orwynn-1.0.0b5/orwynn/base/module/module.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from orwynn.base.controller import Controller
 from orwynn.base.middleware import Middleware as MiddlewareClass
 from orwynn.base.module.errors import (
     CircularDependencyError,
     EmptyRouteError,
     FrameworkServiceModuleReferenceError,
 )
-from orwynn.base.service._FrameworkService import FrameworkService
+from orwynn.base.service.framework import FrameworkService
 from orwynn.utils import validation
 from orwynn.utils.validation import validate, validate_route
 
 
 class Module:
     """Provides metadata to organize the application structure.
```

### Comparing `orwynn-1.0.0b4/orwynn/base/module/module_test.py` & `orwynn-1.0.0b5/orwynn/base/module/test_module.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from orwynn.base.module._Module import Module
+from orwynn.base.module.module import Module
 from orwynn.http import (
     Endpoint,
     HttpController,
     HttpMiddleware,
     HttpNextCall,
     HttpRequest,
     HttpResponse,
```

### Comparing `orwynn-1.0.0b4/orwynn/boot/_Boot.py` & `orwynn-1.0.0b5/orwynn/boot/boot.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,31 +2,31 @@
 import os
 from copy import deepcopy
 from pathlib import Path
 from types import NoneType
 
 import dotenv
 
-from orwynn._di.Di import Di
-from orwynn._di.MissingDiObjectError import MissingDiObjectError
 from orwynn.apiversion import ApiVersion
 from orwynn.app import App, AppMode
 from orwynn.apprc import AppRc, parse_apprc
 from orwynn.base.controller import Controller
 from orwynn.base.errorhandler import ErrorHandler
 from orwynn.base.middleware import GlobalMiddlewareSetup, Middleware
 from orwynn.base.module import Module
 from orwynn.base.worker import Worker
 from orwynn.bootscript import Bootscript, BootscriptWorker, CallTime
 from orwynn.bootscript.errors import NoScriptsForCallTimeError
-from orwynn.http import Cors, EndpointContainer
+from orwynn.di.di import Di
+from orwynn.di.errors import MissingDiObjectError
+from orwynn.http import EndpointContainer
 from orwynn.indication import Indication, default_api_indication
 from orwynn.log import LogConfig, configure_log
-from orwynn.proxy.ApiIndicationOnlyProxy import ApiIndicationOnlyProxy
-from orwynn.proxy.BootProxy import BootProxy
+from orwynn.proxy.boot import BootProxy
+from orwynn.proxy.indicationonly import ApiIndicationOnlyProxy
 from orwynn.router import Router
 from orwynn.testing import Client
 from orwynn.utils import validation
 from orwynn.utils.validation import validate, validate_dict, validate_each
 from orwynn.utils.yml.errors import NotDirError
 
 
@@ -41,17 +41,14 @@
             Root module of the app.
         dotenv_path (optional):
             Path to .env file. Defaults to ".env".
         api_indication (optional):
             Indication object used as a convention for outcoming API
             structures. Defaults to predefined by framework's indication
             convention.
-        cors (optional):
-            CORS policy applied to the whole application. No CORS applied by
-            default.
         ErrorHandlers (optional):
             List of exception handlers to add. By default framework adds
             the builtin Exception and orwynn.Error handlers.
         apprc (optional):
             Application configuration. By default environ ORWYNN_APPRC_PATH is
             checked if this arg is not given.
         mode (optional):
@@ -106,15 +103,14 @@
     """
     def __init__(
         self,
         root_module: Module,
         *,
         dotenv_path: Path | None = None,
         api_indication: Indication | None = None,
-        cors: Cors | None = None,
         ErrorHandlers: set[type[ErrorHandler]] | None = None,
         apprc: AppRc | None = None,
         mode: AppMode | None = None,
         global_http_route: str | None = None,
         global_websocket_route: str | None = None,
         global_modules: list[Module] | None = None,
         global_middleware: GlobalMiddlewareSetup | None = None,
@@ -125,15 +121,14 @@
         if dotenv_path is None:
             dotenv_path = Path(".env")
         validate(dotenv_path, Path)
         validate(root_module, Module)
         if api_indication is None:
             api_indication = default_api_indication
         validate(api_indication, Indication)
-        validate(cors, [Cors, NoneType])
         if ErrorHandlers is None:
             ErrorHandlers = set()
         validate_each(
             ErrorHandlers, ErrorHandler, expected_sequence_type=set
         )
         validate(apprc, [AppRc, NoneType])
         validate(mode, [AppMode, NoneType])
@@ -194,24 +189,22 @@
 
         self.__di: Di = Di(
             root_module,
             global_modules=global_modules,
             global_middleware=global_middleware
         )
 
+        self.__init_router()
+
         # Configure logging
         configure_log(
             validation.apply(self.__di.find("LogConfig"), LogConfig),
             app_mode_prod=AppMode.PROD
         )
 
-        self.__init_router(
-            cors=cors
-        )
-
         # AFTER_ALL bootscript call time
         with contextlib.suppress(NoScriptsForCallTimeError):
             bootscript_worker.call_by_time(
                 CallTime.AFTER_ALL,
                 self.__di._fw_container
             )
 
@@ -238,19 +231,15 @@
             global_http_route=self.__global_http_route,
             global_websocket_route=self.__global_websocket_route,
             api_version=self.__api_version
         )
         EndpointContainer()
         ApiIndicationOnlyProxy(api_indication)
 
-    def __init_router(
-        self,
-        *,
-        cors: Cors | None
-    ) -> Router:
+    def __init_router(self) -> Router:
         try:
             all_modules: list[Module] = self.__di.modules
         except MissingDiObjectError:
             all_modules = []
 
         try:
             all_controllers: list[Controller] = self.__di.controllers
@@ -269,15 +258,14 @@
             all_exception_handlers = []
 
         return Router(
             self.app,
             global_http_route=self.__global_http_route,
             global_websocket_route=self.__global_websocket_route,
             api_version=self.__api_version,
-            cors=cors,
             modules=all_modules,
             controllers=all_controllers,
             middleware_arr=all_middleware,
             exception_handlers=all_exception_handlers
         )
 
     @property
```

### Comparing `orwynn-1.0.0b4/orwynn/boot/boot_test.py` & `orwynn-1.0.0b5/orwynn/boot/test_main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import os
 
 import pytest
 from pytest import fixture
 
-from orwynn._di.Di import Di
 from orwynn.app import AppMode
-from orwynn.apprc._AppRc import AppRc
-from orwynn.base.module._Module import Module
+from orwynn.apprc.apprc import AppRc
 from orwynn.base.module.errors import CircularDependencyError
-from orwynn.base.service._Service import Service
-from orwynn.boot._Boot import Boot
+from orwynn.base.module.module import Module
+from orwynn.base.service.service import Service
+from orwynn.boot.boot import Boot
+from orwynn.di.di import Di
 from orwynn.http import Endpoint, HttpController
-from orwynn.mongo._Mongo import Mongo
-from orwynn.proxy.BootProxy import BootProxy
+from orwynn.mongo.mongo import Mongo
+from orwynn.proxy.boot import BootProxy
 from orwynn.utils import validation
 from tests.std.text import TextConfig
 
 
 class _GService(Service):
     def calculate(self, *args: int) -> int:
         return sum(args)
```

### Comparing `orwynn-1.0.0b4/orwynn/bootscript/_BootscriptWorker.py` & `orwynn-1.0.0b5/orwynn/bootscript/worker.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-from orwynn._di._collect_dependencies_for_acceptor import (
-    collect_dependencies_for_acceptor,
-)
-from orwynn._di.DiContainer import DiContainer
 from orwynn.base.worker import Worker
-from orwynn.bootscript._Bootscript import Bootscript
-from orwynn.bootscript._CallTime import CallTime
+from orwynn.bootscript.bootscript import Bootscript
+from orwynn.bootscript.calltime import CallTime
 from orwynn.bootscript.errors import (
     NoScriptsForCallTimeError,
     ScriptsAlreadyCalledError,
 )
+from orwynn.di.collecting.acceptordependencies import (
+    collect_dependencies_for_acceptor,
+)
+from orwynn.di.container import DiContainer
 
 _IsCallPerformed = bool
 # Represents bootscripts sorted by their call time and followed by
 # a flag signified whether the call was already performed
 _ScriptsState = tuple[list[Bootscript], _IsCallPerformed]
 _CallState = dict[CallTime, _ScriptsState]
```

### Comparing `orwynn-1.0.0b4/orwynn/bootscript/bootscript_test.py` & `orwynn-1.0.0b5/orwynn/bootscript/test_main.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from orwynn._di.Di import Di
 from orwynn.base.module import Module
 from orwynn.base.service import Service
 from orwynn.boot import Boot
-from orwynn.bootscript._Bootscript import Bootscript
-from orwynn.bootscript._CallTime import CallTime
+from orwynn.bootscript.bootscript import Bootscript
+from orwynn.bootscript.calltime import CallTime
+from orwynn.di.di import Di
 from orwynn.utils import validation
 
 
 class SomeService(Service):
     def __init__(self) -> None:
         super().__init__()
         self.some_var: int = 0
```

### Comparing `orwynn-1.0.0b4/orwynn/context/_ContextStorage.py` & `orwynn-1.0.0b5/orwynn/context/storage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from contextvars import ContextVar, Token
 from typing import Any
 
-from orwynn.base.worker._Worker import Worker
+from orwynn.base.worker.worker import Worker
 from orwynn.utils import validation
 
 from .errors import AlreadyInitializedStorageError, UndefinedStorageError
 
 
 class ContextStorage(Worker):
     def __init__(self) -> None:
```

### Comparing `orwynn-1.0.0b4/orwynn/context/_context_manager.py` & `orwynn-1.0.0b5/orwynn/context/manager.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from contextlib import contextmanager
 from contextvars import Token
 
-from orwynn.context._ContextStorage import ContextStorage
+from orwynn.context.storage import ContextStorage
 from orwynn.utils import validation
 
 
 @contextmanager
 def context_manager(
     data: dict | None = None
 ):
```

### Comparing `orwynn-1.0.0b4/orwynn/helpers/SUBCLASSABLES.py` & `orwynn-1.0.0b5/orwynn/helpers/constants.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,28 @@
 """List of classes an user can subclass from."""
-from orwynn.base.controller._Controller import Controller
-from orwynn.base.errorhandler._ErrorHandler import ErrorHandler
+from orwynn.base.controller.controller import Controller
+from orwynn.base.errorhandler.errorhandler import ErrorHandler
 from orwynn.base.middleware import Middleware
-from orwynn.base.model._Model import Model
-from orwynn.base.service._Service import Service
-from orwynn.utils.BaseSubclassable import BaseSubclassable
+from orwynn.base.model.model import Model
+from orwynn.base.service.service import Service
+from orwynn.utils.basesubclassable import BaseSubclassable
 
 # Note that here listed the most basic classes. E.g. Config is not listed
 # since it is a derivative from the Model and on the stage of DI
 # it will be checked to find these more specific classes.
 SUBCLASSABLES: list[BaseSubclassable] = [
     Service,
     Controller,
     Middleware,
     Model,
     ErrorHandler
 ]
+
+ENVIRONS: set[str] = {
+    "ORWYNN_MODE",
+    "ORWYNN_ROOT_DIR",
+    "ORWYNN_APPRC_PATH",
+    "ORWYNN_IS_CATCH_LOGGING_ENABLED_IN_TESTS"
+}
+"""
+All environment variables the framework supports.
+"""
```

### Comparing `orwynn-1.0.0b4/orwynn/helpers/web.py` & `orwynn-1.0.0b5/orwynn/helpers/web.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # A request of any supported protocol
 from enum import Enum
 from typing import TYPE_CHECKING, Union
 
-from orwynn.utils.Protocol import Protocol
+from orwynn.utils.protocol import Protocol
 
 if TYPE_CHECKING:
     from orwynn.http import HttpRequest, HttpResponse
     from orwynn.websocket import Websocket
 
 
 GenericRequest = Union[
```

### Comparing `orwynn-1.0.0b4/orwynn/http/_context/ContextBuiltinMiddleware.py` & `orwynn-1.0.0b5/orwynn/http/context/middleware/builtin.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from orwynn.context._context_manager import context_manager
-from orwynn.http._middleware.BuiltinHttpMiddleware import BuiltinHttpMiddleware
-from orwynn.http._middleware.HttpNextCall import HttpNextCall
-from orwynn.http._requests import HttpRequest
-from orwynn.http._responses import HttpResponse
+from orwynn.context.manager import context_manager
+from orwynn.http.middleware.builtinmiddleware import BuiltinHttpMiddleware
+from orwynn.http.middleware.nextcall import HttpNextCall
+from orwynn.http.requests import HttpRequest
+from orwynn.http.responses import HttpResponse
 
 
 class ContextBuiltinMiddleware(BuiltinHttpMiddleware):
     """
     Creates a shared context storage active within applied request-response
     cycle.
     """
```

### Comparing `orwynn-1.0.0b4/orwynn/http/_context/HttpRequestContextBuiltinMiddleware.py` & `orwynn-1.0.0b5/orwynn/http/context/middleware/contextbuiltin.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from orwynn.http._context.HttpRequestContextId import HttpRequestContextId
-from orwynn.http._middleware.BuiltinHttpMiddleware import BuiltinHttpMiddleware
-from orwynn.http._middleware.HttpNextCall import HttpNextCall
-from orwynn.http._requests import HttpRequest
-from orwynn.http._responses import HttpResponse
+from orwynn.http.context.id import HttpRequestContextId
+from orwynn.http.middleware.builtinmiddleware import BuiltinHttpMiddleware
+from orwynn.http.middleware.nextcall import HttpNextCall
+from orwynn.http.requests import HttpRequest
+from orwynn.http.responses import HttpResponse
 from orwynn.log import Log
 
 
 class HttpRequestContextBuiltinMiddleware(BuiltinHttpMiddleware):
     """Populates the context storage with the current request's id."""
     async def process(
         self, request: HttpRequest, call_next: HttpNextCall
```

### Comparing `orwynn-1.0.0b4/orwynn/http/_context/HttpRequestContextId.py` & `orwynn-1.0.0b5/orwynn/http/context/id.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b4/orwynn/http/_controller/HttpController.py` & `orwynn-1.0.0b5/orwynn/http/controller/controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from typing import Callable, ClassVar, Literal
 
 from orwynn.helpers.web import REQUEST_METHOD_BY_PROTOCOL, RequestMethod
 
-from .endpoint.Endpoint import Endpoint
-from orwynn.base.controller._Controller import Controller
-from orwynn.utils.Protocol import Protocol
+from .endpoint.endpoint import Endpoint
+from orwynn.base.controller.controller import Controller
+from orwynn.utils.protocol import Protocol
 from orwynn.http.errors import UnsupportedHttpMethodError
 from .errors import \
     DefinedTwiceControllerMethodError
 from orwynn.base.controller.errors import \
     MissingControllerClassAttributeError
-from .endpoint.EndpointContainer import EndpointContainer
+from .endpoint.container import EndpointContainer
 from orwynn.utils import validation
 
 
 class HttpController(Controller):
     """Handles incoming requests and returns responses to the client.
 
     Calls service or different services under the hood to prepare a response.
```

### Comparing `orwynn-1.0.0b4/orwynn/http/_controller/endpoint/Endpoint.py` & `orwynn-1.0.0b5/orwynn/http/controller/endpoint/endpoint.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from orwynn.base.model import Model
 
-from .EndpointResponse import EndpointResponse
+from .response import EndpointResponse
 
 
 class Endpoint(Model):
     """Specification of endpoint.
 
     Attributes:
         method:
```

### Comparing `orwynn-1.0.0b4/orwynn/http/_controller/endpoint/EndpointContainer.py` & `orwynn-1.0.0b5/orwynn/http/controller/endpoint/container.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Callable, ItemsView
 
 from orwynn.base.worker import Worker
 from orwynn.http.errors import EndpointNotFoundError
 from orwynn.utils import validation
 
-from .Endpoint import Endpoint
+from .endpoint import Endpoint
 
 
 class EndpointContainer(Worker):
     """Collects endpoint specs to be used on routes registering."""
     def __init__(self) -> None:
         super().__init__()
         self.__spec_by_fn: dict[Callable, Endpoint] = {}
```

### Comparing `orwynn-1.0.0b4/orwynn/http/_controller/endpoint/endpoint_test.py` & `orwynn-1.0.0b5/orwynn/http/controller/endpoint/test_main.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from pytest import fixture
 
 from orwynn import mongo
-from orwynn.base.model._Model import Model
-from orwynn.base.module._Module import Module
-from orwynn.boot._Boot import Boot
+from orwynn.base.model.model import Model
+from orwynn.base.module.module import Module
+from orwynn.boot.boot import Boot
 from orwynn.http import Endpoint, EndpointResponse, HttpController
 from orwynn.router.errors import (
     UnmatchedEndpointEntityError,
 )
 from orwynn.utils import validation
```

### Comparing `orwynn-1.0.0b4/orwynn/http/_controller/http_controller_test.py` & `orwynn-1.0.0b5/orwynn/http/controller/test_main.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 
 from fastapi import Query, Request
 
-from orwynn._di.Di import Di
 from orwynn.apiversion import ApiVersion
 from orwynn.base.controller.errors import (
     AlreadyRegisteredMethodError,
     MissingControllerClassAttributeError,
 )
 from orwynn.base.model import Model
 from orwynn.base.module import Module
 from orwynn.boot import Boot
+from orwynn.di.di import Di
 from orwynn.helpers.web import REQUEST_METHOD_BY_PROTOCOL
 from orwynn.http import Endpoint, HttpController
-from orwynn.http._controller.errors import DefinedTwiceControllerMethodError
+from orwynn.http.controller.errors import DefinedTwiceControllerMethodError
 from orwynn.http.errors import HttpException, UnsupportedHttpMethodError
-from orwynn.proxy.BootProxy import BootProxy
+from orwynn.proxy.boot import BootProxy
 from orwynn.testing import Client
 from orwynn.utils import validation
-from orwynn.utils.Protocol import Protocol
+from orwynn.utils.protocol import Protocol
 from orwynn.utils.validation import expect, validate_re
 from orwynn.utils.validation.errors import (
     RequestValidationException,
     ReValidationError,
     ValidationError,
 )
 from tests.std.text import DEFAULT_ID, Text
```

### Comparing `orwynn-1.0.0b4/orwynn/http/_errorhandler/ErrorHandlerHttpMiddleware.py` & `orwynn-1.0.0b5/orwynn/http/errorhandler/middleware.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from orwynn.base.errorhandler._ErrorHandler import ErrorHandler
-from orwynn.http._middleware.BuiltinHttpMiddleware import BuiltinHttpMiddleware
-from orwynn.http._middleware.HttpNextCall import HttpNextCall
-from orwynn.http._requests import HttpRequest
-from orwynn.http._responses import HttpResponse
+from orwynn.base.errorhandler.errorhandler import ErrorHandler
+from orwynn.http.middleware.builtinmiddleware import BuiltinHttpMiddleware
+from orwynn.http.middleware.nextcall import HttpNextCall
+from orwynn.http.requests import HttpRequest
+from orwynn.http.responses import HttpResponse
 from orwynn.utils import validation
 
 
 class ErrorHandlerHttpMiddleware(BuiltinHttpMiddleware):
     """
     Handles all errors occured at Http layer.
     """
```

### Comparing `orwynn-1.0.0b4/orwynn/http/_errorhandler/default.py` & `orwynn-1.0.0b5/orwynn/http/errorhandler/default.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from orwynn.base.errorhandler import ErrorHandler
-from orwynn.http._requests import HttpRequest
-from orwynn.http._responses import HttpResponse, JsonHttpResponse
 from orwynn.http.errors import HttpException
-from orwynn.proxy.BootProxy import BootProxy
+from orwynn.http.requests import HttpRequest
+from orwynn.http.responses import HttpResponse, JsonHttpResponse
+from orwynn.proxy.boot import BootProxy
 from orwynn.utils.validation.errors import RequestValidationException
 
 
 class DefaultRequestValidationErrorHandler(ErrorHandler):
     E = RequestValidationException
 
     def handle(
```

### Comparing `orwynn-1.0.0b4/orwynn/http/_errorhandler/error_handler_test.py` & `orwynn-1.0.0b5/orwynn/http/errorhandler/test_main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-from orwynn._testingtools import Item
-from orwynn.base.error import ExceptionAlreadyHandledError
+from orwynn.base.error.errors import ExceptionAlreadyHandledError
 from orwynn.base.errorhandler import ErrorHandler
 from orwynn.base.module import Module
-from orwynn.base.service._Service import Service
-from orwynn.boot._Boot import Boot
-from orwynn.http._context.HttpRequestContextBuiltinMiddleware import (
+from orwynn.base.service.service import Service
+from orwynn.boot.boot import Boot
+from orwynn.http.context.middleware.contextbuiltin import (
     HttpRequestContextBuiltinMiddleware,
 )
-from orwynn.http._controller.endpoint.Endpoint import Endpoint
-from orwynn.http._controller.HttpController import HttpController
-from orwynn.http._middleware.HttpMiddleware import HttpMiddleware
-from orwynn.http._middleware.HttpNextCall import HttpNextCall
-from orwynn.http._requests import HttpRequest
-from orwynn.http._responses import (
+from orwynn.http.controller.controller import HttpController
+from orwynn.http.controller.endpoint.endpoint import Endpoint
+from orwynn.http.middleware.middleware import HttpMiddleware
+from orwynn.http.middleware.nextcall import HttpNextCall
+from orwynn.http.requests import HttpRequest
+from orwynn.http.responses import (
     HttpResponse,
     JsonHttpResponse,
     TestHttpResponse,
 )
-from orwynn.proxy.BootProxy import BootProxy
+from orwynn.proxy.boot import BootProxy
 from orwynn.testing import Client
+from orwynn.testingtools import Item
 from orwynn.utils import validation
 
 
 class GeneralEh(ErrorHandler):
     E = Exception
 
     def handle(
```

### Comparing `orwynn-1.0.0b4/orwynn/http/_log/HttpLogger.py` & `orwynn-1.0.0b5/orwynn/http/log/logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import contextlib
 import json
 
 from starlette.concurrency import iterate_in_threadpool
 from starlette.responses import StreamingResponse
 
 from orwynn.base.error import MalfunctionError
-from orwynn.http._requests import HttpRequest
-from orwynn.http._responses import HttpResponse
+from orwynn.http.requests import HttpRequest
+from orwynn.http.responses import HttpResponse
 from orwynn.log import Log
 from orwynn.utils import validation
 
 
 class HttpLogger:
     """Logs HTTP requests and responses."""
     async def log_request(
```

### Comparing `orwynn-1.0.0b4/orwynn/http/_log/LogMiddleware.py` & `orwynn-1.0.0b5/orwynn/http/log/middleware.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from orwynn.http._context.HttpRequestContextId import HttpRequestContextId
-from orwynn.http._log.HttpLogger import HttpLogger
-from orwynn.http._middleware.HttpMiddleware import HttpMiddleware
-from orwynn.http._middleware.HttpNextCall import HttpNextCall
-from orwynn.http._requests import HttpRequest
-from orwynn.http._responses import HttpResponse
+from orwynn.http.context.id import HttpRequestContextId
+from orwynn.http.log.logger import HttpLogger
+from orwynn.http.middleware.middleware import HttpMiddleware
+from orwynn.http.middleware.nextcall import HttpNextCall
+from orwynn.http.requests import HttpRequest
+from orwynn.http.responses import HttpResponse
 
 
 class LogMiddleware(HttpMiddleware):
     """Logs information about request and response lihking them together.
 
     It's recommended to be outermost (at custom level) middleware.
     """
```

### Comparing `orwynn-1.0.0b4/orwynn/http/_middleware/HttpMiddleware.py` & `orwynn-1.0.0b5/orwynn/http/middleware/middleware.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from orwynn.base.middleware import Middleware
-from orwynn.http._middleware.HttpNextCall import HttpNextCall
-from orwynn.http._requests import HttpRequest
-from orwynn.http._responses import HttpResponse
+from orwynn.http.middleware.nextcall import HttpNextCall
+from orwynn.http.requests import HttpRequest
+from orwynn.http.responses import HttpResponse
 
 
 class HttpMiddleware(Middleware):
     """Intermediate operational layer for HTTP requests."""
     async def dispatch(
         self,
         request: HttpRequest,
```

### Comparing `orwynn-1.0.0b4/orwynn/http/_middleware/http_middleware_test.py` & `orwynn-1.0.0b5/orwynn/http/middleware/test_main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from typing import Callable
 
-from orwynn.base.module._Module import Module
-from orwynn.boot._Boot import Boot
+from orwynn.base.module.module import Module
+from orwynn.boot.boot import Boot
 from orwynn.http import (
     Endpoint,
     HttpController,
     HttpMiddleware,
     HttpRequest,
     HttpResponse,
     TestHttpResponse,
 )
-from orwynn.testing._Client import Client
+from orwynn.testing.client import Client
 
 
 class Mw1(HttpMiddleware):
     async def process(
         self, request: HttpRequest, call_next: Callable
     ) -> HttpResponse:
         response: HttpResponse = await call_next(request)
```

### Comparing `orwynn-1.0.0b4/orwynn/http/_responses.py` & `orwynn-1.0.0b5/orwynn/http/responses.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b4/orwynn/http/responses_test.py` & `orwynn-1.0.0b5/orwynn/http/test_responses.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from orwynn.base import Module
 from orwynn.boot import Boot
 from orwynn.http import Endpoint, HttpController
-from orwynn.http._log.LogMiddleware import LogMiddleware
-from orwynn.http._responses import RedirectHttpResponse, TestHttpResponse
+from orwynn.http.log.middleware import LogMiddleware
+from orwynn.http.responses import RedirectHttpResponse, TestHttpResponse
 
 
 def test_redirect():
     class LocalController(HttpController):
         ROUTE = "/"
         ENDPOINTS = [
             Endpoint(
```

### Comparing `orwynn-1.0.0b4/orwynn/indication/_Indication.py` & `orwynn-1.0.0b5/orwynn/indication/indication.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 from enum import Enum
 import json
 from typing import Any, ItemsView
 
 from orwynn.base.error import get_error_code, ErrorCode
 from orwynn.base.error import ErrorValueSchema
-from orwynn.base.model._Model import Model
-from orwynn.http._schema.HttpExceptionValueSchema import \
+from orwynn.base.model.model import Model
+from orwynn.http.schema.value import \
     HttpExceptionValueSchema
-from orwynn.http._schema.RequestValidationExceptionValueSchema import \
+from orwynn.http.schema.validationvalue import \
     RequestValidationExceptionValueSchema
 from orwynn.http.errors import HttpException
-from orwynn.indication._IndicationType import IndicationType
+from orwynn.indication.type import IndicationType
 from orwynn.indication.errors import UnsupportedIndicatorError
 from orwynn.utils import validation
 from orwynn.utils.mp.location import (FieldLocation, find_field_by_location,
                                      find_location_by_field)
 from orwynn.utils.validation import (validate,
                                     validate_dict)
 from orwynn.utils.validation.errors import RequestValidationException
-from orwynn.utils.validation._validator import Validator
+from orwynn.utils.validation.validator import Validator
 
-from ._Indicatable import Indicatable, IndicatableTypeVar
-from ._Indicator import Indicator
+from .indicatable import Indicatable, IndicatableTypeVar
+from .indicator import Indicator
 
 _Locations = dict[Indicator, FieldLocation]
 
 
 class Indication:
     """Holds some representation of how the data should be built like to serve
     as an convention for building objects.
@@ -163,15 +163,15 @@
                         final_field = {
                             "message": message,
                             "locations": locations
                         }
                     elif isinstance(obj, Exception):
                         final_field = {
                             "message": " ;; ".join([str(x) for x in obj.args]),
-                            "error_code": self.__get_final_error_code(
+                            "code": self.__get_final_error_code(
                                 obj
                             )
                         }
                     elif isinstance(obj, Model):
                         # Since pydantic seems to not having a way to deal
                         # with Enums through dict() call (only via Config),
                         # here we do not performance good operation of
```

### Comparing `orwynn-1.0.0b4/orwynn/indication/indication_test.py` & `orwynn-1.0.0b5/orwynn/indication/test_main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from enum import Enum
 from typing import Any
 
 from pytest import fixture
 
-from orwynn.base.model._Model import Model
-from orwynn.indication._Indication import Indication
-from orwynn.indication._Indicator import Indicator
+from orwynn.base.model.model import Model
+from orwynn.indication.indication import Indication
+from orwynn.indication.indicator import Indicator
 from orwynn.utils import validation
 from tests.std.text import Text
 
 
 @fixture
 def default_indication() -> Indication:
     mp: dict[str, Indicator] = {
@@ -110,23 +110,23 @@
         CODE = "hello"
 
     data: dict
 
     data = default_indication.digest(SimpleError("hello world"))
     assert data["type"] == "error"
     assert data["value"]["message"] == "hello world"
-    assert data["value"]["error_code"] == ErrorCode.SIMPLE_CASE.value
+    assert data["value"]["code"] == ErrorCode.SIMPLE_CASE.value
 
     data = default_indication.digest(AdvancedError("hello world"))
     assert data["type"] == "error"
     assert data["value"]["message"] == "hello world"
-    assert data["value"]["error_code"] == ErrorCode.ADVANCED_CASE.value
+    assert data["value"]["code"] == ErrorCode.ADVANCED_CASE.value
 
     data = default_indication.digest(IntError("hello world"))
     assert data["type"] == "error"
     assert data["value"]["message"] == "hello world"
-    assert data["value"]["error_code"] == 5
+    assert data["value"]["code"] == 5
 
     data = default_indication.digest(StrError("hello world"))
     assert data["type"] == "error"
     assert data["value"]["message"] == "hello world"
-    assert data["value"]["error_code"] == "hello"
+    assert data["value"]["code"] == "hello"
```

### Comparing `orwynn-1.0.0b4/orwynn/log/_configure_log.py` & `orwynn-1.0.0b5/orwynn/log/configure.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import sys
 from typing import TYPE_CHECKING, Any
-from orwynn.log._Log import Log
-from orwynn.log._LogConfig import LogConfig
-from orwynn.log._LogHandler import LogHandler
-from orwynn.proxy.BootProxy import BootProxy
+from orwynn.log.log import Log
+from orwynn.log.config import LogConfig
+from orwynn.log.handler import LogHandler
+from orwynn.proxy.boot import BootProxy
 
 if TYPE_CHECKING:
     from orwynn.app import AppMode
 
 
 def configure_log(config: LogConfig, *, app_mode_prod: "AppMode") -> None:
     if config.handlers:
@@ -25,17 +25,17 @@
         Added handler number.
     """
     sink: Any
     if isinstance(handler.sink, str):
         # For apprc-based configuration parse some string literals into
         # actual objects.
         match handler.sink:
-            case "stdout":
+            case "$stdout":
                 sink = sys.stdout
-            case "stderr":
+            case "$stderr":
                 sink = sys.stderr
             case _:
                 # For all other string cases consider the sink as a file
                 # path
                 sink = handler.sink
     else:
         # the sink is given directly to the method as a python object,
```

### Comparing `orwynn-1.0.0b4/orwynn/log/helpers.py` & `orwynn-1.0.0b5/orwynn/log/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import contextlib
 
-from orwynn.log._Log import Log
+from orwynn.log.log import Log
 
 
 def catch_error(error: Exception):
     """Reraise error and catch it by logger."""
     # TODO: Find way to remove this last function from exception stack to not
     #   be displayed
```

### Comparing `orwynn-1.0.0b4/orwynn/log/log_middleware_test.py` & `orwynn-1.0.0b5/orwynn/log/test_middleware.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import json
 from types import NoneType
 from typing import Literal
 
-from orwynn.base.module._Module import Module
-from orwynn.boot._Boot import Boot
+from orwynn.base.module.module import Module
+from orwynn.boot.boot import Boot
 from orwynn.http import Endpoint, HttpController, LogMiddleware
-from orwynn.log._Log import Log
-from orwynn.proxy.BootProxy import BootProxy
+from orwynn.log.log import Log
+from orwynn.proxy.boot import BootProxy
 from orwynn.testing import Writer
-from orwynn.testing._Client import Client
+from orwynn.testing.client import Client
 
 
 def __check_log_message(message: str) -> list[dict]:
     assert message != ""
     items: list[str] = message.split("\n")
     parsed_items: list[dict] = []
```

### Comparing `orwynn-1.0.0b4/orwynn/log/log_test.py` & `orwynn-1.0.0b5/orwynn/log/test_main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import json
 
 import pytest
-from loguru._handler import Message
 
-from orwynn.base.module._Module import Module
-from orwynn.boot._Boot import Boot
+from orwynn.base.module.module import Module
+from orwynn.boot.boot import Boot
 from orwynn.http import Endpoint, HttpController
-from orwynn.log._Log import Log
+from orwynn.log.log import Log
+from orwynn.log.types import LogMessage
 from orwynn.testing import Writer, get_log_apprc
 from orwynn.websocket import Websocket, WebsocketController
 
 
 @pytest.fixture
 def writer() -> Writer:
     return Writer()
 
 
 @pytest.fixture
 def log_apprc_sink_to_writer(writer: Writer) -> dict:
-    def __check(message: Message):
+    def __check(message: LogMessage) -> None:
         writer.write(message)
     return get_log_apprc(__check)
 
 
 def test_logged_request_id(writer: Writer, log_apprc_sink_to_writer: dict):
     class C1(HttpController):
         ROUTE = "/"
@@ -33,15 +33,15 @@
         def get(self) -> dict:
             Log.info("hello")
             return {}
 
     boot: Boot = Boot(
         Module("/", Controllers=[C1]),
         apprc=log_apprc_sink_to_writer
-    )  # type: ignore #worker
+    )
 
     boot.app.client.get("/", 200)
     data: dict = json.loads(str(writer.read()))
     extra: dict = data["record"]["extra"]
 
     assert isinstance(extra["http.request_id"], str)
```

### Comparing `orwynn-1.0.0b4/orwynn/log/log_websocket_middleware_test.py` & `orwynn-1.0.0b5/orwynn/log/test_websocketmiddleware.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import json
 
-from orwynn.base.module._Module import Module
-from orwynn.boot._Boot import Boot
-from orwynn.log._Log import Log
+from orwynn.base.module.module import Module
+from orwynn.boot.boot import Boot
+from orwynn.log.log import Log
 from orwynn.testing import Writer
-from orwynn.testing._Client import Client
+from orwynn.testing.client import Client
 from orwynn.websocket import Websocket, WebsocketController
-from orwynn.websocket._log.LogWebsocketMiddleware import LogWebsocketMiddleware
+from orwynn.websocket.log.middleware import LogWebsocketMiddleware
 
 
 def test_get(
     writer: Writer,
     log_apprc_sink_to_writer: dict
 ):
     class C1(WebsocketController):
```

### Comparing `orwynn-1.0.0b4/orwynn/mapping/_Mapping.py` & `orwynn-1.0.0b5/orwynn/mapping/mapping.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import typing
 from typing import Any
 
-from orwynn.base.model._Model import Model
+from orwynn.base.model.model import Model
 from orwynn.mapping.errors import MappingNotLinkedError
 from orwynn.utils.types import DecoratedCallable
 
 
 def if_linked(
     fn: DecoratedCallable
 ) -> DecoratedCallable:
```

### Comparing `orwynn-1.0.0b4/orwynn/mongo/_Document.py` & `orwynn-1.0.0b5/orwynn/mongo/document.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,24 +2,24 @@
 from typing import Any, Iterable, Self
 
 from bson import ObjectId
 from pydantic.fields import ModelField
 from pymongo.cursor import Cursor
 from pymongo.errors import DuplicateKeyError as PymongoDuplicateKeyError
 
-from orwynn._di.Di import Di
-from orwynn.mapping._Mapping import Mapping, if_linked
+from orwynn.di.di import Di
 from orwynn.mapping.errors import CustomUseOfMappingReservedFieldError
-from orwynn.mongo._Mongo import Mongo
-from orwynn.mongo._MongoEntity import MongoEntity
+from orwynn.mapping.mapping import Mapping, if_linked
+from orwynn.mongo.entity import MongoEntity
 from orwynn.mongo.errors import DuplicateKeyError
+from orwynn.mongo.mongo import Mongo
 from orwynn.utils import validation
 from orwynn.utils.fmt import snakefy
 
-from ._ClientSession import ClientSession
+from .clientsession import ClientSession
 from .errors import DocumentUpdateError
 
 
 class Document(Mapping):
     """Mapping to work with MongoDB.
 
     Itself is some model representing MongoDB document and also has some class
```

### Comparing `orwynn-1.0.0b4/orwynn/mongo/_Mongo.py` & `orwynn-1.0.0b5/orwynn/mongo/mongo.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from pymongo import MongoClient, ReturnDocument
 from pymongo.client_session import ClientSession
 from pymongo.cursor import Cursor
 from pymongo.database import Database as PymongoDatabase
 
 from orwynn.base.database import Database
 from orwynn.base.database.errors import DatabaseEntityNotFoundError
-from orwynn.mongo._MongoConfig import MongoConfig
-from orwynn.mongo._MongoEntity import MongoEntity
+from orwynn.mongo.config import MongoConfig
+from orwynn.mongo.entity import MongoEntity
 from orwynn.utils import validation
 
 
 class Mongo(Database):
     """Manages actions related to MongoDB."""
     def __init__(self, config: MongoConfig) -> None:
         self.__client: MongoClient = MongoClient(config.uri)
```

### Comparing `orwynn-1.0.0b4/orwynn/mongo/document_test.py` & `orwynn-1.0.0b5/orwynn/mongo/test_document.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from pytest import fixture
 
 from orwynn import mongo
 from orwynn.base.module import Module
-from orwynn.boot._Boot import Boot
+from orwynn.boot.boot import Boot
 from orwynn.utils import validation
 
-from ._Document import Document
+from .document import Document
 from .errors import DocumentUpdateError
 
 
 class Item(Document):
     name: str
     price: float
     priority: int = 5
```

### Comparing `orwynn-1.0.0b4/orwynn/mongo/mongo_test.py` & `orwynn-1.0.0b5/orwynn/mongo/test_main.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from orwynn.http import TestHttpResponse
 from orwynn.mapping.errors import CustomUseOfMappingReservedFieldError
-from orwynn.mongo._Document import Document
+from orwynn.mongo.document import Document
 from orwynn.mongo.errors import DuplicateKeyError
-from orwynn.proxy.BootProxy import BootProxy
-from orwynn.testing._Client import Client
+from orwynn.proxy.boot import BootProxy
+from orwynn.testing.client import Client
 from orwynn.utils import validation
 from tests.std.user import User
 
 
 def test_user_create(std_mongo_boot, std_http: Client):
     r: TestHttpResponse = std_http.post(
         "/users",
```

### Comparing `orwynn-1.0.0b4/orwynn/proxy/BootProxy.py` & `orwynn-1.0.0b5/orwynn/proxy/boot.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from pathlib import Path
 from typing import TYPE_CHECKING
 
 from orwynn.base.worker import Worker
-from orwynn.utils.Protocol import Protocol
+from orwynn.utils.protocol import Protocol
 
 if TYPE_CHECKING:
     from orwynn.apiversion import ApiVersion
     from orwynn.app import AppMode
     from orwynn.apprc import AppRc
-    from orwynn.base.errorhandler._ErrorHandler import ErrorHandler
-    from orwynn.indication._Indication import Indication
+    from orwynn.base.errorhandler.errorhandler import ErrorHandler
+    from orwynn.indication.indication import Indication
 
 
 class BootProxy(Worker):
     """Proxy data to prevent DI importing Boot worker directly (and avoid
     circular imports by this) to build BootConfig.
     """
     def __init__(
```

### Comparing `orwynn-1.0.0b4/orwynn/router/_ControllerRegister.py` & `orwynn-1.0.0b5/orwynn/router/register/controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,32 +2,32 @@
 from inspect import isclass
 from typing import Any, Callable, Literal
 
 import pydantic
 
 from orwynn.apiversion import ApiVersion
 from orwynn.app import App
-from orwynn.base.controller._Controller import Controller
+from orwynn.base.controller.controller import Controller
 from orwynn.base.controller.errors import AlreadyRegisteredMethodError
 from orwynn.base.error import MalfunctionError
 from orwynn.base.model import Model
 from orwynn.base.module import Module
 from orwynn.helpers.web import REQUEST_METHOD_BY_PROTOCOL, RequestMethod
 from orwynn.http import Endpoint, EndpointContainer, HttpController
 from orwynn.http.errors import (
     EndpointNotFoundError,
     UnsupportedHttpMethodError,
 )
-from orwynn.indication._Indication import Indication
-from orwynn.proxy.BootProxy import BootProxy
+from orwynn.indication.indication import Indication
+from orwynn.proxy.boot import BootProxy
 from orwynn.router.errors import (
     UnmatchedEndpointEntityError,
 )
 from orwynn.utils import validation
-from orwynn.utils.Protocol import Protocol
+from orwynn.utils.protocol import Protocol
 from orwynn.utils.url import join_routes
 from orwynn.websocket import (
     WebsocketController,
     WebsocketStack,
     routing_handlers,
 )
```

### Comparing `orwynn-1.0.0b4/orwynn/router/_ErrorHandlerManager.py` & `orwynn-1.0.0b5/orwynn/router/errorhandlermanager.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from orwynn.base.error import (ExceptionAlreadyHandledError,
-                               MalfunctionError)
+from orwynn.base.error.errors import (ExceptionAlreadyHandledError,
+                                      MalfunctionError)
 from orwynn.base.errorhandler import ErrorHandler
 from orwynn.http import DEFAULT_HTTP_ERROR_HANDLERS
-from orwynn.utils.Protocol import Protocol
+from orwynn.utils.protocol import Protocol
 from orwynn.websocket import DEFAULT_WEBSOCKET_EXCEPTION_HANDLERS
 
 
 class ErrorHandlerManager:
     """
     Controls the error flow setup for the system.
```

### Comparing `orwynn-1.0.0b4/orwynn/router/_MiddlewareRegister.py` & `orwynn-1.0.0b5/orwynn/router/register/middleware.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,29 @@
-from typing import Any, Callable, Sequence
+from typing import Callable, Sequence
 
-from fastapi.middleware.cors import CORSMiddleware as FastAPI_CORSMiddleware
 from starlette.middleware.base import (
     BaseHTTPMiddleware as StarletteBaseHTTPMiddleware,
 )
 
 from orwynn.app import App
-from orwynn.base.error import get_exception_direct_subclasses
+from orwynn.base.error.utils import get_exception_direct_subclasses
 from orwynn.base.errorhandler import ErrorHandler
 from orwynn.base.middleware import Middleware
 from orwynn.http import (
     BUILTIN_HTTP_MIDDLEWARE,
     BuiltinHttpMiddleware,
-    Cors,
     DefaultErrorHandler,
     DefaultHttpErrorHandler,
     ErrorHandlerHttpMiddleware,
     HttpMiddleware,
 )
 from orwynn.http.errors import HttpException
-from orwynn.router._ErrorHandlerManager import ErrorHandlerManager
+from orwynn.router.errorhandlermanager import ErrorHandlerManager
 from orwynn.utils import validation
-from orwynn.utils.Protocol import Protocol
+from orwynn.utils.protocol import Protocol
 from orwynn.websocket import (
     BUILTIN_WEBSOCKET_MIDDLEWARE,
     BuiltinWebsocketMiddleware,
     ErrorHandlerWebsocketMiddleware,
     WebsocketMiddleware,
     WebsocketStack,
     routing_handlers,
@@ -41,25 +39,23 @@
     """
     def __init__(
         self,
         *,
         app: App,
         middleware_arr: list[Middleware],
         exception_handlers: list[ErrorHandler],
-        cors: Cors | None,
         websocket_stack: WebsocketStack,
     ) -> None:
         self.__app: App = app
 
         self.__middleware_arr: list[Middleware] = middleware_arr
         self.__exception_handlers: set[ErrorHandler] = set(
             exception_handlers
         )
 
-        self.__cors: Cors | None = cors
         self.__websocket_stack: WebsocketStack = websocket_stack
         self.__is_websocket_middleware_added: bool = False
 
     def register_all(self) -> None:
         """
         Registers all middleware to the system.
         """
@@ -163,17 +159,14 @@
                     " class Middleware"
                 )
             else:
                 raise TypeError(
                     f"unrecognized middleware {middleware}"
                 )
 
-        # Add CORS middleware first
-        self.__register_cors_middleware()
-
         # Add HTTP from reversed list to comply Starlette
         for http_middleware in reversed(http_middleware_arr):
             self.__register_middleware_unit(http_middleware)
 
         # Add Websocket normally
         if websocket_middleware_arr != []:
             if self.__is_websocket_middleware_added:
@@ -265,25 +258,7 @@
                 else:
                     handle_fn = DefaultErrorHandler()._fw_handle_wrapper
 
             self.__app._fw_register_exception_handler_fn(
                 Remaining,
                 handle_fn
             )
-
-    def __register_cors_middleware(self) -> None:
-        """
-        Configures CORS policy used for the whole app.
-        """
-        if self.__cors is None:
-            return
-        validation.validate(self.__cors, Cors)
-
-        kwargs: dict[str, Any] = {}
-        for k, v in self.__cors.dict().items():
-            if v:
-                kwargs[k] = v
-
-        self.__app._fw_register_middleware(
-            FastAPI_CORSMiddleware,
-            **kwargs
-        )
```

### Comparing `orwynn-1.0.0b4/orwynn/router/_Router.py` & `orwynn-1.0.0b5/orwynn/router/router.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,57 +1,52 @@
 from orwynn.apiversion import ApiVersion
-from orwynn.app._App import App
-from orwynn.base.controller._Controller import Controller
-from orwynn.base.errorhandler._ErrorHandler import ErrorHandler
+from orwynn.app.app import App
+from orwynn.base.controller.controller import Controller
+from orwynn.base.errorhandler.errorhandler import ErrorHandler
 from orwynn.base.middleware import Middleware
-from orwynn.base.module._Module import Module
-from orwynn.base.worker._Worker import Worker
-from orwynn.http import Cors
+from orwynn.base.module.module import Module
+from orwynn.base.worker.worker import Worker
 from orwynn.websocket import WebsocketStack
 
-from ._ControllerRegister import ControllerRegister
-from ._MiddlewareRegister import MiddlewareRegister
+from .register.controller import ControllerRegister
+from .register.middleware import MiddlewareRegister
 
 
 class Router(Worker):
     """
     Manages how the requests and responses flow through the app.
     """
     def __init__(
         self,
         app: App,
         *,
         modules: list[Module],
         controllers: list[Controller],
         middleware_arr: list[Middleware],
         exception_handlers: list[ErrorHandler],
-        cors: Cors | None,
         global_http_route: str,
         global_websocket_route: str,
         api_version: ApiVersion
     ) -> None:
         super().__init__()
         self.__app: App = app
 
         self.__modules: list[Module] = modules
         self.__controllers: list[Controller] = controllers
         self.__middleware_arr: list[Middleware] = middleware_arr
         self.__exception_handlers: list[ErrorHandler] = exception_handlers
 
-        self.__cors: Cors | None = cors
-
         self.__websocket_stack: WebsocketStack = WebsocketStack(
             self.__app._fw_websocket_handler
         )
 
         self.__middleware_register: MiddlewareRegister = MiddlewareRegister(
             app=self.__app,
             middleware_arr=self.__middleware_arr,
             exception_handlers=self.__exception_handlers,
-            cors=self.__cors,
             websocket_stack=self.__websocket_stack
         )
         self.__controller_register: ControllerRegister = ControllerRegister(
             app=self.__app,
             modules=self.__modules,
             controllers=self.__controllers,
             websocket_stack=self.__websocket_stack,
```

### Comparing `orwynn-1.0.0b4/orwynn/router/global_http_route_test.py` & `orwynn-1.0.0b5/orwynn/router/test_globalroute.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b4/orwynn/singleton/_Singleton.py` & `orwynn-1.0.0b5/orwynn/singleton/singleton.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from __future__ import annotations
 
 import contextlib
-from typing import TypeVar
+from typing import Any, TypeVar
 
 SingletonInstance = TypeVar("SingletonInstance")
 
 
 class SingletonMeta(type):
     """Singleton metaclass for implementing singleton patterns.
 
     See:
         https://stackoverflow.com/questions/6760685/creating-a-singleton-in-python
     """
     __instances: dict[type, object] = {}
 
-    def __call__(cls, *args, **kwargs):
+    def __call__(cls, *args, **kwargs) -> Any:
         if cls not in cls.__instances:
             cls.__instances[cls] = super().__call__(*args, **kwargs)
         return cls.__instances[cls]
 
     def __validate_in_instances(cls, cannot_message: str) -> None:
         if cls not in cls.__instances.keys():
             raise ValueError(
```

### Comparing `orwynn-1.0.0b4/orwynn/sql/_Sql.py` & `orwynn-1.0.0b5/orwynn/sql/sql.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from pathlib import Path
 from typing import Optional, Sequence
 from orwynn.utils import validation
-from orwynn.base.database._Database import Database
+from orwynn.base.database.database import Database
 
-from ._Table import Table
+from .table import Table
 
-from ._SqlDatabaseKind import SQLDatabaseKind
+from .databasekind import SQLDatabaseKind
 
-from orwynn.sql._SqlConfig import SqlConfig
+from orwynn.sql.config import SqlConfig
 from sqlalchemy import create_engine, Engine
 from sqlalchemy import Table as SQLAlchemyTable
 from sqlalchemy.orm import Session
 
 
 class Sql(Database):
     def __init__(
```

### Comparing `orwynn-1.0.0b4/orwynn/sql/_SqlConfig.py` & `orwynn-1.0.0b5/orwynn/sql/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Any
 
 from orwynn.base.config import Config
 from orwynn.base.error import MalfunctionError
 from sqlalchemy.pool import StaticPool, Pool
 
-from orwynn.sql._PoolclassStr import PoolclassStr
-from ._SqlDatabaseKind import SQLDatabaseKind
+from orwynn.sql.poolclass import PoolclassStr
+from .databasekind import SQLDatabaseKind
 
 
 class SqlConfig(Config):
     database_kind: SQLDatabaseKind
     database_name: str | None = None
     database_user: str | None = None
     database_password: str | None = None
```

### Comparing `orwynn-1.0.0b4/orwynn/sql/_Table.py` & `orwynn-1.0.0b5/orwynn/sql/table.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b4/orwynn/sql/sql_test.py` & `orwynn-1.0.0b5/orwynn/sql/test_main.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,18 +9,18 @@
 
 from orwynn import sql
 from orwynn.base.module import Module
 from orwynn.boot import Boot
 from orwynn.utils import validation
 from orwynn.utils.crypto import hash_password
 
-from ._Sql import Sql
-from ._SqlConfig import SqlConfig
-from ._SqlDatabaseKind import SQLDatabaseKind
-from ._Table import Table
+from .config import SqlConfig
+from .databasekind import SQLDatabaseKind
+from .sql import Sql
+from .table import Table
 
 
 class User(Table):
     name: Mapped[str]
     hpassword: Mapped[str]
     tweets: Mapped[list["Tweet"]] = relationship(backref="user")
     likes: Mapped[list["Like"]] = relationship(backref="user")
```

### Comparing `orwynn-1.0.0b4/orwynn/testing/_Client.py` & `orwynn-1.0.0b5/orwynn/testing/client.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 import inspect
 from types import NoneType
-from typing import Any, Callable, Optional, Self, TypeVar
+from typing import TYPE_CHECKING, Any, Callable, Optional, Self, TypeVar
 from orwynn.apiversion import ApiVersion
-from orwynn.base.model._Model import Model
-from orwynn.proxy.BootProxy import BootProxy
+from orwynn.base.model.model import Model
+from orwynn.proxy.boot import BootProxy
 
-from orwynn.testing._EmbeddedTestClient import EmbeddedTestClient
+from orwynn.testing.embeddedclient import EmbeddedTestClient
 from orwynn.utils import validation
 from orwynn.utils.validation import validate
-from orwynn.utils.Protocol import Protocol
-from orwynn.http import TestHttpResponse
+from orwynn.utils.protocol import Protocol
 from orwynn.utils.url import join_routes
 
+if TYPE_CHECKING:
+    from orwynn.http import TestHttpResponse
+
 # If ever you get to Python3.12, see if PEP 696 introduced, then apply
 # but for now it is in the next form
 _JsonifyExpectedType = TypeVar("_JsonifyExpectedType")
 
 
 class _FinalizedRequestData(Model):
     route: str
@@ -67,158 +69,162 @@
         self,
         url: str,
         asserted_status_code: int | None = None,
         *,
         expected_type: type[_JsonifyExpectedType] = dict,
         **kwargs
     ) -> _JsonifyExpectedType:
-        r: TestHttpResponse = self.get(url, asserted_status_code, **kwargs)
+        r: "TestHttpResponse" = self.get(url, asserted_status_code, **kwargs)
         data: Any = r.json()
         validate(data, expected_type)
         return data
 
     def post_jsonify(
         self,
         url: str,
         asserted_status_code: int | None = None,
         *,
         expected_type: type[_JsonifyExpectedType] = dict,
         **kwargs
     ) -> _JsonifyExpectedType:
-        r: TestHttpResponse = self.post(url, asserted_status_code, **kwargs)
+        r: "TestHttpResponse" = self.post(url, asserted_status_code, **kwargs)
         data: Any = r.json()
         validate(data, expected_type)
         return data
 
     def delete_jsonify(
         self,
         url: str,
         asserted_status_code: int | None = None,
         *,
         expected_type: type[_JsonifyExpectedType] = dict,
         **kwargs
     ) -> _JsonifyExpectedType:
-        r: TestHttpResponse = self.delete(url, asserted_status_code, **kwargs)
+        r: "TestHttpResponse" = self.delete(
+            url, asserted_status_code, **kwargs
+        )
         data: Any = r.json()
         validate(data, expected_type)
         return data
 
     def put_jsonify(
         self,
         url: str,
         asserted_status_code: int | None = None,
         *,
         expected_type: type[_JsonifyExpectedType] = dict,
         **kwargs
     ) -> _JsonifyExpectedType:
-        r: TestHttpResponse = self.put(url, asserted_status_code, **kwargs)
+        r: "TestHttpResponse" = self.put(url, asserted_status_code, **kwargs)
         data: Any = r.json()
         validate(data, expected_type)
         return data
 
     def patch_jsonify(
         self,
         url: str,
         asserted_status_code: int | None = None,
         *,
         expected_type: type[_JsonifyExpectedType] = dict,
         **kwargs
     ) -> _JsonifyExpectedType:
-        r: TestHttpResponse = self.patch(url, asserted_status_code, **kwargs)
+        r: "TestHttpResponse" = self.patch(url, asserted_status_code, **kwargs)
         data: Any = r.json()
         validate(data, expected_type)
         return data
 
     def options_jsonify(
         self,
         url: str,
         asserted_status_code: int | None = None,
         *,
         expected_type: type[_JsonifyExpectedType] = dict,
         **kwargs
     ) -> _JsonifyExpectedType:
-        r: TestHttpResponse = self.options(url, asserted_status_code, **kwargs)
+        r: "TestHttpResponse" = self.options(
+            url, asserted_status_code, **kwargs
+        )
         data: Any = r.json()
         validate(data, expected_type)
         return data
 
     def get(
         self,
         url: str,
         asserted_status_code: int | None = None,
         **kwargs
-    ) -> TestHttpResponse:
+    ) -> "TestHttpResponse":
         # Join method name and function to call inner resolver
         # inspect.stack() is for resolving self method name, ref:
         #   https://stackoverflow.com/a/5067654
         return self._get_test_response(
             inspect.stack(), url, asserted_status_code, **kwargs)
 
     def post(
         self,
         url: str,
         asserted_status_code: int | None = None,
         **kwargs
-    ) -> TestHttpResponse:
+    ) -> "TestHttpResponse":
         return self._get_test_response(
             inspect.stack(), url, asserted_status_code, **kwargs)
 
     def delete(
         self,
         url: str,
         asserted_status_code: int | None = None,
         **kwargs
-    ) -> TestHttpResponse:
+    ) -> "TestHttpResponse":
         return self._get_test_response(
             inspect.stack(), url, asserted_status_code, **kwargs)
 
     def put(
         self,
         url: str,
         asserted_status_code: int | None = None,
         **kwargs
-    ) -> TestHttpResponse:
+    ) -> "TestHttpResponse":
         return self._get_test_response(
             inspect.stack(), url, asserted_status_code, **kwargs)
 
     def patch(
         self,
         url: str,
         asserted_status_code: int | None = None,
         **kwargs
-    ) -> TestHttpResponse:
+    ) -> "TestHttpResponse":
         return self._get_test_response(
             inspect.stack(), url, asserted_status_code, **kwargs)
 
     def options(
         self,
         url: str,
         asserted_status_code: int | None = None,
         **kwargs
-    ) -> TestHttpResponse:
+    ) -> "TestHttpResponse":
         return self._get_test_response(
             inspect.stack(), url, asserted_status_code, **kwargs)
 
     def _get_test_response(
         self,
         stack: list[inspect.FrameInfo],
         url: str,
         asserted_status_code: int | None,
         **kwargs
-    ) -> TestHttpResponse:
+    ) -> "TestHttpResponse":
         request: str = " ".join([stack[0][3], url])
         return self._resolve_request(request, asserted_status_code, **kwargs)
 
     def _resolve_request(
         self,
         request: str,
         asserted_status_code: int | None,
         **request_kwargs
-    ) -> TestHttpResponse:
-        response: TestHttpResponse
+    ) -> "TestHttpResponse":
+        response: "TestHttpResponse"
         test_client_method: Callable
         method: str
         route: str
 
         validate(request, str)
         validate(asserted_status_code, [int, NoneType])
 
@@ -248,21 +254,19 @@
         finalized: _FinalizedRequestData = self._process_request_data(
             route=route,
             request_kwargs=request_kwargs,
             protocol=Protocol.HTTP
         )
 
         # Make a request
-        response: TestHttpResponse = test_client_method(
+        response: "TestHttpResponse" = test_client_method(
             finalized.route,
             **finalized.kwargs
         )
 
-        validate(response, TestHttpResponse, is_strict=True)
-
         if asserted_status_code is not None:
             assert \
                 response.status_code == asserted_status_code, \
                 f"response status code {response.status_code}" \
                 f" != asserted status code {asserted_status_code};" \
                 f" response content is {response.content}"
```

### Comparing `orwynn-1.0.0b4/orwynn/testing/__init__.py` & `orwynn-1.0.0b5/orwynn/testing/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Callable
 
-from ._Client import Client
-from ._EmbeddedTestClient import EmbeddedTestClient
+from .client import Client
+from .embeddedclient import EmbeddedTestClient
 
 
 def get_log_apprc(check_fn: Callable) -> dict:
     return {
         "prod": {
             "Log": {
                 "handlers": [
```

### Comparing `orwynn-1.0.0b4/orwynn/testing/client_test.py` & `orwynn-1.0.0b5/orwynn/testing/test_main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from fastapi import Header
 
-from orwynn._testingtools import HeadersGetController
-from orwynn.base.module._Module import Module
+from orwynn.base.module.module import Module
 from orwynn.boot import Boot
 from orwynn.http import Endpoint, HttpController
-from orwynn.testing._Client import Client
+from orwynn.testing.client import Client
+from orwynn.testingtools import HeadersGetController
 
 
 class _Ctrl1(HttpController):
     ROUTE = "/"
     ENDPOINTS = [
         Endpoint(method="get")
     ]
```

### Comparing `orwynn-1.0.0b4/orwynn/utils/crypto/__init__.py` & `orwynn-1.0.0b5/orwynn/utils/crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b4/orwynn/utils/fmt/__init__.py` & `orwynn-1.0.0b5/orwynn/utils/fmt/__init__.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b4/orwynn/utils/fmt/fmt_test.py` & `orwynn-1.0.0b5/orwynn/utils/fmt/test_main.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b4/orwynn/utils/klass/__init__.py` & `orwynn-1.0.0b5/orwynn/utils/klass/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import functools
 from typing import Any, Callable
 
 from orwynn.utils.types import Class
 
-from ._errors import ClassNotFoundError
+from .errors import ClassNotFoundError
 
 
 def find_subclass_by_name(name: str, BaseClass: Class) -> Class:
     """Searches given base class for subclass with given name.
 
     Args:
         name:
```

### Comparing `orwynn-1.0.0b4/orwynn/utils/klass/klass_test.py` & `orwynn-1.0.0b5/orwynn/utils/klass/test_klass.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b4/orwynn/utils/mp/__init__.py` & `orwynn-1.0.0b5/orwynn/utils/mp/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from copy import deepcopy
 from typing import Any
 
 import dictdiffer
 
 from orwynn.utils import validation
-from orwynn.utils.mp._dictpp import dictpp
+from orwynn.utils.mp.dictpp import dictpp
 
 
 def find(location: str, mp: dict) -> Any:
     """Finds field by location.
 
     Args:
         location:
```

### Comparing `orwynn-1.0.0b4/orwynn/utils/mp/location.py` & `orwynn-1.0.0b5/orwynn/utils/mp/location.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b4/orwynn/utils/mp/mp_test.py` & `orwynn-1.0.0b5/orwynn/utils/mp/test_main.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from orwynn.utils.mp import patch
-from orwynn.utils.mp._dictpp import dictpp
+from orwynn.utils.mp.dictpp import dictpp
 
 
 def test_patch():
     a = dictpp({
         "BurgerShot": {
             "location": "Vinewood",
             "employees": 15,
```

### Comparing `orwynn-1.0.0b4/orwynn/utils/url/__init__.py` & `orwynn-1.0.0b5/orwynn/utils/url/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """
 Works with url formatting.
 """
 from orwynn.utils import validation
-from orwynn.utils.url._match_routes import match_routes
+from orwynn.utils.url.utils import match_routes
 
-from ._get_vars import get_vars
-from ._Url import Url
-from ._UrlVars import UrlVars
+from .helpers import get_vars
+from .url import Url
+from .vars import UrlVars
 
 
 def join_routes(*routes: str) -> str:
     """Joins all given routes and normalize final result."""
     validation.validate_each(routes, str, expected_sequence_type=tuple)
 
     result: str = ""
```

### Comparing `orwynn-1.0.0b4/orwynn/utils/url/_get_vars.py` & `orwynn-1.0.0b5/orwynn/utils/url/helpers.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import re
 from itertools import zip_longest
 
-from orwynn.utils.url._match_routes import match_routes
-from orwynn.utils.url._Url import Url
-from orwynn.utils.url._UrlVars import UrlVars
+from orwynn.utils.url.url import Url
+from orwynn.utils.url.utils import match_routes
+from orwynn.utils.url.vars import UrlVars
 
 
 def get_vars(
     url: Url,
     *,
     abstract_route: str
 ) -> UrlVars:
```

### Comparing `orwynn-1.0.0b4/orwynn/utils/url/get_vars_test.py` & `orwynn-1.0.0b5/orwynn/utils/url/test_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from orwynn.utils.url._get_vars import get_vars
-from orwynn.utils.url._Url import Url
-from orwynn.utils.url._UrlVars import UrlVars
+from orwynn.utils.url.helpers import get_vars
+from orwynn.utils.url.url import Url
+from orwynn.utils.url.vars import UrlVars
 
 
 def test_path():
     vars: UrlVars = get_vars(
         url=Url("/user/eg1"),
         abstract_route="/user/{user_id}"
     )
```

### Comparing `orwynn-1.0.0b4/orwynn/utils/validation/__init__.py` & `orwynn-1.0.0b5/orwynn/utils/validation/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from inspect import isclass
 from pathlib import Path
 from typing import Any, Callable, Optional, Sized, TypeVar
 
 from pydantic import ValidationError as _PydanticValidationError
 from pydantic import validator as _pydantic_validator
 
-from orwynn.utils.validation._validator import Validator
+from orwynn.utils.validation.validator import Validator
 from orwynn.utils.validation.errors import (ExpectationError,
                                             ReValidationError,
                                             UnknownValidatorError,
                                             ValidationError)
 
 # WARNING: typing aliases are not currently supported so passing types like
 #   "dict[str, Any]" to check will produce ValidationError in any case since
```

### Comparing `orwynn-1.0.0b4/orwynn/utils/validation/errors.py` & `orwynn-1.0.0b5/orwynn/utils/validation/errors.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b4/orwynn/utils/yml/__init__.py` & `orwynn-1.0.0b5/orwynn/utils/yml/__init__.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b4/orwynn/websocket/_context/ContextBuiltinWebsocketMiddleware.py` & `orwynn-1.0.0b5/orwynn/websocket/context/middleware/builtin.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from orwynn.context._context_manager import context_manager
+from orwynn.context.manager import context_manager
 from orwynn.http import HttpNextCall, HttpRequest, HttpResponse
-from orwynn.websocket._middleware.BuiltinWebsocketMiddleware import (
+from orwynn.websocket.middleware.builtin import (
     BuiltinWebsocketMiddleware,
 )
 
 
 class ContextBuiltinWebsocketMiddleware(BuiltinWebsocketMiddleware):
     """Creates a shared context storage active within applied request-response
     cycle.
```

### Comparing `orwynn-1.0.0b4/orwynn/websocket/_context/RequestContextBuiltinWebsocketMiddleware.py` & `orwynn-1.0.0b5/orwynn/websocket/context/middleware/contextbuiltin.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-from orwynn.log._Log import Log
-from orwynn.websocket._context.WebsocketRequestContextId import (
+from orwynn.log.log import Log
+from orwynn.websocket.context.id import (
     WebsocketRequestContextId,
 )
-from orwynn.websocket._middleware.BuiltinWebsocketMiddleware import (
+from orwynn.websocket.middleware.builtin import (
     BuiltinWebsocketMiddleware,
 )
-from orwynn.websocket._middleware.WebsocketNextCall import WebsocketNextCall
-from orwynn.websocket._Websocket import Websocket
+from orwynn.websocket.middleware.nextcall import WebsocketNextCall
+from orwynn.websocket.websocket import Websocket
 
 
 class RequestContextBuiltinWebsocketMiddleware(BuiltinWebsocketMiddleware):
     """Populates the context storage with the current request's id."""
     async def process(
         self, request: Websocket, call_next: WebsocketNextCall
     ) -> None:
```

### Comparing `orwynn-1.0.0b4/orwynn/websocket/_context/WebsocketRequestContextId.py` & `orwynn-1.0.0b5/orwynn/websocket/context/id.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b4/orwynn/websocket/_context/websocket_context_test.py` & `orwynn-1.0.0b5/orwynn/websocket/context/test_main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-from orwynn.base.module._Module import Module
-from orwynn.boot._Boot import Boot
+from orwynn.base.module.module import Module
+from orwynn.boot.boot import Boot
 from orwynn.context.errors import UndefinedStorageError
 from orwynn.utils import validation
-from orwynn.websocket._context.WebsocketRequestContextId import (
+from orwynn.websocket.context.id import (
     WebsocketRequestContextId,
 )
-from orwynn.websocket._controller.WebsocketController import (
+from orwynn.websocket.controller.controller import (
     WebsocketController,
 )
-from orwynn.websocket._log.LogWebsocketMiddleware import LogWebsocketMiddleware
-from orwynn.websocket._Websocket import Websocket
+from orwynn.websocket.log.middleware import LogWebsocketMiddleware
+from orwynn.websocket.websocket import Websocket
 
 
 def test_basic():
     """Request id should be fetchable from context within request-response
     cycle and unfetchable outside this cycle.
     """
     class C1(WebsocketController):
```

### Comparing `orwynn-1.0.0b4/orwynn/websocket/_controller/WebsocketController.py` & `orwynn-1.0.0b5/orwynn/websocket/controller/controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Callable, ClassVar, Literal
 
-from orwynn.base.controller._Controller import Controller
+from orwynn.base.controller.controller import Controller
 from orwynn.utils import validation
-from orwynn.websocket._controller.WebsocketEventHandlerMethod import (
+from orwynn.websocket.controller.eventhandlermethod import (
     WebsocketEventHandlerMethod,
 )
 
 
 class WebsocketController(Controller):
     """Operates on websocket protocol.
```

### Comparing `orwynn-1.0.0b4/orwynn/websocket/_controller/global_websocket_route_test.py` & `orwynn-1.0.0b5/orwynn/websocket/controller/test_globalroute.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import starlette.websockets
 
 from orwynn.apiversion import ApiVersion
-from orwynn.base.module._Module import Module
+from orwynn.base.module.module import Module
 from orwynn.boot import Boot
-from orwynn.websocket._controller.WebsocketController import (
+from orwynn.websocket.controller.controller import (
     WebsocketController,
 )
-from orwynn.websocket._Websocket import Websocket
+from orwynn.websocket.websocket import Websocket
 
 
 class WsCtrl(WebsocketController):
     ROUTE = "/message"
 
     async def main(self, ws: Websocket) -> None:
         await ws.send_json({"message": "hello"})
```

### Comparing `orwynn-1.0.0b4/orwynn/websocket/_controller/websocket_controller_test.py` & `orwynn-1.0.0b5/orwynn/websocket/controller/test_controller.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,26 @@
-from orwynn.base.module._Module import Module
-from orwynn.boot._Boot import Boot
+from orwynn.apiversion import ApiVersion
+from orwynn.base.module.module import Module
+from orwynn.boot.boot import Boot
+from orwynn.di.di import Di
+from orwynn.utils import validation
 from orwynn.websocket import Websocket, WebsocketController
 
 
+class WsCtrl(WebsocketController):
+    ROUTE = "/"
+    VERSION = {2, 3}
+
+    async def main(self, ws: Websocket) -> None:
+        await ws.send_json({"message": "hello"})
+
+    async def on_connect(self, ws: Websocket) -> None:
+        await ws.send_json({"message": "hello"})
+
+
 class ArgumentedCtrl(WebsocketController):
     ROUTE = "/user/{user_id}"
 
     async def main(
         self,
         ws: Websocket,
         user_id: str,
@@ -112,7 +126,25 @@
 
     with boot.client.websocket("/user/eg1") as ws:
         data: dict = ws.receive_json()
 
         assert data["user_id"] == "eg1"
         assert data["message"] == "welcome"
         assert data["order"] is None
+
+
+
+def test_final_routes():
+    Boot(
+        Module(
+            "/",
+            Controllers=[WsCtrl]
+        ),
+        api_version=ApiVersion(supported={1, 2, 3}),
+        global_websocket_route="/ws/v{version}"
+    )
+
+    wsctrl: WsCtrl = validation.apply(Di.ie().find("WsCtrl"), WsCtrl)
+
+    assert wsctrl.final_routes == {
+        "/ws/v2", "/ws/v3", "/ws/v2/connect", "/ws/v3/connect"
+    }
```

### Comparing `orwynn-1.0.0b4/orwynn/websocket/_errorhandler/ErrorHandlerWebsocketMiddleware.py` & `orwynn-1.0.0b5/orwynn/websocket/errorhandler/middleware.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import inspect
 from types import NoneType
 
-from orwynn.base.error._find_detailed_class_for_exception import (
+from orwynn.base.error.errors import MalfunctionError
+from orwynn.base.error.utils import (
     find_detailed_class_for_exception,
 )
-from orwynn.base.error._MalfunctionError import MalfunctionError
-from orwynn.base.errorhandler._ErrorHandler import ErrorHandler
+from orwynn.base.errorhandler.errorhandler import ErrorHandler
 from orwynn.utils import validation
-from orwynn.websocket._context.WebsocketRequestContextId import (
+from orwynn.websocket.context.id import (
     WebsocketRequestContextId,
 )
-from orwynn.websocket._log.WebsocketLogger import WebsocketLogger
-from orwynn.websocket._middleware.BuiltinWebsocketMiddleware import (
+from orwynn.websocket.log.logger import WebsocketLogger
+from orwynn.websocket.middleware.builtin import (
     BuiltinWebsocketMiddleware,
 )
-from orwynn.websocket._middleware.WebsocketNextCall import WebsocketNextCall
-from orwynn.websocket._Websocket import Websocket
+from orwynn.websocket.middleware.nextcall import WebsocketNextCall
+from orwynn.websocket.websocket import Websocket
 
 
 class ErrorHandlerWebsocketMiddleware(BuiltinWebsocketMiddleware):
     """
     Handles all errors occured at Websocket layer.
     """
     def __init__(
```

### Comparing `orwynn-1.0.0b4/orwynn/websocket/_errorhandler/error_handler_websocket_test.py` & `orwynn-1.0.0b5/orwynn/websocket/errorhandler/test_default.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from orwynn.base.errorhandler._ErrorHandler import ErrorHandler
-from orwynn.base.module._Module import Module
-from orwynn.boot._Boot import Boot
-from orwynn.proxy.BootProxy import BootProxy
+from orwynn.base.errorhandler.errorhandler import ErrorHandler
+from orwynn.base.module.module import Module
+from orwynn.boot.boot import Boot
+from orwynn.proxy.boot import BootProxy
 from orwynn.utils import validation
-from orwynn.utils.Protocol import Protocol
+from orwynn.utils.protocol import Protocol
 from orwynn.websocket import Websocket, WebsocketController
 
 
 class SomeWebsocketError(Exception):
     pass
```

### Comparing `orwynn-1.0.0b4/orwynn/websocket/_log/LogWebsocketMiddleware.py` & `orwynn-1.0.0b5/orwynn/websocket/log/middleware.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from orwynn.websocket import (
     Websocket,
     WebsocketMiddleware,
     WebsocketNextCall,
     WebsocketRequestContextId,
 )
-from orwynn.websocket._log.WebsocketLogger import WebsocketLogger
+from orwynn.websocket.log.logger import WebsocketLogger
 
 
 class LogWebsocketMiddleware(WebsocketMiddleware):
     """Logs information about a websocket request.
 
     It's recommended to be outermost (at custom level) middleware.
     """
```

### Comparing `orwynn-1.0.0b4/orwynn/websocket/_log/WebsocketLogger.py` & `orwynn-1.0.0b5/orwynn/websocket/log/logger.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from orwynn.log._Log import Log
+from orwynn.log.log import Log
 from orwynn.utils import validation
-from orwynn.websocket._Websocket import Websocket
+from orwynn.websocket.websocket import Websocket
 
 
 class WebsocketLogger:
     """Logs websocket requests."""
     async def log_request(
         self,
         request: Websocket,
```

### Comparing `orwynn-1.0.0b4/orwynn/websocket/_middleware/ConnectionBuiltinWebsocketMiddleware.py` & `orwynn-1.0.0b5/orwynn/websocket/middleware/connectionbuiltin.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from orwynn.websocket._middleware.BuiltinWebsocketMiddleware import (
+from orwynn.websocket.middleware.builtin import (
     BuiltinWebsocketMiddleware,
 )
-from orwynn.websocket._middleware.WebsocketNextCall import WebsocketNextCall
-from orwynn.websocket._Websocket import Websocket
+from orwynn.websocket.middleware.nextcall import WebsocketNextCall
+from orwynn.websocket.websocket import Websocket
 
 
 class ConnectionBuiltinWebsocketMiddleware(BuiltinWebsocketMiddleware):
     """Manages websocket's connection acceptance.
 
     Note that you don't need to use websocket.accept() anywhere in your program
     or you will stuck in an endless loop. But you can call websocket.close()
```

### Comparing `orwynn-1.0.0b4/orwynn/websocket/_middleware/WebsocketMiddleware.py` & `orwynn-1.0.0b5/orwynn/websocket/middleware/middleware.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from orwynn.base.middleware import Middleware
-from orwynn.websocket._middleware.WebsocketNextCall import WebsocketNextCall
-from orwynn.websocket._Websocket import Websocket
+from orwynn.websocket.middleware.nextcall import WebsocketNextCall
+from orwynn.websocket.websocket import Websocket
 
 
 class WebsocketMiddleware(Middleware):
     """Intermediate operational layer for Websocket requests.
 
     Note that websocket methods return None since websocket sends data through
     the Websocket object itself.
```

### Comparing `orwynn-1.0.0b4/orwynn/websocket/_middleware/websocket_middleware_test.py` & `orwynn-1.0.0b5/orwynn/websocket/middleware/test_main.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from orwynn.base.module._Module import Module
-from orwynn.boot._Boot import Boot
-from orwynn.testing._Client import Client
+from orwynn.base.module.module import Module
+from orwynn.boot.boot import Boot
+from orwynn.testing.client import Client
 from orwynn.websocket import (
     Websocket,
     WebsocketController,
     WebsocketMiddleware,
     WebsocketNextCall,
 )
```

### Comparing `orwynn-1.0.0b4/orwynn/websocket/_routing/NextCallHandler.py` & `orwynn-1.0.0b5/orwynn/websocket/routing/nextcall.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import contextlib
 
 from orwynn.utils.url import UrlVars
-from orwynn.websocket._Websocket import Websocket
+from orwynn.websocket.websocket import Websocket
 
-from ._get_handler_kwargs import get_handler_kwargs
 from .handlers import DispatchWebsocketHandler, WebsocketHandler
+from .helpers import get_handler_kwargs
 
 
 class NextCallHandler:
     """
     Propagates calls through the given handler list.
     """
     def __init__(
```

### Comparing `orwynn-1.0.0b4/orwynn/websocket/_routing/WebsocketStack.py` & `orwynn-1.0.0b5/orwynn/websocket/routing/stack.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import functools
 from typing import Callable
 
-from orwynn.base.error._MalfunctionError import MalfunctionError
+from orwynn.base.error.errors import MalfunctionError
 from orwynn.utils import url
-from orwynn.websocket._Websocket import Websocket
+from orwynn.websocket.websocket import Websocket
 
 from .handlers import DispatchWebsocketHandler, WebsocketHandler
-from .NextCallHandler import NextCallHandler
+from .nextcall import NextCallHandler
 
 
 class WebsocketStack:
     """
     Manages an order of calls on websocket's request way through middleware and
     controllers.
```

### Comparing `orwynn-1.0.0b4/orwynn/websocket/_routing/_get_handler_kwargs.py` & `orwynn-1.0.0b5/orwynn/websocket/routing/helpers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import inspect
 import typing
 from types import NoneType, UnionType
 
 from orwynn.utils.url import UrlVars
-from orwynn.websocket._Websocket import Websocket
+from orwynn.websocket.websocket import Websocket
 
 from .handlers import WebsocketHandler
 
 # Types allowed to be set at handler's function argument annotations
-_AllowedTypesUnion: UnionType = str | int | float
+_AllowedTypesUnion = str | int | float
 _AllowedTypes: tuple[type] = typing.get_args(_AllowedTypesUnion)
 _Annotation = typing.TypeVar("_Annotation")
 
 # Allowed for handler kwargs
 HandlerKwargs = dict[str, _AllowedTypesUnion]
 
 
@@ -31,30 +31,40 @@
             Collected url variables to select from.
 
     Returns:
         Kwargs dictionary.
     """
     kwargs: HandlerKwargs = {}
 
+
     for param in inspect.signature(handler.fn).parameters.values():
         _check_if_duplicate(
             kwargs=kwargs,
             param=param
         )
 
         if param.annotation is Websocket:
             continue
-        elif isinstance(param.annotation, UnionType):
+        elif (
+            type(param.annotation) is UnionType
+            and any([
+                a in _AllowedTypes
+                    for a in typing.get_args(param.annotation)
+            ])
+        ):
             _set_union_param(
                 kwargs=kwargs,
                 param=param,
                 handler=handler,
                 url_vars=url_vars
             )
-        elif param.annotation in _AllowedTypes:
+        elif (
+            type(param.annotation) is type
+            and param.annotation in _AllowedTypes
+        ):
             _set_regular_param(
                 kwargs=kwargs,
                 param=param,
                 url_vars=url_vars
             )
         else:
             raise TypeError(
@@ -67,20 +77,14 @@
 
 def _set_regular_param(
     *,
     kwargs: HandlerKwargs,
     param: inspect.Parameter,
     url_vars: UrlVars
 ) -> None:
-    if param.annotation not in _AllowedTypes:
-        raise TypeError(
-            f"unsupported type of param {param.name} annotation:"
-            f" {param.annotation}"
-        )
-
     try:
         path_var_value: str = url_vars.path_vars[param.name]
     except KeyError as err:
         # Path variables unlike query ones cannot be defaulted, so here we
         # raise an error
         raise KeyError(
             f"no path variable for name: {param.name}"
@@ -102,14 +106,15 @@
     union_args: tuple = param.annotation.__args__
     _check_union_args(
         union_args,
         handler=handler,
         param=param
     )
 
+    final_value: typing.Any
     try:
         # For union types we operate only with query args
         query_var_value: str = url_vars.query_vars[param.name]
 
         # Choose non-None element of the union
         PositiveAnnotation: type = \
             union_args[0] if union_args[0] is not NoneType else union_args[1]
```

### Comparing `orwynn-1.0.0b4/pyproject.toml` & `orwynn-1.0.0b5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "orwynn"
-version = "1.0.0b4"
+version = "1.0.0b5"
 description = "Scalable web-framework with out-of-the-box architecture"
 authors = ["ryzhovalex <thed4rkof@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 fastapi = "^0.88.0"
```

### Comparing `orwynn-1.0.0b4/PKG-INFO` & `orwynn-1.0.0b5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orwynn
-Version: 1.0.0b4
+Version: 1.0.0b5
 Summary: Scalable web-framework with out-of-the-box architecture
 Author: ryzhovalex
 Author-email: thed4rkof@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: bcrypt (>=4.0.1,<5.0.0)
```

