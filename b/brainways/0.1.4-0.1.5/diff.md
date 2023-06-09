# Comparing `tmp/brainways-0.1.4.tar.gz` & `tmp/brainways-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brainways-0.1.4.tar", last modified: Thu Jun  8 07:42:29 2023, max compression
+gzip compressed data, was "brainways-0.1.5.tar", last modified: Fri Jun  9 09:31:57 2023, max compression
```

## Comparing `brainways-0.1.4.tar` & `brainways-0.1.5.tar`

### file list

```diff
@@ -1,182 +1,187 @@
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-08 07:42:29.548988 brainways-0.1.4/
--rw-rw-r--   0 ben       (1001) ben       (1001)      292 2022-07-13 13:47:58.000000 brainways-0.1.4/.editorconfig
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-08 07:42:29.532988 brainways-0.1.4/.github/
--rw-rw-r--   0 ben       (1001) ben       (1001)      320 2022-07-13 13:47:58.000000 brainways-0.1.4/.github/ISSUE_TEMPLATE.md
--rw-rw-r--   0 ben       (1001) ben       (1001)     1248 2022-07-13 14:46:16.000000 brainways-0.1.4/.gitignore
--rw-rw-r--   0 ben       (1001) ben       (1001)     1194 2022-07-14 13:50:01.000000 brainways-0.1.4/.pre-commit-config.yaml
--rw-rw-r--   0 ben       (1001) ben       (1001)      681 2022-07-13 13:47:58.000000 brainways-0.1.4/.travis.yml
--rw-rw-r--   0 ben       (1001) ben       (1001)      160 2022-07-13 13:47:58.000000 brainways-0.1.4/AUTHORS.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)     3523 2022-07-13 13:47:58.000000 brainways-0.1.4/CONTRIBUTING.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)       89 2022-07-13 13:47:58.000000 brainways-0.1.4/HISTORY.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)    35148 2022-08-24 08:26:24.000000 brainways-0.1.4/LICENSE
--rw-rw-r--   0 ben       (1001) ben       (1001)      262 2022-07-13 13:47:58.000000 brainways-0.1.4/MANIFEST.in
--rw-rw-r--   0 ben       (1001) ben       (1001)     2430 2023-05-26 08:21:13.000000 brainways-0.1.4/Makefile
--rw-rw-r--   0 ben       (1001) ben       (1001)     2343 2023-06-08 07:42:29.548988 brainways-0.1.4/PKG-INFO
--rw-rw-r--   0 ben       (1001) ben       (1001)      962 2023-05-26 08:25:05.000000 brainways-0.1.4/README.rst
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-08 07:42:29.532988 brainways-0.1.4/data/
--rw-rw-r--   0 ben       (1001) ben       (1001)   269441 2022-03-11 09:30:01.000000 brainways-0.1.4/data/test_data.npz
--rw-rw-r--   0 ben       (1001) ben       (1001)    47973 2022-06-30 11:17:43.000000 brainways-0.1.4/data/test_image.jpg
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-08 07:42:29.536988 brainways-0.1.4/docs/
--rw-rw-r--   0 ben       (1001) ben       (1001)      610 2022-07-13 13:47:58.000000 brainways-0.1.4/docs/Makefile
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-08 07:42:29.528988 brainways-0.1.4/docs/_build/
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-08 07:42:29.528988 brainways-0.1.4/docs/_build/html/
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-08 07:42:29.536988 brainways-0.1.4/docs/_build/html/_static/
--rw-rw-r--   0 ben       (1001) ben       (1001)      286 2022-10-06 11:03:00.000000 brainways-0.1.4/docs/_build/html/_static/file.png
--rw-rw-r--   0 ben       (1001) ben       (1001)       90 2022-10-06 11:03:00.000000 brainways-0.1.4/docs/_build/html/_static/minus.png
--rw-rw-r--   0 ben       (1001) ben       (1001)       90 2022-10-06 11:03:00.000000 brainways-0.1.4/docs/_build/html/_static/plus.png
--rw-rw-r--   0 ben       (1001) ben       (1001)       28 2022-07-13 13:47:58.000000 brainways-0.1.4/docs/authors.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)      361 2023-05-26 08:18:55.000000 brainways-0.1.4/docs/brainways.elastix.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)     1317 2023-05-26 08:18:55.000000 brainways-0.1.4/docs/brainways.pipeline.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)      770 2023-05-26 08:18:55.000000 brainways-0.1.4/docs/brainways.project.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)      500 2023-05-26 08:26:43.000000 brainways-0.1.4/docs/brainways.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)     2137 2023-05-26 08:18:55.000000 brainways-0.1.4/docs/brainways.scripts.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)     1387 2023-05-26 08:18:55.000000 brainways-0.1.4/docs/brainways.transforms.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)      601 2023-05-26 08:18:55.000000 brainways-0.1.4/docs/brainways.utils.atlas.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)     1405 2023-05-26 08:18:55.000000 brainways-0.1.4/docs/brainways.utils.cell_detection_importer.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)      386 2023-05-26 08:18:55.000000 brainways-0.1.4/docs/brainways.utils.czi.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)      971 2023-05-26 08:18:55.000000 brainways-0.1.4/docs/brainways.utils.io_utils.file_iterators.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)     1145 2023-05-26 08:18:55.000000 brainways-0.1.4/docs/brainways.utils.io_utils.readers.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)      553 2023-05-26 08:18:55.000000 brainways-0.1.4/docs/brainways.utils.io_utils.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)     1833 2023-05-26 08:18:55.000000 brainways-0.1.4/docs/brainways.utils.rst
--rwxrwxr-x   0 ben       (1001) ben       (1001)     4967 2023-05-26 08:17:55.000000 brainways-0.1.4/docs/conf.py
--rw-rw-r--   0 ben       (1001) ben       (1001)       33 2022-07-13 13:47:58.000000 brainways-0.1.4/docs/contributing.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)       28 2022-07-13 13:47:58.000000 brainways-0.1.4/docs/history.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)      306 2022-07-13 13:47:58.000000 brainways-0.1.4/docs/index.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)     1118 2022-07-13 13:47:58.000000 brainways-0.1.4/docs/installation.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)      807 2022-07-13 13:47:58.000000 brainways-0.1.4/docs/make.bat
--rw-rw-r--   0 ben       (1001) ben       (1001)       64 2023-05-26 08:26:43.000000 brainways-0.1.4/docs/modules.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)       27 2022-07-13 13:47:58.000000 brainways-0.1.4/docs/readme.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)       73 2022-07-13 13:47:58.000000 brainways-0.1.4/docs/usage.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)      383 2023-05-26 08:03:19.000000 brainways-0.1.4/pyproject.toml
--rw-rw-r--   0 ben       (1001) ben       (1001)      165 2022-07-13 14:08:33.000000 brainways-0.1.4/requirements_dev.txt
--rw-rw-r--   0 ben       (1001) ben       (1001)     1967 2023-06-08 07:42:29.548988 brainways-0.1.4/setup.cfg
--rw-rw-r--   0 ben       (1001) ben       (1001)       60 2023-05-26 07:59:05.000000 brainways-0.1.4/setup.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-08 07:42:29.528988 brainways-0.1.4/src/
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-08 07:42:29.536988 brainways-0.1.4/src/brainways/
--rw-rw-r--   0 ben       (1001) ben       (1001)        0 2022-07-13 14:28:10.000000 brainways-0.1.4/src/brainways/__init__.py
--rw-rw-r--   0 ben       (1001) ben       (1001)      160 2023-06-08 07:42:29.000000 brainways-0.1.4/src/brainways/_version.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     7168 2023-06-07 15:59:32.000000 brainways-0.1.4/src/brainways/conftest.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-08 07:42:29.536988 brainways-0.1.4/src/brainways/elastix/
--rw-rw-r--   0 ben       (1001) ben       (1001)     2596 2022-07-14 13:40:58.000000 brainways-0.1.4/src/brainways/elastix/Par0033bspline.txt
--rw-rw-r--   0 ben       (1001) ben       (1001)     2316 2022-07-14 13:40:58.000000 brainways-0.1.4/src/brainways/elastix/Par0033similarity.txt
--rw-rw-r--   0 ben       (1001) ben       (1001)        0 2021-12-09 12:20:50.000000 brainways-0.1.4/src/brainways/elastix/__init__.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-08 07:42:29.536988 brainways-0.1.4/src/brainways/elastix/_tests/
--rw-rw-r--   0 ben       (1001) ben       (1001)      592 2022-10-27 09:03:02.000000 brainways-0.1.4/src/brainways/elastix/_tests/test_elastix.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     2649 2022-09-08 14:32:33.000000 brainways-0.1.4/src/brainways/elastix/elastix.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-08 07:42:29.536988 brainways-0.1.4/src/brainways/pipeline/
--rw-rw-r--   0 ben       (1001) ben       (1001)        0 2022-07-07 09:39:04.000000 brainways-0.1.4/src/brainways/pipeline/__init__.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-08 07:42:29.536988 brainways-0.1.4/src/brainways/pipeline/_tests/
--rw-rw-r--   0 ben       (1001) ben       (1001)      430 2022-10-27 09:03:02.000000 brainways-0.1.4/src/brainways/pipeline/_tests/test_atlas_registration.py
--rw-rw-r--   0 ben       (1001) ben       (1001)      552 2022-11-23 11:34:52.000000 brainways-0.1.4/src/brainways/pipeline/_tests/test_brainways_pipeline.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     1097 2022-11-30 13:23:46.000000 brainways-0.1.4/src/brainways/pipeline/affine_2d.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     2339 2023-05-24 12:27:57.000000 brainways-0.1.4/src/brainways/pipeline/atlas_registration.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     1165 2023-06-07 14:11:19.000000 brainways-0.1.4/src/brainways/pipeline/brainways_params.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     3712 2022-11-30 13:35:53.000000 brainways-0.1.4/src/brainways/pipeline/brainways_pipeline.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     5186 2023-06-07 15:47:46.000000 brainways-0.1.4/src/brainways/pipeline/cell_detector.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     1596 2022-11-30 13:25:23.000000 brainways-0.1.4/src/brainways/pipeline/tps.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-08 07:42:29.540988 brainways-0.1.4/src/brainways/project/
--rw-rw-r--   0 ben       (1001) ben       (1001)        0 2022-07-07 09:39:04.000000 brainways-0.1.4/src/brainways/project/__init__.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-08 07:42:29.540988 brainways-0.1.4/src/brainways/project/_tests/
--rw-rw-r--   0 ben       (1001) ben       (1001)        0 2022-07-14 12:32:42.000000 brainways-0.1.4/src/brainways/project/_tests/__init__.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     1003 2023-06-07 11:33:52.000000 brainways-0.1.4/src/brainways/project/_tests/conftest.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     2598 2023-06-08 07:32:26.000000 brainways-0.1.4/src/brainways/project/_tests/test_brainways_project.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     8619 2023-06-07 11:26:16.000000 brainways-0.1.4/src/brainways/project/_tests/test_brainways_subject.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-08 07:42:29.528988 brainways-0.1.4/src/brainways/project/_tests/test_projects/
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-08 07:42:29.540988 brainways-0.1.4/src/brainways/project/_tests/test_projects/v0.1.1/
--rw-rw-r--   0 ben       (1001) ben       (1001)       38 2023-06-07 15:59:39.000000 brainways-0.1.4/src/brainways/project/_tests/test_projects/v0.1.1/project.bwp
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-08 07:42:29.540988 brainways-0.1.4/src/brainways/project/_tests/test_projects/v0.1.1/subject1/
--rw-rw-r--   0 ben       (1001) ben       (1001)     2155 2023-06-07 10:30:28.000000 brainways-0.1.4/src/brainways/project/_tests/test_projects/v0.1.1/subject1/brainways.bin
--rw-rw-r--   0 ben       (1001) ben       (1001)      388 2023-06-07 11:49:25.000000 brainways-0.1.4/src/brainways/project/_tests/test_utils.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     1493 2023-06-08 07:35:04.000000 brainways-0.1.4/src/brainways/project/_utils.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     8792 2023-06-07 15:29:27.000000 brainways-0.1.4/src/brainways/project/brainways_project.py
--rw-rw-r--   0 ben       (1001) ben       (1001)    18458 2023-06-07 13:06:53.000000 brainways-0.1.4/src/brainways/project/brainways_subject.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     1388 2023-06-07 15:59:32.000000 brainways-0.1.4/src/brainways/project/info_classes.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-08 07:42:29.540988 brainways-0.1.4/src/brainways/scripts/
--rw-rw-r--   0 ben       (1001) ben       (1001)        0 2022-07-14 12:32:42.000000 brainways-0.1.4/src/brainways/scripts/__init__.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-08 07:42:29.540988 brainways-0.1.4/src/brainways/scripts/_tests/
--rw-rw-r--   0 ben       (1001) ben       (1001)      920 2023-05-26 08:21:13.000000 brainways-0.1.4/src/brainways/scripts/_tests/test_cli.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     3031 2022-09-08 14:06:58.000000 brainways-0.1.4/src/brainways/scripts/batch_create_thumbnails.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     3053 2023-05-07 14:18:30.000000 brainways-0.1.4/src/brainways/scripts/cell_detection.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     1142 2023-05-04 08:18:52.000000 brainways-0.1.4/src/brainways/scripts/cli.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     1588 2023-05-07 14:18:29.000000 brainways-0.1.4/src/brainways/scripts/create_excel.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     4944 2022-11-30 14:10:59.000000 brainways-0.1.4/src/brainways/scripts/create_excel_colabelling.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     4023 2022-11-23 12:26:10.000000 brainways-0.1.4/src/brainways/scripts/create_reg_model_data.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     5253 2022-11-23 12:35:34.000000 brainways-0.1.4/src/brainways/scripts/display_area.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     1618 2022-12-08 14:20:04.000000 brainways-0.1.4/src/brainways/scripts/import_cell_detections_keren.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     1192 2022-11-23 12:26:10.000000 brainways-0.1.4/src/brainways/scripts/import_cells.py
--rw-rw-r--   0 ben       (1001) ben       (1001)      920 2022-12-11 10:14:02.000000 brainways-0.1.4/src/brainways/scripts/move_images.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-08 07:42:29.540988 brainways-0.1.4/src/brainways/transforms/
--rw-rw-r--   0 ben       (1001) ben       (1001)        0 2022-04-27 09:13:34.000000 brainways-0.1.4/src/brainways/transforms/__init__.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-08 07:42:29.544988 brainways-0.1.4/src/brainways/transforms/_tests/
--rw-rw-r--   0 ben       (1001) ben       (1001)        0 2022-04-27 09:13:34.000000 brainways-0.1.4/src/brainways/transforms/_tests/__init__.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     2173 2022-07-14 13:48:40.000000 brainways-0.1.4/src/brainways/transforms/_tests/test_affine_transform_2d.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     1813 2022-11-23 11:35:37.000000 brainways-0.1.4/src/brainways/transforms/_tests/test_depth_registration.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     2034 2022-07-14 13:48:40.000000 brainways-0.1.4/src/brainways/transforms/_tests/test_image_to_atlas_transform.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     2667 2022-07-14 13:48:40.000000 brainways-0.1.4/src/brainways/transforms/_tests/test_tps_transform.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     4104 2022-11-30 13:34:33.000000 brainways-0.1.4/src/brainways/transforms/affine_transform_2d.py
--rw-rw-r--   0 ben       (1001) ben       (1001)      436 2022-07-14 12:46:19.000000 brainways-0.1.4/src/brainways/transforms/base.py
--rw-rw-r--   0 ben       (1001) ben       (1001)      623 2022-07-14 13:40:58.000000 brainways-0.1.4/src/brainways/transforms/compose.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     2594 2022-07-14 13:48:40.000000 brainways-0.1.4/src/brainways/transforms/depth_registration.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     2205 2022-09-08 13:13:42.000000 brainways-0.1.4/src/brainways/transforms/image_to_atlas_transform.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     2185 2022-11-30 13:46:38.000000 brainways-0.1.4/src/brainways/transforms/tps_transform.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-08 07:42:29.544988 brainways-0.1.4/src/brainways/utils/
--rw-rw-r--   0 ben       (1001) ben       (1001)        0 2021-07-21 08:14:53.000000 brainways-0.1.4/src/brainways/utils/__init__.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     1674 2022-07-17 07:51:20.000000 brainways-0.1.4/src/brainways/utils/_imports.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-08 07:42:29.544988 brainways-0.1.4/src/brainways/utils/_tests/
--rw-rw-r--   0 ben       (1001) ben       (1001)        0 2022-07-14 12:32:42.000000 brainways-0.1.4/src/brainways/utils/_tests/__init__.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     7710 2023-05-26 08:21:13.000000 brainways-0.1.4/src/brainways/utils/_tests/test_cell_count_summary.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     2715 2023-05-07 14:18:30.000000 brainways-0.1.4/src/brainways/utils/_tests/test_cells.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     2412 2022-07-14 13:48:40.000000 brainways-0.1.4/src/brainways/utils/_tests/test_image.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-08 07:42:29.544988 brainways-0.1.4/src/brainways/utils/atlas/
--rw-rw-r--   0 ben       (1001) ben       (1001)        0 2021-07-21 11:07:35.000000 brainways-0.1.4/src/brainways/utils/atlas/__init__.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-08 07:42:29.544988 brainways-0.1.4/src/brainways/utils/atlas/_tests/
--rw-rw-r--   0 ben       (1001) ben       (1001)        0 2022-04-27 09:13:34.000000 brainways-0.1.4/src/brainways/utils/atlas/_tests/__init__.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     3708 2022-07-14 13:40:59.000000 brainways-0.1.4/src/brainways/utils/atlas/_tests/test_slice_atlas.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     4263 2022-12-11 16:13:39.000000 brainways-0.1.4/src/brainways/utils/atlas/brainways_atlas.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     2280 2023-05-04 09:01:16.000000 brainways-0.1.4/src/brainways/utils/atlas/slice_atlas.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     5751 2023-05-14 15:00:03.000000 brainways-0.1.4/src/brainways/utils/cell_count_summary.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-08 07:42:29.544988 brainways-0.1.4/src/brainways/utils/cell_detection_importer/
--rw-rw-r--   0 ben       (1001) ben       (1001)        0 2022-10-06 09:31:17.000000 brainways-0.1.4/src/brainways/utils/cell_detection_importer/__init__.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-08 07:42:29.548988 brainways-0.1.4/src/brainways/utils/cell_detection_importer/_tests/
--rw-rw-r--   0 ben       (1001) ben       (1001)     7465 2022-10-06 10:12:40.000000 brainways-0.1.4/src/brainways/utils/cell_detection_importer/_tests/qupath_sample_file.txt
--rw-rw-r--   0 ben       (1001) ben       (1001)     1240 2022-11-23 12:23:47.000000 brainways-0.1.4/src/brainways/utils/cell_detection_importer/_tests/test_brainways_cell_detection_importer.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     1722 2022-12-08 14:20:04.000000 brainways-0.1.4/src/brainways/utils/cell_detection_importer/_tests/test_qupath_cell_detection_importer.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     1343 2022-11-23 12:26:10.000000 brainways-0.1.4/src/brainways/utils/cell_detection_importer/brainways_cell_detection_importer.py
--rw-rw-r--   0 ben       (1001) ben       (1001)      507 2022-11-27 15:04:03.000000 brainways-0.1.4/src/brainways/utils/cell_detection_importer/cell_detection_importer.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     2438 2022-12-11 10:33:01.000000 brainways-0.1.4/src/brainways/utils/cell_detection_importer/keren_cell_detection_importer.py
--rw-rw-r--   0 ben       (1001) ben       (1001)      731 2022-12-08 14:20:04.000000 brainways-0.1.4/src/brainways/utils/cell_detection_importer/utils.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     4985 2023-05-02 09:29:03.000000 brainways-0.1.4/src/brainways/utils/cells.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     4270 2022-09-11 13:34:36.000000 brainways-0.1.4/src/brainways/utils/config.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-08 07:42:29.548988 brainways-0.1.4/src/brainways/utils/czi/
--rw-rw-r--   0 ben       (1001) ben       (1001)        0 2021-07-15 08:31:32.000000 brainways-0.1.4/src/brainways/utils/czi/__init__.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     1112 2022-07-14 13:48:40.000000 brainways-0.1.4/src/brainways/utils/czi/czi_to_jpg.py
--rw-rw-r--   0 ben       (1001) ben       (1001)      793 2022-07-14 12:49:34.000000 brainways-0.1.4/src/brainways/utils/dataclasses.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     9025 2023-05-26 13:51:47.000000 brainways-0.1.4/src/brainways/utils/image.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-08 07:42:29.548988 brainways-0.1.4/src/brainways/utils/io_utils/
--rw-rw-r--   0 ben       (1001) ben       (1001)       42 2022-07-17 07:44:03.000000 brainways-0.1.4/src/brainways/utils/io_utils/__init__.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-08 07:42:29.548988 brainways-0.1.4/src/brainways/utils/io_utils/file_iterators/
--rw-rw-r--   0 ben       (1001) ben       (1001)      379 2022-09-08 08:38:22.000000 brainways-0.1.4/src/brainways/utils/io_utils/file_iterators/__init__.py
--rw-rw-r--   0 ben       (1001) ben       (1001)      230 2022-07-07 09:39:04.000000 brainways-0.1.4/src/brainways/utils/io_utils/file_iterators/image_entry.py
--rw-rw-r--   0 ben       (1001) ben       (1001)      407 2022-07-07 09:39:04.000000 brainways-0.1.4/src/brainways/utils/io_utils/file_iterators/path.py
--rw-rw-r--   0 ben       (1001) ben       (1001)      914 2022-11-23 12:29:43.000000 brainways-0.1.4/src/brainways/utils/io_utils/file_iterators/qupath.py
--rw-rw-r--   0 ben       (1001) ben       (1001)      630 2022-07-07 09:39:09.000000 brainways-0.1.4/src/brainways/utils/io_utils/image_path.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-08 07:42:29.548988 brainways-0.1.4/src/brainways/utils/io_utils/readers/
--rw-rw-r--   0 ben       (1001) ben       (1001)     1041 2022-09-11 12:16:49.000000 brainways-0.1.4/src/brainways/utils/io_utils/readers/__init__.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-08 07:42:29.548988 brainways-0.1.4/src/brainways/utils/io_utils/readers/_tests/
--rw-rw-r--   0 ben       (1001) ben       (1001)      218 2022-09-22 07:42:16.000000 brainways-0.1.4/src/brainways/utils/io_utils/readers/_tests/test_qupath_reader.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     1419 2022-09-08 08:38:21.000000 brainways-0.1.4/src/brainways/utils/io_utils/readers/aicsimageio_reader.py
--rw-rw-r--   0 ben       (1001) ben       (1001)      649 2022-07-14 12:39:58.000000 brainways-0.1.4/src/brainways/utils/io_utils/readers/base.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     1364 2022-09-08 08:38:21.000000 brainways-0.1.4/src/brainways/utils/io_utils/readers/czi_reader.py
--rw-rw-r--   0 ben       (1001) ben       (1001)    15748 2023-05-21 10:26:48.000000 brainways-0.1.4/src/brainways/utils/io_utils/readers/qupath_reader.py
--rw-rw-r--   0 ben       (1001) ben       (1001)      108 2022-09-11 13:34:36.000000 brainways-0.1.4/src/brainways/utils/paths.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     1181 2022-07-14 13:48:40.000000 brainways-0.1.4/src/brainways/utils/preprocess.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     3183 2022-09-11 10:47:30.000000 brainways-0.1.4/src/brainways/utils/qupath.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     1083 2022-07-14 13:48:39.000000 brainways-0.1.4/src/brainways/utils/test_utils.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-08 07:42:29.536988 brainways-0.1.4/src/brainways.egg-info/
--rw-rw-r--   0 ben       (1001) ben       (1001)     2343 2023-06-08 07:42:29.000000 brainways-0.1.4/src/brainways.egg-info/PKG-INFO
--rw-rw-r--   0 ben       (1001) ben       (1001)     5542 2023-06-08 07:42:29.000000 brainways-0.1.4/src/brainways.egg-info/SOURCES.txt
--rw-rw-r--   0 ben       (1001) ben       (1001)        1 2023-06-08 07:42:29.000000 brainways-0.1.4/src/brainways.egg-info/dependency_links.txt
--rw-rw-r--   0 ben       (1001) ben       (1001)       57 2023-06-08 07:42:29.000000 brainways-0.1.4/src/brainways.egg-info/entry_points.txt
--rw-rw-r--   0 ben       (1001) ben       (1001)      413 2023-06-08 07:42:29.000000 brainways-0.1.4/src/brainways.egg-info/requires.txt
--rw-rw-r--   0 ben       (1001) ben       (1001)       10 2023-06-08 07:42:29.000000 brainways-0.1.4/src/brainways.egg-info/top_level.txt
--rw-rw-r--   0 ben       (1001) ben       (1001)      540 2022-07-13 13:47:58.000000 brainways-0.1.4/tox.ini
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-09 09:31:57.298109 brainways-0.1.5/
+-rw-rw-r--   0 ben       (1001) ben       (1001)      292 2022-07-13 13:47:58.000000 brainways-0.1.5/.editorconfig
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-09 09:31:57.282109 brainways-0.1.5/.github/
+-rw-rw-r--   0 ben       (1001) ben       (1001)      320 2022-07-13 13:47:58.000000 brainways-0.1.5/.github/ISSUE_TEMPLATE.md
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1248 2022-07-13 14:46:16.000000 brainways-0.1.5/.gitignore
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1194 2022-07-14 13:50:01.000000 brainways-0.1.5/.pre-commit-config.yaml
+-rw-rw-r--   0 ben       (1001) ben       (1001)      681 2022-07-13 13:47:58.000000 brainways-0.1.5/.travis.yml
+-rw-rw-r--   0 ben       (1001) ben       (1001)      160 2022-07-13 13:47:58.000000 brainways-0.1.5/AUTHORS.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)     3523 2022-07-13 13:47:58.000000 brainways-0.1.5/CONTRIBUTING.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)       89 2022-07-13 13:47:58.000000 brainways-0.1.5/HISTORY.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)    35148 2022-08-24 08:26:24.000000 brainways-0.1.5/LICENSE
+-rw-rw-r--   0 ben       (1001) ben       (1001)      262 2022-07-13 13:47:58.000000 brainways-0.1.5/MANIFEST.in
+-rw-rw-r--   0 ben       (1001) ben       (1001)     2430 2023-05-26 08:21:13.000000 brainways-0.1.5/Makefile
+-rw-rw-r--   0 ben       (1001) ben       (1001)     2343 2023-06-09 09:31:57.298109 brainways-0.1.5/PKG-INFO
+-rw-rw-r--   0 ben       (1001) ben       (1001)      962 2023-05-26 08:25:05.000000 brainways-0.1.5/README.rst
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-09 09:31:57.282109 brainways-0.1.5/data/
+-rw-rw-r--   0 ben       (1001) ben       (1001)   269441 2022-03-11 09:30:01.000000 brainways-0.1.5/data/test_data.npz
+-rw-rw-r--   0 ben       (1001) ben       (1001)    47973 2022-06-30 11:17:43.000000 brainways-0.1.5/data/test_image.jpg
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-09 09:31:57.286109 brainways-0.1.5/docs/
+-rw-rw-r--   0 ben       (1001) ben       (1001)      610 2022-07-13 13:47:58.000000 brainways-0.1.5/docs/Makefile
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-09 09:31:57.278109 brainways-0.1.5/docs/_build/
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-09 09:31:57.278109 brainways-0.1.5/docs/_build/html/
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-09 09:31:57.286109 brainways-0.1.5/docs/_build/html/_static/
+-rw-rw-r--   0 ben       (1001) ben       (1001)      286 2022-10-06 11:03:00.000000 brainways-0.1.5/docs/_build/html/_static/file.png
+-rw-rw-r--   0 ben       (1001) ben       (1001)       90 2022-10-06 11:03:00.000000 brainways-0.1.5/docs/_build/html/_static/minus.png
+-rw-rw-r--   0 ben       (1001) ben       (1001)       90 2022-10-06 11:03:00.000000 brainways-0.1.5/docs/_build/html/_static/plus.png
+-rw-rw-r--   0 ben       (1001) ben       (1001)       28 2022-07-13 13:47:58.000000 brainways-0.1.5/docs/authors.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)      361 2023-05-26 08:18:55.000000 brainways-0.1.5/docs/brainways.elastix.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1317 2023-05-26 08:18:55.000000 brainways-0.1.5/docs/brainways.pipeline.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)      770 2023-05-26 08:18:55.000000 brainways-0.1.5/docs/brainways.project.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)      500 2023-05-26 08:26:43.000000 brainways-0.1.5/docs/brainways.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)     2137 2023-05-26 08:18:55.000000 brainways-0.1.5/docs/brainways.scripts.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1387 2023-05-26 08:18:55.000000 brainways-0.1.5/docs/brainways.transforms.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)      601 2023-05-26 08:18:55.000000 brainways-0.1.5/docs/brainways.utils.atlas.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1405 2023-05-26 08:18:55.000000 brainways-0.1.5/docs/brainways.utils.cell_detection_importer.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)      386 2023-05-26 08:18:55.000000 brainways-0.1.5/docs/brainways.utils.czi.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)      971 2023-05-26 08:18:55.000000 brainways-0.1.5/docs/brainways.utils.io_utils.file_iterators.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1145 2023-05-26 08:18:55.000000 brainways-0.1.5/docs/brainways.utils.io_utils.readers.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)      553 2023-05-26 08:18:55.000000 brainways-0.1.5/docs/brainways.utils.io_utils.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1833 2023-05-26 08:18:55.000000 brainways-0.1.5/docs/brainways.utils.rst
+-rwxrwxr-x   0 ben       (1001) ben       (1001)     4967 2023-05-26 08:17:55.000000 brainways-0.1.5/docs/conf.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)       33 2022-07-13 13:47:58.000000 brainways-0.1.5/docs/contributing.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)       28 2022-07-13 13:47:58.000000 brainways-0.1.5/docs/history.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)      306 2022-07-13 13:47:58.000000 brainways-0.1.5/docs/index.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1118 2022-07-13 13:47:58.000000 brainways-0.1.5/docs/installation.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)      807 2022-07-13 13:47:58.000000 brainways-0.1.5/docs/make.bat
+-rw-rw-r--   0 ben       (1001) ben       (1001)       64 2023-05-26 08:26:43.000000 brainways-0.1.5/docs/modules.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)       27 2022-07-13 13:47:58.000000 brainways-0.1.5/docs/readme.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)       73 2022-07-13 13:47:58.000000 brainways-0.1.5/docs/usage.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)      383 2023-05-26 08:03:19.000000 brainways-0.1.5/pyproject.toml
+-rw-rw-r--   0 ben       (1001) ben       (1001)      165 2022-07-13 14:08:33.000000 brainways-0.1.5/requirements_dev.txt
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1967 2023-06-09 09:31:57.298109 brainways-0.1.5/setup.cfg
+-rw-rw-r--   0 ben       (1001) ben       (1001)       60 2023-05-26 07:59:05.000000 brainways-0.1.5/setup.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-09 09:31:57.278109 brainways-0.1.5/src/
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-09 09:31:57.286109 brainways-0.1.5/src/brainways/
+-rw-rw-r--   0 ben       (1001) ben       (1001)        0 2022-07-13 14:28:10.000000 brainways-0.1.5/src/brainways/__init__.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)      160 2023-06-09 09:31:57.000000 brainways-0.1.5/src/brainways/_version.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     7423 2023-06-09 09:30:50.000000 brainways-0.1.5/src/brainways/conftest.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-09 09:31:57.286109 brainways-0.1.5/src/brainways/elastix/
+-rw-rw-r--   0 ben       (1001) ben       (1001)     2596 2022-07-14 13:40:58.000000 brainways-0.1.5/src/brainways/elastix/Par0033bspline.txt
+-rw-rw-r--   0 ben       (1001) ben       (1001)     2316 2022-07-14 13:40:58.000000 brainways-0.1.5/src/brainways/elastix/Par0033similarity.txt
+-rw-rw-r--   0 ben       (1001) ben       (1001)        0 2021-12-09 12:20:50.000000 brainways-0.1.5/src/brainways/elastix/__init__.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-09 09:31:57.286109 brainways-0.1.5/src/brainways/elastix/_tests/
+-rw-rw-r--   0 ben       (1001) ben       (1001)      592 2022-10-27 09:03:02.000000 brainways-0.1.5/src/brainways/elastix/_tests/test_elastix.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     2649 2022-09-08 14:32:33.000000 brainways-0.1.5/src/brainways/elastix/elastix.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-09 09:31:57.286109 brainways-0.1.5/src/brainways/pipeline/
+-rw-rw-r--   0 ben       (1001) ben       (1001)        0 2022-07-07 09:39:04.000000 brainways-0.1.5/src/brainways/pipeline/__init__.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-09 09:31:57.286109 brainways-0.1.5/src/brainways/pipeline/_tests/
+-rw-rw-r--   0 ben       (1001) ben       (1001)      430 2022-10-27 09:03:02.000000 brainways-0.1.5/src/brainways/pipeline/_tests/test_atlas_registration.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)      552 2022-11-23 11:34:52.000000 brainways-0.1.5/src/brainways/pipeline/_tests/test_brainways_pipeline.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)      370 2023-06-09 09:30:50.000000 brainways-0.1.5/src/brainways/pipeline/_tests/test_cell_detector.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1097 2022-11-30 13:23:46.000000 brainways-0.1.5/src/brainways/pipeline/affine_2d.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     2339 2023-05-24 12:27:57.000000 brainways-0.1.5/src/brainways/pipeline/atlas_registration.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1165 2023-06-07 14:11:19.000000 brainways-0.1.5/src/brainways/pipeline/brainways_params.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     3712 2022-11-30 13:35:53.000000 brainways-0.1.5/src/brainways/pipeline/brainways_pipeline.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     5186 2023-06-09 09:29:12.000000 brainways-0.1.5/src/brainways/pipeline/cell_detector.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1596 2022-11-30 13:25:23.000000 brainways-0.1.5/src/brainways/pipeline/tps.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-09 09:31:57.290109 brainways-0.1.5/src/brainways/project/
+-rw-rw-r--   0 ben       (1001) ben       (1001)        0 2022-07-07 09:39:04.000000 brainways-0.1.5/src/brainways/project/__init__.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-09 09:31:57.290109 brainways-0.1.5/src/brainways/project/_tests/
+-rw-rw-r--   0 ben       (1001) ben       (1001)        0 2022-07-14 12:32:42.000000 brainways-0.1.5/src/brainways/project/_tests/__init__.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     2139 2023-06-09 09:23:33.000000 brainways-0.1.5/src/brainways/project/_tests/conftest.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     3207 2023-06-09 09:25:09.000000 brainways-0.1.5/src/brainways/project/_tests/test_brainways_project.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     8662 2023-06-09 09:09:06.000000 brainways-0.1.5/src/brainways/project/_tests/test_brainways_subject.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-09 09:31:57.278109 brainways-0.1.5/src/brainways/project/_tests/test_projects/
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-09 09:31:57.290109 brainways-0.1.5/src/brainways/project/_tests/test_projects/v0.1.1/
+-rw-rw-r--   0 ben       (1001) ben       (1001)       38 2023-06-07 15:59:39.000000 brainways-0.1.5/src/brainways/project/_tests/test_projects/v0.1.1/project.bwp
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-09 09:31:57.290109 brainways-0.1.5/src/brainways/project/_tests/test_projects/v0.1.1/subject1/
+-rw-rw-r--   0 ben       (1001) ben       (1001)     2016 2023-06-09 09:23:59.000000 brainways-0.1.5/src/brainways/project/_tests/test_projects/v0.1.1/subject1/brainways.bin
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-09 09:31:57.290109 brainways-0.1.5/src/brainways/project/_tests/test_projects/v0.1.4/
+-rw-rw-r--   0 ben       (1001) ben       (1001)      153 2023-06-09 09:30:50.000000 brainways-0.1.5/src/brainways/project/_tests/test_projects/v0.1.4/project.bwp
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-09 09:31:57.290109 brainways-0.1.5/src/brainways/project/_tests/test_projects/v0.1.4/subject1/
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1902 2023-06-09 09:25:14.000000 brainways-0.1.5/src/brainways/project/_tests/test_projects/v0.1.4/subject1/brainways.bin
+-rw-rw-r--   0 ben       (1001) ben       (1001)      697 2023-06-09 08:13:53.000000 brainways-0.1.5/src/brainways/project/_tests/test_utils.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     2428 2023-06-09 09:30:50.000000 brainways-0.1.5/src/brainways/project/_utils.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     8792 2023-06-07 15:29:27.000000 brainways-0.1.5/src/brainways/project/brainways_project.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)    18570 2023-06-09 09:06:00.000000 brainways-0.1.5/src/brainways/project/brainways_subject.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1388 2023-06-07 15:59:32.000000 brainways-0.1.5/src/brainways/project/info_classes.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-09 09:31:57.290109 brainways-0.1.5/src/brainways/scripts/
+-rw-rw-r--   0 ben       (1001) ben       (1001)        0 2022-07-14 12:32:42.000000 brainways-0.1.5/src/brainways/scripts/__init__.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-09 09:31:57.290109 brainways-0.1.5/src/brainways/scripts/_tests/
+-rw-rw-r--   0 ben       (1001) ben       (1001)      920 2023-05-26 08:21:13.000000 brainways-0.1.5/src/brainways/scripts/_tests/test_cli.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     3031 2022-09-08 14:06:58.000000 brainways-0.1.5/src/brainways/scripts/batch_create_thumbnails.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     3053 2023-05-07 14:18:30.000000 brainways-0.1.5/src/brainways/scripts/cell_detection.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1142 2023-05-04 08:18:52.000000 brainways-0.1.5/src/brainways/scripts/cli.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1588 2023-05-07 14:18:29.000000 brainways-0.1.5/src/brainways/scripts/create_excel.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     4944 2022-11-30 14:10:59.000000 brainways-0.1.5/src/brainways/scripts/create_excel_colabelling.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     4023 2022-11-23 12:26:10.000000 brainways-0.1.5/src/brainways/scripts/create_reg_model_data.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     5253 2022-11-23 12:35:34.000000 brainways-0.1.5/src/brainways/scripts/display_area.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1618 2022-12-08 14:20:04.000000 brainways-0.1.5/src/brainways/scripts/import_cell_detections_keren.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1192 2022-11-23 12:26:10.000000 brainways-0.1.5/src/brainways/scripts/import_cells.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)      920 2022-12-11 10:14:02.000000 brainways-0.1.5/src/brainways/scripts/move_images.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-09 09:31:57.290109 brainways-0.1.5/src/brainways/transforms/
+-rw-rw-r--   0 ben       (1001) ben       (1001)        0 2022-04-27 09:13:34.000000 brainways-0.1.5/src/brainways/transforms/__init__.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-09 09:31:57.294109 brainways-0.1.5/src/brainways/transforms/_tests/
+-rw-rw-r--   0 ben       (1001) ben       (1001)        0 2022-04-27 09:13:34.000000 brainways-0.1.5/src/brainways/transforms/_tests/__init__.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     2173 2022-07-14 13:48:40.000000 brainways-0.1.5/src/brainways/transforms/_tests/test_affine_transform_2d.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1813 2022-11-23 11:35:37.000000 brainways-0.1.5/src/brainways/transforms/_tests/test_depth_registration.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     2034 2022-07-14 13:48:40.000000 brainways-0.1.5/src/brainways/transforms/_tests/test_image_to_atlas_transform.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     2667 2022-07-14 13:48:40.000000 brainways-0.1.5/src/brainways/transforms/_tests/test_tps_transform.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     4104 2022-11-30 13:34:33.000000 brainways-0.1.5/src/brainways/transforms/affine_transform_2d.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)      436 2022-07-14 12:46:19.000000 brainways-0.1.5/src/brainways/transforms/base.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)      623 2022-07-14 13:40:58.000000 brainways-0.1.5/src/brainways/transforms/compose.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     2594 2022-07-14 13:48:40.000000 brainways-0.1.5/src/brainways/transforms/depth_registration.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     2205 2022-09-08 13:13:42.000000 brainways-0.1.5/src/brainways/transforms/image_to_atlas_transform.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     2185 2022-11-30 13:46:38.000000 brainways-0.1.5/src/brainways/transforms/tps_transform.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-09 09:31:57.294109 brainways-0.1.5/src/brainways/utils/
+-rw-rw-r--   0 ben       (1001) ben       (1001)        0 2021-07-21 08:14:53.000000 brainways-0.1.5/src/brainways/utils/__init__.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1674 2022-07-17 07:51:20.000000 brainways-0.1.5/src/brainways/utils/_imports.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-09 09:31:57.294109 brainways-0.1.5/src/brainways/utils/_tests/
+-rw-rw-r--   0 ben       (1001) ben       (1001)        0 2022-07-14 12:32:42.000000 brainways-0.1.5/src/brainways/utils/_tests/__init__.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     7710 2023-05-26 08:21:13.000000 brainways-0.1.5/src/brainways/utils/_tests/test_cell_count_summary.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     2715 2023-05-07 14:18:30.000000 brainways-0.1.5/src/brainways/utils/_tests/test_cells.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     2412 2022-07-14 13:48:40.000000 brainways-0.1.5/src/brainways/utils/_tests/test_image.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-09 09:31:57.294109 brainways-0.1.5/src/brainways/utils/atlas/
+-rw-rw-r--   0 ben       (1001) ben       (1001)        0 2021-07-21 11:07:35.000000 brainways-0.1.5/src/brainways/utils/atlas/__init__.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-09 09:31:57.294109 brainways-0.1.5/src/brainways/utils/atlas/_tests/
+-rw-rw-r--   0 ben       (1001) ben       (1001)        0 2022-04-27 09:13:34.000000 brainways-0.1.5/src/brainways/utils/atlas/_tests/__init__.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     3708 2022-07-14 13:40:59.000000 brainways-0.1.5/src/brainways/utils/atlas/_tests/test_slice_atlas.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     4263 2022-12-11 16:13:39.000000 brainways-0.1.5/src/brainways/utils/atlas/brainways_atlas.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     2280 2023-05-04 09:01:16.000000 brainways-0.1.5/src/brainways/utils/atlas/slice_atlas.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     5751 2023-05-14 15:00:03.000000 brainways-0.1.5/src/brainways/utils/cell_count_summary.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-09 09:31:57.294109 brainways-0.1.5/src/brainways/utils/cell_detection_importer/
+-rw-rw-r--   0 ben       (1001) ben       (1001)        0 2022-10-06 09:31:17.000000 brainways-0.1.5/src/brainways/utils/cell_detection_importer/__init__.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-09 09:31:57.294109 brainways-0.1.5/src/brainways/utils/cell_detection_importer/_tests/
+-rw-rw-r--   0 ben       (1001) ben       (1001)     7465 2022-10-06 10:12:40.000000 brainways-0.1.5/src/brainways/utils/cell_detection_importer/_tests/qupath_sample_file.txt
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1240 2022-11-23 12:23:47.000000 brainways-0.1.5/src/brainways/utils/cell_detection_importer/_tests/test_brainways_cell_detection_importer.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1722 2022-12-08 14:20:04.000000 brainways-0.1.5/src/brainways/utils/cell_detection_importer/_tests/test_qupath_cell_detection_importer.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1343 2022-11-23 12:26:10.000000 brainways-0.1.5/src/brainways/utils/cell_detection_importer/brainways_cell_detection_importer.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)      507 2022-11-27 15:04:03.000000 brainways-0.1.5/src/brainways/utils/cell_detection_importer/cell_detection_importer.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     2438 2022-12-11 10:33:01.000000 brainways-0.1.5/src/brainways/utils/cell_detection_importer/keren_cell_detection_importer.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)      731 2022-12-08 14:20:04.000000 brainways-0.1.5/src/brainways/utils/cell_detection_importer/utils.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     4985 2023-05-02 09:29:03.000000 brainways-0.1.5/src/brainways/utils/cells.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     4270 2022-09-11 13:34:36.000000 brainways-0.1.5/src/brainways/utils/config.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-09 09:31:57.294109 brainways-0.1.5/src/brainways/utils/czi/
+-rw-rw-r--   0 ben       (1001) ben       (1001)        0 2021-07-15 08:31:32.000000 brainways-0.1.5/src/brainways/utils/czi/__init__.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1112 2022-07-14 13:48:40.000000 brainways-0.1.5/src/brainways/utils/czi/czi_to_jpg.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)      793 2022-07-14 12:49:34.000000 brainways-0.1.5/src/brainways/utils/dataclasses.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     9025 2023-05-26 13:51:47.000000 brainways-0.1.5/src/brainways/utils/image.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-09 09:31:57.298109 brainways-0.1.5/src/brainways/utils/io_utils/
+-rw-rw-r--   0 ben       (1001) ben       (1001)       42 2022-07-17 07:44:03.000000 brainways-0.1.5/src/brainways/utils/io_utils/__init__.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-09 09:31:57.298109 brainways-0.1.5/src/brainways/utils/io_utils/file_iterators/
+-rw-rw-r--   0 ben       (1001) ben       (1001)      379 2022-09-08 08:38:22.000000 brainways-0.1.5/src/brainways/utils/io_utils/file_iterators/__init__.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)      230 2022-07-07 09:39:04.000000 brainways-0.1.5/src/brainways/utils/io_utils/file_iterators/image_entry.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)      407 2022-07-07 09:39:04.000000 brainways-0.1.5/src/brainways/utils/io_utils/file_iterators/path.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)      914 2022-11-23 12:29:43.000000 brainways-0.1.5/src/brainways/utils/io_utils/file_iterators/qupath.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)      630 2022-07-07 09:39:09.000000 brainways-0.1.5/src/brainways/utils/io_utils/image_path.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-09 09:31:57.298109 brainways-0.1.5/src/brainways/utils/io_utils/readers/
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1041 2022-09-11 12:16:49.000000 brainways-0.1.5/src/brainways/utils/io_utils/readers/__init__.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-09 09:31:57.298109 brainways-0.1.5/src/brainways/utils/io_utils/readers/_tests/
+-rw-rw-r--   0 ben       (1001) ben       (1001)      218 2022-09-22 07:42:16.000000 brainways-0.1.5/src/brainways/utils/io_utils/readers/_tests/test_qupath_reader.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1419 2022-09-08 08:38:21.000000 brainways-0.1.5/src/brainways/utils/io_utils/readers/aicsimageio_reader.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)      649 2022-07-14 12:39:58.000000 brainways-0.1.5/src/brainways/utils/io_utils/readers/base.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1364 2022-09-08 08:38:21.000000 brainways-0.1.5/src/brainways/utils/io_utils/readers/czi_reader.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)    15748 2023-05-21 10:26:48.000000 brainways-0.1.5/src/brainways/utils/io_utils/readers/qupath_reader.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)      108 2022-09-11 13:34:36.000000 brainways-0.1.5/src/brainways/utils/paths.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1181 2022-07-14 13:48:40.000000 brainways-0.1.5/src/brainways/utils/preprocess.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     3183 2022-09-11 10:47:30.000000 brainways-0.1.5/src/brainways/utils/qupath.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1083 2022-07-14 13:48:39.000000 brainways-0.1.5/src/brainways/utils/test_utils.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-09 09:31:57.286109 brainways-0.1.5/src/brainways.egg-info/
+-rw-rw-r--   0 ben       (1001) ben       (1001)     2343 2023-06-09 09:31:57.000000 brainways-0.1.5/src/brainways.egg-info/PKG-INFO
+-rw-rw-r--   0 ben       (1001) ben       (1001)     5729 2023-06-09 09:31:57.000000 brainways-0.1.5/src/brainways.egg-info/SOURCES.txt
+-rw-rw-r--   0 ben       (1001) ben       (1001)        1 2023-06-09 09:31:57.000000 brainways-0.1.5/src/brainways.egg-info/dependency_links.txt
+-rw-rw-r--   0 ben       (1001) ben       (1001)       57 2023-06-09 09:31:57.000000 brainways-0.1.5/src/brainways.egg-info/entry_points.txt
+-rw-rw-r--   0 ben       (1001) ben       (1001)      413 2023-06-09 09:31:57.000000 brainways-0.1.5/src/brainways.egg-info/requires.txt
+-rw-rw-r--   0 ben       (1001) ben       (1001)       10 2023-06-09 09:31:57.000000 brainways-0.1.5/src/brainways.egg-info/top_level.txt
+-rw-rw-r--   0 ben       (1001) ben       (1001)      540 2022-07-13 13:47:58.000000 brainways-0.1.5/tox.ini
```

### Comparing `brainways-0.1.4/.gitignore` & `brainways-0.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `brainways-0.1.4/.pre-commit-config.yaml` & `brainways-0.1.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `brainways-0.1.4/.travis.yml` & `brainways-0.1.5/.travis.yml`

 * *Files identical despite different names*

### Comparing `brainways-0.1.4/CONTRIBUTING.rst` & `brainways-0.1.5/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `brainways-0.1.4/LICENSE` & `brainways-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `brainways-0.1.4/Makefile` & `brainways-0.1.5/Makefile`

 * *Files identical despite different names*

### Comparing `brainways-0.1.4/PKG-INFO` & `brainways-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brainways
-Version: 0.1.4
+Version: 0.1.5
 Summary: Brainways
 Home-page: https://github.com/bkntr/brainways
 Author: Ben Kantor
 Author-email: benkantor@mail.tau.ac.il
 License: GPL-3.0
 Project-URL: Bug Tracker, https://github.com/bkntr/brainways/issues
 Project-URL: Documentation, https://github.com/bkntr/brainways#README.md
