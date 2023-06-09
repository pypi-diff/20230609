# Comparing `tmp/Accuinsight-3.4.230516rc1.tar.gz` & `tmp/Accuinsight-3.4.230530.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Accuinsight-3.4.230516rc1.tar", last modified: Tue May 16 00:46:37 2023, max compression
+gzip compressed data, was "Accuinsight-3.4.230530.tar", last modified: Tue May 30 04:45:23 2023, max compression
```

## Comparing `Accuinsight-3.4.230516rc1.tar` & `Accuinsight-3.4.230530.tar`

### file list

```diff
@@ -1,132 +1,127 @@
-drwxr-xr-x   0 a10894     (501) staff       (20)        0 2023-05-16 00:46:37.602403 Accuinsight-3.4.230516rc1/
-drwxr-xr-x   0 a10894     (501) staff       (20)        0 2023-05-16 00:46:37.155850 Accuinsight-3.4.230516rc1/Accuinsight/
-drwxr-xr-x   0 a10894     (501) staff       (20)        0 2023-05-16 00:46:37.201678 Accuinsight-3.4.230516rc1/Accuinsight/Lifecycle/
--rw-r--r--   0 a10894     (501) staff       (20)    23813 2023-05-10 02:33:36.000000 Accuinsight-3.4.230516rc1/Accuinsight/Lifecycle/ML.py
--rw-r--r--   0 a10894     (501) staff       (20)        0 2023-03-14 00:39:55.000000 Accuinsight-3.4.230516rc1/Accuinsight/Lifecycle/__init__.py
--rw-r--r--   0 a10894     (501) staff       (20)    17408 2023-03-22 07:26:18.000000 Accuinsight-3.4.230516rc1/Accuinsight/Lifecycle/common.py
--rw-r--r--   0 a10894     (501) staff       (20)    26875 2023-05-10 05:06:10.000000 Accuinsight-3.4.230516rc1/Accuinsight/Lifecycle/keras.py
--rw-r--r--   0 a10894     (501) staff       (20)      983 2023-03-14 00:39:55.000000 Accuinsight-3.4.230516rc1/Accuinsight/Lifecycle/settings.py
--rw-r--r--   0 a10894     (501) staff       (20)    26656 2023-05-10 05:06:10.000000 Accuinsight-3.4.230516rc1/Accuinsight/Lifecycle/tensorflow.py
--rw-r--r--   0 a10894     (501) staff       (20)     2795 2023-05-10 05:06:10.000000 Accuinsight-3.4.230516rc1/Accuinsight/Lifecycle/utils.py
-drwxr-xr-x   0 a10894     (501) staff       (20)        0 2023-05-16 00:46:37.203496 Accuinsight-3.4.230516rc1/Accuinsight/Monitoring/
--rw-r--r--   0 a10894     (501) staff       (20)       20 2023-03-14 00:39:55.000000 Accuinsight-3.4.230516rc1/Accuinsight/Monitoring/__init__.py
-drwxr-xr-x   0 a10894     (501) staff       (20)        0 2023-05-16 00:46:37.207076 Accuinsight-3.4.230516rc1/Accuinsight/Monitoring/deploy/
--rw-r--r--   0 a10894     (501) staff       (20)      101 2023-03-14 00:39:55.000000 Accuinsight-3.4.230516rc1/Accuinsight/Monitoring/deploy/__init__.py
--rw-r--r--   0 a10894     (501) staff       (20)     3987 2023-03-14 00:39:55.000000 Accuinsight-3.4.230516rc1/Accuinsight/Monitoring/deploy/monitoring_deploy.py
-drwxr-xr-x   0 a10894     (501) staff       (20)        0 2023-05-16 00:46:37.211449 Accuinsight-3.4.230516rc1/Accuinsight/WorkspaceRun/
--rw-r--r--   0 a10894     (501) staff       (20)       92 2023-03-14 00:39:55.000000 Accuinsight-3.4.230516rc1/Accuinsight/WorkspaceRun/__init__.py
--rw-r--r--   0 a10894     (501) staff       (20)     3763 2023-05-08 04:59:50.000000 Accuinsight-3.4.230516rc1/Accuinsight/WorkspaceRun/workspace_run.py
--rw-r--r--   0 a10894     (501) staff       (20)      178 2023-05-16 00:45:44.000000 Accuinsight-3.4.230516rc1/Accuinsight/__about__.py
--rw-r--r--   0 a10894     (501) staff       (20)      353 2023-03-14 00:39:55.000000 Accuinsight-3.4.230516rc1/Accuinsight/__init__.py
--rw-r--r--   0 a10894     (501) staff       (20)     3042 2023-03-14 00:39:55.000000 Accuinsight-3.4.230516rc1/Accuinsight/exceptions.py
--rw-r--r--   0 a10894     (501) staff       (20)      205 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/info.py
-drwxr-xr-x   0 a10894     (501) staff       (20)        0 2023-05-16 00:46:37.243920 Accuinsight-3.4.230516rc1/Accuinsight/modeler/
--rw-r--r--   0 a10894     (501) staff       (20)        0 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/__init__.py
-drwxr-xr-x   0 a10894     (501) staff       (20)        0 2023-05-16 00:46:37.250584 Accuinsight-3.4.230516rc1/Accuinsight/modeler/clients/
--rw-r--r--   0 a10894     (501) staff       (20)        0 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/clients/__init__.py
--rw-r--r--   0 a10894     (501) staff       (20)     2053 2023-04-17 02:18:35.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/clients/modeler_api.py
-drwxr-xr-x   0 a10894     (501) staff       (20)        0 2023-05-16 00:46:37.301913 Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/
-drwxr-xr-x   0 a10894     (501) staff       (20)        0 2023-05-16 00:46:37.306946 Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/LcConst/
--rw-r--r--   0 a10894     (501) staff       (20)     2786 2023-05-10 01:48:37.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/LcConst/LcConst.py
--rw-r--r--   0 a10894     (501) staff       (20)       27 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/LcConst/__init__.py
--rw-r--r--   0 a10894     (501) staff       (20)      460 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/Lifecycle.py
--rw-r--r--   0 a10894     (501) staff       (20)      730 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/ModelType.py
-drwxr-xr-x   0 a10894     (501) staff       (20)        0 2023-05-16 00:46:37.309011 Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/MonitoringConst/
--rw-r--r--   0 a10894     (501) staff       (20)        0 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/MonitoringConst/__init__.py
-drwxr-xr-x   0 a10894     (501) staff       (20)        0 2023-05-16 00:46:37.313821 Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/MonitoringConst/deploy/
--rw-r--r--   0 a10894     (501) staff       (20)      219 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/MonitoringConst/deploy/DeployConst.py
--rw-r--r--   0 a10894     (501) staff       (20)       31 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/MonitoringConst/deploy/__init__.py
-drwxr-xr-x   0 a10894     (501) staff       (20)        0 2023-05-16 00:46:37.336373 Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/Run/
-drwxr-xr-x   0 a10894     (501) staff       (20)        0 2023-05-16 00:46:37.405994 Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/Run/ParseRun/
--rw-r--r--   0 a10894     (501) staff       (20)     4185 2023-05-08 05:02:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/Run/ParseRun/BaseParser.py
--rw-r--r--   0 a10894     (501) staff       (20)     2387 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/Run/ParseRun/ParseExperiment.py
--rw-r--r--   0 a10894     (501) staff       (20)     3556 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/Run/ParseRun/ParseKeras.py
--rw-r--r--   0 a10894     (501) staff       (20)     6127 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/Run/ParseRun/Parse_DLClassification.py
--rw-r--r--   0 a10894     (501) staff       (20)     3877 2023-05-10 05:06:10.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/Run/ParseRun/Parse_DLClassification_evl.py
--rw-r--r--   0 a10894     (501) staff       (20)     6899 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/Run/ParseRun/Parse_DLRegression.py
--rw-r--r--   0 a10894     (501) staff       (20)     4901 2023-05-10 05:06:10.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/Run/ParseRun/Parse_DLRegression_evl.py
--rw-r--r--   0 a10894     (501) staff       (20)      381 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/Run/ParseRun/Parse_Helper.py
--rw-r--r--   0 a10894     (501) staff       (20)     4069 2023-05-08 05:02:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/Run/ParseRun/Parse_MLClassifier.py
--rw-r--r--   0 a10894     (501) staff       (20)     2506 2023-05-10 05:06:10.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/Run/ParseRun/Parse_MLClassifier_evl.py
--rw-r--r--   0 a10894     (501) staff       (20)     6902 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/Run/ParseRun/Parse_MLRegression.py
--rw-r--r--   0 a10894     (501) staff       (20)     5146 2023-05-10 05:06:10.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/Run/ParseRun/Parse_MLRegression_evl.py
--rw-r--r--   0 a10894     (501) staff       (20)     4641 2023-04-27 02:41:11.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/Run/ParseRun/ParserVisualJaon.py
--rw-r--r--   0 a10894     (501) staff       (20)       30 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/Run/ParseRun/__init__.py
-drwxr-xr-x   0 a10894     (501) staff       (20)        0 2023-05-16 00:46:37.410831 Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/Run/RunInfo/
--rw-r--r--   0 a10894     (501) staff       (20)    13570 2023-05-10 05:06:10.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/Run/RunInfo/RunInfo.py
--rw-r--r--   0 a10894     (501) staff       (20)       26 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/Run/RunInfo/__init__.py
--rw-r--r--   0 a10894     (501) staff       (20)     1615 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/Run/RunOjbject.py
--rw-r--r--   0 a10894     (501) staff       (20)        0 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/Run/__init__.py
--rw-r--r--   0 a10894     (501) staff       (20)        0 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/__init__.py
--rw-r--r--   0 a10894     (501) staff       (20)     1878 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/feature_contribution.py
--rw-r--r--   0 a10894     (501) staff       (20)      311 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/func.py
--rw-r--r--   0 a10894     (501) staff       (20)     6753 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/func_for_visual.py
--rw-r--r--   0 a10894     (501) staff       (20)     5931 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/get.py
--rw-r--r--   0 a10894     (501) staff       (20)     7618 2023-05-10 05:06:10.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/get_for_visual.py
--rw-r--r--   0 a10894     (501) staff       (20)      823 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/lossFuncInfo.py
--rw-r--r--   0 a10894     (501) staff       (20)     1144 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/metricsLightgbm.py
--rw-r--r--   0 a10894     (501) staff       (20)     1884 2023-05-10 05:06:10.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/modelEvaluation.py
--rw-r--r--   0 a10894     (501) staff       (20)     8437 2023-04-27 06:49:04.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/path.py
--rw-r--r--   0 a10894     (501) staff       (20)      361 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/sklearnModelType.py
-drwxr-xr-x   0 a10894     (501) staff       (20)        0 2023-05-16 00:46:37.468671 Accuinsight-3.4.230516rc1/Accuinsight/modeler/entities/
--rw-r--r--   0 a10894     (501) staff       (20)      500 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/entities/__init__.py
--rw-r--r--   0 a10894     (501) staff       (20)     1491 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/entities/_modeler_object.py
--rw-r--r--   0 a10894     (501) staff       (20)     1278 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/entities/alarm.py
--rw-r--r--   0 a10894     (501) staff       (20)      803 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/entities/lc_artifact.py
--rw-r--r--   0 a10894     (501) staff       (20)     1204 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/entities/lc_metric.py
--rw-r--r--   0 a10894     (501) staff       (20)      970 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/entities/lc_param.py
--rw-r--r--   0 a10894     (501) staff       (20)      624 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/entities/lc_run.py
--rw-r--r--   0 a10894     (501) staff       (20)     5712 2023-04-17 02:35:03.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/entities/lc_run_info.py
--rw-r--r--   0 a10894     (501) staff       (20)     1506 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/entities/lc_run_status.py
--rw-r--r--   0 a10894     (501) staff       (20)      918 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/entities/lc_run_tag.py
--rw-r--r--   0 a10894     (501) staff       (20)     1287 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/entities/lc_stage.py
--rw-r--r--   0 a10894     (501) staff       (20)     1836 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/entities/lc_view_type.py
--rw-r--r--   0 a10894     (501) staff       (20)     3638 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/entities/monitoring_deploy_log.py
--rw-r--r--   0 a10894     (501) staff       (20)     1286 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/entities/workspace_run_log.py
--rw-r--r--   0 a10894     (501) staff       (20)     3050 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/exceptions.py
--rw-r--r--   0 a10894     (501) staff       (20)      205 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/info.py
-drwxr-xr-x   0 a10894     (501) staff       (20)        0 2023-05-16 00:46:37.505642 Accuinsight-3.4.230516rc1/Accuinsight/modeler/protos/
--rw-r--r--   0 a10894     (501) staff       (20)        0 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/protos/__init__.py
--rw-r--r--   0 a10894     (501) staff       (20)    37721 2023-04-25 08:22:55.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/protos/life_cycle_pb2.py
--rw-r--r--   0 a10894     (501) staff       (20)   107276 2023-04-25 08:22:55.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/protos/service_pb2.py
--rw-r--r--   0 a10894     (501) staff       (20)    27025 2023-04-25 08:22:55.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/protos/skapi_pb2.py
-drwxr-xr-x   0 a10894     (501) staff       (20)        0 2023-05-16 00:46:37.540087 Accuinsight-3.4.230516rc1/Accuinsight/modeler/protos_bak/
--rw-r--r--   0 a10894     (501) staff       (20)        0 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/protos_bak/__init__.py
--rw-r--r--   0 a10894     (501) staff       (20)    36510 2023-03-16 01:29:02.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/protos_bak/life_cycle_pb2.py
--rw-r--r--   0 a10894     (501) staff       (20)   107276 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/protos_bak/service_pb2.py
--rw-r--r--   0 a10894     (501) staff       (20)    27025 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/protos_bak/skapi_pb2.py
-drwxr-xr-x   0 a10894     (501) staff       (20)        0 2023-05-16 00:46:37.542016 Accuinsight-3.4.230516rc1/Accuinsight/modeler/store/
--rw-r--r--   0 a10894     (501) staff       (20)        0 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/store/__init__.py
-drwxr-xr-x   0 a10894     (501) staff       (20)        0 2023-05-16 00:46:37.555128 Accuinsight-3.4.230516rc1/Accuinsight/modeler/store/tracking/
--rw-r--r--   0 a10894     (501) staff       (20)      315 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/store/tracking/__init__.py
--rw-r--r--   0 a10894     (501) staff       (20)      957 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/store/tracking/lc_abstract_store.py
--rw-r--r--   0 a10894     (501) staff       (20)     6918 2023-04-27 02:45:39.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/store/tracking/life_cycle_store.py
--rw-r--r--   0 a10894     (501) staff       (20)     1789 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/store/tracking/monitoring_deploy_store.py
--rw-r--r--   0 a10894     (501) staff       (20)     1416 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/store/tracking/workspace_store.py
-drwxr-xr-x   0 a10894     (501) staff       (20)        0 2023-05-16 00:46:37.594904 Accuinsight-3.4.230516rc1/Accuinsight/modeler/utils/
--rw-r--r--   0 a10894     (501) staff       (20)     1619 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/utils/__init__.py
--rw-r--r--   0 a10894     (501) staff       (20)      365 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/utils/annotations.py
-drwxr-xr-x   0 a10894     (501) staff       (20)        0 2023-05-16 00:46:37.601029 Accuinsight-3.4.230516rc1/Accuinsight/modeler/utils/dependency/
--rw-r--r--   0 a10894     (501) staff       (20)        0 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/utils/dependency/__init__.py
--rw-r--r--   0 a10894     (501) staff       (20)    19325 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/utils/dependency/dependencies.py
--rw-r--r--   0 a10894     (501) staff       (20)     2209 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/utils/dependency/settings.py
--rw-r--r--   0 a10894     (501) staff       (20)     1202 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/utils/dl_utils.py
--rwxr-xr-x   0 a10894     (501) staff       (20)     4122 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/utils/os_getenv.py
--rw-r--r--   0 a10894     (501) staff       (20)     1175 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/utils/proto_json_utils.py
--rwxr-xr-x   0 a10894     (501) staff       (20)    11063 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/utils/rest_utils.py
--rw-r--r--   0 a10894     (501) staff       (20)     2433 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/utils/runs_utils.py
--rw-r--r--   0 a10894     (501) staff       (20)      367 2023-03-22 07:23:16.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/utils/string_utils.py
-drwxr-xr-x   0 a10894     (501) staff       (20)        0 2023-05-16 00:46:37.169055 Accuinsight-3.4.230516rc1/Accuinsight.egg-info/
--rw-r--r--   0 a10894     (501) staff       (20)     2269 2023-05-16 00:46:36.000000 Accuinsight-3.4.230516rc1/Accuinsight.egg-info/PKG-INFO
--rw-r--r--   0 a10894     (501) staff       (20)     4528 2023-05-16 00:46:36.000000 Accuinsight-3.4.230516rc1/Accuinsight.egg-info/SOURCES.txt
--rw-r--r--   0 a10894     (501) staff       (20)        1 2023-05-16 00:46:36.000000 Accuinsight-3.4.230516rc1/Accuinsight.egg-info/dependency_links.txt
--rw-r--r--   0 a10894     (501) staff       (20)        1 2023-05-16 00:46:36.000000 Accuinsight-3.4.230516rc1/Accuinsight.egg-info/not-zip-safe
--rw-r--r--   0 a10894     (501) staff       (20)      281 2023-05-16 00:46:36.000000 Accuinsight-3.4.230516rc1/Accuinsight.egg-info/requires.txt
--rw-r--r--   0 a10894     (501) staff       (20)       12 2023-05-16 00:46:36.000000 Accuinsight-3.4.230516rc1/Accuinsight.egg-info/top_level.txt
--rw-r--r--   0 a10894     (501) staff       (20)       21 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/LICENSE.txt
--rw-r--r--   0 a10894     (501) staff       (20)       63 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/MANIFEST.in
--rw-r--r--   0 a10894     (501) staff       (20)     2269 2023-05-16 00:46:37.602673 Accuinsight-3.4.230516rc1/PKG-INFO
--rw-r--r--   0 a10894     (501) staff       (20)     1487 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/README.rst
--rw-r--r--   0 a10894     (501) staff       (20)      280 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/requirements.txt
--rw-r--r--   0 a10894     (501) staff       (20)      256 2023-05-16 00:46:37.604569 Accuinsight-3.4.230516rc1/setup.cfg
--rw-r--r--   0 a10894     (501) staff       (20)     1294 2023-03-14 00:40:01.000000 Accuinsight-3.4.230516rc1/setup.py
+drwxr-xr-x   0 a10894     (501) staff       (20)        0 2023-05-30 04:45:23.710934 Accuinsight-3.4.230530/
+drwxr-xr-x   0 a10894     (501) staff       (20)        0 2023-05-30 04:45:23.515440 Accuinsight-3.4.230530/Accuinsight/
+drwxr-xr-x   0 a10894     (501) staff       (20)        0 2023-05-30 04:45:23.547011 Accuinsight-3.4.230530/Accuinsight/Lifecycle/
+-rw-rw-r--   0 a10894     (501) staff       (20)    24642 2023-05-30 04:42:08.000000 Accuinsight-3.4.230530/Accuinsight/Lifecycle/ML.py
+-rw-rw-r--   0 a10894     (501) staff       (20)        0 2023-05-30 04:42:08.000000 Accuinsight-3.4.230530/Accuinsight/Lifecycle/__init__.py
+-rw-rw-r--   0 a10894     (501) staff       (20)    17963 2023-05-30 04:42:08.000000 Accuinsight-3.4.230530/Accuinsight/Lifecycle/common.py
+-rw-rw-r--   0 a10894     (501) staff       (20)    27519 2023-05-30 04:42:08.000000 Accuinsight-3.4.230530/Accuinsight/Lifecycle/keras.py
+-rw-rw-r--   0 a10894     (501) staff       (20)      983 2023-05-30 04:42:08.000000 Accuinsight-3.4.230530/Accuinsight/Lifecycle/settings.py
+-rw-rw-r--   0 a10894     (501) staff       (20)    27551 2023-05-30 04:42:08.000000 Accuinsight-3.4.230530/Accuinsight/Lifecycle/tensorflow.py
+-rw-rw-r--   0 a10894     (501) staff       (20)     2795 2023-05-30 04:42:08.000000 Accuinsight-3.4.230530/Accuinsight/Lifecycle/utils.py
+drwxr-xr-x   0 a10894     (501) staff       (20)        0 2023-05-30 04:45:23.547909 Accuinsight-3.4.230530/Accuinsight/Monitoring/
+-rw-rw-r--   0 a10894     (501) staff       (20)       20 2023-05-30 04:42:08.000000 Accuinsight-3.4.230530/Accuinsight/Monitoring/__init__.py
+drwxr-xr-x   0 a10894     (501) staff       (20)        0 2023-05-30 04:45:23.549893 Accuinsight-3.4.230530/Accuinsight/Monitoring/deploy/
+-rw-rw-r--   0 a10894     (501) staff       (20)      101 2023-05-30 04:42:08.000000 Accuinsight-3.4.230530/Accuinsight/Monitoring/deploy/__init__.py
+-rw-rw-r--   0 a10894     (501) staff       (20)     3987 2023-05-30 04:42:08.000000 Accuinsight-3.4.230530/Accuinsight/Monitoring/deploy/monitoring_deploy.py
+drwxr-xr-x   0 a10894     (501) staff       (20)        0 2023-05-30 04:45:23.551753 Accuinsight-3.4.230530/Accuinsight/WorkspaceRun/
+-rw-rw-r--   0 a10894     (501) staff       (20)       92 2023-05-30 04:42:08.000000 Accuinsight-3.4.230530/Accuinsight/WorkspaceRun/__init__.py
+-rw-rw-r--   0 a10894     (501) staff       (20)     3763 2023-05-30 04:42:08.000000 Accuinsight-3.4.230530/Accuinsight/WorkspaceRun/workspace_run.py
+-rw-rw-r--   0 a10894     (501) staff       (20)      174 2023-05-30 04:45:00.000000 Accuinsight-3.4.230530/Accuinsight/__about__.py
+-rw-rw-r--   0 a10894     (501) staff       (20)      353 2023-05-30 04:42:08.000000 Accuinsight-3.4.230530/Accuinsight/__init__.py
+-rw-rw-r--   0 a10894     (501) staff       (20)     3042 2023-05-30 04:42:08.000000 Accuinsight-3.4.230530/Accuinsight/exceptions.py
+-rw-rw-r--   0 a10894     (501) staff       (20)      205 2023-05-30 04:42:08.000000 Accuinsight-3.4.230530/Accuinsight/info.py
+drwxr-xr-x   0 a10894     (501) staff       (20)        0 2023-05-30 04:45:23.554519 Accuinsight-3.4.230530/Accuinsight/modeler/
+-rw-rw-r--   0 a10894     (501) staff       (20)        0 2023-05-30 04:42:08.000000 Accuinsight-3.4.230530/Accuinsight/modeler/__init__.py
+drwxr-xr-x   0 a10894     (501) staff       (20)        0 2023-05-30 04:45:23.556068 Accuinsight-3.4.230530/Accuinsight/modeler/clients/
+-rw-rw-r--   0 a10894     (501) staff       (20)        0 2023-05-30 04:42:08.000000 Accuinsight-3.4.230530/Accuinsight/modeler/clients/__init__.py
+-rw-rw-r--   0 a10894     (501) staff       (20)     2053 2023-05-30 04:42:08.000000 Accuinsight-3.4.230530/Accuinsight/modeler/clients/modeler_api.py
+drwxr-xr-x   0 a10894     (501) staff       (20)        0 2023-05-30 04:45:23.570185 Accuinsight-3.4.230530/Accuinsight/modeler/core/
+drwxr-xr-x   0 a10894     (501) staff       (20)        0 2023-05-30 04:45:23.590849 Accuinsight-3.4.230530/Accuinsight/modeler/core/LcConst/
+-rw-rw-r--   0 a10894     (501) staff       (20)     2786 2023-05-30 04:42:08.000000 Accuinsight-3.4.230530/Accuinsight/modeler/core/LcConst/LcConst.py
+-rw-rw-r--   0 a10894     (501) staff       (20)       27 2023-05-30 04:42:08.000000 Accuinsight-3.4.230530/Accuinsight/modeler/core/LcConst/__init__.py
+-rw-rw-r--   0 a10894     (501) staff       (20)      460 2023-05-30 04:42:08.000000 Accuinsight-3.4.230530/Accuinsight/modeler/core/Lifecycle.py
+-rw-rw-r--   0 a10894     (501) staff       (20)      730 2023-05-30 04:42:08.000000 Accuinsight-3.4.230530/Accuinsight/modeler/core/ModelType.py
+drwxr-xr-x   0 a10894     (501) staff       (20)        0 2023-05-30 04:45:23.592672 Accuinsight-3.4.230530/Accuinsight/modeler/core/MonitoringConst/
+-rw-rw-r--   0 a10894     (501) staff       (20)        0 2023-05-30 04:42:08.000000 Accuinsight-3.4.230530/Accuinsight/modeler/core/MonitoringConst/__init__.py
+drwxr-xr-x   0 a10894     (501) staff       (20)        0 2023-05-30 04:45:23.595097 Accuinsight-3.4.230530/Accuinsight/modeler/core/MonitoringConst/deploy/
+-rw-rw-r--   0 a10894     (501) staff       (20)      219 2023-05-30 04:42:08.000000 Accuinsight-3.4.230530/Accuinsight/modeler/core/MonitoringConst/deploy/DeployConst.py
+-rw-rw-r--   0 a10894     (501) staff       (20)       31 2023-05-30 04:42:08.000000 Accuinsight-3.4.230530/Accuinsight/modeler/core/MonitoringConst/deploy/__init__.py
+drwxr-xr-x   0 a10894     (501) staff       (20)        0 2023-05-30 04:45:23.597562 Accuinsight-3.4.230530/Accuinsight/modeler/core/Run/
+drwxr-xr-x   0 a10894     (501) staff       (20)        0 2023-05-30 04:45:23.615188 Accuinsight-3.4.230530/Accuinsight/modeler/core/Run/ParseRun/
+-rw-rw-r--   0 a10894     (501) staff       (20)     4185 2023-05-30 04:42:08.000000 Accuinsight-3.4.230530/Accuinsight/modeler/core/Run/ParseRun/BaseParser.py
+-rw-rw-r--   0 a10894     (501) staff       (20)     2387 2023-05-30 04:42:08.000000 Accuinsight-3.4.230530/Accuinsight/modeler/core/Run/ParseRun/ParseExperiment.py
+-rw-rw-r--   0 a10894     (501) staff       (20)     3556 2023-05-30 04:42:08.000000 Accuinsight-3.4.230530/Accuinsight/modeler/core/Run/ParseRun/ParseKeras.py
+-rw-rw-r--   0 a10894     (501) staff       (20)     6127 2023-05-30 04:42:08.000000 Accuinsight-3.4.230530/Accuinsight/modeler/core/Run/ParseRun/Parse_DLClassification.py
+-rw-rw-r--   0 a10894     (501) staff       (20)     3877 2023-05-30 04:42:08.000000 Accuinsight-3.4.230530/Accuinsight/modeler/core/Run/ParseRun/Parse_DLClassification_evl.py
+-rw-rw-r--   0 a10894     (501) staff       (20)     6899 2023-05-30 04:42:08.000000 Accuinsight-3.4.230530/Accuinsight/modeler/core/Run/ParseRun/Parse_DLRegression.py
+-rw-rw-r--   0 a10894     (501) staff       (20)     4901 2023-05-30 04:42:08.000000 Accuinsight-3.4.230530/Accuinsight/modeler/core/Run/ParseRun/Parse_DLRegression_evl.py
+-rw-rw-r--   0 a10894     (501) staff       (20)      381 2023-05-30 04:42:08.000000 Accuinsight-3.4.230530/Accuinsight/modeler/core/Run/ParseRun/Parse_Helper.py
+-rw-rw-r--   0 a10894     (501) staff       (20)     4069 2023-05-30 04:42:08.000000 Accuinsight-3.4.230530/Accuinsight/modeler/core/Run/ParseRun/Parse_MLClassifier.py
+-rw-rw-r--   0 a10894     (501) staff       (20)     2506 2023-05-30 04:42:08.000000 Accuinsight-3.4.230530/Accuinsight/modeler/core/Run/ParseRun/Parse_MLClassifier_evl.py
+-rw-rw-r--   0 a10894     (501) staff       (20)     6902 2023-05-30 04:42:08.000000 Accuinsight-3.4.230530/Accuinsight/modeler/core/Run/ParseRun/Parse_MLRegression.py
+-rw-rw-r--   0 a10894     (501) staff       (20)     5146 2023-05-30 04:42:08.000000 Accuinsight-3.4.230530/Accuinsight/modeler/core/Run/ParseRun/Parse_MLRegression_evl.py
+-rw-rw-r--   0 a10894     (501) staff       (20)     4641 2023-05-30 04:42:08.000000 Accuinsight-3.4.230530/Accuinsight/modeler/core/Run/ParseRun/ParserVisualJaon.py
+-rw-rw-r--   0 a10894     (501) staff       (20)       30 2023-05-30 04:42:08.000000 Accuinsight-3.4.230530/Accuinsight/modeler/core/Run/ParseRun/__init__.py
+drwxr-xr-x   0 a10894     (501) staff       (20)        0 2023-05-30 04:45:23.617929 Accuinsight-3.4.230530/Accuinsight/modeler/core/Run/RunInfo/
+-rw-rw-r--   0 a10894     (501) staff       (20)    13570 2023-05-30 04:42:08.000000 Accuinsight-3.4.230530/Accuinsight/modeler/core/Run/RunInfo/RunInfo.py
+-rw-rw-r--   0 a10894     (501) staff       (20)       26 2023-05-30 04:42:08.000000 Accuinsight-3.4.230530/Accuinsight/modeler/core/Run/RunInfo/__init__.py
+-rw-rw-r--   0 a10894     (501) staff       (20)     1615 2023-05-30 04:42:08.000000 Accuinsight-3.4.230530/Accuinsight/modeler/core/Run/RunOjbject.py
+-rw-rw-r--   0 a10894     (501) staff       (20)        0 2023-05-30 04:42:08.000000 Accuinsight-3.4.230530/Accuinsight/modeler/core/Run/__init__.py
+-rw-rw-r--   0 a10894     (501) staff       (20)        0 2023-05-30 04:42:08.000000 Accuinsight-3.4.230530/Accuinsight/modeler/core/__init__.py
+-rw-rw-r--   0 a10894     (501) staff       (20)     1878 2023-05-30 04:42:08.000000 Accuinsight-3.4.230530/Accuinsight/modeler/core/feature_contribution.py
+-rw-rw-r--   0 a10894     (501) staff       (20)      311 2023-05-30 04:42:08.000000 Accuinsight-3.4.230530/Accuinsight/modeler/core/func.py
+-rw-rw-r--   0 a10894     (501) staff       (20)     6753 2023-05-30 04:42:08.000000 Accuinsight-3.4.230530/Accuinsight/modeler/core/func_for_visual.py
+-rw-rw-r--   0 a10894     (501) staff       (20)     5931 2023-05-30 04:42:08.000000 Accuinsight-3.4.230530/Accuinsight/modeler/core/get.py
+-rw-rw-r--   0 a10894     (501) staff       (20)     7618 2023-05-30 04:42:08.000000 Accuinsight-3.4.230530/Accuinsight/modeler/core/get_for_visual.py
+-rw-rw-r--   0 a10894     (501) staff       (20)      823 2023-05-30 04:42:08.000000 Accuinsight-3.4.230530/Accuinsight/modeler/core/lossFuncInfo.py
+-rw-rw-r--   0 a10894     (501) staff       (20)     1144 2023-05-30 04:42:08.000000 Accuinsight-3.4.230530/Accuinsight/modeler/core/metricsLightgbm.py
+-rw-rw-r--   0 a10894     (501) staff       (20)     1884 2023-05-30 04:42:08.000000 Accuinsight-3.4.230530/Accuinsight/modeler/core/modelEvaluation.py
+-rw-rw-r--   0 a10894     (501) staff       (20)     8437 2023-05-30 04:42:08.000000 Accuinsight-3.4.230530/Accuinsight/modeler/core/path.py
+-rw-rw-r--   0 a10894     (501) staff       (20)      361 2023-05-30 04:42:08.000000 Accuinsight-3.4.230530/Accuinsight/modeler/core/sklearnModelType.py
+drwxr-xr-x   0 a10894     (501) staff       (20)        0 2023-05-30 04:45:23.669088 Accuinsight-3.4.230530/Accuinsight/modeler/entities/
+-rw-rw-r--   0 a10894     (501) staff       (20)      500 2023-05-30 04:42:08.000000 Accuinsight-3.4.230530/Accuinsight/modeler/entities/__init__.py
+-rw-rw-r--   0 a10894     (501) staff       (20)     1491 2023-05-30 04:42:08.000000 Accuinsight-3.4.230530/Accuinsight/modeler/entities/_modeler_object.py
+-rw-rw-r--   0 a10894     (501) staff       (20)     1278 2023-05-30 04:42:08.000000 Accuinsight-3.4.230530/Accuinsight/modeler/entities/alarm.py
+-rw-rw-r--   0 a10894     (501) staff       (20)      803 2023-05-30 04:42:08.000000 Accuinsight-3.4.230530/Accuinsight/modeler/entities/lc_artifact.py
+-rw-rw-r--   0 a10894     (501) staff       (20)     1204 2023-05-30 04:42:08.000000 Accuinsight-3.4.230530/Accuinsight/modeler/entities/lc_metric.py
+-rw-rw-r--   0 a10894     (501) staff       (20)      970 2023-05-30 04:42:08.000000 Accuinsight-3.4.230530/Accuinsight/modeler/entities/lc_param.py
+-rw-rw-r--   0 a10894     (501) staff       (20)      624 2023-05-30 04:42:08.000000 Accuinsight-3.4.230530/Accuinsight/modeler/entities/lc_run.py
+-rw-rw-r--   0 a10894     (501) staff       (20)     5712 2023-05-30 04:42:08.000000 Accuinsight-3.4.230530/Accuinsight/modeler/entities/lc_run_info.py
+-rw-rw-r--   0 a10894     (501) staff       (20)     1506 2023-05-30 04:42:08.000000 Accuinsight-3.4.230530/Accuinsight/modeler/entities/lc_run_status.py
+-rw-rw-r--   0 a10894     (501) staff       (20)      918 2023-05-30 04:42:08.000000 Accuinsight-3.4.230530/Accuinsight/modeler/entities/lc_run_tag.py
+-rw-rw-r--   0 a10894     (501) staff       (20)     1287 2023-05-30 04:42:08.000000 Accuinsight-3.4.230530/Accuinsight/modeler/entities/lc_stage.py
+-rw-rw-r--   0 a10894     (501) staff       (20)     1836 2023-05-30 04:42:08.000000 Accuinsight-3.4.230530/Accuinsight/modeler/entities/lc_view_type.py
+-rw-rw-r--   0 a10894     (501) staff       (20)     3638 2023-05-30 04:42:08.000000 Accuinsight-3.4.230530/Accuinsight/modeler/entities/monitoring_deploy_log.py
+-rw-rw-r--   0 a10894     (501) staff       (20)     1286 2023-05-30 04:42:08.000000 Accuinsight-3.4.230530/Accuinsight/modeler/entities/workspace_run_log.py
+-rw-rw-r--   0 a10894     (501) staff       (20)     3050 2023-05-30 04:42:08.000000 Accuinsight-3.4.230530/Accuinsight/modeler/exceptions.py
+-rw-rw-r--   0 a10894     (501) staff       (20)      205 2023-05-30 04:42:08.000000 Accuinsight-3.4.230530/Accuinsight/modeler/info.py
+drwxr-xr-x   0 a10894     (501) staff       (20)        0 2023-05-30 04:45:23.692879 Accuinsight-3.4.230530/Accuinsight/modeler/protos/
+-rw-rw-r--   0 a10894     (501) staff       (20)        0 2023-05-30 04:42:08.000000 Accuinsight-3.4.230530/Accuinsight/modeler/protos/__init__.py
+-rw-rw-r--   0 a10894     (501) staff       (20)    37721 2023-05-30 04:42:08.000000 Accuinsight-3.4.230530/Accuinsight/modeler/protos/life_cycle_pb2.py
+-rw-rw-r--   0 a10894     (501) staff       (20)   107276 2023-05-30 04:42:08.000000 Accuinsight-3.4.230530/Accuinsight/modeler/protos/service_pb2.py
+-rw-rw-r--   0 a10894     (501) staff       (20)    27025 2023-05-30 04:42:08.000000 Accuinsight-3.4.230530/Accuinsight/modeler/protos/skapi_pb2.py
+drwxr-xr-x   0 a10894     (501) staff       (20)        0 2023-05-30 04:45:23.693898 Accuinsight-3.4.230530/Accuinsight/modeler/store/
+-rw-rw-r--   0 a10894     (501) staff       (20)        0 2023-05-30 04:42:08.000000 Accuinsight-3.4.230530/Accuinsight/modeler/store/__init__.py
+drwxr-xr-x   0 a10894     (501) staff       (20)        0 2023-05-30 04:45:23.699099 Accuinsight-3.4.230530/Accuinsight/modeler/store/tracking/
+-rw-rw-r--   0 a10894     (501) staff       (20)      315 2023-05-30 04:42:08.000000 Accuinsight-3.4.230530/Accuinsight/modeler/store/tracking/__init__.py
+-rw-rw-r--   0 a10894     (501) staff       (20)      957 2023-05-30 04:42:08.000000 Accuinsight-3.4.230530/Accuinsight/modeler/store/tracking/lc_abstract_store.py
+-rw-rw-r--   0 a10894     (501) staff       (20)     6918 2023-05-30 04:42:08.000000 Accuinsight-3.4.230530/Accuinsight/modeler/store/tracking/life_cycle_store.py
+-rw-rw-r--   0 a10894     (501) staff       (20)     1789 2023-05-30 04:42:08.000000 Accuinsight-3.4.230530/Accuinsight/modeler/store/tracking/monitoring_deploy_store.py
+-rw-rw-r--   0 a10894     (501) staff       (20)     1416 2023-05-30 04:42:08.000000 Accuinsight-3.4.230530/Accuinsight/modeler/store/tracking/workspace_store.py
+drwxr-xr-x   0 a10894     (501) staff       (20)        0 2023-05-30 04:45:23.707536 Accuinsight-3.4.230530/Accuinsight/modeler/utils/
+-rw-rw-r--   0 a10894     (501) staff       (20)     1619 2023-05-30 04:42:08.000000 Accuinsight-3.4.230530/Accuinsight/modeler/utils/__init__.py
+-rw-rw-r--   0 a10894     (501) staff       (20)      365 2023-05-30 04:42:08.000000 Accuinsight-3.4.230530/Accuinsight/modeler/utils/annotations.py
+drwxr-xr-x   0 a10894     (501) staff       (20)        0 2023-05-30 04:45:23.710171 Accuinsight-3.4.230530/Accuinsight/modeler/utils/dependency/
+-rw-rw-r--   0 a10894     (501) staff       (20)        0 2023-05-30 04:42:08.000000 Accuinsight-3.4.230530/Accuinsight/modeler/utils/dependency/__init__.py
+-rw-rw-r--   0 a10894     (501) staff       (20)    19325 2023-05-30 04:42:08.000000 Accuinsight-3.4.230530/Accuinsight/modeler/utils/dependency/dependencies.py
+-rw-rw-r--   0 a10894     (501) staff       (20)     2209 2023-05-30 04:42:08.000000 Accuinsight-3.4.230530/Accuinsight/modeler/utils/dependency/settings.py
+-rw-rw-r--   0 a10894     (501) staff       (20)     1202 2023-05-30 04:42:08.000000 Accuinsight-3.4.230530/Accuinsight/modeler/utils/dl_utils.py
+-rwxrwxr-x   0 a10894     (501) staff       (20)     4122 2023-05-30 04:42:08.000000 Accuinsight-3.4.230530/Accuinsight/modeler/utils/os_getenv.py
+-rw-rw-r--   0 a10894     (501) staff       (20)     1175 2023-05-30 04:42:08.000000 Accuinsight-3.4.230530/Accuinsight/modeler/utils/proto_json_utils.py
+-rwxrwxr-x   0 a10894     (501) staff       (20)    11063 2023-05-30 04:42:08.000000 Accuinsight-3.4.230530/Accuinsight/modeler/utils/rest_utils.py
+-rw-rw-r--   0 a10894     (501) staff       (20)     2433 2023-05-30 04:42:08.000000 Accuinsight-3.4.230530/Accuinsight/modeler/utils/runs_utils.py
+-rw-rw-r--   0 a10894     (501) staff       (20)      367 2023-05-30 04:42:08.000000 Accuinsight-3.4.230530/Accuinsight/modeler/utils/string_utils.py
+drwxr-xr-x   0 a10894     (501) staff       (20)        0 2023-05-30 04:45:23.522189 Accuinsight-3.4.230530/Accuinsight.egg-info/
+-rw-r--r--   0 a10894     (501) staff       (20)     2266 2023-05-30 04:45:23.000000 Accuinsight-3.4.230530/Accuinsight.egg-info/PKG-INFO
+-rw-r--r--   0 a10894     (501) staff       (20)     4346 2023-05-30 04:45:23.000000 Accuinsight-3.4.230530/Accuinsight.egg-info/SOURCES.txt
+-rw-r--r--   0 a10894     (501) staff       (20)        1 2023-05-30 04:45:23.000000 Accuinsight-3.4.230530/Accuinsight.egg-info/dependency_links.txt
+-rw-r--r--   0 a10894     (501) staff       (20)        1 2023-05-30 04:45:23.000000 Accuinsight-3.4.230530/Accuinsight.egg-info/not-zip-safe
+-rw-r--r--   0 a10894     (501) staff       (20)      288 2023-05-30 04:45:23.000000 Accuinsight-3.4.230530/Accuinsight.egg-info/requires.txt
+-rw-r--r--   0 a10894     (501) staff       (20)       12 2023-05-30 04:45:23.000000 Accuinsight-3.4.230530/Accuinsight.egg-info/top_level.txt
+-rw-rw-r--   0 a10894     (501) staff       (20)       21 2023-05-30 04:42:08.000000 Accuinsight-3.4.230530/LICENSE.txt
+-rw-rw-r--   0 a10894     (501) staff       (20)       63 2023-05-30 04:42:08.000000 Accuinsight-3.4.230530/MANIFEST.in
+-rw-r--r--   0 a10894     (501) staff       (20)     2266 2023-05-30 04:45:23.711109 Accuinsight-3.4.230530/PKG-INFO
+-rw-rw-r--   0 a10894     (501) staff       (20)     1487 2023-05-30 04:42:08.000000 Accuinsight-3.4.230530/README.rst
+-rw-rw-r--   0 a10894     (501) staff       (20)      287 2023-05-30 04:42:08.000000 Accuinsight-3.4.230530/requirements.txt
+-rw-rw-r--   0 a10894     (501) staff       (20)      256 2023-05-30 04:45:23.712218 Accuinsight-3.4.230530/setup.cfg
+-rw-rw-r--   0 a10894     (501) staff       (20)     1294 2023-05-30 04:42:08.000000 Accuinsight-3.4.230530/setup.py
```

### Comparing `Accuinsight-3.4.230516rc1/Accuinsight/Lifecycle/ML.py` & `Accuinsight-3.4.230530/Accuinsight/Lifecycle/ML.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import math
 from collections import OrderedDict
 import warnings
 import logging
 from joblib import dump
 from sklearn import pipeline
 
