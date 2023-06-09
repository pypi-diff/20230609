# Comparing `tmp/lincs-0.4.0.tar.gz` & `tmp/lincs-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lincs-0.4.0.tar", last modified: Thu Jun  8 08:00:09 2023, max compression
+gzip compressed data, was "lincs-0.4.1.tar", last modified: Fri Jun  9 14:13:14 2023, max compression
```

## Comparing `lincs-0.4.0.tar` & `lincs-0.4.1.tar`

### file list

```diff
@@ -1,70 +1,72 @@
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-06-08 08:00:09.112882 lincs-0.4.0/
--rw-rw-r--   0 user      (1002) user      (1002)    35149 2023-06-05 12:32:48.000000 lincs-0.4.0/COPYING
--rw-rw-r--   0 user      (1002) user      (1002)     7652 2023-06-05 12:32:35.000000 lincs-0.4.0/COPYING.LESSER
--rw-rw-r--   0 user      (1002) user      (1002)      109 2023-06-05 12:32:35.000000 lincs-0.4.0/MANIFEST.in
--rw-r--r--   0 user      (1002) user      (1002)     4918 2023-06-08 08:00:09.112882 lincs-0.4.0/PKG-INFO
--rw-rw-r--   0 user      (1002) user      (1002)     4034 2023-06-08 08:00:04.000000 lincs-0.4.0/README.rst
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-06-08 08:00:09.108882 lincs-0.4.0/lincs/
--rw-rw-r--   0 user      (1002) user      (1002)      955 2023-06-08 07:34:07.000000 lincs-0.4.0/lincs/__init__.py
--rw-rw-r--   0 user      (1002) user      (1002)      170 2023-06-05 12:32:35.000000 lincs-0.4.0/lincs/__main__.py
--rw-rw-r--   0 user      (1002) user      (1002)    23086 2023-06-08 07:34:07.000000 lincs-0.4.0/lincs/command_line_interface.py
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-06-08 08:00:09.108882 lincs-0.4.0/lincs/liblincs/
--rw-rw-r--   0 user      (1002) user      (1002)     1627 2023-06-08 07:34:07.000000 lincs-0.4.0/lincs/liblincs/classification.cpp
--rw-rw-r--   0 user      (1002) user      (1002)      369 2023-06-08 07:34:07.000000 lincs-0.4.0/lincs/liblincs/classification.hpp
--rw-rw-r--   0 user      (1002) user      (1002)    10079 2023-06-08 07:34:07.000000 lincs-0.4.0/lincs/liblincs/generation.cpp
--rw-rw-r--   0 user      (1002) user      (1002)     1046 2023-06-08 07:34:07.000000 lincs-0.4.0/lincs/liblincs/generation.hpp
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-06-08 08:00:09.108882 lincs-0.4.0/lincs/liblincs/io/
--rw-rw-r--   0 user      (1002) user      (1002)     2468 2023-06-08 07:34:07.000000 lincs-0.4.0/lincs/liblincs/io/alternatives.cpp
--rw-rw-r--   0 user      (1002) user      (1002)     1012 2023-06-08 07:34:07.000000 lincs-0.4.0/lincs/liblincs/io/alternatives.hpp
--rw-rw-r--   0 user      (1002) user      (1002)     1886 2023-06-08 07:34:07.000000 lincs-0.4.0/lincs/liblincs/io/model.cpp
--rw-rw-r--   0 user      (1002) user      (1002)     1648 2023-06-08 07:34:07.000000 lincs-0.4.0/lincs/liblincs/io/model.hpp
--rw-rw-r--   0 user      (1002) user      (1002)     2610 2023-06-08 07:34:07.000000 lincs-0.4.0/lincs/liblincs/io/problem.cpp
--rw-rw-r--   0 user      (1002) user      (1002)     1892 2023-06-08 07:34:07.000000 lincs-0.4.0/lincs/liblincs/io/problem.hpp
--rw-rw-r--   0 user      (1002) user      (1002)       53 2023-06-05 12:32:35.000000 lincs-0.4.0/lincs/liblincs/io.cpp
--rw-rw-r--   0 user      (1002) user      (1002)      187 2023-06-08 07:34:07.000000 lincs-0.4.0/lincs/liblincs/io.hpp
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-06-08 08:00:09.108882 lincs-0.4.0/lincs/liblincs/learning/
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-06-08 08:00:09.104882 lincs-0.4.0/lincs/liblincs/learning/weights-profiles-breed-mrsort/
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-06-08 08:00:09.108882 lincs-0.4.0/lincs/liblincs/learning/weights-profiles-breed-mrsort/improve-profiles/
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-06-08 08:00:09.108882 lincs-0.4.0/lincs/liblincs/learning/weights-profiles-breed-mrsort/improve-profiles/accuracy-heuristic/
--rw-rw-r--   0 user      (1002) user      (1002)     1495 2023-06-08 06:59:23.000000 lincs-0.4.0/lincs/liblincs/learning/weights-profiles-breed-mrsort/improve-profiles/accuracy-heuristic/desirability.hpp
--rw-rw-r--   0 user      (1002) user      (1002)     9267 2023-06-05 12:32:35.000000 lincs-0.4.0/lincs/liblincs/learning/weights-profiles-breed-mrsort/improve-profiles/accuracy-heuristic-on-cpu.cpp
--rw-rw-r--   0 user      (1002) user      (1002)     1577 2023-06-05 12:32:35.000000 lincs-0.4.0/lincs/liblincs/learning/weights-profiles-breed-mrsort/improve-profiles/accuracy-heuristic-on-cpu.hpp
--rw-rw-r--   0 user      (1002) user      (1002)    14338 2023-06-08 06:59:23.000000 lincs-0.4.0/lincs/liblincs/learning/weights-profiles-breed-mrsort/improve-profiles/accuracy-heuristic-on-gpu.cu
--rw-rw-r--   0 user      (1002) user      (1002)     1817 2023-06-08 06:59:23.000000 lincs-0.4.0/lincs/liblincs/learning/weights-profiles-breed-mrsort/improve-profiles/accuracy-heuristic-on-gpu.hpp
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-06-08 08:00:09.108882 lincs-0.4.0/lincs/liblincs/learning/weights-profiles-breed-mrsort/initialize-profiles/
--rw-rw-r--   0 user      (1002) user      (1002)     4406 2023-06-05 12:32:35.000000 lincs-0.4.0/lincs/liblincs/learning/weights-profiles-breed-mrsort/initialize-profiles/probabilistic-maximal-discrimination-power-per-criterion.cpp
--rw-rw-r--   0 user      (1002) user      (1002)     1265 2023-06-05 12:32:35.000000 lincs-0.4.0/lincs/liblincs/learning/weights-profiles-breed-mrsort/initialize-profiles/probabilistic-maximal-discrimination-power-per-criterion.hpp
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-06-08 08:00:09.108882 lincs-0.4.0/lincs/liblincs/learning/weights-profiles-breed-mrsort/optimize-weights/
--rw-rw-r--   0 user      (1002) user      (1002)     3974 2023-06-08 07:34:07.000000 lincs-0.4.0/lincs/liblincs/learning/weights-profiles-breed-mrsort/optimize-weights/linear-program.cpp
--rw-rw-r--   0 user      (1002) user      (1002)      787 2023-06-08 07:34:07.000000 lincs-0.4.0/lincs/liblincs/learning/weights-profiles-breed-mrsort/optimize-weights/linear-program.hpp
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-06-08 08:00:09.108882 lincs-0.4.0/lincs/liblincs/learning/weights-profiles-breed-mrsort/terminate/
--rw-rw-r--   0 user      (1002) user      (1002)      244 2023-06-05 12:32:35.000000 lincs-0.4.0/lincs/liblincs/learning/weights-profiles-breed-mrsort/terminate/at-accuracy.cpp
--rw-rw-r--   0 user      (1002) user      (1002)      682 2023-06-05 12:32:35.000000 lincs-0.4.0/lincs/liblincs/learning/weights-profiles-breed-mrsort/terminate/at-accuracy.hpp
--rw-rw-r--   0 user      (1002) user      (1002)     6764 2023-06-08 07:34:07.000000 lincs-0.4.0/lincs/liblincs/learning/weights-profiles-breed-mrsort.cpp
--rw-rw-r--   0 user      (1002) user      (1002)     3490 2023-06-08 07:34:07.000000 lincs-0.4.0/lincs/liblincs/learning/weights-profiles-breed-mrsort.hpp
--rw-rw-r--   0 user      (1002) user      (1002)     4697 2023-06-08 07:34:07.000000 lincs-0.4.0/lincs/liblincs/learning.cpp
--rw-rw-r--   0 user      (1002) user      (1002)      968 2023-06-08 07:34:07.000000 lincs-0.4.0/lincs/liblincs/learning.hpp
--rw-rw-r--   0 user      (1002) user      (1002)    16951 2023-06-08 07:34:07.000000 lincs-0.4.0/lincs/liblincs/liblincs_module.cpp
--rw-rw-r--   0 user      (1002) user      (1002)      245 2023-06-05 12:32:35.000000 lincs-0.4.0/lincs/liblincs/lincs.hpp
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-06-08 08:00:09.112882 lincs-0.4.0/lincs/liblincs/linear-programming/
--rw-rw-r--   0 user      (1002) user      (1002)       57 2023-06-08 07:34:07.000000 lincs-0.4.0/lincs/liblincs/linear-programming/alglib.cpp
--rw-rw-r--   0 user      (1002) user      (1002)     2719 2023-06-08 07:34:07.000000 lincs-0.4.0/lincs/liblincs/linear-programming/alglib.hpp
--rw-rw-r--   0 user      (1002) user      (1002)       55 2023-06-08 06:59:23.000000 lincs-0.4.0/lincs/liblincs/linear-programming/glop.cpp
--rw-rw-r--   0 user      (1002) user      (1002)     1697 2023-06-08 06:59:23.000000 lincs-0.4.0/lincs/liblincs/linear-programming/glop.hpp
--rw-rw-r--   0 user      (1002) user      (1002)     1579 2023-06-08 07:34:21.000000 lincs-0.4.0/lincs/liblincs/linear-programming/test.cpp
--rw-rw-r--   0 user      (1002) user      (1002)     2963 2023-06-05 12:32:35.000000 lincs-0.4.0/lincs/liblincs/median-and-max.cpp
--rw-rw-r--   0 user      (1002) user      (1002)      751 2023-06-05 12:32:35.000000 lincs-0.4.0/lincs/liblincs/median-and-max.hpp
--rw-rw-r--   0 user      (1002) user      (1002)      776 2023-06-05 12:32:35.000000 lincs-0.4.0/lincs/liblincs/randomness-utils.cpp
--rw-rw-r--   0 user      (1002) user      (1002)     1736 2023-06-08 06:59:23.000000 lincs-0.4.0/lincs/liblincs/randomness-utils.hpp
--rw-rw-r--   0 user      (1002) user      (1002)    13993 2023-06-08 07:34:07.000000 lincs-0.4.0/lincs/liblincs_module_tests.py
--rw-rw-r--   0 user      (1002) user      (1002)     1403 2023-06-08 07:34:07.000000 lincs-0.4.0/lincs/visualization.py
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-06-08 08:00:09.108882 lincs-0.4.0/lincs.egg-info/
--rw-r--r--   0 user      (1002) user      (1002)     4918 2023-06-08 08:00:09.000000 lincs-0.4.0/lincs.egg-info/PKG-INFO
--rw-r--r--   0 user      (1002) user      (1002)     2438 2023-06-08 08:00:09.000000 lincs-0.4.0/lincs.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1002) user      (1002)        1 2023-06-08 08:00:09.000000 lincs-0.4.0/lincs.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1002) user      (1002)       60 2023-06-08 08:00:09.000000 lincs-0.4.0/lincs.egg-info/entry_points.txt
--rw-r--r--   0 user      (1002) user      (1002)       27 2023-06-08 08:00:09.000000 lincs-0.4.0/lincs.egg-info/requires.txt
--rw-r--r--   0 user      (1002) user      (1002)       15 2023-06-08 08:00:09.000000 lincs-0.4.0/lincs.egg-info/top_level.txt
--rw-rw-r--   0 user      (1002) user      (1002)       61 2023-06-05 12:32:35.000000 lincs-0.4.0/requirements.txt
--rw-r--r--   0 user      (1002) user      (1002)       38 2023-06-08 08:00:09.112882 lincs-0.4.0/setup.cfg
--rw-rw-r--   0 user      (1002) user      (1002)     3897 2023-06-08 07:59:54.000000 lincs-0.4.0/setup.py
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-06-09 14:13:14.047474 lincs-0.4.1/
+-rw-rw-r--   0 user      (1002) user      (1002)    35149 2023-06-05 12:32:48.000000 lincs-0.4.1/COPYING
+-rw-rw-r--   0 user      (1002) user      (1002)     7652 2023-06-05 12:32:35.000000 lincs-0.4.1/COPYING.LESSER
+-rw-rw-r--   0 user      (1002) user      (1002)      109 2023-06-05 12:32:35.000000 lincs-0.4.1/MANIFEST.in
+-rw-r--r--   0 user      (1002) user      (1002)     5184 2023-06-09 14:13:14.047474 lincs-0.4.1/PKG-INFO
+-rw-rw-r--   0 user      (1002) user      (1002)     4300 2023-06-09 14:13:09.000000 lincs-0.4.1/README.rst
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-06-09 14:13:14.043475 lincs-0.4.1/lincs/
+-rw-rw-r--   0 user      (1002) user      (1002)      995 2023-06-09 13:32:09.000000 lincs-0.4.1/lincs/__init__.py
+-rw-rw-r--   0 user      (1002) user      (1002)      170 2023-06-05 12:32:35.000000 lincs-0.4.1/lincs/__main__.py
+-rw-rw-r--   0 user      (1002) user      (1002)    22755 2023-06-09 10:24:25.000000 lincs-0.4.1/lincs/command_line_interface.py
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-06-09 14:13:14.043475 lincs-0.4.1/lincs/liblincs/
+-rw-rw-r--   0 user      (1002) user      (1002)     1627 2023-06-09 08:38:44.000000 lincs-0.4.1/lincs/liblincs/classification.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)      369 2023-06-09 08:38:44.000000 lincs-0.4.1/lincs/liblincs/classification.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)    10079 2023-06-09 08:38:44.000000 lincs-0.4.1/lincs/liblincs/generation.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)     1046 2023-06-09 08:38:44.000000 lincs-0.4.1/lincs/liblincs/generation.hpp
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-06-09 14:13:14.043475 lincs-0.4.1/lincs/liblincs/io/
+-rw-rw-r--   0 user      (1002) user      (1002)     2468 2023-06-09 08:38:44.000000 lincs-0.4.1/lincs/liblincs/io/alternatives.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)     1012 2023-06-09 08:38:44.000000 lincs-0.4.1/lincs/liblincs/io/alternatives.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)     4684 2023-06-09 13:59:35.000000 lincs-0.4.1/lincs/liblincs/io/model.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)     1687 2023-06-09 13:28:54.000000 lincs-0.4.1/lincs/liblincs/io/model.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)     4260 2023-06-09 13:59:28.000000 lincs-0.4.1/lincs/liblincs/io/problem.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)     1931 2023-06-09 13:26:35.000000 lincs-0.4.1/lincs/liblincs/io/problem.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)      983 2023-06-09 12:35:58.000000 lincs-0.4.1/lincs/liblincs/io/validation.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)      580 2023-06-09 12:31:29.000000 lincs-0.4.1/lincs/liblincs/io/validation.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)       53 2023-06-05 12:32:35.000000 lincs-0.4.1/lincs/liblincs/io.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)      187 2023-06-09 08:38:44.000000 lincs-0.4.1/lincs/liblincs/io.hpp
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-06-09 14:13:14.043475 lincs-0.4.1/lincs/liblincs/learning/
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-06-09 14:13:14.039475 lincs-0.4.1/lincs/liblincs/learning/weights-profiles-breed-mrsort/
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-06-09 14:13:14.043475 lincs-0.4.1/lincs/liblincs/learning/weights-profiles-breed-mrsort/improve-profiles/
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-06-09 14:13:14.047474 lincs-0.4.1/lincs/liblincs/learning/weights-profiles-breed-mrsort/improve-profiles/accuracy-heuristic/
+-rw-rw-r--   0 user      (1002) user      (1002)     1495 2023-06-08 06:59:23.000000 lincs-0.4.1/lincs/liblincs/learning/weights-profiles-breed-mrsort/improve-profiles/accuracy-heuristic/desirability.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)     9267 2023-06-05 12:32:35.000000 lincs-0.4.1/lincs/liblincs/learning/weights-profiles-breed-mrsort/improve-profiles/accuracy-heuristic-on-cpu.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)     1577 2023-06-05 12:32:35.000000 lincs-0.4.1/lincs/liblincs/learning/weights-profiles-breed-mrsort/improve-profiles/accuracy-heuristic-on-cpu.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)    14338 2023-06-08 06:59:23.000000 lincs-0.4.1/lincs/liblincs/learning/weights-profiles-breed-mrsort/improve-profiles/accuracy-heuristic-on-gpu.cu
+-rw-rw-r--   0 user      (1002) user      (1002)     1817 2023-06-08 06:59:23.000000 lincs-0.4.1/lincs/liblincs/learning/weights-profiles-breed-mrsort/improve-profiles/accuracy-heuristic-on-gpu.hpp
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-06-09 14:13:14.047474 lincs-0.4.1/lincs/liblincs/learning/weights-profiles-breed-mrsort/initialize-profiles/
+-rw-rw-r--   0 user      (1002) user      (1002)     4406 2023-06-05 12:32:35.000000 lincs-0.4.1/lincs/liblincs/learning/weights-profiles-breed-mrsort/initialize-profiles/probabilistic-maximal-discrimination-power-per-criterion.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)     1265 2023-06-05 12:32:35.000000 lincs-0.4.1/lincs/liblincs/learning/weights-profiles-breed-mrsort/initialize-profiles/probabilistic-maximal-discrimination-power-per-criterion.hpp
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-06-09 14:13:14.047474 lincs-0.4.1/lincs/liblincs/learning/weights-profiles-breed-mrsort/optimize-weights/
+-rw-rw-r--   0 user      (1002) user      (1002)     3974 2023-06-09 08:38:44.000000 lincs-0.4.1/lincs/liblincs/learning/weights-profiles-breed-mrsort/optimize-weights/linear-program.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)      787 2023-06-09 08:38:44.000000 lincs-0.4.1/lincs/liblincs/learning/weights-profiles-breed-mrsort/optimize-weights/linear-program.hpp
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-06-09 14:13:14.047474 lincs-0.4.1/lincs/liblincs/learning/weights-profiles-breed-mrsort/terminate/
+-rw-rw-r--   0 user      (1002) user      (1002)      244 2023-06-05 12:32:35.000000 lincs-0.4.1/lincs/liblincs/learning/weights-profiles-breed-mrsort/terminate/at-accuracy.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)      682 2023-06-05 12:32:35.000000 lincs-0.4.1/lincs/liblincs/learning/weights-profiles-breed-mrsort/terminate/at-accuracy.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)     6764 2023-06-09 08:38:44.000000 lincs-0.4.1/lincs/liblincs/learning/weights-profiles-breed-mrsort.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)     3490 2023-06-09 08:38:44.000000 lincs-0.4.1/lincs/liblincs/learning/weights-profiles-breed-mrsort.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)     4872 2023-06-09 08:40:23.000000 lincs-0.4.1/lincs/liblincs/learning.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)      968 2023-06-09 08:40:23.000000 lincs-0.4.1/lincs/liblincs/learning.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)    17094 2023-06-09 13:31:54.000000 lincs-0.4.1/lincs/liblincs/liblincs_module.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)      245 2023-06-05 12:32:35.000000 lincs-0.4.1/lincs/liblincs/lincs.hpp
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-06-09 14:13:14.047474 lincs-0.4.1/lincs/liblincs/linear-programming/
+-rw-rw-r--   0 user      (1002) user      (1002)       57 2023-06-09 08:38:44.000000 lincs-0.4.1/lincs/liblincs/linear-programming/alglib.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)     2719 2023-06-09 08:38:44.000000 lincs-0.4.1/lincs/liblincs/linear-programming/alglib.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)       55 2023-06-08 06:59:23.000000 lincs-0.4.1/lincs/liblincs/linear-programming/glop.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)     1697 2023-06-08 06:59:23.000000 lincs-0.4.1/lincs/liblincs/linear-programming/glop.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)     1579 2023-06-09 08:38:44.000000 lincs-0.4.1/lincs/liblincs/linear-programming/test.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)     2963 2023-06-05 12:32:35.000000 lincs-0.4.1/lincs/liblincs/median-and-max.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)      751 2023-06-05 12:32:35.000000 lincs-0.4.1/lincs/liblincs/median-and-max.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)      776 2023-06-05 12:32:35.000000 lincs-0.4.1/lincs/liblincs/randomness-utils.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)     1736 2023-06-08 06:59:23.000000 lincs-0.4.1/lincs/liblincs/randomness-utils.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)    14126 2023-06-09 08:40:23.000000 lincs-0.4.1/lincs/liblincs_module_tests.py
+-rw-rw-r--   0 user      (1002) user      (1002)     1403 2023-06-09 08:38:44.000000 lincs-0.4.1/lincs/visualization.py
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-06-09 14:13:14.043475 lincs-0.4.1/lincs.egg-info/
+-rw-r--r--   0 user      (1002) user      (1002)     5184 2023-06-09 14:13:14.000000 lincs-0.4.1/lincs.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1002) user      (1002)     2504 2023-06-09 14:13:14.000000 lincs-0.4.1/lincs.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1002) user      (1002)        1 2023-06-09 14:13:14.000000 lincs-0.4.1/lincs.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1002) user      (1002)       60 2023-06-09 14:13:14.000000 lincs-0.4.1/lincs.egg-info/entry_points.txt
+-rw-r--r--   0 user      (1002) user      (1002)       27 2023-06-09 14:13:14.000000 lincs-0.4.1/lincs.egg-info/requires.txt
+-rw-r--r--   0 user      (1002) user      (1002)       15 2023-06-09 14:13:14.000000 lincs-0.4.1/lincs.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1002) user      (1002)       61 2023-06-05 12:32:35.000000 lincs-0.4.1/requirements.txt
+-rw-r--r--   0 user      (1002) user      (1002)       38 2023-06-09 14:13:14.047474 lincs-0.4.1/setup.cfg
+-rw-rw-r--   0 user      (1002) user      (1002)     3897 2023-06-09 14:11:49.000000 lincs-0.4.1/setup.py
```

### Comparing `lincs-0.4.0/COPYING` & `lincs-0.4.1/COPYING`

 * *Files identical despite different names*

### Comparing `lincs-0.4.0/COPYING.LESSER` & `lincs-0.4.1/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `lincs-0.4.0/PKG-INFO` & `lincs-0.4.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lincs
-Version: 0.4.0
+Version: 0.4.1
 Summary: Learn and Infer Non Compensatory Sortings
 Home-page: https://github.com/MICS-Lab/lincs
 Author: Vincent Jacques
 Author-email: vincent@vincent-jacques.net
 License: LGPLv3
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
@@ -25,15 +25,15 @@
     - on GitHub (https://github.com/mics-lab/lincs/)
     - on PyPI after publication of the package (https://pypi.org/project/lincs/)
     - on GitHub Pages (https://mics-lab.github.io/lincs/)
     So when you change it, take care to check all those places.
 
 *lincs* (Learn and Infer Non Compensatory Sortings) is a collection of MCDA algorithms, usable as a C++ library, a Python package and a command-line utility.
 
-*lincs* is licensed under the GNU Lesser General Public License v3.0 as indicated by the two files `COPYING <https://github.com/MICS-Lab/lincs/blob/v0.4.0/COPYING>`_ and `COPYING.LESSER <https://github.com/MICS-Lab/lincs/blob/v0.4.0/COPYING.LESSER>`_.
+*lincs* is licensed under the GNU Lesser General Public License v3.0 as indicated by the two files `COPYING <https://github.com/MICS-Lab/lincs/blob/v0.4.1/COPYING>`_ and `COPYING.LESSER <https://github.com/MICS-Lab/lincs/blob/v0.4.1/COPYING.LESSER>`_.
 
 @todo (When we have a paper to actually cite) Add a note asking academics to kindly cite our work.
 
 *lincs* is available for install from the `Python package index <https://pypi.org/project/lincs/>`_.
 Its `documentation <http://mics-lab.github.io/lincs/>`_
 and its `source code <https://github.com/mics-lab/lincs/>`_ are on GitHub.
 
