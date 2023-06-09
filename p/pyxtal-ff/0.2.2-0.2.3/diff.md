# Comparing `tmp/pyxtal_ff-0.2.2.tar.gz` & `tmp/pyxtal_ff-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/qiangzhu/Desktop/github/PyXtal_FF/dist/.tmp-zujhbnbg/pyxtal_ff-0.2.2.tar", last modified: Wed Dec 21 20:04:58 2022, max compression
+gzip compressed data, was "/Users/qiangzhu/Desktop/github/PyXtal_FF/dist/.tmp-ohhsuhjm/pyxtal_ff-0.2.3.tar", last modified: Fri Jun  9 17:21:05 2023, max compression
```

## Comparing `pyxtal_ff-0.2.2.tar` & `pyxtal_ff-0.2.3.tar`

### file list

```diff
@@ -1,58 +1,57 @@
-drwxr-xr-x   0 qiangzhu   (501) staff       (20)        0 2022-12-21 20:04:58.000000 pyxtal_ff-0.2.2/
--rw-r--r--   0 qiangzhu   (501) staff       (20)     3335 2022-12-21 20:04:58.000000 pyxtal_ff-0.2.2/PKG-INFO
--rw-r--r--   0 qiangzhu   (501) staff       (20)     2859 2021-05-16 07:05:53.000000 pyxtal_ff-0.2.2/README.md
-drwxr-xr-x   0 qiangzhu   (501) staff       (20)        0 2022-12-21 20:04:58.000000 pyxtal_ff-0.2.2/pyxtal_ff/
--rw-r--r--   0 qiangzhu   (501) staff       (20)    20637 2021-08-19 23:18:01.000000 pyxtal_ff-0.2.2/pyxtal_ff/__init__.py
-drwxr-xr-x   0 qiangzhu   (501) staff       (20)        0 2022-12-21 20:04:58.000000 pyxtal_ff-0.2.2/pyxtal_ff/calculator/
--rw-r--r--   0 qiangzhu   (501) staff       (20)     6459 2022-12-21 20:01:35.000000 pyxtal_ff-0.2.2/pyxtal_ff/calculator/__init__.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)    40718 2021-05-10 20:59:07.000000 pyxtal_ff-0.2.2/pyxtal_ff/calculator/elasticity.py
--rwxr-xr-x   0 qiangzhu   (501) staff       (20)     9647 2021-05-16 07:05:54.000000 pyxtal_ff-0.2.2/pyxtal_ff/calculator/lammpslib.py
--rwxr-xr-x   0 qiangzhu   (501) staff       (20)     9650 2022-02-23 03:51:36.000000 pyxtal_ff-0.2.2/pyxtal_ff/calculator/lammpsrun.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)     6132 2022-03-11 18:27:35.000000 pyxtal_ff-0.2.2/pyxtal_ff/calculator/phonon.py
-drwxr-xr-x   0 qiangzhu   (501) staff       (20)        0 2022-12-21 20:04:58.000000 pyxtal_ff-0.2.2/pyxtal_ff/datasets/
-drwxr-xr-x   0 qiangzhu   (501) staff       (20)        0 2022-12-21 20:04:58.000000 pyxtal_ff-0.2.2/pyxtal_ff/datasets/Si/
-drwxr-xr-x   0 qiangzhu   (501) staff       (20)        0 2022-12-21 20:04:58.000000 pyxtal_ff-0.2.2/pyxtal_ff/datasets/Si/PyXtal/
--rw-r--r--   0 qiangzhu   (501) staff       (20)     1440 2021-05-10 20:56:10.000000 pyxtal_ff-0.2.2/pyxtal_ff/datasets/Si/PyXtal/PES_graph.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)  5962631 2021-05-10 20:56:10.000000 pyxtal_ff-0.2.2/pyxtal_ff/datasets/Si/PyXtal/Si.json
--rw-r--r--   0 qiangzhu   (501) staff       (20)  2796048 2021-05-10 20:56:10.000000 pyxtal_ff-0.2.2/pyxtal_ff/datasets/Si/PyXtal/Si16.json
--rw-r--r--   0 qiangzhu   (501) staff       (20)  2138186 2021-05-10 20:56:10.000000 pyxtal_ff-0.2.2/pyxtal_ff/datasets/Si/PyXtal/Si4.json
--rw-r--r--   0 qiangzhu   (501) staff       (20)  2958905 2021-05-10 20:56:10.000000 pyxtal_ff-0.2.2/pyxtal_ff/datasets/Si/PyXtal/Si6.json
--rw-r--r--   0 qiangzhu   (501) staff       (20)  3623101 2021-05-10 20:56:10.000000 pyxtal_ff-0.2.2/pyxtal_ff/datasets/Si/PyXtal/Si8.json
--rw-r--r--   0 qiangzhu   (501) staff       (20)  8912277 2021-05-10 20:56:10.000000 pyxtal_ff-0.2.2/pyxtal_ff/datasets/Si/PyXtal/Si_train.json
--rw-r--r--   0 qiangzhu   (501) staff       (20)   114201 2021-08-19 23:18:01.000000 pyxtal_ff-0.2.2/pyxtal_ff/datasets/Si/PyXtal/bp-16-16-checkpoint.pth
-drwxr-xr-x   0 qiangzhu   (501) staff       (20)        0 2022-12-21 20:04:58.000000 pyxtal_ff-0.2.2/pyxtal_ff/descriptors/
--rw-r--r--   0 qiangzhu   (501) staff       (20)    51499 2021-12-14 01:33:55.000000 pyxtal_ff-0.2.2/pyxtal_ff/descriptors/ACSF.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)    19163 2021-08-19 23:18:01.000000 pyxtal_ff-0.2.2/pyxtal_ff/descriptors/EAD.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)    61333 2021-08-19 23:18:01.000000 pyxtal_ff-0.2.2/pyxtal_ff/descriptors/SNAP.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)    26915 2021-08-19 23:18:01.000000 pyxtal_ff-0.2.2/pyxtal_ff/descriptors/SO3.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)    60262 2022-08-02 13:35:23.000000 pyxtal_ff-0.2.2/pyxtal_ff/descriptors/SO4.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)   749448 2021-05-10 20:56:10.000000 pyxtal_ff-0.2.2/pyxtal_ff/descriptors/Wigner_coefficients.npy
--rw-r--r--   0 qiangzhu   (501) staff       (20)      851 2021-05-10 20:56:10.000000 pyxtal_ff-0.2.2/pyxtal_ff/descriptors/_generate_coefs.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)    11972 2021-05-16 07:05:54.000000 pyxtal_ff-0.2.2/pyxtal_ff/descriptors/angular_momentum.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)     4550 2021-05-16 07:05:54.000000 pyxtal_ff-0.2.2/pyxtal_ff/descriptors/cutoff.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)     9525 2021-05-10 20:56:10.000000 pyxtal_ff-0.2.2/pyxtal_ff/descriptors/lbispectrum.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)      949 2021-05-10 20:56:10.000000 pyxtal_ff-0.2.2/pyxtal_ff/descriptors/utils.py
-drwxr-xr-x   0 qiangzhu   (501) staff       (20)        0 2022-12-21 20:04:58.000000 pyxtal_ff-0.2.2/pyxtal_ff/models/
--rw-r--r--   0 qiangzhu   (501) staff       (20)    18813 2021-05-10 20:59:07.000000 pyxtal_ff-0.2.2/pyxtal_ff/models/gaussianprocess.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)    53079 2022-05-23 21:19:57.000000 pyxtal_ff-0.2.2/pyxtal_ff/models/neuralnetwork.py
-drwxr-xr-x   0 qiangzhu   (501) staff       (20)        0 2022-12-21 20:04:58.000000 pyxtal_ff-0.2.2/pyxtal_ff/models/optimizers/
--rw-r--r--   0 qiangzhu   (501) staff       (20)    16834 2021-05-10 20:56:10.000000 pyxtal_ff-0.2.2/pyxtal_ff/models/optimizers/lbfgs.py
--rwxr-xr-x   0 qiangzhu   (501) staff       (20)     4630 2021-05-10 20:56:10.000000 pyxtal_ff-0.2.2/pyxtal_ff/models/optimizers/lbfgsb.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)     4693 2021-05-10 20:59:07.000000 pyxtal_ff-0.2.2/pyxtal_ff/models/optimizers/regressor.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)    31465 2022-12-21 20:01:35.000000 pyxtal_ff-0.2.2/pyxtal_ff/models/polynomialregression.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)    16844 2021-08-19 23:18:01.000000 pyxtal_ff-0.2.2/pyxtal_ff/test_all.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)     2425 2021-05-16 07:05:54.000000 pyxtal_ff-0.2.2/pyxtal_ff/test_properties.py
-drwxr-xr-x   0 qiangzhu   (501) staff       (20)        0 2022-12-21 20:04:58.000000 pyxtal_ff-0.2.2/pyxtal_ff/utilities/
--rw-r--r--   0 qiangzhu   (501) staff       (20)    27931 2022-03-30 21:39:32.000000 pyxtal_ff-0.2.2/pyxtal_ff/utilities/__init__.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)    10969 2021-08-19 23:18:01.000000 pyxtal_ff-0.2.2/pyxtal_ff/utilities/base_potential.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)     3543 2021-05-16 07:05:54.000000 pyxtal_ff-0.2.2/pyxtal_ff/utilities/elements.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)     2763 2021-05-10 20:56:10.000000 pyxtal_ff-0.2.2/pyxtal_ff/utilities/gradient.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)       22 2022-12-21 20:01:35.000000 pyxtal_ff-0.2.2/pyxtal_ff/version.py
-drwxr-xr-x   0 qiangzhu   (501) staff       (20)        0 2022-12-21 20:04:58.000000 pyxtal_ff-0.2.2/pyxtal_ff.egg-info/
--rw-r--r--   0 qiangzhu   (501) staff       (20)     3335 2022-12-21 20:04:58.000000 pyxtal_ff-0.2.2/pyxtal_ff.egg-info/PKG-INFO
--rw-r--r--   0 qiangzhu   (501) staff       (20)     1518 2022-12-21 20:04:58.000000 pyxtal_ff-0.2.2/pyxtal_ff.egg-info/SOURCES.txt
--rw-r--r--   0 qiangzhu   (501) staff       (20)        1 2022-12-21 20:04:58.000000 pyxtal_ff-0.2.2/pyxtal_ff.egg-info/dependency_links.txt
--rw-r--r--   0 qiangzhu   (501) staff       (20)      144 2022-12-21 20:04:58.000000 pyxtal_ff-0.2.2/pyxtal_ff.egg-info/requires.txt
--rw-r--r--   0 qiangzhu   (501) staff       (20)       10 2022-12-21 20:04:58.000000 pyxtal_ff-0.2.2/pyxtal_ff.egg-info/top_level.txt
--rw-r--r--   0 qiangzhu   (501) staff       (20)      125 2022-12-21 20:04:58.000000 pyxtal_ff-0.2.2/setup.cfg
--rw-r--r--   0 qiangzhu   (501) staff       (20)     1652 2022-12-21 20:01:35.000000 pyxtal_ff-0.2.2/setup.py
+drwxr-xr-x   0 qiangzhu   (501) staff       (20)        0 2023-06-09 17:21:05.000000 pyxtal_ff-0.2.3/
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     3335 2023-06-09 17:21:05.000000 pyxtal_ff-0.2.3/PKG-INFO
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     2859 2023-06-09 17:19:34.000000 pyxtal_ff-0.2.3/README.md
+drwxr-xr-x   0 qiangzhu   (501) staff       (20)        0 2023-06-09 17:21:04.000000 pyxtal_ff-0.2.3/pyxtal_ff/
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    20637 2023-06-09 17:19:34.000000 pyxtal_ff-0.2.3/pyxtal_ff/__init__.py
+drwxr-xr-x   0 qiangzhu   (501) staff       (20)        0 2023-06-09 17:21:04.000000 pyxtal_ff-0.2.3/pyxtal_ff/calculator/
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     6459 2023-06-09 17:19:34.000000 pyxtal_ff-0.2.3/pyxtal_ff/calculator/__init__.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    40718 2023-06-09 17:19:34.000000 pyxtal_ff-0.2.3/pyxtal_ff/calculator/elasticity.py
+-rwxr-xr-x   0 qiangzhu   (501) staff       (20)     9647 2023-06-09 17:19:34.000000 pyxtal_ff-0.2.3/pyxtal_ff/calculator/lammpslib.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     6132 2023-06-09 17:19:34.000000 pyxtal_ff-0.2.3/pyxtal_ff/calculator/phonon.py
+drwxr-xr-x   0 qiangzhu   (501) staff       (20)        0 2023-06-09 17:21:04.000000 pyxtal_ff-0.2.3/pyxtal_ff/datasets/
+drwxr-xr-x   0 qiangzhu   (501) staff       (20)        0 2023-06-09 17:21:04.000000 pyxtal_ff-0.2.3/pyxtal_ff/datasets/Si/
+drwxr-xr-x   0 qiangzhu   (501) staff       (20)        0 2023-06-09 17:21:05.000000 pyxtal_ff-0.2.3/pyxtal_ff/datasets/Si/PyXtal/
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     1440 2023-06-09 17:19:34.000000 pyxtal_ff-0.2.3/pyxtal_ff/datasets/Si/PyXtal/PES_graph.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)  5962631 2023-06-09 17:19:34.000000 pyxtal_ff-0.2.3/pyxtal_ff/datasets/Si/PyXtal/Si.json
+-rw-r--r--   0 qiangzhu   (501) staff       (20)  2796048 2023-06-09 17:19:34.000000 pyxtal_ff-0.2.3/pyxtal_ff/datasets/Si/PyXtal/Si16.json
+-rw-r--r--   0 qiangzhu   (501) staff       (20)  2138186 2023-06-09 17:19:34.000000 pyxtal_ff-0.2.3/pyxtal_ff/datasets/Si/PyXtal/Si4.json
+-rw-r--r--   0 qiangzhu   (501) staff       (20)  2958905 2023-06-09 17:19:34.000000 pyxtal_ff-0.2.3/pyxtal_ff/datasets/Si/PyXtal/Si6.json
+-rw-r--r--   0 qiangzhu   (501) staff       (20)  3623101 2023-06-09 17:19:34.000000 pyxtal_ff-0.2.3/pyxtal_ff/datasets/Si/PyXtal/Si8.json
+-rw-r--r--   0 qiangzhu   (501) staff       (20)  8912277 2023-06-09 17:19:34.000000 pyxtal_ff-0.2.3/pyxtal_ff/datasets/Si/PyXtal/Si_train.json
+-rw-r--r--   0 qiangzhu   (501) staff       (20)   114201 2023-06-09 17:19:34.000000 pyxtal_ff-0.2.3/pyxtal_ff/datasets/Si/PyXtal/bp-16-16-checkpoint.pth
+drwxr-xr-x   0 qiangzhu   (501) staff       (20)        0 2023-06-09 17:21:05.000000 pyxtal_ff-0.2.3/pyxtal_ff/descriptors/
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    51499 2023-06-09 17:19:34.000000 pyxtal_ff-0.2.3/pyxtal_ff/descriptors/ACSF.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    19163 2023-06-09 17:19:34.000000 pyxtal_ff-0.2.3/pyxtal_ff/descriptors/EAD.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    61333 2023-06-09 17:19:34.000000 pyxtal_ff-0.2.3/pyxtal_ff/descriptors/SNAP.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    27242 2023-06-09 17:19:34.000000 pyxtal_ff-0.2.3/pyxtal_ff/descriptors/SO3.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    60262 2023-06-09 17:19:34.000000 pyxtal_ff-0.2.3/pyxtal_ff/descriptors/SO4.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)   749448 2023-06-09 17:19:34.000000 pyxtal_ff-0.2.3/pyxtal_ff/descriptors/Wigner_coefficients.npy
+-rw-r--r--   0 qiangzhu   (501) staff       (20)      851 2023-06-09 17:19:34.000000 pyxtal_ff-0.2.3/pyxtal_ff/descriptors/_generate_coefs.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    11972 2023-06-09 17:19:34.000000 pyxtal_ff-0.2.3/pyxtal_ff/descriptors/angular_momentum.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     4550 2023-06-09 17:19:34.000000 pyxtal_ff-0.2.3/pyxtal_ff/descriptors/cutoff.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     9525 2023-06-09 17:19:34.000000 pyxtal_ff-0.2.3/pyxtal_ff/descriptors/lbispectrum.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)      949 2023-06-09 17:19:34.000000 pyxtal_ff-0.2.3/pyxtal_ff/descriptors/utils.py
+drwxr-xr-x   0 qiangzhu   (501) staff       (20)        0 2023-06-09 17:21:05.000000 pyxtal_ff-0.2.3/pyxtal_ff/models/
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    18813 2023-06-09 17:19:34.000000 pyxtal_ff-0.2.3/pyxtal_ff/models/gaussianprocess.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    53079 2023-06-09 17:19:34.000000 pyxtal_ff-0.2.3/pyxtal_ff/models/neuralnetwork.py
+drwxr-xr-x   0 qiangzhu   (501) staff       (20)        0 2023-06-09 17:21:05.000000 pyxtal_ff-0.2.3/pyxtal_ff/models/optimizers/
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    16834 2023-06-09 17:19:34.000000 pyxtal_ff-0.2.3/pyxtal_ff/models/optimizers/lbfgs.py
+-rwxr-xr-x   0 qiangzhu   (501) staff       (20)     4630 2023-06-09 17:19:34.000000 pyxtal_ff-0.2.3/pyxtal_ff/models/optimizers/lbfgsb.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     4693 2023-06-09 17:19:34.000000 pyxtal_ff-0.2.3/pyxtal_ff/models/optimizers/regressor.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    31465 2023-06-09 17:19:34.000000 pyxtal_ff-0.2.3/pyxtal_ff/models/polynomialregression.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    16844 2023-06-09 17:19:34.000000 pyxtal_ff-0.2.3/pyxtal_ff/test_all.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     2425 2023-06-09 17:19:34.000000 pyxtal_ff-0.2.3/pyxtal_ff/test_properties.py
+drwxr-xr-x   0 qiangzhu   (501) staff       (20)        0 2023-06-09 17:21:05.000000 pyxtal_ff-0.2.3/pyxtal_ff/utilities/
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    27931 2023-06-09 17:19:34.000000 pyxtal_ff-0.2.3/pyxtal_ff/utilities/__init__.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    10969 2023-06-09 17:19:34.000000 pyxtal_ff-0.2.3/pyxtal_ff/utilities/base_potential.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     3543 2023-06-09 17:19:34.000000 pyxtal_ff-0.2.3/pyxtal_ff/utilities/elements.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     2763 2023-06-09 17:19:34.000000 pyxtal_ff-0.2.3/pyxtal_ff/utilities/gradient.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)       22 2023-06-09 17:19:34.000000 pyxtal_ff-0.2.3/pyxtal_ff/version.py
+drwxr-xr-x   0 qiangzhu   (501) staff       (20)        0 2023-06-09 17:21:04.000000 pyxtal_ff-0.2.3/pyxtal_ff.egg-info/
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     3335 2023-06-09 17:21:04.000000 pyxtal_ff-0.2.3/pyxtal_ff.egg-info/PKG-INFO
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     1484 2023-06-09 17:21:04.000000 pyxtal_ff-0.2.3/pyxtal_ff.egg-info/SOURCES.txt
+-rw-r--r--   0 qiangzhu   (501) staff       (20)        1 2023-06-09 17:21:04.000000 pyxtal_ff-0.2.3/pyxtal_ff.egg-info/dependency_links.txt
+-rw-r--r--   0 qiangzhu   (501) staff       (20)      144 2023-06-09 17:21:04.000000 pyxtal_ff-0.2.3/pyxtal_ff.egg-info/requires.txt
+-rw-r--r--   0 qiangzhu   (501) staff       (20)       10 2023-06-09 17:21:04.000000 pyxtal_ff-0.2.3/pyxtal_ff.egg-info/top_level.txt
+-rw-r--r--   0 qiangzhu   (501) staff       (20)      125 2023-06-09 17:21:05.000000 pyxtal_ff-0.2.3/setup.cfg
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     1652 2023-06-09 17:19:34.000000 pyxtal_ff-0.2.3/setup.py
```

### Comparing `pyxtal_ff-0.2.2/PKG-INFO` & `pyxtal_ff-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyxtal_ff
-Version: 0.2.2
+Version: 0.2.3
 Summary: Python code for force field training of crystals
 Home-page: https://github.com/qzhu2017/PyXtal-FF
 Author: Qiang Zhu, Howard Yanxon, David Zagaceta, Binh Tang
 Author-email: qiang.zhu@unlv.edu
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyxtal_ff-0.2.2/README.md` & `pyxtal_ff-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `pyxtal_ff-0.2.2/pyxtal_ff/__init__.py` & `pyxtal_ff-0.2.3/pyxtal_ff/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxtal_ff-0.2.2/pyxtal_ff/calculator/__init__.py` & `pyxtal_ff-0.2.3/pyxtal_ff/calculator/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxtal_ff-0.2.2/pyxtal_ff/calculator/elasticity.py` & `pyxtal_ff-0.2.3/pyxtal_ff/calculator/elasticity.py`

 * *Files identical despite different names*

