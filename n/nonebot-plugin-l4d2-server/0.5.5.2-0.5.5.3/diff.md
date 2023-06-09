# Comparing `tmp/nonebot_plugin_l4d2_server-0.5.5.2.tar.gz` & `tmp/nonebot_plugin_l4d2_server-0.5.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_l4d2_server-0.5.5.2.tar", max compression
+gzip compressed data, was "nonebot_plugin_l4d2_server-0.5.5.3.tar", max compression
```

## Comparing `nonebot_plugin_l4d2_server-0.5.5.2.tar` & `nonebot_plugin_l4d2_server-0.5.5.3.tar`

### file list

```diff
@@ -1,63 +1,63 @@
--rw-r--r--   0        0        0    35149 2023-06-02 03:01:33.088849 nonebot_plugin_l4d2_server-0.5.5.2/LICENSE
--rw-r--r--   0        0        0    11703 2023-06-02 03:01:33.088849 nonebot_plugin_l4d2_server-0.5.5.2/README.md
--rw-r--r--   0        0        0    17532 2023-06-02 03:01:33.092849 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/__init__.py
--rw-r--r--   0        0        0   158357 2023-06-02 03:01:33.096850 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png
--rw-r--r--   0        0        0   631630 2023-06-02 03:01:33.096850 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png
--rw-r--r--   0        0        0   405369 2023-06-02 03:01:33.100849 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg
--rw-r--r--   0        0        0     1590 2023-06-02 03:01:33.100849 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html
--rw-r--r--   0        0        0   242997 2023-06-02 03:01:33.100849 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png
--rw-r--r--   0        0        0     2135 2023-06-02 03:01:33.100849 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg
--rw-r--r--   0        0        0     6135 2023-06-02 03:01:33.100849 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html
--rw-r--r--   0        0        0     6170 2023-06-02 03:01:33.100849 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html
--rw-r--r--   0        0        0     1523 2023-06-02 03:01:33.100849 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html
--rw-r--r--   0        0        0     5506 2023-06-02 03:01:33.100849 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/l.svg
--rw-r--r--   0        0        0     2408 2023-06-02 03:01:33.100849 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/m.svg
--rw-r--r--   0        0        0     7874 2023-06-02 03:01:33.100849 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/vue.css
--rw-r--r--   0        0        0      486 2023-06-02 03:01:33.100849 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/w.svg
--rw-r--r--   0        0        0     1350 2023-06-02 03:01:33.100849 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/data/img/white.png
--rw-r--r--   0        0        0     8734 2023-06-02 03:01:33.100849 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py
--rw-r--r--   0        0        0     1610 2023-06-02 03:01:33.100849 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py
--rw-r--r--   0        0        0     3010 2023-06-02 03:01:33.100849 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py
--rw-r--r--   0        0        0     1694 2023-06-02 03:01:33.100849 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_anne/server.py
--rw-r--r--   0        0        0      359 2023-06-02 03:01:33.100849 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_anne/startand.py
--rw-r--r--   0        0        0     3252 2023-06-02 03:01:33.100849 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_data/__init__.py
--rw-r--r--   0        0        0      468 2023-06-02 03:01:33.100849 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_data/config.py
--rw-r--r--   0        0        0        0 2023-06-02 03:01:33.100849 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_data/database.py
--rw-r--r--   0        0        0     3232 2023-06-02 03:01:33.100849 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_data/players.py
--rw-r--r--   0        0        0     1295 2023-06-02 03:01:33.100849 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_data/serverip.py
--rw-r--r--   0        0        0     4097 2023-06-02 03:01:33.100849 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_file/__init__.py
--rw-r--r--   0        0        0     1906 2023-06-02 03:01:33.100849 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_file/ayromote.py
--rw-r--r--   0        0        0     1860 2023-06-02 03:01:33.100849 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_file/input_json.py
--rw-r--r--   0        0        0     2688 2023-06-02 03:01:33.100849 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_file/remote.py
--rw-r--r--   0        0        0     4148 2023-06-02 03:01:33.100849 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_image/__init__.py
--rw-r--r--   0        0        0     4007 2023-06-02 03:01:33.100849 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_image/download.py
--rw-r--r--   0        0        0     1038 2023-06-02 03:01:33.100849 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py
--rw-r--r--   0        0        0     9524 2023-06-02 03:01:33.100849 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_image/image.py
--rw-r--r--   0        0        0     1073 2023-06-02 03:01:33.100849 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_image/one.py
--rw-r--r--   0        0        0      936 2023-06-02 03:01:33.100849 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py
--rw-r--r--   0        0        0     3799 2023-06-02 03:01:33.100849 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_image/steam.py
--rw-r--r--   0        0        0     1387 2023-06-02 03:01:33.100849 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py
--rw-r--r--   0        0        0     7415 2023-06-02 03:01:33.100849 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_push/__init__.py
--rw-r--r--   0        0        0     3735 2023-06-02 03:01:33.100849 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py
--rw-r--r--   0        0        0     1157 2023-06-02 03:01:33.104850 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_queries/api.py
--rw-r--r--   0        0        0     1191 2023-06-02 03:01:33.104850 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_queries/ohter.py
--rw-r--r--   0        0        0    10855 2023-06-02 03:01:33.104850 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py
--rw-r--r--   0        0        0     1615 2023-06-02 03:01:33.104850 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_server/__init__.py
--rw-r--r--   0        0        0        0 2023-06-02 03:01:33.104850 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_server/index.py
--rw-r--r--   0        0        0     1248 2023-06-02 03:01:33.104850 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_server/rcon.py
--rw-r--r--   0        0        0     1359 2023-06-02 03:01:33.104850 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_server/workshop.py
--rw-r--r--   0        0        0     4113 2023-06-02 03:01:33.104850 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_update/__init__.py
--rw-r--r--   0        0        0     1175 2023-06-02 03:01:33.104850 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_update/draw_update_log.py
--rw-r--r--   0        0        0     2024 2023-06-02 03:01:33.104850 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_update/restart.py
--rw-r--r--   0        0        0     1417 2023-06-02 03:01:33.104850 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_update/update.py
--rw-r--r--   0        0        0     9724 2023-06-02 03:01:33.104850 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_utils/command.py
--rw-r--r--   0        0        0     6275 2023-06-02 03:01:33.104850 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_utils/config.py
--rw-r--r--   0        0        0     1620 2023-06-02 03:01:33.104850 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_utils/message.py
--rw-r--r--   0        0        0      337 2023-06-02 03:01:33.104850 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_utils/rule.py
--rw-r--r--   0        0        0      992 2023-06-02 03:01:33.104850 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_utils/seach.py
--rw-r--r--   0        0        0     2133 2023-06-02 03:01:33.104850 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_utils/txt_to_img.py
--rw-r--r--   0        0        0     8928 2023-06-02 03:01:33.104850 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_utils/utils.py
--rw-r--r--   0        0        0     8575 2023-06-02 03:01:33.104850 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_web/web.py
--rw-r--r--   0        0        0    14159 2023-06-02 03:01:33.104850 nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_web/webUI.py
--rw-r--r--   0        0        0     1453 2023-06-02 03:01:33.104850 nonebot_plugin_l4d2_server-0.5.5.2/pyproject.toml
--rw-r--r--   0        0        0    13572 1970-01-01 00:00:00.000000 nonebot_plugin_l4d2_server-0.5.5.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-09 11:26:16.190864 nonebot_plugin_l4d2_server-0.5.5.3/LICENSE
+-rw-r--r--   0        0        0    11703 2023-06-09 11:26:16.190864 nonebot_plugin_l4d2_server-0.5.5.3/README.md
+-rw-r--r--   0        0        0    17513 2023-06-09 11:26:16.194865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/__init__.py
+-rw-r--r--   0        0        0   158357 2023-06-09 11:26:16.194865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png
+-rw-r--r--   0        0        0   631630 2023-06-09 11:26:16.194865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png
+-rw-r--r--   0        0        0   405369 2023-06-09 11:26:16.198865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg
+-rw-r--r--   0        0        0     1590 2023-06-09 11:26:16.198865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html
+-rw-r--r--   0        0        0   242997 2023-06-09 11:26:16.198865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png
+-rw-r--r--   0        0        0     2135 2023-06-09 11:26:16.198865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg
+-rw-r--r--   0        0        0     6135 2023-06-09 11:26:16.198865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html
+-rw-r--r--   0        0        0     6170 2023-06-09 11:26:16.198865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html
+-rw-r--r--   0        0        0     1523 2023-06-09 11:26:16.198865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html
+-rw-r--r--   0        0        0     5506 2023-06-09 11:26:16.198865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/l.svg
+-rw-r--r--   0        0        0     2408 2023-06-09 11:26:16.198865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/m.svg
+-rw-r--r--   0        0        0     7874 2023-06-09 11:26:16.198865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/vue.css
+-rw-r--r--   0        0        0      486 2023-06-09 11:26:16.198865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/w.svg
+-rw-r--r--   0        0        0     1350 2023-06-09 11:26:16.198865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/data/img/white.png
+-rw-r--r--   0        0        0     8734 2023-06-09 11:26:16.198865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py
+-rw-r--r--   0        0        0     1610 2023-06-09 11:26:16.198865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py
+-rw-r--r--   0        0        0     3010 2023-06-09 11:26:16.198865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py
+-rw-r--r--   0        0        0     1694 2023-06-09 11:26:16.198865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_anne/server.py
+-rw-r--r--   0        0        0      359 2023-06-09 11:26:16.198865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_anne/startand.py
+-rw-r--r--   0        0        0     3252 2023-06-09 11:26:16.198865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_data/__init__.py
+-rw-r--r--   0        0        0      468 2023-06-09 11:26:16.198865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_data/config.py
+-rw-r--r--   0        0        0        0 2023-06-09 11:26:16.198865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_data/database.py
+-rw-r--r--   0        0        0     3232 2023-06-09 11:26:16.198865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_data/players.py
+-rw-r--r--   0        0        0     1295 2023-06-09 11:26:16.198865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_data/serverip.py
+-rw-r--r--   0        0        0     4097 2023-06-09 11:26:16.198865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_file/__init__.py
+-rw-r--r--   0        0        0     1906 2023-06-09 11:26:16.198865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_file/ayromote.py
+-rw-r--r--   0        0        0     1860 2023-06-09 11:26:16.198865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_file/input_json.py
+-rw-r--r--   0        0        0     2688 2023-06-09 11:26:16.198865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_file/remote.py
+-rw-r--r--   0        0        0     4148 2023-06-09 11:26:16.198865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_image/__init__.py
+-rw-r--r--   0        0        0     4007 2023-06-09 11:26:16.198865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_image/download.py
+-rw-r--r--   0        0        0     1038 2023-06-09 11:26:16.198865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py
+-rw-r--r--   0        0        0     9524 2023-06-09 11:26:16.202865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_image/image.py
+-rw-r--r--   0        0        0     1073 2023-06-09 11:26:16.202865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_image/one.py
+-rw-r--r--   0        0        0      936 2023-06-09 11:26:16.202865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py
+-rw-r--r--   0        0        0     3799 2023-06-09 11:26:16.202865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_image/steam.py
+-rw-r--r--   0        0        0     1387 2023-06-09 11:26:16.202865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py
+-rw-r--r--   0        0        0     7415 2023-06-09 11:26:16.202865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_push/__init__.py
+-rw-r--r--   0        0        0     3735 2023-06-09 11:26:16.202865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py
+-rw-r--r--   0        0        0     1157 2023-06-09 11:26:16.202865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_queries/api.py
+-rw-r--r--   0        0        0     1191 2023-06-09 11:26:16.202865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_queries/ohter.py
+-rw-r--r--   0        0        0    10855 2023-06-09 11:26:16.202865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py
+-rw-r--r--   0        0        0     1615 2023-06-09 11:26:16.202865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_server/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-09 11:26:16.202865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_server/index.py
+-rw-r--r--   0        0        0     1248 2023-06-09 11:26:16.202865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_server/rcon.py
+-rw-r--r--   0        0        0     1359 2023-06-09 11:26:16.202865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_server/workshop.py
+-rw-r--r--   0        0        0     4113 2023-06-09 11:26:16.202865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_update/__init__.py
+-rw-r--r--   0        0        0     1175 2023-06-09 11:26:16.202865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_update/draw_update_log.py
+-rw-r--r--   0        0        0     2024 2023-06-09 11:26:16.202865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_update/restart.py
+-rw-r--r--   0        0        0     1417 2023-06-09 11:26:16.202865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_update/update.py
+-rw-r--r--   0        0        0     9728 2023-06-09 11:26:16.202865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_utils/command.py
+-rw-r--r--   0        0        0     6275 2023-06-09 11:26:16.202865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_utils/config.py
+-rw-r--r--   0        0        0     1620 2023-06-09 11:26:16.202865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_utils/message.py
+-rw-r--r--   0        0        0      337 2023-06-09 11:26:16.202865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_utils/rule.py
+-rw-r--r--   0        0        0      992 2023-06-09 11:26:16.202865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_utils/seach.py
+-rw-r--r--   0        0        0     2133 2023-06-09 11:26:16.202865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_utils/txt_to_img.py
+-rw-r--r--   0        0        0     8928 2023-06-09 11:26:16.202865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_utils/utils.py
+-rw-r--r--   0        0        0     8575 2023-06-09 11:26:16.202865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_web/web.py
+-rw-r--r--   0        0        0    14159 2023-06-09 11:26:16.202865 nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_web/webUI.py
+-rw-r--r--   0        0        0     1453 2023-06-09 11:26:16.202865 nonebot_plugin_l4d2_server-0.5.5.3/pyproject.toml
+-rw-r--r--   0        0        0    13572 1970-01-01 00:00:00.000000 nonebot_plugin_l4d2_server-0.5.5.3/PKG-INFO
```

### Comparing `nonebot_plugin_l4d2_server-0.5.5.2/LICENSE` & `nonebot_plugin_l4d2_server-0.5.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.2/README.md` & `nonebot_plugin_l4d2_server-0.5.5.3/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/__init__.py` & `nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -66,18 +66,16 @@
         matcher.set_arg('txt',args)
         return
     l4_file_path = l4_config.l4_ipall[CHECK_FILE]['location']
     map_path = Path(l4_file_path, vpk_path)
     # 检查下载路径是否存在
     if not Path(l4_file_path).exists():
         await matcher.finish("你填写的路径不存在辣")
