# Comparing `tmp/Leytonium-8.tar.gz` & `tmp/Leytonium-9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Leytonium-8.tar", last modified: Wed Sep  7 16:25:29 2022, max compression
+gzip compressed data, was "dist/Leytonium-9.tar", last modified: Thu Dec 15 17:58:19 2022, max compression
```

## Comparing `Leytonium-8.tar` & `Leytonium-9.tar`

### file list

```diff
@@ -1,97 +1,127 @@
-drwxrwxr-x   0 arc       (1000) arc       (1000)        0 2022-09-07 16:25:29.000000 Leytonium-8/
-drwxrwxr-x   0 arc       (1000) arc       (1000)        0 2022-09-07 16:25:29.000000 Leytonium-8/Leytonium.egg-info/
--rw-rw-r--   0 arc       (1000) arc       (1000)        1 2022-09-07 16:25:29.000000 Leytonium-8/Leytonium.egg-info/dependency_links.txt
--rw-rw-r--   0 arc       (1000) arc       (1000)      204 2022-09-07 16:25:29.000000 Leytonium-8/Leytonium.egg-info/requires.txt
--rw-rw-r--   0 arc       (1000) arc       (1000)     2919 2022-09-07 16:25:29.000000 Leytonium-8/Leytonium.egg-info/entry_points.txt
--rw-rw-r--   0 arc       (1000) arc       (1000)     1929 2022-09-07 16:25:29.000000 Leytonium-8/Leytonium.egg-info/SOURCES.txt
--rw-rw-r--   0 arc       (1000) arc       (1000)       18 2022-09-07 16:25:29.000000 Leytonium-8/Leytonium.egg-info/top_level.txt
--rw-rw-r--   0 arc       (1000) arc       (1000)     5233 2022-09-07 16:25:29.000000 Leytonium-8/Leytonium.egg-info/PKG-INFO
--rw-rw-r--   0 arc       (1000) arc       (1000)     9165 2022-09-07 16:25:28.000000 Leytonium-8/setup.py
--rw-rw-r--   0 arc       (1000) arc       (1000)       67 2022-09-07 16:25:29.000000 Leytonium-8/setup.cfg
--rw-rw-r--   0 arc       (1000) arc       (1000)    35147 2019-11-17 19:03:15.000000 Leytonium-8/COPYING
--rw-rw-r--   0 arc       (1000) arc       (1000)     4956 2022-08-30 18:59:57.000000 Leytonium-8/README.md
-drwxrwxr-x   0 arc       (1000) arc       (1000)        0 2022-09-07 16:25:29.000000 Leytonium-8/diffuse/
--rw-rw-r--   0 arc       (1000) arc       (1000)     7193 2020-12-19 11:20:36.000000 Leytonium-8/diffuse/util.py
--rw-rw-r--   0 arc       (1000) arc       (1000)    14005 2020-12-29 09:55:35.000000 Leytonium-8/diffuse/main.py
--rw-rw-r--   0 arc       (1000) arc       (1000)    54037 2020-12-19 11:37:05.000000 Leytonium-8/diffuse/vcs.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     2091 2020-12-12 20:43:46.000000 Leytonium-8/diffuse/girepo.py
--rw-rw-r--   0 arc       (1000) arc       (1000)    81764 2020-12-21 15:10:05.000000 Leytonium-8/diffuse/diffuse.py
-drwxrwxr-x   0 arc       (1000) arc       (1000)        0 2022-09-07 16:25:29.000000 Leytonium-8/diffuse/viewer/
--rw-rw-r--   0 arc       (1000) arc       (1000)    11630 2020-12-19 11:15:55.000000 Leytonium-8/diffuse/viewer/util.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     5973 2020-12-19 11:13:00.000000 Leytonium-8/diffuse/viewer/undo.py
--rw-rw-r--   0 arc       (1000) arc       (1000)   137983 2020-12-21 15:10:05.000000 Leytonium-8/diffuse/viewer/viewer.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     3469 2020-12-19 11:12:26.000000 Leytonium-8/diffuse/viewer/model.py
--rw-rw-r--   0 arc       (1000) arc       (1000)      697 2020-12-21 15:10:05.000000 Leytonium-8/diffuse/viewer/__init__.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     9992 2020-12-12 14:22:33.000000 Leytonium-8/diffuse/viewer/patience.py
--rw-rw-r--   0 arc       (1000) arc       (1000)    24789 2020-12-19 11:29:42.000000 Leytonium-8/diffuse/resources.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     5001 2020-12-12 20:41:32.000000 Leytonium-8/diffuse/ui.py
--rw-rw-r--   0 arc       (1000) arc       (1000)    20944 2020-12-19 11:28:37.000000 Leytonium-8/diffuse/preferences.py
--rw-rw-r--   0 arc       (1000) arc       (1000)      697 2020-12-12 12:02:01.000000 Leytonium-8/diffuse/__init__.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     5233 2022-09-07 16:25:29.000000 Leytonium-8/PKG-INFO
-drwxrwxr-x   0 arc       (1000) arc       (1000)        0 2022-09-07 16:25:29.000000 Leytonium-8/leytonium/
--rw-rw-r--   0 arc       (1000) arc       (1000)      362 2020-02-16 12:00:56.000000 Leytonium-8/leytonium/vpn.bash
--rw-rw-r--   0 arc       (1000) arc       (1000)      964 2021-06-10 20:36:08.000000 Leytonium-8/leytonium/publish.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     2196 2021-03-06 02:02:53.000000 Leytonium-8/leytonium/shortcommands.py
--rw-rw-r--   0 arc       (1000) arc       (1000)      871 2021-01-17 14:31:16.000000 Leytonium-8/leytonium/ci.py
--rw-rw-r--   0 arc       (1000) arc       (1000)      722 2021-04-06 19:47:00.000000 Leytonium-8/leytonium/watchdesk.arid
--rw-rw-r--   0 arc       (1000) arc       (1000)     3604 2021-06-10 20:36:40.000000 Leytonium-8/leytonium/stacks.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     1136 2021-06-10 20:37:03.000000 Leytonium-8/leytonium/ks.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     1095 2021-01-17 14:31:31.000000 Leytonium-8/leytonium/show.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     3429 2021-06-23 11:37:46.000000 Leytonium-8/leytonium/hgcommit.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     1100 2021-01-17 14:32:24.000000 Leytonium-8/leytonium/ren.py
--rw-rw-r--   0 arc       (1000) arc       (1000)      140 2020-02-16 12:00:56.000000 Leytonium-8/leytonium/eb.bash
--rw-rw-r--   0 arc       (1000) arc       (1000)     1440 2022-07-02 10:37:33.000000 Leytonium-8/leytonium/tempvenv.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     1619 2021-12-09 17:50:23.000000 Leytonium-8/leytonium/veryshortcommands.py
--rw-rw-r--   0 arc       (1000) arc       (1000)      982 2021-01-17 14:32:56.000000 Leytonium-8/leytonium/n.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     1477 2021-03-04 21:03:56.000000 Leytonium-8/leytonium/isotime.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     5401 2021-06-10 20:39:29.000000 Leytonium-8/leytonium/resimp.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     7727 2021-06-10 21:24:06.000000 Leytonium-8/leytonium/common.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     1096 2020-12-06 23:24:53.000000 Leytonium-8/leytonium/setparent.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     2976 2021-03-08 22:06:07.000000 Leytonium-8/leytonium/taskding.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     1259 2021-06-10 20:44:25.000000 Leytonium-8/leytonium/prepare.py
--rw-rw-r--   0 arc       (1000) arc       (1000)      208 2020-07-30 21:29:03.000000 Leytonium-8/leytonium/gimports.bash
--rw-rw-r--   0 arc       (1000) arc       (1000)      918 2021-01-17 14:35:40.000000 Leytonium-8/leytonium/unpub.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     1130 2021-06-10 20:44:35.000000 Leytonium-8/leytonium/scrape85.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     1083 2021-01-17 14:40:11.000000 Leytonium-8/leytonium/delegate.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     1228 2021-07-04 14:08:49.000000 Leytonium-8/leytonium/refactor.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     1209 2022-04-14 21:07:25.000000 Leytonium-8/leytonium/spamtrash.arid
--rw-rw-r--   0 arc       (1000) arc       (1000)     1959 2021-06-10 20:45:02.000000 Leytonium-8/leytonium/slam.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     1542 2021-04-06 19:47:00.000000 Leytonium-8/leytonium/watchdesk.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     1713 2021-06-25 17:53:35.000000 Leytonium-8/leytonium/upgrade.py
--rw-rw-r--   0 arc       (1000) arc       (1000)      829 2020-12-27 16:21:59.000000 Leytonium-8/leytonium/halp.arid
--rw-rw-r--   0 arc       (1000) arc       (1000)     1084 2020-07-30 21:29:07.000000 Leytonium-8/leytonium/squash.bash
--rw-rw-r--   0 arc       (1000) arc       (1000)     7553 2021-06-10 20:48:06.000000 Leytonium-8/leytonium/stmulti.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     2338 2021-06-10 20:48:29.000000 Leytonium-8/leytonium/splitpkgs.py
--rw-rw-r--   0 arc       (1000) arc       (1000)      855 2020-07-01 23:22:58.000000 Leytonium-8/leytonium/drclean.bash
--rw-rw-r--   0 arc       (1000) arc       (1000)     1429 2022-08-30 18:59:33.000000 Leytonium-8/leytonium/extractaudio.py
--rw-rw-r--   0 arc       (1000) arc       (1000)      990 2021-01-17 14:42:33.000000 Leytonium-8/leytonium/autopull.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     1505 2021-03-04 21:20:07.000000 Leytonium-8/leytonium/brown.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     1428 2021-03-05 09:57:59.000000 Leytonium-8/leytonium/gt.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     1069 2021-06-10 20:48:52.000000 Leytonium-8/leytonium/touchb.py
--rw-rw-r--   0 arc       (1000) arc       (1000)      881 2021-01-17 14:44:31.000000 Leytonium-8/leytonium/readjust.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     3569 2021-06-10 21:12:10.000000 Leytonium-8/leytonium/multimerge.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     1108 2021-06-10 21:12:34.000000 Leytonium-8/leytonium/dp.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     2711 2021-06-10 21:21:02.000000 Leytonium-8/leytonium/st.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     1116 2020-12-06 23:25:08.000000 Leytonium-8/leytonium/rol.py
--rw-rw-r--   0 arc       (1000) arc       (1000)      597 2020-02-25 23:02:17.000000 Leytonium-8/leytonium/examine.bash
--rw-rw-r--   0 arc       (1000) arc       (1000)     1500 2021-06-09 22:06:23.000000 Leytonium-8/leytonium/next.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     1931 2021-10-23 15:54:18.000000 Leytonium-8/leytonium/scripts.py
--rw-rw-r--   0 arc       (1000) arc       (1000)      394 2020-12-06 23:19:43.000000 Leytonium-8/leytonium/fixemails.bash
--rw-rw-r--   0 arc       (1000) arc       (1000)      916 2021-01-17 14:46:53.000000 Leytonium-8/leytonium/abandon.py
--rw-rw-r--   0 arc       (1000) arc       (1000)      756 2021-03-05 09:57:42.000000 Leytonium-8/leytonium/common.arid
--rw-rw-r--   0 arc       (1000) arc       (1000)     1029 2021-01-17 14:46:57.000000 Leytonium-8/leytonium/br.py
--rw-rw-r--   0 arc       (1000) arc       (1000)      989 2021-01-17 14:47:01.000000 Leytonium-8/leytonium/co.py
--rw-rw-r--   0 arc       (1000) arc       (1000)      270 2021-01-09 10:32:15.000000 Leytonium-8/leytonium/mdview.bash
--rw-rw-r--   0 arc       (1000) arc       (1000)      460 2020-10-30 22:36:37.000000 Leytonium-8/leytonium/drop.bash
--rw-rw-r--   0 arc       (1000) arc       (1000)     1657 2021-06-10 21:21:40.000000 Leytonium-8/leytonium/dx.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     4646 2022-04-14 21:07:25.000000 Leytonium-8/leytonium/spamtrash.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     2237 2021-11-13 18:07:20.000000 Leytonium-8/leytonium/git_completion.bash
--rw-rw-r--   0 arc       (1000) arc       (1000)     1240 2021-06-10 21:21:55.000000 Leytonium-8/leytonium/shove.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     2614 2021-06-10 21:22:09.000000 Leytonium-8/leytonium/awslogs.py
--rw-rw-r--   0 arc       (1000) arc       (1000)       80 2021-10-23 15:56:30.000000 Leytonium-8/leytonium/t.bash
--rw-rw-r--   0 arc       (1000) arc       (1000)      402 2020-07-30 21:29:13.000000 Leytonium-8/leytonium/reks.bash
--rw-rw-r--   0 arc       (1000) arc       (1000)      932 2021-11-19 19:05:32.000000 Leytonium-8/leytonium/__init__.py
--rw-rw-r--   0 arc       (1000) arc       (1000)      103 2020-04-26 12:53:50.000000 Leytonium-8/leytonium/vunzip.bash
--rw-rw-r--   0 arc       (1000) arc       (1000)     1951 2021-03-07 21:55:57.000000 Leytonium-8/leytonium/halp.py
--rw-rw-r--   0 arc       (1000) arc       (1000)      596 2020-02-16 12:00:56.000000 Leytonium-8/leytonium/git_functions.bash
--rw-rw-r--   0 arc       (1000) arc       (1000)      881 2021-03-02 19:47:12.000000 Leytonium-8/leytonium/taskding.arid
+drwxrwxr-x   0 arc       (1000) arc       (1000)        0 2022-12-15 17:58:19.000000 Leytonium-9/
+drwxrwxr-x   0 arc       (1000) arc       (1000)        0 2022-12-15 17:58:19.000000 Leytonium-9/Leytonium.egg-info/
+-rw-rw-r--   0 arc       (1000) arc       (1000)        1 2022-12-15 17:58:19.000000 Leytonium-9/Leytonium.egg-info/dependency_links.txt
+-rw-rw-r--   0 arc       (1000) arc       (1000)      204 2022-12-15 17:58:19.000000 Leytonium-9/Leytonium.egg-info/requires.txt
+-rw-rw-r--   0 arc       (1000) arc       (1000)     2292 2022-12-15 17:58:19.000000 Leytonium-9/Leytonium.egg-info/entry_points.txt
+-rw-rw-r--   0 arc       (1000) arc       (1000)     2495 2022-12-15 17:58:19.000000 Leytonium-9/Leytonium.egg-info/SOURCES.txt
+-rw-rw-r--   0 arc       (1000) arc       (1000)       18 2022-12-15 17:58:19.000000 Leytonium-9/Leytonium.egg-info/top_level.txt
+-rw-rw-r--   0 arc       (1000) arc       (1000)     5233 2022-12-15 17:58:19.000000 Leytonium-9/Leytonium.egg-info/PKG-INFO
+-rw-rw-r--   0 arc       (1000) arc       (1000)     8538 2022-12-15 17:58:16.000000 Leytonium-9/setup.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)       67 2022-12-15 17:58:19.000000 Leytonium-9/setup.cfg
+-rw-rw-r--   0 arc       (1000) arc       (1000)    35147 2019-11-17 19:03:15.000000 Leytonium-9/COPYING
+-rw-rw-r--   0 arc       (1000) arc       (1000)     4956 2022-08-30 18:59:57.000000 Leytonium-9/README.md
+drwxrwxr-x   0 arc       (1000) arc       (1000)        0 2022-12-15 17:58:19.000000 Leytonium-9/diffuse/
+-rw-rw-r--   0 arc       (1000) arc       (1000)     7193 2020-12-19 11:20:36.000000 Leytonium-9/diffuse/util.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)    13948 2022-10-18 20:56:55.000000 Leytonium-9/diffuse/main.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)    54037 2020-12-19 11:37:05.000000 Leytonium-9/diffuse/vcs.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     2091 2020-12-12 20:43:46.000000 Leytonium-9/diffuse/girepo.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)    81871 2022-10-18 20:57:01.000000 Leytonium-9/diffuse/diffuse.py
+drwxrwxr-x   0 arc       (1000) arc       (1000)        0 2022-12-15 17:58:19.000000 Leytonium-9/diffuse/viewer/
+-rw-rw-r--   0 arc       (1000) arc       (1000)    11630 2020-12-19 11:15:55.000000 Leytonium-9/diffuse/viewer/util.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     5973 2020-12-19 11:13:00.000000 Leytonium-9/diffuse/viewer/undo.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)   137983 2020-12-21 15:10:05.000000 Leytonium-9/diffuse/viewer/viewer.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     3469 2020-12-19 11:12:26.000000 Leytonium-9/diffuse/viewer/model.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)      697 2020-12-21 15:10:05.000000 Leytonium-9/diffuse/viewer/__init__.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     9992 2020-12-12 14:22:33.000000 Leytonium-9/diffuse/viewer/patience.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)    24789 2020-12-19 11:29:42.000000 Leytonium-9/diffuse/resources.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     5001 2020-12-12 20:41:32.000000 Leytonium-9/diffuse/ui.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)    20944 2020-12-19 11:28:37.000000 Leytonium-9/diffuse/preferences.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)      697 2020-12-12 12:02:01.000000 Leytonium-9/diffuse/__init__.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     5233 2022-12-15 17:58:19.000000 Leytonium-9/PKG-INFO
+drwxrwxr-x   0 arc       (1000) arc       (1000)        0 2022-12-15 17:58:19.000000 Leytonium-9/leytonium/
+-rw-rw-r--   0 arc       (1000) arc       (1000)      845 2022-10-18 21:12:29.000000 Leytonium-9/leytonium/t.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)      836 2022-10-18 21:13:16.000000 Leytonium-9/leytonium/vpn.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)      362 2020-02-16 12:00:56.000000 Leytonium-9/leytonium/vpn.bash
+-rw-rw-r--   0 arc       (1000) arc       (1000)      982 2022-10-18 20:58:25.000000 Leytonium-9/leytonium/pd.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)      991 2022-10-18 23:13:56.000000 Leytonium-9/leytonium/publish.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)      868 2022-10-18 21:04:40.000000 Leytonium-9/leytonium/squash.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)      874 2022-10-18 21:11:16.000000 Leytonium-9/leytonium/fixemails.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)      903 2022-10-18 20:53:05.000000 Leytonium-9/leytonium/ci.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)      722 2021-04-06 19:47:00.000000 Leytonium-9/leytonium/watchdesk.arid
+-rw-rw-r--   0 arc       (1000) arc       (1000)     3632 2022-10-18 22:54:09.000000 Leytonium-9/leytonium/stacks.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)      842 2022-10-18 22:34:59.000000 Leytonium-9/leytonium/d.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     1168 2022-10-18 23:15:16.000000 Leytonium-9/leytonium/ks.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)      835 2022-10-18 21:13:20.000000 Leytonium-9/leytonium/vunzip.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     1125 2022-10-18 22:54:23.000000 Leytonium-9/leytonium/show.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)      865 2022-10-18 21:19:12.000000 Leytonium-9/leytonium/rdx.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)      897 2022-10-18 20:49:32.000000 Leytonium-9/leytonium/agi.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     1009 2022-10-18 22:39:05.000000 Leytonium-9/leytonium/bashrc.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     3455 2022-10-18 22:55:23.000000 Leytonium-9/leytonium/hgcommit.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     1131 2022-10-18 23:16:35.000000 Leytonium-9/leytonium/ren.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     1154 2022-10-18 20:49:59.000000 Leytonium-9/leytonium/agil.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)      140 2020-02-16 12:00:56.000000 Leytonium-9/leytonium/eb.bash
+-rw-rw-r--   0 arc       (1000) arc       (1000)     1466 2022-10-18 23:12:53.000000 Leytonium-9/leytonium/tempvenv.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     1015 2022-10-18 22:53:38.000000 Leytonium-9/leytonium/n.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     1232 2022-10-18 23:30:53.000000 Leytonium-9/leytonium/unslam.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)      887 2022-10-18 22:27:10.000000 Leytonium-9/leytonium/rx.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     1496 2022-10-18 23:15:07.000000 Leytonium-9/leytonium/isotime.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     5429 2022-10-18 23:13:07.000000 Leytonium-9/leytonium/resimp.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     7727 2021-06-10 21:24:06.000000 Leytonium-9/leytonium/common.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     1121 2022-10-18 23:16:43.000000 Leytonium-9/leytonium/setparent.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     3256 2022-11-04 23:12:46.000000 Leytonium-9/leytonium/taskding.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     1286 2022-10-18 23:17:02.000000 Leytonium-9/leytonium/prepare.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)      208 2020-07-30 21:29:03.000000 Leytonium-9/leytonium/gimports.bash
+-rw-rw-r--   0 arc       (1000) arc       (1000)     1266 2022-10-18 22:26:45.000000 Leytonium-9/leytonium/rd.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)      847 2022-10-19 21:44:38.000000 Leytonium-9/leytonium/fetchall.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)      947 2022-10-18 20:46:19.000000 Leytonium-9/leytonium/unpub.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     1156 2022-10-18 23:16:53.000000 Leytonium-9/leytonium/scrape85.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     1083 2022-10-06 23:10:56.000000 Leytonium-9/leytonium/delegate.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     1361 2022-10-18 22:49:01.000000 Leytonium-9/leytonium/dxx.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)      869 2022-10-18 21:06:43.000000 Leytonium-9/leytonium/examine.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)      843 2022-10-18 21:13:08.000000 Leytonium-9/leytonium/mdview.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)      881 2022-10-18 22:39:11.000000 Leytonium-9/leytonium/git_functions_path.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)      845 2022-10-18 21:11:31.000000 Leytonium-9/leytonium/reks.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     1209 2022-04-14 21:07:25.000000 Leytonium-9/leytonium/spamtrash.arid
+-rw-rw-r--   0 arc       (1000) arc       (1000)     1524 2022-10-18 23:30:31.000000 Leytonium-9/leytonium/slam.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     1557 2022-10-18 20:46:50.000000 Leytonium-9/leytonium/watchdesk.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     1740 2022-10-18 20:46:36.000000 Leytonium-9/leytonium/upgrade.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)      829 2020-12-27 16:21:59.000000 Leytonium-9/leytonium/halp.arid
+-rw-rw-r--   0 arc       (1000) arc       (1000)     1084 2020-07-30 21:29:07.000000 Leytonium-9/leytonium/squash.bash
+-rw-rw-r--   0 arc       (1000) arc       (1000)     7305 2022-10-19 21:44:23.000000 Leytonium-9/leytonium/stmulti.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     2363 2022-10-18 23:23:53.000000 Leytonium-9/leytonium/splitpkgs.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)      855 2020-07-01 23:22:58.000000 Leytonium-9/leytonium/drclean.bash
+-rw-rw-r--   0 arc       (1000) arc       (1000)     1451 2022-10-18 22:50:23.000000 Leytonium-9/leytonium/extractaudio.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     1016 2022-10-18 20:51:02.000000 Leytonium-9/leytonium/autopull.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     1528 2022-10-18 20:52:56.000000 Leytonium-9/leytonium/brown.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     1461 2022-10-23 22:19:29.000000 Leytonium-9/leytonium/gt.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     1097 2022-10-18 20:46:07.000000 Leytonium-9/leytonium/touchb.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)      907 2022-10-18 23:24:02.000000 Leytonium-9/leytonium/readjust.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     3593 2022-10-18 23:14:21.000000 Leytonium-9/leytonium/multimerge.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)      959 2022-10-18 20:58:04.000000 Leytonium-9/leytonium/dp.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     2743 2022-10-18 23:24:14.000000 Leytonium-9/leytonium/st.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     1147 2022-10-18 23:24:23.000000 Leytonium-9/leytonium/rol.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)      597 2020-02-25 23:02:17.000000 Leytonium-9/leytonium/examine.bash
+-rw-rw-r--   0 arc       (1000) arc       (1000)      863 2022-10-19 21:44:56.000000 Leytonium-9/leytonium/pushall.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)      951 2022-10-18 23:26:00.000000 Leytonium-9/leytonium/dup.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     1530 2022-10-18 22:55:06.000000 Leytonium-9/leytonium/next.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)      898 2022-10-18 22:26:20.000000 Leytonium-9/leytonium/gag.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)      810 2022-10-18 21:18:36.000000 Leytonium-9/leytonium/pb.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)      394 2020-12-06 23:19:43.000000 Leytonium-9/leytonium/fixemails.bash
+-rw-rw-r--   0 arc       (1000) arc       (1000)      846 2022-10-19 21:45:03.000000 Leytonium-9/leytonium/pullall.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)      943 2022-10-18 20:48:11.000000 Leytonium-9/leytonium/abandon.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)      831 2022-10-18 21:05:20.000000 Leytonium-9/leytonium/drst.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)      756 2021-03-05 09:57:42.000000 Leytonium-9/leytonium/common.arid
+-rw-rw-r--   0 arc       (1000) arc       (1000)      825 2022-10-18 21:18:58.000000 Leytonium-9/leytonium/showstash.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     1061 2022-10-18 20:52:45.000000 Leytonium-9/leytonium/br.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     1021 2022-10-18 20:55:04.000000 Leytonium-9/leytonium/co.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)      833 2022-10-18 21:04:05.000000 Leytonium-9/leytonium/drclean.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)      270 2021-01-09 10:32:15.000000 Leytonium-9/leytonium/mdview.bash
+-rw-rw-r--   0 arc       (1000) arc       (1000)      879 2022-10-18 21:11:23.000000 Leytonium-9/leytonium/eb.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)      460 2020-10-30 22:36:37.000000 Leytonium-9/leytonium/drop.bash
+-rw-rw-r--   0 arc       (1000) arc       (1000)      826 2022-10-18 21:07:07.000000 Leytonium-9/leytonium/drop.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)      858 2022-10-18 21:07:31.000000 Leytonium-9/leytonium/gimports.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     1144 2022-10-18 22:49:24.000000 Leytonium-9/leytonium/dx.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)      944 2022-10-18 22:39:08.000000 Leytonium-9/leytonium/git_completion_path.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     4661 2022-10-18 22:53:54.000000 Leytonium-9/leytonium/spamtrash.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     2250 2022-11-04 22:17:56.000000 Leytonium-9/leytonium/git_completion.bash
+-rw-rw-r--   0 arc       (1000) arc       (1000)     1310 2022-10-18 23:24:31.000000 Leytonium-9/leytonium/shove.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     2678 2022-10-18 20:51:13.000000 Leytonium-9/leytonium/awslogs.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     1078 2022-10-18 22:39:26.000000 Leytonium-9/leytonium/insertshlvl.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)       80 2021-10-23 15:56:30.000000 Leytonium-9/leytonium/t.bash
+-rw-rw-r--   0 arc       (1000) arc       (1000)      402 2020-07-30 21:29:13.000000 Leytonium-9/leytonium/reks.bash
+-rw-rw-r--   0 arc       (1000) arc       (1000)      932 2021-11-19 19:05:32.000000 Leytonium-9/leytonium/__init__.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)      103 2020-04-26 12:53:50.000000 Leytonium-9/leytonium/vunzip.bash
+-rw-rw-r--   0 arc       (1000) arc       (1000)      940 2022-10-18 22:35:04.000000 Leytonium-9/leytonium/scrub.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     1976 2022-10-18 23:24:42.000000 Leytonium-9/leytonium/halp.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)      596 2020-02-16 12:00:56.000000 Leytonium-9/leytonium/git_functions.bash
+-rw-rw-r--   0 arc       (1000) arc       (1000)      881 2021-03-02 19:47:12.000000 Leytonium-9/leytonium/taskding.arid
```

### Comparing `Leytonium-8/Leytonium.egg-info/PKG-INFO` & `Leytonium-9/Leytonium.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Leytonium
-Version: 8
+Version: 9
 Summary: Tools for developing git-managed software
 Home-page: https://github.com/combatopera/Leytonium
 Author: Andrzej Cichocki
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: COPYING
```

### Comparing `Leytonium-8/setup.py` & `Leytonium-9/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -132,20 +132,20 @@
 def ext_modules():
     extensions = [path.make_ext() for path in sourceinfo.extpaths]
     return dict(ext_modules = cythonize(extensions)) if extensions else {}
 
 sourceinfo = SourceInfo('.')
 setuptools.setup(
         name = 'Leytonium',
-        version = '8',
+        version = '9',
         description = 'Tools for developing git-managed software',
         long_description = long_description(),
         long_description_content_type = 'text/markdown',
         url = 'https://github.com/combatopera/Leytonium',
         author = 'Andrzej Cichocki',
         packages = sourceinfo.packages,
         py_modules = [],
         install_requires = ['aridity>=35', 'autopep8>=1.5.4', 'awscli>=1.19.53', 'docutils>=0.15.2', 'importlib-metadata>=2.1.1', 'lagoon>=22', 'PyGObject>=3.27.2', 'pytz>=2020.4', 'pyven>=56', 'PyYAML>=5.2', 'setuptools>=44.1.1', 'termcolor>=1.1.0', 'Unidecode>=1.3.2'],
         package_data = {'': ['*.pxd', '*.pyx', '*.pyxbld', '*.arid', '*.aridt', '*.bash']},
         scripts = [],
-        entry_points = {'console_scripts': ['diffuse=diffuse.main:main_diffuse', 'abandon=leytonium.abandon:main_abandon', 'autopull=leytonium.autopull:main_autopull', 'awslogs=leytonium.awslogs:main_awslogs', 'br=leytonium.br:main_br', 'brown=leytonium.brown:main_brown', 'ci=leytonium.ci:main_ci', 'co=leytonium.co:main_co', 'dp=leytonium.dp:main_dp', 'pd=leytonium.dp:main_pd', 'dx=leytonium.dx:main_dx', 'dxx=leytonium.dx:main_dxx', 'extractaudio=leytonium.extractaudio:main_extractaudio', 'gt=leytonium.gt:main_gt', 'halp=leytonium.halp:main_halp', 'hgcommit=leytonium.hgcommit:main_hgcommit', 'isotime=leytonium.isotime:main_isotime', 'ks=leytonium.ks:main_ks', 'multimerge=leytonium.multimerge:main_multimerge', 'n=leytonium.n:main_n', 'next=leytonium.next:main_next', 'prepare=leytonium.prepare:main_prepare', 'publish=leytonium.publish:main_publish', 'readjust=leytonium.readjust:main_readjust', 'agi=leytonium.refactor:main_agi', 'agil=leytonium.refactor:main_agil', 'ren=leytonium.ren:main_ren', 'resimp=leytonium.resimp:main_resimp', 'rol=leytonium.rol:main_rol', 'scrape85=leytonium.scrape85:main_scrape85', 'squash=leytonium.scripts:main_squash', 'drclean=leytonium.scripts:main_drclean', 'drst=leytonium.scripts:main_drst', 'examine=leytonium.scripts:main_examine', 'drop=leytonium.scripts:main_drop', 'gimports=leytonium.scripts:main_gimports', 'reks=leytonium.scripts:main_reks', 'eb=leytonium.scripts:main_eb', 'fixemails=leytonium.scripts:main_fixemails', 'mdview=leytonium.scripts:main_mdview', 'vpn=leytonium.scripts:main_vpn', 'vunzip=leytonium.scripts:main_vunzip', 't=leytonium.scripts:main_t', 'setparent=leytonium.setparent:main_setparent', 'showstash=leytonium.shortcommands:main_showstash', 'pb=leytonium.shortcommands:main_pb', 'd=leytonium.shortcommands:main_d', 'rdx=leytonium.shortcommands:main_rdx', 'rx=leytonium.shortcommands:main_rx', 'gag=leytonium.shortcommands:main_gag', 'rd=leytonium.shortcommands:main_rd', 'dup=leytonium.shortcommands:main_dup', 'scrub=leytonium.shortcommands:main_scrub', 'shove=leytonium.shove:main_shove', 'show=leytonium.show:main_show', 'slam=leytonium.slam:main_slam', 'unslam=leytonium.slam:main_unslam', 'spamtrash=leytonium.spamtrash:main_spamtrash', 'splitpkgs=leytonium.splitpkgs:main_splitpkgs', 'st=leytonium.st:main_st', 'stacks=leytonium.stacks:main_stacks', 'stmulti=leytonium.stmulti:main_stmulti', 'fetchall=leytonium.stmulti:main_fetchall', 'pullall=leytonium.stmulti:main_pullall', 'pushall=leytonium.stmulti:main_pushall', 'taskding=leytonium.taskding:main_taskding', 'tempvenv=leytonium.tempvenv:main_tempvenv', 'touchb=leytonium.touchb:main_touchb', 'unpub=leytonium.unpub:main_unpub', 'upgrade=leytonium.upgrade:main_upgrade', 'git-completion-path=leytonium.veryshortcommands:main_git_completion_path', 'git-functions-path=leytonium.veryshortcommands:main_git_functions_path', 'insertshlvl=leytonium.veryshortcommands:main_insertshlvl', 'bashrc=leytonium.veryshortcommands:main_bashrc', 'watchdesk=leytonium.watchdesk:main_watchdesk']},
+        entry_points = {'console_scripts': ['diffuse=diffuse.diffuse:main', 'abandon=leytonium.abandon:main', 'agi=leytonium.agi:main', 'agil=leytonium.agil:main', 'autopull=leytonium.autopull:main', 'awslogs=leytonium.awslogs:main', 'bashrc=leytonium.bashrc:main', 'br=leytonium.br:main', 'brown=leytonium.brown:main', 'ci=leytonium.ci:main', 'co=leytonium.co:main', 'd=leytonium.d:main', 'dp=leytonium.dp:main', 'drclean=leytonium.drclean:main', 'drop=leytonium.drop:main', 'drst=leytonium.drst:main', 'dup=leytonium.dup:main', 'dx=leytonium.dx:main', 'dxx=leytonium.dxx:main', 'eb=leytonium.eb:main', 'examine=leytonium.examine:main', 'extractaudio=leytonium.extractaudio:main', 'fetchall=leytonium.fetchall:main', 'fixemails=leytonium.fixemails:main', 'gag=leytonium.gag:main', 'gimports=leytonium.gimports:main', 'git-completion-path=leytonium.git_completion_path:main', 'git-functions-path=leytonium.git_functions_path:main', 'gt=leytonium.gt:main', 'halp=leytonium.halp:main', 'hgcommit=leytonium.hgcommit:main', 'insertshlvl=leytonium.insertshlvl:main', 'isotime=leytonium.isotime:main', 'ks=leytonium.ks:main', 'mdview=leytonium.mdview:main', 'multimerge=leytonium.multimerge:main', 'n=leytonium.n:main', 'next=leytonium.next:main', 'pb=leytonium.pb:main', 'pd=leytonium.pd:main', 'prepare=leytonium.prepare:main', 'publish=leytonium.publish:main', 'pullall=leytonium.pullall:main', 'pushall=leytonium.pushall:main', 'rd=leytonium.rd:main', 'rdx=leytonium.rdx:main', 'readjust=leytonium.readjust:main', 'reks=leytonium.reks:main', 'ren=leytonium.ren:main', 'resimp=leytonium.resimp:main', 'rol=leytonium.rol:main', 'rx=leytonium.rx:main', 'scrape85=leytonium.scrape85:main', 'scrub=leytonium.scrub:main', 'setparent=leytonium.setparent:main', 'shove=leytonium.shove:main', 'show=leytonium.show:main', 'showstash=leytonium.showstash:main', 'slam=leytonium.slam:main', 'spamtrash=leytonium.spamtrash:main', 'splitpkgs=leytonium.splitpkgs:main', 'squash=leytonium.squash:main', 'st=leytonium.st:main', 'stacks=leytonium.stacks:main', 'stmulti=leytonium.stmulti:main', 't=leytonium.t:main', 'taskding=leytonium.taskding:main', 'tempvenv=leytonium.tempvenv:main', 'touchb=leytonium.touchb:main', 'unpub=leytonium.unpub:main', 'unslam=leytonium.unslam:main', 'upgrade=leytonium.upgrade:main', 'vpn=leytonium.vpn:main', 'vunzip=leytonium.vunzip:main', 'watchdesk=leytonium.watchdesk:main']},
         **ext_modules())
