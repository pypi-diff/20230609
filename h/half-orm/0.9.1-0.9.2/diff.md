# Comparing `tmp/half_orm-0.9.1.tar.gz` & `tmp/half_orm-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "half_orm-0.9.1.tar", last modified: Mon May 22 08:19:19 2023, max compression
+gzip compressed data, was "half_orm-0.9.2.tar", last modified: Fri Jun  9 07:02:18 2023, max compression
```

## Comparing `half_orm-0.9.1.tar` & `half_orm-0.9.2.tar`

### file list

```diff
@@ -1,66 +1,67 @@
-drwxr-xr-x   0 joel      (1000) joel      (1000)        0 2023-05-22 08:19:19.000856 half_orm-0.9.1/
--rw-r--r--   0 joel      (1000) joel      (1000)       97 2023-02-02 08:59:25.000000 half_orm-0.9.1/AUTHORS
--rw-r--r--   0 joel      (1000) joel      (1000)      699 2023-02-02 08:59:25.000000 half_orm-0.9.1/LICENSE
--rw-r--r--   0 joel      (1000) joel      (1000)    27388 2023-05-22 08:19:19.000856 half_orm-0.9.1/PKG-INFO
--rw-r--r--   0 joel      (1000) joel      (1000)    26447 2023-05-22 08:13:46.000000 half_orm-0.9.1/README.md
-drwxr-xr-x   0 joel      (1000) joel      (1000)        0 2023-05-22 08:19:18.996856 half_orm-0.9.1/half_orm/
--rw-r--r--   0 joel      (1000) joel      (1000)      172 2023-02-02 08:59:25.000000 half_orm-0.9.1/half_orm/__init__.py
--rw-r--r--   0 joel      (1000) joel      (1000)     5495 2023-05-12 08:02:28.000000 half_orm-0.9.1/half_orm/field.py
--rw-r--r--   0 joel      (1000) joel      (1000)       70 2023-02-02 08:59:25.000000 half_orm-0.9.1/half_orm/field_errors.py
--rw-r--r--   0 joel      (1000) joel      (1000)     5558 2023-05-12 08:04:47.000000 half_orm-0.9.1/half_orm/fkey.py
--rw-r--r--   0 joel      (1000) joel      (1000)     3513 2023-05-12 08:00:34.000000 half_orm-0.9.1/half_orm/hotest.py
--rwxr-xr-x   0 joel      (1000) joel      (1000)    14440 2023-04-21 09:03:14.000000 half_orm-0.9.1/half_orm/model.py
--rw-r--r--   0 joel      (1000) joel      (1000)     1143 2023-03-21 09:29:02.000000 half_orm-0.9.1/half_orm/model_errors.py
--rw-r--r--   0 joel      (1000) joel      (1000)      405 2023-03-18 07:38:44.000000 half_orm-0.9.1/half_orm/null.py
-drwxr-xr-x   0 joel      (1000) joel      (1000)        0 2023-05-22 08:19:19.000856 half_orm-0.9.1/half_orm/packager/
--rw-r--r--   0 joel      (1000) joel      (1000)        0 2023-02-28 10:33:54.000000 half_orm-0.9.1/half_orm/packager/__init__.py
--rw-r--r--   0 joel      (1000) joel      (1000)     3794 2023-05-19 09:57:24.000000 half_orm-0.9.1/half_orm/packager/changelog.py
--rw-r--r--   0 joel      (1000) joel      (1000)     4536 2023-05-19 08:11:53.000000 half_orm-0.9.1/half_orm/packager/database.py
--rw-r--r--   0 joel      (1000) joel      (1000)     4652 2023-05-19 09:54:22.000000 half_orm-0.9.1/half_orm/packager/db_conn.py
--rw-r--r--   0 joel      (1000) joel      (1000)     7522 2023-02-28 10:33:54.000000 half_orm-0.9.1/half_orm/packager/hgit.py
--rwxr-xr-x   0 joel      (1000) joel      (1000)     5373 2023-05-19 07:56:23.000000 half_orm-0.9.1/half_orm/packager/hop.py
--rw-r--r--   0 joel      (1000) joel      (1000)     1274 2023-02-28 10:33:54.000000 half_orm-0.9.1/half_orm/packager/manifest.py
--rwxr-xr-x   0 joel      (1000) joel      (1000)     8882 2023-02-28 10:33:54.000000 half_orm-0.9.1/half_orm/packager/modules.py
--rwxr-xr-x   0 joel      (1000) joel      (1000)    13389 2023-05-19 09:54:16.000000 half_orm-0.9.1/half_orm/packager/patch.py
-drwxr-xr-x   0 joel      (1000) joel      (1000)        0 2023-05-22 08:19:19.000856 half_orm-0.9.1/half_orm/packager/patches/
-drwxr-xr-x   0 joel      (1000) joel      (1000)        0 2023-05-22 08:19:18.992856 half_orm-0.9.1/half_orm/packager/patches/0/
-drwxr-xr-x   0 joel      (1000) joel      (1000)        0 2023-05-22 08:19:18.992856 half_orm-0.9.1/half_orm/packager/patches/0/1/
-drwxr-xr-x   0 joel      (1000) joel      (1000)        0 2023-05-22 08:19:19.000856 half_orm-0.9.1/half_orm/packager/patches/0/1/0/
--rw-r--r--   0 joel      (1000) joel      (1000)     1076 2023-02-28 10:33:54.000000 half_orm-0.9.1/half_orm/packager/patches/0/1/0/00_half_orm_meta.database.sql
--rw-r--r--   0 joel      (1000) joel      (1000)      183 2023-02-28 10:33:54.000000 half_orm-0.9.1/half_orm/packager/patches/0/1/0/01_alter_half_orm_meta.hop_release.sql
--rw-r--r--   0 joel      (1000) joel      (1000)      306 2023-05-22 07:11:49.000000 half_orm-0.9.1/half_orm/packager/patches/0/1/0/02_half_orm_meta.view.hop_penultimate_release.sql
--rw-r--r--   0 joel      (1000) joel      (1000)       22 2023-02-28 10:33:54.000000 half_orm-0.9.1/half_orm/packager/patches/log
-drwxr-xr-x   0 joel      (1000) joel      (1000)        0 2023-05-22 08:19:19.000856 half_orm-0.9.1/half_orm/packager/patches/sql/
--rw-r--r--   0 joel      (1000) joel      (1000)     5864 2023-05-22 07:14:29.000000 half_orm-0.9.1/half_orm/packager/patches/sql/half_orm_meta.sql
--rw-r--r--   0 joel      (1000) joel      (1000)     8618 2023-05-19 07:57:31.000000 half_orm-0.9.1/half_orm/packager/repo.py
-drwxr-xr-x   0 joel      (1000) joel      (1000)        0 2023-05-22 08:19:19.000856 half_orm-0.9.1/half_orm/packager/templates/
--rw-r--r--   0 joel      (1000) joel      (1000)       86 2023-02-28 10:33:54.000000 half_orm-0.9.1/half_orm/packager/templates/.gitignore
--rw-r--r--   0 joel      (1000) joel      (1000)       25 2023-02-28 10:33:54.000000 half_orm-0.9.1/half_orm/packager/templates/MANIFEST.in
--rw-r--r--   0 joel      (1000) joel      (1000)      218 2023-02-28 10:33:54.000000 half_orm-0.9.1/half_orm/packager/templates/Pipfile
--rw-r--r--   0 joel      (1000) joel      (1000)      924 2023-02-28 10:33:54.000000 half_orm-0.9.1/half_orm/packager/templates/README
--rw-r--r--   0 joel      (1000) joel      (1000)      367 2023-02-28 10:33:54.000000 half_orm-0.9.1/half_orm/packager/templates/base_test
--rw-r--r--   0 joel      (1000) joel      (1000)      437 2023-02-28 10:33:54.000000 half_orm-0.9.1/half_orm/packager/templates/db_connector.py
--rw-r--r--   0 joel      (1000) joel      (1000)      246 2023-02-28 10:33:54.000000 half_orm-0.9.1/half_orm/packager/templates/module_template_1
--rw-r--r--   0 joel      (1000) joel      (1000)      120 2023-02-28 10:33:54.000000 half_orm-0.9.1/half_orm/packager/templates/module_template_2
--rw-r--r--   0 joel      (1000) joel      (1000)       69 2023-02-28 10:33:54.000000 half_orm-0.9.1/half_orm/packager/templates/module_template_3
--rw-r--r--   0 joel      (1000) joel      (1000)      460 2023-02-28 10:33:54.000000 half_orm-0.9.1/half_orm/packager/templates/relation_test
--rw-r--r--   0 joel      (1000) joel      (1000)     2070 2023-02-28 10:33:54.000000 half_orm-0.9.1/half_orm/packager/templates/setup.py
--rw-r--r--   0 joel      (1000) joel      (1000)      490 2023-02-28 10:33:54.000000 half_orm-0.9.1/half_orm/packager/templates/warning
--rw-r--r--   0 joel      (1000) joel      (1000)     2099 2023-04-20 09:30:05.000000 half_orm-0.9.1/half_orm/packager/utils.py
--rw-r--r--   0 joel      (1000) joel      (1000)        8 2023-02-28 10:33:54.000000 half_orm-0.9.1/half_orm/packager/version.txt
--rw-r--r--   0 joel      (1000) joel      (1000)    17049 2023-04-20 09:30:05.000000 half_orm-0.9.1/half_orm/pg_meta.py
--rw-r--r--   0 joel      (1000) joel      (1000)    39274 2023-05-12 08:04:42.000000 half_orm-0.9.1/half_orm/relation.py
--rw-r--r--   0 joel      (1000) joel      (1000)     1520 2023-05-12 08:00:34.000000 half_orm-0.9.1/half_orm/relation_errors.py
--rw-r--r--   0 joel      (1000) joel      (1000)     3876 2023-05-12 08:00:07.000000 half_orm-0.9.1/half_orm/relation_factory.py
--rw-r--r--   0 joel      (1000) joel      (1000)     2743 2023-03-21 09:29:02.000000 half_orm-0.9.1/half_orm/transaction.py
--rw-r--r--   0 joel      (1000) joel      (1000)        6 2023-05-22 08:12:53.000000 half_orm-0.9.1/half_orm/version.txt
-drwxr-xr-x   0 joel      (1000) joel      (1000)        0 2023-05-22 08:19:18.996856 half_orm-0.9.1/half_orm.egg-info/
--rw-r--r--   0 joel      (1000) joel      (1000)    27388 2023-05-22 08:19:18.000000 half_orm-0.9.1/half_orm.egg-info/PKG-INFO
--rw-r--r--   0 joel      (1000) joel      (1000)     1664 2023-05-22 08:19:18.000000 half_orm-0.9.1/half_orm.egg-info/SOURCES.txt
--rw-r--r--   0 joel      (1000) joel      (1000)        1 2023-05-22 08:19:18.000000 half_orm-0.9.1/half_orm.egg-info/dependency_links.txt
--rw-r--r--   0 joel      (1000) joel      (1000)       51 2023-05-22 08:19:18.000000 half_orm-0.9.1/half_orm.egg-info/entry_points.txt
--rw-r--r--   0 joel      (1000) joel      (1000)       46 2023-05-22 08:19:18.000000 half_orm-0.9.1/half_orm.egg-info/requires.txt
--rw-r--r--   0 joel      (1000) joel      (1000)       27 2023-05-22 08:19:18.000000 half_orm-0.9.1/half_orm.egg-info/top_level.txt
--rw-r--r--   0 joel      (1000) joel      (1000)      100 2023-01-04 14:18:53.000000 half_orm-0.9.1/pyproject.toml
--rw-r--r--   0 joel      (1000) joel      (1000)       38 2023-05-22 08:19:19.000856 half_orm-0.9.1/setup.cfg
--rw-r--r--   0 joel      (1000) joel      (1000)     2502 2023-03-06 08:18:37.000000 half_orm-0.9.1/setup.py
+drwxr-xr-x   0 joel      (1000) joel      (1000)        0 2023-06-09 07:02:18.626452 half_orm-0.9.2/
+-rw-r--r--   0 joel      (1000) joel      (1000)       97 2023-02-02 08:59:25.000000 half_orm-0.9.2/AUTHORS
+-rw-r--r--   0 joel      (1000) joel      (1000)      699 2023-02-02 08:59:25.000000 half_orm-0.9.2/LICENSE
+-rw-r--r--   0 joel      (1000) joel      (1000)    27277 2023-06-09 07:02:18.626452 half_orm-0.9.2/PKG-INFO
+-rw-r--r--   0 joel      (1000) joel      (1000)    26336 2023-06-09 06:36:48.000000 half_orm-0.9.2/README.md
+drwxr-xr-x   0 joel      (1000) joel      (1000)        0 2023-06-09 07:02:18.622452 half_orm-0.9.2/half_orm/
+-rw-r--r--   0 joel      (1000) joel      (1000)      172 2023-02-02 08:59:25.000000 half_orm-0.9.2/half_orm/__init__.py
+-rw-r--r--   0 joel      (1000) joel      (1000)     5495 2023-05-12 08:02:28.000000 half_orm-0.9.2/half_orm/field.py
+-rw-r--r--   0 joel      (1000) joel      (1000)       70 2023-02-02 08:59:25.000000 half_orm-0.9.2/half_orm/field_errors.py
+-rw-r--r--   0 joel      (1000) joel      (1000)     5549 2023-05-31 05:53:13.000000 half_orm-0.9.2/half_orm/fkey.py
+-rw-r--r--   0 joel      (1000) joel      (1000)     3513 2023-05-12 08:00:34.000000 half_orm-0.9.2/half_orm/hotest.py
+-rwxr-xr-x   0 joel      (1000) joel      (1000)    15040 2023-05-30 06:37:38.000000 half_orm-0.9.2/half_orm/model.py
+-rw-r--r--   0 joel      (1000) joel      (1000)     1143 2023-03-21 09:29:02.000000 half_orm-0.9.2/half_orm/model_errors.py
+-rw-r--r--   0 joel      (1000) joel      (1000)      405 2023-03-18 07:38:44.000000 half_orm-0.9.2/half_orm/null.py
+drwxr-xr-x   0 joel      (1000) joel      (1000)        0 2023-06-09 07:02:18.622452 half_orm-0.9.2/half_orm/packager/
+-rw-r--r--   0 joel      (1000) joel      (1000)        0 2023-02-28 10:33:54.000000 half_orm-0.9.2/half_orm/packager/__init__.py
+-rw-r--r--   0 joel      (1000) joel      (1000)     3226 2023-06-09 06:04:05.000000 half_orm-0.9.2/half_orm/packager/api.py
+-rw-r--r--   0 joel      (1000) joel      (1000)     4166 2023-06-09 06:25:39.000000 half_orm-0.9.2/half_orm/packager/changelog.py
+-rw-r--r--   0 joel      (1000) joel      (1000)     4527 2023-05-31 05:53:13.000000 half_orm-0.9.2/half_orm/packager/database.py
+-rw-r--r--   0 joel      (1000) joel      (1000)     4643 2023-05-31 05:53:13.000000 half_orm-0.9.2/half_orm/packager/db_conn.py
+-rw-r--r--   0 joel      (1000) joel      (1000)     7513 2023-05-31 05:53:13.000000 half_orm-0.9.2/half_orm/packager/hgit.py
+-rwxr-xr-x   0 joel      (1000) joel      (1000)     5512 2023-05-31 08:02:38.000000 half_orm-0.9.2/half_orm/packager/hop.py
+-rw-r--r--   0 joel      (1000) joel      (1000)     1265 2023-05-31 05:53:13.000000 half_orm-0.9.2/half_orm/packager/manifest.py
+-rwxr-xr-x   0 joel      (1000) joel      (1000)     8821 2023-05-31 05:53:13.000000 half_orm-0.9.2/half_orm/packager/modules.py
+-rwxr-xr-x   0 joel      (1000) joel      (1000)    13380 2023-06-09 06:04:05.000000 half_orm-0.9.2/half_orm/packager/patch.py
+drwxr-xr-x   0 joel      (1000) joel      (1000)        0 2023-06-09 07:02:18.622452 half_orm-0.9.2/half_orm/packager/patches/
+drwxr-xr-x   0 joel      (1000) joel      (1000)        0 2023-06-09 07:02:18.618452 half_orm-0.9.2/half_orm/packager/patches/0/
+drwxr-xr-x   0 joel      (1000) joel      (1000)        0 2023-06-09 07:02:18.618452 half_orm-0.9.2/half_orm/packager/patches/0/1/
+drwxr-xr-x   0 joel      (1000) joel      (1000)        0 2023-06-09 07:02:18.622452 half_orm-0.9.2/half_orm/packager/patches/0/1/0/
+-rw-r--r--   0 joel      (1000) joel      (1000)     1076 2023-02-28 10:33:54.000000 half_orm-0.9.2/half_orm/packager/patches/0/1/0/00_half_orm_meta.database.sql
+-rw-r--r--   0 joel      (1000) joel      (1000)      183 2023-02-28 10:33:54.000000 half_orm-0.9.2/half_orm/packager/patches/0/1/0/01_alter_half_orm_meta.hop_release.sql
+-rw-r--r--   0 joel      (1000) joel      (1000)      306 2023-05-22 07:11:49.000000 half_orm-0.9.2/half_orm/packager/patches/0/1/0/02_half_orm_meta.view.hop_penultimate_release.sql
+-rw-r--r--   0 joel      (1000) joel      (1000)       22 2023-02-28 10:33:54.000000 half_orm-0.9.2/half_orm/packager/patches/log
+drwxr-xr-x   0 joel      (1000) joel      (1000)        0 2023-06-09 07:02:18.622452 half_orm-0.9.2/half_orm/packager/patches/sql/
+-rw-r--r--   0 joel      (1000) joel      (1000)     5864 2023-05-22 07:14:29.000000 half_orm-0.9.2/half_orm/packager/patches/sql/half_orm_meta.sql
+-rw-r--r--   0 joel      (1000) joel      (1000)     8744 2023-05-31 08:05:20.000000 half_orm-0.9.2/half_orm/packager/repo.py
+drwxr-xr-x   0 joel      (1000) joel      (1000)        0 2023-06-09 07:02:18.626452 half_orm-0.9.2/half_orm/packager/templates/
+-rw-r--r--   0 joel      (1000) joel      (1000)       86 2023-02-28 10:33:54.000000 half_orm-0.9.2/half_orm/packager/templates/.gitignore
+-rw-r--r--   0 joel      (1000) joel      (1000)       25 2023-02-28 10:33:54.000000 half_orm-0.9.2/half_orm/packager/templates/MANIFEST.in
+-rw-r--r--   0 joel      (1000) joel      (1000)      218 2023-02-28 10:33:54.000000 half_orm-0.9.2/half_orm/packager/templates/Pipfile
+-rw-r--r--   0 joel      (1000) joel      (1000)      924 2023-02-28 10:33:54.000000 half_orm-0.9.2/half_orm/packager/templates/README
+-rw-r--r--   0 joel      (1000) joel      (1000)      367 2023-02-28 10:33:54.000000 half_orm-0.9.2/half_orm/packager/templates/base_test
+-rw-r--r--   0 joel      (1000) joel      (1000)      169 2023-05-30 13:56:46.000000 half_orm-0.9.2/half_orm/packager/templates/init_module_template
+-rw-r--r--   0 joel      (1000) joel      (1000)      219 2023-05-30 13:30:44.000000 half_orm-0.9.2/half_orm/packager/templates/module_template_1
+-rw-r--r--   0 joel      (1000) joel      (1000)      108 2023-05-30 13:31:12.000000 half_orm-0.9.2/half_orm/packager/templates/module_template_2
+-rw-r--r--   0 joel      (1000) joel      (1000)       69 2023-02-28 10:33:54.000000 half_orm-0.9.2/half_orm/packager/templates/module_template_3
+-rw-r--r--   0 joel      (1000) joel      (1000)      460 2023-02-28 10:33:54.000000 half_orm-0.9.2/half_orm/packager/templates/relation_test
+-rw-r--r--   0 joel      (1000) joel      (1000)     2070 2023-02-28 10:33:54.000000 half_orm-0.9.2/half_orm/packager/templates/setup.py
+-rw-r--r--   0 joel      (1000) joel      (1000)      490 2023-02-28 10:33:54.000000 half_orm-0.9.2/half_orm/packager/templates/warning
+-rw-r--r--   0 joel      (1000) joel      (1000)        8 2023-06-09 06:35:11.000000 half_orm-0.9.2/half_orm/packager/version.txt
+-rw-r--r--   0 joel      (1000) joel      (1000)    17049 2023-04-20 09:30:05.000000 half_orm-0.9.2/half_orm/pg_meta.py
+-rw-r--r--   0 joel      (1000) joel      (1000)    39558 2023-05-31 19:18:56.000000 half_orm-0.9.2/half_orm/relation.py
+-rw-r--r--   0 joel      (1000) joel      (1000)     1520 2023-05-12 08:00:34.000000 half_orm-0.9.2/half_orm/relation_errors.py
+-rw-r--r--   0 joel      (1000) joel      (1000)     3867 2023-05-31 05:53:13.000000 half_orm-0.9.2/half_orm/relation_factory.py
+-rw-r--r--   0 joel      (1000) joel      (1000)     2743 2023-03-21 09:29:02.000000 half_orm-0.9.2/half_orm/transaction.py
+-rw-r--r--   0 joel      (1000) joel      (1000)     2135 2023-05-31 05:55:37.000000 half_orm-0.9.2/half_orm/utils.py
+-rw-r--r--   0 joel      (1000) joel      (1000)        6 2023-06-09 06:36:48.000000 half_orm-0.9.2/half_orm/version.txt
+drwxr-xr-x   0 joel      (1000) joel      (1000)        0 2023-06-09 07:02:18.622452 half_orm-0.9.2/half_orm.egg-info/
+-rw-r--r--   0 joel      (1000) joel      (1000)    27277 2023-06-09 07:02:18.000000 half_orm-0.9.2/half_orm.egg-info/PKG-INFO
+-rw-r--r--   0 joel      (1000) joel      (1000)     1685 2023-06-09 07:02:18.000000 half_orm-0.9.2/half_orm.egg-info/SOURCES.txt
+-rw-r--r--   0 joel      (1000) joel      (1000)        1 2023-06-09 07:02:18.000000 half_orm-0.9.2/half_orm.egg-info/dependency_links.txt
+-rw-r--r--   0 joel      (1000) joel      (1000)       51 2023-06-09 07:02:18.000000 half_orm-0.9.2/half_orm.egg-info/entry_points.txt
+-rw-r--r--   0 joel      (1000) joel      (1000)       46 2023-06-09 07:02:18.000000 half_orm-0.9.2/half_orm.egg-info/requires.txt
+-rw-r--r--   0 joel      (1000) joel      (1000)       27 2023-06-09 07:02:18.000000 half_orm-0.9.2/half_orm.egg-info/top_level.txt
+-rw-r--r--   0 joel      (1000) joel      (1000)      100 2023-01-04 14:18:53.000000 half_orm-0.9.2/pyproject.toml
+-rw-r--r--   0 joel      (1000) joel      (1000)       38 2023-06-09 07:02:18.626452 half_orm-0.9.2/setup.cfg
+-rw-r--r--   0 joel      (1000) joel      (1000)     2502 2023-03-06 08:18:37.000000 half_orm-0.9.2/setup.py
```

### Comparing `half_orm-0.9.1/LICENSE` & `half_orm-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `half_orm-0.9.1/PKG-INFO` & `half_orm-0.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: half_orm
-Version: 0.9.1
+Version: 0.9.2
 Summary: A simple PostgreSQL to Python mapper.
 Home-page: https://github.com/collorg/halfORM
 Author: Joël Maïzi
 Author-email: joel.maizi@collorg.org
 License: GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: OS Independent
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS
 
-# A simple PostgreSQL to Python mapper [0.9.1] and its packager [0.1.0a3]
+# A simple PostgreSQL to Python mapper [0.9.2] and its packager [0.1.0a4]
 
 ![PyPI version](https://img.shields.io/pypi/v/half_orm)
 ![Python versions](https://img.shields.io/badge/Python-%20&ge;%203.7-blue)
 ![PostgreSQL versions](https://img.shields.io/badge/PostgreSQL-%20&ge;%209.6-blue)
 ![CI badge](https://github.com/collorg/halfORM/actions/workflows/python-package.yml/badge.svg)
 ![Coveralls](https://img.shields.io/coverallsCoverage/github/collorg/halfORM)
 ![PyPI downloads](https://img.shields.io/pypi/dm/half_orm)
@@ -186,17 +186,18 @@
 
 To get a full description of the corresponding relation, print an instance of the class:
 
 ```python
 >>> print(Person())
 ```
 ```