### Comparing `pyxtal_ff-0.2.2/pyxtal_ff/calculator/lammpslib.py` & `pyxtal_ff-0.2.3/pyxtal_ff/calculator/lammpslib.py`

 * *Files identical despite different names*

### Comparing `pyxtal_ff-0.2.2/pyxtal_ff/calculator/phonon.py` & `pyxtal_ff-0.2.3/pyxtal_ff/calculator/phonon.py`

 * *Files identical despite different names*

### Comparing `pyxtal_ff-0.2.2/pyxtal_ff/datasets/Si/PyXtal/PES_graph.py` & `pyxtal_ff-0.2.3/pyxtal_ff/datasets/Si/PyXtal/PES_graph.py`

 * *Files identical despite different names*

### Comparing `pyxtal_ff-0.2.2/pyxtal_ff/datasets/Si/PyXtal/Si.json` & `pyxtal_ff-0.2.3/pyxtal_ff/datasets/Si/PyXtal/Si.json`

 * *Files identical despite different names*

### Comparing `pyxtal_ff-0.2.2/pyxtal_ff/datasets/Si/PyXtal/Si16.json` & `pyxtal_ff-0.2.3/pyxtal_ff/datasets/Si/PyXtal/Si16.json`

 * *Files identical despite different names*

### Comparing `pyxtal_ff-0.2.2/pyxtal_ff/datasets/Si/PyXtal/Si4.json` & `pyxtal_ff-0.2.3/pyxtal_ff/datasets/Si/PyXtal/Si4.json`

 * *Files identical despite different names*

