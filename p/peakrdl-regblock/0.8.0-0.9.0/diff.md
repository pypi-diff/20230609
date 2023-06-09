# Comparing `tmp/peakrdl-regblock-0.8.0.tar.gz` & `tmp/peakrdl-regblock-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peakrdl-regblock-0.8.0.tar", last modified: Wed Oct 19 04:38:44 2022, max compression
+gzip compressed data, was "peakrdl-regblock-0.9.0.tar", last modified: Thu Nov 10 06:07:49 2022, max compression
```

## Comparing `peakrdl-regblock-0.8.0.tar` & `peakrdl-regblock-0.9.0.tar`

### file list

```diff
@@ -1,67 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 04:38:44.758308 peakrdl-regblock-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-10-19 04:38:43.000000 peakrdl-regblock-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       56 2022-10-19 04:38:43.000000 peakrdl-regblock-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1987 2022-10-19 04:38:44.758308 peakrdl-regblock-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      745 2022-10-19 04:38:43.000000 peakrdl-regblock-0.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-19 04:38:44.758308 peakrdl-regblock-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2016 2022-10-19 04:38:43.000000 peakrdl-regblock-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 04:38:44.750308 peakrdl-regblock-0.8.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 04:38:44.750308 peakrdl-regblock-0.8.0/src/peakrdl_regblock/
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-10-19 04:38:43.000000 peakrdl-regblock-0.8.0/src/peakrdl_regblock/__about__.py
--rw-r--r--   0 runner    (1001) docker     (121)       75 2022-10-19 04:38:43.000000 peakrdl-regblock-0.8.0/src/peakrdl_regblock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2857 2022-10-19 04:38:43.000000 peakrdl-regblock-0.8.0/src/peakrdl_regblock/__peakrdl__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4753 2022-10-19 04:38:43.000000 peakrdl-regblock-0.8.0/src/peakrdl_regblock/addr_decode.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 04:38:44.754308 peakrdl-regblock-0.8.0/src/peakrdl_regblock/cpuif/
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-10-19 04:38:43.000000 peakrdl-regblock-0.8.0/src/peakrdl_regblock/cpuif/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 04:38:44.754308 peakrdl-regblock-0.8.0/src/peakrdl_regblock/cpuif/apb3/
--rw-r--r--   0 runner    (1001) docker     (121)      981 2022-10-19 04:38:43.000000 peakrdl-regblock-0.8.0/src/peakrdl_regblock/cpuif/apb3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1309 2022-10-19 04:38:43.000000 peakrdl-regblock-0.8.0/src/peakrdl_regblock/cpuif/apb3/apb3_tmpl.sv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 04:38:44.754308 peakrdl-regblock-0.8.0/src/peakrdl_regblock/cpuif/apb4/
--rw-r--r--   0 runner    (1001) docker     (121)     1118 2022-10-19 04:38:43.000000 peakrdl-regblock-0.8.0/src/peakrdl_regblock/cpuif/apb4/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1486 2022-10-19 04:38:43.000000 peakrdl-regblock-0.8.0/src/peakrdl_regblock/cpuif/apb4/apb4_tmpl.sv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 04:38:44.754308 peakrdl-regblock-0.8.0/src/peakrdl_regblock/cpuif/axi4lite/
--rw-r--r--   0 runner    (1001) docker     (121)     2390 2022-10-19 04:38:43.000000 peakrdl-regblock-0.8.0/src/peakrdl_regblock/cpuif/axi4lite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8946 2022-10-19 04:38:43.000000 peakrdl-regblock-0.8.0/src/peakrdl_regblock/cpuif/axi4lite/axi4lite_tmpl.sv
--rw-r--r--   0 runner    (1001) docker     (121)     1976 2022-10-19 04:38:43.000000 peakrdl-regblock-0.8.0/src/peakrdl_regblock/cpuif/base.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 04:38:44.754308 peakrdl-regblock-0.8.0/src/peakrdl_regblock/cpuif/passthrough/
--rw-r--r--   0 runner    (1001) docker     (121)      835 2022-10-19 04:38:43.000000 peakrdl-regblock-0.8.0/src/peakrdl_regblock/cpuif/passthrough/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      484 2022-10-19 04:38:43.000000 peakrdl-regblock-0.8.0/src/peakrdl_regblock/cpuif/passthrough/passthrough_tmpl.sv
--rw-r--r--   0 runner    (1001) docker     (121)     7868 2022-10-19 04:38:43.000000 peakrdl-regblock-0.8.0/src/peakrdl_regblock/dereferencer.py
--rw-r--r--   0 runner    (1001) docker     (121)     7382 2022-10-19 04:38:43.000000 peakrdl-regblock-0.8.0/src/peakrdl_regblock/exporter.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 04:38:44.754308 peakrdl-regblock-0.8.0/src/peakrdl_regblock/field_logic/
--rw-r--r--   0 runner    (1001) docker     (121)    13757 2022-10-19 04:38:43.000000 peakrdl-regblock-0.8.0/src/peakrdl_regblock/field_logic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2884 2022-10-19 04:38:43.000000 peakrdl-regblock-0.8.0/src/peakrdl_regblock/field_logic/bases.py
--rw-r--r--   0 runner    (1001) docker     (121)    10463 2022-10-19 04:38:43.000000 peakrdl-regblock-0.8.0/src/peakrdl_regblock/field_logic/generators.py
--rw-r--r--   0 runner    (1001) docker     (121)     6452 2022-10-19 04:38:43.000000 peakrdl-regblock-0.8.0/src/peakrdl_regblock/field_logic/hw_interrupts.py
--rw-r--r--   0 runner    (1001) docker     (121)     2414 2022-10-19 04:38:43.000000 peakrdl-regblock-0.8.0/src/peakrdl_regblock/field_logic/hw_set_clr.py
--rw-r--r--   0 runner    (1001) docker     (121)     2437 2022-10-19 04:38:43.000000 peakrdl-regblock-0.8.0/src/peakrdl_regblock/field_logic/hw_write.py
--rw-r--r--   0 runner    (1001) docker     (121)     1018 2022-10-19 04:38:43.000000 peakrdl-regblock-0.8.0/src/peakrdl_regblock/field_logic/sw_onread.py
--rw-r--r--   0 runner    (1001) docker     (121)     5481 2022-10-19 04:38:43.000000 peakrdl-regblock-0.8.0/src/peakrdl_regblock/field_logic/sw_onwrite.py
--rw-r--r--   0 runner    (1001) docker     (121)      696 2022-10-19 04:38:43.000000 peakrdl-regblock-0.8.0/src/peakrdl_regblock/field_logic/sw_singlepulse.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 04:38:44.754308 peakrdl-regblock-0.8.0/src/peakrdl_regblock/field_logic/templates/
--rw-r--r--   0 runner    (1001) docker     (121)     3232 2022-10-19 04:38:43.000000 peakrdl-regblock-0.8.0/src/peakrdl_regblock/field_logic/templates/counter_macros.sv
--rw-r--r--   0 runner    (1001) docker     (121)     1641 2022-10-19 04:38:43.000000 peakrdl-regblock-0.8.0/src/peakrdl_regblock/field_logic/templates/field_storage.sv
--rw-r--r--   0 runner    (1001) docker     (121)     2559 2022-10-19 04:38:43.000000 peakrdl-regblock-0.8.0/src/peakrdl_regblock/forloop_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 04:38:44.754308 peakrdl-regblock-0.8.0/src/peakrdl_regblock/hwif/
--rw-r--r--   0 runner    (1001) docker     (121)     7000 2022-10-19 04:38:43.000000 peakrdl-regblock-0.8.0/src/peakrdl_regblock/hwif/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6328 2022-10-19 04:38:43.000000 peakrdl-regblock-0.8.0/src/peakrdl_regblock/hwif/generators.py
--rw-r--r--   0 runner    (1001) docker     (121)     3124 2022-10-19 04:38:43.000000 peakrdl-regblock-0.8.0/src/peakrdl_regblock/identifier_filter.py
--rw-r--r--   0 runner    (1001) docker     (121)     5446 2022-10-19 04:38:43.000000 peakrdl-regblock-0.8.0/src/peakrdl_regblock/module_tmpl.sv
--rw-r--r--   0 runner    (1001) docker     (121)      218 2022-10-19 04:38:43.000000 peakrdl-regblock-0.8.0/src/peakrdl_regblock/package_tmpl.sv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 04:38:44.754308 peakrdl-regblock-0.8.0/src/peakrdl_regblock/readback/
--rw-r--r--   0 runner    (1001) docker     (121)     2601 2022-10-19 04:38:43.000000 peakrdl-regblock-0.8.0/src/peakrdl_regblock/readback/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10533 2022-10-19 04:38:43.000000 peakrdl-regblock-0.8.0/src/peakrdl_regblock/readback/generators.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 04:38:44.758308 peakrdl-regblock-0.8.0/src/peakrdl_regblock/readback/templates/
--rw-r--r--   0 runner    (1001) docker     (121)     2315 2022-10-19 04:38:43.000000 peakrdl-regblock-0.8.0/src/peakrdl_regblock/readback/templates/readback.sv
--rw-r--r--   0 runner    (1001) docker     (121)     3899 2022-10-19 04:38:43.000000 peakrdl-regblock-0.8.0/src/peakrdl_regblock/scan_design.py
--rw-r--r--   0 runner    (1001) docker     (121)     7439 2022-10-19 04:38:43.000000 peakrdl-regblock-0.8.0/src/peakrdl_regblock/struct_generator.py
--rw-r--r--   0 runner    (1001) docker     (121)     4209 2022-10-19 04:38:43.000000 peakrdl-regblock-0.8.0/src/peakrdl_regblock/udps.py
--rw-r--r--   0 runner    (1001) docker     (121)     1698 2022-10-19 04:38:43.000000 peakrdl-regblock-0.8.0/src/peakrdl_regblock/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     4595 2022-10-19 04:38:43.000000 peakrdl-regblock-0.8.0/src/peakrdl_regblock/validate_design.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 04:38:44.754308 peakrdl-regblock-0.8.0/src/peakrdl_regblock.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1987 2022-10-19 04:38:44.000000 peakrdl-regblock-0.8.0/src/peakrdl_regblock.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2066 2022-10-19 04:38:44.000000 peakrdl-regblock-0.8.0/src/peakrdl_regblock.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-19 04:38:44.000000 peakrdl-regblock-0.8.0/src/peakrdl_regblock.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       69 2022-10-19 04:38:44.000000 peakrdl-regblock-0.8.0/src/peakrdl_regblock.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       40 2022-10-19 04:38:44.000000 peakrdl-regblock-0.8.0/src/peakrdl_regblock.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-10-19 04:38:44.000000 peakrdl-regblock-0.8.0/src/peakrdl_regblock.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 06:07:49.245975 peakrdl-regblock-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-11-10 06:07:48.000000 peakrdl-regblock-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       56 2022-11-10 06:07:48.000000 peakrdl-regblock-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     2038 2022-11-10 06:07:49.245975 peakrdl-regblock-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      745 2022-11-10 06:07:48.000000 peakrdl-regblock-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-10 06:07:49.245975 peakrdl-regblock-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2066 2022-11-10 06:07:48.000000 peakrdl-regblock-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 06:07:49.237975 peakrdl-regblock-0.9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 06:07:49.241975 peakrdl-regblock-0.9.0/src/peakrdl_regblock/
+-rw-r--r--   0 runner    (1001) docker     (121)       22 2022-11-10 06:07:48.000000 peakrdl-regblock-0.9.0/src/peakrdl_regblock/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       75 2022-11-10 06:07:48.000000 peakrdl-regblock-0.9.0/src/peakrdl_regblock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3573 2022-11-10 06:07:48.000000 peakrdl-regblock-0.9.0/src/peakrdl_regblock/__peakrdl__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4821 2022-11-10 06:07:48.000000 peakrdl-regblock-0.9.0/src/peakrdl_regblock/addr_decode.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 06:07:49.241975 peakrdl-regblock-0.9.0/src/peakrdl_regblock/cpuif/
+-rw-r--r--   0 runner    (1001) docker     (121)       28 2022-11-10 06:07:48.000000 peakrdl-regblock-0.9.0/src/peakrdl_regblock/cpuif/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 06:07:49.241975 peakrdl-regblock-0.9.0/src/peakrdl_regblock/cpuif/apb3/
+-rw-r--r--   0 runner    (1001) docker     (121)      981 2022-11-10 06:07:48.000000 peakrdl-regblock-0.9.0/src/peakrdl_regblock/cpuif/apb3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1309 2022-11-10 06:07:48.000000 peakrdl-regblock-0.9.0/src/peakrdl_regblock/cpuif/apb3/apb3_tmpl.sv
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 06:07:49.241975 peakrdl-regblock-0.9.0/src/peakrdl_regblock/cpuif/apb4/
+-rw-r--r--   0 runner    (1001) docker     (121)     1118 2022-11-10 06:07:48.000000 peakrdl-regblock-0.9.0/src/peakrdl_regblock/cpuif/apb4/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1486 2022-11-10 06:07:48.000000 peakrdl-regblock-0.9.0/src/peakrdl_regblock/cpuif/apb4/apb4_tmpl.sv
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 06:07:49.241975 peakrdl-regblock-0.9.0/src/peakrdl_regblock/cpuif/axi4lite/
+-rw-r--r--   0 runner    (1001) docker     (121)     2390 2022-11-10 06:07:48.000000 peakrdl-regblock-0.9.0/src/peakrdl_regblock/cpuif/axi4lite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8946 2022-11-10 06:07:48.000000 peakrdl-regblock-0.9.0/src/peakrdl_regblock/cpuif/axi4lite/axi4lite_tmpl.sv
+-rw-r--r--   0 runner    (1001) docker     (121)     1976 2022-11-10 06:07:48.000000 peakrdl-regblock-0.9.0/src/peakrdl_regblock/cpuif/base.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 06:07:49.241975 peakrdl-regblock-0.9.0/src/peakrdl_regblock/cpuif/passthrough/
+-rw-r--r--   0 runner    (1001) docker     (121)      835 2022-11-10 06:07:48.000000 peakrdl-regblock-0.9.0/src/peakrdl_regblock/cpuif/passthrough/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      484 2022-11-10 06:07:48.000000 peakrdl-regblock-0.9.0/src/peakrdl_regblock/cpuif/passthrough/passthrough_tmpl.sv
+-rw-r--r--   0 runner    (1001) docker     (121)     8074 2022-11-10 06:07:48.000000 peakrdl-regblock-0.9.0/src/peakrdl_regblock/dereferencer.py
+-rw-r--r--   0 runner    (1001) docker     (121)      500 2022-11-10 06:07:48.000000 peakrdl-regblock-0.9.0/src/peakrdl_regblock/entry_points.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8444 2022-11-10 06:07:48.000000 peakrdl-regblock-0.9.0/src/peakrdl_regblock/exporter.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 06:07:49.241975 peakrdl-regblock-0.9.0/src/peakrdl_regblock/field_logic/
+-rw-r--r--   0 runner    (1001) docker     (121)    16834 2022-11-10 06:07:48.000000 peakrdl-regblock-0.9.0/src/peakrdl_regblock/field_logic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2884 2022-11-10 06:07:48.000000 peakrdl-regblock-0.9.0/src/peakrdl_regblock/field_logic/bases.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11156 2022-11-10 06:07:48.000000 peakrdl-regblock-0.9.0/src/peakrdl_regblock/field_logic/generators.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6452 2022-11-10 06:07:48.000000 peakrdl-regblock-0.9.0/src/peakrdl_regblock/field_logic/hw_interrupts.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2414 2022-11-10 06:07:48.000000 peakrdl-regblock-0.9.0/src/peakrdl_regblock/field_logic/hw_set_clr.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2437 2022-11-10 06:07:48.000000 peakrdl-regblock-0.9.0/src/peakrdl_regblock/field_logic/hw_write.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1276 2022-11-10 06:07:48.000000 peakrdl-regblock-0.9.0/src/peakrdl_regblock/field_logic/sw_onread.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7751 2022-11-10 06:07:48.000000 peakrdl-regblock-0.9.0/src/peakrdl_regblock/field_logic/sw_onwrite.py
+-rw-r--r--   0 runner    (1001) docker     (121)      696 2022-11-10 06:07:48.000000 peakrdl-regblock-0.9.0/src/peakrdl_regblock/field_logic/sw_singlepulse.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 06:07:49.241975 peakrdl-regblock-0.9.0/src/peakrdl_regblock/field_logic/templates/
+-rw-r--r--   0 runner    (1001) docker     (121)     3232 2022-11-10 06:07:48.000000 peakrdl-regblock-0.9.0/src/peakrdl_regblock/field_logic/templates/counter_macros.sv
+-rw-r--r--   0 runner    (1001) docker     (121)     1641 2022-11-10 06:07:48.000000 peakrdl-regblock-0.9.0/src/peakrdl_regblock/field_logic/templates/field_storage.sv
+-rw-r--r--   0 runner    (1001) docker     (121)     2559 2022-11-10 06:07:48.000000 peakrdl-regblock-0.9.0/src/peakrdl_regblock/forloop_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 06:07:49.245975 peakrdl-regblock-0.9.0/src/peakrdl_regblock/hwif/
+-rw-r--r--   0 runner    (1001) docker     (121)     7115 2022-11-10 06:07:48.000000 peakrdl-regblock-0.9.0/src/peakrdl_regblock/hwif/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7560 2022-11-10 06:07:48.000000 peakrdl-regblock-0.9.0/src/peakrdl_regblock/hwif/generators.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3124 2022-11-10 06:07:48.000000 peakrdl-regblock-0.9.0/src/peakrdl_regblock/identifier_filter.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6127 2022-11-10 06:07:48.000000 peakrdl-regblock-0.9.0/src/peakrdl_regblock/module_tmpl.sv
+-rw-r--r--   0 runner    (1001) docker     (121)      218 2022-11-10 06:07:48.000000 peakrdl-regblock-0.9.0/src/peakrdl_regblock/package_tmpl.sv
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 06:07:49.245975 peakrdl-regblock-0.9.0/src/peakrdl_regblock/read_buffering/
+-rw-r--r--   0 runner    (1001) docker     (121)     2050 2022-11-10 06:07:48.000000 peakrdl-regblock-0.9.0/src/peakrdl_regblock/read_buffering/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1754 2022-11-10 06:07:48.000000 peakrdl-regblock-0.9.0/src/peakrdl_regblock/read_buffering/implementation_generator.py
+-rw-r--r--   0 runner    (1001) docker     (121)      510 2022-11-10 06:07:48.000000 peakrdl-regblock-0.9.0/src/peakrdl_regblock/read_buffering/storage_generator.py
+-rw-r--r--   0 runner    (1001) docker     (121)      128 2022-11-10 06:07:48.000000 peakrdl-regblock-0.9.0/src/peakrdl_regblock/read_buffering/template.sv
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 06:07:49.245975 peakrdl-regblock-0.9.0/src/peakrdl_regblock/readback/
+-rw-r--r--   0 runner    (1001) docker     (121)     2601 2022-11-10 06:07:48.000000 peakrdl-regblock-0.9.0/src/peakrdl_regblock/readback/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15321 2022-11-10 06:07:48.000000 peakrdl-regblock-0.9.0/src/peakrdl_regblock/readback/generators.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 06:07:49.245975 peakrdl-regblock-0.9.0/src/peakrdl_regblock/readback/templates/
+-rw-r--r--   0 runner    (1001) docker     (121)     2319 2022-11-10 06:07:48.000000 peakrdl-regblock-0.9.0/src/peakrdl_regblock/readback/templates/readback.sv
+-rw-r--r--   0 runner    (1001) docker     (121)     4211 2022-11-10 06:07:48.000000 peakrdl-regblock-0.9.0/src/peakrdl_regblock/scan_design.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7439 2022-11-10 06:07:48.000000 peakrdl-regblock-0.9.0/src/peakrdl_regblock/struct_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 06:07:49.245975 peakrdl-regblock-0.9.0/src/peakrdl_regblock/udps/
+-rw-r--r--   0 runner    (1001) docker     (121)      281 2022-11-10 06:07:48.000000 peakrdl-regblock-0.9.0/src/peakrdl_regblock/udps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      551 2022-11-10 06:07:48.000000 peakrdl-regblock-0.9.0/src/peakrdl_regblock/udps/extended_swacc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4486 2022-11-10 06:07:48.000000 peakrdl-regblock-0.9.0/src/peakrdl_regblock/udps/rw_buffering.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1698 2022-11-10 06:07:48.000000 peakrdl-regblock-0.9.0/src/peakrdl_regblock/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5094 2022-11-10 06:07:48.000000 peakrdl-regblock-0.9.0/src/peakrdl_regblock/validate_design.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 06:07:49.245975 peakrdl-regblock-0.9.0/src/peakrdl_regblock/write_buffering/
+-rw-r--r--   0 runner    (1001) docker     (121)     2893 2022-11-10 06:07:48.000000 peakrdl-regblock-0.9.0/src/peakrdl_regblock/write_buffering/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2261 2022-11-10 06:07:48.000000 peakrdl-regblock-0.9.0/src/peakrdl_regblock/write_buffering/implementation_generator.py
+-rw-r--r--   0 runner    (1001) docker     (121)      941 2022-11-10 06:07:48.000000 peakrdl-regblock-0.9.0/src/peakrdl_regblock/write_buffering/storage_generator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1210 2022-11-10 06:07:48.000000 peakrdl-regblock-0.9.0/src/peakrdl_regblock/write_buffering/template.sv
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 06:07:49.241975 peakrdl-regblock-0.9.0/src/peakrdl_regblock.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     2038 2022-11-10 06:07:49.000000 peakrdl-regblock-0.9.0/src/peakrdl_regblock.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2636 2022-11-10 06:07:49.000000 peakrdl-regblock-0.9.0/src/peakrdl_regblock.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-10 06:07:49.000000 peakrdl-regblock-0.9.0/src/peakrdl_regblock.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       69 2022-11-10 06:07:49.000000 peakrdl-regblock-0.9.0/src/peakrdl_regblock.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       40 2022-11-10 06:07:49.000000 peakrdl-regblock-0.9.0/src/peakrdl_regblock.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       17 2022-11-10 06:07:49.000000 peakrdl-regblock-0.9.0/src/peakrdl_regblock.egg-info/top_level.txt
```

### Comparing `peakrdl-regblock-0.8.0/LICENSE` & `peakrdl-regblock-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `peakrdl-regblock-0.8.0/PKG-INFO` & `peakrdl-regblock-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peakrdl-regblock
-Version: 0.8.0
+Version: 0.9.0
 Summary: Compile SystemRDL into a SystemVerilog control/status register (CSR) block
 Home-page: https://github.com/SystemRDL/PeakRDL-regblock
 Author: Alex Mykyta
 Author-email: amykyta3@github.com
 Project-URL: Documentation, http://peakrdl-regblock.readthedocs.io
 Project-URL: Source, https://github.com/SystemRDL/PeakRDL-regblock
 Project-URL: Tracker, https://github.com/SystemRDL/PeakRDL-regblock/issues
@@ -12,14 +12,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `peakrdl-regblock-0.8.0/README.md` & `peakrdl-regblock-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `peakrdl-regblock-0.8.0/setup.py` & `peakrdl-regblock-0.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     long_description_content_type="text/markdown",
     url="https://github.com/SystemRDL/PeakRDL-regblock",
     package_dir={'': 'src'},
     packages=setuptools.find_packages("src"),
     include_package_data=True,
     python_requires='>=3.6',
     install_requires=[
-        "systemrdl-compiler>=1.25.0",
+        "systemrdl-compiler>=1.25.1",
         "Jinja2>=2.11",
     ],
     entry_points = {
         "peakrdl.exporters": [
             'regblock = peakrdl_regblock.__peakrdl__:Exporter'
         ]
     },
@@ -38,14 +38,15 @@
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3 :: Only",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Operating System :: OS Independent",
         "Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)",
     ),
     project_urls={
```

