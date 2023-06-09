# Comparing `tmp/memray-1.7.0.tar.gz` & `tmp/memray-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "memray-1.7.0.tar", last modified: Tue Feb 21 20:08:39 2023, max compression
+gzip compressed data, was "memray-1.8.0.tar", last modified: Fri Jun  9 19:55:08 2023, max compression
```

## Comparing `memray-1.7.0.tar` & `memray-1.8.0.tar`

### file list

```diff
@@ -1,220 +1,224 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 20:08:39.095390 memray-1.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-02-21 20:08:25.000000 memray-1.7.0/.babelrc
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-02-21 20:08:25.000000 memray-1.7.0/.bumpversion.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-02-21 20:08:25.000000 memray-1.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-02-21 20:08:25.000000 memray-1.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7677 2023-02-21 20:08:25.000000 memray-1.7.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    12482 2023-02-21 20:08:25.000000 memray-1.7.0/NEWS.rst
--rw-r--r--   0 runner    (1001) docker     (123)    16811 2023-02-21 20:08:39.095390 memray-1.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15895 2023-02-21 20:08:25.000000 memray-1.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)   531280 2023-02-21 20:08:25.000000 memray-1.7.0/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-02-21 20:08:25.000000 memray-1.7.0/package.json
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-02-21 20:08:25.000000 memray-1.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-02-21 20:08:39.095390 memray-1.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    10117 2023-02-21 20:08:25.000000 memray-1.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 20:08:39.063387 memray-1.7.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 20:08:39.067387 memray-1.7.0/src/memray/
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-02-21 20:08:25.000000 memray-1.7.0/src/memray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-02-21 20:08:25.000000 memray-1.7.0/src/memray/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-02-21 20:08:25.000000 memray-1.7.0/src/memray/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-02-21 20:08:25.000000 memray-1.7.0/src/memray/_destination.py
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-02-21 20:08:25.000000 memray-1.7.0/src/memray/_errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 20:08:39.067387 memray-1.7.0/src/memray/_ipython/
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-02-21 20:08:25.000000 memray-1.7.0/src/memray/_ipython/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5683 2023-02-21 20:08:25.000000 memray-1.7.0/src/memray/_ipython/flamegraph.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 20:08:39.079388 memray-1.7.0/src/memray/_memray/
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-02-21 20:08:25.000000 memray-1.7.0/src/memray/_memray/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 20:08:25.000000 memray-1.7.0/src/memray/_memray/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-02-21 20:08:25.000000 memray-1.7.0/src/memray/_memray/algorithm.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-02-21 20:08:25.000000 memray-1.7.0/src/memray/_memray/alloc.h
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-02-21 20:08:25.000000 memray-1.7.0/src/memray/_memray/alloc.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-02-21 20:08:25.000000 memray-1.7.0/src/memray/_memray/compat.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-02-21 20:08:25.000000 memray-1.7.0/src/memray/_memray/compat.h
--rw-r--r--   0 runner    (1001) docker     (123)     7114 2023-02-21 20:08:25.000000 memray-1.7.0/src/memray/_memray/elf_shenanigans.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     9617 2023-02-21 20:08:25.000000 memray-1.7.0/src/memray/_memray/elf_utils.h
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-02-21 20:08:25.000000 memray-1.7.0/src/memray/_memray/exceptions.h
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-02-21 20:08:25.000000 memray-1.7.0/src/memray/_memray/frame_tree.h
--rw-r--r--   0 runner    (1001) docker     (123)     9191 2023-02-21 20:08:25.000000 memray-1.7.0/src/memray/_memray/hooks.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6052 2023-02-21 20:08:25.000000 memray-1.7.0/src/memray/_memray/hooks.h
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-02-21 20:08:25.000000 memray-1.7.0/src/memray/_memray/hooks.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     5613 2023-02-21 20:08:25.000000 memray-1.7.0/src/memray/_memray/inject.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-02-21 20:08:25.000000 memray-1.7.0/src/memray/_memray/linker_shenanigans.h
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-02-21 20:08:25.000000 memray-1.7.0/src/memray/_memray/logging.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-02-21 20:08:25.000000 memray-1.7.0/src/memray/_memray/logging.h
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-02-21 20:08:25.000000 memray-1.7.0/src/memray/_memray/logging.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     9616 2023-02-21 20:08:25.000000 memray-1.7.0/src/memray/_memray/lz4_stream.h
--rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-02-21 20:08:25.000000 memray-1.7.0/src/memray/_memray/macho_shenanigans.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-02-21 20:08:25.000000 memray-1.7.0/src/memray/_memray/macho_utils.h
--rw-r--r--   0 runner    (1001) docker     (123)    15624 2023-02-21 20:08:25.000000 memray-1.7.0/src/memray/_memray/native_resolver.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-02-21 20:08:25.000000 memray-1.7.0/src/memray/_memray/native_resolver.h
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-02-21 20:08:25.000000 memray-1.7.0/src/memray/_memray/native_resolver.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-02-21 20:08:25.000000 memray-1.7.0/src/memray/_memray/pthread.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-02-21 20:08:25.000000 memray-1.7.0/src/memray/_memray/python_helpers.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-02-21 20:08:25.000000 memray-1.7.0/src/memray/_memray/python_helpers.h
--rw-r--r--   0 runner    (1001) docker     (123)    42874 2023-02-21 20:08:25.000000 memray-1.7.0/src/memray/_memray/record_reader.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6855 2023-02-21 20:08:25.000000 memray-1.7.0/src/memray/_memray/record_reader.h
--rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-02-21 20:08:25.000000 memray-1.7.0/src/memray/_memray/record_reader.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    20474 2023-02-21 20:08:25.000000 memray-1.7.0/src/memray/_memray/record_writer.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-02-21 20:08:25.000000 memray-1.7.0/src/memray/_memray/record_writer.h
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-02-21 20:08:25.000000 memray-1.7.0/src/memray/_memray/record_writer.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-02-21 20:08:25.000000 memray-1.7.0/src/memray/_memray/records.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     8453 2023-02-21 20:08:25.000000 memray-1.7.0/src/memray/_memray/records.h
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-02-21 20:08:25.000000 memray-1.7.0/src/memray/_memray/records.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    10139 2023-02-21 20:08:25.000000 memray-1.7.0/src/memray/_memray/sink.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-02-21 20:08:25.000000 memray-1.7.0/src/memray/_memray/sink.h
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-02-21 20:08:25.000000 memray-1.7.0/src/memray/_memray/sink.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    19094 2023-02-21 20:08:25.000000 memray-1.7.0/src/memray/_memray/snapshot.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    13891 2023-02-21 20:08:25.000000 memray-1.7.0/src/memray/_memray/snapshot.h
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-02-21 20:08:25.000000 memray-1.7.0/src/memray/_memray/snapshot.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-02-21 20:08:25.000000 memray-1.7.0/src/memray/_memray/socket_reader_thread.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-02-21 20:08:25.000000 memray-1.7.0/src/memray/_memray/socket_reader_thread.h
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-02-21 20:08:25.000000 memray-1.7.0/src/memray/_memray/socket_reader_thread.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     7433 2023-02-21 20:08:25.000000 memray-1.7.0/src/memray/_memray/source.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-02-21 20:08:25.000000 memray-1.7.0/src/memray/_memray/source.h
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-02-21 20:08:25.000000 memray-1.7.0/src/memray/_memray/source.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    36606 2023-02-21 20:08:25.000000 memray-1.7.0/src/memray/_memray/tracking_api.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    11255 2023-02-21 20:08:25.000000 memray-1.7.0/src/memray/_memray/tracking_api.h
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-02-21 20:08:25.000000 memray-1.7.0/src/memray/_memray/tracking_api.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     5906 2023-02-21 20:08:25.000000 memray-1.7.0/src/memray/_memray.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    41959 2023-02-21 20:08:25.000000 memray-1.7.0/src/memray/_memray.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     8577 2023-02-21 20:08:25.000000 memray-1.7.0/src/memray/_memray_test_utils.pyx
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-02-21 20:08:25.000000 memray-1.7.0/src/memray/_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-02-21 20:08:25.000000 memray-1.7.0/src/memray/_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-02-21 20:08:25.000000 memray-1.7.0/src/memray/_stats.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-02-21 20:08:25.000000 memray-1.7.0/src/memray/_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-02-21 20:08:25.000000 memray-1.7.0/src/memray/_test_utils.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-21 20:08:25.000000 memray-1.7.0/src/memray/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 20:08:39.079388 memray-1.7.0/src/memray/commands/
--rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-02-21 20:08:25.000000 memray-1.7.0/src/memray/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-02-21 20:08:25.000000 memray-1.7.0/src/memray/commands/_attach.gdb
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-02-21 20:08:25.000000 memray-1.7.0/src/memray/commands/_attach.lldb
--rw-r--r--   0 runner    (1001) docker     (123)    12367 2023-02-21 20:08:25.000000 memray-1.7.0/src/memray/commands/attach.py
--rw-r--r--   0 runner    (1001) docker     (123)     6221 2023-02-21 20:08:25.000000 memray-1.7.0/src/memray/commands/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-02-21 20:08:25.000000 memray-1.7.0/src/memray/commands/flamegraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-02-21 20:08:25.000000 memray-1.7.0/src/memray/commands/live.py
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-02-21 20:08:25.000000 memray-1.7.0/src/memray/commands/parse.py
--rw-r--r--   0 runner    (1001) docker     (123)    11086 2023-02-21 20:08:25.000000 memray-1.7.0/src/memray/commands/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-02-21 20:08:25.000000 memray-1.7.0/src/memray/commands/stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-02-21 20:08:25.000000 memray-1.7.0/src/memray/commands/summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-02-21 20:08:25.000000 memray-1.7.0/src/memray/commands/table.py
--rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-02-21 20:08:25.000000 memray-1.7.0/src/memray/commands/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     3627 2023-02-21 20:08:25.000000 memray-1.7.0/src/memray/commands/tree.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 20:08:25.000000 memray-1.7.0/src/memray/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 20:08:39.079388 memray-1.7.0/src/memray/reporters/
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-02-21 20:08:25.000000 memray-1.7.0/src/memray/reporters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 20:08:39.083389 memray-1.7.0/src/memray/reporters/assets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 20:08:25.000000 memray-1.7.0/src/memray/reporters/assets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5569 2023-02-21 20:08:25.000000 memray-1.7.0/src/memray/reporters/assets/common.js
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-02-21 20:08:25.000000 memray-1.7.0/src/memray/reporters/assets/common.test.js
--rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-02-21 20:08:25.000000 memray-1.7.0/src/memray/reporters/assets/flamegraph.js
--rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-02-21 20:08:25.000000 memray-1.7.0/src/memray/reporters/assets/flamegraph_common.js
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-02-21 20:08:25.000000 memray-1.7.0/src/memray/reporters/assets/table.js
--rw-r--r--   0 runner    (1001) docker     (123)     6820 2023-02-21 20:08:25.000000 memray-1.7.0/src/memray/reporters/flamegraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-02-21 20:08:25.000000 memray-1.7.0/src/memray/reporters/frame_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     5161 2023-02-21 20:08:25.000000 memray-1.7.0/src/memray/reporters/stats.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-02-21 20:08:25.000000 memray-1.7.0/src/memray/reporters/summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-02-21 20:08:25.000000 memray-1.7.0/src/memray/reporters/table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 20:08:39.083389 memray-1.7.0/src/memray/reporters/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-02-21 20:08:25.000000 memray-1.7.0/src/memray/reporters/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 20:08:39.083389 memray-1.7.0/src/memray/reporters/templates/assets/
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-02-21 20:08:25.000000 memray-1.7.0/src/memray/reporters/templates/assets/flamegraph.css
--rw-r--r--   0 runner    (1001) docker     (123)    78034 2023-02-21 20:08:25.000000 memray-1.7.0/src/memray/reporters/templates/assets/flamegraph.js
--rw-r--r--   0 runner    (1001) docker     (123)    73387 2023-02-21 20:08:25.000000 memray-1.7.0/src/memray/reporters/templates/assets/flamegraph_common.js
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-02-21 20:08:25.000000 memray-1.7.0/src/memray/reporters/templates/assets/table.css
--rw-r--r--   0 runner    (1001) docker     (123)    72877 2023-02-21 20:08:25.000000 memray-1.7.0/src/memray/reporters/templates/assets/table.js
--rw-r--r--   0 runner    (1001) docker     (123)     6259 2023-02-21 20:08:25.000000 memray-1.7.0/src/memray/reporters/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-02-21 20:08:25.000000 memray-1.7.0/src/memray/reporters/templates/classic_base.html
--rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-02-21 20:08:25.000000 memray-1.7.0/src/memray/reporters/templates/flamegraph.html
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-02-21 20:08:25.000000 memray-1.7.0/src/memray/reporters/templates/table.html
--rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-02-21 20:08:25.000000 memray-1.7.0/src/memray/reporters/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     5040 2023-02-21 20:08:25.000000 memray-1.7.0/src/memray/reporters/tree.py
--rw-r--r--   0 runner    (1001) docker     (123)    14218 2023-02-21 20:08:25.000000 memray-1.7.0/src/memray/reporters/tui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 20:08:39.067387 memray-1.7.0/src/memray.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16811 2023-02-21 20:08:39.000000 memray-1.7.0/src/memray.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6894 2023-02-21 20:08:39.000000 memray-1.7.0/src/memray.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-21 20:08:39.000000 memray-1.7.0/src/memray.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-02-21 20:08:39.000000 memray-1.7.0/src/memray.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-02-21 20:08:39.000000 memray-1.7.0/src/memray.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-02-21 20:08:39.000000 memray-1.7.0/src/memray.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 20:08:39.083389 memray-1.7.0/src/vendor/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 20:08:39.095390 memray-1.7.0/src/vendor/libbacktrace/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-02-21 20:08:25.000000 memray-1.7.0/src/vendor/libbacktrace/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)   567198 2023-02-21 20:08:25.000000 memray-1.7.0/src/vendor/libbacktrace/Isaac.Newton-Opticks.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-02-21 20:08:25.000000 memray-1.7.0/src/vendor/libbacktrace/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14971 2023-02-21 20:08:25.000000 memray-1.7.0/src/vendor/libbacktrace/Makefile.am
--rw-r--r--   0 runner    (1001) docker     (123)   123456 2023-02-21 20:08:25.000000 memray-1.7.0/src/vendor/libbacktrace/Makefile.in
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-02-21 20:08:25.000000 memray-1.7.0/src/vendor/libbacktrace/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    32034 2023-02-21 20:08:25.000000 memray-1.7.0/src/vendor/libbacktrace/aclocal.m4
--rw-r--r--   0 runner    (1001) docker     (123)     4445 2023-02-21 20:08:25.000000 memray-1.7.0/src/vendor/libbacktrace/alloc.c
--rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-02-21 20:08:25.000000 memray-1.7.0/src/vendor/libbacktrace/allocfail.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     3135 2023-02-21 20:08:25.000000 memray-1.7.0/src/vendor/libbacktrace/allocfail.sh
--rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-02-21 20:08:25.000000 memray-1.7.0/src/vendor/libbacktrace/atomic.c
--rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-02-21 20:08:25.000000 memray-1.7.0/src/vendor/libbacktrace/backtrace-supported.h.in
--rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-02-21 20:08:25.000000 memray-1.7.0/src/vendor/libbacktrace/backtrace.c
--rw-r--r--   0 runner    (1001) docker     (123)     8782 2023-02-21 20:08:25.000000 memray-1.7.0/src/vendor/libbacktrace/backtrace.h
--rw-r--r--   0 runner    (1001) docker     (123)    11352 2023-02-21 20:08:25.000000 memray-1.7.0/src/vendor/libbacktrace/btest.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     7382 2023-02-21 20:08:25.000000 memray-1.7.0/src/vendor/libbacktrace/compile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 20:08:39.095390 memray-1.7.0/src/vendor/libbacktrace/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-02-21 20:08:25.000000 memray-1.7.0/src/vendor/libbacktrace/config/enable.m4
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-02-21 20:08:25.000000 memray-1.7.0/src/vendor/libbacktrace/config/lead-dot.m4
--rw-r--r--   0 runner    (1001) docker     (123)   263960 2023-02-21 20:08:25.000000 memray-1.7.0/src/vendor/libbacktrace/config/libtool.m4
--rw-r--r--   0 runner    (1001) docker     (123)    11950 2023-02-21 20:08:25.000000 memray-1.7.0/src/vendor/libbacktrace/config/ltoptions.m4
--rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-02-21 20:08:25.000000 memray-1.7.0/src/vendor/libbacktrace/config/ltsugar.m4
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-02-21 20:08:25.000000 memray-1.7.0/src/vendor/libbacktrace/config/ltversion.m4
--rw-r--r--   0 runner    (1001) docker     (123)     6126 2023-02-21 20:08:25.000000 memray-1.7.0/src/vendor/libbacktrace/config/lt~obsolete.m4
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-02-21 20:08:25.000000 memray-1.7.0/src/vendor/libbacktrace/config/multi.m4
--rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-02-21 20:08:25.000000 memray-1.7.0/src/vendor/libbacktrace/config/override.m4
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-02-21 20:08:25.000000 memray-1.7.0/src/vendor/libbacktrace/config/unwind_ipinfo.m4
--rw-r--r--   0 runner    (1001) docker     (123)     8636 2023-02-21 20:08:25.000000 memray-1.7.0/src/vendor/libbacktrace/config/warnings.m4
--rwxr-xr-x   0 runner    (1001) docker     (123)    49446 2023-02-21 20:08:25.000000 memray-1.7.0/src/vendor/libbacktrace/config.guess
--rw-r--r--   0 runner    (1001) docker     (123)     4354 2023-02-21 20:08:25.000000 memray-1.7.0/src/vendor/libbacktrace/config.h.in
--rwxr-xr-x   0 runner    (1001) docker     (123)    35295 2023-02-21 20:08:25.000000 memray-1.7.0/src/vendor/libbacktrace/config.sub
--rwxr-xr-x   0 runner    (1001) docker     (123)   452188 2023-02-21 20:08:25.000000 memray-1.7.0/src/vendor/libbacktrace/configure
--rw-r--r--   0 runner    (1001) docker     (123)    18687 2023-02-21 20:08:25.000000 memray-1.7.0/src/vendor/libbacktrace/configure.ac
--rw-r--r--   0 runner    (1001) docker     (123)     4348 2023-02-21 20:08:25.000000 memray-1.7.0/src/vendor/libbacktrace/debuginfod_support.h
--rw-r--r--   0 runner    (1001) docker     (123)   116397 2023-02-21 20:08:25.000000 memray-1.7.0/src/vendor/libbacktrace/dwarf.c
--rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-02-21 20:08:25.000000 memray-1.7.0/src/vendor/libbacktrace/edtest.c
--rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-02-21 20:08:25.000000 memray-1.7.0/src/vendor/libbacktrace/edtest2.c
--rw-r--r--   0 runner    (1001) docker     (123)   133952 2023-02-21 20:08:25.000000 memray-1.7.0/src/vendor/libbacktrace/elf.c
--rw-r--r--   0 runner    (1001) docker     (123)     8853 2023-02-21 20:08:25.000000 memray-1.7.0/src/vendor/libbacktrace/fileline.c
--rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-02-21 20:08:25.000000 memray-1.7.0/src/vendor/libbacktrace/filenames.h
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-02-21 20:08:25.000000 memray-1.7.0/src/vendor/libbacktrace/filetype.awk
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-02-21 20:08:25.000000 memray-1.7.0/src/vendor/libbacktrace/install-debuginfo-for-buildid.sh.in
--rwxr-xr-x   0 runner    (1001) docker     (123)    14675 2023-02-21 20:08:25.000000 memray-1.7.0/src/vendor/libbacktrace/install-sh
--rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-02-21 20:08:25.000000 memray-1.7.0/src/vendor/libbacktrace/instrumented_alloc.c
--rw-r--r--   0 runner    (1001) docker     (123)    14317 2023-02-21 20:08:25.000000 memray-1.7.0/src/vendor/libbacktrace/internal.h
--rw-r--r--   0 runner    (1001) docker     (123)   263960 2023-02-21 20:08:25.000000 memray-1.7.0/src/vendor/libbacktrace/libtool.m4
--rw-r--r--   0 runner    (1001) docker     (123)   249764 2023-02-21 20:08:25.000000 memray-1.7.0/src/vendor/libbacktrace/ltmain.sh
--rw-r--r--   0 runner    (1001) docker     (123)    11950 2023-02-21 20:08:25.000000 memray-1.7.0/src/vendor/libbacktrace/ltoptions.m4
--rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-02-21 20:08:25.000000 memray-1.7.0/src/vendor/libbacktrace/ltsugar.m4
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-02-21 20:08:25.000000 memray-1.7.0/src/vendor/libbacktrace/ltversion.m4
--rw-r--r--   0 runner    (1001) docker     (123)     6126 2023-02-21 20:08:25.000000 memray-1.7.0/src/vendor/libbacktrace/lt~obsolete.m4
--rw-r--r--   0 runner    (1001) docker     (123)    36287 2023-02-21 20:08:25.000000 memray-1.7.0/src/vendor/libbacktrace/macho.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     6872 2023-02-21 20:08:25.000000 memray-1.7.0/src/vendor/libbacktrace/missing
--rw-r--r--   0 runner    (1001) docker     (123)     8584 2023-02-21 20:08:25.000000 memray-1.7.0/src/vendor/libbacktrace/mmap.c
--rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-02-21 20:08:25.000000 memray-1.7.0/src/vendor/libbacktrace/mmapio.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     2636 2023-02-21 20:08:25.000000 memray-1.7.0/src/vendor/libbacktrace/move-if-change
--rw-r--r--   0 runner    (1001) docker     (123)     9792 2023-02-21 20:08:25.000000 memray-1.7.0/src/vendor/libbacktrace/mtest.c
--rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-02-21 20:08:25.000000 memray-1.7.0/src/vendor/libbacktrace/nounwind.c
--rw-r--r--   0 runner    (1001) docker     (123)    23797 2023-02-21 20:08:25.000000 memray-1.7.0/src/vendor/libbacktrace/pecoff.c
--rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-02-21 20:08:25.000000 memray-1.7.0/src/vendor/libbacktrace/posix.c
--rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-02-21 20:08:25.000000 memray-1.7.0/src/vendor/libbacktrace/print.c
--rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-02-21 20:08:25.000000 memray-1.7.0/src/vendor/libbacktrace/read.c
--rw-r--r--   0 runner    (1001) docker     (123)     3213 2023-02-21 20:08:25.000000 memray-1.7.0/src/vendor/libbacktrace/simple.c
--rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-02-21 20:08:25.000000 memray-1.7.0/src/vendor/libbacktrace/sort.c
--rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-02-21 20:08:25.000000 memray-1.7.0/src/vendor/libbacktrace/state.c
--rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-02-21 20:08:25.000000 memray-1.7.0/src/vendor/libbacktrace/stest.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     4641 2023-02-21 20:08:25.000000 memray-1.7.0/src/vendor/libbacktrace/test-driver
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-02-21 20:08:25.000000 memray-1.7.0/src/vendor/libbacktrace/test_format.c
--rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-02-21 20:08:25.000000 memray-1.7.0/src/vendor/libbacktrace/testlib.c
--rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-02-21 20:08:25.000000 memray-1.7.0/src/vendor/libbacktrace/testlib.h
--rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-02-21 20:08:25.000000 memray-1.7.0/src/vendor/libbacktrace/ttest.c
--rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-02-21 20:08:25.000000 memray-1.7.0/src/vendor/libbacktrace/unittest.c
--rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-02-21 20:08:25.000000 memray-1.7.0/src/vendor/libbacktrace/unknown.c
--rw-r--r--   0 runner    (1001) docker     (123)    41385 2023-02-21 20:08:25.000000 memray-1.7.0/src/vendor/libbacktrace/xcoff.c
--rw-r--r--   0 runner    (1001) docker     (123)    11929 2023-02-21 20:08:25.000000 memray-1.7.0/src/vendor/libbacktrace/xztest.c
--rw-r--r--   0 runner    (1001) docker     (123)    15022 2023-02-21 20:08:25.000000 memray-1.7.0/src/vendor/libbacktrace/ztest.c
--rw-r--r--   0 runner    (1001) docker     (123)    11621 2023-02-21 20:08:25.000000 memray-1.7.0/src/vendor/libbacktrace_2446c66076480ce07a6bd868badcbceb3eeecc2e_debuginfod_patch.diff
--rw-r--r--   0 runner    (1001) docker     (123)     8114 2023-02-21 20:08:25.000000 memray-1.7.0/src/vendor/libbacktrace_2446c66076480ce07a6bd868badcbceb3eeecc2e_patch.diff
--rwxr-xr-x   0 runner    (1001) docker     (123)      716 2023-02-21 20:08:25.000000 memray-1.7.0/src/vendor/regenerate_libbacktrace.sh
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-02-21 20:08:25.000000 memray-1.7.0/webpack.config.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:55:08.129441 memray-1.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-09 19:54:56.000000 memray-1.8.0/.babelrc
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-09 19:54:56.000000 memray-1.8.0/.bumpversion.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-06-09 19:54:56.000000 memray-1.8.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-06-09 19:54:56.000000 memray-1.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-06-09 19:54:56.000000 memray-1.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6436 2023-06-09 19:54:56.000000 memray-1.8.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    13450 2023-06-09 19:54:56.000000 memray-1.8.0/NEWS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    17115 2023-06-09 19:55:08.125440 memray-1.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16199 2023-06-09 19:54:56.000000 memray-1.8.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)   531280 2023-06-09 19:54:56.000000 memray-1.8.0/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-09 19:54:56.000000 memray-1.8.0/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-06-09 19:54:56.000000 memray-1.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 19:55:08.129441 memray-1.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    10117 2023-06-09 19:54:56.000000 memray-1.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:55:08.097440 memray-1.8.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:55:08.101440 memray-1.8.0/src/memray/
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-06-09 19:54:56.000000 memray-1.8.0/src/memray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-09 19:54:56.000000 memray-1.8.0/src/memray/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-09 19:54:56.000000 memray-1.8.0/src/memray/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-06-09 19:54:56.000000 memray-1.8.0/src/memray/_destination.py
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-09 19:54:56.000000 memray-1.8.0/src/memray/_errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:55:08.105440 memray-1.8.0/src/memray/_ipython/
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-09 19:54:56.000000 memray-1.8.0/src/memray/_ipython/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5671 2023-06-09 19:54:56.000000 memray-1.8.0/src/memray/_ipython/flamegraph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:55:08.109440 memray-1.8.0/src/memray/_memray/
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-06-09 19:54:56.000000 memray-1.8.0/src/memray/_memray/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 19:54:56.000000 memray-1.8.0/src/memray/_memray/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-09 19:54:56.000000 memray-1.8.0/src/memray/_memray/algorithm.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-06-09 19:54:56.000000 memray-1.8.0/src/memray/_memray/alloc.h
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-06-09 19:54:56.000000 memray-1.8.0/src/memray/_memray/alloc.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-06-09 19:54:56.000000 memray-1.8.0/src/memray/_memray/compat.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-06-09 19:54:56.000000 memray-1.8.0/src/memray/_memray/compat.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7114 2023-06-09 19:54:56.000000 memray-1.8.0/src/memray/_memray/elf_shenanigans.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9629 2023-06-09 19:54:56.000000 memray-1.8.0/src/memray/_memray/elf_utils.h
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-09 19:54:56.000000 memray-1.8.0/src/memray/_memray/exceptions.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-06-09 19:54:56.000000 memray-1.8.0/src/memray/_memray/frame_tree.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9397 2023-06-09 19:54:56.000000 memray-1.8.0/src/memray/_memray/hooks.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6052 2023-06-09 19:54:56.000000 memray-1.8.0/src/memray/_memray/hooks.h
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-09 19:54:56.000000 memray-1.8.0/src/memray/_memray/hooks.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     5613 2023-06-09 19:54:56.000000 memray-1.8.0/src/memray/_memray/inject.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-09 19:54:56.000000 memray-1.8.0/src/memray/_memray/linker_shenanigans.h
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-06-09 19:54:56.000000 memray-1.8.0/src/memray/_memray/logging.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-06-09 19:54:56.000000 memray-1.8.0/src/memray/_memray/logging.h
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-09 19:54:56.000000 memray-1.8.0/src/memray/_memray/logging.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     9616 2023-06-09 19:54:56.000000 memray-1.8.0/src/memray/_memray/lz4_stream.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5590 2023-06-09 19:54:56.000000 memray-1.8.0/src/memray/_memray/macho_shenanigans.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-06-09 19:54:56.000000 memray-1.8.0/src/memray/_memray/macho_utils.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15624 2023-06-09 19:54:56.000000 memray-1.8.0/src/memray/_memray/native_resolver.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-06-09 19:54:56.000000 memray-1.8.0/src/memray/_memray/native_resolver.h
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-09 19:54:56.000000 memray-1.8.0/src/memray/_memray/native_resolver.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-09 19:54:56.000000 memray-1.8.0/src/memray/_memray/pthread.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-09 19:54:56.000000 memray-1.8.0/src/memray/_memray/python_helpers.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-09 19:54:56.000000 memray-1.8.0/src/memray/_memray/python_helpers.h
+-rw-r--r--   0 runner    (1001) docker     (123)    42922 2023-06-09 19:54:56.000000 memray-1.8.0/src/memray/_memray/record_reader.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6855 2023-06-09 19:54:56.000000 memray-1.8.0/src/memray/_memray/record_reader.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-06-09 19:54:56.000000 memray-1.8.0/src/memray/_memray/record_reader.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    20486 2023-06-09 19:54:56.000000 memray-1.8.0/src/memray/_memray/record_writer.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-06-09 19:54:56.000000 memray-1.8.0/src/memray/_memray/record_writer.h
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-09 19:54:56.000000 memray-1.8.0/src/memray/_memray/record_writer.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-06-09 19:54:56.000000 memray-1.8.0/src/memray/_memray/records.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8453 2023-06-09 19:54:56.000000 memray-1.8.0/src/memray/_memray/records.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-06-09 19:54:56.000000 memray-1.8.0/src/memray/_memray/records.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    10139 2023-06-09 19:54:56.000000 memray-1.8.0/src/memray/_memray/sink.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-06-09 19:54:56.000000 memray-1.8.0/src/memray/_memray/sink.h
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-09 19:54:56.000000 memray-1.8.0/src/memray/_memray/sink.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    34658 2023-06-09 19:54:56.000000 memray-1.8.0/src/memray/_memray/snapshot.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    17962 2023-06-09 19:54:56.000000 memray-1.8.0/src/memray/_memray/snapshot.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-06-09 19:54:56.000000 memray-1.8.0/src/memray/_memray/snapshot.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-06-09 19:54:56.000000 memray-1.8.0/src/memray/_memray/socket_reader_thread.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-09 19:54:56.000000 memray-1.8.0/src/memray/_memray/socket_reader_thread.h
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-09 19:54:56.000000 memray-1.8.0/src/memray/_memray/socket_reader_thread.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     7433 2023-06-09 19:54:56.000000 memray-1.8.0/src/memray/_memray/source.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-06-09 19:54:56.000000 memray-1.8.0/src/memray/_memray/source.h
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-09 19:54:56.000000 memray-1.8.0/src/memray/_memray/source.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    36606 2023-06-09 19:54:56.000000 memray-1.8.0/src/memray/_memray/tracking_api.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11255 2023-06-09 19:54:56.000000 memray-1.8.0/src/memray/_memray/tracking_api.h
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-06-09 19:54:56.000000 memray-1.8.0/src/memray/_memray/tracking_api.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     8111 2023-06-09 19:54:56.000000 memray-1.8.0/src/memray/_memray.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    54621 2023-06-09 19:54:56.000000 memray-1.8.0/src/memray/_memray.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     8574 2023-06-09 19:54:56.000000 memray-1.8.0/src/memray/_memray_test_utils.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-09 19:54:56.000000 memray-1.8.0/src/memray/_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-09 19:54:56.000000 memray-1.8.0/src/memray/_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-06-09 19:54:56.000000 memray-1.8.0/src/memray/_stats.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-06-09 19:54:56.000000 memray-1.8.0/src/memray/_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-06-09 19:54:56.000000 memray-1.8.0/src/memray/_test_utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-09 19:54:56.000000 memray-1.8.0/src/memray/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:55:08.109440 memray-1.8.0/src/memray/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-06-09 19:54:56.000000 memray-1.8.0/src/memray/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-06-09 19:54:56.000000 memray-1.8.0/src/memray/commands/_attach.gdb
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-06-09 19:54:56.000000 memray-1.8.0/src/memray/commands/_attach.lldb
+-rw-r--r--   0 runner    (1001) docker     (123)    12367 2023-06-09 19:54:56.000000 memray-1.8.0/src/memray/commands/attach.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10158 2023-06-09 19:54:56.000000 memray-1.8.0/src/memray/commands/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-06-09 19:54:56.000000 memray-1.8.0/src/memray/commands/flamegraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-06-09 19:54:56.000000 memray-1.8.0/src/memray/commands/live.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-06-09 19:54:56.000000 memray-1.8.0/src/memray/commands/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11086 2023-06-09 19:54:56.000000 memray-1.8.0/src/memray/commands/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-06-09 19:54:56.000000 memray-1.8.0/src/memray/commands/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-06-09 19:54:56.000000 memray-1.8.0/src/memray/commands/summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-09 19:54:56.000000 memray-1.8.0/src/memray/commands/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-06-09 19:54:56.000000 memray-1.8.0/src/memray/commands/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-06-09 19:54:56.000000 memray-1.8.0/src/memray/commands/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 19:54:56.000000 memray-1.8.0/src/memray/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:55:08.113440 memray-1.8.0/src/memray/reporters/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-09 19:54:56.000000 memray-1.8.0/src/memray/reporters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:55:08.113440 memray-1.8.0/src/memray/reporters/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 19:54:56.000000 memray-1.8.0/src/memray/reporters/assets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5569 2023-06-09 19:54:56.000000 memray-1.8.0/src/memray/reporters/assets/common.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-09 19:54:56.000000 memray-1.8.0/src/memray/reporters/assets/common.test.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-06-09 19:54:56.000000 memray-1.8.0/src/memray/reporters/assets/flamegraph.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-06-09 19:54:56.000000 memray-1.8.0/src/memray/reporters/assets/flamegraph_common.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-06-09 19:54:56.000000 memray-1.8.0/src/memray/reporters/assets/table.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9633 2023-06-09 19:54:56.000000 memray-1.8.0/src/memray/reporters/assets/temporal_flamegraph.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8655 2023-06-09 19:54:56.000000 memray-1.8.0/src/memray/reporters/flamegraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-06-09 19:54:56.000000 memray-1.8.0/src/memray/reporters/frame_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7707 2023-06-09 19:54:56.000000 memray-1.8.0/src/memray/reporters/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-09 19:54:56.000000 memray-1.8.0/src/memray/reporters/summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-06-09 19:54:56.000000 memray-1.8.0/src/memray/reporters/table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:55:08.113440 memray-1.8.0/src/memray/reporters/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-06-09 19:54:56.000000 memray-1.8.0/src/memray/reporters/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:55:08.113440 memray-1.8.0/src/memray/reporters/templates/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-06-09 19:54:56.000000 memray-1.8.0/src/memray/reporters/templates/assets/flamegraph.css
+-rw-r--r--   0 runner    (1001) docker     (123)    78034 2023-06-09 19:54:56.000000 memray-1.8.0/src/memray/reporters/templates/assets/flamegraph.js
+-rw-r--r--   0 runner    (1001) docker     (123)    73387 2023-06-09 19:54:56.000000 memray-1.8.0/src/memray/reporters/templates/assets/flamegraph_common.js
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-09 19:54:56.000000 memray-1.8.0/src/memray/reporters/templates/assets/table.css
+-rw-r--r--   0 runner    (1001) docker     (123)    72877 2023-06-09 19:54:56.000000 memray-1.8.0/src/memray/reporters/templates/assets/table.js
+-rw-r--r--   0 runner    (1001) docker     (123)    80852 2023-06-09 19:54:56.000000 memray-1.8.0/src/memray/reporters/templates/assets/temporal_flamegraph.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6259 2023-06-09 19:54:56.000000 memray-1.8.0/src/memray/reporters/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-09 19:54:56.000000 memray-1.8.0/src/memray/reporters/templates/classic_base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3805 2023-06-09 19:54:56.000000 memray-1.8.0/src/memray/reporters/templates/flamegraph.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-06-09 19:54:56.000000 memray-1.8.0/src/memray/reporters/templates/table.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-06-09 19:54:56.000000 memray-1.8.0/src/memray/reporters/templates/temporal_flamegraph.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-06-09 19:54:56.000000 memray-1.8.0/src/memray/reporters/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5040 2023-06-09 19:54:56.000000 memray-1.8.0/src/memray/reporters/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14218 2023-06-09 19:54:56.000000 memray-1.8.0/src/memray/reporters/tui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:55:08.105440 memray-1.8.0/src/memray.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17115 2023-06-09 19:55:08.000000 memray-1.8.0/src/memray.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7076 2023-06-09 19:55:08.000000 memray-1.8.0/src/memray.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 19:55:08.000000 memray-1.8.0/src/memray.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-09 19:55:08.000000 memray-1.8.0/src/memray.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-06-09 19:55:08.000000 memray-1.8.0/src/memray.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-09 19:55:08.000000 memray-1.8.0/src/memray.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:55:08.113440 memray-1.8.0/src/vendor/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:55:08.125440 memray-1.8.0/src/vendor/libbacktrace/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-09 19:54:56.000000 memray-1.8.0/src/vendor/libbacktrace/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)   567198 2023-06-09 19:54:56.000000 memray-1.8.0/src/vendor/libbacktrace/Isaac.Newton-Opticks.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-06-09 19:54:56.000000 memray-1.8.0/src/vendor/libbacktrace/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14971 2023-06-09 19:54:56.000000 memray-1.8.0/src/vendor/libbacktrace/Makefile.am
+-rw-r--r--   0 runner    (1001) docker     (123)   123456 2023-06-09 19:54:56.000000 memray-1.8.0/src/vendor/libbacktrace/Makefile.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-06-09 19:54:56.000000 memray-1.8.0/src/vendor/libbacktrace/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    32034 2023-06-09 19:54:56.000000 memray-1.8.0/src/vendor/libbacktrace/aclocal.m4
+-rw-r--r--   0 runner    (1001) docker     (123)     4445 2023-06-09 19:54:56.000000 memray-1.8.0/src/vendor/libbacktrace/alloc.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-06-09 19:54:56.000000 memray-1.8.0/src/vendor/libbacktrace/allocfail.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3135 2023-06-09 19:54:56.000000 memray-1.8.0/src/vendor/libbacktrace/allocfail.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-06-09 19:54:56.000000 memray-1.8.0/src/vendor/libbacktrace/atomic.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-06-09 19:54:56.000000 memray-1.8.0/src/vendor/libbacktrace/backtrace-supported.h.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-06-09 19:54:56.000000 memray-1.8.0/src/vendor/libbacktrace/backtrace.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8782 2023-06-09 19:54:56.000000 memray-1.8.0/src/vendor/libbacktrace/backtrace.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11352 2023-06-09 19:54:56.000000 memray-1.8.0/src/vendor/libbacktrace/btest.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7382 2023-06-09 19:54:56.000000 memray-1.8.0/src/vendor/libbacktrace/compile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:55:08.125440 memray-1.8.0/src/vendor/libbacktrace/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-06-09 19:54:56.000000 memray-1.8.0/src/vendor/libbacktrace/config/enable.m4
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-06-09 19:54:56.000000 memray-1.8.0/src/vendor/libbacktrace/config/lead-dot.m4
+-rw-r--r--   0 runner    (1001) docker     (123)   263960 2023-06-09 19:54:56.000000 memray-1.8.0/src/vendor/libbacktrace/config/libtool.m4
+-rw-r--r--   0 runner    (1001) docker     (123)    11950 2023-06-09 19:54:56.000000 memray-1.8.0/src/vendor/libbacktrace/config/ltoptions.m4
+-rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-06-09 19:54:56.000000 memray-1.8.0/src/vendor/libbacktrace/config/ltsugar.m4
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-09 19:54:56.000000 memray-1.8.0/src/vendor/libbacktrace/config/ltversion.m4
+-rw-r--r--   0 runner    (1001) docker     (123)     6126 2023-06-09 19:54:56.000000 memray-1.8.0/src/vendor/libbacktrace/config/lt~obsolete.m4
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-06-09 19:54:56.000000 memray-1.8.0/src/vendor/libbacktrace/config/multi.m4
+-rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-06-09 19:54:56.000000 memray-1.8.0/src/vendor/libbacktrace/config/override.m4
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-06-09 19:54:56.000000 memray-1.8.0/src/vendor/libbacktrace/config/unwind_ipinfo.m4
+-rw-r--r--   0 runner    (1001) docker     (123)     8636 2023-06-09 19:54:56.000000 memray-1.8.0/src/vendor/libbacktrace/config/warnings.m4
+-rwxr-xr-x   0 runner    (1001) docker     (123)    49446 2023-06-09 19:54:56.000000 memray-1.8.0/src/vendor/libbacktrace/config.guess
+-rw-r--r--   0 runner    (1001) docker     (123)     4354 2023-06-09 19:54:56.000000 memray-1.8.0/src/vendor/libbacktrace/config.h.in
+-rwxr-xr-x   0 runner    (1001) docker     (123)    35295 2023-06-09 19:54:56.000000 memray-1.8.0/src/vendor/libbacktrace/config.sub
+-rwxr-xr-x   0 runner    (1001) docker     (123)   452188 2023-06-09 19:54:56.000000 memray-1.8.0/src/vendor/libbacktrace/configure
+-rw-r--r--   0 runner    (1001) docker     (123)    18687 2023-06-09 19:54:56.000000 memray-1.8.0/src/vendor/libbacktrace/configure.ac
+-rw-r--r--   0 runner    (1001) docker     (123)     4348 2023-06-09 19:54:56.000000 memray-1.8.0/src/vendor/libbacktrace/debuginfod_support.h
+-rw-r--r--   0 runner    (1001) docker     (123)   116397 2023-06-09 19:54:56.000000 memray-1.8.0/src/vendor/libbacktrace/dwarf.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-06-09 19:54:56.000000 memray-1.8.0/src/vendor/libbacktrace/edtest.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-06-09 19:54:56.000000 memray-1.8.0/src/vendor/libbacktrace/edtest2.c
+-rw-r--r--   0 runner    (1001) docker     (123)   133952 2023-06-09 19:54:56.000000 memray-1.8.0/src/vendor/libbacktrace/elf.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8853 2023-06-09 19:54:56.000000 memray-1.8.0/src/vendor/libbacktrace/fileline.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-06-09 19:54:56.000000 memray-1.8.0/src/vendor/libbacktrace/filenames.h
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-06-09 19:54:56.000000 memray-1.8.0/src/vendor/libbacktrace/filetype.awk
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-06-09 19:54:56.000000 memray-1.8.0/src/vendor/libbacktrace/install-debuginfo-for-buildid.sh.in
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14675 2023-06-09 19:54:56.000000 memray-1.8.0/src/vendor/libbacktrace/install-sh
+-rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-06-09 19:54:56.000000 memray-1.8.0/src/vendor/libbacktrace/instrumented_alloc.c
+-rw-r--r--   0 runner    (1001) docker     (123)    14317 2023-06-09 19:54:56.000000 memray-1.8.0/src/vendor/libbacktrace/internal.h
+-rw-r--r--   0 runner    (1001) docker     (123)   263960 2023-06-09 19:54:56.000000 memray-1.8.0/src/vendor/libbacktrace/libtool.m4
+-rw-r--r--   0 runner    (1001) docker     (123)   249764 2023-06-09 19:54:56.000000 memray-1.8.0/src/vendor/libbacktrace/ltmain.sh
+-rw-r--r--   0 runner    (1001) docker     (123)    11950 2023-06-09 19:54:56.000000 memray-1.8.0/src/vendor/libbacktrace/ltoptions.m4
+-rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-06-09 19:54:56.000000 memray-1.8.0/src/vendor/libbacktrace/ltsugar.m4
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-09 19:54:56.000000 memray-1.8.0/src/vendor/libbacktrace/ltversion.m4
+-rw-r--r--   0 runner    (1001) docker     (123)     6126 2023-06-09 19:54:56.000000 memray-1.8.0/src/vendor/libbacktrace/lt~obsolete.m4
+-rw-r--r--   0 runner    (1001) docker     (123)    36287 2023-06-09 19:54:56.000000 memray-1.8.0/src/vendor/libbacktrace/macho.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6872 2023-06-09 19:54:56.000000 memray-1.8.0/src/vendor/libbacktrace/missing
+-rw-r--r--   0 runner    (1001) docker     (123)     8584 2023-06-09 19:54:56.000000 memray-1.8.0/src/vendor/libbacktrace/mmap.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-06-09 19:54:56.000000 memray-1.8.0/src/vendor/libbacktrace/mmapio.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2636 2023-06-09 19:54:56.000000 memray-1.8.0/src/vendor/libbacktrace/move-if-change
+-rw-r--r--   0 runner    (1001) docker     (123)     9792 2023-06-09 19:54:56.000000 memray-1.8.0/src/vendor/libbacktrace/mtest.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-06-09 19:54:56.000000 memray-1.8.0/src/vendor/libbacktrace/nounwind.c
+-rw-r--r--   0 runner    (1001) docker     (123)    23797 2023-06-09 19:54:56.000000 memray-1.8.0/src/vendor/libbacktrace/pecoff.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-06-09 19:54:56.000000 memray-1.8.0/src/vendor/libbacktrace/posix.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-06-09 19:54:56.000000 memray-1.8.0/src/vendor/libbacktrace/print.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-06-09 19:54:56.000000 memray-1.8.0/src/vendor/libbacktrace/read.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3213 2023-06-09 19:54:56.000000 memray-1.8.0/src/vendor/libbacktrace/simple.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-06-09 19:54:56.000000 memray-1.8.0/src/vendor/libbacktrace/sort.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-06-09 19:54:56.000000 memray-1.8.0/src/vendor/libbacktrace/state.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-06-09 19:54:56.000000 memray-1.8.0/src/vendor/libbacktrace/stest.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4641 2023-06-09 19:54:56.000000 memray-1.8.0/src/vendor/libbacktrace/test-driver
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-06-09 19:54:56.000000 memray-1.8.0/src/vendor/libbacktrace/test_format.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-06-09 19:54:56.000000 memray-1.8.0/src/vendor/libbacktrace/testlib.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-06-09 19:54:56.000000 memray-1.8.0/src/vendor/libbacktrace/testlib.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-06-09 19:54:56.000000 memray-1.8.0/src/vendor/libbacktrace/ttest.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-06-09 19:54:56.000000 memray-1.8.0/src/vendor/libbacktrace/unittest.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-06-09 19:54:56.000000 memray-1.8.0/src/vendor/libbacktrace/unknown.c
+-rw-r--r--   0 runner    (1001) docker     (123)    41385 2023-06-09 19:54:56.000000 memray-1.8.0/src/vendor/libbacktrace/xcoff.c
+-rw-r--r--   0 runner    (1001) docker     (123)    11929 2023-06-09 19:54:56.000000 memray-1.8.0/src/vendor/libbacktrace/xztest.c
+-rw-r--r--   0 runner    (1001) docker     (123)    15022 2023-06-09 19:54:56.000000 memray-1.8.0/src/vendor/libbacktrace/ztest.c
+-rw-r--r--   0 runner    (1001) docker     (123)    11621 2023-06-09 19:54:56.000000 memray-1.8.0/src/vendor/libbacktrace_2446c66076480ce07a6bd868badcbceb3eeecc2e_debuginfod_patch.diff
+-rw-r--r--   0 runner    (1001) docker     (123)     8114 2023-06-09 19:54:56.000000 memray-1.8.0/src/vendor/libbacktrace_2446c66076480ce07a6bd868badcbceb3eeecc2e_patch.diff
+-rwxr-xr-x   0 runner    (1001) docker     (123)      716 2023-06-09 19:54:56.000000 memray-1.8.0/src/vendor/regenerate_libbacktrace.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-09 19:54:56.000000 memray-1.8.0/webpack.config.js
```

### Comparing `memray-1.7.0/LICENSE` & `memray-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/MANIFEST.in` & `memray-1.8.0/MANIFEST.in`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 exclude .clang-format
 exclude asv.conf.json
 exclude CONTRIBUTING.md
 exclude Dockerfile
 exclude Jenkinsfile
 exclude requirements-*.txt
-exclude tox.ini
 exclude .medusarc
 exclude valgrind.supp
 
 recursive-exclude src/vendor/libbacktrace/install *
 recursive-exclude benchmarks *
 recursive-exclude debian *
 recursive-exclude docker *
@@ -26,14 +25,15 @@
 include package-lock.json
 include .bumpversion.cfg
 include .babelrc
 include webpack.config.js
 include NEWS.rst
 include .flake8
 include src/memray/py.typed
+include .pre-commit-config.yaml
 
 recursive-include src/vendor *
 recursive-include src/memray *.py
 recursive-include src/memray *.pyi
 recursive-include src/memray *.html *.js *.css
 recursive-include src/memray *.pyx *.pxd
 recursive-include src/memray *.gdb *.lldb
```

