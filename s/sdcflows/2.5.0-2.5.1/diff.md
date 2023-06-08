# Comparing `tmp/sdcflows-2.5.0.tar.gz` & `tmp/sdcflows-2.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdcflows-2.5.0.tar", last modified: Thu Jun  1 18:35:06 2023, max compression
+gzip compressed data, was "sdcflows-2.5.1.tar", last modified: Thu Jun  8 21:11:44 2023, max compression
```

## Comparing `sdcflows-2.5.0.tar` & `sdcflows-2.5.1.tar`

### file list

```diff
@@ -1,268 +1,268 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:35:06.055788 sdcflows-2.5.0/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:35:06.007788 sdcflows-2.5.0/.maint/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1594 2023-06-01 18:34:46.000000 sdcflows-2.5.0/.maint/CONTRIBUTORS.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      567 2023-06-01 18:34:46.000000 sdcflows-2.5.0/.maint/FORMER.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1146 2023-06-01 18:34:46.000000 sdcflows-2.5.0/.maint/MAINTAINERS.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1399 2023-06-01 18:34:46.000000 sdcflows-2.5.0/.maint/PIs.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      642 2023-06-01 18:34:46.000000 sdcflows-2.5.0/.maint/ROADMAP.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9457 2023-06-01 18:34:46.000000 sdcflows-2.5.0/.maint/update_authors.py
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)     1174 2023-06-01 18:34:46.000000 sdcflows-2.5.0/.maint/update_requirements.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    23275 2023-06-01 18:34:46.000000 sdcflows-2.5.0/CHANGES.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      119 2023-06-01 18:34:46.000000 sdcflows-2.5.0/CONTRIBUTING.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11357 2023-06-01 18:34:46.000000 sdcflows-2.5.0/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)      146 2023-06-01 18:34:46.000000 sdcflows-2.5.0/MANIFEST.in
--rw-r--r--   0 circleci  (1001) circleci  (1002)      411 2023-06-01 18:34:46.000000 sdcflows-2.5.0/Makefile
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2308 2023-06-01 18:35:06.055788 sdcflows-2.5.0/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1274 2023-06-01 18:34:46.000000 sdcflows-2.5.0/README.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      218 2023-06-01 18:34:46.000000 sdcflows-2.5.0/min-requirements.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      295 2023-06-01 18:34:46.000000 sdcflows-2.5.0/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      223 2023-06-01 18:34:46.000000 sdcflows-2.5.0/requirements.txt
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:35:06.007788 sdcflows-2.5.0/sdcflows/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      502 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       85 2023-06-01 18:35:05.000000 sdcflows-2.5.0/sdcflows/_version.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:35:06.007788 sdcflows-2.5.0/sdcflows/cli/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/cli/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3266 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/cli/find_estimators.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:35:06.011788 sdcflows-2.5.0/sdcflows/cli/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/cli/tests/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3464 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/cli/tests/test_find_estimators.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3011 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/conftest.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:35:06.015788 sdcflows-2.5.0/sdcflows/data/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/data/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      872 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/data/affine.json
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:35:06.019788 sdcflows-2.5.0/sdcflows/data/flirtsch/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      944 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/data/flirtsch/b02b0.cnf
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1002 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/data/flirtsch/b02b0_1.cnf
--rw-r--r--   0 circleci  (1001) circleci  (1002)      997 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/data/flirtsch/b02b0_2.cnf
--rw-r--r--   0 circleci  (1001) circleci  (1002)      997 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/data/flirtsch/b02b0_4.cnf
--rw-r--r--   0 circleci  (1001) circleci  (1002)      858 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/data/flirtsch/b02b0_quick.cnf
--rw-r--r--   0 circleci  (1001) circleci  (1002)      824 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/data/fmap-any_registration.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      826 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/data/fmap-any_registration_testing.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)  5801500 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/data/fmap_atlas.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)      193 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/data/fmap_atlas_2_MNI152NLin2009cAsym_affine.mat
--rw-r--r--   0 circleci  (1001) circleci  (1002)      960 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/data/sd_syn.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      978 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/data/sd_syn_sloppy.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      856 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/data/translation_rigid.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17569 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/fieldmaps.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:35:06.019788 sdcflows-2.5.0/sdcflows/interfaces/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/interfaces/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4729 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/interfaces/brainmask.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    23807 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/interfaces/bspline.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4440 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/interfaces/epi.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13361 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/interfaces/fmap.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5483 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/interfaces/reportlets.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:35:06.023788 sdcflows-2.5.0/sdcflows/interfaces/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/interfaces/tests/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4506 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/interfaces/tests/test_bspline.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1482 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/interfaces/tests/test_epi.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1513 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/interfaces/tests/test_fmap.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1770 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/interfaces/tests/test_reportlets.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4243 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/interfaces/tests/test_utils.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18032 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/interfaces/utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:35:06.023788 sdcflows-2.5.0/sdcflows/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:35:06.027788 sdcflows-2.5.0/sdcflows/tests/data/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:35:06.027788 sdcflows-2.5.0/sdcflows/tests/data/dsA/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      256 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsA/dataset_description.json
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:35:06.003788 sdcflows-2.5.0/sdcflows/tests/data/dsA/sub-01/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:35:06.027788 sdcflows-2.5.0/sdcflows/tests/data/dsA/sub-01/anat/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsA/sub-01/anat/sub-01_FLAIR.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsA/sub-01/anat/sub-01_T1w.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsA/sub-01/anat/sub-01_T2w.nii.gz
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:35:06.031788 sdcflows-2.5.0/sdcflows/tests/data/dsA/sub-01/dwi/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsA/sub-01/dwi/sub-01_dir-AP_dwi.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)       69 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsA/sub-01/dwi/sub-01_dir-AP_sbref.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsA/sub-01/dwi/sub-01_dir-AP_sbref.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsA/sub-01/dwi/sub-01_dir-LR_dwi.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)       68 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsA/sub-01/dwi/sub-01_dir-LR_sbref.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsA/sub-01/dwi/sub-01_dir-LR_sbref.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsA/sub-01/dwi/sub-01_dir-PA_dwi.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)       68 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsA/sub-01/dwi/sub-01_dir-PA_sbref.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsA/sub-01/dwi/sub-01_dir-PA_sbref.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsA/sub-01/dwi/sub-01_dir-RL_dwi.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)       69 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsA/sub-01/dwi/sub-01_dir-RL_sbref.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsA/sub-01/dwi/sub-01_dir-RL_sbref.nii.gz
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:35:06.035788 sdcflows-2.5.0/sdcflows/tests/data/dsA/sub-01/fmap/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      268 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_acq-single_dir-PA_epi.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_acq-single_dir-PA_epi.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)       63 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_dir-AP_epi.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_dir-AP_epi.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)       62 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_dir-LR_epi.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_dir-LR_epi.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)       62 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_dir-PA_epi.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_dir-PA_epi.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)       63 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_dir-RL_epi.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_dir-RL_epi.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)       21 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_fieldmap.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_fieldmap.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_magnitude.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_magnitude1.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_magnitude2.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)       22 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_phase1.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_phase1.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)       24 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_phase2.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_phase2.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)       48 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_phasediff.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_phasediff.nii.gz
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:35:06.035788 sdcflows-2.5.0/sdcflows/tests/data/dsA/sub-01/func/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsA/sub-01/func/sub-01_task-rest_bold.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsA/sub-01/func/sub-01_task-rest_sbref.nii.gz
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:35:06.035788 sdcflows-2.5.0/sdcflows/tests/data/dsB/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      270 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsB/dataset_description.json
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:35:06.003788 sdcflows-2.5.0/sdcflows/tests/data/dsB/sub-01/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:35:06.003788 sdcflows-2.5.0/sdcflows/tests/data/dsB/sub-01/ses-1/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:35:06.039788 sdcflows-2.5.0/sdcflows/tests/data/dsB/sub-01/ses-1/anat/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsB/sub-01/ses-1/anat/sub-01_ses-1_FLAIR.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsB/sub-01/ses-1/anat/sub-01_ses-1_T1w.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsB/sub-01/ses-1/anat/sub-01_ses-1_T2w.nii.gz
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:35:06.039788 sdcflows-2.5.0/sdcflows/tests/data/dsB/sub-01/ses-1/dwi/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsB/sub-01/ses-1/dwi/sub-01_ses-1_dir-AP_dwi.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)       69 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsB/sub-01/ses-1/dwi/sub-01_ses-1_dir-AP_sbref.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsB/sub-01/ses-1/dwi/sub-01_ses-1_dir-AP_sbref.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsB/sub-01/ses-1/dwi/sub-01_ses-1_dir-LR_dwi.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)       68 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsB/sub-01/ses-1/dwi/sub-01_ses-1_dir-LR_sbref.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsB/sub-01/ses-1/dwi/sub-01_ses-1_dir-LR_sbref.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsB/sub-01/ses-1/dwi/sub-01_ses-1_dir-PA_dwi.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)       68 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsB/sub-01/ses-1/dwi/sub-01_ses-1_dir-PA_sbref.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsB/sub-01/ses-1/dwi/sub-01_ses-1_dir-PA_sbref.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsB/sub-01/ses-1/dwi/sub-01_ses-1_dir-RL_dwi.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)       69 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsB/sub-01/ses-1/dwi/sub-01_ses-1_dir-RL_sbref.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsB/sub-01/ses-1/dwi/sub-01_ses-1_dir-RL_sbref.nii.gz
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:35:06.043788 sdcflows-2.5.0/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      317 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_acq-single_dir-PA_epi.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_acq-single_dir-PA_epi.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)       63 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_dir-AP_epi.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_dir-AP_epi.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)       62 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_dir-LR_epi.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_dir-LR_epi.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)       62 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_dir-PA_epi.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_dir-PA_epi.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)       63 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_dir-RL_epi.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_dir-RL_epi.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)       21 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_fieldmap.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_fieldmap.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_magnitude.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_magnitude1.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_magnitude2.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)       22 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_phase1.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_phase1.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)       24 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_phase2.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_phase2.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)       48 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_phasediff.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_phasediff.nii.gz
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:35:06.043788 sdcflows-2.5.0/sdcflows/tests/data/dsB/sub-01/ses-1/func/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsB/sub-01/ses-1/func/sub-01_ses-1_task-rest_bold.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsB/sub-01/ses-1/func/sub-01_ses-1_task-rest_sbref.nii.gz
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:35:06.043788 sdcflows-2.5.0/sdcflows/tests/data/dsC/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      256 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsC/dataset_description.json
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:35:06.003788 sdcflows-2.5.0/sdcflows/tests/data/dsC/sub-01/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:35:06.043788 sdcflows-2.5.0/sdcflows/tests/data/dsC/sub-01/anat/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsC/sub-01/anat/sub-01_FLAIR.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsC/sub-01/anat/sub-01_T1w.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsC/sub-01/anat/sub-01_T2w.nii.gz
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:35:06.047788 sdcflows-2.5.0/sdcflows/tests/data/dsC/sub-01/dwi/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsC/sub-01/dwi/sub-01_dir-AP_dwi.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)       69 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsC/sub-01/dwi/sub-01_dir-AP_sbref.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsC/sub-01/dwi/sub-01_dir-AP_sbref.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsC/sub-01/dwi/sub-01_dir-LR_dwi.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)       68 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsC/sub-01/dwi/sub-01_dir-LR_sbref.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsC/sub-01/dwi/sub-01_dir-LR_sbref.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsC/sub-01/dwi/sub-01_dir-PA_dwi.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)       68 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsC/sub-01/dwi/sub-01_dir-PA_sbref.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsC/sub-01/dwi/sub-01_dir-PA_sbref.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsC/sub-01/dwi/sub-01_dir-RL_dwi.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)       69 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsC/sub-01/dwi/sub-01_dir-RL_sbref.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsC/sub-01/dwi/sub-01_dir-RL_sbref.nii.gz
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:35:06.047788 sdcflows-2.5.0/sdcflows/tests/data/dsC/sub-01/fmap/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      268 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_acq-single_dir-PA_epi.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_acq-single_dir-PA_epi.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)       99 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_dir-AP_epi.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_dir-AP_epi.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)       98 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_dir-LR_epi.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_dir-LR_epi.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)       98 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_dir-PA_epi.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_dir-PA_epi.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)       99 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_dir-RL_epi.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_dir-RL_epi.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)       21 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_fieldmap.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_fieldmap.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_magnitude.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_magnitude1.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_magnitude2.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)       22 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_phase1.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_phase1.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)       24 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_phase2.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_phase2.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)       48 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_phasediff.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_phasediff.nii.gz
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:35:06.047788 sdcflows-2.5.0/sdcflows/tests/data/dsC/sub-01/func/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsC/sub-01/func/sub-01_task-rest_bold.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsC/sub-01/func/sub-01_task-rest_sbref.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)       83 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/dsC/task-rest_bold.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)  1954195 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/epi.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2302 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/field-coeff-tests.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)    29820 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/topup-coeff-fixed.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)    29726 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/topup-coeff.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)  2210404 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/data/topup-field.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11243 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/test_fieldmaps.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6003 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/test_transform.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2110 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/tests/test_version.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16934 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/transform.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:35:06.051788 sdcflows-2.5.0/sdcflows/utils/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/utils/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6762 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/utils/bimap.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10294 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/utils/epimanip.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2251 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/utils/misc.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5069 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/utils/phasemanip.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:35:06.051788 sdcflows-2.5.0/sdcflows/utils/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/utils/tests/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1460 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/utils/tests/test_misc.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1850 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/utils/tests/test_phasemanip.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4293 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/utils/tests/test_tools.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9248 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/utils/tests/test_wrangler.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10357 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/utils/tools.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    22975 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/utils/wrangler.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:35:06.051788 sdcflows-2.5.0/sdcflows/viz/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/viz/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4092 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/viz/utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:35:06.051788 sdcflows-2.5.0/sdcflows/workflows/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/workflows/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3747 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/workflows/ancillary.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:35:06.051788 sdcflows-2.5.0/sdcflows/workflows/apply/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/workflows/apply/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6544 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/workflows/apply/correction.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5286 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/workflows/apply/registration.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:35:06.051788 sdcflows-2.5.0/sdcflows/workflows/apply/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/workflows/apply/tests/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    30980 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/workflows/apply/tests/fieldcoeff.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5277 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/workflows/apply/tests/test_correction.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4362 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/workflows/apply/tests/test_registration.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6275 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/workflows/base.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:35:06.051788 sdcflows-2.5.0/sdcflows/workflows/fit/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/workflows/fit/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13571 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/workflows/fit/fieldmap.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16449 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/workflows/fit/pepolar.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    24995 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/workflows/fit/syn.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:35:06.055788 sdcflows-2.5.0/sdcflows/workflows/fit/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/workflows/fit/tests/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1727 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/workflows/fit/tests/test_fit.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3179 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/workflows/fit/tests/test_pepolar.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3946 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/workflows/fit/tests/test_phdiff.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6807 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/workflows/fit/tests/test_syn.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9632 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/workflows/outputs.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:35:06.055788 sdcflows-2.5.0/sdcflows/workflows/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/workflows/tests/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3379 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/workflows/tests/test_ancillary.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2710 2023-06-01 18:34:46.000000 sdcflows-2.5.0/sdcflows/workflows/tests/test_base.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:35:06.007788 sdcflows-2.5.0/sdcflows.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2308 2023-06-01 18:35:05.000000 sdcflows-2.5.0/sdcflows.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10864 2023-06-01 18:35:05.000000 sdcflows-2.5.0/sdcflows.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-06-01 18:35:05.000000 sdcflows-2.5.0/sdcflows.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       79 2023-06-01 18:35:05.000000 sdcflows-2.5.0/sdcflows.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      638 2023-06-01 18:35:05.000000 sdcflows-2.5.0/sdcflows.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        9 2023-06-01 18:35:05.000000 sdcflows-2.5.0/sdcflows.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-06-01 18:35:05.000000 sdcflows-2.5.0/sdcflows.egg-info/zip-safe
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2336 2023-06-01 18:35:06.055788 sdcflows-2.5.0/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)      309 2023-06-01 18:34:46.000000 sdcflows-2.5.0/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 18:35:06.055788 sdcflows-2.5.0/tools/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      300 2023-06-01 18:34:46.000000 sdcflows-2.5.0/tools/cache_templateflow.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:44.828316 sdcflows-2.5.1/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:44.780315 sdcflows-2.5.1/.maint/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1594 2023-06-08 21:11:26.000000 sdcflows-2.5.1/.maint/CONTRIBUTORS.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      567 2023-06-08 21:11:26.000000 sdcflows-2.5.1/.maint/FORMER.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1146 2023-06-08 21:11:26.000000 sdcflows-2.5.1/.maint/MAINTAINERS.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1399 2023-06-08 21:11:26.000000 sdcflows-2.5.1/.maint/PIs.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      642 2023-06-08 21:11:26.000000 sdcflows-2.5.1/.maint/ROADMAP.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9457 2023-06-08 21:11:26.000000 sdcflows-2.5.1/.maint/update_authors.py
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)     1174 2023-06-08 21:11:26.000000 sdcflows-2.5.1/.maint/update_requirements.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    23558 2023-06-08 21:11:26.000000 sdcflows-2.5.1/CHANGES.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      119 2023-06-08 21:11:26.000000 sdcflows-2.5.1/CONTRIBUTING.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11357 2023-06-08 21:11:26.000000 sdcflows-2.5.1/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      146 2023-06-08 21:11:26.000000 sdcflows-2.5.1/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      411 2023-06-08 21:11:26.000000 sdcflows-2.5.1/Makefile
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2308 2023-06-08 21:11:44.828316 sdcflows-2.5.1/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1274 2023-06-08 21:11:26.000000 sdcflows-2.5.1/README.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      218 2023-06-08 21:11:26.000000 sdcflows-2.5.1/min-requirements.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      295 2023-06-08 21:11:26.000000 sdcflows-2.5.1/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      223 2023-06-08 21:11:26.000000 sdcflows-2.5.1/requirements.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:44.780315 sdcflows-2.5.1/sdcflows/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      502 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       85 2023-06-08 21:11:44.000000 sdcflows-2.5.1/sdcflows/_version.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:44.784315 sdcflows-2.5.1/sdcflows/cli/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/cli/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3266 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/cli/find_estimators.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:44.784315 sdcflows-2.5.1/sdcflows/cli/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/cli/tests/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3464 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/cli/tests/test_find_estimators.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3011 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/conftest.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:44.792315 sdcflows-2.5.1/sdcflows/data/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/data/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      872 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/data/affine.json
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:44.792315 sdcflows-2.5.1/sdcflows/data/flirtsch/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      944 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/data/flirtsch/b02b0.cnf
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1002 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/data/flirtsch/b02b0_1.cnf
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      997 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/data/flirtsch/b02b0_2.cnf
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      997 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/data/flirtsch/b02b0_4.cnf
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      858 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/data/flirtsch/b02b0_quick.cnf
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      824 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/data/fmap-any_registration.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      826 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/data/fmap-any_registration_testing.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)  5801500 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/data/fmap_atlas.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      193 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/data/fmap_atlas_2_MNI152NLin2009cAsym_affine.mat
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      960 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/data/sd_syn.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      978 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/data/sd_syn_sloppy.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      856 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/data/translation_rigid.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17569 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/fieldmaps.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:44.792315 sdcflows-2.5.1/sdcflows/interfaces/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/interfaces/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4729 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/interfaces/brainmask.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    24397 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/interfaces/bspline.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4440 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/interfaces/epi.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13361 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/interfaces/fmap.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5483 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/interfaces/reportlets.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:44.796315 sdcflows-2.5.1/sdcflows/interfaces/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/interfaces/tests/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4506 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/interfaces/tests/test_bspline.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1482 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/interfaces/tests/test_epi.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1513 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/interfaces/tests/test_fmap.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1770 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/interfaces/tests/test_reportlets.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4243 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/interfaces/tests/test_utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18032 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/interfaces/utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:44.796315 sdcflows-2.5.1/sdcflows/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:44.800315 sdcflows-2.5.1/sdcflows/tests/data/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:44.800315 sdcflows-2.5.1/sdcflows/tests/data/dsA/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      256 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsA/dataset_description.json
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:44.772315 sdcflows-2.5.1/sdcflows/tests/data/dsA/sub-01/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:44.800315 sdcflows-2.5.1/sdcflows/tests/data/dsA/sub-01/anat/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsA/sub-01/anat/sub-01_FLAIR.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsA/sub-01/anat/sub-01_T1w.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsA/sub-01/anat/sub-01_T2w.nii.gz
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:44.804315 sdcflows-2.5.1/sdcflows/tests/data/dsA/sub-01/dwi/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsA/sub-01/dwi/sub-01_dir-AP_dwi.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       69 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsA/sub-01/dwi/sub-01_dir-AP_sbref.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsA/sub-01/dwi/sub-01_dir-AP_sbref.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsA/sub-01/dwi/sub-01_dir-LR_dwi.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       68 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsA/sub-01/dwi/sub-01_dir-LR_sbref.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsA/sub-01/dwi/sub-01_dir-LR_sbref.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsA/sub-01/dwi/sub-01_dir-PA_dwi.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       68 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsA/sub-01/dwi/sub-01_dir-PA_sbref.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsA/sub-01/dwi/sub-01_dir-PA_sbref.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsA/sub-01/dwi/sub-01_dir-RL_dwi.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       69 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsA/sub-01/dwi/sub-01_dir-RL_sbref.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsA/sub-01/dwi/sub-01_dir-RL_sbref.nii.gz
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:44.808315 sdcflows-2.5.1/sdcflows/tests/data/dsA/sub-01/fmap/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      268 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_acq-single_dir-PA_epi.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_acq-single_dir-PA_epi.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       63 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_dir-AP_epi.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_dir-AP_epi.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       62 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_dir-LR_epi.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_dir-LR_epi.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       62 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_dir-PA_epi.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_dir-PA_epi.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       63 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_dir-RL_epi.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_dir-RL_epi.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       21 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_fieldmap.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_fieldmap.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_magnitude.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_magnitude1.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_magnitude2.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       22 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_phase1.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_phase1.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       24 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_phase2.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_phase2.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       48 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_phasediff.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_phasediff.nii.gz
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:44.808315 sdcflows-2.5.1/sdcflows/tests/data/dsA/sub-01/func/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsA/sub-01/func/sub-01_task-rest_bold.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsA/sub-01/func/sub-01_task-rest_sbref.nii.gz
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:44.808315 sdcflows-2.5.1/sdcflows/tests/data/dsB/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      270 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsB/dataset_description.json
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:44.772315 sdcflows-2.5.1/sdcflows/tests/data/dsB/sub-01/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:44.772315 sdcflows-2.5.1/sdcflows/tests/data/dsB/sub-01/ses-1/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:44.808315 sdcflows-2.5.1/sdcflows/tests/data/dsB/sub-01/ses-1/anat/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsB/sub-01/ses-1/anat/sub-01_ses-1_FLAIR.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsB/sub-01/ses-1/anat/sub-01_ses-1_T1w.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsB/sub-01/ses-1/anat/sub-01_ses-1_T2w.nii.gz
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:44.812315 sdcflows-2.5.1/sdcflows/tests/data/dsB/sub-01/ses-1/dwi/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsB/sub-01/ses-1/dwi/sub-01_ses-1_dir-AP_dwi.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       69 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsB/sub-01/ses-1/dwi/sub-01_ses-1_dir-AP_sbref.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsB/sub-01/ses-1/dwi/sub-01_ses-1_dir-AP_sbref.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsB/sub-01/ses-1/dwi/sub-01_ses-1_dir-LR_dwi.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       68 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsB/sub-01/ses-1/dwi/sub-01_ses-1_dir-LR_sbref.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsB/sub-01/ses-1/dwi/sub-01_ses-1_dir-LR_sbref.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsB/sub-01/ses-1/dwi/sub-01_ses-1_dir-PA_dwi.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       68 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsB/sub-01/ses-1/dwi/sub-01_ses-1_dir-PA_sbref.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsB/sub-01/ses-1/dwi/sub-01_ses-1_dir-PA_sbref.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsB/sub-01/ses-1/dwi/sub-01_ses-1_dir-RL_dwi.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       69 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsB/sub-01/ses-1/dwi/sub-01_ses-1_dir-RL_sbref.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsB/sub-01/ses-1/dwi/sub-01_ses-1_dir-RL_sbref.nii.gz
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:44.816316 sdcflows-2.5.1/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      317 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_acq-single_dir-PA_epi.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_acq-single_dir-PA_epi.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       63 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_dir-AP_epi.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_dir-AP_epi.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       62 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_dir-LR_epi.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_dir-LR_epi.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       62 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_dir-PA_epi.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_dir-PA_epi.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       63 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_dir-RL_epi.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_dir-RL_epi.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       21 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_fieldmap.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_fieldmap.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_magnitude.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_magnitude1.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_magnitude2.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       22 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_phase1.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_phase1.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       24 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_phase2.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_phase2.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       48 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_phasediff.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_phasediff.nii.gz
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:44.816316 sdcflows-2.5.1/sdcflows/tests/data/dsB/sub-01/ses-1/func/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsB/sub-01/ses-1/func/sub-01_ses-1_task-rest_bold.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsB/sub-01/ses-1/func/sub-01_ses-1_task-rest_sbref.nii.gz
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:44.816316 sdcflows-2.5.1/sdcflows/tests/data/dsC/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      256 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsC/dataset_description.json
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:44.776315 sdcflows-2.5.1/sdcflows/tests/data/dsC/sub-01/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:44.816316 sdcflows-2.5.1/sdcflows/tests/data/dsC/sub-01/anat/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsC/sub-01/anat/sub-01_FLAIR.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsC/sub-01/anat/sub-01_T1w.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsC/sub-01/anat/sub-01_T2w.nii.gz
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:44.816316 sdcflows-2.5.1/sdcflows/tests/data/dsC/sub-01/dwi/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsC/sub-01/dwi/sub-01_dir-AP_dwi.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       69 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsC/sub-01/dwi/sub-01_dir-AP_sbref.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsC/sub-01/dwi/sub-01_dir-AP_sbref.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsC/sub-01/dwi/sub-01_dir-LR_dwi.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       68 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsC/sub-01/dwi/sub-01_dir-LR_sbref.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsC/sub-01/dwi/sub-01_dir-LR_sbref.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsC/sub-01/dwi/sub-01_dir-PA_dwi.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       68 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsC/sub-01/dwi/sub-01_dir-PA_sbref.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsC/sub-01/dwi/sub-01_dir-PA_sbref.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsC/sub-01/dwi/sub-01_dir-RL_dwi.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       69 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsC/sub-01/dwi/sub-01_dir-RL_sbref.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsC/sub-01/dwi/sub-01_dir-RL_sbref.nii.gz
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:44.820315 sdcflows-2.5.1/sdcflows/tests/data/dsC/sub-01/fmap/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      268 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_acq-single_dir-PA_epi.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_acq-single_dir-PA_epi.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       99 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_dir-AP_epi.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_dir-AP_epi.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       98 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_dir-LR_epi.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_dir-LR_epi.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       98 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_dir-PA_epi.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_dir-PA_epi.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       99 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_dir-RL_epi.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_dir-RL_epi.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       21 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_fieldmap.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_fieldmap.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_magnitude.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_magnitude1.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_magnitude2.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       22 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_phase1.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_phase1.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       24 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_phase2.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_phase2.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       48 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_phasediff.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_phasediff.nii.gz
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:44.820315 sdcflows-2.5.1/sdcflows/tests/data/dsC/sub-01/func/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsC/sub-01/func/sub-01_task-rest_bold.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsC/sub-01/func/sub-01_task-rest_sbref.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       83 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/dsC/task-rest_bold.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)  1954195 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/epi.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2302 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/field-coeff-tests.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    29820 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/topup-coeff-fixed.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    29726 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/topup-coeff.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)  2210404 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/data/topup-field.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11243 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/test_fieldmaps.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6003 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/test_transform.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2110 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/tests/test_version.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16934 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/transform.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:44.820315 sdcflows-2.5.1/sdcflows/utils/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/utils/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6762 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/utils/bimap.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10294 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/utils/epimanip.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2251 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/utils/misc.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5069 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/utils/phasemanip.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:44.824315 sdcflows-2.5.1/sdcflows/utils/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/utils/tests/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1460 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/utils/tests/test_misc.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1850 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/utils/tests/test_phasemanip.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4293 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/utils/tests/test_tools.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12530 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/utils/tests/test_wrangler.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10357 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/utils/tools.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    25298 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/utils/wrangler.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:44.824315 sdcflows-2.5.1/sdcflows/viz/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/viz/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4092 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/viz/utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:44.824315 sdcflows-2.5.1/sdcflows/workflows/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/workflows/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3747 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/workflows/ancillary.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:44.824315 sdcflows-2.5.1/sdcflows/workflows/apply/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/workflows/apply/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6544 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/workflows/apply/correction.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5286 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/workflows/apply/registration.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:44.824315 sdcflows-2.5.1/sdcflows/workflows/apply/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/workflows/apply/tests/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    30980 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/workflows/apply/tests/fieldcoeff.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5277 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/workflows/apply/tests/test_correction.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4362 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/workflows/apply/tests/test_registration.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6275 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/workflows/base.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:44.824315 sdcflows-2.5.1/sdcflows/workflows/fit/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/workflows/fit/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13571 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/workflows/fit/fieldmap.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16449 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/workflows/fit/pepolar.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    24995 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/workflows/fit/syn.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:44.824315 sdcflows-2.5.1/sdcflows/workflows/fit/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/workflows/fit/tests/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1727 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/workflows/fit/tests/test_fit.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3179 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/workflows/fit/tests/test_pepolar.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3946 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/workflows/fit/tests/test_phdiff.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6807 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/workflows/fit/tests/test_syn.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9632 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/workflows/outputs.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:44.828316 sdcflows-2.5.1/sdcflows/workflows/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/workflows/tests/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3379 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/workflows/tests/test_ancillary.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2710 2023-06-08 21:11:26.000000 sdcflows-2.5.1/sdcflows/workflows/tests/test_base.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:44.784315 sdcflows-2.5.1/sdcflows.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2308 2023-06-08 21:11:44.000000 sdcflows-2.5.1/sdcflows.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10864 2023-06-08 21:11:44.000000 sdcflows-2.5.1/sdcflows.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-06-08 21:11:44.000000 sdcflows-2.5.1/sdcflows.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       79 2023-06-08 21:11:44.000000 sdcflows-2.5.1/sdcflows.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      638 2023-06-08 21:11:44.000000 sdcflows-2.5.1/sdcflows.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        9 2023-06-08 21:11:44.000000 sdcflows-2.5.1/sdcflows.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-06-08 21:11:44.000000 sdcflows-2.5.1/sdcflows.egg-info/zip-safe
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2336 2023-06-08 21:11:44.828316 sdcflows-2.5.1/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      309 2023-06-08 21:11:26.000000 sdcflows-2.5.1/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:11:44.828316 sdcflows-2.5.1/tools/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      300 2023-06-08 21:11:26.000000 sdcflows-2.5.1/tools/cache_templateflow.py
```

### Comparing `sdcflows-2.5.0/.maint/CONTRIBUTORS.md` & `sdcflows-2.5.1/.maint/CONTRIBUTORS.md`

 * *Files identical despite different names*

### Comparing `sdcflows-2.5.0/.maint/FORMER.md` & `sdcflows-2.5.1/.maint/FORMER.md`

 * *Files identical despite different names*

### Comparing `sdcflows-2.5.0/.maint/MAINTAINERS.md` & `sdcflows-2.5.1/.maint/MAINTAINERS.md`

 * *Files identical despite different names*

### Comparing `sdcflows-2.5.0/.maint/PIs.md` & `sdcflows-2.5.1/.maint/PIs.md`

 * *Files identical despite different names*

### Comparing `sdcflows-2.5.0/.maint/ROADMAP.md` & `sdcflows-2.5.1/.maint/ROADMAP.md`

 * *Files identical despite different names*

### Comparing `sdcflows-2.5.0/.maint/update_authors.py` & `sdcflows-2.5.1/.maint/update_authors.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.5.0/.maint/update_requirements.py` & `sdcflows-2.5.1/.maint/update_requirements.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.5.0/CHANGES.rst` & `sdcflows-2.5.1/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+2.5.1 (June 08, 2023)
+=====================
+Bug-fix release in the 2.5.x series.
+
+* FIX: Use ``lsqr`` solver for spline fit, rerun on extreme values (#366)
+* FIX: Ensure metadata is not present in entity query (#367)
+* RF/FIX: Prioritize sbref and shortest echo for SyN-SDC (#364)
+
+
 2.5.0 (June 01, 2023)
 =====================
 New feature release in the 2.5.x series.
 
 This release includes a number of changes to default behaviors.
 SyN-SDC will be performed per-BOLD/DWI image, unless specified otherwise with
 ``B0FieldIdentifier``\s, and may now be specified with T2w images as anatomical
```

### Comparing `sdcflows-2.5.0/LICENSE` & `sdcflows-2.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sdcflows-2.5.0/PKG-INFO` & `sdcflows-2.5.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdcflows
-Version: 2.5.0
+Version: 2.5.1
 Summary: Susceptibility Distortion Correction (SDC) workflows for EPI MR schemes.
 Home-page: https://www.nipreps.org/sdcflows
 Author: The SDCflows developers
 Author-email: nipreps@gmail.com
 License: Apache-2.0
 Project-URL: Documentation, https://www.nipreps.org/sdcflows
 Project-URL: GitHub, https://github.com/nipreps/sdcflows
```

### Comparing `sdcflows-2.5.0/README.rst` & `sdcflows-2.5.1/README.rst`

 * *Files identical despite different names*

### Comparing `sdcflows-2.5.0/sdcflows/cli/find_estimators.py` & `sdcflows-2.5.1/sdcflows/cli/find_estimators.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.5.0/sdcflows/cli/tests/test_find_estimators.py` & `sdcflows-2.5.1/sdcflows/cli/tests/test_find_estimators.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.5.0/sdcflows/conftest.py` & `sdcflows-2.5.1/sdcflows/conftest.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.5.0/sdcflows/data/affine.json` & `sdcflows-2.5.1/sdcflows/data/affine.json`

 * *Files identical despite different names*

### Comparing `sdcflows-2.5.0/sdcflows/data/flirtsch/b02b0.cnf` & `sdcflows-2.5.1/sdcflows/data/flirtsch/b02b0.cnf`

 * *Files identical despite different names*

### Comparing `sdcflows-2.5.0/sdcflows/data/flirtsch/b02b0_1.cnf` & `sdcflows-2.5.1/sdcflows/data/flirtsch/b02b0_1.cnf`

 * *Files identical despite different names*

### Comparing `sdcflows-2.5.0/sdcflows/data/flirtsch/b02b0_2.cnf` & `sdcflows-2.5.1/sdcflows/data/flirtsch/b02b0_2.cnf`

 * *Files identical despite different names*

### Comparing `sdcflows-2.5.0/sdcflows/data/flirtsch/b02b0_4.cnf` & `sdcflows-2.5.1/sdcflows/data/flirtsch/b02b0_4.cnf`

 * *Files identical despite different names*

### Comparing `sdcflows-2.5.0/sdcflows/data/flirtsch/b02b0_quick.cnf` & `sdcflows-2.5.1/sdcflows/data/flirtsch/b02b0_quick.cnf`

 * *Files identical despite different names*

### Comparing `sdcflows-2.5.0/sdcflows/data/fmap-any_registration.json` & `sdcflows-2.5.1/sdcflows/data/fmap-any_registration.json`

 * *Files identical despite different names*

### Comparing `sdcflows-2.5.0/sdcflows/data/fmap-any_registration_testing.json` & `sdcflows-2.5.1/sdcflows/data/fmap-any_registration_testing.json`

 * *Files identical despite different names*

### Comparing `sdcflows-2.5.0/sdcflows/data/fmap_atlas.nii.gz` & `sdcflows-2.5.1/sdcflows/data/fmap_atlas.nii.gz`

 * *Files identical despite different names*

### Comparing `sdcflows-2.5.0/sdcflows/data/sd_syn.json` & `sdcflows-2.5.1/sdcflows/data/sd_syn.json`

 * *Files identical despite different names*

### Comparing `sdcflows-2.5.0/sdcflows/data/sd_syn_sloppy.json` & `sdcflows-2.5.1/sdcflows/data/sd_syn_sloppy.json`

 * *Files identical despite different names*

### Comparing `sdcflows-2.5.0/sdcflows/data/translation_rigid.json` & `sdcflows-2.5.1/sdcflows/data/translation_rigid.json`

 * *Files identical despite different names*

### Comparing `sdcflows-2.5.0/sdcflows/fieldmaps.py` & `sdcflows-2.5.1/sdcflows/fieldmaps.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.5.0/sdcflows/interfaces/brainmask.py` & `sdcflows-2.5.1/sdcflows/interfaces/brainmask.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.5.0/sdcflows/interfaces/bspline.py` & `sdcflows-2.5.1/sdcflows/interfaces/bspline.py`

 * *Files 2% similar despite different names*

```diff
@@ -204,16 +204,28 @@
         LOGGER.info(
             f"Approximating B-Splines grids ({', '.join(bs_grids_str)} [knots]) on a grid of "
             f"{'x'.join(str(s) for s in fmapnii.shape)} ({np.prod(fmapnii.shape)}) voxels,"
             f" of which {mask.sum()} fall within the mask."
         )
 
         # Fit the model
-        model = lm.Ridge(alpha=self.inputs.ridge_alpha, fit_intercept=False)
-        model.fit(colmat[mask.reshape(-1), :], data[mask])
+        model = lm.Ridge(alpha=self.inputs.ridge_alpha, fit_intercept=False, solver='lsqr')
+        for attempt in range(3):
+            model.fit(colmat[mask.reshape(-1), :], data[mask])
+            extreme = np.abs(model.coef_).max()
+            LOGGER.debug(f"Model fit attempt {attempt}: max(|coeffs|) = {extreme}")
+            # Normal values seem to be ~1e2, bad ~1e8. May want to tweak this if
+            # these distributions are wider than I think.
+            if extreme < 1e4:
+                break
+        else:
+            raise RuntimeError(
+                f"Spline fit of input file {self.inputs.in_data} failed. "
+                f"Extreme value {extreme:.2e} detected in spline coefficients."
+            )
 
         # Store coefficients
         index = 0
         self._results["out_coeff"] = []
         for i, bsl in enumerate(bs_grids):
             n = bsl.dataobj.size
             out_level = out_name.replace("_field.", f"_coeff{i:03}.")
```

### Comparing `sdcflows-2.5.0/sdcflows/interfaces/epi.py` & `sdcflows-2.5.1/sdcflows/interfaces/epi.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.5.0/sdcflows/interfaces/fmap.py` & `sdcflows-2.5.1/sdcflows/interfaces/fmap.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.5.0/sdcflows/interfaces/reportlets.py` & `sdcflows-2.5.1/sdcflows/interfaces/reportlets.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.5.0/sdcflows/interfaces/tests/test_bspline.py` & `sdcflows-2.5.1/sdcflows/interfaces/tests/test_bspline.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.5.0/sdcflows/interfaces/tests/test_epi.py` & `sdcflows-2.5.1/sdcflows/interfaces/tests/test_epi.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.5.0/sdcflows/interfaces/tests/test_fmap.py` & `sdcflows-2.5.1/sdcflows/interfaces/tests/test_fmap.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.5.0/sdcflows/interfaces/tests/test_reportlets.py` & `sdcflows-2.5.1/sdcflows/interfaces/tests/test_reportlets.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.5.0/sdcflows/interfaces/tests/test_utils.py` & `sdcflows-2.5.1/sdcflows/interfaces/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.5.0/sdcflows/interfaces/utils.py` & `sdcflows-2.5.1/sdcflows/interfaces/utils.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.5.0/sdcflows/tests/data/epi.nii.gz` & `sdcflows-2.5.1/sdcflows/tests/data/epi.nii.gz`

 * *Files identical despite different names*

### Comparing `sdcflows-2.5.0/sdcflows/tests/data/field-coeff-tests.nii.gz` & `sdcflows-2.5.1/sdcflows/tests/data/field-coeff-tests.nii.gz`

 * *Files identical despite different names*

### Comparing `sdcflows-2.5.0/sdcflows/tests/data/topup-coeff-fixed.nii.gz` & `sdcflows-2.5.1/sdcflows/tests/data/topup-coeff-fixed.nii.gz`

 * *Files identical despite different names*

### Comparing `sdcflows-2.5.0/sdcflows/tests/data/topup-coeff.nii.gz` & `sdcflows-2.5.1/sdcflows/tests/data/topup-coeff.nii.gz`

 * *Files identical despite different names*

### Comparing `sdcflows-2.5.0/sdcflows/tests/data/topup-field.nii.gz` & `sdcflows-2.5.1/sdcflows/tests/data/topup-field.nii.gz`

 * *Files identical despite different names*

### Comparing `sdcflows-2.5.0/sdcflows/tests/test_fieldmaps.py` & `sdcflows-2.5.1/sdcflows/tests/test_fieldmaps.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.5.0/sdcflows/tests/test_transform.py` & `sdcflows-2.5.1/sdcflows/tests/test_transform.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.5.0/sdcflows/tests/test_version.py` & `sdcflows-2.5.1/sdcflows/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.5.0/sdcflows/transform.py` & `sdcflows-2.5.1/sdcflows/transform.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.5.0/sdcflows/utils/bimap.py` & `sdcflows-2.5.1/sdcflows/utils/bimap.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.5.0/sdcflows/utils/epimanip.py` & `sdcflows-2.5.1/sdcflows/utils/epimanip.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.5.0/sdcflows/utils/misc.py` & `sdcflows-2.5.1/sdcflows/utils/misc.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.5.0/sdcflows/utils/phasemanip.py` & `sdcflows-2.5.1/sdcflows/utils/phasemanip.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.5.0/sdcflows/utils/tests/test_misc.py` & `sdcflows-2.5.1/sdcflows/utils/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.5.0/sdcflows/utils/tests/test_phasemanip.py` & `sdcflows-2.5.1/sdcflows/utils/tests/test_phasemanip.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.5.0/sdcflows/utils/tests/test_tools.py` & `sdcflows-2.5.1/sdcflows/utils/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.5.0/sdcflows/utils/tools.py` & `sdcflows-2.5.1/sdcflows/utils/tools.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.5.0/sdcflows/utils/wrangler.py` & `sdcflows-2.5.1/sdcflows/utils/wrangler.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 #
 """Find fieldmaps on the BIDS inputs for :abbr:`SDC (susceptibility distortion correction)`."""
 import logging
 from functools import reduce
 from itertools import product
 from contextlib import suppress
 from pathlib import Path
-from typing import Optional, Union, List
+from typing import Optional, Union, List, Dict, Any
 from bids.layout import BIDSLayout, BIDSFile
 from bids.utils import listify
 
 from .. import fieldmaps as fm
 
 
 def find_estimators(
@@ -437,15 +437,15 @@
             sbrefs = [
                 target for target in all_targets if target.entities["suffix"] == "sbref"
             ]
             if sbrefs:
                 targets = sbrefs
                 intent_map = []
                 for sbref in sbrefs:
-                    ents = sbref.entities.copy()
+                    ents = sbref.get_entities(metadata=False)
                     ents["suffix"] = ["bold", "dwi"]
                     intent_map.append(
                         [
                             target
                             for target in layout.get(**ents)
                             if target in all_targets
                         ]
@@ -489,56 +489,119 @@
     anat_file = layout.get(**{**base_entities, **{'suffix': anat_suffix, 'session': sessions}})
 
     if not fmapless or not anat_file:
         logger.debug("Skipping fmap-less estimation")
         return estimators
 
     logger.debug("Attempting fmap-less estimation")
+    estimator_specs = find_anatomical_estimators(
+        anat_file=anat_file[0],
+        layout=layout,
+        subject=subject,
+        sessions=sessions,
+        base_entities=base_entities,
+        suffixes=fmapless,
+    )
+    for spec in estimator_specs:
+        try:
+            estimator = fm.FieldmapEstimation(spec)
+        except (ValueError, TypeError) as err:
+            _log_debug_estimator_fail(logger, "ANAT", spec, layout.root, str(err))
+        else:
+            _log_debug_estimation(logger, estimator, layout.root)
+            estimators.append(estimator)
+    return estimators
+
+
+def find_anatomical_estimators(
+    *,
+    anat_file: BIDSFile,
+    layout: BIDSLayout,
+    subject: str,
+    sessions: List[str],
+    base_entities: Dict[str, Any],
+    suffixes: List[str],
+) -> List[List[fm.FieldmapFile]]:
+    r"""Find anatomical estimators
+
+    Given an anatomical reference image, create lists of files for estimating
+    susceptibility distortion for the EPI images in a dataset.
+
+    Parameters
+    ----------
+    anat_file : :class:`bids.layout.BIDSFile`
+        Anatomical reference image to use in estimators.
+    layout : :class:`bids.layout.BIDSLayout`
+        An initialized PyBIDS layout.
+    subject : :class:`str`
+        Participant label for this single-subject workflow.
+    sessions : :class:`list`
+        One of more session identifiers. To use all, pass ``[None]``.
+    base_entities : :class:`dict`
+        Entities to use to query for images. These should include any filters.
+    suffixes : :class:`list`
+        EPI suffixes, for example ``["bold", "dwi"]``. Associated ``"sbref"``\s
+        will be found and used in place of BOLD/diffusion EPIs.
+    """
+
     from .epimanip import get_trt
 
-    for ses, suffix in sorted(product(sessions, fmapless)):
-        candidates = layout.get(**{**base_entities, **{'suffix': suffix, 'session': ses}})
+    subject_root = Path(layout.root) / f"sub-{subject}"
+
+    hits = set()  # Avoid duplicates
+    estimators = []
+    for ses, suffix in sorted(product(sessions, suffixes)):
+        suffixes = ["sbref", suffix]  # Order indicates preference; prefer sbref
+        datatype = {
+            "bold": "func",
+            "dwi": "dwi",
+        }[suffix]
+        candidates = layout.get(
+            **{
+                **base_entities,
+                **{"suffix": suffixes, "session": ses, "datatype": datatype},
+            }
+        )
 
         # Filter out candidates without defined PE direction
         epi_targets = []
-        pe_dirs = []
-        ro_totals = []
 
         for candidate in candidates:
             meta = candidate.get_metadata()
-            pe_dir = meta.get("PhaseEncodingDirection")
 
-            if not pe_dir:
+            if not meta.get("PhaseEncodingDirection"):
                 continue
 
-            pe_dirs.append(pe_dir)
-            ro = 1.0
+            trt = 1.0
             with suppress(ValueError):
-                ro = get_trt(meta, candidate.path)
-            ro_totals.append(ro)
-            meta.update({"TotalReadoutTime": ro})
-            epi_targets.append(fm.FieldmapFile(candidate.path, metadata=meta))
-
-        trivial_estimators = [
-            [
-                fm.FieldmapFile(
-                    anat_file[0],
-                    metadata={"IntendedFor": str(Path(epi.path).relative_to(subject_root))},
-                ),
-                epi,
-            ] for epi in epi_targets
-        ]
+                trt = get_trt(meta, candidate.path)
+            meta.update({"TotalReadoutTime": trt})
+            epi_targets.append(fm.FieldmapFile(candidate, metadata=meta))
+
+        def sort_key(fmap):
+            # Return sbref before DWI/BOLD and shortest echo first
+            return suffixes.index(fmap.suffix), fmap.metadata.get("EchoTime", 1)
 
-        # TODO: Grouping could be done here; previously we grouped by (pe_dir, ro_time) pairs
-        syn_estimators = [fm.FieldmapEstimation(e) for e in trivial_estimators]
+        for target in sorted(epi_targets, key=sort_key):
+            if target.path in hits:
+                continue
+            query = {**base_entities, **target.entities}
 
-        for e in syn_estimators:
-            _log_debug_estimation(logger, e, layout.root)
+            # Find all echos, so strip from query, if present
+            query.pop("echo", None)
 
-        estimators.extend(syn_estimators)
+            # Include sbref and EPI images in IntendedFor
+            # No harm in including sbrefs that won't be corrected,
+            # and ensures the hits set prevents doubling up
+            intent = [Path(epi) for epi in layout.get(suffix=suffixes, **query)]
+            metadata = {
+                "IntendedFor": [str(epi.relative_to(subject_root)) for epi in intent]
+            }
+            estimators.append([fm.FieldmapFile(anat_file, metadata=metadata), target])
+            hits.update(intent)
 
     return estimators
 
 
 def _log_debug_estimation(
     logger: logging.Logger,
     estimation: fm.FieldmapEstimation,
```

### Comparing `sdcflows-2.5.0/sdcflows/viz/utils.py` & `sdcflows-2.5.1/sdcflows/viz/utils.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.5.0/sdcflows/workflows/ancillary.py` & `sdcflows-2.5.1/sdcflows/workflows/ancillary.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.5.0/sdcflows/workflows/apply/correction.py` & `sdcflows-2.5.1/sdcflows/workflows/apply/correction.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.5.0/sdcflows/workflows/apply/registration.py` & `sdcflows-2.5.1/sdcflows/workflows/apply/registration.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.5.0/sdcflows/workflows/apply/tests/fieldcoeff.nii.gz` & `sdcflows-2.5.1/sdcflows/workflows/apply/tests/fieldcoeff.nii.gz`

 * *Files identical despite different names*

### Comparing `sdcflows-2.5.0/sdcflows/workflows/apply/tests/test_correction.py` & `sdcflows-2.5.1/sdcflows/workflows/apply/tests/test_correction.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.5.0/sdcflows/workflows/apply/tests/test_registration.py` & `sdcflows-2.5.1/sdcflows/workflows/apply/tests/test_registration.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.5.0/sdcflows/workflows/base.py` & `sdcflows-2.5.1/sdcflows/workflows/base.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.5.0/sdcflows/workflows/fit/fieldmap.py` & `sdcflows-2.5.1/sdcflows/workflows/fit/fieldmap.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.5.0/sdcflows/workflows/fit/pepolar.py` & `sdcflows-2.5.1/sdcflows/workflows/fit/pepolar.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.5.0/sdcflows/workflows/fit/syn.py` & `sdcflows-2.5.1/sdcflows/workflows/fit/syn.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.5.0/sdcflows/workflows/fit/tests/test_fit.py` & `sdcflows-2.5.1/sdcflows/workflows/fit/tests/test_fit.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.5.0/sdcflows/workflows/fit/tests/test_pepolar.py` & `sdcflows-2.5.1/sdcflows/workflows/fit/tests/test_pepolar.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.5.0/sdcflows/workflows/fit/tests/test_phdiff.py` & `sdcflows-2.5.1/sdcflows/workflows/fit/tests/test_phdiff.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.5.0/sdcflows/workflows/fit/tests/test_syn.py` & `sdcflows-2.5.1/sdcflows/workflows/fit/tests/test_syn.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.5.0/sdcflows/workflows/outputs.py` & `sdcflows-2.5.1/sdcflows/workflows/outputs.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.5.0/sdcflows/workflows/tests/test_ancillary.py` & `sdcflows-2.5.1/sdcflows/workflows/tests/test_ancillary.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.5.0/sdcflows/workflows/tests/test_base.py` & `sdcflows-2.5.1/sdcflows/workflows/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.5.0/sdcflows.egg-info/PKG-INFO` & `sdcflows-2.5.1/sdcflows.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdcflows
-Version: 2.5.0
+Version: 2.5.1
 Summary: Susceptibility Distortion Correction (SDC) workflows for EPI MR schemes.
 Home-page: https://www.nipreps.org/sdcflows
 Author: The SDCflows developers
 Author-email: nipreps@gmail.com
 License: Apache-2.0
 Project-URL: Documentation, https://www.nipreps.org/sdcflows
 Project-URL: GitHub, https://github.com/nipreps/sdcflows
```

### Comparing `sdcflows-2.5.0/sdcflows.egg-info/SOURCES.txt` & `sdcflows-2.5.1/sdcflows.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sdcflows-2.5.0/sdcflows.egg-info/requires.txt` & `sdcflows-2.5.1/sdcflows.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `sdcflows-2.5.0/setup.cfg` & `sdcflows-2.5.1/setup.cfg`

 * *Files identical despite different names*

