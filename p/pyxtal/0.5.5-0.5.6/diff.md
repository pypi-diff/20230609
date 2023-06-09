# Comparing `tmp/pyxtal-0.5.5.tar.gz` & `tmp/pyxtal-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/qiangzhu/Desktop/github/PyXtal/dist/tmp3o0cmb_j/pyxtal-0.5.5.tar", last modified: Fri Nov 18 06:14:45 2022, max compression
+gzip compressed data, was "/Users/qiangzhu/Desktop/github/PyXtal/dist/.tmp-ad4xrg8r/pyxtal-0.5.6.tar", last modified: Fri Jun  9 17:12:42 2023, max compression
```

## Comparing `pyxtal-0.5.5.tar` & `pyxtal-0.5.6.tar`

### file list

```diff
@@ -1,156 +1,156 @@
-drwxr-xr-x   0 qiangzhu   (501) staff       (20)        0 2022-11-18 06:14:45.000000 pyxtal-0.5.5/
--rw-r--r--   0 qiangzhu   (501) staff       (20)     1084 2022-06-13 19:36:20.000000 pyxtal-0.5.5/LICENSE.txt
--rwxr-xr-x   0 qiangzhu   (501) staff       (20)       82 2022-06-15 16:30:37.000000 pyxtal-0.5.5/MANIFEST.in
--rw-r--r--   0 qiangzhu   (501) staff       (20)     5203 2022-11-18 06:14:45.000000 pyxtal-0.5.5/PKG-INFO
--rw-r--r--   0 qiangzhu   (501) staff       (20)     4692 2022-07-27 22:43:15.000000 pyxtal-0.5.5/README.md
-drwxr-xr-x   0 qiangzhu   (501) staff       (20)        0 2022-11-18 06:14:45.000000 pyxtal-0.5.5/pyxtal/
--rw-r--r--   0 qiangzhu   (501) staff       (20)    31648 2022-08-14 23:14:59.000000 pyxtal-0.5.5/pyxtal/XRD.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)    98510 2022-09-15 04:16:14.000000 pyxtal-0.5.5/pyxtal/__init__.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)     5985 2022-06-21 15:19:36.000000 pyxtal-0.5.5/pyxtal/block_crystal.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)     1784 2022-06-23 22:59:32.000000 pyxtal-0.5.5/pyxtal/constants.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)    13810 2022-06-21 13:41:23.000000 pyxtal-0.5.5/pyxtal/crystal.py
-drwxr-xr-x   0 qiangzhu   (501) staff       (20)        0 2022-11-18 06:14:45.000000 pyxtal-0.5.5/pyxtal/database/
--rw-r--r--   0 qiangzhu   (501) staff       (20)    22281 2022-06-17 19:11:39.000000 pyxtal-0.5.5/pyxtal/database/HM_Full.csv
--rw-r--r--   0 qiangzhu   (501) staff       (20)        0 2021-08-17 15:48:08.000000 pyxtal-0.5.5/pyxtal/database/__init__.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)     6824 2021-08-17 15:48:08.000000 pyxtal-0.5.5/pyxtal/database/atomic_scattering_params.json
--rw-r--r--   0 qiangzhu   (501) staff       (20)     2120 2022-08-11 19:04:42.000000 pyxtal-0.5.5/pyxtal/database/bonds.json
--rw-------   0 qiangzhu   (501) staff       (20)     2950 2022-01-27 19:42:36.000000 pyxtal-0.5.5/pyxtal/database/bug.json
-drwxr-xr-x   0 qiangzhu   (501) staff       (20)        0 2022-11-18 06:14:45.000000 pyxtal-0.5.5/pyxtal/database/cifs/
--rw-r--r--   0 qiangzhu   (501) staff       (20)     2051 2021-12-27 22:37:10.000000 pyxtal-0.5.5/pyxtal/database/cifs/0-G62.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     1921 2021-11-09 00:08:43.000000 pyxtal-0.5.5/pyxtal/database/cifs/1-G59.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)      367 2021-08-17 15:48:08.000000 pyxtal-0.5.5/pyxtal/database/cifs/191.vasp
--rw-r--r--   0 qiangzhu   (501) staff       (20)     2043 2021-12-27 00:51:46.000000 pyxtal-0.5.5/pyxtal/database/cifs/2-G71.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     2373 2021-12-27 00:21:38.000000 pyxtal-0.5.5/pyxtal/database/cifs/3-G139.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     5688 2021-11-09 00:08:43.000000 pyxtal-0.5.5/pyxtal/database/cifs/4-G225.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     2940 2021-08-17 15:48:08.000000 pyxtal-0.5.5/pyxtal/database/cifs/ACBNZA01.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     9863 2021-08-17 15:48:08.000000 pyxtal-0.5.5/pyxtal/database/cifs/AXOSOW01.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     1184 2022-04-27 19:27:52.000000 pyxtal-0.5.5/pyxtal/database/cifs/Al2SiO5_mp-4753_symmetrized.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     1009 2021-08-17 15:48:08.000000 pyxtal-0.5.5/pyxtal/database/cifs/BTO-Amm2.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     1323 2021-08-17 15:48:08.000000 pyxtal-0.5.5/pyxtal/database/cifs/BTO.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     1534 2022-04-28 13:54:25.000000 pyxtal-0.5.5/pyxtal/database/cifs/CuAu_mp-582681_symmetrized.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     4636 2022-06-17 15:45:22.000000 pyxtal-0.5.5/pyxtal/database/cifs/FAU.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     3542 2021-08-17 15:48:09.000000 pyxtal-0.5.5/pyxtal/database/cifs/Fd3.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     6258 2022-06-17 19:14:34.000000 pyxtal-0.5.5/pyxtal/database/cifs/Fd3.vasp
--rw-r--r--   0 qiangzhu   (501) staff       (20)     4992 2021-12-29 18:59:05.000000 pyxtal-0.5.5/pyxtal/database/cifs/Fd3m.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     9559 2021-08-17 15:48:08.000000 pyxtal-0.5.5/pyxtal/database/cifs/GUMMUW.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)      885 2021-08-17 15:48:08.000000 pyxtal-0.5.5/pyxtal/database/cifs/GeF2.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     2946 2021-08-17 15:48:08.000000 pyxtal-0.5.5/pyxtal/database/cifs/HAHCOI.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)      221 2022-06-17 19:31:24.000000 pyxtal-0.5.5/pyxtal/database/cifs/I41amd.vasp
--rw-r--r--   0 qiangzhu   (501) staff       (20)     1836 2021-08-17 15:48:09.000000 pyxtal-0.5.5/pyxtal/database/cifs/I4_132.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)    10505 2021-08-17 15:48:08.000000 pyxtal-0.5.5/pyxtal/database/cifs/JAPWIH.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)   441469 2021-08-17 15:48:08.000000 pyxtal-0.5.5/pyxtal/database/cifs/LAGNAL.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     7132 2021-08-17 15:48:08.000000 pyxtal-0.5.5/pyxtal/database/cifs/LUFHAW.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     2001 2021-08-17 15:48:08.000000 pyxtal-0.5.5/pyxtal/database/cifs/LiCs.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)    12413 2021-08-17 15:48:08.000000 pyxtal-0.5.5/pyxtal/database/cifs/MERQIM.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     1238 2021-08-17 15:48:08.000000 pyxtal-0.5.5/pyxtal/database/cifs/MPWO.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     4577 2021-08-17 15:48:08.000000 pyxtal-0.5.5/pyxtal/database/cifs/NaCl.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     1416 2021-08-17 15:48:08.000000 pyxtal-0.5.5/pyxtal/database/cifs/NaSb3F10.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     1180 2021-08-17 15:48:08.000000 pyxtal-0.5.5/pyxtal/database/cifs/NbO2.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     1696 2021-08-17 15:48:08.000000 pyxtal-0.5.5/pyxtal/database/cifs/NiS-Cm.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     1134 2021-08-17 15:48:09.000000 pyxtal-0.5.5/pyxtal/database/cifs/P3_112.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     1498 2021-08-17 15:48:09.000000 pyxtal-0.5.5/pyxtal/database/cifs/P4_332.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)      226 2022-06-17 19:18:01.000000 pyxtal-0.5.5/pyxtal/database/cifs/P4nmm.vasp
--rw-r--r--   0 qiangzhu   (501) staff       (20)     1205 2021-08-17 15:48:09.000000 pyxtal-0.5.5/pyxtal/database/cifs/P6_422.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     6482 2021-08-17 15:48:08.000000 pyxtal-0.5.5/pyxtal/database/cifs/PAHYON01.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     1184 2021-08-17 15:48:08.000000 pyxtal-0.5.5/pyxtal/database/cifs/PPO.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     1086 2021-08-17 15:48:08.000000 pyxtal-0.5.5/pyxtal/database/cifs/PVO.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     1222 2021-08-17 15:48:09.000000 pyxtal-0.5.5/pyxtal/database/cifs/Pm3.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)      230 2022-06-17 19:19:37.000000 pyxtal-0.5.5/pyxtal/database/cifs/Pmmn.vasp
--rw-r--r--   0 qiangzhu   (501) staff       (20)      286 2022-06-17 19:13:51.000000 pyxtal-0.5.5/pyxtal/database/cifs/Pn3.vasp
--rw-r--r--   0 qiangzhu   (501) staff       (20)      286 2022-06-17 19:13:21.000000 pyxtal-0.5.5/pyxtal/database/cifs/Pn3m.vasp
--rw-r--r--   0 qiangzhu   (501) staff       (20)     1605 2021-08-17 15:48:09.000000 pyxtal-0.5.5/pyxtal/database/cifs/R-3.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     1933 2021-08-17 15:48:09.000000 pyxtal-0.5.5/pyxtal/database/cifs/R-3c.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)      986 2021-08-17 15:48:09.000000 pyxtal-0.5.5/pyxtal/database/cifs/R32.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     3542 2021-08-17 15:48:08.000000 pyxtal-0.5.5/pyxtal/database/cifs/TMPPIO03.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)    13289 2021-08-17 15:48:08.000000 pyxtal-0.5.5/pyxtal/database/cifs/WEXBOS.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)   177150 2022-06-17 20:12:44.000000 pyxtal-0.5.5/pyxtal/database/cifs/YICMOP.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     2546 2022-07-27 19:22:51.000000 pyxtal-0.5.5/pyxtal/database/cifs/anthracene.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     2703 2021-08-17 15:48:08.000000 pyxtal-0.5.5/pyxtal/database/cifs/aspirin-c.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)    12951 2021-08-17 15:48:08.000000 pyxtal-0.5.5/pyxtal/database/cifs/aspirin.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     1509 2022-07-27 00:49:00.000000 pyxtal-0.5.5/pyxtal/database/cifs/benzene.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)      733 2021-08-17 15:48:08.000000 pyxtal-0.5.5/pyxtal/database/cifs/bug.vasp
--rw-r--r--   0 qiangzhu   (501) staff       (20)    17895 2021-08-17 15:48:08.000000 pyxtal-0.5.5/pyxtal/database/cifs/coumarin.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     2260 2022-01-18 15:40:54.000000 pyxtal-0.5.5/pyxtal/database/cifs/dist_6_0.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     2260 2022-01-18 15:40:53.000000 pyxtal-0.5.5/pyxtal/database/cifs/dist_6_1.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     7884 2021-08-17 15:48:08.000000 pyxtal-0.5.5/pyxtal/database/cifs/gdh.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     1964 2022-08-22 20:08:21.000000 pyxtal-0.5.5/pyxtal/database/cifs/ht_KNbBO.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     5997 2022-08-22 18:10:54.000000 pyxtal-0.5.5/pyxtal/database/cifs/ht_cristobalite.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     1251 2022-08-22 18:21:32.000000 pyxtal-0.5.5/pyxtal/database/cifs/ht_quartz.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     1864 2021-08-17 15:48:08.000000 pyxtal-0.5.5/pyxtal/database/cifs/ice.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     2869 2022-08-22 20:08:21.000000 pyxtal-0.5.5/pyxtal/database/cifs/lt_KNbBO.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)      931 2021-08-17 15:48:08.000000 pyxtal-0.5.5/pyxtal/database/cifs/lt_cristobalite.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)      866 2021-08-17 15:48:08.000000 pyxtal-0.5.5/pyxtal/database/cifs/lt_quartz.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     1541 2022-07-27 00:49:34.000000 pyxtal-0.5.5/pyxtal/database/cifs/naphthalene.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)   317844 2021-11-23 20:29:41.000000 pyxtal-0.5.5/pyxtal/database/cifs/resorcinol.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)      473 2022-01-21 16:08:56.000000 pyxtal-0.5.5/pyxtal/database/cifs/sim-0.vasp
--rw-r--r--   0 qiangzhu   (501) staff       (20)      488 2022-01-21 16:08:55.000000 pyxtal-0.5.5/pyxtal/database/cifs/sim-1.vasp
--rw-r--r--   0 qiangzhu   (501) staff       (20)     4786 2021-08-17 15:48:08.000000 pyxtal-0.5.5/pyxtal/database/cifs/xxvi.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)  1103778 2021-08-17 15:48:08.000000 pyxtal-0.5.5/pyxtal/database/clusters.json
--rw-r--r--   0 qiangzhu   (501) staff       (20)     2617 2022-06-23 00:39:04.000000 pyxtal-0.5.5/pyxtal/database/collection.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)    19164 2022-06-14 14:22:59.000000 pyxtal-0.5.5/pyxtal/database/element.py
--rw-r--r--   0 qiangzhu   (501) staff       (20) 10480157 2021-08-17 15:48:08.000000 pyxtal-0.5.5/pyxtal/database/k_subgroup.json
--rw-r--r--   0 qiangzhu   (501) staff       (20)    20717 2021-08-17 15:48:08.000000 pyxtal-0.5.5/pyxtal/database/layer.csv
--rw-r--r--   0 qiangzhu   (501) staff       (20)    25842 2021-08-17 15:48:08.000000 pyxtal-0.5.5/pyxtal/database/layer_generators.csv
--rw-r--r--   0 qiangzhu   (501) staff       (20)    58872 2021-08-17 15:48:08.000000 pyxtal-0.5.5/pyxtal/database/layer_symmetry.csv
--rw-r--r--   0 qiangzhu   (501) staff       (20)    90734 2021-08-17 15:48:08.000000 pyxtal-0.5.5/pyxtal/database/molecules.json
--rw-r--r--   0 qiangzhu   (501) staff       (20)   130892 2021-08-17 15:48:08.000000 pyxtal-0.5.5/pyxtal/database/point.csv
--rw-r--r--   0 qiangzhu   (501) staff       (20)   146327 2021-08-17 15:48:08.000000 pyxtal-0.5.5/pyxtal/database/point_generators.csv
--rw-r--r--   0 qiangzhu   (501) staff       (20)   301944 2021-08-17 15:48:08.000000 pyxtal-0.5.5/pyxtal/database/point_symmetry.csv
--rw-r--r--   0 qiangzhu   (501) staff       (20)    18501 2021-08-17 15:48:08.000000 pyxtal-0.5.5/pyxtal/database/rod.csv
--rw-r--r--   0 qiangzhu   (501) staff       (20)    21935 2021-08-17 15:48:08.000000 pyxtal-0.5.5/pyxtal/database/rod_generators.csv
--rw-r--r--   0 qiangzhu   (501) staff       (20)    44320 2021-08-17 15:48:08.000000 pyxtal-0.5.5/pyxtal/database/rod_symmetry.csv
--rw-r--r--   0 qiangzhu   (501) staff       (20)     5478 2021-08-17 15:48:08.000000 pyxtal-0.5.5/pyxtal/database/symbols.json
--rw-r--r--   0 qiangzhu   (501) staff       (20)  1245398 2021-08-17 15:48:08.000000 pyxtal-0.5.5/pyxtal/database/t_subgroup.json
--rw-r--r--   0 qiangzhu   (501) staff       (20)   259897 2021-08-17 15:48:08.000000 pyxtal-0.5.5/pyxtal/database/wyckoff_generators.csv
--rw-r--r--   0 qiangzhu   (501) staff       (20)   251719 2021-08-17 15:48:08.000000 pyxtal-0.5.5/pyxtal/database/wyckoff_list.csv
--rw-r--r--   0 qiangzhu   (501) staff       (20)   117892 2021-08-17 15:48:09.000000 pyxtal-0.5.5/pyxtal/database/wyckoff_sets.json
--rw-r--r--   0 qiangzhu   (501) staff       (20)   627207 2021-08-17 15:48:09.000000 pyxtal-0.5.5/pyxtal/database/wyckoff_symmetry.csv
--rw-r--r--   0 qiangzhu   (501) staff       (20)     8405 2022-08-15 16:19:56.000000 pyxtal-0.5.5/pyxtal/db.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)    14642 2022-09-15 04:23:50.000000 pyxtal-0.5.5/pyxtal/descriptor.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)    42770 2022-08-16 23:30:22.000000 pyxtal-0.5.5/pyxtal/elasticity.py
-drwxr-xr-x   0 qiangzhu   (501) staff       (20)        0 2022-11-18 06:14:45.000000 pyxtal-0.5.5/pyxtal/interface/
--rw-r--r--   0 qiangzhu   (501) staff       (20)    13515 2021-08-17 15:48:09.000000 pyxtal-0.5.5/pyxtal/interface/LJ.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)        0 2021-08-17 15:48:09.000000 pyxtal-0.5.5/pyxtal/interface/__init__.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)    25973 2022-11-18 05:09:46.000000 pyxtal-0.5.5/pyxtal/interface/dftb.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)    10231 2021-08-17 15:48:09.000000 pyxtal-0.5.5/pyxtal/interface/gulp.py
--rwxr-xr-x   0 qiangzhu   (501) staff       (20)    19477 2022-01-06 13:19:42.000000 pyxtal-0.5.5/pyxtal/interface/lammpslib.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)     8403 2021-08-17 15:48:09.000000 pyxtal-0.5.5/pyxtal/interface/vasp.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)    31490 2021-08-17 15:48:09.000000 pyxtal-0.5.5/pyxtal/interface/vasprun.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)    23034 2022-09-24 05:16:49.000000 pyxtal-0.5.5/pyxtal/io.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)    66090 2022-07-08 03:35:56.000000 pyxtal-0.5.5/pyxtal/lattice.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)    17952 2022-09-15 04:47:12.000000 pyxtal-0.5.5/pyxtal/molecular_crystal.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)    63216 2022-11-18 06:08:23.000000 pyxtal-0.5.5/pyxtal/molecule.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)     2758 2022-08-09 01:18:08.000000 pyxtal-0.5.5/pyxtal/msg.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)    30344 2022-08-15 15:30:42.000000 pyxtal-0.5.5/pyxtal/operations.py
-drwxr-xr-x   0 qiangzhu   (501) staff       (20)        0 2022-11-18 06:14:45.000000 pyxtal-0.5.5/pyxtal/optimize/
--rw-r--r--   0 qiangzhu   (501) staff       (20)        0 2021-08-17 15:48:09.000000 pyxtal-0.5.5/pyxtal/optimize/__init__.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)     5636 2021-08-17 15:48:09.000000 pyxtal-0.5.5/pyxtal/optimize/fire.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)    12084 2021-08-17 15:48:09.000000 pyxtal-0.5.5/pyxtal/optimize/fire2.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)    14967 2021-08-17 15:48:09.000000 pyxtal-0.5.5/pyxtal/optimize/myscipy_optimize.py
-drwxr-xr-x   0 qiangzhu   (501) staff       (20)        0 2022-11-18 06:14:45.000000 pyxtal-0.5.5/pyxtal/potentials/
--rw-r--r--   0 qiangzhu   (501) staff       (20)  1820580 2021-08-17 15:48:09.000000 pyxtal-0.5.5/pyxtal/potentials/CuAg.eam.alloy
--rw-r--r--   0 qiangzhu   (501) staff       (20)     1652 2021-08-17 15:48:09.000000 pyxtal-0.5.5/pyxtal/potentials/LJ_cluster.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)      837 2021-08-17 15:48:09.000000 pyxtal-0.5.5/pyxtal/potentials/Si.tersoff
--rw-r--r--   0 qiangzhu   (501) staff       (20)     3991 2021-08-17 15:48:09.000000 pyxtal-0.5.5/pyxtal/potentials/SiCGe.tersoff
--rwxr-xr-x   0 qiangzhu   (501) staff       (20)       26 2021-08-17 15:48:09.000000 pyxtal-0.5.5/pyxtal/potentials/__init__.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)    12283 2022-07-08 03:33:23.000000 pyxtal-0.5.5/pyxtal/representation.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)    46514 2022-08-24 01:56:03.000000 pyxtal-0.5.5/pyxtal/supergroup.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)   126770 2022-08-22 17:06:56.000000 pyxtal-0.5.5/pyxtal/symmetry.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)    41831 2022-09-15 04:47:01.000000 pyxtal-0.5.5/pyxtal/test_all.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)    11061 2022-06-20 18:26:47.000000 pyxtal-0.5.5/pyxtal/tolerance.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)    14460 2022-08-13 02:06:51.000000 pyxtal-0.5.5/pyxtal/util.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)       22 2022-11-18 06:10:02.000000 pyxtal-0.5.5/pyxtal/version.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)    13329 2022-09-09 18:39:24.000000 pyxtal-0.5.5/pyxtal/viz.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)    38900 2022-08-13 13:18:51.000000 pyxtal-0.5.5/pyxtal/wyckoff_site.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)    21311 2022-08-22 20:18:26.000000 pyxtal-0.5.5/pyxtal/wyckoff_split.py
-drwxr-xr-x   0 qiangzhu   (501) staff       (20)        0 2022-11-18 06:14:45.000000 pyxtal-0.5.5/pyxtal.egg-info/
--rw-r--r--   0 qiangzhu   (501) staff       (20)     5203 2022-11-18 06:14:45.000000 pyxtal-0.5.5/pyxtal.egg-info/PKG-INFO
--rw-r--r--   0 qiangzhu   (501) staff       (20)     4217 2022-11-18 06:14:45.000000 pyxtal-0.5.5/pyxtal.egg-info/SOURCES.txt
--rw-r--r--   0 qiangzhu   (501) staff       (20)        1 2022-11-18 06:14:45.000000 pyxtal-0.5.5/pyxtal.egg-info/dependency_links.txt
--rw-r--r--   0 qiangzhu   (501) staff       (20)      158 2022-11-18 06:14:45.000000 pyxtal-0.5.5/pyxtal.egg-info/requires.txt
--rw-r--r--   0 qiangzhu   (501) staff       (20)        7 2022-11-18 06:14:45.000000 pyxtal-0.5.5/pyxtal.egg-info/top_level.txt
-drwxr-xr-x   0 qiangzhu   (501) staff       (20)        0 2022-11-18 06:14:45.000000 pyxtal-0.5.5/scripts/
--rwxr-xr-x   0 qiangzhu   (501) staff       (20)     3973 2021-08-17 15:48:09.000000 pyxtal-0.5.5/scripts/pyxtal_main.py
--rwxr-xr-x   0 qiangzhu   (501) staff       (20)      960 2021-08-17 15:48:09.000000 pyxtal-0.5.5/scripts/pyxtal_symmetry.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)      125 2022-11-18 06:14:45.000000 pyxtal-0.5.5/setup.cfg
--rwxr-xr-x   0 qiangzhu   (501) staff       (20)     1796 2022-09-15 04:14:56.000000 pyxtal-0.5.5/setup.py
+drwxr-xr-x   0 qiangzhu   (501) staff       (20)        0 2023-06-09 17:12:42.000000 pyxtal-0.5.6/
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     1084 2022-06-13 19:36:20.000000 pyxtal-0.5.6/LICENSE.txt
+-rwxr-xr-x   0 qiangzhu   (501) staff       (20)       82 2022-06-15 16:30:37.000000 pyxtal-0.5.6/MANIFEST.in
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     5203 2023-06-09 17:12:42.000000 pyxtal-0.5.6/PKG-INFO
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     4692 2022-07-27 22:43:15.000000 pyxtal-0.5.6/README.md
+drwxr-xr-x   0 qiangzhu   (501) staff       (20)        0 2023-06-09 17:12:42.000000 pyxtal-0.5.6/pyxtal/
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    31648 2022-08-14 23:14:59.000000 pyxtal-0.5.6/pyxtal/XRD.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)   100907 2023-06-09 15:11:50.000000 pyxtal-0.5.6/pyxtal/__init__.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     5985 2022-06-21 15:19:36.000000 pyxtal-0.5.6/pyxtal/block_crystal.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     1784 2022-06-23 22:59:32.000000 pyxtal-0.5.6/pyxtal/constants.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    13810 2022-06-21 13:41:23.000000 pyxtal-0.5.6/pyxtal/crystal.py
+drwxr-xr-x   0 qiangzhu   (501) staff       (20)        0 2023-06-09 17:12:42.000000 pyxtal-0.5.6/pyxtal/database/
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    22281 2022-06-17 19:11:39.000000 pyxtal-0.5.6/pyxtal/database/HM_Full.csv
+-rw-r--r--   0 qiangzhu   (501) staff       (20)        0 2021-08-17 15:48:08.000000 pyxtal-0.5.6/pyxtal/database/__init__.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     6824 2021-08-17 15:48:08.000000 pyxtal-0.5.6/pyxtal/database/atomic_scattering_params.json
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     2120 2022-08-11 19:04:42.000000 pyxtal-0.5.6/pyxtal/database/bonds.json
+-rw-------   0 qiangzhu   (501) staff       (20)     2950 2022-01-27 19:42:36.000000 pyxtal-0.5.6/pyxtal/database/bug.json
+drwxr-xr-x   0 qiangzhu   (501) staff       (20)        0 2023-06-09 17:12:42.000000 pyxtal-0.5.6/pyxtal/database/cifs/
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     2051 2021-12-27 22:37:10.000000 pyxtal-0.5.6/pyxtal/database/cifs/0-G62.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     1921 2021-11-09 00:08:43.000000 pyxtal-0.5.6/pyxtal/database/cifs/1-G59.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)      367 2021-08-17 15:48:08.000000 pyxtal-0.5.6/pyxtal/database/cifs/191.vasp
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     2043 2021-12-27 00:51:46.000000 pyxtal-0.5.6/pyxtal/database/cifs/2-G71.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     2373 2021-12-27 00:21:38.000000 pyxtal-0.5.6/pyxtal/database/cifs/3-G139.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     5688 2021-11-09 00:08:43.000000 pyxtal-0.5.6/pyxtal/database/cifs/4-G225.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     2940 2021-08-17 15:48:08.000000 pyxtal-0.5.6/pyxtal/database/cifs/ACBNZA01.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     9863 2021-08-17 15:48:08.000000 pyxtal-0.5.6/pyxtal/database/cifs/AXOSOW01.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     1184 2022-04-27 19:27:52.000000 pyxtal-0.5.6/pyxtal/database/cifs/Al2SiO5_mp-4753_symmetrized.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     1009 2021-08-17 15:48:08.000000 pyxtal-0.5.6/pyxtal/database/cifs/BTO-Amm2.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     1323 2021-08-17 15:48:08.000000 pyxtal-0.5.6/pyxtal/database/cifs/BTO.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     1534 2022-04-28 13:54:25.000000 pyxtal-0.5.6/pyxtal/database/cifs/CuAu_mp-582681_symmetrized.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     4636 2022-06-17 15:45:22.000000 pyxtal-0.5.6/pyxtal/database/cifs/FAU.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     3542 2021-08-17 15:48:09.000000 pyxtal-0.5.6/pyxtal/database/cifs/Fd3.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     6258 2022-06-17 19:14:34.000000 pyxtal-0.5.6/pyxtal/database/cifs/Fd3.vasp
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     4992 2021-12-29 18:59:05.000000 pyxtal-0.5.6/pyxtal/database/cifs/Fd3m.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     9559 2021-08-17 15:48:08.000000 pyxtal-0.5.6/pyxtal/database/cifs/GUMMUW.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)      885 2021-08-17 15:48:08.000000 pyxtal-0.5.6/pyxtal/database/cifs/GeF2.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     2946 2021-08-17 15:48:08.000000 pyxtal-0.5.6/pyxtal/database/cifs/HAHCOI.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)      221 2022-06-17 19:31:24.000000 pyxtal-0.5.6/pyxtal/database/cifs/I41amd.vasp
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     1836 2021-08-17 15:48:09.000000 pyxtal-0.5.6/pyxtal/database/cifs/I4_132.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    10505 2021-08-17 15:48:08.000000 pyxtal-0.5.6/pyxtal/database/cifs/JAPWIH.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)   441469 2021-08-17 15:48:08.000000 pyxtal-0.5.6/pyxtal/database/cifs/LAGNAL.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     7132 2021-08-17 15:48:08.000000 pyxtal-0.5.6/pyxtal/database/cifs/LUFHAW.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     2001 2021-08-17 15:48:08.000000 pyxtal-0.5.6/pyxtal/database/cifs/LiCs.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    12413 2021-08-17 15:48:08.000000 pyxtal-0.5.6/pyxtal/database/cifs/MERQIM.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     1238 2021-08-17 15:48:08.000000 pyxtal-0.5.6/pyxtal/database/cifs/MPWO.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     4577 2021-08-17 15:48:08.000000 pyxtal-0.5.6/pyxtal/database/cifs/NaCl.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     1416 2021-08-17 15:48:08.000000 pyxtal-0.5.6/pyxtal/database/cifs/NaSb3F10.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     1180 2021-08-17 15:48:08.000000 pyxtal-0.5.6/pyxtal/database/cifs/NbO2.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     1696 2021-08-17 15:48:08.000000 pyxtal-0.5.6/pyxtal/database/cifs/NiS-Cm.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     1134 2021-08-17 15:48:09.000000 pyxtal-0.5.6/pyxtal/database/cifs/P3_112.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     1498 2021-08-17 15:48:09.000000 pyxtal-0.5.6/pyxtal/database/cifs/P4_332.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)      226 2022-06-17 19:18:01.000000 pyxtal-0.5.6/pyxtal/database/cifs/P4nmm.vasp
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     1205 2021-08-17 15:48:09.000000 pyxtal-0.5.6/pyxtal/database/cifs/P6_422.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     6482 2021-08-17 15:48:08.000000 pyxtal-0.5.6/pyxtal/database/cifs/PAHYON01.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     1184 2021-08-17 15:48:08.000000 pyxtal-0.5.6/pyxtal/database/cifs/PPO.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     1086 2021-08-17 15:48:08.000000 pyxtal-0.5.6/pyxtal/database/cifs/PVO.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     1222 2021-08-17 15:48:09.000000 pyxtal-0.5.6/pyxtal/database/cifs/Pm3.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)      230 2022-06-17 19:19:37.000000 pyxtal-0.5.6/pyxtal/database/cifs/Pmmn.vasp
+-rw-r--r--   0 qiangzhu   (501) staff       (20)      286 2022-06-17 19:13:51.000000 pyxtal-0.5.6/pyxtal/database/cifs/Pn3.vasp
+-rw-r--r--   0 qiangzhu   (501) staff       (20)      286 2022-06-17 19:13:21.000000 pyxtal-0.5.6/pyxtal/database/cifs/Pn3m.vasp
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     1605 2021-08-17 15:48:09.000000 pyxtal-0.5.6/pyxtal/database/cifs/R-3.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     1933 2021-08-17 15:48:09.000000 pyxtal-0.5.6/pyxtal/database/cifs/R-3c.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)      986 2021-08-17 15:48:09.000000 pyxtal-0.5.6/pyxtal/database/cifs/R32.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     3542 2021-08-17 15:48:08.000000 pyxtal-0.5.6/pyxtal/database/cifs/TMPPIO03.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    13289 2021-08-17 15:48:08.000000 pyxtal-0.5.6/pyxtal/database/cifs/WEXBOS.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)   177150 2022-06-17 20:12:44.000000 pyxtal-0.5.6/pyxtal/database/cifs/YICMOP.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     2546 2022-07-27 19:22:51.000000 pyxtal-0.5.6/pyxtal/database/cifs/anthracene.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     2703 2021-08-17 15:48:08.000000 pyxtal-0.5.6/pyxtal/database/cifs/aspirin-c.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    12951 2021-08-17 15:48:08.000000 pyxtal-0.5.6/pyxtal/database/cifs/aspirin.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     1509 2022-07-27 00:49:00.000000 pyxtal-0.5.6/pyxtal/database/cifs/benzene.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)      733 2021-08-17 15:48:08.000000 pyxtal-0.5.6/pyxtal/database/cifs/bug.vasp
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    17895 2021-08-17 15:48:08.000000 pyxtal-0.5.6/pyxtal/database/cifs/coumarin.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     2260 2022-01-18 15:40:54.000000 pyxtal-0.5.6/pyxtal/database/cifs/dist_6_0.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     2260 2022-01-18 15:40:53.000000 pyxtal-0.5.6/pyxtal/database/cifs/dist_6_1.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     7884 2021-08-17 15:48:08.000000 pyxtal-0.5.6/pyxtal/database/cifs/gdh.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     1964 2022-08-22 20:08:21.000000 pyxtal-0.5.6/pyxtal/database/cifs/ht_KNbBO.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     5997 2022-08-22 18:10:54.000000 pyxtal-0.5.6/pyxtal/database/cifs/ht_cristobalite.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     1251 2022-08-22 18:21:32.000000 pyxtal-0.5.6/pyxtal/database/cifs/ht_quartz.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     1864 2021-08-17 15:48:08.000000 pyxtal-0.5.6/pyxtal/database/cifs/ice.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     2869 2022-08-22 20:08:21.000000 pyxtal-0.5.6/pyxtal/database/cifs/lt_KNbBO.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)      931 2021-08-17 15:48:08.000000 pyxtal-0.5.6/pyxtal/database/cifs/lt_cristobalite.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)      866 2021-08-17 15:48:08.000000 pyxtal-0.5.6/pyxtal/database/cifs/lt_quartz.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     1541 2022-07-27 00:49:34.000000 pyxtal-0.5.6/pyxtal/database/cifs/naphthalene.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)   317844 2021-11-23 20:29:41.000000 pyxtal-0.5.6/pyxtal/database/cifs/resorcinol.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)      473 2022-01-21 16:08:56.000000 pyxtal-0.5.6/pyxtal/database/cifs/sim-0.vasp
+-rw-r--r--   0 qiangzhu   (501) staff       (20)      488 2022-01-21 16:08:55.000000 pyxtal-0.5.6/pyxtal/database/cifs/sim-1.vasp
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     4786 2021-08-17 15:48:08.000000 pyxtal-0.5.6/pyxtal/database/cifs/xxvi.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)  1103778 2021-08-17 15:48:08.000000 pyxtal-0.5.6/pyxtal/database/clusters.json
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     2617 2022-06-23 00:39:04.000000 pyxtal-0.5.6/pyxtal/database/collection.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    19164 2022-06-14 14:22:59.000000 pyxtal-0.5.6/pyxtal/database/element.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20) 10480157 2021-08-17 15:48:08.000000 pyxtal-0.5.6/pyxtal/database/k_subgroup.json
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    20717 2021-08-17 15:48:08.000000 pyxtal-0.5.6/pyxtal/database/layer.csv
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    25842 2021-08-17 15:48:08.000000 pyxtal-0.5.6/pyxtal/database/layer_generators.csv
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    58872 2021-08-17 15:48:08.000000 pyxtal-0.5.6/pyxtal/database/layer_symmetry.csv
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    90734 2021-08-17 15:48:08.000000 pyxtal-0.5.6/pyxtal/database/molecules.json
+-rw-r--r--   0 qiangzhu   (501) staff       (20)   130892 2021-08-17 15:48:08.000000 pyxtal-0.5.6/pyxtal/database/point.csv
+-rw-r--r--   0 qiangzhu   (501) staff       (20)   146327 2021-08-17 15:48:08.000000 pyxtal-0.5.6/pyxtal/database/point_generators.csv
+-rw-r--r--   0 qiangzhu   (501) staff       (20)   301944 2021-08-17 15:48:08.000000 pyxtal-0.5.6/pyxtal/database/point_symmetry.csv
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    18501 2021-08-17 15:48:08.000000 pyxtal-0.5.6/pyxtal/database/rod.csv
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    21935 2021-08-17 15:48:08.000000 pyxtal-0.5.6/pyxtal/database/rod_generators.csv
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    44320 2021-08-17 15:48:08.000000 pyxtal-0.5.6/pyxtal/database/rod_symmetry.csv
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     5478 2021-08-17 15:48:08.000000 pyxtal-0.5.6/pyxtal/database/symbols.json
+-rw-r--r--   0 qiangzhu   (501) staff       (20)  1245398 2021-08-17 15:48:08.000000 pyxtal-0.5.6/pyxtal/database/t_subgroup.json
+-rw-r--r--   0 qiangzhu   (501) staff       (20)   259897 2021-08-17 15:48:08.000000 pyxtal-0.5.6/pyxtal/database/wyckoff_generators.csv
+-rw-r--r--   0 qiangzhu   (501) staff       (20)   251719 2021-08-17 15:48:08.000000 pyxtal-0.5.6/pyxtal/database/wyckoff_list.csv
+-rw-r--r--   0 qiangzhu   (501) staff       (20)   117892 2021-08-17 15:48:09.000000 pyxtal-0.5.6/pyxtal/database/wyckoff_sets.json
+-rw-r--r--   0 qiangzhu   (501) staff       (20)   627207 2021-08-17 15:48:09.000000 pyxtal-0.5.6/pyxtal/database/wyckoff_symmetry.csv
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     8405 2023-06-03 17:11:12.000000 pyxtal-0.5.6/pyxtal/db.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    18767 2023-01-09 17:49:14.000000 pyxtal-0.5.6/pyxtal/descriptor.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    42770 2023-04-04 17:06:21.000000 pyxtal-0.5.6/pyxtal/elasticity.py
+drwxr-xr-x   0 qiangzhu   (501) staff       (20)        0 2023-06-09 17:12:42.000000 pyxtal-0.5.6/pyxtal/interface/
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    13515 2021-08-17 15:48:09.000000 pyxtal-0.5.6/pyxtal/interface/LJ.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)        0 2021-08-17 15:48:09.000000 pyxtal-0.5.6/pyxtal/interface/__init__.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    27549 2023-01-11 02:44:28.000000 pyxtal-0.5.6/pyxtal/interface/dftb.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    10599 2023-06-05 08:33:21.000000 pyxtal-0.5.6/pyxtal/interface/gulp.py
+-rwxr-xr-x   0 qiangzhu   (501) staff       (20)    19477 2022-01-06 13:19:42.000000 pyxtal-0.5.6/pyxtal/interface/lammpslib.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     8403 2021-08-17 15:48:09.000000 pyxtal-0.5.6/pyxtal/interface/vasp.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    31490 2021-08-17 15:48:09.000000 pyxtal-0.5.6/pyxtal/interface/vasprun.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    23034 2022-09-24 05:16:49.000000 pyxtal-0.5.6/pyxtal/io.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    67422 2023-06-05 17:26:36.000000 pyxtal-0.5.6/pyxtal/lattice.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    17952 2022-09-15 04:47:12.000000 pyxtal-0.5.6/pyxtal/molecular_crystal.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    63216 2022-11-18 06:08:23.000000 pyxtal-0.5.6/pyxtal/molecule.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     2758 2022-08-09 01:18:08.000000 pyxtal-0.5.6/pyxtal/msg.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    30344 2022-08-15 15:30:42.000000 pyxtal-0.5.6/pyxtal/operations.py
+drwxr-xr-x   0 qiangzhu   (501) staff       (20)        0 2023-06-09 17:12:42.000000 pyxtal-0.5.6/pyxtal/optimize/
+-rw-r--r--   0 qiangzhu   (501) staff       (20)        0 2021-08-17 15:48:09.000000 pyxtal-0.5.6/pyxtal/optimize/__init__.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     5636 2021-08-17 15:48:09.000000 pyxtal-0.5.6/pyxtal/optimize/fire.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    12084 2021-08-17 15:48:09.000000 pyxtal-0.5.6/pyxtal/optimize/fire2.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    14967 2021-08-17 15:48:09.000000 pyxtal-0.5.6/pyxtal/optimize/myscipy_optimize.py
+drwxr-xr-x   0 qiangzhu   (501) staff       (20)        0 2023-06-09 17:12:42.000000 pyxtal-0.5.6/pyxtal/potentials/
+-rw-r--r--   0 qiangzhu   (501) staff       (20)  1820580 2021-08-17 15:48:09.000000 pyxtal-0.5.6/pyxtal/potentials/CuAg.eam.alloy
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     1652 2021-08-17 15:48:09.000000 pyxtal-0.5.6/pyxtal/potentials/LJ_cluster.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)      837 2021-08-17 15:48:09.000000 pyxtal-0.5.6/pyxtal/potentials/Si.tersoff
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     3991 2021-08-17 15:48:09.000000 pyxtal-0.5.6/pyxtal/potentials/SiCGe.tersoff
+-rwxr-xr-x   0 qiangzhu   (501) staff       (20)       26 2021-08-17 15:48:09.000000 pyxtal-0.5.6/pyxtal/potentials/__init__.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    16730 2023-06-03 11:57:07.000000 pyxtal-0.5.6/pyxtal/representation.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    46380 2023-06-05 08:59:34.000000 pyxtal-0.5.6/pyxtal/supergroup.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)   127177 2023-06-06 20:16:19.000000 pyxtal-0.5.6/pyxtal/symmetry.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    42070 2023-06-05 08:51:40.000000 pyxtal-0.5.6/pyxtal/test_all.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    11061 2022-06-20 18:26:47.000000 pyxtal-0.5.6/pyxtal/tolerance.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    16025 2023-04-04 16:58:20.000000 pyxtal-0.5.6/pyxtal/util.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)       22 2023-06-01 23:30:13.000000 pyxtal-0.5.6/pyxtal/version.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    13329 2022-09-09 18:39:24.000000 pyxtal-0.5.6/pyxtal/viz.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    39382 2023-06-09 13:57:18.000000 pyxtal-0.5.6/pyxtal/wyckoff_site.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    21212 2023-06-05 08:57:39.000000 pyxtal-0.5.6/pyxtal/wyckoff_split.py
+drwxr-xr-x   0 qiangzhu   (501) staff       (20)        0 2023-06-09 17:12:42.000000 pyxtal-0.5.6/pyxtal.egg-info/
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     5203 2023-06-09 17:12:42.000000 pyxtal-0.5.6/pyxtal.egg-info/PKG-INFO
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     4217 2023-06-09 17:12:42.000000 pyxtal-0.5.6/pyxtal.egg-info/SOURCES.txt
+-rw-r--r--   0 qiangzhu   (501) staff       (20)        1 2023-06-09 17:12:42.000000 pyxtal-0.5.6/pyxtal.egg-info/dependency_links.txt
+-rw-r--r--   0 qiangzhu   (501) staff       (20)      158 2023-06-09 17:12:42.000000 pyxtal-0.5.6/pyxtal.egg-info/requires.txt
+-rw-r--r--   0 qiangzhu   (501) staff       (20)        7 2023-06-09 17:12:42.000000 pyxtal-0.5.6/pyxtal.egg-info/top_level.txt
+drwxr-xr-x   0 qiangzhu   (501) staff       (20)        0 2023-06-09 17:12:42.000000 pyxtal-0.5.6/scripts/
+-rwxr-xr-x   0 qiangzhu   (501) staff       (20)     3973 2021-08-17 15:48:09.000000 pyxtal-0.5.6/scripts/pyxtal_main.py
+-rwxr-xr-x   0 qiangzhu   (501) staff       (20)      960 2021-08-17 15:48:09.000000 pyxtal-0.5.6/scripts/pyxtal_symmetry.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)      125 2023-06-09 17:12:42.000000 pyxtal-0.5.6/setup.cfg
+-rwxr-xr-x   0 qiangzhu   (501) staff       (20)     1796 2022-09-15 04:14:56.000000 pyxtal-0.5.6/setup.py
```

### Comparing `pyxtal-0.5.5/LICENSE.txt` & `pyxtal-0.5.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/PKG-INFO` & `pyxtal-0.5.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyxtal
-Version: 0.5.5
+Version: 0.5.6
 Summary: Python code for generation of crystal structures based on symmetry constraints.
 Home-page: https://github.com/qzhu2017/PyXtal
 Author: Scott Fredericks, Qiang Zhu
 Author-email: qiang.zhu@unlv.edu
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyxtal-0.5.5/README.md` & `pyxtal-0.5.6/README.md`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/pyxtal/XRD.py` & `pyxtal-0.5.6/pyxtal/XRD.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/pyxtal/__init__.py` & `pyxtal-0.5.6/pyxtal/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from pyxtal.symmetry import Group, Wyckoff_position
 from pyxtal.operations import apply_ops, SymmOp, get_inverse
 from pyxtal.wyckoff_site import atom_site, mol_site
 from pyxtal.wyckoff_split import wyckoff_split
 from pyxtal.molecule import pyxtal_molecule
 from pyxtal.lattice import Lattice
 from pyxtal.tolerance import Tol_matrix
-from pyxtal.representation import representation
+from pyxtal.representation import representation, representation_atom
 from pyxtal.io import read_cif, write_cif, structure_from_ext
 from pyxtal.constants import letters
 from pyxtal.viz import display_molecular, display_atomic, display_cluster
 from pyxtal.constants import letters
 from pyxtal.descriptor import spherical_image
 
 # name = "pyxtal"
@@ -242,15 +242,15 @@
             names = [site.molecule.name for site in sites]
         else:
             sites = self.atom_sites
             names = [site.specie for site in sites]
 
         dicts = {}
         for name, site in zip(names, sites):
-            label = str(site.wp.multiplicity) + site.wp.letter
+            label = site.wp.get_label() 
             if name not in dicts.keys():
                 dicts[name] = [label]
             else:
                 dicts[name].append(label)
         return dicts
 
 
@@ -907,15 +907,15 @@
             raise RuntimeError("Cannot find the splitter")
 
         if self.molecular:
             struc_sites = self.mol_sites
         else:
             struc_sites = self.atom_sites
 
-        sites = [str(site.wp.multiplicity)+site.wp.letter for site in struc_sites]
+        sites = [site.wp.get_label() for site in struc_sites]
 
         return idx, sites, t_types, k_types
 
     def _subgroup_by_splitter(self, splitter, eps=0.05, mut_lat=False):
         """
         Transform the crystal to subgroup symmetry from a splitter object
 
@@ -1091,20 +1091,24 @@
             numspecies = self.numMols
             species = [str(mol) for mol in self.molecules]
             #print(species, numspecies)
         else:
             specie_list = []
             for site in self.atom_sites:
                 specie_list.extend([site.specie]*site.wp.multiplicity)
-            species = list(set(specie_list))
+            if self.species is None:
+                species = list(set(specie_list))
+                self.species = species
+            else:
+                species = self.species
+
             numIons = np.zeros(len(species), dtype=int)
             for i, sp in enumerate(species):
                 numIons[i] = specie_list.count(sp)
             self.numIons = numIons
-            self.species = species
             numspecies = self.numIons
         for i, s in zip(numspecies, species):
             formula += "{:s}{:d}".format(s, int(i))
         self.formula = formula
 
     def get_zprime(self, integer=False):
         """
@@ -1296,15 +1300,18 @@
         """
         pass
 
     def get_1D_representation(self):
         """
         Get the 1D representation class for molecular crystals
         """
-        return representation.from_pyxtal(self)
+        if self.molecular:
+            return representation.from_pyxtal(self)
+        else:
+            return representation_atom.from_pyxtal(self)
 
     def transform(self, trans, lattice=None):
         """
         Perform cell transformation and symmetry operation
 
         Args:
             trans: 3*3 matrix
@@ -1458,14 +1465,15 @@
 
         self.group = Group(group)
         self.lattice = lattice
         self.dim = 3
         self.factor = 1.0
         self.PBC = [1, 1, 1]
         self.numIons = numIons
+        self.species = species
         numIons_added = np.zeros(len(numIons), dtype=int)
         _sites = []
 
         if len(sites) != len(species):
             raise RuntimeError("Inconsistency between sites and species")
 
         for sp, wps in zip(species, sites):
@@ -1536,14 +1544,28 @@
         """
         A short cut to symmetrize the structure in the stardard setting
         """
         if self.molecular:
             pmg = self.to_pymatgen()
             self.from_seed(pmg, molecules=self.molecules, standard=True)
 
+    def resort_species(self, species):
+        """
+        resort the atomic species
+        """
+        sp1 = deepcopy(species).sort()
+        sp2 = deepcopy(self.species).sort()
+        if sp1 == sp2:
+            self.species = species
+            self.resort()
+            #self._get_formula()
+            #print("=========Sort", species, self.species)
+        else:
+            raise ValueError("the species are inconsistent", species, self.sepecies)
+
     def resort(self):
         """
         A short cut to resort the sites by self.molecules or self.species
         """
         ids = []
         if self.molecular:
             for mol in self.molecules:
@@ -1553,14 +1575,15 @@
             self.mol_sites = [self.mol_sites[j] for j in ids]
         else:
             for specie in self.species:
                 for j, site in enumerate(self.atom_sites):
                     if site.specie == specie and j not in ids:
                         ids.append(j)
             self.atom_sites = [self.atom_sites[j] for j in ids]
+            #print(self.atom_sites)
 
     def _get_alternative(self, wyc_sets, index, ref_lat=None, d_tol=2.0, f_tol=0.15):
         """
         Get alternative structure representations
 
         Args:
             wyc_sets: dictionary of `Coset Representative` and `Transformed WP`
@@ -2053,15 +2076,15 @@
             elements: ['Si', 'O']
             sites: [['4b'], ['4a','4a']]
         """
         elements = []
         sites = []
         for at_site in self.atom_sites:
             e = at_site.specie
-            site = str(at_site.wp.multiplicity) + at_site.wp.letter
+            site = at_site.wp.get_label() 
             if e not in elements:
                 elements.append(e)
                 sites.append([site])
             else:
                 id = elements.index(e)
                 sites[id].append(site)
         return elements, sites
@@ -2534,14 +2557,66 @@
                     #print("add sites", i, m)
                     break
 
         self.molecules = molecules
         self.numMols = numMols
         self.mol_sites = sites
 
+    def set_cutoff(self):
+        """
+        get the cutoff dictionary
+        """
+        cutoff = {}
+        tm = Tol_matrix(prototype="molecular")
+        for i in range(len(self.species)):
+            s1 = self.species[i]
+            for j in range(i, len(self.species)):
+                s2 = self.species[j]
+                tuple_elements = (s1, s2)
+                cutoff[tuple_elements] = tm.get_tol(s1, s2)
+
+        self.cutoff = cutoff
+
+    def set_site_coordination(self, cutoff=None, verbose=False):
+        """
+        Compute the coordination number from each atomic site 
+        """
+        from ase.neighborlist import neighbor_list
+
+        if cutoff is None:
+            if not hasattr(self, 'cutoff'):
+                self.set_cutoff()
+            cutoff = self.cutoff
+
+        if verbose:
+            print("\n The cutoff values for CN calculation are")
+            print(cutoff)
+
+        atoms = self.to_ase(resort=False)
+        NL = neighbor_list('i', atoms, cutoff)
+        coords = np.bincount(NL)
+
+        count = 0
+        for site in self.atom_sites:
+            site.coordination = coords[count]
+            count += site.multiplicity
+
+    def get_dimensionality(self, cutoff=None):
+        """
+        A quick wrapper to compute dimensionality from pymatgen
+        https://pymatgen.org/pymatgen.analysis.dimensionality.html
+        The dimensionality of the structure can be 1/2/3
+        """
+        from pymatgen.analysis.dimensionality import get_dimensionality_gorai
+        if cutoff is None:
+            if not hasattr(self, 'cutoff'):
+                self.set_cutoff()
+            cutoff = self.cutoff
+
+        return get_dimensionality_gorai(self.to_pymatgen(), bonds=cutoff)
 
     def from_CSD(self, csd_code):
         """
         Download the crystal from CCDC
         if csd_code is given, return the single pyxtal object
         if csd_family is given, do group analysis and ignore high pressure form
```