+from Accuinsight.Lifecycle.utils import load_model
 from Accuinsight.modeler.core import func, path, get, modelEvaluation
 from Accuinsight.modeler.core.func import get_time
 from Accuinsight.modeler.core.get_for_visual import roc_pr_curve, get_true_y, get_visual_info_regressor
 from Accuinsight.modeler.core.sklearnModelType import REGRESSION, CLASSIFICATION
 from Accuinsight.modeler.core.LcConst.LcConst import ALL_MODEL_PARAMS, SELECTED_PARAMS, SELECTED_METRICS, VALUE_ERROR, \
     LOGGING_TIME, LOGGING_RUN_ID, FITTED_MODEL, USER_ID, RUN_OBJ_NAME, RUN_MODEL_JSON_PATH, RUN_MODEL_VISUAL_JSON_PATH, \
     RUN_MODEL_SHAP_JSON_PATH, RUN_MODEL_JOBLIB_PATH, RUN_ID, RUN_MODEL_EVL_JSON_PATH
@@ -103,24 +104,28 @@
 
     def get_current_run_id(self):
         try:
             return self.get_current_run_meta()[RUN_OBJ_NAME]
         except TypeError or KeyError:
             return None
 
-    def model_evaluation(self, run_nickname_input=None, loaded_model=None, loaded_model_json=None, x_validation=None, y_validation=None, f1_average_in='weighted', recall_average_in='weighted'):
+    def model_evaluation(self, run_name = None, run_nickname_input=None, x_validation=None, y_validation=None, f1_average_in='weighted', recall_average_in='weighted'):
         start_evl = get_time.now()
