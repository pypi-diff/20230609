# Comparing `tmp/BPTK_Py-1.7.6.tar.gz` & `tmp/BPTK_Py-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BPTK_Py-1.7.6.tar", last modified: Mon Mar 20 22:15:27 2023, max compression
+gzip compressed data, was "BPTK_Py-1.8.0.tar", last modified: Fri Jun  9 14:56:47 2023, max compression
```

## Comparing `BPTK_Py-1.7.6.tar` & `BPTK_Py-1.8.0.tar`

### file list

```diff
@@ -1,126 +1,132 @@
-drwxr-xr-x   0 olivergrasl   (501) staff       (20)        0 2023-03-20 22:15:27.419713 BPTK_Py-1.7.6/
-drwxr-xr-x   0 olivergrasl   (501) staff       (20)        0 2023-03-20 22:15:27.408270 BPTK_Py-1.7.6/BPTK_Py/
--rw-r--r--   0 olivergrasl   (501) staff       (20)      917 2022-08-25 14:46:11.000000 BPTK_Py-1.7.6/BPTK_Py/__init__.py
--rw-r--r--   0 olivergrasl   (501) staff       (20)    65683 2023-03-20 21:56:41.000000 BPTK_Py-1.7.6/BPTK_Py/bptk.py
-drwxr-xr-x   0 olivergrasl   (501) staff       (20)        0 2023-03-20 22:15:27.409391 BPTK_Py-1.7.6/BPTK_Py/config/
--rw-r--r--   0 olivergrasl   (501) staff       (20)       21 2022-08-25 14:46:11.000000 BPTK_Py-1.7.6/BPTK_Py/config/__init__.py
--rw-r--r--   0 olivergrasl   (501) staff       (20)     2354 2022-08-25 14:46:11.000000 BPTK_Py-1.7.6/BPTK_Py/config/config.py
-drwxr-xr-x   0 olivergrasl   (501) staff       (20)        0 2023-03-20 22:15:27.409662 BPTK_Py-1.7.6/BPTK_Py/exceptions/
--rw-r--r--   0 olivergrasl   (501) staff       (20)       25 2022-08-25 14:46:11.000000 BPTK_Py-1.7.6/BPTK_Py/exceptions/__init__.py
--rw-r--r--   0 olivergrasl   (501) staff       (20)      253 2022-08-25 14:46:11.000000 BPTK_Py-1.7.6/BPTK_Py/exceptions/exceptions.py
-drwxr-xr-x   0 olivergrasl   (501) staff       (20)        0 2023-03-20 22:15:27.409878 BPTK_Py-1.7.6/BPTK_Py/externalstateadapter/
--rw-r--r--   0 olivergrasl   (501) staff       (20)       82 2022-08-25 14:46:11.000000 BPTK_Py-1.7.6/BPTK_Py/externalstateadapter/__init__.py
--rw-r--r--   0 olivergrasl   (501) staff       (20)     4627 2022-11-24 12:44:03.000000 BPTK_Py-1.7.6/BPTK_Py/externalstateadapter/externalStateAdapter.py
-drwxr-xr-x   0 olivergrasl   (501) staff       (20)        0 2023-03-20 22:15:27.410081 BPTK_Py-1.7.6/BPTK_Py/logger/
--rw-r--r--   0 olivergrasl   (501) staff       (20)       23 2022-08-25 14:46:11.000000 BPTK_Py-1.7.6/BPTK_Py/logger/__init__.py
--rw-r--r--   0 olivergrasl   (501) staff       (20)     1208 2022-08-25 14:46:11.000000 BPTK_Py-1.7.6/BPTK_Py/logger/logger.py
-drwxr-xr-x   0 olivergrasl   (501) staff       (20)        0 2023-03-20 22:15:27.410804 BPTK_Py-1.7.6/BPTK_Py/modeling/
--rw-r--r--   0 olivergrasl   (501) staff       (20)      331 2022-08-25 14:46:11.000000 BPTK_Py-1.7.6/BPTK_Py/modeling/__init__.py
--rw-r--r--   0 olivergrasl   (501) staff       (20)    12552 2023-02-19 22:05:05.000000 BPTK_Py-1.7.6/BPTK_Py/modeling/agent.py
--rw-r--r--   0 olivergrasl   (501) staff       (20)     4944 2022-08-25 14:46:11.000000 BPTK_Py-1.7.6/BPTK_Py/modeling/dataCollector.py
-drwxr-xr-x   0 olivergrasl   (501) staff       (20)        0 2023-03-20 22:15:27.411196 BPTK_Py-1.7.6/BPTK_Py/modeling/datacollectors/
--rw-r--r--   0 olivergrasl   (501) staff       (20)      232 2022-08-25 14:46:11.000000 BPTK_Py-1.7.6/BPTK_Py/modeling/datacollectors/__init__.py
--rw-r--r--   0 olivergrasl   (501) staff       (20)     3497 2022-08-25 14:46:11.000000 BPTK_Py-1.7.6/BPTK_Py/modeling/datacollectors/agent_datacollector.py
--rwxr-xr-x   0 olivergrasl   (501) staff       (20)     3114 2022-08-25 14:46:11.000000 BPTK_Py-1.7.6/BPTK_Py/modeling/datacollectors/csv_datacollector.py
--rwxr-xr-x   0 olivergrasl   (501) staff       (20)     4371 2022-08-25 14:46:11.000000 BPTK_Py-1.7.6/BPTK_Py/modeling/datacollectors/kinesis_datacollector.py
--rw-r--r--   0 olivergrasl   (501) staff       (20)     1903 2022-08-25 14:46:11.000000 BPTK_Py-1.7.6/BPTK_Py/modeling/event.py
--rw-r--r--   0 olivergrasl   (501) staff       (20)    30380 2023-03-20 16:39:51.000000 BPTK_Py-1.7.6/BPTK_Py/modeling/model.py
--rw-r--r--   0 olivergrasl   (501) staff       (20)     2771 2022-08-25 14:46:11.000000 BPTK_Py-1.7.6/BPTK_Py/modeling/scheduler.py
--rw-r--r--   0 olivergrasl   (501) staff       (20)     4048 2022-08-25 14:46:11.000000 BPTK_Py-1.7.6/BPTK_Py/modeling/simultaneousScheduler.py
-drwxr-xr-x   0 olivergrasl   (501) staff       (20)        0 2023-03-20 22:15:27.411489 BPTK_Py-1.7.6/BPTK_Py/modelmonitor/
--rw-r--r--   0 olivergrasl   (501) staff       (20)       77 2022-08-25 14:46:11.000000 BPTK_Py-1.7.6/BPTK_Py/modelmonitor/__init__.py
--rw-r--r--   0 olivergrasl   (501) staff       (20)     3705 2022-08-25 14:46:11.000000 BPTK_Py-1.7.6/BPTK_Py/modelmonitor/file_monitor.py
--rw-r--r--   0 olivergrasl   (501) staff       (20)     4697 2022-08-25 14:46:11.000000 BPTK_Py-1.7.6/BPTK_Py/modelmonitor/model_monitor.py
-drwxr-xr-x   0 olivergrasl   (501) staff       (20)        0 2023-03-20 22:15:27.412033 BPTK_Py-1.7.6/BPTK_Py/modelparser/
--rw-r--r--   0 olivergrasl   (501) staff       (20)      232 2022-08-25 14:46:11.000000 BPTK_Py-1.7.6/BPTK_Py/modelparser/__init__.py
--rw-r--r--   0 olivergrasl   (501) staff       (20)     1256 2022-08-25 14:46:11.000000 BPTK_Py-1.7.6/BPTK_Py/modelparser/json_model_parser.py
--rw-r--r--   0 olivergrasl   (501) staff       (20)     8756 2022-08-25 14:46:11.000000 BPTK_Py-1.7.6/BPTK_Py/modelparser/meta_model_creator.py
--rw-r--r--   0 olivergrasl   (501) staff       (20)     1197 2022-08-25 14:46:11.000000 BPTK_Py-1.7.6/BPTK_Py/modelparser/parser_factory.py
--rw-r--r--   0 olivergrasl   (501) staff       (20)     5215 2022-08-25 14:46:11.000000 BPTK_Py-1.7.6/BPTK_Py/modelparser/yaml_model_parser.py
-drwxr-xr-x   0 olivergrasl   (501) staff       (20)        0 2023-03-20 22:15:27.412724 BPTK_Py-1.7.6/BPTK_Py/scenariomanager/
--rw-r--r--   0 olivergrasl   (501) staff       (20)      213 2022-08-25 14:46:11.000000 BPTK_Py-1.7.6/BPTK_Py/scenariomanager/__init__.py
--rw-r--r--   0 olivergrasl   (501) staff       (20)     7244 2023-02-16 05:56:09.000000 BPTK_Py-1.7.6/BPTK_Py/scenariomanager/scenario.py
--rw-r--r--   0 olivergrasl   (501) staff       (20)     1073 2022-08-25 14:46:11.000000 BPTK_Py-1.7.6/BPTK_Py/scenariomanager/scenario_manager.py
--rw-r--r--   0 olivergrasl   (501) staff       (20)    18371 2023-03-11 12:01:52.000000 BPTK_Py-1.7.6/BPTK_Py/scenariomanager/scenario_manager_factory.py
--rw-r--r--   0 olivergrasl   (501) staff       (20)     4845 2023-02-28 19:00:15.000000 BPTK_Py-1.7.6/BPTK_Py/scenariomanager/scenario_manager_hybrid.py
--rw-r--r--   0 olivergrasl   (501) staff       (20)    11221 2023-03-15 06:17:29.000000 BPTK_Py-1.7.6/BPTK_Py/scenariomanager/scenario_manager_sd.py
-drwxr-xr-x   0 olivergrasl   (501) staff       (20)        0 2023-03-20 22:15:27.413195 BPTK_Py-1.7.6/BPTK_Py/scenariorunners/
--rw-r--r--   0 olivergrasl   (501) staff       (20)      115 2022-08-25 14:46:11.000000 BPTK_Py-1.7.6/BPTK_Py/scenariorunners/__init__.py
--rw-r--r--   0 olivergrasl   (501) staff       (20)    31251 2022-08-25 14:46:11.000000 BPTK_Py-1.7.6/BPTK_Py/scenariorunners/hybrid_runner.py
--rw-r--r--   0 olivergrasl   (501) staff       (20)     2287 2022-08-25 14:46:11.000000 BPTK_Py-1.7.6/BPTK_Py/scenariorunners/scenario_runner.py
--rw-r--r--   0 olivergrasl   (501) staff       (20)    11854 2023-02-15 20:19:08.000000 BPTK_Py-1.7.6/BPTK_Py/scenariorunners/sd_runner.py
-drwxr-xr-x   0 olivergrasl   (501) staff       (20)        0 2023-03-20 22:15:27.413415 BPTK_Py-1.7.6/BPTK_Py/sdcompiler/
--rw-r--r--   0 olivergrasl   (501) staff       (20)     2624 2022-08-25 14:46:11.000000 BPTK_Py-1.7.6/BPTK_Py/sdcompiler/compile.py
-drwxr-xr-x   0 olivergrasl   (501) staff       (20)        0 2023-03-20 22:15:27.413673 BPTK_Py-1.7.6/BPTK_Py/sdcompiler/generator/
--rw-r--r--   0 olivergrasl   (501) staff       (20)      703 2022-08-25 14:46:11.000000 BPTK_Py-1.7.6/BPTK_Py/sdcompiler/generator/__init__.py
--rw-r--r--   0 olivergrasl   (501) staff       (20)     4567 2022-08-25 14:46:11.000000 BPTK_Py-1.7.6/BPTK_Py/sdcompiler/generator/contextBuilder.py
-drwxr-xr-x   0 olivergrasl   (501) staff       (20)        0 2023-03-20 22:15:27.414054 BPTK_Py-1.7.6/BPTK_Py/sdcompiler/generator/py/
--rw-r--r--   0 olivergrasl   (501) staff       (20)      558 2022-08-25 14:46:11.000000 BPTK_Py-1.7.6/BPTK_Py/sdcompiler/generator/py/__init__.py
--rw-r--r--   0 olivergrasl   (501) staff       (20)    23907 2022-08-25 14:46:11.000000 BPTK_Py-1.7.6/BPTK_Py/sdcompiler/generator/py/jinja_template.py
--rw-r--r--   0 olivergrasl   (501) staff       (20)    32060 2022-08-25 14:46:11.000000 BPTK_Py-1.7.6/BPTK_Py/sdcompiler/generator/py/py.py
-drwxr-xr-x   0 olivergrasl   (501) staff       (20)        0 2023-03-20 22:15:27.414193 BPTK_Py-1.7.6/BPTK_Py/sdcompiler/parsers/
--rw-r--r--   0 olivergrasl   (501) staff       (20)      520 2022-08-25 14:46:11.000000 BPTK_Py-1.7.6/BPTK_Py/sdcompiler/parsers/__init__.py
-drwxr-xr-x   0 olivergrasl   (501) staff       (20)        0 2023-03-20 22:15:27.414419 BPTK_Py-1.7.6/BPTK_Py/sdcompiler/parsers/smile/
--rw-r--r--   0 olivergrasl   (501) staff       (20)      565 2022-08-25 14:46:11.000000 BPTK_Py-1.7.6/BPTK_Py/sdcompiler/parsers/smile/__init__.py
--rw-r--r--   0 olivergrasl   (501) staff       (20)    13634 2023-02-27 20:16:20.000000 BPTK_Py-1.7.6/BPTK_Py/sdcompiler/parsers/smile/grammar.py
-drwxr-xr-x   0 olivergrasl   (501) staff       (20)        0 2023-03-20 22:15:27.414655 BPTK_Py-1.7.6/BPTK_Py/sdcompiler/parsers/xmile/
--rw-r--r--   0 olivergrasl   (501) staff       (20)      520 2022-08-25 14:46:11.000000 BPTK_Py-1.7.6/BPTK_Py/sdcompiler/parsers/xmile/__init__.py
--rw-r--r--   0 olivergrasl   (501) staff       (20)    11118 2023-02-27 20:06:17.000000 BPTK_Py-1.7.6/BPTK_Py/sdcompiler/parsers/xmile/xmile.py
-drwxr-xr-x   0 olivergrasl   (501) staff       (20)        0 2023-03-20 22:15:27.416189 BPTK_Py-1.7.6/BPTK_Py/sdcompiler/plugins/
--rw-r--r--   0 olivergrasl   (501) staff       (20)      998 2022-08-25 14:46:11.000000 BPTK_Py-1.7.6/BPTK_Py/sdcompiler/plugins/__init__.py
--rw-r--r--   0 olivergrasl   (501) staff       (20)    17380 2022-08-25 14:46:11.000000 BPTK_Py-1.7.6/BPTK_Py/sdcompiler/plugins/complexFunctions.py
--rw-r--r--   0 olivergrasl   (501) staff       (20)    14859 2022-08-25 14:46:11.000000 BPTK_Py-1.7.6/BPTK_Py/sdcompiler/plugins/expandArrays.py
--rw-r--r--   0 olivergrasl   (501) staff       (20)      344 2022-08-25 14:46:11.000000 BPTK_Py-1.7.6/BPTK_Py/sdcompiler/plugins/filterGhosts.py
--rw-r--r--   0 olivergrasl   (501) staff       (20)     1592 2022-08-25 14:46:11.000000 BPTK_Py-1.7.6/BPTK_Py/sdcompiler/plugins/fixLabels.py
--rw-r--r--   0 olivergrasl   (501) staff       (20)     1259 2022-08-25 14:46:11.000000 BPTK_Py-1.7.6/BPTK_Py/sdcompiler/plugins/makeAbsolute.py
--rw-r--r--   0 olivergrasl   (501) staff       (20)     2159 2022-08-25 14:46:11.000000 BPTK_Py-1.7.6/BPTK_Py/sdcompiler/plugins/replaceDimensionNames.py
--rw-r--r--   0 olivergrasl   (501) staff       (20)     3481 2022-08-25 14:46:11.000000 BPTK_Py-1.7.6/BPTK_Py/sdcompiler/plugins/resolveAsterisk.py
--rw-r--r--   0 olivergrasl   (501) staff       (20)     1033 2022-08-25 14:46:11.000000 BPTK_Py-1.7.6/BPTK_Py/sdcompiler/plugins/resolveSelf.py
--rw-r--r--   0 olivergrasl   (501) staff       (20)     1347 2022-08-25 14:46:11.000000 BPTK_Py-1.7.6/BPTK_Py/sdcompiler/plugins/sanitizeNames.py
--rw-r--r--   0 olivergrasl   (501) staff       (20)      756 2022-08-25 14:46:11.000000 BPTK_Py-1.7.6/BPTK_Py/sdcompiler/plugins/sortEntities.py
--rw-r--r--   0 olivergrasl   (501) staff       (20)     6100 2022-08-25 14:46:11.000000 BPTK_Py-1.7.6/BPTK_Py/sdcompiler/plugins/stockExpressions.py
--rw-r--r--   0 olivergrasl   (501) staff       (20)    16812 2023-03-20 16:06:34.000000 BPTK_Py-1.7.6/BPTK_Py/sdcompiler/sdmodel.py
-drwxr-xr-x   0 olivergrasl   (501) staff       (20)        0 2023-03-20 22:15:27.417351 BPTK_Py-1.7.6/BPTK_Py/sddsl/
--rw-r--r--   0 olivergrasl   (501) staff       (20)      205 2022-08-25 14:46:11.000000 BPTK_Py-1.7.6/BPTK_Py/sddsl/__init__.py
--rw-r--r--   0 olivergrasl   (501) staff       (20)      640 2022-08-25 14:46:11.000000 BPTK_Py-1.7.6/BPTK_Py/sddsl/biflow.py
--rwxr-xr-x   0 olivergrasl   (501) staff       (20)     1698 2023-01-28 18:02:46.000000 BPTK_Py-1.7.6/BPTK_Py/sddsl/constant.py
--rwxr-xr-x   0 olivergrasl   (501) staff       (20)     1000 2023-01-28 18:02:46.000000 BPTK_Py-1.7.6/BPTK_Py/sddsl/converter.py
--rwxr-xr-x   0 olivergrasl   (501) staff       (20)    17645 2023-03-20 16:46:14.000000 BPTK_Py-1.7.6/BPTK_Py/sddsl/element.py
--rwxr-xr-x   0 olivergrasl   (501) staff       (20)     1582 2023-01-28 18:02:46.000000 BPTK_Py-1.7.6/BPTK_Py/sddsl/flow.py
--rwxr-xr-x   0 olivergrasl   (501) staff       (20)     4834 2022-08-25 14:46:11.000000 BPTK_Py-1.7.6/BPTK_Py/sddsl/functions.py
--rw-r--r--   0 olivergrasl   (501) staff       (20)     3799 2022-08-25 14:46:11.000000 BPTK_Py-1.7.6/BPTK_Py/sddsl/module.py
--rwxr-xr-x   0 olivergrasl   (501) staff       (20)    55078 2023-03-20 17:14:18.000000 BPTK_Py-1.7.6/BPTK_Py/sddsl/operators.py
--rwxr-xr-x   0 olivergrasl   (501) staff       (20)     2853 2023-01-28 18:02:46.000000 BPTK_Py-1.7.6/BPTK_Py/sddsl/stock.py
-drwxr-xr-x   0 olivergrasl   (501) staff       (20)        0 2023-03-20 22:15:27.417561 BPTK_Py-1.7.6/BPTK_Py/sdsimulation/
--rw-r--r--   0 olivergrasl   (501) staff       (20)       39 2022-08-25 14:46:11.000000 BPTK_Py-1.7.6/BPTK_Py/sdsimulation/__init__.py
--rw-r--r--   0 olivergrasl   (501) staff       (20)     8946 2023-03-20 16:24:50.000000 BPTK_Py-1.7.6/BPTK_Py/sdsimulation/sd_simulation.py
-drwxr-xr-x   0 olivergrasl   (501) staff       (20)        0 2023-03-20 22:15:27.417751 BPTK_Py-1.7.6/BPTK_Py/server/
--rw-r--r--   0 olivergrasl   (501) staff       (20)       34 2022-08-25 14:46:11.000000 BPTK_Py-1.7.6/BPTK_Py/server/__init__.py
--rw-r--r--   0 olivergrasl   (501) staff       (20)    39145 2023-02-18 12:01:35.000000 BPTK_Py-1.7.6/BPTK_Py/server/bptkServer.py
-drwxr-xr-x   0 olivergrasl   (501) staff       (20)        0 2023-03-20 22:15:27.418735 BPTK_Py-1.7.6/BPTK_Py/util/
--rw-r--r--   0 olivergrasl   (501) staff       (20)      188 2023-03-20 15:56:23.000000 BPTK_Py-1.7.6/BPTK_Py/util/__init__.py
--rw-r--r--   0 olivergrasl   (501) staff       (20)      984 2022-08-25 14:46:11.000000 BPTK_Py-1.7.6/BPTK_Py/util/didyoumean.py
--rw-r--r--   0 olivergrasl   (501) staff       (20)     1103 2023-03-20 21:52:13.000000 BPTK_Py-1.7.6/BPTK_Py/util/floating_point.py
--rw-r--r--   0 olivergrasl   (501) staff       (20)     1605 2022-08-25 14:46:11.000000 BPTK_Py-1.7.6/BPTK_Py/util/lookup_data.py
--rw-r--r--   0 olivergrasl   (501) staff       (20)     3126 2022-08-25 14:46:11.000000 BPTK_Py-1.7.6/BPTK_Py/util/serializer.py
--rw-r--r--   0 olivergrasl   (501) staff       (20)     6908 2022-08-25 14:46:11.000000 BPTK_Py-1.7.6/BPTK_Py/util/statecompression.py
-drwxr-xr-x   0 olivergrasl   (501) staff       (20)        0 2023-03-20 22:15:27.419102 BPTK_Py-1.7.6/BPTK_Py/visualizations/
--rw-r--r--   0 olivergrasl   (501) staff       (20)       79 2022-08-25 14:46:11.000000 BPTK_Py-1.7.6/BPTK_Py/visualizations/__init__.py
--rw-r--r--   0 olivergrasl   (501) staff       (20)     9989 2023-02-25 12:55:49.000000 BPTK_Py-1.7.6/BPTK_Py/visualizations/simple_dashboard.py
--rw-r--r--   0 olivergrasl   (501) staff       (20)     6502 2022-08-25 14:46:11.000000 BPTK_Py-1.7.6/BPTK_Py/visualizations/visualize.py
-drwxr-xr-x   0 olivergrasl   (501) staff       (20)        0 2023-03-20 22:15:27.419591 BPTK_Py-1.7.6/BPTK_Py/widgets/
--rw-r--r--   0 olivergrasl   (501) staff       (20)      112 2023-02-16 05:00:42.000000 BPTK_Py-1.7.6/BPTK_Py/widgets/__init__.py
--rw-r--r--   0 olivergrasl   (501) staff       (20)     3062 2023-02-16 05:00:42.000000 BPTK_Py-1.7.6/BPTK_Py/widgets/agentstatuswidget.py
--rw-r--r--   0 olivergrasl   (501) staff       (20)     1878 2023-02-16 05:00:42.000000 BPTK_Py-1.7.6/BPTK_Py/widgets/widget.py
-drwxr-xr-x   0 olivergrasl   (501) staff       (20)        0 2023-03-20 22:15:27.409142 BPTK_Py-1.7.6/BPTK_Py.egg-info/
--rw-r--r--   0 olivergrasl   (501) staff       (20)    19490 2023-03-20 22:15:27.000000 BPTK_Py-1.7.6/BPTK_Py.egg-info/PKG-INFO
--rw-r--r--   0 olivergrasl   (501) staff       (20)     3443 2023-03-20 22:15:27.000000 BPTK_Py-1.7.6/BPTK_Py.egg-info/SOURCES.txt
--rw-r--r--   0 olivergrasl   (501) staff       (20)        1 2023-03-20 22:15:27.000000 BPTK_Py-1.7.6/BPTK_Py.egg-info/dependency_links.txt
--rw-r--r--   0 olivergrasl   (501) staff       (20)        1 2023-03-15 06:19:17.000000 BPTK_Py-1.7.6/BPTK_Py.egg-info/not-zip-safe
--rw-r--r--   0 olivergrasl   (501) staff       (20)      256 2023-03-20 22:15:27.000000 BPTK_Py-1.7.6/BPTK_Py.egg-info/requires.txt
--rw-r--r--   0 olivergrasl   (501) staff       (20)        8 2023-03-20 22:15:27.000000 BPTK_Py-1.7.6/BPTK_Py.egg-info/top_level.txt
--rw-r--r--   0 olivergrasl   (501) staff       (20)     1088 2022-08-25 14:46:11.000000 BPTK_Py-1.7.6/LICENSE
--rw-r--r--   0 olivergrasl   (501) staff       (20)    19490 2023-03-20 22:15:27.419816 BPTK_Py-1.7.6/PKG-INFO
--rw-r--r--   0 olivergrasl   (501) staff       (20)    19004 2023-03-20 22:12:43.000000 BPTK_Py-1.7.6/README.md
--rw-r--r--   0 olivergrasl   (501) staff       (20)       63 2023-03-20 22:15:27.420319 BPTK_Py-1.7.6/setup.cfg
--rw-r--r--   0 olivergrasl   (501) staff       (20)     2207 2022-08-25 14:46:11.000000 BPTK_Py-1.7.6/setup.py
+drwxr-xr-x   0 olivergrasl   (501) staff       (20)        0 2023-06-09 14:56:47.220152 BPTK_Py-1.8.0/
+drwxr-xr-x   0 olivergrasl   (501) staff       (20)        0 2023-06-09 14:56:47.198524 BPTK_Py-1.8.0/BPTK_Py/
+-rw-r--r--   0 olivergrasl   (501) staff       (20)      917 2022-08-25 14:46:11.000000 BPTK_Py-1.8.0/BPTK_Py/__init__.py
+-rw-r--r--   0 olivergrasl   (501) staff       (20)    65683 2023-03-20 21:56:41.000000 BPTK_Py-1.8.0/BPTK_Py/bptk.py
+drwxr-xr-x   0 olivergrasl   (501) staff       (20)        0 2023-06-09 14:56:47.200173 BPTK_Py-1.8.0/BPTK_Py/config/
+-rw-r--r--   0 olivergrasl   (501) staff       (20)       21 2022-08-25 14:46:11.000000 BPTK_Py-1.8.0/BPTK_Py/config/__init__.py
+-rw-r--r--   0 olivergrasl   (501) staff       (20)     2354 2022-08-25 14:46:11.000000 BPTK_Py-1.8.0/BPTK_Py/config/config.py
+drwxr-xr-x   0 olivergrasl   (501) staff       (20)        0 2023-06-09 14:56:47.200620 BPTK_Py-1.8.0/BPTK_Py/exceptions/
+-rw-r--r--   0 olivergrasl   (501) staff       (20)       25 2022-08-25 14:46:11.000000 BPTK_Py-1.8.0/BPTK_Py/exceptions/__init__.py
+-rw-r--r--   0 olivergrasl   (501) staff       (20)      253 2022-08-25 14:46:11.000000 BPTK_Py-1.8.0/BPTK_Py/exceptions/exceptions.py
+drwxr-xr-x   0 olivergrasl   (501) staff       (20)        0 2023-06-09 14:56:47.200887 BPTK_Py-1.8.0/BPTK_Py/externalstateadapter/
+-rw-r--r--   0 olivergrasl   (501) staff       (20)       82 2022-08-25 14:46:11.000000 BPTK_Py-1.8.0/BPTK_Py/externalstateadapter/__init__.py
+-rw-r--r--   0 olivergrasl   (501) staff       (20)     4627 2022-11-24 12:44:03.000000 BPTK_Py-1.8.0/BPTK_Py/externalstateadapter/externalStateAdapter.py
+drwxr-xr-x   0 olivergrasl   (501) staff       (20)        0 2023-06-09 14:56:47.201296 BPTK_Py-1.8.0/BPTK_Py/logger/
+-rw-r--r--   0 olivergrasl   (501) staff       (20)       23 2022-08-25 14:46:11.000000 BPTK_Py-1.8.0/BPTK_Py/logger/__init__.py
+-rw-r--r--   0 olivergrasl   (501) staff       (20)     1208 2022-08-25 14:46:11.000000 BPTK_Py-1.8.0/BPTK_Py/logger/logger.py
+drwxr-xr-x   0 olivergrasl   (501) staff       (20)        0 2023-06-09 14:56:47.202907 BPTK_Py-1.8.0/BPTK_Py/modeling/
+-rw-r--r--   0 olivergrasl   (501) staff       (20)      331 2022-08-25 14:46:11.000000 BPTK_Py-1.8.0/BPTK_Py/modeling/__init__.py
+-rw-r--r--   0 olivergrasl   (501) staff       (20)    12552 2023-02-19 22:05:05.000000 BPTK_Py-1.8.0/BPTK_Py/modeling/agent.py
+-rw-r--r--   0 olivergrasl   (501) staff       (20)     4944 2022-08-25 14:46:11.000000 BPTK_Py-1.8.0/BPTK_Py/modeling/dataCollector.py
+drwxr-xr-x   0 olivergrasl   (501) staff       (20)        0 2023-06-09 14:56:47.203642 BPTK_Py-1.8.0/BPTK_Py/modeling/datacollectors/
+-rw-r--r--   0 olivergrasl   (501) staff       (20)      232 2022-08-25 14:46:11.000000 BPTK_Py-1.8.0/BPTK_Py/modeling/datacollectors/__init__.py
+-rw-r--r--   0 olivergrasl   (501) staff       (20)     3497 2022-08-25 14:46:11.000000 BPTK_Py-1.8.0/BPTK_Py/modeling/datacollectors/agent_datacollector.py
+-rwxr-xr-x   0 olivergrasl   (501) staff       (20)     3114 2022-08-25 14:46:11.000000 BPTK_Py-1.8.0/BPTK_Py/modeling/datacollectors/csv_datacollector.py
+-rwxr-xr-x   0 olivergrasl   (501) staff       (20)     4371 2022-08-25 14:46:11.000000 BPTK_Py-1.8.0/BPTK_Py/modeling/datacollectors/kinesis_datacollector.py
+-rw-r--r--   0 olivergrasl   (501) staff       (20)     1903 2022-08-25 14:46:11.000000 BPTK_Py-1.8.0/BPTK_Py/modeling/event.py
+-rw-r--r--   0 olivergrasl   (501) staff       (20)    30380 2023-03-20 16:39:51.000000 BPTK_Py-1.8.0/BPTK_Py/modeling/model.py
+-rw-r--r--   0 olivergrasl   (501) staff       (20)     2771 2022-08-25 14:46:11.000000 BPTK_Py-1.8.0/BPTK_Py/modeling/scheduler.py
+-rw-r--r--   0 olivergrasl   (501) staff       (20)     4048 2022-08-25 14:46:11.000000 BPTK_Py-1.8.0/BPTK_Py/modeling/simultaneousScheduler.py
+drwxr-xr-x   0 olivergrasl   (501) staff       (20)        0 2023-06-09 14:56:47.204065 BPTK_Py-1.8.0/BPTK_Py/modelmonitor/
+-rw-r--r--   0 olivergrasl   (501) staff       (20)       77 2022-08-25 14:46:11.000000 BPTK_Py-1.8.0/BPTK_Py/modelmonitor/__init__.py
+-rw-r--r--   0 olivergrasl   (501) staff       (20)     3705 2022-08-25 14:46:11.000000 BPTK_Py-1.8.0/BPTK_Py/modelmonitor/file_monitor.py
+-rw-r--r--   0 olivergrasl   (501) staff       (20)     4697 2022-08-25 14:46:11.000000 BPTK_Py-1.8.0/BPTK_Py/modelmonitor/model_monitor.py
+drwxr-xr-x   0 olivergrasl   (501) staff       (20)        0 2023-06-09 14:56:47.204899 BPTK_Py-1.8.0/BPTK_Py/modelparser/
+-rw-r--r--   0 olivergrasl   (501) staff       (20)      232 2022-08-25 14:46:11.000000 BPTK_Py-1.8.0/BPTK_Py/modelparser/__init__.py
+-rw-r--r--   0 olivergrasl   (501) staff       (20)     1256 2022-08-25 14:46:11.000000 BPTK_Py-1.8.0/BPTK_Py/modelparser/json_model_parser.py
+-rw-r--r--   0 olivergrasl   (501) staff       (20)     8756 2022-08-25 14:46:11.000000 BPTK_Py-1.8.0/BPTK_Py/modelparser/meta_model_creator.py
+-rw-r--r--   0 olivergrasl   (501) staff       (20)     1197 2022-08-25 14:46:11.000000 BPTK_Py-1.8.0/BPTK_Py/modelparser/parser_factory.py
+-rw-r--r--   0 olivergrasl   (501) staff       (20)     5215 2022-08-25 14:46:11.000000 BPTK_Py-1.8.0/BPTK_Py/modelparser/yaml_model_parser.py
+drwxr-xr-x   0 olivergrasl   (501) staff       (20)        0 2023-06-09 14:56:47.206266 BPTK_Py-1.8.0/BPTK_Py/scenariomanager/
+-rw-r--r--   0 olivergrasl   (501) staff       (20)      213 2022-08-25 14:46:11.000000 BPTK_Py-1.8.0/BPTK_Py/scenariomanager/__init__.py
+-rw-r--r--   0 olivergrasl   (501) staff       (20)     7244 2023-02-16 05:56:09.000000 BPTK_Py-1.8.0/BPTK_Py/scenariomanager/scenario.py
+-rw-r--r--   0 olivergrasl   (501) staff       (20)     1073 2022-08-25 14:46:11.000000 BPTK_Py-1.8.0/BPTK_Py/scenariomanager/scenario_manager.py
+-rw-r--r--   0 olivergrasl   (501) staff       (20)    18371 2023-03-11 12:01:52.000000 BPTK_Py-1.8.0/BPTK_Py/scenariomanager/scenario_manager_factory.py
+-rw-r--r--   0 olivergrasl   (501) staff       (20)     4845 2023-02-28 19:00:15.000000 BPTK_Py-1.8.0/BPTK_Py/scenariomanager/scenario_manager_hybrid.py
+-rw-r--r--   0 olivergrasl   (501) staff       (20)    11221 2023-03-15 06:17:29.000000 BPTK_Py-1.8.0/BPTK_Py/scenariomanager/scenario_manager_sd.py
+drwxr-xr-x   0 olivergrasl   (501) staff       (20)        0 2023-06-09 14:56:47.206996 BPTK_Py-1.8.0/BPTK_Py/scenariorunners/
+-rw-r--r--   0 olivergrasl   (501) staff       (20)      115 2022-08-25 14:46:11.000000 BPTK_Py-1.8.0/BPTK_Py/scenariorunners/__init__.py
+-rw-r--r--   0 olivergrasl   (501) staff       (20)    31251 2022-08-25 14:46:11.000000 BPTK_Py-1.8.0/BPTK_Py/scenariorunners/hybrid_runner.py
+-rw-r--r--   0 olivergrasl   (501) staff       (20)     2287 2022-08-25 14:46:11.000000 BPTK_Py-1.8.0/BPTK_Py/scenariorunners/scenario_runner.py
+-rw-r--r--   0 olivergrasl   (501) staff       (20)    11854 2023-02-15 20:19:08.000000 BPTK_Py-1.8.0/BPTK_Py/scenariorunners/sd_runner.py
+drwxr-xr-x   0 olivergrasl   (501) staff       (20)        0 2023-06-09 14:56:47.207381 BPTK_Py-1.8.0/BPTK_Py/sdcompiler/
+-rw-r--r--   0 olivergrasl   (501) staff       (20)     2624 2022-08-25 14:46:11.000000 BPTK_Py-1.8.0/BPTK_Py/sdcompiler/compile.py
+drwxr-xr-x   0 olivergrasl   (501) staff       (20)        0 2023-06-09 14:56:47.207982 BPTK_Py-1.8.0/BPTK_Py/sdcompiler/generator/
+-rw-r--r--   0 olivergrasl   (501) staff       (20)      703 2022-08-25 14:46:11.000000 BPTK_Py-1.8.0/BPTK_Py/sdcompiler/generator/__init__.py
+-rw-r--r--   0 olivergrasl   (501) staff       (20)     4567 2022-08-25 14:46:11.000000 BPTK_Py-1.8.0/BPTK_Py/sdcompiler/generator/contextBuilder.py
+drwxr-xr-x   0 olivergrasl   (501) staff       (20)        0 2023-06-09 14:56:47.208552 BPTK_Py-1.8.0/BPTK_Py/sdcompiler/generator/py/
+-rw-r--r--   0 olivergrasl   (501) staff       (20)      558 2022-08-25 14:46:11.000000 BPTK_Py-1.8.0/BPTK_Py/sdcompiler/generator/py/__init__.py
+-rw-r--r--   0 olivergrasl   (501) staff       (20)    23907 2022-08-25 14:46:11.000000 BPTK_Py-1.8.0/BPTK_Py/sdcompiler/generator/py/jinja_template.py
+-rw-r--r--   0 olivergrasl   (501) staff       (20)    32060 2022-08-25 14:46:11.000000 BPTK_Py-1.8.0/BPTK_Py/sdcompiler/generator/py/py.py
+drwxr-xr-x   0 olivergrasl   (501) staff       (20)        0 2023-06-09 14:56:47.208742 BPTK_Py-1.8.0/BPTK_Py/sdcompiler/parsers/
+-rw-r--r--   0 olivergrasl   (501) staff       (20)      520 2022-08-25 14:46:11.000000 BPTK_Py-1.8.0/BPTK_Py/sdcompiler/parsers/__init__.py
+drwxr-xr-x   0 olivergrasl   (501) staff       (20)        0 2023-06-09 14:56:47.209055 BPTK_Py-1.8.0/BPTK_Py/sdcompiler/parsers/smile/
+-rw-r--r--   0 olivergrasl   (501) staff       (20)      565 2022-08-25 14:46:11.000000 BPTK_Py-1.8.0/BPTK_Py/sdcompiler/parsers/smile/__init__.py
+-rw-r--r--   0 olivergrasl   (501) staff       (20)    13634 2023-02-27 20:16:20.000000 BPTK_Py-1.8.0/BPTK_Py/sdcompiler/parsers/smile/grammar.py
+drwxr-xr-x   0 olivergrasl   (501) staff       (20)        0 2023-06-09 14:56:47.209594 BPTK_Py-1.8.0/BPTK_Py/sdcompiler/parsers/xmile/
+-rw-r--r--   0 olivergrasl   (501) staff       (20)      520 2022-08-25 14:46:11.000000 BPTK_Py-1.8.0/BPTK_Py/sdcompiler/parsers/xmile/__init__.py
+-rw-r--r--   0 olivergrasl   (501) staff       (20)    11118 2023-02-27 20:06:17.000000 BPTK_Py-1.8.0/BPTK_Py/sdcompiler/parsers/xmile/xmile.py
+drwxr-xr-x   0 olivergrasl   (501) staff       (20)        0 2023-06-09 14:56:47.211650 BPTK_Py-1.8.0/BPTK_Py/sdcompiler/plugins/
+-rw-r--r--   0 olivergrasl   (501) staff       (20)      998 2022-08-25 14:46:11.000000 BPTK_Py-1.8.0/BPTK_Py/sdcompiler/plugins/__init__.py
+-rw-r--r--   0 olivergrasl   (501) staff       (20)    17380 2022-08-25 14:46:11.000000 BPTK_Py-1.8.0/BPTK_Py/sdcompiler/plugins/complexFunctions.py
+-rw-r--r--   0 olivergrasl   (501) staff       (20)    14859 2022-08-25 14:46:11.000000 BPTK_Py-1.8.0/BPTK_Py/sdcompiler/plugins/expandArrays.py
+-rw-r--r--   0 olivergrasl   (501) staff       (20)      344 2022-08-25 14:46:11.000000 BPTK_Py-1.8.0/BPTK_Py/sdcompiler/plugins/filterGhosts.py
+-rw-r--r--   0 olivergrasl   (501) staff       (20)     1592 2022-08-25 14:46:11.000000 BPTK_Py-1.8.0/BPTK_Py/sdcompiler/plugins/fixLabels.py
+-rw-r--r--   0 olivergrasl   (501) staff       (20)     1259 2022-08-25 14:46:11.000000 BPTK_Py-1.8.0/BPTK_Py/sdcompiler/plugins/makeAbsolute.py
+-rw-r--r--   0 olivergrasl   (501) staff       (20)     2159 2022-08-25 14:46:11.000000 BPTK_Py-1.8.0/BPTK_Py/sdcompiler/plugins/replaceDimensionNames.py
+-rw-r--r--   0 olivergrasl   (501) staff       (20)     3481 2022-08-25 14:46:11.000000 BPTK_Py-1.8.0/BPTK_Py/sdcompiler/plugins/resolveAsterisk.py
+-rw-r--r--   0 olivergrasl   (501) staff       (20)     1033 2022-08-25 14:46:11.000000 BPTK_Py-1.8.0/BPTK_Py/sdcompiler/plugins/resolveSelf.py
+-rw-r--r--   0 olivergrasl   (501) staff       (20)     1347 2022-08-25 14:46:11.000000 BPTK_Py-1.8.0/BPTK_Py/sdcompiler/plugins/sanitizeNames.py
+-rw-r--r--   0 olivergrasl   (501) staff       (20)      756 2022-08-25 14:46:11.000000 BPTK_Py-1.8.0/BPTK_Py/sdcompiler/plugins/sortEntities.py
+-rw-r--r--   0 olivergrasl   (501) staff       (20)     6100 2022-08-25 14:46:11.000000 BPTK_Py-1.8.0/BPTK_Py/sdcompiler/plugins/stockExpressions.py
+-rw-r--r--   0 olivergrasl   (501) staff       (20)    16812 2023-03-20 16:06:34.000000 BPTK_Py-1.8.0/BPTK_Py/sdcompiler/sdmodel.py
+drwxr-xr-x   0 olivergrasl   (501) staff       (20)        0 2023-06-09 14:56:47.214149 BPTK_Py-1.8.0/BPTK_Py/sddsl/
+-rw-r--r--   0 olivergrasl   (501) staff       (20)      205 2022-08-25 14:46:11.000000 BPTK_Py-1.8.0/BPTK_Py/sddsl/__init__.py
+-rw-r--r--   0 olivergrasl   (501) staff       (20)      640 2022-08-25 14:46:11.000000 BPTK_Py-1.8.0/BPTK_Py/sddsl/biflow.py
+-rwxr-xr-x   0 olivergrasl   (501) staff       (20)     1698 2023-01-28 18:02:46.000000 BPTK_Py-1.8.0/BPTK_Py/sddsl/constant.py
+-rwxr-xr-x   0 olivergrasl   (501) staff       (20)     1000 2023-01-28 18:02:46.000000 BPTK_Py-1.8.0/BPTK_Py/sddsl/converter.py
+-rwxr-xr-x   0 olivergrasl   (501) staff       (20)    17645 2023-03-20 16:46:14.000000 BPTK_Py-1.8.0/BPTK_Py/sddsl/element.py
+-rwxr-xr-x   0 olivergrasl   (501) staff       (20)     1582 2023-01-28 18:02:46.000000 BPTK_Py-1.8.0/BPTK_Py/sddsl/flow.py
+-rwxr-xr-x   0 olivergrasl   (501) staff       (20)     4834 2022-08-25 14:46:11.000000 BPTK_Py-1.8.0/BPTK_Py/sddsl/functions.py
+-rw-r--r--   0 olivergrasl   (501) staff       (20)     3799 2022-08-25 14:46:11.000000 BPTK_Py-1.8.0/BPTK_Py/sddsl/module.py
+-rwxr-xr-x   0 olivergrasl   (501) staff       (20)    55078 2023-03-20 17:14:18.000000 BPTK_Py-1.8.0/BPTK_Py/sddsl/operators.py
+-rwxr-xr-x   0 olivergrasl   (501) staff       (20)     2853 2023-01-28 18:02:46.000000 BPTK_Py-1.8.0/BPTK_Py/sddsl/stock.py
+drwxr-xr-x   0 olivergrasl   (501) staff       (20)        0 2023-06-09 14:56:47.214568 BPTK_Py-1.8.0/BPTK_Py/sdsimulation/
+-rw-r--r--   0 olivergrasl   (501) staff       (20)       39 2022-08-25 14:46:11.000000 BPTK_Py-1.8.0/BPTK_Py/sdsimulation/__init__.py
+-rw-r--r--   0 olivergrasl   (501) staff       (20)     8946 2023-03-20 16:24:50.000000 BPTK_Py-1.8.0/BPTK_Py/sdsimulation/sd_simulation.py
+drwxr-xr-x   0 olivergrasl   (501) staff       (20)        0 2023-06-09 14:56:47.214986 BPTK_Py-1.8.0/BPTK_Py/server/
+-rw-r--r--   0 olivergrasl   (501) staff       (20)       34 2022-08-25 14:46:11.000000 BPTK_Py-1.8.0/BPTK_Py/server/__init__.py
+-rw-r--r--   0 olivergrasl   (501) staff       (20)    40409 2023-06-09 14:40:10.000000 BPTK_Py-1.8.0/BPTK_Py/server/bptkServer.py
+drwxr-xr-x   0 olivergrasl   (501) staff       (20)        0 2023-06-09 14:56:47.216819 BPTK_Py-1.8.0/BPTK_Py/util/
+-rw-r--r--   0 olivergrasl   (501) staff       (20)      188 2023-03-20 15:56:23.000000 BPTK_Py-1.8.0/BPTK_Py/util/__init__.py
+-rw-r--r--   0 olivergrasl   (501) staff       (20)      984 2022-08-25 14:46:11.000000 BPTK_Py-1.8.0/BPTK_Py/util/didyoumean.py
+-rw-r--r--   0 olivergrasl   (501) staff       (20)     1103 2023-03-20 21:52:13.000000 BPTK_Py-1.8.0/BPTK_Py/util/floating_point.py
+-rw-r--r--   0 olivergrasl   (501) staff       (20)     1605 2022-08-25 14:46:11.000000 BPTK_Py-1.8.0/BPTK_Py/util/lookup_data.py
+-rw-r--r--   0 olivergrasl   (501) staff       (20)     3126 2022-08-25 14:46:11.000000 BPTK_Py-1.8.0/BPTK_Py/util/serializer.py
+-rw-r--r--   0 olivergrasl   (501) staff       (20)     6908 2022-08-25 14:46:11.000000 BPTK_Py-1.8.0/BPTK_Py/util/statecompression.py
+drwxr-xr-x   0 olivergrasl   (501) staff       (20)        0 2023-06-09 14:56:47.217441 BPTK_Py-1.8.0/BPTK_Py/visualizations/
+-rw-r--r--   0 olivergrasl   (501) staff       (20)       79 2022-08-25 14:46:11.000000 BPTK_Py-1.8.0/BPTK_Py/visualizations/__init__.py
+-rw-r--r--   0 olivergrasl   (501) staff       (20)     9989 2023-02-25 12:55:49.000000 BPTK_Py-1.8.0/BPTK_Py/visualizations/simple_dashboard.py
+-rw-r--r--   0 olivergrasl   (501) staff       (20)     6502 2022-08-25 14:46:11.000000 BPTK_Py-1.8.0/BPTK_Py/visualizations/visualize.py
+drwxr-xr-x   0 olivergrasl   (501) staff       (20)        0 2023-06-09 14:56:47.218050 BPTK_Py-1.8.0/BPTK_Py/widgets/
+-rw-r--r--   0 olivergrasl   (501) staff       (20)      112 2023-02-16 05:00:42.000000 BPTK_Py-1.8.0/BPTK_Py/widgets/__init__.py
+-rw-r--r--   0 olivergrasl   (501) staff       (20)     3062 2023-02-16 05:00:42.000000 BPTK_Py-1.8.0/BPTK_Py/widgets/agentstatuswidget.py
+-rw-r--r--   0 olivergrasl   (501) staff       (20)     1878 2023-02-16 05:00:42.000000 BPTK_Py-1.8.0/BPTK_Py/widgets/widget.py
+drwxr-xr-x   0 olivergrasl   (501) staff       (20)        0 2023-06-09 14:56:47.199845 BPTK_Py-1.8.0/BPTK_Py.egg-info/
+-rw-r--r--   0 olivergrasl   (501) staff       (20)    19590 2023-06-09 14:56:47.000000 BPTK_Py-1.8.0/BPTK_Py.egg-info/PKG-INFO
+-rw-r--r--   0 olivergrasl   (501) staff       (20)     3552 2023-06-09 14:56:47.000000 BPTK_Py-1.8.0/BPTK_Py.egg-info/SOURCES.txt
+-rw-r--r--   0 olivergrasl   (501) staff       (20)        1 2023-06-09 14:56:47.000000 BPTK_Py-1.8.0/BPTK_Py.egg-info/dependency_links.txt
+-rw-r--r--   0 olivergrasl   (501) staff       (20)        1 2023-06-09 14:09:45.000000 BPTK_Py-1.8.0/BPTK_Py.egg-info/not-zip-safe
+-rw-r--r--   0 olivergrasl   (501) staff       (20)      256 2023-06-09 14:56:47.000000 BPTK_Py-1.8.0/BPTK_Py.egg-info/requires.txt
+-rw-r--r--   0 olivergrasl   (501) staff       (20)        8 2023-06-09 14:56:47.000000 BPTK_Py-1.8.0/BPTK_Py.egg-info/top_level.txt
+-rw-r--r--   0 olivergrasl   (501) staff       (20)     1088 2022-08-25 14:46:11.000000 BPTK_Py-1.8.0/LICENSE
+-rw-r--r--   0 olivergrasl   (501) staff       (20)    19590 2023-06-09 14:56:47.220256 BPTK_Py-1.8.0/PKG-INFO
+-rw-r--r--   0 olivergrasl   (501) staff       (20)    19104 2023-06-09 14:51:19.000000 BPTK_Py-1.8.0/README.md
+-rw-r--r--   0 olivergrasl   (501) staff       (20)       63 2023-06-09 14:56:47.221138 BPTK_Py-1.8.0/setup.cfg
+-rw-r--r--   0 olivergrasl   (501) staff       (20)     2207 2022-08-25 14:46:11.000000 BPTK_Py-1.8.0/setup.py
+drwxr-xr-x   0 olivergrasl   (501) staff       (20)        0 2023-06-09 14:56:47.219680 BPTK_Py-1.8.0/tests/
+-rw-r--r--   0 olivergrasl   (501) staff       (20)    13983 2023-03-20 21:40:01.000000 BPTK_Py-1.8.0/tests/test_bptk.py
+-rw-r--r--   0 olivergrasl   (501) staff       (20)     5324 2023-02-18 12:06:43.000000 BPTK_Py-1.8.0/tests/test_external_state.py
+-rw-r--r--   0 olivergrasl   (501) staff       (20)    61958 2023-03-20 21:40:41.000000 BPTK_Py-1.8.0/tests/test_sddsl.py
+-rw-r--r--   0 olivergrasl   (501) staff       (20)    17599 2023-06-09 14:48:57.000000 BPTK_Py-1.8.0/tests/test_server.py
+-rw-r--r--   0 olivergrasl   (501) staff       (20)    54591 2023-02-27 20:14:40.000000 BPTK_Py-1.8.0/tests/test_xmile.py
```

### Comparing `BPTK_Py-1.7.6/BPTK_Py/__init__.py` & `BPTK_Py-1.8.0/BPTK_Py/__init__.py`

 * *Files identical despite different names*

### Comparing `BPTK_Py-1.7.6/BPTK_Py/bptk.py` & `BPTK_Py-1.8.0/BPTK_Py/bptk.py`

 * *Files identical despite different names*

### Comparing `BPTK_Py-1.7.6/BPTK_Py/config/config.py` & `BPTK_Py-1.8.0/BPTK_Py/config/config.py`

 * *Files identical despite different names*

### Comparing `BPTK_Py-1.7.6/BPTK_Py/externalstateadapter/externalStateAdapter.py` & `BPTK_Py-1.8.0/BPTK_Py/externalstateadapter/externalStateAdapter.py`

 * *Files identical despite different names*

### Comparing `BPTK_Py-1.7.6/BPTK_Py/logger/logger.py` & `BPTK_Py-1.8.0/BPTK_Py/logger/logger.py`

 * *Files identical despite different names*

### Comparing `BPTK_Py-1.7.6/BPTK_Py/modeling/agent.py` & `BPTK_Py-1.8.0/BPTK_Py/modeling/agent.py`

 * *Files identical despite different names*

### Comparing `BPTK_Py-1.7.6/BPTK_Py/modeling/dataCollector.py` & `BPTK_Py-1.8.0/BPTK_Py/modeling/dataCollector.py`

 * *Files identical despite different names*

### Comparing `BPTK_Py-1.7.6/BPTK_Py/modeling/datacollectors/agent_datacollector.py` & `BPTK_Py-1.8.0/BPTK_Py/modeling/datacollectors/agent_datacollector.py`

 * *Files identical despite different names*

### Comparing `BPTK_Py-1.7.6/BPTK_Py/modeling/datacollectors/csv_datacollector.py` & `BPTK_Py-1.8.0/BPTK_Py/modeling/datacollectors/csv_datacollector.py`

 * *Files identical despite different names*

### Comparing `BPTK_Py-1.7.6/BPTK_Py/modeling/datacollectors/kinesis_datacollector.py` & `BPTK_Py-1.8.0/BPTK_Py/modeling/datacollectors/kinesis_datacollector.py`

 * *Files identical despite different names*

### Comparing `BPTK_Py-1.7.6/BPTK_Py/modeling/event.py` & `BPTK_Py-1.8.0/BPTK_Py/modeling/event.py`

 * *Files identical despite different names*

### Comparing `BPTK_Py-1.7.6/BPTK_Py/modeling/model.py` & `BPTK_Py-1.8.0/BPTK_Py/modeling/model.py`

 * *Files identical despite different names*

### Comparing `BPTK_Py-1.7.6/BPTK_Py/modeling/scheduler.py` & `BPTK_Py-1.8.0/BPTK_Py/modeling/scheduler.py`

 * *Files identical despite different names*

### Comparing `BPTK_Py-1.7.6/BPTK_Py/modeling/simultaneousScheduler.py` & `BPTK_Py-1.8.0/BPTK_Py/modeling/simultaneousScheduler.py`

 * *Files identical despite different names*

### Comparing `BPTK_Py-1.7.6/BPTK_Py/modelmonitor/file_monitor.py` & `BPTK_Py-1.8.0/BPTK_Py/modelmonitor/file_monitor.py`

 * *Files identical despite different names*

### Comparing `BPTK_Py-1.7.6/BPTK_Py/modelmonitor/model_monitor.py` & `BPTK_Py-1.8.0/BPTK_Py/modelmonitor/model_monitor.py`

 * *Files identical despite different names*

### Comparing `BPTK_Py-1.7.6/BPTK_Py/modelparser/json_model_parser.py` & `BPTK_Py-1.8.0/BPTK_Py/modelparser/json_model_parser.py`

 * *Files identical despite different names*

### Comparing `BPTK_Py-1.7.6/BPTK_Py/modelparser/meta_model_creator.py` & `BPTK_Py-1.8.0/BPTK_Py/modelparser/meta_model_creator.py`

 * *Files identical despite different names*

### Comparing `BPTK_Py-1.7.6/BPTK_Py/modelparser/parser_factory.py` & `BPTK_Py-1.8.0/BPTK_Py/modelparser/parser_factory.py`

 * *Files identical despite different names*

### Comparing `BPTK_Py-1.7.6/BPTK_Py/modelparser/yaml_model_parser.py` & `BPTK_Py-1.8.0/BPTK_Py/modelparser/yaml_model_parser.py`

 * *Files identical despite different names*

### Comparing `BPTK_Py-1.7.6/BPTK_Py/scenariomanager/scenario.py` & `BPTK_Py-1.8.0/BPTK_Py/scenariomanager/scenario.py`

 * *Files identical despite different names*

### Comparing `BPTK_Py-1.7.6/BPTK_Py/scenariomanager/scenario_manager.py` & `BPTK_Py-1.8.0/BPTK_Py/scenariomanager/scenario_manager.py`

 * *Files identical despite different names*

### Comparing `BPTK_Py-1.7.6/BPTK_Py/scenariomanager/scenario_manager_factory.py` & `BPTK_Py-1.8.0/BPTK_Py/scenariomanager/scenario_manager_factory.py`

 * *Files identical despite different names*

### Comparing `BPTK_Py-1.7.6/BPTK_Py/scenariomanager/scenario_manager_hybrid.py` & `BPTK_Py-1.8.0/BPTK_Py/scenariomanager/scenario_manager_hybrid.py`

 * *Files identical despite different names*

### Comparing `BPTK_Py-1.7.6/BPTK_Py/scenariomanager/scenario_manager_sd.py` & `BPTK_Py-1.8.0/BPTK_Py/scenariomanager/scenario_manager_sd.py`

 * *Files identical despite different names*

### Comparing `BPTK_Py-1.7.6/BPTK_Py/scenariorunners/hybrid_runner.py` & `BPTK_Py-1.8.0/BPTK_Py/scenariorunners/hybrid_runner.py`

 * *Files identical despite different names*

### Comparing `BPTK_Py-1.7.6/BPTK_Py/scenariorunners/scenario_runner.py` & `BPTK_Py-1.8.0/BPTK_Py/scenariorunners/scenario_runner.py`

 * *Files identical despite different names*

### Comparing `BPTK_Py-1.7.6/BPTK_Py/scenariorunners/sd_runner.py` & `BPTK_Py-1.8.0/BPTK_Py/scenariorunners/sd_runner.py`

 * *Files identical despite different names*

### Comparing `BPTK_Py-1.7.6/BPTK_Py/sdcompiler/compile.py` & `BPTK_Py-1.8.0/BPTK_Py/sdcompiler/compile.py`

 * *Files identical despite different names*

### Comparing `BPTK_Py-1.7.6/BPTK_Py/sdcompiler/generator/__init__.py` & `BPTK_Py-1.8.0/BPTK_Py/sdcompiler/generator/__init__.py`

 * *Files identical despite different names*

### Comparing `BPTK_Py-1.7.6/BPTK_Py/sdcompiler/generator/contextBuilder.py` & `BPTK_Py-1.8.0/BPTK_Py/sdcompiler/generator/contextBuilder.py`

 * *Files identical despite different names*

### Comparing `BPTK_Py-1.7.6/BPTK_Py/sdcompiler/generator/py/__init__.py` & `BPTK_Py-1.8.0/BPTK_Py/sdcompiler/generator/py/__init__.py`

 * *Files identical despite different names*

### Comparing `BPTK_Py-1.7.6/BPTK_Py/sdcompiler/generator/py/jinja_template.py` & `BPTK_Py-1.8.0/BPTK_Py/sdcompiler/generator/py/jinja_template.py`

 * *Files identical despite different names*

### Comparing `BPTK_Py-1.7.6/BPTK_Py/sdcompiler/generator/py/py.py` & `BPTK_Py-1.8.0/BPTK_Py/sdcompiler/generator/py/py.py`

 * *Files identical despite different names*

### Comparing `BPTK_Py-1.7.6/BPTK_Py/sdcompiler/parsers/__init__.py` & `BPTK_Py-1.8.0/BPTK_Py/sdcompiler/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `BPTK_Py-1.7.6/BPTK_Py/sdcompiler/parsers/smile/__init__.py` & `BPTK_Py-1.8.0/BPTK_Py/sdcompiler/parsers/smile/__init__.py`

 * *Files identical despite different names*

