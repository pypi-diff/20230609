# Comparing `tmp/Appium-Python-Client-2.8.1.tar.gz` & `tmp/Appium-Python-Client-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Appium-Python-Client-2.8.1.tar", last modified: Sat Jan 21 04:10:49 2023, max compression
+gzip compressed data, was "Appium-Python-Client-2.9.0.tar", last modified: Sun Apr  2 05:24:29 2023, max compression
```

## Comparing `Appium-Python-Client-2.8.1.tar` & `Appium-Python-Client-2.9.0.tar`

### file list

```diff
@@ -1,448 +1,448 @@
-drwxr-xr-x   0 kazuaki    (501) staff       (20)        0 2023-01-21 04:10:49.261104 Appium-Python-Client-2.8.1/
-drwxr-xr-x   0 kazuaki    (501) staff       (20)        0 2023-01-21 04:10:48.833687 Appium-Python-Client-2.8.1/Appium_Python_Client.egg-info/
--rw-r--r--   0 kazuaki    (501) staff       (20)    10891 2023-01-21 04:10:48.000000 Appium-Python-Client-2.8.1/Appium_Python_Client.egg-info/PKG-INFO
--rw-r--r--   0 kazuaki    (501) staff       (20)    20768 2023-01-21 04:10:48.000000 Appium-Python-Client-2.8.1/Appium_Python_Client.egg-info/SOURCES.txt
--rw-r--r--   0 kazuaki    (501) staff       (20)        1 2023-01-21 04:10:48.000000 Appium-Python-Client-2.8.1/Appium_Python_Client.egg-info/dependency_links.txt
--rw-r--r--   0 kazuaki    (501) staff       (20)       14 2023-01-21 04:10:48.000000 Appium-Python-Client-2.8.1/Appium_Python_Client.egg-info/requires.txt
--rw-r--r--   0 kazuaki    (501) staff       (20)        7 2023-01-21 04:10:48.000000 Appium-Python-Client-2.8.1/Appium_Python_Client.egg-info/top_level.txt
--rw-r--r--   0 kazuaki    (501) staff       (20)    11384 2020-05-09 02:13:31.000000 Appium-Python-Client-2.8.1/LICENSE
--rw-r--r--   0 kazuaki    (501) staff       (20)       41 2017-06-08 13:16:26.000000 Appium-Python-Client-2.8.1/MANIFEST.in
--rw-r--r--   0 kazuaki    (501) staff       (20)    10891 2023-01-21 04:10:49.261289 Appium-Python-Client-2.8.1/PKG-INFO
--rw-r--r--   0 kazuaki    (501) staff       (20)     9795 2022-06-28 18:07:38.000000 Appium-Python-Client-2.8.1/README.md
-drwxr-xr-x   0 kazuaki    (501) staff       (20)        0 2023-01-21 04:10:48.834795 Appium-Python-Client-2.8.1/appium/
--rw-r--r--   0 kazuaki    (501) staff       (20)      597 2020-05-16 16:30:37.000000 Appium-Python-Client-2.8.1/appium/__init__.py
-drwxr-xr-x   0 kazuaki    (501) staff       (20)        0 2023-01-21 04:10:48.836035 Appium-Python-Client-2.8.1/appium/common/
--rw-r--r--   0 kazuaki    (501) staff       (20)      613 2019-01-11 07:10:41.000000 Appium-Python-Client-2.8.1/appium/common/__init__.py
--rw-r--r--   0 kazuaki    (501) staff       (20)      924 2022-02-26 05:26:28.000000 Appium-Python-Client-2.8.1/appium/common/exceptions.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1177 2022-02-26 05:26:28.000000 Appium-Python-Client-2.8.1/appium/common/helper.py
--rw-r--r--   0 kazuaki    (501) staff       (20)      863 2020-05-03 09:17:34.000000 Appium-Python-Client-2.8.1/appium/common/logger.py
-drwxr-xr-x   0 kazuaki    (501) staff       (20)        0 2023-01-21 04:10:48.836328 Appium-Python-Client-2.8.1/appium/options/
--rw-r--r--   0 kazuaki    (501) staff       (20)        0 2022-06-14 05:42:03.000000 Appium-Python-Client-2.8.1/appium/options/__init__.py
-drwxr-xr-x   0 kazuaki    (501) staff       (20)        0 2023-01-21 04:10:48.837551 Appium-Python-Client-2.8.1/appium/options/android/
--rw-r--r--   0 kazuaki    (501) staff       (20)       94 2022-06-14 05:42:03.000000 Appium-Python-Client-2.8.1/appium/options/android/__init__.py
-drwxr-xr-x   0 kazuaki    (501) staff       (20)        0 2023-01-21 04:10:48.837958 Appium-Python-Client-2.8.1/appium/options/android/common/
--rw-r--r--   0 kazuaki    (501) staff       (20)        0 2022-06-28 18:07:38.000000 Appium-Python-Client-2.8.1/appium/options/android/common/__init__.py
-drwxr-xr-x   0 kazuaki    (501) staff       (20)        0 2023-01-21 04:10:48.844322 Appium-Python-Client-2.8.1/appium/options/android/common/adb/
--rw-r--r--   0 kazuaki    (501) staff       (20)        0 2022-06-28 18:07:38.000000 Appium-Python-Client-2.8.1/appium/options/android/common/adb/__init__.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1673 2022-09-22 08:22:12.000000 Appium-Python-Client-2.8.1/appium/options/android/common/adb/adb_exec_timeout_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1338 2022-06-28 18:07:38.000000 Appium-Python-Client-2.8.1/appium/options/android/common/adb/adb_port_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1513 2022-06-28 18:07:38.000000 Appium-Python-Client-2.8.1/appium/options/android/common/adb/allow_delay_adb_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1676 2022-06-28 18:07:38.000000 Appium-Python-Client-2.8.1/appium/options/android/common/adb/build_tools_version_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1600 2022-06-28 18:07:38.000000 Appium-Python-Client-2.8.1/appium/options/android/common/adb/clear_device_logs_on_start_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1687 2022-06-28 18:07:38.000000 Appium-Python-Client-2.8.1/appium/options/android/common/adb/ignore_hidden_api_policy_error_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1727 2022-06-28 18:07:38.000000 Appium-Python-Client-2.8.1/appium/options/android/common/adb/logcat_filter_specs_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1432 2022-06-28 18:07:38.000000 Appium-Python-Client-2.8.1/appium/options/android/common/adb/logcat_format_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1750 2022-06-28 18:07:38.000000 Appium-Python-Client-2.8.1/appium/options/android/common/adb/mock_location_app_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1446 2022-06-28 18:07:38.000000 Appium-Python-Client-2.8.1/appium/options/android/common/adb/remote_adb_host_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1529 2022-06-28 18:07:38.000000 Appium-Python-Client-2.8.1/appium/options/android/common/adb/skip_logcat_capture_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1554 2022-06-28 18:07:38.000000 Appium-Python-Client-2.8.1/appium/options/android/common/adb/suppress_kill_server_option.py
-drwxr-xr-x   0 kazuaki    (501) staff       (20)        0 2023-01-21 04:10:48.861177 Appium-Python-Client-2.8.1/appium/options/android/common/app/
--rw-r--r--   0 kazuaki    (501) staff       (20)        0 2022-06-28 18:07:38.000000 Appium-Python-Client-2.8.1/appium/options/android/common/app/__init__.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1662 2022-06-28 18:07:38.000000 Appium-Python-Client-2.8.1/appium/options/android/common/app/allow_test_packages_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1766 2022-09-22 08:22:12.000000 Appium-Python-Client-2.8.1/appium/options/android/common/app/android_install_timeout_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1462 2022-06-28 18:07:38.000000 Appium-Python-Client-2.8.1/appium/options/android/common/app/app_activity_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1455 2022-06-28 18:07:38.000000 Appium-Python-Client-2.8.1/appium/options/android/common/app/app_package_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1504 2022-06-28 18:07:38.000000 Appium-Python-Client-2.8.1/appium/options/android/common/app/app_wait_activity_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1735 2022-09-22 08:22:12.000000 Appium-Python-Client-2.8.1/appium/options/android/common/app/app_wait_duration_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1695 2022-06-28 18:07:38.000000 Appium-Python-Client-2.8.1/appium/options/android/common/app/app_wait_for_launch_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1499 2022-06-28 18:07:38.000000 Appium-Python-Client-2.8.1/appium/options/android/common/app/app_wait_package_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1574 2022-06-28 18:07:38.000000 Appium-Python-Client-2.8.1/appium/options/android/common/app/auto_grant_premissions_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1629 2022-06-28 18:07:38.000000 Appium-Python-Client-2.8.1/appium/options/android/common/app/enforce_app_install_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1478 2022-06-28 18:07:38.000000 Appium-Python-Client-2.8.1/appium/options/android/common/app/intent_action_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1498 2022-06-28 18:07:38.000000 Appium-Python-Client-2.8.1/appium/options/android/common/app/intent_category_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1465 2022-06-28 18:07:38.000000 Appium-Python-Client-2.8.1/appium/options/android/common/app/intent_flags_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1575 2022-06-28 18:07:38.000000 Appium-Python-Client-2.8.1/appium/options/android/common/app/optional_intent_arguments_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1797 2022-06-28 18:07:38.000000 Appium-Python-Client-2.8.1/appium/options/android/common/app/remote_apps_cache_limit_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1568 2022-06-28 18:07:38.000000 Appium-Python-Client-2.8.1/appium/options/android/common/app/uninstall_other_packages_option.py
-drwxr-xr-x   0 kazuaki    (501) staff       (20)        0 2023-01-21 04:10:48.865975 Appium-Python-Client-2.8.1/appium/options/android/common/avd/
--rw-r--r--   0 kazuaki    (501) staff       (20)        0 2022-06-28 18:07:38.000000 Appium-Python-Client-2.8.1/appium/options/android/common/avd/__init__.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1306 2022-06-28 18:07:38.000000 Appium-Python-Client-2.8.1/appium/options/android/common/avd/avd_args_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1350 2022-06-28 18:07:38.000000 Appium-Python-Client-2.8.1/appium/options/android/common/avd/avd_env_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1681 2022-09-22 08:22:12.000000 Appium-Python-Client-2.8.1/appium/options/android/common/avd/avd_launch_timeout_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1503 2022-06-28 18:07:38.000000 Appium-Python-Client-2.8.1/appium/options/android/common/avd/avd_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1728 2022-09-22 08:22:12.000000 Appium-Python-Client-2.8.1/appium/options/android/common/avd/avd_ready_timeout_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1448 2022-06-28 18:07:38.000000 Appium-Python-Client-2.8.1/appium/options/android/common/avd/gps_enabled_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1541 2022-06-28 18:07:38.000000 Appium-Python-Client-2.8.1/appium/options/android/common/avd/network_speed_option.py
-drwxr-xr-x   0 kazuaki    (501) staff       (20)        0 2023-01-21 04:10:48.873759 Appium-Python-Client-2.8.1/appium/options/android/common/context/
--rw-r--r--   0 kazuaki    (501) staff       (20)        0 2022-06-28 18:07:38.000000 Appium-Python-Client-2.8.1/appium/options/android/common/context/__init__.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1737 2022-09-22 08:22:12.000000 Appium-Python-Client-2.8.1/appium/options/android/common/context/auto_webview_timeout_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1634 2022-06-28 18:07:38.000000 Appium-Python-Client-2.8.1/appium/options/android/common/context/chrome_logging_prefs_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1493 2022-06-28 18:07:38.000000 Appium-Python-Client-2.8.1/appium/options/android/common/context/chrome_options_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1641 2022-06-28 18:07:38.000000 Appium-Python-Client-2.8.1/appium/options/android/common/context/chromedriver_args_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1904 2022-06-28 18:07:38.000000 Appium-Python-Client-2.8.1/appium/options/android/common/context/chromedriver_chrome_mapping_file_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1732 2022-06-28 18:07:38.000000 Appium-Python-Client-2.8.1/appium/options/android/common/context/chromedriver_disable_build_check_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1881 2022-09-27 08:12:17.000000 Appium-Python-Client-2.8.1/appium/options/android/common/context/chromedriver_executable_dir_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1487 2022-06-28 18:07:38.000000 Appium-Python-Client-2.8.1/appium/options/android/common/context/chromedriver_executable_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1482 2022-06-28 18:07:38.000000 Appium-Python-Client-2.8.1/appium/options/android/common/context/chromedriver_port_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1546 2022-06-28 18:07:38.000000 Appium-Python-Client-2.8.1/appium/options/android/common/context/chromedriver_ports_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1723 2022-06-28 18:07:38.000000 Appium-Python-Client-2.8.1/appium/options/android/common/context/chromedriver_use_system_executable_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1673 2022-06-28 18:07:38.000000 Appium-Python-Client-2.8.1/appium/options/android/common/context/ensure_webviews_have_pages_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1826 2022-06-28 18:07:38.000000 Appium-Python-Client-2.8.1/appium/options/android/common/context/extract_chrome_android_package_from_context_name_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1614 2022-06-28 18:07:38.000000 Appium-Python-Client-2.8.1/appium/options/android/common/context/native_web_screenshot_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1735 2022-06-28 18:07:38.000000 Appium-Python-Client-2.8.1/appium/options/android/common/context/recreate_chrome_driver_sessions_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1535 2022-06-28 18:07:38.000000 Appium-Python-Client-2.8.1/appium/options/android/common/context/show_chromedriver_log_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1602 2022-06-28 18:07:38.000000 Appium-Python-Client-2.8.1/appium/options/android/common/context/webview_devtools_port_option.py
-drwxr-xr-x   0 kazuaki    (501) staff       (20)        0 2023-01-21 04:10:48.874707 Appium-Python-Client-2.8.1/appium/options/android/common/localization/
--rw-r--r--   0 kazuaki    (501) staff       (20)        0 2022-06-28 18:07:38.000000 Appium-Python-Client-2.8.1/appium/options/android/common/localization/__init__.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1530 2022-06-28 18:07:38.000000 Appium-Python-Client-2.8.1/appium/options/android/common/localization/locale_script_option.py
-drwxr-xr-x   0 kazuaki    (501) staff       (20)        0 2023-01-21 04:10:48.880336 Appium-Python-Client-2.8.1/appium/options/android/common/locking/
--rw-r--r--   0 kazuaki    (501) staff       (20)        0 2022-06-28 18:07:38.000000 Appium-Python-Client-2.8.1/appium/options/android/common/locking/__init__.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1710 2022-06-28 18:07:38.000000 Appium-Python-Client-2.8.1/appium/options/android/common/locking/skip_unlock_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1426 2022-06-28 18:07:38.000000 Appium-Python-Client-2.8.1/appium/options/android/common/locking/unlock_key_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1512 2022-06-28 18:07:38.000000 Appium-Python-Client-2.8.1/appium/options/android/common/locking/unlock_strategy_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1702 2022-09-22 08:22:12.000000 Appium-Python-Client-2.8.1/appium/options/android/common/locking/unlock_success_timeout_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1475 2022-06-28 18:07:38.000000 Appium-Python-Client-2.8.1/appium/options/android/common/locking/unlock_type_option.py
-drwxr-xr-x   0 kazuaki    (501) staff       (20)        0 2023-01-21 04:10:48.880993 Appium-Python-Client-2.8.1/appium/options/android/common/mjpeg/
--rw-r--r--   0 kazuaki    (501) staff       (20)        0 2022-06-28 18:07:38.000000 Appium-Python-Client-2.8.1/appium/options/android/common/mjpeg/__init__.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1647 2022-06-28 18:07:38.000000 Appium-Python-Client-2.8.1/appium/options/android/common/mjpeg/mjpeg_screenshot_url_option.py
-drwxr-xr-x   0 kazuaki    (501) staff       (20)        0 2023-01-21 04:10:48.881885 Appium-Python-Client-2.8.1/appium/options/android/common/other/
--rw-r--r--   0 kazuaki    (501) staff       (20)        0 2022-06-28 18:07:38.000000 Appium-Python-Client-2.8.1/appium/options/android/common/other/__init__.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1736 2022-06-28 18:07:38.000000 Appium-Python-Client-2.8.1/appium/options/android/common/other/disable_suppress_accessibility_service_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1628 2022-06-28 18:07:38.000000 Appium-Python-Client-2.8.1/appium/options/android/common/other/user_profile_option.py
-drwxr-xr-x   0 kazuaki    (501) staff       (20)        0 2023-01-21 04:10:48.889076 Appium-Python-Client-2.8.1/appium/options/android/common/signing/
--rw-r--r--   0 kazuaki    (501) staff       (20)        0 2022-06-28 18:07:38.000000 Appium-Python-Client-2.8.1/appium/options/android/common/signing/__init__.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1495 2022-06-28 18:07:38.000000 Appium-Python-Client-2.8.1/appium/options/android/common/signing/key_alias_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1525 2022-06-28 18:07:38.000000 Appium-Python-Client-2.8.1/appium/options/android/common/signing/key_password_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1550 2022-06-28 18:07:38.000000 Appium-Python-Client-2.8.1/appium/options/android/common/signing/keystore_password_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1511 2022-06-28 18:07:38.000000 Appium-Python-Client-2.8.1/appium/options/android/common/signing/keystore_path_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1647 2022-06-28 18:07:38.000000 Appium-Python-Client-2.8.1/appium/options/android/common/signing/no_sign_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1637 2022-06-28 18:07:38.000000 Appium-Python-Client-2.8.1/appium/options/android/common/signing/use_keystore_option.py
-drwxr-xr-x   0 kazuaki    (501) staff       (20)        0 2023-01-21 04:10:48.897170 Appium-Python-Client-2.8.1/appium/options/android/espresso/
--rw-r--r--   0 kazuaki    (501) staff       (20)        0 2022-06-14 05:42:03.000000 Appium-Python-Client-2.8.1/appium/options/android/espresso/__init__.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1525 2022-06-28 18:07:38.000000 Appium-Python-Client-2.8.1/appium/options/android/espresso/activity_options_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1815 2022-06-28 18:07:38.000000 Appium-Python-Client-2.8.1/appium/options/android/espresso/app_locale_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)    11526 2022-06-28 18:07:38.000000 Appium-Python-Client-2.8.1/appium/options/android/espresso/base.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1878 2022-06-28 18:07:38.000000 Appium-Python-Client-2.8.1/appium/options/android/espresso/espresso_build_config_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1813 2022-09-22 08:22:12.000000 Appium-Python-Client-2.8.1/appium/options/android/espresso/espresso_server_launch_timeout_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1660 2022-06-28 18:07:38.000000 Appium-Python-Client-2.8.1/appium/options/android/espresso/force_espresso_rebuild_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1543 2022-06-28 18:07:38.000000 Appium-Python-Client-2.8.1/appium/options/android/espresso/intent_options_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1464 2022-06-28 18:07:38.000000 Appium-Python-Client-2.8.1/appium/options/android/espresso/show_gradle_log_option.py
-drwxr-xr-x   0 kazuaki    (501) staff       (20)        0 2023-01-21 04:10:48.914393 Appium-Python-Client-2.8.1/appium/options/android/uiautomator2/
--rw-r--r--   0 kazuaki    (501) staff       (20)        0 2022-06-14 05:42:03.000000 Appium-Python-Client-2.8.1/appium/options/android/uiautomator2/__init__.py
--rw-r--r--   0 kazuaki    (501) staff       (20)    11716 2022-06-28 18:07:38.000000 Appium-Python-Client-2.8.1/appium/options/android/uiautomator2/base.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1566 2022-06-28 18:07:38.000000 Appium-Python-Client-2.8.1/appium/options/android/uiautomator2/disable_window_animation_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1628 2022-06-28 18:07:38.000000 Appium-Python-Client-2.8.1/appium/options/android/uiautomator2/mjpeg_server_port_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1687 2022-06-28 18:07:38.000000 Appium-Python-Client-2.8.1/appium/options/android/uiautomator2/skip_device_initialization_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1871 2022-06-28 18:07:38.000000 Appium-Python-Client-2.8.1/appium/options/android/uiautomator2/skip_server_installation_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1880 2022-09-22 08:22:12.000000 Appium-Python-Client-2.8.1/appium/options/android/uiautomator2/uiautomator2_server_install_timeout_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1871 2022-09-22 08:22:12.000000 Appium-Python-Client-2.8.1/appium/options/android/uiautomator2/uiautomator2_server_launch_timeout_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     2003 2022-09-22 08:22:12.000000 Appium-Python-Client-2.8.1/appium/options/android/uiautomator2/uiautomator2_server_read_timeout_option.py
-drwxr-xr-x   0 kazuaki    (501) staff       (20)        0 2023-01-21 04:10:49.022070 Appium-Python-Client-2.8.1/appium/options/common/
--rw-r--r--   0 kazuaki    (501) staff       (20)       32 2022-06-14 05:42:03.000000 Appium-Python-Client-2.8.1/appium/options/common/__init__.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1395 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/common/app_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1484 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/common/auto_web_view_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1393 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/common/automation_name_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     4125 2022-06-28 18:07:38.000000 Appium-Python-Client-2.8.1/appium/options/common/base.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1356 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/common/bundle_id_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1447 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/common/clear_system_files_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1314 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/common/device_name_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1463 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/common/enable_performance_logging_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1445 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/common/event_timings_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1333 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/common/full_reset_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1464 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/common/is_headless_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1317 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/common/language_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1297 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/common/locale_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1698 2022-09-22 08:22:12.000000 Appium-Python-Client-2.8.1/appium/options/common/new_command_timeout_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1315 2022-08-11 05:26:58.000000 Appium-Python-Client-2.8.1/appium/options/common/no_reset_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1441 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/common/orientation_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1397 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/common/other_apps_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1375 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/common/postrun_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1425 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/common/prerun_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1599 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/common/print_page_source_on_find_failure_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1383 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/common/skip_log_capture_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1063 2022-06-14 05:42:03.000000 Appium-Python-Client-2.8.1/appium/options/common/supports_capabilities.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1382 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/common/system_host_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1386 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/common/system_port_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1285 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/common/udid_option.py
-drwxr-xr-x   0 kazuaki    (501) staff       (20)        0 2023-01-21 04:10:49.025151 Appium-Python-Client-2.8.1/appium/options/gecko/
--rw-r--r--   0 kazuaki    (501) staff       (20)       31 2022-06-14 05:42:03.000000 Appium-Python-Client-2.8.1/appium/options/gecko/__init__.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1458 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/gecko/android_storage_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1893 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/gecko/base.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1441 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/gecko/firefox_options_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1757 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/gecko/marionette_port_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1409 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/gecko/verbosity_option.py
-drwxr-xr-x   0 kazuaki    (501) staff       (20)        0 2023-01-21 04:10:49.025576 Appium-Python-Client-2.8.1/appium/options/ios/
--rw-r--r--   0 kazuaki    (501) staff       (20)       82 2022-06-14 05:42:03.000000 Appium-Python-Client-2.8.1/appium/options/ios/__init__.py
-drwxr-xr-x   0 kazuaki    (501) staff       (20)        0 2023-01-21 04:10:49.032545 Appium-Python-Client-2.8.1/appium/options/ios/safari/
--rw-r--r--   0 kazuaki    (501) staff       (20)        0 2022-06-14 05:42:03.000000 Appium-Python-Client-2.8.1/appium/options/ios/safari/__init__.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1699 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/ios/safari/automatic_inspection_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1624 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/ios/safari/automatic_profiling_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1906 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/ios/safari/base.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1778 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/ios/safari/device_name_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1652 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/ios/safari/device_type_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1715 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/ios/safari/device_udid_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1680 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/ios/safari/platform_build_version_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1665 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/ios/safari/platform_version_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1621 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/ios/safari/use_simulator_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     2325 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/ios/safari/webkit_webrtc_option.py
-drwxr-xr-x   0 kazuaki    (501) staff       (20)        0 2023-01-21 04:10:49.033577 Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/
--rw-r--r--   0 kazuaki    (501) staff       (20)        0 2022-06-14 05:42:03.000000 Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/__init__.py
-drwxr-xr-x   0 kazuaki    (501) staff       (20)        0 2023-01-21 04:10:49.037150 Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/app/
--rw-r--r--   0 kazuaki    (501) staff       (20)        0 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/app/__init__.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1985 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/app/app_install_strategy_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1677 2022-09-22 08:22:12.000000 Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/app/app_push_timeout_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1512 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/app/localizable_strings_dir_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)    11038 2022-08-11 05:26:58.000000 Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/base.py
-drwxr-xr-x   0 kazuaki    (501) staff       (20)        0 2023-01-21 04:10:49.038134 Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/general/
--rw-r--r--   0 kazuaki    (501) staff       (20)        0 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/general/__init__.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1783 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/general/include_device_caps_to_session_info_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1530 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/general/reset_location_service_option.py
-drwxr-xr-x   0 kazuaki    (501) staff       (20)        0 2023-01-21 04:10:49.042153 Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/other/
--rw-r--r--   0 kazuaki    (501) staff       (20)        0 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/other/__init__.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     2627 2022-09-22 08:22:12.000000 Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/other/command_timeouts_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1710 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/other/launch_with_idb_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1427 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/other/show_ios_log_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1479 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/other/use_json_source_option.py
-drwxr-xr-x   0 kazuaki    (501) staff       (20)        0 2023-01-21 04:10:49.054874 Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/simulator/
--rw-r--r--   0 kazuaki    (501) staff       (20)        0 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/simulator/__init__.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1703 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/simulator/calendar_access_authorized_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1374 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/simulator/calendar_format_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1890 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/simulator/connect_hardware_keyboard_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1425 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/simulator/custom_ssl_cert_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1594 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/simulator/enforce_fresh_simulator_creation_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     2127 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/simulator/force_simulator_software_keyboard_presence_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1485 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/simulator/ios_simulator_logs_predicate_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1514 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/simulator/keep_key_chains_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1858 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/simulator/keychains_exclude_patterns_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     2158 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/simulator/permissions_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1491 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/simulator/reduce_motion_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1731 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/simulator/reset_on_session_start_only_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1797 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/simulator/scale_factor_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1951 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/simulator/shutdown_other_simulators_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1695 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/simulator/simulator_devices_set_path_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1866 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/simulator/simulator_pasteboard_automatic_sync_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1919 2022-09-22 08:22:12.000000 Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/simulator/simulator_startup_timeout_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1644 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/simulator/simulator_trace_pointer_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1683 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/simulator/simulator_window_center_option.py
-drwxr-xr-x   0 kazuaki    (501) staff       (20)        0 2023-01-21 04:10:49.078957 Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/wda/
--rw-r--r--   0 kazuaki    (501) staff       (20)        0 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/wda/__init__.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1774 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/wda/allow_provisioning_device_regitration_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1521 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/wda/auto_accept_alerts_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1531 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/wda/auto_disimiss_alerts_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1648 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/wda/derived_data_path_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1623 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/wda/disable_automatic_screenshots_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1711 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/wda/force_app_launch_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1433 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/wda/keychain_password_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1382 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/wda/keychain_path_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1556 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/wda/max_typing_frequency_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1692 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/wda/mjpeg_server_port_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1870 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/wda/process_arguments_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1702 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/wda/result_bundle_path_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1641 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/wda/screenshot_quality_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1705 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/wda/should_terminate_app_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1662 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/wda/should_use_singleton_test_manager_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1547 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/wda/show_xcode_log_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1817 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/wda/simple_is_visible_check_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1510 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/wda/updated_wda_bundle_id_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1715 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/wda/use_native_caching_strategy_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     2403 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/wda/use_new_wda_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1503 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/wda/use_prebuilt_wda_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1635 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/wda/use_simple_build_test_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     2497 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/wda/use_xctestrun_file_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     2074 2022-09-22 08:22:12.000000 Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/wda/wait_for_idle_timeout_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1726 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/wda/wait_for_quiescence_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1608 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/wda/wda_base_url_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1728 2022-09-22 08:22:12.000000 Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/wda/wda_connection_timeout_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     2124 2022-09-22 08:22:12.000000 Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/wda/wda_eventloop_idle_delay_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1702 2022-09-22 08:22:12.000000 Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/wda/wda_launch_timeout_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1558 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/wda/wda_local_port_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1469 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/wda/wda_startup_retries_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1772 2022-09-22 08:22:12.000000 Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/wda/wda_startup_retry_interval_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1471 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/wda/web_driver_agent_url_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1490 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/wda/xcode_org_id_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1490 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/wda/xcode_signing_id_option.py
-drwxr-xr-x   0 kazuaki    (501) staff       (20)        0 2023-01-21 04:10:49.098114 Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/webview/
--rw-r--r--   0 kazuaki    (501) staff       (20)        0 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/webview/__init__.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1759 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/webview/absolute_web_locations_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1668 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/webview/additional_webview_bundle_ids_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1609 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/webview/enable_async_execute_from_https_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1698 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/webview/full_context_list_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1695 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/webview/include_safari_in_webviews_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1582 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/webview/native_web_tap_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1563 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/webview/safari_garbage_collect_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1557 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/webview/safari_ignore_fraud_warning_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1791 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/webview/safari_ignore_web_hostnames_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1395 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/webview/safari_initial_url_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1956 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/webview/safari_log_all_communication_hex_dump_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1674 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/webview/safari_log_all_communication_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1575 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/webview/safari_open_links_in_background_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1718 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/webview/safari_socket_chunk_size_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1788 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/webview/safari_web_inspector_max_frame_length_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1759 2022-09-22 08:22:12.000000 Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/webview/webkit_response_timeout_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1546 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/webview/webview_connect_retries_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1747 2022-09-22 08:22:12.000000 Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/webview/webview_connect_timeout_option.py
-drwxr-xr-x   0 kazuaki    (501) staff       (20)        0 2023-01-21 04:10:49.098511 Appium-Python-Client-2.8.1/appium/options/mac/
--rw-r--r--   0 kazuaki    (501) staff       (20)       35 2022-06-14 05:42:03.000000 Appium-Python-Client-2.8.1/appium/options/mac/__init__.py
-drwxr-xr-x   0 kazuaki    (501) staff       (20)        0 2023-01-21 04:10:49.102540 Appium-Python-Client-2.8.1/appium/options/mac/mac2/
--rw-r--r--   0 kazuaki    (501) staff       (20)        0 2022-06-14 05:42:03.000000 Appium-Python-Client-2.8.1/appium/options/mac/mac2/__init__.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1468 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/mac/mac2/arguments_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     4759 2022-08-11 07:46:16.000000 Appium-Python-Client-2.8.1/appium/options/mac/mac2/base.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1612 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/mac/mac2/bootstrap_root_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1637 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/mac/mac2/environment_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1761 2022-09-22 08:22:12.000000 Appium-Python-Client-2.8.1/appium/options/mac/mac2/server_startup_timeout_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1456 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/mac/mac2/show_server_logs_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1535 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/mac/mac2/skip_app_kill_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1557 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/mac/mac2/web_driver_agent_mac_url_option.py
-drwxr-xr-x   0 kazuaki    (501) staff       (20)        0 2023-01-21 04:10:49.103911 Appium-Python-Client-2.8.1/appium/options/windows/
--rw-r--r--   0 kazuaki    (501) staff       (20)       41 2022-06-14 05:42:03.000000 Appium-Python-Client-2.8.1/appium/options/windows/__init__.py
-drwxr-xr-x   0 kazuaki    (501) staff       (20)        0 2023-01-21 04:10:49.112148 Appium-Python-Client-2.8.1/appium/options/windows/windows/
--rw-r--r--   0 kazuaki    (501) staff       (20)        0 2022-06-14 05:42:03.000000 Appium-Python-Client-2.8.1/appium/options/windows/windows/__init__.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1506 2022-09-22 08:22:12.000000 Appium-Python-Client-2.8.1/appium/options/windows/windows/app_arguments_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1625 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/windows/windows/app_top_level_window_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1558 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/windows/windows/app_working_dir_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     4189 2022-09-22 08:22:12.000000 Appium-Python-Client-2.8.1/appium/options/windows/windows/base.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1928 2022-09-22 08:22:12.000000 Appium-Python-Client-2.8.1/appium/options/windows/windows/create_session_timeout_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1550 2022-06-26 05:30:16.000000 Appium-Python-Client-2.8.1/appium/options/windows/windows/expreimental_web_driver_option.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1846 2022-09-22 08:22:12.000000 Appium-Python-Client-2.8.1/appium/options/windows/windows/wait_for_app_launch_option.py
-drwxr-xr-x   0 kazuaki    (501) staff       (20)        0 2023-01-21 04:10:49.113165 Appium-Python-Client-2.8.1/appium/protocols/
--rw-r--r--   0 kazuaki    (501) staff       (20)      567 2022-02-26 05:26:28.000000 Appium-Python-Client-2.8.1/appium/protocols/__init__.py
--rw-r--r--   0 kazuaki    (501) staff       (20)      776 2022-02-26 05:26:28.000000 Appium-Python-Client-2.8.1/appium/protocols/protocol.py
-drwxr-xr-x   0 kazuaki    (501) staff       (20)        0 2023-01-21 04:10:49.114930 Appium-Python-Client-2.8.1/appium/protocols/webdriver/
--rw-r--r--   0 kazuaki    (501) staff       (20)      567 2022-02-26 05:26:28.000000 Appium-Python-Client-2.8.1/appium/protocols/webdriver/__init__.py
--rw-r--r--   0 kazuaki    (501) staff       (20)      882 2022-12-05 07:06:32.000000 Appium-Python-Client-2.8.1/appium/protocols/webdriver/can_execute_commands.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1044 2022-02-26 05:26:28.000000 Appium-Python-Client-2.8.1/appium/protocols/webdriver/can_execute_scripts.py
--rw-r--r--   0 kazuaki    (501) staff       (20)      976 2022-12-05 07:06:32.000000 Appium-Python-Client-2.8.1/appium/protocols/webdriver/can_find_elements.py
--rw-r--r--   0 kazuaki    (501) staff       (20)        0 2022-08-11 05:26:58.000000 Appium-Python-Client-2.8.1/appium/py.typed
--rw-r--r--   0 kazuaki    (501) staff       (20)       18 2023-01-21 04:10:38.000000 Appium-Python-Client-2.8.1/appium/version.py
-drwxr-xr-x   0 kazuaki    (501) staff       (20)        0 2023-01-21 04:10:49.122838 Appium-Python-Client-2.8.1/appium/webdriver/
--rw-r--r--   0 kazuaki    (501) staff       (20)      694 2019-01-11 07:10:41.000000 Appium-Python-Client-2.8.1/appium/webdriver/__init__.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     2321 2022-02-26 05:26:28.000000 Appium-Python-Client-2.8.1/appium/webdriver/appium_connection.py
--rw-r--r--   0 kazuaki    (501) staff       (20)    11038 2022-10-11 05:37:13.000000 Appium-Python-Client-2.8.1/appium/webdriver/appium_service.py
--rw-r--r--   0 kazuaki    (501) staff       (20)      735 2020-05-03 09:17:34.000000 Appium-Python-Client-2.8.1/appium/webdriver/applicationstate.py
--rw-r--r--   0 kazuaki    (501) staff       (20)      661 2020-05-03 09:17:34.000000 Appium-Python-Client-2.8.1/appium/webdriver/clipboard_content_type.py
--rw-r--r--   0 kazuaki    (501) staff       (20)      792 2021-11-25 19:12:21.000000 Appium-Python-Client-2.8.1/appium/webdriver/command_method.py
-drwxr-xr-x   0 kazuaki    (501) staff       (20)        0 2023-01-21 04:10:49.129071 Appium-Python-Client-2.8.1/appium/webdriver/common/
--rw-r--r--   0 kazuaki    (501) staff       (20)      623 2019-01-11 07:10:41.000000 Appium-Python-Client-2.8.1/appium/webdriver/common/__init__.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1107 2021-12-23 22:07:15.000000 Appium-Python-Client-2.8.1/appium/webdriver/common/appiumby.py
--rw-r--r--   0 kazuaki    (501) staff       (20)      787 2022-02-26 05:26:28.000000 Appium-Python-Client-2.8.1/appium/webdriver/common/mobileby.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     3468 2022-06-28 18:07:38.000000 Appium-Python-Client-2.8.1/appium/webdriver/common/multi_action.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     6821 2022-12-05 07:06:32.000000 Appium-Python-Client-2.8.1/appium/webdriver/common/touch_action.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1567 2020-05-03 09:17:34.000000 Appium-Python-Client-2.8.1/appium/webdriver/connectiontype.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1137 2022-02-26 05:26:28.000000 Appium-Python-Client-2.8.1/appium/webdriver/errorhandler.py
-drwxr-xr-x   0 kazuaki    (501) staff       (20)        0 2023-01-21 04:10:49.152743 Appium-Python-Client-2.8.1/appium/webdriver/extensions/
--rw-r--r--   0 kazuaki    (501) staff       (20)      567 2019-01-11 07:10:41.000000 Appium-Python-Client-2.8.1/appium/webdriver/extensions/__init__.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     7672 2022-08-11 05:26:58.000000 Appium-Python-Client-2.8.1/appium/webdriver/extensions/action_helpers.py
-drwxr-xr-x   0 kazuaki    (501) staff       (20)        0 2023-01-21 04:10:49.163272 Appium-Python-Client-2.8.1/appium/webdriver/extensions/android/
--rw-r--r--   0 kazuaki    (501) staff       (20)        0 2019-05-12 06:29:12.000000 Appium-Python-Client-2.8.1/appium/webdriver/extensions/android/__init__.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     3920 2022-06-28 18:07:38.000000 Appium-Python-Client-2.8.1/appium/webdriver/extensions/android/activities.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     2537 2022-09-27 08:12:17.000000 Appium-Python-Client-2.8.1/appium/webdriver/extensions/android/common.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1411 2022-02-26 05:26:28.000000 Appium-Python-Client-2.8.1/appium/webdriver/extensions/android/display.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     4410 2022-06-28 18:07:38.000000 Appium-Python-Client-2.8.1/appium/webdriver/extensions/android/gsm.py
--rw-r--r--   0 kazuaki    (501) staff       (20)    30132 2021-10-31 06:04:06.000000 Appium-Python-Client-2.8.1/appium/webdriver/extensions/android/nativekey.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     4920 2022-06-28 18:07:38.000000 Appium-Python-Client-2.8.1/appium/webdriver/extensions/android/network.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     2769 2022-12-05 07:06:32.000000 Appium-Python-Client-2.8.1/appium/webdriver/extensions/android/performance.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     2256 2022-06-28 18:07:38.000000 Appium-Python-Client-2.8.1/appium/webdriver/extensions/android/power.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1600 2022-06-28 18:07:38.000000 Appium-Python-Client-2.8.1/appium/webdriver/extensions/android/sms.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1711 2022-02-26 05:26:28.000000 Appium-Python-Client-2.8.1/appium/webdriver/extensions/android/system_bars.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     8889 2022-12-05 07:06:32.000000 Appium-Python-Client-2.8.1/appium/webdriver/extensions/applications.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     3471 2022-06-28 18:07:38.000000 Appium-Python-Client-2.8.1/appium/webdriver/extensions/clipboard.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     2067 2022-02-26 05:26:28.000000 Appium-Python-Client-2.8.1/appium/webdriver/extensions/context.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     2212 2022-02-26 05:26:28.000000 Appium-Python-Client-2.8.1/appium/webdriver/extensions/device_time.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     2710 2022-02-26 05:26:28.000000 Appium-Python-Client-2.8.1/appium/webdriver/extensions/execute_driver.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     2380 2022-06-28 18:07:38.000000 Appium-Python-Client-2.8.1/appium/webdriver/extensions/execute_mobile_command.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     4182 2022-06-28 18:07:38.000000 Appium-Python-Client-2.8.1/appium/webdriver/extensions/hw_actions.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     7151 2022-02-26 05:26:28.000000 Appium-Python-Client-2.8.1/appium/webdriver/extensions/images_comparison.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     3580 2022-06-28 18:07:38.000000 Appium-Python-Client-2.8.1/appium/webdriver/extensions/ime.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     5130 2022-06-28 18:07:38.000000 Appium-Python-Client-2.8.1/appium/webdriver/extensions/keyboard.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     3338 2022-06-28 18:07:38.000000 Appium-Python-Client-2.8.1/appium/webdriver/extensions/location.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     2560 2022-12-05 07:06:32.000000 Appium-Python-Client-2.8.1/appium/webdriver/extensions/log_event.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     3548 2022-06-28 18:07:38.000000 Appium-Python-Client-2.8.1/appium/webdriver/extensions/remote_fs.py
--rw-r--r--   0 kazuaki    (501) staff       (20)    13010 2022-02-26 05:26:28.000000 Appium-Python-Client-2.8.1/appium/webdriver/extensions/screen_record.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     2275 2022-02-26 05:26:28.000000 Appium-Python-Client-2.8.1/appium/webdriver/extensions/session.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     2052 2022-09-27 08:12:17.000000 Appium-Python-Client-2.8.1/appium/webdriver/extensions/settings.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     3954 2023-01-21 04:09:09.000000 Appium-Python-Client-2.8.1/appium/webdriver/mobilecommand.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     1414 2022-06-28 18:07:38.000000 Appium-Python-Client-2.8.1/appium/webdriver/switch_to.py
--rw-r--r--   0 kazuaki    (501) staff       (20)    20948 2023-01-21 04:09:09.000000 Appium-Python-Client-2.8.1/appium/webdriver/webdriver.py
--rw-r--r--   0 kazuaki    (501) staff       (20)     7240 2022-12-05 07:06:32.000000 Appium-Python-Client-2.8.1/appium/webdriver/webelement.py
-drwxr-xr-x   0 kazuaki    (501) staff       (20)        0 2023-01-21 04:10:49.173262 Appium-Python-Client-2.8.1/docs/
--rw-r--r--   0 kazuaki    (501) staff       (20)     6148 2021-11-27 08:36:52.000000 Appium-Python-Client-2.8.1/docs/.DS_Store
--rw-r--r--   0 kazuaki    (501) staff       (20)      634 2020-05-03 09:17:34.000000 Appium-Python-Client-2.8.1/docs/Makefile
--rw-r--r--   0 kazuaki    (501) staff       (20)      323 2021-11-25 18:30:52.000000 Appium-Python-Client-2.8.1/docs/README.md
-drwxr-xr-x   0 kazuaki    (501) staff       (20)        0 2023-01-21 04:10:48.828654 Appium-Python-Client-2.8.1/docs/_build/
-drwxr-xr-x   0 kazuaki    (501) staff       (20)        0 2023-01-21 04:10:49.198133 Appium-Python-Client-2.8.1/docs/_build/doctrees/
--rw-r--r--   0 kazuaki    (501) staff       (20)    22030 2021-11-25 19:55:43.000000 Appium-Python-Client-2.8.1/docs/_build/doctrees/appium.common.doctree
--rw-r--r--   0 kazuaki    (501) staff       (20)     4702 2021-11-25 19:55:43.000000 Appium-Python-Client-2.8.1/docs/_build/doctrees/appium.doctree
--rw-r--r--   0 kazuaki    (501) staff       (20)   100294 2021-11-25 19:55:44.000000 Appium-Python-Client-2.8.1/docs/_build/doctrees/appium.webdriver.common.doctree
--rw-r--r--   0 kazuaki    (501) staff       (20)   377633 2021-11-25 19:55:44.000000 Appium-Python-Client-2.8.1/docs/_build/doctrees/appium.webdriver.doctree
--rw-r--r--   0 kazuaki    (501) staff       (20)   685784 2021-11-25 19:55:46.000000 Appium-Python-Client-2.8.1/docs/_build/doctrees/appium.webdriver.extensions.android.doctree
--rw-r--r--   0 kazuaki    (501) staff       (20)   620400 2021-11-25 19:55:45.000000 Appium-Python-Client-2.8.1/docs/_build/doctrees/appium.webdriver.extensions.doctree
--rw-r--r--   0 kazuaki    (501) staff       (20)   191010 2021-11-25 19:55:46.000000 Appium-Python-Client-2.8.1/docs/_build/doctrees/appium.webdriver.extensions.search_context.doctree
--rw-r--r--   0 kazuaki    (501) staff       (20)   209918 2021-11-25 19:55:46.000000 Appium-Python-Client-2.8.1/docs/_build/doctrees/environment.pickle
--rw-r--r--   0 kazuaki    (501) staff       (20)     5039 2021-11-25 19:55:46.000000 Appium-Python-Client-2.8.1/docs/_build/doctrees/index.doctree
-drwxr-xr-x   0 kazuaki    (501) staff       (20)        0 2023-01-21 04:10:49.215531 Appium-Python-Client-2.8.1/docs/_build/html/
--rw-r--r--   0 kazuaki    (501) staff       (20)      230 2021-11-25 19:55:48.000000 Appium-Python-Client-2.8.1/docs/_build/html/.buildinfo
--rw-r--r--   0 kazuaki    (501) staff       (20)        0 2021-11-25 19:55:46.000000 Appium-Python-Client-2.8.1/docs/_build/html/.nojekyll
-drwxr-xr-x   0 kazuaki    (501) staff       (20)        0 2023-01-21 04:10:49.220679 Appium-Python-Client-2.8.1/docs/_build/html/_sources/
--rw-r--r--   0 kazuaki    (501) staff       (20)      644 2021-11-25 19:55:41.000000 Appium-Python-Client-2.8.1/docs/_build/html/_sources/appium.common.rst.txt
--rw-r--r--   0 kazuaki    (501) staff       (20)      388 2021-11-25 19:55:41.000000 Appium-Python-Client-2.8.1/docs/_build/html/_sources/appium.rst.txt
--rw-r--r--   0 kazuaki    (501) staff       (20)      983 2021-11-25 19:55:41.000000 Appium-Python-Client-2.8.1/docs/_build/html/_sources/appium.webdriver.common.rst.txt
--rw-r--r--   0 kazuaki    (501) staff       (20)     2439 2021-11-25 19:55:41.000000 Appium-Python-Client-2.8.1/docs/_build/html/_sources/appium.webdriver.extensions.android.rst.txt
--rw-r--r--   0 kazuaki    (501) staff       (20)     3872 2021-11-25 19:55:41.000000 Appium-Python-Client-2.8.1/docs/_build/html/_sources/appium.webdriver.extensions.rst.txt
--rw-r--r--   0 kazuaki    (501) staff       (20)     1742 2021-11-25 19:55:41.000000 Appium-Python-Client-2.8.1/docs/_build/html/_sources/appium.webdriver.extensions.search_context.rst.txt
--rw-r--r--   0 kazuaki    (501) staff       (20)     2310 2021-11-25 19:55:41.000000 Appium-Python-Client-2.8.1/docs/_build/html/_sources/appium.webdriver.rst.txt
--rw-r--r--   0 kazuaki    (501) staff       (20)      486 2021-11-25 19:55:41.000000 Appium-Python-Client-2.8.1/docs/_build/html/_sources/index.rst.txt
-drwxr-xr-x   0 kazuaki    (501) staff       (20)        0 2023-01-21 04:10:49.231480 Appium-Python-Client-2.8.1/docs/_build/html/_static/
--rw-r--r--   0 kazuaki    (501) staff       (20)    14667 2021-11-25 19:55:48.000000 Appium-Python-Client-2.8.1/docs/_build/html/_static/basic.css
-drwxr-xr-x   0 kazuaki    (501) staff       (20)        0 2023-01-21 04:10:49.232169 Appium-Python-Client-2.8.1/docs/_build/html/_static/css/
--rw-r--r--   0 kazuaki    (501) staff       (20)     3275 2021-11-25 18:31:24.000000 Appium-Python-Client-2.8.1/docs/_build/html/_static/css/badge_only.css
-drwxr-xr-x   0 kazuaki    (501) staff       (20)        0 2023-01-21 04:10:49.254655 Appium-Python-Client-2.8.1/docs/_build/html/_static/css/fonts/
--rw-r--r--   0 kazuaki    (501) staff       (20)    87624 2021-11-25 18:31:24.000000 Appium-Python-Client-2.8.1/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff
--rw-r--r--   0 kazuaki    (501) staff       (20)    67312 2021-11-25 18:31:24.000000 Appium-Python-Client-2.8.1/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff2
--rw-r--r--   0 kazuaki    (501) staff       (20)    86288 2021-11-25 18:31:24.000000 Appium-Python-Client-2.8.1/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff
--rw-r--r--   0 kazuaki    (501) staff       (20)    66444 2021-11-25 18:31:24.000000 Appium-Python-Client-2.8.1/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff2
--rw-r--r--   0 kazuaki    (501) staff       (20)   165742 2021-11-25 18:31:24.000000 Appium-Python-Client-2.8.1/docs/_build/html/_static/css/fonts/fontawesome-webfont.eot
--rw-r--r--   0 kazuaki    (501) staff       (20)   444379 2021-11-25 18:31:24.000000 Appium-Python-Client-2.8.1/docs/_build/html/_static/css/fonts/fontawesome-webfont.svg
--rw-r--r--   0 kazuaki    (501) staff       (20)   165548 2021-11-25 18:31:24.000000 Appium-Python-Client-2.8.1/docs/_build/html/_static/css/fonts/fontawesome-webfont.ttf
--rw-r--r--   0 kazuaki    (501) staff       (20)    98024 2021-11-25 18:31:24.000000 Appium-Python-Client-2.8.1/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff
--rw-r--r--   0 kazuaki    (501) staff       (20)    77160 2021-11-25 18:31:24.000000 Appium-Python-Client-2.8.1/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff2
--rw-r--r--   0 kazuaki    (501) staff       (20)   323344 2021-11-25 18:31:24.000000 Appium-Python-Client-2.8.1/docs/_build/html/_static/css/fonts/lato-bold-italic.woff
--rw-r--r--   0 kazuaki    (501) staff       (20)   193308 2021-11-25 18:31:24.000000 Appium-Python-Client-2.8.1/docs/_build/html/_static/css/fonts/lato-bold-italic.woff2
--rw-r--r--   0 kazuaki    (501) staff       (20)   309728 2021-11-25 18:31:24.000000 Appium-Python-Client-2.8.1/docs/_build/html/_static/css/fonts/lato-bold.woff
--rw-r--r--   0 kazuaki    (501) staff       (20)   184912 2021-11-25 18:31:24.000000 Appium-Python-Client-2.8.1/docs/_build/html/_static/css/fonts/lato-bold.woff2
--rw-r--r--   0 kazuaki    (501) staff       (20)   328412 2021-11-25 18:31:24.000000 Appium-Python-Client-2.8.1/docs/_build/html/_static/css/fonts/lato-normal-italic.woff
--rw-r--r--   0 kazuaki    (501) staff       (20)   195704 2021-11-25 18:31:24.000000 Appium-Python-Client-2.8.1/docs/_build/html/_static/css/fonts/lato-normal-italic.woff2
--rw-r--r--   0 kazuaki    (501) staff       (20)   309192 2021-11-25 18:31:24.000000 Appium-Python-Client-2.8.1/docs/_build/html/_static/css/fonts/lato-normal.woff
--rw-r--r--   0 kazuaki    (501) staff       (20)   182708 2021-11-25 18:31:24.000000 Appium-Python-Client-2.8.1/docs/_build/html/_static/css/fonts/lato-normal.woff2
--rw-r--r--   0 kazuaki    (501) staff       (20)   129674 2021-11-25 18:31:24.000000 Appium-Python-Client-2.8.1/docs/_build/html/_static/css/theme.css
--rw-r--r--   0 kazuaki    (501) staff       (20)     9630 2021-11-25 18:31:24.000000 Appium-Python-Client-2.8.1/docs/_build/html/_static/doctools.js
--rw-r--r--   0 kazuaki    (501) staff       (20)      351 2021-11-25 19:55:48.000000 Appium-Python-Client-2.8.1/docs/_build/html/_static/documentation_options.js
--rw-r--r--   0 kazuaki    (501) staff       (20)      286 2021-11-25 18:31:24.000000 Appium-Python-Client-2.8.1/docs/_build/html/_static/file.png
--rw-r--r--   0 kazuaki    (501) staff       (20)   287630 2021-11-25 18:31:24.000000 Appium-Python-Client-2.8.1/docs/_build/html/_static/jquery-3.5.1.js
--rw-r--r--   0 kazuaki    (501) staff       (20)    89476 2021-11-25 18:31:24.000000 Appium-Python-Client-2.8.1/docs/_build/html/_static/jquery.js
-drwxr-xr-x   0 kazuaki    (501) staff       (20)        0 2023-01-21 04:10:49.260759 Appium-Python-Client-2.8.1/docs/_build/html/_static/js/
--rw-r--r--   0 kazuaki    (501) staff       (20)      934 2021-11-25 18:31:24.000000 Appium-Python-Client-2.8.1/docs/_build/html/_static/js/badge_only.js
--rw-r--r--   0 kazuaki    (501) staff       (20)     4370 2021-11-25 18:31:24.000000 Appium-Python-Client-2.8.1/docs/_build/html/_static/js/html5shiv-printshiv.min.js
--rw-r--r--   0 kazuaki    (501) staff       (20)     2734 2021-11-25 18:31:24.000000 Appium-Python-Client-2.8.1/docs/_build/html/_static/js/html5shiv.min.js
--rw-r--r--   0 kazuaki    (501) staff       (20)     5023 2021-11-25 18:31:24.000000 Appium-Python-Client-2.8.1/docs/_build/html/_static/js/theme.js
--rw-r--r--   0 kazuaki    (501) staff       (20)    10854 2021-11-25 19:55:48.000000 Appium-Python-Client-2.8.1/docs/_build/html/_static/language_data.js
--rw-r--r--   0 kazuaki    (501) staff       (20)       90 2021-11-25 18:31:24.000000 Appium-Python-Client-2.8.1/docs/_build/html/_static/minus.png
--rw-r--r--   0 kazuaki    (501) staff       (20)       90 2021-11-25 18:31:24.000000 Appium-Python-Client-2.8.1/docs/_build/html/_static/plus.png
--rw-r--r--   0 kazuaki    (501) staff       (20)     4819 2021-11-25 19:55:48.000000 Appium-Python-Client-2.8.1/docs/_build/html/_static/pygments.css
--rw-r--r--   0 kazuaki    (501) staff       (20)    16793 2021-11-25 18:31:24.000000 Appium-Python-Client-2.8.1/docs/_build/html/_static/searchtools.js
--rw-r--r--   0 kazuaki    (501) staff       (20)    68420 2021-11-25 18:31:24.000000 Appium-Python-Client-2.8.1/docs/_build/html/_static/underscore-1.13.1.js
--rw-r--r--   0 kazuaki    (501) staff       (20)    19530 2021-11-25 18:31:24.000000 Appium-Python-Client-2.8.1/docs/_build/html/_static/underscore.js
--rw-r--r--   0 kazuaki    (501) staff       (20)    12068 2021-11-25 19:55:46.000000 Appium-Python-Client-2.8.1/docs/_build/html/appium.common.html
--rw-r--r--   0 kazuaki    (501) staff       (20)    13788 2021-11-25 19:55:46.000000 Appium-Python-Client-2.8.1/docs/_build/html/appium.html
--rw-r--r--   0 kazuaki    (501) staff       (20)    38641 2021-11-25 19:55:47.000000 Appium-Python-Client-2.8.1/docs/_build/html/appium.webdriver.common.html
--rw-r--r--   0 kazuaki    (501) staff       (20)   237013 2021-11-25 19:55:47.000000 Appium-Python-Client-2.8.1/docs/_build/html/appium.webdriver.extensions.android.html
--rw-r--r--   0 kazuaki    (501) staff       (20)   185363 2021-11-25 19:55:47.000000 Appium-Python-Client-2.8.1/docs/_build/html/appium.webdriver.extensions.html
--rw-r--r--   0 kazuaki    (501) staff       (20)    69528 2021-11-25 19:55:47.000000 Appium-Python-Client-2.8.1/docs/_build/html/appium.webdriver.extensions.search_context.html
--rw-r--r--   0 kazuaki    (501) staff       (20)   139852 2021-11-25 19:55:47.000000 Appium-Python-Client-2.8.1/docs/_build/html/appium.webdriver.html
--rw-r--r--   0 kazuaki    (501) staff       (20)   136243 2021-11-25 19:55:48.000000 Appium-Python-Client-2.8.1/docs/_build/html/genindex.html
--rw-r--r--   0 kazuaki    (501) staff       (20)     8361 2021-11-25 19:55:48.000000 Appium-Python-Client-2.8.1/docs/_build/html/index.html
--rw-r--r--   0 kazuaki    (501) staff       (20)     5508 2021-11-25 19:55:48.000000 Appium-Python-Client-2.8.1/docs/_build/html/objects.inv
--rw-r--r--   0 kazuaki    (501) staff       (20)    19014 2021-11-25 19:55:48.000000 Appium-Python-Client-2.8.1/docs/_build/html/py-modindex.html
--rw-r--r--   0 kazuaki    (501) staff       (20)     3625 2021-11-25 19:55:48.000000 Appium-Python-Client-2.8.1/docs/_build/html/search.html
--rw-r--r--   0 kazuaki    (501) staff       (20)    46698 2021-11-25 19:55:48.000000 Appium-Python-Client-2.8.1/docs/_build/html/searchindex.js
--rw-r--r--   0 kazuaki    (501) staff       (20)     2012 2021-10-31 06:04:06.000000 Appium-Python-Client-2.8.1/docs/conf.py
--rw-r--r--   0 kazuaki    (501) staff       (20)      107 2021-11-27 02:48:59.000000 Appium-Python-Client-2.8.1/docs/generate.sh
--rw-r--r--   0 kazuaki    (501) staff       (20)      489 2021-11-27 02:48:59.000000 Appium-Python-Client-2.8.1/docs/index.rst
--rw-r--r--   0 kazuaki    (501) staff       (20)      799 2020-05-03 09:17:34.000000 Appium-Python-Client-2.8.1/docs/make.bat
--rw-r--r--   0 kazuaki    (501) staff       (20)       44 2023-01-20 09:44:26.000000 Appium-Python-Client-2.8.1/docs/requirements.txt
--rw-r--r--   0 kazuaki    (501) staff       (20)      714 2021-11-27 02:48:59.000000 Appium-Python-Client-2.8.1/docs/webdriver.common.rst
--rw-r--r--   0 kazuaki    (501) staff       (20)     2208 2021-11-27 02:48:59.000000 Appium-Python-Client-2.8.1/docs/webdriver.extensions.android.rst
--rw-r--r--   0 kazuaki    (501) staff       (20)     3480 2021-11-27 02:48:59.000000 Appium-Python-Client-2.8.1/docs/webdriver.extensions.rst
--rw-r--r--   0 kazuaki    (501) staff       (20)     1595 2021-11-27 02:48:59.000000 Appium-Python-Client-2.8.1/docs/webdriver.extensions.search_context.rst
--rw-r--r--   0 kazuaki    (501) staff       (20)     1881 2021-11-27 02:48:59.000000 Appium-Python-Client-2.8.1/docs/webdriver.rst
--rw-r--r--   0 kazuaki    (501) staff       (20)      545 2023-01-21 04:10:49.262142 Appium-Python-Client-2.8.1/setup.cfg
--rw-r--r--   0 kazuaki    (501) staff       (20)     2066 2022-08-11 05:26:58.000000 Appium-Python-Client-2.8.1/setup.py
+drwxr-xr-x   0 kazuaki    (501) staff       (20)        0 2023-04-02 05:24:29.099295 Appium-Python-Client-2.9.0/
+drwxr-xr-x   0 kazuaki    (501) staff       (20)        0 2023-04-02 05:24:28.709602 Appium-Python-Client-2.9.0/Appium_Python_Client.egg-info/
+-rw-r--r--   0 kazuaki    (501) staff       (20)    12386 2023-04-02 05:24:28.000000 Appium-Python-Client-2.9.0/Appium_Python_Client.egg-info/PKG-INFO
+-rw-r--r--   0 kazuaki    (501) staff       (20)    20768 2023-04-02 05:24:28.000000 Appium-Python-Client-2.9.0/Appium_Python_Client.egg-info/SOURCES.txt
+-rw-r--r--   0 kazuaki    (501) staff       (20)        1 2023-04-02 05:24:28.000000 Appium-Python-Client-2.9.0/Appium_Python_Client.egg-info/dependency_links.txt
+-rw-r--r--   0 kazuaki    (501) staff       (20)       14 2023-04-02 05:24:28.000000 Appium-Python-Client-2.9.0/Appium_Python_Client.egg-info/requires.txt
+-rw-r--r--   0 kazuaki    (501) staff       (20)        7 2023-04-02 05:24:28.000000 Appium-Python-Client-2.9.0/Appium_Python_Client.egg-info/top_level.txt
+-rw-r--r--   0 kazuaki    (501) staff       (20)    11384 2020-05-09 02:13:31.000000 Appium-Python-Client-2.9.0/LICENSE
+-rw-r--r--   0 kazuaki    (501) staff       (20)       41 2017-06-08 13:16:26.000000 Appium-Python-Client-2.9.0/MANIFEST.in
+-rw-r--r--   0 kazuaki    (501) staff       (20)    12386 2023-04-02 05:24:29.099544 Appium-Python-Client-2.9.0/PKG-INFO
+-rw-r--r--   0 kazuaki    (501) staff       (20)    11290 2023-04-02 05:15:14.000000 Appium-Python-Client-2.9.0/README.md
+drwxr-xr-x   0 kazuaki    (501) staff       (20)        0 2023-04-02 05:24:28.710929 Appium-Python-Client-2.9.0/appium/
+-rw-r--r--   0 kazuaki    (501) staff       (20)      597 2020-05-16 16:30:37.000000 Appium-Python-Client-2.9.0/appium/__init__.py
+drwxr-xr-x   0 kazuaki    (501) staff       (20)        0 2023-04-02 05:24:28.712968 Appium-Python-Client-2.9.0/appium/common/
+-rw-r--r--   0 kazuaki    (501) staff       (20)      613 2019-01-11 07:10:41.000000 Appium-Python-Client-2.9.0/appium/common/__init__.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)      924 2022-02-26 05:26:28.000000 Appium-Python-Client-2.9.0/appium/common/exceptions.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1177 2022-02-26 05:26:28.000000 Appium-Python-Client-2.9.0/appium/common/helper.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)      863 2020-05-03 09:17:34.000000 Appium-Python-Client-2.9.0/appium/common/logger.py
+drwxr-xr-x   0 kazuaki    (501) staff       (20)        0 2023-04-02 05:24:28.713488 Appium-Python-Client-2.9.0/appium/options/
+-rw-r--r--   0 kazuaki    (501) staff       (20)        0 2022-06-14 05:42:03.000000 Appium-Python-Client-2.9.0/appium/options/__init__.py
+drwxr-xr-x   0 kazuaki    (501) staff       (20)        0 2023-04-02 05:24:28.713969 Appium-Python-Client-2.9.0/appium/options/android/
+-rw-r--r--   0 kazuaki    (501) staff       (20)       94 2022-06-14 05:42:03.000000 Appium-Python-Client-2.9.0/appium/options/android/__init__.py
+drwxr-xr-x   0 kazuaki    (501) staff       (20)        0 2023-04-02 05:24:28.714536 Appium-Python-Client-2.9.0/appium/options/android/common/
+-rw-r--r--   0 kazuaki    (501) staff       (20)        0 2022-06-28 18:07:38.000000 Appium-Python-Client-2.9.0/appium/options/android/common/__init__.py
+drwxr-xr-x   0 kazuaki    (501) staff       (20)        0 2023-04-02 05:24:28.729973 Appium-Python-Client-2.9.0/appium/options/android/common/adb/
+-rw-r--r--   0 kazuaki    (501) staff       (20)        0 2022-06-28 18:07:38.000000 Appium-Python-Client-2.9.0/appium/options/android/common/adb/__init__.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1673 2022-09-22 08:22:12.000000 Appium-Python-Client-2.9.0/appium/options/android/common/adb/adb_exec_timeout_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1338 2022-06-28 18:07:38.000000 Appium-Python-Client-2.9.0/appium/options/android/common/adb/adb_port_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1513 2022-06-28 18:07:38.000000 Appium-Python-Client-2.9.0/appium/options/android/common/adb/allow_delay_adb_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1676 2022-06-28 18:07:38.000000 Appium-Python-Client-2.9.0/appium/options/android/common/adb/build_tools_version_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1600 2022-06-28 18:07:38.000000 Appium-Python-Client-2.9.0/appium/options/android/common/adb/clear_device_logs_on_start_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1687 2022-06-28 18:07:38.000000 Appium-Python-Client-2.9.0/appium/options/android/common/adb/ignore_hidden_api_policy_error_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1727 2022-06-28 18:07:38.000000 Appium-Python-Client-2.9.0/appium/options/android/common/adb/logcat_filter_specs_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1432 2022-06-28 18:07:38.000000 Appium-Python-Client-2.9.0/appium/options/android/common/adb/logcat_format_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1750 2022-06-28 18:07:38.000000 Appium-Python-Client-2.9.0/appium/options/android/common/adb/mock_location_app_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1446 2022-06-28 18:07:38.000000 Appium-Python-Client-2.9.0/appium/options/android/common/adb/remote_adb_host_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1529 2022-06-28 18:07:38.000000 Appium-Python-Client-2.9.0/appium/options/android/common/adb/skip_logcat_capture_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1554 2022-06-28 18:07:38.000000 Appium-Python-Client-2.9.0/appium/options/android/common/adb/suppress_kill_server_option.py
+drwxr-xr-x   0 kazuaki    (501) staff       (20)        0 2023-04-02 05:24:28.738375 Appium-Python-Client-2.9.0/appium/options/android/common/app/
+-rw-r--r--   0 kazuaki    (501) staff       (20)        0 2022-06-28 18:07:38.000000 Appium-Python-Client-2.9.0/appium/options/android/common/app/__init__.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1662 2022-06-28 18:07:38.000000 Appium-Python-Client-2.9.0/appium/options/android/common/app/allow_test_packages_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1766 2022-09-22 08:22:12.000000 Appium-Python-Client-2.9.0/appium/options/android/common/app/android_install_timeout_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1462 2022-06-28 18:07:38.000000 Appium-Python-Client-2.9.0/appium/options/android/common/app/app_activity_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1455 2022-06-28 18:07:38.000000 Appium-Python-Client-2.9.0/appium/options/android/common/app/app_package_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1504 2022-06-28 18:07:38.000000 Appium-Python-Client-2.9.0/appium/options/android/common/app/app_wait_activity_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1735 2022-09-22 08:22:12.000000 Appium-Python-Client-2.9.0/appium/options/android/common/app/app_wait_duration_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1695 2022-06-28 18:07:38.000000 Appium-Python-Client-2.9.0/appium/options/android/common/app/app_wait_for_launch_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1499 2022-06-28 18:07:38.000000 Appium-Python-Client-2.9.0/appium/options/android/common/app/app_wait_package_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1574 2022-06-28 18:07:38.000000 Appium-Python-Client-2.9.0/appium/options/android/common/app/auto_grant_premissions_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1629 2022-06-28 18:07:38.000000 Appium-Python-Client-2.9.0/appium/options/android/common/app/enforce_app_install_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1478 2022-06-28 18:07:38.000000 Appium-Python-Client-2.9.0/appium/options/android/common/app/intent_action_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1498 2022-06-28 18:07:38.000000 Appium-Python-Client-2.9.0/appium/options/android/common/app/intent_category_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1465 2022-06-28 18:07:38.000000 Appium-Python-Client-2.9.0/appium/options/android/common/app/intent_flags_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1575 2022-06-28 18:07:38.000000 Appium-Python-Client-2.9.0/appium/options/android/common/app/optional_intent_arguments_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1797 2022-06-28 18:07:38.000000 Appium-Python-Client-2.9.0/appium/options/android/common/app/remote_apps_cache_limit_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1568 2022-06-28 18:07:38.000000 Appium-Python-Client-2.9.0/appium/options/android/common/app/uninstall_other_packages_option.py
+drwxr-xr-x   0 kazuaki    (501) staff       (20)        0 2023-04-02 05:24:28.743155 Appium-Python-Client-2.9.0/appium/options/android/common/avd/
+-rw-r--r--   0 kazuaki    (501) staff       (20)        0 2022-06-28 18:07:38.000000 Appium-Python-Client-2.9.0/appium/options/android/common/avd/__init__.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1306 2022-06-28 18:07:38.000000 Appium-Python-Client-2.9.0/appium/options/android/common/avd/avd_args_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1350 2022-06-28 18:07:38.000000 Appium-Python-Client-2.9.0/appium/options/android/common/avd/avd_env_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1681 2022-09-22 08:22:12.000000 Appium-Python-Client-2.9.0/appium/options/android/common/avd/avd_launch_timeout_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1503 2022-06-28 18:07:38.000000 Appium-Python-Client-2.9.0/appium/options/android/common/avd/avd_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1728 2022-09-22 08:22:12.000000 Appium-Python-Client-2.9.0/appium/options/android/common/avd/avd_ready_timeout_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1448 2022-06-28 18:07:38.000000 Appium-Python-Client-2.9.0/appium/options/android/common/avd/gps_enabled_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1541 2022-06-28 18:07:38.000000 Appium-Python-Client-2.9.0/appium/options/android/common/avd/network_speed_option.py
+drwxr-xr-x   0 kazuaki    (501) staff       (20)        0 2023-04-02 05:24:28.753169 Appium-Python-Client-2.9.0/appium/options/android/common/context/
+-rw-r--r--   0 kazuaki    (501) staff       (20)        0 2022-06-28 18:07:38.000000 Appium-Python-Client-2.9.0/appium/options/android/common/context/__init__.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1737 2022-09-22 08:22:12.000000 Appium-Python-Client-2.9.0/appium/options/android/common/context/auto_webview_timeout_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1634 2022-06-28 18:07:38.000000 Appium-Python-Client-2.9.0/appium/options/android/common/context/chrome_logging_prefs_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1493 2022-06-28 18:07:38.000000 Appium-Python-Client-2.9.0/appium/options/android/common/context/chrome_options_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1641 2022-06-28 18:07:38.000000 Appium-Python-Client-2.9.0/appium/options/android/common/context/chromedriver_args_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1904 2022-06-28 18:07:38.000000 Appium-Python-Client-2.9.0/appium/options/android/common/context/chromedriver_chrome_mapping_file_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1732 2022-06-28 18:07:38.000000 Appium-Python-Client-2.9.0/appium/options/android/common/context/chromedriver_disable_build_check_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1881 2022-09-27 08:12:17.000000 Appium-Python-Client-2.9.0/appium/options/android/common/context/chromedriver_executable_dir_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1487 2022-06-28 18:07:38.000000 Appium-Python-Client-2.9.0/appium/options/android/common/context/chromedriver_executable_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1482 2022-06-28 18:07:38.000000 Appium-Python-Client-2.9.0/appium/options/android/common/context/chromedriver_port_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1546 2022-06-28 18:07:38.000000 Appium-Python-Client-2.9.0/appium/options/android/common/context/chromedriver_ports_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1723 2022-06-28 18:07:38.000000 Appium-Python-Client-2.9.0/appium/options/android/common/context/chromedriver_use_system_executable_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1673 2022-06-28 18:07:38.000000 Appium-Python-Client-2.9.0/appium/options/android/common/context/ensure_webviews_have_pages_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1826 2022-06-28 18:07:38.000000 Appium-Python-Client-2.9.0/appium/options/android/common/context/extract_chrome_android_package_from_context_name_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1614 2022-06-28 18:07:38.000000 Appium-Python-Client-2.9.0/appium/options/android/common/context/native_web_screenshot_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1735 2022-06-28 18:07:38.000000 Appium-Python-Client-2.9.0/appium/options/android/common/context/recreate_chrome_driver_sessions_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1535 2022-06-28 18:07:38.000000 Appium-Python-Client-2.9.0/appium/options/android/common/context/show_chromedriver_log_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1602 2022-06-28 18:07:38.000000 Appium-Python-Client-2.9.0/appium/options/android/common/context/webview_devtools_port_option.py
+drwxr-xr-x   0 kazuaki    (501) staff       (20)        0 2023-04-02 05:24:28.754166 Appium-Python-Client-2.9.0/appium/options/android/common/localization/
+-rw-r--r--   0 kazuaki    (501) staff       (20)        0 2022-06-28 18:07:38.000000 Appium-Python-Client-2.9.0/appium/options/android/common/localization/__init__.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1530 2022-06-28 18:07:38.000000 Appium-Python-Client-2.9.0/appium/options/android/common/localization/locale_script_option.py
+drwxr-xr-x   0 kazuaki    (501) staff       (20)        0 2023-04-02 05:24:28.756841 Appium-Python-Client-2.9.0/appium/options/android/common/locking/
+-rw-r--r--   0 kazuaki    (501) staff       (20)        0 2022-06-28 18:07:38.000000 Appium-Python-Client-2.9.0/appium/options/android/common/locking/__init__.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1710 2022-06-28 18:07:38.000000 Appium-Python-Client-2.9.0/appium/options/android/common/locking/skip_unlock_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1426 2022-06-28 18:07:38.000000 Appium-Python-Client-2.9.0/appium/options/android/common/locking/unlock_key_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1512 2022-06-28 18:07:38.000000 Appium-Python-Client-2.9.0/appium/options/android/common/locking/unlock_strategy_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1702 2022-09-22 08:22:12.000000 Appium-Python-Client-2.9.0/appium/options/android/common/locking/unlock_success_timeout_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1475 2022-06-28 18:07:38.000000 Appium-Python-Client-2.9.0/appium/options/android/common/locking/unlock_type_option.py
+drwxr-xr-x   0 kazuaki    (501) staff       (20)        0 2023-04-02 05:24:28.758002 Appium-Python-Client-2.9.0/appium/options/android/common/mjpeg/
+-rw-r--r--   0 kazuaki    (501) staff       (20)        0 2022-06-28 18:07:38.000000 Appium-Python-Client-2.9.0/appium/options/android/common/mjpeg/__init__.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1647 2022-06-28 18:07:38.000000 Appium-Python-Client-2.9.0/appium/options/android/common/mjpeg/mjpeg_screenshot_url_option.py
+drwxr-xr-x   0 kazuaki    (501) staff       (20)        0 2023-04-02 05:24:28.759290 Appium-Python-Client-2.9.0/appium/options/android/common/other/
+-rw-r--r--   0 kazuaki    (501) staff       (20)        0 2022-06-28 18:07:38.000000 Appium-Python-Client-2.9.0/appium/options/android/common/other/__init__.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1736 2022-06-28 18:07:38.000000 Appium-Python-Client-2.9.0/appium/options/android/common/other/disable_suppress_accessibility_service_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1628 2022-06-28 18:07:38.000000 Appium-Python-Client-2.9.0/appium/options/android/common/other/user_profile_option.py
+drwxr-xr-x   0 kazuaki    (501) staff       (20)        0 2023-04-02 05:24:28.762652 Appium-Python-Client-2.9.0/appium/options/android/common/signing/
+-rw-r--r--   0 kazuaki    (501) staff       (20)        0 2022-06-28 18:07:38.000000 Appium-Python-Client-2.9.0/appium/options/android/common/signing/__init__.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1495 2022-06-28 18:07:38.000000 Appium-Python-Client-2.9.0/appium/options/android/common/signing/key_alias_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1525 2022-06-28 18:07:38.000000 Appium-Python-Client-2.9.0/appium/options/android/common/signing/key_password_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1550 2022-06-28 18:07:38.000000 Appium-Python-Client-2.9.0/appium/options/android/common/signing/keystore_password_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1511 2022-06-28 18:07:38.000000 Appium-Python-Client-2.9.0/appium/options/android/common/signing/keystore_path_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1647 2022-06-28 18:07:38.000000 Appium-Python-Client-2.9.0/appium/options/android/common/signing/no_sign_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1637 2022-06-28 18:07:38.000000 Appium-Python-Client-2.9.0/appium/options/android/common/signing/use_keystore_option.py
+drwxr-xr-x   0 kazuaki    (501) staff       (20)        0 2023-04-02 05:24:28.766858 Appium-Python-Client-2.9.0/appium/options/android/espresso/
+-rw-r--r--   0 kazuaki    (501) staff       (20)        0 2022-06-14 05:42:03.000000 Appium-Python-Client-2.9.0/appium/options/android/espresso/__init__.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1525 2022-06-28 18:07:38.000000 Appium-Python-Client-2.9.0/appium/options/android/espresso/activity_options_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1815 2022-06-28 18:07:38.000000 Appium-Python-Client-2.9.0/appium/options/android/espresso/app_locale_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)    11526 2022-06-28 18:07:38.000000 Appium-Python-Client-2.9.0/appium/options/android/espresso/base.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1878 2022-06-28 18:07:38.000000 Appium-Python-Client-2.9.0/appium/options/android/espresso/espresso_build_config_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1813 2022-09-22 08:22:12.000000 Appium-Python-Client-2.9.0/appium/options/android/espresso/espresso_server_launch_timeout_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1660 2022-06-28 18:07:38.000000 Appium-Python-Client-2.9.0/appium/options/android/espresso/force_espresso_rebuild_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1543 2022-06-28 18:07:38.000000 Appium-Python-Client-2.9.0/appium/options/android/espresso/intent_options_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1464 2022-06-28 18:07:38.000000 Appium-Python-Client-2.9.0/appium/options/android/espresso/show_gradle_log_option.py
+drwxr-xr-x   0 kazuaki    (501) staff       (20)        0 2023-04-02 05:24:28.771297 Appium-Python-Client-2.9.0/appium/options/android/uiautomator2/
+-rw-r--r--   0 kazuaki    (501) staff       (20)        0 2022-06-14 05:42:03.000000 Appium-Python-Client-2.9.0/appium/options/android/uiautomator2/__init__.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)    11716 2022-06-28 18:07:38.000000 Appium-Python-Client-2.9.0/appium/options/android/uiautomator2/base.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1566 2022-06-28 18:07:38.000000 Appium-Python-Client-2.9.0/appium/options/android/uiautomator2/disable_window_animation_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1628 2022-06-28 18:07:38.000000 Appium-Python-Client-2.9.0/appium/options/android/uiautomator2/mjpeg_server_port_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1687 2022-06-28 18:07:38.000000 Appium-Python-Client-2.9.0/appium/options/android/uiautomator2/skip_device_initialization_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1871 2022-06-28 18:07:38.000000 Appium-Python-Client-2.9.0/appium/options/android/uiautomator2/skip_server_installation_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1880 2022-09-22 08:22:12.000000 Appium-Python-Client-2.9.0/appium/options/android/uiautomator2/uiautomator2_server_install_timeout_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1871 2022-09-22 08:22:12.000000 Appium-Python-Client-2.9.0/appium/options/android/uiautomator2/uiautomator2_server_launch_timeout_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     2003 2022-09-22 08:22:12.000000 Appium-Python-Client-2.9.0/appium/options/android/uiautomator2/uiautomator2_server_read_timeout_option.py
+drwxr-xr-x   0 kazuaki    (501) staff       (20)        0 2023-04-02 05:24:28.799146 Appium-Python-Client-2.9.0/appium/options/common/
+-rw-r--r--   0 kazuaki    (501) staff       (20)       32 2022-06-14 05:42:03.000000 Appium-Python-Client-2.9.0/appium/options/common/__init__.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1395 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/common/app_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1484 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/common/auto_web_view_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1393 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/common/automation_name_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     4125 2022-06-28 18:07:38.000000 Appium-Python-Client-2.9.0/appium/options/common/base.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1356 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/common/bundle_id_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1447 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/common/clear_system_files_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1314 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/common/device_name_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1463 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/common/enable_performance_logging_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1445 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/common/event_timings_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1333 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/common/full_reset_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1464 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/common/is_headless_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1317 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/common/language_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1297 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/common/locale_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1698 2022-09-22 08:22:12.000000 Appium-Python-Client-2.9.0/appium/options/common/new_command_timeout_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1315 2022-08-11 05:26:58.000000 Appium-Python-Client-2.9.0/appium/options/common/no_reset_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1441 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/common/orientation_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1397 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/common/other_apps_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1375 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/common/postrun_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1425 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/common/prerun_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1599 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/common/print_page_source_on_find_failure_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1383 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/common/skip_log_capture_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1063 2022-06-14 05:42:03.000000 Appium-Python-Client-2.9.0/appium/options/common/supports_capabilities.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1382 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/common/system_host_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1386 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/common/system_port_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1285 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/common/udid_option.py
+drwxr-xr-x   0 kazuaki    (501) staff       (20)        0 2023-04-02 05:24:28.802300 Appium-Python-Client-2.9.0/appium/options/gecko/
+-rw-r--r--   0 kazuaki    (501) staff       (20)       31 2022-06-14 05:42:03.000000 Appium-Python-Client-2.9.0/appium/options/gecko/__init__.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1458 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/gecko/android_storage_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1893 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/gecko/base.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1441 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/gecko/firefox_options_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1757 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/gecko/marionette_port_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1409 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/gecko/verbosity_option.py
+drwxr-xr-x   0 kazuaki    (501) staff       (20)        0 2023-04-02 05:24:28.802892 Appium-Python-Client-2.9.0/appium/options/ios/
+-rw-r--r--   0 kazuaki    (501) staff       (20)       82 2022-06-14 05:42:03.000000 Appium-Python-Client-2.9.0/appium/options/ios/__init__.py
+drwxr-xr-x   0 kazuaki    (501) staff       (20)        0 2023-04-02 05:24:28.808736 Appium-Python-Client-2.9.0/appium/options/ios/safari/
+-rw-r--r--   0 kazuaki    (501) staff       (20)        0 2022-06-14 05:42:03.000000 Appium-Python-Client-2.9.0/appium/options/ios/safari/__init__.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1699 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/ios/safari/automatic_inspection_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1624 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/ios/safari/automatic_profiling_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1906 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/ios/safari/base.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1778 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/ios/safari/device_name_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1652 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/ios/safari/device_type_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1715 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/ios/safari/device_udid_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1680 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/ios/safari/platform_build_version_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1665 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/ios/safari/platform_version_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1621 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/ios/safari/use_simulator_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     2325 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/ios/safari/webkit_webrtc_option.py
+drwxr-xr-x   0 kazuaki    (501) staff       (20)        0 2023-04-02 05:24:28.810112 Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/
+-rw-r--r--   0 kazuaki    (501) staff       (20)        0 2022-06-14 05:42:03.000000 Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/__init__.py
+drwxr-xr-x   0 kazuaki    (501) staff       (20)        0 2023-04-02 05:24:28.812316 Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/app/
+-rw-r--r--   0 kazuaki    (501) staff       (20)        0 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/app/__init__.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1985 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/app/app_install_strategy_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1677 2022-09-22 08:22:12.000000 Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/app/app_push_timeout_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1512 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/app/localizable_strings_dir_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)    11038 2022-08-11 05:26:58.000000 Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/base.py
+drwxr-xr-x   0 kazuaki    (501) staff       (20)        0 2023-04-02 05:24:28.815222 Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/general/
+-rw-r--r--   0 kazuaki    (501) staff       (20)        0 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/general/__init__.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1783 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/general/include_device_caps_to_session_info_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1530 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/general/reset_location_service_option.py
+drwxr-xr-x   0 kazuaki    (501) staff       (20)        0 2023-04-02 05:24:28.817814 Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/other/
+-rw-r--r--   0 kazuaki    (501) staff       (20)        0 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/other/__init__.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     2627 2022-09-22 08:22:12.000000 Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/other/command_timeouts_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1710 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/other/launch_with_idb_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1427 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/other/show_ios_log_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1479 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/other/use_json_source_option.py
+drwxr-xr-x   0 kazuaki    (501) staff       (20)        0 2023-04-02 05:24:28.828009 Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/simulator/
+-rw-r--r--   0 kazuaki    (501) staff       (20)        0 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/simulator/__init__.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1703 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/simulator/calendar_access_authorized_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1374 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/simulator/calendar_format_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1890 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/simulator/connect_hardware_keyboard_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1425 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/simulator/custom_ssl_cert_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1594 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/simulator/enforce_fresh_simulator_creation_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     2127 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/simulator/force_simulator_software_keyboard_presence_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1485 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/simulator/ios_simulator_logs_predicate_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1514 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/simulator/keep_key_chains_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1858 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/simulator/keychains_exclude_patterns_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     2158 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/simulator/permissions_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1491 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/simulator/reduce_motion_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1731 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/simulator/reset_on_session_start_only_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1797 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/simulator/scale_factor_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1951 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/simulator/shutdown_other_simulators_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1695 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/simulator/simulator_devices_set_path_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1866 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/simulator/simulator_pasteboard_automatic_sync_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1919 2022-09-22 08:22:12.000000 Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/simulator/simulator_startup_timeout_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1644 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/simulator/simulator_trace_pointer_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1683 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/simulator/simulator_window_center_option.py
+drwxr-xr-x   0 kazuaki    (501) staff       (20)        0 2023-04-02 05:24:28.866002 Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/wda/
+-rw-r--r--   0 kazuaki    (501) staff       (20)        0 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/wda/__init__.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1774 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/wda/allow_provisioning_device_regitration_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1521 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/wda/auto_accept_alerts_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1531 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/wda/auto_disimiss_alerts_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1648 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/wda/derived_data_path_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1623 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/wda/disable_automatic_screenshots_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1711 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/wda/force_app_launch_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1433 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/wda/keychain_password_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1382 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/wda/keychain_path_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1556 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/wda/max_typing_frequency_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1692 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/wda/mjpeg_server_port_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1870 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/wda/process_arguments_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1702 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/wda/result_bundle_path_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1641 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/wda/screenshot_quality_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1705 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/wda/should_terminate_app_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1662 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/wda/should_use_singleton_test_manager_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1547 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/wda/show_xcode_log_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1817 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/wda/simple_is_visible_check_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1510 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/wda/updated_wda_bundle_id_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1715 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/wda/use_native_caching_strategy_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     2403 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/wda/use_new_wda_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1503 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/wda/use_prebuilt_wda_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1635 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/wda/use_simple_build_test_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     2497 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/wda/use_xctestrun_file_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     2074 2022-09-22 08:22:12.000000 Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/wda/wait_for_idle_timeout_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1726 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/wda/wait_for_quiescence_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1608 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/wda/wda_base_url_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1728 2022-09-22 08:22:12.000000 Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/wda/wda_connection_timeout_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     2124 2022-09-22 08:22:12.000000 Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/wda/wda_eventloop_idle_delay_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1702 2022-09-22 08:22:12.000000 Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/wda/wda_launch_timeout_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1558 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/wda/wda_local_port_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1469 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/wda/wda_startup_retries_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1772 2022-09-22 08:22:12.000000 Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/wda/wda_startup_retry_interval_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1471 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/wda/web_driver_agent_url_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1490 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/wda/xcode_org_id_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1490 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/wda/xcode_signing_id_option.py
+drwxr-xr-x   0 kazuaki    (501) staff       (20)        0 2023-04-02 05:24:28.875974 Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/webview/
+-rw-r--r--   0 kazuaki    (501) staff       (20)        0 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/webview/__init__.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1759 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/webview/absolute_web_locations_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1668 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/webview/additional_webview_bundle_ids_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1609 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/webview/enable_async_execute_from_https_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1698 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/webview/full_context_list_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1695 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/webview/include_safari_in_webviews_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1582 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/webview/native_web_tap_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1563 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/webview/safari_garbage_collect_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1557 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/webview/safari_ignore_fraud_warning_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1791 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/webview/safari_ignore_web_hostnames_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1395 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/webview/safari_initial_url_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1956 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/webview/safari_log_all_communication_hex_dump_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1674 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/webview/safari_log_all_communication_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1575 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/webview/safari_open_links_in_background_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1718 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/webview/safari_socket_chunk_size_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1788 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/webview/safari_web_inspector_max_frame_length_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1759 2022-09-22 08:22:12.000000 Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/webview/webkit_response_timeout_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1546 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/webview/webview_connect_retries_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1747 2022-09-22 08:22:12.000000 Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/webview/webview_connect_timeout_option.py
+drwxr-xr-x   0 kazuaki    (501) staff       (20)        0 2023-04-02 05:24:28.876570 Appium-Python-Client-2.9.0/appium/options/mac/
+-rw-r--r--   0 kazuaki    (501) staff       (20)       35 2022-06-14 05:42:03.000000 Appium-Python-Client-2.9.0/appium/options/mac/__init__.py
+drwxr-xr-x   0 kazuaki    (501) staff       (20)        0 2023-04-02 05:24:28.884217 Appium-Python-Client-2.9.0/appium/options/mac/mac2/
+-rw-r--r--   0 kazuaki    (501) staff       (20)        0 2022-06-14 05:42:03.000000 Appium-Python-Client-2.9.0/appium/options/mac/mac2/__init__.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1468 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/mac/mac2/arguments_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     4759 2022-08-11 07:46:16.000000 Appium-Python-Client-2.9.0/appium/options/mac/mac2/base.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1612 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/mac/mac2/bootstrap_root_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1637 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/mac/mac2/environment_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1761 2022-09-22 08:22:12.000000 Appium-Python-Client-2.9.0/appium/options/mac/mac2/server_startup_timeout_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1456 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/mac/mac2/show_server_logs_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1535 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/mac/mac2/skip_app_kill_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1557 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/mac/mac2/web_driver_agent_mac_url_option.py
+drwxr-xr-x   0 kazuaki    (501) staff       (20)        0 2023-04-02 05:24:28.885010 Appium-Python-Client-2.9.0/appium/options/windows/
+-rw-r--r--   0 kazuaki    (501) staff       (20)       41 2022-06-14 05:42:03.000000 Appium-Python-Client-2.9.0/appium/options/windows/__init__.py
+drwxr-xr-x   0 kazuaki    (501) staff       (20)        0 2023-04-02 05:24:28.889721 Appium-Python-Client-2.9.0/appium/options/windows/windows/
+-rw-r--r--   0 kazuaki    (501) staff       (20)        0 2022-06-14 05:42:03.000000 Appium-Python-Client-2.9.0/appium/options/windows/windows/__init__.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1506 2022-09-22 08:22:12.000000 Appium-Python-Client-2.9.0/appium/options/windows/windows/app_arguments_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1625 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/windows/windows/app_top_level_window_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1558 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/windows/windows/app_working_dir_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     4189 2022-09-22 08:22:12.000000 Appium-Python-Client-2.9.0/appium/options/windows/windows/base.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1928 2022-09-22 08:22:12.000000 Appium-Python-Client-2.9.0/appium/options/windows/windows/create_session_timeout_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1550 2022-06-26 05:30:16.000000 Appium-Python-Client-2.9.0/appium/options/windows/windows/expreimental_web_driver_option.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1846 2022-09-22 08:22:12.000000 Appium-Python-Client-2.9.0/appium/options/windows/windows/wait_for_app_launch_option.py
+drwxr-xr-x   0 kazuaki    (501) staff       (20)        0 2023-04-02 05:24:28.890709 Appium-Python-Client-2.9.0/appium/protocols/
+-rw-r--r--   0 kazuaki    (501) staff       (20)      567 2022-02-26 05:26:28.000000 Appium-Python-Client-2.9.0/appium/protocols/__init__.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)      776 2022-02-26 05:26:28.000000 Appium-Python-Client-2.9.0/appium/protocols/protocol.py
+drwxr-xr-x   0 kazuaki    (501) staff       (20)        0 2023-04-02 05:24:28.893283 Appium-Python-Client-2.9.0/appium/protocols/webdriver/
+-rw-r--r--   0 kazuaki    (501) staff       (20)      567 2022-02-26 05:26:28.000000 Appium-Python-Client-2.9.0/appium/protocols/webdriver/__init__.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)      882 2022-12-05 07:06:32.000000 Appium-Python-Client-2.9.0/appium/protocols/webdriver/can_execute_commands.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1044 2022-02-26 05:26:28.000000 Appium-Python-Client-2.9.0/appium/protocols/webdriver/can_execute_scripts.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)      976 2022-12-05 07:06:32.000000 Appium-Python-Client-2.9.0/appium/protocols/webdriver/can_find_elements.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)        0 2022-08-11 05:26:58.000000 Appium-Python-Client-2.9.0/appium/py.typed
+-rw-r--r--   0 kazuaki    (501) staff       (20)       18 2023-04-02 05:24:06.000000 Appium-Python-Client-2.9.0/appium/version.py
+drwxr-xr-x   0 kazuaki    (501) staff       (20)        0 2023-04-02 05:24:28.900933 Appium-Python-Client-2.9.0/appium/webdriver/
+-rw-r--r--   0 kazuaki    (501) staff       (20)      694 2019-01-11 07:10:41.000000 Appium-Python-Client-2.9.0/appium/webdriver/__init__.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     2880 2023-04-02 05:15:14.000000 Appium-Python-Client-2.9.0/appium/webdriver/appium_connection.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)    11038 2022-10-11 05:37:13.000000 Appium-Python-Client-2.9.0/appium/webdriver/appium_service.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)      735 2020-05-03 09:17:34.000000 Appium-Python-Client-2.9.0/appium/webdriver/applicationstate.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)      661 2020-05-03 09:17:34.000000 Appium-Python-Client-2.9.0/appium/webdriver/clipboard_content_type.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)      792 2021-11-25 19:12:21.000000 Appium-Python-Client-2.9.0/appium/webdriver/command_method.py
+drwxr-xr-x   0 kazuaki    (501) staff       (20)        0 2023-04-02 05:24:28.903866 Appium-Python-Client-2.9.0/appium/webdriver/common/
+-rw-r--r--   0 kazuaki    (501) staff       (20)      623 2019-01-11 07:10:41.000000 Appium-Python-Client-2.9.0/appium/webdriver/common/__init__.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1107 2021-12-23 22:07:15.000000 Appium-Python-Client-2.9.0/appium/webdriver/common/appiumby.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)      787 2022-02-26 05:26:28.000000 Appium-Python-Client-2.9.0/appium/webdriver/common/mobileby.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     3468 2022-06-28 18:07:38.000000 Appium-Python-Client-2.9.0/appium/webdriver/common/multi_action.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     6821 2022-12-05 07:06:32.000000 Appium-Python-Client-2.9.0/appium/webdriver/common/touch_action.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1567 2020-05-03 09:17:34.000000 Appium-Python-Client-2.9.0/appium/webdriver/connectiontype.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1137 2022-02-26 05:26:28.000000 Appium-Python-Client-2.9.0/appium/webdriver/errorhandler.py
+drwxr-xr-x   0 kazuaki    (501) staff       (20)        0 2023-04-02 05:24:28.914610 Appium-Python-Client-2.9.0/appium/webdriver/extensions/
+-rw-r--r--   0 kazuaki    (501) staff       (20)      567 2019-01-11 07:10:41.000000 Appium-Python-Client-2.9.0/appium/webdriver/extensions/__init__.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     7672 2022-08-11 05:26:58.000000 Appium-Python-Client-2.9.0/appium/webdriver/extensions/action_helpers.py
+drwxr-xr-x   0 kazuaki    (501) staff       (20)        0 2023-04-02 05:24:28.940240 Appium-Python-Client-2.9.0/appium/webdriver/extensions/android/
+-rw-r--r--   0 kazuaki    (501) staff       (20)        0 2019-05-12 06:29:12.000000 Appium-Python-Client-2.9.0/appium/webdriver/extensions/android/__init__.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     3920 2022-06-28 18:07:38.000000 Appium-Python-Client-2.9.0/appium/webdriver/extensions/android/activities.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     2537 2022-09-27 08:12:17.000000 Appium-Python-Client-2.9.0/appium/webdriver/extensions/android/common.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1411 2022-02-26 05:26:28.000000 Appium-Python-Client-2.9.0/appium/webdriver/extensions/android/display.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     4410 2022-06-28 18:07:38.000000 Appium-Python-Client-2.9.0/appium/webdriver/extensions/android/gsm.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)    30132 2021-10-31 06:04:06.000000 Appium-Python-Client-2.9.0/appium/webdriver/extensions/android/nativekey.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     4920 2022-06-28 18:07:38.000000 Appium-Python-Client-2.9.0/appium/webdriver/extensions/android/network.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     2769 2022-12-05 07:06:32.000000 Appium-Python-Client-2.9.0/appium/webdriver/extensions/android/performance.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     2256 2022-06-28 18:07:38.000000 Appium-Python-Client-2.9.0/appium/webdriver/extensions/android/power.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1600 2022-06-28 18:07:38.000000 Appium-Python-Client-2.9.0/appium/webdriver/extensions/android/sms.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1711 2022-02-26 05:26:28.000000 Appium-Python-Client-2.9.0/appium/webdriver/extensions/android/system_bars.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     8889 2022-12-05 07:06:32.000000 Appium-Python-Client-2.9.0/appium/webdriver/extensions/applications.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     3471 2022-06-28 18:07:38.000000 Appium-Python-Client-2.9.0/appium/webdriver/extensions/clipboard.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     2067 2022-02-26 05:26:28.000000 Appium-Python-Client-2.9.0/appium/webdriver/extensions/context.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     2212 2022-02-26 05:26:28.000000 Appium-Python-Client-2.9.0/appium/webdriver/extensions/device_time.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     2710 2022-02-26 05:26:28.000000 Appium-Python-Client-2.9.0/appium/webdriver/extensions/execute_driver.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     2380 2022-06-28 18:07:38.000000 Appium-Python-Client-2.9.0/appium/webdriver/extensions/execute_mobile_command.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     4182 2022-06-28 18:07:38.000000 Appium-Python-Client-2.9.0/appium/webdriver/extensions/hw_actions.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     7151 2022-02-26 05:26:28.000000 Appium-Python-Client-2.9.0/appium/webdriver/extensions/images_comparison.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     3580 2022-06-28 18:07:38.000000 Appium-Python-Client-2.9.0/appium/webdriver/extensions/ime.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     5130 2022-06-28 18:07:38.000000 Appium-Python-Client-2.9.0/appium/webdriver/extensions/keyboard.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     3338 2022-06-28 18:07:38.000000 Appium-Python-Client-2.9.0/appium/webdriver/extensions/location.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     2560 2022-12-05 07:06:32.000000 Appium-Python-Client-2.9.0/appium/webdriver/extensions/log_event.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     3548 2022-06-28 18:07:38.000000 Appium-Python-Client-2.9.0/appium/webdriver/extensions/remote_fs.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)    13010 2022-02-26 05:26:28.000000 Appium-Python-Client-2.9.0/appium/webdriver/extensions/screen_record.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     2275 2022-02-26 05:26:28.000000 Appium-Python-Client-2.9.0/appium/webdriver/extensions/session.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     2052 2022-09-27 08:12:17.000000 Appium-Python-Client-2.9.0/appium/webdriver/extensions/settings.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     3954 2023-01-21 04:09:09.000000 Appium-Python-Client-2.9.0/appium/webdriver/mobilecommand.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1414 2022-06-28 18:07:38.000000 Appium-Python-Client-2.9.0/appium/webdriver/switch_to.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)    21348 2023-04-02 05:15:14.000000 Appium-Python-Client-2.9.0/appium/webdriver/webdriver.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)     7823 2023-04-02 05:15:14.000000 Appium-Python-Client-2.9.0/appium/webdriver/webelement.py
+drwxr-xr-x   0 kazuaki    (501) staff       (20)        0 2023-04-02 05:24:28.948943 Appium-Python-Client-2.9.0/docs/
+-rw-r--r--   0 kazuaki    (501) staff       (20)     6148 2021-11-27 08:36:52.000000 Appium-Python-Client-2.9.0/docs/.DS_Store
+-rw-r--r--   0 kazuaki    (501) staff       (20)      634 2020-05-03 09:17:34.000000 Appium-Python-Client-2.9.0/docs/Makefile
+-rw-r--r--   0 kazuaki    (501) staff       (20)      323 2021-11-25 18:30:52.000000 Appium-Python-Client-2.9.0/docs/README.md
+drwxr-xr-x   0 kazuaki    (501) staff       (20)        0 2023-04-02 05:24:28.702581 Appium-Python-Client-2.9.0/docs/_build/
+drwxr-xr-x   0 kazuaki    (501) staff       (20)        0 2023-04-02 05:24:28.991658 Appium-Python-Client-2.9.0/docs/_build/doctrees/
+-rw-r--r--   0 kazuaki    (501) staff       (20)    22030 2021-11-25 19:55:43.000000 Appium-Python-Client-2.9.0/docs/_build/doctrees/appium.common.doctree
+-rw-r--r--   0 kazuaki    (501) staff       (20)     4702 2021-11-25 19:55:43.000000 Appium-Python-Client-2.9.0/docs/_build/doctrees/appium.doctree
+-rw-r--r--   0 kazuaki    (501) staff       (20)   100294 2021-11-25 19:55:44.000000 Appium-Python-Client-2.9.0/docs/_build/doctrees/appium.webdriver.common.doctree
+-rw-r--r--   0 kazuaki    (501) staff       (20)   377633 2021-11-25 19:55:44.000000 Appium-Python-Client-2.9.0/docs/_build/doctrees/appium.webdriver.doctree
+-rw-r--r--   0 kazuaki    (501) staff       (20)   685784 2021-11-25 19:55:46.000000 Appium-Python-Client-2.9.0/docs/_build/doctrees/appium.webdriver.extensions.android.doctree
+-rw-r--r--   0 kazuaki    (501) staff       (20)   620400 2021-11-25 19:55:45.000000 Appium-Python-Client-2.9.0/docs/_build/doctrees/appium.webdriver.extensions.doctree
+-rw-r--r--   0 kazuaki    (501) staff       (20)   191010 2021-11-25 19:55:46.000000 Appium-Python-Client-2.9.0/docs/_build/doctrees/appium.webdriver.extensions.search_context.doctree
+-rw-r--r--   0 kazuaki    (501) staff       (20)   209918 2021-11-25 19:55:46.000000 Appium-Python-Client-2.9.0/docs/_build/doctrees/environment.pickle
+-rw-r--r--   0 kazuaki    (501) staff       (20)     5039 2021-11-25 19:55:46.000000 Appium-Python-Client-2.9.0/docs/_build/doctrees/index.doctree
+drwxr-xr-x   0 kazuaki    (501) staff       (20)        0 2023-04-02 05:24:29.011266 Appium-Python-Client-2.9.0/docs/_build/html/
+-rw-r--r--   0 kazuaki    (501) staff       (20)      230 2021-11-25 19:55:48.000000 Appium-Python-Client-2.9.0/docs/_build/html/.buildinfo
+-rw-r--r--   0 kazuaki    (501) staff       (20)        0 2021-11-25 19:55:46.000000 Appium-Python-Client-2.9.0/docs/_build/html/.nojekyll
+drwxr-xr-x   0 kazuaki    (501) staff       (20)        0 2023-04-02 05:24:29.020205 Appium-Python-Client-2.9.0/docs/_build/html/_sources/
+-rw-r--r--   0 kazuaki    (501) staff       (20)      644 2021-11-25 19:55:41.000000 Appium-Python-Client-2.9.0/docs/_build/html/_sources/appium.common.rst.txt
+-rw-r--r--   0 kazuaki    (501) staff       (20)      388 2021-11-25 19:55:41.000000 Appium-Python-Client-2.9.0/docs/_build/html/_sources/appium.rst.txt
+-rw-r--r--   0 kazuaki    (501) staff       (20)      983 2021-11-25 19:55:41.000000 Appium-Python-Client-2.9.0/docs/_build/html/_sources/appium.webdriver.common.rst.txt
+-rw-r--r--   0 kazuaki    (501) staff       (20)     2439 2021-11-25 19:55:41.000000 Appium-Python-Client-2.9.0/docs/_build/html/_sources/appium.webdriver.extensions.android.rst.txt
+-rw-r--r--   0 kazuaki    (501) staff       (20)     3872 2021-11-25 19:55:41.000000 Appium-Python-Client-2.9.0/docs/_build/html/_sources/appium.webdriver.extensions.rst.txt
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1742 2021-11-25 19:55:41.000000 Appium-Python-Client-2.9.0/docs/_build/html/_sources/appium.webdriver.extensions.search_context.rst.txt
+-rw-r--r--   0 kazuaki    (501) staff       (20)     2310 2021-11-25 19:55:41.000000 Appium-Python-Client-2.9.0/docs/_build/html/_sources/appium.webdriver.rst.txt
+-rw-r--r--   0 kazuaki    (501) staff       (20)      486 2021-11-25 19:55:41.000000 Appium-Python-Client-2.9.0/docs/_build/html/_sources/index.rst.txt
+drwxr-xr-x   0 kazuaki    (501) staff       (20)        0 2023-04-02 05:24:29.035035 Appium-Python-Client-2.9.0/docs/_build/html/_static/
+-rw-r--r--   0 kazuaki    (501) staff       (20)    14667 2021-11-25 19:55:48.000000 Appium-Python-Client-2.9.0/docs/_build/html/_static/basic.css
+drwxr-xr-x   0 kazuaki    (501) staff       (20)        0 2023-04-02 05:24:29.036875 Appium-Python-Client-2.9.0/docs/_build/html/_static/css/
+-rw-r--r--   0 kazuaki    (501) staff       (20)     3275 2021-11-25 18:31:24.000000 Appium-Python-Client-2.9.0/docs/_build/html/_static/css/badge_only.css
+drwxr-xr-x   0 kazuaki    (501) staff       (20)        0 2023-04-02 05:24:29.083278 Appium-Python-Client-2.9.0/docs/_build/html/_static/css/fonts/
+-rw-r--r--   0 kazuaki    (501) staff       (20)    87624 2021-11-25 18:31:24.000000 Appium-Python-Client-2.9.0/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff
+-rw-r--r--   0 kazuaki    (501) staff       (20)    67312 2021-11-25 18:31:24.000000 Appium-Python-Client-2.9.0/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff2
+-rw-r--r--   0 kazuaki    (501) staff       (20)    86288 2021-11-25 18:31:24.000000 Appium-Python-Client-2.9.0/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff
+-rw-r--r--   0 kazuaki    (501) staff       (20)    66444 2021-11-25 18:31:24.000000 Appium-Python-Client-2.9.0/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff2
+-rw-r--r--   0 kazuaki    (501) staff       (20)   165742 2021-11-25 18:31:24.000000 Appium-Python-Client-2.9.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.eot
+-rw-r--r--   0 kazuaki    (501) staff       (20)   444379 2021-11-25 18:31:24.000000 Appium-Python-Client-2.9.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.svg
+-rw-r--r--   0 kazuaki    (501) staff       (20)   165548 2021-11-25 18:31:24.000000 Appium-Python-Client-2.9.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0 kazuaki    (501) staff       (20)    98024 2021-11-25 18:31:24.000000 Appium-Python-Client-2.9.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff
+-rw-r--r--   0 kazuaki    (501) staff       (20)    77160 2021-11-25 18:31:24.000000 Appium-Python-Client-2.9.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff2
+-rw-r--r--   0 kazuaki    (501) staff       (20)   323344 2021-11-25 18:31:24.000000 Appium-Python-Client-2.9.0/docs/_build/html/_static/css/fonts/lato-bold-italic.woff
+-rw-r--r--   0 kazuaki    (501) staff       (20)   193308 2021-11-25 18:31:24.000000 Appium-Python-Client-2.9.0/docs/_build/html/_static/css/fonts/lato-bold-italic.woff2
+-rw-r--r--   0 kazuaki    (501) staff       (20)   309728 2021-11-25 18:31:24.000000 Appium-Python-Client-2.9.0/docs/_build/html/_static/css/fonts/lato-bold.woff
+-rw-r--r--   0 kazuaki    (501) staff       (20)   184912 2021-11-25 18:31:24.000000 Appium-Python-Client-2.9.0/docs/_build/html/_static/css/fonts/lato-bold.woff2
+-rw-r--r--   0 kazuaki    (501) staff       (20)   328412 2021-11-25 18:31:24.000000 Appium-Python-Client-2.9.0/docs/_build/html/_static/css/fonts/lato-normal-italic.woff
+-rw-r--r--   0 kazuaki    (501) staff       (20)   195704 2021-11-25 18:31:24.000000 Appium-Python-Client-2.9.0/docs/_build/html/_static/css/fonts/lato-normal-italic.woff2
+-rw-r--r--   0 kazuaki    (501) staff       (20)   309192 2021-11-25 18:31:24.000000 Appium-Python-Client-2.9.0/docs/_build/html/_static/css/fonts/lato-normal.woff
+-rw-r--r--   0 kazuaki    (501) staff       (20)   182708 2021-11-25 18:31:24.000000 Appium-Python-Client-2.9.0/docs/_build/html/_static/css/fonts/lato-normal.woff2
+-rw-r--r--   0 kazuaki    (501) staff       (20)   129674 2021-11-25 18:31:24.000000 Appium-Python-Client-2.9.0/docs/_build/html/_static/css/theme.css
+-rw-r--r--   0 kazuaki    (501) staff       (20)     9630 2021-11-25 18:31:24.000000 Appium-Python-Client-2.9.0/docs/_build/html/_static/doctools.js
+-rw-r--r--   0 kazuaki    (501) staff       (20)      351 2021-11-25 19:55:48.000000 Appium-Python-Client-2.9.0/docs/_build/html/_static/documentation_options.js
+-rw-r--r--   0 kazuaki    (501) staff       (20)      286 2021-11-25 18:31:24.000000 Appium-Python-Client-2.9.0/docs/_build/html/_static/file.png
+-rw-r--r--   0 kazuaki    (501) staff       (20)   287630 2021-11-25 18:31:24.000000 Appium-Python-Client-2.9.0/docs/_build/html/_static/jquery-3.5.1.js
+-rw-r--r--   0 kazuaki    (501) staff       (20)    89476 2021-11-25 18:31:24.000000 Appium-Python-Client-2.9.0/docs/_build/html/_static/jquery.js
+drwxr-xr-x   0 kazuaki    (501) staff       (20)        0 2023-04-02 05:24:29.098571 Appium-Python-Client-2.9.0/docs/_build/html/_static/js/
+-rw-r--r--   0 kazuaki    (501) staff       (20)      934 2021-11-25 18:31:24.000000 Appium-Python-Client-2.9.0/docs/_build/html/_static/js/badge_only.js
+-rw-r--r--   0 kazuaki    (501) staff       (20)     4370 2021-11-25 18:31:24.000000 Appium-Python-Client-2.9.0/docs/_build/html/_static/js/html5shiv-printshiv.min.js
+-rw-r--r--   0 kazuaki    (501) staff       (20)     2734 2021-11-25 18:31:24.000000 Appium-Python-Client-2.9.0/docs/_build/html/_static/js/html5shiv.min.js
+-rw-r--r--   0 kazuaki    (501) staff       (20)     5023 2021-11-25 18:31:24.000000 Appium-Python-Client-2.9.0/docs/_build/html/_static/js/theme.js
+-rw-r--r--   0 kazuaki    (501) staff       (20)    10854 2021-11-25 19:55:48.000000 Appium-Python-Client-2.9.0/docs/_build/html/_static/language_data.js
+-rw-r--r--   0 kazuaki    (501) staff       (20)       90 2021-11-25 18:31:24.000000 Appium-Python-Client-2.9.0/docs/_build/html/_static/minus.png
+-rw-r--r--   0 kazuaki    (501) staff       (20)       90 2021-11-25 18:31:24.000000 Appium-Python-Client-2.9.0/docs/_build/html/_static/plus.png
+-rw-r--r--   0 kazuaki    (501) staff       (20)     4819 2021-11-25 19:55:48.000000 Appium-Python-Client-2.9.0/docs/_build/html/_static/pygments.css
+-rw-r--r--   0 kazuaki    (501) staff       (20)    16793 2021-11-25 18:31:24.000000 Appium-Python-Client-2.9.0/docs/_build/html/_static/searchtools.js
+-rw-r--r--   0 kazuaki    (501) staff       (20)    68420 2021-11-25 18:31:24.000000 Appium-Python-Client-2.9.0/docs/_build/html/_static/underscore-1.13.1.js
+-rw-r--r--   0 kazuaki    (501) staff       (20)    19530 2021-11-25 18:31:24.000000 Appium-Python-Client-2.9.0/docs/_build/html/_static/underscore.js
+-rw-r--r--   0 kazuaki    (501) staff       (20)    12068 2021-11-25 19:55:46.000000 Appium-Python-Client-2.9.0/docs/_build/html/appium.common.html
+-rw-r--r--   0 kazuaki    (501) staff       (20)    13788 2021-11-25 19:55:46.000000 Appium-Python-Client-2.9.0/docs/_build/html/appium.html
+-rw-r--r--   0 kazuaki    (501) staff       (20)    38641 2021-11-25 19:55:47.000000 Appium-Python-Client-2.9.0/docs/_build/html/appium.webdriver.common.html
+-rw-r--r--   0 kazuaki    (501) staff       (20)   237013 2021-11-25 19:55:47.000000 Appium-Python-Client-2.9.0/docs/_build/html/appium.webdriver.extensions.android.html
+-rw-r--r--   0 kazuaki    (501) staff       (20)   185363 2021-11-25 19:55:47.000000 Appium-Python-Client-2.9.0/docs/_build/html/appium.webdriver.extensions.html
+-rw-r--r--   0 kazuaki    (501) staff       (20)    69528 2021-11-25 19:55:47.000000 Appium-Python-Client-2.9.0/docs/_build/html/appium.webdriver.extensions.search_context.html
+-rw-r--r--   0 kazuaki    (501) staff       (20)   139852 2021-11-25 19:55:47.000000 Appium-Python-Client-2.9.0/docs/_build/html/appium.webdriver.html
+-rw-r--r--   0 kazuaki    (501) staff       (20)   136243 2021-11-25 19:55:48.000000 Appium-Python-Client-2.9.0/docs/_build/html/genindex.html
+-rw-r--r--   0 kazuaki    (501) staff       (20)     8361 2021-11-25 19:55:48.000000 Appium-Python-Client-2.9.0/docs/_build/html/index.html
+-rw-r--r--   0 kazuaki    (501) staff       (20)     5508 2021-11-25 19:55:48.000000 Appium-Python-Client-2.9.0/docs/_build/html/objects.inv
+-rw-r--r--   0 kazuaki    (501) staff       (20)    19014 2021-11-25 19:55:48.000000 Appium-Python-Client-2.9.0/docs/_build/html/py-modindex.html
+-rw-r--r--   0 kazuaki    (501) staff       (20)     3625 2021-11-25 19:55:48.000000 Appium-Python-Client-2.9.0/docs/_build/html/search.html
+-rw-r--r--   0 kazuaki    (501) staff       (20)    46698 2021-11-25 19:55:48.000000 Appium-Python-Client-2.9.0/docs/_build/html/searchindex.js
+-rw-r--r--   0 kazuaki    (501) staff       (20)     2012 2021-10-31 06:04:06.000000 Appium-Python-Client-2.9.0/docs/conf.py
+-rw-r--r--   0 kazuaki    (501) staff       (20)      107 2021-11-27 02:48:59.000000 Appium-Python-Client-2.9.0/docs/generate.sh
+-rw-r--r--   0 kazuaki    (501) staff       (20)      489 2021-11-27 02:48:59.000000 Appium-Python-Client-2.9.0/docs/index.rst
+-rw-r--r--   0 kazuaki    (501) staff       (20)      799 2020-05-03 09:17:34.000000 Appium-Python-Client-2.9.0/docs/make.bat
+-rw-r--r--   0 kazuaki    (501) staff       (20)       44 2023-01-20 09:44:26.000000 Appium-Python-Client-2.9.0/docs/requirements.txt
+-rw-r--r--   0 kazuaki    (501) staff       (20)      714 2021-11-27 02:48:59.000000 Appium-Python-Client-2.9.0/docs/webdriver.common.rst
+-rw-r--r--   0 kazuaki    (501) staff       (20)     2208 2021-11-27 02:48:59.000000 Appium-Python-Client-2.9.0/docs/webdriver.extensions.android.rst
+-rw-r--r--   0 kazuaki    (501) staff       (20)     3480 2021-11-27 02:48:59.000000 Appium-Python-Client-2.9.0/docs/webdriver.extensions.rst
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1595 2021-11-27 02:48:59.000000 Appium-Python-Client-2.9.0/docs/webdriver.extensions.search_context.rst
+-rw-r--r--   0 kazuaki    (501) staff       (20)     1881 2021-11-27 02:48:59.000000 Appium-Python-Client-2.9.0/docs/webdriver.rst
+-rw-r--r--   0 kazuaki    (501) staff       (20)      545 2023-04-02 05:24:29.100929 Appium-Python-Client-2.9.0/setup.cfg
+-rw-r--r--   0 kazuaki    (501) staff       (20)     2066 2022-08-11 05:26:58.000000 Appium-Python-Client-2.9.0/setup.py
```

### Comparing `Appium-Python-Client-2.8.1/Appium_Python_Client.egg-info/PKG-INFO` & `Appium-Python-Client-2.9.0/Appium_Python_Client.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Appium-Python-Client
-Version: 2.8.1
+Version: 2.9.0
 Summary: Python client for Appium
 Home-page: http://appium.io/
 Author: Isaac Murchie
 Author-email: isaac@saucelabs.com
 Maintainer: Kazuaki Matsuo, Mykola Mokhnach, Mori Atsushi
 License: Apache 2.0
 Keywords: appium,selenium,selenium 4,python client,mobile automation