```

### Comparing `Leytonium-8/COPYING` & `Leytonium-9/COPYING`

 * *Files identical despite different names*

### Comparing `Leytonium-8/README.md` & `Leytonium-9/README.md`

 * *Files identical despite different names*

### Comparing `Leytonium-8/diffuse/util.py` & `Leytonium-9/diffuse/util.py`

 * *Files identical despite different names*

### Comparing `Leytonium-8/diffuse/main.py` & `Leytonium-9/diffuse/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,16 +48,15 @@
         if not os.path.exists(p):
             try:
                 os.mkdir(p)
             except IOError:
                 pass
     return p
 
-def main_diffuse():
-    'Compare an arbitrary number of text files.'
+def main():
     from .diffuse import Diffuse
     from .girepo import GObject, Gtk
     from .resources import Resources
     from .ui import logError
     from .vcs import VCSs
     from .viewer.viewer import FileDiffViewer
     # gettext looks for the language using environment variables which
```

### Comparing `Leytonium-8/diffuse/vcs.py` & `Leytonium-9/diffuse/vcs.py`

 * *Files identical despite different names*

### Comparing `Leytonium-8/diffuse/girepo.py` & `Leytonium-9/diffuse/girepo.py`

 * *Files identical despite different names*

### Comparing `Leytonium-8/diffuse/diffuse.py` & `Leytonium-9/diffuse/diffuse.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,17 @@
 #
 # You should have received a copy of the GNU General Public License along with
 # this program.  You may also obtain a copy of the GNU General Public License
 # from the Free Software Foundation by visiting their web site
 # (http://www.fsf.org/) or by writing to the Free Software Foundation, Inc.,
 # 51 Franklin St, Fifth Floor, Boston, MA  02110-1301  USA
 