### Comparing `BPTK_Py-1.7.6/BPTK_Py/sdcompiler/parsers/smile/grammar.py` & `BPTK_Py-1.8.0/BPTK_Py/sdcompiler/parsers/smile/grammar.py`

 * *Files identical despite different names*

### Comparing `BPTK_Py-1.7.6/BPTK_Py/sdcompiler/parsers/xmile/__init__.py` & `BPTK_Py-1.8.0/BPTK_Py/sdcompiler/parsers/xmile/__init__.py`

 * *Files identical despite different names*

### Comparing `BPTK_Py-1.7.6/BPTK_Py/sdcompiler/parsers/xmile/xmile.py` & `BPTK_Py-1.8.0/BPTK_Py/sdcompiler/parsers/xmile/xmile.py`

 * *Files identical despite different names*

### Comparing `BPTK_Py-1.7.6/BPTK_Py/sdcompiler/plugins/__init__.py` & `BPTK_Py-1.8.0/BPTK_Py/sdcompiler/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `BPTK_Py-1.7.6/BPTK_Py/sdcompiler/plugins/complexFunctions.py` & `BPTK_Py-1.8.0/BPTK_Py/sdcompiler/plugins/complexFunctions.py`

 * *Files identical despite different names*

### Comparing `BPTK_Py-1.7.6/BPTK_Py/sdcompiler/plugins/expandArrays.py` & `BPTK_Py-1.8.0/BPTK_Py/sdcompiler/plugins/expandArrays.py`

 * *Files identical despite different names*