@@ -54,16 +54,18 @@
 
 It's based on work by:
 
 - `Olivier Sobrie <http://olivier.sobrie.be/>`_ (The "weights, profiles, breed" learning strategy for MR-Sort models, and the profiles improvement heuristic, developed in his `Ph.D thesis <http://olivier.sobrie.be/papers/phd_2016_sobrie.pdf>`_, and `implemented in Python <https://github.com/oso/pymcda>`_)
 - Emma Dixneuf, Thibault Monsel and Thomas Vindard (`C++ implementation of Sobrie's heuristic <https://github.com/Mostah/fastPL/>`_)
 
 @todo Add links to the fundamental articles for NCS.
+
 @todo Add links to the articles that define other learning methods we re-implement.
 
+
 Project goals
 =============
 
 Provide MCDA tools usable out of the box
 ----------------------------------------
 
 You should be able to use *lincs* without being a specialist of MCDA and/or NCS models.
@@ -75,14 +77,21 @@
 *lincs* is designed to be easy to extend with new algorithms of even replace parts of existing algorithms.
 See our `contributor guide <https://mics-lab.github.io/lincs/contributor-guide.html>`_ for more details.
 
 *lincs* also provides a benchmark framework to compare algorithms (@todo Implement and document).
 This should make it easier to understand the relative strengths and weaknesses of each algorithm.
 
 
