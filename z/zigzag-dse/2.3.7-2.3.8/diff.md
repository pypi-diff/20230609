# Comparing `tmp/zigzag-dse-2.3.7.tar.gz` & `tmp/zigzag-dse-2.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zigzag-dse-2.3.7.tar", last modified: Fri Jun  9 14:33:03 2023, max compression
+gzip compressed data, was "zigzag-dse-2.3.8.tar", last modified: Fri Jun  9 14:49:12 2023, max compression
```

## Comparing `zigzag-dse-2.3.7.tar` & `zigzag-dse-2.3.8.tar`

### file list

```diff
@@ -1,251 +1,251 @@
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-06-09 14:33:03.731706 zigzag-dse-2.3.7/
--rw-r--r--   0 asymons   (1000) asymons   (1000)     1522 2022-06-17 07:16:25.000000 zigzag-dse-2.3.7/LICENSE
--rw-r--r--   0 asymons   (1000) asymons   (1000)       88 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/MANIFEST.in
--rw-r--r--   0 asymons   (1000) asymons   (1000)     9080 2023-06-09 14:33:03.721706 zigzag-dse-2.3.7/PKG-INFO
--rw-r--r--   0 asymons   (1000) asymons   (1000)     6758 2023-06-01 09:36:49.000000 zigzag-dse-2.3.7/README.md
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-06-09 14:33:03.611706 zigzag-dse-2.3.7/docs/
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-06-09 14:33:03.621706 zigzag-dse-2.3.7/docs/source/
--rw-r--r--   0 asymons   (1000) asymons   (1000)     2591 2023-05-05 06:54:43.000000 zigzag-dse-2.3.7/docs/source/conf.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     1601 2023-06-09 14:32:49.000000 zigzag-dse-2.3.7/pyproject.toml
--rw-r--r--   0 asymons   (1000) asymons   (1000)       38 2023-06-09 14:33:03.731706 zigzag-dse-2.3.7/setup.cfg
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-06-09 14:33:03.621706 zigzag-dse-2.3.7/zigzag/
--rw-r--r--   0 asymons   (1000) asymons   (1000)       22 2023-06-09 14:32:49.000000 zigzag-dse-2.3.7/zigzag/__init__.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     2497 2022-11-06 07:09:28.000000 zigzag-dse-2.3.7/zigzag/__main__.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     4451 2023-06-02 14:22:51.000000 zigzag-dse-2.3.7/zigzag/api.py
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-06-09 14:33:03.621706 zigzag-dse-2.3.7/zigzag/classes/
--rw-r--r--   0 asymons   (1000) asymons   (1000)        0 2022-11-06 21:40:40.000000 zigzag-dse-2.3.7/zigzag/classes/__init__.py
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-06-09 14:33:03.621706 zigzag-dse-2.3.7/zigzag/classes/cacti/
--rw-r--r--   0 asymons   (1000) asymons   (1000)      291 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/README.md
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-06-09 14:33:03.621706 zigzag-dse-2.3.7/zigzag/classes/cacti/__pycache__/
--rw-r--r--   0 asymons   (1000) asymons   (1000)     3412 2023-04-22 21:31:11.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/__pycache__/cacti_parser.cpython-310.pyc
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-06-09 14:33:03.671706 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/
--rw-r--r--   0 asymons   (1000) asymons   (1000)     6576 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/2DDRAM_Samsung2GbDDR2.cfg
--rw-r--r--   0 asymons   (1000) asymons   (1000)     6555 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/2DDRAM_micron1Gb.cfg
--rw-r--r--   0 asymons   (1000) asymons   (1000)     6920 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/3DDRAM_Samsung3D8Gb_extened.cfg
--rw-r--r--   0 asymons   (1000) asymons   (1000)     5324 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/README
--rw-r--r--   0 asymons   (1000) asymons   (1000)     9282 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/TSV.cc
--rw-r--r--   0 asymons   (1000) asymons   (1000)     3322 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/TSV.h
--rw-r--r--   0 asymons   (1000) asymons   (1000)    41184 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/Ucache.cc
--rw-r--r--   0 asymons   (1000) asymons   (1000)     3607 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/Ucache.h
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-06-09 14:33:03.671706 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/__pycache__/
--rw-r--r--   0 asymons   (1000) asymons   (1000)    13713 2023-04-16 14:07:27.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/__pycache__/cacti_config_creator.cpython-310.pyc
--rw-r--r--   0 asymons   (1000) asymons   (1000)     5116 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/arbiter.cc
--rw-r--r--   0 asymons   (1000) asymons   (1000)     2771 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/arbiter.h
--rw-r--r--   0 asymons   (1000) asymons   (1000)     2057 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/area.cc
--rw-r--r--   0 asymons   (1000) asymons   (1000)     2416 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/area.h
--rw-r--r--   0 asymons   (1000) asymons   (1000)     8474 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/bank.cc
--rw-r--r--   0 asymons   (1000) asymons   (1000)     2664 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/bank.h
--rw-r--r--   0 asymons   (1000) asymons   (1000)    29279 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/basic_circuit.cc
--rw-r--r--   0 asymons   (1000) asymons   (1000)     7364 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/basic_circuit.h
--rw-r--r--   0 asymons   (1000) asymons   (1000)    11041 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/cache.cfg_temp
--rw-r--r--   0 asymons   (1000) asymons   (1000)    32713 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/cache_old.cfg.out
--rwxr-xr-x   0 asymons   (1000) asymons   (1000)  2421320 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/cacti
--rw-r--r--   0 asymons   (1000) asymons   (1000)      173 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/cacti.i
--rw-r--r--   0 asymons   (1000) asymons   (1000)     1334 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/cacti.mk
--rw-r--r--   0 asymons   (1000) asymons   (1000)    25297 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/cacti_config_creator.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     5586 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/cacti_interface.cc
--rw-r--r--   0 asymons   (1000) asymons   (1000)    27215 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/cacti_interface.h
--rw-r--r--   0 asymons   (1000) asymons   (1000)     3569 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/cacti_top.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     7561 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/component.cc
--rw-r--r--   0 asymons   (1000) asymons   (1000)     2837 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/component.h
--rw-r--r--   0 asymons   (1000) asymons   (1000)     9565 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/const.h
--rw-r--r--   0 asymons   (1000) asymons   (1000)     5001 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/contention.dat
--rw-r--r--   0 asymons   (1000) asymons   (1000)     7349 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/crossbar.cc
--rw-r--r--   0 asymons   (1000) asymons   (1000)     3204 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/crossbar.h
--rw-r--r--   0 asymons   (1000) asymons   (1000)     9849 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/ddr3.cfg
--rw-r--r--   0 asymons   (1000) asymons   (1000)    62337 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/decoder.cc
--rw-r--r--   0 asymons   (1000) asymons   (1000)     7405 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/decoder.h
--rw-r--r--   0 asymons   (1000) asymons   (1000)     3712 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/dram.cfg
--rw-r--r--   0 asymons   (1000) asymons   (1000)     9750 2023-04-25 15:05:19.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/example_mem_pool.yaml
--rw-r--r--   0 asymons   (1000) asymons   (1000)    17411 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/extio.cc
--rw-r--r--   0 asymons   (1000) asymons   (1000)      878 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/extio.h
--rw-r--r--   0 asymons   (1000) asymons   (1000)    46185 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/extio_technology.cc
--rw-r--r--   0 asymons   (1000) asymons   (1000)     9068 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/extio_technology.h
--rw-r--r--   0 asymons   (1000) asymons   (1000)    23772 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/htree2.cc
--rw-r--r--   0 asymons   (1000) asymons   (1000)     3595 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/htree2.h
--rw-r--r--   0 asymons   (1000) asymons   (1000)   133713 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/io.cc
--rw-r--r--   0 asymons   (1000) asymons   (1000)     2116 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/io.h
--rw-r--r--   0 asymons   (1000) asymons   (1000)     9850 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/lpddr.cfg
--rw-r--r--   0 asymons   (1000) asymons   (1000)     7217 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/main.cc
--rw-r--r--   0 asymons   (1000) asymons   (1000)      407 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/makefile
--rw-r--r--   0 asymons   (1000) asymons   (1000)    94813 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/mat.cc
--rw-r--r--   0 asymons   (1000) asymons   (1000)     6122 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/mat.h
--rw-r--r--   0 asymons   (1000) asymons   (1000)    16630 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/memcad.cc
--rw-r--r--   0 asymons   (1000) asymons   (1000)      553 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/memcad.h
--rw-r--r--   0 asymons   (1000) asymons   (1000)    11483 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/memcad_parameters.cc
--rw-r--r--   0 asymons   (1000) asymons   (1000)     4490 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/memcad_parameters.h
--rw-r--r--   0 asymons   (1000) asymons   (1000)    29014 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/memorybus.cc
--rw-r--r--   0 asymons   (1000) asymons   (1000)     5426 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/memorybus.h
--rw-r--r--   0 asymons   (1000) asymons   (1000)    19629 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/nuca.cc
--rw-r--r--   0 asymons   (1000) asymons   (1000)     3306 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/nuca.h
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-06-09 14:33:03.701706 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/obj_dbg/
--rw-r--r--   0 asymons   (1000) asymons   (1000)   134304 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/obj_dbg/TSV.o
--rw-r--r--   0 asymons   (1000) asymons   (1000)   352744 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/obj_dbg/Ucache.o
--rw-r--r--   0 asymons   (1000) asymons   (1000)   157960 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/obj_dbg/arbiter.o
--rw-r--r--   0 asymons   (1000) asymons   (1000)   124352 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/obj_dbg/area.o
--rw-r--r--   0 asymons   (1000) asymons   (1000)   156624 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/obj_dbg/bank.o
--rw-r--r--   0 asymons   (1000) asymons   (1000)   155192 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/obj_dbg/basic_circuit.o
--rwxr-xr-x   0 asymons   (1000) asymons   (1000)  2421320 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/obj_dbg/cacti
--rw-r--r--   0 asymons   (1000) asymons   (1000)   175768 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/obj_dbg/cacti_interface.o
--rw-r--r--   0 asymons   (1000) asymons   (1000)   159768 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/obj_dbg/component.o
--rw-r--r--   0 asymons   (1000) asymons   (1000)   160680 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/obj_dbg/crossbar.o
--rw-r--r--   0 asymons   (1000) asymons   (1000)   207224 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/obj_dbg/decoder.o
--rw-r--r--   0 asymons   (1000) asymons   (1000)   145592 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/obj_dbg/extio.o
--rw-r--r--   0 asymons   (1000) asymons   (1000)   180464 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/obj_dbg/extio_technology.o
--rw-r--r--   0 asymons   (1000) asymons   (1000)   178384 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/obj_dbg/htree2.o
--rw-r--r--   0 asymons   (1000) asymons   (1000)   411960 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/obj_dbg/io.o
--rw-r--r--   0 asymons   (1000) asymons   (1000)   192248 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/obj_dbg/main.o
--rw-r--r--   0 asymons   (1000) asymons   (1000)   270320 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/obj_dbg/mat.o
--rw-r--r--   0 asymons   (1000) asymons   (1000)   569648 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/obj_dbg/memcad.o
--rw-r--r--   0 asymons   (1000) asymons   (1000)   280416 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/obj_dbg/memcad_parameters.o
--rw-r--r--   0 asymons   (1000) asymons   (1000)   204480 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/obj_dbg/memorybus.o
--rw-r--r--   0 asymons   (1000) asymons   (1000)   256824 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/obj_dbg/nuca.o
--rw-r--r--   0 asymons   (1000) asymons   (1000)   313848 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/obj_dbg/parameter.o
--rw-r--r--   0 asymons   (1000) asymons   (1000)   124400 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/obj_dbg/powergating.o
--rw-r--r--   0 asymons   (1000) asymons   (1000)   175432 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/obj_dbg/router.o
--rw-r--r--   0 asymons   (1000) asymons   (1000)   128080 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/obj_dbg/subarray.o
--rw-r--r--   0 asymons   (1000) asymons   (1000)   144976 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/obj_dbg/technology.o
--rw-r--r--   0 asymons   (1000) asymons   (1000)   228000 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/obj_dbg/uca.o
--rw-r--r--   0 asymons   (1000) asymons   (1000)   232752 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/obj_dbg/wire.o
--rw-r--r--   0 asymons   (1000) asymons   (1000)   111980 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/parameter.cc
--rw-r--r--   0 asymons   (1000) asymons   (1000)    20306 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/parameter.h
--rw-r--r--   0 asymons   (1000) asymons   (1000)     5286 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/powergating.cc
--rw-r--r--   0 asymons   (1000) asymons   (1000)     3055 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/powergating.h
--rwxr-xr-x   0 asymons   (1000) asymons   (1000)     1886 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/regression.test
--rw-r--r--   0 asymons   (1000) asymons   (1000)    10212 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/router.cc
--rw-r--r--   0 asymons   (1000) asymons   (1000)     3721 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/router.h
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-06-09 14:33:03.711706 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/sample_config_files/
--rw-r--r--   0 asymons   (1000) asymons   (1000)     8781 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/sample_config_files/ddr3_cache.cfg
--rw-r--r--   0 asymons   (1000) asymons   (1000)     8768 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/sample_config_files/diff_ddr3_cache.cfg
--rw-r--r--   0 asymons   (1000) asymons   (1000)     8780 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/sample_config_files/lpddr3_cache.cfg
--rw-r--r--   0 asymons   (1000) asymons   (1000)     8784 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/sample_config_files/wideio_cache.cfg
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-06-09 14:33:03.711706 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/self_gen/
--rw-r--r--   0 asymons   (1000) asymons   (1000)     9545 2023-04-25 15:05:19.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/self_gen/cache.cfg
--rw-r--r--   0 asymons   (1000) asymons   (1000)      579 2023-04-25 15:05:19.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/self_gen/cache.cfg.out
--rw-r--r--   0 asymons   (1000) asymons   (1000)     8332 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/subarray.cc
--rw-r--r--   0 asymons   (1000) asymons   (1000)     2542 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/subarray.h
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-06-09 14:33:03.711706 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/tech_params/
--rw-r--r--   0 asymons   (1000) asymons   (1000)       25 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/tech_params/16nm.dat
--rw-r--r--   0 asymons   (1000) asymons   (1000)    23666 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/tech_params/180nm-old.dat
--rw-r--r--   0 asymons   (1000) asymons   (1000)     3842 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/tech_params/180nm.dat
--rw-r--r--   0 asymons   (1000) asymons   (1000)     4575 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/tech_params/22nm.dat
--rw-r--r--   0 asymons   (1000) asymons   (1000)     4759 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/tech_params/32nm.dat
--rw-r--r--   0 asymons   (1000) asymons   (1000)     4755 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/tech_params/45nm.dat
--rw-r--r--   0 asymons   (1000) asymons   (1000)    24571 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/tech_params/65nm-old.dat
--rw-r--r--   0 asymons   (1000) asymons   (1000)     4758 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/tech_params/65nm.dat
--rw-r--r--   0 asymons   (1000) asymons   (1000)    24570 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/tech_params/90nm-old.dat
--rw-r--r--   0 asymons   (1000) asymons   (1000)     4742 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/tech_params/90nm.dat
--rw-r--r--   0 asymons   (1000) asymons   (1000)    15087 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/technology.cc
--rw-r--r--   0 asymons   (1000) asymons   (1000)    41317 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/uca.cc
--rw-r--r--   0 asymons   (1000) asymons   (1000)     4035 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/uca.h
--rw-r--r--   0 asymons   (1000) asymons   (1000)     2064 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/version_cacti.h
--rw-r--r--   0 asymons   (1000) asymons   (1000)    29856 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/wire.cc
--rw-r--r--   0 asymons   (1000) asymons   (1000)     4375 2023-03-27 09:38:39.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/wire.h
--rw-r--r--   0 asymons   (1000) asymons   (1000)     6110 2023-04-22 12:58:13.000000 zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_parser.py
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-06-09 14:33:03.711706 zigzag-dse-2.3.7/zigzag/classes/cost_model/
--rw-r--r--   0 asymons   (1000) asymons   (1000)    62023 2023-04-16 12:43:30.000000 zigzag-dse-2.3.7/zigzag/classes/cost_model/cost_model.py
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-06-09 14:33:03.611706 zigzag-dse-2.3.7/zigzag/classes/hardware/
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-06-09 14:33:03.711706 zigzag-dse-2.3.7/zigzag/classes/hardware/architecture/
--rw-r--r--   0 asymons   (1000) asymons   (1000)     1278 2023-04-16 13:43:29.000000 zigzag-dse-2.3.7/zigzag/classes/hardware/architecture/accelerator.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     9441 2023-04-07 09:22:11.000000 zigzag-dse-2.3.7/zigzag/classes/hardware/architecture/adder_hierarchy.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     6031 2023-04-07 09:22:16.000000 zigzag-dse-2.3.7/zigzag/classes/hardware/architecture/core.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)      918 2023-04-07 09:22:20.000000 zigzag-dse-2.3.7/zigzag/classes/hardware/architecture/dimension.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)    11764 2023-04-07 09:22:26.000000 zigzag-dse-2.3.7/zigzag/classes/hardware/architecture/memory_hierarchy.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     3567 2023-06-02 14:16:12.000000 zigzag-dse-2.3.7/zigzag/classes/hardware/architecture/memory_instance.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)    12231 2023-04-07 09:22:36.000000 zigzag-dse-2.3.7/zigzag/classes/hardware/architecture/memory_level.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     3014 2023-04-07 09:22:40.000000 zigzag-dse-2.3.7/zigzag/classes/hardware/architecture/operational_array.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     1874 2023-04-07 09:22:44.000000 zigzag-dse-2.3.7/zigzag/classes/hardware/architecture/operational_unit.py
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-06-09 14:33:03.611706 zigzag-dse-2.3.7/zigzag/classes/io/
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-06-09 14:33:03.711706 zigzag-dse-2.3.7/zigzag/classes/io/accelerator/
--rw-r--r--   0 asymons   (1000) asymons   (1000)     2805 2022-11-06 21:24:03.000000 zigzag-dse-2.3.7/zigzag/classes/io/accelerator/parser.py
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-06-09 14:33:03.721706 zigzag-dse-2.3.7/zigzag/classes/io/onnx/
--rw-r--r--   0 asymons   (1000) asymons   (1000)     7087 2023-06-09 14:32:23.000000 zigzag-dse-2.3.7/zigzag/classes/io/onnx/conv.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)      884 2023-04-07 09:12:40.000000 zigzag-dse-2.3.7/zigzag/classes/io/onnx/default.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     5382 2023-04-07 09:12:45.000000 zigzag-dse-2.3.7/zigzag/classes/io/onnx/gemm.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     3679 2023-04-07 09:12:49.000000 zigzag-dse-2.3.7/zigzag/classes/io/onnx/matmul.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     4912 2023-04-07 09:12:53.000000 zigzag-dse-2.3.7/zigzag/classes/io/onnx/model.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     1163 2023-04-07 09:12:58.000000 zigzag-dse-2.3.7/zigzag/classes/io/onnx/parser.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     4089 2023-06-09 14:32:23.000000 zigzag-dse-2.3.7/zigzag/classes/io/onnx/utils.py
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-06-09 14:33:03.721706 zigzag-dse-2.3.7/zigzag/classes/mapping/
--rw-r--r--   0 asymons   (1000) asymons   (1000)    40951 2023-04-07 09:24:31.000000 zigzag-dse-2.3.7/zigzag/classes/mapping/combined_mapping.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)      637 2023-04-07 09:24:42.000000 zigzag-dse-2.3.7/zigzag/classes/mapping/loop.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     9386 2023-04-07 09:24:55.000000 zigzag-dse-2.3.7/zigzag/classes/mapping/mapping_assist_funcs.py
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-06-09 14:33:03.721706 zigzag-dse-2.3.7/zigzag/classes/mapping/memory/
--rw-r--r--   0 asymons   (1000) asymons   (1000)        0 2023-04-07 09:25:08.000000 zigzag-dse-2.3.7/zigzag/classes/mapping/memory/data_layout.py
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-06-09 14:33:03.721706 zigzag-dse-2.3.7/zigzag/classes/mapping/spatial/
--rw-r--r--   0 asymons   (1000) asymons   (1000)     7655 2023-06-09 14:31:45.000000 zigzag-dse-2.3.7/zigzag/classes/mapping/spatial/spatial_mapping.py
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-06-09 14:33:03.721706 zigzag-dse-2.3.7/zigzag/classes/mapping/temporal/
--rw-r--r--   0 asymons   (1000) asymons   (1000)      380 2023-04-07 09:25:12.000000 zigzag-dse-2.3.7/zigzag/classes/mapping/temporal/temporal_loop.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     7412 2023-04-07 09:25:16.000000 zigzag-dse-2.3.7/zigzag/classes/mapping/temporal/temporal_mapping.py
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-06-09 14:33:03.611706 zigzag-dse-2.3.7/zigzag/classes/opt/
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-06-09 14:33:03.721706 zigzag-dse-2.3.7/zigzag/classes/opt/spatial/
--rw-r--r--   0 asymons   (1000) asymons   (1000)     7044 2023-04-07 09:30:21.000000 zigzag-dse-2.3.7/zigzag/classes/opt/spatial/generator.py
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-06-09 14:33:03.611706 zigzag-dse-2.3.7/zigzag/classes/opt/temporal/
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-06-09 14:33:03.721706 zigzag-dse-2.3.7/zigzag/classes/opt/temporal/loma/
--rw-r--r--   0 asymons   (1000) asymons   (1000)    11591 2023-04-07 09:29:56.000000 zigzag-dse-2.3.7/zigzag/classes/opt/temporal/loma/engine.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)      489 2023-04-07 09:30:00.000000 zigzag-dse-2.3.7/zigzag/classes/opt/temporal/loma/loop.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)    15479 2023-04-07 09:30:04.000000 zigzag-dse-2.3.7/zigzag/classes/opt/temporal/loma/memory_allocator.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     2837 2023-04-07 09:30:07.000000 zigzag-dse-2.3.7/zigzag/classes/opt/temporal/loma/multipermute.py
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-06-09 14:33:03.721706 zigzag-dse-2.3.7/zigzag/classes/opt/temporal/salsa/
--rw-r--r--   0 asymons   (1000) asymons   (1000)     8726 2023-04-07 09:30:11.000000 zigzag-dse-2.3.7/zigzag/classes/opt/temporal/salsa/engine.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     3616 2023-04-07 09:30:15.000000 zigzag-dse-2.3.7/zigzag/classes/opt/temporal/salsa/state.py
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-06-09 14:33:03.721706 zigzag-dse-2.3.7/zigzag/classes/stages/
--rw-r--r--   0 asymons   (1000) asymons   (1000)     2054 2023-04-07 09:02:40.000000 zigzag-dse-2.3.7/zigzag/classes/stages/CostModelStage.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     1552 2023-04-07 09:03:00.000000 zigzag-dse-2.3.7/zigzag/classes/stages/DumpStage.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     3240 2023-04-07 09:02:56.000000 zigzag-dse-2.3.7/zigzag/classes/stages/GeneralParameterIteratorStage.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     2105 2023-04-07 09:02:49.000000 zigzag-dse-2.3.7/zigzag/classes/stages/LomaStage.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     2163 2023-04-07 09:27:10.000000 zigzag-dse-2.3.7/zigzag/classes/stages/MainInputParserStages.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)      966 2023-04-07 09:03:11.000000 zigzag-dse-2.3.7/zigzag/classes/stages/ONNXModelParserStage.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     1568 2023-04-07 09:03:29.000000 zigzag-dse-2.3.7/zigzag/classes/stages/PlotTemporalMappingsStage.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     6204 2023-04-07 09:03:44.000000 zigzag-dse-2.3.7/zigzag/classes/stages/ReduceStages.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     6260 2023-04-07 09:03:58.000000 zigzag-dse-2.3.7/zigzag/classes/stages/RunOptStages.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     6546 2023-04-07 09:04:04.000000 zigzag-dse-2.3.7/zigzag/classes/stages/SalsaStage.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     6997 2023-04-15 12:05:47.000000 zigzag-dse-2.3.7/zigzag/classes/stages/SaveStage.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     8158 2023-04-07 09:04:25.000000 zigzag-dse-2.3.7/zigzag/classes/stages/SpatialMappingConversionStage.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     3906 2023-04-07 09:05:11.000000 zigzag-dse-2.3.7/zigzag/classes/stages/SpatialMappingGeneratorStage.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     2593 2023-04-07 09:05:30.000000 zigzag-dse-2.3.7/zigzag/classes/stages/Stage.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     4046 2023-04-07 09:05:44.000000 zigzag-dse-2.3.7/zigzag/classes/stages/TemporalOrderingConversionStage.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     1187 2023-04-07 09:05:50.000000 zigzag-dse-2.3.7/zigzag/classes/stages/WorkloadStage.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     2821 2023-04-07 09:28:15.000000 zigzag-dse-2.3.7/zigzag/classes/stages/__init__.py
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-06-09 14:33:03.721706 zigzag-dse-2.3.7/zigzag/classes/workload/
--rw-r--r--   0 asymons   (1000) asymons   (1000)     2468 2023-04-07 09:17:48.000000 zigzag-dse-2.3.7/zigzag/classes/workload/dnn_workload.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     2210 2023-04-07 09:17:53.000000 zigzag-dse-2.3.7/zigzag/classes/workload/dummy_node.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)    21102 2023-04-07 09:19:32.000000 zigzag-dse-2.3.7/zigzag/classes/workload/layer_node.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     1542 2023-04-07 09:18:04.000000 zigzag-dse-2.3.7/zigzag/classes/workload/onnx_workload.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)    14521 2023-04-07 09:18:09.000000 zigzag-dse-2.3.7/zigzag/classes/workload/test_layer_node.py
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-06-09 14:33:03.611706 zigzag-dse-2.3.7/zigzag/inputs/
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-06-09 14:33:03.611706 zigzag-dse-2.3.7/zigzag/inputs/examples/
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-06-09 14:33:03.721706 zigzag-dse-2.3.7/zigzag/inputs/examples/hardware/
--rw-r--r--   0 asymons   (1000) asymons   (1000)     8448 2023-04-16 14:01:57.000000 zigzag-dse-2.3.7/zigzag/inputs/examples/hardware/Ascend_like.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     5849 2023-04-16 14:01:57.000000 zigzag-dse-2.3.7/zigzag/inputs/examples/hardware/Edge_TPU_like.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     5746 2023-04-16 14:01:57.000000 zigzag-dse-2.3.7/zigzag/inputs/examples/hardware/Eyeriss_like.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     7098 2023-04-16 14:01:57.000000 zigzag-dse-2.3.7/zigzag/inputs/examples/hardware/Meta_prototype.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     5112 2023-04-16 14:01:57.000000 zigzag-dse-2.3.7/zigzag/inputs/examples/hardware/TPU_like.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     7287 2023-04-16 14:01:57.000000 zigzag-dse-2.3.7/zigzag/inputs/examples/hardware/Tesla_NPU_like.py
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-06-09 14:33:03.721706 zigzag-dse-2.3.7/zigzag/inputs/examples/mapping/
--rw-r--r--   0 asymons   (1000) asymons   (1000)      561 2023-04-15 09:48:43.000000 zigzag-dse-2.3.7/zigzag/inputs/examples/mapping/assend_like.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)      196 2023-04-15 09:48:46.000000 zigzag-dse-2.3.7/zigzag/inputs/examples/mapping/default.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)      832 2023-04-15 09:48:50.000000 zigzag-dse-2.3.7/zigzag/inputs/examples/mapping/edge_tpu_like.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)      560 2023-04-15 09:48:52.000000 zigzag-dse-2.3.7/zigzag/inputs/examples/mapping/meta_prototype_like.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)      610 2023-04-15 09:48:56.000000 zigzag-dse-2.3.7/zigzag/inputs/examples/mapping/tesla_npu_like.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)      557 2023-04-15 09:49:08.000000 zigzag-dse-2.3.7/zigzag/inputs/examples/mapping/tpu_like.py
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-06-09 14:33:03.721706 zigzag-dse-2.3.7/zigzag/inputs/examples/workload/
--rw-r--r--   0 asymons   (1000) asymons   (1000)     4067 2023-01-16 14:56:40.000000 zigzag-dse-2.3.7/zigzag/inputs/examples/workload/alexnet.onnx
--rw-r--r--   0 asymons   (1000) asymons   (1000)    71724 2022-12-09 21:20:28.000000 zigzag-dse-2.3.7/zigzag/inputs/examples/workload/mobilenetv2.onnx
--rw-r--r--   0 asymons   (1000) asymons   (1000)    18600 2023-04-15 09:55:05.000000 zigzag-dse-2.3.7/zigzag/inputs/examples/workload/resnet18.onnx
--rw-r--r--   0 asymons   (1000) asymons   (1000)    19065 2023-04-15 09:49:14.000000 zigzag-dse-2.3.7/zigzag/inputs/examples/workload/resnet18.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)      504 2022-10-27 21:43:16.000000 zigzag-dse-2.3.7/zigzag/utils.py
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-06-09 14:33:03.621706 zigzag-dse-2.3.7/zigzag/visualization/
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-06-09 14:33:03.721706 zigzag-dse-2.3.7/zigzag/visualization/graph/
--rw-r--r--   0 asymons   (1000) asymons   (1000)     1527 2023-04-15 09:49:36.000000 zigzag-dse-2.3.7/zigzag/visualization/graph/memory_hierarchy.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     1280 2023-04-15 09:49:41.000000 zigzag-dse-2.3.7/zigzag/visualization/graph/workload.py
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-06-09 14:33:03.721706 zigzag-dse-2.3.7/zigzag/visualization/results/
--rw-r--r--   0 asymons   (1000) asymons   (1000)     8773 2023-04-16 16:18:26.000000 zigzag-dse-2.3.7/zigzag/visualization/results/plot_cme.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     3951 2023-04-15 09:49:53.000000 zigzag-dse-2.3.7/zigzag/visualization/results/print_mapping.py
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-06-09 14:33:03.721706 zigzag-dse-2.3.7/zigzag_dse.egg-info/
--rw-r--r--   0 asymons   (1000) asymons   (1000)     9080 2023-06-09 14:33:03.000000 zigzag-dse-2.3.7/zigzag_dse.egg-info/PKG-INFO
--rw-r--r--   0 asymons   (1000) asymons   (1000)     9580 2023-06-09 14:33:03.000000 zigzag-dse-2.3.7/zigzag_dse.egg-info/SOURCES.txt
--rw-r--r--   0 asymons   (1000) asymons   (1000)        1 2023-06-09 14:33:03.000000 zigzag-dse-2.3.7/zigzag_dse.egg-info/dependency_links.txt
--rw-r--r--   0 asymons   (1000) asymons   (1000)       52 2023-06-09 14:33:03.000000 zigzag-dse-2.3.7/zigzag_dse.egg-info/entry_points.txt
--rw-r--r--   0 asymons   (1000) asymons   (1000)      144 2023-06-09 14:33:03.000000 zigzag-dse-2.3.7/zigzag_dse.egg-info/requires.txt
--rw-r--r--   0 asymons   (1000) asymons   (1000)       27 2023-06-09 14:33:03.000000 zigzag-dse-2.3.7/zigzag_dse.egg-info/top_level.txt
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-06-09 14:49:12.521712 zigzag-dse-2.3.8/
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     1522 2022-06-17 07:16:25.000000 zigzag-dse-2.3.8/LICENSE
+-rw-r--r--   0 asymons   (1000) asymons   (1000)       88 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/MANIFEST.in
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     9080 2023-06-09 14:49:12.521712 zigzag-dse-2.3.8/PKG-INFO
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     6758 2023-06-01 09:36:49.000000 zigzag-dse-2.3.8/README.md
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-06-09 14:49:12.471712 zigzag-dse-2.3.8/docs/
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-06-09 14:49:12.471712 zigzag-dse-2.3.8/docs/source/
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     2591 2023-05-05 06:54:43.000000 zigzag-dse-2.3.8/docs/source/conf.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     1601 2023-06-09 14:48:50.000000 zigzag-dse-2.3.8/pyproject.toml
+-rw-r--r--   0 asymons   (1000) asymons   (1000)       38 2023-06-09 14:49:12.521712 zigzag-dse-2.3.8/setup.cfg
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-06-09 14:49:12.471712 zigzag-dse-2.3.8/zigzag/
+-rw-r--r--   0 asymons   (1000) asymons   (1000)       22 2023-06-09 14:48:50.000000 zigzag-dse-2.3.8/zigzag/__init__.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     2497 2022-11-06 07:09:28.000000 zigzag-dse-2.3.8/zigzag/__main__.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     4451 2023-06-02 14:22:51.000000 zigzag-dse-2.3.8/zigzag/api.py
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-06-09 14:49:12.471712 zigzag-dse-2.3.8/zigzag/classes/
+-rw-r--r--   0 asymons   (1000) asymons   (1000)        0 2022-11-06 21:40:40.000000 zigzag-dse-2.3.8/zigzag/classes/__init__.py
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-06-09 14:49:12.471712 zigzag-dse-2.3.8/zigzag/classes/cacti/
+-rw-r--r--   0 asymons   (1000) asymons   (1000)      291 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/README.md
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-06-09 14:49:12.471712 zigzag-dse-2.3.8/zigzag/classes/cacti/__pycache__/
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     3412 2023-04-22 21:31:11.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/__pycache__/cacti_parser.cpython-310.pyc
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-06-09 14:49:12.491712 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     6576 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/2DDRAM_Samsung2GbDDR2.cfg
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     6555 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/2DDRAM_micron1Gb.cfg
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     6920 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/3DDRAM_Samsung3D8Gb_extened.cfg
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     5324 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/README
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     9282 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/TSV.cc
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     3322 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/TSV.h
+-rw-r--r--   0 asymons   (1000) asymons   (1000)    41184 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/Ucache.cc
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     3607 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/Ucache.h
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-06-09 14:49:12.491712 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/__pycache__/
+-rw-r--r--   0 asymons   (1000) asymons   (1000)    13713 2023-04-16 14:07:27.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/__pycache__/cacti_config_creator.cpython-310.pyc
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     5116 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/arbiter.cc
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     2771 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/arbiter.h
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     2057 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/area.cc
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     2416 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/area.h
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     8474 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/bank.cc
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     2664 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/bank.h
+-rw-r--r--   0 asymons   (1000) asymons   (1000)    29279 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/basic_circuit.cc
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     7364 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/basic_circuit.h
+-rw-r--r--   0 asymons   (1000) asymons   (1000)    11041 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/cache.cfg_temp
+-rw-r--r--   0 asymons   (1000) asymons   (1000)    32713 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/cache_old.cfg.out
+-rwxr-xr-x   0 asymons   (1000) asymons   (1000)  2421320 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/cacti
+-rw-r--r--   0 asymons   (1000) asymons   (1000)      173 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/cacti.i
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     1334 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/cacti.mk
+-rw-r--r--   0 asymons   (1000) asymons   (1000)    25297 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/cacti_config_creator.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     5586 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/cacti_interface.cc
+-rw-r--r--   0 asymons   (1000) asymons   (1000)    27215 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/cacti_interface.h
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     3569 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/cacti_top.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     7561 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/component.cc
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     2837 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/component.h
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     9565 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/const.h
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     5001 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/contention.dat
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     7349 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/crossbar.cc
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     3204 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/crossbar.h
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     9849 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/ddr3.cfg
+-rw-r--r--   0 asymons   (1000) asymons   (1000)    62337 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/decoder.cc
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     7405 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/decoder.h
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     3712 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/dram.cfg
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     9750 2023-04-25 15:05:19.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/example_mem_pool.yaml
+-rw-r--r--   0 asymons   (1000) asymons   (1000)    17411 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/extio.cc
+-rw-r--r--   0 asymons   (1000) asymons   (1000)      878 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/extio.h
+-rw-r--r--   0 asymons   (1000) asymons   (1000)    46185 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/extio_technology.cc
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     9068 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/extio_technology.h
+-rw-r--r--   0 asymons   (1000) asymons   (1000)    23772 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/htree2.cc
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     3595 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/htree2.h
+-rw-r--r--   0 asymons   (1000) asymons   (1000)   133713 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/io.cc
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     2116 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/io.h
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     9850 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/lpddr.cfg
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     7217 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/main.cc
+-rw-r--r--   0 asymons   (1000) asymons   (1000)      407 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/makefile
+-rw-r--r--   0 asymons   (1000) asymons   (1000)    94813 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/mat.cc
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     6122 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/mat.h
+-rw-r--r--   0 asymons   (1000) asymons   (1000)    16630 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/memcad.cc
+-rw-r--r--   0 asymons   (1000) asymons   (1000)      553 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/memcad.h
+-rw-r--r--   0 asymons   (1000) asymons   (1000)    11483 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/memcad_parameters.cc
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     4490 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/memcad_parameters.h
+-rw-r--r--   0 asymons   (1000) asymons   (1000)    29014 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/memorybus.cc
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     5426 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/memorybus.h
+-rw-r--r--   0 asymons   (1000) asymons   (1000)    19629 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/nuca.cc
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     3306 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/nuca.h
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-06-09 14:49:12.501712 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/obj_dbg/
+-rw-r--r--   0 asymons   (1000) asymons   (1000)   134304 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/obj_dbg/TSV.o
+-rw-r--r--   0 asymons   (1000) asymons   (1000)   352744 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/obj_dbg/Ucache.o
+-rw-r--r--   0 asymons   (1000) asymons   (1000)   157960 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/obj_dbg/arbiter.o
+-rw-r--r--   0 asymons   (1000) asymons   (1000)   124352 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/obj_dbg/area.o
+-rw-r--r--   0 asymons   (1000) asymons   (1000)   156624 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/obj_dbg/bank.o
+-rw-r--r--   0 asymons   (1000) asymons   (1000)   155192 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/obj_dbg/basic_circuit.o
+-rwxr-xr-x   0 asymons   (1000) asymons   (1000)  2421320 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/obj_dbg/cacti
+-rw-r--r--   0 asymons   (1000) asymons   (1000)   175768 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/obj_dbg/cacti_interface.o
+-rw-r--r--   0 asymons   (1000) asymons   (1000)   159768 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/obj_dbg/component.o
+-rw-r--r--   0 asymons   (1000) asymons   (1000)   160680 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/obj_dbg/crossbar.o
+-rw-r--r--   0 asymons   (1000) asymons   (1000)   207224 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/obj_dbg/decoder.o
+-rw-r--r--   0 asymons   (1000) asymons   (1000)   145592 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/obj_dbg/extio.o
+-rw-r--r--   0 asymons   (1000) asymons   (1000)   180464 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/obj_dbg/extio_technology.o
+-rw-r--r--   0 asymons   (1000) asymons   (1000)   178384 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/obj_dbg/htree2.o
+-rw-r--r--   0 asymons   (1000) asymons   (1000)   411960 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/obj_dbg/io.o
+-rw-r--r--   0 asymons   (1000) asymons   (1000)   192248 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/obj_dbg/main.o
+-rw-r--r--   0 asymons   (1000) asymons   (1000)   270320 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/obj_dbg/mat.o
+-rw-r--r--   0 asymons   (1000) asymons   (1000)   569648 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/obj_dbg/memcad.o
+-rw-r--r--   0 asymons   (1000) asymons   (1000)   280416 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/obj_dbg/memcad_parameters.o
+-rw-r--r--   0 asymons   (1000) asymons   (1000)   204480 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/obj_dbg/memorybus.o
+-rw-r--r--   0 asymons   (1000) asymons   (1000)   256824 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/obj_dbg/nuca.o
+-rw-r--r--   0 asymons   (1000) asymons   (1000)   313848 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/obj_dbg/parameter.o
+-rw-r--r--   0 asymons   (1000) asymons   (1000)   124400 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/obj_dbg/powergating.o
+-rw-r--r--   0 asymons   (1000) asymons   (1000)   175432 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/obj_dbg/router.o
+-rw-r--r--   0 asymons   (1000) asymons   (1000)   128080 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/obj_dbg/subarray.o
+-rw-r--r--   0 asymons   (1000) asymons   (1000)   144976 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/obj_dbg/technology.o
+-rw-r--r--   0 asymons   (1000) asymons   (1000)   228000 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/obj_dbg/uca.o
+-rw-r--r--   0 asymons   (1000) asymons   (1000)   232752 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/obj_dbg/wire.o
+-rw-r--r--   0 asymons   (1000) asymons   (1000)   111980 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/parameter.cc
+-rw-r--r--   0 asymons   (1000) asymons   (1000)    20306 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/parameter.h
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     5286 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/powergating.cc
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     3055 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/powergating.h
+-rwxr-xr-x   0 asymons   (1000) asymons   (1000)     1886 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/regression.test
+-rw-r--r--   0 asymons   (1000) asymons   (1000)    10212 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/router.cc
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     3721 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/router.h
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-06-09 14:49:12.511712 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/sample_config_files/
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     8781 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/sample_config_files/ddr3_cache.cfg
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     8768 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/sample_config_files/diff_ddr3_cache.cfg
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     8780 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/sample_config_files/lpddr3_cache.cfg
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     8784 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/sample_config_files/wideio_cache.cfg
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-06-09 14:49:12.511712 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/self_gen/
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     9545 2023-04-25 15:05:19.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/self_gen/cache.cfg
+-rw-r--r--   0 asymons   (1000) asymons   (1000)      579 2023-04-25 15:05:19.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/self_gen/cache.cfg.out
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     8332 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/subarray.cc
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     2542 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/subarray.h
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-06-09 14:49:12.511712 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/tech_params/
+-rw-r--r--   0 asymons   (1000) asymons   (1000)       25 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/tech_params/16nm.dat
+-rw-r--r--   0 asymons   (1000) asymons   (1000)    23666 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/tech_params/180nm-old.dat
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     3842 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/tech_params/180nm.dat
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     4575 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/tech_params/22nm.dat
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     4759 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/tech_params/32nm.dat
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     4755 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/tech_params/45nm.dat
+-rw-r--r--   0 asymons   (1000) asymons   (1000)    24571 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/tech_params/65nm-old.dat
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     4758 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/tech_params/65nm.dat
+-rw-r--r--   0 asymons   (1000) asymons   (1000)    24570 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/tech_params/90nm-old.dat
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     4742 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/tech_params/90nm.dat
+-rw-r--r--   0 asymons   (1000) asymons   (1000)    15087 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/technology.cc
+-rw-r--r--   0 asymons   (1000) asymons   (1000)    41317 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/uca.cc
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     4035 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/uca.h
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     2064 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/version_cacti.h
+-rw-r--r--   0 asymons   (1000) asymons   (1000)    29856 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/wire.cc
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     4375 2023-03-27 09:38:39.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/wire.h
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     6110 2023-04-22 12:58:13.000000 zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_parser.py
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-06-09 14:49:12.511712 zigzag-dse-2.3.8/zigzag/classes/cost_model/
+-rw-r--r--   0 asymons   (1000) asymons   (1000)    62023 2023-04-16 12:43:30.000000 zigzag-dse-2.3.8/zigzag/classes/cost_model/cost_model.py
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-06-09 14:49:12.471712 zigzag-dse-2.3.8/zigzag/classes/hardware/
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-06-09 14:49:12.511712 zigzag-dse-2.3.8/zigzag/classes/hardware/architecture/
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     1278 2023-04-16 13:43:29.000000 zigzag-dse-2.3.8/zigzag/classes/hardware/architecture/accelerator.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     9441 2023-04-07 09:22:11.000000 zigzag-dse-2.3.8/zigzag/classes/hardware/architecture/adder_hierarchy.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     6031 2023-04-07 09:22:16.000000 zigzag-dse-2.3.8/zigzag/classes/hardware/architecture/core.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)      918 2023-04-07 09:22:20.000000 zigzag-dse-2.3.8/zigzag/classes/hardware/architecture/dimension.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)    11764 2023-04-07 09:22:26.000000 zigzag-dse-2.3.8/zigzag/classes/hardware/architecture/memory_hierarchy.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     3567 2023-06-02 14:16:12.000000 zigzag-dse-2.3.8/zigzag/classes/hardware/architecture/memory_instance.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)    12231 2023-04-07 09:22:36.000000 zigzag-dse-2.3.8/zigzag/classes/hardware/architecture/memory_level.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     3014 2023-04-07 09:22:40.000000 zigzag-dse-2.3.8/zigzag/classes/hardware/architecture/operational_array.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     1874 2023-04-07 09:22:44.000000 zigzag-dse-2.3.8/zigzag/classes/hardware/architecture/operational_unit.py
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-06-09 14:49:12.471712 zigzag-dse-2.3.8/zigzag/classes/io/
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-06-09 14:49:12.511712 zigzag-dse-2.3.8/zigzag/classes/io/accelerator/
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     2805 2022-11-06 21:24:03.000000 zigzag-dse-2.3.8/zigzag/classes/io/accelerator/parser.py
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-06-09 14:49:12.511712 zigzag-dse-2.3.8/zigzag/classes/io/onnx/
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     7087 2023-06-09 14:32:23.000000 zigzag-dse-2.3.8/zigzag/classes/io/onnx/conv.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)      884 2023-04-07 09:12:40.000000 zigzag-dse-2.3.8/zigzag/classes/io/onnx/default.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     5382 2023-04-07 09:12:45.000000 zigzag-dse-2.3.8/zigzag/classes/io/onnx/gemm.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     3679 2023-04-07 09:12:49.000000 zigzag-dse-2.3.8/zigzag/classes/io/onnx/matmul.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     4912 2023-04-07 09:12:53.000000 zigzag-dse-2.3.8/zigzag/classes/io/onnx/model.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     1163 2023-04-07 09:12:58.000000 zigzag-dse-2.3.8/zigzag/classes/io/onnx/parser.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     4089 2023-06-09 14:32:23.000000 zigzag-dse-2.3.8/zigzag/classes/io/onnx/utils.py
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-06-09 14:49:12.511712 zigzag-dse-2.3.8/zigzag/classes/mapping/
+-rw-r--r--   0 asymons   (1000) asymons   (1000)    40951 2023-04-07 09:24:31.000000 zigzag-dse-2.3.8/zigzag/classes/mapping/combined_mapping.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)      637 2023-04-07 09:24:42.000000 zigzag-dse-2.3.8/zigzag/classes/mapping/loop.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     9386 2023-04-07 09:24:55.000000 zigzag-dse-2.3.8/zigzag/classes/mapping/mapping_assist_funcs.py
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-06-09 14:49:12.511712 zigzag-dse-2.3.8/zigzag/classes/mapping/memory/
+-rw-r--r--   0 asymons   (1000) asymons   (1000)        0 2023-04-07 09:25:08.000000 zigzag-dse-2.3.8/zigzag/classes/mapping/memory/data_layout.py
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-06-09 14:49:12.511712 zigzag-dse-2.3.8/zigzag/classes/mapping/spatial/
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     7655 2023-06-09 14:48:12.000000 zigzag-dse-2.3.8/zigzag/classes/mapping/spatial/spatial_mapping.py
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-06-09 14:49:12.511712 zigzag-dse-2.3.8/zigzag/classes/mapping/temporal/
+-rw-r--r--   0 asymons   (1000) asymons   (1000)      380 2023-04-07 09:25:12.000000 zigzag-dse-2.3.8/zigzag/classes/mapping/temporal/temporal_loop.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     7412 2023-04-07 09:25:16.000000 zigzag-dse-2.3.8/zigzag/classes/mapping/temporal/temporal_mapping.py
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-06-09 14:49:12.471712 zigzag-dse-2.3.8/zigzag/classes/opt/
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-06-09 14:49:12.511712 zigzag-dse-2.3.8/zigzag/classes/opt/spatial/
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     7044 2023-04-07 09:30:21.000000 zigzag-dse-2.3.8/zigzag/classes/opt/spatial/generator.py
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-06-09 14:49:12.471712 zigzag-dse-2.3.8/zigzag/classes/opt/temporal/
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-06-09 14:49:12.511712 zigzag-dse-2.3.8/zigzag/classes/opt/temporal/loma/
+-rw-r--r--   0 asymons   (1000) asymons   (1000)    11591 2023-04-07 09:29:56.000000 zigzag-dse-2.3.8/zigzag/classes/opt/temporal/loma/engine.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)      489 2023-04-07 09:30:00.000000 zigzag-dse-2.3.8/zigzag/classes/opt/temporal/loma/loop.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)    15479 2023-04-07 09:30:04.000000 zigzag-dse-2.3.8/zigzag/classes/opt/temporal/loma/memory_allocator.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     2837 2023-04-07 09:30:07.000000 zigzag-dse-2.3.8/zigzag/classes/opt/temporal/loma/multipermute.py
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-06-09 14:49:12.511712 zigzag-dse-2.3.8/zigzag/classes/opt/temporal/salsa/
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     8726 2023-04-07 09:30:11.000000 zigzag-dse-2.3.8/zigzag/classes/opt/temporal/salsa/engine.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     3616 2023-04-07 09:30:15.000000 zigzag-dse-2.3.8/zigzag/classes/opt/temporal/salsa/state.py
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-06-09 14:49:12.511712 zigzag-dse-2.3.8/zigzag/classes/stages/
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     2054 2023-04-07 09:02:40.000000 zigzag-dse-2.3.8/zigzag/classes/stages/CostModelStage.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     1552 2023-04-07 09:03:00.000000 zigzag-dse-2.3.8/zigzag/classes/stages/DumpStage.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     3240 2023-04-07 09:02:56.000000 zigzag-dse-2.3.8/zigzag/classes/stages/GeneralParameterIteratorStage.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     2105 2023-04-07 09:02:49.000000 zigzag-dse-2.3.8/zigzag/classes/stages/LomaStage.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     2163 2023-04-07 09:27:10.000000 zigzag-dse-2.3.8/zigzag/classes/stages/MainInputParserStages.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)      966 2023-04-07 09:03:11.000000 zigzag-dse-2.3.8/zigzag/classes/stages/ONNXModelParserStage.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     1568 2023-04-07 09:03:29.000000 zigzag-dse-2.3.8/zigzag/classes/stages/PlotTemporalMappingsStage.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     6204 2023-04-07 09:03:44.000000 zigzag-dse-2.3.8/zigzag/classes/stages/ReduceStages.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     6260 2023-04-07 09:03:58.000000 zigzag-dse-2.3.8/zigzag/classes/stages/RunOptStages.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     6546 2023-04-07 09:04:04.000000 zigzag-dse-2.3.8/zigzag/classes/stages/SalsaStage.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     6997 2023-04-15 12:05:47.000000 zigzag-dse-2.3.8/zigzag/classes/stages/SaveStage.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     8158 2023-04-07 09:04:25.000000 zigzag-dse-2.3.8/zigzag/classes/stages/SpatialMappingConversionStage.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     3906 2023-04-07 09:05:11.000000 zigzag-dse-2.3.8/zigzag/classes/stages/SpatialMappingGeneratorStage.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     2593 2023-04-07 09:05:30.000000 zigzag-dse-2.3.8/zigzag/classes/stages/Stage.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     4046 2023-04-07 09:05:44.000000 zigzag-dse-2.3.8/zigzag/classes/stages/TemporalOrderingConversionStage.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     1187 2023-04-07 09:05:50.000000 zigzag-dse-2.3.8/zigzag/classes/stages/WorkloadStage.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     2821 2023-04-07 09:28:15.000000 zigzag-dse-2.3.8/zigzag/classes/stages/__init__.py
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-06-09 14:49:12.521712 zigzag-dse-2.3.8/zigzag/classes/workload/
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     2468 2023-04-07 09:17:48.000000 zigzag-dse-2.3.8/zigzag/classes/workload/dnn_workload.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     2210 2023-04-07 09:17:53.000000 zigzag-dse-2.3.8/zigzag/classes/workload/dummy_node.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)    21102 2023-04-07 09:19:32.000000 zigzag-dse-2.3.8/zigzag/classes/workload/layer_node.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     1542 2023-04-07 09:18:04.000000 zigzag-dse-2.3.8/zigzag/classes/workload/onnx_workload.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)    14521 2023-04-07 09:18:09.000000 zigzag-dse-2.3.8/zigzag/classes/workload/test_layer_node.py
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-06-09 14:49:12.471712 zigzag-dse-2.3.8/zigzag/inputs/
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-06-09 14:49:12.471712 zigzag-dse-2.3.8/zigzag/inputs/examples/
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-06-09 14:49:12.521712 zigzag-dse-2.3.8/zigzag/inputs/examples/hardware/
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     8448 2023-04-16 14:01:57.000000 zigzag-dse-2.3.8/zigzag/inputs/examples/hardware/Ascend_like.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     5849 2023-04-16 14:01:57.000000 zigzag-dse-2.3.8/zigzag/inputs/examples/hardware/Edge_TPU_like.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     5746 2023-04-16 14:01:57.000000 zigzag-dse-2.3.8/zigzag/inputs/examples/hardware/Eyeriss_like.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     7098 2023-04-16 14:01:57.000000 zigzag-dse-2.3.8/zigzag/inputs/examples/hardware/Meta_prototype.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     5112 2023-04-16 14:01:57.000000 zigzag-dse-2.3.8/zigzag/inputs/examples/hardware/TPU_like.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     7287 2023-04-16 14:01:57.000000 zigzag-dse-2.3.8/zigzag/inputs/examples/hardware/Tesla_NPU_like.py
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-06-09 14:49:12.521712 zigzag-dse-2.3.8/zigzag/inputs/examples/mapping/
+-rw-r--r--   0 asymons   (1000) asymons   (1000)      561 2023-04-15 09:48:43.000000 zigzag-dse-2.3.8/zigzag/inputs/examples/mapping/assend_like.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)      196 2023-04-15 09:48:46.000000 zigzag-dse-2.3.8/zigzag/inputs/examples/mapping/default.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)      832 2023-04-15 09:48:50.000000 zigzag-dse-2.3.8/zigzag/inputs/examples/mapping/edge_tpu_like.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)      560 2023-04-15 09:48:52.000000 zigzag-dse-2.3.8/zigzag/inputs/examples/mapping/meta_prototype_like.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)      610 2023-04-15 09:48:56.000000 zigzag-dse-2.3.8/zigzag/inputs/examples/mapping/tesla_npu_like.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)      557 2023-04-15 09:49:08.000000 zigzag-dse-2.3.8/zigzag/inputs/examples/mapping/tpu_like.py
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-06-09 14:49:12.521712 zigzag-dse-2.3.8/zigzag/inputs/examples/workload/
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     4067 2023-01-16 14:56:40.000000 zigzag-dse-2.3.8/zigzag/inputs/examples/workload/alexnet.onnx
+-rw-r--r--   0 asymons   (1000) asymons   (1000)    71724 2022-12-09 21:20:28.000000 zigzag-dse-2.3.8/zigzag/inputs/examples/workload/mobilenetv2.onnx
+-rw-r--r--   0 asymons   (1000) asymons   (1000)    18600 2023-04-15 09:55:05.000000 zigzag-dse-2.3.8/zigzag/inputs/examples/workload/resnet18.onnx
+-rw-r--r--   0 asymons   (1000) asymons   (1000)    19065 2023-04-15 09:49:14.000000 zigzag-dse-2.3.8/zigzag/inputs/examples/workload/resnet18.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)      504 2022-10-27 21:43:16.000000 zigzag-dse-2.3.8/zigzag/utils.py
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-06-09 14:49:12.471712 zigzag-dse-2.3.8/zigzag/visualization/
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-06-09 14:49:12.521712 zigzag-dse-2.3.8/zigzag/visualization/graph/
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     1527 2023-04-15 09:49:36.000000 zigzag-dse-2.3.8/zigzag/visualization/graph/memory_hierarchy.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     1280 2023-04-15 09:49:41.000000 zigzag-dse-2.3.8/zigzag/visualization/graph/workload.py
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-06-09 14:49:12.521712 zigzag-dse-2.3.8/zigzag/visualization/results/
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     8773 2023-04-16 16:18:26.000000 zigzag-dse-2.3.8/zigzag/visualization/results/plot_cme.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     3951 2023-04-15 09:49:53.000000 zigzag-dse-2.3.8/zigzag/visualization/results/print_mapping.py
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-06-09 14:49:12.521712 zigzag-dse-2.3.8/zigzag_dse.egg-info/
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     9080 2023-06-09 14:49:12.000000 zigzag-dse-2.3.8/zigzag_dse.egg-info/PKG-INFO
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     9580 2023-06-09 14:49:12.000000 zigzag-dse-2.3.8/zigzag_dse.egg-info/SOURCES.txt
+-rw-r--r--   0 asymons   (1000) asymons   (1000)        1 2023-06-09 14:49:12.000000 zigzag-dse-2.3.8/zigzag_dse.egg-info/dependency_links.txt
+-rw-r--r--   0 asymons   (1000) asymons   (1000)       52 2023-06-09 14:49:12.000000 zigzag-dse-2.3.8/zigzag_dse.egg-info/entry_points.txt
+-rw-r--r--   0 asymons   (1000) asymons   (1000)      144 2023-06-09 14:49:12.000000 zigzag-dse-2.3.8/zigzag_dse.egg-info/requires.txt
+-rw-r--r--   0 asymons   (1000) asymons   (1000)       27 2023-06-09 14:49:12.000000 zigzag-dse-2.3.8/zigzag_dse.egg-info/top_level.txt
```

### Comparing `zigzag-dse-2.3.7/LICENSE` & `zigzag-dse-2.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/PKG-INFO` & `zigzag-dse-2.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zigzag-dse
-Version: 2.3.7
+Version: 2.3.8
 Summary: ZigZag - Deep Learning Hardware Design Space Exploration
 Author-email: Arne Symons <arne.symons@kuleuven.be>, Linyan Mei <linyan.mei@kuleuven.be>
 License: BSD 3-Clause License
         
         Copyright (c) 2021, ZigZag-Project
         All rights reserved.