### Comparing `BPTK_Py-1.7.6/BPTK_Py/sdcompiler/plugins/fixLabels.py` & `BPTK_Py-1.8.0/BPTK_Py/sdcompiler/plugins/fixLabels.py`

 * *Files identical despite different names*

### Comparing `BPTK_Py-1.7.6/BPTK_Py/sdcompiler/plugins/makeAbsolute.py` & `BPTK_Py-1.8.0/BPTK_Py/sdcompiler/plugins/makeAbsolute.py`

 * *Files identical despite different names*

### Comparing `BPTK_Py-1.7.6/BPTK_Py/sdcompiler/plugins/replaceDimensionNames.py` & `BPTK_Py-1.8.0/BPTK_Py/sdcompiler/plugins/replaceDimensionNames.py`

 * *Files identical despite different names*

### Comparing `BPTK_Py-1.7.6/BPTK_Py/sdcompiler/plugins/resolveAsterisk.py` & `BPTK_Py-1.8.0/BPTK_Py/sdcompiler/plugins/resolveAsterisk.py`

 * *Files identical despite different names*

### Comparing `BPTK_Py-1.7.6/BPTK_Py/sdcompiler/plugins/resolveSelf.py` & `BPTK_Py-1.8.0/BPTK_Py/sdcompiler/plugins/resolveSelf.py`

 * *Files identical despite different names*