### Comparing `memray-1.7.0/Makefile` & `memray-1.8.0/Makefile`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,25 @@
 PYTHON ?= python
 NPM ?= npm
 CLANG_FORMAT ?= clang-format
-PRETTIER ?= prettier --no-editorconfig
 
 # Doc generation variables
 UPSTREAM_GIT_REMOTE ?= origin
 DOCSBUILDDIR := docs/_build
 HTMLDIR := $(DOCSBUILDDIR)/html
-PKG_CONFIG_PATH ?= /opt/bb/lib64/pkgconfig
-PIP_INSTALL=PKG_CONFIG_PATH="$(PKG_CONFIG_PATH)" $(PYTHON) -m pip install
+PIP_INSTALL=$(PYTHON) -m pip install
 
 reporters_path := ./src/memray/reporters
 js_files := $(wildcard $(reporters_path)/assets/*.js)
 generated_js_files := \
     $(reporters_path)/templates/assets/flamegraph_common.js \
     $(reporters_path)/templates/assets/flamegraph.js \
+    $(reporters_path)/templates/assets/temporal_flamegraph.js \
     $(reporters_path)/templates/assets/table.js
-css_files := 'src/**/*.css'
-markdown_files := $(shell find . -name \*.md -not -path '*/\.*' -not -path './src/vendor/*')
 cpp_files := $(shell find src/memray/_memray -name \*.cpp -o -name \*.h)
-python_files := $(shell find . -name \*.py -not -path '*/\.*' -not -path './benchmarks/benchmarking/cases/*')
-cython_files := $(shell find src -name \*.pyx -or -name \*.pxd -not -path '*/\.*')
-type_files := $(shell find src -name \*.pyi -not -path '*/\.*')
 
 # Use this to inject arbitrary commands before the make targets (e.g. docker)
 ENV :=
 
 .PHONY: build
 build: build-js build-ext  ## (default) Build package extensions and assets in-place
 
@@ -62,28 +56,29 @@
 
 .PHONY: check-python  ## Run the Python tests
 check-python:
 	$(PYTHON) -m pytest -vvv --log-cli-level=info -s --color=yes $(PYTEST_ARGS) tests
 
 .PHONY: check-js  ## Run the Javascript tests
 check-js:
+	$(NPM) install jest --save-dev
 	$(NPM) run-script test
 
 .PHONY: pycoverage
 pycoverage:  ## Run the test suite, with Python code coverage
 	$(PYTHON) -m pytest \
 		-vvv \
 		--log-cli-level=info \
 		-s \
 		--color=yes \
 		--cov=memray \
 		--cov=tests \
-		--cov-config=tox.ini \
+		--cov-config=pyproject.toml \
 		--cov-report=term \
-		--cov-fail-under=80 \
+		--cov-fail-under=90 \
 		--cov-append $(PYTEST_ARGS) \
 		tests
 
 .PHONY: valgrind
 valgrind:  ## Run valgrind, with the correct configuration
 	PYTHONMALLOC=malloc valgrind \
 		--suppressions=./valgrind.supp \
@@ -104,90 +99,64 @@
 
 .PHONY: ccoverage
 ccoverage:  ## Run the test suite, with C++ code coverage
 	$(MAKE) clean
 	CFLAGS="$(CFLAGS) -O0 -pg --coverage" $(MAKE) build
 	$(MAKE) check
 	gcov -i build/*/src/memray/_memray -i -d
-	lcov --capture --directory .  --output-file memray.info
-	lcov --extract memray.info '*/src/memray/*' --output-file memray.info
-	genhtml memray.info --output-directory memray-coverage
+	lcov --capture --directory .  --output-file cppcoverage.lcov
+	lcov --extract cppcoverage.lcov '*/src/memray/_memray/*' --output-file cppcoverage.lcov
+	genhtml *coverage.lcov --branch-coverage --output-directory memray-coverage
 	find . | grep -E '(\.gcda|\.gcno|\.gcov\.json\.gz)' | xargs rm -rf
 
-.PHONY: format-python
-format-python:  ## Autoformat Python files
-	$(PYTHON) -m isort $(python_files) $(cython_files) $(type_files)
-	$(PYTHON) -m black $(python_files)
-	$(PYTHON) -m black $(type_files)
-
-.PHONY: format-markdown
-format-markdown:  ## Autoformat markdown files
-	$(PRETTIER) --write $(markdown_files)
-
-.PHONY: format-assets
-format-assets:  ## Autoformat CSS and JS files
-	$(PRETTIER) --write $(js_files) $(css_files)
-
 .PHONY: format
-format: format-python format-markdown format-assets  ## Autoformat all files
-	$(CLANG_FORMAT) -i $(cpp_files)
+format:  ## Autoformat all files
+	$(PYTHON) -m pre_commit run --all-files
 
-.PHONY: lint-python
-lint-python:  ## Lint Python files
-	$(PYTHON) -m isort --check $(python_files) $(cython_files) $(type_files)
-	$(PYTHON) -m flake8 $(python_files)
-	$(PYTHON) -m black --check $(python_files)
-	$(PYTHON) -m black --check $(type_files)
+.PHONY: lint
+lint:  ## Lint all files
+	$(PYTHON) -m pre_commit run --all-files
 	$(PYTHON) -m mypy -p memray --strict --ignore-missing-imports
 	$(PYTHON) -m mypy tests --ignore-missing-imports
 
-.PHONY: lint-markdown
-lint-markdown:  ## Lint markdown files
-	$(PRETTIER) --check $(markdown_files)
-
-.PHONY: lint-assets
-lint-assets:  ## Lint CSS and JS files
-	$(PRETTIER) --check $(js_files) $(css_files)
-
-.PHONY: lint
-lint: lint-python lint-markdown lint-assets  ## Lint all files
-	$(CLANG_FORMAT) --Werror --dry-run $(cpp_files)
-	$(PYTHON) -m check_manifest
-
 .PHONY: docs
 docs:  ## Generate documentation
 	$(MAKE) -C docs clean
 	$(MAKE) -C docs html
 
 .PHONY: docs-live
 docs-live:  ## Serve documentation on localhost:8000, with live-reload
 	$(MAKE) -C docs clean
 	$(MAKE) -C docs livehtml
 
 .PHONY: gh-pages
-gh-pages:  ## Publish documentation on BBGitHub Pages
+gh-pages:  ## Publish documentation on GitHub Pages
 	$(eval GIT_REMOTE := $(shell git remote get-url $(UPSTREAM_GIT_REMOTE)))
 	$(eval COMMIT_HASH := $(shell git rev-parse HEAD))
 	touch $(HTMLDIR)/.nojekyll
 	@echo -n "Documentation ready, push to $(GIT_REMOTE)? [Y/n] " && read ans && [ $${ans:-Y} == Y ]
 	git init $(HTMLDIR)
 	GIT_DIR=$(HTMLDIR)/.git GIT_WORK_TREE=$(HTMLDIR) git add -A
 	GIT_DIR=$(HTMLDIR)/.git git commit -m "Documentation for commit $(COMMIT_HASH)"
 	GIT_DIR=$(HTMLDIR)/.git git push $(GIT_REMOTE) HEAD:gh-pages --force
 	rm -rf $(HTMLDIR)/.git
 
 
 .PHONY: clean
 clean:  ## Clean any built/generated artifacts
-	find . | grep -E '(\.o|\.so|\.gcda|\.gcno|\.gcov\.json\.gz)' | xargs rm -rf
+	find . | grep -E '(\.o|\.gcda|\.gcno|\.gcov\.json\.gz)' | xargs rm -rf
 	find . | grep -E '(__pycache__|\.pyc|\.pyo)' | xargs rm -rf
+	rm -rf build
+	rm -f src/memray/_test_utils.*.so
+	rm -f src/memray/_memray.*.so
+	rm -f src/memray/_inject.*.so
 	rm -f src/memray/_memray.cpp
-	rm -f memray.info
 	rm -rf memray-coverage
 	rm -rf node_modules
+	rm -f cppcoverage.lcov
 
 .PHONY: bump_version
 bump_version:
 	bump2version $(RELEASE)
 	$(eval NEW_VERSION := $(shell bump2version \
 	                                --allow-dirty \
 	                                --dry-run \
```

### Comparing `memray-1.7.0/NEWS.rst` & `memray-1.8.0/NEWS.rst`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,34 @@
     fix problems like typo corrections or such.
 
 Changelog
 =========
 
 .. towncrier release notes start
 
+memray 1.8.0 (2023-06-09)
+-------------------------
+
+Features
+~~~~~~~~
+
+- Allow ``memray stats`` to output a JSON report via ``--json`` flag. (#377)
+- We now publish x86-64 musllinux_1_1 wheels, compatible with Alpine Linux. (#379)
+- We now support :ref:`temporal flame graphs`, which provide an exciting new way of analyzing your process's memory usage over time. (#391)
+
+
+Bug Fixes
+~~~~~~~~~
+
+- Fix a bug where a non-import call on the same line as an ``import`` statement would be hidden by the "Hide Import System Frames" checkbox of a flame graph. (#329)
+- Fixed a bug that was hitting an assert when constructing hybrid stack frames in Python 3.11 when no eval symbols are available. (#334)
+- Change the font color used by the ``%%memray_flamegraph`` Jupyter magic's progress updates for better contrast on the JupyterLab dark theme. (#344)
+- Fix a bug that could result in a deadlock when tracking a process linked against an old version of musl libc. (#379)
+
+
 memray 1.7.0 (2023-02-21)
 -------------------------
 
 Features
 ~~~~~~~~
 
 - ``memray run`` now supports ``--aggregate`` to produce :ref:`aggregated capture files <aggregated capture files>`, which can be much smaller but aren't able to be used for generating every type of report. (#277)
```

### Comparing `memray-1.7.0/PKG-INFO` & `memray-1.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: memray
-Version: 1.7.0
+Version: 1.8.0
 Summary: A memory profiler for Python applications
 Home-page: https://github.com/bloomberg/memray
 Author: Pablo Galindo Salgado
 License: Apache 2.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
@@ -111,27 +111,41 @@
 ```shell
 export CFLAGS="-I$(brew --prefix lz4)/include" LDFLAGS="-L$(brew --prefix lz4)/lib -Wl,-rpath,$(brew --prefix lz4)/lib"
 ```
 
 before installing `memray`. Check the documentation of your package manager to know the location of the header and library
 files for more detailed information.
 
+If you are building on MacOS, you will also need to set the deployment target.
+
+```shell
+export MACOSX_DEPLOYMENT_TARGET=10.14
+```
+
 Once you have the binary dependencies installed, you can clone the repository and follow with the normal building process:
 
 ```shell
 git clone git@github.com:bloomberg/memray.git memray
 cd memray
 python3 -m venv ../memray-env/  # just an example, put this wherever you want
 source ../memray-env/bin/activate
 python3 -m pip install --upgrade pip
 python3 -m pip install -e . -r requirements-test.txt -r requirements-extra.txt
 ```
 
 This will install Memray in the virtual environment in development mode (the `-e` of the last `pip install` command).
 
+If you plan to contribute back, you should install the pre-commit hooks:
+
+```shell
+pre-commit install
+```
+
+This will ensure that your contribution passes our linting checks.
+
 # Documentation
 
 You can find the latest documentation available [here](https://bloomberg.github.io/memray/).
 
 # Usage
 
 There are many ways to use Memray. The easiest way is to use it as a command line tool to run your script, application, or library.
@@ -336,20 +350,20 @@
 
 We welcome your contributions to help us improve and extend this project!
 
 Below you will find some basic steps required to be able to contribute to the project. If you have any questions about this process or any other aspect of contributing to a Bloomberg open source project, feel free to send an email to opensource@bloomberg.net and we'll get your questions answered as quickly as we can.
 
 ## Contribution Licensing
 
-Since this project is distributed under the terms of an [open source license](LICENSE), contributions that you make
-are licensed under the same terms. In order for us to be able to accept your contributions,
+Since this project is distributed under the terms of an [open source license](LICENSE), contributions that
+you make are licensed under the same terms. In order for us to be able to accept your contributions,
 we will need explicit confirmation from you that you are able and willing to provide them under
 these terms, and the mechanism we use to do this is called a Developer's Certificate of Origin
-[(DCO)](https://github.com/bloomberg/.github/blob/main/DCO.md). This is very similar to the process used by the Linux(R) kernel, Samba, and many
-other major open source projects.
+[(DCO)](https://github.com/bloomberg/.github/blob/main/DCO.md). This is very similar to the process
+used by the Linux kernel, Samba, and many other major open source projects.
 
 To participate under these terms, all that you must do is include a line like the following as the
 last line of the commit message for each commit in your contribution:
 
     Signed-Off-By: Random J. Developer <random@developer.example.org>
 
 The simplest way to accomplish this is to add `-s` or `--signoff` to your `git commit` command.
```

### Comparing `memray-1.7.0/README.md` & `memray-1.8.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -85,27 +85,41 @@
 ```shell
 export CFLAGS="-I$(brew --prefix lz4)/include" LDFLAGS="-L$(brew --prefix lz4)/lib -Wl,-rpath,$(brew --prefix lz4)/lib"
 ```
 
 before installing `memray`. Check the documentation of your package manager to know the location of the header and library
 files for more detailed information.
 
+If you are building on MacOS, you will also need to set the deployment target.
+
+```shell
+export MACOSX_DEPLOYMENT_TARGET=10.14
+```
+
 Once you have the binary dependencies installed, you can clone the repository and follow with the normal building process:
 
 ```shell
 git clone git@github.com:bloomberg/memray.git memray
 cd memray
 python3 -m venv ../memray-env/  # just an example, put this wherever you want
 source ../memray-env/bin/activate
 python3 -m pip install --upgrade pip
 python3 -m pip install -e . -r requirements-test.txt -r requirements-extra.txt
 ```
 
 This will install Memray in the virtual environment in development mode (the `-e` of the last `pip install` command).
 
+If you plan to contribute back, you should install the pre-commit hooks:
+
+```shell
+pre-commit install
+```
+
+This will ensure that your contribution passes our linting checks.
+
 # Documentation
 
 You can find the latest documentation available [here](https://bloomberg.github.io/memray/).
 
 # Usage
 
 There are many ways to use Memray. The easiest way is to use it as a command line tool to run your script, application, or library.
@@ -310,20 +324,20 @@
 
 We welcome your contributions to help us improve and extend this project!
 
 Below you will find some basic steps required to be able to contribute to the project. If you have any questions about this process or any other aspect of contributing to a Bloomberg open source project, feel free to send an email to opensource@bloomberg.net and we'll get your questions answered as quickly as we can.
 
 ## Contribution Licensing
 
-Since this project is distributed under the terms of an [open source license](LICENSE), contributions that you make
-are licensed under the same terms. In order for us to be able to accept your contributions,
+Since this project is distributed under the terms of an [open source license](LICENSE), contributions that
+you make are licensed under the same terms. In order for us to be able to accept your contributions,
 we will need explicit confirmation from you that you are able and willing to provide them under
 these terms, and the mechanism we use to do this is called a Developer's Certificate of Origin
-[(DCO)](https://github.com/bloomberg/.github/blob/main/DCO.md). This is very similar to the process used by the Linux(R) kernel, Samba, and many
-other major open source projects.
+[(DCO)](https://github.com/bloomberg/.github/blob/main/DCO.md). This is very similar to the process
+used by the Linux kernel, Samba, and many other major open source projects.
 
 To participate under these terms, all that you must do is include a line like the following as the
 last line of the commit message for each commit in your contribution:
 
     Signed-Off-By: Random J. Developer <random@developer.example.org>
 
 The simplest way to accomplish this is to add `-s` or `--signoff` to your `git commit` command.
```

### Comparing `memray-1.7.0/package-lock.json` & `memray-1.8.0/package-lock.json`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/pyproject.toml` & `memray-1.8.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -4,14 +4,24 @@
      "setuptools",
      "wheel",
      "Cython"
 ]
 
 build-backend = 'setuptools.build_meta'
 
+[tool.ruff]
+line-length = 95
+select = ["F", "E", "W", "I001"]
+fix = true
+
+[tool.ruff.isort]
+force-single-line = true
+known-first-party = ["memray"]
+known-third-party=["rich", "elftools", "pytest"]
+
 [tool.isort]
 force_single_line = true
 multi_line_output = 3
 include_trailing_comma = true
 force_grid_wrap = 0
 use_parentheses = true
 line_length = 88
@@ -44,15 +54,15 @@
 ]
 
 [tool.mypy]
 exclude="tests/integration/(native_extension|multithreaded_extension)/"
 
 [tool.cibuildwheel]
 build = ["cp38-*", "cp39-*", "cp310-*", "cp311-*"]
-skip = "*musllinux*"
+skip = "*musllinux*i686*"
 manylinux-x86_64-image = "manylinux2014"
 manylinux-i686-image = "manylinux2014"
 
 [[tool.cibuildwheel.overrides]]
 select = "cp3{7,8,9,10}-*"
 manylinux-x86_64-image = "manylinux2010"
 manylinux-i686-image = "manylinux2010"
@@ -70,7 +80,33 @@
   "make",
   "make install"
 ]
 before-test = [
   "codesign --remove-signature /Library/Frameworks/Python.framework/Versions/*/bin/python3 || true",
   "codesign --remove-signature /Library/Frameworks/Python.framework/Versions/*/Resources/Python.app/Contents/MacOS/Python || true",
 ]
