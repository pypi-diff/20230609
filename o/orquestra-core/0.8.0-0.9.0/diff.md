# Comparing `tmp/orquestra-core-0.8.0.tar.gz` & `tmp/orquestra-core-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orquestra-core-0.8.0.tar", last modified: Fri Jan 13 17:40:50 2023, max compression
+gzip compressed data, was "orquestra-core-0.9.0.tar", last modified: Wed Feb  8 00:04:15 2023, max compression
```

## Comparing `orquestra-core-0.8.0.tar` & `orquestra-core-0.9.0.tar`

### file list

```diff
@@ -1,125 +1,131 @@
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 17:40:50.536054 orquestra-core-0.8.0/
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 17:40:50.488476 orquestra-core-0.8.0/.github/
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 17:40:50.489576 orquestra-core-0.8.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 maxradin   (501) staff       (20)      605 2023-01-13 17:40:43.000000 orquestra-core-0.8.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 maxradin   (501) staff       (20)      600 2023-01-13 17:40:43.000000 orquestra-core-0.8.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 maxradin   (501) staff       (20)      533 2023-01-13 17:40:43.000000 orquestra-core-0.8.0/.github/pull_request_template.md
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 17:40:50.491411 orquestra-core-0.8.0/.github/workflows/
--rw-r--r--   0 maxradin   (501) staff       (20)     2192 2023-01-13 17:40:43.000000 orquestra-core-0.8.0/.github/workflows/coverage.yml
--rw-r--r--   0 maxradin   (501) staff       (20)      631 2023-01-13 17:40:43.000000 orquestra-core-0.8.0/.github/workflows/publish_docs.yml
--rw-r--r--   0 maxradin   (501) staff       (20)      878 2023-01-13 17:40:43.000000 orquestra-core-0.8.0/.github/workflows/publish_release.yml
--rw-r--r--   0 maxradin   (501) staff       (20)     2208 2023-01-13 17:40:43.000000 orquestra-core-0.8.0/.github/workflows/style.yml
--rw-r--r--   0 maxradin   (501) staff       (20)     1982 2023-01-13 17:40:43.000000 orquestra-core-0.8.0/.gitignore
--rw-r--r--   0 maxradin   (501) staff       (20)     5538 2023-01-13 17:40:43.000000 orquestra-core-0.8.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 maxradin   (501) staff       (20)     4817 2023-01-13 17:40:43.000000 orquestra-core-0.8.0/CONTRIBUTING.md
--rw-r--r--   0 maxradin   (501) staff       (20)    11357 2023-01-13 17:40:43.000000 orquestra-core-0.8.0/LICENSE
--rw-r--r--   0 maxradin   (501) staff       (20)     2903 2023-01-13 17:40:43.000000 orquestra-core-0.8.0/Makefile
--rw-r--r--   0 maxradin   (501) staff       (20)     3857 2023-01-13 17:40:50.536284 orquestra-core-0.8.0/PKG-INFO
--rw-r--r--   0 maxradin   (501) staff       (20)     3179 2023-01-13 17:40:43.000000 orquestra-core-0.8.0/README.md
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 17:40:50.498136 orquestra-core-0.8.0/docs/
--rw-r--r--   0 maxradin   (501) staff       (20)     2138 2023-01-13 17:40:43.000000 orquestra-core-0.8.0/docs/DOC_README.md
--rw-r--r--   0 maxradin   (501) staff       (20)      711 2023-01-13 17:40:43.000000 orquestra-core-0.8.0/docs/Makefile
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 17:40:50.504162 orquestra-core-0.8.0/docs/_static/
--rw-r--r--   0 maxradin   (501) staff       (20)    89573 2023-01-13 17:40:43.000000 orquestra-core-0.8.0/docs/_static/ZapataCLA.pdf
--rw-r--r--   0 maxradin   (501) staff       (20)    64068 2023-01-13 17:40:43.000000 orquestra-core-0.8.0/docs/_static/favicon.ico
--rw-r--r--   0 maxradin   (501) staff       (20)    46912 2023-01-13 17:40:43.000000 orquestra-core-0.8.0/docs/_static/orquestra.png
--rw-r--r--   0 maxradin   (501) staff       (20)     5052 2023-01-13 17:40:43.000000 orquestra-core-0.8.0/docs/conf.py
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 17:40:50.504874 orquestra-core-0.8.0/docs/examples/
--rw-r--r--   0 maxradin   (501) staff       (20)      261 2023-01-13 17:40:43.000000 orquestra-core-0.8.0/docs/examples/__init__.py
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 17:40:50.507673 orquestra-core-0.8.0/docs/examples/guides/
--rw-r--r--   0 maxradin   (501) staff       (20)     4273 2023-01-13 17:40:43.000000 orquestra-core-0.8.0/docs/examples/guides/circuit_runners_guide.py
--rw-r--r--   0 maxradin   (501) staff       (20)     3593 2023-01-13 17:40:43.000000 orquestra-core-0.8.0/docs/examples/guides/circuits_guide.py
--rw-r--r--   0 maxradin   (501) staff       (20)     2648 2023-01-13 17:40:43.000000 orquestra-core-0.8.0/docs/examples/guides/estimators_guide.py
--rw-r--r--   0 maxradin   (501) staff       (20)     1505 2023-01-13 17:40:43.000000 orquestra-core-0.8.0/docs/examples/guides/interfaces_guide.py
--rw-r--r--   0 maxradin   (501) staff       (20)     1115 2023-01-13 17:40:43.000000 orquestra-core-0.8.0/docs/examples/guides/mock_ansatz.py
--rw-r--r--   0 maxradin   (501) staff       (20)     5266 2023-01-13 17:40:43.000000 orquestra-core-0.8.0/docs/examples/guides/optimizers.py
--rw-r--r--   0 maxradin   (501) staff       (20)     3313 2023-01-13 17:40:43.000000 orquestra-core-0.8.0/docs/examples/guides/vqa_guide.py
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 17:40:50.508009 orquestra-core-0.8.0/docs/examples/tests/
--rw-r--r--   0 maxradin   (501) staff       (20)      261 2023-01-13 17:40:43.000000 orquestra-core-0.8.0/docs/examples/tests/__init__.py
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 17:40:50.510615 orquestra-core-0.8.0/docs/examples/tests/guides/
--rw-r--r--   0 maxradin   (501) staff       (20)      261 2023-01-13 17:40:43.000000 orquestra-core-0.8.0/docs/examples/tests/guides/__init__.py
--rw-r--r--   0 maxradin   (501) staff       (20)      462 2023-01-13 17:40:43.000000 orquestra-core-0.8.0/docs/examples/tests/guides/test_circuit_runners_guide.py
--rw-r--r--   0 maxradin   (501) staff       (20)      131 2023-01-13 17:40:43.000000 orquestra-core-0.8.0/docs/examples/tests/guides/test_circuits_guide.py
--rw-r--r--   0 maxradin   (501) staff       (20)      137 2023-01-13 17:40:43.000000 orquestra-core-0.8.0/docs/examples/tests/guides/test_estimators_guide.py
--rw-r--r--   0 maxradin   (501) staff       (20)      492 2023-01-13 17:40:43.000000 orquestra-core-0.8.0/docs/examples/tests/guides/test_mock_ansatz.py
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 17:40:50.512039 orquestra-core-0.8.0/docs/examples/tests/tutorials/
--rw-r--r--   0 maxradin   (501) staff       (20)      261 2023-01-13 17:40:43.000000 orquestra-core-0.8.0/docs/examples/tests/tutorials/__init__.py
--rw-r--r--   0 maxradin   (501) staff       (20)      273 2023-01-13 17:40:43.000000 orquestra-core-0.8.0/docs/examples/tests/tutorials/test_bell_state.py
--rw-r--r--   0 maxradin   (501) staff       (20)      186 2023-01-13 17:40:43.000000 orquestra-core-0.8.0/docs/examples/tests/tutorials/test_qaoa_maxcut.py
--rw-r--r--   0 maxradin   (501) staff       (20)      347 2023-01-13 17:40:43.000000 orquestra-core-0.8.0/docs/examples/tests/tutorials/test_superdense_coding.py
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 17:40:50.513332 orquestra-core-0.8.0/docs/examples/tutorials/
--rw-r--r--   0 maxradin   (501) staff       (20)     2204 2023-01-13 17:40:43.000000 orquestra-core-0.8.0/docs/examples/tutorials/bell_state.py
--rw-r--r--   0 maxradin   (501) staff       (20)     1943 2023-01-13 17:40:43.000000 orquestra-core-0.8.0/docs/examples/tutorials/qaoa_maxcut.py
--rw-r--r--   0 maxradin   (501) staff       (20)      642 2023-01-13 17:40:43.000000 orquestra-core-0.8.0/docs/examples/tutorials/superdense_coding.py
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 17:40:50.515939 orquestra-core-0.8.0/docs/guides/
--rw-r--r--   0 maxradin   (501) staff       (20)    19947 2023-01-13 17:40:43.000000 orquestra-core-0.8.0/docs/guides/circuit_runners.rst
--rw-r--r--   0 maxradin   (501) staff       (20)    26892 2023-01-13 17:40:43.000000 orquestra-core-0.8.0/docs/guides/circuits.rst
--rw-r--r--   0 maxradin   (501) staff       (20)     1772 2023-01-13 17:40:43.000000 orquestra-core-0.8.0/docs/guides/contributing.rst
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 17:40:50.516242 orquestra-core-0.8.0/docs/guides/images/
--rw-r--r--   0 maxradin   (501) staff       (20)  1087386 2023-01-13 17:40:43.000000 orquestra-core-0.8.0/docs/guides/images/orquestra_core_connection.excalidraw.png
--rw-r--r--   0 maxradin   (501) staff       (20)      270 2023-01-13 17:40:43.000000 orquestra-core-0.8.0/docs/guides/index.rst
--rw-r--r--   0 maxradin   (501) staff       (20)     6567 2023-01-13 17:40:43.000000 orquestra-core-0.8.0/docs/guides/interfaces.rst
--rw-r--r--   0 maxradin   (501) staff       (20)    18634 2023-01-13 17:40:43.000000 orquestra-core-0.8.0/docs/guides/optimizers.rst
--rw-r--r--   0 maxradin   (501) staff       (20)     2273 2023-01-13 17:40:43.000000 orquestra-core-0.8.0/docs/guides/orq_core_structure.rst
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 17:40:50.519763 orquestra-core-0.8.0/docs/guides/vqa_guide/
--rw-r--r--   0 maxradin   (501) staff       (20)     4366 2023-01-13 17:40:43.000000 orquestra-core-0.8.0/docs/guides/vqa_guide/ansatzes.rst
--rw-r--r--   0 maxradin   (501) staff       (20)    11433 2023-01-13 17:40:43.000000 orquestra-core-0.8.0/docs/guides/vqa_guide/estimators.rst
--rw-r--r--   0 maxradin   (501) staff       (20)      271 2023-01-13 17:40:43.000000 orquestra-core-0.8.0/docs/guides/vqa_guide/index.rst
--rw-r--r--   0 maxradin   (501) staff       (20)    15316 2023-01-13 17:40:43.000000 orquestra-core-0.8.0/docs/guides/vqa_guide/introduction.rst
--rw-r--r--   0 maxradin   (501) staff       (20)     5197 2023-01-13 17:40:43.000000 orquestra-core-0.8.0/docs/guides/vqa_guide/structure.rst
--rw-r--r--   0 maxradin   (501) staff       (20)     1366 2023-01-13 17:40:43.000000 orquestra-core-0.8.0/docs/index.rst
--rw-r--r--   0 maxradin   (501) staff       (20)      795 2023-01-13 17:40:43.000000 orquestra-core-0.8.0/docs/make.bat
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 17:40:50.520178 orquestra-core-0.8.0/docs/repos/
--rw-r--r--   0 maxradin   (501) staff       (20)     1436 2023-01-13 17:40:43.000000 orquestra-core-0.8.0/docs/repos/manifest.json
--rw-r--r--   0 maxradin   (501) staff       (20)      193 2023-01-13 17:40:43.000000 orquestra-core-0.8.0/docs/requirements.txt
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 17:40:50.521483 orquestra-core-0.8.0/docs/tutorials/
--rw-r--r--   0 maxradin   (501) staff       (20)     7783 2023-01-13 17:40:43.000000 orquestra-core-0.8.0/docs/tutorials/basic_qaoa.rst
--rw-r--r--   0 maxradin   (501) staff       (20)     7778 2023-01-13 17:40:43.000000 orquestra-core-0.8.0/docs/tutorials/beginner_tutorial.rst
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 17:40:50.523901 orquestra-core-0.8.0/docs/tutorials/images/
--rw-r--r--   0 maxradin   (501) staff       (20)   164941 2023-01-13 17:40:43.000000 orquestra-core-0.8.0/docs/tutorials/images/cut_graph.excalidraw.png
--rw-r--r--   0 maxradin   (501) staff       (20)   138951 2023-01-13 17:40:43.000000 orquestra-core-0.8.0/docs/tutorials/images/harder_graph.excalidraw.png
--rw-r--r--   0 maxradin   (501) staff       (20)   233342 2023-01-13 17:40:43.000000 orquestra-core-0.8.0/docs/tutorials/images/harder_graph_cut.excalidraw.png
--rw-r--r--   0 maxradin   (501) staff       (20)    86754 2023-01-13 17:40:43.000000 orquestra-core-0.8.0/docs/tutorials/images/uncut_graph.excalidraw.png
--rw-r--r--   0 maxradin   (501) staff       (20)       98 2023-01-13 17:40:43.000000 orquestra-core-0.8.0/docs/tutorials/index.rst
--rw-r--r--   0 maxradin   (501) staff       (20)     1259 2023-01-13 17:40:43.000000 orquestra-core-0.8.0/pyproject.toml
--rw-r--r--   0 maxradin   (501) staff       (20)     1219 2023-01-13 17:40:50.537103 orquestra-core-0.8.0/setup.cfg
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 17:40:50.524449 orquestra-core-0.8.0/src/
--rw-r--r--   0 maxradin   (501) staff       (20)        0 2023-01-13 17:40:43.000000 orquestra-core-0.8.0/src/dummy.py
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 17:40:50.526754 orquestra-core-0.8.0/src/orquestra_core.egg-info/
--rw-r--r--   0 maxradin   (501) staff       (20)     3857 2023-01-13 17:40:50.000000 orquestra-core-0.8.0/src/orquestra_core.egg-info/PKG-INFO
--rw-r--r--   0 maxradin   (501) staff       (20)     3327 2023-01-13 17:40:50.000000 orquestra-core-0.8.0/src/orquestra_core.egg-info/SOURCES.txt
--rw-r--r--   0 maxradin   (501) staff       (20)        1 2023-01-13 17:40:50.000000 orquestra-core-0.8.0/src/orquestra_core.egg-info/dependency_links.txt
--rw-r--r--   0 maxradin   (501) staff       (20)        1 2023-01-13 17:40:49.000000 orquestra-core-0.8.0/src/orquestra_core.egg-info/not-zip-safe
--rw-r--r--   0 maxradin   (501) staff       (20)      404 2023-01-13 17:40:50.000000 orquestra-core-0.8.0/src/orquestra_core.egg-info/requires.txt
--rw-r--r--   0 maxradin   (501) staff       (20)        1 2023-01-13 17:40:50.000000 orquestra-core-0.8.0/src/orquestra_core.egg-info/top_level.txt
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 17:40:50.482117 orquestra-core-0.8.0/subtrees/
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 17:40:50.530391 orquestra-core-0.8.0/subtrees/z_quantum_actions/
--rw-r--r--   0 maxradin   (501) staff       (20)        9 2023-01-13 17:40:43.000000 orquestra-core-0.8.0/subtrees/z_quantum_actions/MANIFEST.in
--rw-r--r--   0 maxradin   (501) staff       (20)     3699 2023-01-13 17:40:43.000000 orquestra-core-0.8.0/subtrees/z_quantum_actions/Makefile
--rw-r--r--   0 maxradin   (501) staff       (20)     5600 2023-01-13 17:40:43.000000 orquestra-core-0.8.0/subtrees/z_quantum_actions/README.rst
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 17:40:50.483096 orquestra-core-0.8.0/subtrees/z_quantum_actions/actions/
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 17:40:50.530761 orquestra-core-0.8.0/subtrees/z_quantum_actions/actions/coverage/
--rw-r--r--   0 maxradin   (501) staff       (20)      790 2023-01-13 17:40:43.000000 orquestra-core-0.8.0/subtrees/z_quantum_actions/actions/coverage/action.yml
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 17:40:50.531108 orquestra-core-0.8.0/subtrees/z_quantum_actions/actions/publish-release/
--rw-r--r--   0 maxradin   (501) staff       (20)     3132 2023-01-13 17:40:43.000000 orquestra-core-0.8.0/subtrees/z_quantum_actions/actions/publish-release/action.yml
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 17:40:50.531402 orquestra-core-0.8.0/subtrees/z_quantum_actions/actions/ssh_setup/
--rw-r--r--   0 maxradin   (501) staff       (20)      458 2023-01-13 17:40:43.000000 orquestra-core-0.8.0/subtrees/z_quantum_actions/actions/ssh_setup/action.yml
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 17:40:50.531886 orquestra-core-0.8.0/subtrees/z_quantum_actions/actions/style/
--rw-r--r--   0 maxradin   (501) staff       (20)      467 2023-01-13 17:40:43.000000 orquestra-core-0.8.0/subtrees/z_quantum_actions/actions/style/action.yml
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 17:40:50.532346 orquestra-core-0.8.0/subtrees/z_quantum_actions/bin/
--rwxr-xr-x   0 maxradin   (501) staff       (20)     2756 2023-01-13 17:40:43.000000 orquestra-core-0.8.0/subtrees/z_quantum_actions/bin/get_next_version.py
--rw-r--r--   0 maxradin   (501) staff       (20)     1253 2023-01-13 17:40:43.000000 orquestra-core-0.8.0/subtrees/z_quantum_actions/pyproject.toml
--rw-r--r--   0 maxradin   (501) staff       (20)       24 2023-01-13 17:40:43.000000 orquestra-core-0.8.0/subtrees/z_quantum_actions/pytest.ini
--rw-r--r--   0 maxradin   (501) staff       (20)     1526 2023-01-13 17:40:43.000000 orquestra-core-0.8.0/subtrees/z_quantum_actions/sample_setup.py
--rw-r--r--   0 maxradin   (501) staff       (20)      550 2023-01-13 17:40:43.000000 orquestra-core-0.8.0/subtrees/z_quantum_actions/setup_extras.py
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 17:40:50.532787 orquestra-core-0.8.0/subtrees/z_quantum_actions/tests/
--rw-r--r--   0 maxradin   (501) staff       (20)     1131 2023-01-13 17:40:43.000000 orquestra-core-0.8.0/subtrees/z_quantum_actions/tests/test_get_next_version.py
--rw-r--r--   0 maxradin   (501) staff       (20)       19 2023-01-13 17:40:43.000000 orquestra-core-0.8.0/subtrees/z_quantum_actions/variables.mk
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 17:40:50.534031 orquestra-core-0.8.0/subtrees/z_quantum_actions/workflow-templates/
--rw-r--r--   0 maxradin   (501) staff       (20)     1310 2023-01-13 17:40:43.000000 orquestra-core-0.8.0/subtrees/z_quantum_actions/workflow-templates/coverage.yml
--rw-r--r--   0 maxradin   (501) staff       (20)      999 2023-01-13 17:40:43.000000 orquestra-core-0.8.0/subtrees/z_quantum_actions/workflow-templates/publish-release.yml
--rw-r--r--   0 maxradin   (501) staff       (20)     1256 2023-01-13 17:40:43.000000 orquestra-core-0.8.0/subtrees/z_quantum_actions/workflow-templates/style.yml
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 17:40:50.535564 orquestra-core-0.8.0/tests/
--rw-r--r--   0 maxradin   (501) staff       (20)     4518 2023-01-13 17:40:43.000000 orquestra-core-0.8.0/tests/fh_vqe_test.py
--rw-r--r--   0 maxradin   (501) staff       (20)     2925 2023-01-13 17:40:43.000000 orquestra-core-0.8.0/tests/qaoa_maxcut_test.py
--rw-r--r--   0 maxradin   (501) staff       (20)     2858 2023-01-13 17:40:43.000000 orquestra-core-0.8.0/tests/qcbm_test.py
+drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-02-08 00:04:15.284805 orquestra-core-0.9.0/
+drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-02-08 00:04:15.252580 orquestra-core-0.9.0/.github/
+drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-02-08 00:04:15.253124 orquestra-core-0.9.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 maxradin   (501) staff       (20)      605 2023-02-08 00:04:06.000000 orquestra-core-0.9.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 maxradin   (501) staff       (20)      600 2023-02-08 00:04:06.000000 orquestra-core-0.9.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 maxradin   (501) staff       (20)      533 2023-02-08 00:04:06.000000 orquestra-core-0.9.0/.github/pull_request_template.md
+drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-02-08 00:04:15.254330 orquestra-core-0.9.0/.github/workflows/
+-rw-r--r--   0 maxradin   (501) staff       (20)     2334 2023-02-08 00:04:06.000000 orquestra-core-0.9.0/.github/workflows/coverage.yml
+-rw-r--r--   0 maxradin   (501) staff       (20)      631 2023-02-08 00:04:06.000000 orquestra-core-0.9.0/.github/workflows/publish_docs.yml
+-rw-r--r--   0 maxradin   (501) staff       (20)      878 2023-02-08 00:04:06.000000 orquestra-core-0.9.0/.github/workflows/publish_release.yml
+-rw-r--r--   0 maxradin   (501) staff       (20)     2352 2023-02-08 00:04:06.000000 orquestra-core-0.9.0/.github/workflows/style.yml
+-rw-r--r--   0 maxradin   (501) staff       (20)     1982 2023-02-08 00:04:06.000000 orquestra-core-0.9.0/.gitignore
+-rw-r--r--   0 maxradin   (501) staff       (20)     5538 2023-02-08 00:04:06.000000 orquestra-core-0.9.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 maxradin   (501) staff       (20)     4817 2023-02-08 00:04:06.000000 orquestra-core-0.9.0/CONTRIBUTING.md
+-rw-r--r--   0 maxradin   (501) staff       (20)    11357 2023-02-08 00:04:06.000000 orquestra-core-0.9.0/LICENSE
+-rw-r--r--   0 maxradin   (501) staff       (20)     2967 2023-02-08 00:04:06.000000 orquestra-core-0.9.0/Makefile
+-rw-r--r--   0 maxradin   (501) staff       (20)     4001 2023-02-08 00:04:15.285000 orquestra-core-0.9.0/PKG-INFO
+-rw-r--r--   0 maxradin   (501) staff       (20)     3280 2023-02-08 00:04:06.000000 orquestra-core-0.9.0/README.md
+drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-02-08 00:04:15.256440 orquestra-core-0.9.0/docs/
+-rw-r--r--   0 maxradin   (501) staff       (20)     2138 2023-02-08 00:04:06.000000 orquestra-core-0.9.0/docs/DOC_README.md
+-rw-r--r--   0 maxradin   (501) staff       (20)      711 2023-02-08 00:04:06.000000 orquestra-core-0.9.0/docs/Makefile
+drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-02-08 00:04:15.257581 orquestra-core-0.9.0/docs/_static/
+-rw-r--r--   0 maxradin   (501) staff       (20)    89573 2023-02-08 00:04:06.000000 orquestra-core-0.9.0/docs/_static/ZapataCLA.pdf
+-rw-r--r--   0 maxradin   (501) staff       (20)    64068 2023-02-08 00:04:06.000000 orquestra-core-0.9.0/docs/_static/favicon.ico
+-rw-r--r--   0 maxradin   (501) staff       (20)    46912 2023-02-08 00:04:06.000000 orquestra-core-0.9.0/docs/_static/orquestra.png
+-rw-r--r--   0 maxradin   (501) staff       (20)     5052 2023-02-08 00:04:06.000000 orquestra-core-0.9.0/docs/conf.py
+-rw-r--r--   0 maxradin   (501) staff       (20)     3675 2023-02-08 00:04:06.000000 orquestra-core-0.9.0/docs/getting_started.rst
+-rw-r--r--   0 maxradin   (501) staff       (20)     1517 2023-02-08 00:04:06.000000 orquestra-core-0.9.0/docs/index.rst
+-rw-r--r--   0 maxradin   (501) staff       (20)      795 2023-02-08 00:04:06.000000 orquestra-core-0.9.0/docs/make.bat
+drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-02-08 00:04:15.257933 orquestra-core-0.9.0/docs/quantum/
+drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-02-08 00:04:15.258257 orquestra-core-0.9.0/docs/quantum/examples/
+-rw-r--r--   0 maxradin   (501) staff       (20)      261 2023-02-08 00:04:06.000000 orquestra-core-0.9.0/docs/quantum/examples/__init__.py
+drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-02-08 00:04:15.260611 orquestra-core-0.9.0/docs/quantum/examples/guides/
+-rw-r--r--   0 maxradin   (501) staff       (20)     4267 2023-02-08 00:04:06.000000 orquestra-core-0.9.0/docs/quantum/examples/guides/circuit_runners_guide.py
+-rw-r--r--   0 maxradin   (501) staff       (20)     3593 2023-02-08 00:04:06.000000 orquestra-core-0.9.0/docs/quantum/examples/guides/circuits_guide.py
+-rw-r--r--   0 maxradin   (501) staff       (20)     2648 2023-02-08 00:04:06.000000 orquestra-core-0.9.0/docs/quantum/examples/guides/estimators_guide.py
+-rw-r--r--   0 maxradin   (501) staff       (20)     1505 2023-02-08 00:04:06.000000 orquestra-core-0.9.0/docs/quantum/examples/guides/interfaces_guide.py
+-rw-r--r--   0 maxradin   (501) staff       (20)     1115 2023-02-08 00:04:06.000000 orquestra-core-0.9.0/docs/quantum/examples/guides/mock_ansatz.py
+-rw-r--r--   0 maxradin   (501) staff       (20)     5266 2023-02-08 00:04:06.000000 orquestra-core-0.9.0/docs/quantum/examples/guides/optimizers.py
+-rw-r--r--   0 maxradin   (501) staff       (20)     3313 2023-02-08 00:04:06.000000 orquestra-core-0.9.0/docs/quantum/examples/guides/vqa_guide.py
+drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-02-08 00:04:15.260967 orquestra-core-0.9.0/docs/quantum/examples/tests/
+-rw-r--r--   0 maxradin   (501) staff       (20)      261 2023-02-08 00:04:06.000000 orquestra-core-0.9.0/docs/quantum/examples/tests/__init__.py
+drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-02-08 00:04:15.262875 orquestra-core-0.9.0/docs/quantum/examples/tests/guides/
+-rw-r--r--   0 maxradin   (501) staff       (20)      261 2023-02-08 00:04:06.000000 orquestra-core-0.9.0/docs/quantum/examples/tests/guides/__init__.py
+-rw-r--r--   0 maxradin   (501) staff       (20)      462 2023-02-08 00:04:06.000000 orquestra-core-0.9.0/docs/quantum/examples/tests/guides/test_circuit_runners_guide.py
+-rw-r--r--   0 maxradin   (501) staff       (20)      131 2023-02-08 00:04:06.000000 orquestra-core-0.9.0/docs/quantum/examples/tests/guides/test_circuits_guide.py
+-rw-r--r--   0 maxradin   (501) staff       (20)      137 2023-02-08 00:04:06.000000 orquestra-core-0.9.0/docs/quantum/examples/tests/guides/test_estimators_guide.py
+-rw-r--r--   0 maxradin   (501) staff       (20)      492 2023-02-08 00:04:06.000000 orquestra-core-0.9.0/docs/quantum/examples/tests/guides/test_mock_ansatz.py
+drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-02-08 00:04:15.264521 orquestra-core-0.9.0/docs/quantum/examples/tests/tutorials/
+-rw-r--r--   0 maxradin   (501) staff       (20)      261 2023-02-08 00:04:06.000000 orquestra-core-0.9.0/docs/quantum/examples/tests/tutorials/__init__.py
+-rw-r--r--   0 maxradin   (501) staff       (20)      273 2023-02-08 00:04:06.000000 orquestra-core-0.9.0/docs/quantum/examples/tests/tutorials/test_bell_state.py
+-rw-r--r--   0 maxradin   (501) staff       (20)      110 2023-02-08 00:04:06.000000 orquestra-core-0.9.0/docs/quantum/examples/tests/tutorials/test_orqviz.py
+-rw-r--r--   0 maxradin   (501) staff       (20)      186 2023-02-08 00:04:06.000000 orquestra-core-0.9.0/docs/quantum/examples/tests/tutorials/test_qaoa_maxcut.py
+-rw-r--r--   0 maxradin   (501) staff       (20)      347 2023-02-08 00:04:06.000000 orquestra-core-0.9.0/docs/quantum/examples/tests/tutorials/test_superdense_coding.py
+drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-02-08 00:04:15.265707 orquestra-core-0.9.0/docs/quantum/examples/tutorials/
+-rw-r--r--   0 maxradin   (501) staff       (20)     2206 2023-02-08 00:04:06.000000 orquestra-core-0.9.0/docs/quantum/examples/tutorials/bell_state.py
+-rw-r--r--   0 maxradin   (501) staff       (20)      565 2023-02-08 00:04:06.000000 orquestra-core-0.9.0/docs/quantum/examples/tutorials/orqviz.py
+-rw-r--r--   0 maxradin   (501) staff       (20)     1943 2023-02-08 00:04:06.000000 orquestra-core-0.9.0/docs/quantum/examples/tutorials/qaoa_maxcut.py
+-rw-r--r--   0 maxradin   (501) staff       (20)      642 2023-02-08 00:04:06.000000 orquestra-core-0.9.0/docs/quantum/examples/tutorials/superdense_coding.py
+drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-02-08 00:04:15.268092 orquestra-core-0.9.0/docs/quantum/guides/
+-rw-r--r--   0 maxradin   (501) staff       (20)    19947 2023-02-08 00:04:06.000000 orquestra-core-0.9.0/docs/quantum/guides/circuit_runners.rst
+-rw-r--r--   0 maxradin   (501) staff       (20)    26892 2023-02-08 00:04:06.000000 orquestra-core-0.9.0/docs/quantum/guides/circuits.rst
+-rw-r--r--   0 maxradin   (501) staff       (20)     1772 2023-02-08 00:04:06.000000 orquestra-core-0.9.0/docs/quantum/guides/contributing.rst
+drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-02-08 00:04:15.268594 orquestra-core-0.9.0/docs/quantum/guides/images/
+-rw-r--r--   0 maxradin   (501) staff       (20)  1087386 2023-02-08 00:04:06.000000 orquestra-core-0.9.0/docs/quantum/guides/images/orquestra_core_connection.excalidraw.png
+-rw-r--r--   0 maxradin   (501) staff       (20)      243 2023-02-08 00:04:06.000000 orquestra-core-0.9.0/docs/quantum/guides/index.rst
+-rw-r--r--   0 maxradin   (501) staff       (20)     6567 2023-02-08 00:04:06.000000 orquestra-core-0.9.0/docs/quantum/guides/interfaces.rst
+-rw-r--r--   0 maxradin   (501) staff       (20)    18634 2023-02-08 00:04:06.000000 orquestra-core-0.9.0/docs/quantum/guides/optimizers.rst
+drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-02-08 00:04:15.271166 orquestra-core-0.9.0/docs/quantum/guides/vqa_guide/
+-rw-r--r--   0 maxradin   (501) staff       (20)     4366 2023-02-08 00:04:06.000000 orquestra-core-0.9.0/docs/quantum/guides/vqa_guide/ansatzes.rst
+-rw-r--r--   0 maxradin   (501) staff       (20)    11433 2023-02-08 00:04:06.000000 orquestra-core-0.9.0/docs/quantum/guides/vqa_guide/estimators.rst
+-rw-r--r--   0 maxradin   (501) staff       (20)      271 2023-02-08 00:04:06.000000 orquestra-core-0.9.0/docs/quantum/guides/vqa_guide/index.rst
+-rw-r--r--   0 maxradin   (501) staff       (20)    15316 2023-02-08 00:04:06.000000 orquestra-core-0.9.0/docs/quantum/guides/vqa_guide/introduction.rst
+-rw-r--r--   0 maxradin   (501) staff       (20)     5197 2023-02-08 00:04:06.000000 orquestra-core-0.9.0/docs/quantum/guides/vqa_guide/structure.rst
+-rw-r--r--   0 maxradin   (501) staff       (20)     1168 2023-02-08 00:04:06.000000 orquestra-core-0.9.0/docs/quantum/index.rst
+drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-02-08 00:04:15.272566 orquestra-core-0.9.0/docs/quantum/tutorials/
+-rw-r--r--   0 maxradin   (501) staff       (20)     7783 2023-02-08 00:04:06.000000 orquestra-core-0.9.0/docs/quantum/tutorials/basic_qaoa.rst
+-rw-r--r--   0 maxradin   (501) staff       (20)     7442 2023-02-08 00:04:06.000000 orquestra-core-0.9.0/docs/quantum/tutorials/beginner_tutorial.rst
+drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-02-08 00:04:15.275183 orquestra-core-0.9.0/docs/quantum/tutorials/images/
+-rw-r--r--   0 maxradin   (501) staff       (20)    45998 2023-02-08 00:04:06.000000 orquestra-core-0.9.0/docs/quantum/tutorials/images/cost_function_landscape.png
+-rw-r--r--   0 maxradin   (501) staff       (20)   164941 2023-02-08 00:04:06.000000 orquestra-core-0.9.0/docs/quantum/tutorials/images/cut_graph.excalidraw.png
+-rw-r--r--   0 maxradin   (501) staff       (20)   138951 2023-02-08 00:04:06.000000 orquestra-core-0.9.0/docs/quantum/tutorials/images/harder_graph.excalidraw.png
+-rw-r--r--   0 maxradin   (501) staff       (20)   233342 2023-02-08 00:04:06.000000 orquestra-core-0.9.0/docs/quantum/tutorials/images/harder_graph_cut.excalidraw.png
+-rw-r--r--   0 maxradin   (501) staff       (20)    86754 2023-02-08 00:04:06.000000 orquestra-core-0.9.0/docs/quantum/tutorials/images/uncut_graph.excalidraw.png
+-rw-r--r--   0 maxradin   (501) staff       (20)      113 2023-02-08 00:04:06.000000 orquestra-core-0.9.0/docs/quantum/tutorials/index.rst
+-rw-r--r--   0 maxradin   (501) staff       (20)     3913 2023-02-08 00:04:06.000000 orquestra-core-0.9.0/docs/quantum/tutorials/orqviz.rst
+drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-02-08 00:04:15.275594 orquestra-core-0.9.0/docs/repos/
+-rw-r--r--   0 maxradin   (501) staff       (20)     1592 2023-02-08 00:04:06.000000 orquestra-core-0.9.0/docs/repos/manifest.json
+-rw-r--r--   0 maxradin   (501) staff       (20)      193 2023-02-08 00:04:06.000000 orquestra-core-0.9.0/docs/requirements.txt
+-rw-r--r--   0 maxradin   (501) staff       (20)     1319 2023-02-08 00:04:06.000000 orquestra-core-0.9.0/pyproject.toml
+-rw-r--r--   0 maxradin   (501) staff       (20)     1514 2023-02-08 00:04:15.285740 orquestra-core-0.9.0/setup.cfg
+drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-02-08 00:04:15.275947 orquestra-core-0.9.0/src/
+-rw-r--r--   0 maxradin   (501) staff       (20)        0 2023-02-08 00:04:06.000000 orquestra-core-0.9.0/src/dummy.py
+drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-02-08 00:04:15.277629 orquestra-core-0.9.0/src/orquestra_core.egg-info/
+-rw-r--r--   0 maxradin   (501) staff       (20)     4001 2023-02-08 00:04:15.000000 orquestra-core-0.9.0/src/orquestra_core.egg-info/PKG-INFO
+-rw-r--r--   0 maxradin   (501) staff       (20)     3847 2023-02-08 00:04:15.000000 orquestra-core-0.9.0/src/orquestra_core.egg-info/SOURCES.txt
+-rw-r--r--   0 maxradin   (501) staff       (20)        1 2023-02-08 00:04:15.000000 orquestra-core-0.9.0/src/orquestra_core.egg-info/dependency_links.txt
+-rw-r--r--   0 maxradin   (501) staff       (20)        1 2023-02-08 00:04:14.000000 orquestra-core-0.9.0/src/orquestra_core.egg-info/not-zip-safe
+-rw-r--r--   0 maxradin   (501) staff       (20)      687 2023-02-08 00:04:15.000000 orquestra-core-0.9.0/src/orquestra_core.egg-info/requires.txt
+-rw-r--r--   0 maxradin   (501) staff       (20)        1 2023-02-08 00:04:15.000000 orquestra-core-0.9.0/src/orquestra_core.egg-info/top_level.txt
+drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-02-08 00:04:15.247544 orquestra-core-0.9.0/subtrees/
+drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-02-08 00:04:15.280133 orquestra-core-0.9.0/subtrees/z_quantum_actions/
+-rw-r--r--   0 maxradin   (501) staff       (20)        9 2023-02-08 00:04:06.000000 orquestra-core-0.9.0/subtrees/z_quantum_actions/MANIFEST.in
+-rw-r--r--   0 maxradin   (501) staff       (20)     3699 2023-02-08 00:04:06.000000 orquestra-core-0.9.0/subtrees/z_quantum_actions/Makefile
+-rw-r--r--   0 maxradin   (501) staff       (20)     5600 2023-02-08 00:04:06.000000 orquestra-core-0.9.0/subtrees/z_quantum_actions/README.rst
+drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-02-08 00:04:15.248313 orquestra-core-0.9.0/subtrees/z_quantum_actions/actions/
+drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-02-08 00:04:15.280392 orquestra-core-0.9.0/subtrees/z_quantum_actions/actions/coverage/
+-rw-r--r--   0 maxradin   (501) staff       (20)      790 2023-02-08 00:04:06.000000 orquestra-core-0.9.0/subtrees/z_quantum_actions/actions/coverage/action.yml
+drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-02-08 00:04:15.280691 orquestra-core-0.9.0/subtrees/z_quantum_actions/actions/publish-release/
+-rw-r--r--   0 maxradin   (501) staff       (20)     3132 2023-02-08 00:04:06.000000 orquestra-core-0.9.0/subtrees/z_quantum_actions/actions/publish-release/action.yml
+drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-02-08 00:04:15.280949 orquestra-core-0.9.0/subtrees/z_quantum_actions/actions/ssh_setup/
+-rw-r--r--   0 maxradin   (501) staff       (20)      458 2023-02-08 00:04:06.000000 orquestra-core-0.9.0/subtrees/z_quantum_actions/actions/ssh_setup/action.yml
+drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-02-08 00:04:15.281274 orquestra-core-0.9.0/subtrees/z_quantum_actions/actions/style/
+-rw-r--r--   0 maxradin   (501) staff       (20)      467 2023-02-08 00:04:06.000000 orquestra-core-0.9.0/subtrees/z_quantum_actions/actions/style/action.yml
+drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-02-08 00:04:15.281682 orquestra-core-0.9.0/subtrees/z_quantum_actions/bin/
+-rwxr-xr-x   0 maxradin   (501) staff       (20)     2756 2023-02-08 00:04:06.000000 orquestra-core-0.9.0/subtrees/z_quantum_actions/bin/get_next_version.py
+-rw-r--r--   0 maxradin   (501) staff       (20)     1253 2023-02-08 00:04:06.000000 orquestra-core-0.9.0/subtrees/z_quantum_actions/pyproject.toml
+-rw-r--r--   0 maxradin   (501) staff       (20)       24 2023-02-08 00:04:06.000000 orquestra-core-0.9.0/subtrees/z_quantum_actions/pytest.ini
+-rw-r--r--   0 maxradin   (501) staff       (20)     1526 2023-02-08 00:04:06.000000 orquestra-core-0.9.0/subtrees/z_quantum_actions/sample_setup.py
+-rw-r--r--   0 maxradin   (501) staff       (20)      550 2023-02-08 00:04:06.000000 orquestra-core-0.9.0/subtrees/z_quantum_actions/setup_extras.py
+drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-02-08 00:04:15.282172 orquestra-core-0.9.0/subtrees/z_quantum_actions/tests/
+-rw-r--r--   0 maxradin   (501) staff       (20)     1131 2023-02-08 00:04:06.000000 orquestra-core-0.9.0/subtrees/z_quantum_actions/tests/test_get_next_version.py
+-rw-r--r--   0 maxradin   (501) staff       (20)       19 2023-02-08 00:04:06.000000 orquestra-core-0.9.0/subtrees/z_quantum_actions/variables.mk
+drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-02-08 00:04:15.283022 orquestra-core-0.9.0/subtrees/z_quantum_actions/workflow-templates/
+-rw-r--r--   0 maxradin   (501) staff       (20)     1310 2023-02-08 00:04:06.000000 orquestra-core-0.9.0/subtrees/z_quantum_actions/workflow-templates/coverage.yml
+-rw-r--r--   0 maxradin   (501) staff       (20)      999 2023-02-08 00:04:06.000000 orquestra-core-0.9.0/subtrees/z_quantum_actions/workflow-templates/publish-release.yml
+-rw-r--r--   0 maxradin   (501) staff       (20)     1256 2023-02-08 00:04:06.000000 orquestra-core-0.9.0/subtrees/z_quantum_actions/workflow-templates/style.yml
+drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-02-08 00:04:15.284616 orquestra-core-0.9.0/tests/
+-rw-r--r--   0 maxradin   (501) staff       (20)     4518 2023-02-08 00:04:06.000000 orquestra-core-0.9.0/tests/fh_vqe_test.py
+-rw-r--r--   0 maxradin   (501) staff       (20)     2925 2023-02-08 00:04:06.000000 orquestra-core-0.9.0/tests/qaoa_maxcut_test.py
+-rw-r--r--   0 maxradin   (501) staff       (20)     2858 2023-02-08 00:04:06.000000 orquestra-core-0.9.0/tests/qcbm_test.py
```

### Comparing `orquestra-core-0.8.0/.github/ISSUE_TEMPLATE/bug_report.md` & `orquestra-core-0.9.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `orquestra-core-0.8.0/.github/ISSUE_TEMPLATE/feature_request.md` & `orquestra-core-0.9.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `orquestra-core-0.8.0/.github/pull_request_template.md` & `orquestra-core-0.9.0/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `orquestra-core-0.8.0/.github/workflows/coverage.yml` & `orquestra-core-0.9.0/.github/workflows/coverage.yml`

 * *Files 2% similar despite different names*

