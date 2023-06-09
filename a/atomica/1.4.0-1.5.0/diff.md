# Comparing `tmp/atomica-1.4.0.tar.gz` & `tmp/atomica-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/atomica-1.4.0.tar", last modified: Wed May 15 02:12:33 2019, max compression
+gzip compressed data, was "dist/atomica-1.5.0.tar", last modified: Fri Jun  7 12:55:07 2019, max compression
```

## Comparing `atomica-1.4.0.tar` & `atomica-1.5.0.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-05-15 02:12:33.000000 atomica-1.4.0/
--rw-rw-r--   0 travis    (2000) travis    (2000)    35141 2019-05-15 02:12:18.000000 atomica-1.4.0/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)      116 2019-05-15 02:12:18.000000 atomica-1.4.0/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)     5820 2019-05-15 02:12:33.000000 atomica-1.4.0/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     4271 2019-05-15 02:12:18.000000 atomica-1.4.0/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-05-15 02:12:33.000000 atomica-1.4.0/atomica/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3155 2019-05-15 02:12:18.000000 atomica-1.4.0/atomica/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8203 2019-05-15 02:12:18.000000 atomica-1.4.0/atomica/calibration.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    43692 2019-05-15 02:12:18.000000 atomica-1.4.0/atomica/cascade.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    47650 2019-05-15 02:12:18.000000 atomica-1.4.0/atomica/data.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4795 2019-05-15 02:12:18.000000 atomica-1.4.0/atomica/defaults.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    50581 2019-05-15 02:12:18.000000 atomica-1.4.0/atomica/excel.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    65103 2019-05-15 02:12:18.000000 atomica-1.4.0/atomica/framework.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3229 2019-05-15 02:12:18.000000 atomica-1.4.0/atomica/function_parser.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-05-15 02:12:33.000000 atomica-1.4.0/atomica/library/
--rw-rw-r--   0 travis    (2000) travis    (2000)    14399 2019-05-15 02:12:18.000000 atomica-1.4.0/atomica/library/cervicalcancer_databook.xlsx
--rw-rw-r--   0 travis    (2000) travis    (2000)    30789 2019-05-15 02:12:18.000000 atomica-1.4.0/atomica/library/cervicalcancer_framework.xlsx
--rw-rw-r--   0 travis    (2000) travis    (2000)    11141 2019-05-15 02:12:18.000000 atomica-1.4.0/atomica/library/cervicalcancer_progbook.xlsx
--rw-rw-r--   0 travis    (2000) travis    (2000)    26731 2019-05-15 02:12:18.000000 atomica-1.4.0/atomica/library/combined_databook.xlsx
--rw-rw-r--   0 travis    (2000) travis    (2000)    41519 2019-05-15 02:12:18.000000 atomica-1.4.0/atomica/library/combined_framework.xlsx
--rw-rw-r--   0 travis    (2000) travis    (2000)    32289 2019-05-15 02:12:18.000000 atomica-1.4.0/atomica/library/combined_progbook.xlsx
--rw-rw-r--   0 travis    (2000) travis    (2000)    19678 2019-05-15 02:12:18.000000 atomica-1.4.0/atomica/library/diabetes_databook.xlsx
--rw-rw-r--   0 travis    (2000) travis    (2000)    43239 2019-05-15 02:12:18.000000 atomica-1.4.0/atomica/library/diabetes_framework.xlsx
--rw-rw-r--   0 travis    (2000) travis    (2000)    14269 2019-05-15 02:12:18.000000 atomica-1.4.0/atomica/library/diabetes_progbook.xlsx
--rw-rw-r--   0 travis    (2000) travis    (2000)    10829 2019-05-15 02:12:18.000000 atomica-1.4.0/atomica/library/dt_databook.xlsx
--rw-rw-r--   0 travis    (2000) travis    (2000)    35748 2019-05-15 02:12:18.000000 atomica-1.4.0/atomica/library/dt_framework.xlsx
--rw-rw-r--   0 travis    (2000) travis    (2000)    44344 2019-05-15 02:12:18.000000 atomica-1.4.0/atomica/library/framework_template.xlsx
--rw-rw-r--   0 travis    (2000) travis    (2000)    58567 2019-05-15 02:12:18.000000 atomica-1.4.0/atomica/library/framework_template_advanced.xlsx
--rw-rw-r--   0 travis    (2000) travis    (2000)    14418 2019-05-15 02:12:18.000000 atomica-1.4.0/atomica/library/hiv_databook.xlsx
--rw-rw-r--   0 travis    (2000) travis    (2000)    15757 2019-05-15 02:12:18.000000 atomica-1.4.0/atomica/library/hiv_dyn_databook.xlsx
--rw-rw-r--   0 travis    (2000) travis    (2000)    31717 2019-05-15 02:12:18.000000 atomica-1.4.0/atomica/library/hiv_dyn_framework.xlsx
--rw-rw-r--   0 travis    (2000) travis    (2000)    14139 2019-05-15 02:12:18.000000 atomica-1.4.0/atomica/library/hiv_dyn_progbook.xlsx
--rw-rw-r--   0 travis    (2000) travis    (2000)    27989 2019-05-15 02:12:18.000000 atomica-1.4.0/atomica/library/hiv_framework.xlsx
--rw-rw-r--   0 travis    (2000) travis    (2000)    13652 2019-05-15 02:12:18.000000 atomica-1.4.0/atomica/library/hiv_progbook.xlsx
--rw-rw-r--   0 travis    (2000) travis    (2000)    16932 2019-05-15 02:12:18.000000 atomica-1.4.0/atomica/library/hypertension_databook.xlsx
--rw-rw-r--   0 travis    (2000) travis    (2000)    19078 2019-05-15 02:12:18.000000 atomica-1.4.0/atomica/library/hypertension_dyn_databook.xlsx
--rw-rw-r--   0 travis    (2000) travis    (2000)    31393 2019-05-15 02:12:18.000000 atomica-1.4.0/atomica/library/hypertension_dyn_framework.xlsx
--rw-rw-r--   0 travis    (2000) travis    (2000)    13793 2019-05-15 02:12:18.000000 atomica-1.4.0/atomica/library/hypertension_dyn_progbook.xlsx
--rw-rw-r--   0 travis    (2000) travis    (2000)    30814 2019-05-15 02:12:18.000000 atomica-1.4.0/atomica/library/hypertension_framework.xlsx
--rw-rw-r--   0 travis    (2000) travis    (2000)    13712 2019-05-15 02:12:18.000000 atomica-1.4.0/atomica/library/hypertension_progbook.xlsx
--rw-rw-r--   0 travis    (2000) travis    (2000)    12974 2019-05-15 02:12:18.000000 atomica-1.4.0/atomica/library/service_databook.xlsx
--rw-rw-r--   0 travis    (2000) travis    (2000)    27405 2019-05-15 02:12:18.000000 atomica-1.4.0/atomica/library/service_framework.xlsx
--rw-rw-r--   0 travis    (2000) travis    (2000)    18826 2019-05-15 02:12:18.000000 atomica-1.4.0/atomica/library/sir_databook.xlsx
--rw-rw-r--   0 travis    (2000) travis    (2000)    26486 2019-05-15 02:12:18.000000 atomica-1.4.0/atomica/library/sir_framework.xlsx
--rw-rw-r--   0 travis    (2000) travis    (2000)    11248 2019-05-15 02:12:18.000000 atomica-1.4.0/atomica/library/sir_progbook.xlsx
--rw-rw-r--   0 travis    (2000) travis    (2000)   117759 2019-05-15 02:12:18.000000 atomica-1.4.0/atomica/library/tb_databook.xlsx
--rw-rw-r--   0 travis    (2000) travis    (2000)    66598 2019-05-15 02:12:18.000000 atomica-1.4.0/atomica/library/tb_framework.xlsx
--rw-rw-r--   0 travis    (2000) travis    (2000)   260571 2019-05-15 02:12:18.000000 atomica-1.4.0/atomica/library/tb_progbook.xlsx
--rw-rw-r--   0 travis    (2000) travis    (2000)    37702 2019-05-15 02:12:18.000000 atomica-1.4.0/atomica/library/tb_progbook_defaults.xlsx
--rw-rw-r--   0 travis    (2000) travis    (2000)    15083 2019-05-15 02:12:18.000000 atomica-1.4.0/atomica/library/tb_simple_databook.xlsx
--rw-rw-r--   0 travis    (2000) travis    (2000)    18046 2019-05-15 02:12:18.000000 atomica-1.4.0/atomica/library/tb_simple_dyn_databook.xlsx
--rw-rw-r--   0 travis    (2000) travis    (2000)    31844 2019-05-15 02:12:18.000000 atomica-1.4.0/atomica/library/tb_simple_dyn_framework.xlsx
--rw-rw-r--   0 travis    (2000) travis    (2000)    11564 2019-05-15 02:12:18.000000 atomica-1.4.0/atomica/library/tb_simple_dyn_progbook.xlsx
--rw-rw-r--   0 travis    (2000) travis    (2000)    29654 2019-05-15 02:12:18.000000 atomica-1.4.0/atomica/library/tb_simple_framework.xlsx
--rw-rw-r--   0 travis    (2000) travis    (2000)    10567 2019-05-15 02:12:18.000000 atomica-1.4.0/atomica/library/tb_simple_progbook.xlsx
--rw-rw-r--   0 travis    (2000) travis    (2000)    12036 2019-05-15 02:12:18.000000 atomica-1.4.0/atomica/library/udt_databook.xlsx
--rw-rw-r--   0 travis    (2000) travis    (2000)    12536 2019-05-15 02:12:18.000000 atomica-1.4.0/atomica/library/udt_dyn_databook.xlsx
--rw-rw-r--   0 travis    (2000) travis    (2000)    36332 2019-05-15 02:12:18.000000 atomica-1.4.0/atomica/library/udt_dyn_framework.xlsx
--rw-rw-r--   0 travis    (2000) travis    (2000)    10165 2019-05-15 02:12:18.000000 atomica-1.4.0/atomica/library/udt_dyn_progbook.xlsx
--rw-rw-r--   0 travis    (2000) travis    (2000)    35906 2019-05-15 02:12:18.000000 atomica-1.4.0/atomica/library/udt_framework.xlsx
--rw-rw-r--   0 travis    (2000) travis    (2000)    10101 2019-05-15 02:12:18.000000 atomica-1.4.0/atomica/library/udt_progbook.xlsx
--rw-rw-r--   0 travis    (2000) travis    (2000)    11479 2019-05-15 02:12:18.000000 atomica-1.4.0/atomica/library/usdt_databook.xlsx
--rw-rw-r--   0 travis    (2000) travis    (2000)    29177 2019-05-15 02:12:18.000000 atomica-1.4.0/atomica/library/usdt_framework.xlsx
--rw-rw-r--   0 travis    (2000) travis    (2000)    13011 2019-05-15 02:12:18.000000 atomica-1.4.0/atomica/library/usdt_progbook.xlsx
--rw-rw-r--   0 travis    (2000) travis    (2000)    20318 2019-05-15 02:12:18.000000 atomica-1.4.0/atomica/migration.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    75900 2019-05-15 02:12:18.000000 atomica-1.4.0/atomica/model.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    46598 2019-05-15 02:12:18.000000 atomica-1.4.0/atomica/optimization.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8314 2019-05-15 02:12:18.000000 atomica-1.4.0/atomica/parameters.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    91890 2019-05-15 02:12:18.000000 atomica-1.4.0/atomica/plotting.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    73650 2019-05-15 02:12:18.000000 atomica-1.4.0/atomica/programs.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    41379 2019-05-15 02:12:18.000000 atomica-1.4.0/atomica/project.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    16602 2019-05-15 02:12:18.000000 atomica-1.4.0/atomica/reconciliation.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    62864 2019-05-15 02:12:18.000000 atomica-1.4.0/atomica/results.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15182 2019-05-15 02:12:18.000000 atomica-1.4.0/atomica/scenarios.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2721 2019-05-15 02:12:18.000000 atomica-1.4.0/atomica/system.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    24903 2019-05-15 02:12:18.000000 atomica-1.4.0/atomica/utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      199 2019-05-15 02:12:18.000000 atomica-1.4.0/atomica/version.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-05-15 02:12:33.000000 atomica-1.4.0/atomica.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     5820 2019-05-15 02:12:33.000000 atomica-1.4.0/atomica.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     2536 2019-05-15 02:12:33.000000 atomica-1.4.0/atomica.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-05-15 02:12:33.000000 atomica-1.4.0/atomica.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      116 2019-05-15 02:12:33.000000 atomica-1.4.0/atomica.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2019-05-15 02:12:33.000000 atomica-1.4.0/atomica.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2019-05-15 02:12:33.000000 atomica-1.4.0/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     1636 2019-05-15 02:12:18.000000 atomica-1.4.0/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-07 12:55:07.000000 atomica-1.5.0/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35141 2019-06-07 12:54:52.000000 atomica-1.5.0/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)      116 2019-06-07 12:54:52.000000 atomica-1.5.0/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5820 2019-06-07 12:55:07.000000 atomica-1.5.0/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4271 2019-06-07 12:54:52.000000 atomica-1.5.0/README.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-07 12:55:07.000000 atomica-1.5.0/atomica/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3155 2019-06-07 12:54:52.000000 atomica-1.5.0/atomica/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8203 2019-06-07 12:54:52.000000 atomica-1.5.0/atomica/calibration.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    43692 2019-06-07 12:54:52.000000 atomica-1.5.0/atomica/cascade.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    47650 2019-06-07 12:54:52.000000 atomica-1.5.0/atomica/data.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4795 2019-06-07 12:54:52.000000 atomica-1.5.0/atomica/defaults.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    50581 2019-06-07 12:54:52.000000 atomica-1.5.0/atomica/excel.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    65692 2019-06-07 12:54:52.000000 atomica-1.5.0/atomica/framework.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3229 2019-06-07 12:54:52.000000 atomica-1.5.0/atomica/function_parser.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-07 12:55:07.000000 atomica-1.5.0/atomica/library/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14399 2019-06-07 12:54:52.000000 atomica-1.5.0/atomica/library/cervicalcancer_databook.xlsx
+-rw-rw-r--   0 travis    (2000) travis    (2000)    30789 2019-06-07 12:54:52.000000 atomica-1.5.0/atomica/library/cervicalcancer_framework.xlsx
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11141 2019-06-07 12:54:52.000000 atomica-1.5.0/atomica/library/cervicalcancer_progbook.xlsx
+-rw-rw-r--   0 travis    (2000) travis    (2000)    26731 2019-06-07 12:54:52.000000 atomica-1.5.0/atomica/library/combined_databook.xlsx
+-rw-rw-r--   0 travis    (2000) travis    (2000)    41519 2019-06-07 12:54:52.000000 atomica-1.5.0/atomica/library/combined_framework.xlsx
+-rw-rw-r--   0 travis    (2000) travis    (2000)    32289 2019-06-07 12:54:52.000000 atomica-1.5.0/atomica/library/combined_progbook.xlsx
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19678 2019-06-07 12:54:52.000000 atomica-1.5.0/atomica/library/diabetes_databook.xlsx
+-rw-rw-r--   0 travis    (2000) travis    (2000)    43239 2019-06-07 12:54:52.000000 atomica-1.5.0/atomica/library/diabetes_framework.xlsx
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14269 2019-06-07 12:54:52.000000 atomica-1.5.0/atomica/library/diabetes_progbook.xlsx
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10829 2019-06-07 12:54:52.000000 atomica-1.5.0/atomica/library/dt_databook.xlsx
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35748 2019-06-07 12:54:52.000000 atomica-1.5.0/atomica/library/dt_framework.xlsx
+-rw-rw-r--   0 travis    (2000) travis    (2000)    44344 2019-06-07 12:54:52.000000 atomica-1.5.0/atomica/library/framework_template.xlsx
+-rw-rw-r--   0 travis    (2000) travis    (2000)    58567 2019-06-07 12:54:52.000000 atomica-1.5.0/atomica/library/framework_template_advanced.xlsx
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14418 2019-06-07 12:54:52.000000 atomica-1.5.0/atomica/library/hiv_databook.xlsx
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15757 2019-06-07 12:54:52.000000 atomica-1.5.0/atomica/library/hiv_dyn_databook.xlsx
+-rw-rw-r--   0 travis    (2000) travis    (2000)    31717 2019-06-07 12:54:52.000000 atomica-1.5.0/atomica/library/hiv_dyn_framework.xlsx
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14139 2019-06-07 12:54:52.000000 atomica-1.5.0/atomica/library/hiv_dyn_progbook.xlsx
+-rw-rw-r--   0 travis    (2000) travis    (2000)    27989 2019-06-07 12:54:52.000000 atomica-1.5.0/atomica/library/hiv_framework.xlsx
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13652 2019-06-07 12:54:52.000000 atomica-1.5.0/atomica/library/hiv_progbook.xlsx
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16932 2019-06-07 12:54:52.000000 atomica-1.5.0/atomica/library/hypertension_databook.xlsx
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19078 2019-06-07 12:54:52.000000 atomica-1.5.0/atomica/library/hypertension_dyn_databook.xlsx
+-rw-rw-r--   0 travis    (2000) travis    (2000)    31393 2019-06-07 12:54:52.000000 atomica-1.5.0/atomica/library/hypertension_dyn_framework.xlsx
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13793 2019-06-07 12:54:52.000000 atomica-1.5.0/atomica/library/hypertension_dyn_progbook.xlsx
+-rw-rw-r--   0 travis    (2000) travis    (2000)    30814 2019-06-07 12:54:52.000000 atomica-1.5.0/atomica/library/hypertension_framework.xlsx
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13712 2019-06-07 12:54:52.000000 atomica-1.5.0/atomica/library/hypertension_progbook.xlsx
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12974 2019-06-07 12:54:52.000000 atomica-1.5.0/atomica/library/service_databook.xlsx
+-rw-rw-r--   0 travis    (2000) travis    (2000)    27405 2019-06-07 12:54:52.000000 atomica-1.5.0/atomica/library/service_framework.xlsx
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18826 2019-06-07 12:54:52.000000 atomica-1.5.0/atomica/library/sir_databook.xlsx
+-rw-rw-r--   0 travis    (2000) travis    (2000)    26486 2019-06-07 12:54:52.000000 atomica-1.5.0/atomica/library/sir_framework.xlsx
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11248 2019-06-07 12:54:52.000000 atomica-1.5.0/atomica/library/sir_progbook.xlsx
+-rw-rw-r--   0 travis    (2000) travis    (2000)   117759 2019-06-07 12:54:52.000000 atomica-1.5.0/atomica/library/tb_databook.xlsx
+-rw-rw-r--   0 travis    (2000) travis    (2000)    66598 2019-06-07 12:54:52.000000 atomica-1.5.0/atomica/library/tb_framework.xlsx
+-rw-rw-r--   0 travis    (2000) travis    (2000)   260571 2019-06-07 12:54:52.000000 atomica-1.5.0/atomica/library/tb_progbook.xlsx
+-rw-rw-r--   0 travis    (2000) travis    (2000)    37702 2019-06-07 12:54:52.000000 atomica-1.5.0/atomica/library/tb_progbook_defaults.xlsx
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15083 2019-06-07 12:54:52.000000 atomica-1.5.0/atomica/library/tb_simple_databook.xlsx
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18046 2019-06-07 12:54:52.000000 atomica-1.5.0/atomica/library/tb_simple_dyn_databook.xlsx
+-rw-rw-r--   0 travis    (2000) travis    (2000)    31844 2019-06-07 12:54:52.000000 atomica-1.5.0/atomica/library/tb_simple_dyn_framework.xlsx
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11564 2019-06-07 12:54:52.000000 atomica-1.5.0/atomica/library/tb_simple_dyn_progbook.xlsx
+-rw-rw-r--   0 travis    (2000) travis    (2000)    29654 2019-06-07 12:54:52.000000 atomica-1.5.0/atomica/library/tb_simple_framework.xlsx
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10567 2019-06-07 12:54:52.000000 atomica-1.5.0/atomica/library/tb_simple_progbook.xlsx
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12036 2019-06-07 12:54:52.000000 atomica-1.5.0/atomica/library/udt_databook.xlsx
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12536 2019-06-07 12:54:52.000000 atomica-1.5.0/atomica/library/udt_dyn_databook.xlsx
+-rw-rw-r--   0 travis    (2000) travis    (2000)    36332 2019-06-07 12:54:52.000000 atomica-1.5.0/atomica/library/udt_dyn_framework.xlsx
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10165 2019-06-07 12:54:52.000000 atomica-1.5.0/atomica/library/udt_dyn_progbook.xlsx
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35906 2019-06-07 12:54:52.000000 atomica-1.5.0/atomica/library/udt_framework.xlsx
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10101 2019-06-07 12:54:52.000000 atomica-1.5.0/atomica/library/udt_progbook.xlsx
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11479 2019-06-07 12:54:52.000000 atomica-1.5.0/atomica/library/usdt_databook.xlsx
+-rw-rw-r--   0 travis    (2000) travis    (2000)    29177 2019-06-07 12:54:52.000000 atomica-1.5.0/atomica/library/usdt_framework.xlsx
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13011 2019-06-07 12:54:52.000000 atomica-1.5.0/atomica/library/usdt_progbook.xlsx
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20804 2019-06-07 12:54:52.000000 atomica-1.5.0/atomica/migration.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    77653 2019-06-07 12:54:52.000000 atomica-1.5.0/atomica/model.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    47608 2019-06-07 12:54:52.000000 atomica-1.5.0/atomica/optimization.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8510 2019-06-07 12:54:52.000000 atomica-1.5.0/atomica/parameters.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    91890 2019-06-07 12:54:52.000000 atomica-1.5.0/atomica/plotting.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    73650 2019-06-07 12:54:52.000000 atomica-1.5.0/atomica/programs.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    41388 2019-06-07 12:54:52.000000 atomica-1.5.0/atomica/project.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16602 2019-06-07 12:54:52.000000 atomica-1.5.0/atomica/reconciliation.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    64427 2019-06-07 12:54:52.000000 atomica-1.5.0/atomica/results.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15639 2019-06-07 12:54:52.000000 atomica-1.5.0/atomica/scenarios.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2721 2019-06-07 12:54:52.000000 atomica-1.5.0/atomica/system.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    24903 2019-06-07 12:54:52.000000 atomica-1.5.0/atomica/utils.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      199 2019-06-07 12:54:52.000000 atomica-1.5.0/atomica/version.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-07 12:55:07.000000 atomica-1.5.0/atomica.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5820 2019-06-07 12:55:07.000000 atomica-1.5.0/atomica.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2536 2019-06-07 12:55:07.000000 atomica-1.5.0/atomica.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-06-07 12:55:07.000000 atomica-1.5.0/atomica.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      114 2019-06-07 12:55:07.000000 atomica-1.5.0/atomica.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2019-06-07 12:55:07.000000 atomica-1.5.0/atomica.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       38 2019-06-07 12:55:07.000000 atomica-1.5.0/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1634 2019-06-07 12:54:53.000000 atomica-1.5.0/setup.py
```

### Comparing `atomica-1.4.0/LICENSE` & `atomica-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `atomica-1.4.0/PKG-INFO` & `atomica-1.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atomica
-Version: 1.4.0
+Version: 1.5.0
 Summary: Toolbox for compartment-based dynamic systems with costing and optimization
 Home-page: https://atomica.tools
 Author: Atomica Team
 Author-email: info@atomica.tools
 License: UNKNOWN
 Description: # Atomica
```

