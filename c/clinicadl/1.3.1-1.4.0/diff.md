# Comparing `tmp/clinicadl-1.3.1.tar.gz` & `tmp/clinicadl-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clinicadl-1.3.1.tar", max compression
+gzip compressed data, was "clinicadl-1.4.0.tar", max compression
```

## Comparing `clinicadl-1.3.1.tar` & `clinicadl-1.4.0.tar`

### file list

```diff
@@ -1,138 +1,147 @@
--rw-r--r--   0        0        0     1093 2023-05-15 15:50:37.044849 clinicadl-1.3.1/LICENSE.txt
--rwxr-xr-x   0        0        0     3737 2023-05-15 15:50:37.044849 clinicadl-1.3.1/README.md
--rw-r--r--   0        0        0      162 2023-05-15 15:50:37.044849 clinicadl-1.3.1/clinicadl/__init__.py
--rw-r--r--   0        0        0     1608 2023-05-15 15:50:37.044849 clinicadl-1.3.1/clinicadl/cmdline.py
--rw-r--r--   0        0        0        0 2023-05-15 15:50:37.044849 clinicadl-1.3.1/clinicadl/generate/__init__.py
--rw-r--r--   0        0        0    21940 2023-05-15 15:50:37.044849 clinicadl-1.3.1/clinicadl/generate/generate.py
--rw-r--r--   0        0        0      797 2023-05-15 15:50:37.044849 clinicadl-1.3.1/clinicadl/generate/generate_cli.py
--rw-r--r--   0        0        0     1760 2023-05-15 15:50:37.044849 clinicadl-1.3.1/clinicadl/generate/generate_hypometabolic_cli.py
--rw-r--r--   0        0        0     1569 2023-05-15 15:50:37.044849 clinicadl-1.3.1/clinicadl/generate/generate_random_cli.py
--rw-r--r--   0        0        0     1637 2023-05-15 15:50:37.044849 clinicadl-1.3.1/clinicadl/generate/generate_shepplogan_cli.py
--rw-r--r--   0        0        0     1759 2023-05-15 15:50:37.044849 clinicadl-1.3.1/clinicadl/generate/generate_trivial_cli.py
--rwxr-xr-x   0        0        0     9883 2023-05-15 15:50:37.044849 clinicadl-1.3.1/clinicadl/generate/generate_utils.py
--rw-r--r--   0        0        0        0 2023-05-15 15:50:37.044849 clinicadl-1.3.1/clinicadl/interpret/__init__.py
--rw-r--r--   0        0        0     4210 2023-05-15 15:50:37.044849 clinicadl-1.3.1/clinicadl/interpret/gradients.py
--rw-r--r--   0        0        0     3524 2023-05-15 15:50:37.044849 clinicadl-1.3.1/clinicadl/interpret/interpret.py
--rw-r--r--   0        0        0     3568 2023-05-15 15:50:37.044849 clinicadl-1.3.1/clinicadl/interpret/interpret_cli.py
--rw-r--r--   0        0        0     2816 2023-05-15 15:50:37.044849 clinicadl-1.3.1/clinicadl/mlflow_test.py
--rw-r--r--   0        0        0        0 2023-05-15 15:50:37.044849 clinicadl-1.3.1/clinicadl/predict/__init__.py
--rw-r--r--   0        0        0     3089 2023-05-15 15:50:37.044849 clinicadl-1.3.1/clinicadl/predict/predict.py
--rw-r--r--   0        0        0     3301 2023-05-15 15:50:37.044849 clinicadl-1.3.1/clinicadl/predict/predict_cli.py
--rw-r--r--   0        0        0        0 2023-05-15 15:50:37.044849 clinicadl-1.3.1/clinicadl/prepare_data/__init__.py
--rw-r--r--   0        0        0     7512 2023-05-15 15:50:37.044849 clinicadl-1.3.1/clinicadl/prepare_data/prepare_data.py
--rw-r--r--   0        0        0     8624 2023-05-15 15:50:37.044849 clinicadl-1.3.1/clinicadl/prepare_data/prepare_data_cli.py
--rw-r--r--   0        0        0    17717 2023-05-15 15:50:37.044849 clinicadl-1.3.1/clinicadl/prepare_data/prepare_data_utils.py
--rw-r--r--   0        0        0        0 2023-05-15 15:50:37.044849 clinicadl-1.3.1/clinicadl/quality_check/__init__.py
--rw-r--r--   0        0        0     1504 2023-05-15 15:50:37.044849 clinicadl-1.3.1/clinicadl/quality_check/pet_linear/cli.py
--rw-r--r--   0        0        0     4484 2023-05-15 15:50:37.044849 clinicadl-1.3.1/clinicadl/quality_check/pet_linear/quality_check.py
--rw-r--r--   0        0        0     1044 2023-05-15 15:50:37.044849 clinicadl-1.3.1/clinicadl/quality_check/pet_linear/utils.py
--rw-r--r--   0        0        0      747 2023-05-15 15:50:37.044849 clinicadl-1.3.1/clinicadl/quality_check/qc_cli.py
--rw-r--r--   0        0        0        0 2023-05-15 15:50:37.044849 clinicadl-1.3.1/clinicadl/quality_check/t1_linear/__init__.py
--rwxr-xr-x   0        0        0     1787 2023-05-15 15:50:37.044849 clinicadl-1.3.1/clinicadl/quality_check/t1_linear/cli.py
--rw-r--r--   0        0        0    22989 2023-05-15 15:50:37.044849 clinicadl-1.3.1/clinicadl/quality_check/t1_linear/models.py
--rwxr-xr-x   0        0        0     5435 2023-05-15 15:50:37.044849 clinicadl-1.3.1/clinicadl/quality_check/t1_linear/quality_check.py
--rwxr-xr-x   0        0        0     8355 2023-05-15 15:50:37.044849 clinicadl-1.3.1/clinicadl/quality_check/t1_linear/utils.py
--rw-r--r--   0        0        0        0 2023-05-15 15:50:37.044849 clinicadl-1.3.1/clinicadl/quality_check/t1_volume/__init__.py
--rw-r--r--   0        0        0      842 2023-05-15 15:50:37.044849 clinicadl-1.3.1/clinicadl/quality_check/t1_volume/cli.py
--rw-r--r--   0        0        0     1823 2023-05-15 15:50:37.044849 clinicadl-1.3.1/clinicadl/quality_check/t1_volume/quality_check.py
--rw-r--r--   0        0        0     4622 2023-05-15 15:50:37.044849 clinicadl-1.3.1/clinicadl/quality_check/t1_volume/utils.py
--rw-r--r--   0        0        0        0 2023-05-15 15:50:37.044849 clinicadl-1.3.1/clinicadl/random_search/__init__.py
--rwxr-xr-x   0        0        0      723 2023-05-15 15:50:37.044849 clinicadl-1.3.1/clinicadl/random_search/random_search.py
--rw-r--r--   0        0        0      628 2023-05-15 15:50:37.044849 clinicadl-1.3.1/clinicadl/random_search/random_search_cli.py
--rw-r--r--   0        0        0     6558 2023-05-15 15:50:37.044849 clinicadl-1.3.1/clinicadl/random_search/random_search_utils.py
--rw-r--r--   0        0        0     1324 2023-05-15 15:50:37.044849 clinicadl-1.3.1/clinicadl/resources/config/train_config.toml
--rw-r--r--   0        0        0      101 2023-05-15 15:50:37.044849 clinicadl-1.3.1/clinicadl/resources/masks/README.md
--rwxr-xr-x   0        0        0        0 2023-05-15 15:50:37.044849 clinicadl-1.3.1/clinicadl/resources/masks/__init__.py
--rw-r--r--   0        0        0      117 2023-05-15 15:50:37.044849 clinicadl-1.3.1/clinicadl/resources/models/README.md
--rwxr-xr-x   0        0        0        0 2023-05-15 15:50:37.044849 clinicadl-1.3.1/clinicadl/resources/models/__init__.py
--rwxr-xr-x   0        0        0       25 2023-05-15 15:50:37.044849 clinicadl-1.3.1/clinicadl/train/__init__.py
--rw-r--r--   0        0        0     1251 2023-05-15 15:50:37.044849 clinicadl-1.3.1/clinicadl/train/from_json_cli.py
--rw-r--r--   0        0        0      773 2023-05-15 15:50:37.044849 clinicadl-1.3.1/clinicadl/train/list_models_cli.py
--rw-r--r--   0        0        0     2057 2023-05-15 15:50:37.044849 clinicadl-1.3.1/clinicadl/train/resume.py
--rw-r--r--   0        0        0      526 2023-05-15 15:50:37.044849 clinicadl-1.3.1/clinicadl/train/resume_cli.py
--rw-r--r--   0        0        0        0 2023-05-15 15:50:37.044849 clinicadl-1.3.1/clinicadl/train/tasks/__init__.py
--rw-r--r--   0        0        0     2354 2023-05-15 15:50:37.044849 clinicadl-1.3.1/clinicadl/train/tasks/classification_cli.py
--rw-r--r--   0        0        0     2190 2023-05-15 15:50:37.044849 clinicadl-1.3.1/clinicadl/train/tasks/reconstruction_cli.py
--rw-r--r--   0        0        0     2203 2023-05-15 15:50:37.044849 clinicadl-1.3.1/clinicadl/train/tasks/regression_cli.py
--rw-r--r--   0        0        0     3589 2023-05-15 15:50:37.044849 clinicadl-1.3.1/clinicadl/train/tasks/task_utils.py
--rw-r--r--   0        0        0      377 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/train/train.py
--rw-r--r--   0        0        0      707 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/train/train_cli.py
--rw-r--r--   0        0        0     8541 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/train/train_option.py
--rw-r--r--   0        0        0     6102 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/train/train_utils.py
--rw-r--r--   0        0        0        0 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/tsvtools/__init__.py
--rw-r--r--   0        0        0        0 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/tsvtools/adapt/__init__.py
--rw-r--r--   0        0        0     3692 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/tsvtools/adapt/adapt.py
--rw-r--r--   0        0        0     1136 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/tsvtools/adapt/adapt_cli.py
--rw-r--r--   0        0        0       44 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/tsvtools/analysis/__init__.py
--rw-r--r--   0        0        0     7885 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/tsvtools/analysis/analysis.py
--rw-r--r--   0        0        0      670 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/tsvtools/analysis/analysis_cli.py
--rw-r--r--   0        0        0     1268 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/tsvtools/cli.py
--rw-r--r--   0        0        0       60 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/tsvtools/get_labels/__init__.py
--rw-r--r--   0        0        0    15681 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/tsvtools/get_labels/get_labels.py
--rw-r--r--   0        0        0     2571 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/tsvtools/get_labels/get_labels_cli.py
--rw-r--r--   0        0        0     2601 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/tsvtools/get_labels/old_get_labels_cli.py
--rw-r--r--   0        0        0        0 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/tsvtools/get_metadata/__init__.py
--rw-r--r--   0        0        0     2465 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/tsvtools/get_metadata/get_metadata.py
--rw-r--r--   0        0        0      964 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/tsvtools/get_metadata/get_metadata_cli.py
--rw-r--r--   0        0        0       45 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/tsvtools/get_progression/__init__.py
--rw-r--r--   0        0        0     7525 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/tsvtools/get_progression/get_progression.py
--rw-r--r--   0        0        0      811 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/tsvtools/get_progression/get_progression_cli.py
--rw-r--r--   0        0        0    23294 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/tsvtools/getlabels/getlabels.py
--rw-r--r--   0        0        0       35 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/tsvtools/kfold/__init__.py
--rw-r--r--   0        0        0     6369 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/tsvtools/kfold/kfold.py
--rw-r--r--   0        0        0     1170 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/tsvtools/kfold/kfold_cli.py
--rw-r--r--   0        0        0     3997 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/tsvtools/prepare_experiment/prepare_experiment_cli.py
--rw-r--r--   0        0        0       35 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/tsvtools/split/__init__.py
--rw-r--r--   0        0        0    12006 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/tsvtools/split/split.py
--rw-r--r--   0        0        0     2470 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/tsvtools/split/split_cli.py
--rw-r--r--   0        0        0        0 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/utils/__init__.py
--rw-r--r--   0        0        0        0 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/utils/caps_dataset/__init__.py
--rw-r--r--   0        0        0    39601 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/utils/caps_dataset/data.py
--rw-r--r--   0        0        0       45 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/utils/cli_param/__init__.py
--rw-r--r--   0        0        0     1465 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/utils/cli_param/argument.py
--rw-r--r--   0        0        0     5309 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/utils/cli_param/option.py
--rw-r--r--   0        0        0      897 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/utils/cli_param/option_group.py
--rw-r--r--   0        0        0      264 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/utils/cmdline_utils.py
--rw-r--r--   0        0        0      803 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/utils/descriptors.py
--rw-r--r--   0        0        0     1264 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/utils/early_stopping.py
--rw-r--r--   0        0        0      755 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/utils/exceptions.py
--rw-r--r--   0        0        0     2362 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/utils/logger.py
--rw-r--r--   0        0        0      192 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/utils/maps_manager/__init__.py
--rw-r--r--   0        0        0    11591 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/utils/maps_manager/iotools.py
--rw-r--r--   0        0        0     4480 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/utils/maps_manager/logwriter.py
--rw-r--r--   0        0        0    86481 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/utils/maps_manager/maps_manager.py
--rw-r--r--   0        0        0     8725 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/utils/maps_manager/maps_manager_utils.py
--rw-r--r--   0        0        0        0 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/utils/meta_maps/__init__.py
--rw-r--r--   0        0        0     2412 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/utils/meta_maps/getter.py
--rw-r--r--   0        0        0    10173 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/utils/metric_module.py
--rw-r--r--   0        0        0      354 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/utils/network/__init__.py
--rw-r--r--   0        0        0        0 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/utils/network/autoencoder/__init__.py
--rw-r--r--   0        0        0     4751 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/utils/network/autoencoder/cnn_transformer.py
--rw-r--r--   0        0        0     1496 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/utils/network/autoencoder/models.py
--rw-r--r--   0        0        0     4491 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/utils/network/cnn/SECNN.py
--rw-r--r--   0        0        0        0 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/utils/network/cnn/__init__.py
--rw-r--r--   0        0        0    10360 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/utils/network/cnn/models.py
--rw-r--r--   0        0        0     8632 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/utils/network/cnn/random.py
--rw-r--r--   0        0        0     2394 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/utils/network/cnn/resnet.py
--rw-r--r--   0        0        0     3033 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/utils/network/cnn/resnet3D.py
--rw-r--r--   0        0        0     2822 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/utils/network/network.py
--rw-r--r--   0        0        0     4065 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/utils/network/network_utils.py
--rw-r--r--   0        0        0     4377 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/utils/network/sub_network.py
--rw-r--r--   0        0        0        0 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/utils/network/vae/__init__.py
--rw-r--r--   0        0        0     2238 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/utils/network/vae/base_vae.py
--rw-r--r--   0        0        0    10052 2023-05-15 15:50:37.052850 clinicadl-1.3.1/clinicadl/utils/network/vae/vae_utils.py
--rw-r--r--   0        0        0    12099 2023-05-15 15:50:37.052850 clinicadl-1.3.1/clinicadl/utils/network/vae/vanilla_vae.py
--rw-r--r--   0        0        0     1280 2023-05-15 15:50:37.052850 clinicadl-1.3.1/clinicadl/utils/preprocessing.py
--rw-r--r--   0        0        0     3661 2023-05-15 15:50:37.052850 clinicadl-1.3.1/clinicadl/utils/seed.py
--rw-r--r--   0        0        0       68 2023-05-15 15:50:37.052850 clinicadl-1.3.1/clinicadl/utils/split_manager/__init__.py
--rw-r--r--   0        0        0     1133 2023-05-15 15:50:37.052850 clinicadl-1.3.1/clinicadl/utils/split_manager/kfold.py
--rw-r--r--   0        0        0      798 2023-05-15 15:50:37.052850 clinicadl-1.3.1/clinicadl/utils/split_manager/single_split.py
--rw-r--r--   0        0        0     9703 2023-05-15 15:50:37.052850 clinicadl-1.3.1/clinicadl/utils/split_manager/split_manager.py
--rw-r--r--   0        0        0      142 2023-05-15 15:50:37.052850 clinicadl-1.3.1/clinicadl/utils/task_manager/__init__.py
--rw-r--r--   0        0        0     7162 2023-05-15 15:50:37.052850 clinicadl-1.3.1/clinicadl/utils/task_manager/classification.py
--rw-r--r--   0        0        0     3540 2023-05-15 15:50:37.052850 clinicadl-1.3.1/clinicadl/utils/task_manager/reconstruction.py
--rw-r--r--   0        0        0     5471 2023-05-15 15:50:37.052850 clinicadl-1.3.1/clinicadl/utils/task_manager/regression.py
--rw-r--r--   0        0        0     6976 2023-05-15 15:50:37.052850 clinicadl-1.3.1/clinicadl/utils/task_manager/task_manager.py
--rw-r--r--   0        0        0     9396 2023-05-15 15:50:37.052850 clinicadl-1.3.1/clinicadl/utils/tsvtools_utils.py
--rw-r--r--   0        0        0     2068 2023-05-15 15:50:37.060850 clinicadl-1.3.1/pyproject.toml
--rw-r--r--   0        0        0     5356 1970-01-01 00:00:00.000000 clinicadl-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1093 2023-06-09 13:43:29.759595 clinicadl-1.4.0/LICENSE.txt
+-rwxr-xr-x   0        0        0     3737 2023-06-09 13:43:29.759595 clinicadl-1.4.0/README.md
+-rw-r--r--   0        0        0      162 2023-06-09 13:43:29.759595 clinicadl-1.4.0/clinicadl/__init__.py
+-rw-r--r--   0        0        0     1608 2023-06-09 13:43:29.759595 clinicadl-1.4.0/clinicadl/cmdline.py
+-rw-r--r--   0        0        0        0 2023-06-09 13:43:29.759595 clinicadl-1.4.0/clinicadl/generate/__init__.py
+-rw-r--r--   0        0        0    27563 2023-06-09 13:43:29.759595 clinicadl-1.4.0/clinicadl/generate/generate.py
+-rw-r--r--   0        0        0      918 2023-06-09 13:43:29.759595 clinicadl-1.4.0/clinicadl/generate/generate_cli.py
+-rw-r--r--   0        0        0     1760 2023-06-09 13:43:29.759595 clinicadl-1.4.0/clinicadl/generate/generate_hypometabolic_cli.py
+-rw-r--r--   0        0        0     1629 2023-06-09 13:43:29.759595 clinicadl-1.4.0/clinicadl/generate/generate_random_cli.py
+-rw-r--r--   0        0        0     1697 2023-06-09 13:43:29.759595 clinicadl-1.4.0/clinicadl/generate/generate_shepplogan_cli.py
+-rw-r--r--   0        0        0     1819 2023-06-09 13:43:29.759595 clinicadl-1.4.0/clinicadl/generate/generate_trivial_cli.py
+-rw-r--r--   0        0        0     1815 2023-06-09 13:43:29.759595 clinicadl-1.4.0/clinicadl/generate/generate_trivial_motion_cli.py
+-rwxr-xr-x   0        0        0     9883 2023-06-09 13:43:29.759595 clinicadl-1.4.0/clinicadl/generate/generate_utils.py
+-rw-r--r--   0        0        0        0 2023-06-09 13:43:29.759595 clinicadl-1.4.0/clinicadl/interpret/__init__.py
+-rw-r--r--   0        0        0     4210 2023-06-09 13:43:29.759595 clinicadl-1.4.0/clinicadl/interpret/gradients.py
+-rw-r--r--   0        0        0     3524 2023-06-09 13:43:29.759595 clinicadl-1.4.0/clinicadl/interpret/interpret.py
+-rw-r--r--   0        0        0     3568 2023-06-09 13:43:29.759595 clinicadl-1.4.0/clinicadl/interpret/interpret_cli.py
+-rw-r--r--   0        0        0     2816 2023-06-09 13:43:29.759595 clinicadl-1.4.0/clinicadl/mlflow_test.py
+-rw-r--r--   0        0        0        0 2023-06-09 13:43:29.759595 clinicadl-1.4.0/clinicadl/predict/__init__.py
+-rw-r--r--   0        0        0     3239 2023-06-09 13:43:29.759595 clinicadl-1.4.0/clinicadl/predict/predict.py
+-rw-r--r--   0        0        0     3627 2023-06-09 13:43:29.759595 clinicadl-1.4.0/clinicadl/predict/predict_cli.py
+-rw-r--r--   0        0        0        0 2023-06-09 13:43:29.759595 clinicadl-1.4.0/clinicadl/prepare_data/__init__.py
+-rw-r--r--   0        0        0     7530 2023-06-09 13:43:29.759595 clinicadl-1.4.0/clinicadl/prepare_data/prepare_data.py
+-rw-r--r--   0        0        0     8624 2023-06-09 13:43:29.759595 clinicadl-1.4.0/clinicadl/prepare_data/prepare_data_cli.py
+-rw-r--r--   0        0        0    17717 2023-06-09 13:43:29.759595 clinicadl-1.4.0/clinicadl/prepare_data/prepare_data_utils.py
+-rw-r--r--   0        0        0        0 2023-06-09 13:43:29.759595 clinicadl-1.4.0/clinicadl/quality_check/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-09 13:43:29.759595 clinicadl-1.4.0/clinicadl/quality_check/pet_linear/__init__.py
+-rw-r--r--   0        0        0     1504 2023-06-09 13:43:29.759595 clinicadl-1.4.0/clinicadl/quality_check/pet_linear/cli.py
+-rw-r--r--   0        0        0     4484 2023-06-09 13:43:29.759595 clinicadl-1.4.0/clinicadl/quality_check/pet_linear/quality_check.py
+-rw-r--r--   0        0        0     1040 2023-06-09 13:43:29.759595 clinicadl-1.4.0/clinicadl/quality_check/pet_linear/utils.py
+-rw-r--r--   0        0        0      747 2023-06-09 13:43:29.759595 clinicadl-1.4.0/clinicadl/quality_check/qc_cli.py
+-rw-r--r--   0        0        0        0 2023-06-09 13:43:29.759595 clinicadl-1.4.0/clinicadl/quality_check/t1_linear/__init__.py
+-rwxr-xr-x   0        0        0     1787 2023-06-09 13:43:29.759595 clinicadl-1.4.0/clinicadl/quality_check/t1_linear/cli.py
+-rw-r--r--   0        0        0    22989 2023-06-09 13:43:29.759595 clinicadl-1.4.0/clinicadl/quality_check/t1_linear/models.py
+-rwxr-xr-x   0        0        0     5368 2023-06-09 13:43:29.759595 clinicadl-1.4.0/clinicadl/quality_check/t1_linear/quality_check.py
+-rwxr-xr-x   0        0        0     8355 2023-06-09 13:43:29.759595 clinicadl-1.4.0/clinicadl/quality_check/t1_linear/utils.py
+-rw-r--r--   0        0        0        0 2023-06-09 13:43:29.759595 clinicadl-1.4.0/clinicadl/quality_check/t1_volume/__init__.py
+-rw-r--r--   0        0        0      842 2023-06-09 13:43:29.759595 clinicadl-1.4.0/clinicadl/quality_check/t1_volume/cli.py
+-rw-r--r--   0        0        0     1823 2023-06-09 13:43:29.759595 clinicadl-1.4.0/clinicadl/quality_check/t1_volume/quality_check.py
+-rw-r--r--   0        0        0     4622 2023-06-09 13:43:29.759595 clinicadl-1.4.0/clinicadl/quality_check/t1_volume/utils.py
+-rw-r--r--   0        0        0        0 2023-06-09 13:43:29.759595 clinicadl-1.4.0/clinicadl/random_search/__init__.py
+-rwxr-xr-x   0        0        0      723 2023-06-09 13:43:29.759595 clinicadl-1.4.0/clinicadl/random_search/random_search.py
+-rw-r--r--   0        0        0      628 2023-06-09 13:43:29.759595 clinicadl-1.4.0/clinicadl/random_search/random_search_cli.py
+-rw-r--r--   0        0        0     6558 2023-06-09 13:43:29.759595 clinicadl-1.4.0/clinicadl/random_search/random_search_utils.py
+-rw-r--r--   0        0        0     1394 2023-06-09 13:43:29.759595 clinicadl-1.4.0/clinicadl/resources/config/train_config.toml
+-rw-r--r--   0        0        0      101 2023-06-09 13:43:29.759595 clinicadl-1.4.0/clinicadl/resources/masks/README.md
+-rwxr-xr-x   0        0        0        0 2023-06-09 13:43:29.759595 clinicadl-1.4.0/clinicadl/resources/masks/__init__.py
+-rw-r--r--   0        0        0      117 2023-06-09 13:43:29.759595 clinicadl-1.4.0/clinicadl/resources/models/README.md
+-rwxr-xr-x   0        0        0        0 2023-06-09 13:43:29.759595 clinicadl-1.4.0/clinicadl/resources/models/__init__.py
+-rwxr-xr-x   0        0        0       25 2023-06-09 13:43:29.759595 clinicadl-1.4.0/clinicadl/train/__init__.py
+-rw-r--r--   0        0        0     1251 2023-06-09 13:43:29.759595 clinicadl-1.4.0/clinicadl/train/from_json_cli.py
+-rw-r--r--   0        0        0      773 2023-06-09 13:43:29.759595 clinicadl-1.4.0/clinicadl/train/list_models_cli.py
+-rw-r--r--   0        0        0     2057 2023-06-09 13:43:29.759595 clinicadl-1.4.0/clinicadl/train/resume.py
+-rw-r--r--   0        0        0      536 2023-06-09 13:43:29.759595 clinicadl-1.4.0/clinicadl/train/resume_cli.py
+-rw-r--r--   0        0        0        0 2023-06-09 13:43:29.759595 clinicadl-1.4.0/clinicadl/train/tasks/__init__.py
+-rw-r--r--   0        0        0     2378 2023-06-09 13:43:29.759595 clinicadl-1.4.0/clinicadl/train/tasks/classification_cli.py
+-rw-r--r--   0        0        0     2214 2023-06-09 13:43:29.759595 clinicadl-1.4.0/clinicadl/train/tasks/reconstruction_cli.py
+-rw-r--r--   0        0        0     2227 2023-06-09 13:43:29.759595 clinicadl-1.4.0/clinicadl/train/tasks/regression_cli.py
+-rw-r--r--   0        0        0     3589 2023-06-09 13:43:29.759595 clinicadl-1.4.0/clinicadl/train/tasks/task_utils.py
+-rw-r--r--   0        0        0      377 2023-06-09 13:43:29.759595 clinicadl-1.4.0/clinicadl/train/train.py
+-rw-r--r--   0        0        0      707 2023-06-09 13:43:29.759595 clinicadl-1.4.0/clinicadl/train/train_cli.py
+-rw-r--r--   0        0        0     6102 2023-06-09 13:43:29.759595 clinicadl-1.4.0/clinicadl/train/train_utils.py
+-rw-r--r--   0        0        0        0 2023-06-09 13:43:29.759595 clinicadl-1.4.0/clinicadl/tsvtools/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-09 13:43:29.759595 clinicadl-1.4.0/clinicadl/tsvtools/adapt/__init__.py
+-rw-r--r--   0        0        0     3692 2023-06-09 13:43:29.759595 clinicadl-1.4.0/clinicadl/tsvtools/adapt/adapt.py
+-rw-r--r--   0        0        0     1136 2023-06-09 13:43:29.759595 clinicadl-1.4.0/clinicadl/tsvtools/adapt/adapt_cli.py
+-rw-r--r--   0        0        0       44 2023-06-09 13:43:29.759595 clinicadl-1.4.0/clinicadl/tsvtools/analysis/__init__.py
+-rw-r--r--   0        0        0     7885 2023-06-09 13:43:29.759595 clinicadl-1.4.0/clinicadl/tsvtools/analysis/analysis.py
+-rw-r--r--   0        0        0      670 2023-06-09 13:43:29.759595 clinicadl-1.4.0/clinicadl/tsvtools/analysis/analysis_cli.py
+-rw-r--r--   0        0        0     1268 2023-06-09 13:43:29.759595 clinicadl-1.4.0/clinicadl/tsvtools/cli.py
+-rw-r--r--   0        0        0       60 2023-06-09 13:43:29.759595 clinicadl-1.4.0/clinicadl/tsvtools/get_labels/__init__.py
+-rw-r--r--   0        0        0    15924 2023-06-09 13:43:29.759595 clinicadl-1.4.0/clinicadl/tsvtools/get_labels/get_labels.py
+-rw-r--r--   0        0        0     2571 2023-06-09 13:43:29.759595 clinicadl-1.4.0/clinicadl/tsvtools/get_labels/get_labels_cli.py
+-rw-r--r--   0        0        0     2601 2023-06-09 13:43:29.759595 clinicadl-1.4.0/clinicadl/tsvtools/get_labels/old_get_labels_cli.py
+-rw-r--r--   0        0        0        0 2023-06-09 13:43:29.759595 clinicadl-1.4.0/clinicadl/tsvtools/get_metadata/__init__.py
+-rw-r--r--   0        0        0     2465 2023-06-09 13:43:29.759595 clinicadl-1.4.0/clinicadl/tsvtools/get_metadata/get_metadata.py
+-rw-r--r--   0        0        0      964 2023-06-09 13:43:29.759595 clinicadl-1.4.0/clinicadl/tsvtools/get_metadata/get_metadata_cli.py
+-rw-r--r--   0        0        0       45 2023-06-09 13:43:29.759595 clinicadl-1.4.0/clinicadl/tsvtools/get_progression/__init__.py
+-rw-r--r--   0        0        0     7525 2023-06-09 13:43:29.759595 clinicadl-1.4.0/clinicadl/tsvtools/get_progression/get_progression.py
+-rw-r--r--   0        0        0      811 2023-06-09 13:43:29.759595 clinicadl-1.4.0/clinicadl/tsvtools/get_progression/get_progression_cli.py
+-rw-r--r--   0        0        0    23294 2023-06-09 13:43:29.759595 clinicadl-1.4.0/clinicadl/tsvtools/getlabels/getlabels.py
+-rw-r--r--   0        0        0       35 2023-06-09 13:43:29.759595 clinicadl-1.4.0/clinicadl/tsvtools/kfold/__init__.py
+-rw-r--r--   0        0        0     6369 2023-06-09 13:43:29.759595 clinicadl-1.4.0/clinicadl/tsvtools/kfold/kfold.py
+-rw-r--r--   0        0        0     1170 2023-06-09 13:43:29.763594 clinicadl-1.4.0/clinicadl/tsvtools/kfold/kfold_cli.py
+-rw-r--r--   0        0        0        0 2023-06-09 13:43:29.763594 clinicadl-1.4.0/clinicadl/tsvtools/prepare_experiment/__init__.py
+-rw-r--r--   0        0        0     3997 2023-06-09 13:43:29.763594 clinicadl-1.4.0/clinicadl/tsvtools/prepare_experiment/prepare_experiment_cli.py
+-rw-r--r--   0        0        0       35 2023-06-09 13:43:29.763594 clinicadl-1.4.0/clinicadl/tsvtools/split/__init__.py
+-rw-r--r--   0        0        0    12736 2023-06-09 13:43:29.763594 clinicadl-1.4.0/clinicadl/tsvtools/split/split.py
+-rw-r--r--   0        0        0     2470 2023-06-09 13:43:29.763594 clinicadl-1.4.0/clinicadl/tsvtools/split/split_cli.py
+-rw-r--r--   0        0        0        0 2023-06-09 13:43:29.763594 clinicadl-1.4.0/clinicadl/utils/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-09 13:43:29.763594 clinicadl-1.4.0/clinicadl/utils/caps_dataset/__init__.py
+-rw-r--r--   0        0        0    43098 2023-06-09 13:43:29.763594 clinicadl-1.4.0/clinicadl/utils/caps_dataset/data.py
+-rw-r--r--   0        0        0       45 2023-06-09 13:43:29.763594 clinicadl-1.4.0/clinicadl/utils/cli_param/__init__.py
+-rw-r--r--   0        0        0     1465 2023-06-09 13:43:29.763594 clinicadl-1.4.0/clinicadl/utils/cli_param/argument.py
+-rw-r--r--   0        0        0     5742 2023-06-09 13:43:29.763594 clinicadl-1.4.0/clinicadl/utils/cli_param/option.py
+-rw-r--r--   0        0        0      897 2023-06-09 13:43:29.763594 clinicadl-1.4.0/clinicadl/utils/cli_param/option_group.py
+-rw-r--r--   0        0        0     8541 2023-06-09 13:43:29.763594 clinicadl-1.4.0/clinicadl/utils/cli_param/train_option.py
+-rw-r--r--   0        0        0      264 2023-06-09 13:43:29.763594 clinicadl-1.4.0/clinicadl/utils/cmdline_utils.py
+-rw-r--r--   0        0        0      803 2023-06-09 13:43:29.763594 clinicadl-1.4.0/clinicadl/utils/descriptors.py
+-rw-r--r--   0        0        0     1264 2023-06-09 13:43:29.763594 clinicadl-1.4.0/clinicadl/utils/early_stopping.py
+-rw-r--r--   0        0        0      755 2023-06-09 13:43:29.763594 clinicadl-1.4.0/clinicadl/utils/exceptions.py
+-rw-r--r--   0        0        0     2336 2023-06-09 13:43:29.763594 clinicadl-1.4.0/clinicadl/utils/logger.py
+-rw-r--r--   0        0        0      192 2023-06-09 13:43:29.763594 clinicadl-1.4.0/clinicadl/utils/maps_manager/__init__.py
+-rw-r--r--   0        0        0    11591 2023-06-09 13:43:29.763594 clinicadl-1.4.0/clinicadl/utils/maps_manager/iotools.py
+-rw-r--r--   0        0        0     4480 2023-06-09 13:43:29.763594 clinicadl-1.4.0/clinicadl/utils/maps_manager/logwriter.py
+-rw-r--r--   0        0        0    90207 2023-06-09 13:43:29.763594 clinicadl-1.4.0/clinicadl/utils/maps_manager/maps_manager.py
+-rw-r--r--   0        0        0     8725 2023-06-09 13:43:29.763594 clinicadl-1.4.0/clinicadl/utils/maps_manager/maps_manager_utils.py
+-rw-r--r--   0        0        0        0 2023-06-09 13:43:29.763594 clinicadl-1.4.0/clinicadl/utils/meta_maps/__init__.py
+-rw-r--r--   0        0        0     2412 2023-06-09 13:43:29.763594 clinicadl-1.4.0/clinicadl/utils/meta_maps/getter.py
+-rw-r--r--   0        0        0    11087 2023-06-09 13:43:29.763594 clinicadl-1.4.0/clinicadl/utils/metric_module.py
+-rw-r--r--   0        0        0      515 2023-06-09 13:43:29.763594 clinicadl-1.4.0/clinicadl/utils/network/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-09 13:43:29.763594 clinicadl-1.4.0/clinicadl/utils/network/autoencoder/__init__.py
+-rw-r--r--   0        0        0     4751 2023-06-09 13:43:29.763594 clinicadl-1.4.0/clinicadl/utils/network/autoencoder/cnn_transformer.py
+-rw-r--r--   0        0        0     2511 2023-06-09 13:43:29.763594 clinicadl-1.4.0/clinicadl/utils/network/autoencoder/models.py
+-rw-r--r--   0        0        0     4468 2023-06-09 13:43:29.763594 clinicadl-1.4.0/clinicadl/utils/network/cnn/SECNN.py
+-rw-r--r--   0        0        0        0 2023-06-09 13:43:29.763594 clinicadl-1.4.0/clinicadl/utils/network/cnn/__init__.py
+-rw-r--r--   0        0        0    10360 2023-06-09 13:43:29.763594 clinicadl-1.4.0/clinicadl/utils/network/cnn/models.py
+-rw-r--r--   0        0        0     8632 2023-06-09 13:43:29.763594 clinicadl-1.4.0/clinicadl/utils/network/cnn/random.py
+-rw-r--r--   0        0        0     2394 2023-06-09 13:43:29.763594 clinicadl-1.4.0/clinicadl/utils/network/cnn/resnet.py
+-rw-r--r--   0        0        0     3010 2023-06-09 13:43:29.763594 clinicadl-1.4.0/clinicadl/utils/network/cnn/resnet3D.py
+-rw-r--r--   0        0        0     2822 2023-06-09 13:43:29.763594 clinicadl-1.4.0/clinicadl/utils/network/network.py
+-rw-r--r--   0        0        0     5181 2023-06-09 13:43:29.763594 clinicadl-1.4.0/clinicadl/utils/network/network_utils.py
+-rw-r--r--   0        0        0     4377 2023-06-09 13:43:29.763594 clinicadl-1.4.0/clinicadl/utils/network/sub_network.py
+-rw-r--r--   0        0        0        0 2023-06-09 13:43:29.763594 clinicadl-1.4.0/clinicadl/utils/network/unet/__init__.py
+-rw-r--r--   0        0        0     3151 2023-06-09 13:43:29.763594 clinicadl-1.4.0/clinicadl/utils/network/unet/unet.py
+-rw-r--r--   0        0        0        0 2023-06-09 13:43:29.763594 clinicadl-1.4.0/clinicadl/utils/network/vae/__init__.py
+-rw-r--r--   0        0        0     5503 2023-06-09 13:43:29.763594 clinicadl-1.4.0/clinicadl/utils/network/vae/advanced_CVAE.py
+-rw-r--r--   0        0        0     2359 2023-06-09 13:43:29.763594 clinicadl-1.4.0/clinicadl/utils/network/vae/base_vae.py
+-rw-r--r--   0        0        0    11247 2023-06-09 13:43:29.763594 clinicadl-1.4.0/clinicadl/utils/network/vae/convolutional_VAE.py
+-rw-r--r--   0        0        0    10599 2023-06-09 13:43:29.763594 clinicadl-1.4.0/clinicadl/utils/network/vae/vae_layers.py
+-rw-r--r--   0        0        0     2886 2023-06-09 13:43:29.763594 clinicadl-1.4.0/clinicadl/utils/network/vae/vae_utils.py
+-rw-r--r--   0        0        0    12199 2023-06-09 13:43:29.763594 clinicadl-1.4.0/clinicadl/utils/network/vae/vanilla_vae.py
+-rw-r--r--   0        0        0     1280 2023-06-09 13:43:29.763594 clinicadl-1.4.0/clinicadl/utils/preprocessing.py
+-rw-r--r--   0        0        0     5612 2023-06-09 13:43:29.763594 clinicadl-1.4.0/clinicadl/utils/pytorch_ssim.py
+-rw-r--r--   0        0        0     3661 2023-06-09 13:43:29.763594 clinicadl-1.4.0/clinicadl/utils/seed.py
+-rw-r--r--   0        0        0       68 2023-06-09 13:43:29.763594 clinicadl-1.4.0/clinicadl/utils/split_manager/__init__.py
+-rw-r--r--   0        0        0     1168 2023-06-09 13:43:29.763594 clinicadl-1.4.0/clinicadl/utils/split_manager/kfold.py
+-rw-r--r--   0        0        0      805 2023-06-09 13:43:29.763594 clinicadl-1.4.0/clinicadl/utils/split_manager/single_split.py
+-rw-r--r--   0        0        0     9869 2023-06-09 13:43:29.763594 clinicadl-1.4.0/clinicadl/utils/split_manager/split_manager.py
+-rw-r--r--   0        0        0      142 2023-06-09 13:43:29.763594 clinicadl-1.4.0/clinicadl/utils/task_manager/__init__.py
+-rw-r--r--   0        0        0     7162 2023-06-09 13:43:29.763594 clinicadl-1.4.0/clinicadl/utils/task_manager/classification.py
+-rw-r--r--   0        0        0     4164 2023-06-09 13:43:29.763594 clinicadl-1.4.0/clinicadl/utils/task_manager/reconstruction.py
+-rw-r--r--   0        0        0     5471 2023-06-09 13:43:29.763594 clinicadl-1.4.0/clinicadl/utils/task_manager/regression.py
+-rw-r--r--   0        0        0     7704 2023-06-09 13:43:29.763594 clinicadl-1.4.0/clinicadl/utils/task_manager/task_manager.py
+-rw-r--r--   0        0        0     9396 2023-06-09 13:43:29.763594 clinicadl-1.4.0/clinicadl/utils/tsvtools_utils.py
+-rw-r--r--   0        0        0     2089 2023-06-09 13:43:29.771595 clinicadl-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0     5399 1970-01-01 00:00:00.000000 clinicadl-1.4.0/PKG-INFO
```

### Comparing `clinicadl-1.3.1/LICENSE.txt` & `clinicadl-1.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.1/README.md` & `clinicadl-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.1/clinicadl/cmdline.py` & `clinicadl-1.4.0/clinicadl/cmdline.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.1/clinicadl/generate/generate.py` & `clinicadl-1.4.0/clinicadl/generate/generate.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,21 +2,23 @@
 
 """
 This file generates data for trivial or intractable (random) data for binary classification.
 """
 import tarfile
 from logging import getLogger
 from pathlib import Path