-        return
     if not Path(map_path).exists():
         await matcher.finish("这个路径并不是求生服务器的路径，请再看看罢")
-        return
     url:str = args['file']['url']
     name: str = args['file']['name']
     # 如果不符合格式则忽略
     await up.send('已收到文件，开始下载')
     sleep(1)   # 等待一秒防止因为文件名获取出现BUG
     vpk_files = await updown_l4d2_vpk(map_path,name,url)
     if vpk_files:
@@ -87,31 +85,34 @@
         await matcher.finish("你可能上传了相同的文件，或者解压失败了捏")
 
 
 
 @up.got("is_sure", prompt="请选择上传位置（输入阿拉伯数字)")    
 async def _(matcher: Matcher):
     args = matcher.get_arg('txt')
-    l4_file = l4_config.l4_ipall[CHECK_FILE]['location']
+    l4_file = l4_config.l4_ipall
     if not args:
         await matcher.finish('获取文件出错辣，再试一次吧')
 
     is_sure = str(matcher.get_arg('is_sure')).strip()
     if not is_sure.isdigit():
         await matcher.finish('已取消上传')
-    file_number = len(l4_file)
-    is_sure = int(is_sure)
-    if is_sure > file_number or is_sure <= 0:
-        await matcher.finish('没有该序号')
-    l4_file_path = l4_file[is_sure - 1]
+    
+    file_path:str = ''
+    for one_server in l4_file:
+        if one_server['id_rank'] == is_sure:
+            file_path = one_server['location']
+    if not file_path:
+        await matcher.finish("没有这个序号拉baka")
 
