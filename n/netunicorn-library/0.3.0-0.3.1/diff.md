# Comparing `tmp/netunicorn-library-0.3.0.tar.gz` & `tmp/netunicorn-library-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netunicorn-library-0.3.0.tar", last modified: Wed May 10 08:30:19 2023, max compression
+gzip compressed data, was "netunicorn-library-0.3.1.tar", last modified: Fri Jun  9 05:08:52 2023, max compression
```

## Comparing `netunicorn-library-0.3.0.tar` & `netunicorn-library-0.3.1.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:30:19.302367 netunicorn-library-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-10 08:30:19.302367 netunicorn-library-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-10 08:30:04.000000 netunicorn-library-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 08:30:19.302367 netunicorn-library-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:30:19.294367 netunicorn-library-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:30:19.294367 netunicorn-library-0.3.0/src/netunicorn/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:30:19.294367 netunicorn-library-0.3.0/src/netunicorn/library/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 08:30:04.000000 netunicorn-library-0.3.0/src/netunicorn/library/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:30:19.294367 netunicorn-library-0.3.0/src/netunicorn/library/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 08:30:04.000000 netunicorn-library-0.3.0/src/netunicorn/library/pipelines/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:30:19.294367 netunicorn-library-0.3.0/src/netunicorn/library/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 08:30:04.000000 netunicorn-library-0.3.0/src/netunicorn/library/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-10 08:30:04.000000 netunicorn-library-0.3.0/src/netunicorn/library/tasks/basic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:30:19.294367 netunicorn-library-0.3.0/src/netunicorn/library/tasks/capture/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 08:30:04.000000 netunicorn-library-0.3.0/src/netunicorn/library/tasks/capture/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-05-10 08:30:04.000000 netunicorn-library-0.3.0/src/netunicorn/library/tasks/capture/tcpdump.py
--rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-05-10 08:30:04.000000 netunicorn-library-0.3.0/src/netunicorn/library/tasks/flags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:30:19.294367 netunicorn-library-0.3.0/src/netunicorn/library/tasks/letsencrypt/
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-05-10 08:30:04.000000 netunicorn-library-0.3.0/src/netunicorn/library/tasks/letsencrypt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-05-10 08:30:04.000000 netunicorn-library-0.3.0/src/netunicorn/library/tasks/letsencrypt/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:30:19.294367 netunicorn-library-0.3.0/src/netunicorn/library/tasks/measurements/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 08:30:04.000000 netunicorn-library-0.3.0/src/netunicorn/library/tasks/measurements/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-10 08:30:04.000000 netunicorn-library-0.3.0/src/netunicorn/library/tasks/measurements/ookla_speedtest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-05-10 08:30:04.000000 netunicorn-library-0.3.0/src/netunicorn/library/tasks/measurements/ping.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:30:19.294367 netunicorn-library-0.3.0/src/netunicorn/library/tasks/network_attacks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 08:30:04.000000 netunicorn-library-0.3.0/src/netunicorn/library/tasks/network_attacks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:30:19.298367 netunicorn-library-0.3.0/src/netunicorn/library/tasks/network_attacks/arp/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-10 08:30:04.000000 netunicorn-library-0.3.0/src/netunicorn/library/tasks/network_attacks/arp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-10 08:30:04.000000 netunicorn-library-0.3.0/src/netunicorn/library/tasks/network_attacks/arp/spoof.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:30:19.298367 netunicorn-library-0.3.0/src/netunicorn/library/tasks/network_attacks/cve202141773/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-10 08:30:04.000000 netunicorn-library-0.3.0/src/netunicorn/library/tasks/network_attacks/cve202141773/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:30:19.298367 netunicorn-library-0.3.0/src/netunicorn/library/tasks/network_attacks/heartbleed/
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-05-10 08:30:04.000000 netunicorn-library-0.3.0/src/netunicorn/library/tasks/network_attacks/heartbleed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-05-10 08:30:04.000000 netunicorn-library-0.3.0/src/netunicorn/library/tasks/network_attacks/heartbleed/heartbleeder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:30:19.298367 netunicorn-library-0.3.0/src/netunicorn/library/tasks/network_attacks/icmp/
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-10 08:30:04.000000 netunicorn-library-0.3.0/src/netunicorn/library/tasks/network_attacks/icmp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-10 08:30:04.000000 netunicorn-library-0.3.0/src/netunicorn/library/tasks/network_attacks/icmp/redirection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:30:19.298367 netunicorn-library-0.3.0/src/netunicorn/library/tasks/network_attacks/land/
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-10 08:30:04.000000 netunicorn-library-0.3.0/src/netunicorn/library/tasks/network_attacks/land/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-10 08:30:04.000000 netunicorn-library-0.3.0/src/netunicorn/library/tasks/network_attacks/land/landattack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:30:19.298367 netunicorn-library-0.3.0/src/netunicorn/library/tasks/network_attacks/log4j/
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-10 08:30:04.000000 netunicorn-library-0.3.0/src/netunicorn/library/tasks/network_attacks/log4j/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:30:19.298367 netunicorn-library-0.3.0/src/netunicorn/library/tasks/network_attacks/loris/
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-05-10 08:30:04.000000 netunicorn-library-0.3.0/src/netunicorn/library/tasks/network_attacks/loris/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-05-10 08:30:04.000000 netunicorn-library-0.3.0/src/netunicorn/library/tasks/network_attacks/loris/slowloris.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-05-10 08:30:04.000000 netunicorn-library-0.3.0/src/netunicorn/library/tasks/network_attacks/loris/smbloris.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:30:19.298367 netunicorn-library-0.3.0/src/netunicorn/library/tasks/network_attacks/mac/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-10 08:30:04.000000 netunicorn-library-0.3.0/src/netunicorn/library/tasks/network_attacks/mac/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-10 08:30:04.000000 netunicorn-library-0.3.0/src/netunicorn/library/tasks/network_attacks/mac/flooder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:30:19.298367 netunicorn-library-0.3.0/src/netunicorn/library/tasks/network_attacks/mail/
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-05-10 08:30:04.000000 netunicorn-library-0.3.0/src/netunicorn/library/tasks/network_attacks/mail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-10 08:30:04.000000 netunicorn-library-0.3.0/src/netunicorn/library/tasks/network_attacks/mail/fake_mail.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:30:19.298367 netunicorn-library-0.3.0/src/netunicorn/library/tasks/qoe_youtube/
--rw-r--r--   0 runner    (1001) docker     (123)     7243 2023-05-10 08:30:04.000000 netunicorn-library-0.3.0/src/netunicorn/library/tasks/qoe_youtube/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-05-10 08:30:04.000000 netunicorn-library-0.3.0/src/netunicorn/library/tasks/qoe_youtube/qoe_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     6461 2023-05-10 08:30:04.000000 netunicorn-library-0.3.0/src/netunicorn/library/tasks/qoe_youtube/watcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:30:19.298367 netunicorn-library-0.3.0/src/netunicorn/library/tasks/upload/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 08:30:04.000000 netunicorn-library-0.3.0/src/netunicorn/library/tasks/upload/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-05-10 08:30:04.000000 netunicorn-library-0.3.0/src/netunicorn/library/tasks/upload/webdav.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:30:19.298367 netunicorn-library-0.3.0/src/netunicorn/library/tasks/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 08:30:04.000000 netunicorn-library-0.3.0/src/netunicorn/library/tasks/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-05-10 08:30:04.000000 netunicorn-library-0.3.0/src/netunicorn/library/tasks/utils/sleep.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:30:19.298367 netunicorn-library-0.3.0/src/netunicorn/library/tasks/video_watchers/
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-10 08:30:04.000000 netunicorn-library-0.3.0/src/netunicorn/library/tasks/video_watchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-05-10 08:30:04.000000 netunicorn-library-0.3.0/src/netunicorn/library/tasks/video_watchers/twitch_watcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     3885 2023-05-10 08:30:04.000000 netunicorn-library-0.3.0/src/netunicorn/library/tasks/video_watchers/vimeo_watcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     4585 2023-05-10 08:30:04.000000 netunicorn-library-0.3.0/src/netunicorn/library/tasks/video_watchers/youtube_watcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:30:19.298367 netunicorn-library-0.3.0/src/netunicorn_library.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-10 08:30:19.000000 netunicorn-library-0.3.0/src/netunicorn_library.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-05-10 08:30:19.000000 netunicorn-library-0.3.0/src/netunicorn_library.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 08:30:19.000000 netunicorn-library-0.3.0/src/netunicorn_library.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-10 08:30:19.000000 netunicorn-library-0.3.0/src/netunicorn_library.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-10 08:30:19.000000 netunicorn-library-0.3.0/src/netunicorn_library.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 05:08:52.934393 netunicorn-library-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-09 05:08:52.934393 netunicorn-library-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-09 05:08:39.000000 netunicorn-library-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 05:08:52.934393 netunicorn-library-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 05:08:52.922392 netunicorn-library-0.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 05:08:52.918392 netunicorn-library-0.3.1/src/netunicorn/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 05:08:52.922392 netunicorn-library-0.3.1/src/netunicorn/library/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 05:08:39.000000 netunicorn-library-0.3.1/src/netunicorn/library/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 05:08:52.922392 netunicorn-library-0.3.1/src/netunicorn/library/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 05:08:39.000000 netunicorn-library-0.3.1/src/netunicorn/library/pipelines/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 05:08:52.922392 netunicorn-library-0.3.1/src/netunicorn/library/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 05:08:39.000000 netunicorn-library-0.3.1/src/netunicorn/library/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-09 05:08:39.000000 netunicorn-library-0.3.1/src/netunicorn/library/tasks/basic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 05:08:52.922392 netunicorn-library-0.3.1/src/netunicorn/library/tasks/capture/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 05:08:39.000000 netunicorn-library-0.3.1/src/netunicorn/library/tasks/capture/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-06-09 05:08:39.000000 netunicorn-library-0.3.1/src/netunicorn/library/tasks/capture/tcpdump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-06-09 05:08:39.000000 netunicorn-library-0.3.1/src/netunicorn/library/tasks/flags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 05:08:52.926392 netunicorn-library-0.3.1/src/netunicorn/library/tasks/letsencrypt/
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-06-09 05:08:39.000000 netunicorn-library-0.3.1/src/netunicorn/library/tasks/letsencrypt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-06-09 05:08:39.000000 netunicorn-library-0.3.1/src/netunicorn/library/tasks/letsencrypt/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 05:08:52.926392 netunicorn-library-0.3.1/src/netunicorn/library/tasks/measurements/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 05:08:39.000000 netunicorn-library-0.3.1/src/netunicorn/library/tasks/measurements/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-06-09 05:08:39.000000 netunicorn-library-0.3.1/src/netunicorn/library/tasks/measurements/ookla_speedtest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-06-09 05:08:39.000000 netunicorn-library-0.3.1/src/netunicorn/library/tasks/measurements/ping.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 05:08:52.926392 netunicorn-library-0.3.1/src/netunicorn/library/tasks/network_attacks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 05:08:39.000000 netunicorn-library-0.3.1/src/netunicorn/library/tasks/network_attacks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 05:08:52.926392 netunicorn-library-0.3.1/src/netunicorn/library/tasks/network_attacks/arp/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-09 05:08:39.000000 netunicorn-library-0.3.1/src/netunicorn/library/tasks/network_attacks/arp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-06-09 05:08:39.000000 netunicorn-library-0.3.1/src/netunicorn/library/tasks/network_attacks/arp/spoof.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 05:08:52.926392 netunicorn-library-0.3.1/src/netunicorn/library/tasks/network_attacks/cve202141773/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-09 05:08:39.000000 netunicorn-library-0.3.1/src/netunicorn/library/tasks/network_attacks/cve202141773/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 05:08:52.926392 netunicorn-library-0.3.1/src/netunicorn/library/tasks/network_attacks/heartbleed/
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-06-09 05:08:39.000000 netunicorn-library-0.3.1/src/netunicorn/library/tasks/network_attacks/heartbleed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-06-09 05:08:39.000000 netunicorn-library-0.3.1/src/netunicorn/library/tasks/network_attacks/heartbleed/heartbleeder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 05:08:52.926392 netunicorn-library-0.3.1/src/netunicorn/library/tasks/network_attacks/icmp/
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-09 05:08:39.000000 netunicorn-library-0.3.1/src/netunicorn/library/tasks/network_attacks/icmp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-09 05:08:39.000000 netunicorn-library-0.3.1/src/netunicorn/library/tasks/network_attacks/icmp/redirection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 05:08:52.926392 netunicorn-library-0.3.1/src/netunicorn/library/tasks/network_attacks/land/
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-09 05:08:39.000000 netunicorn-library-0.3.1/src/netunicorn/library/tasks/network_attacks/land/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-06-09 05:08:39.000000 netunicorn-library-0.3.1/src/netunicorn/library/tasks/network_attacks/land/landattack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 05:08:52.926392 netunicorn-library-0.3.1/src/netunicorn/library/tasks/network_attacks/log4j/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-09 05:08:39.000000 netunicorn-library-0.3.1/src/netunicorn/library/tasks/network_attacks/log4j/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 05:08:52.930392 netunicorn-library-0.3.1/src/netunicorn/library/tasks/network_attacks/loris/
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-06-09 05:08:39.000000 netunicorn-library-0.3.1/src/netunicorn/library/tasks/network_attacks/loris/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-06-09 05:08:39.000000 netunicorn-library-0.3.1/src/netunicorn/library/tasks/network_attacks/loris/slowloris.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-09 05:08:39.000000 netunicorn-library-0.3.1/src/netunicorn/library/tasks/network_attacks/loris/smbloris.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 05:08:52.930392 netunicorn-library-0.3.1/src/netunicorn/library/tasks/network_attacks/mac/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-09 05:08:39.000000 netunicorn-library-0.3.1/src/netunicorn/library/tasks/network_attacks/mac/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-09 05:08:39.000000 netunicorn-library-0.3.1/src/netunicorn/library/tasks/network_attacks/mac/flooder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 05:08:52.930392 netunicorn-library-0.3.1/src/netunicorn/library/tasks/network_attacks/mail/
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-09 05:08:39.000000 netunicorn-library-0.3.1/src/netunicorn/library/tasks/network_attacks/mail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-09 05:08:39.000000 netunicorn-library-0.3.1/src/netunicorn/library/tasks/network_attacks/mail/fake_mail.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 05:08:52.930392 netunicorn-library-0.3.1/src/netunicorn/library/tasks/qoe_youtube/
+-rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-06-09 05:08:39.000000 netunicorn-library-0.3.1/src/netunicorn/library/tasks/qoe_youtube/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-06-09 05:08:39.000000 netunicorn-library-0.3.1/src/netunicorn/library/tasks/qoe_youtube/qoe_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6461 2023-06-09 05:08:39.000000 netunicorn-library-0.3.1/src/netunicorn/library/tasks/qoe_youtube/watcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 05:08:52.930392 netunicorn-library-0.3.1/src/netunicorn/library/tasks/upload/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 05:08:39.000000 netunicorn-library-0.3.1/src/netunicorn/library/tasks/upload/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-06-09 05:08:39.000000 netunicorn-library-0.3.1/src/netunicorn/library/tasks/upload/webdav.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 05:08:52.930392 netunicorn-library-0.3.1/src/netunicorn/library/tasks/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 05:08:39.000000 netunicorn-library-0.3.1/src/netunicorn/library/tasks/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-09 05:08:39.000000 netunicorn-library-0.3.1/src/netunicorn/library/tasks/utils/sleep.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 05:08:52.930392 netunicorn-library-0.3.1/src/netunicorn/library/tasks/video_watchers/
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-09 05:08:39.000000 netunicorn-library-0.3.1/src/netunicorn/library/tasks/video_watchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-06-09 05:08:39.000000 netunicorn-library-0.3.1/src/netunicorn/library/tasks/video_watchers/twitch_watcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-06-09 05:08:39.000000 netunicorn-library-0.3.1/src/netunicorn/library/tasks/video_watchers/vimeo_watcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4652 2023-06-09 05:08:39.000000 netunicorn-library-0.3.1/src/netunicorn/library/tasks/video_watchers/youtube_watcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 05:08:52.934393 netunicorn-library-0.3.1/src/netunicorn_library.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-09 05:08:52.000000 netunicorn-library-0.3.1/src/netunicorn_library.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-06-09 05:08:52.000000 netunicorn-library-0.3.1/src/netunicorn_library.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 05:08:52.000000 netunicorn-library-0.3.1/src/netunicorn_library.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-09 05:08:52.000000 netunicorn-library-0.3.1/src/netunicorn_library.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-09 05:08:52.000000 netunicorn-library-0.3.1/src/netunicorn_library.egg-info/top_level.txt
```

### Comparing `netunicorn-library-0.3.0/pyproject.toml` & `netunicorn-library-0.3.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "netunicorn-library"
-version = "0.3.0"
+version = "0.3.1"
 authors = [
     {name = "Roman Beltiukov", email = "rbeltiukov@ucsb.edu"},
 ]
 description = "netunicorn contrib library"
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = ["netunicorn"]
```

### Comparing `netunicorn-library-0.3.0/src/netunicorn/library/tasks/basic.py` & `netunicorn-library-0.3.1/src/netunicorn/library/tasks/basic.py`

 * *Files identical despite different names*

### Comparing `netunicorn-library-0.3.0/src/netunicorn/library/tasks/capture/tcpdump.py` & `netunicorn-library-0.3.1/src/netunicorn/library/tasks/capture/tcpdump.py`

 * *Files identical despite different names*

### Comparing `netunicorn-library-0.3.0/src/netunicorn/library/tasks/flags.py` & `netunicorn-library-0.3.1/src/netunicorn/library/tasks/flags.py`

 * *Files identical despite different names*

### Comparing `netunicorn-library-0.3.0/src/netunicorn/library/tasks/letsencrypt/__init__.py` & `netunicorn-library-0.3.1/src/netunicorn/library/tasks/letsencrypt/__init__.py`

 * *Files identical despite different names*

### Comparing `netunicorn-library-0.3.0/src/netunicorn/library/tasks/letsencrypt/tasks.py` & `netunicorn-library-0.3.1/src/netunicorn/library/tasks/letsencrypt/tasks.py`

 * *Files identical despite different names*

### Comparing `netunicorn-library-0.3.0/src/netunicorn/library/tasks/measurements/ookla_speedtest.py` & `netunicorn-library-0.3.1/src/netunicorn/library/tasks/measurements/ookla_speedtest.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import subprocess
 from typing import Dict
 