```

### Comparing `brainways-0.1.4/README.rst` & `brainways-0.1.5/README.rst`

 * *Files identical despite different names*

### Comparing `brainways-0.1.4/data/test_data.npz` & `brainways-0.1.5/data/test_data.npz`

 * *Files identical despite different names*

### Comparing `brainways-0.1.4/data/test_image.jpg` & `brainways-0.1.5/data/test_image.jpg`

 * *Files identical despite different names*

### Comparing `brainways-0.1.4/docs/Makefile` & `brainways-0.1.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `brainways-0.1.4/docs/brainways.pipeline.rst` & `brainways-0.1.5/docs/brainways.pipeline.rst`

 * *Files identical despite different names*

### Comparing `brainways-0.1.4/docs/brainways.project.rst` & `brainways-0.1.5/docs/brainways.project.rst`

 * *Files identical despite different names*

### Comparing `brainways-0.1.4/docs/brainways.scripts.rst` & `brainways-0.1.5/docs/brainways.scripts.rst`

 * *Files identical despite different names*

### Comparing `brainways-0.1.4/docs/brainways.transforms.rst` & `brainways-0.1.5/docs/brainways.transforms.rst`

 * *Files identical despite different names*

### Comparing `brainways-0.1.4/docs/brainways.utils.atlas.rst` & `brainways-0.1.5/docs/brainways.utils.atlas.rst`

 * *Files identical despite different names*

