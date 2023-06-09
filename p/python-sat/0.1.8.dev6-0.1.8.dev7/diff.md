# Comparing `tmp/python-sat-0.1.8.dev6.tar.gz` & `tmp/python-sat-0.1.8.dev7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-sat-0.1.8.dev6.tar", last modified: Sun Jun  4 07:55:49 2023, max compression
+gzip compressed data, was "python-sat-0.1.8.dev7.tar", last modified: Fri Jun  9 06:06:03 2023, max compression
```

## Comparing `python-sat-0.1.8.dev6.tar` & `python-sat-0.1.8.dev7.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2023-06-04 07:55:49.073139 python-sat-0.1.8.dev6/
--rw-r--r--   0 aign0002 (892519254) 907548567     1109 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev6/LICENSE.txt
--rw-r--r--   0 aign0002 (892519254) 907548567      217 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev6/MANIFEST.in
--rw-r--r--   0 aign0002 (892519254) 907548567     1193 2023-06-04 07:55:49.073227 python-sat-0.1.8.dev6/PKG-INFO
--rw-r--r--   0 aign0002 (892519254) 907548567    14137 2023-04-21 08:05:23.000000 python-sat-0.1.8.dev6/README.rst
-drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2023-06-04 07:55:49.052925 python-sat-0.1.8.dev6/allies/
--rw-------   0 aign0002 (892519254) 907548567        0 2023-04-14 00:41:27.000000 python-sat-0.1.8.dev6/allies/__init__.py
--rwxr-xr-x   0 aign0002 (892519254) 907548567    13572 2023-05-09 14:01:54.000000 python-sat-0.1.8.dev6/allies/approxmc.py
-drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2023-06-04 07:55:49.055528 python-sat-0.1.8.dev6/cardenc/
--rw-r--r--   0 aign0002 (892519254) 907548567     1375 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev6/cardenc/bitwise.hh
--rw-r--r--   0 aign0002 (892519254) 907548567     2468 2023-03-02 05:23:11.000000 python-sat-0.1.8.dev6/cardenc/card.hh
--rw-r--r--   0 aign0002 (892519254) 907548567     1874 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev6/cardenc/clset.hh
--rw-r--r--   0 aign0002 (892519254) 907548567     1303 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev6/cardenc/common.hh
--rw-r--r--   0 aign0002 (892519254) 907548567     4646 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev6/cardenc/itot.hh
--rw-r--r--   0 aign0002 (892519254) 907548567     2325 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev6/cardenc/ladder.hh
--rw-r--r--   0 aign0002 (892519254) 907548567    11355 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev6/cardenc/mto.hh
--rw-r--r--   0 aign0002 (892519254) 907548567     1008 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev6/cardenc/pairwise.hh
--rw-r--r--   0 aign0002 (892519254) 907548567      918 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev6/cardenc/ptypes.hh
--rw-r--r--   0 aign0002 (892519254) 907548567    15865 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev6/cardenc/pycard.cc
--rw-r--r--   0 aign0002 (892519254) 907548567     4851 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev6/cardenc/seqcounter.hh
--rw-r--r--   0 aign0002 (892519254) 907548567     8355 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev6/cardenc/sortcard.hh
--rw-r--r--   0 aign0002 (892519254) 907548567     5117 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev6/cardenc/utils.hh
-drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2023-06-04 07:55:49.057669 python-sat-0.1.8.dev6/examples/
--rw-------   0 aign0002 (892519254) 907548567        0 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev6/examples/__init__.py
--rwxr-xr-x   0 aign0002 (892519254) 907548567    17968 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev6/examples/fm.py
--rwxr-xr-x   0 aign0002 (892519254) 907548567    18986 2023-03-04 22:56:50.000000 python-sat-0.1.8.dev6/examples/genhard.py
--rwxr-xr-x   0 aign0002 (892519254) 907548567    25406 2023-06-04 07:07:20.000000 python-sat-0.1.8.dev6/examples/hitman.py
--rwxr-xr-x   0 aign0002 (892519254) 907548567    21295 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev6/examples/lbx.py
--rwxr-xr-x   0 aign0002 (892519254) 907548567    15523 2023-01-20 20:56:31.000000 python-sat-0.1.8.dev6/examples/lsu.py
--rwxr-xr-x   0 aign0002 (892519254) 907548567    20320 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev6/examples/mcsls.py
--rwxr-xr-x   0 aign0002 (892519254) 907548567     5724 2023-01-13 10:54:03.000000 python-sat-0.1.8.dev6/examples/models.py
--rwxr-xr-x   0 aign0002 (892519254) 907548567    10563 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev6/examples/musx.py
--rwxr-xr-x   0 aign0002 (892519254) 907548567    25636 2023-06-04 07:39:47.000000 python-sat-0.1.8.dev6/examples/optux.py
--rwxr-xr-x   0 aign0002 (892519254) 907548567    67020 2023-05-25 10:53:45.000000 python-sat-0.1.8.dev6/examples/rc2.py
--rwxr-xr-x   0 aign0002 (892519254) 907548567     2183 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev6/examples/usage.py
-drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2023-06-04 07:55:49.058958 python-sat-0.1.8.dev6/pysat/
--rw-r--r--   0 aign0002 (892519254) 907548567      653 2023-06-04 07:53:48.000000 python-sat-0.1.8.dev6/pysat/__init__.py
--rw-r--r--   0 aign0002 (892519254) 907548567     5814 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev6/pysat/_fileio.py
--rw-r--r--   0 aign0002 (892519254) 907548567     1340 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev6/pysat/_utils.py
--rw-r--r--   0 aign0002 (892519254) 907548567    30043 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev6/pysat/card.py
--rw-r--r--   0 aign0002 (892519254) 907548567    95959 2023-05-19 07:25:29.000000 python-sat-0.1.8.dev6/pysat/formula.py
--rw-r--r--   0 aign0002 (892519254) 907548567    15657 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev6/pysat/pb.py
--rw-r--r--   0 aign0002 (892519254) 907548567    11968 2023-03-05 06:22:14.000000 python-sat-0.1.8.dev6/pysat/process.py
--rw-r--r--   0 aign0002 (892519254) 907548567   175975 2023-06-04 02:20:27.000000 python-sat-0.1.8.dev6/pysat/solvers.py
-drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2023-06-04 07:55:49.059861 python-sat-0.1.8.dev6/python_sat.egg-info/
--rw-r--r--   0 aign0002 (892519254) 907548567     1193 2023-06-04 07:55:48.000000 python-sat-0.1.8.dev6/python_sat.egg-info/PKG-INFO
--rw-r--r--   0 aign0002 (892519254) 907548567     1863 2023-06-04 07:55:49.000000 python-sat-0.1.8.dev6/python_sat.egg-info/SOURCES.txt
--rw-r--r--   0 aign0002 (892519254) 907548567        1 2023-06-04 07:55:48.000000 python-sat-0.1.8.dev6/python_sat.egg-info/dependency_links.txt
--rw-r--r--   0 aign0002 (892519254) 907548567       87 2023-06-04 07:55:48.000000 python-sat-0.1.8.dev6/python_sat.egg-info/requires.txt
--rw-r--r--   0 aign0002 (892519254) 907548567       23 2023-06-04 07:55:48.000000 python-sat-0.1.8.dev6/python_sat.egg-info/top_level.txt
--rw-r--r--   0 aign0002 (892519254) 907548567       39 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev6/requirements.txt
--rw-r--r--   0 aign0002 (892519254) 907548567      107 2023-06-04 07:55:49.073491 python-sat-0.1.8.dev6/setup.cfg
--rw-r--r--   0 aign0002 (892519254) 907548567     6549 2023-04-21 07:47:02.000000 python-sat-0.1.8.dev6/setup.py
-drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2023-06-04 07:55:49.064825 python-sat-0.1.8.dev6/solvers/
--rw-r--r--   0 aign0002 (892519254) 907548567   547031 2023-03-02 05:10:30.000000 python-sat-0.1.8.dev6/solvers/cadical103.tar.gz
--rw-r--r--   0 aign0002 (892519254) 907548567   596433 2023-03-03 10:16:48.000000 python-sat-0.1.8.dev6/solvers/cadical153.tar.gz
--rw-r--r--   0 aign0002 (892519254) 907548567    50813 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev6/solvers/glucose30.tar.gz
--rw-r--r--   0 aign0002 (892519254) 907548567    82779 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev6/solvers/glucose41.tar.gz
--rw-r--r--   0 aign0002 (892519254) 907548567   501731 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev6/solvers/lingeling.tar.gz
--rw-r--r--   0 aign0002 (892519254) 907548567    82656 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev6/solvers/maplechrono.zip
--rw-r--r--   0 aign0002 (892519254) 907548567    94949 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev6/solvers/maplecm.zip
--rw-r--r--   0 aign0002 (892519254) 907548567    77088 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev6/solvers/maplesat.zip
--rw-r--r--   0 aign0002 (892519254) 907548567   179223 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev6/solvers/mergesat3.tar.gz
--rw-r--r--   0 aign0002 (892519254) 907548567  1529188 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev6/solvers/minicard.tar.gz
--rw-r--r--   0 aign0002 (892519254) 907548567    43879 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev6/solvers/minisat22.tar.gz
--rw-r--r--   0 aign0002 (892519254) 907548567    75209 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev6/solvers/minisatgh.zip
-drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2023-06-04 07:55:49.069556 python-sat-0.1.8.dev6/solvers/patches/
--rw-r--r--   0 aign0002 (892519254) 907548567    51588 2023-03-02 05:15:52.000000 python-sat-0.1.8.dev6/solvers/patches/cadical103.patch
--rw-r--r--   0 aign0002 (892519254) 907548567    66092 2023-06-03 01:29:02.000000 python-sat-0.1.8.dev6/solvers/patches/cadical153.patch
--rw-r--r--   0 aign0002 (892519254) 907548567    93207 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev6/solvers/patches/glucose30.patch
--rw-r--r--   0 aign0002 (892519254) 907548567    89206 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev6/solvers/patches/glucose41.patch
--rw-r--r--   0 aign0002 (892519254) 907548567   117955 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev6/solvers/patches/gluecard30.patch
--rw-r--r--   0 aign0002 (892519254) 907548567   137342 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev6/solvers/patches/gluecard41.patch
--rw-r--r--   0 aign0002 (892519254) 907548567    54848 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev6/solvers/patches/lingeling.patch
--rw-r--r--   0 aign0002 (892519254) 907548567    90618 2023-01-14 22:24:35.000000 python-sat-0.1.8.dev6/solvers/patches/maplechrono.patch
--rw-r--r--   0 aign0002 (892519254) 907548567   114715 2023-01-14 21:29:08.000000 python-sat-0.1.8.dev6/solvers/patches/maplecm.patch
--rw-r--r--   0 aign0002 (892519254) 907548567    82379 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev6/solvers/patches/maplesat.patch
--rw-r--r--   0 aign0002 (892519254) 907548567    88893 2023-01-14 22:24:31.000000 python-sat-0.1.8.dev6/solvers/patches/mergesat3.patch
--rw-r--r--   0 aign0002 (892519254) 907548567    51757 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev6/solvers/patches/minicard.patch
--rw-r--r--   0 aign0002 (892519254) 907548567    42627 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev6/solvers/patches/minisat22.patch
--rw-r--r--   0 aign0002 (892519254) 907548567    60626 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev6/solvers/patches/minisatgh.patch
--rw-r--r--   0 aign0002 (892519254) 907548567    25391 2023-06-03 01:04:24.000000 python-sat-0.1.8.dev6/solvers/prepare.py
--rw-r--r--   0 aign0002 (892519254) 907548567   223063 2023-06-04 02:10:25.000000 python-sat-0.1.8.dev6/solvers/pysolvers.cc
-drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2023-06-04 07:55:49.072728 python-sat-0.1.8.dev6/tests/
--rw-r--r--   0 aign0002 (892519254) 907548567      948 2023-03-05 08:16:22.000000 python-sat-0.1.8.dev6/tests/test_accum_stats.py
--rw-r--r--   0 aign0002 (892519254) 907548567      429 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev6/tests/test_atmost.py
--rw-r--r--   0 aign0002 (892519254) 907548567      707 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev6/tests/test_atmost1.py
--rw-r--r--   0 aign0002 (892519254) 907548567      998 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev6/tests/test_atmostk.py
--rw-r--r--   0 aign0002 (892519254) 907548567     2408 2023-03-05 08:17:09.000000 python-sat-0.1.8.dev6/tests/test_cnfplus.py
--rw-r--r--   0 aign0002 (892519254) 907548567      784 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev6/tests/test_equals1.py
--rw-r--r--   0 aign0002 (892519254) 907548567     1007 2023-03-05 06:31:37.000000 python-sat-0.1.8.dev6/tests/test_process.py
--rw-r--r--   0 aign0002 (892519254) 907548567      866 2023-03-05 08:17:46.000000 python-sat-0.1.8.dev6/tests/test_unique_model.py
--rw-r--r--   0 aign0002 (892519254) 907548567      937 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev6/tests/test_unique_mus.py
--rw-r--r--   0 aign0002 (892519254) 907548567      643 2023-01-14 22:33:39.000000 python-sat-0.1.8.dev6/tests/test_warmstart.py
+drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2023-06-09 06:06:03.666219 python-sat-0.1.8.dev7/
+-rw-r--r--   0 aign0002 (892519254) 907548567     1109 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev7/LICENSE.txt
+-rw-r--r--   0 aign0002 (892519254) 907548567      217 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev7/MANIFEST.in
+-rw-r--r--   0 aign0002 (892519254) 907548567     1193 2023-06-09 06:06:03.666314 python-sat-0.1.8.dev7/PKG-INFO
+-rw-r--r--   0 aign0002 (892519254) 907548567    14137 2023-04-21 08:05:23.000000 python-sat-0.1.8.dev7/README.rst
+drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2023-06-09 06:06:03.634205 python-sat-0.1.8.dev7/allies/
+-rw-------   0 aign0002 (892519254) 907548567        0 2023-04-14 00:41:27.000000 python-sat-0.1.8.dev7/allies/__init__.py
+-rwxr-xr-x   0 aign0002 (892519254) 907548567    13572 2023-05-09 14:01:54.000000 python-sat-0.1.8.dev7/allies/approxmc.py
+drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2023-06-09 06:06:03.637763 python-sat-0.1.8.dev7/cardenc/
+-rw-r--r--   0 aign0002 (892519254) 907548567     1375 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev7/cardenc/bitwise.hh
+-rw-r--r--   0 aign0002 (892519254) 907548567     2468 2023-03-02 05:23:11.000000 python-sat-0.1.8.dev7/cardenc/card.hh
+-rw-r--r--   0 aign0002 (892519254) 907548567     1874 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev7/cardenc/clset.hh
+-rw-r--r--   0 aign0002 (892519254) 907548567     1303 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev7/cardenc/common.hh
+-rw-r--r--   0 aign0002 (892519254) 907548567     4646 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev7/cardenc/itot.hh
+-rw-r--r--   0 aign0002 (892519254) 907548567     2325 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev7/cardenc/ladder.hh
+-rw-r--r--   0 aign0002 (892519254) 907548567    11355 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev7/cardenc/mto.hh
+-rw-r--r--   0 aign0002 (892519254) 907548567     1008 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev7/cardenc/pairwise.hh
+-rw-r--r--   0 aign0002 (892519254) 907548567      918 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev7/cardenc/ptypes.hh
+-rw-r--r--   0 aign0002 (892519254) 907548567    15865 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev7/cardenc/pycard.cc
+-rw-r--r--   0 aign0002 (892519254) 907548567     4851 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev7/cardenc/seqcounter.hh
+-rw-r--r--   0 aign0002 (892519254) 907548567     8355 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev7/cardenc/sortcard.hh
+-rw-r--r--   0 aign0002 (892519254) 907548567     5117 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev7/cardenc/utils.hh
+drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2023-06-09 06:06:03.641838 python-sat-0.1.8.dev7/examples/
+-rw-------   0 aign0002 (892519254) 907548567        0 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev7/examples/__init__.py
+-rwxr-xr-x   0 aign0002 (892519254) 907548567    17968 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev7/examples/fm.py
+-rwxr-xr-x   0 aign0002 (892519254) 907548567    18986 2023-03-04 22:56:50.000000 python-sat-0.1.8.dev7/examples/genhard.py
+-rwxr-xr-x   0 aign0002 (892519254) 907548567    25406 2023-06-04 07:07:20.000000 python-sat-0.1.8.dev7/examples/hitman.py
+-rwxr-xr-x   0 aign0002 (892519254) 907548567    21295 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev7/examples/lbx.py
+-rwxr-xr-x   0 aign0002 (892519254) 907548567    15523 2023-01-20 20:56:31.000000 python-sat-0.1.8.dev7/examples/lsu.py
+-rwxr-xr-x   0 aign0002 (892519254) 907548567    20320 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev7/examples/mcsls.py
+-rwxr-xr-x   0 aign0002 (892519254) 907548567     5724 2023-01-13 10:54:03.000000 python-sat-0.1.8.dev7/examples/models.py
+-rwxr-xr-x   0 aign0002 (892519254) 907548567    10563 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev7/examples/musx.py
+-rwxr-xr-x   0 aign0002 (892519254) 907548567    25636 2023-06-04 07:39:47.000000 python-sat-0.1.8.dev7/examples/optux.py
+-rwxr-xr-x   0 aign0002 (892519254) 907548567    67270 2023-06-09 06:00:18.000000 python-sat-0.1.8.dev7/examples/rc2.py
+-rwxr-xr-x   0 aign0002 (892519254) 907548567     2183 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev7/examples/usage.py
+drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2023-06-09 06:06:03.644785 python-sat-0.1.8.dev7/pysat/
+-rw-r--r--   0 aign0002 (892519254) 907548567      653 2023-06-09 06:01:09.000000 python-sat-0.1.8.dev7/pysat/__init__.py
+-rw-r--r--   0 aign0002 (892519254) 907548567     5814 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev7/pysat/_fileio.py
+-rw-r--r--   0 aign0002 (892519254) 907548567     1340 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev7/pysat/_utils.py
+-rw-r--r--   0 aign0002 (892519254) 907548567    30043 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev7/pysat/card.py
+-rw-r--r--   0 aign0002 (892519254) 907548567    95959 2023-05-19 07:25:29.000000 python-sat-0.1.8.dev7/pysat/formula.py
+-rw-r--r--   0 aign0002 (892519254) 907548567    15657 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev7/pysat/pb.py
+-rw-r--r--   0 aign0002 (892519254) 907548567    11968 2023-03-05 06:22:14.000000 python-sat-0.1.8.dev7/pysat/process.py
+-rw-r--r--   0 aign0002 (892519254) 907548567   175975 2023-06-04 02:20:27.000000 python-sat-0.1.8.dev7/pysat/solvers.py
+drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2023-06-09 06:06:03.646113 python-sat-0.1.8.dev7/python_sat.egg-info/
+-rw-r--r--   0 aign0002 (892519254) 907548567     1193 2023-06-09 06:06:03.000000 python-sat-0.1.8.dev7/python_sat.egg-info/PKG-INFO
+-rw-r--r--   0 aign0002 (892519254) 907548567     1863 2023-06-09 06:06:03.000000 python-sat-0.1.8.dev7/python_sat.egg-info/SOURCES.txt
+-rw-r--r--   0 aign0002 (892519254) 907548567        1 2023-06-09 06:06:03.000000 python-sat-0.1.8.dev7/python_sat.egg-info/dependency_links.txt
+-rw-r--r--   0 aign0002 (892519254) 907548567       87 2023-06-09 06:06:03.000000 python-sat-0.1.8.dev7/python_sat.egg-info/requires.txt
+-rw-r--r--   0 aign0002 (892519254) 907548567       23 2023-06-09 06:06:03.000000 python-sat-0.1.8.dev7/python_sat.egg-info/top_level.txt
+-rw-r--r--   0 aign0002 (892519254) 907548567       39 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev7/requirements.txt
+-rw-r--r--   0 aign0002 (892519254) 907548567      107 2023-06-09 06:06:03.666606 python-sat-0.1.8.dev7/setup.cfg
+-rw-r--r--   0 aign0002 (892519254) 907548567     6549 2023-04-21 07:47:02.000000 python-sat-0.1.8.dev7/setup.py
+drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2023-06-09 06:06:03.656003 python-sat-0.1.8.dev7/solvers/
+-rw-r--r--   0 aign0002 (892519254) 907548567   547031 2023-03-02 05:10:30.000000 python-sat-0.1.8.dev7/solvers/cadical103.tar.gz
+-rw-r--r--   0 aign0002 (892519254) 907548567   596433 2023-03-03 10:16:48.000000 python-sat-0.1.8.dev7/solvers/cadical153.tar.gz
+-rw-r--r--   0 aign0002 (892519254) 907548567    50813 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev7/solvers/glucose30.tar.gz
+-rw-r--r--   0 aign0002 (892519254) 907548567    82779 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev7/solvers/glucose41.tar.gz
+-rw-r--r--   0 aign0002 (892519254) 907548567   501731 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev7/solvers/lingeling.tar.gz
+-rw-r--r--   0 aign0002 (892519254) 907548567    82656 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev7/solvers/maplechrono.zip
+-rw-r--r--   0 aign0002 (892519254) 907548567    94949 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev7/solvers/maplecm.zip
+-rw-r--r--   0 aign0002 (892519254) 907548567    77088 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev7/solvers/maplesat.zip
+-rw-r--r--   0 aign0002 (892519254) 907548567   179223 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev7/solvers/mergesat3.tar.gz
+-rw-r--r--   0 aign0002 (892519254) 907548567  1529188 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev7/solvers/minicard.tar.gz
+-rw-r--r--   0 aign0002 (892519254) 907548567    43879 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev7/solvers/minisat22.tar.gz
+-rw-r--r--   0 aign0002 (892519254) 907548567    75209 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev7/solvers/minisatgh.zip
+drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2023-06-09 06:06:03.663515 python-sat-0.1.8.dev7/solvers/patches/
+-rw-r--r--   0 aign0002 (892519254) 907548567    51588 2023-03-02 05:15:52.000000 python-sat-0.1.8.dev7/solvers/patches/cadical103.patch
+-rw-r--r--   0 aign0002 (892519254) 907548567    66092 2023-06-03 01:29:02.000000 python-sat-0.1.8.dev7/solvers/patches/cadical153.patch
+-rw-r--r--   0 aign0002 (892519254) 907548567    93207 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev7/solvers/patches/glucose30.patch
+-rw-r--r--   0 aign0002 (892519254) 907548567    89206 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev7/solvers/patches/glucose41.patch
+-rw-r--r--   0 aign0002 (892519254) 907548567   117955 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev7/solvers/patches/gluecard30.patch
+-rw-r--r--   0 aign0002 (892519254) 907548567   137342 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev7/solvers/patches/gluecard41.patch
+-rw-r--r--   0 aign0002 (892519254) 907548567    54848 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev7/solvers/patches/lingeling.patch
+-rw-r--r--   0 aign0002 (892519254) 907548567    90618 2023-01-14 22:24:35.000000 python-sat-0.1.8.dev7/solvers/patches/maplechrono.patch
+-rw-r--r--   0 aign0002 (892519254) 907548567   114715 2023-01-14 21:29:08.000000 python-sat-0.1.8.dev7/solvers/patches/maplecm.patch
+-rw-r--r--   0 aign0002 (892519254) 907548567    82379 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev7/solvers/patches/maplesat.patch
+-rw-r--r--   0 aign0002 (892519254) 907548567    88893 2023-01-14 22:24:31.000000 python-sat-0.1.8.dev7/solvers/patches/mergesat3.patch
+-rw-r--r--   0 aign0002 (892519254) 907548567    51757 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev7/solvers/patches/minicard.patch
+-rw-r--r--   0 aign0002 (892519254) 907548567    42627 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev7/solvers/patches/minisat22.patch
+-rw-r--r--   0 aign0002 (892519254) 907548567    60626 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev7/solvers/patches/minisatgh.patch
+-rw-r--r--   0 aign0002 (892519254) 907548567    25391 2023-06-03 01:04:24.000000 python-sat-0.1.8.dev7/solvers/prepare.py
+-rw-r--r--   0 aign0002 (892519254) 907548567   223063 2023-06-04 02:10:25.000000 python-sat-0.1.8.dev7/solvers/pysolvers.cc
+drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2023-06-09 06:06:03.665915 python-sat-0.1.8.dev7/tests/
+-rw-r--r--   0 aign0002 (892519254) 907548567      948 2023-03-05 08:16:22.000000 python-sat-0.1.8.dev7/tests/test_accum_stats.py
+-rw-r--r--   0 aign0002 (892519254) 907548567      429 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev7/tests/test_atmost.py
+-rw-r--r--   0 aign0002 (892519254) 907548567      707 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev7/tests/test_atmost1.py
+-rw-r--r--   0 aign0002 (892519254) 907548567      998 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev7/tests/test_atmostk.py
+-rw-r--r--   0 aign0002 (892519254) 907548567     2408 2023-03-05 08:17:09.000000 python-sat-0.1.8.dev7/tests/test_cnfplus.py
+-rw-r--r--   0 aign0002 (892519254) 907548567      784 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev7/tests/test_equals1.py
+-rw-r--r--   0 aign0002 (892519254) 907548567     1007 2023-03-05 06:31:37.000000 python-sat-0.1.8.dev7/tests/test_process.py
+-rw-r--r--   0 aign0002 (892519254) 907548567      866 2023-03-05 08:17:46.000000 python-sat-0.1.8.dev7/tests/test_unique_model.py
+-rw-r--r--   0 aign0002 (892519254) 907548567      937 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev7/tests/test_unique_mus.py
+-rw-r--r--   0 aign0002 (892519254) 907548567      643 2023-01-14 22:33:39.000000 python-sat-0.1.8.dev7/tests/test_warmstart.py
```

### Comparing `python-sat-0.1.8.dev6/LICENSE.txt` & `python-sat-0.1.8.dev7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev6/PKG-INFO` & `python-sat-0.1.8.dev7/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-sat
-Version: 0.1.8.dev6
+Version: 0.1.8.dev7
 Summary: A Python library for prototyping with SAT oracles
 Home-page: https://github.com/pysathq/pysat
 Author: Alexey Ignatiev, Joao Marques-Silva, Antonio Morgado
 Author-email: alexey.ignatiev@monash.edu, joao.marques-silva@univ-toulouse.fr, ajrmorgado@gmail.com
 License: MIT
 Description-Content-Type: text/x-rst; charset=UTF-8
 Provides-Extra: aiger
