# Comparing `tmp/pcvs-0.6.0.tar.gz` & `tmp/pcvs-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pcvs-0.6.0.tar", last modified: Fri Sep 16 08:37:08 2022, max compression
+gzip compressed data, was "/home/adamj/.lnk/code/pcvs-stable/dist/.tmp-zrs668ab/pcvs-0.7.0.tar", last modified: Fri Jun  9 10:15:05 2023, max compression
```

## Comparing `pcvs-0.6.0.tar` & `pcvs-0.7.0.tar`

### file list

```diff
@@ -1,163 +1,168 @@
-drwxr-xr-x   0 adamj     (1000) adamj     (1000)        0 2022-09-16 08:37:08.865061 pcvs-0.6.0/
--rw-r--r--   0 adamj     (1000) adamj     (1000)      617 2022-09-16 08:17:01.000000 pcvs-0.6.0/AUTHORS
--rw-r--r--   0 adamj     (1000) adamj     (1000)      436 2022-09-16 08:17:01.000000 pcvs-0.6.0/CHANGES
--rw-r--r--   0 adamj     (1000) adamj     (1000)    21865 2022-09-16 08:17:01.000000 pcvs-0.6.0/COPYING
--rw-r--r--   0 adamj     (1000) adamj     (1000)      363 2022-09-16 08:17:01.000000 pcvs-0.6.0/MANIFEST.in
--rw-r--r--   0 adamj     (1000) adamj     (1000)     3380 2022-09-16 08:37:08.865061 pcvs-0.6.0/PKG-INFO
--rw-r--r--   0 adamj     (1000) adamj     (1000)     2790 2022-09-16 08:23:16.000000 pcvs-0.6.0/README.md
-drwxr-xr-x   0 adamj     (1000) adamj     (1000)        0 2022-09-16 08:37:08.853061 pcvs-0.6.0/pcvs/
--rw-r--r--   0 adamj     (1000) adamj     (1000)      442 2022-09-16 08:17:01.000000 pcvs-0.6.0/pcvs/__init__.py
-drwxr-xr-x   0 adamj     (1000) adamj     (1000)        0 2022-09-16 08:37:08.853061 pcvs-0.6.0/pcvs/backend/
--rw-r--r--   0 adamj     (1000) adamj     (1000)        0 2022-09-16 08:17:01.000000 pcvs-0.6.0/pcvs/backend/__init__.py
--rw-r--r--   0 adamj     (1000) adamj     (1000)    11206 2022-09-16 08:17:01.000000 pcvs-0.6.0/pcvs/backend/bank.py
--rw-r--r--   0 adamj     (1000) adamj     (1000)    13271 2022-09-16 08:17:01.000000 pcvs-0.6.0/pcvs/backend/config.py
--rw-r--r--   0 adamj     (1000) adamj     (1000)    15064 2022-09-16 08:17:01.000000 pcvs-0.6.0/pcvs/backend/profile.py
--rw-r--r--   0 adamj     (1000) adamj     (1000)     2942 2022-09-16 08:17:01.000000 pcvs-0.6.0/pcvs/backend/report.py
--rw-r--r--   0 adamj     (1000) adamj     (1000)    26272 2022-09-16 08:17:01.000000 pcvs-0.6.0/pcvs/backend/run.py
--rw-r--r--   0 adamj     (1000) adamj     (1000)    13640 2022-09-16 08:17:01.000000 pcvs-0.6.0/pcvs/backend/session.py
--rw-r--r--   0 adamj     (1000) adamj     (1000)     1423 2022-09-16 08:17:01.000000 pcvs-0.6.0/pcvs/backend/spack.py
--rw-r--r--   0 adamj     (1000) adamj     (1000)    13981 2022-09-16 08:17:01.000000 pcvs-0.6.0/pcvs/backend/utilities.py
-drwxr-xr-x   0 adamj     (1000) adamj     (1000)        0 2022-09-16 08:37:08.857061 pcvs-0.6.0/pcvs/cli/
--rw-r--r--   0 adamj     (1000) adamj     (1000)        0 2022-09-16 08:17:01.000000 pcvs-0.6.0/pcvs/cli/__init__.py
--rw-r--r--   0 adamj     (1000) adamj     (1000)     5904 2022-09-16 08:17:01.000000 pcvs-0.6.0/pcvs/cli/cli_bank.py
--rw-r--r--   0 adamj     (1000) adamj     (1000)    12503 2022-09-16 08:17:01.000000 pcvs-0.6.0/pcvs/cli/cli_config.py
--rw-r--r--   0 adamj     (1000) adamj     (1000)      943 2022-09-16 08:17:01.000000 pcvs-0.6.0/pcvs/cli/cli_plumbing.py
--rw-r--r--   0 adamj     (1000) adamj     (1000)    16151 2022-09-16 08:17:01.000000 pcvs-0.6.0/pcvs/cli/cli_profile.py
--rw-r--r--   0 adamj     (1000) adamj     (1000)     2377 2022-09-16 08:17:01.000000 pcvs-0.6.0/pcvs/cli/cli_report.py
--rw-r--r--   0 adamj     (1000) adamj     (1000)    11815 2022-09-16 08:17:01.000000 pcvs-0.6.0/pcvs/cli/cli_run.py
--rw-r--r--   0 adamj     (1000) adamj     (1000)     3407 2022-09-16 08:17:01.000000 pcvs-0.6.0/pcvs/cli/cli_session.py
--rw-r--r--   0 adamj     (1000) adamj     (1000)     9396 2022-09-16 08:17:01.000000 pcvs-0.6.0/pcvs/cli/cli_utilities.py
-drwxr-xr-x   0 adamj     (1000) adamj     (1000)        0 2022-09-16 08:37:08.857061 pcvs-0.6.0/pcvs/converter/
--rw-r--r--   0 adamj     (1000) adamj     (1000)        0 2022-09-16 08:17:01.000000 pcvs-0.6.0/pcvs/converter/__init__.py
--rwxr-xr-x   0 adamj     (1000) adamj     (1000)    13075 2022-09-16 08:17:01.000000 pcvs-0.6.0/pcvs/converter/yaml_converter.py
-drwxr-xr-x   0 adamj     (1000) adamj     (1000)        0 2022-09-16 08:37:08.857061 pcvs-0.6.0/pcvs/dsl/
--rw-r--r--   0 adamj     (1000) adamj     (1000)     7875 2022-09-16 08:17:01.000000 pcvs-0.6.0/pcvs/dsl/__init__.py
--rw-r--r--   0 adamj     (1000) adamj     (1000)     2298 2022-09-16 08:17:01.000000 pcvs-0.6.0/pcvs/dsl/analysis.py
--rw-r--r--   0 adamj     (1000) adamj     (1000)      960 2022-09-16 08:17:22.000000 pcvs-0.6.0/pcvs/dsl/render.py
-drwxr-xr-x   0 adamj     (1000) adamj     (1000)        0 2022-09-16 08:37:08.857061 pcvs-0.6.0/pcvs/helpers/
--rw-r--r--   0 adamj     (1000) adamj     (1000)        0 2022-09-16 08:17:01.000000 pcvs-0.6.0/pcvs/helpers/__init__.py
--rw-r--r--   0 adamj     (1000) adamj     (1000)     2538 2022-09-16 08:17:01.000000 pcvs-0.6.0/pcvs/helpers/communications.py
--rw-r--r--   0 adamj     (1000) adamj     (1000)    16678 2022-09-16 08:17:01.000000 pcvs-0.6.0/pcvs/helpers/criterion.py
--rw-r--r--   0 adamj     (1000) adamj     (1000)     7928 2022-09-16 08:17:01.000000 pcvs-0.6.0/pcvs/helpers/exceptions.py
--rw-r--r--   0 adamj     (1000) adamj     (1000)    28185 2022-09-16 08:17:01.000000 pcvs-0.6.0/pcvs/helpers/git.py
--rw-r--r--   0 adamj     (1000) adamj     (1000)    22703 2022-09-16 08:17:01.000000 pcvs-0.6.0/pcvs/helpers/log.py
--rw-r--r--   0 adamj     (1000) adamj     (1000)     3119 2022-09-16 08:17:01.000000 pcvs-0.6.0/pcvs/helpers/pm.py
--rw-r--r--   0 adamj     (1000) adamj     (1000)    15595 2022-09-16 08:17:01.000000 pcvs-0.6.0/pcvs/helpers/system.py
--rw-r--r--   0 adamj     (1000) adamj     (1000)    13197 2022-09-16 08:17:01.000000 pcvs-0.6.0/pcvs/helpers/utils.py
--rw-r--r--   0 adamj     (1000) adamj     (1000)     3919 2022-09-16 08:17:01.000000 pcvs-0.6.0/pcvs/main.py
-drwxr-xr-x   0 adamj     (1000) adamj     (1000)        0 2022-09-16 08:37:08.857061 pcvs-0.6.0/pcvs/orchestration/
--rw-r--r--   0 adamj     (1000) adamj     (1000)     6069 2022-09-16 08:17:01.000000 pcvs-0.6.0/pcvs/orchestration/__init__.py
--rw-r--r--   0 adamj     (1000) adamj     (1000)      102 2022-09-16 08:17:01.000000 pcvs-0.6.0/pcvs/orchestration/__main__.py
--rw-r--r--   0 adamj     (1000) adamj     (1000)    10332 2022-09-16 08:17:01.000000 pcvs-0.6.0/pcvs/orchestration/manager.py
--rw-r--r--   0 adamj     (1000) adamj     (1000)     3248 2022-09-16 08:17:22.000000 pcvs-0.6.0/pcvs/orchestration/publishers.py
--rw-r--r--   0 adamj     (1000) adamj     (1000)     5364 2022-09-16 08:17:01.000000 pcvs-0.6.0/pcvs/orchestration/set.py
-drwxr-xr-x   0 adamj     (1000) adamj     (1000)        0 2022-09-16 08:37:08.857061 pcvs-0.6.0/pcvs/plugins/
--rw-r--r--   0 adamj     (1000) adamj     (1000)     8058 2022-09-16 08:17:22.000000 pcvs-0.6.0/pcvs/plugins/__init__.py
-drwxr-xr-x   0 adamj     (1000) adamj     (1000)        0 2022-09-16 08:37:08.857061 pcvs-0.6.0/pcvs/plugins/default/
--rw-r--r--   0 adamj     (1000) adamj     (1000)        0 2022-09-16 08:17:01.000000 pcvs-0.6.0/pcvs/plugins/default/__init__.py
--rw-r--r--   0 adamj     (1000) adamj     (1000)     2003 2022-09-16 08:17:01.000000 pcvs-0.6.0/pcvs/plugins/default/validation.py
-drwxr-xr-x   0 adamj     (1000) adamj     (1000)        0 2022-09-16 08:37:08.857061 pcvs-0.6.0/pcvs/schemes/
--rw-r--r--   0 adamj     (1000) adamj     (1000)      699 2022-09-16 08:17:01.000000 pcvs-0.6.0/pcvs/schemes/compiler-scheme.yml
--rw-r--r--   0 adamj     (1000) adamj     (1000)      401 2022-09-16 08:17:01.000000 pcvs-0.6.0/pcvs/schemes/criterion-scheme.yml
--rw-r--r--   0 adamj     (1000) adamj     (1000)     5092 2022-09-16 08:17:01.000000 pcvs-0.6.0/pcvs/schemes/group-scheme.yml
--rw-r--r--   0 adamj     (1000) adamj     (1000)     1127 2022-09-16 08:17:01.000000 pcvs-0.6.0/pcvs/schemes/machine-scheme.yml
--rw-r--r--   0 adamj     (1000) adamj     (1000)      972 2022-09-16 08:17:01.000000 pcvs-0.6.0/pcvs/schemes/runtime-scheme.yml
--rw-r--r--   0 adamj     (1000) adamj     (1000)      919 2022-09-16 08:17:01.000000 pcvs-0.6.0/pcvs/schemes/settings-scheme.yml
--rw-r--r--   0 adamj     (1000) adamj     (1000)     6122 2022-09-16 08:17:01.000000 pcvs-0.6.0/pcvs/schemes/te-scheme.yml
--rw-r--r--   0 adamj     (1000) adamj     (1000)     1300 2022-09-16 08:17:01.000000 pcvs-0.6.0/pcvs/schemes/test-result-scheme.yml
--rw-r--r--   0 adamj     (1000) adamj     (1000)      728 2022-09-16 08:17:01.000000 pcvs-0.6.0/pcvs/schemes/validation-scheme.yml
-drwxr-xr-x   0 adamj     (1000) adamj     (1000)        0 2022-09-16 08:37:08.853061 pcvs-0.6.0/pcvs/templates/
-drwxr-xr-x   0 adamj     (1000) adamj     (1000)        0 2022-09-16 08:37:08.857061 pcvs-0.6.0/pcvs/templates/config/
--rw-r--r--   0 adamj     (1000) adamj     (1000)      874 2022-09-16 08:17:01.000000 pcvs-0.6.0/pcvs/templates/config/compiler.default.yml
--rw-r--r--   0 adamj     (1000) adamj     (1000)      493 2022-09-16 08:17:01.000000 pcvs-0.6.0/pcvs/templates/config/compiler.gcc.yml
--rw-r--r--   0 adamj     (1000) adamj     (1000)      484 2022-09-16 08:17:01.000000 pcvs-0.6.0/pcvs/templates/config/compiler.icc.yml
--rw-r--r--   0 adamj     (1000) adamj     (1000)      874 2022-09-16 08:17:01.000000 pcvs-0.6.0/pcvs/templates/config/compiler.mpi.yml
--rw-r--r--   0 adamj     (1000) adamj     (1000)     2182 2022-09-16 08:17:01.000000 pcvs-0.6.0/pcvs/templates/config/criterion.default.yml
--rw-r--r--   0 adamj     (1000) adamj     (1000)     2316 2022-09-16 08:17:01.000000 pcvs-0.6.0/pcvs/templates/config/criterion.large.yml
--rw-r--r--   0 adamj     (1000) adamj     (1000)     2182 2022-09-16 08:17:01.000000 pcvs-0.6.0/pcvs/templates/config/criterion.small.yml
--rw-r--r--   0 adamj     (1000) adamj     (1000)      472 2022-09-16 08:17:01.000000 pcvs-0.6.0/pcvs/templates/config/group.common.yml
--rw-r--r--   0 adamj     (1000) adamj     (1000)      472 2022-09-16 08:17:01.000000 pcvs-0.6.0/pcvs/templates/config/group.default.yml
--rw-r--r--   0 adamj     (1000) adamj     (1000)      193 2022-09-16 08:17:01.000000 pcvs-0.6.0/pcvs/templates/config/machine.default.yml
--rw-r--r--   0 adamj     (1000) adamj     (1000)      193 2022-09-16 08:17:01.000000 pcvs-0.6.0/pcvs/templates/config/machine.localhost.yml
--rw-r--r--   0 adamj     (1000) adamj     (1000)     1494 2022-09-16 08:17:01.000000 pcvs-0.6.0/pcvs/templates/config/machine.slurm.yml
--rw-r--r--   0 adamj     (1000) adamj     (1000)     1177 2022-09-16 08:17:01.000000 pcvs-0.6.0/pcvs/templates/config/runtime.default.yml
--rw-r--r--   0 adamj     (1000) adamj     (1000)     1177 2022-09-16 08:17:01.000000 pcvs-0.6.0/pcvs/templates/config/runtime.mpi.yml
--rw-r--r--   0 adamj     (1000) adamj     (1000)      643 2022-09-16 08:17:01.000000 pcvs-0.6.0/pcvs/templates/config/runtime.void.yml
-drwxr-xr-x   0 adamj     (1000) adamj     (1000)        0 2022-09-16 08:37:08.861061 pcvs-0.6.0/pcvs/templates/profile/
--rw-r--r--   0 adamj     (1000) adamj     (1000)     1671 2022-09-16 08:17:01.000000 pcvs-0.6.0/pcvs/templates/profile/default.yml
--rw-r--r--   0 adamj     (1000) adamj     (1000)      161 2022-09-16 08:17:01.000000 pcvs-0.6.0/pcvs/templates/profile/gcc.yml
--rw-r--r--   0 adamj     (1000) adamj     (1000)      153 2022-09-16 08:17:01.000000 pcvs-0.6.0/pcvs/templates/profile/icc.yml
--rw-r--r--   0 adamj     (1000) adamj     (1000)     2113 2022-09-16 08:17:01.000000 pcvs-0.6.0/pcvs/templates/profile/mpi-omp.yml
--rw-r--r--   0 adamj     (1000) adamj     (1000)     1800 2022-09-16 08:17:01.000000 pcvs-0.6.0/pcvs/templates/profile/mpi-slurm.yml
--rw-r--r--   0 adamj     (1000) adamj     (1000)     1671 2022-09-16 08:17:01.000000 pcvs-0.6.0/pcvs/templates/profile/mpi.yml
--rw-r--r--   0 adamj     (1000) adamj     (1000)     1604 2022-09-16 08:17:01.000000 pcvs-0.6.0/pcvs/templates/profile/omp.yml
-drwxr-xr-x   0 adamj     (1000) adamj     (1000)        0 2022-09-16 08:37:08.861061 pcvs-0.6.0/pcvs/testing/
--rw-r--r--   0 adamj     (1000) adamj     (1000)     1174 2022-09-16 08:17:01.000000 pcvs-0.6.0/pcvs/testing/__init__.py
--rw-r--r--   0 adamj     (1000) adamj     (1000)    25288 2022-09-16 08:17:01.000000 pcvs-0.6.0/pcvs/testing/tedesc.py
--rw-r--r--   0 adamj     (1000) adamj     (1000)    18860 2022-09-16 08:17:01.000000 pcvs-0.6.0/pcvs/testing/test.py
--rw-r--r--   0 adamj     (1000) adamj     (1000)    10184 2022-09-16 08:17:01.000000 pcvs-0.6.0/pcvs/testing/testfile.py
--rw-r--r--   0 adamj     (1000) adamj     (1000)      211 2022-09-16 08:36:58.000000 pcvs-0.6.0/pcvs/version.py
-drwxr-xr-x   0 adamj     (1000) adamj     (1000)        0 2022-09-16 08:37:08.861061 pcvs-0.6.0/pcvs/webview/
--rw-r--r--   0 adamj     (1000) adamj     (1000)     6254 2022-09-16 08:17:01.000000 pcvs-0.6.0/pcvs/webview/__init__.py
--rw-r--r--   0 adamj     (1000) adamj     (1000)     8184 2022-09-16 08:17:01.000000 pcvs-0.6.0/pcvs/webview/datalayer.py
-drwxr-xr-x   0 adamj     (1000) adamj     (1000)        0 2022-09-16 08:37:08.853061 pcvs-0.6.0/pcvs/webview/static/
-drwxr-xr-x   0 adamj     (1000) adamj     (1000)        0 2022-09-16 08:37:08.861061 pcvs-0.6.0/pcvs/webview/static/css/
--rw-r--r--   0 adamj     (1000) adamj     (1000)   160392 2022-09-16 08:17:01.000000 pcvs-0.6.0/pcvs/webview/static/css/bootstrap.min.css
--rw-r--r--   0 adamj     (1000) adamj     (1000)      713 2022-09-16 08:17:01.000000 pcvs-0.6.0/pcvs/webview/static/css/custom.css
--rwxr-xr-x   0 adamj     (1000) adamj     (1000)    18756 2022-09-16 08:17:01.000000 pcvs-0.6.0/pcvs/webview/static/css/datatables.min.css
--rwxr-xr-x   0 adamj     (1000) adamj     (1000)     9395 2022-09-16 08:17:01.000000 pcvs-0.6.0/pcvs/webview/static/css/open-iconic-bootstrap.min.css
-drwxr-xr-x   0 adamj     (1000) adamj     (1000)        0 2022-09-16 08:37:08.861061 pcvs-0.6.0/pcvs/webview/static/fonts/
--rwxr-xr-x   0 adamj     (1000) adamj     (1000)    54789 2022-09-16 08:17:01.000000 pcvs-0.6.0/pcvs/webview/static/fonts/open-iconic.svg
-drwxr-xr-x   0 adamj     (1000) adamj     (1000)        0 2022-09-16 08:37:08.861061 pcvs-0.6.0/pcvs/webview/static/images/
--rw-r--r--   0 adamj     (1000) adamj     (1000)    41702 2022-09-16 08:17:01.000000 pcvs-0.6.0/pcvs/webview/static/images/cea_logo.png
--rw-r--r--   0 adamj     (1000) adamj     (1000)    20191 2022-09-16 08:17:01.000000 pcvs-0.6.0/pcvs/webview/static/images/favicon.ico
--rw-r--r--   0 adamj     (1000) adamj     (1000)    85307 2022-09-16 08:17:01.000000 pcvs-0.6.0/pcvs/webview/static/images/full_logo.png
--rw-r--r--   0 adamj     (1000) adamj     (1000)    68308 2022-09-16 08:17:01.000000 pcvs-0.6.0/pcvs/webview/static/images/full_logo_transparent.png
--rwxr-xr-x   0 adamj     (1000) adamj     (1000)      160 2022-09-16 08:17:01.000000 pcvs-0.6.0/pcvs/webview/static/images/sort_asc.png
--rwxr-xr-x   0 adamj     (1000) adamj     (1000)      148 2022-09-16 08:17:01.000000 pcvs-0.6.0/pcvs/webview/static/images/sort_asc_disabled.png
--rwxr-xr-x   0 adamj     (1000) adamj     (1000)      201 2022-09-16 08:17:01.000000 pcvs-0.6.0/pcvs/webview/static/images/sort_both.png
--rwxr-xr-x   0 adamj     (1000) adamj     (1000)      158 2022-09-16 08:17:01.000000 pcvs-0.6.0/pcvs/webview/static/images/sort_desc.png
--rwxr-xr-x   0 adamj     (1000) adamj     (1000)      146 2022-09-16 08:17:01.000000 pcvs-0.6.0/pcvs/webview/static/images/sort_desc_disabled.png
-drwxr-xr-x   0 adamj     (1000) adamj     (1000)        0 2022-09-16 08:37:08.865061 pcvs-0.6.0/pcvs/webview/static/js/
--rw-r--r--   0 adamj     (1000) adamj     (1000)    84152 2022-09-16 08:17:01.000000 pcvs-0.6.0/pcvs/webview/static/js/bootstrap.bundle.min.js
--rw-r--r--   0 adamj     (1000) adamj     (1000)     3525 2022-09-16 08:17:01.000000 pcvs-0.6.0/pcvs/webview/static/js/custom.js
--rwxr-xr-x   0 adamj     (1000) adamj     (1000)   103764 2022-09-16 08:17:01.000000 pcvs-0.6.0/pcvs/webview/static/js/datatables.min.js
--rw-r--r--   0 adamj     (1000) adamj     (1000)    86709 2022-09-16 08:17:01.000000 pcvs-0.6.0/pcvs/webview/static/js/jquery.min.js
-drwxr-xr-x   0 adamj     (1000) adamj     (1000)        0 2022-09-16 08:37:08.865061 pcvs-0.6.0/pcvs/webview/templates/
--rw-r--r--   0 adamj     (1000) adamj     (1000)      227 2022-09-16 08:17:01.000000 pcvs-0.6.0/pcvs/webview/templates/404.html
--rw-r--r--   0 adamj     (1000) adamj     (1000)       59 2022-09-16 08:17:01.000000 pcvs-0.6.0/pcvs/webview/templates/base-extend.html
--rw-r--r--   0 adamj     (1000) adamj     (1000)     4910 2022-09-16 08:17:01.000000 pcvs-0.6.0/pcvs/webview/templates/base.html
--rw-r--r--   0 adamj     (1000) adamj     (1000)     2764 2022-09-16 08:17:01.000000 pcvs-0.6.0/pcvs/webview/templates/brief.html
--rw-r--r--   0 adamj     (1000) adamj     (1000)     2715 2022-09-16 08:17:01.000000 pcvs-0.6.0/pcvs/webview/templates/detailed_view.html
--rw-r--r--   0 adamj     (1000) adamj     (1000)       70 2022-09-16 08:17:01.000000 pcvs-0.6.0/pcvs/webview/templates/diff.html
--rw-r--r--   0 adamj     (1000) adamj     (1000)     2138 2022-09-16 08:17:01.000000 pcvs-0.6.0/pcvs/webview/templates/list_view.html
--rw-r--r--   0 adamj     (1000) adamj     (1000)     2677 2022-09-16 08:17:01.000000 pcvs-0.6.0/pcvs/webview/templates/main.html
--rw-r--r--   0 adamj     (1000) adamj     (1000)     1945 2022-09-16 08:17:01.000000 pcvs-0.6.0/pcvs/webview/templates/session_main.html
--rw-r--r--   0 adamj     (1000) adamj     (1000)      287 2022-09-16 08:17:01.000000 pcvs-0.6.0/pcvs/webview/templates/tbw.html
-drwxr-xr-x   0 adamj     (1000) adamj     (1000)        0 2022-09-16 08:37:08.853061 pcvs-0.6.0/pcvs.egg-info/
--rw-r--r--   0 adamj     (1000) adamj     (1000)     3380 2022-09-16 08:37:08.000000 pcvs-0.6.0/pcvs.egg-info/PKG-INFO
--rw-r--r--   0 adamj     (1000) adamj     (1000)     4058 2022-09-16 08:37:08.000000 pcvs-0.6.0/pcvs.egg-info/SOURCES.txt
--rw-r--r--   0 adamj     (1000) adamj     (1000)        1 2022-09-16 08:37:08.000000 pcvs-0.6.0/pcvs.egg-info/dependency_links.txt
--rw-r--r--   0 adamj     (1000) adamj     (1000)       89 2022-09-16 08:37:08.000000 pcvs-0.6.0/pcvs.egg-info/entry_points.txt
--rw-r--r--   0 adamj     (1000) adamj     (1000)      106 2022-09-16 08:37:08.000000 pcvs-0.6.0/pcvs.egg-info/requires.txt
--rw-r--r--   0 adamj     (1000) adamj     (1000)       11 2022-09-16 08:37:08.000000 pcvs-0.6.0/pcvs.egg-info/top_level.txt
--rw-r--r--   0 adamj     (1000) adamj     (1000)      127 2022-09-16 08:17:01.000000 pcvs-0.6.0/requirements-dev.txt
--rw-r--r--   0 adamj     (1000) adamj     (1000)      103 2022-09-16 08:17:01.000000 pcvs-0.6.0/requirements.txt
--rw-r--r--   0 adamj     (1000) adamj     (1000)       38 2022-09-16 08:37:08.865061 pcvs-0.6.0/setup.cfg
--rw-r--r--   0 adamj     (1000) adamj     (1000)     1429 2022-09-16 08:17:01.000000 pcvs-0.6.0/setup.py
-drwxr-xr-x   0 adamj     (1000) adamj     (1000)        0 2022-09-16 08:37:08.865061 pcvs-0.6.0/tests/
--rw-r--r--   0 adamj     (1000) adamj     (1000)        0 2022-09-16 08:17:01.000000 pcvs-0.6.0/tests/__init__.py
-drwxr-xr-x   0 adamj     (1000) adamj     (1000)        0 2022-09-16 08:37:08.865061 pcvs-0.6.0/tests/pcvs/
--rw-r--r--   0 adamj     (1000) adamj     (1000)        0 2022-09-16 08:17:01.000000 pcvs-0.6.0/tests/pcvs/__init__.py
-drwxr-xr-x   0 adamj     (1000) adamj     (1000)        0 2022-09-16 08:37:08.865061 pcvs-0.6.0/tests/pcvs/cli/
--rw-r--r--   0 adamj     (1000) adamj     (1000)        0 2022-09-16 08:17:01.000000 pcvs-0.6.0/tests/pcvs/cli/__init__.py
--rw-r--r--   0 adamj     (1000) adamj     (1000)      264 2022-09-16 08:17:01.000000 pcvs-0.6.0/tests/pcvs/cli/conftest.py
--rw-r--r--   0 adamj     (1000) adamj     (1000)      453 2022-09-16 08:17:01.000000 pcvs-0.6.0/tests/pcvs/cli/test_basics.py
--rw-r--r--   0 adamj     (1000) adamj     (1000)     6391 2022-09-16 08:17:01.000000 pcvs-0.6.0/tests/pcvs/cli/test_config.py
--rw-r--r--   0 adamj     (1000) adamj     (1000)     3024 2022-09-16 08:17:01.000000 pcvs-0.6.0/tests/pcvs/cli/test_profile.py
--rw-r--r--   0 adamj     (1000) adamj     (1000)     1225 2022-09-16 08:17:01.000000 pcvs-0.6.0/tests/pcvs/cli/test_run.py
--rw-r--r--   0 adamj     (1000) adamj     (1000)     1187 2022-09-16 08:17:01.000000 pcvs-0.6.0/tests/pcvs/cli/test_utilities.py
-drwxr-xr-x   0 adamj     (1000) adamj     (1000)        0 2022-09-16 08:37:08.865061 pcvs-0.6.0/tests/pcvs/converter/
--rw-r--r--   0 adamj     (1000) adamj     (1000)        0 2022-09-16 08:17:01.000000 pcvs-0.6.0/tests/pcvs/converter/__init__.py
--rw-r--r--   0 adamj     (1000) adamj     (1000)      284 2022-09-16 08:17:01.000000 pcvs-0.6.0/tests/pcvs/converter/conftest.py
--rw-r--r--   0 adamj     (1000) adamj     (1000)     1155 2022-09-16 08:17:01.000000 pcvs-0.6.0/tests/pcvs/converter/test_converter.py
+drwxr-xr-x   0 adamj     (1000) adamj     (1000)        0 2023-06-09 10:15:05.000000 pcvs-0.7.0/
+-rw-r--r--   0 adamj     (1000) adamj     (1000)      617 2023-06-08 08:49:05.000000 pcvs-0.7.0/AUTHORS
+-rw-r--r--   0 adamj     (1000) adamj     (1000)      436 2023-06-08 08:49:05.000000 pcvs-0.7.0/CHANGES
+-rw-r--r--   0 adamj     (1000) adamj     (1000)    21865 2023-06-08 08:49:05.000000 pcvs-0.7.0/COPYING
+-rw-r--r--   0 adamj     (1000) adamj     (1000)      363 2023-06-08 08:49:05.000000 pcvs-0.7.0/MANIFEST.in
+-rw-r--r--   0 adamj     (1000) adamj     (1000)     3087 2023-06-09 10:15:05.000000 pcvs-0.7.0/PKG-INFO
+-rw-r--r--   0 adamj     (1000) adamj     (1000)     2497 2023-06-09 09:57:20.000000 pcvs-0.7.0/README.md
+drwxr-xr-x   0 adamj     (1000) adamj     (1000)        0 2023-06-09 10:15:05.000000 pcvs-0.7.0/pcvs/
+-rw-r--r--   0 adamj     (1000) adamj     (1000)      760 2023-06-08 12:28:28.000000 pcvs-0.7.0/pcvs/__init__.py
+drwxr-xr-x   0 adamj     (1000) adamj     (1000)        0 2023-06-09 10:15:05.000000 pcvs-0.7.0/pcvs/backend/
+-rw-r--r--   0 adamj     (1000) adamj     (1000)        0 2023-06-08 08:49:05.000000 pcvs-0.7.0/pcvs/backend/__init__.py
+-rw-r--r--   0 adamj     (1000) adamj     (1000)    13266 2023-06-08 08:49:05.000000 pcvs-0.7.0/pcvs/backend/bank.py
+-rw-r--r--   0 adamj     (1000) adamj     (1000)    13285 2023-06-08 08:49:05.000000 pcvs-0.7.0/pcvs/backend/config.py
+-rw-r--r--   0 adamj     (1000) adamj     (1000)    15959 2023-06-08 08:49:05.000000 pcvs-0.7.0/pcvs/backend/profile.py
+-rw-r--r--   0 adamj     (1000) adamj     (1000)     9968 2023-06-08 08:49:05.000000 pcvs-0.7.0/pcvs/backend/report.py
+-rw-r--r--   0 adamj     (1000) adamj     (1000)    23112 2023-06-08 08:49:05.000000 pcvs-0.7.0/pcvs/backend/run.py
+-rw-r--r--   0 adamj     (1000) adamj     (1000)    12584 2023-06-08 08:49:05.000000 pcvs-0.7.0/pcvs/backend/session.py
+-rw-r--r--   0 adamj     (1000) adamj     (1000)     1430 2023-06-08 08:49:05.000000 pcvs-0.7.0/pcvs/backend/spack.py
+-rw-r--r--   0 adamj     (1000) adamj     (1000)    14076 2023-06-08 08:49:05.000000 pcvs-0.7.0/pcvs/backend/utilities.py
+drwxr-xr-x   0 adamj     (1000) adamj     (1000)        0 2023-06-09 10:15:05.000000 pcvs-0.7.0/pcvs/cli/
+-rw-r--r--   0 adamj     (1000) adamj     (1000)        0 2023-06-08 08:49:05.000000 pcvs-0.7.0/pcvs/cli/__init__.py
+-rw-r--r--   0 adamj     (1000) adamj     (1000)     6744 2023-06-08 08:49:05.000000 pcvs-0.7.0/pcvs/cli/cli_bank.py
+-rw-r--r--   0 adamj     (1000) adamj     (1000)    12561 2023-06-08 08:49:05.000000 pcvs-0.7.0/pcvs/cli/cli_config.py
+-rw-r--r--   0 adamj     (1000) adamj     (1000)     1040 2023-06-08 08:49:05.000000 pcvs-0.7.0/pcvs/cli/cli_plumbing.py
+-rw-r--r--   0 adamj     (1000) adamj     (1000)    15742 2023-06-08 08:49:05.000000 pcvs-0.7.0/pcvs/cli/cli_profile.py
+-rw-r--r--   0 adamj     (1000) adamj     (1000)     1616 2023-06-08 08:49:05.000000 pcvs-0.7.0/pcvs/cli/cli_remote_run.py
+-rw-r--r--   0 adamj     (1000) adamj     (1000)     1977 2023-06-08 13:52:13.000000 pcvs-0.7.0/pcvs/cli/cli_report.py
+-rw-r--r--   0 adamj     (1000) adamj     (1000)    12742 2023-06-08 08:49:05.000000 pcvs-0.7.0/pcvs/cli/cli_run.py
+-rw-r--r--   0 adamj     (1000) adamj     (1000)     4455 2023-06-08 08:49:05.000000 pcvs-0.7.0/pcvs/cli/cli_session.py
+-rw-r--r--   0 adamj     (1000) adamj     (1000)    10995 2023-06-08 08:49:05.000000 pcvs-0.7.0/pcvs/cli/cli_utilities.py
+drwxr-xr-x   0 adamj     (1000) adamj     (1000)        0 2023-06-09 10:15:05.000000 pcvs-0.7.0/pcvs/converter/
+-rw-r--r--   0 adamj     (1000) adamj     (1000)        0 2023-06-08 08:49:05.000000 pcvs-0.7.0/pcvs/converter/__init__.py
+-rwxr-xr-x   0 adamj     (1000) adamj     (1000)     1730 2023-06-08 08:49:05.000000 pcvs-0.7.0/pcvs/converter/result_converter.py
+-rwxr-xr-x   0 adamj     (1000) adamj     (1000)    14568 2023-06-08 08:49:05.000000 pcvs-0.7.0/pcvs/converter/yaml_converter.py
+drwxr-xr-x   0 adamj     (1000) adamj     (1000)        0 2023-06-09 10:15:05.000000 pcvs-0.7.0/pcvs/dsl/
+-rw-r--r--   0 adamj     (1000) adamj     (1000)     8725 2023-06-08 08:49:05.000000 pcvs-0.7.0/pcvs/dsl/__init__.py
+-rw-r--r--   0 adamj     (1000) adamj     (1000)     2272 2023-06-08 08:49:05.000000 pcvs-0.7.0/pcvs/dsl/analysis.py
+-rw-r--r--   0 adamj     (1000) adamj     (1000)     1003 2023-06-08 08:49:05.000000 pcvs-0.7.0/pcvs/dsl/render.py
+drwxr-xr-x   0 adamj     (1000) adamj     (1000)        0 2023-06-09 10:15:05.000000 pcvs-0.7.0/pcvs/helpers/
+-rw-r--r--   0 adamj     (1000) adamj     (1000)        0 2023-06-08 08:49:05.000000 pcvs-0.7.0/pcvs/helpers/__init__.py
+-rw-r--r--   0 adamj     (1000) adamj     (1000)     2539 2023-06-08 08:49:05.000000 pcvs-0.7.0/pcvs/helpers/communications.py
+-rw-r--r--   0 adamj     (1000) adamj     (1000)    18436 2023-06-08 08:49:05.000000 pcvs-0.7.0/pcvs/helpers/criterion.py
+-rw-r--r--   0 adamj     (1000) adamj     (1000)     9727 2023-06-08 08:49:05.000000 pcvs-0.7.0/pcvs/helpers/exceptions.py
+-rw-r--r--   0 adamj     (1000) adamj     (1000)    27815 2023-06-08 08:49:05.000000 pcvs-0.7.0/pcvs/helpers/git.py
+-rw-r--r--   0 adamj     (1000) adamj     (1000)     1031 2023-06-08 08:49:05.000000 pcvs-0.7.0/pcvs/helpers/log.py
+-rw-r--r--   0 adamj     (1000) adamj     (1000)     3119 2023-06-08 08:49:05.000000 pcvs-0.7.0/pcvs/helpers/pm.py
+-rw-r--r--   0 adamj     (1000) adamj     (1000)    16384 2023-06-08 08:49:05.000000 pcvs-0.7.0/pcvs/helpers/system.py
+-rw-r--r--   0 adamj     (1000) adamj     (1000)    14251 2023-06-08 08:49:05.000000 pcvs-0.7.0/pcvs/helpers/utils.py
+-rw-r--r--   0 adamj     (1000) adamj     (1000)    15192 2023-06-08 08:49:05.000000 pcvs-0.7.0/pcvs/io.py
+-rw-r--r--   0 adamj     (1000) adamj     (1000)     4392 2023-06-08 08:49:05.000000 pcvs-0.7.0/pcvs/main.py
+drwxr-xr-x   0 adamj     (1000) adamj     (1000)        0 2023-06-09 10:15:05.000000 pcvs-0.7.0/pcvs/orchestration/
+-rw-r--r--   0 adamj     (1000) adamj     (1000)     6738 2023-06-08 08:49:05.000000 pcvs-0.7.0/pcvs/orchestration/__init__.py
+-rw-r--r--   0 adamj     (1000) adamj     (1000)      101 2023-06-08 08:49:05.000000 pcvs-0.7.0/pcvs/orchestration/__main__.py
+-rw-r--r--   0 adamj     (1000) adamj     (1000)    12742 2023-06-08 08:49:05.000000 pcvs-0.7.0/pcvs/orchestration/manager.py
+-rw-r--r--   0 adamj     (1000) adamj     (1000)    32840 2023-06-08 08:49:05.000000 pcvs-0.7.0/pcvs/orchestration/publishers.py
+-rw-r--r--   0 adamj     (1000) adamj     (1000)     9808 2023-06-08 08:49:05.000000 pcvs-0.7.0/pcvs/orchestration/runner.py
+-rw-r--r--   0 adamj     (1000) adamj     (1000)     5087 2023-06-08 08:49:05.000000 pcvs-0.7.0/pcvs/orchestration/set.py
+drwxr-xr-x   0 adamj     (1000) adamj     (1000)        0 2023-06-09 10:15:05.000000 pcvs-0.7.0/pcvs/plugins/
+-rw-r--r--   0 adamj     (1000) adamj     (1000)     8024 2023-06-08 08:49:05.000000 pcvs-0.7.0/pcvs/plugins/__init__.py
+drwxr-xr-x   0 adamj     (1000) adamj     (1000)        0 2023-06-09 10:15:05.000000 pcvs-0.7.0/pcvs/plugins/default/
+-rw-r--r--   0 adamj     (1000) adamj     (1000)        0 2023-06-08 08:49:05.000000 pcvs-0.7.0/pcvs/plugins/default/__init__.py
+-rw-r--r--   0 adamj     (1000) adamj     (1000)     1922 2023-06-08 08:49:05.000000 pcvs-0.7.0/pcvs/plugins/default/validation.py
+drwxr-xr-x   0 adamj     (1000) adamj     (1000)        0 2023-06-09 10:15:05.000000 pcvs-0.7.0/pcvs/schemes/
+-rw-r--r--   0 adamj     (1000) adamj     (1000)     1293 2023-06-08 08:49:05.000000 pcvs-0.7.0/pcvs/schemes/compiler-scheme.yml
+-rw-r--r--   0 adamj     (1000) adamj     (1000)      278 2023-06-08 08:49:05.000000 pcvs-0.7.0/pcvs/schemes/criterion-scheme.yml
+-rw-r--r--   0 adamj     (1000) adamj     (1000)     5092 2023-06-08 08:49:05.000000 pcvs-0.7.0/pcvs/schemes/group-scheme.yml
+-rw-r--r--   0 adamj     (1000) adamj     (1000)     1011 2023-06-08 08:49:05.000000 pcvs-0.7.0/pcvs/schemes/machine-scheme.yml
+-rw-r--r--   0 adamj     (1000) adamj     (1000)      973 2023-06-08 08:49:05.000000 pcvs-0.7.0/pcvs/schemes/runtime-scheme.yml
+-rw-r--r--   0 adamj     (1000) adamj     (1000)      919 2023-06-08 08:49:05.000000 pcvs-0.7.0/pcvs/schemes/settings-scheme.yml
+-rw-r--r--   0 adamj     (1000) adamj     (1000)     6825 2023-06-08 08:49:05.000000 pcvs-0.7.0/pcvs/schemes/te-scheme.yml
+-rw-r--r--   0 adamj     (1000) adamj     (1000)     1566 2023-06-08 08:49:05.000000 pcvs-0.7.0/pcvs/schemes/test-result-scheme.yml
+-rw-r--r--   0 adamj     (1000) adamj     (1000)     1420 2023-06-08 08:49:05.000000 pcvs-0.7.0/pcvs/schemes/validation-scheme.yml
+drwxr-xr-x   0 adamj     (1000) adamj     (1000)        0 2023-06-09 10:15:05.000000 pcvs-0.7.0/pcvs/templates/
+drwxr-xr-x   0 adamj     (1000) adamj     (1000)        0 2023-06-09 10:15:05.000000 pcvs-0.7.0/pcvs/templates/config/
+-rw-r--r--   0 adamj     (1000) adamj     (1000)      186 2023-06-08 08:49:05.000000 pcvs-0.7.0/pcvs/templates/config/compiler.default.yml
+-rw-r--r--   0 adamj     (1000) adamj     (1000)      268 2023-06-08 08:49:05.000000 pcvs-0.7.0/pcvs/templates/config/compiler.gcc.yml
+-rw-r--r--   0 adamj     (1000) adamj     (1000)      257 2023-06-08 08:49:05.000000 pcvs-0.7.0/pcvs/templates/config/compiler.icc.yml
+-rw-r--r--   0 adamj     (1000) adamj     (1000)      186 2023-06-08 08:49:05.000000 pcvs-0.7.0/pcvs/templates/config/compiler.mpi.yml
+-rw-r--r--   0 adamj     (1000) adamj     (1000)     2147 2023-06-08 08:49:05.000000 pcvs-0.7.0/pcvs/templates/config/criterion.default.yml
+-rw-r--r--   0 adamj     (1000) adamj     (1000)     2269 2023-06-08 08:49:05.000000 pcvs-0.7.0/pcvs/templates/config/criterion.large.yml
+-rw-r--r--   0 adamj     (1000) adamj     (1000)     2147 2023-06-08 08:49:05.000000 pcvs-0.7.0/pcvs/templates/config/criterion.small.yml
+-rw-r--r--   0 adamj     (1000) adamj     (1000)      674 2023-06-08 08:49:05.000000 pcvs-0.7.0/pcvs/templates/config/group-compat.yml
+-rw-r--r--   0 adamj     (1000) adamj     (1000)      472 2023-06-08 08:49:05.000000 pcvs-0.7.0/pcvs/templates/config/group.common.yml
+-rw-r--r--   0 adamj     (1000) adamj     (1000)      472 2023-06-08 08:49:05.000000 pcvs-0.7.0/pcvs/templates/config/group.default.yml
+-rw-r--r--   0 adamj     (1000) adamj     (1000)      193 2023-06-08 08:49:05.000000 pcvs-0.7.0/pcvs/templates/config/machine.default.yml
+-rw-r--r--   0 adamj     (1000) adamj     (1000)      193 2023-06-08 08:49:05.000000 pcvs-0.7.0/pcvs/templates/config/machine.localhost.yml
+-rw-r--r--   0 adamj     (1000) adamj     (1000)     1555 2023-06-08 08:49:05.000000 pcvs-0.7.0/pcvs/templates/config/machine.slurm.yml
+-rw-r--r--   0 adamj     (1000) adamj     (1000)     1178 2023-06-08 08:49:05.000000 pcvs-0.7.0/pcvs/templates/config/runtime.default.yml
+-rw-r--r--   0 adamj     (1000) adamj     (1000)     1178 2023-06-08 08:49:05.000000 pcvs-0.7.0/pcvs/templates/config/runtime.mpi.yml
+-rw-r--r--   0 adamj     (1000) adamj     (1000)      605 2023-06-08 08:49:05.000000 pcvs-0.7.0/pcvs/templates/config/runtime.void.yml
+drwxr-xr-x   0 adamj     (1000) adamj     (1000)        0 2023-06-09 10:15:05.000000 pcvs-0.7.0/pcvs/templates/profile/
+-rw-r--r--   0 adamj     (1000) adamj     (1000)     1706 2023-06-08 08:49:05.000000 pcvs-0.7.0/pcvs/templates/profile/default.yml
+-rw-r--r--   0 adamj     (1000) adamj     (1000)      235 2023-06-08 08:49:05.000000 pcvs-0.7.0/pcvs/templates/profile/gcc.yml
+-rw-r--r--   0 adamj     (1000) adamj     (1000)      224 2023-06-08 08:49:05.000000 pcvs-0.7.0/pcvs/templates/profile/icc.yml
+-rw-r--r--   0 adamj     (1000) adamj     (1000)     2208 2023-06-08 08:49:05.000000 pcvs-0.7.0/pcvs/templates/profile/mpi-omp.yml
+-rw-r--r--   0 adamj     (1000) adamj     (1000)     1817 2023-06-08 08:49:05.000000 pcvs-0.7.0/pcvs/templates/profile/mpi-slurm.yml
+-rw-r--r--   0 adamj     (1000) adamj     (1000)     1706 2023-06-08 08:49:05.000000 pcvs-0.7.0/pcvs/templates/profile/mpi.yml
+-rw-r--r--   0 adamj     (1000) adamj     (1000)     1660 2023-06-08 08:49:05.000000 pcvs-0.7.0/pcvs/templates/profile/omp.yml
+drwxr-xr-x   0 adamj     (1000) adamj     (1000)        0 2023-06-09 10:15:05.000000 pcvs-0.7.0/pcvs/testing/
+-rw-r--r--   0 adamj     (1000) adamj     (1000)     1079 2023-06-08 08:49:05.000000 pcvs-0.7.0/pcvs/testing/__init__.py
+-rw-r--r--   0 adamj     (1000) adamj     (1000)    25749 2023-06-08 08:49:05.000000 pcvs-0.7.0/pcvs/testing/tedesc.py
+-rw-r--r--   0 adamj     (1000) adamj     (1000)    21678 2023-06-08 08:49:05.000000 pcvs-0.7.0/pcvs/testing/test.py
+-rw-r--r--   0 adamj     (1000) adamj     (1000)    11459 2023-06-08 08:49:05.000000 pcvs-0.7.0/pcvs/testing/testfile.py
+-rw-r--r--   0 adamj     (1000) adamj     (1000)       22 2023-06-09 09:58:12.000000 pcvs-0.7.0/pcvs/version.py
+drwxr-xr-x   0 adamj     (1000) adamj     (1000)        0 2023-06-09 10:15:05.000000 pcvs-0.7.0/pcvs/webview/
+-rw-r--r--   0 adamj     (1000) adamj     (1000)     6578 2023-06-08 08:49:05.000000 pcvs-0.7.0/pcvs/webview/__init__.py
+-rw-r--r--   0 adamj     (1000) adamj     (1000)     8187 2023-06-08 08:49:05.000000 pcvs-0.7.0/pcvs/webview/datalayer.py
+drwxr-xr-x   0 adamj     (1000) adamj     (1000)        0 2023-06-09 10:15:05.000000 pcvs-0.7.0/pcvs/webview/static/
+drwxr-xr-x   0 adamj     (1000) adamj     (1000)        0 2023-06-09 10:15:05.000000 pcvs-0.7.0/pcvs/webview/static/css/
+-rw-r--r--   0 adamj     (1000) adamj     (1000)   160392 2023-06-08 08:49:05.000000 pcvs-0.7.0/pcvs/webview/static/css/bootstrap.min.css
+-rw-r--r--   0 adamj     (1000) adamj     (1000)      763 2023-06-08 08:49:05.000000 pcvs-0.7.0/pcvs/webview/static/css/custom.css
+-rwxr-xr-x   0 adamj     (1000) adamj     (1000)    18756 2023-06-08 08:49:05.000000 pcvs-0.7.0/pcvs/webview/static/css/datatables.min.css
+-rwxr-xr-x   0 adamj     (1000) adamj     (1000)     9395 2023-06-08 08:49:05.000000 pcvs-0.7.0/pcvs/webview/static/css/open-iconic-bootstrap.min.css
+drwxr-xr-x   0 adamj     (1000) adamj     (1000)        0 2023-06-09 10:15:05.000000 pcvs-0.7.0/pcvs/webview/static/fonts/
+-rwxr-xr-x   0 adamj     (1000) adamj     (1000)    54789 2023-06-08 08:49:05.000000 pcvs-0.7.0/pcvs/webview/static/fonts/open-iconic.svg
+drwxr-xr-x   0 adamj     (1000) adamj     (1000)        0 2023-06-09 10:15:05.000000 pcvs-0.7.0/pcvs/webview/static/images/
+-rw-r--r--   0 adamj     (1000) adamj     (1000)    41702 2023-06-08 08:49:05.000000 pcvs-0.7.0/pcvs/webview/static/images/cea_logo.png
+-rw-r--r--   0 adamj     (1000) adamj     (1000)    20191 2023-06-08 08:49:05.000000 pcvs-0.7.0/pcvs/webview/static/images/favicon.ico
+-rw-r--r--   0 adamj     (1000) adamj     (1000)    85307 2023-06-08 08:49:05.000000 pcvs-0.7.0/pcvs/webview/static/images/full_logo.png
+-rw-r--r--   0 adamj     (1000) adamj     (1000)    68308 2023-06-08 08:49:05.000000 pcvs-0.7.0/pcvs/webview/static/images/full_logo_transparent.png
+-rwxr-xr-x   0 adamj     (1000) adamj     (1000)      160 2023-06-08 08:49:05.000000 pcvs-0.7.0/pcvs/webview/static/images/sort_asc.png
+-rwxr-xr-x   0 adamj     (1000) adamj     (1000)      148 2023-06-08 08:49:05.000000 pcvs-0.7.0/pcvs/webview/static/images/sort_asc_disabled.png
+-rwxr-xr-x   0 adamj     (1000) adamj     (1000)      201 2023-06-08 08:49:05.000000 pcvs-0.7.0/pcvs/webview/static/images/sort_both.png
+-rwxr-xr-x   0 adamj     (1000) adamj     (1000)      158 2023-06-08 08:49:05.000000 pcvs-0.7.0/pcvs/webview/static/images/sort_desc.png
+-rwxr-xr-x   0 adamj     (1000) adamj     (1000)      146 2023-06-08 08:49:05.000000 pcvs-0.7.0/pcvs/webview/static/images/sort_desc_disabled.png
+drwxr-xr-x   0 adamj     (1000) adamj     (1000)        0 2023-06-09 10:15:05.000000 pcvs-0.7.0/pcvs/webview/static/js/
+-rw-r--r--   0 adamj     (1000) adamj     (1000)    84152 2023-06-08 08:49:05.000000 pcvs-0.7.0/pcvs/webview/static/js/bootstrap.bundle.min.js
+-rw-r--r--   0 adamj     (1000) adamj     (1000)     3525 2023-06-08 08:49:05.000000 pcvs-0.7.0/pcvs/webview/static/js/custom.js
+-rwxr-xr-x   0 adamj     (1000) adamj     (1000)   103764 2023-06-08 08:49:05.000000 pcvs-0.7.0/pcvs/webview/static/js/datatables.min.js
+-rw-r--r--   0 adamj     (1000) adamj     (1000)    86709 2023-06-08 08:49:05.000000 pcvs-0.7.0/pcvs/webview/static/js/jquery.min.js
+drwxr-xr-x   0 adamj     (1000) adamj     (1000)        0 2023-06-09 10:15:05.000000 pcvs-0.7.0/pcvs/webview/templates/
+-rw-r--r--   0 adamj     (1000) adamj     (1000)      227 2023-06-08 08:49:05.000000 pcvs-0.7.0/pcvs/webview/templates/404.html
+-rw-r--r--   0 adamj     (1000) adamj     (1000)       59 2023-06-08 08:49:05.000000 pcvs-0.7.0/pcvs/webview/templates/base-extend.html
+-rw-r--r--   0 adamj     (1000) adamj     (1000)     4910 2023-06-08 08:49:05.000000 pcvs-0.7.0/pcvs/webview/templates/base.html
+-rw-r--r--   0 adamj     (1000) adamj     (1000)     2785 2023-06-08 08:49:05.000000 pcvs-0.7.0/pcvs/webview/templates/brief.html
+-rw-r--r--   0 adamj     (1000) adamj     (1000)     2741 2023-06-08 08:49:05.000000 pcvs-0.7.0/pcvs/webview/templates/detailed_view.html
+-rw-r--r--   0 adamj     (1000) adamj     (1000)       70 2023-06-08 08:49:05.000000 pcvs-0.7.0/pcvs/webview/templates/diff.html
+-rw-r--r--   0 adamj     (1000) adamj     (1000)     2159 2023-06-08 08:49:05.000000 pcvs-0.7.0/pcvs/webview/templates/list_view.html
+-rw-r--r--   0 adamj     (1000) adamj     (1000)     2661 2023-06-08 08:49:05.000000 pcvs-0.7.0/pcvs/webview/templates/main.html
+-rw-r--r--   0 adamj     (1000) adamj     (1000)     2173 2023-06-08 08:49:05.000000 pcvs-0.7.0/pcvs/webview/templates/session_main.html
+-rw-r--r--   0 adamj     (1000) adamj     (1000)      287 2023-06-08 08:49:05.000000 pcvs-0.7.0/pcvs/webview/templates/tbw.html
+drwxr-xr-x   0 adamj     (1000) adamj     (1000)        0 2023-06-09 10:15:05.000000 pcvs-0.7.0/pcvs.egg-info/
+-rw-r--r--   0 adamj     (1000) adamj     (1000)     3087 2023-06-09 10:15:05.000000 pcvs-0.7.0/pcvs.egg-info/PKG-INFO
+-rw-r--r--   0 adamj     (1000) adamj     (1000)     4199 2023-06-09 10:15:05.000000 pcvs-0.7.0/pcvs.egg-info/SOURCES.txt
+-rw-r--r--   0 adamj     (1000) adamj     (1000)        1 2023-06-09 10:15:05.000000 pcvs-0.7.0/pcvs.egg-info/dependency_links.txt
+-rw-r--r--   0 adamj     (1000) adamj     (1000)      148 2023-06-09 10:15:05.000000 pcvs-0.7.0/pcvs.egg-info/entry_points.txt
+-rw-r--r--   0 adamj     (1000) adamj     (1000)      117 2023-06-09 10:15:05.000000 pcvs-0.7.0/pcvs.egg-info/requires.txt
+-rw-r--r--   0 adamj     (1000) adamj     (1000)       11 2023-06-09 10:15:05.000000 pcvs-0.7.0/pcvs.egg-info/top_level.txt
+-rw-r--r--   0 adamj     (1000) adamj     (1000)      152 2023-06-08 08:49:05.000000 pcvs-0.7.0/requirements-dev.txt
+-rw-r--r--   0 adamj     (1000) adamj     (1000)      114 2023-06-08 12:15:47.000000 pcvs-0.7.0/requirements.txt
+-rw-r--r--   0 adamj     (1000) adamj     (1000)       38 2023-06-09 10:15:05.000000 pcvs-0.7.0/setup.cfg
+-rw-r--r--   0 adamj     (1000) adamj     (1000)     1678 2023-06-08 13:46:37.000000 pcvs-0.7.0/setup.py
+drwxr-xr-x   0 adamj     (1000) adamj     (1000)        0 2023-06-09 10:15:05.000000 pcvs-0.7.0/tests/
+-rw-r--r--   0 adamj     (1000) adamj     (1000)       76 2023-06-08 08:49:05.000000 pcvs-0.7.0/tests/__init__.py
+drwxr-xr-x   0 adamj     (1000) adamj     (1000)        0 2023-06-09 10:15:05.000000 pcvs-0.7.0/tests/pcvs/
+-rw-r--r--   0 adamj     (1000) adamj     (1000)        0 2023-06-08 08:49:05.000000 pcvs-0.7.0/tests/pcvs/__init__.py
+drwxr-xr-x   0 adamj     (1000) adamj     (1000)        0 2023-06-09 10:15:05.000000 pcvs-0.7.0/tests/pcvs/cli/
+-rw-r--r--   0 adamj     (1000) adamj     (1000)        0 2023-06-08 08:49:05.000000 pcvs-0.7.0/tests/pcvs/cli/__init__.py
+-rw-r--r--   0 adamj     (1000) adamj     (1000)      264 2023-06-08 08:49:05.000000 pcvs-0.7.0/tests/pcvs/cli/conftest.py
+-rw-r--r--   0 adamj     (1000) adamj     (1000)      446 2023-06-08 08:49:05.000000 pcvs-0.7.0/tests/pcvs/cli/test_basics.py
+-rw-r--r--   0 adamj     (1000) adamj     (1000)     5931 2023-06-08 08:49:05.000000 pcvs-0.7.0/tests/pcvs/cli/test_config.py
+-rw-r--r--   0 adamj     (1000) adamj     (1000)     2767 2023-06-08 08:49:05.000000 pcvs-0.7.0/tests/pcvs/cli/test_profile.py
+-rw-r--r--   0 adamj     (1000) adamj     (1000)     1225 2023-06-08 08:49:05.000000 pcvs-0.7.0/tests/pcvs/cli/test_run.py
+-rw-r--r--   0 adamj     (1000) adamj     (1000)     1423 2023-06-08 08:49:05.000000 pcvs-0.7.0/tests/pcvs/cli/test_utilities.py
+drwxr-xr-x   0 adamj     (1000) adamj     (1000)        0 2023-06-09 10:15:05.000000 pcvs-0.7.0/tests/pcvs/converter/
+-rw-r--r--   0 adamj     (1000) adamj     (1000)        0 2023-06-08 08:49:05.000000 pcvs-0.7.0/tests/pcvs/converter/__init__.py
+-rw-r--r--   0 adamj     (1000) adamj     (1000)      284 2023-06-08 08:49:05.000000 pcvs-0.7.0/tests/pcvs/converter/conftest.py
+-rw-r--r--   0 adamj     (1000) adamj     (1000)     1155 2023-06-08 08:49:05.000000 pcvs-0.7.0/tests/pcvs/converter/test_converter.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `pcvs-0.6.0/AUTHORS` & `pcvs-0.7.0/AUTHORS`

 * *Files identical despite different names*

### Comparing `pcvs-0.6.0/COPYING` & `pcvs-0.7.0/COPYING`

 * *Files identical despite different names*

### Comparing `pcvs-0.6.0/PKG-INFO` & `pcvs-0.7.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pcvs
-Version: 0.6.0
+Version: 0.7.0
 Home-page: https://pcvs.io/
 Author: Julien Adam
 Author-email: adamj@paratools.com
 Maintainer: Julien Adam
 Maintainer-email: adamj@paratools.com
 License: CeCILL-C
 Project-URL: Source Code, https://github.com/cea-hpc/pcvs.git/
@@ -16,79 +16,66 @@
 Description-Content-Type: text/markdown
 License-File: COPYING
 License-File: AUTHORS
 
 PCVS Documentation
 ==================
 
-## About
-
 Parallel Computing Validation System (PCVS) is a Validation Orchestrator
 designed by and for software at scale. Its primary target is HPC applications &
 runtimes but can flawlessly address smaller use cases. PCVS can help users to
 create their test scenarios and reuse them among multiples implementations, an
 high value when it comes to validating Programmation standards (like APIs &
 ABIs). No matter the number of programs, benchmarks, languages, or tech
 non-regression bases use, PCVS gathers in a single execution, and, with a focus
 on interacting with HPC batch managers efficiently, run jobs concurrently to
 reduce the time-to-result overall. Through basic YAML-based configuration files,
 PCVS handles more than hundreds of thousands of tests and helps developers to
 ensure code production is moving forward.
 
-PCVS is documented through ReStructuredText. which can be found under the
-`/docs` directory. A built version can be found at (https://pcvs.readthedocs.io)
-
 
 ## Quick installation guide
 
 A more detailed guide to install PCVS can be found in the appropriate
 documentation, here is a quick overview to set up and test the framework.
 
-.. code-block:: bash
+    # considering python3.7+
+    $ pip3 install -r requirements.txt
+    # for dev/testing purposes, use:
+    $ pip3 install -r requirements-dev.txt
+    $ pip3 install pcvs
+    # basic tests:
+    $ tox
+    # OR
+    $ coverage run
 
-	# considering python3.5+
-	$ pip3 install -r requirements.txt
-	# for dev/testing purposes, use:
-	$ pip3 install -r requirements-dev.txt
-	$ pip3 install pcvs
-	# basic tests:
-	$ tox
-	# OR
-	$ coverage run
 
 ## Complete documentation
 
 PCVS documentation is currently in active progress. Feel free to redistribute
 comments and/or notes to the dev team about what should be more covered.
 Multiple documentation can be generated from this repo:
 
 * the CLI is managed and documented through ``click``. The manpages can be
   automatically built with the third-party tool ``click-man`` (not a dep,
   should be installed manually). Note that these manpages may not contain more
   information than the content of each ``--help`` command.
 * The general documentation (readthedocs.io-formatted) through ``sphinx``, able
-  to generate multiple formats:
-
-.. code-block:: bash
-
-	$ pip3 install -r requirements-dev.txt
-	$ make -C docs/source # will list available doc formats
-	$ make -C docs/source man  # global documentation as man pages (not CLI)
-	$ make -C docs/source html  # readthedocs-based
+  to generate multiple formats. A built version can be found [here](https://pcvs.readthedocs.io).
 
 ## Contributions
 
 A guide about contributing to PCVS can be found in the 
 [`CONTRIBUTING`](docs/source/contribution.rst) section of the documentation.
 
 ## Authors
 
 This work is currently supported by the French Alternative Energies and Atomic
 Energy Commission (CEA). For any question and/or remarks, please contact :
 
 * Julien JAEGER <julien.jaeger@cea.fr>
+* Julien ADAM <julien.adam@paratools.com>
 
-
-## License
+## Licensing
 
 PCVS is released under the [CeCILL-C Free Software
-License.](https://cecill.info/licences/Licence_CeCILL-C_V1-en.txt)
+License.](https://cecill.info/licences/Licence_CeCILL-C_V1-en.txt).
```

### Comparing `pcvs-0.6.0/README.md` & `pcvs-0.7.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,75 +1,62 @@
 PCVS Documentation
 ==================
 
-## About
-
 Parallel Computing Validation System (PCVS) is a Validation Orchestrator
 designed by and for software at scale. Its primary target is HPC applications &
 runtimes but can flawlessly address smaller use cases. PCVS can help users to
 create their test scenarios and reuse them among multiples implementations, an
 high value when it comes to validating Programmation standards (like APIs &
 ABIs). No matter the number of programs, benchmarks, languages, or tech
 non-regression bases use, PCVS gathers in a single execution, and, with a focus
 on interacting with HPC batch managers efficiently, run jobs concurrently to
 reduce the time-to-result overall. Through basic YAML-based configuration files,
 PCVS handles more than hundreds of thousands of tests and helps developers to
 ensure code production is moving forward.
 
-PCVS is documented through ReStructuredText. which can be found under the
-`/docs` directory. A built version can be found at (https://pcvs.readthedocs.io)
-
 
 ## Quick installation guide
 
 A more detailed guide to install PCVS can be found in the appropriate
 documentation, here is a quick overview to set up and test the framework.
 
-.. code-block:: bash
+    # considering python3.7+
+    $ pip3 install -r requirements.txt
+    # for dev/testing purposes, use:
+    $ pip3 install -r requirements-dev.txt
+    $ pip3 install pcvs
+    # basic tests:
+    $ tox
+    # OR
+    $ coverage run
 
-	# considering python3.5+
-	$ pip3 install -r requirements.txt
-	# for dev/testing purposes, use:
-	$ pip3 install -r requirements-dev.txt
-	$ pip3 install pcvs
-	# basic tests:
-	$ tox
-	# OR
-	$ coverage run
 
 ## Complete documentation
 
 PCVS documentation is currently in active progress. Feel free to redistribute
 comments and/or notes to the dev team about what should be more covered.
 Multiple documentation can be generated from this repo:
 
 * the CLI is managed and documented through ``click``. The manpages can be
   automatically built with the third-party tool ``click-man`` (not a dep,
   should be installed manually). Note that these manpages may not contain more
   information than the content of each ``--help`` command.
 * The general documentation (readthedocs.io-formatted) through ``sphinx``, able
-  to generate multiple formats:
-
-.. code-block:: bash
-
-	$ pip3 install -r requirements-dev.txt
-	$ make -C docs/source # will list available doc formats
-	$ make -C docs/source man  # global documentation as man pages (not CLI)
-	$ make -C docs/source html  # readthedocs-based
+  to generate multiple formats. A built version can be found [here](https://pcvs.readthedocs.io).
 
 ## Contributions
 
 A guide about contributing to PCVS can be found in the 
 [`CONTRIBUTING`](docs/source/contribution.rst) section of the documentation.
 
 ## Authors
 
 This work is currently supported by the French Alternative Energies and Atomic
 Energy Commission (CEA). For any question and/or remarks, please contact :
 
 * Julien JAEGER <julien.jaeger@cea.fr>
+* Julien ADAM <julien.adam@paratools.com>
 
-
-## License
+## Licensing
 
 PCVS is released under the [CeCILL-C Free Software
-License.](https://cecill.info/licences/Licence_CeCILL-C_V1-en.txt)
+License.](https://cecill.info/licences/Licence_CeCILL-C_V1-en.txt).
```

### Comparing `pcvs-0.6.0/pcvs/backend/bank.py` & `pcvs-0.7.0/pcvs/backend/bank.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import fcntl
+import json
 import os
 import tarfile
 import tempfile
 import time
-import json
 from typing import Dict, List, Optional
 
 from ruamel.yaml import YAML
 
-from pcvs import NAME_BUILD_CONF_FN, NAME_BUILD_RESDIR, PATH_BANK
+from pcvs import NAME_BUILD_CONF_FN, NAME_BUILD_RESDIR, PATH_BANK, dsl
+from pcvs.helpers import utils
 from pcvs.helpers import git
-from pcvs.helpers.exceptions import BankException
+from pcvs.orchestration.publishers import BuildDirectoryManager
+from pcvs.helpers.exceptions import BankException, CommonException
 from pcvs.helpers.system import MetaDict
-from pcvs import dsl
 
 #: :var BANKS: list of available banks when PCVS starts up
 #: :type BANKS: dict, keys are bank names, values are file path
 BANKS: Dict[str, str] = dict()
 
 
 class Bank(dsl.Bank):
@@ -56,40 +57,46 @@
         ``B`` represents the "default" project" where data will be manipulated.
 
         :param path: location of the bank repo (on disk), defaults to None
         :type path: str, optional
         :param token: name & default project to manipulate, defaults to ""
         :type token: str
         """
-        self._dflt_proj = None
-        self._name = None
-        self._config: Optional[MetaDict] = None
-        
+        self._dflt_proj: Optional[str] = None
+        self._name: Optional[str] = None
+        self._path: str = path
+
+        global BANKS
+
         # split name & default-proj from token
         array: List[str] = token.split('@', 1)
         if len(array) > 1:
-            self._dflt_proj  = array[1]
+            self._dflt_proj = array[1]
         self._name = array[0]
 
-        global BANKS
-        self._path = path
         if self.exists():
             if self.name_exist():
                 path = BANKS[self._name.lower()]
             else:
                 for k, v in BANKS.items():
                     if v == path:
                         self._name = k
                         break
-        
-        super().__init__(path, self._dflt_proj )
-    
+
+        super().__init__(path, self._dflt_proj)
+
     @property
-    def default_project(self):
-        return "unkwown" if not self._dflt_proj else self._dflt_proj
+    def default_project(self) -> str:
+        """
+        Get project set as default when none are provided.
+
+        :return: the project name (as a Ref branch)
+        :rtype: str
+        """
+        return "unknown" if not self._dflt_proj else self._dflt_proj
 
     @property
     def prefix(self) -> Optional[str]:
         """Get path to bank directory.
 
         :return: absolute path to directory
         :rtype: str
@@ -99,15 +106,15 @@
     @property
     def name(self) -> str:
         """Get bank name.
 
         :return: the exact label (without default-project suffix)
         :rtype: str
         """
-        return self._name
+        return self._name if self._name else ""
 
     def exists(self) -> bool:
         """Check if the bank is stored in ``PATH_BANK`` file.
 
         Verification is made either on name **or** path.
 
         :return: True if both the bank exist and globally registered
@@ -117,145 +124,186 @@
 
     def name_exist(self) -> bool:
         """Check if the bank name is registered into ``PATH_BANK`` file.
 
         :return: True if the name (lowered) is in the keys()
         :rtype: bool
         """
-        return self._name.lower() in BANKS.keys()
+        return self._name.lower() in BANKS.keys() if self._name else False
 
     def path_exist(self) -> bool:
         """Check if the bank path is registered into ``PATH_BANK`` file.
 
         :return: True if the path is known.
         :rtype: bool
         """
         return self._path in BANKS.values()
-        
+
     def __str__(self) -> str:
         """Stringification of a bank.
 
         :return: a combination of name & path
         :rtype: str
         """
         return str({self._name: self._path})
 
-    def show(self, stringify=False) -> None:
+    def show(self, stringify: bool = False) -> Optional[str]:
         """Print the bank on stdout.
 
         .. note::
             This function does not use :class:`log.IOManager`
         """
         string = ["Projects contained in bank '{}':".format(self._path)]
         # browse references
         for project, series in self.list_all().items():
-            string.append("- {:<8}: {} distinct testsuite(s)".format(project, len(series)))
+            string.append(
+                "- {:<8}: {} distinct testsuite(s)".format(project, len(series)))
             for s in series:
                 string.append("  * {}: {} run(s)".format(s.name, len(s)))
 
         if stringify:
             return "\n".join(string)
         else:
             print("\n".join(string))
 
     def __del__(self) -> None:
-        """Close the bank."""
+        """
+        Close / disconnet a bank (releasing lock)
+        """
         self.disconnect()
 
     def save_to_global(self) -> None:
         """Store the current bank into ``PATH_BANK`` file."""
         global BANKS
         if self._name in BANKS:
             self._name = os.path.basename(self._path).lower()
         add_banklink(self._name, self._path)
-        
-    def load_config_from_str(self, s: str) -> None:
-        """Load the configuration data associated with the archive to process.
-
-        :param s: the configuration data
-        :type s: str
-        """
-        self._config = MetaDict(YAML(typ='safe').load(s))
-        
-    def load_config_from_dict(self, s: dict) -> None:
-        """TODO:
-        """
-        self._config = MetaDict(s)
 
-    def load_config_from_file(self, path: str) -> None:
-        """Load the configuration file associated with the archive to process.
-
-        :param path: the configuration file path
-        :type path: str
-        """
-        with open(os.path.join(path, NAME_BUILD_CONF_FN), 'r') as fh:
-            self._config = MetaDict(YAML(typ='safe').load(fh))
-
-    def save_from_buildir(self, tag: str, buildpath: str) -> None:
+    def save_from_buildir(self, tag: str, buildpath: str, msg: str=None) -> None:
         """Extract results from the given build directory & store into the bank.
 
         :param tag: overridable default project (if different)
         :type tag: str
         :param buildpath: the directory where PCVS stored results
         :type buildpath: str
         """
-        self.load_config_from_file(buildpath)
-        rawdata_dir = os.path.join(buildpath, NAME_BUILD_RESDIR)
+        hdl = BuildDirectoryManager(buildpath)
+        hdl.load_config()
+        hdl.init_results()
         
-        seriename = self.build_target_branch_name(tag)
+        seriename = self.build_target_branch_name(tag, hdl.config.validation.pf_hash)
         serie = self.get_serie(seriename)
-        
-        if not serie:
+        if serie is None:
             serie = self.new_serie(seriename)
-            
+
         run = dsl.Run(from_serie=serie)
         metadata = {'cnt': {}}
-        
-        for result_file in os.listdir(rawdata_dir):
-            d = {}
-            with open(os.path.join(rawdata_dir, result_file), 'r') as fh:
-                data = MetaDict(json.load(fh))
-                # TODO: validate
-            for elt in data['tests']:
-                name = elt['id']['fq_name']
-                state = str(elt['result']['state'])
-                metadata['cnt'].setdefault(state, 0)
-                metadata['cnt'][state] += 1
-                d[name] = elt
-                
-            run.update_flatdict(d)
-        
+
+        for job in hdl.results.browse_tests():
+            metadata['cnt'].setdefault(str(job.state), 0)
+            metadata['cnt'][str(job.state)] += 1
+            run.update(job.name, job.to_json())
+            
         self.set_id(
-            an=self._config.validation.author.name,
-            am=self._config.validation.author.email,
+            an=hdl.config.validation.author.name,
+            am=hdl.config.validation.author.email,
             cn=git.get_current_username(),
             cm=git.get_current_usermail()
         )
+        
+        run.update(".pcvs-cache/conf.json", hdl.config.dump_for_export())
 
-        serie.commit(run, metadata=metadata, timestamp=int(self._config.validation.datetime.timestamp()))
+        serie.commit(run, metadata=metadata, msg=msg, timestamp=int(
+            hdl.config.validation.datetime.timestamp()))
 
-    def save_from_archive(self, tag: str, archivepath: str) -> None:
+    def save_from_archive(self, tag: str, archivepath: str, msg: str=None) -> None:
         """Extract results from the archive, if used to export results.
 
         This is basically the same as :func:`BanK.save_from_buildir` except
         the archive is extracted first.
 
         :param tag: overridable default project (if different)
         :type tag: str
         :param archivepath: archive path
         :type archivepath: str
         """
-        assert(os.path.isfile(archivepath))
+        assert (os.path.isfile(archivepath))
 
         with tempfile.TemporaryDirectory() as tarpath:
             tarfile.open(os.path.join(archivepath)).extractall(tarpath)
-            self.save_from_buildir(
-                tag, os.path.join(tarpath, "save_for_export"))
+            d = [x for x in os.listdir(tarpath) if x.startswith("pcvsrun_")]
+            assert(len(d) == 1)
+            self.save_from_buildir(tag, os.path.join(tarpath, d[0]), msg=msg)
+            
+    def save_new_run_from_instance(self, target_project: str, hdl: BuildDirectoryManager, msg: str=None) -> None:
+        """
+        Create a new node into the bank for the given project, based on the open
+        result handler.
+
+        :param target_project: valid project (=branch)
+        :type target_project: str
+        :param hdl: the result build directory handler
+        :type hdl: class:`BuildDirectoryManager`
+        """
+        seriename = self.build_target_branch_name(target_project, hdl.config.validation.pf_hash)
+        serie = self.get_serie(seriename)
+        metadata = {'cnt': {}}
+        
+        if serie is None:
+            serie = self.new_serie(seriename)
+        
+        #TODO: populate the run with build-dir content
+        #TODO: add metadata to hidden root directory
+        # Init a new fun
+        run = dsl.Run(from_serie=serie)
 
-    def build_target_branch_name(self, tag: str=None, hash: str=None) -> str:
+        # now use the handle to populate the bank
+        # We chose to make the layout slightly different between
+        # runs & banks as the `git-diff` does not permit to store
+        # other than a JSON file per test output (yet) :(
+        # Still, an hidden root directory will store aliases to easily
+        # maps tests to their on-disk counterparts.
+        d = dict()
+        for job in hdl.results.browse_tests():
+            d[job.name] = job.to_json()
+            metadata['cnt'].setdefault(str(job.state), 0)
+            metadata['cnt'][str(job.state)] += 1
+    
+        run.update_flatdict(d)
+        
+        self.set_id(
+            an=hdl.config.validation.author.name,
+            am=hdl.config.validation.author.email,
+            cn=git.get_current_username(),
+            cm=git.get_current_usermail()
+        )
+        
+        run.update(".pcvs-cache/conf.json", hdl.config)
+        
+        serie.commit(run, metadata=metadata, msg=msg, timestamp=int(
+            hdl.config.validation.datetime.timestamp()))
+
+    def save_new_run(self, target_project: str, path: str) -> None:
+        if not utils.check_is_build_or_archive(path):
+            raise CommonException.NotPCVSRelated(
+                reason="Invalid path, not PCVS-related",
+                dbg_info={"path": path}
+            )
+
+        if utils.check_is_archive(path):
+            # convert to prefix
+            # update path according to it
+            hdl = BuildDirectoryManager.load_from_archive(path)
+        else:
+            hdl = BuildDirectoryManager(build_dir=path)
+            hdl.load_config()
+
+        self.save_new_run_from_instance(target_project, hdl)
+        
+    def build_target_branch_name(self, tag: str = None, hash: str = None) -> str:
         """Compute the target branch to store data.
 
         This is used to build the exact Git branch name based on:
             * default-proj
             * unique profile hash, used to run the validation
 
         :param tag: overridable default-proj (if different)
@@ -264,34 +312,37 @@
         :rtype: str
         """
         # a reference (lightweight branch) is tracking a whole test-suite
         # history, there are managed directly
         # TODO: compute the proper name for the current test-suite
         if tag is None:
             tag = self.default_project
-        if hash is None:
-            hash = self._config.validation.pf_hash
         return "{}/{}".format(tag, hash)
 
     def __repr__(self) -> dict:
         """Bank representation.
 
         :return: a dict-based representation
         :rtype: dict
         """
         return {
             'rootpath': self._path,
             'name': self._name
         }
-        
+
     def get_count(self):
-        """TODO:
+        """
+        Get the number of projects managed by this bank handle.
+
+        :return: number of projects
+        :rtype: int
         """
         return len(self.list_projects())
 
+
 def init() -> None:
     """Bank interface detection.
 
     Called when program initializes. Detects defined banks in ``PATH_BANK``
     """
     global BANKS
     try:
```

### Comparing `pcvs-0.6.0/pcvs/backend/config.py` & `pcvs-0.7.0/pcvs/backend/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 import base64
 import glob
 import os
+from typing import Dict, List, Union
 
 import click
 from ruamel.yaml import YAML
 
-from pcvs import PATH_INSTDIR
-from pcvs.helpers import log, system, utils
+from pcvs import PATH_INSTDIR, io
+from pcvs.helpers import system, utils
 from pcvs.helpers.exceptions import ConfigException
 from pcvs.helpers.system import MetaDict
 
 CONFIG_BLOCKS = ['compiler', 'runtime', 'machine', 'criterion', 'group']
 CONFIG_EXISTING = dict()
 
 
 def init() -> None:
     """Load configuration tree available on disk.
 
     This function is called when PCVS starts to load 3-scope configuration
     trees.
     """
+    if hasattr(init, 'done'):
+        return
+
     global CONFIG_BLOCKS, CONFIG_EXISTING
     CONFIG_EXISTING = {}
 
     # this first loop defines configuration order
     for block in CONFIG_BLOCKS:
         CONFIG_EXISTING[block] = {}
         priority_paths = utils.storage_order()
@@ -31,17 +35,18 @@
         for token in priority_paths:  # reverse order (overriding)
             CONFIG_EXISTING[block][token] = []
             for config_file in glob.glob(os.path.join(utils.STORAGES[token],
                                                       block,
                                                       "*.yml")):
                 CONFIG_EXISTING[block][token].append(
                     (os.path.basename(config_file)[:-4], config_file))
+    init.done = True
 
 
-def list_blocks(kind, scope=None):
+def list_blocks(kind, scope=None) -> Union[List[str], Dict[str, List[str]]]:
     """Get available configuration blocks, as present on disk.
 
     :param kind: configBlock kind (see ``CONFIG_BLOCKS`` for possible values)
     :type kind: str, one of ``CONFIG_BLOCKS`` values
     :param scope: where the configblocks is located, defaults to None
     :type scope: 'user', 'global' or 'local', optional
     :return: list blocks with specified kind, restricted by scope (if any)
@@ -51,27 +56,27 @@
     assert (scope in utils.STORAGES.keys() or scope is None)
     if scope is None:
         return CONFIG_EXISTING[kind]
     else:
         return CONFIG_EXISTING[kind][scope]
 
 
-def list_templates():
+def list_templates() -> List[str]:
     """List available templates to be used for boostraping config. blocks.
 
     :return: a list of valid templates.
     :rtype: list"""
     array = list()
     for f in os.listdir(os.path.join(PATH_INSTDIR, "templates/config")):
         array.append(os.path.splitext(f)[0])
 
     return array
 
 
-def check_valid_kind(s):
+def check_valid_kind(s) -> bool:
     """Assert the parameter is a valid kind.
 
     Kind are defined by ``CONFIG_BLOCKS`` module attribute.
 
     :param s: the kind to validate
     :type s: str
     :raises BadTokenError: Kind is None
@@ -121,14 +126,16 @@
         :param kind: which component to initialize this basicblock with
         :type kind: str, one of ``CONFIG_BLOCKS`` values
         :param name: block name
         :type name: str
         :param scope: block scope, defaults to 'local'
         :type scope: str, optional
         """
+        init()
+
         check_valid_kind(kind)
         utils.check_valid_scope(scope)
         self._kind = kind
         self._name = name
         self._details = {}
         self._scope = scope
         self._file = None
@@ -221,15 +228,15 @@
 
         :return: a regular dict() representing the config blocK
         :rtype: dict
         """
         self.load_from_disk()
         return MetaDict(self._details).to_dict()
 
-    def check(self) -> None:
+    def check(self, allow_conversion=True) -> None:
         """Validate a single configuration block according to its scheme."""
         system.ValidationScheme(self._kind).validate(
             self._details, filepath=self.full_name)
 
     def load_from_disk(self) -> None:
         """load the configuration file to populate the current object.
 
@@ -289,39 +296,39 @@
 
         :param clone: the object to mirror
         :type clone: :class:`ConfigurationBlock`
         """
         assert (isinstance(clone, ConfigurationBlock))
         assert (clone._kind == self._kind)
         assert (not self.is_found())
-        assert(clone.is_found())
+        assert (clone.is_found())
 
         self.retrieve_file()
-        assert(not os.path.isfile(self._file))
+        assert (not os.path.isfile(self._file))
 
-        log.manager.info("Compute target prefix: {}".format(self._file))
+        io.console.info("Compute target prefix: {}".format(self._file))
         self._details = clone._details
 
     def delete(self) -> None:
         """Delete a configuration block from disk"""
         assert (self.is_found())
         assert (os.path.isfile(self._file))
 
-        log.manager.info("remove {} from '{} ({})'".format(
+        io.console.info("remove {} from '{} ({})'".format(
             self._name, self._kind, self._scope))
         os.remove(self._file)
 
     def display(self) -> None:
         """Configuration block pretty printer"""
-        log.manager.print_header("Configuration display")
-        log.manager.print_section("Scope: {}".format(self._scope.capitalize()))
-        log.manager.print_section("Path: {}".format(self._file))
-        log.manager.print_section("Details:")
+        io.console.print_header("Configuration display")
+        io.console.print_section("Scope: {}".format(self._scope.capitalize()))
+        io.console.print_section("Path: {}".format(self._file))
+        io.console.print_section("Details:")
         for k, v in self._details.items():
-            log.manager.print_item("{}: {}".format(k, v))
+            io.console.print_item("{}: {}".format(k, v))
 
     def edit(self) -> None:
         """Open the current block for edition.
 
         :raises Exception: Something occured on the edited version.
         :param e: the EDITOR to use instead of default.
         :type e: str
@@ -333,24 +340,21 @@
 
         with open(self._file, 'r') as fh:
             stream = fh.read()
 
         edited_stream = click.edit(
             stream, extension=".yml", require_save=True)
         if edited_stream is not None:
+            edited_yaml = MetaDict(YAML(typ='safe').load(edited_stream))
+            system.ValidationScheme(self._kind).validate(edited_yaml)
+            self.fill(edited_yaml)
+            self.flush_to_disk()
             try:
-                edited_yaml = MetaDict(YAML(typ='safe').load(edited_stream))
-                system.ValidationScheme(self._kind).validate(edited_yaml)
-                self.fill(edited_yaml)
-                self.flush_to_disk()
+                self.check()
             except Exception as e:
-                fname = "./rej{}-{}.yml".format(
-                    random.randint(0, 1000), self.full_name)
-                with open(fname, "w") as fh:
-                    fh.write(edited_stream)
                 raise e
 
     def edit_plugin(self) -> None:
         """Special case to handle 'plugin' key for 'runtime' blocks.
 
         This allows to edit a de-serialized version of the 'plugin' field. By
         default, data are stored as a base64 string. In order to let user edit
```

### Comparing `pcvs-0.6.0/pcvs/backend/profile.py` & `pcvs-0.7.0/pcvs/backend/profile.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,19 @@
+import subprocess
 import base64
 import glob
 import os
 import random
 
 import click
 from ruamel.yaml import YAML
 
-from pcvs import PATH_INSTDIR
+from pcvs import PATH_INSTDIR, io
 from pcvs.backend import config
-from pcvs.helpers import git, log, system, utils
+from pcvs.helpers import git, system, utils
 from pcvs.helpers.exceptions import (ConfigException, ProfileException,
                                      ValidationException)
 from pcvs.helpers.system import MetaDict
 
 PROFILE_EXISTING = dict()
 
 
@@ -212,15 +213,15 @@
         if not self._exists:
             raise ProfileException.NotFoundError(self._name)
         self._retrieve_file()
 
         if not os.path.isfile(self._file):
             raise ProfileException.NotFoundError(self._file)
 
-        log.manager.debug("Load {} ({})".format(self._name, self._scope))
+        io.console.debug("Load {} ({})".format(self._name, self._scope))
         with open(self._file) as f:
             self._details = MetaDict(YAML(typ='safe').load(f))
 
     def load_template(self, name="default"):
         """Populate the profile from templates of 5 basic config. blocks.
 
         Filepath still need to be determined via `retrieve_file()` call.
@@ -232,36 +233,64 @@
         if not os.path.isfile(filepath):
             raise ProfileException.NotFoundError(
                 "{} is not a valid base name.\nPlease use pcvs profile list --all".format(name))
 
         with open(filepath, "r") as fh:
             self.fill(YAML(typ='safe').load(fh))
 
-    def check(self):
+    def check(self, allow_legacy=True):
         """Ensure profile meets scheme requirements, as a concatenation of 5
         configuration block schemes.
 
         :raises FormatError: A 'kind' is missing from
             profile OR incorrect profile.
         """
-        for kind in config.CONFIG_BLOCKS:
-            #if kind not in self._details:
-            #    raise ValidationException.FormatError(
-            #        "Missing '{}' in profile".format(kind))
-            system.ValidationScheme(kind).validate(
-                self._details[kind], filepath=self._name)
-
+        try:
+            err_dbg = list()
+            for k in self._details.keys():
+                if k not in config.CONFIG_BLOCKS:
+                    err_dbg.append(k)
+            if err_dbg:
+                raise ValidationException.FormatError("Unknown kind in Profile", invalid_kinds=err_dbg)
+
+            for kind in config.CONFIG_BLOCKS:
+                # if kind not in self._details:
+                #    raise ValidationException.FormatError(
+                #        "Missing '{}' in profile".format(kind))
+                system.ValidationScheme(kind).validate(
+                    self._details[kind], filepath=self._name)
+        except ValidationException.FormatError as e:
+            if not allow_legacy:
+                raise e
+            # Is the profile a legacy format ?
+            # Attempt to convert it on the fly
+            proc = subprocess.Popen(
+                "pcvs_convert '{}' --stdout -k profile --skip-unknown".format(
+                    self._file),
+                stderr=subprocess.DEVNULL,
+                stdout=subprocess.PIPE,
+                shell=True)
+            
+            fds = proc.communicate()
+            if proc.returncode != 0:
+                raise e
+            converted_data = YAML(typ='safe').load(fds[0].decode('utf-8'))
+            self.fill(converted_data)
+            self.check(allow_legacy=False)
+            io.console.warning("Legacy format for profile '{}'".format(self._name))
+            io.console.warning("Please consider updating it with `pcvs_convert -k profile`")
+            
     def flush_to_disk(self):
         """Write down profile to disk.
 
         Also, ensure the filepath is valid and profile content is compliant with
         schemes.
         """
         self._retrieve_file()
-        self.check()
+        #self.check()
 
         # just in case the block subprefix does not exist yet
         prefix_file = os.path.dirname(self._file)
         if not os.path.isdir(prefix_file):
             os.makedirs(prefix_file, exist_ok=True)
 
         with open(self._file, 'w') as f:
@@ -271,36 +300,36 @@
         """Duplicate a valid profile into the current one.
 
         :param clone: a valid profile object
         :type clone: :class:`Profile`
         """
         self._retrieve_file()
 
-        log.manager.info("Compute target prefix: {}".format(self._file))
-        assert(not os.path.isfile(self._file))
+        io.console.info("Compute target prefix: {}".format(self._file))
+        assert (not os.path.isfile(self._file))
         self._details = clone._details
 
     def delete(self):
         """Remove the current profile from disk.
 
         It does not destroy the Python object, though.
         """
-        log.manager.info("delete {}".format(self._file))
+        io.console.info("delete {}".format(self._file))
         os.remove(self._file)
 
     def display(self):
         """Display profile data into stdout/file.
         """
-        log.manager.print_header("Profile View")
-        log.manager.print_section("Scope: {}".format(self._scope.capitalize()))
-        log.manager.print_section("Profile details:")
+        io.console.print_header("Profile View")
+        io.console.print_section("Scope: {}".format(self._scope.capitalize()))
+        io.console.print_section("Profile details:")
         if self._details:
-            log.manager.print_section("Details:")
+            io.console.print_section("Details:")
             for k, v in self._details.items():
-                log.manager.print_item("{}: {}".format(k, v))
+                io.console.print_item("{}: {}".format(k, v))
 
     def edit(self):
         """Open the editor to manipulate profile content.
 
         :param e: an editor program to use instead of defaults
         :type e: str
 
@@ -319,25 +348,22 @@
 
         with open(self._file, 'r') as fh:
             stream = fh.read()
 
         edited_stream = click.edit(
             stream, extension=".yml", require_save=True)
         if edited_stream is not None:
+            edited_yaml = MetaDict(YAML(typ='safe').load(edited_stream))
+            self.fill(edited_yaml)
+            self.flush_to_disk()
             try:
-                edited_yaml = MetaDict(YAML(typ='safe').load(edited_stream))
-                self.fill(edited_yaml)
                 self.check()
             except Exception as e:
-                fname = "./rej{}-{}.yml".format(
-                    random.randint(0, 1000), self.full_name)
-                with open(fname, "w") as fh:
-                    fh.write(edited_stream)
                 raise e
-            self.flush_to_disk()
+            
 
     def edit_plugin(self):
         """Edit the 'runtime.plugin' section of the current profile.
 
         :param e: an editor program to use instead of defaults
         :type e: str
 
@@ -373,18 +399,14 @@
             edited_code = click.edit(
                 plugin_code, extension=".py", require_save=True)
             if edited_code is not None:
                 self._details['runtime']['plugin'] = base64.b64encode(
                     edited_code.encode('utf-8'))
                 self.flush_to_disk()
         except Exception as e:
-            fname = "./rej{}-{}-plugin.yml".format(
-                random.randint(0, 1000), self.full_name)
-            with open(fname, "w") as fh:
-                fh.write(edited_code)
             raise e
 
     def split_into_configs(self, prefix, blocklist, scope=None):
         """Convert the given profile into a list of basic blocks.
 
         This is the reverse operation of creating a profile (not the 'opposite').
```

### Comparing `pcvs-0.6.0/pcvs/backend/session.py` & `pcvs-0.7.0/pcvs/backend/session.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from datetime import datetime
 from enum import IntEnum
 from multiprocessing import Process
 
 from ruamel.yaml import YAML
 from ruamel.yaml.main import yaml_object
 
-from pcvs import PATH_SESSION
+from pcvs import PATH_SESSION, io
 from pcvs.helpers import log, utils
 
 yml = YAML()
 
 
 def unlock_session_file():
     """Release the lock after manipulating the session.yml file.
@@ -63,15 +63,15 @@
         # Lookup for an available session id number
         sid = all_sessions["__metadata"]["next"]
         while sid in all_sessions.keys() or sid == -1:
             sid += 1
 
         all_sessions["__metadata"]["next"] = (sid + 1) % 1000000
 
-        assert(sid not in all_sessions.keys())
+        assert (sid not in all_sessions.keys())
         all_sessions[sid] = c
 
         # dump the file back
         with open(PATH_SESSION, 'w') as fh:
             yml.dump(all_sessions, fh)
     finally:
         unlock_session_file()
@@ -245,15 +245,15 @@
             :type node: Any
             :return: The session State as an object
             :rtype: :class:`Session.State`
             """
             s = constructor.construct_scalar(node)
             name, value = s.split('||')
             obj = Session.State(int(value))
-            assert(obj.name == name)
+            assert (obj.name == name)
 
             return obj
 
         def __str__(self):
             """Stringify the state.
 
             :return: the enum name.
@@ -301,15 +301,15 @@
         """Access specific data from the session stored info session.yml.
 
         :param kw: the information to retrieve. kw must be a valid key
         :type kw: str
         :return: the requested session infos if exist
         :rtype: Any
         """
-        assert(kw in self._session_infos)
+        assert (kw in self._session_infos)
         return self._session_infos[kw]
 
     def __init__(self, date=None, path="."):
         """constructor method.
 
         :param date: the start timestamp
         :type date: datetime.datetime
@@ -318,15 +318,16 @@
         """
         self._func = None
         self._rc = -1
         self._sid = -1
         # this dict is then flushed to the session.yml
         self._session_infos = {
             "path": path,
-            "io": None,
+            "log": io.console.logfile,
+            "io": io.console.outfile,
             "progress": 0,
             "state": Session.State.WAITING,
             "started": date,
             "ended": None
         }
 
     def load_from(self, sid, data):
@@ -336,48 +337,38 @@
         :type sid: int
         :param data: session infos read from file
         :type data: dict
         """
         self._sid = sid
         self._session_infos = data
 
-    def register_callback(self, callback, io_file=None):
+    def register_callback(self, callback):
         """Register the callback used as main function once the session is
         started.
 
         :param callback: function to invoke
         :type callback: Callable
-        :param io_file: Where I/O will be redirected once session is started
-        :type io_file: str, optional
         """
         self._func = callback
-        self.register_io_file(io_file)
-
-    def register_io_file(self, pathfile=None):
-        """Register the I/O file when stdout/stderr will be flushed once the
-        session is started.
-
-        :param pathfile: the path to redirect I/Os, may be None
-        :type pathfile: str, optional
-        """
-        self._session_infos['io'] = pathfile
-        self._io_file = pathfile
 
     def run_detached(self, *args, **kwargs):
         """Run the session is detached mode.
 
         Arguments are for user function only.
         :param args: user function positional arguments
         :type args: tuple
         :param kwargs user function keyword-based arguments.
         :type kwargs: tuple
 
         :return: the Session id created for this run.
         :rtype: int
         """
+        io.detach_console()
+        self._session_infos['io'] = io.console.outfile
+
         if self._func is not None:
             # some sessions can have their starting time set directly when
             # initializing the object.
             # for instance for runs, elapsed time not session time but wall time"""
             if self.property('started') == None:
                 self._session_infos['started'] = datetime.now()
 
@@ -386,28 +377,16 @@
             self._sid = store_session_to_file(self._session_infos)
 
             # run the new process
             child = Process(target=main_detached_session,
                             args=(self._sid, self._func, *args),
                             kwargs=kwargs)
 
-            # set the child IOManager before starting
-            # enable logfile but disable tty
-            # save the old manager to restore it after child starts
-            old = copy.copy(log.manager)
-            log.manager.set_logfile(enable=True, logfile=self._io_file)
-            log.manager.set_tty(enable=False)
             child.start()
-            # complete the first child, to allow this process to terminate
-            child.join()
-
-            # do not close tty, to extra info to be printed but not logged
-            log.manager = old
-            log.manager.set_logfile(enable=False)
-
+            
             return self._sid
 
     def run(self, *args, **kwargs):
         """Run the session normally, without detaching the focus.
 
         Arguments are user function ones. This function is also in charge of
         redirecting I/O properly (stdout, file, logs)
@@ -421,16 +400,14 @@
             # same as above, shifted starting time or not
             if self.property('started') == None:
                 self._session_infos['started'] = datetime.now()
 
             self._session_infos['state'] = self.State.IN_PROGRESS
             self._sid = store_session_to_file(self._session_infos)
 
-            log.manager.set_logfile(enable=True, logfile=self._io_file)
-            log.manager.set_tty(enable=True)
             # run the code
             try:
                 self._rc = self._func(*args, **kwargs)
             finally:
                 # in that mode, no information is left to users once the session
                 # is complete.
                 remove_session_from_file(self._sid)
```

### Comparing `pcvs-0.6.0/pcvs/backend/spack.py` & `pcvs-0.7.0/pcvs/backend/spack.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,42 +1,46 @@
-import pcvs
 import subprocess
+
+import pcvs
 from pcvs import testing
-from pcvs.testing.testfile import TestFile
-from pcvs.helpers.system import MetaDict
 from pcvs.helpers import utils
+from pcvs.helpers.system import MetaDict
+from pcvs.testing.testfile import TestFile
 
 
 def parse_spec_variants(specname):
     d = dict()
-    cmd = 'spack python -c \'import spack.repo; print("\\n".join(["{}:{}".format(v.name, v.allowed_values) for v in spack.repo.get("'+ specname +'").variants.values()]))\''
+    cmd = 'spack python -c \'import spack.repo; print("\\n".join(["{}:{}".format(v.name, v.allowed_values) for v in spack.repo.get("' + \
+        specname + '").variants.values()]))\''
     p = subprocess.Popen(cmd, shell=True, stdout=subprocess.PIPE)
     fds = p.communicate()
     for line in fds[0].decode().rstrip().split("\n"):
         name, val_raw = line.split(':')
         values = val_raw.split(', ')
-        
+
         d[name] = {
             "option": "{}=".format(name),
             "position": "after",
             "type": "argument",
             "subtitle": "{}=".format(name),
             "values": values
         }
     return d
 
+
 def generate_from_variants(package, label, prefix):
     data = MetaDict()
     dict_of_variants = parse_spec_variants(package)
 
     data[package].run.program = "spack install {} ".format(package)
     data[package].run.iterate.program = dict_of_variants
     data[package].run.attributes = {
-            "command_wrap": False,
-            "path_resolution": False,
-            }
+        "command_wrap": False,
+        "path_resolution": False,
+    }
 
     _, src, _, build = testing.generate_local_variables(label, prefix)
 
-    t = TestFile(file_in=src, path_out=build, data=data, label=label, prefix=prefix)
+    t = TestFile(file_in=src, path_out=build,
+                 data=data, label=label, prefix=prefix)
     t.process()
     t.flush_sh_file()
```

### Comparing `pcvs-0.6.0/pcvs/backend/utilities.py` & `pcvs-0.7.0/pcvs/backend/utilities.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import base64
+import json
 import os
 import subprocess
 import tempfile
 
-import jsonschema
-import json
-from prettytable import PrettyTable
 from ruamel.yaml import YAML, YAMLError
 
-import pcvs
+from pcvs import NAME_BUILDFILE, NAME_BUILDIR, io
+from pcvs.testing.testfile import TestFile
 from pcvs.backend import config, profile, run
-from pcvs.helpers import log, system, utils
+from pcvs.helpers import system, utils
 from pcvs.helpers.exceptions import ValidationException
 from pcvs.helpers.system import MetaDict
+from pcvs.orchestration.publishers import BuildDirectoryManager
 
 
 def locate_scriptpaths(output=None):
     """Path lookup to find all 'list_of_tests' script within a given prefix.
 
     :param output: prefix to walk through, defaults to current directory
     :type output: str, optional
@@ -52,101 +52,93 @@
     return os.path.join(
         buildir,
         'test_suite',
         prefix,
         "list_of_tests.sh"
     )
 
+
 def get_logged_output(prefix, testname):
     if prefix is None:
         prefix = os.getcwd()
-    resdir = os.path.join(
-                    utils.find_buildir_from_prefix(prefix),
-                    pcvs.NAME_BUILD_RESDIR)
+    buildir = utils.find_buildir_from_prefix(prefix)
     s = ""
-    if os.path.isdir(resdir):
-        for f in os.listdir(resdir):
-            
-            with open(os.path.join(resdir, f), 'r') as fh:
-                data = json.load(fh)
-                for job in data['tests']:
-                    if job['id']['fq_name'].startswith(testname):
-                        s += "\n#################\n### Found test-name: {}\n{}#################\n".format(
-                            job['id']['fq_name'],
-                            base64.b64decode(job['result']['output']).decode('utf-8'))
+    if buildir:
+        man = BuildDirectoryManager(build_dir=buildir)
+        man.init_results()
+        for test in man.results.retrieve_tests_by_name(name=testname):
+            s += "\n##### TEST OUTPUT #####\n### Testname: {}\n{}\n".format(
+                test.name, test.get_raw_output(encoding='utf-8'))
+        man.finalize()
     if not s:
         s = "No test named '{}' found here.".format(testname)
-        
-    return s 
-    
 
-def process_check_configs():
+    return s
+
+
+def process_check_configs(conversion=True):
     """Analyse available configurations to ensure their correctness relatively
     to their respective schemes.
 
     :return: caught errors, as a dict, where the keys is the errmsg base64
     :rtype: dict"""
     errors = dict()
-    t = PrettyTable()
-    t.field_names = ["Valid", "ID"]
-    t.align['ID'] = "l"
+    t = io.console.create_table("Configurations", ["Valid", "ID"])
 
     for kind in config.CONFIG_BLOCKS:
         for scope in utils.storage_order():
             for blob in config.list_blocks(kind, scope):
-                token = log.manager.utf('fail')
+                token = io.console.utf('fail')
                 err_msg = ""
                 obj = config.ConfigurationBlock(kind, blob[0], scope)
                 obj.load_from_disk()
 
                 try:
-                    obj.check()
-                    token = log.manager.utf('succ')
-                except jsonschema.exceptions.ValidationError as e:
-                    err_msg = base64.b64encode(str(e.message).encode('utf-8'))
+                    obj.check(allow_legacy=conversion)
+                    token = io.console.utf('succ')
+                except ValidationException.FormatError as e:
+                    err_msg = base64.b64encode(str(e.dbg).encode('utf-8'))
                     errors.setdefault(err_msg, 0)
                     errors[err_msg] += 1
-                    log.manager.debug(str(e))
+                    io.console.debug(str(e))
 
-                t.add_row([token, obj.full_name])
-    print(t)
+                t.add_row(token, obj.full_name)
+    io.console.print(t)
     return errors
 
 
-def process_check_profiles():
+def process_check_profiles(conversion=True):
     """Analyse availables profiles and check their correctness relatively to the
     base scheme.
 
     :return: list of caught errors as a dict, where keys are error msg base64
     :rtype: dict"""
-    t = PrettyTable()
+    t = io.console.create_table("Available Profile", ["valid", "ID"])
     errors = dict()
-    t.field_names = ["Valid", "ID"]
-    t.align['ID'] = "l"
 
     for scope in utils.storage_order():
         for blob in profile.list_profiles(scope):
-            token = log.manager.utf('fail')
+            token = io.console.utf('fail')
             obj = profile.Profile(blob[0], scope)
             obj.load_from_disk()
             try:
-                obj.check()
-                token = log.manager.utf('succ')
-            except jsonschema.exceptions.ValidationError as e:
-                err_msg = base64.b64encode(str(e.message).encode('utf-8'))
+                obj.check(allow_legacy=conversion)
+                token = io.console.utf('succ')
+            except ValidationException.FormatError as e:
+                err_msg = base64.b64encode(str(e.dbg).encode('utf-8'))
                 errors.setdefault(err_msg, 0)
                 errors[err_msg] += 1
-                log.manager.debug(str(e))
+                io.console.debug(str(e))
 
-            t.add_row([token, obj.full_name])
-    print(t)
+            t.add_row(token, obj.full_name)
+    io.console.print(t)
     return errors
 
 
-def process_check_setup_file(filename, prefix, run_configuration):
+def process_check_setup_file(root, prefix, run_configuration):
     """Check if a given pcvs.setup could be parsed if used in a regular process.
 
     :param filename: the pcvs.setup filepath
     :type filename: str
     :param prefix: the subtree the setup is extract from (used as argument)
     :type prefix: str
     :return: a tuple (err msg, icon to print, parsed data)
@@ -156,65 +148,37 @@
     data = None
     env = os.environ
     env.update(run_configuration)
 
     try:
         tdir = tempfile.mkdtemp()
         with utils.cwd(tdir):
-            env['pcvs_src'] = os.path.dirname(filename).replace(prefix, "")
+            env['pcvs_src'] = root
             env['pcvs_testbuild'] = tdir
-
+            
             if not os.path.isdir(os.path.join(tdir, prefix)):
                 os.makedirs(os.path.join(tdir, prefix))
             if not prefix:
                 prefix = ''
             proc = subprocess.Popen(
-                [filename, prefix], env=env, stderr=subprocess.PIPE, stdout=subprocess.PIPE)
+                [os.path.join(root, prefix, "pcvs.setup"), prefix], env=env, stderr=subprocess.PIPE, stdout=subprocess.PIPE)
             fdout, fderr = proc.communicate()
 
             if proc.returncode != 0:
                 if not fderr:
                     fderr = "Non-zero status (no stderr): {}".format(
                         proc.returncode).encode('utf-8')
                 err_msg = base64.b64encode(fderr)
             else:
                 data = fdout.decode('utf-8')
     except subprocess.CalledProcessError as e:
         err_msg = base64.b64encode(str(e.stderr).encode('utf-8'))
 
     return (err_msg, data)
 
-
-scheme = system.ValidationScheme('te')
-
-
-def process_check_yaml_stream(data):
-    """Analyze a pcvs.yml stream and check its correctness relatively to
-    standard. 
-    :param data: the stream to process
-    :type data: str
-    :return: a tuple (err_msg, load status icon, yaml format status icon)
-    :rtype: tuple
-    """
-    global scheme
-    err_msg = None
-    nb_nodes = 0
-    try:
-        stream = YAML(typ='safe').load(data)
-        scheme.validate(stream)
-        nb_nodes = len(stream.keys())
-
-    except YAMLError as e:
-        err_msg = base64.b64encode(str(e).encode('utf-8'))
-    except ValidationException.FormatError as e:
-        err_msg = base64.b64encode(str(e).encode('utf-8'))
-
-    return (err_msg, nb_nodes)
-
-
 def __set_token(token, nset=None) -> str:
     """Manage display token (job display) depending on given condition.
 
     if the condition is a success, insert the UTF 'succ' code, 'fail' otherwise.
     A custom str can be provided if the condition is neither a success or a
     failure (=None was given).
 
@@ -222,86 +186,112 @@
     :type token: bool
     :param nset: default pattern to insert
     :type nset: str, optional
     :return: the pretty-printable token
     :rtype: str
     """
     if not nset:
-        nset = log.manager.utf("none")
+        nset = io.console.utf("none")
     if token is None:
-        return log.manager.style(nset, fg="yellow", bold=True)
+        return "[yellow bold]{}[/]".format(nset)
     elif token:
-        return log.manager.style(log.manager.utf("succ"), fg="green", bold=True)
+        return "[green bold]{}[/]".format(io.console.utf("succ"))
     else:
-        return log.manager.style(log.manager.utf("fail"), fg="red", bold=True)
+        return "[red bold]{}[/]".format(io.console.utf("fail"))
 
 
-def process_check_directory(dir, pf_name="default"):
+def process_check_directory(dir, pf_name="default", conversion=True):
     """Analyze a directory to ensure defined test files are valid.
 
     :param dir: the directory to process.
     :type dir: str
     :return: a dict of caught errors
     :rtype: dict
     """
     errors = dict()
     total_nodes = 0
     pf = profile.Profile(pf_name)
     if not pf.is_found():
         pf.load_template()
     else:
         pf.load_from_disk()
+        pf.check(allow_legacy=conversion)
+    system.MetaConfig.root = system.MetaConfig()
+    system.MetaConfig.root.bootstrap_from_profile(pf.dump())
+    system.MetaConfig.root.validation.output = "/tmp"
     buildenv = run.build_env_from_configuration(pf.dump())
     setup_files, yaml_files = run.find_files_to_process(
         {os.path.basename(dir): dir})
 
-    log.manager.print_section(
-        'Analyzing: Setup{s}Output{s}test Node(s)'.format(s=log.manager.utf('sep_v')))
-
-    for _, subprefix, f in [*setup_files, *yaml_files]:
+    from rich.table import Table
+    table = Table(title="Results", expand=True, row_styles=["dim", ""])
+    table.add_column("Runnable Script", justify="center", max_width=5)
+    table.add_column("Valid", justify="center", max_width=5)
+    table.add_column("Node count", justify="center", max_width=5)
+    table.add_column("File Path", justify="left")
+    # with io.console.pager():
+    # with Live(table, refresh_per_second=4):
+    for _, subprefix, f in io.console.progress_iter([*setup_files, *yaml_files]):
         setup_ok = __set_token(None)
         yaml_ok = __set_token(None)
         nb_nodes = __set_token(None, "----")
         data = ""
         err = None
 
         if subprefix is None:
             subprefix = ""
 
         if f.endswith("pcvs.setup"):
             err, data = process_check_setup_file(
-                os.path.join(dir, subprefix, f), subprefix, buildenv)
+                dir, subprefix, buildenv)
             setup_ok = __set_token(err is None)
         else:
             with open(os.path.join(dir, subprefix, f), 'r') as fh:
                 data = fh.read()
 
         if not err:
-            err, cnt = process_check_yaml_stream(data)
-            yaml_ok = __set_token(err is None)
-            if cnt > 0:
-                nb_nodes = cnt
+            converted = None
+            dflt = None
+            err = None
+            try:
+                cur = TestFile(file_in="", path_out="", label="", prefix=subprefix)
+                cur.load_from_str(data)
+                converted = not(cur.validate(allow_conversion=conversion))
+                nb_nodes = cur.nb_descs
                 total_nodes += nb_nodes
+                success=True
+
+            except YAMLError as e:
+                err = base64.b64encode(str(e).encode('utf-8'))
+                success=False
+            except ValidationException.FormatError as e:
+                err = base64.b64encode(str(e).encode('utf-8'))
+                success=False
+                
+            if converted is True:
+                # yaml VALID but old syntax
+                # --> yellow
+                success=None
+                dflt = "{} {}".format(io.console.utf('succ'), io.console.utf('copy'))
+            yaml_ok = __set_token(success, nset=dflt)
+            
 
-        log.manager.print_item(' {}{}{}{}{}{}{}'.format(
+        table.add_row(
             setup_ok,
-            log.manager.utf('sep_v'),
             yaml_ok,
-            log.manager.utf('sep_v'),
-            log.manager.style("{:>4}".format(nb_nodes),
-                              fg="yellow", bold=True),
-            log.manager.utf('sep_v'),
-            "./" if not subprefix else subprefix), with_bullet=False)
+            "{:>4}" .format(nb_nodes),
+            "./" if not subprefix else subprefix)
 
         if err:
-            log.manager.info("FAILED: {}".format(
+            io.console.info("FAILED: {}".format(
                 base64.b64decode(err).decode('utf-8')))
             errors.setdefault(err, 0)
             errors[err] += 1
-    log.manager.print_item("Jobs count: {}".format(total_nodes))
+    io.console.print(table)
+    io.console.print_item("Total node count: {}".format(total_nodes))
     return errors
 
 
 class BuildSystem:
     """Manage a generic build system discovery service.
 
     :ivar _root: the root directory the discovery service is attached to.
@@ -329,28 +319,28 @@
         self._stream = MetaDict()
 
     def fill(self):
         """This function should be overriden by overriden classes.
 
         Nothing to do, by default.
         """
-        assert(False)
+        assert (False)
 
     def generate_file(self, filename="pcvs.yml", force=False):
         """Build the YAML test file, based on path introspection and build
         model.
 
         :param filename: test file suffix
         :type filename: str
         :param force: erase target file if exist.
         :type force: bool
         """
         out_file = os.path.join(self._root, filename)
         if os.path.isfile(out_file) and not force:
-            log.manager.warn(" --> skipped, already exist;")
+            io.console.warn(" --> skipped, already exist;")
             return
 
         with open(out_file, 'w') as fh:
             YAML(typ='safe').dump(self._stream.to_dict(), fh)
 
 
 class AutotoolsBuildSystem(BuildSystem):
@@ -398,22 +388,22 @@
     :type override: bool
     :param force: True if test files should be replaced if exist, defaut to False
     :type force: bool
     """
     for root, dirs, files in os.walk(path):
         obj = None
         if 'configure' in files:
-            n = log.manager.style("Autotools", fg="yellow", bold=True)
+            n = "[yello bold]Autotools[/]"
             obj = AutotoolsBuildSystem(root, dirs, files)
         if 'CMakeLists.txt' in files:
-            n = log.manager.style("CMake", fg="cyan", bold=True)
+            n = "[cyan bold]CMake[/]"
             obj = CMakeBuildSystem(root, dirs, files)
         if 'Makefile' in files:
-            n = log.manager.style("Make", fg="red", bold=True)
+            n = "[red bold]Make[/]"
             obj = MakefileBuildSystem(root, dirs, files)
 
         if obj is not None:
             dirs[:] = []
-            log.manager.print_item("{} [{}]".format(root, n))
+            io.console.print_item("{} [{}]".format(root, n))
             obj.fill()
             if override:
                 obj.generate_file(filename="pcvs.yml", force=force)
```

### Comparing `pcvs-0.6.0/pcvs/cli/cli_bank.py` & `pcvs-0.7.0/pcvs/cli/cli_bank.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,21 @@
 import os
 import sys
 
-import click
 from click.shell_completion import CompletionItem
 
+from pcvs import io
 from pcvs.backend import bank as pvBank
-from pcvs.helpers import log, utils
+from pcvs.helpers import utils
+
+try:
+    import rich_click as click
+    click.rich_click.SHOW_ARGUMENTS = True
+except ImportError:
+    import click
 
 
 def compl_list_banks(ctx, args, incomplete):
     """bank name completion function.
 
     :param ctx: Click context
     :type ctx: :class:`Click.Context`
@@ -39,56 +45,61 @@
     array = list()
     for bankname, bankpath in compl_list_banks(None, None, ''):
         bank = pvBank.Bank(token=bankname)
         bank.connect()
         for project in bank.list_projects():
             array.append((bankname + "@" + project, bankpath))
         bank.disconnect()
-    
+
     return [CompletionItem(elt[0], help=elt[1]) for elt in array if incomplete in elt[0]]
 
 
 @click.group(name="bank", short_help="Persistent data repository management")
 @click.pass_context
 def bank(ctx):
     """Bank entry-point."""
     pass
 
 
 @bank.command(name="list", short_help="List known repositories")
 @click.pass_context
 def bank_list(ctx):
     """List known repositories, stored under ``PATH_BANK``."""
-    log.manager.print_header("Bank View")
+    io.console.print_header("Bank View")
     for label, path in pvBank.list_banks().items():
-        log.manager.print_item("{:<8}: {}".format(label.upper(), path))
+        io.console.print_item("{:<8}: {}".format(label.upper(), path))
 
 
 @bank.command(name="show", short_help="Display data stored in a repo.")
 @click.argument("name", nargs=1, required=True, type=str, shell_complete=compl_list_banks)
+@click.option("-p", "--path", "path", is_flag=True, default=False,
+              help="Display bank location")
 @click.pass_context
-def bank_show(ctx, name):
+def bank_show(ctx, name, path):
     """Display all data stored into NAME repository"""
-    log.manager.print_header("Bank View")
-
     b = pvBank.Bank(token=name)
     if not b.exists():
         raise click.BadArgumentUsage("'{}' does not exist".format(name))
     else:
         b.connect()
+    
+    if path:
+        print(b.path)
+    else:
+        io.console.print_header("Bank View")
         b.show()
 
 
 @bank.command(name="init", short_help="Register a bank & create a repo if needed")
 @click.argument("name", type=str, shell_complete=compl_list_banks)
 @click.argument("path", required=False, type=click.Path(exists=False, file_okay=False))
 @click.pass_context
 def bank_create(ctx, name, path):
     """Create a new bank, named NAME, data will be stored under PATH."""
-    log.manager.print_header("Bank View")
+    io.console.print_header("Bank View")
     if path is None:
         path = os.getcwd()
 
     path = os.path.abspath(path)
 
     b = pvBank.Bank(path, token=name)
     if b.exists():
@@ -108,60 +119,78 @@
     help="Do not ask for confirmation before deletion")
 @click.pass_context
 def bank_destroy(ctx, name, symlink):
     """Remove the bank NAME from PCVS management. This does not include
     repository deletion. 'data.yml' and bank entry in the configuratino file
     will be removed but existing data are preserved.
     """
-    log.manager.print_header("Bank View")
+    io.console.print_header("Bank View")
     b = pvBank.Bank(token=name)
     if not b.exists():
         raise click.BadArgumentUsage("'{}' does not exist".format(name))
     else:
         if not symlink:
-            log.manager.warn(
+            io.console.warn(
                 "To delete a bank, just remove the directory {}".format(b.prefix))
-        log.manager.print_item("Bank '{}' unlinked".format(name))
+        io.console.print_item("Bank '{}' unlinked".format(name))
         pvBank.rm_banklink(name)
 
 
 @bank.command(name="save", short_help="Save a new run to the datastore")
 @click.argument("name", nargs=1, required=True, type=str, shell_complete=compl_list_banks)
 @click.argument("path", nargs=1, required=True, type=click.Path(exists=True))
+@click.option('--message', "-m", "msg", default=None,
+              help="Use a custom Run() message")
 @click.pass_context
-def bank_save_run(ctx, name, path):
+def bank_save_run(ctx, name, path, msg):
     """Create a backup from a previously generated build directory. NAME will be
     the target bank name, PATH the build directory"""
 
     b = pvBank.Bank(token=name)
     if not b.exists():
         raise click.BadArgumentUsage("'{}' does not exist".format(name))
 
     path = os.path.abspath(path)
     project = b.default_project
 
     b.connect()
     if os.path.isfile(path):
-        b.save_from_archive(project, path)
+        b.save_from_archive(project, path, msg=msg)
     elif os.path.isdir(path):
         path = utils.find_buildir_from_prefix(path)
-        b.save_from_buildir(project, path)
+        b.save_from_buildir(project, path, msg=msg)
 
 
 @bank.command(name="load", short_help="Extract infos from the datastore")
 @click.argument("name", nargs=1, required=True, type=str, shell_complete=compl_list_banks)
-@click.argument("key", nargs=1, required=True)
 @click.option("--since", "start", default=None,
               help="Select a starting point from where data will be extracted")
 @click.option("--until", "end", default=None,
               help="Select the last date (included) where data will be searched for")
-@click.option("-f", "--format", "format",
-              type=click.Choice(['json', 'list']), default='json',
-              help="Request a set of values from a given key")
-@click.pass_context
-def bank_load(ctx, name, key, format, start, end):
-    print(name)
-    b = pvBank.Bank(name)
-    print(b.default_project)
-    serie = b.get_serie(b.default_project)
+@click.option("-s", "--startswith", "prefix",
+              type=str, default="",
+              help="Select only a subset of each runs based on provided prefix")
+@click.pass_context
+def bank_load(ctx, name, prefix, start, end):
+    b = pvBank.Bank(token=name)
+    serie = b.get_serie()
     run = serie.last
-    print(run.get_data(key).to_json())
+    data = []
+    from rich.progress import Progress
+    with Progress():
+        if not prefix:
+            for j in run.jobs:
+                data.append(j.to_json())
+        else:
+            for j in run.get_data(prefix):
+                data.append(j.to_json())
+    import json
+    print(json.dumps(data))
+
+
+@bank.command(name="extract", short_help="Extract infos from the datastore")
+@click.argument("name", nargs=1, required=True, type=str, shell_complete=compl_list_banks)
+@click.argument("key", nargs=1, required=True)
+@click.pass_context
+def bank_extract(ctx, name, key):
+
+    pass
```

### Comparing `pcvs-0.6.0/pcvs/cli/cli_config.py` & `pcvs-0.7.0/pcvs/cli/cli_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,22 @@
 import sys
 
-import click
 from ruamel.yaml import YAML
 
+from pcvs import io
 from pcvs.backend import config as pvConfig
-from pcvs.helpers import log, utils
+from pcvs.helpers import utils
 from pcvs.helpers.exceptions import ConfigException
 
+try:
+    import rich_click as click
+    click.rich_click.SHOW_ARGUMENTS = True
+except ImportError:
+    import click
+
 
 def compl_list_token(ctx, args, incomplete) -> list:  # pragma: no cover
     """config name completion function.
 
     :param ctx: Click context
     :type ctx: :class:`Click.Context`
     :param args: the option/argument requesting completion.
@@ -70,31 +76,30 @@
     :type kind: str
     :param scope: config scope
     :type scope: str
     """
     # retrieve blocks to print
     blocks = pvConfig.list_blocks(kind, scope)
     if not blocks:
-        log.manager.print_item("None")
+        io.console.print_item("None")
         return
     elif scope is None:  # if no scope has been provided by the user
         for sc in utils.storage_order():
             # aggregate names for each sccope
             names = sorted([elt[0] for elt in [array for array in blocks[sc]]])
             if not names:
-                log.manager.print_item("{: <6s}: {}".format(
-                    sc.upper(),
-                    log.manager.style('None', fg='bright_black')))
+                io.console.print_item(
+                    "[bright_black]{: <6s}: None".format(sc.upper()))
             else:
-                log.manager.print_item("{: <6s}: {}".format(
+                io.console.print_item("{: <6s}: {}".format(
                     sc.upper(),
                     ", ".join(names)))
     else:
         names = sorted([x[0] for x in blocks])
-        log.manager.print_item("{: <6s}: {}".format(
+        io.console.print_item("{: <6s}: {}".format(
             scope.upper(), ", ".join(names)))
 
 
 @config.command(name="list", short_help="List available configuration blocks")
 @click.argument("token", nargs=1, required=False,
                 type=click.STRING, shell_complete=compl_list_token)
 @click.option("-a", "--all", "all", is_flag=True, default=False,
@@ -111,42 +116,42 @@
         'all' is a specific value to list all configurations.
     """
     (scope, kind, label) = (None, None, None)
     if token:
         (scope, kind, label) = utils.extract_infos_from_token(
             token, pair="left", single="center")
     if label:
-        log.manager.warn("no LABEL required for this command")
+        io.console.warn("no LABEL required for this command")
 
     # special cases for 'list' command:
     # - no 'label' are required (ignored otherwise)
     # - a special 'all' value is allowed for 'kind' parameter
     if kind is None or kind.lower() == 'all':
         kinds = pvConfig.CONFIG_BLOCKS
     else:
         pvConfig.check_valid_kind(kind)
         kinds = [kind]
     utils.check_valid_scope(scope)
 
-    log.manager.print_header("Configuration view")
+    io.console.print_header("Configuration view")
 
     for k in kinds:
-        log.manager.print_section("Kind '{}'".format(k.upper()))
+        io.console.print_section("Kind '{}'".format(k.upper()))
         config_list_single_kind(k, scope)
 
     if all:
-        log.manager.print_section(
+        io.console.print_section(
             "Available templates to create from (--base option):")
-        log.manager.print_item(
+        io.console.print_item(
             ", ".join([x for x in sorted(pvConfig.list_templates())]))
 
     # in case verbosity is enabled, add scope paths
-    log.manager.info("Scopes are ordered as follows:")
+    io.console.info("Scopes are ordered as follows:")
     for i, scope in enumerate(utils.storage_order()):
-        log.manager.info("{}. {}: {}".format(
+        io.console.info("{}. {}: {}".format(
             i+1, scope.upper(), utils.STORAGES[scope]))
 
 
 @config.command(name="show",
                 short_help="Show detailed view of the selected configuration")
 @click.argument("token", nargs=1, type=click.STRING,
                 shell_complete=compl_list_token)
```

### Comparing `pcvs-0.6.0/pcvs/cli/cli_plumbing.py` & `pcvs-0.7.0/pcvs/cli/cli_plumbing.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,38 @@
 import sys
-import click 
-from pcvs.cli.cli_bank import compl_list_banks
+
 from pcvs.backend.bank import Bank
+from pcvs.cli.cli_bank import compl_list_banks
 from pcvs.dsl.analysis import ResolverAnalysis
 from pcvs.helpers.system import MetaConfig
 
+try:
+    import rich_click as click
+    click.rich_click.SHOW_ARGUMENTS = True
+except ImportError:
+    import click
+
 
 @click.command(name="resolve", short_help="Resolve test status")
 @click.option("-b", "--bank", "bankname", shell_complete=compl_list_banks,
               default=None, help="explicit bank name to use.")
 @click.option("-f", "--file", "file",
               type=click.Path(exists=False), default=None,
               is_flag=False, help="read from file instead of stdin")
 @click.pass_context
 def resolve(ctx, file, bankname):
-    
+
     if file:
         with open(file, 'r') as fh:
             stream = fh.read().rstrip()
     else:
         stream = sys.stdin.read().rstrip()
 
     if not bankname:
         bankname = MetaConfig.root.validation.target_bank
 
     # may deadlock !!
     bank = Bank(bankname)
 
     print(stream)
-    
-    bank.disconnect()
+
+    bank.disconnect()
```

### Comparing `pcvs-0.6.0/pcvs/cli/cli_profile.py` & `pcvs-0.7.0/pcvs/cli/cli_profile.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 import os
 import sys
 
-import click
+from rich.table import Table
 from ruamel.yaml import YAML
 
-from pcvs import PATH_INSTDIR
+from pcvs import PATH_INSTDIR, io
 from pcvs.backend import config as pvConfig
 from pcvs.backend import profile as pvProfile
 from pcvs.cli import cli_config
 from pcvs.helpers import log, utils
 from pcvs.helpers.exceptions import ProfileException, ValidationException
 
+try:
+    import rich_click as click
+    click.rich_click.SHOW_ARGUMENTS = True
+except ImportError:
+    import click
+
 
 def compl_list_token(ctx, args, incomplete):  # pragma: no cover
     """profile name completion function.
 
     :param ctx: Click context
     :type ctx: :class:`Click.Context`
     :param args: the option/argument requesting completion.
@@ -70,57 +76,53 @@
 def profile_list(ctx, token, all):
     """
     List all known profiles to be used as part of a validation process. The
     list can be filtered out depending on the '--scope' option to only print
     out profiles available at a given granularity.
     """
     (scope, label) = (None, None)
+    table = Table("Full name", "Location", title="Profiles", expand=True)
     if token:
         (scope, _, label) = utils.extract_infos_from_token(token, single="left",
                                                            maxsplit=2)
 
     if label:
-        log.manager.warn("no LABEL required for this command")
+        io.console.warn(
+            "no LABEL required for this command (s'{}' given)".format(label))
 
-    utils.check_valid_scope(scope)
+    profiles = list()
+    if scope:
+        utils.check_valid_scope(scope)
+        profiles = pvProfile.list_profiles(scope)
+    else:
+        for pf_list in pvProfile.list_profiles().values():
+            for pf in pf_list:
+                profiles.append((pf[0], pf[1]))
 
-    log.manager.print_header("Profile View")
-    profiles = pvProfile.list_profiles(scope)
     if not profiles:
-        log.manager.print_item("None")
+        io.console.print_item("None")
         return
-    elif scope is None:  # if no scope has been provided by the user
-        for sc in utils.storage_order():
-            # aggregate names for each sccope
-            names = sorted([elt[0]
-                            for elt in [array for array in profiles[sc]]])
-            if not names:
-                log.manager.print_item("{: <6s}: {}".format(sc.upper(),
-                                                            log.manager.style('None',
-                                                                              fg='bright_black')))
-            else:
-                log.manager.print_item("{: <6s}: {}".format(sc.upper(),
-                                                            ", ".join(names)))
-    else:
-        names = sorted([x[0] for x in profiles])
-        log.manager.print_item("{: <6s}: {}".format(
-            scope.upper(), ", ".join(names)))
+
+    for profile in profiles:
+        table.add_row(*profile)
 
     if all:
-        log.manager.print_section(
+        io.console.print_section(
             "Available templates to create from (--base option):")
-        log.manager.print_item(
+        io.console.print_item(
             ", ".join([x[0] for x in pvProfile.list_templates()]))
 
     # in case verbosity is enabled, add scope paths
-    log.manager.info("Scopes are ordered as follows:")
+    io.console.info("Scopes are ordered as follows:")
     for i, scope in enumerate(utils.storage_order()):
-        log.manager.info("{}. {}: {}".format(
+        io.console.info("{}. {}: {}".format(
             i+1, scope.upper(), utils.STORAGES[scope]))
 
+    io.console.print(table)
+
 
 @profile.command(name="show",
                  short_help="Prints single profile details")
 @click.argument("token", nargs=1, type=click.STRING,
                 shell_complete=compl_list_token)
 @click.pass_context
 def profile_show(ctx, token):
@@ -142,27 +144,27 @@
     and waits for a selection. A final profile is built from them.
 
     :return: concatenation of basic blokcs
     :rtype: dict
     """
     composition = {}
     for kind in pvConfig.CONFIG_BLOCKS:
-        log.manager.print_section("Pick up a {}".format(kind.capitalize()))
+        io.console.print_section("Pick up a {}".format(kind.capitalize()))
         choices = []
         for scope, avails in pvConfig.list_blocks(kind).items():
             for elt in avails:
                 choices.append(".".join([scope, elt[0]]))
 
         idx = len(choices) + 1
         try:
             default = choices.index("global.default") + 1
         except ValueError:
             default = None
         for i, cell in enumerate(choices):
-            log.manager.print_item("{}: {}".format(i + 1, cell))
+            io.console.print_item("{}: {}".format(i + 1, cell))
         while idx < 0 or len(choices) <= idx:
             idx = click.prompt("Your selection", default, type=int) - 1
         (scope, _, label) = utils.extract_infos_from_token(
             choices[idx], pair="span")
         composition[kind] = pvConfig.ConfigurationBlock(kind, label, scope)
 
     return composition
@@ -226,15 +228,15 @@
         (c_scope, _, c_label) = utils.extract_infos_from_token(clone, maxsplit=2)
         base = pvProfile.Profile(c_label, c_scope)
         base.load_from_disk()
         pf.clone(base)
     elif base:
         pf.load_template(base)
     elif interactive:
-        log.manager.print_header("profile view (build)")
+        io.console.print_header("profile view (build)")
         pf_blocks = profile_interactive_select()
         pf.fill(pf_blocks)
     else:
         if len(blocks) > 0:
             for blocklist in blocks:
                 for block in blocklist.split(','):
                     (b_sc, b_kind, b_label) = utils.extract_infos_from_token(block)
@@ -248,22 +250,22 @@
                     pf_blocks[b_kind] = cur
             pf.fill(pf_blocks)
         else:
             base = pvProfile.Profile('default', None)
             base.load_template()
             pf.clone(base)
 
-    log.manager.print_header("profile view")
+    io.console.print_header("profile view")
     pf.flush_to_disk()
     # pf.display()
 
-    log.manager.print_section(
+    io.console.print_section(
         "final profile (registered as {})".format(pf.scope))
     for k, v in pf_blocks.items():
-        log.manager.print_item("{: >9s}: {}".format(
+        io.console.print_item("{: >9s}: {}".format(
             k.upper(), ".".join([v.scope, v.short_name])))
 
 
 @profile.command(name="destroy",
                  short_help="Delete a profile from disk")
 @click.confirmation_option(
     "-f", "--force", "force", expose_value=False,
@@ -296,15 +298,15 @@
 @profile.command(name="edit",
                  short_help="Edit an existing profile")
 @click.argument("token", nargs=1, type=click.STRING,
                 shell_complete=compl_list_token)
 @click.option("-p", "--edit-plugin", "edit_plugin", is_flag=True, default=False,
               help="Only edit the plugin code ('runtime')")
 @click.pass_context
-@log.manager.capture_exception(ValidationException.FormatError)
+@io.capture_exception(ValidationException.FormatError)
 def profile_edit(ctx, token, edit_plugin):
     """Edit an existing profile with the given EDITOR. The '-p' option will open
     the decoded runtime plugin code stored as a base64 string into the profile
     for edition.
 
     After edition, the result will be validated to ensure
     coherency. If the test failed a rej*.yml will be created with the edited
@@ -395,11 +397,11 @@
     pf = pvProfile.Profile(label, scope)
     if not pf.is_found():
         click.BadArgumentUsage(
             "Cannot decompose an non-existent profile: '{}'".format(token))
     else:
         pf.load_from_disk()
 
-    log.manager.print_section('"Create the subsequent configuration blocks:')
+    io.console.print_section('"Create the subsequent configuration blocks:')
     for c in pf.split_into_configs(name, blocks, scope):
-        log.manager.print_item(c.full_name)
+        io.console.print_item(c.full_name)
         c.flush_to_disk()
```

### Comparing `pcvs-0.6.0/pcvs/cli/cli_report.py` & `pcvs-0.7.0/pcvs/cli/cli_report.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,59 +1,55 @@
 import os
 
-import click
-
-from pcvs import NAME_BUILDFILE, NAME_BUILDIR
+from pcvs import NAME_BUILDFILE, NAME_BUILDIR, io
 from pcvs.backend import report as pvReport
-from pcvs.helpers import log
+#from pcvs.gui.curses import viewer
+from pcvs.helpers import utils
+
+try:
+    import rich_click as click
+    click.rich_click.SHOW_ARGUMENTS = True
+except ImportError:
+    import click
 
 
 @click.command('report', short_help="Manage PCVS result reporting interface")
 @click.option("-s", "--static-pages", "static", flag_value=".", default=None)
 @click.argument("path_list", nargs=-1, required=False, type=click.Path(exists=True))
 @click.pass_context
 def report(ctx, path_list, static):
     """Start a webserver to browse result during or after execution.
 
-    Listens by default to http://localhost:5000/"""
+     Listens by default to http://localhost:5000/"""
+    if not path_list:
+        path_list = [os.getcwd()]
+
     inputs = list()
-    # sanity check
     for prefix in path_list:
         # if a dir is given BU does not point to a valid build dir,
         # attempt to resolve it.
-        # Note that files are always kept, it ensure to the user to 
+        # Note that files are always kept, it ensure to the user to
         # provide a valid archive-formatted file
-        print(prefix)
-        if not os.path.isfile(prefix) and \
-            not os.path.isfile(os.path.join(prefix, NAME_BUILDFILE)):
-            # if the 'builddir' default name was missing for resolution, add it
-            if os.path.isfile(os.path.join(prefix, NAME_BUILDIR, NAME_BUILDFILE)):
-                prefix = os.path.join(prefix, NAME_BUILDIR)
-            else:  # otherwise, it is a wrong path -> error
-                raise click.BadArgumentUsage(
-                    '{} is not a build directory.'.format(prefix))
-
-        inputs.append(os.path.abspath(prefix))
-
-    # extra step, if the user didn't specify anything, attempt to add cwd
-    current_dir = os.path.join(os.getcwd(), NAME_BUILDIR)
-    if len(inputs) == 0 and os.path.isfile(os.path.join(current_dir, NAME_BUILDFILE)):
-        inputs.append(current_dir)
+        if utils.check_is_build_or_archive(prefix):
+            inputs.append(os.path.abspath(prefix))
+        elif utils.check_is_build_or_archive(os.path.join(prefix, NAME_BUILDIR)):
+            inputs.append(os.path.abspath(os.path.join(prefix, NAME_BUILDIR)))
+        else:
+            raise click.BadArgumentUsage(
+                '{} is not a build directory.'.format(prefix))
 
     if static:
         # server old-style JCRHONOSS pages after JSON transformation
         for prefix in inputs:
             pvReport.build_static_pages(prefix)
     else:
         # feed with prefixes
+        r = pvReport.Report()
         for prefix in inputs:
             try:
-                if os.path.isfile(prefix):
-                    pvReport.upload_buildir_results_from_archive(prefix)
-                else:
-                    pvReport.upload_buildir_results(prefix)
+                r.add_session(prefix)
             except Exception as e:
-                log.manager.warn("Unable to parse {}".format(prefix))
-                log.manager.debug("Caught {}".format(e))
+                io.console.warn("Unable to parse {}".format(prefix))
+                io.console.debug("Caught {}".format(e))
                 raise e
         # create the app
-        pvReport.start_server()
+        pvReport.start_server(r)
```

### Comparing `pcvs-0.6.0/pcvs/cli/cli_run.py` & `pcvs-0.7.0/pcvs/cli/cli_run.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 import os
 import sys
 from datetime import datetime
 
-import click
-
-from pcvs import NAME_BUILDFILE
+from pcvs import NAME_BUILDFILE, NAME_RUN_CONFIG_FILE, io
+from pcvs.io import Verbosity
 from pcvs.backend import bank as pvBank
 from pcvs.backend import profile as pvProfile
 from pcvs.backend import run as pvRun
 from pcvs.backend import session as pvSession
 from pcvs.cli import cli_bank, cli_profile
-from pcvs.helpers import exceptions, log, system, utils
+from pcvs.helpers import exceptions, system, utils
+from pcvs.orchestration.publishers import BuildDirectoryManager
+
+try:
+    import rich_click as click
+    click.rich_click.SHOW_ARGUMENTS = True
+except ImportError:
+    import click
 
 
 def iterate_dirs(ctx, param, value) -> dict:
     """Validate directories provided by users & format them correctly.
 
     Set the defaul label for a given path if not specified & Configure default
     directories if none was provided.
@@ -72,16 +78,15 @@
     abspath = os.path.abspath(incomplete)
 
     if ":" in incomplete:
         label, path = incomplete.split(":", 1)
         label += ":"
     obj = click.Path(exists=True, dir_okay=True, file_okay=False)
     obj.shell_complete(ctx, args, incomplete)
-        
-    
+
 
 def handle_build_lockfile(exc=None):
     """Remove the file lock in build dir if the application stops abrubtly.
 
     This function will automatically forward the raising exception to the next
     handler.
 
@@ -97,15 +102,15 @@
                 utils.unlock_file(prefix)
 
     if exc:
         raise exc
 
 
 @click.command(name="run", short_help="Run a validation")
-@click.option("-p", "--profile", "profilename", default="default",
+@click.option("-p", "--profile", "profilename", default=None,
               shell_complete=cli_profile.compl_list_token,
               type=str, show_envvar=True,
               help="Existing and valid profile supporting this run")
 @click.option("-o", "--output", "output", default=None, show_envvar=True,
               type=click.Path(exists=False, file_okay=False),
               help="F directory where PCVS is allowed to store data")
 @click.option("-c", '--settings-file', "settings_file",
@@ -121,57 +126,72 @@
               default=False, is_flag=True,
               help="Reproduce the whole process without running tests")
 @click.option("-a", "--anonymize", "anon",
               default=None, is_flag=True,
               help="Purge the results from sensitive data (HOME, USER...)")
 @click.option("-b", "--bank", "bank", default=None, shell_complete=cli_bank.compl_bank_projects,
               help="Which bank will store the run in addition to the archive")
+@click.option("-m", "--message", "msg", default=None,
+              help="Message to store the run (if bank is enabled)")
 @click.option("--duplicate", "dup", default=None,
               type=click.Path(exists=True, file_okay=False), required=False,
               help="Reuse old test directories (no DIRS required)")
 @click.option("-r", "--report", "enable_report", show_envvar=True,
-              is_flag=True, default=False,
+              is_flag=True, default=None,
               help="Attach a webview server to the current session run.")
 @click.option("--report-uri", "report_addr", default=None, type=str,
               help="Override default Server address")
 @click.option("-g", "--generate-only", "generate_only", is_flag=True, default=None,
               help="Rebuild the test-base, populating resources for `pcvs exec`")
-@click.option('-t', "--timeout", "timeout", show_envvar=True, type=int,
+@click.option('-t', "--timeout", "timeout", show_envvar=True, type=int, default=None,
               help="PCVS process timeout")
+@click.option("-S", "--successful", "only_success", is_flag=True, default=None,
+              help="Return non-zero exit code if a single test has failed")
 @click.option("-s", "--spack-recipe", "spack_recipe", type=str, multiple=True,
               help="Build test-suites based on Spack recipes")
 @click.option("-P", "--print", "print_level", type=click.Choice(['none', 'errors', 'all']),
-              help="Enable test output to be printed depending on its status")
+              default=None, help="Enable test output to be printed depending on its status")
 @click.argument("dirs", nargs=-1,
                 type=str, callback=iterate_dirs)
 @click.pass_context
-@log.manager.capture_exception(Exception)
-@log.manager.capture_exception(Exception, handle_build_lockfile)
-@log.manager.capture_exception(KeyboardInterrupt, handle_build_lockfile)
+@io.capture_exception(Exception)
+@io.capture_exception(Exception, handle_build_lockfile)
+@io.capture_exception(KeyboardInterrupt, handle_build_lockfile)
 def run(ctx, profilename, output, detach, override, anon, settings_file,
-        generate_only, spack_recipe, print_level, simulated, bank, dup,
-        dirs, enable_report, report_addr, timeout) -> None:
+        generate_only, spack_recipe, print_level, simulated, bank, msg, dup,
+        dirs, enable_report, report_addr, only_success, timeout) -> None:
     """
     Execute a validation suite from a given PROFILE.
 
     By default the current directory is scanned to find test-suites to run.
     May also be provided as a list of directories as described by tests
     found in DIRS.
     """
-    log.manager.info("PRE-RUN: start")
+    
+    io.console.info("PRE-RUN: start")
     # first, prepare raw arguments to be usable
     if output is not None:
         output = os.path.abspath(output)
-        
+
+    if print_level and print_level != "none":
+        # any --print option will imply to disable packed rich console view
+        # --> enable verbose mode
+        io.console.verbose = Verbosity.DETAILED
+        ctx.obj['verbose'] = str(io.console.verbose)
+
     global_config = system.MetaConfig()
     system.MetaConfig.root = global_config
     global_config.set_internal("pColl", ctx.obj['plugins'])
 
     # then init the configuration
-    log.manager.debug(
+    if settings_file is None:
+        # detect ?
+        detect = os.path.join(os.getcwd(), NAME_RUN_CONFIG_FILE)
+        settings_file = detect if os.path.isfile(detect) else None
+    io.console.debug(
         "PRE-RUN: load settings from local file: {}".format(settings_file))
     val_cfg = global_config.bootstrap_validation_from_file(settings_file)
 
     # save 'run' parameters into global configuration
     val_cfg.set_ifdef('datetime', datetime.now())
     val_cfg.set_ifdef('verbose', ctx.obj['verbose'])
     val_cfg.set_ifdef('print_level', print_level)
@@ -181,97 +201,100 @@
     val_cfg.set_ifdef('override', override)
     val_cfg.set_ifdef('simulated', simulated)
     val_cfg.set_ifdef('onlygen', generate_only)
     val_cfg.set_ifdef('anonymize', anon)
     val_cfg.set_ifdef('reused_build', dup)
     val_cfg.set_ifdef('default_profile', profilename)
     val_cfg.set_ifdef('target_bank', bank)
+    val_cfg.set_ifdef('message', msg)
     val_cfg.set_ifdef('enable_report', enable_report)
     val_cfg.set_ifdef('report_addr', report_addr)
     val_cfg.set_ifdef('timeout', timeout)
     val_cfg.set_ifdef('spack_recipe', spack_recipe)
-    val_cfg.set_ifdef('runlog', os.path.join(val_cfg.output, 'out.log'))
+    val_cfg.set_ifdef('only_success', only_success)
     val_cfg.set_ifdef('buildcache', os.path.join(val_cfg.output, 'cache'))
 
     # if dirs not set by config file nor CLI
     if not dirs and not val_cfg.dirs:
         dirs = dict()
         if not spack_recipe:
             testpath = os.getcwd()
             dirs = {os.path.basename(testpath): testpath}
 
     # not overriding if dirs is None
     val_cfg.set_ifdef("dirs", dirs)
 
     if bank is not None:
         obj = pvBank.Bank(token=bank, path=None)
-        log.manager.debug(
+        io.console.debug(
             "PRE-RUN: configure target bank: {}".format(obj.name))
         if not obj.exists():
             raise click.BadOptionUsage(
                 "--bank", "'{}' bank does not exist".format(obj.name))
         obj.disconnect()
 
     # BEFORE the build dir still does not exist !
     buildfile = os.path.join(val_cfg.output, NAME_BUILDFILE)
     if os.path.exists(val_cfg.output):
+        # careful if the build dir does not exist
+        # the condition above may be executed concurrently
+        # by two runs, inducing parallel execution in the same dir
+        # TODO.
         if not utils.trylock_file(buildfile):
             if val_cfg.override:
                 utils.lock_file(buildfile, force=True)
             else:
                 raise exceptions.RunException.InProgressError(path=val_cfg.output,
                                                               lockfile=buildfile,
                                                               owner_pid=utils.get_lock_owner(buildfile))
 
     elif not os.path.exists(val_cfg.output):
-        log.manager.debug(
+        io.console.debug(
             "PRE-RUN: Prepare output directory: {}".format(val_cfg.output))
         os.makedirs(val_cfg.output)
 
     # check if another build should reused
     # this avoids to re-run combinatorial system twice
     if val_cfg.reused_build is not None:
-        log.manager.info("PRE-RUN: Clone previous build to be reused")
+        io.console.info("PRE-RUN: Clone previous build to be reused")
         try:
-            log.manager.debug(
+            io.console.debug(
                 "PRE-RUN: previous build: {}".format(val_cfg.reused_build))
             global_config = pvRun.dup_another_build(
                 val_cfg.reused_build, val_cfg.output)
             # TODO: Currently nothing can be overriden from cloned build except:
             # - 'output'
         except FileNotFoundError:
             raise click.BadOptionUsage(
                 "--duplicate", "{} is not a valid build directory!".format(val_cfg.reused_build))
     else:
         # otherwise create own settings command block
-        log.manager.info(
+        io.console.info(
             "PRE-RUN: Profile lookup: {}".format(val_cfg.default_profile))
         (scope, _, label) = utils.extract_infos_from_token(val_cfg.default_profile,
                                                            maxsplit=2)
         pf = pvProfile.Profile(label, scope)
         if not pf.is_found():
             raise click.BadOptionUsage(
                 "--profile", "Profile '{}' not found".format(val_cfg.default_profile))
         pf.load_from_disk()
+        pf.check()
 
         val_cfg.set_ifdef('pf_name', pf.full_name)
         val_cfg.set_ifdef('pf_hash', pf.get_unique_id())
-        global_config.bootstrap_compiler(pf.compiler)
-        global_config.bootstrap_runtime(pf.runtime)
-        global_config.bootstrap_machine(pf.machine)
-        global_config.bootstrap_criterion(pf.criterion)
-        global_config.bootstrap_group(pf.group)
+        global_config.bootstrap_from_profile(pf.dump())
 
     the_session = pvSession.Session(val_cfg.datetime, val_cfg.output)
-    the_session.register_callback(callback=pvRun.process_main_workflow,
-                                  io_file=val_cfg.runlog)
+    the_session.register_callback(callback=pvRun.process_main_workflow)
 
-    log.manager.info("PRE-RUN: Session to be started")
+    io.console.info("PRE-RUN: Session to be started")
     if val_cfg.background:
         sid = the_session.run_detached(the_session)
-        log.manager.print_item(
+        print(
             "Session successfully started, ID {}".format(sid))
+
     else:
         sid = the_session.run(the_session)
         utils.unlock_file(buildfile)
-
-    sys.exit(the_session.rc)
+       
+    final_rc = the_session.rc if only_success else 0
+    sys.exit(final_rc)
```

### Comparing `pcvs-0.6.0/pcvs/cli/cli_utilities.py` & `pcvs-0.7.0/pcvs/cli/cli_utilities.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,48 +2,79 @@
 import copy
 import os
 import shutil
 import subprocess
 import sys
 from datetime import datetime
 
-import click
-from prettytable import PrettyTable
+from rich.panel import Panel
+from rich.table import Table
 
-from pcvs import NAME_BUILDFILE
+from pcvs import NAME_BUILD_ARCHIVE_DIR, NAME_BUILDFILE, io
 from pcvs.backend import utilities as pvUtils
-from pcvs.helpers import log
+from pcvs.helpers import utils
 from pcvs.helpers.system import MetaConfig
 
+try:
+    import rich_click as click
+    click.rich_click.SHOW_ARGUMENTS = True
+except ImportError:
+    import click
+
 
 @click.command(name="exec", short_help="Running aspecific test")
-@click.option('-o', '--output', 'output', default=None,
+@click.option('-o', '--output', 'output', default=None, type=click.Path(exists=True, dir_okay=True, file_okay=False),
               help="Directory where build artifacts are stored")
 @click.option('-l', '--list', 'gen_list', is_flag=True,
               help='List available tests (may take a while)')
 @click.option("-s", "--show", "display",
-              type=click.Choice(['cmd', 'env', 'loads', 'all', 'out']), default=None,
-              is_flag=False, flag_value="all",
+              type=click.Choice(['cmd', 'env', 'mod', 'all', 'out']), default=None, multiple=True,
               help="Display information instead of executing the command")
+@click.option("-C", "--print-command", "pcmd", flag_value="cmd",
+              help="Dedicated option to print target command")
+@click.option("-E", "--print-env", "penv", flag_value="env",
+              help="Dedicated option to print target modified environment")
+@click.option("-M", "--print-module", "pmod", flag_value="mod",
+              help="Dedicated option to print target manager pre-load")
+@click.option("-O", "--print-output", "pout", flag_value="out",
+              help="Dedicated option to print target output")
+@click.option("-A", "--print-all", "pall", flag_value="all",
+              help="Dedicated option to print everything")
 @click.argument("argument", type=str, required=False)
 @click.pass_context
-def exec(ctx, output, argument, gen_list, display):
+def exec(ctx, output, argument, gen_list, display, pcmd, penv, pmod, pout, pall) -> None:
     """ Run a unit test as it would have been through the whole engine (for
     reproducing purposes) from the command line."""
     rc = 0
     err = subprocess.STDOUT
     env = copy.deepcopy(os.environ)
 
-    if display == 'out':
-        # special case
-        print(pvUtils.get_logged_output(output, argument))
-        return
+    display = set(display)
+    if pall or 'all' in display:
+        pmod = "mod"
+        penv = "env"
+        pcmd = "cmd"
+        pout = "out"
+    
+    if pmod:
+        display.add(pmod)
+    if pcmd:
+        display.add(pcmd)
+    if pout:
+        display.add(pout)
+    if penv:
+        display.add(penv)
+
+    if len(display) > 0:
+        env.update({"PCVS_SHOW": '1'})
+        for e in display:
+            env.update({'PCVS_SHOW_{}'.format(e.upper()): '1'})
 
-    if display:
-        env.update({'PCVS_SHOW': str(display)})
+    if ctx.obj['verbose'] > 0:
+        env.update({"PCVS_VERBOSE": '1'})
 
     if gen_list:
         script_path = pvUtils.locate_scriptpaths(output)
         argument = "--list"
         err = subprocess.DEVNULL
     else:
         if not argument:
@@ -60,14 +91,18 @@
                 env=env,
                 stderr=err)
             fds.communicate()
             rc = fds.returncode
     except subprocess.CalledProcessError as e:
         rc = e.returncode
 
+    if 'out' in display:
+        # special case
+        print(pvUtils.get_logged_output(output, argument))
+
     # return code to console
     sys.exit(rc)
 
 
 @click.command(name="check", short_help="Ensure future input will be conformant to standards")
 @click.option("--encoding", "-E", "encoding", default=False, is_flag=True,
               help="Check capability to print utf-8 characters properly")
@@ -78,78 +113,73 @@
               help="Check correctness for pcvs.* files")
 @click.option("--configs", "-C", "configs", default=False, is_flag=True,
               help="Check correctness for all registered configuation block")
 @click.option("--profiles", "-P", "profiles", default=False, is_flag=True,
               help="Check correctness for all registered profiles")
 @click.option("--profile-model", "-p", "pf_name", default="default",
               help="Custom profile to use when checking pcvs.setup scripts")
+@click.option("--conversion/--no-conversion", "-t/-T", "conversion",
+              is_flag=True, default=True,
+              help="Enable/Disable auto-conversion through `pcvs_convert`")
 @click.pass_context
-def check(ctx, dir, encoding, color, configs, profiles, pf_name):
+def check(ctx, dir, encoding, color, configs, profiles, pf_name, conversion):
     """Global input/output analyzer, validating configuration, profiles &
     terminal supports."""
-    log.manager.print_banner()
+    io.console.print_banner()
     errors = dict()
     if color:
-        log.manager.print_header("Colouring")
-        t = PrettyTable()
-        ctx.color = True
-        t.field_names = ["Name", "Foreground", "Background"]
-        for k in sorted(log.manager.color_list):
-            t.add_row([k, click.style("Test", fg=k),
-                      click.style("Test", bg=k)])
-        print(t)
+        display = Panel.fit("\n".join([
+            "[red bold]Color[/], [i]Styles[/] & [underline]encoding[/] are managed by [cyan bold]Rich[/].",
+            "[green bold]Please[/] visit their project: https://github.com/Textualize/rich",
+            ":warning: To [underline]disable[/] [dim]Markups & Highlighting support[/]",
+            "please use `--no-color` to the [red blink]PCVS[/] root command."
+        ]))
+        io.console.print(display)
+        return
 
     if encoding:
-        log.manager.print_header("Encoding")
-
-        t = PrettyTable()
-        t.field_names = ["Alias", "Symbol", "Fallback"]
-        man_default = log.IOManager(0, False, 100, None, None)
-        man_unicode = log.IOManager(0, True, 100, None, None)
-
-        for k in sorted(man_default.avail_chars()):
-            t.add_row([k, man_unicode.utf(k), man_default.utf(k)])
-        print(t)
+        t = Table("Alias", "Symbol", "Fallback", title="UTF Support")
+        w = io.SpecialChar(utf_support=True)
+        wo = io.SpecialChar(utf_support=False)
+        for k in io.SpecialChar.__dict__.keys():
+            if k.startswith("_"):
+                continue
+            t.add_row(k, str(getattr(w, k)), str(getattr(wo, k)))
+        io.console.print(t)
+        return
 
     if configs:
-        log.manager.print_header("Configurations")
-        errors = {**errors, **pvUtils.process_check_configs()}
+        io.console.print_header("Configurations")
+        errors = {**errors, **pvUtils.process_check_configs(conversion=conversion)}
 
     if profiles:
-        log.manager.print_header("Profile(s)")
-        errors = {**errors, **pvUtils.process_check_profiles()}
+        io.console.print_header("Profile(s)")
+        errors = {**errors, **pvUtils.process_check_profiles(conversion=conversion)}
 
     if dir:
-        log.manager.print_header("Test directories")
-        log.manager.print_section("Prepare the environment")
+        io.console.print_header("Test directories")
+        io.console.print_section("Prepare the environment")
         # first, replace build dir with a temp one
         settings = MetaConfig()
         cfg_val = settings.bootstrap_validation({})
         cfg_val.set_ifdef('output', "/tmp/test")
         errors = {**errors, **
-                  pvUtils.process_check_directory(os.path.abspath(dir), pf_name)}
+                  pvUtils.process_check_directory(os.path.abspath(dir), pf_name, conversion=conversion)}
 
+    table = Table("Count", "Type of error",
+                  title="Classification of errors", expand=True)
     if errors:
-        log.manager.print_section("Classification of errors:")
-        table = PrettyTable()
-        table.field_names = ["Count", "Type of error"]
-
         for k, v in errors.items():
-            table.add_row([v, base64.b64decode(k).decode('utf-8')])
-
-        table.align["Count"] = "c"
-        table.align["Type of error"] = "l"
-        table.sortby = "Count"
-        table.reversesort = True
-        print(table)
+            table.add_row(str(v), base64.b64decode(k).decode('utf-8'))
+        io.console.print(table)
     else:
-        log.manager.print_section("{succ} {cg} {succ}".format(
-            succ=log.manager.utf('succ'),
-            cg=log.manager.style("Everything is OK!", fg='green', bold=True))
-        )
+        io.console.print("{succ} {cg} {succ}".format(
+            succ=io.console.utf('succ'),
+            cg="[green bold]Everything is OK![/]"
+        ))
 
 
 @click.command(name="clean", short_help="Remove artifacts generated from PCVS")
 @click.option("-f", "--force", "force", default=False, is_flag=True,
               help="Acknowledge there is no way back.")
 @click.option("-d", "--dry-run", "fake", default=False, is_flag=True,
               help="Print artefacts instead of deleting them")
@@ -158,59 +188,61 @@
               help="Manage cleanup process interactively")
 @click.option("--remove-dirs", "remove_build_dir", is_flag=True, default=False)
 @click.argument("paths", required=False, type=click.Path(exists=True), nargs=-1)
 @click.pass_context
 def clean(ctx, force, fake, paths, remove_build_dir, interactive):
     """Find & clean workspaces from PCVS artifacts (build & archives)"""
     if not fake and not force:
-        log.manager.warn(["IMPORTANT NOTICE:",
-                          "This command will delete files from previous run(s) and",
-                          "no recovery will be possible after deletion.",
-                          "Please use --force to indicate you acknowledge the risks",
-                          "and will face consequences in case of improper use.",
-                          "",
-                          "To list files to be deleted instead, you may use --dry-run."]
-                         )
+        io.console.warn("\n".join(["IMPORTANT NOTICE:",
+                                   "This command will delete files from previous run(s) and",
+                                   "no recovery will be possible after deletion.",
+                                   "Please use --force to indicate you acknowledge the risks",
+                                   "and will face consequences in case of improper use.",
+                                   "",
+                                   "To list files to be deleted instead, you may use --dry-run."]
+                                  ))
         sys.exit(0)
     if not paths:
         paths = [os.getcwd()]
 
-    log.manager.print_header("DELETION")
+    io.console.print_header("DELETION")
     for path in paths:
         for root, dirs, files in os.walk(path):
             # current root need to be cleaned
             if NAME_BUILDFILE in files:
-                log.manager.print_section("Found build: {}".format(root))
-                archives = [x for x in sorted(files) if x.startswith(
-                    'pcvsrun_') and x.endswith('.tar.gz')]
+                io.console.print_section("Found build: {}".format(root))
+
+                archive_dir = os.path.join(root, NAME_BUILD_ARCHIVE_DIR)
+                archives = sorted([x for x in os.listdir(archive_dir)])
+
                 if len(archives) == 0 and fake:
-                    log.manager.print_item("No archive found.")
+                    io.console.print_item("No archive found.")
                 else:
                     for f in archives:
                         arch_date = datetime.strptime(
                             f.replace('pcvsrun_', '').replace('.tar.gz', ''),
                             "%Y%m%d%H%M%S"
                         )
                         delta = datetime.now() - arch_date
                         if fake:
-                            log.manager.print_item('Age: {:>3} day(s): {}'.format(
+                            io.console.print_item('Age: {:>3} day(s): {}'.format(
                                 delta.days, f))
                             continue
                         elif interactive:
                             if not click.confirm('{}: ({} days ago) ?'.format(f, delta.days)):
                                 continue
-                        os.remove(os.path.join(root, f))
-                        log.manager.print_item('Deleting {}'.format(f))
+                        os.remove(os.path.join(archive_dir, f))
+                        io.console.print_item('Deleting {}'.format(f))
                 if remove_build_dir:
                     if not fake:
                         if interactive:
                             if not click.confirm('{}: ?'.format(root)):
                                 continue
                         shutil.rmtree(root)
-                        log.manager.print_item('Deleted {}'.format(root))
+                        io.console.print_item('Deleted {}'.format(root))
 
                 # stop the walk down to this top directory
                 dirs[:] = []
 
 
 @click.command(name="scan",
                short_help="Analyze directories to build up test conf. files")
@@ -222,9 +254,9 @@
     """Discover & integrate new benchmarks to PCVS format."""
     if not paths:
         paths = [os.getcwd()]
 
     paths = [os.path.abspath(x) for x in paths]
 
     for p in paths:
-        log.manager.print_section("{}".format(p))
+        io.console.print_section("{}".format(p))
         pvUtils.process_discover_directory(p, set, force)
```

### Comparing `pcvs-0.6.0/pcvs/converter/yaml_converter.py` & `pcvs-0.7.0/pcvs/converter/yaml_converter.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import sys
 
 import click
 import pkg_resources
 from ruamel.yaml import YAML
 
 import pcvs
-from pcvs import version
+from pcvs import io
 from pcvs.helpers import log
 from pcvs.helpers.exceptions import CommonException
 
 desc_dict = dict()
 
 
 def separate_key_and_value(s: str, c: str) -> tuple:
@@ -58,52 +58,67 @@
 
 
 def flatten(dd, prefix='') -> dict:
     """ make the n-depth dict 'dd' a "flat" version, where the successive keys
     are chained in a tuple. for instance:
     {'a': {'b': {'c': value}}} --> {('a', 'b', 'c'): value}
     """
-    return {prefix + "." + k if prefix else k: v
+    return {prefix + "||" + k if prefix else k: v
             for kk, vv in dd.items()
             for k, v in flatten(vv, kk).items()
             } if isinstance(dd, dict) else {prefix: dd}
 
 
 def compute_new_key(k, v, m) -> str:
     """replace in 'k' any pattern found in 'm'.
     'k' is a string with placeholders, while 'm' is a match result with groups
     named after placeholders.
     This function will also expand the placeholder if 'call:' token is used to
     execute python code on the fly (complex transformation)
     """
     replacement = ""
-    # basic replace the whole string with any placeholder
-    for elt in m.groupdict().keys():
-        k = k.replace("<"+elt+">", m.group(elt))
-
+    
+    # A tricky thing here. Recently we realised users may use a dot as a
+    # TE name, also used as a split pattern.
+    # To make the converter work again, any dot used to flatten the dict 
+    # is replaced with a "||".
+    # BUT dots in user-defined input & regexes should not be touched
+    # This is why the replacement is done BEFORE applying regex results.
+    # EXCEPTION: dynamic conversion through code execution cannot be parsed
+    # automatically and "||" need to be manually inserted (hard to say which dots
+    # are relevant).
+    
     # if this key is a special python expression to process:
     if k.startswith('call:'):
+        # basic replace the whole string with any placeholder
+        for elt in m.groupdict().keys():
+            k = k.replace("<"+elt+">", m.group(elt))
+
         env = {'k': k, 'v': v, 'm': m}
         # the 'k' & 'm' vars are exposed to evaluated code
         exec("import re\n"+k.split("call:")[1], env)
         # the 'k' is retrieved and used as a whole
         replacement = env['k']
     else:
+        # basic replace the whole string with any placeholder
+        for elt in m.groupdict().keys():
+            k = k.replace(".", "||").replace("<"+elt+">", m.group(elt))
+
         replacement = k
     return replacement
 
 
 def check_if_key_matches(key, value, ref_array) -> tuple:
     """list all matches for the current key in the new YAML description."""
     # for each key to be replaced.
     # WARNING: no order!
     for old_k, new_k in ref_array.items():
         # compile the regex (useful ?)
         r = re.compile(old_k)
-        if re.search(r, key) is not None:  # if the key exist
+        if re.fullmatch(r, key) is not None:  # if the key exist
             # CAUTION: we only parse the first match_obj iteration:
             # we do not consider a token to match multiple times in
             # the source key!
             res = next(r.finditer(key))
             # if there is a associated key in the new tree
             if new_k is not None:
                 if isinstance(new_k, list):
@@ -133,50 +148,49 @@
         # - valid = node changed = key has been found in the desc.
         # - dest_k = an array where each elt can be:
         #    * the new key value
         #    * the new key alongside with the transformed value as well
         # in the latter case, a split is required to identify key & value
         # an array is returned as a single node can produe multiple new nodes
         (valid, dest_k) = check_if_key_matches(k, v, ref_array)
-
         if valid:
-            log.manager.info("Processing {}".format(k))
+            io.console.info("Processing {}".format(k))
             # An empty array means the key does not exist in the new tree.
             # => discard
             if len(dest_k) <= 0:
                 continue
 
             # Process each of the new keys
             for elt_dest_k in dest_k:
                 (final_k, final_v, token) = (elt_dest_k, None, '')
                 # src key won't be kept
                 if final_k is None:
                     continue
                 # if a split is required
-                for token in ['+', '=']:
+                for token in ['|+|', '|=|']:
                     (final_k, final_v) = separate_key_and_value(elt_dest_k,
                                                                 token)
                     # the split() succeeded ? stop
                     if final_v:
                         break
 
                 # special case to handle the "+" operator to append a value
                 should_append = (token == '+')
                 # if none of the split() succeeded, just keep the old value
                 final_v = v if not final_v else final_v
                 # set the new key with the new value
-                set_with(output, final_k.split('.'), final_v, should_append)
+                set_with(output, final_k.split('||'), final_v, should_append)
         else:
             # warn when an old_key hasn't be declared in spec.
-            log.manager.info("DISCARDING {}".format(k))
+            io.console.info("DISCARDING {}".format(k))
             if warn_if_missing:
-                log.manager.warn("Key {} undeclared in spec.".format(k))
-                set_with(output, ['pcvs_missing'] + k.split("."), v)
+                io.console.warn("Key {} undeclared in spec.".format(k))
+                set_with(output, ['pcvs_missing'] + k.split("||"), v)
             else:
-                set_with(output, k.split("."), v)
+                set_with(output, k.split("||"), v)
     return output
 
 
 def process_modifiers(data):
     """applies rules in-place for the data dict.
     Rules are present in the desc_dict['first'] sub-dict."""
     if "first" in desc_dict.keys():
@@ -202,30 +216,30 @@
             insert = False
             for valid_k in refs.keys():
                 if valid_k in elt:
                     insert = True
                     replacement.append(elt.replace(valid_k, refs[valid_k]))
             if not insert:
                 replacement.append(re.escape(elt))
-        final[r"\.".join(replacement)] = new
+        final["\|\|".join(replacement)] = new
     return final
 
 
 def print_version(ctx, param, value) -> None:
     """print converter version number, tied to PCVS version number """
     if not value or ctx.resilient_parsing:
         return
     click.echo(
-        'PCVS Dynamic Converter (pcvs) -- version {}'.format(version.__version__))
+        'PCVS Dynamic Converter (pcvs) -- version {}'.format(pkg_resources.require("pcvs")[0].version))
     ctx.exit()
 
 
 @click.command("pcvs_convert", short_help="YAML to YAML converter")
 @click.option("-k", "--kind", "kind",
-              type=click.Choice(['compiler', 'runtime', 'environment', 'te'],
+              type=click.Choice(['compiler', 'runtime', 'environment', 'te', "profile"],
                                 case_sensitive=False),
               required=True, help="Select a kind to apply for the file")
 @click.option("-t", "--template", "template",
               type=click.Path(exists=True, dir_okay=False, readable=True),
               required=False, default=None,
               help="Optional template file (=group) to resolve aliases")
 @click.option("-s", "--scheme", "scheme", required=False, default=None,
@@ -242,96 +256,109 @@
               default=True, is_flag=True, show_envvar=True,
               help="enable/disable Unicode glyphs")
 @click.option("-o", "--output", "out", default=None,
               type=click.Path(exists=False, dir_okay=False),
               help="Filepath where to put the converted YAML")
 @click.option("--stdout", "stdout", is_flag=True, default=False,
               help="Print the stdout nothing but the converted data")
+@click.option("--skip-unknown", "skip_unknown", default=False, is_flag=True,
+              help="Missing keys are ignored and kept as is in final output")
+@click.option("--in-place", "in_place", is_flag=True, default=False,
+              help="Write conversion back to the original file (DESTRUCTIVE)")
 @click.argument("input_file", type=click.Path(exists=True, dir_okay=False,
                                               readable=True, allow_dash=True))
 @click.pass_context
-def main(ctx, color, encoding, verbose, kind, input_file, out, scheme, template, stdout) -> None:
+def main(ctx, color, encoding, verbose, kind, input_file, out, scheme, template, stdout, skip_unknown, in_place) -> None:
     """
     Process the conversion from one YAML format to another.
     Conversion specifications are described by the SCHEME file.
     """
-    # Click specific-related
+    # Click specific-related²
     ctx.color = color
     kind = kind.lower()
-    log.init(verbose, encoding, None)
-    log.manager.print_header("YAML Conversion")
+    io.init(stderr=True)
+    io.console.print_header("YAML Conversion")
+
+    if in_place and (stdout or out is not None):
+        raise click.BadOptionUsage("--stdout/--in-place", "Cannot use --in-place option with any other output options (--output/--stdout)")
+    elif in_place:
+        out = input_file
 
     if template is None and kind == "te":
-        log.manager.warn(
-            ["If the TE file contains YAML aliases, the conversion may",
-             "fail. Use the '--template' option to provide the YAML file",
-             "containing these aliases"])
+        io.console.warn("\n".join([
+            "If the TE file contains YAML aliases, the conversion may",
+            "fail. Use the '--template' option to provide the YAML file",
+            "containing these aliases"]))
+    if kind == "profile":
+        kind = ""
     # load the input file
     f = sys.stdin if input_file == '-' else open(input_file, 'r')
     try:
-        log.manager.print_item("Load data file: {}".format(f.name))
+        io.console.print_item("Load data file: {}".format(f.name))
         stream = f.read()
         if template:
-            log.manager.print_item("Load template file: {}".format(template))
+            io.console.print_item("Load template file: {}".format(template))
             stream = open(template, 'r').read() + stream
         data_to_convert = YAML(typ='safe').load(stream)
     except yaml.composer.ComposerError as e:
         CommonException.IOError(e, template)
 
     # load the scheme
     if not scheme:
         scheme = open(os.path.join(
             pcvs.PATH_INSTDIR, "converter/convert.json"))
-    log.manager.print_item("Load scheme file: {}".format(scheme.name))
+    io.console.print_item("Load scheme file: {}".format(scheme.name))
     tmp = json.load(scheme)
 
     # if modifiers are declared, replace token with regexes
     if '__modifiers' in tmp.keys():
         desc_dict['first'] = replace_placeholder(tmp['__modifiers'],
                                                  tmp['__tokens'])
     desc_dict['second'] = replace_placeholder(tmp,
                                               tmp['__tokens'])
 
-    log.manager.info(["Conversion list {old_key -> new_key):",
+    io.console.info(["Conversion list {old_key -> new_key):",
                      "{}".format(pprint.pformat(desc_dict))])
 
     # first, "flattening" the original array: {(1, 2, 3): "val"}
     data_to_convert = flatten(data_to_convert, kind)
 
     # then, process modifiers, altering original data before processing
-    log.manager.print_item("Process alterations to the original data")
+    io.console.print_item("Process alterations to the original data")
     data_to_convert = process_modifiers(data_to_convert)
     # as modifiers may have created nested dictionaries:
     # => "flattening" again, but with no prefix (persistent from first)
     data_to_convert = flatten(data_to_convert, "")
-
+    
     # Finally, convert the original data to the final yaml dict
-    log.manager.print_item("Process the data")
-    final_data = process(data_to_convert)
+    io.console.print_item("Process the data")
+    final_data = process(data_to_convert, warn_if_missing=not(skip_unknown))
 
+    # remove appended kind (if any)
+    final_data = final_data.get(kind, final_data)
     # remove template key from the output to avoid polluting the caller
-    log.manager.print_item("Pruning templates from the final data")
+    io.console.print_item("Pruning templates from the final data")
     invalid_nodes = [k for k in final_data.keys() if k.startswith('pcvst_')]
-    log.manager.info(["Prune the following:", "{}".format(
+    io.console.info(["Prune the following:", "{}".format(
         pprint.pformat(invalid_nodes))])
     [final_data.pop(x, None) for x in invalid_nodes + ["pcvs_missing"]]
 
-    log.manager.info(
+    io.console.info(
         ["Final layout:", "{}".format(pprint.pformat(final_data))])
 
     if stdout:
         f = sys.stdout
     else:
         if out is None:
             prefix, base = os.path.split(
                 "./file.yml" if input_file == "-" else input_file)
             out = os.path.join(prefix, "convert-" + base)
         f = open(out, "w")
 
-    log.manager.print_section("Converted data written into {}".format(f.name))
+    io.console.print_section("Converted data written into {}".format(f.name))
     YAML(typ='safe').dump(final_data, f)
 
     f.flush()
     if not stdout:
         f.close()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pcvs-0.6.0/pcvs/dsl/__init__.py` & `pcvs-0.7.0/pcvs/dsl/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,292 +1,327 @@
-from enum import Enum, IntEnum
+import json
 import os
-from typing import List
+from enum import Enum, IntEnum
+from typing import Dict, List
+
+from pcvs import io
+from pcvs.helpers import exceptions, git
 from pcvs.testing.test import Test
-from pcvs.helpers import git, exceptions
-import json
 
 
 class Job(Test):
     """Map a real job representation within a bank."""
     class Trend(IntEnum):
         REGRESSION = 0,
         PROGRESSION = 1,
         STABLE = 2
-        
 
-    def __init__(self, s=None):
+    def __init__(self, s=None) -> None:
         super().__init__()
         if isinstance(s, dict):
             self.from_json(s)
-    
-    def get_state(self):
+
+    def get_state(self) -> Test.State:
+        """Retrieve job state as stored in the Run.
+
+        :return: the state
+        :rtype: Test.State
+        """
         return self._state
-    
-    def get_date(self):
-        return None
-    
-    def load(self, s=""):
+
+    def load(self, s="") -> None:
+        """Populate the job with given data.
+
+        :param s: A Job's data dict representation
+        :type s: dict
+        """
         self.from_json(s)
 
-    def dump(self):
+    def dump(self) -> dict:
+        """Return serialied job data.
+
+        :return: the mapped representation
+        :rtype: dict
+        """
         return self.to_json()
 
 
 class Run:
     """Depict a given run -> Git commit
     """
+
     def __init__(self, repo=None, cid=None, from_serie=None):
-        """TODO:
+        """Create a new run.
+
+        :param repo: the associated repo this run is coming from
+        :type repo: Bank
         """
         # this attribute prevails
         if from_serie:
             repo = from_serie.repo
-            
+
         self._repo = repo
         self._stage = {}
         self._cid = None
-        
+
         if self._repo:
             self._cid = cid
-            #self.load()
-        
+            # self.load()
+
     def load(self, cid=None):
         if cid:
             self._cid = cid
-        #load into _stage the actual content ?
-        
+        # load into _stage the actual content ?
+
     @property
     def changes(self):
         return self._stage
-    
+
     @property
     def previous(self):
         l = self._repo.get_parents(self._cid)
         if l[0].get_info()['message'] == "INIT" or len(l) < 1:
             return None
         return Run(repo=self._repo, cid=l[0])
 
     @property
     def oneline(self):
         """TODO:
         """
-        assert(isinstance(self._cid, git.Commit))
+        assert (isinstance(self._cid, git.Commit))
         d = self._cid.get_info()
-        return "{}: {}".format(self._cid.short, d)
-    
+        return "{}".format(d)
+
     @property
-    def tests(self):
+    def jobs(self):
         for file in self._repo.list_files(rev=self._cid):
             data = self._repo.get_tree(rev=self._cid, prefix=file)
             job = Job(json.loads(str(data)))
             yield job
-        
+
+    @property
+    def get_full_data(self):
+        root = [j.to_json() for j in self.jobs]
+        return json.dumps(root)
+
     def get_data(self, jobname):
         res = Job()
         data = self._repo.get_tree(rev=self._cid, prefix=jobname)
         if not data:
             return data
-        
+
         res.from_json(str(data))
         return res
-        
+
     def update(self, prefix, data):
         if isinstance(data, Job):
             data = data.to_json()
-        
+
         if isinstance(data, dict):
-            data = json.dumps(data)
-    
+            data = json.dumps(data, default=lambda x: "Invalid type: {}".format(type(x)))
+
         self._stage[prefix] = data
 
     def update_flatdict(self, list_of_updates):
         for k, v in list_of_updates.items():
             self.update(k, v)
-    
+
     def __handle_subtree(self, prefix, subdict):
         for k, v in subdict.items():
             if not isinstance(v, dict):
                 self._stage[k] = v
             else:
                 self.__handle_subtree("{}{}/".format(prefix, k), v)
-        
+
     def update_treedict(self, list_of_updates):
         self.__handle_subtree("", list_of_updates)
-        
+
     def get_info(self):
         return self._cid.get_info()
 
     def get_metadata(self):
         raw_msg = self._cid.get_info()['message']
         meta = raw_msg.split('\n')[2]
         return json.loads(meta)
-        
+
 
 class Serie:
     """TODO:
     """
     class Request(IntEnum):
         """TODO:
         """
         REGRESSIONS = 0
         RUNS = 1,
-        
-    
+
     """Depicts an history of runs for a given project/profile.
     """
+
     def __init__(self, branch):
         """TODO:
         """
         self._hdl = branch
         self._repo = branch.repo
-    
+
     @property
     def repo(self):
         return self._repo
-    
+
     @property
     def name(self):
         return self._hdl.name
-    
+
     @property
     def last(self):
         """Return the last run for this serie.
         """
         return Run(self._repo, self._repo.revparse(self._hdl))
 
     def __len__(self):
         return len(self.find(self.Request.RUNS))
 
     def __str__(self):
         res = ""
         for run in self._repo.iterate_over(self._hdl):
             res += "* {}\n".format(Run(repo=self._repo, cid=run).oneline)
         return res
-    
+
     def history(self):
         res = []
-        
+
         parent = self.last
         while parent:
             res.append(parent)
             parent = parent.previous
-        
+
         return res
-    
+
     def find(self, op: Request, since=None, until=None, tree=None):
         """TODO:
         """
         res = None
-        
+
         if op == self.Request.REGRESSIONS:
             job = Test()
             res = []
             for raw_job in self._repo.diff_tree(tree=tree, src=self._hdl,
                                                 dst=None, since=since,
                                                 until=until):
                 job.from_json(raw_job)
                 if job.state != Test.State.SUCCESS:
                     res.append(job)
-                    
+
         elif op == self.Request.RUNS:
             res = []
             for elt in self._repo.list_commits(rev=self._hdl, since=since, until=until):
                 if elt.get_info()['message'] != "INIT":
                     res.append(Run(repo=self._repo, cid=elt))
         return res
-    
-    def commit(self, run, msg="Commit from Serie", metadata={}, timestamp=None):
-        assert(isinstance(run, Run))
+
+    def commit(self, run, msg=None, metadata={}, timestamp=None):
+        assert (isinstance(run, Run))
         root_tree = None
+        msg = "New run" if not msg else msg
         try:
             raw_metadata = json.dumps(metadata)
         except:
             raw_metadata = ""
 
         commit_msg = """{}
 
 {}""".format(msg, raw_metadata)
-        
+
         for k, v in run.changes.items():
             root_tree = self._repo.insert_tree(k, v, root_tree)
-        self._repo.commit(tree=root_tree, msg=commit_msg, 
+        self._repo.commit(tree=root_tree, msg=commit_msg,
                           parent=self._hdl, timestamp=timestamp, orphan=False)
-        #self._repo.gc()
+        # self._repo.gc()
 
 
 class Bank:
     """
     Bank view from Python API
     """
+
     def __init__(self, path="", head=None):
-        self._path = path        
+        self._path = path
         self._repo = git.elect_handler(self._path)
-        self._repo.open()
 
+        self._repo.open()
         if head:
             self._repo.set_head(head)
+        else:
+            first_branch = [
+                b for b in self._repo.branches if b.name != "master"]
+            if len(first_branch) <= 0:
+                io.console.warn(
+                    "This repository seems empty: {}".format(self._path))
+            else:
+                self._repo.set_head(first_branch[0].name)
 
         if not self._repo.get_branch_from_str('master'):
-            t = self._repo.insert_tree('README', "This file is intended to be used as a branch bootstrap.")
+            t = self._repo.insert_tree(
+                'README', "This file is intended to be used as a branch bootstrap.")
             c = self._repo.commit(t, "INIT", orphan=True)
             self._repo.set_branch(git.Branch(self._repo, 'master'), c)
 
     @property
     def path(self):
         return self._path
-    
+
     def set_id(self, an, am, cn, cm):
         self._repo.set_identity(an, am, cn, cm)
-    
+
     def connect(self):
         self._repo.open()
-        
+
     def disconnect(self):
         if self._repo:
             self._repo.close()
-    
+
     def new_serie(self, serie_name=None):
         hdl = self._repo.new_branch(serie_name)
         return Serie(hdl)
-    
+
     def get_serie(self, serie_name=None):
         """TODO
         """
         if not serie_name:
             serie_name = self._repo.get_head().name
-        
+
         branch = self._repo.get_branch_from_str(serie_name)
+    
         if not branch:
             return None
-        
+
         return Serie(branch)
 
     def list_series(self, project=None):
         """TODO:
         """
         res = []
         for elt in self._repo.branches:
             array = elt.name.split('/')
             if project is None or array[0].lower() == project.lower():
                 res.append(Serie(elt))
         return res
 
-    def list_all(self):
+    def list_all(self) -> Dict[str, List]:
         """TODO:
         """
         res = {}
         for project in self.list_projects():
-            res[project] = self.list_series(project)
+            if project != "master":
+                res[project] = self.list_series(project)
         return res
-    
+
     def list_projects(self) -> List[str]:
         """Given the bank, list projects with at least one run.
 
         In a bank, each branch is a project, just list available branches.
         `master` branch is not a valid project.
 
         :return: A list of available projects
         :rtype: list of str
         """
-        projects = [elt.name.split('/')[0] for elt in self._repo.branches]
+        projects = [elt.name.split('/')[0] for elt in self._repo.branches if elt.name != "master"]
         return list(set(projects))
```

### Comparing `pcvs-0.6.0/pcvs/dsl/analysis.py` & `pcvs-0.7.0/pcvs/dsl/analysis.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,35 +1,40 @@
+import json
 from abc import ABC, abstractmethod
-from pcvs.dsl import Serie, Run, Job
+
+from pcvs.dsl import Job, Run, Serie
 from pcvs.testing.test import Test
-import json
+
 
 class BaseAnalysis(ABC):
     """TODO:
     """
+
     def __init__(self, bank):
         self._bank = bank
-    
+
+
 class SimpleAnalysis(BaseAnalysis):
     """TODO:
     """
+
     def __init__(self, bank):
         super().__init__(bank)
-        
+
     def generate_serie_trend(self, serie, start=None, end=None):
         """TODO:
         """
         if not isinstance(serie, Serie):
             serie = self._bank.get_serie(serie)
         stats = []
         for run in serie.find(Serie.Request.RUNS, start, end):
             ci_meta = run.get_info()
             run_meta = run.get_metadata()
             stats.append({'date': ci_meta['date'], **run_meta})
-        
+
         return stats
 
     def generate_weighted_divergence(self, serie, threshold=0, prefix=None):
         """TODO:
         """
         if not isinstance(serie, Serie):
             serie = self._bank.get_serie(serie)
@@ -58,17 +63,17 @@
             stats[div][testname] = weight
         return stats
 
 
 class ResolverAnalysis(BaseAnalysis):
     """TODO:
     """
-    
+
     def __init__(self, bank):
         super().__init__(bank)
         self._data = None
-        
+
     def fill(self, data):
         """TODO:
         """
-        assert(isinstance(data, dict))
+        assert (isinstance(data, dict))
         self._data = data
```

### Comparing `pcvs-0.6.0/pcvs/dsl/render.py` & `pcvs-0.7.0/pcvs/dsl/render.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,31 +1,32 @@
+from matplotlib import pyplot as plt
+
 from pcvs.dsl import Bank
-from pcvs.testing.test import Test
 from pcvs.dsl.analysis import SimpleAnalysis
-from matplotlib import pyplot as plt
+from pcvs.testing.test import Test
 
 
 def generate_serie_trend(res, out):
     x = []
     total = []
     succ = []
     fail = []
     other = []
 
     for e in res:
         nb = sum(e['cnt'].values())
         total.append(nb)
         succ.append(e['cnt'][str(Test.State.SUCCESS)])
         fail.append(e['cnt'][str(Test.State.FAILURE)])
-        other.append(nb - e['cnt'][str(Test.State.SUCCESS)] - e['cnt'][str(Test.State.FAILURE)])
-        
+        other.append(nb - e['cnt'][str(Test.State.SUCCESS)
+                                   ] - e['cnt'][str(Test.State.FAILURE)])
 
     x = [e['date'] for e in res]
     total = [e['cnt'][str(Test.State.SUCCESS)] for e in res]
     succ = [e['cnt'][str(Test.State.SUCCESS)] for e in res]
     fail = [e['cnt'][str(Test.State.FAILURE)] for e in res]
     other = [e['cnt'][str(Test.State.FAILURE)] for e in res]
 
-    plt.stackplot(x, fail, succ, labels=["FAILURE", "SUCCESS"], colors=['red', 'green'])
+    plt.stackplot(x, fail, succ, labels=[
+                  "FAILURE", "SUCCESS"], colors=['red', 'green'])
     plt.legend()
     plt.savefig(fname=out)
-
```

### Comparing `pcvs-0.6.0/pcvs/helpers/communications.py` & `pcvs-0.7.0/pcvs/helpers/communications.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,15 @@
     def retry_pending(self):
         while len(self._waitlist) > 0:
             prev_test = self._waitlist.pop()
             if not self._send_unitary_test(prev_test):
                 self._waitlist.append(prev_test[1])
 
     def _send_unitary_test(self, test):
-        assert(isinstance(test, Test))
+        assert (isinstance(test, Test))
         to_send = {"metadata": self._metadata,
                    "test_data": test.to_json(),
                    "state": test.state}
         return self._json_send("/submit/test", to_send)
 
     def _json_send(self, prefix, json_data):
         try:
```

### Comparing `pcvs-0.6.0/pcvs/helpers/criterion.py` & `pcvs-0.7.0/pcvs/helpers/criterion.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import base64
 import itertools
 import math
 import os
 
-from pcvs.helpers import log
+from pcvs import io
 from pcvs.helpers.exceptions import CommonException
 from pcvs.helpers.system import MetaConfig
 from pcvs.plugins import Plugin
 
 
 class Combination:
     """A combination maps the actual concretization from multiple criterion.
@@ -57,15 +57,15 @@
         c = self._criterions
         string = list()
         # each combination is built following: 'defined-prefix+value'
         for n in sorted(self._combination.keys()):
             subtitle = c[n].subtitle
             if subtitle is None:
                 subtitle = "{}".format(n)
-                
+
             string.append(subtitle +
                           str(self._combination[n]).replace(" ", "-"))
         return "_".join(string)
 
     def translate_to_command(self):
         """Translate the actual combination is tuple of three elements, based
         on the representation of each criterion in the test semantic. It builds
@@ -121,16 +121,16 @@
         :param dict_of_criterion: values to build the serie with
         :type dict_of_criterion: dict"""
         self._values = list()
         self._keys = list()
         # this has to be saved, need to be forwarded to each combination
         self._dict = dict_of_criterion
         for name, node in dict_of_criterion.items():
-            assert(isinstance(node, Criterion))
-            assert(name == node.name)
+            assert (isinstance(node, Criterion))
+            assert (name == node.name)
             self._values.append(node.values)
             self._keys.append(node.name)
 
     def generate(self):
         """Generator to build each combination"""
         for combination in itertools.product(*self._values):
             d = {self._keys[i]: val for i, val in enumerate(combination)}
@@ -167,37 +167,62 @@
         self._after = description.get('position', 'after') == 'after'
         self._alias = description.get('aliases', {})
         self._is_env = description.get('type', 'argument') == 'environment'
         # this should be only set by per-TE criterion definition
         self._local = local
         self._str = description.get('subtitle', None)
         self._values = description.get('values', [])
+        self._expanded = False
+        #Sanity check
+        self.sanitize_values()
+
+    def sanitize_values(self):
+        """
+        Check for any inconsistent values in the current Criterion.
+        
+        Currently, only scalar items or dict (=> sequence) are allowed.
+        Will raise an exeption in case of inconsistency (Maybe this should be
+        managed in another way through the error handling)
+        """
+        if self.is_discarded():
+            return
         if not isinstance(self._values, list):
             self._values = [self._values]
+        for v in self._values:
+            if isinstance(v, list):
+                raise CommonException.UnclassifiableError(
+                    reason="list elements should be scalar OR dict",
+                    dbg_info={"element": v}
+                )
+            if isinstance(v, dict):
+                for key in v.keys():
+                    assert key in ['op', 'of', 'from', 'to']
+            
 
     # only allow overriding values (for now)
-
     def override(self, desc):
         """Replace the value of the criterion using a descriptor containing the
             said value
 
         :param desc: descriptor supposedly containing a ``value``entry
         :type desc: dict
         """
         if 'values' in desc:
             self._values = desc['values']
-
+            self._expanded = False
+            self.sanitize_values()
+    
     def intersect(self, other):
         """Update the calling Criterion with the interesection of the current
         range of possible values with the one given as a parameters.
 
         This is used to refine overriden per-TE criterion according to 
         system-wide's"""
-        assert(isinstance(other, Criterion))
-        assert(self._name == other._name)
+        assert (isinstance(other, Criterion))
+        assert (self._name == other._name)
 
         # None is special value meaning, discard this criterion because
         # irrelevant
         if self._values is None or other._values is None:
             self._values = None
         else:
             self._values = set(self._values).intersection(other._values)
@@ -364,68 +389,96 @@
             if of == 0:
                 values.append()
             start = math.ceil(start**(1/of))
             end = math.floor(end**(1/of))
             for i in range(start, end+1):
                 values.append(i**of)
         else:
-            log.manager.warn("failure in Criterion sequence!")
+            io.console.warn("failure in Criterion sequence!")
 
         return values
 
-    def expand_values(self):
+    @property
+    def expanded(self):
+        return self._expanded
+    
+    @property
+    def min_value(self):
+        assert(self.expanded)
+        return min(self._values)
+    
+    @property
+    def max_value(self):
+        assert(self.expanded)
+        return max(self._values)
+    
+    def expand_values(self, reference=None):
         """Browse values for the current criterion and make it ready to
         generate combinations"""
         values = []
-
+        start = 0
+        end = 100
+        
+        if self.expanded:
+            return
+        if reference:
+            assert isinstance(reference, Criterion)
+            if not reference.expanded:
+                reference.expand_values()
+            start = reference.min_value
+            end = reference.max_value
+        
+        io.console.debug("Expanding {}: {}".format(self.name, self._values))
         if self._numeric is True:
             for v in self._values:
+                
                 if isinstance(v, dict):
-                    values += self.__convert_sequence_to_list(v, s=0, e=100)
+                    values += self.__convert_sequence_to_list(v, s=start, e=end)
                 elif isinstance(v, (int, float, str)):
                     values.append(v)
                 else:
                     raise TypeError("Only accept int or sequence (as string)"
                                     " as values for numeric iterators")
         else:
             values = self._values
         # now ensure values are unique
         self._values = set(values)
-
+        self._expanded = True
+        io.console.debug("EXPANDED {}: {}".format(self.name, self._values))
         # TODO: handle criterion dependency (ex: n_mpi: ['n_node * 2'])
 
 
 def initialize_from_system():
     """Initialise system-wide criterions
 
     TODO: Move this function elsewhere."""
     # sanity checks
     if not MetaConfig.root.criterion:
         MetaConfig.root.set_internal('crit_obj', {})
     else:
         # raw YAML objects
-        runtime_iterators = MetaConfig.root.runtime.iterators
-        criterion_iterators = MetaConfig.root.criterion.iterators
+        runtime_iterators = MetaConfig.root.runtime.criterions
+        criterion_iterators = MetaConfig.root.criterion
         it_to_remove = []
 
         # if a criterion defined in criterion.yaml but
         # not declared as part of a runtime, the criterion
         # should be silently discarded
         # here is the purpose
         for it in criterion_iterators.keys():
             if it not in runtime_iterators:
-                log.manager.warn("Undeclared criterion "
+                io.console.warn("Undeclared criterion "
                                 "as part of runtime: '{}' ".format(it))
             elif criterion_iterators[it]['values'] is None:
-                log.manager.debug('No combination found for {},'
-                                ' removing from schedule'.format(it))
+                io.console.debug('No combination found for {},'
+                                 ' removing from schedule'.format(it))
             else:
                 continue
 
-            log.manager.info("Removing '{}'".format(it))
+            io.console.info("Removing '{}'".format(it))
             it_to_remove.append(it)
 
         # register the new dict {criterion_name: Criterion object}
         # the criterion object gathers both information from runtime & criterion
         MetaConfig.root.set_internal('crit_obj', {k: Criterion(
             k, {**runtime_iterators[k], **criterion_iterators[k]}) for k in criterion_iterators.keys() if k not in it_to_remove})
```

### Comparing `pcvs-0.6.0/pcvs/helpers/exceptions.py` & `pcvs-0.7.0/pcvs/helpers/exceptions.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-class GenericError(Exception):
+class GenericException(Exception):
     """Generic error (custom errors will inherit of this)."""
 
-    def __init__(self, err_msg="Unkown error",
+    def __init__(self, reason="Unkown error",
                  help_msg="Please check pcvs --help for more information.",
                  dbg_info={}):
         """Constructor for generic errors.
         :param *args: unused
         :param **kwargs: messages for the error.
         """
-        self._err_msg = "{} - {}".format(type(self).__name__, err_msg)
         self._help_msg = help_msg
         self._dbg_info = dbg_info
-
+        super().__init__("{} - {}".format(type(self).__name__, reason))
+        
     def __str__(self):
         """Stringify an exception for pretty-printing.
 
         :return: the string.
         :type: str"""
         dbg_str = ""
         if self._dbg_info:
-            dbg_str = "\n\nExtra infos:\n" + self.dbg_str
+            dbg_str = "\n\nAdditional notes:\n" + self.dbg_str
         return "{}\n{}{}".format(
-            self._err_msg,
+            super().__str__(),
             self._help_msg,
             dbg_str
         )
 
     @property
     def err(self):
         """returns the error part of the exceptions.
 
         :return: only the error part
         :rtype: str"""
-        return self._err_msg
-
+        return str(self)
+    
     @property
     def help(self):
         """returns the help part of the exceptions.
 
         :return: only the help part
         :rtype: str"""
         return self._help_msg
@@ -46,14 +46,19 @@
     def dbg(self):
         """returns the extra infos of the exceptions (if any).
 
         :return: only the debug infos.
         :rtype: str"""
         return self._dbg_info
 
+    def add_dbg(self, **kwargs):
+        for k, v in kwargs.items():
+            if k not in self._dbg_info:
+                self._dbg_info[k] = v
+
     @property
     def dbg_str(self):
         """Stringify the debug infos. These infos are stored as a dict
 initially.
 
         :return: a itemized string.
         :rtype: str"""
@@ -61,192 +66,220 @@
             return " - None"
         w = max([len(k) for k in self._dbg_info.keys()])
         return "\n".join([" - {:<{w}}: {}".format(k, v, w=w) for k, v in self._dbg_info.items()])
 
 
 class CommonException:
     """Gathers exceptions commonly encountered by more specific namespaces."""
+    class NotPCVSRelated(GenericException):
+        pass
 
-    class AlreadyExistError(GenericError):
+    class AlreadyExistError(GenericException):
         """The content already exist as it should."""
-        def __init__(self, msg="Invalid format", **kwargs):
+
+        def __init__(self, reason="Already Exist", **kwargs):
             """Updated constructor"""
-            super().__init__(err_msg=msg,
+            super().__init__(reason=reason,
                              help_msg="\n".join([
                                  "Note configuration, profiles & pcvs.* files can be ",
                                  "verified through `pcvs check [-c|-p|-D <path>]`"]),
                              dbg_info=kwargs)
 
-    class UnclassifiableError(GenericError):
+    class UnclassifiableError(GenericException):
         """Unable to classify this common error."""
         pass
 
-    class NotFoundError(GenericError):
+    class NotFoundError(GenericException):
         """Content haven't been found based on specifications."""
-
         pass
 
-    class IOError(GenericError):
+    class IOError(GenericException):
         """Communication error (FS, process) while processing data."""
-
         pass
 
-    class BadTokenError(GenericError):
+    class BadTokenError(GenericException):
         """Badly formatted string, unable to parse."""
-
         pass
 
-    class WIPError(GenericError):
+    class WIPError(GenericException):
         """Work in Progress, not a real error."""
         pass
 
-    class TimeoutError(GenericError):
+    class TimeoutError(GenericException):
         """The parent class timeout error."""
         pass
 
-    class NotImplementedError(GenericError):
+    class NotImplementedError(GenericException):
         """Missing implementation for this particular feature."""
+        pass
 
 
 class BankException(CommonException):
     "Bank-specific exceptions."""
-    class ProjectNameError(GenericError):
+    class ProjectNameError(GenericException):
         """name is not a valid project under the given bank."""
         pass
 
 
 class ConfigException(CommonException):
     """Config-specific exceptions."""
-
     pass
 
 
 class ProfileException(CommonException):
     """Profile-specific exceptions."""
 
-    class IncompleteError(GenericError):
+    class IncompleteError(GenericException):
         """A configuration block is missing to build the profile."""
-
         pass
 
 
 class ValidationException(CommonException):
     """Validation-specific exceptions."""
 
-    class FormatError(GenericError):
+    class FormatError(GenericException):
         """The content does not comply the required format (schemes)."""
+        def __init__(self, reason="Invalid format", **kwargs):
+            """Updated constructor"""
+            super().__init__(reason=reason,
+                             help_msg="\n".join([
+                                 "Input files may be checked with `pcvs check`"]),
+                             dbg_info=kwargs)
+            
+    class WrongTokenError(GenericException):
+        """A unknown token is found in valided content"""
 
-        def __init__(self, msg="Invalid format", **kwargs):
+        def __init__(self, reason="Invalid token(s) used as Placeholders", **kwargs):
             """Updated constructor"""
-            super().__init__(err_msg=msg,
+            super().__init__(reason=reason,
                              help_msg="\n".join([
-                                 "Note configuration, profiles & pcvs.* files can be ",
-                                 "verified through `pcvs check [-c|-p|-D <path>]`"]),
+                                 "A list of valid tokens is available in the documentation"]),
                              dbg_info=kwargs)
 
-    class SchemeError(GenericError):
+    class SchemeError(GenericException):
         """The content is not a valid format (scheme)."""
 
-        def __init__(self, msg="Invalid Scheme provided", **kwargs):
+        def __init__(self, reason="Invalid Scheme provided", **kwargs):
             """Updated constructor"""
-            super().__init__(err_msg=msg,
+            super().__init__(reason=reason,
                              help_msg="\n".join([
                                  "Provided schemes should be static. If code haven't be",
                                  "changed, please report this error."]),
                              dbg_info=kwargs)
 
 
 class RunException(CommonException):
     """Run-specific exceptions."""
 
-    class InProgressError(GenericError):
+    class InProgressError(GenericException):
         """A run is currently occuring in the given dir."""
 
-        def __init__(self, msg="Execution in progress in this build directory", **kwargs):
+        def __init__(self, reason="Build directory currently used by another instance", **kwargs):
             """Updated constructor"""
-            super().__init__(err_msg=msg,
+            super().__init__(reason=reason,
                              help_msg="\n".join([
                                  "Please Wait for previous executions to complete.",
-                                 "You may also use --override or --output to change",
-                                 "the default build directory path"]),
+                                 "You may also use --override or --output to change default build directory"]),
                              dbg_info=kwargs)
 
-    class ProgramError(GenericError):
-        """The given program cannot be found."""
+    class NonZeroSetupScript(GenericException):
+        """a setup script (=pcvs.setup) completed but returned non-zero exit code."""
 
-        def __init__(self, msg="Program cannot be found", **kwargs):
+        def __init__(self, reason="A setup script failed to complete", **kwargs):
             """Updated constructor"""
-            super().__init__(err_msg=msg,
+            super().__init__(reason=reason,
                              help_msg="\n".join([
-                                 "A program/binary defined in loaded profile cannot",
-                                 "be found in $PATH or spack/module. Please report",
-                                 "if this is a false warning."]),
+                                 "Try to run manually the setup script below."]),
                              dbg_info=kwargs)
 
-    class TestUnfoldError(GenericError):
-        """Issue raised during processing test files."""
+    class ProgramError(GenericException):
+        """The given program cannot be found."""
 
-        def __init__(self, msg="Issue(s) while parsing test input", **kwargs):
+        def __init__(self, reason="A program cannot be found", **kwargs):
             """Updated constructor"""
-            super().__init__(err_msg=msg,
+            super().__init__(reason=reason,
                              help_msg="\n".join([
-                                 "Test directories can be checked beforehand with `pcvs check -D <path>`",
-                                 "See pcvs check --help for more information."]),
+                                 "A program/binary defined in loaded profile cannot",
+                                 "be found in $PATH or spack/module. Please report",
+                                 "if this is a false warning."]),
                              dbg_info=kwargs)
 
 
 class TestException(CommonException):
     """Test-specific exceptions."""
 
-    class TDFormatError(GenericError):
+    class TestExpressionError(GenericException):
         """Test description is wrongly formatted."""
 
-        pass
-
-    class DynamicProcessError(GenericError):
-        """Test File is not properly formatted."""
-        pass
+        def __init__(self, reason="Issue(s) while parsing a Test Descriptor", **kwargs):
+            """Updated constructor"""
+            super().__init__(reason=reason,
+                             help_msg="\n".join([
+                                 "Please check input files with `pcvs check`"]),
+                             dbg_info=kwargs)
 
 
 class OrchestratorException(CommonException):
     """Execution-specific errors."""
 
-    class UndefDependencyError(GenericError):
+    class UndefDependencyError(GenericException):
         """Declared job dep cannot be fully qualified, not defined."""
-
         pass
 
-    class CircularDependencyError(GenericError):
+    class CircularDependencyError(GenericException):
         """Circular dep detected while processing job dep tree."""
+        pass
 
+class RunnerException(CommonException):
+    class LaunchError(GenericException):
+        """Unable to run a remote container"""
+        pass
+    
+class PublisherException(CommonException):
+    class BadMagicTokenError(GenericException):
+        """Issue with token stored to file to check consistency"""
         pass
 
+    class UnknownJobError(GenericException):
+        """Unable to identify a job by its ID"""
+        pass
+    
+    class AlreadyExistJobError(GenericException):
+        """A single ID leads to multiple jobs."""
+        pass
+        
 
 class LockException(CommonException):
     """Lock-specific exceptions."""
 
-    class BadOwnerError(GenericError):
+    class BadOwnerError(GenericException):
         """Attempt to manipulate the lock while the current process is not the
         owner."""
         pass
 
-    class TimeoutError(GenericError):
+    class TimeoutError(GenericException):
         """Timeout reached before lock."""
         pass
 
 
 class PluginException(CommonException):
     """Plugin-related exceptions."""
 
-    class BadStepError(GenericError):
+    class BadStepError(GenericException):
         """targeted pass does not exist."""
         pass
 
-    class LoadError(GenericError):
+    class LoadError(GenericException):
         """Unable to load plugin directory."""
-        pass
+        def __init__(self, reason="Issue(s) while loading plugin", **kwargs):
+            """Updated constructor"""
+            super().__init__(reason=reason,
+                             help_msg="\n".join([
+                                 "Please ensure plugins can be imported like:",
+                                 "python3 ./path/to/plugin/file.py"]),
+                             dbg_info=kwargs)
 
-class SpackException(CommonException):
-    pass
 
 class GitException(CommonException):
-    pass
+    class BadEntryError(GenericException):
+        pass
+
```

### Comparing `pcvs-0.6.0/pcvs/helpers/git.py` & `pcvs-0.7.0/pcvs/helpers/git.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,31 @@
+import fcntl
 import getpass
-import socket
+import hashlib
 import os
+import socket
 import time
-import fcntl
-import hashlib
-import sh
-from datetime import datetime
 from abc import ABC, abstractmethod, abstractproperty
-from pcvs.helpers import utils
+from datetime import datetime
+
+import sh
 
+from pcvs.helpers import utils
+from pcvs.helpers.exceptions import GitException
 
 try:
     import pygit2
     has_pygit2 = True
 except ModuleNotFoundError as e:
     has_pygit2 = False
 
+
 def elect_handler(prefix=None):
     """Select the proper repository handler based on python support
-    
+
     Python 3.7+-based PCVS installations come with pygit2, thanks to provided
     wheels. Older versions are relying on regular Git commands (as wheels are
     not provided for Python3.6 and older & building pygit2 requires specific
     libgit2 version to be installed, hardening the installation process)
     """
     if has_pygit2:
         git_handle = GitByAPI(prefix)
@@ -31,50 +34,60 @@
 
     return git_handle
 
 
 class Reference:
     """Maps an object which can be "pointed" (as a Git semantic). It can usually
     be used to refer a commit, a simple hash or a branch. """
+
     def __init__(self, repo):
         self._repo = repo
-        
+
     @property
     def repo(self):
         """Getter to the repo this reference comes from."""
         return self._repo
 
 
 class Branch(Reference):
     """Maps to a regular Git branch."""
+
     def __init__(self, repo, name='master'):
         super().__init__(repo)
-        self.name = name
+        self._name = name
+    
+    @property
+    def name(self):
+        return self._name
+
 
 class Commit(Reference):
     """Maps to a regular Git commit"""
+
     def __init__(self, repo, obj, metadata={}):
         super().__init__(repo)
         self.cid = obj
         self.meta = metadata
-    
+
     def get_info(self):
         """Return commit metadata stored as a dict.
-        
+
         It may contains extra infos compared to what a commit usually contains"""
         return self.meta
 
+
 class Tree(Reference):
     """Maps to a git-lowlevel Tree object"""
+
     def __init__(self, repo, id, prefix='', children=[]):
         super().__init__(repo)
         self.tid = id
         self.prefix = prefix
         self.children = children
-    
+
     @classmethod
     def as_root(self, repo, hdl, children=[]):
         """Create a Tree and attach it with the git-specific handler (if any)
 
         :param repo: the repo handle
         :type repo: any
         :param hdl: the git-specific root handle
@@ -83,199 +96,206 @@
         :type children: any
         :return: the created Tree object
         :rtype: Tree
         """
         self.hdl = hdl
         return self(repo=repo, id=None, prefix='', children=children)
 
+
 class Blob(Tree):
     """Maps a Git 'blob' object, dedicated to hold data ("leaves" in Git trees)"""
+
     def __init__(self, repo, id, prefix='', data=''):
         super().__init__(repo, id, prefix, children=[])
         self.data = data
-    
+
     def __str__(self):
         """Stringify data contained in blob.
-        
+
         :returns: the decoded data
         :rtype: bytes
         """
         return self.data.decode()
 
+
 class GitByGeneric(ABC):
     """
     Create a Git endpoint able to discuss efficiently with repositories.
-    
+
     This base classe serves abstract methods to be implemented to create a new
     derived class. Currently are provided:
     - GitByAPI: relies on python module pygit2 (requires libgit2)
     - GitByCLI: based on regular Git program invocations (require git program)
     """
-    
+
     def __init__(self, prefix=None, head="unknown/00000000"):
         self._path = None
         self._lockname = ""
         self._lockfd = None
         self._authname = None
         self._authmail = None
         self._commmail = None
         self._commname = None
-        
+
         self.set_head(head)
-        
-        if prefix:        
+
+        if prefix:
             self.set_path(prefix)
 
         self.set_identity(None, None, None, None)
 
     @abstractmethod
     def open(self, bare=True):
         """Open the repo, with appropriate method.
-        
+
         :param bare: true by default, manage or bare repo.
         :type bare: boolean
         """
         pass
 
     def set_path(self, prefix):
         """
         Associate a new directory to this bank.
-        
+
         :param prefix: the prefix locating the Git repo
         :type prefix: str
         """
         self._path = prefix
         self._lockname = os.path.join(prefix, ".pcvs")
-        
+
     def _trylock(self):
         """
         Lock the current repository (NON-BLOCKING)
-        
+
         :return: true if the file is locked, false otherwise
         :rtype: boolean
         """
         return utils.trylock_file(self._lockname)
-       
-        
+
     def _lock(self):
         """
         Lock the current reposiotry (BLOCKING)
-        
+
         :return: true if the file is locked, false otherwise
         :rtype: boolean
         """
         return utils.lock_file(self._lockname)
-    
+
     def _unlock(self):
         """
         Unlock the current repository.
         """
         utils.unlock_file(self._lockname)
-    
+
     def _is_locked(self):
         """Locked repo checker
-        
+
         :return: true if the file is locked, false otherwise
         :rtype: boolean
         """
         utils.is_locked(self._lockname)
-            
+
     def set_identity(self, authname, authmail, commname, commmail):
         """Identities to be used if a commit is created.
-        
+
         :param authname: author's name
         :type authname: str
         :param authmail: author's email
         :type authmail: str
         :param commname: Committer's name
         :type commname: str
         :param commmail: Committer's email
         :type commmail: str
         """
         self._authname = authname if authname else get_current_username()
         self._authmail = authmail if authmail else get_current_usermail()
         self._commname = commname if commname else get_current_username()
         self._commmail = commmail if commmail else get_current_usermail()
-    
+
     def get_head(self):
         """Get the current repo's HEAD (used when no default)
-        
+
         :returns: a ref to the HEAD as a branch
         :rtype: Branch
         """
         return self._head
-    
+
     def set_head(self, new_head):
         """Move the repo HEAD (used when no default ref is provided)"""
         self._head = Branch(self, new_head)
-   
+
     @abstractproperty
     def branches(self):
         """
         Returns the list of available local branche names from this repo.
-    
+
         This is an abstract function as its behavior depends on derived classes.
         """
         pass
-    
+
     @abstractmethod
     def open(self):
         """Open a new directory. Also lock to avoid races."""
         pass
+
     @abstractmethod
     def is_open(self):
         """Is the directory currently open ?"""
         pass
+
     @abstractmethod
     def close(self):
         """Unlock the repository."""
         pass
+
     @abstractmethod
     def get_tree(self, tree, prefix):
         """Retrieve data associated with a given prefix. A tree can used
         to set which ref should be used.
-        
+
         :param[in] tree: the ref from where get the data
         :param[in] prefix: the unique prefix associated with data
         """
         pass
-    
+
     @abstractmethod
     def insert_tree(self, prefix, data):
         """Create a new tree mapping a prefix filled with 'data'.
-        
+
         :param[in] prefix: the prefix under Git tree.
         :param[in] data: the data to store.
         """
         pass
+
     @abstractmethod
     def diff_tree(self, prefix, src_rev, dst_rev):
         """
         Compare & return the list of patches 
         """
         pass
+
     @abstractmethod
-    def list_commits(self, rev, since, until): 
+    def list_commits(self, rev, since, until):
         """List past commits finishing with 'rev'.
-        
+
         The list can be shrunk with a start & end
-        
+
         :param rev: the revision to extract commit from
         :typ rev: any
         :param since: the oldest commit should be newer than this date
         :type since: date
         :param until: the newest commit should be older than this date
         :type until: date
         """
         pass
-    
+
     @abstractmethod
     def commit(self, tree, msg="No data", timestamp=None, parent=None, orphan=False):
         """Create a commit from changes.
-        
+
         :param tree: the changes tree to store as a commit
         :type tree: any
         :param msg: the commit msg
         :type msg: str
         :timestamp: a commit date (current if not provided)
         :type: int
         :param parent: the parent commit
@@ -285,108 +305,109 @@
         """
         pass
 
     @abstractmethod
     def revparse(self, rev):
         """
         Convert a revision (tag, branch, commit) to a regular reference.
-        
+
         :param rev: Reference
         :type rev: Reference
         """
         pass
-    
+
     @abstractmethod
     def iterate_over(self, ref):
         """starting from the ref, iterate references backwards (from newest to
         oldest).
-        
+
         :param ref: the starting point
         :type ref: Reference
         """
         pass
-    
+
     @abstractmethod
     def list_files(self, rev):
         """For a given revision, list files (not only changed ones).
-        
+
         :param rev: the revision
         :type rev: Reference
         """
         pass
-    
+
     @abstractmethod
     def gc(self):
         """Run the garbage collector"""
         pass
-    
+
     @abstractmethod
     def get_parents(self, ref):
         """Retrieve parents for a given ref.
-        
+
         This method is not a part of a Reference object as the approach changes
         depending on the Git method used (lazy resolution).
-        
+
         :param ref: the revision
         :type ref: Reference
         """
         pass
-    
+
     def _set_or_head(self, rev):
         """Return a valid revision to be used
-        
+
         If rev is not set, return the default HEAD repo.
-        
+
         :param rev: the revision to use or replace if not set
         :type rev: Reference"""
         return rev if rev else self._head
 
 
 class GitByAPI(GitByGeneric):
     """
     Manage repository through a third-party Python module.
-    
+
     Currently, this work is based on pygit2.
     """
+
     def __init__(self, prefix=None):
         super().__init__(prefix)
         self._repo = None
 
     def open(self, bare=True):
-        assert(not os.path.isfile(self._path))
+        assert (not os.path.isfile(self._path))
         if not os.path.isdir(self._path) or len(os.listdir(self._path)) == 0:
             if not self._is_locked():
                 self._repo = pygit2.init_repository(
-                            self._path,
-                            flags=(pygit2.GIT_REPOSITORY_INIT_MKPATH |
-                                pygit2.GIT_REPOSITORY_INIT_NO_REINIT),
-                            mode=pygit2.GIT_REPOSITORY_INIT_SHARED_GROUP,
-                            bare=bare
-                        )
+                    self._path,
+                    flags=(pygit2.GIT_REPOSITORY_INIT_MKPATH |
+                           pygit2.GIT_REPOSITORY_INIT_NO_REINIT),
+                    mode=pygit2.GIT_REPOSITORY_INIT_SHARED_GROUP,
+                    bare=bare
+                )
                 self._lock()
         else:
             rep = pygit2.discover_repository(self._path)
             if rep:
                 self._repo = pygit2.Repository(rep)
                 self._lock()
-        
+
     def get_branch_from_str(self, name):
         for b in self.branches:
             if name == b.name:
                 return b
         return None
 
     def is_open(self):
         return self._repo is not None
 
     def close(self):
         self._unlock()
 
     def __obj_to_commit(self, obj):
-        assert(isinstance(obj, pygit2.Commit))
+        assert (isinstance(obj, pygit2.Commit))
         return Commit(
             repo=self._repo,
             obj=obj,
             metadata={
                 'obj': obj,
                 'date': datetime.fromtimestamp(obj.author.time),
                 'author': obj.author.name,
@@ -394,130 +415,131 @@
                 'message': obj.message,
                 'parents': obj.parents
             }
         )
 
     @property
     def branches(self):
-        assert(self._repo)
+        assert (self._repo)
         return [Branch(self, e) for e in self._repo.branches.local]
-    
+
     def new_branch(self, name, cid=None):
         if not cid:
             cid = self.revparse(Branch(self, name='master')).cid
-        
-        assert(name not in self._repo.branches.local)
+
+        assert (name not in self._repo.branches.local)
         self._repo.branches.local.create(name, cid)
         return Branch(self, name=name)
-        
+
     def set_branch(self, branch, commit):
-        assert(isinstance(commit, Reference))
-        assert(isinstance(branch, Branch))
-        
+        assert (isinstance(commit, Reference))
+        assert (isinstance(branch, Branch))
+
         pygit_obj = self.revparse(commit).cid.oid
         ref = "refs/heads/{}".format(branch.name)
         if ref in self._repo.references:
             self._repo.references.delete(branch.name)
-        self._repo.references.create("refs/heads/{}".format(branch.name), pygit_obj)
-            
+        self._repo.references.create(
+            "refs/heads/{}".format(branch.name), pygit_obj)
+
     def revparse(self, ref):
-        assert(self._repo)
-        assert(isinstance(ref, Reference))
-        
+        assert (self._repo)
+        assert (isinstance(ref, Reference))
+
         if isinstance(ref, Commit):
             return ref
-        
+
         o = self._repo.revparse_single(ref.name)
         return self.__obj_to_commit(o)
 
     def get_tree(self, rev=None, prefix=""):
-        assert(not rev or isinstance(rev, Reference))
+        assert (not rev or isinstance(rev, Reference))
         rev = self._set_or_head(rev)
-        
+
         tree = None
         if isinstance(rev, Branch):
             tree = self._repo.revparse_single(rev.name).tree
         elif isinstance(rev, Commit):
             tree = rev.cid.tree
-        
+
         if prefix:
             tid = self._get_tree(prefix.split("/"), tree)
         else:
             tid = tree
-        
+
         if isinstance(tid, pygit2.Blob):
             return Blob(self, tid, prefix, tid.data)
         else:
             return Tree(self, tid, prefix)
-        
+
     def _get_tree(self, chain, tree=None):
         if len(chain) <= 0:
             return tree
         else:
             subtree = None
             for i in tree:
                 if chain[0] == i.name:
                     subtree = i
                     break
             return self._get_tree(chain[1:], subtree)
 
     def iterate_over(self, rev=None):
-        assert(not rev or isinstance(rev, Reference))
+        assert (not rev or isinstance(rev, Reference))
         rev = self._set_or_head(rev)
         rev = self.revparse(rev)
-        assert(isinstance(rev, Commit))
+        assert (isinstance(rev, Commit))
         pygit_obj = rev.cid
-        
+
         for o in self._repo.walk(pygit_obj.oid, pygit2.GIT_SORT_REVERSE):
             yield self.__obj_to_commit(o)
 
     def list_files(self, rev=None, prefix=""):
-        assert(not rev or isinstance(rev, Commit))
+        assert (not rev or isinstance(rev, Commit))
         rev = self._set_or_head(rev)
         tree = rev.cid.tree
         return [e.old_file.path for e in tree.diff_to_tree().deltas if e.old_file.path.startswith(prefix)]
-    
+
     def diff_tree(self, prefix=None, src_rev=None, dst_rev=None):
         src_rev = self._set_or_head(src_rev)
         src_rev = self.revparse(src_rev)
-        
-        assert(isinstance(src_rev, pygit2.Object))
+
+        assert (isinstance(src_rev, pygit2.Object))
         if dst_rev:
             dst_rev = self._set_or_head(dst_rev)
             dst_rev = self.revparse(dst_rev)
-            assert(isinstance(dst_rev, pygit2.Object))
-            
+            assert (isinstance(dst_rev, pygit2.Object))
+
             diff = src_rev.diff_to_tree(dst_rev)
         else:
             diff = src_rev.diff_to_tree()
-    
+
     def list_commits(self, rev=None, since=None, until=None):
         res = []
-        assert(not rev or isinstance(rev, Reference))
-        
+        assert (not rev or isinstance(rev, Reference))
+
         if since is None:
             since = datetime.now().timestamp()
-            
+
         if until is None:
             until = 0
-            
+
         for c in self.iterate_over(rev):
             pygit_obj = c.cid
             if pygit_obj.commit_time <= since and pygit_obj.commit_time >= until:
                 res.append(self.__obj_to_commit(pygit_obj))
         return res
-        
+
     def commit(self, tree, msg="No data", timestamp=None, parent=None, orphan=False):
-        assert(self._repo)
-        assert(isinstance(tree, Tree))
-        assert(not parent or isinstance(parent, Reference))
-        
+        assert (self._repo)
+        assert (isinstance(tree, Tree))
+        assert (not parent or isinstance(parent, Reference))
+
         if not timestamp:
             timestamp = int(datetime.now().timestamp())
-        
+
         author = pygit2.Signature(name=self._authname,
                                   email=self._authmail,
                                   time=timestamp)
         committer = pygit2.Signature(name=self._commname,
                                      email=self._commname,
                                      time=timestamp)
 
@@ -526,38 +548,41 @@
         if not orphan:
             parent = self._set_or_head(parent)
             if isinstance(parent, Branch):
                 update_ref = "refs/heads/{}".format(parent.name)
                 parents = [self.revparse(parent).cid.oid]
             elif isinstance(parent, Commit):
                 update_ref = None
-                parents  = [parent.cid.oid]
+                parents = [parent.cid.oid]
             else:
-                raise Exception()
-        
+                raise GitException.BadEntryError(
+                    reason="Parent is unknown",
+                    dbg_info={"ref": parent}
+                )
+
         coid = self._repo.create_commit(update_ref,
-                        author,
-                        committer,
-                        msg,
-                        tree.hdl.write(),
-                        parents
-                    )
+                                        author,
+                                        committer,
+                                        msg,
+                                        tree.hdl.write(),
+                                        parents
+                                        )
         ci = self._repo.get(coid)
         return self.__obj_to_commit(ci)
-    
+
     def insert_tree(self, prefix, data, root=None):
         if not root:
             root = Tree.as_root(self._repo, self._repo.TreeBuilder())
-        
+
         pygit_obj = root.hdl
         self.__insert_path(pygit_obj, prefix.split('/'), data)
-        #root.tid = pygit_obj.
-        
+        # root.tid = pygit_obj.
+
         return root
-                    
+
     def __insert_path(self, treebuild, path, data: any):
         """Associate an object to a given tag (=path).
 
         The result is stored into the parent subtree (treebuild). The path is an
         array of subrefixes, identifying the subtree where the object will
         be stored under the bank. This function associates the path & the object
         together, write the result in the parent and returns its Oid.
@@ -590,150 +615,152 @@
         # otherwise, determine where the current subdir is going
         subtree_name = path[0]
         tree = repo.get(treebuild.write())
 
         try:
             # check if the subdir already exist in this bank subtree
             entry = tree[subtree_name]
-            assert(entry.filemode == pygit2.GIT_FILEMODE_TREE)
+            assert (entry.filemode == pygit2.GIT_FILEMODE_TREE)
             subtree = repo.get(entry.hex)
             # YES it is found -> reuse this subtree
             sub_treebuild = repo.TreeBuilder(subtree)
         except KeyError:
             # NOPE: first time adding a resource to this subtree
             # create a new one
             sub_treebuild = repo.TreeBuilder()
 
         # recursive call, as we didn't reach the subtree bottom
         subtree_oid = self.__insert_path(sub_treebuild, path[1:], data)
         # Pygit2 insert, to build the actual intemediate node
         treebuild.insert(subtree_name, subtree_oid, pygit2.GIT_FILEMODE_TREE)
         return treebuild.write()
-    
+
     def gc(self):
         import sh
         hdl = sh.git.bake(_cwd=self._path)
         hdl.gc()
-        
+
     def get_parents(self, ref):
-        assert(isinstance(ref, Reference))
-        
+        assert (isinstance(ref, Reference))
+
         ref = self._set_or_head(ref)
         ref = self.revparse(ref)
-        
+
         return [self.__obj_to_commit(p) for p in ref.meta['parents']]
 
+
 class GitByCLI(GitByGeneric):
     """
     Git endpoint ot manipulate a repository through basic CLI.
-    
+
     Currently relying on the `sh` module.
     """
+
     def __init__(self, prefix=""):
         super().__init__(prefix)
         self._git = None
-        
+
     @property
     def branches(self):
         array = self._git('for-each-ref', 'refs/heads/').strip().split("\n")
         return [Branch(self, elt.split('\t')[-1].replace("refs/heads/", "")) for elt in array]
-    
+
     def iterate_over(self, ref):
         res = []
-        assert(isinstance(ref, Reference))
+        assert (isinstance(ref, Reference))
         for elt in self._git('rev-list', '--reverse', ref).strip().split("\n"):
             yield Commit(
                 repo=self,
                 obj=elt
             )
-        
+
     def open(self, bare=True):
         if not os.path.isdir(self._path):
             os.makedirs(self._path)
-        
+
         self._lock()
         self._git = sh.git.bake(_cwd=self._path)
-        
+
         if not os.path.isfile(os.path.join(self._path, "HEAD")):
             self._git.init("--bare")
-        
+
     def is_open(self):
         return self._is_locked()
 
     def close(self):
         self._git = None
         self._unlock()
-        
+
     def revparse(self, rev):
-        assert(isinstance(rev, Reference))
+        assert (isinstance(rev, Reference))
         if isinstance(rev, Commit):
             return rev
         return Commit(repo=self, obj=self._git("rev-parse", rev.name).strip())
-    
+
     def _create_blob(self, name, data):
         oid = ""
         oid = self._git('hash-object', "--stdin", "-w", _in=str(data)).strip()
         return (oid, "100644 blob {}\t{}".format(oid, name))
-    
+
     def __valid_object(self, hash):
         try:
             self._git("cat-file", "-e", hash)
         except:
             return False
         return True
-    
+
     def _insert_path(self, treebuild, path, data):
-        assert(isinstance(treebuild, Tree))
-        
+        assert (isinstance(treebuild, Tree))
+
         if len(path) == 1:
             data_hash = generate_data_hash(str(data))
             if not self.__valid_object(data_hash):
                 check = self._create_blob(path, data)
-                assert(check == data_hash)
+                assert (check == data_hash)
             treebuild.children.append(data_hash)
             return data_hash
         else:
             cur = path[0]
-            
+
     def _create_tree(self, name, children):
         array = []
         for k, v in children.items():
             if isinstance(v, dict):
                 array.append(self._create_tree(k, v)[1])
             else:
                 array.append(self._create_blob(k, v)[1])
 
         oid = self._git.mktree(_in="\n".join(array)).strip()
         return (oid, "040000 tree {}\t{}".format(oid, name))
-        
+
     def insert_tree(self, prefix, data, root=None):
         if not root:
             root = Tree.as_root(self, None)
-        
+
         raise NotImplementedError()
         self._insert_path(root, prefix.split("/"), data)
-        
+
         return root
-    
+
     def get_tree(self, rev=None, prefix=""):
-        oid=None
-        assert(not rev or isinstance(rev, Reference))
+        oid = None
+        assert (not rev or isinstance(rev, Reference))
         rev = self._set_or_head(rev)
-        
+
         try:
             self._git("rev-parse", "{}:{}".format(rev, prefix), _out=oid)
         except sh.ErrorReturnCode:
             oid = None
-        
+
         if self._git('cat-file', '-t', oid) == "blob":
             data = self._git('cat-file', "-p", oid).strip()
             return Blob(self, oid, prefix, data)
         else:
             return Tree(self, oid, prefix)
-    
+
     def __obj_to_commit(self, cid):
         s = self.__commit_info_getter("%at:%an:%ae", "-1", cid).split(':')
         msg = self.__commit_info_getter("%B", "-1", cid)
         return Commit(
             repo=self,
             obj=cid,
             metadata={
@@ -742,92 +769,92 @@
                 'author': s[1],
                 'authmail': s[2],
                 'message': msg
             }
         )
 
     def commit(self, tree, msg="VOID", timestamp=None, parent=None, orphan=False):
-        assert(not parent or isinstance(parent, Reference))
-        assert(isinstance(tree, Tree))
+        assert (not parent or isinstance(parent, Reference))
+        assert (isinstance(tree, Tree))
         # if this commit should have parents
         if not orphan:
-            
+
             parent = self._set_or_head(parent)
             parents = self.revparse(parent)
-            commit_id = self._git("commit-tree", tree, 
-                "-m '{}'".format(msg),
-                "-p {}".format(parents.cid)
-            ).strip()
+            commit_id = self._git("commit-tree", tree,
+                                  "-m '{}'".format(msg),
+                                  "-p {}".format(parents.cid)
+                                  ).strip()
             if isinstance(parent, Branch):
-                self._git.push(".", "{}:refs/heads/{}".format(commit_id, parent.name))
+                self._git.push(
+                    ".", "{}:refs/heads/{}".format(commit_id, parent.name))
         # The commit will have no parent
-        else:    
-            commit_id = self._git("commit-tree", tree, 
-                "-m '{}'".format(msg),
-            ).strip()
-        
+        else:
+            commit_id = self._git("commit-tree", tree,
+                                  "-m '{}'".format(msg),
+                                  ).strip()
+
         return self.__obj_to_commit(commit_id)
-        
+
     def get_branch_from_str(self, name):
         for b in self.branches:
             if name == b.name:
                 return b
         return None
-    
+
     def new_branch(self, name, cid=None):
         if not cid:
             cid = self.revparse(Branch(self, name='master')).cid
-        
+
         self._git.push('.', '{}:refs/heads/{}'.format(cid, name))
         return Branch(self, name=name)
-            
+
     def set_branch(self, branch, commit):
-        self._git.push("-f", ".", "{}:refs/heads/{}".format(commit.cid, branch.name))
+        self._git.push(
+            "-f", ".", "{}:refs/heads/{}".format(commit.cid, branch.name))
 
     def list_files(self, prefix):
         if not prefix:
             prefix = ""
         return [self._git('ls-files', prefix).strip().split("\n")]
 
     def list_commits(self, rev=None, since="", until=""):
         rev = self._set_or_head(rev)
         if since:
             since = "--since={}".format(since)
         if until:
             until = "--until={}".format(until)
-        
+
         return [self.__commit_info_getter("%H", rev, since, until)]
 
     def __commit_info_getter(self, pattern, *args):
         return self._git('--no-pager', 'log', "--format={}".format(pattern), *args).strip()
-    
+
     def diff_tree(self, prefix=None, src_rev=None, dst_rev=None):
-        
+
         if not dst_rev:
             return None
-        
+
         src_rev = self._set_or_head(src_rev)
         src_rev = self.revparse(src_rev)
-        
+
         return self._git('diff-tree', src_rev, dst_rev).strip()
-    
+
     def gc(self):
         self._git.gc('--aggressive')
-        
+
     def get_parents(self, ref):
         ref = self._set_or_head(ref)
         ref = self.revparse(ref)
-        
+
         parents = []
         for elt in self._git('cat-file', '-p', ref).strip().split('\n'):
             parents.append(self.__obj_to_commit(elt))
         return parents
-        
-        
- 
+
 
 def request_git_attr(k) -> str:
     """Get a git configuration.
 
     :param k: parameter to get
     :type k: str
     :return: a git configuration
@@ -858,14 +885,15 @@
     """
     c = hashlib.md5()
     if not isinstance(data, bytes):
         data = str(data).encode()
     c.update(data)
     return c.hexdigest()
 
+
 def get_current_username() -> str:
     """Get the git username.
 
     :return: git username
     :rtype: str
     """
     try:
@@ -875,26 +903,25 @@
     except Exception as e:
         pass
     finally:
         if u is None:
             u = "anonymous"
 
     return u
-        
 
 
 def get_current_usermail():
     """Get the git user mail.
 
     :return: git user mail
     :rtype: str
     """
     try:
         m = request_git_attr('user.email')
-        #if m is None:
+        # if m is None:
         #    m = "{}@{}".format(get_current_username(), socket.getfqdn())
     except Exception as e:
         pass
     finally:
         if m is None:
             m = "anonymous@notset"
```

### Comparing `pcvs-0.6.0/pcvs/helpers/log.py` & `pcvs-0.7.0/pcvs/testing/test.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,638 +1,679 @@
-import functools
+import base64
+import json
+import zlib
 import os
-import pprint
+import re
+import shlex
 import sys
-import textwrap
-import traceback
+import hashlib
+from enum import IntEnum
 
-import click
+from pcvs import io
+from pcvs.helpers.criterion import Combination
+from pcvs.helpers.system import MetaConfig, ValidationScheme
+from pcvs.helpers.utils import Program
+from pcvs.plugins import Plugin
+
+
+class Test:
+    """Smallest component of a validation process.
+
+    A test is basically a shell command to run. Depending on its post-execution
+    status, a success or a failure can be determined. To handle such component
+    in a convenient way, more information can be attached to the command like a
+    name, the elapsed time, the output, etc.
+
+    In order to make test content flexible, there is no fixed list of
+    attributes. A Test() constructor is initialized via (*args, **kwargs), to
+    populate a dict `_array`.
 
-from pcvs.helpers import exceptions
-from pcvs.helpers.exceptions import CommonException
+    :cvar int Timeout_RC: special constant given to jobs exceeding their time limit.
+    :cvar str NOSTART_STR: constant, setting default output when job cannot be run.
+    """
+    Timeout_RC = 127
+    SCHED_MAX_ATTEMPTS = 50
+    res_scheme = ValidationScheme("test-result")
+
+    NOSTART_STR = b"This test cannot be started."
+    MAXATTEMPTS_STR = b"This test has failed to be scheduled too many times. Discarded."
+
+    class State(IntEnum):
+        """Provide Status management, specifically for tests/jobs.
+
+        Defined as an enum, it represents different states a job can take during
+        its lifetime. As tests are then serialized into a JSON file, there is
+        no need for construction/representation (as done for Session states).
+
+        :var int WAITING: Job is currently waiting to be scheduled
+        :var int IN_PROGRESS: A running Set() handle the job, and is scheduled
+            for run.
+        :var int SUCCEED: Job successfully run and passes all checks (rc,
+            matchers...)
+        :var int FAILED: Job didn't suceed, at least one condition failed.
+        :var int ERR_DEP: Special cases to manage jobs descheduled because at
+            least one of its dependencies have failed to complete.
+        :var int ERR_OTHER: Any other uncaught situation.
+        """
+        WAITING = 0
+        IN_PROGRESS = 1
+        SUCCESS = 2
+        FAILURE = 3
+        ERR_DEP = 4
+        ERR_OTHER = 5
+        EXECUTED = 6
 
+        def __str__(self):
+            """Stringify to return the label.
 
-def pretty_print_exception(e: exceptions.GenericError):
-    """Display exceptions in a fancy way.
+            :return: the enum name
+            :rtype: str
+            """
+            return self.name
 
-    :param e: the execption to print
-    :type e: exceptions.GenericError.
-    """
-    global manager
-    if isinstance(e, exceptions.GenericError):
-        manager.err([e.err, e.help])
-        manager.info("Extra infos:\n{}".format(e.dbg_str))
-    else:
-        manager.err(str(e))
+        def __repr__(self):
+            """Enum representation a tuple (name, value).
 
+            :return: a tuple mapping the enum.
+            :rtype: tuple
+            """
+            return "({}, {})".format(self.name, self.value)
 
-class IOManager:
-    """
-    Manager for Input/Output streams.
+    def __init__(self, **kwargs):
+        """constructor method.
 
-    Contains methods for logging and printing in PCVS. IOManager handles
-    multiple outputs (file + standard output), logging levels (warning, error,
-    info, etc) and pretty banners. Colors are handled by click and color tags
-    are written in files (use less -r).
-
-    :param special_chars: dictionary for fancy bullet characters
-    :type special_chars: dict
-    :param verb_levels: verbosity level (normal, info, debug)
-    :type verb_levels: list
-    :param color_list: list of colors used by PCVS
-    :type color_list: list
-    """
-    special_chars = {
-        "ascii": {
-            'copy': '(c)',
-            'item': '*',
-            'sec': '#',
-            'hdr': '=',
-            'star': '*',
-            'fail': "X",
-            'succ': "V",
-            'none': "-",
-            'git': '(git)',
-            'time': '(time)',
-            'full_pg': '#',
-            'empty_pg': '-',
-            'sep_v': " | ",
-            'sep_h': "-"
-        },
-        "unicode": {
-            'copy': '\u00A9',
-            'item': '\u27E2',
-            'sec': '\u2756',
-            'hdr': '\u23BC',
-            'star': '\u2605',
-            'fail': '\u2718',
-            'succ': '\u2714',
-            "none": '\u2205',
-            'git': '\u237F',
-            'time': '\U0000231A',
-            'full_pg': click.style("\u25CF", bold=True, fg="cyan"),
-            'empty_pg': click.style("\u25CB", bold=True, fg="bright_black"),
-            'sep_v': " \u237F ",
-            'sep_h': "\u23BC"
+        :param kwargs: flexible list of arguments to initialize a Test with.
+        :type kwargs: dict
+        """
+        self._rc = 0
+        self._comb = kwargs.get('comb')
+        self._cwd = kwargs.get('wd')
+        self._exectime = 0.0
+        self._output = b""
+        self._state = Test.State.WAITING
+        self._dim = kwargs.get('dim', 1)
+        self._testenv = kwargs.get('environment')
+        self._id = {
+            'te_name': kwargs.get('te_name', 'noname'),
+            'label': kwargs.get('label', 'nolabel'),
+            'subtree': kwargs.get('subtree', ''),
+            'comb': self._comb.translate_to_dict() if self._comb else {},
         }
-    }
+        comb_str = self._comb.translate_to_str() if self._comb else None
 
-    verb_levels = [(0, "normal"), (1, "info"), (2, "debug")]
+        self._id['fq_name'] = Test.compute_fq_name(
+            self._id['label'],
+            self._id['subtree'],
+            self._id['te_name'],
+            comb_str,
+            suffix=kwargs.get('user_suffix'))
+        
+        # only positive ids
+        self._id['jid'] = self.get_jid_from_name(self.name)
+        
+        self._execmd = kwargs.get('command', '')
+
+        self._data = {
+            'metrics': kwargs.get('metrics', {}),
+            'tags': kwargs.get('tags', []),
+            'artifacts': kwargs.get('artifacts', {}),
+        }
+
+        self._validation = {
+            'matchers': kwargs.get('matchers'),
+            'analysis': kwargs.get('analysis'),
+            'script': kwargs.get('valscript'),
+            'expect_rc': kwargs.get('rc', 0),
+            'time': kwargs.get('time', -1),
+            'delta': kwargs.get('delta', 0),
+        }
+        
+        self._timeout = kwargs.get('kill_after', None)
 
-    color_list = [
-        "black",
-        "red",
-        "green",
-        "yellow",
-        "blue",
-        "magenta",
-        "cyan",
-        "white",
-        "bright_black",
-        "bright_red",
-        "bright_green",
-        "bright_yellow",
-        "bright_blue",
-        "bright_magenta",
-        "bright_cyan",
-        "bright_white",
-    ]
+        self._mod_deps = kwargs.get("mod_deps", [])
+        self._depnames = kwargs.get('job_deps', [])
+        self._deps = []
+        self._invocation_cmd = self._execmd
+        self._sched_cnt = 0
+        self._output_info = {
+            'file': None,
+            'offset': -1,
+            'length': 0
+        }
 
     @property
-    def verbose(self):
-        """getter for verbosity level
+    def jid(self) -> str:
+        """Getter for unique Job ID within a run.
 
-        :return: verbosity level (0, 1, 2)
-        :rtype: int
+        This attribute is generally set by the manager once job is uploaded
+        to the dataset.
+        :return: the job id
+        :rtype: an positive integer of -1 if not set
         """
-        return self._verbose
+        return self._id['jid']
 
     @property
-    def tty(self):
-        """getter for tty information
+    def basename(self) -> str:
+        return Test.compute_fq_name(self._id['label'], self._id['subtree'], self._id['te_name'])
+    @property
+    def tags(self):
+        """Getter for the full list of tags.
 
-        :return: False if tty not used, 1 if tty used
-        :rtype: bool
+        :return: the list of of tags
+        :rtype: list
         """
-        return self._tty
+        return self._data['tags']
 
-    def set_tty(self, enable):
-        """[summary]
+    @property
+    def label(self):
+        """Getter to the test label.
 
-        :param enable: [description]
-        :type enable: [type]
+        :return: the label
+        :rtype: str
         """
-        self._tty = enable
+        return self._id["label"]
+
+    @property
+    def name(self):
+        """Getter for fully-qualified job name.
 
-    def enable_tty(self):
-        """enables tty
+        :return: test name.
+        :rtype: str
         """
-        self.set_tty(enable=True)
+        return self._id['fq_name']
+
+    @property
+    def subtree(self):
+        """Getter to the test subtree.
 
-    def disable_tty(self):
-        """disables tty
+        :return: test subtree.
+        :rtype: str.
         """
-        self.set_tty(enable=False)
+        return self._id["subtree"]
 
     @property
-    def log_filename(self):
-        """getter for logfile path
+    def te_name(self):
+        """Getter to the test TE name.
 
-        :return: logfile path
-        :rtype: str
+        :return: test TE name.
+        :rtype: str.
         """
-        return os.path.abspath(self._logfile.name) if self._logfile else None
 
-    def set_logfile(self, enable, logfile=None):
-        """setter for logfile path
+        return self._id["te_name"]
+
+    @property
+    def combination(self):
+        """Getter to the test combination dict.
 
-        :param logfile: logfile name, defaults to None
-        :type logfile: str, optional
+        :return: test comb dict.
+        :rtype: dict
         """
 
-        if logfile is not None:
-            if not os.access(os.path.dirname(logfile), os.W_OK):
-                raise CommonException.IOError(
-                    "{} is not writable !".format(logfile))
-
-            if os.path.abspath(logfile) != self.log_filename:
-                self._logfile = open(os.path.abspath(logfile), 'w+')
-            self._logenabled = enable
-
-    def __init__(self, verbose=0, enable_unicode=True, length=80, logfile=None, tty=True):
-        """constructor for IOManager object
-
-        :param verbose: verbosity level (0 : low, 1: info, 2: debug), defaults
-            to 0
-        :type verbose: int, optional
-        :param enable_unicode: True if unicode alphabet usage is authorised,
-            defaults to True
-        :type enable_unicode: bool, optional
-        :param length: length of terminal (character number), defaults to 80
-        :type length: int, optional
-        :param logfile: logfile name, file logging disabled if logfile=None,
-            defaults to None
-        :type logfile: str, optional
-        :param tty: True if logs must be in stdout, defaults to True
-        :type tty: bool, optional
-        :raises CommonException.AlreadyExistError: only one IOManager can
-            exist in a session
-        """
-        self._linelength = 93
-        self._wrapper = None
-        self._tty = tty
-        self._logfile = None
-        self._verbose = verbose
-        self._unicode = enable_unicode
-        self._logbuffer = ""
-        self._logenabled = False
-
-        self.enable_unicode(self._unicode)
-
-        if length is not None:
-            self._linelength = length if length > 0 else click.get_terminal_size()[
-                0]
-        self._wrapper = textwrap.TextWrapper(width=self._linelength)
-
-        if logfile is not None:
-            logfile = os.path.abspath(logfile)
-            if os.path.isfile(logfile):
-                raise CommonException.AlreadyExistError(logfile)
-
-            self.set_logfile(True, logfile)
-
-    def __del__(self):
-        """desctuctor for IOManager (closes streams)
-        """
-
-        if self._logfile and self._logfile.name:
-            self._logfile.close()
-
-    def __print_rawline(self, msg, err=False):
-        """print a line as text
-
-        :param msg: message to be printed
-        :type msg: str
-        :param err: True if the message is an error message, defaults to False
-        :type err: bool, optional
-        """
-        if self._tty:
-            click.echo(msg, err=err)
-
-        content = '{}{}'.format(msg, '\n' if msg[-1] != "\n" else "")
-        if self._logenabled and self._logfile:
-            self._logfile.write(self._logbuffer)
-            self._logfile.write(content)
-            self._logfile.flush()
-            self._logbuffer = ""
-        else:
-            self._logbuffer += content
+        return self._comb
+
+    @property
+    def command(self):
+        """Getter for the full command.
 
-    def has_verb_level(self, match):
-        """ returns true if the verbosity level is activated.
+        This is a real command, executed in a shell, coming from user's
+        specificaition. It should not be confused with `invocation_command`.
 
-        :param match: verbosity level to check
-        :type match: str or int
-        :return: True if "match" verbosity level is supposed to be printed by
-            the IOManager
-        :rtype: bool
+        :return: unescaped command line
+        :rtype: str
         """
-        req_idx = 0
-        for e in self.verb_levels:
-            if match.lower() == e[1].lower():
-                req_idx = e[0]
-                break
-        return req_idx <= self._verbose
-
-    def get_verbosity_str(self):
-        """[summary]
-
-        :return: [description]
-        :rtype: [type]
-        """
-        for e in self.verb_levels:
-            if self._verbose == e[0]:
-                return e[1]
-        return self.verb_levels[0][1]
-
-    def print(self, *msg):
-        """prints a raw line. Takes multiple arguments.
-        """
-        for i in msg:
-            self.__print_rawline(i)
-
-    def write(self, txt):
-        """print a string.
-
-        :param txt: message to be printed
-        :type txt: str
-        """
-        self.__print_rawline(txt)
-
-    def capture_exception(self, e_type, user_func=None):
-        """wraps functions to capture unhandled exceptions for high-level
-            function not to crash.
-            :param *e_type: errors to be caught
-        """
-        def inner_function(func):
-            """wrapper for inner function using try/except to avoid crashing
-
-            :param func: function to wrap
-            :type func: function
-            :raises e: exceptions to catch
-            :return: wrapper
-            :rtype: function
-            """
-            @functools.wraps(func)
-            def wrapper(*args, **kwargs):
-                """functools wrapping function
-
-                :raises e: exception to catch
-                :return: result of wrapped function
-                :rtype: any
-                """
-                try:
-                    return func(*args, **kwargs)
-                except e_type as e:
-                    #raise e
-                    if user_func is None:
-                        pretty_print_exception(e)
-                        manager.debug(
-                            traceback.format_exception(*sys.exc_info()))
-                        sys.exit(1)
-                    else:
-                        user_func(e)
-            return wrapper
-        return inner_function
-
-    def enable_unicode(self, e=True):
-        """enables/disables unicode alphabet usage
-
-        :param e: True to enable unicode usage, defaults to True
-        :type e: bool, optional
+        return self._execmd
+
+    @property
+    def invocation_command(self):
+        """Getter for the list_of_test.sh invocation leading to run the job.
+
+        This command is under the form: `sh /path/list_of_tests.sh <test-name>`
+
+        :return: wrapper command line
+        :rtype: str
         """
-        self.glyphs = self.special_chars["unicode"] if e is True else self.special_chars["ascii"]
+        return self._invocation_cmd
 
-    def avail_chars(self):
-        """lists allowed bullet characters
+    @property
+    def job_deps(self):
+        """"Getter to the dependency list for this job.
 
-        :return: a list of characters
+        The dependency struct is an array, where for each name (=key), the
+        associated Job is stored (value)
+        :return: the list of object-converted deps
         :rtype: list
         """
-        return self.glyphs.keys()
+        return self._deps
 
-    def utf(self, k):
-        """returns the corresponding character to a bullet character
+    @property
+    def job_depnames(self):
+        """Getter to the list of deps, as an array of names.
 
-        :param k: character used as bullet character
-        :type k: char
-        :return: fancy bullet character
-        :rtype: char
+        This array is emptied when all deps are converted to objects.
+
+        :return: the array of dep names
+        :rtype: list
         """
-        assert(k in self.glyphs.keys())
-        return self.glyphs[k]
+        return self._depnames
+
+    @property
+    def mod_deps(self):
+        """Getter to the list of pack-manager rules defined for this job.
 
-    def style(self, *args, **kwargs):
-        """returns a string style using click
+        There is no need for a ``_depnames`` version as these deps are provided
+        as PManager objects directly.
 
-        :return: a string style
-        :rtype: click.style
+        :return: the list of package-manager based deps.
+        :rtype: list
         """
-        return click.style(*args, **kwargs)
+        return self._mod_deps
+    
+    @classmethod
+    def get_jid_from_name(self, name):
+        if not isinstance(name, bytes):
+            name = str(name).encode('utf-8')
+            
+        return hashlib.md5(name).hexdigest()
+    
+    def get_dep_graph(self):
+        res = {}
+        for d in self._deps:
+            res[d.name] = d.get_dep_graph()
+        return res
 
-    def print_header(self, s, out=True):
-        """prints a header
+    def resolve_a_dep(self, name, obj):
+        """Resolve the dep object for a given dep name.
 
-        :param s: header content
-        :type s: str
-        :param out: True if the header has to be logged, False if it has to be
-            returned, defaults to True
-        :type out: bool, optional
-        :return: header string if out=False, Nothing otherwise
-        :rtype: str
+        :param name: the dep name to resolve, should be a valid dep.
+        :type name: str
+        :param obj: the dep object, should be a Test()
+        :type obj: :class:`Test`
         """
-        hdr_char = self.utf('hdr')
-        str_len = self._linelength - (len(s) + 2)  # surrounding spaces
-        # nb chars before the title (centering)
-        begin = hdr_char * int(str_len / 2)
-        # nb chars after the title (centering)
-        end = begin + (hdr_char * (str_len % 2 != 0))
-
-        # formatting & colouring
-        final_string = click.style("\n{} {} {}".format(
-            begin, s.upper(), end), fg="green")
-        if out:
-            self.__print_rawline(final_string)
-        else:
-            return final_string
+        if name not in self._depnames:
+            return
 
-    def print_section(self, s, out=True):
-        """prints a section
+        if obj not in self._deps:
+            self._deps.append(obj)
 
-        :param s: content of the section
-        :type s: str
-        :param out: True if the section has to be logged, False if it has to be
-            returned, defaults to True
-        :type out: bool, optional
-        :return: section string if out=False, Nothing otherwise
-        :rtype: str
+    def has_completed_deps(self):
+        """Check if the test can be scheduled.
+
+        It ensures it hasn't been executed yet (or currently running) and all
+        its deps are resolved and successfully run.
+
+        :return: True if the job can be scheduled
+        :rtype: bool
         """
-        f = "{} {}".format(self.utf('sec'), s)
-        self._wrapper.subsequent_indent = "  "
-        s = self._wrapper.fill(click.style(f, fg='yellow'))
-        if out:
-            self.__print_rawline(s)
-        else:
-            return s
+        return len([d for d in self._deps if not d.been_executed()]) == 0
 
-    def print_item(self, s, depth=1, out=True, with_bullet=True):
-        """prints an item
+    def has_failed_dep(self):
+        """Check if at least one dep is blocking this job from ever be
+        scheduled.
 
-        :param s: item content
-        :type s: str
-        :param depth: number of tabulations used for indentation, defaults to 1
-        :type depth: int, optional
-        :param out: True if the item has to be logged, False if it has to be
-            returned, defaults to True
-        :type out: bool, optional
-        :param with_bullet: True if the item should have a bullet, defaults to True
-        :type with_bullet: bool, optional
-        :return: item string if out=False, Nothing otherwise
-        :rtype: str
+        :return: True if at least one dep is shown a `Test.State.FAILURE` state.
+        :rtype: bool
         """
-        indent = ("   " * depth)
-        bullet = indent + \
-            "{} ".format(self.utf('item')) if with_bullet is True else ""
-        content = "{}".format(s)
-
-        self._wrapper.subsequent_indent = indent + "  "
-        s = self._wrapper.fill(click.style(
-            bullet, fg="red") + click.style(content, fg="reset"))
-        if out:
-            self.__print_rawline(s)
-        else:
-            return s
+        return len([d for d in self._deps if d.state in [Test.State.ERR_DEP, Test.State.ERR_OTHER, Test.State.FAILURE]]) > 0
 
-    def print_job(self, label, time, name, colorname="red", icon=None):
-        """prints a job description
+    def first_incomplete_dep(self):
+        """Retrive the first ready-for-schedule dep.
 
-        :param label: job label
-        :type label: str
-        :param time: time elapsed since the job launch
-        :type time: float
-        :param name: name of the job
-        :type name: str
-        :param colorname: color of the job log, defaults to "red"
-        :type colorname: str, optional
-        :param icon: bullet, defaults to None
-        :type icon: str, optional
-        """
-        if icon is not None:
-            icon = self.utf(icon)
-        self.__print_rawline(click.style("   {} {:8.2f}s{}{:7}{}{}".format(
-            icon,
-            time,
-            self.utf("sep_v"),
-            label,
-            self.utf("sep_v"),
-            name),
-            fg=colorname, bold=True))
-
-    def debug(self, msg):
-        """prints a debug message
-        """
-        if(self._verbose >= 2):
-            if type(msg) != list:
-                msg = [msg]
-            for elt in msg:
-                for line in elt.split('\n'):
-                    self.__print_rawline("DEBUG: {}".format(
-                        click.style(line, fg="bright_black")), err=True)
-
-    def info(self, msg):
-        """prints an info message
-        """
-        if(self._verbose >= 1):
-            if type(msg) != list:
-                msg = [msg]
-            for elt in msg:
-                for line in elt.split('\n'):
-                    self.__print_rawline("INFO : {}".format(
-                        click.style(line, fg="cyan")),  err=True)
-
-    def warn(self, msg):
-        """prints a warning message
-        """
-        if type(msg) != list:
-            msg = [msg]
-        for elt in msg:
-            for line in elt.split('\n'):
-                self.__print_rawline("WARN : {}".format(
-                    click.style(line, fg="yellow", bold=True)),  err=True)
-
-    def err(self, msg):
-        """prints an error message
-        """
-        if type(msg) != list:
-            msg = [msg]
-        enclosing_line = click.style(self.utf('hdr') * self._linelength,
-                                     fg="red",
-                                     bold=True)
-        self.__print_rawline("{}".format(enclosing_line),  err=True)
-        for elt in msg:
-            for line in elt.split('\n'):
-                self.__print_rawline("ERROR: {}".format(
-                    click.style(line, fg="red", bold=True)),  err=True)
-        self.__print_rawline("{}".format(enclosing_line),  err=True)
-
-    def print_short_banner(self, string=False):
-        """prints a little banner
-
-        :param string: True if the banner has to be returned, False if it has to be logged
-        :type string: bool
-        """
-        logo = [
-            r"""             ____    ______  _    __  _____       """,
-            r"""            / __ \  / ____/ | |  / / / ___/       """,
-            r"""           / /_/ / / /      | | / /  \__ \        """,
-            r"""          / ____/ / /___    | |/ /  ___/ /        """,
-            r"""         /_/      \____/    |___/  /____/         """,
-            r"""                                                  """,
-            r"""      Parallel Computing -- Validation System     """,
-            r"""             Copyright {} 2017 -- CEA             """.format(
-                self.utf('copy')),
-            r""""""
-        ]
-        s = []
-        if self._linelength < max(map(lambda x: len(x), logo)):
-            s = [
-                click.style("{}".format(self.utf("star")*14), fg="green"),
-                click.style("{} -- PCVS -- {}".format(self.utf("star"),
-                            self.utf('star')), fg="yellow"),
-                click.style("{} CEA {} 2017 {}".format(
-                    self.utf('star'), self.utf('copy'), self.utf('star')), fg="red"),
-                click.style("{}".format(self.utf("star")*14), fg="green")
-            ]
-        else:
-            start = " " * ((self._linelength - len(logo[0]))//2-1)
-            newline = "\n" + start
-            s = [
-                click.style(start + newline.join(logo[0:3]), fg="green"),
-                click.style(start + newline.join(logo[3:4]), fg="yellow"),
-                click.style(start + newline.join(logo[4:5]), fg="red"),
-                click.style(start + newline.join(logo[5:]))
-            ]
-        if string is True:
-            return "\n".join(s)
-        else:
-            self.__print_rawline("\n".join(s))
+        This is mainly used to ease the scheduling process by following the job
+        dependency graph.
 
-    def nimpl(self, *msg):  # pragma: no cover
-        """prints the "not implemented" error
+        :return: a Test object if possible, None otherwise
+        :rtype: :class:`Test` or NoneType
         """
-        self.err("This is not implemented (yet)!")
+        for d in self._deps:
+            if d.state == Test.State.WAITING:
+                return d
+        return None
 
-    def print_n_stop(self, **kwargs):  # pragma: no cover
-        """prints a message, then exits the program
-        """
-        # not replacing these prints (for debug only)
-        for k, v in kwargs.items():
-            click.secho("{}: ".format(k), fg="yellow", nl=False)
-            click.secho(pprint.pformat(v), fg="blue")
-        sys.exit(0)
-
-    def print_banner(self):
-        """prints a large banner
-        """
-        # ok,  this is ugly but the only way to make flake/pylint happy with
-        # source file formatting AND keeping a nicely logo printed out witout
-        # having to load a file.
-        # But, it is not trivial to edit. A single terminal line is split in
-        # half. Each 'logo' value is a line, created from the implicit
-        # concatenation of multiple raw strings (ex: logo= [r"a" r"b", r"c"])
-        #
-        # the full header can be found under the /utils/ source dir.
-        logo = [
-            r"""    ____                   ____     __   ______                            __  _             """,
-            r"""   / __ \____ __________ _/ / /__  / /  / ____/___  ____ ___  ____  __  __/ /_(_)___  ____ _ """,
-            r"""  / /_/ / __ `/ ___/ __ `/ / / _ \/ /  / /   / __ \/ __ `__ \/ __ \/ / / / __/ / __ \/ __ `/ """,
-            r""" / ____/ /_/ / /  / /_/ / / /  __/ /  / /___/ /_/ / / / / / / /_/ / /_/ / /_/ / / / / /_/ /  """,
-            r"""/_/    \__,_/_/   \__,_/_/_/\___/_/   \____/\____/_/ /_/ /_/ .___/\__,_/\__/_/_/ /_/\__, /   """,
-            r"""                                                          /_/                     /____/     """,
-            r"""                                              {} (PCVS) {}""".format(
-                self.utf('star'), self.utf('star')),
-            r"""    _    __      ___     __      __  _                _____            __                    """,
-            r"""   | |  / /___ _/ (_)___/ /___ _/ /_(_)___  ____     / ___/__  _______/ /____  ____ ___      """,
-            r"""   | | / / __ `/ / / __  / __ `/ __/ / __ \/ __ \    \__ \/ / / / ___/ __/ _ \/ __ `__ \     """,
-            r"""   | |/ / /_/ / / / /_/ / /_/ / /_/ / /_/ / / / /   ___/ / /_/ /__  / /_/  __/ / / / / /     """,
-            r"""   |___/\__,_/_/_/\__,_/\__,_/\__/_/\____/_/ /_/   /____/\__, /____/\__/\___/_/ /_/ /_/      """,
-            r"""                                                        /____/                               """,
-            r"""                                                                                            """,
-            r"""   Copyright {} 2017 Commissariat à l'Énergie Atomique et aux Énergies Alternatives (CEA)   """.format(
-                self.utf('copy')),
-            r"""                                                                                            """,
-            r"""  This program comes with ABSOLUTELY NO WARRANTY;                                           """,
-            r"""  This is free software, and you are welcome to redistribute it                             """,
-            r"""  under certain conditions; Please see COPYING for details.                                 """,
-            r"""                                                                                            """,
-        ]
+    @property
+    def timeout(self):
+        """Getter for Test timeout in seconds.
 
-        if self._linelength < max(map(lambda x: len(x), logo)):
+        It cumulates timeout + tolerance, this value being passed to the
+        subprocess.timeout.
 
-            self.print_short_banner()
-            return
+        :return: an integer if a timeout is defined, None otherwise
+        :rtype: int or NoneType
+        """
+        
+        # timeout is (in order):
+        # 1. explicitly defined
+        # 2. OR extrapolated from defined result.mean
+        # 3. set by default (MetaConfig.root.validation.job_timeout)
+        if self._timeout:
+            return self._timeout
+        elif self._validation['time'] > 0:
+            return (self._validation['time'] + self._validation['delta']) * 1.5
         else:
-            start = " " * ((self._linelength - len(logo[0]))//2-1)
-            newline = "\n" + start
-            self.__print_rawline(click.style(
-                start + newline.join(logo[0:6]), fg="green"))
-            self.__print_rawline(click.style(start + newline.join(logo[6:7])))
-            self.__print_rawline(click.style(start +
-                                             newline.join(logo[7:10]), fg="green"))
-            self.__print_rawline(click.style(start +
-                                             newline.join(logo[10:11]), fg="yellow"))
-            self.__print_rawline(click.style(
-                start + newline.join(logo[11:13]), fg="red"))
-            self.__print_rawline(click.style(start + newline.join(logo[13:])))
-
-
-manager = IOManager()
-
-
-def init(v=0, e=False, l=100, quiet=False):
-    """initializes a global manager for everyone to use
-
-    :param v: verbosity level, defaults to 0
-    :type v: int, optional
-    :param e: True to enable unicode alphabet, False to use ascii, defaults to
-        False
-    :type e: bool, optional
-    :param l: length of the terminal, defaults to 100
-    :type l: int, optional
-    :param quiet: False to write to stdout, defaults to False
-    :type quiet: bool, optional
-    """
-    global manager
-    manager = IOManager(verbose=v, enable_unicode=e, length=l, tty=(not quiet))
+            return MetaConfig.root.validation.job_timeout
 
+    def get_dim(self, unit="n_node"):
+        """Return the orch-dimension value for this test.
 
-def progbar(it, print_func=None, man=None, **kargs):
-    """prints a progress bar using click
+        The dimension can be defined by the user and let the orchestrator knows
+        what resource are, and how to 'count' them'. This accessor allow the
+        orchestrator to exract the information, based on the key name.
 
-    :param it: iterable on which the progress bar has to iterate
-    :type it: iterable
-    :param print_func: method used to show the item next to the progress bar,
-        defaults to None
-    :type print_func: function, optional
-    :param man: manager used to describe the bullets, defaults to None
-    :type man: log.IOManager, optional
-    :return: a click progress bar (iterable)
-    :rtype: click.ProgressBar
-    """
-    if man is None:
-        man = manager
-    return click.progressbar(
-        it, empty_char=man.utf('empty_pg'),
-        info_sep=man.utf('sep_v'), fill_char=man.utf('full_pg'),
-        show_percent=False, show_eta=False, show_pos=False,
-        item_show_func=print_func,
-        **kargs)
+        :param unit: the resource label, such label should exist within the test
+        :type unit: str
+
+        :return: The number of resource this Test is requesting.
+        :rtype: int
+        """
+        return self._dim
+
+    def save_final_result(self, rc=0, time=None, out=b'', state=None):
+        """Build the final Test result node.
+
+        :param rc: return code, defaults to 0
+        :type rc: int, optional
+        :param time: elapsed time, defaults to 0.0
+        :type time: float, optional
+        :param out: standard out/err, defaults to b''
+        :type out: bytes, optional
+        :param state: Job final status (if override needed), defaults to FAILED
+        :type state: :class:`Test.State`, optional
+        """
+        if state is None:
+            state = Test.State.SUCCESS if self._validation['expect_rc'] == rc else Test.State.FAILURE
+
+        self.save_raw_run(rc=rc, out=out, time=time)
+        self.save_status(state)
+
+        for elt_k, elt_v in self._data['artifacts'].items():
+            if os.path.isfile(elt_v):
+                with open(elt_v, 'rb') as fh:
+                    self._data['artifacts'][elt_k] = base64.b64encode(
+                        fh.read()).decode("utf-8")
+
+    def save_raw_run(self, out=None, rc=None, time=None):
+        """TODO:
+        """
+        if rc is not None:
+            self._rc = rc
+        if out is not None:
+            self._output = base64.b64encode(out)
+            self._output_info['raw'] = self._output
+        if time is not None:
+            self._exectime = time
+
+    def extract_metrics(self):
+        """TODO:
+        """
+        raw_output = self.output
+        for name in self._data['metrics'].keys():
+            node = self._data['metrics'][name]
+
+            try:
+                ens = set if node['attributes']['unique'] else list
+            except KeyError:
+                ens = list
+
+            self._data['metrics'][name]['values'] = list(
+                ens(re.findall(node['key'], raw_output)))
+
+    def evaluate(self):
+        """TODO:
+        """
+        state = Test.State.SUCCESS
+
+        if self._validation['expect_rc'] != self._rc:
+            state = Test.State.FAILURE
+
+        raw_output = self.output
+
+        # if test should be validated through a matching regex
+        if state == Test.State.SUCCESS and self._validation['matchers'] is not None:
+            for k, v in self._validation['matchers'].items():
+                expected = (v.get('expect', True) is True)
+                found = re.search(v['expr'], raw_output)
+                if (found and not expected) or (not found and expected):
+                    state = Test.State.FAILURE
+                    break
+
+        if state == Test.State.SUCCESS and self._validation['analysis'] is not None:
+            analysis = self._validation['analysis']
+            args = self._validation.get('args', {})
+            s = MetaConfig.root.get_internal("pColl").invoke_plugins(
+                Plugin.Step.TEST_RESULT_EVAL, analysis=analysis, job=self)
+            if s is not None:
+                state = s
+
+        # if a custom script is provided
+        if state == Test.State.SUCCESS and self._validation['script'] is not None:
+            p = Program(self._validation['script'])
+            p.run()
+            if self._validation['expect_rc'] != p.rc:
+                state = Test.State.FAILURE
+        self._state = state
+
+    def save_status(self, state):
+        self.executed(state)
+
+    def display(self):
+        """Print the Test into stdout (through the manager)."""
+        colorname = "yellow"
+        icon = ""
+        label = str(self._state)
+        raw_output = None
+        if self._state == Test.State.SUCCESS:
+            colorname = "green"
+            icon = "succ"
+        elif self._state == Test.State.FAILURE:
+            colorname = "red"
+            icon = "fail"
+        elif self._state in [Test.State.ERR_DEP, Test.State.ERR_OTHER]:
+            colorname = "yellow"
+            icon = "fail"
+
+        if self._output and \
+            (MetaConfig.root.validation.print_level == 'all' or
+             (self.state == Test.State.FAILURE) and MetaConfig.root.validation.print_level == 'errors'):
+            raw_output = self.output
+
+        io.console.print_job(label, self._exectime, self.label,
+                             "/{}".format(self.subtree) if self.subtree else "",
+                             self.name,
+                             colorname=colorname, icon=icon, content=raw_output)
+
+    def executed(self, state=None):
+        """Set current Test as executed.
+
+        :param state: give a special state to the test, defaults to FAILED
+        :param state: :class:`Test.State`, optional
+        """
+        self._state = state if type(
+            state) == Test.State else Test.State.FAILURE
+
+    def been_executed(self):
+        """Cehck if job has been executed (not waiting or in progress).
+
+        :return: False if job is waiting for scheduling or in progress.
+        :rtype: bool
+        """
+        return self._state not in [Test.State.WAITING, Test.State.IN_PROGRESS]
+
+    def pick(self):
+        """Flag the job as picked up for scheduling."""
+        self._state = Test.State.IN_PROGRESS
+
+    def not_picked(self):
+        self._sched_cnt += 1
+        return self._sched_cnt >= self.SCHED_MAX_ATTEMPTS
+
+    def pick_count(self):
+        return self._sched_cnt
+
+    @property
+    def state(self):
+        """Getter for current job state.
+
+        :return: the job current status.
+        :rtype: :class:`Test.State`
+        """
+        return self._state
+
+    @property
+    def encoded_output(self) -> bytes:
+        return self._output
+    
+    @encoded_output.setter
+    def encoded_output(self, v) -> None:
+        self._output = v
+        self._output_info['raw'] = v
+
+    def get_raw_output(self, encoding="utf-8") -> bytes:
+        base = base64.b64decode(self._output)
+
+        return base if not encoding else base.decode(encoding)
+
+    @property
+    def output(self) -> str:
+        return self.get_raw_output(encoding='utf-8')
+    
+    @property
+    def output_info(self) -> dict:
+        return self._output_info
+
+    @property
+    def time(self):
+        """TODO:
+        """
+        return self._exectime
+    
+    @property
+    def retcode(self):
+        return self._rc
+
+    def to_json(self, strstate=False):
+        """Serialize the whole Test as a JSON object.
+
+        :return: a JSON object mapping the test
+        :rtype: str
+        """
+        res = {
+            "id": self._id,
+            "exec": self._execmd,
+            "result": {
+                "rc": self._rc,
+                "state": str(self._state) if strstate else self._state,
+                "time": self._exectime,
+                "output": self._output_info
+            },
+            "data": self._data
+        }
+        
+        return res
+
+    def to_minimal_json(self):
+        return {
+            "jid": self.jid,
+            "invocation_cmd": self._invocation_cmd,
+        }
+    
+    def from_minimal_json(self, json: str):
+        if isinstance(json, str):
+            json = json.loads(json)
+        self._invocation_cmd = json.get('invocation_cmd', "exit 1")
+        self._id['jid'] = json.get('jid', "-1")
+        
+        
+    def from_json(self, test_json: str) -> None:
+        """Replace the whole Test structure based on input JSON.
+
+        :param json: the json used to set this Test
+        :type json: test-result-valid JSON-formated str
+        """
+
+        if isinstance(test_json, str):
+            test_json = json.loads(test_json)
+
+        assert (isinstance(test_json, dict))
+        self.res_scheme.validate(test_json)
+
+        self._id = test_json.get("id", -1)
+        self._comb = Combination({}, self._id.get('comb', {}))
+        self._execmd = test_json.get("exec", "")
+        self._data = test_json.get("data", "")
+
+        res = test_json.get("result", {})
+        self._rc = res.get("rc", -1)
+        self._state = Test.State(res.get("state", Test.State.ERR_OTHER))
+        self._exectime = res.get("time", 0)
+        self._output_info = res.get("output", {})
+        self._output = self._output_info.get('raw', b"")
+        if type(self._output) == str:
+            # should only be managed as bytes (as produced by b64 encoding)
+            self._output = self._output.encode('utf-8')
+
+    def generate_script(self, srcfile):
+        """Serialize test logic to its Shell representation.
+
+        This script provides the shell sequence to put in a shell script
+        switch-case, in order to reach that test from script arguments.
+
+        :param srcfile: script filepath, to store the actual wrapped command.
+        :type srcfile: str
+        :return: the shell-compliant instruction set to build the test
+        :rtype: str
+        """
+        pm_code = ""
+        cd_code = ""
+        env_code = ""
+        cmd_code = ""
+        post_code = ""
+
+        self._invocation_cmd = 'bash {} {}'.format(
+            srcfile, self._id['fq_name'])
+
+        # if changing directory is required by the test
+        if self._cwd is not None:
+            cd_code += "cd '{}'".format(shlex.quote(self._cwd))
+
+        # manage package-manager deps
+        for elt in self._mod_deps:
+            pm_code += "\n".join([elt.get(load=True, install=True)])
+
+        # manage environment variables defined in TE
+        if self._testenv is not None:
+            envs = []
+            for e in self._testenv:
+                k, v = e.split('=', 1)
+                envs.append("{k}={v}; export {k}".format(k=shlex.quote(k),
+                                                         v=shlex.quote(v)))
+            env_code = "\n".join(envs)
+            
+                
+        cmd_code = self._execmd
+
+        return """
+        "{name}")
+            {cd_code}
+            pcvs_load={pm_code}
+            pcvs_env={env_code}
+            pcvs_cmd={cmd_code}
+            ;;""".format(
+            cmd_code="{}".format(shlex.quote(cmd_code)),
+            env_code="{}".format(shlex.quote(env_code)),
+            pm_code="{}".format(shlex.quote(pm_code)),
+            cd_code=cd_code,
+            name=self._id['fq_name']
+        )
+
+    @classmethod
+    def compute_fq_name(self, label, subtree, name, combination=None, suffix=None):
+        """Generate the fully-qualified (dq) name for a test, based on :
+            - the label & subtree (original FS tree)
+            - the name (the TE name it is originated)
+            - a potential extra suffix
+            - the combination PCVS computed for this iteration."""
+        return "_".join(filter(None, [
+            "/".join(filter(None, [
+                label,
+                subtree,
+                name])),
+            suffix,
+            combination]))
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pcvs-0.6.0/pcvs/helpers/pm.py` & `pcvs-0.7.0/pcvs/helpers/pm.py`

 * *Files identical despite different names*

### Comparing `pcvs-0.6.0/pcvs/helpers/system.py` & `pcvs-0.7.0/pcvs/helpers/system.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import addict
 import jsonschema
 from ruamel.yaml import YAML, YAMLError
 
 import pcvs
 from pcvs import NAME_BUILDIR, PATH_INSTDIR
+from pcvs.io import Verbosity
 from pcvs.helpers import git, pm
 from pcvs.helpers.exceptions import CommonException, ValidationException
 
 
 ####################################
 ####   YAML VALIDATION OBJECT   ####
 ####################q################
@@ -63,17 +64,15 @@
         try:
             if filepath is None:
                 filepath = "'data stream'"
 
             jsonschema.validate(instance=content, schema=self._scheme)
         except jsonschema.exceptions.ValidationError as e:
             raise ValidationException.FormatError(
-                "Scheme '{}' failed to verify the following file:\n{}".format(
-                    self._name, filepath),
-                reason=e.message)
+                reason="Failed to validate input file: {}".format(e.message), file=filepath, scheme=self._scheme)
         except jsonschema.exceptions.SchemaError as e:
             raise ValidationException.SchemeError(
                 name=self._name,
                 content=self._scheme,
                 error=e)
 
 
@@ -121,15 +120,15 @@
         """Check if the Config instance matches the expected format as declared
         in schemes/. As the 'category' is not carried by the object itself, it
         is provided by the function argument.
 
         :param kw: keyword describing the configuration to be validated (scheme)
         :type kw: str
         """
-        assert(kw in ValidationScheme.available_schemes())
+        assert (kw in ValidationScheme.available_schemes())
         ValidationScheme(kw).validate(self)
 
     def __setitem__(self, param, value):
         """extend it to handle dict initialization (needs MetaDict conversion)
         :param param: name of value to add to configuration
         :type param: str
         :param value: value to add to configuration
@@ -149,23 +148,17 @@
 
     def set_nosquash(self, k, v):
         """shortcut function: init self[k] only if v is not already set
         :param k: name of value to add
         :type k: str
         :param v: value to add
         :type v: str"""
-        if not self.isset(k):
+        if k not in self:
             self[k] = v
 
-    def isset(self, k):
-        """check key existence in config dict
-        :param k: name of param to check
-        :type k: str"""
-        return k in self
-
     def to_dict(self):
         """Convert the Config() to regular dict."""
         # this dirty hack is due to a type(self) used into addict.py
         # leading to misconvert derived classes from Dict()
         # --> to_dict() checks if a sub-value is instance of type(self)
         # In our case here, type(self) return Config(), addict not converting
         # sub-Dict() into dict(). This double call to to_dict() seems
@@ -216,16 +209,16 @@
         :param kwargs: list of keyword-based arguments
         """
         super().__init__(*args, **kwargs)
 
         # The 'internal' node is a special one. Put here anything not requiring
         # to be published (like conf.yml, etc...). mainly one-time Python
         # objects
-        if '__internal' not in self:
-            self['__internal'] = Config()
+
+        #self.__internal_config = Config()
 
     def __setitem__(self, param, value):
         """Extend the default MetaDict setter mthod to reach the base class one"""
         super().__setitem__(param, value)
 
     def bootstrap_generic(self, subnode, node):
         """"Initialize a Config() object and store it under name 'node'
@@ -240,14 +233,25 @@
             self[subnode] = Config()
 
         for k, v in node.items():
             self[subnode][k] = v
 
         self[subnode].validate(subnode)
         return self[subnode]
+    
+    def bootstrap_from_profile(self, pf_as_dict):
+        
+        if not isinstance(pf_as_dict, MetaDict):
+            pf_as_dict = MetaDict(pf_as_dict)
+            
+        self.bootstrap_compiler(pf_as_dict.compiler)
+        self.bootstrap_runtime(pf_as_dict.runtime)
+        self.bootstrap_machine(pf_as_dict.machine)
+        self.bootstrap_criterion(pf_as_dict.criterion)
+        self.bootstrap_group(pf_as_dict.group)
 
     def bootstrap_compiler(self, node):
         """"Specific initialize for compiler config block
         :param node: compiler block to initialize
         :type node: dict
         :return: added node
         :rtype: dict"""
@@ -295,49 +299,57 @@
                 with open(filepath, 'r') as fh:
                     node = MetaDict(YAML(typ='safe').load(fh))
             except (IOError, YAMLError) as e:
                 raise CommonException.IOError(
                     "Error(s) found while loading (}".format(filepath))
 
         # some post-actions
-        for field in ["output", "reused_build", "runlog"]:
+        for field in ["output", "reused_build"]:
             if field in node:
                 node[field] = os.path.abspath(node[field])
 
         if node.dirs:
             node.dirs = {k: os.path.abspath(v) for k, v in node.dirs.items()}
 
         return self.bootstrap_validation(node)
 
+    def bootstrap_subnode(root_node, *default_subnode_dict):
+        for k, v in default_subnode_dict:
+            if k not in root_node:
+                root_node[k] = v
+
     def bootstrap_validation(self, node):
         """"Specific initialize for validation config block
         :param node: validation block to initialize
         :type node: dict
         :return: initialized node
         :rtype: dict"""
         subtree = self.bootstrap_generic('validation', node)
 
         # Initialize default values when not set by user or default files
-        subtree.set_nosquash('verbose', 0)
+        subtree.set_nosquash('verbose', str(Verbosity.COMPACT))
         subtree.set_nosquash('print_level', 'none')
         subtree.set_nosquash('color', True)
         subtree.set_nosquash('default_profile', 'default')
         subtree.set_nosquash('output', os.path.join(os.getcwd(), NAME_BUILDIR))
         subtree.set_nosquash('background', False)
         subtree.set_nosquash('override', False)
         subtree.set_nosquash('dirs', None)
         subtree.set_nosquash("spack_recipe", None)
-        subtree.set_nosquash('runlog', os.path.join(subtree.output, 'out.log'))
         subtree.set_nosquash('simulated', False)
         subtree.set_nosquash('anonymize', False)
         subtree.set_nosquash('onlygen', False)
         subtree.set_nosquash('timeout', None)
         subtree.set_nosquash('target_bank', None)
         subtree.set_nosquash('reused_build', None)
         subtree.set_nosquash('webreport', None)
+        subtree.set_nosquash("only_success", False)
+        subtree.set_nosquash("enable_report", False)
+        subtree.set_nosquash('job_timeout', 86400)
+        subtree.set_nosquash('per_result_file_sz', 10 * 1024 * 1024)
         subtree.set_nosquash(
             'buildcache', os.path.join(subtree.output, 'cache'))
         subtree.set_nosquash('result', {"format": ['json']})
         subtree.set_nosquash('author', {
             "name": git.get_current_username(),
             "email": git.get_current_usermail()})
 
@@ -392,30 +404,36 @@
 
     def set_internal(self, k, v):
         """manipulate the internal MetaConfig() node to store not-exportable data
         :param k: name of value to add
         :type k: str
         :param v: value to add
         :type v: str"""
-        self['__internal'][k] = v
+        if not hasattr(self, "__internal_config"):
+            self.__internal_config = {}
+        self.__internal_config[k] = v
 
     def get_internal(self, k):
         """manipulate the internal MetaConfig() node to load not-exportable data
         :param k: value to get
         :type k: str"""
-        if k in self['__internal']:
-            return self['__internal'][k]
+        if not hasattr(self, "__internal_config"):
+            return None
+
+        if k in self.__internal_config:
+            return self.__internal_config[k]
         else:
             return None
 
     def dump_for_export(self):
         """Export the whole configuration as a dict. Prune any __internal node
         beforehand.
         """
-        res = MetaDict()
-        for k, v in self.items():
-            if k == '__internal':
-                continue
-            # should ignore __internal
-            res[k] = v.to_dict()
+        if self.__internal_config:
+            not_exported = self.__internal_config
+            del self.__internal_config
+            res = MetaDict(self.to_dict())
+            self.__internal_config = not_exported
+        else:
+            res = self
 
         return res.to_dict()
```

### Comparing `pcvs-0.6.0/pcvs/helpers/utils.py` & `pcvs-0.7.0/pcvs/helpers/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,18 @@
-import subprocess
 import os
-import socket
 import shutil
 import signal
+import socket
+import subprocess
 import time
 from contextlib import contextmanager
 from shutil import SameFileError
 
 from pcvs import (NAME_BUILDFILE, NAME_BUILDIR, NAME_SRCDIR, PATH_HOMEDIR,
-                  PATH_INSTDIR)
-from pcvs.helpers import log
+                  PATH_INSTDIR, io)
 from pcvs.helpers.exceptions import (CommonException, LockException,
                                      RunException)
 
 ####################################
 ##    STORAGE SCOPE MANAGEMENT    ##
 ####################################
 STORAGES = {
@@ -144,15 +143,15 @@
     :param dir: True if the path is a directory, defaults to False
     :type dir: bool, optional
     """
     if not os.path.exists(prefix):
         if dir:
             os.mkdir(prefix)
         else:
-            assert(os.path.isdir(os.path.dirname(prefix)))
+            assert (os.path.isdir(os.path.dirname(prefix)))
             open(prefix, 'w+').close()
         return
 
     # else, a previous path exists
     if os.path.isdir(prefix):
         shutil.rmtree(prefix)
         os.mkdir(prefix)
@@ -190,14 +189,16 @@
         shutil.copy(src, dest)
     except SameFileError:
         pass
 
 ####################################
 ####           MISC.            ####
 ####################################
+
+
 def check_valid_program(p, succ=None, fail=None, raise_if_fail=True):
     """Check if p is a valid program, using the ``which`` function.
 
     :param p: program to check
     :type p: str
     :param succ: function to call in case of success, defaults to None
     :type succ: optional
@@ -272,15 +273,16 @@
 
     :param f: file locking the directory
     :type f: os.path
     """
     lf_name = get_lockfile_name(f)
     if os.path.exists(lf_name) and os.path.isfile(lf_name):
         os.remove(lf_name)
-        log.manager.debug("Unlock {}".format(lf_name))
+        if io.console:
+            io.console.debug("Unlock {}".format(lf_name))
 
 
 def lock_file(f, reentrant=False, timeout=None, force=True):
     """Try to lock a directory.
 
     :param f: name of lock
     :type f: os.path
@@ -290,16 +292,16 @@
     :param timeout: time before timeout, defaults to None
     :type timeout: int (seconds), optional
     :raises LockException.TimeoutError: timeout is reached before the directory
         is locked
     :return: True if the file is reached, False otherwise
     :rtype: bool
     """
-
-    log.manager.debug("Attempt locking {}".format(f))
+    if io.console:
+        io.console.debug("Attempt locking {}".format(f))
     if force:
         unlock_file(f)
     locked = trylock_file(f, reentrant)
     count = 0
     while not locked:
         time.sleep(1)
         count += 1
@@ -320,21 +322,22 @@
     :return: True if the file is reached, False otherwise
     :rtype: bool
     """
     lockfile_name = get_lockfile_name(f)
     if not os.path.exists(lockfile_name):
         with open(lockfile_name, 'w') as fh:
             fh.write("{}||{}".format(socket.gethostname(), os.getpid()))
-        log.manager.debug("Lock {}".format(lockfile_name))
+        if io.console:
+            io.console.debug("Lock {}".format(lockfile_name))
         return True
     else:
         try:
             hostname, pid = get_lock_owner(f)
             if pid == os.getpid() and hostname == socket.gethostname() and reentrant:
-                log.manager.debug("Lock {}".format(lockfile_name))
+                io.console.debug("Lock {}".format(lockfile_name))
                 return True
         except ValueError as e:
             pass  # return False
 
         return False
 
 
@@ -363,92 +366,131 @@
     with open(lf_name, 'r') as fh:
         s = fh.read().strip().split('||')
         return s[0], int(s[1])
 
 
 def program_timeout(sig, frame):
     """Timeout handler, called when a SIGALRM is received.
-    
+
     :param sig: signal number
     :type sig: int
     :param frame: the callee (unused)
     :type f: 
     :raises CommonException.TimeoutError: timeout is reached
     """
-    assert(sig == signal.SIGALRM)
+    assert (sig == signal.SIGALRM)
     raise CommonException.TimeoutError("Timeout reached")
 
 
 def start_autokill(timeout=None):
     """Initialize a new time to automatically stop the 
     current process once time is expired.
-    
+
     :param timeout: value in seconds before the autokill will be raised
     :type timeout: positive integer
     """
     if isinstance(timeout, int):
-        log.manager.print_item(
+        io.console.print_item(
             "Setting timeout to {} second(s)".format(timeout))
         signal.signal(signal.SIGALRM, program_timeout)
 
         signal.alarm(timeout)
 
 
 class Program:
     """Simple class to encapsulate process management.
-    
+
     This is better and should be preferred as importing subprocess everywhere.
     """
+
     def __init__(self, cmd=None):
         self._cmd = cmd
         self._out = None
         self._rc = None
         self._except = None
 
     def run(self, input="", shell=False, timeout=0):
         """Run the given program and capture I/Os
-        
+
         :param input: raw data to be used as stdin
         :type input: str
         :param shell: is the provided command to be run within a shell
         :type shell: boolean
         :param timeout: allowed time before automatically killing the process
         :type timeout: positive integer
         :return: zero if the process started successfully, non-zero
             otherwise.
         :rtype: integer
         """
         try:
-            s = subprocess.Popen(self._cmd, shell=shell, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
+            s = subprocess.Popen(self._cmd, shell=shell,
+                                 stdout=subprocess.PIPE, stderr=subprocess.PIPE)
             self._out = s.communicate(input=input)
             self._rc = s.returncode
         except Exception as e:
             self._except = e
             return 1
         return 0
 
     @property
     def out(self):
         """Getter to actual execution output.
-        
+
         :return: stderr/stdout combined
         :rtype: str
         """
         return self._out
 
     @property
     def rc(self):
         """Getter, effective return code.
-        
+
         :return: return code
         :rtype: integer
         """
         return self._rc
 
     @property
     def exception(self):
         """Getter, raised exception (for any reason)
-        
+
         :return: an Exception-derived object
         :rtype: Exception
         """
-        return self._except
+        return self._except
+
+
+def str_dict_as_envvar(d):
+    """Convert a dict to a list of shell-compliant variable strings.
+
+    The final result is a regular multiline str, each line being an entry.
+
+    :param d: the dict containing env vars to serialize
+    :type d: dict
+    :return: the str, containing mulitple lines, each of them being a var.
+    :rtype: str
+    """
+    return "\n".join(["{}='{}'".format(i, d[i]) for i in sorted(d.keys())])
+
+
+def check_is_buildir(p):
+    if not os.path.isdir(p):
+        return False
+    return NAME_BUILDFILE in os.listdir(p)
+
+
+def check_is_archive(f):
+    if not os.path.isfile(f):
+        return False
+    return os.path.basename(f).startswith("pcvsrun_")
+
+
+def check_is_build_or_archive(x):
+    return check_is_buildir(x) or check_is_archive(x)
+
+
+def list_valid_buildirs_in_dir(p):
+    return [os.path.join(root, d) for root, d, _ in os.walk(p) if check_is_buildir(p)]
+
+
+def list_valid_archive_in_dir(p):
+    return [os.path.join(root, f) for root, _, f in os.walk(p) if check_is_archive(f)]
```

### Comparing `pcvs-0.6.0/pcvs/main.py` & `pcvs-0.7.0/pcvs/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 #!/usr/bin/env python3
+import pkg_resources
 
-import os
-import shutil
-
-import click
-
-from pcvs import version
-from pcvs.backend import bank, config, profile, session
+from pcvs import io
+from pcvs.backend import bank, config, profile
 from pcvs.cli import (cli_bank, cli_config, cli_profile, cli_report, cli_run,
-                      cli_session, cli_utilities, cli_plumbing)
-from pcvs.helpers import log, utils
+                      cli_session, cli_utilities, cli_remote_run)
+from pcvs.helpers import utils
 from pcvs.helpers.exceptions import PluginException
 from pcvs.plugins import Collection, Plugin
 
+try:
+    import rich_click as click
+    click.rich_click.SHOW_ARGUMENTS = True
+except ImportError:
+    import click
+
 CONTEXT_SETTINGS = dict(
     help_option_names=['-h', '--help', '-help'],
     ignore_unknown_options=True,
     allow_interspersed_args=False,
     auto_envvar_prefix='PCVS'
 )
 
@@ -31,22 +33,27 @@
     :param param: the option triggering the callback (unused here)
     :type param: str
     :param value: the value provided with the option (unused here)
     """
     if not value or ctx.resilient_parsing:
         return
     click.echo(
-        'Parallel Computing Validation System (pcvs) -- version {}'.format(version.__version__))
+        'Parallel Computing Validation System (pcvs) -- version {}'.format(pkg_resources.require("pcvs")[0].version))
     ctx.exit()
 
 
+i = 0
+
+
 @click.group(context_settings=CONTEXT_SETTINGS, name="cli")
 @click.option("-v", "--verbose", "verbose", show_envvar=True,
               count=True, default=0,
-              help="Enable PCVS debug verbosity (cumulative)")
+              help="Enable PCVS verbosity (cumulative)")
+@click.option("-d", "--debug", show_envvar=True, default=False,
+              help="Enable Debug mode (implies `-vvv`)", is_flag=True)
 @click.option("-c", "--color/--no-color", "color",
               default=True, is_flag=True, show_envvar=True,
               help="Use colors to beautify the output")
 @click.option("-g", "--glyph/--no-glyph", "encoding",
               default=True, is_flag=True, show_envvar=True,
               help="enable/disable Unicode glyphs")
 @click.option("-C", "--exec-path", "exec_path", show_envvar=True,
@@ -56,31 +63,32 @@
               is_flag=True, help="Display current version")
 @click.option("-w", "--width", "width", type=int, default=None,
               help="Terminal width (autodetection if omitted")
 @click.option("-P", "--plugin-path", "plugin_path", multiple=True,
               type=click.Path(exists=True), show_envvar=True,
               help="Default Plugin path prefix")
 @click.option("-m", "--plugin", "select_plugins", multiple=True)
+@click.option("-t", "--tui", is_flag=True, default=False, show_envvar=True,
+              help="USe TUI-based interface instead of console (if applicable)")
 @click.pass_context
-@log.manager.capture_exception(PluginException.NotFoundError)
-def cli(ctx, verbose, color, encoding, exec_path, width, plugin_path, select_plugins):
+@io.capture_exception(PluginException.NotFoundError)
+@io.capture_exception(PluginException.LoadError)
+def cli(ctx, verbose, color, encoding, exec_path, width, plugin_path, select_plugins, tui, debug):
     """PCVS main program."""
     ctx.ensure_object(dict)
-    ctx.obj['verbose'] = verbose
+    ctx.obj['verbose'] = verbose if not debug else 10
     ctx.obj['color'] = color
     ctx.obj['encode'] = encoding
     ctx.obj['exec'] = exec_path
+    ctx.obj['tui'] = tui
 
     # Click specific-related
     ctx.color = color
 
-    if width is None:
-        width = shutil.get_terminal_size()[0]
-    log.init(verbose, encoding, width)
-
+    io.init(color=color, verbose=verbose)
     utils.set_local_path(ctx.obj['exec'])
 
     utils.create_home_dir()
 
     pcoll = Collection()
     ctx.obj['plugins'] = pcoll
 
@@ -111,11 +119,12 @@
 cli.add_command(cli_session.session)
 cli.add_command(cli_utilities.exec)
 cli.add_command(cli_utilities.check)
 cli.add_command(cli_utilities.clean)
 cli.add_command(cli_utilities.discover)
 # cli.add_command(cli_gui.gui)
 cli.add_command(cli_report.report)
-#cli.add_command(cli_plumbing.resolve)
+cli.add_command(cli_remote_run.remote_run)
+# cli.add_command(cli_plumbing.resolve)
 
 if __name__ == "__main__":
     cli()
```

### Comparing `pcvs-0.6.0/pcvs/orchestration/__init__.py` & `pcvs-0.7.0/pcvs/orchestration/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,17 @@
+import os
 import queue
 
+from pcvs import NAME_BUILD_RESDIR, io
 from pcvs.backend import session
 from pcvs.helpers import log
 from pcvs.helpers.system import MetaConfig
 from pcvs.orchestration.manager import Manager
-from pcvs.orchestration.publishers import Publisher
-from pcvs.orchestration.set import Runner, Set
+from pcvs.orchestration.set import Set
+from pcvs.orchestration.runner import RunnerAdapter
 from pcvs.plugins import Plugin
 from pcvs.testing.test import Test
 
 
 def global_stop(e):
     Orchestrator.stop()
     raise e
@@ -20,146 +22,155 @@
 
     :ivar _conf: global configuration object
     :type _conf: :class:`MetaConfig`
     :ivar _pending_sets: started Sets not completed yet
     :type _pending_sets: list
     :ivar _max_res: number of resources allowed to be used
     :type _max_res: int
-    :ivar _publisher: result publisher
-    :type _publisher: :class:`Publisher`
+    :ivar _publisher: Result File Manager
+    :type _publisher: :class:`ResultFileManager`
     :ivar _manager: job manager
     :type _manager: :class:`Manager`
     :ivar _maxconcurrent: Max number of sets started at the same time.
     :type _maxconcurrent: int
 
     """
 
     def __init__(self):
         """constructor method"""
         config_tree = MetaConfig.root
         self._conf = config_tree
         self._runners = list()
         self._max_res = config_tree.machine.get('nodes', 1)
-        self._publisher = Publisher(config_tree.validation.output)
+        self._publisher = config_tree.get_internal('build_manager').results
         self._manager = Manager(self._max_res, publisher=self._publisher)
         self._maxconcurrent = config_tree.machine.get('concurrent_run', 1)
         self._complete_q = queue.Queue()
         self._ready_q = queue.Queue()
 
     def print_infos(self):
         """display pre-run infos."""
-        log.manager.print_item("Test count: {}".format(
+        io.console.print_item("Test count: {}".format(
             self._manager.get_count('total')))
-        log.manager.print_item(
+        io.console.print_item(
             "Max simultaneous Sets: {}".format(self._maxconcurrent))
-        log.manager.print_item("Resource count: {}".format(self._max_res))
+        io.console.print_item("Resource count: {}".format(self._max_res))
 
     # This func should only be a passthrough to the job manager
     def add_new_job(self, job):
         """Append a new job to be scheduled.
 
         :param job: job to append
         :type job: :class:`Test`
         """
         self._manager.add_job(job)
 
-    @log.manager.capture_exception(KeyboardInterrupt, global_stop)
+    @io.capture_exception(KeyboardInterrupt, global_stop)
     def start_run(self, the_session=None, restart=False):
         """Start the orchestrator.
 
         :param the_session: container owning the run.
         :type the_session: :class:`Session`
         :param restart: whether the run is starting from scratch
         :type restart: False for a brand new run.
         """
 
         MetaConfig.root.get_internal(
             "pColl").invoke_plugins(Plugin.Step.SCHED_BEFORE)
 
-        log.manager.info("ORCH: initialize runners")
+        io.console.info("ORCH: initialize runners")
         for i in range(0, self._maxconcurrent):
             self.start_new_runner()
 
         self._manager.resolve_deps()
+        if io.console.verb_debug:
+            self._manager.print_dep_graph(outfile="./graph.dat")
 
-        nb_nodes = self._max_res
+        nb_res = self._max_res
         last_progress = 0
-        log.manager.info("ORCH: start job scheduling")
+        pending_list = list()
+        io.console.info("ORCH: start job scheduling")
         # While some jobs are available to run
-        while self._manager.get_leftjob_count() > 0 or not self._ready_q.empty():
-            # dummy init value
-            new_set: Set = not None
-            while new_set is not None:
-                # create a new set, if not possible, returns None
-                new_set = self._manager.create_subset(nb_nodes)
-                if new_set is not None:
-                    # schedule the set asynchronously
-                    nb_nodes -= new_set.dim
-                    log.manager.debug("ORCH: send Set to queue (#{}, sz:{})".format(new_set.id, new_set.size))
-                    self._ready_q.put(new_set)
-
-            # Now, look for a completion
-            try:
-                set = self._complete_q.get(block=False, timeout=2)
-                log.manager.debug("ORCH: recv Set from queue (#{}, sz:{})".format(
+        with io.console.table_container(self._manager.get_count()):
+            while self._manager.get_leftjob_count() > 0 or len(pending_list) > 0:
+                # dummy init value
+                new_set: Set = not None
+                while new_set is not None:
+                    # create a new set, if not possible, returns None
+                    new_set = self._manager.create_subset(nb_res)
+                    if new_set is not None:
+                        assert(isinstance(nb_res, int))
+                        # schedule the set asynchronously
+                        nb_res -= new_set.dim
+                        io.console.debug("ORCH: send Set to queue (#{}, sz:{})".format(
+                            new_set.id, new_set.size))
+                        self._ready_q.put(new_set)
+                    else:
+                        self._manager.prune_non_runnable_jobs()
+
+                # Now, look for a completion
+                try:
+                    set = self._complete_q.get(block=False, timeout=2)
+                    io.console.debug("ORCH: recv Set from queue (#{}, sz:{})".format(
                         set.id, set.size))
-                nb_nodes += set.dim
-                self._manager.merge_subset(set)
-            except queue.Empty:
-                pass
-                # TODO: create backup to allow start/stop
-
-            current_progress = self._manager.get_count(
-                'executed') / self._manager.get_count('total')
-
-            # Condition to trigger a dump of results
-            # info result file at a periodic step of 5% of
-            # the global workload
-            if (current_progress - last_progress) > 0.05:
-                # TODO: Publish results periodically
-                # 1. on file system
-                # 2. directly into the selected bank
-                log.manager.debug("ORCH: Flush a new progression file")
-                self._publisher.flush()
-                last_progress = current_progress
-                if the_session is not None:
-                    session.update_session_from_file(
-                        the_session.id, {'progress': current_progress * 100})
+                    nb_res += set.dim
+                    self._manager.merge_subset(set)
+                except queue.Empty:
+                    self._manager.prune_non_runnable_jobs()
+                    pass
+                    # TODO: create backup to allow start/stop
+
+                current_progress = self._manager.get_count(
+                    'executed') / self._manager.get_count('total')
+
+                # Condition to trigger a dump of results
+                # info result file at a periodic step of 5% of
+                # the global workload
+                if (current_progress - last_progress) > 0.05:
+                    # TODO: Publish results periodically
+                    # 1. on file system
+                    # 2. directly into the selected bank
+                    io.console.debug("ORCH: Flush a new progression file")
+                    self._publisher.flush()
+                    last_progress = current_progress
+                    if the_session is not None:
+                        session.update_session_from_file(
+                            the_session.id, {'progress': current_progress * 100})
 
         self._publisher.flush()
-        assert(self._manager.get_count('executed')
-               == self._manager.get_count('total'))
+        assert (self._manager.get_count('executed')
+                == self._manager.get_count('total'))
 
         MetaConfig.root.get_internal(
             "pColl").invoke_plugins(Plugin.Step.SCHED_AFTER)
 
-        log.manager.info("ORCH: Stop active runners")
+        io.console.info("ORCH: Stop active runners")
         self.stop_runners()
 
         return 0 if self._manager.get_count('total') - self._manager.get_count(Test.State.SUCCESS) == 0 else 1
 
     def start_new_runner(self):
         """Start a new Runner thread & register comm queues."""
-        Runner.sched_in_progress = True
-        r = Runner(ready=self._ready_q, complete=self._complete_q)
+        RunnerAdapter.sched_in_progress = True
+        r = RunnerAdapter(buildir=MetaConfig.root.validation.output, ready=self._ready_q, complete=self._complete_q)
         r.start()
         self._runners.append(r)
 
     def stop_runners(self):
         """Stop all previously started runners.
 
         Wait for their completion."""
         self.stop()
         for t in self._runners:
             t.join()
 
     @classmethod
     def stop(cls):
         """Request runner threads to stop."""
-        Runner.sched_in_progress = False
+        RunnerAdapter.sched_in_progress = False
 
     def run(self, session):
         """Start the orchestrator.
 
         :param session: container owning the run.
         :type session: :class:`Session`
         """
```

### Comparing `pcvs-0.6.0/pcvs/orchestration/manager.py` & `pcvs-0.7.0/pcvs/orchestration/manager.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
+from pcvs.helpers import log
 from pcvs.helpers.exceptions import OrchestratorException
 from pcvs.helpers.system import MetaConfig, MetaDict
 from pcvs.orchestration.set import Set
 from pcvs.plugins import Plugin
 from pcvs.testing.test import Test
-from pcvs.helpers import log
 
 
 class Manager:
     """Gather and manipulate Jobs under a hiararchical architecture.
 
     A Manager is in charge of carrying jobs during the scheduling. Jobs are
     divided hierarchicaly (basically, depending on the number of resource
@@ -16,32 +16,34 @@
     results.
 
     :ivar dims: hierarchical dict storing jobs
     :type dims: dict
     :ivar _max_size: max number of resources allowed by the profile
     :type _max_size: int
     :ivar _publisher: the Formatter object, publishing results into files
-    :type _publisher: :class:`Publisher`
+    :type _publisher: :class:`ResultFileManager`
     :ivar _count: dict gathering various counters (total, executed...)
     :type _count: dict 
     """
     job_hashes = dict()
+    dep_rules = dict()
 
     def __init__(self, max_size=0, builder=None, publisher=None):
         """constructor method.
 
         :param max_size: max number of resource allowed to schedule.
         :type max_size: int
         :param builder: Not used yet
         :type builder: None
         :param publisher: requested publisher by the orchestrator
-        :type publisher: :class:`Publisher`
+        :type publisher: :class:`ResultFileManager`
         """
         self._comman = MetaConfig.root.get_internal('comman')
         self._plugin = MetaConfig.root.get_internal('pColl')
+        self._concurrent_level = MetaConfig.root.machine.get('concurrent_run', 1)
 
         self._dims = dict()
         self._max_size = max_size
         self._publisher = publisher
         self._count = MetaDict({
             "total": 0,
             "executed": 0
@@ -80,20 +82,30 @@
             self._max_size = value
 
         if value not in self._dims:
             self._dims.setdefault(value, list())
 
         self._dims[value].append(job)
 
-        hashed = hash(job.name)
+        hashed = job.jid
         # if test is not know yet, add + increment
         if hashed not in self.job_hashes:
-            self.job_hashes[hash(job.name)] = job
+            self.job_hashes[hashed] = job
             self._count.total += 1
-
+            self.save_dependency_rule(job.basename, job)
+            
+    def save_dependency_rule(self, pattern, jobs):
+        assert(isinstance(pattern, str))
+        
+        if not isinstance(jobs, list):
+            jobs = [jobs]
+            
+        self.dep_rules.setdefault(pattern, list())
+        self.dep_rules[pattern] += jobs
+        
     def get_count(self, tag="total"):
         """Access to a particular counter.
 
         :param tag: a specific counter to target, defaults to "total"
         :type tag: str
         :return: a count
         :rtype: int
@@ -106,14 +118,28 @@
         This function is meant to be called once and browse every single tests
         to resolve dep names to their real associated object.
         """
         for joblist in self._dims.values():
             for job in joblist:
                 self.resolve_single_job_deps(job, list())
 
+    def print_dep_graph(self, outfile=None):
+        s = ["digraph D {"]
+        for joblist in self._dims.values():
+            for job in joblist:
+                for d in job.get_dep_graph().keys():
+                    s.append('"{}"->"{}";'.format(job.name, d))
+        s.append("}")
+        
+        if not outfile:
+            print("\n".join(s))
+        else:
+            with open(outfile, 'w') as fh:
+                fh.write("\n".join(s))
+
     def resolve_single_job_deps(self, job, chain):
         """Resolve the dependency graph for a single test.
 
         The 'chain' argument contains list of "already-seen" dependency, helping
         to detect circular deps.
 
         :raises UndefDependencyError: a depname does not have a related object
@@ -123,34 +149,67 @@
         :type job: :class:`Test`
         :param chain: list of already-seen jobs during this walkthrough
         :type chain: list
         """
         chain.append(job.name)
         for depname in job.job_depnames:
 
-            hashed_dep = hash(depname)
-            if hashed_dep not in self.job_hashes:
+            hashed_dep = Test.get_jid_from_name(depname)
+            if hashed_dep in self.job_hashes:
+                job_dep_list = [self.job_hashes[hashed_dep]]
+            elif depname in self.dep_rules:
+                job_dep_list = self.dep_rules[depname]
+            else:
                 raise OrchestratorException.UndefDependencyError(depname)
 
-            job_dep = self.job_hashes[hashed_dep]
-
-            if job_dep.name in chain:
-                raise OrchestratorException.CircularDependencyError(
-                    job_dep.name)
-            self.resolve_single_job_deps(job_dep, chain)
-            job.resolve_a_dep(depname, job_dep)
+            for job_dep in job_dep_list:
+                if job_dep.name in chain:
+                    raise OrchestratorException.CircularDependencyError(chain)
+                
+                # without copying the chain, resolution of siblings deps will alter
+                # the same list --> a single dep may appear multiple time and raise
+                # a false CiprcularDep
+                # solution: resolve subdep path in their own chain :)
+                self.resolve_single_job_deps(job_dep, list(chain))
+                job.resolve_a_dep(depname, job_dep)
 
     def get_leftjob_count(self):
         """Return the number of jobs remainig to be executed.
 
         :return: a number of jobs
         :rtype: int
         """
         return self._count.total - self._count.executed
 
+    def publish_job(self, job, publish_args=None):
+        if publish_args:
+            job.save_final_result(**publish_args)
+
+        if self._comman:
+            self._comman.send(job)
+        self._count.executed += 1
+        self._count[job.state] += 1
+        self._publisher.save(job)
+
+    def prune_non_runnable_jobs(self):
+        for k in sorted(self._dims.keys(), reverse=True):
+                if len(self._dims[k]) <= 0:
+                    continue
+                else:
+                    removed_jobs = list()
+                    for job in self._dims[k]:
+                        if job.pick_count() > Test.SCHED_MAX_ATTEMPTS:
+                            self.publish_failed_to_run_job(job, Test.MAXATTEMPTS_STR, Test.State.ERR_OTHER)
+                            removed_jobs.append(job)
+                    for elt in removed_jobs:
+                        self._dims[k].remove(elt)
+            
+
+            
+
     def create_subset(self, max_dim):
         """Extract one or more jobs, ready to be run.
 
         :param max_dim: maximum number of resource allowed by any picked job.
         :type max_dim: int
         :return: A set of jobs
         :rtype: :class:`Set`
@@ -159,108 +218,116 @@
         # for instance, gathering multiple tests, and modifying
         # the set to re-run PCVS as the task command
         if max_dim <= 0:
             return None
 
         the_set = None
         self._plugin.invoke_plugins(Plugin.Step.SCHED_SET_BEFORE)
-
+        user_sched_job = self._plugin.has_enabled_step(Plugin.Step.SCHED_JOB_EVAL)
+        
         if self._plugin.has_enabled_step(Plugin.Step.SCHED_SET_EVAL):
             the_set = self._plugin.invoke_plugins(
                 Plugin.Step.SCHED_SET_EVAL,
                 jobman=self,
-                max_dim=max_dim
+                max_dim=max_dim,
+                max_job_limit=int(self._count.total / self._concurrent_level)
             )
         else:
             for k in sorted(self._dims.keys(), reverse=True):
                 if len(self._dims[k]) <= 0 or max_dim < k:
                     continue
                 else:
                     # assert(self._builder.job_grabber)
-                    job: Test = self._dims[k].pop()
-
-                    # if there is still a job available for this dimention
+                    job: Test = self._dims[k].pop(0)
+                    publish_job_args = {}
                     if job:
-                        # but this job won't be run because:
-                        # - already run
-                        # - at least one dep run & failed
-                        if job.been_executed() or job.has_failed_dep():
-                            # jobs can be picked up outside of this pop() call
-                            # if tagged executed, they have been fully handled
-                            # and should just be removed from scheduling
-                            #
-                            # Another case: test can't be picked up because
-                            # job deps have failed.
-                            # in that case, no job management occured.
-                            # do it now.
-                            if job.has_failed_dep():
-                                job.save_final_result(rc=-1, time=0.0,
-                                                      out=Test.NOSTART_STR,
-                                                      state=Test.State.ERR_DEP)
-                                job.display()
-                                if self._comman:
-                                    self._comman.send(job)
-                                self._count.executed += 1
-                                self._count[job.state] += 1
-                                self._publisher.add(job.to_json())
-                            # sad to break, should retry
-                            break
-                        # If this job has at least one dep no executed yet
-                        # -> run it instead
+                        if job.been_executed() or job.state == Test.State.IN_PROGRESS:
+                            # skip job (only a pop() to do)
+                            continue
+
                         elif not job.has_completed_deps():
+
+                            # take the first unresolved dep to be scheduled
+                            # instead
+                            # CAUTION: no schedulable dep may be found at
+                            # present time. In the meantime, the completion may
+                            # occurs concurrently
                             self._dims[k].append(job)
+                            # pick up a dep
+                            dep_job = job.first_incomplete_dep()
+                            while dep_job and not dep_job.has_completed_deps():
+                                dep_job = dep_job.first_incomplete_dep()
+                            # no "incomplete" task has been found
+                            # this may due to a dep completion in the mean time
+                            # discard for now, wait for another process
+                            # to schedule this job
+                            if dep_job:
+                                job = dep_job
+                            else:
+                                break
 
-                            # careful: it means jobs are picked up
-                            # but not popped from
-                            while job and not job.has_completed_deps():
-                                job = job.first_incomplete_dep()
+                        # from here, it can be the original job or one of its
+                        # dep tree. But we are sure this job can be processed
 
-                    # if a job has been elected
-                    if job:
-                        # the job shouldn't be running (scenario where a dep is
-                        # popped out & run but the Set didn't complete yet)
-                        # OR th job dim exceeds remaining resources
-                        if job.state != Test.State.IN_PROGRESS and job.get_dim() <= max_dim:
+                        if job.has_failed_dep():
+                            # Cannot be scheduled for dep purposes
+                            # push it to publisher
+                            self.publish_failed_to_run_job(job, Test.NOSTART_STR, Test.State.ERR_DEP)
+                            # Attempt to find another job to schedule
+                            continue
+
+                        # Reached IF Job hasn't be run yet
+                        # Job has completed its dep scheme
+                        # all deps are successful
+                        # => SCHEDULE
+                        if user_sched_job:
+                            pick_job = self._plugin.invoke_plugins(
+                                                    Plugin.Step.SCHED_JOB_EVAL,
+                                                    job=job,
+                                                    set=the_set)
+                        else:
+                            pick_job = job.get_dim() <= max_dim
+                            
+                        if job.state != Test.State.IN_PROGRESS and pick_job:
                             job.pick()
-                            the_set = Set()
+                            if not the_set:
+                                the_set = Set(execmode=Set.ExecMode.LOCAL)
                             the_set.add(job)
                             break
                         else:
-                            # Ok, this could be rewritten...
-                            # packed with the 'same' code above ?
-                            job.not_picked()
-                            if job.pick_count() > Test.SCHED_MAX_ATTEMPTS:
-                                job.save_final_result(rc=-1, time=0.0,
-                                                      out=Test.MAXATTEMPTS_STR,
-                                                      state=Test.State.ERR_OTHER)
-                                job.display()
-                                if self._comman:
-                                    self._comman.send(job)
-                                self._count.executed += 1
-                                self._count[job.state] += 1
-                                self._publisher.add(job.to_json())
+                            if job.not_picked():
+                                self.publish_failed_to_run_job(job, Test.MAXATTEMPTS_STR, Test.State.ERR_OTHER)
                             else:
                                 self._dims[k].append(job)
-
         self._plugin.invoke_plugins(Plugin.Step.SCHED_SET_AFTER)
-
         return the_set
 
+    def publish_failed_to_run_job(self, job, out, state):
+        publish_job_args = {
+            "rc": -1,
+            "time": 0.0,
+            "out": out,
+            "state": state
+        }
+        self.publish_job(
+            job, publish_args=publish_job_args)
+        job.display()
+
     def merge_subset(self, set):
         """After completion, process the Set to publish test results.
 
         :param set: the set handling jobs during the scheduling.
         :type set: :class:`Set`
         """
         final = list()
         for job in set.content:
             if job.been_executed():
                 job.extract_metrics()
                 job.evaluate()
+                self.publish_job(job, publish_args=None)
                 job.display()
-                if self._comman:
-                    self._comman.send(job)
-                self._count.executed += 1
-                self._count[job.state] += 1
-                self._publisher.add(job.to_json())
             else:
-                self.add_job(job)
+                
+                if job.not_picked():
+                    self.publish_failed_to_run_job(job, Test.MAXATTEMPTS_STR, Test.State.ERR_OTHER)
+                else:
+                    self.add_job(job)
```

### Comparing `pcvs-0.6.0/pcvs/orchestration/set.py` & `pcvs-0.7.0/pcvs/orchestration/set.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,21 @@
+import signal
+import os
 import queue
 import subprocess
 import threading
 import time
+import enum
 from typing import List
 
+from pcvs import io
 from pcvs.helpers import communications, log
 from pcvs.helpers.system import MetaConfig
 from pcvs.testing.test import Test
-
+import json
 
 class Set:
     """Gather multiple jobs to be scheduled.
 
     Created by the manager to manipulate a subset, these jobs are removed from
     the manager during the execution, only reachable from a Set. Sets are
     launched as thread, dealing with their own workflow.
@@ -20,72 +24,105 @@
     :type _id: int
     :ivar _size: number of jobs
     :type _size: int
     :ivar _jobs: list of jobs
     :type _jobs: list
     :ivar _completed: True if all jobs have been executed
     :type _completed: bool
-    :ivar _is_wrapped: not used yet
-    :type _is_wrapped: bool
     """
     global_increment = 0
     comman: communications.GenericServer = None
 
-    def __init__(self):
+    class ExecMode(enum.IntEnum):
+        """
+        Map the current execution mode of a set.
+        - LOCAL: Sets are run by local runners. Runners are threads collocated in
+                 the same process.
+        - ALLOC: Script is provided to user-defined wrapper, intended to prepare
+                 resource for job scheduling. Runners are processed and the launch
+                 command is provided as script's arguments. The 'ALLOC' mode
+                 supposes runners are not actually running on compute resources.
+        - REMOTE: Script is provided to user-defined wrapper, intended to prepare
+                 resource for job scheduling. Runners are processed and the launch
+                 command is provided as script's arguments. The 'REMOTE' mode
+                 supposes runners *are* actually running on compute resources
+                 alongside jobs.
+        - BATCH: Script is provided to user-defined wrapper, intended to prepare
+                 resource for job scheduling. Runners are processed and the launch
+                 command is provided as script's arguments. The 'BATCH' mode
+                 supposes the user script to return before completion. An ACK
+                 method will be required to ensure Runners have properly been
+                 executed.
+        """
+        LOCAL = enum.auto()
+        ALLOC = enum.auto()
+        REMOTE = enum.auto()
+        BATCH = enum.auto()
+        
+    def __init__(self, execmode=ExecMode.LOCAL):
         """constructor method."""
         self._id = Set.global_increment
         Set.global_increment += 1
         self._size = 0
-        self._jobs: List[Test] = list()
+        self._completed: bool = False
+        self._execmode: Set.ExecMode = execmode
         self._completed = False
-        self._is_wrapped = False
-
+        self._map = dict()
+        
         if not self.comman:
             if MetaConfig.root.get_internal('comman') is not None:
                 self.comman = MetaConfig.root.get_internal('comman')
 
-    def enable_wrapping(self, wrap_cli):
-        """Make this Set manipulate multiple jobs evolving together in a
-        dedicated environment.
+    @property
+    def execmode(self) -> ExecMode:
+        """
+        Get execution mode for this Set.
+        
+        See Set.ExecMode for more information.
+        
 
-        .. warning::
-            WIP
+        :return: The current exec mode
+        :rtype: class:`Set.ExecMode`
+        """
+        return self._execmode
+    
+    @execmode.setter
+    def execmode(self, v: ExecMode):
+        """
+        Init the exec mode after the Set is created.
 
-        :param wrap_cli: noit used yet
-        :type wrap_cli: str
+        :param v: Desired Execution mode
+        :type v: class:`ExecMode`
         """
-        self._wrap_cmd = wrap_cli
-        self._is_wrapped = True
+        self._execmode = v
 
     def add(self, l):
         """Add a job or a list of jobs to the current Set.
 
         :param l: a single or a list of jobs
         :type l: :class:`Test` or List[:class:`Test`]
         """
         if not isinstance(l, list):
             l = [l]
-        self._jobs += l
-        self._size = len(self._jobs)
+        for j in l:
+            self._map[j.jid] = j
+        self._size = len(self._map.keys())
+
+    def find(self, job_hash):
+        if job_hash not in self._map:
+            return None
+        return self._map[job_hash]
 
     def is_empty(self):
         """check is the set is empty (contains no jobs)
 
         :return: True if there is no jobs
         :rtype: bool
         """
-        return len(self._jobs) == 0
-
-    def been_completed(self):
-        """check is the Set is complete and can be flushed down to the manager.
-
-        :return: True if all jobs have been completed.
-        :rtype: bool
-        """
-        return self._completed
+        return self._size <= 0
 
     @property
     def size(self):
         """Getter to size property.
 
         :return: Set size
         :rtype: int
@@ -106,82 +143,28 @@
         """Getter to dim property (largest dimension of a single job)
 
         :return: Set dim
         :rtype: int
         """
         if self._size <= 0:
             return 0
-        elif self._size == 1:
-
-            return self._jobs[0].get_dim()
         else:
-            return max(self._jobs, key=lambda x: x.get_dim())
+            return max(map(lambda x: x.get_dim(), self._map.values()))
 
     @property
     def content(self):
         """Generator iterating over the job list."""
-        for j in self._jobs:
+        for j in self._map.values():
             yield j
 
-    def is_complete(self):
-        self._completed = True
-
-
-class Runner(threading.Thread):
-
-    sched_in_progress = True
+    @property
+    def completed(self) -> bool:
+        """check is the Set is complete and can be flushed down to the manager.
 
-    def __init__(self, ready, complete):
-        super().__init__()
-
-        self._rq = ready
-        self._cq = complete
-
-    def run(self):
-        log.manager.debug('{}: Set start'.format(self.ident))
-        while True:
-            try:
-                if self.sched_in_progress:
-                    item = self._rq.get(block=False, timeout=5)
-                    self.process_item(item)
-                    self._cq.put(item)
-                else:
-                    break
-            except queue.Empty:
-                continue
-            except Exception as e:
-                raise e
-
-    def process_item(self, set):
-        """Execute the Set and jobs within it.
-
-        :raises Exception: Something occured while running a test"""
-        for job in set.content:
-            try:
-                p = subprocess.Popen('{}'.format(job.invocation_command),
-                                     shell=True,
-                                     stderr=subprocess.STDOUT,
-                                     stdout=subprocess.PIPE)
-                start = time.time()
-                stdout, _ = p.communicate(timeout=job.timeout)
-                final = time.time() - start
-
-                # Note: The return code here is coming from the script,
-                # not the test itself. It is transitively transmitted once the
-                # test complete, except if test used matchers to validate.
-                # in that case, a non-zero exit code indicates at least one
-                # matcher failed.
-                # The the engine, no other checks than return code evaluation
-                # is necessary to assess test status.
-                rc = p.returncode
-
-            except subprocess.TimeoutExpired:
-                p.kill()
-                final = job.timeout
-                stdout, _ = p.communicate()
-                rc = Test.Timeout_RC  # nah, to be changed
-            except Exception:
-                raise
-            job.save_raw_run(time=final, rc=rc, out=stdout)
-            job.save_status(Test.State.EXECUTED)
+        :return: True if all jobs have been completed.
+        :rtype: bool
+        """
+        return self._completed
 
-        set.is_complete()
+    @completed.setter
+    def completed(self, b: bool) -> None:
+        self._completed = b
```

### Comparing `pcvs-0.6.0/pcvs/plugins/__init__.py` & `pcvs-0.7.0/pcvs/plugins/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import importlib
 import inspect
 import os
 import pkgutil
 import sys
 from abc import abstractmethod
 
-from pcvs.helpers import log
+from pcvs import io
 from pcvs.helpers.exceptions import PluginException
 
 
 class Plugin:
     """Base class to inherit from when implementing a plugin.
 
     This class should be used by any defined plugin and:
@@ -24,35 +24,34 @@
     """
     class Step(enum.Enum):
         """Possible pass a plugin can be loaded into.
 
         ``*_EVAL`` steps describe plugin passes where the function outcome can
         infer with the actual workflow.
         """
-        INVALID = -1,
-
-        START_BEFORE = enum.auto(),
-        START_AFTER = enum.auto(),
-        TFILE_BEFORE = enum.auto(),
-        TDESC_BEFORE = enum.auto(),
-        TEST_EVAL = enum.auto(),
-        TDESC_AFTER = enum.auto(),
-        TFILE_AFTER = enum.auto(),
-        SCHED_BEFORE = enum.auto(),
-        SCHED_SET_BEFORE = enum.auto(),
-        SCHED_SET_EVAL = enum.auto(),
-        SCHED_SET_AFTER = enum.auto(),
-        TEST_RESULT_EVAL = enum.auto(),
-        SCHED_PUBLISH_BEFORE = enum.auto(),
-        SCHED_PUBLISH_WRITE = enum.auto(),
-        SCHED_PUBLISH_AFTER = enum.auto(),
-        SCHED_AFTER = enum.auto(),
-        END_BEFORE = enum.auto(),
+        INVALID = -1
+        START_BEFORE = enum.auto()
+        START_AFTER = enum.auto()
+        TFILE_BEFORE = enum.auto()
+        TDESC_BEFORE = enum.auto()
+        TEST_EVAL = enum.auto()
+        TDESC_AFTER = enum.auto()
+        TFILE_AFTER = enum.auto()
+        SCHED_BEFORE = enum.auto()
+        SCHED_SET_BEFORE = enum.auto()
+        SCHED_SET_EVAL = enum.auto()
+        SCHED_JOB_EVAL = enum.auto()
+        SCHED_SET_AFTER = enum.auto()
+        TEST_RESULT_EVAL = enum.auto()
+        SCHED_PUBLISH_BEFORE = enum.auto()
+        SCHED_PUBLISH_WRITE = enum.auto()
+        SCHED_PUBLISH_AFTER = enum.auto()
+        SCHED_AFTER = enum.auto()
+        END_BEFORE = enum.auto()
         END_AFTER = enum.auto()
-        
 
         def __str__(self):
             """Stringify a Step as a printable string
 
             :return: a printable string according to the step
             :rtype: str
             """
@@ -81,38 +80,39 @@
         """constructor method"""
         self._plugins = {name: [] for name in list(Plugin.Step)}
         self._enabled = {name: None for name in list(Plugin.Step)}
 
     def register_default_plugins(self):
         """Detect plugins stored in default places."""
         try:
-            self.register_plugin_by_package("pcvs.plugins.default", activate=True)
-                
-            self.register_plugin_by_package('pcvs-contrib')
-            
+            self.register_plugin_by_package(
+                "pcvs.plugins.default", activate=True)
+
+            self.register_plugin_by_package('contrib')
+
         except:
-            log.manager.info(
-                "No pcvs-contrib package found for plugin autoloading")
+            io.console.info(
+                "No 'contrib' package found for plugin autoloading")
 
     def activate_plugin(self, name):
         """Flag a plugin as active, meaning it will be called when the pass is
         reached.
 
         :param name: the plugin name.
         :type name: str"""
         for step, plugins in self._plugins.items():
             for p in plugins:
                 if name.lower() == type(p).__name__.lower():
-                    log.manager.debug("Activate {}".format(name))
+                    io.console.debug("Activate {}".format(name))
                     if self._enabled[p.step]:
-                        log.manager.debug(
+                        io.console.debug(
                             " -> overrides {}".format(self._enabled[p.step]))
                     self._enabled[p.step] = p
                     return
-        log.manager.warn("Unable to find a plugin named '{}'".format(name))
+        io.console.warn("Unable to find a plugin named '{}'".format(name))
 
     def invoke_plugins(self, step, *args, **kwargs):
         """Load the appropriate plugin, given a step
 
         :param step: the step to target
         :type step: :class:`Plugin.Step`
         :raises PluginException.BadStepError: wrong Step value
@@ -152,39 +152,39 @@
             return False
         return self._enabled[step] is not None
 
     def show_plugins(self):
         """Display plugin context to stdout."""
         for step, elements in self._plugins.items():
             if len(elements) > 0:
-                log.manager.print_section("Step {}:".format(str(step)))
+                io.console.print_section("Step {}:".format(str(step)))
                 for e in elements:
-                    log.manager.print_item("{}".format(type(e).__name__))
+                    io.console.print_item("{}".format(type(e).__name__))
 
     def show_enabled_plugins(self):
         """Display the list of loaded plugins."""
         empty = True
         for step, e in self._enabled.items():
             if e:
                 empty = False
-                log.manager.print_item(
+                io.console.print_item(
                     "{}: {}".format(str(step), type(e).__name__))
 
         if empty:
-            log.manager.print_item("None")
+            io.console.print_item("None")
 
     def register_plugin_by_file(self, modpath, activate=False):
         """Based on a filepath (as a module dir), load plugins contained in it.
 
         :param modpath: valid python filepath
         :type modpath: str
         """
 
         # the content is added to "pcvs-contrib" module
-        spec = importlib.util.spec_from_file_location("pcvs-contrib",
+        spec = importlib.util.spec_from_file_location("contrib",
                                                       modpath)
         mod = importlib.util.module_from_spec(spec)
         spec.loader.exec_module(mod)
         self.register_plugin_by_module(mod, activate)
 
     def register_plugin_by_module(self, mod, activate=False):
         """Based on a module name, load any defined plugin.
@@ -194,15 +194,15 @@
         :param mod: module name
         :type mod: str
         """
         for (_, the_class) in inspect.getmembers(mod, inspect.isclass):
             if issubclass(the_class, Plugin) and the_class is not Plugin:
                 step_str = str(the_class.step)
                 class_name = the_class.__name__
-                log.manager.debug(
+                io.console.debug(
                     "Register {} ({})".format(class_name, step_str))
                 self._plugins[the_class.step].append(the_class())
                 if activate:
                     self.activate_plugin(class_name)
 
     def register_plugin_by_dir(self, pkgpath, activate=False):
         """From a prefix directory, load any plugin defined in it.
@@ -224,14 +224,13 @@
         """Based on a package name, load any plugin defined into it.
 
         :param pkgname: package name, valid under current PYTHON env.
         :type pkgname: str
         :raises PluginException.LoadError: Error while importing the package
         """
         mod = importlib.import_module(pkgname)
-
         for _, name, _ in pkgutil.iter_modules(mod.__path__, mod.__name__ + "."):
             try:
                 submod = importlib.import_module(name)
                 self.register_plugin_by_module(submod, activate)
             except Exception as e:
                 raise PluginException.LoadError(name)
```

### Comparing `pcvs-0.6.0/pcvs/plugins/default/validation.py` & `pcvs-0.7.0/pcvs/plugins/default/validation.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,64 +1,64 @@
-from pcvs.testing.test import Test
-from pcvs.plugins import Plugin
-from pcvs.helpers.system import MetaConfig
 from pcvs.backend import bank
+from pcvs.helpers.system import MetaConfig
+from pcvs.plugins import Plugin
+from pcvs.testing.test import Test
+
 
 class BankValidationPlugin(Plugin):
     """TODO:
     """
     step = Plugin.Step.TEST_RESULT_EVAL
-    
+
     def __init__(self):
         super().__init__()
         self._bank_hdl = None
-        
-    
+
     def run(self, *args, **kwargs):
         """TODO:
         """
         if not self._bank_hdl:
             bankname = MetaConfig.root.validation.get('target_bank', None)
             if not bankname:
                 return None
-        
+
             self._bank_hdl = bank.Bank(path=None, token=bankname)
             self._bank_hdl.connect()
-            self._bank_hdl.load_config_from_dict(MetaConfig.root)
-        self._serie = self._bank_hdl.get_serie(self._bank_hdl.build_target_branch_name())
+        self._serie = self._bank_hdl.get_serie(
+            self._bank_hdl.build_target_branch_name(hash=MetaConfig.root.validation.pf_hash))
         if not self._serie:
             # no history, stop !
             return None
-            
+
         node = kwargs.get('analysis', {})
         job = kwargs.get('job', None)
-        
+
         method = node.get('method', None)
         args = node.get('args', {})
         if method and hasattr(self, method):
             func = getattr(self, method)
             return func(args, job)
         return None
-        
+
     def not_longer_than_previous_runs(self, args, job):
         """TODO:
         """
         if not self._bank_hdl:
             return Test.State.ERR_OTHER
-        
+
         max_runs = args.get('history_depth', 1)
         tolerance = args.get('tolerance', 0)
         sum = 0
         cnt = 0
         run = self._serie.last
         while cnt < max_runs:
             res = run.get_data(job.name)
             if res and res.state == Test.State.SUCCESS:
-                    sum += res.time
-                    cnt+= 1
+                sum += res.time
+                cnt += 1
             run = run.previous
             if run is None:
                 break
         if cnt >= 0 and job.time >= (sum / cnt) * (1 + tolerance/100):
             return Test.State.FAILURE
         else:
             return Test.State.SUCCESS
```

### Comparing `pcvs-0.6.0/pcvs/schemes/compiler-scheme.yml` & `pcvs-0.7.0/pcvs/schemes/runtime-scheme.yml`

 * *Files 17% similar despite different names*

```diff
@@ -1,32 +1,42 @@
 ---
 type: object
 properties:
-  commands:
-    type: object
-    properties:
-      cc:
-        type: string
-      cxx:
-        type: string
-      fc:
-        type: string
-      f77:
-        type: string
-      f90:
-        type: string
-    additionalProperties: false
-  variants:
+  program:
+    type: string
+  args:
+    type: string
+  plugin:
+    media:
+      binaryEncoding: base64
+  criterions:
     type: object
     patternProperties:
       "^.*$":
         type: object
         properties:
-          args:
+          option:
+            type: string
+          numeric:
+            type: boolean
+          type:
+            type: string
+            enum:
+              - argument
+              - environment
+          position:
             type: string
+            enum:
+              - before
+              - after
+          aliases:
+            patternProperties:
+              "^.*$":
+                type: string
+        additionalProperties: false
     additionalProperties: false
   package_manager:
     type: object
     properties:
       spack:
         type: array
         items:
```

### Comparing `pcvs-0.6.0/pcvs/schemes/group-scheme.yml` & `pcvs-0.7.0/pcvs/schemes/group-scheme.yml`

 * *Files identical despite different names*

### Comparing `pcvs-0.6.0/pcvs/schemes/machine-scheme.yml` & `pcvs-0.7.0/pcvs/schemes/machine-scheme.yml`

 * *Files 22% similar despite different names*

```diff
@@ -24,26 +24,20 @@
             allocate: &alloc_node
               type: object
               properties:
                 program: {"type": "string"}
                 args: {"type": "string"}
                 wrapper: {"type": "string"}
               additionalProperties: false
-            run:
+            remote:
               <<: *alloc_node
             batch:
               <<: *alloc_node
           additionalProperties: false
       additionalProperties: false
 
   <<: *raw_properties
   default_partition:
-    type: string
-  package_manager:
-    type: object
-    properties:
-      spack:
-        type: string
-      module:
-        type: string
-    additionalProperties: false
+    OneOf:
+    - {type: string}
+    - {type: null}
 additionalProperties: false
```

### Comparing `pcvs-0.6.0/pcvs/schemes/settings-scheme.yml` & `pcvs-0.7.0/pcvs/schemes/settings-scheme.yml`

 * *Files identical despite different names*

### Comparing `pcvs-0.6.0/pcvs/schemes/test-result-scheme.yml` & `pcvs-0.7.0/pcvs/schemes/test-result-scheme.yml`

 * *Files 26% similar despite different names*

```diff
@@ -4,14 +4,15 @@
   id:
     type: object
     properties:
       label: {"type": "string"}
       subtree: {"OneOf": [{"type": "string"}, {"type": null}]}
       te_name: {"type": "string"}
       fq_name: {"type": "string"}
+      jid: {"type": "string"}
       comb:
         OneOf:
           - type: null
           - type: object
             patternProperties:
               "^.*$": {type: "string"}
     additionalProperties: false
@@ -19,15 +20,25 @@
   exec: {"type": "string"}
   result:
     type: object
     properties:
       rc: {"type": "integer"}
       state: {"type": "integer"}
       time: {"type": "number"}
-      output: {"OneOf": [{"type": "string"}, {"type": null}]}
+      output:
+        type: object
+        properties:
+          file:
+            OneOf:
+            - {"type": "string"}
+            - {"type": null}
+          offset: {"type": "integer"}
+          length: {"type": "integer"}
+          raw: {"type": "string"}
+        additionalProperties: false
     additionalProperties: false
     required: ['rc', 'state', 'time']
   data:
     type: object
     properties:
       tags:
         OneOf:
```

### Comparing `pcvs-0.6.0/pcvs/templates/config/criterion.default.yml` & `pcvs-0.7.0/pcvs/templates/config/criterion.default.yml`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 ---
 # Defines criterion values to be used during the validation
 # Iterators are only valid if they have been declared
 # previously by the runtime
-iterators:
-  # a criterion name
-  n_node:
-    # the range of values it can take (any type)
-    values: [1] 
-    # the prefix to use when labelling test name for this IT
-    subtitle: "N"
-  n_mpi:
-    values: [1, 2, 4]
-    subtitle: "n"
-  n_omp:
-    values: [2, 4]
-    subtitle: "o"
+# a criterion name
+n_node:
+  # the range of values it can take (any type)
+  values: [1] 
+  # the prefix to use when labelling test name for this IT
+  subtitle: "N"
+n_mpi:
+  values: [1, 2, 4]
+  subtitle: "n"
+n_omp:
+  values: [2, 4]
+  subtitle: "o"
 
 # As a combinatorial scheme, the desc above will generate the following
 # 16 test combinations (for each program defined):
 # (node:1, mpi:2, omp:4, core:1)
 # (node:1, mpi:2, omp:4, core:2)
 # (node:1, mpi:2, omp:8, core:1)
 # (node:1, mpi:2, omp:8, core:2)
```

### Comparing `pcvs-0.6.0/pcvs/templates/config/criterion.large.yml` & `pcvs-0.7.0/pcvs/templates/config/criterion.large.yml`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 ---
 # Defines criterion values to be used during the validation
 # Iterators are only valid if they have been declared
 # previously by the runtime
-iterators:
-  # a criterion name
-  n_node:
-    # the range of values it can take (any type)
-    values: [1, 2, 3, 4]
-    # the prefix to use when labelling test name for this IT
-    subtitle: "N"
-  n_mpi:
-    values: [2, 4, 8, 16, 32]
-    subtitle: "n"
-  n_omp:
-    values: [1, 2, 4, 8]
-    subtitle: "o"
-  n_core:
-    values: [1, 2, 4, 8]
-    subtitle: "c"
-  net:
-    values: ['tcp', 'shmem', 'ib']
-    subtitle: ''
+# a criterion name
+n_node:
+  # the range of values it can take (any type)
+  values: [1, 2, 3, 4]
+  # the prefix to use when labelling test name for this IT
+  subtitle: "N"
+n_mpi:
+  values: [2, 4, 8, 16, 32]
+  subtitle: "n"
+n_omp:
+  values: [1, 2, 4, 8]
+  subtitle: "o"
+n_core:
+  values: [1, 2, 4, 8]
+  subtitle: "c"
+net:
+  values: ['tcp', 'shmem', 'ib']
+  subtitle: ''
 
 # As a combinatorial scheme, the desc above will generate the following
 # 16 test combinations (for each program defined):
 # (node:1, mpi:2, omp:4, core:1)
 # (node:1, mpi:2, omp:4, core:2)
 # (node:1, mpi:2, omp:8, core:1)
 # (node:1, mpi:2, omp:8, core:2)
```

### Comparing `pcvs-0.6.0/pcvs/templates/config/criterion.small.yml` & `pcvs-0.7.0/pcvs/templates/config/criterion.small.yml`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 ---
 # Defines criterion values to be used during the validation
 # Iterators are only valid if they have been declared
 # previously by the runtime
-iterators:
-  # a criterion name
-  n_node:
-    # the range of values it can take (any type)
-    values: [1] 
-    # the prefix to use when labelling test name for this IT
-    subtitle: "N"
-  n_mpi:
-    values: [1, 2, 4]
-    subtitle: "n"
-  n_omp:
-    values: [2, 4]
-    subtitle: "o"
+# a criterion name
+n_node:
+  # the range of values it can take (any type)
+  values: [1] 
+  # the prefix to use when labelling test name for this IT
+  subtitle: "N"
+n_mpi:
+  values: [1, 2, 4]
+  subtitle: "n"
+n_omp:
+  values: [2, 4]
+  subtitle: "o"
 
 # As a combinatorial scheme, the desc above will generate the following
 # 16 test combinations (for each program defined):
 # (node:1, mpi:2, omp:4, core:1)
 # (node:1, mpi:2, omp:4, core:2)
 # (node:1, mpi:2, omp:8, core:1)
 # (node:1, mpi:2, omp:8, core:2)
```

### Comparing `pcvs-0.6.0/pcvs/templates/config/machine.slurm.yml` & `pcvs-0.7.0/pcvs/templates/config/machine.slurm.yml`

 * *Files 16% similar despite different names*

```diff
@@ -21,15 +21,19 @@
   # resource allocation properties (jobs won't spawn by themself on a 
   # remote node. Useful when batch managers is part of the test launching sequence
   allocate:
     program: "echo"
     args: ""
     wrapper: ""
   # Resource alloc & exec properties. Jobs will be spawned on remote nodes).
-  run:
+  remote:
+    program: "echo"
+    args: ""
+    wrapper: ""
+  batch:
     program: "echo"
     args: ""
     wrapper: ""
 # default partition to load (None by default). If specified, a partition will be
 # loaded and will override configuration above
 default_partition: null
 # defines partitions overring settings above
```

### Comparing `pcvs-0.6.0/pcvs/templates/config/runtime.default.yml` & `pcvs-0.7.0/pcvs/templates/config/runtime.default.yml`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # For instance, an MPI program has the following components:
 # - number of nodes to be executed on
 # - number of MPI ranks
 # - number of cores allocated for each MPI rank
 # - Type of network to enable inter process communication
 # A single test is a combination of one single value picked up from
 # these components.
-iterators:
+criterions:
     # please use a short, without-space names
     n_mpi:
         # option known by the runtime to handle a value of this component
         option: "-np "
         # Is the sequence of values only number ?
         numeric: true
         # two cases:
```

### Comparing `pcvs-0.6.0/pcvs/templates/config/runtime.mpi.yml` & `pcvs-0.7.0/pcvs/templates/config/runtime.mpi.yml`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # For instance, an MPI program has the following components:
 # - number of nodes to be executed on
 # - number of MPI ranks
 # - number of cores allocated for each MPI rank
 # - Type of network to enable inter process communication
 # A single test is a combination of one single value picked up from
 # these components.
-iterators:
+criterions:
     # please use a short, without-space names
     n_mpi:
         # option known by the runtime to handle a value of this component
         option: "-np "
         # Is the sequence of values only number ?
         numeric: true
         # two cases:
```

### Comparing `pcvs-0.6.0/pcvs/templates/config/runtime.void.yml` & `pcvs-0.7.0/pcvs/templates/config/runtime.void.yml`

 * *Files 20% similar despite different names*

```diff
@@ -8,12 +8,11 @@
 # For instance, an MPI program has the following components:
 # - number of nodes to be executed on
 # - number of MPI ranks
 # - number of cores allocated for each MPI rank
 # - Type of network to enable inter process communication
 # A single test is a combination of one single value picked up from
 # these components.
-iterators:
-        void:
-                option: ''
-                values: []
+criterions:
+    void:
+        option: ''
```

### Comparing `pcvs-0.6.0/pcvs/templates/profile/default.yml` & `pcvs-0.7.0/pcvs/templates/profile/default.yml`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 compiler:
-  commands: {cc: mpicc, cxx: mpicxx, f77: mpif77, f90: mpif90, fc: mpif90}
+  cc: {program: mpicc}
+  cxx: {program: mpicxx}
+  f77: {program: mpif77}
+  f90: {program: mpif90}
+  fc: {program: mpif90}
 criterion:
-  iterators:
     n_mpi:
       subtitle: n
       values: [1, 2, 3, 4]
 group:
   GRPMPI:
     run:
       iterate:
         n_omp: {values: null}
 machine: {concurrent_run: 4, cores_per_node: 4, name: localhost, nodes: 1}
 runtime:
-  iterators:
+  criterions:
     n_mpi: {numeric: true, option: '-np '}
   plugin: !!binary |
     YVcxd2IzSjBJRzFoZEdnS1puSnZiU0J3WTNaekxuQnNkV2RwYm5NZ2FXMXdiM0owSUZCc2RXZHBi
     Z29LWTJ4aGMzTWdUVkJKVUd4MVoybHVLRkJzZFdkcGJpazZDaUFnSUNCemRHVndJRDBnVUd4MVoy
     bHVMbE4wWlhBdVZFVlRWRjlGVmtGTUNpQWdJQ0FLSUNBZ0lHUmxaaUJ5ZFc0b2MyVnNaaXdnS21G
     eVozTXNJQ29xYTNkaGNtZHpLVG9LSUNBZ0lDQWdJQ0FqSUhKbGRIVnlibk1nVkhKMVpTQnBaaUIw
     YUdVZ1kyOXRZbWx1WVhScGIyNGdjMmh2ZFd4a0lHSmxJSFZ6WldRS0lDQWdJQ0FnSUNCamIyNW1h
```

### Comparing `pcvs-0.6.0/pcvs/templates/profile/mpi-omp.yml` & `pcvs-0.7.0/pcvs/templates/profile/mpi-omp.yml`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 compiler:
-  commands: {cc: mpicc, cxx: mpicxx, f77: mpif77, f90: mpif90, fc: mpif90}
-  variants:
-    openmp: {args: -fopenmp}
+  cc: {program: "mpicc", variants: &var {openmp: {args: ['-fopenmp']}}}
+  cxx: {program: mpicxx, variants: *var}
+  f77: {program: mpif77, variants: *var}
+  f90: {program: mpif90, variants: *var}
+  fc: {program: mpif90, variants: *var}
 criterion:
-  iterators:
-    n_mpi:
-      subtitle: n
-      values: [2, 8]
-    n_omp:
-      subtitle: o
-      values: [2, 4]
+  n_mpi:
+    subtitle: n
+    values: [2, 8]
+  n_omp:
+    subtitle: o
+    values: [2, 4]
 group:
   GRPMPI:
     run:
       iterate:
         n_omp: {values: null}
   GRPOMP:
     run:
@@ -26,15 +27,15 @@
       iterate:
         n_core: {values: null}
         n_mpi: {values: null}
         n_node: {values: null}
         n_omp: {values: null}
 machine: {concurrent_run: 4, cores_per_node: 4, name: localhost, nodes: 1}
 runtime:
-  iterators:
+  criterions:
     n_mpi: {numeric: true, option: '-np '}
     n_omp: {numeric: true, option: OMP_NUM_THREADS=, type: environment}
   plugin: !!binary |
     YVcxd2IzSjBJRzFoZEdnS1puSnZiU0J3WTNaekxuQnNkV2RwYm5NZ2FXMXdiM0owSUZCc2RXZHBi
     Z29LWTJ4aGMzTWdUVkJKVUd4MVoybHVLRkJzZFdkcGJpazZDaUFnSUNCemRHVndJRDBnVUd4MVoy
     bHVMbE4wWlhBdVZFVlRWRjlGVmtGTUNpQWdJQ0FLSUNBZ0lHUmxaaUJ5ZFc0b2MyVnNaaXdnS21G
     eVozTXNJQ29xYTNkaGNtZHpLVG9LSUNBZ0lDQWdJQ0FqSUhKbGRIVnlibk1nVkhKMVpTQnBaaUIw
```

### Comparing `pcvs-0.6.0/pcvs/templates/profile/mpi-slurm.yml` & `pcvs-0.7.0/pcvs/templates/profile/mpi.yml`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 compiler:
-  commands: {cc: mpicc, cxx: mpicxx, f77: mpif77, f90: mpif90, fc: mpif90}
+  cc: {program: mpicc}
+  cxx: {program: mpicxx}
+  f77: {program: mpif77}
+  f90: {program: mpif90}
+  fc: {program: mpif90}
 criterion:
-  iterators:
-    n_node:
-        subtitle: N
-        values: [1, 2, 3, 4]
     n_mpi:
       subtitle: n
       values: [1, 2, 3, 4]
-    n_core:
-      subtitle: c
-      values: [1, 2, 5, 8]
+group:
+  GRPMPI:
+    run:
+      iterate:
+        n_omp: {values: null}
 machine: {concurrent_run: 4, cores_per_node: 4, name: localhost, nodes: 1}
 runtime:
-  iterators:
-    n_core: {numeric: true, option: '-c '}
-    n_node: {numeric: true, option: 'N '}
-    n_mpi: {numeric: true, option: '-n '}
+  criterions:
+    n_mpi: {numeric: true, option: '-np '}
   plugin: !!binary |
     YVcxd2IzSjBJRzFoZEdnS1puSnZiU0J3WTNaekxuQnNkV2RwYm5NZ2FXMXdiM0owSUZCc2RXZHBi
     Z29LWTJ4aGMzTWdUVkJKVUd4MVoybHVLRkJzZFdkcGJpazZDaUFnSUNCemRHVndJRDBnVUd4MVoy
     bHVMbE4wWlhBdVZFVlRWRjlGVmtGTUNpQWdJQ0FLSUNBZ0lHUmxaaUJ5ZFc0b2MyVnNaaXdnS21G
     eVozTXNJQ29xYTNkaGNtZHpLVG9LSUNBZ0lDQWdJQ0FqSUhKbGRIVnlibk1nVkhKMVpTQnBaaUIw
     YUdVZ1kyOXRZbWx1WVhScGIyNGdjMmh2ZFd4a0lHSmxJSFZ6WldRS0lDQWdJQ0FnSUNCamIyNW1h
     V2NnUFNCcmQyRnlaM05iSjJOdmJtWnBaeWRkQ2lBZ0lDQWdJQ0FnYm1KZmJtOWtaWE1nUFNCamIy
@@ -30,8 +30,8 @@
     Q0FnSUNBZ2JsOXRjR2tnUFNCamIyMWlMbWRsZENnbmJsOXRjR2tuTENBeEtRb2dJQ0FnSUNBZ0lH
     NWZiMjF3SUQwZ1kyOXRZaTVuWlhRb0oyNWZiMjF3Snl3Z01Da0tJQ0FnSUNBZ0lDQnVYMjV2WkdV
     Z1BTQmpiMjFpTG1kbGRDZ25ibDl1YjJSbEp5d2dNU2tLQ2lBZ0lDQWdJQ0FnYVdZZ1hBb2dJQ0Fn
     SUNBZ0lDQWdJQ0FvYVc1MEtHNWZiWEJwSUM4Z2JsOXViMlJsS1NBK0lHNWlYMk52Y21WektTQnZj
     aUJjQ2lBZ0lDQWdJQ0FnSUNBZ0lDaHVYMjV2WkdVZ1BpQnVZbDl1YjJSbGN5azZDaUFnSUNBZ0lD
     QWdJQ0FnSUNBZ0lDQnlaWFIxY200Z1JtRnNjMlVLSUNBZ0lDQWdJQ0JsYkhObE9nb2dJQ0FnSUNB
     Z0lDQWdJQ0J5WlhSMWNtNGdWSEoxWlFvPQ==
-  program: srun
+  program: mpirun
```

### Comparing `pcvs-0.6.0/pcvs/templates/profile/mpi.yml` & `pcvs-0.7.0/pcvs/templates/profile/mpi-slurm.yml`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 compiler:
-  commands: {cc: mpicc, cxx: mpicxx, f77: mpif77, f90: mpif90, fc: mpif90}
+  cc: {program: mpicc}
+  cxx: {program: mpicxx}
+  f77: {program: mpif77}
+  f90: {program: mpif90}
+  fc: {program: mpif90}
 criterion:
-  iterators:
-    n_mpi:
-      subtitle: n
+  n_node:
+      subtitle: N
       values: [1, 2, 3, 4]
-group:
-  GRPMPI:
-    run:
-      iterate:
-        n_omp: {values: null}
+  n_mpi:
+    subtitle: n
+    values: [1, 2, 3, 4]
+  n_core:
+    subtitle: c
+    values: [1, 2, 5, 8]
 machine: {concurrent_run: 4, cores_per_node: 4, name: localhost, nodes: 1}
 runtime:
-  iterators:
-    n_mpi: {numeric: true, option: '-np '}
+  criterions:
+    n_core: {numeric: true, option: '-c '}
+    n_node: {numeric: true, option: 'N '}
+    n_mpi: {numeric: true, option: '-n '}
   plugin: !!binary |
     YVcxd2IzSjBJRzFoZEdnS1puSnZiU0J3WTNaekxuQnNkV2RwYm5NZ2FXMXdiM0owSUZCc2RXZHBi
     Z29LWTJ4aGMzTWdUVkJKVUd4MVoybHVLRkJzZFdkcGJpazZDaUFnSUNCemRHVndJRDBnVUd4MVoy
     bHVMbE4wWlhBdVZFVlRWRjlGVmtGTUNpQWdJQ0FLSUNBZ0lHUmxaaUJ5ZFc0b2MyVnNaaXdnS21G
     eVozTXNJQ29xYTNkaGNtZHpLVG9LSUNBZ0lDQWdJQ0FqSUhKbGRIVnlibk1nVkhKMVpTQnBaaUIw
     YUdVZ1kyOXRZbWx1WVhScGIyNGdjMmh2ZFd4a0lHSmxJSFZ6WldRS0lDQWdJQ0FnSUNCamIyNW1h
     V2NnUFNCcmQyRnlaM05iSjJOdmJtWnBaeWRkQ2lBZ0lDQWdJQ0FnYm1KZmJtOWtaWE1nUFNCamIy
@@ -27,8 +33,8 @@
     Q0FnSUNBZ2JsOXRjR2tnUFNCamIyMWlMbWRsZENnbmJsOXRjR2tuTENBeEtRb2dJQ0FnSUNBZ0lH
     NWZiMjF3SUQwZ1kyOXRZaTVuWlhRb0oyNWZiMjF3Snl3Z01Da0tJQ0FnSUNBZ0lDQnVYMjV2WkdV
     Z1BTQmpiMjFpTG1kbGRDZ25ibDl1YjJSbEp5d2dNU2tLQ2lBZ0lDQWdJQ0FnYVdZZ1hBb2dJQ0Fn
     SUNBZ0lDQWdJQ0FvYVc1MEtHNWZiWEJwSUM4Z2JsOXViMlJsS1NBK0lHNWlYMk52Y21WektTQnZj
     aUJjQ2lBZ0lDQWdJQ0FnSUNBZ0lDaHVYMjV2WkdVZ1BpQnVZbDl1YjJSbGN5azZDaUFnSUNBZ0lD
     QWdJQ0FnSUNBZ0lDQnlaWFIxY200Z1JtRnNjMlVLSUNBZ0lDQWdJQ0JsYkhObE9nb2dJQ0FnSUNB
     Z0lDQWdJQ0J5WlhSMWNtNGdWSEoxWlFvPQ==
-  program: mpirun
+  program: srun
```

### Comparing `pcvs-0.6.0/pcvs/templates/profile/omp.yml` & `pcvs-0.7.0/pcvs/templates/profile/omp.yml`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 compiler:
-  commands: {cc: gcc, cxx: g++, f77: gfortran, f90: gfortran, fc: gfortran}
+  cc: {program: gcc}
+  cxx: {program: g++}
+  f77: {program: gfortran}
+  f90: {program: gfortran}
+  f08: {program: gfortran}
+  fc: {program: gfortran}
 criterion:
-  iterators:
-    n_omp:
-      subtitle: o
-      values: [1, 2, 4, 8]
+  n_omp:
+    subtitle: o
+    values: [1, 2, 4, 8]
 group:
   GRPMPI:
     run:
       iterate:
         n_omp: {values: null}
 machine: {concurrent_run: 4, cores_per_node: 4, name: localhost, nodes: 1}
 runtime:
-  iterators:
+  criterions:
     n_omp: {numeric: true, option: OMP_NUM_THREADS=, type: environment}
   plugin: !!binary |
     YVcxd2IzSjBJRzFoZEdnS1puSnZiU0J3WTNaekxuQnNkV2RwYm5NZ2FXMXdiM0owSUZCc2RXZHBi
     Z29LWTJ4aGMzTWdUM0JsYmsxUVVHeDFaMmx1S0ZCc2RXZHBiaWs2Q2lBZ0lDQnpkR1Z3SUQwZ1VH
     eDFaMmx1TGxOMFpYQXVWRVZUVkY5RlZrRk1DaUFnSUNBS0lDQWdJR1JsWmlCeWRXNG9jMlZzWml3
     Z0ttRnlaM01zSUNvcWEzZGhjbWR6S1RvS0lDQWdJQ0FnSUNBaklISmxkSFZ5Ym5NZ1ZISjFaU0Jw
     WmlCMGFHVWdZMjl0WW1sdVlYUnBiMjRnYzJodmRXeGtJR0psSUhWelpXUUtJQ0FnSUNBZ0lDQmpi
```

### Comparing `pcvs-0.6.0/pcvs/testing/__init__.py` & `pcvs-0.7.0/pcvs/testing/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
-from pcvs.helpers.system import MetaConfig
+
 from pcvs.helpers.exceptions import CommonException
+from pcvs.helpers.system import MetaConfig
 
 
 def generate_local_variables(label, subprefix):
     """Return directories from PCVS working tree :
 
         - the base source directory
         - the current source directory
@@ -16,20 +17,17 @@
     :param subprefix: path to the subdirectories in the base path
     :type subprefix: str
     :raises CommonException.NotFoundError: the label is not recognized as to be
         validated
     :return: paths for PCVS working tree
     :rtype: tuple
     """
-    if label not in MetaConfig.root.validation.dirs:
-        raise CommonException.NotFoundError(label)
-
     if subprefix is None:
         subprefix = ""
 
-    base_srcdir = MetaConfig.root.validation.dirs[label]
+    base_srcdir = MetaConfig.root.validation.dirs.get(label, '')
     cur_srcdir = os.path.join(base_srcdir, subprefix)
     base_buildir = os.path.join(
         MetaConfig.root.validation.output, "test_suite", label)
     cur_buildir = os.path.join(base_buildir, subprefix)
 
-    return base_srcdir, cur_srcdir, base_buildir, cur_buildir
+    return base_srcdir, cur_srcdir, base_buildir, cur_buildir
```

### Comparing `pcvs-0.6.0/pcvs/testing/tedesc.py` & `pcvs-0.7.0/pcvs/testing/tedesc.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,21 @@
+import shutil
+import tempfile
 import copy
 import os
 import re
 
-from pcvs.helpers import pm, utils
+import pcvs
+from pcvs import testing
+from pcvs.helpers import pm
 from pcvs.helpers.criterion import Criterion, Serie
-from pcvs.helpers.exceptions import TestException
+from pcvs.helpers.exceptions import TestException, ProfileException
 from pcvs.helpers.system import MetaConfig, MetaDict
 from pcvs.testing.test import Test
-from pcvs import testing
+
 
 def detect_source_lang(array_of_files):
     """Determine compilation language for a target file (or list of files).
 
     Only one language is detected at once.
 
     :param array_of_files: list of files to identify
@@ -19,15 +23,15 @@
     :return: the language code
     :rtype: str
     """
     detect = list()
     for f in array_of_files:
         if re.search(r'\.(h|H|i|I|s|S|c|c90|c99|c11)$', f):
             detect.append('cc')
-        elif re.search(r'\.C|cc|cxx|cpp|c\+\+$', f):
+        elif re.search(r'\.(C|cc|cxx|cpp|c\+\+)$', f):
             detect.append('cxx')
         elif re.search(r'\.(f|F)(77)$', f):
             detect.append('f77')
         elif re.search(r'\.(f|F)90$', f):
             detect.append('f90')
         elif re.search(r'\.(f|F)95$', f):
             detect.append('f95')
@@ -38,40 +42,49 @@
         elif re.search(r'\.(f|F)$', f):
             detect.append('fc')
 
     # now return the first valid language, according to settings
     # order matters: if sources contains multiple languages, the first
     # appearing in this list will be considered as the main language
     for i in ['f08', 'f03', 'f95', 'f90', 'f77', 'fc', 'cxx', 'cc']:
-        if i in detect and i in MetaConfig.root.compiler.commands:
+        if i in detect and i in MetaConfig.root.compiler:
             return i
     return 'cc'
 
 
-def prepare_cmd_build_variants(variants=[]):
-    """Build the list of extra args to add to a test using variants.
-
-    Each defined variant comes with an ``arg`` option. When tests enable this
-    variant, these definitions are additioned to test compilation command. For
-    instance, the variant ``omp`` defines `-fopenmp` within GCC-based profile.
-    When a test requests to be built we ``omp`` variant, the flag is appended to
-    cflags.
+def extract_compiler_config(lang, variants):
+    """
+    Build resource to compile based on language and variants involved.
 
-    :param variants: the list of variants to load
+    :param lang: target language
+    :type lang: str
+    :param variants: list of enabled variants
     :type variants: list
-    :return: the string as the concatenation of variant args
-    :rtype: str
+    :return: the program, its args and env modifiers (in that order)
+    :rtype: tuple
     """
-    s = ""
-    variant_def = MetaConfig.root.compiler.variants
-    for i in variants:
-
-        if i in variant_def.keys():
-            s = "{} {}".format(s, variant_def[i].args)
-    return s
+    if not lang or lang not in MetaConfig.root.compiler:
+        raise ProfileException.IncompleteError(
+            reason="Unknown language, not defined into Profile",
+            dbg_info={"lang": lang, "list": MetaConfig.root.compiler.keys()}
+        )
+    
+    config = MetaConfig.root.compiler[lang]
+    for v in variants:
+        if v in config.variants:
+            for k, v in config.variants[v].items():
+                if k == 'program':
+                    config[k] = v
+                else:
+                    config.setdefault(k, list())
+                    config[k] += v
+        else:
+            return (None, [], [])
+                    
+    return (config.program, config.args, config.envs)
 
 
 def build_job_deps(deps_node, pkg_label, pkg_prefix):
     """Build the dependency list from a given depenency YAML node.
 
     A ``depends_on`` is used by test to establish their relationship. It looks
     like:
@@ -162,47 +175,48 @@
         :type label: str
         :param subprefix: relative path between user dir & current TE testfile
         :type subprefix: str or NoneType
 
         :raises TDFormatError: Unproper YAML TE format (sanity check)
         """
         if not isinstance(node, dict):
-            raise TestException.TDFormatError(node)
+            raise TestException.TestExpressionError(node)
+        
         self._te_name = name
         self._skipped = name.startswith('.')
         self._te_label = label
         self._te_subtree = subprefix
 
         _, self._srcdir, _, self._buildir = testing.generate_local_variables(
             label,
             subprefix
         )
         # before doing anything w/ node:
         # arregate the 'group' definitions with the TE
         # to get all the fields in their final form
-        if 'group' in node:
-            assert(node['group'] in MetaConfig.root.group.keys())
+        if 'group' in node and node['group'] in MetaConfig.root.group.keys():
             tmp = MetaDict(MetaConfig.root.group[node['group']])
             tmp.update(MetaDict(node))
             node = tmp
         # load from descriptions
         self._build = MetaDict(node.get('build', None))
         self._run = MetaDict(node.get('run', None))
         self._validation = MetaDict(node.get('validate', None))
         self._artifacts = MetaDict(node.get('artifact', None))
         self._metrics = MetaDict(node.get('metric', None))
+        self._attributes = MetaDict(node.get("attributes", None))
         self._template = node.get('group', None)
         self._debug = self._te_name+":\n"
         self._effective_cnt = 0
         self._tags = node.get('tag', list())
 
         path_prefix = self._buildir
-        if self.get_run_attr('path_resolution', True) is False:
+        if self.get_attr('path_resolution', True) is False:
             path_prefix = ""
-            
+
         for elt_k, elt_v in self._artifacts.items():
             if not os.path.isabs(elt_v):
                 self._artifacts[elt_k] = os.path.join(path_prefix, elt_v)
 
         # allow tags to be given as array OR a single string
         if not isinstance(self._tags, list):
             self._tags = [self._tags]
@@ -217,28 +231,20 @@
             self._program_criterion = {}
 
         # compute local criterions relatively to system-wide's
         self._configure_criterions()
         # apply retro-compatibility w/ old syntax
         self._compatibility_support(node.get('_compat', None))
 
-    @staticmethod
-    def get_attr(node, name, dflt=None):
-        if 'attributes' in node and name in node['attributes'].keys():
-            return node['attributes'][name]
+    def get_attr(self, name, dflt=None):
+        if name in self._attributes:
+            return self._attributes[name]
         else:
             return dflt
 
-    def get_run_attr(self, name, default=None):
-        return TEDescriptor.get_attr(self._run, name, default)
-
-    def get_build_attr(self, name, default=None):
-        return TEDescriptor.get_attr(self._build, name, default)
-    
-
     def _compatibility_support(self, compat):
         """Convert tricky keywords from old syntax too complex to be handled
         by the automatic converter.
 
         :param compat: dict of complex keyword extracted from old syntax.
         :param compat: dict or NoneType
         """
@@ -265,14 +271,24 @@
             # same as for chdir, 'bin' may be used by both build & run
             # but should set either not existing already
             elif 'bin' in k:
                 if self._build and 'binary' not in self._build:
                     self._build.binary = compat[k]
                 if self._run and 'program' not in self._run:
                     self._run.program = compat[k]
+        
+        if 'cflags' in self._build and 'sources' in self._build:
+            self._build['sources']['cflags'] = self._build['cflags']
+        if 'ldflags' in self._build and 'sources' in self._build:
+            self._build['sources']['ldflags'] = self._build['ldflags']
+        if 'params' in self._build.get('autotools', {}):
+            self._build.autotools.args = self._build.autotools.params
+        if 'vars' in self._build.get('cmake', {}):
+            self._build.cmake.args = self._build.cmake.vars
+        
 
     def _configure_criterions(self):
         """Prepare the list of components this TE will be built against.
 
         It consists in interesecting system-wide criterions and their
         definitions with this overriden criterion by this TE. The result is then
         what tests will be built on. If there is no intersection between
@@ -296,15 +312,15 @@
                     cur_criterion.override(self._run.iterate[k_sys])
 
                     if cur_criterion.is_discarded():
                         continue
                     # merge manually some definitions made by
                     # runtime, as some may be required to expand values:
 
-                    cur_criterion.expand_values()
+                    cur_criterion.expand_values(v_sys)
                     cur_criterion.intersect(v_sys)
                     if cur_criterion.is_empty():
                         self._skipped = True
                     else:
                         tmp[k_sys] = cur_criterion
                 else:  # key is not overriden
                     tmp[k_sys] = v_sys
@@ -322,25 +338,28 @@
         """
         lang = detect_source_lang(self._build.files)
         binary = self._te_name
         if self._build.sources.binary:
             binary = self._build.sources.binary
         elif self._run.program:
             binary = self._run.program
+
         self._build.sources.binary = binary
 
-        command = "{cc} {var} {cflags} {files} {ldflags} {out}".format(
-            cc=MetaConfig.root.compiler.commands.get(lang, ''),
-            var=prepare_cmd_build_variants(self._build.variants),
-            cflags=self._build.get('cflags', ''),
+        program, args, envs = extract_compiler_config(lang, self._build.variants)
+        
+        command = "{cc} {cflags} {files} {ldflags} {args} {out}".format(
+            cc=program,
+            args=" ".join(args),
+            cflags=self._build.sources.get('cflags', ''),
             files=" ".join(self._build.files),
-            ldflags=self._build.get('ldflags', ''),
+            ldflags=self._build.sources.get('ldflags', ''),
             out="-o {}".format(os.path.join(self._buildir, binary))
         )
-        return command
+        return (command, envs)
 
     def __build_from_makefile(self):
         """How to create build tests from a Makefile.
 
         :return: the command to be used.
         :rtype: str
         """
@@ -348,67 +367,56 @@
         basepath = self._srcdir
 
         # change makefile path if overriden by 'files'
         if 'files' in self._build:
             basepath = os.path.dirname(self._build.files[0])
             command.append("-f {}".format(" ".join(self._build.files)))
 
+        compiler, args, envs = extract_compiler_config("cc", self._build.variants)
         # build the 'make' command
         command.append(
-            '-C {path} {target} '
-            'PCVS_CC="{cc}" PCVS_CXX="{cxx}" PCVS_CU="{cu}" PCVS_FC="{fc}" '
-            'PCVS_CFLAGS="{var} {cflags}" PCVS_LDFLAGS="{ldflags}"'.format(
+            '-C {path} {target} '.format(
                 path=basepath,
-                target=self._build.make.get('target', ''),
-                cc=MetaConfig.root.compiler.commands.get('cc', ''),
-                cxx=MetaConfig.root.compiler.commands.get('cxx', ''),
-                fc=MetaConfig.root.compiler.commands.get('fc', ''),
-                cu=MetaConfig.root.compiler.commands.get('cu', ''),
-                var=prepare_cmd_build_variants(self._build.variants),
-                cflags=self._build.get('cflags', ''),
-                ldflags=self._build.get('ldflags', '')
+                target=self._build.make.get('target', '')
             )
         )
-        return " ".join(command)
+        
+        command += " ".join(self._build['make'].get('args', []))
+        envs += self._build['make'].get('envs', [])
+
+        return (" ".join(command), envs)
 
     def __build_from_cmake(self):
         """How to create build tests from a CMake project.
 
         :return: the command to be used.
         :rtype: str
         """
         command = ["cmake"]
         if 'files' in self._build:
             command.append(self._build.files[0])
         else:
             command.append(self._srcdir)
+            
+        _, args, envs = extract_compiler_config("cc", self._build.variants)
         command.append(
-            r"-DCMAKE_C_COMPILER='{cc}' -DCMAKE_CXX_COMPILER='{cxx}' "
-            r"-DCMAKE_FC_COPILER='{fc}' -DCMAKE_CUDA_COMPILER='{cu}' "
-            r"-DCMAKE_C_FLAGS='{var} {cflags}' -DCMAKE_EXE_LINKER_FLAGS='{ldflags}' "
             r"-G 'Unix Makefiles' "
-            r"-DCMAKE_BINARY_DIR='{build}' "
-            r"-DCMAKE_MODULE_LINKER_FLAGS='{ldflags}' "
-            r"-DCMAKE_SHARED_LINKER_FLAGS='{ldflags}'".format(
-                cc=MetaConfig.root.compiler.commands.get('cc', ''),
-                cxx=MetaConfig.root.compiler.commands.get('cxx', ''),
-                fc=MetaConfig.root.compiler.commands.get('fc', ''),
-                cu=MetaConfig.root.compiler.commands.get('cu', ''),
-                var=prepare_cmd_build_variants(self._build.variants),
-                cflags=self._build.get('cflags', ''),
-                ldflags=self._build.get('ldflags', ''),
+            r"-DCMAKE_BINARY_DIR='{build}' ".format(
                 build=self._buildir
             )
         )
-        if 'vars' in self._build['cmake']:
-            command.append("-D"+' -D'.join(self._build['cmake']['vars']))
+
+        command += self._build['cmake'].get('args', [])
+        envs += self._build['cmake'].get('envs', [])
 
         self._build.files = [os.path.join(self._buildir, "Makefile")]
-        next_command = self.__build_from_makefile()
-        return " && ".join([" ".join(command), next_command])
+        tmp =  self.__build_from_makefile()
+        next_command = tmp[0]
+        envs += tmp[1]
+        return (" && ".join([" ".join(command), next_command]), envs)
 
     def __build_from_autotools(self):
         """How to create build tests from a Autotools-based project.
 
         :return: the command to be used.
         :rtype: str
         """
@@ -423,51 +431,57 @@
 
         if self._build.autotools.get('autogen', False) is True:
             autogen_path = os.path.join(
                 os.path.dirname(configure_path),
                 "autogen.sh"
             )
             command.append("{} && ".format(autogen_path))
+            
+        _, _, envs = extract_compiler_config("cc", self._build.variants)
 
-        command.append(
-            r"{configure} "
-            r"CC='{cc}' CXX='{cxx}' "
-            r"FC='{fc}' NVCC='{cu}' "
-            r"CFLAGS='{var} {cflags}' LDFLAGS='{ldflags}' ".format(
-                configure=configure_path,
-                cc=MetaConfig.root.compiler.commands.get('cc', ''),
-                cxx=MetaConfig.root.compiler.commands.get('cxx', ''),
-                fc=MetaConfig.root.compiler.commands.get('fc', ''),
-                cu=MetaConfig.root.compiler.commands.get('cu', ''),
-                var=prepare_cmd_build_variants(self._build.variants),
-                cflags=self._build.get('cflags', ''),
-                ldflags=self._build.get('ldflags', ''),
-            )
-        )
-        if 'params' in self._build['autotools']:
-            command.append(" ".join(self._build['autotools']['params']))
+        command.append(r"{configure} ".format(configure=configure_path))
+        
+        command += self._build['autotools'].get('args', [])
+        envs += self._build['autotools'].get('envs', [])
 
         self._build.files = [os.path.join(self._buildir, "Makefile")]
-        next_command = self.__build_from_makefile()
-
+        tmp = self.__build_from_makefile()
+        next_command = tmp[0]
+        envs += tmp[1]
+        
         # TODO: why not creating another test, with a dep on this one ?
-        return " && ".join([" ".join(command), next_command])
+        return (" && ".join([" ".join(command), next_command]), envs)
+
+    def __build_from_user_script(self):
+        command = []
+        env = []
+        
+        command = self._build.custom.get('program', 'echo')
+        # args not relevant as cflags/ldflags can be used instead
+        env = self._build.custom.get('envs', [])
+        
+        if not os.path.isabs(command):
+            command = os.path.join(self._buildir, command)
+            
+        return (". {} && {}".format(os.path.join(MetaConfig.root.validation.output, pcvs.NAME_BUILD_CONF_SH), command), env)
 
-    def __build_command(self):
+    def __build_exec_process(self):
         """Drive compilation command generation based on TE format.
 
         :return: the command to be used.
         :rtype: str
         """
         if 'autotools' in self._build:
             return self.__build_from_autotools()
         elif 'cmake' in self._build:
             return self.__build_from_cmake()
         elif 'make' in self._build:
             return self.__build_from_makefile()
+        elif 'custom' in self._build:
+            return self.__build_from_user_script()
         else:
             return self.__build_from_sources()
 
     def __construct_compil_tests(self):
         """Meta-function steering compilation tests."""
         job_deps = []
 
@@ -489,30 +503,32 @@
 
         chdir = self._build.get('cwd')
         if chdir is not None and not os.path.isabs(chdir):
             chdir = os.path.abspath(os.path.join(self._buildir, chdir))
 
         tags = ["compilation"] + self._tags
 
-        command = self.__build_command()
+        command, env = self.__build_exec_process()
 
         # count number of built tests
         self._effective_cnt += 1
 
         yield Test(
             te_name=self._te_name,
             user_suffix="cc" if self._run else None,
             label=self._te_label,
             subtree=self._te_subtree,
             command=command,
+            environment=env,
             tags=tags,
             job_deps=job_deps,
             mod_deps=mod_deps,
-            time=self._validation.time.get("mean", 0),
+            time=self._validation.time.get("mean", -1),
             delta=self._validation.time.get("tolerance", 0),
+            kill_after=self._validation.time.get('kill_after', None),
             rc=self._validation.get("expect_exit", 0),
             artifacts=self._artifacts,
             analysis=self._validation.get("analysis", {}),
             resources=1,
             wd=chdir
         )
 
@@ -544,31 +560,37 @@
             # attempt to compute program/binary name
             program = self._te_name
             if self._run.program:
                 program = self._run.program
             elif self._build.sources.binary:
                 program = self._build.sources.binary
 
+
+            clone_outdir = self.get_attr('copy_output', False)
+            if clone_outdir:
+                buildir = tempfile.mkdtemp(prefix="{}.".format(self._te_name), dir=self._buildir)
+            else:
+                buildir = self._buildir
+
             # attempt to determine test working directory
-            chdir = self._run.cwd if self._run.cwd else self._buildir
-            
-                
+            chdir = self._run.cwd if self._run.cwd else buildir
+
             if not os.path.isabs(chdir):
-                chdir = os.path.abspath(os.path.join(self._buildir, chdir))
+                chdir = os.path.abspath(os.path.join(buildir, chdir))
 
             # keep the original value if user disabled prefix resolution
-            if self.get_run_attr('path_resolution', True) is True:
-                program = os.path.abspath(os.path.join(chdir, program))
+            if self.get_attr('path_resolution', True) is True:
+                program = os.path.abspath(os.path.join(self._buildir, program))
 
             command = "{program} {params}".format(
-                    program=program,
-                    params=" ".join(params)
-                )
-            if self.get_run_attr('command_wrap', True) is True:
-                command = "{runtime} {runtime_args} {args} {cmd}".format(
+                program=program,
+                params=" ".join(params)
+            )
+            if self.get_attr('command_wrap', True) is True:
+                command = "{runtime} {args} {runtime_args} {cmd}".format(
                     runtime=MetaConfig.root.runtime.get('program', ''),
                     runtime_args=MetaConfig.root.runtime.get('args', ''),
                     args=" ".join(args),
                     cmd=command
                 )
 
             self._effective_cnt += 1
@@ -580,16 +602,17 @@
                 command=command,
                 job_deps=te_job_deps,
                 mod_deps=te_mod_deps,
                 tags=self._tags,
                 metrics=self._metrics,
                 environment=env,
                 dim=comb.get('n_node', 1),
-                time=self._validation.time.get("mean", 0),
+                time=self._validation.time.get("mean", -1),
                 delta=self._validation.time.get("tolerance", 0),
+                kill_after=self._validation.time.get('kill_after', None),
                 rc=self._validation.get("expect_exit", 0),
                 valscript=self._validation.script.get('path', None),
                 analysis=self._validation.get("analysis", {}),
                 comb=comb,
                 wd=chdir,
                 artifacts=self._artifacts,
                 matchers=self._validation.get('match', None)
@@ -600,63 +623,69 @@
 
         This function will process a YAML node and, through a generator, will
         create each test coming from it.
         """
         # if this TE does not lead to a single test, skip now
         if self._skipped:
             return
-
+        
+        clone_indir = self.get_attr('copy_input', False)
+    
+        if clone_indir:
+            isolation_path = tempfile.mkdtemp(prefix="{}.".format(self._te_name), dir=self._buildir)
+            old_src_dir = self._srcdir
+            self._srcdir = os.path.join(isolation_path, "src")
+            shutil.copytree(old_src_dir, self._srcdir)
+            self._buildir = os.path.join(isolation_path, "build")
+            os.mkdir(self._buildir)
+                
+            
         if self._build:
             yield from self.__construct_compil_tests()
         if self._run:
-                
-            if self.get_run_attr('command_wrap', True) is False:
+
+            if self.get_attr('command_wrap', True) is False:
                 self._serie = Serie({**self._program_criterion})
             else:
-                self._serie = Serie({**self._criterion, **self._program_criterion})
+                self._serie = Serie(
+                    {**self._criterion, **self._program_criterion})
             yield from self.__construct_runtime_tests()
             del self._serie
 
     def get_debug(self):
         """Build information debug for the current TE.
 
         :return: the debug info 
         :rtype: dict
         """
         # if the current TE did not lead to a single test, skip now
         if self._skipped:
             return {}
 
-        user_cnt = 1
-        real_cnt = 1
         self._debug_yaml = dict()
 
-        # count the compilation run
-        if self._build:
-            real_cnt = 1
-
         # count actual tests built
         if self._run:
             # for system-wide iterators, count max number of possibilites
             for k, v in self._criterion.items():
                 self._debug_yaml[k] = list(v.values)
-                real_cnt *= len(v.values)
+                #real_cnt *= len(v.values)
 
             # for program-lavel iterators, count number of possibilies
             self._debug_yaml['program'] = dict()
             for k, v in self._program_criterion.items():
                 self._debug_yaml['program'][k] = list(v.values)
-                user_cnt *= len(v.values)
+                #user_cnt *= len(v.values)
 
         # store debug info
-        self._debug_yaml['.stats'] = {
-            'theoric': user_cnt * real_cnt,
-            'program_factor': user_cnt,
-            'effective': self._effective_cnt
-        }
+        #self._debug_yaml['.stats'] = {
+        #    'theoric': user_cnt * real_cnt,
+        #    'program_factor': user_cnt,
+        #    'effective': self._effective_cnt
+        #}
 
         return self._debug_yaml
 
     @property
     def name(self):
         """Getter to the current TE name.
```

### Comparing `pcvs-0.6.0/pcvs/testing/testfile.py` & `pcvs-0.7.0/pcvs/testing/testfile.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,123 +1,81 @@
+import tempfile
+import re
 import functools
+import pprint
 import getpass
 import operator
 import os
 import pathlib
 import subprocess
 
-import jsonschema
+from pcvs.helpers.exceptions import ValidationException
 from ruamel.yaml import YAML, YAMLError
 
-from pcvs import PATH_INSTDIR
-from pcvs.helpers import log, system, utils
+from pcvs import PATH_INSTDIR, io, testing
+from pcvs.helpers import system
 from pcvs.helpers.exceptions import TestException
 from pcvs.helpers.system import MetaConfig
 from pcvs.plugins import Plugin
 from pcvs.testing import tedesc
-from pcvs import testing
 
-def __load_yaml_file_legacy(f):
-    """Legacy version to load a YAML file.
 
-    This function intends to be backward-compatible with old YAML syntax
-    by relying on external converter (not perfect).
+constant_tokens = None
 
-    :raises DynamicProcessError: the setup script cannot be executed properly
-    :param f: old-syntax YAML filepath
-    :type f: str
-    :return: new-syntax YAML stream
+def init_constant_tokens():
     """
-    # Special case: old files required non-existing tags to be resolved
-    old_group_file = os.path.join(PATH_INSTDIR, "templates/group-compat.yml")
-
-    proc = subprocess.Popen(
-        "pcvs_convert '{}' --stdout -k te -t '{}'".format(
-            f,
-            old_group_file
-        ).split(),
-        stderr=subprocess.DEVNULL,
-        stdout=subprocess.PIPE,
-        shell=True)
-
-    fds = proc.communicate()
-    if proc.returncode != 0:
-        raise TestException.DynamicProcessError(f)
-
-    return fds[0].decode('utf-8')
-
-
-def replace_special_token(stream, src, build, prefix):
-    """Replace placeholders by their actual definition in a stream.
-
-    :param stream: the stream to alter
-    :type stream: str
-    :param src: source directory (replace SRCPATH)
-    :type src: str
-    :param build: build directory (replace BUILDPATH)
-    :type build: str
-    :param prefix: subtree for the current parsed stream
-    :type prefix: str
-    :return: the modified stream
-    :rtype: str
+    Initialize global tokens to be replaced.
+    
+    The dict is built from profile specifications. The exact location for this
+    function is still to be determined.
     """
-
+    global constant_tokens
+    constant_tokens = {
+        '@HOME@': str(pathlib.Path.home()),
+        '@USER@': getpass.getuser(),
+    }
+    for comp, comp_node in MetaConfig.root.compiler.items():
+        constant_tokens['@COMPILER_{}@'.format(comp.upper())] = comp_node.get('program', "")
+        
+    constant_tokens['@RUNTIME_PROGRAM@'] = MetaConfig.root.runtime.get('program', "")
+
+def replace_special_token(content, src, build, prefix, list=False):
+    output = []
+    errors = []
+    
+    global constant_tokens
+    if not constant_tokens:
+        init_constant_tokens()
+    
     if prefix is None:
         prefix = ""
+    
     tokens = {
+        **constant_tokens,
         '@BUILDPATH@': os.path.join(build, prefix),
         '@SRCPATH@': os.path.join(src, prefix),
         '@ROOTPATH@': src,
         '@BROOTPATH@': build,
         '@SPACKPATH@': "TBD",
-        '@HOME@': str(pathlib.Path.home()),
-        '@USER@': getpass.getuser()
     }
-    for k, v in tokens.items():
-        stream = stream.replace(k, v)
-    return stream
-
-
-def load_yaml_file(f, source, build, prefix):
-    """Load a YAML test description file.
-
-    :param f: YAML-based source testfile
-    :type f: str
-    :param source: source directory (used to replace placeholders)
-    :type source: str
-    :param build: build directory (placeholders)
-    :type build: str
-    :param prefix: file subtree (placeholders)
-    :type prefix: str
-    :return: the YAML-to-dict content
-    :rtype: dict
-    """
-    need_conversion = False
-    obj = {}
-    try:
-        with open(f, 'r') as fh:
-            stream = fh.read()
-            stream = replace_special_token(stream, source, build, prefix)
-            obj = YAML(typ='safe').load(stream)
-    # badly formatted YAML
-    except YAMLError:
-        need_conversion = True
-
-    # attempt to convert of the fly the YAML file
-    if need_conversion:
-        log.manager.debug("\t--> Legacy syntax: {}".format(f))
-        obj = YAML(typ='safe').load(__load_yaml_file_legacy(f))
-
-        # when 'debug' is activated, print the converted YAML file
-        if log.manager.has_verb_level('debug'):
-            cv_file = os.path.join(os.path.split(f)[0], "converted-pcvs.yml")
-            log.manager.debug("\t--> Stored file to {}".format(cv_file))
-            with open(cv_file, 'w') as fh:
-                YAML(typ='safe').dump(obj, fh)
-    return obj
+    
+    r = re.compile("(?P<name>@[a-zA-Z0-9-_]+@)")
+    for line in content.split('\n'):
+        for match in r.finditer(line):
+            
+            name = match.group('name')
+            if name not in tokens:
+                errors.append(name)
+            else:
+                line = line.replace(name, tokens[name])
+        output.append(line)
+
+    if errors:
+        raise ValidationException.WrongTokenError(invalid_tokens=errors)
+    return "\n".join(output)
 
 
 class TestFile:
     """A TestFile manipulates source files to be processed as benchmarks
 (pcvs.yml & pcvs.setup).
 
     It handles global informations about source imports & building one execution
@@ -163,59 +121,123 @@
         self._label = label
         self._prefix = prefix
         self._tests = list()
         self._debug = dict()
         if TestFile.val_scheme is None:
             TestFile.val_scheme = system.ValidationScheme('te')
 
+    def load_from_file(self, f):
+        with open(f, 'r') as fh:
+            stream = fh.read()
+            self.load_from_str(stream)
+
     def load_from_str(self, data):
         """Fill a File object from stream.
 
         This allows reusability (by loading only once).
 
         :param data: the YAML-formatted input stream.
         :type data: YAMl-formatted str
         """
         source, _, build, _ = testing.generate_local_variables(
             self._label, self._prefix)
+        
         stream = replace_special_token(data, source, build, self._prefix)
-        self._raw = YAML(typ='safe').load(stream)
+        try:
+            self._raw = YAML(typ='safe').load(stream)
+        except YAMLError as e:
+            raise ValidationException.FormatError(origin="<stream>")
+    
+    def save_yaml(self):
+        src, _, build, curbuild = testing.generate_local_variables(
+            self._label,
+            self._prefix)
+        
+        with open(os.path.join(curbuild, "pcvs.setup.yml"), "w") as fh:
+            YAML(typ='safe').dump(self._raw, fh)
+
+    def validate(self, allow_conversion=True) -> bool:
+        try:
+            if self._raw:
+                TestFile.val_scheme.validate(self._raw, filepath=self._in)
+            return True
+        except ValidationException.WrongTokenError as e:
+            # Issues with replacing @...@ keys
+            e.add_dbg(file=self._in)
+            raise TestException.TestExpressionError(self._in, error=e)
+        
+        except ValidationException.FormatError as e:
+            # YAML is valid but not following the Scheme
+            # If YAML is invalid, load() functions will failed first
+            
+            # At first attempt, YAML are converted.
+            # There is no second chance
+            if not allow_conversion:
+                e.add_dbg(file=self._in)
+                raise e
+            
+            tmpfile = tempfile.mkstemp()[1]
+            with open(tmpfile, 'w') as fh:
+                YAML(typ='safe').dump(self._raw, fh)
+            proc = subprocess.Popen(
+                "pcvs_convert {} --stdout -k te --skip-unknown -t '{}'".format(
+                    tmpfile,
+                    os.path.join(PATH_INSTDIR, "templates/config/group-compat.yml")),
+                stderr=subprocess.DEVNULL,
+                stdout=subprocess.PIPE,
+                shell=True)
+            
+            fds = proc.communicate()
+            os.remove(tmpfile)
+            if proc.returncode != 0:
+                raise e
+            converted_data = YAML(typ='safe').load(fds[0].decode('utf-8'))
+            #keep only TE conversion
+            # anything else is dropped when converting on-the-fly
+            self._raw = converted_data
+            self.validate(allow_conversion=False)
+            io.console.warning("\t--> Legacy syntax for: {}".format(self._in))
+            io.console.warning("Please consider updating it with `pcvs_convert -k te`")
+            return False
+
+    @property
+    def nb_descs(self):
+        if self._raw is None:
+            return 0
+        return len(self._raw.keys())
 
     def process(self):
         """Load the YAML file and map YAML nodes to Test()."""
         src, _, build, _ = testing.generate_local_variables(
             self._label,
             self._prefix)
 
+        # if file hasn't be loaded yet
         if self._raw is None:
-            self._raw = load_yaml_file(self._in, src, build, self._prefix)
-        # this check should also be used while loading the file.
-        # (old syntax files will only be converted if they are wrongly
-        # formatted, not if they are invalid)
-        try:
-            TestFile.val_scheme.validate(self._raw, filepath=self._in)
-        except jsonschema.ValidationError as e:
-            self._debug['.yaml_errors'].append(e)
+            self.load_from_file(self._in)
+            
+        self.validate()
 
         # main loop, parse each node to register tests
         for k, content, in self._raw.items():
             MetaConfig.root.get_internal(
                 "pColl").invoke_plugins(Plugin.Step.TDESC_BEFORE)
             if content is None:
                 # skip empty nodes
                 continue
             td = tedesc.TEDescriptor(k, content, self._label, self._prefix)
             for test in td.construct_tests():
                 self._tests.append(test)
+            io.console.info("{}: {}".format(td.name, pprint.pformat(td.get_debug())))
 
             MetaConfig.root.get_internal(
                 "pColl").invoke_plugins(Plugin.Step.TDESC_AFTER)
 
             # register debug informations relative to the loaded TEs
-            #self._debug[k] = td.get_debug()
+            self._debug[k] = td.get_debug()
 
     def flush_sh_file(self):
         """Store the given input file into their destination."""
         fn_sh = os.path.join(self._path_out, "list_of_tests.sh")
         cobj = MetaConfig.root.get_internal('cc_pm')
         if TestFile.cc_pm_string == "" and cobj:
             TestFile.cc_pm_string = "\n".join([
@@ -228,22 +250,31 @@
             TestFile.rt_pm_string = "\n".join([
                 e.get(load=True, install=False)
                 for e in robj
             ])
 
         with open(fn_sh, 'w') as fh_sh:
             fh_sh.write("""#!/bin/sh
-test -n '{simulated}' && PCVS_SHOW='all'
-if test -n "$PCVS_SHOW"; then
-    test "$PCVS_SHOW" = "env" -o "$PCVS_SHOW" = "all" &&  echo_env="echo " || echo_env="#"
-    test "$PCVS_SHOW" = "loads" -o "$PCVS_SHOW" = "all" &&  echo_load="echo " ||_echo_load="#"
-    test "$PCVS_SHOW" = "cmd" -o "$PCVS_SHOW" = "all" &&  echo_cmd="echo " || echo_cmd="#"
+if test -n "{simulated}"; then
+    PCVS_SHOW=1
+    PCVS_SHOW_ENV=1
+    PCVS_SHOW_MOD=1
+    PCVS_SHOW_CMD=1
+fi
+
+if test -z "$PCVS_SHOW"; then
+eval "{pm_string}"
+elif test -n "$PCVS_SHOW_MOD"; then
+test -n "$PCVS_VERBOSE" && echo "## MODULE LOADED FROM PROFILE ##"
+cat<<EOF
+{pm_string}
+EOF
+#else... SHOW but not this option --> nothing to do
+
 fi
-    
-eval "${{echo_load}}{pm_string}"
 
 for arg in "$@"; do case $arg in
 """.format(simulated="sim" if MetaConfig.root.validation.simulated is True else "",
                 pm_string="\n".join([
                         TestFile.cc_pm_string,
                         TestFile.rt_pm_string
                         ])))
@@ -254,38 +285,61 @@
 
             fh_sh.write("""
         --list) printf "{list_of_tests}\\n"; exit 0;;
         *) printf "Invalid test-name \'$arg\'\\n"; exit 1;;
         esac
     done
     
-    eval "${{echo_load}}${{pcvs_load}}"
-    eval "${{echo_env}}${{pcvs_env}}"
-    eval "${{echo_cmd}}${{pcvs_cmd}}"
+    if test -z "$PCVS_SHOW"; then
+        eval "${{pcvs_load}}" || exit "$?"
+        eval "${{pcvs_env}}" || exit "$?"
+        eval "${{pcvs_cmd}}" || exit "$?"
+        exit $?
+    else   
+        if test -n "$PCVS_SHOW_MOD"; then
+            test -n "$PCVS_VERBOSE" && echo "#### MODULE LOADED ####"
+cat<<EOF
+${{pcvs_load}}
+EOF
+        fi
+        
+        if test -n "$PCVS_SHOW_ENV"; then
+        test -n "$PCVS_VERBOSE" && echo "###### SETUP ENV ######"
+cat<<EOF
+${{pcvs_env}}
+EOF
+        fi
+        if test -n "$PCVS_SHOW_CMD"; then
+        test -n "$PCVS_VERBOSE" && echo "##### RUN COMMAND #####"
+cat<<EOF
+${{pcvs_cmd}}
+EOF
+        fi
+    fi
     exit $?\n""".format(list_of_tests="\n".join([
-                    t.name
-                    for t in self._tests
-                ])))
+                t.name
+                for t in self._tests
+            ])))
 
         self.generate_debug_info()
 
     def generate_debug_info(self):
         """Dump debug info to the appropriate file for the input object."""
-        if len(self._debug) and log.manager.has_verb_level('info'):
+        if len(self._debug) and io.console.verb_debug:
             with open(os.path.join(self._path_out, "dbg-pcvs.yml"), 'w') as fh:
                 # compute max number of combinations from system iterators
                 sys_cnt = functools.reduce(
                     operator.mul,
                     [
                         len(v['values'])
-                        for v in MetaConfig.root.criterion.iterators.values()
+                        for v in MetaConfig.root.criterion.values()
                     ]
                 )
                 self._debug.setdefault('.system-values', {})
                 self._debug['.system-values'].setdefault('stats', {})
 
-                for c_k, c_v in MetaConfig.root.criterion.iterators.items():
+                for c_k, c_v in MetaConfig.root.criterion.items():
                     self._debug[".system-values"][c_k] = c_v['values']
                 self._debug[".system-values"]['stats']['theoric'] = sys_cnt
                 yml = YAML(typ='safe')
                 yml.default_flow_style = None
                 yml.dump(self._debug, fh)
```

### Comparing `pcvs-0.6.0/pcvs/webview/__init__.py` & `pcvs-0.7.0/pcvs/webview/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,28 +2,27 @@
 import json
 import os
 import random
 
 from flask import Flask, abort, jsonify, render_template, request, sessions
 
 from pcvs import PATH_INSTDIR
-from pcvs.backend import session
 from pcvs.testing.test import Test
-from pcvs.webview import datalayer
 
-data_manager = datalayer.DataRepresentation()
+data_manager = None
 
 
-def create_app():
+def create_app(iface):
     """Start and run the Flask application.
 
     :return: the application
     :rtype: :class:`Flask`
     """
     global data_manager
+    data_manager = iface
 
     app = Flask(__name__, template_folder=os.path.join(
         PATH_INSTDIR, "webview/templates"))
 
     # app.config.from_object(...)
     @app.route('/about')
     def about():
@@ -49,40 +48,47 @@
     def root():
         """Provide the main page.
 
         :return: webpage content
         :rtype: str
         """
         if 'json' in request.args.get("render", []):
-            return jsonify(data_manager.get_sessions())
+            return jsonify(list(data_manager.session_infos()))
         return render_template("main.html")
 
     @app.route("/run/<sid>")
     def session_main(sid):
         """Provide the per-session main page
 
         :param sid: session id
         :type sid: str
         :return: page content
         :rtype: str
         """
         sid = int(sid)
-        assert(sid in data_manager.session_ids)
+        if sid not in data_manager.session_ids:
+            abort(404)
+
+        labels = data_manager.single_session_labels(sid)
+        tags = data_manager.single_session_tags(sid)
+        jobs_cnt = data_manager.single_session_job_cnt(sid)
 
         if 'json' in request.args.get('render', []):
-            return jsonify({"tag": data_manager.get_tag_cnt(sid),
-                            "label": data_manager.get_label_cnt(sid),
-                            "test": data_manager.get_test_cnt(sid)
+            return jsonify({"tag": len(tags),
+                            "label": len(labels),
+                            "test": jobs_cnt,
+                            "config": data_manager.single_session_config(sid)
                             })
         return render_template('session_main.html',
                                sid=sid,
-                               rootdir=data_manager.get_root_path(sid),
-                               nb_tests=data_manager.get_test_cnt(sid),
-                               nb_labels=data_manager.get_label_cnt(sid),
-                               nb_tags=data_manager.get_tag_cnt(sid)
+                               rootdir=data_manager.single_session_build_path(
+                                   sid),
+                               nb_tests=jobs_cnt,
+                               nb_labels=len(labels),
+                               nb_tags=len(tags)
                                )
 
     @app.route('/compare')
     def compare():
         """Provide the archive comparaison interface.
 
         :return: webpage content
@@ -91,35 +97,35 @@
         return render_template('tbw.html')
 
     @app.route("/run/<sid>/<selection>/list")
     def get_list(sid, selection):
         """Get a listing.
 
         The response will depend on the request, which can be:
-            * tag
+            * tags
             * label
             * status
 
         Providing a GET ``render`` to ``json`` returns the raw JSON version.
 
         :param selection: which listing to target
         :type selection: str
         :return: web content
         :rtype: str
         """
         sid = int(sid)
         if 'json' in request.args.get('render', []):
             out = list()
-            infos = data_manager.get_token_content(sid, selection)
-            if '__elems' in infos:
-                for k, v in infos['__elems'].items():
-                    out.append({
-                        "name": k,
-                        "count": v['__metadata']['count']
-                    })
+            infos = data_manager.single_session_get_view(
+                sid, selection, summary=True)
+            for k, v in infos.items():
+                out.append({
+                    "name": k,
+                    "count": v
+                })
             return jsonify(out)
 
         return render_template('list_view.html', sid=sid, selection=selection)
 
     @app.route("/run/<sid>/<selection>/detail")
     def get_details(sid, selection):
         """Get a detailed view of a component.
@@ -137,18 +143,31 @@
         :rtype: str
         """
         sid = int(sid)
         out = list()
         request_item = request.args.get('name', None)
 
         if 'json' in request.args.get('render', []):
-            infos = data_manager.get_token_content(sid, selection)
-            if request_item in infos['__elems'].keys():
-                out = data_manager.extract_tests_under(
-                    infos['__elems'][request_item])
+            # special case
+            if selection == "status":
+                job_list = data_manager.single_session_status(
+                    sid, filter=request_item)
+            else:
+                struct = data_manager.single_session_get_view(
+                    sid, selection, subset=request_item, summary=False)
+                # jobs are returned split into 3 lists, depending on their status
+                # -> browse all three lists
+                job_list = list()
+                for e, m in struct.items():
+                    for sn, s in m.items():
+                        job_list += s
+            for elt in job_list:
+                cur: Test = data_manager.single_session_map_id(sid, elt)
+                out.append(cur.to_json(strstate=True))
+
             return jsonify(out)
 
         return render_template("detailed_view.html",
                                sid=sid,
                                selection=selection,
                                sel_item=request_item)
 
@@ -157,36 +176,35 @@
         """Entry point to receive new session request.
 
         :return: OK
         :rtype: HTTP request
         """
         json_session = request.get_json()
         sid = json_session["sid"]
-        data_manager.insert_session(sid, json_session)
+        data_manager.add_session(sid, json_session)
 
         return "OK!", 200
 
     @app.route("/submit/session_fini", methods=["POST"])
     def submit_end_session():
         """Entry point to request a session end.
 
         :return: OK
         :rtype: HTTP request
         """
-        json_session = request.get_json()
-        data_manager.close_session(json_session["sid"], json_session)
         return "OK!", 200
 
     @app.route("/submit/test", methods=["POST"])
     def submit():
         """Entry point to receive test data.
 
         :return: OK
         :rtype: HTTP request
         """
+        return "OK!", 200
         json_str = request.get_json()
 
         test_sid = json_str["metadata"]["sid"]
         test_obj = Test()
         test_obj.from_json(json_str["test_data"])
 
         ok = data_manager.insert_test(test_sid, test_obj)
@@ -203,16 +221,8 @@
         :param e: the caught error, only 404 here
         :type e: int
         :return: web content
         :rtype: str
         """
         return render_template('404.html')
 
-    def get_data_manager():
-        """Getter to the webview data manager.
-
-        :return: the data manager holding test-suite data.
-        :rtype: :class:`DataRepresentation`
-        """
-        return data_manager
-
     return app
```

### Comparing `pcvs-0.6.0/pcvs/webview/datalayer.py` & `pcvs-0.7.0/pcvs/webview/datalayer.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         :param test: the test to insert
         :type test: class:`Test`
         :param node: a global tree intermediate node
         :type node: dict
         :param depth: list of node names to walk through
         :type depth: list
         """
-        assert('__metadata' in node.keys())
+        assert ('__metadata' in node.keys())
 
         node["__metadata"]["count"][str(test.state)] += 1
 
         # if targeted node is reached, insert the test
         if len(depth) == 0:
             if '__elems' not in node:
                 node['__elems'] = list()
@@ -125,15 +125,15 @@
         """Update the tree when the targeted session is completed.
 
         :param sid: targeted session id
         :type sid: int
         :param session_data: session infos (state)
         :type session_data: dict
         """
-        assert(sid in self.rootree.keys())
+        assert (sid in self.rootree.keys())
         self.rootree[sid]["state"] = session_data["state"]
 
     def insert_test(self, sid, test: Test):
         """Insert a new test.
 
         This test is bound to a session.
 
@@ -237,15 +237,15 @@
         """Retrieve all tests undef a given data tree subnode.
 
         :param node: data subnode
         :type node: dict
         :return: list of tests under this subnode
         :rtype: list(class:`Test`)
         """
-        assert('__elems' in node.keys())
+        assert ('__elems' in node.keys())
         if isinstance(node['__elems'], list):
             return [x.to_json(strstate=True) for x in node['__elems'] if isinstance(x, Test)]
 
         ret = list()
         for elt in node['__elems'].values():
             ret += self.extract_tests_under(elt)
         return ret
```

### Comparing `pcvs-0.6.0/pcvs/webview/static/css/bootstrap.min.css` & `pcvs-0.7.0/pcvs/webview/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `pcvs-0.6.0/pcvs/webview/static/css/custom.css` & `pcvs-0.7.0/pcvs/webview/static/css/custom.css`

 * *Files 8% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 {
 	border: #2c2c2c 4px solid;
 	border-radius: 5px;
 	background-color:#2c2c2c;
 	color:white;
 	margin:10px;
 	overflow-x: auto;
+	white-space: pre-wrap; 
+	word-break: break-word;
 	/*white-space: pre-wrap;       /* Since CSS 2.1 */
 	/*white-space: -moz-pre-wrap;  /* Mozilla, since 1999 */
 	/*white-space: -pre-wrap;      /* Opera 4-6 */
 	/*white-space: -o-pre-wrap;    /* Opera 7 */
 	/*word-wrap: break-word;       /* Internet Explorer 5.5+ */
 }
```

### Comparing `pcvs-0.6.0/pcvs/webview/static/css/datatables.min.css` & `pcvs-0.7.0/pcvs/webview/static/css/datatables.min.css`

 * *Files identical despite different names*

### Comparing `pcvs-0.6.0/pcvs/webview/static/css/open-iconic-bootstrap.min.css` & `pcvs-0.7.0/pcvs/webview/static/css/open-iconic-bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `pcvs-0.6.0/pcvs/webview/static/fonts/open-iconic.svg` & `pcvs-0.7.0/pcvs/webview/static/fonts/open-iconic.svg`

 * *Files identical despite different names*

### Comparing `pcvs-0.6.0/pcvs/webview/static/images/cea_logo.png` & `pcvs-0.7.0/pcvs/webview/static/images/cea_logo.png`

 * *Files identical despite different names*

### Comparing `pcvs-0.6.0/pcvs/webview/static/images/favicon.ico` & `pcvs-0.7.0/pcvs/webview/static/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `pcvs-0.6.0/pcvs/webview/static/images/full_logo.png` & `pcvs-0.7.0/pcvs/webview/static/images/full_logo.png`

 * *Files identical despite different names*

### Comparing `pcvs-0.6.0/pcvs/webview/static/images/full_logo_transparent.png` & `pcvs-0.7.0/pcvs/webview/static/images/full_logo_transparent.png`

 * *Files identical despite different names*

### Comparing `pcvs-0.6.0/pcvs/webview/static/js/bootstrap.bundle.min.js` & `pcvs-0.7.0/pcvs/webview/static/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `pcvs-0.6.0/pcvs/webview/static/js/custom.js` & `pcvs-0.7.0/pcvs/webview/static/js/custom.js`

 * *Files identical despite different names*

### Comparing `pcvs-0.6.0/pcvs/webview/static/js/datatables.min.js` & `pcvs-0.7.0/pcvs/webview/static/js/datatables.min.js`

 * *Files identical despite different names*

### Comparing `pcvs-0.6.0/pcvs/webview/static/js/jquery.min.js` & `pcvs-0.7.0/pcvs/webview/static/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `pcvs-0.6.0/pcvs/webview/templates/base.html` & `pcvs-0.7.0/pcvs/webview/templates/base.html`

 * *Files identical despite different names*

### Comparing `pcvs-0.6.0/pcvs/webview/templates/brief.html` & `pcvs-0.7.0/pcvs/webview/templates/brief.html`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 {% extends 'base.html' %}
 {% block body %}
 
 <script type="text/javascript">
 	$(document).ready(function(){
 		$('#theTable').DataTable({
+			"pageLength": -1,
 			"paging": false,
 			"responsive": true
 		});
 		$("#success_bar").popover({
 			trigger: 'hover',
 			placement: 'auto',
 			title: "Successes",
```

### Comparing `pcvs-0.6.0/pcvs/webview/templates/detailed_view.html` & `pcvs-0.7.0/pcvs/webview/templates/detailed_view.html`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 					}
 				}
 	function refresh(){
 		$.getJSON("/run/{{sid}}/{{selection}}/detail?render=json&name={{sel_item}}", function(resp) {
 			$('#theTable').DataTable({
 			bDestroy: true,
 			"responsive": true,
+			pageLength: -1,
 			order: [[1, 'asc']],
 			"createdRow": createRow,
 			"search": {
 				"regex": true
 			},
 			data: resp,
 			columns: [
@@ -41,24 +42,24 @@
 					"orderable": false,
 					"data": null,
 					"className": 'detail-control text-center',
 					"render": function(d,t,s){return '<span class="oi oi-plus"></span>';}
 				},
 				{"responsivePriority": 2, "data": 'id.fq_name'},
 				{"responsivePriority": 4, "data": 'result', "render": function(d, t, s){return d.state;}},
-				{"responsivePriority": 3, "data": 'result', "render": function(d, t, s){return d.time.toFixed(2)+" s";}}
+				{"responsivePriority": 3, "data": 'result', "render": function(d, t, s){return d.time.toFixed(2);}}
 			]
 			});
 		}).done(function(){	
 		function format_testline(data)
 		{
 			var raw_log = "";
 			if(data.result['output'])
 			{
-				raw_log = "<pre><code>"+decodeURIComponent(escape(window.atob(data.result['output'])))+"</code></pre>";
+				raw_log = "<pre><code>"+decodeURIComponent(escape(window.atob(data.result['output']['raw'])))+"</code></pre>";
 			}
 			return '<pre>'+
 				data['exec']+
 				'</pre>'+
 				raw_log
 		}
 		$("#theTable tbody").on('click', 'td.detail-control',function(){
@@ -91,14 +92,14 @@
 <h2 id="#page-title" class="container-fluid text-center">{{selection}} View -- {{sel_item}} </h2>
 <table id='theTable' class="display" style="width:100%">
 	<thead>
 		<tr>
 			<th></th>
 			<th>Name</th>
 			<th>status</th>
-			<th>Elapsed time</th>
+			<th>Elapsed time (s)</th>
 			
 		</tr>
 	</thead>
 </table>
 
 {% endblock %}
```

### Comparing `pcvs-0.6.0/pcvs/webview/templates/list_view.html` & `pcvs-0.7.0/pcvs/webview/templates/list_view.html`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 <script type="text/javascript">
 	function refresh(){
 		$.getJSON("/run/{{sid}}/{{selection}}/list?render=json", function(resp){
 		$('#theTable').DataTable({
 		bDestroy: true,
 		paging: true,
+		pageLength: -1,
 		lengthmenu: [10, 50, 100, -1],
 		data: resp,
 		order: [[0, 'desc']],
 		columns: [
 			{
 				"data": 'count',
 				"render": {
@@ -47,15 +48,15 @@
 			page_ready();
 		});	
 	}
 	$(document).ready(function() {
 		page_waiting()
 		refresh()
 	});
-	var timeout = setInterval(refresh, 2000)
+	//var timeout = setInterval(refresh, 2000)
 </script>
 
 <h2 id="#page-title" class="container-fluid text-center">{{selection}} View</h2>
 <table id='theTable' class="display" style="width:100%">
 	<thead>
 		<tr>
 			<th>Progress</th>
```

### Comparing `pcvs-0.6.0/pcvs/webview/templates/main.html` & `pcvs-0.7.0/pcvs/webview/templates/main.html`

 * *Files 5% similar despite different names*

```diff
@@ -19,30 +19,31 @@
 
 	$.getJSON("/?render=json", function(resp){
 		$('#theTable').DataTable({
 			bDestroy: true,
 			responsive: true,
 			order: [[0, 'desc']],
 			paging: true,
+			pageLength: -1,
 			lengthMenu: [10, 50, 100, -1],
 			data: resp,
 			columnDefs: [
 				{targets: [0], "cellType": "th"},
 				{targets: [0, 1, 5], "className": "dt-body-center"},
 				{targets: [2, 3, 4], "className": "dt-body-right"}
 			],
 			columns: [
 				{"responsivePriority": 1, "title": "Session ID", "class": "center", "data": 'sid', "render": function(d, tr, r){
 					return "<a href='/run/"+d+"'>"+d+"</a>"
 			}},
 				{"responsivePriority": 2, "title": "State", "class": "center", "data": 'state'},
 				{"responsivePriority": 5, "title": "Successes", "data": 'count', "render": function(d, t, s){return d["SUCCESS"];}},
 				{"responsivePriority": 3, "title": "Failures", "data": 'count', "render": function(d, t, s){return d["FAILURE"];}},
-				{"responsivePriority": 6, "title": "Other", "data": 'count', "render": function(d, t, s){return d["WAITING"]+d["IN_PROGRESS"]+d["ERR_DEP"]+d["ERR_OTHER"];}},
-				{"responsivePriority": 4, "title": "Build path", "data": 'path'},
+				{"responsivePriority": 6, "title": "Other", "data": 'count', "render": function(d, t, s){return d["ERR_DEP"]+d["ERR_OTHER"];}},
+				{"responsivePriority": 4, "title": "Info", "data": 'info'},
 			]
 			});
 			
 		}).done(function(){
 		page_ready()
 	})
 }
```

### Comparing `pcvs-0.6.0/pcvs/webview/templates/session_main.html` & `pcvs-0.7.0/pcvs/webview/templates/session_main.html`

 * *Files 12% similar despite different names*

```diff
@@ -5,34 +5,35 @@
 
 <script language="javascript" type="text/javascript">
 	function refresh(){
 		metadata = $.getJSON("/run/{{sid}}?render=json", function(resp){
 			document.getElementById("labelnumber").textContent = resp.label
 			document.getElementById("tagnumber").textContent = resp.tag
 			document.getElementById("testnumber").textContent = resp.test
+			document.getElementById("config-block").textContent = JSON.stringify(resp.config, undefined, 2)
 		}).done(function(){
 			page_ready()
 		})
 	}
 	$(document).ready(function(){
 		page_waiting();
 		refresh();
 	});
-	var timeout = setInterval(refresh, 2000)
+	//var timeout = setInterval(refresh, 2000)
 </script>
 
 <h1 id="main-page-title">PCVS reporting interface</h1>
 
 <p>This mini-webserver gathers validation results processed from <code>{{ main_directory }}</code>
 The content of this main page is still in progress. Here a short list of pages already accessible:
 <ul>
-	<li><a href="/run/{{sid}}/fs-tree/list">Label-based results</a></li>
+	<li><a href="/run/{{sid}}/labels/list">Label-based results</a></li>
 	<li><a href="/run/{{sid}}/tags/list">Tag-based results</a></li>
-	<li><a href="/run/{{sid}}/iterators/list">Criterion-based results</a></li>
-	<li><a href="/run/{{sid}}/failures/list">Failure-only results</a></li>
+	<!--<li><a href="/run/{{sid}}/iterators/list">Criterion-based results</a></li>-->
+	<li><a href="/run/{{sid}}/status/detail?name=FAILURE">Failure-only results</a></li>
 </ul>
 </p>
 
 <div id="stat_cards" class="row">
 <div class="col-sm-4"><div class="card text-center"><div class="card-body">
 <h4 id="testnumber" class="card-title">{{"{:,}".format(nb_tests)}}</h4>
 <p class="card-text">Tests in Total</p>
@@ -45,8 +46,13 @@
 
 <div class="col-sm-4"><div class=" card text-center"><div class="card-body">
 <h4 id="labelnumber" class="card-title">{{"{:,}".format(nb_labels)}}</h4>
 <p class="card-text">Distinct Labels</p>
 </div></div></div>
 </div>
 
+<div class="config-display">
+<p>Configuration:</p>
+<pre><code id="config-block"></code></pre>
+</div>
+
 {% endblock %}
```

### Comparing `pcvs-0.6.0/pcvs.egg-info/PKG-INFO` & `pcvs-0.7.0/pcvs.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pcvs
-Version: 0.6.0
+Version: 0.7.0
 Home-page: https://pcvs.io/
 Author: Julien Adam
 Author-email: adamj@paratools.com
 Maintainer: Julien Adam
 Maintainer-email: adamj@paratools.com
 License: CeCILL-C
 Project-URL: Source Code, https://github.com/cea-hpc/pcvs.git/
@@ -16,79 +16,66 @@
 Description-Content-Type: text/markdown
 License-File: COPYING
 License-File: AUTHORS
 
 PCVS Documentation
 ==================
 
-## About
-
 Parallel Computing Validation System (PCVS) is a Validation Orchestrator
 designed by and for software at scale. Its primary target is HPC applications &
 runtimes but can flawlessly address smaller use cases. PCVS can help users to
 create their test scenarios and reuse them among multiples implementations, an
 high value when it comes to validating Programmation standards (like APIs &
 ABIs). No matter the number of programs, benchmarks, languages, or tech
 non-regression bases use, PCVS gathers in a single execution, and, with a focus
 on interacting with HPC batch managers efficiently, run jobs concurrently to
 reduce the time-to-result overall. Through basic YAML-based configuration files,
 PCVS handles more than hundreds of thousands of tests and helps developers to
 ensure code production is moving forward.
 
-PCVS is documented through ReStructuredText. which can be found under the
-`/docs` directory. A built version can be found at (https://pcvs.readthedocs.io)
-
 
 ## Quick installation guide
 
 A more detailed guide to install PCVS can be found in the appropriate
 documentation, here is a quick overview to set up and test the framework.
 
-.. code-block:: bash
+    # considering python3.7+
+    $ pip3 install -r requirements.txt
+    # for dev/testing purposes, use:
+    $ pip3 install -r requirements-dev.txt
+    $ pip3 install pcvs
+    # basic tests:
+    $ tox
+    # OR
+    $ coverage run
 
-	# considering python3.5+
-	$ pip3 install -r requirements.txt
-	# for dev/testing purposes, use:
-	$ pip3 install -r requirements-dev.txt
-	$ pip3 install pcvs
-	# basic tests:
-	$ tox
-	# OR
-	$ coverage run
 
 ## Complete documentation
 
 PCVS documentation is currently in active progress. Feel free to redistribute
 comments and/or notes to the dev team about what should be more covered.
 Multiple documentation can be generated from this repo:
 
 * the CLI is managed and documented through ``click``. The manpages can be
   automatically built with the third-party tool ``click-man`` (not a dep,
   should be installed manually). Note that these manpages may not contain more
   information than the content of each ``--help`` command.
 * The general documentation (readthedocs.io-formatted) through ``sphinx``, able
-  to generate multiple formats:
-
-.. code-block:: bash
-
-	$ pip3 install -r requirements-dev.txt
-	$ make -C docs/source # will list available doc formats
-	$ make -C docs/source man  # global documentation as man pages (not CLI)
-	$ make -C docs/source html  # readthedocs-based
+  to generate multiple formats. A built version can be found [here](https://pcvs.readthedocs.io).
 
 ## Contributions
 
 A guide about contributing to PCVS can be found in the 
 [`CONTRIBUTING`](docs/source/contribution.rst) section of the documentation.
 
 ## Authors
 
 This work is currently supported by the French Alternative Energies and Atomic
 Energy Commission (CEA). For any question and/or remarks, please contact :
 
 * Julien JAEGER <julien.jaeger@cea.fr>
+* Julien ADAM <julien.adam@paratools.com>
 
-
-## License
+## Licensing
 
 PCVS is released under the [CeCILL-C Free Software
-License.](https://cecill.info/licences/Licence_CeCILL-C_V1-en.txt)
+License.](https://cecill.info/licences/Licence_CeCILL-C_V1-en.txt).
```

### Comparing `pcvs-0.6.0/pcvs.egg-info/SOURCES.txt` & `pcvs-0.7.0/pcvs.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 COPYING
 MANIFEST.in
 README.md
 requirements-dev.txt
 requirements.txt
 setup.py
 pcvs/__init__.py
+pcvs/io.py
 pcvs/main.py
 pcvs/version.py
 pcvs.egg-info/PKG-INFO
 pcvs.egg-info/SOURCES.txt
 pcvs.egg-info/dependency_links.txt
 pcvs.egg-info/entry_points.txt
 pcvs.egg-info/requires.txt
@@ -25,19 +26,21 @@
 pcvs/backend/spack.py
 pcvs/backend/utilities.py
 pcvs/cli/__init__.py
 pcvs/cli/cli_bank.py
 pcvs/cli/cli_config.py
 pcvs/cli/cli_plumbing.py
 pcvs/cli/cli_profile.py
+pcvs/cli/cli_remote_run.py
 pcvs/cli/cli_report.py
 pcvs/cli/cli_run.py
 pcvs/cli/cli_session.py
 pcvs/cli/cli_utilities.py
 pcvs/converter/__init__.py
+pcvs/converter/result_converter.py
 pcvs/converter/yaml_converter.py
 pcvs/dsl/__init__.py
 pcvs/dsl/analysis.py
 pcvs/dsl/render.py
 pcvs/helpers/__init__.py
 pcvs/helpers/communications.py
 pcvs/helpers/criterion.py
@@ -47,14 +50,15 @@
 pcvs/helpers/pm.py
 pcvs/helpers/system.py
 pcvs/helpers/utils.py
 pcvs/orchestration/__init__.py
 pcvs/orchestration/__main__.py
 pcvs/orchestration/manager.py
 pcvs/orchestration/publishers.py
+pcvs/orchestration/runner.py
 pcvs/orchestration/set.py
 pcvs/plugins/__init__.py
 pcvs/plugins/default/__init__.py
 pcvs/plugins/default/validation.py
 pcvs/schemes/compiler-scheme.yml
 pcvs/schemes/criterion-scheme.yml
 pcvs/schemes/group-scheme.yml
@@ -67,14 +71,15 @@
 pcvs/templates/config/compiler.default.yml
 pcvs/templates/config/compiler.gcc.yml
 pcvs/templates/config/compiler.icc.yml
 pcvs/templates/config/compiler.mpi.yml
 pcvs/templates/config/criterion.default.yml
 pcvs/templates/config/criterion.large.yml
 pcvs/templates/config/criterion.small.yml
+pcvs/templates/config/group-compat.yml
 pcvs/templates/config/group.common.yml
 pcvs/templates/config/group.default.yml
 pcvs/templates/config/machine.default.yml
 pcvs/templates/config/machine.localhost.yml
 pcvs/templates/config/machine.slurm.yml
 pcvs/templates/config/runtime.default.yml
 pcvs/templates/config/runtime.mpi.yml
```

### Comparing `pcvs-0.6.0/setup.py` & `pcvs-0.7.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,31 +1,36 @@
+# add -dirty if staged area is not empty
 import os
-import subprocess
-
 import setuptools
-
 loc = {}
 with open(os.path.join("pcvs/version.py")) as fh:
     exec(fh.read(), None, loc)
 version = loc['__version__']
 
+try:
+    import sh
+    version += "+{}".format(sh.git("rev-parse", "HEAD").strip()[:8])
+    if sh.git('diff', 'HEAD'):
+        version += ".dirty"
+except:
+    pass
+
 with open("README.md", 'r') as f:
     desc = f.read()
 
 with open('requirements.txt') as f:
     requires = f.read().strip().split('\n')
 
-
 setuptools.setup(
     name="pcvs",
     version=version,
     license="CeCILL-C",
     author="Julien Adam",
     author_email="adamj@paratools.com",
-    maintainer="Julien Adam", 
+    maintainer="Julien Adam",
     maintainer_email="adamj@paratools.com",
     keywords="validation hpc test-suite",
     url="https://pcvs.io/",
     long_description=desc,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     include_package_data=True,
@@ -37,14 +42,15 @@
             ],
         },
 
     entry_points='''
         [console_scripts]
         pcvs=pcvs.main:cli
         pcvs_convert=pcvs.converter.yaml_converter:main
+        pcvs_result_convert=pcvs.converter.result_converter:main
     ''',
 
     project_urls={
         "Source Code": "https://github.com/cea-hpc/pcvs.git/",
         "Documentation": "https://pcvs.readthedocs.io/",
         },
     classifiers=[
```

### Comparing `pcvs-0.6.0/tests/pcvs/cli/test_config.py` & `pcvs-0.7.0/tests/pcvs/cli/test_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,18 +43,14 @@
     if config_scope and config_kind is None:
         res = click_call('config', 'list', token, success=False)
         assert ("Invalid " in res.stderr)
     else:
         res = click_call('config', 'list', token)
         assert (res.exit_code == 0)
 
-    if config_scope and config_kind:
-        res = click_call('config', 'list', token+".test")
-        assert ("WARN : no LABEL required" in res.stderr)
-
 def test_list_wrong():
     with pytest.raises(pcvs.helpers.exceptions.ConfigException.BadTokenError):
         res = click_call('config', 'list', 'error')
         #assert(res.exit_code != 0)
         #assert ('Invalid KIND' in res.stderr)
 
     with pytest.raises(pcvs.helpers.exceptions.ConfigException.BadTokenError):
@@ -157,21 +153,14 @@
 @patch('pcvs.backend.config.ConfigurationBlock', autospec=True)
 def test_edit(mock_config):
     instance = mock_config.return_value
     instance.is_found.return_value = True
     res = click_call('config', 'edit', "dummy-config")
     assert(res.exit_code == 0)
     instance.is_found.assert_called_once_with()
-    instance.edit.assert_called_once_with(os.environ.get('EDITOR', None))
-    
-    instance.reset_mock()
-    res = click_call('config', 'edit', "dummy-config", "-e", "editor")
-    assert(res.exit_code == 0)
-    instance.is_found.assert_called_once_with()
-    instance.edit.assert_called_once_with("editor")
 
     instance.reset_mock()
     instance.is_found.return_value = False
     res = click_call('config', 'edit', "dummy-config")
     assert(res.exit_code != 0)
     instance.is_found.assert_called_once_with()
-    instance.edit.assert_not_called()
+    instance.edit.assert_not_called()
```

### Comparing `pcvs-0.6.0/tests/pcvs/cli/test_profile.py` & `pcvs-0.7.0/tests/pcvs/cli/test_profile.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,21 +28,14 @@
 
     res = click_call('profile', 'list', 'local')
     assert(res.exit_code == 0)
     assert('default' in res.stdout)
     assert('user' not in res.stdout)
     assert('system-wide' not in res.stdout)
 
-    res = click_call('profile', 'list', 'global.system-wide')
-    assert(res.exit_code == 0)
-    assert('default' not in res.stdout)
-    assert('user' not in res.stdout)
-    assert('system-wide' in res.stdout)
-    assert('no LABEL required' in res.stderr)
-
 
 @patch('pcvs.backend.profile.Profile')
 def test_show(mock_pf):
     instance = mock_pf.return_value
     instance.is_found.return_value = True
     res = click_call('profile', 'show', 'local.default')
     assert(res.exit_code == 0)
```

### Comparing `pcvs-0.6.0/tests/pcvs/cli/test_run.py` & `pcvs-0.7.0/tests/pcvs/cli/test_run.py`

 * *Files identical despite different names*

### Comparing `pcvs-0.6.0/tests/pcvs/converter/test_converter.py` & `pcvs-0.7.0/tests/pcvs/converter/test_converter.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,14 @@
                 "n_mpi": None,
                 "n_omp": None,
                 "net": None
             }}, fh)
 
         ret = click_call('-k', 'te', '--stdout', f)
         assert(ret.exit_code == 0)
-        assert("Converted data written into <stdout>" in ret.stdout)
+        assert("Converted data written into <stdout>" in ret.stderr)
         assert("simple_counter_std_thread:" in ret.stdout)
 
         ret = click_call('-k', 'te', f)
         assert(ret.exit_code == 0)
         assert(os.path.exists(os.path.join(os.getcwd(), "convert-test.yml")))
```

