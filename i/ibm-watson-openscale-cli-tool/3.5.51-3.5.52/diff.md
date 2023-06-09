# Comparing `tmp/ibm-watson-openscale-cli-tool-3.5.51.tar.gz` & `tmp/ibm-watson-openscale-cli-tool-3.5.52.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ibm-watson-openscale-cli-tool-3.5.51.tar", last modified: Thu Jan 12 04:03:03 2023, max compression
+gzip compressed data, was "ibm-watson-openscale-cli-tool-3.5.52.tar", last modified: Fri Jun  9 07:48:08 2023, max compression
```

## Comparing `ibm-watson-openscale-cli-tool-3.5.51.tar` & `ibm-watson-openscale-cli-tool-3.5.52.tar`

### file list

```diff
@@ -1,197 +1,233 @@
-drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-01-12 04:03:03.259409 ibm-watson-openscale-cli-tool-3.5.51/
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)    10173 2022-08-01 08:55:50.000000 ibm-watson-openscale-cli-tool-3.5.51/LICENSE
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)      215 2022-08-01 08:55:50.000000 ibm-watson-openscale-cli-tool-3.5.51/MANIFEST.in
--rw-r--r--   0 prateekgoyal   (501) staff       (20)    21142 2023-01-12 04:03:03.258177 ibm-watson-openscale-cli-tool-3.5.51/PKG-INFO
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)    20369 2022-08-01 08:55:50.000000 ibm-watson-openscale-cli-tool-3.5.51/README.md
-drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-01-12 04:03:02.954468 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/
--rw-r--r--   0 prateekgoyal   (501) staff       (20)        6 2023-01-11 05:32:27.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/VERSION
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)     1557 2022-08-01 08:54:52.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/__init__.py
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)     4804 2022-08-01 08:54:52.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/api_environment.py
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)     4705 2022-08-01 08:54:52.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/credentials.py
-drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-01-12 04:03:02.958555 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/database_classes/
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)     4514 2022-08-01 08:54:52.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/database_classes/cos.py
--rw-r--r--   0 prateekgoyal   (501) staff       (20)    13546 2022-09-26 12:11:09.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/database_classes/db2.py
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)     7086 2022-08-01 08:54:52.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/database_classes/postgres.py
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)     1078 2022-08-01 08:54:52.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/database_classes/postgres_compose.py
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)     1055 2022-08-01 08:54:52.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/database_classes/postgres_icd.py
--rw-r--r--   0 prateekgoyal   (501) staff       (20)     1258 2023-01-11 05:30:47.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/enums.py
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)     5310 2022-08-01 08:54:52.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/environments.py
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)    21757 2022-05-09 05:42:16.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/main.py
-drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-01-12 04:03:02.961237 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/ml_engines/
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)     2900 2022-08-01 08:54:52.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/ml_engines/azure_machine_learning.py
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)     1875 2022-08-01 08:54:52.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/ml_engines/custom_machine_learning.py
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)     2084 2022-08-01 08:54:52.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/ml_engines/sagemaker_machine_learning.py
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)     1584 2022-08-01 08:54:52.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/ml_engines/spss_machine_learning.py
--rw-r--r--   0 prateekgoyal   (501) staff       (20)    24887 2023-01-11 05:30:47.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/ml_engines/watson_machine_learning.py
-drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-01-12 04:03:02.962364 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/
-drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-01-12 04:03:02.976563 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/
-drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-01-12 04:03:02.978543 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/azuremlservice/
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)     2512 2022-08-01 08:54:52.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/azuremlservice/configuration.json
-drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-01-12 04:03:02.980888 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/azuremlstudio/
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)     2512 2022-08-01 08:54:52.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/azuremlstudio/configuration.json
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)   200347 2022-08-01 08:54:52.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/azuremlstudio/history_payloads.json
-drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-01-12 04:03:02.984102 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/custom/
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)     2500 2022-08-01 08:54:52.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/custom/configuration.json
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)   116539 2022-08-01 08:54:52.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/custom/history_payloads.json
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)     7171 2022-08-01 08:54:52.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/feedback_data.csv
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)  1152715 2022-08-01 08:54:52.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/history_fairness.json
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)    90011 2022-08-01 08:54:52.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/history_quality_monitor.json
-drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-01-12 04:03:02.998475 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/sagemaker/
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)     5766 2022-08-01 08:54:52.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/sagemaker/configuration.json
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)     7631 2022-08-01 08:54:52.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/sagemaker/feedback_data.csv
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)   561618 2022-08-01 08:54:52.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/sagemaker/history_fairness.json
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)   107766 2022-08-01 08:54:52.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/sagemaker/history_payloads.json
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)   634377 2022-08-01 08:54:52.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/sagemaker/training_data.csv
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)    24287 2022-08-01 08:54:52.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/sagemaker/training_data_statistics.json
-drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-01-12 04:03:03.000805 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/spss/
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)     2503 2022-08-01 08:54:52.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/spss/configuration.json
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)   337912 2022-08-01 08:54:52.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/spss/history_payloads.json
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)   688531 2022-08-01 08:54:52.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/training_data.csv
--rw-r--r--   0 prateekgoyal   (501) staff       (20)    31533 2022-12-08 09:39:57.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/training_data_statistics.json
-drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-01-12 04:03:03.193998 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)     5916 2022-08-01 08:54:52.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/configuration.json
-drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-01-12 04:03:02.939096 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/drift_archives/
-drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-01-12 04:03:02.937794 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/drift_archives/spark_2.4_model/
-drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-01-12 04:03:03.195023 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/drift_archives/spark_2.4_model/scikit_0.20.2/
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)   224491 2022-08-01 08:54:52.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/drift_archives/spark_2.4_model/scikit_0.20.2/drift_archive.tar.gz
-drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-01-12 04:03:03.196757 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/drift_archives/spark_2.4_model/scikit_0.24.1/
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)   166282 2022-08-01 08:54:52.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/drift_archives/spark_2.4_model/scikit_0.24.1/drift_archive.tar.gz
-drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-01-12 04:03:03.198578 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/drift_archives/spark_2.4_model/scikit_0.24.2/
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)   166284 2022-08-01 08:54:52.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/drift_archives/spark_2.4_model/scikit_0.24.2/drift_archive.tar.gz
-drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-01-12 04:03:02.938450 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/drift_archives/spark_3.0_model/
-drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-01-12 04:03:03.199957 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/drift_archives/spark_3.0_model/scikit_0.24.1/
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)   121711 2022-08-04 06:39:13.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/drift_archives/spark_3.0_model/scikit_0.24.1/drift_archive.tar.gz
-drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-01-12 04:03:03.201851 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/drift_archives/spark_3.0_model/scikit_1.0.2/
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)   121637 2022-08-04 06:39:13.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/drift_archives/spark_3.0_model/scikit_1.0.2/drift_archive.tar.gz
-drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-01-12 04:03:02.938852 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/drift_archives/spark_3.2_model/
-drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-01-12 04:03:03.203361 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/drift_archives/spark_3.2_model/scikit_1.0.2/
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)   121595 2022-08-04 06:39:13.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/drift_archives/spark_3.2_model/scikit_1.0.2/drift_archive.tar.gz
-drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-01-12 04:03:02.939255 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/drift_archives/spark_3.3_model/
-drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-01-12 04:03:03.204853 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/drift_archives/spark_3.3_model/scikit_1.0.2/
--rw-r--r--   0 prateekgoyal   (501) staff       (20)   121449 2023-01-10 12:44:29.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/drift_archives/spark_3.3_model/scikit_1.0.2/drift_archive.tar.gz
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)    14206 2022-08-01 08:55:15.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/feedback_data.csv
--rw-r--r--   0 prateekgoyal   (501) staff       (20)   710154 2022-08-26 05:34:41.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_debias.json
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)   537110 2022-08-01 08:55:15.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_debiased_payloads_0.json
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)   536973 2022-08-01 08:55:15.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_debiased_payloads_1.json
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)   537385 2022-08-01 08:55:15.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_debiased_payloads_2.json
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)   537039 2022-08-01 08:55:15.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_debiased_payloads_3.json
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)   537121 2022-08-01 08:55:15.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_debiased_payloads_4.json
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)   537075 2022-08-01 08:55:15.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_debiased_payloads_5.json
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)   537028 2022-08-01 08:55:15.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_debiased_payloads_6.json
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)   241414 2022-04-25 10:20:41.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_drift_annotations_0.json
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)   271060 2022-04-25 10:20:41.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_drift_annotations_1.json
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)   278958 2022-04-25 10:20:41.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_drift_annotations_2.json
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)   269804 2022-04-25 10:20:41.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_drift_annotations_3.json
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)   252424 2022-04-25 10:20:41.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_drift_annotations_4.json
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)   264277 2022-04-25 10:20:41.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_drift_annotations_5.json
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)   257575 2022-04-25 10:20:41.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_drift_annotations_6.json
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)   850981 2022-08-01 08:55:15.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_drift_measurement_0.json
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)   887827 2022-08-01 08:55:15.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_drift_measurement_1.json
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)   890707 2022-08-01 08:55:15.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_drift_measurement_2.json
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)   931261 2022-08-01 08:55:15.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_drift_measurement_3.json
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)   860376 2022-08-01 08:55:15.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_drift_measurement_4.json
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)   855285 2022-08-01 08:55:15.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_drift_measurement_5.json
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)   860041 2022-08-01 08:55:15.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_drift_measurement_6.json
--rw-r--r--   0 prateekgoyal   (501) staff       (20)     5327 2022-09-01 10:07:13.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_explanations.json
--rw-r--r--   0 prateekgoyal   (501) staff       (20)  1152715 2022-08-26 05:34:41.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_fairness.json
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)  1432534 2022-08-01 08:55:15.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_manual_labeling.json
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)  5209548 2022-08-01 08:55:15.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_payloads_0.json
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)  5207503 2022-08-01 08:55:15.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_payloads_1.json
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)  5210337 2022-08-01 08:55:15.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_payloads_2.json
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)  5210470 2022-08-01 08:55:15.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_payloads_3.json
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)  5209458 2022-08-01 08:55:15.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_payloads_4.json
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)  5210872 2022-08-01 08:55:15.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_payloads_5.json
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)  5209866 2022-08-01 08:55:15.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_payloads_6.json
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)    15288 2022-08-01 08:55:15.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_performance.json
-drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-01-12 04:03:03.210821 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)     2624 2022-08-01 08:55:15.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/configuration.json
-drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-01-12 04:03:02.941612 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/drift_archives/
-drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-01-12 04:03:02.940062 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/drift_archives/py_3.10/
-drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-01-12 04:03:03.211563 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/drift_archives/py_3.10/scikit_1.0.2/
--rw-r--r--   0 prateekgoyal   (501) staff       (20)   136239 2023-01-10 12:44:29.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/drift_archives/py_3.10/scikit_1.0.2/drift_archive.tar.gz
-drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-01-12 04:03:02.940952 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/drift_archives/py_3.7/
-drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-01-12 04:03:03.213227 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/drift_archives/py_3.7/scikit_0.20.2/
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)   222472 2022-08-01 08:55:15.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/drift_archives/py_3.7/scikit_0.20.2/drift_archive.tar.gz
-drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-01-12 04:03:03.215421 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/drift_archives/py_3.7/scikit_0.24.1/
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)   145596 2022-08-01 08:55:15.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/drift_archives/py_3.7/scikit_0.24.1/drift_archive.tar.gz
-drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-01-12 04:03:03.216795 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/drift_archives/py_3.7/scikit_0.24.2/
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)   145596 2022-08-01 08:55:15.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/drift_archives/py_3.7/scikit_0.24.2/drift_archive.tar.gz
-drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-01-12 04:03:02.941367 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/drift_archives/py_3.8/
-drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-01-12 04:03:03.218622 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/drift_archives/py_3.8/scikit_0.24.1/
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)   136587 2022-08-01 08:55:15.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/drift_archives/py_3.8/scikit_0.24.1/drift_archive.tar.gz
-drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-01-12 04:03:02.942014 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/drift_archives/py_3.9/
-drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-01-12 04:03:03.220349 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/drift_archives/py_3.9/scikit_0.24.1/
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)   136587 2022-08-01 08:55:35.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/drift_archives/py_3.9/scikit_0.24.1/drift_archive.tar.gz
-drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-01-12 04:03:03.221914 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/drift_archives/py_3.9/scikit_1.0.2/
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)   136631 2022-08-01 08:55:35.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/drift_archives/py_3.9/scikit_1.0.2/drift_archive.tar.gz
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)    14275 2022-08-01 08:55:35.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/mrm_evaluation_data.csv
-drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-01-12 04:03:03.225950 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/py_3.10/
--rw-r--r--   0 prateekgoyal   (501) staff       (20)    60883 2023-01-10 12:44:29.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/py_3.10/model_content.gzip
--rw-r--r--   0 prateekgoyal   (501) staff       (20)    13447 2023-01-11 05:32:27.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/py_3.10/model_meta.json
-drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-01-12 04:03:03.228171 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/py_3.7/
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)    61574 2022-08-01 08:55:35.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/py_3.7/model_content.gzip
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)    13626 2022-08-01 08:55:35.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/py_3.7/model_meta.json
-drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-01-12 04:03:03.230403 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/py_3.8/
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)    60715 2022-08-01 08:55:35.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/py_3.8/model_content.gzip
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)    13666 2022-08-01 08:55:35.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/py_3.8/model_meta.json
-drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-01-12 04:03:03.232679 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/py_3.9/
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)    60839 2022-08-01 08:55:35.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/py_3.9/model_content.gzip
--rw-r--r--   0 prateekgoyal   (501) staff       (20)    13629 2023-01-09 12:45:40.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/py_3.9/model_meta.json
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)   689622 2022-08-01 08:55:35.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/training_data.csv
--rw-r--r--   0 prateekgoyal   (501) staff       (20)    31531 2022-12-08 09:39:57.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/training_data_statistics.json
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)    14206 2022-08-01 08:55:35.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm_evaluation_data.csv
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)    13227 2022-08-01 08:55:35.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/scoring_data.csv
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)   688531 2022-08-01 08:55:35.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/training_data.csv
--rw-r--r--   0 prateekgoyal   (501) staff       (20)    28527 2022-12-08 09:39:57.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/training_data_statistics.json
-drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-01-12 04:03:03.235227 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/v3/
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)    37201 2022-08-01 08:55:35.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/v3/model_content.gzip
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)    15506 2022-08-01 08:55:35.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/v3/model_meta.json
-drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-01-12 04:03:02.944312 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/v4/
-drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-01-12 04:03:03.238077 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/v4/spark_2.4/
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)    68724 2022-08-01 08:55:35.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/v4/spark_2.4/model_content.gzip
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)    14847 2022-08-01 08:55:35.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/v4/spark_2.4/model_meta.json
-drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-01-12 04:03:03.240028 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/v4/spark_3.0/
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)    49882 2022-08-04 06:39:13.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/v4/spark_3.0/model_content.gzip
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)    14851 2022-08-01 08:55:35.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/v4/spark_3.0/model_meta.json
-drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-01-12 04:03:03.241618 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/v4/spark_3.2/
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)    34280 2022-08-04 06:39:13.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/v4/spark_3.2/model_content.gzip
--rw-r--r--   0 prateekgoyal   (501) staff       (20)    14851 2023-01-09 11:39:33.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/v4/spark_3.2/model_meta.json
-drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-01-12 04:03:03.243580 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/v4/spark_3.3/
--rw-r--r--   0 prateekgoyal   (501) staff       (20)    34255 2023-01-10 12:44:29.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/v4/spark_3.3/model_content.gzip
--rw-r--r--   0 prateekgoyal   (501) staff       (20)    14703 2023-01-11 05:32:27.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/v4/spark_3.3/model_meta.json
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)    29251 2022-08-01 08:55:50.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/model.py
-drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-01-12 04:03:03.245888 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/openscale/
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)     6445 2022-08-01 08:55:50.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/openscale/openscale.py
--rw-r--r--   0 prateekgoyal   (501) staff       (20)    97618 2023-01-10 12:44:29.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/openscale/openscale_client.py
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)     8518 2022-08-01 08:55:50.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/openscale/openscale_reset.py
--rw-r--r--   0 prateekgoyal   (501) staff       (20)    13125 2022-10-04 09:57:14.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/openscale_ops.py
--rw-r--r--   0 prateekgoyal   (501) staff       (20)     7665 2023-01-10 12:44:29.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/ops.py
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)     2733 2022-08-01 08:55:50.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/reset_ops.py
-drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-01-12 04:03:03.251581 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/setup_classes/
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)    10470 2022-08-01 08:55:50.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/setup_classes/cloud_foundry.py
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)     6938 2022-08-01 08:55:50.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/setup_classes/cloud_foundry_cli.py
--rw-r--r--   0 prateekgoyal   (501) staff       (20)     8766 2023-01-11 05:30:47.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/setup_classes/resource_controller.py
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)     5908 2022-08-01 08:55:50.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/setup_classes/resource_controller_cli.py
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)     1331 2022-08-01 08:55:50.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/setup_classes/setup_ibmcloud_services.py
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)     3647 2022-08-01 08:55:50.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/setup_classes/setup_ibmcloud_services_cli.py
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)     8861 2022-08-01 08:55:50.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/setup_classes/setup_ibmcloud_services_rest.py
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)     3750 2022-08-01 08:55:50.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/setup_classes/setup_ibmcloudprivate_services.py
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)     2880 2022-08-01 08:55:50.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/setup_classes/setup_services.py
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)     6794 2022-08-01 08:55:50.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/setup_classes/token_manager.py
-drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-01-12 04:03:03.254661 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/utility_classes/
--rw-r--r--   0 prateekgoyal   (501) staff       (20)     2812 2023-01-10 12:44:29.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/utility_classes/constants.py
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)     5917 2022-08-01 08:55:50.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/utility_classes/fastpath_logger.py
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)     1517 2022-08-01 08:55:50.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/utility_classes/keras_unstructured_binary_text.py
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)     2794 2022-08-01 08:55:50.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/utility_classes/statistics_generator.py
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)      825 2022-08-01 08:55:50.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/utility_classes/timer.py
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)     5494 2022-08-01 08:55:50.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/utility_classes/utils.py
-drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-01-12 04:03:03.257367 ibm-watson-openscale-cli-tool-3.5.51/ibm_watson_openscale_cli_tool.egg-info/
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)    21142 2023-01-12 04:03:02.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_watson_openscale_cli_tool.egg-info/PKG-INFO
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)    10477 2023-01-12 04:03:02.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_watson_openscale_cli_tool.egg-info/SOURCES.txt
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)        1 2023-01-12 04:03:02.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_watson_openscale_cli_tool.egg-info/dependency_links.txt
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)       76 2023-01-12 04:03:02.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_watson_openscale_cli_tool.egg-info/entry_points.txt
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)      233 2023-01-12 04:03:02.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_watson_openscale_cli_tool.egg-info/requires.txt
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)       21 2023-01-12 04:03:02.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_watson_openscale_cli_tool.egg-info/top_level.txt
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)        1 2021-02-19 08:47:18.000000 ibm-watson-openscale-cli-tool-3.5.51/ibm_watson_openscale_cli_tool.egg-info/zip-safe
--rw-r--r--   0 prateekgoyal   (501) staff       (20)       38 2023-01-12 04:03:03.259520 ibm-watson-openscale-cli-tool-3.5.51/setup.cfg
--rw-r--r--   0 prateekgoyal   (501) staff       (20)     3355 2023-01-10 12:44:29.000000 ibm-watson-openscale-cli-tool-3.5.51/setup.py
+drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-06-09 07:48:08.336154 ibm-watson-openscale-cli-tool-3.5.52/
+-rwxrwxrwx   0 prateekgoyal   (501) staff       (20)    10173 2022-08-01 08:55:50.000000 ibm-watson-openscale-cli-tool-3.5.52/LICENSE
+-rwxrwxrwx   0 prateekgoyal   (501) staff       (20)      215 2022-08-01 08:55:50.000000 ibm-watson-openscale-cli-tool-3.5.52/MANIFEST.in
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)    21142 2023-06-09 07:48:08.335822 ibm-watson-openscale-cli-tool-3.5.52/PKG-INFO
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)    20369 2023-02-10 07:19:55.000000 ibm-watson-openscale-cli-tool-3.5.52/README.md
+drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-06-09 07:48:08.025232 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)        6 2023-02-14 09:40:21.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/VERSION
+-rwxrwxrwx   0 prateekgoyal   (501) staff       (20)     1557 2022-08-01 08:54:52.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/__init__.py
+-rwxrwxrwx   0 prateekgoyal   (501) staff       (20)     4804 2022-08-01 08:54:52.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/api_environment.py
+-rwxrwxrwx   0 prateekgoyal   (501) staff       (20)     4705 2022-08-01 08:54:52.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/credentials.py
+drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-06-09 07:48:08.028072 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/database_classes/
+-rwxrwxrwx   0 prateekgoyal   (501) staff       (20)     4514 2022-08-01 08:54:52.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/database_classes/cos.py
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)    13546 2022-09-26 12:11:09.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/database_classes/db2.py
+-rwxrwxrwx   0 prateekgoyal   (501) staff       (20)     7086 2022-08-01 08:54:52.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/database_classes/postgres.py
+-rwxrwxrwx   0 prateekgoyal   (501) staff       (20)     1078 2022-08-01 08:54:52.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/database_classes/postgres_compose.py
+-rwxrwxrwx   0 prateekgoyal   (501) staff       (20)     1055 2022-08-01 08:54:52.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/database_classes/postgres_icd.py
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)     1288 2023-03-27 07:39:06.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/enums.py
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)     5307 2023-06-08 11:51:19.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/environments.py
+-rwxr-xr-x   0 prateekgoyal   (501) staff       (20)    21871 2023-03-27 07:39:06.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/main.py
+drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-06-09 07:48:08.030716 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/ml_engines/
+-rwxrwxrwx   0 prateekgoyal   (501) staff       (20)     2900 2022-08-01 08:54:52.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/ml_engines/azure_machine_learning.py
+-rwxrwxrwx   0 prateekgoyal   (501) staff       (20)     1875 2022-08-01 08:54:52.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/ml_engines/custom_machine_learning.py
+-rwxrwxrwx   0 prateekgoyal   (501) staff       (20)     2084 2022-08-01 08:54:52.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/ml_engines/sagemaker_machine_learning.py
+-rwxrwxrwx   0 prateekgoyal   (501) staff       (20)     1584 2022-08-01 08:54:52.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/ml_engines/spss_machine_learning.py
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)    25312 2023-05-08 06:59:25.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/ml_engines/watson_machine_learning.py
+drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-06-09 07:48:08.031365 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/
+drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-06-09 07:48:08.044232 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/
+drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-06-09 07:48:08.045834 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/azuremlservice/
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)     2512 2023-03-03 06:16:49.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/azuremlservice/configuration.json
+drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-06-09 07:48:08.047757 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/azuremlstudio/
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)     2512 2023-03-03 06:16:49.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/azuremlstudio/configuration.json
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)   200347 2023-03-03 06:16:49.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/azuremlstudio/history_payloads.json
+drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-06-09 07:48:08.050690 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/custom/
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)     2500 2023-03-03 06:16:49.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/custom/configuration.json
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)   116539 2023-03-03 06:16:49.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/custom/history_payloads.json
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)     7171 2023-03-03 05:56:45.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/feedback_data.csv
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)  1152715 2023-03-03 06:16:49.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/history_fairness.json
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)    90011 2023-03-03 05:56:45.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/history_quality_monitor.json
+drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-06-09 07:48:08.061885 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/sagemaker/
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)     5766 2023-03-03 06:16:49.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/sagemaker/configuration.json
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)     7631 2023-03-03 06:16:49.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/sagemaker/feedback_data.csv
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)   561618 2023-03-03 06:16:49.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/sagemaker/history_fairness.json
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)   107766 2023-03-03 06:16:49.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/sagemaker/history_payloads.json
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)   634377 2023-03-03 06:16:49.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/sagemaker/training_data.csv
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)    24287 2023-03-03 06:16:49.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/sagemaker/training_data_statistics.json
+drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-06-09 07:48:08.063701 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/spss/
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)     2503 2023-03-03 06:16:49.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/spss/configuration.json
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)   337912 2023-03-03 06:16:49.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/spss/history_payloads.json
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)   688531 2023-03-03 06:16:49.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/training_data.csv
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)    31533 2023-03-03 06:16:49.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/training_data_statistics.json
+drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-06-09 07:48:08.255030 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)     6043 2023-03-27 07:39:06.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/configuration.json
+drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-06-09 07:48:08.010409 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/drift_archives/
+drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-06-09 07:48:08.009047 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/drift_archives/spark_2.4_model/
+drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-06-09 07:48:08.256141 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/drift_archives/spark_2.4_model/scikit_0.20.2/
+-rwxrwxrwx   0 prateekgoyal   (501) staff       (20)   224491 2022-08-01 08:54:52.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/drift_archives/spark_2.4_model/scikit_0.20.2/drift_archive.tar.gz
+drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-06-09 07:48:08.258299 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/drift_archives/spark_2.4_model/scikit_0.24.1/
+-rwxrwxrwx   0 prateekgoyal   (501) staff       (20)   166282 2022-08-01 08:54:52.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/drift_archives/spark_2.4_model/scikit_0.24.1/drift_archive.tar.gz
+drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-06-09 07:48:08.259930 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/drift_archives/spark_2.4_model/scikit_0.24.2/
+-rwxrwxrwx   0 prateekgoyal   (501) staff       (20)   166284 2022-08-01 08:54:52.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/drift_archives/spark_2.4_model/scikit_0.24.2/drift_archive.tar.gz
+drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-06-09 07:48:08.009728 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/drift_archives/spark_3.0_model/
+drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-06-09 07:48:08.261777 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/drift_archives/spark_3.0_model/scikit_0.24.1/
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)   121711 2023-02-10 07:19:56.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/drift_archives/spark_3.0_model/scikit_0.24.1/drift_archive.tar.gz
+drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-06-09 07:48:08.263427 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/drift_archives/spark_3.0_model/scikit_1.0.2/
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)   121637 2023-02-10 07:19:56.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/drift_archives/spark_3.0_model/scikit_1.0.2/drift_archive.tar.gz
+drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-06-09 07:48:08.010153 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/drift_archives/spark_3.2_model/
+drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-06-09 07:48:08.264952 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/drift_archives/spark_3.2_model/scikit_1.0.2/
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)   121595 2023-02-10 07:19:56.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/drift_archives/spark_3.2_model/scikit_1.0.2/drift_archive.tar.gz
+drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-06-09 07:48:08.010814 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/drift_archives/spark_3.3_model/
+drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-06-09 07:48:08.266245 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/drift_archives/spark_3.3_model/scikit_1.0.2/
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)   121449 2023-02-10 07:19:56.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/drift_archives/spark_3.3_model/scikit_1.0.2/drift_archive.tar.gz
+drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-06-09 07:48:08.267551 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/drift_archives/spark_3.3_model/scikit_1.1.1/
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)   121445 2023-04-24 13:19:16.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/drift_archives/spark_3.3_model/scikit_1.1.1/drift_archive.tar.gz
+drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-06-09 07:48:08.011501 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/drift_v2_archives/
+drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-06-09 07:48:08.268879 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/drift_v2_archives/4.7/
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)   161371 2023-04-24 12:00:29.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/drift_v2_archives/4.7/baseline.tar.gz
+drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-06-09 07:48:08.270689 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/drift_v2_archives/public_cloud/
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)   161371 2023-04-24 12:00:29.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/drift_v2_archives/public_cloud/baseline.tar.gz
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)   320533 2023-04-28 09:23:48.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/drift_v2_history_measurements_payload_per_run.json
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)   377407 2023-04-28 09:23:48.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/drift_v2_insights_record_payloads.json
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)   221506 2023-04-28 09:23:48.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/drift_v2_intervals_record_payloads.json
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)   196012 2023-04-28 09:23:48.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/drift_v2_stats_baseline_record_payloads.json
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)  1200592 2023-04-28 09:23:48.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/drift_v2_stats_production_record_payloads.json
+-rwxrwxrwx   0 prateekgoyal   (501) staff       (20)    14206 2022-08-01 08:55:15.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/feedback_data.csv
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)   710154 2022-08-26 05:34:41.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_debias.json
+-rwxrwxrwx   0 prateekgoyal   (501) staff       (20)   537110 2022-08-01 08:55:15.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_debiased_payloads_0.json
+-rwxrwxrwx   0 prateekgoyal   (501) staff       (20)   536973 2022-08-01 08:55:15.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_debiased_payloads_1.json
+-rwxrwxrwx   0 prateekgoyal   (501) staff       (20)   537385 2022-08-01 08:55:15.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_debiased_payloads_2.json
+-rwxrwxrwx   0 prateekgoyal   (501) staff       (20)   537039 2022-08-01 08:55:15.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_debiased_payloads_3.json
+-rwxrwxrwx   0 prateekgoyal   (501) staff       (20)   537121 2022-08-01 08:55:15.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_debiased_payloads_4.json
+-rwxrwxrwx   0 prateekgoyal   (501) staff       (20)   537075 2022-08-01 08:55:15.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_debiased_payloads_5.json
+-rwxrwxrwx   0 prateekgoyal   (501) staff       (20)   537028 2022-08-01 08:55:15.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_debiased_payloads_6.json
+-rwxrwxrwx   0 prateekgoyal   (501) staff       (20)   241414 2022-04-25 10:20:41.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_drift_annotations_0.json
+-rwxrwxrwx   0 prateekgoyal   (501) staff       (20)   271060 2022-04-25 10:20:41.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_drift_annotations_1.json
+-rwxrwxrwx   0 prateekgoyal   (501) staff       (20)   278958 2022-04-25 10:20:41.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_drift_annotations_2.json
+-rwxrwxrwx   0 prateekgoyal   (501) staff       (20)   269804 2022-04-25 10:20:41.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_drift_annotations_3.json
+-rwxrwxrwx   0 prateekgoyal   (501) staff       (20)   252424 2022-04-25 10:20:41.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_drift_annotations_4.json
+-rwxrwxrwx   0 prateekgoyal   (501) staff       (20)   264277 2022-04-25 10:20:41.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_drift_annotations_5.json
+-rwxrwxrwx   0 prateekgoyal   (501) staff       (20)   257575 2022-04-25 10:20:41.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_drift_annotations_6.json
+-rwxrwxrwx   0 prateekgoyal   (501) staff       (20)   850981 2022-08-01 08:55:15.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_drift_measurement_0.json
+-rwxrwxrwx   0 prateekgoyal   (501) staff       (20)   887827 2022-08-01 08:55:15.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_drift_measurement_1.json
+-rwxrwxrwx   0 prateekgoyal   (501) staff       (20)   890707 2022-08-01 08:55:15.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_drift_measurement_2.json
+-rwxrwxrwx   0 prateekgoyal   (501) staff       (20)   931261 2022-08-01 08:55:15.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_drift_measurement_3.json
+-rwxrwxrwx   0 prateekgoyal   (501) staff       (20)   860376 2022-08-01 08:55:15.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_drift_measurement_4.json
+-rwxrwxrwx   0 prateekgoyal   (501) staff       (20)   855285 2022-08-01 08:55:15.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_drift_measurement_5.json
+-rwxrwxrwx   0 prateekgoyal   (501) staff       (20)   860041 2022-08-01 08:55:15.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_drift_measurement_6.json
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)     5327 2023-02-10 07:19:56.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_explanations.json
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)  1152715 2022-08-26 05:34:41.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_fairness.json
+-rwxrwxrwx   0 prateekgoyal   (501) staff       (20)  1432534 2022-08-01 08:55:15.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_manual_labeling.json
+-rwxrwxrwx   0 prateekgoyal   (501) staff       (20)  5209548 2022-08-01 08:55:15.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_payloads_0.json
+-rwxrwxrwx   0 prateekgoyal   (501) staff       (20)  5207503 2022-08-01 08:55:15.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_payloads_1.json
+-rwxrwxrwx   0 prateekgoyal   (501) staff       (20)  5210337 2022-08-01 08:55:15.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_payloads_2.json
+-rwxrwxrwx   0 prateekgoyal   (501) staff       (20)  5210470 2022-08-01 08:55:15.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_payloads_3.json
+-rwxrwxrwx   0 prateekgoyal   (501) staff       (20)  5209458 2022-08-01 08:55:15.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_payloads_4.json
+-rwxrwxrwx   0 prateekgoyal   (501) staff       (20)  5210872 2022-08-01 08:55:15.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_payloads_5.json
+-rwxrwxrwx   0 prateekgoyal   (501) staff       (20)  5209866 2022-08-01 08:55:15.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_payloads_6.json
+-rwxrwxrwx   0 prateekgoyal   (501) staff       (20)    15288 2022-08-01 08:55:15.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_performance.json
+drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-06-09 07:48:08.275859 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/
+drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-06-09 07:48:08.277913 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/4.7/
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)    60889 2023-04-24 13:19:16.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/4.7/model_content.gzip
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)    13447 2023-04-24 13:19:16.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/4.7/model_meta.json
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)     2751 2023-03-27 07:39:06.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/configuration.json
+drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-06-09 07:48:08.014581 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/drift_archives/
+drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-06-09 07:48:08.012556 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/drift_archives/4.7/
+drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-06-09 07:48:08.278518 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/drift_archives/4.7/scikit_1.1.1/
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)   137080 2023-04-24 13:19:16.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/drift_archives/4.7/scikit_1.1.1/drift_archive.tar.gz
+drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-06-09 07:48:08.012974 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/drift_archives/py_3.10/
+drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-06-09 07:48:08.279931 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/drift_archives/py_3.10/scikit_1.0.2/
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)   136239 2023-02-10 07:19:56.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/drift_archives/py_3.10/scikit_1.0.2/drift_archive.tar.gz
+drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-06-09 07:48:08.013902 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/drift_archives/py_3.7/
+drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-06-09 07:48:08.282417 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/drift_archives/py_3.7/scikit_0.20.2/
+-rwxrwxrwx   0 prateekgoyal   (501) staff       (20)   222472 2022-08-01 08:55:15.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/drift_archives/py_3.7/scikit_0.20.2/drift_archive.tar.gz
+drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-06-09 07:48:08.284856 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/drift_archives/py_3.7/scikit_0.24.1/
+-rwxrwxrwx   0 prateekgoyal   (501) staff       (20)   145596 2022-08-01 08:55:15.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/drift_archives/py_3.7/scikit_0.24.1/drift_archive.tar.gz
+drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-06-09 07:48:08.286072 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/drift_archives/py_3.7/scikit_0.24.2/
+-rwxrwxrwx   0 prateekgoyal   (501) staff       (20)   145596 2022-08-01 08:55:15.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/drift_archives/py_3.7/scikit_0.24.2/drift_archive.tar.gz
+drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-06-09 07:48:08.014323 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/drift_archives/py_3.8/
+drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-06-09 07:48:08.287516 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/drift_archives/py_3.8/scikit_0.24.1/
+-rwxrwxrwx   0 prateekgoyal   (501) staff       (20)   136587 2022-08-01 08:55:15.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/drift_archives/py_3.8/scikit_0.24.1/drift_archive.tar.gz
+drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-06-09 07:48:08.014994 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/drift_archives/py_3.9/
+drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-06-09 07:48:08.289236 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/drift_archives/py_3.9/scikit_0.24.1/
+-rwxrwxrwx   0 prateekgoyal   (501) staff       (20)   136587 2022-08-01 08:55:35.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/drift_archives/py_3.9/scikit_0.24.1/drift_archive.tar.gz
+drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-06-09 07:48:08.290774 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/drift_archives/py_3.9/scikit_1.0.2/
+-rwxrwxrwx   0 prateekgoyal   (501) staff       (20)   136631 2022-08-01 08:55:35.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/drift_archives/py_3.9/scikit_1.0.2/drift_archive.tar.gz
+drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-06-09 07:48:08.015671 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/drift_v2_archives/
+drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-06-09 07:48:08.292468 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/drift_v2_archives/4.7/
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)   158866 2023-04-24 12:00:29.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/drift_v2_archives/4.7/baseline.tar.gz
+drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-06-09 07:48:08.294690 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/drift_v2_archives/public_cloud/
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)   158866 2023-04-24 12:00:29.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/drift_v2_archives/public_cloud/baseline.tar.gz
+-rwxrwxrwx   0 prateekgoyal   (501) staff       (20)    14275 2022-08-01 08:55:35.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/mrm_evaluation_data.csv
+drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-06-09 07:48:08.298327 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/py_3.10/
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)    60883 2023-04-20 13:09:42.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/py_3.10/model_content.gzip
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)    13447 2023-04-20 13:09:42.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/py_3.10/model_meta.json
+drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-06-09 07:48:08.300216 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/py_3.7/
+-rwxrwxrwx   0 prateekgoyal   (501) staff       (20)    61574 2022-08-01 08:55:35.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/py_3.7/model_content.gzip
+-rwxrwxrwx   0 prateekgoyal   (501) staff       (20)    13626 2022-08-01 08:55:35.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/py_3.7/model_meta.json
+drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-06-09 07:48:08.302187 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/py_3.8/
+-rwxrwxrwx   0 prateekgoyal   (501) staff       (20)    60715 2022-08-01 08:55:35.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/py_3.8/model_content.gzip
+-rwxrwxrwx   0 prateekgoyal   (501) staff       (20)    13666 2022-08-01 08:55:35.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/py_3.8/model_meta.json
+drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-06-09 07:48:08.303501 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/py_3.9/
+-rwxrwxrwx   0 prateekgoyal   (501) staff       (20)    60839 2022-08-01 08:55:35.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/py_3.9/model_content.gzip
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)    13629 2023-02-10 07:19:56.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/py_3.9/model_meta.json
+-rwxrwxrwx   0 prateekgoyal   (501) staff       (20)   689622 2022-08-01 08:55:35.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/training_data.csv
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)    31531 2022-12-08 09:39:57.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/training_data_statistics.json
+-rwxrwxrwx   0 prateekgoyal   (501) staff       (20)    14206 2022-08-01 08:55:35.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm_evaluation_data.csv
+-rwxrwxrwx   0 prateekgoyal   (501) staff       (20)    13227 2022-08-01 08:55:35.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/scoring_data.csv
+-rwxrwxrwx   0 prateekgoyal   (501) staff       (20)   688531 2022-08-01 08:55:35.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/training_data.csv
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)    28527 2022-12-08 09:39:57.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/training_data_statistics.json
+drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-06-09 07:48:08.304826 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/v3/
+-rwxrwxrwx   0 prateekgoyal   (501) staff       (20)    37201 2022-08-01 08:55:35.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/v3/model_content.gzip
+-rwxrwxrwx   0 prateekgoyal   (501) staff       (20)    15506 2022-08-01 08:55:35.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/v3/model_meta.json
+drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-06-09 07:48:08.018025 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/v4/
+drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-06-09 07:48:08.307099 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/v4/spark_2.4/
+-rwxrwxrwx   0 prateekgoyal   (501) staff       (20)    68724 2022-08-01 08:55:35.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/v4/spark_2.4/model_content.gzip
+-rwxrwxrwx   0 prateekgoyal   (501) staff       (20)    14847 2022-08-01 08:55:35.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/v4/spark_2.4/model_meta.json
+drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-06-09 07:48:08.309016 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/v4/spark_3.0/
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)    49882 2023-02-10 07:19:56.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/v4/spark_3.0/model_content.gzip
+-rwxrwxrwx   0 prateekgoyal   (501) staff       (20)    14851 2022-08-01 08:55:35.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/v4/spark_3.0/model_meta.json
+drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-06-09 07:48:08.310671 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/v4/spark_3.2/
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)    34280 2023-02-10 07:19:56.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/v4/spark_3.2/model_content.gzip
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)    14851 2023-02-10 07:19:56.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/v4/spark_3.2/model_meta.json
+drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-06-09 07:48:08.312238 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/v4/spark_3.3/
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)    34778 2023-04-24 13:19:16.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/v4/spark_3.3/model_content.gzip
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)    14703 2023-02-10 07:19:56.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/v4/spark_3.3/model_meta.json
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)    32844 2023-05-08 06:59:25.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/model.py
+drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-06-09 07:48:08.315596 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/openscale/
+-rwxrwxrwx   0 prateekgoyal   (501) staff       (20)     6445 2023-02-07 10:22:14.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/openscale/openscale.py
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)   111910 2023-05-24 11:48:09.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/openscale/openscale_client.py
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)     8653 2023-02-17 11:22:39.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/openscale/openscale_reset.py
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)    13267 2023-05-05 04:10:00.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/openscale_ops.py
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)     7791 2023-03-27 07:39:06.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/ops.py
+-rwxrwxrwx   0 prateekgoyal   (501) staff       (20)     2733 2022-08-01 08:55:50.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/reset_ops.py
+drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-06-09 07:48:08.321539 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/setup_classes/
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)    10509 2023-02-17 11:22:39.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/setup_classes/cloud_foundry.py
+-rwxrwxrwx   0 prateekgoyal   (501) staff       (20)     6938 2022-08-01 08:55:50.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/setup_classes/cloud_foundry_cli.py
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)     8801 2023-02-17 11:22:39.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/setup_classes/resource_controller.py
+-rwxrwxrwx   0 prateekgoyal   (501) staff       (20)     5908 2022-08-01 08:55:50.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/setup_classes/resource_controller_cli.py
+-rwxrwxrwx   0 prateekgoyal   (501) staff       (20)     1331 2022-08-01 08:55:50.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/setup_classes/setup_ibmcloud_services.py
+-rwxrwxrwx   0 prateekgoyal   (501) staff       (20)     3647 2022-08-01 08:55:50.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/setup_classes/setup_ibmcloud_services_cli.py
+-rwxrwxrwx   0 prateekgoyal   (501) staff       (20)     8861 2022-08-01 08:55:50.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/setup_classes/setup_ibmcloud_services_rest.py
+-rwxrwxrwx   0 prateekgoyal   (501) staff       (20)     3750 2022-08-01 08:55:50.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/setup_classes/setup_ibmcloudprivate_services.py
+-rwxrwxrwx   0 prateekgoyal   (501) staff       (20)     2880 2022-08-01 08:55:50.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/setup_classes/setup_services.py
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)     6829 2023-02-14 09:40:21.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/setup_classes/token_manager.py
+drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-06-09 07:48:08.324808 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/utility_classes/
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)     4333 2023-05-24 11:48:09.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/utility_classes/constants.py
+-rwxrwxrwx   0 prateekgoyal   (501) staff       (20)     5917 2022-08-01 08:55:50.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/utility_classes/fastpath_logger.py
+-rwxrwxrwx   0 prateekgoyal   (501) staff       (20)     1517 2022-08-01 08:55:50.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/utility_classes/keras_unstructured_binary_text.py
+-rwxrwxrwx   0 prateekgoyal   (501) staff       (20)     2794 2022-08-01 08:55:50.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/utility_classes/statistics_generator.py
+-rwxrwxrwx   0 prateekgoyal   (501) staff       (20)      825 2022-08-01 08:55:50.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/utility_classes/timer.py
+-rwxrwxrwx   0 prateekgoyal   (501) staff       (20)     5494 2022-08-01 08:55:50.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/utility_classes/utils.py
+drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-06-09 07:48:08.328152 ibm-watson-openscale-cli-tool-3.5.52/ibm_watson_openscale_cli_tool.egg-info/
+-rwxrwxrwx   0 prateekgoyal   (501) staff       (20)    21142 2023-06-09 07:48:07.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_watson_openscale_cli_tool.egg-info/PKG-INFO
+-rwxrwxrwx   0 prateekgoyal   (501) staff       (20)    12112 2023-06-09 07:48:07.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_watson_openscale_cli_tool.egg-info/SOURCES.txt
+-rwxrwxrwx   0 prateekgoyal   (501) staff       (20)        1 2023-06-09 07:48:07.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_watson_openscale_cli_tool.egg-info/dependency_links.txt
+-rwxrwxrwx   0 prateekgoyal   (501) staff       (20)       76 2023-06-09 07:48:07.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_watson_openscale_cli_tool.egg-info/entry_points.txt
+-rwxrwxrwx   0 prateekgoyal   (501) staff       (20)      229 2023-06-09 07:48:07.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_watson_openscale_cli_tool.egg-info/requires.txt
+-rwxrwxrwx   0 prateekgoyal   (501) staff       (20)       21 2023-06-09 07:48:07.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_watson_openscale_cli_tool.egg-info/top_level.txt
+-rwxrwxrwx   0 prateekgoyal   (501) staff       (20)        1 2021-02-19 08:47:18.000000 ibm-watson-openscale-cli-tool-3.5.52/ibm_watson_openscale_cli_tool.egg-info/zip-safe
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)       38 2023-06-09 07:48:08.336263 ibm-watson-openscale-cli-tool-3.5.52/setup.cfg
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)     3350 2023-05-24 11:48:09.000000 ibm-watson-openscale-cli-tool-3.5.52/setup.py
+drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-06-09 07:48:08.334954 ibm-watson-openscale-cli-tool-3.5.52/tests/
+-rwxrwxrwx   0 prateekgoyal   (501) staff       (20)    12683 2022-08-01 08:55:50.000000 ibm-watson-openscale-cli-tool-3.5.52/tests/test_cloud_foundry.py
+-rwxrwxrwx   0 prateekgoyal   (501) staff       (20)     2984 2022-08-01 08:55:50.000000 ibm-watson-openscale-cli-tool-3.5.52/tests/test_db2.py
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)     1792 2023-02-17 11:22:39.000000 ibm-watson-openscale-cli-tool-3.5.52/tests/test_openscale.py
+-rwxrwxrwx   0 prateekgoyal   (501) staff       (20)     4229 2022-08-01 08:55:50.000000 ibm-watson-openscale-cli-tool-3.5.52/tests/test_postgres.py
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)    10808 2023-02-17 11:22:39.000000 ibm-watson-openscale-cli-tool-3.5.52/tests/test_resource_controller.py
+-rwxrwxrwx   0 prateekgoyal   (501) staff       (20)        0 2022-08-01 08:55:50.000000 ibm-watson-openscale-cli-tool-3.5.52/tests/test_set_up.py
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)     1434 2023-02-17 11:22:39.000000 ibm-watson-openscale-cli-tool-3.5.52/tests/test_setup_ibmcloud_services.py
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)     9611 2023-02-17 11:22:39.000000 ibm-watson-openscale-cli-tool-3.5.52/tests/test_setup_ibmcloud_services_rest.py
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)     1653 2023-02-17 11:22:39.000000 ibm-watson-openscale-cli-tool-3.5.52/tests/test_setup_ibmcloudprivate_services.py
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)     5170 2023-02-17 11:22:39.000000 ibm-watson-openscale-cli-tool-3.5.52/tests/test_token_manager.py
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)     1744 2023-02-17 11:22:39.000000 ibm-watson-openscale-cli-tool-3.5.52/tests/test_utils.py
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)     8285 2023-02-10 07:19:56.000000 ibm-watson-openscale-cli-tool-3.5.52/tests/test_watson_machine_learning.py
```

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/LICENSE` & `ibm-watson-openscale-cli-tool-3.5.52/LICENSE`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/PKG-INFO` & `ibm-watson-openscale-cli-tool-3.5.52/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibm-watson-openscale-cli-tool
-Version: 3.5.51
+Version: 3.5.52
 Summary: CLI library to automate the onboarding process to IBM Watson OpenScale
 Home-page: https://www.ibm.com/cloud/watson-openscale
 Author: IBM Corp
 Author-email: wps@us.ibm.com
 License: Apache-2.0
 Keywords: ai-openscale,ibm-watson
 Classifier: Programming Language :: Python