### Comparing `BPTK_Py-1.7.6/BPTK_Py/sdcompiler/plugins/sanitizeNames.py` & `BPTK_Py-1.8.0/BPTK_Py/sdcompiler/plugins/sanitizeNames.py`

 * *Files identical despite different names*

### Comparing `BPTK_Py-1.7.6/BPTK_Py/sdcompiler/plugins/sortEntities.py` & `BPTK_Py-1.8.0/BPTK_Py/sdcompiler/plugins/sortEntities.py`

 * *Files identical despite different names*

### Comparing `BPTK_Py-1.7.6/BPTK_Py/sdcompiler/plugins/stockExpressions.py` & `BPTK_Py-1.8.0/BPTK_Py/sdcompiler/plugins/stockExpressions.py`

 * *Files identical despite different names*

### Comparing `BPTK_Py-1.7.6/BPTK_Py/sdcompiler/sdmodel.py` & `BPTK_Py-1.8.0/BPTK_Py/sdcompiler/sdmodel.py`

 * *Files identical despite different names*

### Comparing `BPTK_Py-1.7.6/BPTK_Py/sddsl/biflow.py` & `BPTK_Py-1.8.0/BPTK_Py/sddsl/biflow.py`

 * *Files identical despite different names*

### Comparing `BPTK_Py-1.7.6/BPTK_Py/sddsl/constant.py` & `BPTK_Py-1.8.0/BPTK_Py/sddsl/constant.py`

 * *Files identical despite different names*