+        if run_name is None:
+            raise Exception('run_name is None')
+        # 모델 run_id로 load
+        loaded_model, loaded_model_json = load_model(run_name)
 
         # get_file_path 실행 시 experiment 생성 시 필요한 폴더들이 다 만들어짐.
         # modeler backend 호출 시 파라미터로 경로 내 json 파일 내용을 protobuf 통해서 변환 후 gRPC로 전송을 위해 사용.
         self.dict_path = path.get_file_path(loaded_model)
 
         # dependencies를 가져오기 위한 작업
         if is_in_ipython():
-            var_model_file_path = self.notebook_info
+            # var_model_file_path = self.notebook_info
             _caller_globals = inspect.stack()[1][0].f_globals
             (
                 mainfile,
                 sources,
                 dependencies
             ) = gather_sources_and_dependencies(
                 globs=_caller_globals,
@@ -132,80 +137,87 @@
                 mainfile,
                 sources,
                 dependencies
             ) = gather_sources_and_dependencies(
                 globs=_caller_globals,
                 save_git_info=True
             )
-            var_model_file_path = mainfile['filename']
+            # var_model_file_path = mainfile['filename']
 
+        # run_nickname 설정: 미설정 시 default_run_nick_name(파일 이름) 으로 설정
         if run_nickname_input is None:
             run_nick_name = self.default_run_nick_name
         else:
             run_nick_name = run_nickname_input
 
