# Comparing `tmp/pyreason-1.5.3.tar.gz` & `tmp/pyreason-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyreason-1.5.3.tar", last modified: Sun May 21 04:55:18 2023, max compression
+gzip compressed data, was "pyreason-1.6.0.tar", last modified: Fri Jun  9 19:05:35 2023, max compression
```

## Comparing `pyreason-1.5.3.tar` & `pyreason-1.6.0.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:55:18.832931 pyreason-1.5.3/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1493 2023-05-21 04:55:07.000000 pyreason-1.5.3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-21 04:55:07.000000 pyreason-1.5.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-05-21 04:55:18.832931 pyreason-1.5.3/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     3261 2023-05-21 04:55:07.000000 pyreason-1.5.3/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)       85 2023-05-21 04:55:07.000000 pyreason-1.5.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:55:18.824931 pyreason-1.5.3/pyreason/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-21 04:55:07.000000 pyreason-1.5.3/pyreason/.cache_status.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1307 2023-05-21 04:55:07.000000 pyreason-1.5.3/pyreason/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:55:18.824931 pyreason-1.5.3/pyreason/examples/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:55:07.000000 pyreason-1.5.3/pyreason/examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:55:18.824931 pyreason-1.5.3/pyreason/examples/hello-world/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2646 2023-05-21 04:55:07.000000 pyreason-1.5.3/pyreason/examples/hello-world/facts.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1406 2023-05-21 04:55:07.000000 pyreason-1.5.3/pyreason/examples/hello-world/friends.graphml
--rwxr-xr-x   0 runner    (1001) docker     (123)       13 2023-05-21 04:55:07.000000 pyreason-1.5.3/pyreason/examples/hello-world/ipl.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)      302 2023-05-21 04:55:07.000000 pyreason-1.5.3/pyreason/examples/hello-world/labels.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1048 2023-05-21 04:55:07.000000 pyreason-1.5.3/pyreason/examples/hello-world/rules.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)    27121 2023-05-21 04:55:07.000000 pyreason-1.5.3/pyreason/pyreason.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:55:18.828931 pyreason-1.5.3/pyreason/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:55:07.000000 pyreason-1.5.3/pyreason/scripts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:55:18.828931 pyreason-1.5.3/pyreason/scripts/annotation_functions/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:55:07.000000 pyreason-1.5.3/pyreason/scripts/annotation_functions/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3398 2023-05-21 04:55:07.000000 pyreason-1.5.3/pyreason/scripts/annotation_functions/annotation_functions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6555 2023-05-21 04:55:07.000000 pyreason-1.5.3/pyreason/scripts/args.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:55:18.828931 pyreason-1.5.3/pyreason/scripts/components/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:55:07.000000 pyreason-1.5.3/pyreason/scripts/components/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      431 2023-05-21 04:55:07.000000 pyreason-1.5.3/pyreason/scripts/components/label.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1356 2023-05-21 04:55:07.000000 pyreason-1.5.3/pyreason/scripts/components/world.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4655 2023-05-21 04:55:07.000000 pyreason-1.5.3/pyreason/scripts/diffuse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:55:18.828931 pyreason-1.5.3/pyreason/scripts/facts/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:55:07.000000 pyreason-1.5.3/pyreason/scripts/facts/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1014 2023-05-21 04:55:07.000000 pyreason-1.5.3/pyreason/scripts/facts/fact_edge.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1014 2023-05-21 04:55:07.000000 pyreason-1.5.3/pyreason/scripts/facts/fact_node.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:55:18.828931 pyreason-1.5.3/pyreason/scripts/interpretation/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:55:07.000000 pyreason-1.5.3/pyreason/scripts/interpretation/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    71082 2023-05-21 04:55:07.000000 pyreason-1.5.3/pyreason/scripts/interpretation/interpretation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:55:18.828931 pyreason-1.5.3/pyreason/scripts/interval/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:55:07.000000 pyreason-1.5.3/pyreason/scripts/interval/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1897 2023-05-21 04:55:07.000000 pyreason-1.5.3/pyreason/scripts/interval/interval.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:55:18.828931 pyreason-1.5.3/pyreason/scripts/numba_wrapper/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:55:07.000000 pyreason-1.5.3/pyreason/scripts/numba_wrapper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:55:18.828931 pyreason-1.5.3/pyreason/scripts/numba_wrapper/numba_types/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:55:07.000000 pyreason-1.5.3/pyreason/scripts/numba_wrapper/numba_types/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6241 2023-05-21 04:55:07.000000 pyreason-1.5.3/pyreason/scripts/numba_wrapper/numba_types/fact_edge_type.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6015 2023-05-21 04:55:07.000000 pyreason-1.5.3/pyreason/scripts/numba_wrapper/numba_types/fact_node_type.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4186 2023-05-21 04:55:07.000000 pyreason-1.5.3/pyreason/scripts/numba_wrapper/numba_types/interval_type.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2933 2023-05-21 04:55:07.000000 pyreason-1.5.3/pyreason/scripts/numba_wrapper/numba_types/label_type.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10909 2023-05-21 04:55:07.000000 pyreason-1.5.3/pyreason/scripts/numba_wrapper/numba_types/rule_type.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4779 2023-05-21 04:55:07.000000 pyreason-1.5.3/pyreason/scripts/numba_wrapper/numba_types/world_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:55:18.828931 pyreason-1.5.3/pyreason/scripts/program/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:55:07.000000 pyreason-1.5.3/pyreason/scripts/program/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1894 2023-05-21 04:55:07.000000 pyreason-1.5.3/pyreason/scripts/program/program.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:55:18.828931 pyreason-1.5.3/pyreason/scripts/rules/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:55:07.000000 pyreason-1.5.3/pyreason/scripts/rules/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1251 2023-05-21 04:55:07.000000 pyreason-1.5.3/pyreason/scripts/rules/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:55:18.832931 pyreason-1.5.3/pyreason/scripts/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 04:55:07.000000 pyreason-1.5.3/pyreason/scripts/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4564 2023-05-21 04:55:07.000000 pyreason-1.5.3/pyreason/scripts/utils/filter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4233 2023-05-21 04:55:07.000000 pyreason-1.5.3/pyreason/scripts/utils/graphml_parser.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3375 2023-05-21 04:55:07.000000 pyreason-1.5.3/pyreason/scripts/utils/output.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2763 2023-05-21 04:55:07.000000 pyreason-1.5.3/pyreason/scripts/utils/plotter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      834 2023-05-21 04:55:07.000000 pyreason-1.5.3/pyreason/scripts/utils/visuals.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9058 2023-05-21 04:55:07.000000 pyreason-1.5.3/pyreason/scripts/utils/yaml_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:55:18.824931 pyreason-1.5.3/pyreason.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-05-21 04:55:18.000000 pyreason-1.5.3/pyreason.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-05-21 04:55:18.000000 pyreason-1.5.3/pyreason.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 04:55:18.000000 pyreason-1.5.3/pyreason.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-21 04:55:18.000000 pyreason-1.5.3/pyreason.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-21 04:55:18.000000 pyreason-1.5.3/pyreason.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 04:55:18.832931 pyreason-1.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-21 04:55:07.000000 pyreason-1.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:05:35.979748 pyreason-1.6.0/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1493 2023-06-09 19:05:20.000000 pyreason-1.6.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-09 19:05:20.000000 pyreason-1.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-06-09 19:05:35.979748 pyreason-1.6.0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3261 2023-06-09 19:05:20.000000 pyreason-1.6.0/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)       85 2023-06-09 19:05:20.000000 pyreason-1.6.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:05:35.967748 pyreason-1.6.0/pyreason/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-09 19:05:20.000000 pyreason-1.6.0/pyreason/.cache_status.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1307 2023-06-09 19:05:20.000000 pyreason-1.6.0/pyreason/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:05:35.971747 pyreason-1.6.0/pyreason/examples/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:05:20.000000 pyreason-1.6.0/pyreason/examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:05:35.971747 pyreason-1.6.0/pyreason/examples/hello-world/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2646 2023-06-09 19:05:20.000000 pyreason-1.6.0/pyreason/examples/hello-world/facts.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1406 2023-06-09 19:05:20.000000 pyreason-1.6.0/pyreason/examples/hello-world/friends.graphml
+-rwxr-xr-x   0 runner    (1001) docker     (123)       13 2023-06-09 19:05:20.000000 pyreason-1.6.0/pyreason/examples/hello-world/ipl.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      302 2023-06-09 19:05:20.000000 pyreason-1.6.0/pyreason/examples/hello-world/labels.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1048 2023-06-09 19:05:20.000000 pyreason-1.6.0/pyreason/examples/hello-world/rules.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)    28797 2023-06-09 19:05:20.000000 pyreason-1.6.0/pyreason/pyreason.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:05:35.971747 pyreason-1.6.0/pyreason/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:05:20.000000 pyreason-1.6.0/pyreason/scripts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:05:35.971747 pyreason-1.6.0/pyreason/scripts/annotation_functions/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:05:20.000000 pyreason-1.6.0/pyreason/scripts/annotation_functions/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3398 2023-06-09 19:05:20.000000 pyreason-1.6.0/pyreason/scripts/annotation_functions/annotation_functions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6555 2023-06-09 19:05:20.000000 pyreason-1.6.0/pyreason/scripts/args.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:05:35.971747 pyreason-1.6.0/pyreason/scripts/components/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:05:20.000000 pyreason-1.6.0/pyreason/scripts/components/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      431 2023-06-09 19:05:20.000000 pyreason-1.6.0/pyreason/scripts/components/label.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1356 2023-06-09 19:05:20.000000 pyreason-1.6.0/pyreason/scripts/components/world.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4655 2023-06-09 19:05:20.000000 pyreason-1.6.0/pyreason/scripts/diffuse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:05:35.975748 pyreason-1.6.0/pyreason/scripts/facts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:05:20.000000 pyreason-1.6.0/pyreason/scripts/facts/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1014 2023-06-09 19:05:20.000000 pyreason-1.6.0/pyreason/scripts/facts/fact_edge.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1014 2023-06-09 19:05:20.000000 pyreason-1.6.0/pyreason/scripts/facts/fact_node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:05:35.975748 pyreason-1.6.0/pyreason/scripts/interpretation/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:05:20.000000 pyreason-1.6.0/pyreason/scripts/interpretation/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    66970 2023-06-09 19:05:20.000000 pyreason-1.6.0/pyreason/scripts/interpretation/interpretation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:05:35.975748 pyreason-1.6.0/pyreason/scripts/interval/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:05:20.000000 pyreason-1.6.0/pyreason/scripts/interval/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1897 2023-06-09 19:05:20.000000 pyreason-1.6.0/pyreason/scripts/interval/interval.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:05:35.975748 pyreason-1.6.0/pyreason/scripts/numba_wrapper/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:05:20.000000 pyreason-1.6.0/pyreason/scripts/numba_wrapper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:05:35.975748 pyreason-1.6.0/pyreason/scripts/numba_wrapper/numba_types/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:05:20.000000 pyreason-1.6.0/pyreason/scripts/numba_wrapper/numba_types/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6241 2023-06-09 19:05:20.000000 pyreason-1.6.0/pyreason/scripts/numba_wrapper/numba_types/fact_edge_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6015 2023-06-09 19:05:20.000000 pyreason-1.6.0/pyreason/scripts/numba_wrapper/numba_types/fact_node_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4186 2023-06-09 19:05:20.000000 pyreason-1.6.0/pyreason/scripts/numba_wrapper/numba_types/interval_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2933 2023-06-09 19:05:20.000000 pyreason-1.6.0/pyreason/scripts/numba_wrapper/numba_types/label_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10909 2023-06-09 19:05:20.000000 pyreason-1.6.0/pyreason/scripts/numba_wrapper/numba_types/rule_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4779 2023-06-09 19:05:20.000000 pyreason-1.6.0/pyreason/scripts/numba_wrapper/numba_types/world_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:05:35.975748 pyreason-1.6.0/pyreason/scripts/program/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:05:20.000000 pyreason-1.6.0/pyreason/scripts/program/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2028 2023-06-09 19:05:20.000000 pyreason-1.6.0/pyreason/scripts/program/program.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:05:35.975748 pyreason-1.6.0/pyreason/scripts/rules/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:05:20.000000 pyreason-1.6.0/pyreason/scripts/rules/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1251 2023-06-09 19:05:20.000000 pyreason-1.6.0/pyreason/scripts/rules/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:05:35.979748 pyreason-1.6.0/pyreason/scripts/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 19:05:20.000000 pyreason-1.6.0/pyreason/scripts/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4564 2023-06-09 19:05:20.000000 pyreason-1.6.0/pyreason/scripts/utils/filter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4233 2023-06-09 19:05:20.000000 pyreason-1.6.0/pyreason/scripts/utils/graphml_parser.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3375 2023-06-09 19:05:20.000000 pyreason-1.6.0/pyreason/scripts/utils/output.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2763 2023-06-09 19:05:20.000000 pyreason-1.6.0/pyreason/scripts/utils/plotter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      834 2023-06-09 19:05:20.000000 pyreason-1.6.0/pyreason/scripts/utils/visuals.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9058 2023-06-09 19:05:20.000000 pyreason-1.6.0/pyreason/scripts/utils/yaml_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:05:35.971747 pyreason-1.6.0/pyreason.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-06-09 19:05:35.000000 pyreason-1.6.0/pyreason.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-06-09 19:05:35.000000 pyreason-1.6.0/pyreason.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 19:05:35.000000 pyreason-1.6.0/pyreason.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-09 19:05:35.000000 pyreason-1.6.0/pyreason.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-09 19:05:35.000000 pyreason-1.6.0/pyreason.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 19:05:35.979748 pyreason-1.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-06-09 19:05:20.000000 pyreason-1.6.0/setup.py
```

### Comparing `pyreason-1.5.3/LICENSE.md` & `pyreason-1.6.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyreason-1.5.3/PKG-INFO` & `pyreason-1.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyreason
-Version: 1.5.3
+Version: 1.6.0
 Summary: An explainable inference software supporting annotated, real valued, graph based and temporal logic
 Home-page: https://github.com/lab-v2/pyreason
 Author: Dyuman Aditya
 Author-email: dyuman.aditya@gmail.com
 License: BSD 3-clause
 Project-URL: Bug Tracker, https://github.com/lab-v2/pyreason/issues
 Project-URL: Repository, https://github.com/lab-v2/pyreason
