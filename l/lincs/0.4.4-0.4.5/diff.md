# Comparing `tmp/lincs-0.4.4.tar.gz` & `tmp/lincs-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lincs-0.4.4.tar", last modified: Fri Jun  9 14:31:08 2023, max compression
+gzip compressed data, was "lincs-0.4.5.tar", last modified: Fri Jun  9 14:38:00 2023, max compression
```

## Comparing `lincs-0.4.4.tar` & `lincs-0.4.5.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-06-09 14:31:08.248567 lincs-0.4.4/
--rw-rw-r--   0 user      (1002) user      (1002)    35149 2023-06-05 12:32:48.000000 lincs-0.4.4/COPYING
--rw-rw-r--   0 user      (1002) user      (1002)     7652 2023-06-05 12:32:35.000000 lincs-0.4.4/COPYING.LESSER
--rw-rw-r--   0 user      (1002) user      (1002)      109 2023-06-05 12:32:35.000000 lincs-0.4.4/MANIFEST.in
--rw-r--r--   0 user      (1002) user      (1002)     5184 2023-06-09 14:31:08.248567 lincs-0.4.4/PKG-INFO
--rw-rw-r--   0 user      (1002) user      (1002)     4300 2023-06-09 14:31:03.000000 lincs-0.4.4/README.rst
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-06-09 14:31:08.244567 lincs-0.4.4/lincs/
--rw-rw-r--   0 user      (1002) user      (1002)      995 2023-06-09 13:32:09.000000 lincs-0.4.4/lincs/__init__.py
--rw-rw-r--   0 user      (1002) user      (1002)      170 2023-06-05 12:32:35.000000 lincs-0.4.4/lincs/__main__.py
--rw-rw-r--   0 user      (1002) user      (1002)    22755 2023-06-09 10:24:25.000000 lincs-0.4.4/lincs/command_line_interface.py
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-06-09 14:31:08.248567 lincs-0.4.4/lincs/liblincs/
--rw-rw-r--   0 user      (1002) user      (1002)     1627 2023-06-09 08:38:44.000000 lincs-0.4.4/lincs/liblincs/classification.cpp
--rw-rw-r--   0 user      (1002) user      (1002)      369 2023-06-09 08:38:44.000000 lincs-0.4.4/lincs/liblincs/classification.hpp
--rw-rw-r--   0 user      (1002) user      (1002)    10079 2023-06-09 08:38:44.000000 lincs-0.4.4/lincs/liblincs/generation.cpp
--rw-rw-r--   0 user      (1002) user      (1002)     1046 2023-06-09 08:38:44.000000 lincs-0.4.4/lincs/liblincs/generation.hpp
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-06-09 14:31:08.248567 lincs-0.4.4/lincs/liblincs/io/
--rw-rw-r--   0 user      (1002) user      (1002)     2468 2023-06-09 08:38:44.000000 lincs-0.4.4/lincs/liblincs/io/alternatives.cpp
--rw-rw-r--   0 user      (1002) user      (1002)     1012 2023-06-09 08:38:44.000000 lincs-0.4.4/lincs/liblincs/io/alternatives.hpp
--rw-rw-r--   0 user      (1002) user      (1002)     4684 2023-06-09 13:59:35.000000 lincs-0.4.4/lincs/liblincs/io/model.cpp
--rw-rw-r--   0 user      (1002) user      (1002)     1687 2023-06-09 13:28:54.000000 lincs-0.4.4/lincs/liblincs/io/model.hpp
--rw-rw-r--   0 user      (1002) user      (1002)     4260 2023-06-09 13:59:28.000000 lincs-0.4.4/lincs/liblincs/io/problem.cpp
--rw-rw-r--   0 user      (1002) user      (1002)     1931 2023-06-09 13:26:35.000000 lincs-0.4.4/lincs/liblincs/io/problem.hpp
--rw-rw-r--   0 user      (1002) user      (1002)      983 2023-06-09 12:35:58.000000 lincs-0.4.4/lincs/liblincs/io/validation.cpp
--rw-rw-r--   0 user      (1002) user      (1002)      580 2023-06-09 12:31:29.000000 lincs-0.4.4/lincs/liblincs/io/validation.hpp
--rw-rw-r--   0 user      (1002) user      (1002)       53 2023-06-05 12:32:35.000000 lincs-0.4.4/lincs/liblincs/io.cpp
--rw-rw-r--   0 user      (1002) user      (1002)      187 2023-06-09 08:38:44.000000 lincs-0.4.4/lincs/liblincs/io.hpp
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-06-09 14:31:08.248567 lincs-0.4.4/lincs/liblincs/learning/
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-06-09 14:31:08.244567 lincs-0.4.4/lincs/liblincs/learning/weights-profiles-breed-mrsort/
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-06-09 14:31:08.248567 lincs-0.4.4/lincs/liblincs/learning/weights-profiles-breed-mrsort/improve-profiles/
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-06-09 14:31:08.248567 lincs-0.4.4/lincs/liblincs/learning/weights-profiles-breed-mrsort/improve-profiles/accuracy-heuristic/
--rw-rw-r--   0 user      (1002) user      (1002)     1495 2023-06-08 06:59:23.000000 lincs-0.4.4/lincs/liblincs/learning/weights-profiles-breed-mrsort/improve-profiles/accuracy-heuristic/desirability.hpp
--rw-rw-r--   0 user      (1002) user      (1002)     9267 2023-06-05 12:32:35.000000 lincs-0.4.4/lincs/liblincs/learning/weights-profiles-breed-mrsort/improve-profiles/accuracy-heuristic-on-cpu.cpp
--rw-rw-r--   0 user      (1002) user      (1002)     1577 2023-06-05 12:32:35.000000 lincs-0.4.4/lincs/liblincs/learning/weights-profiles-breed-mrsort/improve-profiles/accuracy-heuristic-on-cpu.hpp
--rw-rw-r--   0 user      (1002) user      (1002)    14338 2023-06-08 06:59:23.000000 lincs-0.4.4/lincs/liblincs/learning/weights-profiles-breed-mrsort/improve-profiles/accuracy-heuristic-on-gpu.cu
--rw-rw-r--   0 user      (1002) user      (1002)     1817 2023-06-08 06:59:23.000000 lincs-0.4.4/lincs/liblincs/learning/weights-profiles-breed-mrsort/improve-profiles/accuracy-heuristic-on-gpu.hpp
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-06-09 14:31:08.248567 lincs-0.4.4/lincs/liblincs/learning/weights-profiles-breed-mrsort/initialize-profiles/
--rw-rw-r--   0 user      (1002) user      (1002)     4406 2023-06-05 12:32:35.000000 lincs-0.4.4/lincs/liblincs/learning/weights-profiles-breed-mrsort/initialize-profiles/probabilistic-maximal-discrimination-power-per-criterion.cpp
--rw-rw-r--   0 user      (1002) user      (1002)     1265 2023-06-05 12:32:35.000000 lincs-0.4.4/lincs/liblincs/learning/weights-profiles-breed-mrsort/initialize-profiles/probabilistic-maximal-discrimination-power-per-criterion.hpp
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-06-09 14:31:08.248567 lincs-0.4.4/lincs/liblincs/learning/weights-profiles-breed-mrsort/optimize-weights/
--rw-rw-r--   0 user      (1002) user      (1002)     3974 2023-06-09 08:38:44.000000 lincs-0.4.4/lincs/liblincs/learning/weights-profiles-breed-mrsort/optimize-weights/linear-program.cpp
--rw-rw-r--   0 user      (1002) user      (1002)      787 2023-06-09 08:38:44.000000 lincs-0.4.4/lincs/liblincs/learning/weights-profiles-breed-mrsort/optimize-weights/linear-program.hpp
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-06-09 14:31:08.248567 lincs-0.4.4/lincs/liblincs/learning/weights-profiles-breed-mrsort/terminate/
--rw-rw-r--   0 user      (1002) user      (1002)      244 2023-06-05 12:32:35.000000 lincs-0.4.4/lincs/liblincs/learning/weights-profiles-breed-mrsort/terminate/at-accuracy.cpp
--rw-rw-r--   0 user      (1002) user      (1002)      682 2023-06-05 12:32:35.000000 lincs-0.4.4/lincs/liblincs/learning/weights-profiles-breed-mrsort/terminate/at-accuracy.hpp
--rw-rw-r--   0 user      (1002) user      (1002)     6764 2023-06-09 08:38:44.000000 lincs-0.4.4/lincs/liblincs/learning/weights-profiles-breed-mrsort.cpp
--rw-rw-r--   0 user      (1002) user      (1002)     3490 2023-06-09 08:38:44.000000 lincs-0.4.4/lincs/liblincs/learning/weights-profiles-breed-mrsort.hpp
--rw-rw-r--   0 user      (1002) user      (1002)     4872 2023-06-09 08:40:23.000000 lincs-0.4.4/lincs/liblincs/learning.cpp
--rw-rw-r--   0 user      (1002) user      (1002)      968 2023-06-09 08:40:23.000000 lincs-0.4.4/lincs/liblincs/learning.hpp
--rw-rw-r--   0 user      (1002) user      (1002)    17094 2023-06-09 13:31:54.000000 lincs-0.4.4/lincs/liblincs/liblincs_module.cpp
--rw-rw-r--   0 user      (1002) user      (1002)      245 2023-06-05 12:32:35.000000 lincs-0.4.4/lincs/liblincs/lincs.hpp
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-06-09 14:31:08.248567 lincs-0.4.4/lincs/liblincs/linear-programming/
--rw-rw-r--   0 user      (1002) user      (1002)       57 2023-06-09 08:38:44.000000 lincs-0.4.4/lincs/liblincs/linear-programming/alglib.cpp
--rw-rw-r--   0 user      (1002) user      (1002)     2719 2023-06-09 08:38:44.000000 lincs-0.4.4/lincs/liblincs/linear-programming/alglib.hpp
--rw-rw-r--   0 user      (1002) user      (1002)       55 2023-06-08 06:59:23.000000 lincs-0.4.4/lincs/liblincs/linear-programming/glop.cpp
--rw-rw-r--   0 user      (1002) user      (1002)     1697 2023-06-08 06:59:23.000000 lincs-0.4.4/lincs/liblincs/linear-programming/glop.hpp
--rw-rw-r--   0 user      (1002) user      (1002)     1579 2023-06-09 08:38:44.000000 lincs-0.4.4/lincs/liblincs/linear-programming/test.cpp
--rw-rw-r--   0 user      (1002) user      (1002)     2963 2023-06-05 12:32:35.000000 lincs-0.4.4/lincs/liblincs/median-and-max.cpp
--rw-rw-r--   0 user      (1002) user      (1002)      751 2023-06-05 12:32:35.000000 lincs-0.4.4/lincs/liblincs/median-and-max.hpp
--rw-rw-r--   0 user      (1002) user      (1002)      776 2023-06-05 12:32:35.000000 lincs-0.4.4/lincs/liblincs/randomness-utils.cpp
--rw-rw-r--   0 user      (1002) user      (1002)     1736 2023-06-08 06:59:23.000000 lincs-0.4.4/lincs/liblincs/randomness-utils.hpp
--rw-rw-r--   0 user      (1002) user      (1002)    14126 2023-06-09 08:40:23.000000 lincs-0.4.4/lincs/liblincs_module_tests.py
--rw-rw-r--   0 user      (1002) user      (1002)     1403 2023-06-09 08:38:44.000000 lincs-0.4.4/lincs/visualization.py
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-06-09 14:31:08.244567 lincs-0.4.4/lincs.egg-info/
--rw-r--r--   0 user      (1002) user      (1002)     5184 2023-06-09 14:31:08.000000 lincs-0.4.4/lincs.egg-info/PKG-INFO
--rw-r--r--   0 user      (1002) user      (1002)     2504 2023-06-09 14:31:08.000000 lincs-0.4.4/lincs.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1002) user      (1002)        1 2023-06-09 14:31:08.000000 lincs-0.4.4/lincs.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1002) user      (1002)       60 2023-06-09 14:31:08.000000 lincs-0.4.4/lincs.egg-info/entry_points.txt
--rw-r--r--   0 user      (1002) user      (1002)       27 2023-06-09 14:31:08.000000 lincs-0.4.4/lincs.egg-info/requires.txt
--rw-r--r--   0 user      (1002) user      (1002)       15 2023-06-09 14:31:08.000000 lincs-0.4.4/lincs.egg-info/top_level.txt
--rw-rw-r--   0 user      (1002) user      (1002)       61 2023-06-05 12:32:35.000000 lincs-0.4.4/requirements.txt
--rw-r--r--   0 user      (1002) user      (1002)       38 2023-06-09 14:31:08.248567 lincs-0.4.4/setup.cfg
--rw-rw-r--   0 user      (1002) user      (1002)     3897 2023-06-09 14:30:37.000000 lincs-0.4.4/setup.py
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-06-09 14:38:00.511468 lincs-0.4.5/
+-rw-rw-r--   0 user      (1002) user      (1002)    35149 2023-06-05 12:32:48.000000 lincs-0.4.5/COPYING
+-rw-rw-r--   0 user      (1002) user      (1002)     7652 2023-06-05 12:32:35.000000 lincs-0.4.5/COPYING.LESSER
+-rw-rw-r--   0 user      (1002) user      (1002)      109 2023-06-05 12:32:35.000000 lincs-0.4.5/MANIFEST.in
+-rw-r--r--   0 user      (1002) user      (1002)     5184 2023-06-09 14:38:00.511468 lincs-0.4.5/PKG-INFO
+-rw-rw-r--   0 user      (1002) user      (1002)     4300 2023-06-09 14:37:55.000000 lincs-0.4.5/README.rst
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-06-09 14:38:00.507468 lincs-0.4.5/lincs/
+-rw-rw-r--   0 user      (1002) user      (1002)      995 2023-06-09 13:32:09.000000 lincs-0.4.5/lincs/__init__.py
+-rw-rw-r--   0 user      (1002) user      (1002)      170 2023-06-05 12:32:35.000000 lincs-0.4.5/lincs/__main__.py
+-rw-rw-r--   0 user      (1002) user      (1002)    22755 2023-06-09 10:24:25.000000 lincs-0.4.5/lincs/command_line_interface.py
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-06-09 14:38:00.507468 lincs-0.4.5/lincs/liblincs/
+-rw-rw-r--   0 user      (1002) user      (1002)     1627 2023-06-09 08:38:44.000000 lincs-0.4.5/lincs/liblincs/classification.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)      369 2023-06-09 08:38:44.000000 lincs-0.4.5/lincs/liblincs/classification.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)    10079 2023-06-09 08:38:44.000000 lincs-0.4.5/lincs/liblincs/generation.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)     1046 2023-06-09 08:38:44.000000 lincs-0.4.5/lincs/liblincs/generation.hpp
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-06-09 14:38:00.511468 lincs-0.4.5/lincs/liblincs/io/
+-rw-rw-r--   0 user      (1002) user      (1002)     2468 2023-06-09 08:38:44.000000 lincs-0.4.5/lincs/liblincs/io/alternatives.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)     1012 2023-06-09 08:38:44.000000 lincs-0.4.5/lincs/liblincs/io/alternatives.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)     4684 2023-06-09 13:59:35.000000 lincs-0.4.5/lincs/liblincs/io/model.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)     1687 2023-06-09 13:28:54.000000 lincs-0.4.5/lincs/liblincs/io/model.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)     4260 2023-06-09 13:59:28.000000 lincs-0.4.5/lincs/liblincs/io/problem.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)     1931 2023-06-09 13:26:35.000000 lincs-0.4.5/lincs/liblincs/io/problem.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)      983 2023-06-09 12:35:58.000000 lincs-0.4.5/lincs/liblincs/io/validation.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)      580 2023-06-09 12:31:29.000000 lincs-0.4.5/lincs/liblincs/io/validation.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)       53 2023-06-05 12:32:35.000000 lincs-0.4.5/lincs/liblincs/io.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)      187 2023-06-09 08:38:44.000000 lincs-0.4.5/lincs/liblincs/io.hpp
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-06-09 14:38:00.511468 lincs-0.4.5/lincs/liblincs/learning/
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-06-09 14:38:00.507468 lincs-0.4.5/lincs/liblincs/learning/weights-profiles-breed-mrsort/
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-06-09 14:38:00.511468 lincs-0.4.5/lincs/liblincs/learning/weights-profiles-breed-mrsort/improve-profiles/
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-06-09 14:38:00.511468 lincs-0.4.5/lincs/liblincs/learning/weights-profiles-breed-mrsort/improve-profiles/accuracy-heuristic/
+-rw-rw-r--   0 user      (1002) user      (1002)     1495 2023-06-08 06:59:23.000000 lincs-0.4.5/lincs/liblincs/learning/weights-profiles-breed-mrsort/improve-profiles/accuracy-heuristic/desirability.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)     9267 2023-06-05 12:32:35.000000 lincs-0.4.5/lincs/liblincs/learning/weights-profiles-breed-mrsort/improve-profiles/accuracy-heuristic-on-cpu.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)     1577 2023-06-05 12:32:35.000000 lincs-0.4.5/lincs/liblincs/learning/weights-profiles-breed-mrsort/improve-profiles/accuracy-heuristic-on-cpu.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)    14338 2023-06-08 06:59:23.000000 lincs-0.4.5/lincs/liblincs/learning/weights-profiles-breed-mrsort/improve-profiles/accuracy-heuristic-on-gpu.cu
+-rw-rw-r--   0 user      (1002) user      (1002)     1817 2023-06-08 06:59:23.000000 lincs-0.4.5/lincs/liblincs/learning/weights-profiles-breed-mrsort/improve-profiles/accuracy-heuristic-on-gpu.hpp
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-06-09 14:38:00.511468 lincs-0.4.5/lincs/liblincs/learning/weights-profiles-breed-mrsort/initialize-profiles/
+-rw-rw-r--   0 user      (1002) user      (1002)     4406 2023-06-05 12:32:35.000000 lincs-0.4.5/lincs/liblincs/learning/weights-profiles-breed-mrsort/initialize-profiles/probabilistic-maximal-discrimination-power-per-criterion.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)     1265 2023-06-05 12:32:35.000000 lincs-0.4.5/lincs/liblincs/learning/weights-profiles-breed-mrsort/initialize-profiles/probabilistic-maximal-discrimination-power-per-criterion.hpp
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-06-09 14:38:00.511468 lincs-0.4.5/lincs/liblincs/learning/weights-profiles-breed-mrsort/optimize-weights/
+-rw-rw-r--   0 user      (1002) user      (1002)     3974 2023-06-09 08:38:44.000000 lincs-0.4.5/lincs/liblincs/learning/weights-profiles-breed-mrsort/optimize-weights/linear-program.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)      787 2023-06-09 08:38:44.000000 lincs-0.4.5/lincs/liblincs/learning/weights-profiles-breed-mrsort/optimize-weights/linear-program.hpp
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-06-09 14:38:00.511468 lincs-0.4.5/lincs/liblincs/learning/weights-profiles-breed-mrsort/terminate/
+-rw-rw-r--   0 user      (1002) user      (1002)      244 2023-06-05 12:32:35.000000 lincs-0.4.5/lincs/liblincs/learning/weights-profiles-breed-mrsort/terminate/at-accuracy.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)      682 2023-06-05 12:32:35.000000 lincs-0.4.5/lincs/liblincs/learning/weights-profiles-breed-mrsort/terminate/at-accuracy.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)     6764 2023-06-09 08:38:44.000000 lincs-0.4.5/lincs/liblincs/learning/weights-profiles-breed-mrsort.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)     3490 2023-06-09 08:38:44.000000 lincs-0.4.5/lincs/liblincs/learning/weights-profiles-breed-mrsort.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)     4872 2023-06-09 08:40:23.000000 lincs-0.4.5/lincs/liblincs/learning.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)      968 2023-06-09 08:40:23.000000 lincs-0.4.5/lincs/liblincs/learning.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)    17094 2023-06-09 13:31:54.000000 lincs-0.4.5/lincs/liblincs/liblincs_module.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)      245 2023-06-05 12:32:35.000000 lincs-0.4.5/lincs/liblincs/lincs.hpp
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-06-09 14:38:00.511468 lincs-0.4.5/lincs/liblincs/linear-programming/
+-rw-rw-r--   0 user      (1002) user      (1002)       57 2023-06-09 08:38:44.000000 lincs-0.4.5/lincs/liblincs/linear-programming/alglib.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)     2719 2023-06-09 08:38:44.000000 lincs-0.4.5/lincs/liblincs/linear-programming/alglib.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)       55 2023-06-08 06:59:23.000000 lincs-0.4.5/lincs/liblincs/linear-programming/glop.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)     1697 2023-06-08 06:59:23.000000 lincs-0.4.5/lincs/liblincs/linear-programming/glop.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)     1579 2023-06-09 08:38:44.000000 lincs-0.4.5/lincs/liblincs/linear-programming/test.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)     2963 2023-06-05 12:32:35.000000 lincs-0.4.5/lincs/liblincs/median-and-max.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)      751 2023-06-05 12:32:35.000000 lincs-0.4.5/lincs/liblincs/median-and-max.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)      776 2023-06-05 12:32:35.000000 lincs-0.4.5/lincs/liblincs/randomness-utils.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)     1736 2023-06-08 06:59:23.000000 lincs-0.4.5/lincs/liblincs/randomness-utils.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)    14126 2023-06-09 08:40:23.000000 lincs-0.4.5/lincs/liblincs_module_tests.py
+-rw-rw-r--   0 user      (1002) user      (1002)     1403 2023-06-09 08:38:44.000000 lincs-0.4.5/lincs/visualization.py
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-06-09 14:38:00.507468 lincs-0.4.5/lincs.egg-info/
+-rw-r--r--   0 user      (1002) user      (1002)     5184 2023-06-09 14:38:00.000000 lincs-0.4.5/lincs.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1002) user      (1002)     2504 2023-06-09 14:38:00.000000 lincs-0.4.5/lincs.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1002) user      (1002)        1 2023-06-09 14:38:00.000000 lincs-0.4.5/lincs.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1002) user      (1002)       60 2023-06-09 14:38:00.000000 lincs-0.4.5/lincs.egg-info/entry_points.txt
+-rw-r--r--   0 user      (1002) user      (1002)       27 2023-06-09 14:38:00.000000 lincs-0.4.5/lincs.egg-info/requires.txt
+-rw-r--r--   0 user      (1002) user      (1002)       15 2023-06-09 14:38:00.000000 lincs-0.4.5/lincs.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1002) user      (1002)       61 2023-06-05 12:32:35.000000 lincs-0.4.5/requirements.txt
+-rw-r--r--   0 user      (1002) user      (1002)       38 2023-06-09 14:38:00.511468 lincs-0.4.5/setup.cfg
+-rw-rw-r--   0 user      (1002) user      (1002)     3897 2023-06-09 14:37:30.000000 lincs-0.4.5/setup.py
```

### Comparing `lincs-0.4.4/COPYING` & `lincs-0.4.5/COPYING`

 * *Files identical despite different names*

### Comparing `lincs-0.4.4/COPYING.LESSER` & `lincs-0.4.5/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `lincs-0.4.4/PKG-INFO` & `lincs-0.4.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lincs
-Version: 0.4.4
+Version: 0.4.5
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
 
-*lincs* is licensed under the GNU Lesser General Public License v3.0 as indicated by the two files `COPYING <https://github.com/MICS-Lab/lincs/blob/v0.4.4/COPYING>`_ and `COPYING.LESSER <https://github.com/MICS-Lab/lincs/blob/v0.4.4/COPYING.LESSER>`_.
+*lincs* is licensed under the GNU Lesser General Public License v3.0 as indicated by the two files `COPYING <https://github.com/MICS-Lab/lincs/blob/v0.4.5/COPYING>`_ and `COPYING.LESSER <https://github.com/MICS-Lab/lincs/blob/v0.4.5/COPYING.LESSER>`_.
 
 @todo (When we have a paper to actually cite) Add a note asking academics to kindly cite our work.
 
 *lincs* is available for install from the `Python package index <https://pypi.org/project/lincs/>`_.
 Its `documentation <http://mics-lab.github.io/lincs/>`_
 and its `source code <https://github.com/mics-lab/lincs/>`_ are on GitHub.
