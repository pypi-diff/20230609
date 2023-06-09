# Comparing `tmp/lamindb_setup-0.47.0.tar.gz` & `tmp/lamindb_setup-0.47.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lamindb_setup-0.47.0.tar", last modified: Thu Jun  8 17:53:03 2023, max compression
+gzip compressed data, was "lamindb_setup-0.47.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `lamindb_setup-0.47.0.tar` & `lamindb_setup-0.47.1.tar`

### file list

```diff
@@ -1,91 +1,91 @@
--rw-r--r--   0        0        0     4010 2023-06-04 10:03:32.188588 lamindb_setup-0.47.0/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2023-05-26 12:29:21.559431 lamindb_setup-0.47.0/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2023-05-26 12:29:21.559519 lamindb_setup-0.47.0/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1204 2023-05-26 12:29:21.559614 lamindb_setup-0.47.0/.gitignore
--rw-r--r--   0        0        0      100 2023-05-31 13:45:54.309833 lamindb_setup-0.47.0/.gitmodules
--rw-r--r--   0        0        0     1798 2023-06-04 10:03:32.189000 lamindb_setup-0.47.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11324 2023-05-26 12:29:21.559824 lamindb_setup-0.47.0/LICENSE
--rw-r--r--   0        0        0      318 2023-06-04 10:03:32.189263 lamindb_setup-0.47.0/README.md
--rw-r--r--   0        0        0    53189 2023-06-08 17:52:33.789547 lamindb_setup-0.47.0/docs/changelog.md
--rw-r--r--   0        0        0     6341 2023-06-04 20:49:27.327815 lamindb_setup-0.47.0/docs/faq/edge-cases-login-init.ipynb
--rw-r--r--   0        0        0       96 2023-06-04 10:03:32.190096 lamindb_setup-0.47.0/docs/faq/index.md
--rw-r--r--   0        0        0     3323 2023-06-01 11:33:10.499233 lamindb_setup-0.47.0/docs/faq/switch-environment.ipynb
--rw-r--r--   0        0        0     6590 2023-06-07 14:57:12.963250 lamindb_setup-0.47.0/docs/faq/test-sqlite-sync.ipynb
--rw-r--r--   0        0        0     8164 2023-06-08 11:34:59.766816 lamindb_setup-0.47.0/docs/guide/01-init-instance.ipynb
--rw-r--r--   0        0        0     4362 2023-06-08 11:34:59.766951 lamindb_setup-0.47.0/docs/guide/02-load-instance.ipynb
--rw-r--r--   0        0        0     5750 2023-06-08 11:34:59.767059 lamindb_setup-0.47.0/docs/guide/03-set-storage.ipynb
--rw-r--r--   0        0        0     2975 2023-06-08 11:34:59.767166 lamindb_setup-0.47.0/docs/guide/04-schema-modules.ipynb
--rw-r--r--   0        0        0      114 2023-06-08 16:08:38.507384 lamindb_setup-0.47.0/docs/guide/index.md
--rw-r--r--   0        0        0      409 2023-06-08 16:11:46.528420 lamindb_setup-0.47.0/docs/guide/migrate.md
--rw-r--r--   0        0        0     1250 2023-06-08 11:34:59.767355 lamindb_setup-0.47.0/docs/guide/setup-user.md
--rw-r--r--   0        0        0      132 2023-06-08 11:34:59.767485 lamindb_setup-0.47.0/docs/index.md
--rw-r--r--   0        0        0       61 2023-06-08 11:34:59.767572 lamindb_setup-0.47.0/docs/reference.md
--rw-r--r--   0        0        0      365 2023-05-31 19:23:44.384942 lamindb_setup-0.47.0/docs/test_notebooks.py
--rw-r--r--   0        0        0      142 2023-06-04 07:52:11.614112 lamindb_setup-0.47.0/lamin-project.yaml
--rw-r--r--   0        0        0     2636 2023-06-08 17:52:21.065655 lamindb_setup-0.47.0/lamindb_setup/__init__.py
--rw-r--r--   0        0        0     5346 2023-06-08 07:33:18.804610 lamindb_setup-0.47.0/lamindb_setup/__main__.py
--rw-r--r--   0        0        0     1410 2023-06-05 07:31:40.592921 lamindb_setup-0.47.0/lamindb_setup/_check_instance_setup.py
--rw-r--r--   0        0        0      621 2023-06-07 14:57:12.963402 lamindb_setup-0.47.0/lamindb_setup/_close.py
--rw-r--r--   0        0        0     2006 2023-06-07 14:57:12.963567 lamindb_setup-0.47.0/lamindb_setup/_delete.py
--rw-r--r--   0        0        0      585 2023-06-04 19:41:00.163095 lamindb_setup-0.47.0/lamindb_setup/_docstrings.py
--rw-r--r--   0        0        0      329 2023-06-04 20:17:47.260552 lamindb_setup-0.47.0/lamindb_setup/_info.py
--rw-r--r--   0        0        0     6893 2023-06-08 07:33:18.804789 lamindb_setup-0.47.0/lamindb_setup/_init_instance.py
--rw-r--r--   0        0        0     5411 2023-06-08 07:33:18.805186 lamindb_setup-0.47.0/lamindb_setup/_load_instance.py
--rw-r--r--   0        0        0      322 2023-06-04 10:03:32.191280 lamindb_setup-0.47.0/lamindb_setup/_migrate.py
--rw-r--r--   0        0        0     1692 2023-06-03 14:40:15.909532 lamindb_setup-0.47.0/lamindb_setup/_notebook.py
--rw-r--r--   0        0        0      825 2023-06-04 19:41:00.163739 lamindb_setup-0.47.0/lamindb_setup/_register_instance.py
--rw-r--r--   0        0        0     1057 2023-06-04 19:41:00.163987 lamindb_setup-0.47.0/lamindb_setup/_schema.py
--rw-r--r--   0        0        0     1891 2023-06-08 07:33:18.805466 lamindb_setup-0.47.0/lamindb_setup/_set.py
--rw-r--r--   0        0        0     2247 2023-06-04 20:17:47.260720 lamindb_setup-0.47.0/lamindb_setup/_settings.py
--rw-r--r--   0        0        0       87 2023-06-01 11:33:10.504660 lamindb_setup-0.47.0/lamindb_setup/_settings_load.py
--rw-r--r--   0        0        0       72 2023-06-01 11:33:10.504736 lamindb_setup-0.47.0/lamindb_setup/_settings_store.py
--rw-r--r--   0        0        0     3548 2023-06-04 19:41:00.164398 lamindb_setup-0.47.0/lamindb_setup/_setup_user.py
--rw-r--r--   0        0        0      785 2023-06-04 19:41:00.164608 lamindb_setup-0.47.0/lamindb_setup/_silence_loggers.py
--rw-r--r--   0        0        0      456 2023-06-04 20:17:47.260896 lamindb_setup-0.47.0/lamindb_setup/dev/__init__.py
--rw-r--r--   0        0        0     5385 2023-06-07 16:31:43.467470 lamindb_setup-0.47.0/lamindb_setup/dev/_cloud_sqlite_locker.py
--rw-r--r--   0        0        0     2491 2023-06-01 11:33:10.505290 lamindb_setup-0.47.0/lamindb_setup/dev/_deprecated.py
--rw-r--r--   0        0        0     2905 2023-06-08 17:51:53.348987 lamindb_setup-0.47.0/lamindb_setup/dev/_django.py
--rw-r--r--   0        0        0      240 2023-06-01 11:33:10.505462 lamindb_setup-0.47.0/lamindb_setup/dev/_docs.py
--rw-r--r--   0        0        0     9315 2023-06-08 17:51:53.349226 lamindb_setup-0.47.0/lamindb_setup/dev/_settings_instance.py
--rw-r--r--   0        0        0     2597 2023-06-01 11:33:10.505847 lamindb_setup-0.47.0/lamindb_setup/dev/_settings_load.py
--rw-r--r--   0        0        0     2061 2023-06-01 11:33:10.505931 lamindb_setup-0.47.0/lamindb_setup/dev/_settings_save.py
--rw-r--r--   0        0        0     2318 2023-06-04 20:49:27.328010 lamindb_setup-0.47.0/lamindb_setup/dev/_settings_store.py
--rw-r--r--   0        0        0     1088 2023-06-01 11:33:10.506112 lamindb_setup-0.47.0/lamindb_setup/dev/_settings_user.py
--rw-r--r--   0        0        0     1839 2023-06-08 07:33:18.805617 lamindb_setup-0.47.0/lamindb_setup/dev/_setup_bionty_sources.py
--rw-r--r--   0        0        0     2140 2023-06-05 07:31:40.593368 lamindb_setup-0.47.0/lamindb_setup/dev/_setup_schema.py
--rw-r--r--   0        0        0     5057 2023-06-04 11:49:29.989719 lamindb_setup-0.47.0/lamindb_setup/dev/_storage.py
--rw-r--r--   0        0        0     2670 2023-06-08 17:51:53.349359 lamindb_setup-0.47.0/lamindb_setup/dev/upath.py
--rw-r--r--   0        0        0     2811 2023-06-02 12:28:18.951248 lamindb_setup-0.47.0/lnschema-core/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2023-05-30 14:21:30.384240 lamindb_setup-0.47.0/lnschema-core/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2023-05-30 14:21:30.384364 lamindb_setup-0.47.0/lnschema-core/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1381 2023-05-30 14:21:30.384442 lamindb_setup-0.47.0/lnschema-core/.gitignore
--rw-r--r--   0        0        0        0 2023-06-02 12:28:18.951387 lamindb_setup-0.47.0/lnschema-core/.gitmodules
--rw-r--r--   0        0        0     1836 2023-05-30 14:21:30.384687 lamindb_setup-0.47.0/lnschema-core/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11324 2023-05-30 14:21:30.384784 lamindb_setup-0.47.0/lnschema-core/LICENSE
--rw-r--r--   0        0        0      364 2023-05-30 14:21:30.384850 lamindb_setup-0.47.0/lnschema-core/README.md
--rw-r--r--   0        0        0    26073 2023-06-08 13:39:21.049523 lamindb_setup-0.47.0/lnschema-core/docs/changelog.md
--rw-r--r--   0        0        0     1485 2023-06-07 12:14:30.488309 lamindb_setup-0.47.0/lnschema-core/docs/guide/core-schema.ipynb
--rw-r--r--   0        0        0       52 2023-06-07 12:14:30.488642 lamindb_setup-0.47.0/lnschema-core/docs/guide/index.md
--rw-r--r--   0        0        0      112 2023-05-30 14:21:30.386018 lamindb_setup-0.47.0/lnschema-core/docs/index.md
--rw-r--r--   0        0        0      202 2023-05-30 14:21:30.386086 lamindb_setup-0.47.0/lnschema-core/lamin-project.yaml
--rw-r--r--   0        0        0      592 2023-06-07 12:14:30.488764 lamindb_setup-0.47.0/lnschema-core/lnschema_core/__init__.py
--rw-r--r--   0        0        0     1560 2023-06-07 12:14:30.488867 lamindb_setup-0.47.0/lnschema-core/lnschema_core/_lookup.py
--rw-r--r--   0        0        0      756 2023-06-07 12:14:30.488965 lamindb_setup-0.47.0/lnschema-core/lnschema_core/_types.py
--rw-r--r--   0        0        0      349 2023-06-02 12:28:18.953894 lamindb_setup-0.47.0/lnschema-core/lnschema_core/_users.py
--rw-r--r--   0        0        0     2810 2023-06-07 12:14:30.489236 lamindb_setup-0.47.0/lnschema-core/lnschema_core/ids.py
--rw-r--r--   0        0        0    11509 2023-06-07 12:14:30.489379 lamindb_setup-0.47.0/lnschema-core/lnschema_core/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-05-30 14:21:30.387900 lamindb_setup-0.47.0/lnschema-core/lnschema_core/migrations/__init__.py
--rw-r--r--   0        0        0    25727 2023-06-08 13:39:21.049900 lamindb_setup-0.47.0/lnschema-core/lnschema_core/models.py
--rw-r--r--   0        0        0      151 2023-06-07 12:14:30.489672 lamindb_setup-0.47.0/lnschema-core/lnschema_core/types.py
--rw-r--r--   0        0        0     1299 2023-06-07 12:14:30.490031 lamindb_setup-0.47.0/lnschema-core/noxfile.py
--rw-r--r--   0        0        0      850 2023-06-07 12:14:30.490216 lamindb_setup-0.47.0/lnschema-core/pyproject.toml
--rw-r--r--   0        0        0      475 2023-05-30 14:21:30.392155 lamindb_setup-0.47.0/lnschema-core/tests/test_notebooks.py
--rw-r--r--   0        0        0     1911 2023-06-07 16:31:43.467939 lamindb_setup-0.47.0/noxfile.py
--rw-r--r--   0        0        0     1337 2023-06-05 12:57:21.542553 lamindb_setup-0.47.0/pyproject.toml
--rw-r--r--   0        0        0      672 2023-06-04 11:49:29.990032 lamindb_setup-0.47.0/tests/test_bionty.py
--rw-r--r--   0        0        0     3041 2023-06-01 11:33:10.508406 lamindb_setup-0.47.0/tests/test_init_instance.py
--rw-r--r--   0        0        0      655 2023-06-01 11:33:10.508620 lamindb_setup-0.47.0/tests/test_load_instance.py
--rw-r--r--   0        0        0      501 2023-06-08 11:34:59.767695 lamindb_setup-0.47.0/tests/test_login.py
--rw-r--r--   0        0        0      243 2023-06-01 11:33:10.508784 lamindb_setup-0.47.0/tests/test_set_storage.py
--rw-r--r--   0        0        0      125 2023-06-08 11:34:59.767783 lamindb_setup-0.47.0/tests/test_signup.py
--rw-r--r--   0        0        0     1366 1970-01-01 00:00:00.000000 lamindb_setup-0.47.0/PKG-INFO
+-rw-r--r--   0        0        0     4010 2023-06-05 07:30:18.302219 lamindb_setup-0.47.1/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2023-06-01 15:58:18.274054 lamindb_setup-0.47.1/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2023-06-01 15:58:18.274134 lamindb_setup-0.47.1/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1204 2023-06-01 15:58:18.274221 lamindb_setup-0.47.1/.gitignore
+-rw-r--r--   0        0        0      100 2023-06-01 15:58:18.274299 lamindb_setup-0.47.1/.gitmodules
+-rw-r--r--   0        0        0     1798 2023-06-05 07:30:18.302425 lamindb_setup-0.47.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11324 2023-06-01 15:58:18.274545 lamindb_setup-0.47.1/LICENSE
+-rw-r--r--   0        0        0      318 2023-06-05 07:30:18.302530 lamindb_setup-0.47.1/README.md
+-rw-r--r--   0        0        0    53528 2023-06-09 20:33:41.387489 lamindb_setup-0.47.1/docs/changelog.md
+-rw-r--r--   0        0        0     6341 2023-06-05 07:30:18.302966 lamindb_setup-0.47.1/docs/faq/edge-cases-login-init.ipynb
+-rw-r--r--   0        0        0       96 2023-06-05 07:30:18.303105 lamindb_setup-0.47.1/docs/faq/index.md
+-rw-r--r--   0        0        0     3323 2023-06-01 15:58:18.275949 lamindb_setup-0.47.1/docs/faq/switch-environment.ipynb
+-rw-r--r--   0        0        0     6590 2023-06-07 16:09:22.842055 lamindb_setup-0.47.1/docs/faq/test-sqlite-sync.ipynb
+-rw-r--r--   0        0        0     8164 2023-06-08 13:53:23.373767 lamindb_setup-0.47.1/docs/guide/01-init-instance.ipynb
+-rw-r--r--   0        0        0     4362 2023-06-08 13:53:23.373956 lamindb_setup-0.47.1/docs/guide/02-load-instance.ipynb
+-rw-r--r--   0        0        0     5750 2023-06-08 13:53:23.374226 lamindb_setup-0.47.1/docs/guide/03-set-storage.ipynb
+-rw-r--r--   0        0        0     3313 2023-06-09 20:32:18.168464 lamindb_setup-0.47.1/docs/guide/04-schema-modules.ipynb
+-rw-r--r--   0        0        0      114 2023-06-08 18:13:52.871462 lamindb_setup-0.47.1/docs/guide/index.md
+-rw-r--r--   0        0        0      409 2023-06-08 18:13:52.872258 lamindb_setup-0.47.1/docs/guide/migrate.md
+-rw-r--r--   0        0        0     1250 2023-06-08 13:53:23.374760 lamindb_setup-0.47.1/docs/guide/setup-user.md
+-rw-r--r--   0        0        0      132 2023-06-08 13:53:23.374929 lamindb_setup-0.47.1/docs/index.md
+-rw-r--r--   0        0        0       61 2023-06-08 13:53:23.375035 lamindb_setup-0.47.1/docs/reference.md
+-rw-r--r--   0        0        0      365 2023-06-01 15:58:18.277034 lamindb_setup-0.47.1/docs/test_notebooks.py
+-rw-r--r--   0        0        0      142 2023-06-04 07:57:01.647274 lamindb_setup-0.47.1/lamin-project.yaml
+-rw-r--r--   0        0        0     2715 2023-06-09 20:33:08.714844 lamindb_setup-0.47.1/lamindb_setup/__init__.py
+-rw-r--r--   0        0        0     5346 2023-06-07 20:38:59.482711 lamindb_setup-0.47.1/lamindb_setup/__main__.py
+-rw-r--r--   0        0        0     1410 2023-06-05 07:31:41.044617 lamindb_setup-0.47.1/lamindb_setup/_check_instance_setup.py
+-rw-r--r--   0        0        0      661 2023-06-09 20:32:18.168808 lamindb_setup-0.47.1/lamindb_setup/_close.py
+-rw-r--r--   0        0        0     2006 2023-06-07 16:09:22.843059 lamindb_setup-0.47.1/lamindb_setup/_delete.py
+-rw-r--r--   0        0        0      585 2023-06-05 07:30:18.304343 lamindb_setup-0.47.1/lamindb_setup/_docstrings.py
+-rw-r--r--   0        0        0      329 2023-06-01 15:58:18.277912 lamindb_setup-0.47.1/lamindb_setup/_info.py
+-rw-r--r--   0        0        0     6835 2023-06-09 20:32:18.169160 lamindb_setup-0.47.1/lamindb_setup/_init_instance.py
+-rw-r--r--   0        0        0     5411 2023-06-09 20:04:14.225151 lamindb_setup-0.47.1/lamindb_setup/_load_instance.py
+-rw-r--r--   0        0        0      322 2023-06-05 07:30:18.304745 lamindb_setup-0.47.1/lamindb_setup/_migrate.py
+-rw-r--r--   0        0        0     1692 2023-06-03 14:25:55.266155 lamindb_setup-0.47.1/lamindb_setup/_notebook.py
+-rw-r--r--   0        0        0      825 2023-06-05 07:30:18.304849 lamindb_setup-0.47.1/lamindb_setup/_register_instance.py
+-rw-r--r--   0        0        0     1057 2023-06-05 07:30:18.305060 lamindb_setup-0.47.1/lamindb_setup/_schema.py
+-rw-r--r--   0        0        0     1891 2023-06-07 20:38:59.483389 lamindb_setup-0.47.1/lamindb_setup/_set.py
+-rw-r--r--   0        0        0     2247 2023-06-01 15:58:18.279311 lamindb_setup-0.47.1/lamindb_setup/_settings.py
+-rw-r--r--   0        0        0       87 2023-06-01 15:58:18.279395 lamindb_setup-0.47.1/lamindb_setup/_settings_load.py
+-rw-r--r--   0        0        0       72 2023-06-01 15:58:18.279466 lamindb_setup-0.47.1/lamindb_setup/_settings_store.py
+-rw-r--r--   0        0        0     3548 2023-06-05 07:30:18.305347 lamindb_setup-0.47.1/lamindb_setup/_setup_user.py
+-rw-r--r--   0        0        0      785 2023-06-05 07:30:18.305424 lamindb_setup-0.47.1/lamindb_setup/_silence_loggers.py
+-rw-r--r--   0        0        0      456 2023-06-01 15:58:18.279648 lamindb_setup-0.47.1/lamindb_setup/dev/__init__.py
+-rw-r--r--   0        0        0     5385 2023-06-07 16:33:24.023221 lamindb_setup-0.47.1/lamindb_setup/dev/_cloud_sqlite_locker.py
+-rw-r--r--   0        0        0     2491 2023-06-01 15:58:18.279932 lamindb_setup-0.47.1/lamindb_setup/dev/_deprecated.py
+-rw-r--r--   0        0        0     2905 2023-06-08 18:13:52.872904 lamindb_setup-0.47.1/lamindb_setup/dev/_django.py
+-rw-r--r--   0        0        0      240 2023-06-01 15:58:18.280089 lamindb_setup-0.47.1/lamindb_setup/dev/_docs.py
+-rw-r--r--   0        0        0     9315 2023-06-08 18:13:52.873426 lamindb_setup-0.47.1/lamindb_setup/dev/_settings_instance.py
+-rw-r--r--   0        0        0     2597 2023-06-01 15:58:18.280386 lamindb_setup-0.47.1/lamindb_setup/dev/_settings_load.py
+-rw-r--r--   0        0        0     2061 2023-06-01 15:58:18.280470 lamindb_setup-0.47.1/lamindb_setup/dev/_settings_save.py
+-rw-r--r--   0        0        0     2318 2023-06-05 07:30:18.305825 lamindb_setup-0.47.1/lamindb_setup/dev/_settings_store.py
+-rw-r--r--   0        0        0     1088 2023-06-01 15:58:18.280631 lamindb_setup-0.47.1/lamindb_setup/dev/_settings_user.py
+-rw-r--r--   0        0        0     2247 2023-06-09 20:32:18.169495 lamindb_setup-0.47.1/lamindb_setup/dev/_setup_bionty_sources.py
+-rw-r--r--   0        0        0     2140 2023-06-05 07:31:41.044990 lamindb_setup-0.47.1/lamindb_setup/dev/_setup_schema.py
+-rw-r--r--   0        0        0     5057 2023-06-05 07:30:18.306219 lamindb_setup-0.47.1/lamindb_setup/dev/_storage.py
+-rw-r--r--   0        0        0     2670 2023-06-08 18:13:52.874452 lamindb_setup-0.47.1/lamindb_setup/dev/upath.py
+-rw-r--r--   0        0        0     2811 2023-06-05 11:32:22.995643 lamindb_setup-0.47.1/lnschema-core/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2023-06-05 11:32:22.995738 lamindb_setup-0.47.1/lnschema-core/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2023-06-05 11:32:22.995812 lamindb_setup-0.47.1/lnschema-core/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1381 2023-06-05 11:32:22.995890 lamindb_setup-0.47.1/lnschema-core/.gitignore
+-rw-r--r--   0        0        0        0 2023-06-05 11:32:22.995916 lamindb_setup-0.47.1/lnschema-core/.gitmodules
+-rw-r--r--   0        0        0     1836 2023-06-05 11:32:22.996008 lamindb_setup-0.47.1/lnschema-core/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11324 2023-06-05 11:32:22.996105 lamindb_setup-0.47.1/lnschema-core/LICENSE
+-rw-r--r--   0        0        0      364 2023-06-05 11:32:22.996173 lamindb_setup-0.47.1/lnschema-core/README.md
+-rw-r--r--   0        0        0    25740 2023-06-05 11:32:22.996389 lamindb_setup-0.47.1/lnschema-core/docs/changelog.md
+-rw-r--r--   0        0        0     1485 2023-06-05 11:32:22.996551 lamindb_setup-0.47.1/lnschema-core/docs/guide/core-schema.ipynb
+-rw-r--r--   0        0        0       52 2023-06-05 11:32:22.996748 lamindb_setup-0.47.1/lnschema-core/docs/guide/index.md
+-rw-r--r--   0        0        0      112 2023-06-05 11:32:22.996845 lamindb_setup-0.47.1/lnschema-core/docs/index.md
+-rw-r--r--   0        0        0      202 2023-06-05 11:32:22.996914 lamindb_setup-0.47.1/lnschema-core/lamin-project.yaml
+-rw-r--r--   0        0        0      592 2023-06-05 11:32:22.997066 lamindb_setup-0.47.1/lnschema-core/lnschema_core/__init__.py
+-rw-r--r--   0        0        0     1515 2023-06-05 11:32:22.997223 lamindb_setup-0.47.1/lnschema-core/lnschema_core/_lookup.py
+-rw-r--r--   0        0        0      756 2023-06-05 11:32:22.997329 lamindb_setup-0.47.1/lnschema-core/lnschema_core/_types.py
+-rw-r--r--   0        0        0      349 2023-06-05 11:32:22.997395 lamindb_setup-0.47.1/lnschema-core/lnschema_core/_users.py
+-rw-r--r--   0        0        0     2810 2023-06-05 11:32:22.997546 lamindb_setup-0.47.1/lnschema-core/lnschema_core/ids.py
+-rw-r--r--   0        0        0    11504 2023-06-05 11:32:22.997705 lamindb_setup-0.47.1/lnschema-core/lnschema_core/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-06-05 11:32:22.997742 lamindb_setup-0.47.1/lnschema-core/lnschema_core/migrations/__init__.py
+-rw-r--r--   0        0        0    24760 2023-06-05 11:32:22.997959 lamindb_setup-0.47.1/lnschema-core/lnschema_core/models.py
+-rw-r--r--   0        0        0      180 2023-06-05 11:32:22.998145 lamindb_setup-0.47.1/lnschema-core/lnschema_core/types.py
+-rw-r--r--   0        0        0     1299 2023-06-05 11:32:22.998461 lamindb_setup-0.47.1/lnschema-core/noxfile.py
+-rw-r--r--   0        0        0      850 2023-06-05 11:32:22.998642 lamindb_setup-0.47.1/lnschema-core/pyproject.toml
+-rw-r--r--   0        0        0      475 2023-06-05 11:32:22.998792 lamindb_setup-0.47.1/lnschema-core/tests/test_notebooks.py
+-rw-r--r--   0        0        0     1911 2023-06-07 16:33:24.024562 lamindb_setup-0.47.1/noxfile.py
+-rw-r--r--   0        0        0     1337 2023-06-07 10:17:03.860879 lamindb_setup-0.47.1/pyproject.toml
+-rw-r--r--   0        0        0      672 2023-06-05 07:30:18.308956 lamindb_setup-0.47.1/tests/test_bionty.py
+-rw-r--r--   0        0        0     3041 2023-06-01 15:58:18.282108 lamindb_setup-0.47.1/tests/test_init_instance.py
+-rw-r--r--   0        0        0      655 2023-06-01 15:58:18.282187 lamindb_setup-0.47.1/tests/test_load_instance.py
+-rw-r--r--   0        0        0      501 2023-06-08 13:53:23.375191 lamindb_setup-0.47.1/tests/test_login.py
+-rw-r--r--   0        0        0      243 2023-06-01 15:58:18.282270 lamindb_setup-0.47.1/tests/test_set_storage.py
+-rw-r--r--   0        0        0      125 2023-06-08 13:53:23.375328 lamindb_setup-0.47.1/tests/test_signup.py
+-rw-r--r--   0        0        0     1366 1970-01-01 00:00:00.000000 lamindb_setup-0.47.1/PKG-INFO
```