### Comparing `peakrdl-regblock-0.8.0/src/peakrdl_regblock/__peakrdl__.py` & `peakrdl-regblock-0.9.0/src/peakrdl_regblock/__peakrdl__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,39 @@
 from typing import TYPE_CHECKING
 
 from .exporter import RegblockExporter
-from .cpuif import apb3, apb4, axi4lite, passthrough
+from .cpuif import apb3, apb4, axi4lite, passthrough, CpuifBase
 from .udps import ALL_UDPS
+from . import entry_points
 
 if TYPE_CHECKING:
     import argparse
     from systemrdl.node import AddrmapNode
 
 
-# TODO: make this user-extensible
 CPUIF_DICT = {
     "apb3": apb3.APB3_Cpuif,
     "apb3-flat": apb3.APB3_Cpuif_flattened,
     "apb4": apb4.APB4_Cpuif,
     "apb4-flat": apb4.APB4_Cpuif_flattened,
     "axi4-lite": axi4lite.AXI4Lite_Cpuif,
     "axi4-lite-flat": axi4lite.AXI4Lite_Cpuif_flattened,
     "passthrough": passthrough.PassthroughCpuif
 }
 
+# Load any user-plugins
+for ep in entry_points.get_entry_points("peakrdl_regblock.cpuif"): # type: ignore
+    name = ep.name
+    cpuif = ep.load()
+    if name in CPUIF_DICT:
+        raise RuntimeError(f"A plugin for 'peakrdl-regblock' tried to load cpuif '{name}' but it already exists")
+    if not issubclass(cpuif, CpuifBase):
+        raise RuntimeError(f"A plugin for 'peakrdl-regblock' tried to load cpuif '{name}' but it not a CpuifBase class")
+    CPUIF_DICT[name] = cpuif
+
 
 class Exporter:
     short_desc = "Generate a SystemVerilog control/status register (CSR) block"
 
     udp_definitions = ALL_UDPS
 
     def add_exporter_arguments(self, arg_group: 'argparse.ArgumentParser') -> None:
