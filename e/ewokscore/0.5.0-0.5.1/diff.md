# Comparing `tmp/ewokscore-0.5.0.tar.gz` & `tmp/ewokscore-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ewokscore-0.5.0.tar", last modified: Fri Jun  9 07:41:46 2023, max compression
+gzip compressed data, was "dist/ewokscore-0.5.1.tar", last modified: Fri Jun  9 17:22:22 2023, max compression
```

## Comparing `ewokscore-0.5.0.tar` & `ewokscore-0.5.1.tar`

### file list

```diff
@@ -1,133 +1,133 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:41:46.000000 ewokscore-0.5.0/
--rw-rw-rw-   0 root         (0) root         (0)     1102 2023-06-09 07:29:47.000000 ewokscore-0.5.0/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)     2638 2023-06-09 07:41:46.000000 ewokscore-0.5.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1896 2023-06-09 07:29:47.000000 ewokscore-0.5.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)      106 2023-06-09 07:29:47.000000 ewokscore-0.5.0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1427 2023-06-09 07:41:46.000000 ewokscore-0.5.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       69 2023-06-09 07:29:47.000000 ewokscore-0.5.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:41:46.000000 ewokscore-0.5.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:41:46.000000 ewokscore-0.5.0/src/ewokscore/
--rw-rw-rw-   0 root         (0) root         (0)      164 2023-06-09 07:35:03.000000 ewokscore-0.5.0/src/ewokscore/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1721 2023-06-09 07:29:47.000000 ewokscore-0.5.0/src/ewokscore/bindings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:41:46.000000 ewokscore-0.5.0/src/ewokscore/cliutils/
--rw-rw-rw-   0 root         (0) root         (0)      738 2023-06-09 07:29:47.000000 ewokscore-0.5.0/src/ewokscore/cliutils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2997 2023-06-09 07:29:47.000000 ewokscore-0.5.0/src/ewokscore/cliutils/cliconvertutils.py
--rw-rw-rw-   0 root         (0) root         (0)     4778 2023-06-09 07:29:47.000000 ewokscore-0.5.0/src/ewokscore/cliutils/cliexecuteutils.py
--rw-rw-rw-   0 root         (0) root         (0)     1303 2023-06-09 07:29:47.000000 ewokscore-0.5.0/src/ewokscore/cliutils/clilogutils.py
--rw-rw-rw-   0 root         (0) root         (0)     1344 2023-06-09 07:29:47.000000 ewokscore-0.5.0/src/ewokscore/cliutils/utils.py
--rw-rw-rw-   0 root         (0) root         (0)      752 2023-06-09 07:29:47.000000 ewokscore-0.5.0/src/ewokscore/dynamictask.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:41:46.000000 ewokscore-0.5.0/src/ewokscore/events/
--rw-rw-rw-   0 root         (0) root         (0)      590 2023-06-09 07:29:47.000000 ewokscore-0.5.0/src/ewokscore/events/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2826 2023-06-09 07:29:47.000000 ewokscore-0.5.0/src/ewokscore/events/contexts.py
--rw-rw-rw-   0 root         (0) root         (0)     4996 2023-06-09 07:29:47.000000 ewokscore-0.5.0/src/ewokscore/events/global_state.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:41:46.000000 ewokscore-0.5.0/src/ewokscore/events/handlers/
--rw-rw-rw-   0 root         (0) root         (0)      191 2023-06-09 07:29:47.000000 ewokscore-0.5.0/src/ewokscore/events/handlers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      503 2023-06-09 07:29:47.000000 ewokscore-0.5.0/src/ewokscore/events/handlers/base.py
--rw-rw-rw-   0 root         (0) root         (0)      295 2023-06-09 07:29:47.000000 ewokscore-0.5.0/src/ewokscore/events/handlers/sqlite3.py
--rw-rw-rw-   0 root         (0) root         (0)     1896 2023-06-09 07:29:47.000000 ewokscore-0.5.0/src/ewokscore/events/initialize_events.py
--rw-rw-rw-   0 root         (0) root         (0)     8072 2023-06-09 07:29:47.000000 ewokscore-0.5.0/src/ewokscore/events/send_events.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:41:46.000000 ewokscore-0.5.0/src/ewokscore/graph/
--rw-rw-rw-   0 root         (0) root         (0)       93 2023-06-09 07:29:47.000000 ewokscore-0.5.0/src/ewokscore/graph/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12469 2023-06-09 07:29:47.000000 ewokscore-0.5.0/src/ewokscore/graph/analysis.py
--rw-rw-rw-   0 root         (0) root         (0)     1822 2023-06-09 07:29:47.000000 ewokscore-0.5.0/src/ewokscore/graph/compare.py
--rw-rw-rw-   0 root         (0) root         (0)     2337 2023-06-09 07:29:47.000000 ewokscore-0.5.0/src/ewokscore/graph/error_handlers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:41:46.000000 ewokscore-0.5.0/src/ewokscore/graph/execute/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-09 07:41:40.000000 ewokscore-0.5.0/src/ewokscore/graph/execute/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4888 2023-06-09 07:29:47.000000 ewokscore-0.5.0/src/ewokscore/graph/execute/sequential.py
--rw-rw-rw-   0 root         (0) root         (0)     7034 2023-06-09 07:29:47.000000 ewokscore-0.5.0/src/ewokscore/graph/graph_io.py
--rw-rw-rw-   0 root         (0) root         (0)      855 2023-06-09 07:29:47.000000 ewokscore-0.5.0/src/ewokscore/graph/multigraph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:41:46.000000 ewokscore-0.5.0/src/ewokscore/graph/schema/
--rw-rw-rw-   0 root         (0) root         (0)     4434 2023-06-09 07:29:47.000000 ewokscore-0.5.0/src/ewokscore/graph/schema/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      154 2023-06-09 07:29:47.000000 ewokscore-0.5.0/src/ewokscore/graph/schema/v0_0.py
--rw-rw-rw-   0 root         (0) root         (0)      123 2023-06-09 07:29:47.000000 ewokscore-0.5.0/src/ewokscore/graph/schema/v0_1.py
--rw-rw-rw-   0 root         (0) root         (0)      156 2023-06-09 07:29:47.000000 ewokscore-0.5.0/src/ewokscore/graph/schema/v0_2.py
--rw-rw-rw-   0 root         (0) root         (0)     6803 2023-06-09 07:29:47.000000 ewokscore-0.5.0/src/ewokscore/graph/serialize.py
--rw-rw-rw-   0 root         (0) root         (0)    10989 2023-06-09 07:29:47.000000 ewokscore-0.5.0/src/ewokscore/graph/subgraph.py
--rw-rw-rw-   0 root         (0) root         (0)     5556 2023-06-09 07:29:47.000000 ewokscore-0.5.0/src/ewokscore/graph/taskgraph.py
--rw-rw-rw-   0 root         (0) root         (0)     2043 2023-06-09 07:29:47.000000 ewokscore-0.5.0/src/ewokscore/graph/validate.py
--rw-rw-rw-   0 root         (0) root         (0)     8690 2023-06-09 07:29:47.000000 ewokscore-0.5.0/src/ewokscore/hashing.py
--rw-rw-rw-   0 root         (0) root         (0)     8562 2023-06-09 07:29:47.000000 ewokscore-0.5.0/src/ewokscore/inittask.py
--rw-rw-rw-   0 root         (0) root         (0)      538 2023-06-09 07:29:47.000000 ewokscore-0.5.0/src/ewokscore/methodtask.py
--rw-rw-rw-   0 root         (0) root         (0)      563 2023-06-09 07:29:47.000000 ewokscore-0.5.0/src/ewokscore/missing_data.py
--rw-rw-rw-   0 root         (0) root         (0)     1799 2023-06-09 07:29:47.000000 ewokscore-0.5.0/src/ewokscore/node.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:41:46.000000 ewokscore-0.5.0/src/ewokscore/persistence/
--rw-rw-rw-   0 root         (0) root         (0)      161 2023-06-09 07:29:47.000000 ewokscore-0.5.0/src/ewokscore/persistence/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1951 2023-06-09 07:29:47.000000 ewokscore-0.5.0/src/ewokscore/persistence/atomic.py
--rw-rw-rw-   0 root         (0) root         (0)     5623 2023-06-09 07:29:47.000000 ewokscore-0.5.0/src/ewokscore/persistence/file.py
--rw-rw-rw-   0 root         (0) root         (0)      757 2023-06-09 07:29:47.000000 ewokscore-0.5.0/src/ewokscore/persistence/json.py
--rw-rw-rw-   0 root         (0) root         (0)     2328 2023-06-09 07:29:47.000000 ewokscore-0.5.0/src/ewokscore/persistence/nexus.py
--rw-rw-rw-   0 root         (0) root         (0)     6064 2023-06-09 07:29:47.000000 ewokscore-0.5.0/src/ewokscore/persistence/proxy.py
--rw-rw-rw-   0 root         (0) root         (0)     3717 2023-06-09 07:29:47.000000 ewokscore-0.5.0/src/ewokscore/persistence/uri.py
--rw-rw-rw-   0 root         (0) root         (0)     1462 2023-06-09 07:29:47.000000 ewokscore-0.5.0/src/ewokscore/ppftasks.py
--rw-rw-rw-   0 root         (0) root         (0)     3415 2023-06-09 07:29:47.000000 ewokscore-0.5.0/src/ewokscore/progress.py
--rw-rw-rw-   0 root         (0) root         (0)     2264 2023-06-09 07:29:47.000000 ewokscore-0.5.0/src/ewokscore/registration.py
--rw-rw-rw-   0 root         (0) root         (0)      940 2023-06-09 07:29:47.000000 ewokscore-0.5.0/src/ewokscore/scripttask.py
--rw-rw-rw-   0 root         (0) root         (0)    14409 2023-06-09 07:29:47.000000 ewokscore-0.5.0/src/ewokscore/task.py
--rw-rw-rw-   0 root         (0) root         (0)     6169 2023-06-09 07:29:47.000000 ewokscore-0.5.0/src/ewokscore/task_discovery.py
--rw-rw-rw-   0 root         (0) root         (0)      977 2023-06-09 07:29:47.000000 ewokscore-0.5.0/src/ewokscore/taskwithprogress.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:41:46.000000 ewokscore-0.5.0/src/ewokscore/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-09 07:41:40.000000 ewokscore-0.5.0/src/ewokscore/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       89 2023-06-09 07:29:47.000000 ewokscore-0.5.0/src/ewokscore/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)      428 2023-06-09 07:29:47.000000 ewokscore-0.5.0/src/ewokscore/tests/discover_module.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:41:46.000000 ewokscore-0.5.0/src/ewokscore/tests/examples/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-09 07:41:40.000000 ewokscore-0.5.0/src/ewokscore/tests/examples/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:41:46.000000 ewokscore-0.5.0/src/ewokscore/tests/examples/graphs/
--rw-rw-rw-   0 root         (0) root         (0)      878 2023-06-09 07:29:47.000000 ewokscore-0.5.0/src/ewokscore/tests/examples/graphs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4825 2023-06-09 07:29:47.000000 ewokscore-0.5.0/src/ewokscore/tests/examples/graphs/acyclic1.py
--rw-rw-rw-   0 root         (0) root         (0)     2447 2023-06-09 07:29:47.000000 ewokscore-0.5.0/src/ewokscore/tests/examples/graphs/acyclic2.py
--rw-rw-rw-   0 root         (0) root         (0)     3029 2023-06-09 07:29:47.000000 ewokscore-0.5.0/src/ewokscore/tests/examples/graphs/acyclic3.py
--rw-rw-rw-   0 root         (0) root         (0)     3166 2023-06-09 07:29:47.000000 ewokscore-0.5.0/src/ewokscore/tests/examples/graphs/cyclic1.py
--rw-rw-rw-   0 root         (0) root         (0)     4139 2023-06-09 07:29:47.000000 ewokscore-0.5.0/src/ewokscore/tests/examples/graphs/demo.py
--rw-rw-rw-   0 root         (0) root         (0)       68 2023-06-09 07:29:47.000000 ewokscore-0.5.0/src/ewokscore/tests/examples/graphs/empty.py
--rw-rw-rw-   0 root         (0) root         (0)     1561 2023-06-09 07:29:47.000000 ewokscore-0.5.0/src/ewokscore/tests/examples/graphs/triangle1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:41:46.000000 ewokscore-0.5.0/src/ewokscore/tests/examples/loadtest/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-09 07:41:40.000000 ewokscore-0.5.0/src/ewokscore/tests/examples/loadtest/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      411 2023-06-09 07:29:47.000000 ewokscore-0.5.0/src/ewokscore/tests/examples/loadtest/graph.json
--rw-rw-rw-   0 root         (0) root         (0)      252 2023-06-09 07:29:47.000000 ewokscore-0.5.0/src/ewokscore/tests/examples/loadtest/subgraph.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:41:46.000000 ewokscore-0.5.0/src/ewokscore/tests/examples/tasks/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-09 07:41:40.000000 ewokscore-0.5.0/src/ewokscore/tests/examples/tasks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       76 2023-06-09 07:29:47.000000 ewokscore-0.5.0/src/ewokscore/tests/examples/tasks/addfunc.py
--rw-rw-rw-   0 root         (0) root         (0)      243 2023-06-09 07:29:47.000000 ewokscore-0.5.0/src/ewokscore/tests/examples/tasks/condsumtask.py
--rw-rw-rw-   0 root         (0) root         (0)      458 2023-06-09 07:29:47.000000 ewokscore-0.5.0/src/ewokscore/tests/examples/tasks/errorsumtask.py
--rw-rw-rw-   0 root         (0) root         (0)      381 2023-06-09 07:29:47.000000 ewokscore-0.5.0/src/ewokscore/tests/examples/tasks/nooutputtask.py
--rw-rw-rw-   0 root         (0) root         (0)      160 2023-06-09 07:29:47.000000 ewokscore-0.5.0/src/ewokscore/tests/examples/tasks/simplemethods.py
--rw-rw-rw-   0 root         (0) root         (0)      796 2023-06-09 07:29:47.000000 ewokscore-0.5.0/src/ewokscore/tests/examples/tasks/sumlist.py
--rw-rw-rw-   0 root         (0) root         (0)      693 2023-06-09 07:29:47.000000 ewokscore-0.5.0/src/ewokscore/tests/examples/tasks/sumtask.py
--rw-rw-rw-   0 root         (0) root         (0)     1671 2023-06-09 07:29:47.000000 ewokscore-0.5.0/src/ewokscore/tests/test_cli_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     7990 2023-06-09 07:29:47.000000 ewokscore-0.5.0/src/ewokscore/tests/test_default_error_handlers.py
--rw-rw-rw-   0 root         (0) root         (0)      827 2023-06-09 07:29:47.000000 ewokscore-0.5.0/src/ewokscore/tests/test_dynamic_tasks.py
--rw-rw-rw-   0 root         (0) root         (0)     2223 2023-06-09 07:29:47.000000 ewokscore-0.5.0/src/ewokscore/tests/test_events.py
--rw-rw-rw-   0 root         (0) root         (0)     4897 2023-06-09 07:29:47.000000 ewokscore-0.5.0/src/ewokscore/tests/test_examples.py
--rw-rw-rw-   0 root         (0) root         (0)     7341 2023-06-09 07:29:47.000000 ewokscore-0.5.0/src/ewokscore/tests/test_execute_graph.py
--rw-rw-rw-   0 root         (0) root         (0)     3896 2023-06-09 07:29:47.000000 ewokscore-0.5.0/src/ewokscore/tests/test_graph.py
--rw-rw-rw-   0 root         (0) root         (0)     6597 2023-06-09 07:29:47.000000 ewokscore-0.5.0/src/ewokscore/tests/test_graph_io.py
--rw-rw-rw-   0 root         (0) root         (0)     1473 2023-06-09 07:29:47.000000 ewokscore-0.5.0/src/ewokscore/tests/test_graph_schema.py
--rw-rw-rw-   0 root         (0) root         (0)     2700 2023-06-09 07:29:47.000000 ewokscore-0.5.0/src/ewokscore/tests/test_graph_serialize.py
--rw-rw-rw-   0 root         (0) root         (0)     2854 2023-06-09 07:29:47.000000 ewokscore-0.5.0/src/ewokscore/tests/test_graph_start_end_nodes.py
--rw-rw-rw-   0 root         (0) root         (0)     4107 2023-06-09 07:29:47.000000 ewokscore-0.5.0/src/ewokscore/tests/test_hashing.py
--rw-rw-rw-   0 root         (0) root         (0)     7463 2023-06-09 07:29:47.000000 ewokscore-0.5.0/src/ewokscore/tests/test_link_is_required.py
--rw-rw-rw-   0 root         (0) root         (0)     1610 2023-06-09 07:29:47.000000 ewokscore-0.5.0/src/ewokscore/tests/test_method_task.py
--rw-rw-rw-   0 root         (0) root         (0)     3810 2023-06-09 07:29:47.000000 ewokscore-0.5.0/src/ewokscore/tests/test_persistence.py
--rw-rw-rw-   0 root         (0) root         (0)     1964 2023-06-09 07:29:47.000000 ewokscore-0.5.0/src/ewokscore/tests/test_script_task.py
--rw-rw-rw-   0 root         (0) root         (0)     8223 2023-06-09 07:29:47.000000 ewokscore-0.5.0/src/ewokscore/tests/test_sub_graph.py
--rw-rw-rw-   0 root         (0) root         (0)    10843 2023-06-09 07:29:47.000000 ewokscore-0.5.0/src/ewokscore/tests/test_sub_graph_serialize.py
--rw-rw-rw-   0 root         (0) root         (0)     4985 2023-06-09 07:29:47.000000 ewokscore-0.5.0/src/ewokscore/tests/test_task.py
--rw-rw-rw-   0 root         (0) root         (0)     6167 2023-06-09 07:29:47.000000 ewokscore-0.5.0/src/ewokscore/tests/test_task_discovery.py
--rw-rw-rw-   0 root         (0) root         (0)     1802 2023-06-09 07:29:47.000000 ewokscore-0.5.0/src/ewokscore/tests/test_task_progress.py
--rw-rw-rw-   0 root         (0) root         (0)     2213 2023-06-09 07:29:47.000000 ewokscore-0.5.0/src/ewokscore/tests/test_uri.py
--rw-rw-rw-   0 root         (0) root         (0)    14406 2023-06-09 07:29:47.000000 ewokscore-0.5.0/src/ewokscore/tests/test_variable.py
--rw-rw-rw-   0 root         (0) root         (0)     2401 2023-06-09 07:29:47.000000 ewokscore-0.5.0/src/ewokscore/tests/test_variable_namespaces.py
--rw-rw-rw-   0 root         (0) root         (0)     7495 2023-06-09 07:29:47.000000 ewokscore-0.5.0/src/ewokscore/tests/test_workflow_events.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:41:46.000000 ewokscore-0.5.0/src/ewokscore/tests/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-09 07:41:40.000000 ewokscore-0.5.0/src/ewokscore/tests/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4916 2023-06-09 07:29:47.000000 ewokscore-0.5.0/src/ewokscore/tests/utils/results.py
--rw-rw-rw-   0 root         (0) root         (0)      392 2023-06-09 07:29:47.000000 ewokscore-0.5.0/src/ewokscore/tests/utils/show.py
--rw-rw-rw-   0 root         (0) root         (0)     1182 2023-06-09 07:29:47.000000 ewokscore-0.5.0/src/ewokscore/utils.py
--rw-rw-rw-   0 root         (0) root         (0)    21421 2023-06-09 07:29:47.000000 ewokscore-0.5.0/src/ewokscore/variable.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:41:46.000000 ewokscore-0.5.0/src/ewokscore.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2638 2023-06-09 07:41:46.000000 ewokscore-0.5.0/src/ewokscore.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4215 2023-06-09 07:41:46.000000 ewokscore-0.5.0/src/ewokscore.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 07:41:46.000000 ewokscore-0.5.0/src/ewokscore.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      132 2023-06-09 07:41:46.000000 ewokscore-0.5.0/src/ewokscore.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      266 2023-06-09 07:41:46.000000 ewokscore-0.5.0/src/ewokscore.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-06-09 07:41:46.000000 ewokscore-0.5.0/src/ewokscore.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 17:22:22.000000 ewokscore-0.5.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1102 2023-06-09 07:29:47.000000 ewokscore-0.5.1/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)     2638 2023-06-09 17:22:22.000000 ewokscore-0.5.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1896 2023-06-09 07:29:47.000000 ewokscore-0.5.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      106 2023-06-09 07:29:47.000000 ewokscore-0.5.1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1427 2023-06-09 17:22:22.000000 ewokscore-0.5.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       69 2023-06-09 07:29:47.000000 ewokscore-0.5.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 17:22:22.000000 ewokscore-0.5.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 17:22:22.000000 ewokscore-0.5.1/src/ewokscore/
+-rw-rw-rw-   0 root         (0) root         (0)      164 2023-06-09 17:20:10.000000 ewokscore-0.5.1/src/ewokscore/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1721 2023-06-09 07:29:47.000000 ewokscore-0.5.1/src/ewokscore/bindings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 17:22:22.000000 ewokscore-0.5.1/src/ewokscore/cliutils/
+-rw-rw-rw-   0 root         (0) root         (0)      738 2023-06-09 07:29:47.000000 ewokscore-0.5.1/src/ewokscore/cliutils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2997 2023-06-09 07:29:47.000000 ewokscore-0.5.1/src/ewokscore/cliutils/cliconvertutils.py
+-rw-rw-rw-   0 root         (0) root         (0)     4778 2023-06-09 07:29:47.000000 ewokscore-0.5.1/src/ewokscore/cliutils/cliexecuteutils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1303 2023-06-09 07:29:47.000000 ewokscore-0.5.1/src/ewokscore/cliutils/clilogutils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1344 2023-06-09 07:29:47.000000 ewokscore-0.5.1/src/ewokscore/cliutils/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      752 2023-06-09 07:29:47.000000 ewokscore-0.5.1/src/ewokscore/dynamictask.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 17:22:22.000000 ewokscore-0.5.1/src/ewokscore/events/
+-rw-rw-rw-   0 root         (0) root         (0)      590 2023-06-09 07:29:47.000000 ewokscore-0.5.1/src/ewokscore/events/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2826 2023-06-09 07:29:47.000000 ewokscore-0.5.1/src/ewokscore/events/contexts.py
+-rw-rw-rw-   0 root         (0) root         (0)     4996 2023-06-09 07:29:47.000000 ewokscore-0.5.1/src/ewokscore/events/global_state.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 17:22:22.000000 ewokscore-0.5.1/src/ewokscore/events/handlers/
+-rw-rw-rw-   0 root         (0) root         (0)      191 2023-06-09 07:29:47.000000 ewokscore-0.5.1/src/ewokscore/events/handlers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      503 2023-06-09 07:29:47.000000 ewokscore-0.5.1/src/ewokscore/events/handlers/base.py
+-rw-rw-rw-   0 root         (0) root         (0)      295 2023-06-09 07:29:47.000000 ewokscore-0.5.1/src/ewokscore/events/handlers/sqlite3.py
+-rw-rw-rw-   0 root         (0) root         (0)     1896 2023-06-09 07:29:47.000000 ewokscore-0.5.1/src/ewokscore/events/initialize_events.py
+-rw-rw-rw-   0 root         (0) root         (0)     8072 2023-06-09 07:29:47.000000 ewokscore-0.5.1/src/ewokscore/events/send_events.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 17:22:22.000000 ewokscore-0.5.1/src/ewokscore/graph/
+-rw-rw-rw-   0 root         (0) root         (0)       93 2023-06-09 07:29:47.000000 ewokscore-0.5.1/src/ewokscore/graph/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12469 2023-06-09 07:29:47.000000 ewokscore-0.5.1/src/ewokscore/graph/analysis.py
+-rw-rw-rw-   0 root         (0) root         (0)     1822 2023-06-09 07:29:47.000000 ewokscore-0.5.1/src/ewokscore/graph/compare.py
+-rw-rw-rw-   0 root         (0) root         (0)     2337 2023-06-09 07:29:47.000000 ewokscore-0.5.1/src/ewokscore/graph/error_handlers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 17:22:22.000000 ewokscore-0.5.1/src/ewokscore/graph/execute/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-09 17:22:16.000000 ewokscore-0.5.1/src/ewokscore/graph/execute/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4888 2023-06-09 07:29:47.000000 ewokscore-0.5.1/src/ewokscore/graph/execute/sequential.py
+-rw-rw-rw-   0 root         (0) root         (0)     7034 2023-06-09 07:29:47.000000 ewokscore-0.5.1/src/ewokscore/graph/graph_io.py
+-rw-rw-rw-   0 root         (0) root         (0)      855 2023-06-09 07:29:47.000000 ewokscore-0.5.1/src/ewokscore/graph/multigraph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 17:22:22.000000 ewokscore-0.5.1/src/ewokscore/graph/schema/
+-rw-rw-rw-   0 root         (0) root         (0)     4434 2023-06-09 07:29:47.000000 ewokscore-0.5.1/src/ewokscore/graph/schema/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      154 2023-06-09 07:29:47.000000 ewokscore-0.5.1/src/ewokscore/graph/schema/v0_0.py
+-rw-rw-rw-   0 root         (0) root         (0)      123 2023-06-09 07:29:47.000000 ewokscore-0.5.1/src/ewokscore/graph/schema/v0_1.py
+-rw-rw-rw-   0 root         (0) root         (0)      156 2023-06-09 07:29:47.000000 ewokscore-0.5.1/src/ewokscore/graph/schema/v0_2.py
+-rw-rw-rw-   0 root         (0) root         (0)     6803 2023-06-09 07:29:47.000000 ewokscore-0.5.1/src/ewokscore/graph/serialize.py
+-rw-rw-rw-   0 root         (0) root         (0)    10989 2023-06-09 07:29:47.000000 ewokscore-0.5.1/src/ewokscore/graph/subgraph.py
+-rw-rw-rw-   0 root         (0) root         (0)     5556 2023-06-09 07:29:47.000000 ewokscore-0.5.1/src/ewokscore/graph/taskgraph.py
+-rw-rw-rw-   0 root         (0) root         (0)     2043 2023-06-09 07:29:47.000000 ewokscore-0.5.1/src/ewokscore/graph/validate.py
+-rw-rw-rw-   0 root         (0) root         (0)     8690 2023-06-09 07:29:47.000000 ewokscore-0.5.1/src/ewokscore/hashing.py
+-rw-rw-rw-   0 root         (0) root         (0)     8562 2023-06-09 07:29:47.000000 ewokscore-0.5.1/src/ewokscore/inittask.py
+-rw-rw-rw-   0 root         (0) root         (0)      538 2023-06-09 07:29:47.000000 ewokscore-0.5.1/src/ewokscore/methodtask.py
+-rw-rw-rw-   0 root         (0) root         (0)      563 2023-06-09 07:29:47.000000 ewokscore-0.5.1/src/ewokscore/missing_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     1799 2023-06-09 07:29:47.000000 ewokscore-0.5.1/src/ewokscore/node.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 17:22:22.000000 ewokscore-0.5.1/src/ewokscore/persistence/
+-rw-rw-rw-   0 root         (0) root         (0)      161 2023-06-09 07:29:47.000000 ewokscore-0.5.1/src/ewokscore/persistence/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1951 2023-06-09 07:29:47.000000 ewokscore-0.5.1/src/ewokscore/persistence/atomic.py
+-rw-rw-rw-   0 root         (0) root         (0)     5623 2023-06-09 07:29:47.000000 ewokscore-0.5.1/src/ewokscore/persistence/file.py
+-rw-rw-rw-   0 root         (0) root         (0)      757 2023-06-09 07:29:47.000000 ewokscore-0.5.1/src/ewokscore/persistence/json.py
+-rw-rw-rw-   0 root         (0) root         (0)     2328 2023-06-09 07:29:47.000000 ewokscore-0.5.1/src/ewokscore/persistence/nexus.py
+-rw-rw-rw-   0 root         (0) root         (0)     6064 2023-06-09 07:29:47.000000 ewokscore-0.5.1/src/ewokscore/persistence/proxy.py
+-rw-rw-rw-   0 root         (0) root         (0)     3717 2023-06-09 07:29:47.000000 ewokscore-0.5.1/src/ewokscore/persistence/uri.py
+-rw-rw-rw-   0 root         (0) root         (0)     1462 2023-06-09 07:29:47.000000 ewokscore-0.5.1/src/ewokscore/ppftasks.py
+-rw-rw-rw-   0 root         (0) root         (0)     3415 2023-06-09 07:29:47.000000 ewokscore-0.5.1/src/ewokscore/progress.py
+-rw-rw-rw-   0 root         (0) root         (0)     2264 2023-06-09 07:29:47.000000 ewokscore-0.5.1/src/ewokscore/registration.py
+-rw-rw-rw-   0 root         (0) root         (0)      940 2023-06-09 07:29:47.000000 ewokscore-0.5.1/src/ewokscore/scripttask.py
+-rw-rw-rw-   0 root         (0) root         (0)    14409 2023-06-09 07:29:47.000000 ewokscore-0.5.1/src/ewokscore/task.py
+-rw-rw-rw-   0 root         (0) root         (0)     7329 2023-06-09 17:20:10.000000 ewokscore-0.5.1/src/ewokscore/task_discovery.py
+-rw-rw-rw-   0 root         (0) root         (0)      977 2023-06-09 07:29:47.000000 ewokscore-0.5.1/src/ewokscore/taskwithprogress.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 17:22:22.000000 ewokscore-0.5.1/src/ewokscore/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-09 17:22:16.000000 ewokscore-0.5.1/src/ewokscore/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       89 2023-06-09 07:29:47.000000 ewokscore-0.5.1/src/ewokscore/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)      428 2023-06-09 07:29:47.000000 ewokscore-0.5.1/src/ewokscore/tests/discover_module.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 17:22:22.000000 ewokscore-0.5.1/src/ewokscore/tests/examples/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-09 17:22:16.000000 ewokscore-0.5.1/src/ewokscore/tests/examples/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 17:22:22.000000 ewokscore-0.5.1/src/ewokscore/tests/examples/graphs/
+-rw-rw-rw-   0 root         (0) root         (0)      878 2023-06-09 07:29:47.000000 ewokscore-0.5.1/src/ewokscore/tests/examples/graphs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4825 2023-06-09 07:29:47.000000 ewokscore-0.5.1/src/ewokscore/tests/examples/graphs/acyclic1.py
+-rw-rw-rw-   0 root         (0) root         (0)     2447 2023-06-09 07:29:47.000000 ewokscore-0.5.1/src/ewokscore/tests/examples/graphs/acyclic2.py
+-rw-rw-rw-   0 root         (0) root         (0)     3029 2023-06-09 07:29:47.000000 ewokscore-0.5.1/src/ewokscore/tests/examples/graphs/acyclic3.py
+-rw-rw-rw-   0 root         (0) root         (0)     3166 2023-06-09 07:29:47.000000 ewokscore-0.5.1/src/ewokscore/tests/examples/graphs/cyclic1.py
+-rw-rw-rw-   0 root         (0) root         (0)     4139 2023-06-09 07:29:47.000000 ewokscore-0.5.1/src/ewokscore/tests/examples/graphs/demo.py
+-rw-rw-rw-   0 root         (0) root         (0)       68 2023-06-09 07:29:47.000000 ewokscore-0.5.1/src/ewokscore/tests/examples/graphs/empty.py
+-rw-rw-rw-   0 root         (0) root         (0)     1561 2023-06-09 07:29:47.000000 ewokscore-0.5.1/src/ewokscore/tests/examples/graphs/triangle1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 17:22:22.000000 ewokscore-0.5.1/src/ewokscore/tests/examples/loadtest/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-09 17:22:16.000000 ewokscore-0.5.1/src/ewokscore/tests/examples/loadtest/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      411 2023-06-09 07:29:47.000000 ewokscore-0.5.1/src/ewokscore/tests/examples/loadtest/graph.json
+-rw-rw-rw-   0 root         (0) root         (0)      252 2023-06-09 07:29:47.000000 ewokscore-0.5.1/src/ewokscore/tests/examples/loadtest/subgraph.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 17:22:22.000000 ewokscore-0.5.1/src/ewokscore/tests/examples/tasks/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-09 17:22:16.000000 ewokscore-0.5.1/src/ewokscore/tests/examples/tasks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       76 2023-06-09 07:29:47.000000 ewokscore-0.5.1/src/ewokscore/tests/examples/tasks/addfunc.py
+-rw-rw-rw-   0 root         (0) root         (0)      243 2023-06-09 07:29:47.000000 ewokscore-0.5.1/src/ewokscore/tests/examples/tasks/condsumtask.py
+-rw-rw-rw-   0 root         (0) root         (0)      458 2023-06-09 07:29:47.000000 ewokscore-0.5.1/src/ewokscore/tests/examples/tasks/errorsumtask.py
+-rw-rw-rw-   0 root         (0) root         (0)      381 2023-06-09 07:29:47.000000 ewokscore-0.5.1/src/ewokscore/tests/examples/tasks/nooutputtask.py
+-rw-rw-rw-   0 root         (0) root         (0)      160 2023-06-09 07:29:47.000000 ewokscore-0.5.1/src/ewokscore/tests/examples/tasks/simplemethods.py
+-rw-rw-rw-   0 root         (0) root         (0)      796 2023-06-09 07:29:47.000000 ewokscore-0.5.1/src/ewokscore/tests/examples/tasks/sumlist.py
+-rw-rw-rw-   0 root         (0) root         (0)      693 2023-06-09 07:29:47.000000 ewokscore-0.5.1/src/ewokscore/tests/examples/tasks/sumtask.py
+-rw-rw-rw-   0 root         (0) root         (0)     1671 2023-06-09 07:29:47.000000 ewokscore-0.5.1/src/ewokscore/tests/test_cli_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     7990 2023-06-09 07:29:47.000000 ewokscore-0.5.1/src/ewokscore/tests/test_default_error_handlers.py
+-rw-rw-rw-   0 root         (0) root         (0)      827 2023-06-09 07:29:47.000000 ewokscore-0.5.1/src/ewokscore/tests/test_dynamic_tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)     2223 2023-06-09 07:29:47.000000 ewokscore-0.5.1/src/ewokscore/tests/test_events.py
+-rw-rw-rw-   0 root         (0) root         (0)     4897 2023-06-09 07:29:47.000000 ewokscore-0.5.1/src/ewokscore/tests/test_examples.py
+-rw-rw-rw-   0 root         (0) root         (0)     7341 2023-06-09 07:29:47.000000 ewokscore-0.5.1/src/ewokscore/tests/test_execute_graph.py
+-rw-rw-rw-   0 root         (0) root         (0)     3896 2023-06-09 07:29:47.000000 ewokscore-0.5.1/src/ewokscore/tests/test_graph.py
+-rw-rw-rw-   0 root         (0) root         (0)     6597 2023-06-09 07:29:47.000000 ewokscore-0.5.1/src/ewokscore/tests/test_graph_io.py
+-rw-rw-rw-   0 root         (0) root         (0)     1473 2023-06-09 07:29:47.000000 ewokscore-0.5.1/src/ewokscore/tests/test_graph_schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     2700 2023-06-09 07:29:47.000000 ewokscore-0.5.1/src/ewokscore/tests/test_graph_serialize.py
+-rw-rw-rw-   0 root         (0) root         (0)     2854 2023-06-09 07:29:47.000000 ewokscore-0.5.1/src/ewokscore/tests/test_graph_start_end_nodes.py
+-rw-rw-rw-   0 root         (0) root         (0)     4107 2023-06-09 07:29:47.000000 ewokscore-0.5.1/src/ewokscore/tests/test_hashing.py
+-rw-rw-rw-   0 root         (0) root         (0)     7463 2023-06-09 07:29:47.000000 ewokscore-0.5.1/src/ewokscore/tests/test_link_is_required.py
+-rw-rw-rw-   0 root         (0) root         (0)     1610 2023-06-09 07:29:47.000000 ewokscore-0.5.1/src/ewokscore/tests/test_method_task.py
+-rw-rw-rw-   0 root         (0) root         (0)     3810 2023-06-09 07:29:47.000000 ewokscore-0.5.1/src/ewokscore/tests/test_persistence.py
+-rw-rw-rw-   0 root         (0) root         (0)     1964 2023-06-09 07:29:47.000000 ewokscore-0.5.1/src/ewokscore/tests/test_script_task.py
+-rw-rw-rw-   0 root         (0) root         (0)     8223 2023-06-09 07:29:47.000000 ewokscore-0.5.1/src/ewokscore/tests/test_sub_graph.py
+-rw-rw-rw-   0 root         (0) root         (0)    10843 2023-06-09 07:29:47.000000 ewokscore-0.5.1/src/ewokscore/tests/test_sub_graph_serialize.py
+-rw-rw-rw-   0 root         (0) root         (0)     4985 2023-06-09 07:29:47.000000 ewokscore-0.5.1/src/ewokscore/tests/test_task.py
+-rw-rw-rw-   0 root         (0) root         (0)     6167 2023-06-09 07:29:47.000000 ewokscore-0.5.1/src/ewokscore/tests/test_task_discovery.py
+-rw-rw-rw-   0 root         (0) root         (0)     1802 2023-06-09 07:29:47.000000 ewokscore-0.5.1/src/ewokscore/tests/test_task_progress.py
+-rw-rw-rw-   0 root         (0) root         (0)     2213 2023-06-09 07:29:47.000000 ewokscore-0.5.1/src/ewokscore/tests/test_uri.py
+-rw-rw-rw-   0 root         (0) root         (0)    14406 2023-06-09 07:29:47.000000 ewokscore-0.5.1/src/ewokscore/tests/test_variable.py
+-rw-rw-rw-   0 root         (0) root         (0)     2401 2023-06-09 07:29:47.000000 ewokscore-0.5.1/src/ewokscore/tests/test_variable_namespaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     7495 2023-06-09 07:29:47.000000 ewokscore-0.5.1/src/ewokscore/tests/test_workflow_events.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 17:22:22.000000 ewokscore-0.5.1/src/ewokscore/tests/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-09 17:22:16.000000 ewokscore-0.5.1/src/ewokscore/tests/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4916 2023-06-09 07:29:47.000000 ewokscore-0.5.1/src/ewokscore/tests/utils/results.py
+-rw-rw-rw-   0 root         (0) root         (0)      392 2023-06-09 07:29:47.000000 ewokscore-0.5.1/src/ewokscore/tests/utils/show.py
+-rw-rw-rw-   0 root         (0) root         (0)     1182 2023-06-09 07:29:47.000000 ewokscore-0.5.1/src/ewokscore/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    21421 2023-06-09 07:29:47.000000 ewokscore-0.5.1/src/ewokscore/variable.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 17:22:22.000000 ewokscore-0.5.1/src/ewokscore.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2638 2023-06-09 17:22:22.000000 ewokscore-0.5.1/src/ewokscore.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4215 2023-06-09 17:22:22.000000 ewokscore-0.5.1/src/ewokscore.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 17:22:22.000000 ewokscore-0.5.1/src/ewokscore.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      132 2023-06-09 17:22:22.000000 ewokscore-0.5.1/src/ewokscore.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      266 2023-06-09 17:22:22.000000 ewokscore-0.5.1/src/ewokscore.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-06-09 17:22:22.000000 ewokscore-0.5.1/src/ewokscore.egg-info/top_level.txt
```

### Comparing `ewokscore-0.5.0/LICENSE.md` & `ewokscore-0.5.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ewokscore-0.5.0/PKG-INFO` & `ewokscore-0.5.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ewokscore
-Version: 0.5.0
+Version: 0.5.1
 Summary: API for graphs and tasks in Ewoks
 Home-page: https://gitlab.esrf.fr/workflow/ewoks/ewokscore/
 Author: ESRF
 Author-email: wout.de_nolf@esrf.fr
 License: MIT
 Project-URL: Source, https://gitlab.esrf.fr/workflow/ewoks/ewokscore/
 Project-URL: Documentation, https://ewokscore.readthedocs.io/