-from typing import Dict, Optional, Tuple
+from typing import Dict, List, Optional, Tuple
 
 import nibabel as nib
 import numpy as np
 import pandas as pd
 import torch
+import torchio as tio
 from clinica.utils.inputs import RemoteFileStructure, clinica_file_reader, fetch_file
+from clinica.utils.participant import get_subject_session_list
 from joblib import Parallel, delayed
 from nilearn.image import resample_to_img
 
 from clinicadl.prepare_data.prepare_data_utils import compute_extract_json
 from clinicadl.utils.caps_dataset.data import CapsDataset
 from clinicadl.utils.exceptions import DownloadError
 from clinicadl.utils.maps_manager.iotools import check_and_clean, commandline_to_json
@@ -35,14 +37,15 @@
 logger = getLogger("clinicadl.generate")
 
 
 def generate_random_dataset(
     caps_directory: Path,
     output_dir: Path,
     n_subjects: int,
+    n_proc: int,
     tsv_path: Optional[Path] = None,
     mean: float = 0,
     sigma: float = 0.5,
     preprocessing: str = "t1-linear",
     multi_cohort: bool = False,
     uncropped_image: bool = False,
     tracer: Optional[str] = None,
@@ -88,14 +91,15 @@
     """
     commandline_to_json(
         {
             "output_dir": output_dir,
             "caps_dir": caps_directory,
             "preprocessing": preprocessing,
             "n_subjects": n_subjects,
+            "n_proc": n_proc,
             "mean": mean,
             "sigma": sigma,
         }
     )
     # Transform caps_directory in dict
     caps_dict = CapsDataset.create_caps_dict(caps_directory, multi_cohort=multi_cohort)
 
@@ -134,38 +138,43 @@
     )
     output_df["age_bl"] = 60
     output_df["sex"] = "F"
     output_df.to_csv(output_dir / "data.tsv", sep="\t", index=False)
 
     input_filename = image_path.name
     filename_pattern = "_".join(input_filename.split("_")[2::])
-    for i in range(2 * n_subjects):
+
+    def create_random_image(subject_id):
         gauss = np.random.normal(mean, sigma, image.shape)
-        participant_id = f"sub-RAND{i}"
+        participant_id = f"sub-RAND{subject_id}"
         noisy_image = image + gauss
         noisy_image_nii = nib.Nifti1Image(
             noisy_image, header=image_nii.header, affine=image_nii.affine
         )
         noisy_image_nii_path = (
             output_dir / "subjects" / participant_id / "ses-M00" / "t1_linear"
         )
 
         noisy_image_nii_filename = f"{participant_id}_ses-M00_{filename_pattern}"
         noisy_image_nii_path.mkdir(parents=True, exist_ok=True)
         nib.save(noisy_image_nii, noisy_image_nii_path / noisy_image_nii_filename)
 
-    write_missing_mods(output_dir, output_df)
+    Parallel(n_jobs=n_proc)(
+        delayed(create_random_image)(subject_id) for subject_id in range(2 * n_subjects)
+    )
 
+    write_missing_mods(output_dir, output_df)
     logger.info(f"Random dataset was generated at {output_dir}")
 
 
 def generate_trivial_dataset(
     caps_directory: Path,
     output_dir: Path,
     n_subjects: int,
+    n_proc: int,
     tsv_path: Optional[Path] = None,
     preprocessing: str = "t1-linear",
     mask_path: Optional[Path] = None,
     atrophy_percent: float = 60,
     multi_cohort: bool = False,
     uncropped_image: bool = False,
     tracer: str = "fdg",
@@ -217,14 +226,15 @@
 
     commandline_to_json(
         {
             "output_dir": output_dir,
             "caps_dir": caps_directory,
             "preprocessing": preprocessing,
             "n_subjects": n_subjects,
+            "n_proc": n_proc,
             "atrophy_percent": atrophy_percent,
         }
     )
 
     # Transform caps_directory in dict
     caps_dict = CapsDataset.create_caps_dict(caps_directory, multi_cohort=multi_cohort)
     # Read DataFrame
@@ -279,17 +289,17 @@
     diagnosis_list = ["AD", "CN"]
 
     # Find appropriate preprocessing file type
     file_type = find_file_type(
         preprocessing, uncropped_image, tracer, suvr_reference_region
     )
 
-    for i in range(2 * n_subjects):
-        data_idx = i // 2
-        label = i % 2
+    def create_trivial_image(subject_id, output_df):
+        data_idx = subject_id // 2
+        label = subject_id % 2
 
         participant_id = data_df.loc[data_idx, "participant_id"]
         session_id = data_df.loc[data_idx, "session_id"]
         cohort = data_df.loc[data_idx, "cohort"]
         image_path = Path(
             clinica_file_reader(
                 [participant_id], [session_id], caps_dict[cohort], file_type
@@ -298,18 +308,24 @@
         image_nii = nib.load(image_path)
         image = image_nii.get_data()
 
         input_filename = image_path.name
         filename_pattern = "_".join(input_filename.split("_")[2::])
 
         trivial_image_nii_dir = (
-            output_dir / "subjects" / f"sub-TRIV{i}" / session_id / preprocessing
+            output_dir
+            / "subjects"
+            / f"sub-TRIV{subject_id}"
+            / session_id
+            / preprocessing
         )
 
-        trivial_image_nii_filename = f"sub-TRIV{i}_{session_id}_{filename_pattern}"
+        trivial_image_nii_filename = (
+            f"sub-TRIV{subject_id}_{session_id}_{filename_pattern}"
+        )
 
         trivial_image_nii_dir.mkdir(parents=True, exist_ok=True)
 
         atlas_to_mask = nib.load(mask_path / f"mask-{label + 1}.nii").get_data()
 
         # Create atrophied image
         trivial_image = im_loss_roi_gaussian_distribution(
@@ -317,28 +333,37 @@
         )
         trivial_image_nii = nib.Nifti1Image(trivial_image, affine=image_nii.affine)
         trivial_image_nii.to_filename(
             trivial_image_nii_dir / trivial_image_nii_filename
         )
 
         # Append row to output tsv
-        row = [f"sub-TRIV{i}", session_id, diagnosis_list[label], 60, "F"]
+        row = [f"sub-TRIV{subject_id}", session_id, diagnosis_list[label], 60, "F"]
         row_df = pd.DataFrame([row], columns=columns)
         output_df = pd.concat([output_df, row_df])
 
-    output_df.to_csv(output_dir / "data.tsv", sep="\t", index=False)
+        return output_df
 
-    write_missing_mods(output_dir, output_df)
+    results_df = Parallel(n_jobs=n_proc)(
+        delayed(create_trivial_image)(subject_id, output_df)
+        for subject_id in range(2 * n_subjects)
+    )
+    output_df = pd.DataFrame()
+    for result in results_df:
+        output_df = pd.concat([result, output_df])
 
+    output_df.to_csv(output_dir / "data.tsv", sep="\t", index=False)
+    write_missing_mods(output_dir, output_df)
     logger.info(f"Trivial dataset was generated at {output_dir}")
 
 
 def generate_shepplogan_dataset(
     output_dir: Path,
     img_size: int,
+    n_proc: int,
     labels_distribution: Dict[str, Tuple[float, float, float]],
     extract_json: str = None,
     samples: int = 100,
     smoothing: bool = True,
 ):
     """
     Creates a CAPS data set of synthetic data based on Shepp-Logan phantom.
@@ -362,17 +387,19 @@
             "samples": samples,
             "smoothing": smoothing,
         }
     )
     columns = ["participant_id", "session_id", "diagnosis", "subtype"]
     data_df = pd.DataFrame(columns=columns)
 
