# Comparing `tmp/v2ray-util-3.9.3.tar.gz` & `tmp/v2ray-util-3.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "v2ray-util-3.9.3.tar", last modified: Mon Feb 22 08:07:59 2021, max compression
+gzip compressed data, was "v2ray-util-3.9.4.tar", last modified: Thu Mar 11 06:50:17 2021, max compression
```

## Comparing `v2ray-util-3.9.3.tar` & `v2ray-util-3.9.4.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxrwxrwx   0        0        0        0 2021-02-22 08:07:59.867793 v2ray-util-3.9.3/
--rw-rw-rw-   0        0        0      312 2019-03-22 00:13:12.000000 v2ray-util-3.9.3/MANIFEST.in
--rw-rw-rw-   0        0        0     7177 2021-02-22 08:07:59.866796 v2ray-util-3.9.3/PKG-INFO
--rw-rw-rw-   0        0        0     4919 2021-02-22 07:39:28.000000 v2ray-util-3.9.3/README.md
--rw-rw-rw-   0        0        0       42 2021-02-22 08:07:59.868790 v2ray-util-3.9.3/setup.cfg
--rw-rw-rw-   0        0        0     1448 2020-12-14 05:27:40.000000 v2ray-util-3.9.3/setup.py
-drwxrwxrwx   0        0        0        0 2021-02-22 08:07:59.667330 v2ray-util-3.9.3/v2ray_util/
--rw-rw-rw-   0        0        0      142 2021-02-22 07:39:07.000000 v2ray-util-3.9.3/v2ray_util/__init__.py
-drwxrwxrwx   0        0        0        0 2021-02-22 08:07:59.770054 v2ray-util-3.9.3/v2ray_util/config_modify/
--rw-rw-rw-   0        0        0       31 2019-04-16 00:44:37.000000 v2ray-util-3.9.3/v2ray_util/config_modify/__init__.py
--rw-rw-rw-   0        0        0     6384 2020-12-09 02:31:43.000000 v2ray-util-3.9.3/v2ray_util/config_modify/base.py
--rw-rw-rw-   0        0        0     2808 2020-11-30 03:28:34.000000 v2ray-util-3.9.3/v2ray_util/config_modify/cdn.py
--rw-rw-rw-   0        0        0     5591 2020-11-30 03:04:27.000000 v2ray-util-3.9.3/v2ray_util/config_modify/multiple.py
--rw-rw-rw-   0        0        0     2099 2021-01-19 06:07:52.000000 v2ray-util-3.9.3/v2ray_util/config_modify/ss.py
--rw-rw-rw-   0        0        0     6373 2021-02-19 08:45:11.000000 v2ray-util-3.9.3/v2ray_util/config_modify/stream.py
--rw-rw-rw-   0        0        0     3703 2020-12-09 02:48:53.000000 v2ray-util-3.9.3/v2ray_util/config_modify/tls.py
-drwxrwxrwx   0        0        0        0 2021-02-22 08:07:59.791004 v2ray-util-3.9.3/v2ray_util/global_setting/
--rw-rw-rw-   0        0        0       31 2019-04-16 00:44:37.000000 v2ray-util-3.9.3/v2ray_util/global_setting/__init__.py
--rw-rw-rw-   0        0        0      615 2019-11-17 06:45:42.000000 v2ray-util-3.9.3/v2ray_util/global_setting/ban_bt.py
--rw-rw-rw-   0        0        0      715 2020-12-02 06:56:50.000000 v2ray-util-3.9.3/v2ray_util/global_setting/calcul_traffic.sh
--rw-rw-rw-   0        0        0      719 2020-12-02 06:57:07.000000 v2ray-util-3.9.3/v2ray_util/global_setting/clean_iptables.sh
--rw-rw-rw-   0        0        0      555 2020-12-02 06:57:23.000000 v2ray-util-3.9.3/v2ray_util/global_setting/clean_traffic.sh
--rw-rw-rw-   0        0        0     1259 2020-12-02 03:52:41.000000 v2ray-util-3.9.3/v2ray_util/global_setting/iptables_ctr.py
--rw-rw-rw-   0        0        0     7352 2020-12-09 03:32:14.000000 v2ray-util-3.9.3/v2ray_util/global_setting/stats_ctr.py
--rw-rw-rw-   0        0        0     2548 2020-12-09 06:27:18.000000 v2ray-util-3.9.3/v2ray_util/global_setting/update_timer.py
-drwxrwxrwx   0        0        0        0 2021-02-22 08:07:59.829895 v2ray-util-3.9.3/v2ray_util/json_template/
--rw-rw-rw-   0        0        0     1739 2020-10-12 06:17:45.000000 v2ray-util-3.9.3/v2ray_util/json_template/client.json
--rw-rw-rw-   0        0        0     1664 2019-03-22 00:13:12.000000 v2ray-util-3.9.3/v2ray_util/json_template/client_socks.json
--rw-rw-rw-   0        0        0     1222 2019-03-22 00:13:12.000000 v2ray-util-3.9.3/v2ray_util/json_template/client_ss.json
--rw-rw-rw-   0        0        0     1252 2020-10-12 06:26:22.000000 v2ray-util-3.9.3/v2ray_util/json_template/client_trojan.json
--rw-rw-rw-   0        0        0      245 2019-03-22 00:13:12.000000 v2ray-util-3.9.3/v2ray_util/json_template/dyn_port.json
--rw-rw-rw-   0        0        0     1366 2019-03-22 00:13:12.000000 v2ray-util-3.9.3/v2ray_util/json_template/http.json
--rw-rw-rw-   0        0        0      204 2019-03-22 00:13:12.000000 v2ray-util-3.9.3/v2ray_util/json_template/http2.json
--rw-rw-rw-   0        0        0      401 2019-03-22 00:13:12.000000 v2ray-util-3.9.3/v2ray_util/json_template/kcp.json
--rw-rw-rw-   0        0        0      392 2019-03-22 00:13:12.000000 v2ray-util-3.9.3/v2ray_util/json_template/mtproto.json
--rw-rw-rw-   0        0        0      272 2019-03-22 00:13:12.000000 v2ray-util-3.9.3/v2ray_util/json_template/quic.json
--rw-rw-rw-   0        0        0     1302 2020-10-12 06:13:48.000000 v2ray-util-3.9.3/v2ray_util/json_template/server.json
--rw-rw-rw-   0        0        0      126 2019-03-22 00:13:12.000000 v2ray-util-3.9.3/v2ray_util/json_template/socks.json
--rw-rw-rw-   0        0        0      157 2019-03-22 00:13:12.000000 v2ray-util-3.9.3/v2ray_util/json_template/ss.json
--rw-rw-rw-   0        0        0      638 2019-03-22 00:13:12.000000 v2ray-util-3.9.3/v2ray_util/json_template/stats_settings.json
--rw-rw-rw-   0        0        0      180 2019-03-22 00:13:12.000000 v2ray-util-3.9.3/v2ray_util/json_template/tcp.json
--rw-rw-rw-   0        0        0      160 2020-11-30 01:10:24.000000 v2ray-util-3.9.3/v2ray_util/json_template/vless.json
--rw-rw-rw-   0        0        0      229 2019-09-19 04:53:49.000000 v2ray-util-3.9.3/v2ray_util/json_template/ws.json
-drwxrwxrwx   0        0        0        0 2021-02-22 08:07:59.593528 v2ray-util-3.9.3/v2ray_util/locale_i18n/
-drwxrwxrwx   0        0        0        0 2021-02-22 08:07:59.592533 v2ray-util-3.9.3/v2ray_util/locale_i18n/en_US/
-drwxrwxrwx   0        0        0        0 2021-02-22 08:07:59.831890 v2ray-util-3.9.3/v2ray_util/locale_i18n/en_US/LC_MESSAGES/
--rw-rw-rw-   0        0        0      490 2020-11-30 02:53:09.000000 v2ray-util-3.9.3/v2ray_util/locale_i18n/en_US/LC_MESSAGES/lang.mo
-drwxrwxrwx   0        0        0        0 2021-02-22 08:07:59.594525 v2ray-util-3.9.3/v2ray_util/locale_i18n/zh_CH/
-drwxrwxrwx   0        0        0        0 2021-02-22 08:07:59.833883 v2ray-util-3.9.3/v2ray_util/locale_i18n/zh_CH/LC_MESSAGES/
--rw-rw-rw-   0        0        0    16321 2020-12-09 07:08:07.000000 v2ray-util-3.9.3/v2ray_util/locale_i18n/zh_CH/LC_MESSAGES/lang.mo
--rw-rw-rw-   0        0        0     9431 2020-12-25 01:54:43.000000 v2ray-util-3.9.3/v2ray_util/main.py
-drwxrwxrwx   0        0        0        0 2021-02-22 08:07:59.864801 v2ray-util-3.9.3/v2ray_util/util_core/
--rw-rw-rw-   0        0        0       20 2019-04-16 00:44:37.000000 v2ray-util-3.9.3/v2ray_util/util_core/__init__.py
--rw-rw-rw-   0        0        0     4407 2020-11-27 02:34:23.000000 v2ray-util-3.9.3/v2ray_util/util_core/client.py
--rw-rw-rw-   0        0        0      944 2020-12-08 08:25:58.000000 v2ray-util-3.9.3/v2ray_util/util_core/config.py
--rw-rw-rw-   0        0        0     9786 2021-02-22 07:11:41.000000 v2ray-util-3.9.3/v2ray_util/util_core/group.py
--rw-rw-rw-   0        0        0     1025 2019-12-30 01:44:43.000000 v2ray-util-3.9.3/v2ray_util/util_core/loader.py
--rw-rw-rw-   0        0        0     6910 2020-12-09 03:16:44.000000 v2ray-util-3.9.3/v2ray_util/util_core/profile.py
--rw-rw-rw-   0        0        0     3750 2020-10-15 10:15:47.000000 v2ray-util-3.9.3/v2ray_util/util_core/selector.py
--rw-rw-rw-   0        0        0      523 2020-12-09 02:10:01.000000 v2ray-util-3.9.3/v2ray_util/util_core/trans.py
--rw-rw-rw-   0        0        0       93 2020-08-21 07:41:48.000000 v2ray-util-3.9.3/v2ray_util/util_core/util.cfg
--rw-rw-rw-   0        0        0    10559 2021-02-19 08:45:11.000000 v2ray-util-3.9.3/v2ray_util/util_core/utils.py
--rw-rw-rw-   0        0        0     7701 2020-12-09 07:49:47.000000 v2ray-util-3.9.3/v2ray_util/util_core/v2ray.py
--rw-rw-rw-   0        0        0    25916 2021-02-19 08:45:11.000000 v2ray-util-3.9.3/v2ray_util/util_core/writer.py
-drwxrwxrwx   0        0        0        0 2021-02-22 08:07:59.751105 v2ray-util-3.9.3/v2ray_util.egg-info/
--rw-rw-rw-   0        0        0     7177 2021-02-22 08:07:57.000000 v2ray-util-3.9.3/v2ray_util.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1948 2021-02-22 08:07:58.000000 v2ray-util-3.9.3/v2ray_util.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-02-22 08:07:57.000000 v2ray-util-3.9.3/v2ray_util.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2021-02-22 08:07:57.000000 v2ray-util-3.9.3/v2ray_util.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2021-02-22 08:07:57.000000 v2ray-util-3.9.3/v2ray_util.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2021-02-22 08:07:57.000000 v2ray-util-3.9.3/v2ray_util.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2021-03-11 06:50:17.228819 v2ray-util-3.9.4/
+-rw-rw-rw-   0        0        0      312 2019-03-22 00:13:12.000000 v2ray-util-3.9.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     7177 2021-03-11 06:50:17.227822 v2ray-util-3.9.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4919 2021-02-22 07:39:28.000000 v2ray-util-3.9.4/README.md
+-rw-rw-rw-   0        0        0       42 2021-03-11 06:50:17.228819 v2ray-util-3.9.4/setup.cfg
+-rw-rw-rw-   0        0        0     1448 2020-12-14 05:27:40.000000 v2ray-util-3.9.4/setup.py
+drwxrwxrwx   0        0        0        0 2021-03-11 06:50:16.554627 v2ray-util-3.9.4/v2ray_util/
+-rw-rw-rw-   0        0        0      142 2021-03-11 06:49:32.000000 v2ray-util-3.9.4/v2ray_util/__init__.py
+drwxrwxrwx   0        0        0        0 2021-03-11 06:50:16.764065 v2ray-util-3.9.4/v2ray_util/config_modify/
+-rw-rw-rw-   0        0        0       31 2019-04-16 00:44:37.000000 v2ray-util-3.9.4/v2ray_util/config_modify/__init__.py
+-rw-rw-rw-   0        0        0     6384 2020-12-09 02:31:43.000000 v2ray-util-3.9.4/v2ray_util/config_modify/base.py
+-rw-rw-rw-   0        0        0     2808 2021-02-25 02:33:07.000000 v2ray-util-3.9.4/v2ray_util/config_modify/cdn.py
+-rw-rw-rw-   0        0        0     5591 2020-11-30 03:04:27.000000 v2ray-util-3.9.4/v2ray_util/config_modify/multiple.py
+-rw-rw-rw-   0        0        0     2099 2021-01-19 06:07:52.000000 v2ray-util-3.9.4/v2ray_util/config_modify/ss.py
+-rw-rw-rw-   0        0        0     6373 2021-02-25 02:33:07.000000 v2ray-util-3.9.4/v2ray_util/config_modify/stream.py
+-rw-rw-rw-   0        0        0     3703 2020-12-09 02:48:53.000000 v2ray-util-3.9.4/v2ray_util/config_modify/tls.py
+drwxrwxrwx   0        0        0        0 2021-03-11 06:50:16.968516 v2ray-util-3.9.4/v2ray_util/global_setting/
+-rw-rw-rw-   0        0        0       31 2019-04-16 00:44:37.000000 v2ray-util-3.9.4/v2ray_util/global_setting/__init__.py
+-rw-rw-rw-   0        0        0      615 2019-11-17 06:45:42.000000 v2ray-util-3.9.4/v2ray_util/global_setting/ban_bt.py
+-rw-rw-rw-   0        0        0      715 2020-12-02 06:56:50.000000 v2ray-util-3.9.4/v2ray_util/global_setting/calcul_traffic.sh
+-rw-rw-rw-   0        0        0      719 2020-12-02 06:57:07.000000 v2ray-util-3.9.4/v2ray_util/global_setting/clean_iptables.sh
+-rw-rw-rw-   0        0        0      555 2020-12-02 06:57:23.000000 v2ray-util-3.9.4/v2ray_util/global_setting/clean_traffic.sh
+-rw-rw-rw-   0        0        0     1259 2020-12-02 03:52:41.000000 v2ray-util-3.9.4/v2ray_util/global_setting/iptables_ctr.py
+-rw-rw-rw-   0        0        0     7352 2020-12-09 03:32:14.000000 v2ray-util-3.9.4/v2ray_util/global_setting/stats_ctr.py
+-rw-rw-rw-   0        0        0     2548 2020-12-09 06:27:18.000000 v2ray-util-3.9.4/v2ray_util/global_setting/update_timer.py
+drwxrwxrwx   0        0        0        0 2021-03-11 06:50:17.097174 v2ray-util-3.9.4/v2ray_util/json_template/
+-rw-rw-rw-   0        0        0     1739 2020-10-12 06:17:45.000000 v2ray-util-3.9.4/v2ray_util/json_template/client.json
+-rw-rw-rw-   0        0        0     1664 2019-03-22 00:13:12.000000 v2ray-util-3.9.4/v2ray_util/json_template/client_socks.json
+-rw-rw-rw-   0        0        0     1222 2019-03-22 00:13:12.000000 v2ray-util-3.9.4/v2ray_util/json_template/client_ss.json
+-rw-rw-rw-   0        0        0     1252 2020-10-12 06:26:22.000000 v2ray-util-3.9.4/v2ray_util/json_template/client_trojan.json
+-rw-rw-rw-   0        0        0      245 2019-03-22 00:13:12.000000 v2ray-util-3.9.4/v2ray_util/json_template/dyn_port.json
+-rw-rw-rw-   0        0        0     1366 2019-03-22 00:13:12.000000 v2ray-util-3.9.4/v2ray_util/json_template/http.json
+-rw-rw-rw-   0        0        0      204 2019-03-22 00:13:12.000000 v2ray-util-3.9.4/v2ray_util/json_template/http2.json
+-rw-rw-rw-   0        0        0      401 2019-03-22 00:13:12.000000 v2ray-util-3.9.4/v2ray_util/json_template/kcp.json
+-rw-rw-rw-   0        0        0      392 2019-03-22 00:13:12.000000 v2ray-util-3.9.4/v2ray_util/json_template/mtproto.json
+-rw-rw-rw-   0        0        0      272 2019-03-22 00:13:12.000000 v2ray-util-3.9.4/v2ray_util/json_template/quic.json
+-rw-rw-rw-   0        0        0     1302 2020-10-12 06:13:48.000000 v2ray-util-3.9.4/v2ray_util/json_template/server.json
+-rw-rw-rw-   0        0        0      126 2019-03-22 00:13:12.000000 v2ray-util-3.9.4/v2ray_util/json_template/socks.json
+-rw-rw-rw-   0        0        0      157 2019-03-22 00:13:12.000000 v2ray-util-3.9.4/v2ray_util/json_template/ss.json
+-rw-rw-rw-   0        0        0      638 2019-03-22 00:13:12.000000 v2ray-util-3.9.4/v2ray_util/json_template/stats_settings.json
+-rw-rw-rw-   0        0        0      180 2019-03-22 00:13:12.000000 v2ray-util-3.9.4/v2ray_util/json_template/tcp.json
+-rw-rw-rw-   0        0        0      160 2020-11-30 01:10:24.000000 v2ray-util-3.9.4/v2ray_util/json_template/vless.json
+-rw-rw-rw-   0        0        0      229 2019-09-19 04:53:49.000000 v2ray-util-3.9.4/v2ray_util/json_template/ws.json
+drwxrwxrwx   0        0        0        0 2021-03-11 06:50:16.537676 v2ray-util-3.9.4/v2ray_util/locale_i18n/
+drwxrwxrwx   0        0        0        0 2021-03-11 06:50:16.536953 v2ray-util-3.9.4/v2ray_util/locale_i18n/en_US/
+drwxrwxrwx   0        0        0        0 2021-03-11 06:50:17.113130 v2ray-util-3.9.4/v2ray_util/locale_i18n/en_US/LC_MESSAGES/
+-rw-rw-rw-   0        0        0      490 2020-11-30 02:53:09.000000 v2ray-util-3.9.4/v2ray_util/locale_i18n/en_US/LC_MESSAGES/lang.mo
+drwxrwxrwx   0        0        0        0 2021-03-11 06:50:16.539667 v2ray-util-3.9.4/v2ray_util/locale_i18n/zh_CH/
+drwxrwxrwx   0        0        0        0 2021-03-11 06:50:17.123102 v2ray-util-3.9.4/v2ray_util/locale_i18n/zh_CH/LC_MESSAGES/
+-rw-rw-rw-   0        0        0    16321 2020-12-09 07:08:07.000000 v2ray-util-3.9.4/v2ray_util/locale_i18n/zh_CH/LC_MESSAGES/lang.mo
+-rw-rw-rw-   0        0        0     9431 2020-12-25 01:54:43.000000 v2ray-util-3.9.4/v2ray_util/main.py
+drwxrwxrwx   0        0        0        0 2021-03-11 06:50:17.224832 v2ray-util-3.9.4/v2ray_util/util_core/
+-rw-rw-rw-   0        0        0       20 2019-04-16 00:44:37.000000 v2ray-util-3.9.4/v2ray_util/util_core/__init__.py
+-rw-rw-rw-   0        0        0     4407 2020-11-27 02:34:23.000000 v2ray-util-3.9.4/v2ray_util/util_core/client.py
+-rw-rw-rw-   0        0        0      944 2020-12-08 08:25:58.000000 v2ray-util-3.9.4/v2ray_util/util_core/config.py
+-rw-rw-rw-   0        0        0     9786 2021-03-11 06:48:13.000000 v2ray-util-3.9.4/v2ray_util/util_core/group.py
+-rw-rw-rw-   0        0        0     1025 2019-12-30 01:44:43.000000 v2ray-util-3.9.4/v2ray_util/util_core/loader.py
+-rw-rw-rw-   0        0        0     6910 2021-02-25 02:33:07.000000 v2ray-util-3.9.4/v2ray_util/util_core/profile.py
+-rw-rw-rw-   0        0        0     3750 2020-10-15 10:15:47.000000 v2ray-util-3.9.4/v2ray_util/util_core/selector.py
+-rw-rw-rw-   0        0        0      523 2020-12-09 02:10:01.000000 v2ray-util-3.9.4/v2ray_util/util_core/trans.py
+-rw-rw-rw-   0        0        0       93 2020-08-21 07:41:48.000000 v2ray-util-3.9.4/v2ray_util/util_core/util.cfg
+-rw-rw-rw-   0        0        0    10559 2021-02-25 02:33:07.000000 v2ray-util-3.9.4/v2ray_util/util_core/utils.py
+-rw-rw-rw-   0        0        0     7701 2020-12-09 07:49:47.000000 v2ray-util-3.9.4/v2ray_util/util_core/v2ray.py
+-rw-rw-rw-   0        0        0    25927 2021-03-11 06:48:00.000000 v2ray-util-3.9.4/v2ray_util/util_core/writer.py
+drwxrwxrwx   0        0        0        0 2021-03-11 06:50:16.680290 v2ray-util-3.9.4/v2ray_util.egg-info/
+-rw-rw-rw-   0        0        0     7177 2021-03-11 06:50:14.000000 v2ray-util-3.9.4/v2ray_util.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1948 2021-03-11 06:50:15.000000 v2ray-util-3.9.4/v2ray_util.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2021-03-11 06:50:14.000000 v2ray-util-3.9.4/v2ray_util.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2021-03-11 06:50:14.000000 v2ray-util-3.9.4/v2ray_util.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2021-03-11 06:50:14.000000 v2ray-util-3.9.4/v2ray_util.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2021-03-11 06:50:14.000000 v2ray-util-3.9.4/v2ray_util.egg-info/top_level.txt
```

### Comparing `v2ray-util-3.9.3/PKG-INFO` & `v2ray-util-3.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: v2ray-util
-Version: 3.9.3
+Version: 3.9.4
 Summary: a tool to manage v2ray config json
 Home-page: https://github.com/Jrohy/multi-v2ray
 Author: Jrohy
 Author-email: euvkzx@gmail.com
 License: GPL
 Description: # multi-v2ray
         V2ray/Xray多用户管理脚本，向导式管理[新增|删除|修改]传输协议
