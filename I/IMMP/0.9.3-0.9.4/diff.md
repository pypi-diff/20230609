# Comparing `tmp/IMMP-0.9.3.tar.gz` & `tmp/IMMP-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/IMMP-0.9.3.tar", last modified: Sat Dec 19 14:40:14 2020, max compression
+gzip compressed data, was "dist/IMMP-0.9.4.tar", last modified: Fri Dec 25 20:28:44 2020, max compression
```

## Comparing `IMMP-0.9.3.tar` & `IMMP-0.9.4.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2020-12-19 14:40:14.000000 IMMP-0.9.3/
--rw-r--r--   0 user      (1000) user      (1000)     3024 2020-12-19 14:40:14.000000 IMMP-0.9.3/PKG-INFO
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2020-12-19 14:40:14.000000 IMMP-0.9.3/IMMP.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)     3024 2020-12-19 14:40:14.000000 IMMP-0.9.3/IMMP.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)       51 2020-12-19 14:40:14.000000 IMMP-0.9.3/IMMP.egg-info/entry_points.txt
--rw-r--r--   0 user      (1000) user      (1000)      421 2020-12-19 14:40:14.000000 IMMP-0.9.3/IMMP.egg-info/requires.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2020-12-19 14:40:14.000000 IMMP-0.9.3/IMMP.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) user      (1000)        5 2020-12-19 14:40:14.000000 IMMP-0.9.3/IMMP.egg-info/top_level.txt
--rw-r--r--   0 user      (1000) user      (1000)     1346 2020-12-19 14:40:14.000000 IMMP-0.9.3/IMMP.egg-info/SOURCES.txt
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2020-12-19 14:40:14.000000 IMMP-0.9.3/bin/
--rwxr-xr-x   0 user      (1000) user      (1000)    21137 2020-11-08 11:43:25.000000 IMMP-0.9.3/bin/immp-migrate-hangoutsbot.py
--rw-r--r--   0 user      (1000) user      (1000)     1947 2020-12-16 17:44:45.000000 IMMP-0.9.3/setup.py
--rw-r--r--   0 user      (1000) user      (1000)       38 2020-12-19 14:40:14.000000 IMMP-0.9.3/setup.cfg
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2020-12-19 14:40:14.000000 IMMP-0.9.3/immp/
--rw-r--r--   0 user      (1000) user      (1000)      708 2020-08-18 17:22:30.000000 IMMP-0.9.3/immp/__init__.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2020-12-19 14:40:14.000000 IMMP-0.9.3/immp/core/
--rw-r--r--   0 user      (1000) user      (1000)     4848 2020-08-18 17:22:30.000000 IMMP-0.9.3/immp/core/stream.py
--rw-r--r--   0 user      (1000) user      (1000)    23207 2020-08-18 17:14:12.000000 IMMP-0.9.3/immp/core/schema.py
--rw-r--r--   0 user      (1000) user      (1000)        0 2018-06-18 06:54:24.000000 IMMP-0.9.3/immp/core/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)      270 2018-11-23 19:45:53.000000 IMMP-0.9.3/immp/core/error.py
--rw-r--r--   0 user      (1000) user      (1000)     5752 2020-11-08 11:43:25.000000 IMMP-0.9.3/immp/core/channel.py
--rw-r--r--   0 user      (1000) user      (1000)    17839 2020-12-16 17:44:05.000000 IMMP-0.9.3/immp/core/host.py
--rw-r--r--   0 user      (1000) user      (1000)     5222 2020-08-18 17:22:30.000000 IMMP-0.9.3/immp/core/hook.py
--rw-r--r--   0 user      (1000) user      (1000)    14605 2020-08-18 17:22:30.000000 IMMP-0.9.3/immp/core/plug.py
--rw-r--r--   0 user      (1000) user      (1000)    33018 2020-12-09 17:27:38.000000 IMMP-0.9.3/immp/core/message.py
--rw-r--r--   0 user      (1000) user      (1000)    16053 2020-12-16 17:44:01.000000 IMMP-0.9.3/immp/core/util.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2020-12-19 14:40:14.000000 IMMP-0.9.3/immp/plug/
--rw-r--r--   0 user      (1000) user      (1000)     1769 2020-08-18 17:14:12.000000 IMMP-0.9.3/immp/plug/dummy.py
--rw-r--r--   0 user      (1000) user      (1000)    28127 2020-11-08 11:43:25.000000 IMMP-0.9.3/immp/plug/irc.py
--rw-r--r--   0 user      (1000) user      (1000)    27886 2020-12-09 17:27:38.000000 IMMP-0.9.3/immp/plug/discord.py
--rw-r--r--   0 user      (1000) user      (1000)    32274 2020-11-08 11:43:25.000000 IMMP-0.9.3/immp/plug/hangouts.py
--rw-r--r--   0 user      (1000) user      (1000)    47564 2020-12-16 17:44:23.000000 IMMP-0.9.3/immp/plug/slack.py
--rw-r--r--   0 user      (1000) user      (1000)    69053 2020-12-16 17:44:25.000000 IMMP-0.9.3/immp/plug/telegram.py
--rw-r--r--   0 user      (1000) user      (1000)    11829 2020-11-08 11:43:25.000000 IMMP-0.9.3/immp/plug/github.py
--rw-r--r--   0 user      (1000) user      (1000)      559 2020-12-09 17:27:38.000000 IMMP-0.9.3/immp/__main__.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2020-12-19 14:40:14.000000 IMMP-0.9.3/immp/hook/
--rw-r--r--   0 user      (1000) user      (1000)    16393 2020-12-16 17:44:05.000000 IMMP-0.9.3/immp/hook/alerts.py
--rw-r--r--   0 user      (1000) user      (1000)    12080 2020-12-11 17:36:04.000000 IMMP-0.9.3/immp/hook/identitylocal.py
--rw-r--r--   0 user      (1000) user      (1000)    35318 2020-12-16 17:44:05.000000 IMMP-0.9.3/immp/hook/sync.py
--rw-r--r--   0 user      (1000) user      (1000)    24473 2020-12-16 17:44:05.000000 IMMP-0.9.3/immp/hook/command.py
--rw-r--r--   0 user      (1000) user      (1000)     7150 2020-11-08 11:57:21.000000 IMMP-0.9.3/immp/hook/notes.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2020-12-19 14:40:14.000000 IMMP-0.9.3/immp/hook/webui/
--rw-r--r--   0 user      (1000) user      (1000)    19605 2020-12-16 17:44:10.000000 IMMP-0.9.3/immp/hook/webui/__init__.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2020-12-19 14:40:14.000000 IMMP-0.9.3/immp/hook/webui/templates/
--rw-r--r--   0 user      (1000) user      (1000)     4483 2020-08-18 17:14:12.000000 IMMP-0.9.3/immp/hook/webui/templates/main.j2
--rw-r--r--   0 user      (1000) user      (1000)     1569 2020-08-18 17:14:12.000000 IMMP-0.9.3/immp/hook/webui/templates/group.j2
--rw-r--r--   0 user      (1000) user      (1000)     2845 2020-12-16 17:44:10.000000 IMMP-0.9.3/immp/hook/webui/templates/add.j2
--rw-r--r--   0 user      (1000) user      (1000)     5274 2020-08-18 17:14:12.000000 IMMP-0.9.3/immp/hook/webui/templates/plug.j2
--rw-r--r--   0 user      (1000) user      (1000)      861 2018-12-24 13:56:07.000000 IMMP-0.9.3/immp/hook/webui/templates/hook_remove.j2
--rw-r--r--   0 user      (1000) user      (1000)     4522 2020-08-18 17:14:12.000000 IMMP-0.9.3/immp/hook/webui/templates/channel.j2
--rw-r--r--   0 user      (1000) user      (1000)     1125 2018-12-24 13:56:07.000000 IMMP-0.9.3/immp/hook/webui/templates/plug_remove.j2
--rw-r--r--   0 user      (1000) user      (1000)     2485 2020-08-18 17:14:12.000000 IMMP-0.9.3/immp/hook/webui/templates/plug_channels.j2
--rw-r--r--   0 user      (1000) user      (1000)     3720 2020-08-18 17:14:12.000000 IMMP-0.9.3/immp/hook/webui/templates/hook.j2
--rw-r--r--   0 user      (1000) user      (1000)     3425 2020-08-18 17:14:12.000000 IMMP-0.9.3/immp/hook/webui/templates/base.j2
--rw-r--r--   0 user      (1000) user      (1000)      566 2020-08-18 17:14:12.000000 IMMP-0.9.3/immp/hook/webui/templates/macros.j2
--rw-r--r--   0 user      (1000) user      (1000)     5951 2020-11-08 11:43:25.000000 IMMP-0.9.3/immp/hook/identity.py
--rw-r--r--   0 user      (1000) user      (1000)     2985 2020-11-08 11:43:25.000000 IMMP-0.9.3/immp/hook/autorespond.py
--rw-r--r--   0 user      (1000) user      (1000)     5958 2020-08-18 17:14:12.000000 IMMP-0.9.3/immp/hook/shell.py
--rw-r--r--   0 user      (1000) user      (1000)     8298 2020-12-16 17:44:10.000000 IMMP-0.9.3/immp/hook/web.py
--rw-r--r--   0 user      (1000) user      (1000)     4198 2020-11-08 11:43:25.000000 IMMP-0.9.3/immp/hook/access.py
--rw-r--r--   0 user      (1000) user      (1000)      728 2020-08-18 17:14:12.000000 IMMP-0.9.3/immp/hook/textcommand.py
--rw-r--r--   0 user      (1000) user      (1000)     6731 2020-12-16 17:44:05.000000 IMMP-0.9.3/immp/hook/runner.py
--rw-r--r--   0 user      (1000) user      (1000)     4718 2020-11-08 11:43:25.000000 IMMP-0.9.3/immp/hook/database.py
--rw-r--r--   0 user      (1000) user      (1000)     2897 2020-08-18 17:14:12.000000 IMMP-0.9.3/immp/hook/hangoutslock.py
--rw-r--r--   0 user      (1000) user      (1000)     2114 2020-08-18 17:14:12.000000 IMMP-0.9.3/immp/hook/discordrole.py
--rw-r--r--   0 user      (1000) user      (1000)     1774 2020-08-18 17:14:12.000000 IMMP-0.9.3/README.rst
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2020-12-25 20:28:44.000000 IMMP-0.9.4/
+-rw-r--r--   0 user      (1000) user      (1000)     3024 2020-12-25 20:28:44.000000 IMMP-0.9.4/PKG-INFO
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2020-12-25 20:28:44.000000 IMMP-0.9.4/IMMP.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)     3024 2020-12-25 20:28:44.000000 IMMP-0.9.4/IMMP.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)       51 2020-12-25 20:28:44.000000 IMMP-0.9.4/IMMP.egg-info/entry_points.txt
+-rw-r--r--   0 user      (1000) user      (1000)      421 2020-12-25 20:28:44.000000 IMMP-0.9.4/IMMP.egg-info/requires.txt
+-rw-r--r--   0 user      (1000) user      (1000)        1 2020-12-25 20:28:44.000000 IMMP-0.9.4/IMMP.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1000) user      (1000)        5 2020-12-25 20:28:44.000000 IMMP-0.9.4/IMMP.egg-info/top_level.txt
+-rw-r--r--   0 user      (1000) user      (1000)     1346 2020-12-25 20:28:44.000000 IMMP-0.9.4/IMMP.egg-info/SOURCES.txt
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2020-12-25 20:28:44.000000 IMMP-0.9.4/bin/
+-rwxr-xr-x   0 user      (1000) user      (1000)    21137 2020-11-08 11:43:25.000000 IMMP-0.9.4/bin/immp-migrate-hangoutsbot.py
+-rw-r--r--   0 user      (1000) user      (1000)     1947 2020-12-25 20:28:35.000000 IMMP-0.9.4/setup.py
+-rw-r--r--   0 user      (1000) user      (1000)       38 2020-12-25 20:28:44.000000 IMMP-0.9.4/setup.cfg
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2020-12-25 20:28:44.000000 IMMP-0.9.4/immp/
+-rw-r--r--   0 user      (1000) user      (1000)      708 2020-08-18 17:22:30.000000 IMMP-0.9.4/immp/__init__.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2020-12-25 20:28:44.000000 IMMP-0.9.4/immp/core/
+-rw-r--r--   0 user      (1000) user      (1000)     4848 2020-08-18 17:22:30.000000 IMMP-0.9.4/immp/core/stream.py
+-rw-r--r--   0 user      (1000) user      (1000)    23207 2020-08-18 17:14:12.000000 IMMP-0.9.4/immp/core/schema.py
+-rw-r--r--   0 user      (1000) user      (1000)        0 2018-06-18 06:54:24.000000 IMMP-0.9.4/immp/core/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)      270 2018-11-23 19:45:53.000000 IMMP-0.9.4/immp/core/error.py
+-rw-r--r--   0 user      (1000) user      (1000)     5752 2020-12-25 20:28:26.000000 IMMP-0.9.4/immp/core/channel.py
+-rw-r--r--   0 user      (1000) user      (1000)    17839 2020-12-25 20:17:54.000000 IMMP-0.9.4/immp/core/host.py
+-rw-r--r--   0 user      (1000) user      (1000)     5222 2020-08-18 17:22:30.000000 IMMP-0.9.4/immp/core/hook.py
+-rw-r--r--   0 user      (1000) user      (1000)    14605 2020-12-25 20:28:26.000000 IMMP-0.9.4/immp/core/plug.py
+-rw-r--r--   0 user      (1000) user      (1000)    33018 2020-12-09 17:27:38.000000 IMMP-0.9.4/immp/core/message.py
+-rw-r--r--   0 user      (1000) user      (1000)    16053 2020-12-25 20:13:28.000000 IMMP-0.9.4/immp/core/util.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2020-12-25 20:28:44.000000 IMMP-0.9.4/immp/plug/
+-rw-r--r--   0 user      (1000) user      (1000)     1769 2020-12-25 20:28:26.000000 IMMP-0.9.4/immp/plug/dummy.py
+-rw-r--r--   0 user      (1000) user      (1000)    28127 2020-12-25 20:28:26.000000 IMMP-0.9.4/immp/plug/irc.py
+-rw-r--r--   0 user      (1000) user      (1000)    27886 2020-12-25 20:28:26.000000 IMMP-0.9.4/immp/plug/discord.py
+-rw-r--r--   0 user      (1000) user      (1000)    32274 2020-12-25 20:28:26.000000 IMMP-0.9.4/immp/plug/hangouts.py
+-rw-r--r--   0 user      (1000) user      (1000)    47564 2020-12-25 20:28:26.000000 IMMP-0.9.4/immp/plug/slack.py
+-rw-r--r--   0 user      (1000) user      (1000)    69053 2020-12-25 20:28:26.000000 IMMP-0.9.4/immp/plug/telegram.py
+-rw-r--r--   0 user      (1000) user      (1000)    11829 2020-12-25 20:14:30.000000 IMMP-0.9.4/immp/plug/github.py
+-rw-r--r--   0 user      (1000) user      (1000)      559 2020-12-09 17:27:38.000000 IMMP-0.9.4/immp/__main__.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2020-12-25 20:28:44.000000 IMMP-0.9.4/immp/hook/
+-rw-r--r--   0 user      (1000) user      (1000)    16393 2020-12-25 20:17:54.000000 IMMP-0.9.4/immp/hook/alerts.py
+-rw-r--r--   0 user      (1000) user      (1000)    12080 2020-12-11 17:36:04.000000 IMMP-0.9.4/immp/hook/identitylocal.py
+-rw-r--r--   0 user      (1000) user      (1000)    35318 2020-12-25 20:28:26.000000 IMMP-0.9.4/immp/hook/sync.py
+-rw-r--r--   0 user      (1000) user      (1000)    24473 2020-12-25 20:17:54.000000 IMMP-0.9.4/immp/hook/command.py
+-rw-r--r--   0 user      (1000) user      (1000)     7150 2020-11-08 11:57:21.000000 IMMP-0.9.4/immp/hook/notes.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2020-12-25 20:28:44.000000 IMMP-0.9.4/immp/hook/webui/
+-rw-r--r--   0 user      (1000) user      (1000)    19605 2020-12-25 20:13:32.000000 IMMP-0.9.4/immp/hook/webui/__init__.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2020-12-25 20:28:44.000000 IMMP-0.9.4/immp/hook/webui/templates/
+-rw-r--r--   0 user      (1000) user      (1000)     4483 2020-08-18 17:14:12.000000 IMMP-0.9.4/immp/hook/webui/templates/main.j2
+-rw-r--r--   0 user      (1000) user      (1000)     1569 2020-08-18 17:14:12.000000 IMMP-0.9.4/immp/hook/webui/templates/group.j2
+-rw-r--r--   0 user      (1000) user      (1000)     2845 2020-12-25 20:13:32.000000 IMMP-0.9.4/immp/hook/webui/templates/add.j2
+-rw-r--r--   0 user      (1000) user      (1000)     5274 2020-08-18 17:14:12.000000 IMMP-0.9.4/immp/hook/webui/templates/plug.j2
+-rw-r--r--   0 user      (1000) user      (1000)      861 2018-12-24 13:56:07.000000 IMMP-0.9.4/immp/hook/webui/templates/hook_remove.j2
+-rw-r--r--   0 user      (1000) user      (1000)     4522 2020-08-18 17:14:12.000000 IMMP-0.9.4/immp/hook/webui/templates/channel.j2
+-rw-r--r--   0 user      (1000) user      (1000)     1125 2018-12-24 13:56:07.000000 IMMP-0.9.4/immp/hook/webui/templates/plug_remove.j2
+-rw-r--r--   0 user      (1000) user      (1000)     2485 2020-08-18 17:14:12.000000 IMMP-0.9.4/immp/hook/webui/templates/plug_channels.j2
+-rw-r--r--   0 user      (1000) user      (1000)     3720 2020-08-18 17:14:12.000000 IMMP-0.9.4/immp/hook/webui/templates/hook.j2
+-rw-r--r--   0 user      (1000) user      (1000)     3425 2020-08-18 17:14:12.000000 IMMP-0.9.4/immp/hook/webui/templates/base.j2
+-rw-r--r--   0 user      (1000) user      (1000)      566 2020-08-18 17:14:12.000000 IMMP-0.9.4/immp/hook/webui/templates/macros.j2
+-rw-r--r--   0 user      (1000) user      (1000)     5951 2020-11-08 11:43:25.000000 IMMP-0.9.4/immp/hook/identity.py
+-rw-r--r--   0 user      (1000) user      (1000)     2985 2020-12-25 20:28:26.000000 IMMP-0.9.4/immp/hook/autorespond.py
+-rw-r--r--   0 user      (1000) user      (1000)     5958 2020-08-18 17:14:12.000000 IMMP-0.9.4/immp/hook/shell.py
+-rw-r--r--   0 user      (1000) user      (1000)     8298 2020-12-25 20:13:32.000000 IMMP-0.9.4/immp/hook/web.py
+-rw-r--r--   0 user      (1000) user      (1000)     4198 2020-11-08 11:43:25.000000 IMMP-0.9.4/immp/hook/access.py
+-rw-r--r--   0 user      (1000) user      (1000)      728 2020-08-18 17:14:12.000000 IMMP-0.9.4/immp/hook/textcommand.py
+-rw-r--r--   0 user      (1000) user      (1000)     6731 2020-12-25 20:17:54.000000 IMMP-0.9.4/immp/hook/runner.py
+-rw-r--r--   0 user      (1000) user      (1000)     4718 2020-11-08 11:43:25.000000 IMMP-0.9.4/immp/hook/database.py
+-rw-r--r--   0 user      (1000) user      (1000)     2897 2020-08-18 17:14:12.000000 IMMP-0.9.4/immp/hook/hangoutslock.py
+-rw-r--r--   0 user      (1000) user      (1000)     2114 2020-08-18 17:14:12.000000 IMMP-0.9.4/immp/hook/discordrole.py
+-rw-r--r--   0 user      (1000) user      (1000)     1774 2020-08-18 17:14:12.000000 IMMP-0.9.4/README.rst
```

### Comparing `IMMP-0.9.3/PKG-INFO` & `IMMP-0.9.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IMMP
-Version: 0.9.3
+Version: 0.9.4
 Summary: A modular processing platform for instant messages.
 Home-page: https://immp.t.allofti.me
 Author: Terrance
 Author-email: immp@terrance.allofti.me
 License: BSD 3-Clause License
 Description: IMMP
         ====