@@ -139,15 +139,15 @@
 from appium.options.android import UiAutomator2Options
 from appium.webdriver.common.appiumby import AppiumBy
 
 options = UiAutomator2Options()
 options.platformVersion = '10'
 options.udid = '123456789ABC'
 options.app = PATH('../../../apps/test-app.apk')
-# Appium1 points to http://127.0.0.1:4723/wd/hub by default 
+# Appium1 points to http://127.0.0.1:4723/wd/hub by default
 self.driver = webdriver.Remote('http://127.0.0.1:4723', options=options)
 el = self.driver.find_element(by=AppiumBy.ACCESSIBILITY_ID, value='item')
 el.click()
 ```
 
 ```python
 # iOS environment
@@ -158,15 +158,15 @@
 from appium.options.ios import XCUITestOptions
 from appium.webdriver.common.appiumby import AppiumBy
 
 options = XCUITestOptions()
 options.platformVersion = '13.4'
 options.udid = '123456789ABC'
 options.app = PATH('../../apps/UICatalog.app.zip')
-# Appium1 points to http://127.0.0.1:4723/wd/hub by default 
+# Appium1 points to http://127.0.0.1:4723/wd/hub by default
 self.driver = webdriver.Remote('http://127.0.0.1:4723', options=options)
 el = self.driver.find_element(by=AppiumBy.ACCESSIBILITY_ID, value='item')
 el.click()
 ```
 
 ## Direct Connect URLs
 
@@ -182,26 +182,26 @@
 ```python
 from appium import webdriver
 # Options are only available since client version 2.3.0
 # If you use an older client then switch to desired_capabilities
 # instead: https://github.com/appium/python-client/pull/720
 from appium.options.ios import XCUITestOptions
 