### Comparing `brainways-0.1.4/docs/brainways.utils.cell_detection_importer.rst` & `brainways-0.1.5/docs/brainways.utils.cell_detection_importer.rst`

 * *Files identical despite different names*

### Comparing `brainways-0.1.4/docs/brainways.utils.io_utils.file_iterators.rst` & `brainways-0.1.5/docs/brainways.utils.io_utils.file_iterators.rst`

 * *Files identical despite different names*

### Comparing `brainways-0.1.4/docs/brainways.utils.io_utils.readers.rst` & `brainways-0.1.5/docs/brainways.utils.io_utils.readers.rst`

 * *Files identical despite different names*

### Comparing `brainways-0.1.4/docs/brainways.utils.io_utils.rst` & `brainways-0.1.5/docs/brainways.utils.io_utils.rst`

 * *Files identical despite different names*

### Comparing `brainways-0.1.4/docs/brainways.utils.rst` & `brainways-0.1.5/docs/brainways.utils.rst`

 * *Files identical despite different names*

### Comparing `brainways-0.1.4/docs/conf.py` & `brainways-0.1.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.4/docs/installation.rst` & `brainways-0.1.5/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `brainways-0.1.4/docs/make.bat` & `brainways-0.1.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `brainways-0.1.4/setup.cfg` & `brainways-0.1.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `brainways-0.1.4/src/brainways/conftest.py` & `brainways-0.1.5/src/brainways/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from pathlib import Path
 from typing import List, Tuple
 from unittest.mock import Mock, create_autospec, patch
 
 import numpy as np
 import pytest
 import torch
