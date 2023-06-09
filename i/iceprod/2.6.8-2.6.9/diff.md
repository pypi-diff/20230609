# Comparing `tmp/iceprod-2.6.8.tar.gz` & `tmp/iceprod-2.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iceprod-2.6.8.tar", last modified: Fri Mar  3 23:07:51 2023, max compression
+gzip compressed data, was "iceprod-2.6.9.tar", last modified: Thu Apr 13 21:55:47 2023, max compression
```

## Comparing `iceprod-2.6.8.tar` & `iceprod-2.6.9.tar`

### file list

```diff
@@ -1,157 +1,161 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 23:07:51.689998 iceprod-2.6.8/
--rw-r--r--   0 root         (0) root         (0)     1078 2023-03-03 23:07:48.000000 iceprod-2.6.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2634 2023-03-03 23:07:51.689998 iceprod-2.6.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1774 2023-03-03 23:07:48.000000 iceprod-2.6.8/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 23:07:51.669998 iceprod-2.6.8/bin/
--rwxr-xr-x   0 root         (0) root         (0)    10083 2023-03-03 23:07:48.000000 iceprod-2.6.8/bin/basic_submit.py
--rwxr-xr-x   0 root         (0) root         (0)     1331 2023-03-03 23:07:48.000000 iceprod-2.6.8/bin/iceprod_add_site_to_master.py
--rwxr-xr-x   0 root         (0) root         (0)     1408 2023-03-03 23:07:48.000000 iceprod-2.6.8/bin/iceprod_debugger.py
--rwxr-xr-x   0 root         (0) root         (0)     1095 2023-03-03 23:07:48.000000 iceprod-2.6.8/bin/iceprod_gridftp_proxy.py
--rwxr-xr-x   0 root         (0) root         (0)     1330 2023-03-03 23:07:48.000000 iceprod-2.6.8/bin/iceprod_join_pool.py
--rwxr-xr-x   0 root         (0) root         (0)     3330 2023-03-03 23:07:48.000000 iceprod-2.6.8/bin/iceprod_rest.py
--rwxr-xr-x   0 root         (0) root         (0)     4606 2023-03-03 23:07:48.000000 iceprod-2.6.8/bin/iceprod_server.py
--rwxr-xr-x   0 root         (0) root         (0)     7147 2023-03-03 23:07:48.000000 iceprod-2.6.8/bin/iceprodsh
--rwxr-xr-x   0 root         (0) root         (0)     3697 2023-03-03 23:07:48.000000 iceprod-2.6.8/bin/loader.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 23:07:51.669998 iceprod-2.6.8/iceprod/
--rw-r--r--   0 root         (0) root         (0)      625 2023-03-03 23:07:49.000000 iceprod-2.6.8/iceprod/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2050 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/client_auth.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 23:07:51.673998 iceprod-2.6.8/iceprod/core/
--rw-r--r--   0 root         (0) root         (0)     2295 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5339 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/core/data_transfer.py
--rw-r--r--   0 root         (0) root         (0)    33372 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/core/dataclasses.py
--rw-r--r--   0 root         (0) root         (0)      580 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/core/defaults.py
--rw-r--r--   0 root         (0) root         (0)    45616 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/core/exe.py
--rw-r--r--   0 root         (0) root         (0)     4147 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/core/exe_helper.py
--rw-r--r--   0 root         (0) root         (0)    18444 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/core/exe_json.py
--rw-r--r--   0 root         (0) root         (0)     4927 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/core/file_catalog.py
--rw-r--r--   0 root         (0) root         (0)    15519 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/core/functions.py
--rw-r--r--   0 root         (0) root         (0)    16121 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/core/gridftp.py
--rw-r--r--   0 root         (0) root         (0)    21592 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/core/i3exec.py
--rw-r--r--   0 root         (0) root         (0)     6108 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/core/jsonUtil.py
--rw-r--r--   0 root         (0) root         (0)     4035 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/core/logger.py
--rw-r--r--   0 root         (0) root         (0)    20137 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/core/parser.py
--rw-r--r--   0 root         (0) root         (0)    25463 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/core/pilot.py
--rw-r--r--   0 root         (0) root         (0)    30084 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/core/resources.py
--rw-r--r--   0 root         (0) root         (0)     1949 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/core/serialization.py
--rw-r--r--   0 root         (0) root         (0)      556 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/core/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 23:07:51.673998 iceprod-2.6.8/iceprod/materialization/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/materialization/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1059 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/materialization/__main__.py
--rw-r--r--   0 root         (0) root         (0)    13808 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/materialization/materialize.py
--rw-r--r--   0 root         (0) root         (0)    14142 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/materialization/server.py
--rw-r--r--   0 root         (0) root         (0)     3247 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/materialization/service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 23:07:51.673998 iceprod-2.6.8/iceprod/modules/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/modules/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 23:07:51.677998 iceprod-2.6.8/iceprod/rest/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/rest/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1059 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/rest/__main__.py
--rw-r--r--   0 root         (0) root         (0)     4892 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/rest/auth.py
--rw-r--r--   0 root         (0) root         (0)     1829 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/rest/base_handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 23:07:51.677998 iceprod-2.6.8/iceprod/rest/handlers/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/rest/handlers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6045 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/rest/handlers/auth.py
--rw-r--r--   0 root         (0) root         (0)     2065 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/rest/handlers/config.py
--rw-r--r--   0 root         (0) root         (0)     8437 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/rest/handlers/credentials.py
--rw-r--r--   0 root         (0) root         (0)    12602 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/rest/handlers/datasets.py
--rw-r--r--   0 root         (0) root         (0)     3804 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/rest/handlers/grids.py
--rw-r--r--   0 root         (0) root         (0)    10884 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/rest/handlers/jobs.py
--rw-r--r--   0 root         (0) root         (0)    11679 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/rest/handlers/logs.py
--rw-r--r--   0 root         (0) root         (0)     5706 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/rest/handlers/pilots.py
--rw-r--r--   0 root         (0) root         (0)     7201 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/rest/handlers/task_stats.py
--rw-r--r--   0 root         (0) root         (0)    39436 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/rest/handlers/tasks.py
--rw-r--r--   0 root         (0) root         (0)     5278 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/rest/server.py
--rw-r--r--   0 root         (0) root         (0)      475 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/roles_groups.py
--rw-r--r--   0 root         (0) root         (0)     3120 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/s3.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 23:07:51.677998 iceprod-2.6.8/iceprod/server/
--rw-r--r--   0 root         (0) root         (0)     7572 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/server/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8125 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/server/config.py
--rw-r--r--   0 root         (0) root         (0)     6025 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/server/daemon.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 23:07:51.665998 iceprod-2.6.8/iceprod/server/data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 23:07:51.677998 iceprod-2.6.8/iceprod/server/data/etc/
--rw-r--r--   0 root         (0) root         (0)     1272 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/server/data/etc/config_defaults.json
--rw-r--r--   0 root         (0) root         (0)     1820 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/server/data/etc/iceprod_schema.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 23:07:51.681998 iceprod-2.6.8/iceprod/server/data/www/
--rw-r--r--   0 root         (0) root         (0)     8032 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/server/data/www/base.css
--rw-r--r--   0 root         (0) root         (0)    13205 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/server/data/www/chart.stackedarea.js
--rw-r--r--   0 root         (0) root         (0)      646 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/server/data/www/chosen-sprite.png
--rw-r--r--   0 root         (0) root         (0)      872 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/server/data/www/chosen-sprite@2x.png
--rw-r--r--   0 root         (0) root         (0)    26966 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/server/data/www/chosen.jquery.min.js
--rw-r--r--   0 root         (0) root         (0)    10751 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/server/data/www/chosen.min.css
--rw-r--r--   0 root         (0) root         (0)      643 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/server/data/www/documentation.css
--rw-r--r--   0 root         (0) root         (0)     1591 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/server/data/www/documentation.js
--rw-r--r--   0 root         (0) root         (0)     1150 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/server/data/www/favicon.ico
--rw-r--r--   0 root         (0) root         (0)      211 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/server/data/www/favicon.png
--rw-r--r--   0 root         (0) root         (0)    13277 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/server/data/www/fetch.js
--rw-r--r--   0 root         (0) root         (0)     1493 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/server/data/www/json-rpc.js
--rw-r--r--   0 root         (0) root         (0)     8775 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/server/data/www/jsonlint.js
--rw-r--r--   0 root         (0) root         (0)    46933 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/server/data/www/jsviews.min.js
--rw-r--r--   0 root         (0) root         (0)     3842 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/server/data/www/logo_155x60.png
--rw-r--r--   0 root         (0) root         (0)    10659 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/server/data/www/rest.js
--rw-r--r--   0 root         (0) root         (0)       26 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/server/data/www/robots.txt
--rw-r--r--   0 root         (0) root         (0)     5218 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/server/data/www/submit.css
--rw-r--r--   0 root         (0) root         (0)    29484 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/server/data/www/submit.js
--rw-r--r--   0 root         (0) root         (0)     7716 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/server/data/www/util.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 23:07:51.685998 iceprod-2.6.8/iceprod/server/data/www_templates/
--rw-r--r--   0 root         (0) root         (0)      315 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/server/data/www_templates/404.html
--rw-r--r--   0 root         (0) root         (0)     3092 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/server/data/www_templates/base.html
--rw-r--r--   0 root         (0) root         (0)     1317 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/server/data/www_templates/dataset_browse.html
--rw-r--r--   0 root         (0) root         (0)     4467 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/server/data/www_templates/dataset_detail.html
--rw-r--r--   0 root         (0) root         (0)     2659 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/server/data/www_templates/groups.html
--rw-r--r--   0 root         (0) root         (0)     2285 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/server/data/www_templates/job_browse.html
--rw-r--r--   0 root         (0) root         (0)     2255 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/server/data/www_templates/job_detail.html
--rw-r--r--   0 root         (0) root         (0)      611 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/server/data/www_templates/login.html
--rw-r--r--   0 root         (0) root         (0)      183 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/server/data/www_templates/logout.html
--rw-r--r--   0 root         (0) root         (0)      352 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/server/data/www_templates/main.html
--rw-r--r--   0 root         (0) root         (0)     5739 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/server/data/www_templates/profile.html
--rw-r--r--   0 root         (0) root         (0)     2121 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/server/data/www_templates/site.html
--rw-r--r--   0 root         (0) root         (0)     6626 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/server/data/www_templates/submit.html
--rw-r--r--   0 root         (0) root         (0)     1790 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/server/data/www_templates/task_browse.html
--rw-r--r--   0 root         (0) root         (0)     4893 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/server/data/www_templates/task_detail.html
--rw-r--r--   0 root         (0) root         (0)      360 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/server/data/www_templates/tasks.html
--rw-r--r--   0 root         (0) root         (0)     4547 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/server/dataset_prio.py
--rw-r--r--   0 root         (0) root         (0)     1125 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/server/documentation.py
--rw-r--r--   0 root         (0) root         (0)     3501 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/server/globus.py
--rw-r--r--   0 root         (0) root         (0)    30230 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/server/grid.py
--rw-r--r--   0 root         (0) root         (0)     6400 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/server/module.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 23:07:51.685998 iceprod-2.6.8/iceprod/server/modules/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/server/modules/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8049 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/server/modules/queue.py
--rw-r--r--   0 root         (0) root         (0)     1148 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/server/modules/schedule.py
--rw-r--r--   0 root         (0) root         (0)    28719 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/server/modules/website.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 23:07:51.685998 iceprod-2.6.8/iceprod/server/plugins/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/server/plugins/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11131 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/server/plugins/condor.py
--rw-r--r--   0 root         (0) root         (0)    43314 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/server/plugins/condor_direct.py
--rw-r--r--   0 root         (0) root         (0)     2463 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/server/plugins/condor_file_transfer.py
--rw-r--r--   0 root         (0) root         (0)    33448 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/server/plugins/sc_demo.py
--rw-r--r--   0 root         (0) root         (0)    10523 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/server/plugins/supercomp_cedar.py
--rw-r--r--   0 root         (0) root         (0)    22909 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/server/plugins/supercomp_graham.py
--rw-r--r--   0 root         (0) root         (0)    10174 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/server/priority.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 23:07:51.689998 iceprod-2.6.8/iceprod/server/scheduled_tasks/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/server/scheduled_tasks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2927 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/server/scheduled_tasks/buffer_jobs_tasks.py
--rw-r--r--   0 root         (0) root         (0)     3846 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/server/scheduled_tasks/dataset_cleanup.py
--rw-r--r--   0 root         (0) root         (0)     3492 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/server/scheduled_tasks/dataset_completion.py
--rw-r--r--   0 root         (0) root         (0)     5660 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/server/scheduled_tasks/dataset_monitor.py
--rw-r--r--   0 root         (0) root         (0)     3183 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/server/scheduled_tasks/job_completion.py
--rw-r--r--   0 root         (0) root         (0)     4904 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/server/scheduled_tasks/job_temp_cleaning.py
--rw-r--r--   0 root         (0) root         (0)     2088 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/server/scheduled_tasks/log_cleanup.py
--rw-r--r--   0 root         (0) root         (0)     5274 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/server/scheduled_tasks/non_active_tasks.py
--rw-r--r--   0 root         (0) root         (0)     1698 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/server/scheduled_tasks/pilot_cleanup.py
--rw-r--r--   0 root         (0) root         (0)     2825 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/server/scheduled_tasks/pilot_monitor.py
--rw-r--r--   0 root         (0) root         (0)     5355 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/server/scheduled_tasks/queue_tasks.py
--rw-r--r--   0 root         (0) root         (0)     2480 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/server/scheduled_tasks/removed_tasks.py
--rw-r--r--   0 root         (0) root         (0)     3500 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/server/scheduled_tasks/reset_tasks.py
--rw-r--r--   0 root         (0) root         (0)     3896 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/server/scheduled_tasks/update_task_priority.py
--rw-r--r--   0 root         (0) root         (0)     3638 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/server/server.py
--rw-r--r--   0 root         (0) root         (0)     8667 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/server/ssl_cert.py
--rw-r--r--   0 root         (0) root         (0)     1344 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/server/task_queue.py
--rw-r--r--   0 root         (0) root         (0)     1177 2023-03-03 23:07:48.000000 iceprod-2.6.8/iceprod/server/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 23:07:51.669998 iceprod-2.6.8/iceprod.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2634 2023-03-03 23:07:51.000000 iceprod-2.6.8/iceprod.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4710 2023-03-03 23:07:51.000000 iceprod-2.6.8/iceprod.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-03 23:07:51.000000 iceprod-2.6.8/iceprod.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      368 2023-03-03 23:07:51.000000 iceprod-2.6.8/iceprod.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-03-03 23:07:51.000000 iceprod-2.6.8/iceprod.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     2051 2023-03-03 23:07:51.689998 iceprod-2.6.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      224 2023-03-03 23:07:48.000000 iceprod-2.6.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 21:55:47.106279 iceprod-2.6.9/
+-rw-r--r--   0 root         (0) root         (0)     1078 2023-04-13 21:55:43.000000 iceprod-2.6.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2634 2023-04-13 21:55:47.106279 iceprod-2.6.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1774 2023-04-13 21:55:43.000000 iceprod-2.6.9/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 21:55:47.082279 iceprod-2.6.9/bin/
+-rwxr-xr-x   0 root         (0) root         (0)    10083 2023-04-13 21:55:43.000000 iceprod-2.6.9/bin/basic_submit.py
+-rwxr-xr-x   0 root         (0) root         (0)     1331 2023-04-13 21:55:43.000000 iceprod-2.6.9/bin/iceprod_add_site_to_master.py
+-rwxr-xr-x   0 root         (0) root         (0)     1408 2023-04-13 21:55:43.000000 iceprod-2.6.9/bin/iceprod_debugger.py
+-rwxr-xr-x   0 root         (0) root         (0)     1095 2023-04-13 21:55:43.000000 iceprod-2.6.9/bin/iceprod_gridftp_proxy.py
+-rwxr-xr-x   0 root         (0) root         (0)     1330 2023-04-13 21:55:43.000000 iceprod-2.6.9/bin/iceprod_join_pool.py
+-rwxr-xr-x   0 root         (0) root         (0)     3330 2023-04-13 21:55:43.000000 iceprod-2.6.9/bin/iceprod_rest.py
+-rwxr-xr-x   0 root         (0) root         (0)     4606 2023-04-13 21:55:43.000000 iceprod-2.6.9/bin/iceprod_server.py
+-rwxr-xr-x   0 root         (0) root         (0)     7147 2023-04-13 21:55:43.000000 iceprod-2.6.9/bin/iceprodsh
+-rwxr-xr-x   0 root         (0) root         (0)     3697 2023-04-13 21:55:43.000000 iceprod-2.6.9/bin/loader.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 21:55:47.082279 iceprod-2.6.9/iceprod/
+-rw-r--r--   0 root         (0) root         (0)      625 2023-04-13 21:55:44.000000 iceprod-2.6.9/iceprod/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2050 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/client_auth.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 21:55:47.086279 iceprod-2.6.9/iceprod/core/
+-rw-r--r--   0 root         (0) root         (0)     2295 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5339 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/core/data_transfer.py
+-rw-r--r--   0 root         (0) root         (0)    33372 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/core/dataclasses.py
+-rw-r--r--   0 root         (0) root         (0)      591 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/core/defaults.py
+-rw-r--r--   0 root         (0) root         (0)    45616 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/core/exe.py
+-rw-r--r--   0 root         (0) root         (0)     4147 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/core/exe_helper.py
+-rw-r--r--   0 root         (0) root         (0)    18444 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/core/exe_json.py
+-rw-r--r--   0 root         (0) root         (0)     4927 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/core/file_catalog.py
+-rw-r--r--   0 root         (0) root         (0)    15519 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/core/functions.py
+-rw-r--r--   0 root         (0) root         (0)    16121 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/core/gridftp.py
+-rw-r--r--   0 root         (0) root         (0)    21592 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/core/i3exec.py
+-rw-r--r--   0 root         (0) root         (0)     6108 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/core/jsonUtil.py
+-rw-r--r--   0 root         (0) root         (0)     4035 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/core/logger.py
+-rw-r--r--   0 root         (0) root         (0)    20137 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/core/parser.py
+-rw-r--r--   0 root         (0) root         (0)    25463 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/core/pilot.py
+-rw-r--r--   0 root         (0) root         (0)    30084 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/core/resources.py
+-rw-r--r--   0 root         (0) root         (0)     1949 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/core/serialization.py
+-rw-r--r--   0 root         (0) root         (0)      556 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/core/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 21:55:47.090279 iceprod-2.6.9/iceprod/credentials/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/credentials/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1059 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/credentials/__main__.py
+-rw-r--r--   0 root         (0) root         (0)    19448 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/credentials/server.py
+-rw-r--r--   0 root         (0) root         (0)     6689 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/credentials/service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 21:55:47.090279 iceprod-2.6.9/iceprod/materialization/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/materialization/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1059 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/materialization/__main__.py
+-rw-r--r--   0 root         (0) root         (0)    13808 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/materialization/materialize.py
+-rw-r--r--   0 root         (0) root         (0)    14142 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/materialization/server.py
+-rw-r--r--   0 root         (0) root         (0)     3247 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/materialization/service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 21:55:47.090279 iceprod-2.6.9/iceprod/modules/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/modules/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 21:55:47.090279 iceprod-2.6.9/iceprod/rest/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/rest/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1059 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/rest/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     4892 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/rest/auth.py
+-rw-r--r--   0 root         (0) root         (0)     1829 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/rest/base_handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 21:55:47.094279 iceprod-2.6.9/iceprod/rest/handlers/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/rest/handlers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6045 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/rest/handlers/auth.py
+-rw-r--r--   0 root         (0) root         (0)     2022 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/rest/handlers/config.py
+-rw-r--r--   0 root         (0) root         (0)    12602 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/rest/handlers/datasets.py
+-rw-r--r--   0 root         (0) root         (0)     3804 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/rest/handlers/grids.py
+-rw-r--r--   0 root         (0) root         (0)    10884 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/rest/handlers/jobs.py
+-rw-r--r--   0 root         (0) root         (0)    11679 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/rest/handlers/logs.py
+-rw-r--r--   0 root         (0) root         (0)     5706 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/rest/handlers/pilots.py
+-rw-r--r--   0 root         (0) root         (0)     7201 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/rest/handlers/task_stats.py
+-rw-r--r--   0 root         (0) root         (0)    39436 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/rest/handlers/tasks.py
+-rw-r--r--   0 root         (0) root         (0)     5278 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/rest/server.py
+-rw-r--r--   0 root         (0) root         (0)      475 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/roles_groups.py
+-rw-r--r--   0 root         (0) root         (0)     3120 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/s3.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 21:55:47.094279 iceprod-2.6.9/iceprod/server/
+-rw-r--r--   0 root         (0) root         (0)     7572 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8125 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/config.py
+-rw-r--r--   0 root         (0) root         (0)     6025 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/daemon.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 21:55:47.078279 iceprod-2.6.9/iceprod/server/data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 21:55:47.094279 iceprod-2.6.9/iceprod/server/data/etc/
+-rw-r--r--   0 root         (0) root         (0)     1272 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/data/etc/config_defaults.json
+-rw-r--r--   0 root         (0) root         (0)     1820 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/data/etc/iceprod_schema.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 21:55:47.098279 iceprod-2.6.9/iceprod/server/data/www/
+-rw-r--r--   0 root         (0) root         (0)     8032 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/data/www/base.css
+-rw-r--r--   0 root         (0) root         (0)    13205 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/data/www/chart.stackedarea.js
+-rw-r--r--   0 root         (0) root         (0)      646 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/data/www/chosen-sprite.png
+-rw-r--r--   0 root         (0) root         (0)      872 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/data/www/chosen-sprite@2x.png
+-rw-r--r--   0 root         (0) root         (0)    26966 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/data/www/chosen.jquery.min.js
+-rw-r--r--   0 root         (0) root         (0)    10751 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/data/www/chosen.min.css
+-rw-r--r--   0 root         (0) root         (0)      643 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/data/www/documentation.css
+-rw-r--r--   0 root         (0) root         (0)     1591 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/data/www/documentation.js
+-rw-r--r--   0 root         (0) root         (0)     1150 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/data/www/favicon.ico
+-rw-r--r--   0 root         (0) root         (0)      211 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/data/www/favicon.png
+-rw-r--r--   0 root         (0) root         (0)    13277 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/data/www/fetch.js
+-rw-r--r--   0 root         (0) root         (0)     1493 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/data/www/json-rpc.js
+-rw-r--r--   0 root         (0) root         (0)     8775 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/data/www/jsonlint.js
+-rw-r--r--   0 root         (0) root         (0)    46933 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/data/www/jsviews.min.js
+-rw-r--r--   0 root         (0) root         (0)     3842 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/data/www/logo_155x60.png
+-rw-r--r--   0 root         (0) root         (0)    10659 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/data/www/rest.js
+-rw-r--r--   0 root         (0) root         (0)       26 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/data/www/robots.txt
+-rw-r--r--   0 root         (0) root         (0)     5218 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/data/www/submit.css
+-rw-r--r--   0 root         (0) root         (0)    29484 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/data/www/submit.js
+-rw-r--r--   0 root         (0) root         (0)     7716 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/data/www/util.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 21:55:47.102279 iceprod-2.6.9/iceprod/server/data/www_templates/
+-rw-r--r--   0 root         (0) root         (0)      315 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/data/www_templates/404.html
+-rw-r--r--   0 root         (0) root         (0)     3092 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/data/www_templates/base.html
+-rw-r--r--   0 root         (0) root         (0)     1317 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/data/www_templates/dataset_browse.html
+-rw-r--r--   0 root         (0) root         (0)     4467 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/data/www_templates/dataset_detail.html
+-rw-r--r--   0 root         (0) root         (0)     2659 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/data/www_templates/groups.html
+-rw-r--r--   0 root         (0) root         (0)     2285 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/data/www_templates/job_browse.html
+-rw-r--r--   0 root         (0) root         (0)     2255 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/data/www_templates/job_detail.html
+-rw-r--r--   0 root         (0) root         (0)      611 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/data/www_templates/login.html
+-rw-r--r--   0 root         (0) root         (0)      183 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/data/www_templates/logout.html
+-rw-r--r--   0 root         (0) root         (0)      352 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/data/www_templates/main.html
+-rw-r--r--   0 root         (0) root         (0)     6133 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/data/www_templates/profile.html
+-rw-r--r--   0 root         (0) root         (0)     2121 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/data/www_templates/site.html
+-rw-r--r--   0 root         (0) root         (0)     6626 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/data/www_templates/submit.html
+-rw-r--r--   0 root         (0) root         (0)     1790 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/data/www_templates/task_browse.html
+-rw-r--r--   0 root         (0) root         (0)     4893 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/data/www_templates/task_detail.html
+-rw-r--r--   0 root         (0) root         (0)      360 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/data/www_templates/tasks.html
+-rw-r--r--   0 root         (0) root         (0)     4547 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/dataset_prio.py
+-rw-r--r--   0 root         (0) root         (0)     1125 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/documentation.py
+-rw-r--r--   0 root         (0) root         (0)     3501 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/globus.py
+-rw-r--r--   0 root         (0) root         (0)    30282 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/grid.py
+-rw-r--r--   0 root         (0) root         (0)     6785 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/module.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 21:55:47.102279 iceprod-2.6.9/iceprod/server/modules/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/modules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8067 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/modules/queue.py
+-rw-r--r--   0 root         (0) root         (0)     1148 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/modules/schedule.py
+-rw-r--r--   0 root         (0) root         (0)    29105 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/modules/website.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 21:55:47.102279 iceprod-2.6.9/iceprod/server/plugins/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/plugins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11131 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/plugins/condor.py
+-rw-r--r--   0 root         (0) root         (0)    43247 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/plugins/condor_direct.py
+-rw-r--r--   0 root         (0) root         (0)     2463 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/plugins/condor_file_transfer.py
+-rw-r--r--   0 root         (0) root         (0)    33448 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/plugins/sc_demo.py
+-rw-r--r--   0 root         (0) root         (0)    10523 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/plugins/supercomp_cedar.py
+-rw-r--r--   0 root         (0) root         (0)    22909 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/plugins/supercomp_graham.py
+-rw-r--r--   0 root         (0) root         (0)    10174 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/priority.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 21:55:47.106279 iceprod-2.6.9/iceprod/server/scheduled_tasks/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/scheduled_tasks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2927 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/scheduled_tasks/buffer_jobs_tasks.py
+-rw-r--r--   0 root         (0) root         (0)     3846 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/scheduled_tasks/dataset_cleanup.py
+-rw-r--r--   0 root         (0) root         (0)     3492 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/scheduled_tasks/dataset_completion.py
+-rw-r--r--   0 root         (0) root         (0)     5660 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/scheduled_tasks/dataset_monitor.py
+-rw-r--r--   0 root         (0) root         (0)     3183 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/scheduled_tasks/job_completion.py
+-rw-r--r--   0 root         (0) root         (0)     4904 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/scheduled_tasks/job_temp_cleaning.py
+-rw-r--r--   0 root         (0) root         (0)     2088 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/scheduled_tasks/log_cleanup.py
+-rw-r--r--   0 root         (0) root         (0)     5274 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/scheduled_tasks/non_active_tasks.py
+-rw-r--r--   0 root         (0) root         (0)     1698 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/scheduled_tasks/pilot_cleanup.py
+-rw-r--r--   0 root         (0) root         (0)     2825 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/scheduled_tasks/pilot_monitor.py
+-rw-r--r--   0 root         (0) root         (0)     5355 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/scheduled_tasks/queue_tasks.py
+-rw-r--r--   0 root         (0) root         (0)     2480 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/scheduled_tasks/removed_tasks.py
+-rw-r--r--   0 root         (0) root         (0)     3500 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/scheduled_tasks/reset_tasks.py
+-rw-r--r--   0 root         (0) root         (0)     3896 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/scheduled_tasks/update_task_priority.py
+-rw-r--r--   0 root         (0) root         (0)     3638 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/server.py
+-rw-r--r--   0 root         (0) root         (0)     8667 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/ssl_cert.py
+-rw-r--r--   0 root         (0) root         (0)     1344 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/task_queue.py
+-rw-r--r--   0 root         (0) root         (0)     1177 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 21:55:47.086279 iceprod-2.6.9/iceprod.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2634 2023-04-13 21:55:47.000000 iceprod-2.6.9/iceprod.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4798 2023-04-13 21:55:47.000000 iceprod-2.6.9/iceprod.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 21:55:47.000000 iceprod-2.6.9/iceprod.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      368 2023-04-13 21:55:47.000000 iceprod-2.6.9/iceprod.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-04-13 21:55:47.000000 iceprod-2.6.9/iceprod.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     2090 2023-04-13 21:55:47.106279 iceprod-2.6.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      224 2023-04-13 21:55:43.000000 iceprod-2.6.9/setup.py
```

### Comparing `iceprod-2.6.8/LICENSE` & `iceprod-2.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.8/PKG-INFO` & `iceprod-2.6.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iceprod
-Version: 2.6.8
+Version: 2.6.9
 Summary: IceCube dataset management system
 Home-page: https://github.com/WIPACrepo/iceprod
 Download-URL: https://pypi.org/project/iceprod/
 Author: WIPAC Developers
 Author-email: developers@icecube.wisc.edu
 License: MIT
 Project-URL: Tracker, https://github.com/WIPACrepo/iceprod/issues
