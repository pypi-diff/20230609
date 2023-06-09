# Comparing `tmp/dimples-0.1.6.tar.gz` & `tmp/dimples-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dimples-0.1.6.tar", last modified: Fri Jun  9 15:09:56 2023, max compression
+gzip compressed data, was "dist/dimples-0.1.7.tar", last modified: Fri Jun  9 17:20:51 2023, max compression
```

## Comparing `dimples-0.1.6.tar` & `dimples-0.1.7.tar`

### file list

```diff
@@ -1,137 +1,138 @@
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-09 15:09:56.000000 dimples-0.1.6/
--rw-r--r--   0 moky       (501) staff       (20)     1061 2023-06-09 15:09:56.000000 dimples-0.1.6/PKG-INFO
--rw-r--r--   0 moky       (501) staff       (20)      568 2022-12-11 05:07:49.000000 dimples-0.1.6/README.md
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-09 15:09:56.000000 dimples-0.1.6/dimples/
--rw-r--r--   0 moky       (501) staff       (20)     7071 2023-06-03 12:10:17.000000 dimples-0.1.6/dimples/__init__.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-09 15:09:56.000000 dimples-0.1.6/dimples/client/
--rw-r--r--   0 moky       (501) staff       (20)     1997 2023-06-03 11:38:39.000000 dimples-0.1.6/dimples/client/__init__.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-09 15:09:56.000000 dimples-0.1.6/dimples/client/cpu/
--rw-r--r--   0 moky       (501) staff       (20)     2122 2023-01-31 05:28:07.000000 dimples-0.1.6/dimples/client/cpu/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     4011 2023-06-02 18:30:20.000000 dimples-0.1.6/dimples/client/cpu/grp_expel.py
--rw-r--r--   0 moky       (501) staff       (20)     4116 2023-06-02 18:31:07.000000 dimples-0.1.6/dimples/client/cpu/grp_invite.py
--rw-r--r--   0 moky       (501) staff       (20)     3554 2023-02-23 11:18:06.000000 dimples-0.1.6/dimples/client/cpu/grp_query.py
--rw-r--r--   0 moky       (501) staff       (20)     3558 2023-06-02 18:31:36.000000 dimples-0.1.6/dimples/client/cpu/grp_quit.py
--rw-r--r--   0 moky       (501) staff       (20)     6498 2023-06-02 18:32:15.000000 dimples-0.1.6/dimples/client/cpu/grp_reset.py
--rw-r--r--   0 moky       (501) staff       (20)     5150 2023-02-23 14:17:47.000000 dimples-0.1.6/dimples/client/cpu/handshake.py
--rw-r--r--   0 moky       (501) staff       (20)     2948 2023-01-31 05:28:07.000000 dimples-0.1.6/dimples/client/cpu/history.py
--rw-r--r--   0 moky       (501) staff       (20)     1869 2023-01-31 05:28:07.000000 dimples-0.1.6/dimples/client/cpu/login.py
--rw-r--r--   0 moky       (501) staff       (20)     1847 2023-01-31 05:28:07.000000 dimples-0.1.6/dimples/client/cpu/receipt.py
--rw-r--r--   0 moky       (501) staff       (20)    16324 2023-06-02 17:03:56.000000 dimples-0.1.6/dimples/client/group.py
--rw-r--r--   0 moky       (501) staff       (20)     7713 2023-06-06 16:33:40.000000 dimples-0.1.6/dimples/client/messenger.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-09 15:09:56.000000 dimples-0.1.6/dimples/client/network/
--rw-r--r--   0 moky       (501) staff       (20)     3246 2023-02-23 14:19:20.000000 dimples-0.1.6/dimples/client/network/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     6258 2023-02-23 14:14:03.000000 dimples-0.1.6/dimples/client/network/session.py
--rw-r--r--   0 moky       (501) staff       (20)     8302 2023-06-03 11:39:42.000000 dimples-0.1.6/dimples/client/network/state.py
--rw-r--r--   0 moky       (501) staff       (20)     9531 2023-01-31 05:28:07.000000 dimples-0.1.6/dimples/client/network/transition.py
--rw-r--r--   0 moky       (501) staff       (20)     6560 2023-06-06 16:21:36.000000 dimples-0.1.6/dimples/client/packer.py
--rw-r--r--   0 moky       (501) staff       (20)     6988 2023-01-31 05:28:07.000000 dimples-0.1.6/dimples/client/processor.py
--rw-r--r--   0 moky       (501) staff       (20)     5521 2023-02-23 14:13:41.000000 dimples-0.1.6/dimples/client/terminal.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-09 15:09:56.000000 dimples-0.1.6/dimples/common/
--rw-r--r--   0 moky       (501) staff       (20)     2209 2023-06-06 13:30:28.000000 dimples-0.1.6/dimples/common/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     4322 2023-06-02 08:44:29.000000 dimples-0.1.6/dimples/common/ans.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-09 15:09:56.000000 dimples-0.1.6/dimples/common/dbi/
--rw-r--r--   0 moky       (501) staff       (20)     2324 2023-06-09 14:20:27.000000 dimples-0.1.6/dimples/common/dbi/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     6396 2023-06-02 10:33:41.000000 dimples-0.1.6/dimples/common/dbi/account.py
--rw-r--r--   0 moky       (501) staff       (20)     2465 2023-06-02 07:39:55.000000 dimples-0.1.6/dimples/common/dbi/message.py
--rw-r--r--   0 moky       (501) staff       (20)     7877 2023-06-09 15:01:59.000000 dimples-0.1.6/dimples/common/dbi/session.py
--rw-r--r--   0 moky       (501) staff       (20)     6739 2023-06-02 09:05:19.000000 dimples-0.1.6/dimples/common/facebook.py
--rw-r--r--   0 moky       (501) staff       (20)     7791 2023-06-09 10:25:42.000000 dimples-0.1.6/dimples/common/messenger.py
--rw-r--r--   0 moky       (501) staff       (20)     7918 2023-06-06 16:22:19.000000 dimples-0.1.6/dimples/common/packer.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-09 15:09:56.000000 dimples-0.1.6/dimples/common/protocol/
--rw-r--r--   0 moky       (501) staff       (20)     2536 2023-02-23 09:20:27.000000 dimples-0.1.6/dimples/common/protocol/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     3317 2023-06-02 08:06:32.000000 dimples-0.1.6/dimples/common/protocol/ans.py
--rw-r--r--   0 moky       (501) staff       (20)     5004 2022-12-23 07:24:37.000000 dimples-0.1.6/dimples/common/protocol/handshake.py
--rw-r--r--   0 moky       (501) staff       (20)     4523 2023-06-02 08:11:42.000000 dimples-0.1.6/dimples/common/protocol/login.py
--rw-r--r--   0 moky       (501) staff       (20)     6085 2023-06-02 08:40:15.000000 dimples-0.1.6/dimples/common/protocol/receipt.py
--rw-r--r--   0 moky       (501) staff       (20)     2521 2023-06-02 08:42:45.000000 dimples-0.1.6/dimples/common/protocol/report.py
--rw-r--r--   0 moky       (501) staff       (20)     4486 2023-06-04 16:41:38.000000 dimples-0.1.6/dimples/common/session.py
--rw-r--r--   0 moky       (501) staff       (20)     6211 2023-06-03 12:24:47.000000 dimples-0.1.6/dimples/config.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-09 15:09:56.000000 dimples-0.1.6/dimples/conn/
--rw-r--r--   0 moky       (501) staff       (20)     4449 2023-01-14 13:47:09.000000 dimples-0.1.6/dimples/conn/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)    10335 2023-06-07 13:23:28.000000 dimples-0.1.6/dimples/conn/gate.py
--rw-r--r--   0 moky       (501) staff       (20)     9892 2023-01-31 05:28:07.000000 dimples-0.1.6/dimples/conn/gatekeeper.py
--rw-r--r--   0 moky       (501) staff       (20)    10305 2023-01-14 13:25:42.000000 dimples-0.1.6/dimples/conn/mars.py
--rw-r--r--   0 moky       (501) staff       (20)     7851 2023-02-23 09:10:59.000000 dimples-0.1.6/dimples/conn/mtp.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-09 15:09:56.000000 dimples-0.1.6/dimples/conn/protocol/
--rw-r--r--   0 moky       (501) staff       (20)     1842 2022-12-11 05:07:49.000000 dimples-0.1.6/dimples/conn/protocol/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     8711 2022-12-11 05:07:49.000000 dimples-0.1.6/dimples/conn/protocol/mars.py
--rw-r--r--   0 moky       (501) staff       (20)     8254 2022-12-11 05:07:49.000000 dimples-0.1.6/dimples/conn/protocol/ws.py
--rw-r--r--   0 moky       (501) staff       (20)     5411 2023-02-23 09:10:59.000000 dimples-0.1.6/dimples/conn/queue.py
--rw-r--r--   0 moky       (501) staff       (20)     7738 2022-12-14 05:44:44.000000 dimples-0.1.6/dimples/conn/seeker.py
--rw-r--r--   0 moky       (501) staff       (20)     5726 2023-06-02 09:57:33.000000 dimples-0.1.6/dimples/conn/session.py
--rw-r--r--   0 moky       (501) staff       (20)     6991 2023-01-14 12:47:37.000000 dimples-0.1.6/dimples/conn/ws.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-09 15:09:56.000000 dimples-0.1.6/dimples/database/
--rw-r--r--   0 moky       (501) staff       (20)     2560 2023-06-04 16:46:57.000000 dimples-0.1.6/dimples/database/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     7000 2023-06-02 12:26:57.000000 dimples-0.1.6/dimples/database/account.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-09 15:09:56.000000 dimples-0.1.6/dimples/database/dos/
--rw-r--r--   0 moky       (501) staff       (20)     1808 2023-06-05 05:13:02.000000 dimples-0.1.6/dimples/database/dos/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     4071 2022-12-22 17:59:17.000000 dimples-0.1.6/dimples/database/dos/base.py
--rw-r--r--   0 moky       (501) staff       (20)     3769 2022-12-11 05:07:49.000000 dimples-0.1.6/dimples/database/dos/document.py
--rw-r--r--   0 moky       (501) staff       (20)     4232 2023-06-02 10:30:44.000000 dimples-0.1.6/dimples/database/dos/group.py
--rw-r--r--   0 moky       (501) staff       (20)     3141 2023-06-02 11:02:33.000000 dimples-0.1.6/dimples/database/dos/login.py
--rw-r--r--   0 moky       (501) staff       (20)     2680 2022-12-22 17:58:13.000000 dimples-0.1.6/dimples/database/dos/meta.py
--rw-r--r--   0 moky       (501) staff       (20)     5630 2023-06-02 11:04:20.000000 dimples-0.1.6/dimples/database/dos/private.py
--rw-r--r--   0 moky       (501) staff       (20)     8033 2023-06-09 14:40:24.000000 dimples-0.1.6/dimples/database/dos/station.py
--rw-r--r--   0 moky       (501) staff       (20)     5625 2023-06-02 11:01:02.000000 dimples-0.1.6/dimples/database/dos/user.py
--rw-r--r--   0 moky       (501) staff       (20)     3097 2022-12-13 10:56:52.000000 dimples-0.1.6/dimples/database/message.py
--rw-r--r--   0 moky       (501) staff       (20)     4229 2023-06-04 17:05:32.000000 dimples-0.1.6/dimples/database/session.py
--rw-r--r--   0 moky       (501) staff       (20)     2972 2023-01-31 05:28:07.000000 dimples-0.1.6/dimples/database/t_cipherkey.py
--rw-r--r--   0 moky       (501) staff       (20)     3710 2023-06-09 14:19:20.000000 dimples-0.1.6/dimples/database/t_document.py
--rw-r--r--   0 moky       (501) staff       (20)     7715 2023-06-05 05:41:56.000000 dimples-0.1.6/dimples/database/t_group.py
--rw-r--r--   0 moky       (501) staff       (20)     3718 2023-06-09 14:19:56.000000 dimples-0.1.6/dimples/database/t_login.py
--rw-r--r--   0 moky       (501) staff       (20)     5144 2022-12-22 18:03:37.000000 dimples-0.1.6/dimples/database/t_message.py
--rw-r--r--   0 moky       (501) staff       (20)     3513 2023-06-05 05:36:10.000000 dimples-0.1.6/dimples/database/t_meta.py
--rw-r--r--   0 moky       (501) staff       (20)     5589 2023-06-05 05:38:08.000000 dimples-0.1.6/dimples/database/t_private.py
--rw-r--r--   0 moky       (501) staff       (20)     6647 2023-06-05 05:31:39.000000 dimples-0.1.6/dimples/database/t_station.py
--rw-r--r--   0 moky       (501) staff       (20)     6455 2023-06-05 05:39:18.000000 dimples-0.1.6/dimples/database/t_user.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-09 15:09:56.000000 dimples-0.1.6/dimples/edge/
--rw-r--r--   0 moky       (501) staff       (20)     2127 2022-12-11 05:07:49.000000 dimples-0.1.6/dimples/edge/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)    13562 2023-06-09 14:59:48.000000 dimples-0.1.6/dimples/edge/octopus.py
--rw-r--r--   0 moky       (501) staff       (20)     5594 2023-06-05 05:51:39.000000 dimples-0.1.6/dimples/edge/shared.py
--rw-r--r--   0 moky       (501) staff       (20)     2726 2023-06-04 10:23:09.000000 dimples-0.1.6/dimples/edge/start.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-09 15:09:56.000000 dimples-0.1.6/dimples/register/
--rw-r--r--   0 moky       (501) staff       (20)     1441 2022-12-11 05:07:49.000000 dimples-0.1.6/dimples/register/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     9516 2023-06-02 10:01:29.000000 dimples-0.1.6/dimples/register/generate.py
--rw-r--r--   0 moky       (501) staff       (20)     7045 2023-06-02 10:02:10.000000 dimples-0.1.6/dimples/register/modify.py
--rwxr-xr-x   0 moky       (501) staff       (20)     3880 2022-12-11 05:07:49.000000 dimples-0.1.6/dimples/register/run.py
--rw-r--r--   0 moky       (501) staff       (20)     1971 2022-12-11 05:07:49.000000 dimples-0.1.6/dimples/register/shared.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-09 15:09:56.000000 dimples-0.1.6/dimples/server/
--rw-r--r--   0 moky       (501) staff       (20)     2561 2023-06-07 12:19:50.000000 dimples-0.1.6/dimples/server/__init__.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-09 15:09:56.000000 dimples-0.1.6/dimples/server/cpu/
--rw-r--r--   0 moky       (501) staff       (20)     1855 2023-02-23 09:37:38.000000 dimples-0.1.6/dimples/server/cpu/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     2640 2023-02-23 10:54:44.000000 dimples-0.1.6/dimples/server/cpu/ans.py
--rw-r--r--   0 moky       (501) staff       (20)     4781 2023-06-03 12:02:30.000000 dimples-0.1.6/dimples/server/cpu/document.py
--rw-r--r--   0 moky       (501) staff       (20)     3341 2023-04-14 16:24:15.000000 dimples-0.1.6/dimples/server/cpu/handshake.py
--rw-r--r--   0 moky       (501) staff       (20)     3853 2023-06-03 12:02:46.000000 dimples-0.1.6/dimples/server/cpu/login.py
--rw-r--r--   0 moky       (501) staff       (20)     1847 2023-01-31 05:28:07.000000 dimples-0.1.6/dimples/server/cpu/receipt.py
--rw-r--r--   0 moky       (501) staff       (20)     3089 2023-01-31 05:28:07.000000 dimples-0.1.6/dimples/server/cpu/report.py
--rw-r--r--   0 moky       (501) staff       (20)    13057 2023-06-09 13:06:31.000000 dimples-0.1.6/dimples/server/dispatcher.py
--rw-r--r--   0 moky       (501) staff       (20)    12816 2023-06-09 13:57:31.000000 dimples-0.1.6/dimples/server/messenger.py
--rw-r--r--   0 moky       (501) staff       (20)     6659 2023-06-09 08:36:13.000000 dimples-0.1.6/dimples/server/packer.py
--rw-r--r--   0 moky       (501) staff       (20)     5791 2023-02-23 11:39:56.000000 dimples-0.1.6/dimples/server/processor.py
--rw-r--r--   0 moky       (501) staff       (20)     6443 2023-06-09 13:36:28.000000 dimples-0.1.6/dimples/server/push_info.py
--rw-r--r--   0 moky       (501) staff       (20)     6719 2022-12-11 05:07:49.000000 dimples-0.1.6/dimples/server/push_service.py
--rw-r--r--   0 moky       (501) staff       (20)     5877 2023-06-07 13:18:30.000000 dimples-0.1.6/dimples/server/pusher.py
--rw-r--r--   0 moky       (501) staff       (20)     7986 2023-01-14 12:19:38.000000 dimples-0.1.6/dimples/server/session.py
--rw-r--r--   0 moky       (501) staff       (20)     6997 2022-12-11 05:07:49.000000 dimples-0.1.6/dimples/server/session_center.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-09 15:09:56.000000 dimples-0.1.6/dimples/station/
--rw-r--r--   0 moky       (501) staff       (20)     1549 2023-02-23 13:34:51.000000 dimples-0.1.6/dimples/station/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     4624 2023-06-07 12:21:10.000000 dimples-0.1.6/dimples/station/handler.py
--rw-r--r--   0 moky       (501) staff       (20)     7087 2023-06-07 11:52:56.000000 dimples-0.1.6/dimples/station/shared.py
--rwxr-xr-x   0 moky       (501) staff       (20)     3782 2023-06-04 10:23:09.000000 dimples-0.1.6/dimples/station/start.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-09 15:09:56.000000 dimples-0.1.6/dimples/utils/
--rw-r--r--   0 moky       (501) staff       (20)     2568 2023-02-23 13:38:40.000000 dimples-0.1.6/dimples/utils/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     6447 2022-12-22 12:24:04.000000 dimples-0.1.6/dimples/utils/cache.py
--rw-r--r--   0 moky       (501) staff       (20)     4016 2023-06-02 18:00:31.000000 dimples-0.1.6/dimples/utils/checker.py
--rw-r--r--   0 moky       (501) staff       (20)     5978 2022-12-11 05:07:49.000000 dimples-0.1.6/dimples/utils/dos.py
--rw-r--r--   0 moky       (501) staff       (20)     2805 2022-12-28 05:23:15.000000 dimples-0.1.6/dimples/utils/log.py
--rw-r--r--   0 moky       (501) staff       (20)     1735 2022-12-11 05:07:49.000000 dimples-0.1.6/dimples/utils/singleton.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-09 15:09:56.000000 dimples-0.1.6/dimples.egg-info/
--rw-r--r--   0 moky       (501) staff       (20)     1061 2023-06-09 15:09:56.000000 dimples-0.1.6/dimples.egg-info/PKG-INFO
--rw-r--r--   0 moky       (501) staff       (20)     3247 2023-06-09 15:09:56.000000 dimples-0.1.6/dimples.egg-info/SOURCES.txt
--rw-r--r--   0 moky       (501) staff       (20)        1 2023-06-09 15:09:56.000000 dimples-0.1.6/dimples.egg-info/dependency_links.txt
--rw-r--r--   0 moky       (501) staff       (20)      118 2023-06-09 15:09:56.000000 dimples-0.1.6/dimples.egg-info/entry_points.txt
--rw-r--r--   0 moky       (501) staff       (20)      108 2023-06-09 15:09:56.000000 dimples-0.1.6/dimples.egg-info/requires.txt
--rw-r--r--   0 moky       (501) staff       (20)        8 2023-06-09 15:09:56.000000 dimples-0.1.6/dimples.egg-info/top_level.txt
--rw-r--r--   0 moky       (501) staff       (20)       38 2023-06-09 15:09:56.000000 dimples-0.1.6/setup.cfg
--rw-r--r--   0 moky       (501) staff       (20)     1675 2023-06-09 08:37:55.000000 dimples-0.1.6/setup.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-09 17:20:51.000000 dimples-0.1.7/
+-rw-r--r--   0 moky       (501) staff       (20)     1061 2023-06-09 17:20:51.000000 dimples-0.1.7/PKG-INFO
+-rw-r--r--   0 moky       (501) staff       (20)      568 2022-12-11 05:07:49.000000 dimples-0.1.7/README.md
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-09 17:20:50.000000 dimples-0.1.7/dimples/
+-rw-r--r--   0 moky       (501) staff       (20)     7071 2023-06-03 12:10:17.000000 dimples-0.1.7/dimples/__init__.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-09 17:20:50.000000 dimples-0.1.7/dimples/client/
+-rw-r--r--   0 moky       (501) staff       (20)     1997 2023-06-03 11:38:39.000000 dimples-0.1.7/dimples/client/__init__.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-09 17:20:50.000000 dimples-0.1.7/dimples/client/cpu/
+-rw-r--r--   0 moky       (501) staff       (20)     2191 2023-06-09 16:37:34.000000 dimples-0.1.7/dimples/client/cpu/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     4011 2023-06-02 18:30:20.000000 dimples-0.1.7/dimples/client/cpu/grp_expel.py
+-rw-r--r--   0 moky       (501) staff       (20)     4116 2023-06-02 18:31:07.000000 dimples-0.1.7/dimples/client/cpu/grp_invite.py
+-rw-r--r--   0 moky       (501) staff       (20)     3554 2023-02-23 11:18:06.000000 dimples-0.1.7/dimples/client/cpu/grp_query.py
+-rw-r--r--   0 moky       (501) staff       (20)     3558 2023-06-02 18:31:36.000000 dimples-0.1.7/dimples/client/cpu/grp_quit.py
+-rw-r--r--   0 moky       (501) staff       (20)     6498 2023-06-02 18:32:15.000000 dimples-0.1.7/dimples/client/cpu/grp_reset.py
+-rw-r--r--   0 moky       (501) staff       (20)     5150 2023-02-23 14:17:47.000000 dimples-0.1.7/dimples/client/cpu/handshake.py
+-rw-r--r--   0 moky       (501) staff       (20)     2948 2023-01-31 05:28:07.000000 dimples-0.1.7/dimples/client/cpu/history.py
+-rw-r--r--   0 moky       (501) staff       (20)     1869 2023-01-31 05:28:07.000000 dimples-0.1.7/dimples/client/cpu/login.py
+-rw-r--r--   0 moky       (501) staff       (20)     1847 2023-01-31 05:28:07.000000 dimples-0.1.7/dimples/client/cpu/receipt.py
+-rw-r--r--   0 moky       (501) staff       (20)     1895 2023-06-09 16:41:36.000000 dimples-0.1.7/dimples/client/cpu/text.py
+-rw-r--r--   0 moky       (501) staff       (20)    16324 2023-06-02 17:03:56.000000 dimples-0.1.7/dimples/client/group.py
+-rw-r--r--   0 moky       (501) staff       (20)     7713 2023-06-06 16:33:40.000000 dimples-0.1.7/dimples/client/messenger.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-09 17:20:50.000000 dimples-0.1.7/dimples/client/network/
+-rw-r--r--   0 moky       (501) staff       (20)     3246 2023-02-23 14:19:20.000000 dimples-0.1.7/dimples/client/network/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     6258 2023-02-23 14:14:03.000000 dimples-0.1.7/dimples/client/network/session.py
+-rw-r--r--   0 moky       (501) staff       (20)     8302 2023-06-03 11:39:42.000000 dimples-0.1.7/dimples/client/network/state.py
+-rw-r--r--   0 moky       (501) staff       (20)     9531 2023-01-31 05:28:07.000000 dimples-0.1.7/dimples/client/network/transition.py
+-rw-r--r--   0 moky       (501) staff       (20)     6560 2023-06-06 16:21:36.000000 dimples-0.1.7/dimples/client/packer.py
+-rw-r--r--   0 moky       (501) staff       (20)     7190 2023-06-09 16:42:29.000000 dimples-0.1.7/dimples/client/processor.py
+-rw-r--r--   0 moky       (501) staff       (20)     5521 2023-02-23 14:13:41.000000 dimples-0.1.7/dimples/client/terminal.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-09 17:20:50.000000 dimples-0.1.7/dimples/common/
+-rw-r--r--   0 moky       (501) staff       (20)     2209 2023-06-06 13:30:28.000000 dimples-0.1.7/dimples/common/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     4322 2023-06-02 08:44:29.000000 dimples-0.1.7/dimples/common/ans.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-09 17:20:50.000000 dimples-0.1.7/dimples/common/dbi/
+-rw-r--r--   0 moky       (501) staff       (20)     2324 2023-06-09 14:20:27.000000 dimples-0.1.7/dimples/common/dbi/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     6396 2023-06-02 10:33:41.000000 dimples-0.1.7/dimples/common/dbi/account.py
+-rw-r--r--   0 moky       (501) staff       (20)     2465 2023-06-02 07:39:55.000000 dimples-0.1.7/dimples/common/dbi/message.py
+-rw-r--r--   0 moky       (501) staff       (20)     7877 2023-06-09 15:01:59.000000 dimples-0.1.7/dimples/common/dbi/session.py
+-rw-r--r--   0 moky       (501) staff       (20)     6739 2023-06-02 09:05:19.000000 dimples-0.1.7/dimples/common/facebook.py
+-rw-r--r--   0 moky       (501) staff       (20)     7945 2023-06-09 16:13:09.000000 dimples-0.1.7/dimples/common/messenger.py
+-rw-r--r--   0 moky       (501) staff       (20)     7918 2023-06-06 16:22:19.000000 dimples-0.1.7/dimples/common/packer.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-09 17:20:50.000000 dimples-0.1.7/dimples/common/protocol/
+-rw-r--r--   0 moky       (501) staff       (20)     2536 2023-02-23 09:20:27.000000 dimples-0.1.7/dimples/common/protocol/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     3321 2023-06-09 16:01:10.000000 dimples-0.1.7/dimples/common/protocol/ans.py
+-rw-r--r--   0 moky       (501) staff       (20)     5004 2022-12-23 07:24:37.000000 dimples-0.1.7/dimples/common/protocol/handshake.py
+-rw-r--r--   0 moky       (501) staff       (20)     4523 2023-06-02 08:11:42.000000 dimples-0.1.7/dimples/common/protocol/login.py
+-rw-r--r--   0 moky       (501) staff       (20)     6085 2023-06-02 08:40:15.000000 dimples-0.1.7/dimples/common/protocol/receipt.py
+-rw-r--r--   0 moky       (501) staff       (20)     2521 2023-06-02 08:42:45.000000 dimples-0.1.7/dimples/common/protocol/report.py
+-rw-r--r--   0 moky       (501) staff       (20)     4486 2023-06-04 16:41:38.000000 dimples-0.1.7/dimples/common/session.py
+-rw-r--r--   0 moky       (501) staff       (20)     6211 2023-06-03 12:24:47.000000 dimples-0.1.7/dimples/config.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-09 17:20:50.000000 dimples-0.1.7/dimples/conn/
+-rw-r--r--   0 moky       (501) staff       (20)     4449 2023-01-14 13:47:09.000000 dimples-0.1.7/dimples/conn/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)    10335 2023-06-07 13:23:28.000000 dimples-0.1.7/dimples/conn/gate.py
+-rw-r--r--   0 moky       (501) staff       (20)     9892 2023-01-31 05:28:07.000000 dimples-0.1.7/dimples/conn/gatekeeper.py
+-rw-r--r--   0 moky       (501) staff       (20)    10305 2023-01-14 13:25:42.000000 dimples-0.1.7/dimples/conn/mars.py
+-rw-r--r--   0 moky       (501) staff       (20)     7851 2023-02-23 09:10:59.000000 dimples-0.1.7/dimples/conn/mtp.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-09 17:20:50.000000 dimples-0.1.7/dimples/conn/protocol/
+-rw-r--r--   0 moky       (501) staff       (20)     1842 2022-12-11 05:07:49.000000 dimples-0.1.7/dimples/conn/protocol/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     8711 2022-12-11 05:07:49.000000 dimples-0.1.7/dimples/conn/protocol/mars.py
+-rw-r--r--   0 moky       (501) staff       (20)     8254 2022-12-11 05:07:49.000000 dimples-0.1.7/dimples/conn/protocol/ws.py
+-rw-r--r--   0 moky       (501) staff       (20)     5411 2023-02-23 09:10:59.000000 dimples-0.1.7/dimples/conn/queue.py
+-rw-r--r--   0 moky       (501) staff       (20)     7738 2022-12-14 05:44:44.000000 dimples-0.1.7/dimples/conn/seeker.py
+-rw-r--r--   0 moky       (501) staff       (20)     5726 2023-06-02 09:57:33.000000 dimples-0.1.7/dimples/conn/session.py
+-rw-r--r--   0 moky       (501) staff       (20)     6991 2023-01-14 12:47:37.000000 dimples-0.1.7/dimples/conn/ws.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-09 17:20:50.000000 dimples-0.1.7/dimples/database/
+-rw-r--r--   0 moky       (501) staff       (20)     2560 2023-06-04 16:46:57.000000 dimples-0.1.7/dimples/database/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     7000 2023-06-02 12:26:57.000000 dimples-0.1.7/dimples/database/account.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-09 17:20:50.000000 dimples-0.1.7/dimples/database/dos/
+-rw-r--r--   0 moky       (501) staff       (20)     1808 2023-06-05 05:13:02.000000 dimples-0.1.7/dimples/database/dos/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     4071 2022-12-22 17:59:17.000000 dimples-0.1.7/dimples/database/dos/base.py
+-rw-r--r--   0 moky       (501) staff       (20)     3769 2022-12-11 05:07:49.000000 dimples-0.1.7/dimples/database/dos/document.py
+-rw-r--r--   0 moky       (501) staff       (20)     4232 2023-06-02 10:30:44.000000 dimples-0.1.7/dimples/database/dos/group.py
+-rw-r--r--   0 moky       (501) staff       (20)     3141 2023-06-02 11:02:33.000000 dimples-0.1.7/dimples/database/dos/login.py
+-rw-r--r--   0 moky       (501) staff       (20)     2680 2022-12-22 17:58:13.000000 dimples-0.1.7/dimples/database/dos/meta.py
+-rw-r--r--   0 moky       (501) staff       (20)     5630 2023-06-02 11:04:20.000000 dimples-0.1.7/dimples/database/dos/private.py
+-rw-r--r--   0 moky       (501) staff       (20)     8033 2023-06-09 14:40:24.000000 dimples-0.1.7/dimples/database/dos/station.py
+-rw-r--r--   0 moky       (501) staff       (20)     5625 2023-06-02 11:01:02.000000 dimples-0.1.7/dimples/database/dos/user.py
+-rw-r--r--   0 moky       (501) staff       (20)     3097 2022-12-13 10:56:52.000000 dimples-0.1.7/dimples/database/message.py
+-rw-r--r--   0 moky       (501) staff       (20)     4229 2023-06-04 17:05:32.000000 dimples-0.1.7/dimples/database/session.py
+-rw-r--r--   0 moky       (501) staff       (20)     2972 2023-01-31 05:28:07.000000 dimples-0.1.7/dimples/database/t_cipherkey.py
+-rw-r--r--   0 moky       (501) staff       (20)     3710 2023-06-09 14:19:20.000000 dimples-0.1.7/dimples/database/t_document.py
+-rw-r--r--   0 moky       (501) staff       (20)     7715 2023-06-05 05:41:56.000000 dimples-0.1.7/dimples/database/t_group.py
+-rw-r--r--   0 moky       (501) staff       (20)     3718 2023-06-09 14:19:56.000000 dimples-0.1.7/dimples/database/t_login.py
+-rw-r--r--   0 moky       (501) staff       (20)     5144 2022-12-22 18:03:37.000000 dimples-0.1.7/dimples/database/t_message.py
+-rw-r--r--   0 moky       (501) staff       (20)     3513 2023-06-05 05:36:10.000000 dimples-0.1.7/dimples/database/t_meta.py
+-rw-r--r--   0 moky       (501) staff       (20)     5589 2023-06-05 05:38:08.000000 dimples-0.1.7/dimples/database/t_private.py
+-rw-r--r--   0 moky       (501) staff       (20)     6647 2023-06-05 05:31:39.000000 dimples-0.1.7/dimples/database/t_station.py
+-rw-r--r--   0 moky       (501) staff       (20)     6455 2023-06-05 05:39:18.000000 dimples-0.1.7/dimples/database/t_user.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-09 17:20:50.000000 dimples-0.1.7/dimples/edge/
+-rw-r--r--   0 moky       (501) staff       (20)     2127 2022-12-11 05:07:49.000000 dimples-0.1.7/dimples/edge/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)    13562 2023-06-09 14:59:48.000000 dimples-0.1.7/dimples/edge/octopus.py
+-rw-r--r--   0 moky       (501) staff       (20)     5594 2023-06-05 05:51:39.000000 dimples-0.1.7/dimples/edge/shared.py
+-rw-r--r--   0 moky       (501) staff       (20)     2726 2023-06-04 10:23:09.000000 dimples-0.1.7/dimples/edge/start.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-09 17:20:51.000000 dimples-0.1.7/dimples/register/
+-rw-r--r--   0 moky       (501) staff       (20)     1441 2022-12-11 05:07:49.000000 dimples-0.1.7/dimples/register/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     9516 2023-06-02 10:01:29.000000 dimples-0.1.7/dimples/register/generate.py
+-rw-r--r--   0 moky       (501) staff       (20)     7045 2023-06-02 10:02:10.000000 dimples-0.1.7/dimples/register/modify.py
+-rwxr-xr-x   0 moky       (501) staff       (20)     3880 2022-12-11 05:07:49.000000 dimples-0.1.7/dimples/register/run.py
+-rw-r--r--   0 moky       (501) staff       (20)     1971 2022-12-11 05:07:49.000000 dimples-0.1.7/dimples/register/shared.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-09 17:20:51.000000 dimples-0.1.7/dimples/server/
+-rw-r--r--   0 moky       (501) staff       (20)     2561 2023-06-07 12:19:50.000000 dimples-0.1.7/dimples/server/__init__.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-09 17:20:51.000000 dimples-0.1.7/dimples/server/cpu/
+-rw-r--r--   0 moky       (501) staff       (20)     1855 2023-02-23 09:37:38.000000 dimples-0.1.7/dimples/server/cpu/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     2640 2023-02-23 10:54:44.000000 dimples-0.1.7/dimples/server/cpu/ans.py
+-rw-r--r--   0 moky       (501) staff       (20)     4781 2023-06-03 12:02:30.000000 dimples-0.1.7/dimples/server/cpu/document.py
+-rw-r--r--   0 moky       (501) staff       (20)     3341 2023-04-14 16:24:15.000000 dimples-0.1.7/dimples/server/cpu/handshake.py
+-rw-r--r--   0 moky       (501) staff       (20)     3853 2023-06-03 12:02:46.000000 dimples-0.1.7/dimples/server/cpu/login.py
+-rw-r--r--   0 moky       (501) staff       (20)     1847 2023-01-31 05:28:07.000000 dimples-0.1.7/dimples/server/cpu/receipt.py
+-rw-r--r--   0 moky       (501) staff       (20)     3089 2023-01-31 05:28:07.000000 dimples-0.1.7/dimples/server/cpu/report.py
+-rw-r--r--   0 moky       (501) staff       (20)    13057 2023-06-09 13:06:31.000000 dimples-0.1.7/dimples/server/dispatcher.py
+-rw-r--r--   0 moky       (501) staff       (20)    12628 2023-06-09 17:18:59.000000 dimples-0.1.7/dimples/server/messenger.py
+-rw-r--r--   0 moky       (501) staff       (20)     6659 2023-06-09 08:36:13.000000 dimples-0.1.7/dimples/server/packer.py
+-rw-r--r--   0 moky       (501) staff       (20)     5791 2023-02-23 11:39:56.000000 dimples-0.1.7/dimples/server/processor.py
+-rw-r--r--   0 moky       (501) staff       (20)     6443 2023-06-09 13:36:28.000000 dimples-0.1.7/dimples/server/push_info.py
+-rw-r--r--   0 moky       (501) staff       (20)     6719 2022-12-11 05:07:49.000000 dimples-0.1.7/dimples/server/push_service.py
+-rw-r--r--   0 moky       (501) staff       (20)     5877 2023-06-07 13:18:30.000000 dimples-0.1.7/dimples/server/pusher.py
+-rw-r--r--   0 moky       (501) staff       (20)     7986 2023-01-14 12:19:38.000000 dimples-0.1.7/dimples/server/session.py
+-rw-r--r--   0 moky       (501) staff       (20)     6997 2022-12-11 05:07:49.000000 dimples-0.1.7/dimples/server/session_center.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-09 17:20:51.000000 dimples-0.1.7/dimples/station/
+-rw-r--r--   0 moky       (501) staff       (20)     1549 2023-02-23 13:34:51.000000 dimples-0.1.7/dimples/station/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     4624 2023-06-07 12:21:10.000000 dimples-0.1.7/dimples/station/handler.py
+-rw-r--r--   0 moky       (501) staff       (20)     7087 2023-06-07 11:52:56.000000 dimples-0.1.7/dimples/station/shared.py
+-rwxr-xr-x   0 moky       (501) staff       (20)     3782 2023-06-04 10:23:09.000000 dimples-0.1.7/dimples/station/start.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-09 17:20:51.000000 dimples-0.1.7/dimples/utils/
+-rw-r--r--   0 moky       (501) staff       (20)     2568 2023-02-23 13:38:40.000000 dimples-0.1.7/dimples/utils/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     6447 2022-12-22 12:24:04.000000 dimples-0.1.7/dimples/utils/cache.py
+-rw-r--r--   0 moky       (501) staff       (20)     4016 2023-06-02 18:00:31.000000 dimples-0.1.7/dimples/utils/checker.py
+-rw-r--r--   0 moky       (501) staff       (20)     5978 2022-12-11 05:07:49.000000 dimples-0.1.7/dimples/utils/dos.py
+-rw-r--r--   0 moky       (501) staff       (20)     2805 2022-12-28 05:23:15.000000 dimples-0.1.7/dimples/utils/log.py
+-rw-r--r--   0 moky       (501) staff       (20)     1735 2022-12-11 05:07:49.000000 dimples-0.1.7/dimples/utils/singleton.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-09 17:20:50.000000 dimples-0.1.7/dimples.egg-info/
+-rw-r--r--   0 moky       (501) staff       (20)     1061 2023-06-09 17:20:50.000000 dimples-0.1.7/dimples.egg-info/PKG-INFO
+-rw-r--r--   0 moky       (501) staff       (20)     3274 2023-06-09 17:20:50.000000 dimples-0.1.7/dimples.egg-info/SOURCES.txt
+-rw-r--r--   0 moky       (501) staff       (20)        1 2023-06-09 17:20:50.000000 dimples-0.1.7/dimples.egg-info/dependency_links.txt
+-rw-r--r--   0 moky       (501) staff       (20)      118 2023-06-09 17:20:50.000000 dimples-0.1.7/dimples.egg-info/entry_points.txt
+-rw-r--r--   0 moky       (501) staff       (20)      108 2023-06-09 17:20:50.000000 dimples-0.1.7/dimples.egg-info/requires.txt
+-rw-r--r--   0 moky       (501) staff       (20)        8 2023-06-09 17:20:50.000000 dimples-0.1.7/dimples.egg-info/top_level.txt
+-rw-r--r--   0 moky       (501) staff       (20)       38 2023-06-09 17:20:51.000000 dimples-0.1.7/setup.cfg
+-rw-r--r--   0 moky       (501) staff       (20)     1675 2023-06-09 16:14:04.000000 dimples-0.1.7/setup.py
```

### Comparing `dimples-0.1.6/PKG-INFO` & `dimples-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dimples
-Version: 0.1.6
+Version: 0.1.7
 Summary: DIMP Library for Edges and Stations
 Home-page: https://github.com/dimchat/demo-py
 Author: Albert Moky
 Author-email: albert.moky@gmail.com
 License: MIT
 Description: # DIMP Library for Edges and Stations (Python version)