```

### Comparing `lincs-0.4.4/README.rst` & `lincs-0.4.5/README.rst`

 * *Files identical despite different names*

### Comparing `lincs-0.4.4/lincs/__init__.py` & `lincs-0.4.5/lincs/__init__.py`

 * *Files identical despite different names*

### Comparing `lincs-0.4.4/lincs/command_line_interface.py` & `lincs-0.4.5/lincs/command_line_interface.py`

 * *Files identical despite different names*

### Comparing `lincs-0.4.4/lincs/liblincs/classification.cpp` & `lincs-0.4.5/lincs/liblincs/classification.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.4.4/lincs/liblincs/generation.cpp` & `lincs-0.4.5/lincs/liblincs/generation.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.4.4/lincs/liblincs/generation.hpp` & `lincs-0.4.5/lincs/liblincs/generation.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.4.4/lincs/liblincs/io/alternatives.cpp` & `lincs-0.4.5/lincs/liblincs/io/alternatives.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.4.4/lincs/liblincs/io/alternatives.hpp` & `lincs-0.4.5/lincs/liblincs/io/alternatives.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.4.4/lincs/liblincs/io/model.cpp` & `lincs-0.4.5/lincs/liblincs/io/model.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.4.4/lincs/liblincs/io/model.hpp` & `lincs-0.4.5/lincs/liblincs/io/model.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.4.4/lincs/liblincs/io/problem.cpp` & `lincs-0.4.5/lincs/liblincs/io/problem.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.4.4/lincs/liblincs/io/problem.hpp` & `lincs-0.4.5/lincs/liblincs/io/problem.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.4.4/lincs/liblincs/io/validation.cpp` & `lincs-0.4.5/lincs/liblincs/io/validation.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.4.4/lincs/liblincs/io/validation.hpp` & `lincs-0.4.5/lincs/liblincs/io/validation.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.4.4/lincs/liblincs/learning/weights-profiles-breed-mrsort/improve-profiles/accuracy-heuristic/desirability.hpp` & `lincs-0.4.5/lincs/liblincs/learning/weights-profiles-breed-mrsort/improve-profiles/accuracy-heuristic/desirability.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.4.4/lincs/liblincs/learning/weights-profiles-breed-mrsort/improve-profiles/accuracy-heuristic-on-cpu.cpp` & `lincs-0.4.5/lincs/liblincs/learning/weights-profiles-breed-mrsort/improve-profiles/accuracy-heuristic-on-cpu.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.4.4/lincs/liblincs/learning/weights-profiles-breed-mrsort/improve-profiles/accuracy-heuristic-on-cpu.hpp` & `lincs-0.4.5/lincs/liblincs/learning/weights-profiles-breed-mrsort/improve-profiles/accuracy-heuristic-on-cpu.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.4.4/lincs/liblincs/learning/weights-profiles-breed-mrsort/improve-profiles/accuracy-heuristic-on-gpu.cu` & `lincs-0.4.5/lincs/liblincs/learning/weights-profiles-breed-mrsort/improve-profiles/accuracy-heuristic-on-gpu.cu`

 * *Files identical despite different names*

### Comparing `lincs-0.4.4/lincs/liblincs/learning/weights-profiles-breed-mrsort/improve-profiles/accuracy-heuristic-on-gpu.hpp` & `lincs-0.4.5/lincs/liblincs/learning/weights-profiles-breed-mrsort/improve-profiles/accuracy-heuristic-on-gpu.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.4.4/lincs/liblincs/learning/weights-profiles-breed-mrsort/initialize-profiles/probabilistic-maximal-discrimination-power-per-criterion.cpp` & `lincs-0.4.5/lincs/liblincs/learning/weights-profiles-breed-mrsort/initialize-profiles/probabilistic-maximal-discrimination-power-per-criterion.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.4.4/lincs/liblincs/learning/weights-profiles-breed-mrsort/initialize-profiles/probabilistic-maximal-discrimination-power-per-criterion.hpp` & `lincs-0.4.5/lincs/liblincs/learning/weights-profiles-breed-mrsort/initialize-profiles/probabilistic-maximal-discrimination-power-per-criterion.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.4.4/lincs/liblincs/learning/weights-profiles-breed-mrsort/optimize-weights/linear-program.cpp` & `lincs-0.4.5/lincs/liblincs/learning/weights-profiles-breed-mrsort/optimize-weights/linear-program.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.4.4/lincs/liblincs/learning/weights-profiles-breed-mrsort/optimize-weights/linear-program.hpp` & `lincs-0.4.5/lincs/liblincs/learning/weights-profiles-breed-mrsort/optimize-weights/linear-program.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.4.4/lincs/liblincs/learning/weights-profiles-breed-mrsort/terminate/at-accuracy.hpp` & `lincs-0.4.5/lincs/liblincs/learning/weights-profiles-breed-mrsort/terminate/at-accuracy.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.4.4/lincs/liblincs/learning/weights-profiles-breed-mrsort.cpp` & `lincs-0.4.5/lincs/liblincs/learning/weights-profiles-breed-mrsort.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.4.4/lincs/liblincs/learning/weights-profiles-breed-mrsort.hpp` & `lincs-0.4.5/lincs/liblincs/learning/weights-profiles-breed-mrsort.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.4.4/lincs/liblincs/learning.cpp` & `lincs-0.4.5/lincs/liblincs/learning.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.4.4/lincs/liblincs/learning.hpp` & `lincs-0.4.5/lincs/liblincs/learning.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.4.4/lincs/liblincs/liblincs_module.cpp` & `lincs-0.4.5/lincs/liblincs/liblincs_module.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.4.4/lincs/liblincs/linear-programming/alglib.hpp` & `lincs-0.4.5/lincs/liblincs/linear-programming/alglib.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.4.4/lincs/liblincs/linear-programming/glop.hpp` & `lincs-0.4.5/lincs/liblincs/linear-programming/glop.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.4.4/lincs/liblincs/linear-programming/test.cpp` & `lincs-0.4.5/lincs/liblincs/linear-programming/test.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.4.4/lincs/liblincs/median-and-max.cpp` & `lincs-0.4.5/lincs/liblincs/median-and-max.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.4.4/lincs/liblincs/median-and-max.hpp` & `lincs-0.4.5/lincs/liblincs/median-and-max.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.4.4/lincs/liblincs/randomness-utils.cpp` & `lincs-0.4.5/lincs/liblincs/randomness-utils.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.4.4/lincs/liblincs/randomness-utils.hpp` & `lincs-0.4.5/lincs/liblincs/randomness-utils.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.4.4/lincs/liblincs_module_tests.py` & `lincs-0.4.5/lincs/liblincs_module_tests.py`

 * *Files identical despite different names*

### Comparing `lincs-0.4.4/lincs/visualization.py` & `lincs-0.4.5/lincs/visualization.py`

 * *Files identical despite different names*

### Comparing `lincs-0.4.4/lincs.egg-info/PKG-INFO` & `lincs-0.4.5/lincs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lincs
-Version: 0.4.4
+Version: 0.4.5
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
 
