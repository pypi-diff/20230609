# Comparing `tmp/hello_robot_stretch_factory-0.4.3.tar.gz` & `tmp/hello_robot_stretch_factory-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hello_robot_stretch_factory-0.4.3.tar", last modified: Fri May  5 11:27:53 2023, max compression
+gzip compressed data, was "hello_robot_stretch_factory-0.4.6.tar", last modified: Fri Jun  9 20:05:37 2023, max compression
```

## Comparing `hello_robot_stretch_factory-0.4.3.tar` & `hello_robot_stretch_factory-0.4.6.tar`

### file list

```diff
@@ -1,59 +1,61 @@
-drwxrwxr-x   0 hello-binit  (1000) hello-binit  (1000)        0 2023-05-05 11:27:53.665849 hello_robot_stretch_factory-0.4.3/
--rw-rw-r--   0 hello-binit  (1000) hello-binit  (1000)      929 2023-05-05 11:27:25.000000 hello_robot_stretch_factory-0.4.3/LICENSE.md
--rw-rw-r--   0 hello-binit  (1000) hello-binit  (1000)      853 2023-05-05 11:27:53.665849 hello_robot_stretch_factory-0.4.3/PKG-INFO
--rw-rw-r--   0 hello-binit  (1000) hello-binit  (1000)      355 2023-05-05 11:27:25.000000 hello_robot_stretch_factory-0.4.3/README.md
-drwxrwxr-x   0 hello-binit  (1000) hello-binit  (1000)        0 2023-05-05 11:27:53.661849 hello_robot_stretch_factory-0.4.3/hello_robot_stretch_factory.egg-info/
--rw-rw-r--   0 hello-binit  (1000) hello-binit  (1000)      853 2023-05-05 11:27:53.000000 hello_robot_stretch_factory-0.4.3/hello_robot_stretch_factory.egg-info/PKG-INFO
--rw-rw-r--   0 hello-binit  (1000) hello-binit  (1000)     1796 2023-05-05 11:27:53.000000 hello_robot_stretch_factory-0.4.3/hello_robot_stretch_factory.egg-info/SOURCES.txt
--rw-rw-r--   0 hello-binit  (1000) hello-binit  (1000)        1 2023-05-05 11:27:53.000000 hello_robot_stretch_factory-0.4.3/hello_robot_stretch_factory.egg-info/dependency_links.txt
--rw-rw-r--   0 hello-binit  (1000) hello-binit  (1000)       74 2023-05-05 11:27:53.000000 hello_robot_stretch_factory-0.4.3/hello_robot_stretch_factory.egg-info/requires.txt
--rw-rw-r--   0 hello-binit  (1000) hello-binit  (1000)       16 2023-05-05 11:27:53.000000 hello_robot_stretch_factory-0.4.3/hello_robot_stretch_factory.egg-info/top_level.txt
--rw-rw-r--   0 hello-binit  (1000) hello-binit  (1000)       38 2023-05-05 11:27:53.665849 hello_robot_stretch_factory-0.4.3/setup.cfg
--rw-rw-r--   0 hello-binit  (1000) hello-binit  (1000)      995 2023-05-05 11:27:25.000000 hello_robot_stretch_factory-0.4.3/setup.py
-drwxrwxr-x   0 hello-binit  (1000) hello-binit  (1000)        0 2023-05-05 11:27:53.665849 hello_robot_stretch_factory-0.4.3/stretch_factory/
--rw-rw-r--   0 hello-binit  (1000) hello-binit  (1000)        0 2023-05-05 11:27:25.000000 hello_robot_stretch_factory-0.4.3/stretch_factory/__init__.py
--rw-rw-r--   0 hello-binit  (1000) hello-binit  (1000)     6326 2023-05-05 11:27:25.000000 hello_robot_stretch_factory-0.4.3/stretch_factory/device_mgmt.py
--rw-rw-r--   0 hello-binit  (1000) hello-binit  (1000)     4641 2023-05-05 11:27:25.000000 hello_robot_stretch_factory-0.4.3/stretch_factory/firmware_available.py
--rw-rw-r--   0 hello-binit  (1000) hello-binit  (1000)     5248 2023-05-05 11:27:25.000000 hello_robot_stretch_factory-0.4.3/stretch_factory/firmware_installed.py
--rw-rw-r--   0 hello-binit  (1000) hello-binit  (1000)     3861 2023-05-05 11:27:25.000000 hello_robot_stretch_factory-0.4.3/stretch_factory/firmware_recommended.py
--rw-rw-r--   0 hello-binit  (1000) hello-binit  (1000)    37747 2023-05-05 11:27:25.000000 hello_robot_stretch_factory-0.4.3/stretch_factory/firmware_updater.py
--rw-rw-r--   0 hello-binit  (1000) hello-binit  (1000)     5254 2023-05-05 11:27:25.000000 hello_robot_stretch_factory-0.4.3/stretch_factory/firmware_utils.py
--rw-rw-r--   0 hello-binit  (1000) hello-binit  (1000)     2726 2023-05-05 11:27:25.000000 hello_robot_stretch_factory-0.4.3/stretch_factory/firmware_version.py
--rw-rw-r--   0 hello-binit  (1000) hello-binit  (1000)    22204 2023-05-05 11:27:25.000000 hello_robot_stretch_factory-0.4.3/stretch_factory/hello_device_utils.py
--rw-rw-r--   0 hello-binit  (1000) hello-binit  (1000)    12828 2023-05-05 11:27:25.000000 hello_robot_stretch_factory-0.4.3/stretch_factory/param_mgmt.py
-drwxrwxr-x   0 hello-binit  (1000) hello-binit  (1000)        0 2023-05-05 11:27:53.665849 hello_robot_stretch_factory-0.4.3/test/
--rw-rw-r--   0 hello-binit  (1000) hello-binit  (1000)      685 2023-05-05 11:27:25.000000 hello_robot_stretch_factory-0.4.3/test/test_firmware_updater.py
--rw-rw-r--   0 hello-binit  (1000) hello-binit  (1000)      668 2023-05-05 11:27:25.000000 hello_robot_stretch_factory-0.4.3/test/test_usb_reset.py
-drwxrwxr-x   0 hello-binit  (1000) hello-binit  (1000)        0 2023-05-05 11:27:53.661849 hello_robot_stretch_factory-0.4.3/tools/
--rwxrwxr-x   0 hello-binit  (1000) hello-binit  (1000)     2456 2023-05-05 11:27:25.000000 hello_robot_stretch_factory-0.4.3/tools/RE1_migrate_contacts.py
--rwxrwxr-x   0 hello-binit  (1000) hello-binit  (1000)     6621 2023-05-05 11:27:25.000000 hello_robot_stretch_factory-0.4.3/tools/RE1_migrate_params.py
--rwxrwxr-x   0 hello-binit  (1000) hello-binit  (1000)    22012 2023-05-05 11:27:25.000000 hello_robot_stretch_factory-0.4.3/tools/REx_D435i_check.py
--rwxrwxr-x   0 hello-binit  (1000) hello-binit  (1000)     5418 2023-05-05 11:27:25.000000 hello_robot_stretch_factory-0.4.3/tools/REx_base_calibrate_imu_collect.py
--rwxrwxr-x   0 hello-binit  (1000) hello-binit  (1000)    32027 2023-05-05 11:27:25.000000 hello_robot_stretch_factory-0.4.3/tools/REx_base_calibrate_imu_process.py
--rwxrwxr-x   0 hello-binit  (1000) hello-binit  (1000)     5950 2023-05-05 11:27:25.000000 hello_robot_stretch_factory-0.4.3/tools/REx_base_calibrate_wheel_separation.py
--rwxrwxr-x   0 hello-binit  (1000) hello-binit  (1000)     4771 2023-05-05 11:27:25.000000 hello_robot_stretch_factory-0.4.3/tools/REx_calibrate_gravity_comp.py
--rwxrwxr-x   0 hello-binit  (1000) hello-binit  (1000)     7456 2023-05-05 11:27:25.000000 hello_robot_stretch_factory-0.4.3/tools/REx_calibrate_guarded_contact.py
--rwxrwxr-x   0 hello-binit  (1000) hello-binit  (1000)     3578 2023-05-05 11:27:25.000000 hello_robot_stretch_factory-0.4.3/tools/REx_calibrate_range.py
--rwxrwxr-x   0 hello-binit  (1000) hello-binit  (1000)     1728 2023-05-05 11:27:25.000000 hello_robot_stretch_factory-0.4.3/tools/REx_cliff_sensor_calibrate.py
--rwxrwxr-x   0 hello-binit  (1000) hello-binit  (1000)    18552 2023-05-05 11:27:25.000000 hello_robot_stretch_factory-0.4.3/tools/REx_discover_hello_devices.py
--rwxrwxr-x   0 hello-binit  (1000) hello-binit  (1000)     1442 2023-05-05 11:27:25.000000 hello_robot_stretch_factory-0.4.3/tools/REx_dynamixel_id_change.py
--rwxrwxr-x   0 hello-binit  (1000) hello-binit  (1000)     1354 2023-05-05 11:27:25.000000 hello_robot_stretch_factory-0.4.3/tools/REx_dynamixel_id_scan.py
--rwxrwxr-x   0 hello-binit  (1000) hello-binit  (1000)     5045 2023-05-05 11:27:25.000000 hello_robot_stretch_factory-0.4.3/tools/REx_dynamixel_jog.py
--rwxrwxr-x   0 hello-binit  (1000) hello-binit  (1000)     1374 2023-05-05 11:27:25.000000 hello_robot_stretch_factory-0.4.3/tools/REx_dynamixel_reboot.py
--rwxrwxr-x   0 hello-binit  (1000) hello-binit  (1000)     1188 2023-05-05 11:27:25.000000 hello_robot_stretch_factory-0.4.3/tools/REx_dynamixel_set_baud.py
--rwxrwxr-x   0 hello-binit  (1000) hello-binit  (1000)     2846 2023-05-05 11:27:25.000000 hello_robot_stretch_factory-0.4.3/tools/REx_firmware_flash.py
--rwxrwxr-x   0 hello-binit  (1000) hello-binit  (1000)     5804 2023-05-05 11:27:25.000000 hello_robot_stretch_factory-0.4.3/tools/REx_firmware_updater.py
--rwxrwxr-x   0 hello-binit  (1000) hello-binit  (1000)     1583 2023-05-05 11:27:25.000000 hello_robot_stretch_factory-0.4.3/tools/REx_gamepad_configure.py
--rwxrwxr-x   0 hello-binit  (1000) hello-binit  (1000)     2338 2023-05-05 11:27:25.000000 hello_robot_stretch_factory-0.4.3/tools/REx_gripper_calibrate.py
--rwxrwxr-x   0 hello-binit  (1000) hello-binit  (1000)     1947 2023-05-05 11:27:25.000000 hello_robot_stretch_factory-0.4.3/tools/REx_hello_dynamixel_jog.py
--rwxrwxr-x   0 hello-binit  (1000) hello-binit  (1000)      870 2023-05-05 11:27:25.000000 hello_robot_stretch_factory-0.4.3/tools/REx_stepper_calibration_YAML_to_flash.py
--rwxrwxr-x   0 hello-binit  (1000) hello-binit  (1000)      735 2023-05-05 11:27:25.000000 hello_robot_stretch_factory-0.4.3/tools/REx_stepper_calibration_flash_to_YAML.py
--rwxrwxr-x   0 hello-binit  (1000) hello-binit  (1000)     1168 2023-05-05 11:27:25.000000 hello_robot_stretch_factory-0.4.3/tools/REx_stepper_calibration_run.py
--rwxrwxr-x   0 hello-binit  (1000) hello-binit  (1000)    18644 2023-05-05 11:27:25.000000 hello_robot_stretch_factory-0.4.3/tools/REx_stepper_ctrl_tuning.py
--rwxrwxr-x   0 hello-binit  (1000) hello-binit  (1000)     1163 2023-05-05 11:27:25.000000 hello_robot_stretch_factory-0.4.3/tools/REx_stepper_gains.py
--rwxrwxr-x   0 hello-binit  (1000) hello-binit  (1000)     4449 2023-05-05 11:27:25.000000 hello_robot_stretch_factory-0.4.3/tools/REx_stepper_jog.py
--rwxrwxr-x   0 hello-binit  (1000) hello-binit  (1000)      852 2023-05-05 11:27:25.000000 hello_robot_stretch_factory-0.4.3/tools/REx_stepper_mechaduino_menu.py
--rwxrwxr-x   0 hello-binit  (1000) hello-binit  (1000)    10577 2023-05-05 11:27:25.000000 hello_robot_stretch_factory-0.4.3/tools/REx_trace_firmware.py
--rwxrwxr-x   0 hello-binit  (1000) hello-binit  (1000)     7819 2023-05-05 11:27:25.000000 hello_robot_stretch_factory-0.4.3/tools/REx_trace_robot.py
--rwxrwxr-x   0 hello-binit  (1000) hello-binit  (1000)     2347 2023-05-05 11:27:25.000000 hello_robot_stretch_factory-0.4.3/tools/REx_usb_reset.py
--rwxrwxr-x   0 hello-binit  (1000) hello-binit  (1000)     1379 2023-05-05 11:27:25.000000 hello_robot_stretch_factory-0.4.3/tools/REx_wacc_calibrate.py
+drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2023-06-09 20:05:37.036178 hello_robot_stretch_factory-0.4.6/
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)      929 2022-08-24 21:41:11.000000 hello_robot_stretch_factory-0.4.6/LICENSE.md
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)      816 2023-06-09 20:05:37.036178 hello_robot_stretch_factory-0.4.6/PKG-INFO
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)      355 2022-09-08 01:34:28.000000 hello_robot_stretch_factory-0.4.6/README.md
+drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2023-06-09 20:05:37.032178 hello_robot_stretch_factory-0.4.6/hello_robot_stretch_factory.egg-info/
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)      816 2023-06-09 20:05:36.000000 hello_robot_stretch_factory-0.4.6/hello_robot_stretch_factory.egg-info/PKG-INFO
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     1852 2023-06-09 20:05:36.000000 hello_robot_stretch_factory-0.4.6/hello_robot_stretch_factory.egg-info/SOURCES.txt
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)        1 2023-06-09 20:05:36.000000 hello_robot_stretch_factory-0.4.6/hello_robot_stretch_factory.egg-info/dependency_links.txt
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)       74 2023-06-09 20:05:36.000000 hello_robot_stretch_factory-0.4.6/hello_robot_stretch_factory.egg-info/requires.txt
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)       16 2023-06-09 20:05:36.000000 hello_robot_stretch_factory-0.4.6/hello_robot_stretch_factory.egg-info/top_level.txt
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)       38 2023-06-09 20:05:37.036178 hello_robot_stretch_factory-0.4.6/setup.cfg
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)      995 2023-06-09 20:04:37.000000 hello_robot_stretch_factory-0.4.6/setup.py
+drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2023-06-09 20:05:37.036178 hello_robot_stretch_factory-0.4.6/stretch_factory/
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)        0 2022-08-24 21:41:11.000000 hello_robot_stretch_factory-0.4.6/stretch_factory/__init__.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     6326 2022-12-27 02:18:42.000000 hello_robot_stretch_factory-0.4.6/stretch_factory/device_mgmt.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     4641 2023-06-09 20:03:58.000000 hello_robot_stretch_factory-0.4.6/stretch_factory/firmware_available.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     5248 2023-06-09 20:03:58.000000 hello_robot_stretch_factory-0.4.6/stretch_factory/firmware_installed.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     3861 2023-06-09 20:03:58.000000 hello_robot_stretch_factory-0.4.6/stretch_factory/firmware_recommended.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    38099 2023-06-09 20:03:58.000000 hello_robot_stretch_factory-0.4.6/stretch_factory/firmware_updater.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     5254 2023-06-09 20:03:58.000000 hello_robot_stretch_factory-0.4.6/stretch_factory/firmware_utils.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     2726 2023-06-09 20:03:58.000000 hello_robot_stretch_factory-0.4.6/stretch_factory/firmware_version.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    22204 2023-06-09 20:03:58.000000 hello_robot_stretch_factory-0.4.6/stretch_factory/hello_device_utils.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    12828 2022-09-08 01:34:28.000000 hello_robot_stretch_factory-0.4.6/stretch_factory/param_mgmt.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     9286 2023-06-09 20:03:58.000000 hello_robot_stretch_factory-0.4.6/stretch_factory/trace_mgmt.py
+drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2023-06-09 20:05:37.036178 hello_robot_stretch_factory-0.4.6/test/
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)      685 2022-08-24 21:41:11.000000 hello_robot_stretch_factory-0.4.6/test/test_firmware_updater.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)      668 2022-08-24 21:41:11.000000 hello_robot_stretch_factory-0.4.6/test/test_usb_reset.py
+drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2023-06-09 20:05:37.032178 hello_robot_stretch_factory-0.4.6/tools/
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     2456 2022-09-08 01:34:28.000000 hello_robot_stretch_factory-0.4.6/tools/RE1_migrate_contacts.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     6621 2022-08-24 21:41:11.000000 hello_robot_stretch_factory-0.4.6/tools/RE1_migrate_params.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)    22012 2023-04-06 22:42:29.000000 hello_robot_stretch_factory-0.4.6/tools/REx_D435i_check.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     5418 2022-09-08 01:34:28.000000 hello_robot_stretch_factory-0.4.6/tools/REx_base_calibrate_imu_collect.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)    32027 2022-09-08 01:33:19.000000 hello_robot_stretch_factory-0.4.6/tools/REx_base_calibrate_imu_process.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     5950 2022-09-08 01:33:19.000000 hello_robot_stretch_factory-0.4.6/tools/REx_base_calibrate_wheel_separation.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     4771 2023-01-19 20:41:45.000000 hello_robot_stretch_factory-0.4.6/tools/REx_calibrate_gravity_comp.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     7456 2023-06-09 20:03:58.000000 hello_robot_stretch_factory-0.4.6/tools/REx_calibrate_guarded_contact.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     3578 2022-12-27 02:18:42.000000 hello_robot_stretch_factory-0.4.6/tools/REx_calibrate_range.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1728 2022-09-08 01:33:19.000000 hello_robot_stretch_factory-0.4.6/tools/REx_cliff_sensor_calibrate.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     5596 2023-06-09 20:03:58.000000 hello_robot_stretch_factory-0.4.6/tools/REx_comm_rates.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)    18552 2023-01-20 00:09:05.000000 hello_robot_stretch_factory-0.4.6/tools/REx_discover_hello_devices.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1442 2022-09-08 01:33:19.000000 hello_robot_stretch_factory-0.4.6/tools/REx_dynamixel_id_change.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1354 2022-09-08 01:33:19.000000 hello_robot_stretch_factory-0.4.6/tools/REx_dynamixel_id_scan.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     5045 2022-12-27 02:18:42.000000 hello_robot_stretch_factory-0.4.6/tools/REx_dynamixel_jog.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1374 2022-09-08 01:33:19.000000 hello_robot_stretch_factory-0.4.6/tools/REx_dynamixel_reboot.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1188 2022-09-08 01:33:19.000000 hello_robot_stretch_factory-0.4.6/tools/REx_dynamixel_set_baud.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     2846 2023-06-09 20:03:58.000000 hello_robot_stretch_factory-0.4.6/tools/REx_firmware_flash.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     5804 2023-06-09 20:03:58.000000 hello_robot_stretch_factory-0.4.6/tools/REx_firmware_updater.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1583 2022-09-08 01:33:19.000000 hello_robot_stretch_factory-0.4.6/tools/REx_gamepad_configure.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     2338 2022-09-08 01:33:19.000000 hello_robot_stretch_factory-0.4.6/tools/REx_gripper_calibrate.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1947 2022-09-08 01:33:19.000000 hello_robot_stretch_factory-0.4.6/tools/REx_hello_dynamixel_jog.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)      870 2022-09-08 01:34:28.000000 hello_robot_stretch_factory-0.4.6/tools/REx_stepper_calibration_YAML_to_flash.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)      735 2023-06-09 20:03:58.000000 hello_robot_stretch_factory-0.4.6/tools/REx_stepper_calibration_flash_to_YAML.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1168 2022-09-08 01:34:28.000000 hello_robot_stretch_factory-0.4.6/tools/REx_stepper_calibration_run.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)    18644 2022-09-08 01:33:19.000000 hello_robot_stretch_factory-0.4.6/tools/REx_stepper_ctrl_tuning.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1163 2022-09-08 01:33:19.000000 hello_robot_stretch_factory-0.4.6/tools/REx_stepper_gains.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     4449 2023-06-09 20:03:58.000000 hello_robot_stretch_factory-0.4.6/tools/REx_stepper_jog.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)      852 2022-09-08 01:33:19.000000 hello_robot_stretch_factory-0.4.6/tools/REx_stepper_mechaduino_menu.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1572 2023-06-09 20:03:58.000000 hello_robot_stretch_factory-0.4.6/tools/REx_trace_firmware.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     7819 2023-04-06 22:42:29.000000 hello_robot_stretch_factory-0.4.6/tools/REx_trace_robot.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     2347 2022-09-08 01:33:19.000000 hello_robot_stretch_factory-0.4.6/tools/REx_usb_reset.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1379 2022-09-08 01:33:19.000000 hello_robot_stretch_factory-0.4.6/tools/REx_wacc_calibrate.py
```

### Comparing `hello_robot_stretch_factory-0.4.3/LICENSE.md` & `hello_robot_stretch_factory-0.4.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.3/PKG-INFO` & `hello_robot_stretch_factory-0.4.6/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: hello_robot_stretch_factory
-Version: 0.4.3
+Version: 0.4.6
 Summary: Stretch Factory Tools
 Home-page: https://github.com/hello-robot/stretch_factory
 Author: Hello Robot Inc.
 Author-email: support@hello-robot.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # Overview