### Comparing `atomica-1.4.0/README.md` & `atomica-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `atomica-1.4.0/atomica/__init__.py` & `atomica-1.5.0/atomica/__init__.py`

 * *Files identical despite different names*

### Comparing `atomica-1.4.0/atomica/calibration.py` & `atomica-1.5.0/atomica/calibration.py`

 * *Files identical despite different names*

### Comparing `atomica-1.4.0/atomica/cascade.py` & `atomica-1.5.0/atomica/cascade.py`

 * *Files identical despite different names*

### Comparing `atomica-1.4.0/atomica/data.py` & `atomica-1.5.0/atomica/data.py`

 * *Files identical despite different names*

### Comparing `atomica-1.4.0/atomica/defaults.py` & `atomica-1.5.0/atomica/defaults.py`

 * *Files identical despite different names*

### Comparing `atomica-1.4.0/atomica/excel.py` & `atomica-1.5.0/atomica/excel.py`

 * *Files identical despite different names*

### Comparing `atomica-1.4.0/atomica/framework.py` & `atomica-1.5.0/atomica/framework.py`

 * *Files 1% similar despite different names*

```diff
@@ -894,21 +894,27 @@
         # State variables are in number amounts unless normalized.
         if item_type in [FS.KEY_COMPARTMENT, FS.KEY_CHARACTERISTIC]:
             if "denominator" in item_spec.index and item_spec["denominator"] is not None:
                 return FS.QUANTITY_TYPE_FRACTION.title()
             else:
                 return FS.QUANTITY_TYPE_NUMBER.title()
         elif item_type == FS.KEY_PARAMETER:
+            units = item_spec['format'].strip() if item_spec['format'] is not None else None
             if item_spec['timescale']:
-                if item_spec['format'] == FS.QUANTITY_TYPE_DURATION:
+                if units is None:
+                    raise InvalidFramework(f'A timescale was provided for Framework quantity {code_name} but no units were provided')
+                elif units.lower() == FS.QUANTITY_TYPE_DURATION:
                     return '%s (%s)' % (FS.QUANTITY_TYPE_DURATION.title(),format_duration(item_spec['timescale'],pluralize=True))
-                elif item_spec['format'] in {FS.QUANTITY_TYPE_NUMBER,FS.QUANTITY_TYPE_PROBABILITY}:
-                    return '%s (per %s)' % (item_spec['format'].title(),format_duration(item_spec['timescale'],pluralize=False))
-            elif item_spec['format']:
-                return item_spec['format']
+                elif units.lower() in {FS.QUANTITY_TYPE_NUMBER,FS.QUANTITY_TYPE_PROBABILITY}:
+                    return '%s (per %s)' % (units.title(),format_duration(item_spec['timescale'],pluralize=False))
+                else:
+                    if units is None:
+                        raise InvalidFramework(f'A timescale was provided for Framework quantity {code_name} but the units were not one of duration, number, or probability. It is therefore not possible to perform any automatic conversions, simply enter the relevant data entry timescale in the units directly instead.')
+            elif units:
+                return units
 
         return FS.DEFAULT_SYMBOL_INAPPLICABLE
 
 
 def sanitize_dataframe(df, required_columns, defaults, valid_content):
     # Take in a DataFrame and sanitize it
     # INPUTS
```