### Comparing `pyxtal-0.5.5/pyxtal/block_crystal.py` & `pyxtal-0.5.6/pyxtal/block_crystal.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/pyxtal/constants.py` & `pyxtal-0.5.6/pyxtal/constants.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/pyxtal/crystal.py` & `pyxtal-0.5.6/pyxtal/crystal.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/pyxtal/database/HM_Full.csv` & `pyxtal-0.5.6/pyxtal/database/HM_Full.csv`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/pyxtal/database/atomic_scattering_params.json` & `pyxtal-0.5.6/pyxtal/database/atomic_scattering_params.json`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/pyxtal/database/bonds.json` & `pyxtal-0.5.6/pyxtal/database/bonds.json`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/pyxtal/database/bug.json` & `pyxtal-0.5.6/pyxtal/database/bug.json`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/pyxtal/database/cifs/0-G62.cif` & `pyxtal-0.5.6/pyxtal/database/cifs/0-G62.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/pyxtal/database/cifs/1-G59.cif` & `pyxtal-0.5.6/pyxtal/database/cifs/1-G59.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/pyxtal/database/cifs/2-G71.cif` & `pyxtal-0.5.6/pyxtal/database/cifs/2-G71.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/pyxtal/database/cifs/3-G139.cif` & `pyxtal-0.5.6/pyxtal/database/cifs/3-G139.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/pyxtal/database/cifs/4-G225.cif` & `pyxtal-0.5.6/pyxtal/database/cifs/4-G225.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/pyxtal/database/cifs/ACBNZA01.cif` & `pyxtal-0.5.6/pyxtal/database/cifs/ACBNZA01.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/pyxtal/database/cifs/AXOSOW01.cif` & `pyxtal-0.5.6/pyxtal/database/cifs/AXOSOW01.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/pyxtal/database/cifs/Al2SiO5_mp-4753_symmetrized.cif` & `pyxtal-0.5.6/pyxtal/database/cifs/Al2SiO5_mp-4753_symmetrized.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/pyxtal/database/cifs/BTO-Amm2.cif` & `pyxtal-0.5.6/pyxtal/database/cifs/BTO-Amm2.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/pyxtal/database/cifs/BTO.cif` & `pyxtal-0.5.6/pyxtal/database/cifs/BTO.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/pyxtal/database/cifs/CuAu_mp-582681_symmetrized.cif` & `pyxtal-0.5.6/pyxtal/database/cifs/CuAu_mp-582681_symmetrized.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/pyxtal/database/cifs/FAU.cif` & `pyxtal-0.5.6/pyxtal/database/cifs/FAU.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/pyxtal/database/cifs/Fd3.cif` & `pyxtal-0.5.6/pyxtal/database/cifs/Fd3.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/pyxtal/database/cifs/Fd3.vasp` & `pyxtal-0.5.6/pyxtal/database/cifs/Fd3.vasp`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/pyxtal/database/cifs/Fd3m.cif` & `pyxtal-0.5.6/pyxtal/database/cifs/Fd3m.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/pyxtal/database/cifs/GUMMUW.cif` & `pyxtal-0.5.6/pyxtal/database/cifs/GUMMUW.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/pyxtal/database/cifs/GeF2.cif` & `pyxtal-0.5.6/pyxtal/database/cifs/GeF2.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/pyxtal/database/cifs/HAHCOI.cif` & `pyxtal-0.5.6/pyxtal/database/cifs/HAHCOI.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/pyxtal/database/cifs/I4_132.cif` & `pyxtal-0.5.6/pyxtal/database/cifs/I4_132.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/pyxtal/database/cifs/JAPWIH.cif` & `pyxtal-0.5.6/pyxtal/database/cifs/JAPWIH.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/pyxtal/database/cifs/LAGNAL.cif` & `pyxtal-0.5.6/pyxtal/database/cifs/LAGNAL.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/pyxtal/database/cifs/LUFHAW.cif` & `pyxtal-0.5.6/pyxtal/database/cifs/LUFHAW.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/pyxtal/database/cifs/LiCs.cif` & `pyxtal-0.5.6/pyxtal/database/cifs/LiCs.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/pyxtal/database/cifs/MERQIM.cif` & `pyxtal-0.5.6/pyxtal/database/cifs/MERQIM.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/pyxtal/database/cifs/MPWO.cif` & `pyxtal-0.5.6/pyxtal/database/cifs/MPWO.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/pyxtal/database/cifs/NaCl.cif` & `pyxtal-0.5.6/pyxtal/database/cifs/NaCl.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/pyxtal/database/cifs/NaSb3F10.cif` & `pyxtal-0.5.6/pyxtal/database/cifs/NaSb3F10.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/pyxtal/database/cifs/NbO2.cif` & `pyxtal-0.5.6/pyxtal/database/cifs/NbO2.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/pyxtal/database/cifs/NiS-Cm.cif` & `pyxtal-0.5.6/pyxtal/database/cifs/NiS-Cm.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/pyxtal/database/cifs/P3_112.cif` & `pyxtal-0.5.6/pyxtal/database/cifs/P3_112.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/pyxtal/database/cifs/P4_332.cif` & `pyxtal-0.5.6/pyxtal/database/cifs/P4_332.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/pyxtal/database/cifs/P6_422.cif` & `pyxtal-0.5.6/pyxtal/database/cifs/P6_422.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/pyxtal/database/cifs/PAHYON01.cif` & `pyxtal-0.5.6/pyxtal/database/cifs/PAHYON01.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/pyxtal/database/cifs/PPO.cif` & `pyxtal-0.5.6/pyxtal/database/cifs/PPO.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/pyxtal/database/cifs/PVO.cif` & `pyxtal-0.5.6/pyxtal/database/cifs/PVO.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/pyxtal/database/cifs/Pm3.cif` & `pyxtal-0.5.6/pyxtal/database/cifs/Pm3.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/pyxtal/database/cifs/R-3.cif` & `pyxtal-0.5.6/pyxtal/database/cifs/R-3.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/pyxtal/database/cifs/R-3c.cif` & `pyxtal-0.5.6/pyxtal/database/cifs/R-3c.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/pyxtal/database/cifs/R32.cif` & `pyxtal-0.5.6/pyxtal/database/cifs/R32.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/pyxtal/database/cifs/TMPPIO03.cif` & `pyxtal-0.5.6/pyxtal/database/cifs/TMPPIO03.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/pyxtal/database/cifs/WEXBOS.cif` & `pyxtal-0.5.6/pyxtal/database/cifs/WEXBOS.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/pyxtal/database/cifs/YICMOP.cif` & `pyxtal-0.5.6/pyxtal/database/cifs/YICMOP.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/pyxtal/database/cifs/anthracene.cif` & `pyxtal-0.5.6/pyxtal/database/cifs/anthracene.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/pyxtal/database/cifs/aspirin-c.cif` & `pyxtal-0.5.6/pyxtal/database/cifs/aspirin-c.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/pyxtal/database/cifs/aspirin.cif` & `pyxtal-0.5.6/pyxtal/database/cifs/aspirin.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/pyxtal/database/cifs/benzene.cif` & `pyxtal-0.5.6/pyxtal/database/cifs/benzene.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/pyxtal/database/cifs/bug.vasp` & `pyxtal-0.5.6/pyxtal/database/cifs/bug.vasp`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/pyxtal/database/cifs/coumarin.cif` & `pyxtal-0.5.6/pyxtal/database/cifs/coumarin.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/pyxtal/database/cifs/dist_6_0.cif` & `pyxtal-0.5.6/pyxtal/database/cifs/dist_6_0.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/pyxtal/database/cifs/dist_6_1.cif` & `pyxtal-0.5.6/pyxtal/database/cifs/dist_6_1.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/pyxtal/database/cifs/gdh.cif` & `pyxtal-0.5.6/pyxtal/database/cifs/gdh.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/pyxtal/database/cifs/ht_KNbBO.cif` & `pyxtal-0.5.6/pyxtal/database/cifs/ht_KNbBO.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/pyxtal/database/cifs/ht_cristobalite.cif` & `pyxtal-0.5.6/pyxtal/database/cifs/ht_cristobalite.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/pyxtal/database/cifs/ht_quartz.cif` & `pyxtal-0.5.6/pyxtal/database/cifs/ht_quartz.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/pyxtal/database/cifs/ice.cif` & `pyxtal-0.5.6/pyxtal/database/cifs/ice.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/pyxtal/database/cifs/lt_KNbBO.cif` & `pyxtal-0.5.6/pyxtal/database/cifs/lt_KNbBO.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/pyxtal/database/cifs/lt_cristobalite.cif` & `pyxtal-0.5.6/pyxtal/database/cifs/lt_cristobalite.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/pyxtal/database/cifs/lt_quartz.cif` & `pyxtal-0.5.6/pyxtal/database/cifs/lt_quartz.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/pyxtal/database/cifs/naphthalene.cif` & `pyxtal-0.5.6/pyxtal/database/cifs/naphthalene.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/pyxtal/database/cifs/resorcinol.cif` & `pyxtal-0.5.6/pyxtal/database/cifs/resorcinol.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/pyxtal/database/cifs/xxvi.cif` & `pyxtal-0.5.6/pyxtal/database/cifs/xxvi.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/pyxtal/database/clusters.json` & `pyxtal-0.5.6/pyxtal/database/clusters.json`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/pyxtal/database/collection.py` & `pyxtal-0.5.6/pyxtal/database/collection.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/pyxtal/database/element.py` & `pyxtal-0.5.6/pyxtal/database/element.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/pyxtal/database/k_subgroup.json` & `pyxtal-0.5.6/pyxtal/database/k_subgroup.json`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/pyxtal/database/layer.csv` & `pyxtal-0.5.6/pyxtal/database/layer.csv`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/pyxtal/database/layer_generators.csv` & `pyxtal-0.5.6/pyxtal/database/layer_generators.csv`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/pyxtal/database/layer_symmetry.csv` & `pyxtal-0.5.6/pyxtal/database/layer_symmetry.csv`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/pyxtal/database/molecules.json` & `pyxtal-0.5.6/pyxtal/database/molecules.json`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/pyxtal/database/point.csv` & `pyxtal-0.5.6/pyxtal/database/point.csv`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/pyxtal/database/point_generators.csv` & `pyxtal-0.5.6/pyxtal/database/point_generators.csv`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/pyxtal/database/point_symmetry.csv` & `pyxtal-0.5.6/pyxtal/database/point_symmetry.csv`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/pyxtal/database/rod.csv` & `pyxtal-0.5.6/pyxtal/database/rod.csv`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/pyxtal/database/rod_generators.csv` & `pyxtal-0.5.6/pyxtal/database/rod_generators.csv`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/pyxtal/database/rod_symmetry.csv` & `pyxtal-0.5.6/pyxtal/database/rod_symmetry.csv`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/pyxtal/database/symbols.json` & `pyxtal-0.5.6/pyxtal/database/symbols.json`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/pyxtal/database/t_subgroup.json` & `pyxtal-0.5.6/pyxtal/database/t_subgroup.json`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/pyxtal/database/wyckoff_generators.csv` & `pyxtal-0.5.6/pyxtal/database/wyckoff_generators.csv`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/pyxtal/database/wyckoff_list.csv` & `pyxtal-0.5.6/pyxtal/database/wyckoff_list.csv`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/pyxtal/database/wyckoff_sets.json` & `pyxtal-0.5.6/pyxtal/database/wyckoff_sets.json`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/pyxtal/database/wyckoff_symmetry.csv` & `pyxtal-0.5.6/pyxtal/database/wyckoff_symmetry.csv`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/pyxtal/db.py` & `pyxtal-0.5.6/pyxtal/db.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/pyxtal/descriptor.py` & `pyxtal-0.5.6/pyxtal/descriptor.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,14 +2,59 @@
 Module for crystal packing descriptor from energy decomposition
 """
 import numpy as np
 import pyshtools as pysh
 from scipy.stats import qmc
 from scipy.spatial.transform import Rotation
 from scipy.optimize import minimize
+from scipy.special import sph_harm
+
+def _qlm(dists, l=4):
+    '''
+    Calculates the vector associated with an atomic site and 
+    one of its neighbors
+
+    Args:
+        distss: a list of distance vectors
+        l:  free integer quantum number
+    Returns:
+        q: numpy array(complex128), the complex vector qlm normalized
+            by the number of nearest neighbors
+    '''
+    # initiate variable as a complex number
+    q = np.zeros(2*l+1, dtype=np.complex128)
+    neighbors_count = len(dists)
+
+    for i, m in enumerate(range(-l, l+1)):
+        for j, r_vec in enumerate(dists):
+            # find the position vector of the site/neighbor pair
+            r_mag = np.linalg.norm(r_vec)
+            theta = np.arccos(r_vec[2] / r_mag)
+            if abs((r_vec[2] / r_mag) - 1.0) < 10.**(-8.):
+                theta = 0.0
+            elif abs((r_vec[2] / r_mag) + 1.0) < 10.**(-8.):
+                theta = np.pi
+
+            # phi
+            if r_vec[0] < 0.:
+                phi = np.pi + np.arctan(r_vec[1] / r_vec[0])
+            elif 0. < r_vec[0] and r_vec[1] < 0.:
+                phi = 2 * np.pi + np.arctan(r_vec[1] / r_vec[0])
+            elif 0. < r_vec[0] and 0. <= r_vec[1]:
+                phi = np.arctan(r_vec[1] / r_vec[0])
+            elif r_vec[0] == 0. and 0. < r_vec[1]:
+                phi = 0.5 * np.pi
+            elif r_vec[0] == 0. and r_vec[1] < 0.:
+                phi = 1.5 * np.pi
+            else:
+                phi = 0.
+
+            q[i] += sph_harm(m, l, phi, theta)
+    # normalize by number of neighbors
+    return q / neighbors_count
 
 def correlation(coef1, coef2, angle=None, s=0):
     """
     Compute the correlation between to sph coefs
 
     Args: 
         coef1: sph coefficients 1