-    for i, label in enumerate(labels_distribution.keys()):
-        for j in range(samples):
-            participant_id = f"sub-CLNC{i}{j:04d}"
+    for label_id, label in enumerate(labels_distribution.keys()):
+
+        def create_shepplogan_image(subject_id, data_df):
+            # for j in range(samples):
+            participant_id = f"sub-CLNC{label_id}{subject_id:04d}"
             session_id = "ses-M00"
             subtype = np.random.choice(
                 np.arange(len(labels_distribution[label])), p=labels_distribution[label]
             )
             row_df = pd.DataFrame(
                 [[participant_id, session_id, label, subtype]], columns=columns
             )
@@ -388,15 +415,14 @@
                 / "slice_based"
                 / "custom"
                 / f"{participant_id}_{session_id}_space-SheppLogan_axis-axi_channel-single_slice-0_phantom.pt"
             )
 
             slice_dir = slice_path.parent
             slice_dir.mkdir(parents=True, exist_ok=True)
-
             slice_np = generate_shepplogan_phantom(
                 img_size, label=subtype, smoothing=smoothing
             )
             slice_tensor = torch.from_numpy(slice_np).float().unsqueeze(0)
             torch.save(slice_tensor, slice_path)
 
             image_path = (
@@ -407,14 +433,24 @@
                 / "shepplogan"
                 / f"{participant_id}_{session_id}_space-SheppLogan_phantom.nii.gz"
             )
             image_dir = image_path.parent
             image_dir.mkdir(parents=True, exist_ok=True)
             with image_path.open("w") as f:
                 f.write("0")