-    map_path = Path(l4_file_path, vpk_path)
+
+    map_path = Path(file_path, vpk_path)
 
     # 检查下载路径是否存在
-    if not Path(l4_file_path).exists():
+    if not Path(file_path).exists():
         await matcher.finish("你填写的路径不存在辣")
     if not map_path.exists():
         await matcher.finish("这个路径并不是求生服务器的路径，请再看看罢")
 
     url = args['file']['url']
     name = args['file']['name']
     # 如果不符合格式则忽略
```

### Comparing `nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png` & `nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png` & `nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg` & `nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html` & `nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png` & `nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg` & `nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html` & `nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html` & `nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html` & `nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/l.svg` & `nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/l.svg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/m.svg` & `nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/m.svg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/vue.css` & `nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/vue.css`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/data/img/white.png` & `nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/data/img/white.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py` & `nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py` & `nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py` & `nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_anne/server.py` & `nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_anne/server.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_data/__init__.py` & `nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_data/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_data/players.py` & `nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_data/players.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_data/serverip.py` & `nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_data/serverip.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_file/__init__.py` & `nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_file/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_file/ayromote.py` & `nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_file/ayromote.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_file/input_json.py` & `nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_file/input_json.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_file/remote.py` & `nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_file/remote.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_image/__init__.py` & `nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_image/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_image/download.py` & `nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_image/download.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py` & `nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_image/image.py` & `nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_image/image.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_image/one.py` & `nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_image/one.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py` & `nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_image/steam.py` & `nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_image/steam.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py` & `nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_push/__init__.py` & `nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_push/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py` & `nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_queries/api.py` & `nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_queries/api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_queries/ohter.py` & `nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_queries/ohter.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py` & `nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_server/__init__.py` & `nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_server/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_server/rcon.py` & `nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_server/rcon.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_server/workshop.py` & `nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_server/workshop.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_update/__init__.py` & `nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_update/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_update/draw_update_log.py` & `nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_update/draw_update_log.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_update/restart.py` & `nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_update/restart.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_update/update.py` & `nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_update/update.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_utils/command.py` & `nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_utils/command.py`

 * *Files 2% similar despite different names*