```

### Comparing `iceprod-2.6.8/README.rst` & `iceprod-2.6.9/README.rst`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.8/bin/basic_submit.py` & `iceprod-2.6.9/bin/basic_submit.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.8/bin/iceprod_add_site_to_master.py` & `iceprod-2.6.9/bin/iceprod_add_site_to_master.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.8/bin/iceprod_debugger.py` & `iceprod-2.6.9/bin/iceprod_debugger.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.8/bin/iceprod_gridftp_proxy.py` & `iceprod-2.6.9/bin/iceprod_gridftp_proxy.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.8/bin/iceprod_join_pool.py` & `iceprod-2.6.9/bin/iceprod_join_pool.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.8/bin/iceprod_rest.py` & `iceprod-2.6.9/bin/iceprod_rest.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.8/bin/iceprod_server.py` & `iceprod-2.6.9/bin/iceprod_server.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.8/bin/iceprodsh` & `iceprod-2.6.9/bin/iceprodsh`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.8/bin/loader.sh` & `iceprod-2.6.9/bin/loader.sh`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.8/iceprod/__init__.py` & `iceprod-2.6.9/iceprod/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,14 @@
 # version is a human-readable version number.
 
 # version_info is a four-tuple for programmatic comparison. The first
 # three numbers are the components of the version number. The fourth
 # is zero for an official release, positive for a development branch,
 # or negative for a release candidate or beta (after the base version
 # number has been incremented)
-__version__ = "2.6.8"
+__version__ = "2.6.9"
 version_info = (
     int(__version__.split(".")[0]),
     int(__version__.split(".")[1]),
     int(__version__.split(".")[2]),
     0,
 )
```

