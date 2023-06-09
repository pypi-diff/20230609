# Comparing `tmp/rattail-fabric2-0.2.4.tar.gz` & `tmp/rattail-fabric2-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/rattail-fabric2-0.2.4.tar", last modified: Fri Sep 25 23:05:54 2020, max compression
+gzip compressed data, was "rattail-fabric2-0.3.0.tar", last modified: Fri Jun  9 02:11:04 2023, max compression
```

## Comparing `rattail-fabric2-0.2.4.tar` & `rattail-fabric2-0.3.0.tar`

### file list

```diff
@@ -1,68 +1,86 @@
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2020-09-25 23:05:54.000000 rattail-fabric2-0.2.4/
--rw-r--r--   0 lance     (1000) lance     (1000)       38 2020-09-25 23:05:54.000000 rattail-fabric2-0.2.4/setup.cfg
--rw-r--r--   0 lance     (1000) lance     (1000)     1218 2020-09-25 23:05:54.000000 rattail-fabric2-0.2.4/PKG-INFO
--rw-r--r--   0 lance     (1000) lance     (1000)      765 2020-09-25 23:05:09.000000 rattail-fabric2-0.2.4/CHANGES.rst
--rw-r--r--   0 lance     (1000) lance     (1000)      341 2020-09-08 21:10:55.000000 rattail-fabric2-0.2.4/README.rst
--rw-r--r--   0 lance     (1000) lance     (1000)      105 2020-09-08 21:13:35.000000 rattail-fabric2-0.2.4/MANIFEST.in
--rw-r--r--   0 lance     (1000) lance     (1000)     3705 2020-09-19 07:51:42.000000 rattail-fabric2-0.2.4/setup.py
--rw-r--r--   0 lance     (1000) lance     (1000)    35147 2020-09-08 21:10:55.000000 rattail-fabric2-0.2.4/COPYING.txt
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2020-09-25 23:05:54.000000 rattail-fabric2-0.2.4/rattail_fabric2.egg-info/
--rw-r--r--   0 lance     (1000) lance     (1000)     1218 2020-09-25 23:05:54.000000 rattail-fabric2-0.2.4/rattail_fabric2.egg-info/PKG-INFO
--rw-r--r--   0 lance     (1000) lance     (1000)        1 2020-09-25 23:05:54.000000 rattail-fabric2-0.2.4/rattail_fabric2.egg-info/not-zip-safe
--rw-r--r--   0 lance     (1000) lance     (1000)       16 2020-09-25 23:05:54.000000 rattail-fabric2-0.2.4/rattail_fabric2.egg-info/top_level.txt
--rw-r--r--   0 lance     (1000) lance     (1000)        1 2020-09-25 23:05:54.000000 rattail-fabric2-0.2.4/rattail_fabric2.egg-info/dependency_links.txt
--rw-r--r--   0 lance     (1000) lance     (1000)       27 2020-09-25 23:05:54.000000 rattail-fabric2-0.2.4/rattail_fabric2.egg-info/requires.txt
--rw-r--r--   0 lance     (1000) lance     (1000)     1924 2020-09-25 23:05:54.000000 rattail-fabric2-0.2.4/rattail_fabric2.egg-info/SOURCES.txt
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2020-09-25 23:05:54.000000 rattail-fabric2-0.2.4/rattail_fabric2/
--rw-r--r--   0 lance     (1000) lance     (1000)    12185 2020-09-24 03:40:51.000000 rattail-fabric2-0.2.4/rattail_fabric2/core.py
--rw-r--r--   0 lance     (1000) lance     (1000)     3364 2020-09-08 21:10:55.000000 rattail-fabric2-0.2.4/rattail_fabric2/rattail.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1680 2020-09-23 18:56:35.000000 rattail-fabric2-0.2.4/rattail_fabric2/mssql.py
--rw-r--r--   0 lance     (1000) lance     (1000)     4673 2020-09-08 21:10:55.000000 rattail-fabric2-0.2.4/rattail_fabric2/apache.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2100 2020-09-08 21:10:55.000000 rattail-fabric2-0.2.4/rattail_fabric2/freetds.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1693 2020-09-08 21:10:55.000000 rattail-fabric2-0.2.4/rattail_fabric2/pod.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1321 2020-09-23 04:11:05.000000 rattail-fabric2-0.2.4/rattail_fabric2/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1500 2020-09-08 21:10:55.000000 rattail-fabric2-0.2.4/rattail_fabric2/composer.py
--rw-r--r--   0 lance     (1000) lance     (1000)     9439 2020-09-08 21:10:55.000000 rattail-fabric2-0.2.4/rattail_fabric2/backup.py
--rw-r--r--   0 lance     (1000) lance     (1000)     5975 2020-09-08 21:10:55.000000 rattail-fabric2-0.2.4/rattail_fabric2/mysql.py
--rw-r--r--   0 lance     (1000) lance     (1000)    11150 2020-09-08 21:10:55.000000 rattail-fabric2-0.2.4/rattail_fabric2/util.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2531 2020-09-08 21:10:55.000000 rattail-fabric2-0.2.4/rattail_fabric2/ssh.py
--rw-r--r--   0 lance     (1000) lance     (1000)     3264 2020-09-18 19:10:58.000000 rattail-fabric2-0.2.4/rattail_fabric2/apt.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2020-09-25 23:05:54.000000 rattail-fabric2-0.2.4/rattail_fabric2/deploy/
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2020-09-25 23:05:54.000000 rattail-fabric2-0.2.4/rattail_fabric2/deploy/composer/
--rwxr-xr-x   0 lance     (1000) lance     (1000)      463 2020-09-08 21:10:55.000000 rattail-fabric2-0.2.4/rattail_fabric2/deploy/composer/install-composer.sh
--rw-r--r--   0 lance     (1000) lance     (1000)     4070 2020-09-08 21:10:55.000000 rattail-fabric2-0.2.4/rattail_fabric2/deploy/bouncer
--rw-r--r--   0 lance     (1000) lance     (1000)     3849 2020-09-08 21:10:55.000000 rattail-fabric2-0.2.4/rattail_fabric2/deploy/soffice
--rwxr-xr-x   0 lance     (1000) lance     (1000)     1598 2020-09-08 21:10:55.000000 rattail-fabric2-0.2.4/rattail_fabric2/deploy/check-systemd-service
--rw-r--r--   0 lance     (1000) lance     (1000)     4538 2020-09-08 21:10:55.000000 rattail-fabric2-0.2.4/rattail_fabric2/deploy/daemon
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2020-09-25 23:05:54.000000 rattail-fabric2-0.2.4/rattail_fabric2/deploy/backup/
--rw-r--r--   0 lance     (1000) lance     (1000)       16 2020-09-08 21:10:55.000000 rattail-fabric2-0.2.4/rattail_fabric2/deploy/backup/git-exclude
--rwxr-xr-x   0 lance     (1000) lance     (1000)      467 2020-09-08 21:10:55.000000 rattail-fabric2-0.2.4/rattail_fabric2/deploy/backup/rattail-backup.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      318 2020-09-08 21:10:55.000000 rattail-fabric2-0.2.4/rattail_fabric2/deploy/backup/supervisor.conf.mako
--rwxr-xr-x   0 lance     (1000) lance     (1000)      557 2020-09-08 21:10:55.000000 rattail-fabric2-0.2.4/rattail_fabric2/deploy/backup/upgrade.sh.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     1029 2020-09-08 21:10:55.000000 rattail-fabric2-0.2.4/rattail_fabric2/deploy/backup/luigi.cfg.mako
--rwxr-xr-x   0 lance     (1000) lance     (1000)      599 2020-09-08 21:10:55.000000 rattail-fabric2-0.2.4/rattail_fabric2/deploy/backup/overnight-backups.sh.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      172 2020-09-08 21:10:55.000000 rattail-fabric2-0.2.4/rattail_fabric2/deploy/backup/crontab.mako
--rwxr-xr-x   0 lance     (1000) lance     (1000)      234 2020-09-08 21:10:55.000000 rattail-fabric2-0.2.4/rattail_fabric2/deploy/backup/restart-overnight-backups.sh.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     2030 2020-09-08 21:10:55.000000 rattail-fabric2-0.2.4/rattail_fabric2/deploy/backup/luigi-overnight.py
--rw-r--r--   0 lance     (1000) lance     (1000)      790 2020-09-08 21:10:55.000000 rattail-fabric2-0.2.4/rattail_fabric2/deploy/backup/luigi-logging.conf.mako
--rwxr-xr-x   0 lance     (1000) lance     (1000)      637 2020-09-08 21:10:55.000000 rattail-fabric2-0.2.4/rattail_fabric2/deploy/backup/backup-everything.mako
--rwxr-xr-x   0 lance     (1000) lance     (1000)     1848 2020-09-08 21:10:55.000000 rattail-fabric2-0.2.4/rattail_fabric2/deploy/check-supervisor-process
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2020-09-25 23:05:54.000000 rattail-fabric2-0.2.4/rattail_fabric2/deploy/apt/
--rw-r--r--   0 lance     (1000) lance     (1000)       98 2020-09-08 21:10:55.000000 rattail-fabric2-0.2.4/rattail_fabric2/deploy/apt/listchanges.conf
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2020-09-25 23:05:54.000000 rattail-fabric2-0.2.4/rattail_fabric2/deploy/rattail/
--rw-r--r--   0 lance     (1000) lance     (1000)     1840 2020-09-08 21:10:55.000000 rattail-fabric2-0.2.4/rattail_fabric2/deploy/rattail/rattail.conf.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     3943 2020-09-08 21:10:55.000000 rattail-fabric2-0.2.4/rattail_fabric2/deploy/luigid
--rwxr-xr-x   0 lance     (1000) lance     (1000)     1945 2020-09-08 21:10:55.000000 rattail-fabric2-0.2.4/rattail_fabric2/deploy/check-rattail-daemon
--rw-r--r--   0 lance     (1000) lance     (1000)     4069 2020-09-08 21:10:55.000000 rattail-fabric2-0.2.4/rattail_fabric2/deploy/filemon
--rw-r--r--   0 lance     (1000) lance     (1000)     4081 2020-09-08 21:10:55.000000 rattail-fabric2-0.2.4/rattail_fabric2/deploy/datasync
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2020-09-25 23:05:54.000000 rattail-fabric2-0.2.4/rattail_fabric2/deploy/python/
--rwxr-xr-x   0 lance     (1000) lance     (1000)      327 2020-09-08 21:10:55.000000 rattail-fabric2-0.2.4/rattail_fabric2/deploy/python/premkvirtualenv
--rw-r--r--   0 lance     (1000) lance     (1000)    10117 2020-09-20 22:43:30.000000 rattail-fabric2-0.2.4/rattail_fabric2/python.py
--rw-r--r--   0 lance     (1000) lance     (1000)     6053 2020-09-08 21:10:55.000000 rattail-fabric2-0.2.4/rattail_fabric2/postgresql.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1996 2020-09-08 21:10:55.000000 rattail-fabric2-0.2.4/rattail_fabric2/nodejs.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1271 2020-09-08 21:10:55.000000 rattail-fabric2-0.2.4/rattail_fabric2/soffice.py
--rw-r--r--   0 lance     (1000) lance     (1000)       48 2020-09-25 23:05:31.000000 rattail-fabric2-0.2.4/rattail_fabric2/_version.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2725 2020-09-08 21:10:55.000000 rattail-fabric2-0.2.4/rattail_fabric2/corepos.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2758 2020-09-08 21:10:55.000000 rattail-fabric2-0.2.4/rattail_fabric2/postfix.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1304 2020-09-08 21:10:55.000000 rattail-fabric2-0.2.4/rattail_fabric2/borg.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2898 2020-09-08 21:10:55.000000 rattail-fabric2-0.2.4/rattail_fabric2/certbot.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-06-09 02:11:04.826073 rattail-fabric2-0.3.0/
+-rw-r--r--   0 lance     (1000) lance     (1000)      859 2023-06-09 02:09:51.000000 rattail-fabric2-0.3.0/CHANGES.rst
+-rw-r--r--   0 lance     (1000) lance     (1000)    35147 2020-09-08 21:10:55.000000 rattail-fabric2-0.3.0/COPYING.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)      105 2020-09-08 21:13:35.000000 rattail-fabric2-0.3.0/MANIFEST.in
+-rw-r--r--   0 lance     (1000) lance     (1000)     1101 2023-06-09 02:11:04.826073 rattail-fabric2-0.3.0/PKG-INFO
+-rw-r--r--   0 lance     (1000) lance     (1000)      341 2020-09-08 21:10:55.000000 rattail-fabric2-0.3.0/README.rst
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-06-09 02:11:04.818073 rattail-fabric2-0.3.0/rattail_fabric2/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1389 2023-05-17 12:21:22.000000 rattail-fabric2-0.3.0/rattail_fabric2/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)       48 2023-06-09 02:09:59.000000 rattail-fabric2-0.3.0/rattail_fabric2/_version.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     4672 2020-10-17 15:21:16.000000 rattail-fabric2-0.3.0/rattail_fabric2/apache.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     3622 2020-09-29 01:17:27.000000 rattail-fabric2-0.3.0/rattail_fabric2/apt.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    10658 2023-02-23 19:05:47.000000 rattail-fabric2-0.3.0/rattail_fabric2/backup.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1304 2020-09-08 21:10:55.000000 rattail-fabric2-0.3.0/rattail_fabric2/borg.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1583 2023-01-05 13:40:50.000000 rattail-fabric2-0.3.0/rattail_fabric2/byjove.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2898 2020-12-15 18:31:03.000000 rattail-fabric2-0.3.0/rattail_fabric2/certbot.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2039 2023-02-19 17:19:37.000000 rattail-fabric2-0.3.0/rattail_fabric2/collectd.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1570 2022-08-27 03:27:45.000000 rattail-fabric2-0.3.0/rattail_fabric2/composer.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    13572 2023-05-31 22:50:09.000000 rattail-fabric2-0.3.0/rattail_fabric2/core.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     6240 2023-05-15 23:28:44.000000 rattail-fabric2-0.3.0/rattail_fabric2/corepos.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-06-09 02:11:04.822073 rattail-fabric2-0.3.0/rattail_fabric2/deploy/
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-06-09 02:11:04.822073 rattail-fabric2-0.3.0/rattail_fabric2/deploy/apt/
+-rw-r--r--   0 lance     (1000) lance     (1000)       98 2020-09-08 21:10:55.000000 rattail-fabric2-0.3.0/rattail_fabric2/deploy/apt/listchanges.conf
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-06-09 02:11:04.822073 rattail-fabric2-0.3.0/rattail_fabric2/deploy/backup/
+-rwxr-xr-x   0 lance     (1000) lance     (1000)      637 2020-09-08 21:10:55.000000 rattail-fabric2-0.3.0/rattail_fabric2/deploy/backup/backup-everything.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      213 2023-02-23 19:03:28.000000 rattail-fabric2-0.3.0/rattail_fabric2/deploy/backup/crontab.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)       16 2020-09-08 21:10:55.000000 rattail-fabric2-0.3.0/rattail_fabric2/deploy/backup/git-exclude
+-rw-r--r--   0 lance     (1000) lance     (1000)      157 2019-02-06 20:44:14.000000 rattail-fabric2-0.3.0/rattail_fabric2/deploy/backup/logrotate.conf
+-rw-r--r--   0 lance     (1000) lance     (1000)      790 2020-09-08 21:10:55.000000 rattail-fabric2-0.3.0/rattail_fabric2/deploy/backup/luigi-logging.conf.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     2030 2020-09-08 21:10:55.000000 rattail-fabric2-0.3.0/rattail_fabric2/deploy/backup/luigi-overnight.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1029 2020-09-08 21:10:55.000000 rattail-fabric2-0.3.0/rattail_fabric2/deploy/backup/luigi.cfg.mako
+-rwxr-xr-x   0 lance     (1000) lance     (1000)      599 2020-09-08 21:10:55.000000 rattail-fabric2-0.3.0/rattail_fabric2/deploy/backup/overnight-backups.sh.mako
+-rwxr-xr-x   0 lance     (1000) lance     (1000)      467 2020-09-08 21:10:55.000000 rattail-fabric2-0.3.0/rattail_fabric2/deploy/backup/rattail-backup.mako
+-rwxr-xr-x   0 lance     (1000) lance     (1000)      234 2020-09-08 21:10:55.000000 rattail-fabric2-0.3.0/rattail_fabric2/deploy/backup/restart-overnight-backups.sh.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      318 2020-09-08 21:10:55.000000 rattail-fabric2-0.3.0/rattail_fabric2/deploy/backup/supervisor.conf.mako
+-rwxr-xr-x   0 lance     (1000) lance     (1000)      656 2022-03-19 02:45:53.000000 rattail-fabric2-0.3.0/rattail_fabric2/deploy/backup/upgrade.sh.mako
+-rwxr-xr-x   0 lance     (1000) lance     (1000)     1945 2020-09-08 21:10:55.000000 rattail-fabric2-0.3.0/rattail_fabric2/deploy/check-rattail-daemon
+-rwxr-xr-x   0 lance     (1000) lance     (1000)     1848 2020-09-08 21:10:55.000000 rattail-fabric2-0.3.0/rattail_fabric2/deploy/check-supervisor-process
+-rwxr-xr-x   0 lance     (1000) lance     (1000)     1598 2020-09-08 21:10:55.000000 rattail-fabric2-0.3.0/rattail_fabric2/deploy/check-systemd-service
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-06-09 02:11:04.822073 rattail-fabric2-0.3.0/rattail_fabric2/deploy/collectd/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1544 2022-08-22 03:36:50.000000 rattail-fabric2-0.3.0/rattail_fabric2/deploy/collectd/check-mountpoints.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-06-09 02:11:04.822073 rattail-fabric2-0.3.0/rattail_fabric2/deploy/composer/
+-rwxr-xr-x   0 lance     (1000) lance     (1000)      463 2020-09-08 21:10:55.000000 rattail-fabric2-0.3.0/rattail_fabric2/deploy/composer/install-composer.sh
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-06-09 02:11:04.822073 rattail-fabric2-0.3.0/rattail_fabric2/deploy/corepos/
+-rw-r--r--   0 lance     (1000) lance     (1000)      386 2023-02-18 02:47:33.000000 rattail-fabric2-0.3.0/rattail_fabric2/deploy/corepos/fannie-config.php.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-06-09 02:11:04.826073 rattail-fabric2-0.3.0/rattail_fabric2/deploy/luigi/
+-rwxr-xr-x   0 lance     (1000) lance     (1000)      364 2022-11-27 18:22:06.000000 rattail-fabric2-0.3.0/rattail_fabric2/deploy/luigi/cron-overnight.sh.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      191 2023-01-08 18:52:51.000000 rattail-fabric2-0.3.0/rattail_fabric2/deploy/luigi/crontab.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      791 2022-01-28 20:25:09.000000 rattail-fabric2-0.3.0/rattail_fabric2/deploy/luigi/logging.conf.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      414 2022-01-28 20:31:34.000000 rattail-fabric2-0.3.0/rattail_fabric2/deploy/luigi/luigi-logrotate.conf.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     1468 2023-01-09 14:58:43.000000 rattail-fabric2-0.3.0/rattail_fabric2/deploy/luigi/luigi.cfg.mako
+-rwxr-xr-x   0 lance     (1000) lance     (1000)      600 2022-01-28 21:02:15.000000 rattail-fabric2-0.3.0/rattail_fabric2/deploy/luigi/overnight.sh.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      364 2022-11-27 18:22:37.000000 rattail-fabric2-0.3.0/rattail_fabric2/deploy/luigi/restart-overnight.sh.mako
+-rwxr-xr-x   0 lance     (1000) lance     (1000)      359 2022-01-28 20:35:54.000000 rattail-fabric2-0.3.0/rattail_fabric2/deploy/luigi/rotate-logs.sh.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      335 2022-01-28 21:00:23.000000 rattail-fabric2-0.3.0/rattail_fabric2/deploy/luigi/supervisor.conf.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-06-09 02:11:04.826073 rattail-fabric2-0.3.0/rattail_fabric2/deploy/python/
+-rwxr-xr-x   0 lance     (1000) lance     (1000)      327 2020-09-08 21:10:55.000000 rattail-fabric2-0.3.0/rattail_fabric2/deploy/python/premkvirtualenv
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-06-09 02:11:04.826073 rattail-fabric2-0.3.0/rattail_fabric2/deploy/rattail/
+-rwxr-xr-x   0 lance     (1000) lance     (1000)      620 2021-11-11 17:40:00.000000 rattail-fabric2-0.3.0/rattail_fabric2/deploy/rattail/check-datasync-queue.mako
+-rwxr-xr-x   0 lance     (1000) lance     (1000)      664 2021-11-11 17:40:07.000000 rattail-fabric2-0.3.0/rattail_fabric2/deploy/rattail/check-datasync-watchers.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     2042 2023-06-02 19:34:23.000000 rattail-fabric2-0.3.0/rattail_fabric2/deploy/rattail/rattail.conf.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     3849 2020-09-08 21:10:55.000000 rattail-fabric2-0.3.0/rattail_fabric2/deploy/soffice
+-rw-r--r--   0 lance     (1000) lance     (1000)     2199 2023-01-05 17:41:25.000000 rattail-fabric2-0.3.0/rattail_fabric2/docker.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1292 2020-12-14 16:19:32.000000 rattail-fabric2-0.3.0/rattail_fabric2/ejabberd.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2099 2021-07-28 13:21:34.000000 rattail-fabric2-0.3.0/rattail_fabric2/freetds.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     6791 2023-03-09 21:28:38.000000 rattail-fabric2-0.3.0/rattail_fabric2/luigi.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1283 2022-02-11 03:26:16.000000 rattail-fabric2-0.3.0/rattail_fabric2/mariadb.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1680 2023-06-09 02:09:13.000000 rattail-fabric2-0.3.0/rattail_fabric2/mssql.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     6441 2021-02-02 17:31:25.000000 rattail-fabric2-0.3.0/rattail_fabric2/mysql.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1996 2020-09-08 21:10:55.000000 rattail-fabric2-0.3.0/rattail_fabric2/nodejs.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1702 2020-10-14 14:21:40.000000 rattail-fabric2-0.3.0/rattail_fabric2/pod.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     3022 2023-01-09 18:03:43.000000 rattail-fabric2-0.3.0/rattail_fabric2/postfix.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     8924 2023-06-09 02:09:13.000000 rattail-fabric2-0.3.0/rattail_fabric2/postgresql.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    11101 2023-01-09 03:18:56.000000 rattail-fabric2-0.3.0/rattail_fabric2/python.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     5088 2023-01-07 21:45:54.000000 rattail-fabric2-0.3.0/rattail_fabric2/rattail.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1271 2020-09-08 21:10:55.000000 rattail-fabric2-0.3.0/rattail_fabric2/soffice.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     3636 2020-10-09 21:38:14.000000 rattail-fabric2-0.3.0/rattail_fabric2/ssh.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    11266 2023-01-07 23:20:19.000000 rattail-fabric2-0.3.0/rattail_fabric2/util.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-06-09 02:11:04.818073 rattail-fabric2-0.3.0/rattail_fabric2.egg-info/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1101 2023-06-09 02:11:04.000000 rattail-fabric2-0.3.0/rattail_fabric2.egg-info/PKG-INFO
+-rw-r--r--   0 lance     (1000) lance     (1000)     2650 2023-06-09 02:11:04.000000 rattail-fabric2-0.3.0/rattail_fabric2.egg-info/SOURCES.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)        1 2023-06-09 02:11:04.000000 rattail-fabric2-0.3.0/rattail_fabric2.egg-info/dependency_links.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)        1 2023-06-09 02:11:04.000000 rattail-fabric2-0.3.0/rattail_fabric2.egg-info/not-zip-safe
+-rw-r--r--   0 lance     (1000) lance     (1000)       27 2023-06-09 02:11:04.000000 rattail-fabric2-0.3.0/rattail_fabric2.egg-info/requires.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)       16 2023-06-09 02:11:04.000000 rattail-fabric2-0.3.0/rattail_fabric2.egg-info/top_level.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)      859 2023-06-09 02:11:04.826073 rattail-fabric2-0.3.0/setup.cfg
+-rw-r--r--   0 lance     (1000) lance     (1000)      974 2023-05-16 18:47:04.000000 rattail-fabric2-0.3.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `rattail-fabric2-0.2.4/PKG-INFO` & `rattail-fabric2-0.3.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: rattail-fabric2
-Version: 0.2.4
+Version: 0.3.0
 Summary: Fabric (v2) Utilities for Rattail
 Home-page: https://rattailproject.org/
 Author: Lance Edgar
 Author-email: lance@edbob.org
 License: GNU GPL v3
-Description: 
-        rattail-fabric2
-        ===============
-        
-        Rattail is a retail software framework, released under the GNU General Public
-        License.
-        
-        This package contains various utility functions for use with `Fabric`_ (v2).
-        
-        .. _`Fabric`: http://www.fabfile.org/
-        
-        Please see Rattail's `home page`_ for more information.
-        
-        .. _`home page`: https://rattailproject.org/
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Topic :: System :: Systems Administration
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+License-File: COPYING.txt
+
+
+rattail-fabric2
+===============
+
+Rattail is a retail software framework, released under the GNU General Public
+License.
+
+This package contains various utility functions for use with `Fabric`_ (v2).
+
+.. _`Fabric`: http://www.fabfile.org/
+
+Please see Rattail's `home page`_ for more information.
+
+.. _`home page`: https://rattailproject.org/
```