```

### Comparing `ewokscore-0.5.0/README.md` & `ewokscore-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `ewokscore-0.5.0/setup.cfg` & `ewokscore-0.5.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `ewokscore-0.5.0/src/ewokscore/bindings.py` & `ewokscore-0.5.1/src/ewokscore/bindings.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.5.0/src/ewokscore/cliutils/__init__.py` & `ewokscore-0.5.1/src/ewokscore/cliutils/__init__.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.5.0/src/ewokscore/cliutils/cliconvertutils.py` & `ewokscore-0.5.1/src/ewokscore/cliutils/cliconvertutils.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.5.0/src/ewokscore/cliutils/cliexecuteutils.py` & `ewokscore-0.5.1/src/ewokscore/cliutils/cliexecuteutils.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.5.0/src/ewokscore/cliutils/clilogutils.py` & `ewokscore-0.5.1/src/ewokscore/cliutils/clilogutils.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.5.0/src/ewokscore/cliutils/utils.py` & `ewokscore-0.5.1/src/ewokscore/cliutils/utils.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.5.0/src/ewokscore/dynamictask.py` & `ewokscore-0.5.1/src/ewokscore/dynamictask.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.5.0/src/ewokscore/events/__init__.py` & `ewokscore-0.5.1/src/ewokscore/events/__init__.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.5.0/src/ewokscore/events/contexts.py` & `ewokscore-0.5.1/src/ewokscore/events/contexts.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.5.0/src/ewokscore/events/global_state.py` & `ewokscore-0.5.1/src/ewokscore/events/global_state.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.5.0/src/ewokscore/events/initialize_events.py` & `ewokscore-0.5.1/src/ewokscore/events/initialize_events.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.5.0/src/ewokscore/events/send_events.py` & `ewokscore-0.5.1/src/ewokscore/events/send_events.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.5.0/src/ewokscore/graph/analysis.py` & `ewokscore-0.5.1/src/ewokscore/graph/analysis.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.5.0/src/ewokscore/graph/compare.py` & `ewokscore-0.5.1/src/ewokscore/graph/compare.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.5.0/src/ewokscore/graph/error_handlers.py` & `ewokscore-0.5.1/src/ewokscore/graph/error_handlers.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.5.0/src/ewokscore/graph/execute/sequential.py` & `ewokscore-0.5.1/src/ewokscore/graph/execute/sequential.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.5.0/src/ewokscore/graph/graph_io.py` & `ewokscore-0.5.1/src/ewokscore/graph/graph_io.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.5.0/src/ewokscore/graph/multigraph.py` & `ewokscore-0.5.1/src/ewokscore/graph/multigraph.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.5.0/src/ewokscore/graph/schema/__init__.py` & `ewokscore-0.5.1/src/ewokscore/graph/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.5.0/src/ewokscore/graph/serialize.py` & `ewokscore-0.5.1/src/ewokscore/graph/serialize.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.5.0/src/ewokscore/graph/subgraph.py` & `ewokscore-0.5.1/src/ewokscore/graph/subgraph.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.5.0/src/ewokscore/graph/taskgraph.py` & `ewokscore-0.5.1/src/ewokscore/graph/taskgraph.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.5.0/src/ewokscore/graph/validate.py` & `ewokscore-0.5.1/src/ewokscore/graph/validate.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.5.0/src/ewokscore/hashing.py` & `ewokscore-0.5.1/src/ewokscore/hashing.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.5.0/src/ewokscore/inittask.py` & `ewokscore-0.5.1/src/ewokscore/inittask.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.5.0/src/ewokscore/methodtask.py` & `ewokscore-0.5.1/src/ewokscore/methodtask.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.5.0/src/ewokscore/missing_data.py` & `ewokscore-0.5.1/src/ewokscore/missing_data.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.5.0/src/ewokscore/node.py` & `ewokscore-0.5.1/src/ewokscore/node.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.5.0/src/ewokscore/persistence/atomic.py` & `ewokscore-0.5.1/src/ewokscore/persistence/atomic.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.5.0/src/ewokscore/persistence/file.py` & `ewokscore-0.5.1/src/ewokscore/persistence/file.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.5.0/src/ewokscore/persistence/json.py` & `ewokscore-0.5.1/src/ewokscore/persistence/json.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.5.0/src/ewokscore/persistence/nexus.py` & `ewokscore-0.5.1/src/ewokscore/persistence/nexus.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.5.0/src/ewokscore/persistence/proxy.py` & `ewokscore-0.5.1/src/ewokscore/persistence/proxy.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.5.0/src/ewokscore/persistence/uri.py` & `ewokscore-0.5.1/src/ewokscore/persistence/uri.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.5.0/src/ewokscore/ppftasks.py` & `ewokscore-0.5.1/src/ewokscore/ppftasks.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.5.0/src/ewokscore/progress.py` & `ewokscore-0.5.1/src/ewokscore/progress.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.5.0/src/ewokscore/registration.py` & `ewokscore-0.5.1/src/ewokscore/registration.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.5.0/src/ewokscore/scripttask.py` & `ewokscore-0.5.1/src/ewokscore/scripttask.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.5.0/src/ewokscore/task.py` & `ewokscore-0.5.1/src/ewokscore/task.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.5.0/src/ewokscore/task_discovery.py` & `ewokscore-0.5.1/src/ewokscore/task_discovery.py`

 * *Files 24% similar despite different names*

```diff
@@ -14,40 +14,56 @@
 from .task import Task
 
 
 logger = logging.getLogger(__name__)
 
 
 def discover_tasks_from_modules(
-    *module_names: Iterable[str], task_type="class", reload: bool = False
+    *module_names: Iterable[str],
+    task_type="class",
+    reload: bool = False,
+    raise_import_failure: bool = True,
 ) -> List[Dict[str, str]]:
     return list(
         iter_discover_tasks_from_modules(
-            *module_names, task_type=task_type, reload=reload
+            *module_names,
+            task_type=task_type,
+            reload=reload,
+            raise_import_failure=raise_import_failure,
         )
     )
 
 
 def iter_discover_tasks_from_modules(
-    *module_names: Iterable[str], task_type="class", reload: bool = False
+    *module_names: Iterable[str],
+    task_type="class",
+    reload: bool = False,
+    raise_import_failure: bool = True,
 ) -> Generator[Dict[str, str], None, None]:
     if "" not in sys.path:
         # This happens when the python process was launched
         # through a python console script
         sys.path.append("")
 
     if task_type == "method":