```

### Comparing `dimples-0.1.6/README.md` & `dimples-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `dimples-0.1.6/dimples/__init__.py` & `dimples-0.1.7/dimples/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.6/dimples/client/__init__.py` & `dimples-0.1.7/dimples/client/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.6/dimples/client/cpu/__init__.py` & `dimples-0.1.7/dimples/client/cpu/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,32 +20,36 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 # ==============================================================================
 
 """
-    Command Processing Unites
+    Content Processing Unites
     ~~~~~~~~~~~~~~~~~~~~~~~~~
 
-    Processors for commands
+    Processors for contents
 """
 
+from .text import TextContentProcessor
+
 from .handshake import HandshakeCommandProcessor
 from .login import LoginCommandProcessor
 from .receipt import ReceiptCommandProcessor
 
 from .history import HistoryCommandProcessor, GroupCommandProcessor
 from .grp_invite import InviteCommandProcessor
 from .grp_expel import ExpelCommandProcessor
 from .grp_quit import QuitCommandProcessor
 from .grp_reset import ResetCommandProcessor
 from .grp_query import QueryCommandProcessor
 
 __all__ = [
+    'TextContentProcessor',
+
     'HandshakeCommandProcessor',
     'LoginCommandProcessor',
     'ReceiptCommandProcessor',
 
     'HistoryCommandProcessor',
     'GroupCommandProcessor',
     'InviteCommandProcessor', 'ExpelCommandProcessor', 'QuitCommandProcessor',
```