### Comparing `rattail-fabric2-0.2.4/CHANGES.rst` & `rattail-fabric2-0.3.0/CHANGES.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 
 CHANGELOG
 =========
 
+0.3.0 (2023-06-08)
+------------------
+
+- OMG so many changes...just needed a fresh release.
+
+
 0.2.4 (2020-09-25)
 ------------------
 
 - Allow kwargs for template context when deploying sudoers file.
 - Pass arbitrary kwargs along, for ``apt.install()``.
 - Add ``method`` kwarg for ``python.install_pip()``.
 - Require the 'rattail' package.
```

### Comparing `rattail-fabric2-0.2.4/COPYING.txt` & `rattail-fabric2-0.3.0/COPYING.txt`

 * *Files identical despite different names*

### Comparing `rattail-fabric2-0.2.4/rattail_fabric2.egg-info/PKG-INFO` & `rattail-fabric2-0.3.0/rattail_fabric2.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: rattail-fabric2
-Version: 0.2.4
+Version: 0.3.0
 Summary: Fabric (v2) Utilities for Rattail
 Home-page: https://rattailproject.org/
 Author: Lance Edgar
 Author-email: lance@edbob.org
 License: GNU GPL v3
-Description: 
-        rattail-fabric2
-        ===============
-        
-        Rattail is a retail software framework, released under the GNU General Public
-        License.
-        
-        This package contains various utility functions for use with `Fabric`_ (v2).
-        
-        .. _`Fabric`: http://www.fabfile.org/
-        
-        Please see Rattail's `home page`_ for more information.
-        
-        .. _`home page`: https://rattailproject.org/
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Topic :: System :: Systems Administration
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+License-File: COPYING.txt
+
+
+rattail-fabric2
+===============
+
+Rattail is a retail software framework, released under the GNU General Public
+License.
+
+This package contains various utility functions for use with `Fabric`_ (v2).
+
+.. _`Fabric`: http://www.fabfile.org/
+
+Please see Rattail's `home page`_ for more information.
+
+.. _`home page`: https://rattailproject.org/
```

### Comparing `rattail-fabric2-0.2.4/rattail_fabric2.egg-info/SOURCES.txt` & `rattail-fabric2-0.3.0/rattail_fabric2.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,30 @@
 CHANGES.rst
 COPYING.txt
 MANIFEST.in
 README.rst