### Comparing `atomica-1.4.0/atomica/function_parser.py` & `atomica-1.5.0/atomica/function_parser.py`

 * *Files identical despite different names*

### Comparing `atomica-1.4.0/atomica/library/cervicalcancer_databook.xlsx` & `atomica-1.5.0/atomica/library/cervicalcancer_databook.xlsx`

 * *Files identical despite different names*

### Comparing `atomica-1.4.0/atomica/library/cervicalcancer_framework.xlsx` & `atomica-1.5.0/atomica/library/cervicalcancer_framework.xlsx`

 * *Files identical despite different names*

### Comparing `atomica-1.4.0/atomica/library/cervicalcancer_progbook.xlsx` & `atomica-1.5.0/atomica/library/cervicalcancer_progbook.xlsx`

 * *Files identical despite different names*

### Comparing `atomica-1.4.0/atomica/library/combined_databook.xlsx` & `atomica-1.5.0/atomica/library/combined_databook.xlsx`

 * *Files identical despite different names*

### Comparing `atomica-1.4.0/atomica/library/combined_framework.xlsx` & `atomica-1.5.0/atomica/library/combined_framework.xlsx`

 * *Files identical despite different names*

### Comparing `atomica-1.4.0/atomica/library/combined_progbook.xlsx` & `atomica-1.5.0/atomica/library/combined_progbook.xlsx`

 * *Files identical despite different names*