### Comparing `dimples-0.1.6/dimples/client/cpu/grp_expel.py` & `dimples-0.1.7/dimples/client/cpu/grp_expel.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.6/dimples/client/cpu/grp_invite.py` & `dimples-0.1.7/dimples/client/cpu/grp_invite.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.6/dimples/client/cpu/grp_query.py` & `dimples-0.1.7/dimples/client/cpu/grp_query.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.6/dimples/client/cpu/grp_quit.py` & `dimples-0.1.7/dimples/client/cpu/grp_quit.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.6/dimples/client/cpu/grp_reset.py` & `dimples-0.1.7/dimples/client/cpu/grp_reset.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.6/dimples/client/cpu/handshake.py` & `dimples-0.1.7/dimples/client/cpu/handshake.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.6/dimples/client/cpu/history.py` & `dimples-0.1.7/dimples/client/cpu/history.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.6/dimples/client/cpu/login.py` & `dimples-0.1.7/dimples/client/cpu/login.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.6/dimples/client/cpu/receipt.py` & `dimples-0.1.7/dimples/client/cpu/receipt.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.6/dimples/client/group.py` & `dimples-0.1.7/dimples/client/group.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.6/dimples/client/messenger.py` & `dimples-0.1.7/dimples/client/messenger.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.6/dimples/client/network/__init__.py` & `dimples-0.1.7/dimples/client/network/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.6/dimples/client/network/session.py` & `dimples-0.1.7/dimples/client/network/session.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.6/dimples/client/network/state.py` & `dimples-0.1.7/dimples/client/network/state.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.6/dimples/client/network/transition.py` & `dimples-0.1.7/dimples/client/network/transition.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.6/dimples/client/packer.py` & `dimples-0.1.7/dimples/client/packer.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.6/dimples/client/processor.py` & `dimples-0.1.7/dimples/client/processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 
 from dimsdk.cpu import BaseContentProcessor, BaseContentProcessorCreator
 
 from ..utils import Logging
 from ..common import HandshakeCommand, ReceiptCommand, LoginCommand
 from ..common import CommonMessenger
 