### Comparing `lamindb_setup-0.47.0/.github/workflows/build.yml` & `lamindb_setup-0.47.1/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.0/.github/workflows/latest-changes.yml` & `lamindb_setup-0.47.1/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.0/.gitignore` & `lamindb_setup-0.47.1/.gitignore`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.0/.pre-commit-config.yaml` & `lamindb_setup-0.47.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.0/LICENSE` & `lamindb_setup-0.47.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.0/docs/changelog.md` & `lamindb_setup-0.47.1/docs/changelog.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
+🚑 Removed `LAMINDB_INSTANCE_LOADED` env variable | [411](https://github.com/laminlabs/lamindb-setup/pull/411) | [sunnyosun](https://github.com/sunnyosun) | 2023-06-09 | 0.47.1
+⬆️ Adapt to bionty naming in 0.18.0 | [410](https://github.com/laminlabs/lamindb-setup/pull/410) | [sunnyosun](https://github.com/sunnyosun) | 2023-06-09 |
 🚸 Warn about migrations | [409](https://github.com/laminlabs/lamindb-setup/pull/409) | [falexwolf](https://github.com/falexwolf) | 2023-06-08 | 0.47.0
 📝 Refactor guide | [408](https://github.com/laminlabs/lamindb-setup/pull/408) | [falexwolf](https://github.com/falexwolf) | 2023-06-08 |
 ✅ More testing of Bionty | [405](https://github.com/laminlabs/lamindb-setup/pull/405) | [falexwolf](https://github.com/falexwolf) | 2023-06-07 | 0.46a5
 ♻️ Reorder args of CLI | [407](https://github.com/laminlabs/lamindb-setup/pull/407) | [falexwolf](https://github.com/falexwolf) | 2023-06-07 |
 ♻️ Refactored init & load instance | [406](https://github.com/laminlabs/lamindb-setup/pull/406) | [falexwolf](https://github.com/falexwolf) | 2023-06-07 |
 💚 Fix dependencies | [404](https://github.com/laminlabs/lamindb-setup/pull/404) | [falexwolf](https://github.com/falexwolf) | 2023-06-07 |
 ♻️ Rename and set empty locker for now | [403](https://github.com/laminlabs/lamindb-setup/pull/403) | [falexwolf](https://github.com/falexwolf) | 2023-06-07 |
```

### Comparing `lamindb_setup-0.47.0/docs/faq/edge-cases-login-init.ipynb` & `lamindb_setup-0.47.1/docs/faq/edge-cases-login-init.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.0/docs/faq/switch-environment.ipynb` & `lamindb_setup-0.47.1/docs/faq/switch-environment.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.0/docs/faq/test-sqlite-sync.ipynb` & `lamindb_setup-0.47.1/docs/faq/test-sqlite-sync.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.0/docs/guide/01-init-instance.ipynb` & `lamindb_setup-0.47.1/docs/guide/01-init-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.0/docs/guide/02-load-instance.ipynb` & `lamindb_setup-0.47.1/docs/guide/02-load-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.0/docs/guide/03-set-storage.ipynb` & `lamindb_setup-0.47.1/docs/guide/03-set-storage.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.0/docs/guide/04-schema-modules.ipynb` & `lamindb_setup-0.47.1/docs/guide/04-schema-modules.ipynb`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9878472222222222%*

 * *Differences: {"'cells'": "{7: {'source': ['sources_df = pd.DataFrame(BiontySource.objects.all().values())\\n', "*

 * *            "'sources_df.head()']}, 11: {'source': {delete: [1, 0]}}, insert: [(8, "*

 * *            "OrderedDict([('cell_type', 'code'), ('execution_count', None), ('metadata', "*

 * *            "OrderedDict([('tags', ['hide-cell'])])), ('outputs', []), ('source', ['from "*

 * *            "bionty.dev._handle_sources import LAMINDB_SOURCES_PATH\\n', '\\n', 'assert "*

 * *            "sources_df.shape[0] > 0\\n', 'assert LAMIN […]*

```diff
@@ -74,15 +74,34 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "pd.DataFrame(BiontySource.objects.all().values()).head()"
+                "sources_df = pd.DataFrame(BiontySource.objects.all().values())\n",
+                "sources_df.head()"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {
+                "tags": [
+                    "hide-cell"
+                ]
+            },
+            "outputs": [],
+            "source": [
+                "from bionty.dev._handle_sources import LAMINDB_SOURCES_PATH\n",
+                "\n",
+                "assert sources_df.shape[0] > 0\n",
+                "assert LAMINDB_SOURCES_PATH.exists()\n",
+                "\n",
+                "LAMINDB_SOURCES_PATH.unlink(missing_ok=True)"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -109,16 +128,14 @@
             "metadata": {
                 "tags": [
                     "hide-cell"
                 ]
             },
             "outputs": [],
             "source": [
-                "from bionty.dev._handle_versions import LAMINDB_SOURCES_PATH\n",
-                "\n",
                 "assert LAMINDB_SOURCES_PATH.exists()"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
```

### Comparing `lamindb_setup-0.47.0/docs/guide/setup-user.md` & `lamindb_setup-0.47.1/docs/guide/setup-user.md`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.0/lamindb_setup/__init__.py` & `lamindb_setup-0.47.1/lamindb_setup/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -47,23 +47,23 @@
 
 .. autosummary::
    :toctree:
 
    dev
 """
 
-import os
 
-__version__ = "0.47.0"  # denote a release candidate for 0.1.0 with 0.1rc1
+__version__ = "0.47.1"  # denote a release candidate for 0.1.0 with 0.1rc1
 
 import builtins
 import sys
 from os import name as _os_name
 
 from . import dev
+from ._check_instance_setup import check_instance_setup as _check_instance_setup  # noqa
 from ._close import close  # noqa
 from ._delete import delete  # noqa
 from ._info import info  # noqa
 from ._init_instance import init  # noqa
 from ._load_instance import load  # noqa
 from ._migrate import migrate
 from ._register_instance import register  # noqa
```

### Comparing `lamindb_setup-0.47.0/lamindb_setup/__main__.py` & `lamindb_setup-0.47.1/lamindb_setup/__main__.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.0/lamindb_setup/_check_instance_setup.py` & `lamindb_setup-0.47.1/lamindb_setup/_check_instance_setup.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.0/lamindb_setup/_close.py` & `lamindb_setup-0.47.1/lamindb_setup/_close.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-import os
-
 from lamin_logger import logger
 
 from ._settings import settings
 from .dev._settings_store import current_instance_settings_file
+from .dev._setup_bionty_sources import delete_bionty_sources_yaml
 
 
 def close() -> None:
     """Close existing instance.
 
     Returns `None` if succeeds, otherwise an exception is raised.
     """
     if current_instance_settings_file().exists():
         instance = settings.instance.identifier
         settings.instance._update_cloud_sqlite_file()
         current_instance_settings_file().unlink()
-        os.environ["LAMINDB_INSTANCE_LOADED"] = "0"
+        delete_bionty_sources_yaml()
         logger.success(f"Closed {instance}")
     else:
         logger.info("No instance loaded")
```

### Comparing `lamindb_setup-0.47.0/lamindb_setup/_delete.py` & `lamindb_setup-0.47.1/lamindb_setup/_delete.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.0/lamindb_setup/_docstrings.py` & `lamindb_setup-0.47.1/lamindb_setup/_docstrings.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.0/lamindb_setup/_init_instance.py` & `lamindb_setup-0.47.1/lamindb_setup/_init_instance.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import importlib
-import os
 import sys
 from pathlib import Path
 from typing import Optional, Union
 
 from lamin_logger import logger
 from pydantic import PostgresDsn
 
@@ -201,15 +200,14 @@
     register_user_and_storage(isettings, settings.user)
     if init:
         write_bionty_sources(isettings)
     else:
         load_bionty_sources(isettings)
     isettings._persist()
     reload_lamindb(isettings)
-    os.environ["LAMINDB_INSTANCE_LOADED"] = "1"
 
 
 def infer_instance_name(
     *,
     storage: Union[str, Path, UPath],
     name: Optional[str] = None,
     db: Optional[PostgresDsn] = None,
```

### Comparing `lamindb_setup-0.47.0/lamindb_setup/_load_instance.py` & `lamindb_setup-0.47.1/lamindb_setup/_load_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.0/lamindb_setup/_notebook.py` & `lamindb_setup-0.47.1/lamindb_setup/_notebook.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.0/lamindb_setup/_register_instance.py` & `lamindb_setup-0.47.1/lamindb_setup/_register_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.0/lamindb_setup/_schema.py` & `lamindb_setup-0.47.1/lamindb_setup/_schema.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.0/lamindb_setup/_set.py` & `lamindb_setup-0.47.1/lamindb_setup/_set.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.0/lamindb_setup/_settings.py` & `lamindb_setup-0.47.1/lamindb_setup/_settings.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.0/lamindb_setup/_setup_user.py` & `lamindb_setup-0.47.1/lamindb_setup/_setup_user.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.0/lamindb_setup/_silence_loggers.py` & `lamindb_setup-0.47.1/lamindb_setup/_silence_loggers.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.0/lamindb_setup/dev/_cloud_sqlite_locker.py` & `lamindb_setup-0.47.1/lamindb_setup/dev/_cloud_sqlite_locker.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.0/lamindb_setup/dev/_deprecated.py` & `lamindb_setup-0.47.1/lamindb_setup/dev/_deprecated.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.0/lamindb_setup/dev/_django.py` & `lamindb_setup-0.47.1/lamindb_setup/dev/_django.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.0/lamindb_setup/dev/_settings_instance.py` & `lamindb_setup-0.47.1/lamindb_setup/dev/_settings_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.0/lamindb_setup/dev/_settings_load.py` & `lamindb_setup-0.47.1/lamindb_setup/dev/_settings_load.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.0/lamindb_setup/dev/_settings_save.py` & `lamindb_setup-0.47.1/lamindb_setup/dev/_settings_save.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.0/lamindb_setup/dev/_settings_store.py` & `lamindb_setup-0.47.1/lamindb_setup/dev/_settings_store.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.0/lamindb_setup/dev/_settings_user.py` & `lamindb_setup-0.47.1/lamindb_setup/dev/_settings_user.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.0/lamindb_setup/dev/_setup_bionty_sources.py` & `lamindb_setup-0.47.1/lamindb_setup/dev/_setup_bionty_sources.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,29 +3,38 @@
 
 from ._settings_instance import InstanceSettings
 
 
 def write_bionty_sources(isettings: InstanceSettings):
     """Write bionty sources to BiontySource table."""
     if "bionty" in isettings.schema:
+        import shutil
+
+        from bionty.dev._handle_sources import (
+            CURRENT_SOURCES_PATH,
+            LAMINDB_SOURCES_PATH,
+        )
+
+        shutil.copy(CURRENT_SOURCES_PATH, LAMINDB_SOURCES_PATH)
+
         import bionty as bt
         from lnschema_bionty.models import BiontySource
 
-        all_versions = bt.display_available_sources().reset_index()
-        all_versions_dict = all_versions.to_dict(orient="records")
+        all_sources = bt.display_available_sources().reset_index()
+        all_sources_dict = all_sources.to_dict(orient="records")
 
-        active_versions = (
+        currently_used = (
             bt.display_currently_used_sources()
             .reset_index()
             .set_index(["entity", "species"])
         )
 
         all_records = []
-        for kwargs in all_versions_dict:
-            act = active_versions.loc[(kwargs["entity"], kwargs["species"])].to_dict()
+        for kwargs in all_sources_dict:
+            act = currently_used.loc[(kwargs["entity"], kwargs["species"])].to_dict()
             if (act["source_key"] == kwargs["source_key"]) and (
                 act["version"] == kwargs["version"]
             ):
                 kwargs["currently_used"] = True
 
             record = BiontySource(**kwargs)
             all_records.append(record)
@@ -34,18 +43,25 @@
             for record in all_records:
                 record.save()
 
 
 def load_bionty_sources(isettings: InstanceSettings):
     """Write currently_used bionty sources to LAMINDB_VERSIONS_PATH in bionty."""
     if "bionty" in isettings.schema:
-        from bionty.dev._handle_versions import (
+        from bionty.dev._handle_sources import (
             LAMINDB_SOURCES_PATH,
             parse_currently_used_sources,
         )
         from bionty.dev._io import write_yaml
         from lnschema_bionty.models import BiontySource
 
         active_records = BiontySource.objects.filter(currently_used=True).all().values()
 
         write_yaml(parse_currently_used_sources(active_records), LAMINDB_SOURCES_PATH)
         logger.hint("Configured default bionty sources from BiontySource table")
+
+
+def delete_bionty_sources_yaml():
+    """Delete LAMINDB_SOURCES_PATH in bionty."""
+    from bionty.dev._handle_sources import LAMINDB_SOURCES_PATH
+
+    LAMINDB_SOURCES_PATH.unlink(missing_ok=True)
```

### Comparing `lamindb_setup-0.47.0/lamindb_setup/dev/_setup_schema.py` & `lamindb_setup-0.47.1/lamindb_setup/dev/_setup_schema.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.0/lamindb_setup/dev/_storage.py` & `lamindb_setup-0.47.1/lamindb_setup/dev/_storage.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.0/lamindb_setup/dev/upath.py` & `lamindb_setup-0.47.1/lamindb_setup/dev/upath.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.0/lnschema-core/.github/workflows/build.yml` & `lamindb_setup-0.47.1/lnschema-core/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.0/lnschema-core/.github/workflows/latest-changes.yml` & `lamindb_setup-0.47.1/lnschema-core/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.0/lnschema-core/.gitignore` & `lamindb_setup-0.47.1/lnschema-core/.gitignore`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.0/lnschema-core/.pre-commit-config.yaml` & `lamindb_setup-0.47.1/lnschema-core/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.0/lnschema-core/LICENSE` & `lamindb_setup-0.47.1/lnschema-core/LICENSE`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.0/lnschema-core/docs/changelog.md` & `lamindb_setup-0.47.1/lnschema-core/docs/changelog.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
-🎨 Auto fetch related names for Featureset | [188](https://github.com/laminlabs/lnschema-core/pull/188) | [sunnyosun](https://github.com/sunnyosun) | 2023-06-08 |
-🏗️ Re-architect transform id | [186](https://github.com/laminlabs/lnschema-core/pull/186) | [falexwolf](https://github.com/falexwolf) | 2023-06-06 | 0.35a7
-🎨 Adapted featureset | [185](https://github.com/laminlabs/lnschema-core/pull/185) | [sunnyosun](https://github.com/sunnyosun) | 2023-06-05 | 0.35a6
+🎨 Adapted featureset | [185](https://github.com/laminlabs/lnschema-core/pull/185) | [sunnyosun](https://github.com/sunnyosun) | 2023-06-05 |
 ♻️ Polish schema | [184](https://github.com/laminlabs/lnschema-core/pull/184) | [falexwolf](https://github.com/falexwolf) | 2023-06-05 |
 🚸 Improve QuerySet | [182](https://github.com/laminlabs/lnschema-core/pull/182) | [falexwolf](https://github.com/falexwolf) | 2023-06-05 |
 :fire: Delete SQLAlchemy related content | [181](https://github.com/laminlabs/lnschema-core/pull/181) | [falexwolf](https://github.com/falexwolf) | 2023-06-04 |
 :fire: Remove unncessary files | [180](https://github.com/laminlabs/lnschema-core/pull/180) | [falexwolf](https://github.com/falexwolf) | 2023-06-04 | 0.35a4
 ♻️ Absorb `DjangoORM.create()` in `DjangoORM.__init__()` | [178](https://github.com/laminlabs/lnschema-core/pull/178) | [falexwolf](https://github.com/falexwolf) | 2023-06-03 |
 ➖ Remove nbproject from code | [179](https://github.com/laminlabs/lnschema-core/pull/179) | [Koncopd](https://github.com/Koncopd) | 2023-06-03 |
 🏗️ Enable Django backend | [177](https://github.com/laminlabs/lnschema-core/pull/177) | [falexwolf](https://github.com/falexwolf) | 2023-06-02 | 0.35a3
```

### Comparing `lamindb_setup-0.47.0/lnschema-core/docs/guide/core-schema.ipynb` & `lamindb_setup-0.47.1/lnschema-core/docs/guide/core-schema.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.0/lnschema-core/lnschema_core/__init__.py` & `lamindb_setup-0.47.1/lnschema-core/lnschema_core/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Data objects & lineage (`yvzi`)."""
 _schema_id = "yvzi"
 _name = "core"
-__version__ = "0.35a7"
+__version__ = "0.35a4"
 
 import lamindb_setup as _lamindb_setup
 from lamindb_setup._check_instance_setup import (
     check_instance_setup as _check_instance_setup,
 )
 
 _INSTANCE_SETUP = _check_instance_setup()
```

### Comparing `lamindb_setup-0.47.0/lnschema-core/lnschema_core/_lookup.py` & `lamindb_setup-0.47.1/lnschema-core/lnschema_core/_lookup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,27 +3,26 @@
 from typing import Iterable, Optional
 
 from django.db import models
 
 
 def lookup(orm: models.Model, field: Optional[str] = None):
     """Lookup rows by field."""
-    model_field_names = [i.name for i in orm._meta.fields]
     if field is None:
         # by default use the name field
-        if "name" in model_field_names:
+        if "name" in orm.__fields__:
             field = "name"
         else:
-            non_ids = [i for i in model_field_names if "id" not in i]
+            non_ids = [i for i in orm.__fields__.keys() if "id" not in i]
             if len(non_ids) > 0:
                 # the first field isn't named with id
                 field = non_ids[0]
             else:
                 # the first field
-                field = model_field_names[0]
+                field = next(iter(orm.__fields__.keys()))
     values = set(orm.objects.values_list(field, flat=True))
     for value in [None, ""]:
         if value in values:
             values.remove(value)
     keys = to_lookup_keys(values, padding=orm.__name__)
     nt = namedtuple_from_dict(d=dict(zip(keys, values)), name=orm.__name__)
     return nt
```

### Comparing `lamindb_setup-0.47.0/lnschema-core/lnschema_core/_types.py` & `lamindb_setup-0.47.1/lnschema-core/lnschema_core/_types.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.0/lnschema-core/lnschema_core/ids.py` & `lamindb_setup-0.47.1/lnschema-core/lnschema_core/ids.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.0/lnschema-core/lnschema_core/migrations/0001_initial.py` & `lamindb_setup-0.47.1/lnschema-core/lnschema_core/migrations/0001_initial.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by Django 4.2.1 on 2023-06-06 01:58
+# Generated by Django 4.2.1 on 2023-06-05 12:36
 
 from typing import List
 
 import django.db.models.deletion
 from django.db import migrations, models
 
 import lnschema_core._types
@@ -48,15 +48,15 @@
         migrations.CreateModel(
             name="Run",
             fields=[
                 ("id", models.CharField(default=lnschema_core.ids.run, max_length=20, primary_key=True, serialize=False)),
                 ("name", models.CharField(db_index=True, max_length=255)),
                 ("external_id", models.CharField(db_index=True, max_length=255)),
                 ("created_at", models.DateTimeField(auto_now_add=True, db_index=True)),
-                ("run_at", models.DateTimeField(auto_now_add=True, db_index=True)),
+                ("updated_at", models.DateTimeField(auto_now=True, db_index=True)),
             ],
             options={
                 "managed": True,
             },
         ),
         migrations.CreateModel(
             name="User",
@@ -71,19 +71,19 @@
             options={
                 "managed": True,
             },
         ),
         migrations.CreateModel(
             name="Transform",
             fields=[
-                ("id", models.CharField(db_index=True, max_length=14, primary_key=True, serialize=False)),
+                ("id", models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name="ID")),
                 ("name", models.CharField(db_index=True, default=None, max_length=255, null=True)),
-                ("short_name", models.CharField(db_index=True, default=None, max_length=30, null=True)),
-                ("stem_id", models.CharField(db_index=True, default=lnschema_core.ids.transform, max_length=12)),
-                ("version", models.CharField(db_index=True, default="0", max_length=10)),
+                ("title", models.TextField(db_index=True, default=None, null=True)),
+                ("uid", models.CharField(db_index=True, default=lnschema_core.ids.transform, max_length=12)),
+                ("version", models.CharField(db_index=True, default=None, max_length=10, null=True)),
                 (
                     "type",
                     models.CharField(
                         choices=[("pipeline", "pipeline"), ("notebook", "notebook"), ("app", "app"), ("api", "api")],
                         db_index=True,
                         default=lnschema_core._types.TransformType["pipeline"],
                         max_length=20,
@@ -97,15 +97,15 @@
                     models.ForeignKey(
                         default=lnschema_core._users.current_user_id, on_delete=django.db.models.deletion.DO_NOTHING, related_name="created_transforms", to="lnschema_core.user"
                     ),
                 ),
             ],
             options={
                 "managed": True,
-                "unique_together": {("stem_id", "version")},
+                "unique_together": {("uid", "version")},
             },
         ),
         migrations.CreateModel(
             name="Storage",
             fields=[
                 ("id", models.CharField(db_index=True, default=lnschema_core.ids.storage, max_length=8, primary_key=True, serialize=False)),
                 ("root", models.CharField(db_index=True, max_length=255)),
```

### Comparing `lamindb_setup-0.47.0/lnschema-core/lnschema_core/models.py` & `lamindb_setup-0.47.1/lnschema-core/lnschema_core/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,16 +30,15 @@
     This brings some of the SQLAlchemy/SQLModel/SQL-inspired calls.
 
     As LaminDB was based on SQLAlchemy/SQLModel in the beginning, and might
     support it again in the future, these calls will be supported longtime.
     """
 
     def df(self):
-        columns = [field.name for field in self.model._meta.fields if not isinstance(field, models.ForeignKey)]
-        columns += [f"{field.name}_id" for field in self.model._meta.fields if isinstance(field, models.ForeignKey)]
+        columns = [field.name for field in self.model._meta.fields]
         df = pd.DataFrame(self.values(), columns=columns)
         if "id" in df.columns:
             df = df.set_index("id")
         return df
 
     def list(self) -> List:
         return list(self)
@@ -91,15 +90,15 @@
         managed = True
 
 
 class User(BaseORM):
     """User accounts.
 
     All data in this table is synched from the cloud user account to ensure a
-    universal user identity, valid across DB instances, email & handle changes.
+    globally unique user identity.
     """
 
     id = models.CharField(max_length=8, primary_key=True)
     """Universal id, valid across DB instances."""
     handle = models.CharField(max_length=30, unique=True, db_index=True)
     """Universal handle, valid across DB instances."""
     email = models.CharField(max_length=255, unique=True, db_index=True)
@@ -112,40 +111,41 @@
     """Time of last update to record."""
 
     class Meta:
         managed = True
 
 
 class Storage(BaseORM):
-    """Storage locations, typically cloud storage buckets.
+    """Storage locations, typically cloud buckets.
 
-    A file can be stored in S3 and GCP buckets or local storage locations.
+    A file or run-associated file can be stored in any desired S3,
+    GCP bucket or local storage location.
 
-    This ORM tracks these locations along with metadata.
+    This table tracks these locations along with metadata.
     """
 
     id = models.CharField(max_length=8, default=ids.storage, db_index=True, primary_key=True)
     """Universal id, valid across DB instances."""
     root = models.CharField(max_length=255, db_index=True)
-    """Path to the root of the storage location (an s3 path, a local path, etc.)."""
+    """Path to the root of the storage location: an s3 path, a local path, etc."""
     type = models.CharField(max_length=63, db_index=True)
     """Local vs. s3 vs. gcp etc."""
     region = models.CharField(max_length=63, db_index=True, null=True)
     """Cloud storage region, if applicable."""
     created_at = models.DateTimeField(auto_now_add=True, db_index=True)
     """Time of creation of record."""
     updated_at = models.DateTimeField(auto_now=True, db_index=True)
     """Time of last update to record."""
     created_by = models.ForeignKey(
         User,
         models.DO_NOTHING,
         default=current_user_id,
         related_name="created_storages",
     )
-    """Creator of record, a :class:`~lamindb.User`."""
+    """Creator of record."""
 
     class Meta:
         managed = True
 
 
 class Project(BaseORM):
     """Projects."""
@@ -166,15 +166,15 @@
     """Time of last update to record."""
     created_by = models.ForeignKey(
         User,
         models.DO_NOTHING,
         default=current_user_id,
         related_name="created_projects",
     )
-    """Creator of record, a :class:`~lamindb.User`."""
+    """Creator of record."""
 
     class Meta:
         managed = True
 
 
 class Transform(BaseORM):
     """Data transformations.
@@ -184,41 +184,39 @@
     A pipeline is versioned software that transforms data.
     This can be anything from typical workflow tools (Nextflow, Snakemake,
     Prefect, Apache Airflow, etc.) to simple (versioned) scripts.
 
     Creating a file is a transform, too.
     """
 
-    id = models.CharField(max_length=14, db_index=True, primary_key=True)
-    """Universal id, composed of stem_id and version suffix."""
     name = models.CharField(max_length=255, db_index=True, null=True, default=None)
-    """Transform name or title, a pipeline name, notebook title, etc..
+    """A name for the transform, a pipeline name, or a file name of a notebook or script.
     """
-    short_name = models.CharField(max_length=30, db_index=True, null=True, default=None)
-    """A short name.
+    title = models.TextField(db_index=True, null=True, default=None)
+    """An additional title, like a notebook title.
     """
-    stem_id = models.CharField(max_length=12, default=ids.transform, db_index=True)
-    """Stem of id, identifying transform up to version."""
-    version = models.CharField(max_length=10, default="0", db_index=True)
-    """Version, defaults to `"0"`.
+    uid = models.CharField(max_length=12, default=ids.transform, db_index=True)
+    """Universal id, valid across DB instances."""
+    version = models.CharField(max_length=10, default=None, db_index=True, null=True)
+    """Version identifier, defaults to `"0"`.
 
-    Use this to label different versions of the same pipeline, notebook, etc.
+    Use this to label different versions of the same transform.
 
     Consider using `semantic versioning <https://semver.org>`__
     with `Python versioning <https://peps.python.org/pep-0440/>`__.
     """
     type = models.CharField(
         max_length=20,
         choices=TransformType.choices(),
         db_index=True,
         default=TRANSFORM_TYPE_DEFAULT,
     )
     """Transform type.
 
-    Defaults to `notebook` if run from ipython and to `pipeline` if run from python.
+    Defaults to `notebook` if run from IPython, from a script to `pipeline`.
 
     If run from the app, it defaults to `app`.
     """
     reference = models.CharField(max_length=255, db_index=True, null=True, default=None)
     """Reference for the transform, e.g., a URL.
     """
     created_at = models.DateTimeField(auto_now_add=True, db_index=True)
@@ -227,50 +225,45 @@
     """Time of last update to record."""
     created_by = models.ForeignKey(
         User,
         models.DO_NOTHING,
         default=current_user_id,
         related_name="created_transforms",
     )
-    """Creator of record, a :class:`~lamindb.User`."""
+    """Creator of record."""
 
     class Meta:
         managed = True
-        unique_together = (("stem_id", "version"),)
-
-    def __init__(self, *args, **kwargs):
-        if len(args) > 0:  # initialize with all fields from db as args
-            super().__init__(*args, **kwargs)
-            return None
-        else:  # user-facing calling signature
-            # set default ids
-            if "id" not in kwargs and "stem_id" not in kwargs:
-                kwargs["id"] = ids.base62(n_char=14)
-                kwargs["stem_id"] = kwargs["id"][:12]
-            elif "stem_id" in kwargs:
-                assert isinstance(kwargs["stem_id"], str) and len(kwargs["stem_id"]) == 12
-                kwargs["id"] = kwargs["stem_id"] + ids.base62(n_char=2)
-            elif "id" in kwargs:
-                assert isinstance(kwargs["id"], str) and len(kwargs["id"]) == 14
-                kwargs["stem_id"] = kwargs["id"][:12]
-            super().__init__(**kwargs)
+        unique_together = (("uid", "version"),)
 
 
 class Run(BaseORM):
-    """Runs of data transformations.
+    """Runs of data transforms.
 
-    Typically, a run has inputs and outputs:
+    A `run` is any transform of a `file`.
 
-    - References to outputs are stored in the `File` ORM in the `run` field.
-      This is possible as every given file has a unique run that created it. Any
-      given `Run` can output multiple `files`: `run.outputs`.
-    - References to inputs are stored in the `RunInput` ORM, a many-to-many link
-      ORM between `File` and `Run`. Any `file` might serve as an input for
-      multiple `runs`: `file.input_of`. Similarly, any `run` might have many
-      `files` as inputs: `run.inputs`.
+    Args:
+        id: Optional[str] = None
+        name: Optional[str] = None
+        load_latest: bool = False - Load latest run for given notebook or pipeline.
+        transform: Optional[Transform] = None
+        inputs: List[File] = None
+        outputs: List[File] = None
+
+    It typically has inputs and outputs:
+
+    - References to outputs are stored in the `file` table in the
+      `run_id` column as a foreign key the `run`
+      table. This is possible as every given `file` has a unique data run:
+      the `run` that produced the `file`. However, note that a given
+      `run` may output several `files`.
+    - References to inputs are stored in the `run_in` table, a
+      many-to-many link table between the `file` and `run` tables. Any
+      `file` might serve as an input for many `runs`. Similarly, any
+      `run` might have many `files` as inputs.
     """
 
     id = models.CharField(max_length=20, default=ids.run, primary_key=True)
     """Universal id, valid across DB instances."""
     name = models.CharField(max_length=255, db_index=True)
     """Name or title of run."""
     external_id = models.CharField(max_length=255, db_index=True)
@@ -278,65 +271,65 @@
     transform = models.ForeignKey(Transform, models.DO_NOTHING, related_name="runs")
     """The transform :class:`~lamindb.Transform` that is being run."""
     inputs = models.ManyToManyField("File", through=RunInput, related_name="input_of")
     """The input files for the run."""
     # outputs on File
     created_at = models.DateTimeField(auto_now_add=True, db_index=True)
     """Time of creation of record."""
-    run_at = models.DateTimeField(auto_now_add=True, db_index=True)
-    """Time of run execution."""
+    updated_at = models.DateTimeField(auto_now=True, db_index=True)
+    """Time of last update to record."""
     created_by = models.ForeignKey(User, models.DO_NOTHING, default=current_user_id, related_name="created_runs")
-    """Creator of record, a :class:`~lamindb.User`."""
+    """Creator of record."""
 
     class Meta:
         managed = True
 
 
 class Featureset(BaseORM):
     """Feature sets.
 
     A feature set is represented by the hash of the set of primary keys and the feature type.
 
-    The current supported feature types are `lnschema_bionty.Gene`,
-    `lnschema_bionty.Protein`, and `lnschema_bionty.CellMarker`.
+    The current supported feature types are lnschema_bionty.Gene,
+    lnschema_bionty.Protein & lnschema_bionty.CellMarker.
 
     Guides:
 
     - :doc:`/biology/scrna`
     - :doc:`/biology/flow`
 
     Examples:
 
     >>> import lnschema_bionty as bt
     >>> reference = bt.Gene(species="mouse")
-    >>> features = ln.Features.from_iterable(adata.var["ensemble_id"], Gene.ensembl_gene_id)
-    >>> features.save()
-    >>> file = ln.File(adata, name="Mouse Lymph Node scRNA-seq")
-    >>> file.save()
-    >>> file.featuresets.add(featureset)
+    >>> features = ln.Features(adata, reference=reference)
+    >>> file = ln.File(adata, name="Mouse Lymph Node scRNA-seq", features=features)
 
+    Args:
+        data: [Path, str, pd.DataFrame, ad.AnnData] - DataFrame or AnnData to parse.
+        reference: Any = None - Reference for mapping features.
     """
 
     id = models.CharField(max_length=64, primary_key=True)
-    """A universal id, valid across DB instances, a hash of the linked set of features."""
+    """A universal id, valid across DB instances: a hash of the linked set of features."""
     type = models.CharField(max_length=64)
     """A feature entity type."""
     files = models.ManyToManyField("File", related_name="featuresets")
     """Files linked to the featureset."""
     created_at = models.DateTimeField(auto_now_add=True, db_index=True)
     """Time of creation of record."""
     updated_at = models.DateTimeField(auto_now=True, db_index=True)
     """Time of last update to record."""
     created_by = models.ForeignKey(
         User,
         models.DO_NOTHING,
         default=current_user_id,
         related_name="created_featuresets",
     )
-    """Creator of record, a :class:`~lamindb.User`."""
+    """Creator of record."""
 
     class Meta:
         managed = True
 
     @classmethod
     def from_iterable(
         cls,
@@ -351,20 +344,21 @@
             iterable=iterable,
             field=field,
             species=species,
         )
         return features
 
     def __init__(self, *args, **kwargs):  # type: ignore
-        related_names = [i.related_name for i in self.__class__._meta.related_objects]
-
         relationships: Dict = {}
-        for related_name in related_names:
-            if related_name in kwargs:
-                relationships[related_name] = kwargs.pop(related_name)
+        if "genes" in kwargs:
+            relationships["genes"] = kwargs.pop("genes")
+        if "proteins" in kwargs:
+            relationships["proteins"] = kwargs.pop("proteins")
+        if "cell_markers" in kwargs:
+            relationships["cell_markers"] = kwargs.pop("cell_markers")
         self._relationships = relationships
 
         super().__init__(*args, **kwargs)
 
     def save(self, *args, **kwargs):
         super().save(*args, **kwargs)
         for key, records in self._relationships.items():
@@ -372,27 +366,27 @@
             getattr(self, key).set(records)
 
 
 class Folder(BaseORM):
     id = models.CharField(max_length=20, default=ids.folder, primary_key=True)
     """A universal random id, valid across DB instances."""
     name = models.CharField(max_length=255, db_index=True)
-    """Name or title of folder."""
+    """Name or title of the folder."""
     key = models.CharField(max_length=255, null=True, default=None, db_index=True)
-    """Storage key of folder."""
+    """Storage key of the folder."""
     storage = models.ForeignKey(Storage, models.DO_NOTHING, related_name="folders", null=True)
-    """:class:`~lamindb.Storage` location of folder, see `.path()` for full path."""
+    """Storage location of the folder."""
     files = models.ManyToManyField("File", related_name="folders")
-    """:class:`~lamindb.File` records in folder."""
+    """Files in folder."""
     created_at = models.DateTimeField(auto_now_add=True, db_index=True)
     """Time of creation of record."""
     updated_at = models.DateTimeField(auto_now=True, db_index=True)
     """Time of last update to record."""
     created_by = models.ForeignKey(User, models.DO_NOTHING, default=current_user_id, related_name="created_folders")
-    """Creator of record, a :class:`~lamindb.User`."""
+    """Creator of record."""
 
     class Meta:
         managed = True
         unique_together = (("storage", "key"),)
 
     @property
     def __name__(cls) -> str:
@@ -484,15 +478,15 @@
     # features from Features.files
     # input_of from Run.inputs
     created_at = models.DateTimeField(auto_now_add=True, db_index=True)
     """Time of creation of record."""
     updated_at = models.DateTimeField(auto_now=True, db_index=True)
     """Time of last update to record."""
     created_by = models.ForeignKey(User, models.DO_NOTHING, default=current_user_id, related_name="created_files")
-    """Creator of record, a :class:`~lamindb.User`."""
+    """Creator of record."""
 
     class Meta:
         managed = True
         unique_together = (("storage", "key"),)
 
     def path(self) -> Union[Path, UPath]:
         """Path on storage."""
@@ -621,16 +615,15 @@
         super().__init__(**kwargs)
         if data is not None:
             self._local_filepath = privates["local_filepath"]
             self._cloud_filepath = privates["cloud_filepath"]
             self._memory_rep = privates["memory_rep"]
             self._to_store = not privates["check_path_in_storage"]
 
-    def save(self, *args, **kwargs) -> None:
-        """Save the file to database & storage."""
+    def save(self, *args, **kwargs):
         if self.transform is not None:
             self.transform.save()
         if self.run is not None:
             self.run.save()
         super().save(*args, **kwargs)
```

### Comparing `lamindb_setup-0.47.0/lnschema-core/noxfile.py` & `lamindb_setup-0.47.1/lnschema-core/noxfile.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.0/lnschema-core/pyproject.toml` & `lamindb_setup-0.47.1/lnschema-core/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.0/noxfile.py` & `lamindb_setup-0.47.1/noxfile.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.0/pyproject.toml` & `lamindb_setup-0.47.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.0/tests/test_bionty.py` & `lamindb_setup-0.47.1/tests/test_bionty.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.0/tests/test_init_instance.py` & `lamindb_setup-0.47.1/tests/test_init_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.0/tests/test_load_instance.py` & `lamindb_setup-0.47.1/tests/test_load_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.0/PKG-INFO` & `lamindb_setup-0.47.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lamindb_setup
-Version: 0.47.0
+Version: 0.47.1
 Summary: LaminDB setup.
 Author-email: Lamin Labs <laminlabs@gmail.com>
 Description-Content-Type: text/markdown
 Requires-Dist: lnhub_rest==0.9.10
 Requires-Dist: sqlmodel
 Requires-Dist: lnschema_core>=0.35a1
 Requires-Dist: lamin_logger>=0.3.3
```