### Comparing `iceprod-2.6.8/iceprod/client_auth.py` & `iceprod-2.6.9/iceprod/client_auth.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.8/iceprod/core/__init__.py` & `iceprod-2.6.9/iceprod/core/__init__.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.8/iceprod/core/data_transfer.py` & `iceprod-2.6.9/iceprod/core/data_transfer.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.8/iceprod/core/dataclasses.py` & `iceprod-2.6.9/iceprod/core/dataclasses.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.8/iceprod/core/defaults.py` & `iceprod-2.6.9/iceprod/core/defaults.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     'job': 0,
     'jobs_submitted': 1,
     'resource_url': 'http://prod-exe.icecube.wisc.edu/',
     'data_url': 'gsiftp://gridftp.icecube.wisc.edu/',
     'svn_repository': 'http://code.icecube.wisc.edu/svn/',
     'site_temp': 'gsiftp://gridftp-scratch.icecube.wisc.edu/local/simprod/',
     'dataset_temp': '$(site_temp)/$(dataset)',
-    'job_temp': '$(site_temp)/$(job)',
+    'job_temp': '$(site_temp)/$(dataset)/$(job)',
 }
 
 
 def add_default_options(opts):
     """Add default config options"""
     for k in DEFAULT_OPTIONS:
         if k not in opts:
```

### Comparing `iceprod-2.6.8/iceprod/core/exe.py` & `iceprod-2.6.9/iceprod/core/exe.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.8/iceprod/core/exe_helper.py` & `iceprod-2.6.9/iceprod/core/exe_helper.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.8/iceprod/core/exe_json.py` & `iceprod-2.6.9/iceprod/core/exe_json.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.8/iceprod/core/file_catalog.py` & `iceprod-2.6.9/iceprod/core/file_catalog.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.8/iceprod/core/functions.py` & `iceprod-2.6.9/iceprod/core/functions.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.8/iceprod/core/gridftp.py` & `iceprod-2.6.9/iceprod/core/gridftp.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.8/iceprod/core/i3exec.py` & `iceprod-2.6.9/iceprod/core/i3exec.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.8/iceprod/core/jsonUtil.py` & `iceprod-2.6.9/iceprod/core/jsonUtil.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.8/iceprod/core/logger.py` & `iceprod-2.6.9/iceprod/core/logger.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.8/iceprod/core/parser.py` & `iceprod-2.6.9/iceprod/core/parser.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.8/iceprod/core/pilot.py` & `iceprod-2.6.9/iceprod/core/pilot.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.8/iceprod/core/resources.py` & `iceprod-2.6.9/iceprod/core/resources.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.8/iceprod/core/serialization.py` & `iceprod-2.6.9/iceprod/core/serialization.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.8/iceprod/core/util.py` & `iceprod-2.6.9/iceprod/core/util.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.8/iceprod/materialization/__main__.py` & `iceprod-2.6.9/iceprod/credentials/__main__.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.8/iceprod/materialization/materialize.py` & `iceprod-2.6.9/iceprod/materialization/materialize.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.8/iceprod/materialization/server.py` & `iceprod-2.6.9/iceprod/materialization/server.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.8/iceprod/materialization/service.py` & `iceprod-2.6.9/iceprod/materialization/service.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.8/iceprod/rest/__main__.py` & `iceprod-2.6.9/iceprod/materialization/__main__.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.8/iceprod/rest/auth.py` & `iceprod-2.6.9/iceprod/rest/auth.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.8/iceprod/rest/base_handler.py` & `iceprod-2.6.9/iceprod/rest/base_handler.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.8/iceprod/rest/handlers/auth.py` & `iceprod-2.6.9/iceprod/rest/handlers/auth.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.8/iceprod/rest/handlers/config.py` & `iceprod-2.6.9/iceprod/rest/handlers/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,14 @@
         Returns:
             dict: config
         """
         ret = await self.db.config.find_one(
             {'dataset_id':dataset_id},
             projection={'_id':False, 'dataset_id':False}
         )
-        logger.info('get config: %r', ret)
         if not ret:
             self.send_error(404, reason="Config not found")
         else:
             self.write(ret)
 
     @authorization(roles=['admin', 'user', 'system'])
     @attr_auth(arg='dataset_id', role='write')
```

### Comparing `iceprod-2.6.8/iceprod/rest/handlers/datasets.py` & `iceprod-2.6.9/iceprod/rest/handlers/datasets.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.8/iceprod/rest/handlers/grids.py` & `iceprod-2.6.9/iceprod/rest/handlers/grids.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.8/iceprod/rest/handlers/jobs.py` & `iceprod-2.6.9/iceprod/rest/handlers/jobs.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.8/iceprod/rest/handlers/logs.py` & `iceprod-2.6.9/iceprod/rest/handlers/logs.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.8/iceprod/rest/handlers/pilots.py` & `iceprod-2.6.9/iceprod/rest/handlers/pilots.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.8/iceprod/rest/handlers/task_stats.py` & `iceprod-2.6.9/iceprod/rest/handlers/task_stats.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.8/iceprod/rest/handlers/tasks.py` & `iceprod-2.6.9/iceprod/rest/handlers/tasks.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.8/iceprod/rest/server.py` & `iceprod-2.6.9/iceprod/rest/server.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.8/iceprod/s3.py` & `iceprod-2.6.9/iceprod/s3.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.8/iceprod/server/__init__.py` & `iceprod-2.6.9/iceprod/server/__init__.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.8/iceprod/server/config.py` & `iceprod-2.6.9/iceprod/server/config.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.8/iceprod/server/daemon.py` & `iceprod-2.6.9/iceprod/server/daemon.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.8/iceprod/server/data/etc/config_defaults.json` & `iceprod-2.6.9/iceprod/server/data/etc/config_defaults.json`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.8/iceprod/server/data/etc/iceprod_schema.json` & `iceprod-2.6.9/iceprod/server/data/etc/iceprod_schema.json`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.8/iceprod/server/data/www/base.css` & `iceprod-2.6.9/iceprod/server/data/www/base.css`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.8/iceprod/server/data/www/chart.stackedarea.js` & `iceprod-2.6.9/iceprod/server/data/www/chart.stackedarea.js`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.8/iceprod/server/data/www/chosen-sprite.png` & `iceprod-2.6.9/iceprod/server/data/www/chosen-sprite.png`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.8/iceprod/server/data/www/chosen-sprite@2x.png` & `iceprod-2.6.9/iceprod/server/data/www/chosen-sprite@2x.png`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.8/iceprod/server/data/www/chosen.jquery.min.js` & `iceprod-2.6.9/iceprod/server/data/www/chosen.jquery.min.js`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.8/iceprod/server/data/www/chosen.min.css` & `iceprod-2.6.9/iceprod/server/data/www/chosen.min.css`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.8/iceprod/server/data/www/documentation.css` & `iceprod-2.6.9/iceprod/server/data/www/documentation.css`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.8/iceprod/server/data/www/documentation.js` & `iceprod-2.6.9/iceprod/server/data/www/documentation.js`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.8/iceprod/server/data/www/favicon.ico` & `iceprod-2.6.9/iceprod/server/data/www/favicon.ico`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.8/iceprod/server/data/www/fetch.js` & `iceprod-2.6.9/iceprod/server/data/www/fetch.js`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.8/iceprod/server/data/www/json-rpc.js` & `iceprod-2.6.9/iceprod/server/data/www/json-rpc.js`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.8/iceprod/server/data/www/jsonlint.js` & `iceprod-2.6.9/iceprod/server/data/www/jsonlint.js`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.8/iceprod/server/data/www/jsviews.min.js` & `iceprod-2.6.9/iceprod/server/data/www/jsviews.min.js`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.8/iceprod/server/data/www/logo_155x60.png` & `iceprod-2.6.9/iceprod/server/data/www/logo_155x60.png`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.8/iceprod/server/data/www/rest.js` & `iceprod-2.6.9/iceprod/server/data/www/rest.js`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.8/iceprod/server/data/www/submit.css` & `iceprod-2.6.9/iceprod/server/data/www/submit.css`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.8/iceprod/server/data/www/submit.js` & `iceprod-2.6.9/iceprod/server/data/www/submit.js`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.8/iceprod/server/data/www/util.js` & `iceprod-2.6.9/iceprod/server/data/www/util.js`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.8/iceprod/server/data/www_templates/base.html` & `iceprod-2.6.9/iceprod/server/data/www_templates/base.html`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.8/iceprod/server/data/www_templates/dataset_browse.html` & `iceprod-2.6.9/iceprod/server/data/www_templates/dataset_browse.html`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.8/iceprod/server/data/www_templates/dataset_detail.html` & `iceprod-2.6.9/iceprod/server/data/www_templates/dataset_detail.html`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.8/iceprod/server/data/www_templates/groups.html` & `iceprod-2.6.9/iceprod/server/data/www_templates/groups.html`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.8/iceprod/server/data/www_templates/job_browse.html` & `iceprod-2.6.9/iceprod/server/data/www_templates/job_browse.html`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.8/iceprod/server/data/www_templates/job_detail.html` & `iceprod-2.6.9/iceprod/server/data/www_templates/job_detail.html`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.8/iceprod/server/data/www_templates/login.html` & `iceprod-2.6.9/iceprod/server/data/www_templates/login.html`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.8/iceprod/server/data/www_templates/profile.html` & `iceprod-2.6.9/iceprod/server/data/www_templates/profile.html`

 * *Files 8% similar despite different names*

```diff
@@ -21,14 +21,29 @@
 }
 div.section>:not(h4) {
     margin: 0 .5em;
 }
 div.section>h4 {
     margin: .5em 0;
 }
+div.section>h3 {
+    margin: .5em 0;
+}
+p, .form_group {
+    margin: .25em 0;
+}
+.indent {
+    margin-left: .25em;
+}
+.inline {
+    display: inline-block;
+}
+form button {
+    margin: .25em 0;
+}
 </style>
 {% end %}
 
 {% block page_title %}My Profile{% end %}
 
 {% block body %}
 <div class="section">
@@ -37,98 +52,98 @@
     <p>{{ username }}</p>
     <h4>Groups</h4>
     <ul class="groups">{% for g in groups %}<li>{{ g }}</li>{% end %}</ul>
 </div>
 <div class="section">
     <h3>Data Movement Credentials</h3>
     <h4>User Credentials</h4>
-    <div class="action">
+    <div class="indent">
     {% for url in user_creds %}
       <div class="cred">
         <p>URL: {{ url }}</p>
         <p>TYPE: {{ user_creds[url]["type"]}}</p>
       </div>
     {% end %}
       <form method="post">
         {% module xsrf_form_html() %}
         <button name="add_icecube_token" value="true" type="submit">Add IceCube Token</button>
       </form>
       <button onclick="$('#add_user_cred_form').show()">Add New User Credentials</button>
       <form method="post" id="add_user_cred_form" style="display: none">
         {% module xsrf_form_html() %}
-        <div>
+        <div class="form_group">
           <label for="userurl">URL:</label>
           <input type="text" name="url" id="userurl" />
         </div>
-        <div>Type:
-          <div class="action">
+        <div class="form_group">Type:
+          <div class="indent inline">
             <label for="usertypes3">S3:</label>
             <input type="radio" name="type" id="usertypes3" value="s3" onclick="$('#useroauth').hide();$('#users3').show()" />
           </div>
-          <div class="action">
+          <div class="indent inline">
             <label for="usertypeoauth">OAuth:</label>
             <input type="radio" name="type" id="usertypeoauth" value="oauth" onclick="$('#useroauth').show();$('#users3').hide()" />
           </div>
         </div>
-        <div id="users3" style="display: none">
+        <div id="users3" class="form_group" style="display: none">
           <label for="userbuckets">Bucket Names (one per line)</label><br>
-          <textarea name="buckets" id="userbuckets"></textarea>
+          <textarea name="buckets" id="userbuckets"></textarea><br>
           <label for="useraccesskey">Access Key</label><br>
           <textarea name="access_key" id="useraccesskey"></textarea><br>
           <label for="usersecretkey">Secret Key</label><br>
           <textarea name="secret_key" id="usersecretkey"></textarea>
         </div>
-        <div id="useroauth" style="display: none">
+        <div id="useroauth" class="form_group" style="display: none">
           <p>Must enter either an access or refresh token (or both)</p>
           <label for="useraccesstoken">Access Token</label><br>
           <textarea name="access_token" id="useraccesstoken"></textarea><br>
           <label for="userrefreshtoken">Refresh Token</label><br>
           <textarea name="refresh_token" id="userrefreshtoken"></textarea>
         </div>
         <button name="add_user_cred" value="true" type="submit">Submit</button>
       </form>
     </div>
     {% if groups != ['users'] %}
     <h4>Group Credentials</h4>
     {% for g in group_creds %}
       <p>GROUP: {{ g }}</p>
-      <div class="action">
+      <div class="indent">
       {% for url in group_creds[g] %}
         <div class="cred">
           <p>URL: {{ url }}</p>
           <p>TYPE: {{ group_creds[g][url]["type"]}}</p>
         </div>
       {% end %}
         <button onclick="$('#add_group_{{ g }}_cred_form').show()">Add New Group Credentials</button>
         <form method="post" id="add_group_{{ g }}_cred_form" style="display: none">
           {% module xsrf_form_html() %}
           <input type="hidden" name="groupname" value="{{ g }}" />
-          <div>
+          <div class="form_group">
             <label for="group_{{ g }}_url">URL:</label>
             <input type="text" name="url" id="group_{{ g }}_url" />
           </div>
-          <div>Type:
-            <div class="action">
+          <div class="form_group">Type:
+            <div class="indent inline">
               <label for="group_{{ g }}_types3">S3:</label>
               <input type="radio" name="type" id="group_{{ g }}_types3" value="s3" onclick="$('#group_{{ g }}_oauth').hide();$('#group_{{ g }}_s3').show()" />
             </div>
-            <div class="action">
+            <div class="indent inline">
               <label for="group_{{ g }}_typeoauth">OAuth:</label>
               <input type="radio" name="type" id="group_{{ g }}_typeoauth" value="oauth" onclick="$('#group_{{ g }}_oauth').show();$('#group_{{ g }}_s3').hide()" />
             </div>
           </div>
-          <div id="group_{{ g }}_s3" style="display: none">
+          <div id="group_{{ g }}_s3" class="form_group" style="display: none">
             <label for="group_{{ g }}_buckets">Bucket Names (one per line)</label><br>
-            <textarea name="buckets" id="group_{{ g }}_buckets"></textarea>
+            <textarea name="buckets" id="group_{{ g }}_buckets"></textarea><br>
             <label for="group_{{ g }}_accesskey">Access Key</label><br>
             <textarea name="access_key" id="group_{{ g }}_accesskey"></textarea><br>
             <label for="group_{{ g }}_secretkey">Secret Key</label><br>
             <textarea name="secret_key" id="group_{{ g }}_secretkey"></textarea>
           </div>
-          <div id="group_{{ g }}_oauth" style="display: none">
+          <div id="group_{{ g }}_oauth" class="form_group" style="display: none">
             <p>Must enter either an access or refresh token (or both)</p>
             <label for="group_{{ g }}_accesstoken">Access Token</label><br>
             <textarea name="access_token" id="group_{{ g }}_accesstoken"></textarea><br>
             <label for="group_{{ g }}_refreshtoken">Refresh Token</label><br>
             <textarea name="refresh_token" id="group_{{ g }}_refreshtoken"></textarea>
           </div>
           <button name="add_group_cred" value="true" type="submit">Submit</button>
```

### Comparing `iceprod-2.6.8/iceprod/server/data/www_templates/site.html` & `iceprod-2.6.9/iceprod/server/data/www_templates/site.html`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.8/iceprod/server/data/www_templates/submit.html` & `iceprod-2.6.9/iceprod/server/data/www_templates/submit.html`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.8/iceprod/server/data/www_templates/task_browse.html` & `iceprod-2.6.9/iceprod/server/data/www_templates/task_browse.html`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.8/iceprod/server/data/www_templates/task_detail.html` & `iceprod-2.6.9/iceprod/server/data/www_templates/task_detail.html`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.8/iceprod/server/dataset_prio.py` & `iceprod-2.6.9/iceprod/server/dataset_prio.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.8/iceprod/server/documentation.py` & `iceprod-2.6.9/iceprod/server/documentation.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.8/iceprod/server/globus.py` & `iceprod-2.6.9/iceprod/server/globus.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.8/iceprod/server/grid.py` & `iceprod-2.6.9/iceprod/server/grid.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,22 +51,23 @@
     Interface for a generic job distribution system.
     Do not use this class directly.  Use one of the plugins.
     """
 
     # use only these grid states when defining grid status
     GRID_STATES = ('queued','processing','completed','error','unknown')
 