```

### Comparing `python-sat-0.1.8.dev6/README.rst` & `python-sat-0.1.8.dev7/README.rst`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev6/allies/approxmc.py` & `python-sat-0.1.8.dev7/allies/approxmc.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev6/cardenc/bitwise.hh` & `python-sat-0.1.8.dev7/cardenc/bitwise.hh`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev6/cardenc/card.hh` & `python-sat-0.1.8.dev7/cardenc/card.hh`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev6/cardenc/clset.hh` & `python-sat-0.1.8.dev7/cardenc/clset.hh`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev6/cardenc/common.hh` & `python-sat-0.1.8.dev7/cardenc/common.hh`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev6/cardenc/itot.hh` & `python-sat-0.1.8.dev7/cardenc/itot.hh`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev6/cardenc/ladder.hh` & `python-sat-0.1.8.dev7/cardenc/ladder.hh`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev6/cardenc/mto.hh` & `python-sat-0.1.8.dev7/cardenc/mto.hh`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev6/cardenc/pairwise.hh` & `python-sat-0.1.8.dev7/cardenc/pairwise.hh`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev6/cardenc/ptypes.hh` & `python-sat-0.1.8.dev7/cardenc/ptypes.hh`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev6/cardenc/pycard.cc` & `python-sat-0.1.8.dev7/cardenc/pycard.cc`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev6/cardenc/seqcounter.hh` & `python-sat-0.1.8.dev7/cardenc/seqcounter.hh`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev6/cardenc/sortcard.hh` & `python-sat-0.1.8.dev7/cardenc/sortcard.hh`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev6/cardenc/utils.hh` & `python-sat-0.1.8.dev7/cardenc/utils.hh`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev6/examples/fm.py` & `python-sat-0.1.8.dev7/examples/fm.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev6/examples/genhard.py` & `python-sat-0.1.8.dev7/examples/genhard.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev6/examples/hitman.py` & `python-sat-0.1.8.dev7/examples/hitman.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev6/examples/lbx.py` & `python-sat-0.1.8.dev7/examples/lbx.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev6/examples/lsu.py` & `python-sat-0.1.8.dev7/examples/lsu.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev6/examples/mcsls.py` & `python-sat-0.1.8.dev7/examples/mcsls.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev6/examples/models.py` & `python-sat-0.1.8.dev7/examples/models.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev6/examples/musx.py` & `python-sat-0.1.8.dev7/examples/musx.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev6/examples/optux.py` & `python-sat-0.1.8.dev7/examples/optux.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev6/examples/rc2.py` & `python-sat-0.1.8.dev7/examples/rc2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1117,29 +1117,35 @@
 
                 # a new at-most-b constraint
                 amb = [[-t.rhs[b]] * (rhs - b) + t.lits, rhs]
                 self.oracle.add_atmost(*amb)
 
         return t, b
 