@@ -21,9 +19,7 @@
 
 This package can be installed by:
 
 ```
 python -m pip install  -U hello-robot-stretch-factory
 ```
 
-
-
```

### Comparing `hello_robot_stretch_factory-0.4.3/hello_robot_stretch_factory.egg-info/PKG-INFO` & `hello_robot_stretch_factory-0.4.6/hello_robot_stretch_factory.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: hello-robot-stretch-factory
-Version: 0.4.3
+Version: 0.4.6
 Summary: Stretch Factory Tools
 Home-page: https://github.com/hello-robot/stretch_factory
 Author: Hello Robot Inc.
 Author-email: support@hello-robot.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # Overview
@@ -21,9 +19,7 @@
 
 This package can be installed by:
 
 ```
 python -m pip install  -U hello-robot-stretch-factory
 ```
 
-
-
```

### Comparing `hello_robot_stretch_factory-0.4.3/hello_robot_stretch_factory.egg-info/SOURCES.txt` & `hello_robot_stretch_factory-0.4.6/hello_robot_stretch_factory.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 ./tools/REx_base_calibrate_imu_collect.py
 ./tools/REx_base_calibrate_imu_process.py
 ./tools/REx_base_calibrate_wheel_separation.py
 ./tools/REx_calibrate_gravity_comp.py
 ./tools/REx_calibrate_guarded_contact.py
 ./tools/REx_calibrate_range.py
 ./tools/REx_cliff_sensor_calibrate.py