```

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/README.md` & `ibm-watson-openscale-cli-tool-3.5.52/README.md`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/__init__.py` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/api_environment.py` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/api_environment.py`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/credentials.py` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/credentials.py`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/database_classes/cos.py` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/database_classes/cos.py`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/database_classes/db2.py` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/database_classes/db2.py`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/database_classes/postgres.py` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/database_classes/postgres.py`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/database_classes/postgres_compose.py` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/database_classes/postgres_compose.py`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/database_classes/postgres_icd.py` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/database_classes/postgres_icd.py`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/enums.py` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/enums.py`

 * *Files 9% similar despite different names*

```diff
@@ -32,8 +32,9 @@
     CPD_3_X = "cpd_3.x"
     CPD_4_0_0 = "cpd_4.0.0"
     CPD_4_0_1 = "cpd_4.0.1"
     CPD_4_0_2_PLUS = "cpd_4.0.2+"
     CPD_4_0_8_PLUS = "cpd_4.0.8+"
     CPD_4_5 = "cpd_4.5"
     CPD_4_5_1_PLUS = "cpd_4.5.1+"
-    CPD_4_5_3_PLUS = "cpd_4.5.3+"
+    CPD_4_5_3_PLUS = "cpd_4.5.3+"
+    CPD_4_7_PLUS = "cpd_4.7+"
```

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/environments.py` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/environments.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,15 @@
         attributes['api'] = 'https://api.ng.bluemix.net'
         attributes['aios_url'] = 'https://api.aiopenscale.test.cloud.ibm.com'
         attributes['iam_url'] = 'https://iam.cloud.ibm.com/identity/token'
         attributes['uaa_url'] = 'https://login.ng.bluemix.net/UAALoginServerWAR/oauth/token'
         attributes['resource_controller_url'] = 'https://resource-controller.cloud.ibm.com'
         attributes['resource_group_url'] = 'https://resource-controller.cloud.ibm.com'
         attributes['cos_url'] = 'https://s3.us.cloud-object-storage.appdomain.cloud'
