# Comparing `tmp/dimples-0.1.5.tar.gz` & `tmp/dimples-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dimples-0.1.5.tar", last modified: Wed Jun  7 17:09:33 2023, max compression
+gzip compressed data, was "dist/dimples-0.1.6.tar", last modified: Fri Jun  9 15:09:56 2023, max compression
```

## Comparing `dimples-0.1.5.tar` & `dimples-0.1.6.tar`

### file list

```diff
@@ -1,137 +1,137 @@
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-07 17:09:33.000000 dimples-0.1.5/
--rw-r--r--   0 moky       (501) staff       (20)     1061 2023-06-07 17:09:33.000000 dimples-0.1.5/PKG-INFO
--rw-r--r--   0 moky       (501) staff       (20)      568 2022-12-11 05:07:49.000000 dimples-0.1.5/README.md
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-07 17:09:33.000000 dimples-0.1.5/dimples/
--rw-r--r--   0 moky       (501) staff       (20)     7071 2023-06-03 12:10:17.000000 dimples-0.1.5/dimples/__init__.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-07 17:09:33.000000 dimples-0.1.5/dimples/client/
--rw-r--r--   0 moky       (501) staff       (20)     1997 2023-06-03 11:38:39.000000 dimples-0.1.5/dimples/client/__init__.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-07 17:09:33.000000 dimples-0.1.5/dimples/client/cpu/
--rw-r--r--   0 moky       (501) staff       (20)     2122 2023-01-31 05:28:07.000000 dimples-0.1.5/dimples/client/cpu/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     4011 2023-06-02 18:30:20.000000 dimples-0.1.5/dimples/client/cpu/grp_expel.py
--rw-r--r--   0 moky       (501) staff       (20)     4116 2023-06-02 18:31:07.000000 dimples-0.1.5/dimples/client/cpu/grp_invite.py
--rw-r--r--   0 moky       (501) staff       (20)     3554 2023-02-23 11:18:06.000000 dimples-0.1.5/dimples/client/cpu/grp_query.py
--rw-r--r--   0 moky       (501) staff       (20)     3558 2023-06-02 18:31:36.000000 dimples-0.1.5/dimples/client/cpu/grp_quit.py
--rw-r--r--   0 moky       (501) staff       (20)     6498 2023-06-02 18:32:15.000000 dimples-0.1.5/dimples/client/cpu/grp_reset.py
--rw-r--r--   0 moky       (501) staff       (20)     5150 2023-02-23 14:17:47.000000 dimples-0.1.5/dimples/client/cpu/handshake.py
--rw-r--r--   0 moky       (501) staff       (20)     2948 2023-01-31 05:28:07.000000 dimples-0.1.5/dimples/client/cpu/history.py
--rw-r--r--   0 moky       (501) staff       (20)     1869 2023-01-31 05:28:07.000000 dimples-0.1.5/dimples/client/cpu/login.py
--rw-r--r--   0 moky       (501) staff       (20)     1847 2023-01-31 05:28:07.000000 dimples-0.1.5/dimples/client/cpu/receipt.py
--rw-r--r--   0 moky       (501) staff       (20)    16324 2023-06-02 17:03:56.000000 dimples-0.1.5/dimples/client/group.py
--rw-r--r--   0 moky       (501) staff       (20)     7713 2023-06-06 16:33:40.000000 dimples-0.1.5/dimples/client/messenger.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-07 17:09:33.000000 dimples-0.1.5/dimples/client/network/
--rw-r--r--   0 moky       (501) staff       (20)     3246 2023-02-23 14:19:20.000000 dimples-0.1.5/dimples/client/network/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     6258 2023-02-23 14:14:03.000000 dimples-0.1.5/dimples/client/network/session.py
--rw-r--r--   0 moky       (501) staff       (20)     8302 2023-06-03 11:39:42.000000 dimples-0.1.5/dimples/client/network/state.py
--rw-r--r--   0 moky       (501) staff       (20)     9531 2023-01-31 05:28:07.000000 dimples-0.1.5/dimples/client/network/transition.py
--rw-r--r--   0 moky       (501) staff       (20)     6560 2023-06-06 16:21:36.000000 dimples-0.1.5/dimples/client/packer.py
--rw-r--r--   0 moky       (501) staff       (20)     6988 2023-01-31 05:28:07.000000 dimples-0.1.5/dimples/client/processor.py
--rw-r--r--   0 moky       (501) staff       (20)     5521 2023-02-23 14:13:41.000000 dimples-0.1.5/dimples/client/terminal.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-07 17:09:33.000000 dimples-0.1.5/dimples/common/
--rw-r--r--   0 moky       (501) staff       (20)     2209 2023-06-06 13:30:28.000000 dimples-0.1.5/dimples/common/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     4322 2023-06-02 08:44:29.000000 dimples-0.1.5/dimples/common/ans.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-07 17:09:33.000000 dimples-0.1.5/dimples/common/dbi/
--rw-r--r--   0 moky       (501) staff       (20)     2079 2023-06-04 17:02:25.000000 dimples-0.1.5/dimples/common/dbi/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     6396 2023-06-02 10:33:41.000000 dimples-0.1.5/dimples/common/dbi/account.py
--rw-r--r--   0 moky       (501) staff       (20)     2465 2023-06-02 07:39:55.000000 dimples-0.1.5/dimples/common/dbi/message.py
--rw-r--r--   0 moky       (501) staff       (20)     7819 2023-06-05 04:31:02.000000 dimples-0.1.5/dimples/common/dbi/session.py
--rw-r--r--   0 moky       (501) staff       (20)     6739 2023-06-02 09:05:19.000000 dimples-0.1.5/dimples/common/facebook.py
--rw-r--r--   0 moky       (501) staff       (20)     6092 2023-06-06 13:27:51.000000 dimples-0.1.5/dimples/common/messenger.py
--rw-r--r--   0 moky       (501) staff       (20)     7918 2023-06-06 16:22:19.000000 dimples-0.1.5/dimples/common/packer.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-07 17:09:33.000000 dimples-0.1.5/dimples/common/protocol/
--rw-r--r--   0 moky       (501) staff       (20)     2536 2023-02-23 09:20:27.000000 dimples-0.1.5/dimples/common/protocol/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     3317 2023-06-02 08:06:32.000000 dimples-0.1.5/dimples/common/protocol/ans.py
--rw-r--r--   0 moky       (501) staff       (20)     5004 2022-12-23 07:24:37.000000 dimples-0.1.5/dimples/common/protocol/handshake.py
--rw-r--r--   0 moky       (501) staff       (20)     4523 2023-06-02 08:11:42.000000 dimples-0.1.5/dimples/common/protocol/login.py
--rw-r--r--   0 moky       (501) staff       (20)     6085 2023-06-02 08:40:15.000000 dimples-0.1.5/dimples/common/protocol/receipt.py
--rw-r--r--   0 moky       (501) staff       (20)     2521 2023-06-02 08:42:45.000000 dimples-0.1.5/dimples/common/protocol/report.py
--rw-r--r--   0 moky       (501) staff       (20)     4486 2023-06-04 16:41:38.000000 dimples-0.1.5/dimples/common/session.py
--rw-r--r--   0 moky       (501) staff       (20)     6211 2023-06-03 12:24:47.000000 dimples-0.1.5/dimples/config.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-07 17:09:33.000000 dimples-0.1.5/dimples/conn/
--rw-r--r--   0 moky       (501) staff       (20)     4449 2023-01-14 13:47:09.000000 dimples-0.1.5/dimples/conn/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)    10335 2023-06-07 13:23:28.000000 dimples-0.1.5/dimples/conn/gate.py
--rw-r--r--   0 moky       (501) staff       (20)     9892 2023-01-31 05:28:07.000000 dimples-0.1.5/dimples/conn/gatekeeper.py
--rw-r--r--   0 moky       (501) staff       (20)    10305 2023-01-14 13:25:42.000000 dimples-0.1.5/dimples/conn/mars.py
--rw-r--r--   0 moky       (501) staff       (20)     7851 2023-02-23 09:10:59.000000 dimples-0.1.5/dimples/conn/mtp.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-07 17:09:33.000000 dimples-0.1.5/dimples/conn/protocol/
--rw-r--r--   0 moky       (501) staff       (20)     1842 2022-12-11 05:07:49.000000 dimples-0.1.5/dimples/conn/protocol/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     8711 2022-12-11 05:07:49.000000 dimples-0.1.5/dimples/conn/protocol/mars.py
--rw-r--r--   0 moky       (501) staff       (20)     8254 2022-12-11 05:07:49.000000 dimples-0.1.5/dimples/conn/protocol/ws.py
--rw-r--r--   0 moky       (501) staff       (20)     5411 2023-02-23 09:10:59.000000 dimples-0.1.5/dimples/conn/queue.py
--rw-r--r--   0 moky       (501) staff       (20)     7738 2022-12-14 05:44:44.000000 dimples-0.1.5/dimples/conn/seeker.py
--rw-r--r--   0 moky       (501) staff       (20)     5726 2023-06-02 09:57:33.000000 dimples-0.1.5/dimples/conn/session.py
--rw-r--r--   0 moky       (501) staff       (20)     6991 2023-01-14 12:47:37.000000 dimples-0.1.5/dimples/conn/ws.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-07 17:09:33.000000 dimples-0.1.5/dimples/database/
--rw-r--r--   0 moky       (501) staff       (20)     2560 2023-06-04 16:46:57.000000 dimples-0.1.5/dimples/database/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     7000 2023-06-02 12:26:57.000000 dimples-0.1.5/dimples/database/account.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-07 17:09:33.000000 dimples-0.1.5/dimples/database/dos/
--rw-r--r--   0 moky       (501) staff       (20)     1808 2023-06-05 05:13:02.000000 dimples-0.1.5/dimples/database/dos/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     4071 2022-12-22 17:59:17.000000 dimples-0.1.5/dimples/database/dos/base.py
--rw-r--r--   0 moky       (501) staff       (20)     3769 2022-12-11 05:07:49.000000 dimples-0.1.5/dimples/database/dos/document.py
--rw-r--r--   0 moky       (501) staff       (20)     4232 2023-06-02 10:30:44.000000 dimples-0.1.5/dimples/database/dos/group.py
--rw-r--r--   0 moky       (501) staff       (20)     3141 2023-06-02 11:02:33.000000 dimples-0.1.5/dimples/database/dos/login.py
--rw-r--r--   0 moky       (501) staff       (20)     2680 2022-12-22 17:58:13.000000 dimples-0.1.5/dimples/database/dos/meta.py
--rw-r--r--   0 moky       (501) staff       (20)     5630 2023-06-02 11:04:20.000000 dimples-0.1.5/dimples/database/dos/private.py
--rw-r--r--   0 moky       (501) staff       (20)     7961 2023-06-05 04:49:04.000000 dimples-0.1.5/dimples/database/dos/station.py
--rw-r--r--   0 moky       (501) staff       (20)     5625 2023-06-02 11:01:02.000000 dimples-0.1.5/dimples/database/dos/user.py
--rw-r--r--   0 moky       (501) staff       (20)     3097 2022-12-13 10:56:52.000000 dimples-0.1.5/dimples/database/message.py
--rw-r--r--   0 moky       (501) staff       (20)     4229 2023-06-04 17:05:32.000000 dimples-0.1.5/dimples/database/session.py
--rw-r--r--   0 moky       (501) staff       (20)     2972 2023-01-31 05:28:07.000000 dimples-0.1.5/dimples/database/t_cipherkey.py
--rw-r--r--   0 moky       (501) staff       (20)     3649 2023-06-05 05:32:38.000000 dimples-0.1.5/dimples/database/t_document.py
--rw-r--r--   0 moky       (501) staff       (20)     7715 2023-06-05 05:41:56.000000 dimples-0.1.5/dimples/database/t_group.py
--rw-r--r--   0 moky       (501) staff       (20)     3658 2023-06-05 05:34:19.000000 dimples-0.1.5/dimples/database/t_login.py
--rw-r--r--   0 moky       (501) staff       (20)     5144 2022-12-22 18:03:37.000000 dimples-0.1.5/dimples/database/t_message.py
--rw-r--r--   0 moky       (501) staff       (20)     3513 2023-06-05 05:36:10.000000 dimples-0.1.5/dimples/database/t_meta.py
--rw-r--r--   0 moky       (501) staff       (20)     5589 2023-06-05 05:38:08.000000 dimples-0.1.5/dimples/database/t_private.py
--rw-r--r--   0 moky       (501) staff       (20)     6647 2023-06-05 05:31:39.000000 dimples-0.1.5/dimples/database/t_station.py
--rw-r--r--   0 moky       (501) staff       (20)     6455 2023-06-05 05:39:18.000000 dimples-0.1.5/dimples/database/t_user.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-07 17:09:33.000000 dimples-0.1.5/dimples/edge/
--rw-r--r--   0 moky       (501) staff       (20)     2127 2022-12-11 05:07:49.000000 dimples-0.1.5/dimples/edge/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)    12884 2023-06-05 09:19:20.000000 dimples-0.1.5/dimples/edge/octopus.py
--rw-r--r--   0 moky       (501) staff       (20)     5594 2023-06-05 05:51:39.000000 dimples-0.1.5/dimples/edge/shared.py
--rw-r--r--   0 moky       (501) staff       (20)     2726 2023-06-04 10:23:09.000000 dimples-0.1.5/dimples/edge/start.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-07 17:09:33.000000 dimples-0.1.5/dimples/register/
--rw-r--r--   0 moky       (501) staff       (20)     1441 2022-12-11 05:07:49.000000 dimples-0.1.5/dimples/register/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     9516 2023-06-02 10:01:29.000000 dimples-0.1.5/dimples/register/generate.py
--rw-r--r--   0 moky       (501) staff       (20)     7045 2023-06-02 10:02:10.000000 dimples-0.1.5/dimples/register/modify.py
--rwxr-xr-x   0 moky       (501) staff       (20)     3880 2022-12-11 05:07:49.000000 dimples-0.1.5/dimples/register/run.py
--rw-r--r--   0 moky       (501) staff       (20)     1971 2022-12-11 05:07:49.000000 dimples-0.1.5/dimples/register/shared.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-07 17:09:33.000000 dimples-0.1.5/dimples/server/
--rw-r--r--   0 moky       (501) staff       (20)     2561 2023-06-07 12:19:50.000000 dimples-0.1.5/dimples/server/__init__.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-07 17:09:33.000000 dimples-0.1.5/dimples/server/cpu/
--rw-r--r--   0 moky       (501) staff       (20)     1855 2023-02-23 09:37:38.000000 dimples-0.1.5/dimples/server/cpu/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     2640 2023-02-23 10:54:44.000000 dimples-0.1.5/dimples/server/cpu/ans.py
--rw-r--r--   0 moky       (501) staff       (20)     4781 2023-06-03 12:02:30.000000 dimples-0.1.5/dimples/server/cpu/document.py
--rw-r--r--   0 moky       (501) staff       (20)     3341 2023-04-14 16:24:15.000000 dimples-0.1.5/dimples/server/cpu/handshake.py
--rw-r--r--   0 moky       (501) staff       (20)     3853 2023-06-03 12:02:46.000000 dimples-0.1.5/dimples/server/cpu/login.py
--rw-r--r--   0 moky       (501) staff       (20)     1847 2023-01-31 05:28:07.000000 dimples-0.1.5/dimples/server/cpu/receipt.py
--rw-r--r--   0 moky       (501) staff       (20)     3089 2023-01-31 05:28:07.000000 dimples-0.1.5/dimples/server/cpu/report.py
--rw-r--r--   0 moky       (501) staff       (20)    12938 2023-06-07 12:15:09.000000 dimples-0.1.5/dimples/server/dispatcher.py
--rw-r--r--   0 moky       (501) staff       (20)    12456 2023-06-07 16:52:51.000000 dimples-0.1.5/dimples/server/messenger.py
--rw-r--r--   0 moky       (501) staff       (20)     7656 2023-06-07 15:42:18.000000 dimples-0.1.5/dimples/server/packer.py
--rw-r--r--   0 moky       (501) staff       (20)     5791 2023-02-23 11:39:56.000000 dimples-0.1.5/dimples/server/processor.py
--rw-r--r--   0 moky       (501) staff       (20)     6433 2022-12-11 05:07:49.000000 dimples-0.1.5/dimples/server/push_info.py
--rw-r--r--   0 moky       (501) staff       (20)     6719 2022-12-11 05:07:49.000000 dimples-0.1.5/dimples/server/push_service.py
--rw-r--r--   0 moky       (501) staff       (20)     5877 2023-06-07 13:18:30.000000 dimples-0.1.5/dimples/server/pusher.py
--rw-r--r--   0 moky       (501) staff       (20)     7986 2023-01-14 12:19:38.000000 dimples-0.1.5/dimples/server/session.py
--rw-r--r--   0 moky       (501) staff       (20)     6997 2022-12-11 05:07:49.000000 dimples-0.1.5/dimples/server/session_center.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-07 17:09:33.000000 dimples-0.1.5/dimples/station/
--rw-r--r--   0 moky       (501) staff       (20)     1549 2023-02-23 13:34:51.000000 dimples-0.1.5/dimples/station/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     4624 2023-06-07 12:21:10.000000 dimples-0.1.5/dimples/station/handler.py
--rw-r--r--   0 moky       (501) staff       (20)     7087 2023-06-07 11:52:56.000000 dimples-0.1.5/dimples/station/shared.py
--rwxr-xr-x   0 moky       (501) staff       (20)     3782 2023-06-04 10:23:09.000000 dimples-0.1.5/dimples/station/start.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-07 17:09:33.000000 dimples-0.1.5/dimples/utils/
--rw-r--r--   0 moky       (501) staff       (20)     2568 2023-02-23 13:38:40.000000 dimples-0.1.5/dimples/utils/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     6447 2022-12-22 12:24:04.000000 dimples-0.1.5/dimples/utils/cache.py
--rw-r--r--   0 moky       (501) staff       (20)     4016 2023-06-02 18:00:31.000000 dimples-0.1.5/dimples/utils/checker.py
--rw-r--r--   0 moky       (501) staff       (20)     5978 2022-12-11 05:07:49.000000 dimples-0.1.5/dimples/utils/dos.py
--rw-r--r--   0 moky       (501) staff       (20)     2805 2022-12-28 05:23:15.000000 dimples-0.1.5/dimples/utils/log.py
--rw-r--r--   0 moky       (501) staff       (20)     1735 2022-12-11 05:07:49.000000 dimples-0.1.5/dimples/utils/singleton.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-07 17:09:33.000000 dimples-0.1.5/dimples.egg-info/
--rw-r--r--   0 moky       (501) staff       (20)     1061 2023-06-07 17:09:32.000000 dimples-0.1.5/dimples.egg-info/PKG-INFO
--rw-r--r--   0 moky       (501) staff       (20)     3247 2023-06-07 17:09:32.000000 dimples-0.1.5/dimples.egg-info/SOURCES.txt
--rw-r--r--   0 moky       (501) staff       (20)        1 2023-06-07 17:09:32.000000 dimples-0.1.5/dimples.egg-info/dependency_links.txt
--rw-r--r--   0 moky       (501) staff       (20)      118 2023-06-07 17:09:32.000000 dimples-0.1.5/dimples.egg-info/entry_points.txt
--rw-r--r--   0 moky       (501) staff       (20)      108 2023-06-07 17:09:32.000000 dimples-0.1.5/dimples.egg-info/requires.txt
--rw-r--r--   0 moky       (501) staff       (20)        8 2023-06-07 17:09:32.000000 dimples-0.1.5/dimples.egg-info/top_level.txt
--rw-r--r--   0 moky       (501) staff       (20)       38 2023-06-07 17:09:33.000000 dimples-0.1.5/setup.cfg
--rw-r--r--   0 moky       (501) staff       (20)     1675 2023-06-02 06:58:43.000000 dimples-0.1.5/setup.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-09 15:09:56.000000 dimples-0.1.6/
+-rw-r--r--   0 moky       (501) staff       (20)     1061 2023-06-09 15:09:56.000000 dimples-0.1.6/PKG-INFO
+-rw-r--r--   0 moky       (501) staff       (20)      568 2022-12-11 05:07:49.000000 dimples-0.1.6/README.md
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-09 15:09:56.000000 dimples-0.1.6/dimples/
+-rw-r--r--   0 moky       (501) staff       (20)     7071 2023-06-03 12:10:17.000000 dimples-0.1.6/dimples/__init__.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-09 15:09:56.000000 dimples-0.1.6/dimples/client/
+-rw-r--r--   0 moky       (501) staff       (20)     1997 2023-06-03 11:38:39.000000 dimples-0.1.6/dimples/client/__init__.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-09 15:09:56.000000 dimples-0.1.6/dimples/client/cpu/
+-rw-r--r--   0 moky       (501) staff       (20)     2122 2023-01-31 05:28:07.000000 dimples-0.1.6/dimples/client/cpu/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     4011 2023-06-02 18:30:20.000000 dimples-0.1.6/dimples/client/cpu/grp_expel.py
+-rw-r--r--   0 moky       (501) staff       (20)     4116 2023-06-02 18:31:07.000000 dimples-0.1.6/dimples/client/cpu/grp_invite.py
+-rw-r--r--   0 moky       (501) staff       (20)     3554 2023-02-23 11:18:06.000000 dimples-0.1.6/dimples/client/cpu/grp_query.py
+-rw-r--r--   0 moky       (501) staff       (20)     3558 2023-06-02 18:31:36.000000 dimples-0.1.6/dimples/client/cpu/grp_quit.py
+-rw-r--r--   0 moky       (501) staff       (20)     6498 2023-06-02 18:32:15.000000 dimples-0.1.6/dimples/client/cpu/grp_reset.py
+-rw-r--r--   0 moky       (501) staff       (20)     5150 2023-02-23 14:17:47.000000 dimples-0.1.6/dimples/client/cpu/handshake.py
+-rw-r--r--   0 moky       (501) staff       (20)     2948 2023-01-31 05:28:07.000000 dimples-0.1.6/dimples/client/cpu/history.py
+-rw-r--r--   0 moky       (501) staff       (20)     1869 2023-01-31 05:28:07.000000 dimples-0.1.6/dimples/client/cpu/login.py
+-rw-r--r--   0 moky       (501) staff       (20)     1847 2023-01-31 05:28:07.000000 dimples-0.1.6/dimples/client/cpu/receipt.py
+-rw-r--r--   0 moky       (501) staff       (20)    16324 2023-06-02 17:03:56.000000 dimples-0.1.6/dimples/client/group.py
+-rw-r--r--   0 moky       (501) staff       (20)     7713 2023-06-06 16:33:40.000000 dimples-0.1.6/dimples/client/messenger.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-09 15:09:56.000000 dimples-0.1.6/dimples/client/network/
+-rw-r--r--   0 moky       (501) staff       (20)     3246 2023-02-23 14:19:20.000000 dimples-0.1.6/dimples/client/network/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     6258 2023-02-23 14:14:03.000000 dimples-0.1.6/dimples/client/network/session.py
+-rw-r--r--   0 moky       (501) staff       (20)     8302 2023-06-03 11:39:42.000000 dimples-0.1.6/dimples/client/network/state.py
+-rw-r--r--   0 moky       (501) staff       (20)     9531 2023-01-31 05:28:07.000000 dimples-0.1.6/dimples/client/network/transition.py
+-rw-r--r--   0 moky       (501) staff       (20)     6560 2023-06-06 16:21:36.000000 dimples-0.1.6/dimples/client/packer.py
+-rw-r--r--   0 moky       (501) staff       (20)     6988 2023-01-31 05:28:07.000000 dimples-0.1.6/dimples/client/processor.py
+-rw-r--r--   0 moky       (501) staff       (20)     5521 2023-02-23 14:13:41.000000 dimples-0.1.6/dimples/client/terminal.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-09 15:09:56.000000 dimples-0.1.6/dimples/common/
+-rw-r--r--   0 moky       (501) staff       (20)     2209 2023-06-06 13:30:28.000000 dimples-0.1.6/dimples/common/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     4322 2023-06-02 08:44:29.000000 dimples-0.1.6/dimples/common/ans.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-09 15:09:56.000000 dimples-0.1.6/dimples/common/dbi/
+-rw-r--r--   0 moky       (501) staff       (20)     2324 2023-06-09 14:20:27.000000 dimples-0.1.6/dimples/common/dbi/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     6396 2023-06-02 10:33:41.000000 dimples-0.1.6/dimples/common/dbi/account.py
+-rw-r--r--   0 moky       (501) staff       (20)     2465 2023-06-02 07:39:55.000000 dimples-0.1.6/dimples/common/dbi/message.py
+-rw-r--r--   0 moky       (501) staff       (20)     7877 2023-06-09 15:01:59.000000 dimples-0.1.6/dimples/common/dbi/session.py
+-rw-r--r--   0 moky       (501) staff       (20)     6739 2023-06-02 09:05:19.000000 dimples-0.1.6/dimples/common/facebook.py
+-rw-r--r--   0 moky       (501) staff       (20)     7791 2023-06-09 10:25:42.000000 dimples-0.1.6/dimples/common/messenger.py
+-rw-r--r--   0 moky       (501) staff       (20)     7918 2023-06-06 16:22:19.000000 dimples-0.1.6/dimples/common/packer.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-09 15:09:56.000000 dimples-0.1.6/dimples/common/protocol/
+-rw-r--r--   0 moky       (501) staff       (20)     2536 2023-02-23 09:20:27.000000 dimples-0.1.6/dimples/common/protocol/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     3317 2023-06-02 08:06:32.000000 dimples-0.1.6/dimples/common/protocol/ans.py
+-rw-r--r--   0 moky       (501) staff       (20)     5004 2022-12-23 07:24:37.000000 dimples-0.1.6/dimples/common/protocol/handshake.py
+-rw-r--r--   0 moky       (501) staff       (20)     4523 2023-06-02 08:11:42.000000 dimples-0.1.6/dimples/common/protocol/login.py
+-rw-r--r--   0 moky       (501) staff       (20)     6085 2023-06-02 08:40:15.000000 dimples-0.1.6/dimples/common/protocol/receipt.py
+-rw-r--r--   0 moky       (501) staff       (20)     2521 2023-06-02 08:42:45.000000 dimples-0.1.6/dimples/common/protocol/report.py
+-rw-r--r--   0 moky       (501) staff       (20)     4486 2023-06-04 16:41:38.000000 dimples-0.1.6/dimples/common/session.py
+-rw-r--r--   0 moky       (501) staff       (20)     6211 2023-06-03 12:24:47.000000 dimples-0.1.6/dimples/config.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-09 15:09:56.000000 dimples-0.1.6/dimples/conn/
+-rw-r--r--   0 moky       (501) staff       (20)     4449 2023-01-14 13:47:09.000000 dimples-0.1.6/dimples/conn/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)    10335 2023-06-07 13:23:28.000000 dimples-0.1.6/dimples/conn/gate.py
+-rw-r--r--   0 moky       (501) staff       (20)     9892 2023-01-31 05:28:07.000000 dimples-0.1.6/dimples/conn/gatekeeper.py
+-rw-r--r--   0 moky       (501) staff       (20)    10305 2023-01-14 13:25:42.000000 dimples-0.1.6/dimples/conn/mars.py
+-rw-r--r--   0 moky       (501) staff       (20)     7851 2023-02-23 09:10:59.000000 dimples-0.1.6/dimples/conn/mtp.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-09 15:09:56.000000 dimples-0.1.6/dimples/conn/protocol/
+-rw-r--r--   0 moky       (501) staff       (20)     1842 2022-12-11 05:07:49.000000 dimples-0.1.6/dimples/conn/protocol/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     8711 2022-12-11 05:07:49.000000 dimples-0.1.6/dimples/conn/protocol/mars.py
+-rw-r--r--   0 moky       (501) staff       (20)     8254 2022-12-11 05:07:49.000000 dimples-0.1.6/dimples/conn/protocol/ws.py
+-rw-r--r--   0 moky       (501) staff       (20)     5411 2023-02-23 09:10:59.000000 dimples-0.1.6/dimples/conn/queue.py
+-rw-r--r--   0 moky       (501) staff       (20)     7738 2022-12-14 05:44:44.000000 dimples-0.1.6/dimples/conn/seeker.py
+-rw-r--r--   0 moky       (501) staff       (20)     5726 2023-06-02 09:57:33.000000 dimples-0.1.6/dimples/conn/session.py
+-rw-r--r--   0 moky       (501) staff       (20)     6991 2023-01-14 12:47:37.000000 dimples-0.1.6/dimples/conn/ws.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-09 15:09:56.000000 dimples-0.1.6/dimples/database/
+-rw-r--r--   0 moky       (501) staff       (20)     2560 2023-06-04 16:46:57.000000 dimples-0.1.6/dimples/database/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     7000 2023-06-02 12:26:57.000000 dimples-0.1.6/dimples/database/account.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-09 15:09:56.000000 dimples-0.1.6/dimples/database/dos/
+-rw-r--r--   0 moky       (501) staff       (20)     1808 2023-06-05 05:13:02.000000 dimples-0.1.6/dimples/database/dos/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     4071 2022-12-22 17:59:17.000000 dimples-0.1.6/dimples/database/dos/base.py
+-rw-r--r--   0 moky       (501) staff       (20)     3769 2022-12-11 05:07:49.000000 dimples-0.1.6/dimples/database/dos/document.py
+-rw-r--r--   0 moky       (501) staff       (20)     4232 2023-06-02 10:30:44.000000 dimples-0.1.6/dimples/database/dos/group.py
+-rw-r--r--   0 moky       (501) staff       (20)     3141 2023-06-02 11:02:33.000000 dimples-0.1.6/dimples/database/dos/login.py
+-rw-r--r--   0 moky       (501) staff       (20)     2680 2022-12-22 17:58:13.000000 dimples-0.1.6/dimples/database/dos/meta.py
+-rw-r--r--   0 moky       (501) staff       (20)     5630 2023-06-02 11:04:20.000000 dimples-0.1.6/dimples/database/dos/private.py
+-rw-r--r--   0 moky       (501) staff       (20)     8033 2023-06-09 14:40:24.000000 dimples-0.1.6/dimples/database/dos/station.py
+-rw-r--r--   0 moky       (501) staff       (20)     5625 2023-06-02 11:01:02.000000 dimples-0.1.6/dimples/database/dos/user.py
+-rw-r--r--   0 moky       (501) staff       (20)     3097 2022-12-13 10:56:52.000000 dimples-0.1.6/dimples/database/message.py
+-rw-r--r--   0 moky       (501) staff       (20)     4229 2023-06-04 17:05:32.000000 dimples-0.1.6/dimples/database/session.py
+-rw-r--r--   0 moky       (501) staff       (20)     2972 2023-01-31 05:28:07.000000 dimples-0.1.6/dimples/database/t_cipherkey.py
+-rw-r--r--   0 moky       (501) staff       (20)     3710 2023-06-09 14:19:20.000000 dimples-0.1.6/dimples/database/t_document.py
+-rw-r--r--   0 moky       (501) staff       (20)     7715 2023-06-05 05:41:56.000000 dimples-0.1.6/dimples/database/t_group.py
+-rw-r--r--   0 moky       (501) staff       (20)     3718 2023-06-09 14:19:56.000000 dimples-0.1.6/dimples/database/t_login.py
+-rw-r--r--   0 moky       (501) staff       (20)     5144 2022-12-22 18:03:37.000000 dimples-0.1.6/dimples/database/t_message.py
+-rw-r--r--   0 moky       (501) staff       (20)     3513 2023-06-05 05:36:10.000000 dimples-0.1.6/dimples/database/t_meta.py
+-rw-r--r--   0 moky       (501) staff       (20)     5589 2023-06-05 05:38:08.000000 dimples-0.1.6/dimples/database/t_private.py
+-rw-r--r--   0 moky       (501) staff       (20)     6647 2023-06-05 05:31:39.000000 dimples-0.1.6/dimples/database/t_station.py
+-rw-r--r--   0 moky       (501) staff       (20)     6455 2023-06-05 05:39:18.000000 dimples-0.1.6/dimples/database/t_user.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-09 15:09:56.000000 dimples-0.1.6/dimples/edge/
+-rw-r--r--   0 moky       (501) staff       (20)     2127 2022-12-11 05:07:49.000000 dimples-0.1.6/dimples/edge/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)    13562 2023-06-09 14:59:48.000000 dimples-0.1.6/dimples/edge/octopus.py
+-rw-r--r--   0 moky       (501) staff       (20)     5594 2023-06-05 05:51:39.000000 dimples-0.1.6/dimples/edge/shared.py
+-rw-r--r--   0 moky       (501) staff       (20)     2726 2023-06-04 10:23:09.000000 dimples-0.1.6/dimples/edge/start.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-09 15:09:56.000000 dimples-0.1.6/dimples/register/
+-rw-r--r--   0 moky       (501) staff       (20)     1441 2022-12-11 05:07:49.000000 dimples-0.1.6/dimples/register/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     9516 2023-06-02 10:01:29.000000 dimples-0.1.6/dimples/register/generate.py
+-rw-r--r--   0 moky       (501) staff       (20)     7045 2023-06-02 10:02:10.000000 dimples-0.1.6/dimples/register/modify.py
+-rwxr-xr-x   0 moky       (501) staff       (20)     3880 2022-12-11 05:07:49.000000 dimples-0.1.6/dimples/register/run.py
+-rw-r--r--   0 moky       (501) staff       (20)     1971 2022-12-11 05:07:49.000000 dimples-0.1.6/dimples/register/shared.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-09 15:09:56.000000 dimples-0.1.6/dimples/server/
+-rw-r--r--   0 moky       (501) staff       (20)     2561 2023-06-07 12:19:50.000000 dimples-0.1.6/dimples/server/__init__.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-09 15:09:56.000000 dimples-0.1.6/dimples/server/cpu/
+-rw-r--r--   0 moky       (501) staff       (20)     1855 2023-02-23 09:37:38.000000 dimples-0.1.6/dimples/server/cpu/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     2640 2023-02-23 10:54:44.000000 dimples-0.1.6/dimples/server/cpu/ans.py
+-rw-r--r--   0 moky       (501) staff       (20)     4781 2023-06-03 12:02:30.000000 dimples-0.1.6/dimples/server/cpu/document.py
+-rw-r--r--   0 moky       (501) staff       (20)     3341 2023-04-14 16:24:15.000000 dimples-0.1.6/dimples/server/cpu/handshake.py
+-rw-r--r--   0 moky       (501) staff       (20)     3853 2023-06-03 12:02:46.000000 dimples-0.1.6/dimples/server/cpu/login.py
+-rw-r--r--   0 moky       (501) staff       (20)     1847 2023-01-31 05:28:07.000000 dimples-0.1.6/dimples/server/cpu/receipt.py
+-rw-r--r--   0 moky       (501) staff       (20)     3089 2023-01-31 05:28:07.000000 dimples-0.1.6/dimples/server/cpu/report.py
+-rw-r--r--   0 moky       (501) staff       (20)    13057 2023-06-09 13:06:31.000000 dimples-0.1.6/dimples/server/dispatcher.py
+-rw-r--r--   0 moky       (501) staff       (20)    12816 2023-06-09 13:57:31.000000 dimples-0.1.6/dimples/server/messenger.py
+-rw-r--r--   0 moky       (501) staff       (20)     6659 2023-06-09 08:36:13.000000 dimples-0.1.6/dimples/server/packer.py
+-rw-r--r--   0 moky       (501) staff       (20)     5791 2023-02-23 11:39:56.000000 dimples-0.1.6/dimples/server/processor.py
+-rw-r--r--   0 moky       (501) staff       (20)     6443 2023-06-09 13:36:28.000000 dimples-0.1.6/dimples/server/push_info.py
+-rw-r--r--   0 moky       (501) staff       (20)     6719 2022-12-11 05:07:49.000000 dimples-0.1.6/dimples/server/push_service.py
+-rw-r--r--   0 moky       (501) staff       (20)     5877 2023-06-07 13:18:30.000000 dimples-0.1.6/dimples/server/pusher.py
+-rw-r--r--   0 moky       (501) staff       (20)     7986 2023-01-14 12:19:38.000000 dimples-0.1.6/dimples/server/session.py
+-rw-r--r--   0 moky       (501) staff       (20)     6997 2022-12-11 05:07:49.000000 dimples-0.1.6/dimples/server/session_center.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-09 15:09:56.000000 dimples-0.1.6/dimples/station/
+-rw-r--r--   0 moky       (501) staff       (20)     1549 2023-02-23 13:34:51.000000 dimples-0.1.6/dimples/station/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     4624 2023-06-07 12:21:10.000000 dimples-0.1.6/dimples/station/handler.py
+-rw-r--r--   0 moky       (501) staff       (20)     7087 2023-06-07 11:52:56.000000 dimples-0.1.6/dimples/station/shared.py
+-rwxr-xr-x   0 moky       (501) staff       (20)     3782 2023-06-04 10:23:09.000000 dimples-0.1.6/dimples/station/start.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-09 15:09:56.000000 dimples-0.1.6/dimples/utils/
+-rw-r--r--   0 moky       (501) staff       (20)     2568 2023-02-23 13:38:40.000000 dimples-0.1.6/dimples/utils/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     6447 2022-12-22 12:24:04.000000 dimples-0.1.6/dimples/utils/cache.py
+-rw-r--r--   0 moky       (501) staff       (20)     4016 2023-06-02 18:00:31.000000 dimples-0.1.6/dimples/utils/checker.py
+-rw-r--r--   0 moky       (501) staff       (20)     5978 2022-12-11 05:07:49.000000 dimples-0.1.6/dimples/utils/dos.py
+-rw-r--r--   0 moky       (501) staff       (20)     2805 2022-12-28 05:23:15.000000 dimples-0.1.6/dimples/utils/log.py
+-rw-r--r--   0 moky       (501) staff       (20)     1735 2022-12-11 05:07:49.000000 dimples-0.1.6/dimples/utils/singleton.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-09 15:09:56.000000 dimples-0.1.6/dimples.egg-info/
+-rw-r--r--   0 moky       (501) staff       (20)     1061 2023-06-09 15:09:56.000000 dimples-0.1.6/dimples.egg-info/PKG-INFO
+-rw-r--r--   0 moky       (501) staff       (20)     3247 2023-06-09 15:09:56.000000 dimples-0.1.6/dimples.egg-info/SOURCES.txt
+-rw-r--r--   0 moky       (501) staff       (20)        1 2023-06-09 15:09:56.000000 dimples-0.1.6/dimples.egg-info/dependency_links.txt
+-rw-r--r--   0 moky       (501) staff       (20)      118 2023-06-09 15:09:56.000000 dimples-0.1.6/dimples.egg-info/entry_points.txt
+-rw-r--r--   0 moky       (501) staff       (20)      108 2023-06-09 15:09:56.000000 dimples-0.1.6/dimples.egg-info/requires.txt
+-rw-r--r--   0 moky       (501) staff       (20)        8 2023-06-09 15:09:56.000000 dimples-0.1.6/dimples.egg-info/top_level.txt
+-rw-r--r--   0 moky       (501) staff       (20)       38 2023-06-09 15:09:56.000000 dimples-0.1.6/setup.cfg
+-rw-r--r--   0 moky       (501) staff       (20)     1675 2023-06-09 08:37:55.000000 dimples-0.1.6/setup.py
```

### Comparing `dimples-0.1.5/PKG-INFO` & `dimples-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dimples
-Version: 0.1.5
+Version: 0.1.6
 Summary: DIMP Library for Edges and Stations
 Home-page: https://github.com/dimchat/demo-py
 Author: Albert Moky
 Author-email: albert.moky@gmail.com
 License: MIT
 Description: # DIMP Library for Edges and Stations (Python version)