+from .cpu import TextContentProcessor
 from .cpu import HandshakeCommandProcessor
 from .cpu import LoginCommandProcessor
 from .cpu import ReceiptCommandProcessor
 from .cpu import HistoryCommandProcessor, GroupCommandProcessor
 from .cpu import InviteCommandProcessor, ExpelCommandProcessor, QuitCommandProcessor
 from .cpu import ResetCommandProcessor, QueryCommandProcessor
 
@@ -115,14 +116,18 @@
         return ClientContentProcessorCreator(facebook=self.facebook, messenger=self.messenger)
 
 
 class ClientContentProcessorCreator(BaseContentProcessorCreator):
 
     # Override
     def create_content_processor(self, msg_type: Union[int, ContentType]) -> Optional[ContentProcessor]:
+        # text
+        if msg_type == ContentType.TEXT:
+            return TextContentProcessor(facebook=self.facebook, messenger=self.messenger)
+        # history
         if msg_type == ContentType.HISTORY.value:
             return HistoryCommandProcessor(facebook=self.facebook, messenger=self.messenger)
         # default
         if msg_type == 0:
             return BaseContentProcessor(facebook=self.facebook, messenger=self.messenger)
         # others
         return super().create_content_processor(msg_type=msg_type)
```

### Comparing `dimples-0.1.6/dimples/client/terminal.py` & `dimples-0.1.7/dimples/client/terminal.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.6/dimples/common/__init__.py` & `dimples-0.1.7/dimples/common/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.6/dimples/common/ans.py` & `dimples-0.1.7/dimples/common/ans.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.6/dimples/common/dbi/__init__.py` & `dimples-0.1.7/dimples/common/dbi/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.6/dimples/common/dbi/account.py` & `dimples-0.1.7/dimples/common/dbi/account.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.6/dimples/common/dbi/message.py` & `dimples-0.1.7/dimples/common/dbi/message.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.6/dimples/common/dbi/session.py` & `dimples-0.1.7/dimples/common/dbi/session.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.6/dimples/common/facebook.py` & `dimples-0.1.7/dimples/common/facebook.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.6/dimples/common/messenger.py` & `dimples-0.1.7/dimples/common/messenger.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,19 +143,22 @@
 
     # noinspection PyMethodMayBeStatic
     def _needs_receipt(self, msg: ReliableMessage) -> bool:
         if msg.type == ContentType.COMMAND:
             # filter for looping message (receipt for receipt)
             return False
         sender = msg.sender