-# load_capabilities API could be used to 
+# load_capabilities API could be used to
 # load options mapping stored in a dictionary
 options = XCUITestOptions().load_capabilities({
     'platformVersion': '13.4',
     'deviceName': 'iPhone Simulator',
     'app': PATH('../../apps/UICatalog.app.zip'),
 })
 
 self.driver = webdriver.Remote(
-    # Appium1 points to http://127.0.0.1:4723/wd/hub by default 
-    'http://127.0.0.1:4723', 
-    options=options, 
+    # Appium1 points to http://127.0.0.1:4723/wd/hub by default
+    'http://127.0.0.1:4723',
+    options=options,
     direct_connection=True
 )
 ```
 
 ## Relax SSL validation
 
 `strict_ssl` option allows you to send commands to an invalid certificate host like a self-signed one.
@@ -216,18 +216,70 @@
 options = AppiumOptions()
 options.platform_name = 'mac'
 options.automation_name = 'safari'
 # set_capability API allows to provide any custom option
 # calls to it could be chained
 options.set_capability('browser_name', 'safari')
 
-# Appium1 points to http://127.0.0.1:4723/wd/hub by default 
+# Appium1 points to http://127.0.0.1:4723/wd/hub by default
 self.driver = webdriver.Remote('http://127.0.0.1:4723', options=options, strict_ssl=False)
 ```
 