+Versioning
+==========
+
+Starting with version 1.0.0, *lincs* tries to apply `semantic versioning <https://semver.org/>`_ at a *code* level:
+upgrading patch and minor releases should not require changes in client code but may require you to recompile and link it.
+
+
 Get started
 ===========
 
 Depending on your favorite approach, you can either start with our `hands-on "Get started" guide <https://mics-lab.github.io/lincs/get-started.html>`_
 or with our `conceptual overview documentation <https://mics-lab.github.io/lincs/conceptual-overview.html>`_.
 The former will show you how to use our tools, the latter will explain the concepts behind them: what's MCDA, what are NCS models, *etc.*
 If in doubt, start with the conceptual overview.
```

### Comparing `lincs-0.4.0/README.rst` & `lincs-0.4.1/README.rst`

 * *Files 22% similar despite different names*

```diff
@@ -33,16 +33,18 @@
 
 It's based on work by:
 
 - `Olivier Sobrie <http://olivier.sobrie.be/>`_ (The "weights, profiles, breed" learning strategy for MR-Sort models, and the profiles improvement heuristic, developed in his `Ph.D thesis <http://olivier.sobrie.be/papers/phd_2016_sobrie.pdf>`_, and `implemented in Python <https://github.com/oso/pymcda>`_)
 - Emma Dixneuf, Thibault Monsel and Thomas Vindard (`C++ implementation of Sobrie's heuristic <https://github.com/Mostah/fastPL/>`_)
 
 @todo Add links to the fundamental articles for NCS.
