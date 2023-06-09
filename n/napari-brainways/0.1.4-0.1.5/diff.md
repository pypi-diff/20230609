# Comparing `tmp/napari_brainways-0.1.4.tar.gz` & `tmp/napari_brainways-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari_brainways-0.1.4.tar", last modified: Thu Jun  8 07:45:34 2023, max compression
+gzip compressed data, was "napari_brainways-0.1.5.tar", last modified: Fri Jun  9 09:41:44 2023, max compression
```

## Comparing `napari_brainways-0.1.4.tar` & `napari_brainways-0.1.5.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:45:34.307019 napari_brainways-0.1.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:45:34.299019 napari_brainways-0.1.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:45:34.303019 napari_brainways-0.1.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-06-08 07:45:11.000000 napari_brainways-0.1.4/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-06-08 07:45:11.000000 napari_brainways-0.1.4/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:45:34.303019 napari_brainways-0.1.4/.napari/
--rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-06-08 07:45:11.000000 napari_brainways-0.1.4/.napari/DESCRIPTION.md
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-06-08 07:45:11.000000 napari_brainways-0.1.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-06-08 07:45:11.000000 napari_brainways-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-08 07:45:11.000000 napari_brainways-0.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-06-08 07:45:34.307019 napari_brainways-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-06-08 07:45:11.000000 napari_brainways-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:45:34.303019 napari_brainways-0.1.4/data/
--rw-r--r--   0 runner    (1001) docker     (123)   269441 2023-06-08 07:45:11.000000 napari_brainways-0.1.4/data/test_data.npz
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-08 07:45:11.000000 napari_brainways-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-06-08 07:45:34.307019 napari_brainways-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-08 07:45:11.000000 napari_brainways-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:45:34.299019 napari_brainways-0.1.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:45:34.303019 napari_brainways-0.1.4/src/napari_brainways/
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-08 07:45:11.000000 napari_brainways-0.1.4/src/napari_brainways/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-08 07:45:11.000000 napari_brainways-0.1.4/src/napari_brainways/_sample_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:45:34.303019 napari_brainways-0.1.4/src/napari_brainways/_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 07:45:11.000000 napari_brainways-0.1.4/src/napari_brainways/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-08 07:45:11.000000 napari_brainways-0.1.4/src/napari_brainways/_tests/test_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-08 07:45:11.000000 napari_brainways-0.1.4/src/napari_brainways/_tests/test_sample_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     8087 2023-06-08 07:45:11.000000 napari_brainways-0.1.4/src/napari_brainways/_tests/test_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-08 07:45:34.000000 napari_brainways-0.1.4/src/napari_brainways/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    18697 2023-06-08 07:45:11.000000 napari_brainways-0.1.4/src/napari_brainways/brainways_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     9124 2023-06-08 07:45:11.000000 napari_brainways-0.1.4/src/napari_brainways/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:45:34.307019 napari_brainways-0.1.4/src/napari_brainways/controllers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 07:45:11.000000 napari_brainways-0.1.4/src/napari_brainways/controllers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:45:34.307019 napari_brainways-0.1.4/src/napari_brainways/controllers/_tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-06-08 07:45:11.000000 napari_brainways-0.1.4/src/napari_brainways/controllers/_tests/test_affine_2d_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-06-08 07:45:11.000000 napari_brainways-0.1.4/src/napari_brainways/controllers/_tests/test_annotation_viewer_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-08 07:45:11.000000 napari_brainways-0.1.4/src/napari_brainways/controllers/_tests/test_cell_3d_viewer_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-08 07:45:11.000000 napari_brainways-0.1.4/src/napari_brainways/controllers/_tests/test_cell_detector_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-08 07:45:11.000000 napari_brainways-0.1.4/src/napari_brainways/controllers/_tests/test_registration_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-06-08 07:45:11.000000 napari_brainways-0.1.4/src/napari_brainways/controllers/_tests/test_tps_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     8463 2023-06-08 07:45:11.000000 napari_brainways-0.1.4/src/napari_brainways/controllers/affine_2d_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-06-08 07:45:11.000000 napari_brainways-0.1.4/src/napari_brainways/controllers/annotation_viewer_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-06-08 07:45:11.000000 napari_brainways-0.1.4/src/napari_brainways/controllers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6567 2023-06-08 07:45:11.000000 napari_brainways-0.1.4/src/napari_brainways/controllers/cell_3d_viewer_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)    10951 2023-06-08 07:45:11.000000 napari_brainways-0.1.4/src/napari_brainways/controllers/cell_detector_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     9043 2023-06-08 07:45:11.000000 napari_brainways-0.1.4/src/napari_brainways/controllers/registration_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     9439 2023-06-08 07:45:11.000000 napari_brainways-0.1.4/src/napari_brainways/controllers/tps_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-08 07:45:11.000000 napari_brainways-0.1.4/src/napari_brainways/napari.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-06-08 07:45:11.000000 napari_brainways-0.1.4/src/napari_brainways/napari_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:45:34.307019 napari_brainways-0.1.4/src/napari_brainways/resources/
--rw-r--r--   0 runner    (1001) docker     (123)   231054 2023-06-08 07:45:11.000000 napari_brainways-0.1.4/src/napari_brainways/resources/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-06-08 07:45:11.000000 napari_brainways-0.1.4/src/napari_brainways/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-06-08 07:45:11.000000 napari_brainways-0.1.4/src/napari_brainways/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:45:34.307019 napari_brainways-0.1.4/src/napari_brainways/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 07:45:11.000000 napari_brainways-0.1.4/src/napari_brainways/widgets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:45:34.307019 napari_brainways-0.1.4/src/napari_brainways/widgets/_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 07:45:11.000000 napari_brainways-0.1.4/src/napari_brainways/widgets/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-06-08 07:45:11.000000 napari_brainways-0.1.4/src/napari_brainways/widgets/_tests/test_create_project_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-06-08 07:45:11.000000 napari_brainways-0.1.4/src/napari_brainways/widgets/_tests/test_registration_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-06-08 07:45:11.000000 napari_brainways-0.1.4/src/napari_brainways/widgets/affine_2d_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-06-08 07:45:11.000000 napari_brainways-0.1.4/src/napari_brainways/widgets/cell_detector_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-06-08 07:45:11.000000 napari_brainways-0.1.4/src/napari_brainways/widgets/cell_viewer_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     9397 2023-06-08 07:45:11.000000 napari_brainways-0.1.4/src/napari_brainways/widgets/create_subject_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-06-08 07:45:11.000000 napari_brainways-0.1.4/src/napari_brainways/widgets/registration_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-08 07:45:11.000000 napari_brainways-0.1.4/src/napari_brainways/widgets/tps_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    22354 2023-06-08 07:45:11.000000 napari_brainways-0.1.4/src/napari_brainways/widgets/workflow_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:45:34.303019 napari_brainways-0.1.4/src/napari_brainways.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-06-08 07:45:34.000000 napari_brainways-0.1.4/src/napari_brainways.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-06-08 07:45:34.000000 napari_brainways-0.1.4/src/napari_brainways.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 07:45:34.000000 napari_brainways-0.1.4/src/napari_brainways.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-08 07:45:34.000000 napari_brainways-0.1.4/src/napari_brainways.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-08 07:45:34.000000 napari_brainways-0.1.4/src/napari_brainways.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-08 07:45:34.000000 napari_brainways-0.1.4/src/napari_brainways.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-06-08 07:45:11.000000 napari_brainways-0.1.4/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:41:44.518506 napari_brainways-0.1.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:41:44.510506 napari_brainways-0.1.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:41:44.510506 napari_brainways-0.1.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-06-09 09:41:26.000000 napari_brainways-0.1.5/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-06-09 09:41:26.000000 napari_brainways-0.1.5/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:41:44.510506 napari_brainways-0.1.5/.napari/
+-rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-06-09 09:41:26.000000 napari_brainways-0.1.5/.napari/DESCRIPTION.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-06-09 09:41:26.000000 napari_brainways-0.1.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-06-09 09:41:26.000000 napari_brainways-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-09 09:41:26.000000 napari_brainways-0.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-06-09 09:41:44.518506 napari_brainways-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-06-09 09:41:26.000000 napari_brainways-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:41:44.514506 napari_brainways-0.1.5/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   269441 2023-06-09 09:41:26.000000 napari_brainways-0.1.5/data/test_data.npz
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-09 09:41:26.000000 napari_brainways-0.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-09 09:41:44.518506 napari_brainways-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-09 09:41:26.000000 napari_brainways-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:41:44.510506 napari_brainways-0.1.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:41:44.514506 napari_brainways-0.1.5/src/napari_brainways/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-09 09:41:26.000000 napari_brainways-0.1.5/src/napari_brainways/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-09 09:41:26.000000 napari_brainways-0.1.5/src/napari_brainways/_sample_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:41:44.514506 napari_brainways-0.1.5/src/napari_brainways/_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 09:41:26.000000 napari_brainways-0.1.5/src/napari_brainways/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-09 09:41:26.000000 napari_brainways-0.1.5/src/napari_brainways/_tests/test_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-09 09:41:26.000000 napari_brainways-0.1.5/src/napari_brainways/_tests/test_sample_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8087 2023-06-09 09:41:26.000000 napari_brainways-0.1.5/src/napari_brainways/_tests/test_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-09 09:41:44.000000 napari_brainways-0.1.5/src/napari_brainways/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18697 2023-06-09 09:41:26.000000 napari_brainways-0.1.5/src/napari_brainways/brainways_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9124 2023-06-09 09:41:26.000000 napari_brainways-0.1.5/src/napari_brainways/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:41:44.514506 napari_brainways-0.1.5/src/napari_brainways/controllers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 09:41:26.000000 napari_brainways-0.1.5/src/napari_brainways/controllers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:41:44.514506 napari_brainways-0.1.5/src/napari_brainways/controllers/_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-06-09 09:41:26.000000 napari_brainways-0.1.5/src/napari_brainways/controllers/_tests/test_affine_2d_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-06-09 09:41:26.000000 napari_brainways-0.1.5/src/napari_brainways/controllers/_tests/test_annotation_viewer_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-09 09:41:26.000000 napari_brainways-0.1.5/src/napari_brainways/controllers/_tests/test_cell_3d_viewer_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-09 09:41:26.000000 napari_brainways-0.1.5/src/napari_brainways/controllers/_tests/test_cell_detector_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-09 09:41:26.000000 napari_brainways-0.1.5/src/napari_brainways/controllers/_tests/test_registration_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-06-09 09:41:26.000000 napari_brainways-0.1.5/src/napari_brainways/controllers/_tests/test_tps_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8463 2023-06-09 09:41:26.000000 napari_brainways-0.1.5/src/napari_brainways/controllers/affine_2d_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-06-09 09:41:26.000000 napari_brainways-0.1.5/src/napari_brainways/controllers/annotation_viewer_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-06-09 09:41:26.000000 napari_brainways-0.1.5/src/napari_brainways/controllers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6567 2023-06-09 09:41:26.000000 napari_brainways-0.1.5/src/napari_brainways/controllers/cell_3d_viewer_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10951 2023-06-09 09:41:26.000000 napari_brainways-0.1.5/src/napari_brainways/controllers/cell_detector_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9043 2023-06-09 09:41:26.000000 napari_brainways-0.1.5/src/napari_brainways/controllers/registration_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9439 2023-06-09 09:41:26.000000 napari_brainways-0.1.5/src/napari_brainways/controllers/tps_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-09 09:41:26.000000 napari_brainways-0.1.5/src/napari_brainways/napari.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-06-09 09:41:26.000000 napari_brainways-0.1.5/src/napari_brainways/napari_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:41:44.518506 napari_brainways-0.1.5/src/napari_brainways/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)   231054 2023-06-09 09:41:26.000000 napari_brainways-0.1.5/src/napari_brainways/resources/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-06-09 09:41:26.000000 napari_brainways-0.1.5/src/napari_brainways/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-06-09 09:41:26.000000 napari_brainways-0.1.5/src/napari_brainways/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:41:44.518506 napari_brainways-0.1.5/src/napari_brainways/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 09:41:26.000000 napari_brainways-0.1.5/src/napari_brainways/widgets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:41:44.518506 napari_brainways-0.1.5/src/napari_brainways/widgets/_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 09:41:26.000000 napari_brainways-0.1.5/src/napari_brainways/widgets/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-06-09 09:41:26.000000 napari_brainways-0.1.5/src/napari_brainways/widgets/_tests/test_create_project_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-06-09 09:41:26.000000 napari_brainways-0.1.5/src/napari_brainways/widgets/_tests/test_registration_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-06-09 09:41:26.000000 napari_brainways-0.1.5/src/napari_brainways/widgets/affine_2d_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-06-09 09:41:26.000000 napari_brainways-0.1.5/src/napari_brainways/widgets/cell_detector_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-06-09 09:41:26.000000 napari_brainways-0.1.5/src/napari_brainways/widgets/cell_viewer_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9397 2023-06-09 09:41:26.000000 napari_brainways-0.1.5/src/napari_brainways/widgets/create_subject_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-06-09 09:41:26.000000 napari_brainways-0.1.5/src/napari_brainways/widgets/registration_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-09 09:41:26.000000 napari_brainways-0.1.5/src/napari_brainways/widgets/tps_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22436 2023-06-09 09:41:26.000000 napari_brainways-0.1.5/src/napari_brainways/widgets/workflow_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:41:44.514506 napari_brainways-0.1.5/src/napari_brainways.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-06-09 09:41:44.000000 napari_brainways-0.1.5/src/napari_brainways.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-06-09 09:41:44.000000 napari_brainways-0.1.5/src/napari_brainways.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 09:41:44.000000 napari_brainways-0.1.5/src/napari_brainways.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-09 09:41:44.000000 napari_brainways-0.1.5/src/napari_brainways.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-09 09:41:44.000000 napari_brainways-0.1.5/src/napari_brainways.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-09 09:41:44.000000 napari_brainways-0.1.5/src/napari_brainways.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-06-09 09:41:26.000000 napari_brainways-0.1.5/tox.ini
```

### Comparing `napari_brainways-0.1.4/.github/workflows/test_and_deploy.yml` & `napari_brainways-0.1.5/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.4/.gitignore` & `napari_brainways-0.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.4/.napari/DESCRIPTION.md` & `napari_brainways-0.1.5/.napari/DESCRIPTION.md`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.4/.pre-commit-config.yaml` & `napari_brainways-0.1.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.4/LICENSE` & `napari_brainways-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.4/PKG-INFO` & `napari_brainways-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari_brainways
-Version: 0.1.4
+Version: 0.1.5
 Summary: Brainways UI
 Home-page: https://github.com/bkntr/napari-brainways
 Author: Ben Kantor
 Author-email: benkantor@mail.tau.ac.il
 License: GPL-3.0
 Project-URL: Bug Tracker, https://github.com/bkntr/napari-brainways/issues
 Project-URL: Documentation, https://github.com/bkntr/napari-brainways#README.md
```