+setup.cfg
 setup.py
 rattail_fabric2/__init__.py
 rattail_fabric2/_version.py
 rattail_fabric2/apache.py
 rattail_fabric2/apt.py
 rattail_fabric2/backup.py
 rattail_fabric2/borg.py
+rattail_fabric2/byjove.py
 rattail_fabric2/certbot.py
+rattail_fabric2/collectd.py
 rattail_fabric2/composer.py
 rattail_fabric2/core.py
 rattail_fabric2/corepos.py
+rattail_fabric2/docker.py
+rattail_fabric2/ejabberd.py
 rattail_fabric2/freetds.py
+rattail_fabric2/luigi.py
+rattail_fabric2/mariadb.py
 rattail_fabric2/mssql.py
 rattail_fabric2/mysql.py
 rattail_fabric2/nodejs.py
 rattail_fabric2/pod.py
 rattail_fabric2/postfix.py
 rattail_fabric2/postgresql.py
 rattail_fabric2/python.py
@@ -27,31 +34,40 @@
 rattail_fabric2/util.py
 rattail_fabric2.egg-info/PKG-INFO
 rattail_fabric2.egg-info/SOURCES.txt
 rattail_fabric2.egg-info/dependency_links.txt
 rattail_fabric2.egg-info/not-zip-safe
 rattail_fabric2.egg-info/requires.txt
 rattail_fabric2.egg-info/top_level.txt
-rattail_fabric2/deploy/bouncer
 rattail_fabric2/deploy/check-rattail-daemon
 rattail_fabric2/deploy/check-supervisor-process
 rattail_fabric2/deploy/check-systemd-service
-rattail_fabric2/deploy/daemon
-rattail_fabric2/deploy/datasync
-rattail_fabric2/deploy/filemon
-rattail_fabric2/deploy/luigid
 rattail_fabric2/deploy/soffice
 rattail_fabric2/deploy/apt/listchanges.conf
 rattail_fabric2/deploy/backup/backup-everything.mako
 rattail_fabric2/deploy/backup/crontab.mako
 rattail_fabric2/deploy/backup/git-exclude
+rattail_fabric2/deploy/backup/logrotate.conf
 rattail_fabric2/deploy/backup/luigi-logging.conf.mako
 rattail_fabric2/deploy/backup/luigi-overnight.py
 rattail_fabric2/deploy/backup/luigi.cfg.mako
 rattail_fabric2/deploy/backup/overnight-backups.sh.mako
 rattail_fabric2/deploy/backup/rattail-backup.mako
 rattail_fabric2/deploy/backup/restart-overnight-backups.sh.mako
 rattail_fabric2/deploy/backup/supervisor.conf.mako
 rattail_fabric2/deploy/backup/upgrade.sh.mako
+rattail_fabric2/deploy/collectd/check-mountpoints.py
 rattail_fabric2/deploy/composer/install-composer.sh