### Comparing `pyxtal_ff-0.2.2/pyxtal_ff/datasets/Si/PyXtal/Si6.json` & `pyxtal_ff-0.2.3/pyxtal_ff/datasets/Si/PyXtal/Si6.json`

 * *Files identical despite different names*

### Comparing `pyxtal_ff-0.2.2/pyxtal_ff/datasets/Si/PyXtal/Si8.json` & `pyxtal_ff-0.2.3/pyxtal_ff/datasets/Si/PyXtal/Si8.json`

 * *Files identical despite different names*

### Comparing `pyxtal_ff-0.2.2/pyxtal_ff/datasets/Si/PyXtal/Si_train.json` & `pyxtal_ff-0.2.3/pyxtal_ff/datasets/Si/PyXtal/Si_train.json`

 * *Files identical despite different names*

### Comparing `pyxtal_ff-0.2.2/pyxtal_ff/datasets/Si/PyXtal/bp-16-16-checkpoint.pth` & `pyxtal_ff-0.2.3/pyxtal_ff/datasets/Si/PyXtal/bp-16-16-checkpoint.pth`

 * *Files identical despite different names*

### Comparing `pyxtal_ff-0.2.2/pyxtal_ff/descriptors/ACSF.py` & `pyxtal_ff-0.2.3/pyxtal_ff/descriptors/ACSF.py`

 * *Files identical despite different names*