-    def __init__(self, gridspec, queue_cfg, cfg, modules, executor, statsd, rest_client):
+    def __init__(self, gridspec, queue_cfg, cfg, modules, executor, statsd, rest_client, cred_client):
         self.gridspec = gridspec
         self.queue_cfg = queue_cfg
         self.cfg = cfg
         self.modules = modules
         self.executor = executor
         self.statsd = statsd
         self.rest_client = rest_client
+        self.cred_client = cred_client
 
         self.site = None
         if 'site' in self.queue_cfg:
             self.site = self.queue_cfg['site']
 
         self.credentials_dir = os.path.expanduser(os.path.expandvars(
             self.cfg['queue']['credentials_dir']))
@@ -386,24 +387,24 @@
                     )
 
             except Exception:
                 logger.error('error submitting pilots', exc_info=True)
 
     @ttl_cache(ttl=600)
     def get_token(self):
-        return self.rest_client.make_access_token()
+        return self.cred_client.make_access_token()
 
     @cached(TTLCache(1024, 60))
     async def get_user_credentials(self, username):
-        ret = await self.rest_client.request('GET', f'/users/{username}/credentials')
+        ret = await self.cred_client.request('GET', f'/users/{username}/credentials')
         return ret
 
     @cached(TTLCache(1024, 60))
     async def get_group_credentials(self, group):
