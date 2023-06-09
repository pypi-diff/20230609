# Comparing `tmp/tenyks-cli-0.2.45.tar.gz` & `tmp/tenyks-cli-0.2.46.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tenyks-cli-0.2.45.tar", last modified: Wed Jun  7 10:10:16 2023, max compression
+gzip compressed data, was "tenyks-cli-0.2.46.tar", last modified: Fri Jun  9 10:24:16 2023, max compression
```

## Comparing `tenyks-cli-0.2.45.tar` & `tenyks-cli-0.2.46.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxrwxr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-06-07 10:10:16.125957 tenyks-cli-0.2.45/
--rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)      584 2023-06-06 14:49:32.000000 tenyks-cli-0.2.45/Internal README.md
--rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)       47 2023-06-06 14:49:32.000000 tenyks-cli-0.2.45/MANIFEST.in
--rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)      670 2023-06-07 10:10:16.125957 tenyks-cli-0.2.45/PKG-INFO
--rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)      290 2023-06-06 14:49:32.000000 tenyks-cli-0.2.45/README.md
--rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)       86 2023-06-06 14:49:32.000000 tenyks-cli-0.2.45/pyproject.toml
--rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)       88 2023-06-06 14:49:32.000000 tenyks-cli-0.2.45/requirements.txt
--rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)      138 2023-06-07 10:10:16.125957 tenyks-cli-0.2.45/setup.cfg
--rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)      812 2023-06-07 10:09:09.000000 tenyks-cli-0.2.45/setup.py
-drwxrwxr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-06-07 10:10:16.109957 tenyks-cli-0.2.45/tenyks/
--rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-06-06 14:49:32.000000 tenyks-cli-0.2.45/tenyks/__init__.py
--rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)       75 2023-06-06 14:49:32.000000 tenyks-cli-0.2.45/tenyks/__main__.py
-drwxrwxr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-06-07 10:10:16.109957 tenyks-cli-0.2.45/tenyks/adapters/
--rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-06-06 14:49:32.000000 tenyks-cli-0.2.45/tenyks/adapters/__init__.py
-drwxrwxr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-06-07 10:10:16.109957 tenyks-cli-0.2.45/tenyks/adapters/categories/
--rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-06-06 14:49:32.000000 tenyks-cli-0.2.45/tenyks/adapters/categories/__init__.py
--rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)      746 2023-06-06 14:49:32.000000 tenyks-cli-0.2.45/tenyks/adapters/categories/category_reader_factory.py
-drwxrwxr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-06-07 10:10:16.109957 tenyks-cli-0.2.45/tenyks/adapters/categories/readers/
--rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-06-06 14:49:32.000000 tenyks-cli-0.2.45/tenyks/adapters/categories/readers/__init__.py
--rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)      255 2023-06-06 14:49:32.000000 tenyks-cli-0.2.45/tenyks/adapters/categories/readers/category_reader.py
--rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)      321 2023-06-06 14:49:32.000000 tenyks-cli-0.2.45/tenyks/adapters/categories/readers/json_category_reader.py
--rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)      440 2023-06-06 14:49:32.000000 tenyks-cli-0.2.45/tenyks/adapters/categories/readers/txt_category_reader.py
--rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)      349 2023-06-06 14:49:32.000000 tenyks-cli-0.2.45/tenyks/adapters/config.py
-drwxrwxr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-06-07 10:10:16.113957 tenyks-cli-0.2.45/tenyks/adapters/detection/
--rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-06-06 14:49:32.000000 tenyks-cli-0.2.45/tenyks/adapters/detection/__init__.py
--rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)     2530 2023-06-06 14:49:32.000000 tenyks-cli-0.2.45/tenyks/adapters/detection/detection_adapter.py
--rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)     1883 2023-06-06 14:49:32.000000 tenyks-cli-0.2.45/tenyks/adapters/detection/detection_adapter_factory.py
--rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)      416 2023-06-06 14:49:32.000000 tenyks-cli-0.2.45/tenyks/adapters/detection/detection_data.py
-drwxrwxr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-06-07 10:10:16.113957 tenyks-cli-0.2.45/tenyks/adapters/detection/readers/
--rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-06-06 14:49:32.000000 tenyks-cli-0.2.45/tenyks/adapters/detection/readers/__init__.py
--rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)     2617 2023-06-06 14:49:32.000000 tenyks-cli-0.2.45/tenyks/adapters/detection/readers/classification_reader.py
--rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)     3114 2023-06-06 14:49:32.000000 tenyks-cli-0.2.45/tenyks/adapters/detection/readers/deepstream_reader.py
--rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)      477 2023-06-06 14:49:32.000000 tenyks-cli-0.2.45/tenyks/adapters/detection/readers/detection_reader.py
--rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)     2586 2023-06-06 14:49:32.000000 tenyks-cli-0.2.45/tenyks/adapters/detection/readers/vott_csv_reader.py
--rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)     3291 2023-06-06 14:49:32.000000 tenyks-cli-0.2.45/tenyks/adapters/detection/readers/yolo_reader.py
-drwxrwxr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-06-07 10:10:16.113957 tenyks-cli-0.2.45/tenyks/adapters/detection/writers/
--rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-06-06 14:49:32.000000 tenyks-cli-0.2.45/tenyks/adapters/detection/writers/__init__.py
--rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)     1599 2023-06-06 14:49:32.000000 tenyks-cli-0.2.45/tenyks/adapters/detection/writers/coco_writer.py
--rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)      414 2023-06-06 14:49:32.000000 tenyks-cli-0.2.45/tenyks/adapters/detection/writers/detection_writer.py
-drwxrwxr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-06-07 10:10:16.113957 tenyks-cli-0.2.45/tenyks/adapters/utilities/
--rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-06-06 14:49:32.000000 tenyks-cli-0.2.45/tenyks/adapters/utilities/__init__.py
--rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)     1274 2023-06-06 14:49:32.000000 tenyks-cli-0.2.45/tenyks/adapters/utilities/bbox.py
--rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)      388 2023-06-06 14:49:32.000000 tenyks-cli-0.2.45/tenyks/adapters/utilities/file.py
--rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)     4490 2023-06-06 14:49:32.000000 tenyks-cli-0.2.45/tenyks/api.py
--rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)     1600 2023-06-06 14:49:32.000000 tenyks-cli-0.2.45/tenyks/cli.py
--rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)      995 2023-06-06 14:49:32.000000 tenyks-cli-0.2.45/tenyks/click_utilities.py
-drwxrwxr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-06-07 10:10:16.117957 tenyks-cli-0.2.45/tenyks/config/
--rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-06-06 14:49:32.000000 tenyks-cli-0.2.45/tenyks/config/__init__.py
--rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)     1719 2023-06-06 14:49:32.000000 tenyks-cli-0.2.45/tenyks/config/config.py
--rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)     1499 2023-06-06 14:49:32.000000 tenyks-cli-0.2.45/tenyks/config/configure.py
-drwxrwxr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-06-07 10:10:16.117957 tenyks-cli-0.2.45/tenyks/config/providers/
--rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-06-06 14:49:32.000000 tenyks-cli-0.2.45/tenyks/config/providers/__init__.py
-drwxrwxr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-06-07 10:10:16.117957 tenyks-cli-0.2.45/tenyks/config/providers/aws/
--rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-06-06 14:49:32.000000 tenyks-cli-0.2.45/tenyks/config/providers/aws/__init__.py
--rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)      841 2023-06-06 14:49:32.000000 tenyks-cli-0.2.45/tenyks/config/providers/aws/config_aws.py
--rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)     1007 2023-06-06 14:49:32.000000 tenyks-cli-0.2.45/tenyks/config/providers/aws/configure_aws.py
-drwxrwxr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-06-07 10:10:16.117957 tenyks-cli-0.2.45/tenyks/convert/
--rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-06-06 14:49:32.000000 tenyks-cli-0.2.45/tenyks/convert/__init__.py
--rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)     2096 2023-06-06 14:49:32.000000 tenyks-cli-0.2.45/tenyks/convert/convert_detections_file.py
--rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)     1616 2023-06-06 14:49:32.000000 tenyks-cli-0.2.45/tenyks/convert/detection_file_processor.py
-drwxrwxr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-06-07 10:10:16.117957 tenyks-cli-0.2.45/tenyks/dataset/
--rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-06-06 14:49:32.000000 tenyks-cli-0.2.45/tenyks/dataset/__init__.py
-drwxrwxr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-06-07 10:10:16.121957 tenyks-cli-0.2.45/tenyks/dataset/aws/
--rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-06-06 14:49:32.000000 tenyks-cli-0.2.45/tenyks/dataset/aws/__init__.py
--rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)      545 2023-06-06 14:49:32.000000 tenyks-cli-0.2.45/tenyks/dataset/aws/dataclasses.py
--rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)      107 2023-06-06 14:49:32.000000 tenyks-cli-0.2.45/tenyks/dataset/config.py
--rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)     4200 2023-06-06 14:49:32.000000 tenyks-cli-0.2.45/tenyks/dataset/create_dataset.py
--rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)     1939 2023-06-06 14:49:32.000000 tenyks-cli-0.2.45/tenyks/dataset/upload_annotations.py
--rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)     1040 2023-06-06 14:49:32.000000 tenyks-cli-0.2.45/tenyks/dataset/upload_class_names.py
--rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)      975 2023-06-06 14:49:32.000000 tenyks-cli-0.2.45/tenyks/dataset/upload_images.py
--rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)     1104 2023-06-06 14:49:32.000000 tenyks-cli-0.2.45/tenyks/dataset/utilities.py
-drwxrwxr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-06-07 10:10:16.121957 tenyks-cli-0.2.45/tenyks/embeddings/
--rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-06-06 14:49:32.000000 tenyks-cli-0.2.45/tenyks/embeddings/__init__.py
--rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)     1306 2023-06-06 14:49:32.000000 tenyks-cli-0.2.45/tenyks/embeddings/upload_annotation_bbox_embeddings.py
--rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)     1254 2023-06-06 14:49:32.000000 tenyks-cli-0.2.45/tenyks/embeddings/upload_image_embeddings.py
--rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)     1471 2023-06-06 14:49:32.000000 tenyks-cli-0.2.45/tenyks/embeddings/upload_prediction_bbox_embeddings.py
--rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)      346 2023-06-06 14:49:32.000000 tenyks-cli-0.2.45/tenyks/exceptions_handler.py
-drwxrwxr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-06-07 10:10:16.121957 tenyks-cli-0.2.45/tenyks/model/
--rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-06-06 14:49:32.000000 tenyks-cli-0.2.45/tenyks/model/__init__.py
--rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)     2730 2023-06-06 14:49:32.000000 tenyks-cli-0.2.45/tenyks/model/create_model.py
--rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)     2119 2023-06-06 14:49:32.000000 tenyks-cli-0.2.45/tenyks/model/upload_predictions.py
--rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)     4878 2023-06-06 14:49:32.000000 tenyks-cli-0.2.45/tenyks/upload_utilities.py
--rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)      629 2023-06-06 14:49:32.000000 tenyks-cli-0.2.45/tenyks/utilities.py
-drwxrwxr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-06-07 10:10:16.125957 tenyks-cli-0.2.45/tenyks_cli.egg-info/
--rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)      670 2023-06-07 10:10:16.000000 tenyks-cli-0.2.45/tenyks_cli.egg-info/PKG-INFO
--rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)     2495 2023-06-07 10:10:16.000000 tenyks-cli-0.2.45/tenyks_cli.egg-info/SOURCES.txt
--rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)        1 2023-06-07 10:10:16.000000 tenyks-cli-0.2.45/tenyks_cli.egg-info/dependency_links.txt
--rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)       47 2023-06-07 10:10:16.000000 tenyks-cli-0.2.45/tenyks_cli.egg-info/entry_points.txt
--rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)       54 2023-06-07 10:10:16.000000 tenyks-cli-0.2.45/tenyks_cli.egg-info/requires.txt
--rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)        7 2023-06-07 10:10:16.000000 tenyks-cli-0.2.45/tenyks_cli.egg-info/top_level.txt
+drwxrwxr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-06-09 10:24:16.130616 tenyks-cli-0.2.46/
+-rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)      584 2023-06-06 14:49:32.000000 tenyks-cli-0.2.46/Internal README.md
+-rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)       47 2023-06-06 14:49:32.000000 tenyks-cli-0.2.46/MANIFEST.in
+-rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)      670 2023-06-09 10:24:16.130616 tenyks-cli-0.2.46/PKG-INFO
+-rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)      290 2023-06-06 14:49:32.000000 tenyks-cli-0.2.46/README.md
+-rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)       86 2023-06-06 14:49:32.000000 tenyks-cli-0.2.46/pyproject.toml
+-rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)       88 2023-06-06 14:49:32.000000 tenyks-cli-0.2.46/requirements.txt
+-rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)      138 2023-06-09 10:24:16.130616 tenyks-cli-0.2.46/setup.cfg
+-rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)      812 2023-06-09 10:23:56.000000 tenyks-cli-0.2.46/setup.py
+drwxrwxr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-06-09 10:24:16.106616 tenyks-cli-0.2.46/tenyks/
+-rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-06-06 14:49:32.000000 tenyks-cli-0.2.46/tenyks/__init__.py
+-rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)       75 2023-06-06 14:49:32.000000 tenyks-cli-0.2.46/tenyks/__main__.py
+drwxrwxr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-06-09 10:24:16.106616 tenyks-cli-0.2.46/tenyks/adapters/
+-rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-06-06 14:49:32.000000 tenyks-cli-0.2.46/tenyks/adapters/__init__.py
+drwxrwxr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-06-09 10:24:16.106616 tenyks-cli-0.2.46/tenyks/adapters/categories/
+-rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-06-06 14:49:32.000000 tenyks-cli-0.2.46/tenyks/adapters/categories/__init__.py
+-rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)      746 2023-06-06 14:49:32.000000 tenyks-cli-0.2.46/tenyks/adapters/categories/category_reader_factory.py
+drwxrwxr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-06-09 10:24:16.110616 tenyks-cli-0.2.46/tenyks/adapters/categories/readers/
+-rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-06-06 14:49:32.000000 tenyks-cli-0.2.46/tenyks/adapters/categories/readers/__init__.py
+-rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)      255 2023-06-06 14:49:32.000000 tenyks-cli-0.2.46/tenyks/adapters/categories/readers/category_reader.py
+-rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)      321 2023-06-06 14:49:32.000000 tenyks-cli-0.2.46/tenyks/adapters/categories/readers/json_category_reader.py
+-rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)      440 2023-06-06 14:49:32.000000 tenyks-cli-0.2.46/tenyks/adapters/categories/readers/txt_category_reader.py
+-rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)      349 2023-06-06 14:49:32.000000 tenyks-cli-0.2.46/tenyks/adapters/config.py
+drwxrwxr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-06-09 10:24:16.110616 tenyks-cli-0.2.46/tenyks/adapters/detection/
+-rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-06-06 14:49:32.000000 tenyks-cli-0.2.46/tenyks/adapters/detection/__init__.py
+-rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)     2530 2023-06-06 14:49:32.000000 tenyks-cli-0.2.46/tenyks/adapters/detection/detection_adapter.py
+-rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)     1883 2023-06-06 14:49:32.000000 tenyks-cli-0.2.46/tenyks/adapters/detection/detection_adapter_factory.py
+-rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)      416 2023-06-06 14:49:32.000000 tenyks-cli-0.2.46/tenyks/adapters/detection/detection_data.py
+drwxrwxr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-06-09 10:24:16.114616 tenyks-cli-0.2.46/tenyks/adapters/detection/readers/
+-rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-06-06 14:49:32.000000 tenyks-cli-0.2.46/tenyks/adapters/detection/readers/__init__.py
+-rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)     2617 2023-06-06 14:49:32.000000 tenyks-cli-0.2.46/tenyks/adapters/detection/readers/classification_reader.py
+-rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)     3114 2023-06-06 14:49:32.000000 tenyks-cli-0.2.46/tenyks/adapters/detection/readers/deepstream_reader.py
+-rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)      477 2023-06-06 14:49:32.000000 tenyks-cli-0.2.46/tenyks/adapters/detection/readers/detection_reader.py
+-rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)     2586 2023-06-06 14:49:32.000000 tenyks-cli-0.2.46/tenyks/adapters/detection/readers/vott_csv_reader.py
+-rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)     3291 2023-06-06 14:49:32.000000 tenyks-cli-0.2.46/tenyks/adapters/detection/readers/yolo_reader.py
+drwxrwxr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-06-09 10:24:16.114616 tenyks-cli-0.2.46/tenyks/adapters/detection/writers/
+-rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-06-06 14:49:32.000000 tenyks-cli-0.2.46/tenyks/adapters/detection/writers/__init__.py
+-rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)     1599 2023-06-06 14:49:32.000000 tenyks-cli-0.2.46/tenyks/adapters/detection/writers/coco_writer.py
+-rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)      414 2023-06-06 14:49:32.000000 tenyks-cli-0.2.46/tenyks/adapters/detection/writers/detection_writer.py
+drwxrwxr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-06-09 10:24:16.118616 tenyks-cli-0.2.46/tenyks/adapters/utilities/
+-rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-06-06 14:49:32.000000 tenyks-cli-0.2.46/tenyks/adapters/utilities/__init__.py
+-rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)     1274 2023-06-06 14:49:32.000000 tenyks-cli-0.2.46/tenyks/adapters/utilities/bbox.py
+-rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)      388 2023-06-06 14:49:32.000000 tenyks-cli-0.2.46/tenyks/adapters/utilities/file.py
+-rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)     4490 2023-06-06 14:49:32.000000 tenyks-cli-0.2.46/tenyks/api.py
+-rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)     1600 2023-06-06 14:49:32.000000 tenyks-cli-0.2.46/tenyks/cli.py
+-rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)      995 2023-06-06 14:49:32.000000 tenyks-cli-0.2.46/tenyks/click_utilities.py
+drwxrwxr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-06-09 10:24:16.118616 tenyks-cli-0.2.46/tenyks/config/
+-rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-06-06 14:49:32.000000 tenyks-cli-0.2.46/tenyks/config/__init__.py
+-rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)     1719 2023-06-06 14:49:32.000000 tenyks-cli-0.2.46/tenyks/config/config.py
+-rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)     1499 2023-06-06 14:49:32.000000 tenyks-cli-0.2.46/tenyks/config/configure.py
+drwxrwxr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-06-09 10:24:16.118616 tenyks-cli-0.2.46/tenyks/config/providers/
+-rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-06-06 14:49:32.000000 tenyks-cli-0.2.46/tenyks/config/providers/__init__.py
+drwxrwxr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-06-09 10:24:16.118616 tenyks-cli-0.2.46/tenyks/config/providers/aws/
+-rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-06-06 14:49:32.000000 tenyks-cli-0.2.46/tenyks/config/providers/aws/__init__.py
+-rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)      841 2023-06-06 14:49:32.000000 tenyks-cli-0.2.46/tenyks/config/providers/aws/config_aws.py
+-rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)     1007 2023-06-06 14:49:32.000000 tenyks-cli-0.2.46/tenyks/config/providers/aws/configure_aws.py
+drwxrwxr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-06-09 10:24:16.122616 tenyks-cli-0.2.46/tenyks/convert/
+-rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-06-06 14:49:32.000000 tenyks-cli-0.2.46/tenyks/convert/__init__.py
+-rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)     2096 2023-06-06 14:49:32.000000 tenyks-cli-0.2.46/tenyks/convert/convert_detections_file.py
+-rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)     1616 2023-06-06 14:49:32.000000 tenyks-cli-0.2.46/tenyks/convert/detection_file_processor.py
+drwxrwxr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-06-09 10:24:16.122616 tenyks-cli-0.2.46/tenyks/dataset/
+-rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-06-06 14:49:32.000000 tenyks-cli-0.2.46/tenyks/dataset/__init__.py
+drwxrwxr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-06-09 10:24:16.126616 tenyks-cli-0.2.46/tenyks/dataset/aws/
+-rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-06-06 14:49:32.000000 tenyks-cli-0.2.46/tenyks/dataset/aws/__init__.py
+-rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)      545 2023-06-06 14:49:32.000000 tenyks-cli-0.2.46/tenyks/dataset/aws/dataclasses.py
+-rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)      107 2023-06-06 14:49:32.000000 tenyks-cli-0.2.46/tenyks/dataset/config.py
+-rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)     4200 2023-06-06 14:49:32.000000 tenyks-cli-0.2.46/tenyks/dataset/create_dataset.py
+-rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)     1939 2023-06-06 14:49:32.000000 tenyks-cli-0.2.46/tenyks/dataset/upload_annotations.py
+-rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)     1040 2023-06-06 14:49:32.000000 tenyks-cli-0.2.46/tenyks/dataset/upload_class_names.py
+-rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)      975 2023-06-06 14:49:32.000000 tenyks-cli-0.2.46/tenyks/dataset/upload_images.py
+-rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)     1104 2023-06-06 14:49:32.000000 tenyks-cli-0.2.46/tenyks/dataset/utilities.py
+drwxrwxr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-06-09 10:24:16.126616 tenyks-cli-0.2.46/tenyks/embeddings/
+-rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-06-06 14:49:32.000000 tenyks-cli-0.2.46/tenyks/embeddings/__init__.py
+-rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)     1306 2023-06-06 14:49:32.000000 tenyks-cli-0.2.46/tenyks/embeddings/upload_annotation_bbox_embeddings.py
+-rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)     1254 2023-06-06 14:49:32.000000 tenyks-cli-0.2.46/tenyks/embeddings/upload_image_embeddings.py
+-rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)     1471 2023-06-06 14:49:32.000000 tenyks-cli-0.2.46/tenyks/embeddings/upload_prediction_bbox_embeddings.py
+-rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)      346 2023-06-06 14:49:32.000000 tenyks-cli-0.2.46/tenyks/exceptions_handler.py
+drwxrwxr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-06-09 10:24:16.130616 tenyks-cli-0.2.46/tenyks/model/
+-rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-06-06 14:49:32.000000 tenyks-cli-0.2.46/tenyks/model/__init__.py
+-rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)     2730 2023-06-06 14:49:32.000000 tenyks-cli-0.2.46/tenyks/model/create_model.py
+-rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)     2119 2023-06-06 14:49:32.000000 tenyks-cli-0.2.46/tenyks/model/upload_predictions.py
+-rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)     4942 2023-06-09 10:23:56.000000 tenyks-cli-0.2.46/tenyks/upload_utilities.py
+-rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)      629 2023-06-06 14:49:32.000000 tenyks-cli-0.2.46/tenyks/utilities.py
+drwxrwxr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-06-09 10:24:16.130616 tenyks-cli-0.2.46/tenyks_cli.egg-info/
+-rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)      670 2023-06-09 10:24:16.000000 tenyks-cli-0.2.46/tenyks_cli.egg-info/PKG-INFO
+-rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)     2495 2023-06-09 10:24:16.000000 tenyks-cli-0.2.46/tenyks_cli.egg-info/SOURCES.txt
+-rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)        1 2023-06-09 10:24:16.000000 tenyks-cli-0.2.46/tenyks_cli.egg-info/dependency_links.txt
+-rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)       47 2023-06-09 10:24:16.000000 tenyks-cli-0.2.46/tenyks_cli.egg-info/entry_points.txt
+-rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)       54 2023-06-09 10:24:16.000000 tenyks-cli-0.2.46/tenyks_cli.egg-info/requires.txt
+-rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)        7 2023-06-09 10:24:16.000000 tenyks-cli-0.2.46/tenyks_cli.egg-info/top_level.txt
```

### Comparing `tenyks-cli-0.2.45/Internal README.md` & `tenyks-cli-0.2.46/Internal README.md`

 * *Files identical despite different names*

### Comparing `tenyks-cli-0.2.45/PKG-INFO` & `tenyks-cli-0.2.46/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tenyks-cli
-Version: 0.2.45
+Version: 0.2.46
 Summary: Tenyks AI
 Home-page: https://www.tenyks.ai/
 Author: Tenyks AI
 Author-email: info@tenyks.ai
 License: MIT
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tenyks-cli-0.2.45/setup.py` & `tenyks-cli-0.2.46/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("requirements.txt", "r") as fh:
     install_requires = fh.read().split("\n")
 
 setup(
     name="tenyks-cli",
-    version="0.2.45",
+    version="0.2.46",
     author="Tenyks AI",
     author_email="info@tenyks.ai",
     license="MIT",
     description="Tenyks AI",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://www.tenyks.ai/",
```

### Comparing `tenyks-cli-0.2.45/tenyks/adapters/categories/category_reader_factory.py` & `tenyks-cli-0.2.46/tenyks/adapters/categories/category_reader_factory.py`

 * *Files identical despite different names*

### Comparing `tenyks-cli-0.2.45/tenyks/adapters/detection/detection_adapter.py` & `tenyks-cli-0.2.46/tenyks/adapters/detection/detection_adapter.py`

 * *Files identical despite different names*

### Comparing `tenyks-cli-0.2.45/tenyks/adapters/detection/detection_adapter_factory.py` & `tenyks-cli-0.2.46/tenyks/adapters/detection/detection_adapter_factory.py`

 * *Files identical despite different names*

### Comparing `tenyks-cli-0.2.45/tenyks/adapters/detection/readers/classification_reader.py` & `tenyks-cli-0.2.46/tenyks/adapters/detection/readers/classification_reader.py`

 * *Files identical despite different names*

### Comparing `tenyks-cli-0.2.45/tenyks/adapters/detection/readers/deepstream_reader.py` & `tenyks-cli-0.2.46/tenyks/adapters/detection/readers/deepstream_reader.py`

 * *Files identical despite different names*

### Comparing `tenyks-cli-0.2.45/tenyks/adapters/detection/readers/vott_csv_reader.py` & `tenyks-cli-0.2.46/tenyks/adapters/detection/readers/vott_csv_reader.py`

 * *Files identical despite different names*

### Comparing `tenyks-cli-0.2.45/tenyks/adapters/detection/readers/yolo_reader.py` & `tenyks-cli-0.2.46/tenyks/adapters/detection/readers/yolo_reader.py`

 * *Files identical despite different names*

### Comparing `tenyks-cli-0.2.45/tenyks/adapters/detection/writers/coco_writer.py` & `tenyks-cli-0.2.46/tenyks/adapters/detection/writers/coco_writer.py`

 * *Files identical despite different names*

### Comparing `tenyks-cli-0.2.45/tenyks/adapters/utilities/bbox.py` & `tenyks-cli-0.2.46/tenyks/adapters/utilities/bbox.py`

 * *Files identical despite different names*

### Comparing `tenyks-cli-0.2.45/tenyks/api.py` & `tenyks-cli-0.2.46/tenyks/api.py`

 * *Files identical despite different names*

### Comparing `tenyks-cli-0.2.45/tenyks/cli.py` & `tenyks-cli-0.2.46/tenyks/cli.py`

 * *Files identical despite different names*

### Comparing `tenyks-cli-0.2.45/tenyks/click_utilities.py` & `tenyks-cli-0.2.46/tenyks/click_utilities.py`

 * *Files identical despite different names*

### Comparing `tenyks-cli-0.2.45/tenyks/config/config.py` & `tenyks-cli-0.2.46/tenyks/config/config.py`

 * *Files identical despite different names*

### Comparing `tenyks-cli-0.2.45/tenyks/config/configure.py` & `tenyks-cli-0.2.46/tenyks/config/configure.py`

 * *Files identical despite different names*

### Comparing `tenyks-cli-0.2.45/tenyks/config/providers/aws/config_aws.py` & `tenyks-cli-0.2.46/tenyks/config/providers/aws/config_aws.py`

 * *Files identical despite different names*

### Comparing `tenyks-cli-0.2.45/tenyks/config/providers/aws/configure_aws.py` & `tenyks-cli-0.2.46/tenyks/config/providers/aws/configure_aws.py`

 * *Files identical despite different names*

### Comparing `tenyks-cli-0.2.45/tenyks/convert/convert_detections_file.py` & `tenyks-cli-0.2.46/tenyks/convert/convert_detections_file.py`

 * *Files identical despite different names*

### Comparing `tenyks-cli-0.2.45/tenyks/convert/detection_file_processor.py` & `tenyks-cli-0.2.46/tenyks/convert/detection_file_processor.py`

 * *Files identical despite different names*

### Comparing `tenyks-cli-0.2.45/tenyks/dataset/aws/dataclasses.py` & `tenyks-cli-0.2.46/tenyks/dataset/aws/dataclasses.py`

 * *Files identical despite different names*

### Comparing `tenyks-cli-0.2.45/tenyks/dataset/create_dataset.py` & `tenyks-cli-0.2.46/tenyks/dataset/create_dataset.py`

 * *Files identical despite different names*

### Comparing `tenyks-cli-0.2.45/tenyks/dataset/upload_annotations.py` & `tenyks-cli-0.2.46/tenyks/dataset/upload_annotations.py`

 * *Files identical despite different names*

### Comparing `tenyks-cli-0.2.45/tenyks/dataset/upload_class_names.py` & `tenyks-cli-0.2.46/tenyks/dataset/upload_class_names.py`

 * *Files identical despite different names*

### Comparing `tenyks-cli-0.2.45/tenyks/dataset/upload_images.py` & `tenyks-cli-0.2.46/tenyks/dataset/upload_images.py`

 * *Files identical despite different names*

### Comparing `tenyks-cli-0.2.45/tenyks/dataset/utilities.py` & `tenyks-cli-0.2.46/tenyks/dataset/utilities.py`

 * *Files identical despite different names*

### Comparing `tenyks-cli-0.2.45/tenyks/embeddings/upload_annotation_bbox_embeddings.py` & `tenyks-cli-0.2.46/tenyks/embeddings/upload_annotation_bbox_embeddings.py`

 * *Files identical despite different names*

### Comparing `tenyks-cli-0.2.45/tenyks/embeddings/upload_image_embeddings.py` & `tenyks-cli-0.2.46/tenyks/embeddings/upload_image_embeddings.py`

 * *Files identical despite different names*

### Comparing `tenyks-cli-0.2.45/tenyks/embeddings/upload_prediction_bbox_embeddings.py` & `tenyks-cli-0.2.46/tenyks/embeddings/upload_prediction_bbox_embeddings.py`

 * *Files identical despite different names*

### Comparing `tenyks-cli-0.2.45/tenyks/model/create_model.py` & `tenyks-cli-0.2.46/tenyks/model/create_model.py`

 * *Files identical despite different names*

### Comparing `tenyks-cli-0.2.45/tenyks/model/upload_predictions.py` & `tenyks-cli-0.2.46/tenyks/model/upload_predictions.py`

 * *Files identical despite different names*

### Comparing `tenyks-cli-0.2.45/tenyks/upload_utilities.py` & `tenyks-cli-0.2.46/tenyks/upload_utilities.py`

 * *Files 3% similar despite different names*

```diff
@@ -74,18 +74,18 @@
             def handle_succeeded(file_info: FileInfo) -> None:
                 successful_upload_file_names.append(file_info.name)
                 if verbose:
                     click.echo(f"Successfully uploaded {file_info.name}")
                 else:
                     progress_bar.update(1)
 
-            def handle_failed(file_info: FileInfo) -> None:
+            def handle_failed(file_info: FileInfo, response) -> None:
                 failed_upload_file_names.append(file_info.name)
                 if verbose:
-                    click.echo(f"Failed to upload {file_info.name}")
+                    click.echo(f"Failed to upload {file_info.name}, {response}")
                 else:
                     progress_bar.update(1)
 
             for file_info in file_info_list:
                 task = asyncio.create_task(
                     upload_file_to_location(
                         file_info,
@@ -106,15 +106,15 @@
 async def upload_file_to_location(
     file_info: FileInfo,
     upload_url: str,
     session,
     sem,
     api: Api,
     on_succeeded: Callable[[str], None],
-    on_failed: Callable[[str], None],
+    on_failed: Callable[[str, object], None],
 ):
     async with sem:
         file = open(file_info.path, "rb")
         file_content = file.read()
         file.close()
         for i in range(RETRIES_PER_FILE):
             data = aiohttp.FormData()
@@ -131,23 +131,23 @@
                         return
 
                     click.echo(
                         f"Failed to upload {file_info.name} on attempt {i+1} out of {RETRIES_PER_FILE}. Retrying.."
                     )
 
                     if i >= RETRIES_PER_FILE:
-                        on_failed(file_info)
+                        on_failed(file_info, response)
                         return
                     elif status == 401:
                         new_auth = api.get_authenticated_header()
                         session.headers["Authorization"] = new_auth["Authorization"]
                         await asyncio.sleep(i * i)
 
-            except aiohttp.ClientError:
-                on_failed(file_info)
+            except aiohttp.ClientError as exception:
+                on_failed(file_info, exception)
 
 
 def get_valid_files_from_directory(
     directory: str, accepted_extensions: List[str]
 ) -> List[FileInfo]:
     if os.path.exists(directory) is False:
         raise ValueError(f"File path {directory} does not exist...")
```

### Comparing `tenyks-cli-0.2.45/tenyks/utilities.py` & `tenyks-cli-0.2.46/tenyks/utilities.py`

 * *Files identical despite different names*

### Comparing `tenyks-cli-0.2.45/tenyks_cli.egg-info/PKG-INFO` & `tenyks-cli-0.2.46/tenyks_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tenyks-cli
-Version: 0.2.45
+Version: 0.2.46
 Summary: Tenyks AI
 Home-page: https://www.tenyks.ai/
 Author: Tenyks AI
 Author-email: info@tenyks.ai
 License: MIT
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tenyks-cli-0.2.45/tenyks_cli.egg-info/SOURCES.txt` & `tenyks-cli-0.2.46/tenyks_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