### Comparing `BPTK_Py-1.7.6/BPTK_Py/sddsl/converter.py` & `BPTK_Py-1.8.0/BPTK_Py/sddsl/converter.py`

 * *Files identical despite different names*

### Comparing `BPTK_Py-1.7.6/BPTK_Py/sddsl/element.py` & `BPTK_Py-1.8.0/BPTK_Py/sddsl/element.py`

 * *Files identical despite different names*

### Comparing `BPTK_Py-1.7.6/BPTK_Py/sddsl/flow.py` & `BPTK_Py-1.8.0/BPTK_Py/sddsl/flow.py`

 * *Files identical despite different names*

### Comparing `BPTK_Py-1.7.6/BPTK_Py/sddsl/functions.py` & `BPTK_Py-1.8.0/BPTK_Py/sddsl/functions.py`

 * *Files identical despite different names*

### Comparing `BPTK_Py-1.7.6/BPTK_Py/sddsl/module.py` & `BPTK_Py-1.8.0/BPTK_Py/sddsl/module.py`

 * *Files identical despite different names*

### Comparing `BPTK_Py-1.7.6/BPTK_Py/sddsl/operators.py` & `BPTK_Py-1.8.0/BPTK_Py/sddsl/operators.py`

 * *Files identical despite different names*