+            return data_df
+
+        results_df = Parallel(n_jobs=n_proc)(
+            delayed(create_shepplogan_image)(subject_id, data_df)
+            for subject_id in range(samples)
+        )
+
+        data_df = pd.DataFrame()
+        for result in results_df:
+            data_df = pd.concat([result, data_df])
 
     # Save data
     data_df.to_csv(output_dir / "data.tsv", sep="\t", index=False)
 
     # Save preprocessing JSON file
     preprocessing_dict = {
         "preprocessing": "custom",
@@ -564,53 +600,177 @@
     mask = mask_resample_nii.get_fdata()
 
     mask = mask_processing(mask, anomaly_degree, sigma)
 
     # Create subjects dir
     (output_dir / "subjects").mkdir(parents=True, exist_ok=True)
 
-    def generate_hypometabolic_image(i, output_df):
-        image_path = Path(images_paths[i])
+    def generate_hypometabolic_image(subject_id, output_df):
+        image_path = Path(images_paths[subject_id])
         image_nii = nib.load(image_path)
         image = image_nii.get_fdata()
         if image_path.suffix == ".gz":
             input_filename = Path(image_path.stem).stem
         else:
             input_filename = image_path.stem
         input_filename = input_filename.strip("pet")
         hypo_image_nii_dir = (
-            output_dir / "subjects" / participants[i] / sessions[i] / preprocessing
+            output_dir
+            / "subjects"
+            / participants[subject_id]
+            / sessions[subject_id]
+            / preprocessing
         )
         hypo_image_nii_filename = (
             f"{input_filename}pat-{pathology}_deg-{int(anomaly_degree)}_pet.nii.gz"
         )
         hypo_image_nii_dir.mkdir(parents=True, exist_ok=True)
 
         # Create atrophied image
         hypo_image = image * mask
         hypo_image_nii = nib.Nifti1Image(hypo_image, affine=image_nii.affine)
         hypo_image_nii.to_filename(hypo_image_nii_dir / hypo_image_nii_filename)
 
         # Append row to output tsv
         row = [
-            participants[i],
-            sessions[i],
+            participants[subject_id],
+            sessions[subject_id],
             pathology,
             anomaly_degree,
         ]
         row_df = pd.DataFrame([row], columns=columns)
         output_df = pd.concat([output_df, row_df])
         return output_df
 
     results_list = Parallel(n_jobs=n_proc)(
-        delayed(generate_hypometabolic_image)(i, output_df) for i in range(n_subjects)
+        delayed(generate_hypometabolic_image)(subject_id, output_df)
+        for subject_id in range(n_subjects)
     )
+
+    output_df = pd.DataFrame()
     for result_df in results_list:
         output_df = pd.concat([result_df, output_df])
 
     output_df.to_csv(output_dir / "data.tsv", sep="\t", index=False)
 
     write_missing_mods(output_dir, output_df)
 
     logger.info(
         f"Hypometabolic dataset was generated, with {anomaly_degree} % of dementia {pathology} at {output_dir}."
     )
+
+
+def generate_motion_dataset(
+    caps_directory: Path,
+    output_dir: Path,
+    n_proc: int,
+    tsv_path: Optional[str] = None,
+    preprocessing: str = "t1-linear",
+    multi_cohort: bool = False,
+    uncropped_image: bool = False,
+    tracer: str = "fdg",
+    suvr_reference_region: str = "pons",
+    translation: List = [2, 4],
+    rotation: List = [2, 4],
+    num_transforms: int = 2,
+):
+    """
+    Generates a fully separable dataset.
+    Generates a dataset, based on the images of the CAPS directory, where a
+    half of the image is corrupted with motion artefacts using the image-based simulation of torchio.
+    Args:
+        caps_directory: path to the CAPS directory.
+        output_dir: folder containing the synthetic dataset in CAPS format.
+        n_subjects: number of subjects in each class of the synthetic dataset.
+        tsv_path: path to tsv file of list of subjects/sessions.
+        preprocessing: preprocessing performed. Must be in ['linear', 'extensive'].
+        multi_cohort: If True caps_directory is the path to a TSV file linking cohort names and paths.
+        uncropped_image: If True the uncropped image of `t1-linear` or `pet-linear` will be used.
+        tracer: name of the tracer when using `pet-linear` preprocessing.
+        suvr_reference_region: name of the reference region when using `pet-linear` preprocessing.
+    Returns:
+        Folder structure where images are stored in CAPS format.
+    Raises:
+        IndexError: if `n_subjects` is higher than the length of the TSV file at `tsv_path`.
+    """
+
+    commandline_to_json(
+        {
+            "output_dir": output_dir,
+            "caps_dir": caps_directory,
+            "preprocessing": preprocessing,
+        }
+    )
+
+    # Transform caps_directory in dict
+    caps_dict = CapsDataset.create_caps_dict(caps_directory, multi_cohort=multi_cohort)
+    # Read DataFrame
+    data_df = load_and_check_tsv(tsv_path, caps_dict, output_dir)
+    data_df = extract_baseline(data_df)
+    # Create subjects dir
+    (output_dir / "subjects").mkdir(parents=True, exist_ok=True)
+
+    # Output tsv file
+    columns = ["participant_id", "session_id", "diagnosis"]
+    output_df = pd.DataFrame(columns=columns)
+
+    # Find appropriate preprocessing file type
+    file_type = find_file_type(
+        preprocessing, uncropped_image, tracer, suvr_reference_region
+    )
+
+    def create_motion_image(data_idx, output_df):
+        participant_id = data_df.loc[data_idx, "participant_id"]
+        session_id = data_df.loc[data_idx, "session_id"]
+        cohort = data_df.loc[data_idx, "cohort"]
+        image_path = Path(
+            clinica_file_reader(
+                [participant_id], [session_id], caps_dict[cohort], file_type
+            )[0][0]
+        )
+        input_filename = image_path.name
+        filename_pattern = "_".join(input_filename.split("_")[2::])
+
+        motion_image_nii_dir = (
+            output_dir
+            / "subjects"
+            / f"{participant_id}-RM{data_idx}"
+            / session_id
+            / preprocessing
+        )
+        motion_image_nii_filename = (
+            f"{participant_id}-RM{data_idx}_{session_id}_{filename_pattern}"
+        )
+
+        motion_image_nii_dir.mkdir(parents=True, exist_ok=True)
+
+        motion = tio.RandomMotion(
+            degrees=(rotation[0], rotation[1]),
+            translation=(translation[0], translation[1]),
+            num_transforms=num_transforms,
+        )
+
+        motion_image = motion(tio.ScalarImage(image_path))
+        motion_image.save(motion_image_nii_dir / motion_image_nii_filename)
+
+        # Append row to output tsv
+        row = [f"{participant_id}_RM{data_idx}", session_id, "motion"]
+        row_df = pd.DataFrame([row], columns=columns)
+        output_df = pd.concat([output_df, row_df])
+
+        return output_df
+
+    results_df = Parallel(n_jobs=n_proc)(
+        delayed(create_motion_image)(data_idx, output_df)
+        for data_idx in range(len(data_df))
+    )
+    output_df = pd.DataFrame()
+    for result in results_df:
+        output_df = pd.concat([result, output_df])
+
+    output_df.to_csv(output_dir / "data.tsv", sep="\t", index=False)
+
+    write_missing_mods(output_dir, output_df)
+
+    logger.info(
+        f"Images corrupted with motion artefacts were generated at {output_dir}"
+    )
```

### Comparing `clinicadl-1.3.1/clinicadl/generate/generate_cli.py` & `clinicadl-1.4.0/clinicadl/generate/generate_cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import click
 
 from .generate_hypometabolic_cli import cli as generate_hypo_cli
 from .generate_random_cli import cli as generate_random_cli
 from .generate_shepplogan_cli import cli as generate_shepplogan_cli
 from .generate_trivial_cli import cli as generate_trivial_cli
+from .generate_trivial_motion_cli import cli as generate_trivial_motion_cli
 
 
 class RegistrationOrderGroup(click.Group):
     """CLI group which lists commands by order or registration."""
 
     def list_commands(self, ctx):
         return self.commands.keys()
@@ -19,11 +20,12 @@
     pass
 
 
 cli.add_command(generate_random_cli)
 cli.add_command(generate_trivial_cli)
 cli.add_command(generate_shepplogan_cli)
 cli.add_command(generate_hypo_cli)
+cli.add_command(generate_trivial_motion_cli)
 
 
 if __name__ == "__main__":
     cli()
```

### Comparing `clinicadl-1.3.1/clinicadl/generate/generate_hypometabolic_cli.py` & `clinicadl-1.4.0/clinicadl/generate/generate_hypometabolic_cli.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.1/clinicadl/generate/generate_random_cli.py` & `clinicadl-1.4.0/clinicadl/generate/generate_random_cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 @click.command(name="random", no_args_is_help=True)
 @cli_param.argument.caps_directory
 @cli_param.argument.generated_caps
 @cli_param.option.preprocessing
 @cli_param.option.participant_list
 @cli_param.option.n_subjects
+@cli_param.option.n_proc
 @click.option(
     "--mean",
     type=float,
     default=0,
     help="Mean value of the gaussian noise added to synthetic images.",
 )
 @click.option(
@@ -26,14 +27,15 @@
 @cli_param.option.suvr_reference_region
 def cli(
     caps_directory,
     generated_caps_directory,
     preprocessing,
     participants_tsv,
     n_subjects,
+    n_proc,
     mean,
     sigma,
     use_uncropped_image,
     tracer,
     suvr_reference_region,
 ):
     """Addition of random gaussian noise to brain images.
@@ -46,14 +48,15 @@
 
     generate_random_dataset(
         caps_directory=caps_directory,
         preprocessing=preprocessing,
         tsv_path=participants_tsv,
         output_dir=generated_caps_directory,
         n_subjects=n_subjects,
+        n_proc=n_proc,
         mean=mean,
         sigma=sigma,
         uncropped_image=use_uncropped_image,
         tracer=tracer,
         suvr_reference_region=suvr_reference_region,
     )
```

### Comparing `clinicadl-1.3.1/clinicadl/generate/generate_shepplogan_cli.py` & `clinicadl-1.4.0/clinicadl/generate/generate_shepplogan_cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from clinicadl.utils import cli_param
 
 
 @click.command(name="shepplogan", no_args_is_help=True)
 @cli_param.argument.generated_caps
 @cli_param.option.n_subjects
+@cli_param.option.n_proc
 @cli_param.option.extract_json
 @click.option(
     "--image_size",
     help="Size in pixels of the squared images.",
     type=int,
     default=128,
 )
@@ -33,14 +34,15 @@
     "--smoothing/--no-smoothing",
     default=False,
     help="Adds random smoothing to generated data.",
 )
 def cli(
     generated_caps_directory,
     image_size,
+    n_proc,
     extract_json,
     ad_subtypes_distribution,
     cn_subtypes_distribution,
     n_subjects,
     smoothing,
 ):
     """Random generation of 2D Shepp-Logan phantoms.
@@ -53,14 +55,15 @@
     labels_distribution = {
         "AD": ad_subtypes_distribution,
         "CN": cn_subtypes_distribution,
     }
     generate_shepplogan_dataset(
         output_dir=generated_caps_directory,
         img_size=image_size,
+        n_proc=n_proc,
         labels_distribution=labels_distribution,
         extract_json=extract_json,
         samples=n_subjects,
         smoothing=smoothing,
     )
```

### Comparing `clinicadl-1.3.1/clinicadl/generate/generate_trivial_cli.py` & `clinicadl-1.4.0/clinicadl/generate/generate_trivial_cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 @click.command(name="trivial", no_args_is_help=True)
 @cli_param.argument.caps_directory
 @cli_param.argument.generated_caps
 @cli_param.option.preprocessing
 @cli_param.option.participant_list
 @cli_param.option.n_subjects
+@cli_param.option.n_proc
 @click.option(
     "--mask_path",
     type=click.Path(exists=True, path_type=Path),
     default=None,
     help="Path to the extracted masks to generate the two labels. "
     "Default will try to download masks and store them at '~/.cache/clinicadl'.",
 )
@@ -29,14 +30,15 @@
 @cli_param.option.suvr_reference_region
 def cli(
     caps_directory,
     generated_caps_directory,
     preprocessing,
     participants_tsv,
     n_subjects,
+    n_proc,
     mask_path,
     atrophy_percent,
     use_uncropped_image,
     tracer,
     suvr_reference_region,
 ):
     """Generation of trivial dataset with addition of synthetic brain atrophy.
@@ -49,14 +51,15 @@
 
     generate_trivial_dataset(
         caps_directory=caps_directory,
         tsv_path=participants_tsv,
         preprocessing=preprocessing,
         output_dir=generated_caps_directory,
         n_subjects=n_subjects,
+        n_proc=n_proc,
         mask_path=mask_path,
         atrophy_percent=atrophy_percent,
         uncropped_image=use_uncropped_image,
         tracer=tracer,
         suvr_reference_region=suvr_reference_region,
     )
```

### Comparing `clinicadl-1.3.1/clinicadl/generate/generate_utils.py` & `clinicadl-1.4.0/clinicadl/generate/generate_utils.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.1/clinicadl/interpret/gradients.py` & `clinicadl-1.4.0/clinicadl/interpret/gradients.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.1/clinicadl/interpret/interpret.py` & `clinicadl-1.4.0/clinicadl/interpret/interpret.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.1/clinicadl/interpret/interpret_cli.py` & `clinicadl-1.4.0/clinicadl/interpret/interpret_cli.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.1/clinicadl/mlflow_test.py` & `clinicadl-1.4.0/clinicadl/mlflow_test.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.1/clinicadl/predict/predict.py` & `clinicadl-1.4.0/clinicadl/predict/predict.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,21 +11,23 @@
     data_group: str,
     caps_directory: Path,
     tsv_path: Path,
     use_labels: bool = True,
     label: str = None,
     gpu: bool = True,
     n_proc: int = 0,
-    batch_size: int = 1,
+    batch_size: int = 8,
+    split_list: List[int] = None,
     selection_metrics: List[str] = None,
     diagnoses: List[str] = None,
     multi_cohort: bool = False,
     overwrite: bool = False,
     save_tensor: bool = False,
     save_nifti: bool = False,
+    save_latent_tensor: bool = False,
 ):
     """
     This function loads a MAPS and predicts the global metrics and individual values
     for all the models selected using a metric in selection_metrics.
 
     Args:
         maps_dir: path to the MAPS.
@@ -57,19 +59,21 @@
         raise ClinicaDLArgumentError(
             "Cannot save nifti if the network task is not reconstruction. Please remove --save_nifti option."
         )
     maps_manager.predict(
         data_group,
         caps_directory=caps_directory,
         tsv_path=tsv_path,
+        split_list=split_list,
         selection_metrics=selection_metrics,
         multi_cohort=multi_cohort,
         diagnoses=diagnoses,
         label=label,
         use_labels=use_labels,
         batch_size=batch_size,
         n_proc=n_proc,
         gpu=gpu,
         overwrite=overwrite,
         save_tensor=save_tensor,
         save_nifti=save_nifti,
+        save_latent_tensor=save_latent_tensor,
     )
```

### Comparing `clinicadl-1.3.1/clinicadl/predict/predict_cli.py` & `clinicadl-1.4.0/clinicadl/predict/predict_cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,34 +61,45 @@
     "--save_tensor",
     type=bool,
     default=False,
     is_flag=True,
     help="Save the reconstruction output in the MAPS in Pytorch tensor format.",
 )
 @cli_param.option.save_nifti
+@click.option(
+    "--save_latent_tensor",
+    type=bool,
+    default=False,
+    is_flag=True,
+    help="""Save the latent representation of the image.""",
+)
+@cli_param.option.split
+@cli_param.option.selection_metrics
 @cli_param.option.use_gpu
 @cli_param.option.n_proc
 @cli_param.option.batch_size
 @cli_param.option.overwrite
 def cli(
     input_maps_directory,
     data_group,
     caps_directory,
     participants_tsv,
+    split,
     gpu,
     n_proc,
     batch_size,
     use_labels,
     label,
     selection_metrics,
     diagnoses,
     multi_cohort,
     overwrite,
     save_tensor,
     save_nifti,
+    save_latent_tensor,
 ):
     """Infer the outputs of a trained model on a test set.
 
     INPUT_MAPS_DIRECTORY is the MAPS folder from where the model used for prediction will be loaded.
 
     DATA_GROUP is the name of the subjects and sessions list used for the interpretation.
     """
@@ -105,14 +116,16 @@
         caps_directory=caps_directory,
         tsv_path=participants_tsv,
         use_labels=use_labels,
         label=label,
         gpu=gpu,
         n_proc=n_proc,
         batch_size=batch_size,
+        split_list=split,
         selection_metrics=selection_metrics,
         diagnoses=diagnoses,
         multi_cohort=multi_cohort,
         overwrite=overwrite,
         save_tensor=save_tensor,
         save_nifti=save_nifti,
+        save_latent_tensor=save_latent_tensor,
     )
```

### Comparing `clinicadl-1.3.1/clinicadl/prepare_data/prepare_data.py` & `clinicadl-1.4.0/clinicadl/prepare_data/prepare_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,27 +46,27 @@
     mod_subfolder, file_type = compute_folder_and_file_type(parameters)
     parameters["file_type"] = file_type
 
     # Input file:
     input_files = clinica_file_reader(
         subjects, sessions, caps_directory.as_posix(), file_type
     )[0]
+    logger.debug(f"Selected image file name list: {input_files}.")
 
     def write_output_imgs(output_mode, container, subfolder):
         # Write the extracted tensor on a .pt file
         for filename, tensor in output_mode:
             output_file_dir = (
                 caps_directory
                 / container
                 / "deeplearning_prepare_data"
                 / subfolder
                 / mod_subfolder
             )
-            if not output_file_dir.is_dir():
-                output_file_dir.mkdir(parents=True, exist_ok=True)
+            output_file_dir.mkdir(parents=True, exist_ok=True)
             output_file = output_file_dir / filename
             save_tensor(tensor, output_file)
             logger.debug(f"Output tensor saved at {output_file}")
 
     if parameters["mode"] == "image" or not parameters["prepare_dl"]:
 
         def prepare_image(file):
```

### Comparing `clinicadl-1.3.1/clinicadl/prepare_data/prepare_data_cli.py` & `clinicadl-1.4.0/clinicadl/prepare_data/prepare_data_cli.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.1/clinicadl/prepare_data/prepare_data_utils.py` & `clinicadl-1.4.0/clinicadl/prepare_data/prepare_data_utils.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.1/clinicadl/quality_check/pet_linear/cli.py` & `clinicadl-1.4.0/clinicadl/quality_check/pet_linear/cli.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.1/clinicadl/quality_check/pet_linear/quality_check.py` & `clinicadl-1.4.0/clinicadl/quality_check/pet_linear/quality_check.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.1/clinicadl/quality_check/pet_linear/utils.py` & `clinicadl-1.4.0/clinicadl/quality_check/pet_linear/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
     shape3D = image_np.shape
     img_copy = copy(image_np)
     img_norm_thresh = MinMaxNormalization()(img_copy)
     img_norm_thresh[img_norm_thresh < 0.35] = 0
 
     if not (shape3D == contour_np.shape):
-        print("numpy array hasn't the same size and cannot be compare")
+        raise ValueError(f"The images must be of shape: {shape3D}")
 
     sum_in_contour = 0
 
     for idx, _ in np.ndenumerate(image_np):
         tmp_norm_tresh = img_norm_thresh[idx]
         tmp_contour = int(contour_np[idx])
```

### Comparing `clinicadl-1.3.1/clinicadl/quality_check/qc_cli.py` & `clinicadl-1.4.0/clinicadl/quality_check/qc_cli.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.1/clinicadl/quality_check/t1_linear/cli.py` & `clinicadl-1.4.0/clinicadl/quality_check/t1_linear/cli.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.1/clinicadl/quality_check/t1_linear/models.py` & `clinicadl-1.4.0/clinicadl/quality_check/t1_linear/models.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.1/clinicadl/quality_check/t1_linear/quality_check.py` & `clinicadl-1.4.0/clinicadl/quality_check/t1_linear/quality_check.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,15 +83,14 @@
     if network == "darq":
         FILE1 = RemoteFileStructure(
             filename="resnet_18_darq.pth",
             url=url_aramis,
             checksum="321928e0532f1be7a8dd7f5d805b747c7147ff52594f77ffed0858ab19c5df03",
         )
 
