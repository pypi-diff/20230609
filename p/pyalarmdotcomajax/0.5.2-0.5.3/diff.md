# Comparing `tmp/pyalarmdotcomajax-0.5.2.tar.gz` & `tmp/pyalarmdotcomajax-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyalarmdotcomajax-0.5.2.tar", last modified: Thu Jun  1 16:05:14 2023, max compression
+gzip compressed data, was "pyalarmdotcomajax-0.5.3.tar", last modified: Fri Jun  9 01:22:03 2023, max compression
```

## Comparing `pyalarmdotcomajax-0.5.2.tar` & `pyalarmdotcomajax-0.5.3.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:05:14.499249 pyalarmdotcomajax-0.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-01 16:04:59.000000 pyalarmdotcomajax-0.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18038 2023-06-01 16:05:14.499249 pyalarmdotcomajax-0.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-06-01 16:04:59.000000 pyalarmdotcomajax-0.5.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:05:14.491249 pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/
--rw-r--r--   0 runner    (1001) docker     (123)    46790 2023-06-01 16:04:59.000000 pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-01 16:04:59.000000 pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20986 2023-06-01 16:04:59.000000 pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-01 16:04:59.000000 pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/const.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:05:14.495249 pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/devices/
--rw-r--r--   0 runner    (1001) docker     (123)    11965 2023-06-01 16:04:59.000000 pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-01 16:04:59.000000 pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/devices/camera.py
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-06-01 16:04:59.000000 pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/devices/garage_door.py
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-06-01 16:04:59.000000 pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/devices/gate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-06-01 16:04:59.000000 pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/devices/image_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-06-01 16:04:59.000000 pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/devices/light.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-01 16:04:59.000000 pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/devices/lock.py
--rw-r--r--   0 runner    (1001) docker     (123)     6557 2023-06-01 16:04:59.000000 pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/devices/partition.py
--rw-r--r--   0 runner    (1001) docker     (123)    14829 2023-06-01 16:04:59.000000 pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/devices/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-06-01 16:04:59.000000 pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/devices/sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-01 16:04:59.000000 pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/devices/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     7986 2023-06-01 16:04:59.000000 pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/devices/thermostat.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-01 16:04:59.000000 pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/devices/water_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-06-01 16:04:59.000000 pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    22829 2023-06-01 16:04:59.000000 pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-06-01 16:04:59.000000 pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:05:14.495249 pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/websockets/
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-01 16:04:59.000000 pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/websockets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8883 2023-06-01 16:04:59.000000 pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/websockets/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-06-01 16:04:59.000000 pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/websockets/const.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:05:14.499249 pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/websockets/handler/
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-06-01 16:04:59.000000 pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/websockets/handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-06-01 16:04:59.000000 pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/websockets/handler/garage_door.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-01 16:04:59.000000 pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/websockets/handler/gate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-06-01 16:04:59.000000 pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/websockets/handler/light.py
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-06-01 16:04:59.000000 pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/websockets/handler/lock.py
--rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-06-01 16:04:59.000000 pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/websockets/handler/partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-06-01 16:04:59.000000 pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/websockets/handler/sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-06-01 16:04:59.000000 pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/websockets/handler/thermostat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-06-01 16:04:59.000000 pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/websockets/handler/water_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5066 2023-06-01 16:04:59.000000 pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/websockets/messages.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:05:14.491249 pyalarmdotcomajax-0.5.2/pyalarmdotcomajax.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18038 2023-06-01 16:05:14.000000 pyalarmdotcomajax-0.5.2/pyalarmdotcomajax.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-06-01 16:05:14.000000 pyalarmdotcomajax-0.5.2/pyalarmdotcomajax.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 16:05:14.000000 pyalarmdotcomajax-0.5.2/pyalarmdotcomajax.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-01 16:05:14.000000 pyalarmdotcomajax-0.5.2/pyalarmdotcomajax.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-01 16:05:14.000000 pyalarmdotcomajax-0.5.2/pyalarmdotcomajax.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-01 16:05:14.000000 pyalarmdotcomajax-0.5.2/pyalarmdotcomajax.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 16:05:14.000000 pyalarmdotcomajax-0.5.2/pyalarmdotcomajax.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-06-01 16:04:59.000000 pyalarmdotcomajax-0.5.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-06-01 16:05:14.499249 pyalarmdotcomajax-0.5.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:05:14.499249 pyalarmdotcomajax-0.5.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-01 16:04:59.000000 pyalarmdotcomajax-0.5.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5080 2023-06-01 16:04:59.000000 pyalarmdotcomajax-0.5.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:05:14.499249 pyalarmdotcomajax-0.5.2/tests/responses/
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-01 16:04:59.000000 pyalarmdotcomajax-0.5.2/tests/responses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-06-01 16:04:59.000000 pyalarmdotcomajax-0.5.2/tests/test_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-06-01 16:04:59.000000 pyalarmdotcomajax-0.5.2/tests/test_device_extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-06-01 16:04:59.000000 pyalarmdotcomajax-0.5.2/tests/test_partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-06-01 16:04:59.000000 pyalarmdotcomajax-0.5.2/tests/test_sensors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-06-01 16:04:59.000000 pyalarmdotcomajax-0.5.2/tests/test_thermostat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:22:03.880803 pyalarmdotcomajax-0.5.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-09 01:21:44.000000 pyalarmdotcomajax-0.5.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18038 2023-06-09 01:22:03.880803 pyalarmdotcomajax-0.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-06-09 01:21:44.000000 pyalarmdotcomajax-0.5.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:22:03.872803 pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/
+-rw-r--r--   0 runner    (1001) docker     (123)    47043 2023-06-09 01:21:44.000000 pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-09 01:21:44.000000 pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20881 2023-06-09 01:21:44.000000 pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-06-09 01:21:44.000000 pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/const.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:22:03.876803 pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/devices/
+-rw-r--r--   0 runner    (1001) docker     (123)    13688 2023-06-09 01:21:44.000000 pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-09 01:21:44.000000 pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/devices/camera.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-06-09 01:21:44.000000 pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/devices/garage_door.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-06-09 01:21:44.000000 pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/devices/gate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-06-09 01:21:44.000000 pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/devices/image_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-06-09 01:21:44.000000 pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/devices/light.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-06-09 01:21:44.000000 pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/devices/lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6942 2023-06-09 01:21:44.000000 pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/devices/partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14854 2023-06-09 01:21:44.000000 pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/devices/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-06-09 01:21:44.000000 pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/devices/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-09 01:21:44.000000 pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/devices/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7610 2023-06-09 01:21:44.000000 pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/devices/thermostat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-06-09 01:21:44.000000 pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/devices/water_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-06-09 01:21:44.000000 pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22829 2023-06-09 01:21:44.000000 pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-06-09 01:21:44.000000 pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:22:03.876803 pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/websockets/
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-09 01:21:44.000000 pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/websockets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9122 2023-06-09 01:21:44.000000 pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/websockets/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-06-09 01:21:44.000000 pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/websockets/const.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:22:03.880803 pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/websockets/handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-06-09 01:21:44.000000 pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/websockets/handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-06-09 01:21:44.000000 pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/websockets/handler/garage_door.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-06-09 01:21:44.000000 pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/websockets/handler/gate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-06-09 01:21:44.000000 pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/websockets/handler/light.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-06-09 01:21:44.000000 pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/websockets/handler/lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-06-09 01:21:44.000000 pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/websockets/handler/partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-06-09 01:21:44.000000 pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/websockets/handler/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-06-09 01:21:44.000000 pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/websockets/handler/thermostat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-06-09 01:21:44.000000 pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/websockets/handler/water_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6313 2023-06-09 01:21:44.000000 pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/websockets/messages.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:22:03.872803 pyalarmdotcomajax-0.5.3/pyalarmdotcomajax.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18038 2023-06-09 01:22:03.000000 pyalarmdotcomajax-0.5.3/pyalarmdotcomajax.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-06-09 01:22:03.000000 pyalarmdotcomajax-0.5.3/pyalarmdotcomajax.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 01:22:03.000000 pyalarmdotcomajax-0.5.3/pyalarmdotcomajax.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-09 01:22:03.000000 pyalarmdotcomajax-0.5.3/pyalarmdotcomajax.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-09 01:22:03.000000 pyalarmdotcomajax-0.5.3/pyalarmdotcomajax.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-09 01:22:03.000000 pyalarmdotcomajax-0.5.3/pyalarmdotcomajax.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 01:22:03.000000 pyalarmdotcomajax-0.5.3/pyalarmdotcomajax.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-06-09 01:21:44.000000 pyalarmdotcomajax-0.5.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-06-09 01:22:03.880803 pyalarmdotcomajax-0.5.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:22:03.880803 pyalarmdotcomajax-0.5.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-09 01:21:44.000000 pyalarmdotcomajax-0.5.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5080 2023-06-09 01:21:44.000000 pyalarmdotcomajax-0.5.3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:22:03.880803 pyalarmdotcomajax-0.5.3/tests/responses/
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-09 01:21:44.000000 pyalarmdotcomajax-0.5.3/tests/responses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-06-09 01:21:44.000000 pyalarmdotcomajax-0.5.3/tests/test_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-06-09 01:21:44.000000 pyalarmdotcomajax-0.5.3/tests/test_device_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-06-09 01:21:44.000000 pyalarmdotcomajax-0.5.3/tests/test_partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-06-09 01:21:44.000000 pyalarmdotcomajax-0.5.3/tests/test_sensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-06-09 01:21:44.000000 pyalarmdotcomajax-0.5.3/tests/test_thermostat.py
```

### Comparing `pyalarmdotcomajax-0.5.2/LICENSE` & `pyalarmdotcomajax-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.2/PKG-INFO` & `pyalarmdotcomajax-0.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyalarmdotcomajax
-Version: 0.5.2
+Version: 0.5.3
 Summary: Python Interface for Alarm.com
 Home-page: https://github.com/pyalarmdotcom/pyalarmdotcomajax
 Author: Justin Wong
 Author-email: 46082645+uvjustin@users.noreply.github.com
 Maintainer: Elahd Bar-Shai
 Maintainer-email: 46082645+uvjustin@users.noreply.github.com, 466460+elahd@users.noreply.github.com
 License: MIT
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyalarmdotcomajax Version: 0.5.2 Summary: Python
+Metadata-Version: 2.1 Name: pyalarmdotcomajax Version: 0.5.3 Summary: Python
 Interface for Alarm.com Home-page: https://github.com/pyalarmdotcom/
 pyalarmdotcomajax Author: Justin Wong Author-email:
 46082645+uvjustin@users.noreply.github.com Maintainer: Elahd Bar-Shai
 Maintainer-email: 46082645+uvjustin@users.noreply.github.com,
 466460+elahd@users.noreply.github.com License: MIT Keywords: Alarm.com,Security
 System,Home Assistant Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: English Classifier: Environment :: Web