-        yield from _iter_method_tasks(*module_names, reload=reload)
+        yield from _iter_method_tasks(
+            *module_names, reload=reload, raise_import_failure=raise_import_failure
+        )
     elif task_type == "ppfmethod":
         yield from _iter_method_tasks(
-            *module_names, filter_method_name=lambda name: name == "run", reload=reload
+            *module_names,
+            filter_method_name=lambda name: name == "run",
+            reload=reload,
+            raise_import_failure=raise_import_failure,
         )
     elif task_type == "class":
         for module_name in module_names:
-            _safe_import_module(module_name, reload=reload)
+            _safe_import_module(
+                module_name, reload=reload, raise_import_failure=raise_import_failure
+            )
         yield from _iter_registered_tasks(*module_names)
     else:
         raise ValueError("Class type does not support discovery")
 
 
 def _iter_registered_tasks(
     *filter_modules: Iterable[str],
@@ -72,20 +88,23 @@
         }
 
 
 def _iter_method_tasks(
     *module_names: Iterable[str],
     filter_method_name: Optional[Callable[[str], bool]] = None,
     reload: bool = False,
+    raise_import_failure: bool = False,
 ) -> Generator[Dict[str, str], None, None]:
     """Yields all task methods from the provided module_names. The module_names will be will
     imported for discovery.
     """
     for module_name in module_names:
-        mod = _safe_import_module(module_name, reload=reload)
+        mod = _safe_import_module(
+            module_name, reload=reload, raise_import_failure=raise_import_failure
+        )
         if mod is None:
             continue
         for method in inspect.getmembers(mod, inspect.isfunction):
             method_name, method_qn = method
             if filter_method_name and not filter_method_name(method_name):
                 continue
             if method_name.startswith("_"):
@@ -104,58 +123,80 @@
                 "output_names": ["return_value"],
                 "category": category,
                 "description": method.__doc__,
             }
 
 
 def iter_discover_all_tasks(
-    reload: bool = False,
+    reload: bool = False, raise_import_failure: bool = False
 ) -> Generator[Dict[str, str], None, None]:
     visited = set()
     for task_type in ("class", "ppfmethod", "method"):
         group = "ewoks.tasks." + task_type
         for entrypoint in pkg_resources.iter_entry_points(group):
             module_pattern = entrypoint.name
             if module_pattern is visited:
                 continue
             visited.add(module_pattern)
             for module_name in _iter_modules_from_pattern(
-                module_pattern, reload=reload
+                module_pattern, reload=reload, raise_import_failure=raise_import_failure
             ):
                 yield from iter_discover_tasks_from_modules(
-                    module_name, task_type=task_type, reload=reload
+                    module_name,
+                    task_type=task_type,
+                    reload=reload,
+                    raise_import_failure=raise_import_failure,
                 )
 
 