-        attributes['wml_v4_url'] = 'https://us-south.ml.cloud.ibm.com'
+        attributes['wml_v4_url'] = 'https://yp-qa.ml.cloud.ibm.com'
         return attributes
 
     def _getYPCREnv(self):
         attributes = {}
         attributes['name'] = 'YPCR'
         attributes['api'] = 'https://api.ng.bluemix.net'
         attributes['aios_url'] = 'https://aios-yp-cr.us-south.containers.appdomain.cloud'
```

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/main.py` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,14 +130,15 @@
     parser.add_argument('--organization', help=argparse.SUPPRESS, required=False)
     parser.add_argument('--space', help=argparse.SUPPRESS, required=False)
     parser.add_argument('--summary', action='store_true', help=argparse.SUPPRESS, required=False)  # Generate and print a report of failed metric checks
     parser.add_argument('--database-counts', action='store_true', help=argparse.SUPPRESS, required=False)  # Display counts of all the datamart tables at key points
     parser.add_argument('--timers', action='store_true', help=argparse.SUPPRESS, required=False)  # Display TIMERs to STDOUT, not just log
     parser.add_argument('--subscription-details', action='store_true', help=argparse.SUPPRESS, required=False)  #  save subscription details
     parser.add_argument("--is-zlinux", action="store_true", help=argparse.SUPPRESS, required=False, default=False)