-
+        # 모델과 검증용 데이터 유무 판별
+        # loaded_model_json: 모델의 json 파일 내용 -> /runs/best-model/ 아래 존재
         if loaded_model is None or x_validation is None or y_validation is None or loaded_model_json is None:
             raise ValueError("Please set parameter -> model or validation data. ")
         x_val = x_validation
         y_val = y_validation
 
         # set current run
         set_current_runs(get.model_type(loaded_model))
 
         # path for for-evl-json
         # visualCallback 참고 해서 actual data로 성능평가
         path_for_setting_evl_json = self.dict_path['evl_json']
         evl_json_full_path = self.dict_path[RUN_MODEL_EVL_JSON_PATH]
         set_evl_json_path(path_for_setting_evl_json)
 
+        # json to dict
         loaded_model_json_dict = json.loads(loaded_model_json)
         run_id = loaded_model_json_dict['run_id']
 
         '''
         RunInfo.py 내 아래 데이터에 set
         global _runData
         run_obj = _runData[0]
         '''
-        # set_optimizer_info_path(loaded_model_json_dict['optimizer_info'])
+        # 아래 set_ ~~ 함수들은 modeler-api를 통해 DB에 데이터 유지 + UI 표기를 위한 과정
         set_model_file_path(loaded_model_json_dict['path'])
         set_python_dependencies(py_depenpency=loaded_model_json_dict['model_dependencies'])
         set_prefix_path(self.dict_path[LcConst.RUN_PREFIX_PATH])
         set_run_name(loaded_model_json_dict[FITTED_MODEL], run_id, run_nick_name)
 
         set_best_model_json_path(loaded_model_json_dict['best_model_json'])
         set_best_model_joblib_path(loaded_model_json_dict['best_model_joblib'])
         set_all_model_params(loaded_model_json_dict[ALL_MODEL_PARAMS])
         set_selected_params(loaded_model_json_dict[SELECTED_PARAMS])
 
 
         # classifier
         if any(i in loaded_model_json_dict[FITTED_MODEL] for i in CLASSIFICATION) or loaded_model_json_dict[ALL_MODEL_PARAMS]['metric'] in metricsLightgbm.CLASSIFICATION:
             print("ML_CLASSIFICATION in model_evaluation method")
+            # roc pr curve
             visual_classification_json = roc_pr_curve(loaded_model, x_val, y_val, f1_average=f1_average_in,
                                                           recall_average=recall_average_in)
             with open(evl_json_full_path, 'w', encoding='utf-8') as save_file:
                 json.dump(visual_classification_json, save_file, indent="\t")
 
+            # confusion matrix, f1, recall, precision
             selected_metrics = modelEvaluation.calculate_classification_metrics(loaded_model, x_val, y_val, average=f1_average_in)
             set_model_type("ML_CLASSIFICATION")
 
         # regressor
         elif any(i in loaded_model_json_dict[FITTED_MODEL] for i in REGRESSION)  or loaded_model_json_dict[ALL_MODEL_PARAMS]['metric'] in metricsLightgbm.REGRESSION:
             print("ML_REGRESSION in model_evaluation method")
             visual_regression_json = OrderedDict()
             visual_regression_json['True_y'] = get_true_y(y_val)
+            # predict_y
             visual_regression_json['Predicted_y'] = get_visual_info_regressor(loaded_model, x_val)
 
             set_true_y(visual_regression_json['True_y'])
             set_predict_y(visual_regression_json['Predicted_y'])
 
             with open(evl_json_full_path, 'w', encoding='utf-8') as save_file:
                 json.dump(visual_regression_json, save_file, indent="\t")
 
+            # mae, mse, rmse, r2, mape
             selected_metrics = modelEvaluation.calculate_regression_metrics(loaded_model, x_val, y_val)
             set_model_type("ML_REGRESSION")
 
         else:
             raise ValueError('현재 설정한 모델은 지원되지 않습니다. 관리자에게 문의하십시오.')
 
         loaded_model_json_dict[SELECTED_METRICS] = selected_metrics
@@ -213,20 +225,22 @@
 
         end_evl = get_time.now()
 
         start_ts = int(start_evl.timestamp())
         end_ts = int(end_evl.timestamp())
         delta_ts = end_ts - start_ts
 
+        # 현재까지 set 했던 run 정보를 run_meta dict에 담아서 modeler-api로 전송
         run_meta = clear_runs(start_ts, end_ts, delta_ts, isEvaluation="true")
         print(run_meta)
         env_value = get_os_env('ENV')
         modeler_rest = LifecycleRestApi(env_value[LcConst.BACK_END_API_URL],
                                         env_value[LcConst.BACK_END_API_PORT],
                                         env_value[LcConst.BACK_END_API_URI])
+        # modeler-api로 전송
         modeler_rest.lc_create_run(run_meta)
 
     class add_experiment(object):
         def __init__(self, model_name, *args, model_monitor=False, runtime=False, f1_average_in='weighted', recall_average_in='weighted'):
             self.shap_on = model_monitor
             self.runtime = runtime
             logging.info('Using add_experiment(model_monitor={})'.format(model_monitor))
@@ -473,15 +487,16 @@
             global run_meta
             run_meta = clear_runs(start_time, end_time, delta_ts)
 
             accuinsight._send_message(metric=None,
                                       current_value=None,
                                       message=message_param,
                                       thresholds=None,
-                                      alarm_object=alarm,
+                                      alarm_object=None,
+                                      # direct_email=,
                                       alarm_api=alarm_api)
 
             env_value = get_os_env('ENV')
             modeler_rest = LifecycleRestApi(env_value[LcConst.BACK_END_API_URL],
                                             env_value[LcConst.BACK_END_API_PORT],
                                             env_value[LcConst.BACK_END_API_URI])
             modeler_rest.lc_create_run(run_meta)
```

### Comparing `Accuinsight-3.4.230516rc1/Accuinsight/Lifecycle/common.py` & `Accuinsight-3.4.230530/Accuinsight/Lifecycle/common.py`

 * *Files 7% similar despite different names*

```diff
@@ -307,17 +307,30 @@
         if hook_url:
             self.workspace_alarm.notifiers['slack'] = hook_url
 
     def unset_slack(self):
         if 'slack' in self.workspace_alarm.notifiers.keys():
             del self.workspace_alarm.notifiers['slack']
 
-    def set_mail(self, address=None):
-        if address:
-            self.workspace_alarm.notifiers['mail'] = address
+    # 기존 modeler-api를 통한 기능 주석처리
+    # def set_mail(self, address=None):
+    #     if address:
+    #         self.workspace_alarm.notifiers['mail'] = address
+    #
+    # def unset_mail(self):
+    #     if 'mail' in self.workspace_alarm.notifiers.keys():
+    #         del self.workspace_alarm.notifiers['mail']
+
+    ''' setting example
+    accu.set_email(to='aaa@sk.com, bbb@sk.com', cc='aaa@sk.com, bbb@sk.com', bcc='aaa@sk.com, bbb@sk.com',
+                   subject='test mail from accu sdk', contents='something')
+    '''
+    def set_mail(self, json_body=None):
+        if json_body:
+            self.workspace_alarm.notifiers['mail'] = json_body
 
     def unset_mail(self):
         if 'mail' in self.workspace_alarm.notifiers.keys():
             del self.workspace_alarm.notifiers['mail']
 
     def send_message(self, message=None, thresholds=None):
         if message and thresholds:
```

### Comparing `Accuinsight-3.4.230516rc1/Accuinsight/Lifecycle/keras.py` & `Accuinsight-3.4.230530/Accuinsight/Lifecycle/tensorflow.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,38 @@
 import inspect
 import json
+import logging
 import warnings
 from collections import OrderedDict
+
 import gorilla
-import logging
 import numpy as np
-import keras
-from keras.callbacks import CSVLogger
-from Accuinsight.modeler.core import func, path, get, modelEvaluation, lossFuncInfo
+import tensorflow
+from tensorflow.keras.callbacks import CSVLogger
+
+from Accuinsight.Lifecycle.utils import load_model
+from Accuinsight.modeler.core import func, path, get
 from Accuinsight.modeler.core.func import get_time
 from Accuinsight.modeler.core.LcConst import LcConst
-from Accuinsight.modeler.core.LcConst.LcConst import RUN_NAME_KERAS, RUN_OBJ_NAME, RUN_MODEL_JSON_PATH, \
-    RUN_MODEL_SHAP_JSON_PATH, RUN_MODEL_VISUAL_JSON_PATH, SELECTED_METRICS, USER_ID, RUN_MODEL_EVL_JSON_PATH
-from Accuinsight.modeler.core.get_for_visual import roc_pr_curve, get_visual_info_regressor, get_true_y
+from Accuinsight.modeler.core.LcConst.LcConst import RUN_NAME_TENSORFLOW, RUN_OBJ_NAME, RUN_MODEL_JSON_PATH, \
+    RUN_MODEL_VISUAL_JSON_PATH,RUN_MODEL_EVL_JSON_PATH, RUN_MODEL_VISUAL_CSV_PATH, SELECTED_METRICS, USER_ID
 from Accuinsight.modeler.core.Run.RunInfo.RunInfo import set_current_runs, clear_runs, set_model_json_path, \
-    set_visual_csv_path, set_visual_json_path, set_best_model_h5_path, set_best_model_json_path, \
-    set_python_dependencies, set_run_name, set_model_file_path, set_prefix_path, set_shap_json_path, set_model_type, \
-    set_optimizer_info_path, set_evl_json_path, set_selected_metrics_path
-from Accuinsight.modeler.core.feature_contribution import shap_value
-from Accuinsight.modeler.utils.dl_utils import delete_files_except_best, get_best_model_path
+    set_visual_csv_path, set_visual_json_path, set_best_model_json_path, set_best_model_h5_path, \
+    set_python_dependencies, set_run_name, set_model_file_path, set_prefix_path, set_shap_json_path, set_evl_json_path, \
+    set_optimizer_info_path, set_selected_metrics_path, set_model_type, set_true_y, set_predict_y
+from Accuinsight.modeler.core.get_for_visual import roc_pr_curve, get_true_y, get_visual_info_regressor
+from Accuinsight.modeler.clients.modeler_api import LifecycleRestApi
 from Accuinsight.modeler.utils.dependency.dependencies import gather_sources_and_dependencies
+from Accuinsight.modeler.utils.dl_utils import delete_files_except_best, get_best_model_path
 from Accuinsight.modeler.utils.os_getenv import is_in_ipython, get_os_env
-from Accuinsight.modeler.clients.modeler_api import LifecycleRestApi
+from Accuinsight.modeler.core.feature_contribution import shap_value
 from Accuinsight.Lifecycle.common import Common
+from Accuinsight.modeler.core import lossFuncInfo
+from Accuinsight.modeler.core import modelEvaluation
+
 
 logging.basicConfig(level=logging.INFO,
                     format='%(message)s')
 
 warnings.filterwarnings("ignore")
 
 
@@ -47,24 +53,28 @@
 
     def get_current_run_id(self):
         try:
             return self.get_current_run_meta()[RUN_OBJ_NAME]
         except TypeError or KeyError:
             return None
 
-    def model_evaluation(self, run_nickname_input=None, loaded_model=None, loaded_model_json=None, x_validation=None, y_validation=None):
+    def model_evaluation(self, run_name = None, run_nickname_input=None, loaded_model=None, loaded_model_json=None, x_validation=None, y_validation=None, f1_average_in='weighted', recall_average_in='weighted'):
         start_evl = get_time.now()
+        if run_name is None:
+            raise Exception('run_name is None')
+        # 모델 run_id로 load
+        loaded_model, loaded_model_json = load_model(run_name)
 
         # get_file_path 실행 시 experiment 생성 시 필요한 폴더들이 다 만들어짐.
         # modeler backend 호출 시 파라미터로 경로 내 json 파일 내용을 protobuf 통해서 변환 후 gRPC로 전송을 위해 사용.
         self.dict_path = path.get_file_path(loaded_model, usedFramework='tensorflow')
 
         # dependencies를 가져오기 위한 작업
         if is_in_ipython():
-            var_model_file_path = self.notebook_info
+            # var_model_file_path = self.notebook_info
             _caller_globals = inspect.stack()[1][0].f_globals
             (
                 mainfile,
                 sources,
                 dependencies
             ) = gather_sources_and_dependencies(
                 globs=_caller_globals,
@@ -76,105 +86,113 @@
                 mainfile,
                 sources,
                 dependencies
             ) = gather_sources_and_dependencies(
                 globs=_caller_globals,
                 save_git_info=True
             )
-            var_model_file_path = mainfile['filename']
+            # var_model_file_path = mainfile['filename']
 
+        # run_nickname 설정: 미설정 시 default_run_nick_name(파일 이름) 으로 설정
         if run_nickname_input is None:
             run_nick_name = self.default_run_nick_name
         else:
             run_nick_name = run_nickname_input
 
-
+        # 모델과 검증용 데이터 유무 판별
+        # loaded_model_json: 모델의 json 파일 내용 -> /runs/best-model/ 아래 존재
         if loaded_model is None or x_validation is None or y_validation is None or loaded_model_json is None:
             raise ValueError("Please set parameter -> model or validation data. ")
         x_val = x_validation
         y_val = y_validation
 
         # set current run