-__RCLS: <class 'half_orm.relation.Table_HalftestActorPerson'>
-This class allows you to manipulate the data in the PG relation:
-TABLE: "halftest":"actor"."person"
+DATABASE: halftest
+SCHEMA: actor
+TABLE: person
+
 DESCRIPTION:
 The table actor.person contains the persons of the blogging system.
 The id attribute is a serial. Just pass first_name, last_name and birth_date
 to insert a new person.
 FIELDS:
 - id:         (int4) NOT NULL
 - first_name: (text) NOT NULL
@@ -576,15 +577,16 @@
 ```python
 >>> class Post(halftest.get_relation_class('blog.post')):
 ...     pass
 ...
 >>> Post()
 ```
 ```
-__RCLS: <class '__main__.Post'>
+Inherits: <class '__main__.Post'>
+
 This class allows you to manipulate the data in the PG relation:
 TABLE: "halftest":"blog"."post"
 DESCRIPTION:
 The table blog.post contains all the post
 made by a person in the blogging system.
 FIELDS:
 - id:                (int4) NOT NULL
```

### Comparing `half_orm-0.9.1/README.md` & `half_orm-0.9.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# A simple PostgreSQL to Python mapper [0.9.1] and its packager [0.1.0a3]
+# A simple PostgreSQL to Python mapper [0.9.2] and its packager [0.1.0a4]
 
 ![PyPI version](https://img.shields.io/pypi/v/half_orm)
 ![Python versions](https://img.shields.io/badge/Python-%20&ge;%203.7-blue)
 ![PostgreSQL versions](https://img.shields.io/badge/PostgreSQL-%20&ge;%209.6-blue)
 ![CI badge](https://github.com/collorg/halfORM/actions/workflows/python-package.yml/badge.svg)
 ![Coveralls](https://img.shields.io/coverallsCoverage/github/collorg/halfORM)
 ![PyPI downloads](https://img.shields.io/pypi/dm/half_orm)
@@ -162,17 +162,18 @@
 
 To get a full description of the corresponding relation, print an instance of the class:
 
 ```python
 >>> print(Person())
 ```
 ```
-__RCLS: <class 'half_orm.relation.Table_HalftestActorPerson'>
-This class allows you to manipulate the data in the PG relation:
-TABLE: "halftest":"actor"."person"
+DATABASE: halftest
+SCHEMA: actor
+TABLE: person
+
 DESCRIPTION:
 The table actor.person contains the persons of the blogging system.
 The id attribute is a serial. Just pass first_name, last_name and birth_date
 to insert a new person.
 FIELDS:
 - id:         (int4) NOT NULL
 - first_name: (text) NOT NULL
@@ -552,15 +553,16 @@
 ```python
 >>> class Post(halftest.get_relation_class('blog.post')):
 ...     pass
 ...
 >>> Post()
 ```
 ```
-__RCLS: <class '__main__.Post'>
+Inherits: <class '__main__.Post'>
+
 This class allows you to manipulate the data in the PG relation:
 TABLE: "halftest":"blog"."post"
 DESCRIPTION:
 The table blog.post contains all the post
 made by a person in the blogging system.
 FIELDS:
 - id:                (int4) NOT NULL
```

### Comparing `half_orm-0.9.1/half_orm/field.py` & `half_orm-0.9.2/half_orm/field.py`

 * *Files identical despite different names*

### Comparing `half_orm-0.9.1/half_orm/fkey.py` & `half_orm-0.9.2/half_orm/fkey.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 # pylint: disable=protected-access
 
 """This module provides the FKey class."""
 
 from half_orm.pg_meta import normalize_fqrn, normalize_qrn
-from half_orm.packager import utils
+from half_orm import utils
 
 class FKey:
     """Foreign key class
 
     A foreign key is set by assigning to it a Relation object of the
     corresponding type (see FKey.set method).
     It is then used to construct the join query for Relation.ho_select
```

### Comparing `half_orm-0.9.1/half_orm/hotest.py` & `half_orm-0.9.2/half_orm/hotest.py`

 * *Files identical despite different names*

### Comparing `half_orm-0.9.1/half_orm/model.py` & `half_orm-0.9.2/half_orm/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     ...     # Your business code goes here
 
 Note:
     The default schema is ``public`` in PostgreSQL, so to reference a table
     ``my_table`` in this schema you'll have to use ``pubic.my_table``.
 """
 
-
+import importlib
 import os
 import sys
 from configparser import ConfigParser
 from os import environ
 from typing import List
 
 import psycopg2
@@ -375,7 +375,21 @@
             >>> halftest.desc()
             [('r', ('halftest', 'actor', 'person'), []), ('r', ('halftest', 'blog', 'comment'), []), ('r', ('halftest', 'blog', 'event'), [('halftest', 'blog', 'post')]), ('r', ('halftest', 'blog', 'post'), []), ('v', ('halftest', 'blog.view', 'post_comment'), [])]
         """
         return self.__pg_meta.desc(self.__dbname)
 
     def __str__(self):
         return self.__pg_meta.str(self.__dbname)
+
+    def classes(self):
+        "Returns the all the classes of the model"
+        for relation in self._relations():
+            package_name = relation[1][0]
+            module_name = ".".join(relation[1][1:])
+            if module_name.find('half_orm_meta') == 0:
+                continue
+            class_name = pg_meta.camel_case(relation[1][-1])
+            try:
+                module = importlib.import_module(f".{module_name}", package_name)
+            except ModuleNotFoundError as err:
+                raise err
+            yield getattr(module, class_name), relation[0]
```

### Comparing `half_orm-0.9.1/half_orm/model_errors.py` & `half_orm-0.9.2/half_orm/model_errors.py`

 * *Files identical despite different names*

### Comparing `half_orm-0.9.1/half_orm/packager/changelog.py` & `half_orm-0.9.2/half_orm/packager/changelog.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
   preparation.
 * previous commit is the last commit on hop_main before the rebase of hop_<release>
 
 """
 
 import os
 
-from half_orm.packager import utils
+from half_orm import utils
 
 class Changelog:
     "The Changelog class..."
     __log_list = []
     __log_dict = {}
     __releases = []
     def __init__(self, repo):
@@ -32,19 +32,29 @@
         self.__seq()
 
     def __seq(self):
         self.__log_list = [elt.strip('\n').split('\t') for elt in utils.readlines(self.__file)]
         self.__log_dict = {elt[1]: elt for elt in self.__log_list}
         self.__releases = list(self.__log_dict.keys())
 
+    @staticmethod
+    def _sort_releases(releases):
+        "Sort the releases"
+        int_releases = list([tuple(int(elt) for elt in release.split('.'))
+            for release in releases])
+        int_releases.sort()
+        releases = list([".".join(str(elt) for elt in release)
+            for release in int_releases])
+        return releases
+
     def new_release(self, release):
         """Update with the release the .hop/CHANGELOG file"""
         releases = self.__releases
         releases.append(release)
-        releases.sort()
+        releases = Changelog._sort_releases(releases)
         utils.write(self.__file, '')
         for elt in releases:
             rel = self.__log_dict.get(elt)
             if rel:
                 utils.write(self.__file, f'{rel[0]}\t{rel[1]}\t{rel[2]}\t{rel[3]}\n', mode='a+')
             else:
                 utils.write(self.__file, f'{utils.hop_version()}\t{release}\t\t\n', mode='a+')
```

### Comparing `half_orm-0.9.1/half_orm/packager/database.py` & `half_orm-0.9.2/half_orm/packager/database.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import os
 import subprocess
 import sys
 
 from psycopg2 import OperationalError
 from half_orm.model import Model
 from half_orm.model_errors import UnknownRelation
-from half_orm.packager import utils
+from half_orm import utils
 from half_orm.packager.db_conn import DbConn
 
 
 class Database:
     """Reads and writes the halfORM connection file
     """
```

### Comparing `half_orm-0.9.1/half_orm/packager/db_conn.py` & `half_orm-0.9.2/half_orm/packager/db_conn.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import subprocess
 import sys
 
 from getpass import getpass
 from configparser import ConfigParser
 
 from half_orm.model import CONF_DIR
-from half_orm.packager import utils
+from half_orm import utils
 
 CONF_NOT_FOUND = '''
 The configuration file {} is missing.
 You must create it before proceeding.
 
 '''
```

### Comparing `half_orm-0.9.1/half_orm/packager/hgit.py` & `half_orm-0.9.2/half_orm/packager/hgit.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import os
 import sys
 import subprocess
 from git import Repo
 from git.exc import GitCommandError
 
-from half_orm.packager import utils
+from half_orm import utils
 from half_orm.packager.manifest import Manifest
 
 class HGit:
     "Manages the git operations on the repo."
     def __init__(self, repo=None):
         self.__origin = None
         self.__repo = repo
```

### Comparing `half_orm-0.9.1/half_orm/packager/hop.py` & `half_orm-0.9.2/half_orm/packager/hop.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,33 +20,33 @@
 """
 
 import sys
 
 import click
 
 from half_orm.packager.repo import Repo
-from half_orm.packager import utils
+from half_orm import utils
 
 class Hop:
     "Sets the options available to the hop command"
     __available_cmds = []
     __command = None
     def __init__(self):
         self.__repo: Repo = Repo()
         if not self.repo_checked:
             Hop.__available_cmds = ['new']
         else:
             if not self.__repo.devel:
-                Hop.__available_cmds = ['sync-package']
+                Hop.__available_cmds = ['sync-package', 'gen-api']
             else:
                 if not self.__repo.production and self.__repo:
                     if self.__repo.hgit.branch == 'hop_main':
-                        Hop.__available_cmds = ['prepare']
+                        Hop.__available_cmds = ['prepare', 'gen-api']
                     elif self.__repo.hgit.is_hop_patch_branch:
-                        Hop.__available_cmds = ['apply', 'undo', 'release']
+                        Hop.__available_cmds = ['apply', 'undo', 'release', 'gen-api']
                 elif self:
                     Hop.__available_cmds = ['upgrade', 'restore']
 
     @property
     def repo_checked(self):
         "Returns wether we are in a repo or not."
         return self.__repo.checked
@@ -128,21 +128,26 @@
         def release(push=False):
             self.__repo.commit_release(push)
 
         @click.command()
         def sync_package():
             self.__repo.sync_package()
 
+        @click.command()
+        def gen_api():
+            self.__repo.gen_api()
+
         cmds = {
             'new': new,
             'prepare': prepare,
             'apply': apply,
             'undo': undo,
             'release': release,
             'sync-package': sync_package,
+            'gen-api': gen_api,
             'upgrade': upgrade,
             'restore': restore
         }
 
         for cmd in self.__available_cmds:
             click_main.add_command(cmds[cmd])
```

### Comparing `half_orm-0.9.1/half_orm/packager/manifest.py` & `half_orm-0.9.2/half_orm/packager/manifest.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Manages the MANIFEST.json
 """
 
 import json
 import os
 
-from half_orm.packager import utils
+from half_orm import utils
 
 class Manifest:
     "Manages the manifest of a release"
     def __init__(self, path):
         self.__hop_version = None
         self.__changelog_msg = None
         self.__file = os.path.join(path, 'MANIFEST.json')
```

### Comparing `half_orm-0.9.1/half_orm/packager/modules.py` & `half_orm-0.9.2/half_orm/packager/modules.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,22 +23,22 @@
 import os
 import sys
 from keyword import iskeyword
 
 from half_orm.pg_meta import camel_case
 from half_orm.model_errors import UnknownRelation
 
-from half_orm.packager import utils
+from half_orm import utils
 
 def read_template(file_name):
     "helper"
     with open(os.path.join(utils.TEMPLATE_DIRS, file_name), encoding='utf-8') as file_:
         return file_.read()
 
-DB_CONNECTOR_TEMPLATE = read_template('db_connector.py')
+INIT_MODULE_TEMPLATE = read_template('init_module_template')
 MODULE_TEMPLATE_1 = read_template('module_template_1')
 MODULE_TEMPLATE_2 = read_template('module_template_2')
 MODULE_TEMPLATE_3 = read_template('module_template_3')
 # FKEYS_PROPS = read_template('fkeys_properties')
 WARNING_TEMPLATE = read_template('warning')
 BASE_TEST = read_template('base_test')
 TEST = read_template('relation_test')
@@ -47,32 +47,32 @@
     "{rt1}" +
     "{bc_}{global_user_s_code}{ec_}" +
     "{rt2}" +
     "    {bc_}{user_s_class_attr}    {ec_}" +
     "{rt3}\n        " +
     "{bc_}{user_s_code}")
 AP_EPILOG = """"""
-DO_NOT_REMOVE = ['db_connector.py', '__init__.py', 'base_test.py']
+DO_NOT_REMOVE = ['__init__.py', 'base_test.py']
 
 MODEL = None
 
 def __update_init_files(package_dir, files_list, warning):
     """Update __all__ lists in __init__ files.
     """
     skip = re.compile('[A-Z]')
     for root, dirs, files in os.walk(package_dir):
+        if root == package_dir:
+            continue
         all_ = []
         reldir = root.replace(package_dir, '')
         if re.findall(skip, reldir):
             continue
         for dir_ in dirs:
             if re.findall(skip, dir_):
                 continue
-            if dir_ != '__pycache__':
-                all_.append(dir_)
         for file_ in files:
             if re.findall(skip, file_):
                 continue
             path_ = os.path.join(root, file_)
             if path_ not in files_list and file_ not in DO_NOT_REMOVE:
                 if path_.find('__pycache__') == -1 and path_.find('_test.py') == -1:
                     print(f"REMOVING: {path_}")
@@ -81,15 +81,15 @@
             if (re.findall('.py$', file_) and
                     file_ != '__init__.py' and
                     file_ != '__pycache__' and
                     file_.find('_test.py') == -1):
                 all_.append(file_.replace('.py', ''))
         all_.sort()
         with open(os.path.join(root, '__init__.py'), 'w', encoding='utf-8') as init_file:
-            init_file.write(f'"""{warning}"""\n\n')
+            init_file.write(f'"""{root}\n{warning}"""\n\n')
 
             all_ = ",\n    ".join([f"'{elt}'" for elt in all_])
             init_file.write(f'__all__ = [\n    {all_}\n]\n')
 
 def __get_inheritance_info(rel, package_name):
     """Returns inheritance informations for the rel relation.
     """
@@ -191,16 +191,16 @@
     """
     package_name = repo.name
     package_dir = os.path.join(repo.base_dir, package_name)
     files_list = []
     repo.database.model._reload()
     if not os.path.exists(package_dir):
         os.mkdir(package_dir)
-    with open(os.path.join(package_dir, 'db_connector.py'), 'w', encoding='utf-8') as file_:
-        file_.write(DB_CONNECTOR_TEMPLATE.format(dbname=package_name, package_name=package_name))
+    with open(os.path.join(package_dir, '__init__.py'), 'w', encoding='utf-8') as file_:
+        file_.write(INIT_MODULE_TEMPLATE.format(package_name=package_name))
 
     if not os.path.exists(os.path.join(package_dir, 'base_test.py')):
         with open(os.path.join(package_dir, 'base_test.py'), 'w', encoding='utf-8') as file_:
             file_.write(BASE_TEST.format(
                 BEGIN_CODE=utils.BEGIN_CODE,
                 END_CODE=utils.END_CODE,
                 package_name=package_name))
```

### Comparing `half_orm-0.9.1/half_orm/packager/patch.py` & `half_orm-0.9.2/half_orm/packager/patch.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import os
 import subprocess
 import sys
 
 import pydash
 import psycopg2
 
-from half_orm.packager import utils
+from half_orm import utils
 from half_orm.packager import modules
 from half_orm.packager.changelog import Changelog
 
 try:
     PYTEST_OK = True
     import pytest
 except ImportError:
```

### Comparing `half_orm-0.9.1/half_orm/packager/patches/0/1/0/00_half_orm_meta.database.sql` & `half_orm-0.9.2/half_orm/packager/patches/0/1/0/00_half_orm_meta.database.sql`

 * *Files identical despite different names*

### Comparing `half_orm-0.9.1/half_orm/packager/patches/sql/half_orm_meta.sql` & `half_orm-0.9.2/half_orm/packager/patches/sql/half_orm_meta.sql`

 * *Files identical despite different names*

### Comparing `half_orm-0.9.1/half_orm/packager/repo.py` & `half_orm-0.9.2/half_orm/packager/repo.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 """The pkg_conf module provides the Repo class.
 """
 
 import os
 from configparser import ConfigParser
 import half_orm
-from half_orm.packager import utils
+from half_orm import utils
 from half_orm.packager.database import Database
 from half_orm.packager.hgit import HGit
 from half_orm.packager import modules
 from half_orm.packager.patch import Patch
 from half_orm.packager.changelog import Changelog
+from half_orm.packager.api import Api
 
 class Config:
     """
     """
     __name: str = None
     __git_origin: str = ''
     __devel: bool = False
@@ -251,7 +252,11 @@
     def undo_release(self, database_only=False):
         "Undo the current release (devel)"
         Patch(self).undo(database_only=database_only)
 
     def commit_release(self, push):
         "Release a 'release' (devel)"
         Patch(self).release(push)
+
+    def gen_api(self):
+        "Generates the API for the package"
+        Api(self).generate()
```

### Comparing `half_orm-0.9.1/half_orm/packager/templates/README` & `half_orm-0.9.2/half_orm/packager/templates/README`

 * *Files identical despite different names*

### Comparing `half_orm-0.9.1/half_orm/packager/templates/setup.py` & `half_orm-0.9.2/half_orm/packager/templates/setup.py`

 * *Files identical despite different names*

### Comparing `half_orm-0.9.1/half_orm/packager/utils.py` & `half_orm-0.9.2/half_orm/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,16 @@
         "blue"
         return f"\033[1;34m{text}\033[0m"
     @staticmethod
     def bold(text):
         "bold"
         return f"\033[1m{text}\033[0m"
 
-HOP_PATH = os.path.dirname(__file__)
+PWD = os.path.dirname(__file__)
+HOP_PATH = os.path.join(PWD, 'packager')
 TEMPLATE_DIRS = os.path.join(HOP_PATH, 'templates')
 
 BEGIN_CODE = "#>>> PLACE YOUR CODE BELOW THIS LINE. DO NOT REMOVE THIS LINE!\n"
 END_CODE = "#<<< PLACE YOUR CODE ABOVE THIS LINE. DO NOT REMOVE THIS LINE!\n"
 
 def read(file_):
     "Read file helper"
```

### Comparing `half_orm-0.9.1/half_orm/pg_meta.py` & `half_orm-0.9.2/half_orm/pg_meta.py`

 * *Files identical despite different names*

### Comparing `half_orm-0.9.1/half_orm/relation.py` & `half_orm-0.9.2/half_orm/relation.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 
 
 import yaml
 
 from half_orm import relation_errors
 from half_orm.transaction import Transaction
 from half_orm.field import Field
-from half_orm.packager import utils
+from half_orm import utils
 
 class _SetOperators:
     """_SetOperators class stores the set operations made on the Relation class objects
 
     - __operator is one of {'or', 'and', 'sub', 'neg'}
     - __right is a Relation object. It can be None if the operator is 'neg'.
     """
@@ -533,18 +533,18 @@
 want to use. The aliases must be unique and different from any of the column names. Empty
 string keys are ignored.
 
 Fkeys = {"""
 
     rel_kind = self.__kind
     ret = []
-    ret.append(f"__RCLS: {self.__class__}")
-    ret.append(
-        "This class allows you to manipulate the data in the PG relation:")
-    ret.append(f"{rel_kind.upper()}: {self._fqrn}")
+    database, schema, relation = self._t_fqrn
+    ret.append(f"DATABASE: {database}")
+    ret.append(f"SCHEMA: {schema}")
+    ret.append(f"{rel_kind.upper()}: {relation}\n")
     if self.__metadata['description']:
         ret.append(f"DESCRIPTION:\n{self.__metadata['description']}")
     ret.append('FIELDS:')
     mx_fld_n_len = 0
     for field_name in self._ho_fields.keys():
         if len(field_name) > mx_fld_n_len:
             mx_fld_n_len = len(field_name)
@@ -799,14 +799,23 @@
         if fk_prep_select is not None:
             fk_values += list(fkey.values()[0])
             fk_fields += fk_prep_select[0]
             fk_queries = ["%s" for _ in range(len(fk_values))]
 
     return fields_names, set_fields, fk_fields, fk_queries, fk_values
 
+@classmethod
+def ho_description(self):
+    """Returns the description (comment) of the relation
+    """
+    description = self.__metadata['description']
+    if description:
+        description = description.strip()
+    return description or 'No description available'
+
 def __call__(self, **kwargs):
     return self.__class__(**kwargs)
 
 def ho_cast(self, qrn):
     """Cast a relation into another relation.
 
     TODO: check that qrn inherits self (or is inherited by self)?
@@ -1071,14 +1080,15 @@
     # protected methods
     'ho_freeze': ho_freeze,
     'ho_unfreeze': ho_unfreeze,
     'ho_prep_select': ho_prep_select,
     'ho_mogrify': ho_mogrify,
 
     # public methods
+    'ho_description': ho_description,
     'ho_id': ho_id,
     'ho_order_by': ho_order_by,
     'ho_limit': ho_limit,
     'ho_offset': ho_offset,
     'ho_distinct': ho_distinct,
     'ho_unaccent': ho_unaccent,
     'ho_cast': ho_cast,
```

### Comparing `half_orm-0.9.1/half_orm/relation_errors.py` & `half_orm-0.9.2/half_orm/relation_errors.py`

 * *Files identical despite different names*

### Comparing `half_orm-0.9.1/half_orm/relation_factory.py` & `half_orm-0.9.2/half_orm/relation_factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import sys
 import inspect
 from functools import wraps
 
 from half_orm import pg_meta
 from half_orm import model_errors
-from half_orm.packager import utils
+from half_orm import utils
 from half_orm.relation import Relation, REL_INTERFACES, REL_CLASS_NAMES
 
 def __deprecated(fct):
     @wraps(fct)
     def wrapper(self, *args, **kwargs):
         name = fct.__name__
         dep_name = name.replace('ho_', '')
```

### Comparing `half_orm-0.9.1/half_orm/transaction.py` & `half_orm-0.9.2/half_orm/transaction.py`

 * *Files identical despite different names*

### Comparing `half_orm-0.9.1/half_orm.egg-info/PKG-INFO` & `half_orm-0.9.2/half_orm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: half-orm
-Version: 0.9.1
+Version: 0.9.2
 Summary: A simple PostgreSQL to Python mapper.
 Home-page: https://github.com/collorg/halfORM
 Author: Joël Maïzi
 Author-email: joel.maizi@collorg.org
 License: GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: OS Independent
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS
 
-# A simple PostgreSQL to Python mapper [0.9.1] and its packager [0.1.0a3]
+# A simple PostgreSQL to Python mapper [0.9.2] and its packager [0.1.0a4]
 
 ![PyPI version](https://img.shields.io/pypi/v/half_orm)
 ![Python versions](https://img.shields.io/badge/Python-%20&ge;%203.7-blue)
 ![PostgreSQL versions](https://img.shields.io/badge/PostgreSQL-%20&ge;%209.6-blue)
 ![CI badge](https://github.com/collorg/halfORM/actions/workflows/python-package.yml/badge.svg)
 ![Coveralls](https://img.shields.io/coverallsCoverage/github/collorg/halfORM)
 ![PyPI downloads](https://img.shields.io/pypi/dm/half_orm)
@@ -186,17 +186,18 @@
 
 To get a full description of the corresponding relation, print an instance of the class:
 
 ```python
 >>> print(Person())
 ```
 ```
-__RCLS: <class 'half_orm.relation.Table_HalftestActorPerson'>
-This class allows you to manipulate the data in the PG relation:
-TABLE: "halftest":"actor"."person"
+DATABASE: halftest
+SCHEMA: actor
+TABLE: person
+
 DESCRIPTION:
 The table actor.person contains the persons of the blogging system.
 The id attribute is a serial. Just pass first_name, last_name and birth_date
 to insert a new person.
 FIELDS:
 - id:         (int4) NOT NULL
 - first_name: (text) NOT NULL
@@ -576,15 +577,16 @@
 ```python
 >>> class Post(halftest.get_relation_class('blog.post')):
 ...     pass
 ...
 >>> Post()
 ```
 ```
-__RCLS: <class '__main__.Post'>
+Inherits: <class '__main__.Post'>
+
 This class allows you to manipulate the data in the PG relation:
 TABLE: "halftest":"blog"."post"
 DESCRIPTION:
 The table blog.post contains all the post
 made by a person in the blogging system.
 FIELDS:
 - id:                (int4) NOT NULL
```

### Comparing `half_orm-0.9.1/half_orm.egg-info/SOURCES.txt` & `half_orm-0.9.2/half_orm.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -12,43 +12,44 @@
 half_orm/model_errors.py
 half_orm/null.py
 half_orm/pg_meta.py
 half_orm/relation.py
 half_orm/relation_errors.py
 half_orm/relation_factory.py
 half_orm/transaction.py
+half_orm/utils.py
 half_orm/version.txt
 half_orm.egg-info/PKG-INFO
 half_orm.egg-info/SOURCES.txt
 half_orm.egg-info/dependency_links.txt
 half_orm.egg-info/entry_points.txt
 half_orm.egg-info/requires.txt
 half_orm.egg-info/top_level.txt
 half_orm/packager/__init__.py
+half_orm/packager/api.py
 half_orm/packager/changelog.py
 half_orm/packager/database.py
 half_orm/packager/db_conn.py
 half_orm/packager/hgit.py
 half_orm/packager/hop.py
 half_orm/packager/manifest.py
 half_orm/packager/modules.py
 half_orm/packager/patch.py
 half_orm/packager/repo.py
-half_orm/packager/utils.py
 half_orm/packager/version.txt
 half_orm/packager/patches/log
 half_orm/packager/patches/0/1/0/00_half_orm_meta.database.sql
 half_orm/packager/patches/0/1/0/01_alter_half_orm_meta.hop_release.sql
 half_orm/packager/patches/0/1/0/02_half_orm_meta.view.hop_penultimate_release.sql
 half_orm/packager/patches/sql/half_orm_meta.sql
 half_orm/packager/templates/.gitignore
 half_orm/packager/templates/MANIFEST.in
 half_orm/packager/templates/Pipfile
 half_orm/packager/templates/README
 half_orm/packager/templates/base_test
-half_orm/packager/templates/db_connector.py
+half_orm/packager/templates/init_module_template
 half_orm/packager/templates/module_template_1
 half_orm/packager/templates/module_template_2
 half_orm/packager/templates/module_template_3
 half_orm/packager/templates/relation_test
 half_orm/packager/templates/setup.py
 half_orm/packager/templates/warning
```

### Comparing `half_orm-0.9.1/setup.py` & `half_orm-0.9.2/setup.py`

 * *Files identical despite different names*