+rattail_fabric2/deploy/corepos/fannie-config.php.mako
+rattail_fabric2/deploy/luigi/cron-overnight.sh.mako
+rattail_fabric2/deploy/luigi/crontab.mako
+rattail_fabric2/deploy/luigi/logging.conf.mako
+rattail_fabric2/deploy/luigi/luigi-logrotate.conf.mako
+rattail_fabric2/deploy/luigi/luigi.cfg.mako
+rattail_fabric2/deploy/luigi/overnight.sh.mako
+rattail_fabric2/deploy/luigi/restart-overnight.sh.mako
+rattail_fabric2/deploy/luigi/rotate-logs.sh.mako
+rattail_fabric2/deploy/luigi/supervisor.conf.mako
 rattail_fabric2/deploy/python/premkvirtualenv
+rattail_fabric2/deploy/rattail/check-datasync-queue.mako
+rattail_fabric2/deploy/rattail/check-datasync-watchers.mako
 rattail_fabric2/deploy/rattail/rattail.conf.mako
```

### Comparing `rattail-fabric2-0.2.4/rattail_fabric2/core.py` & `rattail-fabric2-0.3.0/rattail_fabric2/core.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8; -*-
 ################################################################################
 #
 #  Rattail -- Retail Software Framework
-#  Copyright © 2010-2019 Lance Edgar
+#  Copyright © 2010-2023 Lance Edgar
 #
 #  This file is part of Rattail.
 #
 #  Rattail is free software: you can redistribute it and/or modify it under the
 #  terms of the GNU General Public License as published by the Free Software
 #  Foundation, either version 3 of the License, or (at your option) any later
 #  version.
@@ -23,14 +23,15 @@
 """
 Core Utilities
 """
 
 import os
 import re
 import tempfile
+import warnings
 
 from mako.template import Template
 
 
 UNSPECIFIED = object()
 
 
@@ -123,25 +124,41 @@
         func = c.sudo if use_sudo else c.run
         func('chown {} {}'.format(owner, ' '.join(paths)))
     if mode is not None:
         func = c.sudo if use_sudo else c.run
         func('chmod {} {}'.format(mode, ' '.join(paths)))
 
 
-def make_system_user(c, name, home=None, uid=None, shell=None):
+def make_normal_user(c, name, full_name=None, disabled_login=True):
+    """
+    Make a new "normal" user account.
+    """
+    if not c.run('getent passwd {}'.format(name), warn=True).failed:
+        return
+
+    disabled_login = '--disabled-login' if disabled_login else ''
+    c.sudo("adduser --gecos '{}' {} {}".format(full_name or name,
+                                               disabled_login,
+                                               name))
+
+
+def make_system_user(c, name, home=None, uid=None, shell=None,
+                     disabled_password=None):
     """
     Make a new system user account, with the given home folder and shell path.
     """
     if not c.run('getent passwd {}'.format(name), warn=True).failed:
         return
 
     home = '--home {}'.format(home) if home else ''
     uid = '--uid {}'.format(uid) if uid else ''
     shell = '--shell {}'.format(shell) if shell else ''
-    c.sudo('adduser --system --group {} {} {} {}'.format(name, home, uid, shell))
+    disabled_password = '--disabled-password' if disabled_password else ''
+    c.sudo('adduser --system --group {} {} {} {} {}'.format(name, home, uid, shell,
+                                                            disabled_password))
 
 
 def set_timezone(c, timezone):
     """
     Set the system timezone to the given value, e.g. 'America/Chicago'.
     """
     c.sudo("bash -c 'echo {} > /etc/timezone'".format(timezone))
@@ -242,41 +259,46 @@
         kwargs['use_sudo'] = True
         deploy_conf(c, self, local_path, name, **kwargs)
 
     def backup_app(self, c, envname='backup', *args, **kwargs):
         from rattail_fabric2.backup import deploy_backup_app
         deploy_backup_app(c, self, envname, *args, **kwargs)
 
-    def certbot_account(self, c, uuid, localdir='certbot/account'):
+    def certbot_account(self, c, uuid, localdir='certbot/account',
+                        version='01'):
         """
         Deploy files to establish a certbot account on target server
         """
         from .util import exists
 
         localdir = localdir.rstrip('/')
         paths = [
             '/etc/letsencrypt/accounts',
-            '/etc/letsencrypt/accounts/acme-v01.api.letsencrypt.org',
-            '/etc/letsencrypt/accounts/acme-v01.api.letsencrypt.org/directory',
+            '/etc/letsencrypt/accounts/acme-v{}.api.letsencrypt.org'.format(version),
+            '/etc/letsencrypt/accounts/acme-v{}.api.letsencrypt.org/directory'.format(version),
         ]
         final_path = '{}/{}'.format(paths[-1], uuid)
         paths.append(final_path)
         if not exists(c, final_path, use_sudo=True):
             mkdir(c, paths, mode='0700', use_sudo=True)
             self.deploy(c, '{}/private_key.json'.format(localdir), '{}/private_key.json'.format(final_path), mode='0600', use_sudo=True)
             self.deploy(c, '{}/meta.json'.format(localdir), '{}/meta.json'.format(final_path), use_sudo=True)
             self.deploy(c, '{}/regr.json'.format(localdir), '{}/regr.json'.format(final_path), use_sudo=True)
 
     def soffice_daemon(self, c, local_path, name=None, register=True, start=True, **kwargs):
         """
         Deploy a "soffice" (headless LibreOffice) daemon.
         """
+        warnings.warn("deploy.soffice_daemon() is deprecated as it only supports "
+                      "/etc/init.d scripts.  please deploy your own systemd config "
+                      "instead, as needed.", DeprecationWarning)
         if name is None:
             name = local_path.split('/')[-1]
         kwargs.setdefault('use_sudo', True)
+        kwargs.setdefault('mode', '0755')
         self.deploy(c, local_path, '/etc/init.d/{}'.format(name), **kwargs)
         if register:
             c.sudo('update-rc.d {} defaults'.format(name))
             if start:
                 c.sudo('service {} restart'.format(name))
 
 
@@ -326,17 +348,25 @@
            `-- rattail/
                |-- init-filemon
                |-- rattail.conf.template
     """
     return Deployer(deploy_path, last_segment)
 
 
-def rsync(c, host, *paths):
+def rsync(c, host, *paths, files=False, target=None):
     """
     Runs rsync as root, for the given host and file paths.
+
+    :param files: If set, this indicates that each of the ``paths``
+       are actual files, as opposed to directories.
+
+    :param target: If set, this will be used instead of the given
+       path, for destination path.  This only works correctly if
+       ``paths`` contains only one path.
     """
     for path in paths:
         assert path.startswith('/')
         path = path.rstrip('/')
         # escape path for rsync
         path = path.replace(' ', r'\\\ ').replace("'", r"\\\'")
-        agent_sudo(c, 'rsync -aP --del root@{0}:{1}/ {1}'.format(host, path))
+        suffix = '' if files else '/'
+        agent_sudo(c, f'rsync -aP --del root@{host}:{path}{suffix} {target or path}')
```

### Comparing `rattail-fabric2-0.2.4/rattail_fabric2/mssql.py` & `rattail-fabric2-0.3.0/rattail_fabric2/mssql.py`

 * *Files identical despite different names*

### Comparing `rattail-fabric2-0.2.4/rattail_fabric2/apache.py` & `rattail-fabric2-0.3.0/rattail_fabric2/apache.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,15 @@
 
 def get_php_version(c):
     """
     Fetch the version of PHP running on the target system
     """
     result = c.sudo('php --version')
     if not result.failed:
-        match = re.match(r'^PHP (\d+\.\d+)\.\d+-', result.stdout)
+        match = re.match(r'^PHP (\d+\.\d+)\.\d+', result.stdout)
         if match:
             return float(match.group(1))
 
 
 def enable_mod(c, *names):
     """
     Enable the given Apache modules
```

### Comparing `rattail-fabric2-0.2.4/rattail_fabric2/freetds.py` & `rattail-fabric2-0.3.0/rattail_fabric2/freetds.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 
 def install_from_source(c, user='rattail', branch=None):
     """
     Install the FreeTDS library from source.
 
     Per instructions found here:
-    https://github.com/FreeTDS/freetds/blob/master/INSTALL.GIT
+    https://github.com/FreeTDS/freetds/blob/master/INSTALL.md
     """
     apt.install(
         c,
         'automake',
         'autoconf',
         'gettext',
         'gperf',
```

### Comparing `rattail-fabric2-0.2.4/rattail_fabric2/pod.py` & `rattail-fabric2-0.3.0/rattail_fabric2/pod.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,10 +34,10 @@
     Install the Product Open Data (POD) files to the given path.
     """
     apt.install(c, 'unzip')
     mkdir(c, path, use_sudo=True)
     if not exists(c, os.path.join(path, 'pod_pictures_gtin.zip')):
         if not download_url:
             download_url = 'http://www.product-open-data.com/docs/pod_pictures_gtin_2013.08.29_01.zip'
-        c.sudo("bash -c 'cd {}; wget --output-document=pod_pictures_gtin.zip {}'".format(path, url))
+        c.sudo("bash -c 'cd {}; wget --output-document=pod_pictures_gtin.zip {}'".format(path, download_url))
     if not exists(c, os.path.join(path, 'pictures/gtin')):
         c.sudo("bash -c 'cd {}; unzip pod_pictures_gtin.zip -d pictures'".format(path))
```

### Comparing `rattail-fabric2-0.2.4/rattail_fabric2/__init__.py` & `rattail-fabric2-0.3.0/rattail_fabric2/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8; -*-
 ################################################################################
 #
 #  Rattail -- Retail Software Framework
-#  Copyright © 2010-2020 Lance Edgar
+#  Copyright © 2010-2023 Lance Edgar
 #
 #  This file is part of Rattail.
 #
 #  Rattail is free software: you can redistribute it and/or modify it under the
 #  terms of the GNU General Public License as published by the Free Software
 #  Foundation, either version 3 of the License, or (at your option) any later
 #  version.
@@ -23,20 +23,23 @@
 """
 Rattail-Fabric2 Library
 
 This package contains various tasks and associated functions for use with
 Fabric deployment and maintenance.
 """
 