-        receiver = msg.receiver
-        if sender.type == EntityType.STATION or sender.type == EntityType.BOT:
-            if receiver.type == EntityType.STATION or receiver.type == EntityType.BOT:
-                # message between bots
-                return False
+        # receiver = msg.receiver
+        # if sender.type == EntityType.STATION or sender.type == EntityType.BOT:
+        #     if receiver.type == EntityType.STATION or receiver.type == EntityType.BOT:
+        #         # message between bots
+        #         return False
+        if sender.type != EntityType.USER:  # and receiver.type != EntityType.USER:
+            # message between bots
+            return False
         # current_user = self.facebook.current_user
         # if receiver != current_user.identifier:
         #     # forward message
         #     return True
         # TODO: other condition?
         return True
```

### Comparing `dimples-0.1.6/dimples/common/packer.py` & `dimples-0.1.7/dimples/common/packer.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.6/dimples/common/protocol/__init__.py` & `dimples-0.1.7/dimples/common/protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.6/dimples/common/protocol/ans.py` & `dimples-0.1.7/dimples/common/protocol/ans.py`

 * *Files 5% similar despite different names*

```diff
@@ -70,15 +70,15 @@
             super().__init__(content=content)
 
     #
     #   ANS aliases
     #
     @property
     def names(self) -> List[str]:
