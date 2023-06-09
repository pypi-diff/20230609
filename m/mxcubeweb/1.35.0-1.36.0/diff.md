# Comparing `tmp/mxcubeweb-1.35.0.tar.gz` & `tmp/mxcubeweb-1.36.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mxcubeweb-1.35.0.tar", max compression
+gzip compressed data, was "mxcubeweb-1.36.0.tar", max compression
```

## Comparing `mxcubeweb-1.35.0.tar` & `mxcubeweb-1.36.0.tar`

### file list

```diff
@@ -1,67 +1,69 @@
--rw-r--r--   0        0        0     7652 2023-06-08 15:07:45.217556 mxcubeweb-1.35.0/LICENSE
--rw-r--r--   0        0        0     3638 2023-06-08 15:07:45.217556 mxcubeweb-1.35.0/README.md
--rw-r--r--   0        0        0     3584 2023-06-08 15:07:45.221557 mxcubeweb-1.35.0/mxcube3/__init__.py
--rw-r--r--   0        0        0    17723 2023-06-08 15:07:45.221557 mxcubeweb-1.35.0/mxcube3/app.py
--rw-r--r--   0        0        0     1409 2023-06-08 15:07:45.221557 mxcubeweb-1.35.0/mxcube3/config.py
--rw-r--r--   0        0        0        0 2023-06-08 15:07:45.221557 mxcubeweb-1.35.0/mxcube3/core/__init__.py
--rw-r--r--   0        0        0        0 2023-06-08 15:07:45.221557 mxcubeweb-1.35.0/mxcube3/core/adapter/__init__.py
--rw-r--r--   0        0        0     2408 2023-06-08 15:07:45.221557 mxcubeweb-1.35.0/mxcube3/core/adapter/actuator_adapter.py
--rw-r--r--   0        0        0    13582 2023-06-08 15:07:45.221557 mxcubeweb-1.35.0/mxcube3/core/adapter/adapter_base.py
--rw-r--r--   0        0        0     1846 2023-06-08 15:07:45.221557 mxcubeweb-1.35.0/mxcube3/core/adapter/beam_adapter.py
--rw-r--r--   0        0        0     1642 2023-06-08 15:07:45.221557 mxcubeweb-1.35.0/mxcube3/core/adapter/beamline_action_adapter.py
--rw-r--r--   0        0        0     2689 2023-06-08 15:07:45.221557 mxcubeweb-1.35.0/mxcube3/core/adapter/beamline_adapter.py
--rw-r--r--   0        0        0     1586 2023-06-08 15:07:45.221557 mxcubeweb-1.35.0/mxcube3/core/adapter/data_publisher_adapter.py
--rw-r--r--   0        0        0      494 2023-06-08 15:07:45.221557 mxcubeweb-1.35.0/mxcube3/core/adapter/detector_adapter.py
--rw-r--r--   0        0        0      988 2023-06-08 15:07:45.221557 mxcubeweb-1.35.0/mxcube3/core/adapter/diffractometer_adapter.py
--rw-r--r--   0        0        0      591 2023-06-08 15:07:45.221557 mxcubeweb-1.35.0/mxcube3/core/adapter/energy_adapter.py
--rw-r--r--   0        0        0     1384 2023-06-08 15:07:45.221557 mxcubeweb-1.35.0/mxcube3/core/adapter/flux_adapter.py
--rw-r--r--   0        0        0     2111 2023-06-08 15:07:45.221557 mxcubeweb-1.35.0/mxcube3/core/adapter/machine_info_adapter.py
--rw-r--r--   0        0        0     2218 2023-06-08 15:07:45.221557 mxcubeweb-1.35.0/mxcube3/core/adapter/motor_adapter.py
--rw-r--r--   0        0        0     1763 2023-06-08 15:07:45.221557 mxcubeweb-1.35.0/mxcube3/core/adapter/nstate_adapter.py
--rw-r--r--   0        0        0     2905 2023-06-08 15:07:45.221557 mxcubeweb-1.35.0/mxcube3/core/adapter/wavelength_adapter.py
--rw-r--r--   0        0        0    12293 2023-06-08 15:07:45.221557 mxcubeweb-1.35.0/mxcube3/core/components/beamline.py
--rw-r--r--   0        0        0     1384 2023-06-08 15:07:45.221557 mxcubeweb-1.35.0/mxcube3/core/components/chat.py
--rw-r--r--   0        0        0      630 2023-06-08 15:07:45.221557 mxcubeweb-1.35.0/mxcube3/core/components/component_base.py
--rw-r--r--   0        0        0    16902 2023-06-08 15:07:45.221557 mxcubeweb-1.35.0/mxcube3/core/components/lims.py
--rw-r--r--   0        0        0    90181 2023-06-08 15:07:45.221557 mxcubeweb-1.35.0/mxcube3/core/components/queue.py
--rw-r--r--   0        0        0    18591 2023-06-08 15:07:45.221557 mxcubeweb-1.35.0/mxcube3/core/components/samplechanger.py
--rw-r--r--   0        0        0    22573 2023-06-08 15:07:45.221557 mxcubeweb-1.35.0/mxcube3/core/components/sampleview.py
--rw-r--r--   0        0        0     1896 2023-06-08 15:07:45.221557 mxcubeweb-1.35.0/mxcube3/core/components/user/database.py
--rw-r--r--   0        0        0      418 2023-06-08 15:07:45.221557 mxcubeweb-1.35.0/mxcube3/core/components/user/dummyusermanager.py
--rw-r--r--   0        0        0    15081 2023-06-08 15:07:45.221557 mxcubeweb-1.35.0/mxcube3/core/components/user/usermanager.py
--rw-r--r--   0        0        0     1986 2023-06-08 15:07:45.221557 mxcubeweb-1.35.0/mxcube3/core/components/workflow.py
--rw-r--r--   0        0        0     2344 2023-06-08 15:07:45.221557 mxcubeweb-1.35.0/mxcube3/core/models/adaptermodels.py
--rw-r--r--   0        0        0     2689 2023-06-08 15:07:45.221557 mxcubeweb-1.35.0/mxcube3/core/models/configmodels.py
--rw-r--r--   0        0        0      254 2023-06-08 15:07:45.221557 mxcubeweb-1.35.0/mxcube3/core/models/generic.py
--rw-r--r--   0        0        0     3359 2023-06-08 15:07:45.221557 mxcubeweb-1.35.0/mxcube3/core/models/usermodels.py
--rw-r--r--   0        0        0     2344 2023-06-08 15:07:45.221557 mxcubeweb-1.35.0/mxcube3/core/util/adapterutils.py
--rw-r--r--   0        0        0     1630 2023-06-08 15:07:45.221557 mxcubeweb-1.35.0/mxcube3/core/util/convertutils.py
--rw-r--r--   0        0        0      523 2023-06-08 15:07:45.221557 mxcubeweb-1.35.0/mxcube3/core/util/fsutils.py
--rw-r--r--   0        0        0     4507 2023-06-08 15:07:45.221557 mxcubeweb-1.35.0/mxcube3/core/util/networkutils.py
--rw-r--r--   0        0        0     1188 2023-06-08 15:07:45.221557 mxcubeweb-1.35.0/mxcube3/logging_handler.py
--rw-r--r--   0        0        0        0 2023-06-08 15:07:45.221557 mxcubeweb-1.35.0/mxcube3/routes/__init__.py
--rw-r--r--   0        0        0     8128 2023-06-08 15:07:45.221557 mxcubeweb-1.35.0/mxcube3/routes/beamline.py
--rw-r--r--   0        0        0      859 2023-06-08 15:07:45.221557 mxcubeweb-1.35.0/mxcube3/routes/detector.py
--rw-r--r--   0        0        0     4033 2023-06-08 15:07:45.221557 mxcubeweb-1.35.0/mxcube3/routes/diffractometer.py
--rw-r--r--   0        0        0     5165 2023-06-08 15:07:45.221557 mxcubeweb-1.35.0/mxcube3/routes/lims.py
--rw-r--r--   0        0        0      563 2023-06-08 15:07:45.221557 mxcubeweb-1.35.0/mxcube3/routes/log.py
--rw-r--r--   0        0        0     3235 2023-06-08 15:07:45.221557 mxcubeweb-1.35.0/mxcube3/routes/login.py
--rw-r--r--   0        0        0     2613 2023-06-08 15:07:45.221557 mxcubeweb-1.35.0/mxcube3/routes/main.py
--rw-r--r--   0        0        0     4291 2023-06-08 15:07:45.221557 mxcubeweb-1.35.0/mxcube3/routes/mockups.py
--rw-r--r--   0        0        0    10369 2023-06-08 15:07:45.221557 mxcubeweb-1.35.0/mxcube3/routes/queue.py
--rw-r--r--   0        0        0     6224 2023-06-08 15:07:45.221557 mxcubeweb-1.35.0/mxcube3/routes/ra.py
--rw-r--r--   0        0        0    13766 2023-06-08 15:07:45.221557 mxcubeweb-1.35.0/mxcube3/routes/samplecentring.py
--rw-r--r--   0        0        0     4671 2023-06-08 15:07:45.221557 mxcubeweb-1.35.0/mxcube3/routes/samplechanger.py
--rw-r--r--   0        0        0    20592 2023-06-08 15:07:45.221557 mxcubeweb-1.35.0/mxcube3/routes/signals.py
--rw-r--r--   0        0        0     1125 2023-06-08 15:07:45.221557 mxcubeweb-1.35.0/mxcube3/routes/workflow.py
--rw-r--r--   0        0        0     6709 2023-06-08 15:07:45.221557 mxcubeweb-1.35.0/mxcube3/server.py
--rw-r--r--   0        0        0     1396 2023-06-08 15:07:45.221557 mxcubeweb-1.35.0/mxcube3/state_storage.py
--rw-r--r--   0        0        0      771 2023-06-08 15:07:45.221557 mxcubeweb-1.35.0/mxcube3/templates/characterisation-results.js
--rw-r--r--   0        0        0     3610 2023-06-08 15:07:45.221557 mxcubeweb-1.35.0/mxcube3/templates/data-collection-results.html
--rw-r--r--   0        0        0   329138 2023-06-08 15:07:45.225558 mxcubeweb-1.35.0/mxcube3/templates/precompiled.templates.min.js
--rw-r--r--   0        0        0      721 2023-06-08 15:07:45.225558 mxcubeweb-1.35.0/mxcube3/templates/workflow-results.js
--rw-r--r--   0        0        0       22 2023-06-08 15:07:45.225558 mxcubeweb-1.35.0/mxcube3/version.py
--rw-r--r--   0        0        0        0 2023-06-08 15:07:45.225558 mxcubeweb-1.35.0/mxcube3/video/__init__.py
--rw-r--r--   0        0        0     2647 2023-06-08 15:07:45.225558 mxcubeweb-1.35.0/mxcube3/video/websocket-relay.js
--rw-r--r--   0        0        0     1785 2023-06-08 15:08:01.033923 mxcubeweb-1.35.0/pyproject.toml
--rw-r--r--   0        0        0     5484 1970-01-01 00:00:00.000000 mxcubeweb-1.35.0/PKG-INFO
+-rw-r--r--   0        0        0     7652 2023-06-09 11:52:46.604171 mxcubeweb-1.36.0/LICENSE
+-rw-r--r--   0        0        0     3638 2023-06-09 11:52:46.604171 mxcubeweb-1.36.0/README.md
+-rw-r--r--   0        0        0     3584 2023-06-09 11:52:46.608173 mxcubeweb-1.36.0/mxcube3/__init__.py
+-rw-r--r--   0        0        0    17864 2023-06-09 11:52:46.608173 mxcubeweb-1.36.0/mxcube3/app.py
+-rw-r--r--   0        0        0     1409 2023-06-09 11:52:46.608173 mxcubeweb-1.36.0/mxcube3/config.py
+-rw-r--r--   0        0        0        0 2023-06-09 11:52:46.608173 mxcubeweb-1.36.0/mxcube3/core/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-09 11:52:46.608173 mxcubeweb-1.36.0/mxcube3/core/adapter/__init__.py
+-rw-r--r--   0        0        0     2408 2023-06-09 11:52:46.608173 mxcubeweb-1.36.0/mxcube3/core/adapter/actuator_adapter.py
+-rw-r--r--   0        0        0    13582 2023-06-09 11:52:46.608173 mxcubeweb-1.36.0/mxcube3/core/adapter/adapter_base.py
+-rw-r--r--   0        0        0     1846 2023-06-09 11:52:46.608173 mxcubeweb-1.36.0/mxcube3/core/adapter/beam_adapter.py
+-rw-r--r--   0        0        0     1642 2023-06-09 11:52:46.608173 mxcubeweb-1.36.0/mxcube3/core/adapter/beamline_action_adapter.py
+-rw-r--r--   0        0        0     3095 2023-06-09 11:52:46.608173 mxcubeweb-1.36.0/mxcube3/core/adapter/beamline_adapter.py
+-rw-r--r--   0        0        0     1586 2023-06-09 11:52:46.608173 mxcubeweb-1.36.0/mxcube3/core/adapter/data_publisher_adapter.py
+-rw-r--r--   0        0        0      494 2023-06-09 11:52:46.608173 mxcubeweb-1.36.0/mxcube3/core/adapter/detector_adapter.py
+-rw-r--r--   0        0        0      988 2023-06-09 11:52:46.608173 mxcubeweb-1.36.0/mxcube3/core/adapter/diffractometer_adapter.py
+-rw-r--r--   0        0        0      591 2023-06-09 11:52:46.608173 mxcubeweb-1.36.0/mxcube3/core/adapter/energy_adapter.py
+-rw-r--r--   0        0        0     1384 2023-06-09 11:52:46.608173 mxcubeweb-1.36.0/mxcube3/core/adapter/flux_adapter.py
+-rw-r--r--   0        0        0     2111 2023-06-09 11:52:46.608173 mxcubeweb-1.36.0/mxcube3/core/adapter/machine_info_adapter.py
+-rw-r--r--   0        0        0     2218 2023-06-09 11:52:46.608173 mxcubeweb-1.36.0/mxcube3/core/adapter/motor_adapter.py
+-rw-r--r--   0        0        0     1763 2023-06-09 11:52:46.608173 mxcubeweb-1.36.0/mxcube3/core/adapter/nstate_adapter.py
+-rw-r--r--   0        0        0     2905 2023-06-09 11:52:46.608173 mxcubeweb-1.36.0/mxcube3/core/adapter/wavelength_adapter.py
+-rw-r--r--   0        0        0    12293 2023-06-09 11:52:46.608173 mxcubeweb-1.36.0/mxcube3/core/components/beamline.py
+-rw-r--r--   0        0        0     1384 2023-06-09 11:52:46.608173 mxcubeweb-1.36.0/mxcube3/core/components/chat.py
+-rw-r--r--   0        0        0      630 2023-06-09 11:52:46.608173 mxcubeweb-1.36.0/mxcube3/core/components/component_base.py
+-rw-r--r--   0        0        0     1246 2023-06-09 11:52:46.608173 mxcubeweb-1.36.0/mxcube3/core/components/gphl_workflow.py
+-rw-r--r--   0        0        0    16902 2023-06-09 11:52:46.608173 mxcubeweb-1.36.0/mxcube3/core/components/lims.py
+-rw-r--r--   0        0        0    90191 2023-06-09 11:52:46.608173 mxcubeweb-1.36.0/mxcube3/core/components/queue.py
+-rw-r--r--   0        0        0    18591 2023-06-09 11:52:46.608173 mxcubeweb-1.36.0/mxcube3/core/components/samplechanger.py
+-rw-r--r--   0        0        0    22573 2023-06-09 11:52:46.608173 mxcubeweb-1.36.0/mxcube3/core/components/sampleview.py
+-rw-r--r--   0        0        0     1896 2023-06-09 11:52:46.608173 mxcubeweb-1.36.0/mxcube3/core/components/user/database.py
+-rw-r--r--   0        0        0      418 2023-06-09 11:52:46.608173 mxcubeweb-1.36.0/mxcube3/core/components/user/dummyusermanager.py
+-rw-r--r--   0        0        0    15081 2023-06-09 11:52:46.608173 mxcubeweb-1.36.0/mxcube3/core/components/user/usermanager.py
+-rw-r--r--   0        0        0     1986 2023-06-09 11:52:46.608173 mxcubeweb-1.36.0/mxcube3/core/components/workflow.py
+-rw-r--r--   0        0        0     2344 2023-06-09 11:52:46.608173 mxcubeweb-1.36.0/mxcube3/core/models/adaptermodels.py
+-rw-r--r--   0        0        0     2689 2023-06-09 11:52:46.608173 mxcubeweb-1.36.0/mxcube3/core/models/configmodels.py
+-rw-r--r--   0        0        0      254 2023-06-09 11:52:46.608173 mxcubeweb-1.36.0/mxcube3/core/models/generic.py
+-rw-r--r--   0        0        0     3359 2023-06-09 11:52:46.608173 mxcubeweb-1.36.0/mxcube3/core/models/usermodels.py
+-rw-r--r--   0        0        0     2344 2023-06-09 11:52:46.608173 mxcubeweb-1.36.0/mxcube3/core/util/adapterutils.py
+-rw-r--r--   0        0        0     1630 2023-06-09 11:52:46.608173 mxcubeweb-1.36.0/mxcube3/core/util/convertutils.py
+-rw-r--r--   0        0        0      523 2023-06-09 11:52:46.608173 mxcubeweb-1.36.0/mxcube3/core/util/fsutils.py
+-rw-r--r--   0        0        0     4507 2023-06-09 11:52:46.608173 mxcubeweb-1.36.0/mxcube3/core/util/networkutils.py
+-rw-r--r--   0        0        0     1188 2023-06-09 11:52:46.608173 mxcubeweb-1.36.0/mxcube3/logging_handler.py
+-rw-r--r--   0        0        0        0 2023-06-09 11:52:46.608173 mxcubeweb-1.36.0/mxcube3/routes/__init__.py
+-rw-r--r--   0        0        0     8128 2023-06-09 11:52:46.608173 mxcubeweb-1.36.0/mxcube3/routes/beamline.py
+-rw-r--r--   0        0        0      859 2023-06-09 11:52:46.608173 mxcubeweb-1.36.0/mxcube3/routes/detector.py
+-rw-r--r--   0        0        0     4033 2023-06-09 11:52:46.608173 mxcubeweb-1.36.0/mxcube3/routes/diffractometer.py
+-rw-r--r--   0        0        0      587 2023-06-09 11:52:46.608173 mxcubeweb-1.36.0/mxcube3/routes/gphl_workflow.py
+-rw-r--r--   0        0        0     5165 2023-06-09 11:52:46.608173 mxcubeweb-1.36.0/mxcube3/routes/lims.py
+-rw-r--r--   0        0        0      563 2023-06-09 11:52:46.608173 mxcubeweb-1.36.0/mxcube3/routes/log.py
+-rw-r--r--   0        0        0     3235 2023-06-09 11:52:46.608173 mxcubeweb-1.36.0/mxcube3/routes/login.py
+-rw-r--r--   0        0        0     2613 2023-06-09 11:52:46.608173 mxcubeweb-1.36.0/mxcube3/routes/main.py
+-rw-r--r--   0        0        0     4291 2023-06-09 11:52:46.608173 mxcubeweb-1.36.0/mxcube3/routes/mockups.py
+-rw-r--r--   0        0        0    10369 2023-06-09 11:52:46.608173 mxcubeweb-1.36.0/mxcube3/routes/queue.py
+-rw-r--r--   0        0        0     6224 2023-06-09 11:52:46.608173 mxcubeweb-1.36.0/mxcube3/routes/ra.py
+-rw-r--r--   0        0        0    13766 2023-06-09 11:52:46.608173 mxcubeweb-1.36.0/mxcube3/routes/samplecentring.py
+-rw-r--r--   0        0        0     4671 2023-06-09 11:52:46.608173 mxcubeweb-1.36.0/mxcube3/routes/samplechanger.py
+-rw-r--r--   0        0        0    20592 2023-06-09 11:52:46.608173 mxcubeweb-1.36.0/mxcube3/routes/signals.py
+-rw-r--r--   0        0        0     1125 2023-06-09 11:52:46.608173 mxcubeweb-1.36.0/mxcube3/routes/workflow.py
+-rw-r--r--   0        0        0     6921 2023-06-09 11:52:46.612176 mxcubeweb-1.36.0/mxcube3/server.py
+-rw-r--r--   0        0        0     1396 2023-06-09 11:52:46.612176 mxcubeweb-1.36.0/mxcube3/state_storage.py
+-rw-r--r--   0        0        0      771 2023-06-09 11:52:46.612176 mxcubeweb-1.36.0/mxcube3/templates/characterisation-results.js
+-rw-r--r--   0        0        0     3610 2023-06-09 11:52:46.612176 mxcubeweb-1.36.0/mxcube3/templates/data-collection-results.html
+-rw-r--r--   0        0        0   329138 2023-06-09 11:52:46.612176 mxcubeweb-1.36.0/mxcube3/templates/precompiled.templates.min.js
+-rw-r--r--   0        0        0      721 2023-06-09 11:52:46.612176 mxcubeweb-1.36.0/mxcube3/templates/workflow-results.js
+-rw-r--r--   0        0        0       22 2023-06-09 11:52:46.612176 mxcubeweb-1.36.0/mxcube3/version.py
+-rw-r--r--   0        0        0        0 2023-06-09 11:52:46.612176 mxcubeweb-1.36.0/mxcube3/video/__init__.py
+-rw-r--r--   0        0        0     2647 2023-06-09 11:52:46.612176 mxcubeweb-1.36.0/mxcube3/video/websocket-relay.js
+-rw-r--r--   0        0        0     1785 2023-06-09 11:53:05.193511 mxcubeweb-1.36.0/pyproject.toml
+-rw-r--r--   0        0        0     5484 1970-01-01 00:00:00.000000 mxcubeweb-1.36.0/PKG-INFO
```

### Comparing `mxcubeweb-1.35.0/LICENSE` & `mxcubeweb-1.36.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.35.0/README.md` & `mxcubeweb-1.36.0/README.md`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.35.0/mxcube3/__init__.py` & `mxcubeweb-1.36.0/mxcube3/__init__.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.35.0/mxcube3/app.py` & `mxcubeweb-1.36.0/mxcube3/app.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 from mxcube3.core.components.lims import Lims
 from mxcube3.core.components.chat import Chat
 from mxcube3.core.components.samplechanger import SampleChanger
 from mxcube3.core.components.beamline import Beamline
 from mxcube3.core.components.sampleview import SampleView
 from mxcube3.core.components.queue import Queue
 from mxcube3.core.components.workflow import Workflow
+from mxcube3.core.components.gphl_workflow import GphlWorkflow
 
 
 removeLoggingHandlers()
 
 
 class MXCUBECore:
     # The HardwareRepository object
@@ -282,14 +283,15 @@
             MXCUBEApplication, cfg.app.usermanager
         )
         MXCUBEApplication.chat = Chat(MXCUBEApplication, {})
         MXCUBEApplication.sample_changer = SampleChanger(MXCUBEApplication, {})
         MXCUBEApplication.beamline = Beamline(MXCUBEApplication, {})
         MXCUBEApplication.sample_view = SampleView(MXCUBEApplication, {})
         MXCUBEApplication.workflow = Workflow(MXCUBEApplication, {})
+        MXCUBEApplication.gphl_workflow = GphlWorkflow(MXCUBEApplication, {})
 
         MXCUBEApplication.init_signal_handlers()
         atexit.register(MXCUBEApplication.app_atexit)
 
         # Install server-side UI state storage
         MXCUBEApplication.init_state_storage()
```