-        set_current_runs(RUN_NAME_KERAS)
+        set_current_runs(RUN_NAME_TENSORFLOW)
 
         # path for for-evl-json
         # visualCallback 참고 해서 actual data로 성능평가
         path_for_setting_evl_json = self.dict_path['evl_json']
         evl_json_full_path = self.dict_path[RUN_MODEL_EVL_JSON_PATH]
         set_evl_json_path(path_for_setting_evl_json)
 
+        # json to dict
         loaded_model_json_dict = json.loads(loaded_model_json)
         loss_function = loaded_model_json_dict['loss_function']
         run_id = loaded_model_json_dict['run_id']
 
         '''
         RunInfo.py 내 아래 데이터에 set
         global _runData
         run_obj = _runData[0]
         '''
+        # 아래 set_ ~~ 함수들은 modeler-api를 통해 DB에 데이터 유지 + UI 표기를 위한 과정
         set_optimizer_info_path(loaded_model_json_dict['optimizer_info'])
         set_model_file_path(loaded_model_json_dict['path'])
         set_python_dependencies(py_depenpency=loaded_model_json_dict['model_dependencies'])
         set_prefix_path(self.dict_path[LcConst.RUN_PREFIX_PATH])
         set_run_name('tf.keras', run_id, run_nick_name)
 
         set_best_model_json_path(loaded_model_json_dict['best_model_json'])
         set_best_model_h5_path(loaded_model_json_dict['best_model_h5'])
 
 
         # 모델 라이브러리 확인 (tf or keras)
-        if isinstance(loaded_model, keras.Model): #Sequential은 Model에서 상속 받아 같음.
-
-            # print(loss_function)
-            # print(self.dict_path[RUN_MODEL_EVL_JSON_PATH])
-
+        if isinstance(loaded_model, tensorflow.keras.Model): #Sequential은 Model에서 상속 받아 같음.
             # classification
             if loss_function in lossFuncInfo.CLASSIFICATION:
                 print("DL_CLASSIFICATION in model_evaluation method")
-                # visual_classification_json = roc_pr_curve(loaded_model, x_val, y_val, f1_average=f1_average_in,
-                #                                           recall_average=recall_average_in)
-                visual_classification_json = roc_pr_curve(loaded_model, x_val, y_val, f1_average="weighted",
-                                                          recall_average="weighted")
+                # roc pr curve
+                visual_classification_json = roc_pr_curve(loaded_model, x_val, y_val, f1_average=f1_average_in,
+                                                          recall_average=recall_average_in)
                 with open(evl_json_full_path, 'w', encoding='utf-8') as save_file:
                     json.dump(visual_classification_json, save_file, indent="\t")
 
-                selected_metrics = modelEvaluation.calculate_classification_metrics(loaded_model, x_val, y_val, average='weighted')
+                # confusion matrix, f1, recall, precision
+                selected_metrics = modelEvaluation.calculate_classification_metrics(loaded_model, x_val, y_val, average=f1_average_in)
                 set_model_type("DL_CLASSIFICATION")
+
             # regression
             elif loss_function in lossFuncInfo.REGRESSION:
                 print("DL_REGRESSION in model_evaluation method")
                 visual_regression_json = OrderedDict()
                 visual_regression_json['True_y'] = get_true_y(y_val)
+                # predict_y
                 visual_regression_json['Predicted_y'] = get_visual_info_regressor(loaded_model, x_val)
 
+                set_true_y(visual_regression_json['True_y'])
+                set_predict_y(visual_regression_json['Predicted_y'])
+
                 with open(evl_json_full_path, 'w', encoding='utf-8') as save_file:
                     json.dump(visual_regression_json, save_file, indent="\t")
 
+                # mae, mse, rmse, r2, mape
                 selected_metrics = modelEvaluation.calculate_regression_metrics(loaded_model, x_val, y_val)
                 set_model_type("DL_REGRESSION")
 
             else:
-                raise ValueError('현재 설정한 loss는 지원되지 않습니다. 관리자에게 문의하십시오.')
+                raise ValueError('현재 설정한 모델은 지원되지 않습니다. 관리자에게 문의하십시오.')
         else: # keras 만을 사용한 경우 없음. 추후 pytorch 대응용
             pass
         loaded_model_json_dict[SELECTED_METRICS] = selected_metrics
         set_selected_metrics_path(loaded_model_json_dict[SELECTED_METRICS])
 
         end_evl = get_time.now()
 
         start_ts = int(start_evl.timestamp())
         end_ts = int(end_evl.timestamp())
         delta_ts = end_ts - start_ts
 
+        # 현재까지 set 했던 run 정보를 run_meta dict에 담아서 modeler-api로 전송
         run_meta = clear_runs(start_ts, end_ts, delta_ts, isEvaluation="true")
-
+        print(run_meta)
         env_value = get_os_env('ENV')
         modeler_rest = LifecycleRestApi(env_value[LcConst.BACK_END_API_URL],
                                         env_value[LcConst.BACK_END_API_PORT],
                                         env_value[LcConst.BACK_END_API_URI])
+        # modeler-api로 전송
         modeler_rest.lc_create_run(run_meta)
 
     def autolog(self, run_nickname_input=None, tag=None, best_weights=False, model_monitor=False, runtime=False, f1_average_in='weighted', recall_average_in='weighted'):
         global description, endpoint, var_model_file_path, message, thresholds, best_weights_on, run_id, alarm, alarm_api, shap_on, feature_name, run_meta, run_nick_name
         description = tag
         endpoint = self.endpoint
         message = self.message # common.py send_message 호출을 통해 생성
@@ -237,25 +255,22 @@
                 dependencies
             ) = gather_sources_and_dependencies(
                 globs=_caller_globals,
                 save_git_info=True
             )
             var_model_file_path = mainfile['filename']
 
-        class TrainHistoryCallbacks(keras.callbacks.Callback):
-            def __init__(self, verbose=1, mode='auto', period=1):
+        class TrainHistoryCallbacks(tensorflow.keras.callbacks.Callback):
+            def __init__(self, verbose=1, mode='auto'):
                 super(TrainHistoryCallbacks, self).__init__()
                 self.verbose = verbose
-                self.period = period
                 self.best_epochs = 0
                 self.epochs_since_last_save = 0
                 self.mode = mode
                 self.model_summary = OrderedDict()
-                self.run_id = None
-                self.model_type = None
 
             def on_train_begin(self, logs={}):
                 logging.info('Using autolog(best_weights={}, model_monitor={}'
                              .format(str(best_weights_on), str(shap_on)))
 
                 global start
                 start = get_time.now()
@@ -279,15 +294,15 @@
                     self.model_summary['loss_function'] = self.model.loss
 
                 self.model_summary['optimizer_info'] = {opt['name']: opt_result}
 
                 '''[get best model] on_train_begin '''
                 self.best_weights = self.model.get_weights()
 
-                self.dict_path = path.get_file_path(self.model, usedFramework='keras')
+                self.dict_path = path.get_file_path(self.model, usedFramework='tensorflow')
 
                 set_prefix_path(self.dict_path[LcConst.RUN_PREFIX_PATH])
 
                 set_run_name(self.model_summary['model_type'], self.model_summary['run_id'], self.model_summary['run_nick_name'])
                 set_python_dependencies(py_depenpency=dependencies)
 
             '''[get best model] on_epoch_end '''
@@ -340,24 +355,24 @@
 
                     self.current_value = current
 
                 # Not using best_weights
                 else:
                     self.last_epoch_metric = logs.get(self.monitor)
                     self.best_epochs = epoch + 1
-                    self.current_value = logs.get(self.monitor)
+                    current = logs.get(self.monitor)
+                    self.current_value = current
 
                 # model save path
                 run_id = self.model_summary['model_type'] + '-' + self.model_summary['run_id']
-                common_path = self.dict_path['save_model_path'] + run_id + '-epoch-' + str(epoch + 1).zfill(5) \
-                              + '-' + self.monitor + '-' + str(current).zfill(5)
+                common_path = self.dict_path['save_model_path'] + run_id + '-epoch-' + str(epoch + 1).zfill(5) + '-' + self.monitor + '-' + str(current).zfill(5)
                 save_model_path = common_path + '.json'
                 save_weights_path = common_path + '.h5'
 
-                # model evaluation path(in jupyter lab browser path)
+                # model evaluation path(in jupyter lab browser path - 상대경로 의미...)
                 browser_common_path = self.dict_path['save_model_dir'] + '/' + run_id + '-epoch-' + str(epoch + 1).zfill(
                     5) + '-' + self.monitor + '-' + str(current).zfill(5)
                 save_model_path_browser = browser_common_path + '.json'
                 save_weights_path_browser = browser_common_path + '.h5'
 
                 # model to JSON
                 model_json = self.model.to_json()
@@ -383,35 +398,38 @@
 
                 # weights to H5
                 # self.model.save_weights(save_weights_path)
                 self.model.save(save_weights_path)
 
             def on_train_end(self, logs={}):
                 '''[get best model] on_train_end '''
-                if self.verbose > 0:
-                    print('Using epoch %05d with %s: %0.5f' % (self.best_epochs, self.monitor, self.best))
-                self.model.set_weights(self.best_weights)  # set best model's weights
-                
+                if best_weights_on:
+                    if self.verbose > 0:
+                        print('\nUsing epoch %05d with %s: %0.5f' % (self.best_epochs, self.monitor, self.best))
+                    self.model.set_weights(self.best_weights)  # set best model's weights
+                    
+                    self.model_summary[SELECTED_METRICS] = {self.monitor: np.float64(self.best)}
+                else:
+                    self.model_summary[SELECTED_METRICS] = {self.monitor: np.float64(self.last_epoch_metric)}
+    
+          #      print('model_summary: ', self.model_summary)   ##############################
                 end = get_time.now()
                 self.model_summary['time_delta'] = str(end - start)
-                self.model_summary[SELECTED_METRICS] = {self.monitor: self.best}
-            
+
                 # path for model_info.json
-                set_model_json_path(self.dict_path['model_json'])
+                self.path_for_setting_model_json = self.dict_path['model_json']
+                set_model_json_path(self.path_for_setting_model_json)
+
                 model_json_full_path = self.dict_path[RUN_MODEL_JSON_PATH]
 
                 with open(model_json_full_path, 'w', encoding='utf-8') as save_file:
                     json.dump(self.model_summary, save_file, indent="\t")
-            
-                if best_weights_on:
-                    delete_files_except_best(run_id=self.model_summary['run_id'], epochs=str(self.best_epochs),
-                                            path=self.dict_path)
-                else:
-                    delete_files_except_best(run_id=self.model_summary['run_id'], epochs=str(self.last_epochs),
-                    path=self.dict_path)
+
+                delete_files_except_best(run_id=self.model_summary['run_id'], epochs=str(self.best_epochs),
+                                         path=self.dict_path)
 
                 path_for_setting_model_json = self.dict_path['save_model_dir'] + \
                                               get_best_model_path(run_id=self.model_summary['run_id'],
                                                                   path=self.dict_path)['json']
                 path_for_setting_model_h5 = self.dict_path['save_model_dir'] + \
                                             get_best_model_path(run_id=self.model_summary['run_id'],
                                                                 path=self.dict_path)['h5']
@@ -423,35 +441,34 @@
                 delta_ts = end_ts - start_ts
 
                 global run_meta
                 run_meta = clear_runs(start_ts, end_ts, delta_ts)
                 accuinsight._send_message(metric=self.monitor,
                                           current_value=self.current_value,
                                           message=message,
-                                          thresholds=thresholds,
-                                          alarm_object=alarm,
+                                          alarm_object=None,
+                                          # direct_email=,
                                           alarm_api=alarm_api)
                 env_value = get_os_env('ENV')
                 modeler_rest = LifecycleRestApi(env_value[LcConst.BACK_END_API_URL],
                                                 env_value[LcConst.BACK_END_API_PORT],
                                                 env_value[LcConst.BACK_END_API_URI])
                 modeler_rest.lc_create_run(run_meta)
                 if runtime:
-                    accuinsight.set_runtime_model('keras')
-                accuinsight.off_autolog()
+                    accuinsight.set_runtime_model('tensorflow')
+                accuinsight._off_autolog()
 
-        class visualCallbacks(keras.callbacks.Callback):
+        class visualCallbacks(tensorflow.keras.callbacks.Callback):
             def __init__(self, x_validation=None, y_validation=None):
                 super(visualCallbacks, self).__init__()
                 self.x_val = x_validation
                 self.y_val = y_validation
 
             def on_train_end(self, logs={}):
-                self.dict_path = path.get_file_path(self.model, usedFramework='keras')
-
+                self.dict_path = path.get_file_path(self.model, usedFramework='tensorflow')
                 # path for visual.json
                 path_for_setting_visual_json = self.dict_path['visual_json']
                 visual_json_full_path = self.dict_path[RUN_MODEL_VISUAL_JSON_PATH]
                 set_visual_json_path(path_for_setting_visual_json)
 
                 # classification
                 if get.is_classification(self.model):
@@ -459,94 +476,85 @@
 
                     with open(visual_json_full_path, 'w', encoding='utf-8') as save_file:
                         json.dump(visual_classification_json, save_file, indent="\t")
 
                 # regression
                 else:
                     visual_regression_json = OrderedDict()
-                    visual_regression_json['True_y'] = self.y_val.tolist()
+                    visual_regression_json['True_y'] = get_true_y(self.y_val)
                     visual_regression_json['Predicted_y'] = get_visual_info_regressor(self.model, self.x_val)
 
                     with open(visual_json_full_path, 'w', encoding='utf-8') as save_file:
                         json.dump(visual_regression_json, save_file, indent="\t")
 
-        class shapCallbacks(keras.callbacks.Callback):
+        class shapCallbacks(tensorflow.keras.callbacks.Callback):
             def __init__(self, trainX, feature_name, run_id, trigger=shap_on):
                 super(shapCallbacks, self).__init__()
                 self.trainX = trainX
                 self.trigger = trigger
                 self.run_id = run_id
                 self.feature_name_in_shap = feature_name
 
             def on_train_end(self, logs={}):
                 if self.trigger:
                     self.shap_value = shap_value(self.model, self.trainX, self.feature_name_in_shap)
-
-                    self.dict_path = path.get_file_path(self.model, usedFramework='keras')
+                    
+#                     func.insertDB(self.shap_value, 2)  # 수정: 2 -> self.run_id
+                    
+                    self.dict_path = path.get_file_path(self.model, usedFramework='tensorflow')
 
                     # path for shap.json
-                    shap_json_full_path = self.dict_path[RUN_MODEL_SHAP_JSON_PATH]
+                    shap_json_full_path = self.dict_path['shap_json_full']
                     set_shap_json_path(self.dict_path['shap_json'])
 
                     with open(shap_json_full_path, 'w', encoding='utf-8') as save_file:
                         json.dump(self.shap_value, save_file, indent='\t')
 
                 else:
                     pass
 
-        def run_and_log_function(self, original, x, y, kwargs, unlogged_params):
-            dict_path = path.get_file_path(self, usedFramework='keras')
-
+        def run_and_log_function(self, original, x, y, kwargs):
+            dict_path = path.get_file_path(self, usedFramework='tensorflow')
             path_for_setting_visual_csv = dict_path['visual_csv']
