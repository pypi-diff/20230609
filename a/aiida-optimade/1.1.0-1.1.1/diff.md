# Comparing `tmp/aiida-optimade-1.1.0.tar.gz` & `tmp/aiida-optimade-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiida-optimade-1.1.0.tar", last modified: Tue Oct 11 11:10:41 2022, max compression
+gzip compressed data, was "aiida-optimade-1.1.1.tar", last modified: Fri Jun  9 16:41:30 2023, max compression
```

## Comparing `aiida-optimade-1.1.0.tar` & `aiida-optimade-1.1.1.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 11:10:41.811125 aiida-optimade-1.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 11:10:41.807125 aiida-optimade-1.1.0/.docker/
--rwxr-xr-x   0 runner    (1001) docker     (121)      853 2022-10-11 11:06:52.000000 aiida-optimade-1.1.0/.docker/run.sh
--rw-r--r--   0 runner    (1001) docker     (121)       67 2022-10-11 11:06:52.000000 aiida-optimade-1.1.0/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (121)      606 2022-10-11 11:06:52.000000 aiida-optimade-1.1.0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (121)     1067 2022-10-11 11:06:52.000000 aiida-optimade-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      245 2022-10-11 11:06:52.000000 aiida-optimade-1.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    14374 2022-10-11 11:10:41.811125 aiida-optimade-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    12982 2022-10-11 11:06:52.000000 aiida-optimade-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 11:10:41.807125 aiida-optimade-1.1.0/aiida_optimade/
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-10-11 11:10:06.000000 aiida-optimade-1.1.0/aiida_optimade/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 11:10:41.807125 aiida-optimade-1.1.0/aiida_optimade/cli/
--rw-r--r--   0 runner    (1001) docker     (121)      155 2022-10-11 11:06:52.000000 aiida-optimade-1.1.0/aiida_optimade/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1604 2022-10-11 11:06:52.000000 aiida-optimade-1.1.0/aiida_optimade/cli/cmd_aiida_optimade.py
--rw-r--r--   0 runner    (1001) docker     (121)     5440 2022-10-11 11:06:52.000000 aiida-optimade-1.1.0/aiida_optimade/cli/cmd_calc.py
--rw-r--r--   0 runner    (1001) docker     (121)    10248 2022-10-11 11:06:52.000000 aiida-optimade-1.1.0/aiida_optimade/cli/cmd_init.py
--rw-r--r--   0 runner    (1001) docker     (121)     2063 2022-10-11 11:06:52.000000 aiida-optimade-1.1.0/aiida_optimade/cli/cmd_run.py
--rw-r--r--   0 runner    (1001) docker     (121)      197 2022-10-11 11:06:52.000000 aiida-optimade-1.1.0/aiida_optimade/cli/options.py
--rw-r--r--   0 runner    (1001) docker     (121)      535 2022-10-11 11:06:52.000000 aiida-optimade-1.1.0/aiida_optimade/cli/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 11:10:41.811125 aiida-optimade-1.1.0/aiida_optimade/common/
--rw-r--r--   0 runner    (1001) docker     (121)      233 2022-10-11 11:06:52.000000 aiida-optimade-1.1.0/aiida_optimade/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      841 2022-10-11 11:06:52.000000 aiida-optimade-1.1.0/aiida_optimade/common/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     1800 2022-10-11 11:06:52.000000 aiida-optimade-1.1.0/aiida_optimade/common/logger.py
--rw-r--r--   0 runner    (1001) docker     (121)      403 2022-10-11 11:06:52.000000 aiida-optimade-1.1.0/aiida_optimade/common/warnings.py
--rw-r--r--   0 runner    (1001) docker     (121)      915 2022-10-11 11:10:06.000000 aiida-optimade-1.1.0/aiida_optimade/config.json
--rw-r--r--   0 runner    (1001) docker     (121)      400 2022-10-11 11:06:52.000000 aiida-optimade-1.1.0/aiida_optimade/config.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 11:10:41.811125 aiida-optimade-1.1.0/aiida_optimade/data/
--rw-r--r--   0 runner    (1001) docker     (121)      245 2022-10-11 11:06:52.000000 aiida-optimade-1.1.0/aiida_optimade/data/links.json
--rw-r--r--   0 runner    (1001) docker     (121)    21069 2022-10-11 11:06:52.000000 aiida-optimade-1.1.0/aiida_optimade/entry_collections.py
--rw-r--r--   0 runner    (1001) docker     (121)     5854 2022-10-11 11:06:52.000000 aiida-optimade-1.1.0/aiida_optimade/main.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 11:10:41.811125 aiida-optimade-1.1.0/aiida_optimade/mappers/
--rw-r--r--   0 runner    (1001) docker     (121)      176 2022-10-11 11:06:52.000000 aiida-optimade-1.1.0/aiida_optimade/mappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3068 2022-10-11 11:06:52.000000 aiida-optimade-1.1.0/aiida_optimade/mappers/entries.py
--rw-r--r--   0 runner    (1001) docker     (121)     4433 2022-10-11 11:06:52.000000 aiida-optimade-1.1.0/aiida_optimade/mappers/structures.py
--rw-r--r--   0 runner    (1001) docker     (121)     1421 2022-10-11 11:06:52.000000 aiida-optimade-1.1.0/aiida_optimade/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 11:10:41.811125 aiida-optimade-1.1.0/aiida_optimade/models/
--rw-r--r--   0 runner    (1001) docker     (121)      135 2022-10-11 11:06:52.000000 aiida-optimade-1.1.0/aiida_optimade/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1062 2022-10-11 11:06:52.000000 aiida-optimade-1.1.0/aiida_optimade/models/structures.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 11:10:41.811125 aiida-optimade-1.1.0/aiida_optimade/routers/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-11 11:06:52.000000 aiida-optimade-1.1.0/aiida_optimade/routers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3530 2022-10-11 11:06:52.000000 aiida-optimade-1.1.0/aiida_optimade/routers/info.py
--rw-r--r--   0 runner    (1001) docker     (121)     1068 2022-10-11 11:06:52.000000 aiida-optimade-1.1.0/aiida_optimade/routers/links.py
--rw-r--r--   0 runner    (1001) docker     (121)     2375 2022-10-11 11:06:52.000000 aiida-optimade-1.1.0/aiida_optimade/routers/structures.py
--rw-r--r--   0 runner    (1001) docker     (121)     5099 2022-10-11 11:06:52.000000 aiida-optimade-1.1.0/aiida_optimade/routers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 11:10:41.811125 aiida-optimade-1.1.0/aiida_optimade/transformers/
--rw-r--r--   0 runner    (1001) docker     (121)      111 2022-10-11 11:06:52.000000 aiida-optimade-1.1.0/aiida_optimade/transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8065 2022-10-11 11:06:52.000000 aiida-optimade-1.1.0/aiida_optimade/transformers/aiida.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 11:10:41.811125 aiida-optimade-1.1.0/aiida_optimade/translators/
--rw-r--r--   0 runner    (1001) docker     (121)      340 2022-10-11 11:06:52.000000 aiida-optimade-1.1.0/aiida_optimade/translators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4692 2022-10-11 11:06:52.000000 aiida-optimade-1.1.0/aiida_optimade/translators/cifs.py
--rw-r--r--   0 runner    (1001) docker     (121)     4997 2022-10-11 11:06:52.000000 aiida-optimade-1.1.0/aiida_optimade/translators/entities.py
--rw-r--r--   0 runner    (1001) docker     (121)    18454 2022-10-11 11:06:52.000000 aiida-optimade-1.1.0/aiida_optimade/translators/structures.py
--rw-r--r--   0 runner    (1001) docker     (121)     2714 2022-10-11 11:06:52.000000 aiida-optimade-1.1.0/aiida_optimade/translators/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     2258 2022-10-11 11:06:52.000000 aiida-optimade-1.1.0/aiida_optimade/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 11:10:41.807125 aiida-optimade-1.1.0/aiida_optimade.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    14374 2022-10-11 11:10:41.000000 aiida-optimade-1.1.0/aiida_optimade.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1751 2022-10-11 11:10:41.000000 aiida-optimade-1.1.0/aiida_optimade.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-11 11:10:41.000000 aiida-optimade-1.1.0/aiida_optimade.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       77 2022-10-11 11:10:41.000000 aiida-optimade-1.1.0/aiida_optimade.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      265 2022-10-11 11:10:41.000000 aiida-optimade-1.1.0/aiida_optimade.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-10-11 11:10:41.000000 aiida-optimade-1.1.0/aiida_optimade.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 11:10:41.811125 aiida-optimade-1.1.0/profiles/
--rw-r--r--   0 runner    (1001) docker     (121)     1216 2022-10-11 11:06:52.000000 aiida-optimade-1.1.0/profiles/config.j2
--rw-r--r--   0 runner    (1001) docker     (121)      895 2022-10-11 11:06:52.000000 aiida-optimade-1.1.0/profiles/docker-compose-mongo.j2
--rw-r--r--   0 runner    (1001) docker     (121)     1103 2022-10-11 11:06:52.000000 aiida-optimade-1.1.0/profiles/docker-compose-mongo.yml
--rw-r--r--   0 runner    (1001) docker     (121)      681 2022-10-11 11:06:52.000000 aiida-optimade-1.1.0/profiles/docker-compose.j2
--rw-r--r--   0 runner    (1001) docker     (121)      843 2022-10-11 11:06:52.000000 aiida-optimade-1.1.0/profiles/docker-compose.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1245 2022-10-11 11:06:52.000000 aiida-optimade-1.1.0/profiles/test_psql_dos.json
--rw-r--r--   0 runner    (1001) docker     (121)      278 2022-10-11 11:06:52.000000 aiida-optimade-1.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       42 2022-10-11 11:06:52.000000 aiida-optimade-1.1.0/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (121)       53 2022-10-11 11:06:52.000000 aiida-optimade-1.1.0/requirements_testing.txt
--rw-r--r--   0 runner    (1001) docker     (121)       76 2022-10-11 11:10:41.811125 aiida-optimade-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1257 2022-10-11 11:10:06.000000 aiida-optimade-1.1.0/setup.json
--rw-r--r--   0 runner    (1001) docker     (121)     1072 2022-10-11 11:06:52.000000 aiida-optimade-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:41:30.498096 aiida-optimade-1.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:41:30.490096 aiida-optimade-1.1.1/.docker/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      853 2023-06-09 16:26:02.000000 aiida-optimade-1.1.1/.docker/run.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-09 16:26:02.000000 aiida-optimade-1.1.1/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-06-09 16:26:02.000000 aiida-optimade-1.1.1/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-09 16:26:02.000000 aiida-optimade-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-09 16:26:02.000000 aiida-optimade-1.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14374 2023-06-09 16:41:30.498096 aiida-optimade-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12982 2023-06-09 16:26:02.000000 aiida-optimade-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:41:30.490096 aiida-optimade-1.1.1/aiida_optimade/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-09 16:40:44.000000 aiida-optimade-1.1.1/aiida_optimade/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:41:30.494096 aiida-optimade-1.1.1/aiida_optimade/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-09 16:26:02.000000 aiida-optimade-1.1.1/aiida_optimade/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-06-09 16:26:02.000000 aiida-optimade-1.1.1/aiida_optimade/cli/cmd_aiida_optimade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5580 2023-06-09 16:26:02.000000 aiida-optimade-1.1.1/aiida_optimade/cli/cmd_calc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10395 2023-06-09 16:26:02.000000 aiida-optimade-1.1.1/aiida_optimade/cli/cmd_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-06-09 16:26:02.000000 aiida-optimade-1.1.1/aiida_optimade/cli/cmd_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-09 16:26:02.000000 aiida-optimade-1.1.1/aiida_optimade/cli/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-06-09 16:26:02.000000 aiida-optimade-1.1.1/aiida_optimade/cli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:41:30.494096 aiida-optimade-1.1.1/aiida_optimade/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-09 16:26:02.000000 aiida-optimade-1.1.1/aiida_optimade/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-09 16:26:02.000000 aiida-optimade-1.1.1/aiida_optimade/common/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-06-09 16:26:02.000000 aiida-optimade-1.1.1/aiida_optimade/common/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-09 16:26:02.000000 aiida-optimade-1.1.1/aiida_optimade/common/warnings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-06-09 16:40:44.000000 aiida-optimade-1.1.1/aiida_optimade/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-09 16:26:02.000000 aiida-optimade-1.1.1/aiida_optimade/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:41:30.494096 aiida-optimade-1.1.1/aiida_optimade/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-09 16:26:02.000000 aiida-optimade-1.1.1/aiida_optimade/data/links.json
+-rw-r--r--   0 runner    (1001) docker     (123)    21069 2023-06-09 16:26:02.000000 aiida-optimade-1.1.1/aiida_optimade/entry_collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5854 2023-06-09 16:26:02.000000 aiida-optimade-1.1.1/aiida_optimade/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:41:30.494096 aiida-optimade-1.1.1/aiida_optimade/mappers/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-09 16:26:02.000000 aiida-optimade-1.1.1/aiida_optimade/mappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-06-09 16:26:02.000000 aiida-optimade-1.1.1/aiida_optimade/mappers/entries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4433 2023-06-09 16:26:02.000000 aiida-optimade-1.1.1/aiida_optimade/mappers/structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-06-09 16:26:02.000000 aiida-optimade-1.1.1/aiida_optimade/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:41:30.494096 aiida-optimade-1.1.1/aiida_optimade/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-09 16:26:02.000000 aiida-optimade-1.1.1/aiida_optimade/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-09 16:26:02.000000 aiida-optimade-1.1.1/aiida_optimade/models/structures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:41:30.494096 aiida-optimade-1.1.1/aiida_optimade/routers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 16:26:02.000000 aiida-optimade-1.1.1/aiida_optimade/routers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-06-09 16:26:02.000000 aiida-optimade-1.1.1/aiida_optimade/routers/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-09 16:26:02.000000 aiida-optimade-1.1.1/aiida_optimade/routers/links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-06-09 16:26:02.000000 aiida-optimade-1.1.1/aiida_optimade/routers/structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5493 2023-06-09 16:26:02.000000 aiida-optimade-1.1.1/aiida_optimade/routers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:41:30.494096 aiida-optimade-1.1.1/aiida_optimade/transformers/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-09 16:26:02.000000 aiida-optimade-1.1.1/aiida_optimade/transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8065 2023-06-09 16:26:02.000000 aiida-optimade-1.1.1/aiida_optimade/transformers/aiida.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:41:30.494096 aiida-optimade-1.1.1/aiida_optimade/translators/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-09 16:26:02.000000 aiida-optimade-1.1.1/aiida_optimade/translators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4691 2023-06-09 16:26:02.000000 aiida-optimade-1.1.1/aiida_optimade/translators/cifs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-06-09 16:26:02.000000 aiida-optimade-1.1.1/aiida_optimade/translators/entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18454 2023-06-09 16:26:02.000000 aiida-optimade-1.1.1/aiida_optimade/translators/structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-06-09 16:26:02.000000 aiida-optimade-1.1.1/aiida_optimade/translators/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-06-09 16:26:02.000000 aiida-optimade-1.1.1/aiida_optimade/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:41:30.490096 aiida-optimade-1.1.1/aiida_optimade.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14374 2023-06-09 16:41:30.000000 aiida-optimade-1.1.1/aiida_optimade.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-06-09 16:41:30.000000 aiida-optimade-1.1.1/aiida_optimade.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 16:41:30.000000 aiida-optimade-1.1.1/aiida_optimade.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-09 16:41:30.000000 aiida-optimade-1.1.1/aiida_optimade.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-09 16:41:30.000000 aiida-optimade-1.1.1/aiida_optimade.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-09 16:41:30.000000 aiida-optimade-1.1.1/aiida_optimade.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:41:30.498096 aiida-optimade-1.1.1/profiles/
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-06-09 16:26:02.000000 aiida-optimade-1.1.1/profiles/config.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-06-09 16:26:02.000000 aiida-optimade-1.1.1/profiles/docker-compose-mongo.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-06-09 16:26:02.000000 aiida-optimade-1.1.1/profiles/docker-compose-mongo.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-09 16:26:02.000000 aiida-optimade-1.1.1/profiles/docker-compose.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-09 16:26:02.000000 aiida-optimade-1.1.1/profiles/docker-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-06-09 16:26:02.000000 aiida-optimade-1.1.1/profiles/test_psql_dos.json
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-09 16:26:02.000000 aiida-optimade-1.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-09 16:26:02.000000 aiida-optimade-1.1.1/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-09 16:26:02.000000 aiida-optimade-1.1.1/requirements_testing.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-09 16:41:30.498096 aiida-optimade-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-06-09 16:40:44.000000 aiida-optimade-1.1.1/setup.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-09 16:26:02.000000 aiida-optimade-1.1.1/setup.py
```

### Comparing `aiida-optimade-1.1.0/.docker/run.sh` & `aiida-optimade-1.1.1/.docker/run.sh`

 * *Files identical despite different names*

### Comparing `aiida-optimade-1.1.0/Dockerfile` & `aiida-optimade-1.1.1/Dockerfile`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 FROM python:3.9
 
 WORKDIR /app
 
 # Install specific optimade and aiida-core versions
-ARG OPTIMADE_TOOLS_VERSION=0.19.4
-ARG AIIDA_VERSION=2.0.4
+ARG OPTIMADE_TOOLS_VERSION=0.24.1
+ARG AIIDA_VERSION=2.3.1
 
 # Copy repo contents
 COPY setup.py setup.json README.md requirements*.txt ./
 COPY aiida_optimade ./aiida_optimade
 
 RUN pip install -U pip setuptools wheel \
     && pip install optimade==${OPTIMADE_TOOLS_VERSION} \
```