+    parser.add_argument("--drift-v2", action="store_true", help=argparse.SUPPRESS, required=False, default=False)
 
     parser._action_groups.append(optional_args)
     return parser
 
 
 def log_error_raise_exception(error_msg):
     logger.log_error(error_msg)
```

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/ml_engines/azure_machine_learning.py` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/ml_engines/azure_machine_learning.py`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/ml_engines/custom_machine_learning.py` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/ml_engines/custom_machine_learning.py`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/ml_engines/sagemaker_machine_learning.py` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/ml_engines/sagemaker_machine_learning.py`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/ml_engines/spss_machine_learning.py` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/ml_engines/spss_machine_learning.py`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/ml_engines/watson_machine_learning.py` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/ml_engines/watson_machine_learning.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 # The source code for this program is not published or other-wise divested of its trade 
 # secrets, irrespective of what has been deposited with the U.S.Copyright Office.
 # ----------------------------------------------------------------------------------------------------
 
 # coding=utf-8
 import time
 
-from retry import retry
+from retrying import retry
 
 from ibm_ai_openscale_cli.utility_classes.fastpath_logger import FastpathLogger
 from ibm_ai_openscale_cli.utility_classes.utils import jsonFileToDict
 from ibm_watson_machine_learning import APIClient
 from ibm_watson_machine_learning.wml_client_error import ApiRequestFailure
-from ibm_ai_openscale_cli.utility_classes.constants import WML_CHALLENGER_SOFTWARE_SPEC_MAPPING
+from ibm_ai_openscale_cli.utility_classes.constants import WML_CHALLENGER_SOFTWARE_SPEC_MAPPING, WML_CHALLENGER_SOFTWARE_SPEC_MAPPING_ZLINUX
 
 logger = FastpathLogger(__name__)
 
 
 class WatsonMachineLearningEngine:
 
     def __init__(self, credentials, openscale_client, cos_credentials=None, is_v4=False, is_mrm=False, is_icp=False, is_zlinux=False):
@@ -41,15 +41,15 @@
 
     def get_native_client(self):
         return self._client
 
     def set_model(self, model):
         self._model_metadata = model.metadata
 