```

### Comparing `pyreason-1.5.3/README.md` & `pyreason-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `pyreason-1.5.3/pyreason/__init__.py` & `pyreason-1.6.0/pyreason/__init__.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.5.3/pyreason/examples/hello-world/facts.yaml` & `pyreason-1.6.0/pyreason/examples/hello-world/facts.yaml`

 * *Files identical despite different names*

### Comparing `pyreason-1.5.3/pyreason/examples/hello-world/friends.graphml` & `pyreason-1.6.0/pyreason/examples/hello-world/friends.graphml`

 * *Files identical despite different names*

### Comparing `pyreason-1.5.3/pyreason/examples/hello-world/rules.yaml` & `pyreason-1.6.0/pyreason/examples/hello-world/rules.yaml`

 * *Files identical despite different names*

### Comparing `pyreason-1.5.3/pyreason/pyreason.py` & `pyreason-1.6.0/pyreason/pyreason.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,14 +30,15 @@
         self.__memory_profile = False
         self.__reverse_digraph = False
         self.__atom_trace = False
         self.__save_graph_attributes_to_trace = False
         self.__canonical = False
         self.__inconsistency_check = True
         self.__static_graph_facts = True
+        self.__store_interpretation_changes = True
 
     @property
     def verbose(self) -> bool:
         """Returns whether verbose mode is on or not. Default is True
 
         :return: bool
         """
@@ -130,14 +131,23 @@
     def static_graph_facts(self) -> bool:
         """Returns whether to make graph facts static or not. Default is True
 
         :return: bool
         """
         return self.__static_graph_facts
 
+    @property
+    def store_interpretation_changes(self) -> bool:
+        """Returns whether to keep track of changes that occur in the interpretation. You will not be able to view
+        interpretation results after reasoning. Default is True
+
+        :return: bool
+        """
+        return self.__store_interpretation_changes
+
     @verbose.setter
     def verbose(self, value: bool) -> None:
         """Set verbose mode. Default is True
 
         :param value: verbose or not
         :raises TypeError: If not boolean, raise error
         """
@@ -278,14 +288,27 @@
         :raises TypeError: If not bool raise error
         """
         if not isinstance(value, bool):
             raise TypeError('value has to be a bool')
         else:
             self.__static_graph_facts = value
 
+    @store_interpretation_changes.setter
+    def store_interpretation_changes(self, value: bool) -> None:
+        """Whether to keep track of changes that occur to the interpretation. You will not be able to view interpretation
+        results after reasoning.
+
+        :param value: Whether to make graphml facts static or not
+        :raises TypeError: If not bool raise error
+        """
+        if not isinstance(value, bool):
+            raise TypeError('value has to be a bool')
+        else:
+            self.__store_interpretation_changes = value
+
 
 # VARIABLES
 __graph = None
 __rules = None
 __node_facts = None
 __edge_facts = None
 __ipl = None
@@ -564,16 +587,20 @@
             __specific_edge_labels[label_name] = edges
 
     all_node_facts = numba.typed.List(__node_facts)
     all_edge_facts = numba.typed.List(__edge_facts)
     all_node_facts.extend(__non_fluent_graph_facts_node)
     all_edge_facts.extend(__non_fluent_graph_facts_edge)
 
+    # Atom trace cannot be true when store interpretations is false
+    if not settings.store_interpretation_changes:
+        settings.atom_trace = False
+
     # Setup logical program
-    __program = Program(__graph, all_node_facts, all_edge_facts, __rules, __ipl, settings.reverse_digraph, settings.atom_trace, settings.save_graph_attributes_to_trace, settings.canonical, settings.inconsistency_check)
+    __program = Program(__graph, all_node_facts, all_edge_facts, __rules, __ipl, settings.reverse_digraph, settings.atom_trace, settings.save_graph_attributes_to_trace, settings.canonical, settings.inconsistency_check, settings.store_interpretation_changes)
     __program.available_labels_node = __node_labels
     __program.available_labels_edge = __edge_labels
     __program.specific_node_labels = __specific_node_labels
     __program.specific_edge_labels = __specific_edge_labels
 
     # Run Program and get final interpretation
     interpretation = __program.reason(timesteps, convergence_threshold, convergence_bound_threshold, settings.verbose)
@@ -584,34 +611,38 @@
 def _reason_again(timesteps, convergence_threshold, convergence_bound_threshold, node_facts, edge_facts):
     # Globals
     global __graph, __rules, __node_facts, __edge_facts, __ipl, __node_labels, __edge_labels, __specific_node_labels, __specific_edge_labels, __graphml_parser
     global settings, __timestamp, __program
 
     assert __program is not None, 'To run `reason_again` you need to have reasoned once before'
 
-    # Extend current set of nodes with the new nodes supplied
+    # Extend current set of facts with the new facts supplied
+    all_edge_facts = numba.typed.List.empty_list(fact_edge.fact_type)
+    all_node_facts = numba.typed.List.empty_list(fact_node.fact_type)
     if node_facts is not None:
-        __node_facts.extend(numba.typed.List(node_facts))
+        all_node_facts.extend(numba.typed.List(node_facts))
     if edge_facts is not None:
-        __edge_facts.extend(numba.typed.List(edge_facts))
+        all_edge_facts.extend(numba.typed.List(edge_facts))
 
     # Run Program and get final interpretation
-    interpretation = __program.reason_again(timesteps, convergence_threshold, convergence_bound_threshold, __node_facts, __edge_facts, settings.verbose)
+    interpretation = __program.reason_again(timesteps, convergence_threshold, convergence_bound_threshold, all_node_facts, all_edge_facts, settings.verbose)
 
     return interpretation
 
 
 def save_rule_trace(interpretation, folder: str='./'):
     """Saves the trace of the program. This includes every change that has occured to the interpretation. If `atom_trace` was set to true
     this gives us full explainability of why interpretations changed
 
     :param interpretation: the output of `pyreason.reason()`, the final interpretation
     :param folder: the folder in which to save the result, defaults to './'
     """
-    global __timestamp
+    global __timestamp, settings
+
+    assert settings.store_interpretation_changes, 'store interpretation changes setting is off, turn on to save rule trace'
 
     output = Output(__timestamp)
     output.save_rule_trace(interpretation, folder)
 
 
 def filter_and_sort_nodes(interpretation, labels: List[str], bound: interval.Interval=interval.closed(0,1), sort_by: str='lower', descending: bool=True):
     """Filters and sorts the node changes in the interpretation and returns as a list of Pandas dataframes that are easy to access