-        ret = await self.rest_client.request('GET', f'/groups/{group}/credentials')
+        ret = await self.cred_client.request('GET', f'/groups/{group}/credentials')
         return ret
 
     async def customize_task_config(self, task_cfg, job_cfg=None, dataset=None):
         """Transforms for the task config"""
         logger.info('customize_task_config for %s', job_cfg.get('options', {}).get('task_id', 'unknown'))
 
         # first expand site temp urls
```

### Comparing `iceprod-2.6.8/iceprod/server/module.py` & `iceprod-2.6.9/iceprod/server/module.py`

 * *Files 7% similar despite different names*

```diff
@@ -109,14 +109,15 @@
     def __init__(self, cfg, executor, modules):
         self.cfg = cfg
         self.executor = executor
         self.statsd = FakeStatsClient()
         self.elasticsearch = FakeStatsClient()
         self.s3 = None
         self.rest_client = None
+        self.cred_client = None
         self.modules = modules
         self.service = {'start': self.start,
                         'stop': self.stop,
                         'kill': self.kill}
 
     def start(self):
         """
@@ -166,14 +167,20 @@
             try:
                 self.rest_client = ClientCredentialsAuth(
                     address=self.cfg['rest_api']['url'],
                     token_url=self.cfg['rest_api']['oauth_url'],
                     client_id=self.cfg['rest_api']['oauth_client_id'],
                     client_secret=self.cfg['rest_api']['oauth_client_secret'],
                 )
+                self.cred_client = ClientCredentialsAuth(
+                    address=self.cfg['rest_api']['cred_url'],
+                    token_url=self.cfg['rest_api']['oauth_url'],
+                    client_id=self.cfg['rest_api']['oauth_client_id'],
+                    client_secret=self.cfg['rest_api']['oauth_client_secret'],
+                )
             except Exception:
                 logger.warning('failed to connect to rest api: %r',
                                self.cfg['rest_api'].get('url',''), exc_info=True)
 
     def stop(self):
         logger.warning('stopping module %s', self.__class__.__name__)
```

### Comparing `iceprod-2.6.8/iceprod/server/modules/queue.py` & `iceprod-2.6.9/iceprod/server/modules/queue.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,15 +107,15 @@
         if 'max_task_processing_time' in self.cfg['queue']:
             self.max_duration += self.cfg['queue']['max_task_processing_time']
         for p,p_name,p_cfg in plugins_tmp:
             logger.warning('queueing plugin found: %s = %s', p_name, p_cfg['type'])
             # try instantiating the plugin
             args = (self.cfg['site_id']+'.'+p_name, p_cfg, self.cfg,
                     self.modules, self.executor, self.statsd,
-                    self.rest_client)
+                    self.rest_client, self.cred_client)
             try:
                 self.plugins.append(iceprod.server.run_module(p,*args))
             except Exception:
                 logger.error('Error importing plugin', exc_info=True)
             else:
                 desc = p_cfg['description'] if 'description' in p_cfg else ''
                 gridspec_types[self.cfg['site_id']+'.'+p_name] = {
```

### Comparing `iceprod-2.6.8/iceprod/server/modules/schedule.py` & `iceprod-2.6.9/iceprod/server/modules/schedule.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.8/iceprod/server/modules/website.py` & `iceprod-2.6.9/iceprod/server/modules/website.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 import os
 import random
 import logging
 from collections import defaultdict
 import functools
 from urllib.parse import urlencode
 import re
+from datetime import datetime, timedelta
 
 from iceprod.core.jsonUtil import json_encode
 
 import tornado.web
 import tornado.httpserver
 import tornado.gen
 import jwt
@@ -111,42 +112,48 @@
                         and 'oauth_client_id' in self.cfg['rest_api']
                         and 'oauth_client_secret' in self.cfg['rest_api']):
                     raise Exception('must set oauth_ params in cfg[rest_api]')
                 rest_cfg['auth'] = {
                     'audience': self.cfg['rest_api'].get('oauth_audience', 'iceprod'),
                     'openid_url': self.cfg['rest_api']['oauth_url'],
                 }
+
+                if 'cred_url' not in self.cfg['rest_api']:
+                    raise Exception('must set cred_url in cfg[rest_api]')
+                if not self.cred_client:
+                    raise Exception('credentials rest client not set up!')
+
             handler_args = RestHandlerSetup(rest_cfg)
+            handler_args['cred_rest_client'] = self.cred_client
+
+            full_url = self.cfg['webserver'].get('full_url', '')
+            handler_args['full_url'] = full_url
+            login_url = full_url+'/login'
 
             login_handler_args = handler_args.copy()
             if not os.environ.get('CI_TESTING', None):
                 login_handler_args['oauth_client_id'] = self.cfg['rest_api']['oauth_client_id']
                 login_handler_args['oauth_client_secret'] = self.cfg['rest_api']['oauth_client_secret']
                 login_handler_args['oauth_client_scope'] = 'offline_access posix profile'
 
             handler_args.update({
                 'cfg': self.cfg,
                 'modules': self.modules,
                 'statsd': self.statsd,
                 'rest_api': rest_address,
-                'module_rest_client': self.rest_client,
             })
             if 'debug' in self.cfg['webserver'] and self.cfg['webserver']['debug']:
                 handler_args['debug'] = True
             if 'cookie_secret' in self.cfg['webserver']:
                 cookie_secret = self.cfg['webserver']['cookie_secret']
                 logger.info('using supplied cookie secret %r', cookie_secret)
             else:
                 cookie_secret = ''.join(hex(random.randint(0,15))[-1] for _ in range(64))
                 self.cfg['webserver']['cookie_secret'] = cookie_secret
 
-            full_url = self.cfg['webserver'].get('full_url', '')
-            handler_args['full_url'] = full_url
-            login_url = full_url+'/login'
-
             routes = [
                 (r"/", Default, handler_args),
                 (r"/submit", Submit, handler_args),
                 (r"/config", Config, handler_args),
                 (r"/dataset", DatasetBrowse, handler_args),
                 (r"/dataset/(\w+)", Dataset, handler_args),
                 (r"/dataset/(\w+)/task", TaskBrowse, handler_args),
@@ -248,15 +255,15 @@
         """Get the current user, and set auth-related attributes."""
         try:
             username = self.get_secure_cookie('iceprod_username')
             if not username:
                 return None
             if isinstance(username, bytes):
                 username = username.decode('utf-8')
-            creds = await self.module_rest_client.request('GET', f'/users/{username}/credentials')
+            creds = await self.cred_rest_client.request('GET', f'/users/{username}/credentials', {'url': self.full_url})
             cred = creds[self.full_url]
             access_token = cred['access_token']
             try:
                 data = self.auth.validate(access_token)
             except jwt.ExpiredSignatureError:
                 logger.debug('user access_token expired')
                 return None
@@ -297,65 +304,64 @@
             access_token (str): jwt access token
             access_token_exp (int): access token expiration in seconds
             refresh_token (str): jwt refresh token
             refresh_token_exp (int): refresh token expiration in seconds
             user_info (dict): user info (from id token or user info lookup)
             user_info_exp (int): user info expiration in seconds
         """