### Comparing `atomica-1.4.0/atomica/library/diabetes_databook.xlsx` & `atomica-1.5.0/atomica/library/diabetes_databook.xlsx`

 * *Files identical despite different names*

### Comparing `atomica-1.4.0/atomica/library/diabetes_framework.xlsx` & `atomica-1.5.0/atomica/library/diabetes_framework.xlsx`

 * *Files identical despite different names*

### Comparing `atomica-1.4.0/atomica/library/diabetes_progbook.xlsx` & `atomica-1.5.0/atomica/library/diabetes_progbook.xlsx`

 * *Files identical despite different names*

### Comparing `atomica-1.4.0/atomica/library/dt_databook.xlsx` & `atomica-1.5.0/atomica/library/dt_databook.xlsx`

 * *Files identical despite different names*

### Comparing `atomica-1.4.0/atomica/library/dt_framework.xlsx` & `atomica-1.5.0/atomica/library/dt_framework.xlsx`

 * *Files identical despite different names*

### Comparing `atomica-1.4.0/atomica/library/framework_template.xlsx` & `atomica-1.5.0/atomica/library/framework_template.xlsx`

 * *Files identical despite different names*

### Comparing `atomica-1.4.0/atomica/library/framework_template_advanced.xlsx` & `atomica-1.5.0/atomica/library/framework_template_advanced.xlsx`

 * *Files identical despite different names*

### Comparing `atomica-1.4.0/atomica/library/hiv_databook.xlsx` & `atomica-1.5.0/atomica/library/hiv_databook.xlsx`

 * *Files identical despite different names*

### Comparing `atomica-1.4.0/atomica/library/hiv_dyn_databook.xlsx` & `atomica-1.5.0/atomica/library/hiv_dyn_databook.xlsx`

 * *Files identical despite different names*

### Comparing `atomica-1.4.0/atomica/library/hiv_dyn_framework.xlsx` & `atomica-1.5.0/atomica/library/hiv_dyn_framework.xlsx`

 * *Files identical despite different names*

### Comparing `atomica-1.4.0/atomica/library/hiv_dyn_progbook.xlsx` & `atomica-1.5.0/atomica/library/hiv_dyn_progbook.xlsx`

 * *Files identical despite different names*

### Comparing `atomica-1.4.0/atomica/library/hiv_framework.xlsx` & `atomica-1.5.0/atomica/library/hiv_framework.xlsx`

 * *Files identical despite different names*

### Comparing `atomica-1.4.0/atomica/library/hiv_progbook.xlsx` & `atomica-1.5.0/atomica/library/hiv_progbook.xlsx`

 * *Files identical despite different names*

### Comparing `atomica-1.4.0/atomica/library/hypertension_databook.xlsx` & `atomica-1.5.0/atomica/library/hypertension_databook.xlsx`

 * *Files identical despite different names*

### Comparing `atomica-1.4.0/atomica/library/hypertension_dyn_databook.xlsx` & `atomica-1.5.0/atomica/library/hypertension_dyn_databook.xlsx`

 * *Files identical despite different names*

### Comparing `atomica-1.4.0/atomica/library/hypertension_dyn_framework.xlsx` & `atomica-1.5.0/atomica/library/hypertension_dyn_framework.xlsx`

 * *Files identical despite different names*

### Comparing `atomica-1.4.0/atomica/library/hypertension_dyn_progbook.xlsx` & `atomica-1.5.0/atomica/library/hypertension_dyn_progbook.xlsx`

 * *Files identical despite different names*

### Comparing `atomica-1.4.0/atomica/library/hypertension_framework.xlsx` & `atomica-1.5.0/atomica/library/hypertension_framework.xlsx`

 * *Files identical despite different names*

### Comparing `atomica-1.4.0/atomica/library/hypertension_progbook.xlsx` & `atomica-1.5.0/atomica/library/hypertension_progbook.xlsx`

 * *Files identical despite different names*

### Comparing `atomica-1.4.0/atomica/library/service_databook.xlsx` & `atomica-1.5.0/atomica/library/service_databook.xlsx`

 * *Files identical despite different names*

### Comparing `atomica-1.4.0/atomica/library/service_framework.xlsx` & `atomica-1.5.0/atomica/library/service_framework.xlsx`

 * *Files identical despite different names*

### Comparing `atomica-1.4.0/atomica/library/sir_databook.xlsx` & `atomica-1.5.0/atomica/library/sir_databook.xlsx`

 * *Files identical despite different names*

### Comparing `atomica-1.4.0/atomica/library/sir_framework.xlsx` & `atomica-1.5.0/atomica/library/sir_framework.xlsx`

 * *Files identical despite different names*

### Comparing `atomica-1.4.0/atomica/library/sir_progbook.xlsx` & `atomica-1.5.0/atomica/library/sir_progbook.xlsx`

 * *Files identical despite different names*

### Comparing `atomica-1.4.0/atomica/library/tb_databook.xlsx` & `atomica-1.5.0/atomica/library/tb_databook.xlsx`

 * *Files identical despite different names*

### Comparing `atomica-1.4.0/atomica/library/tb_framework.xlsx` & `atomica-1.5.0/atomica/library/tb_framework.xlsx`

 * *Files identical despite different names*

### Comparing `atomica-1.4.0/atomica/library/tb_progbook.xlsx` & `atomica-1.5.0/atomica/library/tb_progbook.xlsx`

 * *Files identical despite different names*

### Comparing `atomica-1.4.0/atomica/library/tb_progbook_defaults.xlsx` & `atomica-1.5.0/atomica/library/tb_progbook_defaults.xlsx`

 * *Files identical despite different names*