@@ -67,21 +77,28 @@
             default="lexical",
             help="""Choose how HWIF struct type names are generated.
             The 'lexical' style will use RDL lexical scope & type names where
             possible and attempt to re-use equivalent type definitions.
             The 'hier' style uses component's hierarchy as the struct type name. [lexical]
             """
         )
+        arg_group.add_argument(
+            "--hwif-report",
+            action="store_true",
+            default=False,
+            help="Generate a HWIF report file"
+        )
 
 
     def do_export(self, top_node: 'AddrmapNode', options: 'argparse.Namespace') -> None:
         x = RegblockExporter()
         x.export(
             top_node,
             options.output,
             cpuif_cls=CPUIF_DICT[options.cpuif],
             module_name=options.module_name,
             package_name=options.package_name,
             reuse_hwif_typedefs=(options.type_style == "lexical"),
             retime_read_fanin=options.rt_read_fanin,
             retime_read_response=options.rt_read_response,
+            generate_hwif_report=options.hwif_report,
         )
```

### Comparing `peakrdl-regblock-0.8.0/src/peakrdl_regblock/addr_decode.py` & `peakrdl-regblock-0.9.0/src/peakrdl_regblock/addr_decode.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,14 +116,15 @@
         regwidth = node.get_property('regwidth')
         accesswidth = node.get_property('accesswidth')
 
         if regwidth == accesswidth:
             s = f"{self.addr_decode.get_access_strobe(node)} = cpuif_req_masked & (cpuif_addr == {self._get_address_str(node)});"
             self.add_content(s)
         else:
+            # Register is wide. Create a substrobe for each subword
             n_subwords = regwidth // accesswidth
             subword_stride = accesswidth // 8
             for i in range(n_subwords):
                 s = f"{self.addr_decode.get_access_strobe(node)}[{i}] = cpuif_req_masked & (cpuif_addr == {self._get_address_str(node, subword_offset=(i*subword_stride))});"
                 self.add_content(s)
```

### Comparing `peakrdl-regblock-0.8.0/src/peakrdl_regblock/cpuif/apb3/__init__.py` & `peakrdl-regblock-0.9.0/src/peakrdl_regblock/cpuif/apb3/__init__.py`

 * *Files identical despite different names*

### Comparing `peakrdl-regblock-0.8.0/src/peakrdl_regblock/cpuif/apb3/apb3_tmpl.sv` & `peakrdl-regblock-0.9.0/src/peakrdl_regblock/cpuif/apb3/apb3_tmpl.sv`

 * *Files identical despite different names*

### Comparing `peakrdl-regblock-0.8.0/src/peakrdl_regblock/cpuif/apb4/__init__.py` & `peakrdl-regblock-0.9.0/src/peakrdl_regblock/cpuif/apb4/__init__.py`

 * *Files identical despite different names*

### Comparing `peakrdl-regblock-0.8.0/src/peakrdl_regblock/cpuif/apb4/apb4_tmpl.sv` & `peakrdl-regblock-0.9.0/src/peakrdl_regblock/cpuif/apb4/apb4_tmpl.sv`

 * *Files identical despite different names*

### Comparing `peakrdl-regblock-0.8.0/src/peakrdl_regblock/cpuif/axi4lite/__init__.py` & `peakrdl-regblock-0.9.0/src/peakrdl_regblock/cpuif/axi4lite/__init__.py`

 * *Files identical despite different names*

### Comparing `peakrdl-regblock-0.8.0/src/peakrdl_regblock/cpuif/axi4lite/axi4lite_tmpl.sv` & `peakrdl-regblock-0.9.0/src/peakrdl_regblock/cpuif/axi4lite/axi4lite_tmpl.sv`

 * *Files identical despite different names*

### Comparing `peakrdl-regblock-0.8.0/src/peakrdl_regblock/cpuif/base.py` & `peakrdl-regblock-0.9.0/src/peakrdl_regblock/cpuif/base.py`

 * *Files identical despite different names*

### Comparing `peakrdl-regblock-0.8.0/src/peakrdl_regblock/cpuif/passthrough/__init__.py` & `peakrdl-regblock-0.9.0/src/peakrdl_regblock/cpuif/passthrough/__init__.py`

 * *Files identical despite different names*

### Comparing `peakrdl-regblock-0.8.0/src/peakrdl_regblock/dereferencer.py` & `peakrdl-regblock-0.9.0/src/peakrdl_regblock/dereferencer.py`

 * *Files 2% similar despite different names*

```diff
@@ -157,14 +157,18 @@
             else:
                 return self.get_value(prop_value)
 
         if prop_name == "swacc":
             return self.field_logic.get_swacc_identifier(field)
         if prop_name == "swmod":
             return self.field_logic.get_swmod_identifier(field)