-        if user_info:
-            username = user_info['username']
-        else:
-            data = self.auth.validate(access_token)
-            username = data.get('preferred_username')
-            if not username:
-                username = data.get('upn')
-            if not username:
-                raise tornado.web.HTTPError(400, reason='no username in token')
+        if not user_info:
+            user_info = self.auth.validate(access_token)
+        username = user_info.get('preferred_username')
+        if not username:
+            username = user_info.get('upn')
+        if not username:
+            raise tornado.web.HTTPError(400, reason='no username in token')
         args = {
             'url': self.full_url,
             'type': 'oauth',
             'access_token': access_token,
         }
         if refresh_token:
             args['refresh_token'] = refresh_token
 
-        self.module_rest_client.request_seq('POST', f'/users/{username}/credentials', args)
+        self.cred_rest_client.request_seq('POST', f'/users/{username}/credentials', args)
 
         self.set_secure_cookie('iceprod_username', username, expires_days=30)
 
     def clear_tokens(self):
         """
         Clear token data, usually on logout.
         """
         self.clear_cookie('iceprod_username')
 
 
 class Login(TokenStorageMixin, OpenIDLoginHandler):
-    def initialize(self, module_rest_client=None, **kwargs):
+    def initialize(self, cred_rest_client=None, full_url=None, **kwargs):
         super().initialize(**kwargs)
-        self.module_rest_client = module_rest_client
+        self.cred_rest_client = cred_rest_client
+        self.full_url = full_url
 
 
 class PublicHandler(TokenStorageMixin, RestHandler):
     """Default Handler"""
-    def initialize(self, cfg=None, modules=None, statsd=None, rest_api=None, module_rest_client=None, full_url=None, **kwargs):
+    def initialize(self, cfg=None, modules=None, statsd=None, rest_api=None, cred_rest_client=None, full_url=None, **kwargs):
         """
         Get some params from the website module
 
         :param cfg: the global config
         :param modules: modules handle
         :param statsd: statsd client
         :param rest_api: the rest api url
         """
         super().initialize(**kwargs)
         self.cfg = cfg
         self.modules = modules
         self.statsd = statsd
         self.rest_api = rest_api