+./tools/REx_comm_rates.py
 ./tools/REx_discover_hello_devices.py
 ./tools/REx_dynamixel_id_change.py
 ./tools/REx_dynamixel_id_scan.py
 ./tools/REx_dynamixel_jog.py
 ./tools/REx_dynamixel_reboot.py
 ./tools/REx_dynamixel_set_baud.py
 ./tools/REx_firmware_flash.py
@@ -44,9 +45,10 @@
 stretch_factory/firmware_installed.py
 stretch_factory/firmware_recommended.py
 stretch_factory/firmware_updater.py
 stretch_factory/firmware_utils.py
 stretch_factory/firmware_version.py
 stretch_factory/hello_device_utils.py
 stretch_factory/param_mgmt.py
+stretch_factory/trace_mgmt.py
 test/test_firmware_updater.py
 test/test_usb_reset.py
```

### Comparing `hello_robot_stretch_factory-0.4.3/setup.py` & `hello_robot_stretch_factory-0.4.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 script_path='./tools'
 ex_scripts = glob.glob(script_path+'/*.py') + glob.glob(script_path+'/*.sh')
 stretch_scripts=[f for f in ex_scripts if isfile(f)]
 
 setuptools.setup(
     name="hello_robot_stretch_factory",
-    version="0.4.3",
+    version="0.4.6",
     author="Hello Robot Inc.",
     author_email="support@hello-robot.com",
     description="Stretch Factory Tools",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/hello-robot/stretch_factory",
     scripts = stretch_scripts,
```

### Comparing `hello_robot_stretch_factory-0.4.3/stretch_factory/device_mgmt.py` & `hello_robot_stretch_factory-0.4.6/stretch_factory/device_mgmt.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.3/stretch_factory/firmware_available.py` & `hello_robot_stretch_factory-0.4.6/stretch_factory/firmware_available.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.3/stretch_factory/firmware_installed.py` & `hello_robot_stretch_factory-0.4.6/stretch_factory/firmware_installed.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.3/stretch_factory/firmware_recommended.py` & `hello_robot_stretch_factory-0.4.6/stretch_factory/firmware_recommended.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.3/stretch_factory/firmware_updater.py` & `hello_robot_stretch_factory-0.4.6/stretch_factory/firmware_updater.py`

 * *Files 1% similar despite different names*

```diff
@@ -527,16 +527,21 @@
                     device_name.upper(), str(self.fw_installed.get_version(device_name))), fg="blue", bold=True)
                     default_id = 0
                     for i in range(len(vs)):
                         if vs[i] == self.fw_recommended.recommended[device_name]:
                             default_id = i
                         print('%d: %s' % (i, vs[i]))
                     print('----------------------')