```diff
@@ -73,10 +73,16 @@
 
       - name: Get orquestra-forest
         uses: actions/checkout@v2
         with:
           repository: zapatacomputing/orquestra-forest
           path: orquestra-forest
 
+      - name: Get orqviz
+        uses: actions/checkout@v2
+        with:
+          repository: zapatacomputing/orqviz
+          path: orqviz
+
       - uses: ./subtrees/z_quantum_actions/actions/coverage
         env:
           ZAPATA_IBMQ_API_TOKEN: ${{ secrets.ZAPATA_IBMQ_API_TOKEN }}
```

### Comparing `orquestra-core-0.8.0/.github/workflows/publish_docs.yml` & `orquestra-core-0.9.0/.github/workflows/publish_docs.yml`

 * *Files identical despite different names*

### Comparing `orquestra-core-0.8.0/.github/workflows/publish_release.yml` & `orquestra-core-0.9.0/.github/workflows/publish_release.yml`

 * *Files identical despite different names*

### Comparing `orquestra-core-0.8.0/.github/workflows/style.yml` & `orquestra-core-0.9.0/.github/workflows/style.yml`

 * *Files 6% similar despite different names*

```diff
@@ -72,12 +72,18 @@
           path: orquestra-braket
 
       - name: Get orquestra-forest
         uses: actions/checkout@v2
         with:
           repository: zapatacomputing/orquestra-forest
           path: orquestra-forest
+  
+      - name: Get orqviz
+        uses: actions/checkout@v2
+        with:
+          repository: zapatacomputing/orqviz
+          path: orqviz
 
       # Installs project, checks codestyle
       - uses: ./subtrees/z_quantum_actions/actions/style
         env:
           ZAPATA_IBMQ_API_TOKEN: ${{ secrets.ZAPATA_IBMQ_API_TOKEN }}
```