+'Compare an arbitrary number of text files.'
 from .girepo import Gdk, GdkPixbuf, GObject, Gtk, Pango
+from .main import main
 from .preferences import Preferences
 from .ui import createMenu, EncodingMenu, MessageDialog
 from .util import APP_NAME, bin_dir, Format, isWindows, lang, logDebug, Mode, readlines, splitlines, VERSION, WEBSITE
 from .viewer.viewer import FileDiffViewer
 from gettext import gettext as _
 from urllib.parse import urlparse
 import codecs, os, shlex, stat, webbrowser
@@ -1782,7 +1784,10 @@
         webbrowser.open(help_url)
 
     # callback for the about menu item
     def about_cb(self, widget, data):
         dialog = AboutDialog(self.copyright)
         dialog.run()
         dialog.destroy()
+
+if '__main__' == __name__:
+    main()
```

### Comparing `Leytonium-8/diffuse/viewer/util.py` & `Leytonium-9/diffuse/viewer/util.py`

 * *Files identical despite different names*

### Comparing `Leytonium-8/diffuse/viewer/undo.py` & `Leytonium-9/diffuse/viewer/undo.py`

 * *Files identical despite different names*

### Comparing `Leytonium-8/diffuse/viewer/viewer.py` & `Leytonium-9/diffuse/viewer/viewer.py`

 * *Files identical despite different names*

### Comparing `Leytonium-8/diffuse/viewer/model.py` & `Leytonium-9/diffuse/viewer/model.py`

 * *Files identical despite different names*

### Comparing `Leytonium-8/diffuse/viewer/__init__.py` & `Leytonium-9/diffuse/viewer/__init__.py`

 * *Files identical despite different names*

### Comparing `Leytonium-8/diffuse/viewer/patience.py` & `Leytonium-9/diffuse/viewer/patience.py`

 * *Files identical despite different names*

### Comparing `Leytonium-8/diffuse/resources.py` & `Leytonium-9/diffuse/resources.py`

 * *Files identical despite different names*

### Comparing `Leytonium-8/diffuse/ui.py` & `Leytonium-9/diffuse/ui.py`

 * *Files identical despite different names*

### Comparing `Leytonium-8/diffuse/preferences.py` & `Leytonium-9/diffuse/preferences.py`

 * *Files identical despite different names*

### Comparing `Leytonium-8/diffuse/__init__.py` & `Leytonium-9/diffuse/__init__.py`

 * *Files identical despite different names*

### Comparing `Leytonium-8/PKG-INFO` & `Leytonium-9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Leytonium
-Version: 8
+Version: 9
 Summary: Tools for developing git-managed software
 Home-page: https://github.com/combatopera/Leytonium
 Author: Andrzej Cichocki
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: COPYING
```

### Comparing `Leytonium-8/leytonium/publish.py` & `Leytonium-9/leytonium/publish.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,14 +11,17 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with Leytonium.  If not, see <http://www.gnu.org/licenses/>.
 