-
-                    self.target[device_name] = vt
+                    id = click.prompt('Please enter desired version id [Recommended]', default=default_id)
+                    if id >= 0 and id < len(vs):
+                        vt = vs[id]
+                    else:
+                        click.secho('Invalid ID', fg="red")
+                print('Selected version %s for device %s' % (vt, device_name))
+                self.target[device_name] = vt
         print('')
         print('')
         return True
 
     def set_target_from_install_path(self, path_name):
         # Burn the Head of the branch to each board regardless of what is currently installed
         click.secho('>>> Flashing firmware from path %s ' % path_name, fg="cyan", bold=True)
```

### Comparing `hello_robot_stretch_factory-0.4.3/stretch_factory/firmware_utils.py` & `hello_robot_stretch_factory-0.4.6/stretch_factory/firmware_utils.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.3/stretch_factory/firmware_version.py` & `hello_robot_stretch_factory-0.4.6/stretch_factory/firmware_version.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.3/stretch_factory/hello_device_utils.py` & `hello_robot_stretch_factory-0.4.6/stretch_factory/hello_device_utils.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.3/stretch_factory/param_mgmt.py` & `hello_robot_stretch_factory-0.4.6/stretch_factory/param_mgmt.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.3/test/test_firmware_updater.py` & `hello_robot_stretch_factory-0.4.6/test/test_firmware_updater.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.3/test/test_usb_reset.py` & `hello_robot_stretch_factory-0.4.6/test/test_usb_reset.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.3/tools/RE1_migrate_contacts.py` & `hello_robot_stretch_factory-0.4.6/tools/RE1_migrate_contacts.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.3/tools/RE1_migrate_params.py` & `hello_robot_stretch_factory-0.4.6/tools/RE1_migrate_params.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.3/tools/REx_D435i_check.py` & `hello_robot_stretch_factory-0.4.6/tools/REx_D435i_check.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.3/tools/REx_base_calibrate_imu_collect.py` & `hello_robot_stretch_factory-0.4.6/tools/REx_base_calibrate_imu_collect.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.3/tools/REx_base_calibrate_imu_process.py` & `hello_robot_stretch_factory-0.4.6/tools/REx_base_calibrate_imu_process.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.3/tools/REx_base_calibrate_wheel_separation.py` & `hello_robot_stretch_factory-0.4.6/tools/REx_base_calibrate_wheel_separation.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.3/tools/REx_calibrate_gravity_comp.py` & `hello_robot_stretch_factory-0.4.6/tools/REx_calibrate_gravity_comp.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.3/tools/REx_calibrate_guarded_contact.py` & `hello_robot_stretch_factory-0.4.6/tools/REx_calibrate_guarded_contact.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.3/tools/REx_calibrate_range.py` & `hello_robot_stretch_factory-0.4.6/tools/REx_calibrate_range.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.3/tools/REx_cliff_sensor_calibrate.py` & `hello_robot_stretch_factory-0.4.6/tools/REx_cliff_sensor_calibrate.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.3/tools/REx_discover_hello_devices.py` & `hello_robot_stretch_factory-0.4.6/tools/REx_discover_hello_devices.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.3/tools/REx_dynamixel_id_change.py` & `hello_robot_stretch_factory-0.4.6/tools/REx_dynamixel_id_change.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.3/tools/REx_dynamixel_id_scan.py` & `hello_robot_stretch_factory-0.4.6/tools/REx_dynamixel_id_scan.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.3/tools/REx_dynamixel_jog.py` & `hello_robot_stretch_factory-0.4.6/tools/REx_dynamixel_jog.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.3/tools/REx_dynamixel_reboot.py` & `hello_robot_stretch_factory-0.4.6/tools/REx_dynamixel_reboot.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.3/tools/REx_dynamixel_set_baud.py` & `hello_robot_stretch_factory-0.4.6/tools/REx_dynamixel_set_baud.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.3/tools/REx_firmware_flash.py` & `hello_robot_stretch_factory-0.4.6/tools/REx_firmware_flash.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.3/tools/REx_firmware_updater.py` & `hello_robot_stretch_factory-0.4.6/tools/REx_firmware_updater.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.3/tools/REx_gamepad_configure.py` & `hello_robot_stretch_factory-0.4.6/tools/REx_gamepad_configure.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.3/tools/REx_gripper_calibrate.py` & `hello_robot_stretch_factory-0.4.6/tools/REx_gripper_calibrate.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.3/tools/REx_hello_dynamixel_jog.py` & `hello_robot_stretch_factory-0.4.6/tools/REx_hello_dynamixel_jog.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.3/tools/REx_stepper_calibration_YAML_to_flash.py` & `hello_robot_stretch_factory-0.4.6/tools/REx_stepper_calibration_YAML_to_flash.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.3/tools/REx_stepper_calibration_flash_to_YAML.py` & `hello_robot_stretch_factory-0.4.6/tools/REx_stepper_calibration_flash_to_YAML.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.3/tools/REx_stepper_calibration_run.py` & `hello_robot_stretch_factory-0.4.6/tools/REx_stepper_calibration_run.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.3/tools/REx_stepper_ctrl_tuning.py` & `hello_robot_stretch_factory-0.4.6/tools/REx_stepper_ctrl_tuning.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.3/tools/REx_stepper_gains.py` & `hello_robot_stretch_factory-0.4.6/tools/REx_stepper_gains.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.3/tools/REx_stepper_jog.py` & `hello_robot_stretch_factory-0.4.6/tools/REx_stepper_jog.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.3/tools/REx_stepper_mechaduino_menu.py` & `hello_robot_stretch_factory-0.4.6/tools/REx_stepper_mechaduino_menu.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.3/tools/REx_trace_firmware.py` & `hello_robot_stretch_factory-0.4.6/stretch_factory/trace_mgmt.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,60 +1,18 @@
 #!/usr/bin/env python