-        # model = resnet18(weights=ResNet18_Weights.IMAGENET1K_V1)
         model = darq_r18()
 
     if network == "sq101":
         FILE1 = RemoteFileStructure(
             filename="sq101_darq.pth",
             url=url_aramis,
             checksum="1f4f3ebd20aaa726d634165a89df12461d9b7c6f2f45931bd29d16cf2616d00f",
```

### Comparing `clinicadl-1.3.1/clinicadl/quality_check/t1_linear/utils.py` & `clinicadl-1.4.0/clinicadl/quality_check/t1_linear/utils.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.1/clinicadl/quality_check/t1_volume/cli.py` & `clinicadl-1.4.0/clinicadl/quality_check/t1_volume/cli.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.1/clinicadl/quality_check/t1_volume/quality_check.py` & `clinicadl-1.4.0/clinicadl/quality_check/t1_volume/quality_check.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.1/clinicadl/quality_check/t1_volume/utils.py` & `clinicadl-1.4.0/clinicadl/quality_check/t1_volume/utils.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.1/clinicadl/random_search/random_search.py` & `clinicadl-1.4.0/clinicadl/random_search/random_search.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.1/clinicadl/random_search/random_search_cli.py` & `clinicadl-1.4.0/clinicadl/random_search/random_search_cli.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.1/clinicadl/random_search/random_search_utils.py` & `clinicadl-1.4.0/clinicadl/random_search/random_search_utils.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.1/clinicadl/resources/config/train_config.toml` & `clinicadl-1.4.0/clinicadl/resources/config/train_config.toml`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 # architecture.n_layers = 4
 # VAE
 latent_space_size = 128
 feature_size = 1024
 n_conv = 4
 io_layer_channels = 8
 recons_weight = 1
-KL_weight = 1
+kl_weight = 1
+normalization = "batch"
 
 [Classification]
 selection_metrics = ["loss"]
 label = "diagnosis"
 label_code = {}
 selection_threshold = 0.0 # Will only be used if num_networks != 1
 loss = "CrossEntropyLoss"
@@ -55,21 +56,24 @@
 [Data]
 multi_cohort = false
 diagnoses = ["AD", "CN"]
 baseline = false
 normalize = true
 data_augmentation = false
 sampler = "random"
+size_reduction=false
+size_reduction_factor=2
 
 [Cross_validation]
 n_splits = 0
 split = []
 
 [Optimization]
 optimizer = "Adam"
 epochs = 20
 learning_rate = 1e-4
 weight_decay = 1e-4
 patience = 0
 tolerance = 0.0
 accumulation_steps = 1
 profiler = false
+
```

### Comparing `clinicadl-1.3.1/clinicadl/train/from_json_cli.py` & `clinicadl-1.4.0/clinicadl/train/from_json_cli.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.1/clinicadl/train/list_models_cli.py` & `clinicadl-1.4.0/clinicadl/train/list_models_cli.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.1/clinicadl/train/resume.py` & `clinicadl-1.4.0/clinicadl/train/resume.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.1/clinicadl/train/resume_cli.py` & `clinicadl-1.4.0/clinicadl/train/resume_cli.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import click
 
-from clinicadl.train import train_option
 from clinicadl.utils import cli_param
+from clinicadl.utils.cli_param import train_option
 
 
 @click.command(name="resume", no_args_is_help=True)
 @cli_param.argument.input_maps
 @train_option.split
 def cli(input_maps_directory, split):
     """Resume training job in specified maps.
```

### Comparing `clinicadl-1.3.1/clinicadl/train/tasks/classification_cli.py` & `clinicadl-1.4.0/clinicadl/train/tasks/classification_cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import click
 
-from .. import train_option
+from clinicadl.utils.cli_param import train_option
+
 from .task_utils import task_launcher
 
 
 @click.command(name="classification", no_args_is_help=True)
 # Mandatory arguments
 @train_option.caps_directory
 @train_option.preprocessing_json
```

### Comparing `clinicadl-1.3.1/clinicadl/train/tasks/reconstruction_cli.py` & `clinicadl-1.4.0/clinicadl/train/tasks/regression_cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import click
 
-from .. import train_option
+from clinicadl.utils.cli_param import train_option
+
 from .task_utils import task_launcher
 
 
-@click.command(name="reconstruction", no_args_is_help=True)
+@click.command(name="regression", no_args_is_help=True)
 # Mandatory arguments
 @train_option.caps_directory
 @train_option.preprocessing_json
 @train_option.tsv_directory
 @train_option.output_maps
 # Options
 @train_option.config_file
@@ -44,28 +45,29 @@
 @train_option.tolerance
 @train_option.accumulation_steps
 @train_option.profiler
 # transfer learning
 @train_option.transfer_path
 @train_option.transfer_selection_metric
 # Task-related
+@train_option.label
 @train_option.selection_metrics
-@train_option.reconstruction_loss
+@train_option.regression_loss
 def cli(**kwargs):
     """
-    Train a deep learning model to learn a reconstruction task on neuroimaging data.
+    Train a deep learning model to learn a regression task on neuroimaging data.
 
     CAPS_DIRECTORY is the CAPS folder from where tensors will be loaded.
 
     PREPROCESSING_JSON is the name of the JSON file in CAPS_DIRECTORY/tensor_extraction folder where
     all information about extraction are stored in order to read the wanted tensors.
 
     TSV_DIRECTORY is a folder were TSV files defining train and validation sets are stored.
 
     OUTPUT_MAPS_DIRECTORY is the path to the MAPS folder where outputs and results will be saved.
 
     Options for this command can be input by declaring argument on the command line or by providing a
     configuration file in TOML format. For more details, please visit the documentation:
     https://clinicadl.readthedocs.io/en/stable/Train/Introduction/#configuration-file
     """
-    task_specific_options = ["selection_metrics", "loss"]
-    task_launcher("reconstruction", task_specific_options, **kwargs)
+    task_specific_options = ["label", "selection_metrics", "loss"]
+    task_launcher("regression", task_specific_options, **kwargs)
```

### Comparing `clinicadl-1.3.1/clinicadl/train/tasks/regression_cli.py` & `clinicadl-1.4.0/clinicadl/train/tasks/reconstruction_cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import click
 
-from .. import train_option
+from clinicadl.utils.cli_param import train_option
+
 from .task_utils import task_launcher
 
 
-@click.command(name="regression", no_args_is_help=True)
+@click.command(name="reconstruction", no_args_is_help=True)
 # Mandatory arguments
 @train_option.caps_directory
 @train_option.preprocessing_json
 @train_option.tsv_directory
 @train_option.output_maps
 # Options
 @train_option.config_file
@@ -44,29 +45,28 @@
 @train_option.tolerance
 @train_option.accumulation_steps
 @train_option.profiler
 # transfer learning
 @train_option.transfer_path
 @train_option.transfer_selection_metric
 # Task-related
-@train_option.label
 @train_option.selection_metrics
-@train_option.regression_loss
+@train_option.reconstruction_loss
 def cli(**kwargs):
     """
-    Train a deep learning model to learn a regression task on neuroimaging data.
+    Train a deep learning model to learn a reconstruction task on neuroimaging data.
 
     CAPS_DIRECTORY is the CAPS folder from where tensors will be loaded.
 
     PREPROCESSING_JSON is the name of the JSON file in CAPS_DIRECTORY/tensor_extraction folder where
     all information about extraction are stored in order to read the wanted tensors.
 
     TSV_DIRECTORY is a folder were TSV files defining train and validation sets are stored.
 
     OUTPUT_MAPS_DIRECTORY is the path to the MAPS folder where outputs and results will be saved.
 
     Options for this command can be input by declaring argument on the command line or by providing a
     configuration file in TOML format. For more details, please visit the documentation:
     https://clinicadl.readthedocs.io/en/stable/Train/Introduction/#configuration-file
     """
-    task_specific_options = ["label", "selection_metrics", "loss"]
-    task_launcher("regression", task_specific_options, **kwargs)
+    task_specific_options = ["selection_metrics", "loss"]
+    task_launcher("reconstruction", task_specific_options, **kwargs)
```

### Comparing `clinicadl-1.3.1/clinicadl/train/tasks/task_utils.py` & `clinicadl-1.4.0/clinicadl/train/tasks/task_utils.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.1/clinicadl/train/train_cli.py` & `clinicadl-1.4.0/clinicadl/train/train_cli.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.1/clinicadl/train/train_option.py` & `clinicadl-1.4.0/clinicadl/utils/cli_param/train_option.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.1/clinicadl/train/train_utils.py` & `clinicadl-1.4.0/clinicadl/train/train_utils.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.1/clinicadl/tsvtools/adapt/adapt.py` & `clinicadl-1.4.0/clinicadl/tsvtools/adapt/adapt.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.1/clinicadl/tsvtools/adapt/adapt_cli.py` & `clinicadl-1.4.0/clinicadl/tsvtools/adapt/adapt_cli.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.1/clinicadl/tsvtools/analysis/analysis.py` & `clinicadl-1.4.0/clinicadl/tsvtools/analysis/analysis.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.1/clinicadl/tsvtools/analysis/analysis_cli.py` & `clinicadl-1.4.0/clinicadl/tsvtools/analysis/analysis_cli.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.1/clinicadl/tsvtools/cli.py` & `clinicadl-1.4.0/clinicadl/tsvtools/cli.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.1/clinicadl/tsvtools/get_labels/get_labels.py` & `clinicadl-1.4.0/clinicadl/tsvtools/get_labels/get_labels.py`

 * *Files 0% similar despite different names*

```diff
@@ -313,35 +313,40 @@
         compute_missing_mods(bids_directory, missing_mods_directory, "missing_mods")
 
     logger.info(
         f"output of clinica iotools check-missing-modalities: {missing_mods_directory}"
     )
 
     # Generating the output of `clinica iotools merge-tsv `
-    if merged_tsv is None:
+    if not merged_tsv:
         merged_tsv = output_dir / "merged.tsv"
-    elif not merged_tsv.is_file():
-        from clinica.iotools.utils.data_handling import create_merge_file
+        if merged_tsv.is_file():
+            logger.warning(
+                f"A merged_tsv file already exists at {merged_tsv}. It will be used to run the command."
+            )
+        else:
+            from clinica.iotools.utils.data_handling import create_merge_file
 
-        logger.info("create merge tsv")
-        check_bids_folder(bids_directory)
-        create_merge_file(
-            bids_directory,
-            merged_tsv,
-            caps_dir=caps_directory,
-            pipelines=None,
-            ignore_scan_files=None,
-            ignore_sessions_files=None,
-            volume_atlas_selection=None,
-            freesurfer_atlas_selection=None,
-            pvc_restriction=None,
-            tsv_file=None,
-            group_selection=False,
-            tracers_selection=False,
-        )
+            logger.info("Running Clinica merge TSV pipeline.")
+
+            check_bids_folder(bids_directory)
+            create_merge_file(
+                bids_directory,
+                merged_tsv,
+                caps_dir=caps_directory,
+                pipelines=None,
+                ignore_scan_files=None,
+                ignore_sessions_files=None,
+                volume_atlas_selection=None,
+                freesurfer_atlas_selection=None,
+                pvc_restriction=None,
+                tsv_file=None,
+                group_selection=False,
+                tracers_selection=False,
+            )
 
     logger.info(f"output of clinica iotools merge-tsv: {merged_tsv}")
 
     # Reading files
     if not merged_tsv.is_file():
         raise ClinicaDLTSVError(f"{merged_tsv} file was not found. ")
     bids_df = pd.read_csv(merged_tsv, sep="\t")
```

### Comparing `clinicadl-1.3.1/clinicadl/tsvtools/get_labels/get_labels_cli.py` & `clinicadl-1.4.0/clinicadl/tsvtools/get_labels/get_labels_cli.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.1/clinicadl/tsvtools/get_labels/old_get_labels_cli.py` & `clinicadl-1.4.0/clinicadl/tsvtools/get_labels/old_get_labels_cli.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.1/clinicadl/tsvtools/get_metadata/get_metadata.py` & `clinicadl-1.4.0/clinicadl/tsvtools/get_metadata/get_metadata.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.1/clinicadl/tsvtools/get_metadata/get_metadata_cli.py` & `clinicadl-1.4.0/clinicadl/tsvtools/get_metadata/get_metadata_cli.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.1/clinicadl/tsvtools/get_progression/get_progression.py` & `clinicadl-1.4.0/clinicadl/tsvtools/get_progression/get_progression.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.1/clinicadl/tsvtools/get_progression/get_progression_cli.py` & `clinicadl-1.4.0/clinicadl/tsvtools/get_progression/get_progression_cli.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.1/clinicadl/tsvtools/getlabels/getlabels.py` & `clinicadl-1.4.0/clinicadl/tsvtools/getlabels/getlabels.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.1/clinicadl/tsvtools/kfold/kfold.py` & `clinicadl-1.4.0/clinicadl/tsvtools/kfold/kfold.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.1/clinicadl/tsvtools/kfold/kfold_cli.py` & `clinicadl-1.4.0/clinicadl/tsvtools/kfold/kfold_cli.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.1/clinicadl/tsvtools/prepare_experiment/prepare_experiment_cli.py` & `clinicadl-1.4.0/clinicadl/tsvtools/prepare_experiment/prepare_experiment_cli.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.1/clinicadl/tsvtools/split/split.py` & `clinicadl-1.4.0/clinicadl/tsvtools/split/split.py`

 * *Files 6% similar despite different names*

```diff
@@ -50,14 +50,43 @@
         if p > p_min_max:
             p_min_max = p
             best_train_df, best_test_df = train_df, test_df
 
     return (best_train_df, best_test_df, p_min_max)
 
 
+def KStests(train_df, test_df, threshold=0.5):
+    pmin = 1
+    column = ""
+    for col in train_df.columns:
+        if col == "session_id":
+            continue
+        _, pval = ks_2samp(train_df[col], test_df[col])
+        if pval < pmin:
+            pmin = pval
+            column = col
+    return (pmin, column)
+
+
+def shuffle_choice(df, n_shuffle=10):
+    p_min_max, n_col_min = 0, df.columns.size
+
+    for i in range(n_shuffle):
+        train_df = df.sample(frac=0.75)
+        test_df = df.drop(train_df.index)
+
+        p, col = KStests(train_df, test_df)
+
+        if p > p_min_max:
+            p_min_max = p
+            best_train_df, best_test_df = train_df, test_df
+
+    return (best_train_df, best_test_df, p_min_max)
+
+
 def create_split(
     diagnosis_df,
     split_label,
     n_test,
     p_age_threshold=0.80,
     p_sex_threshold=0.80,
     supplementary_train_df=None,
```

### Comparing `clinicadl-1.3.1/clinicadl/tsvtools/split/split_cli.py` & `clinicadl-1.4.0/clinicadl/tsvtools/split/split_cli.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.1/clinicadl/utils/caps_dataset/data.py` & `clinicadl-1.4.0/clinicadl/utils/caps_dataset/data.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from logging import getLogger
 from pathlib import Path
 from typing import Any, Callable, Dict, List, Optional, Tuple, Union
 
 import numpy as np
 import pandas as pd
 import torch
+import torchio as tio
 import torchvision.transforms as transforms
 from clinica.utils.exceptions import ClinicaCAPSError
 from torch.utils.data import Dataset
 
 from clinicadl.prepare_data.prepare_data_utils import (
     PATTERN_DICT,
     TEMPLATE_DICT,
@@ -130,15 +131,15 @@
                     caps_dict[cohort] = caps_path
         else:
             check_caps_folder(caps_directory)
             caps_dict = {"single": caps_directory}
 
         return caps_dict
 
-    def _get_image_path(self, participant: str, session: str, cohort: str) -> str:
+    def _get_image_path(self, participant: str, session: str, cohort: str) -> Path:
         """
         Gets the path to the tensor image (*.pt)
 
         Args:
             participant: ID of the participant.
             session: ID of the session.
             cohort: Name of the cohort.
@@ -149,16 +150,18 @@
 
         # Try to find .nii.gz file
         try:
             file_type = self.preprocessing_dict["file_type"]
             results = clinica_file_reader(
                 [participant], [session], self.caps_dict[cohort], file_type
             )
+            logger.debug(f"clinica_file_reader output: {results}")
             filepath = Path(results[0][0])
             image_filename = filepath.name.replace(".nii.gz", ".pt")
+
             folder, _ = compute_folder_and_file_type(self.preprocessing_dict)
             image_dir = (
                 self.caps_dict[cohort]
                 / "subjects"
                 / participant
                 / session
                 / "deeplearning_prepare_data"
@@ -170,15 +173,15 @@
         except ClinicaCAPSError:
             file_type = self.preprocessing_dict["file_type"]
             file_type["pattern"] = file_type["pattern"].replace(".nii.gz", ".pt")
             results = clinica_file_reader(
                 [participant], [session], self.caps_dict[cohort], file_type
             )
             filepath = results[0]
-            image_path = filepath[0]
+            image_path = Path(filepath[0])
 
         return image_path
 
     def _get_meta_data(self, idx: int) -> Tuple[str, str, str, int, int]:
         """
         Gets all meta data necessary to compute the path with _get_image_path
 
@@ -880,14 +883,105 @@
         np.nan_to_num(image, copy=False)
         smoothed_image = gaussian_filter(image, sigma=self.sigma)
         sample["image"] = smoothed_image
 
         return sample
 
 
+class RandomMotion(object):
+    """Applies a Random Motion"""
+
+    def __init__(self, translation, rotation, num_transforms):
+        self.rotation = rotation
+        self.translation = translation
+        self.num_transforms = num_transforms
+
+    def __call__(self, image):
+        motion = tio.RandomMotion(
+            degrees=self.rotation,
+            translation=self.translation,
+            num_transforms=self.num_transforms,
+        )
+        image = motion(image)
+
+        return image
+
+
+class RandomGhosting(object):
+    """Applies a Random Ghosting"""
+
+    def __init__(self, num_ghosts):
+        self.num_ghosts = num_ghosts
+
+    def __call__(self, image):
+        ghost = tio.RandomGhosting(num_ghosts=self.num_ghosts)
+        image = ghost(image)
+
+        return image
+
+
+class RandomSpike(object):
+    """Applies a Random Spike"""
+
+    def __init__(self, num_spikes, intensity):
+        self.num_spikes = num_spikes
+        self.intensity = intensity
+
+    def __call__(self, image):
+        spike = tio.RandomSpike(
+            num_spikes=self.num_spikes,
+            intensity=self.intensity,
+        )
+        image = spike(image)
+
+        return image
+
+
+class RandomBiasField(object):
+    """Applies a Random Bias Field"""
+
+    def __init__(self, coefficients):
+        self.coefficients = coefficients
+
+    def __call__(self, image):
+        bias_field = tio.RandomBiasField(coefficients=self.coefficients)
+        image = bias_field(image)
+
+        return image
+
+
+class RandomBlur(object):
+    """Applies a Random Blur"""
+
+    def __init__(self, std):
+        self.std = std
+
+    def __call__(self, image):
+        blur = tio.RandomBlur(std=self.std)
+        image = blur(image)
+
+        return image
+
+
+class RandomSwap(object):
+    """Applies a Random Swap"""
+
+    def __init__(self, patch_size, num_iterations):
+        self.patch_size = patch_size
+        self.num_iterations = num_iterations
+
+    def __call__(self, image):
+        swap = tio.RandomSwap(
+            patch_size=self.patch_size, num_iterations=self.num_iterations
+        )
+        image = swap(image)
+
+        return image
+
+
 class ToTensor(object):
     """Convert image type to Tensor and diagnosis to diagnosis code"""
 
     def __call__(self, image):
         np.nan_to_num(image, copy=False)
         image = image.astype(float)
 
@@ -913,16 +1007,40 @@
                 )
                 self.nan_detected = True
             return torch.nan_to_num(image)
         else:
             return image
 
 
+class SizeReduction(object):
+    """Reshape the input tensor to be of size [80, 96, 80]"""
+
+    def __init__(self, size_reduction_factor=2) -> None:
+        self.size_reduction_factor = size_reduction_factor
+
+    def __call__(self, image):
+        if self.size_reduction_factor == 2:
+            return image[:, 4:164:2, 8:200:2, 8:168:2]
+        elif self.size_reduction_factor == 3:
+            return image[:, 0:168:3, 8:200:3, 4:172:3]
+        elif self.size_reduction_factor == 4:
+            return image[:, 4:164:4, 8:200:4, 8:168:4]
+        elif self.size_reduction_factor == 5:
+            return image[:, 4:164:5, 0:200:5, 8:168:5]
+        else:
+            raise ClinicaDLConfigurationError(
+                "size_reduction_factor must be 2, 3, 4 or 5."
+            )
+
+
 def get_transforms(
-    normalize: bool = True, data_augmentation: List[str] = None
+    normalize: bool = True,
+    data_augmentation: List[str] = None,
+    size_reduction: bool = False,
+    size_reduction_factor: int = 2,
 ) -> Tuple[transforms.Compose, transforms.Compose]:
     """
     Outputs the transformations that will be applied to the dataset
 
     Args:
         normalize: if True will perform MinMaxNormalization.
         data_augmentation: list of data augmentation performed on the training set.
@@ -931,27 +1049,36 @@
         transforms to apply in train and evaluation mode / transforms to apply in evaluation mode only.
     """
     augmentation_dict = {
         "Noise": RandomNoising(sigma=0.1),
         "Erasing": transforms.RandomErasing(),
         "CropPad": RandomCropPad(10),
         "Smoothing": RandomSmoothing(),
+        "Motion": RandomMotion((2, 4), (2, 4), 2),
+        "Ghosting": RandomGhosting((4, 10)),
+        "Spike": RandomSpike(1, (1, 3)),
+        "BiasField": RandomBiasField(0.5),
+        "RandomBlur": RandomBlur((0, 2)),
+        "RandomSwap": RandomSwap(15, 100),
         "None": None,
     }
+
+    augmentation_list = []
+    transformations_list = []
+
     if data_augmentation:
-        augmentation_list = [
-            augmentation_dict[augmentation] for augmentation in data_augmentation
-        ]
-    else:
-        augmentation_list = []
+        augmentation_list.extend(
+            [augmentation_dict[augmentation] for augmentation in data_augmentation]
+        )
 
+    transformations_list.append(NanRemoval())
     if normalize:
-        transformations_list = [NanRemoval(), MinMaxNormalization()]
-    else:
-        transformations_list = [NanRemoval()]
+        transformations_list.append(MinMaxNormalization())
+    if size_reduction:
+        transformations_list.append(SizeReduction(size_reduction_factor))
 
     all_transformations = transforms.Compose(transformations_list)
     train_transformations = transforms.Compose(augmentation_list)
 
     return train_transformations, all_transformations
 
 
@@ -1051,15 +1178,15 @@
                 )
             else:
                 test_path = test_path.parent / "labels.tsv"
         else:
             test_path = test_path.parent / "train.tsv"
 
     test_df = pd.read_csv(test_path, sep="\t")
-
+    test_df = test_df[test_df.diagnosis.isin(diagnoses_list)]
     test_df.reset_index(inplace=True, drop=True)
 
     return test_df
 
 
 def check_multi_cohort_tsv(tsv_df, purpose):
     """
```

### Comparing `clinicadl-1.3.1/clinicadl/utils/cli_param/argument.py` & `clinicadl-1.4.0/clinicadl/utils/cli_param/argument.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.1/clinicadl/utils/cli_param/option.py` & `clinicadl-1.4.0/clinicadl/utils/cli_param/option.py`

 * *Files 6% similar despite different names*

```diff
@@ -89,15 +89,15 @@
     default=2,
     show_default=True,
     help="Number of cores used during the task.",
 )
 batch_size = click.option(
     "--batch_size",
     type=int,
-    default=2,
+    default=8,
     show_default=True,
     help="Batch size for data loading.",
 )
 
 # Extract
 save_features = click.option(
     "--save_features",
@@ -157,26 +157,40 @@
     help=(
         "Suffix of output files if MODALITY is `custom`. "
         "Suffix to append to filenames, for instance "
         "`graymatter_space-Ixi549Space_modulated-off_probability.nii.gz`, or "
         "`segm-whitematter_probability.nii.gz`"
     ),
 )
+
+# PREDICT & INTERPRET
 # Data group
 overwrite = click.option(
     "--overwrite",
     "-o",
     default=False,
     is_flag=True,
-    help="Will overwrite data group if existing. Please give caps_directory and partcipants_tsv to"
+    help="Will overwrite data group if existing. Please give caps_directory and participants_tsv to"
     " define new data group.",
 )
-
 # Predict and interpret
 
 save_nifti = click.option(
     "--save_nifti",
     type=bool,
     default=False,
     is_flag=True,
     help="Save the output map(s) in the MAPS in NIfTI format.",
 )
+split = click.option(
+    "--split",
+    "-s",
+    type=int,
+    multiple=True,
+    help="Make inference on the list of given splits. By default, inference is done on all the splits.",
+)
+selection_metrics = click.option(
+    "--selection_metrics",
+    "-sm",
+    multiple=True,
+    help="""Make inference on the list of given metrics used for selection. By default, inference is done on all the metrics.""",
+)
```

### Comparing `clinicadl-1.3.1/clinicadl/utils/cli_param/option_group.py` & `clinicadl-1.4.0/clinicadl/utils/cli_param/option_group.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.1/clinicadl/utils/descriptors.py` & `clinicadl-1.4.0/clinicadl/utils/descriptors.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.1/clinicadl/utils/early_stopping.py` & `clinicadl-1.4.0/clinicadl/utils/early_stopping.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.1/clinicadl/utils/exceptions.py` & `clinicadl-1.4.0/clinicadl/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.1/clinicadl/utils/logger.py` & `clinicadl-1.4.0/clinicadl/utils/logger.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,9 +64,8 @@
             "%(asctime)s - %(name)s - %(levelname)s: %(message)s", "%Y-%m-%d %H:%M:%S"
         )
         debug_file_name = "clinicadl_debug.log"
         file_handler = logging.FileHandler(debug_file_name)
         file_handler.setLevel(logging.DEBUG)
         file_handler.setFormatter(debug_file_formatter)
         logger.addHandler(file_handler)