+## Set custom `AppiumConnection`
+
+The first argument of `webdriver.Remote` can set an arbitrary command executor for you.
+
+1. Set init arguments for the pool manager Appium Python client uses to manage http requests.
+
+```python
+from appium import webdriver
+from appium.options.ios import XCUITestOptions
+
+import urllib3
+from appium.webdriver.appium_connection import AppiumConnection
+
+# Retry connection error up to 3 times.
+init_args_for_pool_manage = {
+    'retries': urllib3.util.retry.Retry(total=3, connect=3, read=False)
+}
+appium_executor = AppiumConnection(remote_server_addr='http://127.0.0.1:4723',
+    init_args_for_pool_manage=init_args_for_pool_manage)
+
+options = XCUITestOptions()
+options.platformVersion = '13.4'
+options.udid = '123456789ABC'
+options.app = PATH('../../apps/UICatalog.app.zip')
+driver = webdriver.Remote(appium_executor, options=options)
+```
+
+
+2. Define a subclass of `AppiumConnection`
+
+```python
+from appium import webdriver
+from appium.options.ios import XCUITestOptions
+
+from appium.webdriver.appium_connection import AppiumConnection
+
+class CustomAppiumConnection(AppiumConnection):
+    # Can add your own methods for the custom class
+    pass
+
+custom_executor = CustomAppiumConnection(remote_server_addr='http://127.0.0.1:4723')
+
+options = XCUITestOptions().load_capabilities({
+    'platformVersion': '13.4',
+    'deviceName': 'iPhone Simulator',
+    'app': PATH('../../apps/UICatalog.app.zip'),
+})
+driver = webdriver.Remote(custom_executor, options=options)
+
+```
+
+
 ## Documentation
 
 - https://appium.github.io/python-client-sphinx/ is detailed documentation
 - [functional tests](test/functional) also may help to see concrete examples.
 
 ## Development