-        string = self.get_str('names')
+        string = self.get_str(key='names')
         return [] if string is None else string.split()
 
     @property
     def records(self) -> Dict[str, str]:
         dictionary = self.get('records')
         return {} if dictionary is None else dictionary
```

### Comparing `dimples-0.1.6/dimples/common/protocol/handshake.py` & `dimples-0.1.7/dimples/common/protocol/handshake.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.6/dimples/common/protocol/login.py` & `dimples-0.1.7/dimples/common/protocol/login.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.6/dimples/common/protocol/receipt.py` & `dimples-0.1.7/dimples/common/protocol/receipt.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.6/dimples/common/protocol/report.py` & `dimples-0.1.7/dimples/common/protocol/report.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.6/dimples/common/session.py` & `dimples-0.1.7/dimples/common/session.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.6/dimples/config.py` & `dimples-0.1.7/dimples/config.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.6/dimples/conn/__init__.py` & `dimples-0.1.7/dimples/conn/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.6/dimples/conn/gate.py` & `dimples-0.1.7/dimples/conn/gate.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.6/dimples/conn/gatekeeper.py` & `dimples-0.1.7/dimples/conn/gatekeeper.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.6/dimples/conn/mars.py` & `dimples-0.1.7/dimples/conn/mars.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.6/dimples/conn/mtp.py` & `dimples-0.1.7/dimples/conn/mtp.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.6/dimples/conn/protocol/__init__.py` & `dimples-0.1.7/dimples/conn/protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.6/dimples/conn/protocol/mars.py` & `dimples-0.1.7/dimples/conn/protocol/mars.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.6/dimples/conn/protocol/ws.py` & `dimples-0.1.7/dimples/conn/protocol/ws.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.6/dimples/conn/queue.py` & `dimples-0.1.7/dimples/conn/queue.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.6/dimples/conn/seeker.py` & `dimples-0.1.7/dimples/conn/seeker.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.6/dimples/conn/session.py` & `dimples-0.1.7/dimples/conn/session.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.6/dimples/conn/ws.py` & `dimples-0.1.7/dimples/conn/ws.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.6/dimples/database/__init__.py` & `dimples-0.1.7/dimples/database/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.6/dimples/database/account.py` & `dimples-0.1.7/dimples/database/account.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.6/dimples/database/dos/__init__.py` & `dimples-0.1.7/dimples/database/dos/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.6/dimples/database/dos/base.py` & `dimples-0.1.7/dimples/database/dos/base.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.6/dimples/database/dos/document.py` & `dimples-0.1.7/dimples/database/dos/document.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.6/dimples/database/dos/group.py` & `dimples-0.1.7/dimples/database/dos/group.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.6/dimples/database/dos/login.py` & `dimples-0.1.7/dimples/database/dos/login.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.6/dimples/database/dos/meta.py` & `dimples-0.1.7/dimples/database/dos/meta.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.6/dimples/database/dos/private.py` & `dimples-0.1.7/dimples/database/dos/private.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.6/dimples/database/dos/station.py` & `dimples-0.1.7/dimples/database/dos/station.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.6/dimples/database/dos/user.py` & `dimples-0.1.7/dimples/database/dos/user.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.6/dimples/database/message.py` & `dimples-0.1.7/dimples/database/message.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.6/dimples/database/session.py` & `dimples-0.1.7/dimples/database/session.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.6/dimples/database/t_cipherkey.py` & `dimples-0.1.7/dimples/database/t_cipherkey.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.6/dimples/database/t_document.py` & `dimples-0.1.7/dimples/database/t_document.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.6/dimples/database/t_group.py` & `dimples-0.1.7/dimples/database/t_group.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.6/dimples/database/t_login.py` & `dimples-0.1.7/dimples/database/t_login.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.6/dimples/database/t_message.py` & `dimples-0.1.7/dimples/database/t_message.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.6/dimples/database/t_meta.py` & `dimples-0.1.7/dimples/database/t_meta.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.6/dimples/database/t_private.py` & `dimples-0.1.7/dimples/database/t_private.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.6/dimples/database/t_station.py` & `dimples-0.1.7/dimples/database/t_station.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.6/dimples/database/t_user.py` & `dimples-0.1.7/dimples/database/t_user.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.6/dimples/edge/__init__.py` & `dimples-0.1.7/dimples/edge/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.6/dimples/edge/octopus.py` & `dimples-0.1.7/dimples/edge/octopus.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.6/dimples/edge/shared.py` & `dimples-0.1.7/dimples/edge/shared.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.6/dimples/edge/start.py` & `dimples-0.1.7/dimples/edge/start.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.6/dimples/register/__init__.py` & `dimples-0.1.7/dimples/register/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.6/dimples/register/generate.py` & `dimples-0.1.7/dimples/register/generate.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.6/dimples/register/modify.py` & `dimples-0.1.7/dimples/register/modify.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.6/dimples/register/run.py` & `dimples-0.1.7/dimples/register/run.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.6/dimples/register/shared.py` & `dimples-0.1.7/dimples/register/shared.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.6/dimples/server/__init__.py` & `dimples-0.1.7/dimples/server/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.6/dimples/server/cpu/__init__.py` & `dimples-0.1.7/dimples/server/cpu/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.6/dimples/server/cpu/ans.py` & `dimples-0.1.7/dimples/server/cpu/ans.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.6/dimples/server/cpu/document.py` & `dimples-0.1.7/dimples/server/cpu/document.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.6/dimples/server/cpu/handshake.py` & `dimples-0.1.7/dimples/server/cpu/handshake.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.6/dimples/server/cpu/login.py` & `dimples-0.1.7/dimples/server/cpu/login.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.6/dimples/server/cpu/receipt.py` & `dimples-0.1.7/dimples/server/cpu/receipt.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.6/dimples/server/cpu/report.py` & `dimples-0.1.7/dimples/server/cpu/report.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.6/dimples/server/dispatcher.py` & `dimples-0.1.7/dimples/server/dispatcher.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.6/dimples/server/messenger.py` & `dimples-0.1.7/dimples/server/messenger.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,53 +37,52 @@
 from dimsdk import EntityType, ID, EVERYONE
 from dimsdk import Station
 from dimsdk import Envelope, Command, MetaCommand, DocumentCommand
 from dimsdk import InstantMessage
 from dimsdk import SecureMessage, ReliableMessage
 
 from ..utils import Singleton, Log, QueryFrequencyChecker