### Comparing `pyxtal_ff-0.2.2/pyxtal_ff/descriptors/EAD.py` & `pyxtal_ff-0.2.3/pyxtal_ff/descriptors/EAD.py`

 * *Files identical despite different names*

### Comparing `pyxtal_ff-0.2.2/pyxtal_ff/descriptors/SNAP.py` & `pyxtal_ff-0.2.3/pyxtal_ff/descriptors/SNAP.py`

 * *Files identical despite different names*

### Comparing `pyxtal_ff-0.2.2/pyxtal_ff/descriptors/SO3.py` & `pyxtal_ff-0.2.3/pyxtal_ff/descriptors/SO3.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,26 +13,28 @@
 
     args:
         nmax: int, degree of radial expansion
         lmax: int, degree of spherical harmonic expansion
         rcut: float, cutoff radius for neighbor calculation
         alpha: float, gaussian width parameter
         derivative: bool, whether to calculate the gradient of not
+        weight_on: bool, if True, the neighbors with different type will be counted as negative
     '''
 
-    def __init__(self, nmax=3, lmax=3, rcut=3.5, alpha=2.0, derivative=True, stress=False, cutoff_function='cosine'):
+    def __init__(self, nmax=3, lmax=3, rcut=3.5, alpha=2.0, derivative=True, stress=False, cutoff_function='cosine', weight_on=False):
         # populate attributes
         self.nmax = nmax
         self.lmax = lmax
         self.rcut = rcut
         self.alpha = alpha
         self.derivative = derivative
         self.stress = stress
         self._type = "SO3"
         self.cutoff_function = cutoff_function
+        self.weight_on = weight_on
         return
 
     def __str__(self):
         s = "SO3 descriptor with Cutoff: {:6.3f}".format(self.rcut)
         s += " lmax: {:d}, nmax: {:d}, alpha: {:.3f}\n".format(self.lmax, self.nmax, self.alpha)
         return s
 
@@ -172,15 +174,15 @@
 
     def clear_memory(self):
         '''
         Clears all memory that isn't an essential attribute for the calculator
         '''
         attrs = list(vars(self).keys())
         for attr in attrs:
-            if attr not in {'_nmax', '_lmax', '_rcut', '_alpha', '_derivative', '_stress', '_cutoff_function'}:
+            if attr not in {'_nmax', '_lmax', '_rcut', '_alpha', '_derivative', '_stress', '_cutoff_function', 'weight_on'}:
                 delattr(self, attr)
         return
 
     def calculate(self, atoms, atom_ids=None):
         '''
         Calculates the SO(3) power spectrum components of the
         smoothened atomic neighbor density function