-    def set_bound(self, tobj, rhs, weight):
+    def set_bound(self, tobj, rhs, weight=None):
         """
             Given a totalizer sum, its right-hand side to be enforced, and a
             weight, the method creates a new sum assumption literal, which
-            will be used in the following SAT oracle calls.
+            will be used in the following SAT oracle calls. If ``weight`` is
+            left unspecified, the current core's weight, i.e. ``self.minw``,
+            is used.
 
             :param tobj: totalizer sum
             :param rhs: right-hand side
             :param weight: numeric weight of the assumption
 
             :type tobj: :class:`.ITotalizer`
             :type rhs: int
             :type weight: int
         """
 
+        if weight is None:
+            # if no specific weight is provided, use the core's weight
+            weight = self.minw
+
         # saving the sum and its weight in a mapping
         self.tobj[-tobj.rhs[rhs]] = tobj
         self.bnds[-tobj.rhs[rhs]] = rhs
         self.wght[-tobj.rhs[rhs]] = weight
         self.swgt[-tobj.rhs[rhs]] = weight
 
         # adding a new assumption to force the sum to be at most rhs
```

### Comparing `python-sat-0.1.8.dev6/examples/usage.py` & `python-sat-0.1.8.dev7/examples/usage.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev6/pysat/__init__.py` & `python-sat-0.1.8.dev7/pysat/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 ##  Created on: Mar 4, 2017
 ##      Author: Alexey S. Ignatiev
 ##      E-mail: aignatiev@ciencias.ulisboa.pt
 ##
 
 # current version
 #==============================================================================