+
 @todo Add links to the articles that define other learning methods we re-implement.
 
+
 Project goals
 =============
 
 Provide MCDA tools usable out of the box
 ----------------------------------------
 
 You should be able to use *lincs* without being a specialist of MCDA and/or NCS models.
@@ -54,14 +56,21 @@
 *lincs* is designed to be easy to extend with new algorithms of even replace parts of existing algorithms.
 See our `contributor guide <https://mics-lab.github.io/lincs/contributor-guide.html>`_ for more details.
 
 *lincs* also provides a benchmark framework to compare algorithms (@todo Implement and document).
 This should make it easier to understand the relative strengths and weaknesses of each algorithm.
 
 
+Versioning
+==========
+
+Starting with version 1.0.0, *lincs* tries to apply `semantic versioning <https://semver.org/>`_ at a *code* level:
+upgrading patch and minor releases should not require changes in client code but may require you to recompile and link it.
+
+
 Get started
 ===========
 
 Depending on your favorite approach, you can either start with our `hands-on "Get started" guide <https://mics-lab.github.io/lincs/get-started.html>`_
 or with our `conceptual overview documentation <https://mics-lab.github.io/lincs/conceptual-overview.html>`_.
 The former will show you how to use our tools, the latter will explain the concepts behind them: what's MCDA, what are NCS models, *etc.*
 If in doubt, start with the conceptual overview.