@@ -95,14 +140,36 @@
         theta = phi * i  # golden angle increment
         x = np.cos(theta) * radius
         z = np.sin(theta) * radius
         points.append((x, y, z))
 
     return np.array(points)
 
+def cart2sph(x, y, z):
+    """
+    convert the x, y, z to spherical coordinates (phi, theta, r)
+    phi: [-pi, pi]
+    theta: [-pi/2, pi/2]
+    """
+    hxy = np.hypot(x, y)
+    r = np.hypot(hxy, z)
+    theta = np.arctan2(z, hxy)
+    phi = np.arctan2(y, x)
+    return phi, theta, r
+
+def sph2cart(phi, theta, r):
+    """
+    convert spherical coordinates (phi, theta, r) to Cartesian (x, y, z)
+    """
+    rcos_theta = r * np.cos(theta)
+    x = rcos_theta * np.cos(phi)
+    y = rcos_theta * np.sin(phi)
+    z = r * np.sin(theta)
+    return x, y, z
+
 def xyz2sph(xyzs, radian=True):
     """
     convert the vectors (x, y, z) to the sphere representation (theta, phi)
 
     Args:
         xyzs: 3D xyz coordinates
         radian: return in radian (otherwise degree)
@@ -160,16 +227,20 @@
         cilm: float, dimension (2, lmax+1, lmax+1)
             Coefficients of the spherican harmonic
 
         chi2: float
             The residual sum of squares misfit for an overdetermined inversion.
     """
     thetas, phis, vals = pts[:,0], pts[:,1], pts[:,2]