### Comparing `aiida-optimade-1.1.0/LICENSE` & `aiida-optimade-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aiida-optimade-1.1.0/PKG-INFO` & `aiida-optimade-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiida-optimade
-Version: 1.1.0
+Version: 1.1.1
 Summary: Expose an AiiDA database according to the [OPTIMADE API specification](https://www.optimade.org).
 Home-page: https://github.com/aiidateam/aiida-optimade
 Author: Casper Welzel Andersen
 Author-email: developers@aiida.net
 License: MIT License
 Keywords: optimade aiida materials
 Classifier: Development Status :: 4 - Beta
@@ -39,15 +39,15 @@
 | Plugin | AiiDA | Python | Specification |
 |-|-|-|-|
 | `v1.0 < v2.0` | ![Compatibility for v1.0][AiiDA v2 range] |  [![PyPI pyversions](https://img.shields.io/pypi/pyversions/aiida-optimade)](https://pypi.org/project/aiida-optimade) | ![OPTIMADE API compatibility][OPTIMADE from OPT] |
 | `v0.18 <= v0.20` | ![Compatibility for v0][AiiDA v1 range] |  [![PyPI pyversions][Python v3.7-v3.9]](https://pypi.org/project/aiida-optimade/0.20.0/) | ![OPTIMADE API compatibility][OPTIMADE from OPT] |
 
 | Latest release | Build status | Activity |
 |:--------------:|:------------:|:--------:|
-| [![AiiDA](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/aiidateam/aiida-optimade/develop/.ci/aiida-version.json)](https://github.com/aiidateam/aiida-core/)<br>[![PyPI](https://img.shields.io/pypi/v/aiida-optimade)](https://pypi.org/project/aiida-optimade/)<br>[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/aiida-optimade)](https://pypi.org/project/aiida-optimade/)<br>[![OPTIMADE](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/Materials-Consortia/optimade-python-tools/v0.19.4/optimade-version.json)](https://github.com/Materials-Consortia/OPTIMADE/) | [![GitHub Workflow Status](https://img.shields.io/github/workflow/status/aiidateam/aiida-optimade/aiida-optimade)](https://github.com/aiidateam/aiida-optimade/actions/)<br>[![Codecov](https://img.shields.io/codecov/c/gh/aiidateam/aiida-optimade)](https://codecov.io/gh/aiidateam/aiida-optimade) | [![GitHub last commit](https://img.shields.io/github/last-commit/aiidateam/aiida-optimade)](https://github.com/aiidateam/aiida-optimade) |
+| [![AiiDA](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/aiidateam/aiida-optimade/develop/.ci/aiida-version.json)](https://github.com/aiidateam/aiida-core/)<br>[![PyPI](https://img.shields.io/pypi/v/aiida-optimade)](https://pypi.org/project/aiida-optimade/)<br>[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/aiida-optimade)](https://pypi.org/project/aiida-optimade/)<br>[![OPTIMADE](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/Materials-Consortia/optimade-python-tools/v0.24.1/optimade-version.json)](https://github.com/Materials-Consortia/OPTIMADE/) | [![GitHub Workflow Status](https://img.shields.io/github/workflow/status/aiidateam/aiida-optimade/aiida-optimade)](https://github.com/aiidateam/aiida-optimade/actions/)<br>[![Codecov](https://img.shields.io/codecov/c/gh/aiidateam/aiida-optimade)](https://codecov.io/gh/aiidateam/aiida-optimade) | [![GitHub last commit](https://img.shields.io/github/last-commit/aiidateam/aiida-optimade)](https://github.com/aiidateam/aiida-optimade) |
 
 This is a RESTful API server created with [FastAPI](https://fastapi.tiangolo.com/) that exposes an AiiDA database according to the [OPTIMADE specification](https://github.com/Materials-Consortia/OPTIMADE/blob/develop/optimade.rst).
 
 It is mainly used by [Materials Cloud](https://www.materialscloud.org/) to expose access to archived AiiDA databases through the OPTIMADE API.
 But it may be freely implemented by any to fulfill a similar purpose.
 
 The server is based on the test server "template" used in the [`optimade-python-tools`](https://github.com/Materials-Consortia/optimade-python-tools) package.
@@ -113,15 +113,15 @@
 
 ```shell
 $ aiida-optimade -p <PROFILE> init
 ```
 
 Where `<PROFILE>` is the AiiDA profile.
 
-> **Note**: Currently, the default is `optimade`, if the `-p / --profile` option is now specified.
+> **Note**: Currently, the default is `optimade`, if the `-p / --profile` option is not specified.
 > This will be changed in the future to use the default AiiDA profile.
 
 Initialization goes through your profile's `StructureData` nodes, adding an `optimade` extra, wherein all OPTIMADE-specific fields that do not have an equivalent AiiDA property are stored.
 
 If in the future, more `StructureData` nodes are added to your profile's database, these will be automatically updated for the first query, filtering on any of these OPTIMADE-specific fields.
 However, if you do not wish a significant lag for the user or risking several GET requests coming in at the same time, trying to update your profile's database, you should re-run `aiida-optimade init` for your profile (in between shutting the server down and restarting it again).
 
@@ -207,8 +207,8 @@
 
 [AiiDA v2 range]: https://img.shields.io/badge/AiiDA->=2.0.0,<3.0.0-007ec6.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACMAAAAhCAYAAABTERJSAAAABHNCSVQICAgIfAhkiAAAAAlwSFlzAAAFhgAABYYBG6Yz4AAAABl0RVh0U29mdHdhcmUAd3d3Lmlua3NjYXBlLm9yZ5vuPBoAAAUbSURBVFiFzZhrbFRVEMd%2Fc%2B5uu6UUbIFC%2FUAUVEQCLbQJBIiBDyiImJiIhmohYNCkqJAQxASLF8tDgYRHBLXRhIcKNtFEhVDgAxBJqgmVh4JEKg3EIn2QYqBlt917xg%2BFss%2ByaDHOtzsz5z%2B%2FuZl7ztmF%2F5HJvxVQN6cPYX8%2FPLnOmsvNAvqfwuib%2FbNIk9cQeQnLcKRL5xLIV%2Fic9eJeunjPYbRs4FjQSpTB3aS1IpRKeeOOewajy%2FKKEO8Q0DuVdKy8IqsbPulxGHUfCBBu%2BwUYGuFuBTK7wQnht6PEbf4tlRomVRjCbXNjQEB0AyrFQOL5ENIJm7dTLZE6DPJCnEtFZVXDLny%2B4Sjv0PmmYu1ZdUek9RiMgoDmJ8V0L7XJqsZ3UW8YsBOwEeHeeFce7jEYXBy0m9m4BbXqSj2%2Bxnkg26MCVrN6DEZcwggtd8pTFx%2Fh3B9B50YLaFOPwXQKUt0tBLegtSomfBlfY13PwijbEnhztGzgJsK5h9W9qeWwBqjvyhB2iBs1Qz0AU974DciRGO8CVN8AJhAeMAdA3KbrKEtvxhsI%2B9emWiJlGBEU680Cfk%2BSsVqXZvcFYGXjF8ABVJ%2BTNfVXehyms1zzn1gmIOxLEB6E31%2FWBe5rnCarmo7elf7dJEeaLh80GasliI5F6Q9cAz1GY1OJVNDxTzQTw7iY%2FHEZRQY7xqJ9RU2LFe%2FYqakdP911ha0XhjjiTVAkDwgatWfCGeYocx8M3glG8g8EXhSrLrHnEFJ5Ymow%2FkhIYv6ttYUW1iFmEqqxdVoUs9FmsDYSqmtmJh3Cl1%2BVtl2s7owDUdocR5bceiyoSivGTT5vzpbzL1uoBpmcAAQgW7ArnKD9ng9rc%2BNgrobSNwpSkkhcRN%2BvmXLjIsDovYHHEfmsYFygPAnIDEQrQPzJYCOaLHLUfIt7Oq0LJn9fxkSgNCb1qEIQ5UKgT%2Fs6gJmVOOroJhQBXVqw118QtWLdyUxEP45sUpSzqP7RDdFYMyB9UReMiF1MzPwoUqHt8hjGFFeP5wZAbZ%2F0%2BcAtAAcji6LeSq%2FMYiAvSsdw3GtrfVSVFUBbIhwRWYR7yOcr%2FBi%2FB1MSJZ16JlgH1AGM3EO2QnmMyrSbTSiACgFBv4yCUapZkt9qwWVL7aeOyHvArJjm8%2Fz9BhdI4XcZgz2%2FvRALosjsk1ODOyMcJn9%2FYI6IrkS5vxMGdUwou2YKfyVqJpn5t9aNs3gbQMbdbkxnGdsr4bTHm2AxWo9yNZK4PXR3uzhAh%2BM0AZejnCrGdy0UvJxl0oMKgWSLR%2B1LH2aE9ViejiFs%2BXn6bTjng3MlIhJ1I1TkuLdg6OcAbD7Xx%2Bc3y9TrWAiSHqVkbZ2v9ilCo6s4AjwZCzFyD9mOL305nV9aonvsQeT2L0gVk4OwOJqXXVRW7naaxswDKVdlYLyMXAnntteYmws2xcVVZzq%2BtHPAooQggmJkc6TLSusOiL4RKgwzzYU1iFQgiUBA1H7E8yPau%2BZl9P7AblVNebtHqTgxLfRqrNvZWjsHZFuqMqKcDWdlFjF7UGvX8Jn24DyEAykJwNcdg0OvJ4p5pQ9tV6SMlP4A0PNh8aYze1ArROyUNTNouy8tNF3Rt0CSXb6bRFl4%2FIfQzNMjaE9WwpYOWQnOdEF%2BTdJNO0iFh7%2BI0kfORzQZb6P2kymS9oTxzBiM9rUqLWr1WE5G6ODhycQd%2FUnNVeMbcH68hYkGycNoUNWc8fxaxfwhDbHpfwM5oeTY7rUX8QAAAABJRU5ErkJggg%3D%3D
 
 [AiiDA v1 range]: https://img.shields.io/badge/AiiDA->=1.6.0,<2.0.0-007ec6.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACMAAAAhCAYAAABTERJSAAAABHNCSVQICAgIfAhkiAAAAAlwSFlzAAAFhgAABYYBG6Yz4AAAABl0RVh0U29mdHdhcmUAd3d3Lmlua3NjYXBlLm9yZ5vuPBoAAAUbSURBVFiFzZhrbFRVEMd%2Fc%2B5uu6UUbIFC%2FUAUVEQCLbQJBIiBDyiImJiIhmohYNCkqJAQxASLF8tDgYRHBLXRhIcKNtFEhVDgAxBJqgmVh4JEKg3EIn2QYqBlt917xg%2BFss%2ByaDHOtzsz5z%2B%2FuZl7ztmF%2F5HJvxVQN6cPYX8%2FPLnOmsvNAvqfwuib%2FbNIk9cQeQnLcKRL5xLIV%2Fic9eJeunjPYbRs4FjQSpTB3aS1IpRKeeOOewajy%2FKKEO8Q0DuVdKy8IqsbPulxGHUfCBBu%2BwUYGuFuBTK7wQnht6PEbf4tlRomVRjCbXNjQEB0AyrFQOL5ENIJm7dTLZE6DPJCnEtFZVXDLny%2B4Sjv0PmmYu1ZdUek9RiMgoDmJ8V0L7XJqsZ3UW8YsBOwEeHeeFce7jEYXBy0m9m4BbXqSj2%2Bxnkg26MCVrN6DEZcwggtd8pTFx%2Fh3B9B50YLaFOPwXQKUt0tBLegtSomfBlfY13PwijbEnhztGzgJsK5h9W9qeWwBqjvyhB2iBs1Qz0AU974DciRGO8CVN8AJhAeMAdA3KbrKEtvxhsI%2B9emWiJlGBEU680Cfk%2BSsVqXZvcFYGXjF8ABVJ%2BTNfVXehyms1zzn1gmIOxLEB6E31%2FWBe5rnCarmo7elf7dJEeaLh80GasliI5F6Q9cAz1GY1OJVNDxTzQTw7iY%2FHEZRQY7xqJ9RU2LFe%2FYqakdP911ha0XhjjiTVAkDwgatWfCGeYocx8M3glG8g8EXhSrLrHnEFJ5Ymow%2FkhIYv6ttYUW1iFmEqqxdVoUs9FmsDYSqmtmJh3Cl1%2BVtl2s7owDUdocR5bceiyoSivGTT5vzpbzL1uoBpmcAAQgW7ArnKD9ng9rc%2BNgrobSNwpSkkhcRN%2BvmXLjIsDovYHHEfmsYFygPAnIDEQrQPzJYCOaLHLUfIt7Oq0LJn9fxkSgNCb1qEIQ5UKgT%2Fs6gJmVOOroJhQBXVqw118QtWLdyUxEP45sUpSzqP7RDdFYMyB9UReMiF1MzPwoUqHt8hjGFFeP5wZAbZ%2F0%2BcAtAAcji6LeSq%2FMYiAvSsdw3GtrfVSVFUBbIhwRWYR7yOcr%2FBi%2FB1MSJZ16JlgH1AGM3EO2QnmMyrSbTSiACgFBv4yCUapZkt9qwWVL7aeOyHvArJjm8%2Fz9BhdI4XcZgz2%2FvRALosjsk1ODOyMcJn9%2FYI6IrkS5vxMGdUwou2YKfyVqJpn5t9aNs3gbQMbdbkxnGdsr4bTHm2AxWo9yNZK4PXR3uzhAh%2BM0AZejnCrGdy0UvJxl0oMKgWSLR%2B1LH2aE9ViejiFs%2BXn6bTjng3MlIhJ1I1TkuLdg6OcAbD7Xx%2Bc3y9TrWAiSHqVkbZ2v9ilCo6s4AjwZCzFyD9mOL305nV9aonvsQeT2L0gVk4OwOJqXXVRW7naaxswDKVdlYLyMXAnntteYmws2xcVVZzq%2BtHPAooQggmJkc6TLSusOiL4RKgwzzYU1iFQgiUBA1H7E8yPau%2BZl9P7AblVNebtHqTgxLfRqrNvZWjsHZFuqMqKcDWdlFjF7UGvX8Jn24DyEAykJwNcdg0OvJ4p5pQ9tV6SMlP4A0PNh8aYze1ArROyUNTNouy8tNF3Rt0CSXb6bRFl4%2FIfQzNMjaE9WwpYOWQnOdEF%2BTdJNO0iFh7%2BI0kfORzQZb6P2kymS9oTxzBiM9rUqLWr1WE5G6ODhycQd%2FUnNVeMbcH68hYkGycNoUNWc8fxaxfwhDbHpfwM5oeTY7rUX8QAAAABJRU5ErkJggg%3D%3D
 
 [Python v3.7-v3.9]: https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9-blue
 
-[OPTIMADE from OPT]: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/Materials-Consortia/optimade-python-tools/v0.19.4/optimade-version.json
+[OPTIMADE from OPT]: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/Materials-Consortia/optimade-python-tools/v0.24.1/optimade-version.json
```

### Comparing `aiida-optimade-1.1.0/README.md` & `aiida-optimade-1.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 | Plugin | AiiDA | Python | Specification |
 |-|-|-|-|
 | `v1.0 < v2.0` | ![Compatibility for v1.0][AiiDA v2 range] |  [![PyPI pyversions](https://img.shields.io/pypi/pyversions/aiida-optimade)](https://pypi.org/project/aiida-optimade) | ![OPTIMADE API compatibility][OPTIMADE from OPT] |
 | `v0.18 <= v0.20` | ![Compatibility for v0][AiiDA v1 range] |  [![PyPI pyversions][Python v3.7-v3.9]](https://pypi.org/project/aiida-optimade/0.20.0/) | ![OPTIMADE API compatibility][OPTIMADE from OPT] |
 
 | Latest release | Build status | Activity |
 |:--------------:|:------------:|:--------:|
-| [![AiiDA](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/aiidateam/aiida-optimade/develop/.ci/aiida-version.json)](https://github.com/aiidateam/aiida-core/)<br>[![PyPI](https://img.shields.io/pypi/v/aiida-optimade)](https://pypi.org/project/aiida-optimade/)<br>[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/aiida-optimade)](https://pypi.org/project/aiida-optimade/)<br>[![OPTIMADE](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/Materials-Consortia/optimade-python-tools/v0.19.4/optimade-version.json)](https://github.com/Materials-Consortia/OPTIMADE/) | [![GitHub Workflow Status](https://img.shields.io/github/workflow/status/aiidateam/aiida-optimade/aiida-optimade)](https://github.com/aiidateam/aiida-optimade/actions/)<br>[![Codecov](https://img.shields.io/codecov/c/gh/aiidateam/aiida-optimade)](https://codecov.io/gh/aiidateam/aiida-optimade) | [![GitHub last commit](https://img.shields.io/github/last-commit/aiidateam/aiida-optimade)](https://github.com/aiidateam/aiida-optimade) |
+| [![AiiDA](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/aiidateam/aiida-optimade/develop/.ci/aiida-version.json)](https://github.com/aiidateam/aiida-core/)<br>[![PyPI](https://img.shields.io/pypi/v/aiida-optimade)](https://pypi.org/project/aiida-optimade/)<br>[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/aiida-optimade)](https://pypi.org/project/aiida-optimade/)<br>[![OPTIMADE](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/Materials-Consortia/optimade-python-tools/v0.24.1/optimade-version.json)](https://github.com/Materials-Consortia/OPTIMADE/) | [![GitHub Workflow Status](https://img.shields.io/github/workflow/status/aiidateam/aiida-optimade/aiida-optimade)](https://github.com/aiidateam/aiida-optimade/actions/)<br>[![Codecov](https://img.shields.io/codecov/c/gh/aiidateam/aiida-optimade)](https://codecov.io/gh/aiidateam/aiida-optimade) | [![GitHub last commit](https://img.shields.io/github/last-commit/aiidateam/aiida-optimade)](https://github.com/aiidateam/aiida-optimade) |
 
 This is a RESTful API server created with [FastAPI](https://fastapi.tiangolo.com/) that exposes an AiiDA database according to the [OPTIMADE specification](https://github.com/Materials-Consortia/OPTIMADE/blob/develop/optimade.rst).
 
 It is mainly used by [Materials Cloud](https://www.materialscloud.org/) to expose access to archived AiiDA databases through the OPTIMADE API.
 But it may be freely implemented by any to fulfill a similar purpose.
 
 The server is based on the test server "template" used in the [`optimade-python-tools`](https://github.com/Materials-Consortia/optimade-python-tools) package.
@@ -79,15 +79,15 @@
 
 ```shell
 $ aiida-optimade -p <PROFILE> init
 ```
 
 Where `<PROFILE>` is the AiiDA profile.
 
-> **Note**: Currently, the default is `optimade`, if the `-p / --profile` option is now specified.
+> **Note**: Currently, the default is `optimade`, if the `-p / --profile` option is not specified.
 > This will be changed in the future to use the default AiiDA profile.
 
 Initialization goes through your profile's `StructureData` nodes, adding an `optimade` extra, wherein all OPTIMADE-specific fields that do not have an equivalent AiiDA property are stored.
 
 If in the future, more `StructureData` nodes are added to your profile's database, these will be automatically updated for the first query, filtering on any of these OPTIMADE-specific fields.
 However, if you do not wish a significant lag for the user or risking several GET requests coming in at the same time, trying to update your profile's database, you should re-run `aiida-optimade init` for your profile (in between shutting the server down and restarting it again).
 
@@ -173,8 +173,8 @@
 
 [AiiDA v2 range]: https://img.shields.io/badge/AiiDA->=2.0.0,<3.0.0-007ec6.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACMAAAAhCAYAAABTERJSAAAABHNCSVQICAgIfAhkiAAAAAlwSFlzAAAFhgAABYYBG6Yz4AAAABl0RVh0U29mdHdhcmUAd3d3Lmlua3NjYXBlLm9yZ5vuPBoAAAUbSURBVFiFzZhrbFRVEMd%2Fc%2B5uu6UUbIFC%2FUAUVEQCLbQJBIiBDyiImJiIhmohYNCkqJAQxASLF8tDgYRHBLXRhIcKNtFEhVDgAxBJqgmVh4JEKg3EIn2QYqBlt917xg%2BFss%2ByaDHOtzsz5z%2B%2FuZl7ztmF%2F5HJvxVQN6cPYX8%2FPLnOmsvNAvqfwuib%2FbNIk9cQeQnLcKRL5xLIV%2Fic9eJeunjPYbRs4FjQSpTB3aS1IpRKeeOOewajy%2FKKEO8Q0DuVdKy8IqsbPulxGHUfCBBu%2BwUYGuFuBTK7wQnht6PEbf4tlRomVRjCbXNjQEB0AyrFQOL5ENIJm7dTLZE6DPJCnEtFZVXDLny%2B4Sjv0PmmYu1ZdUek9RiMgoDmJ8V0L7XJqsZ3UW8YsBOwEeHeeFce7jEYXBy0m9m4BbXqSj2%2Bxnkg26MCVrN6DEZcwggtd8pTFx%2Fh3B9B50YLaFOPwXQKUt0tBLegtSomfBlfY13PwijbEnhztGzgJsK5h9W9qeWwBqjvyhB2iBs1Qz0AU974DciRGO8CVN8AJhAeMAdA3KbrKEtvxhsI%2B9emWiJlGBEU680Cfk%2BSsVqXZvcFYGXjF8ABVJ%2BTNfVXehyms1zzn1gmIOxLEB6E31%2FWBe5rnCarmo7elf7dJEeaLh80GasliI5F6Q9cAz1GY1OJVNDxTzQTw7iY%2FHEZRQY7xqJ9RU2LFe%2FYqakdP911ha0XhjjiTVAkDwgatWfCGeYocx8M3glG8g8EXhSrLrHnEFJ5Ymow%2FkhIYv6ttYUW1iFmEqqxdVoUs9FmsDYSqmtmJh3Cl1%2BVtl2s7owDUdocR5bceiyoSivGTT5vzpbzL1uoBpmcAAQgW7ArnKD9ng9rc%2BNgrobSNwpSkkhcRN%2BvmXLjIsDovYHHEfmsYFygPAnIDEQrQPzJYCOaLHLUfIt7Oq0LJn9fxkSgNCb1qEIQ5UKgT%2Fs6gJmVOOroJhQBXVqw118QtWLdyUxEP45sUpSzqP7RDdFYMyB9UReMiF1MzPwoUqHt8hjGFFeP5wZAbZ%2F0%2BcAtAAcji6LeSq%2FMYiAvSsdw3GtrfVSVFUBbIhwRWYR7yOcr%2FBi%2FB1MSJZ16JlgH1AGM3EO2QnmMyrSbTSiACgFBv4yCUapZkt9qwWVL7aeOyHvArJjm8%2Fz9BhdI4XcZgz2%2FvRALosjsk1ODOyMcJn9%2FYI6IrkS5vxMGdUwou2YKfyVqJpn5t9aNs3gbQMbdbkxnGdsr4bTHm2AxWo9yNZK4PXR3uzhAh%2BM0AZejnCrGdy0UvJxl0oMKgWSLR%2B1LH2aE9ViejiFs%2BXn6bTjng3MlIhJ1I1TkuLdg6OcAbD7Xx%2Bc3y9TrWAiSHqVkbZ2v9ilCo6s4AjwZCzFyD9mOL305nV9aonvsQeT2L0gVk4OwOJqXXVRW7naaxswDKVdlYLyMXAnntteYmws2xcVVZzq%2BtHPAooQggmJkc6TLSusOiL4RKgwzzYU1iFQgiUBA1H7E8yPau%2BZl9P7AblVNebtHqTgxLfRqrNvZWjsHZFuqMqKcDWdlFjF7UGvX8Jn24DyEAykJwNcdg0OvJ4p5pQ9tV6SMlP4A0PNh8aYze1ArROyUNTNouy8tNF3Rt0CSXb6bRFl4%2FIfQzNMjaE9WwpYOWQnOdEF%2BTdJNO0iFh7%2BI0kfORzQZb6P2kymS9oTxzBiM9rUqLWr1WE5G6ODhycQd%2FUnNVeMbcH68hYkGycNoUNWc8fxaxfwhDbHpfwM5oeTY7rUX8QAAAABJRU5ErkJggg%3D%3D
 
 [AiiDA v1 range]: https://img.shields.io/badge/AiiDA->=1.6.0,<2.0.0-007ec6.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACMAAAAhCAYAAABTERJSAAAABHNCSVQICAgIfAhkiAAAAAlwSFlzAAAFhgAABYYBG6Yz4AAAABl0RVh0U29mdHdhcmUAd3d3Lmlua3NjYXBlLm9yZ5vuPBoAAAUbSURBVFiFzZhrbFRVEMd%2Fc%2B5uu6UUbIFC%2FUAUVEQCLbQJBIiBDyiImJiIhmohYNCkqJAQxASLF8tDgYRHBLXRhIcKNtFEhVDgAxBJqgmVh4JEKg3EIn2QYqBlt917xg%2BFss%2ByaDHOtzsz5z%2B%2FuZl7ztmF%2F5HJvxVQN6cPYX8%2FPLnOmsvNAvqfwuib%2FbNIk9cQeQnLcKRL5xLIV%2Fic9eJeunjPYbRs4FjQSpTB3aS1IpRKeeOOewajy%2FKKEO8Q0DuVdKy8IqsbPulxGHUfCBBu%2BwUYGuFuBTK7wQnht6PEbf4tlRomVRjCbXNjQEB0AyrFQOL5ENIJm7dTLZE6DPJCnEtFZVXDLny%2B4Sjv0PmmYu1ZdUek9RiMgoDmJ8V0L7XJqsZ3UW8YsBOwEeHeeFce7jEYXBy0m9m4BbXqSj2%2Bxnkg26MCVrN6DEZcwggtd8pTFx%2Fh3B9B50YLaFOPwXQKUt0tBLegtSomfBlfY13PwijbEnhztGzgJsK5h9W9qeWwBqjvyhB2iBs1Qz0AU974DciRGO8CVN8AJhAeMAdA3KbrKEtvxhsI%2B9emWiJlGBEU680Cfk%2BSsVqXZvcFYGXjF8ABVJ%2BTNfVXehyms1zzn1gmIOxLEB6E31%2FWBe5rnCarmo7elf7dJEeaLh80GasliI5F6Q9cAz1GY1OJVNDxTzQTw7iY%2FHEZRQY7xqJ9RU2LFe%2FYqakdP911ha0XhjjiTVAkDwgatWfCGeYocx8M3glG8g8EXhSrLrHnEFJ5Ymow%2FkhIYv6ttYUW1iFmEqqxdVoUs9FmsDYSqmtmJh3Cl1%2BVtl2s7owDUdocR5bceiyoSivGTT5vzpbzL1uoBpmcAAQgW7ArnKD9ng9rc%2BNgrobSNwpSkkhcRN%2BvmXLjIsDovYHHEfmsYFygPAnIDEQrQPzJYCOaLHLUfIt7Oq0LJn9fxkSgNCb1qEIQ5UKgT%2Fs6gJmVOOroJhQBXVqw118QtWLdyUxEP45sUpSzqP7RDdFYMyB9UReMiF1MzPwoUqHt8hjGFFeP5wZAbZ%2F0%2BcAtAAcji6LeSq%2FMYiAvSsdw3GtrfVSVFUBbIhwRWYR7yOcr%2FBi%2FB1MSJZ16JlgH1AGM3EO2QnmMyrSbTSiACgFBv4yCUapZkt9qwWVL7aeOyHvArJjm8%2Fz9BhdI4XcZgz2%2FvRALosjsk1ODOyMcJn9%2FYI6IrkS5vxMGdUwou2YKfyVqJpn5t9aNs3gbQMbdbkxnGdsr4bTHm2AxWo9yNZK4PXR3uzhAh%2BM0AZejnCrGdy0UvJxl0oMKgWSLR%2B1LH2aE9ViejiFs%2BXn6bTjng3MlIhJ1I1TkuLdg6OcAbD7Xx%2Bc3y9TrWAiSHqVkbZ2v9ilCo6s4AjwZCzFyD9mOL305nV9aonvsQeT2L0gVk4OwOJqXXVRW7naaxswDKVdlYLyMXAnntteYmws2xcVVZzq%2BtHPAooQggmJkc6TLSusOiL4RKgwzzYU1iFQgiUBA1H7E8yPau%2BZl9P7AblVNebtHqTgxLfRqrNvZWjsHZFuqMqKcDWdlFjF7UGvX8Jn24DyEAykJwNcdg0OvJ4p5pQ9tV6SMlP4A0PNh8aYze1ArROyUNTNouy8tNF3Rt0CSXb6bRFl4%2FIfQzNMjaE9WwpYOWQnOdEF%2BTdJNO0iFh7%2BI0kfORzQZb6P2kymS9oTxzBiM9rUqLWr1WE5G6ODhycQd%2FUnNVeMbcH68hYkGycNoUNWc8fxaxfwhDbHpfwM5oeTY7rUX8QAAAABJRU5ErkJggg%3D%3D
 
 [Python v3.7-v3.9]: https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9-blue
 
-[OPTIMADE from OPT]: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/Materials-Consortia/optimade-python-tools/v0.19.4/optimade-version.json
+[OPTIMADE from OPT]: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/Materials-Consortia/optimade-python-tools/v0.24.1/optimade-version.json
```

### Comparing `aiida-optimade-1.1.0/aiida_optimade/cli/cmd_aiida_optimade.py` & `aiida-optimade-1.1.1/aiida_optimade/cli/cmd_aiida_optimade.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,31 @@
 import os
 from pathlib import Path
+from typing import TYPE_CHECKING
 
 import click
-from aiida.cmdline.params.options import PROFILE as VERDI_PROFILE
+from aiida.cmdline.groups import VerdiCommandGroup
+from aiida.cmdline.params.options import PROFILE as AIIDA_PROFILE
 from aiida.cmdline.params.types import ProfileParamType as VerdiProfileParamType
-from aiida.manage.configuration import Profile, get_config
 
 from aiida_optimade.cli.options import AIIDA_PROFILES
 from aiida_optimade.cli.utils import AIIDA_OPTIMADE_TEST_PROFILE
 
+if TYPE_CHECKING:  # pragma: no cover
+    from aiida.cmdline.groups.verdi import VerdiContext
+    from aiida.manage.configuration import Profile
 
-@click.group(context_settings={"help_option_names": ["-h", "--help"]})
+
+@click.command(
+    cls=VerdiCommandGroup, context_settings={"help_option_names": ["-h", "--help"]}
+)
 @click.version_option(
     None, "-v", "--version", message="AiiDA-OPTIMADE version %(version)s"
 )
-@VERDI_PROFILE(
+@AIIDA_PROFILE(
     type=VerdiProfileParamType(),
     default="optimade",
     show_default=True,
     help="AiiDA profile to use and serve. Configured profiles: "
     f"{', '.join([repr(name) for name in AIIDA_PROFILES])}.",
 )
 @click.option(
@@ -26,25 +33,22 @@
     is_flag=True,
     default=False,
     show_default=True,
     help=f"Run in development mode (use the {AIIDA_OPTIMADE_TEST_PROFILE!r} AiiDA "
     "profile and `--debug` options).",
 )
 @click.pass_context
-def cli(ctx, profile: Profile, dev: bool):  # pragma: no cover
+def cli(ctx: "VerdiContext", profile: "Profile", dev: bool):  # pragma: no cover
     """AiiDA-OPTIMADE command line interface (CLI)."""
 
-    if ctx.obj is None:
-        ctx.obj = {}
-
     if dev:
-        profile = get_config(create=True).get_profile(AIIDA_OPTIMADE_TEST_PROFILE)
+        profile = ctx.obj.config.get_profile(AIIDA_OPTIMADE_TEST_PROFILE)
 
-    ctx.obj["profile"] = profile
-    ctx.obj["dev"] = dev
+    ctx.obj.profile = profile
+    ctx.obj.dev = dev
 
     # Set config
     if (
         not os.getenv("OPTIMADE_CONFIG_FILE")
         or not Path(os.getenv("OPTIMADE_CONFIG_FILE")).exists()
     ):
         os.environ["OPTIMADE_CONFIG_FILE"] = str(
```

### Comparing `aiida-optimade-1.1.0/aiida_optimade/cli/cmd_calc.py` & `aiida-optimade-1.1.1/aiida_optimade/cli/cmd_calc.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 # pylint: disable=protected-access,too-many-locals,too-many-branches
-from typing import Tuple
+from typing import TYPE_CHECKING
 
 import click
 from tqdm import tqdm
 
 from aiida_optimade.cli.cmd_aiida_optimade import cli
 from aiida_optimade.common.logger import LOGGER, disable_logging
 
+if TYPE_CHECKING:  # pragma: no cover
+    from typing import Tuple
+
+    from aiida.common.extendeddicts import AttributeDict
+
 
 @cli.command()
 @click.argument(
     "fields",
     type=click.STRING,
     required=True,
     nargs=-1,
@@ -31,25 +36,25 @@
     "--silent",
     is_flag=True,
     default=False,
     show_default=True,
     help="Suppress informational output.",
 )
 @click.pass_obj
-def calc(obj: dict, fields: Tuple[str], force_yes: bool, silent: bool):
+def calc(obj: "AttributeDict", fields: "Tuple[str]", force_yes: bool, silent: bool):
     """Calculate OPTIMADE fields in the AiiDA database."""
     from aiida import load_profile
     from aiida.cmdline.utils import echo
 
     # The default aiida.cmdline loglevel inherit from aiida loglevel is REPORT
     # Here we use INFO loglevel for the operations
     echo.CMDLINE_LOGGER.setLevel("INFO")
 
     try:
-        profile: str = obj.get("profile").name
+        profile: str = obj.profile.name
     except AttributeError:
         profile = None
     profile = load_profile(profile).name
 
     try:
         with disable_logging():
             from aiida_optimade.routers.structures import STRUCTURES
```

### Comparing `aiida-optimade-1.1.0/aiida_optimade/cli/cmd_init.py` & `aiida-optimade-1.1.1/aiida_optimade/cli/cmd_init.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 # pylint: disable=protected-access,too-many-statements
 from pathlib import Path
-from typing import IO, Generator, Iterator, List, Union
+from typing import TYPE_CHECKING
 
 import click
 from tqdm import tqdm
 
 from aiida_optimade.cli.cmd_aiida_optimade import cli
 from aiida_optimade.common.logger import LOGGER, disable_logging
 
+if TYPE_CHECKING:  # pragma: no cover
+    from typing import IO, Generator, Iterator, List, Union
+
+    from aiida.common.extendeddicts import AttributeDict
+
 
 @cli.command()
 @click.option(
     "-f",
     "--force",
     is_flag=True,
     default=False,
@@ -39,30 +44,30 @@
 )
 @click.option(
     "--filename",
     type=click.Path(exists=True, dir_okay=False, readable=True, resolve_path=True),
     help="Filename to load as database (currently only usable for MongoDB).",
 )
 @click.pass_obj
-def init(obj: dict, force: bool, silent: bool, mongo: bool, filename: str):
+def init(obj: "AttributeDict", force: bool, silent: bool, mongo: bool, filename: str):
     """Initialize an AiiDA database to be served with AiiDA-OPTIMADE."""
     from aiida import load_profile
     from aiida.cmdline.utils import echo
 
     # The default aiida.cmdline loglevel inherit from aiida loglevel is REPORT
     # Here we use INFO loglevel for the operations
     echo.CMDLINE_LOGGER.setLevel("INFO")
 
     filename: Path = Path(filename) if filename else filename
 
     if mongo and filename:
         profile = f"MongoDB JSON file {filename.name}"
     else:
         try:
-            profile: str = obj.get("profile").name
+            profile: str = obj.profile.name
         except AttributeError:
             profile = None
         profile = load_profile(profile).name
 
     try:
         with disable_logging():
             from aiida_optimade.routers.structures import STRUCTURES
@@ -217,16 +222,16 @@
             echo.echo_info(
                 "No new StructureData and CifData Nodes or MongoDB documents found to "
                 f"initialize for {profile}."
             )
 
 
 def read_chunks(
-    file_object: IO, chunk_size: int = None
-) -> Generator[Union[str, bytes], None, None]:
+    file_object: "IO", chunk_size: int = None
+) -> "Generator[Union[str, bytes], None, None]":
     """Generator to read a file piece by piece
 
     Parameters:
         file_object: The opened file or file-like object.
         chunk_size: Size of bytes/characters to read and yield (default size: 16 MB).
 
     Yields:
@@ -239,16 +244,16 @@
         data = file_object.read(chunk_size)
         if not data:
             break
         yield data
 
 
 def get_documents(
-    chunk_iterator: Union[Generator[str, None, None], Iterator[str]]
-) -> Generator[List[dict], None, None]:
+    chunk_iterator: "Union[Generator[str, None, None], Iterator[str]]",
+) -> "Generator[List[dict], None, None]":
     """Generator to return MongoDB documents from file"""
     rest_chunk = ""
 
     for raw_chunk in chunk_iterator:
         raw_chunk = rest_chunk + raw_chunk
         rest_chunk = ""
```

### Comparing `aiida-optimade-1.1.0/aiida_optimade/cli/cmd_run.py` & `aiida-optimade-1.1.1/aiida_optimade/cli/cmd_run.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 # pylint: disable=too-many-arguments
+from typing import TYPE_CHECKING
+
 import click
 
 from aiida_optimade.cli.cmd_aiida_optimade import cli
 from aiida_optimade.cli.options import LOGGING_LEVELS
 
+if TYPE_CHECKING:  # pragma: no cover
+    from aiida.common.extendeddicts import AttributeDict
+
 
 @cli.command()
 @click.option(
     "--log-level",
     type=click.Choice(LOGGING_LEVELS, case_sensitive=False),
     default="info",
     show_default=True,
@@ -39,21 +44,28 @@
     "--reload",
     is_flag=True,
     default=False,
     show_default=True,
     help="Enable auto-reload. Note, if --debug is set, this will also be set to True.",
 )
 @click.pass_obj
-def run(obj: dict, log_level: str, debug: bool, host: str, port: int, reload: bool):
+def run(
+    obj: "AttributeDict",
+    log_level: str,
+    debug: bool,
+    host: str,
+    port: int,
+    reload: bool,
+):
     """Run AiiDA-OPTIMADE server."""
     import os
 
     import uvicorn
 
-    if obj.get("dev", False):
+    if getattr(obj, "dev", False):
         debug = True
 
     log_level = log_level.lower()
     if debug and log_level == "info":
         log_level = "debug"
 
     if debug and not reload:
@@ -66,21 +78,20 @@
 
     os.environ["AIIDA_OPTIMADE_LOG_LEVEL"] = log_level.upper()
 
     if os.getenv("AIIDA_PROFILE") is None:
         from aiida import load_profile
 
         try:
-            profile: str = obj.get("profile").name
+            profile: str = obj.profile.name
         except AttributeError:
             profile = None
         profile_name: str = load_profile(profile).name
         os.environ["AIIDA_PROFILE"] = profile_name
 
     uvicorn.run(
         "aiida_optimade.main:APP",
         reload=reload,
         host=host,
         port=port,
         log_level=log_level,
-        debug=debug,
     )
```

### Comparing `aiida-optimade-1.1.0/aiida_optimade/cli/utils.py` & `aiida-optimade-1.1.1/aiida_optimade/cli/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,19 @@
-from typing import List
+from typing import TYPE_CHECKING
 
 from aiida.common.exceptions import ConfigurationError, MissingConfigurationError
 from aiida.manage.configuration import get_config
 
+if TYPE_CHECKING:  # pragma: no cover
+    from typing import List
+
 AIIDA_OPTIMADE_TEST_PROFILE = "aiida-optimade_test"
 
 
-def get_aiida_profiles() -> List[str]:
+def get_aiida_profiles() -> "List[str]":
     """Retrieve list of configured AiiDA profiles"""
 
     try:
         config = get_config()
     except (MissingConfigurationError, ConfigurationError):
         return []
```

### Comparing `aiida-optimade-1.1.0/aiida_optimade/common/exceptions.py` & `aiida-optimade-1.1.1/aiida_optimade/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `aiida-optimade-1.1.0/aiida_optimade/common/logger.py` & `aiida-optimade-1.1.1/aiida_optimade/common/logger.py`

 * *Files identical despite different names*

### Comparing `aiida-optimade-1.1.0/aiida_optimade/config.json` & `aiida-optimade-1.1.1/aiida_optimade/config.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9921875%*

 * *Differences: {"'implementation'": "{'version': '1.1.1'}"}*

```diff
@@ -12,15 +12,15 @@
     "base_url": null,
     "implementation": {
         "maintainer": {
             "email": "casper.andersen@epfl.ch"
         },
         "name": "aiida-optimade",
         "source_url": "https://github.com/aiidateam/aiida-optimade",
-        "version": "1.1.0"
+        "version": "1.1.1"
     },
     "page_limit": 15,
     "page_limit_max": 500,
     "provider": {
         "description": "AiiDA: Automated Interactive Infrastructure and Database for Computational Science (http://www.aiida.net)",
         "homepage": "http://www.aiida.net",
         "index_base_url": null,
```

### Comparing `aiida-optimade-1.1.0/aiida_optimade/entry_collections.py` & `aiida-optimade-1.1.1/aiida_optimade/entry_collections.py`

 * *Files identical despite different names*

### Comparing `aiida-optimade-1.1.0/aiida_optimade/main.py` & `aiida-optimade-1.1.1/aiida_optimade/main.py`

 * *Files identical despite different names*

### Comparing `aiida-optimade-1.1.0/aiida_optimade/mappers/entries.py` & `aiida-optimade-1.1.1/aiida_optimade/mappers/entries.py`

 * *Files identical despite different names*

### Comparing `aiida-optimade-1.1.0/aiida_optimade/mappers/structures.py` & `aiida-optimade-1.1.1/aiida_optimade/mappers/structures.py`

 * *Files identical despite different names*

### Comparing `aiida-optimade-1.1.0/aiida_optimade/middleware.py` & `aiida-optimade-1.1.1/aiida_optimade/middleware.py`

 * *Files identical despite different names*

### Comparing `aiida-optimade-1.1.0/aiida_optimade/models/structures.py` & `aiida-optimade-1.1.1/aiida_optimade/models/structures.py`

 * *Files identical despite different names*

### Comparing `aiida-optimade-1.1.0/aiida_optimade/routers/info.py` & `aiida-optimade-1.1.1/aiida_optimade/routers/info.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,26 +26,30 @@
 def get_info(request: Request):
     from optimade.models import BaseInfoAttributes, BaseInfoResource
     from optimade.server.routers.utils import get_base_url
 
     parse_result = urllib.parse.urlparse(str(request.url))
     base_url = get_base_url(parse_result)
 
+    root_path_str = ""
+    if CONFIG.root_path:
+        root_path_str = f"/{CONFIG.root_path.strip('/')}"
+
     return InfoResponse(
         meta=meta_values(
             str(request.url), 1, 1, more_data_available=False, schema=CONFIG.schema_url
         ),
         data=BaseInfoResource(
             id=BaseInfoResource.schema()["properties"]["id"]["default"],
             type=BaseInfoResource.schema()["properties"]["type"]["default"],
             attributes=BaseInfoAttributes(
                 api_version=__api_version__,
                 available_api_versions=[
                     {
-                        "url": f"{base_url}/v{__api_version__.split('-')[0].split('+')[0].split('.')[0]}",
+                        "url": f"{base_url}{root_path_str}/v{__api_version__.split('-')[0].split('+')[0].split('.')[0]}",
                         "version": __api_version__,
                     }
                 ],
                 formats=["json"],
                 entry_types_by_format={"json": list(ENTRY_INFO_SCHEMAS.keys())},
                 available_endpoints=[
                     "info",
```

### Comparing `aiida-optimade-1.1.0/aiida_optimade/routers/links.py` & `aiida-optimade-1.1.1/aiida_optimade/routers/links.py`

 * *Files identical despite different names*

### Comparing `aiida-optimade-1.1.0/aiida_optimade/routers/structures.py` & `aiida-optimade-1.1.1/aiida_optimade/routers/structures.py`

 * *Files identical despite different names*

### Comparing `aiida-optimade-1.1.0/aiida_optimade/routers/utils.py` & `aiida-optimade-1.1.1/aiida_optimade/routers/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 import functools
 import urllib.parse
-from typing import Union
+from typing import TYPE_CHECKING
 
 from fastapi import HTTPException, Request
 from optimade.models import EntryResponseMany, EntryResponseOne, ToplevelLinks
 from optimade.server.config import CONFIG
 from optimade.server.entry_collections.mongo import MongoCollection
 from optimade.server.query_params import EntryListingQueryParams, SingleEntryQueryParams
 from optimade.server.routers.utils import handle_response_fields, meta_values
 
 from aiida_optimade.entry_collections import AiidaCollection
 
+if TYPE_CHECKING:  # pragma: no cover
+    from typing import Type, Union
+
 
 def handle_pagination(
     request: Request, more_data_available: bool, nresults: int
 ) -> dict:
     """Handle pagination for request with number of results equal nresults"""
     from optimade.server.routers.utils import get_base_url
 
@@ -54,33 +57,47 @@
     else:
         pagination["next"] = None
 
     return pagination
 
 
 def get_entries(
-    collection: Union[AiidaCollection, MongoCollection],
-    response: EntryResponseMany,
+    collection: "Union[AiidaCollection, MongoCollection]",
+    response: "Type[EntryResponseMany]",
     request: Request,
     params: EntryListingQueryParams,
 ) -> EntryResponseMany:
     """Generalized /{entry} endpoint getter"""
     (
         results,
         data_returned,
         more_data_available,
         fields,
         include_fields,
     ) = collection.find(params)
 
-    pagination = handle_pagination(
-        request=request, more_data_available=more_data_available, nresults=len(results)
-    )
+    if results is None:
+        nresults = 0
+        results = []
+    else:
+        try:
+            nresults = len(results)
+        except TypeError:
+            nresults = 1
+            results = [results]
+
+    pagination = {}
+    if results:
+        pagination = handle_pagination(
+            request=request,
+            more_data_available=more_data_available,
+            nresults=nresults,
+        )
 
-    if fields or include_fields:
+    if (fields or include_fields) and results:
         results = handle_response_fields(
             results=results, exclude_fields=fields, include_fields=include_fields
         )
 
     return response(
         links=ToplevelLinks(**pagination),
         data=results,
@@ -91,17 +108,17 @@
             more_data_available=more_data_available,
             schema=CONFIG.schema_url,
         ),
     )
 
 
 def get_single_entry(
-    collection: Union[AiidaCollection, MongoCollection],
+    collection: "Union[AiidaCollection, MongoCollection]",
     entry_id: str,
-    response: EntryResponseOne,
+    response: "Type[EntryResponseOne]",
     request: Request,
     params: SingleEntryQueryParams,
 ) -> EntryResponseOne:
     """Generalized /{entry}/{entry_id} endpoint getter"""
     params.filter = f'id="{entry_id}"'
     (
         results,
```

### Comparing `aiida-optimade-1.1.0/aiida_optimade/transformers/aiida.py` & `aiida-optimade-1.1.1/aiida_optimade/transformers/aiida.py`

 * *Files identical despite different names*

### Comparing `aiida-optimade-1.1.0/aiida_optimade/translators/cifs.py` & `aiida-optimade-1.1.1/aiida_optimade/translators/cifs.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,14 @@
 
     with cif.open() as handle:
         parser = CifParser(handle, **constructor_kwargs)
 
     try:
         structures = parser.get_structures(**parameters)
     except ValueError as exc_one:
-
         # Verify whether the failure was due to wrong occupancy numbers
         try:
             constructor_kwargs["occupancy_tolerance"] = 1e10
             with cif.open() as handle:
                 parser = CifParser(handle, **constructor_kwargs)
             structures = parser.get_structures(**parameters)
         except ValueError as exc_two:
```

### Comparing `aiida-optimade-1.1.0/aiida_optimade/translators/entities.py` & `aiida-optimade-1.1.1/aiida_optimade/translators/entities.py`

 * *Files identical despite different names*

### Comparing `aiida-optimade-1.1.0/aiida_optimade/translators/structures.py` & `aiida-optimade-1.1.1/aiida_optimade/translators/structures.py`

 * *Files identical despite different names*

### Comparing `aiida-optimade-1.1.0/aiida_optimade/translators/utils.py` & `aiida-optimade-1.1.1/aiida_optimade/translators/utils.py`

 * *Files identical despite different names*

### Comparing `aiida-optimade-1.1.0/aiida_optimade/utils.py` & `aiida-optimade-1.1.1/aiida_optimade/utils.py`

 * *Files identical despite different names*

### Comparing `aiida-optimade-1.1.0/aiida_optimade.egg-info/PKG-INFO` & `aiida-optimade-1.1.1/aiida_optimade.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiida-optimade
-Version: 1.1.0
+Version: 1.1.1
 Summary: Expose an AiiDA database according to the [OPTIMADE API specification](https://www.optimade.org).
 Home-page: https://github.com/aiidateam/aiida-optimade
 Author: Casper Welzel Andersen
 Author-email: developers@aiida.net
 License: MIT License
 Keywords: optimade aiida materials
 Classifier: Development Status :: 4 - Beta
@@ -39,15 +39,15 @@
 | Plugin | AiiDA | Python | Specification |
 |-|-|-|-|
 | `v1.0 < v2.0` | ![Compatibility for v1.0][AiiDA v2 range] |  [![PyPI pyversions](https://img.shields.io/pypi/pyversions/aiida-optimade)](https://pypi.org/project/aiida-optimade) | ![OPTIMADE API compatibility][OPTIMADE from OPT] |
 | `v0.18 <= v0.20` | ![Compatibility for v0][AiiDA v1 range] |  [![PyPI pyversions][Python v3.7-v3.9]](https://pypi.org/project/aiida-optimade/0.20.0/) | ![OPTIMADE API compatibility][OPTIMADE from OPT] |
 
 | Latest release | Build status | Activity |
 |:--------------:|:------------:|:--------:|
-| [![AiiDA](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/aiidateam/aiida-optimade/develop/.ci/aiida-version.json)](https://github.com/aiidateam/aiida-core/)<br>[![PyPI](https://img.shields.io/pypi/v/aiida-optimade)](https://pypi.org/project/aiida-optimade/)<br>[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/aiida-optimade)](https://pypi.org/project/aiida-optimade/)<br>[![OPTIMADE](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/Materials-Consortia/optimade-python-tools/v0.19.4/optimade-version.json)](https://github.com/Materials-Consortia/OPTIMADE/) | [![GitHub Workflow Status](https://img.shields.io/github/workflow/status/aiidateam/aiida-optimade/aiida-optimade)](https://github.com/aiidateam/aiida-optimade/actions/)<br>[![Codecov](https://img.shields.io/codecov/c/gh/aiidateam/aiida-optimade)](https://codecov.io/gh/aiidateam/aiida-optimade) | [![GitHub last commit](https://img.shields.io/github/last-commit/aiidateam/aiida-optimade)](https://github.com/aiidateam/aiida-optimade) |
+| [![AiiDA](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/aiidateam/aiida-optimade/develop/.ci/aiida-version.json)](https://github.com/aiidateam/aiida-core/)<br>[![PyPI](https://img.shields.io/pypi/v/aiida-optimade)](https://pypi.org/project/aiida-optimade/)<br>[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/aiida-optimade)](https://pypi.org/project/aiida-optimade/)<br>[![OPTIMADE](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/Materials-Consortia/optimade-python-tools/v0.24.1/optimade-version.json)](https://github.com/Materials-Consortia/OPTIMADE/) | [![GitHub Workflow Status](https://img.shields.io/github/workflow/status/aiidateam/aiida-optimade/aiida-optimade)](https://github.com/aiidateam/aiida-optimade/actions/)<br>[![Codecov](https://img.shields.io/codecov/c/gh/aiidateam/aiida-optimade)](https://codecov.io/gh/aiidateam/aiida-optimade) | [![GitHub last commit](https://img.shields.io/github/last-commit/aiidateam/aiida-optimade)](https://github.com/aiidateam/aiida-optimade) |
 
 This is a RESTful API server created with [FastAPI](https://fastapi.tiangolo.com/) that exposes an AiiDA database according to the [OPTIMADE specification](https://github.com/Materials-Consortia/OPTIMADE/blob/develop/optimade.rst).
 
 It is mainly used by [Materials Cloud](https://www.materialscloud.org/) to expose access to archived AiiDA databases through the OPTIMADE API.
 But it may be freely implemented by any to fulfill a similar purpose.
 
 The server is based on the test server "template" used in the [`optimade-python-tools`](https://github.com/Materials-Consortia/optimade-python-tools) package.
@@ -113,15 +113,15 @@
 
 ```shell
 $ aiida-optimade -p <PROFILE> init
 ```
 
 Where `<PROFILE>` is the AiiDA profile.
 
-> **Note**: Currently, the default is `optimade`, if the `-p / --profile` option is now specified.
+> **Note**: Currently, the default is `optimade`, if the `-p / --profile` option is not specified.
 > This will be changed in the future to use the default AiiDA profile.
 
 Initialization goes through your profile's `StructureData` nodes, adding an `optimade` extra, wherein all OPTIMADE-specific fields that do not have an equivalent AiiDA property are stored.
 
 If in the future, more `StructureData` nodes are added to your profile's database, these will be automatically updated for the first query, filtering on any of these OPTIMADE-specific fields.
 However, if you do not wish a significant lag for the user or risking several GET requests coming in at the same time, trying to update your profile's database, you should re-run `aiida-optimade init` for your profile (in between shutting the server down and restarting it again).
 
@@ -207,8 +207,8 @@
 
 [AiiDA v2 range]: https://img.shields.io/badge/AiiDA->=2.0.0,<3.0.0-007ec6.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACMAAAAhCAYAAABTERJSAAAABHNCSVQICAgIfAhkiAAAAAlwSFlzAAAFhgAABYYBG6Yz4AAAABl0RVh0U29mdHdhcmUAd3d3Lmlua3NjYXBlLm9yZ5vuPBoAAAUbSURBVFiFzZhrbFRVEMd%2Fc%2B5uu6UUbIFC%2FUAUVEQCLbQJBIiBDyiImJiIhmohYNCkqJAQxASLF8tDgYRHBLXRhIcKNtFEhVDgAxBJqgmVh4JEKg3EIn2QYqBlt917xg%2BFss%2ByaDHOtzsz5z%2B%2FuZl7ztmF%2F5HJvxVQN6cPYX8%2FPLnOmsvNAvqfwuib%2FbNIk9cQeQnLcKRL5xLIV%2Fic9eJeunjPYbRs4FjQSpTB3aS1IpRKeeOOewajy%2FKKEO8Q0DuVdKy8IqsbPulxGHUfCBBu%2BwUYGuFuBTK7wQnht6PEbf4tlRomVRjCbXNjQEB0AyrFQOL5ENIJm7dTLZE6DPJCnEtFZVXDLny%2B4Sjv0PmmYu1ZdUek9RiMgoDmJ8V0L7XJqsZ3UW8YsBOwEeHeeFce7jEYXBy0m9m4BbXqSj2%2Bxnkg26MCVrN6DEZcwggtd8pTFx%2Fh3B9B50YLaFOPwXQKUt0tBLegtSomfBlfY13PwijbEnhztGzgJsK5h9W9qeWwBqjvyhB2iBs1Qz0AU974DciRGO8CVN8AJhAeMAdA3KbrKEtvxhsI%2B9emWiJlGBEU680Cfk%2BSsVqXZvcFYGXjF8ABVJ%2BTNfVXehyms1zzn1gmIOxLEB6E31%2FWBe5rnCarmo7elf7dJEeaLh80GasliI5F6Q9cAz1GY1OJVNDxTzQTw7iY%2FHEZRQY7xqJ9RU2LFe%2FYqakdP911ha0XhjjiTVAkDwgatWfCGeYocx8M3glG8g8EXhSrLrHnEFJ5Ymow%2FkhIYv6ttYUW1iFmEqqxdVoUs9FmsDYSqmtmJh3Cl1%2BVtl2s7owDUdocR5bceiyoSivGTT5vzpbzL1uoBpmcAAQgW7ArnKD9ng9rc%2BNgrobSNwpSkkhcRN%2BvmXLjIsDovYHHEfmsYFygPAnIDEQrQPzJYCOaLHLUfIt7Oq0LJn9fxkSgNCb1qEIQ5UKgT%2Fs6gJmVOOroJhQBXVqw118QtWLdyUxEP45sUpSzqP7RDdFYMyB9UReMiF1MzPwoUqHt8hjGFFeP5wZAbZ%2F0%2BcAtAAcji6LeSq%2FMYiAvSsdw3GtrfVSVFUBbIhwRWYR7yOcr%2FBi%2FB1MSJZ16JlgH1AGM3EO2QnmMyrSbTSiACgFBv4yCUapZkt9qwWVL7aeOyHvArJjm8%2Fz9BhdI4XcZgz2%2FvRALosjsk1ODOyMcJn9%2FYI6IrkS5vxMGdUwou2YKfyVqJpn5t9aNs3gbQMbdbkxnGdsr4bTHm2AxWo9yNZK4PXR3uzhAh%2BM0AZejnCrGdy0UvJxl0oMKgWSLR%2B1LH2aE9ViejiFs%2BXn6bTjng3MlIhJ1I1TkuLdg6OcAbD7Xx%2Bc3y9TrWAiSHqVkbZ2v9ilCo6s4AjwZCzFyD9mOL305nV9aonvsQeT2L0gVk4OwOJqXXVRW7naaxswDKVdlYLyMXAnntteYmws2xcVVZzq%2BtHPAooQggmJkc6TLSusOiL4RKgwzzYU1iFQgiUBA1H7E8yPau%2BZl9P7AblVNebtHqTgxLfRqrNvZWjsHZFuqMqKcDWdlFjF7UGvX8Jn24DyEAykJwNcdg0OvJ4p5pQ9tV6SMlP4A0PNh8aYze1ArROyUNTNouy8tNF3Rt0CSXb6bRFl4%2FIfQzNMjaE9WwpYOWQnOdEF%2BTdJNO0iFh7%2BI0kfORzQZb6P2kymS9oTxzBiM9rUqLWr1WE5G6ODhycQd%2FUnNVeMbcH68hYkGycNoUNWc8fxaxfwhDbHpfwM5oeTY7rUX8QAAAABJRU5ErkJggg%3D%3D
 
 [AiiDA v1 range]: https://img.shields.io/badge/AiiDA->=1.6.0,<2.0.0-007ec6.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACMAAAAhCAYAAABTERJSAAAABHNCSVQICAgIfAhkiAAAAAlwSFlzAAAFhgAABYYBG6Yz4AAAABl0RVh0U29mdHdhcmUAd3d3Lmlua3NjYXBlLm9yZ5vuPBoAAAUbSURBVFiFzZhrbFRVEMd%2Fc%2B5uu6UUbIFC%2FUAUVEQCLbQJBIiBDyiImJiIhmohYNCkqJAQxASLF8tDgYRHBLXRhIcKNtFEhVDgAxBJqgmVh4JEKg3EIn2QYqBlt917xg%2BFss%2ByaDHOtzsz5z%2B%2FuZl7ztmF%2F5HJvxVQN6cPYX8%2FPLnOmsvNAvqfwuib%2FbNIk9cQeQnLcKRL5xLIV%2Fic9eJeunjPYbRs4FjQSpTB3aS1IpRKeeOOewajy%2FKKEO8Q0DuVdKy8IqsbPulxGHUfCBBu%2BwUYGuFuBTK7wQnht6PEbf4tlRomVRjCbXNjQEB0AyrFQOL5ENIJm7dTLZE6DPJCnEtFZVXDLny%2B4Sjv0PmmYu1ZdUek9RiMgoDmJ8V0L7XJqsZ3UW8YsBOwEeHeeFce7jEYXBy0m9m4BbXqSj2%2Bxnkg26MCVrN6DEZcwggtd8pTFx%2Fh3B9B50YLaFOPwXQKUt0tBLegtSomfBlfY13PwijbEnhztGzgJsK5h9W9qeWwBqjvyhB2iBs1Qz0AU974DciRGO8CVN8AJhAeMAdA3KbrKEtvxhsI%2B9emWiJlGBEU680Cfk%2BSsVqXZvcFYGXjF8ABVJ%2BTNfVXehyms1zzn1gmIOxLEB6E31%2FWBe5rnCarmo7elf7dJEeaLh80GasliI5F6Q9cAz1GY1OJVNDxTzQTw7iY%2FHEZRQY7xqJ9RU2LFe%2FYqakdP911ha0XhjjiTVAkDwgatWfCGeYocx8M3glG8g8EXhSrLrHnEFJ5Ymow%2FkhIYv6ttYUW1iFmEqqxdVoUs9FmsDYSqmtmJh3Cl1%2BVtl2s7owDUdocR5bceiyoSivGTT5vzpbzL1uoBpmcAAQgW7ArnKD9ng9rc%2BNgrobSNwpSkkhcRN%2BvmXLjIsDovYHHEfmsYFygPAnIDEQrQPzJYCOaLHLUfIt7Oq0LJn9fxkSgNCb1qEIQ5UKgT%2Fs6gJmVOOroJhQBXVqw118QtWLdyUxEP45sUpSzqP7RDdFYMyB9UReMiF1MzPwoUqHt8hjGFFeP5wZAbZ%2F0%2BcAtAAcji6LeSq%2FMYiAvSsdw3GtrfVSVFUBbIhwRWYR7yOcr%2FBi%2FB1MSJZ16JlgH1AGM3EO2QnmMyrSbTSiACgFBv4yCUapZkt9qwWVL7aeOyHvArJjm8%2Fz9BhdI4XcZgz2%2FvRALosjsk1ODOyMcJn9%2FYI6IrkS5vxMGdUwou2YKfyVqJpn5t9aNs3gbQMbdbkxnGdsr4bTHm2AxWo9yNZK4PXR3uzhAh%2BM0AZejnCrGdy0UvJxl0oMKgWSLR%2B1LH2aE9ViejiFs%2BXn6bTjng3MlIhJ1I1TkuLdg6OcAbD7Xx%2Bc3y9TrWAiSHqVkbZ2v9ilCo6s4AjwZCzFyD9mOL305nV9aonvsQeT2L0gVk4OwOJqXXVRW7naaxswDKVdlYLyMXAnntteYmws2xcVVZzq%2BtHPAooQggmJkc6TLSusOiL4RKgwzzYU1iFQgiUBA1H7E8yPau%2BZl9P7AblVNebtHqTgxLfRqrNvZWjsHZFuqMqKcDWdlFjF7UGvX8Jn24DyEAykJwNcdg0OvJ4p5pQ9tV6SMlP4A0PNh8aYze1ArROyUNTNouy8tNF3Rt0CSXb6bRFl4%2FIfQzNMjaE9WwpYOWQnOdEF%2BTdJNO0iFh7%2BI0kfORzQZb6P2kymS9oTxzBiM9rUqLWr1WE5G6ODhycQd%2FUnNVeMbcH68hYkGycNoUNWc8fxaxfwhDbHpfwM5oeTY7rUX8QAAAABJRU5ErkJggg%3D%3D
 
 [Python v3.7-v3.9]: https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9-blue
 
-[OPTIMADE from OPT]: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/Materials-Consortia/optimade-python-tools/v0.19.4/optimade-version.json
+[OPTIMADE from OPT]: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/Materials-Consortia/optimade-python-tools/v0.24.1/optimade-version.json
```

### Comparing `aiida-optimade-1.1.0/aiida_optimade.egg-info/SOURCES.txt` & `aiida-optimade-1.1.1/aiida_optimade.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aiida-optimade-1.1.0/profiles/config.j2` & `aiida-optimade-1.1.1/profiles/config.j2`

 * *Files identical despite different names*

### Comparing `aiida-optimade-1.1.0/profiles/docker-compose-mongo.j2` & `aiida-optimade-1.1.1/profiles/docker-compose-mongo.j2`

 * *Files 16% similar despite different names*

```diff
@@ -6,16 +6,16 @@
     restart: always
     depends_on:
       - mongo
     build:
       context: ..
       dockerfile: Dockerfile
       args:
-        OPTIMADE_TOOLS_VERSION: 0.19.4
-        AIIDA_VERSION: 2.0.4
+        OPTIMADE_TOOLS_VERSION: 0.24.1
+        AIIDA_VERSION: 2.3.1
         CONFIG_FILE: aiida_optimade/config.json
     environment:
       AIIDA_PATH: /app
       AIIDA_PROFILE: {{ aiida_profile }}
       FORCE_INIT: {{ force_init }}
       USE_MONGO: {{ use_mongo }}
       MONGO_FILENAME: {{ mongo_filename }}
```

### Comparing `aiida-optimade-1.1.0/profiles/docker-compose-mongo.yml` & `aiida-optimade-1.1.1/profiles/docker-compose-mongo.yml`

 * *Files 3% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 ---
 version: '3'
 
 services:
 
-    aiida-optimade:
-        restart: always
-        depends_on:
-            - mongo
-        build:
-            context: ..
-            dockerfile: Dockerfile
-            args:
-                OPTIMADE_TOOLS_VERSION: 0.19.4
-                AIIDA_VERSION: 2.0.4
-                CONFIG_FILE: aiida_optimade/config.json
-        environment:
-            AIIDA_PATH: /app
-            AIIDA_PROFILE: test_psql_dos
-            FORCE_INIT:
-            USE_MONGO:
-            MONGO_FILENAME:
-            AIIDA_OPTIMADE_LOG_LEVEL:
-            OPTIMADE_MONGO_URI: mongodb://mongo:27017
-        volumes:
-            - /tmp/test_repository_test_psql_dos:/app/.aiida/repository-quicksetup
-            - .:/profiles
-            - ../.github/mongo:/app/.mongo
-        ports:
-            - 3253:80
+  aiida-optimade:
+    restart: always
+    depends_on:
+    - mongo
+    build:
+      context: ..
+      dockerfile: Dockerfile
+      args:
+        OPTIMADE_TOOLS_VERSION: 0.24.1
+        AIIDA_VERSION: 2.3.1
+        CONFIG_FILE: aiida_optimade/config.json
+    environment:
+      AIIDA_PATH: /app
+      AIIDA_PROFILE: test_psql_dos
+      FORCE_INIT:
+      USE_MONGO:
+      MONGO_FILENAME:
+      AIIDA_OPTIMADE_LOG_LEVEL:
+      OPTIMADE_MONGO_URI: mongodb://mongo:27017
+    volumes:
+    - /tmp/test_repository_test_psql_dos:/app/.aiida/repository-quicksetup
+    - .:/profiles
+    - ../.github/mongo:/app/.mongo
+    ports:
+    - 3253:80
     # Extra field ONLY for use with GitHub Actions CI
-        extra_hosts:
-            - docker.host.internal:${DOCKER_HOST_IP}
-        networks:
-            - optimade
+    extra_hosts:
+    - docker.host.internal:${DOCKER_HOST_IP}
+    networks:
+    - optimade
 
-    mongo:
-        restart: always
-        image: mongo:4
-        networks:
-            - optimade
+  mongo:
+    restart: always
+    image: mongo:4
+    networks:
+    - optimade
 
 networks:
-    optimade:
+  optimade:
```

### Comparing `aiida-optimade-1.1.0/profiles/docker-compose.j2` & `aiida-optimade-1.1.1/profiles/docker-compose.j2`

 * *Files 3% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
   aiida-optimade-{{ aiida_profile }}:
     restart: always
     build:
       context: ..
       dockerfile: Dockerfile
       args:
-        OPTIMADE_TOOLS_VERSION: 0.19.4
-        AIIDA_VERSION: 2.0.4
+        OPTIMADE_TOOLS_VERSION: 0.24.1
+        AIIDA_VERSION: 2.3.1
         CONFIG_FILE: aiida_optimade/config.json
     environment:
       AIIDA_PATH: /app
       AIIDA_PROFILE: {{ aiida_profile }}
       FORCE_INIT: {{ force_init }}
       USE_MONGO: {{ use_mongo }}
       MONGO_FILENAME: {{ mongo_filename }}
```

### Comparing `aiida-optimade-1.1.0/profiles/docker-compose.yml` & `aiida-optimade-1.1.1/profiles/docker-compose.yml`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 ---
 version: '3'
 
 services:
 
-    aiida-optimade:
-        restart: always
-        build:
-            context: ..
-            dockerfile: Dockerfile
-            args:
-                OPTIMADE_TOOLS_VERSION: 0.19.4
-                AIIDA_VERSION: 2.0.4
-                CONFIG_FILE: aiida_optimade/config.json
-        environment:
-            AIIDA_PATH: /app
-            AIIDA_PROFILE: test_psql_dos
-            FORCE_INIT:
-            USE_MONGO:
-            MONGO_FILENAME:
-            AIIDA_OPTIMADE_LOG_LEVEL:
-        volumes:
-            - /tmp/test_repository_test_psql_dos:/app/.aiida/repository-quicksetup
-            - .:/profiles
-            - ../.github/mongo:/app/.mongo
-        ports:
-            - 3253:80
+  aiida-optimade:
+    restart: always
+    build:
+      context: ..
+      dockerfile: Dockerfile
+      args:
+        OPTIMADE_TOOLS_VERSION: 0.24.1
+        AIIDA_VERSION: 2.3.1
+        CONFIG_FILE: aiida_optimade/config.json
+    environment:
+      AIIDA_PATH: /app
+      AIIDA_PROFILE: test_psql_dos
+      FORCE_INIT:
+      USE_MONGO:
+      MONGO_FILENAME:
+      AIIDA_OPTIMADE_LOG_LEVEL:
+    volumes:
+    - /tmp/test_repository_test_psql_dos:/app/.aiida/repository-quicksetup
+    - .:/profiles
+    - ../.github/mongo:/app/.mongo
+    ports:
+    - 3253:80
     # Extra field ONLY for use with GitHub Actions CI
-        extra_hosts:
-            - docker.host.internal:${DOCKER_HOST_IP}
+    extra_hosts:
+    - docker.host.internal:${DOCKER_HOST_IP}
```

### Comparing `aiida-optimade-1.1.0/profiles/test_psql_dos.json` & `aiida-optimade-1.1.1/profiles/test_psql_dos.json`

 * *Files identical despite different names*

### Comparing `aiida-optimade-1.1.0/setup.json` & `aiida-optimade-1.1.1/setup.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.95%*

 * *Differences: {"'version'": "'1.1.1'"}*

```diff
@@ -24,9 +24,9 @@
     ],
     "description": "Expose an AiiDA database according to the [OPTIMADE API specification](https://www.optimade.org).",
     "include_package_data": true,
     "keywords": "optimade aiida materials",
     "license": "MIT License",
     "name": "aiida-optimade",
     "url": "https://github.com/aiidateam/aiida-optimade",
-    "version": "1.1.0"
+    "version": "1.1.1"
 }
```

### Comparing `aiida-optimade-1.1.0/setup.py` & `aiida-optimade-1.1.1/setup.py`

 * *Files identical despite different names*