```

### Comparing `dimples-0.1.5/README.md` & `dimples-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `dimples-0.1.5/dimples/__init__.py` & `dimples-0.1.6/dimples/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.5/dimples/client/__init__.py` & `dimples-0.1.6/dimples/client/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.5/dimples/client/cpu/__init__.py` & `dimples-0.1.6/dimples/client/cpu/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.5/dimples/client/cpu/grp_expel.py` & `dimples-0.1.6/dimples/client/cpu/grp_expel.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.5/dimples/client/cpu/grp_invite.py` & `dimples-0.1.6/dimples/client/cpu/grp_invite.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.5/dimples/client/cpu/grp_query.py` & `dimples-0.1.6/dimples/client/cpu/grp_query.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.5/dimples/client/cpu/grp_quit.py` & `dimples-0.1.6/dimples/client/cpu/grp_quit.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.5/dimples/client/cpu/grp_reset.py` & `dimples-0.1.6/dimples/client/cpu/grp_reset.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.5/dimples/client/cpu/handshake.py` & `dimples-0.1.6/dimples/client/cpu/handshake.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.5/dimples/client/cpu/history.py` & `dimples-0.1.6/dimples/client/cpu/history.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.5/dimples/client/cpu/login.py` & `dimples-0.1.6/dimples/client/cpu/login.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.5/dimples/client/cpu/receipt.py` & `dimples-0.1.6/dimples/client/cpu/receipt.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.5/dimples/client/group.py` & `dimples-0.1.6/dimples/client/group.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.5/dimples/client/messenger.py` & `dimples-0.1.6/dimples/client/messenger.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.5/dimples/client/network/__init__.py` & `dimples-0.1.6/dimples/client/network/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.5/dimples/client/network/session.py` & `dimples-0.1.6/dimples/client/network/session.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.5/dimples/client/network/state.py` & `dimples-0.1.6/dimples/client/network/state.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.5/dimples/client/network/transition.py` & `dimples-0.1.6/dimples/client/network/transition.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.5/dimples/client/packer.py` & `dimples-0.1.6/dimples/client/packer.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.5/dimples/client/processor.py` & `dimples-0.1.6/dimples/client/processor.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.5/dimples/client/terminal.py` & `dimples-0.1.6/dimples/client/terminal.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.5/dimples/common/__init__.py` & `dimples-0.1.6/dimples/common/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.5/dimples/common/ans.py` & `dimples-0.1.6/dimples/common/ans.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.5/dimples/common/dbi/__init__.py` & `dimples-0.1.6/dimples/common/dbi/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -25,27 +25,39 @@
 
 """
     Database Interfaces
     ~~~~~~~~~~~~~~~~~~~
 
 """
 
+from typing import Optional
+
 from .account import PrivateKeyDBI, MetaDBI, DocumentDBI
 from .account import UserDBI, ContactDBI, GroupDBI
 from .account import AccountDBI
 
 from .message import ReliableMessageDBI, CipherKeyDBI
 from .message import MessageDBI
 
 from .session import LoginDBI, ProviderDBI, StationDBI
 from .session import SessionDBI
 from .session import ProviderInfo, StationInfo
 
 
+def is_expired(old_time: Optional[float], new_time: Optional[float]) -> bool:
+    if old_time is None or new_time is None:
+        return False
+    else:
+        return 0 < new_time <= old_time
+
+
 __all__ = [
+
+    'is_expired',
+
     #
     #   Account
     #
     'PrivateKeyDBI', 'MetaDBI', 'DocumentDBI',
     'UserDBI', 'ContactDBI', 'GroupDBI',
     'AccountDBI',
```