```

### Comparing `zigzag-dse-2.3.7/README.md` & `zigzag-dse-2.3.8/README.md`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/docs/source/conf.py` & `zigzag-dse-2.3.8/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/pyproject.toml` & `zigzag-dse-2.3.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 where = ["."]  # ["."] by default
 include = ["*"]  # ["*"] by default
 exclude = ["inputs*", "outputs*", "docs*"]
 namespaces = true  # true by default
 
 [project]
 name = "zigzag-dse"
-version = "2.3.7"
+version = "2.3.8"
 description = "ZigZag - Deep Learning Hardware Design Space Exploration"
 readme = "README.md"
 authors = [{ name = "Arne Symons", email = "arne.symons@kuleuven.be" }, { name = "Linyan Mei", email = "linyan.mei@kuleuven.be" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: BSD License",
     "Programming Language :: Python",
@@ -41,15 +41,15 @@
 [project.urls]
 Homepage = "https://github.com/ZigZag-Project/zigzag"
 
 [project.scripts]
 realpython = "zigzag.__main__:main"
 
 [tool.bumpver]
-current_version = "2.3.7"
+current_version = "2.3.8"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `zigzag-dse-2.3.7/zigzag/__main__.py` & `zigzag-dse-2.3.8/zigzag/__main__.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/api.py` & `zigzag-dse-2.3.8/zigzag/api.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/__pycache__/cacti_parser.cpython-310.pyc` & `zigzag-dse-2.3.8/zigzag/classes/cacti/__pycache__/cacti_parser.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/2DDRAM_Samsung2GbDDR2.cfg` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/2DDRAM_Samsung2GbDDR2.cfg`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/2DDRAM_micron1Gb.cfg` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/2DDRAM_micron1Gb.cfg`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/3DDRAM_Samsung3D8Gb_extened.cfg` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/3DDRAM_Samsung3D8Gb_extened.cfg`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/README` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/README`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/TSV.cc` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/TSV.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/TSV.h` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/TSV.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/Ucache.cc` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/Ucache.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/Ucache.h` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/Ucache.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/__pycache__/cacti_config_creator.cpython-310.pyc` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/__pycache__/cacti_config_creator.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/arbiter.cc` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/arbiter.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/arbiter.h` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/arbiter.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/area.cc` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/area.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/area.h` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/area.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/bank.cc` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/bank.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/bank.h` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/bank.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/basic_circuit.cc` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/basic_circuit.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/basic_circuit.h` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/basic_circuit.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/cache.cfg_temp` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/cache.cfg_temp`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/cache_old.cfg.out` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/cache_old.cfg.out`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/cacti` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/cacti`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/cacti.mk` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/cacti.mk`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/cacti_config_creator.py` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/cacti_config_creator.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/cacti_interface.cc` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/cacti_interface.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/cacti_interface.h` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/cacti_interface.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/cacti_top.py` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/cacti_top.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/component.cc` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/component.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/component.h` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/component.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/const.h` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/const.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/contention.dat` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/contention.dat`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/crossbar.cc` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/crossbar.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/crossbar.h` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/crossbar.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/ddr3.cfg` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/ddr3.cfg`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/decoder.cc` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/decoder.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/decoder.h` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/decoder.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/dram.cfg` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/dram.cfg`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/example_mem_pool.yaml` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/example_mem_pool.yaml`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/extio.cc` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/extio.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/extio.h` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/extio.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/extio_technology.cc` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/extio_technology.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/extio_technology.h` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/extio_technology.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/htree2.cc` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/htree2.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/htree2.h` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/htree2.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/io.cc` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/io.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/io.h` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/io.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/lpddr.cfg` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/lpddr.cfg`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/main.cc` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/main.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/mat.cc` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/mat.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/mat.h` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/mat.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/memcad.cc` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/memcad.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/memcad.h` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/memcad.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/memcad_parameters.cc` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/memcad_parameters.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/memcad_parameters.h` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/memcad_parameters.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/memorybus.cc` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/memorybus.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/memorybus.h` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/memorybus.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/nuca.cc` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/nuca.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/nuca.h` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/nuca.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/obj_dbg/TSV.o` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/obj_dbg/TSV.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/obj_dbg/Ucache.o` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/obj_dbg/Ucache.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/obj_dbg/arbiter.o` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/obj_dbg/arbiter.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/obj_dbg/area.o` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/obj_dbg/area.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/obj_dbg/bank.o` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/obj_dbg/bank.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/obj_dbg/basic_circuit.o` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/obj_dbg/basic_circuit.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/obj_dbg/cacti` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/obj_dbg/cacti`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/obj_dbg/cacti_interface.o` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/obj_dbg/cacti_interface.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/obj_dbg/component.o` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/obj_dbg/component.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/obj_dbg/crossbar.o` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/obj_dbg/crossbar.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/obj_dbg/decoder.o` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/obj_dbg/decoder.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/obj_dbg/extio.o` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/obj_dbg/extio.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/obj_dbg/extio_technology.o` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/obj_dbg/extio_technology.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/obj_dbg/htree2.o` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/obj_dbg/htree2.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/obj_dbg/io.o` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/obj_dbg/io.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/obj_dbg/main.o` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/obj_dbg/main.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/obj_dbg/mat.o` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/obj_dbg/mat.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/obj_dbg/memcad.o` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/obj_dbg/memcad.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/obj_dbg/memcad_parameters.o` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/obj_dbg/memcad_parameters.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/obj_dbg/memorybus.o` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/obj_dbg/memorybus.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/obj_dbg/nuca.o` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/obj_dbg/nuca.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/obj_dbg/parameter.o` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/obj_dbg/parameter.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/obj_dbg/powergating.o` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/obj_dbg/powergating.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/obj_dbg/router.o` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/obj_dbg/router.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/obj_dbg/subarray.o` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/obj_dbg/subarray.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/obj_dbg/technology.o` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/obj_dbg/technology.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/obj_dbg/uca.o` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/obj_dbg/uca.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/obj_dbg/wire.o` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/obj_dbg/wire.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/parameter.cc` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/parameter.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/parameter.h` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/parameter.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/powergating.cc` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/powergating.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/powergating.h` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/powergating.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/regression.test` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/regression.test`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/router.cc` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/router.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/router.h` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/router.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/sample_config_files/ddr3_cache.cfg` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/sample_config_files/ddr3_cache.cfg`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/sample_config_files/diff_ddr3_cache.cfg` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/sample_config_files/diff_ddr3_cache.cfg`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/sample_config_files/lpddr3_cache.cfg` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/sample_config_files/lpddr3_cache.cfg`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/sample_config_files/wideio_cache.cfg` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/sample_config_files/wideio_cache.cfg`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/self_gen/cache.cfg` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/self_gen/cache.cfg`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/self_gen/cache.cfg.out` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/self_gen/cache.cfg.out`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/subarray.cc` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/subarray.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/subarray.h` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/subarray.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/tech_params/180nm-old.dat` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/tech_params/180nm-old.dat`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/tech_params/180nm.dat` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/tech_params/180nm.dat`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/tech_params/22nm.dat` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/tech_params/22nm.dat`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/tech_params/32nm.dat` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/tech_params/32nm.dat`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/tech_params/45nm.dat` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/tech_params/45nm.dat`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/tech_params/65nm-old.dat` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/tech_params/65nm-old.dat`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/tech_params/65nm.dat` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/tech_params/65nm.dat`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/tech_params/90nm-old.dat` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/tech_params/90nm-old.dat`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/tech_params/90nm.dat` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/tech_params/90nm.dat`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/technology.cc` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/technology.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/uca.cc` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/uca.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/uca.h` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/uca.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/version_cacti.h` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/version_cacti.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/wire.cc` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/wire.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_master/wire.h` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_master/wire.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cacti/cacti_parser.py` & `zigzag-dse-2.3.8/zigzag/classes/cacti/cacti_parser.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/cost_model/cost_model.py` & `zigzag-dse-2.3.8/zigzag/classes/cost_model/cost_model.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/hardware/architecture/accelerator.py` & `zigzag-dse-2.3.8/zigzag/classes/hardware/architecture/accelerator.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/hardware/architecture/adder_hierarchy.py` & `zigzag-dse-2.3.8/zigzag/classes/hardware/architecture/adder_hierarchy.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/hardware/architecture/core.py` & `zigzag-dse-2.3.8/zigzag/classes/hardware/architecture/core.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/hardware/architecture/dimension.py` & `zigzag-dse-2.3.8/zigzag/classes/hardware/architecture/dimension.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/hardware/architecture/memory_hierarchy.py` & `zigzag-dse-2.3.8/zigzag/classes/hardware/architecture/memory_hierarchy.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/hardware/architecture/memory_instance.py` & `zigzag-dse-2.3.8/zigzag/classes/hardware/architecture/memory_instance.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/hardware/architecture/memory_level.py` & `zigzag-dse-2.3.8/zigzag/classes/hardware/architecture/memory_level.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/hardware/architecture/operational_array.py` & `zigzag-dse-2.3.8/zigzag/classes/hardware/architecture/operational_array.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/hardware/architecture/operational_unit.py` & `zigzag-dse-2.3.8/zigzag/classes/hardware/architecture/operational_unit.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/io/accelerator/parser.py` & `zigzag-dse-2.3.8/zigzag/classes/io/accelerator/parser.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/io/onnx/conv.py` & `zigzag-dse-2.3.8/zigzag/classes/io/onnx/conv.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/io/onnx/default.py` & `zigzag-dse-2.3.8/zigzag/classes/io/onnx/default.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/io/onnx/gemm.py` & `zigzag-dse-2.3.8/zigzag/classes/io/onnx/gemm.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/io/onnx/matmul.py` & `zigzag-dse-2.3.8/zigzag/classes/io/onnx/matmul.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/io/onnx/model.py` & `zigzag-dse-2.3.8/zigzag/classes/io/onnx/model.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/io/onnx/parser.py` & `zigzag-dse-2.3.8/zigzag/classes/io/onnx/parser.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/io/onnx/utils.py` & `zigzag-dse-2.3.8/zigzag/classes/io/onnx/utils.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/mapping/combined_mapping.py` & `zigzag-dse-2.3.8/zigzag/classes/mapping/combined_mapping.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/mapping/loop.py` & `zigzag-dse-2.3.8/zigzag/classes/mapping/loop.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/mapping/mapping_assist_funcs.py` & `zigzag-dse-2.3.8/zigzag/classes/mapping/mapping_assist_funcs.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/mapping/spatial/spatial_mapping.py` & `zigzag-dse-2.3.8/zigzag/classes/mapping/spatial/spatial_mapping.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,15 @@
         Calculate total/unique/duplicate unit count per operand per architecture level
         """
         """ Number of unit at each level (for each operand) """
         # Added round call as number doesn't remain integer due to self.mapping_dict_reform number instability
         unit_count = {
             op: [
                 round(
-                    round(prod(self.unroll_size_total[op][lv : self.arch_level[op]])), 3
+                    round(prod(self.unroll_size_total[op][lv : self.arch_level[op]]), 3)
                 )
                 for lv in range(self.arch_level[op])
             ]
             for op in self.operand_list
         }
 
         """ ASSERT: The bottom level (MAC level) unit count must be the same for all operand """
```

### Comparing `zigzag-dse-2.3.7/zigzag/classes/mapping/temporal/temporal_mapping.py` & `zigzag-dse-2.3.8/zigzag/classes/mapping/temporal/temporal_mapping.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/opt/spatial/generator.py` & `zigzag-dse-2.3.8/zigzag/classes/opt/spatial/generator.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/opt/temporal/loma/engine.py` & `zigzag-dse-2.3.8/zigzag/classes/opt/temporal/loma/engine.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/opt/temporal/loma/memory_allocator.py` & `zigzag-dse-2.3.8/zigzag/classes/opt/temporal/loma/memory_allocator.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/opt/temporal/loma/multipermute.py` & `zigzag-dse-2.3.8/zigzag/classes/opt/temporal/loma/multipermute.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/opt/temporal/salsa/engine.py` & `zigzag-dse-2.3.8/zigzag/classes/opt/temporal/salsa/engine.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/opt/temporal/salsa/state.py` & `zigzag-dse-2.3.8/zigzag/classes/opt/temporal/salsa/state.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/stages/CostModelStage.py` & `zigzag-dse-2.3.8/zigzag/classes/stages/CostModelStage.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/stages/DumpStage.py` & `zigzag-dse-2.3.8/zigzag/classes/stages/DumpStage.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/stages/GeneralParameterIteratorStage.py` & `zigzag-dse-2.3.8/zigzag/classes/stages/GeneralParameterIteratorStage.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/stages/LomaStage.py` & `zigzag-dse-2.3.8/zigzag/classes/stages/LomaStage.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/stages/MainInputParserStages.py` & `zigzag-dse-2.3.8/zigzag/classes/stages/MainInputParserStages.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/stages/ONNXModelParserStage.py` & `zigzag-dse-2.3.8/zigzag/classes/stages/ONNXModelParserStage.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/stages/PlotTemporalMappingsStage.py` & `zigzag-dse-2.3.8/zigzag/classes/stages/PlotTemporalMappingsStage.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/stages/ReduceStages.py` & `zigzag-dse-2.3.8/zigzag/classes/stages/ReduceStages.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/stages/RunOptStages.py` & `zigzag-dse-2.3.8/zigzag/classes/stages/RunOptStages.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/stages/SalsaStage.py` & `zigzag-dse-2.3.8/zigzag/classes/stages/SalsaStage.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/stages/SaveStage.py` & `zigzag-dse-2.3.8/zigzag/classes/stages/SaveStage.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/stages/SpatialMappingConversionStage.py` & `zigzag-dse-2.3.8/zigzag/classes/stages/SpatialMappingConversionStage.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/stages/SpatialMappingGeneratorStage.py` & `zigzag-dse-2.3.8/zigzag/classes/stages/SpatialMappingGeneratorStage.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/stages/Stage.py` & `zigzag-dse-2.3.8/zigzag/classes/stages/Stage.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/stages/TemporalOrderingConversionStage.py` & `zigzag-dse-2.3.8/zigzag/classes/stages/TemporalOrderingConversionStage.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/stages/WorkloadStage.py` & `zigzag-dse-2.3.8/zigzag/classes/stages/WorkloadStage.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/stages/__init__.py` & `zigzag-dse-2.3.8/zigzag/classes/stages/__init__.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/workload/dnn_workload.py` & `zigzag-dse-2.3.8/zigzag/classes/workload/dnn_workload.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/workload/dummy_node.py` & `zigzag-dse-2.3.8/zigzag/classes/workload/dummy_node.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/workload/layer_node.py` & `zigzag-dse-2.3.8/zigzag/classes/workload/layer_node.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/workload/onnx_workload.py` & `zigzag-dse-2.3.8/zigzag/classes/workload/onnx_workload.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/classes/workload/test_layer_node.py` & `zigzag-dse-2.3.8/zigzag/classes/workload/test_layer_node.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/inputs/examples/hardware/Ascend_like.py` & `zigzag-dse-2.3.8/zigzag/inputs/examples/hardware/Ascend_like.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/inputs/examples/hardware/Edge_TPU_like.py` & `zigzag-dse-2.3.8/zigzag/inputs/examples/hardware/Edge_TPU_like.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/inputs/examples/hardware/Eyeriss_like.py` & `zigzag-dse-2.3.8/zigzag/inputs/examples/hardware/Eyeriss_like.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/inputs/examples/hardware/Meta_prototype.py` & `zigzag-dse-2.3.8/zigzag/inputs/examples/hardware/Meta_prototype.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/inputs/examples/hardware/TPU_like.py` & `zigzag-dse-2.3.8/zigzag/inputs/examples/hardware/TPU_like.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/inputs/examples/hardware/Tesla_NPU_like.py` & `zigzag-dse-2.3.8/zigzag/inputs/examples/hardware/Tesla_NPU_like.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/inputs/examples/mapping/assend_like.py` & `zigzag-dse-2.3.8/zigzag/inputs/examples/mapping/assend_like.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/inputs/examples/mapping/edge_tpu_like.py` & `zigzag-dse-2.3.8/zigzag/inputs/examples/mapping/edge_tpu_like.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/inputs/examples/mapping/meta_prototype_like.py` & `zigzag-dse-2.3.8/zigzag/inputs/examples/mapping/meta_prototype_like.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/inputs/examples/mapping/tesla_npu_like.py` & `zigzag-dse-2.3.8/zigzag/inputs/examples/mapping/tesla_npu_like.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/inputs/examples/mapping/tpu_like.py` & `zigzag-dse-2.3.8/zigzag/inputs/examples/mapping/tpu_like.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/inputs/examples/workload/alexnet.onnx` & `zigzag-dse-2.3.8/zigzag/inputs/examples/workload/alexnet.onnx`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/inputs/examples/workload/mobilenetv2.onnx` & `zigzag-dse-2.3.8/zigzag/inputs/examples/workload/mobilenetv2.onnx`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/inputs/examples/workload/resnet18.onnx` & `zigzag-dse-2.3.8/zigzag/inputs/examples/workload/resnet18.onnx`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/inputs/examples/workload/resnet18.py` & `zigzag-dse-2.3.8/zigzag/inputs/examples/workload/resnet18.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/visualization/graph/memory_hierarchy.py` & `zigzag-dse-2.3.8/zigzag/visualization/graph/memory_hierarchy.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/visualization/graph/workload.py` & `zigzag-dse-2.3.8/zigzag/visualization/graph/workload.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/visualization/results/plot_cme.py` & `zigzag-dse-2.3.8/zigzag/visualization/results/plot_cme.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag/visualization/results/print_mapping.py` & `zigzag-dse-2.3.8/zigzag/visualization/results/print_mapping.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.7/zigzag_dse.egg-info/PKG-INFO` & `zigzag-dse-2.3.8/zigzag_dse.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zigzag-dse
-Version: 2.3.7
+Version: 2.3.8
 Summary: ZigZag - Deep Learning Hardware Design Space Exploration
 Author-email: Arne Symons <arne.symons@kuleuven.be>, Linyan Mei <linyan.mei@kuleuven.be>
 License: BSD 3-Clause License
         
         Copyright (c) 2021, ZigZag-Project
         All rights reserved.
```

### Comparing `zigzag-dse-2.3.7/zigzag_dse.egg-info/SOURCES.txt` & `zigzag-dse-2.3.8/zigzag_dse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