```

### Comparing `lincs-0.4.0/lincs/__init__.py` & `lincs-0.4.1/lincs/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Copyright 2023 Vincent Jacques
 
-from liblincs import ValueType, CategoryCorrelation, Criterion, Category, Problem, load_problem, generate_problem
-from liblincs import SufficientCoalitionsKind, SufficientCoalitions, Boundary, Model, load_model, generate_mrsort_model
+from liblincs import ValueType, CategoryCorrelation, Criterion, Category, Problem, PROBLEM_JSON_SCHEMA, load_problem, generate_problem
+from liblincs import SufficientCoalitionsKind, SufficientCoalitions, Boundary, Model, MODEL_JSON_SCHEMA, load_model, generate_mrsort_model
 from liblincs import Alternative, Alternatives, load_alternatives, generate_alternatives, classify_alternatives
 from liblincs import ProfilesInitializationStrategy, InitializeProfilesForProbabilisticMaximalDiscriminationPowerPerCriterion
 from liblincs import WeightsOptimizationStrategy, OptimizeWeightsUsingGlop, OptimizeWeightsUsingAlglib
 from liblincs import ProfilesImprovementStrategy, ImproveProfilesWithAccuracyHeuristicOnCpu, ImproveProfilesWithAccuracyHeuristicOnGpu
 from liblincs import TerminationStrategy, TerminateAtAccuracy
 from liblincs import make_models, make_gpu_models, WeightsProfilesBreedMrSortLearning