+from netunicorn.base.architecture import Architecture
 from netunicorn.base.nodes import Node
 from netunicorn.base.task import Failure, Task, TaskDispatcher
 
 
 class SpeedTest(TaskDispatcher):
     def dispatch(self, node: Node) -> Task:
-        if node.properties.get("os_family", "").lower() == "linux":
+        if node.architecture in {Architecture.LINUX_AMD64, Architecture.LINUX_ARM64}:
             return SpeedTestLinuxImplementation()
 
         raise NotImplementedError(
-            f'SpeedTest is not implemented for {node.properties.get("os_family", "")}'
+            f'SpeedTest is not implemented for architecture: {node.architecture}'
         )
 
 
 class SpeedTestLinuxImplementation(Task):
     requirements = ["pip install speedtest-cli"]
 
     def run(self):
```

### Comparing `netunicorn-library-0.3.0/src/netunicorn/library/tasks/measurements/ping.py` & `netunicorn-library-0.3.1/src/netunicorn/library/tasks/measurements/ping.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import subprocess
 from dataclasses import dataclass
 from typing import List
 
+from netunicorn.base.architecture import Architecture
 from netunicorn.base.nodes import Node
 from netunicorn.base.task import Failure, Task, TaskDispatcher
 
 
 @dataclass
 class PacketResult:
     icmp_seq: int