-    thetas = np.degrees(thetas) - 90
     phis = np.degrees(phis)
+    thetas = np.degrees(thetas)
+
+    # if thetas is within [0, 180]
+    if abs(thetas.min()) < 1e-3: thetas -= 90
+    #print('check thetas', thetas.min())
     cilm, chi2 = SHExpandLSQ(vals, thetas, phis, l_max, norm=norm, csphase=csphase)
 
     return cilm, chi2
 
 def get_alignment(pts, degrees=True):
     """
     Here we define the equator is the plane with three most important neighbors.
@@ -198,15 +269,14 @@
     angles = r.as_euler('zyz')
     if degrees: angles = np.degrees(angles)
     return angles
 
 
 class spherical_image():
 
-
     """
     A class to handle the crystal packing descriptor from spherical image
 
     Args:
         xtal: pyxtal structure
         model: 'molecule' or 'contact'
         max_d: maximum intermolecular distances
@@ -412,14 +482,72 @@
             coef1 = self.coefs[i]
             for j in range(len(sph2.coefs)):
                 coef2 = sph2.coefs[j]
                 d, _ = correlation_go(coef1, coef2, M=M, d_cut=cutoff)
                 S[i, j] = d
         return S
 
+class orientation_order():
+
+    """
+    Computes the Steinhardt orientation order parameters
+
+    Args:
+        xtal: pyxtal structure
+        max_d: maximum intermolecular distances
+        lmax: maximum bandwidth for spherical harmonic expansion
+    """
+    def __init__(self, xtal, max_CN=14):
+
+        self.xtal = xtal
+        self.max_CN = max_CN
+        self.dists = self.get_neighbors()
+
+    def get_neighbors(self):
+        '''
+        get neighboring molecules
+    
+        Returns:
+            pts: [N, 3] array, (theta, phi, eng)
+        '''
+        pts = []
+        for i, site in enumerate(self.xtal.mol_sites):
+            _, neighs, comps, _, engs = self.xtal.get_neighboring_molecules(i)
+            xyz, _ = site._get_coords_and_species(absolute=True, first=True) 
+            center = site.molecule.get_center(xyz)
+            coords = np.zeros([len(neighs), 3])
+            #print(len(neighs))
+            if len(neighs) > self.max_CN: neighs = neighs[:self.max_CN]
+            for _i, xyz in enumerate(neighs):
+                coords[_i, :] = self.xtal.molecules[comps[_i]].get_center(xyz) - center
+            pts.append(coords)
+        return pts
+ 
+    def get_parameters(self, ls=[4, 6]):
+        '''
+        Computes 
+        Args:
+            center: center xyz coordinate
+            neighbors: a list of neighboring xyz coordinates
+            weights: a list of weights for each neighbor
+        Returns:
+             q: numpy array(complex128), the complex vector qlm normalized
+                by the number of nearest neighbors
+        '''
+        qs = []
+        for dist in self.dists:
+            for l in ls:
+                factor = (4 * np.pi) / (2*l + 1)
+                qlms = _qlm(dist, l)
+                dot = float(np.sum(qlms*np.conjugate(qlms)))
+                qs.append(np.sqrt((4 * np.pi)/(2*l+1) * dot))
+
+        return qs
+ 
+
 if __name__ == '__main__':
     
     from pkg_resources import resource_filename
     from pyxtal import pyxtal
 
     cif_path = resource_filename("pyxtal", "database/cifs/")
     c1 = pyxtal(molecular=True)