```

### Comparing `pyalarmdotcomajax-0.5.2/README.md` & `pyalarmdotcomajax-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/__init__.py` & `pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,31 +42,36 @@
     CameraSkybellControllerExtension,
     ConfigurationOption,
     ControllerExtensions_t,
     ExtendedProperties,
 )
 from pyalarmdotcomajax.websockets.client import WebSocketClient, WebSocketState
 
-__version__ = "0.5.2"
+__version__ = "0.5.3"
 
 log = logging.getLogger(__name__)
 
 
 class ExtensionResults(TypedDict):
     """Results of multi-device extension calls."""
 
     settings: dict[str, ConfigurationOption]
     controller: ControllerExtensions_t
 
 
 class AlarmController:
     """Base class for communicating with Alarm.com via API."""
 
+    HOME_URL = "https://www.alarm.com/web/system/home"
+    UA = f"pyalarmdotcomajax/{__version__}"
+
     AJAX_HEADERS_TEMPLATE = {
         "Accept": "application/vnd.api+json",
+        "User-Agent": UA,
+        "Referrer": HOME_URL,
         "ajaxrequestuniquekey": None,
     }
 
     ALL_DEVICES_URL_TEMPLATE = (  # Substitute with base url and system ID.
         "{}web/api/settings/manageDevices/deviceCatalogs/{}"
     )
     ALL_SYSTEMS_URL_TEMPLATE = "{}web/api/systems/availableSystemItems?searchString="
@@ -305,15 +310,15 @@
     async def async_send_command(
         self,
         device_type: DeviceType,
         event: BaseDevice.Command,
         device_id: str,  # ID corresponds to device_type
         msg_body: dict = {},  # Body of request. No abstractions here.
         retry_on_failure: bool = True,  # Set to prevent infinite loops when function calls itself
-    ) -> bool:
+    ) -> dict:
         """Send commands to Alarm.com."""
         log.info("Sending %s to Alarm.com.", event)
 
         msg_body["statePollOnly"] = False
 
         try:
             url = (
@@ -321,15 +326,17 @@
             )
         except KeyError as err:
             raise UnsupportedDeviceType(device_type, device_id) from err
 
         log.debug("Url %s", url)
 
         try:
-            async with self._websession.post(url=url, json=msg_body, headers=self._ajax_headers) as resp:
+            async with self._websession.post(
+                url=url, json=msg_body, headers=self._ajax_headers, raise_for_status=True
+            ) as resp:
                 log.debug("Response from Alarm.com %s", resp.status)
 
                 json_rsp = await resp.json()
 
                 # Special handling of 422 status.
                 # 422 sometimes occurs when forceBypass is True but there's nothing to bypass.
                 if (
@@ -354,19 +361,20 @@
                     )
 
                 # Run standard server response checks.
                 await self._async_handle_server_errors(json_rsp, "send_command", retry_on_failure)
 
                 # If above pass and we have a 200, we're good.
                 if str(resp.status) == "200":
-                    return True
+                    return dict(json_rsp)
 
         except aiohttp.ClientResponseError as err:
             log.exception("Failed to send command.")
             raise UnexpectedResponse from err