```

### Comparing `Appium-Python-Client-2.8.1/Appium_Python_Client.egg-info/SOURCES.txt` & `Appium-Python-Client-2.9.0/Appium_Python_Client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/LICENSE` & `Appium-Python-Client-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/PKG-INFO` & `Appium-Python-Client-2.9.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Appium-Python-Client
-Version: 2.8.1
+Version: 2.9.0
 Summary: Python client for Appium
 Home-page: http://appium.io/
 Author: Isaac Murchie
 Author-email: isaac@saucelabs.com
 Maintainer: Kazuaki Matsuo, Mykola Mokhnach, Mori Atsushi
 License: Apache 2.0
 Keywords: appium,selenium,selenium 4,python client,mobile automation
@@ -139,15 +139,15 @@
 from appium.options.android import UiAutomator2Options
 from appium.webdriver.common.appiumby import AppiumBy
 
 options = UiAutomator2Options()
 options.platformVersion = '10'
 options.udid = '123456789ABC'
 options.app = PATH('../../../apps/test-app.apk')
-# Appium1 points to http://127.0.0.1:4723/wd/hub by default 
+# Appium1 points to http://127.0.0.1:4723/wd/hub by default
 self.driver = webdriver.Remote('http://127.0.0.1:4723', options=options)
 el = self.driver.find_element(by=AppiumBy.ACCESSIBILITY_ID, value='item')
 el.click()
 ```
 
 ```python
 # iOS environment