-from ..common import HandshakeCommand, ReceiptCommand
+from ..common import HandshakeCommand
 from ..common import CommonMessenger
 from ..common import SessionDBI
 
 from .packer import FilterManager
 from .dispatcher import Dispatcher
 from .session_center import SessionCenter
 
 
 class ServerMessenger(CommonMessenger):
 
-    def __broadcast_reliable_message(self, msg: ReliableMessage, station: ID) -> int:
+    def __broadcast_reliable_message(self, msg: ReliableMessage, station: ID):
         receiver = msg.receiver
         db = self.session.database
         # get other recipients
         recipients = get_recipients(msg=msg, receiver=receiver, db=db)
         if len(recipients) == 0:
-            Log.warning('other recipients not found: %s' % receiver)
+            self.warning('other recipients not found: %s' % receiver)
             return 0
-        else:
-            Log.info(msg='other recipients: %s => %s' % (receiver, recipients))
+        sender = msg.sender
         # dispatch
         dispatcher = Dispatcher()
         for target in recipients:
             assert not target.is_broadcast, 'recipient error: %s, %s' % (target, receiver)
             if target == station:
-                Log.error(msg='current station should not exists here: %s, %s' % (target, recipients))
+                self.error(msg='current station should not exists here: %s, %s' % (target, recipients))
+                continue
+            elif target == sender:
+                self.warning(msg='skip sender: %s, %s' % (target, recipients))
                 continue
             dispatcher.deliver_message(msg=msg, receiver=target)
 
             # TODO: after deliver to connected neighbors, the dispatcher will continue
             #       delivering via station bridge, should we mark 'sent_neighbors' in
             #       only one message to the bridge, let the bridge to separate for other
             #       neighbors which not connect to this station directly?