+'Publish this branch, accepts push options.'
 from .common import thisbranch, pb, args
 from lagoon import git
 from lagoon.program import ONELINE
 
-def main_publish():
-    'Publish this branch, accepts push options.'
+def main():
     git.push._u[print](git.config.__get[ONELINE](f"branch.{pb()}.remote"), thisbranch(), *args())
+
+if '__main__' == __name__:
+    main()
```

### Comparing `Leytonium-8/leytonium/ci.py` & `Leytonium-9/leytonium/rx.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with Leytonium.  If not, see <http://www.gnu.org/licenses/>.
 
-from .common import args
+'Restore given file to parent branch version.'
+from .common import args, pb
 from lagoon import git
 
-def main_ci():
-    'Commit with the given args as message.'
-    message = ' '.join(args())
-    git.commit._m[print](message)
+def main():
+    git.checkout[print](pb(), *args())
+
+if '__main__' == __name__:
+    main()
```

### Comparing `Leytonium-8/leytonium/watchdesk.arid` & `Leytonium-9/leytonium/watchdesk.arid`

 * *Files identical despite different names*

### Comparing `Leytonium-8/leytonium/stacks.py` & `Leytonium-9/leytonium/stacks.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with Leytonium.  If not, see <http://www.gnu.org/licenses/>.
 
+'Compare stack traces across build logs.'
 import sys, tempfile, subprocess, re, datetime
 
 class Stack:
 
     def __init__(self, lines):
         self.lines = lines
 
@@ -94,17 +95,19 @@
 
 def compare(stackslist):
     files = [stacks.tofile() for stacks in stackslist]
     subprocess.run(['vim' if 1 == len(files) else 'diffuse'] + [f.name for f in files])
     for f in files:
         f.close()
 
-def main_stacks():
-    'Compare stack traces across build logs.'
+def main():
     paths = sys.argv[1:]
     stackslist = []
     for path in paths:
         stacks = Stacks()
         with open(path) as f:
             stacks.load(f)
         stackslist.append(stacks)
     compare(stackslist)
+
+if '__main__' == __name__:
+    main()
```

### Comparing `Leytonium-8/leytonium/ks.py` & `Leytonium-9/leytonium/ks.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,20 +11,23 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with Leytonium.  If not, see <http://www.gnu.org/licenses/>.
 
+'Create a kitchen-sink branch.'
 from .common import addparents
 from lagoon import git
 import os, re
 
 def githubuser():
     with open(os.path.join(os.path.expanduser('~'), '.git-credentials')) as f:
         return re.search('//([^:]+):.*github', f.read()).group(1)
 
-def main_ks():
-    'Create a kitchen-sink branch.'
+def main():
     master, ks = 'master', 'kitchen-sink'
     git.checkout._b[print](ks, master)
     addparents(ks, master, 'controversial/*', f"public/{githubuser()}-*")
+
+if '__main__' == __name__:
+    main()
```

### Comparing `Leytonium-8/leytonium/show.py` & `Leytonium-9/leytonium/show.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,22 +11,25 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with Leytonium.  If not, see <http://www.gnu.org/licenses/>.
 
+'Show a commit that was listed by st.'
 from .common import showmenu, AllBranches, savedcommits
 from lagoon import git
 import sys
 
-def main_show():
-    'Show a commit that was listed by st.'
+def main():
     items = AllBranches().branchcommits()
     n, = sys.argv[1:]
     n = int(n)
     if n > 0:
         commit = showmenu(items, False)[n]
     else:
         saved = savedcommits()
         commit = saved[len(saved) - 1 + n]
     git.show[exec](commit)