@@ -158,15 +158,15 @@
 from appium.options.ios import XCUITestOptions
 from appium.webdriver.common.appiumby import AppiumBy
 
 options = XCUITestOptions()
 options.platformVersion = '13.4'
 options.udid = '123456789ABC'
 options.app = PATH('../../apps/UICatalog.app.zip')
-# Appium1 points to http://127.0.0.1:4723/wd/hub by default 
+# Appium1 points to http://127.0.0.1:4723/wd/hub by default
 self.driver = webdriver.Remote('http://127.0.0.1:4723', options=options)
 el = self.driver.find_element(by=AppiumBy.ACCESSIBILITY_ID, value='item')
 el.click()
 ```
 
 ## Direct Connect URLs
 
@@ -182,26 +182,26 @@
 ```python
 from appium import webdriver
 # Options are only available since client version 2.3.0
 # If you use an older client then switch to desired_capabilities
 # instead: https://github.com/appium/python-client/pull/720
 from appium.options.ios import XCUITestOptions
 
-# load_capabilities API could be used to 
+# load_capabilities API could be used to
 # load options mapping stored in a dictionary
 options = XCUITestOptions().load_capabilities({
     'platformVersion': '13.4',
     'deviceName': 'iPhone Simulator',
     'app': PATH('../../apps/UICatalog.app.zip'),
 })
 
 self.driver = webdriver.Remote(
-    # Appium1 points to http://127.0.0.1:4723/wd/hub by default 
-    'http://127.0.0.1:4723', 
-    options=options, 
+    # Appium1 points to http://127.0.0.1:4723/wd/hub by default
+    'http://127.0.0.1:4723',
+    options=options,
     direct_connection=True
 )
 ```
 
 ## Relax SSL validation
 
 `strict_ssl` option allows you to send commands to an invalid certificate host like a self-signed one.
@@ -216,18 +216,70 @@
 options = AppiumOptions()
 options.platform_name = 'mac'
 options.automation_name = 'safari'
 # set_capability API allows to provide any custom option
 # calls to it could be chained
 options.set_capability('browser_name', 'safari')
 
-# Appium1 points to http://127.0.0.1:4723/wd/hub by default 
+# Appium1 points to http://127.0.0.1:4723/wd/hub by default
 self.driver = webdriver.Remote('http://127.0.0.1:4723', options=options, strict_ssl=False)
 ```
 
+## Set custom `AppiumConnection`
+
+The first argument of `webdriver.Remote` can set an arbitrary command executor for you.
+
+1. Set init arguments for the pool manager Appium Python client uses to manage http requests.
+
+```python
+from appium import webdriver
+from appium.options.ios import XCUITestOptions
+
+import urllib3
+from appium.webdriver.appium_connection import AppiumConnection
+
+# Retry connection error up to 3 times.
+init_args_for_pool_manage = {
+    'retries': urllib3.util.retry.Retry(total=3, connect=3, read=False)
+}
+appium_executor = AppiumConnection(remote_server_addr='http://127.0.0.1:4723',
+    init_args_for_pool_manage=init_args_for_pool_manage)
+
+options = XCUITestOptions()
+options.platformVersion = '13.4'
+options.udid = '123456789ABC'
+options.app = PATH('../../apps/UICatalog.app.zip')
+driver = webdriver.Remote(appium_executor, options=options)
+```
+
+
+2. Define a subclass of `AppiumConnection`
+
+```python
+from appium import webdriver
+from appium.options.ios import XCUITestOptions
+
+from appium.webdriver.appium_connection import AppiumConnection
+
+class CustomAppiumConnection(AppiumConnection):
+    # Can add your own methods for the custom class
+    pass
+
+custom_executor = CustomAppiumConnection(remote_server_addr='http://127.0.0.1:4723')
+
+options = XCUITestOptions().load_capabilities({
+    'platformVersion': '13.4',
+    'deviceName': 'iPhone Simulator',
+    'app': PATH('../../apps/UICatalog.app.zip'),
+})
+driver = webdriver.Remote(custom_executor, options=options)
+
+```
+
+
 ## Documentation
 
 - https://appium.github.io/python-client-sphinx/ is detailed documentation
 - [functional tests](test/functional) also may help to see concrete examples.
 
 ## Development
```

### Comparing `Appium-Python-Client-2.8.1/README.md` & `Appium-Python-Client-2.9.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -111,15 +111,15 @@
 from appium.options.android import UiAutomator2Options
 from appium.webdriver.common.appiumby import AppiumBy
 
 options = UiAutomator2Options()
 options.platformVersion = '10'
 options.udid = '123456789ABC'
 options.app = PATH('../../../apps/test-app.apk')
-# Appium1 points to http://127.0.0.1:4723/wd/hub by default 
+# Appium1 points to http://127.0.0.1:4723/wd/hub by default
 self.driver = webdriver.Remote('http://127.0.0.1:4723', options=options)
 el = self.driver.find_element(by=AppiumBy.ACCESSIBILITY_ID, value='item')
 el.click()
 ```
 
 ```python
 # iOS environment
@@ -130,15 +130,15 @@
 from appium.options.ios import XCUITestOptions
 from appium.webdriver.common.appiumby import AppiumBy
 
 options = XCUITestOptions()
 options.platformVersion = '13.4'
 options.udid = '123456789ABC'
 options.app = PATH('../../apps/UICatalog.app.zip')
-# Appium1 points to http://127.0.0.1:4723/wd/hub by default 
+# Appium1 points to http://127.0.0.1:4723/wd/hub by default
 self.driver = webdriver.Remote('http://127.0.0.1:4723', options=options)
 el = self.driver.find_element(by=AppiumBy.ACCESSIBILITY_ID, value='item')
 el.click()
 ```
 
 ## Direct Connect URLs
 
@@ -154,26 +154,26 @@
 ```python
 from appium import webdriver
 # Options are only available since client version 2.3.0
 # If you use an older client then switch to desired_capabilities
 # instead: https://github.com/appium/python-client/pull/720
 from appium.options.ios import XCUITestOptions
 
-# load_capabilities API could be used to 
+# load_capabilities API could be used to
 # load options mapping stored in a dictionary
 options = XCUITestOptions().load_capabilities({
     'platformVersion': '13.4',
     'deviceName': 'iPhone Simulator',
     'app': PATH('../../apps/UICatalog.app.zip'),
 })
 
 self.driver = webdriver.Remote(
-    # Appium1 points to http://127.0.0.1:4723/wd/hub by default 
-    'http://127.0.0.1:4723', 
-    options=options, 
+    # Appium1 points to http://127.0.0.1:4723/wd/hub by default
+    'http://127.0.0.1:4723',
+    options=options,
     direct_connection=True
 )
 ```
 
 ## Relax SSL validation
 
 `strict_ssl` option allows you to send commands to an invalid certificate host like a self-signed one.
@@ -188,18 +188,70 @@
 options = AppiumOptions()
 options.platform_name = 'mac'
 options.automation_name = 'safari'
 # set_capability API allows to provide any custom option
 # calls to it could be chained
 options.set_capability('browser_name', 'safari')
 
-# Appium1 points to http://127.0.0.1:4723/wd/hub by default 
+# Appium1 points to http://127.0.0.1:4723/wd/hub by default
 self.driver = webdriver.Remote('http://127.0.0.1:4723', options=options, strict_ssl=False)
 ```
 
+## Set custom `AppiumConnection`
+
+The first argument of `webdriver.Remote` can set an arbitrary command executor for you.
+
+1. Set init arguments for the pool manager Appium Python client uses to manage http requests.
+
+```python
+from appium import webdriver
+from appium.options.ios import XCUITestOptions
+
+import urllib3
+from appium.webdriver.appium_connection import AppiumConnection
+
+# Retry connection error up to 3 times.
+init_args_for_pool_manage = {
+    'retries': urllib3.util.retry.Retry(total=3, connect=3, read=False)
+}
+appium_executor = AppiumConnection(remote_server_addr='http://127.0.0.1:4723',
+    init_args_for_pool_manage=init_args_for_pool_manage)
+
+options = XCUITestOptions()
+options.platformVersion = '13.4'
+options.udid = '123456789ABC'
+options.app = PATH('../../apps/UICatalog.app.zip')
+driver = webdriver.Remote(appium_executor, options=options)
+```
+
+
+2. Define a subclass of `AppiumConnection`
+
+```python
+from appium import webdriver
+from appium.options.ios import XCUITestOptions
+
+from appium.webdriver.appium_connection import AppiumConnection
+
+class CustomAppiumConnection(AppiumConnection):
+    # Can add your own methods for the custom class
+    pass
+
+custom_executor = CustomAppiumConnection(remote_server_addr='http://127.0.0.1:4723')
+
+options = XCUITestOptions().load_capabilities({
+    'platformVersion': '13.4',
+    'deviceName': 'iPhone Simulator',
+    'app': PATH('../../apps/UICatalog.app.zip'),
+})
+driver = webdriver.Remote(custom_executor, options=options)
+
+```
+
+
 ## Documentation
 
 - https://appium.github.io/python-client-sphinx/ is detailed documentation
 - [functional tests](test/functional) also may help to see concrete examples.
 
 ## Development
