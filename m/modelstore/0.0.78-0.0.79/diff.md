# Comparing `tmp/modelstore-0.0.78.tar.gz` & `tmp/modelstore-0.0.79.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelstore-0.0.78.tar", last modified: Sat Mar 11 17:52:34 2023, max compression
+gzip compressed data, was "modelstore-0.0.79.tar", last modified: Fri Jun  9 14:53:14 2023, max compression
```

## Comparing `modelstore-0.0.78.tar` & `modelstore-0.0.79.tar`

### file list

```diff
@@ -1,260 +1,269 @@
-drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-03-11 17:52:34.523767 modelstore-0.0.78/
-drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-03-11 17:52:34.361981 modelstore-0.0.78/.github/
-drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-03-11 17:52:34.388494 modelstore-0.0.78/.github/workflows/
--rw-r--r--   0 neallathia   (501) staff       (20)     2296 2022-12-02 10:38:39.000000 modelstore-0.0.78/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 neallathia   (501) staff       (20)     2024 2022-12-03 00:48:26.000000 modelstore-0.0.78/.github/workflows/integration-tests.yml
--rw-r--r--   0 neallathia   (501) staff       (20)      716 2023-03-05 21:12:21.000000 modelstore-0.0.78/.github/workflows/unit-tests.yml
--rw-r--r--   0 neallathia   (501) staff       (20)      189 2023-03-05 21:12:21.000000 modelstore-0.0.78/.gitignore
--rw-r--r--   0 neallathia   (501) staff       (20)    12115 2023-03-11 17:50:24.000000 modelstore-0.0.78/CHANGELOG.md
--rw-r--r--   0 neallathia   (501) staff       (20)     5223 2022-01-13 15:38:40.000000 modelstore-0.0.78/CODE_OF_CONDUCT.md
--rw-r--r--   0 neallathia   (501) staff       (20)     3306 2022-01-30 13:01:45.000000 modelstore-0.0.78/CONTRIBUTING.md
--rw-r--r--   0 neallathia   (501) staff       (20)    11342 2022-01-13 15:38:40.000000 modelstore-0.0.78/LICENSE
--rw-r--r--   0 neallathia   (501) staff       (20)      451 2023-02-11 15:06:42.000000 modelstore-0.0.78/Makefile
--rw-r--r--   0 neallathia   (501) staff       (20)      685 2023-03-11 17:52:34.522972 modelstore-0.0.78/PKG-INFO
--rw-r--r--   0 neallathia   (501) staff       (20)     6520 2023-02-04 14:33:11.000000 modelstore-0.0.78/README.md
-drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-03-11 17:52:34.395363 modelstore-0.0.78/bin/
--rwxr-xr-x   0 neallathia   (501) staff       (20)      607 2023-02-11 15:06:42.000000 modelstore-0.0.78/bin/_brew_install
--rwxr-xr-x   0 neallathia   (501) staff       (20)      277 2022-12-17 10:26:28.000000 modelstore-0.0.78/bin/_build_library
--rwxr-xr-x   0 neallathia   (501) staff       (20)      222 2022-12-17 10:26:28.000000 modelstore-0.0.78/bin/_cleanup
--rwxr-xr-x   0 neallathia   (501) staff       (20)      262 2023-03-05 21:12:21.000000 modelstore-0.0.78/bin/_pyenv_config
--rwxr-xr-x   0 neallathia   (501) staff       (20)      758 2023-02-11 15:06:42.000000 modelstore-0.0.78/bin/_pyenv_install
--rwxr-xr-x   0 neallathia   (501) staff       (20)      466 2023-02-11 15:06:42.000000 modelstore-0.0.78/bin/_pyenv_uninstall
--rwxr-xr-x   0 neallathia   (501) staff       (20)      225 2022-12-17 10:26:28.000000 modelstore-0.0.78/bin/_release_prod
--rwxr-xr-x   0 neallathia   (501) staff       (20)      251 2022-12-17 10:26:28.000000 modelstore-0.0.78/bin/_release_test
-drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-03-11 17:52:34.397013 modelstore-0.0.78/examples/
--rw-r--r--   0 neallathia   (501) staff       (20)      971 2023-03-05 21:12:21.000000 modelstore-0.0.78/examples/Makefile-example
--rw-r--r--   0 neallathia   (501) staff       (20)     2346 2022-01-13 15:38:40.000000 modelstore-0.0.78/examples/README.md
-drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-03-11 17:52:34.400943 modelstore-0.0.78/examples/cli-examples/
--rw-r--r--   0 neallathia   (501) staff       (20)       32 2022-01-13 15:38:40.000000 modelstore-0.0.78/examples/cli-examples/.gitignore
--rw-r--r--   0 neallathia   (501) staff       (20)       61 2022-01-13 15:38:40.000000 modelstore-0.0.78/examples/cli-examples/Makefile
--rw-r--r--   0 neallathia   (501) staff       (20)     1009 2022-05-08 13:46:10.000000 modelstore-0.0.78/examples/cli-examples/model.py
--rw-r--r--   0 neallathia   (501) staff       (20)       13 2022-12-17 13:52:20.000000 modelstore-0.0.78/examples/cli-examples/requirements.txt
--rwxr-xr-x   0 neallathia   (501) staff       (20)      497 2022-01-13 15:38:40.000000 modelstore-0.0.78/examples/cli-examples/run-all.sh
-drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-03-11 17:52:34.404232 modelstore-0.0.78/examples/examples-by-ml-library/
--rw-r--r--   0 neallathia   (501) staff       (20)       62 2022-04-15 16:06:05.000000 modelstore-0.0.78/examples/examples-by-ml-library/Makefile
-drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-03-11 17:52:34.417147 modelstore-0.0.78/examples/examples-by-ml-library/libraries/
--rw-r--r--   0 neallathia   (501) staff       (20)        0 2022-01-13 15:38:40.000000 modelstore-0.0.78/examples/examples-by-ml-library/libraries/__init__.py
--rw-r--r--   0 neallathia   (501) staff       (20)     1472 2022-04-15 00:22:02.000000 modelstore-0.0.78/examples/examples-by-ml-library/libraries/annoy_example.py
--rw-r--r--   0 neallathia   (501) staff       (20)     1448 2022-04-15 00:22:02.000000 modelstore-0.0.78/examples/examples-by-ml-library/libraries/catboost_example.py
--rw-r--r--   0 neallathia   (501) staff       (20)     1140 2022-04-15 00:22:02.000000 modelstore-0.0.78/examples/examples-by-ml-library/libraries/fastai_example.py
--rw-r--r--   0 neallathia   (501) staff       (20)     1391 2022-04-15 00:22:02.000000 modelstore-0.0.78/examples/examples-by-ml-library/libraries/gensim_example.py
--rw-r--r--   0 neallathia   (501) staff       (20)     1571 2022-04-15 00:22:02.000000 modelstore-0.0.78/examples/examples-by-ml-library/libraries/keras_example.py
--rw-r--r--   0 neallathia   (501) staff       (20)     1610 2022-04-15 00:22:02.000000 modelstore-0.0.78/examples/examples-by-ml-library/libraries/lightgbm_example.py
--rw-r--r--   0 neallathia   (501) staff       (20)     1655 2022-04-15 00:22:02.000000 modelstore-0.0.78/examples/examples-by-ml-library/libraries/mxnet_example.py
--rw-r--r--   0 neallathia   (501) staff       (20)     2510 2022-04-15 00:22:02.000000 modelstore-0.0.78/examples/examples-by-ml-library/libraries/onnx_lightgbm_example.py
--rw-r--r--   0 neallathia   (501) staff       (20)     1869 2022-12-05 23:25:36.000000 modelstore-0.0.78/examples/examples-by-ml-library/libraries/onnx_sklearn_example.py
--rw-r--r--   0 neallathia   (501) staff       (20)     1432 2022-04-15 00:22:02.000000 modelstore-0.0.78/examples/examples-by-ml-library/libraries/prophet_example.py
--rw-r--r--   0 neallathia   (501) staff       (20)     2312 2022-12-17 10:26:28.000000 modelstore-0.0.78/examples/examples-by-ml-library/libraries/pyspark_example.py
--rw-r--r--   0 neallathia   (501) staff       (20)     1956 2022-04-15 00:22:02.000000 modelstore-0.0.78/examples/examples-by-ml-library/libraries/pytorch_example.py
--rw-r--r--   0 neallathia   (501) staff       (20)     2828 2022-04-15 00:22:02.000000 modelstore-0.0.78/examples/examples-by-ml-library/libraries/pytorch_lightning_example.py
--rw-r--r--   0 neallathia   (501) staff       (20)     1116 2022-04-15 00:22:02.000000 modelstore-0.0.78/examples/examples-by-ml-library/libraries/raw_file_example.py
--rw-r--r--   0 neallathia   (501) staff       (20)     1868 2022-04-15 00:22:02.000000 modelstore-0.0.78/examples/examples-by-ml-library/libraries/shap_example.py
--rw-r--r--   0 neallathia   (501) staff       (20)     1779 2022-04-15 00:22:02.000000 modelstore-0.0.78/examples/examples-by-ml-library/libraries/sklearn_example.py
--rw-r--r--   0 neallathia   (501) staff       (20)     2095 2022-04-15 00:22:02.000000 modelstore-0.0.78/examples/examples-by-ml-library/libraries/sklearn_with_explainer_example.py
--rw-r--r--   0 neallathia   (501) staff       (20)     2072 2022-04-15 00:22:02.000000 modelstore-0.0.78/examples/examples-by-ml-library/libraries/sklearn_with_extras_example.py
--rw-r--r--   0 neallathia   (501) staff       (20)     1810 2022-04-15 00:22:02.000000 modelstore-0.0.78/examples/examples-by-ml-library/libraries/skorch_example.py
--rw-r--r--   0 neallathia   (501) staff       (20)     1635 2022-04-15 00:22:02.000000 modelstore-0.0.78/examples/examples-by-ml-library/libraries/tensorflow_example.py
--rw-r--r--   0 neallathia   (501) staff       (20)     1617 2022-04-15 00:22:02.000000 modelstore-0.0.78/examples/examples-by-ml-library/libraries/transformers_example.py
-drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-03-11 17:52:34.418788 modelstore-0.0.78/examples/examples-by-ml-library/libraries/util/
--rw-r--r--   0 neallathia   (501) staff       (20)     1748 2022-12-05 22:53:38.000000 modelstore-0.0.78/examples/examples-by-ml-library/libraries/util/datasets.py
--rw-r--r--   0 neallathia   (501) staff       (20)      141 2022-12-05 23:20:42.000000 modelstore-0.0.78/examples/examples-by-ml-library/libraries/util/domains.py
--rw-r--r--   0 neallathia   (501) staff       (20)     1592 2022-05-21 09:54:03.000000 modelstore-0.0.78/examples/examples-by-ml-library/libraries/xgboost_booster_example.py
--rw-r--r--   0 neallathia   (501) staff       (20)     1519 2022-04-15 00:22:02.000000 modelstore-0.0.78/examples/examples-by-ml-library/libraries/xgboost_example.py
--rw-r--r--   0 neallathia   (501) staff       (20)     2862 2023-03-05 21:12:21.000000 modelstore-0.0.78/examples/examples-by-ml-library/main.py
--rw-r--r--   0 neallathia   (501) staff       (20)     3290 2022-12-17 10:26:28.000000 modelstore-0.0.78/examples/examples-by-ml-library/modelstores.py
--rw-r--r--   0 neallathia   (501) staff       (20)      659 2023-03-05 19:21:58.000000 modelstore-0.0.78/examples/examples-by-ml-library/requirements.txt
--rwxr-xr-x   0 neallathia   (501) staff       (20)      643 2023-03-05 21:12:21.000000 modelstore-0.0.78/examples/examples-by-ml-library/run-all.sh
-drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-03-11 17:52:34.421933 modelstore-0.0.78/modelstore/
--rw-r--r--   0 neallathia   (501) staff       (20)      236 2022-01-13 15:38:40.000000 modelstore-0.0.78/modelstore/__init__.py
--rw-r--r--   0 neallathia   (501) staff       (20)     2601 2022-09-08 11:52:33.000000 modelstore-0.0.78/modelstore/__main__.py
-drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-03-11 17:52:34.426508 modelstore-0.0.78/modelstore/ids/
--rw-r--r--   0 neallathia   (501) staff       (20)        0 2022-04-15 14:47:26.000000 modelstore-0.0.78/modelstore/ids/__init__.py
--rw-r--r--   0 neallathia   (501) staff       (20)     1638 2022-05-08 13:46:10.000000 modelstore-0.0.78/modelstore/ids/model_ids.py
-drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-03-11 17:52:34.427642 modelstore-0.0.78/modelstore/metadata/
--rw-r--r--   0 neallathia   (501) staff       (20)        0 2022-05-25 22:34:04.000000 modelstore-0.0.78/modelstore/metadata/__init__.py
-drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-03-11 17:52:34.430216 modelstore-0.0.78/modelstore/metadata/code/
--rw-r--r--   0 neallathia   (501) staff       (20)        0 2022-05-25 22:34:04.000000 modelstore-0.0.78/modelstore/metadata/code/__init__.py
--rw-r--r--   0 neallathia   (501) staff       (20)     1937 2022-12-17 10:26:28.000000 modelstore-0.0.78/modelstore/metadata/code/code.py
--rw-r--r--   0 neallathia   (501) staff       (20)     2156 2022-12-17 10:26:28.000000 modelstore-0.0.78/modelstore/metadata/code/dependencies.py
--rw-r--r--   0 neallathia   (501) staff       (20)     1699 2022-12-17 10:26:28.000000 modelstore-0.0.78/modelstore/metadata/code/revision.py
--rw-r--r--   0 neallathia   (501) staff       (20)      936 2022-12-17 10:26:28.000000 modelstore-0.0.78/modelstore/metadata/code/runtime.py
-drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-03-11 17:52:34.432898 modelstore-0.0.78/modelstore/metadata/dataset/
--rw-r--r--   0 neallathia   (501) staff       (20)        0 2022-06-12 22:21:05.000000 modelstore-0.0.78/modelstore/metadata/dataset/__init__.py
--rw-r--r--   0 neallathia   (501) staff       (20)     1608 2022-12-17 10:26:28.000000 modelstore-0.0.78/modelstore/metadata/dataset/dataset.py
--rw-r--r--   0 neallathia   (501) staff       (20)     1715 2022-12-17 10:26:28.000000 modelstore-0.0.78/modelstore/metadata/dataset/features.py
--rw-r--r--   0 neallathia   (501) staff       (20)     2676 2022-12-17 10:26:28.000000 modelstore-0.0.78/modelstore/metadata/dataset/labels.py
--rw-r--r--   0 neallathia   (501) staff       (20)     1271 2022-12-17 10:26:28.000000 modelstore-0.0.78/modelstore/metadata/dataset/types.py
--rw-r--r--   0 neallathia   (501) staff       (20)     2853 2022-12-17 10:26:28.000000 modelstore-0.0.78/modelstore/metadata/metadata.py
-drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-03-11 17:52:34.434443 modelstore-0.0.78/modelstore/metadata/model/
--rw-r--r--   0 neallathia   (501) staff       (20)        0 2022-05-25 22:34:04.000000 modelstore-0.0.78/modelstore/metadata/model/__init__.py
--rw-r--r--   0 neallathia   (501) staff       (20)     1794 2022-12-17 10:26:28.000000 modelstore-0.0.78/modelstore/metadata/model/model.py
--rw-r--r--   0 neallathia   (501) staff       (20)     2070 2022-12-17 10:26:28.000000 modelstore-0.0.78/modelstore/metadata/model/model_type.py
-drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-03-11 17:52:34.435354 modelstore-0.0.78/modelstore/metadata/storage/
--rw-r--r--   0 neallathia   (501) staff       (20)        0 2022-05-25 22:34:04.000000 modelstore-0.0.78/modelstore/metadata/storage/__init__.py
--rw-r--r--   0 neallathia   (501) staff       (20)     2638 2022-12-17 10:26:28.000000 modelstore-0.0.78/modelstore/metadata/storage/storage.py
-drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-03-11 17:52:34.436381 modelstore-0.0.78/modelstore/metadata/utils/
--rw-r--r--   0 neallathia   (501) staff       (20)        0 2022-05-25 22:34:04.000000 modelstore-0.0.78/modelstore/metadata/utils/__init__.py
--rw-r--r--   0 neallathia   (501) staff       (20)     1544 2022-12-17 10:26:28.000000 modelstore-0.0.78/modelstore/metadata/utils/utils.py
--rw-r--r--   0 neallathia   (501) staff       (20)    13002 2023-02-19 11:42:44.000000 modelstore-0.0.78/modelstore/model_store.py
-drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-03-11 17:52:34.448570 modelstore-0.0.78/modelstore/models/
--rw-r--r--   0 neallathia   (501) staff       (20)     7775 2022-01-13 15:38:40.000000 modelstore-0.0.78/modelstore/models/CONTRIBUTING.md
--rw-r--r--   0 neallathia   (501) staff       (20)        0 2022-01-13 15:38:40.000000 modelstore-0.0.78/modelstore/models/__init__.py
--rw-r--r--   0 neallathia   (501) staff       (20)     2830 2022-12-17 10:26:28.000000 modelstore-0.0.78/modelstore/models/annoy.py
--rw-r--r--   0 neallathia   (501) staff       (20)     5348 2022-12-17 10:26:28.000000 modelstore-0.0.78/modelstore/models/catboost.py
--rw-r--r--   0 neallathia   (501) staff       (20)     1119 2022-05-08 12:34:43.000000 modelstore-0.0.78/modelstore/models/common.py
--rw-r--r--   0 neallathia   (501) staff       (20)     3895 2022-07-03 11:35:08.000000 modelstore-0.0.78/modelstore/models/fastai.py
--rw-r--r--   0 neallathia   (501) staff       (20)     3246 2022-07-03 11:35:08.000000 modelstore-0.0.78/modelstore/models/gensim.py
--rw-r--r--   0 neallathia   (501) staff       (20)     2965 2022-07-03 11:35:08.000000 modelstore-0.0.78/modelstore/models/lightgbm.py
--rw-r--r--   0 neallathia   (501) staff       (20)     3956 2023-02-07 00:36:23.000000 modelstore-0.0.78/modelstore/models/managers.py
--rw-r--r--   0 neallathia   (501) staff       (20)     2241 2022-06-12 22:21:05.000000 modelstore-0.0.78/modelstore/models/missing_manager.py
--rw-r--r--   0 neallathia   (501) staff       (20)     3154 2022-12-17 10:26:28.000000 modelstore-0.0.78/modelstore/models/model_file.py
--rw-r--r--   0 neallathia   (501) staff       (20)     9070 2023-02-11 15:06:42.000000 modelstore-0.0.78/modelstore/models/model_manager.py
--rw-r--r--   0 neallathia   (501) staff       (20)     2903 2022-12-17 10:26:28.000000 modelstore-0.0.78/modelstore/models/multiple_models.py
--rw-r--r--   0 neallathia   (501) staff       (20)     3743 2022-07-03 11:35:08.000000 modelstore-0.0.78/modelstore/models/mxnet.py
--rw-r--r--   0 neallathia   (501) staff       (20)     2784 2022-07-03 11:35:08.000000 modelstore-0.0.78/modelstore/models/onnx.py
--rw-r--r--   0 neallathia   (501) staff       (20)     3236 2023-02-11 15:06:42.000000 modelstore-0.0.78/modelstore/models/prophet.py
--rw-r--r--   0 neallathia   (501) staff       (20)     4234 2022-12-17 10:26:28.000000 modelstore-0.0.78/modelstore/models/pyspark.py
--rw-r--r--   0 neallathia   (501) staff       (20)     4907 2022-07-03 11:35:08.000000 modelstore-0.0.78/modelstore/models/pytorch.py
--rw-r--r--   0 neallathia   (501) staff       (20)     3607 2022-07-03 11:35:08.000000 modelstore-0.0.78/modelstore/models/pytorch_lightning.py
--rw-r--r--   0 neallathia   (501) staff       (20)     2356 2022-12-17 10:26:28.000000 modelstore-0.0.78/modelstore/models/shap.py
--rw-r--r--   0 neallathia   (501) staff       (20)     4538 2022-07-03 11:35:08.000000 modelstore-0.0.78/modelstore/models/sklearn.py
--rw-r--r--   0 neallathia   (501) staff       (20)     3121 2022-07-03 11:35:08.000000 modelstore-0.0.78/modelstore/models/skorch.py
--rw-r--r--   0 neallathia   (501) staff       (20)     2968 2022-07-03 11:35:08.000000 modelstore-0.0.78/modelstore/models/tensorflow.py
--rw-r--r--   0 neallathia   (501) staff       (20)     3837 2022-07-03 11:35:08.000000 modelstore-0.0.78/modelstore/models/transformers.py
--rw-r--r--   0 neallathia   (501) staff       (20)     1556 2022-05-08 13:46:10.000000 modelstore-0.0.78/modelstore/models/util.py
--rw-r--r--   0 neallathia   (501) staff       (20)     4662 2022-12-17 10:26:28.000000 modelstore-0.0.78/modelstore/models/xgboost.py
-drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-03-11 17:52:34.451687 modelstore-0.0.78/modelstore/storage/
--rw-r--r--   0 neallathia   (501) staff       (20)     3470 2022-01-13 15:38:40.000000 modelstore-0.0.78/modelstore/storage/CONTRIBUTING.md
--rw-r--r--   0 neallathia   (501) staff       (20)        0 2022-01-13 15:38:40.000000 modelstore-0.0.78/modelstore/storage/__init__.py
--rw-r--r--   0 neallathia   (501) staff       (20)     6039 2022-12-17 10:26:28.000000 modelstore-0.0.78/modelstore/storage/aws.py
--rw-r--r--   0 neallathia   (501) staff       (20)     6808 2022-12-17 10:26:28.000000 modelstore-0.0.78/modelstore/storage/azure.py
--rw-r--r--   0 neallathia   (501) staff       (20)    15166 2022-12-17 10:26:28.000000 modelstore-0.0.78/modelstore/storage/blob_storage.py
--rw-r--r--   0 neallathia   (501) staff       (20)     9828 2022-12-17 10:26:28.000000 modelstore-0.0.78/modelstore/storage/gcloud.py
--rw-r--r--   0 neallathia   (501) staff       (20)     6651 2022-12-17 10:26:28.000000 modelstore-0.0.78/modelstore/storage/local.py
--rw-r--r--   0 neallathia   (501) staff       (20)     6720 2023-02-19 11:42:44.000000 modelstore-0.0.78/modelstore/storage/minio.py
-drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-03-11 17:52:34.452223 modelstore-0.0.78/modelstore/storage/states/
--rw-r--r--   0 neallathia   (501) staff       (20)        0 2022-02-20 17:43:37.000000 modelstore-0.0.78/modelstore/storage/states/__init__.py
--rw-r--r--   0 neallathia   (501) staff       (20)     1452 2022-05-08 13:46:10.000000 modelstore-0.0.78/modelstore/storage/states/model_states.py
--rw-r--r--   0 neallathia   (501) staff       (20)     3940 2022-12-17 10:26:28.000000 modelstore-0.0.78/modelstore/storage/storage.py
-drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-03-11 17:52:34.453518 modelstore-0.0.78/modelstore/storage/util/
--rw-r--r--   0 neallathia   (501) staff       (20)        0 2022-01-13 15:38:40.000000 modelstore-0.0.78/modelstore/storage/util/__init__.py
--rw-r--r--   0 neallathia   (501) staff       (20)     1382 2022-05-08 13:46:10.000000 modelstore-0.0.78/modelstore/storage/util/environment.py
--rw-r--r--   0 neallathia   (501) staff       (20)     4456 2022-12-17 10:26:28.000000 modelstore-0.0.78/modelstore/storage/util/paths.py
--rw-r--r--   0 neallathia   (501) staff       (20)     1147 2022-05-08 13:46:10.000000 modelstore-0.0.78/modelstore/storage/util/versions.py
-drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-03-11 17:52:34.454580 modelstore-0.0.78/modelstore/utils/
--rw-r--r--   0 neallathia   (501) staff       (20)        0 2022-01-13 15:38:40.000000 modelstore-0.0.78/modelstore/utils/__init__.py
--rw-r--r--   0 neallathia   (501) staff       (20)     3555 2022-12-03 00:48:26.000000 modelstore-0.0.78/modelstore/utils/cli.py
--rw-r--r--   0 neallathia   (501) staff       (20)     1917 2022-05-08 13:46:10.000000 modelstore-0.0.78/modelstore/utils/exceptions.py
--rw-r--r--   0 neallathia   (501) staff       (20)      982 2023-02-13 23:42:08.000000 modelstore-0.0.78/modelstore/utils/log.py
-drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-03-11 17:52:34.425573 modelstore-0.0.78/modelstore.egg-info/
--rw-r--r--   0 neallathia   (501) staff       (20)      685 2023-03-11 17:52:34.000000 modelstore-0.0.78/modelstore.egg-info/PKG-INFO
--rw-r--r--   0 neallathia   (501) staff       (20)     7537 2023-03-11 17:52:34.000000 modelstore-0.0.78/modelstore.egg-info/SOURCES.txt
--rw-r--r--   0 neallathia   (501) staff       (20)        1 2023-03-11 17:52:34.000000 modelstore-0.0.78/modelstore.egg-info/dependency_links.txt
--rw-r--r--   0 neallathia   (501) staff       (20)      147 2023-03-11 17:52:34.000000 modelstore-0.0.78/modelstore.egg-info/requires.txt
--rw-r--r--   0 neallathia   (501) staff       (20)       17 2023-03-11 17:52:34.000000 modelstore-0.0.78/modelstore.egg-info/top_level.txt
--rw-r--r--   0 neallathia   (501) staff       (20)      367 2022-01-13 15:38:40.000000 modelstore-0.0.78/pytest.ini
--rw-r--r--   0 neallathia   (501) staff       (20)      436 2023-02-11 15:06:42.000000 modelstore-0.0.78/requirements-dev0.txt
--rw-r--r--   0 neallathia   (501) staff       (20)      792 2023-02-11 15:06:42.000000 modelstore-0.0.78/requirements-dev1.txt
--rw-r--r--   0 neallathia   (501) staff       (20)      144 2022-05-25 22:34:04.000000 modelstore-0.0.78/requirements.txt
--rw-r--r--   0 neallathia   (501) staff       (20)       38 2023-03-11 17:52:34.523929 modelstore-0.0.78/setup.cfg
--rw-r--r--   0 neallathia   (501) staff       (20)     1096 2023-03-11 17:42:37.000000 modelstore-0.0.78/setup.py
-drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-03-11 17:52:34.456156 modelstore-0.0.78/tests/
--rw-r--r--   0 neallathia   (501) staff       (20)        0 2022-01-13 15:38:40.000000 modelstore-0.0.78/tests/__init__.py
-drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-03-11 17:52:34.456818 modelstore-0.0.78/tests/ids/
--rw-r--r--   0 neallathia   (501) staff       (20)        0 2022-04-15 14:47:26.000000 modelstore-0.0.78/tests/ids/__init__.py
--rw-r--r--   0 neallathia   (501) staff       (20)     1336 2022-05-25 22:34:04.000000 modelstore-0.0.78/tests/ids/test_model_ids.py
-drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-03-11 17:52:34.457366 modelstore-0.0.78/tests/metadata/
--rw-r--r--   0 neallathia   (501) staff       (20)        0 2022-05-25 22:34:04.000000 modelstore-0.0.78/tests/metadata/__init__.py
-drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-03-11 17:52:34.460568 modelstore-0.0.78/tests/metadata/code/
--rw-r--r--   0 neallathia   (501) staff       (20)        0 2022-05-25 22:34:04.000000 modelstore-0.0.78/tests/metadata/code/__init__.py
--rw-r--r--   0 neallathia   (501) staff       (20)     1746 2022-12-17 10:26:28.000000 modelstore-0.0.78/tests/metadata/code/test_code.py
--rw-r--r--   0 neallathia   (501) staff       (20)     1541 2022-12-17 10:26:28.000000 modelstore-0.0.78/tests/metadata/code/test_dependencies.py
--rw-r--r--   0 neallathia   (501) staff       (20)     1710 2022-05-25 22:34:04.000000 modelstore-0.0.78/tests/metadata/code/test_revision.py
--rw-r--r--   0 neallathia   (501) staff       (20)     1115 2022-07-03 11:35:08.000000 modelstore-0.0.78/tests/metadata/code/test_runtime.py
-drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-03-11 17:52:34.465299 modelstore-0.0.78/tests/metadata/dataset/
--rw-r--r--   0 neallathia   (501) staff       (20)        0 2022-06-12 22:21:05.000000 modelstore-0.0.78/tests/metadata/dataset/__init__.py
--rw-r--r--   0 neallathia   (501) staff       (20)     1123 2022-06-12 22:21:05.000000 modelstore-0.0.78/tests/metadata/dataset/fixtures.py
--rw-r--r--   0 neallathia   (501) staff       (20)     1516 2022-12-17 10:26:28.000000 modelstore-0.0.78/tests/metadata/dataset/test_dataset.py
--rw-r--r--   0 neallathia   (501) staff       (20)     1386 2022-12-17 10:26:28.000000 modelstore-0.0.78/tests/metadata/dataset/test_features.py
--rw-r--r--   0 neallathia   (501) staff       (20)     1577 2022-12-17 10:26:28.000000 modelstore-0.0.78/tests/metadata/dataset/test_labels.py
--rw-r--r--   0 neallathia   (501) staff       (20)     1716 2022-12-17 10:26:28.000000 modelstore-0.0.78/tests/metadata/dataset/test_types.py
-drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-03-11 17:52:34.467315 modelstore-0.0.78/tests/metadata/model/
--rw-r--r--   0 neallathia   (501) staff       (20)        0 2022-05-25 22:34:04.000000 modelstore-0.0.78/tests/metadata/model/__init__.py
--rw-r--r--   0 neallathia   (501) staff       (20)     1421 2022-12-17 10:26:28.000000 modelstore-0.0.78/tests/metadata/model/test_model.py
--rw-r--r--   0 neallathia   (501) staff       (20)     2271 2022-12-17 10:26:28.000000 modelstore-0.0.78/tests/metadata/model/test_model_type.py
-drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-03-11 17:52:34.468613 modelstore-0.0.78/tests/metadata/storage/
--rw-r--r--   0 neallathia   (501) staff       (20)        0 2022-05-25 22:34:04.000000 modelstore-0.0.78/tests/metadata/storage/__init__.py
--rw-r--r--   0 neallathia   (501) staff       (20)     2069 2022-12-17 10:26:28.000000 modelstore-0.0.78/tests/metadata/storage/test_storage.py
--rw-r--r--   0 neallathia   (501) staff       (20)     2706 2022-12-17 10:26:28.000000 modelstore-0.0.78/tests/metadata/test_metadata.py
-drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-03-11 17:52:34.469727 modelstore-0.0.78/tests/metadata/utils/
--rw-r--r--   0 neallathia   (501) staff       (20)        0 2022-05-25 22:34:04.000000 modelstore-0.0.78/tests/metadata/utils/__init__.py
--rw-r--r--   0 neallathia   (501) staff       (20)     1866 2022-12-17 10:26:28.000000 modelstore-0.0.78/tests/metadata/utils/test_utils.py
-drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-03-11 17:52:34.490808 modelstore-0.0.78/tests/models/
--rw-r--r--   0 neallathia   (501) staff       (20)        0 2022-01-13 15:38:40.000000 modelstore-0.0.78/tests/models/__init__.py
--rw-r--r--   0 neallathia   (501) staff       (20)     3567 2022-06-12 22:21:05.000000 modelstore-0.0.78/tests/models/test_annoy.py
--rw-r--r--   0 neallathia   (501) staff       (20)     4216 2022-06-12 22:21:05.000000 modelstore-0.0.78/tests/models/test_catboost.py
--rw-r--r--   0 neallathia   (501) staff       (20)     1424 2022-06-12 21:52:40.000000 modelstore-0.0.78/tests/models/test_common.py
--rw-r--r--   0 neallathia   (501) staff       (20)     5098 2023-03-11 17:40:56.000000 modelstore-0.0.78/tests/models/test_fastai.py
--rw-r--r--   0 neallathia   (501) staff       (20)     3449 2022-12-17 10:26:28.000000 modelstore-0.0.78/tests/models/test_gensim.py
--rw-r--r--   0 neallathia   (501) staff       (20)     4143 2022-06-12 22:21:05.000000 modelstore-0.0.78/tests/models/test_lightgbm.py
--rw-r--r--   0 neallathia   (501) staff       (20)     2571 2022-12-17 10:26:28.000000 modelstore-0.0.78/tests/models/test_managers.py
--rw-r--r--   0 neallathia   (501) staff       (20)     1302 2022-05-25 22:34:04.000000 modelstore-0.0.78/tests/models/test_missing_manager.py
--rw-r--r--   0 neallathia   (501) staff       (20)     2627 2022-06-12 22:21:05.000000 modelstore-0.0.78/tests/models/test_model_file.py
--rw-r--r--   0 neallathia   (501) staff       (20)     6166 2022-07-03 11:35:08.000000 modelstore-0.0.78/tests/models/test_model_manager.py
--rw-r--r--   0 neallathia   (501) staff       (20)     4993 2022-12-17 10:26:28.000000 modelstore-0.0.78/tests/models/test_multiple_models.py
--rw-r--r--   0 neallathia   (501) staff       (20)     3659 2022-06-12 22:21:05.000000 modelstore-0.0.78/tests/models/test_mxnet.py
--rw-r--r--   0 neallathia   (501) staff       (20)     4082 2022-06-12 22:21:05.000000 modelstore-0.0.78/tests/models/test_onnx.py
--rw-r--r--   0 neallathia   (501) staff       (20)     3856 2022-06-12 22:21:05.000000 modelstore-0.0.78/tests/models/test_prophet.py
--rw-r--r--   0 neallathia   (501) staff       (20)     4185 2022-12-17 10:26:28.000000 modelstore-0.0.78/tests/models/test_pyspark.py
--rw-r--r--   0 neallathia   (501) staff       (20)     4648 2022-06-12 22:21:05.000000 modelstore-0.0.78/tests/models/test_pytorch.py
--rw-r--r--   0 neallathia   (501) staff       (20)     5347 2022-06-12 22:21:05.000000 modelstore-0.0.78/tests/models/test_pytorch_lightning.py
--rw-r--r--   0 neallathia   (501) staff       (20)     3662 2022-06-12 22:21:05.000000 modelstore-0.0.78/tests/models/test_shap.py
--rw-r--r--   0 neallathia   (501) staff       (20)     5420 2022-12-17 10:26:28.000000 modelstore-0.0.78/tests/models/test_sklearn.py
--rw-r--r--   0 neallathia   (501) staff       (20)     3942 2022-06-12 22:21:05.000000 modelstore-0.0.78/tests/models/test_skorch.py
--rw-r--r--   0 neallathia   (501) staff       (20)     4664 2022-06-12 22:21:05.000000 modelstore-0.0.78/tests/models/test_tensorflow.py
--rw-r--r--   0 neallathia   (501) staff       (20)     4415 2022-12-17 10:26:28.000000 modelstore-0.0.78/tests/models/test_transformers.py
--rw-r--r--   0 neallathia   (501) staff       (20)     6108 2022-12-17 10:26:28.000000 modelstore-0.0.78/tests/models/test_xgboost.py
--rw-r--r--   0 neallathia   (501) staff       (20)     1519 2023-03-11 17:40:56.000000 modelstore-0.0.78/tests/models/utils.py
-drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-03-11 17:52:34.500741 modelstore-0.0.78/tests/storage/
--rw-r--r--   0 neallathia   (501) staff       (20)        0 2022-01-13 15:38:40.000000 modelstore-0.0.78/tests/storage/__init__.py
-drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-03-11 17:52:34.502397 modelstore-0.0.78/tests/storage/states/
--rw-r--r--   0 neallathia   (501) staff       (20)        0 2022-02-20 17:43:37.000000 modelstore-0.0.78/tests/storage/states/__init__.py
--rw-r--r--   0 neallathia   (501) staff       (20)     1281 2022-05-08 13:46:10.000000 modelstore-0.0.78/tests/storage/states/test_model_states.py
--rw-r--r--   0 neallathia   (501) staff       (20)     5982 2022-12-17 10:26:28.000000 modelstore-0.0.78/tests/storage/test_aws.py
--rw-r--r--   0 neallathia   (501) staff       (20)     9263 2022-12-17 10:26:28.000000 modelstore-0.0.78/tests/storage/test_azure.py
--rw-r--r--   0 neallathia   (501) staff       (20)     1828 2022-12-17 10:26:28.000000 modelstore-0.0.78/tests/storage/test_blob_storage.py
--rw-r--r--   0 neallathia   (501) staff       (20)     3190 2022-11-05 16:00:49.000000 modelstore-0.0.78/tests/storage/test_blob_storage_artifacts.py
--rw-r--r--   0 neallathia   (501) staff       (20)     3732 2022-12-03 00:48:26.000000 modelstore-0.0.78/tests/storage/test_blob_storage_meta_data.py
--rw-r--r--   0 neallathia   (501) staff       (20)     5172 2022-05-25 22:34:04.000000 modelstore-0.0.78/tests/storage/test_blob_storage_states.py
--rw-r--r--   0 neallathia   (501) staff       (20)    10049 2022-12-17 10:26:28.000000 modelstore-0.0.78/tests/storage/test_gcloud.py
--rw-r--r--   0 neallathia   (501) staff       (20)     6350 2022-12-17 10:26:28.000000 modelstore-0.0.78/tests/storage/test_local.py
--rw-r--r--   0 neallathia   (501) staff       (20)     5518 2022-12-17 10:26:28.000000 modelstore-0.0.78/tests/storage/test_minio.py
--rw-r--r--   0 neallathia   (501) staff       (20)     2504 2022-12-17 10:26:28.000000 modelstore-0.0.78/tests/storage/test_utils.py
-drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-03-11 17:52:34.503992 modelstore-0.0.78/tests/storage/util/
--rw-r--r--   0 neallathia   (501) staff       (20)        0 2022-01-13 15:38:40.000000 modelstore-0.0.78/tests/storage/util/__init__.py
--rw-r--r--   0 neallathia   (501) staff       (20)     4361 2022-12-17 10:26:28.000000 modelstore-0.0.78/tests/storage/util/test_paths.py
--rw-r--r--   0 neallathia   (501) staff       (20)     3814 2022-12-17 10:26:28.000000 modelstore-0.0.78/tests/test_model_store.py
--rw-r--r--   0 neallathia   (501) staff       (20)     3323 2023-02-11 15:06:42.000000 modelstore-0.0.78/tests/test_model_store_filesystem.py
--rw-r--r--   0 neallathia   (501) staff       (20)     1777 2022-07-03 11:35:08.000000 modelstore-0.0.78/tests/test_model_store_gcp.py
--rw-r--r--   0 neallathia   (501) staff       (20)     2201 2023-02-07 00:37:01.000000 modelstore-0.0.78/tests/test_utils.py
-drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-03-11 17:52:34.508138 modelstore-0.0.78/workflows/
--rw-r--r--   0 neallathia   (501) staff       (20)      640 2023-02-19 11:42:44.000000 modelstore-0.0.78/workflows/Makefile
-drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-03-11 17:52:34.514143 modelstore-0.0.78/workflows/actions/
--rw-r--r--   0 neallathia   (501) staff       (20)        0 2022-06-25 18:07:50.000000 modelstore-0.0.78/workflows/actions/__init__.py
--rw-r--r--   0 neallathia   (501) staff       (20)     1917 2022-12-17 10:26:28.000000 modelstore-0.0.78/workflows/actions/actions.py
--rw-r--r--   0 neallathia   (501) staff       (20)     1910 2022-12-17 10:26:28.000000 modelstore-0.0.78/workflows/actions/cli.py
--rw-r--r--   0 neallathia   (501) staff       (20)     5143 2022-12-17 10:26:28.000000 modelstore-0.0.78/workflows/actions/models.py
--rw-r--r--   0 neallathia   (501) staff       (20)     1788 2022-12-17 10:26:28.000000 modelstore-0.0.78/workflows/actions/storage.py
-drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-03-11 17:52:34.516291 modelstore-0.0.78/workflows/fixtures/
--rw-r--r--   0 neallathia   (501) staff       (20)        0 2022-06-25 18:07:50.000000 modelstore-0.0.78/workflows/fixtures/__init__.py
--rw-r--r--   0 neallathia   (501) staff       (20)     1433 2022-12-17 10:26:28.000000 modelstore-0.0.78/workflows/fixtures/extra.py
--rw-r--r--   0 neallathia   (501) staff       (20)     2058 2023-02-11 15:06:42.000000 modelstore-0.0.78/workflows/fixtures/models.py
--rw-r--r--   0 neallathia   (501) staff       (20)     3070 2022-12-17 10:26:28.000000 modelstore-0.0.78/workflows/fixtures/modelstores.py
--rw-r--r--   0 neallathia   (501) staff       (20)     2430 2023-02-19 11:42:44.000000 modelstore-0.0.78/workflows/main.py
-drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-03-11 17:52:34.520457 modelstore-0.0.78/workflows/requirements/
--rw-r--r--   0 neallathia   (501) staff       (20)       14 2022-09-08 11:52:33.000000 modelstore-0.0.78/workflows/requirements/aws-s3.txt
--rw-r--r--   0 neallathia   (501) staff       (20)       45 2022-09-08 11:52:33.000000 modelstore-0.0.78/workflows/requirements/azure-container.txt
--rw-r--r--   0 neallathia   (501) staff       (20)        0 2022-06-25 18:07:50.000000 modelstore-0.0.78/workflows/requirements/filesystem.txt
--rw-r--r--   0 neallathia   (501) staff       (20)      104 2022-09-08 11:52:33.000000 modelstore-0.0.78/workflows/requirements/google-cloud-storage.txt
--rw-r--r--   0 neallathia   (501) staff       (20)       13 2022-12-03 00:48:26.000000 modelstore-0.0.78/workflows/requirements/minio.txt
--rw-r--r--   0 neallathia   (501) staff       (20)       48 2023-02-11 15:06:42.000000 modelstore-0.0.78/workflows/requirements.txt
+drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-06-09 14:53:14.761871 modelstore-0.0.79/
+drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-06-09 14:53:14.621928 modelstore-0.0.79/.github/
+drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-06-09 14:53:14.640371 modelstore-0.0.79/.github/workflows/
+-rw-r--r--   0 neallathia   (501) staff       (20)     2296 2022-12-02 10:38:39.000000 modelstore-0.0.79/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 neallathia   (501) staff       (20)     2024 2022-12-03 00:48:26.000000 modelstore-0.0.79/.github/workflows/integration-tests.yml
+-rw-r--r--   0 neallathia   (501) staff       (20)      716 2023-03-05 21:12:21.000000 modelstore-0.0.79/.github/workflows/unit-tests.yml
+-rw-r--r--   0 neallathia   (501) staff       (20)      189 2023-03-05 21:12:21.000000 modelstore-0.0.79/.gitignore
+-rw-r--r--   0 neallathia   (501) staff       (20)    13166 2023-06-09 08:48:24.000000 modelstore-0.0.79/CHANGELOG.md
+-rw-r--r--   0 neallathia   (501) staff       (20)     5223 2022-01-13 15:38:40.000000 modelstore-0.0.79/CODE_OF_CONDUCT.md
+-rw-r--r--   0 neallathia   (501) staff       (20)     4548 2023-03-19 19:25:32.000000 modelstore-0.0.79/CONTRIBUTING.md
+-rw-r--r--   0 neallathia   (501) staff       (20)    11342 2022-01-13 15:38:40.000000 modelstore-0.0.79/LICENSE
+-rw-r--r--   0 neallathia   (501) staff       (20)      451 2023-02-11 15:06:42.000000 modelstore-0.0.79/Makefile
+-rw-r--r--   0 neallathia   (501) staff       (20)      685 2023-06-09 14:53:14.761493 modelstore-0.0.79/PKG-INFO
+-rw-r--r--   0 neallathia   (501) staff       (20)     7392 2023-03-19 19:25:32.000000 modelstore-0.0.79/README.md
+drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-06-09 14:53:14.645691 modelstore-0.0.79/bin/
+-rwxr-xr-x   0 neallathia   (501) staff       (20)      684 2023-06-08 11:33:57.000000 modelstore-0.0.79/bin/_brew_install
+-rwxr-xr-x   0 neallathia   (501) staff       (20)      277 2022-12-17 10:26:28.000000 modelstore-0.0.79/bin/_build_library
+-rwxr-xr-x   0 neallathia   (501) staff       (20)      222 2022-12-17 10:26:28.000000 modelstore-0.0.79/bin/_cleanup
+-rwxr-xr-x   0 neallathia   (501) staff       (20)      262 2023-06-08 11:33:57.000000 modelstore-0.0.79/bin/_pyenv_config
+-rwxr-xr-x   0 neallathia   (501) staff       (20)      758 2023-03-12 00:03:54.000000 modelstore-0.0.79/bin/_pyenv_install
+-rwxr-xr-x   0 neallathia   (501) staff       (20)      466 2023-02-11 15:06:42.000000 modelstore-0.0.79/bin/_pyenv_uninstall
+-rwxr-xr-x   0 neallathia   (501) staff       (20)      225 2022-12-17 10:26:28.000000 modelstore-0.0.79/bin/_release_prod
+-rwxr-xr-x   0 neallathia   (501) staff       (20)      251 2022-12-17 10:26:28.000000 modelstore-0.0.79/bin/_release_test
+drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-06-09 14:53:14.646748 modelstore-0.0.79/examples/
+-rw-r--r--   0 neallathia   (501) staff       (20)      971 2023-03-05 21:12:21.000000 modelstore-0.0.79/examples/Makefile-example
+-rw-r--r--   0 neallathia   (501) staff       (20)     2346 2022-01-13 15:38:40.000000 modelstore-0.0.79/examples/README.md
+drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-06-09 14:53:14.650120 modelstore-0.0.79/examples/cli-examples/
+-rw-r--r--   0 neallathia   (501) staff       (20)       32 2022-01-13 15:38:40.000000 modelstore-0.0.79/examples/cli-examples/.gitignore
+-rw-r--r--   0 neallathia   (501) staff       (20)       61 2022-01-13 15:38:40.000000 modelstore-0.0.79/examples/cli-examples/Makefile
+-rw-r--r--   0 neallathia   (501) staff       (20)     1615 2023-03-19 20:28:18.000000 modelstore-0.0.79/examples/cli-examples/model.py
+-rw-r--r--   0 neallathia   (501) staff       (20)       13 2022-12-17 13:52:20.000000 modelstore-0.0.79/examples/cli-examples/requirements.txt
+-rwxr-xr-x   0 neallathia   (501) staff       (20)      497 2022-01-13 15:38:40.000000 modelstore-0.0.79/examples/cli-examples/run-all.sh
+drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-06-09 14:53:14.653032 modelstore-0.0.79/examples/examples-by-ml-library/
+-rw-r--r--   0 neallathia   (501) staff       (20)       62 2022-04-15 16:06:05.000000 modelstore-0.0.79/examples/examples-by-ml-library/Makefile
+drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-06-09 14:53:14.667285 modelstore-0.0.79/examples/examples-by-ml-library/libraries/
+-rw-r--r--   0 neallathia   (501) staff       (20)        0 2022-01-13 15:38:40.000000 modelstore-0.0.79/examples/examples-by-ml-library/libraries/__init__.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     2077 2023-03-19 20:28:18.000000 modelstore-0.0.79/examples/examples-by-ml-library/libraries/annoy_example.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     2054 2023-03-19 20:28:18.000000 modelstore-0.0.79/examples/examples-by-ml-library/libraries/catboost_example.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     1746 2023-03-19 20:28:18.000000 modelstore-0.0.79/examples/examples-by-ml-library/libraries/fastai_example.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     1997 2023-03-19 20:28:18.000000 modelstore-0.0.79/examples/examples-by-ml-library/libraries/gensim_example.py
+drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-06-09 14:53:14.670855 modelstore-0.0.79/examples/examples-by-ml-library/libraries/huggingface/
+-rw-r--r--   0 neallathia   (501) staff       (20)        0 2023-05-06 22:45:07.000000 modelstore-0.0.79/examples/examples-by-ml-library/libraries/huggingface/__init__.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     2224 2023-05-06 22:45:07.000000 modelstore-0.0.79/examples/examples-by-ml-library/libraries/huggingface/distilbert.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     1971 2023-05-29 21:43:35.000000 modelstore-0.0.79/examples/examples-by-ml-library/libraries/huggingface/dpt.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     2001 2023-05-06 22:45:07.000000 modelstore-0.0.79/examples/examples-by-ml-library/libraries/huggingface/gpt2_pytorch.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     1997 2023-05-06 22:45:07.000000 modelstore-0.0.79/examples/examples-by-ml-library/libraries/huggingface/gpt2_tensorflow.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     1897 2023-05-06 22:45:07.000000 modelstore-0.0.79/examples/examples-by-ml-library/libraries/huggingface/sam.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     2177 2023-03-19 20:28:18.000000 modelstore-0.0.79/examples/examples-by-ml-library/libraries/keras_example.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     2216 2023-03-19 20:28:18.000000 modelstore-0.0.79/examples/examples-by-ml-library/libraries/lightgbm_example.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     2261 2023-03-19 20:28:18.000000 modelstore-0.0.79/examples/examples-by-ml-library/libraries/mxnet_example.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     3116 2023-03-19 20:28:18.000000 modelstore-0.0.79/examples/examples-by-ml-library/libraries/onnx_lightgbm_example.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     2475 2023-03-19 20:28:18.000000 modelstore-0.0.79/examples/examples-by-ml-library/libraries/onnx_sklearn_example.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     2038 2023-03-19 20:28:18.000000 modelstore-0.0.79/examples/examples-by-ml-library/libraries/prophet_example.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     2918 2023-03-19 20:28:18.000000 modelstore-0.0.79/examples/examples-by-ml-library/libraries/pyspark_example.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     2562 2023-03-19 20:28:18.000000 modelstore-0.0.79/examples/examples-by-ml-library/libraries/pytorch_example.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     3434 2023-03-19 20:28:18.000000 modelstore-0.0.79/examples/examples-by-ml-library/libraries/pytorch_lightning_example.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     1722 2023-03-19 20:28:18.000000 modelstore-0.0.79/examples/examples-by-ml-library/libraries/raw_file_example.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     2474 2023-03-19 20:28:18.000000 modelstore-0.0.79/examples/examples-by-ml-library/libraries/shap_example.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     2396 2023-03-19 20:28:18.000000 modelstore-0.0.79/examples/examples-by-ml-library/libraries/sklearn_example.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     2663 2023-03-19 20:28:18.000000 modelstore-0.0.79/examples/examples-by-ml-library/libraries/sklearn_with_explainer_example.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     2689 2023-03-19 20:28:18.000000 modelstore-0.0.79/examples/examples-by-ml-library/libraries/sklearn_with_extras_example.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     2416 2023-03-19 20:28:18.000000 modelstore-0.0.79/examples/examples-by-ml-library/libraries/skorch_example.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     2241 2023-03-19 20:28:18.000000 modelstore-0.0.79/examples/examples-by-ml-library/libraries/tensorflow_example.py
+drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-06-09 14:53:14.671762 modelstore-0.0.79/examples/examples-by-ml-library/libraries/util/
+-rw-r--r--   0 neallathia   (501) staff       (20)     2353 2023-03-19 20:28:18.000000 modelstore-0.0.79/examples/examples-by-ml-library/libraries/util/datasets.py
+-rw-r--r--   0 neallathia   (501) staff       (20)      747 2023-03-19 20:28:18.000000 modelstore-0.0.79/examples/examples-by-ml-library/libraries/util/domains.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     2198 2023-03-19 20:28:18.000000 modelstore-0.0.79/examples/examples-by-ml-library/libraries/xgboost_booster_example.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     2125 2023-03-19 20:28:18.000000 modelstore-0.0.79/examples/examples-by-ml-library/libraries/xgboost_example.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     1516 2023-03-19 20:28:18.000000 modelstore-0.0.79/examples/examples-by-ml-library/libraries/yolo_example.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     3761 2023-06-09 14:41:27.000000 modelstore-0.0.79/examples/examples-by-ml-library/main.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     3579 2023-06-08 18:02:17.000000 modelstore-0.0.79/examples/examples-by-ml-library/modelstores.py
+-rw-r--r--   0 neallathia   (501) staff       (20)      590 2023-06-09 10:10:35.000000 modelstore-0.0.79/examples/examples-by-ml-library/requirements.txt
+-rwxr-xr-x   0 neallathia   (501) staff       (20)      688 2023-06-09 10:31:43.000000 modelstore-0.0.79/examples/examples-by-ml-library/run-all.sh
+drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-06-09 14:53:14.673587 modelstore-0.0.79/modelstore/
+-rw-r--r--   0 neallathia   (501) staff       (20)      236 2022-01-13 15:38:40.000000 modelstore-0.0.79/modelstore/__init__.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     2601 2022-09-08 11:52:33.000000 modelstore-0.0.79/modelstore/__main__.py
+drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-06-09 14:53:14.675944 modelstore-0.0.79/modelstore/ids/
+-rw-r--r--   0 neallathia   (501) staff       (20)        0 2022-04-15 14:47:26.000000 modelstore-0.0.79/modelstore/ids/__init__.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     1638 2022-05-08 13:46:10.000000 modelstore-0.0.79/modelstore/ids/model_ids.py
+drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-06-09 14:53:14.677387 modelstore-0.0.79/modelstore/metadata/
+-rw-r--r--   0 neallathia   (501) staff       (20)        0 2022-05-25 22:34:04.000000 modelstore-0.0.79/modelstore/metadata/__init__.py
+drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-06-09 14:53:14.679643 modelstore-0.0.79/modelstore/metadata/code/
+-rw-r--r--   0 neallathia   (501) staff       (20)        0 2022-05-25 22:34:04.000000 modelstore-0.0.79/modelstore/metadata/code/__init__.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     1937 2022-12-17 10:26:28.000000 modelstore-0.0.79/modelstore/metadata/code/code.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     2156 2022-12-17 10:26:28.000000 modelstore-0.0.79/modelstore/metadata/code/dependencies.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     1699 2022-12-17 10:26:28.000000 modelstore-0.0.79/modelstore/metadata/code/revision.py
+-rw-r--r--   0 neallathia   (501) staff       (20)      936 2022-12-17 10:26:28.000000 modelstore-0.0.79/modelstore/metadata/code/runtime.py
+drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-06-09 14:53:14.682290 modelstore-0.0.79/modelstore/metadata/dataset/
+-rw-r--r--   0 neallathia   (501) staff       (20)        0 2022-06-12 22:21:05.000000 modelstore-0.0.79/modelstore/metadata/dataset/__init__.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     1638 2023-03-19 20:28:18.000000 modelstore-0.0.79/modelstore/metadata/dataset/dataset.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     1735 2023-03-19 20:28:18.000000 modelstore-0.0.79/modelstore/metadata/dataset/features.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     2706 2023-03-19 20:28:18.000000 modelstore-0.0.79/modelstore/metadata/dataset/labels.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     1271 2022-12-17 10:26:28.000000 modelstore-0.0.79/modelstore/metadata/dataset/types.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     2853 2022-12-17 10:26:28.000000 modelstore-0.0.79/modelstore/metadata/metadata.py
+drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-06-09 14:53:14.684251 modelstore-0.0.79/modelstore/metadata/model/
+-rw-r--r--   0 neallathia   (501) staff       (20)        0 2022-05-25 22:34:04.000000 modelstore-0.0.79/modelstore/metadata/model/__init__.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     1794 2022-12-17 10:26:28.000000 modelstore-0.0.79/modelstore/metadata/model/model.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     2080 2023-03-19 20:28:18.000000 modelstore-0.0.79/modelstore/metadata/model/model_type.py
+drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-06-09 14:53:14.685182 modelstore-0.0.79/modelstore/metadata/storage/
+-rw-r--r--   0 neallathia   (501) staff       (20)        0 2022-05-25 22:34:04.000000 modelstore-0.0.79/modelstore/metadata/storage/__init__.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     2638 2022-12-17 10:26:28.000000 modelstore-0.0.79/modelstore/metadata/storage/storage.py
+drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-06-09 14:53:14.685917 modelstore-0.0.79/modelstore/metadata/utils/
+-rw-r--r--   0 neallathia   (501) staff       (20)        0 2022-05-25 22:34:04.000000 modelstore-0.0.79/modelstore/metadata/utils/__init__.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     1544 2022-12-17 10:26:28.000000 modelstore-0.0.79/modelstore/metadata/utils/utils.py
+-rw-r--r--   0 neallathia   (501) staff       (20)    13481 2023-06-08 11:33:57.000000 modelstore-0.0.79/modelstore/model_store.py
+drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-06-09 14:53:14.703474 modelstore-0.0.79/modelstore/models/
+-rw-r--r--   0 neallathia   (501) staff       (20)     7775 2022-01-13 15:38:40.000000 modelstore-0.0.79/modelstore/models/CONTRIBUTING.md
+-rw-r--r--   0 neallathia   (501) staff       (20)        0 2022-01-13 15:38:40.000000 modelstore-0.0.79/modelstore/models/__init__.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     2830 2022-12-17 10:26:28.000000 modelstore-0.0.79/modelstore/models/annoy.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     5348 2022-12-17 10:26:28.000000 modelstore-0.0.79/modelstore/models/catboost.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     1119 2022-05-08 12:34:43.000000 modelstore-0.0.79/modelstore/models/common.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     3895 2022-07-03 11:35:08.000000 modelstore-0.0.79/modelstore/models/fastai.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     3246 2022-07-03 11:35:08.000000 modelstore-0.0.79/modelstore/models/gensim.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     2965 2022-07-03 11:35:08.000000 modelstore-0.0.79/modelstore/models/lightgbm.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     3956 2023-03-19 19:28:29.000000 modelstore-0.0.79/modelstore/models/managers.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     2241 2022-06-12 22:21:05.000000 modelstore-0.0.79/modelstore/models/missing_manager.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     3154 2022-12-17 10:26:28.000000 modelstore-0.0.79/modelstore/models/model_file.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     9070 2023-02-11 15:06:42.000000 modelstore-0.0.79/modelstore/models/model_manager.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     2903 2022-12-17 10:26:28.000000 modelstore-0.0.79/modelstore/models/multiple_models.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     3743 2022-07-03 11:35:08.000000 modelstore-0.0.79/modelstore/models/mxnet.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     2784 2022-07-03 11:35:08.000000 modelstore-0.0.79/modelstore/models/onnx.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     3236 2023-02-11 15:06:42.000000 modelstore-0.0.79/modelstore/models/prophet.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     4257 2023-06-08 11:33:57.000000 modelstore-0.0.79/modelstore/models/pyspark.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     4907 2022-07-03 11:35:08.000000 modelstore-0.0.79/modelstore/models/pytorch.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     3607 2022-07-03 11:35:08.000000 modelstore-0.0.79/modelstore/models/pytorch_lightning.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     2356 2022-12-17 10:26:28.000000 modelstore-0.0.79/modelstore/models/shap.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     4538 2022-07-03 11:35:08.000000 modelstore-0.0.79/modelstore/models/sklearn.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     3121 2022-07-03 11:35:08.000000 modelstore-0.0.79/modelstore/models/skorch.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     3531 2023-06-09 14:43:17.000000 modelstore-0.0.79/modelstore/models/tensorflow.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     7860 2023-06-09 14:44:29.000000 modelstore-0.0.79/modelstore/models/transformers.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     1556 2022-05-08 13:46:10.000000 modelstore-0.0.79/modelstore/models/util.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     4662 2022-12-17 10:26:28.000000 modelstore-0.0.79/modelstore/models/xgboost.py
+drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-06-09 14:53:14.709991 modelstore-0.0.79/modelstore/storage/
+-rw-r--r--   0 neallathia   (501) staff       (20)     3470 2022-01-13 15:38:40.000000 modelstore-0.0.79/modelstore/storage/CONTRIBUTING.md
+-rw-r--r--   0 neallathia   (501) staff       (20)        0 2022-01-13 15:38:40.000000 modelstore-0.0.79/modelstore/storage/__init__.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     6039 2022-12-17 10:26:28.000000 modelstore-0.0.79/modelstore/storage/aws.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     6808 2022-12-17 10:26:28.000000 modelstore-0.0.79/modelstore/storage/azure.py
+-rw-r--r--   0 neallathia   (501) staff       (20)    15166 2022-12-17 10:26:28.000000 modelstore-0.0.79/modelstore/storage/blob_storage.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     9828 2022-12-17 10:26:28.000000 modelstore-0.0.79/modelstore/storage/gcloud.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     4715 2023-06-08 18:02:17.000000 modelstore-0.0.79/modelstore/storage/hdfs.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     6651 2022-12-17 10:26:28.000000 modelstore-0.0.79/modelstore/storage/local.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     6721 2023-03-19 19:25:32.000000 modelstore-0.0.79/modelstore/storage/minio.py
+drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-06-09 14:53:14.710630 modelstore-0.0.79/modelstore/storage/states/
+-rw-r--r--   0 neallathia   (501) staff       (20)        0 2022-02-20 17:43:37.000000 modelstore-0.0.79/modelstore/storage/states/__init__.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     1452 2022-05-08 13:46:10.000000 modelstore-0.0.79/modelstore/storage/states/model_states.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     3940 2022-12-17 10:26:28.000000 modelstore-0.0.79/modelstore/storage/storage.py
+drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-06-09 14:53:14.712502 modelstore-0.0.79/modelstore/storage/util/
+-rw-r--r--   0 neallathia   (501) staff       (20)        0 2022-01-13 15:38:40.000000 modelstore-0.0.79/modelstore/storage/util/__init__.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     1382 2022-05-08 13:46:10.000000 modelstore-0.0.79/modelstore/storage/util/environment.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     4456 2022-12-17 10:26:28.000000 modelstore-0.0.79/modelstore/storage/util/paths.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     1147 2022-05-08 13:46:10.000000 modelstore-0.0.79/modelstore/storage/util/versions.py
+drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-06-09 14:53:14.714118 modelstore-0.0.79/modelstore/utils/
+-rw-r--r--   0 neallathia   (501) staff       (20)        0 2022-01-13 15:38:40.000000 modelstore-0.0.79/modelstore/utils/__init__.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     3555 2022-12-03 00:48:26.000000 modelstore-0.0.79/modelstore/utils/cli.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     1917 2022-05-08 13:46:10.000000 modelstore-0.0.79/modelstore/utils/exceptions.py
+-rw-r--r--   0 neallathia   (501) staff       (20)      982 2023-06-08 17:30:28.000000 modelstore-0.0.79/modelstore/utils/log.py
+drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-06-09 14:53:14.675405 modelstore-0.0.79/modelstore.egg-info/
+-rw-r--r--   0 neallathia   (501) staff       (20)      685 2023-06-09 14:53:14.000000 modelstore-0.0.79/modelstore.egg-info/PKG-INFO
+-rw-r--r--   0 neallathia   (501) staff       (20)     7982 2023-06-09 14:53:14.000000 modelstore-0.0.79/modelstore.egg-info/SOURCES.txt
+-rw-r--r--   0 neallathia   (501) staff       (20)        1 2023-06-09 14:53:14.000000 modelstore-0.0.79/modelstore.egg-info/dependency_links.txt
+-rw-r--r--   0 neallathia   (501) staff       (20)      147 2023-06-09 14:53:14.000000 modelstore-0.0.79/modelstore.egg-info/requires.txt
+-rw-r--r--   0 neallathia   (501) staff       (20)       17 2023-06-09 14:53:14.000000 modelstore-0.0.79/modelstore.egg-info/top_level.txt
+-rw-r--r--   0 neallathia   (501) staff       (20)      367 2022-01-13 15:38:40.000000 modelstore-0.0.79/pytest.ini
+-rw-r--r--   0 neallathia   (501) staff       (20)      436 2023-05-06 22:45:07.000000 modelstore-0.0.79/requirements-dev0.txt
+-rw-r--r--   0 neallathia   (501) staff       (20)      831 2023-06-08 11:33:57.000000 modelstore-0.0.79/requirements-dev1.txt
+-rw-r--r--   0 neallathia   (501) staff       (20)      144 2022-05-25 22:34:04.000000 modelstore-0.0.79/requirements.txt
+-rw-r--r--   0 neallathia   (501) staff       (20)       38 2023-06-09 14:53:14.761966 modelstore-0.0.79/setup.cfg
+-rw-r--r--   0 neallathia   (501) staff       (20)     1109 2023-06-09 08:51:29.000000 modelstore-0.0.79/setup.py
+drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-06-09 14:53:14.717113 modelstore-0.0.79/tests/
+-rw-r--r--   0 neallathia   (501) staff       (20)        0 2022-01-13 15:38:40.000000 modelstore-0.0.79/tests/__init__.py
+drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-06-09 14:53:14.717996 modelstore-0.0.79/tests/ids/
+-rw-r--r--   0 neallathia   (501) staff       (20)        0 2022-04-15 14:47:26.000000 modelstore-0.0.79/tests/ids/__init__.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     1336 2022-05-25 22:34:04.000000 modelstore-0.0.79/tests/ids/test_model_ids.py
+drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-06-09 14:53:14.718809 modelstore-0.0.79/tests/metadata/
+-rw-r--r--   0 neallathia   (501) staff       (20)        0 2022-05-25 22:34:04.000000 modelstore-0.0.79/tests/metadata/__init__.py
+drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-06-09 14:53:14.721267 modelstore-0.0.79/tests/metadata/code/
+-rw-r--r--   0 neallathia   (501) staff       (20)        0 2022-05-25 22:34:04.000000 modelstore-0.0.79/tests/metadata/code/__init__.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     1746 2022-12-17 10:26:28.000000 modelstore-0.0.79/tests/metadata/code/test_code.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     1541 2022-12-17 10:26:28.000000 modelstore-0.0.79/tests/metadata/code/test_dependencies.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     1710 2022-05-25 22:34:04.000000 modelstore-0.0.79/tests/metadata/code/test_revision.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     1115 2022-07-03 11:35:08.000000 modelstore-0.0.79/tests/metadata/code/test_runtime.py
+drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-06-09 14:53:14.724156 modelstore-0.0.79/tests/metadata/dataset/
+-rw-r--r--   0 neallathia   (501) staff       (20)        0 2022-06-12 22:21:05.000000 modelstore-0.0.79/tests/metadata/dataset/__init__.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     1123 2022-06-12 22:21:05.000000 modelstore-0.0.79/tests/metadata/dataset/fixtures.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     1516 2022-12-17 10:26:28.000000 modelstore-0.0.79/tests/metadata/dataset/test_dataset.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     1386 2022-12-17 10:26:28.000000 modelstore-0.0.79/tests/metadata/dataset/test_features.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     1577 2022-12-17 10:26:28.000000 modelstore-0.0.79/tests/metadata/dataset/test_labels.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     1716 2022-12-17 10:26:28.000000 modelstore-0.0.79/tests/metadata/dataset/test_types.py
+drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-06-09 14:53:14.725412 modelstore-0.0.79/tests/metadata/model/
+-rw-r--r--   0 neallathia   (501) staff       (20)        0 2022-05-25 22:34:04.000000 modelstore-0.0.79/tests/metadata/model/__init__.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     1421 2022-12-17 10:26:28.000000 modelstore-0.0.79/tests/metadata/model/test_model.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     2271 2022-12-17 10:26:28.000000 modelstore-0.0.79/tests/metadata/model/test_model_type.py
+drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-06-09 14:53:14.726124 modelstore-0.0.79/tests/metadata/storage/
+-rw-r--r--   0 neallathia   (501) staff       (20)        0 2022-05-25 22:34:04.000000 modelstore-0.0.79/tests/metadata/storage/__init__.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     2069 2022-12-17 10:26:28.000000 modelstore-0.0.79/tests/metadata/storage/test_storage.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     2706 2022-12-17 10:26:28.000000 modelstore-0.0.79/tests/metadata/test_metadata.py
+drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-06-09 14:53:14.726916 modelstore-0.0.79/tests/metadata/utils/
+-rw-r--r--   0 neallathia   (501) staff       (20)        0 2022-05-25 22:34:04.000000 modelstore-0.0.79/tests/metadata/utils/__init__.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     1866 2022-12-17 10:26:28.000000 modelstore-0.0.79/tests/metadata/utils/test_utils.py
+drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-06-09 14:53:14.742205 modelstore-0.0.79/tests/models/
+-rw-r--r--   0 neallathia   (501) staff       (20)        0 2022-01-13 15:38:40.000000 modelstore-0.0.79/tests/models/__init__.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     3567 2022-06-12 22:21:05.000000 modelstore-0.0.79/tests/models/test_annoy.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     4216 2022-06-12 22:21:05.000000 modelstore-0.0.79/tests/models/test_catboost.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     1424 2022-06-12 21:52:40.000000 modelstore-0.0.79/tests/models/test_common.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     5096 2023-03-19 19:25:32.000000 modelstore-0.0.79/tests/models/test_fastai.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     3449 2022-12-17 10:26:28.000000 modelstore-0.0.79/tests/models/test_gensim.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     4143 2022-06-12 22:21:05.000000 modelstore-0.0.79/tests/models/test_lightgbm.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     2571 2022-12-17 10:26:28.000000 modelstore-0.0.79/tests/models/test_managers.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     1302 2022-05-25 22:34:04.000000 modelstore-0.0.79/tests/models/test_missing_manager.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     2627 2022-06-12 22:21:05.000000 modelstore-0.0.79/tests/models/test_model_file.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     6166 2022-07-03 11:35:08.000000 modelstore-0.0.79/tests/models/test_model_manager.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     4993 2022-12-17 10:26:28.000000 modelstore-0.0.79/tests/models/test_multiple_models.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     3659 2022-06-12 22:21:05.000000 modelstore-0.0.79/tests/models/test_mxnet.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     4082 2022-06-12 22:21:05.000000 modelstore-0.0.79/tests/models/test_onnx.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     3856 2022-06-12 22:21:05.000000 modelstore-0.0.79/tests/models/test_prophet.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     4419 2023-06-08 11:33:57.000000 modelstore-0.0.79/tests/models/test_pyspark.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     4648 2022-06-12 22:21:05.000000 modelstore-0.0.79/tests/models/test_pytorch.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     5347 2022-06-12 22:21:05.000000 modelstore-0.0.79/tests/models/test_pytorch_lightning.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     3662 2022-06-12 22:21:05.000000 modelstore-0.0.79/tests/models/test_shap.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     5420 2022-12-17 10:26:28.000000 modelstore-0.0.79/tests/models/test_sklearn.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     3942 2022-06-12 22:21:05.000000 modelstore-0.0.79/tests/models/test_skorch.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     4664 2022-06-12 22:21:05.000000 modelstore-0.0.79/tests/models/test_tensorflow.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     4757 2023-05-06 22:45:07.000000 modelstore-0.0.79/tests/models/test_transformers.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     6108 2022-12-17 10:26:28.000000 modelstore-0.0.79/tests/models/test_xgboost.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     1519 2023-03-11 17:40:56.000000 modelstore-0.0.79/tests/models/utils.py
+drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-06-09 14:53:14.750142 modelstore-0.0.79/tests/storage/
+-rw-r--r--   0 neallathia   (501) staff       (20)        0 2022-01-13 15:38:40.000000 modelstore-0.0.79/tests/storage/__init__.py
+drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-06-09 14:53:14.750787 modelstore-0.0.79/tests/storage/states/
+-rw-r--r--   0 neallathia   (501) staff       (20)        0 2022-02-20 17:43:37.000000 modelstore-0.0.79/tests/storage/states/__init__.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     1281 2022-05-08 13:46:10.000000 modelstore-0.0.79/tests/storage/states/test_model_states.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     5982 2022-12-17 10:26:28.000000 modelstore-0.0.79/tests/storage/test_aws.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     9263 2022-12-17 10:26:28.000000 modelstore-0.0.79/tests/storage/test_azure.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     1828 2022-12-17 10:26:28.000000 modelstore-0.0.79/tests/storage/test_blob_storage.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     3190 2022-11-05 16:00:49.000000 modelstore-0.0.79/tests/storage/test_blob_storage_artifacts.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     3732 2022-12-03 00:48:26.000000 modelstore-0.0.79/tests/storage/test_blob_storage_meta_data.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     5172 2022-05-25 22:34:04.000000 modelstore-0.0.79/tests/storage/test_blob_storage_states.py
+-rw-r--r--   0 neallathia   (501) staff       (20)    10049 2022-12-17 10:26:28.000000 modelstore-0.0.79/tests/storage/test_gcloud.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     4306 2023-06-08 11:33:57.000000 modelstore-0.0.79/tests/storage/test_hdfs.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     6350 2022-12-17 10:26:28.000000 modelstore-0.0.79/tests/storage/test_local.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     5518 2022-12-17 10:26:28.000000 modelstore-0.0.79/tests/storage/test_minio.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     2504 2022-12-17 10:26:28.000000 modelstore-0.0.79/tests/storage/test_utils.py
+drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-06-09 14:53:14.751491 modelstore-0.0.79/tests/storage/util/
+-rw-r--r--   0 neallathia   (501) staff       (20)        0 2022-01-13 15:38:40.000000 modelstore-0.0.79/tests/storage/util/__init__.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     4361 2022-12-17 10:26:28.000000 modelstore-0.0.79/tests/storage/util/test_paths.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     3814 2022-12-17 10:26:28.000000 modelstore-0.0.79/tests/test_model_store.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     3323 2023-02-11 15:06:42.000000 modelstore-0.0.79/tests/test_model_store_filesystem.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     1777 2022-07-03 11:35:08.000000 modelstore-0.0.79/tests/test_model_store_gcp.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     2201 2023-02-07 00:37:01.000000 modelstore-0.0.79/tests/test_utils.py
+drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-06-09 14:53:14.753178 modelstore-0.0.79/workflows/
+-rw-r--r--   0 neallathia   (501) staff       (20)      640 2023-02-19 11:42:44.000000 modelstore-0.0.79/workflows/Makefile
+drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-06-09 14:53:14.754855 modelstore-0.0.79/workflows/actions/
+-rw-r--r--   0 neallathia   (501) staff       (20)        0 2022-06-25 18:07:50.000000 modelstore-0.0.79/workflows/actions/__init__.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     1917 2022-12-17 10:26:28.000000 modelstore-0.0.79/workflows/actions/actions.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     1910 2022-12-17 10:26:28.000000 modelstore-0.0.79/workflows/actions/cli.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     5143 2022-12-17 10:26:28.000000 modelstore-0.0.79/workflows/actions/models.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     1788 2022-12-17 10:26:28.000000 modelstore-0.0.79/workflows/actions/storage.py
+drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-06-09 14:53:14.757299 modelstore-0.0.79/workflows/fixtures/
+-rw-r--r--   0 neallathia   (501) staff       (20)        0 2022-06-25 18:07:50.000000 modelstore-0.0.79/workflows/fixtures/__init__.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     1433 2022-12-17 10:26:28.000000 modelstore-0.0.79/workflows/fixtures/extra.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     2058 2023-02-11 15:06:42.000000 modelstore-0.0.79/workflows/fixtures/models.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     3070 2022-12-17 10:26:28.000000 modelstore-0.0.79/workflows/fixtures/modelstores.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     2430 2023-06-08 13:00:47.000000 modelstore-0.0.79/workflows/main.py
+drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-06-09 14:53:14.760415 modelstore-0.0.79/workflows/requirements/
+-rw-r--r--   0 neallathia   (501) staff       (20)       14 2022-09-08 11:52:33.000000 modelstore-0.0.79/workflows/requirements/aws-s3.txt
+-rw-r--r--   0 neallathia   (501) staff       (20)       45 2022-09-08 11:52:33.000000 modelstore-0.0.79/workflows/requirements/azure-container.txt
+-rw-r--r--   0 neallathia   (501) staff       (20)        0 2022-06-25 18:07:50.000000 modelstore-0.0.79/workflows/requirements/filesystem.txt
+-rw-r--r--   0 neallathia   (501) staff       (20)      104 2022-09-08 11:52:33.000000 modelstore-0.0.79/workflows/requirements/google-cloud-storage.txt
+-rw-r--r--   0 neallathia   (501) staff       (20)       13 2022-12-03 00:48:26.000000 modelstore-0.0.79/workflows/requirements/minio.txt
+-rw-r--r--   0 neallathia   (501) staff       (20)       48 2023-02-11 15:06:42.000000 modelstore-0.0.79/workflows/requirements.txt
```

### Comparing `modelstore-0.0.78/.github/workflows/codeql-analysis.yml` & `modelstore-0.0.79/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/.github/workflows/integration-tests.yml` & `modelstore-0.0.79/.github/workflows/integration-tests.yml`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/.github/workflows/unit-tests.yml` & `modelstore-0.0.79/.github/workflows/unit-tests.yml`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/CHANGELOG.md` & `modelstore-0.0.79/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,21 @@
 # Change log
 