@@ -335,15 +337,19 @@
             # get indices and cell offsets for each neighbor
             indices, offsets = nl.get_neighbors(i)
             temp_indices.append(indices)
             for j, offset in zip(indices, offsets):
                 pos = atoms.positions[j] + np.dot(offset,atoms.get_cell()) - center_atom
                 center_atoms.append(center_atom)
                 neighbors.append(pos)
-                atomic_weights.append(atoms[j].number)
+                if self.weight_on and atoms[j].number != atoms[i].number:
+                    factor = -1
+                else:
+                    factor = 1
+                atomic_weights.append(factor*atoms[j].number)
                 neighbor_indices.append([i,j])
 
         neighbor_indices = np.array(neighbor_indices, dtype=np.int64)
         Seq = []
         for i in atom_ids:
             ineighs = neighbor_indices[:,0] == i
             unique_atoms = np.unique(neighbor_indices[ineighs])
```

### Comparing `pyxtal_ff-0.2.2/pyxtal_ff/descriptors/SO4.py` & `pyxtal_ff-0.2.3/pyxtal_ff/descriptors/SO4.py`

 * *Files identical despite different names*

### Comparing `pyxtal_ff-0.2.2/pyxtal_ff/descriptors/Wigner_coefficients.npy` & `pyxtal_ff-0.2.3/pyxtal_ff/descriptors/Wigner_coefficients.npy`

 * *Files identical despite different names*

### Comparing `pyxtal_ff-0.2.2/pyxtal_ff/descriptors/_generate_coefs.py` & `pyxtal_ff-0.2.3/pyxtal_ff/descriptors/_generate_coefs.py`

 * *Files identical despite different names*

### Comparing `pyxtal_ff-0.2.2/pyxtal_ff/descriptors/angular_momentum.py` & `pyxtal_ff-0.2.3/pyxtal_ff/descriptors/angular_momentum.py`

 * *Files identical despite different names*

### Comparing `pyxtal_ff-0.2.2/pyxtal_ff/descriptors/cutoff.py` & `pyxtal_ff-0.2.3/pyxtal_ff/descriptors/cutoff.py`

 * *Files identical despite different names*

### Comparing `pyxtal_ff-0.2.2/pyxtal_ff/descriptors/lbispectrum.py` & `pyxtal_ff-0.2.3/pyxtal_ff/descriptors/lbispectrum.py`

 * *Files identical despite different names*

### Comparing `pyxtal_ff-0.2.2/pyxtal_ff/descriptors/utils.py` & `pyxtal_ff-0.2.3/pyxtal_ff/descriptors/utils.py`

 * *Files identical despite different names*

### Comparing `pyxtal_ff-0.2.2/pyxtal_ff/models/gaussianprocess.py` & `pyxtal_ff-0.2.3/pyxtal_ff/models/gaussianprocess.py`

 * *Files identical despite different names*

### Comparing `pyxtal_ff-0.2.2/pyxtal_ff/models/neuralnetwork.py` & `pyxtal_ff-0.2.3/pyxtal_ff/models/neuralnetwork.py`

 * *Files identical despite different names*

### Comparing `pyxtal_ff-0.2.2/pyxtal_ff/models/optimizers/lbfgs.py` & `pyxtal_ff-0.2.3/pyxtal_ff/models/optimizers/lbfgs.py`

 * *Files identical despite different names*

### Comparing `pyxtal_ff-0.2.2/pyxtal_ff/models/optimizers/lbfgsb.py` & `pyxtal_ff-0.2.3/pyxtal_ff/models/optimizers/lbfgsb.py`

 * *Files identical despite different names*

### Comparing `pyxtal_ff-0.2.2/pyxtal_ff/models/optimizers/regressor.py` & `pyxtal_ff-0.2.3/pyxtal_ff/models/optimizers/regressor.py`

 * *Files identical despite different names*

### Comparing `pyxtal_ff-0.2.2/pyxtal_ff/models/polynomialregression.py` & `pyxtal_ff-0.2.3/pyxtal_ff/models/polynomialregression.py`

 * *Files identical despite different names*

### Comparing `pyxtal_ff-0.2.2/pyxtal_ff/test_all.py` & `pyxtal_ff-0.2.3/pyxtal_ff/test_all.py`

 * *Files identical despite different names*

### Comparing `pyxtal_ff-0.2.2/pyxtal_ff/test_properties.py` & `pyxtal_ff-0.2.3/pyxtal_ff/test_properties.py`

 * *Files identical despite different names*

### Comparing `pyxtal_ff-0.2.2/pyxtal_ff/utilities/__init__.py` & `pyxtal_ff-0.2.3/pyxtal_ff/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxtal_ff-0.2.2/pyxtal_ff/utilities/base_potential.py` & `pyxtal_ff-0.2.3/pyxtal_ff/utilities/base_potential.py`

 * *Files identical despite different names*

### Comparing `pyxtal_ff-0.2.2/pyxtal_ff/utilities/elements.py` & `pyxtal_ff-0.2.3/pyxtal_ff/utilities/elements.py`

 * *Files identical despite different names*

### Comparing `pyxtal_ff-0.2.2/pyxtal_ff/utilities/gradient.py` & `pyxtal_ff-0.2.3/pyxtal_ff/utilities/gradient.py`

 * *Files identical despite different names*

### Comparing `pyxtal_ff-0.2.2/pyxtal_ff.egg-info/PKG-INFO` & `pyxtal_ff-0.2.3/pyxtal_ff.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyxtal-ff
-Version: 0.2.2
+Version: 0.2.3
 Summary: Python code for force field training of crystals
 Home-page: https://github.com/qzhu2017/PyXtal-FF
 Author: Qiang Zhu, Howard Yanxon, David Zagaceta, Binh Tang
 Author-email: qiang.zhu@unlv.edu
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyxtal_ff-0.2.2/pyxtal_ff.egg-info/SOURCES.txt` & `pyxtal_ff-0.2.3/pyxtal_ff.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 pyxtal_ff.egg-info/SOURCES.txt
 pyxtal_ff.egg-info/dependency_links.txt
 pyxtal_ff.egg-info/requires.txt
 pyxtal_ff.egg-info/top_level.txt
 pyxtal_ff/calculator/__init__.py
 pyxtal_ff/calculator/elasticity.py
 pyxtal_ff/calculator/lammpslib.py
-pyxtal_ff/calculator/lammpsrun.py
 pyxtal_ff/calculator/phonon.py
 pyxtal_ff/datasets/Si/PyXtal/PES_graph.py
 pyxtal_ff/datasets/Si/PyXtal/Si.json
 pyxtal_ff/datasets/Si/PyXtal/Si16.json
 pyxtal_ff/datasets/Si/PyXtal/Si4.json
 pyxtal_ff/datasets/Si/PyXtal/Si6.json
 pyxtal_ff/datasets/Si/PyXtal/Si8.json
```

### Comparing `pyxtal_ff-0.2.2/setup.py` & `pyxtal_ff-0.2.3/setup.py`

 * *Files identical despite different names*