+from ._version import __version__
+
 from .core import (
     is_debian,
     get_debian_version,
     get_ubuntu_version,
     Deployer,
     make_deploy,
+    make_normal_user,
     make_system_user,
     mkdir,
     rsync,
     set_timezone,
     UNSPECIFIED,
 )
-from .util import exists, contains, append, sed
+from .util import exists, contains, append, sed, uncomment
```

### Comparing `rattail-fabric2-0.2.4/rattail_fabric2/composer.py` & `rattail-fabric2-0.3.0/rattail_fabric2/composer.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8; -*-
 ################################################################################
 #
 #  Rattail -- Retail Software Framework
-#  Copyright © 2010-2019 Lance Edgar
+#  Copyright © 2010-2022 Lance Edgar
 #
 #  This file is part of Rattail.
 #
 #  Rattail is free software: you can redistribute it and/or modify it under the
 #  terms of the GNU General Public License as published by the Free Software
 #  Foundation, either version 3 of the License, or (at your option) any later
 #  version.
@@ -20,22 +20,27 @@
 #  Rattail.  If not, see <http://www.gnu.org/licenses/>.
 #
 ################################################################################
 """
 Fabric lib for Composer (PHP dependency manager)
 """
 
-from __future__ import unicode_literals, absolute_import
-
-from rattail_fabric2 import make_deploy, exists
+from rattail_fabric2 import apt, make_deploy, exists
 
 
 deploy = make_deploy(__file__)
 
 
+def install(c, with_apt=True):
+    if with_apt:
+        apt.install(c, 'composer')
+    else:
+        install_globally(c)
+
+
 def install_globally(c):
     """
     Install `composer.phar` in global location
     """
     if not exists(c, '/usr/local/bin/composer.phar'):
         deploy(c, 'composer/install-composer.sh', '/tmp/install-composer.sh', mode='0700', use_sudo=True)
         c.sudo("bash -c 'cd /usr/local/bin; /tmp/install-composer.sh'")
```

### Comparing `rattail-fabric2-0.2.4/rattail_fabric2/backup.py` & `rattail-fabric2-0.3.0/rattail_fabric2/backup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8; -*-
 ################################################################################
 #
 #  Rattail -- Retail Software Framework
-#  Copyright © 2010-2019 Lance Edgar
+#  Copyright © 2010-2023 Lance Edgar
 #
 #  This file is part of Rattail.
 #
 #  Rattail is free software: you can redistribute it and/or modify it under the
 #  terms of the GNU General Public License as published by the Free Software
 #  Foundation, either version 3 of the License, or (at your option) any later
 #  version.
@@ -49,103 +49,121 @@
     context.setdefault('envname', 'backup')
     context.setdefault('user', 'rattail')
     deploy_generic(c, 'backup/backup-everything.mako', '/usr/local/bin/backup-everything',
                    mode='0700', context=context, use_sudo=True)
 
 
 def deploy_backup_app(c, deploy, envname, mkvirtualenv=True, user='rattail',
+                      python_exe='/usr/bin/python3',
                       install_borg=False,
+                      pyfuse3=False,
                       link_borg_to_bin=True,
                       install_luigi=False,
                       luigi_history_db=None,
                       luigi_listen_address='0.0.0.0',
                       install_rattail=True,
                       config=None,
                       rattail_backup_script=None,
                       everything=None,
                       crontab=None,
+                      crontab_mailto=None,
                       runat=UNSPECIFIED,
+                      logrotate=False,
                       context={}):
     """
     Make an app which can run backups for the server.
     """
     if install_rattail and not config:
         path = '{}/rattail.conf.mako'.format(envname)
         if deploy.local_exists(path):
             config = path
         else:
             path = '{}/rattail.conf'.format(envname)
             if deploy.local_exists(path):
                 config = path
             else:
-                raise ValueError("Must provide config path for backup app")
+                raise ValueError("Config file not found for backup; "
+                                 "please add {} to your deploy folder".format(path))
 
     if install_borg:
         borg.install_dependencies(c)
 
     if install_luigi:
         c.sudo('supervisorctl stop backup:')
 
     # virtualenv
-    if mkvirtualenv:
-        python.mkvirtualenv(c, envname, python='/usr/bin/python3', runas_user=user)
     envpath = '/srv/envs/{}'.format(envname)
-    c.sudo('chown -R {}: {}'.format(user, envpath))
-    mkdir(c, os.path.join(envpath, 'src'), use_sudo=True, runas_user=user)
-    c.sudo("bash -l -c 'workon {} && pip install --upgrade pip'".format(envname), user=user)
+    if mkvirtualenv and not exists(c, envpath):
+        mkdir(c, envpath, use_sudo=True, owner=user)
+        python.mkvirtualenv(c, envname, python=python_exe, runas_user=user)
+        c.sudo("bash -c 'PIP_CONFIG_FILE={0}/pip.conf {0}/bin/pip install -U pip setuptools wheel'".format(envpath),
+               user=user)
 
     if install_rattail:
 
         # rattail
+        mkdir(c, os.path.join(envpath, 'src'), use_sudo=True, runas_user=user)
         if not exists(c, os.path.join(envpath, 'src/rattail')):
-            c.sudo('git clone https://rattailproject.org/git/rattail.git {}/src/rattail'.format(envpath), user=user)
-            c.sudo("bash -l -c 'workon {} && cdvirtualenv && bin/pip install --editable src/rattail'".format(envname), user=user)
+            c.sudo('git clone https://kallithea.rattailproject.org/rattail-project/rattail {}/src/rattail'.format(envpath), user=user)
+            c.sudo("bash -c 'PIP_CONFIG_FILE={0}/pip.conf {0}/bin/pip install --editable {0}/src/rattail'".format(envpath),
+                   user=user)
         deploy_generic(c, 'backup/git-exclude', os.path.join(envpath, 'src/rattail/.git/info/exclude'), use_sudo=True, owner=user)
 
         # config
-        c.sudo("bash -l -c 'workon {} && cdvirtualenv && rattail make-appdir'".format(envname), user=user)
+        if not exists(c, os.path.join(envpath, 'app')):
+            c.sudo("bash -c 'cd {} && bin/rattail make-appdir'".format(envpath),
+                   user=user)
         # note, config is owned by root regardless of `user` - since we always run backups as root
-        deploy(c, config, os.path.join(envpath, 'app/rattail.conf'), owner='root:{}'.format(user), mode='0640', use_sudo=True, context=context)
-        c.sudo("bash -l -c 'workon {} && cdvirtualenv && bin/rattail -c app/rattail.conf make-config -T quiet -O app/'".format(envname), user=user)
-        c.sudo("bash -l -c 'workon {} && cdvirtualenv && bin/rattail -c app/rattail.conf make-config -T silent -O app/'".format(envname), user=user)
+        deploy(c, config, os.path.join(envpath, 'app/rattail.conf'), 
+               use_sudo=True, owner='root:{}'.format(user), mode='0640', 
+               context=context)
+        if not exists(c, os.path.join(envpath, 'app', 'quiet.conf')):
+            c.sudo("bash -c 'cd {} && bin/rattail -c app/rattail.conf make-config -T quiet -O app/'".format(envpath),
+                   user=user)
+        if not exists(c, os.path.join(envpath, 'app', 'silent.conf')):
+            c.sudo("bash -c 'cd {} && bin/rattail -c app/rattail.conf make-config -T silent -O app/'".format(envpath),
+                   user=user)
 
         # rattail-backup script
         script_context = dict(context)
         script_context['envname'] = envname
         if rattail_backup_script:
             deploy(c, rattail_backup_script, '/usr/local/bin/rattail-backup', mode='0700', use_sudo=True,
                    context=script_context)
         else:
             deploy_rattail_backup_script(c, **script_context)
 
     # borg
     if install_borg:
-        if install_rattail:
-            packages = [
-                'rattail[backup]',
-            ]
-        else:
-            # these should be same as rattail[backup]
-            packages = [
-                'msgpack',
-                'borgbackup',
-                'llfuse==1.3.4',
-            ]
-        c.sudo("bash -l -c 'workon {} && cdvirtualenv && bin/pip install {}'".format(envname, ' '.join(packages)), user=user)
+        if isinstance(install_borg, list):
+            packages = install_borg
+        elif isinstance(install_borg, str):
+            packages = [install_borg]
+        else:
+            packages = ['msgpack']
+            if pyfuse3:
+                apt.install(c, 'libfuse3-dev')
+                packages.append('borgbackup[pyfuse3]')
+            else:
+                # TODO: this is legacy and should stop being default
+                packages.append('borgbackup[fuse]')
+            c.sudo("bash -c 'PIP_CONFIG_FILE={0}/pip.conf {0}/bin/pip install {1}'".format(envpath, ' '.join(packages)),
+               user=user)
         if link_borg_to_bin:
             c.sudo("ln -sf {}/bin/borg /usr/local/bin/borg".format(envpath))
 
     # luigi
     if install_luigi:
         packages = ['luigi']
         if luigi_history_db:
             packages.append('SQLAlchemy')
             if luigi_history_db.startswith('postgresql://'):
                 packages.append('psycopg2')
-        c.sudo("bash -l -c 'workon {}; pip install {}'".format(envname, ' '.join(packages)), user=user)
+        c.sudo("bash -c 'PIP_CONFIG_FILE={0}/pip.conf {0}/bin/pip install {1}'".format(envpath, ' '.join(packages)),
+               user=user)
 
         # basic config
         mkdir(c, ['{}/app/luigitasks'.format(envpath),
                   '{}/app/luigi'.format(envpath),
                   '{}/app/luigi/log'.format(envpath),
                   '{}/app/work'.format(envpath),
         ], owner=user, use_sudo=True)
@@ -204,11 +222,23 @@
     if runat is UNSPECIFIED:
         runat = datetime.time(0) # defaults to midnight
     if runat is not None and (install_rattail or everything):
         crontab_context = dict(context)
         crontab_context['envname'] = envname
         crontab_context['pretty_time'] = runat.strftime('%I:%M %p')
         crontab_context['cron_time'] = runat.strftime('%M %H')
+
+        if crontab_mailto:
+            if isinstance(crontab_mailto, str):
+                crontab_mailto = [crontab_mailto]
+            crontab_mailto = ','.join(crontab_mailto)
+        crontab_context['mailto'] = crontab_mailto
+
         if crontab:
             deploy(c, crontab, '/etc/cron.d/backup', context=crontab_context, use_sudo=True)
         else:
             deploy_generic(c, 'backup/crontab.mako', '/etc/cron.d/backup', context=crontab_context, use_sudo=True)