-        self.module_rest_client = module_rest_client
+        self.cred_rest_client = cred_rest_client
         self.rest_client = None
         self.full_url = full_url
 
     def get_template_namespace(self):
         namespace = super().get_template_namespace()
         namespace['version'] = iceprod.__version__
         namespace['section'] = self.request.uri.lstrip('/').split('?')[0].split('/')[0]
@@ -702,14 +708,15 @@
             args = {
                 'url': 'https://data.icecube.aq',
                 'type': 'oauth',
                 'access_token': self.auth_access_token,
             }
             if self.auth_refresh_token:
                 args['refresh_token'] = self.auth_refresh_token
+                args['expiration'] = (datetime.utcnow() + timedelta(days=30)).isoformat()
             await self.rest_client.request('POST', f'/users/{username}/credentials', args)
 
         else:
             type_ = self.get_argument('type')
             args = {
                 'url': self.get_argument('url'),
                 'type': type_,
```

### Comparing `iceprod-2.6.8/iceprod/server/plugins/condor.py` & `iceprod-2.6.9/iceprod/server/plugins/condor.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.8/iceprod/server/plugins/condor_direct.py` & `iceprod-2.6.9/iceprod/server/plugins/condor_direct.py`

 * *Files 0% similar despite different names*

```diff
@@ -742,17 +742,14 @@
 
     async def download_input(self, task):
         pass
 
     async def upload_output(self, task):
         pass
 
-    async def customize_task_config(self, task_cfg):
-        pass
-
     async def generate_submit_file(self, task, cfg=None, passkey=None,
                                    filelist=None):
         """Generate queueing system submit file for task in dir."""
         args = self.get_submit_args(task,cfg=cfg)
         args.extend(['--offline', '--offline_transfer', 'True', '--gzip-logs'])
 
         # get requirements and batchopts
```

### Comparing `iceprod-2.6.8/iceprod/server/plugins/condor_file_transfer.py` & `iceprod-2.6.9/iceprod/server/plugins/condor_file_transfer.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.8/iceprod/server/plugins/sc_demo.py` & `iceprod-2.6.9/iceprod/server/plugins/sc_demo.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.8/iceprod/server/plugins/supercomp_cedar.py` & `iceprod-2.6.9/iceprod/server/plugins/supercomp_cedar.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.8/iceprod/server/plugins/supercomp_graham.py` & `iceprod-2.6.9/iceprod/server/plugins/supercomp_graham.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.8/iceprod/server/priority.py` & `iceprod-2.6.9/iceprod/server/priority.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.8/iceprod/server/scheduled_tasks/buffer_jobs_tasks.py` & `iceprod-2.6.9/iceprod/server/scheduled_tasks/buffer_jobs_tasks.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.8/iceprod/server/scheduled_tasks/dataset_cleanup.py` & `iceprod-2.6.9/iceprod/server/scheduled_tasks/dataset_cleanup.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.8/iceprod/server/scheduled_tasks/dataset_completion.py` & `iceprod-2.6.9/iceprod/server/scheduled_tasks/dataset_completion.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.8/iceprod/server/scheduled_tasks/dataset_monitor.py` & `iceprod-2.6.9/iceprod/server/scheduled_tasks/dataset_monitor.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.8/iceprod/server/scheduled_tasks/job_completion.py` & `iceprod-2.6.9/iceprod/server/scheduled_tasks/job_completion.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.8/iceprod/server/scheduled_tasks/job_temp_cleaning.py` & `iceprod-2.6.9/iceprod/server/scheduled_tasks/job_temp_cleaning.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.8/iceprod/server/scheduled_tasks/log_cleanup.py` & `iceprod-2.6.9/iceprod/server/scheduled_tasks/log_cleanup.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.8/iceprod/server/scheduled_tasks/non_active_tasks.py` & `iceprod-2.6.9/iceprod/server/scheduled_tasks/non_active_tasks.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.8/iceprod/server/scheduled_tasks/pilot_cleanup.py` & `iceprod-2.6.9/iceprod/server/scheduled_tasks/pilot_cleanup.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.8/iceprod/server/scheduled_tasks/pilot_monitor.py` & `iceprod-2.6.9/iceprod/server/scheduled_tasks/pilot_monitor.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.8/iceprod/server/scheduled_tasks/queue_tasks.py` & `iceprod-2.6.9/iceprod/server/scheduled_tasks/queue_tasks.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.8/iceprod/server/scheduled_tasks/removed_tasks.py` & `iceprod-2.6.9/iceprod/server/scheduled_tasks/removed_tasks.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.8/iceprod/server/scheduled_tasks/reset_tasks.py` & `iceprod-2.6.9/iceprod/server/scheduled_tasks/reset_tasks.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.8/iceprod/server/scheduled_tasks/update_task_priority.py` & `iceprod-2.6.9/iceprod/server/scheduled_tasks/update_task_priority.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.8/iceprod/server/server.py` & `iceprod-2.6.9/iceprod/server/server.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.8/iceprod/server/ssl_cert.py` & `iceprod-2.6.9/iceprod/server/ssl_cert.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.8/iceprod/server/task_queue.py` & `iceprod-2.6.9/iceprod/server/task_queue.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.8/iceprod/server/util.py` & `iceprod-2.6.9/iceprod/server/util.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.8/iceprod.egg-info/PKG-INFO` & `iceprod-2.6.9/iceprod.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iceprod
-Version: 2.6.8
+Version: 2.6.9
 Summary: IceCube dataset management system
 Home-page: https://github.com/WIPACrepo/iceprod
 Download-URL: https://pypi.org/project/iceprod/
 Author: WIPAC Developers
 Author-email: developers@icecube.wisc.edu
 License: MIT
 Project-URL: Tracker, https://github.com/WIPACrepo/iceprod/issues
```

### Comparing `iceprod-2.6.8/iceprod.egg-info/SOURCES.txt` & `iceprod-2.6.9/iceprod.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -34,29 +34,32 @@
 iceprod/core/jsonUtil.py
 iceprod/core/logger.py
 iceprod/core/parser.py
 iceprod/core/pilot.py
 iceprod/core/resources.py
 iceprod/core/serialization.py
 iceprod/core/util.py
+iceprod/credentials/__init__.py
+iceprod/credentials/__main__.py
+iceprod/credentials/server.py
+iceprod/credentials/service.py
 iceprod/materialization/__init__.py
 iceprod/materialization/__main__.py
 iceprod/materialization/materialize.py
 iceprod/materialization/server.py
 iceprod/materialization/service.py
 iceprod/modules/__init__.py
 iceprod/rest/__init__.py
 iceprod/rest/__main__.py
 iceprod/rest/auth.py
 iceprod/rest/base_handler.py
 iceprod/rest/server.py
 iceprod/rest/handlers/__init__.py
 iceprod/rest/handlers/auth.py
 iceprod/rest/handlers/config.py
-iceprod/rest/handlers/credentials.py
 iceprod/rest/handlers/datasets.py
 iceprod/rest/handlers/grids.py
 iceprod/rest/handlers/jobs.py
 iceprod/rest/handlers/logs.py
 iceprod/rest/handlers/pilots.py
 iceprod/rest/handlers/task_stats.py
 iceprod/rest/handlers/tasks.py
```

### Comparing `iceprod-2.6.8/setup.cfg` & `iceprod-2.6.9/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -31,27 +31,29 @@
 	Tracker = https://github.com/WIPACrepo/iceprod/issues
 	Source = https://github.com/WIPACrepo/iceprod
 
 [semantic_release]
 version_variable = iceprod/__init__.py:__version__
 upload_to_pypi = True
 patch_without_tag = True
-commit_parser = semantic_release.history.tag_parser
-minor_tag = [minor]
-fix_tag = [fix]
+commit_parser = semantic_release.history.emoji_parser
+major_emoji = [major]
+minor_emoji = [minor]
+patch_emoji = [fix], [patch]
 branch = master
 
 [options]
 install_requires = 
 	PyYAML
 	asyncache
 	boto3
 	cachetools
 	certifi
 	cryptography
+	httpx
 	ldap3
 	motor
 	psutil
 	pyOpenSSL
 	pymongo
 	python-dateutil
 	requests
@@ -68,15 +70,14 @@
 
 [options.extras_require]
 tests = 
 	beautifulsoup4
 	coverage
 	flake8
 	flexmock
-	httpx
 	mock
 	moto
 	pytest
 	pytest-asyncio
 	pytest-cov
 	pytest-mock
 	requests-mock
```