```

### Comparing `pyxtal-0.5.5/pyxtal/elasticity.py` & `pyxtal-0.5.6/pyxtal/elasticity.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/pyxtal/interface/LJ.py` & `pyxtal-0.5.6/pyxtal/interface/LJ.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/pyxtal/interface/dftb.py` & `pyxtal-0.5.6/pyxtal/interface/dftb.py`

 * *Files 4% similar despite different names*

```diff
@@ -151,22 +151,25 @@
     #matsci
     #ob2
     #pbc
     #print(calc_type, kwargs)
     return kwargs
 
 
-def DFTB_relax(struc, skf_dir, opt_cell=False, step=500, fmax=0.1, kresol=0.10, folder='tmp', disp='D3', symmetrize=True, logfile=None):
+def DFTB_relax(struc, skf_dir, opt_cell=False, step=500, \
+               fmax=0.1, kresol=0.10, folder='tmp', disp='D3', \
+               mask=None, symmetrize=True, logfile=None):
     """
     DFTB optimizer based on ASE
 
     Args:
         struc: ase atoms object
         mode: [`single`, `relax`, `vc_relax`] (str)
         step: optimization steps (int)
+        mask: apply constraints on strain
     """
     if not os.path.exists(folder):
         os.makedirs(folder)
     cwd = os.getcwd()
     os.chdir(folder)
 
     kpts = Kgrid(struc, kresol)
@@ -174,29 +177,25 @@
     kwargs = make_Hamiltonian(skf_dir, atom_types, disp, kpts)
 
     calc = Dftb(label='test',
                 atoms=struc,
                 kpts=kpts,
                 **kwargs,
                 )
-
     struc.set_calculator(calc)
-    if symmetrize:
-        struc.set_constraint(FixSymmetry(struc)) 
+
+    # impose symmetry
+    if symmetrize: struc.set_constraint(FixSymmetry(struc)) 
+
+    # impose cell constraints
     if opt_cell:
-        ecf = ExpCellFilter(struc)
-        if logfile is not None:
-            dyn = FIRE(ecf, logfile=logfile)
-        else:
-            dyn = FIRE(ecf)
+        ecf = ExpCellFilter(struc, mask=mask)
+        dyn = FIRE(ecf, logfile=logfile)
     else:
-        if logfile is not None:
-            dyn = FIRE(struc, logfile=logfile)
-        else:
-            dyn = FIRE(struc)
+        dyn = FIRE(struc, logfile=logfile)
     try:
         dyn.run(fmax=fmax, steps=step)
         os.remove('dftb_pin.hsd')
         os.remove('geo_end.gen')
         os.remove('charges.bin')
     except:
         print("Problem in DFTB calculation")
@@ -273,15 +272,15 @@
         self.label = label
         self.kpts = Kgrid(struc, kresol)
         self.prefix = prefix
         self.use_omp = use_omp
         if not os.path.exists(self.folder):
            os.makedirs(self.folder)   
 
-    def get_calculator(self, mode, step=500, ftol=1e-3, FixAngles=False, eVperA=True):
+    def get_calculator(self, mode, step=500, ftol=1e-3, FixAngles=False, eVperA=True, md_params={}):
         """
         get the ase style calculator
 
         Args:
             mode: ['single', 'relax', 'vc_relax'] (str)
             step: relaxation steps (int)
             ftol: force tolerance (float)
@@ -289,15 +288,15 @@
             eVperA: unit in eV/A
 
         Returns:
             ase calculator
         """
         if eVperA: ftol *= 0.194469064593167E-01
         atom_types = set(self.struc.get_chemical_symbols())
-        kwargs = make_Hamiltonian(self.skf_dir, atom_types, self.disp, self.kpts, self.use_omp)
+        kwargs = make_Hamiltonian(self.skf_dir, atom_types, self.disp, self.kpts, use_omp=self.use_omp)
        
         if mode in ['relax', 'vc-relax']:
             #kwargs['Driver_'] = 'ConjugateGradient'
             kwargs['Driver_'] = 'GeometryOptimization'
             kwargs['Driver_Optimizer'] = 'FIRE {}'
             #kwargs['Driver_MaxForceComponent'] = ftol
             kwargs['Driver_MaxSteps'] = step
@@ -306,33 +305,65 @@
             kwargs['Driver_Convergence_GradElem'] = ftol
             
             if mode == 'vc-relax':
                 kwargs['Driver_MovedAtoms'] = "1:-1"
                 kwargs['Driver_LatticeOpt'] = "Yes"
                 if FixAngles:
                     kwargs['Driver_FixAngles'] = "Yes"
+
+        elif mode in ['nve', 'nvt', 'npt']:
+            # 1fs = 41.3 au
+            # 1000K = 0.0031668 au
+            dicts = {
+                     'temperature': 300,
+                     'pressure': 1e+5, #1atm
+                     'timestep': 1,
+                     'Thermostat': 'NoseHoover',
+                     'MDRestartFrequency': 1000,
+                     'band': 'No',
+                    }
+            dicts.update(md_params)
+
+            kwargs['Analysis_WriteBandOut'] = dicts['band']
+            kwargs['Driver_'] = 'VelocityVerlet'
+            kwargs['Driver_Steps'] = step
+            kwargs['Driver_TimeStep [fs]'] = dicts['timestep']
+            kwargs['Driver_MDRestartFrequency'] = dicts['MDRestartFrequency']
+            kwargs['Driver_MovedAtoms'] = "1:-1"
+            kwargs['Driver_OutputPrefix'] = self.prefix
+
+            if mode in ['nvt', 'npt']:
+                kwargs['Driver_Thermostat_'] = dicts['Thermostat']
+                kwargs['Driver_Thermostat_Temperature [Kelvin]'] = dicts['temperature']
+                kwargs['Driver_Thermostat_CouplingStrength [cm^-1]'] = 3200
+
+                if mode == 'npt':
+                    kwargs['Driver_Barostat_'] = ''
+                    kwargs['Driver_Barostat_Pressure [Pa]'] = dicts['pressure']
+                    kwargs['Driver_Barostat_Timescale [ps]'] = 0.1
+
     
         calc = Dftb(label=self.label,
                     #run_manyDftb_steps=True,
                     atoms=self.struc,
                     kpts=self.kpts,
                     **kwargs,
                     )
         return calc
 
-    def run(self, mode, step=500, ftol=1e-3, FixAngles=False):
+    def run(self, mode, step=500, ftol=1e-3, FixAngles=False, md_params={}):
         """
         execute the actual calculation
         """
         from time import time
         t0 = time()
         cwd = os.getcwd()
         os.chdir(self.folder)
 