+
+[tool.coverage.run]
+plugins = [
+  "Cython.Coverage",
+]
+source = [
+  "src/memray",
+  "tests/",
+]
+branch = true
+parallel = true
+omit = [
+  "*__init__.py",
+]
+
+[tool.coverage.report]
+skip_covered = true
+show_missing = true
+
+
+# Override the default linux before-all for musl linux
+[[tool.cibuildwheel.overrides]]
+select = "*-musllinux*"
+before-all = [
+  "apk add --update libunwind-dev lz4-dev gdb lldb",
+]
```

### Comparing `memray-1.7.0/setup.py` & `memray-1.8.0/setup.py`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/memray/__init__.py` & `memray-1.8.0/src/memray/__init__.py`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/memray/__init__.pyi` & `memray-1.8.0/src/memray/__init__.pyi`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/memray/_destination.py` & `memray-1.8.0/src/memray/_destination.py`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/memray/_ipython/flamegraph.py` & `memray-1.8.0/src/memray/_ipython/flamegraph.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,13 +155,13 @@
             reporter.render(
                 outfile=f,
                 metadata=reader.metadata,
                 show_memory_leaks=options.show_memory_leaks,
                 merge_threads=merge_threads,
             )
         dump_file.unlink()
-        pprint(f"Results saved to [bold blue]{flamegraph_path}[/bold blue]")
+        pprint(f"Results saved to [bold cyan]{flamegraph_path}")
         display(IFrame(flamegraph_path, width="100%", height="600"))  # type: ignore
 
 
 assert FlamegraphMagics.memray_flamegraph.__doc__ is not None
 FlamegraphMagics.memray_flamegraph.__doc__ += "\n\n" + argument_parser().format_help()