-import argparse
+
 import click
 from colorama import Style
 import glob
-from datetime import datetime
 import matplotlib.pyplot as plt
-import numpy as np
-import stretch_body.pimu
-import stretch_body.wacc
-import stretch_body.stepper
-
 import stretch_body.hello_utils as hu
 from os import makedirs
 import yaml
 from yaml import CDumper as Dumper
 
-hu.print_stretch_re_use()
-
-parser = argparse.ArgumentParser(description='Tool to load and view the firmware trace data.', )
-group = parser.add_mutually_exclusive_group()
-group.add_argument("--pimu", help="Trace Pimu firmware", action="store_true")
-group.add_argument("--wacc", help="Trace Wacc firmware", action="store_true")
-group.add_argument("--arm", help="Trace Arm Stepper firmware", action="store_true")
-group.add_argument("--lift", help="Trace Lift Stepper firmware", action="store_true")
-group.add_argument("--left_wheel", help="Trace Left Wheel Stepper firmware", action="store_true")
-group.add_argument("--right_wheel", help="Trace Right Wheel Stepper firmware", action="store_true")
-args = parser.parse_args()
-
-if not (args.pimu or args.wacc or args.arm or args.lift or args.left_wheel or args.right_wheel):
-    print('Device argument required')
-    exit(0)
-
-if args.pimu:
-    device=stretch_body.pimu.Pimu()
-if args.wacc:
-    device=stretch_body.wacc.Wacc()
-if args.arm:
-    device=stretch_body.stepper.Stepper('/dev/hello-motor-arm')
-if args.lift:
-    device=stretch_body.stepper.Stepper('/dev/hello-motor-lift')
-if args.left_wheel:
-    device=stretch_body.stepper.Stepper('/dev/hello-motor-left-wheel')
-if args.right_wheel:
-    device=stretch_body.stepper.Stepper('/dev/hello-motor-right-wheel')
-
-
-
-device.startup()
-# if not robot.startup():
-#     exit(1)
-
-
 class TraceMgmt:
     """
     Manage trace data
     """
     def __init__(self,device):
         self.device=device
         self.device_name = device.name