+## modelstore 0.0.79 ([June 2023](https://github.com/operatorai/modelstore/pull/243))
+
+**🆕  New functionality**
+
+Added support for any HDFS storage that you can access via [pydoop](https://crs4.github.io/pydoop/tutorial/hdfs_api.html#hdfs-api-tutorial): `ModelStore.from_hdfs()` [#241](https://github.com/operatorai/modelstore/pull/241), thanks [@sayandigital](https://github.com/sayandigital).
+
+Updated the transformers manager: it no longer requires a `tokenizer` argument, so it can now be used to (for example) save/load SAM models [#238](https://github.com/operatorai/modelstore/pull/238) or DPT models [#239](https://github.com/operatorai/modelstore/pull/239). Thank you, [Cate in the MLOps Community](https://mlops-community.slack.com/archives/C0227QJCDS8/p1683293544101389)
+
+**🐛  Bug fixes & general updates**
+
+Fixed [issues with saving & loading GPT-2 models](https://github.com/operatorai/modelstore/issues/233) in [#234](https://github.com/operatorai/modelstore/pull/234), thank you [@sayandigital](https://github.com/sayandigital).
+
 ## modelstore 0.0.78 ([March 2023](https://github.com/operatorai/modelstore/pull/227))
 
 **🆕  New functionality**
 
 Added support for Python 3.9, and an example where a yolov5 model is loaded from the torch hub, saved to modelstore, and then loaded back from the model store [#225](https://github.com/operatorai/modelstore/pull/225), thanks to @h4mmer in the MLOps Community.
 
 **🐛  Bug fixes & general updates**
```

### Comparing `modelstore-0.0.78/CODE_OF_CONDUCT.md` & `modelstore-0.0.79/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/CONTRIBUTING.md` & `modelstore-0.0.79/CONTRIBUTING.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,33 @@
 # Contributing to modelstore
 
 👋🏽 We'd love for you to contribute!
 
-If you have any questions or ideas, feel free to reach out.
+If you have any questions or ideas, feel free to reach out. 
 
-## Setup a virtual environment
+💬  Come and find us in the [MLOps Community Slack](https://go.mlops.community/slack)'s `#oss-modelstore` channel.
+
+# Contribute your experience
+
+If you've ever used `modelstore`, we've love for you to blog about your experience and link to your blog post in the repo's [README.md](https://github.com/operatorai/modelstore/blob/main/README.md) in the "Read more about modelstore" section.
+
+You can also contribute to the [modelstore documentation](https://github.com/operatorai/modelstore-docs), which is in a separate Github repo.
+
+# Contribute to the code base
+
+To contribute to `modelstore`'s code base, we recommend taking the following journey:
+
+1. Get familiar with the code base
+2. Contribute fixes for [bugs or issues](https://github.com/operatorai/modelstore/issues)
+3. Contribute new feature ideas from the [discussions](https://github.com/operatorai/modelstore/discussions) section 
+
+
+## 👨🏽‍💻 Get familiar with the code base
+
+### Setup a virtual environment
 
 This library has been developed using [pyenv](https://github.com/pyenv/pyenv)
 and [pyenv-virtualenv](https://github.com/pyenv/pyenv-virtualenv), using the
 requirements that are in `requirements.txt` and `requirements-dev.txt`.
 
 This project has two requirements files:
 * `requirements.txt` contains any dependencies that `modelstore` users must have in order to use `modelstore`. This should be as lightweight as possible. We do not require users to install every single machine learning library - just the ones that they want to use.
@@ -25,52 +44,57 @@
 Will update `brew` and install `libomp` (required by `xgboost`).
 
 It will then create a Python virtual environment, using `pyenv-virtualenv`,
 and install all of the dependencies in the requirements files. If you want
 to use a different version of Python, update the [bin/_config](bin/config) file.
 
 Notes:
-* I've seen trouble with installing `prophet`
+* I've seen trouble with installing `prophet` and have sometimes had to install it manually
 * Even when `prophet` installs, there are sometimes issues with running `test_prophet`? See [this issue](https://github.com/facebook/prophet/issues/689). Uninstalling and reinstalling has worked for me.
 
-## Run the tests
+### Run the tests
 
 We're using `pytest` for the tests. You can type `pytest`, or use
 this `Makefile` command:
 
 ```bash
 ❯ make test
 ```
 
-## Run the examples
+### Run the examples
 
 We have two types of examples:
 
 * `examples-by-ml-library`, which has iterates over  machine learning model library and writes to three different model stores (GCP, AWS, file system)
-* `examples-by-storage` which has 2 machine learning libraries (`sklearn` and `xgboost`) and writes to one type of model store
+* `cli-examples` shows how to use the `modelstore` command line interface
 
 For details, head over to the [README.md](examples/README.md) in the `examples` directory.
 
-## Code formatting
 
-This project uses `black` for code formatting.
+## 🐛 Contribute fixes for bugs or issues
+
+All of `modelstore`'s bugs are publicly tracked via [Github issues](https://github.com/operatorai/modelstore/issues). 
+
 
-## Add support for a new machine learning framework
+## 💡 Contribute new feature ideas
+
+There are a variety of ideas that have been listed in the repo's [discussions](https://github.com/operatorai/modelstore/discussions) section. For example:
+
+### Add support for a new machine learning framework
 
 The list of machine learning frameworks that are supported by `modelstore`
 are found in the [modelstore/models/](modelstore/models) directory.
 
 For a tutorial on how to add a new framework, refer to the [CONTRIBUTING.md](modelstore/models/CONTRIBUTING.md) guide in that directory.
 
-## Add support for a new storage type
+### Add support for a new storage type
 
 The list of storage types that are supported by `modelstore`
 are found in the [modelstore/storage/](modelstore/storage) directory.
 
 For a tutorial on how to add a new storage type, refer to the [CONTRIBUTING.md](modelstore/storage/CONTRIBUTING.md) guide in that directory.
 
-## Adding other features
+### Adding other features
 
 Do you have ideas for other features that it may be useful to add to `modelstore`?
 
 Please get in touch by opening a [discussion](https://github.com/operatorai/modelstore/discussions) or [issue](https://github.com/operatorai/modelstore/issues) on Github.
-
```

### Comparing `modelstore-0.0.78/LICENSE` & `modelstore-0.0.79/LICENSE`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/PKG-INFO` & `modelstore-0.0.79/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelstore
-Version: 0.0.78
+Version: 0.0.79
 Summary: modelstore is a library for versioning, exporting, storing, and loading machine learning models
 Home-page: https://github.com/operatorai/modelstore
 Author: Neal Lathia
 License: Please refer to the readme
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `modelstore-0.0.78/README.md` & `modelstore-0.0.79/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,36 +1,44 @@
 # modelstore
 
 `modelstore` is a Python library that allows you to version, export, save and download machine learning models in your choice of storage.
 
 [![Downloads](https://pepy.tech/badge/modelstore)](https://pepy.tech/project/modelstore) [![Downloads](https://pepy.tech/badge/modelstore/month)](https://pepy.tech/project/modelstore)
 
-For more details, please refer to [the documentation](https://modelstore.readthedocs.io/en/latest/) or come to the [MLOps Community Slack](https://go.mlops.community/slack)'s `#oss-modelstore` channel.
+💭  Give us feedback by completing this survey: https://forms.gle/XShU3zrZcnLRWsk36
 
-## modelstore is an open source model registry library
+[![](https://img.shields.io/static/v1?label=Sponsor&message=%E2%9D%A4&logo=GitHub&color=%23fe8e86)](https://github.com/sponsors/nlathia/)
 
-No tracking server required
+## modelstore is an open source model registry
+
+✅ No tracking server required
 * Store models on a local file system or in a bucket
 * Support for multiple clouds (AWS, GCP, Azure)
 
-Upload and version all your models
+✅ Upload and version all your models
 * Models are versioned on each upload
 * Replaces all the boiler plate code you need to save models
 
-Manage models by domains and states
+✅ Manage models by domains and states
 * List models in a domain
 * Create model states and manage which state a model is in
 
-Download and load
+✅ Download or load straight into memory
 * Download models by id
 * Load models straight from your storage back into memory
 
-Use as a command line tool
+✅ Use as a command line tool
 * Download models from the command line
 
+For more details, please refer to [the documentation](https://modelstore.readthedocs.io/en/latest/).
+
+## modelstore is being built in the open
+
+💬. Come and find us in the [MLOps Community Slack](https://go.mlops.community/slack)'s `#oss-modelstore` channel.
+
 ## Installation
 
 ```python
 pip install modelstore
 ```
 
 ## Supported storage types
@@ -63,14 +71,21 @@
 * [Transformers](https://github.com/operatorai/modelstore/blob/main/examples/examples-by-ml-library/libraries/transformers_example.py)
 * [XGBoost](https://github.com/operatorai/modelstore/blob/main/examples/examples-by-ml-library/libraries/xgboost_example.py)
 
 Is there a machine learning framework that is missing? 
 * Save your model and then upload it [as a raw file](https://github.com/operatorai/modelstore/blob/main/examples/examples-by-ml-library/libraries/raw_file_example.py).
 * Feel free to [open an issue](https://github.com/operatorai/modelstore/issues)
 
+## Read more about modelstore
+
+* [Evidently.AI AMA with Neal Lathia](https://www.evidentlyai.com/blog/ama-neal-lathia), January 2023
+* [MLOps Model Stores: Definition, Functionality, Tools Review](https://neptune.ai/blog/mlops-model-stores), January 2023
+* [Monzo's machine learning stack](https://monzo.com/blog/2022/04/26/monzos-machine-learning-stack), April 2022
+* [Model arterfacts: the war stories](https://nlathia.github.io/2020/09/Model-artifacts-war-stories.html), September 2020
+
 ## Example Usage
 
 ### Colab Notebook
 
 There is a [full example in this Colab notebook](https://colab.research.google.com/drive/1yEY6wy68k7TlHzm8iJMKKBG_Pl-MGZUe?usp=sharing).
 
 ### Python Script
@@ -93,29 +108,25 @@
 # Upload the archive to your model store
 domain = "example-model"
 meta_data = model_store.upload(domain, model=clf)
 
 # Print the meta-data about the model
 print(json.dumps(meta_data, indent=4))
 
-# Download the model back!
-target = f"downloaded-{model_type}-model"
-os.makedirs(target, exist_ok=True)
-model_path = model_store.download(
-   local_path=target,
-   domain=model_domain,
-   model_id=meta["model"]["model_id"],
-)
+# Load the model back!
+clf = model_store.load(domain=model_domain, model_id=meta["model"]["model_id"])
 ```
 
-## Recorded demo from Data Talks Club
+## Find out more
+
+💭  Give us feedback by completing this survey: https://forms.gle/XShU3zrZcnLRWsk36
 
-_Note_ the talk below is based on an older version of `modelstore` and the API has been simplified since then.
+[![](https://img.shields.io/static/v1?label=Sponsor&message=%E2%9D%A4&logo=GitHub&color=%23fe8e86)](https://github.com/sponsors/nlathia/)
 
-This interview and demo, recorded with Alexey from the [Data Talks Club](https://datatalks.club/) in July 2021, is based on `modelstore==0.0.6`. Click [here to watch on YouTube](https://www.youtube.com/watch?v=85BWnKmOZl8 "DTC's minis: Model Store").
+Watch an interview and demo, recorded with Alexey from the [Data Talks Club](https://datatalks.club/) in July 2021, is based on `modelstore==0.0.6`, [on YouTube](https://www.youtube.com/watch?v=85BWnKmOZl8 "DTC's minis: Model Store"). _Note_ the talk below is based on an older version of `modelstore` and the API has been simplified since then.
 
 ## License
 
 Copyright 2020 Neal Lathia
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
```

### Comparing `modelstore-0.0.78/bin/_brew_install` & `modelstore-0.0.79/bin/_brew_install`

 * *Files 25% similar despite different names*

```diff
@@ -6,18 +6,20 @@
 
 # To get pystan to install correctly (required by prophet)
 # https://stackoverflow.com/questions/52814868/pystan-compileerror-command-gcc-failed-with-exit-status-1-macos
 brew install gcc
 export CC=gcc-11
 export CXX=g++-11
 
-# To use xgboost
+# To use xgboost models on mac
 # https://xgboost.readthedocs.io/en/latest/build.html#building-on-osx
-
 # Note: it looks like there's trouble with libomp 12
 # https://github.com/dmlc/xgboost/issues/7039
 brew install rajivshah3/libomp-tap/libomp@11.1.0
 
-# To use pyspark
+# To use pyspark models on mac
 brew install java
 
+# To use hdfs storage on mac
+brew install hadoop
+
 echo "\n ✅  Done."
```

### Comparing `modelstore-0.0.78/bin/_pyenv_install` & `modelstore-0.0.79/bin/_pyenv_install`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/examples/Makefile-example` & `modelstore-0.0.79/examples/Makefile-example`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/examples/README.md` & `modelstore-0.0.79/examples/README.md`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/examples/examples-by-ml-library/libraries/annoy_example.py` & `modelstore-0.0.79/examples/examples-by-ml-library/libraries/yolo_example.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,50 +1,43 @@
-import random
+#    Copyright 2023 Neal Lathia
+#
+#    Licensed under the Apache License, Version 2.0 (the "License");
+#    you may not use this file except in compliance with the License.
+#    You may obtain a copy of the License at
+#
+#        http://www.apache.org/licenses/LICENSE-2.0
+#
+#    Unless required by applicable law or agreed to in writing, software
+#    distributed under the License is distributed on an "AS IS" BASIS,
+#    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#    See the License for the specific language governing permissions and
+#    limitations under the License.
 
-from annoy import AnnoyIndex
+import torch
 from modelstore.model_store import ModelStore
 
-_NUM_DIMENSIONS = 40
-_NUM_TREES = 10
-_METRIC = "angular"
-_DOMAIN_NAME = "example-annoy-index"
-
-
-def _train_example_model() -> AnnoyIndex:
-    # Create an index
-    print("🤖  Creating an Annoy index...")
-    model = AnnoyIndex(_NUM_DIMENSIONS, _METRIC)
-    for i in range(1000):
-        vector = [random.gauss(0, 1) for z in range(_NUM_DIMENSIONS)]
-        model.add_item(i, vector)
-    model.build(_NUM_TREES)
-
-    # Show some nearest neighbours
-    results = model.get_nns_by_item(0, 10)
-    print(f"🔍  Nearest neighbors = {results}.")
-    return model
+_YOLO_DOMAIN = "yolov5"
+
+
+def _predict(model):
+    model.eval()
+    img = "https://ultralytics.com/images/zidane.jpg"
+    results = model(img)
+    print(f"🔍  Prediction result: \n{results.pandas().xyxy[0]}.")
 
 
 def train_and_upload(modelstore: ModelStore) -> dict:
-    # Train an Annoy index
-    model = _train_example_model()
+    # Load the yolov5 model
+    model = torch.hub.load("ultralytics/yolov5", "yolov5s")
+    _predict(model)
 
     # Upload the model to the model store
-    print(f'⤴️  Uploading the Annoy model to the "{_DOMAIN_NAME}" domain.')
-    meta_data = modelstore.upload(
-        _DOMAIN_NAME,
-        model=model,
-        num_dimensions=_NUM_DIMENSIONS,
-        metric=_METRIC,
-        num_trees=_NUM_TREES,
-    )
+    print(f'⤴️  Uploading the yolo model to the "{_YOLO_DOMAIN}" domain.')
+    meta_data = modelstore.upload(_YOLO_DOMAIN, model=model)
     return meta_data
 
 
 def load_and_test(modelstore: ModelStore, model_domain: str, model_id: str):
     # Load the model back into memory!
-    print(f'⤵️  Loading the Annoy "{model_domain}" domain model={model_id}')
+    print(f'⤵️  Loading the yolo "{model_domain}" domain model={model_id}')
     model = modelstore.load(model_domain, model_id)
-
-    # Find some nearest neighbours
-    results = model.get_nns_by_item(0, 10)
-    print(f"🔍  Nearest neighbors = {results}.")
+    _predict(model)
```

### Comparing `modelstore-0.0.78/examples/examples-by-ml-library/libraries/onnx_lightgbm_example.py` & `modelstore-0.0.79/examples/examples-by-ml-library/libraries/onnx_lightgbm_example.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+#    Copyright 2023 Neal Lathia
+#
+#    Licensed under the Apache License, Version 2.0 (the "License");
+#    you may not use this file except in compliance with the License.
+#    You may obtain a copy of the License at
+#
+#        http://www.apache.org/licenses/LICENSE-2.0
+#
+#    Unless required by applicable law or agreed to in writing, software
+#    distributed under the License is distributed on an "AS IS" BASIS,
+#    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#    See the License for the specific language governing permissions and
+#    limitations under the License.
+
 import numpy as np
 import onnx
 from modelstore.model_store import ModelStore
 
 from onnxruntime import InferenceSession
 from skl2onnx import convert_sklearn, update_registered_converter
 from skl2onnx.common.shape_calculator import (
```

### Comparing `modelstore-0.0.78/examples/examples-by-ml-library/libraries/pyspark_example.py` & `modelstore-0.0.79/examples/examples-by-ml-library/libraries/pyspark_example.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+#    Copyright 2023 Neal Lathia
+#
+#    Licensed under the Apache License, Version 2.0 (the "License");
+#    you may not use this file except in compliance with the License.
+#    You may obtain a copy of the License at
+#
+#        http://www.apache.org/licenses/LICENSE-2.0
+#
+#    Unless required by applicable law or agreed to in writing, software
+#    distributed under the License is distributed on an "AS IS" BASIS,
+#    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#    See the License for the specific language governing permissions and
+#    limitations under the License.
+
 from pyspark.sql import SparkSession
 from pyspark.sql import SQLContext
 from pyspark.ml.feature import VectorAssembler
 
 from pyspark.ml import Pipeline, PipelineModel
 from pyspark.ml.regression import RandomForestRegressor
```

### Comparing `modelstore-0.0.78/examples/examples-by-ml-library/libraries/pytorch_example.py` & `modelstore-0.0.79/examples/examples-by-ml-library/libraries/tensorflow_example.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,60 +1,61 @@
-import torch
+#    Copyright 2023 Neal Lathia
+#
+#    Licensed under the Apache License, Version 2.0 (the "License");
+#    you may not use this file except in compliance with the License.
+#    You may obtain a copy of the License at
+#
+#        http://www.apache.org/licenses/LICENSE-2.0
+#
+#    Unless required by applicable law or agreed to in writing, software
+#    distributed under the License is distributed on an "AS IS" BASIS,
+#    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#    See the License for the specific language governing permissions and
+#    limitations under the License.
+
+import tensorflow as tf
 from modelstore.model_store import ModelStore
 from sklearn.metrics import mean_squared_error
-from torch import nn
 
 from libraries.util.datasets import load_regression_dataset
 from libraries.util.domains import DIABETES_DOMAIN
 
 
-# pylint: disable=missing-class-docstring
-class ExampleNet(nn.Module):
-    def __init__(self):
-        super(ExampleNet, self).__init__()
-        self.linear = nn.Linear(10, 1)
-
-    def forward(self, x):
-        return self.linear(x)
-
-
-def _train_example_model() -> ExampleNet:
+def _train_example_model() -> tf.keras.models.Sequential:
     # Load the data
-    X_train, X_test, y_train, y_test = load_regression_dataset(as_numpy=True)
+    X_train, X_test, y_train, y_test = load_regression_dataset()
 
-    # Train the model
-    model = ExampleNet()
-    criterion = torch.nn.MSELoss()
-    optimizer = torch.optim.Adam(model.parameters())
-
-    for epoch in range(5):
-        print(f"🤖  Training epoch: {epoch}...")
-        optimizer.zero_grad()
-        outputs = model(X_train)
-        loss = criterion(outputs, y_train)
-        loss.backward()
-        optimizer.step()
-
-    results = mean_squared_error(y_test, model(X_test).detach().numpy())
-    print(f"🔍  Fit model MSE={results}.")
-    return model, optimizer
+    # Train a model
+    model = tf.keras.models.Sequential(
+        [
+            tf.keras.layers.Dense(5, activation="relu", input_shape=(10,)),
+            tf.keras.layers.Dropout(0.2),
+            tf.keras.layers.Dense(1),
+        ]
+    )
+    model.compile(optimizer="adam", loss="mean_squared_error")
+    model.fit(X_train, y_train, epochs=10)
+
+    results = mean_squared_error(y_test, model.predict(X_test))
+    print(f"🔍  Trained model MSE={results}.")
+    return model
 
 
 def train_and_upload(modelstore: ModelStore) -> dict:
-    # Train a PyTorch model
-    model, optimizer = _train_example_model()
+    # Train a model
+    model = _train_example_model()
 
     # Upload the model to the model store
-    print(f'⤴️  Uploading the pytorch model to the "{DIABETES_DOMAIN}" domain.')
-    meta_data = modelstore.upload(DIABETES_DOMAIN, model=model, optimizer=optimizer)
+    print(f'⤴️  Uploading the tensorflow model to the "{DIABETES_DOMAIN}" domain.')
+    meta_data = modelstore.upload(DIABETES_DOMAIN, model=model)
     return meta_data
 
 
 def load_and_test(modelstore: ModelStore, model_domain: str, model_id: str):
     # Load the model back into memory!
-    print(f'⤵️  Loading the pytorch "{model_domain}" domain model={model_id}')
+    print(f'⤵️  Loading the tensorflow "{model_domain}" domain model={model_id}')
     model = modelstore.load(model_domain, model_id)
-    model.eval()
 
-    _, X_test, _, y_test = load_regression_dataset(as_numpy=True)
-    results = mean_squared_error(y_test, model(X_test).detach().numpy())
+    # Run some test predictions
+    _, X_test, _, y_test = load_regression_dataset()
+    results = mean_squared_error(y_test, model.predict(X_test))
     print(f"🔍  Loaded model MSE={results}.")
```

### Comparing `modelstore-0.0.78/examples/examples-by-ml-library/libraries/pytorch_lightning_example.py` & `modelstore-0.0.79/examples/examples-by-ml-library/libraries/pytorch_lightning_example.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+#    Copyright 2023 Neal Lathia
+#
+#    Licensed under the Apache License, Version 2.0 (the "License");
+#    you may not use this file except in compliance with the License.
+#    You may obtain a copy of the License at
+#
+#        http://www.apache.org/licenses/LICENSE-2.0
+#
+#    Unless required by applicable law or agreed to in writing, software
+#    distributed under the License is distributed on an "AS IS" BASIS,
+#    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#    See the License for the specific language governing permissions and
+#    limitations under the License.
+
 import tempfile
 
 import pytorch_lightning as pl
 import torch
 import torch.nn.functional as F
 from modelstore.model_store import ModelStore
 from sklearn.metrics import mean_squared_error
```

### Comparing `modelstore-0.0.78/examples/examples-by-ml-library/libraries/shap_example.py` & `modelstore-0.0.79/examples/examples-by-ml-library/libraries/xgboost_booster_example.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,56 +1,62 @@
-import shap
+#    Copyright 2023 Neal Lathia
+#
+#    Licensed under the Apache License, Version 2.0 (the "License");
+#    you may not use this file except in compliance with the License.
+#    You may obtain a copy of the License at
+#
+#        http://www.apache.org/licenses/LICENSE-2.0
+#
+#    Unless required by applicable law or agreed to in writing, software
+#    distributed under the License is distributed on an "AS IS" BASIS,
+#    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#    See the License for the specific language governing permissions and
+#    limitations under the License.
+
+import xgboost as xgb
 from modelstore.model_store import ModelStore
-from sklearn.ensemble import GradientBoostingRegressor
 from sklearn.metrics import mean_squared_error
-from sklearn.pipeline import Pipeline
 
 from libraries.util.datasets import load_regression_dataset
 from libraries.util.domains import DIABETES_DOMAIN
 
-EXPLAINER_DOMAIN = f"{DIABETES_DOMAIN}-explainer"
-
 
-def _train_example_model() -> Pipeline:
+def _train_example_model() -> xgb.Booster:
+    # Load the data
     X_train, X_test, y_train, y_test = load_regression_dataset()
 
-    # Train a model using an sklearn pipeline
-    params = {
-        "n_estimators": 250,
-        "max_depth": 4,
-        "min_samples_split": 5,
-        "learning_rate": 0.01,
-        "loss": "ls",
-    }
-    model = GradientBoostingRegressor(**params)
+    # Train a model
+    model = xgb.XGBRegressor(
+        objective="reg:squarederror",
+        colsample_bytree=0.3,
+        learning_rate=0.1,
+        max_depth=5,
+        alpha=10,
+        n_estimators=10,
+    )
     model.fit(X_train, y_train)
-    results = mean_squared_error(y_test, model.predict(X_test))
-    print(f"🔍  Trained model MSE={results}.")
+    booster = model.get_booster()
 
-    explainer = shap.TreeExplainer(model)
-
-    # Example only
-    shap_values = explainer.shap_values(X_test)[0]
-    print(f"🔍  Shap values={shap_values[:10]}.")
-
-    return explainer
+    results = mean_squared_error(y_test, booster.predict(xgb.DMatrix(X_test)))
+    print(f"🔍  Trained model MSE={results}.")
+    return booster
 
 
 def train_and_upload(modelstore: ModelStore) -> dict:
-    # Train a model and return the explainer
-    explainer = _train_example_model()
+    # Train a model
+    model = _train_example_model()
 
-    # Upload the explainer to the model store
-    print(f'⤴️  Uploading the explainer to the "{EXPLAINER_DOMAIN}" domain.')
-    meta_data = modelstore.upload(EXPLAINER_DOMAIN, explainer=explainer)
+    # Upload the model to the model store
+    print(f'⤴️  Uploading the xgboost booster to the "{DIABETES_DOMAIN}" domain.')
+    meta_data = modelstore.upload(DIABETES_DOMAIN, model=model)
     return meta_data
 
 
 def load_and_test(modelstore: ModelStore, model_domain: str, model_id: str):
-    # Load the explainer back into memory!
-    print(f'⤵️  Loading the explainer "{model_domain}" domain model={model_id}')
-    explainer = modelstore.load(model_domain, model_id)
+    # Load the model back into memory!
+    print(f'⤵️  Loading the xgboost booster "{model_domain}" domain model={model_id}')
+    booster = modelstore.load(model_domain, model_id)
 
     # Run some example predictions
-    _, X_test, _, _ = load_regression_dataset()
-    shap_values = explainer.shap_values(X_test)[0]
-    print(f"🔍  Shap values={shap_values[:10]}.")
+    _, X_test, _, y_test = load_regression_dataset()
+    results = mean_squared_error(y_test, booster.predict(xgb.DMatrix(X_test)))
+    print(f"🔍  Loaded model MSE={results}.")
```

### Comparing `modelstore-0.0.78/examples/examples-by-ml-library/libraries/sklearn_with_extras_example.py` & `modelstore-0.0.79/examples/examples-by-ml-library/libraries/sklearn_with_extras_example.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+#    Copyright 2023 Neal Lathia
+#
+#    Licensed under the Apache License, Version 2.0 (the "License");
+#    you may not use this file except in compliance with the License.
+#    You may obtain a copy of the License at
+#
+#        http://www.apache.org/licenses/LICENSE-2.0
+#
+#    Unless required by applicable law or agreed to in writing, software
+#    distributed under the License is distributed on an "AS IS" BASIS,
+#    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#    See the License for the specific language governing permissions and
+#    limitations under the License.
+
 from typing import Tuple
 import tempfile
 import numpy
 import os
 
 from modelstore.model_store import ModelStore
 from sklearn.ensemble import GradientBoostingRegressor
@@ -17,15 +31,15 @@
 
     # Train a model using an sklearn pipeline
     params = {
         "n_estimators": 250,
         "max_depth": 4,
         "min_samples_split": 5,
         "learning_rate": 0.01,
-        "loss": "ls",
+        "loss": "squared_error",
     }
     model = GradientBoostingRegressor(**params)
     model.fit(X_train, y_train)
 
     predictions = model.predict(X_test)
     results = mean_squared_error(y_test, model.predict(X_test))
     print(f"🔍  Trained model MSE={results}.")
```

### Comparing `modelstore-0.0.78/examples/examples-by-ml-library/libraries/skorch_example.py` & `modelstore-0.0.79/examples/examples-by-ml-library/libraries/catboost_example.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,56 +1,55 @@
+#    Copyright 2023 Neal Lathia
+#
+#    Licensed under the Apache License, Version 2.0 (the "License");
+#    you may not use this file except in compliance with the License.
+#    You may obtain a copy of the License at
+#
+#        http://www.apache.org/licenses/LICENSE-2.0
+#
+#    Unless required by applicable law or agreed to in writing, software
+#    distributed under the License is distributed on an "AS IS" BASIS,
+#    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#    See the License for the specific language governing permissions and
+#    limitations under the License.
+
+import catboost as ctb
 from modelstore.model_store import ModelStore
 from sklearn.metrics import mean_squared_error
-from skorch.regressor import NeuralNetRegressor
-from torch import nn
 
 from libraries.util.datasets import load_regression_dataset
 from libraries.util.domains import DIABETES_DOMAIN
 
 
-class ExampleModule(nn.Module):
-    def __init__(self, num_units=1):
-        super(ExampleModule, self).__init__()
-        self.linear = nn.Linear(10, num_units)
-
-    def forward(self, X, **kwargs):
-        return self.linear(X)
-
-
-def _train_example_model() -> NeuralNetRegressor:
+def _train_example_model() -> ctb.CatBoostRegressor:
     # Load the data
-    X_train, X_test, y_train, y_test = load_regression_dataset(as_numpy=True)
+    X_train, X_test, y_train, y_test = load_regression_dataset()
+
+    # Train the model
+    print("🤖  Training a CatBoostRegressor")
+    model = ctb.CatBoostRegressor(allow_writing_files=False)
+    model.fit(X_train, y_train)
 
-    # Train a model
-    net = NeuralNetRegressor(
-        ExampleModule,
-        max_epochs=1,
-        lr=0.1,
-        # Shuffle training data on each epoch
-        iterator_train__shuffle=True,
-    )
-    net.fit(X_train, y_train)
-
-    results = mean_squared_error(y_test, net.predict(X_test))
-    print(f"🔍  Trained model MSE={results}.")
-    return net
+    results = mean_squared_error(y_test, model.predict(X_test))
+    print(f"🔍  Fit model MSE={results}.")
+    return model
 
 
 def train_and_upload(modelstore: ModelStore) -> dict:
-    # Train a skorch model
+    # Train a Catboost model
     model = _train_example_model()
 
     # Upload the model to the model store
-    print(f'⤴️  Uploading the skorch model to the "{DIABETES_DOMAIN}" domain.')
+    print(f'⤴️  Uploading the catboost model to the "{DIABETES_DOMAIN}" domain.')
     meta_data = modelstore.upload(DIABETES_DOMAIN, model=model)
     return meta_data
 
 
 def load_and_test(modelstore: ModelStore, model_domain: str, model_id: str):
     # Load the model back into memory!
-    print(f'⤵️  Loading the skorch "{model_domain}" domain model={model_id}')
+    print(f'⤵️  Loading the catboost "{model_domain}" domain model={model_id}')
     model = modelstore.load(model_domain, model_id)
 
     # Run some example predictions
-    _, X_test, _, y_test = load_regression_dataset(as_numpy=True)
+    _, X_test, _, y_test = load_regression_dataset()
     results = mean_squared_error(y_test, model.predict(X_test))
     print(f"🔍  Loaded model MSE={results}.")
```

### Comparing `modelstore-0.0.78/examples/examples-by-ml-library/modelstores.py` & `modelstore-0.0.79/examples/examples-by-ml-library/modelstores.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,74 +12,85 @@
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 import os
 
 from modelstore import ModelStore
 from modelstore.storage.aws import AWSStorage
 from modelstore.storage.azure import AzureBlobStorage
-from modelstore.storage.gcloud import GoogleCloudStorage
 from modelstore.storage.local import FileSystemStorage
+from modelstore.storage.gcloud import GoogleCloudStorage
+from modelstore.storage.hdfs import HdfsStorage
 from modelstore.storage.minio import MinIOStorage
 
 
-def create_model_store(backend) -> ModelStore:
-    """Returns a modelstore instance with the required storage type"""
-    modelstores = {
-        AWSStorage.NAME: create_aws_model_store,
-        AzureBlobStorage.NAME: create_azure_model_store,
-        GoogleCloudStorage.NAME: create_gcloud_model_store,
-        FileSystemStorage.NAME: create_file_system_model_store,
-        MinIOStorage.NAME: create_minio_model_store,
-    }
-    return modelstores[backend]()
-
-
 def create_aws_model_store() -> ModelStore:
     """A model store that uses an s3 bucket"""
     return ModelStore.from_aws_s3(
         os.environ["MODEL_STORE_AWS_BUCKET"],
         root_prefix="example-by-ml-library",
     )
 
 
-def create_minio_model_store() -> ModelStore:
-    """A model store that uses an s3 bucket with a MinIO client"""
-    return ModelStore.from_minio(
-        access_key=os.environ["AWS_ACCESS_KEY_ID"],
-        secret_key=os.environ["AWS_SECRET_ACCESS_KEY"],
-        bucket_name=os.environ["MODEL_STORE_AWS_BUCKET"],
-        root_prefix="example-by-ml-library",
-    )
-
-
 def create_azure_model_store() -> ModelStore:
     """A model store that uses an azure container"""
     # A model store in an Azure Container
     # The modelstore library assumes that:
     # 1. You have already created an Azure container
     # 2. You have an os environment variable called AZURE_STORAGE_CONNECTION_STRING
     return ModelStore.from_azure(
         container_name=os.environ["MODEL_STORE_AZURE_CONTAINER"],
         root_prefix=os.environ.get("MODEL_STORE_AZURE_ROOT_PREFIX"),
     )
 
 
+def create_file_system_model_store() -> ModelStore:
+    """A model store in a local file system"""
+    # Here, we create a new local model store in our home directory
+    root_dir = os.environ.get(
+        "MODEL_STORE_ROOT_PREFIX",
+        os.path.expanduser("~"),
+    )
+    print(f"🏦  Creating store in: {root_dir}")
+    return ModelStore.from_file_system(root_directory=root_dir)
+
+
 def create_gcloud_model_store() -> ModelStore:
     """A model store in a Google Cloud bucket"""
     # The modelstore library assumes you have already created
     # a Cloud Storage bucket and will raise an exception if it doesn't exist
     return ModelStore.from_gcloud(
         os.environ["MODEL_STORE_GCP_PROJECT"],
         os.environ["MODEL_STORE_GCP_BUCKET"],
         root_prefix=os.environ.get("MODEL_STORE_GCP_ROOT_PREFIX"),
     )
 
 
-def create_file_system_model_store() -> ModelStore:
-    """A model store in a local file system"""
-    # Here, we create a new local model store in our home directory
-    root_dir = os.environ.get(
-        "MODEL_STORE_ROOT_PREFIX",
-        os.path.expanduser("~"),
+def create_hdfs_model_store() -> ModelStore:
+    """A model store in HDFS storage"""
+    return ModelStore.from_hdfs(
+        root_prefix=os.environ["MODEL_STORE_HDFS_ROOT_PREFIX"],
+        create_directory=True,
     )
-    print(f"🏦  Creating store in: {root_dir}")
-    return ModelStore.from_file_system(root_directory=root_dir)
+
+
+def create_minio_model_store() -> ModelStore:
+    """A model store that uses an s3 bucket with a MinIO client"""
+    return ModelStore.from_minio(
+        access_key=os.environ["AWS_ACCESS_KEY_ID"],
+        secret_key=os.environ["AWS_SECRET_ACCESS_KEY"],
+        bucket_name=os.environ["MODEL_STORE_AWS_BUCKET"],
+        root_prefix="example-by-ml-library",
+    )
+
+
+MODELSTORES = {
+    AWSStorage.NAME: create_aws_model_store,
+    AzureBlobStorage.NAME: create_azure_model_store,
+    FileSystemStorage.NAME: create_file_system_model_store,
+    GoogleCloudStorage.NAME: create_gcloud_model_store,
+    HdfsStorage.NAME: create_hdfs_model_store,
+    MinIOStorage.NAME: create_minio_model_store,
+}
+
+def create_model_store(backend) -> ModelStore:
+    """Returns a modelstore instance with the required storage type"""
+    return MODELSTORES[backend]()
```

### Comparing `modelstore-0.0.78/examples/examples-by-ml-library/requirements.txt` & `modelstore-0.0.79/examples/examples-by-ml-library/requirements.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # Demo requirements
 # Versions unpinned to make it easier to test everything with
 # the latest version
 click
 
 # Storage requirements
-protobuf==3.20.1 # https://github.com/protocolbuffers/protobuf/issues/10051
-google-cloud-storage
-boto3
 azure-core
 azure-storage-blob
+boto3
+google-cloud-storage
+pydoop
 minio
 
 # Data / dependencies for ML libraries
-numpy>=1.19.2
+numba==0.56.4
+numpy==1.23.5
 python-Levenshtein==0.12.2
-numba==0.55.1
 
 # Prophet
 pystan==2.19.1.1 # required to be installed before prophet
 
 # Machine learning libraries
 annoy
 catboost
```

### Comparing `modelstore-0.0.78/modelstore/__main__.py` & `modelstore-0.0.79/modelstore/__main__.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/modelstore/ids/model_ids.py` & `modelstore-0.0.79/modelstore/ids/model_ids.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/modelstore/metadata/code/code.py` & `modelstore-0.0.79/modelstore/metadata/code/code.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/modelstore/metadata/code/dependencies.py` & `modelstore-0.0.79/modelstore/metadata/code/dependencies.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/modelstore/metadata/code/revision.py` & `modelstore-0.0.79/modelstore/metadata/code/revision.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/modelstore/metadata/code/runtime.py` & `modelstore-0.0.79/modelstore/metadata/code/runtime.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/modelstore/metadata/dataset/dataset.py` & `modelstore-0.0.79/modelstore/metadata/dataset/dataset.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #        http://www.apache.org/licenses/LICENSE-2.0
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
-from typing import Any
+from typing import Any, Optional
 from dataclasses import dataclass, field
 from dataclasses_json import dataclass_json
 from dataclasses_json.cfg import config
 
 from modelstore.metadata.dataset.features import Features
 from modelstore.metadata.dataset.labels import Labels
 from modelstore.metadata.utils.utils import exclude_field
@@ -24,16 +24,16 @@
 @dataclass_json
 @dataclass
 class Dataset:
 
     """Dataset contains fields that are captured about
     the training dataset when the model is saved"""
 
-    features: Features = field(default=None, metadata=config(exclude=exclude_field))
-    labels: Labels = field(default=None, metadata=config(exclude=exclude_field))
+    features: Optional[Features] = field(default=None, metadata=config(exclude=exclude_field))
+    labels: Optional[Labels] = field(default=None, metadata=config(exclude=exclude_field))
 
     @classmethod
     def generate(cls, features: Any = None, labels: Any = None) -> "Dataset":
         """Returns summary stats about a dataset"""
         features = Features.generate(features)
         labels = Labels.generate(labels)
         if features is None and labels is None:
```

### Comparing `modelstore-0.0.78/modelstore/metadata/dataset/features.py` & `modelstore-0.0.79/modelstore/metadata/dataset/features.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #        http://www.apache.org/licenses/LICENSE-2.0
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
-from typing import Any, List
+from typing import Any, List, Optional
 
 from dataclasses import dataclass, field
 from dataclasses_json import dataclass_json
 from dataclasses_json.cfg import config
 
 from modelstore.metadata.dataset.types import is_numpy_array, is_pandas_dataframe
 from modelstore.metadata.utils.utils import exclude_field
@@ -25,15 +25,15 @@
 @dataclass_json
 @dataclass
 class Features:
 
     """Features contains fields that are captured about
     the training dataset's features when the model is saved"""
 
-    shape: List[int] = field(default=None, metadata=config(exclude=exclude_field))
+    shape: Optional[List[int]] = field(default=None, metadata=config(exclude=exclude_field))
 
     @classmethod
     def generate(cls, values: Any = None) -> "Features":
         """Returns summary stats about a set of features"""
         if values is None:
             return None
         if is_numpy_array(values):
```

### Comparing `modelstore-0.0.78/modelstore/metadata/dataset/labels.py` & `modelstore-0.0.79/modelstore/metadata/dataset/labels.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #        http://www.apache.org/licenses/LICENSE-2.0
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
-from typing import List, Any
+from typing import List, Any, Optional
 from dataclasses import dataclass, field
 from dataclasses_json import dataclass_json
 from dataclasses_json.cfg import config
 import numpy as np
 
 from modelstore.metadata.dataset.types import (
     is_numpy_array,
@@ -29,16 +29,16 @@
 @dataclass_json
 @dataclass
 class Labels:
 
     """Labels contains fields that are captured about
     the training dataset's labels when the model is saved"""
 
-    shape: List[int] = field(default=None, metadata=config(exclude=exclude_field))
-    values: dict = field(default=None, metadata=config(exclude=exclude_field))
+    shape: Optional[List[int]] = field(default=None, metadata=config(exclude=exclude_field))
+    values: Optional[dict] = field(default=None, metadata=config(exclude=exclude_field))
 
     @classmethod
     def generate(cls, values: Any = None) -> "Labels":
         """Returns summary stats about a set of labels"""
         if values is None:
             return None
         if is_numpy_array(values):
```

### Comparing `modelstore-0.0.78/modelstore/metadata/dataset/types.py` & `modelstore-0.0.79/modelstore/metadata/dataset/types.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/modelstore/metadata/metadata.py` & `modelstore-0.0.79/modelstore/metadata/metadata.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/modelstore/metadata/model/model.py` & `modelstore-0.0.79/modelstore/metadata/model/model.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/modelstore/metadata/model/model_type.py` & `modelstore-0.0.79/modelstore/metadata/model/model_type.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 @dataclass
 class ModelType:
 
     """ModelType contains fields that are captured about
     the model type when it is saved"""
 
     library: str
-    type: str = field(default=None, metadata=config(exclude=exclude_field))
+    type: Optional[str] = field(default=None, metadata=config(exclude=exclude_field))
 
     # When saving multiple models together, the models'
     # types are specified in this list
     models: Optional[List["ModelType"]] = field(
         default=None, metadata=config(exclude=exclude_field)
     )
```

### Comparing `modelstore-0.0.78/modelstore/metadata/storage/storage.py` & `modelstore-0.0.79/modelstore/metadata/storage/storage.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/modelstore/metadata/utils/utils.py` & `modelstore-0.0.79/modelstore/metadata/utils/utils.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/modelstore/model_store.py` & `modelstore-0.0.79/modelstore/model_store.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 from modelstore.ids import model_ids
 from modelstore.storage.states.model_states import ReservedModelStates
 from modelstore.models.managers import iter_libraries, matching_managers, get_manager
 from modelstore.models.multiple_models import MultipleModelsManager
 from modelstore.storage.aws import BOTO_EXISTS, AWSStorage
 from modelstore.storage.azure import AZURE_EXISTS, AzureBlobStorage
 from modelstore.storage.gcloud import GCLOUD_EXISTS, GoogleCloudStorage
+from modelstore.storage.hdfs import HDFS_EXISTS, HdfsStorage
 from modelstore.storage.local import FileSystemStorage
 from modelstore.storage.minio import MINIO_EXISTS, MinIOStorage
 from modelstore.storage.storage import CloudStorage
 from modelstore.utils.exceptions import (
     ModelExistsException,
     DomainNotFoundException,
     ModelNotFoundException,
@@ -102,15 +103,15 @@
     def from_minio(
         cls,
         endpoint: Optional[str] = None,  # Defaults to s3.amazonaws.com
         access_key: Optional[str] = None,
         secret_key: Optional[str] = None,
         bucket_name: Optional[str] = None,
         root_prefix: Optional[str] = None,
-        secure: Optional[bool] = True
+        secure: Optional[bool] = True,
     ) -> "ModelStore":
         """Creates a ModelStore instance that stores models using a MinIO client.
         This assumes that the bucket already exists."""
         if not MINIO_EXISTS:
             raise ModuleNotFoundError("minio is not installed!")
         return ModelStore(
             storage=MinIOStorage(
@@ -120,14 +121,24 @@
                 bucket_name=bucket_name,
                 root_prefix=root_prefix,
                 secure=secure,
             )
         )
 
     @classmethod
+    def from_hdfs(
+        cls, root_prefix: Optional[str] = None, create_directory: bool = False
+    ) -> "ModelStore":
+        """Creates a ModelStore instance that stores models to
+        the local HDFS system."""
+        if not HDFS_EXISTS:
+            raise ModuleNotFoundError("pydoop is not installed!")
+        return ModelStore(storage=HdfsStorage(root_prefix, create_directory))
+
+    @classmethod
     def from_file_system(
         cls, root_directory: Optional[str] = None, create_directory: bool = False
     ) -> "ModelStore":
         """Creates a ModelStore instance that stores models to
         the local file system."""
         return ModelStore(storage=FileSystemStorage(root_directory, create_directory))
 
@@ -189,15 +200,16 @@
     def list_model_states(self) -> list:
         """Returns a list of the available model states that
         have been created with `create_model_state()`"""
         return self.storage.list_model_states()
 
     def create_model_state(self, state_name: str):
         """Creates a state label models (e.g., shadow/prod/archived).
-        There are some values that are reserved, see modelstore/storage/states/model_states.py"""
+        There are some values that are reserved, see modelstore/storage/states/model_states.py
+        """
         return self.storage.create_model_state(state_name)
 
     def set_model_state(self, domain: str, model_id: str, state_name: str):
         """Sets the model_id model to a specific state.
         That state must already exist (ref: `create_model_state()`) unless
         it is a reserved value (modelstore/storage/states/model_states.py)
         """
```

### Comparing `modelstore-0.0.78/modelstore/models/CONTRIBUTING.md` & `modelstore-0.0.79/modelstore/models/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/modelstore/models/annoy.py` & `modelstore-0.0.79/modelstore/models/annoy.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/modelstore/models/catboost.py` & `modelstore-0.0.79/modelstore/models/catboost.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/modelstore/models/common.py` & `modelstore-0.0.79/modelstore/models/common.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/modelstore/models/fastai.py` & `modelstore-0.0.79/modelstore/models/fastai.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/modelstore/models/gensim.py` & `modelstore-0.0.79/modelstore/models/gensim.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/modelstore/models/lightgbm.py` & `modelstore-0.0.79/modelstore/models/lightgbm.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/modelstore/models/managers.py` & `modelstore-0.0.79/modelstore/models/managers.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/modelstore/models/missing_manager.py` & `modelstore-0.0.79/modelstore/models/missing_manager.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/modelstore/models/model_file.py` & `modelstore-0.0.79/modelstore/models/model_file.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/modelstore/models/model_manager.py` & `modelstore-0.0.79/modelstore/models/model_manager.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/modelstore/models/multiple_models.py` & `modelstore-0.0.79/modelstore/models/multiple_models.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/modelstore/models/mxnet.py` & `modelstore-0.0.79/modelstore/models/mxnet.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/modelstore/models/onnx.py` & `modelstore-0.0.79/modelstore/models/onnx.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/modelstore/models/prophet.py` & `modelstore-0.0.79/modelstore/models/prophet.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/modelstore/models/pyspark.py` & `modelstore-0.0.79/modelstore/models/pyspark.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,8 +101,11 @@
 
 
 def save_model(tmp_dir: str, model: "pyspark.ml.Model") -> List[str]:
     """Saves the pyspark model"""
     logger.debug("Saving pyspark model")
     target = os.path.join(tmp_dir, "pyspark")
     model.save(target)
-    return [os.path.join(target, "metadata"), os.path.join(target, "stages")]
+    return [
+        os.path.join(target, "metadata"),
+        os.path.join(target, "stages"),
+    ]
```

### Comparing `modelstore-0.0.78/modelstore/models/pytorch.py` & `modelstore-0.0.79/modelstore/models/pytorch.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/modelstore/models/pytorch_lightning.py` & `modelstore-0.0.79/modelstore/models/pytorch_lightning.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/modelstore/models/shap.py` & `modelstore-0.0.79/modelstore/models/shap.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/modelstore/models/sklearn.py` & `modelstore-0.0.79/modelstore/models/sklearn.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/modelstore/models/skorch.py` & `modelstore-0.0.79/modelstore/models/skorch.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/modelstore/models/tensorflow.py` & `modelstore-0.0.79/modelstore/models/tensorflow.py`

 * *Files 20% similar despite different names*

```diff
@@ -46,14 +46,28 @@
         ]
 
     def _required_kwargs(self):
         return ["model"]
 
     def matches_with(self, **kwargs) -> bool:
         # pylint: disable=import-outside-toplevel
+        try:
+            from transformers import TFPreTrainedModel
+
+            # transformer tensorflow models are an instance of keras.Model
+            # but we want to upload them using the transformers manager
+            # we therefore check specifically for this case
+            if isinstance(kwargs.get("model"), TFPreTrainedModel):
+                return False
+        except ImportError:
+            # transformers does not exist
+            pass
+        except RuntimeError:
+            # transformers cannot import tensorflow stuff
+            pass
         from tensorflow import keras
 
         return isinstance(kwargs.get("model"), keras.Model)
 
     def _get_functions(self, **kwargs) -> list:
         model = kwargs["model"]
         return [
```

### Comparing `modelstore-0.0.78/modelstore/models/util.py` & `modelstore-0.0.79/modelstore/models/util.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/modelstore/models/xgboost.py` & `modelstore-0.0.79/modelstore/models/xgboost.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/modelstore/storage/CONTRIBUTING.md` & `modelstore-0.0.79/modelstore/storage/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/modelstore/storage/aws.py` & `modelstore-0.0.79/modelstore/storage/aws.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/modelstore/storage/azure.py` & `modelstore-0.0.79/modelstore/storage/azure.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/modelstore/storage/blob_storage.py` & `modelstore-0.0.79/modelstore/storage/blob_storage.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/modelstore/storage/gcloud.py` & `modelstore-0.0.79/modelstore/storage/gcloud.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/modelstore/storage/local.py` & `modelstore-0.0.79/modelstore/storage/local.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/modelstore/storage/minio.py` & `modelstore-0.0.79/modelstore/storage/minio.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,15 +86,15 @@
     def client(self):
         """Returns the minio client"""
         if self.__client is None:
             self.__client = Minio(
                 self.endpoint,
                 access_key=self.access_key,
                 secret_key=self.secret_key,
-                secure=self.secure
+                secure=self.secure,
             )
         return self.__client
 
     def validate(self) -> bool:
         logger.debug("Querying for bucket=%s...", self.bucket_name)
         return self.client.bucket_exists(self.bucket_name)
```

### Comparing `modelstore-0.0.78/modelstore/storage/states/model_states.py` & `modelstore-0.0.79/modelstore/storage/states/model_states.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/modelstore/storage/storage.py` & `modelstore-0.0.79/modelstore/storage/storage.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/modelstore/storage/util/environment.py` & `modelstore-0.0.79/modelstore/storage/util/environment.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/modelstore/storage/util/paths.py` & `modelstore-0.0.79/modelstore/storage/util/paths.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/modelstore/storage/util/versions.py` & `modelstore-0.0.79/modelstore/storage/util/versions.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/modelstore/utils/cli.py` & `modelstore-0.0.79/modelstore/utils/cli.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/modelstore/utils/exceptions.py` & `modelstore-0.0.79/modelstore/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/modelstore/utils/log.py` & `modelstore-0.0.79/modelstore/utils/log.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/modelstore.egg-info/PKG-INFO` & `modelstore-0.0.79/modelstore.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelstore
-Version: 0.0.78
+Version: 0.0.79
 Summary: modelstore is a library for versioning, exporting, storing, and loading machine learning models
 Home-page: https://github.com/operatorai/modelstore
 Author: Neal Lathia
 License: Please refer to the readme
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `modelstore-0.0.78/modelstore.egg-info/SOURCES.txt` & `modelstore-0.0.79/modelstore.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -50,17 +50,23 @@
 examples/examples-by-ml-library/libraries/raw_file_example.py
 examples/examples-by-ml-library/libraries/shap_example.py
 examples/examples-by-ml-library/libraries/sklearn_example.py
 examples/examples-by-ml-library/libraries/sklearn_with_explainer_example.py
 examples/examples-by-ml-library/libraries/sklearn_with_extras_example.py
 examples/examples-by-ml-library/libraries/skorch_example.py
 examples/examples-by-ml-library/libraries/tensorflow_example.py
-examples/examples-by-ml-library/libraries/transformers_example.py
 examples/examples-by-ml-library/libraries/xgboost_booster_example.py
 examples/examples-by-ml-library/libraries/xgboost_example.py
+examples/examples-by-ml-library/libraries/yolo_example.py
+examples/examples-by-ml-library/libraries/huggingface/__init__.py
+examples/examples-by-ml-library/libraries/huggingface/distilbert.py
+examples/examples-by-ml-library/libraries/huggingface/dpt.py
+examples/examples-by-ml-library/libraries/huggingface/gpt2_pytorch.py
+examples/examples-by-ml-library/libraries/huggingface/gpt2_tensorflow.py
+examples/examples-by-ml-library/libraries/huggingface/sam.py
 examples/examples-by-ml-library/libraries/util/datasets.py
 examples/examples-by-ml-library/libraries/util/domains.py
 modelstore/__init__.py
 modelstore/__main__.py
 modelstore/model_store.py
 modelstore.egg-info/PKG-INFO
 modelstore.egg-info/SOURCES.txt
@@ -116,14 +122,15 @@
 modelstore/models/xgboost.py
 modelstore/storage/CONTRIBUTING.md
 modelstore/storage/__init__.py
 modelstore/storage/aws.py
 modelstore/storage/azure.py
 modelstore/storage/blob_storage.py
 modelstore/storage/gcloud.py
+modelstore/storage/hdfs.py
 modelstore/storage/local.py
 modelstore/storage/minio.py
 modelstore/storage/storage.py
 modelstore/storage/states/__init__.py
 modelstore/storage/states/model_states.py
 modelstore/storage/util/__init__.py
 modelstore/storage/util/environment.py
@@ -189,14 +196,15 @@
 tests/storage/test_aws.py
 tests/storage/test_azure.py
 tests/storage/test_blob_storage.py
 tests/storage/test_blob_storage_artifacts.py
 tests/storage/test_blob_storage_meta_data.py
 tests/storage/test_blob_storage_states.py
 tests/storage/test_gcloud.py
+tests/storage/test_hdfs.py
 tests/storage/test_local.py
 tests/storage/test_minio.py
 tests/storage/test_utils.py
 tests/storage/states/__init__.py
 tests/storage/states/test_model_states.py
 tests/storage/util/__init__.py
 tests/storage/util/test_paths.py
```

### Comparing `modelstore-0.0.78/requirements-dev1.txt` & `modelstore-0.0.79/requirements-dev1.txt`

 * *Files 11% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 
 # Storage
 azure-core>=1.23.1
 azure-storage-blob>=12.11.0
 boto3>=1.21.41
 google-cloud-storage>=2.3.0
 minio>=7.1.12
-
+pydoop<=2.0.0; sys_platform == 'darwin'
 pystan>=2.19.1.1 # required to be installed before prophet
 
 # Machine Learning
 annoy>=1.17.0
 catboost>=1.0.5
 fastai>=2.5.6  # Note: 1.0.61 has different import paths!
 gensim>=4.1.2
 Keras-Preprocessing>=1.1.2
 lightgbm>=3.3.2
 mxnet>=1.8.0.post0
-onnx>=1.11.0 # onnx 1.13.0 depends on protobuf<4 and >=3.20.2, which breaks everything else
+onnx==1.12.0 # onnx 1.13.0 depends on protobuf<4 and >=3.20.2, which breaks everything else
 onnxruntime>=1.11.0
 prophet>=1.0.1
 pyspark>=3.3.1
 pytorch-lightning>=1.6.1
 scikit-learn>=1.0.2
 shap>=0.40.0
 skl2onnx>=1.11.1
```

### Comparing `modelstore-0.0.78/setup.py` & `modelstore-0.0.79/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 # pylint: disable=unspecified-encoding
 with open("requirements.txt", "r") as lines:
     requirements = lines.read().splitlines()
 
 
 setup(
     name="modelstore",
-    version="0.0.78",
-    packages=find_packages(exclude=["tests", "examples", "docs"]),
+    version="0.0.79",
+    packages=find_packages(exclude=["tests", "examples", "docs", "workflows"]),
     include_package_data=True,
     description="modelstore is a library for versioning, exporting, storing, and loading machine learning models",
     long_description="Please refer to: https://modelstore.readthedocs.io/en/latest/",
     long_description_content_type="text/markdown",
     url="https://github.com/operatorai/modelstore",
     author="Neal Lathia",
     classifiers=[
```

### Comparing `modelstore-0.0.78/tests/ids/test_model_ids.py` & `modelstore-0.0.79/tests/ids/test_model_ids.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/tests/metadata/code/test_code.py` & `modelstore-0.0.79/tests/metadata/code/test_code.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/tests/metadata/code/test_dependencies.py` & `modelstore-0.0.79/tests/metadata/code/test_dependencies.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/tests/metadata/code/test_revision.py` & `modelstore-0.0.79/tests/metadata/code/test_revision.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/tests/metadata/code/test_runtime.py` & `modelstore-0.0.79/tests/metadata/code/test_runtime.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/tests/metadata/dataset/fixtures.py` & `modelstore-0.0.79/tests/metadata/dataset/fixtures.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/tests/metadata/dataset/test_dataset.py` & `modelstore-0.0.79/tests/metadata/dataset/test_dataset.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/tests/metadata/dataset/test_features.py` & `modelstore-0.0.79/tests/metadata/dataset/test_features.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/tests/metadata/dataset/test_labels.py` & `modelstore-0.0.79/tests/metadata/dataset/test_labels.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/tests/metadata/dataset/test_types.py` & `modelstore-0.0.79/tests/metadata/dataset/test_types.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/tests/metadata/model/test_model.py` & `modelstore-0.0.79/tests/metadata/model/test_model.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/tests/metadata/model/test_model_type.py` & `modelstore-0.0.79/tests/metadata/model/test_model_type.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/tests/metadata/storage/test_storage.py` & `modelstore-0.0.79/tests/metadata/storage/test_storage.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/tests/metadata/test_metadata.py` & `modelstore-0.0.79/tests/metadata/test_metadata.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/tests/metadata/utils/test_utils.py` & `modelstore-0.0.79/tests/metadata/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/tests/models/test_annoy.py` & `modelstore-0.0.79/tests/models/test_annoy.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/tests/models/test_catboost.py` & `modelstore-0.0.79/tests/models/test_catboost.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/tests/models/test_common.py` & `modelstore-0.0.79/tests/models/test_common.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/tests/models/test_fastai.py` & `modelstore-0.0.79/tests/models/test_fastai.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,9 +152,9 @@
                 git=None,
             ),
             storage=None,
             modelstore=None,
         ),
     )
 
-#     # Expect the two to be the same
+    # Expect the two to be the same
     assert_models_equal(fai_learner, loaded_learner, classification_row)
```

### Comparing `modelstore-0.0.78/tests/models/test_gensim.py` & `modelstore-0.0.79/tests/models/test_gensim.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/tests/models/test_lightgbm.py` & `modelstore-0.0.79/tests/models/test_lightgbm.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/tests/models/test_managers.py` & `modelstore-0.0.79/tests/models/test_managers.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/tests/models/test_missing_manager.py` & `modelstore-0.0.79/tests/models/test_missing_manager.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/tests/models/test_model_file.py` & `modelstore-0.0.79/tests/models/test_model_file.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/tests/models/test_model_manager.py` & `modelstore-0.0.79/tests/models/test_model_manager.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/tests/models/test_multiple_models.py` & `modelstore-0.0.79/tests/models/test_multiple_models.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/tests/models/test_mxnet.py` & `modelstore-0.0.79/tests/models/test_mxnet.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/tests/models/test_onnx.py` & `modelstore-0.0.79/tests/models/test_onnx.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/tests/models/test_prophet.py` & `modelstore-0.0.79/tests/models/test_prophet.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/tests/models/test_pyspark.py` & `modelstore-0.0.79/tests/models/test_pyspark.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 import os
-
+import platform
 import pytest
 from pyspark import SparkContext
 from pyspark.sql import SQLContext
 from pyspark.ml.feature import VectorAssembler
 
 from pyspark.ml import Pipeline
 from pyspark.ml.classification import RandomForestClassifier
@@ -93,15 +93,21 @@
 def test_save_model(spark_model, tmp_path):
     res = pyspark.save_model(tmp_path, spark_model)
     exp = [
         os.path.join(tmp_path, "pyspark", "metadata"),
         os.path.join(tmp_path, "pyspark", "stages"),
     ]
     assert exp == res
-    assert all(os.path.exists(x) for x in exp)
+    exists_fn = os.path.exists
+    if platform.system() == 'Darwin':
+        # Running hadoop locally, so need to check
+        # for the files in hdfs
+        import pydoop.hdfs as hdfs
+        exists_fn = hdfs.path.exists
+    assert all(exists_fn(x) for x in exp)
 
 
 def test_load_model(tmp_path, spark_manager, spark_model, spark_df):
     # Get the model predictions
     y_pred = spark_model.transform(spark_df).toPandas()
 
     # Save the model to a tmp directory
```

### Comparing `modelstore-0.0.78/tests/models/test_pytorch.py` & `modelstore-0.0.79/tests/models/test_pytorch.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/tests/models/test_pytorch_lightning.py` & `modelstore-0.0.79/tests/models/test_pytorch_lightning.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/tests/models/test_shap.py` & `modelstore-0.0.79/tests/models/test_shap.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/tests/models/test_sklearn.py` & `modelstore-0.0.79/tests/models/test_sklearn.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/tests/models/test_skorch.py` & `modelstore-0.0.79/tests/models/test_skorch.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/tests/models/test_tensorflow.py` & `modelstore-0.0.79/tests/models/test_tensorflow.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/tests/models/test_transformers.py` & `modelstore-0.0.79/tests/models/test_transformers.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,15 +23,14 @@
     DistilBertModel,
     DistilBertTokenizerFast,
     PreTrainedTokenizerFast,
 )
 from transformers.file_utils import CONFIG_NAME
 
 from modelstore.metadata import metadata
-from modelstore.metadata.dataset.dataset import Features, Labels
 from modelstore.models.transformers import (
     MODEL_DIRECTORY,
     TransformersManager,
     _save_transformers,
 )
 
 # pylint: disable=protected-access
@@ -79,15 +78,15 @@
 
 def test_model_data(tr_manager, tr_model):
     res = tr_manager.model_data(model=tr_model)
     assert res is None
 
 
 def test_required_kwargs(tr_manager):
-    assert tr_manager._required_kwargs() == ["model", "tokenizer", "config"]
+    assert tr_manager._required_kwargs() == ["model"]
 
 
 def test_matches_with(tr_manager, tr_config, tr_model, tr_tokenizer):
     assert tr_manager.matches_with(
         config=tr_config, model=tr_model, tokenizer=tr_tokenizer
     )
     assert not tr_manager.matches_with(
@@ -111,15 +110,15 @@
     exp = tr_config.to_dict()
     res = tr_manager.get_params(config=tr_config)
     assert exp == res
 
 
 def test_save_transformers(tr_config, tr_model, tr_tokenizer, tmp_path):
     exp = os.path.join(tmp_path, "transformers")
-    file_path = _save_transformers(tmp_path, tr_config, tr_model, tr_tokenizer)
+    file_path = _save_transformers(tmp_path, entities=[tr_config, tr_model, tr_tokenizer])
     assert exp == file_path
 
     # Validate config
     config_file = os.path.join(exp, CONFIG_NAME)
     assert os.path.exists(config_file)
     with open(config_file, "r") as lines:
         config_json = json.loads(lines.read())
@@ -141,13 +140,29 @@
     # Save the model to a tmp directory
     model_dir = os.path.join(tmp_path, MODEL_DIRECTORY)
     tr_model.save_pretrained(model_dir)
     tr_config.save_pretrained(model_dir)
     tr_tokenizer.save_pretrained(model_dir)
 
     #  Load the model
-    loaded_model, loaded_tokenizer, loaded_config = tr_manager.load(tmp_path, None)
+    meta_data = metadata.Summary(
+        model=metadata.Model(
+            domain=None,
+            model_id=None,
+            model_type=metadata.ModelType(
+                library=None,
+                type=type(tr_model).__name__,
+                models=None,
+            ),
+            parameters=None,
+            data=None,
+        ),
+        code=None,
+        storage=None,
+        modelstore=None,
+    )
+    loaded_model, loaded_tokenizer, loaded_config = tr_manager.load(tmp_path, meta_data)
 
     # Expect the two to be the same
     assert isinstance(loaded_model, DistilBertModel)
     assert isinstance(loaded_config, type(tr_config))
     assert isinstance(loaded_tokenizer, DistilBertTokenizerFast)
```

### Comparing `modelstore-0.0.78/tests/models/test_xgboost.py` & `modelstore-0.0.79/tests/models/test_xgboost.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/tests/models/utils.py` & `modelstore-0.0.79/tests/models/utils.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/tests/storage/states/test_model_states.py` & `modelstore-0.0.79/tests/storage/states/test_model_states.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/tests/storage/test_aws.py` & `modelstore-0.0.79/tests/storage/test_aws.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/tests/storage/test_azure.py` & `modelstore-0.0.79/tests/storage/test_azure.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/tests/storage/test_blob_storage.py` & `modelstore-0.0.79/tests/storage/test_blob_storage.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/tests/storage/test_blob_storage_artifacts.py` & `modelstore-0.0.79/tests/storage/test_blob_storage_artifacts.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/tests/storage/test_blob_storage_meta_data.py` & `modelstore-0.0.79/tests/storage/test_blob_storage_meta_data.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/tests/storage/test_blob_storage_states.py` & `modelstore-0.0.79/tests/storage/test_blob_storage_states.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/tests/storage/test_gcloud.py` & `modelstore-0.0.79/tests/storage/test_gcloud.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/tests/storage/test_local.py` & `modelstore-0.0.79/tests/storage/test_local.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/tests/storage/test_minio.py` & `modelstore-0.0.79/tests/storage/test_minio.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/tests/storage/test_utils.py` & `modelstore-0.0.79/tests/storage/test_utils.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/tests/storage/util/test_paths.py` & `modelstore-0.0.79/tests/storage/util/test_paths.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/tests/test_model_store.py` & `modelstore-0.0.79/tests/test_model_store.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/tests/test_model_store_filesystem.py` & `modelstore-0.0.79/tests/test_model_store_filesystem.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/tests/test_model_store_gcp.py` & `modelstore-0.0.79/tests/test_model_store_gcp.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/tests/test_utils.py` & `modelstore-0.0.79/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/workflows/Makefile` & `modelstore-0.0.79/workflows/Makefile`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/workflows/actions/actions.py` & `modelstore-0.0.79/workflows/actions/actions.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/workflows/actions/cli.py` & `modelstore-0.0.79/workflows/actions/cli.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/workflows/actions/models.py` & `modelstore-0.0.79/workflows/actions/models.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/workflows/actions/storage.py` & `modelstore-0.0.79/workflows/actions/storage.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/workflows/fixtures/extra.py` & `modelstore-0.0.79/workflows/fixtures/extra.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/workflows/fixtures/models.py` & `modelstore-0.0.79/workflows/fixtures/models.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/workflows/fixtures/modelstores.py` & `modelstore-0.0.79/workflows/fixtures/modelstores.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.78/workflows/main.py` & `modelstore-0.0.79/workflows/main.py`

 * *Files identical despite different names*