-        calc = self.get_calculator(mode, step, ftol, FixAngles)
+        calc = self.get_calculator(mode, step, ftol, FixAngles, md_params=md_params)
         self.struc.set_calculator(calc)
         # self.struc.write('geo_o.gen', format='dftb')
         # execute the simulation
         calc.calculate(self.struc)
         if mode in ['relax', 'vc-relax']:
             final = read(self.prefix+'.gen')
         else:
@@ -655,16 +686,18 @@
             return None
 
         # Take into account that the last row may lack
         # columns if nkpt * nspin * nband % ncol != 0
         nrow = int(np.ceil(nkpt * nspin * nband * 1. / ncol))
         index_eig_end = index_eig_begin + nrow
         ncol_last = len(self.lines[index_eig_end - 1].split())
-        self.lines[index_eig_end - 1] += ' 0.0 ' * (ncol - ncol_last)
-
+        if ncol - ncol_last > 0:
+            self.lines[index_eig_end - 1] = self.lines[index_eig_end - 1].replace('\n', '')
+            self.lines[index_eig_end - 1] += ' 0.0 ' * (ncol - ncol_last)
+            self.lines[index_eig_end - 1] += '\n'
         eig = np.loadtxt(self.lines[index_eig_begin:index_eig_end]).flatten()
         eig *= Hartree
         N = nkpt * nband
         eigenvalues = [eig[i * N:(i + 1) * N].reshape((nkpt, nband))
                        for i in range(nspin)]
 
         return eigenvalues
@@ -707,18 +740,18 @@
     from ase.build import bulk
 
     skf_dir = os.environ['DFTB_PREFIX'] + 'pbc-0-3/'
     #skf_dir = os.environ['DFTB_PREFIX'] + '3ob-3-1/'
 
     struc = bulk('Si', 'diamond', cubic=True)
     struc.set_cell(1.1*struc.cell)
-    for mode in ['single', 'relax', 'vc-relax']:
+    for mode in ['single', 'relax', 'vc-relax', 'npt']:
         my = DFTB(struc, skf_dir)
         struc, energy = my.run(mode)
         res = "{:8s} ".format(mode)
         res += "{:8.4f} ".format(struc.cell[0,0])
         res += "{:8.4f} ".format(struc.cell[1,1])
         res += "{:8.4f} ".format(struc.cell[2,2])
         res += "{:12.4f}".format(energy)
         print(res)
-    gap = DFTB_SCF(struc, skf_dir)
-    print(gap)
+    #gap = DFTB_SCF(struc, skf_dir)
+    #print(gap)
```

### Comparing `pyxtal-0.5.5/pyxtal/interface/gulp.py` & `pyxtal-0.5.6/pyxtal/interface/gulp.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,20 +19,22 @@
     """
 
     def __init__(self, struc, label="_", path='tmp', ff='reax', \
                  pstress=None, opt='conp', steps=1000, exe='gulp',\
                  input='gulp.in', output='gulp.log', dump=None):
 
         if isinstance(struc, pyxtal):
-            struc = struc.to_ase()
+            self.species = struc.species
+            struc = struc.to_ase(resort=False)
 
         if isinstance(struc, Atoms):
             self.lattice = Lattice.from_matrix(struc.cell)
             self.frac_coords = struc.get_scaled_positions()
             self.sites = struc.get_chemical_symbols()
+            self.species = None
         else:
             raise NotImplementedError("only support ASE atoms object")
 
         self.structure = struc
         self.pstress= pstress
         self.label = label
         self.ff = ff
@@ -76,20 +78,24 @@
         return Atoms(self.sites, scaled_positions=self.frac_coords, cell=self.lattice.matrix)
 
     def to_pymatgen(self):
         from pymatgen.core.structure import Structure
         return Structure(self.lattice.matrix, self.sites, self.frac_coords)
 
     def to_pyxtal(self):
-        #print(self.sites)
-        #print(self.frac_coords)
-        #print(self.lattice.matrix)
         ase_atoms = self.to_ase()
-        struc = pyxtal()
-        struc.from_seed(ase_atoms)
+        for tol in [1e-2, 1e-3, 1e-4, 1e-5]:
+            try:
+                struc = pyxtal()
+                struc.from_seed(ase_atoms, tol=tol)
+                break
+            except:
+                pass
+                #print('Something is wrong', tol)
+                #struc.from_seed('bug.vasp', tol*10)
         return struc
 
     def write(self):
         a, b, c, alpha, beta, gamma = self.lattice.get_para(degree=True)
         
         with open(self.input, 'w') as f:
             if self.opt == 'conv':
@@ -103,15 +109,18 @@
             f.write('{:12.6f}{:12.6f}{:12.6f}{:12.6f}{:12.6f}{:12.6f}\n'.format(\
                     a, b, c, alpha, beta, gamma))
             f.write('\nfractional\n')
             
             symbols = []
             for coord, site in zip(self.frac_coords, self.sites):
                 f.write('{:4s} {:12.6f} {:12.6f} {:12.6f} core \n'.format(site, *coord))
-            species = list(set(self.sites))
+            if self.species is not None:
+                species = self.structure.species
+            else:
+                species = list(set(self.sites))
 
             f.write('\nSpecies\n')
             for specie in species:
                 f.write('{:4s} core {:4s}\n'.format(specie, specie))
 
             f.write('\nlibrary {:s}\n'.format(self.ff))
             f.write('ewald 10.0\n')
@@ -219,26 +228,26 @@
                 self.energy = None
                 print("GULP calculation is wrong, reading------")
         except:
             self.error = True
             self.energy = None
             print("GULP calculation is wrong")
 
-def single_optimize(struc, ff, pstress=None, opt="conp", exe="gulp", path="tmp", label="_", clean=True):
-    calc = GULP(struc, label=label, path=path, pstress=pstress, ff=ff, opt=opt)
+def single_optimize(struc, ff, steps=1000, pstress=None, opt="conp", exe="gulp", path="tmp", label="_", clean=True):
+    calc = GULP(struc, steps=steps, label=label, path=path, pstress=pstress, ff=ff, opt=opt)
     calc.run(clean=clean)
     if calc.error:
         print("GULP error in single optimize")
         return None, None, 0, True
     else:
         struc = calc.to_pyxtal()
         #if sum(struc.numIons) == 42:
         #    print("SSSSSSSSSSSSSS")
         #    import sys; sys.exit()   
-        return calc.to_pyxtal(), calc.energy_per_atom, calc.cputime, calc.error
+        return struc, calc.energy_per_atom, calc.cputime, calc.error
 
 def optimize(struc, ff, optimizations=["conp", "conp"], exe="gulp", 
             pstress=None, path="tmp", label="_", clean=True, adjust=False):
     time_total = 0
     for opt in optimizations:
         struc, energy, time, error = single_optimize(struc, ff, pstress, opt, exe, path, label, clean)
         time_total += time
```

### Comparing `pyxtal-0.5.5/pyxtal/interface/lammpslib.py` & `pyxtal-0.5.6/pyxtal/interface/lammpslib.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/pyxtal/interface/vasp.py` & `pyxtal-0.5.6/pyxtal/interface/vasp.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/pyxtal/interface/vasprun.py` & `pyxtal-0.5.6/pyxtal/interface/vasprun.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/pyxtal/io.py` & `pyxtal-0.5.6/pyxtal/io.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/pyxtal/lattice.py` & `pyxtal-0.5.6/pyxtal/lattice.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,14 +139,31 @@
         elif self.ltype in ['orthorhombic']:
             self.dof = 3
         elif self.ltype in ['tetragonal', 'hexagonal', 'trigonal']:
             self.dof = 2
         else:
             self.dof = 1
 
+    @classmethod
+    def get_dofs(self, ltype):
+        """
+        get the number of degree of freedom
+        """
+        if ltype in ["triclinic"]:
+            dofs = [3, 3] 
+        elif ltype in ["monoclinic"]:
+            dofs = [3, 1]
+        elif ltype in ['orthorhombic']:
+            dofs = [3, 0]
+        elif ltype in ['tetragonal', 'hexagonal', 'trigonal']:
+            dofs = [2, 0]
+        else:
+            dofs = [1, 0]
+        return dofs
+
     def copy(self):
         """
         simply copy the structure
         """
         from copy import deepcopy
         return deepcopy(self)
 
@@ -439,14 +456,35 @@
         elif self.ltype in ['orthorhombic']:
             return [a, b, c]
         elif self.ltype in ['monoclinic']:
             return [a, b, c, beta]
         else:
             return [a, b, c, alpha, beta, gamma]
 
+    @classmethod
+    def from_1d_representation(self, v, ltype):
+        if ltype == 'triclinic':
+            a, b, c, alpha, beta, gamma = v[0], v[1], v[2], v[3], v[4], v[5]
+        elif ltype == 'monoclinic':
+            a, b, c, alpha, beta, gamma = v[0], v[1], v[2], 90, v[3], 90
+        elif ltype == 'orthorhombic':
+            a, b, c, alpha, beta, gamma = v[0], v[1], v[2], 90, 90, 90
+        elif ltype == 'tetragonal':
+            a, b, c, alpha, beta, gamma = v[0], v[0], v[1], 90, 90, 90
+        elif ltype == 'hexagonal':
+            a, b, c, alpha, beta, gamma = v[0], v[0], v[1], 90, 90, 120
+        else:
+            a, b, c, alpha, beta, gamma = v[0], v[0], v[0], 90, 90, 90
+        try:
+            l = Lattice.from_para(a, b, c, alpha, beta, gamma, ltype=ltype)
+            return l
+        except:
+            print(a, b, c, alpha, beta, gamma, ltype)
+
+
     def mutate(self, degree=0.20, frozen=False):
         """
         mutate the lattice object
         """
         rand = 1 + degree*(np.random.sample(6)-0.5)
         a0, b0, c0, alpha0, beta0, gamma0 = self.get_para()
         a = a0*rand[0]
```

### Comparing `pyxtal-0.5.5/pyxtal/molecular_crystal.py` & `pyxtal-0.5.6/pyxtal/molecular_crystal.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/pyxtal/molecule.py` & `pyxtal-0.5.6/pyxtal/molecule.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/pyxtal/msg.py` & `pyxtal-0.5.6/pyxtal/msg.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/pyxtal/operations.py` & `pyxtal-0.5.6/pyxtal/operations.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/pyxtal/optimize/fire.py` & `pyxtal-0.5.6/pyxtal/optimize/fire.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/pyxtal/optimize/fire2.py` & `pyxtal-0.5.6/pyxtal/optimize/fire2.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/pyxtal/optimize/myscipy_optimize.py` & `pyxtal-0.5.6/pyxtal/optimize/myscipy_optimize.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/pyxtal/potentials/CuAg.eam.alloy` & `pyxtal-0.5.6/pyxtal/potentials/CuAg.eam.alloy`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/pyxtal/potentials/LJ_cluster.py` & `pyxtal-0.5.6/pyxtal/potentials/LJ_cluster.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/pyxtal/potentials/Si.tersoff` & `pyxtal-0.5.6/pyxtal/potentials/Si.tersoff`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/pyxtal/potentials/SiCGe.tersoff` & `pyxtal-0.5.6/pyxtal/potentials/SiCGe.tersoff`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/pyxtal/representation.py` & `pyxtal-0.5.6/pyxtal/representation.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,164 @@
 import os
 import numpy as np
 from pyxtal.symmetry import Group
 from pyxtal.lattice import Lattice
-from pyxtal.wyckoff_site import mol_site
+from pyxtal.wyckoff_site import mol_site, atom_site
 from pyxtal.molecule import find_rotor_from_smile
  
+class representation_atom():
+    """
+    A class to handle the 1D representation of atomic crystal   
+    Works for Zprime > 1
+
+    Args:
+        x: a list of [cell, site_1, site_2, ...]
+    """
+
+    def __init__(self, x):
+        self.x = x
+
+    def __str__(self):
+        return self.to_string()
+
+    @classmethod
+    def from_pyxtal(cls, struc, standard=False):
+        """
+        Initialize 1D rep. from the pyxtal object
+
+        Args:
+            struc: pyxtal object
+        """
+        if standard and not struc.standard_setting:
+            pmg = struc.to_pymatgen()
+            struc.from_seed(pmg, standard=True)
+        symmetry = [struc.atom_sites[0].wp.hall_number]
+        lat = struc.lattice.encode()
+        vector = [symmetry + lat]
+        smiles = []
+        for site in struc.atom_sites:
+            vector.append(site.encode())
+        x = vector
+        return cls(x)
+    
+    def to_standard_setting(self):
+        xtal = self.to_pyxtal()
+        self.x = representation.from_pyxtal(xtal, standard=True).x
+ 
+    def to_pyxtal(self):
+        """
+        Export the pyxtal structure
+
+        Args:
+            smiles: list of smiles
+            compoisition: list of composition
+        """
+        from pyxtal import pyxtal
+
+        # symmetry
+        v = self.x[0]
+        struc = pyxtal()
+        struc.group, number = Group(v[0], use_hall=True), v[0]
+    
+        # lattice
+        ltype = struc.group.lattice_type
+        if ltype == 'triclinic':
+            a, b, c, alpha, beta, gamma = v[1], v[2], v[3], v[4], v[5], v[6]
+        elif ltype == 'monoclinic':
+            a, b, c, alpha, beta, gamma = v[1], v[2], v[3], 90, v[4], 90
+        elif ltype == 'orthorhombic':
+            a, b, c, alpha, beta, gamma = v[1], v[2], v[3], 90, 90, 90
+        elif ltype == 'tetragonal':
+            a, b, c, alpha, beta, gamma = v[1], v[1], v[2], 90, 90, 90
+        elif ltype == 'hexagonal':
+            a, b, c, alpha, beta, gamma = v[1], v[1], v[2], 90, 90, 120
+        else:
+            a, b, c, alpha, beta, gamma = v[1], v[1], v[1], 90, 90, 90
+        try:
+            struc.lattice = Lattice.from_para(a, b, c, alpha, beta, gamma, ltype=ltype)
+        except:
+            print(a, b, c, alpha, beta, gamma, ltype)
+            raise ValueError("Problem in Lattice")
+    
+        # sites
+        struc.numIons = [0] * len(smiles) 
+        struc.atom_sites = [] 
+
+        count = 1
+        for i, comp in enumerate(composition): 
+            for j in range(comp):
+                v = self.x[count]
+                dicts = {}
+                dicts['type'] = i
+                dicts['dim'] = 3
+                dicts['PBC'] = [1, 1, 1]
+                dicts['hn'] = struc.group.hall_number
+                dicts['index'] = 0
+                dicts['lattice'] = struc.lattice.matrix
+                dicts['lattice_type'] = ltype
+                site = atom_site.from_1D_dicts(dicts)
+                site.type = i
+                struc.atom_sites.append(site)
+                struc.numIons[i] += site.wp.multiplicity
+                #move to next rep
+                count += 1
+            struc.species.append(site.specie)
+
+        struc._get_formula()
+        struc.source = '1D rep.'
+        struc.valid = True
+        struc.standard_setting = site.wp.is_standard_setting()
+
+        return struc
+    
+    def to_string(self, time=None, eng=None, tag=None):
+        """
+        Export string representation
+
+        Args:
+            time: float
+            eng: float
+            tag: string
+        """
+        x = self.x
+        strs = "{:3d} ".format(int(x[0][0]))
+
+        # data for cell
+        if x[0][0] <= 348:
+            num = 4
+        elif x[0][0] <= 488:
+            num = 3
+        else: #cubic
+            num = 2
+
+        for c in x[0][1:num]:
+            strs += "{:5.2f} ".format(c)
+        for c in x[0][num:]:
+            strs += "{:5.1f} ".format(c)
+        
+        # data for atoms
+        strs += "{:d} ".format(len(x)-1)  # Number of sites
+        for i in range(1, len(x)):
+            strs += "{:s} ".format(x[i][0])
+            strs += "{:d} ".format(x[i][1])
+            for v in x[i][2:]:
+                strs += "{:4.2f} ".format(v)      
+
+        if time is not None:
+            strs += "{:5.2f}".format(time)
+
+        if eng is not None:
+            strs += "{:11.3f}".format(eng)
+    
+        if tag is not None:
+            strs += " {:s}".format(tag)
+    
+        return strs
+
+
 class representation():
     """
     A class to handle the 1D representation of molecular crystal   
     Works for Zprime > 1
 
     Args:
         x: a list of [cell, site_1, site_2, ...]