### Comparing `mxcubeweb-1.35.0/mxcube3/config.py` & `mxcubeweb-1.36.0/mxcube3/config.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.35.0/mxcube3/core/adapter/actuator_adapter.py` & `mxcubeweb-1.36.0/mxcube3/core/adapter/actuator_adapter.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.35.0/mxcube3/core/adapter/adapter_base.py` & `mxcubeweb-1.36.0/mxcube3/core/adapter/adapter_base.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.35.0/mxcube3/core/adapter/beam_adapter.py` & `mxcubeweb-1.36.0/mxcube3/core/adapter/beam_adapter.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.35.0/mxcube3/core/adapter/beamline_action_adapter.py` & `mxcubeweb-1.36.0/mxcube3/core/adapter/beamline_action_adapter.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.35.0/mxcube3/core/adapter/beamline_adapter.py` & `mxcubeweb-1.36.0/mxcube3/core/adapter/beamline_adapter.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,20 +25,32 @@
 
     def __init__(self, beamline_hwobj, app):
         self.app = app
         self._bl = beamline_hwobj
         self.adapter_dict = {}
 
         workflow = self._bl.workflow
-
         if workflow:
             workflow.connect("parametersNeeded", self.wf_parameters_needed)
 
+        gphl_workflow = self._bl.gphl_workflow
+        if gphl_workflow:
+            gphl_workflow.connect(
+                "gphlParametersNeeded", self.gphl_wf_parameters_needed
+            )
+
     def wf_parameters_needed(self, params):