### Comparing `atomica-1.4.0/atomica/library/tb_simple_databook.xlsx` & `atomica-1.5.0/atomica/library/tb_simple_databook.xlsx`

 * *Files identical despite different names*

### Comparing `atomica-1.4.0/atomica/library/tb_simple_dyn_databook.xlsx` & `atomica-1.5.0/atomica/library/tb_simple_dyn_databook.xlsx`

 * *Files identical despite different names*

### Comparing `atomica-1.4.0/atomica/library/tb_simple_dyn_framework.xlsx` & `atomica-1.5.0/atomica/library/tb_simple_dyn_framework.xlsx`

 * *Files identical despite different names*

### Comparing `atomica-1.4.0/atomica/library/tb_simple_dyn_progbook.xlsx` & `atomica-1.5.0/atomica/library/tb_simple_dyn_progbook.xlsx`

 * *Files identical despite different names*

### Comparing `atomica-1.4.0/atomica/library/tb_simple_framework.xlsx` & `atomica-1.5.0/atomica/library/tb_simple_framework.xlsx`

 * *Files identical despite different names*

### Comparing `atomica-1.4.0/atomica/library/tb_simple_progbook.xlsx` & `atomica-1.5.0/atomica/library/tb_simple_progbook.xlsx`

 * *Files identical despite different names*

### Comparing `atomica-1.4.0/atomica/library/udt_databook.xlsx` & `atomica-1.5.0/atomica/library/udt_databook.xlsx`

 * *Files identical despite different names*

### Comparing `atomica-1.4.0/atomica/library/udt_dyn_databook.xlsx` & `atomica-1.5.0/atomica/library/udt_dyn_databook.xlsx`

 * *Files identical despite different names*

### Comparing `atomica-1.4.0/atomica/library/udt_dyn_framework.xlsx` & `atomica-1.5.0/atomica/library/udt_dyn_framework.xlsx`

 * *Files identical despite different names*

### Comparing `atomica-1.4.0/atomica/library/udt_dyn_progbook.xlsx` & `atomica-1.5.0/atomica/library/udt_dyn_progbook.xlsx`

 * *Files identical despite different names*

### Comparing `atomica-1.4.0/atomica/library/udt_framework.xlsx` & `atomica-1.5.0/atomica/library/udt_framework.xlsx`

 * *Files identical despite different names*

### Comparing `atomica-1.4.0/atomica/library/udt_progbook.xlsx` & `atomica-1.5.0/atomica/library/udt_progbook.xlsx`

 * *Files identical despite different names*

### Comparing `atomica-1.4.0/atomica/library/usdt_databook.xlsx` & `atomica-1.5.0/atomica/library/usdt_databook.xlsx`

 * *Files identical despite different names*

### Comparing `atomica-1.4.0/atomica/library/usdt_framework.xlsx` & `atomica-1.5.0/atomica/library/usdt_framework.xlsx`

 * *Files identical despite different names*

### Comparing `atomica-1.4.0/atomica/library/usdt_progbook.xlsx` & `atomica-1.5.0/atomica/library/usdt_progbook.xlsx`

 * *Files identical despite different names*

### Comparing `atomica-1.4.0/atomica/migration.py` & `atomica-1.5.0/atomica/migration.py`

 * *Files 2% similar despite different names*

```diff
@@ -522,7 +522,21 @@
         fw.pars['is derivative'] = 'n'
     for result in all_results(proj):
         for pop in result.model.pops:
             for par in pop.pars:
                 par.derivative = False
     return proj
 
+@migration('1.4.3', '1.5.0', 'Parameters with functions can be overwritten')
+def add_parset_disable_function(proj):
+
+    # Add skip_function flag to parset Parameter instances
+    for parset in proj.parsets.values():
+        for par in parset.all_pars():
+            par.skip_function = sc.odict.fromkeys(par.ts, None)
+
+    for result in all_results(proj):
+        for pop in result.model.pops:
+            for par in pop.pars:
+                par.skip_function = None
+    return proj
+
```

### Comparing `atomica-1.4.0/atomica/model.py` & `atomica-1.5.0/atomica/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -364,14 +364,15 @@
         self._source_popsize_cache_val = None #: Internal cache for the last previously computed source popsize
         self.fcn_str = None  #: String representation of parameter function
         self.deps = dict()  #: Dict of dependencies containing lists of integration objects
         self._fcn = None  #: Internal cache for parsed parameter function (this will be dropped when pickled)
         self._precompute = False #: If True, the parameter function will be computed in a vector operation prior to integration
         self._is_dynamic = False #: If True, this parameter will be updated during integration. Note that `precompute` and `dynamic` are mutually exclusive
         self.derivative = False #: If True, the parameter function will be treated as a derivative and the value added on to the end
+        self.skip_function = None #: Can optionally be set to a (start,stop) tuple of times. Between these times, the parameter will not be updated so the parset value will be left unchanged
 
         #: For transition parameters, the ``vals`` stored by the parameter is effectively a rate. The ``timescale``
         #: attribute informs the time period corresponding to the units in which the rate has been provided.
         #: If the units are ``number`` or ``probability`` then the ``timescale`` corresponds to the denominator of the units
         #: e.g. probability/day (with ``timescale=1/365``).
         #: If the units are ``duration`` then the timescale stores the units in which the duration has been specified
         #: e.g. ``duration=1`` with ``timescale=1/52`` is the same as ``duration=7`` with ``timescale=1/365``
@@ -524,20 +525,32 @@
         """
 
         if not self._fcn or self.pop_aggregation:
             return
 
         if ti is None:
             if self.derivative:
-                raise Exception('Cannot perform a vector update of a derivate parameter')
+                raise Exception('Cannot perform a vector update of a derivative parameter (these parameters intrinsically require integration to be computed)')
             ti = np.arange(0, self.vals.size)  # This corresponds to every time point
 
         if self.derivative and ti == 0:
             return
 
+        if self.skip_function:
+            # If we don't want to overwrite the parameter in certain years, those years need to be excluded
+            if hasattr(ti, '__len__'):
+                # Filter out years outside the excluded range
+                ti = ti[np.where((self.t[ti] < self.skip_function[0]) | (self.t[ti] > self.skip_function[1]))]
+                if ti.size == 0: # If all times were removed
+                    return
+            else:
+                # Dealing with a scalar ti
+                if (self.t[ti] >= self.skip_function[0]) and (self.t[ti] <= self.skip_function[1]):
+                    return
+
         dep_vals = dict.fromkeys(self.deps, 0.0)
         for dep_name, deps in self.deps.items():
             for dep in deps:
                 if isinstance(dep, Link):
                     dep_vals[dep_name] += dep.vals[ti] / dep.dt
                 else:
                     dep_vals[dep_name] += dep.vals[ti]
@@ -755,15 +768,18 @@
 
             return links
         else:
             raise NotFoundError(f"Object '{name}' not found in population '{self.name}'")
 
     def get_comp(self, comp_name):
         """ Allow compartments to be retrieved by name rather than index. Returns a Compartment. """
-        return self.comp_lookup[comp_name]
+        try:
+            return self.comp_lookup[comp_name]
+        except KeyError:
+            raise NotFoundError(f'Compartment {comp_name} not found')
 
     def get_links(self, name) -> list:
         """ Retrieve Links. """
         # Links can be looked up by parameter name or by link name, unlike get_variable. This is because
         # get_links() is guaranteed to return a list of Link objects
         # As opposed to get_variable which would retrieve the Parameter for 'doth rate' and the Links for 'z'
         if name in self.par_lookup:
@@ -771,19 +787,25 @@
         elif name in self.link_lookup:
             return self.link_lookup[name]
         else:
             raise NotFoundError("Object '{0}' not found.".format(name))
 
     def get_charac(self, charac_name):
         """ Allow dependencies to be retrieved by name rather than index. Returns a Variable. """
-        return self.charac_lookup[charac_name]
+        try:
+            return self.charac_lookup[charac_name]
+        except KeyError:
+            raise NotFoundError(f'Characteristic {charac_name} not found')
 
     def get_par(self, par_name):
         """ Allow dependencies to be retrieved by name rather than index. Returns a Variable. """
-        return self.par_lookup[par_name]
+        try:
+            return self.par_lookup[par_name]
+        except KeyError:
+            raise NotFoundError(f'Parameter {par_name} not found')
 
     def gen_cascade(self, framework, progset):
         """
         Generate a compartmental cascade as defined in a settings object.
         Fill out the compartment, transition and dependency lists within the model population object.
         Maintaining order as defined in a cascade workbook is crucial due to cross-referencing.
         """
@@ -1180,28 +1202,36 @@
                 for var in self._vars_by_pop[pars[0].pop_aggregation[1]]:
                     var.set_dynamic(progset=self.progset)
                 if len(pars[0].pop_aggregation) > 3:
                     for var in self._vars_by_pop[pars[0].pop_aggregation[3]]:
                         var.set_dynamic(progset=self.progset)
 
         # Insert parameter initial values and do any required precomputation
-        for par_name in self.framework.pars.index:
+        for par_name in self.framework.pars.index: # Iterate only over framework pars (parset.pars also includes characteristics)
             cascade_par = parset.pars[par_name]
             if cascade_par.name in self._vars_by_pop: # The parameter could be missing if it is defined in a population type that is not present in the simulation
                 pars = self._vars_by_pop[cascade_par.name]
                 for par in pars:
-                    par.scale_vactor = cascade_par.meta_y_factor # Set meta scale factor regardless of whether a population-specific y-factor is also provided
+                    par.scale_factor = cascade_par.meta_y_factor # Set meta scale factor regardless of whether a population-specific y-factor is also provided
+
                     if par.pop.name in cascade_par.y_factor:
                         par.scale_factor *= cascade_par.y_factor[par.pop.name] # Add in population-specific scale factor
+
+                    if par.pop.name in cascade_par.skip_function:
+                        par.skip_function = cascade_par.skip_function[par.pop.name] # Copy in any skipped evaluations
+                        if par.skip_function:
+                            assert cascade_par.has_values(par.pop.name), 'Parameter function was marked as being skipped for some of the simulation, but the ParameterSet has no values to use instead. If skipping, the ParameterSet must contain some values'
+
                     if cascade_par.has_values(par.pop.name): # If the databook contains values, then insert them now
                         par.vals = cascade_par.interpolate(tvec=self.t, pop_name=par.pop.name) * par.scale_factor
-                        par.constrain()  # Sampling might result in the parameter value going out of bounds (or user might have entered bad values in the databook) so ensure they are clipped here
+
                     if par.fcn_str and par._precompute: # If the parameter is marked for precomputation, then insert it now
                         par.update()
-                        par.constrain()
+
+                    par.constrain()  # Sampling might result in the parameter value going out of bounds (or user might have entered bad values in the databook) so ensure they are clipped here
 
     def process(self):
         """ Run the full model. """
 
         assert self._t_index == 0  # Only makes sense to process a simulation once, starting at ti=0 - this might be relaxed later on
 
         self.update_program_cache()
```

### Comparing `atomica-1.4.0/atomica/optimization.py` & `atomica-1.5.0/atomica/optimization.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 This module implements the :class:`Optimization` class, which contains the
 information required to perform an optimization in Atomica. An Optimization
 effectively serves as a mapping from one set of program instructions to another.
 
 """
 
 import sciris as sc