```

### Comparing `Appium-Python-Client-2.8.1/appium/__init__.py` & `Appium-Python-Client-2.9.0/appium/__init__.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/common/__init__.py` & `Appium-Python-Client-2.9.0/appium/common/__init__.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/common/exceptions.py` & `Appium-Python-Client-2.9.0/appium/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/common/helper.py` & `Appium-Python-Client-2.9.0/appium/common/helper.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/common/logger.py` & `Appium-Python-Client-2.9.0/appium/common/logger.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/android/common/adb/adb_exec_timeout_option.py` & `Appium-Python-Client-2.9.0/appium/options/android/common/adb/adb_exec_timeout_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/android/common/adb/adb_port_option.py` & `Appium-Python-Client-2.9.0/appium/options/android/common/adb/adb_port_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/android/common/adb/allow_delay_adb_option.py` & `Appium-Python-Client-2.9.0/appium/options/android/common/adb/allow_delay_adb_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/android/common/adb/build_tools_version_option.py` & `Appium-Python-Client-2.9.0/appium/options/android/common/adb/build_tools_version_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/android/common/adb/clear_device_logs_on_start_option.py` & `Appium-Python-Client-2.9.0/appium/options/android/common/adb/clear_device_logs_on_start_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/android/common/adb/ignore_hidden_api_policy_error_option.py` & `Appium-Python-Client-2.9.0/appium/options/android/common/adb/ignore_hidden_api_policy_error_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/android/common/adb/logcat_filter_specs_option.py` & `Appium-Python-Client-2.9.0/appium/options/android/common/adb/logcat_filter_specs_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/android/common/adb/logcat_format_option.py` & `Appium-Python-Client-2.9.0/appium/options/android/common/adb/logcat_format_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/android/common/adb/mock_location_app_option.py` & `Appium-Python-Client-2.9.0/appium/options/android/common/adb/mock_location_app_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/android/common/adb/remote_adb_host_option.py` & `Appium-Python-Client-2.9.0/appium/options/android/common/adb/remote_adb_host_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/android/common/adb/skip_logcat_capture_option.py` & `Appium-Python-Client-2.9.0/appium/options/android/common/adb/skip_logcat_capture_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/android/common/adb/suppress_kill_server_option.py` & `Appium-Python-Client-2.9.0/appium/options/android/common/adb/suppress_kill_server_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/android/common/app/allow_test_packages_option.py` & `Appium-Python-Client-2.9.0/appium/options/android/common/app/allow_test_packages_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/android/common/app/android_install_timeout_option.py` & `Appium-Python-Client-2.9.0/appium/options/android/common/app/android_install_timeout_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/android/common/app/app_activity_option.py` & `Appium-Python-Client-2.9.0/appium/options/android/common/app/app_activity_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/android/common/app/app_package_option.py` & `Appium-Python-Client-2.9.0/appium/options/android/common/app/app_package_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/android/common/app/app_wait_activity_option.py` & `Appium-Python-Client-2.9.0/appium/options/android/common/app/app_wait_activity_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/android/common/app/app_wait_duration_option.py` & `Appium-Python-Client-2.9.0/appium/options/android/common/app/app_wait_duration_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/android/common/app/app_wait_for_launch_option.py` & `Appium-Python-Client-2.9.0/appium/options/android/common/app/app_wait_for_launch_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/android/common/app/app_wait_package_option.py` & `Appium-Python-Client-2.9.0/appium/options/android/common/app/app_wait_package_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/android/common/app/auto_grant_premissions_option.py` & `Appium-Python-Client-2.9.0/appium/options/android/common/app/auto_grant_premissions_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/android/common/app/enforce_app_install_option.py` & `Appium-Python-Client-2.9.0/appium/options/android/common/app/enforce_app_install_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/android/common/app/intent_action_option.py` & `Appium-Python-Client-2.9.0/appium/options/android/common/app/intent_action_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/android/common/app/intent_category_option.py` & `Appium-Python-Client-2.9.0/appium/options/android/common/app/intent_category_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/android/common/app/intent_flags_option.py` & `Appium-Python-Client-2.9.0/appium/options/android/common/app/intent_flags_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/android/common/app/optional_intent_arguments_option.py` & `Appium-Python-Client-2.9.0/appium/options/android/common/app/optional_intent_arguments_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/android/common/app/remote_apps_cache_limit_option.py` & `Appium-Python-Client-2.9.0/appium/options/android/common/app/remote_apps_cache_limit_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/android/common/app/uninstall_other_packages_option.py` & `Appium-Python-Client-2.9.0/appium/options/android/common/app/uninstall_other_packages_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/android/common/avd/avd_args_option.py` & `Appium-Python-Client-2.9.0/appium/options/android/common/avd/avd_args_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/android/common/avd/avd_env_option.py` & `Appium-Python-Client-2.9.0/appium/options/android/common/avd/avd_env_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/android/common/avd/avd_launch_timeout_option.py` & `Appium-Python-Client-2.9.0/appium/options/android/common/avd/avd_launch_timeout_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/android/common/avd/avd_option.py` & `Appium-Python-Client-2.9.0/appium/options/android/common/avd/avd_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/android/common/avd/avd_ready_timeout_option.py` & `Appium-Python-Client-2.9.0/appium/options/android/common/avd/avd_ready_timeout_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/android/common/avd/gps_enabled_option.py` & `Appium-Python-Client-2.9.0/appium/options/android/common/avd/gps_enabled_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/android/common/avd/network_speed_option.py` & `Appium-Python-Client-2.9.0/appium/options/android/common/avd/network_speed_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/android/common/context/auto_webview_timeout_option.py` & `Appium-Python-Client-2.9.0/appium/options/android/common/context/auto_webview_timeout_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/android/common/context/chrome_logging_prefs_option.py` & `Appium-Python-Client-2.9.0/appium/options/android/common/context/chrome_logging_prefs_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/android/common/context/chrome_options_option.py` & `Appium-Python-Client-2.9.0/appium/options/android/common/context/chrome_options_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/android/common/context/chromedriver_args_option.py` & `Appium-Python-Client-2.9.0/appium/options/android/common/context/chromedriver_args_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/android/common/context/chromedriver_chrome_mapping_file_option.py` & `Appium-Python-Client-2.9.0/appium/options/android/common/context/chromedriver_chrome_mapping_file_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/android/common/context/chromedriver_disable_build_check_option.py` & `Appium-Python-Client-2.9.0/appium/options/android/common/context/chromedriver_disable_build_check_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/android/common/context/chromedriver_executable_dir_option.py` & `Appium-Python-Client-2.9.0/appium/options/android/common/context/chromedriver_executable_dir_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/android/common/context/chromedriver_executable_option.py` & `Appium-Python-Client-2.9.0/appium/options/android/common/context/chromedriver_executable_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/android/common/context/chromedriver_port_option.py` & `Appium-Python-Client-2.9.0/appium/options/android/common/context/chromedriver_port_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/android/common/context/chromedriver_ports_option.py` & `Appium-Python-Client-2.9.0/appium/options/android/common/context/chromedriver_ports_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/android/common/context/chromedriver_use_system_executable_option.py` & `Appium-Python-Client-2.9.0/appium/options/android/common/context/chromedriver_use_system_executable_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/android/common/context/ensure_webviews_have_pages_option.py` & `Appium-Python-Client-2.9.0/appium/options/android/common/context/ensure_webviews_have_pages_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/android/common/context/extract_chrome_android_package_from_context_name_option.py` & `Appium-Python-Client-2.9.0/appium/options/android/common/context/extract_chrome_android_package_from_context_name_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/android/common/context/native_web_screenshot_option.py` & `Appium-Python-Client-2.9.0/appium/options/android/common/context/native_web_screenshot_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/android/common/context/recreate_chrome_driver_sessions_option.py` & `Appium-Python-Client-2.9.0/appium/options/android/common/context/recreate_chrome_driver_sessions_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/android/common/context/show_chromedriver_log_option.py` & `Appium-Python-Client-2.9.0/appium/options/android/common/context/show_chromedriver_log_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/android/common/context/webview_devtools_port_option.py` & `Appium-Python-Client-2.9.0/appium/options/android/common/context/webview_devtools_port_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/android/common/localization/locale_script_option.py` & `Appium-Python-Client-2.9.0/appium/options/android/common/localization/locale_script_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/android/common/locking/skip_unlock_option.py` & `Appium-Python-Client-2.9.0/appium/options/android/common/locking/skip_unlock_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/android/common/locking/unlock_key_option.py` & `Appium-Python-Client-2.9.0/appium/options/android/common/locking/unlock_key_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/android/common/locking/unlock_strategy_option.py` & `Appium-Python-Client-2.9.0/appium/options/android/common/locking/unlock_strategy_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/android/common/locking/unlock_success_timeout_option.py` & `Appium-Python-Client-2.9.0/appium/options/android/common/locking/unlock_success_timeout_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/android/common/locking/unlock_type_option.py` & `Appium-Python-Client-2.9.0/appium/options/android/common/locking/unlock_type_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/android/common/mjpeg/mjpeg_screenshot_url_option.py` & `Appium-Python-Client-2.9.0/appium/options/android/common/mjpeg/mjpeg_screenshot_url_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/android/common/other/disable_suppress_accessibility_service_option.py` & `Appium-Python-Client-2.9.0/appium/options/android/common/other/disable_suppress_accessibility_service_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/android/common/other/user_profile_option.py` & `Appium-Python-Client-2.9.0/appium/options/android/common/other/user_profile_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/android/common/signing/key_alias_option.py` & `Appium-Python-Client-2.9.0/appium/options/android/common/signing/key_alias_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/android/common/signing/key_password_option.py` & `Appium-Python-Client-2.9.0/appium/options/android/common/signing/key_password_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/android/common/signing/keystore_password_option.py` & `Appium-Python-Client-2.9.0/appium/options/android/common/signing/keystore_password_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/android/common/signing/keystore_path_option.py` & `Appium-Python-Client-2.9.0/appium/options/android/common/signing/keystore_path_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/android/common/signing/no_sign_option.py` & `Appium-Python-Client-2.9.0/appium/options/android/common/signing/no_sign_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/android/common/signing/use_keystore_option.py` & `Appium-Python-Client-2.9.0/appium/options/android/common/signing/use_keystore_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/android/espresso/activity_options_option.py` & `Appium-Python-Client-2.9.0/appium/options/android/espresso/activity_options_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/android/espresso/app_locale_option.py` & `Appium-Python-Client-2.9.0/appium/options/android/espresso/app_locale_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/android/espresso/base.py` & `Appium-Python-Client-2.9.0/appium/options/android/espresso/base.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/android/espresso/espresso_build_config_option.py` & `Appium-Python-Client-2.9.0/appium/options/android/espresso/espresso_build_config_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/android/espresso/espresso_server_launch_timeout_option.py` & `Appium-Python-Client-2.9.0/appium/options/android/espresso/espresso_server_launch_timeout_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/android/espresso/force_espresso_rebuild_option.py` & `Appium-Python-Client-2.9.0/appium/options/android/espresso/force_espresso_rebuild_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/android/espresso/intent_options_option.py` & `Appium-Python-Client-2.9.0/appium/options/android/espresso/intent_options_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/android/espresso/show_gradle_log_option.py` & `Appium-Python-Client-2.9.0/appium/options/android/espresso/show_gradle_log_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/android/uiautomator2/base.py` & `Appium-Python-Client-2.9.0/appium/options/android/uiautomator2/base.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/android/uiautomator2/disable_window_animation_option.py` & `Appium-Python-Client-2.9.0/appium/options/android/uiautomator2/disable_window_animation_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/android/uiautomator2/mjpeg_server_port_option.py` & `Appium-Python-Client-2.9.0/appium/options/android/uiautomator2/mjpeg_server_port_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/android/uiautomator2/skip_device_initialization_option.py` & `Appium-Python-Client-2.9.0/appium/options/android/uiautomator2/skip_device_initialization_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/android/uiautomator2/skip_server_installation_option.py` & `Appium-Python-Client-2.9.0/appium/options/android/uiautomator2/skip_server_installation_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/android/uiautomator2/uiautomator2_server_install_timeout_option.py` & `Appium-Python-Client-2.9.0/appium/options/android/uiautomator2/uiautomator2_server_install_timeout_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/android/uiautomator2/uiautomator2_server_launch_timeout_option.py` & `Appium-Python-Client-2.9.0/appium/options/android/uiautomator2/uiautomator2_server_launch_timeout_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/android/uiautomator2/uiautomator2_server_read_timeout_option.py` & `Appium-Python-Client-2.9.0/appium/options/android/uiautomator2/uiautomator2_server_read_timeout_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/common/app_option.py` & `Appium-Python-Client-2.9.0/appium/options/common/app_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/common/auto_web_view_option.py` & `Appium-Python-Client-2.9.0/appium/options/common/auto_web_view_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/common/automation_name_option.py` & `Appium-Python-Client-2.9.0/appium/options/common/automation_name_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/common/base.py` & `Appium-Python-Client-2.9.0/appium/options/common/base.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/common/bundle_id_option.py` & `Appium-Python-Client-2.9.0/appium/options/common/bundle_id_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/common/clear_system_files_option.py` & `Appium-Python-Client-2.9.0/appium/options/common/clear_system_files_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/common/device_name_option.py` & `Appium-Python-Client-2.9.0/appium/options/common/device_name_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/common/enable_performance_logging_option.py` & `Appium-Python-Client-2.9.0/appium/options/common/enable_performance_logging_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/common/event_timings_option.py` & `Appium-Python-Client-2.9.0/appium/options/common/event_timings_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/common/full_reset_option.py` & `Appium-Python-Client-2.9.0/appium/options/common/full_reset_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/common/is_headless_option.py` & `Appium-Python-Client-2.9.0/appium/options/common/is_headless_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/common/language_option.py` & `Appium-Python-Client-2.9.0/appium/options/common/language_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/common/locale_option.py` & `Appium-Python-Client-2.9.0/appium/options/common/locale_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/common/new_command_timeout_option.py` & `Appium-Python-Client-2.9.0/appium/options/common/new_command_timeout_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/common/no_reset_option.py` & `Appium-Python-Client-2.9.0/appium/options/common/no_reset_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/common/orientation_option.py` & `Appium-Python-Client-2.9.0/appium/options/common/orientation_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/common/other_apps_option.py` & `Appium-Python-Client-2.9.0/appium/options/common/other_apps_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/common/postrun_option.py` & `Appium-Python-Client-2.9.0/appium/options/common/postrun_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/common/prerun_option.py` & `Appium-Python-Client-2.9.0/appium/options/common/prerun_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/common/print_page_source_on_find_failure_option.py` & `Appium-Python-Client-2.9.0/appium/options/common/print_page_source_on_find_failure_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/common/skip_log_capture_option.py` & `Appium-Python-Client-2.9.0/appium/options/common/skip_log_capture_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/common/supports_capabilities.py` & `Appium-Python-Client-2.9.0/appium/options/common/supports_capabilities.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/common/system_host_option.py` & `Appium-Python-Client-2.9.0/appium/options/common/system_host_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/common/system_port_option.py` & `Appium-Python-Client-2.9.0/appium/options/common/system_port_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/common/udid_option.py` & `Appium-Python-Client-2.9.0/appium/options/common/udid_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/gecko/android_storage_option.py` & `Appium-Python-Client-2.9.0/appium/options/gecko/android_storage_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/gecko/base.py` & `Appium-Python-Client-2.9.0/appium/options/gecko/base.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/gecko/firefox_options_option.py` & `Appium-Python-Client-2.9.0/appium/options/gecko/firefox_options_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/gecko/marionette_port_option.py` & `Appium-Python-Client-2.9.0/appium/options/gecko/marionette_port_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/gecko/verbosity_option.py` & `Appium-Python-Client-2.9.0/appium/options/gecko/verbosity_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/ios/safari/automatic_inspection_option.py` & `Appium-Python-Client-2.9.0/appium/options/ios/safari/automatic_inspection_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/ios/safari/automatic_profiling_option.py` & `Appium-Python-Client-2.9.0/appium/options/ios/safari/automatic_profiling_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/ios/safari/base.py` & `Appium-Python-Client-2.9.0/appium/options/ios/safari/base.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/ios/safari/device_name_option.py` & `Appium-Python-Client-2.9.0/appium/options/ios/safari/device_name_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/ios/safari/device_type_option.py` & `Appium-Python-Client-2.9.0/appium/options/ios/safari/device_type_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/ios/safari/device_udid_option.py` & `Appium-Python-Client-2.9.0/appium/options/ios/safari/device_udid_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/ios/safari/platform_build_version_option.py` & `Appium-Python-Client-2.9.0/appium/options/ios/safari/platform_build_version_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/ios/safari/platform_version_option.py` & `Appium-Python-Client-2.9.0/appium/options/ios/safari/platform_version_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/ios/safari/use_simulator_option.py` & `Appium-Python-Client-2.9.0/appium/options/ios/safari/use_simulator_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/ios/safari/webkit_webrtc_option.py` & `Appium-Python-Client-2.9.0/appium/options/ios/safari/webkit_webrtc_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/app/app_install_strategy_option.py` & `Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/app/app_install_strategy_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/app/app_push_timeout_option.py` & `Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/app/app_push_timeout_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/app/localizable_strings_dir_option.py` & `Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/app/localizable_strings_dir_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/base.py` & `Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/base.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/general/include_device_caps_to_session_info_option.py` & `Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/general/include_device_caps_to_session_info_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/general/reset_location_service_option.py` & `Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/general/reset_location_service_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/other/command_timeouts_option.py` & `Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/other/command_timeouts_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/other/launch_with_idb_option.py` & `Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/other/launch_with_idb_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/other/show_ios_log_option.py` & `Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/other/show_ios_log_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/other/use_json_source_option.py` & `Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/other/use_json_source_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/simulator/calendar_access_authorized_option.py` & `Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/simulator/calendar_access_authorized_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/simulator/calendar_format_option.py` & `Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/simulator/calendar_format_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/simulator/connect_hardware_keyboard_option.py` & `Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/simulator/connect_hardware_keyboard_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/simulator/custom_ssl_cert_option.py` & `Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/simulator/custom_ssl_cert_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/simulator/enforce_fresh_simulator_creation_option.py` & `Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/simulator/enforce_fresh_simulator_creation_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/simulator/force_simulator_software_keyboard_presence_option.py` & `Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/simulator/force_simulator_software_keyboard_presence_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/simulator/ios_simulator_logs_predicate_option.py` & `Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/simulator/ios_simulator_logs_predicate_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/simulator/keep_key_chains_option.py` & `Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/simulator/keep_key_chains_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/simulator/keychains_exclude_patterns_option.py` & `Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/simulator/keychains_exclude_patterns_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/simulator/permissions_option.py` & `Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/simulator/permissions_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/simulator/reduce_motion_option.py` & `Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/simulator/reduce_motion_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/simulator/reset_on_session_start_only_option.py` & `Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/simulator/reset_on_session_start_only_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/simulator/scale_factor_option.py` & `Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/simulator/scale_factor_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/simulator/shutdown_other_simulators_option.py` & `Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/simulator/shutdown_other_simulators_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/simulator/simulator_devices_set_path_option.py` & `Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/simulator/simulator_devices_set_path_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/simulator/simulator_pasteboard_automatic_sync_option.py` & `Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/simulator/simulator_pasteboard_automatic_sync_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/simulator/simulator_startup_timeout_option.py` & `Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/simulator/simulator_startup_timeout_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/simulator/simulator_trace_pointer_option.py` & `Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/simulator/simulator_trace_pointer_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/simulator/simulator_window_center_option.py` & `Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/simulator/simulator_window_center_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/wda/allow_provisioning_device_regitration_option.py` & `Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/wda/allow_provisioning_device_regitration_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/wda/auto_accept_alerts_option.py` & `Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/wda/auto_accept_alerts_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/wda/auto_disimiss_alerts_option.py` & `Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/wda/auto_disimiss_alerts_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/wda/derived_data_path_option.py` & `Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/wda/derived_data_path_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/wda/disable_automatic_screenshots_option.py` & `Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/wda/disable_automatic_screenshots_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/wda/force_app_launch_option.py` & `Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/wda/force_app_launch_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/wda/keychain_password_option.py` & `Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/wda/keychain_password_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/wda/keychain_path_option.py` & `Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/wda/keychain_path_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/wda/max_typing_frequency_option.py` & `Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/wda/max_typing_frequency_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/wda/mjpeg_server_port_option.py` & `Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/wda/mjpeg_server_port_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/wda/process_arguments_option.py` & `Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/wda/process_arguments_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/wda/result_bundle_path_option.py` & `Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/wda/result_bundle_path_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/wda/screenshot_quality_option.py` & `Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/wda/screenshot_quality_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/wda/should_terminate_app_option.py` & `Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/wda/should_terminate_app_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/wda/should_use_singleton_test_manager_option.py` & `Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/wda/should_use_singleton_test_manager_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/wda/show_xcode_log_option.py` & `Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/wda/show_xcode_log_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/wda/simple_is_visible_check_option.py` & `Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/wda/simple_is_visible_check_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/wda/updated_wda_bundle_id_option.py` & `Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/wda/updated_wda_bundle_id_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/wda/use_native_caching_strategy_option.py` & `Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/wda/use_native_caching_strategy_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/wda/use_new_wda_option.py` & `Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/wda/use_new_wda_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/wda/use_prebuilt_wda_option.py` & `Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/wda/use_prebuilt_wda_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/wda/use_simple_build_test_option.py` & `Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/wda/use_simple_build_test_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/wda/use_xctestrun_file_option.py` & `Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/wda/use_xctestrun_file_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/wda/wait_for_idle_timeout_option.py` & `Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/wda/wait_for_idle_timeout_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/wda/wait_for_quiescence_option.py` & `Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/wda/wait_for_quiescence_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/wda/wda_base_url_option.py` & `Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/wda/wda_base_url_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/wda/wda_connection_timeout_option.py` & `Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/wda/wda_connection_timeout_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/wda/wda_eventloop_idle_delay_option.py` & `Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/wda/wda_eventloop_idle_delay_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/wda/wda_launch_timeout_option.py` & `Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/wda/wda_launch_timeout_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/wda/wda_local_port_option.py` & `Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/wda/wda_local_port_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/wda/wda_startup_retries_option.py` & `Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/wda/wda_startup_retries_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/wda/wda_startup_retry_interval_option.py` & `Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/wda/wda_startup_retry_interval_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/wda/web_driver_agent_url_option.py` & `Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/wda/web_driver_agent_url_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/wda/xcode_org_id_option.py` & `Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/wda/xcode_org_id_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/wda/xcode_signing_id_option.py` & `Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/wda/xcode_signing_id_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/webview/absolute_web_locations_option.py` & `Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/webview/absolute_web_locations_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/webview/additional_webview_bundle_ids_option.py` & `Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/webview/additional_webview_bundle_ids_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/webview/enable_async_execute_from_https_option.py` & `Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/webview/enable_async_execute_from_https_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/webview/full_context_list_option.py` & `Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/webview/full_context_list_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/webview/include_safari_in_webviews_option.py` & `Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/webview/include_safari_in_webviews_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/webview/native_web_tap_option.py` & `Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/webview/native_web_tap_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/webview/safari_garbage_collect_option.py` & `Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/webview/safari_garbage_collect_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/webview/safari_ignore_fraud_warning_option.py` & `Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/webview/safari_ignore_fraud_warning_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/webview/safari_ignore_web_hostnames_option.py` & `Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/webview/safari_ignore_web_hostnames_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/webview/safari_initial_url_option.py` & `Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/webview/safari_initial_url_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/webview/safari_log_all_communication_hex_dump_option.py` & `Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/webview/safari_log_all_communication_hex_dump_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/webview/safari_log_all_communication_option.py` & `Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/webview/safari_log_all_communication_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/webview/safari_open_links_in_background_option.py` & `Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/webview/safari_open_links_in_background_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/webview/safari_socket_chunk_size_option.py` & `Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/webview/safari_socket_chunk_size_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/webview/safari_web_inspector_max_frame_length_option.py` & `Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/webview/safari_web_inspector_max_frame_length_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/webview/webkit_response_timeout_option.py` & `Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/webview/webkit_response_timeout_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/webview/webview_connect_retries_option.py` & `Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/webview/webview_connect_retries_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/ios/xcuitest/webview/webview_connect_timeout_option.py` & `Appium-Python-Client-2.9.0/appium/options/ios/xcuitest/webview/webview_connect_timeout_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/mac/mac2/arguments_option.py` & `Appium-Python-Client-2.9.0/appium/options/mac/mac2/arguments_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/mac/mac2/base.py` & `Appium-Python-Client-2.9.0/appium/options/mac/mac2/base.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/mac/mac2/bootstrap_root_option.py` & `Appium-Python-Client-2.9.0/appium/options/mac/mac2/bootstrap_root_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/mac/mac2/environment_option.py` & `Appium-Python-Client-2.9.0/appium/options/mac/mac2/environment_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/mac/mac2/server_startup_timeout_option.py` & `Appium-Python-Client-2.9.0/appium/options/mac/mac2/server_startup_timeout_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/mac/mac2/show_server_logs_option.py` & `Appium-Python-Client-2.9.0/appium/options/mac/mac2/show_server_logs_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/mac/mac2/skip_app_kill_option.py` & `Appium-Python-Client-2.9.0/appium/options/mac/mac2/skip_app_kill_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/mac/mac2/web_driver_agent_mac_url_option.py` & `Appium-Python-Client-2.9.0/appium/options/mac/mac2/web_driver_agent_mac_url_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/windows/windows/app_arguments_option.py` & `Appium-Python-Client-2.9.0/appium/options/windows/windows/app_arguments_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/windows/windows/app_top_level_window_option.py` & `Appium-Python-Client-2.9.0/appium/options/windows/windows/app_top_level_window_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/windows/windows/app_working_dir_option.py` & `Appium-Python-Client-2.9.0/appium/options/windows/windows/app_working_dir_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/windows/windows/base.py` & `Appium-Python-Client-2.9.0/appium/options/windows/windows/base.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/windows/windows/create_session_timeout_option.py` & `Appium-Python-Client-2.9.0/appium/options/windows/windows/create_session_timeout_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/windows/windows/expreimental_web_driver_option.py` & `Appium-Python-Client-2.9.0/appium/options/windows/windows/expreimental_web_driver_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/options/windows/windows/wait_for_app_launch_option.py` & `Appium-Python-Client-2.9.0/appium/options/windows/windows/wait_for_app_launch_option.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/protocols/__init__.py` & `Appium-Python-Client-2.9.0/appium/protocols/__init__.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/protocols/protocol.py` & `Appium-Python-Client-2.9.0/appium/protocols/protocol.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/protocols/webdriver/__init__.py` & `Appium-Python-Client-2.9.0/appium/protocols/webdriver/__init__.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/protocols/webdriver/can_execute_commands.py` & `Appium-Python-Client-2.9.0/appium/protocols/webdriver/can_execute_commands.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/protocols/webdriver/can_execute_scripts.py` & `Appium-Python-Client-2.9.0/appium/protocols/webdriver/can_execute_scripts.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/protocols/webdriver/can_find_elements.py` & `Appium-Python-Client-2.9.0/appium/protocols/webdriver/can_find_elements.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/webdriver/__init__.py` & `Appium-Python-Client-2.9.0/appium/webdriver/__init__.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/webdriver/appium_connection.py` & `Appium-Python-Client-2.9.0/appium/webdriver/appium_connection.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,37 +9,52 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import uuid
-from typing import TYPE_CHECKING, Any, Dict, Union
+from typing import TYPE_CHECKING, Any, Dict, Optional, Union
 
 import urllib3
 from selenium.webdriver.remote.remote_connection import RemoteConnection
 
 from appium.common.helper import library_version
 
 if TYPE_CHECKING:
     from urllib.parse import ParseResult
 
 
 class AppiumConnection(RemoteConnection):