### Comparing `orquestra-core-0.8.0/.gitignore` & `orquestra-core-0.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `orquestra-core-0.8.0/CODE_OF_CONDUCT.md` & `orquestra-core-0.9.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `orquestra-core-0.8.0/CONTRIBUTING.md` & `orquestra-core-0.9.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `orquestra-core-0.8.0/LICENSE` & `orquestra-core-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `orquestra-core-0.8.0/Makefile` & `orquestra-core-0.9.0/Makefile`

 * *Files 4% similar despite different names*

```diff
@@ -29,19 +29,20 @@
 		${VENV_NAME}/bin/python3 -m pip install ./orquestra-opt[all] && \
 		${VENV_NAME}/bin/python3 -m pip install ./orquestra-vqa && \
 		${VENV_NAME}/bin/python3 -m pip install ./orquestra-qiskit && \
 		${VENV_NAME}/bin/python3 -m pip install ./orquestra-cirq[qsim] && \
 		${VENV_NAME}/bin/python3 -m pip install ./orquestra-qulacs && \
 		${VENV_NAME}/bin/python3 -m pip install ./orquestra-braket && \
 		${VENV_NAME}/bin/python3 -m pip install ./orquestra-forest && \
+		${VENV_NAME}/bin/python3 -m pip install ./orqviz && \
 		${VENV_NAME}/bin/python3 -m pip install -r docs/requirements.txt
 
 coverage:
 	$(PYTHON) -m pytest tests/
-	$(PYTHON) -m pytest docs/examples/tests
+	$(PYTHON) -m pytest docs/quantum/examples/tests
 
 # Runs tests with the latest dependncies from PyPI
 run_tests_before_release:
 	python3 -m venv ${VENV_NAME} && \
 		${VENV_NAME}/bin/python3 -m pip install --upgrade pip && \
 		${VENV_NAME}/bin/python3 -m pip install -e '.[dev]'
 		${VENV_NAME}/bin/python3 -m pytest tests/
```