+
         except TryAgain:
             return await self.async_send_command(
                 device_type=device_type,
                 event=event,
                 device_id=device_id,
                 msg_body=msg_body,
                 retry_on_failure=False,
@@ -432,15 +440,15 @@
 
         #
         # Step 1: Get login page and cookies
         #
 
         try:
             # load login page once and grab VIEWSTATE/cookies
-            async with self._websession.get(url=self.LOGIN_URL, cookies=self._two_factor_cookie) as resp:
+            async with self._websession.get(url=self.LOGIN_URL, cookies=None) as resp:
                 text = await resp.text()
                 log.debug("Response status from Alarm.com: %s", resp.status)
                 tree = BeautifulSoup(text, "html.parser")
                 login_info = {
                     self.VIEWSTATE_FIELD: tree.select(f"#{self.VIEWSTATE_FIELD}")[0].attrs.get("value"),
                     self.VIEWSTATEGENERATOR_FIELD: tree.select(f"#{self.VIEWSTATEGENERATOR_FIELD}")[0].attrs.get(
                         "value"
@@ -469,15 +477,17 @@
                 data={
                     self.LOGIN_USERNAME_FIELD: self._username,
                     self.LOGIN_PASSWORD_FIELD: self._password,
                     self.VIEWSTATE_FIELD: login_info[self.VIEWSTATE_FIELD],
                     self.VIEWSTATEGENERATOR_FIELD: login_info[self.VIEWSTATEGENERATOR_FIELD],
                     self.EVENTVALIDATION_FIELD: login_info[self.EVENTVALIDATION_FIELD],
                     self.PREVIOUSPAGE_FIELD: login_info[self.PREVIOUSPAGE_FIELD],
-                    self.LOGIN_REMEMBERME_FIELD: "on",
+                    "__EVENTTARGET": None,
+                    "__EVENTARGUMENT": None,
+                    "__VIEWSTATEENCRYPTED": None,
                     "IsFromNewSite": "1",
                 },
                 cookies=self._two_factor_cookie,
                 raise_for_status=True,
             ) as resp:
                 if re.search("m=login_fail", str(resp.url)) is not None:
                     log.exception("Login failed.")
@@ -503,15 +513,14 @@
         #
         # Step 3: Get user's profile.
         #
 
         async with self._websession.get(
             url=c.IDENTITIES_URL_TEMPLATE.format(c.URL_BASE, ""),
             headers=self._ajax_headers,
-            cookies=self._two_factor_cookie,
         ) as resp:
             json_rsp = await resp.json()
 
             try:
                 self._user_id = json_rsp["data"][0]["id"]
                 self._provider_name = json_rsp["data"][0]["attributes"]["logoName"]
                 self._provider_name = json_rsp["data"][0]["attributes"]["logoName"]
@@ -683,14 +692,16 @@
         raise UnexpectedResponse("Failed to find two-factor authentication cookie.")
 
     async def is_logged_in(self, throw: bool = False) -> bool:
         """Check if we are still logged in."""
 
         url = f"{c.URL_BASE[:-1]}{self._keep_alive_url}{self.KEEP_ALIVE_URL_PARAM_TEMPLATE.format(int(round(datetime.now().timestamp())))}"
 
+        text_rsp: str
+
         try:
             async with self._websession.get(
                 url=url,
                 headers=self._ajax_headers,
                 raise_for_status=True,
             ) as resp:
                 text_rsp = await resp.text()
@@ -793,17 +804,17 @@
                     for sub_device in family_data["data"]:
                         children.append((sub_device["id"], DeviceType(family_name)))
 
         #
         # BUILD DEVICE INSTANCE
         #
 
-        device_extension_results: ExtensionResults | dict = extension_results.get(
-            entity_id := raw_device["id"], {}
-        )
+        entity_id = raw_device["id"]
+
+        device_extension_results: ExtensionResults | dict = extension_results.get(entity_id, {})
 
         return device_class(
             id_=entity_id,
             raw_device_data=raw_device,
             children=children,
             device_type_specific_data=device_type_specific_data.get(entity_id),
             send_action_callback=self.async_send_command,
@@ -1149,23 +1160,23 @@
 
             case "403":  # Invalid Anti-Forgery Token
                 # 403 means that either the user doesn't have access to this class of device or that the user has logged out.
                 # Unsupported device types should be stripped out in async_update(), so assume logged out.
                 # If logged out, try logging in again, then give up by pretending that we couldn't find any devices of this type.
 
                 if not retry_on_failure:
-                    log.exception(
+                    log.error(
                         "Error fetching data from Alarm.com. Got 403 status when"
                         f" fetching {request_name}. Logging in"
                         " again didn't help. Giving up on device type."
                     )
                     raise UnexpectedResponse(error_msg)
 
                 if not self.is_logged_in():
-                    log.debug(
+                    log.info(
                         "Error fetching data from Alarm.com. Got 403 status"
                         f" when requesting {request_name}. Trying to"
                         " refresh auth tokens by logging in again."
                     )
 
                     await self.async_login()
```

### Comparing `pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/cli.py` & `pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -486,18 +486,16 @@
     output_str += "\n"
 
     # BATTERY
     if element.battery_critical:
         battery = "Critical"
     elif element.battery_low:
         battery = "Low"
-    elif element.battery_critical is not None or element.battery_low is not None:
-        battery = "Normal"
     else:
-        battery = None
+        battery = "Normal"
 
     # ATTRIBUTES
     output_str += "ATTRIBUTES: "
 
     if isinstance(element.device_subtype, Sensor.Subtype) or element.state or battery or element.read_only:
         if isinstance(element.device_subtype, Sensor.Subtype):
             output_str += f'[TYPE: {element.device_subtype.name.title().replace("_"," ")}] '
```

### Comparing `pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/const.py` & `pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/const.py`

 * *Files 22% similar despite different names*

```diff
@@ -21,7 +21,13 @@
     # https://www.alarm.com/web/system/assets/customer-ember/enums/TwoFactorAuthenticationType.js
     # Keep these lowercase. Strings.json in Home Assistant requires lowercase values.
 
     disabled = 0
     app = 1
     sms = 2
     email = 4
+
+
+ATTR_STATE_TEXT = "displayStateText"
+ATTR_MAC_ADDRESS = "mac_address"
+ATTR_STATE = "state"
+ATTR_DESIRED_STATE = "desiredState"
```

### Comparing `pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/devices/__init__.py` & `pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/devices/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,16 +3,17 @@
 
 import contextlib
 import logging
 from abc import ABC
 from collections.abc import Callable
 from dataclasses import dataclass
 from enum import Enum
-from typing import Any, TypedDict
+from typing import Any, Final, TypedDict
 
+from pyalarmdotcomajax.const import ATTR_DESIRED_STATE, ATTR_STATE
 from pyalarmdotcomajax.exceptions import (
     InvalidConfigurationOption,
 )
 from pyalarmdotcomajax.extensions import (
     CameraSkybellControllerExtension,
     ConfigurationOption,
 )
@@ -73,15 +74,14 @@
     raw_recent_images: list[dict]
 
 
 class BaseDevice(ABC, CastingMixin):
     """Contains properties shared by all ADC devices."""
 
     _DEVICE_MODELS: dict  # deviceModelId: {"manufacturer": str, "model": str}
-    _ATTRIB_STATE = "state"
 
     def __init__(
         self,
         id_: str,
         send_action_callback: Callable,
         config_change_callback: Callable | None,
         children: list[tuple[str, DeviceType]],
@@ -89,84 +89,92 @@
         device_type_specific_data: DeviceTypeSpecificData | None = None,
         trouble_conditions: list | None = None,
         partition_id: str | None = None,
         settings: dict | None = None,  # slug: ConfigurationOption
     ) -> None:
         """Initialize base element class."""
 
-        self._id_: str = id_
-        self._family_raw: str | None = raw_device_data.get("type")
-        self._attribs_raw: dict = raw_device_data.get("attributes", {})
+        self.id_: Final[str] = id_
+        self._raw: dict = raw_device_data
         self._device_type_specific_data: DeviceTypeSpecificData = (
             device_type_specific_data if device_type_specific_data else {}
         )
-        self._send_action_callback: Callable = send_action_callback
-        self._config_change_callback: Callable | None = config_change_callback
         self._settings: dict = settings if settings else {}
+        self._partition_id: str | None = partition_id
 
         self.children = children
         self.trouble_conditions: list[TroubleCondition] = trouble_conditions if trouble_conditions else []
 
-        self._system_id: str | None = (
-            raw_device_data.get("relationships", {}).get("system", {}).get("data", {}).get("id")
-        )
-        self._partition_id: str | None = partition_id
+        self._send_action_callback = send_action_callback
+        self._config_change_callback: Callable | None = config_change_callback
 
         self.external_update_callback: list[Callable] = []
 
         self.process_device_type_specific_data()
 
-        log.debug("Initialized %s %s", self._family_raw, self.name)
+        log.debug("Initialized %s %s", raw_device_data.get("type"), self.name)
 
     #
     # Properties
     #
 
     @property
     def read_only(self) -> bool | None:
         """Return whether logged in user has permission to change state."""
         return (
             not result
             if isinstance(
-                (result := self._attribs_raw.get("hasPermissionToChangeState")),
+                (result := self.raw_attributes.get("hasPermissionToChangeState")),
                 bool,
             )
             else None
         )
 
     @property
-    def id_(self) -> str:
-        """Return device ID."""
-        return self._id_
-
-    @property
-    def name(self) -> None | str:
+    def name(self) -> str:
         """Return user-assigned device name."""
 
-        return self._attribs_raw.get("description", None)
+        return str(self.raw_attributes["description"])
 
     @property
-    def attribs_raw(self) -> None | dict:
+    def raw_attributes(self) -> dict:
         """Return raw attributes."""
 
-        return self._attribs_raw
+        return self._raw.get("attributes", {})
+
+    @property
+    def available(self) -> bool:
+        """Return whether the light can be manipulated."""
+        return not self.malfunction
 
     @property
-    def has_state(self) -> bool:
+    def has_state(self) -> bool | None:
         """Return whether entity reports state."""
-        return self._attribs_raw.get("hasState", False)
+
+        return self.raw_attributes.get("hasState")
 
     @property
-    def state(self) -> Enum | None:
+    def state(self) -> DeviceState | None:
         """Return state."""
 
         # Devices that don't report state on Alarm.com still have a value in the state field.
         if self.has_state:
             with contextlib.suppress(ValueError):
-                return self.DeviceState(self._attribs_raw.get("state"))
+                return self.DeviceState(self.raw_attributes.get("state"))
+
+        return None
+
+    @property
+    def desired_state(self) -> DeviceState | None:
+        """Return state."""
+
+        # Devices that don't report state on Alarm.com still have a value in the desiredState field.
+        if self.has_state:
+            with contextlib.suppress(ValueError, KeyError):
+                return self.DeviceState(self.raw_attributes.get("desiredState"))
 
         return None
 
     @property
     def settings(self) -> dict:
         """Return user-changable settings."""
 
@@ -175,103 +183,145 @@
             for config_option in self._settings.values()
             if isinstance(config_option, ConfigurationOption) and config_option.user_configurable
         }
 
     @property
     def battery_low(self) -> bool | None:
         """Return whether battery is low."""
-        return self._attribs_raw.get("lowBattery")
+
+        return self.raw_attributes.get("lowBattery")
 
     @property
     def battery_critical(self) -> bool | None:
         """Return whether battery is critically low."""
-        return self._attribs_raw.get("criticalBattery")
+
+        return self.raw_attributes.get("criticalBattery")
 
     @property
     def system_id(self) -> str | None:
         """Return ID of device's parent system."""
-        return self._system_id
+
+        if sys := self._raw.get("relationships", {}).get("system", {}).get("data", {}).get("id"):
+            return str(sys)
+
+        return None
 
     @property
     def partition_id(self) -> str | None:
         """Return ID of device's parent partition."""
         return self._partition_id
 
     @property
     def malfunction(self) -> bool | None:
         """Return whether device is malfunctioning."""
-        return self._attribs_raw.get("isMalfunctioning", True) or self.state is None
+        return self.raw_attributes.get("isMalfunctioning")
 
     @property
     def mac_address(self) -> str | None:
         """Return device MAC address."""
-        return self._attribs_raw.get("macAddress")
+        return str(self.raw_attributes.get("macAddress"))
 
     @property
     def raw_state_text(self) -> str | None:
         """Return state description as reported by ADC."""
-        return self._attribs_raw.get("displayStateText")
+        return str(self.raw_attributes.get("displayStateText"))
 
     @property
-    def model_text(self) -> str | None:
+    def model_text(self) -> str:
         """Return device model as reported by ADC."""
-        return (
-            reported_model
-            if (reported_model := self._attribs_raw.get("deviceModel"))
-            else self._DEVICE_MODELS.get(self._attribs_raw.get("deviceModelId"))
-        )
+
+        if model := self.raw_attributes.get("deviceModel"):
+            return str(model)
+
+        if model := self._DEVICE_MODELS.get(self.raw_attributes.get("deviceModelId")):
+            return str(model)
+
+        return ""
 
     @property
     def manufacturer(self) -> str | None:
         """Return device model as reported by ADC."""
-        return self._attribs_raw.get("manufacturer")
+        return self.raw_attributes.get("manufacturer")
 
     @property
     def debug_data(self) -> dict:
         """Return data that is helpful for debugging."""
-        return self._attribs_raw
+        return self.raw_attributes
 
     @property
     def device_subtype(self) -> Enum | None:
         """Return normalized device subtype const. E.g.: contact, glass break, etc."""
         try:
-            return self.Subtype(self._attribs_raw["deviceType"])
-        except (ValueError, KeyError):
+            return self.Subtype(self.raw_attributes.get("deviceType"))
+        except ValueError:
             return None
 
     # #
     # FUNCTIONS
     # #
 
-    async def async_handle_external_state_change(self, raw_state: int) -> None:
-        """Update device state when notified of externally-triggered change."""
+    async def _send_action(
+        self,
+        device_type: DeviceType,
+        event: BaseDevice.Command,
+        device_id: str,
+        msg_body: dict = {},
+        retry_on_failure: bool = True,
+    ) -> None:
+        """Send action to ADC."""
 
-        self._attribs_raw.update({self._ATTRIB_STATE: raw_state})
+        if updated_device_object := await self._send_action_callback(
+            device_type, event, device_id, msg_body, retry_on_failure
+        ):
+            try:
+                await self.async_handle_external_attribute_change(
+                    updated_device_object["data"]["attributes"], "user action response"
+                )
+            except KeyError:
+                log.exception(f"Failed to update device {self.name} with response {updated_device_object}")
+
+    async def async_handle_external_dual_state_change(self, state: BaseDevice.DeviceState | int | None) -> None:
+        """Update device state when notified of externally-triggered change.
 
-        log.info(f"{__name__} Got async update for {self.name} ({self.id_}) with new state: {self.state}.")
+        Takes either a DeviceState or a DeviceState int value for the new state.
+        """
 
-        for external_callback in self.external_update_callback:
-            external_callback()
+        final_state = state.value if isinstance(state, Enum) else state
 
-    async def async_handle_external_attribute_change(self, new_attribute: dict) -> None:
-        """Update device attribute when notified of externally-triggered change."""
+        await self.async_handle_external_attribute_change(
+            {ATTR_STATE: final_state, ATTR_DESIRED_STATE: final_state}, "WebSocket message"
+        )
 
-        self._attribs_raw.update(new_attribute)
+    async def async_handle_external_desired_state_change(self, state: BaseDevice.DeviceState | None) -> None:
+        """Update device state when notified of externally-triggered change."""
 
-        for external_callback in self.external_update_callback:
-            external_callback()
+        await self.async_handle_external_attribute_change(
+            {ATTR_DESIRED_STATE: state.value if isinstance(state, Enum) else state}, "WebSocket message"
+        )
 
-    async def async_log_new_attribute(self, attribute_name: str, attribute_value: Any) -> None:
-        """Log externally-triggered attribute change."""
+    async def async_handle_external_attribute_change(
+        self, new_attributes: dict, source: str | None = None
+    ) -> None:
+        """Update device attribute when notified of externally-triggered change."""
 
         log.info(
-            f"{__name__} Got async update for {self.name} ({self.id_}) with new {attribute_name}:"
-            f" {attribute_value}."
+            f"{__name__} Got async update for {self.name} ({self.id_}){' from ' + source if source else ''} with"
+            f" new {new_attributes}."
         )
 
+        self.raw_attributes.update(new_attributes)
+
+        new_attrib_key = list(new_attributes.keys())[0]
+        new_attrib_value = list(new_attributes.values())[0]
+
+        log.debug(f"Desired: [{new_attrib_value}] | Current: [{self.raw_attributes.get(new_attrib_key)}]")
+
+        for external_callback in self.external_update_callback:
+            external_callback()
+
     def register_external_update_callback(self, callback: Callable) -> None:
         """Register callback to be called when device state changes."""
 
         self.external_update_callback.append(callback)
 
     def unregister_external_update_callback(self, callback: Callable) -> None:
         """Unregister callback to be called when device state changes."""
@@ -340,29 +390,29 @@
     # #
     # CASTING FUNCTIONS
     # #
 
     # Override CastingMixin functions to automatically pass in _raw_attribs dict.
 
     def _get_int(self, key: str) -> int | None:
-        """Return int value from _attribs_raw."""
-        return super()._safe_int_from_dict(self._attribs_raw, key)
+        """Return int value from _raw_attributes."""
+        return super()._safe_int_from_dict(self.raw_attributes, key)
 
     def _get_float(self, key: str) -> float | None:
-        """Return float value from _attribs_raw."""
-        return super()._safe_float_from_dict(self._attribs_raw, key)
+        """Return float value from _raw_attributes."""
+        return super()._safe_float_from_dict(self.raw_attributes, key)
 
     def _get_str(self, key: str) -> str | None:
-        """Return str value from _attribs_raw."""
-        return super()._safe_str_from_dict(self._attribs_raw, key)
+        """Return str value from _raw_attributes."""
+        return super()._safe_str_from_dict(self.raw_attributes, key)
 
     def _get_bool(self, key: str) -> bool | None:
-        """Return bool value from _attribs_raw."""
-        return super()._safe_bool_from_dict(self._attribs_raw, key)
+        """Return bool value from _raw_attributes."""
+        return super()._safe_bool_from_dict(self.raw_attributes, key)
 
     def _get_list(self, key: str, value_type: type) -> list | None:
-        """Return list value from _attribs_raw."""
-        return super()._safe_list_from_dict(self._attribs_raw, key, value_type)
+        """Return list value from _raw_attributes."""
+        return super()._safe_list_from_dict(self.raw_attributes, key, value_type)
 
     def _get_special(self, key: str, value_type: type) -> Any | None:
-        """Return specified type value from _attribs_raw."""
-        return super()._safe_special_from_dict(self._attribs_raw, key, value_type)
+        """Return specified type value from _raw_attributes."""
+        return super()._safe_special_from_dict(self.raw_attributes, key, value_type)
```

### Comparing `pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/devices/gate.py` & `pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/devices/lock.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,70 +1,51 @@
-"""Alarm.com gate."""
+"""Alarm.com lock."""
 from __future__ import annotations
 
 import logging
-from dataclasses import dataclass
-from enum import Enum
 
 from pyalarmdotcomajax.devices import DeviceType
 
 from . import BaseDevice
 
 log = logging.getLogger(__name__)
 
 
-class Gate(BaseDevice):
-    """Represent Alarm.com gate element."""
+class Lock(BaseDevice):
+    """Represent Alarm.com sensor element."""
 
-    @dataclass
-    class GateAttributes(BaseDevice.DeviceAttributes):
-        """Gate attributes."""
+    class DeviceState(BaseDevice.DeviceState):
+        """Enum of lock states."""
 
-        supports_remote_close: bool | None  # Specifies whether the gate can be closed remotely.
-
-    class DeviceState(Enum):
-        """Enum of gate states."""
-
-        # https://www.alarm.com/web/system/assets/customer-ember/enums/GateStatus.js
+        # https://www.alarm.com/web/system/assets/customer-ember/enums/LockStatus.js
 
         UNKNOWN = 0
-        OPEN = 1
-        CLOSED = 2
+        LOCKED = 1
+        UNLOCKED = 2
 
-    class Command(Enum):
-        """Commands for ADC gates."""
+    class Command(BaseDevice.Command):
+        """Commands for ADC locks."""
 
-        OPEN = "open"
-        CLOSE = "close"
+        LOCK = "lock"
+        UNLOCK = "unlock"
 
-    @property
-    def attributes(self) -> GateAttributes | None:
-        """Return thermostat attributes."""
+    async def async_lock(self) -> None:
+        """Send lock command."""
 
-        return self.GateAttributes(
-            supports_remote_close=self._get_bool("supportsRemoteClose"),
-        )
+        await self.async_handle_external_desired_state_change(self.DeviceState.LOCKED)
 
-    async def async_open(self) -> None:
-        """Send open command."""
-
-        await self._send_action_callback(
-            device_type=DeviceType.GATE,
-            event=self.Command.OPEN,
+        await self._send_action(
+            device_type=DeviceType.LOCK,
+            event=self.Command.LOCK,
             device_id=self.id_,
         )
 
-    async def async_close(self) -> None:
-        """Send close command."""
+    async def async_unlock(self) -> None:
+        """Send unlock command."""
+
+        await self.async_handle_external_desired_state_change(self.DeviceState.UNLOCKED)
 
-        if (
-            self.attributes is not None
-            and hasattr(self.attributes, "supports_remote_close")
-            and not self.attributes.supports_remote_close
-        ):
-            raise NotImplementedError("Gate does not support remote close.")
-
-        await self._send_action_callback(
-            device_type=DeviceType.GATE,
-            event=self.Command.CLOSE,
+        await self._send_action(
+            device_type=DeviceType.LOCK,
+            event=self.Command.UNLOCK,
             device_id=self.id_,
         )
```

### Comparing `pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/devices/image_sensor.py` & `pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/devices/image_sensor.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """Alarm.com image sensor."""
 from __future__ import annotations
 
 import logging
 from datetime import datetime
-from enum import Enum
 from typing import TypedDict
 
 from dateutil import parser
 
 from pyalarmdotcomajax.devices import DeviceType
 
 from . import BaseDevice
@@ -24,15 +23,17 @@
     description: str
     timestamp: datetime
 
 
 class ImageSensor(BaseDevice):
     """Represent Alarm.com image sensor element."""
 
-    class Command(Enum):
+    malfunction = False
+
+    class Command(BaseDevice.Command):
         """Commands for ADC image sensors."""
 
         PEEK_IN = "doPeekInNow"
 
     _recent_images: list[ImageSensorImage] = []
 
     def process_device_type_specific_data(self) -> None:
@@ -53,25 +54,20 @@
                     "image_src": image["attributes"]["imageSrc"],
                     "description": image["attributes"]["description"],
                     "timestamp": parser.parse(image["attributes"]["timestamp"]),
                 }
                 self._recent_images.append(image_data)
 
     @property
-    def malfunction(self) -> bool | None:
-        """Return whether device is malfunctioning."""
-        return None
-
-    @property
     def images(self) -> list[ImageSensorImage] | None:
         """Get a list of images taken by the image sensor."""
 
         return self._recent_images
 
     async def async_peek_in(self) -> None:
         """Send peek in command to take photo."""
 
-        await self._send_action_callback(
+        await self._send_action(
             device_type=DeviceType.IMAGE_SENSOR,
             event=self.Command.PEEK_IN,
             device_id=self.id_,
         )
```

### Comparing `pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/devices/light.py` & `pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/devices/light.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,86 +1,75 @@
 """Alarm.com light."""
 from __future__ import annotations
 
 import logging
-from enum import Enum
 
 from pyalarmdotcomajax.devices import BaseDevice, DeviceType
 
 log = logging.getLogger(__name__)
 
 
 # WebSocket Handler: https://www.alarm.com/web/system/assets/customer-ember/websockets/handlers/lights.ts
 class Light(BaseDevice):
     """Represent Alarm.com light element."""
 
     ATTRIB_LIGHT_LEVEL = "lightLevel"
 
-    class DeviceState(Enum):
+    class DeviceState(BaseDevice.DeviceState):
         """Enum of light states."""
 
         # https://www.alarm.com/web/system/assets/customer-ember/enums/LightStatus.js
 
         OFFLINE = 0
         NOSTATE = 1
         ON = 2
         OFF = 3
         LEVELCHANGE = 4
 
-    class Command(Enum):
+    class Command(BaseDevice.Command):
         """Commands for ADC lights."""
 
         ON = "turnOn"
         OFF = "turnOff"
 
     @property
-    def available(self) -> bool:
-        """Return whether the light can be manipulated."""
-        return (
-            self._attribs_raw.get("canReceiveCommands", False)
-            and self._attribs_raw.get("remoteCommandsEnabled", False)
-            and self._attribs_raw.get("hasPermissionToChangeState", False)
-            and self.state in [self.DeviceState.ON, self.DeviceState.OFF, self.DeviceState.LEVELCHANGE]
-        )
-
-    @property
     def brightness(self) -> int | None:
         """Return light's brightness."""
-        if not self._attribs_raw.get("isDimmer", False):
+        if not self.raw_attributes.get("isDimmer", False):
             return None
 
-        if isinstance(level := self._attribs_raw.get(self.ATTRIB_LIGHT_LEVEL, 0), int):
+        if isinstance(level := self.raw_attributes.get(self.ATTRIB_LIGHT_LEVEL, 0), int):
             return level
 
         return None
 
     @property
     def supports_state_tracking(self) -> bool | None:
         """Return whether the light reports its current state."""
 
-        if isinstance(supports := self._attribs_raw.get("stateTrackingEnabled"), bool):
+        if isinstance(supports := self.raw_attributes.get("stateTrackingEnabled"), bool):
             return supports
 
         return None
 
     async def async_turn_on(self, brightness: int | None = None) -> None:
         """Send turn on command with optional brightness."""
 
         msg_body: dict = {}
         if brightness:
             msg_body["dimmerLevel"] = brightness
 
-        await self._send_action_callback(
+        await self._send_action(
             device_type=DeviceType.LIGHT,
             event=self.Command.ON,
             device_id=self.id_,
             msg_body=msg_body,
         )
 
     async def async_turn_off(self) -> None:
         """Send turn off command."""
 
-        await self._send_action_callback(
+        await self._send_action(
             device_type=DeviceType.LIGHT,
             event=self.Command.OFF,
             device_id=self.id_,
         )
```

### Comparing `pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/devices/partition.py` & `pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/devices/partition.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,36 +37,36 @@
 
     @dataclass
     class PartitionAttributes(BaseDevice.DeviceAttributes):
         """Partition attributes."""
 
         extended_arming_options: Partition.ExtendedArmingMapping  # List of extended arming options
 
-    class DeviceState(Enum):
+    class DeviceState(BaseDevice.DeviceState):
         """Enum of arming states."""
 
         # https://www.alarm.com/web/system/assets/customer-ember/enums/ArmingState.js
 
         UNKNOWN = 0
         DISARMED = 1
         ARMED_STAY = 2
         ARMED_AWAY = 3
         ARMED_NIGHT = 4
 
-    class Command(Enum):
+    class Command(BaseDevice.Command):
         """Commands for ADC partitions."""
 
         DISARM = "disarm"
         ARM_STAY = "armStay"
         ARM_AWAY = "armAway"
 
     @property
     def uncleared_issues(self) -> bool | None:
         """Return whether user needs to clear device state on alarm.com."""
-        if isinstance(issues := self._attribs_raw.get("needsClearIssuesPrompt", None), bool):
+        if isinstance(issues := self.raw_attributes.get("needsClearIssuesPrompt", None), bool):
             return issues
 
         return None
 
     async def _async_arm(
         self,
         arm_type: Command,
@@ -92,15 +92,15 @@
 
         if silent_arming and Partition.ExtendedArmingOption.SILENT_ARMING in extended_arming_options:
             msg_body.update({"silentArming": silent_arming})
 
         if night_arming and Partition.ExtendedArmingOption.NIGHT_ARMING in extended_arming_options:
             msg_body.update({"nightArming": night_arming})
 
-        await self._send_action_callback(
+        await self._send_action(
             device_type=DeviceType.PARTITION,
             event=arm_type,
             device_id=self.id_,
             msg_body=msg_body,
         )
 
     @property
@@ -118,14 +118,16 @@
         no_entry_delay: bool | None = None,
         silent_arming: bool | None = None,
     ) -> None:
         """Arm stay alarm."""
 
         log.debug("Calling arm stay.")
 
+        await self.async_handle_external_desired_state_change(self.DeviceState.ARMED_STAY)
+
         await self._async_arm(
             arm_type=self.Command.ARM_STAY,
             extended_arming_options=self.attributes.extended_arming_options.arm_stay,
             force_bypass=force_bypass,
             no_entry_delay=no_entry_delay,
             silent_arming=silent_arming,
         )
@@ -136,14 +138,16 @@
         no_entry_delay: bool | None = None,
         silent_arming: bool | None = None,
     ) -> None:
         """Arm stay alarm."""
 
         log.debug("Calling arm away.")
 
+        await self.async_handle_external_desired_state_change(self.DeviceState.ARMED_AWAY)
+
         await self._async_arm(
             arm_type=self.Command.ARM_AWAY,
             extended_arming_options=self.attributes.extended_arming_options.arm_away,
             force_bypass=force_bypass,
             no_entry_delay=no_entry_delay,
             silent_arming=silent_arming,
         )
@@ -154,14 +158,16 @@
         no_entry_delay: bool | None = None,
         silent_arming: bool | None = None,
     ) -> None:
         """Arm stay alarm."""
 
         log.debug("Calling arm night.")
 
+        await self.async_handle_external_desired_state_change(self.DeviceState.ARMED_NIGHT)
+
         await self._async_arm(
             arm_type=self.Command.ARM_STAY,
             extended_arming_options=self.attributes.extended_arming_options.arm_night,
             force_bypass=force_bypass,
             no_entry_delay=no_entry_delay,
             silent_arming=silent_arming,
             night_arming=True,
@@ -170,30 +176,32 @@
     async def async_disarm(
         self,
     ) -> None:
         """Disarm alarm system."""
 
         log.debug("Calling disarm.")
 
-        await self._send_action_callback(
+        await self.async_handle_external_desired_state_change(self.DeviceState.DISARMED)
+
+        await self._send_action(
             device_type=DeviceType.PARTITION,
             event=self.Command.DISARM,
             device_id=self.id_,
         )
 
     def _get_extended_arming_options(self, options_list: list) -> list[Partition.ExtendedArmingOption | None]:
         """Convert raw extended arming options to ExtendedArmingOption."""
 
         return [self.ExtendedArmingOption(option) for option in options_list]
 
     @property
     def attributes(self) -> PartitionAttributes:
         """Return partition attributes."""
 
-        extended_arming_options = dict(self._attribs_raw.get("extendedArmingOptions", {}))
+        extended_arming_options = dict(self.raw_attributes.get("extendedArmingOptions", {}))
 
         return self.PartitionAttributes(
             extended_arming_options=self.ExtendedArmingMapping(
                 disarm=self._get_extended_arming_options(extended_arming_options.get("Disarmed", [])),
                 arm_stay=self._get_extended_arming_options(extended_arming_options.get("ArmedStay", [])),
                 arm_away=self._get_extended_arming_options(extended_arming_options.get("ArmedAway", [])),
                 arm_night=self._get_extended_arming_options(extended_arming_options.get("ArmedNight", [])),
```

### Comparing `pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/devices/registry.py` & `pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/devices/registry.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,56 +18,55 @@
 from pyalarmdotcomajax.devices.thermostat import Thermostat
 from pyalarmdotcomajax.devices.water_sensor import WaterSensor
 from pyalarmdotcomajax.exceptions import UnkonwnDevice, UnsupportedDeviceType
 from pyalarmdotcomajax.helpers import classproperty
 
 log = logging.getLogger(__name__)
 
+AllDevices_t = (
+    Camera
+    | GarageDoor
+    | Gate
+    | ImageSensor
+    | Light
+    | Lock
+    | Partition
+    | Sensor
+    | System
+    | Thermostat
+    | WaterSensor
+)
+
 AllDeviceTypes_t = (
     type[Camera]
     | type[GarageDoor]
     | type[Gate]
     | type[ImageSensor]
     | type[Light]
     | type[Lock]
     | type[Partition]
     | type[Sensor]
     | type[System]
     | type[Thermostat]
     | type[WaterSensor]
 )
 
-AllCommands_t = (
-    Camera.Command
-    | GarageDoor.Command
-    | Gate.Command
-    | ImageSensor.Command
-    | Light.Command
-    | Lock.Command
-    | Partition.Command
-    | Sensor.Command
-    | System.Command
-    | Thermostat.Command
-    | WaterSensor.Command
-)
-
-
-AllDevices_t = (
-    Camera
-    | GarageDoor
-    | Gate
-    | ImageSensor
-    | Light
-    | Lock
-    | Partition
-    | Sensor
-    | System
-    | Thermostat
-    | WaterSensor
-)
+# AllCommands_t = (
+#     Camera.Command
+#     | GarageDoor.Command
+#     | Gate.Command
+#     | ImageSensor.Command
+#     | Light.Command
+#     | Lock.Command
+#     | Partition.Command
+#     | Sensor.Command
+#     | System.Command
+#     | Thermostat.Command
+#     | WaterSensor.Command
+# )
 
 
 AllDevicesLists_t = (
     list[Camera]
     | list[GarageDoor]
     | list[Gate]
     | list[ImageSensor]
```

### Comparing `pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/devices/sensor.py` & `pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/devices/sensor.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """Alarm.com sensor."""
 from __future__ import annotations
 
 import logging
-from enum import Enum, IntEnum
+from enum import IntEnum
 
 from . import BaseDevice
 
 log = logging.getLogger(__name__)
 
 
 class Sensor(BaseDevice):
     """Represent Alarm.com sensor element."""
 
-    class DeviceState(Enum):
+    class DeviceState(BaseDevice.DeviceState):
         """Enum of sensor states."""
 
         # https://www.alarm.com/web/system/assets/customer-ember/enums/SensorStatus.js
 
         UNKNOWN = 0
         CLOSED = 1
         OPEN = 2
```

### Comparing `pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/devices/thermostat.py` & `pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/devices/thermostat.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """Alarm.com thermostat."""
 from __future__ import annotations
 
 import logging
 from dataclasses import dataclass
 from enum import Enum
 
-from pyalarmdotcomajax.devices import DeviceType
+from pyalarmdotcomajax.const import ATTR_STATE
 from pyalarmdotcomajax.exceptions import UnexpectedResponse
 
-from . import BaseDevice
+from . import BaseDevice, DeviceType
 
 log = logging.getLogger(__name__)
 
 
 class Thermostat(BaseDevice):
     """Represent Alarm.com thermostat element."""
 
@@ -41,15 +41,15 @@
         # AUTO_HIGH = 2
         # ON_HIGH = 3
         # AUTO_MEDIUM = 4
         # ON_MEDIUM = 5
         # CIRCULATE = 6
         # HUMIDITY = 7
 
-    class DeviceState(Enum):
+    class DeviceState(BaseDevice.DeviceState):
         """Enum of thermostat states."""
 
         # https://www.alarm.com/web/system/assets/customer-ember/enums/ThermostatStatus.js
 
         UNKNOWN = 0
         OFF = 1
         HEAT = 2
@@ -79,15 +79,15 @@
         """Enum of thermostat setpoint types."""
 
         FIXED = 0
         AWAY = 1
         HOME = 2
         SLEEP = 3
 
-    class Command(Enum):
+    class Command(BaseDevice.Command):
         """Commands for ADC lights."""
 
         SET_STATE = "setState"
 
     @dataclass
     class ThermostatAttributes(BaseDevice.DeviceAttributes):
         """Thermostat attributes."""
@@ -127,24 +127,14 @@
 
     _DEVICE_MODELS = {
         4293: {"manufacturer": "Honeywell", "model": "T6 Pro"},
         10023: {"manufacturer": "ecobee", "model": "ecobee3 lite"},
     }
 
     @property
-    def available(self) -> bool:
-        """Return whether the light can be manipulated."""
-        return (
-            self._attribs_raw.get("canReceiveCommands", False)
-            and self._attribs_raw.get("remoteCommandsEnabled", False)
-            and self._attribs_raw.get("hasPermissionToChangeState", False)
-            and self.state is not self.DeviceState.UNKNOWN
-        )
-
-    @property
     def attributes(self) -> ThermostatAttributes:
         """Return thermostat attributes."""
 
         return self.ThermostatAttributes(
             temp_average=self._get_float("forwardingAmbientTemp"),
             temp_at_tstat=self._get_float(self.ATTRIB_AMBIENT_TEMP),
             inferred_mode=self._get_special("inferredMode", self.DeviceState),
@@ -189,27 +179,27 @@
         if (attrib_list := [state, fan, cool_setpoint, heat_setpoint, schedule_mode]).count(None) < len(
             attrib_list
         ) - 1:
             raise UnexpectedResponse
 
         # Build the request body.
         if state:
-            msg_body = {self._ATTRIB_STATE: state.value}
+            msg_body = {ATTR_STATE: state.value}
         elif fan:
             msg_body = {
                 self.ATTRIB_DESIRED_FAN_MODE: self.FanMode(fan[0]).value,
                 "desiredFanDuration": 0 if self.FanMode(fan[0]) == self.FanMode.AUTO else fan[1],
             }
         elif cool_setpoint:
             msg_body = {self.ATTRIB_DESIRED_COOL_SETPOINT: cool_setpoint}
         elif heat_setpoint:
             msg_body = {self.ATTRIB_DESIRED_HEAT_SETPOINT: heat_setpoint}
         elif schedule_mode:
             msg_body = {"desiredScheduleMode": schedule_mode.value}
 
         # Send
-        await self._send_action_callback(
+        await self._send_action(
             device_type=DeviceType.THERMOSTAT,
             event=self.Command.SET_STATE,
             device_id=self.id_,
             msg_body=msg_body,
         )
```

### Comparing `pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/exceptions.py` & `pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/extensions.py` & `pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/extensions.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/helpers.py` & `pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/helpers.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/websockets/client.py` & `pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/websockets/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,23 +12,28 @@
 import aiohttp
 from aiohttp import ClientSession
 
 from pyalarmdotcomajax import const as c
 from pyalarmdotcomajax.devices.garage_door import GarageDoor
 from pyalarmdotcomajax.devices.gate import Gate
 from pyalarmdotcomajax.devices.light import Light
+from pyalarmdotcomajax.devices.lock import Lock
 from pyalarmdotcomajax.devices.partition import Partition
 from pyalarmdotcomajax.devices.registry import DeviceRegistry
 from pyalarmdotcomajax.devices.sensor import Sensor
 from pyalarmdotcomajax.devices.thermostat import Thermostat
 from pyalarmdotcomajax.devices.water_sensor import WaterSensor
-from pyalarmdotcomajax.exceptions import AuthenticationFailed, UnexpectedResponse
+from pyalarmdotcomajax.exceptions import (
+    AuthenticationFailed,
+    UnexpectedResponse,
+)
 from pyalarmdotcomajax.websockets.handler.garage_door import GarageDoorWebSocketHandler
 from pyalarmdotcomajax.websockets.handler.gate import GateWebSocketHandler
 from pyalarmdotcomajax.websockets.handler.light import LightWebSocketHandler
+from pyalarmdotcomajax.websockets.handler.lock import LockWebSocketHandler
 from pyalarmdotcomajax.websockets.handler.partition import PartitionWebSocketHandler
 from pyalarmdotcomajax.websockets.handler.sensor import SensorWebSocketHandler
 from pyalarmdotcomajax.websockets.handler.thermostat import ThermostatWebSocketHandler
 from pyalarmdotcomajax.websockets.handler.water_sensor import (
     WaterSensorWebSocketHandler,
 )
 from pyalarmdotcomajax.websockets.messages import (
@@ -179,14 +184,16 @@
             match message.device:
                 case Light():
                     await LightWebSocketHandler().process_message(message)
                 case Sensor():
                     await SensorWebSocketHandler().process_message(message)
                 case Partition():
                     await PartitionWebSocketHandler().process_message(message)
+                case Lock():
+                    await LockWebSocketHandler().process_message(message)
                 case GarageDoor():
                     await GarageDoorWebSocketHandler().process_message(message)
                 case Gate():
                     await GateWebSocketHandler().process_message(message)
                 case Thermostat():
                     await ThermostatWebSocketHandler().process_message(message)
                 case WaterSensor():
```

### Comparing `pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/websockets/const.py` & `pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/websockets/const.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/websockets/handler/__init__.py` & `pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/websockets/handler/__init__.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/websockets/handler/garage_door.py` & `pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/websockets/handler/garage_door.py`

 * *Files 13% similar despite different names*

```diff
@@ -17,32 +17,40 @@
 
 
 class GarageDoorWebSocketHandler(BaseWebSocketHandler):
     """Base class for device-type-specific websocket message handler."""
 
     SUPPORTED_DEVICE_TYPE = GarageDoor
 
-    EVENT_TO_STATE_MAP = {
-        EventType.Opened: GarageDoor.DeviceState.OPEN.value,
-        EventType.Closed: GarageDoor.DeviceState.CLOSED.value,
+    EVENT_STATE_MAP = {
+        EventType.Opened: GarageDoor.DeviceState.OPEN,
+        EventType.Closed: GarageDoor.DeviceState.CLOSED,
     }
 
     async def process_message(self, message: WebSocketMessage) -> None:
         """Handle websocket message."""
 
         # www.alarm.com\web\system\assets\customer-ember\websockets\handlers\garage-doors.ts
 
         if type(message.device) != GarageDoor:
             return
 
         match message:
             case StatusChangeMessage():
-                if message.new_state:
-                    await message.device.async_handle_external_state_change(message.new_state)
+                await message.device.async_handle_external_dual_state_change(message.new_state)
 
             case EventMessage():
-                log.debug("Ignoring message. Already handled in separate status change message.")
+                match message.event_type:
+                    case EventType.Opened | EventType.Closed:
+                        await message.device.async_handle_external_dual_state_change(
+                            self.EVENT_STATE_MAP[message.event_type]
+                        )
+                    case _:
+                        log.debug(
+                            f"Support for event {message.event_type} ({message.event_type_id}) not yet implemented"
+                            f" by {self.SUPPORTED_DEVICE_TYPE.__name__}."
+                        )
 
             case _:
                 log.debug(
                     f"Support for {type(message)} not yet implemented by {self.SUPPORTED_DEVICE_TYPE.__name__}."
                 )
```

### Comparing `pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/websockets/handler/gate.py` & `pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/websockets/handler/lock.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,48 +1,54 @@
-"""Gate websocket message handler."""
+"""Lock websocket message handler."""
 
 from __future__ import annotations
 
 import logging
 
-from pyalarmdotcomajax.devices.gate import Gate
+from pyalarmdotcomajax.devices.lock import Lock
 from pyalarmdotcomajax.websockets.const import EventType
 from pyalarmdotcomajax.websockets.handler import BaseWebSocketHandler
 from pyalarmdotcomajax.websockets.messages import (
     EventMessage,
     StatusChangeMessage,
     WebSocketMessage,
 )
 
 log = logging.getLogger(__name__)
 
 
-class GateWebSocketHandler(BaseWebSocketHandler):
+class LockWebSocketHandler(BaseWebSocketHandler):
     """Base class for device-type-specific websocket message handler."""
 
-    SUPPORTED_DEVICE_TYPE = Gate
+    SUPPORTED_DEVICE_TYPE = Lock
 
-    EVENT_TO_STATE_MAP = {
-        EventType.Opened: Gate.DeviceState.OPEN.value,
-        EventType.Closed: Gate.DeviceState.CLOSED.value,
+    EVENT_STATE_MAP = {
+        EventType.DoorLocked: Lock.DeviceState.LOCKED,
+        EventType.DoorUnlocked: Lock.DeviceState.UNLOCKED,
     }
 
     async def process_message(self, message: WebSocketMessage) -> None:
         """Handle websocket message."""
 
-        # www.alarm.com\web\system\assets\customer-ember\websockets\handlers\gates.ts
+        # www.alarm.com\web\system\assets\customer-ember\websockets\handlers\locks.ts
 
-        if type(message.device) != Gate:
+        if type(message.device) != Lock:
             return
 
         match message:
             case StatusChangeMessage():
-                if message.new_state:
-                    await message.device.async_handle_external_state_change(message.new_state)
-
+                await message.device.async_handle_external_dual_state_change(message.new_state)
             case EventMessage():
-                log.debug("Ignoring message. Already handled in separate status change message.")
-
+                match message.event_type:
+                    case EventType.DoorLocked | EventType.DoorUnlocked:
+                        await message.device.async_handle_external_dual_state_change(
+                            self.EVENT_STATE_MAP[message.event_type]
+                        )
+                    case _:
+                        log.debug(
+                            f"Support for event {message.event_type} ({message.event_type_id}) not yet implemented"
+                            f" by {self.SUPPORTED_DEVICE_TYPE.__name__}."
+                        )
             case _:
                 log.debug(
                     f"Support for {type(message)} not yet implemented by {self.SUPPORTED_DEVICE_TYPE.__name__}."
                 )
```

### Comparing `pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/websockets/handler/light.py` & `pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/websockets/handler/water_sensor.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,68 +1,53 @@
-"""Light websocket message handler."""
+"""WaterSensor websocket message handler."""
 
 from __future__ import annotations
 
 import logging
 
-from pyalarmdotcomajax.devices.light import Light
-from pyalarmdotcomajax.websockets.const import EventType, PropertyChangeType
+from pyalarmdotcomajax.devices.water_sensor import WaterSensor
+from pyalarmdotcomajax.websockets.const import EventType
 from pyalarmdotcomajax.websockets.handler import BaseWebSocketHandler
 from pyalarmdotcomajax.websockets.messages import (
     EventMessage,
-    PropertyChangeMessage,
     StatusChangeMessage,
     WebSocketMessage,
 )
 
 log = logging.getLogger(__name__)
 
 
-class LightWebSocketHandler(BaseWebSocketHandler):
+class WaterSensorWebSocketHandler(BaseWebSocketHandler):
     """Base class for device-type-specific websocket message handler."""
 
-    SUPPORTED_DEVICE_TYPE = Light
+    SUPPORTED_DEVICE_TYPE = WaterSensor
 
-    STATE_MAP = {
-        0: Light.DeviceState.OFF.value,
-        1: Light.DeviceState.ON.value,
+    EVENT_STATE_MAP = {
+        EventType.Opened: WaterSensor.DeviceState.WET,
+        EventType.Closed: WaterSensor.DeviceState.DRY,
     }
 
     async def process_message(self, message: WebSocketMessage) -> None:
         """Handle websocket message."""
 
-        # www.alarm.com\web\system\assets\customer-ember\websockets\handlers\lights.ts
+        # www.alarm.com\web\system\assets\customer-ember\websockets\handlers\water_sensors.ts
 
-        if type(message.device) != Light:
+        if type(message.device) != WaterSensor:
             return
 
         match message:
-            case PropertyChangeMessage():
-                match message.property:
-                    case PropertyChangeType.LightColor:
-                        # RGBW light not currently supported by library.
-                        pass
             case StatusChangeMessage():
-                if message.new_state in self.STATE_MAP:
-                    await message.device.async_handle_external_state_change(self.STATE_MAP[message.new_state])
-                else:
-                    log.exception(
-                        f"{self.__class__.__name__}: Failed to update"
-                        f" {message.device.name} ({message.device.id_}). Unknown state: {message.new_state}."
-                    )
+                await message.device.async_handle_external_dual_state_change(message.new_state)
+
             case EventMessage():
                 match message.event_type:
-                    case EventType.SwitchLevelChanged:
-                        if message.value:
-                            await message.device.async_handle_external_attribute_change(
-                                {message.device.ATTRIB_LIGHT_LEVEL: int(message.value)}
-                            )
-                            await message.device.async_log_new_attribute("brightness", message.device.brightness)
-                    case EventType.LightTurnedOff | EventType.LightTurnedOn:
-                        log.debug("Ignoring message. Already handled in separate status change message.")
+                    case EventType.Opened | EventType.Closed:
+                        await message.device.async_handle_external_dual_state_change(
+                            self.EVENT_STATE_MAP[message.event_type]
+                        )
                     case _:
                         log.debug(
                             f"Support for event {message.event_type} ({message.event_type_id}) not yet implemented"
                             f" by {self.SUPPORTED_DEVICE_TYPE.__name__}."
                         )
             case _:
                 log.debug(
```

### Comparing `pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/websockets/handler/lock.py` & `pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/websockets/handler/gate.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,46 +1,57 @@
-"""Lock websocket message handler."""
+"""Gate websocket message handler."""
 
 from __future__ import annotations
 
 import logging
 
-from pyalarmdotcomajax.devices.lock import Lock
+from pyalarmdotcomajax.devices.gate import Gate
 from pyalarmdotcomajax.websockets.const import EventType
 from pyalarmdotcomajax.websockets.handler import BaseWebSocketHandler
 from pyalarmdotcomajax.websockets.messages import (
     EventMessage,
     StatusChangeMessage,
     WebSocketMessage,
 )
 
 log = logging.getLogger(__name__)
 
 
-class LockWebSocketHandler(BaseWebSocketHandler):
+class GateWebSocketHandler(BaseWebSocketHandler):
     """Base class for device-type-specific websocket message handler."""
 
-    SUPPORTED_DEVICE_TYPE = Lock
+    SUPPORTED_DEVICE_TYPE = Gate
 
     EVENT_STATE_MAP = {
-        EventType.DoorLocked: Lock.DeviceState.LOCKED,
-        EventType.DoorUnlocked: Lock.DeviceState.UNLOCKED,
+        EventType.Opened: Gate.DeviceState.OPEN,
+        EventType.Closed: Gate.DeviceState.CLOSED,
     }
 
     async def process_message(self, message: WebSocketMessage) -> None:
         """Handle websocket message."""
 
-        # www.alarm.com\web\system\assets\customer-ember\websockets\handlers\locks.ts
+        # www.alarm.com\web\system\assets\customer-ember\websockets\handlers\gates.ts
 
-        if type(message.device) != Lock:
+        if type(message.device) != Gate:
             return
 
         match message:
             case StatusChangeMessage():
                 if message.new_state:
-                    await message.device.async_handle_external_state_change(int(message.new_state))
+                    await message.device.async_handle_external_dual_state_change(message.new_state)
+
             case EventMessage():
-                log.debug("Ignoring message. Already handled in separate status change message.")
+                match message.event_type:
+                    case EventType.Opened | EventType.Closed:
+                        await message.device.async_handle_external_dual_state_change(
+                            self.EVENT_STATE_MAP[message.event_type]
+                        )
+                    case _:
+                        log.debug(
+                            f"Support for event {message.event_type} ({message.event_type_id}) not yet implemented"
+                            f" by {self.SUPPORTED_DEVICE_TYPE.__name__}."
+                        )
+
             case _:
                 log.debug(
                     f"Support for {type(message)} not yet implemented by {self.SUPPORTED_DEVICE_TYPE.__name__}."
                 )
```

### Comparing `pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/websockets/handler/partition.py` & `pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/websockets/handler/partition.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,33 +17,33 @@
 
 class PartitionWebSocketHandler(BaseWebSocketHandler):
     """Base class for device-type-specific websocket message handler."""
 
     SUPPORTED_DEVICE_TYPE = Partition
 
     EVENT_TO_STATE_MAP = {
-        EventType.Disarmed: Partition.DeviceState.DISARMED.value,
-        EventType.ArmedAway: Partition.DeviceState.ARMED_AWAY.value,
-        EventType.ArmedStay: Partition.DeviceState.ARMED_STAY.value,
-        EventType.ArmedNight: Partition.DeviceState.ARMED_NIGHT.value,
+        EventType.Disarmed: Partition.DeviceState.DISARMED,
+        EventType.ArmedAway: Partition.DeviceState.ARMED_AWAY,
+        EventType.ArmedStay: Partition.DeviceState.ARMED_STAY,
+        EventType.ArmedNight: Partition.DeviceState.ARMED_NIGHT,
     }
 
     async def process_message(self, message: WebSocketMessage) -> None:
         """Handle websocket message."""
 
         # www.alarm.com\web\system\assets\customer-ember\websockets\handlers\partitions.ts
 
         if type(message.device) != Partition:
             return
 
         match message:
             case EventMessage():
                 match message.event_type:
                     case EventType.Disarmed | EventType.ArmedAway | EventType.ArmedStay | EventType.ArmedNight:
-                        await message.device.async_handle_external_state_change(
+                        await message.device.async_handle_external_dual_state_change(
                             self.EVENT_TO_STATE_MAP[message.event_type]
                         )
                     case EventType.Alarm | EventType.PolicePanic:
                         # TODO: Support these alarm events. These do not trigger a state change on ADC but rather trigger a notification.
                         log.debug(
                             f"Support for event {message.event_type} ({message.event_type_id}) not yet implemented"
                             f" by {self.SUPPORTED_DEVICE_TYPE.__name__}."
```

### Comparing `pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/websockets/handler/sensor.py` & `pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/websockets/handler/sensor.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,65 +11,68 @@
 from pyalarmdotcomajax.websockets.messages import (
     EventMessage,
     WebSocketMessage,
 )
 
 log = logging.getLogger(__name__)
 
+MOTION_EVENT_STATE_MAP = {
+    EventType.Closed: Sensor.DeviceState.IDLE,
+    EventType.OpenedClosed: Sensor.DeviceState.IDLE,
+    EventType.Opened: Sensor.DeviceState.ACTIVE,
+}
+SENSOR_EVENT_STATE_MAP = {
+    EventType.Closed: Sensor.DeviceState.CLOSED,
+    EventType.OpenedClosed: Sensor.DeviceState.CLOSED,
+    EventType.Opened: Sensor.DeviceState.OPEN,
+}
+
 
 class SensorWebSocketHandler(BaseWebSocketHandler):
     """Base class for device-type-specific websocket message handler."""
 
     # www.alarm.com\web\system\assets\customer-ember\websockets\handlers\sensors.ts
 
     SUPPORTED_DEVICE_TYPE = Sensor
 
-    async def async_get_state_from_event_type(self, message: EventMessage) -> int:
+    def get_state_from_event_type(self, message: EventMessage) -> Sensor.DeviceState:
         """Get sensor state from websocket message event type."""
 
+        if not message.event_type:
+            return Sensor.DeviceState.UNKNOWN
+
         match message.device.device_subtype:
             case Sensor.Subtype.MOTION_SENSOR:
-                match message.event_type:
-                    case EventType.Closed | EventType.OpenedClosed:
-                        return Sensor.DeviceState.IDLE.value
-                    case EventType.Opened:
-                        return Sensor.DeviceState.ACTIVE.value
+                return MOTION_EVENT_STATE_MAP[message.event_type]
             case _:
-                match message.event_type:
-                    case EventType.Closed | EventType.OpenedClosed:
-                        return Sensor.DeviceState.CLOSED.value
-                    case EventType.Opened:
-                        return Sensor.DeviceState.OPEN.value
-
-        return Sensor.DeviceState.UNKNOWN.value
+                return SENSOR_EVENT_STATE_MAP[message.event_type]
 
     async def process_message(self, message: WebSocketMessage) -> None:
         """Handle websocket message."""
 
         if type(message.device) != Sensor:
             return
 
         match message:
             case EventMessage():
                 match message.event_type:
                     case EventType.Closed | EventType.Opened:
-                        state = await self.async_get_state_from_event_type(message)
-                        await message.device.async_handle_external_state_change(state)
+                        await message.device.async_handle_external_dual_state_change(
+                            self.get_state_from_event_type(message)
+                        )
 
                     case EventType.OpenedClosed:
                         # Lock ensures that state changes are executed in order.
                         lock = asyncio.Lock()
 
                         async with lock:
-                            await message.device.async_handle_external_state_change(Sensor.DeviceState.OPEN.value)
+                            await message.device.async_handle_external_dual_state_change(Sensor.DeviceState.OPEN)
 
                         async with lock:
-                            await message.device.async_handle_external_state_change(
-                                Sensor.DeviceState.CLOSED.value
-                            )
+                            await message.device.async_handle_external_dual_state_change(Sensor.DeviceState.CLOSED)
                     case _:
                         log.debug(
                             f"Support for event {message.event_type} ({message.event_type_id}) not yet implemented"
                             f" by {self.SUPPORTED_DEVICE_TYPE.__name__}."
                         )
             case _:
                 log.debug(
```

### Comparing `pyalarmdotcomajax-0.5.2/pyalarmdotcomajax/websockets/handler/thermostat.py` & `pyalarmdotcomajax-0.5.3/pyalarmdotcomajax/websockets/handler/thermostat.py`

 * *Files 24% similar despite different names*

```diff
@@ -47,61 +47,39 @@
                                 (
                                     message.device.ATTRIB_DESIRED_HEAT_SETPOINT
                                     if message.property == PropertyChangeType.HeatSetPoint
                                     else message.device.ATTRIB_DESIRED_COOL_SETPOINT
                                 ): (message.value / 100),
                             },
                         )
-                        await message.device.async_log_new_attribute(
-                            (
-                                f"{'heat' if message.property == PropertyChangeType.HeatSetPoint else 'cool'} setpoint"
-                            ),
-                            (
-                                message.device.attributes.heat_setpoint
-                                if message.property == PropertyChangeType.HeatSetPoint
-                                else message.device.attributes.cool_setpoint
-                            ),
-                        )
 
                     case PropertyChangeType.AmbientTemperature:
                         await message.device.async_handle_external_attribute_change(
                             {message.device.ATTRIB_AMBIENT_TEMP: message.value / 100},
                         )
-                        await message.device.async_log_new_attribute(
-                            "ambient temperature", message.device.attributes.temp_at_tstat
-                        )
 
             case EventMessage():
-                if not message.value:
-                    log.debug("Malformed message. Missing value.")
-                    return
-
                 match message.event_type:
                     case EventType.ThermostatOffset:
                         await message.device.async_handle_external_attribute_change(
                             {message.device.ATTRIB_SETPOINT_OFFSET: message.value},
                         )
-                        await message.device.async_log_new_attribute(
-                            "setpoint offset", message.device.attributes.setpoint_offset
-                        )
 
                     case EventType.ThermostatModeChanged:
-                        await message.device.async_handle_external_state_change(int(message.value) + 1)
-                        await message.device.async_log_new_attribute("mode", message.device.state)
+                        await message.device.async_handle_external_dual_state_change(
+                            message.device.DeviceState(message.value + 1)
+                        )
 
                     case EventType.ThermostatFanModeChanged:
                         await message.device.async_handle_external_attribute_change(
                             {
                                 message.device.ATTRIB_FAN_MODE: message.value,
                                 message.device.ATTRIB_DESIRED_FAN_MODE: message.value,
                             },
                         )
-                        await message.device.async_log_new_attribute(
-                            "fan mode", message.device.attributes.fan_mode
-                        )
 
                     case EventType.ThermostatSetPointChanged:
                         log.debug("Ignoring message. Already handled in separate status change message.")
 
                     case _:
                         log.debug(
                             f"Support for event {message.event_type} ({message.event_type_id}) not yet implemented"
```

### Comparing `pyalarmdotcomajax-0.5.2/pyalarmdotcomajax.egg-info/PKG-INFO` & `pyalarmdotcomajax-0.5.3/pyalarmdotcomajax.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyalarmdotcomajax
-Version: 0.5.2
+Version: 0.5.3
 Summary: Python Interface for Alarm.com
 Home-page: https://github.com/pyalarmdotcom/pyalarmdotcomajax
 Author: Justin Wong
 Author-email: 46082645+uvjustin@users.noreply.github.com
 Maintainer: Elahd Bar-Shai
 Maintainer-email: 46082645+uvjustin@users.noreply.github.com, 466460+elahd@users.noreply.github.com
 License: MIT
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyalarmdotcomajax Version: 0.5.2 Summary: Python
+Metadata-Version: 2.1 Name: pyalarmdotcomajax Version: 0.5.3 Summary: Python
 Interface for Alarm.com Home-page: https://github.com/pyalarmdotcom/
 pyalarmdotcomajax Author: Justin Wong Author-email:
 46082645+uvjustin@users.noreply.github.com Maintainer: Elahd Bar-Shai
 Maintainer-email: 46082645+uvjustin@users.noreply.github.com,
 466460+elahd@users.noreply.github.com License: MIT Keywords: Alarm.com,Security
 System,Home Assistant Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: English Classifier: Environment :: Web
```

### Comparing `pyalarmdotcomajax-0.5.2/pyalarmdotcomajax.egg-info/SOURCES.txt` & `pyalarmdotcomajax-0.5.3/pyalarmdotcomajax.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.2/pyproject.toml` & `pyalarmdotcomajax-0.5.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.2/setup.cfg` & `pyalarmdotcomajax-0.5.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.2/tests/__init__.py` & `pyalarmdotcomajax-0.5.3/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.2/tests/conftest.py` & `pyalarmdotcomajax-0.5.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.2/tests/test_controller.py` & `pyalarmdotcomajax-0.5.3/tests/test_controller.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.2/tests/test_device_extensions.py` & `pyalarmdotcomajax-0.5.3/tests/test_device_extensions.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.2/tests/test_partition.py` & `pyalarmdotcomajax-0.5.3/tests/test_partition.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.2/tests/test_sensors.py` & `pyalarmdotcomajax-0.5.3/tests/test_sensors.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.2/tests/test_thermostat.py` & `pyalarmdotcomajax-0.5.3/tests/test_thermostat.py`

 * *Files identical despite different names*