@@ -31,18 +32,18 @@
 class Ping(TaskDispatcher):
     def __init__(self, address: str, count: int = 1, *args, **kwargs):
         self.address = address
         self.count = count
         super().__init__(*args, **kwargs)
 
     def dispatch(self, node: Node) -> Task:
-        if node.properties.get("os_family", "").lower() == "linux":
+        if node.architecture in {Architecture.LINUX_AMD64, Architecture.LINUX_ARM64}:
             return PingLinuxImplementation(self.address, self.count)
         raise NotImplementedError(
-            f'Ping is not implemented for {node.properties.get("os_family", "")}'
+            f'Ping is not implemented for architecture: {node.architecture}'
         )
 
 
 class PingLinuxImplementation(Task):
     requirements = ["sudo apt-get install -y inetutils-ping"]
 
     def __init__(self, address: str, count: int = 1, *args, **kwargs):
```

### Comparing `netunicorn-library-0.3.0/src/netunicorn/library/tasks/network_attacks/arp/__init__.py` & `netunicorn-library-0.3.1/src/netunicorn/library/tasks/network_attacks/arp/__init__.py`

 * *Files identical despite different names*

### Comparing `netunicorn-library-0.3.0/src/netunicorn/library/tasks/network_attacks/cve202141773/__init__.py` & `netunicorn-library-0.3.1/src/netunicorn/library/tasks/network_attacks/cve202141773/__init__.py`

 * *Files identical despite different names*

### Comparing `netunicorn-library-0.3.0/src/netunicorn/library/tasks/network_attacks/heartbleed/__init__.py` & `netunicorn-library-0.3.1/src/netunicorn/library/tasks/network_attacks/heartbleed/__init__.py`

 * *Files identical despite different names*

### Comparing `netunicorn-library-0.3.0/src/netunicorn/library/tasks/network_attacks/heartbleed/heartbleeder.py` & `netunicorn-library-0.3.1/src/netunicorn/library/tasks/network_attacks/heartbleed/heartbleeder.py`

 * *Files identical despite different names*

### Comparing `netunicorn-library-0.3.0/src/netunicorn/library/tasks/network_attacks/land/__init__.py` & `netunicorn-library-0.3.1/src/netunicorn/library/tasks/network_attacks/land/__init__.py`

 * *Files identical despite different names*

### Comparing `netunicorn-library-0.3.0/src/netunicorn/library/tasks/network_attacks/log4j/__init__.py` & `netunicorn-library-0.3.1/src/netunicorn/library/tasks/network_attacks/log4j/__init__.py`

 * *Files identical despite different names*

### Comparing `netunicorn-library-0.3.0/src/netunicorn/library/tasks/network_attacks/loris/__init__.py` & `netunicorn-library-0.3.1/src/netunicorn/library/tasks/network_attacks/loris/__init__.py`

 * *Files identical despite different names*

### Comparing `netunicorn-library-0.3.0/src/netunicorn/library/tasks/network_attacks/loris/slowloris.py` & `netunicorn-library-0.3.1/src/netunicorn/library/tasks/network_attacks/loris/slowloris.py`

 * *Files identical despite different names*

### Comparing `netunicorn-library-0.3.0/src/netunicorn/library/tasks/network_attacks/loris/smbloris.py` & `netunicorn-library-0.3.1/src/netunicorn/library/tasks/network_attacks/loris/smbloris.py`

 * *Files identical despite different names*

### Comparing `netunicorn-library-0.3.0/src/netunicorn/library/tasks/network_attacks/mail/__init__.py` & `netunicorn-library-0.3.1/src/netunicorn/library/tasks/network_attacks/mail/__init__.py`

 * *Files identical despite different names*

### Comparing `netunicorn-library-0.3.0/src/netunicorn/library/tasks/network_attacks/mail/fake_mail.py` & `netunicorn-library-0.3.1/src/netunicorn/library/tasks/network_attacks/mail/fake_mail.py`

 * *Files identical despite different names*

### Comparing `netunicorn-library-0.3.0/src/netunicorn/library/tasks/qoe_youtube/__init__.py` & `netunicorn-library-0.3.1/src/netunicorn/library/tasks/qoe_youtube/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -77,15 +77,15 @@
 
 class StopQoECollectionServer(TaskDispatcher):
     def __init__(self, start_task_name: str, *args, **kwargs):
         self.start_task_name = start_task_name
         super().__init__(*args, **kwargs)
 
     def dispatch(self, node: Node) -> Task:
-        if node.properties.get("os_family", "").lower() == "linux":
+        if node.architecture in {Architecture.LINUX_AMD64, Architecture.LINUX_ARM64}:
             return StopQoECollectionServerLinuxImplementation(start_task_name=self.start_task_name, name=self.name)
 
         raise NotImplementedError(
             f'StopQoECollectionServer is not implemented for {node.architecture}'
         )
 
 
@@ -133,15 +133,15 @@
                 self.qoe_server_address,
                 self.qoe_server_port,
                 self.report_time,
                 name=self.name,
             )
 
         raise NotImplementedError(
-            f'WatchYouTubeVideo is not implemented for {node.properties.get("os_family", "")}'
+            f'WatchYouTubeVideo is not implemented for architecture: {node.architecture}'
         )
 
 
 class WatchYouTubeVideoLinuxImplementation(Task):
     requirements = [
         "sudo apt update",
         "sudo apt install -y python3-pip wget xvfb unzip",
```

### Comparing `netunicorn-library-0.3.0/src/netunicorn/library/tasks/qoe_youtube/qoe_collector.py` & `netunicorn-library-0.3.1/src/netunicorn/library/tasks/qoe_youtube/qoe_collector.py`

 * *Files identical despite different names*

### Comparing `netunicorn-library-0.3.0/src/netunicorn/library/tasks/qoe_youtube/watcher.py` & `netunicorn-library-0.3.1/src/netunicorn/library/tasks/qoe_youtube/watcher.py`

 * *Files identical despite different names*

### Comparing `netunicorn-library-0.3.0/src/netunicorn/library/tasks/upload/webdav.py` & `netunicorn-library-0.3.1/src/netunicorn/library/tasks/upload/webdav.py`

 * *Files identical despite different names*

### Comparing `netunicorn-library-0.3.0/src/netunicorn/library/tasks/utils/sleep.py` & `netunicorn-library-0.3.1/src/netunicorn/library/tasks/utils/sleep.py`

 * *Files identical despite different names*

### Comparing `netunicorn-library-0.3.0/src/netunicorn/library/tasks/video_watchers/twitch_watcher.py` & `netunicorn-library-0.3.1/src/netunicorn/library/tasks/video_watchers/twitch_watcher.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import os
 import random
 import subprocess
 import time
 from typing import Optional
 
 from netunicorn.base import Result, Success, Task, TaskDispatcher
+from netunicorn.base.architecture import Architecture
 from netunicorn.base.nodes import Node
 
 from selenium import webdriver
 from selenium.webdriver.chrome.options import Options
 from selenium.webdriver.chrome.service import Service
 
 
@@ -44,19 +45,19 @@
 class WatchTwitchStream(TaskDispatcher):
     def __init__(self, video_url: str, duration: Optional[int] = None, *args, **kwargs):
         self.video_url = video_url
         self.duration = duration
         super().__init__(*args, **kwargs)
 
     def dispatch(self, node: Node) -> Task:
-        if node.properties.get("os_family", "").lower() == "linux":
+        if node.architecture in {Architecture.LINUX_AMD64, Architecture.LINUX_ARM64}:
             return WatchTwitchStreamLinuxImplementation(self.video_url, self.duration, name=self.name)
 
         raise NotImplementedError(
-            f'WatchYouTubeVideo is not implemented for {node.properties.get("os_family", "")}'
+            f'WatchTwitchVideo is not implemented for architecture: {node.architecture}'
         )
 
 
 class WatchTwitchStreamLinuxImplementation(Task):
     requirements = [
         "sudo apt update",
         "sudo apt install -y python3-pip wget xvfb",
```

### Comparing `netunicorn-library-0.3.0/src/netunicorn/library/tasks/video_watchers/vimeo_watcher.py` & `netunicorn-library-0.3.1/src/netunicorn/library/tasks/video_watchers/vimeo_watcher.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import os
 import random
 import subprocess
 import time
 from typing import Optional
 
 from netunicorn.base import Result, Failure, Success, Task, TaskDispatcher
+from netunicorn.base.architecture import Architecture
 from netunicorn.base.nodes import Node
 
 from selenium import webdriver
 from selenium.webdriver.chrome.options import Options
 from selenium.webdriver.chrome.service import Service
 
 
@@ -74,19 +75,19 @@
 class WatchVimeoVideo(TaskDispatcher):
     def __init__(self, video_url: str, duration: Optional[int] = None, *args, **kwargs):
         self.video_url = video_url
         self.duration = duration
         super().__init__(*args, **kwargs)
 
     def dispatch(self, node: Node) -> Task:
-        if node.properties.get("os_family", "").lower() == "linux":
+        if node.architecture in {Architecture.LINUX_AMD64, Architecture.LINUX_ARM64}:
             return WatchVimeoVideoLinuxImplementation(self.video_url, self.duration, name=self.name)
 
         raise NotImplementedError(
-            f'WatchYouTubeVideo is not implemented for {node.properties.get("os_family", "")}'
+            f'WatchVimeoVideo is not implemented for architecture: {node.architecture}'
         )
 
 
 class WatchVimeoVideoLinuxImplementation(Task):
     requirements = [
         "sudo apt update",
         "sudo apt install -y python3-pip wget xvfb",
```

### Comparing `netunicorn-library-0.3.0/src/netunicorn/library/tasks/video_watchers/youtube_watcher.py` & `netunicorn-library-0.3.1/src/netunicorn/library/tasks/video_watchers/youtube_watcher.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import random
 import subprocess
 import time
 from typing import Optional
 from enum import IntEnum
 
 from netunicorn.base import Result, Failure, Success, Task, TaskDispatcher
+from netunicorn.base.architecture import Architecture
 from netunicorn.base.nodes import Node
 
 from selenium import webdriver
 from selenium.webdriver.chrome.options import Options
 from selenium.webdriver.chrome.service import Service
 from selenium.webdriver.common.by import By
 from selenium.webdriver.common.keys import Keys
@@ -97,19 +98,19 @@
 class WatchYouTubeVideo(TaskDispatcher):
     def __init__(self, video_url: str, duration: Optional[int] = None, *args, **kwargs):
         self.video_url = video_url
         self.duration = duration
         super().__init__(*args, **kwargs)
 
     def dispatch(self, node: Node) -> Task:
-        if node.properties.get("os_family", "").lower() == "linux":
+        if node.architecture in {Architecture.LINUX_AMD64, Architecture.LINUX_ARM64}:
             return WatchYouTubeVideoLinuxImplementation(self.video_url, self.duration, name=self.name)
 
         raise NotImplementedError(
-            f'WatchYouTubeVideo is not implemented for {node.properties.get("os_family", "")}'
+            f'WatchYouTubeVideo is not implemented for architecture: {node.architecture}'
         )
 
 
 class WatchYouTubeVideoLinuxImplementation(Task):
     requirements = [
         "sudo apt update",
         "sudo apt install -y python3-pip wget xvfb",
```

### Comparing `netunicorn-library-0.3.0/src/netunicorn_library.egg-info/SOURCES.txt` & `netunicorn-library-0.3.1/src/netunicorn_library.egg-info/SOURCES.txt`

 * *Files identical despite different names*