+
+    # logrotate
+    if logrotate:
+        deploy_generic(c, 'backup/logrotate.conf', '/etc/logrotate.d/backup',
+                       use_sudo=True)
```

### Comparing `rattail-fabric2-0.2.4/rattail_fabric2/mysql.py` & `rattail-fabric2-0.3.0/rattail_fabric2/mysql.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8; -*-
 ################################################################################
 #
 #  Rattail -- Retail Software Framework
-#  Copyright © 2010-2020 Lance Edgar
+#  Copyright © 2010-2021 Lance Edgar
 #
 #  This file is part of Rattail.
 #
 #  Rattail is free software: you can redistribute it and/or modify it under the
 #  terms of the GNU General Public License as published by the Free Software
 #  Foundation, either version 3 of the License, or (at your option) any later
 #  version.
@@ -66,16 +66,23 @@
 def create_user(c, name, host='localhost', password=None, checkfirst=True):
     """
     Create a MySQL user account.
     """
     if not checkfirst or not user_exists(c, name, host):
         sql(c, "CREATE USER '{}'@'{}';".format(name, host))
     if password:
-        sql(c, "SET PASSWORD FOR '{}'@'{}' = PASSWORD('{}');".format(
-            name, host, password), hide=True, echo=False)
+        # supposedly this is the new way to do it
+        result = sql(c, "ALTER USER '{}'@'{}' IDENTIFIED BY '{}';".format(
+            name, host, password),
+            echo=False, hide=True, warn=True)
+        if result.failed: # but this may fail for older systems
+            # in which case we try it the old way
+            sql(c, "SET PASSWORD FOR '{}'@'{}' = PASSWORD('{}');".format(
+                name, host, password),
+                echo=False, hide=True)
 
 
 def db_exists(c, name):
     """
     Determine if a given MySQL database exists.
     """
     db = sql(c, "SELECT SCHEMA_NAME FROM SCHEMATA WHERE SCHEMA_NAME = '{0}'".format(name), database='information_schema').stdout.strip()
@@ -138,23 +145,25 @@
 def script(c, path, database=''):
     """
     Execute a SQL script against the given database.
     """
     c.sudo("bash -c 'mysql {} < {}'".format(database, path))
 
 
-def download_db(c, name, destination=None):
+def download_db(c, name, destination=None, **kwargs):
     """
     Download a database from the "current" server.
     """
     if destination is None:
         destination = './{}.sql.gz'.format(name)
+    triggers = '--skip-triggers' if kwargs.get('skip_triggers') else ''
+    mysqldump = 'mysqldump {0} --result-file={1}.sql {1}'.format(triggers, name)
     # note, we force sudo "as root" to ensure -H flag is used
     # (which allows us to leverage /root/.my.cnf config file)
-    c.sudo('mysqldump --result-file={0}.sql {0}'.format(name), user='root')
+    c.sudo(mysqldump, user='root')
     c.sudo('gzip --force {}.sql'.format(name))
     c.get('{}.sql.gz'.format(name), destination)
     c.sudo('rm {}.sql.gz'.format(name))
 
 
 def clone_db(c, name, download, user=None, force=False):
     """
```

### Comparing `rattail-fabric2-0.2.4/rattail_fabric2/util.py` & `rattail-fabric2-0.3.0/rattail_fabric2/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8; -*-
 ################################################################################
 #
 #  Rattail -- Retail Software Framework
-#  Copyright © 2010-2019 Lance Edgar
+#  Copyright © 2010-2023 Lance Edgar
 #
 #  This file is part of Rattail.
 #
 #  Rattail is free software: you can redistribute it and/or modify it under the
 #  terms of the GNU General Public License as published by the Free Software
 #  Foundation, either version 3 of the License, or (at your option) any later
 #  version.
@@ -236,14 +236,18 @@
         after = after.replace(char, r'\%s' % char)
     # Characters to be escaped in replacement only (they're useful in regexen
     # in the 'before' part)
     for char in "()":
         after = after.replace(char, r'\%s' % char)
     if limit:
         limit = r'/%s/ ' % limit
+
+    # if replacement text contains single quote chars, must escape them
+    after = after.replace("'", "'\"'\"'")
+
     context = {
         'script': r"'%ss/%s/%s/%sg'" % (limit, before, after, flags),
         'filename': _expand_path(c, filename),
         'backup': backup
     }
     # Test the OS because of differences between sed versions
```

### Comparing `rattail-fabric2-0.2.4/rattail_fabric2/apt.py` & `rattail-fabric2-0.3.0/rattail_fabric2/apt.py`

 * *Files 13% similar despite different names*

```diff
@@ -63,14 +63,24 @@
     Add a new entry to the apt/sources.list file
     """
     if c.run("grep '^{}' /etc/apt/sources.list".format(entry), warn=True).failed:
         c.sudo("""bash -c 'echo "{}" >> /etc/apt/sources.list'""".format(entry))
         update(c)
 
 
+def upgrade(c, frontend='noninteractive'):
+    """
+    Perform an ``apt-get upgrade`` operation.
+    """
+    options = ''
+    if frontend == 'noninteractive':
+        options = '--option Dpkg::Options::="--force-confdef" --option Dpkg::Options::="--force-confold"'
+    c.sudo('DEBIAN_FRONTEND={} apt-get --assume-yes {} upgrade'.format(frontend, options))
+
+
 def dist_upgrade(c, frontend='noninteractive'):
     """
     Perform a full ``apt-get dist-upgrade`` operation.
     """
     update(c)
     options = ''
     if frontend == 'noninteractive':
```

### Comparing `rattail-fabric2-0.2.4/rattail_fabric2/deploy/bouncer` & `rattail-fabric2-0.3.0/rattail_fabric2/deploy/soffice`

 * *Files 13% similar despite different names*

```diff
@@ -17,85 +17,68 @@
 #  FOR A PARTICULAR PURPOSE.  See the GNU General Public License for more
 #  details.
 #
 #  You should have received a copy of the GNU General Public License along with
 #  Rattail.  If not, see <http://www.gnu.org/licenses/>.
 #
 ################################################################################
+#
+# Generic 'init' script for headless LibreOffice Writer
+#
+################################################################################
 
+# "calling" init script may define any of the following as necessary:
 
-# This script is mostly based on the ``/etc/init.d/skeleton`` file from a
-# Debian 6 system.
-
-
-DESC=${DESC:-"Rattail Email Bouncer"}
-NAME=${NAME:-"rattail-bouncer"}
+NAME=${NAME:-"rattail-soffice"}
 SCRIPTNAME=${SCRIPTNAME:-"/etc/init.d/$NAME"}
-PIDFILE=${PIDFILE:-"/var/run/rattail/$NAME.pid"}
-
-PYTHON=${PYTHON:-"/usr/bin/python"}
-RATTAIL=${RATTAIL:-"/usr/local/bin/rattail"}
-RATTAIL_ARGS=${RATTAIL_ARGS:-""}
-BOUNCER_ARGS=${BOUNCER_ARGS:-"--pidfile=$PIDFILE"}
-
+DESC=${DESC:-"LibreOffice for Rattail"}
+DAEMON=${DAEMON:-"/usr/lib/libreoffice/program/soffice.bin"}
+SOFFICE=${SOFFICE:-"/usr/bin/soffice"}
 USER=${USER:-"rattail"}
 GROUP=${GROUP:-"rattail"}
-
-
-# Read configuration variable files if present.
-[ -r /etc/default/rattail ] && . /etc/default/rattail
-[ -r /etc/default/$NAME ] && . /etc/default/$NAME
-
-# Load the VERBOSE setting and other rcS variables.
-. /lib/init/vars.sh
-
-# Define LSB log_* functions.
-# Depend on lsb-base (>= 3.2-14) to ensure that this file is present
-# and status_of_proc is working.
-. /lib/lsb/init-functions
+PIDFILE=${PIDFILE:-"/var/run/rattail/$NAME.pid"}
+PORT=${PORT:-"2002"}
 
 
 create_pid_dir() {
     PIDDIR=`dirname "$PIDFILE"`
     if [ ! -d "$PIDDIR" ]; then
         mkdir --parents "$PIDDIR"
     fi
     chown $USER:$GROUP "$PIDDIR"
 }
 
 
-#
-# Function that starts the daemon/service
-#
-do_start()
-{
-    # Return
-    #   0 if daemon has been started
-    #   1 if daemon was already running
-    #   2 if daemon could not be started
+# Return
+#   0 if daemon has been started
+#   1 if daemon was already running
+#   2 if daemon could not be started
+do_start() {
+
     create_pid_dir
-    start-stop-daemon --start --pidfile $PIDFILE --exec $PYTHON --user $USER --test --quiet > /dev/null \
+
+    start-stop-daemon --test --start --exec $DAEMON --user $USER --pidfile $PIDFILE --quiet > /dev/null \
         || return 1
-    start-stop-daemon --start --pidfile $PIDFILE --exec $PYTHON --startas $RATTAIL --chuid $USER --group $GROUP --quiet -- \
-        $RATTAIL_ARGS bouncer $BOUNCER_ARGS start \
+    start-stop-daemon --start --chuid $USER --exec $DAEMON --startas $SOFFICE --pidfile $PIDFILE --background --quiet -- \
+                      --headless --pidfile=$PIDFILE --accept="socket,host=localhost,port=$PORT;urp;" \
         || return 2
 }
 
 
-#
-# Function that stops the daemon/service
-#
+# Return
+#   0 if daemon has been stopped
+#   1 if daemon was already stopped
+#   2 if daemon could not be stopped
+#   other if a failure occurred
 do_stop()
 {
-    # Return
-    #   0 if daemon has been stopped
-    #   1 if daemon was already stopped
-    #   2 if daemon could not be stopped
-    #   other if a failure occurred
-    sudo -u $USER $RATTAIL $RATTAIL_ARGS bouncer $BOUNCER_ARGS stop > /dev/null 2>&1
+    start-stop-daemon --test --stop --exec $DAEMON --user $USER --pidfile $PIDFILE --quiet > /dev/null \
+        || return 1
+    start-stop-daemon --stop --exec $DAEMON --user $USER --pidfile $PIDFILE --quiet > /dev/null \
+        || return 2
 }
 
 
 case "$1" in
     start)
         [ "$VERBOSE" != no ] && log_daemon_msg "Starting $DESC" "$NAME"
         do_start