+    def __init__(
+        self,
+        remote_server_addr: str,
+        keep_alive: bool = False,
+        ignore_proxy: Optional[bool] = False,
+        init_args_for_pool_manager: Union[Dict[str, Any], None] = None,
+    ):
+
+        # Need to call before super().__init__ in order to pass arguments for the pool manager in the super.
+        self._init_args_for_pool_manager = init_args_for_pool_manager or {}
+
+        super().__init__(remote_server_addr, keep_alive=keep_alive, ignore_proxy=ignore_proxy)
+
     def _get_connection_manager(self) -> Union[urllib3.PoolManager, urllib3.ProxyManager]:
         # https://github.com/SeleniumHQ/selenium/blob/0e0194b0e52a34e7df4b841f1ed74506beea5c3e/py/selenium/webdriver/remote/remote_connection.py#L134
         pool_manager_init_args = {'timeout': self._timeout}
-        # pylint: disable=E1101
+
         if self._ca_certs:
             pool_manager_init_args['cert_reqs'] = 'CERT_REQUIRED'
             pool_manager_init_args['ca_certs'] = self._ca_certs
         else:
             # This line is necessary to disable certificate verification
             pool_manager_init_args['cert_reqs'] = 'CERT_NONE'
 
+        pool_manager_init_args.update(self._init_args_for_pool_manager)
+
         return (
             urllib3.PoolManager(**pool_manager_init_args)
             if self._proxy_url is None
             else urllib3.ProxyManager(self._proxy_url, **pool_manager_init_args)
         )
 
     @classmethod
```

### Comparing `Appium-Python-Client-2.8.1/appium/webdriver/appium_service.py` & `Appium-Python-Client-2.9.0/appium/webdriver/appium_service.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/webdriver/applicationstate.py` & `Appium-Python-Client-2.9.0/appium/webdriver/applicationstate.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/webdriver/clipboard_content_type.py` & `Appium-Python-Client-2.9.0/appium/webdriver/clipboard_content_type.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/webdriver/command_method.py` & `Appium-Python-Client-2.9.0/appium/webdriver/command_method.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/webdriver/common/__init__.py` & `Appium-Python-Client-2.9.0/appium/webdriver/common/__init__.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/webdriver/common/appiumby.py` & `Appium-Python-Client-2.9.0/appium/webdriver/common/appiumby.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/webdriver/common/mobileby.py` & `Appium-Python-Client-2.9.0/appium/webdriver/common/mobileby.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/webdriver/common/multi_action.py` & `Appium-Python-Client-2.9.0/appium/webdriver/common/multi_action.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/webdriver/common/touch_action.py` & `Appium-Python-Client-2.9.0/appium/webdriver/common/touch_action.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/webdriver/connectiontype.py` & `Appium-Python-Client-2.9.0/appium/webdriver/connectiontype.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/webdriver/errorhandler.py` & `Appium-Python-Client-2.9.0/appium/webdriver/errorhandler.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/webdriver/extensions/__init__.py` & `Appium-Python-Client-2.9.0/appium/webdriver/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/webdriver/extensions/action_helpers.py` & `Appium-Python-Client-2.9.0/appium/webdriver/extensions/action_helpers.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/webdriver/extensions/android/activities.py` & `Appium-Python-Client-2.9.0/appium/webdriver/extensions/android/activities.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/webdriver/extensions/android/common.py` & `Appium-Python-Client-2.9.0/appium/webdriver/extensions/android/common.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/webdriver/extensions/android/display.py` & `Appium-Python-Client-2.9.0/appium/webdriver/extensions/android/display.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/webdriver/extensions/android/gsm.py` & `Appium-Python-Client-2.9.0/appium/webdriver/extensions/android/gsm.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/webdriver/extensions/android/nativekey.py` & `Appium-Python-Client-2.9.0/appium/webdriver/extensions/android/nativekey.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/webdriver/extensions/android/network.py` & `Appium-Python-Client-2.9.0/appium/webdriver/extensions/android/network.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/webdriver/extensions/android/performance.py` & `Appium-Python-Client-2.9.0/appium/webdriver/extensions/android/performance.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/webdriver/extensions/android/power.py` & `Appium-Python-Client-2.9.0/appium/webdriver/extensions/android/power.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/webdriver/extensions/android/sms.py` & `Appium-Python-Client-2.9.0/appium/webdriver/extensions/android/sms.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/webdriver/extensions/android/system_bars.py` & `Appium-Python-Client-2.9.0/appium/webdriver/extensions/android/system_bars.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/webdriver/extensions/applications.py` & `Appium-Python-Client-2.9.0/appium/webdriver/extensions/applications.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/webdriver/extensions/clipboard.py` & `Appium-Python-Client-2.9.0/appium/webdriver/extensions/clipboard.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/webdriver/extensions/context.py` & `Appium-Python-Client-2.9.0/appium/webdriver/extensions/context.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/webdriver/extensions/device_time.py` & `Appium-Python-Client-2.9.0/appium/webdriver/extensions/device_time.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/webdriver/extensions/execute_driver.py` & `Appium-Python-Client-2.9.0/appium/webdriver/extensions/execute_driver.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/webdriver/extensions/execute_mobile_command.py` & `Appium-Python-Client-2.9.0/appium/webdriver/extensions/execute_mobile_command.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/webdriver/extensions/hw_actions.py` & `Appium-Python-Client-2.9.0/appium/webdriver/extensions/hw_actions.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/webdriver/extensions/images_comparison.py` & `Appium-Python-Client-2.9.0/appium/webdriver/extensions/images_comparison.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/webdriver/extensions/ime.py` & `Appium-Python-Client-2.9.0/appium/webdriver/extensions/ime.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/webdriver/extensions/keyboard.py` & `Appium-Python-Client-2.9.0/appium/webdriver/extensions/keyboard.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/webdriver/extensions/location.py` & `Appium-Python-Client-2.9.0/appium/webdriver/extensions/location.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/webdriver/extensions/log_event.py` & `Appium-Python-Client-2.9.0/appium/webdriver/extensions/log_event.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/webdriver/extensions/remote_fs.py` & `Appium-Python-Client-2.9.0/appium/webdriver/extensions/remote_fs.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/webdriver/extensions/screen_record.py` & `Appium-Python-Client-2.9.0/appium/webdriver/extensions/screen_record.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/webdriver/extensions/session.py` & `Appium-Python-Client-2.9.0/appium/webdriver/extensions/session.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/webdriver/extensions/settings.py` & `Appium-Python-Client-2.9.0/appium/webdriver/extensions/settings.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/webdriver/mobilecommand.py` & `Appium-Python-Client-2.9.0/appium/webdriver/mobilecommand.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/webdriver/switch_to.py` & `Appium-Python-Client-2.9.0/appium/webdriver/switch_to.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/appium/webdriver/webdriver.py` & `Appium-Python-Client-2.9.0/appium/webdriver/webdriver.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # pylint: disable=too-many-lines,too-many-public-methods,too-many-statements,no-self-use
 
+import warnings
 from typing import Any, Callable, Dict, List, Optional, Tuple, TypeVar, Union
 
 from selenium import webdriver
 from selenium.common.exceptions import InvalidArgumentException, SessionNotCreatedException, WebDriverException
 from selenium.webdriver.common.by import By
 from selenium.webdriver.remote.command import Command as RemoteCommand
 from selenium.webdriver.remote.remote_connection import RemoteConnection
@@ -199,15 +200,15 @@
     Session,
     Settings,
     Sms,
     SystemBars,
 ):
     def __init__(
         self,
-        command_executor: str = 'http://127.0.0.1:4444/wd/hub',
+        command_executor: Union[str, AppiumConnection] = 'http://127.0.0.1:4444/wd/hub',
         desired_capabilities: Optional[Dict] = None,
         browser_profile: Union[str, None] = None,
         proxy: Union[str, None] = None,
         keep_alive: bool = True,
         direct_connection: bool = True,
         extensions: Optional[List['WebDriver']] = None,
         strict_ssl: bool = True,
@@ -223,16 +224,19 @@
             # noinspection PyPackageRequirements
             import urllib3.exceptions
 
             # noinspection PyUnresolvedReferences
             AppiumConnection.set_certificate_bundle_path(None)
             urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
 
+        if isinstance(command_executor, str):
+            command_executor = AppiumConnection(command_executor, keep_alive=keep_alive)
+
         super().__init__(
-            command_executor=AppiumConnection(command_executor, keep_alive=keep_alive),
+            command_executor=command_executor,
             desired_capabilities=desired_capabilities,
             browser_profile=browser_profile,
             proxy=proxy,
             options=options,
         )
 
         if hasattr(self, 'command_executor'):
@@ -430,26 +434,31 @@
         Returns:
             `MobileWebElement`
         """
         return MobileWebElement(self, element_id)
 
     def set_value(self: T, element: MobileWebElement, value: str) -> T:
         """Set the value on an element in the application.
+        deprecated:: 2.8.1
 
         Args:
             element: the element whose value will be set
             value: the value to set on the element
 
         Returns:
             `appium.webdriver.webdriver.WebDriver`: Self instance
         """
-        data = {
-            'id': element.id,
-            'value': [value],
-        }
+        warnings.warn(
+            'The "setValue" API is deprecated and will be removed in future versions. '
+            'Instead the "send_keys" API or W3C Actions can be used. '
+            'See https://github.com/appium/python-client/pull/831',
+            DeprecationWarning,
+        )
+
+        data = {'text': value}
         self.execute(Command.SET_IMMEDIATE_VALUE, data)
         return self
 
     @property
     def switch_to(self) -> MobileSwitchTo:
         """Returns an object containing all options to switch focus into
```

### Comparing `Appium-Python-Client-2.8.1/appium/webdriver/webelement.py` & `Appium-Python-Client-2.9.0/appium/webdriver/webelement.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import warnings
 from typing import Callable, Dict, List, Optional, Union
 
 from selenium.webdriver.common.utils import keys_to_typing
 from selenium.webdriver.remote.command import Command as RemoteCommand
 from selenium.webdriver.remote.webelement import WebElement as SeleniumWebElement
 
 from appium.webdriver.common.appiumby import AppiumBy
@@ -153,28 +154,36 @@
         """
         data = {'id': self.id}
         self._execute(Command.CLEAR, data)
         return self
 
     def set_text(self, keys: str = '') -> 'WebElement':
         """Sends text to the element.
+        deprecated:: 2.8.1
 
         Previous text is removed.
         Android only.
 
         Args:
             keys: the text to be sent to the element.
 
         Usage:
             element.set_text('some text')
 
         Returns:
             `appium.webdriver.webelement.WebElement`
         """
-        data = {'id': self._id, 'value': [keys]}
+        warnings.warn(
+            'The "setText" API is deprecated and will be removed in future versions. '
+            'Instead the "send_keys" API or W3C Actions can be used. '
+            'See https://github.com/appium/python-client/pull/831',
+            DeprecationWarning,
+        )
+
+        data = {'text': keys}
         self._execute(Command.REPLACE_KEYS, data)
         return self
 
     @property
     def location_in_view(self) -> Dict[str, int]:
         """Gets the location of an element relative to the view.
 
@@ -186,25 +195,30 @@
         Returns:
             dict: The location of an element relative to the view
         """
         return self._execute(Command.LOCATION_IN_VIEW)['value']
 
     def set_value(self, value: str) -> 'WebElement':
         """Set the value on this element in the application
+        deprecated:: 2.8.1
 
         Args:
             value: The value to be set
 
         Returns:
             `appium.webdriver.webelement.WebElement`
         """
-        data = {
-            'id': self.id,
-            'value': [value],
-        }
+        warnings.warn(
+            'The "setValue" API is deprecated and will be removed in future versions. '
+            'Instead the "send_keys" API or W3C Actions can be used. '
+            'See https://github.com/appium/python-client/pull/831',
+            DeprecationWarning,
+        )
+
+        data = {'text': value}
         self._execute(Command.SET_IMMEDIATE_VALUE, data)
         return self
 
     # Override
     def send_keys(self, *value: str) -> 'WebElement':
         """Simulates typing into the element.
```

### Comparing `Appium-Python-Client-2.8.1/docs/.DS_Store` & `Appium-Python-Client-2.9.0/docs/.DS_Store`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/docs/Makefile` & `Appium-Python-Client-2.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/docs/_build/doctrees/appium.common.doctree` & `Appium-Python-Client-2.9.0/docs/_build/doctrees/appium.common.doctree`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/docs/_build/doctrees/appium.doctree` & `Appium-Python-Client-2.9.0/docs/_build/doctrees/appium.doctree`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/docs/_build/doctrees/appium.webdriver.common.doctree` & `Appium-Python-Client-2.9.0/docs/_build/doctrees/appium.webdriver.common.doctree`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/docs/_build/doctrees/appium.webdriver.doctree` & `Appium-Python-Client-2.9.0/docs/_build/doctrees/appium.webdriver.doctree`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/docs/_build/doctrees/appium.webdriver.extensions.android.doctree` & `Appium-Python-Client-2.9.0/docs/_build/doctrees/appium.webdriver.extensions.android.doctree`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/docs/_build/doctrees/appium.webdriver.extensions.doctree` & `Appium-Python-Client-2.9.0/docs/_build/doctrees/appium.webdriver.extensions.doctree`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/docs/_build/doctrees/appium.webdriver.extensions.search_context.doctree` & `Appium-Python-Client-2.9.0/docs/_build/doctrees/appium.webdriver.extensions.search_context.doctree`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/docs/_build/doctrees/environment.pickle` & `Appium-Python-Client-2.9.0/docs/_build/doctrees/environment.pickle`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/docs/_build/doctrees/index.doctree` & `Appium-Python-Client-2.9.0/docs/_build/doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/docs/_build/html/_sources/appium.common.rst.txt` & `Appium-Python-Client-2.9.0/docs/_build/html/_sources/appium.common.rst.txt`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/docs/_build/html/_sources/appium.webdriver.common.rst.txt` & `Appium-Python-Client-2.9.0/docs/_build/html/_sources/appium.webdriver.common.rst.txt`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/docs/_build/html/_sources/appium.webdriver.extensions.android.rst.txt` & `Appium-Python-Client-2.9.0/docs/_build/html/_sources/appium.webdriver.extensions.android.rst.txt`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/docs/_build/html/_sources/appium.webdriver.extensions.rst.txt` & `Appium-Python-Client-2.9.0/docs/_build/html/_sources/appium.webdriver.extensions.rst.txt`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/docs/_build/html/_sources/appium.webdriver.extensions.search_context.rst.txt` & `Appium-Python-Client-2.9.0/docs/_build/html/_sources/appium.webdriver.extensions.search_context.rst.txt`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/docs/_build/html/_sources/appium.webdriver.rst.txt` & `Appium-Python-Client-2.9.0/docs/_build/html/_sources/appium.webdriver.rst.txt`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/docs/_build/html/_static/basic.css` & `Appium-Python-Client-2.9.0/docs/_build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/docs/_build/html/_static/css/badge_only.css` & `Appium-Python-Client-2.9.0/docs/_build/html/_static/css/badge_only.css`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff` & `Appium-Python-Client-2.9.0/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff2` & `Appium-Python-Client-2.9.0/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff2`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff` & `Appium-Python-Client-2.9.0/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff2` & `Appium-Python-Client-2.9.0/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff2`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/docs/_build/html/_static/css/fonts/fontawesome-webfont.eot` & `Appium-Python-Client-2.9.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/docs/_build/html/_static/css/fonts/fontawesome-webfont.svg` & `Appium-Python-Client-2.9.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/docs/_build/html/_static/css/fonts/fontawesome-webfont.ttf` & `Appium-Python-Client-2.9.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff` & `Appium-Python-Client-2.9.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff2` & `Appium-Python-Client-2.9.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/docs/_build/html/_static/css/fonts/lato-bold-italic.woff` & `Appium-Python-Client-2.9.0/docs/_build/html/_static/css/fonts/lato-bold-italic.woff`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/docs/_build/html/_static/css/fonts/lato-bold-italic.woff2` & `Appium-Python-Client-2.9.0/docs/_build/html/_static/css/fonts/lato-bold-italic.woff2`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/docs/_build/html/_static/css/fonts/lato-bold.woff` & `Appium-Python-Client-2.9.0/docs/_build/html/_static/css/fonts/lato-bold.woff`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/docs/_build/html/_static/css/fonts/lato-bold.woff2` & `Appium-Python-Client-2.9.0/docs/_build/html/_static/css/fonts/lato-bold.woff2`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/docs/_build/html/_static/css/fonts/lato-normal-italic.woff` & `Appium-Python-Client-2.9.0/docs/_build/html/_static/css/fonts/lato-normal-italic.woff`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/docs/_build/html/_static/css/fonts/lato-normal-italic.woff2` & `Appium-Python-Client-2.9.0/docs/_build/html/_static/css/fonts/lato-normal-italic.woff2`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/docs/_build/html/_static/css/fonts/lato-normal.woff` & `Appium-Python-Client-2.9.0/docs/_build/html/_static/css/fonts/lato-normal.woff`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/docs/_build/html/_static/css/fonts/lato-normal.woff2` & `Appium-Python-Client-2.9.0/docs/_build/html/_static/css/fonts/lato-normal.woff2`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/docs/_build/html/_static/css/theme.css` & `Appium-Python-Client-2.9.0/docs/_build/html/_static/css/theme.css`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/docs/_build/html/_static/doctools.js` & `Appium-Python-Client-2.9.0/docs/_build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/docs/_build/html/_static/jquery-3.5.1.js` & `Appium-Python-Client-2.9.0/docs/_build/html/_static/jquery-3.5.1.js`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/docs/_build/html/_static/jquery.js` & `Appium-Python-Client-2.9.0/docs/_build/html/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/docs/_build/html/_static/js/badge_only.js` & `Appium-Python-Client-2.9.0/docs/_build/html/_static/js/badge_only.js`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/docs/_build/html/_static/js/html5shiv-printshiv.min.js` & `Appium-Python-Client-2.9.0/docs/_build/html/_static/js/html5shiv-printshiv.min.js`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/docs/_build/html/_static/js/html5shiv.min.js` & `Appium-Python-Client-2.9.0/docs/_build/html/_static/js/html5shiv.min.js`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/docs/_build/html/_static/js/theme.js` & `Appium-Python-Client-2.9.0/docs/_build/html/_static/js/theme.js`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/docs/_build/html/_static/language_data.js` & `Appium-Python-Client-2.9.0/docs/_build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/docs/_build/html/_static/pygments.css` & `Appium-Python-Client-2.9.0/docs/_build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/docs/_build/html/_static/searchtools.js` & `Appium-Python-Client-2.9.0/docs/_build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/docs/_build/html/_static/underscore-1.13.1.js` & `Appium-Python-Client-2.9.0/docs/_build/html/_static/underscore-1.13.1.js`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/docs/_build/html/_static/underscore.js` & `Appium-Python-Client-2.9.0/docs/_build/html/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/docs/_build/html/appium.common.html` & `Appium-Python-Client-2.9.0/docs/_build/html/appium.common.html`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/docs/_build/html/appium.html` & `Appium-Python-Client-2.9.0/docs/_build/html/appium.html`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/docs/_build/html/appium.webdriver.common.html` & `Appium-Python-Client-2.9.0/docs/_build/html/appium.webdriver.common.html`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/docs/_build/html/appium.webdriver.extensions.android.html` & `Appium-Python-Client-2.9.0/docs/_build/html/appium.webdriver.extensions.android.html`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/docs/_build/html/appium.webdriver.extensions.html` & `Appium-Python-Client-2.9.0/docs/_build/html/appium.webdriver.extensions.html`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/docs/_build/html/appium.webdriver.extensions.search_context.html` & `Appium-Python-Client-2.9.0/docs/_build/html/appium.webdriver.extensions.search_context.html`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/docs/_build/html/appium.webdriver.html` & `Appium-Python-Client-2.9.0/docs/_build/html/appium.webdriver.html`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/docs/_build/html/genindex.html` & `Appium-Python-Client-2.9.0/docs/_build/html/genindex.html`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/docs/_build/html/index.html` & `Appium-Python-Client-2.9.0/docs/_build/html/index.html`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/docs/_build/html/objects.inv` & `Appium-Python-Client-2.9.0/docs/_build/html/objects.inv`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/docs/_build/html/py-modindex.html` & `Appium-Python-Client-2.9.0/docs/_build/html/py-modindex.html`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/docs/_build/html/search.html` & `Appium-Python-Client-2.9.0/docs/_build/html/search.html`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/docs/_build/html/searchindex.js` & `Appium-Python-Client-2.9.0/docs/_build/html/searchindex.js`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/docs/conf.py` & `Appium-Python-Client-2.9.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/docs/make.bat` & `Appium-Python-Client-2.9.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/docs/webdriver.common.rst` & `Appium-Python-Client-2.9.0/docs/webdriver.common.rst`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/docs/webdriver.extensions.android.rst` & `Appium-Python-Client-2.9.0/docs/webdriver.extensions.android.rst`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/docs/webdriver.extensions.rst` & `Appium-Python-Client-2.9.0/docs/webdriver.extensions.rst`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/docs/webdriver.extensions.search_context.rst` & `Appium-Python-Client-2.9.0/docs/webdriver.extensions.search_context.rst`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/docs/webdriver.rst` & `Appium-Python-Client-2.9.0/docs/webdriver.rst`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/setup.cfg` & `Appium-Python-Client-2.9.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `Appium-Python-Client-2.8.1/setup.py` & `Appium-Python-Client-2.9.0/setup.py`

 * *Files identical despite different names*