-    @retry(tries=5, delay=4, backoff=2)
+    @retry(stop_max_attempt_number=5, wait_exponential_multiplier=4000)
     def _reliable_create_space(self, space_name):
         logger.log_debug('Creating space {} ...'.format(space_name))
         start = time.time()
         space_props = None
         if not self._is_icp:
             space_props = {
                     self._client.spaces.ConfigurationMetaNames.NAME: space_name,
@@ -78,15 +78,15 @@
                 if state == "error":
                     raise Exception("Space creation failed with error. Status: {}".format(details["entity"]["status"]))
         elapsed = time.time() - start
         self._openscale_client.timer('WML create space completed', elapsed)
         logger.log_debug('Succesfully created space {} (id: {})'.format(space_name, space_id))
         return space_id
 
-    @retry(tries=5, delay=4, backoff=2)
+    @retry(stop_max_attempt_number=5, wait_exponential_multiplier=4000)
     def _reliable_set_space(self, space_id, space_name):
         start = time.time()
         rc = self._client.set.default_space(space_id)
         elapsed = time.time() - start
         if not rc == 'SUCCESS':
             error_msg = 'ERROR: WML set.default_space failed for space {} (id: {}) {}'.format(space_name, space_id, rc)
             logger.log_error(error_msg)
@@ -176,15 +176,15 @@
                     self._reliable_delete_model(model_guid)
                     logger.log_info('Model deleted successfully')
                 except Exception as e:
                     logger.log_warning('Error deleting WML deployment "{}": {}'.format(model_guid, str(e)))
         if not found_model:
             logger.log_info('No existing model found with name: {}'.format(model_name))
 
-    @retry(tries=2, delay=2, backoff=2)
+    @retry(stop_max_attempt_number=2, wait_exponential_multiplier=2000)
     def _reliable_delete_model(self, model_guid):
         all_models = self._client.repository.get_model_details()
         all_functions = self._client.repository.get_function_details()
         for model in (all_models['resources'] + all_functions['resources']):
             if self._is_v4:
                 artifact_model_id = model['metadata']['id']
             else:
@@ -207,15 +207,18 @@
         model_props = {
             self._client.repository.ModelMetaNames.NAME: model_name
         }
         if self._is_v4:
             fw = metadata['framework']
             software_spec_uid = None
             if fw["name"] == "scikit-learn":
-                fw_runtime_uid = WML_CHALLENGER_SOFTWARE_SPEC_MAPPING[self._openscale_client._args.environment]
+                if self._is_zlinux:
+                    fw_runtime_uid = WML_CHALLENGER_SOFTWARE_SPEC_MAPPING_ZLINUX[self._openscale_client._args.environment]
+                else:
+                    fw_runtime_uid = WML_CHALLENGER_SOFTWARE_SPEC_MAPPING[self._openscale_client._args.environment]
             else:
                 fw_runtime_uid = '{}-{}_{}'.format(fw['runtimes'][0]['name'], fw['name'], fw['runtimes'][0]['version'])
 
             software_spec_uid = self._client.software_specifications.get_uid_by_name(fw_runtime_uid)
             model_props[self._client.repository.ModelMetaNames.SOFTWARE_SPEC_UID] = software_spec_uid
             fw_type = '{}_{}'.format(fw['name'], fw['version'])
             model_props[self._client.repository.ModelMetaNames.TYPE] = fw_type
@@ -271,15 +274,15 @@
             model_guid = self._client.repository.get_model_id(model_details)
         logger.log_info('Created new model {} successfully (guid: {})'.format(model_name, model_guid))
         model_url = '{}{}?space_id={}&version=2020-06-22'.format(self._credentials['url'],
                                                                  self._client._models.get_href(model_details),
                                                                  self.space_id)
         return metadata, model_guid, model_url
 
-    @retry(tries=5, delay=4, backoff=2)
+    @retry(stop_max_attempt_number=5, wait_exponential_multiplier=4000)
     def _reliable_create_model(self, model_file, model_props):
         start = time.time()
         try:
             if "type" in model_props and model_props["type"] == "python":
                 model_details = self._client.repository.store_function(model_file, model_props)
             else:
                 model_details = self._client.repository.store_model(model_file, model_props)
@@ -311,15 +314,15 @@
         elapsed_time, deployment_details = self._reliable_deploy_model(model_guid, deployment_name, deployment_description)
         if self._is_v4:
             deployment_guid = deployment_details['metadata']['id']
         deployment_url = deployment_details["entity"]["status"]["serving_urls"][0] if "serving_urls" in deployment_details["entity"]["status"] else deployment_details["entity"]["status"]["online_url"]["url"]
         logger.log_info('Created new deployment {} (guid: {}) successfully in {} seconds'.format(deployment_name, deployment_guid, round(elapsed_time, 2)))
         return deployment_guid, deployment_url
 
-    @retry(tries=5, delay=4, backoff=2)
+    @retry(stop_max_attempt_number=5, wait_exponential_multiplier=4000)
     def _reliable_deploy_model(self, model_guid, deployment_name, deployment_description):
         start = time.time()
         deployment_details = None
         if self._is_v4:
             meta_props = {
                 self._client.deployments.ConfigurationMetaNames.NAME: deployment_name,
                 self._client.deployments.ConfigurationMetaNames.DESCRIPTION: deployment_description,
@@ -328,15 +331,15 @@
             deployment_details = self._client.deployments.create(artifact_uid=model_guid, meta_props=meta_props)
         else:
             deployment_details = self._client.deployments.create(artifact_uid=model_guid, name=deployment_name, description=deployment_description)
         elapsed = time.time() - start
         self._openscale_client.timer('WML deployments.create', elapsed)
         return elapsed, deployment_details
 
-    @retry(tries=5, delay=4, backoff=2)
+    @retry(stop_max_attempt_number=5, wait_exponential_multiplier=4000)
     def _reliable_delete_deployment(self, deployment_guid):
         all_deployments = self._client.deployments.get_details()
         for deployment in all_deployments['resources']:
             if self._is_v4:
                 artifact_deployment_id = deployment['metadata']['id']
             else:
                 artifact_deployment_id = deployment['metadata']['guid']
```

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/azuremlservice/configuration.json` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/azuremlservice/configuration.json`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/azuremlstudio/configuration.json` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/azuremlstudio/configuration.json`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/azuremlstudio/history_payloads.json` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/azuremlstudio/history_payloads.json`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/custom/configuration.json` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/custom/configuration.json`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/custom/history_payloads.json` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/custom/history_payloads.json`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/feedback_data.csv` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/feedback_data.csv`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/history_fairness.json` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/history_fairness.json`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/history_quality_monitor.json` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/history_quality_monitor.json`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/sagemaker/configuration.json` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/sagemaker/configuration.json`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/sagemaker/feedback_data.csv` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/sagemaker/feedback_data.csv`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/sagemaker/history_fairness.json` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/sagemaker/history_fairness.json`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/sagemaker/history_payloads.json` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/sagemaker/history_payloads.json`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/sagemaker/training_data.csv` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/sagemaker/training_data.csv`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/sagemaker/training_data_statistics.json` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/sagemaker/training_data_statistics.json`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/spss/configuration.json` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/spss/configuration.json`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/spss/history_payloads.json` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/spss/history_payloads.json`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/training_data.csv` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/training_data.csv`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/training_data_statistics.json` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/training_data_statistics.json`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/configuration.json` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/configuration.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.875%*

 * *Differences: {"'drift_v2_configuration'": "OrderedDict([('max_samples', 1000), ('min_samples', 100), "*

 * *                             "('train_archive', False)])"}*

```diff
@@ -137,14 +137,19 @@
             ]
         }
     },
     "drift_configuration": {
         "min_records": 100,
         "threshold": 0.05
     },
+    "drift_v2_configuration": {
+        "max_samples": 1000,
+        "min_samples": 100,
+        "train_archive": false
+    },
     "fairness_configuration": {
         "favourable_classes": [
             "No Risk"
         ],
         "features": [
             {
                 "feature": "Age",
```

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/drift_archives/spark_2.4_model/scikit_0.20.2/drift_archive.tar.gz` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/drift_archives/spark_2.4_model/scikit_0.20.2/drift_archive.tar.gz`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/drift_archives/spark_2.4_model/scikit_0.24.1/drift_archive.tar.gz` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/drift_archives/spark_2.4_model/scikit_0.24.1/drift_archive.tar.gz`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/drift_archives/spark_2.4_model/scikit_0.24.2/drift_archive.tar.gz` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/drift_archives/spark_2.4_model/scikit_0.24.2/drift_archive.tar.gz`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/drift_archives/spark_3.0_model/scikit_0.24.1/drift_archive.tar.gz` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/drift_archives/spark_3.0_model/scikit_0.24.1/drift_archive.tar.gz`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/drift_archives/spark_3.0_model/scikit_1.0.2/drift_archive.tar.gz` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/drift_archives/spark_3.0_model/scikit_1.0.2/drift_archive.tar.gz`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/drift_archives/spark_3.2_model/scikit_1.0.2/drift_archive.tar.gz` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/drift_archives/spark_3.2_model/scikit_1.0.2/drift_archive.tar.gz`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/drift_archives/spark_3.3_model/scikit_1.0.2/drift_archive.tar.gz` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/drift_archives/spark_3.3_model/scikit_1.0.2/drift_archive.tar.gz`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/feedback_data.csv` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/feedback_data.csv`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_debias.json` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_debias.json`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_debiased_payloads_0.json` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_debiased_payloads_0.json`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_debiased_payloads_1.json` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_debiased_payloads_1.json`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_debiased_payloads_2.json` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_debiased_payloads_2.json`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_debiased_payloads_3.json` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_debiased_payloads_3.json`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_debiased_payloads_4.json` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_debiased_payloads_4.json`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_debiased_payloads_5.json` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_debiased_payloads_5.json`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_debiased_payloads_6.json` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_debiased_payloads_6.json`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_drift_annotations_0.json` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_drift_annotations_0.json`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_drift_annotations_1.json` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_drift_annotations_1.json`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_drift_annotations_2.json` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_drift_annotations_2.json`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_drift_annotations_3.json` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_drift_annotations_3.json`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_drift_annotations_4.json` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_drift_annotations_4.json`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_drift_annotations_5.json` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_drift_annotations_5.json`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_drift_annotations_6.json` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_drift_annotations_6.json`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_drift_measurement_0.json` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_drift_measurement_0.json`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_drift_measurement_1.json` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_drift_measurement_1.json`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_drift_measurement_2.json` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_drift_measurement_2.json`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_drift_measurement_3.json` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_drift_measurement_3.json`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_drift_measurement_4.json` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_drift_measurement_4.json`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_drift_measurement_5.json` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_drift_measurement_5.json`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_drift_measurement_6.json` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_drift_measurement_6.json`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_explanations.json` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_explanations.json`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_fairness.json` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_fairness.json`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_manual_labeling.json` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_manual_labeling.json`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_payloads_0.json` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_payloads_0.json`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_payloads_1.json` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_payloads_1.json`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_payloads_2.json` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_payloads_2.json`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_payloads_3.json` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_payloads_3.json`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_payloads_4.json` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_payloads_4.json`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_payloads_5.json` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_payloads_5.json`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_payloads_6.json` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_payloads_6.json`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_performance.json` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_performance.json`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/configuration.json` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/configuration.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8571428571428571%*

 * *Differences: {"'drift_v2_configuration'": "OrderedDict([('max_samples', 1000), ('min_samples', 100), "*

 * *                             "('train_archive', False)])"}*

```diff
@@ -43,14 +43,19 @@
         "probability_column": "probability",
         "problem_type": "BINARY_CLASSIFICATION"
     },
     "drift_configuration": {
         "min_records": 100,
         "threshold": 0.05
     },
+    "drift_v2_configuration": {
+        "max_samples": 1000,
+        "min_samples": 100,
+        "train_archive": false
+    },
     "fairness_configuration": {
         "favourable_classes": [
             "No Risk"
         ],
         "features": [
             {
                 "feature": "Age",
```

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/drift_archives/py_3.10/scikit_1.0.2/drift_archive.tar.gz` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/drift_archives/py_3.10/scikit_1.0.2/drift_archive.tar.gz`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/drift_archives/py_3.7/scikit_0.20.2/drift_archive.tar.gz` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/drift_archives/py_3.7/scikit_0.20.2/drift_archive.tar.gz`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/drift_archives/py_3.7/scikit_0.24.1/drift_archive.tar.gz` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/drift_archives/py_3.7/scikit_0.24.1/drift_archive.tar.gz`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/drift_archives/py_3.7/scikit_0.24.2/drift_archive.tar.gz` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/drift_archives/py_3.7/scikit_0.24.2/drift_archive.tar.gz`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/drift_archives/py_3.8/scikit_0.24.1/drift_archive.tar.gz` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/drift_archives/py_3.8/scikit_0.24.1/drift_archive.tar.gz`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/drift_archives/py_3.9/scikit_0.24.1/drift_archive.tar.gz` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/drift_archives/py_3.9/scikit_0.24.1/drift_archive.tar.gz`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/drift_archives/py_3.9/scikit_1.0.2/drift_archive.tar.gz` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/drift_archives/py_3.9/scikit_1.0.2/drift_archive.tar.gz`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/mrm_evaluation_data.csv` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/mrm_evaluation_data.csv`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/py_3.10/model_content.gzip` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/py_3.10/model_content.gzip`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/py_3.10/model_meta.json` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/py_3.10/model_meta.json`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/py_3.7/model_content.gzip` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/py_3.7/model_content.gzip`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/py_3.7/model_meta.json` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/py_3.7/model_meta.json`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/py_3.8/model_content.gzip` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/py_3.8/model_content.gzip`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/py_3.8/model_meta.json` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/py_3.8/model_meta.json`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/py_3.9/model_content.gzip` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/py_3.9/model_content.gzip`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/py_3.9/model_meta.json` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/py_3.9/model_meta.json`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/training_data.csv` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/training_data.csv`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/training_data_statistics.json` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/training_data_statistics.json`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm_evaluation_data.csv` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm_evaluation_data.csv`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/scoring_data.csv` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/scoring_data.csv`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/training_data.csv` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/training_data.csv`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/training_data_statistics.json` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/training_data_statistics.json`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/v3/model_content.gzip` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/v3/model_content.gzip`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/v3/model_meta.json` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/v3/model_meta.json`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/v4/spark_2.4/model_content.gzip` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/v4/spark_2.4/model_content.gzip`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/v4/spark_2.4/model_meta.json` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/v4/spark_2.4/model_meta.json`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/v4/spark_3.0/model_content.gzip` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/v4/spark_3.0/model_content.gzip`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/v4/spark_3.0/model_meta.json` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/v4/spark_3.0/model_meta.json`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/v4/spark_3.2/model_content.gzip` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/v4/spark_3.2/model_content.gzip`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/v4/spark_3.2/model_meta.json` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/v4/spark_3.2/model_meta.json`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/v4/spark_3.3/model_meta.json` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/v4/spark_3.3/model_meta.json`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/models/model.py` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/models/model.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,23 +6,24 @@
 # The source code for this program is not published or other-wise divested of its trade 
 # secrets, irrespective of what has been deposited with the U.S.Copyright Office.
 # ----------------------------------------------------------------------------------------------------
 
 # coding=utf-8
 import datetime
 import json
+import io
 import os
 import random
 import pandas as pd
 from io import StringIO
 from pathlib import Path
 
 from ibm_ai_openscale_cli.database_classes.cos import CloudObjectStorage
 from ibm_ai_openscale_cli.enums import MLEngineType
-from ibm_ai_openscale_cli.utility_classes.constants import WML_CHALLENGER_ENVIRONMENT_MAPPING, WML_SPARK_VERSION_SUPPORT_MAPPING
+from ibm_ai_openscale_cli.utility_classes.constants import WML_CHALLENGER_ENVIRONMENT_MAPPING, WML_CHALLENGER_ENVIRONMENT_MAPPING_ZLINUX, WML_SPARK_VERSION_SUPPORT_MAPPING
 from ibm_ai_openscale_cli.utility_classes.fastpath_logger import FastpathLogger
 from ibm_ai_openscale_cli.utility_classes.keras_unstructured_binary_text import read_lines, split_lines, format_scoring_input
 from ibm_ai_openscale_cli.utility_classes.utils import jsonFileToDict, get_path, load_pickle_file
 
 from ibm_watson_openscale.base_classes.watson_open_scale_v2 import MonitorMeasurementRequest, Source
 from ibm_watson_openscale.supporting_classes.payload_record import PayloadRecord
 
@@ -33,14 +34,15 @@
 
     CONFIGURATION_FILENAME = 'configuration.json'
     MODEL_META_FILENAME = 'model_meta.json'
     MODEL_CONTENT_FILENAME = 'model_content.gzip'
     PIPELINE_META_FILENAME = 'pipeline_meta.json'
     PIPELINE_CONTENT_FILENAME = 'pipeline_content.gzip'
     DRIFT_MODEL_FILENAME = 'drift_archive.tar.gz'
+    DRIFT_V2_ARCHIVE_FILENAME = 'baseline.tar.gz'
     TRAINING_DATA_STATISTICS_FILENAME = 'training_data_statistics.json'
     FAIRNESS_HISTORY_FILENAME = 'history_fairness.json'
     PAYLOAD_HISTORY_FILENAME = 'history_payloads.json'
     TRAINING_DATA_CSV_FILENAME = 'training_data.csv'
     SCORING_DATA_CSV_FILENAME = 'scoring_data.csv'
     FEEDBACK_HISTORY_CSV_FILENAME = 'history_feedback.csv'
     FEEDBACK_CSV_FILENAME = 'feedback_data.csv'
@@ -50,14 +52,19 @@
     QUALITY_MONITOR_HISTORY_FILENAME = 'history_quality_monitor.json'
     MANUAL_LABELING_HISTORY_FILENAME = 'history_manual_labeling.json'
     PERFORMANCE_HISTORY_FILENAME = 'history_performance.json'
     EXPLAIN_HISTORY_FILENAME = 'history_explanations.json'
     DRIFT_ANNOTATIONS_HISTORY_FILENAME = 'history_drift_annotations.json'
     DRIFT_MEASUREMENT_HISTORY_FILENAME = 'history_drift_measurement.json'
     TOKENIZER_PICKLE_FILENAME = 'tokenizer.pickle'
+    DRIFT_V2_HISTORY_MEASUREMENTS_FILENAME = "drift_v2_history_measurements_payload_per_run.json"
+    DRIFT_V2_HISTORY_INSIGHTS_FILENAME = "drift_v2_insights_record_payloads.json"
+    DRIFT_V2_HISTORY_INTERVALS_FILENAME = "drift_v2_intervals_record_payloads.json"
+    DRIFT_V2_HISTORY_STATS_BASELINE_FILENAME = "drift_v2_stats_baseline_record_payloads.json"
+    DRIFT_V2_HISTORY_STATS_PRODUCTION_FILENAME = "drift_v2_stats_production_record_payloads.json"
 
     def __init__(self, name, args, model_instances=1):
         self._args = args
         self.name = name
         if model_instances > 1:
             self.name += str(model_instances)
 
@@ -82,16 +89,20 @@
         
         if "Challenger" not in self.name:
             # Checking for spark version support based on environment
             model_meta_filename = "{}/{}".format(WML_SPARK_VERSION_SUPPORT_MAPPING[self._args.environment], Model.MODEL_META_FILENAME)
             model_content_filename = "{}/{}".format(WML_SPARK_VERSION_SUPPORT_MAPPING[self._args.environment], Model.MODEL_CONTENT_FILENAME)
         else:
             # Checking for Python version support based on environment
-            model_meta_filename = "{}/{}".format(WML_CHALLENGER_ENVIRONMENT_MAPPING[self._args.environment], Model.MODEL_META_FILENAME)
-            model_content_filename = "{}/{}".format(WML_CHALLENGER_ENVIRONMENT_MAPPING[self._args.environment], Model.MODEL_CONTENT_FILENAME)
+            if self._args.is_zlinux:
+                model_meta_filename = "{}/{}".format(WML_CHALLENGER_ENVIRONMENT_MAPPING_ZLINUX[self._args.environment], Model.MODEL_META_FILENAME)
+                model_content_filename = "{}/{}".format(WML_CHALLENGER_ENVIRONMENT_MAPPING_ZLINUX[self._args.environment], Model.MODEL_CONTENT_FILENAME)
+            else:
+                model_meta_filename = "{}/{}".format(WML_CHALLENGER_ENVIRONMENT_MAPPING[self._args.environment], Model.MODEL_META_FILENAME)
+                model_content_filename = "{}/{}".format(WML_CHALLENGER_ENVIRONMENT_MAPPING[self._args.environment], Model.MODEL_CONTENT_FILENAME)
         
         self.metadata['model_metadata_file'] = self._get_file_path(model_meta_filename)
         self.metadata['model_file'] = self._get_file_path(model_content_filename)
         self.metadata['pipeline_metadata_file'] = self._get_file_path(Model.PIPELINE_META_FILENAME)
         self.metadata['pipeline_file'] = self._get_file_path(Model.PIPELINE_CONTENT_FILENAME)
         if self._args.deployment_name: # if this is an existing deployment use the name provided
             self.metadata['deployment_name'] = self._args.deployment_name
@@ -433,14 +444,94 @@
             count = len(resp['values'])
         elif 'Results' in resp and 'output1' in resp['Results']: # payload history format for Azure
             count = len(resp['Results']['output1'])
         elif 'rowValues' in resp: # payload history format for SPSS
             count = len(resp['rowValues'])
         self.historical_payload_row_count += count
         return count
+    
+    def get_drift_v2_history_measurements(self) -> dict:
+        """
+        Gets the `drift_v2` history measurements.
+
+        :returns: The `drift_v2` history measurements.
+        """
+        history_measurements = None
+
+        # Getting the file path
+        file_path = self._get_file_path(Model.DRIFT_V2_HISTORY_MEASUREMENTS_FILENAME)
+
+        # Reading the file
+        history_measurements = self._read_json(file_path)
+
+        return history_measurements
+    
+    def get_drift_v2_history_insights(self) -> dict:
+        """
+        Gets the `drift_v2` history insights.
+
+        :returns: The `drift_v2` history insights.
+        """
+        history_insights = None
+
+        # Getting the file path
+        file_path = self._get_file_path(Model.DRIFT_V2_HISTORY_INSIGHTS_FILENAME)
+
+        # Reading the file
+        history_insights = self._read_json(file_path)
+
+        return history_insights
+    
+    def get_drift_v2_history_intervals(self) -> dict:
+        """
+        Gets the `drift_v2` history intervals.
+
+        :returns: The `drift_v2` history intervals.
+        """
+        history_intervals = None
+
+        # Getting the file path
+        file_path = self._get_file_path(Model.DRIFT_V2_HISTORY_INTERVALS_FILENAME)
+
+        # Reading the file
+        history_intervals = self._read_json(file_path)
+
+        return history_intervals
+    
+    def get_drift_v2_history_stats_baseline(self) -> dict:
+        """
+        Gets the `drift_v2` history stats-baseline.
+
+        :returns: The `drift_v2` history stats-baseline.
+        """
+        history_stats_baseline = None
+
+        # Getting the file path
+        file_path = self._get_file_path(Model.DRIFT_V2_HISTORY_STATS_BASELINE_FILENAME)
+
+        # Reading the file
+        history_stats_baseline = self._read_json(file_path)
+
+        return history_stats_baseline
+    
+    def get_drift_v2_history_stats_production(self) -> dict:
+        """
+        Gets the `drift_v2` history stats-production.
+
+        :returns: The `drift_v2` history stats-production.
+        """
+        history_stats_production = None
+
+        # Getting the file path
+        file_path = self._get_file_path(Model.DRIFT_V2_HISTORY_STATS_PRODUCTION_FILENAME)
+
+        # Reading the file
+        history_stats_production = self._read_json(file_path)
+
+        return history_stats_production
 
     def get_payload_history(self, num_day):
         # There are 3 ways to specify payload history:
         # 1. a set of 'payload_history_N.json' files, each containing a full day of payloads specific to one specific day, to be evenly divided across 24 hours
         # 2. one 'payload_history_day.json' file contains one full day of payloads, to be divided across 24 hours and duplicated every day
         # 3. one 'payload_history.json' file contains one hour of payloads, to be duplicated for every hour of every day
         fullRecordsList = []
@@ -538,7 +629,21 @@
             with open(history_file) as f:
                 drift_measurement = json.load(f)
 
         if drift_annotations and drift_measurement:
             return [{ 'drift_annotations': drift_annotations, 'drift_measurement': drift_measurement }]
         else:
             return [] # both files are required for a complete drift history
+    
+    def _read_json(self, file_path: str) -> dict:
+        """
+        Reads the file for the given file path.
+        :file_path: The file path.
+
+        :returns: The file read as dictionary.
+        """
+        js = None
+
+        with io.open(file_path, "r") as f:
+            js = json.loads(f.read())
+
+        return js
```

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/openscale/openscale.py` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/openscale/openscale.py`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/openscale/openscale_client.py` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/openscale/openscale_client.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,22 +13,22 @@
 import os
 import random
 import requests
 import time
 import uuid
 
 from datetime import datetime, timedelta
-from retry import retry
+from retrying import retry
 
 from ibm_ai_openscale_cli import logging_temp_file, name as cli_name
 from ibm_ai_openscale_cli.api_environment import ApiEnvironment
 from ibm_ai_openscale_cli.enums import MLEngineType
 from ibm_ai_openscale_cli.models.model import Model
 from ibm_ai_openscale_cli.openscale.openscale_reset import OpenScaleReset
-from ibm_ai_openscale_cli.utility_classes.constants import DRIFT_ARCHIVE_ENV_MAPPING, WML_CHALLENGER_ENVIRONMENT_MAPPING, WML_SPARK_VERSION_SUPPORT_MAPPING
+from ibm_ai_openscale_cli.utility_classes.constants import DRIFT_ARCHIVE_ENV_MAPPING, DRIFT_V2_ARCHIVE_ENV_MAPPING, WML_CHALLENGER_ENVIRONMENT_MAPPING, WML_SPARK_VERSION_SUPPORT_MAPPING
 from ibm_ai_openscale_cli.utility_classes.fastpath_logger import FastpathLogger
 from ibm_ai_openscale_cli.utility_classes.utils import remove_port_from_url, update_url, get_url_elements
 from ibm_watson_openscale.base_classes.watson_open_scale_v2 import Asset, AssetDeploymentRequest, AssetPropertiesRequest, DatabaseConfigurationRequest, LocationSchemaName, Measurements, PatchDocument, PrimaryStorageCredentialsLong, Records, SparkStruct, Target, WMLCredentialsCP4D
 from ibm_watson_openscale.supporting_classes.enums import AssetTypes, DatabaseType, DataSetTypes, DeploymentTypes, InputDataType, ProblemType, ServiceTypes, TargetTypes
 from ibm_watson_openscale.supporting_classes.payload_record import PayloadRecord
 
 logger = FastpathLogger(__name__)
@@ -62,15 +62,15 @@
         self._explainability_run_once = True
         self._use_bkpi = False
         self._configure_explain = True
 
     def set_cos_credentials(self, _cos_credentials):
         self._cos_credentials = _cos_credentials
 
-    @retry(tries=5, delay=4, backoff=2)
+    @retry(stop_max_attempt_number=5, wait_exponential_multiplier=4000)
     def _reliable_get_or_create_bucket(self, _cos_instance):
         bucket = _cos_instance.get_wos_bucket()
         if not bucket:
             bucket = _cos_instance.create_wos_bucket()
         return bucket.name
 
     def perform_cos_operations(self, _cos_instance):
@@ -141,19 +141,19 @@
         if self._database is None:
             logger.log_info('PostgreSQL instance: internal')
         else:
             self._reliable_create_schema()
         self._reliable_create_datamart()
         logger.log_info('Datamart {} created successfully'.format(self._datamart_name))
 
-    @retry(tries=3, delay=5, backoff=2)
+    @retry(stop_max_attempt_number=3, wait_exponential_multiplier=5000)
     def _reliable_create_schema(self):
         self._database.create_new_schema(self._datamart_name, self._keep_schema)
 
-    @retry(tries=5, delay=4, backoff=2)
+    @retry(stop_max_attempt_number=5, wait_exponential_multiplier=4000)
     def _reliable_create_datamart(self):
         start = time.time()
         if self._database is None:
             self._client.data_marts.add(name=self._datamart_name, internal_database=True, background_mode=False)
         else:
             db_config_request = None
             if self._database_credentials['db_type'] == 'postgresql':
@@ -222,15 +222,15 @@
                     )
             except Exception as e:
                 raise Exception("Failed while creating datamart with the specified database instance: {}".format(str(e)))
 
         elapsed = time.time() - start
         self.timer('data_mart.setup', elapsed)
 
-    @retry(tries=5, delay=4, backoff=2)
+    @retry(stop_max_attempt_number=5, wait_exponential_multiplier=4000)
     def _reliable_bind_mlinstance(self, credentials, ml_engine=None, is_mrm_preprod=False):
         # if self._args.ml_engine_type is MLEngineType.WML:
         #     if self._args.is_icp:
         #         if 'apikey' in credentials:
         #             ml_instance = WMLCredentialsCloud(credentials)
         #             binding_name = 'IBM Cloud {}'.format(binding_name)
         #         else:
@@ -352,15 +352,15 @@
                     self._binding_id = provider_id
                 elif provider_name == SERVICE_PROVIDER_NAME.format(OPERATIONAL_PRE_PRODUCTION_SPACE_ID):
                     self._binding_id_mrm_preprod = provider_id
         else:
             self._binding_id = asset_details_dict["binding_uid"]
         logger.log_info("Use existing binding {}".format(self.get_binding_id()))
 
-    @retry(tries=5, delay=4, backoff=2)
+    @retry(stop_max_attempt_number=5, wait_exponential_multiplier=4000)
     def use_existing_subscription(self, asset_details_dict):
         self._asset_details_dict = asset_details_dict
         asset_uid = asset_details_dict['source_uid']
         deployment_uid = asset_details_dict['source_entry_metadata_guid']
         logger.log_info('Get existing subscription for model {} deployment {}...'.format(asset_uid, deployment_uid))
         start = time.time()
         all_subscriptions = self._client.subscriptions.list().result.subscriptions
@@ -384,15 +384,15 @@
                                         target_target_type=TargetTypes.SUBSCRIPTION
                                     ).result.data_sets[0].metadata.id
         elapsed = time.time() - start
         self._model.expected_payload_row_count = self._reliable_count_payload_rows('use existing subscription')
         logger.log_info('Subscription {} found successfully'.format(self.get_subscription_id()))
         self._reliable_count_datamart_rows('use existing subscription')
 
-    @retry(tries=1, delay=4, backoff=2)
+    @retry(stop_max_attempt_number=1, wait_exponential_multiplier=4000)
     def subscribe_to_model_deployment(self, asset_details_dict):
         '''
         Create subscription for the given model
         '''
         logger.log_info('Subscribing ML deployment to {} ...'.format(self._args.service_name))
         self._reliable_count_datamart_rows('create subscription start')
         asset_metadata = self._model.configuration_data['asset_metadata']
@@ -513,15 +513,15 @@
         elif data == 'MULTICLASS_CLASSIFICATION':
             return ProblemType.MULTICLASS_CLASSIFICATION
         elif data == 'REGRESSION':
             return ProblemType.REGRESSION
         return None
 
     # not actually called, because payload logging and performance monitoring are both already enabled by default
-    @retry(tries=5, delay=8, backoff=2)
+    @retry(stop_max_attempt_number=5, wait_exponential_multiplier=8000)
     def configure_subscription(self):
         '''
         Configure payload logging and performance monitoring
         '''
         logger.log_info('Enabling payload logging ...')
         start = time.time()
         self._subscription.payload_logging.enable()
@@ -544,23 +544,26 @@
                 params = self._model.configuration_data[param_key_name]
                 logger.log_info('Configuring {} ...'.format(param_name))
             else:
                 logger.log_info('Configuration for {} not provided for this model - skipping'.format(param_name))
             return params
 
         self.configure_explainability()
+        if self._args.drift_v2:
+            self.configure_drift_v2(_get_config_params("drift_v2_configuration"))
+        else:
+            self.configure_drift(_get_config_params('drift_configuration'))
         self.configure_fairness(_get_config_params('fairness_configuration'))
         self.configure_quality(_get_config_params('quality_configuration'))
-        self.configure_drift(_get_config_params('drift_configuration'))
         # if self._args.bkpi:
         #     self.configure_bkpi(_get_config_params('businesskpi_configuration'))
         if self._args.mrm:
             self.configure_mrm(_get_config_params('mrm_configuration'))
 
-    @retry(tries=5, delay=8, backoff=2)
+    @retry(stop_max_attempt_number=5, wait_exponential_multiplier=8000)
     def configure_fairness(self, params):
         if params:
             start = time.time()
             if self._fairness_run_once:  # in case of retry
                 self._fairness_run_once = False
             parameters = {
                 "features": params["features"],
@@ -603,15 +606,15 @@
                 thresholds=thresholds
             ).result
             self._fairness_monitor_instance_id = fairness_monitor_details.metadata.id
             elapsed = time.time() - start
             self.timer("subscription.fairness_monitoring.enable", elapsed)
             logger.log_info('Fairness configured successfully')
 
-    @retry(tries=5, delay=8, backoff=2)
+    @retry(stop_max_attempt_number=5, wait_exponential_multiplier=8000)
     def configure_quality(self, params):
         if params:
             start = time.time()
             target = Target(
                 target_type=TargetTypes.SUBSCRIPTION,
                 target_id=self._subscription_id
             )
@@ -632,15 +635,15 @@
                 thresholds=thresholds
             ).result
             self._quality_monitor_instance_id = quality_monitor_details.metadata.id
             elapsed = time.time() - start
             self.timer('subscription.quality_monitoring.enable', elapsed)
             logger.log_info('Quality configured successfully')
 
-    @retry(tries=5, delay=8, backoff=2)
+    @retry(stop_max_attempt_number=5, wait_exponential_multiplier=8000)
     def configure_explainability(self):
         explain_required_columns_absent = 'class_probability_columns' not in self._model.configuration_data['asset_metadata'] and 'probability_column' not in self._model.configuration_data['asset_metadata']
         is_xgboost_model = 'xgboost' in self._model.name.lower()
         if not is_xgboost_model and explain_required_columns_absent:
             logger.log_info('Explainability not available for this model')
             self._configure_explain = False
             return
@@ -672,15 +675,15 @@
             parameters=parameters
         ).result
         self._explainability_monitor_id = explainability_details.metadata.id
         elapsed = time.time() - start
         self.timer('subscription.explainability.enable', elapsed)
         logger.log_info('Explainability configured successfully')
 