```

### Comparing `lincs-0.4.0/lincs/command_line_interface.py` & `lincs-0.4.1/lincs/command_line_interface.py`

 * *Files 3% similar despite different names*

```diff
@@ -406,15 +406,15 @@
     ),
     {
         "ucncs": [],
         "mrsort": [
             (
                 "strategy",
                 dict(
-                    help="The top-level strategy to use to learn the MRSort model. See (@todo Add link to doc) for details about the available strategies.",
+                    help="The top-level strategy to use to learn the MRSort model. See https://mics-lab.github.io/lincs/user-guide.html#learning-strategies about strategies.",
                     type=click.Choice(["weights-profiles-breed"]),
                     default="weights-profiles-breed",
                     show_default=True,
                 ),
                 {
                     "weights-profiles-breed": [
                         (
@@ -446,48 +446,48 @@
                                 show_default=True,
                             ),
                             {},
                         ),
                         (
                             "initialization-strategy",
                             dict(
-                                help="The strategy to use to initialize the MRSort models. See (@todo Add link to doc) for details about the available strategies.",
+                                help="The strategy to use to initialize the MRSort models.",
                                 type=click.Choice(["maximize-discrimination-per-criterion"]),
                                 default="maximize-discrimination-per-criterion",
                                 show_default=True,
                             ),
                             {},
                         ),
                         (
                             "weights-strategy",
                             dict(
-                                help="The strategy to use to improve the weights of the MRSort models. See (@todo Add link to doc) for details about the available strategies.",
+                                help="The strategy to use to improve the weights of the MRSort models.",
                                 type=click.Choice(["linear-program"]),
                                 default="linear-program",
                                 show_default=True,
                             ),
                             {
                                 "linear-program": [
                                     (
                                         "solver",
                                         dict(
-                                            help="The solver to use to solve the linear programs. See (@todo Add link to doc) for details of available solvers.",
+                                            help="The solver to use to solve the linear programs.",
                                             type=click.Choice(["glop", "alglib"]),
                                             default="glop",
                                             show_default=True,
                                         ),
                                         {},
                                     ),
                                 ],
                             },
                         ),
                         (
                             "profiles-strategy",
                             dict(
-                                help="The strategy to use to improve the profiles of the MRSort models. See (@todo Add link to doc) for details about the available strategies.",
+                                help="The strategy to use to improve the profiles of the MRSort models.",
                                 type=click.Choice(["accuracy-heuristic"]),
                                 default="accuracy-heuristic",
                                 show_default=True,
                             ),
                             {
                                 "accuracy-heuristic": [
                                     (
@@ -511,15 +511,15 @@
                                     ),
                                 ],
                             },
                         ),
                         (
                             "breed-strategy",
                             dict(
-                                help="The strategy to use to breed the MRSort models. See (@todo Add link to doc) for details about the available strategies.",
+                                help="The strategy to use to breed the MRSort models.",
                                 type=click.Choice(["reinitialize-least-accurate"]),
                                 default="reinitialize-least-accurate",
                                 show_default=True,
                             ),
                             {
                                 "reinitialize-least-accurate": [
                                     (
```

### Comparing `lincs-0.4.0/lincs/liblincs/classification.cpp` & `lincs-0.4.1/lincs/liblincs/classification.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.4.0/lincs/liblincs/generation.cpp` & `lincs-0.4.1/lincs/liblincs/generation.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.4.0/lincs/liblincs/generation.hpp` & `lincs-0.4.1/lincs/liblincs/generation.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.4.0/lincs/liblincs/io/alternatives.cpp` & `lincs-0.4.1/lincs/liblincs/io/alternatives.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.4.0/lincs/liblincs/io/alternatives.hpp` & `lincs-0.4.1/lincs/liblincs/io/alternatives.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.4.0/lincs/liblincs/io/model.hpp` & `lincs-0.4.1/lincs/liblincs/io/model.hpp`

 * *Files 12% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     bool operator==(const Boundary& other) const { return profile == other.profile && sufficient_coalitions.kind == other.sufficient_coalitions.kind && sufficient_coalitions.criterion_weights == other.sufficient_coalitions.criterion_weights; }
   };
 
   std::vector<Boundary> boundaries;  // boundary_index 0 is between category_index 0 and category_index 1
 
   Model(const Problem& problem_, const std::vector<Boundary>& boundaries_) : problem(problem_), boundaries(boundaries_) {}
 
+  static const std::string json_schema;
   void dump(std::ostream&) const;
   static Model load(const Problem&, std::istream&);
-
 };
 
 }  // namespace lincs
 
 #endif  // LINCS__IO__MODEL_HPP
```

### Comparing `lincs-0.4.0/lincs/liblincs/io/problem.hpp` & `lincs-0.4.1/lincs/liblincs/io/problem.hpp`

 * *Files 6% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     bool operator==(const Category& other) const { return name == other.name; }
   };
 
   std::vector<Category> categories;
 
   Problem(const std::vector<Criterion>& criteria_, const std::vector<Category>& categories_): criteria(criteria_), categories(categories_) {}
 
+  static const std::string json_schema;
   void dump(std::ostream&) const;
   static Problem load(std::istream&);
-
 };
 
 }  // namespace lincs
 
 #endif  // LINCS__IO__PROBLEM_HPP
```

### Comparing `lincs-0.4.0/lincs/liblincs/learning/weights-profiles-breed-mrsort/improve-profiles/accuracy-heuristic/desirability.hpp` & `lincs-0.4.1/lincs/liblincs/learning/weights-profiles-breed-mrsort/improve-profiles/accuracy-heuristic/desirability.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.4.0/lincs/liblincs/learning/weights-profiles-breed-mrsort/improve-profiles/accuracy-heuristic-on-cpu.cpp` & `lincs-0.4.1/lincs/liblincs/learning/weights-profiles-breed-mrsort/improve-profiles/accuracy-heuristic-on-cpu.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.4.0/lincs/liblincs/learning/weights-profiles-breed-mrsort/improve-profiles/accuracy-heuristic-on-cpu.hpp` & `lincs-0.4.1/lincs/liblincs/learning/weights-profiles-breed-mrsort/improve-profiles/accuracy-heuristic-on-cpu.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.4.0/lincs/liblincs/learning/weights-profiles-breed-mrsort/improve-profiles/accuracy-heuristic-on-gpu.cu` & `lincs-0.4.1/lincs/liblincs/learning/weights-profiles-breed-mrsort/improve-profiles/accuracy-heuristic-on-gpu.cu`

 * *Files identical despite different names*

### Comparing `lincs-0.4.0/lincs/liblincs/learning/weights-profiles-breed-mrsort/improve-profiles/accuracy-heuristic-on-gpu.hpp` & `lincs-0.4.1/lincs/liblincs/learning/weights-profiles-breed-mrsort/improve-profiles/accuracy-heuristic-on-gpu.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.4.0/lincs/liblincs/learning/weights-profiles-breed-mrsort/initialize-profiles/probabilistic-maximal-discrimination-power-per-criterion.cpp` & `lincs-0.4.1/lincs/liblincs/learning/weights-profiles-breed-mrsort/initialize-profiles/probabilistic-maximal-discrimination-power-per-criterion.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.4.0/lincs/liblincs/learning/weights-profiles-breed-mrsort/initialize-profiles/probabilistic-maximal-discrimination-power-per-criterion.hpp` & `lincs-0.4.1/lincs/liblincs/learning/weights-profiles-breed-mrsort/initialize-profiles/probabilistic-maximal-discrimination-power-per-criterion.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.4.0/lincs/liblincs/learning/weights-profiles-breed-mrsort/optimize-weights/linear-program.cpp` & `lincs-0.4.1/lincs/liblincs/learning/weights-profiles-breed-mrsort/optimize-weights/linear-program.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.4.0/lincs/liblincs/learning/weights-profiles-breed-mrsort/optimize-weights/linear-program.hpp` & `lincs-0.4.1/lincs/liblincs/learning/weights-profiles-breed-mrsort/optimize-weights/linear-program.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.4.0/lincs/liblincs/learning/weights-profiles-breed-mrsort/terminate/at-accuracy.hpp` & `lincs-0.4.1/lincs/liblincs/learning/weights-profiles-breed-mrsort/terminate/at-accuracy.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.4.0/lincs/liblincs/learning/weights-profiles-breed-mrsort.cpp` & `lincs-0.4.1/lincs/liblincs/learning/weights-profiles-breed-mrsort.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.4.0/lincs/liblincs/learning/weights-profiles-breed-mrsort.hpp` & `lincs-0.4.1/lincs/liblincs/learning/weights-profiles-breed-mrsort.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.4.0/lincs/liblincs/learning.cpp` & `lincs-0.4.1/lincs/liblincs/learning.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,19 @@
 
 #include "classification.hpp"  // Only for tests
 #include "generation.hpp"  // Only for tests
 
 #include <doctest.h>  // Keep last because it defines really common names like CHECK that we don't want injected into other headers
 
 
+namespace {
+  const char* env = std::getenv("LINCS_DEV_FORBID_GPU");
+  const bool forbid_gpu = env && std::string(env) == "true";
+}  // namespace
+
 namespace lincs {
 
 TEST_CASE("Basic MR-Sort learning") {
   Problem problem = generate_problem(5, 3, 41);
   Model model = generate_mrsort_model(problem, 42);
   Alternatives learning_set = generate_alternatives(problem, model, 200, 43);
 
@@ -78,15 +83,15 @@
     Alternatives testing_set = generate_alternatives(problem, model, 1000, 44);
     ClassificationResult result = classify_alternatives(problem, learned_model, &testing_set);
     CHECK(result.changed == 24);
     CHECK(result.unchanged == 976);
   }
 }
 
-TEST_CASE("GPU MR-Sort learning") {
+TEST_CASE("GPU MR-Sort learning" * doctest::skip(forbid_gpu)) {
   Problem problem = generate_problem(5, 3, 41);
   Model model = generate_mrsort_model(problem, 42);
   Alternatives learning_set = generate_alternatives(problem, model, 200, 43);
 
   const unsigned random_seed = 44;
   auto host_models = WeightsProfilesBreedMrSortLearning::Models::make(
     problem, learning_set, WeightsProfilesBreedMrSortLearning::default_models_count, random_seed);
```

### Comparing `lincs-0.4.0/lincs/liblincs/learning.hpp` & `lincs-0.4.1/lincs/liblincs/learning.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.4.0/lincs/liblincs/liblincs_module.cpp` & `lincs-0.4.1/lincs/liblincs/liblincs_module.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -219,14 +219,16 @@
 
   bp::class_<std::vector<lincs::Problem::Category>>("categories_vector")
     .def(bp::vector_indexing_suite<std::vector<lincs::Problem::Category>>())
   ;
   bp::class_<std::vector<lincs::Problem::Criterion>>("criteria_vector")
     .def(bp::vector_indexing_suite<std::vector<lincs::Problem::Criterion>>())
   ;
+
+  bp::scope().attr("PROBLEM_JSON_SCHEMA") = lincs::Problem::json_schema;
   bp::class_<lincs::Problem>("Problem", bp::init<std::vector<lincs::Problem::Criterion>, std::vector<lincs::Problem::Category>>())
     .def_readwrite("criteria", &lincs::Problem::criteria)
     .def_readwrite("categories", &lincs::Problem::categories)
     .def(
       "dump",
       &dump_problem,
       (bp::arg("self"), "out"),
@@ -258,14 +260,15 @@
   bp::class_<lincs::Model::Boundary>("Boundary", bp::init<std::vector<float>, lincs::Model::SufficientCoalitions>())
     .def_readwrite("profile", &lincs::Model::Boundary::profile)
     .def_readwrite("sufficient_coalitions", &lincs::Model::Boundary::sufficient_coalitions)
   ;
   bp::class_<std::vector<lincs::Model::Boundary>>("boundaries_vector")
     .def(bp::vector_indexing_suite<std::vector<lincs::Model::Boundary>>())
   ;
+  bp::scope().attr("MODEL_JSON_SCHEMA") = lincs::Model::json_schema;
   bp::class_<lincs::Model>("Model", bp::init<const lincs::Problem&, const std::vector<lincs::Model::Boundary>&>())
     .def_readwrite("boundaries", &lincs::Model::boundaries)
     .def(
       "dump",
       &dump_model,
       (bp::arg("self"), "out"),
       "Dump the model to the provided `.write()`-supporting file-like object, in YAML format."
```

### Comparing `lincs-0.4.0/lincs/liblincs/linear-programming/alglib.hpp` & `lincs-0.4.1/lincs/liblincs/linear-programming/alglib.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.4.0/lincs/liblincs/linear-programming/glop.hpp` & `lincs-0.4.1/lincs/liblincs/linear-programming/glop.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.4.0/lincs/liblincs/linear-programming/test.cpp` & `lincs-0.4.1/lincs/liblincs/linear-programming/test.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.4.0/lincs/liblincs/median-and-max.cpp` & `lincs-0.4.1/lincs/liblincs/median-and-max.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.4.0/lincs/liblincs/median-and-max.hpp` & `lincs-0.4.1/lincs/liblincs/median-and-max.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.4.0/lincs/liblincs/randomness-utils.cpp` & `lincs-0.4.1/lincs/liblincs/randomness-utils.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.4.0/lincs/liblincs/randomness-utils.hpp` & `lincs-0.4.1/lincs/liblincs/randomness-utils.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.4.0/lincs/liblincs_module_tests.py` & `lincs-0.4.1/lincs/liblincs_module_tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 # Copyright 2023 Vincent Jacques
 
 import unittest
+import os
 
 from . import *
 
 
+forbid_gpu = os.environ.get("LINCS_DEV_FORBID_GPU", "false") == "true"
+
+
 class ProblemTestCase(unittest.TestCase):
     def test_init_empty(self):
         problem = Problem([], [])
         self.assertEqual(len(problem.criteria), 0)
         self.assertEqual(len(problem.categories), 0)
 
     def test_init_wrong_types(self):
@@ -282,14 +286,15 @@
         self.assertEqual(result.unchanged, 200)
 
         testing_set = generate_alternatives(problem, model, 1000, 44)
         result = classify_alternatives(problem, learned_model, testing_set)
         self.assertEqual(result.changed, 24)
         self.assertEqual(result.unchanged, 976)
 
+    @unittest.skipIf(forbid_gpu, "Can't use GPU")
     def test_gpu_mrsort_learning(self):
         problem = generate_problem(5, 3, 41)
         model = generate_mrsort_model(problem, 42)
         learning_set = generate_alternatives(problem, model, 200, 43)
 
         models = make_models(problem, learning_set, 9, 44)
         termination_strategy = TerminateAtAccuracy(len(learning_set.alternatives))
```

### Comparing `lincs-0.4.0/lincs/visualization.py` & `lincs-0.4.1/lincs/visualization.py`

 * *Files identical despite different names*

### Comparing `lincs-0.4.0/lincs.egg-info/PKG-INFO` & `lincs-0.4.1/lincs.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lincs
-Version: 0.4.0
+Version: 0.4.1
 Summary: Learn and Infer Non Compensatory Sortings
 Home-page: https://github.com/MICS-Lab/lincs
 Author: Vincent Jacques
 Author-email: vincent@vincent-jacques.net
 License: LGPLv3
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
@@ -25,15 +25,15 @@
     - on GitHub (https://github.com/mics-lab/lincs/)
     - on PyPI after publication of the package (https://pypi.org/project/lincs/)
     - on GitHub Pages (https://mics-lab.github.io/lincs/)
     So when you change it, take care to check all those places.
 
 *lincs* (Learn and Infer Non Compensatory Sortings) is a collection of MCDA algorithms, usable as a C++ library, a Python package and a command-line utility.
 
-*lincs* is licensed under the GNU Lesser General Public License v3.0 as indicated by the two files `COPYING <https://github.com/MICS-Lab/lincs/blob/v0.4.0/COPYING>`_ and `COPYING.LESSER <https://github.com/MICS-Lab/lincs/blob/v0.4.0/COPYING.LESSER>`_.
+*lincs* is licensed under the GNU Lesser General Public License v3.0 as indicated by the two files `COPYING <https://github.com/MICS-Lab/lincs/blob/v0.4.1/COPYING>`_ and `COPYING.LESSER <https://github.com/MICS-Lab/lincs/blob/v0.4.1/COPYING.LESSER>`_.
 
 @todo (When we have a paper to actually cite) Add a note asking academics to kindly cite our work.
 
 *lincs* is available for install from the `Python package index <https://pypi.org/project/lincs/>`_.
 Its `documentation <http://mics-lab.github.io/lincs/>`_
 and its `source code <https://github.com/mics-lab/lincs/>`_ are on GitHub.
 
@@ -54,16 +54,18 @@
 
 It's based on work by:
 
 - `Olivier Sobrie <http://olivier.sobrie.be/>`_ (The "weights, profiles, breed" learning strategy for MR-Sort models, and the profiles improvement heuristic, developed in his `Ph.D thesis <http://olivier.sobrie.be/papers/phd_2016_sobrie.pdf>`_, and `implemented in Python <https://github.com/oso/pymcda>`_)
 - Emma Dixneuf, Thibault Monsel and Thomas Vindard (`C++ implementation of Sobrie's heuristic <https://github.com/Mostah/fastPL/>`_)
 
 @todo Add links to the fundamental articles for NCS.
+
 @todo Add links to the articles that define other learning methods we re-implement.
 
+
 Project goals
 =============
 
 Provide MCDA tools usable out of the box
 ----------------------------------------
 
 You should be able to use *lincs* without being a specialist of MCDA and/or NCS models.
@@ -75,14 +77,21 @@
 *lincs* is designed to be easy to extend with new algorithms of even replace parts of existing algorithms.
 See our `contributor guide <https://mics-lab.github.io/lincs/contributor-guide.html>`_ for more details.
 
 *lincs* also provides a benchmark framework to compare algorithms (@todo Implement and document).
 This should make it easier to understand the relative strengths and weaknesses of each algorithm.
 
 
+Versioning
+==========
+
+Starting with version 1.0.0, *lincs* tries to apply `semantic versioning <https://semver.org/>`_ at a *code* level:
+upgrading patch and minor releases should not require changes in client code but may require you to recompile and link it.
+
+
 Get started
 ===========
 
 Depending on your favorite approach, you can either start with our `hands-on "Get started" guide <https://mics-lab.github.io/lincs/get-started.html>`_
 or with our `conceptual overview documentation <https://mics-lab.github.io/lincs/conceptual-overview.html>`_.
 The former will show you how to use our tools, the latter will explain the concepts behind them: what's MCDA, what are NCS models, *etc.*
 If in doubt, start with the conceptual overview.
```

### Comparing `lincs-0.4.0/lincs.egg-info/SOURCES.txt` & `lincs-0.4.1/lincs.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -31,14 +31,16 @@
 lincs/liblincs/randomness-utils.hpp
 lincs/liblincs/io/alternatives.cpp
 lincs/liblincs/io/alternatives.hpp
 lincs/liblincs/io/model.cpp
 lincs/liblincs/io/model.hpp
 lincs/liblincs/io/problem.cpp
 lincs/liblincs/io/problem.hpp
+lincs/liblincs/io/validation.cpp
+lincs/liblincs/io/validation.hpp
 lincs/liblincs/learning/weights-profiles-breed-mrsort.cpp
 lincs/liblincs/learning/weights-profiles-breed-mrsort.hpp
 lincs/liblincs/learning/weights-profiles-breed-mrsort/improve-profiles/accuracy-heuristic-on-cpu.cpp
 lincs/liblincs/learning/weights-profiles-breed-mrsort/improve-profiles/accuracy-heuristic-on-cpu.hpp
 lincs/liblincs/learning/weights-profiles-breed-mrsort/improve-profiles/accuracy-heuristic-on-gpu.cu
 lincs/liblincs/learning/weights-profiles-breed-mrsort/improve-profiles/accuracy-heuristic-on-gpu.hpp
 lincs/liblincs/learning/weights-profiles-breed-mrsort/improve-profiles/accuracy-heuristic/desirability.hpp
```

### Comparing `lincs-0.4.0/setup.py` & `lincs-0.4.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import glob
 import os
 import setuptools
 import setuptools.command.build_ext
 
 
-version = "0.4.0"
+version = "0.4.1"
 
 with open("README.rst") as f:
     long_description = f.read()
 for file in ["COPYING", "COPYING.LESSER"]:
     long_description = long_description.replace(f" <{file}>`_", f" <https://github.com/MICS-Lab/lincs/blob/v{version}/{file}>`_")
 for lang in ["yaml", "shell", "text", "diff"]:
     long_description = long_description.replace(f".. highlight:: {lang}", "")
```