-        print(Path.cwd())
         logger.warning(f"Debug log will be saved at {Path.cwd() / debug_file_name}")
```

### Comparing `clinicadl-1.3.1/clinicadl/utils/maps_manager/iotools.py` & `clinicadl-1.4.0/clinicadl/utils/maps_manager/iotools.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.1/clinicadl/utils/maps_manager/logwriter.py` & `clinicadl-1.4.0/clinicadl/utils/maps_manager/logwriter.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.1/clinicadl/utils/maps_manager/maps_manager.py` & `clinicadl-1.4.0/clinicadl/utils/maps_manager/maps_manager.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import json
 import shutil
 import subprocess
 from datetime import datetime
-from glob import glob
 from logging import getLogger
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 import pandas as pd
 import torch
 from torch.utils.data import DataLoader
@@ -80,15 +79,14 @@
             self.split_name = (
                 self._check_split_wording()
             )  # Used only for retro-compatibility
 
         # Initiate MAPS
         else:
             self._check_args(parameters)
-            print(parameters)
             parameters["tsv_path"] = Path(parameters["tsv_path"])
 
             if (maps_path.is_dir() and maps_path.is_file()) or (  # Non-folder file
                 maps_path.is_dir() and list(maps_path.iterdir())  # Non empty folder
             ):
                 raise MAPSError(
                     f"You are trying to create a new MAPS at {maps_path} but "
@@ -193,14 +191,15 @@
         n_proc: int = None,
         gpu: bool = None,
         overwrite: bool = False,
         label: str = None,
         label_code: Optional[Dict[str, int]] = "default",
         save_tensor: bool = False,
         save_nifti: bool = False,
+        save_latent_tensor: bool = False,
     ):
         """
         Performs the prediction task on a subset of caps_directory defined in a TSV file.
 
         Args:
             data_group: name of the data group tested.
             caps_directory: path to the CAPS folder. For more information please refer to
@@ -218,21 +217,23 @@
             batch_size: If given, sets the value of batch_size, else use the same as in training step.
             n_proc: If given, sets the value of num_workers, else use the same as in training step.
             gpu: If given, a new value for the device of the model will be computed.
             overwrite: If True erase the occurrences of data_group.
             label: Target label used for training (if network_task in [`regression`, `classification`]).
             label_code: dictionary linking the target values to a node number.
         """