-            visual_csv_full_path = dict_path['visual_csv_full']
+            visual_csv_full_path = dict_path[RUN_MODEL_VISUAL_CSV_PATH]
 
             # set current run
-            set_current_runs(RUN_NAME_KERAS)
+            set_current_runs(RUN_NAME_TENSORFLOW)
             set_model_file_path(var_model_file_path)
             set_visual_csv_path(path_for_setting_visual_csv)
 
             csv_logger = CSVLogger(visual_csv_full_path, append=True, separator=';')
 
             # get train data(x) for computing shap value
             if 'x':
                 x_train = x
             if shap_on:
                 get_shap = shapCallbacks(x_train, feature_name, run_id, trigger=shap_on)
             else:
                 pass
- 
+
             ''' save json for visualization '''
-            kwargs_dict = OrderedDict()
-            
-            for key, value in kwargs.items():
-                kwargs_dict[key] = value
-            
             # using validation_data argument
-            if 'validation_data' in kwargs_dict.keys():
+            if 'validation_data' in kwargs:
                 validation_set = kwargs['validation_data']
 
                 try:
                     x_val = validation_set[0]
                     y_val = validation_set[1]
 
                 except:
                     iterator = iter(validation_set)
                     valid_set = next(iterator)
                     x_val = valid_set[0].numpy()
                     y_val = valid_set[1].numpy()
-            
-#            elif 'validation_split' in kwargs_dict.keys():
-#                (x, y), validation_set = (data_adapter.train_validation_split((x,y), validation_split=kwargs_dict['validation_split']))
-#                if validation_set:
-#                    x_val, y_val, val_sample_weight = (data_adapter.unpack_x_y_sample_weight(validation_set))
-#
+
+                get_visual = visualCallbacks(x_validation=x_val, y_validation=y_val)
+
             else:
-                raise ValueError('"validation_data" or "validation_split" does not exist.')
-            
-            get_visual = visualCallbacks(x_validation=x_val, y_validation=y_val)
+                raise ValueError('"validation_data" does not exist.')
 
             if 'callbacks' in kwargs:
                 kwargs['callbacks'] += [csv_logger]
             else:
                 kwargs['callbacks'] = [csv_logger]
 
             kwargs['callbacks'] += [get_visual]
@@ -554,28 +562,28 @@
                 kwargs['callbacks'] += [get_shap]
             else:
                 pass
             kwargs['callbacks'] += [TrainHistoryCallbacks()]
 
             return original(self, x, y, **kwargs)
 
-        @gorilla.patch(keras.Model)
+        @gorilla.patch(tensorflow.keras.Model)
         def fit(self, x, y, **kwargs):
-            original = gorilla.get_original_attribute(keras.Model, 'fit')
-            unlogged_params = ['self', 'x', 'y', 'callbacks', 'validation_data', 'verbose']
-            return run_and_log_function(self, original, x, y, kwargs, unlogged_params)
+            original = gorilla.get_original_attribute(tensorflow.keras.Model, 'fit')
+            unlogged_params = ['self', 'callbacks', 'validation_data', 'verbose']
+            return run_and_log_function(self, original, x, y, kwargs)
 
         settings = gorilla.Settings(allow_hit=True, store_hit=True)
-        gorilla.apply(gorilla.Patch(keras.Model, 'fit', fit, settings=settings))
+        gorilla.apply(gorilla.Patch(tensorflow.keras.Model, 'fit', fit, settings=settings))
 
-    def off_autolog():
+    def _off_autolog():
         def stop_log(self, original, args, kwargs, unlogged_params):
             return original(self, *args, **kwargs)
 
-        @gorilla.patch(keras.Model)
+        @gorilla.patch(tensorflow.keras.Model)
         def fit(self, *args, **kwargs):
-            original = gorilla.get_original_attribute(keras.Model, 'fit')
+            original = gorilla.get_original_attribute(tensorflow.keras.Model, 'fit')
             unlogged_params = ['self', 'x', 'y', 'callbacks', 'validation_data', 'verbose']
             return stop_log(self, original, args, kwargs, unlogged_params)
 
         settings = gorilla.Settings(allow_hit=True, store_hit=True)
-        gorilla.apply(gorilla.Patch(keras.Model, 'fit', fit, settings=settings))
+        gorilla.apply(gorilla.Patch(tensorflow.keras.Model, 'fit', fit, settings=settings))
```

### Comparing `Accuinsight-3.4.230516rc1/Accuinsight/Lifecycle/settings.py` & `Accuinsight-3.4.230530/Accuinsight/Lifecycle/settings.py`

 * *Files identical despite different names*

### Comparing `Accuinsight-3.4.230516rc1/Accuinsight/Lifecycle/tensorflow.py` & `Accuinsight-3.4.230530/Accuinsight/Lifecycle/keras.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,34 @@
 import inspect
 import json
-import logging
 import warnings
 from collections import OrderedDict
-
 import gorilla
+import logging
 import numpy as np
-import tensorflow
-from tensorflow.keras.callbacks import CSVLogger
-from Accuinsight.modeler.core import func, path, get
+import keras
+from keras.callbacks import CSVLogger
+
+from Accuinsight.Lifecycle.utils import load_model
+from Accuinsight.modeler.core import func, path, get, modelEvaluation, lossFuncInfo
 from Accuinsight.modeler.core.func import get_time
 from Accuinsight.modeler.core.LcConst import LcConst
-from Accuinsight.modeler.core.LcConst.LcConst import RUN_NAME_TENSORFLOW, RUN_OBJ_NAME, RUN_MODEL_JSON_PATH, \
-    RUN_MODEL_VISUAL_JSON_PATH,RUN_MODEL_EVL_JSON_PATH, RUN_MODEL_VISUAL_CSV_PATH, SELECTED_METRICS, USER_ID
+from Accuinsight.modeler.core.LcConst.LcConst import RUN_NAME_KERAS, RUN_OBJ_NAME, RUN_MODEL_JSON_PATH, \
+    RUN_MODEL_SHAP_JSON_PATH, RUN_MODEL_VISUAL_JSON_PATH, SELECTED_METRICS, USER_ID, RUN_MODEL_EVL_JSON_PATH
+from Accuinsight.modeler.core.get_for_visual import roc_pr_curve, get_visual_info_regressor, get_true_y
 from Accuinsight.modeler.core.Run.RunInfo.RunInfo import set_current_runs, clear_runs, set_model_json_path, \
-    set_visual_csv_path, set_visual_json_path, set_best_model_json_path, set_best_model_h5_path, \
-    set_python_dependencies, set_run_name, set_model_file_path, set_prefix_path, set_shap_json_path, set_evl_json_path, \
-    set_optimizer_info_path, set_selected_metrics_path, set_model_type, set_true_y, set_predict_y
-from Accuinsight.modeler.core.get_for_visual import roc_pr_curve, get_true_y, get_visual_info_regressor
-from Accuinsight.modeler.clients.modeler_api import LifecycleRestApi
-from Accuinsight.modeler.utils.dependency.dependencies import gather_sources_and_dependencies
+    set_visual_csv_path, set_visual_json_path, set_best_model_h5_path, set_best_model_json_path, \
+    set_python_dependencies, set_run_name, set_model_file_path, set_prefix_path, set_shap_json_path, set_model_type, \
+    set_optimizer_info_path, set_evl_json_path, set_selected_metrics_path
+from Accuinsight.modeler.core.feature_contribution import shap_value
 from Accuinsight.modeler.utils.dl_utils import delete_files_except_best, get_best_model_path
+from Accuinsight.modeler.utils.dependency.dependencies import gather_sources_and_dependencies
 from Accuinsight.modeler.utils.os_getenv import is_in_ipython, get_os_env
-from Accuinsight.modeler.core.feature_contribution import shap_value
+from Accuinsight.modeler.clients.modeler_api import LifecycleRestApi
 from Accuinsight.Lifecycle.common import Common
-from Accuinsight.modeler.core import lossFuncInfo
-from Accuinsight.modeler.core import modelEvaluation
-
 
 logging.basicConfig(level=logging.INFO,
                     format='%(message)s')
 
 warnings.filterwarnings("ignore")
 
 
@@ -51,24 +49,28 @@
 
     def get_current_run_id(self):
         try:
             return self.get_current_run_meta()[RUN_OBJ_NAME]
         except TypeError or KeyError:
             return None
 
-    def model_evaluation(self, run_nickname_input=None, loaded_model=None, loaded_model_json=None, x_validation=None, y_validation=None, f1_average_in='weighted', recall_average_in='weighted'):
+    def model_evaluation(self, run_name = None, run_nickname_input=None, x_validation=None, y_validation=None):
         start_evl = get_time.now()
+        if run_name is None:
+            raise Exception('run_name is None')
+        # 모델 run_id로 load
+        loaded_model, loaded_model_json = load_model(run_name)
 
         # get_file_path 실행 시 experiment 생성 시 필요한 폴더들이 다 만들어짐.
         # modeler backend 호출 시 파라미터로 경로 내 json 파일 내용을 protobuf 통해서 변환 후 gRPC로 전송을 위해 사용.
         self.dict_path = path.get_file_path(loaded_model, usedFramework='tensorflow')
 
         # dependencies를 가져오기 위한 작업
         if is_in_ipython():
-            var_model_file_path = self.notebook_info
+            # var_model_file_path = self.notebook_info
             _caller_globals = inspect.stack()[1][0].f_globals
             (
                 mainfile,
                 sources,
                 dependencies
             ) = gather_sources_and_dependencies(
                 globs=_caller_globals,
@@ -80,106 +82,110 @@
                 mainfile,
                 sources,
                 dependencies
             ) = gather_sources_and_dependencies(
                 globs=_caller_globals,
                 save_git_info=True
             )
-            var_model_file_path = mainfile['filename']
+            # var_model_file_path = mainfile['filename']
 
+        # run_nickname 설정: 미설정 시 default_run_nick_name(파일 이름) 으로 설정
         if run_nickname_input is None:
             run_nick_name = self.default_run_nick_name
         else:
             run_nick_name = run_nickname_input
 
-
+        # 모델과 검증용 데이터 유무 판별
+        # loaded_model_json: 모델의 json 파일 내용 -> /runs/best-model/ 아래 존재
         if loaded_model is None or x_validation is None or y_validation is None or loaded_model_json is None:
             raise ValueError("Please set parameter -> model or validation data. ")
         x_val = x_validation
         y_val = y_validation
 
         # set current run
-        set_current_runs(RUN_NAME_TENSORFLOW)
+        set_current_runs(RUN_NAME_KERAS)
 
         # path for for-evl-json
         # visualCallback 참고 해서 actual data로 성능평가
         path_for_setting_evl_json = self.dict_path['evl_json']
         evl_json_full_path = self.dict_path[RUN_MODEL_EVL_JSON_PATH]
         set_evl_json_path(path_for_setting_evl_json)
 
+        # json to dict
         loaded_model_json_dict = json.loads(loaded_model_json)
         loss_function = loaded_model_json_dict['loss_function']
         run_id = loaded_model_json_dict['run_id']
 
         '''
         RunInfo.py 내 아래 데이터에 set
         global _runData
         run_obj = _runData[0]
         '''
+        # 아래 set_ ~~ 함수들은 modeler-api를 통해 DB에 데이터 유지 + UI 표기를 위한 과정
         set_optimizer_info_path(loaded_model_json_dict['optimizer_info'])
         set_model_file_path(loaded_model_json_dict['path'])
         set_python_dependencies(py_depenpency=loaded_model_json_dict['model_dependencies'])
         set_prefix_path(self.dict_path[LcConst.RUN_PREFIX_PATH])
         set_run_name('tf.keras', run_id, run_nick_name)
 
         set_best_model_json_path(loaded_model_json_dict['best_model_json'])
         set_best_model_h5_path(loaded_model_json_dict['best_model_h5'])
 
 
         # 모델 라이브러리 확인 (tf or keras)
-        if isinstance(loaded_model, tensorflow.keras.Model): #Sequential은 Model에서 상속 받아 같음.
-
-            # print(loss_function)
-            # print(self.dict_path[RUN_MODEL_EVL_JSON_PATH])
-
+        if isinstance(loaded_model, keras.Model): #Sequential은 Model에서 상속 받아 같음.
             # classification
             if loss_function in lossFuncInfo.CLASSIFICATION:
                 print("DL_CLASSIFICATION in model_evaluation method")
-                visual_classification_json = roc_pr_curve(loaded_model, x_val, y_val, f1_average=f1_average_in,
-                                                          recall_average=recall_average_in)
+                # roc pr curve
+                visual_classification_json = roc_pr_curve(loaded_model, x_val, y_val, f1_average="weighted",
+                                                          recall_average="weighted")
                 with open(evl_json_full_path, 'w', encoding='utf-8') as save_file:
                     json.dump(visual_classification_json, save_file, indent="\t")
 
-                selected_metrics = modelEvaluation.calculate_classification_metrics(loaded_model, x_val, y_val, average=f1_average_in)
+                # confusion matrix, f1, recall, precision
+                selected_metrics = modelEvaluation.calculate_classification_metrics(loaded_model, x_val, y_val, average='weighted')
                 set_model_type("DL_CLASSIFICATION")
+
             # regression
             elif loss_function in lossFuncInfo.REGRESSION:
                 print("DL_REGRESSION in model_evaluation method")
                 visual_regression_json = OrderedDict()
                 visual_regression_json['True_y'] = get_true_y(y_val)
+                # predict_y
                 visual_regression_json['Predicted_y'] = get_visual_info_regressor(loaded_model, x_val)
 
-                set_true_y(visual_regression_json['True_y'])
-                set_predict_y(visual_regression_json['Predicted_y'])
-
                 with open(evl_json_full_path, 'w', encoding='utf-8') as save_file:
                     json.dump(visual_regression_json, save_file, indent="\t")
 
+                # mae, mse, rmse, r2, mape
                 selected_metrics = modelEvaluation.calculate_regression_metrics(loaded_model, x_val, y_val)
                 set_model_type("DL_REGRESSION")
 
             else:
-                raise ValueError('현재 설정한 모델은 지원되지 않습니다. 관리자에게 문의하십시오.')
+                raise ValueError('현재 설정한 loss는 지원되지 않습니다. 관리자에게 문의하십시오.')
         else: # keras 만을 사용한 경우 없음. 추후 pytorch 대응용
             pass
         loaded_model_json_dict[SELECTED_METRICS] = selected_metrics
         set_selected_metrics_path(loaded_model_json_dict[SELECTED_METRICS])
 
         end_evl = get_time.now()
 
         start_ts = int(start_evl.timestamp())
         end_ts = int(end_evl.timestamp())
         delta_ts = end_ts - start_ts
 
+        # 현재까지 set 했던 run 정보를 run_meta dict에 담아서 modeler-api로 전송
         run_meta = clear_runs(start_ts, end_ts, delta_ts, isEvaluation="true")