```

### Comparing `memray-1.7.0/src/memray/_memray/CMakeLists.txt` & `memray-1.8.0/src/memray/_memray/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/memray/_memray/alloc.pxd` & `memray-1.8.0/src/memray/_memray/alloc.pxd`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/memray/_memray/compat.cpp` & `memray-1.8.0/src/memray/_memray/compat.cpp`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/memray/_memray/compat.h` & `memray-1.8.0/src/memray/_memray/compat.h`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/memray/_memray/elf_shenanigans.cpp` & `memray-1.8.0/src/memray/_memray/elf_shenanigans.cpp`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/memray/_memray/elf_utils.h` & `memray-1.8.0/src/memray/_memray/elf_utils.h`

 * *Files 0% similar despite different names*

```diff
@@ -237,15 +237,16 @@
 
         // Search for the symbol in the chain that we found.
         while (true) {
             auto* sym = symbol_table.table + symbol_index;
             const auto* sym_name = string_table.table + sym->st_name;
             const uint32_t hash = chain[symbol_index - symbol_offset];
             if ((namehash | 1) == (hash | 1) && isDefinedGlobalSymbol(sym)
-                && strcmp(sym_name, name) == 0) {
+                && strcmp(sym_name, name) == 0)
+            {
                 return base + sym->st_value;
             }
 
             // Chain ends with an element with the lowest bit set to 1: end of the chain
             if (hash & 1) {
                 break;
             }
```

### Comparing `memray-1.7.0/src/memray/_memray/frame_tree.h` & `memray-1.8.0/src/memray/_memray/frame_tree.h`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/memray/_memray/hooks.cpp` & `memray-1.8.0/src/memray/_memray/hooks.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -186,15 +186,19 @@
 }
 
 void*
 realloc(void* ptr, size_t size) noexcept
 {
     assert(hooks::realloc);
 
-    void* ret = hooks::realloc(ptr, size);
+    void* ret;
+    {
+        tracking_api::RecursionGuard guard;
+        ret = hooks::realloc(ptr, size);
+    }
     if (ret) {
         if (ptr != nullptr) {
             tracking_api::Tracker::trackDeallocation(ptr, 0, hooks::Allocator::FREE);
         }
         tracking_api::Tracker::trackAllocation(ret, size, hooks::Allocator::REALLOC);
     }
     return ret;
@@ -276,16 +280,19 @@
     return ret;
 }
 
 void*
 dlopen(const char* filename, int flag) noexcept
 {
     assert(hooks::dlopen);
-
-    void* ret = hooks::dlopen(filename, flag);
+    void* ret;
+    {
+        tracking_api::RecursionGuard guard;
+        ret = hooks::dlopen(filename, flag);
+    }
     if (ret) {
         tracking_api::Tracker::invalidate_module_cache();
         if (filename && nullptr != strstr(filename, "/_greenlet.")) {
             tracking_api::Tracker::beginTrackingGreenlets();
         }
     }
     return ret;
@@ -303,15 +310,19 @@
 }
 
 void*
 aligned_alloc(size_t alignment, size_t size) noexcept
 {
     assert(hooks::aligned_alloc);
 
-    void* ret = hooks::aligned_alloc(alignment, size);
+    void* ret;
+    {
+        tracking_api::RecursionGuard guard;
+        ret = hooks::aligned_alloc(alignment, size);
+    }
     if (ret) {
         tracking_api::Tracker::trackAllocation(ret, size, hooks::Allocator::ALIGNED_ALLOC);
     }
     return ret;
 }
 
 #if defined(__linux__)
```

### Comparing `memray-1.7.0/src/memray/_memray/hooks.h` & `memray-1.8.0/src/memray/_memray/hooks.h`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/memray/_memray/inject.cpp` & `memray-1.8.0/src/memray/_memray/inject.cpp`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/memray/_memray/logging.cpp` & `memray-1.8.0/src/memray/_memray/logging.cpp`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/memray/_memray/logging.h` & `memray-1.8.0/src/memray/_memray/logging.h`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/memray/_memray/lz4_stream.h` & `memray-1.8.0/src/memray/_memray/lz4_stream.h`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/memray/_memray/macho_shenanigans.cpp` & `memray-1.8.0/src/memray/_memray/macho_shenanigans.cpp`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -144,8 +144,8 @@
 
 void
 SymbolPatcher::restore_symbols() noexcept
 {
     patch_symbols_in_all_shared_objects(true, symbols);
 }
 
-}  // namespace memray::linker
+}  // namespace memray::linker
```

### Comparing `memray-1.7.0/src/memray/_memray/macho_utils.h` & `memray-1.8.0/src/memray/_memray/macho_utils.h`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/memray/_memray/native_resolver.cpp` & `memray-1.8.0/src/memray/_memray/native_resolver.cpp`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/memray/_memray/native_resolver.h` & `memray-1.8.0/src/memray/_memray/native_resolver.h`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/memray/_memray/pthread.pxd` & `memray-1.8.0/src/memray/_memray/pthread.pxd`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -15,8 +15,8 @@
     int pthread_cancel(pthread_t thread)
     int pthread_setcancelstate(int state, int *oldstate)
     pthread_t pthread_self()
     int pthread_equal(pthread_t t1, pthread_t t2)
     int pthread_create(pthread_t *thread, pthread_attr_t *attr,
                        void *(*start_routine) (void *), void *arg)
     int pthread_join(pthread_t thread, void **retval)
-    int pthread_kill(pthread_t thread, int sig)
+    int pthread_kill(pthread_t thread, int sig)
```

### Comparing `memray-1.7.0/src/memray/_memray/python_helpers.cpp` & `memray-1.8.0/src/memray/_memray/python_helpers.cpp`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/memray/_memray/record_reader.cpp` & `memray-1.8.0/src/memray/_memray/record_reader.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -510,15 +510,16 @@
 RecordReader::RecordResult
 RecordReader::nextRecordFromAllAllocationsFile()
 {
     while (true) {
         RecordTypeAndFlags record_type_and_flags;
         if (!d_input->read(
                     reinterpret_cast<char*>(&record_type_and_flags),
-                    sizeof(record_type_and_flags))) {
+                    sizeof(record_type_and_flags)))
+        {
             return RecordResult::END_OF_FILE;
         }
 
         switch (record_type_and_flags.record_type) {
             case RecordType::OTHER: {
                 switch (static_cast<OtherRecordType>(record_type_and_flags.flags)) {
                     case OtherRecordType::TRAILER: {
@@ -529,15 +530,16 @@
                         return RecordResult::ERROR;
                     } break;
                 }
             } break;
             case RecordType::ALLOCATION: {
                 AllocationRecord record;
                 if (!parseAllocationRecord(&record, record_type_and_flags.flags)
-                    || !processAllocationRecord(record)) {
+                    || !processAllocationRecord(record))
+                {
                     if (d_input->is_open()) LOG(ERROR) << "Failed to process allocation record";
                     return RecordResult::ERROR;
                 }
                 return RecordResult::ALLOCATION_RECORD;
             } break;
             case RecordType::ALLOCATION_WITH_NATIVE: {
                 NativeAllocationRecord record;
@@ -645,15 +647,16 @@
 
                 return RecordResult::MEMORY_SNAPSHOT;
             } break;
 
             case AggregatedRecordType::AGGREGATED_ALLOCATION: {
                 AggregatedAllocation record;
                 if (!parseAggregatedAllocationRecord(&record)
-                    || !processAggregatedAllocationRecord(record)) {
+                    || !processAggregatedAllocationRecord(record))
+                {
                     if (d_input->is_open()) {
                         LOG(ERROR) << "Failed to process aggregated allocation record";
                     }
                     return RecordResult::ERROR;
                 }
 
                 return RecordResult::AGGREGATED_ALLOCATION_RECORD;
@@ -967,15 +970,16 @@
         if (0 != PyErr_CheckSignals()) {
             return nullptr;
         }
 
         RecordTypeAndFlags record_type_and_flags;
         if (!d_input->read(
                     reinterpret_cast<char*>(&record_type_and_flags),
-                    sizeof(record_type_and_flags))) {
+                    sizeof(record_type_and_flags)))
+        {
             Py_RETURN_NONE;
         }
 
         switch (record_type_and_flags.record_type) {
             case RecordType::OTHER: {
                 switch (static_cast<OtherRecordType>(record_type_and_flags.flags)) {
                     case OtherRecordType::TRAILER: {
```

### Comparing `memray-1.7.0/src/memray/_memray/record_reader.h` & `memray-1.8.0/src/memray/_memray/record_reader.h`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/memray/_memray/record_reader.pxd` & `memray-1.8.0/src/memray/_memray/record_reader.pxd`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/memray/_memray/record_writer.cpp` & `memray-1.8.0/src/memray/_memray/record_writer.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -231,15 +231,16 @@
             return false;
         }
 
         RecordTypeAndFlags segment_token{RecordType::SEGMENT, 0};
 
         for (const auto& segment : image.segments) {
             if (!writeSimpleType(segment_token) || !writeSimpleType(segment.vaddr)
-                || !writeVarint(segment.memsz)) {
+                || !writeVarint(segment.memsz))
+            {
                 return false;
             }
         }
     }
 
     return true;
 }
```

### Comparing `memray-1.7.0/src/memray/_memray/record_writer.h` & `memray-1.8.0/src/memray/_memray/record_writer.h`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/memray/_memray/records.cpp` & `memray-1.8.0/src/memray/_memray/records.cpp`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/memray/_memray/records.h` & `memray-1.8.0/src/memray/_memray/records.h`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/memray/_memray/records.pxd` & `memray-1.8.0/src/memray/_memray/records.pxd`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/memray/_memray/sink.cpp` & `memray-1.8.0/src/memray/_memray/sink.cpp`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/memray/_memray/sink.h` & `memray-1.8.0/src/memray/_memray/sink.h`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/memray/_memray/snapshot.h` & `memray-1.8.0/src/memray/_memray/snapshot.h`

 * *Files 14% similar despite different names*

```diff
@@ -146,14 +146,24 @@
     }
 
     iterator end()
     {
         return d_intervals.end();
     }
 
+    const_iterator begin() const
+    {
+        return d_intervals.begin();
+    }
+
+    const_iterator end() const
+    {
+        return d_intervals.end();
+    }
+
     const_iterator cbegin()
     {
         return d_intervals.cbegin();
     }
 
     const_iterator cend()
     {
@@ -244,14 +254,16 @@
     thread_id_t thread_id;
     size_t python_frame_id;
     size_t native_frame_id;
     size_t native_segment_generation;
     hooks::Allocator allocator;
 
     bool operator==(const HighWaterMarkLocationKey& rhs) const;
+    bool operator!=(const HighWaterMarkLocationKey& rhs) const;
+    bool operator<(const HighWaterMarkLocationKey& rhs) const;
 };
 
 struct HighWaterMarkLocationKeyHash
 {
     size_t operator()(const HighWaterMarkLocationKey& p) const
     {
         // Keep the fewest bits from the hashes of the fields that vary least.
@@ -260,70 +272,190 @@
         ret = (ret << 1) ^ std::hash<thread_id_t>{}(p.thread_id);
         ret = (ret << 1) ^ std::hash<size_t>{}(p.native_frame_id);
         ret = (ret << 1) ^ std::hash<size_t>{}(p.python_frame_id);
         return ret;
     }
 };
 
-class HighWaterMarkAggregator
+struct Contribution
 {
-  public:
-    void addAllocation(const Allocation& allocation);
-    size_t getCurrentHeapSize() const noexcept;
+    size_t bytes;
+    size_t allocations;
+};
 
-    using allocation_callback_t = std::function<bool(const AggregatedAllocation&)>;
-    bool visitAllocations(const allocation_callback_t& callback) const;
+bool
+operator==(const Contribution& lhs, const Contribution& rhs);
 
-  private:
-    // Number of high water marks found (incremented on the falling edge)
-    uint64_t d_peak_count{};
-    size_t d_heap_size_at_last_peak{};
-    size_t d_current_heap_size{};
+bool
+operator!=(const Contribution& lhs, const Contribution& rhs);
 
+struct HistoricalContribution
+{
+    size_t as_of_snapshot;
+    size_t peak_index;
+    Contribution contrib;
+};
+
+class UsageHistory
+{
+  public:
+    void recordUsageDelta(
+            const std::vector<size_t>& highest_peak_by_snapshot,
+            size_t current_peak,
+            size_t count_delta,
+            size_t bytes_delta);
+
+    Contribution highWaterMarkContribution(size_t highest_peak) const;
+    Contribution leaksContribution() const;
+    std::vector<HistoricalContribution> contributionsBySnapshot(
+            const std::vector<size_t>& highest_peak_by_snapshot,
+            size_t current_peak) const;
+
+  private:
     // This class represents allocations observed at some location over time.
     // When an allocation or deallocation is observed, we first check if a new
     // peak was discovered after the last time an allocation or deallocation
     // was performed here. If so, the counters tracking what happened since the
     // last peak must be merged into allocations_contributed_to_last_known_peak
     // and bytes_contributed_to_last_known_peak and reset: they didn't
     // contribute to the previous peak, but they are accounted for in the newly
     // discovered peak. Finally, we update those counters to account for
     // allocations or deallocations since the current peak.
-    struct UsageHistory
+    struct UsageHistoryImpl
     {
+        uint64_t last_known_snapshot;
         uint64_t last_known_peak;
         size_t allocations_contributed_to_last_known_peak;
         size_t bytes_contributed_to_last_known_peak;
         // NOTE: We may have more deallocations than allocations since the last
         // peak, or more bytes deallocated than allocated. These 2 size_t's
         // may represent negative counts as large positive numbers. That's OK:
         // they represent deltas since the last known peak, and are always
         // added to the values from the last known peak. Unsigned integers use
         // modular arithmetic, and addition will overflow to the correct value.
         size_t count_since_last_peak;
         size_t bytes_since_last_peak;
+
+        // Update so that `last_known_peak == new_peak`.
+        void rebase(size_t new_peak);
     };
 
+    UsageHistoryImpl d_history{};
+    std::vector<HistoricalContribution> d_heap_contribution_by_snapshot;
+
+    // Append records for already-completed snapshots to the given vector.
+    UsageHistoryImpl recordContributionsToCompletedSnapshots(
+            const std::vector<size_t>& highest_peak_by_snapshot,
+            std::vector<HistoricalContribution>& heap_contribution_by_snapshot) const;
+};
+
+struct AllocationLifetime
+{
+    size_t allocatedBeforeSnapshot;
+    size_t deallocatedBeforeSnapshot;  // SIZE_MAX if never deallocated
+    HighWaterMarkLocationKey key;
+    size_t n_allocations;
+    size_t n_bytes;
+};
+
+class HighWaterMarkAggregator
+{
+  public:
+    using Index = std::vector<AllocationLifetime>;
+
+    void addAllocation(const Allocation& allocation);
+    void captureSnapshot();
+
+    size_t getCurrentHeapSize() const noexcept;
+    const std::vector<size_t>& highWaterMarkBytesBySnapshot() const;
+    Index generateIndex() const;
+
+    using allocation_callback_t = std::function<bool(const AggregatedAllocation&)>;
+    bool visitAllocations(const allocation_callback_t& callback) const;
+
+  private:
+    // For each call to captureSnapshot(), record the index of the highest
+    // high water mark found since the last snapshot was taken.
+    std::vector<size_t> d_high_water_mark_index_by_snapshot;
+
+    // For each call to captureSnapshot(), record the heap size at the highest
+    // high water mark found since the last snapshot was taken.
+    std::vector<size_t> d_high_water_mark_bytes_by_snapshot;
+
+    // Number of high water marks found (incremented on the falling edge,
+    // as well as on a new snapshot being taken).
+    uint64_t d_peak_count{};
+    size_t d_heap_size_at_last_peak{};
+    size_t d_current_heap_size{};
+
     // Information about allocations and deallocations, aggregated by location.
     using UsageHistoryByLocation =
             std::unordered_map<HighWaterMarkLocationKey, UsageHistory, HighWaterMarkLocationKeyHash>;
     UsageHistoryByLocation d_usage_history_by_location;
 
     // Simple allocations contributing to the current heap size.
     std::unordered_map<uintptr_t, Allocation> d_ptr_to_allocation;
 
     // Ranged allocations contributing to the current heap size.
     IntervalTree<Allocation> d_mmap_intervals;
 
     UsageHistory& getUsageHistory(const Allocation& allocation);
-    void refreshUsageHistory(UsageHistory& history);
     void recordUsageDelta(const Allocation& allocation, size_t count_delta, size_t bytes_delta);
     reduced_snapshot_map_t getAllocations(bool merge_threads, bool stop_at_high_water_mark) const;
 };
 