@@ -100,14 +58,15 @@
             print('Enter command. (q to quit)')
             print('r: record trace on device')
             print('d: load trace from device')
             print('l: load trace from file')
             print('s: save trace to file')
             print('y: display trace data')
             print('x: print trace to console')
+            print('q: quit')
             print('-------------------------------------')
             #try:
             r = input()
             if r == 'q' or r == 'Q':
                 return
             elif r=='r':
                 trace_data=self.record_trace()
@@ -118,30 +77,30 @@
             elif r == 's':
                 self.save_trace(trace_data)
             elif r == 'y':
                 self.display_trace(trace_data)
             elif r== 'x':
                 print(trace_data)
             else:
-                print('Invalid entry')
+                self.device.pull_status()
+                self.device.pretty_print()
             # except(TypeError, ValueError):
             #     print('Invalid entry')
 
     def record_trace(self):
         print('')
         dd=None
 
         input("Hit enter to begin recording")
         self.device.enable_firmware_trace()
         self.device.push_command()
         print('\nRecording...\n')
         input("Hit enter to end recording")
         self.device.disable_firmware_trace()
         self.device.push_command()
-
         print('Reading trace back from recording. This may take a minute...')
         trace_data = self.device.read_firmware_trace()
         if len(trace_data)==0:
             print('No trace data found for %s'%self.device_name)
         return trace_data
 
     def load_trace_from_file(self):