-    @retry(tries=5, delay=8, backoff=2)
+    @retry(stop_max_attempt_number=5, wait_exponential_multiplier=8000)
     def configure_drift(self, params):
         if params:
             start = time.time()
 
             # Configuring Drift
             data_mart_id = self.get_datamart_id()
             subscription_id = self.get_subscription_id()
@@ -746,15 +749,15 @@
         if response.ok is False:
             error_msg = "ERROR: Failed to get the fairness heartbeat, url: {}, rc: {}, response: {}".format(url, response.status_code, response.text)
             logger.log_error(error_msg)
             raise Exception(error_msg)
 
         return response.json()
 
-    @retry(tries=5, delay=8, backoff=2)
+    @retry(stop_max_attempt_number=5, wait_exponential_multiplier=8000)
     def configure_mrm(self, params):
         # save preprod subscription id so it can be used later by prod subscription mrm configuration
         if self.is_mrm_preprod:
             self.mrm_preprod_subscription_id = self.get_subscription_id()
         start = time.time()
         target = Target(target_type="subscription", target_id=self.get_subscription_id())
         parameters = {}
@@ -792,14 +795,103 @@
             if response.status_code != 200:
                 error_msg = 'ERROR: Failed to patch subscription with pre-prod reference, rc: {} url: {} payload: {} response: {}'.format(response.status_code, mrm_url, payload, response.text)
                 logger.log_error(error_msg)
                 raise Exception(error_msg)
             self.timer('subscription.mrm patch prod', elapsed)
 
         logger.log_info('MRM configured successfully')
+    
+    def upload_drift_v2_archive(self, file_path: str) -> None:
+        """
+        Uploads the Drift_V2 baseline archive for the given subscription.
+        :file_path: The file_path of the baseline archive.
+
+        :returns: None.
+        """
+
+        url = "{}/openscale/{}/v2/monitoring_services/drift_v2/archives?archive_name={}&subscription_id={}".format(self._client.service_url.split("/openscale")[0], self.get_datamart_id(), Model.DRIFT_V2_ARCHIVE_FILENAME, self.get_subscription_id())
+
+        payload = open(file_path, "rb")
+        token = self._args.iam_token if self._args.iam_token else self._client.authenticator.token_manager.get_token()
+        headers = {
+            "Authorization": "bearer {}".format(token),
+            "Content-Type": "application/octet-stream"
+        }
+
+        response = requests.request("PUT", url, headers=headers, data=payload, verify=False)
+
+        if not response.ok:
+            error_msg = "ERROR: Failed to upload drift_v2 baseline archive, url: {}, rc: {}, response: {}".format(url, response.status_code, response.text)
+            logger.log_error(error_msg)
+            raise Exception(error_msg)
+
+        return
+    
+    def configure_drift_v2(self, params: dict) -> None:
+        """
+        Configures Drift 2.0 (`drift_v2`) monitor for the current subscription.
+        :params: The parameters with which the monitor instance is to be created.
+
+        :returns: None.
+        """
+
+        start = time.time()
+
+        # Getting IDs
+        data_mart_id = self.get_datamart_id()
+        subscription_id = self.get_subscription_id()
+        target = Target(
+            target_type=TargetTypes.SUBSCRIPTION,
+            target_id=subscription_id
+        )
+
+        # Uploading the Drift_V2 archive
+        logger.log_info("Uploading the Drift V2 baseline archive.")
+
+        # Getting the file path
+        file_name = "drift_v2_archives/{}/{}".format(DRIFT_V2_ARCHIVE_ENV_MAPPING[self._args.environment], Model.DRIFT_V2_ARCHIVE_FILENAME)
+        file_path = self._model._get_file_path(file_name)
+
+        # Uploading the baseline archive
+        self.upload_drift_v2_archive(file_path)
+        logger.log_info("Drift V2 baseline archive uploaded successfully for drift configuration.")
+
+        # Configuring the drift_v2 monitor
+        drift_v2_monitor_details = self._client.monitor_instances.create(
+            data_mart_id=data_mart_id,
+            background_mode=True,
+            monitor_definition_id=self._client.monitor_definitions.MONITORS.DRIFT_V2.ID,
+            target=target,
+            parameters=params
+        ).result
+        self._drift_v2_monitor_instance_id = drift_v2_monitor_details.metadata.id
+
+        # Polling the status
+        drift_v2_state = drift_v2_monitor_details.to_dict()["entity"]["status"]["state"]
+        total_wait_time = 0
+        while drift_v2_state == "preparing":
+            logger.log_info("Drift_V2 monitor instance state: {}".format(drift_v2_state))
+            if total_wait_time >= 600:
+                raise Exception("Drift_V2 did not turn to `active` state in 10 mins.")
+            time.sleep(10)
+            total_wait_time += 10
+            drift_v2_monitor_details = self._client.monitor_instances.get(self._drift_v2_monitor_instance_id).result.to_dict()
+            drift_v2_state = drift_v2_monitor_details["entity"]["status"]["state"]
+            if drift_v2_state == "active":
+                logger.log_info("Drift_V2 monitor instance state: {}".format(drift_v2_state))
+                logger.log_info("Drift V2 configured successfully.")
+                break
+            elif drift_v2_state == "error":
+                logger.log_error("Drift V2 configuration failed with error: {}".format(drift_v2_monitor_details["entity"]["status"]))
+                raise Exception(drift_v2_monitor_details["entity"]["status"])
+        
+        elapsed = time.time() - start
+        self.timer("subscription.drift_v2_monitoring.enable", elapsed)
+
+        return
 
     def generate_sample_metrics(self):
         if self._args.history < 1 or (self._args.mrm and self.is_mrm_challenger or self.is_mrm_preprod):
             return False
         self._reliable_count_datamart_rows('generate sample metrics start')
         return True
 
@@ -962,15 +1054,15 @@
                 )
                 patch_documents.append(patch_document)
             if len(patch_documents) > 0:
                 response = records_client.patch(data_set_id=self._payload_dataset_id, patch_document=patch_documents)
             if (day + 1) == self._args.history:
                 logger.log_info('Historical manual labeling data loaded successfully')
     
-    @retry(tries=5, delay=4, backoff=2)
+    @retry(stop_max_attempt_number=5, wait_exponential_multiplier=4000)
     def _reliable_store_fairness_monitor_metrics(self, records):
         '''
         Retry the loading metrics so that if a specific day fails, just retry that day, rather than retry the whole sequence
         '''
         if not records:
             logger.log_debug('No fairness_monitor history provided to load - skipping')
             return
@@ -1041,17 +1133,161 @@
                             break
                         else:
                             logger.log_info('Loading historical drift metrics to {} ...'.format(self._args.service_name))
                     logger.log_info(' - Loading day {}'.format(day + 1))
                     self._post_drift_metrics(records, day)
                     if (day + 1) == self._args.history:
                         logger.log_info('Historical drift metrics loaded successfully')
+        
+        return
+    
+    def load_historical_drift_v2(self) -> None:
+        """
+        Loads historical data for `drift_v2` monitor that includes the measurements and the data-sets for insights, intervals, stats.
+
+        :returns: None.
+        """
+
+        if "drift_v2_configuration" in self._model.configuration_data and self._args.history > 0:
+            if self._no_historical_payloads:
+                logger.log_info("No historical payloads provided - skipping drift_v2 history generation.")
+            else:
+                logger.log_info('Generating {} days of historical drift_v2 metrics to {} ...'.format(self._args.history, self._args.service_name))
 
+                # Reading the historical measurements
+                drift_v2_measurement_payloads = self._model.get_drift_v2_history_measurements()
+                measurement_mapping = {}
+                run_id_mapping = {"day_{}".format(x): str(uuid.uuid4()) for x in range(1, 8)}
+                old_measurement_timestamp_mapping = {}
+                run_id_timestamp_mapping = {}
+
+                # DRIFT_V2 Data-set IDs for the GCR model stored in history,
+                # to be replaced with actual IDs generated at runtime
+                HISTORY_DRIFT_V2_STATS_DATASET_ID = "a8e3ed29-f412-4364-a22f-22efb3966733"
+                HISTORY_DRIFT_V2_INTERVALS_DATASET_ID = "16ece0c1-ef48-442b-bf61-0a33354189dd"
+                HISTORY_DRIFT_V2_INSIGHTS_DATASET_ID = "500ab456-4ae0-4082-ac23-72ec2b350a4b"
+
+                # Getting the actual runtime data-set IDs
+                drift_v2_monitor_instance = self._client.monitor_instances.get(self._drift_v2_monitor_instance_id).result.to_dict()
+                drift_v2_dataset_ids = drift_v2_monitor_instance["entity"]["parameters"]["context"]["data_sets"]
+                ACTUAL_DRIFT_V2_STATS_DATASET_ID = drift_v2_dataset_ids["drift_stats"]
+                ACTUAL_DRIFT_V2_INTERVALS_DATASET_ID = drift_v2_dataset_ids["drift_intervals"]
+                ACTUAL_DRIFT_V2_INSIGHTS_DATASET_ID = drift_v2_dataset_ids["drift_insights"]
 