-
+        print(run_meta)
         env_value = get_os_env('ENV')
         modeler_rest = LifecycleRestApi(env_value[LcConst.BACK_END_API_URL],
                                         env_value[LcConst.BACK_END_API_PORT],
                                         env_value[LcConst.BACK_END_API_URI])
+        # modeler-api로 전송
         modeler_rest.lc_create_run(run_meta)
 
     def autolog(self, run_nickname_input=None, tag=None, best_weights=False, model_monitor=False, runtime=False, f1_average_in='weighted', recall_average_in='weighted'):
         global description, endpoint, var_model_file_path, message, thresholds, best_weights_on, run_id, alarm, alarm_api, shap_on, feature_name, run_meta, run_nick_name
         description = tag
         endpoint = self.endpoint
         message = self.message # common.py send_message 호출을 통해 생성
@@ -242,22 +248,25 @@
                 dependencies
             ) = gather_sources_and_dependencies(
                 globs=_caller_globals,
                 save_git_info=True
             )
             var_model_file_path = mainfile['filename']
 
-        class TrainHistoryCallbacks(tensorflow.keras.callbacks.Callback):
-            def __init__(self, verbose=1, mode='auto'):
+        class TrainHistoryCallbacks(keras.callbacks.Callback):
+            def __init__(self, verbose=1, mode='auto', period=1):
                 super(TrainHistoryCallbacks, self).__init__()
                 self.verbose = verbose
+                self.period = period
                 self.best_epochs = 0
                 self.epochs_since_last_save = 0
                 self.mode = mode
                 self.model_summary = OrderedDict()
+                self.run_id = None
+                self.model_type = None
 
             def on_train_begin(self, logs={}):
                 logging.info('Using autolog(best_weights={}, model_monitor={}'
                              .format(str(best_weights_on), str(shap_on)))
 
                 global start
                 start = get_time.now()
@@ -281,15 +290,15 @@
                     self.model_summary['loss_function'] = self.model.loss
 
                 self.model_summary['optimizer_info'] = {opt['name']: opt_result}
 
                 '''[get best model] on_train_begin '''
                 self.best_weights = self.model.get_weights()
 
-                self.dict_path = path.get_file_path(self.model, usedFramework='tensorflow')
+                self.dict_path = path.get_file_path(self.model, usedFramework='keras')
 
                 set_prefix_path(self.dict_path[LcConst.RUN_PREFIX_PATH])
 
                 set_run_name(self.model_summary['model_type'], self.model_summary['run_id'], self.model_summary['run_nick_name'])
                 set_python_dependencies(py_depenpency=dependencies)
 
             '''[get best model] on_epoch_end '''
@@ -342,24 +351,24 @@
 
                     self.current_value = current
 
                 # Not using best_weights
                 else:
                     self.last_epoch_metric = logs.get(self.monitor)
                     self.best_epochs = epoch + 1
-                    current = logs.get(self.monitor)
-                    self.current_value = current
+                    self.current_value = logs.get(self.monitor)
 
                 # model save path
                 run_id = self.model_summary['model_type'] + '-' + self.model_summary['run_id']
-                common_path = self.dict_path['save_model_path'] + run_id + '-epoch-' + str(epoch + 1).zfill(5) + '-' + self.monitor + '-' + str(current).zfill(5)
+                common_path = self.dict_path['save_model_path'] + run_id + '-epoch-' + str(epoch + 1).zfill(5) \
+                              + '-' + self.monitor + '-' + str(current).zfill(5)
                 save_model_path = common_path + '.json'
                 save_weights_path = common_path + '.h5'
 
-                # model evaluation path(in jupyter lab browser path - 상대경로 의미...)
+                # model evaluation path(in jupyter lab browser path)
                 browser_common_path = self.dict_path['save_model_dir'] + '/' + run_id + '-epoch-' + str(epoch + 1).zfill(
                     5) + '-' + self.monitor + '-' + str(current).zfill(5)
                 save_model_path_browser = browser_common_path + '.json'
                 save_weights_path_browser = browser_common_path + '.h5'
 
                 # model to JSON
                 model_json = self.model.to_json()
@@ -385,38 +394,35 @@
 
                 # weights to H5
                 # self.model.save_weights(save_weights_path)
                 self.model.save(save_weights_path)
 
             def on_train_end(self, logs={}):
                 '''[get best model] on_train_end '''
-                if best_weights_on:
-                    if self.verbose > 0:
-                        print('\nUsing epoch %05d with %s: %0.5f' % (self.best_epochs, self.monitor, self.best))
-                    self.model.set_weights(self.best_weights)  # set best model's weights
-                    
-                    self.model_summary[SELECTED_METRICS] = {self.monitor: np.float64(self.best)}
-                else:
-                    self.model_summary[SELECTED_METRICS] = {self.monitor: np.float64(self.last_epoch_metric)}
-    
-          #      print('model_summary: ', self.model_summary)   ##############################
+                if self.verbose > 0:
+                    print('Using epoch %05d with %s: %0.5f' % (self.best_epochs, self.monitor, self.best))
+                self.model.set_weights(self.best_weights)  # set best model's weights
+                
                 end = get_time.now()
                 self.model_summary['time_delta'] = str(end - start)
-
+                self.model_summary[SELECTED_METRICS] = {self.monitor: self.best}
+            
                 # path for model_info.json
-                self.path_for_setting_model_json = self.dict_path['model_json']
-                set_model_json_path(self.path_for_setting_model_json)
-
+                set_model_json_path(self.dict_path['model_json'])
                 model_json_full_path = self.dict_path[RUN_MODEL_JSON_PATH]
 
                 with open(model_json_full_path, 'w', encoding='utf-8') as save_file:
                     json.dump(self.model_summary, save_file, indent="\t")
-
-                delete_files_except_best(run_id=self.model_summary['run_id'], epochs=str(self.best_epochs),
-                                         path=self.dict_path)
+            
+                if best_weights_on:
+                    delete_files_except_best(run_id=self.model_summary['run_id'], epochs=str(self.best_epochs),
+                                            path=self.dict_path)
+                else:
+                    delete_files_except_best(run_id=self.model_summary['run_id'], epochs=str(self.last_epochs),
+                    path=self.dict_path)
 
                 path_for_setting_model_json = self.dict_path['save_model_dir'] + \
                                               get_best_model_path(run_id=self.model_summary['run_id'],
                                                                   path=self.dict_path)['json']
                 path_for_setting_model_h5 = self.dict_path['save_model_dir'] + \
                                             get_best_model_path(run_id=self.model_summary['run_id'],
                                                                 path=self.dict_path)['h5']
@@ -428,33 +434,36 @@
                 delta_ts = end_ts - start_ts
 
                 global run_meta
                 run_meta = clear_runs(start_ts, end_ts, delta_ts)
                 accuinsight._send_message(metric=self.monitor,
                                           current_value=self.current_value,
                                           message=message,
-                                          alarm_object=alarm,
+                                          thresholds=thresholds,
+                                          alarm_object=None,
+                                          # direct_email=,
                                           alarm_api=alarm_api)
                 env_value = get_os_env('ENV')
                 modeler_rest = LifecycleRestApi(env_value[LcConst.BACK_END_API_URL],
                                                 env_value[LcConst.BACK_END_API_PORT],
                                                 env_value[LcConst.BACK_END_API_URI])
                 modeler_rest.lc_create_run(run_meta)
                 if runtime:
-                    accuinsight.set_runtime_model('tensorflow')
-                accuinsight._off_autolog()
+                    accuinsight.set_runtime_model('keras')
+                accuinsight.off_autolog()
 
-        class visualCallbacks(tensorflow.keras.callbacks.Callback):
+        class visualCallbacks(keras.callbacks.Callback):
             def __init__(self, x_validation=None, y_validation=None):
                 super(visualCallbacks, self).__init__()
                 self.x_val = x_validation
                 self.y_val = y_validation
 
             def on_train_end(self, logs={}):
-                self.dict_path = path.get_file_path(self.model, usedFramework='tensorflow')
+                self.dict_path = path.get_file_path(self.model, usedFramework='keras')
+
                 # path for visual.json
                 path_for_setting_visual_json = self.dict_path['visual_json']
                 visual_json_full_path = self.dict_path[RUN_MODEL_VISUAL_JSON_PATH]
                 set_visual_json_path(path_for_setting_visual_json)
 
                 # classification
                 if get.is_classification(self.model):
@@ -462,85 +471,94 @@
 
                     with open(visual_json_full_path, 'w', encoding='utf-8') as save_file:
                         json.dump(visual_classification_json, save_file, indent="\t")
 
                 # regression
                 else:
                     visual_regression_json = OrderedDict()
-                    visual_regression_json['True_y'] = get_true_y(self.y_val)
+                    visual_regression_json['True_y'] = self.y_val.tolist()
                     visual_regression_json['Predicted_y'] = get_visual_info_regressor(self.model, self.x_val)
 
                     with open(visual_json_full_path, 'w', encoding='utf-8') as save_file:
                         json.dump(visual_regression_json, save_file, indent="\t")
 
-        class shapCallbacks(tensorflow.keras.callbacks.Callback):
+        class shapCallbacks(keras.callbacks.Callback):
             def __init__(self, trainX, feature_name, run_id, trigger=shap_on):
                 super(shapCallbacks, self).__init__()
                 self.trainX = trainX
                 self.trigger = trigger
                 self.run_id = run_id
                 self.feature_name_in_shap = feature_name
 
             def on_train_end(self, logs={}):
                 if self.trigger:
                     self.shap_value = shap_value(self.model, self.trainX, self.feature_name_in_shap)
-                    
-#                     func.insertDB(self.shap_value, 2)  # 수정: 2 -> self.run_id
-                    
-                    self.dict_path = path.get_file_path(self.model, usedFramework='tensorflow')
+
+                    self.dict_path = path.get_file_path(self.model, usedFramework='keras')
 
                     # path for shap.json
-                    shap_json_full_path = self.dict_path['shap_json_full']
+                    shap_json_full_path = self.dict_path[RUN_MODEL_SHAP_JSON_PATH]
                     set_shap_json_path(self.dict_path['shap_json'])
 
                     with open(shap_json_full_path, 'w', encoding='utf-8') as save_file:
                         json.dump(self.shap_value, save_file, indent='\t')
 
                 else:
                     pass
 
-        def run_and_log_function(self, original, x, y, kwargs):
-            dict_path = path.get_file_path(self, usedFramework='tensorflow')
+        def run_and_log_function(self, original, x, y, kwargs, unlogged_params):
+            dict_path = path.get_file_path(self, usedFramework='keras')
+
             path_for_setting_visual_csv = dict_path['visual_csv']
-            visual_csv_full_path = dict_path[RUN_MODEL_VISUAL_CSV_PATH]
+            visual_csv_full_path = dict_path['visual_csv_full']
 
             # set current run
-            set_current_runs(RUN_NAME_TENSORFLOW)
+            set_current_runs(RUN_NAME_KERAS)
             set_model_file_path(var_model_file_path)
             set_visual_csv_path(path_for_setting_visual_csv)
 
             csv_logger = CSVLogger(visual_csv_full_path, append=True, separator=';')
 
             # get train data(x) for computing shap value
             if 'x':
                 x_train = x
             if shap_on:
                 get_shap = shapCallbacks(x_train, feature_name, run_id, trigger=shap_on)
             else:
                 pass
-
+ 
             ''' save json for visualization '''
+            kwargs_dict = OrderedDict()
+            
+            for key, value in kwargs.items():
+                kwargs_dict[key] = value
+            
             # using validation_data argument
-            if 'validation_data' in kwargs:
+            if 'validation_data' in kwargs_dict.keys():
                 validation_set = kwargs['validation_data']
 
                 try:
                     x_val = validation_set[0]
                     y_val = validation_set[1]
 
                 except:
                     iterator = iter(validation_set)
                     valid_set = next(iterator)
                     x_val = valid_set[0].numpy()
                     y_val = valid_set[1].numpy()
-
-                get_visual = visualCallbacks(x_validation=x_val, y_validation=y_val)
-
+            
+#            elif 'validation_split' in kwargs_dict.keys():
+#                (x, y), validation_set = (data_adapter.train_validation_split((x,y), validation_split=kwargs_dict['validation_split']))
+#                if validation_set:
+#                    x_val, y_val, val_sample_weight = (data_adapter.unpack_x_y_sample_weight(validation_set))
+#
             else:
-                raise ValueError('"validation_data" does not exist.')
+                raise ValueError('"validation_data" or "validation_split" does not exist.')
+            
+            get_visual = visualCallbacks(x_validation=x_val, y_validation=y_val)
 
             if 'callbacks' in kwargs:
                 kwargs['callbacks'] += [csv_logger]
             else:
                 kwargs['callbacks'] = [csv_logger]
 
             kwargs['callbacks'] += [get_visual]
@@ -548,28 +566,28 @@
                 kwargs['callbacks'] += [get_shap]
             else:
                 pass
             kwargs['callbacks'] += [TrainHistoryCallbacks()]
 
             return original(self, x, y, **kwargs)
 
-        @gorilla.patch(tensorflow.keras.Model)
+        @gorilla.patch(keras.Model)
         def fit(self, x, y, **kwargs):
-            original = gorilla.get_original_attribute(tensorflow.keras.Model, 'fit')
-            unlogged_params = ['self', 'callbacks', 'validation_data', 'verbose']
-            return run_and_log_function(self, original, x, y, kwargs)
+            original = gorilla.get_original_attribute(keras.Model, 'fit')
+            unlogged_params = ['self', 'x', 'y', 'callbacks', 'validation_data', 'verbose']
+            return run_and_log_function(self, original, x, y, kwargs, unlogged_params)
 
         settings = gorilla.Settings(allow_hit=True, store_hit=True)
-        gorilla.apply(gorilla.Patch(tensorflow.keras.Model, 'fit', fit, settings=settings))
+        gorilla.apply(gorilla.Patch(keras.Model, 'fit', fit, settings=settings))
 
-    def _off_autolog():
+    def off_autolog():
         def stop_log(self, original, args, kwargs, unlogged_params):
             return original(self, *args, **kwargs)
 
-        @gorilla.patch(tensorflow.keras.Model)
+        @gorilla.patch(keras.Model)
         def fit(self, *args, **kwargs):
-            original = gorilla.get_original_attribute(tensorflow.keras.Model, 'fit')
+            original = gorilla.get_original_attribute(keras.Model, 'fit')
             unlogged_params = ['self', 'x', 'y', 'callbacks', 'validation_data', 'verbose']
             return stop_log(self, original, args, kwargs, unlogged_params)
 
         settings = gorilla.Settings(allow_hit=True, store_hit=True)