-def discover_all_tasks(reload: bool = False) -> Generator[Dict[str, str], None, None]:
-    return list(iter_discover_all_tasks(reload=reload))
+def discover_all_tasks(
+    reload: bool = False, raise_import_failure: bool = False
+) -> Generator[Dict[str, str], None, None]:
+    return list(
+        iter_discover_all_tasks(
+            reload=reload, raise_import_failure=raise_import_failure
+        )
+    )
 
 
 def _iter_modules_from_pattern(
-    module_pattern: str, reload: bool = False
+    module_pattern: str, reload: bool = False, raise_import_failure: bool = False
 ) -> Generator[str, None, None]:
     if "*" not in module_pattern:
         yield module_pattern
         return
     ndots = module_pattern.count(".")
     parts = module_pattern.split(".")
-    pkg = _safe_import_module(parts[0], reload=reload)
+    pkg = _safe_import_module(
+        parts[0], reload=reload, raise_import_failure=raise_import_failure
+    )
     if pkg is None:
         return
+    if raise_import_failure:
+
+        def onerror(module_name):
+            raise
+
+    else:
+        onerror = _onerror
     for pkginfo in pkgutil.walk_packages(
-        pkg.__path__, pkg.__name__ + ".", onerror=_onerror
+        pkg.__path__, pkg.__name__ + ".", onerror=onerror
     ):
         if pkginfo.name.count(".") == ndots and fnmatch(pkginfo.name, module_pattern):
             yield pkginfo.name
 
 