+class AllocationLifetimeAggregator
+{
+  public:
+    void addAllocation(const Allocation& allocation);
+    void captureSnapshot();
+
+    std::vector<AllocationLifetime> generateIndex() const;
+
+  private:
+    size_t d_num_snapshots{};
+
+    struct allocation_history_key_hash
+    {
+        size_t operator()(const std::tuple<size_t, size_t, HighWaterMarkLocationKey>& key) const
+        {
+            size_t ret = HighWaterMarkLocationKeyHash{}(std::get<2>(key));
+            ret = (ret << 1) ^ std::get<1>(key);
+            ret = (ret << 1) ^ std::get<0>(key);
+            return ret;
+        }
+    };
+
+    // Record of freed allocations that spanned multiple snapshots.
+    std::unordered_map<
+            std::tuple<size_t, size_t, HighWaterMarkLocationKey>,
+            std::pair<size_t, size_t>,
+            allocation_history_key_hash>
+            d_allocation_history;
+
+    // Simple allocations contributing to the current heap size.
+    std::unordered_map<uintptr_t, std::pair<Allocation, size_t>> d_ptr_to_allocation;
+
+    // Ranged allocations contributing to the current heap size.
+    IntervalTree<std::pair<std::shared_ptr<Allocation>, size_t>> d_mmap_intervals;
+
+    HighWaterMarkLocationKey extractKey(const Allocation& allocation) const;
+
+    void recordRangedDeallocation(
+            const std::shared_ptr<Allocation>& allocation,
+            size_t bytes_deallocated,
+            size_t generation_allocated);
+
+    void recordDeallocation(
+            const HighWaterMarkLocationKey& key,
+            size_t count_delta,
+            size_t bytes_delta,
+            size_t generation);
+};
+
 class AllocationStatsAggregator
 {
   public:
     void addAllocation(const Allocation& allocation, std::optional<frame_id_t> python_frame_id);
 
     uint64_t totalAllocations()
     {
```

### Comparing `memray-1.7.0/src/memray/_memray/socket_reader_thread.cpp` & `memray-1.8.0/src/memray/_memray/socket_reader_thread.cpp`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/memray/_memray/socket_reader_thread.h` & `memray-1.8.0/src/memray/_memray/socket_reader_thread.h`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/memray/_memray/source.cpp` & `memray-1.8.0/src/memray/_memray/source.cpp`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/memray/_memray/source.h` & `memray-1.8.0/src/memray/_memray/source.h`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/memray/_memray/tracking_api.cpp` & `memray-1.8.0/src/memray/_memray/tracking_api.cpp`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/memray/_memray/tracking_api.h` & `memray-1.8.0/src/memray/_memray/tracking_api.h`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/memray/_memray/tracking_api.pxd` & `memray-1.8.0/src/memray/_memray/tracking_api.pxd`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/memray/_memray.pyi` & `memray-1.8.0/src/memray/_memray.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -38,14 +38,18 @@
     @property
     def size(self) -> int: ...
     @property
     def stack_id(self) -> int: ...
     @property
     def tid(self) -> int: ...
     @property
+    def native_stack_id(self) -> int: ...
+    @property
+    def native_segment_generation(self) -> int: ...
+    @property
     def thread_name(self) -> str: ...
     def hybrid_stack_trace(
         self,
         max_stacks: Optional[int] = None,
     ) -> List[Union[PythonStackElement, NativeStackElement]]: ...
     def native_stack_trace(
         self, max_stacks: Optional[int] = None
@@ -57,14 +61,55 @@
     def __ge__(self, other: Any) -> Any: ...
     def __gt__(self, other: Any) -> Any: ...
     def __hash__(self) -> Any: ...
     def __le__(self, other: Any) -> Any: ...
     def __lt__(self, other: Any) -> Any: ...
     def __ne__(self, other: Any) -> Any: ...
 
+class Interval:
+    def __init__(
+        self,
+        allocated_before_snapshot: int,
+        deallocated_before_snapshot: int | None,
+        n_allocations: int,
+        n_bytes: int,
+    ) -> None: ...
+    def __eq__(self, other: Any) -> Any: ...
+    allocated_before_snapshot: int
+    deallocated_before_snapshot: int | None
+    n_allocations: int
+    n_bytes: int
+
+class TemporalAllocationRecord:
+    @property
+    def allocator(self) -> int: ...
+    @property
+    def stack_id(self) -> int: ...
+    @property
+    def tid(self) -> int: ...
+    @property
+    def native_stack_id(self) -> int: ...
+    @property
+    def native_segment_generation(self) -> int: ...
+    @property
+    def thread_name(self) -> str: ...
+    def hybrid_stack_trace(
+        self,
+        max_stacks: Optional[int] = None,
+    ) -> List[Union[PythonStackElement, NativeStackElement]]: ...
+    def native_stack_trace(
+        self, max_stacks: Optional[int] = None
+    ) -> List[NativeStackElement]: ...
+    def stack_trace(
+        self, max_stacks: Optional[int] = None
+    ) -> List[PythonStackElement]: ...
+    def __eq__(self, other: Any) -> Any: ...
+    def __hash__(self) -> Any: ...
+    intervals: List[Interval]
+
 class AllocatorType(enum.IntEnum):
     MALLOC: int
     FREE: int
     CALLOC: int
     REALLOC: int
     POSIX_MEMALIGN: int
     ALIGNED_ALLOC: int
@@ -87,14 +132,22 @@
 class FileReader:
     @property
     def metadata(self) -> Metadata: ...
     def __init__(
         self, file_name: Union[str, Path], *, report_progress: bool = False
     ) -> None: ...
     def get_allocation_records(self) -> Iterable[AllocationRecord]: ...
+    def get_temporal_allocation_records(
+        self,
+        merge_threads: bool,
+    ) -> Iterable[TemporalAllocationRecord]: ...
+    def get_temporal_high_water_mark_allocation_records(
+        self,
+        merge_threads: bool,
+    ) -> Tuple[List[TemporalAllocationRecord], List[int]]: ...
     def get_high_watermark_allocation_records(
         self,
         merge_threads: bool = ...,
     ) -> Iterable[AllocationRecord]: ...
     def get_leaked_allocation_records(
         self, merge_threads: bool = ...
     ) -> Iterable[AllocationRecord]: ...
@@ -201,9 +254,26 @@
         address: int,
         size: int,
         allocator: int,
         native_frame_id: int,
         frame_index: int,
         native_segment_generation: int,
     ) -> None: ...
+    def capture_snapshot(self) -> None: ...
+    def high_water_mark_bytes_by_snapshot(self) -> list[int]: ...
     def get_current_heap_size(self) -> int: ...
+    def get_temporal_allocations(self) -> list[TemporalAllocationRecord]: ...
     def get_allocations(self) -> list[dict[str, int]]: ...
+
+class AllocationLifetimeAggregatorTestHarness:
+    def add_allocation(
+        self,
+        tid: int,
+        address: int,
+        size: int,
+        allocator: int,
+        native_frame_id: int,
+        frame_index: int,
+        native_segment_generation: int,
+    ) -> None: ...
+    def capture_snapshot(self) -> None: ...
+    def get_allocations(self) -> list[TemporalAllocationRecord]: ...
```

### Comparing `memray-1.7.0/src/memray/_memray.pyx` & `memray-1.8.0/src/memray/_memray.pyx`

 * *Files 14% similar despite different names*

```diff
@@ -31,20 +31,24 @@
 from _memray.records cimport FileFormat as _FileFormat
 from _memray.records cimport MemoryRecord
 from _memray.records cimport MemorySnapshot as _MemorySnapshot
 from _memray.sink cimport FileSink
 from _memray.sink cimport NullSink
 from _memray.sink cimport Sink
 from _memray.sink cimport SocketSink
+from _memray.snapshot cimport NO_THREAD_INFO
 from _memray.snapshot cimport AbstractAggregator
 from _memray.snapshot cimport AggregatedCaptureReaggregator
+from _memray.snapshot cimport AllocationLifetime
+from _memray.snapshot cimport AllocationLifetimeAggregator
 from _memray.snapshot cimport AllocationStatsAggregator
 from _memray.snapshot cimport HighWatermark
 from _memray.snapshot cimport HighWaterMarkAggregator
 from _memray.snapshot cimport HighWatermarkFinder
+from _memray.snapshot cimport HighWaterMarkLocationKey
 from _memray.snapshot cimport Py_GetSnapshotAllocationRecords
 from _memray.snapshot cimport Py_ListFromSnapshotAllocationRecords
 from _memray.snapshot cimport SnapshotAllocationAggregator
 from _memray.snapshot cimport TemporaryAllocationsAggregator
 from _memray.socket_reader_thread cimport BackgroundSocketReader
 from _memray.source cimport FileSource
 from _memray.source cimport SocketSource
@@ -116,26 +120,146 @@
         if abs(num) < 1024.0:
             return f"{num:5.3f}{unit}{suffix}"
         num /= 1024.0
     return f"{num:.1f}Y{suffix}"
 
 # Memray core
 
-PYTHON_VERSION = (sys.version_info.major, sys.version_info.minor)
+cdef stack_trace(
+    RecordReader* reader,
+    tid,
+    allocator,
+    python_stack_id,
+    max_stacks=None,
+):
+    if allocator in (AllocatorType.FREE, AllocatorType.MUNMAP):
+        raise NotImplementedError("Stack traces for deallocations aren't captured.")
+
+    assert reader != NULL, "Cannot get stack trace without reader."
+    cdef ssize_t to_skip
+    cdef ssize_t to_keep
+
+    if max_stacks is not None:
+        return reader.Py_GetStackFrame(python_stack_id, max_stacks)
+
+    stack_trace = reader.Py_GetStackFrame(python_stack_id)
+    if tid == reader.getMainThreadTid():
+        to_skip = reader.getSkippedFramesOnMainThread()
+        to_keep = max(len(stack_trace) - to_skip, 0)
+        del stack_trace[to_keep:]
+    return stack_trace
+
+
+cdef native_stack_trace(
+    RecordReader* reader,
+    allocator,
+    native_stack_id,
+    generation,
+    max_stacks=None,
+):
+    if allocator in (AllocatorType.FREE, AllocatorType.MUNMAP):
+        raise NotImplementedError("Stack traces for deallocations aren't captured.")
+
+    assert reader != NULL, "Cannot get stack trace without reader."
+    if max_stacks is None:
+        return reader.Py_GetNativeStackFrame(native_stack_id, generation)
+    return reader.Py_GetNativeStackFrame(native_stack_id, generation, max_stacks)
+
+
+cdef hybrid_stack_trace(
+    RecordReader* reader,
+    tid,
+    allocator,
+    python_stack_id,
+    native_stack_id,
+    generation,
+    max_stacks=None,
+):
+    # This function merges a Python stack and a native stack into
+    # a "hybrid" stack. It substitutes _PyFrame_EvalFrameDefault calls in
+    # the native stack with the corresponding frame in the Python stack.
+    # This sounds easy, but there are several tricky aspects:
+    # 1. For the thread that called Tracker.__enter__, we want to hide
+    #    frames (both Python and C) above the one that made that call.
+    #    For other threads we want to keep all frames.
+    # 2. If _PyFrame_EvalFrameDefault allocates memory before calling our
+    #    profile function, we'll have too few Python frames to pair up
+    #    every _PyFrame_EvalFrameDefault call. This happens in 3.11.
+    # 3. Since Python 3.11, one _PyFrame_EvalFrameDefault call can evaluate
+    #    many Python frames. If a frame's is_entry_frame flag is unset, it
+    #    uses the same _PyFrame_EvalFrameDefault call as its caller.
+    # 4. If the interpreter was stripped, we may not be able to recognize
+    #    every (or even any) _PyFrame_EvalFrameDefault call, so we may
+    #    have extra Python frames left after pairing.
+    cdef vector[unsigned char] is_entry_frame
+    native_stack = native_stack_trace(reader, allocator, native_stack_id, generation)
+    python_stack = reader.Py_GetStackFrameAndEntryInfo(python_stack_id, &is_entry_frame)
+
+    cdef ssize_t num_non_entry_frames = count(
+        is_entry_frame.begin(), is_entry_frame.end(), 0
+    )
+
+    # Entry frames replace native frames; non-entry frames are inserted.
+    hybrid_stack = [None] * (len(native_stack) + num_non_entry_frames)
+
+    # Both stacks are from most recent to least, but we must pair things up
+    # least recent to most to handle cases where _PyFrame_EvalFrameDefault
+    # allocated memory before calling the profile function.
+    native_stack.reverse()
+    cdef ssize_t pidx = len(python_stack) - 1
+    cdef ssize_t hidx = len(hybrid_stack) - 1
+
+    cdef ssize_t to_skip = 0
+    if tid == reader.getMainThreadTid():
+        to_skip = reader.getSkippedFramesOnMainThread()
+    cdef ssize_t first_kept_frame = pidx - to_skip
+
+    for native_frame in native_stack:
+        symbol = native_frame[0]
+        if pidx >= 0 and "_PyEval_EvalFrameDefault" in symbol:
+            while True:
+                # If we're not keeping all frames and we've reached the
+                # first one we want to keep, remove frames above it.
+                if to_skip != 0 and pidx == first_kept_frame:
+                    del hybrid_stack[hidx + 1:]
+
+                assert hidx >= 0
+                hybrid_stack[hidx] = python_stack[pidx]
+                hidx -= 1
+                pidx -= 1
+
+                # Stop when we either run out of Python frames or reach the
+                # entry frame being evaluated by the next eval loop.
+                if pidx < 0 or is_entry_frame[pidx]:
+                    break
+        else:
+            assert hidx >= 0
+            hybrid_stack[hidx] = native_frame
+            hidx -= 1
+
+    if pidx >= 0:
+        # We ran out of native frames without using up all of our Python
+        # frames. We've seen this happen on stripped interpreters on Alpine
+        # Linux in CI. Presumably this indicates that unwinding failed to
+        # symbolify some of the calls to _PyEval_EvalFrameDefault.
+        return python_stack
+    assert hidx == -1
+
+    return hybrid_stack[:max_stacks]
+
 
 @cython.freelist(1024)
 cdef class AllocationRecord:
     cdef object _tuple
-    cdef object _stack_trace
-    cdef object _native_stack_trace
+    cdef dict _stack_trace_cache
     cdef shared_ptr[RecordReader] _reader
 
     def __init__(self, record):
         self._tuple = record
-        self._stack_trace = None
+        self._stack_trace_cache = {}
 
     def __eq__(self, other):
         cdef AllocationRecord _other
         if isinstance(other, AllocationRecord):
             _other = other
             return self._tuple == _other._tuple
         return NotImplemented
@@ -164,136 +288,276 @@
         return self._tuple[4]
 
     @property
     def n_allocations(self):
         return self._tuple[5]
 
     @property
+    def native_stack_id(self):
+        return self._tuple[6]
+
+    @property
+    def native_segment_generation(self):
+        return self._tuple[7]
+
+    @property
     def thread_name(self):
         if self.tid == -1:
             return "merged thread"
         assert self._reader.get() != NULL, "Cannot get thread name without reader."
         cdef object name = self._reader.get().getThreadName(self.tid)
         thread_id = hex(self.tid)
         return f"{thread_id} ({name})" if name else f"{thread_id}"
 
     def stack_trace(self, max_stacks=None):
-        assert self._reader.get() != NULL, "Cannot get stack trace without reader."
-        cdef ssize_t to_skip
-        cdef ssize_t to_keep
-        if self._stack_trace is None:
-            if self.allocator in (AllocatorType.FREE, AllocatorType.MUNMAP):
-                raise NotImplementedError("Stack traces for deallocations aren't captured.")
-
-            if max_stacks is None:
-                self._stack_trace = self._reader.get().Py_GetStackFrame(self._tuple[4])
-                if self._tuple[0] == self._reader.get().getMainThreadTid():
-                    to_skip = self._reader.get().getSkippedFramesOnMainThread()
-                    to_keep = max(len(self._stack_trace) - to_skip, 0)
-                    del self._stack_trace[to_keep:]
-            else:
-                self._stack_trace = self._reader.get().Py_GetStackFrame(self._tuple[4], max_stacks)
-        return self._stack_trace
+        cache_key = ("python", max_stacks)
+        if cache_key not in self._stack_trace_cache:
+            self._stack_trace_cache[cache_key] = stack_trace(
+                self._reader.get(),
+                self.tid,
+                self.allocator,
+                self.stack_id,
+                max_stacks,
+            )
+        return self._stack_trace_cache[cache_key]
 
     def native_stack_trace(self, max_stacks=None):
-        assert self._reader.get() != NULL, "Cannot get stack trace without reader."
-        if self._native_stack_trace is None:
-            if self.allocator in (AllocatorType.FREE, AllocatorType.MUNMAP):
-                raise NotImplementedError("Stack traces for deallocations aren't captured.")
-
-            if max_stacks is None:
-                self._native_stack_trace = self._reader.get().Py_GetNativeStackFrame(
-                        self._tuple[6], self._tuple[7])
-            else:
-                self._native_stack_trace = self._reader.get().Py_GetNativeStackFrame(
-                        self._tuple[6], self._tuple[7], max_stacks)
-        return self._native_stack_trace
-
-    cdef _is_eval_frame(self, object symbol):
-        return "_PyEval_EvalFrameDefault" in symbol
+        cache_key = ("native", max_stacks)
+        if cache_key not in self._stack_trace_cache:
+            self._stack_trace_cache[cache_key] = native_stack_trace(
+                self._reader.get(),
+                self.allocator,
+                self.native_stack_id,
+                self.native_segment_generation,
+                max_stacks,
+            )
+        return self._stack_trace_cache[cache_key]
 
     def hybrid_stack_trace(self, max_stacks=None):
-        # This function merges a Python stack and a native stack into
-        # a "hybrid" stack. It substitutes _PyFrame_EvalFrameDefault calls in
-        # the native stack with the corresponding frame in the Python stack.
-        # This sounds easy, but there are several tricky aspects:
-        # 1. For the thread that called Tracker.__enter__, we want to hide
-        #    frames (both Python and C) above the one that made that call.
-        #    For other threads we want to keep all frames.
-        # 2. If _PyFrame_EvalFrameDefault allocates memory before calling our
-        #    profile function, we'll have too few Python frames to pair up
-        #    every _PyFrame_EvalFrameDefault call. This happens in 3.11.
-        # 3. Since Python 3.11, one _PyFrame_EvalFrameDefault call can evaluate
-        #    many Python frames. If a frame's is_entry_frame flag is unset, it
-        #    uses the same _PyFrame_EvalFrameDefault call as its caller.
-        # 4. If the interpreter was stripped, we may not be able to recognize
-        #    every (or even any) _PyFrame_EvalFrameDefault call, so we may
-        #    have extra Python frames left after pairing.
-        cdef vector[unsigned char] is_entry_frame
-        python_stack = self._reader.get().Py_GetStackFrameAndEntryInfo(
-            self._tuple[4], &is_entry_frame
+        cache_key = ("hybrid", max_stacks)
+        if cache_key not in self._stack_trace_cache:
+            self._stack_trace_cache[cache_key] = hybrid_stack_trace(
+                self._reader.get(),
+                self.tid,
+                self.allocator,
+                self.stack_id,
+                self.native_stack_id,
+                self.native_segment_generation,
+                max_stacks,
+            )
+        return self._stack_trace_cache[cache_key]
+
+    def __repr__(self):
+        return (f"AllocationRecord<tid={hex(self.tid)}, address={hex(self.address)}, "
+                f"size={'N/A' if not self.size else size_fmt(self.size)}, allocator={self.allocator!r}, "
+                f"allocations={self.n_allocations}>")
+
+
+@cython.freelist(1024)
+cdef class Interval:
+    cdef public size_t allocated_before_snapshot
+    cdef public object deallocated_before_snapshot
+    cdef public size_t n_allocations
+    cdef public size_t n_bytes
+
+    def __cinit__(
+        self,
+        size_t allocated_before_snapshot,
+        object deallocated_before_snapshot,
+        size_t n_allocations,
+        size_t n_bytes,
+    ):
+        self.allocated_before_snapshot = allocated_before_snapshot
+        self.deallocated_before_snapshot = deallocated_before_snapshot
+        self.n_allocations = n_allocations
+        self.n_bytes = n_bytes
+
+    def __eq__(self, other):
+        if type(other) is not Interval:
+            return NotImplemented
+        return (
+            self.allocated_before_snapshot,
+            self.deallocated_before_snapshot,
+            self.n_allocations,
+            self.n_bytes,
+        ) == (
+            other.allocated_before_snapshot,
+            other.deallocated_before_snapshot,
+            other.n_allocations,
+            other.n_bytes,
         )
-        native_stack = self.native_stack_trace()
 
-        cdef ssize_t num_non_entry_frames = count(
-            is_entry_frame.begin(), is_entry_frame.end(), 0
+    def __repr__(self):
+        return (
+            f"Interval(allocated_before_snapshot={self.allocated_before_snapshot},"
+            f" deallocated_before_snapshot={self.deallocated_before_snapshot},"
+            f" n_allocations={self.n_allocations},"
+            f" n_bytes={self.n_bytes})"
         )
 
-        # Entry frames replace native frames; non-entry frames are inserted.
-        hybrid_stack = [None] * (len(native_stack) + num_non_entry_frames)
 
-        # Both stacks are from most recent to least, but we must pair things up
-        # least recent to most to handle cases where _PyFrame_EvalFrameDefault
-        # allocated memory before calling the profile function.
-        native_stack.reverse()
-        cdef ssize_t pidx = len(python_stack) - 1
-        cdef ssize_t hidx = len(hybrid_stack) - 1
-
-        cdef ssize_t to_skip = 0
-        if self._tuple[0] == self._reader.get().getMainThreadTid():
-            to_skip = self._reader.get().getSkippedFramesOnMainThread()
-        cdef ssize_t first_kept_frame = pidx - to_skip
-
-        for native_frame in native_stack:
-            symbol = native_frame[0]
-            if pidx >= 0 and self._is_eval_frame(symbol):
-                while True:
-                    # If we're not keeping all frames and we've reached the
-                    # first one we want to keep, remove frames above it.
-                    if to_skip != 0 and pidx == first_kept_frame:
-                        del hybrid_stack[hidx + 1:]
-
-                    assert hidx >= 0
-                    hybrid_stack[hidx] = python_stack[pidx]
-                    hidx -= 1
-                    pidx -= 1
-
-                    # Stop when we either run out of Python frames or reach the
-                    # entry frame being evaluated by the next eval loop.
-                    if pidx < 0 or is_entry_frame[pidx]:
-                        break
+@cython.freelist(1024)
+cdef class TemporalAllocationRecord:
+    cdef object _tuple
+    cdef dict _stack_trace_cache
+    cdef shared_ptr[RecordReader] _reader
+    cdef public object intervals
+
+    def __cinit__(self, record):
+        self._tuple = record
+        self._stack_trace_cache = {}
+        self.intervals = []
+
+    def __eq__(self, other):
+        if type(other) != TemporalAllocationRecord:
+            return NotImplemented
+        cdef TemporalAllocationRecord o = other
+        return self._tuple == o._tuple and self._intervals == o._intervals
+
+    def __hash__(self):
+        return hash(self._tuple)
+
+    @property
+    def tid(self):
+        return self._tuple[0]
+
+    @property
+    def allocator(self):
+        return self._tuple[1]
+
+    @property
+    def stack_id(self):
+        return self._tuple[2]
+
+    @property
+    def native_stack_id(self):
+        return self._tuple[3]
+
+    @property
+    def native_segment_generation(self):
+        return self._tuple[4]
+
+    @property
+    def thread_name(self):
+        assert self._reader.get() != NULL, "Cannot get thread name without reader."
+        cdef object name = self._reader.get().getThreadName(self.tid)
+        thread_id = hex(self.tid)
+        return f"{thread_id} ({name})" if name else f"{thread_id}"
+
+    def stack_trace(self, max_stacks=None):
+        cache_key = ("python", max_stacks)
+        if cache_key not in self._stack_trace_cache:
+            self._stack_trace_cache[cache_key] = stack_trace(
+                self._reader.get(),
+                self.tid,
+                self.allocator,
+                self.stack_id,
+                max_stacks,
+            )
+        return self._stack_trace_cache[cache_key]
+
+    def native_stack_trace(self, max_stacks=None):
+        cache_key = ("native", max_stacks)
+        if cache_key not in self._stack_trace_cache:
+            self._stack_trace_cache[cache_key] = native_stack_trace(
+                self._reader.get(),
+                self.allocator,
+                self.native_stack_id,
+                self.native_segment_generation,
+                max_stacks,
+            )
+        return self._stack_trace_cache[cache_key]
+
+    def hybrid_stack_trace(self, max_stacks=None):
+        cache_key = ("hybrid", max_stacks)
+        if cache_key not in self._stack_trace_cache:
+            self._stack_trace_cache[cache_key] = hybrid_stack_trace(
+                self._reader.get(),
+                self.tid,
+                self.allocator,
+                self.stack_id,
+                self.native_stack_id,
+                self.native_segment_generation,
+                max_stacks,
+            )
+        return self._stack_trace_cache[cache_key]
+
+
+cdef create_temporal_allocation_record(
+    const HighWaterMarkLocationKey& key,
+    shared_ptr[RecordReader] reader,
+):
+    cdef object elem = (
+        key.thread_id,
+        <int>key.allocator,
+        key.python_frame_id,
+        key.native_frame_id,
+        key.native_segment_generation,
+    )
+    cdef TemporalAllocationRecord alloc = TemporalAllocationRecord(elem)
+    alloc._reader = reader
+    return alloc
+
+
+cdef class TemporalAllocationGenerator:
+    cdef vector[AllocationLifetime] lifetimes
+    cdef shared_ptr[RecordReader] reader
+
+    cdef TemporalAllocationRecord curr_record
+    cdef HighWaterMarkLocationKey last_key
+    cdef size_t idx
+
+    cdef setup(
+        self,
+        vector[AllocationLifetime]&& lifetimes,
+        shared_ptr[RecordReader] reader,
+    ):
+        self.lifetimes = move(lifetimes)
+        self.reader = move(reader)
+
+    def __iter__(self):
+        return self
+
+    def __next__(self):
+        to_return = None
+        cdef AllocationLifetime lifetime
+        while self.idx < self.lifetimes.size():
+            lifetime = self.lifetimes[self.idx]
+            self.idx += 1
+
+            if lifetime.key != self.last_key:
+                if self.curr_record is not None:
+                    to_return = self.curr_record
+                self.last_key = lifetime.key
+                self.curr_record = create_temporal_allocation_record(
+                    lifetime.key, self.reader
+                )
+
+            if lifetime.deallocatedBeforeSnapshot == <size_t>(-1):
+                deallocated_before_snapshot = None
             else:
-                assert hidx >= 0
-                hybrid_stack[hidx] = native_frame
-                hidx -= 1
+                deallocated_before_snapshot = lifetime.deallocatedBeforeSnapshot
 
-        assert hidx == -1
-        if pidx >= 0:
-            # We ran out of native frames without using up all of our Python
-            # frames. We've seen this happen on stripped interpreters on Alpine
-            # Linux in CI. Presumably this indicates that unwinding failed to
-            # symbolify some of the calls to _PyEval_EvalFrameDefault.
-            return [("<unknown stack>", "<unknown>", 0)]
+            self.curr_record.intervals.append(
+                Interval(
+                    lifetime.allocatedBeforeSnapshot,
+                    deallocated_before_snapshot,
+                    lifetime.n_allocations,
+                    lifetime.n_bytes,
+                )
+            )
 
-        return hybrid_stack[:max_stacks]
+            if to_return is not None:
+                return to_return
 
-    def __repr__(self):
-        return (f"AllocationRecord<tid={hex(self.tid)}, address={hex(self.address)}, "
-                f"size={'N/A' if not self.size else size_fmt(self.size)}, allocator={self.allocator!r}, "
-                f"allocations={self.n_allocations}>")
+        if self.curr_record is not None:
+            to_return = self.curr_record
+            self.curr_record = None
+            return to_return
+        raise StopIteration
 
 
 MemorySnapshot = collections.namedtuple("MemorySnapshot", "time rss heap")
 
 cdef class ProfileFunctionGuard:
     def __dealloc__(self):
         """When our profile function gets deregistered, drop our cached stack.
@@ -530,15 +794,15 @@
             )
 
     def __enter__(self):
         if not self._report_progress:
             return self
         self._context_manager = self._indicator.__enter__()
         self._task = self._context_manager.add_task(
-            f"[blue]{self._task_description}...",
+            f"[cyan]{self._task_description}...",
             total=self._total
         )
         return self
 
     def __exit__(self, type, value, traceback):
         if not self._report_progress:
             return
@@ -809,14 +1073,103 @@
         cdef size_t max_records = self._header["stats"]["n_allocations"]
         yield from self._aggregate_allocations(
             max_records,
             merge_threads,
             temporary_buffer_size=threshold + 1,
         )
 
+    def get_temporal_allocation_records(self, merge_threads=True):
+        self._ensure_not_closed()
+        if self._header["file_format"] == FileFormat.AGGREGATED_ALLOCATIONS:
+            raise NotImplementedError(
+                "Can't get allocation history using a pre-aggregated capture file."
+            )
+
+        cdef shared_ptr[RecordReader] reader_sp = make_shared[RecordReader](
+            unique_ptr[FileSource](new FileSource(self._path))
+        )
+        cdef RecordReader* reader = reader_sp.get()
+
+        cdef size_t records_to_process = self._header["stats"]["n_allocations"]
+        cdef ProgressIndicator progress_indicator = ProgressIndicator(
+            "Processing allocation records",
+            total=records_to_process,
+            report_progress=self._report_progress
+        )
+
+        cdef AllocationLifetimeAggregator aggregator
+        cdef _Allocation allocation
+
+        with progress_indicator:
+            while records_to_process > 0:
+                PyErr_CheckSignals()
+                ret = reader.nextRecord()
+                if ret == RecordResult.RecordResultAllocationRecord:
+                    allocation = reader.getLatestAllocation()
+                    if merge_threads:
+                        allocation.tid = NO_THREAD_INFO
+                    aggregator.addAllocation(allocation)
+                    records_to_process -= 1
+                    progress_indicator.update(1)
+                elif ret == RecordResult.RecordResultMemoryRecord:
+                    aggregator.captureSnapshot()
+                else:
+                    assert ret != RecordResult.RecordResultMemorySnapshot
+                    assert ret != RecordResult.RecordResultAggregatedAllocationRecord
+                    break
+
+        cdef TemporalAllocationGenerator gen = TemporalAllocationGenerator()
+        gen.setup(move(aggregator.generateIndex()), reader_sp)
+        yield from gen
+
+    def get_temporal_high_water_mark_allocation_records(self, merge_threads=True):
+        self._ensure_not_closed()
+        if self._header["file_format"] == FileFormat.AGGREGATED_ALLOCATIONS:
+            raise NotImplementedError(
+                "Can't get allocation history using a pre-aggregated capture file."
+            )
+
+        cdef shared_ptr[RecordReader] reader_sp = make_shared[RecordReader](
+            unique_ptr[FileSource](new FileSource(self._path))
+        )
+        cdef RecordReader* reader = reader_sp.get()
+
+        cdef size_t records_to_process = self._header["stats"]["n_allocations"]
+        cdef ProgressIndicator progress_indicator = ProgressIndicator(
+            "Processing allocation records",
+            total=records_to_process,
+            report_progress=self._report_progress
+        )
+
+        cdef HighWaterMarkAggregator aggregator
+        cdef _Allocation allocation
+
+        with progress_indicator:
+            while records_to_process > 0:
+                PyErr_CheckSignals()
+                ret = reader.nextRecord()
+                if ret == RecordResult.RecordResultAllocationRecord:
+                    allocation = reader.getLatestAllocation()
+                    if merge_threads:
+                        allocation.tid = 0
+                    aggregator.addAllocation(allocation)
+                    records_to_process -= 1
+                    progress_indicator.update(1)
+                elif ret == RecordResult.RecordResultMemoryRecord:
+                    aggregator.captureSnapshot()
+                else:
+                    assert ret != RecordResult.RecordResultMemorySnapshot
+                    assert ret != RecordResult.RecordResultAggregatedAllocationRecord
+                    break
+
+        cdef TemporalAllocationGenerator gen = TemporalAllocationGenerator()
+        gen.setup(move(aggregator.generateIndex()), reader_sp)
+        hwm_by_snapshot = aggregator.highWaterMarkBytesBySnapshot()
+        return gen, hwm_by_snapshot
+
     def get_allocation_records(self):
         self._ensure_not_closed()
         if self._header["file_format"] == FileFormat.AGGREGATED_ALLOCATIONS:
             raise NotImplementedError(
                 "Can't get all allocations from a pre-aggregated capture file."
             )
 
@@ -1087,17 +1440,29 @@
         allocation.allocator = <Allocator><int>allocator
         allocation.native_frame_id = native_frame_id
         allocation.frame_index = frame_index
         allocation.native_segment_generation = native_segment_generation
         allocation.n_allocations = 1
         self.aggregator.addAllocation(allocation)
 
+    def capture_snapshot(self):
+        return self.aggregator.captureSnapshot()
+
+    def high_water_mark_bytes_by_snapshot(self):
+        return self.aggregator.highWaterMarkBytesBySnapshot()
+
     def get_current_heap_size(self):
         return self.aggregator.getCurrentHeapSize()
 
+    def get_temporal_allocations(self):
+        cdef shared_ptr[RecordReader] reader
+        cdef TemporalAllocationGenerator gen = TemporalAllocationGenerator()
+        gen.setup(move(self.aggregator.generateIndex()), reader)
+        yield from gen
+
     def get_allocations(self):
         ret = []
         for allocation in collectAllocations(self.aggregator):
             ret.append(
                 dict(
                     tid=allocation.tid,
                     allocator=AllocatorType(<int>allocation.allocator),
@@ -1107,7 +1472,41 @@
                     n_allocations_in_high_water_mark=allocation.n_allocations_in_high_water_mark,
                     n_allocations_leaked=allocation.n_allocations_leaked,
                     bytes_in_high_water_mark=allocation.bytes_in_high_water_mark,
                     bytes_leaked=allocation.bytes_leaked,
                 )
             )
         return ret
+
+
+cdef class AllocationLifetimeAggregatorTestHarness:
+    cdef AllocationLifetimeAggregator aggregator
+
+    def add_allocation(
+        self,
+        tid,
+        address,
+        size,
+        allocator,
+        native_frame_id,
+        frame_index,
+        native_segment_generation,
+    ):
+        cdef _Allocation allocation
+        allocation.tid = tid
+        allocation.address = address
+        allocation.size = size
+        allocation.allocator = <Allocator><int>allocator
+        allocation.native_frame_id = native_frame_id
+        allocation.frame_index = frame_index
+        allocation.native_segment_generation = native_segment_generation
+        allocation.n_allocations = 1
+        self.aggregator.addAllocation(allocation)
+
+    def capture_snapshot(self):
+        return self.aggregator.captureSnapshot()
+
+    def get_allocations(self):
+        cdef shared_ptr[RecordReader] reader
+        cdef TemporalAllocationGenerator gen = TemporalAllocationGenerator()
+        gen.setup(move(self.aggregator.generateIndex()), reader)
+        yield from gen
```

### Comparing `memray-1.7.0/src/memray/_memray_test_utils.pyx` & `memray-1.8.0/src/memray/_memray_test_utils.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -158,41 +158,41 @@
             self.ptr = PyMem_RawMalloc(size)
         elif self.domain == PYMALLOC_MEM:
             self.ptr = PyMem_Malloc(size)
         elif self.domain == PYMALLOC_OBJECT:
             self.ptr = PyObject_Malloc(size)
         else:
             raise RuntimeError("Invlid pymalloc domain")
- 
+
         return self.ptr != NULL
 
     @cython.profile(True)
     def calloc(self, size_t size):
         if self.domain == PYMALLOC_RAW:
             self.ptr = PyMem_RawCalloc(1, size)
         elif self.domain == PYMALLOC_MEM:
             self.ptr = PyMem_Calloc(1, size)
         elif self.domain == PYMALLOC_OBJECT:
             self.ptr = PyObject_Calloc(1, size)
         else:
             raise RuntimeError("Invlid pymalloc domain")
- 
+
         return self.ptr != NULL
 
     @cython.profile(True)
     def realloc(self, size_t size):
         if self.domain == PYMALLOC_RAW:
             self.ptr = PyMem_RawRealloc(self.ptr, size)
         elif self.domain == PYMALLOC_MEM:
             self.ptr = PyMem_Realloc(self.ptr, size)
         elif self.domain == PYMALLOC_OBJECT:
             self.ptr = PyObject_Realloc(self.ptr, size)
         else:
             raise RuntimeError("Invlid pymalloc domain")
- 
+
         return self.ptr != NULL
 
 cdef do_not_optimize_ptr(void* ptr):
     return ptr == <void*>(1)
 
 @cython.profile(True)
 def _cython_nested_allocation(allocator_fn, size):
```

### Comparing `memray-1.7.0/src/memray/_test.py` & `memray-1.8.0/src/memray/_test.py`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/memray/_test_utils.pyi` & `memray-1.8.0/src/memray/_test_utils.pyi`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/memray/commands/__init__.py` & `memray-1.8.0/src/memray/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/memray/commands/_attach.gdb` & `memray-1.8.0/src/memray/commands/_attach.gdb`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/memray/commands/_attach.lldb` & `memray-1.8.0/src/memray/commands/_attach.lldb`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/memray/commands/attach.py` & `memray-1.8.0/src/memray/commands/attach.py`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/memray/commands/flamegraph.py` & `memray-1.8.0/src/memray/commands/summary.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,48 +1,39 @@
 import argparse
+import os
+from pathlib import Path
 from textwrap import dedent
-from typing import cast
 
-from ..reporters.flamegraph import FlameGraphReporter
-from .common import HighWatermarkCommand
-from .common import ReporterFactory
+from memray import FileReader
+from memray._errors import MemrayCommandError
+from memray.commands.common import warn_if_not_enough_symbols
+from memray.reporters.summary import SummaryReporter
 
 
-class FlamegraphCommand(HighWatermarkCommand):
-    """Generate an HTML flame graph for peak memory usage"""
-
-    def __init__(self) -> None:
-        super().__init__(
-            reporter_factory=cast(ReporterFactory, FlameGraphReporter.from_snapshot),
-            reporter_name="flamegraph",
-        )
+class SummaryCommand:
+    """Generate a terminal-based summary report of the functions that allocate most memory"""
 
     def prepare_parser(self, parser: argparse.ArgumentParser) -> None:
+        parser.add_argument("results", help="Results of the tracker run")
         parser.add_argument(
-            "-o",
-            "--output",
-            help="Output file name",
-            default=None,
+            "-s",
+            "--sort-column",
+            help="Column number to sort on",
+            type=int,
+            default=1,
         )
         parser.add_argument(
-            "-f",
-            "--force",
-            help="If the output file already exists, overwrite it",
-            action="store_true",
-            default=False,
+            "-r",
+            "--max-rows",
+            help="Maximum number of rows to display",
+            type=int,
+            default=None,
         )
         alloc_type_group = parser.add_mutually_exclusive_group()
         alloc_type_group.add_argument(
-            "--leaks",
-            help="Show memory leaks, instead of peak memory usage",
-            action="store_true",
-            dest="show_memory_leaks",
-            default=False,
-        )
-        alloc_type_group.add_argument(
             "--temporary-allocation-threshold",
             metavar="N",
             help=dedent(
                 """
                 Report temporary allocations, as opposed to leaked allocations
                 or high watermark allocations.  An allocation is considered
                 temporary if at most N other allocations occur before it is
@@ -59,14 +50,42 @@
             "--temporary-allocations",
             help="Equivalent to --temporary-allocation-threshold=1",
             action="store_const",
             dest="temporary_allocation_threshold",
             const=1,
         )
 
-        parser.add_argument(
-            "--split-threads",
-            help="Do not merge allocations across threads",
-            action="store_true",
-            default=False,
+    def run(self, args: argparse.Namespace, parser: argparse.ArgumentParser) -> None:
+        max_cols = SummaryReporter.N_COLUMNS
+        if args.sort_column < 1 or args.sort_column > max_cols:
+            parser.error(f"The --sort-column argument must be between 1 and {max_cols}")
+
+        result_path = Path(args.results)
+        if not result_path.exists() or not result_path.is_file():
+            raise MemrayCommandError(f"No such file: {args.results}", exit_code=1)
+
+        try:
+            reader = FileReader(os.fspath(args.results), report_progress=True)
+            if reader.metadata.has_native_traces:
+                warn_if_not_enough_symbols()
+
+            if args.temporary_allocation_threshold >= 0:
+                snapshot = iter(
+                    reader.get_temporary_allocation_records(
+                        threshold=args.temporary_allocation_threshold,
+                        merge_threads=False,
+                    )
+                )
+            else:
+                snapshot = iter(
+                    reader.get_high_watermark_allocation_records(merge_threads=True)
+                )
+        except OSError as e:
+            raise MemrayCommandError(
+                f"Failed to parse allocation records in {result_path}\nReason: {e}",
+                exit_code=1,
+            )
+        reporter = SummaryReporter.from_snapshot(
+            snapshot,
+            native=reader.metadata.has_native_traces,
         )
-        parser.add_argument("results", help="Results of the tracker run")
+        reporter.render(sort_column=args.sort_column, max_rows=args.max_rows)
```

### Comparing `memray-1.7.0/src/memray/commands/live.py` & `memray-1.8.0/src/memray/commands/live.py`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/memray/commands/parse.py` & `memray-1.8.0/src/memray/commands/parse.py`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/memray/commands/run.py` & `memray-1.8.0/src/memray/commands/run.py`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/memray/commands/stats.py` & `memray-1.8.0/src/memray/commands/stats.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import argparse
 import os
 from pathlib import Path
+from typing import Optional
 
 from memray._errors import MemrayCommandError
 from memray._memray import compute_statistics
 from memray.reporters.stats import StatsReporter
 
 
 class StatsCommand:
@@ -29,14 +30,34 @@
             "-n",
             "--num-largest",
             help="Displays the top 'n' largest allocating functions. Default is 5",
             type=valid_positive_int,
             default=5,
         )
 
+        parser.add_argument(
+            "--json",
+            help="Exports stats to a JSON file",
+            action="store_true",
+            default=False,
+        )
+        parser.add_argument(
+            "-o",
+            "--output",
+            help="Output file name for JSON output",
+            default=None,
+        )
+        parser.add_argument(
+            "-f",
+            "--force",
+            help="If the JSON output file already exists, overwrite it",
+            action="store_true",
+            default=False,
+        )
+
     def run(self, args: argparse.Namespace, parser: argparse.ArgumentParser) -> None:
         result_path = Path(args.results)
         if not result_path.exists() or not result_path.is_file():
             raise MemrayCommandError(f"No such file: {args.results}", exit_code=1)
         try:
             stats = compute_statistics(
                 os.fspath(args.results),
@@ -45,9 +66,28 @@
             )
         except OSError as e:
             raise MemrayCommandError(
                 f"Failed to compute statistics for {result_path}\nReason: {e}",
                 exit_code=1,
             )
 
+        json_output_file: Optional[Path] = None
+        if args.json:
+            if args.output:
+                json_output_file = Path(args.output)
+            else:
+                filename = str(result_path.name) + ".json"
+                if filename.startswith("memray-"):
+                    filename = filename[len("memray-") :]
+                filename = "memray-stats-" + filename
+                json_output_file = result_path.with_name(filename)
+
+            if not args.force and json_output_file.exists():
+                raise MemrayCommandError(
+                    f"File already exists, will not overwrite: {json_output_file}",
+                    exit_code=1,
+                )
+
         reporter = StatsReporter(stats, args.num_largest)
-        reporter.render()
+        reporter.render(json_output_file=json_output_file)
+        if json_output_file is not None:
+            print(f"Wrote {json_output_file}")
```

### Comparing `memray-1.7.0/src/memray/commands/summary.py` & `memray-1.8.0/src/memray/commands/tree.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,36 +1,32 @@
 import argparse
 import os
 from pathlib import Path
 from textwrap import dedent
 
+from rich import print as rprint
+
 from memray import FileReader
 from memray._errors import MemrayCommandError
+from memray._memray import size_fmt
 from memray.commands.common import warn_if_not_enough_symbols
-from memray.reporters.summary import SummaryReporter
+from memray.reporters.tree import TreeReporter
 
 
-class SummaryCommand:
-    """Generate a terminal-based summary report of the functions that allocate most memory"""
+class TreeCommand:
+    """Generate a tree view in the terminal for peak memory usage"""
 
     def prepare_parser(self, parser: argparse.ArgumentParser) -> None:
         parser.add_argument("results", help="Results of the tracker run")
         parser.add_argument(
-            "-s",
-            "--sort-column",
-            help="Column number to sort on",
-            type=int,
-            default=1,
-        )
-        parser.add_argument(
-            "-r",
-            "--max-rows",
-            help="Maximum number of rows to display",
+            "-b",
+            "--biggest-allocs",
+            help="Show n biggest allocations (defaults to 10)",
             type=int,
-            default=None,
+            default=10,
         )
         alloc_type_group = parser.add_mutually_exclusive_group()
         alloc_type_group.add_argument(
             "--temporary-allocation-threshold",
             metavar="N",
             help=dedent(
                 """
@@ -51,41 +47,47 @@
             help="Equivalent to --temporary-allocation-threshold=1",
             action="store_const",
             dest="temporary_allocation_threshold",
             const=1,
         )
 
     def run(self, args: argparse.Namespace, parser: argparse.ArgumentParser) -> None:
-        max_cols = SummaryReporter.N_COLUMNS
-        if args.sort_column < 1 or args.sort_column > max_cols:
-            parser.error(f"The --sort-column argument must be between 1 and {max_cols}")
-
         result_path = Path(args.results)
         if not result_path.exists() or not result_path.is_file():
             raise MemrayCommandError(f"No such file: {args.results}", exit_code=1)
 
-        reader = FileReader(os.fspath(args.results), report_progress=True)
-        if reader.metadata.has_native_traces:
-            warn_if_not_enough_symbols()
-
         try:
+            reader = FileReader(os.fspath(args.results), report_progress=True)
+            if reader.metadata.has_native_traces:
+                warn_if_not_enough_symbols()
             if args.temporary_allocation_threshold >= 0:
                 snapshot = iter(
                     reader.get_temporary_allocation_records(
                         threshold=args.temporary_allocation_threshold,
                         merge_threads=False,
                     )
                 )
             else:
                 snapshot = iter(
-                    reader.get_high_watermark_allocation_records(merge_threads=True)
+                    reader.get_high_watermark_allocation_records(merge_threads=False)
                 )
+            reporter = TreeReporter.from_snapshot(
+                snapshot,
+                biggest_allocs=args.biggest_allocs,
+                native_traces=reader.metadata.has_native_traces,
+            )
         except OSError as e:
             raise MemrayCommandError(
                 f"Failed to parse allocation records in {result_path}\nReason: {e}",
                 exit_code=1,
             )
-        reporter = SummaryReporter.from_snapshot(
-            snapshot,
-            native=reader.metadata.has_native_traces,
-        )
-        reporter.render(sort_column=args.sort_column, max_rows=args.max_rows)
+        print()
+        header = "Allocation metadata"
+        rprint(f"{header}\n{'-'*len(header)}")
+        rprint(f"Command line arguments: '{reader.metadata.command_line}'")
+        rprint(f"Peak memory size: {size_fmt(reader.metadata.peak_memory)}")
+        rprint(f"Number of allocations: {reader.metadata.total_allocations}")
+        print()
+        header = f"Biggest {args.biggest_allocs} allocations:"
+        rprint(header)
+        rprint("-" * len(header))
+        reporter.render()
```

### Comparing `memray-1.7.0/src/memray/reporters/assets/common.js` & `memray-1.8.0/src/memray/reporters/assets/common.js`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/memray/reporters/assets/common.test.js` & `memray-1.8.0/src/memray/reporters/assets/common.test.js`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/memray/reporters/assets/flamegraph.js` & `memray-1.8.0/src/memray/reporters/assets/flamegraph.js`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/memray/reporters/assets/flamegraph_common.js` & `memray-1.8.0/src/memray/reporters/assets/flamegraph_common.js`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/memray/reporters/assets/table.js` & `memray-1.8.0/src/memray/reporters/assets/table.js`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/memray/reporters/frame_tools.py` & `memray-1.8.0/src/memray/reporters/frame_tools.py`

 * *Files 5% similar despite different names*

```diff
@@ -51,29 +51,29 @@
 
     if is_candidate:
         return re.search(RE_CPYTHON_PATHS, file) is not None
     return False
 
 
 def is_cpython_internal(frame: StackFrame) -> bool:
-    symbol, file, *_ = frame
+    symbol, file, _ = frame
     return _is_cpython_internal_symbol(symbol, file)
 
 
 def is_frame_interesting(frame: StackFrame) -> bool:
-    function, file, *_ = frame
+    function, file, _ = frame
 
     if file.endswith("runpy.py"):
         return False
 
     return not _is_cpython_internal_symbol(function, file)
 
 
 def is_frame_from_import_system(frame: StackFrame) -> bool:
-    function, file, *_ = frame
+    function, file, _ = frame
     if "frozen importlib" in file:
         return True
     if function in {"import_name", "import_from", "import_all_from"} and file.endswith(
         "ceval.c"
     ):
         return True
     return False
```

### Comparing `memray-1.7.0/src/memray/reporters/stats.py` & `memray-1.8.0/src/memray/reporters/stats.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,27 @@
+import datetime
+import json
 import math
 from collections import Counter
+from dataclasses import asdict
+from pathlib import Path
+from typing import Any
 from typing import Dict
 from typing import Iterator
 from typing import List
+from typing import Optional
 from typing import Tuple
 
 import rich
 
 from memray._memray import size_fmt
 from memray._stats import Stats
 
+PythonStackElement = Tuple[str, str, int]
+
 
 def get_histogram_databins(data: Dict[int, int], bins: int) -> List[Tuple[int, int]]:
     if bins <= 0:
         raise ValueError(f"Invalid input bins={bins}, should be greater than 0")
 
     low = math.log(min(filter(None, data)))
     high = math.log(max(data))
@@ -26,14 +34,27 @@
     dist: Dict[int, int] = Counter()
     for size, count in data.items():
         bucket = min(int((math.log(size) - low) // step), bins - 1) if size else 0
         dist[bucket] += count
     return [(steps[b], dist[b]) for b in range(bins)]
 
 
+def describe_histogram_databins(
+    databins: List[Tuple[int, int]]
+) -> List[Dict[str, int]]:
+    ret: List[Dict[str, int]] = []
+    start = 0
+    for i, (end, count) in enumerate(databins):
+        # The max size for the last bucket is inclusive, not exclusive
+        adjustment = 1 if i != len(databins) - 1 else 0
+        ret.append(dict(min_bytes=start, max_bytes=end - adjustment, count=count))
+        start = end
+    return ret
+
+
 def draw_histogram(
     data: Dict[int, int], bins: int, *, hist_scale_factor: int = 25
 ) -> str:
     """
     @param data: list of allocation sizes
     @param bins: number of bins in the histogram
     @param hist_scale_factor: length of the largest bar in the histogram (# of chars)
@@ -85,68 +106,111 @@
 class StatsReporter:
     def __init__(self, stats: Stats, num_largest: int):
         self._stats = stats
         if num_largest < 1:
             raise ValueError(f"Invalid input num_largest={num_largest}, should be >=1")
         self.num_largest = num_largest
 
-    def render(self) -> None:
+    def render(self, json_output_file: Optional[Path] = None) -> None:
+        histogram_params = dict(
+            num_bins=10,
+            histogram_scale_factor=25,
+        )
+        if json_output_file:
+            self._render_to_json(histogram_params, json_output_file)
+        else:
+            self._render_to_terminal(histogram_params)
+
+    def _render_to_terminal(self, histogram_params: Dict[str, int]) -> None:
         rich.print("📏 [bold]Total allocations:[/]")
         print(f"\t{self._stats.total_num_allocations}")
 
         print()
         rich.print("📦 [bold]Total memory allocated:[/]")
         print(f"\t{size_fmt(self._stats.total_memory_allocated)}")
 
         print()
-        num_bins = 10
-        histogram_scale_factor = 25
+
         rich.print("📊 [bold]Histogram of allocation size:[/]")
         histogram = draw_histogram(
             self._stats.allocation_count_by_size,
-            num_bins,
-            hist_scale_factor=histogram_scale_factor,
+            histogram_params["num_bins"],
+            hist_scale_factor=histogram_params["histogram_scale_factor"],
         )
         print(f"\t{histogram}")
 
         print()
         rich.print("📂 [bold]Allocator type distribution:[/]")
-        for entry in self._get_allocator_type_distribution():
-            print(f"\t {entry}")
+        for allocator_name, count in self._get_allocator_type_distribution():
+            print(f"\t {allocator_name}: {count}")
 
         print()
         rich.print(
             f"🥇 [bold]Top {self.num_largest} largest allocating locations (by size):[/]"
         )
-        for entry in self._get_top_allocations_by_size():
-            print(f"\t- {entry}")
+        for location, size in self._get_top_allocations_by_size():
+            print(f"\t- {self._format_location(location)} -> {size_fmt(size)}")
 
         print()
         rich.print(
             f"🥇 [bold]Top {self.num_largest} largest allocating "
             "locations (by number of allocations):[/]"
         )
-        for entry in self._get_top_allocations_by_count():
-            print(f"\t- {entry}")
+        for location, count in self._get_top_allocations_by_count():
+            print(f"\t- {self._format_location(location)} -> {count}")
+
+    def _render_to_json(self, histogram_params: Dict[str, int], out_path: Path) -> None:
+        alloc_size_hist = describe_histogram_databins(
+            get_histogram_databins(
+                self._stats.allocation_count_by_size, bins=histogram_params["num_bins"]
+            )
+        )
+
+        metadata = asdict(self._stats.metadata)
+        for name, val in metadata.items():
+            if isinstance(val, datetime.datetime):
+                metadata[name] = str(val)
+
+        data: Dict[str, Any] = dict(
+            total_num_allocations=self._stats.total_num_allocations,
+            total_bytes_allocated=self._stats.total_memory_allocated,
+            allocation_size_histogram=alloc_size_hist,
+            allocator_type_distribution={
+                allocation_type: count
+                for allocation_type, count in self._get_allocator_type_distribution()
+            },
+            top_allocations_by_size=[
+                {"location": self._format_location(location), "size": size}
+                for location, size in self._get_top_allocations_by_size()
+            ],
+            top_allocations_by_count=[
+                {"location": self._format_location(location), "count": count}
+                for location, count in self._get_top_allocations_by_count()
+            ],
+            metadata=metadata,
+        )
+
+        with open(out_path, "w") as f:
+            json.dump(data, f, indent=2)
 
     @staticmethod
     def _format_location(loc: Tuple[str, str, int]) -> str:
         function, file, line = loc
         if function == "<unknown>":
             return "<stack trace unavailable>"
         return f"{function}:{file}:{line}"
 
-    def _get_top_allocations_by_size(self) -> Iterator[str]:
+    def _get_top_allocations_by_size(self) -> Iterator[Tuple[PythonStackElement, int]]:
         for location, size in self._stats.top_locations_by_size:
-            yield f"{self._format_location(location)} -> {size_fmt(size)}"
+            yield (location, size)
 
-    def _get_top_allocations_by_count(self) -> Iterator[str]:
+    def _get_top_allocations_by_count(self) -> Iterator[Tuple[PythonStackElement, int]]:
         for location, count in self._stats.top_locations_by_count:
-            yield f"{self._format_location(location)} -> {count}"
+            yield (location, count)
 
-    def _get_allocator_type_distribution(self) -> Iterator[str]:
+    def _get_allocator_type_distribution(self) -> Iterator[Tuple[str, int]]:
         for allocator_name, count in sorted(
             self._stats.allocation_count_by_allocator.items(),
             key=lambda item: item[1],
             reverse=True,
         ):
-            yield f"{allocator_name}: {count}"
+            yield (allocator_name, count)
```

### Comparing `memray-1.7.0/src/memray/reporters/summary.py` & `memray-1.8.0/src/memray/reporters/summary.py`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/memray/reporters/table.py` & `memray-1.8.0/src/memray/reporters/table.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import html
 from typing import Any
 from typing import Dict
 from typing import Iterable
-from typing import Iterator
 from typing import List
 from typing import TextIO
 
 from memray import AllocationRecord
 from memray import AllocatorType
 from memray import MemorySnapshot
 from memray import Metadata
@@ -23,15 +22,15 @@
         super().__init__()
         self.data = data
         self.memory_records = memory_records
 
     @classmethod
     def from_snapshot(
         cls,
-        allocations: Iterator[AllocationRecord],
+        allocations: Iterable[AllocationRecord],
         *,
         memory_records: Iterable[MemorySnapshot],
         native_traces: bool,
     ) -> "TableReporter":
         result = []
         for record in allocations:
             stack_trace = (
@@ -58,17 +57,20 @@
         return cls(result, memory_records=memory_records)
 
     def render(
         self,
         outfile: TextIO,
         metadata: Metadata,
         show_memory_leaks: bool,
+        merge_threads: bool,
     ) -> None:
+        if not merge_threads:
+            raise NotImplementedError("TableReporter only supports merged threads.")
         html_code = render_report(
             kind="table",
             data=self.data,
             metadata=metadata,
             memory_records=self.memory_records,
             show_memory_leaks=show_memory_leaks,
-            merge_threads=True,
+            merge_threads=merge_threads,
         )
         print(html_code, file=outfile)
```

### Comparing `memray-1.7.0/src/memray/reporters/templates/__init__.py` & `memray-1.8.0/src/memray/reporters/templates/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,17 +34,18 @@
     memory_records: Iterable[MemorySnapshot],
     show_memory_leaks: bool,
     merge_threads: bool,
 ) -> str:
     env = get_render_environment()
     template = env.get_template(kind + ".html")
 
-    title = get_report_title(kind=kind, show_memory_leaks=show_memory_leaks)
+    pretty_kind = kind.replace("_", " ")
+    title = get_report_title(kind=pretty_kind, show_memory_leaks=show_memory_leaks)
     return template.render(
-        kind=kind,
+        kind=pretty_kind,
         title=title,
         data=data,
         metadata=metadata,
         memory_records=memory_records,
         show_memory_leaks=show_memory_leaks,
         merge_threads=merge_threads,
     )
```

### Comparing `memray-1.7.0/src/memray/reporters/templates/assets/flamegraph.js` & `memray-1.8.0/src/memray/reporters/templates/assets/flamegraph.js`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/memray/reporters/templates/assets/flamegraph_common.js` & `memray-1.8.0/src/memray/reporters/templates/assets/flamegraph_common.js`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/memray/reporters/templates/assets/table.js` & `memray-1.8.0/src/memray/reporters/templates/assets/table.js`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/memray/reporters/templates/base.html` & `memray-1.8.0/src/memray/reporters/templates/base.html`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/memray/reporters/templates/classic_base.html` & `memray-1.8.0/src/memray/reporters/templates/classic_base.html`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/memray/reporters/templates/flamegraph.html` & `memray-1.8.0/src/memray/reporters/templates/flamegraph.html`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
   </button>
   <div class="dropdown-menu" aria-labelledby="threadsDropdownButton" id="threadsDropdownList">
     <a class="dropdown-item" data-thread="-0x1" id="resetThreadFilterItem">Reset</a>
   </div>
 </div>
 <div class="form-check mr-3">
   <input class="form-check-input" type="checkbox" data-toggle="tooltip" id="hideUninteresting"
-          title="Hide CPython eval frames and other, memray-related frames" checked>
+          title="Hide CPython eval frames and Memray-related frames" checked>
     <label class="form-check-label text-white bg-dark">Hide Irrelevant Frames</label>
 </div>
 <div class="form-check mr-3">
   <input class="form-check-input" type="checkbox" data-toggle="tooltip" id="hideImportSystem"
           title="Hide frames related to the Python import system" >
     <label class="form-check-label text-white bg-dark">Hide Import System Frames</label>
 </div>
@@ -40,14 +40,16 @@
   Note that the Python allocator doesn't necessarily release memory to the system when Python objects are deallocated and these can still appear as "leaks". If you want to exclude these, you can run your application with the `PYTHONMALLOC=malloc` environment variable set.
 </div>
 {% else %}
 <p>
   The flame graph displays a snapshot of memory used across stack frames at the time <b>when the memory usage was at its peak</b>.
 </p>
 {% endif %}
+{% block slider_help %}
+{% endblock %}
 <p>
   The vertical ordering of the stack frames corresponds to the order of function calls, from parent to children.
   The horizontal ordering does not represent the passage of time in the application: they simply represent child frames in arbitrary order.
 </p>
 <p>
   On the flame graph, each bar represents a stack frame and shows the code which triggered the memory allocation.
   Hovering over the frame you can also see the overall memory allocated in the given frame and its children and the number of times allocations have occurred.
@@ -68,11 +70,15 @@
 
 {% block scripts %}
 {{ super() }}
 <script src="https://d3js.org/d3.v4.min.js" charset="utf-8"></script>
 <script src="https://d3js.org/d3-scale-chromatic.v1.min.js"></script>
 <script src="https://cdn.jsdelivr.net/npm/d3-tip@0.9.1/dist/index.min.js"></script>
 <script src="https://cdn.jsdelivr.net/npm/d3-flame-graph@4.0.6/dist/d3-flamegraph.min.js"></script>
+
+{% block flamegraph_script %}
 <script type="text/javascript">
   {%- include "assets/flamegraph.js" -%}
 </script>
 {% endblock %}
+
+{% endblock %}
```

#### html2text {}

```diff
@@ -10,15 +10,15 @@
 Note that the Python allocator doesn't necessarily release memory to the system
 when Python objects are deallocated and these can still appear as "leaks". If
 you want to exclude these, you can run your application with the
 `PYTHONMALLOC=malloc` environment variable set.
 {% else %}
 The flame graph displays a snapshot of memory used across stack frames at the
 time when the memory usage was at its peak.
-{% endif %}
+{% endif %} {% block slider_help %} {% endblock %}
 The vertical ordering of the stack frames corresponds to the order of function
 calls, from parent to children. The horizontal ordering does not represent the
 passage of time in the application: they simply represent child frames in
 arbitrary order.
 On the flame graph, each bar represents a stack frame and shows the code which
 triggered the memory allocation. Hovering over the frame you can also see the
 overall memory allocated in the given frame and its children and the number of
@@ -26,8 +26,9 @@
 The Show/Hide Irrelevant Frames button can be used to reveal and hide frames
 which contain allocations in code which might not be relevant for the
 application. These include frames in the CPython eval loop as well as frames
 introduced by memray during the analysis.
 You can find more information in the documentation.
 {% endblock %} {% block styles %} {{ super() }}
  {% endblock %} {% block scripts %} {{ super() }}
- {% endblock %}
+ {% block flamegraph_script %}
+ {% endblock %} {% endblock %}
```

### Comparing `memray-1.7.0/src/memray/reporters/templates/table.html` & `memray-1.8.0/src/memray/reporters/templates/table.html`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/memray/reporters/transform.py` & `memray-1.8.0/src/memray/reporters/transform.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import csv
 import json
 from typing import Any
 from typing import Dict
 from typing import Iterable
-from typing import Iterator
 from typing import List
 from typing import TextIO
 from typing import Tuple
 
 from memray import AllocationRecord
 from memray import AllocatorType
 from memray import MemorySnapshot
@@ -20,15 +19,15 @@
     SUFFIX_MAP = {
         "gprof2dot": ".json",
         "csv": ".csv",
     }
 
     def __init__(
         self,
-        allocations: Iterator[AllocationRecord],
+        allocations: Iterable[AllocationRecord],
         *,
         format: str,
         native_traces: bool,
         memory_records: Iterable[MemorySnapshot],
     ) -> None:
         super().__init__()
         self.allocations = allocations
@@ -73,15 +72,18 @@
         json.dump(result, outfile)
 
     def render(
         self,
         outfile: TextIO,
         metadata: Metadata,
         show_memory_leaks: bool,
+        merge_threads: bool,
     ) -> None:
+        if not merge_threads:
+            raise NotImplementedError("TransformReporter only supports merged threads.")
         renderer = getattr(self, f"render_as_{self.format}")
         renderer(outfile, metadata=metadata, show_memory_leaks=show_memory_leaks)
 
     def render_as_csv(
         self,
         outfile: TextIO,
         **kwargs: Any,
```

### Comparing `memray-1.7.0/src/memray/reporters/tree.py` & `memray-1.8.0/src/memray/reporters/tree.py`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/memray/reporters/tui.py` & `memray-1.8.0/src/memray/reporters/tui.py`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/memray.egg-info/PKG-INFO` & `memray-1.8.0/src/memray.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: memray
-Version: 1.7.0
+Version: 1.8.0
 Summary: A memory profiler for Python applications
 Home-page: https://github.com/bloomberg/memray
 Author: Pablo Galindo Salgado
 License: Apache 2.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
@@ -111,27 +111,41 @@
 ```shell
 export CFLAGS="-I$(brew --prefix lz4)/include" LDFLAGS="-L$(brew --prefix lz4)/lib -Wl,-rpath,$(brew --prefix lz4)/lib"
 ```
 
 before installing `memray`. Check the documentation of your package manager to know the location of the header and library
 files for more detailed information.
 
+If you are building on MacOS, you will also need to set the deployment target.
+
+```shell
+export MACOSX_DEPLOYMENT_TARGET=10.14
+```
+
 Once you have the binary dependencies installed, you can clone the repository and follow with the normal building process:
 
 ```shell
 git clone git@github.com:bloomberg/memray.git memray
 cd memray
 python3 -m venv ../memray-env/  # just an example, put this wherever you want
 source ../memray-env/bin/activate
 python3 -m pip install --upgrade pip
 python3 -m pip install -e . -r requirements-test.txt -r requirements-extra.txt
 ```
 
 This will install Memray in the virtual environment in development mode (the `-e` of the last `pip install` command).
 
+If you plan to contribute back, you should install the pre-commit hooks:
+
+```shell
+pre-commit install
+```
+
+This will ensure that your contribution passes our linting checks.
+
 # Documentation
 
 You can find the latest documentation available [here](https://bloomberg.github.io/memray/).
 
 # Usage
 
 There are many ways to use Memray. The easiest way is to use it as a command line tool to run your script, application, or library.
@@ -336,20 +350,20 @@
 
 We welcome your contributions to help us improve and extend this project!
 
 Below you will find some basic steps required to be able to contribute to the project. If you have any questions about this process or any other aspect of contributing to a Bloomberg open source project, feel free to send an email to opensource@bloomberg.net and we'll get your questions answered as quickly as we can.
 
 ## Contribution Licensing
 
-Since this project is distributed under the terms of an [open source license](LICENSE), contributions that you make
-are licensed under the same terms. In order for us to be able to accept your contributions,
+Since this project is distributed under the terms of an [open source license](LICENSE), contributions that
+you make are licensed under the same terms. In order for us to be able to accept your contributions,
 we will need explicit confirmation from you that you are able and willing to provide them under
 these terms, and the mechanism we use to do this is called a Developer's Certificate of Origin
-[(DCO)](https://github.com/bloomberg/.github/blob/main/DCO.md). This is very similar to the process used by the Linux(R) kernel, Samba, and many
-other major open source projects.
+[(DCO)](https://github.com/bloomberg/.github/blob/main/DCO.md). This is very similar to the process
+used by the Linux kernel, Samba, and many other major open source projects.
 
 To participate under these terms, all that you must do is include a line like the following as the
 last line of the commit message for each commit in your contribution:
 
     Signed-Off-By: Random J. Developer <random@developer.example.org>
 
 The simplest way to accomplish this is to add `-s` or `--signoff` to your `git commit` command.
```

### Comparing `memray-1.7.0/src/memray.egg-info/SOURCES.txt` & `memray-1.8.0/src/memray.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 .babelrc
 .bumpversion.cfg
+.pre-commit-config.yaml
 LICENSE
 MANIFEST.in
 Makefile
 NEWS.rst
 README.md
 package-lock.json
 package.json
 pyproject.toml
-setup.cfg
 setup.py
 webpack.config.js
 src/memray/__init__.py
 src/memray/__init__.pyi
 src/memray/__main__.py
 src/memray/_destination.py
 src/memray/_errors.py
@@ -111,24 +111,27 @@
 src/memray/reporters/tui.py
 src/memray/reporters/assets/__init__.py
 src/memray/reporters/assets/common.js
 src/memray/reporters/assets/common.test.js
 src/memray/reporters/assets/flamegraph.js
 src/memray/reporters/assets/flamegraph_common.js
 src/memray/reporters/assets/table.js
+src/memray/reporters/assets/temporal_flamegraph.js
 src/memray/reporters/templates/__init__.py
 src/memray/reporters/templates/base.html
 src/memray/reporters/templates/classic_base.html
 src/memray/reporters/templates/flamegraph.html
 src/memray/reporters/templates/table.html
+src/memray/reporters/templates/temporal_flamegraph.html
 src/memray/reporters/templates/assets/flamegraph.css
 src/memray/reporters/templates/assets/flamegraph.js
 src/memray/reporters/templates/assets/flamegraph_common.js
 src/memray/reporters/templates/assets/table.css
 src/memray/reporters/templates/assets/table.js
+src/memray/reporters/templates/assets/temporal_flamegraph.js
 src/vendor/libbacktrace_2446c66076480ce07a6bd868badcbceb3eeecc2e_debuginfod_patch.diff
 src/vendor/libbacktrace_2446c66076480ce07a6bd868badcbceb3eeecc2e_patch.diff
 src/vendor/regenerate_libbacktrace.sh
 src/vendor/libbacktrace/.gitignore
 src/vendor/libbacktrace/Isaac.Newton-Opticks.txt
 src/vendor/libbacktrace/LICENSE
 src/vendor/libbacktrace/Makefile.am
```

### Comparing `memray-1.7.0/src/vendor/libbacktrace/Isaac.Newton-Opticks.txt` & `memray-1.8.0/src/vendor/libbacktrace/Isaac.Newton-Opticks.txt`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/vendor/libbacktrace/LICENSE` & `memray-1.8.0/src/vendor/libbacktrace/LICENSE`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/vendor/libbacktrace/Makefile.am` & `memray-1.8.0/src/vendor/libbacktrace/Makefile.am`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/vendor/libbacktrace/Makefile.in` & `memray-1.8.0/src/vendor/libbacktrace/Makefile.in`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/vendor/libbacktrace/README.md` & `memray-1.8.0/src/vendor/libbacktrace/README.md`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/vendor/libbacktrace/aclocal.m4` & `memray-1.8.0/src/vendor/libbacktrace/aclocal.m4`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/vendor/libbacktrace/alloc.c` & `memray-1.8.0/src/vendor/libbacktrace/alloc.c`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/vendor/libbacktrace/allocfail.c` & `memray-1.8.0/src/vendor/libbacktrace/allocfail.c`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/vendor/libbacktrace/allocfail.sh` & `memray-1.8.0/src/vendor/libbacktrace/allocfail.sh`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/vendor/libbacktrace/atomic.c` & `memray-1.8.0/src/vendor/libbacktrace/atomic.c`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/vendor/libbacktrace/backtrace-supported.h.in` & `memray-1.8.0/src/vendor/libbacktrace/backtrace-supported.h.in`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/vendor/libbacktrace/backtrace.c` & `memray-1.8.0/src/vendor/libbacktrace/backtrace.c`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/vendor/libbacktrace/backtrace.h` & `memray-1.8.0/src/vendor/libbacktrace/backtrace.h`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/vendor/libbacktrace/btest.c` & `memray-1.8.0/src/vendor/libbacktrace/btest.c`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/vendor/libbacktrace/compile` & `memray-1.8.0/src/vendor/libbacktrace/compile`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/vendor/libbacktrace/config/enable.m4` & `memray-1.8.0/src/vendor/libbacktrace/config/enable.m4`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/vendor/libbacktrace/config/lead-dot.m4` & `memray-1.8.0/src/vendor/libbacktrace/config/lead-dot.m4`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/vendor/libbacktrace/config/libtool.m4` & `memray-1.8.0/src/vendor/libbacktrace/config/libtool.m4`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/vendor/libbacktrace/config/ltoptions.m4` & `memray-1.8.0/src/vendor/libbacktrace/config/ltoptions.m4`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/vendor/libbacktrace/config/ltsugar.m4` & `memray-1.8.0/src/vendor/libbacktrace/config/ltsugar.m4`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/vendor/libbacktrace/config/ltversion.m4` & `memray-1.8.0/src/vendor/libbacktrace/config/ltversion.m4`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/vendor/libbacktrace/config/lt~obsolete.m4` & `memray-1.8.0/src/vendor/libbacktrace/config/lt~obsolete.m4`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/vendor/libbacktrace/config/multi.m4` & `memray-1.8.0/src/vendor/libbacktrace/config/multi.m4`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/vendor/libbacktrace/config/override.m4` & `memray-1.8.0/src/vendor/libbacktrace/config/override.m4`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/vendor/libbacktrace/config/unwind_ipinfo.m4` & `memray-1.8.0/src/vendor/libbacktrace/config/unwind_ipinfo.m4`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/vendor/libbacktrace/config/warnings.m4` & `memray-1.8.0/src/vendor/libbacktrace/config/warnings.m4`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/vendor/libbacktrace/config.guess` & `memray-1.8.0/src/vendor/libbacktrace/config.guess`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/vendor/libbacktrace/config.h.in` & `memray-1.8.0/src/vendor/libbacktrace/config.h.in`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/vendor/libbacktrace/config.sub` & `memray-1.8.0/src/vendor/libbacktrace/config.sub`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/vendor/libbacktrace/configure` & `memray-1.8.0/src/vendor/libbacktrace/configure`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/vendor/libbacktrace/configure.ac` & `memray-1.8.0/src/vendor/libbacktrace/configure.ac`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/vendor/libbacktrace/debuginfod_support.h` & `memray-1.8.0/src/vendor/libbacktrace/debuginfod_support.h`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/vendor/libbacktrace/dwarf.c` & `memray-1.8.0/src/vendor/libbacktrace/dwarf.c`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/vendor/libbacktrace/edtest.c` & `memray-1.8.0/src/vendor/libbacktrace/edtest.c`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/vendor/libbacktrace/edtest2.c` & `memray-1.8.0/src/vendor/libbacktrace/edtest2.c`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/vendor/libbacktrace/elf.c` & `memray-1.8.0/src/vendor/libbacktrace/elf.c`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/vendor/libbacktrace/fileline.c` & `memray-1.8.0/src/vendor/libbacktrace/fileline.c`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/vendor/libbacktrace/filenames.h` & `memray-1.8.0/src/vendor/libbacktrace/filenames.h`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/vendor/libbacktrace/filetype.awk` & `memray-1.8.0/src/vendor/libbacktrace/filetype.awk`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/vendor/libbacktrace/install-debuginfo-for-buildid.sh.in` & `memray-1.8.0/src/vendor/libbacktrace/install-debuginfo-for-buildid.sh.in`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/vendor/libbacktrace/install-sh` & `memray-1.8.0/src/vendor/libbacktrace/install-sh`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/vendor/libbacktrace/instrumented_alloc.c` & `memray-1.8.0/src/vendor/libbacktrace/instrumented_alloc.c`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/vendor/libbacktrace/internal.h` & `memray-1.8.0/src/vendor/libbacktrace/internal.h`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/vendor/libbacktrace/libtool.m4` & `memray-1.8.0/src/vendor/libbacktrace/libtool.m4`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/vendor/libbacktrace/ltmain.sh` & `memray-1.8.0/src/vendor/libbacktrace/ltmain.sh`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/vendor/libbacktrace/ltoptions.m4` & `memray-1.8.0/src/vendor/libbacktrace/ltoptions.m4`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/vendor/libbacktrace/ltsugar.m4` & `memray-1.8.0/src/vendor/libbacktrace/ltsugar.m4`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/vendor/libbacktrace/ltversion.m4` & `memray-1.8.0/src/vendor/libbacktrace/ltversion.m4`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/vendor/libbacktrace/lt~obsolete.m4` & `memray-1.8.0/src/vendor/libbacktrace/lt~obsolete.m4`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/vendor/libbacktrace/macho.c` & `memray-1.8.0/src/vendor/libbacktrace/macho.c`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/vendor/libbacktrace/missing` & `memray-1.8.0/src/vendor/libbacktrace/missing`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/vendor/libbacktrace/mmap.c` & `memray-1.8.0/src/vendor/libbacktrace/mmap.c`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/vendor/libbacktrace/mmapio.c` & `memray-1.8.0/src/vendor/libbacktrace/mmapio.c`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/vendor/libbacktrace/move-if-change` & `memray-1.8.0/src/vendor/libbacktrace/move-if-change`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/vendor/libbacktrace/mtest.c` & `memray-1.8.0/src/vendor/libbacktrace/mtest.c`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/vendor/libbacktrace/nounwind.c` & `memray-1.8.0/src/vendor/libbacktrace/nounwind.c`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/vendor/libbacktrace/pecoff.c` & `memray-1.8.0/src/vendor/libbacktrace/pecoff.c`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/vendor/libbacktrace/posix.c` & `memray-1.8.0/src/vendor/libbacktrace/posix.c`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/vendor/libbacktrace/print.c` & `memray-1.8.0/src/vendor/libbacktrace/print.c`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/vendor/libbacktrace/read.c` & `memray-1.8.0/src/vendor/libbacktrace/read.c`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/vendor/libbacktrace/simple.c` & `memray-1.8.0/src/vendor/libbacktrace/simple.c`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/vendor/libbacktrace/sort.c` & `memray-1.8.0/src/vendor/libbacktrace/sort.c`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/vendor/libbacktrace/state.c` & `memray-1.8.0/src/vendor/libbacktrace/state.c`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/vendor/libbacktrace/stest.c` & `memray-1.8.0/src/vendor/libbacktrace/stest.c`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/vendor/libbacktrace/test-driver` & `memray-1.8.0/src/vendor/libbacktrace/test-driver`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/vendor/libbacktrace/test_format.c` & `memray-1.8.0/src/vendor/libbacktrace/test_format.c`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/vendor/libbacktrace/testlib.c` & `memray-1.8.0/src/vendor/libbacktrace/testlib.c`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/vendor/libbacktrace/testlib.h` & `memray-1.8.0/src/vendor/libbacktrace/testlib.h`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/vendor/libbacktrace/ttest.c` & `memray-1.8.0/src/vendor/libbacktrace/ttest.c`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/vendor/libbacktrace/unittest.c` & `memray-1.8.0/src/vendor/libbacktrace/unittest.c`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/vendor/libbacktrace/unknown.c` & `memray-1.8.0/src/vendor/libbacktrace/unknown.c`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/vendor/libbacktrace/xcoff.c` & `memray-1.8.0/src/vendor/libbacktrace/xcoff.c`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/vendor/libbacktrace/xztest.c` & `memray-1.8.0/src/vendor/libbacktrace/xztest.c`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/vendor/libbacktrace/ztest.c` & `memray-1.8.0/src/vendor/libbacktrace/ztest.c`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/vendor/libbacktrace_2446c66076480ce07a6bd868badcbceb3eeecc2e_debuginfod_patch.diff` & `memray-1.8.0/src/vendor/libbacktrace_2446c66076480ce07a6bd868badcbceb3eeecc2e_debuginfod_patch.diff`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/vendor/libbacktrace_2446c66076480ce07a6bd868badcbceb3eeecc2e_patch.diff` & `memray-1.8.0/src/vendor/libbacktrace_2446c66076480ce07a6bd868badcbceb3eeecc2e_patch.diff`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/src/vendor/regenerate_libbacktrace.sh` & `memray-1.8.0/src/vendor/regenerate_libbacktrace.sh`

 * *Files identical despite different names*

### Comparing `memray-1.7.0/webpack.config.js` & `memray-1.8.0/webpack.config.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -2,14 +2,15 @@
 const TerserPlugin = require("terser-webpack-plugin");
 
 module.exports = {
     mode: "production",
     entry: {
         flamegraph_common: "./src/memray/reporters/assets/flamegraph_common.js",
         flamegraph: "./src/memray/reporters/assets/flamegraph.js",
+        temporal_flamegraph: "./src/memray/reporters/assets/temporal_flamegraph.js",
         table: "./src/memray/reporters/assets/table.js",
     },
     output: {
         path: path.resolve("src/memray/reporters/templates/assets"),
         filename: "[name].js",
     },
     externals: {
```