-VERSION = (0, 1, 8, "dev", 6)
+VERSION = (0, 1, 8, "dev", 7)
 
 
 # PEP440 Format
 #==============================================================================
 __version__ = "%d.%d.%d.%s%d" % VERSION if len(VERSION) == 5 else \
               "%d.%d.%d" % VERSION
```

### Comparing `python-sat-0.1.8.dev6/pysat/_fileio.py` & `python-sat-0.1.8.dev7/pysat/_fileio.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev6/pysat/_utils.py` & `python-sat-0.1.8.dev7/pysat/_utils.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev6/pysat/card.py` & `python-sat-0.1.8.dev7/pysat/card.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev6/pysat/formula.py` & `python-sat-0.1.8.dev7/pysat/formula.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev6/pysat/pb.py` & `python-sat-0.1.8.dev7/pysat/pb.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev6/pysat/process.py` & `python-sat-0.1.8.dev7/pysat/process.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev6/pysat/solvers.py` & `python-sat-0.1.8.dev7/pysat/solvers.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev6/python_sat.egg-info/PKG-INFO` & `python-sat-0.1.8.dev7/python_sat.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-sat
-Version: 0.1.8.dev6
+Version: 0.1.8.dev7
 Summary: A Python library for prototyping with SAT oracles
 Home-page: https://github.com/pysathq/pysat
 Author: Alexey Ignatiev, Joao Marques-Silva, Antonio Morgado
 Author-email: alexey.ignatiev@monash.edu, joao.marques-silva@univ-toulouse.fr, ajrmorgado@gmail.com
 License: MIT
 Description-Content-Type: text/x-rst; charset=UTF-8
 Provides-Extra: aiger