@@ -200,15 +159,16 @@
                 data.append(k['print']['x'])
             print('---------- PLOT DATA ----------')
             print(data)
             print('')
 
             plt.ion()  # enable interactivity
             fig, axes = plt.subplots(1, 1, figsize=(15.0, 8.0), sharex=True)
-            fig.canvas.set_window_title('TRACE %s | %s' % (self.device_name.upper(), 'X'))
+            if fig.canvas.manager is not None:
+                fig.canvas.manager.set_window_title('TRACE %s | %s' % (self.device_name.upper(), field_name.upper()))
             axes.set_yscale('linear')
             axes.set_xlabel('Sample')
             axes.set_ylabel('X')
             axes.grid(True)
             axes.plot(data, 'b')
             fig.canvas.draw_idle()
 
@@ -233,15 +193,16 @@
             data.append(t['debug'][field_name])
         print('---------- PLOT DATA ----------')
         print(data)
         print('')
 
         plt.ion()  # enable interactivity
         fig, axes = plt.subplots(1, 1, figsize=(15.0, 8.0), sharex=True)
-        fig.canvas.set_window_title('TRACE %s | %s'%(self.device_name.upper(),field_name.upper()))
+        if fig.canvas.manager is not None:
+            fig.canvas.manager.set_window_title('TRACE %s | %s' % (self.device_name.upper(), field_name.upper()))
         axes.set_yscale('linear')
         axes.set_xlabel('Sample')
         axes.set_ylabel(field_name.upper())
         axes.grid(True)
         axes.plot(data, 'b')
         fig.canvas.draw_idle()
 