-        # response
-        text = 'Broadcast message delivering'
-        command = ReceiptCommand.create(text=text, msg=msg)
-        command['recipients'] = ID.revert(array=recipients)
-        self.send_content(sender=station, receiver=msg.sender, content=command, priority=1)
+        # OK
+        self.info(msg='Broadcast message delivered: %s, sender: %s' % (recipients, sender))
         return len(recipients)
 
     def __broadcast_command(self, content: Command, receiver: ID):
         sid = self.facebook.current_user.identifier
         env = Envelope.create(sender=sid, receiver=receiver)
         i_msg = InstantMessage.create(head=env, body=content)
         # pack & deliver message
@@ -171,17 +170,16 @@
             self.send_content(sender=sid, receiver=sender, content=cmd)
             # DISCUSS: suspend this message for waiting handshake accepted
             #          or let the client to send it again?
             return None
         # session is active, so this message is not for current station,
         # deliver to the real receiver and respond to sender
         dispatcher = Dispatcher()
-        responses = dispatcher.deliver_message(msg=msg, receiver=receiver)
-        for res in responses:
-            self.send_content(sender=sid, receiver=sender, content=res)
+        dispatcher.deliver_message(msg=msg, receiver=receiver)
+        # TODO: send responses to the sender?
 
     # Override
     def process_reliable_message(self, msg: ReliableMessage) -> List[ReliableMessage]:
         # call super
         responses = super().process_reliable_message(msg=msg)
         current = self.facebook.current_user
         sid = current.identifier
```

### Comparing `dimples-0.1.6/dimples/server/packer.py` & `dimples-0.1.7/dimples/server/packer.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.6/dimples/server/processor.py` & `dimples-0.1.7/dimples/server/processor.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.6/dimples/server/push_info.py` & `dimples-0.1.7/dimples/server/push_info.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.6/dimples/server/push_service.py` & `dimples-0.1.7/dimples/server/push_service.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.6/dimples/server/pusher.py` & `dimples-0.1.7/dimples/server/pusher.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.6/dimples/server/session.py` & `dimples-0.1.7/dimples/server/session.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.6/dimples/server/session_center.py` & `dimples-0.1.7/dimples/server/session_center.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.6/dimples/station/__init__.py` & `dimples-0.1.7/dimples/station/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.6/dimples/station/handler.py` & `dimples-0.1.7/dimples/station/handler.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.6/dimples/station/shared.py` & `dimples-0.1.7/dimples/station/shared.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.6/dimples/station/start.py` & `dimples-0.1.7/dimples/station/start.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.6/dimples/utils/__init__.py` & `dimples-0.1.7/dimples/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.6/dimples/utils/cache.py` & `dimples-0.1.7/dimples/utils/cache.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.6/dimples/utils/checker.py` & `dimples-0.1.7/dimples/utils/checker.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.6/dimples/utils/dos.py` & `dimples-0.1.7/dimples/utils/dos.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.6/dimples/utils/log.py` & `dimples-0.1.7/dimples/utils/log.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.6/dimples/utils/singleton.py` & `dimples-0.1.7/dimples/utils/singleton.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.6/dimples.egg-info/PKG-INFO` & `dimples-0.1.7/dimples.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dimples
-Version: 0.1.6
+Version: 0.1.7
 Summary: DIMP Library for Edges and Stations
 Home-page: https://github.com/dimchat/demo-py
 Author: Albert Moky
 Author-email: albert.moky@gmail.com
 License: MIT
 Description: # DIMP Library for Edges and Stations (Python version)
```

### Comparing `dimples-0.1.6/dimples.egg-info/SOURCES.txt` & `dimples-0.1.7/dimples.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 dimples/client/cpu/grp_query.py
 dimples/client/cpu/grp_quit.py
 dimples/client/cpu/grp_reset.py
 dimples/client/cpu/handshake.py
 dimples/client/cpu/history.py
 dimples/client/cpu/login.py
 dimples/client/cpu/receipt.py
+dimples/client/cpu/text.py
 dimples/client/network/__init__.py
 dimples/client/network/session.py
 dimples/client/network/state.py
 dimples/client/network/transition.py
 dimples/common/__init__.py
 dimples/common/ans.py
 dimples/common/facebook.py
```

### Comparing `dimples-0.1.6/setup.py` & `dimples-0.1.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     communications between accounts safely by end-to-end encryption.
 """
 
 import io
 
 from setuptools import setup, find_packages
 
-__version__ = '0.1.6'
+__version__ = '0.1.7'
 __author__ = 'Albert Moky'
 __contact__ = 'albert.moky@gmail.com'
 
 with io.open('README.md', 'r', encoding='utf-8') as fh:
     readme = fh.read()
 
 setup(
```