@@ -619,14 +650,15 @@
     :param interpretation: the output of `pyreason.reason()`, the final interpretation
     :param labels: A list of strings, labels that are in the interpretation that are to be filtered
     :param bound: The bound that will filter any interpretation that is not in it. the default does not filter anything, defaults to interval.closed(0,1)
     :param sort_by: String that is either 'lower' or 'upper', sorts by the lower/upper bound, defaults to 'lower'
     :param descending: A bool that sorts by descending/ascending order, defaults to True
     :return: A list of Pandas dataframes that contain the filtered and sorted interpretations that are easy to access
     """
+    assert settings.store_interpretation_changes, 'store interpretation changes setting is off, turn on to filter and sort nodes'
     filterer = Filter(interpretation.time)
     filtered_df = filterer.filter_and_sort_nodes(interpretation, labels, bound, sort_by, descending)
     return filtered_df
 
 
 def filter_and_sort_edges(interpretation, labels: List[str], bound: interval.Interval=interval.closed(0,1), sort_by: str='lower', descending: bool=True):
     """Filters and sorts the edge changes in the interpretation and returns as a list of Pandas dataframes that are easy to access
@@ -634,10 +666,11 @@
     :param interpretation: the output of `pyreason.reason()`, the final interpretation
     :param labels: A list of strings, labels that are in the interpretation that are to be filtered
     :param bound: The bound that will filter any interpretation that is not in it. the default does not filter anything, defaults to interval.closed(0,1)
     :param sort_by: String that is either 'lower' or 'upper', sorts by the lower/upper bound, defaults to 'lower'
     :param descending: A bool that sorts by descending/ascending order, defaults to True
     :return: A list of Pandas dataframes that contain the filtered and sorted interpretations that are easy to access
     """
+    assert settings.store_interpretation_changes, 'store interpretation changes setting is off, turn on to filter and sort edges'
     filterer = Filter(interpretation.time)
     filtered_df = filterer.filter_and_sort_edges(interpretation, labels, bound, sort_by, descending)
     return filtered_df
```

### Comparing `pyreason-1.5.3/pyreason/scripts/annotation_functions/annotation_functions.py` & `pyreason-1.6.0/pyreason/scripts/annotation_functions/annotation_functions.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.5.3/pyreason/scripts/args.py` & `pyreason-1.6.0/pyreason/scripts/args.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.5.3/pyreason/scripts/components/world.py` & `pyreason-1.6.0/pyreason/scripts/components/world.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.5.3/pyreason/scripts/diffuse.py` & `pyreason-1.6.0/pyreason/scripts/diffuse.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.5.3/pyreason/scripts/facts/fact_edge.py` & `pyreason-1.6.0/pyreason/scripts/facts/fact_edge.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.5.3/pyreason/scripts/facts/fact_node.py` & `pyreason-1.6.0/pyreason/scripts/facts/fact_node.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.5.3/pyreason/scripts/interpretation/interpretation.py` & `pyreason-1.6.0/pyreason/scripts/interpretation/interpretation.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,22 +20,23 @@
 
 class Interpretation:
 	available_labels_node = []
 	available_labels_edge = []
 	specific_node_labels = numba.typed.Dict.empty(key_type=label.label_type, value_type=numba.types.ListType(node_type))
 	specific_edge_labels = numba.typed.Dict.empty(key_type=label.label_type, value_type=numba.types.ListType(edge_type))
 
-	def __init__(self, graph, ipl, reverse_graph, atom_trace, save_graph_attributes_to_rule_trace, canonical, inconsistency_check):
+	def __init__(self, graph, ipl, reverse_graph, atom_trace, save_graph_attributes_to_rule_trace, canonical, inconsistency_check, store_interpretation_changes):
 		self.graph = graph
 		self.ipl = ipl
 		self.reverse_graph = reverse_graph
 		self.atom_trace = atom_trace
 		self.save_graph_attributes_to_rule_trace = save_graph_attributes_to_rule_trace
 		self.canonical = canonical
 		self.inconsistency_check = inconsistency_check
+		self.store_interpretation_changes = store_interpretation_changes
 
 		# For reasoning and reasoning again (contains previous time and previous fp operation cnt)
 		self.time = 0
 		self.prev_reasoning_data = numba.typed.List([0, 0])
 
 		# Initialize list of tuples for rules/facts to be applied, along with all the ground atoms that fired the rule. One to One correspondence between rules_to_be_applied_node and rules_to_be_applied_node_trace if atom_trace is true
 		self.rules_to_be_applied_node_trace = numba.typed.List.empty_list(numba.types.Tuple((numba.types.ListType(numba.types.ListType(node_type)), numba.types.ListType(numba.types.ListType(edge_type)), numba.types.string)))
@@ -146,29 +147,31 @@
 				graph_attribute = True if name=='graph-attribute-fact' else False
 				facts_to_be_applied_edge.append((numba.types.uint16(t), fact.get_component(), fact.get_label(), fact.get_bound(), fact.static, graph_attribute))
 				if atom_trace:
 					facts_to_be_applied_edge_trace.append(fact.get_name())
 		return max_time
 
 	def _start_fp(self, rules, max_facts_time, verbose):
-		fp_cnt, t = self.reason(self.interpretations_node, self.interpretations_edge, self.tmax, self.prev_reasoning_data, rules, self.nodes, self.edges, self.neighbors, self.rules_to_be_applied_node, self.rules_to_be_applied_edge, self.edges_to_be_added_node_rule, self.edges_to_be_added_edge_rule, self.rules_to_be_applied_node_trace, self.rules_to_be_applied_edge_trace, self.facts_to_be_applied_node, self.facts_to_be_applied_edge, self.facts_to_be_applied_node_trace, self.facts_to_be_applied_edge_trace, self.available_labels_node, self.available_labels_edge, self.specific_node_labels, self.specific_edge_labels, self.ipl, self.rule_trace_node, self.rule_trace_edge, self.rule_trace_node_atoms, self.rule_trace_edge_atoms, self.reverse_graph, self.atom_trace, self.save_graph_attributes_to_rule_trace, self.canonical, self.inconsistency_check, max_facts_time, self._convergence_mode, self._convergence_delta, verbose)
+		fp_cnt, t = self.reason(self.interpretations_node, self.interpretations_edge, self.tmax, self.prev_reasoning_data, rules, self.nodes, self.edges, self.neighbors, self.rules_to_be_applied_node, self.rules_to_be_applied_edge, self.edges_to_be_added_node_rule, self.edges_to_be_added_edge_rule, self.rules_to_be_applied_node_trace, self.rules_to_be_applied_edge_trace, self.facts_to_be_applied_node, self.facts_to_be_applied_edge, self.facts_to_be_applied_node_trace, self.facts_to_be_applied_edge_trace, self.available_labels_node, self.available_labels_edge, self.specific_node_labels, self.specific_edge_labels, self.ipl, self.rule_trace_node, self.rule_trace_edge, self.rule_trace_node_atoms, self.rule_trace_edge_atoms, self.reverse_graph, self.atom_trace, self.save_graph_attributes_to_rule_trace, self.canonical, self.inconsistency_check, self.store_interpretation_changes, max_facts_time, self._convergence_mode, self._convergence_delta, verbose)
 		self.time = t - 1
 		# If we need to reason again, store the next timestep to start from
 		self.prev_reasoning_data[0] = t
 		self.prev_reasoning_data[1] = fp_cnt
 		if verbose:
 			print('Fixed Point iterations:', fp_cnt)
 
 	@staticmethod
 	@numba.njit(cache=True)
-	def reason(interpretations_node, interpretations_edge, tmax, prev_reasoning_data, rules, nodes, edges, neighbors, rules_to_be_applied_node, rules_to_be_applied_edge, edges_to_be_added_node_rule, edges_to_be_added_edge_rule, rules_to_be_applied_node_trace, rules_to_be_applied_edge_trace, facts_to_be_applied_node, facts_to_be_applied_edge, facts_to_be_applied_node_trace, facts_to_be_applied_edge_trace, labels_node, labels_edge, specific_labels_node, specific_labels_edge, ipl, rule_trace_node, rule_trace_edge, rule_trace_node_atoms, rule_trace_edge_atoms, reverse_graph, atom_trace, save_graph_attributes_to_rule_trace, canonical, inconsistency_check, max_facts_time, convergence_mode, convergence_delta, verbose):
+	def reason(interpretations_node, interpretations_edge, tmax, prev_reasoning_data, rules, nodes, edges, neighbors, rules_to_be_applied_node, rules_to_be_applied_edge, edges_to_be_added_node_rule, edges_to_be_added_edge_rule, rules_to_be_applied_node_trace, rules_to_be_applied_edge_trace, facts_to_be_applied_node, facts_to_be_applied_edge, facts_to_be_applied_node_trace, facts_to_be_applied_edge_trace, labels_node, labels_edge, specific_labels_node, specific_labels_edge, ipl, rule_trace_node, rule_trace_edge, rule_trace_node_atoms, rule_trace_edge_atoms, reverse_graph, atom_trace, save_graph_attributes_to_rule_trace, canonical, inconsistency_check, store_interpretation_changes, max_facts_time, convergence_mode, convergence_delta, verbose):
 		t = prev_reasoning_data[0]
 		fp_cnt = prev_reasoning_data[1]
 		max_rules_time = 0
 		timestep_loop = True
+		facts_to_remove_idx = numba.typed.List.empty_list(numba.types.int64)
+		rules_to_remove_idx = numba.typed.List.empty_list(numba.types.int64)
 		while timestep_loop:
 			if t==tmax:
 				timestep_loop=False
 			if verbose:
 				with objmode():
 					print('Timestep:', t, flush=True)
 			# Reset Interpretation at beginning of timestep if non-canonical
@@ -207,21 +210,23 @@
 			immediate_rule_applied = False
 			# When delta_t = 0, we don't want to check the same rule with the same node/edge after coming back to the fp operator
 			nodes_to_skip = numba.typed.List.empty_list(int_tuple)
 			edges_to_skip = numba.typed.List.empty_list(int_tuple)
 
 			# Start by applying facts
 			# Nodes
+			facts_to_remove_idx.clear()
 			for i in range(len(facts_to_be_applied_node)):
 				if facts_to_be_applied_node[i][0]==t:
 					comp, l, bnd, static, graph_attribute = facts_to_be_applied_node[i][1], facts_to_be_applied_node[i][2], facts_to_be_applied_node[i][3], facts_to_be_applied_node[i][4], facts_to_be_applied_node[i][5]
 					# Check if bnd is static. Then no need to update, just add to rule trace, check if graph attribute and add ipl complement to rule trace as well
 					if interpretations_node[comp].world[l].is_static():
+						# Check if we should even store any of the changes to the rule trace etc.
 						# Inverse of this is: if not save_graph_attributes_to_rule_trace and graph_attribute
-						if save_graph_attributes_to_rule_trace or not graph_attribute:
+						if (save_graph_attributes_to_rule_trace or not graph_attribute) and store_interpretation_changes:
 							rule_trace_node.append((numba.types.uint16(t), numba.types.uint16(fp_cnt), comp, l, bnd))
 							if atom_trace:
 								_update_rule_trace(rule_trace_node_atoms, numba.typed.List.empty_list(numba.typed.List.empty_list(node_type)), numba.typed.List.empty_list(numba.typed.List.empty_list(edge_type)), bnd, facts_to_be_applied_node_trace[i])
 							for p1, p2 in ipl:
 								if p1==l:
 									rule_trace_node.append((numba.types.uint16(t), numba.types.uint16(fp_cnt), comp, p2, interpretations_node[comp].world[p2]))
 									if atom_trace:
@@ -231,50 +236,55 @@
 									if atom_trace:
 										_update_rule_trace(rule_trace_node_atoms, numba.typed.List.empty_list(numba.typed.List.empty_list(node_type)), numba.typed.List.empty_list(numba.typed.List.empty_list(edge_type)), interpretations_node[comp].world[p1], facts_to_be_applied_node_trace[i])
 							
 					else:
 						# Check for inconsistencies (multiple facts)
 						if check_consistent_node(interpretations_node, comp, (l, bnd)):
 							mode = 'graph-attribute-fact' if graph_attribute else 'fact'
-							u, changes = _update_node(interpretations_node, comp, (l, bnd), ipl, rule_trace_node, fp_cnt, t, static, convergence_mode, atom_trace, save_graph_attributes_to_rule_trace, rules_to_be_applied_node_trace, i, facts_to_be_applied_node_trace, rule_trace_node_atoms, mode=mode)
+							u, changes = _update_node(interpretations_node, comp, (l, bnd), ipl, rule_trace_node, fp_cnt, t, static, convergence_mode, atom_trace, save_graph_attributes_to_rule_trace, rules_to_be_applied_node_trace, i, facts_to_be_applied_node_trace, rule_trace_node_atoms, store_interpretation_changes, mode=mode)
 
 							update = u or update
 							# Update convergence params
 							if convergence_mode=='delta_bound':
 								bound_delta = max(bound_delta, changes)
 							else:
 								changes_cnt += changes
 						# Resolve inconsistency if necessary otherwise override bounds
 						else:
 							if inconsistency_check:
-								resolve_inconsistency_node(interpretations_node, comp, (l, bnd), ipl, t, fp_cnt, atom_trace, rule_trace_node, rule_trace_node_atoms)
+								resolve_inconsistency_node(interpretations_node, comp, (l, bnd), ipl, t, fp_cnt, atom_trace, rule_trace_node, rule_trace_node_atoms, store_interpretation_changes)
 							else:
 								mode = 'graph-attribute-fact' if graph_attribute else 'fact'
-								u, changes = _override_update_node(interpretations_node, comp, (l, bnd), ipl, rule_trace_node, fp_cnt, t, static, convergence_mode, atom_trace, save_graph_attributes_to_rule_trace, rules_to_be_applied_node_trace, i, facts_to_be_applied_node_trace, rule_trace_node_atoms, mode=mode)
+								u, changes = _update_node(interpretations_node, comp, (l, bnd), ipl, rule_trace_node, fp_cnt, t, static, convergence_mode, atom_trace, save_graph_attributes_to_rule_trace, rules_to_be_applied_node_trace, i, facts_to_be_applied_node_trace, rule_trace_node_atoms, store_interpretation_changes, mode=mode, override=True)
 
 								update = u or update
 								# Update convergence params
 								if convergence_mode=='delta_bound':
 									bound_delta = max(bound_delta, changes)
 								else:
 									changes_cnt += changes
 
 					if static:
 						facts_to_be_applied_node[i] = (numba.types.uint16(facts_to_be_applied_node[i][0]+1), comp, l, bnd, static, graph_attribute)
+					else:
+						# Add to list to be removed later
+						facts_to_remove_idx.append(i)
+
+			# Delete facts that are not static
+			facts_to_be_applied_node[:] = numba.typed.List([facts_to_be_applied_node[i] for i in range(len(facts_to_be_applied_node)) if i not in facts_to_remove_idx])
 
-			# Deleting facts that have been applied is very inefficient
-			
 			# Edges
+			facts_to_remove_idx.clear()
 			for i in range(len(facts_to_be_applied_edge)):
 				if facts_to_be_applied_edge[i][0]==t:
 					comp, l, bnd, static, graph_attribute = facts_to_be_applied_edge[i][1], facts_to_be_applied_edge[i][2], facts_to_be_applied_edge[i][3], facts_to_be_applied_edge[i][4], facts_to_be_applied_edge[i][5]
 					# Check if bnd is static. Then no need to update, just add to rule trace, check if graph attribute, and add ipl complement to rule trace as well
 					if interpretations_edge[comp].world[l].is_static():
 						# Inverse of this is: if not save_graph_attributes_to_rule_trace and graph_attribute
-						if save_graph_attributes_to_rule_trace or not graph_attribute:
+						if (save_graph_attributes_to_rule_trace or not graph_attribute) and store_interpretation_changes:
 							rule_trace_edge.append((numba.types.uint16(t), numba.types.uint16(fp_cnt), comp, l, interpretations_edge[comp].world[l]))
 							if atom_trace:
 								_update_rule_trace(rule_trace_edge_atoms, numba.typed.List.empty_list(numba.typed.List.empty_list(node_type)), numba.typed.List.empty_list(numba.typed.List.empty_list(edge_type)), bnd, facts_to_be_applied_edge_trace[i])
 							for p1, p2 in ipl:
 								if p1==l:
 									rule_trace_edge.append((numba.types.uint16(t), numba.types.uint16(fp_cnt), comp, p2, interpretations_edge[comp].world[p2]))
 									if atom_trace:
@@ -283,49 +293,54 @@
 									rule_trace_edge.append((numba.types.uint16(t), numba.types.uint16(fp_cnt), comp, p1, interpretations_edge[comp].world[p1]))
 									if atom_trace:
 										_update_rule_trace(rule_trace_edge_atoms, numba.typed.List.empty_list(numba.typed.List.empty_list(node_type)), numba.typed.List.empty_list(numba.typed.List.empty_list(edge_type)), interpretations_edge[comp].world[p1], facts_to_be_applied_edge_trace[i])
 					else:
 						# Check for inconsistencies
 						if check_consistent_edge(interpretations_edge, comp, (l, bnd)):
 							mode = 'graph-attribute-fact' if graph_attribute else 'fact'
-							u, changes = _update_edge(interpretations_edge, comp, (l, bnd), ipl, rule_trace_edge, fp_cnt, t, static, convergence_mode, atom_trace, save_graph_attributes_to_rule_trace, rules_to_be_applied_edge_trace, i, facts_to_be_applied_edge_trace, rule_trace_edge_atoms, mode=mode)
+							u, changes = _update_edge(interpretations_edge, comp, (l, bnd), ipl, rule_trace_edge, fp_cnt, t, static, convergence_mode, atom_trace, save_graph_attributes_to_rule_trace, rules_to_be_applied_edge_trace, i, facts_to_be_applied_edge_trace, rule_trace_edge_atoms, store_interpretation_changes, mode=mode)
 
 							update = u or update
 							# Update convergence params
 							if convergence_mode=='delta_bound':
 								bound_delta = max(bound_delta, changes)
 							else:
 								changes_cnt += changes
 						# Resolve inconsistency
 						else:
 							if inconsistency_check:
-								resolve_inconsistency_edge(interpretations_edge, comp, (l, bnd), ipl, t, fp_cnt, atom_trace, rule_trace_edge, rule_trace_edge_atoms)
+								resolve_inconsistency_edge(interpretations_edge, comp, (l, bnd), ipl, t, fp_cnt, atom_trace, rule_trace_edge, rule_trace_edge_atoms, store_interpretation_changes)
 							else:
 								mode = 'graph-attribute-fact' if graph_attribute else 'fact'
-								u, changes = _override_update_edge(interpretations_edge, comp, (l, bnd), ipl, rule_trace_edge, fp_cnt, t, static, convergence_mode, atom_trace, save_graph_attributes_to_rule_trace, rules_to_be_applied_edge_trace, i, facts_to_be_applied_edge_trace, rule_trace_edge_atoms, mode=mode)
+								u, changes = _update_edge(interpretations_edge, comp, (l, bnd), ipl, rule_trace_edge, fp_cnt, t, static, convergence_mode, atom_trace, save_graph_attributes_to_rule_trace, rules_to_be_applied_edge_trace, i, facts_to_be_applied_edge_trace, rule_trace_edge_atoms, store_interpretation_changes, mode=mode, override=True)
 
 								update = u or update
 								# Update convergence params
 								if convergence_mode=='delta_bound':
 									bound_delta = max(bound_delta, changes)
 								else:
 									changes_cnt += changes
 
 					if static:
 						facts_to_be_applied_edge[i] = (numba.types.uint16(facts_to_be_applied_edge[i][0]+1), comp, l, bnd, static, graph_attribute)
+					else:
+						# Add to list to be removed later
+						facts_to_remove_idx.append(i)
 
-			# Deleting facts that have been applied is very inefficient
+			# Delete facts that are not static
+			facts_to_be_applied_edge[:] = numba.typed.List([facts_to_be_applied_edge[i] for i in range(len(facts_to_be_applied_edge)) if i not in facts_to_remove_idx])
 
 			in_loop = True
 			while in_loop:
 				# This will become true only if delta_t = 0 for some rule, otherwise we go to the next timestep
 				in_loop = False
 
 				# Apply the rules that need to be applied at this timestep
 				# Nodes
+				rules_to_remove_idx.clear()
 				for idx, i in enumerate(rules_to_be_applied_node):
 					# If we are coming here from an immediate rule firing with delta_t=0 we have to apply that one rule. Which was just added to the list to_be_applied
 					if immediate_node_rule_fire and rules_to_be_applied_node[-1][4]:
 						i = rules_to_be_applied_node[-1]
 						idx = -1
 
 					if i[0]==t:
@@ -334,76 +349,81 @@
 						edges_added, changes = _add_edges(sources, targets, neighbors, nodes, edges, edge_l, interpretations_node, interpretations_edge)
 						changes_cnt += changes
 
 						# Update bound for newly added edges. Use bnd to update all edges if label is specified, else use bnd to update normally
 						if edge_l.value!='':
 							for e in edges_added:
 								if check_consistent_edge(interpretations_edge, e, (edge_l, bnd)):
-									u, changes = _update_edge(interpretations_edge, e, (edge_l, bnd), ipl, rule_trace_edge, fp_cnt, t, False, convergence_mode, atom_trace, save_graph_attributes_to_rule_trace, rules_to_be_applied_node_trace, idx, facts_to_be_applied_edge_trace, rule_trace_edge_atoms, mode='rule')
+									u, changes = _update_edge(interpretations_edge, e, (edge_l, bnd), ipl, rule_trace_edge, fp_cnt, t, False, convergence_mode, atom_trace, save_graph_attributes_to_rule_trace, rules_to_be_applied_node_trace, idx, facts_to_be_applied_edge_trace, rule_trace_edge_atoms, store_interpretation_changes, mode='rule')
 
 									update = u or update
 
 									# Update convergence params
 									if convergence_mode=='delta_bound':
 										bound_delta = max(bound_delta, changes)
 									else:
 										changes_cnt += changes
 								# Resolve inconsistency
 								else:
 									if inconsistency_check:
-										resolve_inconsistency_edge(interpretations_edge, e, (edge_l, bnd), ipl, t, fp_cnt, atom_trace, rule_trace_edge, rule_trace_edge_atoms)
+										resolve_inconsistency_edge(interpretations_edge, e, (edge_l, bnd), ipl, t, fp_cnt, atom_trace, rule_trace_edge, rule_trace_edge_atoms, store_interpretation_changes)
 									else:
-										u, changes = _override_update_edge(interpretations_edge, e, (edge_l, bnd), ipl, rule_trace_edge, fp_cnt, t, False, convergence_mode, atom_trace, save_graph_attributes_to_rule_trace, rules_to_be_applied_node_trace, idx, facts_to_be_applied_edge_trace, rule_trace_edge_atoms, mode='rule')
+										u, changes = _update_edge(interpretations_edge, e, (edge_l, bnd), ipl, rule_trace_edge, fp_cnt, t, False, convergence_mode, atom_trace, save_graph_attributes_to_rule_trace, rules_to_be_applied_node_trace, idx, facts_to_be_applied_edge_trace, rule_trace_edge_atoms, store_interpretation_changes, mode='rule', override=True)
 
 										update = u or update
 
 										# Update convergence params
 										if convergence_mode=='delta_bound':
 											bound_delta = max(bound_delta, changes)
 										else:
 											changes_cnt += changes
 						else:
 							# Check for inconsistencies
 							if check_consistent_node(interpretations_node, comp, (l, bnd)):
-								u, changes = _update_node(interpretations_node, comp, (l, bnd), ipl, rule_trace_node, fp_cnt, t, False, convergence_mode, atom_trace, save_graph_attributes_to_rule_trace, rules_to_be_applied_node_trace, idx, facts_to_be_applied_node_trace, rule_trace_node_atoms, mode='rule')
+								u, changes = _update_node(interpretations_node, comp, (l, bnd), ipl, rule_trace_node, fp_cnt, t, False, convergence_mode, atom_trace, save_graph_attributes_to_rule_trace, rules_to_be_applied_node_trace, idx, facts_to_be_applied_node_trace, rule_trace_node_atoms, store_interpretation_changes, mode='rule')
 
 								update = u or update
 								# Update convergence params
 								if convergence_mode=='delta_bound':
 									bound_delta = max(bound_delta, changes)
 								else:
 									changes_cnt += changes
 							# Resolve inconsistency
 							else:
 								if inconsistency_check:
-									resolve_inconsistency_node(interpretations_node, comp, (l, bnd), ipl, t, fp_cnt, atom_trace, rule_trace_node, rule_trace_node_atoms)
+									resolve_inconsistency_node(interpretations_node, comp, (l, bnd), ipl, t, fp_cnt, atom_trace, rule_trace_node, rule_trace_node_atoms, store_interpretation_changes)
 								else:
-									u, changes = _override_update_node(interpretations_node, comp, (l, bnd), ipl, rule_trace_node, fp_cnt, t, False, convergence_mode, atom_trace, save_graph_attributes_to_rule_trace, rules_to_be_applied_node_trace, idx, facts_to_be_applied_node_trace, rule_trace_node_atoms, mode='rule')
+									u, changes = _update_node(interpretations_node, comp, (l, bnd), ipl, rule_trace_node, fp_cnt, t, False, convergence_mode, atom_trace, save_graph_attributes_to_rule_trace, rules_to_be_applied_node_trace, idx, facts_to_be_applied_node_trace, rule_trace_node_atoms, store_interpretation_changes, mode='rule', override=True)
 
 									update = u or update
 									# Update convergence params
 									if convergence_mode=='delta_bound':
 										bound_delta = max(bound_delta, changes)
 									else:
 										changes_cnt += changes
 
-						# Delete rules that have been applied from list by changing t to -1
-						rules_to_be_applied_node[idx] = (numba.types.uint16(-1), comp, l, bnd, False)
+						# Delete rules that have been applied from list by adding index to list
+						rules_to_remove_idx.append(idx)
 
 						# Break out of the apply rules loop if a rule is immediate. Then we go to the fp operator and check for other applicable rules then come back
 						if immediate:
 							# If delta_t=0 we want to apply one rule and go back to the fp operator
 							# If delta_t>0 we want to come back here and apply the rest of the rules
 							if immediate_edge_rule_fire:
 								break
 							elif not immediate_edge_rule_fire and u:
 								immediate_rule_applied = True
 								break
 
+				# Remove from rules to be applied and edges to be applied lists after coming out from loop
+				rules_to_be_applied_node[:] = numba.typed.List([rules_to_be_applied_node[i] for i in range(len(rules_to_be_applied_node)) if i not in rules_to_remove_idx])
+				edges_to_be_added_node_rule[:] = numba.typed.List([edges_to_be_added_node_rule[i] for i in range(len(edges_to_be_added_node_rule)) if i not in rules_to_remove_idx])
+
 				# Edges
+				rules_to_remove_idx.clear()
 				for idx, i in enumerate(rules_to_be_applied_edge):
 					# If we broke from above loop to apply more rules, then break from here
 					if immediate_rule_applied and not immediate_edge_rule_fire:
 						break
 					# If we are coming here from an immediate rule firing with delta_t=0 we have to apply that one rule. Which was just added to the list to_be_applied
 					if immediate_edge_rule_fire and rules_to_be_applied_edge[-1][4]:
 						i = rules_to_be_applied_edge[-1]
@@ -415,75 +435,79 @@
 						edges_added, changes = _add_edges(sources, targets, neighbors, nodes, edges, edge_l, interpretations_node, interpretations_edge)
 						changes_cnt += changes
 
 						# Update bound for newly added edges. Use bnd to update all edges if label is specified, else use bnd to update normally
 						if edge_l.value!='':
 							for e in edges_added:
 								if check_consistent_edge(interpretations_edge, e, (edge_l, bnd)):
-									u, changes = _update_edge(interpretations_edge, e, (edge_l, bnd), ipl, rule_trace_edge, fp_cnt, t, False, convergence_mode, atom_trace, save_graph_attributes_to_rule_trace, rules_to_be_applied_edge_trace, idx, facts_to_be_applied_edge_trace, rule_trace_edge_atoms, mode='rule')
+									u, changes = _update_edge(interpretations_edge, e, (edge_l, bnd), ipl, rule_trace_edge, fp_cnt, t, False, convergence_mode, atom_trace, save_graph_attributes_to_rule_trace, rules_to_be_applied_edge_trace, idx, facts_to_be_applied_edge_trace, rule_trace_edge_atoms, store_interpretation_changes, mode='rule')
 
 									update = u or update
 
 									# Update convergence params
 									if convergence_mode=='delta_bound':
 										bound_delta = max(bound_delta, changes)
 									else:
 										changes_cnt += changes
 								# Resolve inconsistency
 								else:
 									if inconsistency_check:
-										resolve_inconsistency_edge(interpretations_edge, e, (edge_l, bnd), ipl, t, fp_cnt, atom_trace, rule_trace_edge, rule_trace_edge_atoms)
+										resolve_inconsistency_edge(interpretations_edge, e, (edge_l, bnd), ipl, t, fp_cnt, atom_trace, rule_trace_edge, rule_trace_edge_atoms, store_interpretation_changes)
 									else:
-										u, changes = _override_update_edge(interpretations_edge, e, (edge_l, bnd), ipl, rule_trace_edge, fp_cnt, t, False, convergence_mode, atom_trace, save_graph_attributes_to_rule_trace, rules_to_be_applied_edge_trace, idx, facts_to_be_applied_edge_trace, rule_trace_edge_atoms, mode='rule')
+										u, changes = _update_edge(interpretations_edge, e, (edge_l, bnd), ipl, rule_trace_edge, fp_cnt, t, False, convergence_mode, atom_trace, save_graph_attributes_to_rule_trace, rules_to_be_applied_edge_trace, idx, facts_to_be_applied_edge_trace, rule_trace_edge_atoms, store_interpretation_changes, mode='rule', override=True)
 
 										update = u or update
 
 										# Update convergence params
 										if convergence_mode=='delta_bound':
 											bound_delta = max(bound_delta, changes)
 										else:
 											changes_cnt += changes
 
 						else:
 							# Check for inconsistencies
 							if check_consistent_edge(interpretations_edge, comp, (l, bnd)):
-								u, changes = _update_edge(interpretations_edge, comp, (l, bnd), ipl, rule_trace_edge, fp_cnt, t, False, convergence_mode, atom_trace, save_graph_attributes_to_rule_trace, rules_to_be_applied_edge_trace, idx, facts_to_be_applied_edge_trace, rule_trace_edge_atoms, mode='rule')
+								u, changes = _update_edge(interpretations_edge, comp, (l, bnd), ipl, rule_trace_edge, fp_cnt, t, False, convergence_mode, atom_trace, save_graph_attributes_to_rule_trace, rules_to_be_applied_edge_trace, idx, facts_to_be_applied_edge_trace, rule_trace_edge_atoms, store_interpretation_changes, mode='rule')
 
 								update = u or update
 								# Update convergence params
 								if convergence_mode=='delta_bound':
 									bound_delta = max(bound_delta, changes)
 								else:
 									changes_cnt += changes
 							# Resolve inconsistency
 							else:
 								if inconsistency_check:
-									resolve_inconsistency_edge(interpretations_edge, comp, (l, bnd), ipl, t, fp_cnt, atom_trace, rule_trace_edge, rule_trace_edge_atoms)
+									resolve_inconsistency_edge(interpretations_edge, comp, (l, bnd), ipl, t, fp_cnt, atom_trace, rule_trace_edge, rule_trace_edge_atoms, store_interpretation_changes)
 								else:
-									u, changes = _override_update_edge(interpretations_edge, comp, (l, bnd), ipl, rule_trace_edge, fp_cnt, t, False, convergence_mode, atom_trace, save_graph_attributes_to_rule_trace, rules_to_be_applied_edge_trace, idx, facts_to_be_applied_edge_trace, rule_trace_edge_atoms, mode='rule')
+									u, changes = _update_edge(interpretations_edge, comp, (l, bnd), ipl, rule_trace_edge, fp_cnt, t, False, convergence_mode, atom_trace, save_graph_attributes_to_rule_trace, rules_to_be_applied_edge_trace, idx, facts_to_be_applied_edge_trace, rule_trace_edge_atoms, store_interpretation_changes, mode='rule', override=True)
 
 									update = u or update
 									# Update convergence params
 									if convergence_mode=='delta_bound':
 										bound_delta = max(bound_delta, changes)
 									else:
 										changes_cnt += changes
 
-						# Delete rules that have been applied from list by changing t to -1
-						rules_to_be_applied_edge[idx] = (numba.types.uint16(-1), comp, l, bnd, False)
+						# Delete rules that have been applied from list by adding the index to list
+						rules_to_remove_idx.append(idx)
 
 						# Break out of the apply rules loop if a rule is immediate. Then we go to the fp operator and check for other applicable rules then come back
 						if immediate:
 							# If t=0 we want to apply one rule and go back to the fp operator
 							# If t>0 we want to come back here and apply the rest of the rules
 							if immediate_edge_rule_fire:
 								break
 							elif not immediate_edge_rule_fire and u:
 								immediate_rule_applied = True
 								break
+								
+				# Remove from rules to be applied and edges to be applied lists after coming out from loop
+				rules_to_be_applied_edge[:] = numba.typed.List([rules_to_be_applied_edge[i] for i in range(len(rules_to_be_applied_edge)) if i not in rules_to_remove_idx])
+				edges_to_be_added_edge_rule[:] = numba.typed.List([edges_to_be_added_edge_rule[i] for i in range(len(edges_to_be_added_edge_rule)) if i not in rules_to_remove_idx])
 
 				# Fixed point
 				# if update or immediate_node_rule_fire or immediate_edge_rule_fire or immediate_rule_applied:
 				if update:
 					# Increase fp operator count only if not an immediate rule
 					if not (immediate_node_rule_fire or immediate_edge_rule_fire):
 						fp_cnt += 1
@@ -915,147 +939,75 @@
 		elif threshold[0]=='equal':
 			result = True if num_qualified_component/num_neigh == threshold[2]*0.01 else False
 
 	return result
 
 
 @numba.njit(cache=True)
-def _update_node(interpretations, comp, na, ipl, rule_trace, fp_cnt, t_cnt, static, convergence_mode, atom_trace, save_graph_attributes_to_rule_trace, rules_to_be_applied_trace, idx, facts_to_be_applied_trace, rule_trace_atoms, mode):
+def _update_node(interpretations, comp, na, ipl, rule_trace, fp_cnt, t_cnt, static, convergence_mode, atom_trace, save_graph_attributes_to_rule_trace, rules_to_be_applied_trace, idx, facts_to_be_applied_trace, rule_trace_atoms, store_interpretation_changes, mode, override=False):
 	updated = False
 	# This is to prevent a key error in case the label is a specific label
 	try:
 		world = interpretations[comp]
 		l, bnd = na
 		updated_bnds = numba.typed.List.empty_list(interval.interval_type)
 
 		# Check if update is necessary with previous bnd
 		prev_bnd = world.world[l].copy()
-		world.update(l, bnd)
-		world.world[l].set_static(static)
-		if world.world[l]!=prev_bnd:
-			updated = True
-			updated_bnds.append(world.world[l])
-
-			# Add to rule trace if update happened and add to atom trace if necessary
-			if save_graph_attributes_to_rule_trace or not mode=='graph-attribute-fact':
-				rule_trace.append((numba.types.uint16(t_cnt), numba.types.uint16(fp_cnt), comp, l, world.world[l].copy()))
-				if atom_trace:
-					# Mode can be fact or rule, updation of trace will happen accordingly
-					if mode=='fact' or mode=='graph-attribute-fact':
-						qn = numba.typed.List.empty_list(numba.typed.List.empty_list(node_type))
-						qe = numba.typed.List.empty_list(numba.typed.List.empty_list(edge_type))
-						name = facts_to_be_applied_trace[idx]
-						_update_rule_trace(rule_trace_atoms, qn, qe, prev_bnd, name)
-					elif mode=='rule':
-						qn, qe, name = rules_to_be_applied_trace[idx]
-						_update_rule_trace(rule_trace_atoms, qn, qe, prev_bnd, name)
-
-		# Update complement of predicate (if exists) based on new knowledge of predicate
-		if updated:
-			ip_update_cnt = 0
-			for p1, p2 in ipl:
-				if p1==l:
-					if atom_trace:
-						_update_rule_trace(rule_trace_atoms, numba.typed.List.empty_list(numba.typed.List.empty_list(node_type)), numba.typed.List.empty_list(numba.typed.List.empty_list(edge_type)), world.world[p2], f'IPL: {l.get_value()}')
-					lower = max(world.world[p2].lower, 1 - world.world[p1].upper)
-					upper = min(world.world[p2].upper, 1 - world.world[p1].lower)
-					world.world[p2].set_lower_upper(lower, upper)
-					world.world[p2].set_static(static)
-					ip_update_cnt += 1
-					updated_bnds.append(world.world[p2])
-					rule_trace.append((numba.types.uint16(t_cnt), numba.types.uint16(fp_cnt), comp, p2, interval.closed(lower, upper)))
-				if p2==l:
-					if atom_trace:
-						_update_rule_trace(rule_trace_atoms, numba.typed.List.empty_list(numba.typed.List.empty_list(node_type)), numba.typed.List.empty_list(numba.typed.List.empty_list(edge_type)), world.world[p1], f'IPL: {l.get_value()}')
-					lower = max(world.world[p1].lower, 1 - world.world[p2].upper)
-					upper = min(world.world[p1].upper, 1 - world.world[p2].lower)
-					world.world[p1].set_lower_upper(lower, upper)
-					world.world[p1].set_static(static)
-					ip_update_cnt += 1
-					updated_bnds.append(world.world[p1])
-					rule_trace.append((numba.types.uint16(t_cnt), numba.types.uint16(fp_cnt), comp, p1, interval.closed(lower, upper)))
-		
-		# Gather convergence data
-		change = 0
-		if updated:
-			# Find out if it has changed from previous interp
-			current_bnd = world.world[l]
-			prev_t_bnd = interval.closed(world.world[l].prev_lower, world.world[l].prev_upper)
-			if current_bnd != prev_t_bnd:
-				if convergence_mode=='delta_bound':
-					for i in updated_bnds:
-						lower_delta = abs(i.lower-prev_t_bnd.lower)
-						upper_delta = abs(i.upper-prev_t_bnd.upper)
-						max_delta = max(lower_delta, upper_delta)
-						change = max(change, max_delta)
-				else:
-					change = 1 + ip_update_cnt
-
-		return (updated, change)
-
-	except:
-		return (False, 0)
-
 
-@numba.njit(cache=True)
-def _override_update_node(interpretations, comp, na, ipl, rule_trace, fp_cnt, t_cnt, static, convergence_mode, atom_trace, save_graph_attributes_to_rule_trace, rules_to_be_applied_trace, idx, facts_to_be_applied_trace, rule_trace_atoms, mode):
-	updated = False
-	# This is to prevent a key error in case the label is a specific label
-	try:
-		world = interpretations[comp]
-		l, bnd = na
-		updated_bnds = numba.typed.List.empty_list(interval.interval_type)
-
-		# Check if update is necessary with previous bnd
-		prev_bnd = world.world[l].copy()
-		world.world[l].set_lower_upper(bnd.lower, bnd.upper)
+		# override will not check for inconsistencies
+		if override:
+			world.world[l].set_lower_upper(bnd.lower, bnd.upper)
+		else:
+			world.update(l, bnd)
 		world.world[l].set_static(static)
 		if world.world[l]!=prev_bnd:
 			updated = True
 			updated_bnds.append(world.world[l])
 
 			# Add to rule trace if update happened and add to atom trace if necessary
-			if save_graph_attributes_to_rule_trace or not mode=='graph-attribute-fact':
+			if (save_graph_attributes_to_rule_trace or not mode=='graph-attribute-fact') and store_interpretation_changes:
 				rule_trace.append((numba.types.uint16(t_cnt), numba.types.uint16(fp_cnt), comp, l, world.world[l].copy()))
 				if atom_trace:
 					# Mode can be fact or rule, updation of trace will happen accordingly
 					if mode=='fact' or mode=='graph-attribute-fact':
 						qn = numba.typed.List.empty_list(numba.typed.List.empty_list(node_type))
 						qe = numba.typed.List.empty_list(numba.typed.List.empty_list(edge_type))
 						name = facts_to_be_applied_trace[idx]
 						_update_rule_trace(rule_trace_atoms, qn, qe, prev_bnd, name)
 					elif mode=='rule':
 						qn, qe, name = rules_to_be_applied_trace[idx]
 						_update_rule_trace(rule_trace_atoms, qn, qe, prev_bnd, name)
-			
 
 		# Update complement of predicate (if exists) based on new knowledge of predicate
 		if updated:
 			ip_update_cnt = 0
 			for p1, p2 in ipl:
 				if p1==l:
 					if atom_trace:
 						_update_rule_trace(rule_trace_atoms, numba.typed.List.empty_list(numba.typed.List.empty_list(node_type)), numba.typed.List.empty_list(numba.typed.List.empty_list(edge_type)), world.world[p2], f'IPL: {l.get_value()}')
 					lower = max(world.world[p2].lower, 1 - world.world[p1].upper)
 					upper = min(world.world[p2].upper, 1 - world.world[p1].lower)
 					world.world[p2].set_lower_upper(lower, upper)
 					world.world[p2].set_static(static)
 					ip_update_cnt += 1
 					updated_bnds.append(world.world[p2])
-					rule_trace.append((numba.types.uint16(t_cnt), numba.types.uint16(fp_cnt), comp, p2, interval.closed(lower, upper)))
+					if store_interpretation_changes:
+						rule_trace.append((numba.types.uint16(t_cnt), numba.types.uint16(fp_cnt), comp, p2, interval.closed(lower, upper)))
 				if p2==l:
 					if atom_trace:
 						_update_rule_trace(rule_trace_atoms, numba.typed.List.empty_list(numba.typed.List.empty_list(node_type)), numba.typed.List.empty_list(numba.typed.List.empty_list(edge_type)), world.world[p1], f'IPL: {l.get_value()}')
 					lower = max(world.world[p1].lower, 1 - world.world[p2].upper)
 					upper = min(world.world[p1].upper, 1 - world.world[p2].lower)
 					world.world[p1].set_lower_upper(lower, upper)
 					world.world[p1].set_static(static)
 					ip_update_cnt += 1
 					updated_bnds.append(world.world[p1])
-					rule_trace.append((numba.types.uint16(t_cnt), numba.types.uint16(fp_cnt), comp, p1, interval.closed(lower, upper)))
+					if store_interpretation_changes:
+						rule_trace.append((numba.types.uint16(t_cnt), numba.types.uint16(fp_cnt), comp, p1, interval.closed(lower, upper)))
 		
 		# Gather convergence data
 		change = 0
 		if updated:
 			# Find out if it has changed from previous interp
 			current_bnd = world.world[l]
 			prev_t_bnd = interval.closed(world.world[l].prev_lower, world.world[l].prev_upper)
@@ -1069,112 +1021,40 @@
 				else:
 					change = 1 + ip_update_cnt
 
 		return (updated, change)
 
 	except:
 		return (False, 0)
-	
-
-@numba.njit(cache=True)
-def _update_edge(interpretations, comp, na, ipl, rule_trace, fp_cnt, t_cnt, static, convergence_mode, atom_trace, save_graph_attributes_to_rule_trace, rules_to_be_applied_trace, idx, facts_to_be_applied_trace, rule_trace_atoms, mode):
-	updated = False
-	# This is to prevent a key error in case the label is a specific label
-	try:
-		world = interpretations[comp]
-		l, bnd = na
-		updated_bnds = numba.typed.List.empty_list(interval.interval_type)
-
-		# Check if update is necessary with previous bnd
-		prev_bnd = world.world[l].copy()
-		world.update(l, bnd)
-		world.world[l].set_static(static)
-		if world.world[l]!=prev_bnd:
-			updated = True
-			updated_bnds.append(world.world[l])
-
-			# Add to rule trace if update happened and add to atom trace if necessary
-			if save_graph_attributes_to_rule_trace or not mode=='graph-attribute-fact':
-				rule_trace.append((numba.types.uint16(t_cnt), numba.types.uint16(fp_cnt), comp, l, world.world[l].copy()))
-				if atom_trace:
-					# Mode can be fact or rule, updation of trace will happen accordingly
-					if mode=='fact' or mode=='graph-attribute-fact':
-						qn = numba.typed.List.empty_list(numba.typed.List.empty_list(node_type))
-						qe = numba.typed.List.empty_list(numba.typed.List.empty_list(edge_type))
-						name = facts_to_be_applied_trace[idx]
-						_update_rule_trace(rule_trace_atoms, qn, qe, prev_bnd, name)
-					elif mode=='rule':
-						qn, qe, name = rules_to_be_applied_trace[idx]
-						_update_rule_trace(rule_trace_atoms, qn, qe, prev_bnd, name)
-
-		# Update complement of predicate (if exists) based on new knowledge of predicate
-		if updated:
-			ip_update_cnt = 0
-			for p1, p2 in ipl:
-				if p1==l:
-					if atom_trace:
-						_update_rule_trace(rule_trace_atoms, numba.typed.List.empty_list(numba.typed.List.empty_list(node_type)), numba.typed.List.empty_list(numba.typed.List.empty_list(edge_type)), world.world[p2], f'IPL: {l.get_value()}')
-					lower = max(world.world[p2].lower, 1 - world.world[p1].upper)
-					upper = min(world.world[p2].upper, 1 - world.world[p1].lower)
-					world.world[p2].set_lower_upper(lower, upper)
-					world.world[p2].set_static(static)
-					ip_update_cnt += 1
-					updated_bnds.append(world.world[p2])
-					rule_trace.append((numba.types.uint16(t_cnt), numba.types.uint16(fp_cnt), comp, p2, interval.closed(lower, upper)))
-				if p2==l:
-					if atom_trace:
-						_update_rule_trace(rule_trace_atoms, numba.typed.List.empty_list(numba.typed.List.empty_list(node_type)), numba.typed.List.empty_list(numba.typed.List.empty_list(edge_type)), world.world[p1], f'IPL: {l.get_value()}')
-					lower = max(world.world[p1].lower, 1 - world.world[p2].upper)
-					upper = min(world.world[p1].upper, 1 - world.world[p2].lower)
-					world.world[p1].set_lower_upper(lower, upper)
-					world.world[p1].set_static(static)
-					ip_update_cnt += 1
-					updated_bnds.append(world.world[p2])
-					rule_trace.append((numba.types.uint16(t_cnt), numba.types.uint16(fp_cnt), comp, p1, interval.closed(lower, upper)))
-	
-		# Gather convergence data
-		change = 0
-		if updated:
-			# Find out if it has changed from previous interp
-			current_bnd = world.world[l]
-			prev_t_bnd = interval.closed(world.world[l].prev_lower, world.world[l].prev_upper)
-			if current_bnd != prev_t_bnd:
-				if convergence_mode=='delta_bound':
-					for i in updated_bnds:
-						lower_delta = abs(i.lower-prev_t_bnd.lower)
-						upper_delta = abs(i.upper-prev_t_bnd.upper)
-						max_delta = max(lower_delta, upper_delta)
-						change = max(change, max_delta)
-				else:
-					change = 1 + ip_update_cnt
-		
-		return (updated, change)
-	except:
-		return (False, 0)
 
 
 @numba.njit(cache=True)
-def _override_update_edge(interpretations, comp, na, ipl, rule_trace, fp_cnt, t_cnt, static, convergence_mode, atom_trace, save_graph_attributes_to_rule_trace, rules_to_be_applied_trace, idx, facts_to_be_applied_trace, rule_trace_atoms, mode):
+def _update_edge(interpretations, comp, na, ipl, rule_trace, fp_cnt, t_cnt, static, convergence_mode, atom_trace, save_graph_attributes_to_rule_trace, rules_to_be_applied_trace, idx, facts_to_be_applied_trace, rule_trace_atoms, store_interpretation_changes, mode, override=False):
 	updated = False
 	# This is to prevent a key error in case the label is a specific label
 	try:
 		world = interpretations[comp]
 		l, bnd = na
 		updated_bnds = numba.typed.List.empty_list(interval.interval_type)
 
 		# Check if update is necessary with previous bnd
 		prev_bnd = world.world[l].copy()
-		world.world[l].set_lower_upper(bnd.lower, bnd.upper)
+
+		# override will not check for inconsistencies
+		if override:
+			world.world[l].set_lower_upper(bnd.lower, bnd.upper)
+		else:
+			world.update(l, bnd)
 		world.world[l].set_static(static)
 		if world.world[l]!=prev_bnd:
 			updated = True
 			updated_bnds.append(world.world[l])
 
 			# Add to rule trace if update happened and add to atom trace if necessary
-			if save_graph_attributes_to_rule_trace or not mode=='graph-attribute-fact':
+			if (save_graph_attributes_to_rule_trace or not mode=='graph-attribute-fact') and store_interpretation_changes:
 				rule_trace.append((numba.types.uint16(t_cnt), numba.types.uint16(fp_cnt), comp, l, world.world[l].copy()))
 				if atom_trace:
 					# Mode can be fact or rule, updation of trace will happen accordingly
 					if mode=='fact' or mode=='graph-attribute-fact':
 						qn = numba.typed.List.empty_list(numba.typed.List.empty_list(node_type))
 						qe = numba.typed.List.empty_list(numba.typed.List.empty_list(edge_type))
 						name = facts_to_be_applied_trace[idx]
@@ -1192,25 +1072,27 @@
 						_update_rule_trace(rule_trace_atoms, numba.typed.List.empty_list(numba.typed.List.empty_list(node_type)), numba.typed.List.empty_list(numba.typed.List.empty_list(edge_type)), world.world[p2], f'IPL: {l.get_value()}')
 					lower = max(world.world[p2].lower, 1 - world.world[p1].upper)
 					upper = min(world.world[p2].upper, 1 - world.world[p1].lower)
 					world.world[p2].set_lower_upper(lower, upper)
 					world.world[p2].set_static(static)
 					ip_update_cnt += 1
 					updated_bnds.append(world.world[p2])
-					rule_trace.append((numba.types.uint16(t_cnt), numba.types.uint16(fp_cnt), comp, p2, interval.closed(lower, upper)))
+					if store_interpretation_changes:
+						rule_trace.append((numba.types.uint16(t_cnt), numba.types.uint16(fp_cnt), comp, p2, interval.closed(lower, upper)))
 				if p2==l:
 					if atom_trace:
 						_update_rule_trace(rule_trace_atoms, numba.typed.List.empty_list(numba.typed.List.empty_list(node_type)), numba.typed.List.empty_list(numba.typed.List.empty_list(edge_type)), world.world[p1], f'IPL: {l.get_value()}')
 					lower = max(world.world[p1].lower, 1 - world.world[p2].upper)
 					upper = min(world.world[p1].upper, 1 - world.world[p2].lower)
 					world.world[p1].set_lower_upper(lower, upper)
 					world.world[p1].set_static(static)
 					ip_update_cnt += 1
 					updated_bnds.append(world.world[p2])
-					rule_trace.append((numba.types.uint16(t_cnt), numba.types.uint16(fp_cnt), comp, p1, interval.closed(lower, upper)))
+					if store_interpretation_changes:
+						rule_trace.append((numba.types.uint16(t_cnt), numba.types.uint16(fp_cnt), comp, p1, interval.closed(lower, upper)))
 	
 		# Gather convergence data
 		change = 0
 		if updated:
 			# Find out if it has changed from previous interp
 			current_bnd = world.world[l]
 			prev_t_bnd = interval.closed(world.world[l].prev_lower, world.world[l].prev_upper)
@@ -1312,62 +1194,68 @@
 	if (na[1].lower > bnd.upper) or (bnd.lower > na[1].upper):
 		return False
 	else:
 		return True
 
 
 @numba.njit(cache=True)
-def resolve_inconsistency_node(interpretations, comp, na, ipl, t_cnt, fp_cnt, atom_trace, rule_trace, rule_trace_atoms):
+def resolve_inconsistency_node(interpretations, comp, na, ipl, t_cnt, fp_cnt, atom_trace, rule_trace, rule_trace_atoms, store_interpretation_changes):
 	world = interpretations[comp]
-	rule_trace.append((numba.types.uint16(t_cnt), numba.types.uint16(fp_cnt), comp, na[0], interval.closed(0,1)))
-	if atom_trace:
-		_update_rule_trace(rule_trace_atoms, numba.typed.List.empty_list(numba.typed.List.empty_list(node_type)), numba.typed.List.empty_list(numba.typed.List.empty_list(edge_type)), world.world[na[0]], 'Inconsistency')
+	if store_interpretation_changes:
+		rule_trace.append((numba.types.uint16(t_cnt), numba.types.uint16(fp_cnt), comp, na[0], interval.closed(0,1)))
+		if atom_trace:
+			_update_rule_trace(rule_trace_atoms, numba.typed.List.empty_list(numba.typed.List.empty_list(node_type)), numba.typed.List.empty_list(numba.typed.List.empty_list(edge_type)), world.world[na[0]], 'Inconsistency')
 	# Resolve inconsistency and set static
 	world.world[na[0]].set_lower_upper(0, 1)
 	world.world[na[0]].set_static(True)
 	for p1, p2 in ipl:
 		if p1==na[0]:
 			if atom_trace:
 				_update_rule_trace(rule_trace_atoms, numba.typed.List.empty_list(numba.typed.List.empty_list(node_type)), numba.typed.List.empty_list(numba.typed.List.empty_list(edge_type)), world.world[p2], 'Inconsistency')
 			world.world[p2].set_lower_upper(0, 1)
 			world.world[p2].set_static(True)
-			rule_trace.append((numba.types.uint16(t_cnt), numba.types.uint16(fp_cnt), comp, p2, interval.closed(0,1)))
+			if store_interpretation_changes:
+				rule_trace.append((numba.types.uint16(t_cnt), numba.types.uint16(fp_cnt), comp, p2, interval.closed(0,1)))
 
 		if p2==na[0]:
 			if atom_trace:
 				_update_rule_trace(rule_trace_atoms, numba.typed.List.empty_list(numba.typed.List.empty_list(node_type)), numba.typed.List.empty_list(numba.typed.List.empty_list(edge_type)), world.world[p1], 'Inconsistency')
 			world.world[p1].set_lower_upper(0, 1)
 			world.world[p1].set_static(True)
-			rule_trace.append((numba.types.uint16(t_cnt), numba.types.uint16(fp_cnt), comp, p1, interval.closed(0,1)))
+			if store_interpretation_changes:
+				rule_trace.append((numba.types.uint16(t_cnt), numba.types.uint16(fp_cnt), comp, p1, interval.closed(0,1)))
 	# Add inconsistent predicates to a list 
 
 
 @numba.njit(cache=True)
-def resolve_inconsistency_edge(interpretations, comp, na, ipl, t_cnt, fp_cnt, atom_trace, rule_trace, rule_trace_atoms):
+def resolve_inconsistency_edge(interpretations, comp, na, ipl, t_cnt, fp_cnt, atom_trace, rule_trace, rule_trace_atoms, store_interpretation_changes):
 	world = interpretations[comp]
-	rule_trace.append((numba.types.uint16(t_cnt), numba.types.uint16(fp_cnt), comp, na[0], interval.closed(0,1)))
-	if atom_trace:
-		_update_rule_trace(rule_trace_atoms, numba.typed.List.empty_list(numba.typed.List.empty_list(node_type)), numba.typed.List.empty_list(numba.typed.List.empty_list(edge_type)), world.world[na[0]], 'Inconsistency')
+	if store_interpretation_changes:
+		rule_trace.append((numba.types.uint16(t_cnt), numba.types.uint16(fp_cnt), comp, na[0], interval.closed(0,1)))
+		if atom_trace:
+			_update_rule_trace(rule_trace_atoms, numba.typed.List.empty_list(numba.typed.List.empty_list(node_type)), numba.typed.List.empty_list(numba.typed.List.empty_list(edge_type)), world.world[na[0]], 'Inconsistency')
 	# Resolve inconsistency and set static
 	world.world[na[0]].set_lower_upper(0, 1)
 	world.world[na[0]].set_static(True)
 	for p1, p2 in ipl:
 		if p1==na[0]:
 			if atom_trace:
 				_update_rule_trace(rule_trace_atoms, numba.typed.List.empty_list(numba.typed.List.empty_list(node_type)), numba.typed.List.empty_list(numba.typed.List.empty_list(edge_type)), world.world[p2], 'Inconsistency')
 			world.world[p2].set_lower_upper(0, 1)
 			world.world[p2].set_static(True)
-			rule_trace.append((numba.types.uint16(t_cnt), numba.types.uint16(fp_cnt), comp, p2, interval.closed(0,1)))
+			if store_interpretation_changes:
+				rule_trace.append((numba.types.uint16(t_cnt), numba.types.uint16(fp_cnt), comp, p2, interval.closed(0,1)))
 
 		if p2==na[0]:
 			if atom_trace:
 				_update_rule_trace(rule_trace_atoms, numba.typed.List.empty_list(numba.typed.List.empty_list(node_type)), numba.typed.List.empty_list(numba.typed.List.empty_list(edge_type)), world.world[p1], 'Inconsistency')
 			world.world[p1].set_lower_upper(0, 1)
 			world.world[p1].set_static(True)
-			rule_trace.append((numba.types.uint16(t_cnt), numba.types.uint16(fp_cnt), comp, p1, interval.closed(0,1)))
+			if store_interpretation_changes:
+				rule_trace.append((numba.types.uint16(t_cnt), numba.types.uint16(fp_cnt), comp, p1, interval.closed(0,1)))
 
 
 @numba.njit(cache=True)
 def _add_node(node, neighbors, nodes, interpretations_node):
 	nodes.append(node)
 	neighbors[node] = numba.typed.List.empty_list(node_type)
 	interpretations_node[node] = world.World(numba.typed.List.empty_list(label.label_type))
```

### Comparing `pyreason-1.5.3/pyreason/scripts/interval/interval.py` & `pyreason-1.6.0/pyreason/scripts/interval/interval.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.5.3/pyreason/scripts/numba_wrapper/numba_types/fact_edge_type.py` & `pyreason-1.6.0/pyreason/scripts/numba_wrapper/numba_types/fact_edge_type.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.5.3/pyreason/scripts/numba_wrapper/numba_types/fact_node_type.py` & `pyreason-1.6.0/pyreason/scripts/numba_wrapper/numba_types/fact_node_type.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.5.3/pyreason/scripts/numba_wrapper/numba_types/interval_type.py` & `pyreason-1.6.0/pyreason/scripts/numba_wrapper/numba_types/interval_type.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.5.3/pyreason/scripts/numba_wrapper/numba_types/label_type.py` & `pyreason-1.6.0/pyreason/scripts/numba_wrapper/numba_types/label_type.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.5.3/pyreason/scripts/numba_wrapper/numba_types/rule_type.py` & `pyreason-1.6.0/pyreason/scripts/numba_wrapper/numba_types/rule_type.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.5.3/pyreason/scripts/numba_wrapper/numba_types/world_type.py` & `pyreason-1.6.0/pyreason/scripts/numba_wrapper/numba_types/world_type.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.5.3/pyreason/scripts/program/program.py` & `pyreason-1.6.0/pyreason/scripts/program/program.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,36 +3,37 @@
 
 class Program:
 	available_labels_node = []
 	available_labels_edge = []
 	specific_node_labels = []
 	specific_edge_labels = []
 
-	def __init__(self, graph, facts_node, facts_edge, rules, ipl, reverse_graph, atom_trace, save_graph_attributes_to_rule_trace, canonical, inconsistency_check):
+	def __init__(self, graph, facts_node, facts_edge, rules, ipl, reverse_graph, atom_trace, save_graph_attributes_to_rule_trace, canonical, inconsistency_check, store_interpretation_changes):
 		self._graph = graph
 		self._facts_node = facts_node
 		self._facts_edge = facts_edge
 		self._rules = rules
 		self._ipl = ipl
 		self._reverse_graph = reverse_graph
 		self._atom_trace = atom_trace
 		self._save_graph_attributes_to_rule_trace = save_graph_attributes_to_rule_trace
 		self._canonical = canonical
 		self._inconsistency_check = inconsistency_check
+		self._store_interpretation_changes = store_interpretation_changes
 		self.interp = None
 
 	def reason(self, tmax, convergence_threshold, convergence_bound_threshold, verbose=True):
 		self._tmax = tmax
 		# Set up available labels
 		Interpretation.available_labels_node = self.available_labels_node
 		Interpretation.available_labels_edge = self.available_labels_edge
 		Interpretation.specific_node_labels = self.specific_node_labels
 		Interpretation.specific_edge_labels = self.specific_edge_labels
 
-		self.interp = Interpretation(self._graph, self._ipl, self._reverse_graph, self._atom_trace, self._save_graph_attributes_to_rule_trace, self._canonical, self._inconsistency_check)
+		self.interp = Interpretation(self._graph, self._ipl, self._reverse_graph, self._atom_trace, self._save_graph_attributes_to_rule_trace, self._canonical, self._inconsistency_check, self._store_interpretation_changes)
 		self.interp.start_fp(self._tmax, self._facts_node, self._facts_edge, self._rules, verbose, convergence_threshold, convergence_bound_threshold)
 
 		return self.interp
 	
 	def reason_again(self, tmax, convergence_threshold, convergence_bound_threshold, facts_node, facts_edge, verbose=True):
 		assert self.interp is not None, 'Call reason before calling reason again'
 		self._tmax = self.interp.time + tmax
```

### Comparing `pyreason-1.5.3/pyreason/scripts/rules/rule.py` & `pyreason-1.6.0/pyreason/scripts/rules/rule.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.5.3/pyreason/scripts/utils/filter.py` & `pyreason-1.6.0/pyreason/scripts/utils/filter.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.5.3/pyreason/scripts/utils/graphml_parser.py` & `pyreason-1.6.0/pyreason/scripts/utils/graphml_parser.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.5.3/pyreason/scripts/utils/output.py` & `pyreason-1.6.0/pyreason/scripts/utils/output.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.5.3/pyreason/scripts/utils/plotter.py` & `pyreason-1.6.0/pyreason/scripts/utils/plotter.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.5.3/pyreason/scripts/utils/visuals.py` & `pyreason-1.6.0/pyreason/scripts/utils/visuals.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.5.3/pyreason/scripts/utils/yaml_parser.py` & `pyreason-1.6.0/pyreason/scripts/utils/yaml_parser.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.5.3/pyreason.egg-info/PKG-INFO` & `pyreason-1.6.0/pyreason.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyreason
-Version: 1.5.3
+Version: 1.6.0
 Summary: An explainable inference software supporting annotated, real valued, graph based and temporal logic
 Home-page: https://github.com/lab-v2/pyreason
 Author: Dyuman Aditya
 Author-email: dyuman.aditya@gmail.com
 License: BSD 3-clause
 Project-URL: Bug Tracker, https://github.com/lab-v2/pyreason/issues
 Project-URL: Repository, https://github.com/lab-v2/pyreason
```

### Comparing `pyreason-1.5.3/pyreason.egg-info/SOURCES.txt` & `pyreason-1.6.0/pyreason.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyreason-1.5.3/setup.py` & `pyreason-1.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 
 setup(
     name = 'pyreason',
-    version = '1.5.3',
+    version = '1.6.0',
     author = 'Dyuman Aditya',
     author_email = 'dyuman.aditya@gmail.com',
     description = 'An explainable inference software supporting annotated, real valued, graph based and temporal logic',
     long_description = long_description,
     long_description_content_type = 'text/markdown',
     url = 'https://github.com/lab-v2/pyreason',
     license = 'BSD 3-clause',
```