### Comparing `dimples-0.1.5/dimples/common/dbi/account.py` & `dimples-0.1.6/dimples/common/dbi/account.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.5/dimples/common/dbi/message.py` & `dimples-0.1.6/dimples/common/dbi/message.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.5/dimples/common/dbi/session.py` & `dimples-0.1.6/dimples/common/dbi/session.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,14 +151,16 @@
             host = item.get('host')
             port = item.get('port')
             provider = ID.parse(identifier=item.get('provider'))
             chosen = item.get('chosen')
             if host is None or port is None:  # or provider is None:
                 # station socket error
                 continue
+            if chosen is None:
+                chosen = 0
             info = StationInfo(identifier=identifier, host=host, port=port, provider=provider, chosen=chosen)
             stations.append(info)
         return stations
 
     # noinspection PyMethodMayBeStatic
     def revert_stations(self, array: List[StationInfo]) -> List[Dict[str, Any]]:
         stations = []
```

### Comparing `dimples-0.1.5/dimples/common/facebook.py` & `dimples-0.1.6/dimples/common/facebook.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.5/dimples/common/messenger.py` & `dimples-0.1.6/dimples/common/messenger.py`

 * *Files 19% similar despite different names*

```diff
@@ -27,23 +27,24 @@
     Common extensions for Messenger
     ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
     Transform and send message
 """
 
 from abc import ABC, abstractmethod
-from typing import Optional, Tuple
+from typing import Optional, Tuple, List
 
-from dimsdk import ID
-from dimsdk import Content, Envelope
+from dimsdk import EntityType, ID
+from dimsdk import ContentType, Content, Envelope
 from dimsdk import InstantMessage, ReliableMessage
 from dimsdk import EntityDelegate, CipherKeyDelegate
 from dimsdk import Messenger, Packer, Processor
 
 from ..utils import Logging
+from ..common import ReceiptCommand
 
 from .dbi import MessageDBI
 
 from .facebook import CommonFacebook
 from .session import Transmitter, Session
 
 
@@ -120,14 +121,48 @@
     #         key.pop('reused', None)
     #     data = super().serialize_key(key=key, msg=msg)
     #     if reused is not None:
     #         # put it back
     #         key['reused'] = reused
     #     return data
 
+    # Override
+    def process_reliable_message(self, msg: ReliableMessage) -> List[ReliableMessage]:
+        # call super
+        responses = super().process_reliable_message(msg=msg)
+        if len(responses) == 0 and self._needs_receipt(msg=msg):
+            current_user = self.facebook.current_user
+            res = ReceiptCommand.create(text='Message received', msg=msg)
+            env = Envelope.create(sender=current_user.identifier, receiver=msg.sender)
+            i_msg = InstantMessage.create(head=env, body=res)
+            s_msg = self.encrypt_message(msg=i_msg)
+            assert s_msg is not None, 'failed to encrypt message: %s -> %s' % (current_user, msg.sender)
+            r_msg = self.sign_message(msg=s_msg)
+            assert r_msg is not None, 'failed to sign message: %s -> %s' % (current_user, msg.sender)
+            responses = [r_msg]
+        return responses
+
+    # noinspection PyMethodMayBeStatic
+    def _needs_receipt(self, msg: ReliableMessage) -> bool:
+        if msg.type == ContentType.COMMAND:
+            # filter for looping message (receipt for receipt)
+            return False
+        sender = msg.sender
+        receiver = msg.receiver
+        if sender.type == EntityType.STATION or sender.type == EntityType.BOT:
+            if receiver.type == EntityType.STATION or receiver.type == EntityType.BOT:
+                # message between bots
+                return False
+        # current_user = self.facebook.current_user
+        # if receiver != current_user.identifier:
+        #     # forward message
+        #     return True
+        # TODO: other condition?
+        return True
+
     #
     #   Interfaces for Transmitting Message
     #
 
     # Override
     def send_content(self, sender: Optional[ID], receiver: ID, content: Content,
                      priority: int = 0) -> Tuple[InstantMessage, Optional[ReliableMessage]]:
```

### Comparing `dimples-0.1.5/dimples/common/packer.py` & `dimples-0.1.6/dimples/common/packer.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.5/dimples/common/protocol/__init__.py` & `dimples-0.1.6/dimples/common/protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.5/dimples/common/protocol/ans.py` & `dimples-0.1.6/dimples/common/protocol/ans.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.5/dimples/common/protocol/handshake.py` & `dimples-0.1.6/dimples/common/protocol/handshake.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.5/dimples/common/protocol/login.py` & `dimples-0.1.6/dimples/common/protocol/login.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.5/dimples/common/protocol/receipt.py` & `dimples-0.1.6/dimples/common/protocol/receipt.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.5/dimples/common/protocol/report.py` & `dimples-0.1.6/dimples/common/protocol/report.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.5/dimples/common/session.py` & `dimples-0.1.6/dimples/common/session.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.5/dimples/config.py` & `dimples-0.1.6/dimples/config.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.5/dimples/conn/__init__.py` & `dimples-0.1.6/dimples/conn/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.5/dimples/conn/gate.py` & `dimples-0.1.6/dimples/conn/gate.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.5/dimples/conn/gatekeeper.py` & `dimples-0.1.6/dimples/conn/gatekeeper.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.5/dimples/conn/mars.py` & `dimples-0.1.6/dimples/conn/mars.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.5/dimples/conn/mtp.py` & `dimples-0.1.6/dimples/conn/mtp.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.5/dimples/conn/protocol/__init__.py` & `dimples-0.1.6/dimples/conn/protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.5/dimples/conn/protocol/mars.py` & `dimples-0.1.6/dimples/conn/protocol/mars.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.5/dimples/conn/protocol/ws.py` & `dimples-0.1.6/dimples/conn/protocol/ws.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.5/dimples/conn/queue.py` & `dimples-0.1.6/dimples/conn/queue.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.5/dimples/conn/seeker.py` & `dimples-0.1.6/dimples/conn/seeker.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.5/dimples/conn/session.py` & `dimples-0.1.6/dimples/conn/session.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.5/dimples/conn/ws.py` & `dimples-0.1.6/dimples/conn/ws.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.5/dimples/database/__init__.py` & `dimples-0.1.6/dimples/database/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.5/dimples/database/account.py` & `dimples-0.1.6/dimples/database/account.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.5/dimples/database/dos/__init__.py` & `dimples-0.1.6/dimples/database/dos/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.5/dimples/database/dos/base.py` & `dimples-0.1.6/dimples/database/dos/base.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.5/dimples/database/dos/document.py` & `dimples-0.1.6/dimples/database/dos/document.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.5/dimples/database/dos/group.py` & `dimples-0.1.6/dimples/database/dos/group.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.5/dimples/database/dos/login.py` & `dimples-0.1.6/dimples/database/dos/login.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.5/dimples/database/dos/meta.py` & `dimples-0.1.6/dimples/database/dos/meta.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.5/dimples/database/dos/private.py` & `dimples-0.1.6/dimples/database/dos/private.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.5/dimples/database/dos/station.py` & `dimples-0.1.6/dimples/database/dos/station.py`

 * *Files 1% similar despite different names*

```diff
@@ -168,15 +168,16 @@
                     return True
                 info = item
                 break
         if info is None:
             info = StationInfo(identifier=identifier, host=host, port=port, provider=provider, chosen=chosen)
             stations.insert(0, info)
         else:
-            info.identifier = identifier
+            if not (identifier is None or identifier.is_broadcast):
+                info.identifier = identifier
             info.chosen = chosen
         return self._save_stations(stations=stations, provider=provider)
 
     # Override
     def remove_station(self, host: str, port: int, provider: ID) -> bool:
         """ remove station with SP ID """
         stations = self.all_stations(provider=provider)
```

### Comparing `dimples-0.1.5/dimples/database/dos/user.py` & `dimples-0.1.6/dimples/database/dos/user.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.5/dimples/database/message.py` & `dimples-0.1.6/dimples/database/message.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.5/dimples/database/session.py` & `dimples-0.1.6/dimples/database/session.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.5/dimples/database/t_cipherkey.py` & `dimples-0.1.6/dimples/database/t_cipherkey.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.5/dimples/database/t_document.py` & `dimples-0.1.6/dimples/database/t_document.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 import time
 from typing import Optional
 
 from dimsdk import ID, Document
 
 from ..utils import CacheManager
 from ..common import DocumentDBI
+from ..common.dbi import is_expired
 
 from .dos import DocumentStorage
 
 
 class DocumentTable(DocumentDBI):
     """ Implementations of DocumentDBI """
 
@@ -53,15 +54,15 @@
     # Override
     def save_document(self, document: Document) -> bool:
         assert document.valid, 'document invalid: %s' % document
         identifier = document.identifier
         doc_type = document.type
         # 0. check old record with time
         old = self.document(identifier=identifier, doc_type=doc_type)
-        if old is not None and 0 < document.time < old.time:
+        if old is not None and is_expired(old_time=old.time, new_time=document.time):
             # document expired, drop it
             return False
         # 1. store into memory cache
         self.__doc_cache.update(key=identifier, value=document, life_span=600)
         # 2. store into local storage
         return self.__doc_storage.save_document(document=document)
```

### Comparing `dimples-0.1.5/dimples/database/t_group.py` & `dimples-0.1.6/dimples/database/t_group.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.5/dimples/database/t_login.py` & `dimples-0.1.6/dimples/database/t_login.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 from typing import Optional, Tuple
 
 from dimsdk import ID
 from dimsdk import ReliableMessage
 
 from ..utils import CacheManager
 from ..common import LoginDBI, LoginCommand
+from ..common.dbi import is_expired
 
 from .dos import LoginStorage
 
 
 class LoginTable(LoginDBI):
     """ Implementations of LoginDBI """
 
@@ -72,14 +73,14 @@
         # OK, return cached value
         return value
 
     # Override
     def save_login_command_message(self, user: ID, content: LoginCommand, msg: ReliableMessage) -> bool:
         # 1. check old record
         old, _ = self.login_command_message(user=user)
-        if isinstance(old, LoginCommand) and old.time >= content.time > 0:
+        if isinstance(old, LoginCommand) and is_expired(old_time=old.time, new_time=content.time):
             # command expired
             return False
         # 2. store into memory cache
         self.__login_cache.update(key=user, value=(content, msg), life_span=600)
         # 3. store into local storage
         return self.__login_storage.save_login_command_message(user=user, content=content, msg=msg)
```

### Comparing `dimples-0.1.5/dimples/database/t_message.py` & `dimples-0.1.6/dimples/database/t_message.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.5/dimples/database/t_meta.py` & `dimples-0.1.6/dimples/database/t_meta.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.5/dimples/database/t_private.py` & `dimples-0.1.6/dimples/database/t_private.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.5/dimples/database/t_station.py` & `dimples-0.1.6/dimples/database/t_station.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.5/dimples/database/t_user.py` & `dimples-0.1.6/dimples/database/t_user.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.5/dimples/edge/__init__.py` & `dimples-0.1.6/dimples/edge/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.5/dimples/edge/octopus.py` & `dimples-0.1.6/dimples/edge/octopus.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,18 +35,20 @@
 import weakref
 from abc import ABC, abstractmethod
 from typing import Optional, List, Set
 
 from dimsdk import ContentType
 from dimsdk import EntityType, ID
 from dimsdk import ReliableMessage
+from dimsdk import Station
 
-from ..utils import Logging
+from ..utils import Log, Logging
 from ..utils import Runner
 from ..common import CommonFacebook
+from ..common import ProviderInfo
 from ..common import MessageDBI, SessionDBI
 from ..common import HandshakeCommand
 from ..conn.session import get_sig
 
 from ..client import ClientSession
 from ..client import ClientMessenger
 from ..client import ClientMessagePacker
@@ -259,62 +261,63 @@
             self.error(msg='drop cycled msg(type=%d): %s -> %s | from %s, traces: %s'
                        % (msg.type, msg.sender, msg.receiver, get_remote_station(messenger=self), msg.get('traces')))
             return []
         # handshake accepted, redirecting message
         sig = get_sig(msg=msg)
         self.info(msg='redirect msg(type=%d, sig=%s): %s -> %s | from %s, traces: %s'
                   % (msg.type, sig, msg.sender, msg.receiver, get_remote_station(messenger=self), msg.get('traces')))
-        return self.deliver_message(msg=msg)
+        return self._deliver_message(msg=msg)
 
     @abstractmethod
-    def deliver_message(self, msg: ReliableMessage) -> List[ReliableMessage]:
+    def _deliver_message(self, msg: ReliableMessage) -> List[ReliableMessage]:
         """ call octopus to redirect message """
         pass
 
 
 def get_remote_station(messenger: ClientMessenger) -> ID:
     session = messenger.session
     station = session.station
     return station.identifier
 
 
 class InnerMessenger(OctopusMessenger):
     """ Messenger for local station """
 
     # Override
-    def deliver_message(self, msg: ReliableMessage) -> List[ReliableMessage]:
+    def _deliver_message(self, msg: ReliableMessage) -> List[ReliableMessage]:
         priority = 0  # NORMAL
         if msg.receiver.is_broadcast:
             priority = 1  # SLOWER
         octopus = self.octopus
         return octopus.outgo_message(msg=msg, priority=priority)
 
 
 class OuterMessenger(OctopusMessenger):
     """ Messenger for remote station """
 
     # Override
-    def process_reliable_message(self, msg: ReliableMessage) -> List[ReliableMessage]:
-        if msg.sender == self.local_station:
-            self.debug(msg='cycled message from this station: %s => %s' % (msg.sender, msg.receiver))
-            return []
-        return super().process_reliable_message(msg=msg)
-
-    # Override
-    def deliver_message(self, msg: ReliableMessage) -> List[ReliableMessage]:
+    def _deliver_message(self, msg: ReliableMessage) -> List[ReliableMessage]:
         priority = 0  # NORMAL
         if msg.receiver.is_broadcast:
             priority = 1  # SLOWER
         octopus = self.octopus
         return octopus.income_message(msg=msg, priority=priority)
 
     # Override
+    def process_reliable_message(self, msg: ReliableMessage) -> List[ReliableMessage]:
+        if msg.sender == self.local_station:
+            self.debug(msg='cycled message from this station: %s => %s' % (msg.sender, msg.receiver))
+            return []
+        return super().process_reliable_message(msg=msg)
+
+    # Override
     def handshake_success(self):
         super().handshake_success()
         station = self.session.station
+        update_station(station=station)
         octopus = self.octopus
         octopus.add_index(identifier=station.identifier, terminal=self.terminal)
 
 
 def create_messenger(facebook: CommonFacebook, database: MessageDBI,
                      session: ClientSession, messenger_class) -> OctopusMessenger:
     assert issubclass(messenger_class, OctopusMessenger), 'messenger class error: %s' % messenger_class
@@ -330,7 +333,24 @@
 
 
 def create_terminal(messenger: OctopusMessenger) -> Terminal:
     terminal = Terminal(messenger=messenger)
     messenger.terminal = terminal
     terminal.start()
     return terminal
+
+
+def update_station(station: Station):
+    Log.info(msg='update station: %s' % station)
+    shared = GlobalVariable()
+    db = shared.sdb
+    # SP ID
+    provider = station.provider
+    if provider is None:
+        provider = ProviderInfo.GSP
+    # new info
+    sid = station.identifier
+    host = station.host
+    port = station.port
+    assert not sid.is_broadcast, 'station ID error: %s' % sid
+    assert host is not None and port > 0, 'station error: %s, %d' % (host, port)
+    db.update_station(identifier=sid, host=host, port=port, provider=provider, chosen=0)
```

### Comparing `dimples-0.1.5/dimples/edge/shared.py` & `dimples-0.1.6/dimples/edge/shared.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.5/dimples/edge/start.py` & `dimples-0.1.6/dimples/edge/start.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.5/dimples/register/__init__.py` & `dimples-0.1.6/dimples/register/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.5/dimples/register/generate.py` & `dimples-0.1.6/dimples/register/generate.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.5/dimples/register/modify.py` & `dimples-0.1.6/dimples/register/modify.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.5/dimples/register/run.py` & `dimples-0.1.6/dimples/register/run.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.5/dimples/register/shared.py` & `dimples-0.1.6/dimples/register/shared.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.5/dimples/server/__init__.py` & `dimples-0.1.6/dimples/server/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.5/dimples/server/cpu/__init__.py` & `dimples-0.1.6/dimples/server/cpu/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.5/dimples/server/cpu/ans.py` & `dimples-0.1.6/dimples/server/cpu/ans.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.5/dimples/server/cpu/document.py` & `dimples-0.1.6/dimples/server/cpu/document.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.5/dimples/server/cpu/handshake.py` & `dimples-0.1.6/dimples/server/cpu/handshake.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.5/dimples/server/cpu/login.py` & `dimples-0.1.6/dimples/server/cpu/login.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.5/dimples/server/cpu/receipt.py` & `dimples-0.1.6/dimples/server/cpu/receipt.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.5/dimples/server/cpu/report.py` & `dimples-0.1.6/dimples/server/cpu/report.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.5/dimples/server/dispatcher.py` & `dimples-0.1.6/dimples/server/dispatcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,14 +112,18 @@
     def pusher(self) -> Pusher:
         return self.__pusher
 
     @pusher.setter
     def pusher(self, service: Pusher):
         self.__pusher = service
 
+    @property
+    def worker(self):  # -> DeliverWorker:
+        return self.__worker
+
     def start(self):
         worker = DeliverWorker(database=self.__sdb, facebook=self.__facebook)
         roamer = Roamer(database=self.__mdb)
         self.__worker = worker
         self.__roamer = roamer
         roamer.start()
 
@@ -236,17 +240,18 @@
                 info.start_pos = start + limit
                 self.__append(info=info)
             elif cached_messages is None or len(cached_messages) == 0:
                 self.debug(msg='no cached message for this user: %s' % receiver)
                 return True
             # get deliver delegate for receiver
             dispatcher = Dispatcher()
+            worker = dispatcher.worker
             # deliver cached messages one by one
             for msg in cached_messages:
-                dispatcher.deliver_message(msg=msg, receiver=receiver)
+                worker.push_message(msg=msg, receiver=receiver)
         except Exception as e:
             self.error(msg='process roaming user (%s => %s) error: %s' % (receiver, roaming, e))
         # return True to process next immediately
         return True
 
     def start(self):
         thread = threading.Thread(target=self.run, daemon=True)
```

### Comparing `dimples-0.1.5/dimples/server/messenger.py` & `dimples-0.1.6/dimples/server/messenger.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 from .packer import FilterManager
 from .dispatcher import Dispatcher
 from .session_center import SessionCenter
 
 
 class ServerMessenger(CommonMessenger):
 
-    def broadcast_reliable_message(self, msg: ReliableMessage, station: ID) -> int:
+    def __broadcast_reliable_message(self, msg: ReliableMessage, station: ID) -> int:
         receiver = msg.receiver
         db = self.session.database
         # get other recipients
         recipients = get_recipients(msg=msg, receiver=receiver, db=db)
         if len(recipients) == 0:
             Log.warning('other recipients not found: %s' % receiver)
             return 0
@@ -85,15 +85,15 @@
     def __broadcast_command(self, content: Command, receiver: ID):
         sid = self.facebook.current_user.identifier
         env = Envelope.create(sender=sid, receiver=receiver)
         i_msg = InstantMessage.create(head=env, body=content)
         # pack & deliver message
         s_msg = self.encrypt_message(msg=i_msg)
         r_msg = self.sign_message(msg=s_msg)
-        self.broadcast_reliable_message(msg=r_msg, station=sid)
+        self.__broadcast_reliable_message(msg=r_msg, station=sid)
 
     # Override
     def query_meta(self, identifier: ID) -> bool:
         checker = QueryFrequencyChecker()
         if not checker.meta_query_expired(identifier=identifier):
             # query not expired yet
             self.debug(msg='meta query not expired yet: %s' % identifier)
@@ -130,51 +130,58 @@
     def verify_message(self, msg: ReliableMessage) -> Optional[SecureMessage]:
         # check block list
         if self.is_blocked(msg=msg):
             self.warning(msg='user is blocked: %s -> %s (group: %s)' % (msg.sender, msg.receiver, msg.group))
             return None
         sender = msg.sender
         receiver = msg.receiver
-        facebook = self.facebook
-        current = facebook.current_user
+        current = self.facebook.current_user
+        sid = current.identifier
         # 1. verify message
         s_msg = super().verify_message(msg=msg)
-        if receiver == current.identifier:
+        if receiver == sid:
             # message to this station
             # maybe a meta command, document command, etc ...
             return s_msg
         elif receiver.is_broadcast:
             # if receiver == 'station@anywhere':
             #     it must be the first handshake without station ID;
             # if receiver == 'anyone@anywhere':
             #     it should be other plain message without encryption.
             # if receiver.is_group:
             #     broadcast message to multiple destinations,
             #     current station is it's receiver too.
+            if receiver.is_group:
+                # broadcast to neighbor stations
+                self.__broadcast_reliable_message(msg=msg, station=sid)
+            elif receiver == 'archivist@anywhere':
+                # forward to search bot
+                self.__broadcast_reliable_message(msg=msg, station=sid)
+                return None
             return s_msg
         elif receiver.is_group:
             self.error(msg='group message should not send to station: %s -> %s' % (sender, receiver))
             return None
 
         # 2. check session for delivering
         session = self.session
         if session.identifier is None or not session.active:
             # not login? ask client to handshake again (with session key)
             # this message won't be delivered before handshake accepted
             cmd = HandshakeCommand.ask(session=session.key)
-            self.send_content(sender=current.identifier, receiver=sender, content=cmd)
+            self.send_content(sender=sid, receiver=sender, content=cmd)
             # DISCUSS: suspend this message for waiting handshake accepted
             #          or let the client to send it again?
             return None
         # session is active, so this message is not for current station,
         # deliver to the real receiver and respond to sender
         dispatcher = Dispatcher()
         responses = dispatcher.deliver_message(msg=msg, receiver=receiver)
         for res in responses:
-            self.send_content(sender=current.identifier, receiver=sender, content=res)
+            self.send_content(sender=sid, receiver=sender, content=res)
 
     # Override
     def process_reliable_message(self, msg: ReliableMessage) -> List[ReliableMessage]:
         # call super
         responses = super().process_reliable_message(msg=msg)
         current = self.facebook.current_user
         sid = current.identifier
@@ -263,35 +270,36 @@
     # get nodes passed through, includes current node which is just added before
     traces = msg.get('traces')
     if traces is None:
         traces = []
     # if this message is sending to 'stations@everywhere' or 'everyone@everywhere'
     # get all neighbor stations to broadcast, but
     # traced nodes should be ignored to avoid cycled delivering
-    if receiver == Station.EVERY or recipients == EVERYONE:
-        Log.debug(msg='forward to neighbors: %s' % receiver)
+    if receiver == Station.EVERY or receiver == EVERYONE:
+        Log.info(msg='forward to neighbors: %s' % receiver)
         # get neighbor stations
         neighbors = get_neighbors(db=db)
         for sid in neighbors:
             if sid not in traces:  # and sid != station:
                 recipients.add(sid)
             else:
                 Log.warning(msg='ignore neighbor: %s' % sid)
         # get archivist bot
         if receiver == EVERYONE:
             # include 'archivist' as 'everyone@everywhere'
             bot = ans_id(name='archivist')
             if bot is not None and bot not in traces:
                 recipients.add(bot)
-    # elif receiver == 'archivist@anywhere' or receiver == 'archivists@everywhere':
-    #     Log.debug(msg='forward to archivist: %s' % receiver)
-    #     # get archivist bot for search command
-    #     bot = ans_id(name='archivist')
-    #     if bot is not None and bot not in traces:
-    #         recipients.add(bot)
+    elif receiver == 'archivist@anywhere' or receiver == 'archivists@everywhere':
+        Log.info(msg='forward to archivist: %s' % receiver)
+        # get archivist bot for search command
+        bot = ans_id(name='archivist')
+        if bot is not None and bot not in traces:
+            recipients.add(bot)
+    Log.info(msg='recipients: %s -> %s' % (receiver, recipients))
     return recipients
 
 
 def ans_id(name: str) -> Optional[ID]:
     try:
         return ID.parse(identifier=name)
     except ValueError as e:
```

### Comparing `dimples-0.1.5/dimples/server/packer.py` & `dimples-0.1.6/dimples/server/packer.py`

 * *Files 10% similar despite different names*

```diff
@@ -116,37 +116,15 @@
 
     # Override
     def _check_reliable_message_receiver(self, msg: ReliableMessage) -> bool:
         # skip for "super().verify_message(msg=msg)"
         return True
 
     def __check_reliable_message_receiver(self, msg: ReliableMessage) -> bool:
-        node = self.__current()
-        receiver = msg.receiver
-        if receiver.is_broadcast:
-            if receiver.is_group:
-                # broadcast to neighbor stations
-                messenger = get_messenger(packer=self)
-                messenger.broadcast_reliable_message(msg=msg, station=node)
-            # elif receiver == 'archivist@anywhere':
-            #     # forward to search bot
-            #     pass
-            else:
-                # broadcast message to single destination
-                # if receiver == 'station@anywhere',
-                #     it must be the first handshake without station ID;
-                # if receiver == 'anyone@anywhere',
-                #     it should be other plain message without encryption.
-                pass
-            # OK
-            return True
-        # elif receiver.is_group:
-        #     sender = msg.sender
-        #     self.error(msg='Should not send group message to a station!! %s -> %s' % (sender, receiver))
-        #     return False
+        # check for group
         return super()._check_reliable_message_receiver(msg=msg)
 
 
 def get_facebook(packer: CommonMessagePacker) -> CommonFacebook:
     barrack = packer.facebook
     assert isinstance(barrack, CommonFacebook), 'facebook error: %s' % barrack
     return barrack
```

### Comparing `dimples-0.1.5/dimples/server/processor.py` & `dimples-0.1.6/dimples/server/processor.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.5/dimples/server/push_info.py` & `dimples-0.1.6/dimples/server/push_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -169,15 +169,15 @@
         return self.to_json()
 
     def __repr__(self) -> str:
         return self.to_json()
 
     def to_json(self) -> str:
         info = {
-            'alert': self.__alert
+            'alert': self.__alert.to_json()
         }
         if self.__title is not None:
             info['title'] = self.__title
         if self.__content is not None:
             info['content'] = self.__content
         if self.__sound is not None:
             info['sound'] = self.__sound
```

### Comparing `dimples-0.1.5/dimples/server/push_service.py` & `dimples-0.1.6/dimples/server/push_service.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.5/dimples/server/pusher.py` & `dimples-0.1.6/dimples/server/pusher.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.5/dimples/server/session.py` & `dimples-0.1.6/dimples/server/session.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.5/dimples/server/session_center.py` & `dimples-0.1.6/dimples/server/session_center.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.5/dimples/station/__init__.py` & `dimples-0.1.6/dimples/station/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.5/dimples/station/handler.py` & `dimples-0.1.6/dimples/station/handler.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.5/dimples/station/shared.py` & `dimples-0.1.6/dimples/station/shared.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.5/dimples/station/start.py` & `dimples-0.1.6/dimples/station/start.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.5/dimples/utils/__init__.py` & `dimples-0.1.6/dimples/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.5/dimples/utils/cache.py` & `dimples-0.1.6/dimples/utils/cache.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.5/dimples/utils/checker.py` & `dimples-0.1.6/dimples/utils/checker.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.5/dimples/utils/dos.py` & `dimples-0.1.6/dimples/utils/dos.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.5/dimples/utils/log.py` & `dimples-0.1.6/dimples/utils/log.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.5/dimples/utils/singleton.py` & `dimples-0.1.6/dimples/utils/singleton.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.5/dimples.egg-info/PKG-INFO` & `dimples-0.1.6/dimples.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dimples
-Version: 0.1.5
+Version: 0.1.6
 Summary: DIMP Library for Edges and Stations
 Home-page: https://github.com/dimchat/demo-py
 Author: Albert Moky
 Author-email: albert.moky@gmail.com
 License: MIT
 Description: # DIMP Library for Edges and Stations (Python version)
```

### Comparing `dimples-0.1.5/dimples.egg-info/SOURCES.txt` & `dimples-0.1.6/dimples.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dimples-0.1.5/setup.py` & `dimples-0.1.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     communications between accounts safely by end-to-end encryption.
 """
 
 import io
 
 from setuptools import setup, find_packages
 
-__version__ = '0.1.5'
+__version__ = '0.1.6'
 __author__ = 'Albert Moky'
 __contact__ = 'albert.moky@gmail.com'
 
 with io.open('README.md', 'r', encoding='utf-8') as fh:
     readme = fh.read()
 
 setup(
```