+from aicsimageio.types import PhysicalPixelSizes
 from bg_atlasapi.structure_class import StructuresDict
 from PIL import Image
 from pytest import fixture
 
 from brainways.pipeline.brainways_params import (
     AffineTransform2DParams,
     AtlasRegistrationParams,
@@ -22,14 +23,15 @@
 )
 from brainways.project.brainways_subject import BrainwaysSubject
 from brainways.project.info_classes import ProjectSettings, SliceInfo
 from brainways.utils.atlas.brainways_atlas import AtlasSlice, BrainwaysAtlas
 from brainways.utils.image import ImageSizeHW
 from brainways.utils.io_utils import ImagePath
 from brainways.utils.io_utils.readers.base import ImageReader
+from brainways.utils.io_utils.readers.qupath_reader import QupathReader
 
 
 @fixture(autouse=True)
 def seed():
     np.random.seed(0)
 
 
@@ -125,14 +127,15 @@
 
 
 @pytest.fixture
 def mock_image_path(test_data: Tuple[np.ndarray, AtlasSlice], tmpdir) -> ImagePath:
     image, _ = test_data
     image_path = ImagePath(str(tmpdir / "image.jpg"), scene=0)
     Image.fromarray(image).save(image_path.filename)
+    QupathReader.physical_pixel_sizes = PhysicalPixelSizes(Z=None, Y=10.0, X=10.0)
     return image_path
 
 
 @pytest.fixture
 def mock_subject_documents(
     mock_image_path: ImagePath, test_data: Tuple[np.ndarray, AtlasSlice]
 ) -> List[SliceInfo]:
@@ -165,14 +168,15 @@
         documents.append(
             SliceInfo(
                 path=doc_image_path,
                 image_size=(image_height, image_width),
                 lowres_image_size=(image_height, image_width),
                 params=params,
                 ignore=i == 0,
+                physical_pixel_sizes=(10.0, 10.0),
             )
         )
     return documents
 
 
 @pytest.fixture
 def mock_project_settings() -> ProjectSettings:
```

### Comparing `brainways-0.1.4/src/brainways/elastix/Par0033bspline.txt` & `brainways-0.1.5/src/brainways/elastix/Par0033bspline.txt`

 * *Files identical despite different names*

### Comparing `brainways-0.1.4/src/brainways/elastix/Par0033similarity.txt` & `brainways-0.1.5/src/brainways/elastix/Par0033similarity.txt`

 * *Files identical despite different names*

### Comparing `brainways-0.1.4/src/brainways/elastix/_tests/test_elastix.py` & `brainways-0.1.5/src/brainways/elastix/_tests/test_elastix.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.4/src/brainways/elastix/elastix.py` & `brainways-0.1.5/src/brainways/elastix/elastix.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.4/src/brainways/pipeline/_tests/test_brainways_pipeline.py` & `brainways-0.1.5/src/brainways/pipeline/_tests/test_brainways_pipeline.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.4/src/brainways/pipeline/affine_2d.py` & `brainways-0.1.5/src/brainways/pipeline/affine_2d.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.4/src/brainways/pipeline/atlas_registration.py` & `brainways-0.1.5/src/brainways/pipeline/atlas_registration.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.4/src/brainways/pipeline/brainways_params.py` & `brainways-0.1.5/src/brainways/pipeline/brainways_params.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.4/src/brainways/pipeline/brainways_pipeline.py` & `brainways-0.1.5/src/brainways/pipeline/brainways_pipeline.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.4/src/brainways/pipeline/cell_detector.py` & `brainways-0.1.5/src/brainways/pipeline/cell_detector.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.4/src/brainways/pipeline/tps.py` & `brainways-0.1.5/src/brainways/pipeline/tps.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.4/src/brainways/project/_tests/test_brainways_project.py` & `brainways-0.1.5/src/brainways/project/_tests/test_brainways_project.py`

 * *Files 16% similar despite different names*

```diff
@@ -68,7 +68,25 @@
         project.subjects[0].documents[0].params.atlas
         == mock_subject_documents[0].params.atlas
     )
     assert (
         project.subjects[0].documents[0].params.affine
         == mock_subject_documents[0].params.affine
     )