### Comparing `napari_brainways-0.1.4/README.md` & `napari_brainways-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.4/data/test_data.npz` & `napari_brainways-0.1.5/data/test_data.npz`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.4/setup.cfg` & `napari_brainways-0.1.5/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -27,18 +27,20 @@
 	Documentation = https://github.com/bkntr/napari-brainways#README.md
 	Source Code = https://github.com/bkntr/napari-brainways
 	User Support = https://github.com/bkntr/napari-brainways/issues
 
 [options]
 packages = find:
 install_requires = 
-	brainways==0.1.4
+	brainways==0.1.5
 	importlib-resources
 	napari
 	qtpy
+	stardist==0.8.3
+	tensorflow
 python_requires = >=3.8
 include_package_data = True
 package_dir = 
 	=src
 setup_requires = 
 	setuptools-scm
```

### Comparing `napari_brainways-0.1.4/src/napari_brainways/_sample_data.py` & `napari_brainways-0.1.5/src/napari_brainways/_sample_data.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.4/src/napari_brainways/_tests/test_reader.py` & `napari_brainways-0.1.5/src/napari_brainways/_tests/test_reader.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.4/src/napari_brainways/_tests/test_widget.py` & `napari_brainways-0.1.5/src/napari_brainways/_tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.4/src/napari_brainways/brainways_ui.py` & `napari_brainways-0.1.5/src/napari_brainways/brainways_ui.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.4/src/napari_brainways/conftest.py` & `napari_brainways-0.1.5/src/napari_brainways/conftest.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.4/src/napari_brainways/controllers/_tests/test_affine_2d_controller.py` & `napari_brainways-0.1.5/src/napari_brainways/controllers/_tests/test_affine_2d_controller.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.4/src/napari_brainways/controllers/_tests/test_annotation_viewer_controller.py` & `napari_brainways-0.1.5/src/napari_brainways/controllers/_tests/test_annotation_viewer_controller.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.4/src/napari_brainways/controllers/_tests/test_cell_3d_viewer_controller.py` & `napari_brainways-0.1.5/src/napari_brainways/controllers/_tests/test_cell_3d_viewer_controller.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.4/src/napari_brainways/controllers/_tests/test_tps_controller.py` & `napari_brainways-0.1.5/src/napari_brainways/controllers/_tests/test_tps_controller.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.4/src/napari_brainways/controllers/affine_2d_controller.py` & `napari_brainways-0.1.5/src/napari_brainways/controllers/affine_2d_controller.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.4/src/napari_brainways/controllers/annotation_viewer_controller.py` & `napari_brainways-0.1.5/src/napari_brainways/controllers/annotation_viewer_controller.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.4/src/napari_brainways/controllers/base.py` & `napari_brainways-0.1.5/src/napari_brainways/controllers/base.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.4/src/napari_brainways/controllers/cell_3d_viewer_controller.py` & `napari_brainways-0.1.5/src/napari_brainways/controllers/cell_3d_viewer_controller.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.4/src/napari_brainways/controllers/cell_detector_controller.py` & `napari_brainways-0.1.5/src/napari_brainways/controllers/cell_detector_controller.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.4/src/napari_brainways/controllers/registration_controller.py` & `napari_brainways-0.1.5/src/napari_brainways/controllers/registration_controller.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.4/src/napari_brainways/controllers/tps_controller.py` & `napari_brainways-0.1.5/src/napari_brainways/controllers/tps_controller.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.4/src/napari_brainways/napari.yaml` & `napari_brainways-0.1.5/src/napari_brainways/napari.yaml`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.4/src/napari_brainways/napari_reader.py` & `napari_brainways-0.1.5/src/napari_brainways/napari_reader.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.4/src/napari_brainways/resources/logo.png` & `napari_brainways-0.1.5/src/napari_brainways/resources/logo.png`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.4/src/napari_brainways/test_utils.py` & `napari_brainways-0.1.5/src/napari_brainways/test_utils.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.4/src/napari_brainways/utils.py` & `napari_brainways-0.1.5/src/napari_brainways/utils.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.4/src/napari_brainways/widgets/_tests/test_create_project_dialog.py` & `napari_brainways-0.1.5/src/napari_brainways/widgets/_tests/test_create_project_dialog.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.4/src/napari_brainways/widgets/_tests/test_registration_widget.py` & `napari_brainways-0.1.5/src/napari_brainways/widgets/_tests/test_registration_widget.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.4/src/napari_brainways/widgets/affine_2d_widget.py` & `napari_brainways-0.1.5/src/napari_brainways/widgets/affine_2d_widget.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.4/src/napari_brainways/widgets/cell_detector_widget.py` & `napari_brainways-0.1.5/src/napari_brainways/widgets/cell_detector_widget.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.4/src/napari_brainways/widgets/cell_viewer_widget.py` & `napari_brainways-0.1.5/src/napari_brainways/widgets/cell_viewer_widget.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.4/src/napari_brainways/widgets/create_subject_dialog.py` & `napari_brainways-0.1.5/src/napari_brainways/widgets/create_subject_dialog.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.4/src/napari_brainways/widgets/registration_widget.py` & `napari_brainways-0.1.5/src/napari_brainways/widgets/registration_widget.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.4/src/napari_brainways/widgets/tps_widget.py` & `napari_brainways-0.1.5/src/napari_brainways/widgets/tps_widget.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.4/src/napari_brainways/widgets/workflow_widget.py` & `napari_brainways-0.1.5/src/napari_brainways/widgets/workflow_widget.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,22 +88,22 @@
                 self.project_buttons,
                 self.subject_navigation,
                 self.subject_controls,
             ]
         )
         self.all_widgets.layout().addStretch()
 