@@ -109,15 +92,15 @@
         do_stop
         case "$?" in
             0|1) [ "$VERBOSE" != no ] && log_end_msg 0 ;;
             2) [ "$VERBOSE" != no ] && log_end_msg 1 ;;
         esac
         ;;
     status)
-        status_of_proc "$DAEMON" "$NAME" && exit 0 || exit $?
+        /usr/local/bin/check-rattail-daemon "$NAME" && exit 0 || exit $?
         ;;
     restart|force-reload)
         log_daemon_msg "Restarting $DESC" "$NAME"
         do_stop
         case "$?" in
             0|1)
                 do_start
```

### Comparing `rattail-fabric2-0.2.4/rattail_fabric2/deploy/check-systemd-service` & `rattail-fabric2-0.3.0/rattail_fabric2/deploy/check-systemd-service`

 * *Files identical despite different names*

### Comparing `rattail-fabric2-0.2.4/rattail_fabric2/deploy/backup/upgrade.sh.mako` & `rattail-fabric2-0.3.0/rattail_fabric2/deploy/backup/upgrade.sh.mako`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 #!/bin/sh -e
 
 if [ "$1" = "-v" -o "$1" = "--verbose" ]; then
     VERBOSE='--verbose'
     QUIET=
+    PROGRESSBAR='--progress-bar=on'
 else
     VERBOSE=
     QUIET='--quiet'
+    PROGRESSBAR='--progress-bar=off'
 fi
 
 PIP="sudo -H -u ${user} PIP_CONFIG_FILE=${envpath}/pip.conf ${envpath}/bin/pip"
 
 
 # upgrade pip
-$PIP install $QUIET --upgrade pip
+$PIP install $QUIET $PROGRESSBAR --upgrade pip
 
 # upgrade rattail
 cd ${envpath}/src/rattail
 if [ "$(sudo -H -u ${user} git status --porcelain)" != '' ]; then
    sudo -H -u ${user} git status
    exit 1
 fi
 sudo -H -u ${user} git pull $QUIET
 find . -name '*.pyc' -delete
-$PIP install $QUIET --upgrade --upgrade-strategy eager --editable .
+$PIP install $QUIET $PROGRESSBAR --upgrade --upgrade-strategy eager --editable .
```

### Comparing `rattail-fabric2-0.2.4/rattail_fabric2/deploy/backup/luigi.cfg.mako` & `rattail-fabric2-0.3.0/rattail_fabric2/deploy/backup/luigi.cfg.mako`

 * *Files identical despite different names*

### Comparing `rattail-fabric2-0.2.4/rattail_fabric2/deploy/backup/overnight-backups.sh.mako` & `rattail-fabric2-0.3.0/rattail_fabric2/deploy/backup/overnight-backups.sh.mako`

 * *Files identical despite different names*

### Comparing `rattail-fabric2-0.2.4/rattail_fabric2/deploy/backup/luigi-overnight.py` & `rattail-fabric2-0.3.0/rattail_fabric2/deploy/backup/luigi-overnight.py`

 * *Files identical despite different names*

### Comparing `rattail-fabric2-0.2.4/rattail_fabric2/deploy/backup/luigi-logging.conf.mako` & `rattail-fabric2-0.3.0/rattail_fabric2/deploy/backup/luigi-logging.conf.mako`

 * *Files identical despite different names*

### Comparing `rattail-fabric2-0.2.4/rattail_fabric2/deploy/backup/backup-everything.mako` & `rattail-fabric2-0.3.0/rattail_fabric2/deploy/backup/backup-everything.mako`

 * *Files identical despite different names*

### Comparing `rattail-fabric2-0.2.4/rattail_fabric2/deploy/check-supervisor-process` & `rattail-fabric2-0.3.0/rattail_fabric2/deploy/check-supervisor-process`

 * *Files identical despite different names*

### Comparing `rattail-fabric2-0.2.4/rattail_fabric2/deploy/check-rattail-daemon` & `rattail-fabric2-0.3.0/rattail_fabric2/deploy/check-rattail-daemon`

 * *Files identical despite different names*

### Comparing `rattail-fabric2-0.2.4/rattail_fabric2/python.py` & `rattail-fabric2-0.3.0/rattail_fabric2/python.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8; -*-
 ################################################################################
 #
 #  Rattail -- Retail Software Framework
-#  Copyright © 2010-2020 Lance Edgar
+#  Copyright © 2010-2022 Lance Edgar
 #
 #  This file is part of Rattail.
 #
 #  Rattail is free software: you can redistribute it and/or modify it under the
 #  terms of the GNU General Public License as published by the Free Software
 #  Foundation, either version 3 of the License, or (at your option) any later
 #  version.
@@ -22,27 +22,30 @@
 ################################################################################
 """
 Fabric Library for Python
 """
 
 from contextlib import contextmanager
 