```

### Comparing `v2ray-util-3.9.3/README.md` & `v2ray-util-3.9.4/README.md`

 * *Files identical despite different names*

### Comparing `v2ray-util-3.9.3/setup.py` & `v2ray-util-3.9.4/setup.py`

 * *Files identical despite different names*

### Comparing `v2ray-util-3.9.3/v2ray_util/config_modify/base.py` & `v2ray-util-3.9.4/v2ray_util/config_modify/base.py`

 * *Files identical despite different names*

### Comparing `v2ray-util-3.9.3/v2ray_util/config_modify/cdn.py` & `v2ray-util-3.9.4/v2ray_util/config_modify/cdn.py`

 * *Files identical despite different names*

### Comparing `v2ray-util-3.9.3/v2ray_util/config_modify/multiple.py` & `v2ray-util-3.9.4/v2ray_util/config_modify/multiple.py`

 * *Files identical despite different names*

### Comparing `v2ray-util-3.9.3/v2ray_util/config_modify/ss.py` & `v2ray-util-3.9.4/v2ray_util/config_modify/ss.py`

 * *Files identical despite different names*

### Comparing `v2ray-util-3.9.3/v2ray_util/config_modify/stream.py` & `v2ray-util-3.9.4/v2ray_util/config_modify/stream.py`

 * *Files identical despite different names*

### Comparing `v2ray-util-3.9.3/v2ray_util/config_modify/tls.py` & `v2ray-util-3.9.4/v2ray_util/config_modify/tls.py`

 * *Files identical despite different names*

### Comparing `v2ray-util-3.9.3/v2ray_util/global_setting/ban_bt.py` & `v2ray-util-3.9.4/v2ray_util/global_setting/ban_bt.py`

 * *Files identical despite different names*

### Comparing `v2ray-util-3.9.3/v2ray_util/global_setting/calcul_traffic.sh` & `v2ray-util-3.9.4/v2ray_util/global_setting/calcul_traffic.sh`

 * *Files identical despite different names*

### Comparing `v2ray-util-3.9.3/v2ray_util/global_setting/clean_iptables.sh` & `v2ray-util-3.9.4/v2ray_util/global_setting/clean_iptables.sh`

 * *Files identical despite different names*

### Comparing `v2ray-util-3.9.3/v2ray_util/global_setting/clean_traffic.sh` & `v2ray-util-3.9.4/v2ray_util/global_setting/clean_traffic.sh`

 * *Files identical despite different names*

### Comparing `v2ray-util-3.9.3/v2ray_util/global_setting/iptables_ctr.py` & `v2ray-util-3.9.4/v2ray_util/global_setting/iptables_ctr.py`

 * *Files identical despite different names*

### Comparing `v2ray-util-3.9.3/v2ray_util/global_setting/stats_ctr.py` & `v2ray-util-3.9.4/v2ray_util/global_setting/stats_ctr.py`

 * *Files identical despite different names*

### Comparing `v2ray-util-3.9.3/v2ray_util/global_setting/update_timer.py` & `v2ray-util-3.9.4/v2ray_util/global_setting/update_timer.py`

 * *Files identical despite different names*

### Comparing `v2ray-util-3.9.3/v2ray_util/json_template/client.json` & `v2ray-util-3.9.4/v2ray_util/json_template/client.json`

 * *Files identical despite different names*

### Comparing `v2ray-util-3.9.3/v2ray_util/json_template/client_socks.json` & `v2ray-util-3.9.4/v2ray_util/json_template/client_socks.json`

 * *Files identical despite different names*

### Comparing `v2ray-util-3.9.3/v2ray_util/json_template/client_ss.json` & `v2ray-util-3.9.4/v2ray_util/json_template/client_ss.json`

 * *Files identical despite different names*

### Comparing `v2ray-util-3.9.3/v2ray_util/json_template/client_trojan.json` & `v2ray-util-3.9.4/v2ray_util/json_template/client_trojan.json`

 * *Files identical despite different names*

### Comparing `v2ray-util-3.9.3/v2ray_util/json_template/http.json` & `v2ray-util-3.9.4/v2ray_util/json_template/http.json`

 * *Files identical despite different names*

### Comparing `v2ray-util-3.9.3/v2ray_util/json_template/server.json` & `v2ray-util-3.9.4/v2ray_util/json_template/server.json`

 * *Files identical despite different names*

### Comparing `v2ray-util-3.9.3/v2ray_util/json_template/stats_settings.json` & `v2ray-util-3.9.4/v2ray_util/json_template/stats_settings.json`

 * *Files identical despite different names*

### Comparing `v2ray-util-3.9.3/v2ray_util/locale_i18n/zh_CH/LC_MESSAGES/lang.mo` & `v2ray-util-3.9.4/v2ray_util/locale_i18n/zh_CH/LC_MESSAGES/lang.mo`

 * *Files identical despite different names*

### Comparing `v2ray-util-3.9.3/v2ray_util/main.py` & `v2ray-util-3.9.4/v2ray_util/main.py`

 * *Files identical despite different names*

### Comparing `v2ray-util-3.9.3/v2ray_util/util_core/client.py` & `v2ray-util-3.9.4/v2ray_util/util_core/client.py`

 * *Files identical despite different names*

### Comparing `v2ray-util-3.9.3/v2ray_util/util_core/config.py` & `v2ray-util-3.9.4/v2ray_util/util_core/config.py`

 * *Files identical despite different names*

### Comparing `v2ray-util-3.9.3/v2ray_util/util_core/group.py` & `v2ray-util-3.9.4/v2ray_util/util_core/group.py`

 * *Files identical despite different names*

### Comparing `v2ray-util-3.9.3/v2ray_util/util_core/loader.py` & `v2ray-util-3.9.4/v2ray_util/util_core/loader.py`

 * *Files identical despite different names*

### Comparing `v2ray-util-3.9.3/v2ray_util/util_core/profile.py` & `v2ray-util-3.9.4/v2ray_util/util_core/profile.py`

 * *Files identical despite different names*

### Comparing `v2ray-util-3.9.3/v2ray_util/util_core/selector.py` & `v2ray-util-3.9.4/v2ray_util/util_core/selector.py`

 * *Files identical despite different names*

### Comparing `v2ray-util-3.9.3/v2ray_util/util_core/trans.py` & `v2ray-util-3.9.4/v2ray_util/util_core/trans.py`

 * *Files identical despite different names*

### Comparing `v2ray-util-3.9.3/v2ray_util/util_core/utils.py` & `v2ray-util-3.9.4/v2ray_util/util_core/utils.py`

 * *Files identical despite different names*

### Comparing `v2ray-util-3.9.3/v2ray_util/util_core/v2ray.py` & `v2ray-util-3.9.4/v2ray_util/util_core/v2ray.py`

 * *Files identical despite different names*

### Comparing `v2ray-util-3.9.3/v2ray_util/util_core/writer.py` & `v2ray-util-3.9.4/v2ray_util/util_core/writer.py`

 * *Files 0% similar despite different names*

```diff
@@ -397,15 +397,15 @@
                 self.part_json["streamSettings"].update({"sockopt":sockoptDict})
         self.save()
 
 class ClientWriter(Writer):
     def __init__(self, group_tag = 'A', group_index = 0, client_index = 0):
         super(ClientWriter, self).__init__(group_tag, group_index)
         self.client_index = client_index
-        self.client_str = "clients" if self.part_json["protocol"] == "vmess" else "users"
+        self.client_str = "clients" if self.part_json["protocol"] in ("vmess", "vless") else "users"
 
     def write_aid(self, aid = 32):
         self.part_json["settings"][self.client_str][self.client_index]["alterId"] = int(aid)
         self.save()
 
     def write_uuid(self, new_uuid):
         self.part_json["settings"][self.client_str][self.client_index]["id"] = str(new_uuid)
```

### Comparing `v2ray-util-3.9.3/v2ray_util.egg-info/PKG-INFO` & `v2ray-util-3.9.4/v2ray_util.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: v2ray-util
-Version: 3.9.3
+Version: 3.9.4
 Summary: a tool to manage v2ray config json
 Home-page: https://github.com/Jrohy/multi-v2ray
 Author: Jrohy
 Author-email: euvkzx@gmail.com
 License: GPL
 Description: # multi-v2ray
         V2ray/Xray多用户管理脚本，向导式管理[新增|删除|修改]传输协议
```

### Comparing `v2ray-util-3.9.3/v2ray_util.egg-info/SOURCES.txt` & `v2ray-util-3.9.4/v2ray_util.egg-info/SOURCES.txt`

 * *Files identical despite different names*