-        gorilla.apply(gorilla.Patch(tensorflow.keras.Model, 'fit', fit, settings=settings))
+        gorilla.apply(gorilla.Patch(keras.Model, 'fit', fit, settings=settings))
```

### Comparing `Accuinsight-3.4.230516rc1/Accuinsight/Lifecycle/utils.py` & `Accuinsight-3.4.230530/Accuinsight/Lifecycle/utils.py`

 * *Files identical despite different names*

### Comparing `Accuinsight-3.4.230516rc1/Accuinsight/Monitoring/deploy/monitoring_deploy.py` & `Accuinsight-3.4.230530/Accuinsight/Monitoring/deploy/monitoring_deploy.py`

 * *Files identical despite different names*

### Comparing `Accuinsight-3.4.230516rc1/Accuinsight/WorkspaceRun/workspace_run.py` & `Accuinsight-3.4.230530/Accuinsight/WorkspaceRun/workspace_run.py`

 * *Files identical despite different names*

### Comparing `Accuinsight-3.4.230516rc1/Accuinsight/exceptions.py` & `Accuinsight-3.4.230530/Accuinsight/exceptions.py`

 * *Files identical despite different names*

### Comparing `Accuinsight-3.4.230516rc1/Accuinsight/modeler/clients/modeler_api.py` & `Accuinsight-3.4.230530/Accuinsight/modeler/clients/modeler_api.py`

 * *Files identical despite different names*

### Comparing `Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/LcConst/LcConst.py` & `Accuinsight-3.4.230530/Accuinsight/modeler/core/LcConst/LcConst.py`

 * *Files identical despite different names*

### Comparing `Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/ModelType.py` & `Accuinsight-3.4.230530/Accuinsight/modeler/core/ModelType.py`

 * *Files identical despite different names*

### Comparing `Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/Run/ParseRun/BaseParser.py` & `Accuinsight-3.4.230530/Accuinsight/modeler/core/Run/ParseRun/BaseParser.py`

 * *Files identical despite different names*

### Comparing `Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/Run/ParseRun/ParseExperiment.py` & `Accuinsight-3.4.230530/Accuinsight/modeler/core/Run/ParseRun/ParseExperiment.py`

 * *Files identical despite different names*

### Comparing `Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/Run/ParseRun/ParseKeras.py` & `Accuinsight-3.4.230530/Accuinsight/modeler/core/Run/ParseRun/ParseKeras.py`

 * *Files identical despite different names*

### Comparing `Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/Run/ParseRun/Parse_DLClassification.py` & `Accuinsight-3.4.230530/Accuinsight/modeler/core/Run/ParseRun/Parse_DLClassification.py`

 * *Files identical despite different names*

### Comparing `Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/Run/ParseRun/Parse_DLClassification_evl.py` & `Accuinsight-3.4.230530/Accuinsight/modeler/core/Run/ParseRun/Parse_DLClassification_evl.py`

 * *Files identical despite different names*

### Comparing `Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/Run/ParseRun/Parse_DLRegression.py` & `Accuinsight-3.4.230530/Accuinsight/modeler/core/Run/ParseRun/Parse_DLRegression.py`

 * *Files identical despite different names*

### Comparing `Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/Run/ParseRun/Parse_DLRegression_evl.py` & `Accuinsight-3.4.230530/Accuinsight/modeler/core/Run/ParseRun/Parse_DLRegression_evl.py`

 * *Files identical despite different names*

### Comparing `Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/Run/ParseRun/Parse_MLClassifier.py` & `Accuinsight-3.4.230530/Accuinsight/modeler/core/Run/ParseRun/Parse_MLClassifier.py`

 * *Files identical despite different names*

### Comparing `Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/Run/ParseRun/Parse_MLClassifier_evl.py` & `Accuinsight-3.4.230530/Accuinsight/modeler/core/Run/ParseRun/Parse_MLClassifier_evl.py`

 * *Files identical despite different names*

### Comparing `Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/Run/ParseRun/Parse_MLRegression.py` & `Accuinsight-3.4.230530/Accuinsight/modeler/core/Run/ParseRun/Parse_MLRegression.py`

 * *Files identical despite different names*

### Comparing `Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/Run/ParseRun/Parse_MLRegression_evl.py` & `Accuinsight-3.4.230530/Accuinsight/modeler/core/Run/ParseRun/Parse_MLRegression_evl.py`

 * *Files identical despite different names*

### Comparing `Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/Run/ParseRun/ParserVisualJaon.py` & `Accuinsight-3.4.230530/Accuinsight/modeler/core/Run/ParseRun/ParserVisualJaon.py`

 * *Files identical despite different names*

### Comparing `Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/Run/RunInfo/RunInfo.py` & `Accuinsight-3.4.230530/Accuinsight/modeler/core/Run/RunInfo/RunInfo.py`

 * *Files identical despite different names*

### Comparing `Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/Run/RunOjbject.py` & `Accuinsight-3.4.230530/Accuinsight/modeler/core/Run/RunOjbject.py`

 * *Files identical despite different names*

### Comparing `Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/feature_contribution.py` & `Accuinsight-3.4.230530/Accuinsight/modeler/core/feature_contribution.py`

 * *Files identical despite different names*

### Comparing `Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/func_for_visual.py` & `Accuinsight-3.4.230530/Accuinsight/modeler/core/func_for_visual.py`

 * *Files identical despite different names*

### Comparing `Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/get.py` & `Accuinsight-3.4.230530/Accuinsight/modeler/core/get.py`

 * *Files identical despite different names*

### Comparing `Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/get_for_visual.py` & `Accuinsight-3.4.230530/Accuinsight/modeler/core/get_for_visual.py`

 * *Files identical despite different names*

### Comparing `Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/lossFuncInfo.py` & `Accuinsight-3.4.230530/Accuinsight/modeler/core/lossFuncInfo.py`

 * *Files identical despite different names*

### Comparing `Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/metricsLightgbm.py` & `Accuinsight-3.4.230530/Accuinsight/modeler/core/metricsLightgbm.py`

 * *Files identical despite different names*

### Comparing `Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/modelEvaluation.py` & `Accuinsight-3.4.230530/Accuinsight/modeler/core/modelEvaluation.py`

 * *Files identical despite different names*

### Comparing `Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/path.py` & `Accuinsight-3.4.230530/Accuinsight/modeler/core/path.py`

 * *Files identical despite different names*

### Comparing `Accuinsight-3.4.230516rc1/Accuinsight/modeler/entities/_modeler_object.py` & `Accuinsight-3.4.230530/Accuinsight/modeler/entities/_modeler_object.py`

 * *Files identical despite different names*

### Comparing `Accuinsight-3.4.230516rc1/Accuinsight/modeler/entities/alarm.py` & `Accuinsight-3.4.230530/Accuinsight/modeler/entities/alarm.py`

 * *Files identical despite different names*

### Comparing `Accuinsight-3.4.230516rc1/Accuinsight/modeler/entities/lc_artifact.py` & `Accuinsight-3.4.230530/Accuinsight/modeler/entities/lc_artifact.py`

 * *Files identical despite different names*

### Comparing `Accuinsight-3.4.230516rc1/Accuinsight/modeler/entities/lc_metric.py` & `Accuinsight-3.4.230530/Accuinsight/modeler/entities/lc_metric.py`

 * *Files identical despite different names*

### Comparing `Accuinsight-3.4.230516rc1/Accuinsight/modeler/entities/lc_param.py` & `Accuinsight-3.4.230530/Accuinsight/modeler/entities/lc_param.py`

 * *Files identical despite different names*

### Comparing `Accuinsight-3.4.230516rc1/Accuinsight/modeler/entities/lc_run.py` & `Accuinsight-3.4.230530/Accuinsight/modeler/entities/lc_run.py`

 * *Files identical despite different names*

### Comparing `Accuinsight-3.4.230516rc1/Accuinsight/modeler/entities/lc_run_info.py` & `Accuinsight-3.4.230530/Accuinsight/modeler/entities/lc_run_info.py`

 * *Files identical despite different names*

### Comparing `Accuinsight-3.4.230516rc1/Accuinsight/modeler/entities/lc_run_status.py` & `Accuinsight-3.4.230530/Accuinsight/modeler/entities/lc_run_status.py`

 * *Files identical despite different names*

### Comparing `Accuinsight-3.4.230516rc1/Accuinsight/modeler/entities/lc_run_tag.py` & `Accuinsight-3.4.230530/Accuinsight/modeler/entities/lc_run_tag.py`

 * *Files identical despite different names*

### Comparing `Accuinsight-3.4.230516rc1/Accuinsight/modeler/entities/lc_stage.py` & `Accuinsight-3.4.230530/Accuinsight/modeler/entities/lc_stage.py`

 * *Files identical despite different names*

### Comparing `Accuinsight-3.4.230516rc1/Accuinsight/modeler/entities/lc_view_type.py` & `Accuinsight-3.4.230530/Accuinsight/modeler/entities/lc_view_type.py`

 * *Files identical despite different names*

### Comparing `Accuinsight-3.4.230516rc1/Accuinsight/modeler/entities/monitoring_deploy_log.py` & `Accuinsight-3.4.230530/Accuinsight/modeler/entities/monitoring_deploy_log.py`

 * *Files identical despite different names*

### Comparing `Accuinsight-3.4.230516rc1/Accuinsight/modeler/entities/workspace_run_log.py` & `Accuinsight-3.4.230530/Accuinsight/modeler/entities/workspace_run_log.py`

 * *Files identical despite different names*

### Comparing `Accuinsight-3.4.230516rc1/Accuinsight/modeler/exceptions.py` & `Accuinsight-3.4.230530/Accuinsight/modeler/exceptions.py`

 * *Files identical despite different names*

### Comparing `Accuinsight-3.4.230516rc1/Accuinsight/modeler/protos/life_cycle_pb2.py` & `Accuinsight-3.4.230530/Accuinsight/modeler/protos/life_cycle_pb2.py`

 * *Files identical despite different names*

### Comparing `Accuinsight-3.4.230516rc1/Accuinsight/modeler/protos/service_pb2.py` & `Accuinsight-3.4.230530/Accuinsight/modeler/protos/service_pb2.py`

 * *Files identical despite different names*

### Comparing `Accuinsight-3.4.230516rc1/Accuinsight/modeler/protos/skapi_pb2.py` & `Accuinsight-3.4.230530/Accuinsight/modeler/protos/skapi_pb2.py`

 * *Files identical despite different names*

### Comparing `Accuinsight-3.4.230516rc1/Accuinsight/modeler/store/tracking/lc_abstract_store.py` & `Accuinsight-3.4.230530/Accuinsight/modeler/store/tracking/lc_abstract_store.py`

 * *Files identical despite different names*

### Comparing `Accuinsight-3.4.230516rc1/Accuinsight/modeler/store/tracking/life_cycle_store.py` & `Accuinsight-3.4.230530/Accuinsight/modeler/store/tracking/life_cycle_store.py`

 * *Files identical despite different names*

### Comparing `Accuinsight-3.4.230516rc1/Accuinsight/modeler/store/tracking/monitoring_deploy_store.py` & `Accuinsight-3.4.230530/Accuinsight/modeler/store/tracking/monitoring_deploy_store.py`

 * *Files identical despite different names*

### Comparing `Accuinsight-3.4.230516rc1/Accuinsight/modeler/store/tracking/workspace_store.py` & `Accuinsight-3.4.230530/Accuinsight/modeler/store/tracking/workspace_store.py`

 * *Files identical despite different names*

### Comparing `Accuinsight-3.4.230516rc1/Accuinsight/modeler/utils/__init__.py` & `Accuinsight-3.4.230530/Accuinsight/modeler/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `Accuinsight-3.4.230516rc1/Accuinsight/modeler/utils/dependency/dependencies.py` & `Accuinsight-3.4.230530/Accuinsight/modeler/utils/dependency/dependencies.py`

 * *Files identical despite different names*

### Comparing `Accuinsight-3.4.230516rc1/Accuinsight/modeler/utils/dependency/settings.py` & `Accuinsight-3.4.230530/Accuinsight/modeler/utils/dependency/settings.py`

 * *Files identical despite different names*

### Comparing `Accuinsight-3.4.230516rc1/Accuinsight/modeler/utils/dl_utils.py` & `Accuinsight-3.4.230530/Accuinsight/modeler/utils/dl_utils.py`

 * *Files identical despite different names*

### Comparing `Accuinsight-3.4.230516rc1/Accuinsight/modeler/utils/os_getenv.py` & `Accuinsight-3.4.230530/Accuinsight/modeler/utils/os_getenv.py`

 * *Files identical despite different names*

### Comparing `Accuinsight-3.4.230516rc1/Accuinsight/modeler/utils/proto_json_utils.py` & `Accuinsight-3.4.230530/Accuinsight/modeler/utils/proto_json_utils.py`

 * *Files identical despite different names*

### Comparing `Accuinsight-3.4.230516rc1/Accuinsight/modeler/utils/rest_utils.py` & `Accuinsight-3.4.230530/Accuinsight/modeler/utils/rest_utils.py`

 * *Files identical despite different names*

### Comparing `Accuinsight-3.4.230516rc1/Accuinsight/modeler/utils/runs_utils.py` & `Accuinsight-3.4.230530/Accuinsight/modeler/utils/runs_utils.py`

 * *Files identical despite different names*

### Comparing `Accuinsight-3.4.230516rc1/Accuinsight.egg-info/PKG-INFO` & `Accuinsight-3.4.230530/Accuinsight.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Accuinsight
-Version: 3.4.230516rc1
+Version: 3.4.230530
 Summary: Model life cycle and monitoring library in Accuinsight+
 Home-page: 
 Author: SK
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
```

### Comparing `Accuinsight-3.4.230516rc1/Accuinsight.egg-info/SOURCES.txt` & `Accuinsight-3.4.230530/Accuinsight.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -81,18 +81,14 @@
 Accuinsight/modeler/entities/lc_view_type.py
 Accuinsight/modeler/entities/monitoring_deploy_log.py
 Accuinsight/modeler/entities/workspace_run_log.py
 Accuinsight/modeler/protos/__init__.py
 Accuinsight/modeler/protos/life_cycle_pb2.py
 Accuinsight/modeler/protos/service_pb2.py
 Accuinsight/modeler/protos/skapi_pb2.py
-Accuinsight/modeler/protos_bak/__init__.py
-Accuinsight/modeler/protos_bak/life_cycle_pb2.py
-Accuinsight/modeler/protos_bak/service_pb2.py
-Accuinsight/modeler/protos_bak/skapi_pb2.py
 Accuinsight/modeler/store/__init__.py
 Accuinsight/modeler/store/tracking/__init__.py
 Accuinsight/modeler/store/tracking/lc_abstract_store.py
 Accuinsight/modeler/store/tracking/life_cycle_store.py
 Accuinsight/modeler/store/tracking/monitoring_deploy_store.py
 Accuinsight/modeler/store/tracking/workspace_store.py
 Accuinsight/modeler/utils/__init__.py
```

### Comparing `Accuinsight-3.4.230516rc1/PKG-INFO` & `Accuinsight-3.4.230530/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Accuinsight
-Version: 3.4.230516rc1
+Version: 3.4.230530
 Summary: Model life cycle and monitoring library in Accuinsight+
 Home-page: 
 Author: SK
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
```

### Comparing `Accuinsight-3.4.230516rc1/README.rst` & `Accuinsight-3.4.230530/README.rst`

 * *Files identical despite different names*

### Comparing `Accuinsight-3.4.230516rc1/setup.py` & `Accuinsight-3.4.230530/setup.py`

 * *Files identical despite different names*