-        scroll_area = QScrollArea(self)
-        scroll_area.setWidget(self.all_widgets)
-        scroll_area.setWidgetResizable(True)
-        scroll_area.setAlignment(Qt.AlignmentFlag.AlignTop)
+        self.scroll_area = QScrollArea(self)
+        self.scroll_area.setWidget(self.all_widgets)
+        self.scroll_area.setWidgetResizable(True)
+        self.scroll_area.setAlignment(Qt.AlignmentFlag.AlignTop)
 
         self.setLayout(QVBoxLayout())
         self.layout().setContentsMargins(0, 0, 0, 0)
-        self.layout().addWidget(scroll_area)
+        self.layout().addWidget(self.scroll_area)
 
         self.subject_controls.hide()
 
         # self.setMinimumWidth(400)
         self.setSizePolicy(QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Expanding)
 
     def _stack_widgets(self, widgets) -> QWidget:
@@ -369,14 +369,15 @@
 
     def show_progress_bar(self, max_value: int = 0, label: str = ""):
         self.all_widgets.setEnabled(False)
         self.progress_bar.value = 0
         self.progress_bar.text = label
         self.progress_bar.max = max_value
         self.header_section.show_progress()
+        self.scroll_area.verticalScrollBar().setValue(0)
 
     def hide_progress_bar(self):
         self.all_widgets.setEnabled(True)
         self.header_section.hide_progress()
 
     def update_enabled_steps(self):
         self.step_buttons.update_enabled(self.controller.current_params)
```

### Comparing `napari_brainways-0.1.4/src/napari_brainways.egg-info/PKG-INFO` & `napari_brainways-0.1.5/src/napari_brainways.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-brainways
-Version: 0.1.4
+Version: 0.1.5
 Summary: Brainways UI
 Home-page: https://github.com/bkntr/napari-brainways
 Author: Ben Kantor
 Author-email: benkantor@mail.tau.ac.il
 License: GPL-3.0
 Project-URL: Bug Tracker, https://github.com/bkntr/napari-brainways/issues
 Project-URL: Documentation, https://github.com/bkntr/napari-brainways#README.md
```

### Comparing `napari_brainways-0.1.4/src/napari_brainways.egg-info/SOURCES.txt` & `napari_brainways-0.1.5/src/napari_brainways.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.4/tox.ini` & `napari_brainways-0.1.5/tox.ini`

 * *Files identical despite different names*