+        if prop_name == "rd_swacc":
+            return self.field_logic.get_rd_swacc_identifier(field)
+        if prop_name == "wr_swacc":
+            return self.field_logic.get_wr_swacc_identifier(field)
 
 
         # translate aliases
         aliases = {
             "saturate": "incrsaturate",
             "threshold": "incrthreshold",
         }
```

### Comparing `peakrdl-regblock-0.8.0/src/peakrdl_regblock/exporter.py` & `peakrdl-regblock-0.9.0/src/peakrdl_regblock/exporter.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,34 +6,38 @@
 
 from .addr_decode import AddressDecode
 from .field_logic import FieldLogic
 from .dereferencer import Dereferencer
 from .readback import Readback
 from .identifier_filter import kw_filter as kwf
 
-from .cpuif import CpuifBase
-from .cpuif.apb4 import APB4_Cpuif
-from .hwif import Hwif
 from .utils import get_always_ff_event
 from .scan_design import DesignScanner
 from .validate_design import DesignValidator
+from .cpuif import CpuifBase
+from .cpuif.apb4 import APB4_Cpuif
+from .hwif import Hwif
+from .write_buffering import WriteBuffering
+from .read_buffering import ReadBuffering
 
 class RegblockExporter:
     def __init__(self, **kwargs: Any) -> None:
         # Check for stray kwargs
         if kwargs:
             raise TypeError(f"got an unexpected keyword argument '{list(kwargs.keys())[0]}'")
 
 
         self.top_node = None # type: AddrmapNode
         self.hwif = None # type: Hwif
         self.cpuif = None # type: CpuifBase
         self.address_decode = AddressDecode(self)
         self.field_logic = FieldLogic(self)
         self.readback = None # type: Readback