-    @retry(tries=5, delay=8, backoff=2)
+                for day in range(self._args.history):
+                    logger.log_info(' - Loading day {}'.format(day + 1))
+                    
+                    # Taking the day's measurements from the consolidated JSON
+                    run_id = "day_{}".format(day + 1)
+                    day_measurement_payloads = drift_v2_measurement_payloads[run_id]
+
+                    # Getting the timestamp for the day's measurements
+                    timestamp = (datetime.utcnow() + timedelta(days=-(day + 1))).strftime("%Y-%m-%dT%H:%M:%SZ")
+                    run_id_timestamp_mapping[run_id] = timestamp
+
+                    for measurement_payload in day_measurement_payloads:
+                        old_measurement_id = measurement_payload["old_measurement_id"]
+                        del measurement_payload["old_measurement_id"]
+                        old_measurement_timestamp_mapping[old_measurement_id] = timestamp
+
+                        # Updating the values in the payload
+                        measurement_payload["timestamp"] = timestamp
+                        measurement_payload["run_id"] = run_id_mapping[run_id]
+
+                        # Replaing the data-set IDs
+                        measurement_payload = json.loads(json.dumps(measurement_payload).replace(HISTORY_DRIFT_V2_STATS_DATASET_ID, ACTUAL_DRIFT_V2_STATS_DATASET_ID))
+                        measurement_payload = json.loads(json.dumps(measurement_payload).replace(HISTORY_DRIFT_V2_INTERVALS_DATASET_ID, ACTUAL_DRIFT_V2_INTERVALS_DATASET_ID))
+                        measurement_payload = json.loads(json.dumps(measurement_payload).replace(HISTORY_DRIFT_V2_INSIGHTS_DATASET_ID, ACTUAL_DRIFT_V2_INSIGHTS_DATASET_ID))
+
+                        # Replacing run ID
+                        measurement_payload = json.loads(json.dumps(measurement_payload).replace(run_id, run_id_mapping[run_id]))
+
+                        # Publishing the measurement
+                        measurement_response = self._client.monitor_instances.measurements.add(
+                            monitor_instance_id=self._drift_v2_monitor_instance_id,
+                            monitor_measurement_request=[measurement_payload]
+                        ).result[0]
+                        measurement_mapping[old_measurement_id] = measurement_response["measurement_id"]
+                
+                # Loading the `drift_v2` data-sets
+                drift_v2_data_sets = ["drift_insights", "drift_intervals", "drift_stats"]
+                for data_set_type in drift_v2_data_sets:
+                    # Getting the data-set ID
+                    data_set_id = self._client.data_sets.list(
+                        targe_target_id=self.get_subscription_id(),
+                        target_target_type="subscription",
+                        type=data_set_type
+                    ).result.to_dict()["data_sets"][0]["metadata"]["id"]
+
+                    # Loading the data in the data-sets
+                    if data_set_type in ["drift_insights", "drift_intervals"]:
+                        # Reading the payloads
+                        payloads = self._model.get_drift_v2_history_insights() if data_set_type == "drift_insights" else self._model.get_drift_v2_history_intervals()
+                        for payload in payloads:
+                            # Getting the old measurement ID
+                            old_measurement_id = payload["measurement_id"]
+                            # Getting the new measurement ID
+                            new_measurement_id = measurement_mapping[old_measurement_id]
+                            # Getting the timestamp
+                            timestamp = old_measurement_timestamp_mapping[old_measurement_id]
+                            # Getting the run_id
+                            run_id = run_id_mapping[payload["run_id"]]
+
+                            # Updating the values in the payload
+                            payload["measurement_id"] = new_measurement_id
+                            payload["run_id"] = run_id
+                            payload["ts"] = timestamp
+                        # Storing the record
+                        logger.log_info("Loading the {} records!".format(data_set_type))
+                        self._client.data_sets.store_records(
+                            data_set_id=data_set_id,
+                            request_body=payloads,
+                            background_mode=False
+                        )
+                    elif data_set_type == "drift_stats":
+                        # Loading the baseline
+                        baseline_records = self._model.get_drift_v2_history_stats_baseline()
+
+                        # Generating the baseline timestamp
+                        baseline_timestamp = (datetime.utcnow() + timedelta(days=-8)).strftime("%Y-%m-%dT%H:%M:%SZ")
+
+                        for payload in baseline_records:
+                            payload["monitor_instance_id"] = self._drift_v2_monitor_instance_id
+                            payload["ts"] = baseline_timestamp
+                        
+                        # Storing the record
+                        logger.log_info("Loading the {}_baseline records!".format(data_set_type))
+                        self._client.data_sets.store_records(
+                            data_set_id=data_set_id,
+                            request_body=baseline_records,
+                            background_mode=False
+                        )
+
+                        # Loading the production
+                        production_records = self._model.get_drift_v2_history_stats_production()
+
+                        for payload in production_records:
+                            payload["monitor_instance_id"] = self._drift_v2_monitor_instance_id
+                            if "day" in payload["drift_data_set_id"]:
+                                payload["ts"] = run_id_timestamp_mapping[payload["drift_data_set_id"]]
+                                payload["monitor_instance_id"] = self._drift_v2_monitor_instance_id
+                                payload["drift_data_set_id"] = run_id_mapping[payload["drift_data_set_id"]]
+                        
+                        # Storing the record
+                        logger.log_info("Loading the {}_production records!".format(data_set_type))
+                        self._client.data_sets.store_records(
+                            data_set_id=data_set_id,
+                            request_body=production_records,
+                            background_mode=False
+                        )
+                logger.log_info('Historical drift_v2 metrics generated successfully.')
+        
+        return
+
+    @retry(stop_max_attempt_number=5, wait_exponential_multiplier=8000)
     def _reliable_upload_feedback(self, feedback_data):
         start = time.time()
         if self._model.is_unstructured_text:
             self._subscription.feedback_logging.store(feedback_data)
         else:
             self._feedback_dataset_id = self._client.data_sets.list(
                 type=DataSetTypes.FEEDBACK,
@@ -1064,15 +1300,15 @@
                 self._feedback_dataset_id,
                 request_body=feedback_data,
                 background_mode=False
             ).result.to_dict()
         elapsed = time.time() - start
         self.timer('subscription.feedback_logging.store', elapsed)
 
-    @retry(tries=5, delay=4, backoff=2)
+    @retry(stop_max_attempt_number=5, wait_exponential_multiplier=4000)
     def _reliable_single_score(self, engine_client, deployment_url, score_input, score_num, values_per_score, totalelapsed, firststart, lastend, tokenizer=None):
         record = None
         start = time.time()
         if self._args.v4:
             deployment_id = self._asset_details_dict['source_entry_metadata_guid']
             if 'fields' in score_input:
                 record = engine_client.score(deployment_id, values=score_input['values'], fields=score_input['fields'])
@@ -1262,27 +1498,27 @@
         if to_init_payload_logging:
             context = 'init payload logging'
         else:
             context = 'live scoring'
         self.wait_for_payload_logging(context=context, to_init_payload_logging=to_init_payload_logging)
         self._reliable_count_datamart_rows('generated sample scores and confirmed payload logging')
 
-    @retry(tries=5, delay=4, backoff=2)
+    @retry(stop_max_attempt_number=5, wait_exponential_multiplier=4000)
     def _reliable_count_payload_rows(self, context=None):
         start = time.time()
         actual_payload_rows = self._client.data_sets.get_records_count(data_set_id = self._payload_dataset_id)
         elapsed = time.time() - start
         if context:
             context = ', {}'.format(context)
         else:
             context = ''
         logger.log_timer('subscription count payload rows in {:.3f} seconds, rows={}, expected={}{}'.format(elapsed, actual_payload_rows, self._model.expected_payload_row_count, context))
         return actual_payload_rows
 
-    @retry(tries=5, delay=4, backoff=2)
+    @retry(stop_max_attempt_number=5, wait_exponential_multiplier=4000)
     def _reliable_count_datamart_rows(self, context=None):
         if self._database is None: # internal db
             logger.log_debug('DEBUG: cannot count datamart rows for internal db')
             if self._args.database_counts:
                 logger.log_info('Cannot count datamart rows for internal db - skipping')
             return
         start = time.time()
@@ -1343,16 +1579,32 @@
             self._reliable_count_datamart_rows('fairness monitor triggered')
             self._reliable_trigger_quality_check(background_mode)
             self._reliable_count_datamart_rows('quality monitor triggered')
             self._reliable_trigger_drift_check(background_mode)
             self._reliable_count_datamart_rows('drift monitor triggered')
         
         return
+    
+    def trigger_drift_v2_check(self) -> None:
+        """
+        Triggers the `drift_v2` monitor for the current drift_v2 monitor instance.
 
-    @retry(tries=5, delay=4, backoff=2)
+        :returns: None.
+        """
+
+        # Running the `drift_v2` monitor
+        self._client.monitor_instances.run(
+            monitor_instance_id=self._drift_v2_monitor_instance_id,
+            triggered_by="user",
+            background_mode=True
+        )
+
+        return
+
+    @retry(stop_max_attempt_number=5, wait_exponential_multiplier=4000)
     def _reliable_trigger_fairness_check(self, background_mode):
         if 'fairness_configuration' not in self._model.configuration_data:
             logger.log_info('Skip fairness check since fairness not configured for model')
         else:
             try:
                 deployment_uid = self._asset_details_dict['source_entry_metadata_guid']
                 logger.log_info('Triggering immediate fairness check ...')
@@ -1365,15 +1617,15 @@
                     if not result or (isinstance(result, str) and 'error' in result.lower()) or result.entity.status.state.lower() != 'finished':
                         self.metric_check_errors.append([self._model.name, 'fairness-check', 'failed'])
             except Exception as e:
                 message = 'WARNING: Problems occurred while running fairness check: {}'.format(str(e))
                 logger.log_warning(message)
                 self.metric_check_errors.append([self._model.name, 'fairness-check', 'failed'])
 
-    @retry(tries=5, delay=4, backoff=2)
+    @retry(stop_max_attempt_number=5, wait_exponential_multiplier=4000)
     def _reliable_trigger_quality_check(self, background_mode):
         if 'quality_configuration' not in self._model.configuration_data:
             logger.log_info('Skip quality check since quality monitoring not configured for model')
         elif (not self._model.feedback_data or self._args.no_new_feedback) and (not self._model.feedback_history or self._args.history < 1):
             logger.log_info('Skip quality check for model since there is no feedback data yet')
         else:
             try:
@@ -1387,15 +1639,15 @@
                     if not result or (isinstance(result, str) and 'error' in result.lower()) or result.entity.status.state.lower() != 'finished':
                         self.metric_check_errors.append([self._model.name, 'quality-check', 'failed'])
             except Exception as e:
                 message = 'WARNING: Problems occurred while running quality check: {}'.format(str(e))
                 logger.log_warning(message)
                 self.metric_check_errors.append([self._model.name, 'quality-check', 'failed'])
 
-    @retry(tries=5, delay=4, backoff=2)
+    @retry(stop_max_attempt_number=5, wait_exponential_multiplier=4000)
     def _reliable_trigger_drift_check(self, background_mode):
         if 'drift_configuration' not in self._model.configuration_data:
             logger.log_info('Skip drift check since drift monitoring not configured for model')
         else:
             try:
                 logger.log_info('Triggering immediate drift check ...')
                 start = time.time()
@@ -1406,15 +1658,15 @@
                 if not result or (isinstance(result, str) and 'error' in result.lower()):
                     self.metric_check_errors.append([self._model.name, 'drift-check', 'failed'])
             except Exception as e:
                 message = 'WARNING: Problems occurred while running drift check: {}'.format(str(e))
                 logger.log_warning(message)
                 self.metric_check_errors.append([self._model.name, 'drift-check', 'failed'])
 