@@ -78,16 +78,16 @@
 Platform: Any
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Communications :: Chat
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
-Provides-Extra: console
-Provides-Extra: discord
 Provides-Extra: sync
+Provides-Extra: uv
+Provides-Extra: runner
 Provides-Extra: telegram
-Provides-Extra: web
 Provides-Extra: hangouts
-Provides-Extra: runner
-Provides-Extra: uv
 Provides-Extra: db
+Provides-Extra: console
+Provides-Extra: discord
+Provides-Extra: web
```

### Comparing `IMMP-0.9.3/IMMP.egg-info/PKG-INFO` & `IMMP-0.9.4/IMMP.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IMMP
-Version: 0.9.3
+Version: 0.9.4
 Summary: A modular processing platform for instant messages.
 Home-page: https://immp.t.allofti.me
 Author: Terrance
 Author-email: immp@terrance.allofti.me
 License: BSD 3-Clause License
 Description: IMMP
         ====
@@ -78,16 +78,16 @@
 Platform: Any
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Communications :: Chat
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
-Provides-Extra: console
-Provides-Extra: discord
 Provides-Extra: sync
+Provides-Extra: uv
+Provides-Extra: runner
 Provides-Extra: telegram
-Provides-Extra: web
 Provides-Extra: hangouts
-Provides-Extra: runner
-Provides-Extra: uv
 Provides-Extra: db