```

### Comparing `python-sat-0.1.8.dev6/python_sat.egg-info/SOURCES.txt` & `python-sat-0.1.8.dev7/python_sat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev6/setup.py` & `python-sat-0.1.8.dev7/setup.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev6/solvers/cadical103.tar.gz` & `python-sat-0.1.8.dev7/solvers/cadical103.tar.gz`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev6/solvers/cadical153.tar.gz` & `python-sat-0.1.8.dev7/solvers/cadical153.tar.gz`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev6/solvers/glucose30.tar.gz` & `python-sat-0.1.8.dev7/solvers/glucose30.tar.gz`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev6/solvers/glucose41.tar.gz` & `python-sat-0.1.8.dev7/solvers/glucose41.tar.gz`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev6/solvers/lingeling.tar.gz` & `python-sat-0.1.8.dev7/solvers/lingeling.tar.gz`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev6/solvers/maplechrono.zip` & `python-sat-0.1.8.dev7/solvers/maplechrono.zip`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev6/solvers/maplecm.zip` & `python-sat-0.1.8.dev7/solvers/maplecm.zip`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev6/solvers/maplesat.zip` & `python-sat-0.1.8.dev7/solvers/maplesat.zip`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev6/solvers/mergesat3.tar.gz` & `python-sat-0.1.8.dev7/solvers/mergesat3.tar.gz`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev6/solvers/minicard.tar.gz` & `python-sat-0.1.8.dev7/solvers/minicard.tar.gz`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev6/solvers/minisat22.tar.gz` & `python-sat-0.1.8.dev7/solvers/minisat22.tar.gz`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev6/solvers/minisatgh.zip` & `python-sat-0.1.8.dev7/solvers/minisatgh.zip`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev6/solvers/patches/cadical103.patch` & `python-sat-0.1.8.dev7/solvers/patches/cadical103.patch`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev6/solvers/patches/cadical153.patch` & `python-sat-0.1.8.dev7/solvers/patches/cadical153.patch`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev6/solvers/patches/glucose30.patch` & `python-sat-0.1.8.dev7/solvers/patches/glucose30.patch`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev6/solvers/patches/glucose41.patch` & `python-sat-0.1.8.dev7/solvers/patches/glucose41.patch`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev6/solvers/patches/gluecard30.patch` & `python-sat-0.1.8.dev7/solvers/patches/gluecard30.patch`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev6/solvers/patches/gluecard41.patch` & `python-sat-0.1.8.dev7/solvers/patches/gluecard41.patch`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev6/solvers/patches/lingeling.patch` & `python-sat-0.1.8.dev7/solvers/patches/lingeling.patch`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev6/solvers/patches/maplechrono.patch` & `python-sat-0.1.8.dev7/solvers/patches/maplechrono.patch`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev6/solvers/patches/maplecm.patch` & `python-sat-0.1.8.dev7/solvers/patches/maplecm.patch`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev6/solvers/patches/maplesat.patch` & `python-sat-0.1.8.dev7/solvers/patches/maplesat.patch`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev6/solvers/patches/mergesat3.patch` & `python-sat-0.1.8.dev7/solvers/patches/mergesat3.patch`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev6/solvers/patches/minicard.patch` & `python-sat-0.1.8.dev7/solvers/patches/minicard.patch`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev6/solvers/patches/minisat22.patch` & `python-sat-0.1.8.dev7/solvers/patches/minisat22.patch`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev6/solvers/patches/minisatgh.patch` & `python-sat-0.1.8.dev7/solvers/patches/minisatgh.patch`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev6/solvers/prepare.py` & `python-sat-0.1.8.dev7/solvers/prepare.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev6/solvers/pysolvers.cc` & `python-sat-0.1.8.dev7/solvers/pysolvers.cc`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev6/tests/test_accum_stats.py` & `python-sat-0.1.8.dev7/tests/test_accum_stats.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev6/tests/test_atmost1.py` & `python-sat-0.1.8.dev7/tests/test_atmost1.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev6/tests/test_atmostk.py` & `python-sat-0.1.8.dev7/tests/test_atmostk.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev6/tests/test_cnfplus.py` & `python-sat-0.1.8.dev7/tests/test_cnfplus.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev6/tests/test_equals1.py` & `python-sat-0.1.8.dev7/tests/test_equals1.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev6/tests/test_process.py` & `python-sat-0.1.8.dev7/tests/test_process.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev6/tests/test_unique_model.py` & `python-sat-0.1.8.dev7/tests/test_unique_model.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev6/tests/test_unique_mus.py` & `python-sat-0.1.8.dev7/tests/test_unique_mus.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev6/tests/test_warmstart.py` & `python-sat-0.1.8.dev7/tests/test_warmstart.py`

 * *Files identical despite different names*