```

### Comparing `pyxtal-0.5.5/pyxtal/supergroup.py` & `pyxtal-0.5.6/pyxtal/supergroup.py`

 * *Files 2% similar despite different names*

```diff
@@ -604,17 +604,17 @@
         return coords_G1, coords_G2, coords_H, elements, ordered_mapping
 
     def print_wp(self, sp, id):
         """
         A short cut to print the wp information (for debug purpose)
         """
         wp1 = sp.wp1_lists[id]
-        l = str(wp1.multiplicity) + wp1.letter + '->'
+        l = wp1.get_label() + '->'
         for wp in sp.wp2_lists[id]:
-            l += str(wp.multiplicity) + wp.letter + ','
+            l += wp.get_label() + ','
         strs = '{:2s}{:s} ID-{:d} {:s}'.format(sp.elements[id], sp.group_type, id, l)
         return strs
 
     def symmetrize_site_single(self, splitter, id, base, translation, run_type=1):
         """
         Symmetrize one WP to another with higher symmetry
 
@@ -880,16 +880,15 @@
         count = 0
         disps = []
         for i, wp2 in enumerate(sp.wp2_lists):
             wp1 = sp.wp1_lists[i]
             strs = ''
             for wp in wp2:
                 x, y, ele = coords_H[count], coords_G[count], elements[count]
-                label = str(wp.multiplicity) + wp.letter + '->'
-                label += str(wp1.multiplicity) + wp1.letter
+                label = wp.get_label() + '->' + wp1.get_label()
                 dis = y - x - translation
                 dis -= np.round(dis)
                 dis_abs = np.linalg.norm(dis.dot(self.cell))
                 output = "{:2s}[{:8s}] {:8.4f}{:8.4f}{:8.4f}".format(ele, label, *x)
                 output += " -> {:8.4f}{:8.4f}{:8.4f}".format(*y)
                 output += " -> {:8.4f}{:8.4f}{:8.4f} {:8.4f}".format(*dis, dis_abs)
                 count += 1
@@ -1130,17 +1129,17 @@
             print("\nTransition: ", sp.H.number, '->', sp.G.number)
             output = "Cell: {:7.3f}{:7.3f}{:7.3f}".format(*trans)
             output += ", Disp (A): {:6.3f}".format(max_disp)
             print(output)
             for i, wp2 in enumerate(sp.wp2_lists):
                 wp1 = sp.wp1_lists[i]
                 ele = sp.elements[i]
-                l2 = str(wp1.multiplicity) + wp1.letter
+                l2 = wp1.get_label()
                 for j, wp in enumerate(wp2):
-                    l1 = str(wp.multiplicity) + wp.letter
+                    l1 = wp.get_label()
                     output = "{:2s} [{:2d}]: ".format(ele, mapping[i][j])
                     output += "{:3s} -> {:3s}".format(l1, l2)
                     print(output)
 
     def get_transformation(self, N_images=2):
         """
         Get the series of transformed structures between H and G
```

### Comparing `pyxtal-0.5.5/pyxtal/symmetry.py` & `pyxtal-0.5.6/pyxtal/symmetry.py`

 * *Files 1% similar despite different names*

```diff
@@ -221,14 +221,15 @@
         use_hall (default: False): whether or not use the hall number
         style (default: `pyxtal`): the choice of hall number ('pyxtal'/'spglib')
         quick (defaut: False): whether or not ignore the wyckoff information
     """
 
     def __init__(self, group, dim=3, use_hall=False, style='pyxtal', quick=False):
 
+        self.string = None
         self.dim = dim
         names = ['Point', 'Rod', 'Layer', 'Space']
         self.header = "-- " + names[dim] + 'group --'
         if not use_hall:
             self.symbol, self.number = get_symbol_and_number(group, dim)
         else:
             self.symbol = hall_table['Symbol'][group-1]
@@ -289,25 +290,24 @@
                 self.Wyckoff_positions.append(wp)
 
             # A 2D list of WP objects, grouped and sorted by multiplicity
             self.wyckoffs_organized = organized_wyckoffs(self)
 
 
     def __str__(self):
-        try:
+        if self.string is not None:
             return self.string
-        except:
+        else:
             s = self.header
             s += "# " + str(self.number) + " (" + self.symbol + ")--"
 
             for wp in self.Wyckoff_positions:
-                ops = ss_string_from_ops(wp.symmetry[0], self.number, dim=self.dim)
-                s += "\n" + str(wp.multiplicity)
-                s += wp.letter
-                s += "\tsite symm: " + ops
+                s += "\n" + wp.get_label()
+                if not hasattr(wp, "site_symm"): wp.get_site_symmetry()
+                s += "\tsite symm: " + wp.site_symm
             self.string = s
 
             return self.string
 
     def __repr__(self):
         return str(self)
 
@@ -499,36 +499,14 @@
             for c in index:
                 if c.isalpha():
                     letter = c
                     break
             index = index_from_letter(letter, self.wyckoffs, dim=self.dim)
         return self.Wyckoff_positions[index]
 
-    def get_wyckoff_symmetry(self, index, molecular=False):
-        """
-        Returns the site symmetry symbol for the Wyckoff position
-
-        Args:
-            index: the index of the Wyckoff position within the group
-            molecular: use the Euclidean operations or not (for hexagonal group)
-
-        Returns: a Hermann-Mauguin style string for the site symmetry
-        """
-        if type(index) == str:
-            # Extract letter from number-letter combinations ("4d"->"d")
-            for c in index:
-                if c.isalpha():
-                    letter = c
-                    break
-            index = index_from_letter(letter, self.wyckoffs, dim=self.dim)
-        if molecular:
-            ops = self.w_symm_m[index][0]
-        else:
-            ops = self.w_symm[index][0]
-        return ss_string_from_ops(ops, self.number, dim=self.dim)
 
     def get_alternatives(self):
         """
         Get the alternative settings as a dictionary
         """
         if self.dim == 3:
             return wyc_sets[str(self.number)]
@@ -565,15 +543,16 @@
             dicts = self.get_max_t_subgroup()
         return dicts, g_type
 
     def get_wp_list(self, reverse=False):
         """
         Get the reversed list of wps
         """
-        wp_list = [(str(x.multiplicity)+x.letter) for x in self.Wyckoff_positions]
+        #wp_list = [(str(x.multiplicity)+x.letter) for x in self.Wyckoff_positions]
+        wp_list = [(x.get_label()) for x in self.Wyckoff_positions]
         if reverse: wp_list.reverse()
         return wp_list
 
     def get_splitters_from_structure(self, struc, group_type='t'):
         """
         Get the valid symmetry relations for a structure to its supergroup
         e.g.,
@@ -1036,15 +1015,16 @@
             group: Group object
             index: the index of starting wp
             max_steps: the number of steps to search
 
         Return:
             a list of (g_types, subgroup_id, spg_number, wp_list (optional))
         """
-        label = [str(self[index].multiplicity) + self[index].letter]
+        #label = [str(self[index].multiplicity) + self[index].letter]
+        label = [self[index].get_label()]
         potential=[[(None, None, self.number, label)]]
         solutions=[]
 
         for step in range(max_steps):
             _potential = []
             for p in potential:
                 tail = p[-1]
@@ -1294,15 +1274,16 @@
                 P = abc2matrix(hall_table['P'][hall_number-1])
                 P1 = abc2matrix(hall_table['P^-1'][hall_number-1])
         elif dim == 2:
             PBC = [1, 1, 0]
         elif dim == 1:
             PBC = [0, 0, 1]
 
-        if wyckoffs is None: wyckoffs = get_wyckoffs(number, dim=dim)
+        if wyckoffs is None: 
+            wyckoffs = get_wyckoffs(number, dim=dim)
 
         wpdict = {
                   "index": index,
                   "letter": letter_from_index(index, wyckoffs, dim=dim),
                   "ops": wyckoffs[index],
                   "multiplicity": len(wyckoffs[index]),
                   "symmetry":  get_wyckoff_symmetry(number, dim=dim)[index],
@@ -1397,15 +1378,15 @@
 
 
     #=============================Fundamentals===========================
     def __str__(self, supress=False):
         if self.dim not in [0, 1, 2, 3]:
             return "invalid crystal dimension. Must be between 0 and 3."
         if not hasattr(self, "site_symm"): self.get_site_symmetry()
-        s = "Wyckoff position " + str(self.multiplicity) + self.letter + " in "
+        s = "Wyckoff position " + self.get_label() + " in "
         if self.dim == 3:
             s += "space "
         elif self.dim == 2:
             s += "layer "
         elif self.dim == 1:
             s += "Rod "
         elif self.dim == 0:
@@ -1678,25 +1659,36 @@
 
     def get_dof(self):
         """
         Simply return the degree of freedom
         """
         return np.linalg.matrix_rank(self.ops[0].rotation_matrix)
 
+    def get_label(self):
+        """
+        get the string like 4a
+        """
+        return str(self.multiplicity) + self.letter
+
     def get_frozen_axis(self):
         if self.index == 0:
             return []
         elif self.get_dof() == 0:
             return [0, 1, 2]
         else:
             if self.number >=75:
-                if self.ops[0].rotation_matrix[2,2] == 1:
-                    return [0, 1]
-                else:
-                    return [0, 1, 2]
+                #if self.ops[0].rotation_matrix[2,2] == 1:
+                #    return [0, 1]
+                #else:
+                #    return [0, 1, 2]
+                axs = []
+                for ax in range(3):
+                    if self.ops[0].rotation_matrix[ax, ax] == 0:
+                        axs.append(ax)
+                return axs
             else:
                 if self.get_dof() == 1:
                     if self.ops[0].rotation_matrix[2,2] == 1:
                         return [0, 1]
                     elif self.ops[0].rotation_matrix[1,1] == 1:
                         return [0, 2]
                     elif self.ops[0].rotation_matrix[0,0] == 1:
@@ -1739,14 +1731,38 @@
         op = self.generators[idx]
         if self.euclidean:
             hat = SymmOp.from_rotation_and_translation(cell.T, [0, 0, 0])
             op = hat * op * hat.inverse
 
         return op
 
+    def get_free_xyzs(self, pos):
+        """
+        return the free xyz paramters from the given xyz position
+        """
+        #print(self.apply_ops(pos)[0])
+        res = self.apply_ops(pos)[0]
+        res = np.delete(res, self.get_frozen_axis())
+        return res
+
+    def get_position_from_free_xyzs(self, xyz):
+        """
+        generate the full xyz position from the free xyzs
+        """
+        pos = np.zeros(3)
+        frozen = self.get_frozen_axis()
+        count = 0
+        for axis in range(3):
+            if axis not in frozen:
+                pos[axis] = xyz[count]
+                count += 1
+        pos = self.apply_ops(pos)[0]
+        pos -= np.floor(pos)
+        return pos
+
     def get_all_positions(self, pos):
         """
         return the list of position from any single coordinate from wp.
         The position does not have to be the 1st number in the wp list
 
         >>> from pyxtal.symmetry import Group
         >>> wp2 = Group(62)[-1]
@@ -1868,15 +1884,15 @@
         for op in ops:
             print(op.as_xyz_string())
 
     def gen_pos(self):
         """
         Returns the general Wyckoff position
         """
-        return self.Wyckoff_positions[0]
+        return self.ops[0]
 
     def are_equivalent_pts(self, pt1, pt2, cell=np.eye(3), tol=0.05):
         """
         Check if two pts are equivalent
         """
         pt1 = self.search_generator(pt1, tol=tol)
         pt2 = self.search_generator(pt2, tol=tol)
@@ -2528,15 +2544,15 @@
     # TODO: replace sg with number, add dim variable
     # Return the symbol for a single axis
     # Will be called later in the function
     def get_symbol(opas, order, has_reflection):
         # ops: a list of Symmetry operations about the axis
         # order: highest order of any symmetry operation about the axis
         # has_reflection: whether or not the axis has mirror symmetry