-from rattail_fabric2 import apt, exists, make_deploy, mkdir
+from rattail_fabric2 import apt, append, exists, make_deploy, mkdir
 
 
-deploy = make_deploy(__file__)
+deploy_common = make_deploy(__file__)
 
 
-def bootstrap_python(c, pip_from_apt=True, pip_eager=True,
+def bootstrap_python(c, deploy=None,
+                     pip_from_apt=True,
+                     pip_eager=True,
                      pip_method=None,
                      pip_auto=False,
                      pip_package_name=None,
                      virtualenvwrapper_from_apt=False,
                      upgrade_virtualenvwrapper=True,
-                     workon_home='/srv/envs', user='rattail',
+                     workon_home='/srv/envs',
+                     user='rattail',
                      python3=False):
     """
     Bootstrap a "complete" Python install.
     """
     # build dependencies
     apt.install(
         c,
@@ -63,39 +66,56 @@
 
     # virtualenvwrapper
     workon_home = workon_home.rstrip('/')
     install_virtualenvwrapper(c, workon_home=workon_home, user=user,
                               use_apt=virtualenvwrapper_from_apt,
                               upgrade=upgrade_virtualenvwrapper,
                               configure_me=False)
-    deploy(c, 'python/premkvirtualenv', '{}/premkvirtualenv'.format(workon_home), owner=user, use_sudo=True)
+    # TODO: let custom deploy override this
+    deploy_common(c, 'python/premkvirtualenv', '{}/premkvirtualenv'.format(workon_home), owner=user, use_sudo=True)
 
 
 def install_pythonz(c):
     """
     Install the 'pythonz' utility, for installing arbitrary versions of python.
 
     https://github.com/saghul/pythonz/blob/master/README.rst#installation
     """
     apt.install(
         c,
         'curl',
         # these are needed when building python:
         'libsqlite3-dev',
+        'libssl-dev',
         'zlib1g-dev',
     )
     if not exists(c, '/usr/local/pythonz'):
         if not exists(c, '/usr/local/src/pythonz'):
             mkdir(c, '/usr/local/src/pythonz', use_sudo=True)
         if not exists(c, '/usr/local/src/pythonz/pythonz-install'):
             c.sudo('curl -kL -o /usr/local/src/pythonz/pythonz-install https://raw.github.com/saghul/pythonz/master/pythonz-install')
             c.sudo('chmod +x /usr/local/src/pythonz/pythonz-install')
         c.sudo('/usr/local/src/pythonz/pythonz-install')
 
 
+def configure_pythonz(c, user):
+    """
+    Configure the given user's ``.bashrc`` to allow use of pythonz.
+    """
+    # TODO: should normalize this get_home_dir() logic?
+    home = c.run('getent passwd {} | cut -d: -f6'.format(user)).stdout.strip()
+    home = home.rstrip('/')
+
+    script = '{}/.bashrc'.format(home)
+    append(c, script, 'export PYTHONZ_ROOT=/usr/local/pythonz',
+           use_sudo=True)
+    append(c, script, '[[ -s /usr/local/pythonz/etc/bashrc ]] && source /usr/local/pythonz/etc/bashrc',
+           use_sudo=True)
+
+
 def install_python(c, version, globally=False, verbose=False):
     """
     Install a specific version of python, via pythonz.
 
     :param globally: Whether or not this python should be registered globally,
        by placing a symlink to it in ``/usr/local/bin``.  Note that this
        symlink, if installed, will use the "short" version, e.g. if the
@@ -126,15 +146,18 @@
     if method == 'apt':
         package = apt_package_name
         if not package:
             package = 'python3-pip' if python3 else 'python-pip'
         apt.install(c, package, warn=True)
 
     elif method == 'get-pip':
-        c.sudo('wget -O get-pip.py https://bootstrap.pypa.io/get-pip.py')
+        url = 'https://bootstrap.pypa.io/get-pip.py'
+        if not python3:
+            url = 'https://bootstrap.pypa.io/pip/2.7/get-pip.py'
+        c.sudo('wget -O get-pip.py {}'.format(url))
         python = 'python3' if python3 else 'python2'
         c.sudo('{} get-pip.py'.format(python))
         c.sudo('rm get-pip.py')
 
     elif auto: # try apt first, then fall back to get-pip.py
         package = apt_package_name
         if not package:
@@ -200,22 +223,24 @@
     mkdir(c, workon_home, owner=user, use_sudo=True)
     if use_apt:
         apt.install(c, 'virtualenvwrapper')
         configure_virtualenvwrapper(c, user, workon_home,
                                     wrapper='/usr/share/virtualenvwrapper/virtualenvwrapper.sh')
     else:
         pip(c, 'virtualenvwrapper', upgrade=upgrade)
-        configure_virtualenvwrapper(c, user, workon_home)
+        configure_virtualenvwrapper(c, user, workon_home,
+                                    wrapper='/usr/local/bin/virtualenvwrapper.sh')
         if configure_me:
             # TODO
             # configure_virtualenvwrapper(c, env.user, workon_home)
             raise NotImplementedError
 
 
 def configure_virtualenvwrapper(c, user, workon_home='/srv/envs',
+                                # TODO: this default should change, per apt
                                 wrapper='/usr/local/bin/virtualenvwrapper.sh'):
     """
     Configure virtualenvwrapper for the given user account.
     """
     home = c.run('getent passwd {} | cut -d: -f6'.format(user)).stdout.strip()
     home = home.rstrip('/')
```

### Comparing `rattail-fabric2-0.2.4/rattail_fabric2/postgresql.py` & `rattail-fabric2-0.3.0/rattail_fabric2/postgresql.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8; -*-
 ################################################################################
 #
 #  Rattail -- Retail Software Framework
-#  Copyright © 2010-2019 Lance Edgar
+#  Copyright © 2010-2023 Lance Edgar
 #
 #  This file is part of Rattail.
 #
 #  Rattail is free software: you can redistribute it and/or modify it under the
 #  terms of the GNU General Public License as published by the Free Software
 #  Foundation, either version 3 of the License, or (at your option) any later
 #  version.
@@ -23,58 +23,120 @@
 """
 Fabric Library for PostgreSQL
 """
 
 import os
 import re
 
-from rattail_fabric2 import apt
+from rattail_fabric2 import apt, append, contains, sed, uncomment
 
 
 def install(c):
     """
     Install the PostgreSQL database service
     """
-    apt.install(c, 'postgresql')
+    apt.install(c, 'postgresql', 'libpq-dev')
 
 
 def get_version(c):
     """
     Fetch the version of PostgreSQL running on the target system
     """
     result = c.run('psql --version', warn=True)
     if not result.failed:
         match = re.match(r'^psql \(PostgreSQL\) (\d+\.\d+)(?:\.\d+)?', result.stdout.strip())
         if match:
             return float(match.group(1))
 
+
+def set_listen_addresses(c, *addresses):
+    """
+    Overwrite the `listen_addresses` config setting in `postgresql.conf`.
+    """
+    version = get_version(c)
+    if version > 12:
+        version = int(version)
+
+    addresses = ','.join(addresses)
+
+    if not contains(c, '/etc/postgresql/{}/main/postgresql.conf'.format(version),
+                    "listen_addresses = '{}'".format(addresses),
+                    exact=True):
+
+        uncomment(c, '/etc/postgresql/{}/main/postgresql.conf'.format(version),
+                  r'^# *listen_addresses\s*=.*',
+                  use_sudo=True)
+
+        sed(c, '/etc/postgresql/{}/main/postgresql.conf'.format(version),
+            r'listen_addresses\s*=.*',
+            "listen_addresses = '{}'".format(addresses),
+            use_sudo=True)
+
+        restart(c)
+
+
+def add_hba_entry(c, entry):
+    """
+    Add an entry to the `pg_hba.conf` file.
+    """
+    version = get_version(c)
+    if version > 12:
+        version = int(version)
+
+    if not contains(c, '/etc/postgresql/{}/main/pg_hba.conf'.format(version),
+                    entry, use_sudo=True):
+        append(c, '/etc/postgresql/{}/main/pg_hba.conf'.format(version),
+               entry, use_sudo=True)
+        reload_(c)
+
+
 def restart(c):
     """
     Restart the PostgreSQL database service
     """
     c.sudo('systemctl restart postgresql.service')
 
 
-def reload(c):
+def reload_(c):
     """
     Reload config for the PostgreSQL database service
     """
     c.sudo('systemctl reload postgresql.service')
 
+# TODO: deprecate / remove this
+reload = reload_
+
 
 def sql(c, sql, database='', port=None, **kwargs):
     """
     Execute some SQL as the 'postgres' user.
     """
     cmd = 'psql {port} --tuples-only --no-align --command="{sql}" {database}'.format(
         port='--port={}'.format(port) if port else '',
         sql=sql, database=database)
     return c.sudo(cmd, user='postgres', **kwargs)
 
 
+def script(c, path, database='', port=None, user=None, password=None):
+    """
+    Execute a SQL script.  By default this will run as 'postgres' user, but can
+    use PGPASSWORD authentication if necessary.
+    """
+    port = '--port={}'.format(port) if port else ''
+    if user and password:
+        kw = dict(pw=password, user=user, port=port, path=path, db=database)
+        return c.sudo(" PGPASSWORD='{pw}' psql --host=localhost {port} --username='{user}' --file='{path}' {db}".format(**kw),
+                      echo=False)
+
+    else: # run as postgres
+        kw = dict(port=port, path=path, db=database)
+        return c.sudo("psql {port} --file='{path}' {db}".format(**kw),
+                      user='postgres')
+
+
 def user_exists(c, name, port=None):
     """
     Determine if a given PostgreSQL user exists.
     """
     user = sql(c, "SELECT rolname FROM pg_roles WHERE rolname = '{0}'".format(name), port=port).stdout.strip()
     return bool(user)
 
@@ -133,30 +195,42 @@
     """
     Drop a PostgreSQL database.
     """
     if not checkfirst or db_exists(c, name):
         c.sudo('dropdb {}'.format(name), user='postgres')
 
 
-def download_db(c, name, destination=None, port=None, exclude_tables=None):
+def dump_db(c, name, port=None, exclude_tables=None):
     """
-    Download a database from the server represented by ``c`` param.
+    Dump a database to file, on the server represented by ``c`` param.
+
+    This function returns the name of the DB dump file.  The name will not have
+    a path component as it's assumed to be in the home folder of the connection
+    user.
     """
-    if destination is None:
-        destination = './{}.sql.gz'.format(name)
     c.run('touch {}.sql'.format(name))
     c.run('chmod 0666 {}.sql'.format(name))
     cmd = 'pg_dump {port} {exclude_tables} --file={name}.sql {name}'.format(
         name=name,
         port='--port={}'.format(port) if port else '',
         exclude_tables='--exclude-table-data={}'.format(exclude_tables) if exclude_tables else '')
     c.sudo(cmd, user='postgres')
     c.run('gzip --force {}.sql'.format(name))
-    c.get('{}.sql.gz'.format(name), destination)
-    c.run('rm {}.sql.gz'.format(name))
+    return '{}.sql.gz'.format(name)
+
+
+def download_db(c, name, destination=None, port=None, exclude_tables=None):
+    """
+    Download a database from the server represented by ``c`` param.
+    """
+    if destination is None:
+        destination = './{}.sql.gz'.format(name)
+    dumpfile = dump_db(c, name, port=port, exclude_tables=exclude_tables)
+    c.get(dumpfile, destination)
+    c.run('rm {}'.format(dumpfile))
 
 
 def clone_db(c, name, owner, download, user='rattail', force=False, workdir=None):
     """
     Clone a database from a (presumably live) server
 
     :param name: Name of the database.
@@ -181,10 +255,26 @@
     download(c, '{}.sql.gz'.format(name), user=user)
     c.put('{}.sql.gz'.format(name))
     c.local('rm {}.sql.gz'.format(name))
     if workdir:
         os.chdir(curdir)
 
     # restore database on target server
-    c.run('gunzip --force {}.sql.gz'.format(name))
-    c.sudo('psql --echo-errors --file={0}.sql {0}'.format(name), user='postgres')
-    c.run('rm {}.sql'.format(name))
+    restore_db(c, name, '{}.sql.gz'.format(name))
+
+
+def restore_db(c, name, path):
+    """
+    Restore a database from a dump file.
+
+    :param name: Name of the database to restore.
+
+    :param path: Path to the DB dump file, which should end in ``.sql.gz``
+    """
+    if not path.endswith('.sql.gz'):
+        raise ValueError("Path to dump file must end in `.sql.gz`")
+
+    c.run('gunzip --force {}'.format(path))
+    sql_path = path[:-3]
+    c.sudo('psql --echo-errors --file={} {}'.format(sql_path, name),
+           user='postgres')
+    c.run('rm {}'.format(sql_path))
```

### Comparing `rattail-fabric2-0.2.4/rattail_fabric2/nodejs.py` & `rattail-fabric2-0.3.0/rattail_fabric2/nodejs.py`

 * *Files identical despite different names*

### Comparing `rattail-fabric2-0.2.4/rattail_fabric2/soffice.py` & `rattail-fabric2-0.3.0/rattail_fabric2/soffice.py`

 * *Files identical despite different names*

### Comparing `rattail-fabric2-0.2.4/rattail_fabric2/postfix.py` & `rattail-fabric2-0.3.0/rattail_fabric2/postfix.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8; -*-
 ################################################################################
 #
 #  Rattail -- Retail Software Framework
-#  Copyright © 2010-2019 Lance Edgar
+#  Copyright © 2010-2022 Lance Edgar
 #
 #  This file is part of Rattail.
 #
 #  Rattail is free software: you can redistribute it and/or modify it under the
 #  terms of the GNU General Public License as published by the Free Software
 #  Foundation, either version 3 of the License, or (at your option) any later
 #  version.
@@ -21,14 +21,15 @@
 #
 ################################################################################
 """
 Fabric library for Postfix
 """
 
 from rattail_fabric2 import apt
+from rattail.util import shlex_join
 
 
 def install(c):
     """
     Install the Postfix mail service
     """
     apt.install(c, 'postfix')
@@ -38,18 +39,25 @@
 def alias(c, name, alias_to, path='/etc/aliases'):
     """
     Set a mail alias for Postfix
     """
     # does alias entry already exist?
     if c.run("grep '^{}:' /etc/aliases".format(name), warn=True).failed:
         # append new entry
-        c.sudo("""bash -c 'echo "{}: {}" >> /etc/aliases'""".format(name, alias_to))
+        entry = '{}: {}'.format(name, alias_to)
+        echo = shlex_join(['echo', entry])
+        cmd = '{} >> /etc/aliases'.format(echo)
+        cmd = shlex_join(['bash', '-c', cmd])
+        c.sudo(cmd)
     else:
         # update existing entry
-        c.sudo('sed -i.bak -e "s/^{}: .*/{}: {}/" /etc/aliases'.format(name, name, alias_to))
+        alias_to = alias_to.replace('|', '\\|')
+        sub = "s|^{}: .*|{}: {}|".format(name, name, alias_to)
+        cmd = shlex_join(['sed', '-i.bak', '-E', sub, '/etc/aliases'])
+        c.sudo(cmd)
 
     c.sudo('newaliases')
 
 
 def restart(c):
     """
     Restart the Postfix mail service
```

### Comparing `rattail-fabric2-0.2.4/rattail_fabric2/borg.py` & `rattail-fabric2-0.3.0/rattail_fabric2/borg.py`

 * *Files identical despite different names*

### Comparing `rattail-fabric2-0.2.4/rattail_fabric2/certbot.py` & `rattail-fabric2-0.3.0/rattail_fabric2/certbot.py`

 * *Files identical despite different names*