+
+if '__main__' == __name__:
+    main()
```

### Comparing `Leytonium-8/leytonium/hgcommit.py` & `Leytonium-9/leytonium/hgcommit.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with Leytonium.  If not, see <http://www.gnu.org/licenses/>.
 
+'Commit hook to push to central clone of repo on local network.'
 from . import effectivehome, initlogging
 from .stmulti import loadconfig, trunknames
 from diapyr.util import singleton
 from lagoon import git, ls, rsync
 from lagoon.program import ONELINE
 from pathlib import Path
 import os, subprocess, multiprocessing as mp, queue, logging
@@ -88,21 +89,23 @@
         rhs = f".{os.sep}", f"{dest.repohost}::{dest.reponame}/{dest.reldir}"
         rsync[print](*lhs, *rhs)
         os.utime('.rsync')
         lhs += '--del',
         rsync[print](*lhs, '--dry-run', *rhs)
         print(f"(cd {Path.cwd()} && rsync {' '.join(lhs)} {' '.join(rhs)})")
 
-def main_hgcommit():
-    'Commit hook to push to central clone of repo on local network.'
+def main():
     initlogging()
     config = loadconfig()
     reldir = Path.cwd().relative_to(effectivehome)
     for c in Git, Rsync:
         if Path(c.dirname).exists():
             command = c
             break
     dest = PathDest(config, command.mangle(reldir))
     if dest.check():
         command.pushorclone(dest)
     else:
         log.error("Bad path: %s", dest.clonespath)
+
+if '__main__' == __name__:
+    main()
```

### Comparing `Leytonium-8/leytonium/ren.py` & `Leytonium-9/leytonium/ren.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,19 +11,22 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with Leytonium.  If not, see <http://www.gnu.org/licenses/>.
 
+'Rename current branch.'
 from .common import thisbranch, args, findproject, infodirname
 from lagoon import git
 import os
 
-def main_ren():
-    'Rename current branch.'
+def main():
     fromname = thisbranch()
     git.branch._m[print](*args())
     d = os.path.join(findproject(), infodirname)
     target = os.path.join(d, thisbranch())
     os.makedirs(os.path.dirname(target), exist_ok = True)
     os.rename(os.path.join(d, fromname), target)
+
+if '__main__' == __name__:
+    main()
```

### Comparing `Leytonium-8/leytonium/tempvenv.py` & `Leytonium-9/leytonium/tempvenv.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,26 +11,29 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with Leytonium.  If not, see <http://www.gnu.org/licenses/>.
 
+'Activate a writable venv from the pool with the given requires.'
 from . import initlogging
 from argparse import ArgumentParser
 from lagoon.program import Program
 from pathlib import Path
 from venvpool import Pool, SimpleInstallDeps
 import logging, os, sys
 
 log = logging.getLogger(__name__)
 shellpath = os.environ['SHELL']
 
-def main_tempvenv():
-    'Activate a writable venv from the pool with the given requires.'
+def main():
     initlogging()
     parser = ArgumentParser()
     parser.add_argument('-p', type = int, default = sys.version_info.major)
     parser.add_argument('reqs', nargs = '*')
     args = parser.parse_args()
     with Pool(args.p).readwrite(SimpleInstallDeps(args.reqs)) as venv:
         Program.text(shellpath)._c[print]('. "$1" && exec "$2"', '-c', Path(venv.venvpath, 'bin', 'activate'), shellpath)
+
+if '__main__' == __name__:
+    main()
```

### Comparing `Leytonium-8/leytonium/veryshortcommands.py` & `Leytonium-9/leytonium/agil.py`

 * *Files 23% similar despite different names*

```diff
@@ -11,39 +11,24 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with Leytonium.  If not, see <http://www.gnu.org/licenses/>.
 
-from pathlib import Path
-import shlex, sys
+'Edit project files containing identifier.'
+from .common import findproject
+from lagoon import ag
+from lagoon.program import Program
+import os, sys
+
+def main():
+    search = sys.argv[1:]
+    editor = os.environ['EDITOR']
+    if 1 == len(search) and 'vim' == editor:
+        args = [rf"+/\<{search[0]}\>"]
+    else:
+        args = []
+    Program.text(editor)[exec](*args, *ag._wsl(*search, findproject()).splitlines())
 