-from .system import logger
+from .system import logger, NotFoundError
 from .utils import NamedItem
 import numpy as np
 from .model import Model, Link
 import pickle
 import scipy.optimize
 from collections import defaultdict
 from .utils import TimeSeries
@@ -231,22 +231,41 @@
             t_filter = (model.t >= self.t[0]) & (model.t < self.t[1])  # Don't include upper bound, so [2018,2019] will include exactly one year
 
         if self.measurable_name in model.progset.programs:
             alloc = model.progset.get_alloc(model.t, model.program_instructions)
             val = np.sum(alloc[self.measurable_name][t_filter])
         else:  # If the measurable is a model output...
             val = 0.0
+            matched = False # Flag whether any variables were found
             for pop in model.pops:
-                if not self.pop_names or pop in self.pop_names:
-                    vars = pop.get_variable(self.measurable_name)
-                    for var in vars:
-                        if isinstance(var, Link):
-                            val += np.sum(var.vals[t_filter] / var.dt)  # Annualize link values - usually this won't make a difference, but it matters if the user mixes Links with something else in the objective
-                        else:
-                            val += np.sum(var.vals[t_filter])
+                if not self.pop_names:
+                    # If no pops were provided, then iterate over all pops but skip those where the measureable is not defined
+                    # Use this approach rather than checking the pop type in the framework because user could be optimizating
+                    # flow rates or transitions that don't appear in the framework
+                    try:
+                        vars = pop.get_variable(self.measurable_name)
+                        matched = True
+                    except NotFoundError:
+                        continue
+                elif pop not in self.pop_names:
+                    continue
+                else:
+                    vars = pop.get_variable(self.measurable_name) # If variable is missing and the pop was explicitly defined, raise the error
+                    matched = True
+
+                for var in vars:
+                    if isinstance(var, Link):
+                        val += np.sum(var.vals[t_filter] / var.dt)  # Annualize link values - usually this won't make a difference, but it matters if the user mixes Links with something else in the objective
+                    else:
+                        val += np.sum(var.vals[t_filter])
+
+            if not matched:
+                # Raise an error if the measureable was not found in any populations
+                raise Exception('"%s" not found in any populations' % (self.measurable_name))
+
         return val
 
     def _transform_val(self, val):
         # Apply function transformation and weight to the value
         if self.fcn:
             val = self.fcn(val)
         val *= self.weight
@@ -595,15 +614,15 @@
         progset_instructions = ProgramInstructions(alloc=progset, start_year=start_year)  # passing in the progset means we fix the spending in the start year
 
         # Add a spending adjustment in the start/optimization year for every program in the progset, using the lower/upper bounds
         # passed in as arguments to this function
         adjustments = []
         default_spend = progset.get_alloc(tvec=adjustment_year, instructions=progset_instructions)  # Record the default spend for scale-up in money minimization
         for prog_name in progset.programs:
-            limits = sc.dcp(prog_spending[prog_name])
+            limits = list(sc.dcp(prog_spending[prog_name]))
             if limits[0] is None:
                 limits[0] = 0.0
             if limits[1] is None and optim_type == 'money':
                 # Money minimization requires an absolute upper bound. Limit it to 5x default spend by default
                 limits[1] = 5 * default_spend[prog_name]
             adjustments.append(SpendingAdjustment(prog_name, t=adjustment_year, limit_type='abs', lower=limits[0], upper=limits[1]))
```

### Comparing `atomica-1.4.0/atomica/parameters.py` & `atomica-1.5.0/atomica/parameters.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     """
 
     def __init__(self, name: str, ts: dict):
         NamedItem.__init__(self, name)
         self.ts = ts #: Population-specific data is stored in TimeSeries within this dict, keyed by population name
         self.y_factor = sc.odict.fromkeys(self.ts,1.0) #: Calibration scale factors for the parameter in each population
         self.meta_y_factor = 1.0 #: Calibration scale factor for all populations
-
+        self.skip_function = sc.odict.fromkeys(self.ts,None) #: This can be a range of years [start,stop] between which the parameter function will not be evaluated
 
     @property
     def pops(self):
         """
         Get populations contained in the Parameter
 
         :return: Generator/list of available populations
@@ -125,15 +125,15 @@
         self.transfers = sc.odict() #: Stores the Parameter instances contained by this ParameterSet associated with databook transfers, keyed by source population
         self.interactions = sc.odict() #: Stores the Parameter instances contained by this ParameterSet associated with framework interactions, keyed by source population
 
         # Instantiate all quantities that appear in the databook (compartments, characteristics, parameters)
         for name, tdve in data.tdve.items():
             for pop_name, ts in tdve.ts.items(): # The TDVE has already been validated to contain any required populations (although it might also contain extra ones)
                 units = framework.get_databook_units(name)
-                if units != ts.units:
+                if units.strip().lower() != ts.units.strip().lower():
                     raise Exception('The units entered in the databook do not match the units entered in the framework')
             self.pars[name] = Parameter(name,sc.dcp(tdve.ts))
 
         # Instantiate parameters not in the databook
         for _, spec in framework.pars.iterrows():
             if spec.name not in self.pars:
                 ts = dict()
```

### Comparing `atomica-1.4.0/atomica/plotting.py` & `atomica-1.5.0/atomica/plotting.py`

 * *Files identical despite different names*

### Comparing `atomica-1.4.0/atomica/programs.py` & `atomica-1.5.0/atomica/programs.py`

 * *Files identical despite different names*

### Comparing `atomica-1.4.0/atomica/project.py` & `atomica-1.5.0/atomica/project.py`

 * *Files 0% similar despite different names*

```diff
@@ -185,15 +185,15 @@
 
         data = ProjectData.from_spreadsheet(databook_spreadsheet, self.framework)
 
         # If there are existing progsets, make sure the new data is consistent with them
         if self.progsets:
             data_pops = set((x,y['label']) for x,y in data.pops.items())
             for progset in self.progsets.values():