-def _safe_import_module(module_name: str, reload: bool = False) -> Optional[ModuleType]:
+def _safe_import_module(
+    module_name: str, reload: bool = False, raise_import_failure: bool = False
+) -> Optional[ModuleType]:
     try:
         return import_module(module_name, reload=reload)
-    except ImportError as e:
+    except Exception as e:
+        if raise_import_failure:
+            raise
         _onerror(module_name, exception=e)
 
 
 def _onerror(module_name, exception: Exception = None):
     if exception is None:
         exception = sys.exc_info()[1]
     logger.error(f"Module '{module_name}' cannot be imported: {exception}")
@@ -172,7 +213,10 @@
         if param.kind == param.VAR_KEYWORD:
             continue
         if required:
             required_input_names.append(name)
         else:
             optional_input_names.append(name)
     return required_input_names, optional_input_names
+
+
+print(discover_all_tasks(raise_import_failure=True))
```

### Comparing `ewokscore-0.5.0/src/ewokscore/taskwithprogress.py` & `ewokscore-0.5.1/src/ewokscore/taskwithprogress.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.5.0/src/ewokscore/tests/examples/graphs/__init__.py` & `ewokscore-0.5.1/src/ewokscore/tests/examples/graphs/__init__.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.5.0/src/ewokscore/tests/examples/graphs/acyclic1.py` & `ewokscore-0.5.1/src/ewokscore/tests/examples/graphs/acyclic1.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.5.0/src/ewokscore/tests/examples/graphs/acyclic2.py` & `ewokscore-0.5.1/src/ewokscore/tests/examples/graphs/acyclic2.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.5.0/src/ewokscore/tests/examples/graphs/acyclic3.py` & `ewokscore-0.5.1/src/ewokscore/tests/examples/graphs/acyclic3.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.5.0/src/ewokscore/tests/examples/graphs/cyclic1.py` & `ewokscore-0.5.1/src/ewokscore/tests/examples/graphs/cyclic1.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.5.0/src/ewokscore/tests/examples/graphs/demo.py` & `ewokscore-0.5.1/src/ewokscore/tests/examples/graphs/demo.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.5.0/src/ewokscore/tests/examples/graphs/triangle1.py` & `ewokscore-0.5.1/src/ewokscore/tests/examples/graphs/triangle1.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.5.0/src/ewokscore/tests/examples/tasks/sumlist.py` & `ewokscore-0.5.1/src/ewokscore/tests/examples/tasks/sumlist.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.5.0/src/ewokscore/tests/examples/tasks/sumtask.py` & `ewokscore-0.5.1/src/ewokscore/tests/examples/tasks/sumtask.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.5.0/src/ewokscore/tests/test_cli_utils.py` & `ewokscore-0.5.1/src/ewokscore/tests/test_cli_utils.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.5.0/src/ewokscore/tests/test_default_error_handlers.py` & `ewokscore-0.5.1/src/ewokscore/tests/test_default_error_handlers.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.5.0/src/ewokscore/tests/test_dynamic_tasks.py` & `ewokscore-0.5.1/src/ewokscore/tests/test_dynamic_tasks.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.5.0/src/ewokscore/tests/test_events.py` & `ewokscore-0.5.1/src/ewokscore/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.5.0/src/ewokscore/tests/test_examples.py` & `ewokscore-0.5.1/src/ewokscore/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.5.0/src/ewokscore/tests/test_execute_graph.py` & `ewokscore-0.5.1/src/ewokscore/tests/test_execute_graph.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.5.0/src/ewokscore/tests/test_graph.py` & `ewokscore-0.5.1/src/ewokscore/tests/test_graph.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.5.0/src/ewokscore/tests/test_graph_io.py` & `ewokscore-0.5.1/src/ewokscore/tests/test_graph_io.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.5.0/src/ewokscore/tests/test_graph_schema.py` & `ewokscore-0.5.1/src/ewokscore/tests/test_graph_schema.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.5.0/src/ewokscore/tests/test_graph_serialize.py` & `ewokscore-0.5.1/src/ewokscore/tests/test_graph_serialize.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.5.0/src/ewokscore/tests/test_graph_start_end_nodes.py` & `ewokscore-0.5.1/src/ewokscore/tests/test_graph_start_end_nodes.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.5.0/src/ewokscore/tests/test_hashing.py` & `ewokscore-0.5.1/src/ewokscore/tests/test_hashing.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.5.0/src/ewokscore/tests/test_link_is_required.py` & `ewokscore-0.5.1/src/ewokscore/tests/test_link_is_required.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.5.0/src/ewokscore/tests/test_method_task.py` & `ewokscore-0.5.1/src/ewokscore/tests/test_method_task.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.5.0/src/ewokscore/tests/test_persistence.py` & `ewokscore-0.5.1/src/ewokscore/tests/test_persistence.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.5.0/src/ewokscore/tests/test_script_task.py` & `ewokscore-0.5.1/src/ewokscore/tests/test_script_task.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.5.0/src/ewokscore/tests/test_sub_graph.py` & `ewokscore-0.5.1/src/ewokscore/tests/test_sub_graph.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.5.0/src/ewokscore/tests/test_sub_graph_serialize.py` & `ewokscore-0.5.1/src/ewokscore/tests/test_sub_graph_serialize.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.5.0/src/ewokscore/tests/test_task.py` & `ewokscore-0.5.1/src/ewokscore/tests/test_task.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.5.0/src/ewokscore/tests/test_task_discovery.py` & `ewokscore-0.5.1/src/ewokscore/tests/test_task_discovery.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.5.0/src/ewokscore/tests/test_task_progress.py` & `ewokscore-0.5.1/src/ewokscore/tests/test_task_progress.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.5.0/src/ewokscore/tests/test_uri.py` & `ewokscore-0.5.1/src/ewokscore/tests/test_uri.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.5.0/src/ewokscore/tests/test_variable.py` & `ewokscore-0.5.1/src/ewokscore/tests/test_variable.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.5.0/src/ewokscore/tests/test_variable_namespaces.py` & `ewokscore-0.5.1/src/ewokscore/tests/test_variable_namespaces.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.5.0/src/ewokscore/tests/test_workflow_events.py` & `ewokscore-0.5.1/src/ewokscore/tests/test_workflow_events.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.5.0/src/ewokscore/tests/utils/results.py` & `ewokscore-0.5.1/src/ewokscore/tests/utils/results.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.5.0/src/ewokscore/utils.py` & `ewokscore-0.5.1/src/ewokscore/utils.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.5.0/src/ewokscore/variable.py` & `ewokscore-0.5.1/src/ewokscore/variable.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.5.0/src/ewokscore.egg-info/PKG-INFO` & `ewokscore-0.5.1/src/ewokscore.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ewokscore
-Version: 0.5.0
+Version: 0.5.1
 Summary: API for graphs and tasks in Ewoks
 Home-page: https://gitlab.esrf.fr/workflow/ewoks/ewokscore/
 Author: ESRF
 Author-email: wout.de_nolf@esrf.fr
 License: MIT
 Project-URL: Source, https://gitlab.esrf.fr/workflow/ewoks/ewokscore/
 Project-URL: Documentation, https://ewokscore.readthedocs.io/
```

### Comparing `ewokscore-0.5.0/src/ewokscore.egg-info/SOURCES.txt` & `ewokscore-0.5.1/src/ewokscore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