### Comparing `BPTK_Py-1.7.6/BPTK_Py/sddsl/stock.py` & `BPTK_Py-1.8.0/BPTK_Py/sddsl/stock.py`

 * *Files identical despite different names*

### Comparing `BPTK_Py-1.7.6/BPTK_Py/sdsimulation/sd_simulation.py` & `BPTK_Py-1.8.0/BPTK_Py/sdsimulation/sd_simulation.py`

 * *Files identical despite different names*

### Comparing `BPTK_Py-1.7.6/BPTK_Py/server/bptkServer.py` & `BPTK_Py-1.8.0/BPTK_Py/server/bptkServer.py`

 * *Files 1% similar despite different names*

```diff
@@ -213,14 +213,15 @@
         self.route("/", methods=['GET'],strict_slashes=False)(self._home_resource)
         self.route("/healthy", methods=['GET'],strict_slashes=False)(self._healthy_resource)
         self.route("/run", methods=['POST', 'PUT'], strict_slashes=False)(self._run_resource)
         self.route("/scenarios", methods=['GET'], strict_slashes=False)(self._scenarios_resource)
         self.route("/equations", methods=['POST'], strict_slashes=False)(self._equations_resource)
         self.route("/agents", methods=['POST', 'PUT'], strict_slashes=False)(self._agents_resource)
         self.route("/start-instance", methods=['POST'], strict_slashes=False)(self._start_instance_resource)
+        self.route("/start-instances", methods=['POST'], strict_slashes=False)(self._start_instances_resource)
         self.route("/<instance_uuid>/run-step", methods=['POST'], strict_slashes=False)(self._run_step_resource)
         self.route("/<instance_uuid>/run-steps", methods=['POST'], strict_slashes=False)(self._run_steps_resource)
         self.route("/<instance_uuid>/stream-steps", methods=['POST'], strict_slashes=False)(self._stream_steps_resource)
         self.route("/<instance_uuid>/begin-session", methods=['POST'], strict_slashes=False)(self._begin_session_resource)
         self.route("/<instance_uuid>/end-session", methods=['POST'], strict_slashes=False)(self._end_session_resource)
         self.route("/<instance_uuid>/session-results", methods=['GET'], strict_slashes=False)(self._session_results_resource)
         self.route("/<instance_uuid>/flat-session-results", methods=['GET'], strict_slashes=False)(self._flat_session_results_resource)
@@ -550,30 +551,60 @@
 
         Arguments: timeout (dict,optional)
             The timeout period after which the instance is delete if it is not accessed in the meantime. The timer is reset every time the instance is accessed. The timeout dictionary can have the following keys: weeks, days, hours, minutes, seconds, milliseconds, microseconds. Values must be integers.
         """
 
         # store the new instance in the instance dictionary.
         timeout = {"weeks":0, "days":0, "hours":12, "minutes":0,"seconds":0,"milliseconds":0,"microseconds":0}
+        instances = 1
+        
         if request.is_json:
             content = request.get_json()
             if "timeout" in content:
                 timeout = content["timeout"]
         instance_uuid = self._instance_manager.create_instance(**timeout)
 
         if instance_uuid is not None:
-            resp = make_response(f'{{"instance_uuid":"{instance_uuid}","timeout":"{timeout}"}}', 200)
+            response_data = {"instance_uuid":instance_uuid,"timeout":timeout}
+            resp = make_response(json.dumps(response_data), 200)
         else:
             resp = make_response('{"error": "instance could not be started"}', 500)
 
         resp.headers['Content-Type']='application/json'
         resp.headers['Access-Control-Allow-Origin']='*'
         return resp
 
     @token_required
+    def _start_instances_resource(self):
+        """
+        This endpoint start N new instances of BPTK on the server side. The endpoint returns a list of instance_ids, which is needed to identify the instance in later calls.         
+        """
+
+        timeout = {"weeks":0, "days":0, "hours":12, "minutes":0,"seconds":0,"milliseconds":0,"microseconds":0}
+        instances = 1
+        instance_uuids = []
+        
+        if request.is_json:
+            content = request.get_json()
+            if "timeout" in content:
+                timeout = content["timeout"]
+            if "instances" in content:
+                instances = content["instances"]
+
+        for i in range(instances):
+            instance_uuids.append(self._instance_manager.create_instance(**timeout))
+
+        response_data={"instance_uuids":instance_uuids,"timeout":timeout}
+        
+        resp = make_response(json.dumps(response_data), 200)
+        resp.headers['Content-Type'] = 'application/json'
+        resp.headers['Access-Control-Allow-Origin'] = '*'
+        return resp
+
+    @token_required
     def _begin_session_resource(self, instance_uuid):
         """This endpoint starts a session for single step simulation. There can only be one session per instance at a time.
         Currently only System Dynamics scenarios are supported for both SD DSL and XMILE models.
         """
 
         if not request.is_json:
             resp = make_response('{"error": "please pass the request with content-type application/json"}', 500)
```

