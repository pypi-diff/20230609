# Comparing `tmp/ninia-0.0.82.tar.gz` & `tmp/ninia-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ninia-0.0.82.tar", last modified: Fri Jun  9 19:17:38 2023, max compression
+gzip compressed data, was "C:\Users\ajs0201\PycharmProjects\ninia\dist\tmpx63x1vgh\ninia-0.0.9.tar", last modified: Tue Jun 22 23:39:30 2021, max compression
```

## Comparing `ninia-0.0.82.tar` & `ninia-0.0.9.tar`

### file list

```diff
@@ -1,32 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 19:17:38.538451 ninia-0.0.82/
--rw-rw-rw-   0        0        0     1088 2021-06-21 22:31:41.000000 ninia-0.0.82/LICENSE
--rw-rw-rw-   0        0        0      109 2022-11-03 20:23:15.000000 ninia-0.0.82/MANIFEST.in
--rw-rw-rw-   0        0        0     4292 2023-06-09 19:17:38.538451 ninia-0.0.82/PKG-INFO
--rw-rw-rw-   0        0        0     3715 2021-11-17 16:23:10.000000 ninia-0.0.82/README.md
-drwxrwxrwx   0        0        0        0 2023-06-09 19:17:38.520500 ninia-0.0.82/ninia/
--rw-rw-rw-   0        0        0      403 2023-06-09 19:17:31.000000 ninia-0.0.82/ninia/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-09 19:17:38.527480 ninia-0.0.82/ninia/data/
--rw-rw-rw-   0        0        0     1402 2021-06-23 18:18:53.000000 ninia-0.0.82/ninia/data/mm_of_elements.csv
--rw-rw-rw-   0        0        0       45 2021-06-21 21:47:30.000000 ninia-0.0.82/ninia/example.py
-drwxrwxrwx   0        0        0        0 2023-06-09 19:17:38.536457 ninia-0.0.82/ninia/input/
--rw-rw-rw-   0        0        0      546 2023-06-07 02:45:26.000000 ninia-0.0.82/ninia/input/SISSO.in.jinja2
--rw-rw-rw-   0        0        0      597 2023-06-07 20:42:24.000000 ninia-0.0.82/ninia/input/SISSO_job.sh.jinja2
--rw-rw-rw-   0        0        0      340 2022-01-06 21:11:51.000000 ninia-0.0.82/ninia/input/pbs.sh
--rw-rw-rw-   0        0        0      869 2022-09-14 22:17:01.000000 ninia-0.0.82/ninia/input/relax.i
--rw-rw-rw-   0        0        0     5702 2023-05-25 22:05:57.000000 ninia-0.0.82/ninia/input/relax.jinja2
--rw-rw-rw-   0        0        0      723 2022-11-04 20:23:11.000000 ninia-0.0.82/ninia/input/slurm.jinja2
--rw-rw-rw-   0        0        0      544 2022-09-14 22:15:09.000000 ninia-0.0.82/ninia/input/slurm.sh
--rw-rw-rw-   0        0        0     1995 2021-06-22 20:18:25.000000 ninia-0.0.82/ninia/mw_species_.py
--rw-rw-rw-   0        0        0    11959 2022-11-04 02:15:58.000000 ninia-0.0.82/ninia/old_relax.py
--rw-rw-rw-   0        0        0     1434 2021-11-17 22:57:21.000000 ninia-0.0.82/ninia/output.py
--rw-rw-rw-   0        0        0     7750 2023-05-10 19:42:47.000000 ninia-0.0.82/ninia/relax.py
--rw-rw-rw-   0        0        0     4131 2023-06-09 19:12:01.000000 ninia-0.0.82/ninia/sisso.py
--rw-rw-rw-   0        0        0     9122 2023-06-09 19:17:31.000000 ninia-0.0.82/ninia/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-09 19:17:38.526484 ninia-0.0.82/ninia.egg-info/
--rw-rw-rw-   0        0        0     4292 2023-06-09 19:17:38.000000 ninia-0.0.82/ninia.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      505 2023-06-09 19:17:38.000000 ninia-0.0.82/ninia.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 19:17:38.000000 ninia-0.0.82/ninia.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-09 19:17:38.000000 ninia-0.0.82/ninia.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      111 2021-06-21 21:53:26.000000 ninia-0.0.82/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-09 19:17:38.539449 ninia-0.0.82/setup.cfg
--rw-rw-rw-   0        0        0      837 2023-06-09 19:17:31.000000 ninia-0.0.82/setup.py
+drwxrwxrwx   0        0        0        0 2021-06-22 23:39:30.060138 ninia-0.0.9/
+-rw-rw-rw-   0        0        0     1088 2021-06-21 22:31:41.000000 ninia-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0      718 2021-06-22 23:39:30.060138 ninia-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      142 2021-06-21 22:29:54.000000 ninia-0.0.9/README.md
+-rw-rw-rw-   0        0        0      111 2021-06-21 21:53:26.000000 ninia-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2021-06-22 23:39:30.060138 ninia-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      939 2021-06-22 23:37:45.000000 ninia-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2021-06-22 23:39:30.046175 ninia-0.0.9/src/
+drwxrwxrwx   0        0        0        0 2021-06-22 23:39:30.054154 ninia-0.0.9/src/ninia/
+-rw-rw-rw-   0        0        0        0 2021-06-21 21:45:05.000000 ninia-0.0.9/src/ninia/__init__.py
+-rw-rw-rw-   0        0        0       45 2021-06-21 21:47:30.000000 ninia-0.0.9/src/ninia/example.py
+-rw-rw-rw-   0        0        0     1995 2021-06-22 20:18:25.000000 ninia-0.0.9/src/ninia/mw_species_.py
+-rw-rw-rw-   0        0        0    11220 2021-06-22 23:37:45.000000 ninia-0.0.9/src/ninia/relax.py
+drwxrwxrwx   0        0        0        0 2021-06-22 23:39:30.059143 ninia-0.0.9/src/ninia.egg-info/
+-rw-rw-rw-   0        0        0      718 2021-06-22 23:39:30.000000 ninia-0.0.9/src/ninia.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      260 2021-06-22 23:39:30.000000 ninia-0.0.9/src/ninia.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2021-06-22 23:39:30.000000 ninia-0.0.9/src/ninia.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2021-06-22 23:39:30.000000 ninia-0.0.9/src/ninia.egg-info/top_level.txt
```

### Comparing `ninia-0.0.82/LICENSE` & `ninia-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ninia-0.0.82/ninia/mw_species_.py` & `ninia-0.0.9/src/ninia/mw_species_.py`

 * *Files identical despite different names*