-                assert data_pops == set((x,y) for x,y in progset.pops.items()), 'Existing progsets exist with populations that do not match the new databook'
+                assert data_pops == set((x,y['label']) for x,y in progset.pops.items()), 'Existing progsets exist with populations that do not match the new databook'
 
         self.data = data
         self.data.validate(self.framework)  # Make sure the data is suitable for use in the Project (as opposed to just manipulating the databook)
         self.databook = sc.dcp(databook_spreadsheet)  # Actually a shallow copy is fine here because sc.Spreadsheet contains no mutable properties
         self.modified = sc.now()
         self.settings.update_time_vector(start=self.data.start_year)  # Align sim start year with data start year.
```

### Comparing `atomica-1.4.0/atomica/reconciliation.py` & `atomica-1.5.0/atomica/reconciliation.py`

 * *Files identical despite different names*

### Comparing `atomica-1.4.0/atomica/results.py` & `atomica-1.5.0/atomica/results.py`

 * *Files 2% similar despite different names*

```diff
@@ -296,25 +296,38 @@
         :return: A DataFrame with all model outputs
 
         """
 
         # Assemble the outputs into a dict
         d = dict()
 
+        def gl(name):
+            # Local helper to get name and gracefully deal with transfer parameters that don't appear in the framework
+            try:
+                return self.framework.get_label(name)
+            except NotFoundError:
+                return '-'
+
         for pop in self.model.pops:
             for comp in pop.comps:
-                d[('Compartments', pop.name, comp.name)] = comp.vals
+                d[('Compartments', pop.name, comp.name,gl(comp.name))] = comp.vals
             for charac in pop.characs:
-                d[('Characteristics', pop.name, charac.name)] = charac.vals
+                d[('Characteristics', pop.name, charac.name, gl(charac.name))] = charac.vals
             for par in pop.pars:
                 if par.vals is not None:
-                    d[('Parameters', pop.name, par.name)] = par.vals
+                    d[('Parameters', pop.name, par.name, gl(par.name))] = par.vals
             for link in pop.links:
                 # Sum over duplicate links and annualize flow rate
-                key = ('Flow rates', pop.name, link.name)
+                par_label = gl(link.parameter.name)
+                if par_label == '-':
+                    link_label = par_label
+                else:
+                    link_label = '%s (flow)' % (par_label)
+
+                key = ('Flow rates', pop.name, link.name,  link_label)
                 if key not in d:
                     d[key] = np.zeros(self.t.shape)
                 d[key] += link.vals / self.dt
 
         # Create DataFrame from dict
         df = pd.DataFrame(d, index=self.t)
         df.index.name = 'Time'
@@ -359,29 +372,15 @@
 
         quantities = evaluate_plot_string(this_plot['quantities'])
 
         # Work out which populations these are defined in
         # Going via Result.get_variable() means that it will automatically
         # work correctly for flow rate syntax as well
         if not pops:
-            if sc.isstring(quantities):
-                vars = self.get_variable(quantities)
-            elif isinstance(quantities,list):
-                vars = self.get_variable(quantities[0])
-            elif isinstance(quantities,dict):
-                v = list(quantities.values())[0]
-                if isinstance(v, list):
-                    vars = self.get_variable(v[0])
-                elif sc.isstring(v):
-                    # It could be a function aggregation or it could be a single one
-                    _, deps = parse_function(v)
-                    vars = self.get_variable(deps[0])
-            else:
-                raise Exception('Could not determine population type')
-            pops = [x.pop.name for x in vars]
+            pops = _filter_pops_by_output(self,quantities)
 
         d = PlotData(self, outputs=quantities, pops=pops, project=project)
         h = plot_series(d, axis='pops', data=(project.data if project is not None else None))
         plt.title(this_plot['name'])
         return h
 
     def budget(self, year=None):
@@ -399,14 +398,45 @@
         if self.model.progset is None:
             return None
         else:
             if year is None:
                 year = self.t
             return self.model.progset.get_alloc(year, self.model.program_instructions)
 
+def _filter_pops_by_output(result,output) -> list:
+    """
+    Helper function for plotting quantities
+
+    With population types, a given output/output aggregation may only be defined
+    in a subset of populations. To deal with this when plotting Result objects,
+    it's necessary to work out which population the requested output aggregation can be
+    plotted in. This function takes in an output definition and returns a list of populations
+    matching this.
+
+    :param output: An output aggregation string e.g. 'alive' or ':ddis' or {['lt_inf','lteu']} (supported by PlotData/get_variable)
+    :return: A list of population code names
+
+    """
+
+    if sc.isstring(output):
+        vars = result.get_variable(output)
+    elif isinstance(output, list):
+        vars = result.get_variable(output[0])
+    elif isinstance(output, dict):
+        v = list(output.values())[0]
+        if isinstance(v, list):
+            vars = result.get_variable(v[0])
+        elif sc.isstring(v):
+            # It could be a function aggregation or it could be a single one
+            _, deps = parse_function(v)
+            vars = result.get_variable(deps[0])
+    else:
+        raise Exception('Could not determine population type')
+    return [x.pop.name for x in vars]
+
 
 def export_results(results, filename=None, output_ordering=('output', 'result', 'pop'),
                    cascade_ordering=('pop', 'result', 'stage'), program_ordering=('program', 'result', 'quantity')):
     """ Export Result outputs to a file
 
     This function writes an XLSX file with the data corresponding to any Cascades or Plots
     that are present. Note that results are exported for every year by selecting integer years.
@@ -563,21 +593,25 @@
     :param results: List of Results
     :param cascade_name: The name or index of a cascade stage (interpretable by get_cascade_vals)
     :param tvals: Outputs will be interpolated onto the times in this array (typically would be annual)
     :return: A DataFrame
 
     """
 
-    from .cascade import get_cascade_vals
+    from .cascade import get_cascade_vals, sanitize_cascade
+
+    # Find the cascade pop type
+    _, cascade_dict, pop_type = sanitize_cascade(results[0].framework, cascade_name)
 
     # Prepare the population names and time values
     pop_names = dict()
     pop_names['all'] = 'Entire population'
-    for pop_name, pop_label in zip(results[0].pop_names, results[0].pop_labels):
-        pop_names[pop_name] = pop_label
+    for pop in results[0].model.pops:
+        if pop.type == pop_type:
+            pop_names[pop.name] = pop.label
 
     cascade_df = []
     for pop, label in pop_names.items():
         data = sc.odict()
         for result in results:
             cascade_vals, _ = get_cascade_vals(result, cascade_name, pops=pop, year=tvals)
             for stage, vals in cascade_vals.items():
@@ -595,50 +629,49 @@
     Convert an output to a DataFrame for a group of results
 
     This function takes in a list of results, and an output specification recognised by :class:`PlotData`.
     It extracts the outputs from all results and stores them in a 3-level MultiIndexed dataframe, which is
     returned. The index levels are the name of the output, the name of the results, and the populations.
 
     In addition, this function attempts to aggregate the outputs, if the units of the outputs matches
-    known units. If the units lead to an obvious use of summation or weighted averating, it will be used.
+    known units. If the units lead to anver obvious use of summation or weighted averating, it will be used.
     Otherwise, the output will contain NaNs for the population-aggregated results, which will appear as empty
     cells in the Excel spreadsheet so the user is able to fill them in themselves.
 
     :param results: List of Results
     :param output_name: The name to use for the output quantity
     :param output: An output specification/aggregation supported by :class:`PlotData`
     :param tvals: Outputs will be interpolated onto the times in this array (typically would be annual)
     :return: A DataFrame
 
     """
 
     from .plotting import PlotData
 
-    pop_labels = {x: y for x, y in zip(results[0].pop_names, results[0].pop_labels)}
+    pops = _filter_pops_by_output(results[0],output)
+    pop_labels = {x: y for x, y in zip(results[0].pop_names, results[0].pop_labels) if x in pops}
     data = dict()
-    popdata = PlotData(results, outputs=output)
-    assert len(
-        popdata.outputs) == 1, 'Framework plot specification should evaluate to exactly one output series - there were %d' % (
-        len(popdata.outputs))
+
+    popdata = PlotData(results, pops=pops, outputs=output)
+    assert len(popdata.outputs) == 1, 'Framework plot specification should evaluate to exactly one output series - there were %d' % (len(popdata.outputs))
     popdata.interpolate(tvals)
     for result in popdata.results:
         for pop_name in popdata.pops:
-            data[(output_name, popdata.results[result], pop_labels[pop_name])] = popdata[
-                result, pop_name, popdata.outputs[0]].vals
+            data[(output_name, popdata.results[result], pop_labels[pop_name])] = popdata[result, pop_name, popdata.outputs[0]].vals
 
     # Now do a population total. Need to check the units after any aggregations
     # Check results[0].model.pops[0].comps[0].units just in case someone changes it later on
     if popdata.series[0].units in {FS.QUANTITY_TYPE_NUMBER, results[0].model.pops[0].comps[0].units}:
         # Number units, can use summation
-        popdata = PlotData(results, outputs=output, pops='total', pop_aggregation='sum')
+        popdata = PlotData(results, outputs=output, pops={'total':pops}, pop_aggregation='sum')
         popdata.interpolate(tvals)
         for result in popdata.results:
             data[(output_name, popdata.results[result], 'Total (sum)')] = popdata[result, popdata.pops[0], popdata.outputs[0]].vals
     elif popdata.series[0].units in {FS.QUANTITY_TYPE_FRACTION, FS.QUANTITY_TYPE_PROPORTION,FS.QUANTITY_TYPE_PROBABILITY}:
-        popdata = PlotData(results, outputs=output, pops='total', pop_aggregation='weighted')
+        popdata = PlotData(results, outputs=output, pops={'total':pops}, pop_aggregation='weighted')
         popdata.interpolate(tvals)
         for result in popdata.results:
             data[(output_name, popdata.results[result], 'Total (weighted average)')] = popdata[result, popdata.pops[0], popdata.outputs[0]].vals
     else:
         for result in popdata.results:
             data[(output_name, popdata.results[result], 'Total (unknown units)')] = np.full(tvals.shape, np.nan)
 
@@ -1274,15 +1307,22 @@
                         else:
                             vals = np.array([x.interpolate(year) for x in series_lookup[result, pop, output]])
                             labels.append('%s: %s-%s-%s (%g)' % (self.name, result, pop, output, year))
                         x.append(vals.ravel())
 
 
         locations = offset + np.arange(len(x))
-        plt.boxplot(np.vstack(x).T, positions=locations, manage_xticks=False)
+
+        # TODO - force matplotlib>=3.1 to address this
+        import matplotlib
+        if sc.compareversions(matplotlib.__version__,'3.1') < 0:
+            plt.boxplot(np.vstack(x).T, positions=locations, manage_xticks=False)
+        else:
+            plt.boxplot(np.vstack(x).T, positions=locations, manage_ticks=False)
+
         ax.set_xlim(-0.5, locations[-1] + 0.5)
         if offset == 0:
             ax.set_xticks(np.arange(locations[-1] + 1))
             ax.set_xticklabels(labels)
         else:
             new_labels = [x.get_text() for x in ax.get_xticklabels()] + labels
             ax.set_xticks(np.arange(locations[-1] + 1))
```

### Comparing `atomica-1.4.0/atomica/scenarios.py` & `atomica-1.5.0/atomica/scenarios.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,15 +108,15 @@
 
         if parset is None:
             parset = project.parsets[self.parsetname]
         else:
             parset = project.parset(parset)
 
         if progset is None and self.progsetname is not None:
-            progset = project.progsets[self.parsetname]
+            progset = project.progsets[self.progsetname]
         elif progset is not None:
             progset = project.progset(progset)
 
         parset = self.get_parset(parset, project)
         progset = self.get_progset(progset, project)
         instructions = self.get_instructions(progset, project)
 
@@ -247,51 +247,54 @@
         # on a per-parameter+pop basis. Within the scenario, only the data points in scvalues will be used
 
         new_parset = sc.dcp(parset)
         new_parset.name = self.name + '_' + parset.name
 
         for par_label in self.scenario_values.keys():
             par = new_parset.pars[par_label]  # This is the parameter we are updating
+            has_function = project.framework.pars.at[par.name, 'function'] # Flag whether this is a function parameter in the framework
 
             for pop_label, overwrite in self.scenario_values[par_label].items():
 
                 # Remove Nones and Nans
                 overwrite = sc.dcp(overwrite)
                 overwrite['t'] = sc.promotetoarray(overwrite['t']).astype('float') # astype('float') converts None to np.nan
                 overwrite['y'] = sc.promotetoarray(overwrite['y']).astype('float')
                 idx = ~np.isnan(overwrite['t']) & ~np.isnan(overwrite['y'])
                 if not np.any(idx):
                     continue
                 overwrite['t'] = overwrite['t'][idx]
                 overwrite['y'] = overwrite['y'][idx]
 
-                if not par.has_values(pop_label):
-                    raise Exception("You cannot specify overwrites for a parameter with a function, instead you should overwrite its dependencies")
-
                 original_y_end = par.interpolate(np.array([max(overwrite['t']) + 1e-5]), pop_label)
 
                 # If the Parameter had an assumption, then insert the assumption value in the start year
                 if not par.ts[pop_label].has_time_data:
                     par.ts[pop_label].insert(project.settings.sim_start, par.ts[pop_label].assumption)
 
+                if has_function and 'smooth_onset' in overwrite:
+                    raise Exception('Parameter function overwrites cannot have smooth onsets (because the value at the onset time is not yet known)')
+
                 if 'smooth_onset' not in overwrite:
+                    # Note parameter functions still get smooth onset set here - this ensures
+                    # correct non-smooth-onset behaviour _during_ the overwrite
                     overwrite['smooth_onset'] = 1e-5
 
                 if np.isscalar(overwrite['smooth_onset']):
                     onset = [overwrite['smooth_onset']]*len(overwrite['y'])
                 else:
                     assert len(overwrite['smooth_onset']) == len(overwrite['y']), 'Smooth onset must be either a scalar or an array with length matching y-values'
                     onset = overwrite['smooth_onset']
 
                 # Now, insert all of the program overwrites
                 if len(overwrite['t']) != len(overwrite['y']):
                     raise Exception('Number of time points in overwrite does not match number of values')
 
                 if len(overwrite['t']) == 1:
-                    logger.warning('Only one time point was specified in the overwrite, which means that the overwrite will not have any effect')
+                    raise Exception('Only one time point was specified in the overwrite, which means that the overwrite will not have any effect')
 
                 for i in range(0, len(overwrite['t'])):
 
                     # Account for smooth onset
                     if onset[i] > 0:
                         t = overwrite['t'][i] - onset[i]
 
@@ -314,9 +317,12 @@
 
                     # Insert the overwrite value - assume scenario value is AFTER y-factor rescaling
                     par.ts[pop_label].insert(overwrite['t'][i], overwrite['y'][i] / par.y_factor[pop_label] / par.meta_y_factor)
 
                 # Add an extra point to return the parset back to it's original value after the final overwrite
                 par.ts[pop_label].insert(max(overwrite['t']) + 1e-5, original_y_end)
 
+                if has_function:
+                    par.skip_function[pop_label] = (min(overwrite['t']), max(overwrite['t']))
+
         return new_parset
```

### Comparing `atomica-1.4.0/atomica/system.py` & `atomica-1.5.0/atomica/system.py`

 * *Files identical despite different names*

### Comparing `atomica-1.4.0/atomica/utils.py` & `atomica-1.5.0/atomica/utils.py`

 * *Files identical despite different names*

### Comparing `atomica-1.4.0/atomica.egg-info/PKG-INFO` & `atomica-1.5.0/atomica.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atomica
-Version: 1.4.0
+Version: 1.5.0
 Summary: Toolbox for compartment-based dynamic systems with costing and optimization
 Home-page: https://atomica.tools
 Author: Atomica Team
 Author-email: info@atomica.tools
 License: UNKNOWN
 Description: # Atomica
```

### Comparing `atomica-1.4.0/atomica.egg-info/SOURCES.txt` & `atomica-1.5.0/atomica.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `atomica-1.4.0/setup.py` & `atomica-1.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     url='https://atomica.tools',
     keywords=['dynamic','compartment','optimization', 'disease'],
     platforms=['OS Independent'],
     classifiers=CLASSIFIERS,
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
-        'matplotlib>=1.4.2',
+        'matplotlib>=3.0',
         'numpy>=1.10.1',
         'scipy',
         'pandas',
         'six>=1.11.0',
         'xlsxwriter',
         'openpyxl>=2.5,<2.6',
         'pyswarm',
```