### Comparing `BPTK_Py-1.7.6/BPTK_Py/util/didyoumean.py` & `BPTK_Py-1.8.0/BPTK_Py/util/didyoumean.py`

 * *Files identical despite different names*

### Comparing `BPTK_Py-1.7.6/BPTK_Py/util/floating_point.py` & `BPTK_Py-1.8.0/BPTK_Py/util/floating_point.py`

 * *Files identical despite different names*

### Comparing `BPTK_Py-1.7.6/BPTK_Py/util/lookup_data.py` & `BPTK_Py-1.8.0/BPTK_Py/util/lookup_data.py`

 * *Files identical despite different names*

### Comparing `BPTK_Py-1.7.6/BPTK_Py/util/serializer.py` & `BPTK_Py-1.8.0/BPTK_Py/util/serializer.py`

 * *Files identical despite different names*

### Comparing `BPTK_Py-1.7.6/BPTK_Py/util/statecompression.py` & `BPTK_Py-1.8.0/BPTK_Py/util/statecompression.py`

 * *Files identical despite different names*

### Comparing `BPTK_Py-1.7.6/BPTK_Py/visualizations/simple_dashboard.py` & `BPTK_Py-1.8.0/BPTK_Py/visualizations/simple_dashboard.py`

 * *Files identical despite different names*