-*lincs* is licensed under the GNU Lesser General Public License v3.0 as indicated by the two files `COPYING <https://github.com/MICS-Lab/lincs/blob/v0.4.4/COPYING>`_ and `COPYING.LESSER <https://github.com/MICS-Lab/lincs/blob/v0.4.4/COPYING.LESSER>`_.
+*lincs* is licensed under the GNU Lesser General Public License v3.0 as indicated by the two files `COPYING <https://github.com/MICS-Lab/lincs/blob/v0.4.5/COPYING>`_ and `COPYING.LESSER <https://github.com/MICS-Lab/lincs/blob/v0.4.5/COPYING.LESSER>`_.
 
 @todo (When we have a paper to actually cite) Add a note asking academics to kindly cite our work.
 
 *lincs* is available for install from the `Python package index <https://pypi.org/project/lincs/>`_.
 Its `documentation <http://mics-lab.github.io/lincs/>`_
 and its `source code <https://github.com/mics-lab/lincs/>`_ are on GitHub.
```

### Comparing `lincs-0.4.4/lincs.egg-info/SOURCES.txt` & `lincs-0.4.5/lincs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lincs-0.4.4/setup.py` & `lincs-0.4.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import glob
 import os
 import setuptools
 import setuptools.command.build_ext
 
 
-version = "0.4.4"
+version = "0.4.5"
 
 with open("README.rst") as f:
     long_description = f.read()
 for file in ["COPYING", "COPYING.LESSER"]:
     long_description = long_description.replace(f" <{file}>`_", f" <https://github.com/MICS-Lab/lincs/blob/v{version}/{file}>`_")
 for lang in ["yaml", "shell", "text", "diff"]:
     long_description = long_description.replace(f".. highlight:: {lang}", "")
```