+Provides-Extra: console
+Provides-Extra: discord
+Provides-Extra: web
```

### Comparing `IMMP-0.9.3/IMMP.egg-info/SOURCES.txt` & `IMMP-0.9.4/IMMP.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `IMMP-0.9.3/bin/immp-migrate-hangoutsbot.py` & `IMMP-0.9.4/bin/immp-migrate-hangoutsbot.py`

 * *Files identical despite different names*

### Comparing `IMMP-0.9.3/setup.py` & `IMMP-0.9.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import setup
 
 
 README = os.path.join(os.path.abspath(os.path.dirname(__file__)), "README.rst")
 
 setup(name="IMMP",
-      version="0.9.3",
+      version="0.9.4",
       author="Terrance",
       author_email="immp@terrance.allofti.me",
       url="https://immp.t.allofti.me",
       description="A modular processing platform for instant messages.",
       long_description=open(README).read(),
       long_description_content_type="text/x-rst",
       license="BSD 3-Clause License",
```

### Comparing `IMMP-0.9.3/immp/__init__.py` & `IMMP-0.9.4/immp/__init__.py`

 * *Files identical despite different names*

### Comparing `IMMP-0.9.3/immp/core/stream.py` & `IMMP-0.9.4/immp/core/stream.py`

 * *Files identical despite different names*

### Comparing `IMMP-0.9.3/immp/core/schema.py` & `IMMP-0.9.4/immp/core/schema.py`

 * *Files identical despite different names*

### Comparing `IMMP-0.9.3/immp/core/channel.py` & `IMMP-0.9.4/immp/core/channel.py`

 * *Files identical despite different names*

### Comparing `IMMP-0.9.3/immp/core/host.py` & `IMMP-0.9.4/immp/core/host.py`

 * *Files identical despite different names*

### Comparing `IMMP-0.9.3/immp/core/hook.py` & `IMMP-0.9.4/immp/core/hook.py`

 * *Files identical despite different names*

### Comparing `IMMP-0.9.3/immp/core/plug.py` & `IMMP-0.9.4/immp/core/plug.py`

 * *Files identical despite different names*

### Comparing `IMMP-0.9.3/immp/core/message.py` & `IMMP-0.9.4/immp/core/message.py`

 * *Files identical despite different names*

### Comparing `IMMP-0.9.3/immp/core/util.py` & `IMMP-0.9.4/immp/core/util.py`

 * *Files identical despite different names*

### Comparing `IMMP-0.9.3/immp/plug/dummy.py` & `IMMP-0.9.4/immp/plug/dummy.py`

 * *Files identical despite different names*

### Comparing `IMMP-0.9.3/immp/plug/irc.py` & `IMMP-0.9.4/immp/plug/irc.py`

 * *Files identical despite different names*

### Comparing `IMMP-0.9.3/immp/plug/discord.py` & `IMMP-0.9.4/immp/plug/discord.py`

 * *Files identical despite different names*

### Comparing `IMMP-0.9.3/immp/plug/hangouts.py` & `IMMP-0.9.4/immp/plug/hangouts.py`

 * *Files identical despite different names*

### Comparing `IMMP-0.9.3/immp/plug/slack.py` & `IMMP-0.9.4/immp/plug/slack.py`

 * *Files 1% similar despite different names*

```diff
@@ -986,30 +986,30 @@
                 # Slack permanently caches user icon URLs; add monotonic hashes to keep them fresh.
                 data["icon_url"] = "{}#{}".format(msg.user.avatar, int(time.time()))
             elif self.config["fallback-image"]:
                 data["icon_url"] = self.config["fallback-image"]
         for attach in msg.attachments:
             if isinstance(attach, immp.File):
                 # Upload each file to Slack.
-                data = FormData({"channels": channel.source,
+                form = FormData({"channels": channel.source,
                                  "filename": attach.title or ""})
                 if isinstance(parent.reply_to, immp.Receipt):
                     # Reply directly to the corresponding thread.  Note that thread_ts can be any
                     # message in the thread, it need not be resolved to the parent.
-                    data.add_field("thread_ts", msg.reply_to.id)
+                    form.add_field("thread_ts", msg.reply_to.id)
                     if self.config["thread-broadcast"]:
-                        data.add_field("broadcast", "true")
+                        form.add_field("broadcast", "true")
                 if name:
                     comment = immp.RichText([immp.Segment(name, bold=True, italic=True,
                                                           link=msg.user.link),
                                              immp.Segment(" uploaded this file", italic=True)])
-                    data.add_field("initial_comment", SlackRichText.to_mrkdwn(self, comment))
+                    form.add_field("initial_comment", SlackRichText.to_mrkdwn(self, comment))
                 img_resp = await attach.get_content(self.session)
-                data.add_field("file", img_resp.content, filename="file")
-                upload = await self._api("files.upload", _Schema.upload, data=data)
+                form.add_field("file", img_resp.content, filename="file")
+                upload = await self._api("files.upload", _Schema.upload, data=form)
                 uploads += 1
                 for shared in upload["file"]["shares"].values():
                     if channel.source in shared:
                         ids += [share["ts"] for share in shared[channel.source]]
         if len(ids) < uploads:
             log.warning("Missing some file shares: sent %d, got %d", uploads, len(ids))
         rich = None
```

### Comparing `IMMP-0.9.3/immp/plug/telegram.py` & `IMMP-0.9.4/immp/plug/telegram.py`

 * *Files identical despite different names*

### Comparing `IMMP-0.9.3/immp/plug/github.py` & `IMMP-0.9.4/immp/plug/github.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
     _repo = {"full_name": str}
 
     _issue = {"number": int,
               "title": str,
               "html_url": str}
 
-    _pull = {immp.Optional("merged", False), bool}
+    _pull = {immp.Optional("merged", False): bool}
     _pull.update(_issue)
 
     event = immp.Schema({"sender": _sender,
                          immp.Optional("organization"): immp.Nullable(_sender),
                          immp.Optional("repository"): immp.Nullable(_repo),
                          immp.Optional("issue"): immp.Nullable(_issue),
                          immp.Optional("pull_request"): immp.Nullable(_pull)})
```

### Comparing `IMMP-0.9.3/immp/__main__.py` & `IMMP-0.9.4/immp/__main__.py`

 * *Files identical despite different names*

### Comparing `IMMP-0.9.3/immp/hook/alerts.py` & `IMMP-0.9.4/immp/hook/alerts.py`

 * *Files identical despite different names*

### Comparing `IMMP-0.9.3/immp/hook/identitylocal.py` & `IMMP-0.9.4/immp/hook/identitylocal.py`

 * *Files identical despite different names*

### Comparing `IMMP-0.9.3/immp/hook/sync.py` & `IMMP-0.9.4/immp/hook/sync.py`

 * *Files identical despite different names*

### Comparing `IMMP-0.9.3/immp/hook/command.py` & `IMMP-0.9.4/immp/hook/command.py`

 * *Files identical despite different names*

### Comparing `IMMP-0.9.3/immp/hook/notes.py` & `IMMP-0.9.4/immp/hook/notes.py`

 * *Files identical despite different names*

### Comparing `IMMP-0.9.3/immp/hook/webui/__init__.py` & `IMMP-0.9.4/immp/hook/webui/__init__.py`

 * *Files identical despite different names*

### Comparing `IMMP-0.9.3/immp/hook/webui/templates/main.j2` & `IMMP-0.9.4/immp/hook/webui/templates/main.j2`

 * *Files identical despite different names*

### Comparing `IMMP-0.9.3/immp/hook/webui/templates/group.j2` & `IMMP-0.9.4/immp/hook/webui/templates/group.j2`

 * *Files identical despite different names*

### Comparing `IMMP-0.9.3/immp/hook/webui/templates/add.j2` & `IMMP-0.9.4/immp/hook/webui/templates/add.j2`

 * *Files identical despite different names*

### Comparing `IMMP-0.9.3/immp/hook/webui/templates/plug.j2` & `IMMP-0.9.4/immp/hook/webui/templates/plug.j2`

 * *Files identical despite different names*

### Comparing `IMMP-0.9.3/immp/hook/webui/templates/hook_remove.j2` & `IMMP-0.9.4/immp/hook/webui/templates/hook_remove.j2`

 * *Files identical despite different names*

### Comparing `IMMP-0.9.3/immp/hook/webui/templates/channel.j2` & `IMMP-0.9.4/immp/hook/webui/templates/channel.j2`

 * *Files identical despite different names*

### Comparing `IMMP-0.9.3/immp/hook/webui/templates/plug_remove.j2` & `IMMP-0.9.4/immp/hook/webui/templates/plug_remove.j2`

 * *Files identical despite different names*

### Comparing `IMMP-0.9.3/immp/hook/webui/templates/plug_channels.j2` & `IMMP-0.9.4/immp/hook/webui/templates/plug_channels.j2`

 * *Files identical despite different names*

### Comparing `IMMP-0.9.3/immp/hook/webui/templates/hook.j2` & `IMMP-0.9.4/immp/hook/webui/templates/hook.j2`

 * *Files identical despite different names*

### Comparing `IMMP-0.9.3/immp/hook/webui/templates/base.j2` & `IMMP-0.9.4/immp/hook/webui/templates/base.j2`

 * *Files identical despite different names*

### Comparing `IMMP-0.9.3/immp/hook/webui/templates/macros.j2` & `IMMP-0.9.4/immp/hook/webui/templates/macros.j2`

 * *Files identical despite different names*

### Comparing `IMMP-0.9.3/immp/hook/identity.py` & `IMMP-0.9.4/immp/hook/identity.py`

 * *Files identical despite different names*

### Comparing `IMMP-0.9.3/immp/hook/autorespond.py` & `IMMP-0.9.4/immp/hook/autorespond.py`

 * *Files identical despite different names*

### Comparing `IMMP-0.9.3/immp/hook/shell.py` & `IMMP-0.9.4/immp/hook/shell.py`

 * *Files identical despite different names*

### Comparing `IMMP-0.9.3/immp/hook/web.py` & `IMMP-0.9.4/immp/hook/web.py`

 * *Files identical despite different names*

### Comparing `IMMP-0.9.3/immp/hook/access.py` & `IMMP-0.9.4/immp/hook/access.py`

 * *Files identical despite different names*

### Comparing `IMMP-0.9.3/immp/hook/textcommand.py` & `IMMP-0.9.4/immp/hook/textcommand.py`

 * *Files identical despite different names*

### Comparing `IMMP-0.9.3/immp/hook/runner.py` & `IMMP-0.9.4/immp/hook/runner.py`

 * *Files identical despite different names*

### Comparing `IMMP-0.9.3/immp/hook/database.py` & `IMMP-0.9.4/immp/hook/database.py`

 * *Files identical despite different names*

### Comparing `IMMP-0.9.3/immp/hook/hangoutslock.py` & `IMMP-0.9.4/immp/hook/hangoutslock.py`

 * *Files identical despite different names*

### Comparing `IMMP-0.9.3/immp/hook/discordrole.py` & `IMMP-0.9.4/immp/hook/discordrole.py`

 * *Files identical despite different names*

### Comparing `IMMP-0.9.3/README.rst` & `IMMP-0.9.4/README.rst`

 * *Files identical despite different names*