+        self.write_buffering = WriteBuffering(self)
+        self.read_buffering = ReadBuffering(self)
         self.dereferencer = Dereferencer(self)
         self.min_read_latency = 0
         self.min_write_latency = 0
 
         loader = jj.ChoiceLoader([
             jj.FileSystemLoader(os.path.dirname(__file__)),
             jj.PrefixLoader({
@@ -89,26 +93,30 @@
             response logic fully combinationally. Enabling this stage can better
             isolate timing paths in the register file from the rest of your system.
 
             Enabling this when using CPU interfaces that already implement the
             response path sequentially may not result in any meaningful timing improvement.
 
             Enabling this option will increase read transfer latency by 1 clock cycle.
+        generate_hwif_report: bool
+            If set, generates a hwif report that can help understand the structure
+            of the hwif_in and hwif_out structures.
         """
         # If it is the root node, skip to top addrmap
         if isinstance(node, RootNode):
             self.top_node = node.top
         else:
             self.top_node = node
 
 
         cpuif_cls = kwargs.pop("cpuif_cls", None) or APB4_Cpuif # type: Type[CpuifBase]
         module_name = kwargs.pop("module_name", None) or kwf(self.top_node.inst_name) # type: str
         package_name = kwargs.pop("package_name", None) or (module_name + "_pkg") # type: str
         reuse_hwif_typedefs = kwargs.pop("reuse_hwif_typedefs", True) # type: bool
+        generate_hwif_report = kwargs.pop("generate_hwif_report", False) # type: bool
 
         # Pipelining options
         retime_read_fanin = kwargs.pop("retime_read_fanin", False) # type: bool
         retime_read_response = kwargs.pop("retime_read_response", True) # type: bool
 
         # Check for stray kwargs
         if kwargs:
@@ -121,27 +129,34 @@
         if retime_read_response:
             self.min_read_latency += 1
 
         # Scan the design for pre-export information
         scanner = DesignScanner(self)
         scanner.do_scan()
 
+        if generate_hwif_report:
+            path = os.path.join(output_dir, f"{module_name}_hwif.rpt")
+            hwif_report_file = open(path, "w", encoding='utf-8') # pylint: disable=consider-using-with
+        else:
+            hwif_report_file = None
+
         # Construct exporter components
         self.cpuif = cpuif_cls(
             self,
             cpuif_reset=self.top_node.cpuif_reset,
             data_width=scanner.cpuif_data_width,
             addr_width=self.top_node.size.bit_length()
         )
         self.hwif = Hwif(
             self,
             package_name=package_name,
             in_hier_signal_paths=scanner.in_hier_signal_paths,
             out_of_hier_signals=scanner.out_of_hier_signals,
             reuse_typedefs=reuse_hwif_typedefs,
+            hwif_report_file=hwif_report_file,
         )
         self.readback = Readback(
             self,
             retime_read_fanin
         )
 
         # Validate that there are no unsupported constructs
@@ -149,16 +164,20 @@
         validator.do_validate()
 
         # Build Jinja template context
         context = {
             "module_name": module_name,
             "user_out_of_hier_signals": scanner.out_of_hier_signals.values(),
             "has_writable_msb0_fields": scanner.has_writable_msb0_fields,
+            "has_buffered_write_regs": scanner.has_buffered_write_regs,
+            "has_buffered_read_regs": scanner.has_buffered_read_regs,
             "cpuif": self.cpuif,
             "hwif": self.hwif,
+            "write_buffering": self.write_buffering,
+            "read_buffering": self.read_buffering,
             "get_resetsignal": self.dereferencer.get_resetsignal,
             "address_decode": self.address_decode,
             "field_logic": self.field_logic,
             "readback": self.readback,
             "get_always_ff_event": lambda resetsignal : get_always_ff_event(self.dereferencer, resetsignal),
             "retime_read_response": retime_read_response,
             "min_read_latency": self.min_read_latency,
@@ -172,7 +191,10 @@
         stream = template.stream(context)
         stream.dump(package_file_path)
 
         module_file_path = os.path.join(output_dir, module_name + ".sv")
         template = self.jj_env.get_template("module_tmpl.sv")
         stream = template.stream(context)
         stream.dump(module_file_path)
+
+        if hwif_report_file:
+            hwif_report_file.close()
```

### Comparing `peakrdl-regblock-0.8.0/src/peakrdl_regblock/field_logic/__init__.py` & `peakrdl-regblock-0.9.0/src/peakrdl_regblock/field_logic/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from typing import TYPE_CHECKING
 
-from systemrdl.rdltypes import PropertyReference, PrecedenceType, InterruptType
-from systemrdl.node import Node
+from systemrdl.rdltypes import PrecedenceType, InterruptType
 
 from .bases import AssignmentPrecedence, NextStateConditional
 from . import sw_onread
 from . import sw_onwrite
 from . import sw_singlepulse
 from . import hw_write
 from . import hw_set_clr
@@ -170,39 +169,107 @@
         if isinstance(prop_value, bool):
             # No explicit value set. use min
             return "'d0"
         return self.exp.dereferencer.get_value(prop_value)
 
     def get_swacc_identifier(self, field: 'FieldNode') -> str:
         """
+        Asserted when field is software accessed (read or write)
+        """
+        buffer_reads = field.parent.get_property('buffer_reads')
+        buffer_writes = field.parent.get_property('buffer_writes')
+        if buffer_reads and buffer_writes:
+            rstrb = self.exp.read_buffering.get_trigger(field.parent)
+            wstrb = self.exp.write_buffering.get_write_strobe(field)
+            return f"{rstrb} || {wstrb}"
+        elif buffer_reads and not buffer_writes:
+            strb = self.exp.dereferencer.get_access_strobe(field)
+            rstrb = self.exp.read_buffering.get_trigger(field.parent)
+            return f"{rstrb} || ({strb} && decoded_req_is_wr)"
+        elif not buffer_reads and buffer_writes:
+            strb = self.exp.dereferencer.get_access_strobe(field)
+            wstrb = self.exp.write_buffering.get_write_strobe(field)
+            return f"{wstrb} || ({strb} && !decoded_req_is_wr)"
+        else:
+            strb = self.exp.dereferencer.get_access_strobe(field)
+            return strb
+
+    def get_rd_swacc_identifier(self, field: 'FieldNode') -> str:
+        """
         Asserted when field is software accessed (read)
         """
-        strb = self.exp.dereferencer.get_access_strobe(field)
-        return f"{strb} && !decoded_req_is_wr"
+        buffer_reads = field.parent.get_property('buffer_reads')
+        if buffer_reads:
+            rstrb = self.exp.read_buffering.get_trigger(field.parent)
+            return rstrb
+        else:
+            strb = self.exp.dereferencer.get_access_strobe(field)
+            return f"{strb} && !decoded_req_is_wr"
+
+    def get_wr_swacc_identifier(self, field: 'FieldNode') -> str:
+        """
+        Asserted when field is software accessed (write)
+        """
+        buffer_writes = field.parent.get_property('buffer_writes')
+        if buffer_writes:
+            wstrb = self.exp.write_buffering.get_write_strobe(field)
+            return wstrb
+        else:
+            strb = self.exp.dereferencer.get_access_strobe(field)
+            return f"{strb} && decoded_req_is_wr"
 
     def get_swmod_identifier(self, field: 'FieldNode') -> str:
         """
         Asserted when field is modified by software (written or read with a
         set or clear side effect).
         """
         w_modifiable = field.is_sw_writable
         r_modifiable = (field.get_property('onread') is not None)
-        strb = self.exp.dereferencer.get_access_strobe(field)
+        buffer_writes = field.parent.get_property('buffer_writes')
+        buffer_reads = field.parent.get_property('buffer_reads')
 
         if w_modifiable and not r_modifiable:
             # assert swmod only on sw write
-            return f"{strb} && decoded_req_is_wr"
+            if buffer_writes:
+                # Write strobe arrives from buffer layer instead
+                wstrb = self.exp.write_buffering.get_write_strobe(field)
+                return wstrb
+            else:
+                # Unbuffered. Use decoder strobe directly
+                astrb = self.exp.dereferencer.get_access_strobe(field)
+                return f"{astrb} && decoded_req_is_wr"
 
         if w_modifiable and r_modifiable:
-            # assert swmod on all sw actions
-            return strb
+            # assert swmod on both sw read and write
+            astrb = self.exp.dereferencer.get_access_strobe(field)
+            if buffer_writes or buffer_reads:
+                if buffer_reads:
+                    rstrb = self.exp.read_buffering.get_trigger(field.parent)
+                else:
+                    rstrb = f"{astrb} && !decoded_req_is_wr"
+
+                if buffer_writes:
+                    wstrb = self.exp.write_buffering.get_write_strobe(field)
+                else:
+                    wstrb = f"{astrb} && decoded_req_is_wr"
+
+                return f"{wstrb} || {rstrb}"
+            else:
+                # Unbuffered. Use decoder strobe directly
+                astrb = self.exp.dereferencer.get_access_strobe(field)
+                return astrb
 
         if not w_modifiable and r_modifiable:
             # assert swmod only on sw read
-            return f"{strb} && !decoded_req_is_wr"
+            astrb = self.exp.dereferencer.get_access_strobe(field)
+            if buffer_reads:
+                rstrb = self.exp.read_buffering.get_trigger(field.parent)
+            else:
+                rstrb = f"{astrb} && !decoded_req_is_wr"
+            return rstrb
 
         # Not sw modifiable
         return "1'b0"
 
 
     def has_next_q(self, field: 'FieldNode') -> bool:
         """
```

### Comparing `peakrdl-regblock-0.8.0/src/peakrdl_regblock/field_logic/bases.py` & `peakrdl-regblock-0.9.0/src/peakrdl_regblock/field_logic/bases.py`

 * *Files identical despite different names*

### Comparing `peakrdl-regblock-0.8.0/src/peakrdl_regblock/field_logic/generators.py` & `peakrdl-regblock-0.9.0/src/peakrdl_regblock/field_logic/generators.py`

 * *Files 3% similar despite different names*

```diff
@@ -81,15 +81,15 @@
 
 class FieldLogicGenerator(RDLForLoopGenerator):
     i_type = "genvar"
     def __init__(self, field_logic: 'FieldLogic') -> None:
         super().__init__()
         self.field_logic = field_logic
         self.exp = field_logic.exp
-        self.field_storage_template = self.field_logic.exp.jj_env.get_template(
+        self.field_storage_template = self.exp.jj_env.get_template(
             "field_logic/templates/field_storage.sv"
         )
         self.intr_fields = [] # type: List[FieldNode]
         self.halt_fields = [] # type: List[FieldNode]
 
 
     def enter_Reg(self, node: 'RegNode') -> None:
@@ -220,41 +220,55 @@
         if node.get_property('xored'):
             output_identifier = self.exp.hwif.get_implied_prop_output_identifier(node, "xored")
             value = self.exp.dereferencer.get_field_propref_value(node, "xored")
             self.add_content(
                 f"assign {output_identifier} = {value};"
             )
 
+        # Software access strobes
         if node.get_property('swmod'):
             output_identifier = self.exp.hwif.get_implied_prop_output_identifier(node, "swmod")
             value = self.field_logic.get_swmod_identifier(node)
             self.add_content(
                 f"assign {output_identifier} = {value};"
             )
-
         if node.get_property('swacc'):
             output_identifier = self.exp.hwif.get_implied_prop_output_identifier(node, "swacc")
             value = self.field_logic.get_swacc_identifier(node)
             self.add_content(
                 f"assign {output_identifier} = {value};"
             )
+        if node.get_property('rd_swacc'):
+            output_identifier = self.exp.hwif.get_implied_prop_output_identifier(node, "rd_swacc")
+            value = self.field_logic.get_rd_swacc_identifier(node)
+            self.add_content(
+                f"assign {output_identifier} = {value};"
+            )
+        if node.get_property('wr_swacc'):
+            output_identifier = self.exp.hwif.get_implied_prop_output_identifier(node, "wr_swacc")
+            value = self.field_logic.get_wr_swacc_identifier(node)
+            self.add_content(
+                f"assign {output_identifier} = {value};"
+            )
 
+        # Counter thresholds
         if node.get_property('incrthreshold') is not False: # (explicitly not False. Not 0)
             output_identifier = self.exp.hwif.get_implied_prop_output_identifier(node, "incrthreshold")
             value = self.field_logic.get_field_combo_identifier(node, 'incrthreshold')
             self.add_content(
                 f"assign {output_identifier} = {value};"
             )
         if node.get_property('decrthreshold') is not False: # (explicitly not False. Not 0)
             output_identifier = self.exp.hwif.get_implied_prop_output_identifier(node, "decrthreshold")
             value = self.field_logic.get_field_combo_identifier(node, 'decrthreshold')
             self.add_content(
                 f"assign {output_identifier} = {value};"
             )
 
+        # Counter events
         if node.get_property('overflow'):
             output_identifier = self.exp.hwif.get_implied_prop_output_identifier(node, "overflow")
             value = self.field_logic.get_field_combo_identifier(node, 'overflow')
             self.add_content(
                 f"assign {output_identifier} = {value};"
             )
         if node.get_property('underflow'):
```

### Comparing `peakrdl-regblock-0.8.0/src/peakrdl_regblock/field_logic/hw_interrupts.py` & `peakrdl-regblock-0.9.0/src/peakrdl_regblock/field_logic/hw_interrupts.py`

 * *Files identical despite different names*

### Comparing `peakrdl-regblock-0.8.0/src/peakrdl_regblock/field_logic/hw_set_clr.py` & `peakrdl-regblock-0.9.0/src/peakrdl_regblock/field_logic/hw_set_clr.py`

 * *Files identical despite different names*

### Comparing `peakrdl-regblock-0.8.0/src/peakrdl_regblock/field_logic/hw_write.py` & `peakrdl-regblock-0.9.0/src/peakrdl_regblock/field_logic/hw_write.py`

 * *Files identical despite different names*

### Comparing `peakrdl-regblock-0.8.0/src/peakrdl_regblock/field_logic/sw_onread.py` & `peakrdl-regblock-0.9.0/src/peakrdl_regblock/field_logic/sw_onread.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,16 +9,22 @@
 
 class _OnRead(NextStateConditional):
     onreadtype = None
     def is_match(self, field: 'FieldNode') -> bool:
         return field.get_property('onread') == self.onreadtype
 
     def get_predicate(self, field: 'FieldNode') -> str:
-        strb = self.exp.dereferencer.get_access_strobe(field)
-        return f"{strb} && !decoded_req_is_wr"
+        if field.parent.get_property('buffer_reads'):
+            # Is buffered read. Use alternate strobe
+            rstrb = self.exp.read_buffering.get_trigger(field.parent)
+            return rstrb
+        else:
+            # is regular register
+            strb = self.exp.dereferencer.get_access_strobe(field)
+            return f"{strb} && !decoded_req_is_wr"
 
 
 class ClearOnRead(_OnRead):
     comment = "SW clear on read"
     onreadtype = OnReadType.rclr
 
     def get_assignments(self, field: 'FieldNode') -> List[str]:
```

### Comparing `peakrdl-regblock-0.8.0/src/peakrdl_regblock/field_logic/sw_singlepulse.py` & `peakrdl-regblock-0.9.0/src/peakrdl_regblock/field_logic/sw_singlepulse.py`

 * *Files identical despite different names*

### Comparing `peakrdl-regblock-0.8.0/src/peakrdl_regblock/field_logic/templates/counter_macros.sv` & `peakrdl-regblock-0.9.0/src/peakrdl_regblock/field_logic/templates/counter_macros.sv`

 * *Files identical despite different names*

### Comparing `peakrdl-regblock-0.8.0/src/peakrdl_regblock/field_logic/templates/field_storage.sv` & `peakrdl-regblock-0.9.0/src/peakrdl_regblock/field_logic/templates/field_storage.sv`

 * *Files identical despite different names*

### Comparing `peakrdl-regblock-0.8.0/src/peakrdl_regblock/forloop_generator.py` & `peakrdl-regblock-0.9.0/src/peakrdl_regblock/forloop_generator.py`

 * *Files identical despite different names*

### Comparing `peakrdl-regblock-0.8.0/src/peakrdl_regblock/hwif/__init__.py` & `peakrdl-regblock-0.9.0/src/peakrdl_regblock/hwif/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from typing import TYPE_CHECKING, Union, List, Set, Dict
+from typing import TYPE_CHECKING, Union, Set, Dict, Optional, TextIO
 
-from systemrdl.node import AddrmapNode, Node, SignalNode, FieldNode, AddressableNode, RegNode
+from systemrdl.node import AddrmapNode, SignalNode, FieldNode, RegNode
 from systemrdl.rdltypes import PropertyReference
 
 from ..utils import get_indexed_path
 from ..identifier_filter import kw_filter as kwf
 
 from .generators import InputStructGenerator_Hier, OutputStructGenerator_Hier
 from .generators import InputStructGenerator_TypeScope, OutputStructGenerator_TypeScope
@@ -19,25 +19,27 @@
     - Field inputs
     - Signal inputs (except those that are promoted to the top)
     """
 
     def __init__(
         self, exp: 'RegblockExporter', package_name: str,
         in_hier_signal_paths: Set[str], out_of_hier_signals: Dict[str, SignalNode],
-        reuse_typedefs: bool
+        reuse_typedefs: bool, hwif_report_file: Optional[TextIO]
     ):
         self.exp = exp
         self.package_name = package_name
 
         self.has_input_struct = False
         self.has_output_struct = False
 
         self.in_hier_signal_paths = in_hier_signal_paths
         self.out_of_hier_signals = out_of_hier_signals
 
+        self.hwif_report_file = hwif_report_file
+
         if reuse_typedefs:
             self._gen_in_cls = InputStructGenerator_TypeScope
             self._gen_out_cls = OutputStructGenerator_TypeScope
         else:
             self._gen_in_cls = InputStructGenerator_Hier
             self._gen_out_cls = OutputStructGenerator_Hier
 
@@ -184,14 +186,15 @@
 
 
     def get_implied_prop_output_identifier(self, node: Union[FieldNode, RegNode], prop: str) -> str:
         if isinstance(node, FieldNode):
             assert prop in {
                 "anded", "ored", "xored", "swmod", "swacc",
                 "incrthreshold", "decrthreshold", "overflow", "underflow",
+                "rd_swacc", "wr_swacc",
             }
         elif isinstance(node, RegNode):
             assert prop in {
                 "intr", "halt",
             }
         path = get_indexed_path(self.top_node, node)
         return "hwif_out." + path + "." + prop
```

### Comparing `peakrdl-regblock-0.8.0/src/peakrdl_regblock/hwif/generators.py` & `peakrdl-regblock-0.9.0/src/peakrdl_regblock/hwif/generators.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,58 @@
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Optional, List
 
 from systemrdl.node import FieldNode
 
 from ..struct_generator import RDLFlatStructGenerator
 from ..identifier_filter import kw_filter as kwf
 
 if TYPE_CHECKING:
     from systemrdl.node import Node, SignalNode, RegNode
     from . import Hwif
 
-class InputStructGenerator_Hier(RDLFlatStructGenerator):
-    def __init__(self, hwif: 'Hwif') -> None:
+class HWIFStructGenerator(RDLFlatStructGenerator):
+    def __init__(self, hwif: 'Hwif', hwif_name: str) -> None:
         super().__init__()
         self.hwif = hwif
         self.top_node = hwif.top_node
 
+        self.hwif_report_stack = [hwif_name]
+
+    def push_struct(self, type_name: str, inst_name: str, array_dimensions: Optional[List[int]] = None) -> None: # type: ignore
+        super().push_struct(type_name, inst_name, array_dimensions)
+
+        if array_dimensions:
+            array_suffix = "".join([f"[0:{dim-1}]" for dim in array_dimensions])
+            segment = inst_name + array_suffix
+        else:
+            segment = inst_name
+        self.hwif_report_stack.append(segment)
+
+    def pop_struct(self) -> None:
+        super().pop_struct()
+        self.hwif_report_stack.pop()
+
+    def add_member(self, name: str, width: int = 1) -> None: # type: ignore # pylint: disable=arguments-differ
+        super().add_member(name, width)
+
+        if width > 1:
+            suffix = f"[{width-1}:0]"
+        else:
+            suffix = ""
+
+        path = ".".join(self.hwif_report_stack)
+        if self.hwif.hwif_report_file:
+            self.hwif.hwif_report_file.write(f"{path}.{name}{suffix}\n")
+
+#-------------------------------------------------------------------------------
+
+class InputStructGenerator_Hier(HWIFStructGenerator):
+    def __init__(self, hwif: 'Hwif') -> None:
+        super().__init__(hwif, "hwif_in")
+
     def get_typdef_name(self, node:'Node') -> str:
         base = node.get_rel_path(
             self.top_node.parent,
             hier_separator="__",
             array_suffix="x",
             empty_array_suffix="x"
         )
@@ -68,19 +102,17 @@
                 # Implies a corresponding decrvalue input
                 self.add_member('decrvalue', width)
 
     def exit_Field(self, node: 'FieldNode') -> None:
         self.pop_struct()
 
 
-class OutputStructGenerator_Hier(RDLFlatStructGenerator):
+class OutputStructGenerator_Hier(HWIFStructGenerator):
     def __init__(self, hwif: 'Hwif') -> None:
-        super().__init__()
-        self.hwif = hwif
-        self.top_node = hwif.top_node
+        super().__init__(hwif, "hwif_out")
 
     def get_typdef_name(self, node:'Node') -> str:
         base = node.get_rel_path(
             self.top_node.parent,
             hier_separator="__",
             array_suffix="x",
             empty_array_suffix="x"
@@ -92,15 +124,15 @@
         self.push_struct(type_name, kwf(node.inst_name))
 
         # Expose field's value if it is readable by hw
         if node.is_hw_readable:
             self.add_member("value", node.width)
 
         # Generate output bit signals enabled via property
-        for prop_name in ["anded", "ored", "xored", "swmod", "swacc", "overflow", "underflow"]:
+        for prop_name in ["anded", "ored", "xored", "swmod", "swacc", "overflow", "underflow", "rd_swacc", "wr_swacc"]:
             if node.get_property(prop_name):
                 self.add_member(prop_name)
 
         if node.get_property('incrthreshold') is not False: # (explicitly not False. Not 0)
             self.add_member('incrthreshold')
         if node.get_property('decrthreshold') is not False: # (explicitly not False. Not 0)
             self.add_member('decrthreshold')
```

### Comparing `peakrdl-regblock-0.8.0/src/peakrdl_regblock/identifier_filter.py` & `peakrdl-regblock-0.9.0/src/peakrdl_regblock/identifier_filter.py`

 * *Files identical despite different names*

### Comparing `peakrdl-regblock-0.8.0/src/peakrdl_regblock/module_tmpl.sv` & `peakrdl-regblock-0.9.0/src/peakrdl_regblock/module_tmpl.sv`

 * *Files 7% similar despite different names*

```diff
@@ -104,31 +104,48 @@
     assign decoded_wr_biten_bswap = {<<{decoded_wr_biten}};
 {%- endif %}
 
     // Writes are always granted with no error response
     assign cpuif_wr_ack = decoded_req & decoded_req_is_wr;
     assign cpuif_wr_err = '0;
 
+{%- if has_buffered_write_regs %}
+
+    //--------------------------------------------------------------------------
+    // Write double-buffers
+    //--------------------------------------------------------------------------
+    {{write_buffering.get_storage_struct()|indent}}
+
+    {{write_buffering.get_implementation()|indent}}
+{%- endif %}
     //--------------------------------------------------------------------------
     // Field logic
     //--------------------------------------------------------------------------
     {{field_logic.get_combo_struct()|indent}}
 
     {{field_logic.get_storage_struct()|indent}}
 
     {{field_logic.get_implementation()|indent}}
 
+{%- if has_buffered_read_regs %}
+
+    //--------------------------------------------------------------------------
+    // Read double-buffers
+    //--------------------------------------------------------------------------
+    {{read_buffering.get_storage_struct()|indent}}
+
+    {{read_buffering.get_implementation()|indent}}
+{%- endif %}
     //--------------------------------------------------------------------------
     // Readback
     //--------------------------------------------------------------------------
     logic readback_err;
     logic readback_done;
     logic [{{cpuif.data_width-1}}:0] readback_data;
     {{readback.get_implementation()|indent}}
-
 {% if retime_read_response %}
     always_ff {{get_always_ff_event(cpuif.reset)}} begin
         if({{get_resetsignal(cpuif.reset)}}) begin
             cpuif_rd_ack <= '0;
             cpuif_rd_data <= '0;
             cpuif_rd_err <= '0;
         end else begin
@@ -137,10 +154,9 @@
             cpuif_rd_err <= readback_err;
         end
     end
 {% else %}
     assign cpuif_rd_ack = readback_done;
     assign cpuif_rd_data = readback_data;
     assign cpuif_rd_err = readback_err;
-{% endif %}
-
+{%- endif %}
 endmodule
```

### Comparing `peakrdl-regblock-0.8.0/src/peakrdl_regblock/readback/__init__.py` & `peakrdl-regblock-0.9.0/src/peakrdl_regblock/readback/__init__.py`

 * *Files identical despite different names*

### Comparing `peakrdl-regblock-0.8.0/src/peakrdl_regblock/readback/generators.py` & `peakrdl-regblock-0.9.0/src/peakrdl_regblock/readback/generators.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import TYPE_CHECKING, List
 
+from systemrdl.node import RegNode
+
 from ..forloop_generator import RDLForLoopGenerator, LoopBody
 
 if TYPE_CHECKING:
     from ..exporter import RegblockExporter
-    from systemrdl.node import RegNode
 
 class ReadbackLoopBody(LoopBody):
     def __init__(self, dim: int, iterator: str, i_type: str) -> None:
         super().__init__(dim, iterator, i_type)
         self.n_regs = 0
 
     def __str__(self) -> str:
@@ -72,57 +73,159 @@
 
         super().pop_loop()
 
         # Advance current scope's offset to account for loop's contents
         self.current_offset = start_offset + n_regs * dim
 
 
-    def enter_Reg(self, node: 'RegNode') -> None:
+    def enter_Reg(self, node: RegNode) -> None:
         if not node.has_sw_readable:
             return
 
         accesswidth = node.get_property('accesswidth')
         regwidth = node.get_property('regwidth')
-        if accesswidth < regwidth:
+        rbuf = node.get_property('buffer_reads')
+        if rbuf:
+            trigger = node.get_property('rbuffer_trigger')
+            is_own_trigger = (isinstance(trigger, RegNode) and trigger == node)
+            if is_own_trigger:
+                if accesswidth < regwidth:
+                    self.process_buffered_reg_with_bypass(node, regwidth, accesswidth)
+                else:
+                    # bypass cancels out. Behaves like a normal reg
+                    self.process_reg(node)
+            else:
+                self.process_buffered_reg(node, regwidth, accesswidth)
+        elif accesswidth < regwidth:
             self.process_wide_reg(node, accesswidth)
         else:
             self.process_reg(node)
 
 
-    def process_reg(self, node: 'RegNode') -> None:
+    def process_reg(self, node: RegNode) -> None:
         current_bit = 0
         rd_strb = f"({self.exp.dereferencer.get_access_strobe(node)} && !decoded_req_is_wr)"
         # Fields are sorted by ascending low bit
         for field in node.fields():
             if not field.is_sw_readable:
                 continue
 
             # insert reserved assignment before this field if needed
             if field.low != current_bit:
                 self.add_content(f"assign readback_array[{self.current_offset_str}][{field.low-1}:{current_bit}] = '0;")
 
+            value = self.exp.dereferencer.get_value(field)
             if field.msb < field.lsb:
                 # Field gets bitswapped since it is in [low:high] orientation
-                value = f"{{<<{{{self.exp.dereferencer.get_value(field)}}}}}"
-            else:
-                value = self.exp.dereferencer.get_value(field)
+                value = f"{{<<{{{value}}}}}"
 
             self.add_content(f"assign readback_array[{self.current_offset_str}][{field.high}:{field.low}] = {rd_strb} ? {value} : '0;")
 
             current_bit = field.high + 1
 
         # Insert final reserved assignment if needed
         bus_width = self.exp.cpuif.data_width
         if current_bit < bus_width:
             self.add_content(f"assign readback_array[{self.current_offset_str}][{bus_width-1}:{current_bit}] = '0;")
 
         self.current_offset += 1
 
 
-    def process_wide_reg(self, node: 'RegNode', accesswidth: int) -> None:
+    def process_buffered_reg(self, node: RegNode, regwidth: int, accesswidth: int) -> None:
+        rbuf = self.exp.read_buffering.get_rbuf_data(node)
+
+        if accesswidth < regwidth:
+            # Is wide reg
+            n_subwords = regwidth // accesswidth
+            astrb = self.exp.dereferencer.get_access_strobe(node, reduce_substrobes=False)
+            for i in range(n_subwords):
+                rd_strb = f"({astrb}[{i}] && !decoded_req_is_wr)"
+                bslice = f"[{(i + 1) * accesswidth - 1}:{i*accesswidth}]"
+                self.add_content(f"assign readback_array[{self.current_offset_str}] = {rd_strb} ? {rbuf}{bslice} : '0;")
+                self.current_offset += 1
+
+        else:
+            # Is regular reg
+            rd_strb = f"({self.exp.dereferencer.get_access_strobe(node)} && !decoded_req_is_wr)"
+            self.add_content(f"assign readback_array[{self.current_offset_str}][{regwidth-1}:0] = {rd_strb} ? {rbuf} : '0;")
+
+            bus_width = self.exp.cpuif.data_width
+            if regwidth < bus_width:
+                self.add_content(f"assign readback_array[{self.current_offset_str}][{bus_width-1}:{regwidth}] = '0;")
+
+            self.current_offset += 1
+
+
+    def process_buffered_reg_with_bypass(self, node: RegNode, regwidth: int, accesswidth: int) -> None:
+        """
+        Special case for a buffered register when the register is its own trigger.
+        First sub-word shall bypass the read buffer and assign directly.
+        Subsequent subwords assign from the buffer.
+        Caller guarantees this is a wide reg
+        """
+        astrb = self.exp.dereferencer.get_access_strobe(node, reduce_substrobes=False)
+
+        # Generate assignments for first sub-word
+        bidx = 0
+        rd_strb = f"({astrb}[0] && !decoded_req_is_wr)"
+        for field in node.fields():
+            if not field.is_sw_readable:
+                continue
+
+            if field.low >= accesswidth:
+                # field is not in this subword.
+                break
+
+            if bidx < field.low:
+                # insert padding before
+                self.add_content(f"assign readback_array[{self.current_offset_str}][{field.low - 1}:{bidx}] = '0;")
+
+            if field.high >= accesswidth:
+                # field gets truncated
+                r_low = field.low
+                r_high = accesswidth - 1
+                f_low = 0
+                f_high = accesswidth - 1 - field.low
+
+                if field.msb < field.lsb:
+                    # Field gets bitswapped since it is in [low:high] orientation
+                    # Mirror the low/high indexes
+                    f_low = field.width - 1 - f_low
+                    f_high = field.width - 1 - f_high
+                    f_low, f_high = f_high, f_low
+                    value = f"{{<<{{{self.exp.dereferencer.get_value(field)}[{f_high}:{f_low}]}}}}"
+                else:
+                    value = self.exp.dereferencer.get_value(field) + f"[{f_high}:{f_low}]"
+
+                self.add_content(f"assign readback_array[{self.current_offset_str}][{r_high}:{r_low}] = {rd_strb} ? {value} : '0;")
+                bidx = accesswidth
+            else:
+                # field fits in subword
+                value = self.exp.dereferencer.get_value(field)
+                if field.msb < field.lsb:
+                    # Field gets bitswapped since it is in [low:high] orientation
+                    value = f"{{<<{{{value}}}}}"
+                self.add_content(f"assign readback_array[{self.current_offset_str}][{field.high}:{field.low}] = {rd_strb} ? {value} : '0;")
+                bidx = field.high + 1
+
+        # pad up remainder of subword
+        if bidx < accesswidth:
+            self.add_content(f"assign readback_array[{self.current_offset_str}][{accesswidth-1}:{bidx}] = '0;")
+        self.current_offset += 1
+
+        # Assign remainder of subwords from read buffer
+        n_subwords = regwidth // accesswidth
+        rbuf = self.exp.read_buffering.get_rbuf_data(node)
+        for i in range(1, n_subwords):
+            rd_strb = f"({astrb}[{i}] && !decoded_req_is_wr)"
+            bslice = f"[{(i + 1) * accesswidth - 1}:{i*accesswidth}]"
+            self.add_content(f"assign readback_array[{self.current_offset_str}] = {rd_strb} ? {rbuf}{bslice} : '0;")
+            self.current_offset += 1
+
+    def process_wide_reg(self, node: RegNode, accesswidth: int) -> None:
         bus_width = self.exp.cpuif.data_width
 
         subword_idx = 0
         current_bit = 0 # Bit-offset within the wide register
         access_strb = self.exp.dereferencer.get_access_strobe(node, reduce_substrobes=False)
         # Fields are sorted by ascending low bit
         for field in node.fields():
@@ -158,19 +261,18 @@
                 # Assign the field
                 rd_strb = f"({access_strb}[{subword_idx}] && !decoded_req_is_wr)"
                 if (field_pos == field.low) and (field.high < accesswidth*(subword_idx+1)):
                     # entire field fits into this subword
                     low = field.low - accesswidth * subword_idx
                     high = field.high - accesswidth * subword_idx
 
+                    value = self.exp.dereferencer.get_value(field)
                     if field.msb < field.lsb:
                         # Field gets bitswapped since it is in [low:high] orientation
-                        value = f"{{<<{{{self.exp.dereferencer.get_value(field)}}}}}"
-                    else:
-                        value = self.exp.dereferencer.get_value(field)
+                        value = f"{{<<{{{value}}}}}"
 
                     self.add_content(f"assign readback_array[{self.current_offset_str}][{high}:{low}] = {rd_strb} ? {value} : '0;")
 
                     current_bit = field.high + 1
 
                     if current_bit == accesswidth*(subword_idx+1):
                         # Field ends at the subword boundary
```

### Comparing `peakrdl-regblock-0.8.0/src/peakrdl_regblock/readback/templates/readback.sv` & `peakrdl-regblock-0.9.0/src/peakrdl_regblock/readback/templates/readback.sv`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 {% if array_assignments is not none %}
 // Assign readback values to a flattened array
 logic [{{cpuif.data_width-1}}:0] readback_array[{{array_size}}];
 {{array_assignments}}
 
-{% if do_fanin_stage %}
+
+{%- if do_fanin_stage %}
+
 // fanin stage
 logic [{{cpuif.data_width-1}}:0] readback_array_c[{{fanin_array_size}}];
 for(genvar g=0; g<{{fanin_loop_iter}}; g++) begin
     always_comb begin
         automatic logic [{{cpuif.data_width-1}}:0] readback_data_var;
         readback_data_var = '0;
         for(int i=g*{{fanin_stride}}; i<((g+1)*{{fanin_stride}}); i++) readback_data_var |= readback_array[i];
@@ -44,14 +46,15 @@
     readback_err = '0;
     readback_data_var = '0;
     for(int i=0; i<{{fanin_array_size}}; i++) readback_data_var |= readback_array_r[i];
     readback_data = readback_data_var;
 end
 
 {%- else %}
+
 // Reduce the array
 always_comb begin
     automatic logic [{{cpuif.data_width-1}}:0] readback_data_var;
     readback_done = decoded_req & ~decoded_req_is_wr;
     readback_err = '0;
     readback_data_var = '0;
     for(int i=0; i<{{array_size}}; i++) readback_data_var |= readback_array[i];
```

### Comparing `peakrdl-regblock-0.8.0/src/peakrdl_regblock/scan_design.py` & `peakrdl-regblock-0.9.0/src/peakrdl_regblock/scan_design.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,14 +22,16 @@
         self.msg = exp.top_node.env.msg
 
         # Collections of signals that were actually referenced by the design
         self.in_hier_signal_paths = set() # type: Set[str]
         self.out_of_hier_signals = OrderedDict() # type: OrderedDict[str, SignalNode]
 
         self.has_writable_msb0_fields = False
+        self.has_buffered_write_regs = False
+        self.has_buffered_read_regs = False
 
     def _get_out_of_hier_field_reset(self) -> None:
         current_node = self.exp.top_node.parent
         while current_node is not None:
             for signal in current_node.signals():
                 if signal.get_property('field_reset'):
                     path = signal.get_path()
@@ -65,33 +67,37 @@
                 "Unable to export due to previous errors"
             )
 
     def enter_Component(self, node: 'Node') -> Optional[WalkerAction]:
         if node.external and (node != self.exp.top_node):
             # Do not inspect external components. None of my business
             return WalkerAction.SkipDescendants
+
+        # Collect any signals that are referenced by a property
+        for prop_name in node.list_properties():
+            value = node.get_property(prop_name)
+            if isinstance(value, SignalNode):
+                path = value.get_path()
+                rel_path = value.get_rel_path(self.exp.top_node)
+                if rel_path.startswith("^"):
+                    self.out_of_hier_signals[path] = value
+                else:
+                    self.in_hier_signal_paths.add(path)
+
         return None
 
     def enter_Reg(self, node: 'RegNode') -> None:
         # The CPUIF's bus width is sized according to the largest accesswidth in the design
         accesswidth = node.get_property('accesswidth')
         self.cpuif_data_width = max(self.cpuif_data_width, accesswidth)
 
+        self.has_buffered_write_regs = self.has_buffered_write_regs or bool(node.get_property('buffer_writes'))
+        self.has_buffered_read_regs = self.has_buffered_read_regs or bool(node.get_property('buffer_reads'))
+
     def enter_Signal(self, node: 'SignalNode') -> None:
         if node.get_property('field_reset'):
             path = node.get_path()
             self.in_hier_signal_paths.add(path)
 
     def enter_Field(self, node: 'FieldNode') -> None:
-        # Collect any signals that are referenced by a property
-        for prop_name in node.list_properties():
-            value = node.get_property(prop_name)
-            if isinstance(value, SignalNode):
-                path = value.get_path()
-                rel_path = value.get_rel_path(self.exp.top_node)
-                if rel_path.startswith("^"):
-                    self.out_of_hier_signals[path] = value
-                else:
-                    self.in_hier_signal_paths.add(path)
-
         if node.is_sw_writable and (node.msb < node.lsb):
             self.has_writable_msb0_fields = True
```

### Comparing `peakrdl-regblock-0.8.0/src/peakrdl_regblock/struct_generator.py` & `peakrdl-regblock-0.9.0/src/peakrdl_regblock/struct_generator.py`

 * *Files identical despite different names*

### Comparing `peakrdl-regblock-0.8.0/src/peakrdl_regblock/udps.py` & `peakrdl-regblock-0.9.0/src/peakrdl_regblock/udps/rw_buffering.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,47 @@
 from typing import Any
 
 from systemrdl.udp import UDPDefinition
 from systemrdl.component import Reg
 from systemrdl.rdltypes.references import RefType, PropertyReference
-from systemrdl.node import Node, RegNode, VectorNode
+from systemrdl.rdltypes import NoValue
+from systemrdl.node import Node, RegNode, VectorNode, SignalNode
 
 
 class xBufferTrigger(UDPDefinition):
     valid_components = {Reg}
     valid_type = RefType
 
     def validate(self, node: Node, value: Any) -> None:
         # TODO: Reference shall not cross an internal/external boundary
 
-        if isinstance(value, VectorNode):
+        if value is NoValue:
+            self.msg.error(
+                "Double-buffer trigger property is missing a value assignment",
+                self.get_src_ref(node)
+            )
+        elif isinstance(value, VectorNode):
             # Trigger can reference a vector, but only if it is a single-bit
             if value.width != 1:
                 self.msg.error(
                     "%s '%s' references %s '%s' but it's width is not 1"
                     % (
                         type(node.inst).__name__.lower(), node.inst_name,
                         type(value.inst).__name__.lower(), value.inst_name
                     ),
                     self.get_src_ref(node)
                 )
+
+            if isinstance(value, SignalNode):
+                if not value.get_property('activehigh') and not value.get_property('activelow'):
+                    self.msg.error(
+                        "Trigger was asigned a signal, but it does not specify whether it is activehigh/activelow",
+                        self.get_src_ref(node)
+                    )
+
         elif isinstance(value, PropertyReference) and value.width is not None:
             # Trigger can reference a property, but only if it is a single-bit
             if value.width != 1:
                 self.msg.error(
                     "%s '%s' references property '%s->%s' but it's width is not 1"
                     % (
                         type(node.inst).__name__.lower(), node.inst_name,
@@ -50,25 +64,23 @@
             )
 
 #-------------------------------------------------------------------------------
 class BufferWrites(UDPDefinition):
     name = "buffer_writes"
     valid_components = {Reg}
     valid_type = bool
-    default_assignment = True
 
     def validate(self, node: 'Node', value: Any) -> None:
         assert isinstance(node, RegNode)
         if value:
             if not node.has_sw_writable:
                 self.msg.error(
                     "'buffer_writes' is set to true, but this register does not contain any writable fields.",
                     self.get_src_ref(node)
                 )
-        # TODO: Should I limit the use of other properties on double-buffered registers?
 
     def get_unassigned_default(self, node: 'Node') -> Any:
         return False
 
 
 class WBufferTrigger(xBufferTrigger):
     name = "wbuffer_trigger"
@@ -80,41 +92,29 @@
         return None
 
 
 class BufferReads(UDPDefinition):
     name = "buffer_reads"
     valid_components = {Reg}
     valid_type = bool
-    default_assignment = True
 
     def validate(self, node: 'Node', value: Any) -> None:
         assert isinstance(node, RegNode)
         if value:
             if not node.has_sw_readable:
                 self.msg.error(
                     "'buffer_reads' is set to true, but this register does not contain any readable fields.",
                     self.get_src_ref(node)
                 )
 
-        # TODO: Should I limit the use of other properties on double-buffered registers?
-
     def get_unassigned_default(self, node: 'Node') -> Any:
         return False
 
 
 class RBufferTrigger(xBufferTrigger):
     name = "rbuffer_trigger"
 
     def get_unassigned_default(self, node: 'Node') -> Any:
         # If buffering is enabled, trigger is the register itself
         if node.get_property('buffer_reads'):
             return node
         return None
-
-
-
-ALL_UDPS = [
-    BufferWrites,
-    WBufferTrigger,
-    BufferReads,
-    RBufferTrigger,
-]
```

### Comparing `peakrdl-regblock-0.8.0/src/peakrdl_regblock/utils.py` & `peakrdl-regblock-0.9.0/src/peakrdl_regblock/utils.py`

 * *Files identical despite different names*

### Comparing `peakrdl-regblock-0.8.0/src/peakrdl_regblock/validate_design.py` & `peakrdl-regblock-0.9.0/src/peakrdl_regblock/validate_design.py`

 * *Files 26% similar despite different names*

```diff
@@ -73,27 +73,36 @@
                     "that is inconsistent with this regblock's CPU bus width "
                     f"({self.exp.cpuif.data_width}) are not supported.",
                     node.inst.inst_src_ref
                 )
 
 
     def enter_Field(self, node: 'FieldNode') -> None:
-        # 10.6.1-f: Any field that is software-writable or clear on read shall
-        # not span multiple software accessible sub-words (e.g., a 64-bit
-        # register with a 32-bit access width may not have a writable field with
-        # bits in both the upper and lower half of the register).
-        #
-        # Interpreting this further - this rule applies any time a field is
-        # software-modifiable by any means, including rclr, rset, ruser
-        # TODO: suppress this check for registers that have the appropriate
-        # buffer_writes/buffer_reads UDP set
         parent_accesswidth = node.parent.get_property('accesswidth')
         parent_regwidth = node.parent.get_property('regwidth')
-        if ((parent_accesswidth < parent_regwidth)
-                and (node.lsb // parent_accesswidth) != (node.msb // parent_accesswidth)
-                and (node.is_sw_writable or node.get_property('onread') is not None)):
-            # Field spans across sub-words
-            self.msg.error(
-                f"Software-modifiable field '{node.inst_name}' shall not span "
-                "multiple software-accessible subwords.",
-                node.inst.inst_src_ref
-            )
+        if (
+            (parent_accesswidth < parent_regwidth)
+            and (node.lsb // parent_accesswidth) != (node.msb // parent_accesswidth)
+        ):
+            # field spans multiple sub-words
+            if node.is_sw_writable and not node.parent.get_property('buffer_writes'):
+                # ... and is writable without the protection of double-buffering
+                # Enforce 10.6.1-f
+                self.msg.error(
+                    f"Software-writable field '{node.inst_name}' shall not span"
+                    " multiple software-accessible subwords. Consider enabling"
+                    " write double-buffering.\n"
+                    "For more details, see: https://peakrdl-regblock.readthedocs.io/en/latest/udps/write_buffering.html",
+                    node.inst.inst_src_ref
+                )
+
+            if node.get_property('onread') is not None and not node.parent.get_property('buffer_reads'):
+                # ... is modified by an onread action without the atomicity of read buffering
+                # Enforce 10.6.1-f
+                self.msg.error(
+                    f"The field '{node.inst_name}' spans multiple software-accessible"
+                    " subwords and is modified on-read, making it impossible to"
+                    " access its value correctly. Consider enabling read"
+                    " double-buffering. \n"
+                    "For more details, see: https://peakrdl-regblock.readthedocs.io/en/latest/udps/read_buffering.html",
+                    node.inst.inst_src_ref
+                )
```

### Comparing `peakrdl-regblock-0.8.0/src/peakrdl_regblock.egg-info/PKG-INFO` & `peakrdl-regblock-0.9.0/src/peakrdl_regblock.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peakrdl-regblock
-Version: 0.8.0
+Version: 0.9.0
 Summary: Compile SystemRDL into a SystemVerilog control/status register (CSR) block
 Home-page: https://github.com/SystemRDL/PeakRDL-regblock
 Author: Alex Mykyta
 Author-email: amykyta3@github.com
 Project-URL: Documentation, http://peakrdl-regblock.readthedocs.io
 Project-URL: Source, https://github.com/SystemRDL/PeakRDL-regblock
 Project-URL: Tracker, https://github.com/SystemRDL/PeakRDL-regblock/issues
@@ -12,14 +12,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `peakrdl-regblock-0.8.0/src/peakrdl_regblock.egg-info/SOURCES.txt` & `peakrdl-regblock-0.9.0/src/peakrdl_regblock.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 README.md
 setup.py
 src/peakrdl_regblock/__about__.py
 src/peakrdl_regblock/__init__.py
 src/peakrdl_regblock/__peakrdl__.py
 src/peakrdl_regblock/addr_decode.py
 src/peakrdl_regblock/dereferencer.py
+src/peakrdl_regblock/entry_points.py
 src/peakrdl_regblock/exporter.py
 src/peakrdl_regblock/forloop_generator.py
 src/peakrdl_regblock/identifier_filter.py
 src/peakrdl_regblock/module_tmpl.sv
 src/peakrdl_regblock/package_tmpl.sv
 src/peakrdl_regblock/scan_design.py
 src/peakrdl_regblock/struct_generator.py
-src/peakrdl_regblock/udps.py
 src/peakrdl_regblock/utils.py
 src/peakrdl_regblock/validate_design.py
 src/peakrdl_regblock.egg-info/PKG-INFO
 src/peakrdl_regblock.egg-info/SOURCES.txt
 src/peakrdl_regblock.egg-info/dependency_links.txt
 src/peakrdl_regblock.egg-info/entry_points.txt
 src/peakrdl_regblock.egg-info/requires.txt
@@ -42,10 +42,21 @@
 src/peakrdl_regblock/field_logic/sw_onread.py
 src/peakrdl_regblock/field_logic/sw_onwrite.py
 src/peakrdl_regblock/field_logic/sw_singlepulse.py
 src/peakrdl_regblock/field_logic/templates/counter_macros.sv
 src/peakrdl_regblock/field_logic/templates/field_storage.sv
 src/peakrdl_regblock/hwif/__init__.py
 src/peakrdl_regblock/hwif/generators.py
+src/peakrdl_regblock/read_buffering/__init__.py
+src/peakrdl_regblock/read_buffering/implementation_generator.py
+src/peakrdl_regblock/read_buffering/storage_generator.py
+src/peakrdl_regblock/read_buffering/template.sv
 src/peakrdl_regblock/readback/__init__.py
 src/peakrdl_regblock/readback/generators.py
-src/peakrdl_regblock/readback/templates/readback.sv
+src/peakrdl_regblock/readback/templates/readback.sv
+src/peakrdl_regblock/udps/__init__.py
+src/peakrdl_regblock/udps/extended_swacc.py
+src/peakrdl_regblock/udps/rw_buffering.py
+src/peakrdl_regblock/write_buffering/__init__.py
+src/peakrdl_regblock/write_buffering/implementation_generator.py
+src/peakrdl_regblock/write_buffering/storage_generator.py
+src/peakrdl_regblock/write_buffering/template.sv
```