### Comparing `orquestra-core-0.8.0/PKG-INFO` & `orquestra-core-0.9.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orquestra-core
-Version: 0.8.0
+Version: 0.9.0
 Summary: "Orquestra Core meta-package"
 Home-page: https://github.com/zapatacomputing/orquestra-core
 Author: Zapata Computing Inc.
 Author-email: info@zapatacomputing.com,
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
@@ -13,14 +13,16 @@
 Description-Content-Type: text/markdown; charset=UTF-8
 Provides-Extra: dev
 Provides-Extra: qulacs
 Provides-Extra: qiskit
 Provides-Extra: cirq
 Provides-Extra: braket
 Provides-Extra: forest
+Provides-Extra: all
+Provides-Extra: orqviz
 License-File: LICENSE
 
 # orquestra-core
 
 ## What is it?
 
 Orquestra Core is a set of libraries used for quantum computing developed by [Zapata Computing](https://www.zapatacomputing.com). It's a part of [Orquestra](https://www.zapatacomputing.com/orquestra/) platform, but can be used as standalone Python libraries.
@@ -49,14 +51,16 @@
 - [`orquestra-qiskit`](https://github.com/zapatacomputing/orquestra-qiskit) – integration with [qiskit](https://qiskit.org/).
 - [`orquestra-cirq`](https://github.com/zapatacomputing/orquestra-cirq) – integration with [CirQ](https://quantumai.google/cirq).
 - [`orquestra-qulacs`](https://github.com/zapatacomputing/orquestra-qulacs) – integration with [Qulacs simulator](http://docs.qulacs.org/en/latest/).
 - [`orquestra-braket`](https://github.com/zapatacomputing/orquestra-braket) - integration with [Amazon Braket Python SDK](https://github.com/aws/amazon-braket-sdk-python)
 
 We have temporarily removed [`orquestra-forest`](https://github.com/zapatacomputing/orquestra-forest) (integration with [Forest SDK](https://docs.rigetti.com/qcs/)) due to compatibility issues. It should work in most cases, if you need it feel free to install it manually.
 
+- [`orqviz`](https://github.com/zapatacomputing/orqviz) – Visualization tool for VQA landscapes.
+
 ## Installation
 
 To install the latest versions of all of the Orquestra Core packages together run:
 
 `pip install orquestra-core`
 
 Libraries to interact with other frameworks (e.g. qiskit, cirq), simulators or QPU can be installed as optional dependencies, i.e.: `pip install orquestra[cirq]`.
```

### Comparing `orquestra-core-0.8.0/README.md` & `orquestra-core-0.9.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -28,14 +28,16 @@
 - [`orquestra-qiskit`](https://github.com/zapatacomputing/orquestra-qiskit) – integration with [qiskit](https://qiskit.org/).
 - [`orquestra-cirq`](https://github.com/zapatacomputing/orquestra-cirq) – integration with [CirQ](https://quantumai.google/cirq).
 - [`orquestra-qulacs`](https://github.com/zapatacomputing/orquestra-qulacs) – integration with [Qulacs simulator](http://docs.qulacs.org/en/latest/).
 - [`orquestra-braket`](https://github.com/zapatacomputing/orquestra-braket) - integration with [Amazon Braket Python SDK](https://github.com/aws/amazon-braket-sdk-python)
 
 We have temporarily removed [`orquestra-forest`](https://github.com/zapatacomputing/orquestra-forest) (integration with [Forest SDK](https://docs.rigetti.com/qcs/)) due to compatibility issues. It should work in most cases, if you need it feel free to install it manually.
 
+- [`orqviz`](https://github.com/zapatacomputing/orqviz) – Visualization tool for VQA landscapes.
+
 ## Installation
 
 To install the latest versions of all of the Orquestra Core packages together run:
 
 `pip install orquestra-core`
 
 Libraries to interact with other frameworks (e.g. qiskit, cirq), simulators or QPU can be installed as optional dependencies, i.e.: `pip install orquestra[cirq]`.
```

### Comparing `orquestra-core-0.8.0/docs/DOC_README.md` & `orquestra-core-0.9.0/docs/DOC_README.md`

 * *Files identical despite different names*

### Comparing `orquestra-core-0.8.0/docs/Makefile` & `orquestra-core-0.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `orquestra-core-0.8.0/docs/_static/ZapataCLA.pdf` & `orquestra-core-0.9.0/docs/_static/ZapataCLA.pdf`

 * *Files identical despite different names*

### Comparing `orquestra-core-0.8.0/docs/_static/favicon.ico` & `orquestra-core-0.9.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `orquestra-core-0.8.0/docs/_static/orquestra.png` & `orquestra-core-0.9.0/docs/_static/orquestra.png`

 * *Files identical despite different names*

### Comparing `orquestra-core-0.8.0/docs/conf.py` & `orquestra-core-0.9.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `orquestra-core-0.8.0/docs/examples/guides/circuit_runners_guide.py` & `orquestra-core-0.9.0/docs/quantum/examples/guides/circuit_runners_guide.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,17 +83,17 @@
 
 from orquestra.integrations.cirq.conversions._circuit_conversions import (
     export_to_cirq,
     import_from_cirq,
 )
 
 # Importing and Exporting with different frameworks
-from orquestra.integrations.forest.conversions import (
-    export_to_pyquil,
-    import_from_pyquil,
+from orquestra.integrations.cirq.conversions import (
+    export_to_cirq,
+    import_from_cirq,
 )
 from orquestra.integrations.qiskit.conversions import (
     export_to_qiskit,
     import_from_qiskit,
 )
 from orquestra.integrations.qulacs.conversions import convert_to_qulacs
```

### Comparing `orquestra-core-0.8.0/docs/examples/guides/circuits_guide.py` & `orquestra-core-0.9.0/docs/quantum/examples/guides/circuits_guide.py`

 * *Files identical despite different names*

### Comparing `orquestra-core-0.8.0/docs/examples/guides/estimators_guide.py` & `orquestra-core-0.9.0/docs/quantum/examples/guides/estimators_guide.py`

 * *Files identical despite different names*

### Comparing `orquestra-core-0.8.0/docs/examples/guides/interfaces_guide.py` & `orquestra-core-0.9.0/docs/quantum/examples/guides/interfaces_guide.py`

 * *Files identical despite different names*

### Comparing `orquestra-core-0.8.0/docs/examples/guides/mock_ansatz.py` & `orquestra-core-0.9.0/docs/quantum/examples/guides/mock_ansatz.py`

 * *Files identical despite different names*

### Comparing `orquestra-core-0.8.0/docs/examples/guides/optimizers.py` & `orquestra-core-0.9.0/docs/quantum/examples/guides/optimizers.py`

 * *Files identical despite different names*

### Comparing `orquestra-core-0.8.0/docs/examples/guides/vqa_guide.py` & `orquestra-core-0.9.0/docs/quantum/examples/guides/vqa_guide.py`

 * *Files identical despite different names*

### Comparing `orquestra-core-0.8.0/docs/examples/tutorials/bell_state.py` & `orquestra-core-0.9.0/docs/quantum/examples/tutorials/bell_state.py`

 * *Files 5% similar despite different names*

```diff
@@ -62,10 +62,10 @@
 bell_circuit_X = import_from_qiskit(qiskit_circuit)
 cirq_circuit = export_to_cirq(bell_circuit_X)
 print(cirq_circuit)
 
 wavefunction = sv_simulator.get_wavefunction(bell_circuit_X)
 ic(wavefunction.amplitudes)
 
-from orquestra.integrations.forest.conversions import export_to_pyquil
+from orquestra.integrations.qulacs.conversions import convert_to_qulacs
 
-pyquil_circuit = export_to_pyquil(bell_circuit_X)
+qulacs_circuit = convert_to_qulacs(bell_circuit_X)
```

### Comparing `orquestra-core-0.8.0/docs/examples/tutorials/qaoa_maxcut.py` & `orquestra-core-0.9.0/docs/quantum/examples/tutorials/qaoa_maxcut.py`

 * *Files identical despite different names*

### Comparing `orquestra-core-0.8.0/docs/examples/tutorials/superdense_coding.py` & `orquestra-core-0.9.0/docs/quantum/examples/tutorials/superdense_coding.py`

 * *Files identical despite different names*

### Comparing `orquestra-core-0.8.0/docs/guides/circuit_runners.rst` & `orquestra-core-0.9.0/docs/quantum/guides/circuit_runners.rst`

 * *Files identical despite different names*

### Comparing `orquestra-core-0.8.0/docs/guides/circuits.rst` & `orquestra-core-0.9.0/docs/quantum/guides/circuits.rst`

 * *Files identical despite different names*

### Comparing `orquestra-core-0.8.0/docs/guides/contributing.rst` & `orquestra-core-0.9.0/docs/quantum/guides/contributing.rst`

 * *Files identical despite different names*

### Comparing `orquestra-core-0.8.0/docs/guides/images/orquestra_core_connection.excalidraw.png` & `orquestra-core-0.9.0/docs/quantum/guides/images/orquestra_core_connection.excalidraw.png`

 * *Files identical despite different names*

### Comparing `orquestra-core-0.8.0/docs/guides/interfaces.rst` & `orquestra-core-0.9.0/docs/quantum/guides/interfaces.rst`

 * *Files identical despite different names*

### Comparing `orquestra-core-0.8.0/docs/guides/optimizers.rst` & `orquestra-core-0.9.0/docs/quantum/guides/optimizers.rst`

 * *Files identical despite different names*

### Comparing `orquestra-core-0.8.0/docs/guides/vqa_guide/ansatzes.rst` & `orquestra-core-0.9.0/docs/quantum/guides/vqa_guide/ansatzes.rst`

 * *Files identical despite different names*

### Comparing `orquestra-core-0.8.0/docs/guides/vqa_guide/estimators.rst` & `orquestra-core-0.9.0/docs/quantum/guides/vqa_guide/estimators.rst`

 * *Files identical despite different names*

### Comparing `orquestra-core-0.8.0/docs/guides/vqa_guide/introduction.rst` & `orquestra-core-0.9.0/docs/quantum/guides/vqa_guide/introduction.rst`

 * *Files identical despite different names*

### Comparing `orquestra-core-0.8.0/docs/guides/vqa_guide/structure.rst` & `orquestra-core-0.9.0/docs/quantum/guides/vqa_guide/structure.rst`

 * *Files identical despite different names*

### Comparing `orquestra-core-0.8.0/docs/make.bat` & `orquestra-core-0.9.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `orquestra-core-0.8.0/docs/repos/manifest.json` & `orquestra-core-0.9.0/docs/repos/manifest.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9722222222222222%*

 * *Differences: {"'repos'": "{'orqviz': OrderedDict([('url', 'https://github.com/zapatacomputing/orqviz.git'), "*

 * *            "('ref', 'main'), ('type', 'python'), ('autodoc', ['src/'])])}"}*

```diff
@@ -59,11 +59,19 @@
         "orquestra-vqa": {
             "autodoc": [
                 "src/"
             ],
             "ref": "main",
             "type": "python",
             "url": "https://github.com/zapatacomputing/orquestra-vqa.git"
+        },
+        "orqviz": {
+            "autodoc": [
+                "src/"
+            ],
+            "ref": "main",
+            "type": "python",
+            "url": "https://github.com/zapatacomputing/orqviz.git"
         }
     },
     "version": "1.1.0"
 }
```

### Comparing `orquestra-core-0.8.0/docs/tutorials/basic_qaoa.rst` & `orquestra-core-0.9.0/docs/quantum/tutorials/basic_qaoa.rst`

 * *Files identical despite different names*

### Comparing `orquestra-core-0.8.0/docs/tutorials/beginner_tutorial.rst` & `orquestra-core-0.9.0/docs/quantum/tutorials/beginner_tutorial.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,12 @@
-===============
-Getting Started
-===============
-
-
-Installing orquestra-core
-=========================
-
-Orquestra Core can be installed by running ``pip install orquestra-core``.
-
-The ``orquestra-core`` metapackage bundles together :doc:`several packages <orq_core_structure>`, including the ``orquestra-quantum``, ``orquestra-qiskit``, and ``orquestra-cirq`` packages used in this tutorial.
-
-Note that Orquestra Core can also be installed from source from the `orquestra-core GitHub repository <https://github.com/zapatacomputing/orquestra-core>`_.
+================
+Quantum Circuits
+================
 
+This tutorial explains how to use the Orquestra Quantum SDK to define and run quantum circuits, as well as translate between frameworks such as Qiskit and Cirq. 
 
 .. _creating_basic_circuits:
 
 Creating basic circuits
 =======================
 
 Let's say you want to build a quantum circuit just to build a Bell State and measure it. As a quick reminder, a Bell State is a maximally entangled state with the most well-known form:
@@ -180,18 +171,18 @@
         :start-at: wavefunction = sv_simulator.get_wavefunction(bell_circuit_X)
         :end-at: ic(wavefunction.amplitudes)
 
 And we should get ``wavefunction.amplitudes: array([0.70710678+0.j, 0.+0.j, 0.+0.j, 0.70710678+0.j])`` if everything went according to plan.
 
 **Your turn!**
 
-Try to export our new ``bell_circuit_X`` to pyQuil!
+Try to export our new ``bell_circuit_X`` to Qulacs!
 
 .. hint::
     :class: dropdown
 
     .. literalinclude:: ../examples/tutorials/bell_state.py
         :language: python
-        :start-at: import export_to_pyquil
-        :end-at: pyquil_circuit = 
+        :start-at: import export_to_qulacs
+        :end-at: qulacs_circuit = 
 
 Ready for something a bit more interesting? Try the :ref:`qaoa tutorial <qaoa>`!
```

### Comparing `orquestra-core-0.8.0/docs/tutorials/images/cut_graph.excalidraw.png` & `orquestra-core-0.9.0/docs/quantum/tutorials/images/cut_graph.excalidraw.png`

 * *Files identical despite different names*

### Comparing `orquestra-core-0.8.0/docs/tutorials/images/harder_graph.excalidraw.png` & `orquestra-core-0.9.0/docs/quantum/tutorials/images/harder_graph.excalidraw.png`

 * *Files identical despite different names*

### Comparing `orquestra-core-0.8.0/docs/tutorials/images/harder_graph_cut.excalidraw.png` & `orquestra-core-0.9.0/docs/quantum/tutorials/images/harder_graph_cut.excalidraw.png`

 * *Files identical despite different names*

### Comparing `orquestra-core-0.8.0/docs/tutorials/images/uncut_graph.excalidraw.png` & `orquestra-core-0.9.0/docs/quantum/tutorials/images/uncut_graph.excalidraw.png`

 * *Files identical despite different names*

### Comparing `orquestra-core-0.8.0/pyproject.toml` & `orquestra-core-0.9.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -23,15 +23,18 @@
 [[tool.mypy.overrides]]
 module = [
     'scipy.*',
     'sympy.*',
     'rapidjson',
     'networkx.*',
     'openfermion.*',
-    'qiskit.*'
+    'qiskit.*',
+    'matplotlib.*',
+    'sklearn.*',
+    'mpl_toolkits.*',
 ]
 ignore_missing_imports = true
 
 [tool.coverage.run]
 omit = ["*/__init__.py"]
 
 [tool.coverage.report]
```

### Comparing `orquestra-core-0.8.0/src/orquestra_core.egg-info/PKG-INFO` & `orquestra-core-0.9.0/src/orquestra_core.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orquestra-core
-Version: 0.8.0
+Version: 0.9.0
 Summary: "Orquestra Core meta-package"
 Home-page: https://github.com/zapatacomputing/orquestra-core
 Author: Zapata Computing Inc.
 Author-email: info@zapatacomputing.com,
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
@@ -13,14 +13,16 @@
 Description-Content-Type: text/markdown; charset=UTF-8
 Provides-Extra: dev
 Provides-Extra: qulacs
 Provides-Extra: qiskit
 Provides-Extra: cirq
 Provides-Extra: braket
 Provides-Extra: forest
+Provides-Extra: all
+Provides-Extra: orqviz
 License-File: LICENSE
 
 # orquestra-core
 
 ## What is it?
 
 Orquestra Core is a set of libraries used for quantum computing developed by [Zapata Computing](https://www.zapatacomputing.com). It's a part of [Orquestra](https://www.zapatacomputing.com/orquestra/) platform, but can be used as standalone Python libraries.
@@ -49,14 +51,16 @@
 - [`orquestra-qiskit`](https://github.com/zapatacomputing/orquestra-qiskit) – integration with [qiskit](https://qiskit.org/).
 - [`orquestra-cirq`](https://github.com/zapatacomputing/orquestra-cirq) – integration with [CirQ](https://quantumai.google/cirq).
 - [`orquestra-qulacs`](https://github.com/zapatacomputing/orquestra-qulacs) – integration with [Qulacs simulator](http://docs.qulacs.org/en/latest/).
 - [`orquestra-braket`](https://github.com/zapatacomputing/orquestra-braket) - integration with [Amazon Braket Python SDK](https://github.com/aws/amazon-braket-sdk-python)
 
 We have temporarily removed [`orquestra-forest`](https://github.com/zapatacomputing/orquestra-forest) (integration with [Forest SDK](https://docs.rigetti.com/qcs/)) due to compatibility issues. It should work in most cases, if you need it feel free to install it manually.
 
+- [`orqviz`](https://github.com/zapatacomputing/orqviz) – Visualization tool for VQA landscapes.
+
 ## Installation
 
 To install the latest versions of all of the Orquestra Core packages together run:
 
 `pip install orquestra-core`
 
 Libraries to interact with other frameworks (e.g. qiskit, cirq), simulators or QPU can be installed as optional dependencies, i.e.: `pip install orquestra[cirq]`.
```

### Comparing `orquestra-core-0.8.0/subtrees/z_quantum_actions/Makefile` & `orquestra-core-0.9.0/subtrees/z_quantum_actions/Makefile`

 * *Files identical despite different names*

### Comparing `orquestra-core-0.8.0/subtrees/z_quantum_actions/README.rst` & `orquestra-core-0.9.0/subtrees/z_quantum_actions/README.rst`

 * *Files identical despite different names*

### Comparing `orquestra-core-0.8.0/subtrees/z_quantum_actions/actions/coverage/action.yml` & `orquestra-core-0.9.0/subtrees/z_quantum_actions/actions/coverage/action.yml`

 * *Files identical despite different names*

### Comparing `orquestra-core-0.8.0/subtrees/z_quantum_actions/actions/publish-release/action.yml` & `orquestra-core-0.9.0/subtrees/z_quantum_actions/actions/publish-release/action.yml`

 * *Files identical despite different names*

### Comparing `orquestra-core-0.8.0/subtrees/z_quantum_actions/bin/get_next_version.py` & `orquestra-core-0.9.0/subtrees/z_quantum_actions/bin/get_next_version.py`

 * *Files identical despite different names*

### Comparing `orquestra-core-0.8.0/subtrees/z_quantum_actions/pyproject.toml` & `orquestra-core-0.9.0/subtrees/z_quantum_actions/pyproject.toml`

 * *Files identical despite different names*

### Comparing `orquestra-core-0.8.0/subtrees/z_quantum_actions/sample_setup.py` & `orquestra-core-0.9.0/subtrees/z_quantum_actions/sample_setup.py`

 * *Files identical despite different names*

### Comparing `orquestra-core-0.8.0/subtrees/z_quantum_actions/setup_extras.py` & `orquestra-core-0.9.0/subtrees/z_quantum_actions/setup_extras.py`

 * *Files identical despite different names*

### Comparing `orquestra-core-0.8.0/subtrees/z_quantum_actions/tests/test_get_next_version.py` & `orquestra-core-0.9.0/subtrees/z_quantum_actions/tests/test_get_next_version.py`

 * *Files identical despite different names*

### Comparing `orquestra-core-0.8.0/subtrees/z_quantum_actions/workflow-templates/coverage.yml` & `orquestra-core-0.9.0/subtrees/z_quantum_actions/workflow-templates/coverage.yml`

 * *Files identical despite different names*

### Comparing `orquestra-core-0.8.0/subtrees/z_quantum_actions/workflow-templates/publish-release.yml` & `orquestra-core-0.9.0/subtrees/z_quantum_actions/workflow-templates/publish-release.yml`

 * *Files identical despite different names*

### Comparing `orquestra-core-0.8.0/subtrees/z_quantum_actions/workflow-templates/style.yml` & `orquestra-core-0.9.0/subtrees/z_quantum_actions/workflow-templates/style.yml`

 * *Files identical despite different names*

### Comparing `orquestra-core-0.8.0/tests/fh_vqe_test.py` & `orquestra-core-0.9.0/tests/fh_vqe_test.py`

 * *Files identical despite different names*

### Comparing `orquestra-core-0.8.0/tests/qaoa_maxcut_test.py` & `orquestra-core-0.9.0/tests/qaoa_maxcut_test.py`

 * *Files identical despite different names*

### Comparing `orquestra-core-0.8.0/tests/qcbm_test.py` & `orquestra-core-0.9.0/tests/qcbm_test.py`

 * *Files identical despite different names*