-        if split_list is None:
+        if not split_list:
             split_list = self._find_splits()
         logger.debug(f"List of splits {split_list}")
 
         _, all_transforms = get_transforms(
             normalize=self.normalize,
             data_augmentation=self.data_augmentation,
+            size_reduction=self.size_reduction,
+            size_reduction_factor=self.size_reduction_factor,
         )
 
         group_df = None
         if tsv_path is not None:
             group_df = load_data_test(
                 tsv_path,
                 diagnoses if len(diagnoses) != 0 else self.diagnoses,
@@ -251,15 +252,15 @@
             logger.info(f"Prediction of split {split}")
             group_df, group_parameters = self.get_group_info(data_group, split)
             # Find label code if not given
             if label is not None and label != self.label and label_code == "default":
                 self.task_manager.generate_label_code(group_df, label)
 
             # Erase previous TSV files
-            if selection_metrics is None:
+            if not selection_metrics:
                 split_selection_metrics = self._find_selection_metrics(split)
             else:
                 split_selection_metrics = selection_metrics
             for selection in split_selection_metrics:
                 tsv_dir = (
                     self.maps_path
                     / f"{self.split_name}-{split}"
@@ -302,14 +303,15 @@
                         split,
                         split_selection_metrics,
                         use_labels=use_labels,
                         gpu=gpu,
                         network=network,
                     )
                     if save_tensor:
+                        logger.debug("Saving tensors")
                         self._compute_output_tensors(
                             data_test,
                             data_group,
                             split,
                             selection_metrics,
                             gpu=gpu,
                             network=network,
@@ -319,14 +321,23 @@
                             data_test,
                             data_group,
                             split,
                             selection_metrics,
                             gpu=gpu,
                             network=network,
                         )
+                    if save_latent_tensor:
+                        self._compute_latent_tensors(
+                            data_test,
+                            data_group,
+                            split,
+                            selection_metrics,
+                            gpu=gpu,
+                            network=network,
+                        )
             else:
                 data_test = return_dataset(
                     group_parameters["caps_directory"],
                     group_df,
                     self.preprocessing_dict,
                     all_transformations=all_transforms,
                     multi_cohort=group_parameters["multi_cohort"],
@@ -351,14 +362,15 @@
                     data_group,
                     split,
                     split_selection_metrics,
                     use_labels=use_labels,
                     gpu=gpu,
                 )
                 if save_tensor:
+                    logger.debug("Saving tensors")
                     self._compute_output_tensors(
                         data_test,
                         data_group,
                         split,
                         selection_metrics,
                         gpu=gpu,
                     )
@@ -366,14 +378,23 @@
                     self._compute_output_nifti(
                         data_test,
                         data_group,
                         split,
                         selection_metrics,
                         gpu=gpu,
                     )
+                if save_latent_tensor:
+                    self._compute_latent_tensors(
+                        data_test,
+                        data_group,
+                        split,
+                        selection_metrics,
+                        gpu=gpu,
+                    )
+
             self._ensemble_prediction(data_group, split, selection_metrics, use_labels)
 
     def interpret(
         self,
         data_group,
         name,
         method,
@@ -448,26 +469,28 @@
 
         if method not in method_dict.keys():
             raise NotImplementedError(
                 f"Interpretation method {method} is not implemented. "
                 f"Please choose in {method_dict.keys()}"
             )
 
-        if split_list is None:
+        if not split_list:
             split_list = self._find_splits()
         logger.debug(f"List of splits {split_list}")
 
         if self.multi_network:
             raise NotImplementedError(
                 "The interpretation of multi-network framework is not implemented."
             )
 
         _, all_transforms = get_transforms(
             normalize=self.normalize,
             data_augmentation=self.data_augmentation,
+            size_reduction=self.size_reduction,
+            size_reduction_factor=self.size_reduction_factor,
         )
 
         group_df = None
         if tsv_path is not None:
             group_df = load_data_test(
                 tsv_path,
                 diagnoses if len(diagnoses) != 0 else self.diagnoses,
@@ -494,15 +517,15 @@
             test_loader = DataLoader(
                 data_test,
                 batch_size=batch_size if batch_size is not None else self.batch_size,
                 shuffle=False,
                 num_workers=n_proc if n_proc is not None else self.n_proc,
             )
 
-            if selection_metrics is None:
+            if not selection_metrics:
                 selection_metrics = self._find_selection_metrics(split)
 
             for selection_metric in selection_metrics:
                 logger.info(f"Interpretation of metric {selection_metric}")
                 results_path = (
                     self.maps_path
                     / f"{self.split_name}-{split}"
@@ -587,14 +610,16 @@
             resume (bool): If True the job is resumed from checkpoint.
         """
         from torch.utils.data import DataLoader
 
         train_transforms, all_transforms = get_transforms(
             normalize=self.normalize,
             data_augmentation=self.data_augmentation,
+            size_reduction=self.size_reduction,
+            size_reduction_factor=self.size_reduction_factor,
         )
         split_manager = self._init_split_manager(split_list)
         for split in split_manager.split_iterator():
             logger.info(f"Training split {split}")
             seed_everything(self.seed, self.deterministic, self.compensation)
 
             split_df_dict = split_manager[split]
@@ -670,14 +695,16 @@
             resume: If True the job is resumed from checkpoint.
         """
         from torch.utils.data import DataLoader
 
         train_transforms, all_transforms = get_transforms(
             normalize=self.normalize,
             data_augmentation=self.data_augmentation,
+            size_reduction=self.size_reduction,
+            size_reduction_factor=self.size_reduction_factor,
         )
 
         split_manager = self._init_split_manager(split_list)
         for split in split_manager.split_iterator():
             logger.info(f"Training split {split}")
             seed_everything(self.seed, self.deterministic, self.compensation)
 
@@ -788,15 +815,15 @@
         model, beginning_epoch = self._init_model(
             split=split,
             resume=resume,
             transfer_path=self.transfer_path,
             transfer_selection=self.transfer_selection_metric,
         )
         criterion = self.task_manager.get_criterion(self.loss)
-        logger.debug(f"Criterion for {self.network_task} is {criterion}")
+        logger.info(f"Criterion for {self.network_task} is {criterion}")
         optimizer = self._init_optimizer(model, split=split, resume=resume)
         logger.debug(f"Optimizer used for training is optimizer")
 
         model.train()
         train_loader.dataset.train()
 
         early_stopping = EarlyStopping(
@@ -1156,25 +1183,86 @@
                     f"{participant_id}_{session_id}_{self.mode}-{mode_id}_input.pt"
                 )
                 output_filename = (
                     f"{participant_id}_{session_id}_{self.mode}-{mode_id}_output.pt"
                 )
                 torch.save(image, tensor_path / input_filename)
                 torch.save(output, tensor_path / output_filename)
+                logger.debug(f"File saved at {[input_filename, output_filename]}")
+
+    def _compute_latent_tensors(
+        self,
+        dataset,
+        data_group,
+        split,
+        selection_metrics,
+        nb_images=None,
+        gpu=None,
+        network=None,
+    ):
+        """
+        Compute the output tensors and saves them in the MAPS.
+
+        Args:
+            dataset (clinicadl.utils.caps_dataset.data.CapsDataset): wrapper of the data set.
+            data_group (str): name of the data group used for the task.
+            split (int): split number.
+            selection_metrics (list[str]): metrics used for model selection.
+            nb_images (int): number of full images to write. Default computes the outputs of the whole data set.
+            gpu (bool): If given, a new value for the device of the model will be computed.
+            network (int): Index of the network tested (only used in multi-network setting).
+        """
+        for selection_metric in selection_metrics:
+            # load the best trained model during the training
+            model, _ = self._init_model(
+                transfer_path=self.maps_path,
+                split=split,
+                transfer_selection=selection_metric,
+                gpu=gpu,
+                network=network,
+            )
+
+            tensor_path = (
+                self.maps_path
+                / f"{self.split_name}-{split}"
+                / f"best-{selection_metric}"
+                / data_group
+                / "latent_tensors"
+            )
+            tensor_path.mkdir(parents=True, exist_ok=True)
+
+            if nb_images is None:  # Compute outputs for the whole data set
+                nb_modes = len(dataset)
+            else:
+                nb_modes = nb_images * dataset.elem_per_image
+
+            for i in range(nb_modes):
+                data = dataset[i]
+                image = data["image"]
+                logger.debug(f"Image for latent representation {image}")
+                _, latent, _ = model.forward(image.unsqueeze(0).to(model.device))
+                latent = latent.squeeze(0).cpu()
+                participant_id = data["participant_id"]
+                session_id = data["session_id"]
+                mode_id = data[f"{self.mode}_id"]
+                output_filename = (
+                    f"{participant_id}_{session_id}_{self.mode}-{mode_id}_latent.pt"
+                )
+                torch.save(latent, tensor_path / output_filename)
 
     def _ensemble_prediction(
         self,
         data_group,
         split,
         selection_metrics,
         use_labels=True,
     ):
         """Computes the results on the image-level."""
 
-        if selection_metrics is None:
+        if not selection_metrics:
             selection_metrics = self._find_selection_metrics(split)
 
         for selection_metric in selection_metrics:
             # Soft voting
             if self.num_networks > 1:
                 self._ensemble_to_tsv(
                     split,
@@ -1212,15 +1300,19 @@
                     f"No value was given for {arg}."
                 )
         self.parameters = add_default_values(parameters)
         self.parameters = change_str_to_path(parameters)
         if self.parameters["gpu"]:
             check_gpu()
 
-        _, transformations = get_transforms(self.normalize)
+        _, transformations = get_transforms(
+            normalize=self.normalize,
+            size_reduction=self.size_reduction,
+            size_reduction_factor=self.size_reduction_factor,
+        )
 
         split_manager = self._init_split_manager(None)
         train_df = split_manager[0]["train"]
         if "label" not in self.parameters:
             self.parameters["label"] = None
 
         self.task_manager = self._init_task_manager(df=train_df)
@@ -1307,15 +1399,15 @@
             for metric in list(split_path.iterdir())
             if metric.name[:5:] == "best-"
         ]
 
     def _check_selection_metric(self, split, selection_metric=None):
         """Check that a given selection metric is available for a given split."""
         available_metrics = self._find_selection_metrics(split)
-        if selection_metric is None:
+        if not selection_metric:
             if len(available_metrics) > 1:
                 raise ClinicaDLArgumentError(
                     f"Several metrics are available for split {split}. "
                     f"Please choose which one you want to read among {available_metrics}"
                 )
             else:
                 selection_metric = available_metrics[0]
@@ -1429,16 +1521,14 @@
         from pathlib import PosixPath
 
         """Write JSON files of parameters."""
         logger.debug("Writing parameters...")
         json_path.mkdir(parents=True, exist_ok=True)
 
         parameters = change_path_to_str(parameters)
-        print("just before error")
-        print(parameters)
         # save to json file
         json_data = json.dumps(parameters, skipkeys=True, indent=4)
         json_path = json_path / "maps.json"
         if verbose:
             logger.info(f"Path of json file: {json_path}")
         with json_path.open(mode="w") as f:
             f.write(json_data)
```

### Comparing `clinicadl-1.3.1/clinicadl/utils/maps_manager/maps_manager_utils.py` & `clinicadl-1.4.0/clinicadl/utils/maps_manager/maps_manager_utils.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.1/clinicadl/utils/meta_maps/getter.py` & `clinicadl-1.4.0/clinicadl/utils/meta_maps/getter.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.1/clinicadl/utils/metric_module.py` & `clinicadl-1.4.0/clinicadl/utils/metric_module.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     "sensitivity": "max",
     "specificity": "max",
     "PPV": "max",
     "NPV": "max",
     "BA": "max",
     "PSNR": "max",
     "SSIM": "max",
+    "LNCC": "max",
     "loss": "min",
 }
 
 logger = getLogger("clinicadl.metric")
 
 
 class MetricModule:
@@ -222,31 +223,63 @@
         """
         Args:
             y (List): list of labels
             y_pred (List): list of predictions
         Returns:
             (float) SSIM
         """
-        from skimage.metrics import structural_similarity
+        from clinicadl.utils.pytorch_ssim import ssim, ssim3D
 
-        return structural_similarity(y, y_pred)
+        if len(y) == 3:
+            return ssim(y, y_pred)
+        else:
+            return ssim3D(y, y_pred)
 
     @staticmethod
     def psnr_fn(y, y_pred):
         """
         Args:
             y (List): list of labels
             y_pred (List): list of predictions
         Returns:
             (float) PSNR
         """
         from skimage.metrics import peak_signal_noise_ratio
 
         return peak_signal_noise_ratio(y, y_pred)
 
+    @staticmethod
+    def lncc_fn(y, y_pred):
+        """
+        Args:
+            y (List): list of labels
+            y_pred (List): list of predictions
+        Returns:
+            (float) LNCC
+        """
+        from scipy.ndimage import gaussian_filter
+
+        sigma = 2
+
+        mean1 = gaussian_filter(y, sigma)
+        mean2 = gaussian_filter(y_pred, sigma)
+
+        mean12 = gaussian_filter(
+            y * y_pred, sigma
+        )  # the * operator is term by term product
+        mean11 = gaussian_filter(y * y, sigma)
+        mean22 = gaussian_filter(y_pred * y_pred, sigma)
+
+        covar12 = mean12 - (mean1 * mean2)
+        var1 = np.sqrt(mean11 - (mean1 * mean1))
+        var2 = np.sqrt(mean22 - (mean2 * mean2))
+
+        lcc_matrix = np.maximum(covar12 / (var1 * var2), 0)
+        return np.mean(lcc_matrix)
+
 
 class RetainBest:
     """
     A class to retain the best and overfitting values for a set of wanted metrics.
     """
 
     def __init__(self, selection_metrics: List[str], n_classes: int = 0):
```

### Comparing `clinicadl-1.3.1/clinicadl/utils/network/autoencoder/cnn_transformer.py` & `clinicadl-1.4.0/clinicadl/utils/network/autoencoder/cnn_transformer.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.1/clinicadl/utils/network/cnn/SECNN.py` & `clinicadl-1.4.0/clinicadl/utils/network/cnn/SECNN.py`

 * *Files 3% similar despite different names*

```diff
@@ -104,15 +104,14 @@
         out = self.layer0(input_tensor)
         out = self.layer1(out)
         out = self.layer2(out)
         out = self.layer3(out)
         out = self.layer4(out)
 
         d, h, w = self._maxpool_output_size(input_size[1::], nb_layers=5)
-        print(d, h, w)
         self.fc = nn.Sequential(
             Flatten(),
             nn.Dropout(p=0.5),
             nn.Linear(128 * d * h * w, 256),  # t1 image
             nn.ReLU(),
             nn.Linear(256, 2),
         )
```

### Comparing `clinicadl-1.3.1/clinicadl/utils/network/cnn/models.py` & `clinicadl-1.4.0/clinicadl/utils/network/cnn/models.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.1/clinicadl/utils/network/cnn/random.py` & `clinicadl-1.4.0/clinicadl/utils/network/cnn/random.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.1/clinicadl/utils/network/cnn/resnet.py` & `clinicadl-1.4.0/clinicadl/utils/network/cnn/resnet.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.1/clinicadl/utils/network/cnn/resnet3D.py` & `clinicadl-1.4.0/clinicadl/utils/network/cnn/resnet3D.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,14 @@
         out = self.layer0(input_tensor)
         out = self.layer1(out)
         out = self.layer2(out)
         out = self.layer3(out)
         out = self.layer4(out)
 
         d, h, w = self._maxpool_output_size(input_size[1::], nb_layers=5)
-        print(d, h, w)
         self.fc = nn.Sequential(
             Flatten(),
             nn.Linear(128 * d * h * w, 256),  # t1 image
             nn.ELU(),
             nn.Dropout(p=0.8),
             nn.Linear(256, 2),
         )
```

### Comparing `clinicadl-1.3.1/clinicadl/utils/network/network.py` & `clinicadl-1.4.0/clinicadl/utils/network/network.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.1/clinicadl/utils/network/network_utils.py` & `clinicadl-1.4.0/clinicadl/utils/network/network_utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -120,7 +120,39 @@
         output = self.unpool(f_maps, indices)
         if padding is not None:
             x1 = padding[2]
             y1 = padding[0]
             output = output[:, :, x1::, y1::]
 
         return output
+
+
+def torch_summarize(model, show_weights=True, show_parameters=True):
+    """Summarizes torch model by showing trainable parameters and weights."""
+    import numpy as np
+    import torch
+    from torch.nn.modules.module import _addindent
+
+    tmpstr = model.__class__.__name__ + " (\n"
+    for key, module in model._modules.items():
+        # if it contains layers let call it recursively to get params and weights
+        if type(module) in [
+            torch.nn.modules.container.Container,
+            torch.nn.modules.container.Sequential,
+        ]:
+            modstr = torch_summarize(module)
+        else:
+            modstr = module.__repr__()
+        modstr = _addindent(modstr, 2)
+
+        params = sum([np.prod(p.size()) for p in module.parameters()])
+        weights = tuple([tuple(p.size()) for p in module.parameters()])
+
+        tmpstr += "  (" + key + "): " + modstr
+        if show_weights:
+            tmpstr += ", weights={}".format(weights)
+        if show_parameters:
+            tmpstr += ", parameters={}".format(params)
+        tmpstr += "\n"
+
+    tmpstr = tmpstr + ")"
+    return tmpstr
```

### Comparing `clinicadl-1.3.1/clinicadl/utils/network/sub_network.py` & `clinicadl-1.4.0/clinicadl/utils/network/sub_network.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.1/clinicadl/utils/network/vae/vae_utils.py` & `clinicadl-1.4.0/clinicadl/utils/network/vae/vae_layers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-import torch
 import torch.nn.functional as F
 from torch import nn
 
+from clinicadl.utils.network.vae.vae_utils import get_norm2d, get_norm3d
+
 
 class EncoderLayer2D(nn.Module):
     """
     Class defining the encoder's part of the Autoencoder.
     This layer is composed of one 2D convolutional layer,
     a batch normalization layer with a leaky relu
     activation function.
@@ -14,26 +15,29 @@
     def __init__(
         self,
         input_channels,
         output_channels,
         kernel_size=4,
         stride=2,
         padding=1,
+        output_padding=0,
+        normalization="batch",
     ):
         super(EncoderLayer2D, self).__init__()
         self.layer = nn.Sequential(
             nn.Conv2d(
                 input_channels,
                 output_channels,
                 kernel_size,
                 stride=stride,
                 padding=padding,
+                output_padding=output_padding,
                 bias=False,
             ),
-            nn.BatchNorm2d(output_channels),
+            get_norm2d(normalization, output_channels),
         )
 
     def forward(self, x):
         x = F.leaky_relu(self.layer(x), negative_slope=0.2, inplace=True)
         return x
 
 
@@ -41,27 +45,35 @@
     """
     Class defining the decoder's part of the Autoencoder.
     This layer is composed of one 2D transposed convolutional layer,
     a batch normalization layer with a relu activation function.
     """
 
     def __init__(
-        self, input_channels, output_channels, kernel_size=4, stride=2, padding=1
+        self,
+        input_channels,
+        output_channels,
+        kernel_size=4,
+        stride=2,
+        padding=1,
+        output_padding=0,
+        normalization="batch",
     ):
         super(DecoderLayer2D, self).__init__()
         self.layer = nn.Sequential(
             nn.ConvTranspose2d(
                 input_channels,
                 output_channels,
                 kernel_size,
                 stride=stride,
                 padding=padding,
+                output_padding=output_padding,
                 bias=False,
             ),
-            nn.BatchNorm2d(output_channels),
+            get_norm2d(normalization, output_channels),
         )
 
     def forward(self, x):
         x = F.relu(self.layer(x), inplace=True)
         return x
 
 
@@ -70,27 +82,33 @@
     Class defining the encoder's part of the Autoencoder.
     This layer is composed of one 3D convolutional layer,
     a batch normalization layer with a leaky relu
     activation function.
     """
 
     def __init__(
-        self, input_channels, output_channels, kernel_size=4, stride=2, padding=1
+        self,
+        input_channels,
+        output_channels,
+        kernel_size=4,
+        stride=2,
+        padding=1,
+        normalization="batch",
     ):
         super(EncoderLayer3D, self).__init__()
         self.layer = nn.Sequential(
             nn.Conv3d(
                 input_channels,
                 output_channels,
                 kernel_size,
                 stride=stride,
                 padding=padding,
                 bias=False,
             ),
-            nn.BatchNorm3d(output_channels),
+            get_norm3d(normalization, output_channels),
         )
 
     def forward(self, x):
         x = F.leaky_relu(self.layer(x), negative_slope=0.2, inplace=True)
         return x
 
 
@@ -105,27 +123,28 @@
         self,
         input_channels,
         output_channels,
         kernel_size=4,
         stride=2,
         padding=1,
         output_padding=0,
+        normalization="batch",
     ):
         super(DecoderLayer3D, self).__init__()
         self.layer = nn.Sequential(
             nn.ConvTranspose3d(
                 input_channels,
                 output_channels,
                 kernel_size,
                 stride=stride,
                 padding=padding,
                 output_padding=output_padding,
                 bias=False,
             ),
-            nn.BatchNorm3d(output_channels),
+            get_norm3d(normalization, output_channels),
         )
 
     def forward(self, x):
         x = F.relu(self.layer(x), inplace=True)
         return x
 
 
@@ -206,14 +225,15 @@
                 padding_h = 1
             if tensor_w % 2 != 0:
                 padding_w = 1
             decoder_padding.append([padding_h, padding_w])
             tensor_h, tensor_w = tensor_h // 2, tensor_w // 2
 
         self.decoder_padding = decoder_padding
+        print(self.decoder_padding)
 
         # Final Layer
         if latent_dim == 1:
             n_pix = (
                 first_layer_channels
                 * 2 ** (n_conv - 1)
                 * (self.input_h // (2**n_conv))
@@ -323,14 +343,15 @@
             )
 
         for i in range(n_conv - 1, 0, -1):
             self.layers.append(
                 DecoderLayer2D(
                     last_layer_channels * 2 ** (i),
                     last_layer_channels * 2 ** (i - 1),
+                    output_padding=output_padding[i],
                 )
             )
 
         self.layers.append(
             nn.Sequential(
                 nn.ConvTranspose2d(
                     last_layer_channels,
```

### Comparing `clinicadl-1.3.1/clinicadl/utils/network/vae/vanilla_vae.py` & `clinicadl-1.4.0/clinicadl/utils/network/vae/vanilla_vae.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import torch
 from torch import nn
 
 from clinicadl.utils.network.vae.base_vae import BaseVAE
-from clinicadl.utils.network.vae.vae_utils import (
+from clinicadl.utils.network.vae.vae_layers import (
     DecoderLayer3D,
     EncoderLayer3D,
     Flatten,
     Unflatten3D,
     VAE_Decoder,
     VAE_Encoder,
 )
@@ -19,18 +19,18 @@
     reference: Diederik P Kingma et al., Auto-Encoding Variational Bayes.
     https://arxiv.org/abs/1312.6114
     """
 
     def __init__(
         self,
         input_size,
-        latent_space_size=128,
-        feature_size=1024,
-        recons_weight=1,
-        KL_weight=1,
+        latent_space_size,
+        feature_size,
+        recons_weight,
+        kl_weight,
         gpu=True,
     ):
         n_conv = 4
         io_layer_channel = 32
 
         encoder = VAE_Encoder(
             input_size=input_size,
@@ -55,15 +55,15 @@
             encoder,
             decoder,
             mu_layer,
             var_layer,
             latent_space_size,
             gpu=gpu,
             recons_weight=recons_weight,
-            KL_weight=KL_weight,
+            kl_weight=kl_weight,
             is_3D=False,
         )
 
     @staticmethod
     def get_input_size():
         return "1@128x128"
 
@@ -83,18 +83,18 @@
     reference: Diederik P Kingma et al., Auto-Encoding Variational Bayes.
     https://arxiv.org/abs/1312.6114
     """
 
     def __init__(
         self,
         input_size,
-        latent_space_size=128,
-        feature_size=1024,
-        recons_weight=1,
-        KL_weight=1,
+        latent_space_size,
+        feature_size,
+        recons_weight,
+        kl_weight,
         gpu=True,
     ):
         feature_channels = 64
         latent_channels = 1
         n_conv = 4
         io_layer_channel = 32
 
@@ -125,15 +125,15 @@
             encoder,
             decoder,
             mu_layer,
             var_layer,
             latent_space_size,
             gpu=gpu,
             recons_weight=recons_weight,
-            KL_weight=KL_weight,
+            kl_weight=kl_weight,
             is_3D=False,
         )
 
     @staticmethod
     def get_input_size():
         return "1@128x128"
 
@@ -142,29 +142,29 @@
         return "2D"
 
     @staticmethod
     def get_task():
         return ["reconstruction"]
 
 
-class Vanilla3DVAE(BaseVAE):
+class Vanilla3DspacialVAE(BaseVAE):
     """
     This network is a 3D convolutional variational autoencoder with a spacial latent space.
 
     reference: Diederik P Kingma et al., Auto-Encoding Variational Bayes.
     https://arxiv.org/abs/1312.6114
     """
 
     def __init__(
         self,
         input_size,
-        latent_space_size=256,
-        feature_size=1024,
-        recons_weight=1,
-        KL_weight=1,
+        latent_space_size,
+        feature_size,
+        recons_weight,
+        kl_weight,
         gpu=True,
     ):
         n_conv = 4
         first_layer_channels = 32
         last_layer_channels = 32
         feature_channels = 512
         latent_channels = 1
@@ -238,15 +238,15 @@
             )
         )
         for i in range(n_conv - 1, 0, -1):
             decoder_layers.append(
                 DecoderLayer3D(
                     last_layer_channels * 2 ** (i),
                     last_layer_channels * 2 ** (i - 1),
-                    output_padding=decoder_output_padding[-i],
+                    output_padding=decoder_output_padding[i],
                 )
             )
         decoder_layers.append(
             nn.Sequential(
                 nn.ConvTranspose3d(
                     last_layer_channels,
                     input_c,
@@ -257,23 +257,23 @@
                     bias=False,
                 ),
                 nn.Sigmoid(),
             )
         )
         decoder = nn.Sequential(*decoder_layers)
 
-        super(Vanilla3DVAE, self).__init__(
+        super(Vanilla3DspacialVAE, self).__init__(
             encoder,
             decoder,
             mu_layer,
             var_layer,
             latent_space_size,
             gpu=gpu,
             recons_weight=recons_weight,
-            KL_weight=KL_weight,
+            kl_weight=kl_weight,
             is_3D=False,
         )
 
     @staticmethod
     def get_input_size():
         return "1@128x128x128"
 
@@ -292,36 +292,41 @@
 
     reference: Diederik P Kingma et al., Auto-Encoding Variational Bayes.
     https://arxiv.org/abs/1312.6114
     """
 
     def __init__(
         self,
-        input_size,
+        size_reduction_factor,
         latent_space_size=256,
         feature_size=1024,
         n_conv=4,
         io_layer_channels=8,
         recons_weight=1,
-        KL_weight=1,
+        kl_weight=1,
         gpu=True,
     ):
         first_layer_channels = io_layer_channels
         last_layer_channels = io_layer_channels
         # automatically compute padding
-        decoder_output_padding = [
-            # [1, 0, 0],
-            # [0, 0, 0],
-            # [0, 0, 1],
-        ]
+        decoder_output_padding = []
 
-        input_c = input_size[0]
-        input_d = input_size[1]
-        input_h = input_size[2]
-        input_w = input_size[3]
+        if size_reduction_factor == 2:
+            self.input_size = [1, 80, 96, 80]
+        elif size_reduction_factor == 3:
+            self.input_size = [1, 56, 64, 56]
+        elif size_reduction_factor == 4:
+            self.input_size = [1, 40, 48, 40]
+        elif size_reduction_factor == 5:
+            self.input_size = [1, 32, 40, 32]
+
+        input_c = self.input_size[0]
+        input_d = self.input_size[1]
+        input_h = self.input_size[2]
+        input_w = self.input_size[3]
         d, h, w = input_d, input_h, input_w
 
         # ENCODER
         encoder_layers = []
         # Input Layer
         encoder_layers.append(EncoderLayer3D(input_c, first_layer_channels))
         decoder_output_padding.append([d % 2, h % 2, w % 2])
@@ -332,14 +337,15 @@
                 EncoderLayer3D(
                     first_layer_channels * 2**i, first_layer_channels * 2 ** (i + 1)
                 )
             )
             # Construct output paddings
             decoder_output_padding.append([d % 2, h % 2, w % 2])
             d, h, w = d // 2, h // 2, w // 2
+        # Compute size of the feature space
         n_pix = (
             first_layer_channels
             * 2 ** (n_conv - 1)
             * (input_d // (2**n_conv))
             * (input_h // (2**n_conv))
             * (input_w // (2**n_conv))
         )
@@ -418,21 +424,9 @@
             decoder,
             mu_layer,
             var_layer,
             latent_space_size,
             gpu=gpu,
             is_3D=False,
             recons_weight=recons_weight,
-            KL_weight=KL_weight,
+            kl_weight=kl_weight,
         )
-
-    @staticmethod
-    def get_input_size():
-        return "1@128x128x128"
-
-    @staticmethod
-    def get_dimension():
-        return "3D"
-
-    @staticmethod
-    def get_task():
-        return ["reconstruction"]
```

### Comparing `clinicadl-1.3.1/clinicadl/utils/preprocessing.py` & `clinicadl-1.4.0/clinicadl/utils/preprocessing.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.1/clinicadl/utils/seed.py` & `clinicadl-1.4.0/clinicadl/utils/seed.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.1/clinicadl/utils/split_manager/kfold.py` & `clinicadl-1.4.0/clinicadl/utils/split_manager/kfold.py`

 * *Files 12% similar despite different names*

```diff
@@ -34,11 +34,12 @@
 
     def split_iterator(self):
         if not self.split_list:
             return range(self.n_splits)
         else:
             return self.split_list
 
-    def _get_tsv_paths(self, cohort_path: Path, split):
-        train_path = cohort_path / f"split-{split}"
-        valid_path = cohort_path / f"split-{split}"
+    def _get_tsv_paths(self, cohort_path: Path, *args):
+        for split in args:
+            train_path = cohort_path / f"split-{split}"
+            valid_path = cohort_path / f"split-{split}"
         return train_path, valid_path
```

### Comparing `clinicadl-1.3.1/clinicadl/utils/split_manager/single_split.py` & `clinicadl-1.4.0/clinicadl/utils/split_manager/single_split.py`

 * *Files 20% similar despite different names*

```diff
@@ -26,12 +26,12 @@
     @property
     def allowed_splits_list(self):
         return [0]
 
     def split_iterator(self):
         return range(1)
 
-    def _get_tsv_paths(self, cohort_path: Path):
+    def _get_tsv_paths(self, cohort_path: Path, *args):
         train_path = cohort_path
         valid_path = cohort_path
 
         return train_path, valid_path
```

### Comparing `clinicadl-1.3.1/clinicadl/utils/split_manager/split_manager.py` & `clinicadl-1.4.0/clinicadl/utils/split_manager/split_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,18 +121,18 @@
             "validation": valid_df,
         }
 
     def concatenate_diagnoses(
         self, split, cohort_path: Path = None, cohort_diagnoses=None
     ):
         """Concatenated the diagnoses needed to form the train and validation sets."""
-
+        tmp_cohort_path = cohort_path if cohort_path is not None else self.tsv_path
         train_path, valid_path = self._get_tsv_paths(
-            split=split,
-            cohort_path=cohort_path if cohort_path is not None else self.tsv_path,
+            tmp_cohort_path,
+            split,
         )
         logger.debug(f"Training data loaded at {train_path}")
         logger.debug(f"Validation data loaded at {valid_path}")
         if cohort_diagnoses is None:
             cohort_diagnoses = self.diagnoses
 
         if self.baseline:
@@ -192,21 +192,24 @@
                     labels_df,
                     how="inner",
                     on=["participant_id", "session_id"],
                 )
             except:
                 pass
 
+        train_df = train_df[train_df.diagnosis.isin(cohort_diagnoses)]
+        valid_df = valid_df[valid_df.diagnosis.isin(cohort_diagnoses)]
+
         train_df.reset_index(inplace=True, drop=True)
         valid_df.reset_index(inplace=True, drop=True)
 
         return train_df, valid_df
 
     @abc.abstractmethod
-    def _get_tsv_paths(self, cohort_path, split):
+    def _get_tsv_paths(self, cohort_path, *args):
         """
         Computes the paths to the TSV files needed depending on the split structure.
 
         Args:
             cohort_path (str): path to the split structure of a cohort.
             split (int): Index of the split.
         Returns:
```

### Comparing `clinicadl-1.3.1/clinicadl/utils/task_manager/classification.py` & `clinicadl-1.4.0/clinicadl/utils/task_manager/classification.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.1/clinicadl/utils/task_manager/reconstruction.py` & `clinicadl-1.4.0/clinicadl/utils/task_manager/reconstruction.py`

 * *Files 17% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         columns = ["participant_id", "session_id", f"{self.mode}_id"]
         for metric in self.evaluation_metrics:
             columns.append(metric)
         return columns
 
     @property
     def evaluation_metrics(self):
-        return ["MSE", "MAE", "PSNR"]
+        return ["MSE", "MAE", "PSNR", "SSIM"]
 
     @property
     def save_outputs(self):
         return True
 
     def generate_test_row(self, idx, data, outputs):
         y = data["image"][idx]
@@ -98,19 +98,34 @@
         compatible_losses = [
             "L1Loss",
             "MSELoss",
             "KLDivLoss",
             "BCEWithLogitsLoss",
             "HuberLoss",
             "SmoothL1Loss",
+            "VAEGaussianLoss",
+            "VAEBernoulliLoss",
+            "VAEContinuousBernoulliLoss",
         ]
         if criterion is None:
             return nn.MSELoss()
         if criterion not in compatible_losses:
             raise ClinicaDLArgumentError(
                 f"Reconstruction loss must be chosen in {compatible_losses}."
             )
+        if criterion == "VAEGaussianLoss":
+            from clinicadl.utils.network.vae.vae_utils import VAEGaussianLoss
+
+            return VAEGaussianLoss
+        elif criterion == "VAEBernoulliLoss":
+            from clinicadl.utils.network.vae.vae_utils import VAEBernoulliLoss
+
+            return VAEBernoulliLoss
+        elif criterion == "VAEContinuousBernoulliLoss":
+            from clinicadl.utils.network.vae.vae_utils import VAEContinuousBernoulliLoss
+
+            return VAEContinuousBernoulliLoss
         return getattr(nn, criterion)()
 
     @staticmethod
     def get_default_network():
         return "AE_Conv5_FC3"
```

### Comparing `clinicadl-1.3.1/clinicadl/utils/task_manager/regression.py` & `clinicadl-1.4.0/clinicadl/utils/task_manager/regression.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.1/clinicadl/utils/task_manager/task_manager.py` & `clinicadl-1.4.0/clinicadl/utils/task_manager/task_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -185,32 +185,44 @@
         Returns:
             the results and metrics on the image level.
         """
         model.eval()
         dataloader.dataset.eval()
 
         results_df = pd.DataFrame(columns=self.columns)
-        total_loss = 0
+        total_loss = {}
         with torch.no_grad():
             for i, data in enumerate(dataloader):
-                outputs, loss_dict = model.compute_outputs_and_loss(
-                    data, criterion, use_labels=use_labels
-                )
-                total_loss += loss_dict["loss"].item()
+                # initialize the loss list to save the loss components
+                if i == 0:
+                    outputs, loss_dict = model.compute_outputs_and_loss(
+                        data, criterion, use_labels=use_labels
+                    )
+                    for loss_component in loss_dict.keys():
+                        total_loss[loss_component] = 0
+                    for loss_component in total_loss.keys():
+                        total_loss[loss_component] += loss_dict[loss_component].item()
+                else:
+                    outputs, loss_dict = model.compute_outputs_and_loss(
+                        data, criterion, use_labels=use_labels
+                    )
+                    for loss_component in total_loss.keys():
+                        total_loss[loss_component] += loss_dict[loss_component].item()
 
                 # Generate detailed DataFrame
                 for idx in range(len(data["participant_id"])):
                     row = self.generate_test_row(idx, data, outputs)
                     row_df = pd.DataFrame(row, columns=self.columns)
                     results_df = pd.concat([results_df, row_df])
 
                 del outputs, loss_dict
             results_df.reset_index(inplace=True, drop=True)
 
         if not use_labels:
             metrics_dict = None
         else:
             metrics_dict = self.compute_metrics(results_df)
-            metrics_dict["loss"] = total_loss
+            for loss_component in total_loss.keys():
+                metrics_dict[loss_component] = total_loss[loss_component]
         torch.cuda.empty_cache()
 
         return results_df, metrics_dict
```

### Comparing `clinicadl-1.3.1/clinicadl/utils/tsvtools_utils.py` & `clinicadl-1.4.0/clinicadl/utils/tsvtools_utils.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.1/pyproject.toml` & `clinicadl-1.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "clinicadl"
-version = "1.3.1"
+version = "1.4.0"
 description = "Framework for the reproducible processing of neuroimaging data with deep learning methods"
 license = "MIT"
 authors = ["ARAMIS Lab"]
 maintainers = ["Clinica developers <clinica-user@inria.fr>"]
 readme = "README.md"
 homepage = "https://clinicadl.readthedocs.io"
 repository = "https://github.com/aramis-lab/clinicadl.git"
@@ -37,14 +37,15 @@
 numpy = "^1.17"
 scikit-learn = "^1.0"
 scikit-image = "^0.19"
 joblib = "^1.2.0"
 click = "^8"
 click-option-group = "^0.5"
 pynvml = "*"
+torchio = "^0.18.90"
 
 [tool.poetry.group.dev.dependencies]
 black = "*"
 isort = "*"
 pre-commit = "*"
 pytest = "*"
 pytest-timeout = "*"
```

### Comparing `clinicadl-1.3.1/PKG-INFO` & `clinicadl-1.4.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clinicadl
-Version: 1.3.1
+Version: 1.4.0
 Summary: Framework for the reproducible processing of neuroimaging data with deep learning methods
 Home-page: https://clinicadl.readthedocs.io
 License: MIT
 Keywords: bids,image processing,deep learning,neuroimaging,neuroscience
 Author: ARAMIS Lab
 Maintainer: Clinica developers
 Maintainer-email: clinica-user@inria.fr
@@ -29,14 +29,15 @@
 Requires-Dist: pandas (>=1.2,<2.0)
 Requires-Dist: pynvml
 Requires-Dist: scikit-image (>=0.19,<0.20)
 Requires-Dist: scikit-learn (>=1.0,<2.0)
 Requires-Dist: tensorboard
 Requires-Dist: toml
 Requires-Dist: torch (>=1.8.0,<2.0.0)
+Requires-Dist: torchio (>=0.18.90,<0.19.0)
 Requires-Dist: torchvision
 Project-URL: Documentation, https://clinicadl.readthedocs.io
 Project-URL: Repository, https://github.com/aramis-lab/clinicadl.git
 Description-Content-Type: text/markdown
 
 <h1 align="center">
   <a href="http://www.clinicadl.readthedocs.io">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: clinicadl Version: 1.3.1 Summary: Framework for the
+Metadata-Version: 2.1 Name: clinicadl Version: 1.4.0 Summary: Framework for the
 reproducible processing of neuroimaging data with deep learning methods Home-
 page: https://clinicadl.readthedocs.io License: MIT Keywords: bids,image
 processing,deep learning,neuroimaging,neuroscience Author: ARAMIS Lab
 Maintainer: Clinica developers Maintainer-email: clinica-user@inria.fr
 Requires-Python: >=3.8,<3.11 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop Classifier: License :: OSI
@@ -13,17 +13,17 @@
 Scientific/Engineering :: Image Processing Classifier: Topic :: Scientific/
 Engineering :: Medical Science Apps. Requires-Dist: click (>=8,<9) Requires-
 Dist: click-option-group (>=0.5,<0.6) Requires-Dist: clinica (>=0.7.4,<0.8.0)
 Requires-Dist: joblib (>=1.2.0,<2.0.0) Requires-Dist: numpy (>=1.17,<2.0)
 Requires-Dist: pandas (>=1.2,<2.0) Requires-Dist: pynvml Requires-Dist: scikit-
 image (>=0.19,<0.20) Requires-Dist: scikit-learn (>=1.0,<2.0) Requires-Dist:
 tensorboard Requires-Dist: toml Requires-Dist: torch (>=1.8.0,<2.0.0) Requires-
-Dist: torchvision Project-URL: Documentation, https://clinicadl.readthedocs.io
-Project-URL: Repository, https://github.com/aramis-lab/clinicadl.git
-Description-Content-Type: text/markdown
+Dist: torchio (>=0.18.90,<0.19.0) Requires-Dist: torchvision Project-URL:
+Documentation, https://clinicadl.readthedocs.io Project-URL: Repository, https:
+//github.com/aramis-lab/clinicadl.git Description-Content-Type: text/markdown
                            ****** [ClinicaDL_Logo]
                                ClinicaDL ******
    Framework for the reproducible processing of neuroimaging data with deep
                                learning methods
        [Build_Status] [PyPI_version] [Documentation_Status] [Downloads]
                        Documentation | Tutorial | Forum
 ## About the project This repository hosts ClinicaDL, the deep learning
```