@@ -266,18 +227,15 @@
             data.append(t['status'][field_name])
         print('---------- PLOT DATA ----------')
         print(data)
         print('')
 
         plt.ion()  # enable interactivity
         fig, axes = plt.subplots(1, 1, figsize=(15.0, 8.0), sharex=True)
-        fig.canvas.set_window_title('TRACE %s | %s'%(self.device_name.upper(),field_name.upper()))
+        if fig.canvas.manager is not None:
+            fig.canvas.manager.set_window_title('TRACE %s | %s' % (self.device_name.upper(), field_name.upper()))
         axes.set_yscale('linear')
         axes.set_xlabel('Sample')
         axes.set_ylabel(field_name.upper())
         axes.grid(True)
         axes.plot(data, 'b')
         fig.canvas.draw_idle()
-
-
-mgmt=TraceMgmt(device)
-mgmt.run_menu()
```

### Comparing `hello_robot_stretch_factory-0.4.3/tools/REx_trace_robot.py` & `hello_robot_stretch_factory-0.4.6/tools/REx_trace_robot.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.3/tools/REx_usb_reset.py` & `hello_robot_stretch_factory-0.4.6/tools/REx_usb_reset.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.3/tools/REx_wacc_calibrate.py` & `hello_robot_stretch_factory-0.4.6/tools/REx_wacc_calibrate.py`

 * *Files identical despite different names*