-def main_git_completion_path():
-    'Get path to git completion file, used by scripts.'
-    print(_git_completion_path())
-
-def _git_completion_path():
-    return Path(__file__).parent / 'git_completion.bash'
-
-def main_git_functions_path():
-    'Get path to git functions file, used by scripts.'
-    print(Path(__file__).parent / 'git_functions.bash')
-
-def main_insertshlvl():
-    'Insert SHLVL indicator into given prompt.'
-    print(_insertshlvl(*sys.argv[1:]))
-
-def _insertshlvl(ps1, shlvl):
-    try:
-        colon = ps1.rindex(':')
-    except ValueError:
-        return ps1
-    n = int(shlvl)
-    tally = '"' * (n // 2) + ("'" if n % 2 else '')
-    return f"{ps1[:colon]}{tally}{ps1[colon + 1:]}"
-
-def main_bashrc():
-    'To eval in your .bashrc file.'
-    sys.stdout.write(f""". {shlex.quote(str(_git_completion_path()))}
-PS1={shlex.quote(_insertshlvl(*sys.argv[1:]))}
-""")
+if '__main__' == __name__:
+    main()
```

### Comparing `Leytonium-8/leytonium/n.py` & `Leytonium-9/leytonium/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,18 +11,14 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with Leytonium.  If not, see <http://www.gnu.org/licenses/>.
 
-from lagoon import co, git, st
+from pathlib import Path
+import logging, os
 
-def main_n():
-    'Switch to the next branch and run st.'
-    lines = git.branch().splitlines()
-    for i, line in enumerate(lines):
-        if line.startswith('*'):
-            b = lines[i + 1].strip()
-            break
-    co[print](b)
-    st[exec]()
+effectivehome = Path(f"~{os.environ.get('SUDO_USER', '')}").expanduser()
+
+def initlogging():
+    logging.basicConfig(level = logging.DEBUG, format = "%(asctime)s %(levelname)s %(message)s")
```

### Comparing `Leytonium-8/leytonium/isotime.py` & `Leytonium-9/leytonium/isotime.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with Leytonium.  If not, see <http://www.gnu.org/licenses/>.
 
+'Filter UNIX timestamps to human-readable form.'
 from aridity.config import ConfigCtrl
 from datetime import datetime
 import pytz, re, sys
 
 pattern = re.compile('(9[0-9]{8}|[1-3][0-9]{9})([0-9]{3})?')
 
 class Repl:
@@ -28,12 +29,14 @@
 
     def __call__(self, m):
         tstr, mstr = m.groups()
         t = int(tstr) + (int(mstr) / 1000 if mstr else 0)
         dt = datetime.utcfromtimestamp(t).replace(tzinfo = pytz.utc).astimezone(self.tz)
         return f"{dt.strftime('%Y-%m-%dT%H:%M:%S.%f')[:-3]}{dt.strftime('%z')}"
 
-def main_isotime():
-    'Filter UNIX timestamps to human-readable form.'
-    repl = Repl(ConfigCtrl().loadappconfig(main_isotime, 'common.arid'))
+def main():
+    repl = Repl(ConfigCtrl().loadappconfig(main, 'common.arid'))
     for line in sys.stdin:
         sys.stdout.write(pattern.sub(repl, line))
+
+if '__main__' == __name__:
+    main()
```

### Comparing `Leytonium-8/leytonium/resimp.py` & `Leytonium-9/leytonium/resimp.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with Leytonium.  If not, see <http://www.gnu.org/licenses/>.
 
+'Resolve conflicts in imports and adjacent-line conflicts.'
 from .common import stderr, findproject
 from lagoon import git
 import itertools, os, re
 
 def resimp(path):
     output = []
     chunks = [0]
@@ -135,13 +136,15 @@
             handler = handler(line) or handler
     if resolved[0]:
         with open(path, 'w') as g:
             for line in output:
                 g.write(line)
         stderr(f"[{path}] Auto-resolved {resolved[0]} adjacent-line conflicts.")
 
-def main_resimp():
-    'Resolve conflicts in imports and adjacent-line conflicts.'
+def main():
     os.chdir(findproject()) # Paths below are relative to project root.
     for path in git.diff.__name_only('--diff-filter=U').splitlines():
         for task in resimp, resadj:
             task(path)
+
+if '__main__' == __name__:
+    main()
```

### Comparing `Leytonium-8/leytonium/common.py` & `Leytonium-9/leytonium/common.py`

 * *Files identical despite different names*

### Comparing `Leytonium-8/leytonium/setparent.py` & `Leytonium-9/leytonium/setparent.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,19 +11,22 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with Leytonium.  If not, see <http://www.gnu.org/licenses/>.
 
+'Change declared parent of current branch.'
 from .common import args as getargs, addparents, thisbranch, getpublic
 
-def main_setparent():
-    'Change declared parent of current branch.'
+def main():
     args = getargs()
     if args:
         newparent, = args
     else:
         newparent = getpublic()
         if newparent is None:
             raise Exception('Please specify a branch to be parent.')
     addparents(thisbranch(), newparent, clobber = True)
+
+if '__main__' == __name__:
+    main()
```

### Comparing `Leytonium-8/leytonium/taskding.py` & `Leytonium-9/leytonium/taskding.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with Leytonium.  If not, see <http://www.gnu.org/licenses/>.
 
+'Play a sound when a long-running child of shell terminates.'
 from argparse import ArgumentParser
 from aridity.config import ConfigCtrl
 from diapyr.util import innerclass
 from lagoon import pgrep
 from lagoon.program import bg
 from pathlib import Path
 import os, subprocess, time
@@ -44,37 +45,48 @@
                     self.armed = f.read().rstrip() not in self.always_interactive
                     return True
             except (FileNotFoundError, ProcessLookupError):
                 pass
 
         def fire(self, now):
             from lagoon import paplay
-            if self.start + self.threshold <= now and self.armed and self.sound_path.exists() and not os.fork():
-                paplay[exec](self.sound_path) # FIXME: These leak as zombie processes.
+            if self.start + self.threshold <= now and self.armed and self.sound_path.exists():
+                pid = os.fork()
+                if pid:
+                    return pid
+                paplay[exec](self.sound_path)
 
     def run(self):
         children = {}
+        soundpids = set()
         while True:
             nowchildren = {}
             now = time.time()
             try:
                 with pgrep[bg]('-P', self.shpidstr) as stdout:
                     for line in stdout:
                         nowchildren[int(line)] = self.Child(now)
             except subprocess.CalledProcessError:
                 break
+            for pid in soundpids - nowchildren.keys():
+                os.waitpid(pid, 0)
+            soundpids &= nowchildren.keys()
             for pid in children.keys() - nowchildren.keys():
-                children.pop(pid).fire(now)
+                q = children.pop(pid).fire(now)
+                if q is not None:
+                    soundpids.add(q)
             for pid, child in nowchildren.items():
                 if pid not in children and child.fetch(pid):
                     children[pid] = child
             time.sleep(self.sleep_time) # FIXME LATER: I suspect keyboard interrupt can kill script when not asleep.
 
-def main_taskding():
-    'Play a sound when a long-running child of shell terminates.'
+def main():
     if 'SSH_CLIENT' in os.environ:
         return
-    config = ConfigCtrl().loadappconfig(main_taskding, 'taskding.arid')
+    config = ConfigCtrl().loadappconfig(main, 'taskding.arid')
     parser = ArgumentParser()
     parser.add_argument('shpidstr')
     parser.parse_args(namespace = config)
     TaskDing(config).run()
+
+if '__main__' == __name__:
+    main()
```

### Comparing `Leytonium-8/leytonium/prepare.py` & `Leytonium-9/leytonium/prepare.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,23 +11,26 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with Leytonium.  If not, see <http://www.gnu.org/licenses/>.
 
+'Create a master-based branch from this non-master-based one.'
 from .common import thisbranch, pb, AllBranches, addparents
 from lagoon import git, ren
 
-def main_prepare():
-    'Create a master-based branch from this non-master-based one.'
+def main():
     master = 'master'
     parent = pb()
     if parent == master:
         raise Exception(f"Parent is already {master}!")
     name = thisbranch()
     allbranches = AllBranches()
     commits = [commit for commit, _ in allbranches.branchcommits(name)]
     ren[print](f"{name}.bak")
     git.checkout._b[print](name, master)
     addparents(name, master)
     git.cherry_pick[print](*commits)
+
+if '__main__' == __name__:
+    main()
```

### Comparing `Leytonium-8/leytonium/unpub.py` & `Leytonium-9/leytonium/unpub.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,14 +11,17 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with Leytonium.  If not, see <http://www.gnu.org/licenses/>.
 
+'Unpublish this branch.'
 from .common import thisbranch
 from lagoon import git
 
-def main_unpub():
-    'Unpublish this branch.'
+def main():
     git.push.origin.__delete[print](thisbranch(), check = False) # Idempotent.
     git.branch.__unset_upstream[exec]()
+
+if '__main__' == __name__:
+    main()
```

### Comparing `Leytonium-8/leytonium/scrape85.py` & `Leytonium-9/leytonium/scrape85.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,22 +11,25 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with Leytonium.  If not, see <http://www.gnu.org/licenses/>.
 
+'Extract Adobe Ascii85-encoded images from given file.'
 import sys, re, base64, os
 
 pattern = re.compile('<~(.+?)~>', re.DOTALL)
 
-def main_scrape85():
-    'Extract Adobe Ascii85-encoded images from given file.'
+def main():
     if os.listdir():
         raise Exception
     path, = sys.argv[1:]
     with open(path) as f:
         text = f.read()
     for i, image in enumerate(pattern.findall(text)):
         print(i)
         with open(f"{i}.png", 'wb') as g:
             g.write(base64.a85decode(image))
+
+if '__main__' == __name__:
+    main()
```

### Comparing `Leytonium-8/leytonium/delegate.py` & `Leytonium-9/leytonium/delegate.py`

 * *Files identical despite different names*

### Comparing `Leytonium-8/leytonium/refactor.py` & `Leytonium-9/leytonium/agi.py`

 * *Files 24% similar despite different names*

```diff
@@ -11,25 +11,17 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with Leytonium.  If not, see <http://www.gnu.org/licenses/>.
 
+'Search for identifier in project.'
 from .common import findproject
 from lagoon import ag
-from lagoon.program import Program
-import os, sys
+import sys
 
-def main_agi():
-    'Search for identifier in project.'
+def main():
     ag._ws[exec](*sys.argv[1:], findproject())
 
-def main_agil():
-    'Edit project files containing identifier.'
-    search = sys.argv[1:]
-    editor = os.environ['EDITOR']
-    if 1 == len(search) and 'vim' == editor:
-        args = [rf"+/\<{search[0]}\>"]
-    else:
-        args = []
-    Program.text(editor)[exec](*args, *ag._wsl(*search, findproject()).splitlines())
+if '__main__' == __name__:
+    main()
```

### Comparing `Leytonium-8/leytonium/spamtrash.arid` & `Leytonium-9/leytonium/spamtrash.arid`

 * *Files identical despite different names*

### Comparing `Leytonium-8/leytonium/slam.py` & `Leytonium-9/leytonium/slam.py`

 * *Files 24% similar despite different names*

```diff
@@ -11,21 +11,20 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with Leytonium.  If not, see <http://www.gnu.org/licenses/>.
 
-from .common import AllBranches, showmenu, pb, savecommits, savedcommits, findproject, thisbranch, infodirname, os, stderr
+'Reset branch to given commit number.'
+from .common import AllBranches, showmenu, pb, savecommits, savedcommits
 from lagoon import git
-from lagoon.program import partial
 import sys
 
-def main_slam():
-    'Reset branch to given commit number.'
+def main():
     items = AllBranches().branchcommits() + [[pb(), '']]
     # TODO: Use argparse.
     args = sys.argv[1:]
     if '-f' == args[0]:
         save = False
         n, = args[1:]
     else:
@@ -41,17 +40,9 @@
         saved = savedcommits()
         i = len(saved) - 1 + n
         commit = saved[i]
         if save:
             savecommits(saved[:i], True)
         git.cherry_pick[exec](*reversed(saved[i:]))
 
-def main_unslam():
-    'Cherry-pick commits lost in a previous slam.'
-    path = os.path.join(findproject(), infodirname, f"{thisbranch()} slammed")
-    with open(path) as f:
-        commits = f.read().splitlines()
-    commits.reverse()
-    command = git.cherry_pick[partial](*commits)
-    stderr(f"Command: git {' '.join(command.args)}")
-    os.remove(path)
-    command[exec]()
+if '__main__' == __name__:
+    main()
```

### Comparing `Leytonium-8/leytonium/watchdesk.py` & `Leytonium-9/leytonium/watchdesk.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,30 +11,33 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with Leytonium.  If not, see <http://www.gnu.org/licenses/>.
 
+'Different background for each desktop.'
 from aridity.config import ConfigCtrl
 from lagoon import gsettings, xprop
 from lagoon.program import bg
 from pathlib import Path
 import logging, re
 
 log = logging.getLogger(__name__)
 number = re.compile('[0-9]+')
 
-def main_watchdesk():
-    'Different background for each desktop.'
-    config = ConfigCtrl().loadappconfig(main_watchdesk, 'watchdesk.arid').path
+def main():
+    config = ConfigCtrl().loadappconfig(main, 'watchdesk.arid').path
     with xprop._root._spy[bg]('_NET_CURRENT_DESKTOP') as f:
         for line in f:
             m = number.search(line)
             if m is not None:
                 key = str(1 + int(m.group()))
                 try:
                     path = getattr(config, key)
                 except AttributeError:
                     log.exception('No such path:')
                 else:
                     gsettings.set[print]('org.gnome.desktop.background', 'picture-uri', Path(path).as_uri())
+
+if '__main__' == __name__:
+    main()
```

### Comparing `Leytonium-8/leytonium/upgrade.py` & `Leytonium-9/leytonium/upgrade.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,25 +11,25 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with Leytonium.  If not, see <http://www.gnu.org/licenses/>.
 
+'Upgrade the system and silence the nag.'
 from . import initlogging
 from argparse import ArgumentParser
 from lagoon import docker, sudo
 from pathlib import Path
 import logging
 
 log = logging.getLogger(__name__)
 boot = Path('/boot')
 
-def main_upgrade():
-    'Upgrade the system and silence the nag.'
+def main():
     initlogging()
     parser = ArgumentParser()
     parser.add_argument('-k', action = 'store_true', help = 'first remove all kernels except old and current')
     args = parser.parse_args()
     apt_get = sudo.apt_get[print]
     if args.k:
         keep = {(boot / name).resolve() for name in ['vmlinuz.old', 'vmlinuz']}
@@ -39,7 +39,10 @@
     apt_get.__with_new_pkgs.upgrade()
     apt_get.autoremove()
     touchpath = Path.home() / 'var' / 'last-upgrade'
     touchpath.parent.mkdir(parents = True, exist_ok = True)
     touchpath.write_text('')
     log.info('Containers still up:')
     docker.ps[print]()
+
+if '__main__' == __name__:
+    main()
```

### Comparing `Leytonium-8/leytonium/halp.arid` & `Leytonium-9/leytonium/halp.arid`

 * *Files identical despite different names*

### Comparing `Leytonium-8/leytonium/squash.bash` & `Leytonium-9/leytonium/squash.bash`

 * *Files identical despite different names*

### Comparing `Leytonium-8/leytonium/stmulti.py` & `Leytonium-9/leytonium/stmulti.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with Leytonium.  If not, see <http://www.gnu.org/licenses/>.
 
+'Short status of all shallow projects in directory.'
 from . import effectivehome
 from aridity.config import ConfigCtrl
 from lagoon import clear, co, git, hg, hgcommit, md5sum, rsync, test, tput
 try:
     from lagoon import gfind as find
 except ImportError:
     from lagoon import find
@@ -184,28 +185,18 @@
 
     def status(self):
         tput.setaf[print](4)
         tput.bold[print]()
         self.find._newer[print](self.dirname)
         tput.sgr0[print]()
 
-def main(action):
+def mainimpl(action):
     config = loadconfig()
     clear[print]()
     for projecttype in Mercurial, Git, Rsync:
         projecttype.forprojects(config, action)
 
-def main_stmulti():
-    'Short status of all shallow projects in directory.'
-    main('status')
-
-def main_fetchall():
-    'Fetch all remotes of projects in directory.'
-    main('fetch')
-
-def main_pullall():
-    'Pull all branches of projects in directory.'
-    main('pull')
-
-def main_pushall():
-    'Push (using hgcommit) all branches of projects in directory.'
-    main('push')
+def main():
+    mainimpl('status')
+
+if '__main__' == __name__:
+    main()
```

### Comparing `Leytonium-8/leytonium/splitpkgs.py` & `Leytonium-9/leytonium/splitpkgs.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,24 +11,24 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with Leytonium.  If not, see <http://www.gnu.org/licenses/>.
 
+'Show packages that exist in more than one module.'
 import os
 
 def relativise(context, path):
     if context == path:
         return []
     else:
         return path[len(context + os.sep):].split(os.sep)
 
-def main_splitpkgs():
-    'Show packages that exist in more than one module.'
+def main():
     packagetomodules = {}
     def register(module, package):
         try:
             packagetomodules[package].add(module)
         except KeyError:
             packagetomodules[package] = set([module])
     def findpackages(langpath):
@@ -54,7 +54,10 @@
             process(''.join(f":{w}" for w in relativise(projectpath, dirpath)), dirpath)
         dirnames.sort()
     for package, modules in sorted(packagetomodules.items()):
         if 1 != len(modules):
             print(package)
             for m in modules:
                 print(f"\t{m}")
+
+if '__main__' == __name__:
+    main()
```

### Comparing `Leytonium-8/leytonium/drclean.bash` & `Leytonium-9/leytonium/drclean.bash`

 * *Files identical despite different names*

### Comparing `Leytonium-8/leytonium/extractaudio.py` & `Leytonium-9/leytonium/extractaudio.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,30 +11,33 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with Leytonium.  If not, see <http://www.gnu.org/licenses/>.
 
+'Extract the audio from the given video files.'
 from . import initlogging
 from argparse import ArgumentParser
 from lagoon import ffmpeg
 from lagoon.program import partial
 from pathlib import Path
 import logging
 
 log = logging.getLogger(__name__)
 
-def main_extractaudio():
-    'Extract the audio from the given video files.'
+def main():
     initlogging()
     parser = ArgumentParser()
     parser.add_argument('-d', action = 'store_true')
     parser.add_argument('path', nargs = '+', type = Path)
     args = parser.parse_args()
     for inpath in args.path:
         outpath = inpath.with_suffix('.aac')
         log.info("Extract: %s", outpath)
         ffmpeg._i[partial](inpath)._vn._acodec.copy(outpath)
         if args.d:
             log.info("Delete: %s", inpath)
             inpath.unlink()
+
+if '__main__' == __name__:
+    main()
```

### Comparing `Leytonium-8/leytonium/autopull.py` & `Leytonium-9/leytonium/rol.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,17 +11,25 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with Leytonium.  If not, see <http://www.gnu.org/licenses/>.
 
-from .common import nicely, publicbranches
-from lagoon import git
+'Move given slammed commit (default top) to the bottom.'
+from .common import savedcommits, savecommits, args as getargs
 
-def main_autopull():
-    'Pull master and releases with automatic stash and switch.'
-    def pullthem():
-        for b in publicbranches():
-            git.checkout[print](b)
-            git.pull[print]()
-    nicely(pullthem)
+def main():
+    v = savedcommits()
+    args = getargs()
+    if args:
+        n, = args
+        n = int(n)
+        if n < 0:
+            raise Exception("Don't bother with the minus.")
+        i = len(v) - int(n) - 1
+    else:
+        i = 0
+    savecommits(v[:i] + v[i + 1:] + [v[i]], True)
+
+if '__main__' == __name__:
+    main()
```

### Comparing `Leytonium-8/leytonium/brown.py` & `Leytonium-9/leytonium/brown.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,23 +11,23 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with Leytonium.  If not, see <http://www.gnu.org/licenses/>.
 
+'Satisfy PEP 8 with minimal impact.'
 from .common import findproject
 from aridity.config import ConfigCtrl
 from lagoon import autopep8, sed
 from lagoon.program import partial
 import re, subprocess, sys
 
-def main_brown():
-    'Satisfy PEP 8 with minimal impact.'
-    config = ConfigCtrl().loadappconfig(main_brown, 'common.arid')
+def main():
+    config = ConfigCtrl().loadappconfig(main, 'common.arid')
     roots = sys.argv[1:]
     if not roots:
         roots = [findproject()]
     brown(config.cols, roots)
 
 def brown(cols, paths):
     command = autopep8._rv[partial]('--max-line-length', cols, *paths)
@@ -35,7 +35,10 @@
     def paths():
         for line in result.splitlines():
             m = re.fullmatch(r'\[file:(.+)]', line)
             if m is not None:
                 yield m.group(1)
     sed._ni[print](r'/\S/p', *paths())
     command._i[print]()
+
+if '__main__' == __name__:
+    main()
```

### Comparing `Leytonium-8/leytonium/gt.py` & `Leytonium-9/leytonium/gt.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,25 +11,28 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with Leytonium.  If not, see <http://www.gnu.org/licenses/>.
 
-from . import st
-from .brown import main_brown, brown
+'Stage all outgoing changes and show them.'
+from . import brown, st
 from .common import findproject
 from aridity.config import ConfigCtrl
+from aridity.util import dotpy
 from lagoon import git
 from pathlib import Path
 
-def main_gt():
-    'Stage all outgoing changes and show them.'
-    config = (-ConfigCtrl().loadappconfig(main_brown, 'common.arid')).reapplysettings(main_gt)
+def main():
+    config = (-ConfigCtrl().loadappconfig(brown.main, 'common.arid')).reapplysettings(main)
     projectdir = Path(findproject()).resolve()
     paths = [projectdir / line[line.index("'") + 1:-1] for line in git.add._n(projectdir).splitlines()]
     if projectdir.name in config.formattedprojects:
-        toformat = [path for path in paths if path.exists() and path.name.endswith('.py')]
+        toformat = [path for path in paths if path.exists() and path.name.endswith(dotpy)]
         if toformat:
-            brown(config.cols, toformat)
+            brown.brown(config.cols, toformat)
     git.add[print](*paths)
-    st.main_st()
+    st.main()
+
+if '__main__' == __name__:
+    main()
```

### Comparing `Leytonium-8/leytonium/touchb.py` & `Leytonium-9/leytonium/touchb.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,18 +11,21 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with Leytonium.  If not, see <http://www.gnu.org/licenses/>.
 
+'Give the current branch its own identity.'
 from .common import touchmsg, findproject, thisbranch
 from lagoon import git
 import os, time
 
-def main_touchb():
-    'Give the current branch its own identity.'
+def main():
     path = os.path.join(findproject(), 'TOUCHME')
     with open(path, 'w') as f:
         print(f"{time.strftime('%c %Z')} {thisbranch()}", file = f)
     git.add[print](path)
     git.commit._m[print](touchmsg())
+
+if '__main__' == __name__:
+    main()
```

### Comparing `Leytonium-8/leytonium/readjust.py` & `Leytonium-9/leytonium/d.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with Leytonium.  If not, see <http://www.gnu.org/licenses/>.
 
-from lagoon import sudo
+'Show local changes.'
+from lagoon import clear, git
 
-def main_readjust():
-    'Set system clock to correct time.'
-    sudo[print].service.ntp.stop()
-    sudo[print].ntpd._gq()
-    sudo[print].service.ntp.start()
+def main():
+    clear[print]()
+    git.diff[print]()
+
+if '__main__' == __name__:
+    main()
```

### Comparing `Leytonium-8/leytonium/multimerge.py` & `Leytonium-9/leytonium/multimerge.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with Leytonium.  If not, see <http://www.gnu.org/licenses/>.
 
+'Merge master into all PRs and carrion.'
 from .common import findproject, nicely, AllBranches, getpublic, stderr, touchmsg
 from lagoon import git, touchb
 import os
 
 merge = git.merge.__no_edit
 
 def reportornone(b):
@@ -94,11 +95,13 @@
         remaining2 = [b for b, _ in status]
         if remaining2 == remaining:
             for b, deps in status:
                 stderr(f"{b}: {' '.join(deps)}")
             raise Exception(f"Still remain: {remaining}")
         remaining = remaining2
 
-def main_multimerge():
-    'Merge master into all PRs and carrion.'
+def main():
     os.chdir(findproject()) # Don't fail if working directory doesn't exist in some branch.
     nicely(multimerge)
+
+if '__main__' == __name__:
+    main()
```

### Comparing `Leytonium-8/leytonium/dp.py` & `Leytonium-9/leytonium/pd.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,22 +11,19 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with Leytonium.  If not, see <http://www.gnu.org/licenses/>.
 
+'Diff from public branch, the other way.'
 from .common import getpublic, stderr
 from lagoon import git
 import sys
 
-def main_dp():
-    'Diff from public branch.'
-    parent = getpublic()
-    stderr(f"Public branch: {parent}")
-    git.diff._M25[exec](*sys.argv[1:], parent)
-
-def main_pd():
-    'Diff from public branch, the other way.'
+def main():
     parent = getpublic()
     stderr(f"Public branch: {parent}")
     git.diff._M25[exec](*sys.argv[1:], 'HEAD', parent)
+
+if '__main__' == __name__:
+    main()
```

### Comparing `Leytonium-8/leytonium/st.py` & `Leytonium-9/leytonium/st.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with Leytonium.  If not, see <http://www.gnu.org/licenses/>.
 
+'Show list of branches and outgoing changes.'
 from .common import showmenu, UnknownParentException, showexception, stripansi, getpublic, savedcommits, AllBranches, highlight
 from lagoon import clear, git
 try:
     from lagoon import gls as ls
 except ImportError:
     from lagoon import ls
 from termcolor import colored
@@ -47,16 +48,15 @@
 
     def colorline(self, ispr):
         return colored(self.line, 'green', attrs = ['reverse']) if ispr else self.line
 
 def title(commit):
     return git.log('-n', 1, '--pretty=format:%B', commit).splitlines()[0]
 
-def main_st():
-    'Show list of branches and outgoing changes.'
+def main():
     clear[print]()
     try:
         allbranches = AllBranches()
     except subprocess.CalledProcessError:
         ls._l[print]('--color=always')
         return
     rows = [Row(allbranches, l[2:]) for l in git('-c', 'color.ui=always', 'branch', '-vv').splitlines()]
@@ -71,7 +71,10 @@
         count = len(entries) - limit
         if count > 0:
             print(f"({count} more)")
     except UnknownParentException:
         showexception()
     git.status._v[print](check = False)
     git.stash.list[print]()
+
+if '__main__' == __name__:
+    main()
```

### Comparing `Leytonium-8/leytonium/rol.py` & `Leytonium-9/leytonium/unslam.py`

 * *Files 24% similar despite different names*

```diff
@@ -11,22 +11,24 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with Leytonium.  If not, see <http://www.gnu.org/licenses/>.
 
-from .common import savedcommits, savecommits, args as getargs
+'Cherry-pick commits lost in a previous slam.'
+from .common import findproject, thisbranch, infodirname, os, stderr
+from lagoon import git
+from lagoon.program import partial
 
-def main_rol():
-    'Move given slammed commit (default top) to the bottom.'
-    v = savedcommits()
-    args = getargs()
-    if args:
-        n, = args
-        n = int(n)
-        if n < 0:
-            raise Exception("Don't bother with the minus.")
-        i = len(v) - int(n) - 1
-    else:
-        i = 0
-    savecommits(v[:i] + v[i + 1:] + [v[i]], True)
+def main():
+    path = os.path.join(findproject(), infodirname, f"{thisbranch()} slammed")
+    with open(path) as f:
+        commits = f.read().splitlines()
+    commits.reverse()
+    command = git.cherry_pick[partial](*commits)
+    stderr(f"Command: git {' '.join(command.args)}")
+    os.remove(path)
+    command[exec]()
+
+if '__main__' == __name__:
+    main()
```

### Comparing `Leytonium-8/leytonium/examine.bash` & `Leytonium-9/leytonium/examine.bash`

 * *Files identical despite different names*

### Comparing `Leytonium-8/leytonium/next.py` & `Leytonium-9/leytonium/next.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,20 +11,20 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with Leytonium.  If not, see <http://www.gnu.org/licenses/>.
 
+'Go to next step in current git workflow.'
 from lagoon import git
 from lagoon.program import NOEOL
 from pathlib import Path
 
-def main_next():
-    'Go to next step in current git workflow.'
+def main():
     gitdir = Path(git.rev_parse.__git_dir[NOEOL]())
     if (gitdir / 'rebase-apply').is_dir():
         if git.status.__porcelain().splitlines():
             git[print].rebase.__continue()
         else:
             git[print].rebase.__skip()
     elif (gitdir / 'MERGE_HEAD').is_file():
@@ -33,7 +33,10 @@
         git[print].cherry_pick.__continue()
     elif (gitdir / 'REVERT_HEAD').is_file():
         git[print].revert.__continue()
     elif (gitdir / 'sequencer').is_dir():
         git[print].cherry_pick.__continue()
     else:
         raise Exception('Unknown git workflow, giving up.')
+
+if '__main__' == __name__:
+    main()
```

### Comparing `Leytonium-8/leytonium/abandon.py` & `Leytonium-9/leytonium/abandon.py`

 * *Files 21% similar despite different names*

```diff
@@ -11,14 +11,17 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with Leytonium.  If not, see <http://www.gnu.org/licenses/>.
 
+'Discard all local changes, with confirmation step.'
 from lagoon import git
 
-def main_abandon():
-    'Discard all local changes, with confirmation step.'
+def main():
     git.status[print]()
     input('Press enter to permanently lose all these changes.')
     git.reset.__hard[print]()
+
+if '__main__' == __name__:
+    main()
```

### Comparing `Leytonium-8/leytonium/common.arid` & `Leytonium-9/leytonium/common.arid`

 * *Files identical despite different names*

### Comparing `Leytonium-8/leytonium/br.py` & `Leytonium-9/leytonium/autopull.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,16 +11,20 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with Leytonium.  If not, see <http://www.gnu.org/licenses/>.
 
-from .common import addparents, args, AllBranches, menu
+'Pull master and releases with automatic stash and switch.'
+from .common import nicely, publicbranches
 from lagoon import git
 
-def main_br():
-    'Create given branch with completion and dashes, show menu for parent.'
-    _, base = menu([[n, ''] for n in AllBranches().names], 'From')
-    name = '-'.join(args())
-    git.checkout._b[print](name, base)
-    addparents(name, base)
+def main():
+    def pullthem():
+        for b in publicbranches():
+            git.checkout[print](b)
+            git.pull[print]()
+    nicely(pullthem)
+
+if '__main__' == __name__:
+    main()
```

### Comparing `Leytonium-8/leytonium/co.py` & `Leytonium-9/leytonium/co.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,17 +11,20 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with Leytonium.  If not, see <http://www.gnu.org/licenses/>.
 
+'Switch to the given branch, with completion.'
 from .common import args, AllBranches, addparents, getpublic
 from lagoon import git
 
-def main_co():
-    'Switch to the given branch, with completion.'
+def main():
     name, = args()
     new = name not in AllBranches().names
     git.checkout[print](name)
     if new:
         addparents(name, getpublic())
+
+if '__main__' == __name__:
+    main()
```

### Comparing `Leytonium-8/leytonium/dx.py` & `Leytonium-9/leytonium/dxx.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,32 +11,20 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with Leytonium.  If not, see <http://www.gnu.org/licenses/>.
 
+'Short diff from parent branch or of passed-in commit number.'
 from .common import AllBranches, pb, savedcommits, showmenu, stderr
 from lagoon import git
 import sys
 
-def main_dx():
-    'Diff from parent branch or from passed-in commit number.'
-    args = sys.argv[1:]
-    if args:
-        n, = args
-        n = int(n)
-        parent = showmenu(AllBranches().branchcommits(), False)[n]
-    else:
-        parent = pb()
-        stderr(f"Parent branch: {parent}")
-    git.diff._M25[exec](parent)
-
-def main_dxx():
-    'Short diff from parent branch or of passed-in commit number.'
+def main():
     args = sys.argv[1:]
     if args:
         n, = args
         n = int(n)
         if n > 0:
             commit = showmenu(AllBranches().branchcommits(), False)[n]
         else:
@@ -44,7 +32,10 @@
             commit = saved[len(saved) - 1 + n]
         commits = f"{commit}^", commit
     else:
         parent = pb()
         stderr(f"Parent branch: {parent}")
         commits = parent,
     git.diff._M25.__name_status[exec](*commits)
+
+if '__main__' == __name__:
+    main()
```

### Comparing `Leytonium-8/leytonium/spamtrash.py` & `Leytonium-9/leytonium/spamtrash.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with Leytonium.  If not, see <http://www.gnu.org/licenses/>.
 
+'Delete spam emails.'
 from . import initlogging
 from argparse import ArgumentParser
 from aridity.config import ConfigCtrl
 from email import message_from_bytes
 from itertools import islice
 from unidecode import unidecode
 import logging, re
@@ -70,18 +71,17 @@
         if Subject is not None:
             plain = _toplain(Subject)
             for subjectre in self.subjects:
                 if subjectre.search(plain) is not None:
                     log.debug("Subject match: %s", subjectre)
                     return True
 
-def main_spamtrash():
-    'Delete spam emails.'
+def main():
     initlogging()
-    config = ConfigCtrl().loadappconfig(main_spamtrash, 'spamtrash.arid', encoding = 'utf-8')
+    config = ConfigCtrl().loadappconfig(main, 'spamtrash.arid', encoding = 'utf-8')
     parser = ArgumentParser()
     parser.add_argument('--cron', action = 'store_true')
     parser.add_argument('-v', action = 'store_true')
     parser.parse_args(namespace = config.cli)
     logging.getLogger().setLevel(logging.DEBUG if config.verbose else logging.INFO)
     regex = Regex(config)
     with config.imap(config.host) as imap:
@@ -109,7 +109,10 @@
             else:
                 log.info("Ignore %s: %s", id, msg)
         if deleteids:
             log.info("Delete %s emails.", len(deleteids))
             imap.store(','.join(deleteids), '+X-GM-LABELS', r'\Trash')
         else:
             log.info('Nothing to delete.')
+
+if '__main__' == __name__:
+    main()
```

### Comparing `Leytonium-8/leytonium/git_completion.bash` & `Leytonium-9/leytonium/git_completion.bash`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-. "$(git-functions-path)"
+. "$(~/.local/bin/git-functions-path)"
 
 function _allbranches {
     local branches="$(git branch | cut -c 3-)"
     COMPREPLY=($(compgen -W "$branches" $2))
 }
 
 function _otherbranches {
```

### Comparing `Leytonium-8/leytonium/shove.py` & `Leytonium-9/leytonium/shove.py`

 * *Files 21% similar despite different names*

```diff
@@ -11,21 +11,25 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with Leytonium.  If not, see <http://www.gnu.org/licenses/>.
 
+'Update a latest tag in ECR with the given image.'
 import sys, subprocess, re
 
 pattern = re.compile('latest|.+[.]latest')
 
-def main_shove():
-    'Update a latest tag in ECR with the given image.'
+def main():
     spec, = sys.argv[1:]
     slash = spec.index('/')
     colon = spec.rindex(':')
     tag = spec[colon + 1:]
     if pattern.fullmatch(tag) is None:
         raise Exception('REFUSAL!')
+    # TODO: Do not use interactive mode.
     subprocess.check_call(['bash', '-ic', 'aws ecr batch-delete-image --repository-name "$1" --image-ids "$2"', 'ecr', spec[slash + 1:colon], f"imageTag={tag}"])
     subprocess.check_call(['docker', 'push', spec])
+
+if '__main__' == __name__:
+    main()
```

### Comparing `Leytonium-8/leytonium/awslogs.py` & `Leytonium-9/leytonium/awslogs.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,19 +11,20 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with Leytonium.  If not, see <http://www.gnu.org/licenses/>.
 
+'Reconstruct logs from AWS CloudWatch.'
 from lagoon.binary import bash, date
 from lagoon.program import partial
 import argparse, json
 
-logs = bash._ic[partial]('aws logs "$@"', 'logs')
+logs = bash._ic[partial]('aws logs "$@"', 'logs') # TODO: Do not use interactive mode.
 tskey = 'lastIngestionTime'
 
 def _shorten(line, radius = 250):
     if len(line) <= 2 * radius:
         return line
     sep = '...'
     return line[:radius - len(sep)] + sep + line[-radius:]
@@ -36,16 +37,15 @@
             if s.get(tskey, 0) < starttime:
                 break
             yield s['logStreamName']
     names = list(g())
     names.reverse()
     return names
 
-def main_awslogs():
-    'Reconstruct logs from AWS CloudWatch.'
+def main():
     parser = argparse.ArgumentParser()
     parser.add_argument('--no-trunc', action='store_true')
     parser.add_argument('--ago', default='1 hour')
     parser.add_argument('group')
     config = parser.parse_args()
     shorten = (lambda x: x) if config.no_trunc else _shorten
     for stream in streamnames(config.group, int(date('-d', f"{config.ago} ago", '+%s000'))):
@@ -61,7 +61,10 @@
                         print()
                         print('> ', end = '')
                     print(shorten(l), end = '')
             t = page['nextForwardToken']
             if token and t == token[1]: # Looks like first page can never be final page.
                 break
             token = ['--next-token', t]
+
+if '__main__' == __name__:
+    main()
```

### Comparing `Leytonium-8/leytonium/__init__.py` & `Leytonium-9/leytonium/readjust.py`

 * *Files 24% similar despite different names*

```diff
@@ -11,14 +11,17 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with Leytonium.  If not, see <http://www.gnu.org/licenses/>.
 
-from pathlib import Path
-import logging, os
+'Set system clock to correct time.'
+from lagoon import sudo
 
-effectivehome = Path(f"~{os.environ.get('SUDO_USER', '')}").expanduser()
+def main():
+    sudo[print].service.ntp.stop()
+    sudo[print].ntpd._gq()
+    sudo[print].service.ntp.start()
 
-def initlogging():
-    logging.basicConfig(level = logging.DEBUG, format = "%(asctime)s %(levelname)s %(message)s")
+if '__main__' == __name__:
+    main()
```

### Comparing `Leytonium-8/leytonium/halp.py` & `Leytonium-9/leytonium/halp.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,26 +11,26 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with Leytonium.  If not, see <http://www.gnu.org/licenses/>.
 
+'''You're looking at it!'''
 from . import initlogging
 from aridity.config import ConfigCtrl
 from importlib import import_module
 from importlib_metadata import entry_points
 import logging
 
 log = logging.getLogger(__name__)
 
-def main_halp():
-    '''You're looking at it!'''
+def main():
     initlogging()
-    config = ConfigCtrl().loadappconfig(main_halp, 'halp.arid')
+    config = ConfigCtrl().loadappconfig(main, 'halp.arid')
     ignore_projects = set(config.ignore.projects)
     projects = set(config.projects)
     others = set()
     undocumented = set()
     halps = []
     for ep in entry_points()['console_scripts']:
         project = ep.dist.name
@@ -49,7 +49,10 @@
             others.add(project)
     if others:
         log.debug("Other projects: %s", ' '.join(sorted(others)))
     log.debug("Undocumented commands: %s", ' '.join(sorted(undocumented)))
     format = "%%-%ss %%s" % max(len(halp[0]) for halp in halps)
     for halp in sorted(halps):
         print(format % halp)
+
+if '__main__' == __name__:
+    main()
```

### Comparing `Leytonium-8/leytonium/git_functions.bash` & `Leytonium-9/leytonium/git_functions.bash`

 * *Files identical despite different names*

### Comparing `Leytonium-8/leytonium/taskding.arid` & `Leytonium-9/leytonium/taskding.arid`

 * *Files identical despite different names*