```diff
@@ -235,22 +235,22 @@
         if len(message) == 0:
             # 关键词不匹配，忽略
             return
         ip = str(message['ip'])
         logger.info(ip)
         
         try:
-            if l4_config.l4_image:
-                host,port = split_maohao(ip)
-                msgs = await queries_dict(host,port)
-                msgs['Players'] += await player_queries_anne_dict(host,port)
-                imgs = await one_server_img()
-            else:
-                msgs = await get_anne_server_ip(ip)
-                return  msgs
+        #     if l4_config.l4_image:
+        #         host,port = split_maohao(ip)
+        #         msgs = await queries_dict(host,port)
+        #         msgs['Players'] += await player_queries_anne_dict(host,port)
+        #         imgs = await one_server_img()
+            # else:
+            msgs = await get_anne_server_ip(ip)
+            return  msgs
         except (OSError,asyncio.exceptions.TimeoutError):
             return '服务器无响应'
```

### Comparing `nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_utils/config.py` & `nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_utils/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_utils/message.py` & `nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_utils/message.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_utils/seach.py` & `nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_utils/seach.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_utils/txt_to_img.py` & `nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_utils/txt_to_img.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_utils/utils.py` & `nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_utils/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_web/web.py` & `nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_web/web.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.2/nonebot_plugin_l4d2_server/l4d2_web/webUI.py` & `nonebot_plugin_l4d2_server-0.5.5.3/nonebot_plugin_l4d2_server/l4d2_web/webUI.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.5.2/pyproject.toml` & `nonebot_plugin_l4d2_server-0.5.5.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-l4d2-server"
-version = "0.5.5.2"
+version = "0.5.5.3"
 description = "L4D2 server related operations plugin for NoneBot2"
 authors = ["Agnes_Digital <Z735803792@163.com>"]
 license = "GPLv3"
 readme = "README.md"
 homepage = "https://github.com/Agnes4m/nonebot_plugin_l4d2_server"
 repository = "https://github.com/Agnes4m/nonebot_plugin_l4d2_server"
 keywords = ["steam", "game", "l4d2", "nonebot2", "plugin"]
```

### Comparing `nonebot_plugin_l4d2_server-0.5.5.2/PKG-INFO` & `nonebot_plugin_l4d2_server-0.5.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-l4d2-server
-Version: 0.5.5.2
+Version: 0.5.5.3
 Summary: L4D2 server related operations plugin for NoneBot2
 Home-page: https://github.com/Agnes4m/nonebot_plugin_l4d2_server
 License: GPLv3
 Keywords: steam,game,l4d2,nonebot2,plugin
 Author: Agnes_Digital
 Author-email: Z735803792@163.com
 Requires-Python: >=3.9,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-l4d2-server Version: 0.5.5.2
+Metadata-Version: 2.1 Name: nonebot-plugin-l4d2-server Version: 0.5.5.3
 Summary: L4D2 server related operations plugin for NoneBot2 Home-page: https://
 github.com/Agnes4m/nonebot_plugin_l4d2_server License: GPLv3 Keywords:
 steam,game,l4d2,nonebot2,plugin Author: Agnes_Digital Author-email:
 Z735803792@163.com Requires-Python: >=3.9,<4.0 Classifier: License :: OSI
 Approved :: GNU General Public License v3 (GPLv3) Classifier: License :: Other/
 Proprietary License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
```