-    @retry(tries=5, delay=4, backoff=2)
+    @retry(stop_max_attempt_number=5, wait_exponential_multiplier=4000)
     def _reliable_trigger_mrm_prod_check(self, mrm_instance_id, background_mode):
         mrm_url = '{}/openscale/{}/v2/monitor_instances/{}/runs'.format(self._credentials['url'], self._credentials['data_mart_id'], mrm_instance_id)
         payload = {
             "parameters": {
                 "publish_fact": "true",
                 "on_demand_trigger": True
             },
@@ -1438,15 +1690,15 @@
             mrm_run_id = json_data["metadata"]["id"]
         else:
             error_msg = 'ERROR: Failed to trigger MRM check, url: {}, rc: {}, response: {}'.format(mrm_url, response.status_code, response.text)
             logger.log_error(error_msg)
             raise Exception(error_msg)
         return mrm_run_id
 
-    @retry(tries=5, delay=4, backoff=2)
+    @retry(stop_max_attempt_number=5, wait_exponential_multiplier=4000)
     def _reliable_trigger_mrm_preprod_check(self, mrm_instance_id, background_mode):
         if self.is_mrm_challenger:
             filename = 'test_data_challenger.csv'
         else:
             filename = 'test_data_preprod.csv'
         mrm_url = '{}/openscale/{}/v2/monitoring_services/mrm/monitor_instances/{}/risk_evaluations?test_data_set_name={}'.format(self._credentials['url'], self._credentials['data_mart_id'], mrm_instance_id, filename)
         payload = self._model.mrm_evaluation_data
@@ -1460,15 +1712,15 @@
 
         # check to see if the call was successful
         if response.status_code != 201 and response.status_code != 202:
             error_msg = 'ERROR: Failed to trigger MRM check, url: {}, rc: {}, response: {}'.format(mrm_url, response.status_code, response.text)
             logger.log_error(error_msg)
             raise Exception(error_msg)
 
-    @retry(tries=5, delay=4, backoff=2)
+    @retry(stop_max_attempt_number=5, wait_exponential_multiplier=4000)
     def _reliable_get_mrm_check_status(self, mrm_instance_id, mrm_run_id=None):
         # different URLs to check MRM run status between prod and pre-prod (PreProd or Challenger)
         if self.is_mrm_prod:
             results_url = '{}/openscale/{}/v2/monitor_instances/{}/runs/{}'.format(self._credentials['url'], self._credentials['data_mart_id'], mrm_instance_id, mrm_run_id)
         else:
             results_url = '{}/openscale/{}/v2/monitoring_services/mrm/monitor_instances/{}/risk_evaluations'.format(self._credentials['url'], self._credentials['data_mart_id'], mrm_instance_id)
         start = time.time()
@@ -1522,28 +1774,28 @@
             else:
                 logger.log_info('MRM check did not complete in 3 minutes, continuing')
         except Exception as e:
             message = 'WARNING: Problems occurred while running MRM check: {}'.format(str(e))
             logger.log_warning(message)
             self.metric_check_errors.append([self._model.name, 'mrm-check', 'failed'])
 
-    @retry(tries=5, delay=4, backoff=2)
+    @retry(stop_max_attempt_number=5, wait_exponential_multiplier=4000)
     def _reliable_post_payloads(self, records):
         '''
         Retry the loading payloads so that if a specific day fails, just retry that day, rather than retry the whole sequence
         '''
         if not records:
             logger.log_debug('No payload history provided to load - skipping')
             return
         start = time.time()
         self._client.data_sets.store_records(data_set_id=self._payload_dataset_id, request_body=records)
         elapsed = time.time() - start
         self.timer('subscription.payload_logging.store', elapsed)
 
-    @retry(tries=5, delay=4, backoff=2)
+    @retry(stop_max_attempt_number=5, wait_exponential_multiplier=4000)
     def _reliable_post_debiased_payloads(self, records):
         """
         Retry the loading so that if a specific day fails, just retry that day, rather than retry the whole sequence
         """
         if not records:
             logger.log_debug('No debiased payloads history provided to load - skipping')
             return
@@ -1580,29 +1832,29 @@
 
         elapsed = time.time() - start
         self.timer('post data_mart debiased payloads history', elapsed)
 
         if response.status_code < 200 or response.status_code > 299:
             logger.log_warning('WARNING: while posting debiased payloads history: {}'.format(str(response.result.to_dict())))
 
-    @retry(tries=5, delay=4, backoff=2)
+    @retry(stop_max_attempt_number=5, wait_exponential_multiplier=4000)
     def _reliable_store_quality_monitor_metrics(self, records):
         '''
         Retry the loading metrics so that if a specific day fails, just retry that day, rather than retry the whole sequence
         '''
         if not records:
             logger.log_debug('No quality_monitor history provided to load - skipping')
             return
         start = time.time()
         measurements_client = Measurements(watson_open_scale=self._client)
         measurements_client.add(monitor_instance_id=self._quality_monitor_instance_id, monitor_measurement_request=records)
         elapsed = time.time() - start
         self.timer('post data_mart quality_monitor metrics', elapsed)
 
-    @retry(tries=5, delay=4, backoff=2)
+    @retry(stop_max_attempt_number=5, wait_exponential_multiplier=4000)
     def _reliable_generate_drift_metrics(self, start_time, end_time, windows=8): # eight 3-hour drift windows in 24 hours
         date_format = '%Y-%m-%dT%H:%M:%S.%fZ'
         start_time_param = start_time.strftime(date_format)
         end_time_param = end_time.strftime(date_format)
 
         drift_tasks_url = '{}/v1/data_marts/{}/service_bindings/{}/subscriptions/{}/drift_tasks'.format(self._credentials['url'], self._credentials['data_mart_id'], self.get_binding_id(), self.get_subscription_id())
         drift_tasks_url += '?start_time={}&end_time={}&compute_windows={}'.format(start_time_param, end_time_param, windows)
@@ -1667,15 +1919,15 @@
                 break
         if not 'source_uid' in asset_details_dict:
             error_msg = 'ERROR: Could not find a deployment with the name: {}'.format(name)
             logger.log_error(error_msg)
             raise Exception(error_msg)
         return asset_details_dict
 
-    @retry(tries=5, delay=1, backoff=2)
+    @retry(stop_max_attempt_number=5, wait_exponential_multiplier=1000)
     def _get_explanation_status(self, scoring_id, background_mode):
         cem = not self._args.explain_no_cem
         logger.log_info("Starting explain request for scoring id: {}".format(scoring_id))
         start = time.time()
         subscription_id = self.get_subscription_id()
         explain = self._client.monitor_instances.get_explanation_tasks(explanation_task_id=scoring_id, subscription_id=subscription_id).result.to_dict()
         status = explain['entity']['status']['state']
@@ -1709,16 +1961,16 @@
             num_records = len(payload_table["records"])
             scoring_ids = [payload_table["records"][i]["entity"]["values"]["scoring_id"] for i in range(min(max_explain_candidates, num_records))]
             random.shuffle(scoring_ids)
             return start, end, scoring_ids
         except Exception as e:
             logger.log_warning('WARNING: Problems occurred while getting scoring ids for explanation: {}'.format(str(e)))
         return None, None, None
-
-    @retry(tries=3, delay=4, backoff=2)
+    
+    @retry(stop_max_attempt_number=3, wait_exponential_multiplier=4000)
     def generate_explain_requests(self):
         # no explains for an MRM pre-production model
         if self._args.mrm and not self.is_mrm_prod:
             return
         num_explains = self._args.num_explains
         if num_explains < 1:
             return
```

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/openscale/openscale_reset.py` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/openscale/openscale_reset.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # secrets, irrespective of what has been deposited with the U.S.Copyright Office.
 # ----------------------------------------------------------------------------------------------------
 
 # coding=utf-8
 import logging
 import os
 import time
-from retry import retry
+from retrying import retry
 
 from ibm_ai_openscale_cli.enums import ResetType
 from ibm_ai_openscale_cli.openscale.openscale import OpenScale
 from ibm_ai_openscale_cli.utility_classes.fastpath_logger import FastpathLogger
 
 logger = FastpathLogger(__name__)
 parent_dir = os.path.dirname(__file__)
@@ -40,29 +40,29 @@
             self.reset_metrics()
             self.reset_monitors()
         # "factory reset" the system
         elif reset_type is ResetType.DATAMART:
             self.delete_datamart()
             self.clean_database()
 
-    @retry(tries=5, delay=4, backoff=2)
+    @retry(stop_max_attempt_number=5, wait_exponential_multiplier=4000)
     def reset_metrics(self):
         '''
         Clean up the payload logging table, monitoring history tables etc, so that it restores the system
         to a fresh state with datamart configured, model deployments added, all monitors configured,
         but no actual metrics in the system yet. The system is ready to go.
         '''
         if self._database is None:
             logger.log_info('Internal database metrics cannot be reset - skipping')
         else:
             logger.log_info('Deleting datamart metrics ...')
             self._database.reset_metrics_tables(self._datamart_name)
             logger.log_info('Datamart metrics deleted successfully')
 
-    @retry(tries=5, delay=4, backoff=2)
+    @retry(stop_max_attempt_number=5, wait_exponential_multiplier=4000)
     def reset_monitors(self):
         '''
         Remove all configured monitors and corresponding metrics and history, but leave the actual model deployments
         (if any) in the datamart. User can proceed to configure the monitors via user interface, API, or fastpath.
         '''
         logger.log_info('Deleting datamart monitors ...')
         subscription_uids = self._client.data_mart.subscriptions.get_uids()
@@ -101,15 +101,15 @@
         if self._database is None:
             logger.log_info('Internal database monitor-related tables cannot be deleted - skipping')
         else:
             logger.log_info('Deleting datamart monitor-related tables ...')
             self._database.drop_metrics_tables(self._datamart_name)
             logger.log_info('Datamart monitor-related tables deleted successfully')
 
-    @retry(tries=5, delay=4, backoff=2)
+    @retry(stop_max_attempt_number=5, wait_exponential_multiplier=4000)
     def delete_datamart(self):
         attempt = 0
         added_filter = False
         try:
             start = time.time()
             while attempt < DATAMART_MAX_DELETION_ATTEMPTS:  # Wait until exception is thrown to confirm datamart is completely deleted
                 if attempt == 1:
@@ -154,16 +154,16 @@
                     logger.log_info('Datamart not present, nothing to delete')
                 else:
                     logger.log_info('Confirmed datamart deletion')
             else:
                 raise e
         if added_filter:
             logger.logger.removeFilter(NonExistingDatamartDeleteErrorFilter())
-
-    @retry(tries=5, delay=4, backoff=2)
+    
+    @retry(stop_max_attempt_number=5, wait_exponential_multiplier=4000)
     def clean_database(self):
         if self._database is None:
             logger.log_info('Internal database instance cannot be deleted - skipping')
         else:
             logger.log_info('Cleaning database ...')
             self._database.drop_existing_schema(self._datamart_name, self._keep_schema)
             logger.log_info('Database cleaned successfully')
```

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/openscale_ops.py` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/openscale_ops.py`

 * *Files 1% similar despite different names*

```diff
@@ -197,15 +197,18 @@
                     openscale_client.save_subscription_details()
                 if openscale_client.generate_sample_metrics():
                     openscale_client.load_historical_payloads()
                     openscale_client.load_historical_fairness()
                     openscale_client.load_historical_quality()
                     openscale_client.confirm_payload_logging()
                     openscale_client.load_historical_debiased_payloads()
-                    openscale_client.load_historical_drift()
+                    if self._args.drift_v2:
+                        openscale_client.load_historical_drift_v2()
+                    else:
+                        openscale_client.load_historical_drift()
                     openscale_client.load_historical_performance()
                     # Skip loading historic explanations in the case of CLI run
                     # Tracker: 24375
                     #openscale_client.load_historical_explanations()
                 
                 openscale_client.generate_sample_scoring(ml_engine, numscores=self._args.num_scores, values_per_score=self._args.values_per_score)
                 openscale_client.trigger_monitors()
```

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/ops.py` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/ops.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,11 +133,13 @@
             self._args.environment = Environment.CPD_4_0_2_PLUS.value
         elif fairness_version.startswith("4.0."):
             self._args.environment = Environment.CPD_4_0_8_PLUS.value
         elif fairness_version.startswith("4.5.0"):
             self._args.environment = Environment.CPD_4_5.value
         elif fairness_version.startswith(("4.5.1", "4.5.2")):
             self._args.environment = Environment.CPD_4_5_1_PLUS.value
-        else:
+        elif fairness_version.startswith(("4.5", "4.6")):
             self._args.environment = Environment.CPD_4_5_3_PLUS.value
+        else:
+            self._args.environment = Environment.CPD_4_7_PLUS.value
 
         return
```

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/reset_ops.py` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/reset_ops.py`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/setup_classes/cloud_foundry.py` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/setup_classes/cloud_foundry.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 # coding=utf-8
 from __future__ import print_function
 import json as json_import
 from ibm_ai_openscale_cli.utility_classes.fastpath_logger import FastpathLogger
 import requests
 import time
-from retry import retry
+from retrying import retry
 from ibm_ai_openscale_cli.utility_classes.utils import get_error_message
 
 logger = FastpathLogger(__name__)
 
 DEFAULT_URL = 'https://api.ng.bluemix.net'
 USER_INFO_URL = 'https://uaa.ng.bluemix.net/userinfo'
 
@@ -222,16 +222,16 @@
         logger.log_debug('CloudFoundry.delete_instance_key()')
         response = self._request(
             method='DELETE',
             url='/v2/resource_keys/{0}'.format(guid),
             accept_json=False)
 
         return response
-
-    @retry(tries=5, delay=1, backoff=2)
+    
+    @retry(stop_max_attempt_number=5, wait_exponential_multiplier=1000)
     def get_or_create_instance(self, service_name, service_instance_name=None, service_plan_guid=None, organization_name=None, space_name=None):
         """Returns a service instance.
         If there is no instance available, a new one is provisioned.
         If there is no existing service key, a new one is created.
 
         Arguments:
             service_name {string} -- service label, e.g.: conversation, spark, compose-for-postgres
```

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/setup_classes/cloud_foundry_cli.py` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/setup_classes/cloud_foundry_cli.py`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/setup_classes/resource_controller.py` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/setup_classes/resource_controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 # coding=utf-8
 from __future__ import print_function
 import json as json_import
 import time
 from ibm_ai_openscale_cli.utility_classes.fastpath_logger import FastpathLogger
 import requests
-from retry import retry
+from retrying import retry
 from ibm_ai_openscale_cli.utility_classes.utils import get_error_message
 
 DEFAULT_RESOURCE_GROUP_URL = 'https://resource-manager.cloud.ibm.com'
 DEFAULT_URL = 'https://resource-controller.cloud.ibm.com'
 ROLE_WRITER = 'Writer'
 REGION_ID_US_SOUTH = 'us-south'
 
@@ -139,15 +139,15 @@
         response = self._request(
             method='DELETE',
             url=self.url + '/v2/resource_keys/{0}'.format(guid),
             accept_json=False)
 
         return response
 
-    @retry(tries=5, delay=1, backoff=2)
+    @retry(stop_max_attempt_number=5, wait_exponential_multiplier=1000)
     def get_or_create_instance(self, resource_id, resource_name=None, resource_plan_id=None, resource_group=None, resource_group_name=None, create_credentials=True, target=REGION_ID_US_SOUTH, credentials_role=ROLE_WRITER):
         """Returns a service instance.
         If there is no instance available, a new one is provisioned.
         If there is no existing service key, a new one is created.
 
         Arguments:
             resource_id {string} -- The resource_id that identifies the service in the global catalog
```

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/setup_classes/resource_controller_cli.py` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/setup_classes/resource_controller_cli.py`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/setup_classes/setup_ibmcloud_services.py` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/setup_classes/setup_ibmcloud_services.py`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/setup_classes/setup_ibmcloud_services_cli.py` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/setup_classes/setup_ibmcloud_services_cli.py`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/setup_classes/setup_ibmcloud_services_rest.py` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/setup_classes/setup_ibmcloud_services_rest.py`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/setup_classes/setup_ibmcloudprivate_services.py` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/setup_classes/setup_ibmcloudprivate_services.py`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/setup_classes/setup_services.py` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/setup_classes/setup_services.py`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/setup_classes/token_manager.py` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/setup_classes/token_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # secrets, irrespective of what has been deposited with the U.S.Copyright Office.
 # ----------------------------------------------------------------------------------------------------
 
 # coding=utf-8
 import requests
 import time
 from ibm_ai_openscale_cli.utility_classes.fastpath_logger import FastpathLogger
-from retry import retry
+from retrying import retry
 from ibm_ai_openscale_cli.utility_classes.utils import get_error_message
 
 DEFAULT_IAM_URL = 'https://iam.bluemix.net/identity/token'
 DEFAULT_UAA_URL = 'https://login.ng.bluemix.net/UAALoginServerWAR/oauth/token'
 CONTENT_TYPE = 'application/x-www-form-urlencoded'
 ACCEPT = 'application/json'
 DEFAULT_IAM_AUTHORIZATION = 'Basic Yng6Yng='
@@ -47,15 +47,15 @@
                                     headers=headers, params=params,
                                     data=data, **kwargs)
         if 200 <= response.status_code <= 299:
             return response.json() if accept_json else response.text
 
         raise Exception(get_error_message(response))
 
-    @retry(tries=5, delay=1, backoff=2)
+    @retry(stop_max_attempt_number=5, wait_exponential_multiplier=1000)
     def get_token(self):
         """
         The source of the token is determined by the following logic:
         1. If user provides their own managed access token, assume it is valid and send it
         2. If this class is managing tokens and does not yet have one, make a request for one
         3. If this class is managing tokens and the token has expired refresh it. In case the refresh token is expired, get a new one
         If this class is managing tokens and has a valid token stored, send it
```

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/utility_classes/fastpath_logger.py` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/utility_classes/fastpath_logger.py`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/utility_classes/keras_unstructured_binary_text.py` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/utility_classes/keras_unstructured_binary_text.py`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/utility_classes/statistics_generator.py` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/utility_classes/statistics_generator.py`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/utility_classes/timer.py` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/utility_classes/timer.py`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_ai_openscale_cli/utility_classes/utils.py` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_ai_openscale_cli/utility_classes/utils.py`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_watson_openscale_cli_tool.egg-info/PKG-INFO` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_watson_openscale_cli_tool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibm-watson-openscale-cli-tool
-Version: 3.5.51
+Version: 3.5.52
 Summary: CLI library to automate the onboarding process to IBM Watson OpenScale
 Home-page: https://www.ibm.com/cloud/watson-openscale
 Author: IBM Corp
 Author-email: wps@us.ibm.com
 License: Apache-2.0
 Keywords: ai-openscale,ibm-watson
 Classifier: Programming Language :: Python
```

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/ibm_watson_openscale_cli_tool.egg-info/SOURCES.txt` & `ibm-watson-openscale-cli-tool-3.5.52/ibm_watson_openscale_cli_tool.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -38,14 +38,19 @@
 ibm_ai_openscale_cli/models/GermanCreditRiskModel/sagemaker/history_fairness.json
 ibm_ai_openscale_cli/models/GermanCreditRiskModel/sagemaker/history_payloads.json
 ibm_ai_openscale_cli/models/GermanCreditRiskModel/sagemaker/training_data.csv
 ibm_ai_openscale_cli/models/GermanCreditRiskModel/sagemaker/training_data_statistics.json
 ibm_ai_openscale_cli/models/GermanCreditRiskModel/spss/configuration.json
 ibm_ai_openscale_cli/models/GermanCreditRiskModel/spss/history_payloads.json
 ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/configuration.json
+ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/drift_v2_history_measurements_payload_per_run.json
+ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/drift_v2_insights_record_payloads.json
+ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/drift_v2_intervals_record_payloads.json
+ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/drift_v2_stats_baseline_record_payloads.json
+ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/drift_v2_stats_production_record_payloads.json
 ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/feedback_data.csv
 ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_debias.json
 ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_debiased_payloads_0.json
 ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_debiased_payloads_1.json
 ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_debiased_payloads_2.json
 ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_debiased_payloads_3.json
 ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_debiased_payloads_4.json
@@ -83,25 +88,33 @@
 ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/drift_archives/spark_2.4_model/scikit_0.20.2/drift_archive.tar.gz
 ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/drift_archives/spark_2.4_model/scikit_0.24.1/drift_archive.tar.gz
 ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/drift_archives/spark_2.4_model/scikit_0.24.2/drift_archive.tar.gz
 ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/drift_archives/spark_3.0_model/scikit_0.24.1/drift_archive.tar.gz
 ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/drift_archives/spark_3.0_model/scikit_1.0.2/drift_archive.tar.gz
 ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/drift_archives/spark_3.2_model/scikit_1.0.2/drift_archive.tar.gz
 ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/drift_archives/spark_3.3_model/scikit_1.0.2/drift_archive.tar.gz
+ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/drift_archives/spark_3.3_model/scikit_1.1.1/drift_archive.tar.gz
+ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/drift_v2_archives/4.7/baseline.tar.gz
+ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/drift_v2_archives/public_cloud/baseline.tar.gz
 ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/configuration.json
 ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/mrm_evaluation_data.csv
 ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/training_data.csv
 ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/training_data_statistics.json
+ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/4.7/model_content.gzip
+ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/4.7/model_meta.json
+ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/drift_archives/4.7/scikit_1.1.1/drift_archive.tar.gz
 ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/drift_archives/py_3.10/scikit_1.0.2/drift_archive.tar.gz
 ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/drift_archives/py_3.7/scikit_0.20.2/drift_archive.tar.gz
 ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/drift_archives/py_3.7/scikit_0.24.1/drift_archive.tar.gz
 ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/drift_archives/py_3.7/scikit_0.24.2/drift_archive.tar.gz
 ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/drift_archives/py_3.8/scikit_0.24.1/drift_archive.tar.gz
 ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/drift_archives/py_3.9/scikit_0.24.1/drift_archive.tar.gz
 ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/drift_archives/py_3.9/scikit_1.0.2/drift_archive.tar.gz
+ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/drift_v2_archives/4.7/baseline.tar.gz
+ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/drift_v2_archives/public_cloud/baseline.tar.gz
 ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/py_3.10/model_content.gzip
 ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/py_3.10/model_meta.json
 ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/py_3.7/model_content.gzip
 ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/py_3.7/model_meta.json
 ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/py_3.8/model_content.gzip
 ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/py_3.8/model_meta.json
 ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/py_3.9/model_content.gzip
@@ -137,8 +150,20 @@
 ibm_ai_openscale_cli/utility_classes/utils.py
 ibm_watson_openscale_cli_tool.egg-info/PKG-INFO
 ibm_watson_openscale_cli_tool.egg-info/SOURCES.txt
 ibm_watson_openscale_cli_tool.egg-info/dependency_links.txt
 ibm_watson_openscale_cli_tool.egg-info/entry_points.txt
 ibm_watson_openscale_cli_tool.egg-info/requires.txt
 ibm_watson_openscale_cli_tool.egg-info/top_level.txt
-ibm_watson_openscale_cli_tool.egg-info/zip-safe
+ibm_watson_openscale_cli_tool.egg-info/zip-safe
+tests/test_cloud_foundry.py
+tests/test_db2.py
+tests/test_openscale.py
+tests/test_postgres.py
+tests/test_resource_controller.py
+tests/test_set_up.py
+tests/test_setup_ibmcloud_services.py
+tests/test_setup_ibmcloud_services_rest.py
+tests/test_setup_ibmcloudprivate_services.py
+tests/test_token_manager.py
+tests/test_utils.py
+tests/test_watson_machine_learning.py
```

### Comparing `ibm-watson-openscale-cli-tool-3.5.51/setup.py` & `ibm-watson-openscale-cli-tool-3.5.52/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,22 +62,22 @@
     license='Apache-2.0',
     python_requires='>=3.5',
     long_description_content_type='text/markdown',
     install_requires=[
         'h5py>=2.9.0',
         'requests>=2.0, <3.0',
         'urllib3==1.26.12',
-        'retry>=0.9.0, <1.0.0',
+        'retrying==1.3.3',
         'boto3==1.17.22',
         'psycopg2==2.8.6',
         'ibm-db==3.0.3',
         'ibm-cloud-sdk-core==3.10.1',
         'ibm-watson-openscale>=3.0.12',
         'ibm-watson-machine-learning>=1.0.264',
-        'pandas==1.0.5',
+        'pandas==1.3.5',
         "pyJWT==2.4.0"
     ],
     dependency_links=[],
     tests_require=['responses', 'pytest', 'python_dotenv', 'pytest-rerunfailures', 'tox'],
     cmdclass={'test': PyTest},
     entry_points={'console_scripts': ['ibm-watson-openscale-cli=ibm_ai_openscale_cli.main:main']},
     author='IBM Corp',
```