### Comparing `BPTK_Py-1.7.6/BPTK_Py/visualizations/visualize.py` & `BPTK_Py-1.8.0/BPTK_Py/visualizations/visualize.py`

 * *Files identical despite different names*

### Comparing `BPTK_Py-1.7.6/BPTK_Py/widgets/agentstatuswidget.py` & `BPTK_Py-1.8.0/BPTK_Py/widgets/agentstatuswidget.py`

 * *Files identical despite different names*

### Comparing `BPTK_Py-1.7.6/BPTK_Py/widgets/widget.py` & `BPTK_Py-1.8.0/BPTK_Py/widgets/widget.py`

 * *Files identical despite different names*

### Comparing `BPTK_Py-1.7.6/BPTK_Py.egg-info/PKG-INFO` & `BPTK_Py-1.8.0/BPTK_Py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BPTK-Py
-Version: 1.7.6
+Version: 1.8.0
 Summary: A python simulation engine for System Dynamics & Agent based models
 Home-page: https://www.transentis.com/business-prototyping-toolkit/en
 Author: transentis labs GmbH
 Author-email: support@transentis.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -49,14 +49,17 @@
 
 Our [beergame repository](https://github.com/transentis/bptk_py_tutorial/tree/master/model_library/beergame) contains Jupyter notebooks that analyse the Beergame in-depth and also provides XMILE, SD DSL and Agent-based versions of the Beergame.
 
 For any questions our suggestions you have regarding BPTK, please contact us at: [support@transentis.com](mailto:support@transentis.com).
 
 ## Changelog
 
+### 1.8.0
+* BPTKServer: Add new endpoint start-instances that starts multiple instances in one goo
+
 ### 1.7.6
 * BPTK: Improve handling of floating point numbers when using small DTs
 * ScenarioManagerSD: Fixed an issue that caused models with biflows to be cloned incorrectly
 
 ### 1.7.5
 * BPTK: Fix that caused a crash when using multiple scenario files for hybrid models
```

### Comparing `BPTK_Py-1.7.6/BPTK_Py.egg-info/SOURCES.txt` & `BPTK_Py-1.8.0/BPTK_Py.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -92,8 +92,13 @@
 BPTK_Py/util/serializer.py
 BPTK_Py/util/statecompression.py
 BPTK_Py/visualizations/__init__.py
 BPTK_Py/visualizations/simple_dashboard.py
 BPTK_Py/visualizations/visualize.py
 BPTK_Py/widgets/__init__.py
 BPTK_Py/widgets/agentstatuswidget.py
-BPTK_Py/widgets/widget.py
+BPTK_Py/widgets/widget.py
+tests/test_bptk.py
+tests/test_external_state.py
+tests/test_sddsl.py
+tests/test_server.py
+tests/test_xmile.py
```

### Comparing `BPTK_Py-1.7.6/LICENSE` & `BPTK_Py-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `BPTK_Py-1.7.6/PKG-INFO` & `BPTK_Py-1.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BPTK_Py
-Version: 1.7.6
+Version: 1.8.0
 Summary: A python simulation engine for System Dynamics & Agent based models
 Home-page: https://www.transentis.com/business-prototyping-toolkit/en
 Author: transentis labs GmbH
 Author-email: support@transentis.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -49,14 +49,17 @@
 
 Our [beergame repository](https://github.com/transentis/bptk_py_tutorial/tree/master/model_library/beergame) contains Jupyter notebooks that analyse the Beergame in-depth and also provides XMILE, SD DSL and Agent-based versions of the Beergame.
 
 For any questions our suggestions you have regarding BPTK, please contact us at: [support@transentis.com](mailto:support@transentis.com).
 
 ## Changelog
 
+### 1.8.0
+* BPTKServer: Add new endpoint start-instances that starts multiple instances in one goo
+
 ### 1.7.6
 * BPTK: Improve handling of floating point numbers when using small DTs
 * ScenarioManagerSD: Fixed an issue that caused models with biflows to be cloned incorrectly
 
 ### 1.7.5
 * BPTK: Fix that caused a crash when using multiple scenario files for hybrid models
```

### Comparing `BPTK_Py-1.7.6/README.md` & `BPTK_Py-1.8.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,17 @@
 
 Our [beergame repository](https://github.com/transentis/bptk_py_tutorial/tree/master/model_library/beergame) contains Jupyter notebooks that analyse the Beergame in-depth and also provides XMILE, SD DSL and Agent-based versions of the Beergame.
 
 For any questions our suggestions you have regarding BPTK, please contact us at: [support@transentis.com](mailto:support@transentis.com).
 
 ## Changelog
 
+### 1.8.0
+* BPTKServer: Add new endpoint start-instances that starts multiple instances in one goo
+
 ### 1.7.6
 * BPTK: Improve handling of floating point numbers when using small DTs
 * ScenarioManagerSD: Fixed an issue that caused models with biflows to be cloned incorrectly
 
 ### 1.7.5
 * BPTK: Fix that caused a crash when using multiple scenario files for hybrid models
```

### Comparing `BPTK_Py-1.7.6/setup.py` & `BPTK_Py-1.8.0/setup.py`

 * *Files identical despite different names*