-        self.app.server.emit("workflowParametersDialog", params, namespace="/hwr")
+        self.app.server.emit(
+            "workflowParametersDialog", params, broadcast=True, namespace="/hwr"
+        )
+
+    def gphl_wf_parameters_needed(self, params):
+        self.app.server.emit(
+            "gphlWorkflowParametersDialog", params, broadcast=True, namespace="/hwr"
+        )
 
     def get_object(self, name):
         return self.get_attr_from_path(name)
 
     def dict(self):
         """
         Build dictionary value-representation for each beamline attribute
```

### Comparing `mxcubeweb-1.35.0/mxcube3/core/adapter/data_publisher_adapter.py` & `mxcubeweb-1.36.0/mxcube3/core/adapter/data_publisher_adapter.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.35.0/mxcube3/core/adapter/diffractometer_adapter.py` & `mxcubeweb-1.36.0/mxcube3/core/adapter/diffractometer_adapter.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.35.0/mxcube3/core/adapter/energy_adapter.py` & `mxcubeweb-1.36.0/mxcube3/core/adapter/energy_adapter.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.35.0/mxcube3/core/adapter/flux_adapter.py` & `mxcubeweb-1.36.0/mxcube3/core/adapter/flux_adapter.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.35.0/mxcube3/core/adapter/machine_info_adapter.py` & `mxcubeweb-1.36.0/mxcube3/core/adapter/machine_info_adapter.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.35.0/mxcube3/core/adapter/motor_adapter.py` & `mxcubeweb-1.36.0/mxcube3/core/adapter/motor_adapter.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.35.0/mxcube3/core/adapter/nstate_adapter.py` & `mxcubeweb-1.36.0/mxcube3/core/adapter/nstate_adapter.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.35.0/mxcube3/core/adapter/wavelength_adapter.py` & `mxcubeweb-1.36.0/mxcube3/core/adapter/wavelength_adapter.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.35.0/mxcube3/core/components/beamline.py` & `mxcubeweb-1.36.0/mxcube3/core/components/beamline.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.35.0/mxcube3/core/components/chat.py` & `mxcubeweb-1.36.0/mxcube3/core/components/chat.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.35.0/mxcube3/core/components/component_base.py` & `mxcubeweb-1.36.0/mxcube3/core/components/component_base.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.35.0/mxcube3/core/components/lims.py` & `mxcubeweb-1.36.0/mxcube3/core/components/lims.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.35.0/mxcube3/core/components/queue.py` & `mxcubeweb-1.36.0/mxcube3/core/components/queue.py`

 * *Files 0% similar despite different names*

```diff
@@ -374,15 +374,15 @@
         return res
 
     def _handle_gphl_wf(self, sample_node, node, include_lims_data=False):
         pt = node.path_template
         parameters = pt.as_dict()
         parameters["path"] = parameters["directory"]
 
-        parameters["strategy_name"] = node.get_type()
+        parameters["strategy_name"] = node.strategy_name
         parameters["label"] = "GΦL " + parameters["strategy_name"]
         parameters["shape"] = node.shape
 
         queueID = node._node_id
         enabled, state = self.get_node_state(queueID)
 
         raw_data = HWR.beamline.session.raw_data_folder_name
@@ -2398,15 +2398,15 @@
         if not sample:
             msg = "[QUEUE] sample info could not be retrieved"
             logging.getLogger("MX3.HWR").error(msg)
 
         return sample
 
     def get_method(self, sample_id, method_id):
-        sample = self.queue_to_dict().get(int(id), None)
+        sample = self.queue_to_dict().get(int(sample_id), None)
 
         if not sample:
             msg = "[QUEUE] sample info could not be retrieved"
             logging.getLogger("MX3.HWR").error(msg)
             raise Exception(msg)
         else:
             # Find task with queue id method_id
```

### Comparing `mxcubeweb-1.35.0/mxcube3/core/components/samplechanger.py` & `mxcubeweb-1.36.0/mxcube3/core/components/samplechanger.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.35.0/mxcube3/core/components/sampleview.py` & `mxcubeweb-1.36.0/mxcube3/core/components/sampleview.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.35.0/mxcube3/core/components/user/database.py` & `mxcubeweb-1.36.0/mxcube3/core/components/user/database.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.35.0/mxcube3/core/components/user/usermanager.py` & `mxcubeweb-1.36.0/mxcube3/core/components/user/usermanager.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.35.0/mxcube3/core/components/workflow.py` & `mxcubeweb-1.36.0/mxcube3/core/components/workflow.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.35.0/mxcube3/core/models/adaptermodels.py` & `mxcubeweb-1.36.0/mxcube3/core/models/adaptermodels.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.35.0/mxcube3/core/models/configmodels.py` & `mxcubeweb-1.36.0/mxcube3/core/models/configmodels.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.35.0/mxcube3/core/models/usermodels.py` & `mxcubeweb-1.36.0/mxcube3/core/models/usermodels.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.35.0/mxcube3/core/util/adapterutils.py` & `mxcubeweb-1.36.0/mxcube3/core/util/adapterutils.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.35.0/mxcube3/core/util/convertutils.py` & `mxcubeweb-1.36.0/mxcube3/core/util/convertutils.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.35.0/mxcube3/core/util/fsutils.py` & `mxcubeweb-1.36.0/mxcube3/core/util/fsutils.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.35.0/mxcube3/core/util/networkutils.py` & `mxcubeweb-1.36.0/mxcube3/core/util/networkutils.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.35.0/mxcube3/logging_handler.py` & `mxcubeweb-1.36.0/mxcube3/logging_handler.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.35.0/mxcube3/routes/beamline.py` & `mxcubeweb-1.36.0/mxcube3/routes/beamline.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.35.0/mxcube3/routes/detector.py` & `mxcubeweb-1.36.0/mxcube3/routes/detector.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.35.0/mxcube3/routes/diffractometer.py` & `mxcubeweb-1.36.0/mxcube3/routes/diffractometer.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.35.0/mxcube3/routes/lims.py` & `mxcubeweb-1.36.0/mxcube3/routes/lims.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.35.0/mxcube3/routes/log.py` & `mxcubeweb-1.36.0/mxcube3/routes/log.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.35.0/mxcube3/routes/login.py` & `mxcubeweb-1.36.0/mxcube3/routes/login.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.35.0/mxcube3/routes/main.py` & `mxcubeweb-1.36.0/mxcube3/routes/main.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.35.0/mxcube3/routes/mockups.py` & `mxcubeweb-1.36.0/mxcube3/routes/mockups.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.35.0/mxcube3/routes/queue.py` & `mxcubeweb-1.36.0/mxcube3/routes/queue.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.35.0/mxcube3/routes/ra.py` & `mxcubeweb-1.36.0/mxcube3/routes/ra.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.35.0/mxcube3/routes/samplecentring.py` & `mxcubeweb-1.36.0/mxcube3/routes/samplecentring.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.35.0/mxcube3/routes/samplechanger.py` & `mxcubeweb-1.36.0/mxcube3/routes/samplechanger.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.35.0/mxcube3/routes/signals.py` & `mxcubeweb-1.36.0/mxcube3/routes/signals.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.35.0/mxcube3/routes/workflow.py` & `mxcubeweb-1.36.0/mxcube3/routes/workflow.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.35.0/mxcube3/server.py` & `mxcubeweb-1.36.0/mxcube3/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,14 +131,15 @@
         from mxcube3.routes.main import init_route as init_main_route
         from mxcube3.routes.mockups import init_route as init_mockups_route
         from mxcube3.routes.queue import init_route as init_queue_route
         from mxcube3.routes.ra import init_route as init_ra_route
         from mxcube3.routes.samplecentring import init_route as init_sampleview_route
         from mxcube3.routes.samplechanger import init_route as init_samplechanger_route
         from mxcube3.routes.workflow import init_route as init_workflow_route
+        from mxcube3.routes.gphl_workflow import init_route as init_gphl_workflow_route
 
         url_root_prefix = "/mxcube/api/v0.1"
 
         Server._register_route(
             init_beamline_route, mxcube, f"{url_root_prefix}/beamline"
         )
 
@@ -172,14 +173,18 @@
             init_samplechanger_route, mxcube, f"{url_root_prefix}/sample_changer"
         )
 
         Server._register_route(
             init_workflow_route, mxcube, f"{url_root_prefix}/workflow"
         )
 
+        Server._register_route(
+            init_gphl_workflow_route, mxcube, f"{url_root_prefix}/gphl_workflow"
+        )
+
         Server.security = flask_security.Security(
             Server.flask,
             Server.user_datastore
         )
 
     @staticmethod
     def emit(*args, **kwargs):
```

### Comparing `mxcubeweb-1.35.0/mxcube3/state_storage.py` & `mxcubeweb-1.36.0/mxcube3/state_storage.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.35.0/mxcube3/templates/characterisation-results.js` & `mxcubeweb-1.36.0/mxcube3/templates/characterisation-results.js`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.35.0/mxcube3/templates/data-collection-results.html` & `mxcubeweb-1.36.0/mxcube3/templates/data-collection-results.html`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.35.0/mxcube3/templates/precompiled.templates.min.js` & `mxcubeweb-1.36.0/mxcube3/templates/precompiled.templates.min.js`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.35.0/mxcube3/templates/workflow-results.js` & `mxcubeweb-1.36.0/mxcube3/templates/workflow-results.js`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.35.0/mxcube3/video/websocket-relay.js` & `mxcubeweb-1.36.0/mxcube3/video/websocket-relay.js`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.35.0/pyproject.toml` & `mxcubeweb-1.36.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mxcubeweb"
-version = "1.35.0"
+version = "1.36.0"
 license = "LGPL-3.0-or-later"
 description = "MXCuBE Web user interface"
 authors = ["The MXCuBE collaboration <mxcube@esrf.fr>"]
 maintainers = [
     "MXCuBE collaboration <mxcube@esrf.fr>",
 ]
 readme = "README.md"
```

### Comparing `mxcubeweb-1.35.0/PKG-INFO` & `mxcubeweb-1.36.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mxcubeweb
-Version: 1.35.0
+Version: 1.36.0
 Summary: MXCuBE Web user interface
 Home-page: http://github.com/mxcube/mxcubeweb
 License: LGPL-3.0-or-later
 Keywords: mxcube,mxcube3,mxcubeweb
 Author: The MXCuBE collaboration
 Author-email: mxcube@esrf.fr
 Maintainer: MXCuBE collaboration
```