-        if has_reflection is True:
+        if has_reflection:
             # rotations have priority
             for opa in opas:
                 if opa.order == order and opa.type == "rotation":
                     return str(opa.rotation_order) + "/m"
             for opa in opas:
                 if (
                     opa.order == order
@@ -2593,18 +2609,21 @@
                 max_j = j
                 max_index = i
         if use_list is True:
             return symbol_list[max_index]
         else:
             return symbols[max_j]
 
-    # Return whether or not two axes are symmetrically equivalent
-    # It is assumed that both axes possess the same symbol
-    # Will be called within combine_axes
     def are_symmetrically_equivalent(index1, index2):
+        """
+        Return whether or not two axes are symmetrically equivalent
+        It is assumed that both axes possess the same symbol
+        Will be called within combine_axes
+        """
+
         axis1 = axes[index1]
         axis2 = axes[index2]
         condition1 = False
         condition2 = False
         # Check for an operation mapping one axis onto the other
         for op in ops:
             if condition1 is False or condition2 is False:
@@ -2615,58 +2634,67 @@
                 if np.isclose(abs(np.dot(new2, axis1)), 1):
                     condition2 = True
         if condition1 is True and condition2 is True:
             return True
         else:
             return False
 
-    # Given a list of axis indices, return the combined symbol
-    # Axes may or may not be symmetrically equivalent, but must be of the same
-    # type (x/y/z, face-diagonal, body-diagonal)
-    # Will be called for mid- and high-symmetry crystallographic point groups
     def combine_axes(indices):
+        """
+        Given a list of axis indices, return the combined symbol
+        Axes may or may not be symmetrically equivalent, but must be of the same
+        type (x/y/z, face-diagonal, body-diagonal)
+        Will be called for mid- and high-symmetry crystallographic point groups
+        """
+
         symbols = {}
         for index in deepcopy(indices):
             symbol = get_symbol(params[index], orders[index], reflections[index])
             if symbol == ".":
                 indices.remove(index)
             else:
                 symbols[index] = symbol
-        if indices == []:
+
+        if len(indices) == 0:
             return "."
+
         # Remove redundant axes
         for i in deepcopy(indices):
             for j in deepcopy(indices):
                 if j > i:
                     if symbols[i] == symbols[j]:
                         if are_symmetrically_equivalent(i, j):
                             if j in indices:
                                 indices.remove(j)
+
         # Combine symbols for non-equivalent axes
         new_symbols = []
         for i in indices:
             new_symbols.append(symbols[i])
+
         symbol = ""
         while new_symbols != []:
             highest = get_highest_symbol(new_symbols)
             symbol += highest
             new_symbols.remove(highest)
         if symbol == "":
             printx("Error: could not combine site symmetry axes.", priority=1)
             return
         else:
             return symbol
 
     # Generate needed ops
     if not complete:
         ops = generate_full_symmops(ops, 1e-3)
+
     # Get OperationAnalyzer object for all ops
     opas = []
     for op in ops:
         opas.append(OperationAnalyzer(op))
+
     # Store the symmetry of each axis
     params = [[], [], [], [], [], [], [], [], [], [], [], [], []]
     has_inversion = False
     # Store possible symmetry axes for crystallographic point groups
     axes = [
         [1, 0, 0],
         [0, 1, 0],
@@ -2678,38 +2706,45 @@
         [0, 1, -1],
         [1, 0, -1],
         [1, 1, 1],
         [-1, 1, 1],
         [1, -1, 1],
         [1, 1, -1],
     ]
+
     for i, axis in enumerate(axes):
         axes[i] = axis / np.linalg.norm(axis)
+
     for opa in opas:
+
+        # Search for the primary rotation axis
         if opa.type != "identity" and opa.type != "inversion":
             found = False
             for i, axis in enumerate(axes):
                 if np.isclose(abs(np.dot(opa.axis, axis)), 1):
                     found = True
                     params[i].append(opa)
+
             # Store uncommon axes for trigonal and hexagonal lattices
-            if found is False:
+            if not found: #is False:
                 axes.append(opa.axis)
                 # Check that new axis is not symmetrically equivalent to others
                 unique = True
                 for i, axis in enumerate(axes):
                     if i != len(axes) - 1:
                         if are_symmetrically_equivalent(i, len(axes) - 1):
                             unique = False
-                if unique is True:
+                if unique: # is True:
                     params.append([opa])
-                elif unique is False:
+                else: #if unique is False:
                     axes.pop()
+
         elif opa.type == "inversion":
             has_inversion = True
+
     # Determine how many high-symmetry axes are present
     n_axes = 0
     # Store the order of each axis
     orders = []
     # Store whether or not each axis has reflection symmetry
     reflections = []
     for axis in params:
@@ -2720,29 +2755,30 @@
             if opa.order >= 3:
                 high_symm = True
             if opa.order > order:
                 order = opa.order
             if opa.order == 2 and opa.type == "rotoinversion":
                 has_reflection = True
         orders.append(order)
-        if high_symm == True:
+
+        if high_symm: #== True:
             n_axes += 1
         reflections.append(has_reflection)
     # Triclinic, monoclinic, orthorhombic
     # Positions in symbol refer to x,y,z axes respectively
     if symm_type == "low":
         symbol = (
             get_symbol(params[0], orders[0], reflections[0])
             + get_symbol(params[1], orders[1], reflections[1])
             + get_symbol(params[2], orders[2], reflections[2])
         )
         if symbol != "...":
             return symbol
         elif symbol == "...":
-            if has_inversion is True:
+            if has_inversion: #is True:
                 return "-1"
             else:
                 return "1"
     # Trigonal, Hexagonal, Tetragonal
     elif symm_type == "medium":
         # 1st symbol: z axis
         s1 = get_symbol(params[2], orders[2], reflections[2])
@@ -2750,15 +2786,15 @@
         s2 = combine_axes([0, 1])
         # 3rd symbol: face-diagonal axes (whichever have highest symmetry)
         s3 = combine_axes(list(range(3, len(axes))))
         symbol = s1 + " " + s2 + " " + s3
         if symbol != ". . .":
             return symbol
         elif symbol == ". . .":
-            if has_inversion is True:
+            if has_inversion: #is True:
                 return "-1"
             else:
                 return "1"
     # Cubic
     elif symm_type == "high":
         pass
         # 1st symbol: x, y, and/or z axes (whichever have highest symmetry)
@@ -2767,15 +2803,15 @@
         s2 = combine_axes([9, 10, 11, 12])
         # 3rd symbol: face-diagonal axes (whichever have highest symmetry)
         s3 = combine_axes([3, 4, 5, 6, 7, 8])
         symbol = s1 + " " + s2 + " " + s3
         if symbol != ". . .":
             return symbol
         elif symbol == ". . .":
-            if has_inversion is True:
+            if has_inversion: #is True:
                 return "-1"
             else:
                 return "1"
     else:
         printx("Error: invalid spacegroup number", priority=1)
         return
```

### Comparing `pyxtal-0.5.5/pyxtal/test_all.py` & `pyxtal-0.5.6/pyxtal/test_all.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,14 +30,19 @@
     def test_list_wyckoff_combinations(self):
         g = Group(64)
         a1, _ = g.list_wyckoff_combinations([4, 2])
         self.assertTrue(a1 is None)
         a2, _ = g.list_wyckoff_combinations([4, 8], quick=False) 
         self.assertTrue(len(a2) == 8)
 
+    def test_print_group(self):
+        for sg in [1, 15, 60, 143, 188]:
+            g = Group(sg)
+            #print(g)
+
     def test_short_path(self):
         g = Group(217)
         path = g.short_path_to_general_wp(7)
         self.assertTrue(path[-1][2] == 145)
 
     def test_spg_symmetry(self):
         N_polar, N_centro, N_chiral = 0, 0, 0
@@ -428,39 +433,46 @@
                 (160, 1, '. . m'),
                 (160, 2, '3 m .')]
         for d in data:
             (sg, i, symbol) = d
             wp = Group(sg)[i]
             wp.get_site_symmetry()
             self.assertTrue(wp.site_symm == symbol)
+            
+    def test_wp_dof(self):
+        for sg in range(1, 231):
+            g = Group(sg)
+            for wp in g:
+                axs = wp.get_frozen_axis()
+                self.assertTrue(wp.get_dof() + len(axs) == 3)
 
     def test_wp_label(self):
-        symbol = str(wp1.multiplicity) + wp1.letter
+        symbol = wp1.get_label()
         self.assertTrue(symbol == "8b")
-        symbol = str(wp2.multiplicity) + wp2.letter
+        symbol = wp2.get_label()
         self.assertTrue(symbol == "4a")
 
     def test_merge(self):
         pt, wp, _ = wp1.merge([0.05, 0.7, 0.24], l01.matrix, 0.5)
-        symbol = str(wp.multiplicity) + wp.letter
+        symbol = wp.get_label()
         self.assertTrue(symbol == "4a")
         pt, wp, _ = wp1.merge([0.15, 0.7, 0.24], l01.matrix, 0.5)
-        symbol = str(wp.multiplicity) + wp.letter
+        symbol = wp.get_label()
         self.assertTrue(symbol == "8b")
 
         wp = Group(167)[0]
         cell = np.diag([9, 9, 7])
         for pt in [[0.12, 0, 0.25], [0, 0.1316, 0.25]]:
             _, wpt, _ = wp.merge(pt, cell, 0.1)
-            symbol = str(wpt.multiplicity) + wpt.letter
+            symbol = wpt.get_label()
             self.assertTrue(symbol == "18e")
 
         for pt in [[0, 0, 3/4], [2/3, 1/3, 7/12]]:
             _, wpt, _ = wp.merge(pt, cell, 0.1)
-            symbol = str(wpt.multiplicity) + wpt.letter
+            symbol = wpt.get_label()
             self.assertTrue(symbol == "6a")
 
     def test_search_generator(self):
         wp = Group(167)[1]
         for pt in [[0, 0.13, 0.25], [0.13, 0, 0.25]]:
             wp0 = wp.search_generator(pt)
             self.assertTrue(wp0 is not None)
```

### Comparing `pyxtal-0.5.5/pyxtal/tolerance.py` & `pyxtal-0.5.6/pyxtal/tolerance.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/pyxtal/util.py` & `pyxtal-0.5.6/pyxtal/util.py`

 * *Files 15% similar despite different names*

```diff
@@ -430,14 +430,69 @@
     #print(vol/(a*b*np.sin(gamma)), a*b, np.sin(gamma))
     #print(vol/(a*c*np.sin(beta)), a*c, np.sin(beta))
     #print(vol/(b*c*np.sin(alpha)), b*c, np.sin(alpha))
     #print(Kpoints)
     #import sys; sys.exit()
     return Kpoints.astype(int)
 
+
+def sort_by_dimer(atoms, N_mols, id=10, tol=4.0):
+    """
+    sort the ase atoms' xyz according to dimer
+    so far only tested on aspirin
+
+    Args:
+        atoms: atoms object from pyxtal
+        N_mols: number of molecules
+        id: the refrence atom id
+        tol: tolerence distance to check if it is a dimer
+    """
+
+    N_atoms = int(len(atoms)/N_mols)
+    pos = atoms.get_scaled_positions()
+    refs = pos[id:len(pos):N_atoms, :]
+    #print(refs)
+
+    # compuate the indices and shift
+    orders = []
+    shifts = []
+    while len(orders) < N_mols:
+        lefts = [i for i in range(N_mols) if i not in orders]
+        i = lefts[0]
+        orders.append(i)
+        shifts.append(np.zeros(3))
+        ref_i = refs[i]
+        good = False
+        for j in lefts[1:]:
+            ref_j = refs[j]
+            dist = ref_j - ref_i
+            shift = np.round(dist)
+            dist -= shift
+            dist = np.linalg.norm(dist.dot(atoms.cell[:]))
+            if dist < tol:
+                orders.append(j)
+                shifts.append(shift)
+                good = True
+                break
+        if not good:
+            raise RuntimeError('Cannot find match on molecule', i)
+        else:
+            print('get', i, j, dist, shift)
+
+    pos0 = atoms.get_positions()
+    pos1 = np.zeros([len(pos), 3])
+    for i, id in enumerate(orders):
+        s1, e1 = id*N_atoms, (id+1)*N_atoms
+        s2, e2 = i*N_atoms, (i+1)*N_atoms
+        pos1[s2:e2, :] += pos0[s1:e1, :] - shifts[i].dot(atoms.cell[:])
+
+    atoms.set_positions(pos1)
+    return atoms
+ 
+
 if __name__ == "__main__":
     from argparse import ArgumentParser
 
     parser = ArgumentParser()
     parser.add_argument(
         "-f",
         dest="file",
```

### Comparing `pyxtal-0.5.5/pyxtal/viz.py` & `pyxtal-0.5.6/pyxtal/viz.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/pyxtal/wyckoff_site.py` & `pyxtal-0.5.6/pyxtal/wyckoff_site.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,26 +35,29 @@
         search: to search for the optimum position for special wyckoff site
     """
 
     def __init__(self, wp=None, coordinate=None, specie=1, search=False):
         self.position = np.array(coordinate)
         self.specie = Element(specie).short_name
         self.wp = wp
+        self.coordination = None
 
         self._get_dof()
         self.PBC = self.wp.PBC
         self.multiplicity = self.wp.multiplicity
         if search:
             self.search_position()
         self.update()
 
     def __str__(self):
         if not hasattr(self.wp, "site_symm"): self.wp.get_site_symmetry()
         s = "{:>2s} @ [{:7.4f} {:7.4f} {:7.4f}], ".format(self.specie, *self.position)
-        s += "WP [{:}{:}] ".format(self.wp.multiplicity, self.wp.letter)
+        s += "WP [{:}] ".format(self.wp.get_label())
+        if self.coordination is not None:
+            s += " CN [{:2d}] ".format(self.coordination)
         s += "Site [{:}]".format(self.wp.site_symm.replace(" ",""))
 
         return s
 
     def __repr__(self):
         return str(self)
 
@@ -110,14 +113,25 @@
                 ans = self.wp.ops[0].operate(coord)
                 diff = coord - ans
                 diff -= np.floor(diff)
                 if np.sum(diff**2)<1e-4:
                     self.position = coord - np.floor(coord)
                     break
 
+    def encode(self):
+        """
+        transform dict to 1D vector
+        [specie, wp.index, free x, y, z]
+        """
+        xyz = self.wp.get_free_xyzs(self.position)
+        #print(self.wp.ops[0].rotation_matrix, self.wp.get_frozen_axis(), self.wp.get_dof())
+        #print([self.specie, self.wp.index] + list(xyz))
+        return [self.specie, self.wp.index] + list(xyz)
+        
+
     def swap_axis(self, swap_id, shift=np.zeros(3)):
         """
         sometimes space groups like Pmm2 allows one to swap the a,b axes
         to get an alternative representation
         """
         self.position += shift
         self.position = self.position[swap_id]
@@ -288,15 +302,15 @@
     def __str__(self):
         if not hasattr(self.wp, "site_symm"): 
             self.wp.get_site_symmetry()
 
         self.angles = self.orientation.r.as_euler('zxy', degrees=True)
         formula = self.mol.formula.replace(" ","")
         s = "{:12s} @ [{:7.4f} {:7.4f} {:7.4f}]  ".format(formula, *self.position)
-        s += "WP [{:d}{:s}] ".format(self.wp.multiplicity, self.wp.letter)
+        s += "WP [{:s}] ".format(self.wp.get_label())
         s += "Site [{:}]".format(self.wp.site_symm.replace(" ",""))
         if len(self.molecule.mol) > 1:
             s += " Euler [{:6.1f} {:6.1f} {:6.1f}]".format(*self.angles)
 
         return s
 
     def __repr__(self):
```

### Comparing `pyxtal-0.5.5/pyxtal/wyckoff_split.py` & `pyxtal-0.5.6/pyxtal/wyckoff_split.py`

 * *Files 2% similar despite different names*

```diff
@@ -445,33 +445,32 @@
             if vector not in final_translation_list:
                 final_translation_list.append(vector)
 
         return final_translation_list
 
     def check_orbits(self, g1_orbits, wp2, wp2_lists):
         if len(g1_orbits) < len(wp2):
-            #s1 = str(wp1.multiplicity)+wp1.letter
             s2 = ""
             for wp2 in wp2_lists:
-                s2 += str(wp2.multiplicity)+wp2.letter
+                s2 += wp2.get_label() 
                 s2 += ', '
             # g, h = self.G.number, self.H.number
             # print("Error between {:d}[{:s}] -> {:d}[{:s}]".format(g, s1, h, s2))
             # print(self.R)
             # print(g1_orbits)
             # import sys; sys.exit()
             raise ValueError("Cannot find the generator for wp2")
 
     def __str__(self):
         s = "Wycokff split from {:d} to {:d}\n".format(self.G.number, self.H.number)
         for i, wp1 in enumerate(self.wp1_lists):
-            s += "\n{:d}{:s} -> ".format(wp1.multiplicity, wp1.letter)
+            s += "\n{:s} -> ".format(wp1.get_label()) 
 
             for j, wp2 in enumerate(self.wp2_lists[i]):
-                s += "{:d}{:s}\n".format(wp2.multiplicity, wp2.letter)
+                s += "{:s}\n".format(wp2.get_label()) 
                 g1s = self.G1_orbits[i][j]
                 g2s = self.G2_orbits[i][j]
                 Hs = self.H_orbits[i][j]
                 for g1_orbit, g2_orbit, h_orbit in zip(g1s, g2s, Hs):
                     g1_xyz = g1_orbit.as_xyz_string()
                     g2_xyz = g2_orbit.as_xyz_string()
                     h_xyz = h_orbit.as_xyz_string()
```

### Comparing `pyxtal-0.5.5/pyxtal.egg-info/PKG-INFO` & `pyxtal-0.5.6/pyxtal.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyxtal
-Version: 0.5.5
+Version: 0.5.6
 Summary: Python code for generation of crystal structures based on symmetry constraints.
 Home-page: https://github.com/qzhu2017/PyXtal
 Author: Scott Fredericks, Qiang Zhu
 Author-email: qiang.zhu@unlv.edu
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyxtal-0.5.5/pyxtal.egg-info/SOURCES.txt` & `pyxtal-0.5.6/pyxtal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/scripts/pyxtal_main.py` & `pyxtal-0.5.6/scripts/pyxtal_main.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/scripts/pyxtal_symmetry.py` & `pyxtal-0.5.6/scripts/pyxtal_symmetry.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.5/setup.py` & `pyxtal-0.5.6/setup.py`

 * *Files identical despite different names*