+
+
+def test_open_brainways_project_v0_1_4(
+    brainways_project_path_v0_1_4: Path,
+    mock_project_settings: ProjectSettings,
+    mock_subject_documents: List[SliceInfo],
+):
+    project = BrainwaysProject.open(brainways_project_path_v0_1_4, lazy_init=True)
+    assert project.settings.atlas == mock_project_settings.atlas
+    assert len(project.subjects) == 1
+    assert (
+        project.subjects[0].documents[0].params.atlas
+        == mock_subject_documents[0].params.atlas
+    )
+    assert (
+        project.subjects[0].documents[0].params.affine
+        == mock_subject_documents[0].params.affine
+    )
```

### Comparing `brainways-0.1.4/src/brainways/project/_tests/test_brainways_subject.py` & `brainways-0.1.5/src/brainways/project/_tests/test_brainways_subject.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,14 +111,15 @@
 ):
     image, _ = test_data
     brainways_subject.add_image(path=mock_image_path)
     expected_document = SliceInfo(
         path=mock_image_path,
         image_size=image.shape,
         lowres_image_size=(788, 1024),
+        physical_pixel_sizes=(10.0, 10.0),
     )
     assert brainways_subject.documents[-1] == expected_document
 
 
 def test_add_image_saves_lowres_image(
     brainways_subject: BrainwaysSubject,
     test_data: Tuple[np.ndarray, AtlasSlice],
```

### Comparing `brainways-0.1.4/src/brainways/project/_tests/test_projects/v0.1.1/subject1/brainways.bin` & `brainways-0.1.5/src/brainways/project/_tests/test_projects/v0.1.1/subject1/brainways.bin`

 * *Files 12% similar despite different names*

```diff
@@ -1,135 +1,126 @@
-00000000: 8004 9560 0800 0000 0000 007d 9428 8c05  ...`.......}.(..
+00000000: 8004 95d5 0700 0000 0000 007d 9428 8c05  ...........}.(..
 00000010: 6174 6c61 7394 8c0a 4d4f 434b 5f41 544c  atlas...MOCK_ATL
 00000020: 4153 948c 0763 6861 6e6e 656c 944b 0075  AS...channel.K.u
 00000030: 5d94 287d 9428 8c04 7061 7468 947d 9428  ].(}.(..path.}.(
-00000040: 8c08 6669 6c65 6e61 6d65 948c 452f 746d  ..filename..E/tm
+00000040: 8c08 6669 6c65 6e61 6d65 948c 462f 746d  ..filename..F/tm
 00000050: 702f 7079 7465 7374 2d6f 662d 6265 6e2f  p/pytest-of-ben/
-00000060: 7079 7465 7374 2d33 352f 7465 7374 5f6f  pytest-35/test_o
-00000070: 7065 6e5f 6272 6169 6e77 6179 735f 7072  pen_brainways_pr
-00000080: 6f6a 6563 7430 2f69 6d61 6765 5f30 2e6a  oject0/image_0.j
-00000090: 7067 948c 0573 6365 6e65 944b 0068 034e  pg...scene.K.h.N
-000000a0: 758c 0a69 6d61 6765 5f73 697a 6594 4d8a  u..image_size.M.
-000000b0: 014d 0002 8694 8c11 6c6f 7772 6573 5f69  .M......lowres_i
-000000c0: 6d61 6765 5f73 697a 6594 4d8a 014d 0002  mage_size.M..M..
-000000d0: 8694 8c06 7061 7261 6d73 947d 9428 6801  ....params.}.(h.
-000000e0: 7d94 288c 0261 7094 4b05 8c0b 726f 745f  }.(..ap.K...rot_
-000000f0: 6672 6f6e 7461 6c94 4700 0000 0000 0000  frontal.G.......
-00000100: 008c 0e72 6f74 5f68 6f72 697a 6f6e 7461  ...rot_horizonta
-00000110: 6c94 4700 0000 0000 0000 008c 0c72 6f74  l.G..........rot
-00000120: 5f73 6167 6974 7461 6c94 4700 0000 0000  _sagittal.G.....
-00000130: 0000 008c 0a68 656d 6973 7068 6572 6594  .....hemisphere.
-00000140: 8c04 626f 7468 948c 0a63 6f6e 6669 6465  ..both...confide
-00000150: 6e63 6594 473f f000 0000 0000 0075 8c06  nce.G?.......u..
-00000160: 6166 6669 6e65 947d 9428 8c05 616e 676c  affine.}.(..angl
-00000170: 6594 4700 0000 0000 0000 008c 0274 7894  e.G..........tx.
-00000180: 4700 0000 0000 0000 008c 0274 7994 4700  G..........ty.G.
-00000190: 0000 0000 0000 008c 0273 7894 473f f000  .........sx.G?..
-000001a0: 0000 0000 008c 0273 7994 473f f000 0000  .......sy.G?....
-000001b0: 0000 008c 0263 7894 4e8c 0263 7994 4e75  .....cx.N..cy.Nu
-000001c0: 8c03 7470 7394 7d94 288c 0a70 6f69 6e74  ..tps.}.(..point
-000001d0: 735f 7372 6394 8c15 6e75 6d70 792e 636f  s_src...numpy.co
-000001e0: 7265 2e6d 756c 7469 6172 7261 7994 8c0c  re.multiarray...
-000001f0: 5f72 6563 6f6e 7374 7275 6374 9493 948c  _reconstruct....
-00000200: 056e 756d 7079 948c 076e 6461 7272 6179  .numpy...ndarray
-00000210: 9493 944b 0085 9443 0162 9487 9452 9428  ...K...C.b...R.(
-00000220: 4b01 4b0a 4b02 8694 6828 8c05 6474 7970  K.K.K...h(..dtyp
-00000230: 6594 9394 8c02 6634 9489 8887 9452 9428  e.....f4.....R.(
-00000240: 4b03 8c01 3c94 4e4e 4e4a ffff ffff 4aff  K...<.NNNJ....J.
-00000250: ffff ff4b 0074 9462 8943 500b 7f8c 436e  ...K.t.b.CP...Cn
-00000260: e48c 43b3 4e9a 4319 af56 4348 e958 4377  ..C.N.C..VCH.XCw
-00000270: 7b7e 436e 0b60 43e5 adaf 439a b2f6 4372  {~Cn.`C...C...Cr
-00000280: 1317 437e aeca 4375 6250 435e 6b91 43b1  ..C~..CubPC^k.C.
-00000290: 57b6 435a 7b11 42d7 5009 420d a125 41af  W.CZ{.B.P.B..%A.
-000002a0: 06a4 4348 35c7 4374 64ab 4394 7494 628c  ..CH5.Ctd.C.t.b.
-000002b0: 0a70 6f69 6e74 735f 6473 7494 6827 682a  .points_dst.h'h*
-000002c0: 4b00 8594 682c 8794 5294 284b 014b 0a4b  K...h,..R.(K.K.K
-000002d0: 0286 9468 3489 4350 0b7f 8c43 6ee4 8c43  ...h4.CP...Cn..C
-000002e0: b34e 9a43 19af 5643 48e9 5843 777b 7e43  .N.C..VCH.XCw{~C
-000002f0: 6e0b 6043 e5ad af43 9ab2 f643 7213 1743  n.`C...C...Cr..C
-00000300: 7eae ca43 7562 5043 5e6b 9143 b157 b643  ~..CubPC^k.C.W.C
-00000310: 5a7b 1142 d750 0942 0da1 2541 af06 a443  Z{.B.P.B..%A...C
-00000320: 4835 c743 7464 ab43 9474 9462 758c 0463  H5.Ctd.C.t.bu..c
-00000330: 656c 6c94 7d94 288c 0864 6961 6d65 7465  ell.}.(..diamete
-00000340: 7294 473f f000 0000 0000 008c 076e 6574  r.G?.........net
-00000350: 5f61 7667 9488 8c0e 666c 6f77 5f74 6872  _avg....flow_thr
-00000360: 6573 686f 6c64 9447 3ff0 0000 0000 0000  eshold.G?.......
-00000370: 8c0e 6d61 736b 5f74 6872 6573 686f 6c64  ..mask_threshold
-00000380: 9447 3ff0 0000 0000 0000 8c0a 7072 6576  .G?.........prev
-00000390: 6965 775f 6262 9428 4700 0000 0000 0000  iew_bb.(G.......
-000003a0: 0047 0000 0000 0000 0000 473f f000 0000  .G........G?....
-000003b0: 0000 0047 3ff0 0000 0000 0000 7494 7575  ...G?.......t.uu
-000003c0: 8c06 6967 6e6f 7265 9488 8c14 7068 7973  ..ignore....phys
-000003d0: 6963 616c 5f70 6978 656c 5f73 697a 6573  ical_pixel_sizes
-000003e0: 944e 8c07 7665 7273 696f 6e94 8c05 302e  .N..version...0.
-000003f0: 312e 3194 757d 9428 6806 7d94 2868 088c  1.1.u}.(h.}.(h..
-00000400: 452f 746d 702f 7079 7465 7374 2d6f 662d  E/tmp/pytest-of-
-00000410: 6265 6e2f 7079 7465 7374 2d33 352f 7465  ben/pytest-35/te
-00000420: 7374 5f6f 7065 6e5f 6272 6169 6e77 6179  st_open_brainway
-00000430: 735f 7072 6f6a 6563 7430 2f69 6d61 6765  s_project0/image
-00000440: 5f31 2e6a 7067 9468 0a4b 0068 034e 7568  _1.jpg.h.K.h.Nuh
-00000450: 0b4d 8a01 4d00 0286 9468 0d4d 8a01 4d00  .M..M....h.M..M.
-00000460: 0286 9468 0f7d 9428 6801 7d94 2868 124b  ...h.}.(h.}.(h.K
-00000470: 0568 1347 0000 0000 0000 0000 6814 4700  .h.G........h.G.
-00000480: 0000 0000 0000 0068 1547 0000 0000 0000  .......h.G......
-00000490: 0000 6816 6817 6818 473f f000 0000 0000  ..h.h.h.G?......
-000004a0: 0075 6819 7d94 2868 1b47 0000 0000 0000  .uh.}.(h.G......
-000004b0: 0000 681c 4700 0000 0000 0000 0068 1d47  ..h.G........h.G
-000004c0: 0000 0000 0000 0000 681e 473f f000 0000  ........h.G?....
-000004d0: 0000 0068 1f47 3ff0 0000 0000 0000 6820  ...h.G?.......h 
-000004e0: 4e68 214e 7568 227d 9428 6824 6827 682a  Nh!Nuh"}.(h$h'h*
-000004f0: 4b00 8594 682c 8794 5294 284b 014b 0a4b  K...h,..R.(K.K.K
-00000500: 0286 9468 3489 4350 0b7f 8c43 6ee4 8c43  ...h4.CP...Cn..C
-00000510: b34e 9a43 19af 5643 48e9 5843 777b 7e43  .N.C..VCH.XCw{~C
-00000520: 6e0b 6043 e5ad af43 9ab2 f643 7213 1743  n.`C...C...Cr..C
-00000530: 7eae ca43 7562 5043 5e6b 9143 b157 b643  ~..CubPC^k.C.W.C
-00000540: 5a7b 1142 d750 0942 0da1 2541 af06 a443  Z{.B.P.B..%A...C
-00000550: 4835 c743 7464 ab43 9474 9462 6839 6827  H5.Ctd.C.t.bh9h'
-00000560: 682a 4b00 8594 682c 8794 5294 284b 014b  h*K...h,..R.(K.K
-00000570: 0a4b 0286 9468 3489 4350 0b7f 8c43 6ee4  .K...h4.CP...Cn.
-00000580: 8c43 b34e 9a43 19af 5643 48e9 5843 777b  .C.N.C..VCH.XCw{
-00000590: 7e43 6e0b 6043 e5ad af43 9ab2 f643 7213  ~Cn.`C...C...Cr.
-000005a0: 1743 7eae ca43 7562 5043 5e6b 9143 b157  .C~..CubPC^k.C.W
-000005b0: b643 5a7b 1142 d750 0942 0da1 2541 af06  .CZ{.B.P.B..%A..
-000005c0: a443 4835 c743 7464 ab43 9474 9462 7568  .CH5.Ctd.C.t.buh
-000005d0: 407d 9428 6842 473f f000 0000 0000 0068  @}.(hBG?.......h
-000005e0: 4388 6844 473f f000 0000 0000 0068 4547  C.hDG?.......hEG
-000005f0: 3ff0 0000 0000 0000 6846 2847 0000 0000  ?.......hF(G....
-00000600: 0000 0000 4700 0000 0000 0000 0047 3ff0  ....G........G?.
-00000610: 0000 0000 0000 473f f000 0000 0000 0074  ......G?.......t
-00000620: 9475 7568 4889 6849 4e68 4a68 4b75 7d94  .uuhH.hINhJhKu}.
-00000630: 2868 067d 9428 6808 8c45 2f74 6d70 2f70  (h.}.(h..E/tmp/p
-00000640: 7974 6573 742d 6f66 2d62 656e 2f70 7974  ytest-of-ben/pyt
-00000650: 6573 742d 3335 2f74 6573 745f 6f70 656e  est-35/test_open
-00000660: 5f62 7261 696e 7761 7973 5f70 726f 6a65  _brainways_proje
-00000670: 6374 302f 696d 6167 655f 322e 6a70 6794  ct0/image_2.jpg.
-00000680: 680a 4b00 6803 4e75 680b 4d8a 014d 0002  h.K.h.Nuh.M..M..
-00000690: 8694 680d 4d8a 014d 0002 8694 680f 7d94  ..h.M..M....h.}.
-000006a0: 2868 017d 9428 6812 4b05 6813 4700 0000  (h.}.(h.K.h.G...
-000006b0: 0000 0000 0068 1447 0000 0000 0000 0000  .....h.G........
-000006c0: 6815 4700 0000 0000 0000 0068 1668 1768  h.G........h.h.h
-000006d0: 1847 3ff0 0000 0000 0000 7568 197d 9428  .G?.......uh.}.(
-000006e0: 681b 4700 0000 0000 0000 0068 1c47 0000  h.G........h.G..
-000006f0: 0000 0000 0000 681d 4700 0000 0000 0000  ......h.G.......
-00000700: 0068 1e47 3ff0 0000 0000 0000 681f 473f  .h.G?.......h.G?
-00000710: f000 0000 0000 0068 204e 6821 4e75 6822  .......h Nh!Nuh"
-00000720: 7d94 2868 2468 2768 2a4b 0085 9468 2c87  }.(h$h'h*K...h,.
-00000730: 9452 9428 4b01 4b0a 4b02 8694 6834 8943  .R.(K.K.K...h4.C
-00000740: 500b 7f8c 436e e48c 43b3 4e9a 4319 af56  P...Cn..C.N.C..V
-00000750: 4348 e958 4377 7b7e 436e 0b60 43e5 adaf  CH.XCw{~Cn.`C...
-00000760: 439a b2f6 4372 1317 437e aeca 4375 6250  C...Cr..C~..CubP
-00000770: 435e 6b91 43b1 57b6 435a 7b11 42d7 5009  C^k.C.W.CZ{.B.P.
-00000780: 420d a125 41af 06a4 4348 35c7 4374 64ab  B..%A...CH5.Ctd.
-00000790: 4394 7494 6268 3968 2768 2a4b 0085 9468  C.t.bh9h'h*K...h
-000007a0: 2c87 9452 9428 4b01 4b0a 4b02 8694 6834  ,..R.(K.K.K...h4
-000007b0: 8943 500b 7f8c 436e e48c 43b3 4e9a 4319  .CP...Cn..C.N.C.
-000007c0: af56 4348 e958 4377 7b7e 436e 0b60 43e5  .VCH.XCw{~Cn.`C.
-000007d0: adaf 439a b2f6 4372 1317 437e aeca 4375  ..C...Cr..C~..Cu
-000007e0: 6250 435e 6b91 43b1 57b6 435a 7b11 42d7  bPC^k.C.W.CZ{.B.
-000007f0: 5009 420d a125 41af 06a4 4348 35c7 4374  P.B..%A...CH5.Ct
-00000800: 64ab 4394 7494 6275 6840 7d94 2868 4247  d.C.t.buh@}.(hBG
-00000810: 3ff0 0000 0000 0000 6843 8868 4447 3ff0  ?.......hC.hDG?.
-00000820: 0000 0000 0000 6845 473f f000 0000 0000  ......hEG?......
-00000830: 0068 4628 4700 0000 0000 0000 0047 0000  .hF(G........G..
-00000840: 0000 0000 0000 473f f000 0000 0000 0047  ......G?.......G
-00000850: 3ff0 0000 0000 0000 7494 7575 6848 8968  ?.......t.uuhH.h
-00000860: 494e 684a 684b 7565 8694 2e              INhJhKue...
+00000060: 7079 7465 7374 2d39 382f 7465 7374 5f75  pytest-98/test_u
+00000070: 7064 6174 655f 7072 6f6a 6563 745f 6672  pdate_project_fr
+00000080: 6f6d 5f76 305f 315f 302f 696d 6167 652e  om_v0_1_0/image.
+00000090: 6a70 6794 8c05 7363 656e 6594 4b00 6803  jpg...scene.K.h.
+000000a0: 4e75 8c0a 696d 6167 655f 7369 7a65 944d  Nu..image_size.M
+000000b0: 8a01 4d00 0286 948c 116c 6f77 7265 735f  ..M......lowres_
+000000c0: 696d 6167 655f 7369 7a65 944d 8a01 4d00  image_size.M..M.
+000000d0: 0286 948c 0670 6172 616d 7394 7d94 2868  .....params.}.(h
+000000e0: 017d 9428 8c02 6170 944b 058c 0b72 6f74  .}.(..ap.K...rot
+000000f0: 5f66 726f 6e74 616c 9447 0000 0000 0000  _frontal.G......
+00000100: 0000 8c0e 726f 745f 686f 7269 7a6f 6e74  ....rot_horizont
+00000110: 616c 9447 0000 0000 0000 0000 8c0c 726f  al.G..........ro
+00000120: 745f 7361 6769 7474 616c 9447 0000 0000  t_sagittal.G....
+00000130: 0000 0000 8c0a 6865 6d69 7370 6865 7265  ......hemisphere
+00000140: 948c 0462 6f74 6894 8c0a 636f 6e66 6964  ...both...confid
+00000150: 656e 6365 9447 3ff0 0000 0000 0000 758c  ence.G?.......u.
+00000160: 0661 6666 696e 6594 7d94 288c 0561 6e67  .affine.}.(..ang
+00000170: 6c65 9447 0000 0000 0000 0000 8c02 7478  le.G..........tx
+00000180: 9447 0000 0000 0000 0000 8c02 7479 9447  .G..........ty.G
+00000190: 0000 0000 0000 0000 8c02 7378 9447 3ff0  ..........sx.G?.
+000001a0: 0000 0000 0000 8c02 7379 9447 3ff0 0000  ........sy.G?...
+000001b0: 0000 0000 8c02 6378 944e 8c02 6379 944e  ......cx.N..cy.N
+000001c0: 758c 0374 7073 947d 9428 8c0a 706f 696e  u..tps.}.(..poin
+000001d0: 7473 5f73 7263 948c 156e 756d 7079 2e63  ts_src...numpy.c
+000001e0: 6f72 652e 6d75 6c74 6961 7272 6179 948c  ore.multiarray..
+000001f0: 0c5f 7265 636f 6e73 7472 7563 7494 9394  ._reconstruct...
+00000200: 8c05 6e75 6d70 7994 8c07 6e64 6172 7261  ..numpy...ndarra
+00000210: 7994 9394 4b00 8594 4301 6294 8794 5294  y...K...C.b...R.
+00000220: 284b 014b 0a4b 0286 9468 288c 0564 7479  (K.K.K...h(..dty
+00000230: 7065 9493 948c 0266 3494 8988 8794 5294  pe.....f4.....R.
+00000240: 284b 038c 013c 944e 4e4e 4aff ffff ff4a  (K...<.NNNJ....J
+00000250: ffff ffff 4b00 7494 6289 4350 0b7f 8c43  ....K.t.b.CP...C
+00000260: 6ee4 8c43 b34e 9a43 19af 5643 48e9 5843  n..C.N.C..VCH.XC
+00000270: 777b 7e43 6e0b 6043 e5ad af43 9ab2 f643  w{~Cn.`C...C...C
+00000280: 7213 1743 7eae ca43 7562 5043 5e6b 9143  r..C~..CubPC^k.C
+00000290: b157 b643 5a7b 1142 d750 0942 0da1 2541  .W.CZ{.B.P.B..%A
+000002a0: af06 a443 4835 c743 7464 ab43 9474 9462  ...CH5.Ctd.C.t.b
+000002b0: 8c0a 706f 696e 7473 5f64 7374 9468 2768  ..points_dst.h'h
+000002c0: 2a4b 0085 9468 2c87 9452 9428 4b01 4b0a  *K...h,..R.(K.K.
+000002d0: 4b02 8694 6834 8943 500b 7f8c 436e e48c  K...h4.CP...Cn..
+000002e0: 43b3 4e9a 4319 af56 4348 e958 4377 7b7e  C.N.C..VCH.XCw{~
+000002f0: 436e 0b60 43e5 adaf 439a b2f6 4372 1317  Cn.`C...C...Cr..
+00000300: 437e aeca 4375 6250 435e 6b91 43b1 57b6  C~..CubPC^k.C.W.
+00000310: 435a 7b11 42d7 5009 420d a125 41af 06a4  CZ{.B.P.B..%A...
+00000320: 4348 35c7 4374 64ab 4394 7494 6275 8c04  CH5.Ctd.C.t.bu..
+00000330: 6365 6c6c 947d 9428 8c08 6469 616d 6574  cell.}.(..diamet
+00000340: 6572 9447 3ff0 0000 0000 0000 8c07 6e65  er.G?.........ne
+00000350: 745f 6176 6794 888c 0e66 6c6f 775f 7468  t_avg....flow_th
+00000360: 7265 7368 6f6c 6494 473f f000 0000 0000  reshold.G?......
+00000370: 008c 0e6d 6173 6b5f 7468 7265 7368 6f6c  ...mask_threshol
+00000380: 6494 473f f000 0000 0000 008c 0a70 7265  d.G?.........pre
+00000390: 7669 6577 5f62 6294 2847 0000 0000 0000  view_bb.(G......
+000003a0: 0000 4700 0000 0000 0000 0047 3ff0 0000  ..G........G?...
+000003b0: 0000 0000 473f f000 0000 0000 0074 9475  ....G?.......t.u
+000003c0: 758c 0669 676e 6f72 6594 888c 1470 6879  u..ignore....phy
+000003d0: 7369 6361 6c5f 7069 7865 6c5f 7369 7a65  sical_pixel_size
+000003e0: 7394 4e8c 0776 6572 7369 6f6e 948c 0530  s.N..version...0
+000003f0: 2e31 2e31 9475 7d94 2868 067d 9428 6808  .1.1.u}.(h.}.(h.
+00000400: 6809 680a 4b00 6803 4e75 680b 4d8a 014d  h.h.K.h.Nuh.M..M
+00000410: 0002 8694 680d 4d8a 014d 0002 8694 680f  ....h.M..M....h.
+00000420: 7d94 2868 017d 9428 6812 4b05 6813 4700  }.(h.}.(h.K.h.G.
+00000430: 0000 0000 0000 0068 1447 0000 0000 0000  .......h.G......
+00000440: 0000 6815 4700 0000 0000 0000 0068 1668  ..h.G........h.h
+00000450: 1768 1847 3ff0 0000 0000 0000 7568 197d  .h.G?.......uh.}
+00000460: 9428 681b 4700 0000 0000 0000 0068 1c47  .(h.G........h.G
+00000470: 0000 0000 0000 0000 681d 4700 0000 0000  ........h.G.....
+00000480: 0000 0068 1e47 3ff0 0000 0000 0000 681f  ...h.G?.......h.
+00000490: 473f f000 0000 0000 0068 204e 6821 4e75  G?.......h Nh!Nu
+000004a0: 6822 7d94 2868 2468 2768 2a4b 0085 9468  h"}.(h$h'h*K...h
+000004b0: 2c87 9452 9428 4b01 4b0a 4b02 8694 6834  ,..R.(K.K.K...h4
+000004c0: 8943 500b 7f8c 436e e48c 43b3 4e9a 4319  .CP...Cn..C.N.C.
+000004d0: af56 4348 e958 4377 7b7e 436e 0b60 43e5  .VCH.XCw{~Cn.`C.
+000004e0: adaf 439a b2f6 4372 1317 437e aeca 4375  ..C...Cr..C~..Cu
+000004f0: 6250 435e 6b91 43b1 57b6 435a 7b11 42d7  bPC^k.C.W.CZ{.B.
+00000500: 5009 420d a125 41af 06a4 4348 35c7 4374  P.B..%A...CH5.Ct
+00000510: 64ab 4394 7494 6268 3968 2768 2a4b 0085  d.C.t.bh9h'h*K..
+00000520: 9468 2c87 9452 9428 4b01 4b0a 4b02 8694  .h,..R.(K.K.K...
+00000530: 6834 8943 500b 7f8c 436e e48c 43b3 4e9a  h4.CP...Cn..C.N.
+00000540: 4319 af56 4348 e958 4377 7b7e 436e 0b60  C..VCH.XCw{~Cn.`
+00000550: 43e5 adaf 439a b2f6 4372 1317 437e aeca  C...C...Cr..C~..
+00000560: 4375 6250 435e 6b91 43b1 57b6 435a 7b11  CubPC^k.C.W.CZ{.
+00000570: 42d7 5009 420d a125 41af 06a4 4348 35c7  B.P.B..%A...CH5.
+00000580: 4374 64ab 4394 7494 6275 6840 7d94 2868  Ctd.C.t.buh@}.(h
+00000590: 4247 3ff0 0000 0000 0000 6843 8868 4447  BG?.......hC.hDG
+000005a0: 3ff0 0000 0000 0000 6845 473f f000 0000  ?.......hEG?....
+000005b0: 0000 0068 4628 4700 0000 0000 0000 0047  ...hF(G........G
+000005c0: 0000 0000 0000 0000 473f f000 0000 0000  ........G?......
+000005d0: 0047 3ff0 0000 0000 0000 7494 7575 6848  .G?.......t.uuhH
+000005e0: 8968 494e 684a 684b 757d 9428 6806 7d94  .hINhJhKu}.(h.}.
+000005f0: 2868 0868 0968 0a4b 0068 034e 7568 0b4d  (h.h.h.K.h.Nuh.M
+00000600: 8a01 4d00 0286 9468 0d4d 8a01 4d00 0286  ..M....h.M..M...
+00000610: 9468 0f7d 9428 6801 7d94 2868 124b 0568  .h.}.(h.}.(h.K.h
+00000620: 1347 0000 0000 0000 0000 6814 4700 0000  .G........h.G...
+00000630: 0000 0000 0068 1547 0000 0000 0000 0000  .....h.G........
+00000640: 6816 6817 6818 473f f000 0000 0000 0075  h.h.h.G?.......u
+00000650: 6819 7d94 2868 1b47 0000 0000 0000 0000  h.}.(h.G........
+00000660: 681c 4700 0000 0000 0000 0068 1d47 0000  h.G........h.G..
+00000670: 0000 0000 0000 681e 473f f000 0000 0000  ......h.G?......
+00000680: 0068 1f47 3ff0 0000 0000 0000 6820 4e68  .h.G?.......h Nh
+00000690: 214e 7568 227d 9428 6824 6827 682a 4b00  !Nuh"}.(h$h'h*K.
+000006a0: 8594 682c 8794 5294 284b 014b 0a4b 0286  ..h,..R.(K.K.K..
+000006b0: 9468 3489 4350 0b7f 8c43 6ee4 8c43 b34e  .h4.CP...Cn..C.N
+000006c0: 9a43 19af 5643 48e9 5843 777b 7e43 6e0b  .C..VCH.XCw{~Cn.
+000006d0: 6043 e5ad af43 9ab2 f643 7213 1743 7eae  `C...C...Cr..C~.
+000006e0: ca43 7562 5043 5e6b 9143 b157 b643 5a7b  .CubPC^k.C.W.CZ{
+000006f0: 1142 d750 0942 0da1 2541 af06 a443 4835  .B.P.B..%A...CH5
+00000700: c743 7464 ab43 9474 9462 6839 6827 682a  .Ctd.C.t.bh9h'h*
+00000710: 4b00 8594 682c 8794 5294 284b 014b 0a4b  K...h,..R.(K.K.K
+00000720: 0286 9468 3489 4350 0b7f 8c43 6ee4 8c43  ...h4.CP...Cn..C
+00000730: b34e 9a43 19af 5643 48e9 5843 777b 7e43  .N.C..VCH.XCw{~C
+00000740: 6e0b 6043 e5ad af43 9ab2 f643 7213 1743  n.`C...C...Cr..C
+00000750: 7eae ca43 7562 5043 5e6b 9143 b157 b643  ~..CubPC^k.C.W.C
+00000760: 5a7b 1142 d750 0942 0da1 2541 af06 a443  Z{.B.P.B..%A...C
+00000770: 4835 c743 7464 ab43 9474 9462 7568 407d  H5.Ctd.C.t.buh@}
+00000780: 9428 6842 473f f000 0000 0000 0068 4388  .(hBG?.......hC.
+00000790: 6844 473f f000 0000 0000 0068 4547 3ff0  hDG?.......hEG?.
+000007a0: 0000 0000 0000 6846 2847 0000 0000 0000  ......hF(G......
+000007b0: 0000 4700 0000 0000 0000 0047 3ff0 0000  ..G........G?...
+000007c0: 0000 0000 473f f000 0000 0000 0074 9475  ....G?.......t.u
+000007d0: 7568 4889 6849 4e68 4a68 4b75 6586 942e  uhH.hINhJhKue...
```

### Comparing `brainways-0.1.4/src/brainways/project/_utils.py` & `brainways-0.1.5/src/brainways/project/_utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import pickle
 from pathlib import Path
 from typing import Optional
 
 from packaging import version
 
 import brainways
+from brainways.utils.io_utils.readers.qupath_reader import QupathReader
 
 
 def rewrite_project_version(path: Path, version: Optional[str] = None):
     if version is None:
         version = brainways._version.version
 
     with open(path) as f:
@@ -21,14 +22,16 @@
 
 def update_project_from_previous_versions(path: Path):
     with open(path) as f:
         serialized_settings = json.load(f)
     project_version = serialized_settings.get("version", "0.1.1")
     if version.parse(project_version) <= version.parse("0.1.1"):
         update_project_from_0_1_1_to_0_1_4(path)
+    if version.parse(project_version) <= version.parse("0.1.4"):
+        update_project_from_0_1_4_to_0_1_5(path)
 
     rewrite_project_version(path)
 
 
 def update_project_from_0_1_1_to_0_1_4(path: Path):
     brainways_subject_paths = path.parent.rglob("brainways.bin")
     for brainways_subject_path in brainways_subject_paths:
@@ -37,7 +40,22 @@
         for serialized_slice_info in serialized_slice_infos:
             if "cell" in serialized_slice_info["params"]:
                 del serialized_slice_info["params"]["cell"]
         with open(brainways_subject_path, "wb") as f:
             pickle.dump((serialized_settings, serialized_slice_infos), f)
 
     rewrite_project_version(path=path, version="0.1.4")
+
+
+def update_project_from_0_1_4_to_0_1_5(path: Path):
+    brainways_subject_paths = path.parent.rglob("brainways.bin")
+    for brainways_subject_path in brainways_subject_paths:
+        with open(brainways_subject_path, "rb") as f:
+            serialized_settings, serialized_slice_infos = pickle.load(f)
+        for serialized_slice_info in serialized_slice_infos:
+            reader = QupathReader(serialized_slice_info["path"]["filename"])
+            pps = reader.physical_pixel_sizes
+            serialized_slice_info["physical_pixel_sizes"] = (pps.Y, pps.X)
+        with open(brainways_subject_path, "wb") as f:
+            pickle.dump((serialized_settings, serialized_slice_infos), f)
+
+    rewrite_project_version(path=path, version="0.1.5")
```

### Comparing `brainways-0.1.4/src/brainways/project/brainways_project.py` & `brainways-0.1.5/src/brainways/project/brainways_project.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.4/src/brainways/project/brainways_subject.py` & `brainways-0.1.5/src/brainways/project/brainways_subject.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,18 +114,20 @@
         return image
 
     def add_image(self, path: ImagePath, load_thumbnail: bool = True) -> SliceInfo:
         image_size = get_image_size(path)
         lowres_image_size = get_resize_size(
             input_size=image_size, output_size=(1024, 1024), keep_aspect=True
         )
+        pps = QupathReader(path.filename).physical_pixel_sizes
         document = SliceInfo(
             path=path,
             image_size=image_size,
             lowres_image_size=lowres_image_size,
+            physical_pixel_sizes=(pps.Y, pps.X),
         )
         if load_thumbnail:
             self.read_lowres_image(document)
         self.documents.append(document)
         return document
 
     @staticmethod
```

### Comparing `brainways-0.1.4/src/brainways/project/info_classes.py` & `brainways-0.1.5/src/brainways/project/info_classes.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.4/src/brainways/scripts/_tests/test_cli.py` & `brainways-0.1.5/src/brainways/scripts/_tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.4/src/brainways/scripts/batch_create_thumbnails.py` & `brainways-0.1.5/src/brainways/scripts/batch_create_thumbnails.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.4/src/brainways/scripts/cell_detection.py` & `brainways-0.1.5/src/brainways/scripts/cell_detection.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.4/src/brainways/scripts/cli.py` & `brainways-0.1.5/src/brainways/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.4/src/brainways/scripts/create_excel.py` & `brainways-0.1.5/src/brainways/scripts/create_excel.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.4/src/brainways/scripts/create_excel_colabelling.py` & `brainways-0.1.5/src/brainways/scripts/create_excel_colabelling.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.4/src/brainways/scripts/create_reg_model_data.py` & `brainways-0.1.5/src/brainways/scripts/create_reg_model_data.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.4/src/brainways/scripts/display_area.py` & `brainways-0.1.5/src/brainways/scripts/display_area.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.4/src/brainways/scripts/import_cell_detections_keren.py` & `brainways-0.1.5/src/brainways/scripts/import_cell_detections_keren.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.4/src/brainways/scripts/import_cells.py` & `brainways-0.1.5/src/brainways/scripts/import_cells.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.4/src/brainways/scripts/move_images.py` & `brainways-0.1.5/src/brainways/scripts/move_images.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.4/src/brainways/transforms/_tests/test_affine_transform_2d.py` & `brainways-0.1.5/src/brainways/transforms/_tests/test_affine_transform_2d.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.4/src/brainways/transforms/_tests/test_depth_registration.py` & `brainways-0.1.5/src/brainways/transforms/_tests/test_depth_registration.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.4/src/brainways/transforms/_tests/test_image_to_atlas_transform.py` & `brainways-0.1.5/src/brainways/transforms/_tests/test_image_to_atlas_transform.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.4/src/brainways/transforms/_tests/test_tps_transform.py` & `brainways-0.1.5/src/brainways/transforms/_tests/test_tps_transform.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.4/src/brainways/transforms/affine_transform_2d.py` & `brainways-0.1.5/src/brainways/transforms/affine_transform_2d.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.4/src/brainways/transforms/compose.py` & `brainways-0.1.5/src/brainways/transforms/compose.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.4/src/brainways/transforms/depth_registration.py` & `brainways-0.1.5/src/brainways/transforms/depth_registration.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.4/src/brainways/transforms/image_to_atlas_transform.py` & `brainways-0.1.5/src/brainways/transforms/image_to_atlas_transform.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.4/src/brainways/transforms/tps_transform.py` & `brainways-0.1.5/src/brainways/transforms/tps_transform.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.4/src/brainways/utils/_imports.py` & `brainways-0.1.5/src/brainways/utils/_imports.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.4/src/brainways/utils/_tests/test_cell_count_summary.py` & `brainways-0.1.5/src/brainways/utils/_tests/test_cell_count_summary.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.4/src/brainways/utils/_tests/test_cells.py` & `brainways-0.1.5/src/brainways/utils/_tests/test_cells.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.4/src/brainways/utils/_tests/test_image.py` & `brainways-0.1.5/src/brainways/utils/_tests/test_image.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.4/src/brainways/utils/atlas/_tests/test_slice_atlas.py` & `brainways-0.1.5/src/brainways/utils/atlas/_tests/test_slice_atlas.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.4/src/brainways/utils/atlas/brainways_atlas.py` & `brainways-0.1.5/src/brainways/utils/atlas/brainways_atlas.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.4/src/brainways/utils/atlas/slice_atlas.py` & `brainways-0.1.5/src/brainways/utils/atlas/slice_atlas.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.4/src/brainways/utils/cell_count_summary.py` & `brainways-0.1.5/src/brainways/utils/cell_count_summary.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.4/src/brainways/utils/cell_detection_importer/_tests/qupath_sample_file.txt` & `brainways-0.1.5/src/brainways/utils/cell_detection_importer/_tests/qupath_sample_file.txt`

 * *Files identical despite different names*

### Comparing `brainways-0.1.4/src/brainways/utils/cell_detection_importer/_tests/test_brainways_cell_detection_importer.py` & `brainways-0.1.5/src/brainways/utils/cell_detection_importer/_tests/test_brainways_cell_detection_importer.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.4/src/brainways/utils/cell_detection_importer/_tests/test_qupath_cell_detection_importer.py` & `brainways-0.1.5/src/brainways/utils/cell_detection_importer/_tests/test_qupath_cell_detection_importer.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.4/src/brainways/utils/cell_detection_importer/brainways_cell_detection_importer.py` & `brainways-0.1.5/src/brainways/utils/cell_detection_importer/brainways_cell_detection_importer.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.4/src/brainways/utils/cell_detection_importer/keren_cell_detection_importer.py` & `brainways-0.1.5/src/brainways/utils/cell_detection_importer/keren_cell_detection_importer.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.4/src/brainways/utils/cell_detection_importer/utils.py` & `brainways-0.1.5/src/brainways/utils/cell_detection_importer/utils.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.4/src/brainways/utils/cells.py` & `brainways-0.1.5/src/brainways/utils/cells.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.4/src/brainways/utils/config.py` & `brainways-0.1.5/src/brainways/utils/config.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.4/src/brainways/utils/czi/czi_to_jpg.py` & `brainways-0.1.5/src/brainways/utils/czi/czi_to_jpg.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.4/src/brainways/utils/dataclasses.py` & `brainways-0.1.5/src/brainways/utils/dataclasses.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.4/src/brainways/utils/image.py` & `brainways-0.1.5/src/brainways/utils/image.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.4/src/brainways/utils/io_utils/file_iterators/qupath.py` & `brainways-0.1.5/src/brainways/utils/io_utils/file_iterators/qupath.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.4/src/brainways/utils/io_utils/image_path.py` & `brainways-0.1.5/src/brainways/utils/io_utils/image_path.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.4/src/brainways/utils/io_utils/readers/__init__.py` & `brainways-0.1.5/src/brainways/utils/io_utils/readers/__init__.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.4/src/brainways/utils/io_utils/readers/aicsimageio_reader.py` & `brainways-0.1.5/src/brainways/utils/io_utils/readers/aicsimageio_reader.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.4/src/brainways/utils/io_utils/readers/base.py` & `brainways-0.1.5/src/brainways/utils/io_utils/readers/base.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.4/src/brainways/utils/io_utils/readers/czi_reader.py` & `brainways-0.1.5/src/brainways/utils/io_utils/readers/czi_reader.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.4/src/brainways/utils/io_utils/readers/qupath_reader.py` & `brainways-0.1.5/src/brainways/utils/io_utils/readers/qupath_reader.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.4/src/brainways/utils/preprocess.py` & `brainways-0.1.5/src/brainways/utils/preprocess.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.4/src/brainways/utils/qupath.py` & `brainways-0.1.5/src/brainways/utils/qupath.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.4/src/brainways/utils/test_utils.py` & `brainways-0.1.5/src/brainways/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.4/src/brainways.egg-info/PKG-INFO` & `brainways-0.1.5/src/brainways.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brainways
-Version: 0.1.4
+Version: 0.1.5
 Summary: Brainways
 Home-page: https://github.com/bkntr/brainways
 Author: Ben Kantor
 Author-email: benkantor@mail.tau.ac.il
 License: GPL-3.0
 Project-URL: Bug Tracker, https://github.com/bkntr/brainways/issues
 Project-URL: Documentation, https://github.com/bkntr/brainways#README.md
```

### Comparing `brainways-0.1.4/src/brainways.egg-info/SOURCES.txt` & `brainways-0.1.5/src/brainways.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -63,26 +63,29 @@
 src/brainways/pipeline/atlas_registration.py
 src/brainways/pipeline/brainways_params.py
 src/brainways/pipeline/brainways_pipeline.py
 src/brainways/pipeline/cell_detector.py
 src/brainways/pipeline/tps.py
 src/brainways/pipeline/_tests/test_atlas_registration.py
 src/brainways/pipeline/_tests/test_brainways_pipeline.py
+src/brainways/pipeline/_tests/test_cell_detector.py
 src/brainways/project/__init__.py
 src/brainways/project/_utils.py
 src/brainways/project/brainways_project.py
 src/brainways/project/brainways_subject.py
 src/brainways/project/info_classes.py
 src/brainways/project/_tests/__init__.py
 src/brainways/project/_tests/conftest.py
 src/brainways/project/_tests/test_brainways_project.py
 src/brainways/project/_tests/test_brainways_subject.py
 src/brainways/project/_tests/test_utils.py
 src/brainways/project/_tests/test_projects/v0.1.1/project.bwp
 src/brainways/project/_tests/test_projects/v0.1.1/subject1/brainways.bin
+src/brainways/project/_tests/test_projects/v0.1.4/project.bwp
+src/brainways/project/_tests/test_projects/v0.1.4/subject1/brainways.bin
 src/brainways/scripts/__init__.py
 src/brainways/scripts/batch_create_thumbnails.py
 src/brainways/scripts/cell_detection.py
 src/brainways/scripts/cli.py
 src/brainways/scripts/create_excel.py
 src/brainways/scripts/create_excel_colabelling.py
 src/brainways/scripts/create_reg_model_data.py
```

### Comparing `brainways-0.1.4/tox.ini` & `brainways-0.1.5/tox.ini`

 * *Files identical despite different names*

