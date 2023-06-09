# Comparing `tmp/fluidsimfoam-0.0.5.tar.gz` & `tmp/fluidsimfoam-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fluidsimfoam-0.0.5.tar", max compression
+gzip compressed data, was "fluidsimfoam-0.0.6.tar", max compression
```

## Comparing `fluidsimfoam-0.0.5.tar` & `fluidsimfoam-0.0.6.tar`

### file list

```diff
@@ -1,94 +1,76 @@
--rw-r--r--   0        0        0     1521 2023-02-27 10:14:44.107434 fluidsimfoam-0.0.5/LICENSE
--rw-r--r--   0        0        0     7375 2023-06-05 07:50:58.783012 fluidsimfoam-0.0.5/README.md
--rw-r--r--   0        0        0     2307 2023-06-05 07:50:58.791012 fluidsimfoam-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     2059 2023-06-01 13:07:51.325421 fluidsimfoam-0.0.5/src/fluidsimfoam/__init__.py
--rw-r--r--   0        0        0     3164 2023-06-05 07:50:58.795012 fluidsimfoam-0.0.5/src/fluidsimfoam/foam_input_files/__init__.py
--rw-r--r--   0        0        0     2581 2023-05-10 08:25:28.979644 fluidsimfoam-0.0.5/src/fluidsimfoam/foam_input_files/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     3517 2023-06-01 13:39:28.446879 fluidsimfoam-0.0.5/src/fluidsimfoam/foam_input_files/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0    16638 2023-05-11 13:39:09.365344 fluidsimfoam-0.0.5/src/fluidsimfoam/foam_input_files/__pycache__/ast.cpython-310.pyc
--rw-r--r--   0        0        0    16882 2023-06-01 13:39:28.450879 fluidsimfoam-0.0.5/src/fluidsimfoam/foam_input_files/__pycache__/ast.cpython-39.pyc
--rw-r--r--   0        0        0     2351 2023-05-11 11:01:22.162680 fluidsimfoam-0.0.5/src/fluidsimfoam/foam_input_files/__pycache__/constant_files.cpython-310.pyc
--rw-r--r--   0        0        0     1949 2023-06-01 13:39:28.634883 fluidsimfoam-0.0.5/src/fluidsimfoam/foam_input_files/__pycache__/constant_files.cpython-39.pyc
--rw-r--r--   0        0        0     3462 2023-06-01 13:39:28.638882 fluidsimfoam-0.0.5/src/fluidsimfoam/foam_input_files/__pycache__/control_dict.cpython-39.pyc
--rw-r--r--   0        0        0     2212 2023-05-23 10:21:24.950902 fluidsimfoam-0.0.5/src/fluidsimfoam/foam_input_files/__pycache__/decompose_par.cpython-39.pyc
--rw-r--r--   0        0        0     6200 2023-05-11 13:45:09.791386 fluidsimfoam-0.0.5/src/fluidsimfoam/foam_input_files/__pycache__/fields.cpython-310.pyc
--rw-r--r--   0        0        0     7157 2023-06-01 13:39:28.642883 fluidsimfoam-0.0.5/src/fluidsimfoam/foam_input_files/__pycache__/fields.cpython-39.pyc
--rw-r--r--   0        0        0     4954 2023-05-22 08:22:48.134465 fluidsimfoam-0.0.5/src/fluidsimfoam/foam_input_files/__pycache__/fv_options.cpython-39.pyc
--rw-r--r--   0        0        0     2761 2023-05-10 08:25:29.207648 fluidsimfoam-0.0.5/src/fluidsimfoam/foam_input_files/__pycache__/fv_schemes.cpython-310.pyc
--rw-r--r--   0        0        0     2426 2023-06-01 13:39:28.642883 fluidsimfoam-0.0.5/src/fluidsimfoam/foam_input_files/__pycache__/fv_schemes.cpython-39.pyc
--rw-r--r--   0        0        0     5365 2023-05-10 08:25:29.355651 fluidsimfoam-0.0.5/src/fluidsimfoam/foam_input_files/__pycache__/generators.cpython-310.pyc
--rw-r--r--   0        0        0     5389 2023-05-23 10:21:25.798917 fluidsimfoam-0.0.5/src/fluidsimfoam/foam_input_files/__pycache__/generators.cpython-39.pyc
--rw-r--r--   0        0        0    10482 2023-05-10 08:25:28.991645 fluidsimfoam-0.0.5/src/fluidsimfoam/foam_input_files/__pycache__/parser.cpython-310.pyc
--rw-r--r--   0        0        0    10664 2023-05-11 15:19:26.288038 fluidsimfoam-0.0.5/src/fluidsimfoam/foam_input_files/__pycache__/parser.cpython-39.pyc
--rw-r--r--   0        0        0     1091 2023-05-04 07:22:21.758230 fluidsimfoam-0.0.5/src/fluidsimfoam/foam_input_files/__pycache__/polymesh.cpython-310.pyc
--rw-r--r--   0        0        0     1083 2023-05-11 15:19:27.040051 fluidsimfoam-0.0.5/src/fluidsimfoam/foam_input_files/__pycache__/polymesh.cpython-39.pyc
--rw-r--r--   0        0        0      896 2023-06-01 13:39:28.638882 fluidsimfoam-0.0.5/src/fluidsimfoam/foam_input_files/__pycache__/util.cpython-39.pyc
--rw-r--r--   0        0        0    16765 2023-06-05 07:50:58.795012 fluidsimfoam-0.0.5/src/fluidsimfoam/foam_input_files/ast.py
--rw-r--r--   0        0        0     1080 2023-05-05 08:40:03.756342 fluidsimfoam-0.0.5/src/fluidsimfoam/foam_input_files/blockmesh/LICENSE
--rw-r--r--   0        0        0    15028 2023-06-05 07:50:58.795012 fluidsimfoam-0.0.5/src/fluidsimfoam/foam_input_files/blockmesh/__init__.py
--rw-r--r--   0        0        0    15409 2023-05-10 08:25:29.203648 fluidsimfoam-0.0.5/src/fluidsimfoam/foam_input_files/blockmesh/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0    15609 2023-06-01 15:02:51.930901 fluidsimfoam-0.0.5/src/fluidsimfoam/foam_input_files/blockmesh/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     2353 2023-05-05 08:41:29.209815 fluidsimfoam-0.0.5/src/fluidsimfoam/foam_input_files/blockmesh/__pycache__/edges.cpython-310.pyc
--rw-r--r--   0        0        0     2419 2023-05-11 15:19:26.868048 fluidsimfoam-0.0.5/src/fluidsimfoam/foam_input_files/blockmesh/__pycache__/edges.cpython-39.pyc
--rw-r--r--   0        0        0     3094 2023-05-05 08:41:29.209815 fluidsimfoam-0.0.5/src/fluidsimfoam/foam_input_files/blockmesh/__pycache__/grading.cpython-310.pyc
--rw-r--r--   0        0        0     3148 2023-05-11 15:19:26.872048 fluidsimfoam-0.0.5/src/fluidsimfoam/foam_input_files/blockmesh/__pycache__/grading.cpython-39.pyc
--rw-r--r--   0        0        0     1810 2023-05-05 08:40:03.756342 fluidsimfoam-0.0.5/src/fluidsimfoam/foam_input_files/blockmesh/edges.py
--rw-r--r--   0        0        0     3426 2023-05-05 08:40:03.756342 fluidsimfoam-0.0.5/src/fluidsimfoam/foam_input_files/blockmesh/grading.py
--rw-r--r--   0        0        0     2058 2023-06-01 13:07:51.329422 fluidsimfoam-0.0.5/src/fluidsimfoam/foam_input_files/constant_files.py
--rw-r--r--   0        0        0     2822 2023-06-01 13:07:51.329422 fluidsimfoam-0.0.5/src/fluidsimfoam/foam_input_files/control_dict.py
--rw-r--r--   0        0        0     2540 2023-05-23 10:20:23.357858 fluidsimfoam-0.0.5/src/fluidsimfoam/foam_input_files/decompose_par.py
--rw-r--r--   0        0        0     6673 2023-06-01 13:07:51.329422 fluidsimfoam-0.0.5/src/fluidsimfoam/foam_input_files/fields.py
--rw-r--r--   0        0        0     1345 2023-06-05 07:50:58.795012 fluidsimfoam-0.0.5/src/fluidsimfoam/foam_input_files/format.py
--rw-r--r--   0        0        0     6107 2023-05-22 08:22:36.874278 fluidsimfoam-0.0.5/src/fluidsimfoam/foam_input_files/fv_options.py
--rw-r--r--   0        0        0     1987 2023-06-01 13:07:51.329422 fluidsimfoam-0.0.5/src/fluidsimfoam/foam_input_files/fv_schemes.py
--rw-r--r--   0        0        0     5250 2023-05-23 10:20:23.357858 fluidsimfoam-0.0.5/src/fluidsimfoam/foam_input_files/generators.py
--rw-r--r--   0        0        0     1916 2023-05-15 15:12:04.403422 fluidsimfoam-0.0.5/src/fluidsimfoam/foam_input_files/grammar.lark
--rw-r--r--   0        0        0     2337 2023-05-15 15:09:00.692349 fluidsimfoam-0.0.5/src/fluidsimfoam/foam_input_files/grammar_advanced.lark
--rw-r--r--   0        0        0     9522 2023-05-10 08:15:22.273340 fluidsimfoam-0.0.5/src/fluidsimfoam/foam_input_files/parser.py
--rw-r--r--   0        0        0      973 2023-05-03 13:57:31.639504 fluidsimfoam-0.0.5/src/fluidsimfoam/foam_input_files/polymesh.py
--rw-r--r--   0        0        0      766 2023-06-01 13:07:51.333422 fluidsimfoam-0.0.5/src/fluidsimfoam/foam_input_files/util.py
--rw-r--r--   0        0        0     1400 2023-05-10 08:15:22.273340 fluidsimfoam-0.0.5/src/fluidsimfoam/info.py
--rw-r--r--   0        0        0      124 2023-05-10 08:15:22.273340 fluidsimfoam-0.0.5/src/fluidsimfoam/init_fields.py
--rw-r--r--   0        0        0      747 2023-05-10 08:15:22.273340 fluidsimfoam-0.0.5/src/fluidsimfoam/log.py
--rw-r--r--   0        0        0      608 2023-05-11 08:16:54.779023 fluidsimfoam-0.0.5/src/fluidsimfoam/make.py
--rw-r--r--   0        0        0     1210 2023-05-22 10:55:42.519938 fluidsimfoam-0.0.5/src/fluidsimfoam/operators.py
--rw-r--r--   0        0        0      423 2023-06-01 13:07:51.333422 fluidsimfoam-0.0.5/src/fluidsimfoam/output/__init__.py
--rw-r--r--   0        0        0      323 2023-05-10 08:25:29.347651 fluidsimfoam-0.0.5/src/fluidsimfoam/output/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      551 2023-06-01 14:10:06.823343 fluidsimfoam-0.0.5/src/fluidsimfoam/output/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     7791 2023-05-11 13:57:19.091606 fluidsimfoam-0.0.5/src/fluidsimfoam/output/__pycache__/base.cpython-310.pyc
--rw-r--r--   0        0        0     7625 2023-06-01 14:10:06.823343 fluidsimfoam-0.0.5/src/fluidsimfoam/output/__pycache__/base.cpython-39.pyc
--rw-r--r--   0        0        0     1534 2023-06-01 14:10:06.847343 fluidsimfoam-0.0.5/src/fluidsimfoam/output/__pycache__/dataframe_from_paths.cpython-39.pyc
--rw-r--r--   0        0        0     1018 2023-05-11 13:57:19.479612 fluidsimfoam-0.0.5/src/fluidsimfoam/output/__pycache__/fields.cpython-310.pyc
--rw-r--r--   0        0        0     3516 2023-06-01 14:10:07.435354 fluidsimfoam-0.0.5/src/fluidsimfoam/output/__pycache__/fields.cpython-39.pyc
--rw-r--r--   0        0        0     2773 2023-05-11 07:59:46.541407 fluidsimfoam-0.0.5/src/fluidsimfoam/output/__pycache__/log.cpython-310.pyc
--rw-r--r--   0        0        0     5460 2023-06-01 14:10:07.071347 fluidsimfoam-0.0.5/src/fluidsimfoam/output/__pycache__/log.cpython-39.pyc
--rw-r--r--   0        0        0    10233 2023-06-05 07:50:58.795012 fluidsimfoam-0.0.5/src/fluidsimfoam/output/base.py
--rw-r--r--   0        0        0     1080 2023-06-01 13:07:51.333422 fluidsimfoam-0.0.5/src/fluidsimfoam/output/dataframe_from_paths.py
--rw-r--r--   0        0        0     3046 2023-06-01 13:07:51.333422 fluidsimfoam-0.0.5/src/fluidsimfoam/output/fields.py
--rw-r--r--   0        0        0     6580 2023-06-01 13:07:51.333422 fluidsimfoam-0.0.5/src/fluidsimfoam/output/log.py
--rw-r--r--   0        0        0     2886 2023-05-22 11:57:10.378120 fluidsimfoam-0.0.5/src/fluidsimfoam/params.py
--rw-r--r--   0        0        0     1516 2023-06-01 13:07:51.333422 fluidsimfoam-0.0.5/src/fluidsimfoam/resources/LICENSE.template
--rw-r--r--   0        0        0      235 2023-06-01 13:07:51.337422 fluidsimfoam-0.0.5/src/fluidsimfoam/resources/README.md.template
--rw-r--r--   0        0        0      573 2023-05-10 08:15:22.277340 fluidsimfoam-0.0.5/src/fluidsimfoam/resources/__init__.py
--rw-r--r--   0        0        0      535 2023-06-01 13:07:51.337422 fluidsimfoam-0.0.5/src/fluidsimfoam/resources/__init__.py.template
--rw-r--r--   0        0        0      964 2023-05-10 08:25:29.363651 fluidsimfoam-0.0.5/src/fluidsimfoam/resources/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      960 2023-05-16 08:00:14.420535 fluidsimfoam-0.0.5/src/fluidsimfoam/resources/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0      516 2023-06-05 07:50:58.799013 fluidsimfoam-0.0.5/src/fluidsimfoam/resources/output.py.template
--rw-r--r--   0        0        0      507 2023-06-01 13:07:51.337422 fluidsimfoam-0.0.5/src/fluidsimfoam/resources/pyproject.toml.template
--rw-r--r--   0        0        0       42 2023-06-01 13:07:51.337422 fluidsimfoam-0.0.5/src/fluidsimfoam/resources/tasks.py.template
--rw-r--r--   0        0        0      726 2023-06-05 07:50:58.799013 fluidsimfoam-0.0.5/src/fluidsimfoam/resources/test_generated_solver.py.template
--rw-r--r--   0        0        0     2765 2023-05-10 08:15:22.277340 fluidsimfoam-0.0.5/src/fluidsimfoam/solvers/__init__.py
--rw-r--r--   0        0        0     2629 2023-05-10 08:25:29.355651 fluidsimfoam-0.0.5/src/fluidsimfoam/solvers/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2626 2023-05-11 15:19:26.904049 fluidsimfoam-0.0.5/src/fluidsimfoam/solvers/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     2757 2023-05-11 08:22:40.884944 fluidsimfoam-0.0.5/src/fluidsimfoam/solvers/__pycache__/base.cpython-310.pyc
--rw-r--r--   0        0        0     2725 2023-06-01 14:10:06.639340 fluidsimfoam-0.0.5/src/fluidsimfoam/solvers/__pycache__/base.cpython-39.pyc
--rw-r--r--   0        0        0     2915 2023-06-01 13:07:51.341422 fluidsimfoam-0.0.5/src/fluidsimfoam/solvers/base.py
--rw-r--r--   0        0        0     3298 2023-06-05 07:50:58.799013 fluidsimfoam-0.0.5/src/fluidsimfoam/tasks.py
--rw-r--r--   0        0        0     1610 2023-06-01 13:07:51.341422 fluidsimfoam-0.0.5/src/fluidsimfoam/testing.py
--rw-r--r--   0        0        0       77 2023-05-10 08:15:22.281340 fluidsimfoam-0.0.5/src/fluidsimfoam/util/__init__.py
--rw-r--r--   0        0        0      247 2023-05-10 08:25:29.427652 fluidsimfoam-0.0.5/src/fluidsimfoam/util/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      245 2023-05-11 15:19:26.944050 fluidsimfoam-0.0.5/src/fluidsimfoam/util/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     1154 2023-03-09 14:33:14.296195 fluidsimfoam-0.0.5/src/fluidsimfoam/util/__pycache__/console.cpython-310.pyc
--rw-r--r--   0        0        0     5233 2023-06-01 15:08:54.809264 fluidsimfoam-0.0.5/src/fluidsimfoam/util/__pycache__/console.cpython-39.pyc
--rw-r--r--   0        0        0     6906 2023-06-05 07:50:58.799013 fluidsimfoam-0.0.5/src/fluidsimfoam/util/console.py
--rw-r--r--   0        0        0     8672 1970-01-01 00:00:00.000000 fluidsimfoam-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1521 2023-03-02 21:01:46.291446 fluidsimfoam-0.0.6/LICENSE
+-rw-r--r--   0        0        0     7375 2023-06-04 19:44:44.715013 fluidsimfoam-0.0.6/README.md
+-rw-r--r--   0        0        0     2342 2023-06-09 19:17:24.747107 fluidsimfoam-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     2059 2023-05-25 19:17:46.752187 fluidsimfoam-0.0.6/src/fluidsimfoam/__init__.py
+-rw-r--r--   0        0        0     3164 2023-06-02 09:21:38.899122 fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/__init__.py
+-rw-r--r--   0        0        0     3428 2023-06-02 09:23:55.178145 fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0    16781 2023-06-02 07:08:26.447668 fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/__pycache__/ast.cpython-310.pyc
+-rw-r--r--   0        0        0     1980 2023-05-25 19:19:08.676600 fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/__pycache__/constant_files.cpython-310.pyc
+-rw-r--r--   0        0        0     3457 2023-06-01 08:42:32.898140 fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/__pycache__/control_dict.cpython-310.pyc
+-rw-r--r--   0        0        0     2743 2023-06-07 09:45:32.720354 fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/__pycache__/decompose_par.cpython-310.pyc
+-rw-r--r--   0        0        0     7155 2023-05-30 20:33:58.056468 fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/__pycache__/fields.cpython-310.pyc
+-rw-r--r--   0        0        0     1450 2023-06-02 09:25:06.533632 fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/__pycache__/format.cpython-310.pyc
+-rw-r--r--   0        0        0     5005 2023-05-22 18:59:45.385794 fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/__pycache__/fv_options.cpython-310.pyc
+-rw-r--r--   0        0        0     2441 2023-05-24 19:26:28.851965 fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/__pycache__/fv_schemes.cpython-310.pyc
+-rw-r--r--   0        0        0     1844 2023-05-05 07:20:02.628943 fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/__pycache__/fv_schemes_helper.cpython-310.pyc
+-rw-r--r--   0        0        0     5418 2023-05-23 07:52:07.543018 fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/__pycache__/generators.cpython-310.pyc
+-rw-r--r--   0        0        0    10473 2023-05-09 12:43:04.027476 fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/__pycache__/parser.cpython-310.pyc
+-rw-r--r--   0        0        0     1082 2023-05-03 21:01:43.908143 fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/__pycache__/polymesh.cpython-310.pyc
+-rw-r--r--   0        0        0      889 2023-05-24 19:26:28.847965 fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/__pycache__/util.cpython-310.pyc
+-rw-r--r--   0        0        0    16765 2023-06-02 07:07:00.868495 fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/ast.py
+-rw-r--r--   0        0        0     1080 2023-04-23 15:48:42.099657 fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/blockmesh/LICENSE
+-rw-r--r--   0        0        0    16070 2023-06-05 19:44:44.570045 fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/blockmesh/__init__.py
+-rw-r--r--   0        0        0    17560 2023-06-05 19:44:47.242342 fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/blockmesh/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2999 2023-06-05 19:24:15.763776 fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/blockmesh/__pycache__/edges.cpython-310.pyc
+-rw-r--r--   0        0        0     3085 2023-05-05 07:26:24.622314 fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/blockmesh/__pycache__/grading.cpython-310.pyc
+-rw-r--r--   0        0        0     2124 2023-06-05 19:23:23.082283 fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/blockmesh/edges.py
+-rw-r--r--   0        0        0     3426 2023-04-24 20:58:16.942659 fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/blockmesh/grading.py
+-rw-r--r--   0        0        0     2058 2023-05-25 19:17:46.752187 fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/constant_files.py
+-rw-r--r--   0        0        0     2822 2023-05-31 20:11:47.954320 fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/control_dict.py
+-rw-r--r--   0        0        0     3238 2023-06-07 07:30:57.181605 fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/decompose_par.py
+-rw-r--r--   0        0        0     6673 2023-05-30 19:50:15.784136 fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/fields.py
+-rw-r--r--   0        0        0     1345 2023-06-02 09:25:03.501654 fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/format.py
+-rw-r--r--   0        0        0     6107 2023-05-22 18:56:58.335368 fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/fv_options.py
+-rw-r--r--   0        0        0     1987 2023-05-24 19:23:08.313065 fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/fv_schemes.py
+-rw-r--r--   0        0        0     5250 2023-05-23 07:52:05.747013 fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/generators.py
+-rw-r--r--   0        0        0     1916 2023-05-16 18:45:49.936442 fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/grammar.lark
+-rw-r--r--   0        0        0     2337 2023-05-16 18:45:49.940441 fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/grammar_advanced.lark
+-rw-r--r--   0        0        0     9522 2023-05-09 12:42:41.039310 fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/parser.py
+-rw-r--r--   0        0        0      973 2023-05-03 19:26:40.332634 fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/polymesh.py
+-rw-r--r--   0        0        0      766 2023-05-24 19:24:59.484896 fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/util.py
+-rw-r--r--   0        0        0     1400 2023-05-09 20:05:14.235128 fluidsimfoam-0.0.6/src/fluidsimfoam/info.py
+-rw-r--r--   0        0        0      124 2023-05-09 13:01:28.476575 fluidsimfoam-0.0.6/src/fluidsimfoam/init_fields.py
+-rw-r--r--   0        0        0      747 2023-05-09 13:00:38.420124 fluidsimfoam-0.0.6/src/fluidsimfoam/log.py
+-rw-r--r--   0        0        0      608 2023-05-11 19:44:39.696948 fluidsimfoam-0.0.6/src/fluidsimfoam/make.py
+-rw-r--r--   0        0        0     1210 2023-05-22 18:56:58.335368 fluidsimfoam-0.0.6/src/fluidsimfoam/operators.py
+-rw-r--r--   0        0        0      423 2023-05-25 19:38:04.703998 fluidsimfoam-0.0.6/src/fluidsimfoam/output/__init__.py
+-rw-r--r--   0        0        0      544 2023-05-25 19:41:05.807251 fluidsimfoam-0.0.6/src/fluidsimfoam/output/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     7746 2023-06-04 20:15:04.168667 fluidsimfoam-0.0.6/src/fluidsimfoam/output/__pycache__/base.cpython-310.pyc
+-rw-r--r--   0        0        0     1539 2023-05-25 19:19:08.700611 fluidsimfoam-0.0.6/src/fluidsimfoam/output/__pycache__/dataframe_from_paths.cpython-310.pyc
+-rw-r--r--   0        0        0     3514 2023-06-07 09:45:34.666101 fluidsimfoam-0.0.6/src/fluidsimfoam/output/__pycache__/fields.cpython-310.pyc
+-rw-r--r--   0        0        0     5445 2023-05-25 19:19:08.944725 fluidsimfoam-0.0.6/src/fluidsimfoam/output/__pycache__/log.cpython-310.pyc
+-rw-r--r--   0        0        0    10233 2023-06-04 20:13:56.099256 fluidsimfoam-0.0.6/src/fluidsimfoam/output/base.py
+-rw-r--r--   0        0        0     1080 2023-05-25 19:17:46.756188 fluidsimfoam-0.0.6/src/fluidsimfoam/output/dataframe_from_paths.py
+-rw-r--r--   0        0        0     2998 2023-06-07 07:30:21.271923 fluidsimfoam-0.0.6/src/fluidsimfoam/output/fields.py
+-rw-r--r--   0        0        0     6580 2023-05-25 19:17:46.756188 fluidsimfoam-0.0.6/src/fluidsimfoam/output/log.py
+-rw-r--r--   0        0        0     2886 2023-05-22 18:56:58.339368 fluidsimfoam-0.0.6/src/fluidsimfoam/params.py
+-rw-r--r--   0        0        0     1516 2023-05-30 19:50:11.700069 fluidsimfoam-0.0.6/src/fluidsimfoam/resources/LICENSE.template
+-rw-r--r--   0        0        0      235 2023-05-30 19:50:11.700069 fluidsimfoam-0.0.6/src/fluidsimfoam/resources/README.md.template
+-rw-r--r--   0        0        0      573 2023-05-09 13:02:35.270502 fluidsimfoam-0.0.6/src/fluidsimfoam/resources/__init__.py
+-rw-r--r--   0        0        0      535 2023-05-30 19:50:11.700069 fluidsimfoam-0.0.6/src/fluidsimfoam/resources/__init__.py.template
+-rw-r--r--   0        0        0      955 2023-05-09 13:02:39.537858 fluidsimfoam-0.0.6/src/fluidsimfoam/resources/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      516 2023-06-01 20:14:27.398486 fluidsimfoam-0.0.6/src/fluidsimfoam/resources/output.py.template
+-rw-r--r--   0        0        0      507 2023-06-01 09:02:52.471699 fluidsimfoam-0.0.6/src/fluidsimfoam/resources/pyproject.toml.template
+-rw-r--r--   0        0        0       42 2023-05-30 19:50:11.700069 fluidsimfoam-0.0.6/src/fluidsimfoam/resources/tasks.py.template
+-rw-r--r--   0        0        0      726 2023-06-02 09:41:43.285771 fluidsimfoam-0.0.6/src/fluidsimfoam/resources/test_generated_solver.py.template
+-rw-r--r--   0        0        0     2765 2023-05-09 13:04:52.906067 fluidsimfoam-0.0.6/src/fluidsimfoam/solvers/__init__.py
+-rw-r--r--   0        0        0     2620 2023-05-09 13:05:27.378825 fluidsimfoam-0.0.6/src/fluidsimfoam/solvers/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2748 2023-05-24 19:26:28.699960 fluidsimfoam-0.0.6/src/fluidsimfoam/solvers/__pycache__/base.cpython-310.pyc
+-rw-r--r--   0        0        0     2915 2023-05-24 19:14:04.619885 fluidsimfoam-0.0.6/src/fluidsimfoam/solvers/base.py
+-rw-r--r--   0        0        0     3298 2023-06-02 08:33:23.157994 fluidsimfoam-0.0.6/src/fluidsimfoam/tasks.py
+-rw-r--r--   0        0        0     1716 2023-06-05 19:47:19.026905 fluidsimfoam-0.0.6/src/fluidsimfoam/testing.py
+-rw-r--r--   0        0        0       77 2023-05-09 20:05:14.251128 fluidsimfoam-0.0.6/src/fluidsimfoam/util/__init__.py
+-rw-r--r--   0        0        0      238 2023-05-09 20:27:04.597492 fluidsimfoam-0.0.6/src/fluidsimfoam/util/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     5471 2023-06-02 09:35:15.850833 fluidsimfoam-0.0.6/src/fluidsimfoam/util/__pycache__/console.cpython-310.pyc
+-rw-r--r--   0        0        0     6906 2023-06-02 09:35:05.306884 fluidsimfoam-0.0.6/src/fluidsimfoam/util/console.py
+-rw-r--r--   0        0        0     8672 1970-01-01 00:00:00.000000 fluidsimfoam-0.0.6/PKG-INFO
```

### Comparing `fluidsimfoam-0.0.5/LICENSE` & `fluidsimfoam-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `fluidsimfoam-0.0.5/README.md` & `fluidsimfoam-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `fluidsimfoam-0.0.5/pyproject.toml` & `fluidsimfoam-0.0.6/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [tool.poetry]
 name = "fluidsimfoam"
-version = "0.0.5"
+version = "0.0.6"
 description = "Python framework for OpenFOAM"
 authors = ["pierre.augier <pierre.augier@univ-grenoble-alpes.fr>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 fluidsim-core = "^0.7.3"
 inflection = "^0.5.1"
 fluiddyn = "^0.5.2"
-ipython = "^8.11.0"
+ipython = "^8.14.0"
 pandas = "^1.5.3"
 jinja2 = "^3.1.2"
 lark = "^1.1.5"
 rich = "^13.3.3"
 invoke = "^2.0.0"
-PySide6 = {version = "^6.5.0", optional = true, python = ">=3.9,<3.12"}
+PySide6 = {version = "^6.5.1", optional = true, python = ">=3.9,<3.12"}
 jupyterlab = {version = "^3.6.3", optional = true}
 jupyterlab_myst = {version = "^1.1.3", optional = true}
 jupytext = {version = "^1.14.5", optional = true}
 mdformat-myst = {version = "^0.1.4", optional = true}
 
 [tool.poetry.extras]
 qt = ["PySide6"]
@@ -39,14 +39,16 @@
 pytest-cov = "^4.0.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.1.0"
 flake8 = "^6.0.0"
 isort = "^5.12.0"
 ipdb = "^0.13.13"
+build = "^0.10.0"
+twine = "^4.0.2"
 
 [tool.poetry.group.doc.dependencies]
 myst-nb = "^0.17.1"
 sphinx-inline-tabs = "^2022.1.2b11"
 sphinx-copybutton = "^0.5.1"
 pydata-sphinx-theme = "^0.13.1"
```

### Comparing `fluidsimfoam-0.0.5/src/fluidsimfoam/__init__.py` & `fluidsimfoam-0.0.6/src/fluidsimfoam/__init__.py`

 * *Files identical despite different names*

### Comparing `fluidsimfoam-0.0.5/src/fluidsimfoam/foam_input_files/__init__.py` & `fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/__init__.py`

 * *Files identical despite different names*

### Comparing `fluidsimfoam-0.0.5/src/fluidsimfoam/foam_input_files/__pycache__/__init__.cpython-310.pyc` & `fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed May 10 08:15:22 2023 UTC, .py size: 2280 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 23% similar despite different names*

```diff
@@ -1,162 +1,215 @@
-00000000: 6f0d 0d0a 0000 0000 9a52 5b64 e808 0000  o........R[d....
+00000000: 6f0d 0d0a 0000 0000 a2b4 7964 5c0c 0000  o.........yd\...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0011 0000 0040 0000 0073 ce00 0000 6400  .....@...s....d.
+00000020: 0004 0000 0040 0000 0073 0a01 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 6d03 5a03  Z.d.d.l.m.Z.m.Z.
-00000040: 0100 6403 6404 6c04 6d05 5a05 6d06 5a06  ..d.d.l.m.Z.m.Z.
-00000050: 6d07 5a07 6d08 5a08 0100 6403 6405 6c09  m.Z.m.Z...d.d.l.
-00000060: 6d0a 5a0a 6d0b 5a0b 0100 6700 6406 a201  m.Z.m.Z...g.d...
-00000070: 5a0c 4700 6407 6408 8400 6408 6502 8303  Z.G.d.d...d.e...
-00000080: 5a0d 6409 5a0e 650e 6403 640a 8502 1900  Z.d.Z.e.d.d.....
-00000090: 5a0e 650f 640b 640c 6401 640d 640e 640f  Z.e.d.d.d.d.d.d.
-000000a0: 6410 6411 6401 6412 6413 6414 6415 6413  d.d.d.d.d.d.d.d.
-000000b0: 6416 6417 8d0f 5a10 6403 6418 6c11 6d12  d.d...Z.d.d.l.m.
-000000c0: 5a12 6d13 5a13 6d14 5a14 0100 6403 6419  Z.m.Z.m.Z...d.d.
-000000d0: 6c15 6d16 5a16 0100 6403 641a 6c17 6d18  l.m.Z...d.d.l.m.
-000000e0: 5a18 6d19 5a19 6d1a 5a1a 0100 6403 641b  Z.m.Z.m.Z...d.d.
-000000f0: 6c1b 6d1c 5a1c 0100 641c 5300 291d 7af9  l.m.Z...d.S.).z.
-00000100: 4f70 656e 464f 414d 2069 6e70 7574 2066  OpenFOAM input f
-00000110: 696c 6573 0a0a 2e2e 2072 7562 7269 633a  iles.... rubric:
-00000120: 3a20 4153 5420 616e 6420 7061 7273 6572  : AST and parser
-00000130: 0a0a 2e2e 2061 7574 6f73 756d 6d61 7279  .... autosummary
-00000140: 3a3a 0a20 2020 3a74 6f63 7472 6565 3a0a  ::.   :toctree:.
-00000150: 0a20 2020 2061 7374 0a20 2020 2067 656e  .    ast.    gen
-00000160: 6572 6174 6f72 730a 2020 2020 7061 7273  erators.    pars
-00000170: 6572 0a0a 2e2e 2072 7562 7269 633a 3a20  er.... rubric:: 
-00000180: 4865 6c70 6572 2074 6f20 6372 6561 7465  Helper to create
-00000190: 2069 6e70 7574 2066 696c 6573 0a0a 2e2e   input files....
-000001a0: 2061 7574 6f73 756d 6d61 7279 3a3a 0a20   autosummary::. 
-000001b0: 2020 3a74 6f63 7472 6565 3a0a 0a20 2020    :toctree:..   
-000001c0: 2062 6c6f 636b 6d65 7368 0a20 2020 2066   blockmesh.    f
-000001d0: 6965 6c64 730a 2020 2020 6676 5f73 6368  ields.    fv_sch
-000001e0: 656d 6573 0a20 2020 2063 6f6e 7374 616e  emes.    constan
-000001f0: 745f 6669 6c65 730a 0ae9 0000 0000 2902  t_files.......).
-00000200: da03 4142 43da 0e61 6273 7472 6163 746d  ..ABC..abstractm
-00000210: 6574 686f 64e9 0100 0000 2904 da04 4469  ethod.....)...Di
-00000220: 6374 da0d 466f 616d 496e 7075 7446 696c  ct..FoamInputFil
-00000230: 65da 044c 6973 74da 0556 616c 7565 2902  e..List..Value).
-00000240: da04 6475 6d70 da05 7061 7273 6529 1072  ..dump..parse).r
-00000250: 0a00 0000 7209 0000 0072 0600 0000 da0e  ....r....r......
-00000260: 4445 4641 554c 545f 4845 4144 4552 7205  DEFAULT_HEADERr.
-00000270: 0000 0072 0700 0000 7208 0000 00da 0d42  ...r....r......B
-00000280: 6c6f 636b 4d65 7368 4469 6374 da0e 566f  lockMeshDict..Vo
-00000290: 6c53 6361 6c61 7246 6965 6c64 da0e 566f  lScalarField..Vo
-000002a0: 6c56 6563 746f 7246 6965 6c64 da0f 4676  lVectorField..Fv
-000002b0: 5363 6865 6d65 7348 656c 7065 72da 0656  SchemesHelper..V
-000002c0: 6572 7465 78da 0f72 6561 645f 6669 656c  ertex..read_fiel
-000002d0: 645f 6669 6c65 da0a 4669 6c65 4865 6c70  d_file..FileHelp
-000002e0: 6572 da12 436f 6e73 7461 6e74 4669 6c65  er..ConstantFile
-000002f0: 4865 6c70 6572 da18 426c 6f63 6b4d 6573  Helper..BlockMes
-00000300: 6844 6963 7452 6563 7469 6c69 6e65 6172  hDictRectilinear
-00000310: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-00000320: 0003 0000 0040 0000 0073 2800 0000 6500  .....@...s(...e.
-00000330: 5a01 6400 5a02 6401 5a03 6504 6402 6403  Z.d.Z.d.Z.e.d.d.
-00000340: 8400 8301 5a05 6504 6404 6405 8400 8301  ....Z.e.d.d.....
-00000350: 5a06 6406 5300 2907 7212 0000 007a 2341  Z.d.S.).r....z#A
-00000360: 6273 7472 6163 7420 636c 6173 7320 666f  bstract class fo
-00000370: 7220 2248 656c 7065 7222 206f 626a 6563  r "Helper" objec
-00000380: 7473 6302 0000 0000 0000 0000 0000 0002  tsc.............
-00000390: 0000 0001 0000 0043 0000 00f3 0400 0000  .......C........
-000003a0: 6401 5300 2902 7a1a 436f 6d70 6c65 7465  d.S.).z.Complete
-000003b0: 2074 6865 2070 6172 616d 7320 6f62 6a65   the params obje
-000003c0: 6374 4ea9 00a9 02da 0473 656c 66da 0670  ctN......self..p
-000003d0: 6172 616d 7372 1600 0000 7216 0000 00fa  aramsr....r.....
-000003e0: 542f 686f 6d65 2f75 7365 7273 2f61 7567  T/home/users/aug
-000003f0: 6965 7233 7069 2f44 6576 2f66 6c75 6964  ier3pi/Dev/fluid
-00000400: 7369 6d66 6f61 6d2f 7372 632f 666c 7569  simfoam/src/flui
-00000410: 6473 696d 666f 616d 2f66 6f61 6d5f 696e  dsimfoam/foam_in
-00000420: 7075 745f 6669 6c65 732f 5f5f 696e 6974  put_files/__init
-00000430: 5f5f 2e70 79da 0f63 6f6d 706c 6574 655f  __.py..complete_
-00000440: 7061 7261 6d73 3400 0000 f302 0000 0004  params4.........
-00000450: 007a 1a46 696c 6548 656c 7065 722e 636f  .z.FileHelper.co
-00000460: 6d70 6c65 7465 5f70 6172 616d 7363 0200  mplete_paramsc..
-00000470: 0000 0000 0000 0000 0000 0200 0000 0100  ................
-00000480: 0000 4300 0000 7215 0000 0029 027a 244d  ..C...r....).z$M
-00000490: 616b 6520 7468 6520 4153 5420 636f 7272  ake the AST corr
-000004a0: 6573 706f 6e64 696e 6720 746f 2061 2066  esponding to a f
-000004b0: 696c 654e 7216 0000 0072 1700 0000 7216  ileNr....r....r.
-000004c0: 0000 0072 1600 0000 721a 0000 00da 096d  ...r....r......m
-000004d0: 616b 655f 7472 6565 3800 0000 721c 0000  ake_tree8...r...
-000004e0: 007a 1446 696c 6548 656c 7065 722e 6d61  .z.FileHelper.ma
-000004f0: 6b65 5f74 7265 654e 2907 da08 5f5f 6e61  ke_treeN)...__na
-00000500: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
-00000510: da0c 5f5f 7175 616c 6e61 6d65 5f5f da07  ..__qualname__..
-00000520: 5f5f 646f 635f 5f72 0300 0000 721b 0000  __doc__r....r...
-00000530: 0072 1d00 0000 7216 0000 0072 1600 0000  .r....r....r....
-00000540: 7216 0000 0072 1a00 0000 7212 0000 0031  r....r....r....1
-00000550: 0000 0073 0c00 0000 0800 0401 0202 0a01  ...s............
-00000560: 0203 0e01 7212 0000 0061 3102 0000 0a2f  ....r....a1..../
-00000570: 2a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  *---------------
-00000580: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000590: 2d2a 2d20 432b 2b20 2d2a 2d2d 2d2d 2d2d  -*- C++ -*------
-000005a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000005b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2a5c 0a7c  ------------*\.|
-000005c0: 203d 3d3d 3d3d 3d3d 3d3d 2020 2020 2020   =========      
-000005d0: 2020 2020 2020 2020 2020 207c 2020 2020             |    
-000005e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000005f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000600: 2020 2020 2020 2020 2020 2020 207c 0a7c               |.|
-00000610: 205c 5c20 2020 2020 202f 2020 4620 6965   \\      /  F ie
-00000620: 6c64 2020 2020 2020 2020 207c 204f 7065  ld         | Ope
-00000630: 6e46 4f41 4d3a 2054 6865 204f 7065 6e20  nFOAM: The Open 
-00000640: 536f 7572 6365 2043 4644 2054 6f6f 6c62  Source CFD Toolb
-00000650: 6f78 2020 2020 2020 2020 2020 207c 0a7c  ox           |.|
-00000660: 2020 5c5c 2020 2020 2f20 2020 4f20 7065    \\    /   O pe
-00000670: 7261 7469 6f6e 2020 2020 207c 2056 6572  ration     | Ver
-00000680: 7369 6f6e 3a20 2076 3232 3036 2020 2020  sion:  v2206    
-00000690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000006a0: 2020 2020 2020 2020 2020 2020 207c 0a7c               |.|
-000006b0: 2020 205c 5c20 202f 2020 2020 4120 6e64     \\  /    A nd
-000006c0: 2020 2020 2020 2020 2020 207c 2057 6562             | Web
-000006d0: 7369 7465 3a20 2077 7777 2e6f 7065 6e66  site:  www.openf
-000006e0: 6f61 6d2e 636f 6d20 2020 2020 2020 2020  oam.com         
-000006f0: 2020 2020 2020 2020 2020 2020 207c 0a7c               |.|
-00000700: 2020 2020 5c5c 2f20 2020 2020 4d20 616e      \\/     M an
-00000710: 6970 756c 6174 696f 6e20 207c 2020 2020  ipulation  |    
-00000720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000740: 2020 2020 2020 2020 2020 2020 207c 0a5c               |.\
-00000750: 2a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  *---------------
-00000760: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000770: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000780: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000790: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2a2f 0ae9  ------------*/..
-000007a0: ffff ffff 5a07 6963 6f46 6f61 6dda 0973  ....Z.icoFoam..s
-000007b0: 7461 7274 5469 6d65 da07 656e 6454 696d  tartTime..endTim
-000007c0: 6567 0000 0000 0000 e03f 677b 14ae 47e1  eg.......?g{..G.
-000007d0: 7a74 3f5a 0874 696d 6553 7465 70e9 1400  zt?Z.timeStep...
-000007e0: 0000 da05 6173 6369 69e9 0600 0000 da03  ....ascii.......
-000007f0: 6f66 66da 0767 656e 6572 616c da04 7472  off..general..tr
-00000800: 7565 290f da0b 6170 706c 6963 6174 696f  ue)...applicatio
-00000810: 6e5a 0973 7461 7274 4672 6f6d 7223 0000  nZ.startFromr#..
-00000820: 005a 0673 746f 7041 7472 2400 0000 5a06  .Z.stopAtr$...Z.
-00000830: 6465 6c74 6154 5a0c 7772 6974 6543 6f6e  deltaTZ.writeCon
-00000840: 7472 6f6c 5a0d 7772 6974 6549 6e74 6572  trolZ.writeInter
-00000850: 7661 6c5a 0a70 7572 6765 5772 6974 655a  valZ.purgeWriteZ
-00000860: 0b77 7269 7465 466f 726d 6174 5a0e 7772  .writeFormatZ.wr
-00000870: 6974 6550 7265 6369 7369 6f6e 5a10 7772  itePrecisionZ.wr
-00000880: 6974 6543 6f6d 7072 6573 7369 6f6e 5a0a  iteCompressionZ.
-00000890: 7469 6d65 466f 726d 6174 5a0d 7469 6d65  timeFormatZ.time
-000008a0: 5072 6563 6973 696f 6e5a 1172 756e 5469  PrecisionZ.runTi
-000008b0: 6d65 4d6f 6469 6669 6162 6c65 2903 720c  meModifiable).r.
-000008c0: 0000 0072 1400 0000 7210 0000 0029 0172  ...r....r....).r
-000008d0: 1300 0000 2903 720d 0000 0072 0e00 0000  ....).r....r....
-000008e0: 7211 0000 0029 0172 0f00 0000 4e29 1d72  r....).r....N).r
-000008f0: 2100 0000 da03 6162 6372 0200 0000 7203  !.....abcr....r.
-00000900: 0000 00da 0361 7374 7205 0000 0072 0600  .....astr....r..
-00000910: 0000 7207 0000 0072 0800 0000 da06 7061  ..r....r......pa
-00000920: 7273 6572 7209 0000 0072 0a00 0000 da07  rserr....r......
-00000930: 5f5f 616c 6c5f 5f72 1200 0000 720b 0000  __all__r....r...
-00000940: 00da 0464 6963 745a 1444 4546 4155 4c54  ...dictZ.DEFAULT
-00000950: 5f43 4f4e 5452 4f4c 5f44 4943 545a 0962  _CONTROL_DICTZ.b
-00000960: 6c6f 636b 6d65 7368 720c 0000 0072 1400  lockmeshr....r..
-00000970: 0000 7210 0000 005a 0e63 6f6e 7374 616e  ..r....Z.constan
-00000980: 745f 6669 6c65 7372 1300 0000 da06 6669  t_filesr......fi
-00000990: 656c 6473 720d 0000 0072 0e00 0000 7211  eldsr....r....r.
-000009a0: 0000 005a 0a66 765f 7363 6865 6d65 7372  ...Z.fv_schemesr
-000009b0: 0f00 0000 7216 0000 0072 1600 0000 7216  ....r....r....r.
-000009c0: 0000 0072 1a00 0000 da08 3c6d 6f64 756c  ...r......<modul
-000009d0: 653e 0100 0000 733a 0000 0004 0010 1718  e>....s:........
-000009e0: 0210 0108 0210 1404 0c0c 0a02 0302 0102  ................
-000009f0: 0102 0102 0102 0102 0102 0102 0102 0102  ................
-00000a00: 0102 0102 0102 0102 0102 0106 f114 120c  ................
-00000a10: 0114 0110 01                             .....
+00000040: 0100 6401 6403 6c04 6d05 5a05 0100 6404  ..d.d.l.m.Z...d.
+00000050: 6405 6c06 6d07 5a07 6d08 5a08 6d09 5a09  d.l.m.Z.m.Z.m.Z.
+00000060: 6d0a 5a0a 6d0b 5a0b 0100 6404 6406 6c0c  m.Z.m.Z...d.d.l.
+00000070: 6d0d 5a0d 6d0e 5a0e 0100 6700 6407 a201  m.Z.m.Z...g.d...
+00000080: 5a0f 6408 6409 8400 5a10 640a 640b 8400  Z.d.d...Z.d.d...
+00000090: 5a11 641b 640d 640e 8401 5a12 4700 640f  Z.d.d.d...Z.G.d.
+000000a0: 6410 8400 6410 6502 8303 5a13 6411 5a14  d...d.e...Z.d.Z.
+000000b0: 6514 6404 6412 8502 1900 5a14 6404 6413  e.d.d.....Z.d.d.
+000000c0: 6c15 6d16 5a16 6d17 5a17 6d18 5a18 0100  l.m.Z.m.Z.m.Z...
+000000d0: 6404 6414 6c19 6d1a 5a1a 0100 6404 6415  d.d.l.m.Z...d.d.
+000000e0: 6c1b 6d1c 5a1c 0100 6404 6416 6c1d 6d1e  l.m.Z...d.d.l.m.
+000000f0: 5a1e 0100 6404 6417 6c1f 6d20 5a20 6d21  Z...d.d.l.m Z m!
+00000100: 5a21 6d22 5a22 6d23 5a23 0100 6404 6418  Z!m"Z"m#Z#..d.d.
+00000110: 6c24 6d25 5a25 6d26 5a26 0100 6404 6419  l$m%Z%m&Z&..d.d.
+00000120: 6c27 6d28 5a28 0100 6404 641a 6c29 6d2a  l'm(Z(..d.d.l)m*
+00000130: 5a2a 0100 640c 5300 291c 613f 0100 004f  Z*..d.S.).a?...O
+00000140: 7065 6e46 4f41 4d20 696e 7075 7420 6669  penFOAM input fi
+00000150: 6c65 730a 0a2e 2e20 7275 6272 6963 3a3a  les.... rubric::
+00000160: 2041 5354 2061 6e64 2070 6172 7365 720a   AST and parser.
+00000170: 0a2e 2e20 6175 746f 7375 6d6d 6172 793a  ... autosummary:
+00000180: 3a0a 2020 203a 746f 6374 7265 653a 0a0a  :.   :toctree:..
+00000190: 2020 2020 6173 740a 2020 2020 6765 6e65      ast.    gene
+000001a0: 7261 746f 7273 0a20 2020 2070 6172 7365  rators.    parse
+000001b0: 720a 2020 2020 666f 726d 6174 0a0a 2e2e  r.    format....
+000001c0: 2072 7562 7269 633a 3a20 4865 6c70 6572   rubric:: Helper
+000001d0: 2074 6f20 6372 6561 7465 2069 6e70 7574   to create input
+000001e0: 2066 696c 6573 0a0a 2e2e 2061 7574 6f73   files.... autos
+000001f0: 756d 6d61 7279 3a3a 0a20 2020 3a74 6f63  ummary::.   :toc
+00000200: 7472 6565 3a0a 0a20 2020 2062 6c6f 636b  tree:..    block
+00000210: 6d65 7368 0a20 2020 2063 6f6e 7472 6f6c  mesh.    control
+00000220: 5f64 6963 740a 2020 2020 6669 656c 6473  _dict.    fields
+00000230: 0a20 2020 2066 765f 7363 6865 6d65 730a  .    fv_schemes.
+00000240: 2020 2020 636f 6e73 7461 6e74 5f66 696c      constant_fil
+00000250: 6573 0a20 2020 2066 765f 6f70 7469 6f6e  es.    fv_option
+00000260: 730a 2020 2020 6465 636f 6d70 6f73 655f  s.    decompose_
+00000270: 7061 720a 2020 2020 7574 696c 0a0a e900  par.    util....
+00000280: 0000 0029 02da 0341 4243 da0e 6162 7374  ...)...ABC..abst
+00000290: 7261 6374 6d65 7468 6f64 2901 da0a 756e  ractmethod)...un
+000002a0: 6465 7273 636f 7265 e901 0000 0029 05da  derscore.....)..
+000002b0: 0444 6963 74da 0c44 696d 656e 7369 6f6e  .Dict..Dimension
+000002c0: 5365 74da 0d46 6f61 6d49 6e70 7574 4669  Set..FoamInputFi
+000002d0: 6c65 da04 4c69 7374 da05 5661 6c75 6529  le..List..Value)
+000002e0: 02da 0464 756d 70da 0570 6172 7365 2917  ...dump..parse).
+000002f0: 720c 0000 0072 0b00 0000 da16 6372 6561  r....r......crea
+00000300: 7465 5f66 6965 6c64 5f66 726f 6d5f 636f  te_field_from_co
+00000310: 6465 7208 0000 00da 0e44 4546 4155 4c54  der......DEFAULT
+00000320: 5f48 4541 4445 52da 1143 6f6e 7472 6f6c  _HEADER..Control
+00000330: 4469 6374 4865 6c70 6572 7206 0000 0072  DictHelperr....r
+00000340: 0900 0000 720a 0000 00da 0d42 6c6f 636b  ....r......Block
+00000350: 4d65 7368 4469 6374 da0e 566f 6c53 6361  MeshDict..VolSca
+00000360: 6c61 7246 6965 6c64 da0e 566f 6c56 6563  larField..VolVec
+00000370: 746f 7246 6965 6c64 da0f 4676 5363 6865  torField..FvSche
+00000380: 6d65 7348 656c 7065 72da 0656 6572 7465  mesHelper..Verte
+00000390: 78da 0f72 6561 645f 6669 656c 645f 6669  x..read_field_fi
+000003a0: 6c65 da0a 4669 6c65 4865 6c70 6572 da12  le..FileHelper..
+000003b0: 436f 6e73 7461 6e74 4669 6c65 4865 6c70  ConstantFileHelp
+000003c0: 6572 da18 426c 6f63 6b4d 6573 6844 6963  er..BlockMeshDic
+000003d0: 7452 6563 7469 6c69 6e65 6172 da0f 4676  tRectilinear..Fv
+000003e0: 4f70 7469 6f6e 7348 656c 7065 7272 0700  OptionsHelperr..
+000003f0: 0000 da16 4465 636f 6d70 6f73 6550 6172  ....DecomposePar
+00000400: 4469 6374 4865 6c70 6572 da0b 666f 726d  DictHelper..form
+00000410: 6174 5f63 6f64 65da 0f46 6f61 6d46 6f72  at_code..FoamFor
+00000420: 6d61 7445 7272 6f72 6301 0000 0000 0000  matErrorc.......
+00000430: 0000 0000 0001 0000 0004 0000 0043 0000  .............C..
+00000440: 0073 1000 0000 7400 7c00 8301 a001 6401  .s....t.|.....d.
+00000450: 6402 a102 5300 2903 4eda 012e da01 5f29  d...S.).N....._)
+00000460: 0272 0400 0000 da07 7265 706c 6163 6529  .r......replace)
+00000470: 01da 046e 616d 65a9 0072 2100 0000 fa4b  ...name..r!....K
+00000480: 2f68 6f6d 652f 7069 6572 7265 2f44 6576  /home/pierre/Dev
+00000490: 2f66 6c75 6964 7369 6d66 6f61 6d2f 7372  /fluidsimfoam/sr
+000004a0: 632f 666c 7569 6473 696d 666f 616d 2f66  c/fluidsimfoam/f
+000004b0: 6f61 6d5f 696e 7075 745f 6669 6c65 732f  oam_input_files/
+000004c0: 5f5f 696e 6974 5f5f 2e70 79da 0b5f 6173  __init__.py.._as
+000004d0: 5f70 795f 6e61 6d65 3e00 0000 7302 0000  _py_name>...s...
+000004e0: 0010 0172 2300 0000 6302 0000 0000 0000  ...r#...c.......
+000004f0: 0000 0000 0006 0000 000a 0000 0043 0000  .............C..
+00000500: 0073 6000 0000 7c00 a000 a100 4400 5d29  .s`...|.....D.])
+00000510: 5c02 7d02 7d03 7401 7c02 8301 7d04 7a06  \.}.}.t.|...}.z.
+00000520: 7c01 7c04 1900 7d05 5700 6e0b 0400 7402  |.|...}.W.n...t.
+00000530: 7403 6602 791d 0100 0100 0100 5900 7104  t.f.y.......Y.q.
+00000540: 7700 7404 7c03 7405 8302 7229 7406 7c03  w.t.|.t...r)t.|.
+00000550: 7c05 8302 0100 7104 7c05 7c00 7c02 3c00  |.....q.|.|.|.<.
+00000560: 7104 6400 5300 a901 4e29 07da 0569 7465  q.d.S...N)...ite
+00000570: 6d73 7204 0000 00da 084b 6579 4572 726f  msr......KeyErro
+00000580: 72da 0e41 7474 7269 6275 7465 4572 726f  r..AttributeErro
+00000590: 72da 0a69 7369 6e73 7461 6e63 65da 0464  r..isinstance..d
+000005a0: 6963 74da 185f 7570 6461 7465 5f64 6963  ict.._update_dic
+000005b0: 745f 7769 7468 5f70 6172 616d 7329 06da  t_with_params)..
+000005c0: 0464 6174 615a 0b70 6172 616d 735f 6461  .dataZ.params_da
+000005d0: 7461 da03 6b65 79da 0576 616c 7565 7220  ta..key..valuer 
+000005e0: 0000 005a 0b70 6172 616d 5f76 616c 7565  ...Z.param_value
+000005f0: 7221 0000 0072 2100 0000 7222 0000 0072  r!...r!...r"...r
+00000600: 2a00 0000 4200 0000 7316 0000 0010 0108  *...B...s.......
+00000610: 0102 020c 0110 0104 0102 ff0a 030c 010a  ................
+00000620: 0204 f572 2a00 0000 4e63 0400 0000 0000  ...r*...Nc......
+00000630: 0000 0000 0000 0700 0000 0500 0000 4300  ..............C.
+00000640: 0000 7354 0000 0074 007c 0183 017d 017c  ..sT...t.|...}.|
+00000650: 006a 017c 017c 0364 018d 027d 047c 02a0  .j.|.|.d...}.|..
+00000660: 02a1 0044 005d 185c 027d 057d 0674 037c  ...D.].\.}.}.t.|
+00000670: 0674 0483 0272 1f74 057c 047c 057c 0683  .t...r.t.|.|.|..
+00000680: 0301 0071 0f7c 04a0 0674 007c 0583 017c  ...q.|...t.|...|
+00000690: 06a1 0201 0071 0f64 0053 0029 024e 2901  .....q.d.S.).N).
+000006a0: da03 646f 6329 0772 2300 0000 da0a 5f73  ..doc).r#....._s
+000006b0: 6574 5f63 6869 6c64 7225 0000 0072 2800  et_childr%...r(.
+000006c0: 0000 7229 0000 00da 155f 636f 6d70 6c65  ..r)....._comple
+000006d0: 7465 5f70 6172 616d 735f 6469 6374 da0b  te_params_dict..
+000006e0: 5f73 6574 5f61 7474 7269 6229 07da 0973  _set_attrib)...s
+000006f0: 7562 7061 7261 6d73 7220 0000 00da 0764  ubparamsr .....d
+00000700: 6566 6175 6c74 722e 0000 005a 0c73 7562  efaultr....Z.sub
+00000710: 7375 6270 6172 616d 7372 2c00 0000 722d  subparamsr,...r-
+00000720: 0000 0072 2100 0000 7221 0000 0072 2200  ...r!...r!...r".
+00000730: 0000 7230 0000 0051 0000 0073 1000 0000  ..r0...Q...s....
+00000740: 0801 0e01 1002 0a01 0c01 0201 1202 04fb  ................
+00000750: 7230 0000 0063 0000 0000 0000 0000 0000  r0...c..........
+00000760: 0000 0000 0000 0300 0000 4000 0000 7328  ..........@...s(
+00000770: 0000 0065 005a 0164 005a 0264 015a 0365  ...e.Z.d.Z.d.Z.e
+00000780: 0464 0264 0384 0083 015a 0565 0464 0464  .d.d.....Z.e.d.d
+00000790: 0584 0083 015a 0664 0653 0029 0772 1600  .....Z.d.S.).r..
+000007a0: 0000 7a23 4162 7374 7261 6374 2063 6c61  ..z#Abstract cla
+000007b0: 7373 2066 6f72 2022 4865 6c70 6572 2220  ss for "Helper" 
+000007c0: 6f62 6a65 6374 7363 0200 0000 0000 0000  objectsc........
+000007d0: 0000 0000 0200 0000 0100 0000 4300 0000  ............C...
+000007e0: f304 0000 0064 0153 0029 027a 1a43 6f6d  .....d.S.).z.Com
+000007f0: 706c 6574 6520 7468 6520 7061 7261 6d73  plete the params
+00000800: 206f 626a 6563 744e 7221 0000 00a9 02da   objectNr!......
+00000810: 0473 656c 66da 0670 6172 616d 7372 2100  .self..paramsr!.
+00000820: 0000 7221 0000 0072 2200 0000 da0f 636f  ..r!...r".....co
+00000830: 6d70 6c65 7465 5f70 6172 616d 7360 0000  mplete_params`..
+00000840: 00f3 0200 0000 0400 7a1a 4669 6c65 4865  ........z.FileHe
+00000850: 6c70 6572 2e63 6f6d 706c 6574 655f 7061  lper.complete_pa
+00000860: 7261 6d73 6302 0000 0000 0000 0000 0000  ramsc...........
+00000870: 0002 0000 0001 0000 0043 0000 0072 3400  .........C...r4.
+00000880: 0000 2902 7a24 4d61 6b65 2074 6865 2041  ..).z$Make the A
+00000890: 5354 2063 6f72 7265 7370 6f6e 6469 6e67  ST corresponding
+000008a0: 2074 6f20 6120 6669 6c65 4e72 2100 0000   to a fileNr!...
+000008b0: 7235 0000 0072 2100 0000 7221 0000 0072  r5...r!...r!...r
+000008c0: 2200 0000 da09 6d61 6b65 5f74 7265 6564  ".....make_treed
+000008d0: 0000 0072 3900 0000 7a14 4669 6c65 4865  ...r9...z.FileHe
+000008e0: 6c70 6572 2e6d 616b 655f 7472 6565 4e29  lper.make_treeN)
+000008f0: 07da 085f 5f6e 616d 655f 5fda 0a5f 5f6d  ...__name__..__m
+00000900: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
+00000910: 616d 655f 5fda 075f 5f64 6f63 5f5f 7203  ame__..__doc__r.
+00000920: 0000 0072 3800 0000 723a 0000 0072 2100  ...r8...r:...r!.
+00000930: 0000 7221 0000 0072 2100 0000 7222 0000  ..r!...r!...r"..
+00000940: 0072 1600 0000 5d00 0000 730c 0000 0008  .r....]...s.....
+00000950: 0004 0102 020a 0102 030e 0172 1600 0000  ...........r....
+00000960: 6131 0200 000a 2f2a 2d2d 2d2d 2d2d 2d2d  a1..../*--------
+00000970: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000980: 2d2d 2d2d 2d2d 2d2d 2a2d 2043 2b2b 202d  --------*- C++ -
+00000990: 2a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  *---------------
+000009a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000009b0: 2d2d 2d2a 5c0a 7c20 3d3d 3d3d 3d3d 3d3d  ---*\.| ========
+000009c0: 3d20 2020 2020 2020 2020 2020 2020 2020  =               
+000009d0: 2020 7c20 2020 2020 2020 2020 2020 2020    |             
+000009e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000009f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000a00: 2020 2020 7c0a 7c20 5c5c 2020 2020 2020      |.| \\      
+00000a10: 2f20 2046 2069 656c 6420 2020 2020 2020  /  F ield       
+00000a20: 2020 7c20 4f70 656e 464f 414d 3a20 5468    | OpenFOAM: Th
+00000a30: 6520 4f70 656e 2053 6f75 7263 6520 4346  e Open Source CF
+00000a40: 4420 546f 6f6c 626f 7820 2020 2020 2020  D Toolbox       
+00000a50: 2020 2020 7c0a 7c20 205c 5c20 2020 202f      |.|  \\    /
+00000a60: 2020 204f 2070 6572 6174 696f 6e20 2020     O peration   
+00000a70: 2020 7c20 5665 7273 696f 6e3a 2020 7632    | Version:  v2
+00000a80: 3230 3620 2020 2020 2020 2020 2020 2020  206             
+00000a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000aa0: 2020 2020 7c0a 7c20 2020 5c5c 2020 2f20      |.|   \\  / 
+00000ab0: 2020 2041 206e 6420 2020 2020 2020 2020     A nd         
+00000ac0: 2020 7c20 5765 6273 6974 653a 2020 7777    | Website:  ww
+00000ad0: 772e 6f70 656e 666f 616d 2e63 6f6d 2020  w.openfoam.com  
+00000ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000af0: 2020 2020 7c0a 7c20 2020 205c 5c2f 2020      |.|    \\/  
+00000b00: 2020 204d 2061 6e69 7075 6c61 7469 6f6e     M anipulation
+00000b10: 2020 7c20 2020 2020 2020 2020 2020 2020    |             
+00000b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000b40: 2020 2020 7c0a 5c2a 2d2d 2d2d 2d2d 2d2d      |.\*--------
+00000b50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000b60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000b70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000b80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000b90: 2d2d 2d2a 2f0a e9ff ffff ff29 0372 1000  ---*/......).r..
+00000ba0: 0000 7218 0000 0072 1400 0000 2901 7217  ..r....r....).r.
+00000bb0: 0000 0029 0172 0f00 0000 2901 721a 0000  ...).r....).r...
+00000bc0: 0029 0472 1100 0000 7212 0000 0072 0d00  .).r....r....r..
+00000bd0: 0000 7215 0000 0029 0272 1c00 0000 721b  ..r....).r....r.
+00000be0: 0000 0029 0172 1900 0000 2901 7213 0000  ...).r....).r...
+00000bf0: 0072 2400 0000 292b 723e 0000 00da 0361  .r$...)+r>.....a
+00000c00: 6263 7202 0000 0072 0300 0000 5a0a 696e  bcr....r....Z.in
+00000c10: 666c 6563 7469 6f6e 7204 0000 00da 0361  flectionr......a
+00000c20: 7374 7206 0000 0072 0700 0000 7208 0000  str....r....r...
+00000c30: 0072 0900 0000 720a 0000 00da 0670 6172  .r....r......par
+00000c40: 7365 7272 0b00 0000 720c 0000 00da 075f  serr....r......_
+00000c50: 5f61 6c6c 5f5f 7223 0000 0072 2a00 0000  _all__r#...r*...
+00000c60: 7230 0000 0072 1600 0000 720e 0000 005a  r0...r....r....Z
+00000c70: 0962 6c6f 636b 6d65 7368 7210 0000 0072  .blockmeshr....r
+00000c80: 1800 0000 7214 0000 005a 0e63 6f6e 7374  ....r....Z.const
+00000c90: 616e 745f 6669 6c65 7372 1700 0000 5a0c  ant_filesr....Z.
+00000ca0: 636f 6e74 726f 6c5f 6469 6374 720f 0000  control_dictr...
+00000cb0: 005a 0d64 6563 6f6d 706f 7365 5f70 6172  .Z.decompose_par
+00000cc0: 721a 0000 00da 0666 6965 6c64 7372 1100  r......fieldsr..
+00000cd0: 0000 7212 0000 0072 0d00 0000 7215 0000  ..r....r....r...
+00000ce0: 00da 0666 6f72 6d61 7472 1c00 0000 721b  ...formatr....r.
+00000cf0: 0000 005a 0a66 765f 6f70 7469 6f6e 7372  ...Z.fv_optionsr
+00000d00: 1900 0000 5a0a 6676 5f73 6368 656d 6573  ....Z.fv_schemes
+00000d10: 7213 0000 0072 2100 0000 7221 0000 0072  r....r!...r!...r
+00000d20: 2100 0000 7222 0000 00da 083c 6d6f 6475  !...r".....<modu
+00000d30: 6c65 3e01 0000 0073 2800 0000 0400 101b  le>....s(.......
+00000d40: 0c02 1c02 1001 0802 081b 0804 0a0f 100c  ................
+00000d50: 040c 0c0a 1402 0c01 0c01 0c01 1801 1006  ................
+00000d60: 0c01 1001                                ....
```

### Comparing `fluidsimfoam-0.0.5/src/fluidsimfoam/foam_input_files/__pycache__/ast.cpython-310.pyc` & `fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/__pycache__/ast.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu May 11 13:30:48 2023 UTC, .py size: 16418 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 08ee 5c64 2240 0000  o.........\d"@..
+00000000: 6f0d 0d0a 0000 0000 1495 7964 7d41 0000  o.........yd}A..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 8e01 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 6d04 5a04 0100 6401 6404 6c05  m.Z.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6401 6405 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 0100 6401 6406 6c09 6d0a 5a0a 0100 6401  ..d.d.l.m.Z...d.
 00000070: 6407 6c0b 6d0c 5a0c 0100 6401 6402 6c0d  d.l.m.Z...d.d.l.
@@ -59,982 +59,991 @@
 000003a0: 7465 4572 726f 72da 0573 706c 6974 da03  teError..split..
 000003b0: 696e 74da 0773 796d 626f 6c73 da05 696e  int..symbols..in
 000003c0: 6465 7829 09da 0575 6e69 7473 da06 7265  dex)...units..re
 000003d0: 7375 6c74 da04 7369 676e 721c 0000 005a  sult..signr....Z
 000003e0: 0875 6e69 745f 616c 6c5a 096e 6578 745f  .unit_allZ.next_
 000003f0: 6f70 6572 da09 756e 6974 5f6e 616d 655a  oper..unit_nameZ
 00000400: 0a75 6e69 745f 7661 6c75 655a 0a75 6e69  .unit_valueZ.uni
-00000410: 745f 696e 6465 78a9 0072 2100 0000 fa4f  t_index..r!....O
-00000420: 2f68 6f6d 652f 7573 6572 732f 6175 6769  /home/users/augi
-00000430: 6572 3370 692f 4465 762f 666c 7569 6473  er3pi/Dev/fluids
-00000440: 696d 666f 616d 2f73 7263 2f66 6c75 6964  imfoam/src/fluid
-00000450: 7369 6d66 6f61 6d2f 666f 616d 5f69 6e70  simfoam/foam_inp
-00000460: 7574 5f66 696c 6573 2f61 7374 2e70 79da  ut_files/ast.py.
-00000470: 0e73 7472 3266 6f61 6d5f 756e 6974 7310  .str2foam_units.
-00000480: 0000 0073 3000 0000 0a01 0401 0401 0201  ...s0...........
-00000490: 1401 0c01 0401 0401 0801 02fd 0805 0c01  ................
-000004a0: 0c01 1001 0801 0e01 0a01 0a02 0801 0a01  ................
-000004b0: 0c01 1001 04ec 0415 7223 0000 0063 0100  ........r#...c..
-000004c0: 0000 0000 0000 0000 0000 0500 0000 0800  ................
-000004d0: 0000 4300 0000 73a8 0000 0067 007d 0174  ..C...s....g.}.t
-000004e0: 0074 017c 0083 0244 005d 2f5c 027d 027d  .t.|...D.]/\.}.}
-000004f0: 037c 0364 016b 0272 1071 077c 0364 016b  .|.d.k.r.q.|.d.k
-00000500: 0472 1664 026e 0164 037d 0474 027c 0383  .r.d.n.d.}.t.|..
-00000510: 0164 046b 0272 287c 01a0 037c 049b 007c  .d.k.r(|...|...|
-00000520: 029b 009d 02a1 0101 0071 077c 01a0 037c  .........q.|...|
-00000530: 049b 007c 029b 0064 0574 027c 0383 019b  ...|...d.t.|....
-00000540: 009d 04a1 0101 0071 0764 06a0 047c 01a1  .......q.d...|..
-00000550: 017d 017c 01a0 0564 02a1 0172 497c 0164  .}.|...d...rI|.d
-00000560: 0464 0085 0219 007d 017c 0153 007c 01a0  .d.....}.|.S.|..
-00000570: 0564 03a1 0172 5264 077c 0117 007d 017c  .d...rRd.|...}.|
-00000580: 0153 0029 084e 7201 0000 0072 1100 0000  .S.).Nr....r....
-00000590: fa01 2f72 0f00 0000 7212 0000 0072 1000  ../r....r....r..
-000005a0: 0000 7213 0000 0029 06da 037a 6970 721b  ..r....)...zipr.
-000005b0: 0000 00da 0361 6273 da06 6170 7065 6e64  .....abs..append
-000005c0: da04 6a6f 696e da0a 7374 6172 7473 7769  ..join..startswi
-000005d0: 7468 2905 da0a 666f 616d 5f75 6e69 7473  th)...foam_units
-000005e0: 721e 0000 00da 0673 796d 626f 6cda 0865  r......symbol..e
-000005f0: 7870 6f6e 656e 74da 086f 7065 7261 746f  xponent..operato
-00000600: 7272 2100 0000 7221 0000 0072 2200 0000  rr!...r!...r"...
-00000610: da0e 666f 616d 5f75 6e69 7473 3273 7472  ..foam_units2str
-00000620: 2b00 0000 731e 0000 0004 0112 0108 0102  +...s...........
-00000630: 0110 010c 0114 011e 020a 010a 010c 0104  ................
-00000640: 030a fe08 0104 0172 2e00 0000 e914 0000  .......r........
-00000650: 0063 0200 0000 0000 0000 0000 0000 0300  .c..............
-00000660: 0000 0800 0000 4300 0000 7344 0000 007a  ......C...sD...z
-00000670: 1074 007c 0174 0164 0164 0284 007c 00a0  .t.|.t.d.d...|..
-00000680: 02a1 0044 0083 0183 0183 027d 0157 006e  ...D.......}.W.n
-00000690: 0b04 0074 0379 1b01 0001 0001 0064 037d  ...t.y.......d.}
-000006a0: 0159 006e 0177 0064 047d 027c 017c 0217  .Y.n.w.d.}.|.|..
-000006b0: 0053 0029 054e 6301 0000 0000 0000 0000  .S.).Nc.........
-000006c0: 0000 0003 0000 0005 0000 0073 0000 0073  ...........s...s
-000006d0: 2a00 0000 8100 7c00 5d10 5c02 7d01 7d02  *.....|.].\.}.}.
-000006e0: 7400 7c02 7401 7402 6602 8302 7302 7403  t.|.t.t.f...s.t.
-000006f0: 7c01 8301 5600 0100 7102 6400 5300 a901  |...V...q.d.S...
-00000700: 4e29 04da 0a69 7369 6e73 7461 6e63 65da  N)...isinstance.
-00000710: 0444 6963 74da 044c 6973 74da 036c 656e  .Dict..List..len
-00000720: 2903 da02 2e30 da03 6b65 79da 0576 616c  )....0..key..val
-00000730: 7565 7221 0000 0072 2100 0000 7222 0000  uer!...r!...r"..
-00000740: 00da 093c 6765 6e65 7870 723e 4100 0000  ...<genexpr>A...
-00000750: 730e 0000 0002 8004 0006 020c 0102 fd06  s...............
-00000760: 010a ff7a 2b5f 636f 6d70 7574 655f 7370  ...z+_compute_sp
-00000770: 6163 6573 5f74 6f5f 616c 6967 6e2e 3c6c  aces_to_align.<l
-00000780: 6f63 616c 733e 2e3c 6765 6e65 7870 723e  ocals>.<genexpr>
-00000790: 7201 0000 00e9 0400 0000 2904 da03 6d69  r.........)...mi
-000007a0: 6eda 036d 6178 da05 6974 656d 73da 0a56  n..max..items..V
-000007b0: 616c 7565 4572 726f 7229 03da 0464 6174  alueError)...dat
-000007c0: 61da 0a6d 6178 5f6c 656e 6774 685a 0d64  a..max_lengthZ.d
-000007d0: 6566 6175 6c74 5f73 7061 6365 7221 0000  efault_spacer!..
-000007e0: 0072 2100 0000 7222 0000 00da 185f 636f  .r!...r"....._co
-000007f0: 6d70 7574 655f 7370 6163 6573 5f74 6f5f  mpute_spaces_to_
-00000800: 616c 6967 6e3d 0000 0073 1800 0000 0201  align=...s......
-00000810: 0201 0201 0801 0602 06fe 08fe 0c08 0801  ................
-00000820: 02ff 0403 0801 7240 0000 0063 0000 0000  ......r@...c....
-00000830: 0000 0000 0000 0000 0000 0000 0200 0000  ................
-00000840: 4000 0000 7314 0000 0065 005a 0164 005a  @...s....e.Z.d.Z
-00000850: 0264 0164 0284 005a 0364 0353 0029 04da  .d.d...Z.d.S.)..
-00000860: 044e 6f64 6563 0200 0000 0000 0000 0000  .Nodec..........
-00000870: 0000 0200 0000 0300 0000 4300 0000 7320  ..........C...s 
-00000880: 0000 0074 007c 0183 0174 007c 0083 0175  ...t.|...t.|...u
-00000890: 0072 0e7c 006a 017c 016a 016b 0253 0064  .r.|.j.|.j.k.S.d
-000008a0: 0153 0029 024e 4629 02da 0474 7970 65da  .S.).NF)...type.
-000008b0: 085f 5f64 6963 745f 5f29 02da 0473 656c  .__dict__)...sel
-000008c0: 66da 056f 7468 6572 7221 0000 0072 2100  f..otherr!...r!.
-000008d0: 0000 7222 0000 00da 065f 5f65 715f 5f4f  ..r".....__eq__O
-000008e0: 0000 0073 0600 0000 1001 0c01 0401 7a0b  ...s..........z.
-000008f0: 4e6f 6465 2e5f 5f65 715f 5f4e 2904 da08  Node.__eq__N)...
-00000900: 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f 6475  __name__..__modu
-00000910: 6c65 5f5f da0c 5f5f 7175 616c 6e61 6d65  le__..__qualname
-00000920: 5f5f 7246 0000 0072 2100 0000 7221 0000  __rF...r!...r!..
-00000930: 0072 2100 0000 7222 0000 0072 4100 0000  .r!...r"...rA...
-00000940: 4e00 0000 7304 0000 0008 000c 0172 4100  N...s........rA.
-00000950: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
-00000960: 0000 0008 0000 0040 0000 0073 5000 0000  .......@...sP...
-00000970: 6500 5a01 6400 5a02 0901 0902 0901 640e  e.Z.d.Z.......d.
-00000980: 6403 6503 6404 6504 6503 1900 6405 6504  d.e.d.e.e...d.e.
-00000990: 6503 1900 6606 6406 6407 8405 5a05 6408  e...f.d.d...Z.d.
-000009a0: 6409 8400 5a06 640f 640a 640b 8401 5a07  d...Z.d.d.d...Z.
-000009b0: 6508 640c 640d 8400 8301 5a09 6401 5300  e.d.d.....Z.d.S.
-000009c0: 2910 da0e 4e6f 6465 4c69 6b65 5079 4469  )...NodeLikePyDi
-000009d0: 6374 4e46 723e 0000 00da 0a64 696d 656e  ctNFr>.....dimen
-000009e0: 7369 6f6e 73da 0863 6f6d 6d65 6e74 7363  sions..commentsc
-000009f0: 0500 0000 0000 0000 0000 0000 0b00 0000  ................
-00000a00: 0700 0000 4300 0000 73fa 0000 007c 0264  ....C...s....|.d
-00000a10: 0075 0072 0669 007d 027c 0464 0075 0072  .u.r.i.}.|.d.u.r
-00000a20: 0c69 007d 047c 01a0 00a1 0044 005d 6a5c  .i.}.|.....D.]j\
-00000a30: 027d 057d 0674 017c 0674 0264 0083 0174  .}.}.t.|.t.d...t
-00000a40: 0366 0283 0272 247c 00a0 047c 057c 06a1  .f...r$|...|.|..
-00000a50: 0201 0071 1074 017c 0674 0574 0666 0283  ...q.t.|.t.t.f..
-00000a60: 0272 4d7c 0364 0175 0072 367c 00a0 047c  .rM|.d.u.r6|...|
-00000a70: 057c 06a1 0201 0071 107c 02a0 077c 057c  .|.....q.|...|.|
-00000a80: 03a1 027d 0774 017c 0674 0683 0272 4574  ...}.t.|.t...rEt
-00000a90: 087c 0683 017d 067c 00a0 097c 057c 067c  .|...}.|...|.|.|
-00000aa0: 07a1 0301 0071 1074 017c 0674 0a83 0272  .....q.t.|.t...r
-00000ab0: 757c 02a0 077c 0564 00a1 027d 087c 04a0  u|...|.d...}.|..
-00000ac0: 077c 0564 00a1 027d 0974 0b69 007c 057c  .|.d...}.t.i.|.|
-00000ad0: 0964 028d 037d 0a7c 0a6a 0c7c 067c 087c  .d...}.|.j.|.|.|
-00000ae0: 037c 0964 038d 0401 007c 00a0 0d7c 057c  .|.d.....|...|.|
-00000af0: 0aa1 0201 0071 1074 0e74 027c 0683 0183  .....q.t.t.|....
-00000b00: 0182 0164 0053 0029 044e 4629 02da 046e  ...d.S.).NF)...n
-00000b10: 616d 6572 4c00 0000 2903 724b 0000 00da  amerL...).rK....
-00000b20: 1164 6566 6175 6c74 5f64 696d 656e 7369  .default_dimensi
-00000b30: 6f6e 724c 0000 0029 0f72 3c00 0000 7231  onrL...).r<...r1
-00000b40: 0000 0072 4200 0000 da03 7374 72da 0973  ...rB.....str..s
-00000b50: 6574 5f63 6869 6c64 7205 0000 00da 046c  et_childr......l
-00000b60: 6973 74da 0367 6574 7233 0000 00da 0973  ist..getr3.....s
-00000b70: 6574 5f76 616c 7565 da04 6469 6374 7232  et_value..dictr2
-00000b80: 0000 00da 1469 6e69 745f 6672 6f6d 5f70  .....init_from_p
-00000b90: 795f 6f62 6a65 6374 73da 095f 7365 745f  y_objects.._set_
-00000ba0: 6974 656d da13 4e6f 7449 6d70 6c65 6d65  item..NotImpleme
-00000bb0: 6e74 6564 4572 726f 7229 0b72 4400 0000  ntedError).rD...
-00000bc0: 723e 0000 0072 4b00 0000 724e 0000 0072  r>...rK...rN...r
-00000bd0: 4c00 0000 7236 0000 0072 3700 0000 da09  L...r6...r7.....
-00000be0: 6469 6d65 6e73 696f 6e5a 0f64 696d 656e  dimensionZ.dimen
-00000bf0: 7369 6f6e 735f 6469 6374 5a0d 636f 6d6d  sions_dictZ.comm
-00000c00: 656e 7473 5f64 6963 74da 036f 626a 7221  ents_dict..objr!
-00000c10: 0000 0072 2100 0000 7222 0000 0072 5500  ...r!...r"...rU.
-00000c20: 0000 5600 0000 7336 0000 0008 0704 0108  ..V...s6........
-00000c30: 0104 0110 0112 010e 010e 0108 010e 010c  ................
-00000c40: 020a 0108 0110 010a 010c 010c 010e 0104  ................
-00000c50: 0102 0102 0102 0102 0106 fc0e 060c 0204  ................
-00000c60: e97a 234e 6f64 654c 696b 6550 7944 6963  .z#NodeLikePyDic
-00000c70: 742e 696e 6974 5f66 726f 6d5f 7079 5f6f  t.init_from_py_o
-00000c80: 626a 6563 7473 6303 0000 0000 0000 0000  bjectsc.........
-00000c90: 0000 0006 0000 0005 0000 0043 0000 0073  ...........C...s
-00000ca0: 3801 0000 7400 7c02 7401 8302 7222 7c02  8...t.|.t...r"|.
-00000cb0: 7222 7400 7c02 6401 1900 7401 8302 7222  r"t.|.d...t...r"
-00000cc0: 7c02 6401 1900 7222 7402 6402 6403 8400  |.d...r"t.d.d...
-00000cd0: 7c02 6401 1900 4400 8301 8301 7222 7403  |.d...D.....r"t.
-00000ce0: a004 7c02 a101 7d02 7400 7c02 7405 6400  ..|...}.t.|.t.d.
-00000cf0: 8301 7406 7407 6603 8302 722d 6e67 7400  ..t.t.f...r-ngt.
-00000d00: 7c02 7408 8302 7239 7409 7c02 7c01 6404  |.t...r9t.|.|.d.
-00000d10: 8d02 7d02 6e5b 7400 7c02 7401 8302 7245  ..}.n[t.|.t...rE
-00000d20: 740a 7c02 7c01 6404 8d02 7d02 6e4f 7400  t.|.|.d...}.nOt.
-00000d30: 7c02 7403 6a0b 8302 7288 7c02 6a0c 7d03  |.t.j...r.|.j.}.
-00000d40: 7c02 6a0d 7d04 7c02 a00e a100 0100 6400  |.j.}.|.......d.
-00000d50: 7d05 7c04 6405 6b02 7277 7c03 6406 1900  }.|.d.k.rw|.d...
-00000d60: 6407 6b02 7264 6408 7d05 6e0b 7c03 6406  d.k.rdd.}.n.|.d.
-00000d70: 1900 6409 6b02 726d 640a 7d05 6e02 740f  ..d.k.rmd.}.n.t.
-00000d80: 8201 640b 640c 8400 7c02 4400 8301 7d02  ..d.d...|.D...}.
-00000d90: 6e09 7c04 6406 6b02 727e 640d 7d05 6e02  n.|.d.k.r~d.}.n.
-00000da0: 740f 8201 740a 7c02 7c01 7c05 640e 8d03  t...t.|.|.|.d...
-00000db0: 7d02 6e0c 7400 7c02 7410 8302 728e 6e06  }.n.t.|.t...r.n.
-00000dc0: 740f 7405 7c02 8301 8301 8201 7c00 a011  t.t.|.......|...
-00000dd0: 7c01 7c02 a102 0100 6400 5300 290f 4e72  |.|.....d.S.).Nr
-00000de0: 0100 0000 6301 0000 0000 0000 0000 0000  ....c...........
-00000df0: 0002 0000 0004 0000 0073 0000 00f3 1a00  .........s......
-00000e00: 0000 8100 7c00 5d08 7d01 7400 7c01 7401  ....|.].}.t.|.t.
-00000e10: 8302 5600 0100 7102 6400 5300 7230 0000  ..V...q.d.S.r0..
-00000e20: 0029 0272 3100 0000 7205 0000 0029 0272  .).r1...r....).r
-00000e30: 3500 0000 da01 6e72 2100 0000 7221 0000  5.....nr!...r!..
-00000e40: 0072 2200 0000 7238 0000 0080 0000 00f3  .r"...r8........
-00000e50: 0400 0000 0280 1800 7a2b 4e6f 6465 4c69  ........z+NodeLi
-00000e60: 6b65 5079 4469 6374 2e73 6574 5f63 6869  kePyDict.set_chi
-00000e70: 6c64 2e3c 6c6f 6361 6c73 3e2e 3c67 656e  ld.<locals>.<gen
-00000e80: 6578 7072 3ea9 0172 4d00 0000 e902 0000  expr>..rM.......
-00000e90: 0072 0f00 0000 e909 0000 00da 0674 656e  .r...........ten
-00000ea0: 736f 72e9 0300 0000 da06 7665 6374 6f72  sor.......vector
-00000eb0: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
-00000ec0: 0004 0000 0053 0000 0073 1400 0000 6700  .....S...s....g.
-00000ed0: 7c00 5d06 7d01 7400 7c01 8301 9102 7102  |.].}.t.|.....q.
-00000ee0: 5300 7221 0000 0029 0172 3300 0000 2902  S.r!...).r3...).
-00000ef0: 7235 0000 00da 0873 6571 7565 6e63 6572  r5.....sequencer
-00000f00: 2100 0000 7221 0000 0072 2200 0000 da0a  !...r!...r".....
-00000f10: 3c6c 6973 7463 6f6d 703e 9600 0000 7302  <listcomp>....s.
-00000f20: 0000 0014 007a 2c4e 6f64 654c 696b 6550  .....z,NodeLikeP
-00000f30: 7944 6963 742e 7365 745f 6368 696c 642e  yDict.set_child.
-00000f40: 3c6c 6f63 616c 733e 2e3c 6c69 7374 636f  <locals>.<listco
-00000f50: 6d70 3eda 0673 6361 6c61 7229 0272 4d00  mp>..scalar).rM.
-00000f60: 0000 da05 6474 7970 6529 1272 3100 0000  ....dtype).r1...
-00000f70: 7251 0000 00da 0361 6c6c da02 6e70 da05  rQ.....all..np..
-00000f80: 6172 7261 7972 4200 0000 724f 0000 0072  arrayrB...rO...r
-00000f90: 0500 0000 7254 0000 0072 3200 0000 7233  ....rT...r2...r3
-00000fa0: 0000 00da 076e 6461 7272 6179 da05 7368  .....ndarray..sh
-00000fb0: 6170 65da 046e 6469 6dda 0674 6f6c 6973  ape..ndim..tolis
-00000fc0: 7472 5700 0000 7241 0000 0072 5600 0000  trW...rA...rV...
-00000fd0: 2906 7244 0000 0072 3600 0000 da05 6368  ).rD...r6.....ch
-00000fe0: 696c 6472 6b00 0000 726c 0000 0072 6600  ildrk...rl...rf.
-00000ff0: 0000 7221 0000 0072 2100 0000 7222 0000  ..r!...r!...r"..
-00001000: 0072 5000 0000 7a00 0000 734a 0000 0008  .rP...z...sJ....
-00001010: 0202 ff02 0202 fe0c 0302 fd06 0402 fc14  ................
-00001020: 0502 fb0a 0714 0202 010a 010e 010a 010e  ................
-00001030: 010c 0106 0106 0108 0104 0108 010c 0106  ................
-00001040: 010c 0106 0104 0210 0108 0106 0104 0210  ................
-00001050: 010a 0102 010c 0210 017a 184e 6f64 654c  .........z.NodeL
-00001060: 696b 6550 7944 6963 742e 7365 745f 6368  ikePyDict.set_ch
-00001070: 696c 6463 0400 0000 0000 0000 0000 0000  ildc............
-00001080: 0400 0000 0500 0000 4300 0000 7330 0000  ........C...s0..
-00001090: 0074 007c 0274 0183 0273 097c 0364 0075  .t.|.t...s.|.d.u
-000010a0: 0172 1074 027c 027c 017c 0364 018d 037d  .r.t.|.|.|.d...}
-000010b0: 027c 00a0 037c 017c 02a1 0201 0064 0053  .|...|.|.....d.S
-000010c0: 0029 024e 2901 7258 0000 0029 0472 3100  .).N).rX...).r1.
-000010d0: 0000 7205 0000 00da 0556 616c 7565 7256  ..r......ValuerV
-000010e0: 0000 0029 0472 4400 0000 724d 0000 0072  ...).rD...rM...r
-000010f0: 3700 0000 7258 0000 0072 2100 0000 7221  7...rX...r!...r!
-00001100: 0000 0072 2200 0000 7253 0000 00a2 0000  ...r"...rS......
-00001110: 0073 0600 0000 1201 0e01 1001 7a18 4e6f  .s..........z.No
-00001120: 6465 4c69 6b65 5079 4469 6374 2e73 6574  deLikePyDict.set
-00001130: 5f76 616c 7565 6303 0000 0000 0000 0000  _valuec.........
-00001140: 0000 0003 0000 0001 0000 0043 0000 0073  ...........C...s
-00001150: 0400 0000 6401 5300 2902 7a0b 5365 7420  ....d.S.).z.Set 
-00001160: 616e 2069 7465 6d4e 7221 0000 00a9 0372  an itemNr!.....r
-00001170: 4400 0000 7236 0000 0072 3700 0000 7221  D...r6...r7...r!
-00001180: 0000 0072 2100 0000 7222 0000 0072 5600  ...r!...r"...rV.
-00001190: 0000 a700 0000 7302 0000 0004 007a 184e  ......s......z.N
-000011a0: 6f64 654c 696b 6550 7944 6963 742e 5f73  odeLikePyDict._s
-000011b0: 6574 5f69 7465 6d29 034e 464e 7230 0000  et_item).NFNr0..
-000011c0: 0029 0a72 4700 0000 7248 0000 0072 4900  .).rG...rH...rI.
-000011d0: 0000 7254 0000 0072 0700 0000 7255 0000  ..rT...r....rU..
-000011e0: 0072 5000 0000 7253 0000 0072 0300 0000  .rP...rS...r....
-000011f0: 7256 0000 0072 2100 0000 7221 0000 0072  rV...r!...r!...r
-00001200: 2100 0000 7222 0000 0072 4a00 0000 5500  !...r"...rJ...U.
-00001210: 0000 731e 0000 0008 0002 0402 0102 0104  ..s.............
-00001220: fb02 0202 fe06 0302 fd06 050a fb08 240a  ..............$.
-00001230: 2802 050e 0172 4a00 0000 6300 0000 0000  (....rJ...c.....
-00001240: 0000 0000 0000 0000 0000 0003 0000 0040  ...............@
-00001250: 0000 0073 4600 0000 6500 5a01 6400 5a02  ...sF...e.Z.d.Z.
-00001260: 6410 6402 6403 8401 5a03 6404 6405 8400  d.d.d...Z.d.d...
-00001270: 5a04 6406 6407 8400 5a05 6408 6409 8400  Z.d.d...Z.d.d...
-00001280: 5a06 640a 640b 8400 5a07 640c 640d 8400  Z.d.d...Z.d.d...
-00001290: 5a08 640e 640f 8400 5a09 6401 5300 2911  Z.d.d...Z.d.S.).
-000012a0: da0d 466f 616d 496e 7075 7446 696c 654e  ..FoamInputFileN
-000012b0: 6305 0000 0000 0000 0000 0000 0005 0000  c...............
-000012c0: 0002 0000 0043 0000 0073 2e00 0000 7c01  .....C...s....|.
-000012d0: 7c00 5f00 7c02 6400 7500 7209 6900 7d02  |._.|.d.u.r.i.}.
-000012e0: 7c02 7c00 5f01 7c03 7c00 5f02 7c04 7c00  |.|._.|.|._.|.|.
-000012f0: 5f03 6400 7c00 5f04 6400 5300 7230 0000  _.d.|._.d.S.r0..
-00001300: 0029 05da 0469 6e66 6fda 0863 6869 6c64  .)...info..child
-00001310: 7265 6eda 0668 6561 6465 7272 4c00 0000  ren..headerrL...
-00001320: da04 7061 7468 2905 7244 0000 0072 7200  ..path).rD...rr.
-00001330: 0000 7273 0000 0072 7400 0000 724c 0000  ..rs...rt...rL..
-00001340: 0072 2100 0000 7221 0000 0072 2200 0000  .r!...r!...r"...
-00001350: da08 5f5f 696e 6974 5f5f ad00 0000 730e  ..__init__....s.
-00001360: 0000 0006 0108 0104 0106 0106 0106 010a  ................
-00001370: 017a 1646 6f61 6d49 6e70 7574 4669 6c65  .z.FoamInputFile
-00001380: 2e5f 5f69 6e69 745f 5f63 0100 0000 0000  .__init__c......
-00001390: 0000 0000 0000 0200 0000 0500 0000 4300  ..............C.
-000013a0: 0000 7342 0000 0064 0167 017d 017c 006a  ..sB...d.g.}.|.j
-000013b0: 0064 0075 0172 127c 01a0 0164 027c 006a  .d.u.r.|...d.|.j
-000013c0: 009b 0064 039d 03a1 0101 007c 01a0 0164  ...d.......|...d
-000013d0: 047c 006a 029b 0064 059d 03a1 0101 0064  .|.j...d.......d
-000013e0: 06a0 037c 01a1 0153 0029 074e 7a0b 496e  ...|...S.).Nz.In
-000013f0: 7075 7446 696c 6528 0a7a 0569 6e66 6f3d  putFile(.z.info=
-00001400: 7a02 2c0a 7a09 6368 696c 6472 656e 3d7a  z.,.z.children=z
-00001410: 020a 2972 1000 0000 2904 7272 0000 0072  ..)r....).rr...r
-00001420: 2700 0000 7273 0000 0072 2800 0000 2902  '...rs...r(...).
-00001430: 7244 0000 00da 0374 6d70 7221 0000 0072  rD.....tmpr!...r
-00001440: 2100 0000 7222 0000 00da 085f 5f72 6570  !...r".....__rep
-00001450: 725f 5fb6 0000 0073 0a00 0000 0601 0a01  r__....s........
-00001460: 1401 1401 0a01 7a16 466f 616d 496e 7075  ......z.FoamInpu
-00001470: 7446 696c 652e 5f5f 7265 7072 5f5f 6301  tFile.__repr__c.
-00001480: 0000 0000 0000 0000 0000 000b 0000 0008  ................
-00001490: 0000 0043 0000 0073 a201 0000 6700 7d01  ...C...s....g.}.
-000014a0: 7c00 6a00 6400 7501 7236 6401 6701 7d02  |.j.d.u.r6d.g.}.
-000014b0: 7c00 6a00 a001 a100 4400 5d19 5c02 7d03  |.j.....D.].\.}.
-000014c0: 7d04 6402 7402 7c03 8301 1800 6403 1400  }.d.t.|.....d...
-000014d0: 7d05 7c02 a003 6404 7c03 9b00 7c05 9b00  }.|...d.|...|...
-000014e0: 7c04 9b00 6405 9d05 a101 0100 710f 7c02  |...d.......q.|.
-000014f0: a003 6406 a101 0100 7c01 a003 6407 a004  ..d.....|...d...
-00001500: 7c02 a101 a101 0100 7405 7c00 6a06 6408  |.......t.|.j.d.
-00001510: 6409 8d02 7d06 7c00 6a06 a001 a100 4400  d...}.|.j.....D.
-00001520: 5d71 5c02 7d03 7d04 7407 7c04 640a 8302  ]q\.}.}.t.|.d...
-00001530: 725d 7c04 a008 a100 7d07 7c03 6400 7500  r]|.....}.|.d.u.
-00001540: 725c 7409 7c04 740a 8302 725c 7c07 6405  r\t.|.t...r\|.d.
-00001550: 3700 7d07 6e2f 7c04 6400 7500 7265 7c03  7.}.n/|.d.u.re|.
-00001560: 9b00 7d07 6e27 7407 7c04 640b 8302 726f  ..}.n't.|.d...ro
-00001570: 7c04 a00b a100 7d08 6e02 7c04 7d08 7c08  |.....}.n.|.}.|.
-00001580: 640c 6b02 7278 640c 7d05 6e0b 740c 640d  d.k.rxd.}.n.t.d.
-00001590: 7c06 7402 7c03 8301 1800 8302 6403 1400  |.t.|.......d...
-000015a0: 7d05 7c03 9b00 7c05 9b00 7c08 9b00 6405  }.|...|...|...d.
-000015b0: 9d04 7d07 7c00 6a0d 6400 7501 72ae 7c03  ..}.|.j.d.u.r.|.
-000015c0: 7c00 6a0d 7600 72ae 7c00 6a0d 7c03 1900  |.j.v.r.|.j.|...
-000015d0: 7d09 7409 7c09 740e 8302 72ae 640e 7c09  }.t.|.t...r.d.|.
-000015e0: a00f 6407 640f a102 1700 7d09 7c09 6407  ..d.d.....}.|.d.
-000015f0: 1700 7c07 1700 7d07 7c01 a003 7c07 a101  ..|...}.|...|...
-00001600: 0100 7142 6410 a004 7c01 a101 7d0a 7c00  ..qBd...|...}.|.
-00001610: 6a10 6400 7501 72c5 7c00 6a10 6407 1700  j.d.u.r.|.j.d...
-00001620: 7c0a 1700 7d0a 7c0a 6411 1900 6407 6b03  |...}.|.d...d.k.
-00001630: 72cf 7c0a 6407 3700 7d0a 7c0a 5300 2912  r.|.d.7.}.|.S.).
-00001640: 4e7a 0a46 6f61 6d46 696c 650a 7be9 0c00  Nz.FoamFile.{...
-00001650: 0000 fa01 20fa 0420 2020 20fa 013b da01  .... ..    ..;..
-00001660: 7dda 010a e90e 0000 0029 0172 3f00 0000  }........).r?...
-00001670: da04 6475 6d70 da17 6475 6d70 5f77 6974  ..dump..dump_wit
-00001680: 686f 7574 5f61 7373 6967 6e6d 656e 7472  hout_assignmentr
-00001690: 1000 0000 725e 0000 007a 032f 2f20 7a04  ....r^...z.// z.
-000016a0: 0a2f 2f20 7a02 0a0a 7214 0000 0029 1172  .// z...r....).r
-000016b0: 7200 0000 723c 0000 0072 3400 0000 7227  r...r<...r4...r'
-000016c0: 0000 0072 2800 0000 7240 0000 0072 7300  ...r(...r@...rs.
-000016d0: 0000 da07 6861 7361 7474 7272 8000 0000  ....hasattrr....
-000016e0: 7231 0000 0072 3300 0000 7281 0000 0072  r1...r3...r....r
-000016f0: 3b00 0000 724c 0000 0072 4f00 0000 da07  ;...rL...rO.....
-00001700: 7265 706c 6163 6572 7400 0000 290b 7244  replacert...).rD
-00001710: 0000 0072 7700 0000 5a04 746d 7031 7236  ...rw...Z.tmp1r6
-00001720: 0000 00da 046e 6f64 6572 0a00 0000 da0a  .....noder......
-00001730: 6e75 6d5f 7370 6163 6573 da09 636f 6465  num_spaces..code
-00001740: 5f6e 6f64 655a 0b6e 6f64 655f 6475 6d70  _nodeZ.node_dump
-00001750: 6564 da07 636f 6d6d 656e 7472 1e00 0000  ed..commentr....
-00001760: 7221 0000 0072 2100 0000 7222 0000 0072  r!...r!...r"...r
-00001770: 8000 0000 bd00 0000 7348 0000 0004 010a  ........sH......
-00001780: 0106 0112 0110 011c 010a 0110 010e 0212  ................
-00001790: 010a 0108 0112 0208 0102 8008 0108 010a  ................
-000017a0: 020a 0104 0208 0106 0116 0212 0114 010a  ................
-000017b0: 010a 0110 010c 010c 010a 010a 010e 010c  ................
-000017c0: 0108 0104 017a 1246 6f61 6d49 6e70 7574  .....z.FoamInput
-000017d0: 4669 6c65 2e64 756d 7063 0100 0000 0000  File.dumpc......
-000017e0: 0000 0000 0000 0200 0000 0800 0000 4300  ..............C.
-000017f0: 0000 7352 0000 007c 006a 0064 0075 0072  ..sR...|.j.d.u.r
-00001800: 0974 0164 0183 0182 0174 027c 006a 0064  .t.d.....t.|.j.d
-00001810: 0283 028f 107d 017c 01a0 037c 00a0 04a1  .....}.|...|....
-00001820: 00a1 0101 0057 0064 0004 0004 0083 0301  .....W.d........
-00001830: 0064 0053 0031 0073 2277 0101 0001 0001  .d.S.1.s"w......
-00001840: 0059 0001 0064 0053 0029 034e 7a11 7365  .Y...d.S.).Nz.se
-00001850: 6c66 2e70 6174 6820 6973 204e 6f6e 65da  lf.path is None.
-00001860: 0177 2905 7275 0000 0072 3d00 0000 da04  .w).ru...r=.....
-00001870: 6f70 656e da05 7772 6974 6572 8000 0000  open..writer....
-00001880: 2902 7244 0000 00da 0466 696c 6572 2100  ).rD.....filer!.
-00001890: 0000 7221 0000 0072 2200 0000 da09 6f76  ..r!...r".....ov
-000018a0: 6572 7772 6974 65e7 0000 0073 0a00 0000  erwrite....s....
-000018b0: 0a01 0801 0e01 1001 22ff 7a17 466f 616d  ........".z.Foam
-000018c0: 496e 7075 7446 696c 652e 6f76 6572 7772  InputFile.overwr
-000018d0: 6974 6563 0300 0000 0000 0000 0000 0000  itec............
-000018e0: 0300 0000 0300 0000 4300 0000 f30e 0000  ........C.......
-000018f0: 007c 027c 006a 007c 013c 0064 0053 0072  .|.|.j.|.<.d.S.r
-00001900: 3000 0000 a901 7273 0000 0072 7000 0000  0.....rs...rp...
-00001910: 7221 0000 0072 2100 0000 7222 0000 0072  r!...r!...r"...r
-00001920: 5600 0000 ed00 0000 f302 0000 000e 017a  V..............z
-00001930: 1746 6f61 6d49 6e70 7574 4669 6c65 2e5f  .FoamInputFile._
-00001940: 7365 745f 6974 656d 6303 0000 0000 0000  set_itemc.......
-00001950: 0000 0000 0003 0000 0003 0000 0043 0000  .............C..
-00001960: 0072 8d00 0000 7230 0000 0072 8e00 0000  .r....r0...r....
-00001970: 2903 7244 0000 0072 3600 0000 da04 6974  ).rD...r6.....it
-00001980: 656d 7221 0000 0072 2100 0000 7222 0000  emr!...r!...r"..
-00001990: 00da 0b5f 5f73 6574 6974 656d 5f5f f000  ...__setitem__..
-000019a0: 0000 728f 0000 007a 1946 6f61 6d49 6e70  ..r....z.FoamInp
-000019b0: 7574 4669 6c65 2e5f 5f73 6574 6974 656d  utFile.__setitem
-000019c0: 5f5f 6302 0000 0000 0000 0000 0000 0002  __c.............
-000019d0: 0000 0002 0000 0043 0000 0073 0a00 0000  .......C...s....
-000019e0: 7c00 6a00 7c01 1900 5300 7230 0000 0072  |.j.|...S.r0...r
-000019f0: 8e00 0000 2902 7244 0000 0072 3600 0000  ....).rD...r6...
-00001a00: 7221 0000 0072 2100 0000 7222 0000 00da  r!...r!...r"....
-00001a10: 0b5f 5f67 6574 6974 656d 5f5f f300 0000  .__getitem__....
-00001a20: f302 0000 000a 017a 1946 6f61 6d49 6e70  .......z.FoamInp
-00001a30: 7574 4669 6c65 2e5f 5f67 6574 6974 656d  utFile.__getitem
-00001a40: 5f5f a903 4e4e 4e29 0a72 4700 0000 7248  __..NNN).rG...rH
-00001a50: 0000 0072 4900 0000 7276 0000 0072 7800  ...rI...rv...rx.
-00001a60: 0000 7280 0000 0072 8c00 0000 7256 0000  ..r....r....rV..
-00001a70: 0072 9100 0000 7292 0000 0072 2100 0000  .r....r....r!...
-00001a80: 7221 0000 0072 2100 0000 7222 0000 0072  r!...r!...r"...r
-00001a90: 7100 0000 ac00 0000 7310 0000 0008 000a  q.......s.......
-00001aa0: 0108 0908 0708 2a08 0608 030c 0372 7100  ......*......rq.
-00001ab0: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
-00001ac0: 0000 0003 0000 0040 0000 0073 2800 0000  .......@...s(...
-00001ad0: 6500 5a01 6400 5a02 5500 6503 6504 6401  e.Z.d.Z.U.e.e.d.
-00001ae0: 3c00 6505 6504 6402 3c00 6407 6404 6405  <.e.e.d.<.d.d.d.
-00001af0: 8401 5a06 6406 5300 2908 da0a 4173 7369  ..Z.d.S.)...Assi
-00001b00: 676e 6d65 6e74 724d 0000 0072 3700 0000  gnmentrM...r7...
-00001b10: 7201 0000 0063 0200 0000 0000 0000 0000  r....c..........
-00001b20: 0000 0200 0000 0500 0000 4300 0000 7334  ..........C...s4
-00001b30: 0000 0074 007c 006a 0164 0183 0272 0c7c  ...t.|.j.d...r.|
-00001b40: 006a 01a0 027c 01a1 0153 007c 0164 0214  .j...|...S.|.d..
-00001b50: 007c 006a 039b 0064 037c 006a 019b 0064  .|.j...d.|.j...d
-00001b60: 049d 0417 0053 00a9 054e 7280 0000 0072  .....S...Nr....r
-00001b70: 7a00 0000 fa02 2020 727c 0000 0029 0472  z.....  r|...).r
-00001b80: 8200 0000 7237 0000 0072 8000 0000 724d  ....r7...r....rM
-00001b90: 0000 00a9 0272 4400 0000 da06 696e 6465  .....rD.....inde
-00001ba0: 6e74 7221 0000 0072 2100 0000 7222 0000  ntr!...r!...r"..
-00001bb0: 0072 8000 0000 fc00 0000 7306 0000 000c  .r........s.....
-00001bc0: 010c 011c 027a 0f41 7373 6967 6e6d 656e  .....z.Assignmen
-00001bd0: 742e 6475 6d70 4ea9 0172 0100 0000 2907  t.dumpN..r....).
-00001be0: 7247 0000 0072 4800 0000 7249 0000 0072  rG...rH...rI...r
-00001bf0: 4f00 0000 da0f 5f5f 616e 6e6f 7461 7469  O.....__annotati
-00001c00: 6f6e 735f 5fda 066f 626a 6563 7472 8000  ons__..objectr..
-00001c10: 0000 7221 0000 0072 2100 0000 7221 0000  ..r!...r!...r!..
-00001c20: 0072 2200 0000 7295 0000 00f7 0000 0073  .r"...r........s
-00001c30: 0800 0000 0a00 0802 0801 0e02 7295 0000  ............r...
-00001c40: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
-00001c50: 0000 0300 0000 0000 0000 7326 0000 0065  ..........s&...e
-00001c60: 005a 0164 005a 0287 0066 0164 0164 0284  .Z.d.Z...f.d.d..
-00001c70: 085a 0364 0664 0464 0584 015a 0487 0004  .Z.d.d.d...Z....
-00001c80: 005a 0553 0029 07da 1256 6172 6961 626c  .Z.S.)...Variabl
-00001c90: 6541 7373 6967 6e6d 656e 7463 0100 0000  eAssignmentc....
-00001ca0: 0000 0000 0000 0000 0200 0000 0200 0000  ................
-00001cb0: 0300 0000 730e 0000 0074 0083 00a0 01a1  ....s....t......
-00001cc0: 007d 017c 0153 0072 3000 0000 a902 da05  .}.|.S.r0.......
-00001cd0: 7375 7065 7272 7800 0000 2902 7244 0000  superrx...).rD..
-00001ce0: 0072 0a00 0000 a901 da09 5f5f 636c 6173  .r........__clas
-00001cf0: 735f 5f72 2100 0000 7222 0000 0072 7800  s__r!...r"...rx.
-00001d00: 0000 0401 0000 7304 0000 000a 0104 017a  ......s........z
-00001d10: 1b56 6172 6961 626c 6541 7373 6967 6e6d  .VariableAssignm
-00001d20: 656e 742e 5f5f 7265 7072 5f5f 7201 0000  ent.__repr__r...
-00001d30: 0063 0200 0000 0000 0000 0000 0000 0200  .c..............
-00001d40: 0000 0600 0000 4300 0000 734a 0000 0074  ......C...sJ...t
-00001d50: 007c 006a 0164 0183 0272 177c 0164 0214  .|.j.d...r.|.d..
-00001d60: 007c 006a 029b 0064 037c 006a 01a0 037c  .|.j...d.|.j...|
-00001d70: 01a1 019b 0064 049d 0417 0053 007c 0164  .....d.....S.|.d
-00001d80: 0214 007c 006a 029b 0064 037c 006a 019b  ...|.j...d.|.j..
-00001d90: 0064 049d 0417 0053 0072 9600 0000 2904  .d.....S.r....).
-00001da0: 7282 0000 0072 3700 0000 724d 0000 0072  r....r7...rM...r
-00001db0: 8000 0000 7298 0000 0072 2100 0000 7221  ....r....r!...r!
-00001dc0: 0000 0072 2200 0000 7280 0000 0008 0100  ...r"...r.......
-00001dd0: 0073 0600 0000 0c01 2201 1c02 7a17 5661  .s......"...z.Va
-00001de0: 7269 6162 6c65 4173 7369 676e 6d65 6e74  riableAssignment
-00001df0: 2e64 756d 7072 9a00 0000 2906 7247 0000  .dumpr....).rG..
-00001e00: 0072 4800 0000 7249 0000 0072 7800 0000  .rH...rI...rx...
-00001e10: 7280 0000 00da 0d5f 5f63 6c61 7373 6365  r......__classce
-00001e20: 6c6c 5f5f 7221 0000 0072 2100 0000 72a0  ll__r!...r!...r.
-00001e30: 0000 0072 2200 0000 729d 0000 0003 0100  ...r"...r.......
-00001e40: 0073 0600 0000 0800 0c01 1204 729d 0000  .s..........r...
-00001e50: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
-00001e60: 0000 0300 0000 4000 0000 f328 0000 0065  ......@....(...e
-00001e70: 005a 0164 005a 0264 0964 0264 0384 015a  .Z.d.Z.d.d.d...Z
-00001e80: 0364 0464 0584 005a 0464 0a64 0764 0884  .d.d...Z.d.d.d..
-00001e90: 015a 0564 0153 0029 0b72 6f00 0000 4e63  .Z.d.S.).ro...Nc
-00001ea0: 0400 0000 0000 0000 0000 0000 0400 0000  ................
-00001eb0: 0400 0000 4300 0000 732c 0000 007c 017c  ....C...s,...|.|
-00001ec0: 005f 007c 027c 005f 0174 027c 0374 0374  ._.|.|._.t.|.t.t
-00001ed0: 0466 0283 0272 1174 057c 0383 017d 037c  .f...r.t.|...}.|
-00001ee0: 037c 005f 0664 0053 0072 3000 0000 2907  .|._.d.S.r0...).
-00001ef0: 7237 0000 0072 4d00 0000 7231 0000 0072  r7...rM...r1...r
-00001f00: 5100 0000 da05 7475 706c 6572 2e00 0000  Q.....tupler....
-00001f10: 7258 0000 0029 0472 4400 0000 7237 0000  rX...).rD...r7..
-00001f20: 0072 4d00 0000 7258 0000 0072 2100 0000  .rM...rX...r!...
-00001f30: 7221 0000 0072 2200 0000 7276 0000 0011  r!...r"...rv....
-00001f40: 0100 0073 0a00 0000 0601 0601 0e01 0801  ...s............
-00001f50: 0a01 7a0e 5661 6c75 652e 5f5f 696e 6974  ..z.Value.__init
-00001f60: 5f5f 6301 0000 0000 0000 0000 0000 0001  __c.............
-00001f70: 0000 0007 0000 0043 0000 0073 9400 0000  .......C...s....
-00001f80: 7c00 6a00 6400 7501 7219 7c00 6a01 6400  |.j.d.u.r.|.j.d.
-00001f90: 7501 7219 6401 7c00 6a02 9b00 6402 7c00  u.r.d.|.j...d.|.
-00001fa0: 6a01 9b00 6403 7c00 6a00 9b00 6404 9d07  j...d.|.j...d...
-00001fb0: 5300 7c00 6a00 6400 7500 722e 7c00 6a01  S.|.j.d.u.r.|.j.
-00001fc0: 6400 7501 722e 6401 7c00 6a02 9b00 6402  d.u.r.d.|.j...d.
-00001fd0: 7c00 6a01 9b00 6404 9d05 5300 7c00 6a00  |.j...d...S.|.j.
-00001fe0: 6400 7501 7243 7c00 6a01 6400 7500 7243  d.u.rC|.j.d.u.rC
-00001ff0: 6401 7c00 6a02 9b00 6405 7c00 6a00 9b00  d.|.j...d.|.j...
-00002000: 6404 9d05 5300 6401 7c00 6a02 9b00 6406  d...S.d.|.j...d.
-00002010: 9d03 5300 2907 4e7a 0656 616c 7565 287a  ..S.).Nz.Value(z
-00002020: 082c 206e 616d 653d 227a 0e22 2c20 6469  ., name="z.", di
-00002030: 6d65 6e73 696f 6e3d 227a 0222 297a 0d2c  mension="z.")z.,
-00002040: 2064 696d 656e 7369 6f6e 3d22 fa01 2929   dimension="..))
-00002050: 0372 5800 0000 724d 0000 0072 3700 0000  .rX...rM...r7...
-00002060: a901 7244 0000 0072 2100 0000 7221 0000  ..rD...r!...r!..
-00002070: 0072 2200 0000 7278 0000 0018 0100 0073  .r"...rx.......s
-00002080: 0e00 0000 1401 1e01 1401 1601 1401 1601  ................
-00002090: 0e02 7a0e 5661 6c75 652e 5f5f 7265 7072  ..z.Value.__repr
-000020a0: 5f5f 7201 0000 0063 0200 0000 0000 0000  __r....c........
-000020b0: 0000 0000 0500 0000 0500 0000 4300 0000  ............C...
-000020c0: 73ce 0000 007c 006a 0064 0075 0172 1474  s....|.j.d.u.r.t
-000020d0: 017c 006a 0083 017d 0264 01a0 0264 0264  .|.j...}.d...d.d
-000020e0: 0384 007c 0244 0083 01a1 017d 0374 037c  ...|.D.....}.t.|
-000020f0: 006a 0474 0583 0272 2674 067c 006a 0464  .j.t...r&t.|.j.d
-00002100: 0483 0272 267c 006a 04a0 07a1 007d 046e  ...r&|.j.....}.n
-00002110: 0574 087c 006a 0483 017d 047c 006a 0064  .t.|.j...}.|.j.d
-00002120: 0075 0172 407c 006a 0964 0075 0172 407c  .u.r@|.j.d.u.r@|
-00002130: 006a 099b 0064 057c 039b 0064 067c 049b  .j...d.|...d.|..
-00002140: 009d 0553 007c 006a 0064 0075 0072 527c  ...S.|.j.d.u.rR|
-00002150: 006a 0964 0075 0172 527c 006a 099b 0064  .j.d.u.rR|.j...d
-00002160: 017c 049b 009d 0353 007c 006a 0064 0075  .|.....S.|.j.d.u
-00002170: 0172 647c 006a 0964 0075 0072 6464 077c  .rd|.j.d.u.rdd.|
-00002180: 039b 0064 067c 049b 009d 0453 007c 049b  ...d.|.....S.|..
-00002190: 0053 0029 084e 727a 0000 0063 0100 0000  .S.).Nrz...c....
-000021a0: 0000 0000 0000 0000 0200 0000 0300 0000  ................
-000021b0: 7300 0000 f318 0000 0081 007c 005d 077d  s..........|.].}
-000021c0: 0174 007c 0183 0156 0001 0071 0264 0053  .t.|...V...q.d.S
-000021d0: 0072 3000 0000 a901 724f 0000 00a9 0272  .r0.....rO.....r
-000021e0: 3500 0000 da06 6e75 6d62 6572 7221 0000  5.....numberr!..
-000021f0: 0072 2100 0000 7222 0000 0072 3800 0000  .r!...r"...r8...
-00002200: 2501 0000 f304 0000 0002 8016 007a 3056  %............z0V
-00002210: 616c 7565 2e64 756d 705f 7769 7468 6f75  alue.dump_withou
-00002220: 745f 6173 7369 676e 6d65 6e74 2e3c 6c6f  t_assignment.<lo
-00002230: 6361 6c73 3e2e 3c67 656e 6578 7072 3e72  cals>.<genexpr>r
-00002240: 8000 0000 7a02 205b 7a02 5d20 fa01 5b29  ....z. [z.] ..[)
-00002250: 0a72 5800 0000 7223 0000 0072 2800 0000  .rX...r#...r(...
-00002260: 7231 0000 0072 3700 0000 7241 0000 0072  r1...r7...rA...r
-00002270: 8200 0000 7280 0000 0072 4f00 0000 724d  ....r....rO...rM
-00002280: 0000 0029 0572 4400 0000 7299 0000 005a  ...).rD...r....Z
-00002290: 0e64 696d 656e 7369 6f6e 5f6c 6973 745a  .dimension_listZ
-000022a0: 1064 696d 656e 7369 6f6e 5f64 756d 7065  .dimension_dumpe
-000022b0: 645a 0c76 616c 7565 5f64 756d 7065 6472  dZ.value_dumpedr
-000022c0: 2100 0000 7221 0000 0072 2200 0000 7281  !...r!...r"...r.
-000022d0: 0000 0022 0100 0073 1a00 0000 0a01 0a01  ..."...s........
-000022e0: 1401 1802 0c01 0a02 1402 1601 1401 1001  ................
-000022f0: 1401 1001 0602 7a1d 5661 6c75 652e 6475  ......z.Value.du
-00002300: 6d70 5f77 6974 686f 7574 5f61 7373 6967  mp_without_assig
-00002310: 6e6d 656e 7429 024e 4e72 9a00 0000 2906  nment).NNr....).
-00002320: 7247 0000 0072 4800 0000 7249 0000 0072  rG...rH...rI...r
-00002330: 7600 0000 7278 0000 0072 8100 0000 7221  v...rx...r....r!
-00002340: 0000 0072 2100 0000 7221 0000 0072 2200  ...r!...r!...r".
-00002350: 0000 726f 0000 000f 0100 0073 0800 0000  ..ro.......s....
-00002360: 0800 0a02 0807 0e0a 726f 0000 0063 0000  ........ro...c..
-00002370: 0000 0000 0000 0000 0000 0000 0000 0300  ................
-00002380: 0000 0000 0000 732e 0000 0065 005a 0164  ......s....e.Z.d
-00002390: 005a 0287 0066 0164 0164 0284 085a 0364  .Z...f.d.d...Z.d
-000023a0: 0364 0484 005a 0464 0864 0664 0784 015a  .d...Z.d.d.d...Z
-000023b0: 0587 0004 005a 0653 0029 09da 0c44 696d  .....Z.S.)...Dim
-000023c0: 656e 7369 6f6e 5365 7463 0200 0000 0000  ensionSetc......
-000023d0: 0000 0000 0000 0200 0000 0300 0000 0300  ................
-000023e0: 0000 732a 0000 0074 0064 0164 0284 007c  ..s*...t.d.d...|
-000023f0: 0144 0083 0183 0173 0d74 0164 0383 0182  .D.....s.t.d....
-00002400: 0174 0283 00a0 037c 01a1 0101 0064 0053  .t.....|.....d.S
-00002410: 0029 044e 6301 0000 0000 0000 0000 0000  .).Nc...........
-00002420: 0002 0000 0004 0000 0073 0000 0072 5a00  .........s...rZ.
-00002430: 0000 7230 0000 0029 0272 3100 0000 721a  ..r0...).r1...r.
-00002440: 0000 0029 0272 3500 0000 da04 656c 656d  ...).r5.....elem
-00002450: 7221 0000 0072 2100 0000 7222 0000 0072  r!...r!...r"...r
-00002460: 3800 0000 3801 0000 725c 0000 007a 2844  8...8...r\...z(D
-00002470: 696d 656e 7369 6f6e 5365 742e 5f5f 696e  imensionSet.__in
-00002480: 6974 5f5f 2e3c 6c6f 6361 6c73 3e2e 3c67  it__.<locals>.<g
-00002490: 656e 6578 7072 3e7a 1342 6164 207b 666f  enexpr>z.Bad {fo
-000024a0: 616d 5f75 6e69 7473 203d 207d 2904 7267  am_units = }).rg
-000024b0: 0000 0072 3d00 0000 729f 0000 0072 7600  ...r=...r....rv.
-000024c0: 0000 2902 7244 0000 0072 2a00 0000 72a0  ..).rD...r*...r.
-000024d0: 0000 0072 2100 0000 7222 0000 0072 7600  ...r!...r"...rv.
-000024e0: 0000 3701 0000 7306 0000 0012 0108 0110  ..7...s.........
-000024f0: 017a 1544 696d 656e 7369 6f6e 5365 742e  .z.DimensionSet.
-00002500: 5f5f 696e 6974 5f5f 6301 0000 0000 0000  __init__c.......
-00002510: 0000 0000 0001 0000 0002 0000 0043 0000  .............C..
-00002520: 0073 0800 0000 7400 7c00 8301 5300 7230  .s....t.|...S.r0
-00002530: 0000 0029 0172 2e00 0000 72a6 0000 0072  ...).r....r....r
-00002540: 2100 0000 7221 0000 0072 2200 0000 7278  !...r!...r"...rx
-00002550: 0000 003c 0100 00f3 0200 0000 0801 7a15  ...<..........z.
-00002560: 4469 6d65 6e73 696f 6e53 6574 2e5f 5f72  DimensionSet.__r
-00002570: 6570 725f 5f72 0100 0000 6302 0000 0000  epr__r....c.....
-00002580: 0000 0000 0000 0002 0000 0005 0000 0043  ...............C
-00002590: 0000 0073 1c00 0000 6401 6402 a000 6403  ...s....d.d...d.
-000025a0: 6404 8400 7c00 4400 8301 a101 1700 6405  d...|.D.......d.
-000025b0: 1700 5300 2906 4e72 ac00 0000 727a 0000  ..S.).Nr....rz..
-000025c0: 0063 0100 0000 0000 0000 0000 0000 0200  .c..............
-000025d0: 0000 0300 0000 7300 0000 72a7 0000 0072  ......s...r....r
-000025e0: 3000 0000 72a8 0000 0072 a900 0000 7221  0...r....r....r!
-000025f0: 0000 0072 2100 0000 7222 0000 0072 3800  ...r!...r"...r8.
-00002600: 0000 4001 0000 72ab 0000 007a 3744 696d  ..@...r....z7Dim
-00002610: 656e 7369 6f6e 5365 742e 6475 6d70 5f77  ensionSet.dump_w
-00002620: 6974 686f 7574 5f61 7373 6967 6e6d 656e  ithout_assignmen
-00002630: 742e 3c6c 6f63 616c 733e 2e3c 6765 6e65  t.<locals>.<gene
-00002640: 7870 723e fa01 5da9 0172 2800 0000 7298  xpr>..]..r(...r.
-00002650: 0000 0072 2100 0000 7221 0000 0072 2200  ...r!...r!...r".
-00002660: 0000 7281 0000 003f 0100 00f3 0200 0000  ..r....?........
-00002670: 1c01 7a24 4469 6d65 6e73 696f 6e53 6574  ..z$DimensionSet
-00002680: 2e64 756d 705f 7769 7468 6f75 745f 6173  .dump_without_as
-00002690: 7369 676e 6d65 6e74 729a 0000 0029 0772  signmentr....).r
-000026a0: 4700 0000 7248 0000 0072 4900 0000 7276  G...rH...rI...rv
-000026b0: 0000 0072 7800 0000 7281 0000 0072 a200  ...rx...r....r..
-000026c0: 0000 7221 0000 0072 2100 0000 72a0 0000  ..r!...r!...r...
-000026d0: 0072 2200 0000 72ad 0000 0036 0100 0073  .r"...r....6...s
-000026e0: 0800 0000 0800 0c01 0805 1203 72ad 0000  ............r...
-000026f0: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
-00002700: 0000 0400 0000 0000 0000 7344 0000 0065  ..........sD...e
-00002710: 005a 0164 005a 0264 0d87 0066 0164 0264  .Z.d.Z.d...f.d.d
-00002720: 0384 095a 0364 0464 0584 005a 0487 0066  ...Z.d.d...Z...f
-00002730: 0164 0664 0784 085a 0564 0e64 0964 0a84  .d.d...Z.d.d.d..
-00002740: 015a 0664 0b64 0c84 005a 0787 0004 005a  .Z.d.d...Z.....Z
-00002750: 0853 0029 0f72 3200 0000 4e63 0500 0000  .S.).r2...Nc....
-00002760: 0000 0000 0000 0000 0500 0000 0400 0000  ................
-00002770: 0300 0000 7328 0000 007c 027c 005f 007c  ....s(...|.|._.|
-00002780: 037c 005f 017c 047c 005f 0274 0383 006a  .|._.|.|._.t...j
-00002790: 0464 0169 007c 01a4 018e 0101 0064 0053  .d.i.|.......d.S
-000027a0: 0029 024e 7221 0000 0029 05da 055f 6e61  .).Nr!...)..._na
-000027b0: 6d65 da0a 5f64 6972 6563 7469 7665 724c  me.._directiverL
-000027c0: 0000 0072 9f00 0000 7276 0000 0029 0572  ...r....rv...).r
-000027d0: 4400 0000 723e 0000 0072 4d00 0000 da09  D...r>...rM.....
-000027e0: 6469 7265 6374 6976 6572 4c00 0000 72a0  directiverL...r.
-000027f0: 0000 0072 2100 0000 7222 0000 0072 7600  ...r!...r"...rv.
-00002800: 0000 4401 0000 7308 0000 0006 0106 0106  ..D...s.........
-00002810: 0116 017a 0d44 6963 742e 5f5f 696e 6974  ...z.Dict.__init
-00002820: 5f5f 6301 0000 0000 0000 0000 0000 0001  __c.............
-00002830: 0000 0001 0000 0043 0000 00f3 0600 0000  .......C........
-00002840: 7c00 6a00 5300 7230 0000 00a9 0172 b300  |.j.S.r0.....r..
-00002850: 0000 72a6 0000 0072 2100 0000 7221 0000  ..r....r!...r!..
-00002860: 0072 2200 0000 da08 6765 745f 6e61 6d65  .r".....get_name
-00002870: 4a01 0000 f302 0000 0006 017a 0d44 6963  J..........z.Dic
-00002880: 742e 6765 745f 6e61 6d65 6301 0000 0000  t.get_namec.....
-00002890: 0000 0000 0000 0001 0000 0002 0000 0003  ................
-000028a0: 0000 00f3 0a00 0000 7400 8300 a001 a100  ........t.......
-000028b0: 5300 7230 0000 0072 9e00 0000 72a6 0000  S.r0...r....r...
-000028c0: 0072 a000 0000 7221 0000 0072 2200 0000  .r....r!...r"...
-000028d0: 7278 0000 004d 0100 0072 9300 0000 7a0d  rx...M...r....z.
-000028e0: 4469 6374 2e5f 5f72 6570 725f 5f72 0100  Dict.__repr__r..
-000028f0: 0000 6302 0000 0000 0000 0000 0000 000b  ..c.............
-00002900: 0000 0009 0000 0043 0000 0073 5401 0000  .......C...sT...
-00002910: 6700 7d02 7c01 6401 1400 7d03 7c00 6a00  g.}.|.d...}.|.j.
-00002920: 6400 7501 7228 7c03 7c00 6a00 1700 7d04  d.u.r(|.|.j...}.
-00002930: 7c00 6a01 6400 7501 721c 7c04 6402 7c00  |.j.d.u.r.|.d.|.
-00002940: 6a01 1700 3700 7d04 7c02 a002 7c04 6403  j...7.}.|...|.d.
-00002950: 7c03 9b00 9d02 1700 6404 1700 a101 0100  |.......d.......
-00002960: 7403 7c00 8301 7d05 7c00 a004 a100 4400  t.|...}.|.....D.
-00002970: 5d60 5c02 7d06 7d07 7c00 6a05 6400 7501  ]`\.}.}.|.j.d.u.
-00002980: 7253 7c06 7c00 6a05 7600 7253 7c00 6a05  rS|.|.j.v.rS|.j.
-00002990: 7c06 1900 7d08 7406 7c08 7407 8302 7253  |...}.t.|.t...rS
-000029a0: 7c02 a002 6405 7c08 a008 6403 6406 a102  |...d.|...d.d...
-000029b0: 1700 a101 0100 7409 7c07 6407 8302 7263  ......t.|.d...rc
-000029c0: 7c02 a002 7c07 a00a 7c01 6408 1700 a101  |...|...|.d.....
-000029d0: a101 0100 7130 7409 7c07 6409 8302 726d  ....q0t.|.d...rm
-000029e0: 7c07 a00b a100 7d09 6e02 7c07 7d09 7c07  |.....}.n.|.}.|.
-000029f0: 640a 6b02 7276 640a 7d0a 6e0b 740c 640b  d.k.rvd.}.n.t.d.
-00002a00: 7c05 740d 7c06 8301 1800 8302 6401 1400  |.t.|.......d...
-00002a10: 7d0a 7c02 a002 7c03 640c 7c06 9b00 7c0a  }.|...|.d.|...|.
-00002a20: 9b00 7c09 9b00 640d 9d05 1700 a101 0100  ..|...d.........
-00002a30: 7130 7c02 a002 7c03 640e 1700 a101 0100  q0|...|.d.......
-00002a40: 7406 7c00 740e 8302 72a5 7c02 640f 0500  t.|.t...r.|.d...
-00002a50: 1900 640d 3700 0300 3c00 6403 a00f 7c02  ..d.7...<.d...|.
-00002a60: a101 5300 2910 4e72 7a00 0000 7297 0000  ..S.).Nrz...r...
-00002a70: 0072 7e00 0000 da01 7b7a 0720 2020 202f  .r~.....{z.    /
-00002a80: 2f20 7a08 0a20 2020 202f 2f20 7280 0000  / z..    // r...
-00002a90: 0072 3900 0000 7281 0000 0072 1000 0000  .r9...r....r....
-00002aa0: 725e 0000 0072 7b00 0000 727c 0000 0072  r^...r{...r|...r
-00002ab0: 7d00 0000 7214 0000 0029 1072 b300 0000  }...r....).r....
-00002ac0: 72b4 0000 0072 2700 0000 7240 0000 0072  r....r'...r@...r
-00002ad0: 3c00 0000 724c 0000 0072 3100 0000 724f  <...rL...r1...rO
-00002ae0: 0000 0072 8300 0000 7282 0000 0072 8000  ...r....r....r..
-00002af0: 0000 7281 0000 0072 3b00 0000 7234 0000  ..r....r;...r4..
-00002b00: 00da 0a43 6f64 6553 7472 6561 6d72 2800  ...CodeStreamr(.
-00002b10: 0000 290b 7244 0000 0072 9900 0000 7277  ..).rD...r....rw
-00002b20: 0000 00da 0b69 6e64 656e 7461 7469 6f6e  .....indentation
-00002b30: da04 6c69 6e65 7285 0000 0072 3600 0000  ..liner....r6...
-00002b40: 7284 0000 0072 8700 0000 7286 0000 0072  r....r....r....r
-00002b50: 0a00 0000 7221 0000 0072 2100 0000 7222  ....r!...r!...r"
-00002b60: 0000 0072 8000 0000 5001 0000 7334 0000  ...r....P...s4..
-00002b70: 0004 0108 010a 010a 010a 010e 0118 0108  ................
-00002b80: 0210 0114 010a 010a 0116 010a 0216 010a  ................
-00002b90: 020a 0104 0208 0106 0116 0220 010e 010a  ........... ....
-00002ba0: 0310 010a 027a 0944 6963 742e 6475 6d70  .....z.Dict.dump
-00002bb0: 6303 0000 0000 0000 0000 0000 0003 0000  c...............
-00002bc0: 0003 0000 0043 0000 0073 0c00 0000 7c02  .....C...s....|.
-00002bd0: 7c00 7c01 3c00 6400 5300 7230 0000 0072  |.|.<.d.S.r0...r
-00002be0: 2100 0000 7270 0000 0072 2100 0000 7221  !...rp...r!...r!
-00002bf0: 0000 0072 2200 0000 7256 0000 0074 0100  ...r"...rV...t..
-00002c00: 0073 0200 0000 0c01 7a0e 4469 6374 2e5f  .s......z.Dict._
-00002c10: 7365 745f 6974 656d 7294 0000 0072 9a00  set_itemr....r..
-00002c20: 0000 2909 7247 0000 0072 4800 0000 7249  ..).rG...rH...rI
-00002c30: 0000 0072 7600 0000 72b8 0000 0072 7800  ...rv...r....rx.
-00002c40: 0000 7280 0000 0072 5600 0000 72a2 0000  ..r....rV...r...
-00002c50: 0072 2100 0000 7221 0000 0072 a000 0000  .r!...r!...r....
-00002c60: 7222 0000 0072 3200 0000 4301 0000 730c  r"...r2...C...s.
-00002c70: 0000 0008 000e 0108 060c 030a 0310 2472  ..............$r
-00002c80: 3200 0000 6300 0000 0000 0000 0000 0000  2...c...........
-00002c90: 0000 0000 0004 0000 0000 0000 0073 5a00  .............sZ.
-00002ca0: 0000 6500 5a01 6400 5a02 6401 5a03 6412  ..e.Z.d.Z.d.Z.d.
-00002cb0: 8700 6601 6403 6404 8409 5a04 6405 6406  ..f.d.d...Z.d.d.
-00002cc0: 8400 5a05 6407 6408 8400 5a06 8700 6601  ..Z.d.d...Z...f.
-00002cd0: 6409 640a 8408 5a07 640b 640c 8400 5a08  d.d...Z.d.d...Z.
-00002ce0: 6413 640e 640f 8401 5a09 6413 6410 6411  d.d.d...Z.d.d.d.
-00002cf0: 8401 5a0a 8700 0400 5a0b 5300 2914 7233  ..Z.....Z.S.).r3
-00002d00: 0000 007a 1b52 6570 7265 7365 6e74 7320  ...z.Represents 
-00002d10: 616e 204f 7065 6e46 6f61 6d20 6c69 7374  an OpenFoam list
-00002d20: 4e63 0400 0000 0000 0000 0000 0000 0400  Nc..............
-00002d30: 0000 0300 0000 0300 0000 731c 0000 007c  ..........s....|
-00002d40: 027c 005f 007c 037c 005f 0174 0283 00a0  .|._.|.|._.t....
-00002d50: 037c 01a1 0101 0064 0053 0072 3000 0000  .|.....d.S.r0...
-00002d60: 2904 72b3 0000 00da 065f 6474 7970 6572  ).r......_dtyper
-00002d70: 9f00 0000 7276 0000 0029 0472 4400 0000  ....rv...).rD...
-00002d80: da08 6974 6572 6162 6c65 724d 0000 0072  ..iterablerM...r
-00002d90: 6600 0000 72a0 0000 0072 2100 0000 7222  f...r....r!...r"
-00002da0: 0000 0072 7600 0000 7b01 0000 7306 0000  ...rv...{...s...
-00002db0: 0006 0106 0110 017a 0d4c 6973 742e 5f5f  .......z.List.__
-00002dc0: 696e 6974 5f5f 6301 0000 0000 0000 0000  init__c.........
-00002dd0: 0000 0001 0000 0001 0000 0043 0000 0072  ...........C...r
-00002de0: b600 0000 7230 0000 0072 b700 0000 72a6  ....r0...r....r.
-00002df0: 0000 0072 2100 0000 7221 0000 0072 2200  ...r!...r!...r".
-00002e00: 0000 72b8 0000 0080 0100 0072 b900 0000  ..r........r....
-00002e10: 7a0d 4c69 7374 2e67 6574 5f6e 616d 6563  z.List.get_namec
-00002e20: 0200 0000 0000 0000 0000 0000 0200 0000  ................
-00002e30: 0300 0000 4300 0000 7348 0000 007c 006a  ....C...sH...|.j
-00002e40: 0064 0075 0072 0a7c 017c 005f 0064 0053  .d.u.r.|.|._.d.S
-00002e50: 0074 017c 006a 0074 0283 0272 217c 006a  .t.|.j.t...r!|.j
-00002e60: 007c 016b 0372 1f7c 0164 0117 007c 006a  .|.k.r.|.d...|.j
-00002e70: 0017 007c 005f 0064 0053 0064 0053 0074  ...|._.d.S.d.S.t
-00002e80: 0383 0082 0129 024e 727a 0000 0029 0472  .....).Nrz...).r
-00002e90: b300 0000 7231 0000 0072 4f00 0000 da0c  ....r1...rO.....
-00002ea0: 5275 6e74 696d 6545 7272 6f72 2902 7244  RuntimeError).rD
-00002eb0: 0000 0072 4d00 0000 7221 0000 0072 2100  ...rM...r!...r!.
-00002ec0: 0000 7222 0000 00da 0861 6464 5f6e 616d  ..r".....add_nam
-00002ed0: 6583 0100 0073 0e00 0000 0a01 0a01 0c01  e....s..........
-00002ee0: 0a01 1401 04ff 0603 7a0d 4c69 7374 2e61  ........z.List.a
-00002ef0: 6464 5f6e 616d 6563 0100 0000 0000 0000  dd_namec........
-00002f00: 0000 0000 0100 0000 0200 0000 0300 0000  ................
-00002f10: 72ba 0000 0072 3000 0000 729e 0000 0072  r....r0...r....r
-00002f20: a600 0000 72a0 0000 0072 2100 0000 7222  ....r....r!...r"
-00002f30: 0000 0072 7800 0000 8c01 0000 7293 0000  ...rx.......r...
-00002f40: 007a 0d4c 6973 742e 5f5f 7265 7072 5f5f  .z.List.__repr__
-00002f50: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
-00002f60: 0003 0000 0003 0000 0073 1400 0000 8700  .........s......
-00002f70: 8701 6602 6401 6402 8408 8801 4400 8301  ..f.d.d.....D...
-00002f80: 5300 2903 4e63 0100 0000 0000 0000 0000  S.).Nc..........
-00002f90: 0000 0200 0000 0600 0000 1300 0000 7318  ..............s.
-00002fa0: 0000 0067 007c 005d 087d 0188 01a0 007c  ...g.|.].}.....|
-00002fb0: 0188 00a1 0291 0271 0253 0072 2100 0000  .......q.S.r!...
-00002fc0: a901 da0a 5f64 756d 705f 6974 656d 2902  ...._dump_item).
-00002fd0: 7235 0000 0072 9000 0000 a902 7299 0000  r5...r......r...
-00002fe0: 0072 4400 0000 7221 0000 0072 2200 0000  .rD...r!...r"...
-00002ff0: 7264 0000 0090 0100 0073 0200 0000 1800  rd.......s......
-00003000: 7a2b 4c69 7374 2e5f 6d61 6b65 5f6c 6973  z+List._make_lis
-00003010: 745f 7374 7269 6e67 732e 3c6c 6f63 616c  t_strings.<local
-00003020: 733e 2e3c 6c69 7374 636f 6d70 3e72 2100  s>.<listcomp>r!.
-00003030: 0000 7298 0000 0072 2100 0000 72c5 0000  ..r....r!...r...
-00003040: 0072 2200 0000 da12 5f6d 616b 655f 6c69  .r"....._make_li
-00003050: 7374 5f73 7472 696e 6773 8f01 0000 7302  st_strings....s.
-00003060: 0000 0014 017a 174c 6973 742e 5f6d 616b  .....z.List._mak
-00003070: 655f 6c69 7374 5f73 7472 696e 6773 7201  e_list_stringsr.
-00003080: 0000 0063 0300 0000 0000 0000 0000 0000  ...c............
-00003090: 0300 0000 0400 0000 4300 0000 7332 0000  ........C...s2..
-000030a0: 0074 007c 0174 0174 0266 0283 0272 1174  .t.|.t.t.f...r.t
-000030b0: 037c 0164 0183 0272 117c 01a0 047c 02a1  .|.d...r.|...|..
-000030c0: 0153 007c 0264 0214 0074 057c 0183 0117  .S.|.d...t.|....
-000030d0: 0053 0029 034e 7280 0000 0072 7a00 0000  .S.).Nr....rz...
-000030e0: 2906 7231 0000 0072 4100 0000 7295 0000  ).r1...rA...r...
-000030f0: 0072 8200 0000 7280 0000 0072 4f00 0000  .r....r....rO...
-00003100: 2903 7244 0000 0072 9000 0000 7299 0000  ).rD...r....r...
-00003110: 0072 2100 0000 7221 0000 0072 2200 0000  .r!...r!...r"...
-00003120: 72c4 0000 0092 0100 0073 0600 0000 1801  r........s......
-00003130: 0a01 1002 7a0f 4c69 7374 2e5f 6475 6d70  ....z.List._dump
-00003140: 5f69 7465 6d63 0200 0000 0000 0000 0000  _itemc..........
-00003150: 0000 0a00 0000 0800 0000 0300 0000 7368  ..............sh
-00003160: 0100 0067 007d 0288 0064 0114 007d 0388  ...g.}...d...}..
-00003170: 016a 0064 0075 0072 1f7c 02a0 0188 016a  .j.d.u.r.|.....j
-00003180: 0264 0264 038d 01a1 0101 007c 0364 0417  .d.d.......|.d..
-00003190: 0064 01a0 037c 02a1 0117 0064 0517 0053  .d...|.....d...S
-000031a0: 0088 016a 007d 0488 016a 0464 0075 0172  ...j.}...j.d.u.r
-000031b0: 367c 0464 0688 016a 049b 0064 077c 039b  6|.d...j...d.|..
-000031c0: 0074 0588 0183 019b 009d 0537 007d 047c  .t.........7.}.|
-000031d0: 02a0 067c 037c 0417 0064 087c 039b 009d  ...|.|...d.|....
-000031e0: 0217 0064 0417 00a1 0101 0064 0964 0a64  ...d.......d.d.d
-000031f0: 0b9c 027d 0588 016a 007c 05a0 07a1 0076  ...}...j.|.....v
-00003200: 0172 5e7c 02a0 0664 08a0 0388 01a0 0288  .r^|...d........
-00003210: 0064 0c17 00a1 01a1 01a1 0101 006e 4a88  .d...........nJ.
-00003220: 0172 a87c 0588 016a 0019 007d 0688 0164  .r.|...j...}...d
-00003230: 0219 007c 066b 0273 6f74 0888 0183 0182  ...|.k.sot......
-00003240: 0167 007d 0764 007d 0888 0144 005d 187d  .g.}.d.}...D.].}
-00003250: 097c 097c 066b 0272 887c 0864 0075 0172  .|.|.k.r.|.d.u.r
-00003260: 847c 07a0 067c 08a1 0101 007c 0967 017d  .|...|.....|.g.}
-00003270: 0871 757c 08a0 067c 09a1 0101 0071 757c  .qu|...|.....qu|
-00003280: 07a0 067c 08a1 0101 0087 0166 0164 0d64  ...|.......f.d.d
-00003290: 0e84 087c 0744 0083 017d 077c 02a0 0187  ...|.D...}.|....
-000032a0: 0066 0164 0f64 1084 087c 0744 0083 01a1  .f.d.d...|.D....
-000032b0: 0101 007c 02a0 067c 0364 1117 00a1 0101  ...|...|.d......
-000032c0: 0064 08a0 037c 02a1 0153 0029 124e 727a  .d...|...S.).Nrz
-000032d0: 0000 0072 0100 0000 a901 7299 0000 00fa  ...r......r.....
-000032e0: 0128 72a5 0000 007a 1320 2020 6e6f 6e75  .(r....z.   nonu
-000032f0: 6e69 666f 726d 204c 6973 743c 7a02 3e0a  niform List<z.>.
-00003300: 727e 0000 00da 0368 6578 5a06 7370 6c69  r~.....hexZ.spli
-00003310: 6e65 2902 da06 626c 6f63 6b73 da05 6564  ne)...blocks..ed
-00003320: 6765 7372 3900 0000 6301 0000 0000 0000  gesr9...c.......
-00003330: 0000 0000 0002 0000 0007 0000 0013 0000  ................
-00003340: 0073 2400 0000 6700 7c00 5d0e 7d01 6400  .s$...g.|.].}.d.
-00003350: a000 8700 6601 6401 6402 8408 7c01 4400  ....f.d.d...|.D.
-00003360: 8301 a101 9102 7102 5300 2903 727a 0000  ......q.S.).rz..
-00003370: 0063 0100 0000 0000 0000 0000 0000 0200  .c..............
-00003380: 0000 0400 0000 3300 0000 731a 0000 0081  ......3...s.....
-00003390: 007c 005d 087d 0188 00a0 007c 01a1 0156  .|.].}.....|...V
-000033a0: 0001 0071 0264 0053 0072 3000 0000 72c3  ...q.d.S.r0...r.
-000033b0: 0000 0029 0272 3500 0000 da05 5f69 7465  ...).r5....._ite
-000033c0: 6d72 a600 0000 7221 0000 0072 2200 0000  mr....r!...r"...
-000033d0: 7238 0000 00b9 0100 0072 5c00 0000 7a27  r8.......r\...z'
-000033e0: 4c69 7374 2e64 756d 702e 3c6c 6f63 616c  List.dump.<local
-000033f0: 733e 2e3c 6c69 7374 636f 6d70 3e2e 3c67  s>.<listcomp>.<g
-00003400: 656e 6578 7072 3e72 b100 0000 2902 7235  enexpr>r....).r5
-00003410: 0000 00da 0a69 7465 6d73 5f6c 696e 6572  .....items_liner
-00003420: a600 0000 7221 0000 0072 2200 0000 7264  ....r!...r"...rd
-00003430: 0000 00b8 0100 0073 0800 0000 0600 0202  .......s........
-00003440: 16ff 06ff 7a1d 4c69 7374 2e64 756d 702e  ....z.List.dump.
-00003450: 3c6c 6f63 616c 733e 2e3c 6c69 7374 636f  <locals>.<listco
-00003460: 6d70 3e63 0100 0000 0000 0000 0000 0000  mp>c............
-00003470: 0200 0000 0300 0000 3300 0000 7320 0000  ........3...s ..
-00003480: 0081 007c 005d 0b7d 0188 0064 0017 0064  ...|.].}...d...d
-00003490: 0114 007c 0117 0056 0001 0071 0264 0253  ...|...V...q.d.S
-000034a0: 0029 0372 3900 0000 727a 0000 004e 7221  .).r9...rz...Nr!
-000034b0: 0000 0029 0272 3500 0000 72be 0000 0072  ...).r5...r....r
-000034c0: c700 0000 7221 0000 0072 2200 0000 7238  ....r!...r"...r8
-000034d0: 0000 00bc 0100 0073 0400 0000 0280 1e00  .......s........
-000034e0: 7a1c 4c69 7374 2e64 756d 702e 3c6c 6f63  z.List.dump.<loc
-000034f0: 616c 733e 2e3c 6765 6e65 7870 723e 7a02  als>.<genexpr>z.
-00003500: 293b 2909 72b3 0000 00da 0665 7874 656e  );).r......exten
-00003510: 6472 c600 0000 7228 0000 0072 bf00 0000  dr....r(...r....
-00003520: 7234 0000 0072 2700 0000 da04 6b65 7973  r4...r'.....keys
-00003530: 723d 0000 0029 0a72 4400 0000 7299 0000  r=...).rD...r...
-00003540: 0072 7700 0000 72bd 0000 0072 7400 0000  .rw...r....rt...
-00003550: 5a0c 7370 6563 6961 6c5f 6b65 7973 5a0b  Z.special_keysZ.
-00003560: 7370 6563 6961 6c5f 6b65 79da 056c 696e  special_key..lin
-00003570: 6573 72cd 0000 0072 9000 0000 7221 0000  esr....r....r!..
-00003580: 0072 c500 0000 7222 0000 0072 8000 0000  .r....r"...r....
-00003590: 9801 0000 734a 0000 0004 0108 010a 0112  ....sJ..........
-000035a0: 0116 0106 020a 0102 010a 0102 0102 ff06  ................
-000035b0: 0104 ff04 ff1c 050a 010e 011c 0104 010a  ................
-000035c0: 010c 0108 0104 0104 0108 0108 0108 010a  ................
-000035d0: 0108 010c 020a 010a 0102 0206 fe18 040e  ................
-000035e0: 010a 017a 094c 6973 742e 6475 6d70 7294  ...z.List.dumpr.
-000035f0: 0000 0072 9a00 0000 290c 7247 0000 0072  ...r....).rG...r
-00003600: 4800 0000 7249 0000 00da 075f 5f64 6f63  H...rI.....__doc
-00003610: 5f5f 7276 0000 0072 b800 0000 72c2 0000  __rv...r....r...
-00003620: 0072 7800 0000 72c6 0000 0072 c400 0000  .rx...r....r....
-00003630: 7280 0000 0072 a200 0000 7221 0000 0072  r....r....r!...r
-00003640: 2100 0000 72a0 0000 0072 2200 0000 7233  !...r....r"...r3
-00003650: 0000 0078 0100 0073 1200 0000 0800 0401  ...x...s........
-00003660: 0e02 0805 0803 0c09 0803 0a03 1206 7233  ..............r3
-00003670: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
-00003680: 0000 0000 0100 0000 4000 0000 7310 0000  ........@...s...
-00003690: 0065 005a 0164 005a 0264 015a 0364 0253  .e.Z.d.Z.d.Z.d.S
-000036a0: 0029 0372 bc00 0000 7a22 4120 6469 6374  .).r....z"A dict
-000036b0: 696f 6e6e 6172 7920 746f 2073 746f 7265  ionnary to store
-000036c0: 2023 636f 6465 5374 7265 616d 4e29 0472   #codeStreamN).r
-000036d0: 4700 0000 7248 0000 0072 4900 0000 72d1  G...rH...rI...r.
-000036e0: 0000 0072 2100 0000 7221 0000 0072 2100  ...r!...r!...r!.
-000036f0: 0000 7222 0000 0072 bc00 0000 c101 0000  ..r"...r........
-00003700: 7304 0000 0008 0008 0172 bc00 0000 6301  s........r....c.
-00003710: 0000 0000 0000 0000 0000 0003 0000 0003  ................
-00003720: 0000 0003 0000 0073 2200 0000 8700 6601  .......s".....f.
-00003730: 6401 6402 8408 7d01 8700 6601 6403 6404  d.d...}...f.d.d.
-00003740: 8408 7d02 7400 7c01 7c02 8302 5300 2905  ..}.t.|.|...S.).
-00003750: 4e63 0100 0000 0000 0000 0000 0000 0100  Nc..............
-00003760: 0000 0200 0000 1300 0000 730a 0000 007c  ..........s....|
-00003770: 0088 0019 006a 0053 0072 3000 0000 a901  .....j.S.r0.....
-00003780: da04 636f 6465 72a6 0000 0072 5d00 0000  ..coder....r]...
-00003790: 7221 0000 0072 2200 0000 7252 0000 00c6  r!...r"...rR....
-000037a0: 0100 0072 9300 0000 7a18 5f6d 616b 655f  ...r....z._make_
-000037b0: 616c 6961 732e 3c6c 6f63 616c 733e 2e67  alias.<locals>.g
-000037c0: 6574 6302 0000 0000 0000 0000 0000 0002  etc.............
-000037d0: 0000 0003 0000 0013 0000 0073 0e00 0000  ...........s....
-000037e0: 7c01 7c00 8800 1900 5f00 6400 5300 7230  |.|....._.d.S.r0
-000037f0: 0000 0072 d200 0000 2902 da05 5f73 656c  ...r....)..._sel
-00003800: 6672 3700 0000 725d 0000 0072 2100 0000  fr7...r]...r!...
-00003810: 7222 0000 00da 0373 6574 c901 0000 728f  r".....set....r.
-00003820: 0000 007a 185f 6d61 6b65 5f61 6c69 6173  ...z._make_alias
-00003830: 2e3c 6c6f 6361 6c73 3e2e 7365 7429 01da  .<locals>.set)..
-00003840: 0870 726f 7065 7274 7929 0372 4d00 0000  .property).rM...
-00003850: 7252 0000 0072 d500 0000 7221 0000 0072  rR...r....r!...r
-00003860: 5d00 0000 7222 0000 00da 0b5f 6d61 6b65  ]...r"....._make
-00003870: 5f61 6c69 6173 c501 0000 7306 0000 000c  _alias....s.....
-00003880: 010c 030a 0372 d700 0000 2904 5a0b 636f  .....r....).Z.co
-00003890: 6465 496e 636c 7564 655a 0b63 6f64 654f  deIncludeZ.codeO
-000038a0: 7074 696f 6e73 5a08 636f 6465 4c69 6273  ptionsZ.codeLibs
-000038b0: 72d3 0000 0063 0000 0000 0000 0000 0000  r....c..........
-000038c0: 0000 0000 0000 0300 0000 4000 0000 72a3  ..........@...r.
-000038d0: 0000 0029 0bda 0443 6f64 654e 6304 0000  ...)...CodeNc...
-000038e0: 0000 0000 0000 0000 0004 0000 0002 0000  ................
-000038f0: 0043 0000 0073 1a00 0000 7c01 7c00 5f00  .C...s....|.|._.
-00003900: 7401 7c02 8301 7c00 5f02 7c03 7c00 5f03  t.|...|._.|.|._.
-00003910: 6400 5300 7230 0000 0029 0472 4d00 0000  d.S.r0...).rM...
-00003920: 7206 0000 0072 d300 0000 72b5 0000 0029  r....r....r....)
-00003930: 0472 4400 0000 724d 0000 0072 d300 0000  .rD...rM...r....
-00003940: 72b5 0000 0072 2100 0000 7221 0000 0072  r....r!...r!...r
-00003950: 2200 0000 7276 0000 00d4 0100 0073 0600  "...rv.......s..
-00003960: 0000 0601 0a01 0a01 7a0d 436f 6465 2e5f  ........z.Code._
-00003970: 5f69 6e69 745f 5f63 0100 0000 0000 0000  _init__c........
-00003980: 0000 0000 0100 0000 0500 0000 4300 0000  ............C...
-00003990: 733e 0000 007c 006a 0064 0075 0072 1064  s>...|.j.d.u.r.d
-000039a0: 017c 006a 0164 0064 0285 0219 009b 0064  .|.j.d.d.......d
-000039b0: 039d 0353 0064 017c 006a 0164 0064 0285  ...S.d.|.j.d.d..
-000039c0: 0219 009b 0064 047c 006a 009b 0064 059d  .....d.|.j...d..
-000039d0: 0553 0029 064e 7a06 436f 6465 2822 722f  .S.).Nz.Code("r/
-000039e0: 0000 007a 075b 2e2e 2e5d 2229 7a12 5b2e  ...z.[...]")z.[.
-000039f0: 2e2e 5d22 2c20 6469 7265 6374 6976 653d  ..]", directive=
-00003a00: 72a5 0000 0029 0272 b500 0000 72d3 0000  r....).r....r...
-00003a10: 0072 a600 0000 7221 0000 0072 2100 0000  .r....r!...r!...
-00003a20: 7222 0000 0072 7800 0000 d901 0000 7306  r"...rx.......s.
-00003a30: 0000 000a 0116 011e 017a 0d43 6f64 652e  .........z.Code.
-00003a40: 5f5f 7265 7072 5f5f 7201 0000 0063 0200  __repr__r....c..
-00003a50: 0000 0000 0000 0000 0000 0700 0000 0500  ................
-00003a60: 0000 4300 0000 738a 0000 0067 007d 027c  ..C...s....g.}.|
-00003a70: 0164 0114 007d 037c 0164 0217 0064 0114  .d...}.|.d...d..
-00003a80: 007d 047c 037c 006a 0017 007d 057c 006a  .}.|.|.j...}.|.j
-00003a90: 0164 0075 0172 1d7c 0564 017c 006a 0117  .d.u.r.|.d.|.j..
-00003aa0: 0037 007d 057c 02a0 027c 0564 037c 039b  .7.}.|...|.d.|..
-00003ab0: 009d 0217 0064 0417 00a1 0101 007c 006a  .....d.......|.j
-00003ac0: 03a0 0464 03a1 0144 005d 097d 067c 02a0  ...d...D.].}.|..
-00003ad0: 027c 047c 0617 00a1 0101 0071 2f7c 02a0  .|.|.......q/|..
-00003ae0: 027c 0364 0517 00a1 0101 0064 03a0 057c  .|.d.......d...|
-00003af0: 02a1 0153 0029 064e 727a 0000 0072 3900  ...S.).Nrz...r9.
-00003b00: 0000 727e 0000 007a 0223 7b7a 0323 7d3b  ..r~...z.#{z.#};
-00003b10: 2906 724d 0000 0072 b500 0000 7227 0000  ).rM...r....r'..
-00003b20: 0072 d300 0000 7219 0000 0072 2800 0000  .r....r....r(...
-00003b30: 2907 7244 0000 0072 9900 0000 7277 0000  ).rD...r....rw..
-00003b40: 0072 bd00 0000 5a0c 696e 6465 6e74 6174  .r....Z.indentat
-00003b50: 696f 6e34 7217 0000 0072 be00 0000 7221  ion4r....r....r!
-00003b60: 0000 0072 2100 0000 7222 0000 0072 8000  ...r!...r"...r..
-00003b70: 0000 de01 0000 7316 0000 0004 0108 010c  ......s.........
-00003b80: 010a 010a 010e 0118 0110 0110 010e 010a  ................
-00003b90: 017a 0943 6f64 652e 6475 6d70 7230 0000  .z.Code.dumpr0..
-00003ba0: 0072 9a00 0000 a906 7247 0000 0072 4800  .r......rG...rH.
-00003bb0: 0000 7249 0000 0072 7600 0000 7278 0000  ..rI...rv...rx..
-00003bc0: 0072 8000 0000 7221 0000 0072 2100 0000  .r....r!...r!...
-00003bd0: 7221 0000 0072 2200 0000 72d8 0000 00d3  r!...r"...r.....
-00003be0: 0100 0073 0800 0000 0800 0a01 0805 0e05  ...s............
-00003bf0: 72d8 0000 0063 0000 0000 0000 0000 0000  r....c..........
-00003c00: 0000 0000 0000 0300 0000 4000 0000 72a3  ..........@...r.
-00003c10: 0000 0029 0bda 044e 616d 654e 6303 0000  ...)...NameNc...
-00003c20: 0000 0000 0000 0000 0003 0000 0002 0000  ................
-00003c30: 0043 0000 00f3 1000 0000 7c01 7c00 5f00  .C........|.|._.
-00003c40: 7c02 7c00 5f01 6400 5300 7230 0000 0029  |.|._.d.S.r0...)
-00003c50: 0272 4d00 0000 7237 0000 0029 0372 4400  .rM...r7...).rD.
-00003c60: 0000 724d 0000 0072 3700 0000 7221 0000  ..rM...r7...r!..
-00003c70: 0072 2100 0000 7222 0000 0072 7600 0000  .r!...r"...rv...
-00003c80: ee01 0000 f304 0000 0006 010a 017a 0d4e  .............z.N
-00003c90: 616d 652e 5f5f 696e 6974 5f5f 6301 0000  ame.__init__c...
-00003ca0: 0000 0000 0000 0000 0001 0000 0003 0000  ................
-00003cb0: 0043 0000 0073 0e00 0000 6401 7c00 6a00  .C...s....d.|.j.
-00003cc0: 9b00 6402 9d03 5300 2903 4e7a 054e 616d  ..d...S.).Nz.Nam
-00003cd0: 6528 72a5 0000 0072 5d00 0000 72a6 0000  e(r....r]...r...
-00003ce0: 0072 2100 0000 7221 0000 0072 2200 0000  .r!...r!...r"...
-00003cf0: 7278 0000 00f2 0100 0072 8f00 0000 7a0d  rx.......r....z.
-00003d00: 4e61 6d65 2e5f 5f72 6570 725f 5f72 0100  Name.__repr__r..
-00003d10: 0000 6302 0000 0000 0000 0000 0000 0002  ..c.............
-00003d20: 0000 0001 0000 0043 0000 0073 0800 0000  .......C...s....
-00003d30: 7c00 6a00 9b00 5300 7230 0000 0072 5d00  |.j...S.r0...r].
-00003d40: 0000 7298 0000 0072 2100 0000 7221 0000  ..r....r!...r!..
-00003d50: 0072 2200 0000 7280 0000 00f5 0100 0072  .r"...r........r
-00003d60: af00 0000 7a09 4e61 6d65 2e64 756d 7072  ....z.Name.dumpr
-00003d70: 3000 0000 729a 0000 0072 d900 0000 7221  0...r....r....r!
-00003d80: 0000 0072 2100 0000 7221 0000 0072 2200  ...r!...r!...r".
-00003d90: 0000 72da 0000 00ec 0100 0073 0800 0000  ..r........s....
-00003da0: 0800 0a02 0804 0e03 72da 0000 0063 0000  ........r....c..
-00003db0: 0000 0000 0000 0000 0000 0000 0000 0300  ................
-00003dc0: 0000 4000 0000 7326 0000 0065 005a 0164  ..@...s&...e.Z.d
-00003dd0: 005a 0264 0164 0284 005a 0364 0364 0484  .Z.d.d...Z.d.d..
-00003de0: 005a 0464 0964 0664 0784 015a 0564 0853  .Z.d.d.d...Z.d.S
-00003df0: 0029 0ada 0944 6972 6563 7469 7665 6303  .)...Directivec.
-00003e00: 0000 0000 0000 0000 0000 0003 0000 0002  ................
-00003e10: 0000 0043 0000 0072 db00 0000 7230 0000  ...C...r....r0..
-00003e20: 00a9 0272 b500 0000 da07 636f 6e74 656e  ...r......conten
-00003e30: 7429 0372 4400 0000 72b5 0000 0072 df00  t).rD...r....r..
-00003e40: 0000 7221 0000 0072 2100 0000 7222 0000  ..r!...r!...r"..
-00003e50: 0072 7600 0000 fa01 0000 72dc 0000 007a  .rv.......r....z
-00003e60: 1244 6972 6563 7469 7665 2e5f 5f69 6e69  .Directive.__ini
-00003e70: 745f 5f63 0100 0000 0000 0000 0000 0000  t__c............
-00003e80: 0100 0000 0300 0000 4300 0000 7312 0000  ........C...s...
-00003e90: 007c 006a 009b 0064 017c 006a 019b 009d  .|.j...d.|.j....
-00003ea0: 0353 0029 024e 7297 0000 0072 de00 0000  .S.).Nr....r....
-00003eb0: 72a6 0000 0072 2100 0000 7221 0000 0072  r....r!...r!...r
-00003ec0: 2200 0000 7278 0000 00fe 0100 0073 0200  "...rx.......s..
-00003ed0: 0000 1201 7a12 4469 7265 6374 6976 652e  ....z.Directive.
-00003ee0: 5f5f 7265 7072 5f5f 7201 0000 0063 0200  __repr__r....c..
-00003ef0: 0000 0000 0000 0000 0000 0200 0000 0500  ................
-00003f00: 0000 4300 0000 731c 0000 007c 0164 0114  ..C...s....|.d..
-00003f10: 007c 006a 009b 0064 027c 006a 019b 0064  .|.j...d.|.j...d
-00003f20: 039d 0417 0053 0029 044e 727a 0000 0072  .....S.).Nrz...r
-00003f30: 9700 0000 727c 0000 0072 de00 0000 7298  ....r|...r....r.
-00003f40: 0000 0072 2100 0000 7221 0000 0072 2200  ...r!...r!...r".
-00003f50: 0000 7280 0000 0001 0200 0072 b200 0000  ..r........r....
-00003f60: 7a0e 4469 7265 6374 6976 652e 6475 6d70  z.Directive.dump
-00003f70: 4e72 9a00 0000 72d9 0000 0072 2100 0000  Nr....r....r!...
-00003f80: 7221 0000 0072 2100 0000 7222 0000 0072  r!...r!...r"...r
-00003f90: dd00 0000 f901 0000 7308 0000 0008 0008  ........s.......
-00003fa0: 0108 040e 0372 dd00 0000 2901 722f 0000  .....r....).r/..
-00003fb0: 0029 2772 d100 0000 7215 0000 00da 0361  .)'r....r......a
-00003fc0: 6263 7202 0000 0072 0300 0000 da0b 6461  bcr....r......da
-00003fd0: 7461 636c 6173 7365 7372 0400 0000 da07  taclassesr......
-00003fe0: 6e75 6d62 6572 7372 0500 0000 da08 7465  numbersr......te
-00003ff0: 7874 7772 6170 7206 0000 00da 0674 7970  xtwrapr......typ
-00004000: 696e 6772 0700 0000 da05 6e75 6d70 7972  ingr......numpyr
-00004010: 6800 0000 5a0a 696e 666c 6563 7469 6f6e  h...Z.inflection
-00004020: 7208 0000 0072 1b00 0000 7223 0000 0072  r....r....r#...r
-00004030: 2e00 0000 7240 0000 0072 4100 0000 724a  ....r@...rA...rJ
-00004040: 0000 0072 7100 0000 7295 0000 0072 9d00  ...rq...r....r..
-00004050: 0000 726f 0000 0072 5100 0000 72ad 0000  ..ro...rQ...r...
-00004060: 0072 5400 0000 7232 0000 0072 3300 0000  .rT...r2...r3...
-00004070: 72bc 0000 0072 d700 0000 72b3 0000 00da  r....r....r.....
-00004080: 0773 6574 6174 7472 72d8 0000 0072 da00  .setattrr....r..
-00004090: 0000 72dd 0000 0072 2100 0000 7221 0000  ..r....r!...r!..
-000040a0: 0072 2100 0000 7222 0000 00da 083c 6d6f  .r!...r".....<mo
-000040b0: 6475 6c65 3e01 0000 0073 4000 0000 0400  dule>....s@.....
-000040c0: 0802 1001 0c01 0c01 0c01 0c01 0802 0c01  ................
-000040d0: 0802 0803 081b 0a12 0e11 1007 1257 024b  .............W.K
-000040e0: 1001 100b 020c 1201 1226 140d 1235 1049  .........&...5.I
-000040f0: 0804 080a 1601 1003 0219 1201 140c       ..............
+00000410: 745f 696e 6465 78a9 0072 2100 0000 fa46  t_index..r!....F
+00000420: 2f68 6f6d 652f 7069 6572 7265 2f44 6576  /home/pierre/Dev
+00000430: 2f66 6c75 6964 7369 6d66 6f61 6d2f 7372  /fluidsimfoam/sr
+00000440: 632f 666c 7569 6473 696d 666f 616d 2f66  c/fluidsimfoam/f
+00000450: 6f61 6d5f 696e 7075 745f 6669 6c65 732f  oam_input_files/
+00000460: 6173 742e 7079 da0e 7374 7232 666f 616d  ast.py..str2foam
+00000470: 5f75 6e69 7473 1000 0000 7330 0000 000a  _units....s0....
+00000480: 0104 0104 0102 0114 010c 0104 0104 0108  ................
+00000490: 0102 fd08 050c 010c 0110 0108 010e 010a  ................
+000004a0: 010a 0208 010a 010c 0110 0104 ec04 1572  ...............r
+000004b0: 2300 0000 6301 0000 0000 0000 0000 0000  #...c...........
+000004c0: 0005 0000 0008 0000 0043 0000 0073 a800  .........C...s..
+000004d0: 0000 6700 7d01 7400 7401 7c00 8302 4400  ..g.}.t.t.|...D.
+000004e0: 5d2f 5c02 7d02 7d03 7c03 6401 6b02 7210  ]/\.}.}.|.d.k.r.
+000004f0: 7107 7c03 6401 6b04 7216 6402 6e01 6403  q.|.d.k.r.d.n.d.
+00000500: 7d04 7402 7c03 8301 6404 6b02 7228 7c01  }.t.|...d.k.r(|.
+00000510: a003 7c04 9b00 7c02 9b00 9d02 a101 0100  ..|...|.........
+00000520: 7107 7c01 a003 7c04 9b00 7c02 9b00 6405  q.|...|...|...d.
+00000530: 7402 7c03 8301 9b00 9d04 a101 0100 7107  t.|...........q.
+00000540: 6406 a004 7c01 a101 7d01 7c01 a005 6402  d...|...}.|...d.
+00000550: a101 7249 7c01 6404 6400 8502 1900 7d01  ..rI|.d.d.....}.
+00000560: 7c01 5300 7c01 a005 6403 a101 7252 6407  |.S.|...d...rRd.
+00000570: 7c01 1700 7d01 7c01 5300 2908 4e72 0100  |...}.|.S.).Nr..
+00000580: 0000 7211 0000 00fa 012f 720f 0000 0072  ..r....../r....r
+00000590: 1200 0000 7210 0000 0072 1300 0000 2906  ....r....r....).
+000005a0: da03 7a69 7072 1b00 0000 da03 6162 73da  ..zipr......abs.
+000005b0: 0661 7070 656e 64da 046a 6f69 6eda 0a73  .append..join..s
+000005c0: 7461 7274 7377 6974 6829 05da 0a66 6f61  tartswith)...foa
+000005d0: 6d5f 756e 6974 7372 1e00 0000 da06 7379  m_unitsr......sy
+000005e0: 6d62 6f6c da08 6578 706f 6e65 6e74 da08  mbol..exponent..
+000005f0: 6f70 6572 6174 6f72 7221 0000 0072 2100  operatorr!...r!.
+00000600: 0000 7222 0000 00da 0e66 6f61 6d5f 756e  ..r".....foam_un
+00000610: 6974 7332 7374 722b 0000 0073 1e00 0000  its2str+...s....
+00000620: 0401 1201 0801 0201 1001 0c01 1401 1e02  ................
+00000630: 0a01 0a01 0c01 0403 0afe 0801 0401 722e  ..............r.
+00000640: 0000 00e9 1400 0000 6302 0000 0000 0000  ........c.......
+00000650: 0000 0000 0003 0000 0008 0000 0043 0000  .............C..
+00000660: 0073 4400 0000 7a10 7400 7c01 7401 6401  .sD...z.t.|.t.d.
+00000670: 6402 8400 7c00 a002 a100 4400 8301 8301  d...|.....D.....
+00000680: 8302 7d01 5700 6e0b 0400 7403 791b 0100  ..}.W.n...t.y...
+00000690: 0100 0100 6403 7d01 5900 6e01 7700 6404  ....d.}.Y.n.w.d.
+000006a0: 7d02 7c01 7c02 1700 5300 2905 4e63 0100  }.|.|...S.).Nc..
+000006b0: 0000 0000 0000 0000 0000 0300 0000 0500  ................
+000006c0: 0000 7300 0000 7332 0000 0081 007c 005d  ..s...s2.....|.]
+000006d0: 145c 027d 017d 027c 0264 0075 0172 0274  .\.}.}.|.d.u.r.t
+000006e0: 007c 0274 0174 0266 0283 0273 0274 037c  .|.t.t.f...s.t.|
+000006f0: 0183 0156 0001 0071 0264 0053 00a9 014e  ...V...q.d.S...N
+00000700: 2904 da0a 6973 696e 7374 616e 6365 da04  )...isinstance..
+00000710: 4469 6374 da04 4c69 7374 da03 6c65 6e29  Dict..List..len)
+00000720: 03da 022e 30da 036b 6579 da05 7661 6c75  ....0..key..valu
+00000730: 6572 2100 0000 7221 0000 0072 2200 0000  er!...r!...r"...
+00000740: da09 3c67 656e 6578 7072 3e41 0000 0073  ..<genexpr>A...s
+00000750: 1200 0000 0280 0400 0602 0601 02fd 0c03  ................
+00000760: 02fd 0601 0aff 7a2b 5f63 6f6d 7075 7465  ......z+_compute
+00000770: 5f73 7061 6365 735f 746f 5f61 6c69 676e  _spaces_to_align
+00000780: 2e3c 6c6f 6361 6c73 3e2e 3c67 656e 6578  .<locals>.<genex
+00000790: 7072 3e72 0100 0000 e904 0000 0029 04da  pr>r.........)..
+000007a0: 036d 696e da03 6d61 78da 0569 7465 6d73  .min..max..items
+000007b0: da0a 5661 6c75 6545 7272 6f72 2903 da04  ..ValueError)...
+000007c0: 6461 7461 da0a 6d61 785f 6c65 6e67 7468  data..max_length
+000007d0: 5a0d 6465 6661 756c 745f 7370 6163 6572  Z.default_spacer
+000007e0: 2100 0000 7221 0000 0072 2200 0000 da18  !...r!...r".....
+000007f0: 5f63 6f6d 7075 7465 5f73 7061 6365 735f  _compute_spaces_
+00000800: 746f 5f61 6c69 676e 3d00 0000 7318 0000  to_align=...s...
+00000810: 0002 0102 0102 0108 0106 0206 fe08 fe0c  ................
+00000820: 0808 0102 ff04 0308 0172 4000 0000 6300  .........r@...c.
+00000830: 0000 0000 0000 0000 0000 0000 0000 0002  ................
+00000840: 0000 0040 0000 0073 1400 0000 6500 5a01  ...@...s....e.Z.
+00000850: 6400 5a02 6401 6402 8400 5a03 6403 5300  d.Z.d.d...Z.d.S.
+00000860: 2904 da04 4e6f 6465 6302 0000 0000 0000  )...Nodec.......
+00000870: 0000 0000 0002 0000 0003 0000 0043 0000  .............C..
+00000880: 0073 2000 0000 7400 7c01 8301 7400 7c00  .s ...t.|...t.|.
+00000890: 8301 7500 720e 7c00 6a01 7c01 6a01 6b02  ..u.r.|.j.|.j.k.
+000008a0: 5300 6401 5300 2902 4e46 2902 da04 7479  S.d.S.).NF)...ty
+000008b0: 7065 da08 5f5f 6469 6374 5f5f 2902 da04  pe..__dict__)...
+000008c0: 7365 6c66 da05 6f74 6865 7272 2100 0000  self..otherr!...
+000008d0: 7221 0000 0072 2200 0000 da06 5f5f 6571  r!...r".....__eq
+000008e0: 5f5f 4f00 0000 7306 0000 0010 010c 0104  __O...s.........
+000008f0: 017a 0b4e 6f64 652e 5f5f 6571 5f5f 4e29  .z.Node.__eq__N)
+00000900: 04da 085f 5f6e 616d 655f 5fda 0a5f 5f6d  ...__name__..__m
+00000910: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
+00000920: 616d 655f 5f72 4600 0000 7221 0000 0072  ame__rF...r!...r
+00000930: 2100 0000 7221 0000 0072 2200 0000 7241  !...r!...r"...rA
+00000940: 0000 004e 0000 0073 0400 0000 0800 0c01  ...N...s........
+00000950: 7241 0000 0063 0000 0000 0000 0000 0000  rA...c..........
+00000960: 0000 0000 0000 0800 0000 4000 0000 7350  ..........@...sP
+00000970: 0000 0065 005a 0164 005a 0209 0109 0209  ...e.Z.d.Z......
+00000980: 0164 0e64 0365 0364 0465 0465 0319 0064  .d.d.e.d.e.e...d
+00000990: 0565 0465 0319 0066 0664 0664 0784 055a  .e.e...f.d.d...Z
+000009a0: 0564 0864 0984 005a 0664 0f64 0a64 0b84  .d.d...Z.d.d.d..
+000009b0: 015a 0765 0864 0c64 0d84 0083 015a 0964  .Z.e.d.d.....Z.d
+000009c0: 0153 0029 10da 0e4e 6f64 654c 696b 6550  .S.)...NodeLikeP
+000009d0: 7944 6963 744e 4672 3e00 0000 da0a 6469  yDictNFr>.....di
+000009e0: 6d65 6e73 696f 6e73 da08 636f 6d6d 656e  mensions..commen
+000009f0: 7473 6305 0000 0000 0000 0000 0000 000b  tsc.............
+00000a00: 0000 0007 0000 0043 0000 0073 fa00 0000  .......C...s....
+00000a10: 7c02 6400 7500 7206 6900 7d02 7c04 6400  |.d.u.r.i.}.|.d.
+00000a20: 7500 720c 6900 7d04 7c01 a000 a100 4400  u.r.i.}.|.....D.
+00000a30: 5d6a 5c02 7d05 7d06 7401 7c06 7402 6400  ]j\.}.}.t.|.t.d.
+00000a40: 8301 7403 6602 8302 7224 7c00 a004 7c05  ..t.f...r$|...|.
+00000a50: 7c06 a102 0100 7110 7401 7c06 7405 7406  |.....q.t.|.t.t.
+00000a60: 6602 8302 724d 7c03 6401 7500 7236 7c00  f...rM|.d.u.r6|.
+00000a70: a004 7c05 7c06 a102 0100 7110 7c02 a007  ..|.|.....q.|...
+00000a80: 7c05 7c03 a102 7d07 7401 7c06 7406 8302  |.|...}.t.|.t...
+00000a90: 7245 7408 7c06 8301 7d06 7c00 a009 7c05  rEt.|...}.|...|.
+00000aa0: 7c06 7c07 a103 0100 7110 7401 7c06 740a  |.|.....q.t.|.t.
+00000ab0: 8302 7275 7c02 a007 7c05 6400 a102 7d08  ..ru|...|.d...}.
+00000ac0: 7c04 a007 7c05 6400 a102 7d09 740b 6900  |...|.d...}.t.i.
+00000ad0: 7c05 7c09 6402 8d03 7d0a 7c0a 6a0c 7c06  |.|.d...}.|.j.|.
+00000ae0: 7c08 7c03 7c09 6403 8d04 0100 7c00 a00d  |.|.|.d.....|...
+00000af0: 7c05 7c0a a102 0100 7110 740e 7402 7c06  |.|.....q.t.t.|.
+00000b00: 8301 8301 8201 6400 5300 2904 4e46 2902  ......d.S.).NF).
+00000b10: da04 6e61 6d65 724c 0000 0029 0372 4b00  ..namerL...).rK.
+00000b20: 0000 da11 6465 6661 756c 745f 6469 6d65  ....default_dime
+00000b30: 6e73 696f 6e72 4c00 0000 290f 723c 0000  nsionrL...).r<..
+00000b40: 0072 3100 0000 7242 0000 00da 0373 7472  .r1...rB.....str
+00000b50: da09 7365 745f 6368 696c 6472 0500 0000  ..set_childr....
+00000b60: da04 6c69 7374 da03 6765 7472 3300 0000  ..list..getr3...
+00000b70: da09 7365 745f 7661 6c75 65da 0464 6963  ..set_value..dic
+00000b80: 7472 3200 0000 da14 696e 6974 5f66 726f  tr2.....init_fro
+00000b90: 6d5f 7079 5f6f 626a 6563 7473 da09 5f73  m_py_objects.._s
+00000ba0: 6574 5f69 7465 6dda 134e 6f74 496d 706c  et_item..NotImpl
+00000bb0: 656d 656e 7465 6445 7272 6f72 290b 7244  ementedError).rD
+00000bc0: 0000 0072 3e00 0000 724b 0000 0072 4e00  ...r>...rK...rN.
+00000bd0: 0000 724c 0000 0072 3600 0000 7237 0000  ..rL...r6...r7..
+00000be0: 00da 0964 696d 656e 7369 6f6e 5a0f 6469  ...dimensionZ.di
+00000bf0: 6d65 6e73 696f 6e73 5f64 6963 745a 0d63  mensions_dictZ.c
+00000c00: 6f6d 6d65 6e74 735f 6469 6374 da03 6f62  omments_dict..ob
+00000c10: 6a72 2100 0000 7221 0000 0072 2200 0000  jr!...r!...r"...
+00000c20: 7255 0000 0056 0000 0073 3600 0000 0807  rU...V...s6.....
+00000c30: 0401 0801 0401 1001 1201 0e01 0e01 0801  ................
+00000c40: 0e01 0c02 0a01 0801 1001 0a01 0c01 0c01  ................
+00000c50: 0e01 0401 0201 0201 0201 0201 06fc 0e06  ................
+00000c60: 0c02 04e9 7a23 4e6f 6465 4c69 6b65 5079  ....z#NodeLikePy
+00000c70: 4469 6374 2e69 6e69 745f 6672 6f6d 5f70  Dict.init_from_p
+00000c80: 795f 6f62 6a65 6374 7363 0300 0000 0000  y_objectsc......
+00000c90: 0000 0000 0000 0600 0000 0600 0000 4300  ..............C.
+00000ca0: 0000 733a 0100 0074 007c 0274 0183 0272  ..s:...t.|.t...r
+00000cb0: 227c 0272 2274 007c 0264 0119 0074 0183  "|.r"t.|.d...t..
+00000cc0: 0272 227c 0264 0119 0072 2274 0264 0264  .r"|.d...r"t.d.d
+00000cd0: 0384 007c 0264 0119 0044 0083 0183 0172  ...|.d...D.....r
+00000ce0: 2274 03a0 047c 02a1 017d 0274 007c 0274  "t...|...}.t.|.t
+00000cf0: 0564 0083 0174 0674 0774 0866 0483 0272  .d...t.t.t.f...r
+00000d00: 2e6e 6774 007c 0274 0983 0272 3a74 0a7c  .ngt.|.t...r:t.|
+00000d10: 027c 0164 048d 027d 026e 5b74 007c 0274  .|.d...}.n[t.|.t
+00000d20: 0183 0272 4674 0b7c 027c 0164 048d 027d  ...rFt.|.|.d...}
+00000d30: 026e 4f74 007c 0274 036a 0c83 0272 897c  .nOt.|.t.j...r.|
+00000d40: 026a 0d7d 037c 026a 0e7d 047c 02a0 0fa1  .j.}.|.j.}.|....
+00000d50: 0001 0064 007d 057c 0464 056b 0272 787c  ...d.}.|.d.k.rx|
+00000d60: 0364 0619 0064 076b 0272 6564 087d 056e  .d...d.k.red.}.n
+00000d70: 0b7c 0364 0619 0064 096b 0272 6e64 0a7d  .|.d...d.k.rnd.}
+00000d80: 056e 0274 1082 0164 0b64 0c84 007c 0244  .n.t...d.d...|.D
+00000d90: 0083 017d 026e 097c 0464 066b 0272 7f64  ...}.n.|.d.k.r.d
+00000da0: 0d7d 056e 0274 1082 0174 0b7c 027c 017c  .}.n.t...t.|.|.|
+00000db0: 0564 0e8d 037d 026e 0c74 007c 0274 1183  .d...}.n.t.|.t..
+00000dc0: 0272 8f6e 0674 1074 057c 0283 0183 0182  .r.n.t.t.|......
+00000dd0: 017c 00a0 127c 017c 02a1 0201 0064 0053  .|...|.|.....d.S
+00000de0: 0029 0f4e 7201 0000 0063 0100 0000 0000  .).Nr....c......
+00000df0: 0000 0000 0000 0200 0000 0400 0000 7300  ..............s.
+00000e00: 0000 f31a 0000 0081 007c 005d 087d 0174  .........|.].}.t
+00000e10: 007c 0174 0183 0256 0001 0071 0264 0053  .|.t...V...q.d.S
+00000e20: 0072 3000 0000 2902 7231 0000 0072 0500  .r0...).r1...r..
+00000e30: 0000 2902 7235 0000 00da 016e 7221 0000  ..).r5.....nr!..
+00000e40: 0072 2100 0000 7222 0000 0072 3800 0000  .r!...r"...r8...
+00000e50: 8000 0000 f304 0000 0002 8018 007a 2b4e  .............z+N
+00000e60: 6f64 654c 696b 6550 7944 6963 742e 7365  odeLikePyDict.se
+00000e70: 745f 6368 696c 642e 3c6c 6f63 616c 733e  t_child.<locals>
+00000e80: 2e3c 6765 6e65 7870 723e a901 724d 0000  .<genexpr>..rM..
+00000e90: 00e9 0200 0000 720f 0000 00e9 0900 0000  ......r.........
+00000ea0: da06 7465 6e73 6f72 e903 0000 005a 0676  ..tensor.....Z.v
+00000eb0: 6563 746f 7263 0100 0000 0000 0000 0000  ectorc..........
+00000ec0: 0000 0200 0000 0400 0000 5300 0000 7314  ..........S...s.
+00000ed0: 0000 0067 007c 005d 067d 0174 007c 0183  ...g.|.].}.t.|..
+00000ee0: 0191 0271 0253 0072 2100 0000 2901 7233  ...q.S.r!...).r3
+00000ef0: 0000 0029 0272 3500 0000 da08 7365 7175  ...).r5.....sequ
+00000f00: 656e 6365 7221 0000 0072 2100 0000 7222  encer!...r!...r"
+00000f10: 0000 00da 0a3c 6c69 7374 636f 6d70 3e96  .....<listcomp>.
+00000f20: 0000 0073 0200 0000 1400 7a2c 4e6f 6465  ...s......z,Node
+00000f30: 4c69 6b65 5079 4469 6374 2e73 6574 5f63  LikePyDict.set_c
+00000f40: 6869 6c64 2e3c 6c6f 6361 6c73 3e2e 3c6c  hild.<locals>.<l
+00000f50: 6973 7463 6f6d 703e da06 7363 616c 6172  istcomp>..scalar
+00000f60: 2902 724d 0000 00da 0564 7479 7065 2913  ).rM.....dtype).
+00000f70: 7231 0000 0072 5100 0000 da03 616c 6cda  r1...rQ.....all.
+00000f80: 026e 70da 0561 7272 6179 7242 0000 0072  .np..arrayrB...r
+00000f90: 4f00 0000 7205 0000 00da 0c44 696d 656e  O...r......Dimen
+00000fa0: 7369 6f6e 5365 7472 5400 0000 7232 0000  sionSetrT...r2..
+00000fb0: 0072 3300 0000 da07 6e64 6172 7261 79da  .r3.....ndarray.
+00000fc0: 0573 6861 7065 da04 6e64 696d da06 746f  .shape..ndim..to
+00000fd0: 6c69 7374 7257 0000 0072 4100 0000 7256  listrW...rA...rV
+00000fe0: 0000 0029 0672 4400 0000 7236 0000 00da  ...).rD...r6....
+00000ff0: 0563 6869 6c64 726b 0000 0072 6c00 0000  .childrk...rl...
+00001000: 7265 0000 0072 2100 0000 7221 0000 0072  re...r!...r!...r
+00001010: 2200 0000 7250 0000 007a 0000 0073 4a00  "...rP...z...sJ.
+00001020: 0000 0802 02ff 0202 02fe 0c03 02fd 0604  ................
+00001030: 02fc 1405 02fb 0a07 1602 0201 0a01 0e01  ................
+00001040: 0a01 0e01 0c01 0601 0601 0801 0401 0801  ................
+00001050: 0c01 0601 0c01 0601 0402 1001 0801 0601  ................
+00001060: 0402 1001 0a01 0201 0c02 1001 7a18 4e6f  ............z.No
+00001070: 6465 4c69 6b65 5079 4469 6374 2e73 6574  deLikePyDict.set
+00001080: 5f63 6869 6c64 6304 0000 0000 0000 0000  _childc.........
+00001090: 0000 0004 0000 0005 0000 0043 0000 0073  ...........C...s
+000010a0: 3000 0000 7400 7c02 7401 8302 7309 7c03  0...t.|.t...s.|.
+000010b0: 6400 7501 7210 7402 7c02 7c01 7c03 6401  d.u.r.t.|.|.|.d.
+000010c0: 8d03 7d02 7c00 a003 7c01 7c02 a102 0100  ..}.|...|.|.....
+000010d0: 6400 5300 2902 4e29 0172 5800 0000 2904  d.S.).N).rX...).
+000010e0: 7231 0000 0072 0500 0000 da05 5661 6c75  r1...r......Valu
+000010f0: 6572 5600 0000 2904 7244 0000 0072 4d00  erV...).rD...rM.
+00001100: 0000 7237 0000 0072 5800 0000 7221 0000  ..r7...rX...r!..
+00001110: 0072 2100 0000 7222 0000 0072 5300 0000  .r!...r"...rS...
+00001120: a200 0000 7306 0000 0012 010e 0110 017a  ....s..........z
+00001130: 184e 6f64 654c 696b 6550 7944 6963 742e  .NodeLikePyDict.
+00001140: 7365 745f 7661 6c75 6563 0300 0000 0000  set_valuec......
+00001150: 0000 0000 0000 0300 0000 0100 0000 4300  ..............C.
+00001160: 0000 7304 0000 0064 0153 0029 027a 0b53  ..s....d.S.).z.S
+00001170: 6574 2061 6e20 6974 656d 4e72 2100 0000  et an itemNr!...
+00001180: a903 7244 0000 0072 3600 0000 7237 0000  ..rD...r6...r7..
+00001190: 0072 2100 0000 7221 0000 0072 2200 0000  .r!...r!...r"...
+000011a0: 7256 0000 00a7 0000 0073 0200 0000 0400  rV.......s......
+000011b0: 7a18 4e6f 6465 4c69 6b65 5079 4469 6374  z.NodeLikePyDict
+000011c0: 2e5f 7365 745f 6974 656d 2903 4e46 4e72  ._set_item).NFNr
+000011d0: 3000 0000 290a 7247 0000 0072 4800 0000  0...).rG...rH...
+000011e0: 7249 0000 0072 5400 0000 7207 0000 0072  rI...rT...r....r
+000011f0: 5500 0000 7250 0000 0072 5300 0000 7203  U...rP...rS...r.
+00001200: 0000 0072 5600 0000 7221 0000 0072 2100  ...rV...r!...r!.
+00001210: 0000 7221 0000 0072 2200 0000 724a 0000  ..r!...r"...rJ..
+00001220: 0055 0000 0073 1e00 0000 0800 0204 0201  .U...s..........
+00001230: 0201 04fb 0202 02fe 0603 02fd 0605 0afb  ................
+00001240: 0824 0a28 0205 0e01 724a 0000 0063 0000  .$.(....rJ...c..
+00001250: 0000 0000 0000 0000 0000 0000 0000 0300  ................
+00001260: 0000 4000 0000 7346 0000 0065 005a 0164  ..@...sF...e.Z.d
+00001270: 005a 0264 1064 0264 0384 015a 0364 0464  .Z.d.d.d...Z.d.d
+00001280: 0584 005a 0464 0664 0784 005a 0564 0864  ...Z.d.d...Z.d.d
+00001290: 0984 005a 0664 0a64 0b84 005a 0764 0c64  ...Z.d.d...Z.d.d
+000012a0: 0d84 005a 0864 0e64 0f84 005a 0964 0153  ...Z.d.d...Z.d.S
+000012b0: 0029 11da 0d46 6f61 6d49 6e70 7574 4669  .)...FoamInputFi
+000012c0: 6c65 4e63 0500 0000 0000 0000 0000 0000  leNc............
+000012d0: 0500 0000 0200 0000 4300 0000 732e 0000  ........C...s...
+000012e0: 007c 017c 005f 007c 0264 0075 0072 0969  .|.|._.|.d.u.r.i
+000012f0: 007d 027c 027c 005f 017c 037c 005f 027c  .}.|.|._.|.|._.|
+00001300: 047c 005f 0364 007c 005f 0464 0053 0072  .|._.d.|._.d.S.r
+00001310: 3000 0000 2905 da04 696e 666f da08 6368  0...)...info..ch
+00001320: 696c 6472 656e da06 6865 6164 6572 724c  ildren..headerrL
+00001330: 0000 00da 0470 6174 6829 0572 4400 0000  .....path).rD...
+00001340: 7272 0000 0072 7300 0000 7274 0000 0072  rr...rs...rt...r
+00001350: 4c00 0000 7221 0000 0072 2100 0000 7222  L...r!...r!...r"
+00001360: 0000 00da 085f 5f69 6e69 745f 5fad 0000  .....__init__...
+00001370: 0073 0e00 0000 0601 0801 0401 0601 0601  .s..............
+00001380: 0601 0a01 7a16 466f 616d 496e 7075 7446  ....z.FoamInputF
+00001390: 696c 652e 5f5f 696e 6974 5f5f 6301 0000  ile.__init__c...
+000013a0: 0000 0000 0000 0000 0002 0000 0005 0000  ................
+000013b0: 0043 0000 0073 4200 0000 6401 6701 7d01  .C...sB...d.g.}.
+000013c0: 7c00 6a00 6400 7501 7212 7c01 a001 6402  |.j.d.u.r.|...d.
+000013d0: 7c00 6a00 9b00 6403 9d03 a101 0100 7c01  |.j...d.......|.
+000013e0: a001 6404 7c00 6a02 9b00 6405 9d03 a101  ..d.|.j...d.....
+000013f0: 0100 6406 a003 7c01 a101 5300 2907 4e7a  ..d...|...S.).Nz
+00001400: 0b49 6e70 7574 4669 6c65 280a 7a05 696e  .InputFile(.z.in
+00001410: 666f 3d7a 022c 0a7a 0963 6869 6c64 7265  fo=z.,.z.childre
+00001420: 6e3d 7a02 0a29 7210 0000 0029 0472 7200  n=z..)r....).rr.
+00001430: 0000 7227 0000 0072 7300 0000 7228 0000  ..r'...rs...r(..
+00001440: 0029 0272 4400 0000 da03 746d 7072 2100  .).rD.....tmpr!.
+00001450: 0000 7221 0000 0072 2200 0000 da08 5f5f  ..r!...r".....__
+00001460: 7265 7072 5f5f b600 0000 730a 0000 0006  repr__....s.....
+00001470: 010a 0114 0114 010a 017a 1646 6f61 6d49  .........z.FoamI
+00001480: 6e70 7574 4669 6c65 2e5f 5f72 6570 725f  nputFile.__repr_
+00001490: 5f63 0100 0000 0000 0000 0000 0000 0b00  _c..............
+000014a0: 0000 0800 0000 4300 0000 73a2 0100 0067  ......C...s....g
+000014b0: 007d 017c 006a 0064 0075 0172 3664 0167  .}.|.j.d.u.r6d.g
+000014c0: 017d 027c 006a 00a0 01a1 0044 005d 195c  .}.|.j.....D.].\
+000014d0: 027d 037d 0464 0274 027c 0383 0118 0064  .}.}.d.t.|.....d
+000014e0: 0314 007d 057c 02a0 0364 047c 039b 007c  ...}.|...d.|...|
+000014f0: 059b 007c 049b 0064 059d 05a1 0101 0071  ...|...d.......q
+00001500: 0f7c 02a0 0364 06a1 0101 007c 01a0 0364  .|...d.....|...d
+00001510: 07a0 047c 02a1 01a1 0101 0074 057c 006a  ...|.......t.|.j
+00001520: 0664 0864 098d 027d 067c 006a 06a0 01a1  .d.d...}.|.j....
+00001530: 0044 005d 715c 027d 037d 0474 077c 0464  .D.]q\.}.}.t.|.d
+00001540: 0a83 0272 5d7c 04a0 08a1 007d 077c 0364  ...r]|.....}.|.d
+00001550: 0075 0072 5c74 097c 0474 0a83 0272 5c7c  .u.r\t.|.t...r\|
+00001560: 0764 0537 007d 076e 2f7c 0464 0075 0072  .d.7.}.n/|.d.u.r
+00001570: 657c 039b 007d 076e 2774 077c 0464 0b83  e|...}.n't.|.d..
+00001580: 0272 6f7c 04a0 0ba1 007d 086e 027c 047d  .ro|.....}.n.|.}
+00001590: 087c 0864 0c6b 0272 7864 0c7d 056e 0b74  .|.d.k.rxd.}.n.t
+000015a0: 0c64 0d7c 0674 027c 0383 0118 0083 0264  .d.|.t.|.......d
+000015b0: 0314 007d 057c 039b 007c 059b 007c 089b  ...}.|...|...|..
+000015c0: 0064 059d 047d 077c 006a 0d64 0075 0172  .d...}.|.j.d.u.r
+000015d0: ae7c 037c 006a 0d76 0072 ae7c 006a 0d7c  .|.|.j.v.r.|.j.|
+000015e0: 0319 007d 0974 097c 0974 0e83 0272 ae64  ...}.t.|.t...r.d
+000015f0: 0e7c 09a0 0f64 0764 0fa1 0217 007d 097c  .|...d.d.....}.|
+00001600: 0964 0717 007c 0717 007d 077c 01a0 037c  .d...|...}.|...|
+00001610: 07a1 0101 0071 4264 10a0 047c 01a1 017d  .....qBd...|...}
+00001620: 0a7c 006a 1064 0075 0172 c57c 006a 1064  .|.j.d.u.r.|.j.d
+00001630: 0717 007c 0a17 007d 0a7c 0a64 1119 0064  ...|...}.|.d...d
+00001640: 076b 0372 cf7c 0a64 0737 007d 0a7c 0a53  .k.r.|.d.7.}.|.S
+00001650: 0029 124e 7a0a 466f 616d 4669 6c65 0a7b  .).Nz.FoamFile.{
+00001660: e90c 0000 00fa 0120 fa04 2020 2020 fa01  ....... ..    ..
+00001670: 3bda 017d da01 0ae9 0e00 0000 2901 723f  ;..}........).r?
+00001680: 0000 00da 0464 756d 70da 1764 756d 705f  .....dump..dump_
+00001690: 7769 7468 6f75 745f 6173 7369 676e 6d65  without_assignme
+000016a0: 6e74 7210 0000 0072 5e00 0000 7a03 2f2f  ntr....r^...z.//
+000016b0: 207a 040a 2f2f 207a 020a 0a72 1400 0000   z..// z...r....
+000016c0: 2911 7272 0000 0072 3c00 0000 7234 0000  ).rr...r<...r4..
+000016d0: 0072 2700 0000 7228 0000 0072 4000 0000  .r'...r(...r@...
+000016e0: 7273 0000 00da 0768 6173 6174 7472 7280  rs.....hasattrr.
+000016f0: 0000 0072 3100 0000 7233 0000 0072 8100  ...r1...r3...r..
+00001700: 0000 723b 0000 0072 4c00 0000 724f 0000  ..r;...rL...rO..
+00001710: 00da 0772 6570 6c61 6365 7274 0000 0029  ...replacert...)
+00001720: 0b72 4400 0000 7277 0000 005a 0474 6d70  .rD...rw...Z.tmp
+00001730: 3172 3600 0000 da04 6e6f 6465 720a 0000  1r6.....noder...
+00001740: 00da 0a6e 756d 5f73 7061 6365 73da 0963  ...num_spaces..c
+00001750: 6f64 655f 6e6f 6465 5a0b 6e6f 6465 5f64  ode_nodeZ.node_d
+00001760: 756d 7065 64da 0763 6f6d 6d65 6e74 721e  umped..commentr.
+00001770: 0000 0072 2100 0000 7221 0000 0072 2200  ...r!...r!...r".
+00001780: 0000 7280 0000 00bd 0000 0073 4800 0000  ..r........sH...
+00001790: 0401 0a01 0601 1201 1001 1c01 0a01 1001  ................
+000017a0: 0e02 1201 0a01 0801 1202 0801 0280 0801  ................
+000017b0: 0801 0a02 0a01 0402 0801 0601 1602 1201  ................
+000017c0: 1401 0a01 0a01 1001 0c01 0c01 0a01 0a01  ................
+000017d0: 0e01 0c01 0801 0401 7a12 466f 616d 496e  ........z.FoamIn
+000017e0: 7075 7446 696c 652e 6475 6d70 6301 0000  putFile.dumpc...
+000017f0: 0000 0000 0000 0000 0002 0000 0008 0000  ................
+00001800: 0043 0000 0073 5200 0000 7c00 6a00 6400  .C...sR...|.j.d.
+00001810: 7500 7209 7401 6401 8301 8201 7402 7c00  u.r.t.d.....t.|.
+00001820: 6a00 6402 8302 8f10 7d01 7c01 a003 7c00  j.d.....}.|...|.
+00001830: a004 a100 a101 0100 5700 6400 0400 0400  ........W.d.....
+00001840: 8303 0100 6400 5300 3100 7322 7701 0100  ....d.S.1.s"w...
+00001850: 0100 0100 5900 0100 6400 5300 2903 4e7a  ....Y...d.S.).Nz
+00001860: 1173 656c 662e 7061 7468 2069 7320 4e6f  .self.path is No
+00001870: 6e65 da01 7729 0572 7500 0000 723d 0000  ne..w).ru...r=..
+00001880: 00da 046f 7065 6eda 0577 7269 7465 7280  ...open..writer.
+00001890: 0000 0029 0272 4400 0000 da04 6669 6c65  ...).rD.....file
+000018a0: 7221 0000 0072 2100 0000 7222 0000 00da  r!...r!...r"....
+000018b0: 096f 7665 7277 7269 7465 e700 0000 730a  .overwrite....s.
+000018c0: 0000 000a 0108 010e 0110 0122 ff7a 1746  ...........".z.F
+000018d0: 6f61 6d49 6e70 7574 4669 6c65 2e6f 7665  oamInputFile.ove
+000018e0: 7277 7269 7465 6303 0000 0000 0000 0000  rwritec.........
+000018f0: 0000 0003 0000 0003 0000 0043 0000 00f3  ...........C....
+00001900: 0e00 0000 7c02 7c00 6a00 7c01 3c00 6400  ....|.|.j.|.<.d.
+00001910: 5300 7230 0000 00a9 0172 7300 0000 7270  S.r0.....rs...rp
+00001920: 0000 0072 2100 0000 7221 0000 0072 2200  ...r!...r!...r".
+00001930: 0000 7256 0000 00ed 0000 00f3 0200 0000  ..rV............
+00001940: 0e01 7a17 466f 616d 496e 7075 7446 696c  ..z.FoamInputFil
+00001950: 652e 5f73 6574 5f69 7465 6d63 0300 0000  e._set_itemc....
+00001960: 0000 0000 0000 0000 0300 0000 0300 0000  ................
+00001970: 4300 0000 728d 0000 0072 3000 0000 728e  C...r....r0...r.
+00001980: 0000 0029 0372 4400 0000 7236 0000 00da  ...).rD...r6....
+00001990: 0469 7465 6d72 2100 0000 7221 0000 0072  .itemr!...r!...r
+000019a0: 2200 0000 da0b 5f5f 7365 7469 7465 6d5f  ".....__setitem_
+000019b0: 5ff0 0000 0072 8f00 0000 7a19 466f 616d  _....r....z.Foam
+000019c0: 496e 7075 7446 696c 652e 5f5f 7365 7469  InputFile.__seti
+000019d0: 7465 6d5f 5f63 0200 0000 0000 0000 0000  tem__c..........
+000019e0: 0000 0200 0000 0200 0000 4300 0000 730a  ..........C...s.
+000019f0: 0000 007c 006a 007c 0119 0053 0072 3000  ...|.j.|...S.r0.
+00001a00: 0000 728e 0000 0029 0272 4400 0000 7236  ..r....).rD...r6
+00001a10: 0000 0072 2100 0000 7221 0000 0072 2200  ...r!...r!...r".
+00001a20: 0000 da0b 5f5f 6765 7469 7465 6d5f 5ff3  ....__getitem__.
+00001a30: 0000 00f3 0200 0000 0a01 7a19 466f 616d  ..........z.Foam
+00001a40: 496e 7075 7446 696c 652e 5f5f 6765 7469  InputFile.__geti
+00001a50: 7465 6d5f 5fa9 034e 4e4e 290a 7247 0000  tem__..NNN).rG..
+00001a60: 0072 4800 0000 7249 0000 0072 7600 0000  .rH...rI...rv...
+00001a70: 7278 0000 0072 8000 0000 728c 0000 0072  rx...r....r....r
+00001a80: 5600 0000 7291 0000 0072 9200 0000 7221  V...r....r....r!
+00001a90: 0000 0072 2100 0000 7221 0000 0072 2200  ...r!...r!...r".
+00001aa0: 0000 7271 0000 00ac 0000 0073 1000 0000  ..rq.......s....
+00001ab0: 0800 0a01 0809 0807 082a 0806 0803 0c03  .........*......
+00001ac0: 7271 0000 0063 0000 0000 0000 0000 0000  rq...c..........
+00001ad0: 0000 0000 0000 0300 0000 4000 0000 7328  ..........@...s(
+00001ae0: 0000 0065 005a 0164 005a 0255 0065 0365  ...e.Z.d.Z.U.e.e
+00001af0: 0464 013c 0065 0565 0464 023c 0064 0764  .d.<.e.e.d.<.d.d
+00001b00: 0464 0584 015a 0664 0653 0029 08da 0a41  .d...Z.d.S.)...A
+00001b10: 7373 6967 6e6d 656e 7472 4d00 0000 7237  ssignmentrM...r7
+00001b20: 0000 0072 0100 0000 6302 0000 0000 0000  ...r....c.......
+00001b30: 0000 0000 0002 0000 0005 0000 0043 0000  .............C..
+00001b40: 0073 3400 0000 7400 7c00 6a01 6401 8302  .s4...t.|.j.d...
+00001b50: 720c 7c00 6a01 a002 7c01 a101 5300 7c01  r.|.j...|...S.|.
+00001b60: 6402 1400 7c00 6a03 9b00 6403 7c00 6a01  d...|.j...d.|.j.
+00001b70: 9b00 6404 9d04 1700 5300 a905 4e72 8000  ..d.....S...Nr..
+00001b80: 0000 727a 0000 00fa 0220 2072 7c00 0000  ..rz.....  r|...
+00001b90: 2904 7282 0000 0072 3700 0000 7280 0000  ).r....r7...r...
+00001ba0: 0072 4d00 0000 a902 7244 0000 00da 0669  .rM.....rD.....i
+00001bb0: 6e64 656e 7472 2100 0000 7221 0000 0072  ndentr!...r!...r
+00001bc0: 2200 0000 7280 0000 00fc 0000 0073 0600  "...r........s..
+00001bd0: 0000 0c01 0c01 1c02 7a0f 4173 7369 676e  ........z.Assign
+00001be0: 6d65 6e74 2e64 756d 704e a901 7201 0000  ment.dumpN..r...
+00001bf0: 0029 0772 4700 0000 7248 0000 0072 4900  .).rG...rH...rI.
+00001c00: 0000 724f 0000 00da 0f5f 5f61 6e6e 6f74  ..rO.....__annot
+00001c10: 6174 696f 6e73 5f5f da06 6f62 6a65 6374  ations__..object
+00001c20: 7280 0000 0072 2100 0000 7221 0000 0072  r....r!...r!...r
+00001c30: 2100 0000 7222 0000 0072 9500 0000 f700  !...r"...r......
+00001c40: 0000 7308 0000 000a 0008 0208 010e 0272  ..s............r
+00001c50: 9500 0000 6300 0000 0000 0000 0000 0000  ....c...........
+00001c60: 0000 0000 0003 0000 0000 0000 0073 2600  .............s&.
+00001c70: 0000 6500 5a01 6400 5a02 8700 6601 6401  ..e.Z.d.Z...f.d.
+00001c80: 6402 8408 5a03 6406 6404 6405 8401 5a04  d...Z.d.d.d...Z.
+00001c90: 8700 0400 5a05 5300 2907 da12 5661 7269  ....Z.S.)...Vari
+00001ca0: 6162 6c65 4173 7369 676e 6d65 6e74 6301  ableAssignmentc.
+00001cb0: 0000 0000 0000 0000 0000 0002 0000 0002  ................
+00001cc0: 0000 0003 0000 0073 0e00 0000 7400 8300  .......s....t...
+00001cd0: a001 a100 7d01 7c01 5300 7230 0000 00a9  ....}.|.S.r0....
+00001ce0: 02da 0573 7570 6572 7278 0000 0029 0272  ...superrx...).r
+00001cf0: 4400 0000 720a 0000 00a9 01da 095f 5f63  D...r........__c
+00001d00: 6c61 7373 5f5f 7221 0000 0072 2200 0000  lass__r!...r"...
+00001d10: 7278 0000 0004 0100 0073 0400 0000 0a01  rx.......s......
+00001d20: 0401 7a1b 5661 7269 6162 6c65 4173 7369  ..z.VariableAssi
+00001d30: 676e 6d65 6e74 2e5f 5f72 6570 725f 5f72  gnment.__repr__r
+00001d40: 0100 0000 6302 0000 0000 0000 0000 0000  ....c...........
+00001d50: 0002 0000 0006 0000 0043 0000 0073 4a00  .........C...sJ.
+00001d60: 0000 7400 7c00 6a01 6401 8302 7217 7c01  ..t.|.j.d...r.|.
+00001d70: 6402 1400 7c00 6a02 9b00 6403 7c00 6a01  d...|.j...d.|.j.
+00001d80: a003 7c01 a101 9b00 6404 9d04 1700 5300  ..|.....d.....S.
+00001d90: 7c01 6402 1400 7c00 6a02 9b00 6403 7c00  |.d...|.j...d.|.
+00001da0: 6a01 9b00 6404 9d04 1700 5300 7296 0000  j...d.....S.r...
+00001db0: 0029 0472 8200 0000 7237 0000 0072 4d00  .).r....r7...rM.
+00001dc0: 0000 7280 0000 0072 9800 0000 7221 0000  ..r....r....r!..
+00001dd0: 0072 2100 0000 7222 0000 0072 8000 0000  .r!...r"...r....
+00001de0: 0801 0000 7306 0000 000c 0122 011c 027a  ....s......"...z
+00001df0: 1756 6172 6961 626c 6541 7373 6967 6e6d  .VariableAssignm
+00001e00: 656e 742e 6475 6d70 729a 0000 0029 0672  ent.dumpr....).r
+00001e10: 4700 0000 7248 0000 0072 4900 0000 7278  G...rH...rI...rx
+00001e20: 0000 0072 8000 0000 da0d 5f5f 636c 6173  ...r......__clas
+00001e30: 7363 656c 6c5f 5f72 2100 0000 7221 0000  scell__r!...r!..
+00001e40: 0072 a000 0000 7222 0000 0072 9d00 0000  .r....r"...r....
+00001e50: 0301 0000 7306 0000 0008 000c 0112 0472  ....s..........r
+00001e60: 9d00 0000 6300 0000 0000 0000 0000 0000  ....c...........
+00001e70: 0000 0000 0003 0000 0040 0000 00f3 2800  .........@....(.
+00001e80: 0000 6500 5a01 6400 5a02 6409 6402 6403  ..e.Z.d.Z.d.d.d.
+00001e90: 8401 5a03 6404 6405 8400 5a04 640a 6407  ..Z.d.d...Z.d.d.
+00001ea0: 6408 8401 5a05 6401 5300 290b 726f 0000  d...Z.d.S.).ro..
+00001eb0: 004e 6304 0000 0000 0000 0000 0000 0004  .Nc.............
+00001ec0: 0000 0004 0000 0043 0000 0073 2c00 0000  .......C...s,...
+00001ed0: 7c01 7c00 5f00 7c02 7c00 5f01 7402 7c03  |.|._.|.|._.t.|.
+00001ee0: 7403 7404 6602 8302 7211 7405 7c03 8301  t.t.f...r.t.|...
+00001ef0: 7d03 7c03 7c00 5f06 6400 5300 7230 0000  }.|.|._.d.S.r0..
+00001f00: 0029 0772 3700 0000 724d 0000 0072 3100  .).r7...rM...r1.
+00001f10: 0000 7251 0000 00da 0574 7570 6c65 722e  ..rQ.....tupler.
+00001f20: 0000 0072 5800 0000 2904 7244 0000 0072  ...rX...).rD...r
+00001f30: 3700 0000 724d 0000 0072 5800 0000 7221  7...rM...rX...r!
+00001f40: 0000 0072 2100 0000 7222 0000 0072 7600  ...r!...r"...rv.
+00001f50: 0000 1101 0000 730a 0000 0006 0106 010e  ......s.........
+00001f60: 0108 010a 017a 0e56 616c 7565 2e5f 5f69  .....z.Value.__i
+00001f70: 6e69 745f 5f63 0100 0000 0000 0000 0000  nit__c..........
+00001f80: 0000 0100 0000 0700 0000 4300 0000 7394  ..........C...s.
+00001f90: 0000 007c 006a 0064 0075 0172 197c 006a  ...|.j.d.u.r.|.j
+00001fa0: 0164 0075 0172 1964 017c 006a 029b 0064  .d.u.r.d.|.j...d
+00001fb0: 027c 006a 019b 0064 037c 006a 009b 0064  .|.j...d.|.j...d
+00001fc0: 049d 0753 007c 006a 0064 0075 0072 2e7c  ...S.|.j.d.u.r.|
+00001fd0: 006a 0164 0075 0172 2e64 017c 006a 029b  .j.d.u.r.d.|.j..
+00001fe0: 0064 027c 006a 019b 0064 049d 0553 007c  .d.|.j...d...S.|
+00001ff0: 006a 0064 0075 0172 437c 006a 0164 0075  .j.d.u.rC|.j.d.u
+00002000: 0072 4364 017c 006a 029b 0064 057c 006a  .rCd.|.j...d.|.j
+00002010: 009b 0064 049d 0553 0064 017c 006a 029b  ...d...S.d.|.j..
+00002020: 0064 069d 0353 0029 074e 7a06 5661 6c75  .d...S.).Nz.Valu
+00002030: 6528 7a08 2c20 6e61 6d65 3d22 7a0e 222c  e(z., name="z.",
+00002040: 2064 696d 656e 7369 6f6e 3d22 7a02 2229   dimension="z.")
+00002050: 7a0d 2c20 6469 6d65 6e73 696f 6e3d 22fa  z., dimension=".
+00002060: 0129 2903 7258 0000 0072 4d00 0000 7237  .)).rX...rM...r7
+00002070: 0000 00a9 0172 4400 0000 7221 0000 0072  .....rD...r!...r
+00002080: 2100 0000 7222 0000 0072 7800 0000 1801  !...r"...rx.....
+00002090: 0000 730e 0000 0014 011e 0114 0116 0114  ..s.............
+000020a0: 0116 010e 027a 0e56 616c 7565 2e5f 5f72  .....z.Value.__r
+000020b0: 6570 725f 5f72 0100 0000 6302 0000 0000  epr__r....c.....
+000020c0: 0000 0000 0000 0005 0000 0005 0000 0043  ...............C
+000020d0: 0000 0073 ce00 0000 7c00 6a00 6400 7501  ...s....|.j.d.u.
+000020e0: 7214 7401 7c00 6a00 8301 7d02 6401 a002  r.t.|.j...}.d...
+000020f0: 6402 6403 8400 7c02 4400 8301 a101 7d03  d.d...|.D.....}.
+00002100: 7403 7c00 6a04 7405 8302 7226 7406 7c00  t.|.j.t...r&t.|.
+00002110: 6a04 6404 8302 7226 7c00 6a04 a007 a100  j.d...r&|.j.....
+00002120: 7d04 6e05 7408 7c00 6a04 8301 7d04 7c00  }.n.t.|.j...}.|.
+00002130: 6a00 6400 7501 7240 7c00 6a09 6400 7501  j.d.u.r@|.j.d.u.
+00002140: 7240 7c00 6a09 9b00 6405 7c03 9b00 6406  r@|.j...d.|...d.
+00002150: 7c04 9b00 9d05 5300 7c00 6a00 6400 7500  |.....S.|.j.d.u.
+00002160: 7252 7c00 6a09 6400 7501 7252 7c00 6a09  rR|.j.d.u.rR|.j.
+00002170: 9b00 6401 7c04 9b00 9d03 5300 7c00 6a00  ..d.|.....S.|.j.
+00002180: 6400 7501 7264 7c00 6a09 6400 7500 7264  d.u.rd|.j.d.u.rd
+00002190: 6407 7c03 9b00 6406 7c04 9b00 9d04 5300  d.|...d.|.....S.
+000021a0: 7c04 9b00 5300 2908 4e72 7a00 0000 6301  |...S.).Nrz...c.
+000021b0: 0000 0000 0000 0000 0000 0002 0000 0003  ................
+000021c0: 0000 0073 0000 00f3 1800 0000 8100 7c00  ...s..........|.
+000021d0: 5d07 7d01 7400 7c01 8301 5600 0100 7102  ].}.t.|...V...q.
+000021e0: 6400 5300 7230 0000 00a9 0172 4f00 0000  d.S.r0.....rO...
+000021f0: a902 7235 0000 00da 066e 756d 6265 7272  ..r5.....numberr
+00002200: 2100 0000 7221 0000 0072 2200 0000 7238  !...r!...r"...r8
+00002210: 0000 0025 0100 00f3 0400 0000 0280 1600  ...%............
+00002220: 7a30 5661 6c75 652e 6475 6d70 5f77 6974  z0Value.dump_wit
+00002230: 686f 7574 5f61 7373 6967 6e6d 656e 742e  hout_assignment.
+00002240: 3c6c 6f63 616c 733e 2e3c 6765 6e65 7870  <locals>.<genexp
+00002250: 723e 7280 0000 007a 0220 5b7a 025d 20fa  r>r....z. [z.] .
+00002260: 015b 290a 7258 0000 0072 2300 0000 7228  .[).rX...r#...r(
+00002270: 0000 0072 3100 0000 7237 0000 0072 4100  ...r1...r7...rA.
+00002280: 0000 7282 0000 0072 8000 0000 724f 0000  ..r....r....rO..
+00002290: 0072 4d00 0000 2905 7244 0000 0072 9900  .rM...).rD...r..
+000022a0: 0000 5a0e 6469 6d65 6e73 696f 6e5f 6c69  ..Z.dimension_li
+000022b0: 7374 5a10 6469 6d65 6e73 696f 6e5f 6475  stZ.dimension_du
+000022c0: 6d70 6564 5a0c 7661 6c75 655f 6475 6d70  mpedZ.value_dump
+000022d0: 6564 7221 0000 0072 2100 0000 7222 0000  edr!...r!...r"..
+000022e0: 0072 8100 0000 2201 0000 731a 0000 000a  .r...."...s.....
+000022f0: 010a 0114 0118 020c 010a 0214 0216 0114  ................
+00002300: 0110 0114 0110 0106 027a 1d56 616c 7565  .........z.Value
+00002310: 2e64 756d 705f 7769 7468 6f75 745f 6173  .dump_without_as
+00002320: 7369 676e 6d65 6e74 2902 4e4e 729a 0000  signment).NNr...
+00002330: 0029 0672 4700 0000 7248 0000 0072 4900  .).rG...rH...rI.
+00002340: 0000 7276 0000 0072 7800 0000 7281 0000  ..rv...rx...r...
+00002350: 0072 2100 0000 7221 0000 0072 2100 0000  .r!...r!...r!...
+00002360: 7222 0000 0072 6f00 0000 0f01 0000 7308  r"...ro.......s.
+00002370: 0000 0008 000a 0208 070e 0a72 6f00 0000  ...........ro...
+00002380: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+00002390: 0003 0000 0000 0000 0073 2e00 0000 6500  .........s....e.
+000023a0: 5a01 6400 5a02 8700 6601 6401 6402 8408  Z.d.Z...f.d.d...
+000023b0: 5a03 6403 6404 8400 5a04 6408 6406 6407  Z.d.d...Z.d.d.d.
+000023c0: 8401 5a05 8700 0400 5a06 5300 2909 7269  ..Z.....Z.S.).ri
+000023d0: 0000 0063 0200 0000 0000 0000 0000 0000  ...c............
+000023e0: 0200 0000 0300 0000 0300 0000 733c 0000  ............s<..
+000023f0: 0074 007c 0174 0183 0272 0974 027c 0183  .t.|.t...r.t.|..
+00002400: 017d 0174 0364 0164 0284 007c 0144 0083  .}.t.d.d...|.D..
+00002410: 0183 0173 1674 0464 0383 0182 0174 0583  ...s.t.d.....t..
+00002420: 00a0 067c 01a1 0101 0064 0053 0029 044e  ...|.....d.S.).N
+00002430: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
+00002440: 0004 0000 0073 0000 0072 5a00 0000 7230  .....s...rZ...r0
+00002450: 0000 0029 0272 3100 0000 721a 0000 0029  ...).r1...r....)
+00002460: 0272 3500 0000 da04 656c 656d 7221 0000  .r5.....elemr!..
+00002470: 0072 2100 0000 7222 0000 0072 3800 0000  .r!...r"...r8...
+00002480: 3a01 0000 725c 0000 007a 2844 696d 656e  :...r\...z(Dimen
+00002490: 7369 6f6e 5365 742e 5f5f 696e 6974 5f5f  sionSet.__init__
+000024a0: 2e3c 6c6f 6361 6c73 3e2e 3c67 656e 6578  .<locals>.<genex
+000024b0: 7072 3e7a 1342 6164 207b 666f 616d 5f75  pr>z.Bad {foam_u
+000024c0: 6e69 7473 203d 207d 2907 7231 0000 0072  nits = }).r1...r
+000024d0: 4f00 0000 7223 0000 0072 6600 0000 723d  O...r#...rf...r=
+000024e0: 0000 0072 9f00 0000 7276 0000 0029 0272  ...r....rv...).r
+000024f0: 4400 0000 722a 0000 0072 a000 0000 7221  D...r*...r....r!
+00002500: 0000 0072 2200 0000 7276 0000 0037 0100  ...r"...rv...7..
+00002510: 0073 0a00 0000 0a01 0801 1201 0801 1001  .s..............
+00002520: 7a15 4469 6d65 6e73 696f 6e53 6574 2e5f  z.DimensionSet._
+00002530: 5f69 6e69 745f 5f63 0100 0000 0000 0000  _init__c........
+00002540: 0000 0000 0100 0000 0200 0000 4300 0000  ............C...
+00002550: 7308 0000 0074 007c 0083 0153 0072 3000  s....t.|...S.r0.
+00002560: 0000 2901 722e 0000 0072 a600 0000 7221  ..).r....r....r!
+00002570: 0000 0072 2100 0000 7222 0000 0072 7800  ...r!...r"...rx.
+00002580: 0000 3e01 0000 f302 0000 0008 017a 1544  ..>..........z.D
+00002590: 696d 656e 7369 6f6e 5365 742e 5f5f 7265  imensionSet.__re
+000025a0: 7072 5f5f 7201 0000 0063 0200 0000 0000  pr__r....c......
+000025b0: 0000 0000 0000 0200 0000 0500 0000 4300  ..............C.
+000025c0: 0000 731c 0000 0064 0164 02a0 0064 0364  ..s....d.d...d.d
+000025d0: 0484 007c 0044 0083 01a1 0117 0064 0517  ...|.D.......d..
+000025e0: 0053 0029 064e 72ac 0000 0072 7a00 0000  .S.).Nr....rz...
+000025f0: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
+00002600: 0003 0000 0073 0000 0072 a700 0000 7230  .....s...r....r0
+00002610: 0000 0072 a800 0000 72a9 0000 0072 2100  ...r....r....r!.
+00002620: 0000 7221 0000 0072 2200 0000 7238 0000  ..r!...r"...r8..
+00002630: 0042 0100 0072 ab00 0000 7a37 4469 6d65  .B...r....z7Dime
+00002640: 6e73 696f 6e53 6574 2e64 756d 705f 7769  nsionSet.dump_wi
+00002650: 7468 6f75 745f 6173 7369 676e 6d65 6e74  thout_assignment
+00002660: 2e3c 6c6f 6361 6c73 3e2e 3c67 656e 6578  .<locals>.<genex
+00002670: 7072 3efa 015d a901 7228 0000 0072 9800  pr>..]..r(...r..
+00002680: 0000 7221 0000 0072 2100 0000 7222 0000  ..r!...r!...r"..
+00002690: 0072 8100 0000 4101 0000 f302 0000 001c  .r....A.........
+000026a0: 017a 2444 696d 656e 7369 6f6e 5365 742e  .z$DimensionSet.
+000026b0: 6475 6d70 5f77 6974 686f 7574 5f61 7373  dump_without_ass
+000026c0: 6967 6e6d 656e 7472 9a00 0000 2907 7247  ignmentr....).rG
+000026d0: 0000 0072 4800 0000 7249 0000 0072 7600  ...rH...rI...rv.
+000026e0: 0000 7278 0000 0072 8100 0000 72a2 0000  ..rx...r....r...
+000026f0: 0072 2100 0000 7221 0000 0072 a000 0000  .r!...r!...r....
+00002700: 7222 0000 0072 6900 0000 3601 0000 7308  r"...ri...6...s.
+00002710: 0000 0008 000c 0108 0712 0372 6900 0000  ...........ri...
+00002720: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+00002730: 0004 0000 0000 0000 0073 4400 0000 6500  .........sD...e.
+00002740: 5a01 6400 5a02 640d 8700 6601 6402 6403  Z.d.Z.d...f.d.d.
+00002750: 8409 5a03 6404 6405 8400 5a04 8700 6601  ..Z.d.d...Z...f.
+00002760: 6406 6407 8408 5a05 640e 6409 640a 8401  d.d...Z.d.d.d...
+00002770: 5a06 640b 640c 8400 5a07 8700 0400 5a08  Z.d.d...Z.....Z.
+00002780: 5300 290f 7232 0000 004e 6305 0000 0000  S.).r2...Nc.....
+00002790: 0000 0000 0000 0005 0000 0004 0000 0003  ................
+000027a0: 0000 0073 2800 0000 7c02 7c00 5f00 7c03  ...s(...|.|._.|.
+000027b0: 7c00 5f01 7c04 7c00 5f02 7403 8300 6a04  |._.|.|._.t...j.
+000027c0: 6401 6900 7c01 a401 8e01 0100 6400 5300  d.i.|.......d.S.
+000027d0: 2902 4e72 2100 0000 2905 da05 5f6e 616d  ).Nr!...)..._nam
+000027e0: 65da 0a5f 6469 7265 6374 6976 6572 4c00  e.._directiverL.
+000027f0: 0000 729f 0000 0072 7600 0000 2905 7244  ..r....rv...).rD
+00002800: 0000 0072 3e00 0000 724d 0000 00da 0964  ...r>...rM.....d
+00002810: 6972 6563 7469 7665 724c 0000 0072 a000  irectiverL...r..
+00002820: 0000 7221 0000 0072 2200 0000 7276 0000  ..r!...r"...rv..
+00002830: 0046 0100 0073 0800 0000 0601 0601 0601  .F...s..........
+00002840: 1601 7a0d 4469 6374 2e5f 5f69 6e69 745f  ..z.Dict.__init_
+00002850: 5f63 0100 0000 0000 0000 0000 0000 0100  _c..............
+00002860: 0000 0100 0000 4300 0000 f306 0000 007c  ......C........|
+00002870: 006a 0053 0072 3000 0000 a901 72b2 0000  .j.S.r0.....r...
+00002880: 0072 a600 0000 7221 0000 0072 2100 0000  .r....r!...r!...
+00002890: 7222 0000 00da 0867 6574 5f6e 616d 654c  r".....get_nameL
+000028a0: 0100 00f3 0200 0000 0601 7a0d 4469 6374  ..........z.Dict
+000028b0: 2e67 6574 5f6e 616d 6563 0100 0000 0000  .get_namec......
+000028c0: 0000 0000 0000 0100 0000 0200 0000 0300  ................
+000028d0: 0000 f30a 0000 0074 0083 00a0 01a1 0053  .......t.......S
+000028e0: 0072 3000 0000 729e 0000 0072 a600 0000  .r0...r....r....
+000028f0: 72a0 0000 0072 2100 0000 7222 0000 0072  r....r!...r"...r
+00002900: 7800 0000 4f01 0000 7293 0000 007a 0d44  x...O...r....z.D
+00002910: 6963 742e 5f5f 7265 7072 5f5f 7201 0000  ict.__repr__r...
+00002920: 0063 0200 0000 0000 0000 0000 0000 0b00  .c..............
+00002930: 0000 0900 0000 4300 0000 7372 0100 0067  ......C...sr...g
+00002940: 007d 027c 0164 0114 007d 037c 006a 0064  .}.|.d...}.|.j.d
+00002950: 0075 0172 287c 037c 006a 0017 007d 047c  .u.r(|.|.j...}.|
+00002960: 006a 0164 0075 0172 1c7c 0464 027c 006a  .j.d.u.r.|.d.|.j
+00002970: 0117 0037 007d 047c 02a0 027c 0464 037c  ...7.}.|...|.d.|
+00002980: 039b 009d 0217 0064 0417 00a1 0101 0074  .......d.......t
+00002990: 037c 0083 017d 057c 00a0 04a1 0044 005d  .|...}.|.....D.]
+000029a0: 6f5c 027d 067d 077c 006a 0564 0075 0172  o\.}.}.|.j.d.u.r
+000029b0: 537c 067c 006a 0576 0072 537c 006a 057c  S|.|.j.v.rS|.j.|
+000029c0: 0619 007d 0874 067c 0874 0783 0272 537c  ...}.t.|.t...rS|
+000029d0: 02a0 0264 057c 08a0 0864 0364 06a1 0217  ...d.|...d.d....
+000029e0: 00a1 0101 0074 097c 0764 0783 0272 637c  .....t.|.d...rc|
+000029f0: 02a0 027c 07a0 0a7c 0164 0817 00a1 01a1  ...|...|.d......
+00002a00: 0101 0071 307c 0764 0075 0072 727c 02a0  ...q0|.d.u.rr|..
+00002a10: 027c 0364 097c 069b 009d 0217 00a1 0101  .|.d.|..........
+00002a20: 0071 3074 097c 0764 0a83 0272 7c7c 07a0  .q0t.|.d...r||..
+00002a30: 0ba1 007d 096e 027c 077d 097c 0764 0b6b  ...}.n.|.}.|.d.k
+00002a40: 0272 8564 0b7d 0a6e 0b74 0c64 0c7c 0574  .r.d.}.n.t.d.|.t
+00002a50: 0d7c 0683 0118 0083 0264 0114 007d 0a7c  .|.......d...}.|
+00002a60: 02a0 027c 0364 097c 069b 007c 0a9b 007c  ...|.d.|...|...|
+00002a70: 099b 0064 0d9d 0517 00a1 0101 0071 307c  ...d.........q0|
+00002a80: 02a0 027c 0364 0e17 00a1 0101 0074 067c  ...|.d.......t.|
+00002a90: 0074 0e83 0272 b47c 0264 0f05 0019 0064  .t...r.|.d.....d
+00002aa0: 0d37 0003 003c 0064 03a0 0f7c 02a1 0153  .7...<.d...|...S
+00002ab0: 0029 104e 727a 0000 0072 9700 0000 727e  .).Nrz...r....r~
+00002ac0: 0000 00da 017b 7a07 2020 2020 2f2f 207a  .....{z.    // z
+00002ad0: 080a 2020 2020 2f2f 2072 8000 0000 7239  ..    // r....r9
+00002ae0: 0000 0072 7b00 0000 7281 0000 0072 1000  ...r{...r....r..
+00002af0: 0000 725e 0000 0072 7c00 0000 727d 0000  ..r^...r|...r}..
+00002b00: 0072 1400 0000 2910 72b2 0000 0072 b300  .r....).r....r..
+00002b10: 0000 7227 0000 0072 4000 0000 723c 0000  ..r'...r@...r<..
+00002b20: 0072 4c00 0000 7231 0000 0072 4f00 0000  .rL...r1...rO...
+00002b30: 7283 0000 0072 8200 0000 7280 0000 0072  r....r....r....r
+00002b40: 8100 0000 723b 0000 0072 3400 0000 da0a  ....r;...r4.....
+00002b50: 436f 6465 5374 7265 616d 7228 0000 0029  CodeStreamr(...)
+00002b60: 0b72 4400 0000 7299 0000 0072 7700 0000  .rD...r....rw...
+00002b70: da0b 696e 6465 6e74 6174 696f 6eda 046c  ..indentation..l
+00002b80: 696e 6572 8500 0000 7236 0000 0072 8400  iner....r6...r..
+00002b90: 0000 7287 0000 0072 8600 0000 720a 0000  ..r....r....r...
+00002ba0: 0072 2100 0000 7221 0000 0072 2200 0000  .r!...r!...r"...
+00002bb0: 7280 0000 0052 0100 0073 3800 0000 0401  r....R...s8.....
+00002bc0: 0801 0a01 0a01 0a01 0e01 1801 0802 1001  ................
+00002bd0: 1401 0a01 0a01 1601 0a02 1601 0801 1601  ................
+00002be0: 0a02 0a01 0402 0801 0601 1602 2001 0e01  ............ ...
+00002bf0: 0a03 1001 0a02 7a09 4469 6374 2e64 756d  ......z.Dict.dum
+00002c00: 7063 0300 0000 0000 0000 0000 0000 0300  pc..............
+00002c10: 0000 0300 0000 4300 0000 730c 0000 007c  ......C...s....|
+00002c20: 027c 007c 013c 0064 0053 0072 3000 0000  .|.|.<.d.S.r0...
+00002c30: 7221 0000 0072 7000 0000 7221 0000 0072  r!...rp...r!...r
+00002c40: 2100 0000 7222 0000 0072 5600 0000 7801  !...r"...rV...x.
+00002c50: 0000 7302 0000 000c 017a 0e44 6963 742e  ..s......z.Dict.
+00002c60: 5f73 6574 5f69 7465 6d72 9400 0000 729a  _set_itemr....r.
+00002c70: 0000 0029 0972 4700 0000 7248 0000 0072  ...).rG...rH...r
+00002c80: 4900 0000 7276 0000 0072 b700 0000 7278  I...rv...r....rx
+00002c90: 0000 0072 8000 0000 7256 0000 0072 a200  ...r....rV...r..
+00002ca0: 0000 7221 0000 0072 2100 0000 72a0 0000  ..r!...r!...r...
+00002cb0: 0072 2200 0000 7232 0000 0045 0100 0073  .r"...r2...E...s
+00002cc0: 0c00 0000 0800 0e01 0806 0c03 0a03 1026  ...............&
+00002cd0: 7232 0000 0063 0000 0000 0000 0000 0000  r2...c..........
+00002ce0: 0000 0000 0000 0400 0000 0000 0000 735a  ..............sZ
+00002cf0: 0000 0065 005a 0164 005a 0264 015a 0364  ...e.Z.d.Z.d.Z.d
+00002d00: 1287 0066 0164 0364 0484 095a 0464 0564  ...f.d.d...Z.d.d
+00002d10: 0684 005a 0564 0764 0884 005a 0687 0066  ...Z.d.d...Z...f
+00002d20: 0164 0964 0a84 085a 0764 0b64 0c84 005a  .d.d...Z.d.d...Z
+00002d30: 0864 1364 0e64 0f84 015a 0964 1364 1064  .d.d.d...Z.d.d.d
+00002d40: 1184 015a 0a87 0004 005a 0b53 0029 1472  ...Z.....Z.S.).r
+00002d50: 3300 0000 7a1b 5265 7072 6573 656e 7473  3...z.Represents
+00002d60: 2061 6e20 4f70 656e 466f 616d 206c 6973   an OpenFoam lis
+00002d70: 744e 6304 0000 0000 0000 0000 0000 0004  tNc.............
+00002d80: 0000 0003 0000 0003 0000 0073 1c00 0000  ...........s....
+00002d90: 7c02 7c00 5f00 7c03 7c00 5f01 7402 8300  |.|._.|.|._.t...
+00002da0: a003 7c01 a101 0100 6400 5300 7230 0000  ..|.....d.S.r0..
+00002db0: 0029 0472 b200 0000 da06 5f64 7479 7065  .).r......_dtype
+00002dc0: 729f 0000 0072 7600 0000 2904 7244 0000  r....rv...).rD..
+00002dd0: 00da 0869 7465 7261 626c 6572 4d00 0000  ...iterablerM...
+00002de0: 7265 0000 0072 a000 0000 7221 0000 0072  re...r....r!...r
+00002df0: 2200 0000 7276 0000 007f 0100 0073 0600  "...rv.......s..
+00002e00: 0000 0601 0601 1001 7a0d 4c69 7374 2e5f  ........z.List._
+00002e10: 5f69 6e69 745f 5f63 0100 0000 0000 0000  _init__c........
+00002e20: 0000 0000 0100 0000 0100 0000 4300 0000  ............C...
+00002e30: 72b5 0000 0072 3000 0000 72b6 0000 0072  r....r0...r....r
+00002e40: a600 0000 7221 0000 0072 2100 0000 7222  ....r!...r!...r"
+00002e50: 0000 0072 b700 0000 8401 0000 72b8 0000  ...r........r...
+00002e60: 007a 0d4c 6973 742e 6765 745f 6e61 6d65  .z.List.get_name
+00002e70: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
+00002e80: 0003 0000 0043 0000 0073 4800 0000 7c00  .....C...sH...|.
+00002e90: 6a00 6400 7500 720a 7c01 7c00 5f00 6400  j.d.u.r.|.|._.d.
+00002ea0: 5300 7401 7c00 6a00 7402 8302 7221 7c00  S.t.|.j.t...r!|.
+00002eb0: 6a00 7c01 6b03 721f 7c01 6401 1700 7c00  j.|.k.r.|.d...|.
+00002ec0: 6a00 1700 7c00 5f00 6400 5300 6400 5300  j...|._.d.S.d.S.
+00002ed0: 7403 8300 8201 2902 4e72 7a00 0000 2904  t.....).Nrz...).
+00002ee0: 72b2 0000 0072 3100 0000 724f 0000 00da  r....r1...rO....
+00002ef0: 0c52 756e 7469 6d65 4572 726f 7229 0272  .RuntimeError).r
+00002f00: 4400 0000 724d 0000 0072 2100 0000 7221  D...rM...r!...r!
+00002f10: 0000 0072 2200 0000 da08 6164 645f 6e61  ...r".....add_na
+00002f20: 6d65 8701 0000 730e 0000 000a 010a 010c  me....s.........
+00002f30: 010a 0114 0104 ff06 037a 0d4c 6973 742e  .........z.List.
+00002f40: 6164 645f 6e61 6d65 6301 0000 0000 0000  add_namec.......
+00002f50: 0000 0000 0001 0000 0002 0000 0003 0000  ................
+00002f60: 0072 b900 0000 7230 0000 0072 9e00 0000  .r....r0...r....
+00002f70: 72a6 0000 0072 a000 0000 7221 0000 0072  r....r....r!...r
+00002f80: 2200 0000 7278 0000 0090 0100 0072 9300  "...rx.......r..
+00002f90: 0000 7a0d 4c69 7374 2e5f 5f72 6570 725f  ..z.List.__repr_
+00002fa0: 5f63 0200 0000 0000 0000 0000 0000 0200  _c..............
+00002fb0: 0000 0300 0000 0300 0000 7314 0000 0087  ..........s.....
+00002fc0: 0087 0166 0264 0164 0284 0888 0144 0083  ...f.d.d.....D..
+00002fd0: 0153 0029 034e 6301 0000 0000 0000 0000  .S.).Nc.........
+00002fe0: 0000 0002 0000 0006 0000 0013 0000 0073  ...............s
+00002ff0: 1800 0000 6700 7c00 5d08 7d01 8801 a000  ....g.|.].}.....
+00003000: 7c01 8800 a102 9102 7102 5300 7221 0000  |.......q.S.r!..
+00003010: 00a9 01da 0a5f 6475 6d70 5f69 7465 6d29  ....._dump_item)
+00003020: 0272 3500 0000 7290 0000 00a9 0272 9900  .r5...r......r..
+00003030: 0000 7244 0000 0072 2100 0000 7222 0000  ..rD...r!...r"..
+00003040: 0072 6300 0000 9401 0000 7302 0000 0018  .rc.......s.....
+00003050: 007a 2b4c 6973 742e 5f6d 616b 655f 6c69  .z+List._make_li
+00003060: 7374 5f73 7472 696e 6773 2e3c 6c6f 6361  st_strings.<loca
+00003070: 6c73 3e2e 3c6c 6973 7463 6f6d 703e 7221  ls>.<listcomp>r!
+00003080: 0000 0072 9800 0000 7221 0000 0072 c400  ...r....r!...r..
+00003090: 0000 7222 0000 00da 125f 6d61 6b65 5f6c  ..r"....._make_l
+000030a0: 6973 745f 7374 7269 6e67 7393 0100 0073  ist_strings....s
+000030b0: 0200 0000 1401 7a17 4c69 7374 2e5f 6d61  ......z.List._ma
+000030c0: 6b65 5f6c 6973 745f 7374 7269 6e67 7372  ke_list_stringsr
+000030d0: 0100 0000 6303 0000 0000 0000 0000 0000  ....c...........
+000030e0: 0003 0000 0004 0000 0043 0000 0073 3200  .........C...s2.
+000030f0: 0000 7400 7c01 7401 7402 6602 8302 7211  ..t.|.t.t.f...r.
+00003100: 7403 7c01 6401 8302 7211 7c01 a004 7c02  t.|.d...r.|...|.
+00003110: a101 5300 7c02 6402 1400 7405 7c01 8301  ..S.|.d...t.|...
+00003120: 1700 5300 2903 4e72 8000 0000 727a 0000  ..S.).Nr....rz..
+00003130: 0029 0672 3100 0000 7241 0000 0072 9500  .).r1...rA...r..
+00003140: 0000 7282 0000 0072 8000 0000 724f 0000  ..r....r....rO..
+00003150: 0029 0372 4400 0000 7290 0000 0072 9900  .).rD...r....r..
+00003160: 0000 7221 0000 0072 2100 0000 7222 0000  ..r!...r!...r"..
+00003170: 0072 c300 0000 9601 0000 7306 0000 0018  .r........s.....
+00003180: 010a 0110 027a 0f4c 6973 742e 5f64 756d  .....z.List._dum
+00003190: 705f 6974 656d 6302 0000 0000 0000 0000  p_itemc.........
+000031a0: 0000 000b 0000 0008 0000 0003 0000 0073  ...............s
+000031b0: 7001 0000 6700 7d02 8800 6401 1400 7d03  p...g.}...d...}.
+000031c0: 8801 6a00 6400 7500 721f 7c02 a001 8801  ..j.d.u.r.|.....
+000031d0: 6a02 6402 6403 8d01 a101 0100 7c03 6404  j.d.d.......|.d.
+000031e0: 1700 6401 a003 7c02 a101 1700 6405 1700  ..d...|.....d...
+000031f0: 5300 8801 6a00 7d04 8801 6a04 6400 7501  S...j.}...j.d.u.
+00003200: 7236 7c04 6406 8801 6a04 9b00 6407 7c03  r6|.d...j...d.|.
+00003210: 9b00 7405 8801 8301 9b00 9d05 3700 7d04  ..t.........7.}.
+00003220: 7c02 a006 7c03 7c04 1700 6408 7c03 9b00  |...|.|...d.|...
+00003230: 9d02 1700 6404 1700 a101 0100 6409 640a  ....d.......d.d.
+00003240: 640b 9c02 7d05 8801 6a00 7c05 a007 a100  d...}...j.|.....
+00003250: 7601 725e 7c02 a006 6408 a003 8801 a002  v.r^|...d.......
+00003260: 8800 640c 1700 a101 a101 a101 0100 6e4e  ..d...........nN
+00003270: 8801 72ac 7c05 8801 6a00 1900 7d06 8801  ..r.|...j...}...
+00003280: 6402 1900 7c06 7601 726f 7408 8801 8301  d...|.v.rot.....
+00003290: 8201 8801 6402 1900 7d07 6700 7d08 6400  ....d...}.g.}.d.
+000032a0: 7d09 8801 4400 5d18 7d0a 7c0a 7c07 6b02  }...D.].}.|.|.k.
+000032b0: 728c 7c09 6400 7501 7288 7c08 a006 7c09  r.|.d.u.r.|...|.
+000032c0: a101 0100 7c0a 6701 7d09 7179 7c09 a006  ....|.g.}.qy|...
+000032d0: 7c0a a101 0100 7179 7c08 a006 7c09 a101  |.....qy|...|...
+000032e0: 0100 8701 6601 640d 640e 8408 7c08 4400  ....f.d.d...|.D.
+000032f0: 8301 7d08 7c02 a001 8700 6601 640f 6410  ..}.|.....f.d.d.
+00003300: 8408 7c08 4400 8301 a101 0100 7c02 a006  ..|.D.......|...
+00003310: 7c03 6411 1700 a101 0100 6408 a003 7c02  |.d.......d...|.
+00003320: a101 5300 2912 4e72 7a00 0000 7201 0000  ..S.).Nrz...r...
+00003330: 00a9 0172 9900 0000 fa01 2872 a500 0000  ...r......(r....
+00003340: 7a13 2020 206e 6f6e 756e 6966 6f72 6d20  z.   nonuniform 
+00003350: 4c69 7374 3c7a 023e 0a72 7e00 0000 2901  List<z.>.r~...).
+00003360: da03 6865 7829 055a 0673 706c 696e 65da  ..hex).Z.spline.
+00003370: 0361 7263 5a08 706f 6c79 4c69 6e65 5a07  .arcZ.polyLineZ.
+00003380: 4253 706c 696e 6572 bd00 0000 2902 da06  BSpliner....)...
+00003390: 626c 6f63 6b73 da05 6564 6765 7372 3900  blocks..edgesr9.
+000033a0: 0000 6301 0000 0000 0000 0000 0000 0002  ..c.............
+000033b0: 0000 0007 0000 0013 0000 0073 2400 0000  ...........s$...
+000033c0: 6700 7c00 5d0e 7d01 6400 a000 8700 6601  g.|.].}.d.....f.
+000033d0: 6401 6402 8408 7c01 4400 8301 a101 9102  d.d...|.D.......
+000033e0: 7102 5300 2903 727a 0000 0063 0100 0000  q.S.).rz...c....
+000033f0: 0000 0000 0000 0000 0200 0000 0400 0000  ................
+00003400: 3300 0000 731a 0000 0081 007c 005d 087d  3...s......|.].}
+00003410: 0188 00a0 007c 01a1 0156 0001 0071 0264  .....|...V...q.d
+00003420: 0053 0072 3000 0000 72c2 0000 0029 0272  .S.r0...r....).r
+00003430: 3500 0000 da05 5f69 7465 6d72 a600 0000  5....._itemr....
+00003440: 7221 0000 0072 2200 0000 7238 0000 00c1  r!...r"...r8....
+00003450: 0100 0072 5c00 0000 7a27 4c69 7374 2e64  ...r\...z'List.d
+00003460: 756d 702e 3c6c 6f63 616c 733e 2e3c 6c69  ump.<locals>.<li
+00003470: 7374 636f 6d70 3e2e 3c67 656e 6578 7072  stcomp>.<genexpr
+00003480: 3e72 b000 0000 2902 7235 0000 00da 0a69  >r....).r5.....i
+00003490: 7465 6d73 5f6c 696e 6572 a600 0000 7221  tems_liner....r!
+000034a0: 0000 0072 2200 0000 7263 0000 00c0 0100  ...r"...rc......
+000034b0: 0073 0800 0000 0600 0202 16ff 06ff 7a1d  .s............z.
+000034c0: 4c69 7374 2e64 756d 702e 3c6c 6f63 616c  List.dump.<local
+000034d0: 733e 2e3c 6c69 7374 636f 6d70 3e63 0100  s>.<listcomp>c..
+000034e0: 0000 0000 0000 0000 0000 0200 0000 0300  ................
+000034f0: 0000 3300 0000 7320 0000 0081 007c 005d  ..3...s .....|.]
+00003500: 0b7d 0188 0064 0017 0064 0114 007c 0117  .}...d...d...|..
+00003510: 0056 0001 0071 0264 0253 0029 0372 3900  .V...q.d.S.).r9.
+00003520: 0000 727a 0000 004e 7221 0000 0029 0272  ..rz...Nr!...).r
+00003530: 3500 0000 72bd 0000 0072 c600 0000 7221  5...r....r....r!
+00003540: 0000 0072 2200 0000 7238 0000 00c4 0100  ...r"...r8......
+00003550: 0073 0400 0000 0280 1e00 7a1c 4c69 7374  .s........z.List
+00003560: 2e64 756d 702e 3c6c 6f63 616c 733e 2e3c  .dump.<locals>.<
+00003570: 6765 6e65 7870 723e 7a02 293b 2909 72b2  genexpr>z.);).r.
+00003580: 0000 00da 0665 7874 656e 6472 c500 0000  .....extendr....
+00003590: 7228 0000 0072 be00 0000 7234 0000 0072  r(...r....r4...r
+000035a0: 2700 0000 da04 6b65 7973 723d 0000 0029  '.....keysr=...)
+000035b0: 0b72 4400 0000 7299 0000 0072 7700 0000  .rD...r....rw...
+000035c0: 72bc 0000 0072 7400 0000 5a0d 7370 6563  r....rt...Z.spec
+000035d0: 6961 6c5f 6b65 7973 735a 0c73 7065 6369  ial_keyssZ.speci
+000035e0: 616c 5f6b 6579 735a 0b73 7065 6369 616c  al_keysZ.special
+000035f0: 5f6b 6579 da05 6c69 6e65 7372 cd00 0000  _key..linesr....
+00003600: 7290 0000 0072 2100 0000 72c4 0000 0072  r....r!...r....r
+00003610: 2200 0000 7280 0000 009c 0100 0073 5000  "...r........sP.
+00003620: 0000 0401 0801 0a01 1201 1601 0602 0a01  ................
+00003630: 0201 0a01 0201 02ff 0601 04ff 04ff 1c05  ................
+00003640: 0202 0201 06fe 0e04 1c01 0401 0a01 0c01  ................
+00003650: 0801 0801 0401 0401 0801 0801 0801 0a01  ................
+00003660: 0801 0c02 0a01 0a01 0202 06fe 1804 0e01  ................
+00003670: 0a01 7a09 4c69 7374 2e64 756d 7072 9400  ..z.List.dumpr..
+00003680: 0000 729a 0000 0029 0c72 4700 0000 7248  ..r....).rG...rH
+00003690: 0000 0072 4900 0000 da07 5f5f 646f 635f  ...rI.....__doc_
+000036a0: 5f72 7600 0000 72b7 0000 0072 c100 0000  _rv...r....r....
+000036b0: 7278 0000 0072 c500 0000 72c3 0000 0072  rx...r....r....r
+000036c0: 8000 0000 72a2 0000 0072 2100 0000 7221  ....r....r!...r!
+000036d0: 0000 0072 a000 0000 7222 0000 0072 3300  ...r....r"...r3.
+000036e0: 0000 7c01 0000 7312 0000 0008 0004 010e  ..|...s.........
+000036f0: 0208 0508 030c 0908 030a 0312 0672 3300  .............r3.
+00003700: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
+00003710: 0000 0001 0000 0040 0000 0073 1000 0000  .......@...s....
+00003720: 6500 5a01 6400 5a02 6401 5a03 6402 5300  e.Z.d.Z.d.Z.d.S.
+00003730: 2903 72bb 0000 007a 2241 2064 6963 7469  ).r....z"A dicti
+00003740: 6f6e 6e61 7279 2074 6f20 7374 6f72 6520  onnary to store 
+00003750: 2363 6f64 6553 7472 6561 6d4e 2904 7247  #codeStreamN).rG
+00003760: 0000 0072 4800 0000 7249 0000 0072 d100  ...rH...rI...r..
+00003770: 0000 7221 0000 0072 2100 0000 7221 0000  ..r!...r!...r!..
+00003780: 0072 2200 0000 72bb 0000 00c9 0100 0073  .r"...r........s
+00003790: 0400 0000 0800 0801 72bb 0000 0063 0100  ........r....c..
+000037a0: 0000 0000 0000 0000 0000 0300 0000 0300  ................
+000037b0: 0000 0300 0000 7322 0000 0087 0066 0164  ......s".....f.d
+000037c0: 0164 0284 087d 0187 0066 0164 0364 0484  .d...}...f.d.d..
+000037d0: 087d 0274 007c 017c 0283 0253 0029 054e  .}.t.|.|...S.).N
+000037e0: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+000037f0: 0002 0000 0013 0000 0073 0a00 0000 7c00  .........s....|.
+00003800: 8800 1900 6a00 5300 7230 0000 00a9 01da  ....j.S.r0......
+00003810: 0463 6f64 6572 a600 0000 725d 0000 0072  .coder....r]...r
+00003820: 2100 0000 7222 0000 0072 5200 0000 ce01  !...r"...rR.....
+00003830: 0000 7293 0000 007a 185f 6d61 6b65 5f61  ..r....z._make_a
+00003840: 6c69 6173 2e3c 6c6f 6361 6c73 3e2e 6765  lias.<locals>.ge
+00003850: 7463 0200 0000 0000 0000 0000 0000 0200  tc..............
+00003860: 0000 0300 0000 1300 0000 730e 0000 007c  ..........s....|
+00003870: 017c 0088 0019 005f 0064 0053 0072 3000  .|....._.d.S.r0.
+00003880: 0000 72d2 0000 0029 02da 055f 7365 6c66  ..r....)..._self
+00003890: 7237 0000 0072 5d00 0000 7221 0000 0072  r7...r]...r!...r
+000038a0: 2200 0000 da03 7365 74d1 0100 0072 8f00  ".....set....r..
+000038b0: 0000 7a18 5f6d 616b 655f 616c 6961 732e  ..z._make_alias.
+000038c0: 3c6c 6f63 616c 733e 2e73 6574 2901 da08  <locals>.set)...
+000038d0: 7072 6f70 6572 7479 2903 724d 0000 0072  property).rM...r
+000038e0: 5200 0000 72d5 0000 0072 2100 0000 725d  R...r....r!...r]
+000038f0: 0000 0072 2200 0000 da0b 5f6d 616b 655f  ...r"....._make_
+00003900: 616c 6961 73cd 0100 0073 0600 0000 0c01  alias....s......
+00003910: 0c03 0a03 72d7 0000 0029 045a 0b63 6f64  ....r....).Z.cod
+00003920: 6549 6e63 6c75 6465 5a0b 636f 6465 4f70  eIncludeZ.codeOp
+00003930: 7469 6f6e 735a 0863 6f64 654c 6962 7372  tionsZ.codeLibsr
+00003940: d300 0000 6300 0000 0000 0000 0000 0000  ....c...........
+00003950: 0000 0000 0003 0000 0040 0000 0072 a300  .........@...r..
+00003960: 0000 290b da04 436f 6465 4e63 0400 0000  ..)...CodeNc....
+00003970: 0000 0000 0000 0000 0400 0000 0200 0000  ................
+00003980: 4300 0000 731a 0000 007c 017c 005f 0074  C...s....|.|._.t
+00003990: 017c 0283 017c 005f 027c 037c 005f 0364  .|...|._.|.|._.d
+000039a0: 0053 0072 3000 0000 2904 724d 0000 0072  .S.r0...).rM...r
+000039b0: 0600 0000 72d3 0000 0072 b400 0000 2904  ....r....r....).
+000039c0: 7244 0000 0072 4d00 0000 72d3 0000 0072  rD...rM...r....r
+000039d0: b400 0000 7221 0000 0072 2100 0000 7222  ....r!...r!...r"
+000039e0: 0000 0072 7600 0000 dc01 0000 7306 0000  ...rv.......s...
+000039f0: 0006 010a 010a 017a 0d43 6f64 652e 5f5f  .......z.Code.__
+00003a00: 696e 6974 5f5f 6301 0000 0000 0000 0000  init__c.........
+00003a10: 0000 0001 0000 0005 0000 0043 0000 0073  ...........C...s
+00003a20: 3e00 0000 7c00 6a00 6400 7500 7210 6401  >...|.j.d.u.r.d.
+00003a30: 7c00 6a01 6400 6402 8502 1900 9b00 6403  |.j.d.d.......d.
+00003a40: 9d03 5300 6401 7c00 6a01 6400 6402 8502  ..S.d.|.j.d.d...
+00003a50: 1900 9b00 6404 7c00 6a00 9b00 6405 9d05  ....d.|.j...d...
+00003a60: 5300 2906 4e7a 0643 6f64 6528 2272 2f00  S.).Nz.Code("r/.
+00003a70: 0000 7a07 5b2e 2e2e 5d22 297a 125b 2e2e  ..z.[...]")z.[..
+00003a80: 2e5d 222c 2064 6972 6563 7469 7665 3d72  .]", directive=r
+00003a90: a500 0000 2902 72b4 0000 0072 d300 0000  ....).r....r....
+00003aa0: 72a6 0000 0072 2100 0000 7221 0000 0072  r....r!...r!...r
+00003ab0: 2200 0000 7278 0000 00e1 0100 0073 0600  "...rx.......s..
+00003ac0: 0000 0a01 1601 1e01 7a0d 436f 6465 2e5f  ........z.Code._
+00003ad0: 5f72 6570 725f 5f72 0100 0000 6302 0000  _repr__r....c...
+00003ae0: 0000 0000 0000 0000 0007 0000 0005 0000  ................
+00003af0: 0043 0000 0073 8a00 0000 6700 7d02 7c01  .C...s....g.}.|.
+00003b00: 6401 1400 7d03 7c01 6402 1700 6401 1400  d...}.|.d...d...
+00003b10: 7d04 7c03 7c00 6a00 1700 7d05 7c00 6a01  }.|.|.j...}.|.j.
+00003b20: 6400 7501 721d 7c05 6401 7c00 6a01 1700  d.u.r.|.d.|.j...
+00003b30: 3700 7d05 7c02 a002 7c05 6403 7c03 9b00  7.}.|...|.d.|...
+00003b40: 9d02 1700 6404 1700 a101 0100 7c00 6a03  ....d.......|.j.
+00003b50: a004 6403 a101 4400 5d09 7d06 7c02 a002  ..d...D.].}.|...
+00003b60: 7c04 7c06 1700 a101 0100 712f 7c02 a002  |.|.......q/|...
+00003b70: 7c03 6405 1700 a101 0100 6403 a005 7c02  |.d.......d...|.
+00003b80: a101 5300 2906 4e72 7a00 0000 7239 0000  ..S.).Nrz...r9..
+00003b90: 0072 7e00 0000 7a02 237b 7a03 237d 3b29  .r~...z.#{z.#};)
+00003ba0: 0672 4d00 0000 72b4 0000 0072 2700 0000  .rM...r....r'...
+00003bb0: 72d3 0000 0072 1900 0000 7228 0000 0029  r....r....r(...)
+00003bc0: 0772 4400 0000 7299 0000 0072 7700 0000  .rD...r....rw...
+00003bd0: 72bc 0000 005a 0c69 6e64 656e 7461 7469  r....Z.indentati
+00003be0: 6f6e 3472 1700 0000 72bd 0000 0072 2100  on4r....r....r!.
+00003bf0: 0000 7221 0000 0072 2200 0000 7280 0000  ..r!...r"...r...
+00003c00: 00e6 0100 0073 1600 0000 0401 0801 0c01  .....s..........
+00003c10: 0a01 0a01 0e01 1801 1001 1001 0e01 0a01  ................
+00003c20: 7a09 436f 6465 2e64 756d 7072 3000 0000  z.Code.dumpr0...
+00003c30: 729a 0000 00a9 0672 4700 0000 7248 0000  r......rG...rH..
+00003c40: 0072 4900 0000 7276 0000 0072 7800 0000  .rI...rv...rx...
+00003c50: 7280 0000 0072 2100 0000 7221 0000 0072  r....r!...r!...r
+00003c60: 2100 0000 7222 0000 0072 d800 0000 db01  !...r"...r......
+00003c70: 0000 7308 0000 0008 000a 0108 050e 0572  ..s............r
+00003c80: d800 0000 6300 0000 0000 0000 0000 0000  ....c...........
+00003c90: 0000 0000 0003 0000 0040 0000 0072 a300  .........@...r..
+00003ca0: 0000 290b da04 4e61 6d65 4e63 0300 0000  ..)...NameNc....
+00003cb0: 0000 0000 0000 0000 0300 0000 0200 0000  ................
+00003cc0: 4300 0000 f310 0000 007c 017c 005f 007c  C........|.|._.|
+00003cd0: 027c 005f 0164 0053 0072 3000 0000 2902  .|._.d.S.r0...).
+00003ce0: 724d 0000 0072 3700 0000 2903 7244 0000  rM...r7...).rD..
+00003cf0: 0072 4d00 0000 7237 0000 0072 2100 0000  .rM...r7...r!...
+00003d00: 7221 0000 0072 2200 0000 7276 0000 00f6  r!...r"...rv....
+00003d10: 0100 00f3 0400 0000 0601 0a01 7a0d 4e61  ............z.Na
+00003d20: 6d65 2e5f 5f69 6e69 745f 5f63 0100 0000  me.__init__c....
+00003d30: 0000 0000 0000 0000 0100 0000 0300 0000  ................
+00003d40: 4300 0000 730e 0000 0064 017c 006a 009b  C...s....d.|.j..
+00003d50: 0064 029d 0353 0029 034e 7a05 4e61 6d65  .d...S.).Nz.Name
+00003d60: 2872 a500 0000 725d 0000 0072 a600 0000  (r....r]...r....
+00003d70: 7221 0000 0072 2100 0000 7222 0000 0072  r!...r!...r"...r
+00003d80: 7800 0000 fa01 0000 728f 0000 007a 0d4e  x.......r....z.N
+00003d90: 616d 652e 5f5f 7265 7072 5f5f 7201 0000  ame.__repr__r...
+00003da0: 0063 0200 0000 0000 0000 0000 0000 0200  .c..............
+00003db0: 0000 0100 0000 4300 0000 7308 0000 007c  ......C...s....|
+00003dc0: 006a 009b 0053 0072 3000 0000 725d 0000  .j...S.r0...r]..
+00003dd0: 0072 9800 0000 7221 0000 0072 2100 0000  .r....r!...r!...
+00003de0: 7222 0000 0072 8000 0000 fd01 0000 72ae  r"...r........r.
+00003df0: 0000 007a 094e 616d 652e 6475 6d70 7230  ...z.Name.dumpr0
+00003e00: 0000 0072 9a00 0000 72d9 0000 0072 2100  ...r....r....r!.
+00003e10: 0000 7221 0000 0072 2100 0000 7222 0000  ..r!...r!...r"..
+00003e20: 0072 da00 0000 f401 0000 7308 0000 0008  .r........s.....
+00003e30: 000a 0208 040e 0372 da00 0000 6300 0000  .......r....c...
+00003e40: 0000 0000 0000 0000 0000 0000 0003 0000  ................
+00003e50: 0040 0000 0073 2600 0000 6500 5a01 6400  .@...s&...e.Z.d.
+00003e60: 5a02 6401 6402 8400 5a03 6403 6404 8400  Z.d.d...Z.d.d...
+00003e70: 5a04 6409 6406 6407 8401 5a05 6408 5300  Z.d.d.d...Z.d.S.
+00003e80: 290a da09 4469 7265 6374 6976 6563 0300  )...Directivec..
+00003e90: 0000 0000 0000 0000 0000 0300 0000 0200  ................
+00003ea0: 0000 4300 0000 72db 0000 0072 3000 0000  ..C...r....r0...
+00003eb0: a902 72b4 0000 00da 0763 6f6e 7465 6e74  ..r......content
+00003ec0: 2903 7244 0000 0072 b400 0000 72df 0000  ).rD...r....r...
+00003ed0: 0072 2100 0000 7221 0000 0072 2200 0000  .r!...r!...r"...
+00003ee0: 7276 0000 0002 0200 0072 dc00 0000 7a12  rv.......r....z.
+00003ef0: 4469 7265 6374 6976 652e 5f5f 696e 6974  Directive.__init
+00003f00: 5f5f 6301 0000 0000 0000 0000 0000 0001  __c.............
+00003f10: 0000 0003 0000 0043 0000 0073 1200 0000  .......C...s....
+00003f20: 7c00 6a00 9b00 6401 7c00 6a01 9b00 9d03  |.j...d.|.j.....
+00003f30: 5300 2902 4e72 9700 0000 72de 0000 0072  S.).Nr....r....r
+00003f40: a600 0000 7221 0000 0072 2100 0000 7222  ....r!...r!...r"
+00003f50: 0000 0072 7800 0000 0602 0000 7302 0000  ...rx.......s...
+00003f60: 0012 017a 1244 6972 6563 7469 7665 2e5f  ...z.Directive._
+00003f70: 5f72 6570 725f 5f72 0100 0000 6302 0000  _repr__r....c...
+00003f80: 0000 0000 0000 0000 0002 0000 0005 0000  ................
+00003f90: 0043 0000 0073 1c00 0000 7c01 6401 1400  .C...s....|.d...
+00003fa0: 7c00 6a00 9b00 6402 7c00 6a01 9b00 6403  |.j...d.|.j...d.
+00003fb0: 9d04 1700 5300 2904 4e72 7a00 0000 7297  ....S.).Nrz...r.
+00003fc0: 0000 0072 7c00 0000 72de 0000 0072 9800  ...r|...r....r..
+00003fd0: 0000 7221 0000 0072 2100 0000 7222 0000  ..r!...r!...r"..
+00003fe0: 0072 8000 0000 0902 0000 72b1 0000 007a  .r........r....z
+00003ff0: 0e44 6972 6563 7469 7665 2e64 756d 704e  .Directive.dumpN
+00004000: 729a 0000 0072 d900 0000 7221 0000 0072  r....r....r!...r
+00004010: 2100 0000 7221 0000 0072 2200 0000 72dd  !...r!...r"...r.
+00004020: 0000 0001 0200 0073 0800 0000 0800 0801  .......s........
+00004030: 0804 0e03 72dd 0000 0029 0172 2f00 0000  ....r....).r/...
+00004040: 2927 72d1 0000 0072 1500 0000 da03 6162  )'r....r......ab
+00004050: 6372 0200 0000 7203 0000 00da 0b64 6174  cr....r......dat
+00004060: 6163 6c61 7373 6573 7204 0000 00da 076e  aclassesr......n
+00004070: 756d 6265 7273 7205 0000 00da 0874 6578  umbersr......tex
+00004080: 7477 7261 7072 0600 0000 da06 7479 7069  twrapr......typi
+00004090: 6e67 7207 0000 00da 056e 756d 7079 7267  ngr......numpyrg
+000040a0: 0000 00da 0a69 6e66 6c65 6374 696f 6e72  .....inflectionr
+000040b0: 0800 0000 721b 0000 0072 2300 0000 722e  ....r....r#...r.
+000040c0: 0000 0072 4000 0000 7241 0000 0072 4a00  ...r@...rA...rJ.
+000040d0: 0000 7271 0000 0072 9500 0000 729d 0000  ..rq...r....r...
+000040e0: 0072 6f00 0000 7251 0000 0072 6900 0000  .ro...rQ...ri...
+000040f0: 7254 0000 0072 3200 0000 7233 0000 0072  rT...r2...r3...r
+00004100: bb00 0000 72d7 0000 0072 b200 0000 da07  ....r....r......
+00004110: 7365 7461 7474 7272 d800 0000 72da 0000  setattrr....r...
+00004120: 0072 dd00 0000 7221 0000 0072 2100 0000  .r....r!...r!...
+00004130: 7221 0000 0072 2200 0000 da08 3c6d 6f64  r!...r".....<mod
+00004140: 756c 653e 0100 0000 7340 0000 0004 0008  ule>....s@......
+00004150: 0210 010c 010c 010c 010c 0108 020c 0108  ................
+00004160: 0208 0308 1b0a 120e 1110 0712 5702 4b10  ............W.K.
+00004170: 0110 0b02 0c12 0112 2614 0f12 3710 4d08  ........&...7.M.
+00004180: 0408 0a16 0110 0302 1912 0114 0c         .............
```

### Comparing `fluidsimfoam-0.0.5/src/fluidsimfoam/foam_input_files/__pycache__/constant_files.cpython-39.pyc` & `fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/__pycache__/constant_files.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun  1 13:07:51 2023 UTC, .py size: 2058 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 2798 7864 0a08 0000  a.......'.xd....
+00000000: 6f0d 0d0a 0000 0000 5ab4 6f64 0a08 0000  o.......Z.od....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4400 0000 6400  .....@...sD...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 6d05 5a05 6d06 5a06  d.l.m.Z.m.Z.m.Z.
 00000050: 6d07 5a07 6d08 5a08 6d09 5a09 0100 4700  m.Z.m.Z.m.Z...G.
 00000060: 6404 6405 8400 6405 6505 8303 5a0a 6406  d.d...d.e...Z.d.
 00000070: 5300 2907 7a1f 4865 6c70 6572 2074 6f20  S.).z.Helper to 
@@ -12,111 +12,113 @@
 000000b0: 696f 6e53 6574 da0a 4669 6c65 4865 6c70  ionSet..FileHelp
 000000c0: 6572 da0d 466f 616d 496e 7075 7446 696c  er..FoamInputFil
 000000d0: 65da 0b5f 6173 5f70 795f 6e61 6d65 da15  e.._as_py_name..
 000000e0: 5f63 6f6d 706c 6574 655f 7061 7261 6d73  _complete_params
 000000f0: 5f64 6963 74da 185f 7570 6461 7465 5f64  _dict.._update_d
 00000100: 6963 745f 7769 7468 5f70 6172 616d 7363  ict_with_paramsc
 00000110: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000120: 0900 0000 4000 0000 7338 0000 0065 005a  ....@...s8...e.Z
-00000130: 0164 005a 0264 0b65 0365 0465 0365 0465  .d.Z.d.e.e.e.e.e
-00000140: 0465 0365 0364 049c 0764 0564 0684 055a  .e.e.d...d.d...Z
-00000150: 0564 0764 0884 005a 0664 0964 0a84 005a  .d.d...Z.d.d...Z
-00000160: 0764 0253 0029 0cda 1243 6f6e 7374 616e  .d.S.)...Constan
-00000170: 7446 696c 6548 656c 7065 7246 4eda 0a64  tFileHelperFN..d
-00000180: 6963 7469 6f6e 6172 7929 07da 0966 696c  ictionary)...fil
-00000190: 655f 6e61 6d65 da07 6465 6661 756c 74da  e_name..default.
-000001a0: 1164 6566 6175 6c74 5f64 696d 656e 7369  .default_dimensi
-000001b0: 6f6e da0a 6469 6d65 6e73 696f 6e73 da08  on..dimensions..
-000001c0: 636f 6d6d 656e 7473 da03 646f 63da 0363  comments..doc..c
-000001d0: 6c73 6309 0000 0000 0000 0000 0000 0009  lsc.............
-000001e0: 0000 0005 0000 0043 0000 0073 4800 0000  .......C...sH...
-000001f0: 7c01 7c00 5f00 7c02 7c00 5f01 7c03 7c00  |.|._.|.|._.|.|.
-00000200: 5f02 7c04 7c00 5f03 7c05 7c00 5f04 7c06  _.|.|._.|.|._.|.
-00000210: 7c00 5f05 7c07 7c00 5f06 7c08 7c00 5f07  |._.|.|._.|.|._.
-00000220: 7408 7c00 6a00 a009 6401 6402 a102 8301  t.|.j...d.d.....
-00000230: 7c00 5f0a 6400 5300 2903 4eda 0a50 726f  |._.d.S.).N..Pro
-00000240: 7065 7274 6965 73da 0029 0b72 0b00 0000  perties..).r....
-00000250: 720c 0000 0072 0d00 0000 720e 0000 0072  r....r....r....r
-00000260: 0f00 0000 7210 0000 0072 1100 0000 da09  ....r....r......
-00000270: 6469 6d65 6e73 696f 6e72 0600 0000 da07  dimensionr......
-00000280: 7265 706c 6163 65da 116e 616d 655f 7061  replace..name_pa
-00000290: 7261 6d73 5f63 6869 6c64 2909 da04 7365  rams_child)...se
-000002a0: 6c66 720b 0000 0072 0c00 0000 720d 0000  lfr....r....r...
-000002b0: 0072 0e00 0000 720f 0000 0072 1000 0000  .r....r....r....
-000002c0: 7211 0000 0072 1400 0000 a900 7218 0000  r....r......r...
-000002d0: 00fa 5a2f 686f 6d65 2f75 7365 7273 2f61  ..Z/home/users/a
-000002e0: 7567 6965 7233 7069 2f44 6576 2f66 6c75  ugier3pi/Dev/flu
-000002f0: 6964 7369 6d66 6f61 6d2f 7372 632f 666c  idsimfoam/src/fl
-00000300: 7569 6473 696d 666f 616d 2f66 6f61 6d5f  uidsimfoam/foam_
-00000310: 696e 7075 745f 6669 6c65 732f 636f 6e73  input_files/cons
-00000320: 7461 6e74 5f66 696c 6573 2e70 79da 085f  tant_files.py.._
-00000330: 5f69 6e69 745f 5f10 0000 0073 1600 0000  _init__....s....
-00000340: 000b 0601 0601 0601 0601 0601 0601 0601  ................
-00000350: 0601 0201 0cff 7a1b 436f 6e73 7461 6e74  ......z.Constant
-00000360: 4669 6c65 4865 6c70 6572 2e5f 5f69 6e69  FileHelper.__ini
-00000370: 745f 5f63 0200 0000 0000 0000 0000 0000  t__c............
-00000380: 0300 0000 0800 0000 4300 0000 7342 0000  ........C...sB..
-00000390: 007a 0c7c 0164 0119 007d 0257 006e 1c04  .z.|.d...}.W.n..
-000003a0: 0074 0079 2801 0001 0001 007c 01a0 0164  .t.y(......|...d
-000003b0: 01a1 017d 0259 006e 0230 0074 027c 027c  ...}.Y.n.0.t.|.|
-000003c0: 006a 037c 006a 047c 006a 0583 0401 0064  .j.|.j.|.j.....d
-000003d0: 0053 0029 024e da08 636f 6e73 7461 6e74  .S.).N..constant
-000003e0: 2906 da0e 4174 7472 6962 7574 6545 7272  )...AttributeErr
-000003f0: 6f72 da0a 5f73 6574 5f63 6869 6c64 7207  or.._set_childr.
-00000400: 0000 0072 1600 0000 720c 0000 0072 1000  ...r....r....r..
-00000410: 0000 2903 7217 0000 00da 0670 6172 616d  ..).r......param
-00000420: 735a 0f63 6f6e 7374 616e 745f 7061 7261  sZ.constant_para
-00000430: 6d73 7218 0000 0072 1800 0000 7219 0000  msr....r....r...
-00000440: 00da 0f63 6f6d 706c 6574 655f 7061 7261  ...complete_para
-00000450: 6d73 2700 0000 730e 0000 0000 0102 010c  ms'...s.........
-00000460: 010c 0110 0202 010e ff7a 2243 6f6e 7374  .........z"Const
-00000470: 616e 7446 696c 6548 656c 7065 722e 636f  antFileHelper.co
-00000480: 6d70 6c65 7465 5f70 6172 616d 7363 0200  mplete_paramsc..
-00000490: 0000 0000 0000 0000 0000 0500 0000 0700  ................
-000004a0: 0000 4300 0000 7376 0000 0074 0064 0164  ..C...sv...t.d.d
-000004b0: 027c 006a 0164 037c 006a 0264 049c 057c  .|.j.d.|.j.d...|
-000004c0: 006a 0364 058d 027d 027c 006a 0464 0075  .j.d...}.|.j.d.u
-000004d0: 0172 3a7c 02a0 0564 0674 067c 006a 0483  .r:|...d.t.|.j..
-000004e0: 01a1 0201 007c 016a 077c 006a 0819 007d  .....|.j.|.j...}
-000004f0: 0374 097c 006a 0a83 017d 0474 0b7c 047c  .t.|.j...}.t.|.|
-00000500: 0383 0201 007c 026a 0c7c 047c 006a 0d7c  .....|.j.|.|.j.|
-00000510: 006a 0e7c 006a 0364 078d 0401 007c 0253  .j.|.j.d.....|.S
-00000520: 0029 084e 6700 0000 0000 0000 40da 0561  .).Ng.......@..a
-00000530: 7363 6969 7a0a 2263 6f6e 7374 616e 7422  sciiz."constant"
-00000540: 2905 da07 7665 7273 696f 6eda 0666 6f72  )...version..for
-00000550: 6d61 74da 0563 6c61 7373 da08 6c6f 6361  mat..class..loca
-00000560: 7469 6f6e da06 6f62 6a65 6374 2902 da04  tion..object)...
-00000570: 696e 666f 720f 0000 0072 0e00 0000 2903  infor....r....).
-00000580: 720e 0000 0072 0d00 0000 720f 0000 0029  r....r....r....)
-00000590: 0f72 0500 0000 7211 0000 0072 0b00 0000  .r....r....r....
-000005a0: 720f 0000 0072 1400 0000 da09 7365 745f  r....r......set_
-000005b0: 6368 696c 6472 0300 0000 721b 0000 0072  childr....r....r
-000005c0: 1600 0000 7202 0000 0072 0c00 0000 7208  ....r....r....r.
-000005d0: 0000 00da 1469 6e69 745f 6672 6f6d 5f70  .....init_from_p
-000005e0: 795f 6f62 6a65 6374 7372 0e00 0000 720d  y_objectsr....r.
-000005f0: 0000 0029 0572 1700 0000 721e 0000 00da  ...).r....r.....
-00000600: 0474 7265 655a 0b70 6172 616d 735f 6669  .treeZ.params_fi
-00000610: 6c65 720c 0000 0072 1800 0000 7218 0000  ler....r....r...
-00000620: 0072 1900 0000 da09 6d61 6b65 5f74 7265  .r......make_tre
-00000630: 6531 0000 0073 2a00 0000 0001 0202 0201  e1...s*.........
-00000640: 0201 0401 0201 04fb 0407 04f8 060b 0a01  ................
-00000650: 1202 0c02 0a01 0a02 0401 0201 0401 0401  ................
-00000660: 04fc 0607 7a1c 436f 6e73 7461 6e74 4669  ....z.ConstantFi
-00000670: 6c65 4865 6c70 6572 2e6d 616b 655f 7472  leHelper.make_tr
-00000680: 6565 2906 464e 4e4e 720a 0000 004e 2908  ee).FNNNr....N).
-00000690: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
-000006a0: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
-000006b0: 6d65 5f5f da03 7374 72da 0464 6963 7472  me__..str..dictr
-000006c0: 1a00 0000 721f 0000 0072 2a00 0000 7218  ....r....r*...r.
-000006d0: 0000 0072 1800 0000 7218 0000 0072 1900  ...r....r....r..
-000006e0: 0000 7209 0000 000f 0000 0073 2200 0000  ..r........s"...
-000006f0: 0805 0001 0001 0001 0001 0001 00f7 0202  ................
-00000700: 0201 0201 0201 0201 0201 0201 02f8 0c17  ................
-00000710: 080a 7209 0000 004e 290b da07 5f5f 646f  ..r....N)...__do
-00000720: 635f 5fda 0463 6f70 7972 0200 0000 5a1d  c__..copyr....Z.
-00000730: 666c 7569 6473 696d 666f 616d 2e66 6f61  fluidsimfoam.foa
-00000740: 6d5f 696e 7075 745f 6669 6c65 7372 0300  m_input_filesr..
-00000750: 0000 7204 0000 0072 0500 0000 7206 0000  ..r....r....r...
-00000760: 0072 0700 0000 7208 0000 0072 0900 0000  .r....r....r....
-00000770: 7218 0000 0072 1800 0000 7218 0000 0072  r....r....r....r
-00000780: 1900 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
-00000790: 0000 7306 0000 0004 020c 0220 0a         ..s........ .
+00000120: 0f00 0000 4000 0000 7350 0000 0065 005a  ....@...sP...e.Z
+00000130: 0164 005a 0209 0109 0209 0209 0209 0309  .d.Z............
+00000140: 0264 1164 0465 0364 0565 0464 0665 0364  .d.d.e.d.e.d.e.d
+00000150: 0765 0464 0865 0464 0965 0364 0a65 0366  .e.d.e.d.e.d.e.f
+00000160: 0e64 0b64 0c84 055a 0564 0d64 0e84 005a  .d.d...Z.d.d...Z
+00000170: 0664 0f64 1084 005a 0764 0253 0029 12da  .d.d...Z.d.S.)..
+00000180: 1243 6f6e 7374 616e 7446 696c 6548 656c  .ConstantFileHel
+00000190: 7065 7246 4eda 0a64 6963 7469 6f6e 6172  perFN..dictionar
+000001a0: 79da 0966 696c 655f 6e61 6d65 da07 6465  y..file_name..de
+000001b0: 6661 756c 74da 1164 6566 6175 6c74 5f64  fault..default_d
+000001c0: 696d 656e 7369 6f6e da0a 6469 6d65 6e73  imension..dimens
+000001d0: 696f 6e73 da08 636f 6d6d 656e 7473 da03  ions..comments..
+000001e0: 646f 63da 0363 6c73 6309 0000 0000 0000  doc..clsc.......
+000001f0: 0000 0000 0009 0000 0005 0000 0043 0000  .............C..
+00000200: 0073 4800 0000 7c01 7c00 5f00 7c02 7c00  .sH...|.|._.|.|.
+00000210: 5f01 7c03 7c00 5f02 7c04 7c00 5f03 7c05  _.|.|._.|.|._.|.
+00000220: 7c00 5f04 7c06 7c00 5f05 7c07 7c00 5f06  |._.|.|._.|.|._.
+00000230: 7c08 7c00 5f07 7408 7c00 6a00 a009 6401  |.|._.t.|.j...d.
+00000240: 6402 a102 8301 7c00 5f0a 6400 5300 2903  d.....|._.d.S.).
+00000250: 4eda 0a50 726f 7065 7274 6965 73da 0029  N..Properties..)
+00000260: 0b72 0b00 0000 720c 0000 0072 0d00 0000  .r....r....r....
+00000270: 720e 0000 0072 0f00 0000 7210 0000 0072  r....r....r....r
+00000280: 1100 0000 da09 6469 6d65 6e73 696f 6e72  ......dimensionr
+00000290: 0600 0000 da07 7265 706c 6163 65da 116e  ......replace..n
+000002a0: 616d 655f 7061 7261 6d73 5f63 6869 6c64  ame_params_child
+000002b0: 2909 da04 7365 6c66 720b 0000 0072 0c00  )...selfr....r..
+000002c0: 0000 720d 0000 0072 0e00 0000 720f 0000  ..r....r....r...
+000002d0: 0072 1000 0000 7211 0000 0072 1400 0000  .r....r....r....
+000002e0: a900 7218 0000 00fa 512f 686f 6d65 2f70  ..r.....Q/home/p
+000002f0: 6965 7272 652f 4465 762f 666c 7569 6473  ierre/Dev/fluids
+00000300: 696d 666f 616d 2f73 7263 2f66 6c75 6964  imfoam/src/fluid
+00000310: 7369 6d66 6f61 6d2f 666f 616d 5f69 6e70  simfoam/foam_inp
+00000320: 7574 5f66 696c 6573 2f63 6f6e 7374 616e  ut_files/constan
+00000330: 745f 6669 6c65 732e 7079 da08 5f5f 696e  t_files.py..__in
+00000340: 6974 5f5f 1000 0000 7316 0000 0006 0b06  it__....s.......
+00000350: 0106 0106 0106 0106 0106 0106 0102 010c  ................
+00000360: 010a ff7a 1b43 6f6e 7374 616e 7446 696c  ...z.ConstantFil
+00000370: 6548 656c 7065 722e 5f5f 696e 6974 5f5f  eHelper.__init__
+00000380: 6302 0000 0000 0000 0000 0000 0003 0000  c...............
+00000390: 0008 0000 0043 0000 0073 4200 0000 7a06  .....C...sB...z.
+000003a0: 7c01 6401 1900 7d02 5700 6e0e 0400 7400  |.d...}.W.n...t.
+000003b0: 7914 0100 0100 0100 7c01 a001 6401 a101  y.......|...d...
+000003c0: 7d02 5900 6e01 7700 7402 7c02 7c00 6a03  }.Y.n.w.t.|.|.j.
+000003d0: 7c00 6a04 7c00 6a05 8304 0100 6400 5300  |.j.|.j.....d.S.
+000003e0: 2902 4eda 0863 6f6e 7374 616e 7429 06da  ).N..constant)..
+000003f0: 0e41 7474 7269 6275 7465 4572 726f 72da  .AttributeError.
+00000400: 0a5f 7365 745f 6368 696c 6472 0700 0000  ._set_childr....
+00000410: 7216 0000 0072 0c00 0000 7210 0000 0029  r....r....r....)
+00000420: 0372 1700 0000 da06 7061 7261 6d73 5a0f  .r......paramsZ.
+00000430: 636f 6e73 7461 6e74 5f70 6172 616d 7372  constant_paramsr
+00000440: 1800 0000 7218 0000 0072 1900 0000 da0f  ....r....r......
+00000450: 636f 6d70 6c65 7465 5f70 6172 616d 7327  complete_params'
+00000460: 0000 0073 1000 0000 0201 0c01 0c01 0e01  ...s............
+00000470: 02ff 0203 0e01 08ff 7a22 436f 6e73 7461  ........z"Consta
+00000480: 6e74 4669 6c65 4865 6c70 6572 2e63 6f6d  ntFileHelper.com
+00000490: 706c 6574 655f 7061 7261 6d73 6302 0000  plete_paramsc...
+000004a0: 0000 0000 0000 0000 0005 0000 0007 0000  ................
+000004b0: 0043 0000 0073 7600 0000 7400 6401 6402  .C...sv...t.d.d.
+000004c0: 7c00 6a01 6403 7c00 6a02 6404 9c05 7c00  |.j.d.|.j.d...|.
+000004d0: 6a03 6405 8d02 7d02 7c00 6a04 6400 7501  j.d...}.|.j.d.u.
+000004e0: 721d 7c02 a005 6406 7406 7c00 6a04 8301  r.|...d.t.|.j...
+000004f0: a102 0100 7c01 6a07 7c00 6a08 1900 7d03  ....|.j.|.j...}.
+00000500: 7409 7c00 6a0a 8301 7d04 740b 7c04 7c03  t.|.j...}.t.|.|.
+00000510: 8302 0100 7c02 6a0c 7c04 7c00 6a0d 7c00  ....|.j.|.|.j.|.
+00000520: 6a0e 7c00 6a03 6407 8d04 0100 7c02 5300  j.|.j.d.....|.S.
+00000530: 2908 4e67 0000 0000 0000 0040 da05 6173  ).Ng.......@..as
+00000540: 6369 697a 0a22 636f 6e73 7461 6e74 2229  ciiz."constant")
+00000550: 05da 0776 6572 7369 6f6e da06 666f 726d  ...version..form
+00000560: 6174 da05 636c 6173 73da 086c 6f63 6174  at..class..locat
+00000570: 696f 6eda 066f 626a 6563 7429 02da 0469  ion..object)...i
+00000580: 6e66 6f72 0f00 0000 720e 0000 0029 0372  nfor....r....).r
+00000590: 0e00 0000 720d 0000 0072 0f00 0000 290f  ....r....r....).
+000005a0: 7205 0000 0072 1100 0000 720b 0000 0072  r....r....r....r
+000005b0: 0f00 0000 7214 0000 00da 0973 6574 5f63  ....r......set_c
+000005c0: 6869 6c64 7203 0000 0072 1b00 0000 7216  hildr....r....r.
+000005d0: 0000 0072 0200 0000 720c 0000 0072 0800  ...r....r....r..
+000005e0: 0000 da14 696e 6974 5f66 726f 6d5f 7079  ....init_from_py
+000005f0: 5f6f 626a 6563 7473 720e 0000 0072 0d00  _objectsr....r..
+00000600: 0000 2905 7217 0000 0072 1e00 0000 da04  ..).r....r......
+00000610: 7472 6565 5a0b 7061 7261 6d73 5f66 696c  treeZ.params_fil
+00000620: 6572 0c00 0000 7218 0000 0072 1800 0000  er....r....r....
+00000630: 7219 0000 00da 096d 616b 655f 7472 6565  r......make_tree
+00000640: 3100 0000 732a 0000 0002 0102 0202 0104  1...s*..........
+00000650: 0102 0104 0104 fb04 0706 f80a 0b12 010c  ................
+00000660: 020a 020a 0104 0202 0104 0104 0104 0106  ................
+00000670: fc04 077a 1c43 6f6e 7374 616e 7446 696c  ...z.ConstantFil
+00000680: 6548 656c 7065 722e 6d61 6b65 5f74 7265  eHelper.make_tre
+00000690: 6529 0646 4e4e 4e72 0a00 0000 4e29 08da  e).FNNNr....N)..
+000006a0: 085f 5f6e 616d 655f 5fda 0a5f 5f6d 6f64  .__name__..__mod
+000006b0: 756c 655f 5fda 0c5f 5f71 7561 6c6e 616d  ule__..__qualnam
+000006c0: 655f 5fda 0373 7472 da04 6469 6374 721a  e__..str..dictr.
+000006d0: 0000 0072 1f00 0000 722a 0000 0072 1800  ...r....r*...r..
+000006e0: 0000 7218 0000 0072 1800 0000 7219 0000  ..r....r....r...
+000006f0: 0072 0900 0000 0f00 0000 7330 0000 0008  .r........s0....
+00000700: 0002 0502 0102 0102 0102 0102 0104 f702  ................
+00000710: 0202 fe02 0302 fd02 0402 fc02 0502 fb02  ................
+00000720: 0602 fa02 0702 f902 080a f808 170c 0a72  ...............r
+00000730: 0900 0000 4e29 0bda 075f 5f64 6f63 5f5f  ....N)...__doc__
+00000740: da04 636f 7079 7202 0000 00da 1d66 6c75  ..copyr......flu
+00000750: 6964 7369 6d66 6f61 6d2e 666f 616d 5f69  idsimfoam.foam_i
+00000760: 6e70 7574 5f66 696c 6573 7203 0000 0072  nput_filesr....r
+00000770: 0400 0000 7205 0000 0072 0600 0000 7207  ....r....r....r.
+00000780: 0000 0072 0800 0000 7209 0000 0072 1800  ...r....r....r..
+00000790: 0000 7218 0000 0072 1800 0000 7219 0000  ..r....r....r...
+000007a0: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
+000007b0: 0800 0000 0400 0c02 2002 140a            ........ ...
```

### Comparing `fluidsimfoam-0.0.5/src/fluidsimfoam/foam_input_files/__pycache__/control_dict.cpython-39.pyc` & `fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/__pycache__/control_dict.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun  1 13:07:51 2023 UTC, .py size: 2822 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 2798 7864 060b 0000  a.......'.xd....
+00000000: 6f0d 0d0a 0000 0000 03aa 7764 060b 0000  o.........wd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0011 0000 0040 0000 0073 7c00 0000 6400  .....@...s|...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 6d05 5a05 6d06 5a06  d.l.m.Z.m.Z.m.Z.
 00000050: 6d07 5a07 0100 6401 6404 6c08 6d09 5a09  m.Z...d.d.l.m.Z.
 00000060: 0100 650a 6405 6406 6401 6407 6408 6409  ..e.d.d.d.d.d.d.
 00000070: 640a 640b 6401 640c 640d 640e 640f 640d  d.d.d.d.d.d.d.d.
@@ -19,16 +19,16 @@
 00000120: 6d73 5f64 6963 7429 01da 0761 735f 6469  ms_dict)...as_di
 00000130: 6374 5a07 6963 6f46 6f61 6dda 0973 7461  ctZ.icoFoam..sta
 00000140: 7274 5469 6d65 da07 656e 6454 696d 6567  rtTime..endTimeg
 00000150: 0000 0000 0000 e03f 677b 14ae 47e1 7a74  .......?g{..G.zt
 00000160: 3f5a 0874 696d 6553 7465 70e9 1400 0000  ?Z.timeStep.....
 00000170: da05 6173 6369 69e9 0600 0000 da03 6f66  ..ascii.......of
 00000180: 66da 0767 656e 6572 616c da04 7472 7565  f..general..true
-00000190: 290f da0b 6170 706c 6963 6174 696f 6e5a  )...applicationZ
-000001a0: 0973 7461 7274 4672 6f6d 7208 0000 005a  .startFromr....Z
+00000190: 290f 5a0b 6170 706c 6963 6174 696f 6e5a  ).Z.applicationZ
+000001a0: 0973 7461 7274 4672 6f6d 7208 0000 00da  .startFromr.....
 000001b0: 0673 746f 7041 7472 0900 0000 5a06 6465  .stopAtr....Z.de
 000001c0: 6c74 6154 5a0c 7772 6974 6543 6f6e 7472  ltaTZ.writeContr
 000001d0: 6f6c 5a0d 7772 6974 6549 6e74 6572 7661  olZ.writeInterva
 000001e0: 6c5a 0a70 7572 6765 5772 6974 655a 0b77  lZ.purgeWriteZ.w
 000001f0: 7269 7465 466f 726d 6174 5a0e 7772 6974  riteFormatZ.writ
 00000200: 6550 7265 6369 7369 6f6e 5a10 7772 6974  ePrecisionZ.writ
 00000210: 6543 6f6d 7072 6573 7369 6f6e 5a0a 7469  eCompressionZ.ti
@@ -42,176 +42,176 @@
 00000290: 6f6e 4e63 0400 0000 0000 0000 0000 0000  onNc............
 000002a0: 0400 0000 0200 0000 4300 0000 7316 0000  ........C...s...
 000002b0: 007c 017c 005f 007c 027c 005f 017c 037c  .|.|._.|.|._.|.|
 000002c0: 005f 0264 0053 00a9 014e 2903 da04 7479  ._.d.S...N)...ty
 000002d0: 7065 da04 6c69 6273 da07 656e 7472 6965  pe..libs..entrie
 000002e0: 7329 04da 0473 656c 6672 1300 0000 7214  s)...selfr....r.
 000002f0: 0000 0072 1500 0000 a900 7217 0000 00fa  ...r......r.....
-00000300: 582f 686f 6d65 2f75 7365 7273 2f61 7567  X/home/users/aug
-00000310: 6965 7233 7069 2f44 6576 2f66 6c75 6964  ier3pi/Dev/fluid
-00000320: 7369 6d66 6f61 6d2f 7372 632f 666c 7569  simfoam/src/flui
-00000330: 6473 696d 666f 616d 2f66 6f61 6d5f 696e  dsimfoam/foam_in
-00000340: 7075 745f 6669 6c65 732f 636f 6e74 726f  put_files/contro
-00000350: 6c5f 6469 6374 2e70 79da 085f 5f69 6e69  l_dict.py..__ini
-00000360: 745f 5f22 0000 0073 0600 0000 0001 0601  t__"...s........
-00000370: 0601 7a11 4675 6e63 7469 6f6e 2e5f 5f69  ..z.Function.__i
-00000380: 6e69 745f 5f63 0100 0000 0000 0000 0000  nit__c..........
-00000390: 0000 0200 0000 0600 0000 4300 0000 7330  ..........C...s0
-000003a0: 0000 007c 006a 007c 006a 0164 019c 027d  ...|.j.|.j.d...}
-000003b0: 017c 006a 0264 0075 0172 2c7c 01a0 0374  .|.j.d.u.r,|...t
-000003c0: 047c 006a 0264 0264 038d 02a1 0101 007c  .|.j.d.d.......|
-000003d0: 0153 0029 044e 2902 7213 0000 0072 1400  .S.).N).r....r..
-000003e0: 0000 4629 015a 0f66 696c 7465 725f 636f  ..F).Z.filter_co
-000003f0: 6d6d 656e 7473 2905 7213 0000 0072 1400  mments).r....r..
-00000400: 0000 7215 0000 00da 0675 7064 6174 6572  ..r......updater
-00000410: 0700 0000 2902 7216 0000 00da 0464 6174  ....).r......dat
-00000420: 6172 1700 0000 7217 0000 0072 1800 0000  ar....r....r....
-00000430: da09 6d61 6b65 5f64 6963 7427 0000 0073  ..make_dict'...s
-00000440: 0800 0000 0001 0e01 0a01 1401 7a12 4675  ............z.Fu
-00000450: 6e63 7469 6f6e 2e6d 616b 655f 6469 6374  nction.make_dict
-00000460: 2901 4e29 05da 085f 5f6e 616d 655f 5fda  ).N)...__name__.
-00000470: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
-00000480: 7561 6c6e 616d 655f 5f72 1900 0000 721c  ualname__r....r.
-00000490: 0000 0072 1700 0000 7217 0000 0072 1700  ...r....r....r..
-000004a0: 0000 7218 0000 0072 1100 0000 2100 0000  ..r....r....!...
-000004b0: 7304 0000 0008 010a 0572 1100 0000 6300  s........r....c.
-000004c0: 0000 0000 0000 0000 0000 0000 0000 0003  ................
-000004d0: 0000 0040 0000 0073 4e00 0000 6500 5a01  ...@...sN...e.Z.
-000004e0: 6400 5a02 6410 6402 6403 8401 5a03 6404  d.Z.d.d.d...Z.d.
-000004f0: 6405 8400 5a04 6406 6407 8400 5a05 6411  d...Z.d.d...Z.d.
-00000500: 6408 6409 8401 5a06 6412 640a 640b 8401  d.d...Z.d.d.d...
-00000510: 5a07 6413 640c 640d 8401 5a08 6414 640e  Z.d.d.d...Z.d.d.
-00000520: 640f 8401 5a09 6401 5300 2915 da11 436f  d...Z.d.S.)...Co
-00000530: 6e74 726f 6c44 6963 7448 656c 7065 724e  ntrolDictHelperN
-00000540: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
-00000550: 0004 0000 0043 0000 0073 3200 0000 7400  .....C...s2...t.
-00000560: a001 a100 7c00 5f02 7c01 6400 7501 7222  ....|._.|.d.u.r"
-00000570: 7c00 6a02 a003 7404 7c01 8301 a101 0100  |.j...t.|.......
-00000580: 6900 7c00 5f05 6900 7c00 5f06 6400 5300  i.|._.i.|._.d.S.
-00000590: 7212 0000 0029 07da 1444 4546 4155 4c54  r....)...DEFAULT
-000005a0: 5f43 4f4e 5452 4f4c 5f44 4943 54da 0463  _CONTROL_DICT..c
-000005b0: 6f70 79da 1b64 6566 6175 6c74 5f63 6f6e  opy..default_con
-000005c0: 7472 6f6c 5f64 6963 745f 7061 7261 6d73  trol_dict_params
-000005d0: 721a 0000 0072 0700 0000 da09 6675 6e63  r....r......func
-000005e0: 7469 6f6e 73da 1266 756e 6374 696f 6e73  tions..functions
-000005f0: 5f69 6e63 6c75 6465 64a9 0272 1600 0000  _included..r....
-00000600: da07 6465 6661 756c 7472 1700 0000 7217  ..defaultr....r.
-00000610: 0000 0072 1800 0000 7219 0000 002f 0000  ...r....r..../..
-00000620: 0073 0a00 0000 0001 0a01 0801 1002 0601  .s..............
-00000630: 7a1a 436f 6e74 726f 6c44 6963 7448 656c  z.ControlDictHel
-00000640: 7065 722e 5f5f 696e 6974 5f5f 6302 0000  per.__init__c...
-00000650: 0000 0000 0000 0000 0002 0000 0004 0000  ................
-00000660: 0043 0000 0073 1200 0000 7400 7c01 6401  .C...s....t.|.d.
-00000670: 7c00 6a01 8303 0100 6400 5300 2902 4eda  |.j.....d.S.).N.
-00000680: 0c63 6f6e 7472 6f6c 5f64 6963 7429 0272  .control_dict).r
-00000690: 0600 0000 7223 0000 0029 0272 1600 0000  ....r#...).r....
-000006a0: da06 7061 7261 6d73 7217 0000 0072 1700  ..paramsr....r..
-000006b0: 0000 7218 0000 00da 0f63 6f6d 706c 6574  ..r......complet
-000006c0: 655f 7061 7261 6d73 3700 0000 7306 0000  e_params7...s...
-000006d0: 0000 0102 0108 ff7a 2143 6f6e 7472 6f6c  .......z!Control
-000006e0: 4469 6374 4865 6c70 6572 2e63 6f6d 706c  DictHelper.compl
-000006f0: 6574 655f 7061 7261 6d73 6302 0000 0000  ete_paramsc.....
-00000700: 0000 0000 0000 0007 0000 0007 0000 0003  ................
-00000710: 0000 0073 9a00 0000 7400 6401 6402 6403  ...s....t.d.d.d.
-00000720: 6404 6405 6406 9c05 8700 6601 6407 6408  d.d.d.....f.d.d.
-00000730: 8408 7c00 6a01 a002 a100 4400 8301 7403  ..|.j.....D...t.
-00000740: 6409 8d03 7d02 6900 7d03 7c00 6a04 a005  d...}.i.}.|.j...
-00000750: a100 4400 5d26 5c02 7d04 7d05 7c05 6400  ..D.]&\.}.}.|.d.
-00000760: 7500 7250 640a 7d05 6400 7c03 7c05 9b00  u.rPd.}.d.|.|...
-00000770: 640b 7c04 9b00 9d03 3c00 713c 7c00 6a06  d.|.....<.q<|.j.
-00000780: a005 a100 4400 5d14 5c02 7d04 7d06 7c06  ....D.].\.}.}.|.
-00000790: a007 a100 7c03 7c04 3c00 716e 7c03 7296  ....|.|.<.qn|.r.
-000007a0: 7c02 a008 640c 7c03 6901 a101 0100 7c02  |...d.|.i.....|.
-000007b0: 5300 290d 4e7a 0332 2e30 720b 0000 00da  S.).Nz.2.0r.....
-000007c0: 0a64 6963 7469 6f6e 6172 797a 0822 7379  .dictionaryz."sy
-000007d0: 7374 656d 225a 0b63 6f6e 7472 6f6c 4469  stem"Z.controlDi
-000007e0: 6374 2905 da07 7665 7273 696f 6eda 0666  ct)...version..f
-000007f0: 6f72 6d61 74da 0563 6c61 7373 da08 6c6f  ormat..class..lo
-00000800: 6361 7469 6f6e da06 6f62 6a65 6374 6301  cation..objectc.
-00000810: 0000 0000 0000 0000 0000 0002 0000 0006  ................
-00000820: 0000 0013 0000 0073 1c00 0000 6900 7c00  .......s....i.|.
-00000830: 5d14 7d01 7c01 8800 6a00 7401 7c01 8301  ].}.|...j.t.|...
-00000840: 1900 9302 7104 5300 7217 0000 0029 0272  ....q.S.r....).r
-00000850: 2800 0000 7202 0000 0029 02da 022e 30da  (...r....)....0.
-00000860: 036b 6579 a901 7229 0000 0072 1700 0000  .key..r)...r....
-00000870: 7218 0000 00da 0a3c 6469 6374 636f 6d70  r......<dictcomp
-00000880: 3e45 0000 0073 0400 0000 0602 02ff 7a2f  >E...s........z/
-00000890: 436f 6e74 726f 6c44 6963 7448 656c 7065  ControlDictHelpe
-000008a0: 722e 6d61 6b65 5f74 7265 652e 3c6c 6f63  r.make_tree.<loc
-000008b0: 616c 733e 2e3c 6469 6374 636f 6d70 3e29  als>.<dictcomp>)
-000008c0: 03da 0469 6e66 6fda 0863 6869 6c64 7265  ...info..childre
-000008d0: 6eda 0668 6561 6465 727a 0c23 696e 636c  n..headerz.#incl
-000008e0: 7564 6546 756e 63fa 0120 7224 0000 0029  udeFunc.. r$...)
-000008f0: 0972 0500 0000 7223 0000 00da 046b 6579  .r....r#.....key
-00000900: 7372 0300 0000 7225 0000 00da 0569 7465  sr....r%.....ite
-00000910: 6d73 7224 0000 0072 1c00 0000 da14 696e  msr$...r......in
-00000920: 6974 5f66 726f 6d5f 7079 5f6f 626a 6563  it_from_py_objec
-00000930: 7473 2907 7216 0000 0072 2900 0000 da04  ts).r....r).....
-00000940: 7472 6565 721b 0000 00da 046e 616d 65da  treer......name.
-00000950: 046b 696e 64da 0866 756e 6374 696f 6e72  .kind..functionr
-00000960: 1700 0000 7233 0000 0072 1800 0000 da09  ....r3...r......
-00000970: 6d61 6b65 5f74 7265 653c 0000 0073 2c00  make_tree<...s,.
-00000980: 0000 0001 0202 0201 0201 0201 0201 02fb  ................
-00000990: 0407 0a02 08fe 0404 02f4 060f 0401 1201  ................
-000009a0: 0801 0401 1401 1201 0e01 0401 0e02 7a1b  ..............z.
-000009b0: 436f 6e74 726f 6c44 6963 7448 656c 7065  ControlDictHelpe
-000009c0: 722e 6d61 6b65 5f74 7265 6563 0200 0000  r.make_treec....
-000009d0: 0000 0000 0000 0000 0200 0000 0200 0000  ................
-000009e0: 4300 0000 730c 0000 0074 007c 0083 017c  C...s....t.|...|
-000009f0: 0183 0153 0072 1200 0000 2901 7213 0000  ...S.r....).r...
-00000a00: 0072 2600 0000 7217 0000 0072 1700 0000  .r&...r....r....
-00000a10: 7218 0000 00da 036e 6577 5800 0000 7302  r......newX...s.
-00000a20: 0000 0000 017a 1543 6f6e 7472 6f6c 4469  .....z.ControlDi
-00000a30: 6374 4865 6c70 6572 2e6e 6577 6305 0000  ctHelper.newc...
-00000a40: 0000 0000 0000 0000 0005 0000 0004 0000  ................
-00000a50: 0043 0000 0073 1600 0000 7400 7c02 7c03  .C...s....t.|.|.
-00000a60: 7c04 8303 7c00 6a01 7c01 3c00 6400 5300  |...|.j.|.<.d.S.
-00000a70: 7212 0000 0029 0272 1100 0000 7224 0000  r....).r....r$..
-00000a80: 0029 0572 1600 0000 7232 0000 0072 1300  .).r....r2...r..
-00000a90: 0000 7214 0000 0072 1500 0000 7217 0000  ..r....r....r...
-00000aa0: 0072 1700 0000 7218 0000 00da 0c61 6464  .r....r......add
-00000ab0: 5f66 756e 6374 696f 6e5b 0000 0073 0200  _function[...s..
-00000ac0: 0000 0001 7a1e 436f 6e74 726f 6c44 6963  ....z.ControlDic
-00000ad0: 7448 656c 7065 722e 6164 645f 6675 6e63  tHelper.add_func
-00000ae0: 7469 6f6e 6303 0000 0000 0000 0000 0000  tionc...........
-00000af0: 0003 0000 0003 0000 0043 0000 0073 0e00  .........C...s..
-00000b00: 0000 7c02 7c00 6a00 7c01 3c00 6400 5300  ..|.|.j.|.<.d.S.
-00000b10: 7212 0000 0029 0172 2500 0000 2903 7216  r....).r%...).r.
-00000b20: 0000 0072 3d00 0000 723e 0000 0072 1700  ...r=...r>...r..
-00000b30: 0000 7217 0000 0072 1800 0000 da10 696e  ..r....r......in
-00000b40: 636c 7564 655f 6675 6e63 7469 6f6e 5e00  clude_function^.
-00000b50: 0000 7302 0000 0000 017a 2243 6f6e 7472  ..s......z"Contr
-00000b60: 6f6c 4469 6374 4865 6c70 6572 2e69 6e63  olDictHelper.inc
-00000b70: 6c75 6465 5f66 756e 6374 696f 6e63 0300  lude_functionc..
-00000b80: 0000 0000 0000 0000 0000 0400 0000 0500  ................
-00000b90: 0000 4300 0000 731a 0000 007c 0144 005d  ..C...s....|.D.]
-00000ba0: 107d 037c 00a0 007c 037c 02a1 0201 0071  .}.|...|.|.....q
-00000bb0: 0464 0053 0072 1200 0000 2901 7243 0000  .d.S.r....).rC..
-00000bc0: 0029 0472 1600 0000 da05 6e61 6d65 7372  .).r......namesr
-00000bd0: 3e00 0000 723d 0000 0072 1700 0000 7217  >...r=...r....r.
-00000be0: 0000 0072 1800 0000 da11 696e 636c 7564  ...r......includ
-00000bf0: 655f 6675 6e63 7469 6f6e 7361 0000 0073  e_functionsa...s
-00000c00: 0400 0000 0001 0801 7a23 436f 6e74 726f  ........z#Contro
-00000c10: 6c44 6963 7448 656c 7065 722e 696e 636c  lDictHelper.incl
-00000c20: 7564 655f 6675 6e63 7469 6f6e 7329 014e  ude_functions).N
-00000c30: 2901 4e29 014e 2901 4e29 014e 290a 721d  ).N).N).N).N).r.
-00000c40: 0000 0072 1e00 0000 721f 0000 0072 1900  ...r....r....r..
-00000c50: 0000 722a 0000 0072 4000 0000 7241 0000  ..r*...r@...rA..
-00000c60: 0072 4200 0000 7243 0000 0072 4500 0000  .rB...rC...rE...
-00000c70: 7217 0000 0072 1700 0000 7217 0000 0072  r....r....r....r
-00000c80: 1800 0000 7220 0000 002e 0000 0073 0e00  ....r .......s..
-00000c90: 0000 0801 0a08 0805 081c 0a03 0a03 0a03  ................
-00000ca0: 7220 0000 004e 290e da07 5f5f 646f 635f  r ...N)...__doc_
-00000cb0: 5fda 0a69 6e66 6c65 6374 696f 6e72 0200  _..inflectionr..
-00000cc0: 0000 5a1d 666c 7569 6473 696d 666f 616d  ..Z.fluidsimfoam
-00000cd0: 2e66 6f61 6d5f 696e 7075 745f 6669 6c65  .foam_input_file
-00000ce0: 7372 0300 0000 7204 0000 0072 0500 0000  sr....r....r....
-00000cf0: 7206 0000 005a 2266 6c75 6964 7369 6d66  r....Z"fluidsimf
-00000d00: 6f61 6d2e 666f 616d 5f69 6e70 7574 5f66  oam.foam_input_f
-00000d10: 696c 6573 2e75 7469 6c72 0700 0000 da04  iles.utilr......
-00000d20: 6469 6374 7221 0000 0072 1100 0000 7220  dictr!...r....r 
-00000d30: 0000 0072 1700 0000 7217 0000 0072 1700  ...r....r....r..
-00000d40: 0000 7218 0000 00da 083c 6d6f 6475 6c65  ..r......<module
-00000d50: 3e01 0000 0073 2c00 0000 0402 0c02 1806  >....s,.........
-00000d60: 0c03 0201 0201 0201 0201 0201 0201 0201  ................
-00000d70: 0201 0201 0201 0201 0201 0201 0201 0201  ................
-00000d80: 02f1 0613 0e0d                           ......
+00000300: 4f2f 686f 6d65 2f70 6965 7272 652f 4465  O/home/pierre/De
+00000310: 762f 666c 7569 6473 696d 666f 616d 2f73  v/fluidsimfoam/s
+00000320: 7263 2f66 6c75 6964 7369 6d66 6f61 6d2f  rc/fluidsimfoam/
+00000330: 666f 616d 5f69 6e70 7574 5f66 696c 6573  foam_input_files
+00000340: 2f63 6f6e 7472 6f6c 5f64 6963 742e 7079  /control_dict.py
+00000350: da08 5f5f 696e 6974 5f5f 2200 0000 7306  ..__init__"...s.
+00000360: 0000 0006 0106 010a 017a 1146 756e 6374  .........z.Funct
+00000370: 696f 6e2e 5f5f 696e 6974 5f5f 6301 0000  ion.__init__c...
+00000380: 0000 0000 0000 0000 0002 0000 0006 0000  ................
+00000390: 0043 0000 0073 3000 0000 7c00 6a00 7c00  .C...s0...|.j.|.
+000003a0: 6a01 6401 9c02 7d01 7c00 6a02 6400 7501  j.d...}.|.j.d.u.
+000003b0: 7216 7c01 a003 7404 7c00 6a02 6402 6403  r.|...t.|.j.d.d.
+000003c0: 8d02 a101 0100 7c01 5300 2904 4e29 0272  ......|.S.).N).r
+000003d0: 1300 0000 7214 0000 0046 2901 5a0f 6669  ....r....F).Z.fi
+000003e0: 6c74 6572 5f63 6f6d 6d65 6e74 7329 0572  lter_comments).r
+000003f0: 1300 0000 7214 0000 0072 1500 0000 da06  ....r....r......
+00000400: 7570 6461 7465 7207 0000 0029 0272 1600  updater....).r..
+00000410: 0000 da04 6461 7461 7217 0000 0072 1700  ....datar....r..
+00000420: 0000 7218 0000 00da 096d 616b 655f 6469  ..r......make_di
+00000430: 6374 2700 0000 7308 0000 000e 010a 0114  ct'...s.........
+00000440: 0104 017a 1246 756e 6374 696f 6e2e 6d61  ...z.Function.ma
+00000450: 6b65 5f64 6963 7472 1200 0000 2905 da08  ke_dictr....)...
+00000460: 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f 6475  __name__..__modu
+00000470: 6c65 5f5f da0c 5f5f 7175 616c 6e61 6d65  le__..__qualname
+00000480: 5f5f 7219 0000 0072 1c00 0000 7217 0000  __r....r....r...
+00000490: 0072 1700 0000 7217 0000 0072 1800 0000  .r....r....r....
+000004a0: 7211 0000 0021 0000 0073 0600 0000 0800  r....!...s......
+000004b0: 0a01 0c05 7211 0000 0063 0000 0000 0000  ....r....c......
+000004c0: 0000 0000 0000 0000 0000 0300 0000 4000  ..............@.
+000004d0: 0000 734e 0000 0065 005a 0164 005a 0264  ..sN...e.Z.d.Z.d
+000004e0: 1064 0264 0384 015a 0364 0464 0584 005a  .d.d...Z.d.d...Z
+000004f0: 0464 0664 0784 005a 0564 1064 0864 0984  .d.d...Z.d.d.d..
+00000500: 015a 0664 1064 0a64 0b84 015a 0764 1064  .Z.d.d.d...Z.d.d
+00000510: 0c64 0d84 015a 0864 1064 0e64 0f84 015a  .d...Z.d.d.d...Z
+00000520: 0964 0153 0029 11da 1143 6f6e 7472 6f6c  .d.S.)...Control
+00000530: 4469 6374 4865 6c70 6572 4e63 0200 0000  DictHelperNc....
+00000540: 0000 0000 0000 0000 0200 0000 0400 0000  ................
+00000550: 4300 0000 7332 0000 0074 00a0 01a1 007c  C...s2...t.....|
+00000560: 005f 027c 0164 0075 0172 117c 006a 02a0  ._.|.d.u.r.|.j..
+00000570: 0374 047c 0183 01a1 0101 0069 007c 005f  .t.|.......i.|._
+00000580: 0569 007c 005f 0664 0053 0072 1200 0000  .i.|._.d.S.r....
+00000590: 2907 da14 4445 4641 554c 545f 434f 4e54  )...DEFAULT_CONT
+000005a0: 524f 4c5f 4449 4354 da04 636f 7079 da1b  ROL_DICT..copy..
+000005b0: 6465 6661 756c 745f 636f 6e74 726f 6c5f  default_control_
+000005c0: 6469 6374 5f70 6172 616d 7372 1a00 0000  dict_paramsr....
+000005d0: 7207 0000 00da 0966 756e 6374 696f 6e73  r......functions
+000005e0: da12 6675 6e63 7469 6f6e 735f 696e 636c  ..functions_incl
+000005f0: 7564 6564 a902 7216 0000 00da 0764 6566  uded..r......def
+00000600: 6175 6c74 7217 0000 0072 1700 0000 7218  aultr....r....r.
+00000610: 0000 0072 1900 0000 2f00 0000 730a 0000  ...r..../...s...
+00000620: 000a 0108 0110 0106 020a 017a 1a43 6f6e  ...........z.Con
+00000630: 7472 6f6c 4469 6374 4865 6c70 6572 2e5f  trolDictHelper._
+00000640: 5f69 6e69 745f 5f63 0200 0000 0000 0000  _init__c........
+00000650: 0000 0000 0200 0000 0400 0000 4300 0000  ............C...
+00000660: 7312 0000 0074 007c 0164 017c 006a 0183  s....t.|.d.|.j..
+00000670: 0301 0064 0053 0029 024e da0c 636f 6e74  ...d.S.).N..cont
+00000680: 726f 6c5f 6469 6374 2902 7206 0000 0072  rol_dict).r....r
+00000690: 2300 0000 2902 7216 0000 00da 0670 6172  #...).r......par
+000006a0: 616d 7372 1700 0000 7217 0000 0072 1800  amsr....r....r..
+000006b0: 0000 da0f 636f 6d70 6c65 7465 5f70 6172  ....complete_par
+000006c0: 616d 7337 0000 0073 0600 0000 0201 0801  ams7...s........
+000006d0: 08ff 7a21 436f 6e74 726f 6c44 6963 7448  ..z!ControlDictH
+000006e0: 656c 7065 722e 636f 6d70 6c65 7465 5f70  elper.complete_p
+000006f0: 6172 616d 7363 0200 0000 0000 0000 0000  aramsc..........
+00000700: 0000 0700 0000 0700 0000 0300 0000 739a  ..............s.
+00000710: 0000 0074 0064 0164 0264 0364 0464 0564  ...t.d.d.d.d.d.d
+00000720: 069c 0587 0066 0164 0764 0884 087c 006a  .....f.d.d...|.j
+00000730: 01a0 02a1 0044 0083 0174 0364 098d 037d  .....D...t.d...}
+00000740: 0269 007d 037c 006a 04a0 05a1 0044 005d  .i.}.|.j.....D.]
+00000750: 135c 027d 047d 057c 0564 0075 0072 2864  .\.}.}.|.d.u.r(d
+00000760: 0a7d 0564 007c 037c 059b 0064 0b7c 049b  .}.d.|.|...d.|..
+00000770: 009d 033c 0071 1e7c 006a 06a0 05a1 0044  ...<.q.|.j.....D
+00000780: 005d 0a5c 027d 047d 067c 06a0 07a1 007c  .].\.}.}.|.....|
+00000790: 037c 043c 0071 377c 0372 4b7c 02a0 0864  .|.<.q7|.rK|...d
+000007a0: 0c7c 0369 01a1 0101 007c 0253 0029 0d4e  .|.i.....|.S.).N
+000007b0: 7a03 322e 3072 0b00 0000 da0a 6469 6374  z.2.0r......dict
+000007c0: 696f 6e61 7279 7a08 2273 7973 7465 6d22  ionaryz."system"
+000007d0: da0b 636f 6e74 726f 6c44 6963 7429 05da  ..controlDict)..
+000007e0: 0776 6572 7369 6f6e da06 666f 726d 6174  .version..format
+000007f0: da05 636c 6173 73da 086c 6f63 6174 696f  ..class..locatio
+00000800: 6eda 066f 626a 6563 7463 0100 0000 0000  n..objectc......
+00000810: 0000 0000 0000 0200 0000 0600 0000 1300  ................
+00000820: 0000 731c 0000 0069 007c 005d 0a7d 017c  ..s....i.|.].}.|
+00000830: 0188 006a 0074 017c 0183 0119 0093 0271  ...j.t.|.......q
+00000840: 0253 0072 1700 0000 2902 7228 0000 0072  .S.r....).r(...r
+00000850: 0200 0000 2902 da02 2e30 da03 6b65 79a9  ....)....0..key.
+00000860: 0172 2900 0000 7217 0000 0072 1800 0000  .r)...r....r....
+00000870: da0a 3c64 6963 7463 6f6d 703e 4500 0000  ..<dictcomp>E...
+00000880: 7308 0000 0006 0002 020e ff06 ff7a 2f43  s............z/C
+00000890: 6f6e 7472 6f6c 4469 6374 4865 6c70 6572  ontrolDictHelper
+000008a0: 2e6d 616b 655f 7472 6565 2e3c 6c6f 6361  .make_tree.<loca
+000008b0: 6c73 3e2e 3c64 6963 7463 6f6d 703e 2903  ls>.<dictcomp>).
+000008c0: da04 696e 666f da08 6368 696c 6472 656e  ..info..children
+000008d0: da06 6865 6164 6572 7a0c 2369 6e63 6c75  ..headerz.#inclu
+000008e0: 6465 4675 6e63 da01 2072 2400 0000 2909  deFunc.. r$...).
+000008f0: 7205 0000 0072 2300 0000 da04 6b65 7973  r....r#.....keys
+00000900: 7203 0000 0072 2500 0000 da05 6974 656d  r....r%.....item
+00000910: 7372 2400 0000 721c 0000 00da 1469 6e69  sr$...r......ini
+00000920: 745f 6672 6f6d 5f70 795f 6f62 6a65 6374  t_from_py_object
+00000930: 7329 0772 1600 0000 7229 0000 00da 0474  s).r....r).....t
+00000940: 7265 6572 1b00 0000 da04 6e61 6d65 da04  reer......name..
+00000950: 6b69 6e64 da08 6675 6e63 7469 6f6e 7217  kind..functionr.
+00000960: 0000 0072 3400 0000 7218 0000 00da 096d  ...r4...r......m
+00000970: 616b 655f 7472 6565 3c00 0000 732c 0000  ake_tree<...s,..
+00000980: 0002 0102 0202 0102 0102 0102 0104 fb0a  ................
+00000990: 0708 0204 fe02 0406 f404 0f12 0108 0104  ................
+000009a0: 0114 0112 010e 0104 010e 0104 027a 1b43  .............z.C
+000009b0: 6f6e 7472 6f6c 4469 6374 4865 6c70 6572  ontrolDictHelper
+000009c0: 2e6d 616b 655f 7472 6565 6302 0000 0000  .make_treec.....
+000009d0: 0000 0000 0000 0002 0000 0002 0000 0043  ...............C
+000009e0: 0000 0073 0c00 0000 7400 7c00 8301 7c01  ...s....t.|...|.
+000009f0: 8301 5300 7212 0000 0029 0172 1300 0000  ..S.r....).r....
+00000a00: 7226 0000 0072 1700 0000 7217 0000 0072  r&...r....r....r
+00000a10: 1800 0000 da03 6e65 7758 0000 0073 0200  ......newX...s..
+00000a20: 0000 0c01 7a15 436f 6e74 726f 6c44 6963  ....z.ControlDic
+00000a30: 7448 656c 7065 722e 6e65 7763 0500 0000  tHelper.newc....
+00000a40: 0000 0000 0000 0000 0500 0000 0400 0000  ................
+00000a50: 4300 0000 7316 0000 0074 007c 027c 037c  C...s....t.|.|.|
+00000a60: 0483 037c 006a 017c 013c 0064 0053 0072  ...|.j.|.<.d.S.r
+00000a70: 1200 0000 2902 7211 0000 0072 2400 0000  ....).r....r$...
+00000a80: 2905 7216 0000 0072 3300 0000 7213 0000  ).r....r3...r...
+00000a90: 0072 1400 0000 7215 0000 0072 1700 0000  .r....r....r....
+00000aa0: 7217 0000 0072 1800 0000 da0c 6164 645f  r....r......add_
+00000ab0: 6675 6e63 7469 6f6e 5b00 0000 7302 0000  function[...s...
+00000ac0: 0016 017a 1e43 6f6e 7472 6f6c 4469 6374  ...z.ControlDict
+00000ad0: 4865 6c70 6572 2e61 6464 5f66 756e 6374  Helper.add_funct
+00000ae0: 696f 6e63 0300 0000 0000 0000 0000 0000  ionc............
+00000af0: 0300 0000 0300 0000 4300 0000 730e 0000  ........C...s...
+00000b00: 007c 027c 006a 007c 013c 0064 0053 0072  .|.|.j.|.<.d.S.r
+00000b10: 1200 0000 2901 7225 0000 0029 0372 1600  ....).r%...).r..
+00000b20: 0000 723e 0000 0072 3f00 0000 7217 0000  ..r>...r?...r...
+00000b30: 0072 1700 0000 7218 0000 00da 1069 6e63  .r....r......inc
+00000b40: 6c75 6465 5f66 756e 6374 696f 6e5e 0000  lude_function^..
+00000b50: 0073 0200 0000 0e01 7a22 436f 6e74 726f  .s......z"Contro
+00000b60: 6c44 6963 7448 656c 7065 722e 696e 636c  lDictHelper.incl
+00000b70: 7564 655f 6675 6e63 7469 6f6e 6303 0000  ude_functionc...
+00000b80: 0000 0000 0000 0000 0004 0000 0005 0000  ................
+00000b90: 0043 0000 0073 1a00 0000 7c01 4400 5d08  .C...s....|.D.].
+00000ba0: 7d03 7c00 a000 7c03 7c02 a102 0100 7102  }.|...|.|.....q.
+00000bb0: 6400 5300 7212 0000 0029 0172 4400 0000  d.S.r....).rD...
+00000bc0: 2904 7216 0000 00da 056e 616d 6573 723f  ).r......namesr?
+00000bd0: 0000 0072 3e00 0000 7217 0000 0072 1700  ...r>...r....r..
+00000be0: 0000 7218 0000 00da 1169 6e63 6c75 6465  ..r......include
+00000bf0: 5f66 756e 6374 696f 6e73 6100 0000 7306  _functionsa...s.
+00000c00: 0000 0008 010e 0104 ff7a 2343 6f6e 7472  .........z#Contr
+00000c10: 6f6c 4469 6374 4865 6c70 6572 2e69 6e63  olDictHelper.inc
+00000c20: 6c75 6465 5f66 756e 6374 696f 6e73 7212  lude_functionsr.
+00000c30: 0000 0029 0a72 1d00 0000 721e 0000 0072  ...).r....r....r
+00000c40: 1f00 0000 7219 0000 0072 2a00 0000 7241  ....r....r*...rA
+00000c50: 0000 0072 4200 0000 7243 0000 0072 4400  ...rB...rC...rD.
+00000c60: 0000 7246 0000 0072 1700 0000 7217 0000  ..rF...r....r...
+00000c70: 0072 1700 0000 7218 0000 0072 2000 0000  .r....r....r ...
+00000c80: 2e00 0000 7310 0000 0008 000a 0108 0808  ....s...........
+00000c90: 050a 1c0a 030a 030e 0372 2000 0000 4e29  .........r ...N)
+00000ca0: 0eda 075f 5f64 6f63 5f5f da0a 696e 666c  ...__doc__..infl
+00000cb0: 6563 7469 6f6e 7202 0000 00da 1d66 6c75  ectionr......flu
+00000cc0: 6964 7369 6d66 6f61 6d2e 666f 616d 5f69  idsimfoam.foam_i
+00000cd0: 6e70 7574 5f66 696c 6573 7203 0000 0072  nput_filesr....r
+00000ce0: 0400 0000 7205 0000 0072 0600 0000 5a22  ....r....r....Z"
+00000cf0: 666c 7569 6473 696d 666f 616d 2e66 6f61  fluidsimfoam.foa
+00000d00: 6d5f 696e 7075 745f 6669 6c65 732e 7574  m_input_files.ut
+00000d10: 696c 7207 0000 00da 0464 6963 7472 2100  ilr......dictr!.
+00000d20: 0000 7211 0000 0072 2000 0000 7217 0000  ..r....r ...r...
+00000d30: 0072 1700 0000 7217 0000 0072 1800 0000  .r....r....r....
+00000d40: da08 3c6d 6f64 756c 653e 0100 0000 732e  ..<module>....s.
+00000d50: 0000 0004 000c 0218 020c 0602 0302 0102  ................
+00000d60: 0102 0102 0102 0102 0102 0102 0102 0102  ................
+00000d70: 0102 0102 0102 0102 0102 0106 f10e 1314  ................
+00000d80: 0d                                       .
```

### Comparing `fluidsimfoam-0.0.5/src/fluidsimfoam/foam_input_files/__pycache__/fields.cpython-310.pyc` & `fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/__pycache__/fields.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu May 11 13:43:46 2023 UTC, .py size: 5808 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 16% similar despite different names*

```diff
@@ -1,388 +1,448 @@
-00000000: 6f0d 0d0a 0000 0000 12f1 5c64 b016 0000  o.........\d....
+00000000: 6f0d 0d0a 0000 0000 7753 7664 111a 0000  o.......wSvd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 e000 0000 6400  .....@...s....d.
+00000020: 0004 0000 0040 0000 0073 f600 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 6d04 5a04 0100 6401 6404 6c05  m.Z.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6401 6405 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 0100 6401 6406 6c09 6d0a 5a0a 0100 6401  ..d.d.l.m.Z...d.
 00000070: 6402 6c0b 5a0c 6401 6407 6c0d 6d0e 5a0e  d.l.Z.d.d.l.m.Z.
 00000080: 0100 6401 6408 6c0f 6d10 5a10 6d11 5a11  ..d.d.l.m.Z.m.Z.
 00000090: 6d12 5a12 6d13 5a13 6d14 5a14 6d15 5a15  m.Z.m.Z.m.Z.m.Z.
-000000a0: 6d16 5a16 6d17 5a17 0100 6409 5a18 640a  m.Z.m.Z...d.Z.d.
-000000b0: 5a19 640b 5a1a 4700 640c 640d 8400 640d  Z.d.Z.G.d.d...d.
-000000c0: 6503 8303 5a1b 4700 640e 640f 8400 640f  e...Z.G.d.d...d.
-000000d0: 651b 8303 5a1c 4700 6410 6411 8400 6411  e...Z.G.d.d...d.
-000000e0: 651b 8303 5a1d 4700 6412 6413 8400 6413  e...Z.G.d.d...d.
-000000f0: 651b 8303 5a1e 651c 651d 651e 6414 9c03  e...Z.e.e.e.d...
-00000100: 5a1f 6415 6416 8400 5a20 6402 5300 2917  Z.d.d...Z d.S.).
-00000110: 7a1e 4865 6c70 6572 2074 6f20 6372 6561  z.Helper to crea
-00000120: 7465 2066 6965 6c64 2066 696c 6573 0a0a  te field files..
-00000130: e900 0000 004e 2902 da03 4142 43da 0e61  .....N)...ABC..a
-00000140: 6273 7472 6163 746d 6574 686f 6429 01da  bstractmethod)..
-00000150: 0853 7472 696e 6749 4f29 01da 064e 756d  .StringIO)...Num
-00000160: 6265 7229 01da 0450 6174 6829 01da 0570  ber)...Path)...p
-00000170: 6172 7365 2908 da04 436f 6465 da0a 436f  arse)...Code..Co
-00000180: 6465 5374 7265 616d da04 4469 6374 da0c  deStream..Dict..
-00000190: 4469 6d65 6e73 696f 6e53 6574 da0d 466f  DimensionSet..Fo
-000001a0: 616d 496e 7075 7446 696c 65da 044c 6973  amInputFile..Lis
-000001b0: 74da 0556 616c 7565 da0e 7374 7232 666f  t..Value..str2fo
-000001c0: 616d 5f75 6e69 7473 7a12 2369 6e63 6c75  am_unitsz.#inclu
-000001d0: 6465 2022 6676 4346 442e 4822 7a46 2d49  de "fvCFD.H"zF-I
-000001e0: 2428 4c49 425f 5352 4329 2f66 696e 6974  $(LIB_SRC)/finit
-000001f0: 6556 6f6c 756d 652f 6c6e 496e 636c 7564  eVolume/lnInclud
-00000200: 6520 5c0a 2d49 2428 4c49 425f 5352 4329  e \.-I$(LIB_SRC)
-00000210: 2f6d 6573 6854 6f6f 6c73 2f6c 6e49 6e63  /meshTools/lnInc
-00000220: 6c75 6465 7a1c 2d6c 6d65 7368 546f 6f6c  ludez.-lmeshTool
-00000230: 7320 5c0a 2d6c 6669 6e69 7465 566f 6c75  s \.-lfiniteVolu
-00000240: 6d65 6300 0000 0000 0000 0000 0000 0000  mec.............
-00000250: 0000 0004 0000 0040 0000 0073 8e00 0000  .......@...s....
-00000260: 6500 5a01 6400 5a02 5500 6503 6504 6401  e.Z.d.Z.U.e.e.d.
-00000270: 3c00 6505 6402 6503 6602 6403 6404 8404  <.e.d.e.f.d.d...
-00000280: 8301 5a06 6505 6405 6503 7017 6507 6602  ..Z.e.d.e.p.e.f.
-00000290: 6406 6407 8404 8301 5a08 6419 6409 640a  d.d.....Z.d.d.d.
-000002a0: 8401 5a09 640b 640c 8400 5a0a 640d 640e  ..Z.d.d...Z.d.d.
-000002b0: 8400 5a0b 650c 640f 6410 8400 8301 5a0d  ..Z.e.d.d.....Z.
-000002c0: 650e 650f 6510 6603 6411 6412 8401 5a11  e.e.e.f.d.d...Z.
-000002d0: 6419 6413 6414 8401 5a12 6415 6416 8400  d.d.d...Z.d.d...
-000002e0: 5a13 6417 6418 8400 5a14 6408 5300 291a  Z.d.d...Z.d.S.).
-000002f0: da08 4669 656c 6441 4243 da03 636c 73da  ..FieldABC..cls.
-00000300: 0463 6f64 6563 0200 0000 0000 0000 0000  .codec..........
-00000310: 0000 0a00 0000 0600 0000 4300 0000 73c4  ..........C...s.
-00000320: 0000 0064 017c 0176 0172 0f74 007c 0183  ...d.|.v.r.t.|..
-00000330: 017d 027c 0064 0064 007c 0264 028d 0353  .}.|.d.d.|.d...S
-00000340: 007c 01a0 0164 01a1 017d 037c 01a0 0264  .|...d...}.|...d
-00000350: 037c 03a1 027d 047c 01a0 0164 047c 037c  .|...}.|...d.|.|
-00000360: 04a1 037d 057c 01a0 0264 057c 037c 04a1  ...}.|...d.|.|..
-00000370: 037d 067c 0164 007c 0385 0219 0064 0617  .}.|.d.|.....d..
-00000380: 007c 017c 0464 0085 0219 0017 007d 0774  .|.|.d.......}.t
-00000390: 007c 0783 017d 027c 017c 0564 0717 007c  .|...}.|.|.d...|
-000003a0: 0685 0219 00a0 03a1 007d 087c 08a0 0464  .........}.|...d
-000003b0: 04a1 0172 5074 05a0 0664 0864 097c 08a1  ...rPt...d.d.|..
-000003c0: 037d 0874 07a0 0874 097c 0883 01a1 017d  .}.t...t.|.....}
-000003d0: 097c 097c 025f 0a7c 0064 0964 097c 027c  .|.|._.|.d.d.|.|
-000003e0: 0964 0a8d 0453 0029 0b4e 5a0a 6e6f 6e75  .d...S.).NZ.nonu
-000003f0: 6e69 666f 726d 2901 da04 7472 6565 da0d  niform)...tree..
-00000400: 626f 756e 6461 7279 4669 656c 64fa 0128  boundaryField..(
-00000410: fa01 297a 033b 0a0a e901 0000 007a 045b  ..)z.;.......z.[
-00000420: 2829 5dda 0029 0272 1300 0000 da06 7661  ()]..).r......va
-00000430: 6c75 6573 290b 7207 0000 00da 0569 6e64  lues).r......ind
-00000440: 6578 da06 7269 6e64 6578 da05 7374 7269  ex..rindex..stri
-00000450: 70da 0a73 7461 7274 7377 6974 68da 0272  p..startswith..r
-00000460: 65da 0373 7562 da02 6e70 da07 6c6f 6164  e..sub..np..load
-00000470: 7478 7472 0400 0000 da04 6461 7461 290a  txtr......data).
-00000480: 7211 0000 0072 1200 0000 7213 0000 005a  r....r....r....Z
-00000490: 1069 6e64 6578 5f6e 6f6e 756e 6966 6f72  .index_nonunifor
-000004a0: 6d5a 1369 6e64 6578 5f62 6f75 6e64 6172  mZ.index_boundar
-000004b0: 7946 6965 6c64 5a11 696e 6465 785f 6f70  yFieldZ.index_op
-000004c0: 656e 696e 675f 7061 725a 1169 6e64 6578  ening_parZ.index
-000004d0: 5f63 6c6f 7369 6e67 5f70 6172 5a0d 636f  _closing_parZ.co
-000004e0: 6465 5f74 6f5f 7061 7273 655a 0963 6f64  de_to_parseZ.cod
-000004f0: 655f 6461 7461 7222 0000 00a9 0072 2300  e_datar".....r#.
-00000500: 0000 fa52 2f68 6f6d 652f 7573 6572 732f  ...R/home/users/
-00000510: 6175 6769 6572 3370 692f 4465 762f 666c  augier3pi/Dev/fl
-00000520: 7569 6473 696d 666f 616d 2f73 7263 2f66  uidsimfoam/src/f
-00000530: 6c75 6964 7369 6d66 6f61 6d2f 666f 616d  luidsimfoam/foam
-00000540: 5f69 6e70 7574 5f66 696c 6573 2f66 6965  _input_files/fie
-00000550: 6c64 732e 7079 da09 6672 6f6d 5f63 6f64  lds.py..from_cod
-00000560: 6523 0000 0073 2400 0000 0802 0801 0e01  e#...s$.........
-00000570: 0a02 0c01 0e01 0401 0601 04ff 1a05 02ff  ................
-00000580: 0804 1401 0a02 0e01 0e02 0602 1001 7a12  ..............z.
-00000590: 4669 656c 6441 4243 2e66 726f 6d5f 636f  FieldABC.from_co
-000005a0: 6465 da04 7061 7468 6302 0000 0000 0000  de..pathc.......
-000005b0: 0000 0000 0003 0000 0004 0000 0043 0000  .............C..
-000005c0: 0073 2000 0000 7400 7c01 8301 7d01 7c00  .s ...t.|...}.|.
-000005d0: a001 7c01 a002 a100 a101 7d02 7c01 7c02  ..|.......}.|.|.
-000005e0: 5f03 7c02 5300 a901 4e29 0472 0600 0000  _.|.S...N).r....
-000005f0: 7225 0000 00da 0972 6561 645f 7465 7874  r%.....read_text
-00000600: 7226 0000 0029 0372 1100 0000 7226 0000  r&...).r....r&..
-00000610: 00da 0566 6965 6c64 7223 0000 0072 2300  ...fieldr#...r#.
-00000620: 0000 7224 0000 00da 0966 726f 6d5f 7061  ..r$.....from_pa
-00000630: 7468 3f00 0000 7308 0000 0008 020e 0106  th?...s.........
-00000640: 0104 017a 1246 6965 6c64 4142 432e 6672  ...z.FieldABC.fr
-00000650: 6f6d 5f70 6174 684e 6305 0000 0000 0000  om_pathNc.......
-00000660: 0000 0000 0006 0000 0005 0000 0043 0000  .............C..
-00000670: 0073 7400 0000 7c03 6400 7501 7208 7c03  .st...|.d.u.r.|.
-00000680: 7c00 5f00 6e24 6401 6402 7c00 6a01 7c01  |._.n$d.d.|.j.|.
-00000690: 6403 9c04 7d05 7402 7c02 7403 8302 731b  d...}.t.|.t...s.
-000006a0: 7403 7404 7c02 8301 8301 7d02 7405 7c05  t.t.|.....}.t.|.
-000006b0: 7c02 6400 6404 9c02 6405 8d02 7c00 5f00  |.d.d...d...|._.
-000006c0: 7c00 6a00 a006 6406 6900 a102 0100 7c04  |.j...d.i.....|.
-000006d0: 6400 7501 7235 7c00 a007 7c04 a101 0100  d.u.r5|...|.....
-000006e0: 6400 7c00 5f08 6400 5300 2907 4e7a 0332  d.|._.d.S.).Nz.2
-000006f0: 2e30 da05 6173 6369 6929 04da 0776 6572  .0..ascii)...ver
-00000700: 7369 6f6e da06 666f 726d 6174 da05 636c  sion..format..cl
-00000710: 6173 73da 066f 626a 6563 7429 02da 0a64  ass..object)...d
-00000720: 696d 656e 7369 6f6e 73da 0d69 6e74 6572  imensions..inter
-00000730: 6e61 6c46 6965 6c64 2901 da08 6368 696c  nalField)...chil
-00000740: 6472 656e 7214 0000 0029 0972 1300 0000  drenr....).r....
-00000750: 7211 0000 00da 0a69 7369 6e73 7461 6e63  r......isinstanc
-00000760: 6572 0b00 0000 720f 0000 0072 0c00 0000  er....r....r....
-00000770: da09 7365 745f 6368 696c 64da 0a73 6574  ..set_child..set
-00000780: 5f76 616c 7565 7372 2600 0000 2906 da04  _valuesr&...)...
-00000790: 7365 6c66 da04 6e61 6d65 da09 6469 6d65  self..name..dime
-000007a0: 6e73 696f 6e72 1300 0000 7219 0000 00da  nsionr....r.....
-000007b0: 0469 6e66 6f72 2300 0000 7223 0000 0072  .infor#...r#...r
-000007c0: 2400 0000 da08 5f5f 696e 6974 5f5f 4600  $.....__init__F.
-000007d0: 0000 7320 0000 0008 0108 0102 0302 0104  ..s ............
-000007e0: 0102 0106 fc0a 070c 0102 020a 0108 ff0e  ................
-000007f0: 0408 020a 010a 027a 1146 6965 6c64 4142  .......z.FieldAB
-00000800: 432e 5f5f 696e 6974 5f5f 6301 0000 0000  C.__init__c.....
-00000810: 0000 0000 0000 0001 0000 0002 0000 0043  ...............C
-00000820: 0000 0073 0a00 0000 7c00 6a00 a001 a100  ...s....|.j.....
-00000830: 5300 7227 0000 0029 0272 1300 0000 da04  S.r'...).r......
-00000840: 6475 6d70 a901 7236 0000 0072 2300 0000  dump..r6...r#...
-00000850: 7223 0000 0072 2400 0000 723b 0000 005f  r#...r$...r;..._
-00000860: 0000 0073 0200 0000 0a01 7a0d 4669 656c  ...s......z.Fiel
-00000870: 6441 4243 2e64 756d 7063 0100 0000 0000  dABC.dumpc......
-00000880: 0000 0000 0000 0200 0000 0800 0000 4300  ..............C.
-00000890: 0000 7352 0000 007c 006a 0064 0075 0072  ..sR...|.j.d.u.r
-000008a0: 0974 0164 0183 0182 0174 027c 006a 0064  .t.d.....t.|.j.d
-000008b0: 0283 028f 107d 017c 01a0 037c 00a0 04a1  .....}.|...|....
-000008c0: 00a1 0101 0057 0064 0004 0004 0083 0301  .....W.d........
-000008d0: 0064 0053 0031 0073 2277 0101 0001 0001  .d.S.1.s"w......
-000008e0: 0059 0001 0064 0053 0029 034e 7a11 7365  .Y...d.S.).Nz.se
-000008f0: 6c66 2e70 6174 6820 6973 204e 6f6e 65da  lf.path is None.
-00000900: 0177 2905 7226 0000 00da 0a56 616c 7565  .w).r&.....Value
-00000910: 4572 726f 72da 046f 7065 6eda 0577 7269  Error..open..wri
-00000920: 7465 723b 0000 0029 0272 3600 0000 da04  ter;...).r6.....
-00000930: 6669 6c65 7223 0000 0072 2300 0000 7224  filer#...r#...r$
-00000940: 0000 00da 096f 7665 7277 7269 7465 6200  .....overwriteb.
-00000950: 0000 730a 0000 000a 0108 010e 0110 0122  ..s............"
-00000960: ff7a 1246 6965 6c64 4142 432e 6f76 6572  .z.FieldABC.over
-00000970: 7772 6974 6563 0200 0000 0000 0000 0000  writec..........
-00000980: 0000 0200 0000 0100 0000 4300 0000 7304  ..........C...s.
-00000990: 0000 0064 0153 0029 027a 1f53 6574 2069  ...d.S.).z.Set i
-000009a0: 6e74 6572 6e61 6c46 6965 6c64 2077 6974  nternalField wit
-000009b0: 6820 7661 6c75 6528 7329 4e72 2300 0000  h value(s)Nr#...
-000009c0: a902 7236 0000 0072 1900 0000 7223 0000  ..r6...r....r#..
-000009d0: 0072 2300 0000 7224 0000 0072 3500 0000  .r#...r$...r5...
-000009e0: 6800 0000 7302 0000 0004 007a 1346 6965  h...s......z.Fie
-000009f0: 6c64 4142 432e 7365 745f 7661 6c75 6573  ldABC.set_values
-00000a00: 6305 0000 0000 0000 0000 0000 0006 0000  c...............
-00000a10: 0005 0000 0043 0000 0073 3a00 0000 7c02  .....C...s:...|.
-00000a20: 7c03 7c04 7c01 6401 9c04 7d05 6402 6403  |.|.|.d...}.d.d.
-00000a30: 8400 7c05 a000 a100 4400 8301 7d05 7401  ..|.....D...}.t.
-00000a40: 7c05 6404 6405 6406 8d03 7c00 6a02 6a03  |.d.d.d...|.j.j.
-00000a50: 6404 3c00 6400 5300 2907 4e29 04da 0b63  d.<.d.S.).N)...c
-00000a60: 6f64 6549 6e63 6c75 6465 da0b 636f 6465  odeInclude..code
-00000a70: 4f70 7469 6f6e 73da 0863 6f64 654c 6962  Options..codeLib
-00000a80: 7372 1200 0000 6301 0000 0000 0000 0000  sr....c.........
-00000a90: 0000 0003 0000 0007 0000 0053 0000 0073  ...........S...s
-00000aa0: 2000 0000 6900 7c00 5d0c 5c02 7d01 7d02   ...i.|.].\.}.}.
-00000ab0: 7c01 7400 7c01 7c02 a001 a100 8302 9302  |.t.|.|.........
-00000ac0: 7102 5300 7223 0000 0029 0272 0800 0000  q.S.r#...).r....
-00000ad0: 721c 0000 0029 03da 022e 30da 036b 6579  r....)....0..key
-00000ae0: da05 7661 6c75 6572 2300 0000 7223 0000  ..valuer#...r#..
-00000af0: 0072 2400 0000 da0a 3c64 6963 7463 6f6d  .r$.....<dictcom
-00000b00: 703e 7900 0000 7302 0000 0020 007a 2b46  p>y...s.... .z+F
-00000b10: 6965 6c64 4142 432e 7365 745f 636f 6465  ieldABC.set_code
-00000b20: 7374 7265 616d 2e3c 6c6f 6361 6c73 3e2e  stream.<locals>.
-00000b30: 3c64 6963 7463 6f6d 703e 7231 0000 007a  <dictcomp>r1...z
-00000b40: 0b23 636f 6465 5374 7265 616d 2902 7237  .#codeStream).r7
-00000b50: 0000 00da 0964 6972 6563 7469 7665 2904  .....directive).
-00000b60: da05 6974 656d 7372 0900 0000 7213 0000  ..itemsr....r...
-00000b70: 0072 3200 0000 2906 7236 0000 0072 1200  .r2...).r6...r..
-00000b80: 0000 da07 696e 636c 7564 65da 076f 7074  ....include..opt
-00000b90: 696f 6e73 5a04 6c69 6273 7222 0000 0072  ionsZ.libsr"...r
-00000ba0: 2300 0000 7223 0000 0072 2400 0000 da0e  #...r#...r$.....
-00000bb0: 7365 745f 636f 6465 7374 7265 616d 6c00  set_codestreaml.
-00000bc0: 0000 7312 0000 0002 0802 0102 0102 0106  ..s.............
-00000bd0: fc12 0602 0106 0112 ff7a 1746 6965 6c64  .........z.Field
-00000be0: 4142 432e 7365 745f 636f 6465 7374 7265  ABC.set_codestre
-00000bf0: 616d 6305 0000 0000 0000 0000 0000 0007  amc.............
-00000c00: 0000 0004 0000 0043 0000 0073 4800 0000  .......C...sH...
-00000c10: 7c00 6a00 6a01 6401 1900 7d05 6402 7c02  |.j.j.d...}.d.|.
-00000c20: 6901 7d06 7c03 6400 7501 7212 7c03 7c06  i.}.|.d.u.r.|.|.
-00000c30: 6403 3c00 7c04 6400 7501 721a 7c04 7c06  d.<.|.d.u.r.|.|.
-00000c40: 6404 3c00 7402 7c06 7c01 6405 8d02 7c05  d.<.t.|.|.d...|.
-00000c50: 7c01 3c00 6400 5300 2906 4e72 1400 0000  |.<.d.S.).Nr....
-00000c60: da04 7479 7065 7249 0000 00da 0867 7261  ..typerI.....gra
-00000c70: 6469 656e 74a9 0172 3700 0000 2903 7213  dient..r7...).r.
-00000c80: 0000 0072 3200 0000 720a 0000 0029 0772  ...r2...r....).r
-00000c90: 3600 0000 7237 0000 00da 0574 7970 655f  6...r7.....type_
-00000ca0: 7249 0000 0072 5100 0000 da0a 626f 756e  rI...rQ.....boun
-00000cb0: 6461 7269 6573 7222 0000 0072 2300 0000  dariesr"...r#...
-00000cc0: 7223 0000 0072 2400 0000 da0c 7365 745f  r#...r$.....set_
-00000cd0: 626f 756e 6461 7279 7e00 0000 730e 0000  boundary~...s...
-00000ce0: 000c 0108 0108 0108 0108 0108 0114 017a  ...............z
-00000cf0: 1546 6965 6c64 4142 432e 7365 745f 626f  .FieldABC.set_bo
-00000d00: 756e 6461 7279 6302 0000 0000 0000 0000  undaryc.........
-00000d10: 0000 0002 0000 0003 0000 0043 0000 0073  ...........C...s
-00000d20: 1000 0000 7c01 7c00 6a00 6a01 6401 3c00  ....|.|.j.j.d.<.
-00000d30: 6400 5300 2902 4e72 2f00 0000 2902 7213  d.S.).Nr/...).r.
-00000d40: 0000 0072 3900 0000 2902 7236 0000 0072  ...r9...).r6...r
-00000d50: 3700 0000 7223 0000 0072 2300 0000 7224  7...r#...r#...r$
-00000d60: 0000 00da 0873 6574 5f6e 616d 6587 0000  .....set_name...
-00000d70: 0073 0200 0000 1001 7a11 4669 656c 6441  .s......z.FieldA
-00000d80: 4243 2e73 6574 5f6e 616d 6563 0100 0000  BC.set_namec....
-00000d90: 0000 0000 0000 0000 0100 0000 0400 0000  ................
-00000da0: 4300 0000 7312 0000 0074 00a0 017c 006a  C...s....t...|.j
-00000db0: 026a 0364 0119 00a1 0153 0029 024e 7231  .j.d.....S.).Nr1
-00000dc0: 0000 0029 0472 2000 0000 da05 6172 7261  ...).r .....arra
-00000dd0: 7972 1300 0000 7232 0000 0072 3c00 0000  yr....r2...r<...
-00000de0: 7223 0000 0072 2300 0000 7224 0000 00da  r#...r#...r$....
-00000df0: 0967 6574 5f61 7272 6179 8a00 0000 7302  .get_array....s.
-00000e00: 0000 0012 017a 1246 6965 6c64 4142 432e  .....z.FieldABC.
-00000e10: 6765 745f 6172 7261 79a9 024e 4e29 15da  get_array..NN)..
-00000e20: 085f 5f6e 616d 655f 5fda 0a5f 5f6d 6f64  .__name__..__mod
-00000e30: 756c 655f 5fda 0c5f 5f71 7561 6c6e 616d  ule__..__qualnam
-00000e40: 655f 5fda 0373 7472 da0f 5f5f 616e 6e6f  e__..str..__anno
-00000e50: 7461 7469 6f6e 735f 5fda 0b63 6c61 7373  tations__..class
-00000e60: 6d65 7468 6f64 7225 0000 0072 0600 0000  methodr%...r....
-00000e70: 722a 0000 0072 3a00 0000 723b 0000 0072  r*...r:...r;...r
-00000e80: 4200 0000 7203 0000 0072 3500 0000 da14  B...r....r5.....
-00000e90: 4445 4641 554c 545f 434f 4445 5f49 4e43  DEFAULT_CODE_INC
-00000ea0: 4c55 4445 da14 4445 4641 554c 545f 434f  LUDE..DEFAULT_CO
-00000eb0: 4445 5f4f 5054 494f 4e53 da11 4445 4641  DE_OPTIONS..DEFA
-00000ec0: 554c 545f 434f 4445 5f4c 4942 5372 4f00  ULT_CODE_LIBSrO.
-00000ed0: 0000 7255 0000 0072 5600 0000 7258 0000  ..rU...rV...rX..
-00000ee0: 0072 2300 0000 7223 0000 0072 2300 0000  .r#...r#...r#...
-00000ef0: 7224 0000 0072 1000 0000 2000 0000 7324  r$...r.... ...s$
-00000f00: 0000 000a 0008 0102 0210 0102 1b14 010a  ................
-00000f10: 0608 1908 0302 060a 0102 0602 0102 010a  ................
-00000f20: fb0a 1208 090c 0372 1000 0000 6300 0000  .......r....c...
-00000f30: 0000 0000 0000 0000 0000 0000 0002 0000  ................
-00000f40: 0040 0000 0073 1800 0000 6500 5a01 6400  .@...s....e.Z.d.
-00000f50: 5a02 6401 5a03 6402 6403 8400 5a04 6404  Z.d.Z.d.d...Z.d.
-00000f60: 5300 2905 da0e 566f 6c53 6361 6c61 7246  S.)...VolScalarF
-00000f70: 6965 6c64 da0e 766f 6c53 6361 6c61 7246  ield..volScalarF
-00000f80: 6965 6c64 6302 0000 0000 0000 0000 0000  ieldc...........
-00000f90: 0003 0000 0005 0000 0043 0000 0073 4200  .........C...sB.
-00000fa0: 0000 7400 7c01 7401 8302 720c 7402 7c01  ..t.|.t...r.t.|.
-00000fb0: 6401 6402 8d02 7d02 6e0d 7403 7404 7c01  d.d...}.n.t.t.|.
-00000fc0: 8301 6403 7405 7c01 8301 9b00 9d02 6402  ..d.t.|.......d.
-00000fd0: 8d02 7d02 7c02 7c00 6a06 6a07 6404 3c00  ..}.|.|.j.j.d.<.
-00000fe0: 6400 5300 2905 4eda 0775 6e69 666f 726d  d.S.).N..uniform
-00000ff0: 7252 0000 007a 2669 6e74 6572 6e61 6c46  rR...z&internalF
-00001000: 6965 6c64 206e 6f6e 756e 6966 6f72 6d0a  ield nonuniform.
-00001010: 4c69 7374 3c73 6361 6c61 723e 0a72 3100  List<scalar>.r1.
-00001020: 0000 2908 7233 0000 0072 0500 0000 720e  ..).r3...r....r.
-00001030: 0000 0072 0d00 0000 da04 6c69 7374 da03  ...r......list..
-00001040: 6c65 6e72 1300 0000 7232 0000 0029 0372  lenr....r2...).r
-00001050: 3600 0000 7219 0000 0072 4900 0000 7223  6...r....rI...r#
-00001060: 0000 0072 2300 0000 7224 0000 0072 3500  ...r#...r$...r5.
-00001070: 0000 9100 0000 730e 0000 000a 010e 0102  ......s.........
-00001080: 0206 010c 0106 fe10 047a 1956 6f6c 5363  .........z.VolSc
-00001090: 616c 6172 4669 656c 642e 7365 745f 7661  alarField.set_va
-000010a0: 6c75 6573 4ea9 0572 5a00 0000 725b 0000  luesN..rZ...r[..
-000010b0: 0072 5c00 0000 7211 0000 0072 3500 0000  .r\...r....r5...
-000010c0: 7223 0000 0072 2300 0000 7223 0000 0072  r#...r#...r#...r
-000010d0: 2400 0000 7263 0000 008e 0000 0073 0600  $...rc.......s..
-000010e0: 0000 0800 0401 0c02 7263 0000 0063 0000  ........rc...c..
-000010f0: 0000 0000 0000 0000 0000 0000 0000 0300  ................
-00001100: 0000 4000 0000 731a 0000 0065 005a 0164  ..@...s....e.Z.d
-00001110: 005a 0264 015a 0364 0564 0364 0484 015a  .Z.d.Z.d.d.d...Z
-00001120: 0464 0253 0029 06da 0e56 6f6c 5665 6374  .d.S.)...VolVect
-00001130: 6f72 4669 656c 64da 0e76 6f6c 5665 6374  orField..volVect
-00001140: 6f72 4669 656c 644e 6304 0000 0000 0000  orFieldNc.......
-00001150: 0000 0000 0007 0000 0006 0000 0043 0000  .............C..
-00001160: 0073 c200 0000 7c02 6400 7501 7234 7c03  .s....|.d.u.r4|.
-00001170: 6400 7500 720a 7400 8201 7401 7c01 7402  d.u.r.t...t.|.t.
-00001180: 6a03 8302 7312 7400 8201 7c01 6a04 6401  j...s.t...|.j.d.
-00001190: 6b03 7327 7c01 6a05 7c02 6a05 0400 0300  k.s'|.j.|.j.....
-000011a0: 6b03 7225 7c03 6a05 6b03 7229 7400 8201  k.r%|.j.k.r)t...
-000011b0: 0100 6e02 7400 8201 7c01 7d04 7402 a006  ..n.t...|.}.t...
-000011c0: 7c04 7c02 7c03 6703 a101 6a07 7d01 7408  |.|.|.g...j.}.t.
-000011d0: 7c01 8301 7d05 7c05 6402 6b02 7256 7401  |...}.|.d.k.rVt.
-000011e0: 7c01 6403 1900 7409 8302 7256 740a 6404  |.d...t...rVt.d.
-000011f0: 6405 a00b 6406 6407 8400 7c01 4400 8301  d...d.d...|.D...
-00001200: a101 1700 6408 1700 6409 640a 8d02 7d06  ....d...d.d...}.
-00001210: 6e02 7c01 7d06 7c00 6a0c a00d 640b 7c06  n.|.}.|.j...d.|.
-00001220: a102 0100 6400 5300 290c 4e72 1700 0000  ....d.S.).Nr....
-00001230: e903 0000 0072 0100 0000 7215 0000 00da  .....r....r.....
-00001240: 0120 6301 0000 0000 0000 0000 0000 0002  . c.............
-00001250: 0000 0003 0000 0073 0000 0073 1800 0000  .......s...s....
-00001260: 8100 7c00 5d07 7d01 7400 7c01 8301 5600  ..|.].}.t.|...V.
-00001270: 0100 7102 6400 5300 7227 0000 0029 0172  ..q.d.S.r'...).r
-00001280: 5d00 0000 2902 7247 0000 0072 4900 0000  ]...).rG...rI...
-00001290: 7223 0000 0072 2300 0000 7224 0000 00da  r#...r#...r$....
-000012a0: 093c 6765 6e65 7870 723e ad00 0000 7304  .<genexpr>....s.
-000012b0: 0000 0002 8016 007a 2c56 6f6c 5665 6374  .......z,VolVect
-000012c0: 6f72 4669 656c 642e 7365 745f 7661 6c75  orField.set_valu
-000012d0: 6573 2e3c 6c6f 6361 6c73 3e2e 3c67 656e  es.<locals>.<gen
-000012e0: 6578 7072 3e72 1600 0000 7265 0000 0072  expr>r....re...r
-000012f0: 5200 0000 7231 0000 0029 0e72 3e00 0000  R...r1...).r>...
-00001300: 7233 0000 0072 2000 0000 da07 6e64 6172  r3...r .....ndar
-00001310: 7261 79da 046e 6469 6dda 0473 697a 65da  ray..ndim..size.
-00001320: 0573 7461 636b da01 5472 6700 0000 7205  .stack..Trg...r.
-00001330: 0000 0072 0e00 0000 da04 6a6f 696e 7213  ...r......joinr.
-00001340: 0000 0072 3400 0000 2907 7236 0000 0072  ...r4...).r6...r
-00001350: 1900 0000 5a02 7679 5a02 767a 5a02 7678  ....Z.vyZ.vzZ.vx
-00001360: 5a06 6e5f 656c 656d 7249 0000 0072 2300  Z.n_elemrI...r#.
-00001370: 0000 7223 0000 0072 2400 0000 7235 0000  ..r#...r$...r5..
-00001380: 009f 0000 0073 2600 0000 0801 0801 0401  .....s&.........
-00001390: 0c01 0401 2201 0401 04ff 0401 0401 1201  ...."...........
-000013a0: 0802 1601 0201 1a01 0201 08fe 0405 1201  ................
-000013b0: 7a19 566f 6c56 6563 746f 7246 6965 6c64  z.VolVectorField
-000013c0: 2e73 6574 5f76 616c 7565 7372 5900 0000  .set_valuesrY...
-000013d0: 7268 0000 0072 2300 0000 7223 0000 0072  rh...r#...r#...r
-000013e0: 2300 0000 7224 0000 0072 6900 0000 9c00  #...r$...ri.....
-000013f0: 0000 7306 0000 0008 0004 010e 0272 6900  ..s..........ri.
-00001400: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
-00001410: 0000 0002 0000 0040 0000 0073 1400 0000  .......@...s....
-00001420: 6500 5a01 6400 5a02 6401 6402 8400 5a03  e.Z.d.Z.d.d...Z.
-00001430: 6403 5300 2904 da0e 566f 6c54 656e 736f  d.S.)...VolTenso
-00001440: 7246 6965 6c64 6302 0000 0000 0000 0000  rFieldc.........
-00001450: 0000 0002 0000 0004 0000 0043 0000 0073  ...........C...s
-00001460: 3000 0000 7400 7c01 7401 6a02 8302 720b  0...t.|.t.j...r.
-00001470: 7c01 6a03 6401 6b03 720f 7404 6402 8301  |.j.d.k.r.t.d...
-00001480: 8201 7c00 6a05 a006 6403 7c01 a102 0100  ..|.j...d.|.....
-00001490: 6400 5300 2904 4ee9 0200 0000 7a36 6e6f  d.S.).N.....z6no
-000014a0: 7420 6973 696e 7374 616e 6365 2876 616c  t isinstance(val
-000014b0: 7565 732c 206e 702e 6e64 6172 7261 7929  ues, np.ndarray)
-000014c0: 206f 7220 7661 6c75 6573 2e6e 6469 6d20   or values.ndim 
-000014d0: 213d 2032 7231 0000 0029 0772 3300 0000  != 2r1...).r3...
-000014e0: 7220 0000 0072 6e00 0000 726f 0000 00da  r ...rn...ro....
-000014f0: 134e 6f74 496d 706c 656d 656e 7465 6445  .NotImplementedE
-00001500: 7272 6f72 7213 0000 0072 3400 0000 7243  rrorr....r4...rC
-00001510: 0000 0072 2300 0000 7223 0000 0072 2400  ...r#...r#...r$.
-00001520: 0000 7235 0000 00b6 0000 0073 0a00 0000  ..r5.......s....
-00001530: 1601 0201 0201 04ff 1204 7a19 566f 6c54  ..........z.VolT
-00001540: 656e 736f 7246 6965 6c64 2e73 6574 5f76  ensorField.set_v
-00001550: 616c 7565 734e 2904 725a 0000 0072 5b00  aluesN).rZ...r[.
-00001560: 0000 725c 0000 0072 3500 0000 7223 0000  ..r\...r5...r#..
-00001570: 0072 2300 0000 7223 0000 0072 2400 0000  .r#...r#...r$...
-00001580: 7274 0000 00b5 0000 0073 0400 0000 0800  rt.......s......
-00001590: 0c01 7274 0000 0029 0372 6400 0000 726a  ..rt...).rd...rj
-000015a0: 0000 005a 0e76 6f6c 5465 6e73 6f72 4669  ...Z.volTensorFi
-000015b0: 656c 6463 0100 0000 0000 0000 0000 0000  eldc............
-000015c0: 0400 0000 0800 0000 4300 0000 7380 0000  ........C...s...
-000015d0: 0064 007d 0174 007c 0064 0183 028f 227d  .d.}.t.|.d...."}
-000015e0: 027c 0244 005d 177d 037c 03a0 01a1 007d  .|.D.].}.|.....}
-000015f0: 037c 03a0 0264 02a1 0172 217c 03a0 03a1  .|...d...r!|....
-00001600: 0064 0319 0064 0064 0385 0219 007d 0101  .d...d.d.....}..
-00001610: 006e 0171 0a57 0064 0004 0004 0083 0301  .n.q.W.d........
-00001620: 006e 0831 0073 2c77 0101 0001 0001 0059  .n.1.s,w.......Y
-00001630: 0001 007c 0164 0075 0072 3774 0482 0174  ...|.d.u.r7t...t
-00001640: 057c 0119 007d 017c 01a0 067c 00a1 0153  .|...}.|...|...S
-00001650: 0029 044e da01 727a 0663 6c61 7373 20e9  .).N..rz.class .
-00001660: ffff ffff 2907 723f 0000 0072 1c00 0000  ....).r?...r....
-00001670: 721d 0000 00da 0573 706c 6974 da0c 5275  r......split..Ru
-00001680: 6e74 696d 6545 7272 6f72 da07 636c 6173  ntimeError..clas
-00001690: 7365 7372 2a00 0000 2904 7226 0000 0072  sesr*...).r&...r
-000016a0: 1100 0000 7241 0000 00da 046c 696e 6572  ....rA.....liner
-000016b0: 2300 0000 7223 0000 0072 2400 0000 da0f  #...r#...r$.....
-000016c0: 7265 6164 5f66 6965 6c64 5f66 696c 65c6  read_field_file.
-000016d0: 0000 0073 1c00 0000 0401 0c01 0801 0801  ...s............
-000016e0: 0a01 1401 0401 02fe 0280 1cfd 0807 0401  ................
-000016f0: 0802 0a02 727d 0000 0029 21da 075f 5f64  ....r}...)!..__d
-00001700: 6f63 5f5f 721e 0000 00da 0361 6263 7202  oc__r......abcr.
-00001710: 0000 0072 0300 0000 da02 696f 7204 0000  ...r......ior...
-00001720: 00da 076e 756d 6265 7273 7205 0000 00da  ...numbersr.....
-00001730: 0770 6174 686c 6962 7206 0000 00da 056e  .pathlibr......n
-00001740: 756d 7079 7220 0000 005a 1d66 6c75 6964  umpyr ...Z.fluid
-00001750: 7369 6d66 6f61 6d2e 666f 616d 5f69 6e70  simfoam.foam_inp
-00001760: 7574 5f66 696c 6573 7207 0000 00da 2166  ut_filesr.....!f
-00001770: 6c75 6964 7369 6d66 6f61 6d2e 666f 616d  luidsimfoam.foam
-00001780: 5f69 6e70 7574 5f66 696c 6573 2e61 7374  _input_files.ast
-00001790: 7208 0000 0072 0900 0000 720a 0000 0072  r....r....r....r
-000017a0: 0b00 0000 720c 0000 0072 0d00 0000 720e  ....r....r....r.
-000017b0: 0000 0072 0f00 0000 7260 0000 0072 6100  ...r....r`...ra.
-000017c0: 0000 7262 0000 0072 1000 0000 7263 0000  ..rb...r....rc..
-000017d0: 0072 6900 0000 7274 0000 0072 7b00 0000  .ri...rt...r{...
-000017e0: 727d 0000 0072 2300 0000 7223 0000 0072  r}...r#...r#...r
-000017f0: 2300 0000 7224 0000 00da 083c 6d6f 6475  #...r$.....<modu
-00001800: 6c65 3e01 0000 0073 2c00 0000 0400 0804  le>....s,.......
-00001810: 1001 0c01 0c01 0c01 0802 0c02 2801 040b  ............(...
-00001820: 0202 02ff 0403 1003 106e 100e 1019 020b  .........n......
-00001830: 0201 0201 06fd 0c07                      ........
+000000a0: 6d16 5a16 0100 6409 5a17 640a 5a18 640b  m.Z...d.Z.d.Z.d.
+000000b0: 5a19 4700 640c 640d 8400 640d 6503 8303  Z.G.d.d...d.e...
+000000c0: 5a1a 4700 640e 640f 8400 640f 651a 8303  Z.G.d.d...d.e...
+000000d0: 5a1b 4700 6410 6411 8400 6411 651a 8303  Z.G.d.d...d.e...
+000000e0: 5a1c 4700 6412 6413 8400 6413 651a 8303  Z.G.d.d...d.e...
+000000f0: 5a1d 6414 6415 8400 651b 651c 651d 6603  Z.d.d...e.e.e.f.
+00000100: 4400 8301 5a1e 6416 6417 8400 5a1f 641d  D...Z.d.d...Z.d.
+00000110: 6419 641a 8401 5a20 641b 641c 8400 5a21  d.d...Z d.d...Z!
+00000120: 6402 5300 291e 7a1e 4865 6c70 6572 2074  d.S.).z.Helper t
+00000130: 6f20 6372 6561 7465 2066 6965 6c64 2066  o create field f
+00000140: 696c 6573 0a0a e900 0000 004e 2902 da03  iles.......N)...
+00000150: 4142 43da 0e61 6273 7472 6163 746d 6574  ABC..abstractmet
+00000160: 686f 6429 01da 0853 7472 696e 6749 4f29  hod)...StringIO)
+00000170: 01da 064e 756d 6265 7229 01da 0450 6174  ...Number)...Pat
+00000180: 6829 01da 0570 6172 7365 2907 da04 436f  h)...parse)...Co
+00000190: 6465 da0a 436f 6465 5374 7265 616d da04  de..CodeStream..
+000001a0: 4469 6374 da0c 4469 6d65 6e73 696f 6e53  Dict..DimensionS
+000001b0: 6574 da0d 466f 616d 496e 7075 7446 696c  et..FoamInputFil
+000001c0: 65da 044c 6973 74da 0556 616c 7565 7a12  e..List..Valuez.
+000001d0: 2369 6e63 6c75 6465 2022 6676 4346 442e  #include "fvCFD.
+000001e0: 4822 7a46 2d49 2428 4c49 425f 5352 4329  H"zF-I$(LIB_SRC)
+000001f0: 2f66 696e 6974 6556 6f6c 756d 652f 6c6e  /finiteVolume/ln
+00000200: 496e 636c 7564 6520 5c0a 2d49 2428 4c49  Include \.-I$(LI
+00000210: 425f 5352 4329 2f6d 6573 6854 6f6f 6c73  B_SRC)/meshTools
+00000220: 2f6c 6e49 6e63 6c75 6465 7a1c 2d6c 6d65  /lnIncludez.-lme
+00000230: 7368 546f 6f6c 7320 5c0a 2d6c 6669 6e69  shTools \.-lfini
+00000240: 7465 566f 6c75 6d65 6300 0000 0000 0000  teVolumec.......
+00000250: 0000 0000 0000 0000 0005 0000 0040 0000  .............@..
+00000260: 0073 9200 0000 6500 5a01 6400 5a02 5500  .s....e.Z.d.Z.U.
+00000270: 6503 6504 6401 3c00 6505 641a 6403 6503  e.e.d.<.e.d.d.e.
+00000280: 6602 6404 6405 8405 8301 5a06 6505 641a  f.d.d.....Z.e.d.
+00000290: 6406 6503 7019 6507 6602 6407 6408 8405  d.e.p.e.f.d.d...
+000002a0: 8301 5a08 641b 640a 640b 8401 5a09 640c  ..Z.d.d.d...Z.d.
+000002b0: 640d 8400 5a0a 640e 640f 8400 5a0b 650c  d...Z.d.d...Z.e.
+000002c0: 6410 6411 8400 8301 5a0d 650e 650f 6510  d.d.....Z.e.e.e.
+000002d0: 6603 6412 6413 8401 5a11 641b 6414 6415  f.d.d...Z.d.d.d.
+000002e0: 8401 5a12 6416 6417 8400 5a13 6418 6419  ..Z.d.d...Z.d.d.
+000002f0: 8400 5a14 6409 5300 291c da08 4669 656c  ..Z.d.S.)...Fiel
+00000300: 6441 4243 da03 636c 7346 da04 636f 6465  dABC..clsF..code
+00000310: 6303 0000 0000 0000 0000 0000 000b 0000  c...............
+00000320: 0006 0000 0043 0000 0073 d000 0000 6401  .....C...s....d.
+00000330: 7c01 7601 720f 7400 7c01 8301 7d03 7c00  |.v.r.t.|...}.|.
+00000340: 6400 6400 7c03 6402 8d03 5300 7c01 a001  d.d.|.d...S.|...
+00000350: 6401 a101 7d04 7c01 a002 6403 7c04 a102  d...}.|...d.|...
+00000360: 7d05 7c01 a001 6404 7c04 7c05 a103 7d06  }.|...d.|.|...}.
+00000370: 7c01 a002 6405 7c04 7c05 a103 7d07 7c01  |...d.|.|...}.|.
+00000380: 6400 7c04 8502 1900 6406 1700 7d08 7c02  d.|.....d...}.|.
+00000390: 733c 7c08 6407 7c01 7c05 6400 8502 1900  s<|.d.|.|.d.....
+000003a0: 1700 3700 7d08 7400 7c08 8301 7d03 7c01  ..7.}.t.|...}.|.
+000003b0: 7c06 6408 1700 7c07 8502 1900 a003 a100  |.d...|.........
+000003c0: 7d09 7c09 a004 6404 a101 7256 7405 a006  }.|...d...rVt...
+000003d0: 6409 640a 7c09 a103 7d09 7407 a008 7409  d.d.|...}.t...t.
+000003e0: 7c09 8301 a101 7d0a 7c0a 7c03 5f0a 7c00  |.....}.|.|._.|.
+000003f0: 640a 640a 7c03 7c0a 640b 8d04 5300 290c  d.d.|.|.d...S.).
+00000400: 4e5a 0a6e 6f6e 756e 6966 6f72 6d29 01da  NZ.nonuniform)..
+00000410: 0474 7265 65da 0d62 6f75 6e64 6172 7946  .tree..boundaryF
+00000420: 6965 6c64 fa01 28fa 0129 7a02 3b0a da01  ield..(..)z.;...
+00000430: 0ae9 0100 0000 7a04 5b28 295d da00 2902  ......z.[()]..).
+00000440: 7212 0000 00da 0676 616c 7565 7329 0b72  r......values).r
+00000450: 0700 0000 da05 696e 6465 78da 0672 696e  ......index..rin
+00000460: 6465 78da 0573 7472 6970 da0a 7374 6172  dex..strip..star
+00000470: 7473 7769 7468 da02 7265 da03 7375 62da  tswith..re..sub.
+00000480: 026e 70da 076c 6f61 6474 7874 7204 0000  .np..loadtxtr...
+00000490: 00da 0464 6174 6129 0b72 1000 0000 7211  ...data).r....r.
+000004a0: 0000 00da 1373 6b69 705f 626f 756e 6461  .....skip_bounda
+000004b0: 7279 5f66 6965 6c64 7212 0000 005a 1069  ry_fieldr....Z.i
+000004c0: 6e64 6578 5f6e 6f6e 756e 6966 6f72 6d5a  ndex_nonuniformZ
+000004d0: 1369 6e64 6578 5f62 6f75 6e64 6172 7946  .index_boundaryF
+000004e0: 6965 6c64 5a11 696e 6465 785f 6f70 656e  ieldZ.index_open
+000004f0: 696e 675f 7061 725a 1169 6e64 6578 5f63  ing_parZ.index_c
+00000500: 6c6f 7369 6e67 5f70 6172 5a0d 636f 6465  losing_parZ.code
+00000510: 5f74 6f5f 7061 7273 655a 0963 6f64 655f  _to_parseZ.code_
+00000520: 6461 7461 7222 0000 00a9 0072 2400 0000  datar".....r$...
+00000530: fa49 2f68 6f6d 652f 7069 6572 7265 2f44  .I/home/pierre/D
+00000540: 6576 2f66 6c75 6964 7369 6d66 6f61 6d2f  ev/fluidsimfoam/
+00000550: 7372 632f 666c 7569 6473 696d 666f 616d  src/fluidsimfoam
+00000560: 2f66 6f61 6d5f 696e 7075 745f 6669 6c65  /foam_input_file
+00000570: 732f 6669 656c 6473 2e70 79da 0966 726f  s/fields.py..fro
+00000580: 6d5f 636f 6465 2200 0000 7326 0000 0008  m_code"...s&....
+00000590: 0208 010e 010a 020c 010e 0104 0106 0104  ................
+000005a0: ff10 0404 0114 0108 0214 010a 020e 010e  ................
+000005b0: 0206 0210 017a 1246 6965 6c64 4142 432e  .....z.FieldABC.
+000005c0: 6672 6f6d 5f63 6f64 65da 0470 6174 6863  from_code..pathc
+000005d0: 0300 0000 0000 0000 0000 0000 0400 0000  ................
+000005e0: 0400 0000 4300 0000 7324 0000 0074 007c  ....C...s$...t.|
+000005f0: 0183 017d 017c 006a 017c 01a0 02a1 007c  ...}.|.j.|.....|
+00000600: 0264 018d 027d 037c 017c 035f 037c 0353  .d...}.|.|._.|.S
+00000610: 0029 024e 2901 7223 0000 0029 0472 0600  .).N).r#...).r..
+00000620: 0000 7226 0000 00da 0972 6561 645f 7465  ..r&.....read_te
+00000630: 7874 7227 0000 0029 0472 1000 0000 7227  xtr'...).r....r'
+00000640: 0000 0072 2300 0000 da05 6669 656c 6472  ...r#.....fieldr
+00000650: 2400 0000 7224 0000 0072 2500 0000 da09  $...r$...r%.....
+00000660: 6672 6f6d 5f70 6174 683e 0000 0073 0c00  from_path>...s..
+00000670: 0000 0802 0401 0801 06ff 0603 0401 7a12  ..............z.
+00000680: 4669 656c 6441 4243 2e66 726f 6d5f 7061  FieldABC.from_pa
+00000690: 7468 4e63 0500 0000 0000 0000 0000 0000  thNc............
+000006a0: 0600 0000 0500 0000 4300 0000 7370 0000  ........C...sp..
+000006b0: 007c 0364 0075 0172 087c 037c 005f 006e  .|.d.u.r.|.|._.n
+000006c0: 2264 0164 027c 006a 017c 0164 039c 047d  "d.d.|.j.|.d...}
+000006d0: 0574 027c 0274 0383 0273 1974 037c 0283  .t.|.t...s.t.|..
+000006e0: 017d 0274 047c 057c 0264 0064 049c 0264  .}.t.|.|.d.d...d
+000006f0: 058d 027c 005f 007c 006a 00a0 0564 0669  ...|._.|.j...d.i
+00000700: 00a1 0201 007c 0464 0075 0172 337c 00a0  .....|.d.u.r3|..
+00000710: 067c 04a1 0101 0064 007c 005f 0764 0053  .|.....d.|._.d.S
+00000720: 0029 074e 7a03 322e 30da 0561 7363 6969  .).Nz.2.0..ascii
+00000730: 2904 da07 7665 7273 696f 6eda 0666 6f72  )...version..for
+00000740: 6d61 74da 0563 6c61 7373 da06 6f62 6a65  mat..class..obje
+00000750: 6374 2902 da0a 6469 6d65 6e73 696f 6e73  ct)...dimensions
+00000760: da0d 696e 7465 726e 616c 4669 656c 6429  ..internalField)
+00000770: 01da 0863 6869 6c64 7265 6e72 1300 0000  ...childrenr....
+00000780: 2908 7212 0000 0072 1000 0000 da0a 6973  ).r....r......is
+00000790: 696e 7374 616e 6365 720b 0000 0072 0c00  instancer....r..
+000007a0: 0000 da09 7365 745f 6368 696c 64da 0a73  ....set_child..s
+000007b0: 6574 5f76 616c 7565 7372 2700 0000 2906  et_valuesr'...).
+000007c0: da04 7365 6c66 da04 6e61 6d65 da09 6469  ..self..name..di
+000007d0: 6d65 6e73 696f 6e72 1200 0000 7219 0000  mensionr....r...
+000007e0: 00da 0469 6e66 6f72 2400 0000 7224 0000  ...infor$...r$..
+000007f0: 0072 2500 0000 da08 5f5f 696e 6974 5f5f  .r%.....__init__
+00000800: 4700 0000 7320 0000 0008 0108 0102 0302  G...s ..........
+00000810: 0104 0102 0106 fc0a 0708 0102 020a 0108  ................
+00000820: ff0e 0408 020a 010a 027a 1146 6965 6c64  .........z.Field
+00000830: 4142 432e 5f5f 696e 6974 5f5f 6301 0000  ABC.__init__c...
+00000840: 0000 0000 0000 0000 0001 0000 0002 0000  ................
+00000850: 0043 0000 0073 0a00 0000 7c00 6a00 a001  .C...s....|.j...
+00000860: a100 5300 a901 4e29 0272 1200 0000 da04  ..S...N).r......
+00000870: 6475 6d70 a901 7236 0000 0072 2400 0000  dump..r6...r$...
+00000880: 7224 0000 0072 2500 0000 723c 0000 0060  r$...r%...r<...`
+00000890: 0000 0073 0200 0000 0a01 7a0d 4669 656c  ...s......z.Fiel
+000008a0: 6441 4243 2e64 756d 7063 0100 0000 0000  dABC.dumpc......
+000008b0: 0000 0000 0000 0200 0000 0800 0000 4300  ..............C.
+000008c0: 0000 7352 0000 007c 006a 0064 0075 0072  ..sR...|.j.d.u.r
+000008d0: 0974 0164 0183 0182 0174 027c 006a 0064  .t.d.....t.|.j.d
+000008e0: 0283 028f 107d 017c 01a0 037c 00a0 04a1  .....}.|...|....
+000008f0: 00a1 0101 0057 0064 0004 0004 0083 0301  .....W.d........
+00000900: 0064 0053 0031 0073 2277 0101 0001 0001  .d.S.1.s"w......
+00000910: 0059 0001 0064 0053 0029 034e 7a11 7365  .Y...d.S.).Nz.se
+00000920: 6c66 2e70 6174 6820 6973 204e 6f6e 65da  lf.path is None.
+00000930: 0177 2905 7227 0000 00da 0a56 616c 7565  .w).r'.....Value
+00000940: 4572 726f 72da 046f 7065 6eda 0577 7269  Error..open..wri
+00000950: 7465 723c 0000 0029 0272 3600 0000 da04  ter<...).r6.....
+00000960: 6669 6c65 7224 0000 0072 2400 0000 7225  filer$...r$...r%
+00000970: 0000 00da 096f 7665 7277 7269 7465 6300  .....overwritec.
+00000980: 0000 730a 0000 000a 0108 010e 0110 0122  ..s............"
+00000990: ff7a 1246 6965 6c64 4142 432e 6f76 6572  .z.FieldABC.over
+000009a0: 7772 6974 6563 0200 0000 0000 0000 0000  writec..........
+000009b0: 0000 0200 0000 0100 0000 4300 0000 7304  ..........C...s.
+000009c0: 0000 0064 0153 0029 027a 1f53 6574 2069  ...d.S.).z.Set i
+000009d0: 6e74 6572 6e61 6c46 6965 6c64 2077 6974  nternalField wit
+000009e0: 6820 7661 6c75 6528 7329 4e72 2400 0000  h value(s)Nr$...
+000009f0: a902 7236 0000 0072 1900 0000 7224 0000  ..r6...r....r$..
+00000a00: 0072 2400 0000 7225 0000 0072 3500 0000  .r$...r%...r5...
+00000a10: 6900 0000 7302 0000 0004 007a 1346 6965  i...s......z.Fie
+00000a20: 6c64 4142 432e 7365 745f 7661 6c75 6573  ldABC.set_values
+00000a30: 6305 0000 0000 0000 0000 0000 0006 0000  c...............
+00000a40: 0005 0000 0043 0000 0073 3a00 0000 7c02  .....C...s:...|.
+00000a50: 7c03 7c04 7c01 6401 9c04 7d05 6402 6403  |.|.|.d...}.d.d.
+00000a60: 8400 7c05 a000 a100 4400 8301 7d05 7401  ..|.....D...}.t.
+00000a70: 7c05 6404 6405 6406 8d03 7c00 6a02 6a03  |.d.d.d...|.j.j.
+00000a80: 6404 3c00 6400 5300 2907 4e29 04da 0b63  d.<.d.S.).N)...c
+00000a90: 6f64 6549 6e63 6c75 6465 da0b 636f 6465  odeInclude..code
+00000aa0: 4f70 7469 6f6e 73da 0863 6f64 654c 6962  Options..codeLib
+00000ab0: 7372 1100 0000 6301 0000 0000 0000 0000  sr....c.........
+00000ac0: 0000 0003 0000 0007 0000 0053 0000 0073  ...........S...s
+00000ad0: 2000 0000 6900 7c00 5d0c 5c02 7d01 7d02   ...i.|.].\.}.}.
+00000ae0: 7c01 7400 7c01 7c02 a001 a100 8302 9302  |.t.|.|.........
+00000af0: 7102 5300 7224 0000 0029 0272 0800 0000  q.S.r$...).r....
+00000b00: 721c 0000 0029 03da 022e 30da 036b 6579  r....)....0..key
+00000b10: da05 7661 6c75 6572 2400 0000 7224 0000  ..valuer$...r$..
+00000b20: 0072 2500 0000 da0a 3c64 6963 7463 6f6d  .r%.....<dictcom
+00000b30: 703e 7a00 0000 7302 0000 0020 007a 2b46  p>z...s.... .z+F
+00000b40: 6965 6c64 4142 432e 7365 745f 636f 6465  ieldABC.set_code
+00000b50: 7374 7265 616d 2e3c 6c6f 6361 6c73 3e2e  stream.<locals>.
+00000b60: 3c64 6963 7463 6f6d 703e 7231 0000 007a  <dictcomp>r1...z
+00000b70: 0b23 636f 6465 5374 7265 616d 2902 7237  .#codeStream).r7
+00000b80: 0000 00da 0964 6972 6563 7469 7665 2904  .....directive).
+00000b90: da05 6974 656d 7372 0900 0000 7212 0000  ..itemsr....r...
+00000ba0: 0072 3200 0000 2906 7236 0000 0072 1100  .r2...).r6...r..
+00000bb0: 0000 da07 696e 636c 7564 65da 076f 7074  ....include..opt
+00000bc0: 696f 6e73 da04 6c69 6273 7222 0000 0072  ions..libsr"...r
+00000bd0: 2400 0000 7224 0000 0072 2500 0000 da0e  $...r$...r%.....
+00000be0: 7365 745f 636f 6465 7374 7265 616d 6d00  set_codestreamm.
+00000bf0: 0000 7312 0000 0002 0802 0102 0102 0106  ..s.............
+00000c00: fc12 0602 0106 0112 ff7a 1746 6965 6c64  .........z.Field
+00000c10: 4142 432e 7365 745f 636f 6465 7374 7265  ABC.set_codestre
+00000c20: 616d 6305 0000 0000 0000 0000 0000 0007  amc.............
+00000c30: 0000 0004 0000 0043 0000 0073 4800 0000  .......C...sH...
+00000c40: 7c00 6a00 6a01 6401 1900 7d05 6402 7c02  |.j.j.d...}.d.|.
+00000c50: 6901 7d06 7c03 6400 7501 7212 7c03 7c06  i.}.|.d.u.r.|.|.
+00000c60: 6403 3c00 7c04 6400 7501 721a 7c04 7c06  d.<.|.d.u.r.|.|.
+00000c70: 6404 3c00 7402 7c06 7c01 6405 8d02 7c05  d.<.t.|.|.d...|.
+00000c80: 7c01 3c00 6400 5300 2906 4e72 1300 0000  |.<.d.S.).Nr....
+00000c90: da04 7479 7065 724a 0000 00da 0867 7261  ..typerJ.....gra
+00000ca0: 6469 656e 74a9 0172 3700 0000 2903 7212  dient..r7...).r.
+00000cb0: 0000 0072 3200 0000 720a 0000 0029 0772  ...r2...r....).r
+00000cc0: 3600 0000 7237 0000 00da 0574 7970 655f  6...r7.....type_
+00000cd0: 724a 0000 0072 5300 0000 da0a 626f 756e  rJ...rS.....boun
+00000ce0: 6461 7269 6573 7222 0000 0072 2400 0000  dariesr"...r$...
+00000cf0: 7224 0000 0072 2500 0000 da0c 7365 745f  r$...r%.....set_
+00000d00: 626f 756e 6461 7279 7f00 0000 730e 0000  boundary....s...
+00000d10: 000c 0108 0108 0108 0108 0108 0114 017a  ...............z
+00000d20: 1546 6965 6c64 4142 432e 7365 745f 626f  .FieldABC.set_bo
+00000d30: 756e 6461 7279 6302 0000 0000 0000 0000  undaryc.........
+00000d40: 0000 0002 0000 0003 0000 0043 0000 0073  ...........C...s
+00000d50: 1000 0000 7c01 7c00 6a00 6a01 6401 3c00  ....|.|.j.j.d.<.
+00000d60: 6400 5300 2902 4e72 2f00 0000 2902 7212  d.S.).Nr/...).r.
+00000d70: 0000 0072 3900 0000 2902 7236 0000 0072  ...r9...).r6...r
+00000d80: 3700 0000 7224 0000 0072 2400 0000 7225  7...r$...r$...r%
+00000d90: 0000 00da 0873 6574 5f6e 616d 6588 0000  .....set_name...
+00000da0: 0073 0200 0000 1001 7a11 4669 656c 6441  .s......z.FieldA
+00000db0: 4243 2e73 6574 5f6e 616d 6563 0100 0000  BC.set_namec....
+00000dc0: 0000 0000 0000 0000 0100 0000 0400 0000  ................
+00000dd0: 4300 0000 7312 0000 0074 00a0 017c 006a  C...s....t...|.j
+00000de0: 026a 0364 0119 00a1 0153 0029 024e 7231  .j.d.....S.).Nr1
+00000df0: 0000 0029 0472 2000 0000 da05 6172 7261  ...).r .....arra
+00000e00: 7972 1200 0000 7232 0000 0072 3d00 0000  yr....r2...r=...
+00000e10: 7224 0000 0072 2400 0000 7225 0000 00da  r$...r$...r%....
+00000e20: 0967 6574 5f61 7272 6179 8b00 0000 7302  .get_array....s.
+00000e30: 0000 0012 017a 1246 6965 6c64 4142 432e  .....z.FieldABC.
+00000e40: 6765 745f 6172 7261 7929 0146 a902 4e4e  get_array).F..NN
+00000e50: 2915 da08 5f5f 6e61 6d65 5f5f da0a 5f5f  )...__name__..__
+00000e60: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
+00000e70: 6e61 6d65 5f5f da03 7374 72da 0f5f 5f61  name__..str..__a
+00000e80: 6e6e 6f74 6174 696f 6e73 5f5f da0b 636c  nnotations__..cl
+00000e90: 6173 736d 6574 686f 6472 2600 0000 7206  assmethodr&...r.
+00000ea0: 0000 0072 2a00 0000 723a 0000 0072 3c00  ...r*...r:...r<.
+00000eb0: 0000 7243 0000 0072 0300 0000 7235 0000  ..rC...r....r5..
+00000ec0: 00da 1444 4546 4155 4c54 5f43 4f44 455f  ...DEFAULT_CODE_
+00000ed0: 494e 434c 5544 45da 1444 4546 4155 4c54  INCLUDE..DEFAULT
+00000ee0: 5f43 4f44 455f 4f50 5449 4f4e 53da 1144  _CODE_OPTIONS..D
+00000ef0: 4546 4155 4c54 5f43 4f44 455f 4c49 4253  EFAULT_CODE_LIBS
+00000f00: 7251 0000 0072 5700 0000 7258 0000 0072  rQ...rW...rX...r
+00000f10: 5a00 0000 7224 0000 0072 2400 0000 7224  Z...r$...r$...r$
+00000f20: 0000 0072 2500 0000 720f 0000 001f 0000  ...r%...r.......
+00000f30: 0073 2400 0000 0a00 0801 0202 1201 021b  .s$.............
+00000f40: 1601 0a08 0819 0803 0206 0a01 0206 0201  ................
+00000f50: 0201 0afb 0a12 0809 0c03 720f 0000 0063  ..........r....c
+00000f60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000f70: 0200 0000 4000 0000 f318 0000 0065 005a  ....@........e.Z
+00000f80: 0164 005a 0264 015a 0364 0264 0384 005a  .d.Z.d.Z.d.d...Z
+00000f90: 0464 0453 0029 05da 0e56 6f6c 5363 616c  .d.S.)...VolScal
+00000fa0: 6172 4669 656c 645a 0e76 6f6c 5363 616c  arFieldZ.volScal
+00000fb0: 6172 4669 656c 6463 0200 0000 0000 0000  arFieldc........
+00000fc0: 0000 0000 0300 0000 0500 0000 4300 0000  ............C...
+00000fd0: 7342 0000 0074 007c 0174 0183 0272 0c74  sB...t.|.t...r.t
+00000fe0: 027c 0164 0164 028d 027d 026e 0d74 0374  .|.d.d...}.n.t.t
+00000ff0: 047c 0183 0164 0374 057c 0183 019b 009d  .|...d.t.|......
+00001000: 0264 028d 027d 027c 027c 006a 066a 0764  .d...}.|.|.j.j.d
+00001010: 043c 0064 0053 0029 054e da07 756e 6966  .<.d.S.).N..unif
+00001020: 6f72 6d72 5400 0000 7a26 696e 7465 726e  ormrT...z&intern
+00001030: 616c 4669 656c 6420 6e6f 6e75 6e69 666f  alField nonunifo
+00001040: 726d 0a4c 6973 743c 7363 616c 6172 3e0a  rm.List<scalar>.
+00001050: 7231 0000 0029 0872 3300 0000 7205 0000  r1...).r3...r...
+00001060: 0072 0e00 0000 720d 0000 00da 046c 6973  .r....r......lis
+00001070: 74da 036c 656e 7212 0000 0072 3200 0000  t..lenr....r2...
+00001080: 2903 7236 0000 0072 1900 0000 724a 0000  ).r6...r....rJ..
+00001090: 0072 2400 0000 7224 0000 0072 2500 0000  .r$...r$...r%...
+000010a0: 7235 0000 0092 0000 0073 0e00 0000 0a01  r5.......s......
+000010b0: 0e01 0202 0601 0c01 06fe 1004 7a19 566f  ............z.Vo
+000010c0: 6c53 6361 6c61 7246 6965 6c64 2e73 6574  lScalarField.set
+000010d0: 5f76 616c 7565 734e a905 725c 0000 0072  _valuesN..r\...r
+000010e0: 5d00 0000 725e 0000 0072 1000 0000 7235  ]...r^...r....r5
+000010f0: 0000 0072 2400 0000 7224 0000 0072 2400  ...r$...r$...r$.
+00001100: 0000 7225 0000 0072 6600 0000 8f00 0000  ..r%...rf.......
+00001110: f306 0000 0008 0004 010c 0272 6600 0000  ...........rf...
+00001120: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+00001130: 0003 0000 0040 0000 0073 2200 0000 6500  .....@...s"...e.
+00001140: 5a01 6400 5a02 6401 5a03 6407 6403 6404  Z.d.Z.d.Z.d.d.d.
+00001150: 8401 5a04 6405 6406 8400 5a05 6402 5300  ..Z.d.d...Z.d.S.
+00001160: 2908 da0e 566f 6c56 6563 746f 7246 6965  )...VolVectorFie
+00001170: 6c64 5a0e 766f 6c56 6563 746f 7246 6965  ldZ.volVectorFie
+00001180: 6c64 4e63 0400 0000 0000 0000 0000 0000  ldNc............
+00001190: 0700 0000 0600 0000 4300 0000 73c2 0000  ........C...s...
+000011a0: 007c 0264 0075 0172 347c 0364 0075 0072  .|.d.u.r4|.d.u.r
+000011b0: 0a74 0082 0174 017c 0174 026a 0383 0273  .t...t.|.t.j...s
+000011c0: 1274 0082 017c 016a 0464 016b 0373 277c  .t...|.j.d.k.s'|
+000011d0: 016a 057c 026a 0504 0003 006b 0372 257c  .j.|.j.....k.r%|
+000011e0: 036a 056b 0372 2974 0082 0101 006e 0274  .j.k.r)t.....n.t
+000011f0: 0082 017c 017d 0474 02a0 067c 047c 027c  ...|.}.t...|.|.|
+00001200: 0367 03a1 016a 077d 0174 087c 0183 017d  .g...j.}.t.|...}
+00001210: 057c 0564 026b 0272 5674 017c 0164 0319  .|.d.k.rVt.|.d..
+00001220: 0074 0983 0272 5674 0a64 0464 05a0 0b64  .t...rVt.d.d...d
+00001230: 0664 0784 007c 0144 0083 01a1 0117 0064  .d...|.D.......d
+00001240: 0817 0064 0964 0a8d 027d 066e 027c 017d  ...d.d...}.n.|.}
+00001250: 067c 006a 0ca0 0d64 0b7c 06a1 0201 0064  .|.j...d.|.....d
+00001260: 0053 0029 0c4e 7217 0000 00e9 0300 0000  .S.).Nr.........
+00001270: 7201 0000 0072 1400 0000 da01 2063 0100  r....r...... c..
+00001280: 0000 0000 0000 0000 0000 0200 0000 0300  ................
+00001290: 0000 7300 0000 7318 0000 0081 007c 005d  ..s...s......|.]
+000012a0: 077d 0174 007c 0183 0156 0001 0071 0264  .}.t.|...V...q.d
+000012b0: 0053 0072 3b00 0000 2901 725f 0000 0029  .S.r;...).r_...)
+000012c0: 0272 4800 0000 724a 0000 0072 2400 0000  .rH...rJ...r$...
+000012d0: 7224 0000 0072 2500 0000 da09 3c67 656e  r$...r%.....<gen
+000012e0: 6578 7072 3eae 0000 0073 0400 0000 0280  expr>....s......
+000012f0: 1600 7a2c 566f 6c56 6563 746f 7246 6965  ..z,VolVectorFie
+00001300: 6c64 2e73 6574 5f76 616c 7565 732e 3c6c  ld.set_values.<l
+00001310: 6f63 616c 733e 2e3c 6765 6e65 7870 723e  ocals>.<genexpr>
+00001320: 7215 0000 0072 6700 0000 7254 0000 0072  r....rg...rT...r
+00001330: 3100 0000 290e 723f 0000 0072 3300 0000  1...).r?...r3...
+00001340: 7220 0000 00da 076e 6461 7272 6179 da04  r .....ndarray..
+00001350: 6e64 696d da04 7369 7a65 da05 7374 6163  ndim..size..stac
+00001360: 6bda 0154 7269 0000 0072 0500 0000 720e  k..Tri...r....r.
+00001370: 0000 00da 046a 6f69 6e72 1200 0000 7234  .....joinr....r4
+00001380: 0000 0029 0772 3600 0000 7219 0000 00da  ...).r6...r.....
+00001390: 0276 795a 0276 7ada 0276 785a 066e 5f65  .vyZ.vz..vxZ.n_e
+000013a0: 6c65 6d72 4a00 0000 7224 0000 0072 2400  lemrJ...r$...r$.
+000013b0: 0000 7225 0000 0072 3500 0000 a000 0000  ..r%...r5.......
+000013c0: 7326 0000 0008 0108 0104 010c 0104 0122  s&............."
+000013d0: 0104 0104 ff04 0104 0112 0108 0216 0102  ................
+000013e0: 011a 0102 0108 fe04 0512 017a 1956 6f6c  ...........z.Vol
+000013f0: 5665 6374 6f72 4669 656c 642e 7365 745f  VectorField.set_
+00001400: 7661 6c75 6573 6301 0000 0000 0000 0000  valuesc.........
+00001410: 0000 0002 0000 0005 0000 0043 0000 0073  ...........C...s
+00001420: 3600 0000 7c00 a000 a100 7d01 7c01 6400  6...|.....}.|.d.
+00001430: 6400 8502 6401 6602 1900 7c01 6400 6400  d...d.f...|.d.d.
+00001440: 8502 6402 6602 1900 7c01 6400 6400 8502  ..d.f...|.d.d...
+00001450: 6403 6602 1900 6603 5300 2904 4e72 0100  d.f...f.S.).Nr..
+00001460: 0000 7217 0000 00e9 0200 0000 2901 725a  ..r.........).rZ
+00001470: 0000 0029 0272 3600 0000 da03 6172 7272  ...).r6.....arrr
+00001480: 2400 0000 7224 0000 0072 2500 0000 da0e  $...r$...r%.....
+00001490: 6765 745f 636f 6d70 6f6e 656e 7473 b500  get_components..
+000014a0: 0000 7304 0000 0008 012e 017a 1d56 6f6c  ..s........z.Vol
+000014b0: 5665 6374 6f72 4669 656c 642e 6765 745f  VectorField.get_
+000014c0: 636f 6d70 6f6e 656e 7473 725b 0000 0029  componentsr[...)
+000014d0: 0672 5c00 0000 725d 0000 0072 5e00 0000  .r\...r]...r^...
+000014e0: 7210 0000 0072 3500 0000 727a 0000 0072  r....r5...rz...r
+000014f0: 2400 0000 7224 0000 0072 2400 0000 7225  $...r$...r$...r%
+00001500: 0000 0072 6c00 0000 9d00 0000 7308 0000  ...rl.......s...
+00001510: 0008 0004 010a 020c 1572 6c00 0000 6300  .........rl...c.
+00001520: 0000 0000 0000 0000 0000 0000 0000 0002  ................
+00001530: 0000 0040 0000 0072 6500 0000 2905 da0e  ...@...re...)...
+00001540: 566f 6c54 656e 736f 7246 6965 6c64 5a0e  VolTensorFieldZ.
+00001550: 766f 6c54 656e 736f 7246 6965 6c64 6302  volTensorFieldc.
+00001560: 0000 0000 0000 0000 0000 0002 0000 0004  ................
+00001570: 0000 0043 0000 0073 3000 0000 7400 7c01  ...C...s0...t.|.
+00001580: 7401 6a02 8302 720b 7c01 6a03 6401 6b03  t.j...r.|.j.d.k.
+00001590: 720f 7404 6402 8301 8201 7c00 6a05 a006  r.t.d.....|.j...
+000015a0: 6403 7c01 a102 0100 6400 5300 2904 4e72  d.|.....d.S.).Nr
+000015b0: 7800 0000 7a36 6e6f 7420 6973 696e 7374  x...z6not isinst
+000015c0: 616e 6365 2876 616c 7565 732c 206e 702e  ance(values, np.
+000015d0: 6e64 6172 7261 7929 206f 7220 7661 6c75  ndarray) or valu
+000015e0: 6573 2e6e 6469 6d20 213d 2032 7231 0000  es.ndim != 2r1..
+000015f0: 0029 0772 3300 0000 7220 0000 0072 7000  .).r3...r ...rp.
+00001600: 0000 7271 0000 00da 134e 6f74 496d 706c  ..rq.....NotImpl
+00001610: 656d 656e 7465 6445 7272 6f72 7212 0000  ementedErrorr...
+00001620: 0072 3400 0000 7244 0000 0072 2400 0000  .r4...rD...r$...
+00001630: 7224 0000 0072 2500 0000 7235 0000 00bd  r$...r%...r5....
+00001640: 0000 0073 0a00 0000 1601 0201 0201 04ff  ...s............
+00001650: 1204 7a19 566f 6c54 656e 736f 7246 6965  ..z.VolTensorFie
+00001660: 6c64 2e73 6574 5f76 616c 7565 734e 726a  ld.set_valuesNrj
+00001670: 0000 0072 2400 0000 7224 0000 0072 2400  ...r$...r$...r$.
+00001680: 0000 7225 0000 0072 7b00 0000 ba00 0000  ..r%...r{.......
+00001690: 726b 0000 0072 7b00 0000 6301 0000 0000  rk...r{...c.....
+000016a0: 0000 0000 0000 0002 0000 0004 0000 0043  ...............C
+000016b0: 0000 0073 1400 0000 6900 7c00 5d06 7d01  ...s....i.|.].}.
+000016c0: 7c01 6a00 7c01 9302 7102 5300 7224 0000  |.j.|...q.S.r$..
+000016d0: 0029 0172 1000 0000 2902 7248 0000 0072  .).r....).rH...r
+000016e0: 1000 0000 7224 0000 0072 2400 0000 7225  ....r$...r$...r%
+000016f0: 0000 0072 4b00 0000 c600 0000 7306 0000  ...rK.......s...
+00001700: 0006 0008 0106 ff72 4b00 0000 6301 0000  .......rK...c...
+00001710: 0000 0000 0000 0000 0004 0000 0008 0000  ................
+00001720: 0043 0000 0073 8a00 0000 6400 7d01 7400  .C...s....d.}.t.
+00001730: 7c00 6401 8302 8f22 7d02 7c02 4400 5d17  |.d...."}.|.D.].
+00001740: 7d03 7c03 a001 a100 7d03 7c03 a002 6402  }.|.....}.|...d.
+00001750: a101 7221 7c03 a003 a100 6403 1900 6400  ..r!|.....d...d.
+00001760: 6403 8502 1900 7d01 0100 6e01 710a 5700  d.....}...n.q.W.
+00001770: 6400 0400 0400 8303 0100 6e08 3100 732c  d.........n.1.s,
+00001780: 7701 0100 0100 0100 5900 0100 7c01 6400  w.......Y...|.d.
+00001790: 7500 723c 7404 6404 7c00 9b00 9d02 8301  u.r<t.d.|.......
+000017a0: 8201 7405 7c01 1900 7d01 7c01 a006 7c00  ..t.|...}.|...|.
+000017b0: a101 5300 2905 4eda 0172 fa06 636c 6173  ..S.).N..r..clas
+000017c0: 7320 e9ff ffff ff7a 186e 6f20 636c 6173  s .....z.no clas
+000017d0: 7320 666f 756e 6420 666f 7220 6669 6c65  s found for file
+000017e0: 2029 0772 4000 0000 721c 0000 0072 1d00   ).r@...r....r..
+000017f0: 0000 da05 7370 6c69 74da 0c52 756e 7469  ....split..Runti
+00001800: 6d65 4572 726f 72da 0763 6c61 7373 6573  meError..classes
+00001810: 722a 0000 0029 0472 2700 0000 7210 0000  r*...).r'...r...
+00001820: 0072 4200 0000 da04 6c69 6e65 7224 0000  .rB.....liner$..
+00001830: 0072 2400 0000 7225 0000 00da 0f72 6561  .r$...r%.....rea
+00001840: 645f 6669 656c 645f 6669 6c65 cb00 0000  d_field_file....
+00001850: 731c 0000 0004 010c 0108 0108 010a 0114  s...............
+00001860: 0104 0102 fe02 801c fd08 070e 0108 020a  ................
+00001870: 0272 8400 0000 7216 0000 0063 0200 0000  .r....r....c....
+00001880: 0000 0000 0000 0000 0500 0000 0400 0000  ................
+00001890: 6300 0000 734e 0000 0081 0074 007c 0183  c...sN.....t.|..
+000018a0: 017d 0264 017d 0309 007c 00a0 017c 017c  .}.d.}...|...|.|
+000018b0: 03a1 027d 047c 0464 036b 0272 1b7c 007c  ...}.|.d.k.r.|.|
+000018c0: 0364 0085 0219 0056 0001 0064 0053 007c  .d.....V...d.S.|
+000018d0: 007c 037c 0485 0219 0056 0001 007c 047c  .|.|.....V...|.|
+000018e0: 0217 007d 0371 0829 044e 7201 0000 0054  ...}.q.).Nr....T
+000018f0: 727f 0000 0029 0272 6900 0000 da04 6669  r....).ri.....fi
+00001900: 6e64 2905 da06 736f 7572 6365 da03 7365  nd)...source..se
+00001910: 705a 0773 6570 7369 7a65 da05 7374 6172  pZ.sepsize..star
+00001920: 74da 0369 6478 7224 0000 0072 2400 0000  t..idxr$...r$...
+00001930: 7225 0000 00da 075f 6973 706c 6974 dc00  r%....._isplit..
+00001940: 0000 7316 0000 0002 8008 0104 0102 010c  ..s.............
+00001950: 0108 010e 0104 010e 0108 0102 fa72 8a00  .............r..
+00001960: 0000 6301 0000 0000 0000 0000 0000 0003  ..c.............
+00001970: 0000 0005 0000 0043 0000 0073 6800 0000  .......C...sh...
+00001980: 7400 7c00 8301 4400 5d17 7d01 7c01 a001  t.|...D.].}.|...
+00001990: a100 7d01 7c01 a002 6401 a101 721b 7c01  ..}.|...d...r.|.
+000019a0: a003 a100 6402 1900 6400 6402 8502 1900  ....d...d.d.....
+000019b0: 7d02 0100 6e01 7104 7c02 6400 7500 722b  }...n.q.|.d.u.r+
+000019c0: 7404 6403 7c00 6400 6404 8502 1900 9b02  t.d.|.d.d.......
+000019d0: 9d02 8301 8201 7405 7c02 1900 7d02 7c02  ......t.|...}.|.
+000019e0: a006 7c00 a101 5300 2905 4e72 7e00 0000  ..|...S.).Nr~...
+000019f0: 727f 0000 007a 2b6e 6f20 636c 6173 7320  r....z+no class 
+00001a00: 666f 756e 6420 666f 7220 7468 6973 2063  found for this c
+00001a10: 6f64 653a 2063 6f64 655b 3a35 3030 5d20  ode: code[:500] 
+00001a20: 3d20 69f4 0100 0029 0772 8a00 0000 721c  = i....).r....r.
+00001a30: 0000 0072 1d00 0000 7280 0000 0072 8100  ...r....r....r..
+00001a40: 0000 7282 0000 0072 2600 0000 2903 7211  ..r....r&...).r.
+00001a50: 0000 0072 8300 0000 7210 0000 0072 2400  ...r....r....r$.
+00001a60: 0000 7224 0000 0072 2500 0000 da16 6372  ..r$...r%.....cr
+00001a70: 6561 7465 5f66 6965 6c64 5f66 726f 6d5f  eate_field_from_
+00001a80: 636f 6465 e800 0000 7314 0000 000c 0108  code....s.......
+00001a90: 010a 0114 0104 0102 fe08 0416 0108 020a  ................
+00001aa0: 0272 8b00 0000 2901 7216 0000 0029 22da  .r....).r....)".
+00001ab0: 075f 5f64 6f63 5f5f 721e 0000 00da 0361  .__doc__r......a
+00001ac0: 6263 7202 0000 0072 0300 0000 da02 696f  bcr....r......io
+00001ad0: 7204 0000 00da 076e 756d 6265 7273 7205  r......numbersr.
+00001ae0: 0000 00da 0770 6174 686c 6962 7206 0000  .....pathlibr...
+00001af0: 00da 056e 756d 7079 7220 0000 00da 1d66  ...numpyr .....f
+00001b00: 6c75 6964 7369 6d66 6f61 6d2e 666f 616d  luidsimfoam.foam
+00001b10: 5f69 6e70 7574 5f66 696c 6573 7207 0000  _input_filesr...
+00001b20: 005a 2166 6c75 6964 7369 6d66 6f61 6d2e  .Z!fluidsimfoam.
+00001b30: 666f 616d 5f69 6e70 7574 5f66 696c 6573  foam_input_files
+00001b40: 2e61 7374 7208 0000 0072 0900 0000 720a  .astr....r....r.
+00001b50: 0000 0072 0b00 0000 720c 0000 0072 0d00  ...r....r....r..
+00001b60: 0000 720e 0000 0072 6200 0000 7263 0000  ..r....rb...rc..
+00001b70: 0072 6400 0000 720f 0000 0072 6600 0000  .rd...r....rf...
+00001b80: 726c 0000 0072 7b00 0000 7282 0000 0072  rl...r{...r....r
+00001b90: 8400 0000 728a 0000 0072 8b00 0000 7224  ....r....r....r$
+00001ba0: 0000 0072 2400 0000 7224 0000 0072 2500  ...r$...r$...r%.
+00001bb0: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
+00001bc0: 732e 0000 0004 0008 0410 010c 010c 010c  s...............
+00001bd0: 0108 020c 0224 0104 0a02 0202 ff04 0310  .....$..........
+00001be0: 0310 7010 0e10 1d06 0c08 0106 ff08 050a  ..p.............
+00001bf0: 110c 0c                                  ...
```

### Comparing `fluidsimfoam-0.0.5/src/fluidsimfoam/foam_input_files/__pycache__/fv_options.cpython-39.pyc` & `fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/__pycache__/fv_options.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May 22 08:22:36 2023 UTC, .py size: 6107 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 16% similar despite different names*

```diff
@@ -1,310 +1,313 @@
-00000000: 610d 0d0a 0000 0000 4c26 6b64 db17 0000  a.......L&kd....
+00000000: 6f0d 0d0a 0000 0000 faba 6b64 db17 0000  o.........kd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 6c00 0000 6400  .....@...sl...d.
+00000020: 0006 0000 0040 0000 0073 7000 0000 6400  .....@...sp...d.
 00000030: 5a00 6401 6402 6c01 5a02 6401 6403 6c03  Z.d.d.l.Z.d.d.l.
 00000040: 6d04 5a04 6d05 5a05 6d06 5a06 6d07 5a07  m.Z.m.Z.m.Z.m.Z.
-00000050: 6d08 5a08 0100 6404 6405 8400 5a09 650a  m.Z...d.d...Z.e.
-00000060: 650b 650a 6406 9c03 6407 6408 8404 5a0c  e.e.d...d.d...Z.
-00000070: 6409 640a 8400 5a0d 4700 640b 640c 8400  d.d...Z.G.d.d...
-00000080: 640c 8302 5a0e 4700 640d 640e 8400 640e  d...Z.G.d.d...d.
-00000090: 6504 8303 5a0f 6402 5300 290f 7a22 4865  e...Z.d.S.).z"He
-000000a0: 6c70 6572 2074 6f20 6372 6561 7465 2066  lper to create f
-000000b0: 764f 7074 696f 6e73 2066 696c 6573 0a0a  vOptions files..
-000000c0: e900 0000 004e 2905 da0a 4669 6c65 4865  .....N)...FileHe
-000000d0: 6c70 6572 da0d 466f 616d 496e 7075 7446  lper..FoamInputF
-000000e0: 696c 65da 0b5f 6173 5f70 795f 6e61 6d65  ile.._as_py_name
-000000f0: da15 5f63 6f6d 706c 6574 655f 7061 7261  .._complete_para
-00000100: 6d73 5f64 6963 74da 185f 7570 6461 7465  ms_dict.._update
-00000110: 5f64 6963 745f 7769 7468 5f70 6172 616d  _dict_with_param
-00000120: 7363 0200 0000 0000 0000 0000 0000 0400  sc..............
-00000130: 0000 0600 0000 4300 0000 7344 0000 007c  ......C...sD...|
-00000140: 01a0 00a1 0044 005d 365c 027d 027d 0374  .....D.]6\.}.}.t
-00000150: 017c 0374 026a 036a 0483 0272 3674 057c  .|.t.j.j...r6t.|
-00000160: 00a0 067c 0269 00a1 027c 0383 027c 007c  ...|.i...|...|.|
-00000170: 023c 0071 087c 037c 007c 023c 0071 087c  .<.q.|.|.|.<.q.|
-00000180: 0053 00a9 014e 2907 da05 6974 656d 73da  .S...N)...items.
-00000190: 0a69 7369 6e73 7461 6e63 65da 0b63 6f6c  .isinstance..col
-000001a0: 6c65 6374 696f 6e73 da03 6162 63da 074d  lections..abc..M
-000001b0: 6170 7069 6e67 da0b 6465 6570 5f75 7064  apping..deep_upd
-000001c0: 6174 65da 0367 6574 2904 da01 64da 0175  ate..get)...d..u
-000001d0: da01 6bda 0176 a900 7213 0000 00fa 562f  ..k..v..r.....V/
-000001e0: 686f 6d65 2f75 7365 7273 2f61 7567 6965  home/users/augie
-000001f0: 7233 7069 2f44 6576 2f66 6c75 6964 7369  r3pi/Dev/fluidsi
-00000200: 6d66 6f61 6d2f 7372 632f 666c 7569 6473  mfoam/src/fluids
-00000210: 696d 666f 616d 2f66 6f61 6d5f 696e 7075  imfoam/foam_inpu
-00000220: 745f 6669 6c65 732f 6676 5f6f 7074 696f  t_files/fv_optio
-00000230: 6e73 2e70 7972 0d00 0000 0f00 0000 730a  ns.pyr........s.
-00000240: 0000 0000 0210 010e 0118 020a 0172 0d00  .............r..
-00000250: 0000 2903 da07 6465 6661 756c 74da 0f6e  ..)...default..n
-00000260: 616d 655f 7061 7261 6d65 7465 7273 da06  ame_parameters..
-00000270: 7265 7375 6c74 6303 0000 0000 0000 0000  resultc.........
-00000280: 0000 000a 0000 0009 0000 0043 0000 0073  ...........C...s
-00000290: dc00 0000 7c00 a000 a100 4400 5d78 5c02  ....|.....D.]x\.
-000002a0: 7d03 7d04 7401 7c04 7402 8302 7270 7403  }.}.t.|.t...rpt.
-000002b0: 8300 7d05 7c01 4400 5d2c 7d06 7c06 a004  ..}.|.D.],}.|...
-000002c0: 7c03 6401 1700 a101 7224 7c05 a005 7c06  |.d.....r$|...|.
-000002d0: 7406 7c03 8301 6402 1700 6400 8502 1900  t.|...d...d.....
-000002e0: a101 0100 7124 7c05 7280 6900 7c02 7c03  ....q$|.r.i.|.|.
-000002f0: 3c00 7407 7c04 7c05 7c02 7c03 1900 8303  <.t.|.|.|.|.....
-00000300: 0100 7108 7c03 7c01 7600 7208 7c04 7c02  ..q.|.|.v.r.|.|.
-00000310: 7c03 3c00 7108 7c01 4400 5d50 7d06 7c06  |.<.q.|.D.]P}.|.
-00000320: a008 6401 a101 7d07 7c00 7d08 7a16 7c07  ..d...}.|.}.z.|.
-00000330: 4400 5d0c 7d09 7c08 7c09 1900 7d08 719e  D.].}.|.|...}.q.
-00000340: 5700 7186 0400 7409 79d4 0100 0100 0100  W.q...t.y.......
-00000350: 740a 6403 7c06 9b00 6404 7c00 9b00 9d04  t.d.|...d.|.....
-00000360: 8301 8201 5900 7186 3000 7186 7c02 5300  ....Y.q.0.q.|.S.
-00000370: 2905 4efa 012f e901 0000 00fa 0127 7a28  ).N../.......'z(
-00000380: 2720 646f 6573 206e 6f74 2063 6f72 7265  ' does not corre
-00000390: 7370 6f6e 6420 746f 2061 2070 6172 616d  spond to a param
-000003a0: 6574 6572 2069 6e20 290b 7208 0000 0072  eter in ).r....r
-000003b0: 0900 0000 da04 6469 6374 da03 7365 74da  ......dict..set.
-000003c0: 0a73 7461 7274 7377 6974 68da 0361 6464  .startswith..add
-000003d0: da03 6c65 6eda 195f 6d61 6b65 5f64 6566  ..len.._make_def
-000003e0: 6175 6c74 5f70 6172 616d 735f 6469 6374  ault_params_dict
-000003f0: da05 7370 6c69 74da 084b 6579 4572 726f  ..split..KeyErro
-00000400: 72da 0a56 616c 7565 4572 726f 7229 0a72  r..ValueError).r
-00000410: 1500 0000 7216 0000 0072 1700 0000 da04  ....r....r......
-00000420: 6e61 6d65 da05 7661 6c75 655a 106e 616d  name..valueZ.nam
-00000430: 655f 7061 7261 6d65 7465 7273 315a 0966  e_parameters1Z.f
-00000440: 756c 6c5f 6e61 6d65 da04 6b65 7973 da05  ull_name..keys..
-00000450: 7468 696e 67da 036b 6579 7213 0000 0072  thing..keyr....r
-00000460: 1300 0000 7214 0000 0072 2000 0000 1900  ....r....r .....
-00000470: 0000 732c 0000 0000 0110 010a 0106 0108  ..s,............
-00000480: 010e 011c 0204 0108 0112 0208 010a 0308  ................
-00000490: 010a 0104 0102 0108 010e 010c 0102 010e  ................
-000004a0: ff0c 0472 2000 0000 6303 0000 0000 0000  ...r ...c.......
-000004b0: 0000 0000 0006 0000 0004 0000 0043 0000  .............C..
-000004c0: 0073 6600 0000 6401 6402 8400 7c00 7c01  .sf...d.d...|.|.
-000004d0: 7c02 6603 4400 8301 7d03 7400 7c03 8301  |.f.D...}.t.|...
-000004e0: 7d04 7c04 6403 6b02 7228 6404 5300 7c04  }.|.d.k.r(d.S.|.
-000004f0: 6405 6b04 7234 7401 8201 7c00 6400 7501  d.k.r4t...|.d.u.
-00000500: 7242 6406 7d05 6e20 7c01 6400 7501 7250  rBd.}.n |.d.u.rP
-00000510: 6407 7d05 6e12 7c02 6400 7501 725e 6408  d.}.n.|.d.u.r^d.
-00000520: 7d05 6e04 7402 8201 7c05 5300 2909 4e63  }.n.t...|.S.).Nc
-00000530: 0100 0000 0000 0000 0000 0000 0200 0000  ................
-00000540: 0400 0000 5300 0000 7314 0000 0067 007c  ....S...s....g.|
-00000550: 005d 0c7d 017c 0164 0075 0191 0271 0453  .].}.|.d.u...q.S
-00000560: 0072 0700 0000 7213 0000 0029 02da 022e  .r....r....)....
-00000570: 30da 0376 6172 7213 0000 0072 1300 0000  0..varr....r....
-00000580: 7214 0000 00da 0a3c 6c69 7374 636f 6d70  r......<listcomp
-00000590: 3e38 0000 00f3 0000 0000 7a26 6765 745f  >8........z&get_
-000005a0: 7365 6c65 6374 696f 6e5f 6d6f 6465 2e3c  selection_mode.<
-000005b0: 6c6f 6361 6c73 3e2e 3c6c 6973 7463 6f6d  locals>.<listcom
-000005c0: 703e 7201 0000 00da 0361 6c6c 7219 0000  p>r......allr...
-000005d0: 00da 0863 656c 6c5a 6f6e 65da 0763 656c  ...cellZone..cel
-000005e0: 6c53 6574 da06 706f 696e 7473 2903 da03  lSet..points)...
-000005f0: 7375 6d72 2300 0000 da0c 5275 6e74 696d  sumr#.....Runtim
-00000600: 6545 7272 6f72 2906 da09 6365 6c6c 5f7a  eError)...cell_z
-00000610: 6f6e 65da 0863 656c 6c5f 7365 7472 3000  one..cell_setr0.
-00000620: 0000 5a0b 6973 5f6e 6f74 5f6e 6f6e 655a  ..Z.is_not_noneZ
-00000630: 0f6e 625f 7661 725f 6e6f 745f 6e6f 6e65  .nb_var_not_none
-00000640: 5a0e 7365 6c65 6374 696f 6e5f 6d6f 6465  Z.selection_mode
-00000650: 7213 0000 0072 1300 0000 7214 0000 00da  r....r....r.....
-00000660: 1267 6574 5f73 656c 6563 7469 6f6e 5f6d  .get_selection_m
-00000670: 6f64 6537 0000 0073 1c00 0000 0001 1401  ode7...s........
-00000680: 0802 0801 0401 0801 0402 0801 0601 0801  ................
-00000690: 0601 0801 0602 0402 7235 0000 0063 0000  ........r5...c..
-000006a0: 0000 0000 0000 0000 0000 0000 0000 0700  ................
-000006b0: 0000 4000 0000 7326 0000 0065 005a 0164  ..@...s&...e.Z.d
-000006c0: 005a 0264 0964 0364 0484 015a 0364 0564  .Z.d.d.d...Z.d.d
-000006d0: 0684 005a 0464 0764 0884 005a 0564 0253  ...Z.d.d...Z.d.S
-000006e0: 0029 0ada 0846 764f 7074 696f 6e54 4e63  .)...FvOptionTNc
-000006f0: 0a00 0000 0000 0000 0000 0000 0a00 0000  ................
-00000700: 0300 0000 4300 0000 7398 0000 007c 017c  ....C...s....|.|
-00000710: 005f 007c 027c 005f 017c 0964 0075 0072  ._.|.|._.|.d.u.r
-00000720: 1c74 0283 007d 096e 0874 027c 0983 017d  .t...}.n.t.|...}
-00000730: 097c 0764 0075 0172 3c7c 0864 0075 0172  .|.d.u.r<|.d.u.r
-00000740: 3c74 0364 0183 0182 017c 0764 0075 0072  <t.d.....|.d.u.r
-00000750: 4869 007d 077c 017c 0764 023c 007c 037c  Hi.}.|.|.d.<.|.|
-00000760: 005f 047c 087c 005f 057c 0864 0075 0172  ._.|.|._.|.d.u.r
-00000770: 767c 087c 0764 033c 007c 0164 0417 007c  v|.|.d.<.|.d...|
-00000780: 005f 067c 047c 005f 077c 057c 005f 087c  ._.|.|._.|.|._.|
-00000790: 067c 005f 097c 077c 005f 0a7c 097c 005f  .|._.|.|._.|.|._
-000007a0: 0b64 0053 0029 054e 7a2a 6465 6661 756c  .d.S.).Nz*defaul
-000007b0: 7420 6973 206e 6f74 204e 6f6e 6520 616e  t is not None an
-000007c0: 6420 636f 6566 6673 2069 7320 6e6f 7420  d coeffs is not 
-000007d0: 4e6f 6e65 da04 7479 7065 da06 636f 6566  None..type..coef
-000007e0: 6673 5a06 436f 6566 6673 290c 7237 0000  fsZ.Coeffs).r7..
-000007f0: 0072 2400 0000 721c 0000 0072 2300 0000  .r$...r....r#...
-00000800: da06 6163 7469 7665 7238 0000 00da 0f6e  ..activer8.....n
-00000810: 616d 655f 636f 6566 6673 5f6b 6579 7233  ame_coeffs_keyr3
-00000820: 0000 0072 3400 0000 7230 0000 0072 1500  ...r4...r0...r..
-00000830: 0000 da0a 7061 7261 6d65 7465 7273 a90a  ....parameters..
-00000840: da04 7365 6c66 7237 0000 0072 2400 0000  ..selfr7...r$...
-00000850: 7239 0000 0072 3300 0000 7234 0000 0072  r9...r3...r4...r
-00000860: 3000 0000 7215 0000 0072 3800 0000 723b  0...r....r8...r;
-00000870: 0000 0072 1300 0000 7213 0000 0072 1400  ...r....r....r..
-00000880: 0000 da08 5f5f 696e 6974 5f5f 4d00 0000  ....__init__M...
-00000890: 7328 0000 0000 0c06 0106 0208 0108 0208  s(..............
-000008a0: 0210 0108 0208 0104 0208 0106 0206 0108  ................
-000008b0: 0108 010a 0206 0106 0106 0206 017a 1146  .............z.F
-000008c0: 764f 7074 696f 6e2e 5f5f 696e 6974 5f5f  vOption.__init__
-000008d0: 6302 0000 0000 0000 0000 0000 0004 0000  c...............
-000008e0: 0005 0000 0043 0000 0073 6000 0000 7c00  .....C...s`...|.
-000008f0: 6a00 7c00 6a01 7c00 6a02 7c00 6a03 6401  j.|.j.|.j.|.j.d.
-00000900: 9c03 6402 9c02 7d02 7c00 6a04 6400 7500  ..d...}.|.j.d.u.
-00000910: 722c 7c00 6a05 7d03 6e14 7406 6403 6404  r,|.j.}.n.t.d.d.
-00000920: 8400 7c00 6a05 4400 8301 8301 7d03 7407  ..|.j.D.....}.t.
-00000930: 7c00 6a08 7c03 7c02 8303 0100 7409 7c01  |.j.|.|.....t.|.
-00000940: 7c00 6a0a 7c02 8303 0100 6400 5300 2905  |.j.|.....d.S.).
-00000950: 4e29 0372 3300 0000 7234 0000 0072 3000  N).r3...r4...r0.
-00000960: 0000 2902 7239 0000 00da 0973 656c 6563  ..).r9.....selec
-00000970: 7469 6f6e 6301 0000 0000 0000 0000 0000  tionc...........
-00000980: 0002 0000 0003 0000 0073 0000 0073 1600  .........s...s..
-00000990: 0000 7c00 5d0e 7d01 6400 7c01 1700 5600  ..|.].}.d.|...V.
-000009a0: 0100 7102 6401 5300 2902 7a07 636f 6566  ..q.d.S.).z.coef
-000009b0: 6673 2f4e 7213 0000 0029 0272 2900 0000  fs/Nr....).r)...
-000009c0: 7224 0000 0072 1300 0000 7213 0000 0072  r$...r....r....r
-000009d0: 1400 0000 da09 3c67 656e 6578 7072 3e82  ......<genexpr>.
-000009e0: 0000 0072 2c00 0000 7a2b 4676 4f70 7469  ...r,...z+FvOpti
-000009f0: 6f6e 2e63 6f6d 706c 6574 655f 7061 7261  on.complete_para
-00000a00: 6d73 2e3c 6c6f 6361 6c73 3e2e 3c67 656e  ms.<locals>.<gen
-00000a10: 6578 7072 3e29 0b72 3900 0000 7233 0000  expr>).r9...r3..
-00000a20: 0072 3400 0000 7230 0000 0072 3800 0000  .r4...r0...r8...
-00000a30: 723b 0000 0072 1c00 0000 7220 0000 0072  r;...r....r ...r
-00000a40: 1500 0000 7205 0000 0072 2400 0000 2904  ....r....r$...).
-00000a50: 723d 0000 00da 1170 6172 616d 735f 6676  r=.....params_fv
-00000a60: 5f6f 7074 696f 6e73 5a0e 6465 6661 756c  _optionsZ.defaul
-00000a70: 745f 7061 7261 6d73 723b 0000 0072 1300  t_paramsr;...r..
-00000a80: 0000 7213 0000 0072 1400 0000 da0f 636f  ..r....r......co
-00000a90: 6d70 6c65 7465 5f70 6172 616d 7376 0000  mplete_paramsv..
-00000aa0: 0073 1600 0000 0002 0402 0401 0401 04fd  .s..............
-00000ab0: 04fe 0608 0a01 0802 1401 0e01 7a18 4676  ............z.Fv
-00000ac0: 4f70 7469 6f6e 2e63 6f6d 706c 6574 655f  Option.complete_
-00000ad0: 7061 7261 6d73 6302 0000 0000 0000 0000  paramsc.........
-00000ae0: 0000 0009 0000 0004 0000 0043 0000 0073  ...........C...s
-00000af0: d400 0000 7c01 7400 7c00 6a01 8301 1900  ....|.t.|.j.....
-00000b00: 7d02 7c00 6a02 6400 6401 9c02 7d03 7c00  }.|.j.d.d...}.|.
-00000b10: 6a03 6400 7500 722a 7c03 7d04 6e0c 7c03  j.d.u.r*|.}.n.|.
-00000b20: a004 6402 6900 a102 7d04 7c02 6a05 7d05  ..d.i...}.|.j.}.
-00000b30: 7406 7c05 6a07 7c05 6a08 7c05 6a09 8303  t.|.j.|.j.|.j...
-00000b40: 7c04 6403 3c00 6404 4400 5d24 7d06 7400  |.d.<.d.D.]$}.t.
-00000b50: 7c06 8301 7d07 7c05 7c07 1900 6400 7501  |...}.|.|...d.u.
-00000b60: 7256 7c05 7c07 1900 7c04 7c06 3c00 7156  rV|.|...|.|.<.qV
-00000b70: 740a 7c03 7c00 6a0b 8302 0100 740c 7c03  t.|.|.j.....t.|.
-00000b80: 7c02 8302 0100 7c02 6a0d 7d08 740e 7c08  |.....|.j.}.t.|.
-00000b90: 740f 8302 72ae 6405 7410 7c08 8301 1900  t...r.d.t.|.....
-00000ba0: 7d08 7c08 7c03 6406 3c00 7c00 6a03 6400  }.|.|.d.<.|.j.d.
-00000bb0: 7501 72d0 7c03 a011 6402 a101 7c03 7c00  u.r.|...d...|.|.
-00000bc0: 6a12 3c00 7c03 5300 2907 4e29 0272 3700  j.<.|.S.).N).r7.
-00000bd0: 0000 7239 0000 0072 3800 0000 5a0d 7365  ..r9...r8...Z.se
-00000be0: 6c65 6374 696f 6e4d 6f64 6529 0372 2e00  lectionMode).r..
-00000bf0: 0000 722f 0000 0072 3000 0000 2902 da02  ..r/...r0...)...
-00000c00: 6e6f da03 7965 7372 3900 0000 2913 7204  no..yesr9...).r.
-00000c10: 0000 0072 2400 0000 7237 0000 0072 3800  ...r$...r7...r8.
-00000c20: 0000 da0a 7365 7464 6566 6175 6c74 723f  ....setdefaultr?
-00000c30: 0000 0072 3500 0000 7233 0000 0072 3400  ...r5...r3...r4.
-00000c40: 0000 7230 0000 0072 0d00 0000 7215 0000  ..r0...r....r...
-00000c50: 0072 0600 0000 7239 0000 0072 0900 0000  .r....r9...r....
-00000c60: da04 626f 6f6c da03 696e 74da 0370 6f70  ..bool..int..pop
-00000c70: 723a 0000 0029 0972 3d00 0000 7241 0000  r:...).r=...rA..
-00000c80: 005a 0d70 6172 616d 735f 6f70 7469 6f6e  .Z.params_option
-00000c90: 5a0d 6469 6374 5f66 6f72 5f74 7265 655a  Z.dict_for_treeZ
-00000ca0: 0b64 6963 745f 7365 6c65 6374 da06 7365  .dict_select..se
-00000cb0: 6c65 6374 7228 0000 005a 0e6b 6579 5f61  lectr(...Z.key_a
-00000cc0: 735f 7079 5f6e 616d 6572 3900 0000 7213  s_py_namer9...r.
-00000cd0: 0000 0072 1300 0000 7214 0000 00da 1167  ...r....r......g
-00000ce0: 6574 5f64 6963 745f 666f 725f 7472 6565  et_dict_for_tree
-00000cf0: 8600 0000 732c 0000 0000 010e 020c 020a  ....s,..........
-00000d00: 0106 020c 0206 0102 010c ff08 0408 0108  ................
-00000d10: 010c 010e 020c 020a 0206 010a 010c 0108  ................
-00000d20: 010a 0110 017a 1a46 764f 7074 696f 6e2e  .....z.FvOption.
-00000d30: 6765 745f 6469 6374 5f66 6f72 5f74 7265  get_dict_for_tre
-00000d40: 6529 0754 4e4e 4e4e 4e4e 2906 da08 5f5f  e).TNNNNNN)...__
-00000d50: 6e61 6d65 5f5f da0a 5f5f 6d6f 6475 6c65  name__..__module
-00000d60: 5f5f da0c 5f5f 7175 616c 6e61 6d65 5f5f  __..__qualname__
-00000d70: 723e 0000 0072 4200 0000 724a 0000 0072  r>...rB...rJ...r
-00000d80: 1300 0000 7213 0000 0072 1300 0000 7214  ....r....r....r.
-00000d90: 0000 0072 3600 0000 4c00 0000 7314 0000  ...r6...L...s...
-00000da0: 0008 0500 0100 0100 0100 0100 0100 0100  ................
-00000db0: f60a 2908 1072 3600 0000 6300 0000 0000  ..)..r6...c.....
-00000dc0: 0000 0000 0000 0000 0000 0008 0000 0040  ...............@
-00000dd0: 0000 0073 3600 0000 6500 5a01 6400 5a02  ...s6...e.Z.d.Z.
-00000de0: 6401 6402 8400 5a03 640d 6405 6406 8401  d.d...Z.d.d.d...
-00000df0: 5a04 6407 6408 8400 5a05 6409 640a 8400  Z.d.d...Z.d.d...
-00000e00: 5a06 640b 640c 8400 5a07 6403 5300 290e  Z.d.d...Z.d.S.).
-00000e10: da0f 4676 4f70 7469 6f6e 7348 656c 7065  ..FvOptionsHelpe
-00000e20: 7263 0100 0000 0000 0000 0000 0000 0100  rc..............
-00000e30: 0000 0200 0000 4300 0000 730a 0000 0069  ......C...s....i
-00000e40: 007c 005f 0064 0053 0072 0700 0000 a901  .|._.d.S.r......
-00000e50: da07 6f70 7469 6f6e 7329 0172 3d00 0000  ..options).r=...
-00000e60: 7213 0000 0072 1300 0000 7214 0000 0072  r....r....r....r
-00000e70: 3e00 0000 a800 0000 7302 0000 0000 017a  >.......s......z
-00000e80: 1846 764f 7074 696f 6e73 4865 6c70 6572  .FvOptionsHelper
-00000e90: 2e5f 5f69 6e69 745f 5f4e 5463 0a00 0000  .__init__NTc....
-00000ea0: 0000 0000 0000 0000 0a00 0000 0a00 0000  ................
-00000eb0: 4300 0000 732e 0000 007c 0264 0075 0072  C...s....|.d.u.r
-00000ec0: 0c7c 017d 0274 007c 017c 027c 037c 047c  .|.}.t.|.|.|.|.|
-00000ed0: 057c 067c 077c 087c 0983 097c 006a 017c  .|.|.|.|...|.j.|
-00000ee0: 023c 0064 0053 0072 0700 0000 2902 7236  .<.d.S.r....).r6
-00000ef0: 0000 0072 5000 0000 723c 0000 0072 1300  ...rP...r<...r..
-00000f00: 0000 7213 0000 0072 1400 0000 da0a 6164  ..r....r......ad
-00000f10: 645f 6f70 7469 6f6e ab00 0000 731a 0000  d_option....s...
-00000f20: 0000 0c08 0104 0202 0102 0102 0102 0102  ................
-00000f30: 0102 0102 0102 0102 0102 f77a 1a46 764f  ...........z.FvO
-00000f40: 7074 696f 6e73 4865 6c70 6572 2e61 6464  ptionsHelper.add
-00000f50: 5f6f 7074 696f 6e63 0200 0000 0000 0000  _optionc........
-00000f60: 0000 0000 0200 0000 0200 0000 4300 0000  ............C...
-00000f70: 730c 0000 007c 006a 007c 013d 0064 0053  s....|.j.|.=.d.S
-00000f80: 0072 0700 0000 724f 0000 0029 0272 3d00  .r....rO...).r=.
-00000f90: 0000 7224 0000 0072 1300 0000 7213 0000  ..r$...r....r...
-00000fa0: 0072 1400 0000 da0d 7265 6d6f 7665 5f6f  .r......remove_o
-00000fb0: 7074 696f 6ec6 0000 0073 0200 0000 0001  ption....s......
-00000fc0: 7a1d 4676 4f70 7469 6f6e 7348 656c 7065  z.FvOptionsHelpe
-00000fd0: 722e 7265 6d6f 7665 5f6f 7074 696f 6e63  r.remove_optionc
-00000fe0: 0200 0000 0000 0000 0000 0000 0400 0000  ................
-00000ff0: 0400 0000 4300 0000 732c 0000 007c 016a  ....C...s,...|.j
-00001000: 0064 0164 0264 038d 027d 027c 006a 01a0  .d.d.d...}.|.j..
-00001010: 02a1 0044 005d 0e7d 037c 03a0 037c 02a1  ...D.].}.|...|..
-00001020: 0101 0071 1864 0053 0029 044e da0a 6676  ...q.d.S.).N..fv
-00001030: 5f6f 7074 696f 6e73 da04 544f 444f 2901  _options..TODO).
-00001040: da03 646f 6329 04da 0a5f 7365 745f 6368  ..doc)..._set_ch
-00001050: 696c 6472 5000 0000 da06 7661 6c75 6573  ildrP.....values
-00001060: 7242 0000 0029 0472 3d00 0000 da06 7061  rB...).r=.....pa
-00001070: 7261 6d73 7241 0000 00da 066f 7074 696f  ramsrA.....optio
-00001080: 6e72 1300 0000 7213 0000 0072 1400 0000  nr....r....r....
-00001090: 7242 0000 00c9 0000 0073 0600 0000 0001  rB.......s......
-000010a0: 0e01 0e01 7a1f 4676 4f70 7469 6f6e 7348  ....z.FvOptionsH
-000010b0: 656c 7065 722e 636f 6d70 6c65 7465 5f70  elper.complete_p
-000010c0: 6172 616d 7363 0200 0000 0000 0000 0000  aramsc..........
-000010d0: 0000 0500 0000 0700 0000 4300 0000 7344  ..........C...sD
-000010e0: 0000 0074 0064 0164 0264 0364 0464 0564  ...t.d.d.d.d.d.d
-000010f0: 069c 0564 078d 017d 027c 006a 01a0 02a1  ...d...}.|.j....
-00001100: 0044 005d 1e5c 027d 037d 047c 02a0 037c  .D.].\.}.}.|...|
-00001110: 037c 04a0 047c 016a 05a1 0169 01a1 0101  .|...|.j...i....
-00001120: 0071 207c 0253 0029 084e 6700 0000 0000  .q |.S.).Ng.....
-00001130: 0000 40da 0561 7363 6969 da0a 6469 6374  ..@..ascii..dict
-00001140: 696f 6e61 7279 7a08 2273 7973 7465 6d22  ionaryz."system"
-00001150: da09 6676 4f70 7469 6f6e 7329 05da 0776  ..fvOptions)...v
-00001160: 6572 7369 6f6e da06 666f 726d 6174 da05  ersion..format..
-00001170: 636c 6173 73da 086c 6f63 6174 696f 6eda  class..location.
-00001180: 066f 626a 6563 7429 01da 0469 6e66 6f29  .object)...info)
-00001190: 0672 0300 0000 7250 0000 0072 0800 0000  .r....rP...r....
-000011a0: da14 696e 6974 5f66 726f 6d5f 7079 5f6f  ..init_from_py_o
-000011b0: 626a 6563 7473 724a 0000 0072 5300 0000  bjectsrJ...rS...
-000011c0: 2905 723d 0000 0072 5800 0000 da04 7472  ).r=...rX.....tr
-000011d0: 6565 7224 0000 0072 5900 0000 7213 0000  eer$...rY...r...
-000011e0: 0072 1300 0000 7214 0000 00da 096d 616b  .r....r......mak
-000011f0: 655f 7472 6565 ce00 0000 731a 0000 0000  e_tree....s.....
-00001200: 0102 0202 0102 0102 0102 0102 fb04 ff06  ................
-00001210: 0912 0104 010e ff06 037a 1946 764f 7074  .........z.FvOpt
-00001220: 696f 6e73 4865 6c70 6572 2e6d 616b 655f  ionsHelper.make_
-00001230: 7472 6565 2908 4e54 4e4e 4e4e 4e4e 2908  tree).NTNNNNNN).
-00001240: 724b 0000 0072 4c00 0000 724d 0000 0072  rK...rL...rM...r
-00001250: 3e00 0000 7251 0000 0072 5200 0000 7242  >...rQ...rR...rB
-00001260: 0000 0072 6500 0000 7213 0000 0072 1300  ...re...r....r..
-00001270: 0000 7213 0000 0072 1400 0000 724e 0000  ..r....r....rN..
-00001280: 00a7 0000 0073 1a00 0000 0801 0806 0001  .....s..........
-00001290: 0001 0001 0001 0001 0001 0001 00f6 0a1b  ................
-000012a0: 0803 0805 724e 0000 0029 10da 075f 5f64  ....rN...)...__d
-000012b0: 6f63 5f5f da0f 636f 6c6c 6563 7469 6f6e  oc__..collection
-000012c0: 732e 6162 6372 0a00 0000 5a1d 666c 7569  s.abcr....Z.flui
-000012d0: 6473 696d 666f 616d 2e66 6f61 6d5f 696e  dsimfoam.foam_in
-000012e0: 7075 745f 6669 6c65 7372 0200 0000 7203  put_filesr....r.
-000012f0: 0000 0072 0400 0000 7205 0000 0072 0600  ...r....r....r..
-00001300: 0000 720d 0000 0072 1b00 0000 721c 0000  ..r....r....r...
-00001310: 0072 2000 0000 7235 0000 0072 3600 0000  .r ...r5...r6...
-00001320: 724e 0000 0072 1300 0000 7213 0000 0072  rN...r....r....r
-00001330: 1300 0000 7214 0000 00da 083c 6d6f 6475  ....r......<modu
-00001340: 6c65 3e01 0000 0073 0e00 0000 0403 0802  le>....s........
-00001350: 1c09 080a 121e 0815 0e5b                 .........[
+00000050: 6d08 5a08 0100 6404 6405 8400 5a09 6406  m.Z...d.d...Z.d.
+00000060: 650a 6407 650b 6408 650a 6606 6409 640a  e.d.e.d.e.f.d.d.
+00000070: 8404 5a0c 640b 640c 8400 5a0d 4700 640d  ..Z.d.d...Z.G.d.
+00000080: 640e 8400 640e 8302 5a0e 4700 640f 6410  d...d...Z.G.d.d.
+00000090: 8400 6410 6504 8303 5a0f 6402 5300 2911  ..d.e...Z.d.S.).
+000000a0: 7a22 4865 6c70 6572 2074 6f20 6372 6561  z"Helper to crea
+000000b0: 7465 2066 764f 7074 696f 6e73 2066 696c  te fvOptions fil
+000000c0: 6573 0a0a e900 0000 004e 2905 da0a 4669  es.......N)...Fi
+000000d0: 6c65 4865 6c70 6572 da0d 466f 616d 496e  leHelper..FoamIn
+000000e0: 7075 7446 696c 65da 0b5f 6173 5f70 795f  putFile.._as_py_
+000000f0: 6e61 6d65 da15 5f63 6f6d 706c 6574 655f  name.._complete_
+00000100: 7061 7261 6d73 5f64 6963 74da 185f 7570  params_dict.._up
+00000110: 6461 7465 5f64 6963 745f 7769 7468 5f70  date_dict_with_p
+00000120: 6172 616d 7363 0200 0000 0000 0000 0000  aramsc..........
+00000130: 0000 0400 0000 0600 0000 4300 0000 7344  ..........C...sD
+00000140: 0000 007c 01a0 00a1 0044 005d 1b5c 027d  ...|.....D.].\.}
+00000150: 027d 0374 017c 0374 026a 036a 0483 0272  .}.t.|.t.j.j...r
+00000160: 1b74 057c 00a0 067c 0269 00a1 027c 0383  .t.|...|.i...|..
+00000170: 027c 007c 023c 0071 047c 037c 007c 023c  .|.|.<.q.|.|.|.<
+00000180: 0071 047c 0053 00a9 014e 2907 da05 6974  .q.|.S...N)...it
+00000190: 656d 73da 0a69 7369 6e73 7461 6e63 65da  ems..isinstance.
+000001a0: 0b63 6f6c 6c65 6374 696f 6e73 da03 6162  .collections..ab
+000001b0: 63da 074d 6170 7069 6e67 da0b 6465 6570  c..Mapping..deep
+000001c0: 5f75 7064 6174 65da 0367 6574 2904 da01  _update..get)...
+000001d0: 64da 0175 da01 6bda 0176 a900 7213 0000  d..u..k..v..r...
+000001e0: 00fa 4d2f 686f 6d65 2f70 6965 7272 652f  ..M/home/pierre/
+000001f0: 4465 762f 666c 7569 6473 696d 666f 616d  Dev/fluidsimfoam
+00000200: 2f73 7263 2f66 6c75 6964 7369 6d66 6f61  /src/fluidsimfoa
+00000210: 6d2f 666f 616d 5f69 6e70 7574 5f66 696c  m/foam_input_fil
+00000220: 6573 2f66 765f 6f70 7469 6f6e 732e 7079  es/fv_options.py
+00000230: 720d 0000 000f 0000 0073 0a00 0000 1002  r........s......
+00000240: 0e01 1801 0a02 0401 720d 0000 00da 0764  ........r......d
+00000250: 6566 6175 6c74 da0f 6e61 6d65 5f70 6172  efault..name_par
+00000260: 616d 6574 6572 73da 0672 6573 756c 7463  ameters..resultc
+00000270: 0300 0000 0000 0000 0000 0000 0a00 0000  ................
+00000280: 0900 0000 4300 0000 73d6 0000 007c 00a0  ....C...s....|..
+00000290: 00a1 0044 005d 3c5c 027d 037d 0474 017c  ...D.]<\.}.}.t.|
+000002a0: 0474 0283 0272 3874 0383 007d 057c 0144  .t...r8t...}.|.D
+000002b0: 005d 167d 067c 06a0 047c 0364 0117 00a1  .].}.|...|.d....
+000002c0: 0172 287c 05a0 057c 0674 067c 0383 0164  .r(|...|.t.|...d
+000002d0: 0217 0064 0085 0219 00a1 0101 0071 127c  ...d.........q.|
+000002e0: 0572 3769 007c 027c 033c 0074 077c 047c  .r7i.|.|.<.t.|.|
+000002f0: 057c 027c 0319 0083 0301 0071 047c 037c  .|.|.......q.|.|
+00000300: 0176 0072 407c 047c 027c 033c 0071 047c  .v.r@|.|.|.<.q.|
+00000310: 0144 005d 257d 067c 06a0 0864 01a1 017d  .D.]%}.|...d...}
+00000320: 077c 007d 087a 0b7c 0744 005d 067d 097c  .|.}.z.|.D.].}.|
+00000330: 087c 0919 007d 0871 4f57 0071 4304 0074  .|...}.qOW.qC..t
+00000340: 0979 6801 0001 0001 0074 0a64 037c 069b  .yh......t.d.|..
+00000350: 0064 047c 009b 009d 0483 0182 0177 007c  .d.|.........w.|
+00000360: 0253 0029 054e fa01 2fe9 0100 0000 fa01  .S.).N../.......
+00000370: 277a 2827 2064 6f65 7320 6e6f 7420 636f  'z(' does not co
+00000380: 7272 6573 706f 6e64 2074 6f20 6120 7061  rrespond to a pa
+00000390: 7261 6d65 7465 7220 696e 2029 0b72 0800  rameter in ).r..
+000003a0: 0000 7209 0000 00da 0464 6963 74da 0373  ..r......dict..s
+000003b0: 6574 da0a 7374 6172 7473 7769 7468 da03  et..startswith..
+000003c0: 6164 64da 036c 656e da19 5f6d 616b 655f  add..len.._make_
+000003d0: 6465 6661 756c 745f 7061 7261 6d73 5f64  default_params_d
+000003e0: 6963 74da 0573 706c 6974 da08 4b65 7945  ict..split..KeyE
+000003f0: 7272 6f72 da0a 5661 6c75 6545 7272 6f72  rror..ValueError
+00000400: 290a 7215 0000 0072 1600 0000 7217 0000  ).r....r....r...
+00000410: 00da 046e 616d 65da 0576 616c 7565 5a10  ...name..valueZ.
+00000420: 6e61 6d65 5f70 6172 616d 6574 6572 7331  name_parameters1
+00000430: da09 6675 6c6c 5f6e 616d 65da 046b 6579  ..full_name..key
+00000440: 73da 0574 6869 6e67 da03 6b65 7972 1300  s..thing..keyr..
+00000450: 0000 7213 0000 0072 1400 0000 7220 0000  ..r....r....r ..
+00000460: 0019 0000 0073 3600 0000 1001 0a01 0601  .....s6.........
+00000470: 0801 0e01 1a01 0280 0402 0801 1001 0280  ................
+00000480: 0802 0801 0280 0803 0a01 0401 0201 0801  ................
+00000490: 0a01 04ff 0c02 0201 0e01 04ff 02ff 0405  ................
+000004a0: 7220 0000 0063 0300 0000 0000 0000 0000  r ...c..........
+000004b0: 0000 0600 0000 0400 0000 4300 0000 7368  ..........C...sh
+000004c0: 0000 0064 0164 0284 007c 007c 017c 0266  ...d.d...|.|.|.f
+000004d0: 0344 0083 017d 0374 007c 0383 017d 047c  .D...}.t.|...}.|
+000004e0: 0464 036b 0272 1464 0453 007c 0464 056b  .d.k.r.d.S.|.d.k
+000004f0: 0472 1a74 0182 017c 0064 0075 0172 2264  .r.t...|.d.u.r"d
+00000500: 067d 057c 0553 007c 0164 0075 0172 2a64  .}.|.S.|.d.u.r*d
+00000510: 077d 057c 0553 007c 0264 0075 0172 3264  .}.|.S.|.d.u.r2d
+00000520: 087d 057c 0553 0074 0282 0129 094e 6301  .}.|.S.t...).Nc.
+00000530: 0000 0000 0000 0000 0000 0002 0000 0004  ................
+00000540: 0000 0053 0000 0073 1400 0000 6700 7c00  ...S...s....g.|.
+00000550: 5d06 7d01 7c01 6400 7501 9102 7102 5300  ].}.|.d.u...q.S.
+00000560: 7207 0000 0072 1300 0000 2902 da02 2e30  r....r....)....0
+00000570: da03 7661 7272 1300 0000 7213 0000 0072  ..varr....r....r
+00000580: 1400 0000 da0a 3c6c 6973 7463 6f6d 703e  ......<listcomp>
+00000590: 3800 0000 7302 0000 0014 007a 2667 6574  8...s......z&get
+000005a0: 5f73 656c 6563 7469 6f6e 5f6d 6f64 652e  _selection_mode.
+000005b0: 3c6c 6f63 616c 733e 2e3c 6c69 7374 636f  <locals>.<listco
+000005c0: 6d70 3e72 0100 0000 da03 616c 6c72 1900  mp>r......allr..
+000005d0: 0000 da08 6365 6c6c 5a6f 6e65 da07 6365  ....cellZone..ce
+000005e0: 6c6c 5365 74da 0670 6f69 6e74 7329 03da  llSet..points)..
+000005f0: 0373 756d 7223 0000 00da 0c52 756e 7469  .sumr#.....Runti
+00000600: 6d65 4572 726f 7229 06da 0963 656c 6c5f  meError)...cell_
+00000610: 7a6f 6e65 da08 6365 6c6c 5f73 6574 7230  zone..cell_setr0
+00000620: 0000 005a 0b69 735f 6e6f 745f 6e6f 6e65  ...Z.is_not_none
+00000630: 5a0f 6e62 5f76 6172 5f6e 6f74 5f6e 6f6e  Z.nb_var_not_non
+00000640: 655a 0e73 656c 6563 7469 6f6e 5f6d 6f64  eZ.selection_mod
+00000650: 6572 1300 0000 7213 0000 0072 1400 0000  er....r....r....
+00000660: da12 6765 745f 7365 6c65 6374 696f 6e5f  ..get_selection_
+00000670: 6d6f 6465 3700 0000 7320 0000 0014 0108  mode7...s ......
+00000680: 0108 0204 0108 0104 0108 0204 0104 0808  ................
+00000690: f904 0104 0608 fb04 0104 0404 fe72 3500  .............r5.
+000006a0: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
+000006b0: 0000 0003 0000 0040 0000 0073 3400 0000  .......@...s4...
+000006c0: 6500 5a01 6400 5a02 0901 0902 0902 0902  e.Z.d.Z.........
+000006d0: 0902 0902 0902 6409 6403 6404 8401 5a03  ......d.d.d...Z.
+000006e0: 6405 6406 8400 5a04 6407 6408 8400 5a05  d.d...Z.d.d...Z.
+000006f0: 6402 5300 290a da08 4676 4f70 7469 6f6e  d.S.)...FvOption
+00000700: 544e 630a 0000 0000 0000 0000 0000 000a  TNc.............
+00000710: 0000 0003 0000 0043 0000 0073 9800 0000  .......C...s....
+00000720: 7c01 7c00 5f00 7c02 7c00 5f01 7c09 6400  |.|._.|.|._.|.d.
+00000730: 7500 720e 7402 8300 7d09 6e04 7402 7c09  u.r.t...}.n.t.|.
+00000740: 8301 7d09 7c07 6400 7501 721e 7c08 6400  ..}.|.d.u.r.|.d.
+00000750: 7501 721e 7403 6401 8301 8201 7c07 6400  u.r.t.d.....|.d.
+00000760: 7500 7224 6900 7d07 7c01 7c07 6402 3c00  u.r$i.}.|.|.d.<.
+00000770: 7c03 7c00 5f04 7c08 7c00 5f05 7c08 6400  |.|._.|.|._.|.d.
+00000780: 7501 723b 7c08 7c07 6403 3c00 7c01 6404  u.r;|.|.d.<.|.d.
+00000790: 1700 7c00 5f06 7c04 7c00 5f07 7c05 7c00  ..|._.|.|._.|.|.
+000007a0: 5f08 7c06 7c00 5f09 7c07 7c00 5f0a 7c09  _.|.|._.|.|._.|.
+000007b0: 7c00 5f0b 6400 5300 2905 4e7a 2a64 6566  |._.d.S.).Nz*def
+000007c0: 6175 6c74 2069 7320 6e6f 7420 4e6f 6e65  ault is not None
+000007d0: 2061 6e64 2063 6f65 6666 7320 6973 206e   and coeffs is n
+000007e0: 6f74 204e 6f6e 65da 0474 7970 65da 0663  ot None..type..c
+000007f0: 6f65 6666 735a 0643 6f65 6666 7329 0c72  oeffsZ.Coeffs).r
+00000800: 3700 0000 7224 0000 0072 1c00 0000 7223  7...r$...r....r#
+00000810: 0000 00da 0661 6374 6976 6572 3800 0000  .....activer8...
+00000820: da0f 6e61 6d65 5f63 6f65 6666 735f 6b65  ..name_coeffs_ke
+00000830: 7972 3300 0000 7234 0000 0072 3000 0000  yr3...r4...r0...
+00000840: 7215 0000 00da 0a70 6172 616d 6574 6572  r......parameter
+00000850: 73a9 0ada 0473 656c 6672 3700 0000 7224  s....selfr7...r$
+00000860: 0000 0072 3900 0000 7233 0000 0072 3400  ...r9...r3...r4.
+00000870: 0000 7230 0000 0072 1500 0000 7238 0000  ..r0...r....r8..
+00000880: 0072 3b00 0000 7213 0000 0072 1300 0000  .r;...r....r....
+00000890: 7214 0000 00da 085f 5f69 6e69 745f 5f4d  r......__init__M
+000008a0: 0000 0073 2800 0000 060c 0601 0802 0801  ...s(...........
+000008b0: 0802 1002 0801 0802 0401 0802 0601 0602  ................
+000008c0: 0801 0801 0a01 0602 0601 0601 0602 0a01  ................
+000008d0: 7a11 4676 4f70 7469 6f6e 2e5f 5f69 6e69  z.FvOption.__ini
+000008e0: 745f 5f63 0200 0000 0000 0000 0000 0000  t__c............
+000008f0: 0400 0000 0500 0000 4300 0000 7360 0000  ........C...s`..
+00000900: 007c 006a 007c 006a 017c 006a 027c 006a  .|.j.|.j.|.j.|.j
+00000910: 0364 019c 0364 029c 027d 027c 006a 0464  .d...d...}.|.j.d
+00000920: 0075 0072 167c 006a 057d 036e 0a74 0664  .u.r.|.j.}.n.t.d
+00000930: 0364 0484 007c 006a 0544 0083 0183 017d  .d...|.j.D.....}
+00000940: 0374 077c 006a 087c 037c 0283 0301 0074  .t.|.j.|.|.....t
+00000950: 097c 017c 006a 0a7c 0283 0301 0064 0053  .|.|.j.|.....d.S
+00000960: 0029 054e 2903 7233 0000 0072 3400 0000  .).N).r3...r4...
+00000970: 7230 0000 0029 0272 3900 0000 da09 7365  r0...).r9.....se
+00000980: 6c65 6374 696f 6e63 0100 0000 0000 0000  lectionc........
+00000990: 0000 0000 0200 0000 0300 0000 7300 0000  ............s...
+000009a0: 7318 0000 0081 007c 005d 077d 0164 007c  s......|.].}.d.|
+000009b0: 0117 0056 0001 0071 0264 0153 0029 027a  ...V...q.d.S.).z
+000009c0: 0763 6f65 6666 732f 4e72 1300 0000 2902  .coeffs/Nr....).
+000009d0: 722a 0000 0072 2400 0000 7213 0000 0072  r*...r$...r....r
+000009e0: 1300 0000 7214 0000 00da 093c 6765 6e65  ....r......<gene
+000009f0: 7870 723e 8200 0000 7304 0000 0002 8016  xpr>....s.......
+00000a00: 007a 2b46 764f 7074 696f 6e2e 636f 6d70  .z+FvOption.comp
+00000a10: 6c65 7465 5f70 6172 616d 732e 3c6c 6f63  lete_params.<loc
+00000a20: 616c 733e 2e3c 6765 6e65 7870 723e 290b  als>.<genexpr>).
+00000a30: 7239 0000 0072 3300 0000 7234 0000 0072  r9...r3...r4...r
+00000a40: 3000 0000 7238 0000 0072 3b00 0000 721c  0...r8...r;...r.
+00000a50: 0000 0072 2000 0000 7215 0000 0072 0500  ...r ...r....r..
+00000a60: 0000 7224 0000 0029 0472 3d00 0000 da11  ..r$...).r=.....
+00000a70: 7061 7261 6d73 5f66 765f 6f70 7469 6f6e  params_fv_option
+00000a80: 735a 0e64 6566 6175 6c74 5f70 6172 616d  sZ.default_param
+00000a90: 7372 3b00 0000 7213 0000 0072 1300 0000  sr;...r....r....
+00000aa0: 7214 0000 00da 0f63 6f6d 706c 6574 655f  r......complete_
+00000ab0: 7061 7261 6d73 7600 0000 7316 0000 0004  paramsv...s.....
+00000ac0: 0204 0204 0104 0104 fd06 fe0a 0808 0114  ................
+00000ad0: 020e 0112 017a 1846 764f 7074 696f 6e2e  .....z.FvOption.
+00000ae0: 636f 6d70 6c65 7465 5f70 6172 616d 7363  complete_paramsc
+00000af0: 0200 0000 0000 0000 0000 0000 0900 0000  ................
+00000b00: 0400 0000 4300 0000 73d4 0000 007c 0174  ....C...s....|.t
+00000b10: 007c 006a 0183 0119 007d 027c 006a 0264  .|.j.....}.|.j.d
+00000b20: 0064 019c 027d 037c 006a 0364 0075 0072  .d...}.|.j.d.u.r
+00000b30: 157c 037d 046e 067c 03a0 0464 0269 00a1  .|.}.n.|...d.i..
+00000b40: 027d 047c 026a 057d 0574 067c 056a 077c  .}.|.j.}.t.|.j.|
+00000b50: 056a 087c 056a 0983 037c 0464 033c 0064  .j.|.j...|.d.<.d
+00000b60: 0444 005d 127d 0674 007c 0683 017d 077c  .D.].}.t.|...}.|
+00000b70: 057c 0719 0064 0075 0172 3d7c 057c 0719  .|...d.u.r=|.|..
+00000b80: 007c 047c 063c 0071 2b74 0a7c 037c 006a  .|.|.<.q+t.|.|.j
+00000b90: 0b83 0201 0074 0c7c 037c 0283 0201 007c  .....t.|.|.....|
+00000ba0: 026a 0d7d 0874 0e7c 0874 0f83 0272 5764  .j.}.t.|.t...rWd
+00000bb0: 0574 107c 0883 0119 007d 087c 087c 0364  .t.|.....}.|.|.d
+00000bc0: 063c 007c 006a 0364 0075 0172 687c 03a0  .<.|.j.d.u.rh|..
+00000bd0: 1164 02a1 017c 037c 006a 123c 007c 0353  .d...|.|.j.<.|.S
+00000be0: 0029 074e 2902 7237 0000 0072 3900 0000  .).N).r7...r9...
+00000bf0: 7238 0000 005a 0d73 656c 6563 7469 6f6e  r8...Z.selection
+00000c00: 4d6f 6465 2903 722e 0000 0072 2f00 0000  Mode).r....r/...
+00000c10: 7230 0000 0029 02da 026e 6fda 0379 6573  r0...)...no..yes
+00000c20: 7239 0000 0029 1372 0400 0000 7224 0000  r9...).r....r$..
+00000c30: 0072 3700 0000 7238 0000 00da 0a73 6574  .r7...r8.....set
+00000c40: 6465 6661 756c 7472 3f00 0000 7235 0000  defaultr?...r5..
+00000c50: 0072 3300 0000 7234 0000 0072 3000 0000  .r3...r4...r0...
+00000c60: 720d 0000 0072 1500 0000 7206 0000 0072  r....r....r....r
+00000c70: 3900 0000 7209 0000 00da 0462 6f6f 6cda  9...r......bool.
+00000c80: 0369 6e74 da03 706f 7072 3a00 0000 2909  .int..popr:...).
+00000c90: 723d 0000 0072 4100 0000 5a0d 7061 7261  r=...rA...Z.para
+00000ca0: 6d73 5f6f 7074 696f 6e5a 0d64 6963 745f  ms_optionZ.dict_
+00000cb0: 666f 725f 7472 6565 5a0b 6469 6374 5f73  for_treeZ.dict_s
+00000cc0: 656c 6563 74da 0673 656c 6563 7472 2900  elect..selectr).
+00000cd0: 0000 5a0e 6b65 795f 6173 5f70 795f 6e61  ..Z.key_as_py_na
+00000ce0: 6d65 7239 0000 0072 1300 0000 7213 0000  mer9...r....r...
+00000cf0: 0072 1400 0000 da11 6765 745f 6469 6374  .r......get_dict
+00000d00: 5f66 6f72 5f74 7265 6586 0000 0073 2e00  _for_tree....s..
+00000d10: 0000 0e01 0c02 0a02 0601 0c02 0602 0201  ................
+00000d20: 0c01 08ff 0804 0801 0c01 0c01 0280 0c02  ................
+00000d30: 0a02 0602 0a01 0c01 0801 0a01 1001 0401  ................
+00000d40: 7a1a 4676 4f70 7469 6f6e 2e67 6574 5f64  z.FvOption.get_d
+00000d50: 6963 745f 666f 725f 7472 6565 2907 544e  ict_for_tree).TN
+00000d60: 4e4e 4e4e 4e29 06da 085f 5f6e 616d 655f  NNNNN)...__name_
+00000d70: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
+00000d80: 5f71 7561 6c6e 616d 655f 5f72 3e00 0000  _qualname__r>...
+00000d90: 7242 0000 0072 4a00 0000 7213 0000 0072  rB...rJ...r....r
+00000da0: 1300 0000 7213 0000 0072 1400 0000 7236  ....r....r....r6
+00000db0: 0000 004c 0000 0073 1600 0000 0800 0205  ...L...s........
+00000dc0: 0201 0201 0201 0201 0201 0201 0af6 0829  ...............)
+00000dd0: 0c10 7236 0000 0063 0000 0000 0000 0000  ..r6...c........
+00000de0: 0000 0000 0000 0000 0300 0000 4000 0000  ............@...
+00000df0: 7346 0000 0065 005a 0164 005a 0264 0164  sF...e.Z.d.Z.d.d
+00000e00: 0284 005a 0309 0309 0409 0309 0309 0309  ...Z............
+00000e10: 0309 0309 0364 0d64 0564 0684 015a 0464  .....d.d.d...Z.d
+00000e20: 0764 0884 005a 0564 0964 0a84 005a 0664  .d...Z.d.d...Z.d
+00000e30: 0b64 0c84 005a 0764 0353 0029 0eda 0f46  .d...Z.d.S.)...F
+00000e40: 764f 7074 696f 6e73 4865 6c70 6572 6301  vOptionsHelperc.
+00000e50: 0000 0000 0000 0000 0000 0001 0000 0002  ................
+00000e60: 0000 0043 0000 0073 0a00 0000 6900 7c00  ...C...s....i.|.
+00000e70: 5f00 6400 5300 7207 0000 00a9 01da 076f  _.d.S.r........o
+00000e80: 7074 696f 6e73 2901 723d 0000 0072 1300  ptions).r=...r..
+00000e90: 0000 7213 0000 0072 1400 0000 723e 0000  ..r....r....r>..
+00000ea0: 00a8 0000 0073 0200 0000 0a01 7a18 4676  .....s......z.Fv
+00000eb0: 4f70 7469 6f6e 7348 656c 7065 722e 5f5f  OptionsHelper.__
+00000ec0: 696e 6974 5f5f 4e54 630a 0000 0000 0000  init__NTc.......
+00000ed0: 0000 0000 000a 0000 000a 0000 0043 0000  .............C..
+00000ee0: 0073 2e00 0000 7c02 6400 7500 7206 7c01  .s....|.d.u.r.|.
+00000ef0: 7d02 7400 7c01 7c02 7c03 7c04 7c05 7c06  }.t.|.|.|.|.|.|.
+00000f00: 7c07 7c08 7c09 8309 7c00 6a01 7c02 3c00  |.|.|...|.j.|.<.
+00000f10: 6400 5300 7207 0000 0029 0272 3600 0000  d.S.r....).r6...
+00000f20: 7250 0000 0072 3c00 0000 7213 0000 0072  rP...r<...r....r
+00000f30: 1300 0000 7214 0000 00da 0a61 6464 5f6f  ....r......add_o
+00000f40: 7074 696f 6eab 0000 0073 1a00 0000 080c  ption....s......
+00000f50: 0401 0202 0201 0201 0201 0201 0201 0201  ................
+00000f60: 0201 0201 0201 0ef7 7a1a 4676 4f70 7469  ........z.FvOpti
+00000f70: 6f6e 7348 656c 7065 722e 6164 645f 6f70  onsHelper.add_op
+00000f80: 7469 6f6e 6302 0000 0000 0000 0000 0000  tionc...........
+00000f90: 0002 0000 0002 0000 0043 0000 0073 0c00  .........C...s..
+00000fa0: 0000 7c00 6a00 7c01 3d00 6400 5300 7207  ..|.j.|.=.d.S.r.
+00000fb0: 0000 0072 4f00 0000 2902 723d 0000 0072  ...rO...).r=...r
+00000fc0: 2400 0000 7213 0000 0072 1300 0000 7214  $...r....r....r.
+00000fd0: 0000 00da 0d72 656d 6f76 655f 6f70 7469  .....remove_opti
+00000fe0: 6f6e c600 0000 7302 0000 000c 017a 1d46  on....s......z.F
+00000ff0: 764f 7074 696f 6e73 4865 6c70 6572 2e72  vOptionsHelper.r
+00001000: 656d 6f76 655f 6f70 7469 6f6e 6302 0000  emove_optionc...
+00001010: 0000 0000 0000 0000 0004 0000 0004 0000  ................
+00001020: 0043 0000 0073 2c00 0000 7c01 6a00 6401  .C...s,...|.j.d.
+00001030: 6402 6403 8d02 7d02 7c00 6a01 a002 a100  d.d...}.|.j.....
+00001040: 4400 5d07 7d03 7c03 a003 7c02 a101 0100  D.].}.|...|.....
+00001050: 710c 6400 5300 2904 4eda 0a66 765f 6f70  q.d.S.).N..fv_op
+00001060: 7469 6f6e 73da 0454 4f44 4f29 01da 0364  tions..TODO)...d
+00001070: 6f63 2904 da0a 5f73 6574 5f63 6869 6c64  oc)..._set_child
+00001080: 7250 0000 00da 0676 616c 7565 7372 4200  rP.....valuesrB.
+00001090: 0000 2904 723d 0000 00da 0670 6172 616d  ..).r=.....param
+000010a0: 7372 4100 0000 da06 6f70 7469 6f6e 7213  srA.....optionr.
+000010b0: 0000 0072 1300 0000 7214 0000 0072 4200  ...r....r....rB.
+000010c0: 0000 c900 0000 7308 0000 000e 010e 010c  ......s.........
+000010d0: 0104 ff7a 1f46 764f 7074 696f 6e73 4865  ...z.FvOptionsHe
+000010e0: 6c70 6572 2e63 6f6d 706c 6574 655f 7061  lper.complete_pa
+000010f0: 7261 6d73 6302 0000 0000 0000 0000 0000  ramsc...........
+00001100: 0005 0000 0007 0000 0043 0000 0073 4400  .........C...sD.
+00001110: 0000 7400 6401 6402 6403 6404 6405 6406  ..t.d.d.d.d.d.d.
+00001120: 9c05 6407 8d01 7d02 7c00 6a01 a002 a100  ..d...}.|.j.....
+00001130: 4400 5d0f 5c02 7d03 7d04 7c02 a003 7c03  D.].\.}.}.|...|.
+00001140: 7c04 a004 7c01 6a05 a101 6901 a101 0100  |...|.j...i.....
+00001150: 7110 7c02 5300 2908 4e67 0000 0000 0000  q.|.S.).Ng......
+00001160: 0040 da05 6173 6369 69da 0a64 6963 7469  .@..ascii..dicti
+00001170: 6f6e 6172 797a 0822 7379 7374 656d 225a  onaryz."system"Z
+00001180: 0966 764f 7074 696f 6e73 2905 da07 7665  .fvOptions)...ve
+00001190: 7273 696f 6eda 0666 6f72 6d61 74da 0563  rsion..format..c
+000011a0: 6c61 7373 da08 6c6f 6361 7469 6f6e da06  lass..location..
+000011b0: 6f62 6a65 6374 2901 da04 696e 666f 2906  object)...info).
+000011c0: 7203 0000 0072 5000 0000 7208 0000 00da  r....rP...r.....
+000011d0: 1469 6e69 745f 6672 6f6d 5f70 795f 6f62  .init_from_py_ob
+000011e0: 6a65 6374 7372 4a00 0000 7253 0000 0029  jectsrJ...rS...)
+000011f0: 0572 3d00 0000 7258 0000 00da 0474 7265  .r=...rX.....tre
+00001200: 6572 2400 0000 7259 0000 0072 1300 0000  er$...rY...r....
+00001210: 7213 0000 0072 1400 0000 da09 6d61 6b65  r....r......make
+00001220: 5f74 7265 65ce 0000 0073 1a00 0000 0201  _tree....s......
+00001230: 0202 0201 0201 0201 0201 04fb 06ff 1209  ................
+00001240: 0401 0e01 06ff 0403 7a19 4676 4f70 7469  ........z.FvOpti
+00001250: 6f6e 7348 656c 7065 722e 6d61 6b65 5f74  onsHelper.make_t
+00001260: 7265 6529 084e 544e 4e4e 4e4e 4e29 0872  ree).NTNNNNNN).r
+00001270: 4b00 0000 724c 0000 0072 4d00 0000 723e  K...rL...rM...r>
+00001280: 0000 0072 5100 0000 7252 0000 0072 4200  ...rQ...rR...rB.
+00001290: 0000 7264 0000 0072 1300 0000 7213 0000  ..rd...r....r...
+000012a0: 0072 1300 0000 7214 0000 0072 4e00 0000  .r....r....rN...
+000012b0: a700 0000 731c 0000 0008 0008 0102 0602  ....s...........
+000012c0: 0102 0102 0102 0102 0102 0102 010a f608  ................
+000012d0: 1b08 030c 0572 4e00 0000 2910 da07 5f5f  .....rN...)...__
+000012e0: 646f 635f 5fda 0f63 6f6c 6c65 6374 696f  doc__..collectio
+000012f0: 6e73 2e61 6263 720a 0000 005a 1d66 6c75  ns.abcr....Z.flu
+00001300: 6964 7369 6d66 6f61 6d2e 666f 616d 5f69  idsimfoam.foam_i
+00001310: 6e70 7574 5f66 696c 6573 7202 0000 0072  nput_filesr....r
+00001320: 0300 0000 7204 0000 0072 0500 0000 7206  ....r....r....r.
+00001330: 0000 0072 0d00 0000 721b 0000 0072 1c00  ...r....r....r..
+00001340: 0000 7220 0000 0072 3500 0000 7236 0000  ..r ...r5...r6..
+00001350: 0072 4e00 0000 7213 0000 0072 1300 0000  .rN...r....r....
+00001360: 7213 0000 0072 1400 0000 da08 3c6d 6f64  r....r......<mod
+00001370: 756c 653e 0100 0000 7310 0000 0004 0008  ule>....s.......
+00001380: 031c 0208 0916 0a08 1e0e 1514 5b         ............[
```

### Comparing `fluidsimfoam-0.0.5/src/fluidsimfoam/foam_input_files/__pycache__/fv_schemes.cpython-39.pyc` & `fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/__pycache__/fv_schemes.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun  1 13:07:51 2023 UTC, .py size: 1987 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 24% similar despite different names*

```diff
@@ -1,152 +1,153 @@
-00000000: 610d 0d0a 0000 0000 2798 7864 c307 0000  a.......'.xd....
+00000000: 6f0d 0d0a 0000 0000 1c64 6e64 c307 0000  o........dnd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4000 0000 6400  .....@...s@...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 6d05 5a05 0100 6401  d.l.m.Z.m.Z...d.
 00000050: 6404 6c06 6d07 5a07 0100 4700 6405 6406  d.l.m.Z...G.d.d.
 00000060: 8400 6406 6504 8303 5a08 6407 5300 2908  ..d.e...Z.d.S.).
 00000070: 7a22 4865 6c70 6572 2074 6f20 6372 6561  z"Helper to crea
 00000080: 7465 2066 7653 6368 656d 6573 2066 696c  te fvSchemes fil
 00000090: 6573 0a0a e900 0000 0029 01da 0a75 6e64  es.......)...und
 000000a0: 6572 7363 6f72 6529 02da 0a46 696c 6548  erscore)...FileH
 000000b0: 656c 7065 72da 0d46 6f61 6d49 6e70 7574  elper..FoamInput
 000000c0: 4669 6c65 2901 da07 6173 5f64 6963 7463  File)...as_dictc
 000000d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000000e0: 0600 0000 4000 0000 7336 0000 0065 005a  ....@...s6...e.Z
-000000f0: 0164 005a 0267 0064 01a2 015a 0364 0b64  .d.Z.g.d...Z.d.d
-00000100: 0364 0484 015a 0464 0564 0684 005a 0564  .d...Z.d.d...Z.d
-00000110: 0764 0884 005a 0664 0964 0a84 005a 0764  .d...Z.d.d...Z.d
-00000120: 0253 0029 0cda 0f46 7653 6368 656d 6573  .S.)...FvSchemes
-00000130: 4865 6c70 6572 2906 da03 6464 74da 0467  Helper)...ddt..g
-00000140: 7261 64da 0364 6976 da09 6c61 706c 6163  rad..div..laplac
-00000150: 6961 6eda 0d69 6e74 6572 706f 6c61 7469  ian..interpolati
-00000160: 6f6e 5a06 736e 4772 6164 4e63 0700 0000  onZ.snGradNc....
-00000170: 0000 0000 0000 0000 0b00 0000 0500 0000  ................
-00000180: 4300 0000 7350 0000 007c 006a 0044 005d  C...sP...|.j.D.]
-00000190: 3e7d 0774 0183 007d 0874 027c 0783 017d  >}.t...}.t.|...}
-000001a0: 097c 087c 0919 0064 0075 0072 2c69 007c  .|.|...d.u.r,i.|
-000001b0: 087c 093c 0074 037c 087c 0919 0083 017d  .|.<.t.|.|.....}
-000001c0: 0a74 047c 007c 097c 0a83 0301 0071 0669  .t.|.|.|.....q.i
-000001d0: 007c 005f 0564 0053 00a9 014e 2906 da04  .|._.d.S...N)...
-000001e0: 6b65 7973 da06 6c6f 6361 6c73 7202 0000  keys..localsr...
-000001f0: 0072 0500 0000 da07 7365 7461 7474 72da  .r......setattr.
-00000200: 0a6f 7468 6572 5f64 6963 7429 0bda 0473  .other_dict)...s
-00000210: 656c 6672 0700 0000 7208 0000 0072 0900  elfr....r....r..
-00000220: 0000 720a 0000 0072 0b00 0000 5a07 736e  ..r....r....Z.sn
-00000230: 5f67 7261 64da 036b 6579 da03 6c6f 63da  _grad..key..loc.
-00000240: 0861 7267 5f6e 616d 65da 0464 6174 61a9  .arg_name..data.
-00000250: 0072 1600 0000 fa56 2f68 6f6d 652f 7573  .r.....V/home/us
-00000260: 6572 732f 6175 6769 6572 3370 692f 4465  ers/augier3pi/De
-00000270: 762f 666c 7569 6473 696d 666f 616d 2f73  v/fluidsimfoam/s
-00000280: 7263 2f66 6c75 6964 7369 6d66 6f61 6d2f  rc/fluidsimfoam/
-00000290: 666f 616d 5f69 6e70 7574 5f66 696c 6573  foam_input_files
-000002a0: 2f66 765f 7363 6865 6d65 732e 7079 da08  /fv_schemes.py..
-000002b0: 5f5f 696e 6974 5f5f 0e00 0000 7310 0000  __init__....s...
-000002c0: 0000 090a 0106 0108 010c 0108 020c 010e  ................
-000002d0: 027a 1846 7653 6368 656d 6573 4865 6c70  .z.FvSchemesHelp
-000002e0: 6572 2e5f 5f69 6e69 745f 5f63 0200 0000  er.__init__c....
-000002f0: 0000 0000 0000 0000 0600 0000 0600 0000  ................
-00000300: 4300 0000 7364 0000 007c 016a 0064 0164  C...sd...|.j.d.d
-00000310: 0264 038d 027d 027c 006a 0144 005d 207d  .d...}.|.j.D.] }
-00000320: 0374 027c 0383 017d 047c 026a 007c 0474  .t.|...}.|.j.|.t
-00000330: 037c 007c 0483 0264 048d 0201 0071 147c  .|.|...d.....q.|
-00000340: 006a 04a0 05a1 0044 005d 1e5c 027d 037d  .j.....D.].\.}.}
-00000350: 0574 027c 0383 017d 047c 026a 007c 047c  .t.|...}.|.j.|.|
-00000360: 0564 048d 0201 0071 4064 0053 0029 054e  .d.....q@d.S.).N
-00000370: da0a 6676 5f73 6368 656d 6573 da04 544f  ..fv_schemes..TO
-00000380: 444f 2901 da03 646f 6329 01da 0761 7474  DO)...doc)...att
-00000390: 7269 6273 2906 da0a 5f73 6574 5f63 6869  ribs)..._set_chi
-000003a0: 6c64 720d 0000 0072 0200 0000 da07 6765  ldr....r......ge
-000003b0: 7461 7474 7272 1000 0000 da05 6974 656d  tattrr......item
-000003c0: 7329 0672 1100 0000 da06 7061 7261 6d73  s).r......params
-000003d0: 7219 0000 0072 1200 0000 da04 6e61 6d65  r....r......name
-000003e0: da05 7661 6c75 6572 1600 0000 7216 0000  ..valuer....r...
-000003f0: 0072 1700 0000 da0f 636f 6d70 6c65 7465  .r......complete
-00000400: 5f70 6172 616d 7322 0000 0073 0e00 0000  _params"...s....
-00000410: 0001 0e01 0a01 0801 1602 1201 0801 7a1f  ..............z.
-00000420: 4676 5363 6865 6d65 7348 656c 7065 722e  FvSchemesHelper.
-00000430: 636f 6d70 6c65 7465 5f70 6172 616d 7363  complete_paramsc
-00000440: 0200 0000 0000 0000 0000 0000 0400 0000  ................
-00000450: 0600 0000 0300 0000 7354 0000 0074 0064  ........sT...t.d
-00000460: 0164 0264 0364 0464 059c 0464 068d 0189  .d.d.d.d...d....
-00000470: 0164 0a87 0087 0166 0264 0764 0884 097d  .d.....f.d.d...}
-00000480: 027c 006a 0144 005d 0c7d 037c 027c 0383  .|.j.D.].}.|.|..
-00000490: 0101 0071 2a7c 006a 0244 005d 107d 037c  ...q*|.j.D.].}.|
-000004a0: 027c 037c 0364 098d 0201 0071 3e88 0153  .|.|.d.....q>..S
-000004b0: 0029 0b4e 6700 0000 0000 0000 40da 0561  .).Ng.......@..a
-000004c0: 7363 6969 da0a 6469 6374 696f 6e61 7279  scii..dictionary
-000004d0: 5a09 6676 5363 6865 6d65 7329 04da 0776  Z.fvSchemes)...v
-000004e0: 6572 7369 6f6e da06 666f 726d 6174 da05  ersion..format..
-000004f0: 636c 6173 73da 066f 626a 6563 7429 01da  class..object)..
-00000500: 0469 6e66 6f63 0200 0000 0000 0000 0000  .infoc..........
-00000510: 0000 0300 0000 0400 0000 1300 0000 7354  ..............sT
-00000520: 0000 007c 0164 0075 0072 107c 0064 0117  ...|.d.u.r.|.d..
-00000530: 007d 0188 016a 0074 017c 0083 0119 0089  .}...j.t.|......
-00000540: 0087 0066 0164 0264 0384 0888 006a 0244  ...f.d.d.....j.D
-00000550: 0083 017d 0264 0464 0384 007c 02a0 03a1  ...}.d.d...|....
-00000560: 0044 0083 017d 0288 02a0 047c 017c 02a1  .D...}.....|.|..
-00000570: 0201 0064 0053 0029 054e 5a07 5363 6865  ...d.S.).NZ.Sche
-00000580: 6d65 7363 0100 0000 0000 0000 0000 0000  mesc............
-00000590: 0200 0000 0500 0000 1300 0000 7316 0000  ............s...
-000005a0: 0069 007c 005d 0e7d 017c 0188 007c 0119  .i.|.].}.|...|..
-000005b0: 0093 0271 0453 0072 1600 0000 7216 0000  ...q.S.r....r...
-000005c0: 0029 02da 022e 30da 016b a901 5a0a 7061  .)....0..k..Z.pa
-000005d0: 7261 6d73 5f6b 6579 7216 0000 0072 1700  rams_keyr....r..
-000005e0: 0000 da0a 3c64 6963 7463 6f6d 703e 3a00  ....<dictcomp>:.
-000005f0: 0000 f300 0000 007a 4046 7653 6368 656d  .......z@FvSchem
-00000600: 6573 4865 6c70 6572 2e6d 616b 655f 7472  esHelper.make_tr
-00000610: 6565 2e3c 6c6f 6361 6c73 3e2e 7365 745f  ee.<locals>.set_
-00000620: 6368 696c 642e 3c6c 6f63 616c 733e 2e3c  child.<locals>.<
-00000630: 6469 6374 636f 6d70 3e63 0100 0000 0000  dictcomp>c......
-00000640: 0000 0000 0000 0300 0000 0400 0000 5300  ..............S.
-00000650: 0000 731e 0000 0069 007c 005d 165c 027d  ..s....i.|.].\.}
-00000660: 017d 027c 0264 0075 0172 047c 017c 0293  .}.|.d.u.r.|.|..
-00000670: 0271 0453 0029 0146 7216 0000 0029 0372  .q.S.).Fr....).r
-00000680: 2b00 0000 722c 0000 00da 0176 7216 0000  +...r,.....vr...
-00000690: 0072 1600 0000 7217 0000 0072 2e00 0000  .r....r....r....
-000006a0: 3b00 0000 722f 0000 0029 0572 1900 0000  ;...r/...).r....
-000006b0: 7202 0000 00da 0c5f 6b65 795f 6174 7472  r......_key_attr
-000006c0: 6962 7372 1f00 0000 da09 7365 745f 6368  ibsr......set_ch
-000006d0: 696c 6429 0372 1200 0000 7221 0000 0072  ild).r....r!...r
-000006e0: 1c00 0000 a902 7220 0000 00da 0474 7265  ......r .....tre
-000006f0: 6572 2d00 0000 7217 0000 0072 3200 0000  er-...r....r2...
-00000700: 3600 0000 730c 0000 0000 0108 0108 010e  6...s...........
-00000710: 0114 0112 017a 2c46 7653 6368 656d 6573  .....z,FvSchemes
-00000720: 4865 6c70 6572 2e6d 616b 655f 7472 6565  Helper.make_tree
-00000730: 2e3c 6c6f 6361 6c73 3e2e 7365 745f 6368  .<locals>.set_ch
-00000740: 696c 6429 0172 2100 0000 2901 4e29 0372  ild).r!...).N).r
-00000750: 0400 0000 720d 0000 0072 1000 0000 2904  ....r....r....).
-00000760: 7211 0000 0072 2000 0000 7232 0000 0072  r....r ...r2...r
-00000770: 1200 0000 7216 0000 0072 3300 0000 7217  ....r....r3...r.
-00000780: 0000 00da 096d 616b 655f 7472 6565 2c00  .....make_tree,.
-00000790: 0000 731a 0000 0000 0102 0202 0102 0102  ..s.............
-000007a0: 0102 fc04 ff06 0910 080a 010a 020a 010e  ................
-000007b0: 027a 1946 7653 6368 656d 6573 4865 6c70  .z.FvSchemesHelp
-000007c0: 6572 2e6d 616b 655f 7472 6565 6303 0000  er.make_treec...
-000007d0: 0000 0000 0000 0000 0003 0000 0003 0000  ................
-000007e0: 0043 0000 0073 0e00 0000 7c02 7c00 6a00  .C...s....|.|.j.
-000007f0: 7c01 3c00 6400 5300 720c 0000 0029 0172  |.<.d.S.r....).r
-00000800: 1000 0000 2903 7211 0000 0072 2100 0000  ....).r....r!...
-00000810: 7215 0000 0072 1600 0000 7216 0000 0072  r....r....r....r
-00000820: 1700 0000 da08 6164 645f 6469 6374 4600  ......add_dictF.
-00000830: 0000 7302 0000 0000 017a 1846 7653 6368  ..s......z.FvSch
-00000840: 656d 6573 4865 6c70 6572 2e61 6464 5f64  emesHelper.add_d
-00000850: 6963 7429 064e 4e4e 4e4e 4e29 08da 085f  ict).NNNNNN)..._
-00000860: 5f6e 616d 655f 5fda 0a5f 5f6d 6f64 756c  _name__..__modul
-00000870: 655f 5fda 0c5f 5f71 7561 6c6e 616d 655f  e__..__qualname_
-00000880: 5f72 0d00 0000 7218 0000 0072 2300 0000  _r....r....r#...
-00000890: 7235 0000 0072 3600 0000 7216 0000 0072  r5...r6...r....r
-000008a0: 1600 0000 7216 0000 0072 1700 0000 7206  ....r....r....r.
-000008b0: 0000 000b 0000 0073 1600 0000 0801 0804  .......s........
-000008c0: 0001 0001 0001 0001 0001 00f9 0a14 080a  ................
-000008d0: 081a 7206 0000 004e 2909 da07 5f5f 646f  ..r....N)...__do
-000008e0: 635f 5fda 0a69 6e66 6c65 6374 696f 6e72  c__..inflectionr
-000008f0: 0200 0000 5a1d 666c 7569 6473 696d 666f  ....Z.fluidsimfo
-00000900: 616d 2e66 6f61 6d5f 696e 7075 745f 6669  am.foam_input_fi
-00000910: 6c65 7372 0300 0000 7204 0000 00da 2266  lesr....r....."f
-00000920: 6c75 6964 7369 6d66 6f61 6d2e 666f 616d  luidsimfoam.foam
-00000930: 5f69 6e70 7574 5f66 696c 6573 2e75 7469  _input_files.uti
-00000940: 6c72 0500 0000 7206 0000 0072 1600 0000  lr....r....r....
-00000950: 7216 0000 0072 1600 0000 7217 0000 00da  r....r....r.....
-00000960: 083c 6d6f 6475 6c65 3e01 0000 0073 0800  .<module>....s..
-00000970: 0000 0404 0c02 1001 0c03                 ..........
+000000e0: 0300 0000 4000 0000 7342 0000 0065 005a  ....@...sB...e.Z
+000000f0: 0164 005a 0267 0064 01a2 015a 0309 0209  .d.Z.g.d...Z....
+00000100: 0209 0209 0209 0209 0264 0b64 0364 0484  .........d.d.d..
+00000110: 015a 0464 0564 0684 005a 0564 0764 0884  .Z.d.d...Z.d.d..
+00000120: 005a 0664 0964 0a84 005a 0764 0253 0029  .Z.d.d...Z.d.S.)
+00000130: 0cda 0f46 7653 6368 656d 6573 4865 6c70  ...FvSchemesHelp
+00000140: 6572 2906 da03 6464 74da 0467 7261 64da  er)...ddt..grad.
+00000150: 0364 6976 da09 6c61 706c 6163 6961 6eda  .div..laplacian.
+00000160: 0d69 6e74 6572 706f 6c61 7469 6f6e 5a06  .interpolationZ.
+00000170: 736e 4772 6164 4e63 0700 0000 0000 0000  snGradNc........
+00000180: 0000 0000 0b00 0000 0500 0000 4300 0000  ............C...
+00000190: 7350 0000 007c 006a 0044 005d 1f7d 0774  sP...|.j.D.].}.t
+000001a0: 0183 007d 0874 027c 0783 017d 097c 087c  ...}.t.|...}.|.|
+000001b0: 0919 0064 0075 0072 1669 007c 087c 093c  ...d.u.r.i.|.|.<
+000001c0: 0074 037c 087c 0919 0083 017d 0a74 047c  .t.|.|.....}.t.|
+000001d0: 007c 097c 0a83 0301 0071 0369 007c 005f  .|.|.....q.i.|._
+000001e0: 0564 0053 00a9 014e 2906 da04 6b65 7973  .d.S...N)...keys
+000001f0: da06 6c6f 6361 6c73 7202 0000 0072 0500  ..localsr....r..
+00000200: 0000 da07 7365 7461 7474 72da 0a6f 7468  ....setattr..oth
+00000210: 6572 5f64 6963 7429 0bda 0473 656c 6672  er_dict)...selfr
+00000220: 0700 0000 7208 0000 0072 0900 0000 720a  ....r....r....r.
+00000230: 0000 0072 0b00 0000 5a07 736e 5f67 7261  ...r....Z.sn_gra
+00000240: 64da 036b 6579 da03 6c6f 63da 0861 7267  d..key..loc..arg
+00000250: 5f6e 616d 65da 0464 6174 61a9 0072 1600  _name..data..r..
+00000260: 0000 fa4d 2f68 6f6d 652f 7069 6572 7265  ...M/home/pierre
+00000270: 2f44 6576 2f66 6c75 6964 7369 6d66 6f61  /Dev/fluidsimfoa
+00000280: 6d2f 7372 632f 666c 7569 6473 696d 666f  m/src/fluidsimfo
+00000290: 616d 2f66 6f61 6d5f 696e 7075 745f 6669  am/foam_input_fi
+000002a0: 6c65 732f 6676 5f73 6368 656d 6573 2e70  les/fv_schemes.p
+000002b0: 79da 085f 5f69 6e69 745f 5f0e 0000 0073  y..__init__....s
+000002c0: 1000 0000 0a09 0601 0801 0c01 0801 0c02  ................
+000002d0: 0e01 0a02 7a18 4676 5363 6865 6d65 7348  ....z.FvSchemesH
+000002e0: 656c 7065 722e 5f5f 696e 6974 5f5f 6302  elper.__init__c.
+000002f0: 0000 0000 0000 0000 0000 0006 0000 0006  ................
+00000300: 0000 0043 0000 0073 6400 0000 7c01 6a00  ...C...sd...|.j.
+00000310: 6401 6402 6403 8d02 7d02 7c00 6a01 4400  d.d.d...}.|.j.D.
+00000320: 5d10 7d03 7402 7c03 8301 7d04 7c02 6a00  ].}.t.|...}.|.j.
+00000330: 7c04 7403 7c00 7c04 8302 6404 8d02 0100  |.t.|.|...d.....
+00000340: 710a 7c00 6a04 a005 a100 4400 5d0f 5c02  q.|.j.....D.].\.
+00000350: 7d03 7d05 7402 7c03 8301 7d04 7c02 6a00  }.}.t.|...}.|.j.
+00000360: 7c04 7c05 6404 8d02 0100 7120 6400 5300  |.|.d.....q d.S.
+00000370: 2905 4eda 0a66 765f 7363 6865 6d65 73da  ).N..fv_schemes.
+00000380: 0454 4f44 4f29 01da 0364 6f63 2901 da07  .TODO)...doc)...
+00000390: 6174 7472 6962 7329 06da 0a5f 7365 745f  attribs)..._set_
+000003a0: 6368 696c 6472 0d00 0000 7202 0000 00da  childr....r.....
+000003b0: 0767 6574 6174 7472 7210 0000 00da 0569  .getattrr......i
+000003c0: 7465 6d73 2906 7211 0000 00da 0670 6172  tems).r......par
+000003d0: 616d 7372 1900 0000 7212 0000 00da 046e  amsr....r......n
+000003e0: 616d 65da 0576 616c 7565 7216 0000 0072  ame..valuer....r
+000003f0: 1600 0000 7217 0000 00da 0f63 6f6d 706c  ....r......compl
+00000400: 6574 655f 7061 7261 6d73 2200 0000 7310  ete_params"...s.
+00000410: 0000 000e 010a 0108 0116 0112 0208 0110  ................
+00000420: 0104 fe7a 1f46 7653 6368 656d 6573 4865  ...z.FvSchemesHe
+00000430: 6c70 6572 2e63 6f6d 706c 6574 655f 7061  lper.complete_pa
+00000440: 7261 6d73 6302 0000 0000 0000 0000 0000  ramsc...........
+00000450: 0004 0000 0006 0000 0003 0000 0073 5400  .............sT.
+00000460: 0000 7400 6401 6402 6403 6404 6405 9c04  ..t.d.d.d.d.d...
+00000470: 6406 8d01 8901 640a 8700 8701 6602 6407  d.....d.....f.d.
+00000480: 6408 8409 7d02 7c00 6a01 4400 5d06 7d03  d...}.|.j.D.].}.
+00000490: 7c02 7c03 8301 0100 7115 7c00 6a02 4400  |.|.....q.|.j.D.
+000004a0: 5d08 7d03 7c02 7c03 7c03 6409 8d02 0100  ].}.|.|.|.d.....
+000004b0: 711f 8801 5300 290b 4e67 0000 0000 0000  q...S.).Ng......
+000004c0: 0040 da05 6173 6369 69da 0a64 6963 7469  .@..ascii..dicti
+000004d0: 6f6e 6172 795a 0966 7653 6368 656d 6573  onaryZ.fvSchemes
+000004e0: 2904 da07 7665 7273 696f 6eda 0666 6f72  )...version..for
+000004f0: 6d61 74da 0563 6c61 7373 da06 6f62 6a65  mat..class..obje
+00000500: 6374 2901 da04 696e 666f 6302 0000 0000  ct)...infoc.....
+00000510: 0000 0000 0000 0003 0000 0004 0000 0013  ................
+00000520: 0000 0073 5400 0000 7c01 6400 7500 7208  ...sT...|.d.u.r.
+00000530: 7c00 6401 1700 7d01 8801 6a00 7401 7c00  |.d...}...j.t.|.
+00000540: 8301 1900 8900 8700 6601 6402 6403 8408  ........f.d.d...
+00000550: 8800 6a02 4400 8301 7d02 6404 6403 8400  ..j.D...}.d.d...
+00000560: 7c02 a003 a100 4400 8301 7d02 8802 a004  |.....D...}.....
+00000570: 7c01 7c02 a102 0100 6400 5300 2905 4e5a  |.|.....d.S.).NZ
+00000580: 0753 6368 656d 6573 6301 0000 0000 0000  .Schemesc.......
+00000590: 0000 0000 0002 0000 0005 0000 0013 0000  ................
+000005a0: 0073 1600 0000 6900 7c00 5d07 7d01 7c01  .s....i.|.].}.|.
+000005b0: 8800 7c01 1900 9302 7102 5300 7216 0000  ..|.....q.S.r...
+000005c0: 0072 1600 0000 2902 da02 2e30 da01 6ba9  .r....)....0..k.
+000005d0: 015a 0a70 6172 616d 735f 6b65 7972 1600  .Z.params_keyr..
+000005e0: 0000 7217 0000 00da 0a3c 6469 6374 636f  ..r......<dictco
+000005f0: 6d70 3e3a 0000 0073 0200 0000 1600 7a40  mp>:...s......z@
+00000600: 4676 5363 6865 6d65 7348 656c 7065 722e  FvSchemesHelper.
+00000610: 6d61 6b65 5f74 7265 652e 3c6c 6f63 616c  make_tree.<local
+00000620: 733e 2e73 6574 5f63 6869 6c64 2e3c 6c6f  s>.set_child.<lo
+00000630: 6361 6c73 3e2e 3c64 6963 7463 6f6d 703e  cals>.<dictcomp>
+00000640: 6301 0000 0000 0000 0000 0000 0003 0000  c...............
+00000650: 0004 0000 0053 0000 0073 1e00 0000 6900  .....S...s....i.
+00000660: 7c00 5d0b 5c02 7d01 7d02 7c02 6400 7501  |.].\.}.}.|.d.u.
+00000670: 7202 7c01 7c02 9302 7102 5300 2901 4672  r.|.|...q.S.).Fr
+00000680: 1600 0000 2903 722b 0000 0072 2c00 0000  ....).r+...r,...
+00000690: da01 7672 1600 0000 7216 0000 0072 1700  ..vr....r....r..
+000006a0: 0000 722e 0000 003b 0000 0073 0200 0000  ..r....;...s....
+000006b0: 1e00 2905 7219 0000 0072 0200 0000 da0c  ..).r....r......
+000006c0: 5f6b 6579 5f61 7474 7269 6273 721f 0000  _key_attribsr...
+000006d0: 00da 0973 6574 5f63 6869 6c64 2903 7212  ...set_child).r.
+000006e0: 0000 0072 2100 0000 721c 0000 00a9 0272  ...r!...r......r
+000006f0: 2000 0000 da04 7472 6565 722d 0000 0072   .....treer-...r
+00000700: 1700 0000 7231 0000 0036 0000 0073 0c00  ....r1...6...s..
+00000710: 0000 0801 0801 0e01 1401 1201 1001 7a2c  ..............z,
+00000720: 4676 5363 6865 6d65 7348 656c 7065 722e  FvSchemesHelper.
+00000730: 6d61 6b65 5f74 7265 652e 3c6c 6f63 616c  make_tree.<local
+00000740: 733e 2e73 6574 5f63 6869 6c64 2901 7221  s>.set_child).r!
+00000750: 0000 0072 0c00 0000 2903 7204 0000 0072  ...r....).r....r
+00000760: 0d00 0000 7210 0000 0029 0472 1100 0000  ....r....).r....
+00000770: 7220 0000 0072 3100 0000 7212 0000 0072  r ...r1...r....r
+00000780: 1600 0000 7232 0000 0072 1700 0000 da09  ....r2...r......
+00000790: 6d61 6b65 5f74 7265 652c 0000 0073 1a00  make_tree,...s..
+000007a0: 0000 0201 0202 0201 0201 0201 04fc 06ff  ................
+000007b0: 1009 0a08 0a01 0a02 0e01 0402 7a19 4676  ............z.Fv
+000007c0: 5363 6865 6d65 7348 656c 7065 722e 6d61  SchemesHelper.ma
+000007d0: 6b65 5f74 7265 6563 0300 0000 0000 0000  ke_treec........
+000007e0: 0000 0000 0300 0000 0300 0000 4300 0000  ............C...
+000007f0: 730e 0000 007c 027c 006a 007c 013c 0064  s....|.|.j.|.<.d
+00000800: 0053 0072 0c00 0000 2901 7210 0000 0029  .S.r....).r....)
+00000810: 0372 1100 0000 7221 0000 0072 1500 0000  .r....r!...r....
+00000820: 7216 0000 0072 1600 0000 7217 0000 00da  r....r....r.....
+00000830: 0861 6464 5f64 6963 7446 0000 0073 0200  .add_dictF...s..
+00000840: 0000 0e01 7a18 4676 5363 6865 6d65 7348  ....z.FvSchemesH
+00000850: 656c 7065 722e 6164 645f 6469 6374 2906  elper.add_dict).
+00000860: 4e4e 4e4e 4e4e 2908 da08 5f5f 6e61 6d65  NNNNNN)...__name
+00000870: 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f da0c  __..__module__..
+00000880: 5f5f 7175 616c 6e61 6d65 5f5f 720d 0000  __qualname__r...
+00000890: 0072 1800 0000 7223 0000 0072 3400 0000  .r....r#...r4...
+000008a0: 7235 0000 0072 1600 0000 7216 0000 0072  r5...r....r....r
+000008b0: 1600 0000 7217 0000 0072 0600 0000 0b00  ....r....r......
+000008c0: 0000 7318 0000 0008 0008 0102 0402 0102  ..s.............
+000008d0: 0102 0102 0102 010a f908 1408 0a0c 1a72  ...............r
+000008e0: 0600 0000 4e29 09da 075f 5f64 6f63 5f5f  ....N)...__doc__
+000008f0: da0a 696e 666c 6563 7469 6f6e 7202 0000  ..inflectionr...
+00000900: 00da 1d66 6c75 6964 7369 6d66 6f61 6d2e  ...fluidsimfoam.
+00000910: 666f 616d 5f69 6e70 7574 5f66 696c 6573  foam_input_files
+00000920: 7203 0000 0072 0400 0000 da22 666c 7569  r....r....."flui
+00000930: 6473 696d 666f 616d 2e66 6f61 6d5f 696e  dsimfoam.foam_in
+00000940: 7075 745f 6669 6c65 732e 7574 696c 7205  put_files.utilr.
+00000950: 0000 0072 0600 0000 7216 0000 0072 1600  ...r....r....r..
+00000960: 0000 7216 0000 0072 1700 0000 da08 3c6d  ..r....r......<m
+00000970: 6f64 756c 653e 0100 0000 730a 0000 0004  odule>....s.....
+00000980: 000c 0410 020c 0114 03                   .........
```

### Comparing `fluidsimfoam-0.0.5/src/fluidsimfoam/foam_input_files/__pycache__/generators.cpython-310.pyc` & `fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/__pycache__/generators.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed May 10 08:15:22 2023 UTC, .py size: 5070 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 9a52 5b64 ce13 0000  o........R[d....
+00000000: 6f0d 0d0a 0000 0000 a570 6c64 8214 0000  o........pld....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 a000 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 6d03 5a03  Z.d.d.l.m.Z.m.Z.
 00000040: 0100 6401 6403 6c04 6d05 5a05 0100 6401  ..d.d.l.m.Z...d.
 00000050: 6404 6c06 6d07 5a07 0100 6401 6405 6c08  d.l.m.Z...d.d.l.
 00000060: 5a08 6401 6406 6c09 6d0a 5a0a 6d0b 5a0b  Z.d.d.l.m.Z.m.Z.
 00000070: 0100 6401 6407 6c0c 6d0d 5a0d 0100 6401  ..d.d.l.m.Z...d.
@@ -33,304 +33,307 @@
 00000200: 0000 0000 0000 0400 0000 0700 0000 4300  ..............C.
 00000210: 0000 7362 0000 007c 017c 005f 0074 0174  ..sb...|.|._.t.t
 00000220: 027c 016a 0383 0183 017d 0274 047c 026a  .|.j.....}.t.|.j
 00000230: 0583 01a0 06a1 006a 0764 011b 007c 005f  .......j.d...|._
 00000240: 0874 09a0 0a74 09a0 0b7c 026a 0c64 01a1  .t...t...|.j.d..
 00000250: 0274 09a0 0b64 0264 03a1 0267 02a1 017d  .t...d.d...g...}
 00000260: 0374 096a 0d7c 0374 096a 0e64 0464 058d  .t.j.|.t.j.d.d..
-00000270: 037c 005f 0f64 0053 0029 064e da09 7465  .|._.d.S.).N..te
+00000270: 037c 005f 0f64 0053 0029 064e 5a09 7465  .|._.d.S.).NZ.te
 00000280: 6d70 6c61 7465 73da 0c66 6c75 6964 7369  mplates..fluidsi
-00000290: 6d66 6f61 6dda 0972 6573 6f75 7263 6573  mfoam..resources
+00000290: 6d66 6f61 6d5a 0972 6573 6f75 7263 6573  mfoamZ.resources
 000002a0: 5429 03da 066c 6f61 6465 72da 0975 6e64  T)...loader..und
-000002b0: 6566 696e 6564 da15 6b65 6570 5f74 7261  efined..keep_tra
+000002b0: 6566 696e 6564 5a15 6b65 6570 5f74 7261  efinedZ.keep_tra
 000002c0: 696c 696e 675f 6e65 776c 696e 6529 10da  iling_newline)..
 000002d0: 066f 7574 7075 7472 0400 0000 da04 7479  .outputr......ty
 000002e0: 7065 da03 7369 6d72 0500 0000 da08 5f5f  pe..simr......__
 000002f0: 6669 6c65 5f5f da08 6162 736f 6c75 7465  file__..absolute
 00000300: da06 7061 7265 6e74 da0d 7465 6d70 6c61  ..parent..templa
-00000310: 7465 735f 6469 72da 066a 696e 6a61 32da  tes_dir..jinja2.
-00000320: 0c43 686f 6963 654c 6f61 6465 72da 0d50  .ChoiceLoader..P
+00000310: 7465 735f 6469 72da 066a 696e 6a61 325a  tes_dir..jinja2Z
+00000320: 0c43 686f 6963 654c 6f61 6465 725a 0d50  .ChoiceLoaderZ.P
 00000330: 6163 6b61 6765 4c6f 6164 6572 da0b 5f5f  ackageLoader..__
-00000340: 7061 636b 6167 655f 5fda 0b45 6e76 6972  package__..Envir
-00000350: 6f6e 6d65 6e74 da0f 5374 7269 6374 556e  onment..StrictUn
+00000340: 7061 636b 6167 655f 5f5a 0b45 6e76 6972  package__Z.Envir
+00000350: 6f6e 6d65 6e74 5a0f 5374 7269 6374 556e  onmentZ.StrictUn
 00000360: 6465 6669 6e65 64da 096a 696e 6a61 5f65  defined..jinja_e
-00000370: 6e76 2904 da04 7365 6c66 7213 0000 00da  nv)...selfr.....
-00000380: 036d 6f64 7210 0000 00a9 0072 2300 0000  .modr......r#...
-00000390: fa56 2f68 6f6d 652f 7573 6572 732f 6175  .V/home/users/au
-000003a0: 6769 6572 3370 692f 4465 762f 666c 7569  gier3pi/Dev/flui
-000003b0: 6473 696d 666f 616d 2f73 7263 2f66 6c75  dsimfoam/src/flu
-000003c0: 6964 7369 6d66 6f61 6d2f 666f 616d 5f69  idsimfoam/foam_i
-000003d0: 6e70 7574 5f66 696c 6573 2f67 656e 6572  nput_files/gener
-000003e0: 6174 6f72 732e 7079 da08 5f5f 696e 6974  ators.py..__init
-000003f0: 5f5f 1100 0000 731a 0000 0006 010e 0116  __....s.........
-00000400: 0104 020c 020a 0102 fe04 ff04 0702 0104  ................
-00000410: 0102 010c fd7a 1349 6e70 7574 4669 6c65  .....z.InputFile
-00000420: 732e 5f5f 696e 6974 5f5f 6302 0000 0000  s.__init__c.....
-00000430: 0000 0000 0000 0002 0000 0003 0000 0043  ...............C
-00000440: 0000 0073 0c00 0000 7c00 6a00 a001 7c01  ...s....|.j...|.
-00000450: a101 5300 a901 4e29 0272 2000 0000 da0c  ..S...N).r .....
-00000460: 6765 745f 7465 6d70 6c61 7465 2902 7221  get_template).r!
-00000470: 0000 00da 0d74 656d 706c 6174 655f 6e61  .....template_na
-00000480: 6d65 7223 0000 0072 2300 0000 7224 0000  mer#...r#...r$..
-00000490: 0072 2700 0000 2300 0000 f302 0000 000c  .r'...#.........
-000004a0: 017a 1749 6e70 7574 4669 6c65 732e 6765  .z.InputFiles.ge
-000004b0: 745f 7465 6d70 6c61 7465 4e29 06da 085f  t_templateN)..._
-000004c0: 5f6e 616d 655f 5fda 0a5f 5f6d 6f64 756c  _name__..__modul
-000004d0: 655f 5fda 0c5f 5f71 7561 6c6e 616d 655f  e__..__qualname_
-000004e0: 5fda 075f 5f64 6f63 5f5f 7225 0000 0072  _..__doc__r%...r
-000004f0: 2700 0000 7223 0000 0072 2300 0000 7223  '...r#...r#...r#
-00000500: 0000 0072 2400 0000 720c 0000 000e 0000  ...r$...r.......
-00000510: 0073 0800 0000 0800 0401 0802 0c12 720c  .s............r.
-00000520: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
-00000530: 0000 0000 0300 0000 4000 0000 7344 0000  ........@...sD..
-00000540: 0065 005a 0164 005a 0255 0065 0365 0464  .e.Z.d.Z.U.e.e.d
-00000550: 013c 0064 0264 0384 005a 0564 0d64 0564  .<.d.d...Z.d.d.d
-00000560: 0684 015a 0665 0764 0764 0884 0083 015a  ...Z.e.d.d.....Z
-00000570: 0864 0964 0a84 005a 0964 0b64 0c84 005a  .d.d...Z.d.d...Z
-00000580: 0a64 0453 0029 0eda 1046 696c 6547 656e  .d.S.)...FileGen
-00000590: 6572 6174 6f72 4142 43da 0872 656c 5f70  eratorABC..rel_p
-000005a0: 6174 6863 0200 0000 0000 0000 0000 0000  athc............
-000005b0: 0200 0000 0200 0000 4300 0000 7312 0000  ........C...s...
-000005c0: 007c 017c 005f 007c 016a 017c 005f 0164  .|.|._.|.j.|._.d
-000005d0: 0053 0072 2600 0000 2902 7213 0000 00da  .S.r&...).r.....
-000005e0: 0b69 6e70 7574 5f66 696c 6573 a902 7221  .input_files..r!
-000005f0: 0000 0072 1300 0000 7223 0000 0072 2300  ...r....r#...r#.
-00000600: 0000 7224 0000 0072 2500 0000 2a00 0000  ..r$...r%...*...
-00000610: 7304 0000 0006 010c 017a 1946 696c 6547  s........z.FileG
-00000620: 656e 6572 6174 6f72 4142 432e 5f5f 696e  eneratorABC.__in
-00000630: 6974 5f5f 4e63 0200 0000 0000 0000 0000  it__Nc..........
-00000640: 0000 0300 0000 0800 0000 4300 0000 735c  ..........C...s\
-00000650: 0000 007c 0164 0175 0072 097c 006a 006a  ...|.d.u.r.|.j.j
-00000660: 016a 027d 0174 037c 006a 006a 047c 006a  .j.}.t.|.j.j.|.j
-00000670: 051b 0064 0283 028f 117d 027c 02a0 067c  ...d.....}.|...|
-00000680: 00a0 077c 01a1 01a1 0101 0057 0064 0104  ...|.......W.d..
-00000690: 0004 0083 0301 0064 0153 0031 0073 2777  .......d.S.1.s'w
-000006a0: 0101 0001 0001 0059 0001 0064 0153 0029  .......Y...d.S.)
-000006b0: 037a 1147 656e 6572 6174 6520 7468 6520  .z.Generate the 
-000006c0: 6669 6c65 4eda 0177 2908 7213 0000 0072  fileN..w).r....r
-000006d0: 1500 0000 da06 7061 7261 6d73 da04 6f70  ......params..op
-000006e0: 656e da08 7061 7468 5f72 756e 722f 0000  en..path_runr/..
-000006f0: 00da 0577 7269 7465 da0d 6765 6e65 7261  ...write..genera
-00000700: 7465 5f63 6f64 6529 0372 2100 0000 7233  te_code).r!...r3
-00000710: 0000 00da 0466 696c 6572 2300 0000 7223  .....filer#...r#
-00000720: 0000 0072 2400 0000 da0d 6765 6e65 7261  ...r$.....genera
-00000730: 7465 5f66 696c 652e 0000 0073 0a00 0000  te_file....s....
-00000740: 0802 0a01 1601 1201 22ff 7a1e 4669 6c65  ........".z.File
-00000750: 4765 6e65 7261 746f 7241 4243 2e67 656e  GeneratorABC.gen
-00000760: 6572 6174 655f 6669 6c65 6301 0000 0000  erate_filec.....
-00000770: 0000 0000 0000 0001 0000 0001 0000 0043  ...............C
-00000780: 0000 0073 0400 0000 6401 5300 2902 7a1d  ...s....d.S.).z.
-00000790: 4765 6e65 7261 7465 2074 6865 2063 6f64  Generate the cod
-000007a0: 6520 6f66 2074 6865 2066 696c 654e 7223  e of the fileNr#
-000007b0: 0000 00a9 0172 2100 0000 7223 0000 0072  .....r!...r#...r
-000007c0: 2300 0000 7224 0000 0072 3700 0000 3500  #...r$...r7...5.
-000007d0: 0000 7302 0000 0004 007a 1e46 696c 6547  ..s......z.FileG
-000007e0: 656e 6572 6174 6f72 4142 432e 6765 6e65  eneratorABC.gene
-000007f0: 7261 7465 5f63 6f64 6563 0100 0000 0000  rate_codec......
-00000800: 0000 0000 0000 0300 0000 0400 0000 0300  ................
-00000810: 0000 7342 0000 0088 006a 006a 0188 006a  ..sB.....j.j...j
-00000820: 021b 007d 0174 0387 0066 0164 0164 0284  ...}.t...f.d.d..
-00000830: 0864 0344 0083 0183 0172 1d74 047c 01a0  .d.D.....r.t.|..
-00000840: 05a1 0083 017d 027c 017c 025f 067c 0253  .....}.|.|._.|.S
-00000850: 0074 077c 0183 0153 0029 044e 6301 0000  .t.|...S.).Nc...
-00000860: 0000 0000 0000 0000 0002 0000 0004 0000  ................
-00000870: 0033 0000 0073 1c00 0000 8100 7c00 5d09  .3...s......|.].
-00000880: 7d01 8800 6a00 a001 7c01 a101 5600 0100  }...j...|...V...
-00000890: 7102 6400 5300 7226 0000 0029 0272 2f00  q.d.S.r&...).r/.
-000008a0: 0000 da0a 7374 6172 7473 7769 7468 2902  ....startswith).
-000008b0: da02 2e30 da05 7374 6172 7472 3a00 0000  ...0..startr:...
-000008c0: 7223 0000 0072 2400 0000 da09 3c67 656e  r#...r$.....<gen
-000008d0: 6578 7072 3e3b 0000 0073 0800 0000 0280  expr>;...s......
-000008e0: 0400 0c01 0aff 7a28 4669 6c65 4765 6e65  ......z(FileGene
-000008f0: 7261 746f 7241 4243 2e72 6561 642e 3c6c  ratorABC.read.<l
-00000900: 6f63 616c 733e 2e3c 6765 6e65 7870 723e  ocals>.<genexpr>
-00000910: 2902 da06 7379 7374 656d da08 636f 6e73  )...system..cons
-00000920: 7461 6e74 2908 7213 0000 0072 3500 0000  tant).r....r5...
-00000930: 722f 0000 00da 0361 6e79 720a 0000 00da  r/.....anyr.....
-00000940: 0972 6561 645f 7465 7874 da04 7061 7468  .read_text..path
-00000950: 720b 0000 0029 0372 2100 0000 7243 0000  r....).r!...rC..
-00000960: 00da 0474 7265 6572 2300 0000 723a 0000  ...treer#...r:..
-00000970: 0072 2400 0000 da04 7265 6164 3900 0000  .r$.....read9...
-00000980: 7310 0000 000e 010c 0102 0108 ff0c 0306  s...............
-00000990: 0104 0108 027a 1546 696c 6547 656e 6572  .....z.FileGener
-000009a0: 6174 6f72 4142 432e 7265 6164 6302 0000  atorABC.readc...
-000009b0: 0000 0000 0000 0000 0003 0000 0008 0000  ................
-000009c0: 0043 0000 0073 4800 0000 7400 7c00 6a01  .C...sH...t.|.j.
-000009d0: 6a02 7c00 6a03 1b00 6401 8302 8f10 7d02  j.|.j...d.....}.
-000009e0: 7c02 a004 7c01 a005 a100 a101 0100 5700  |...|.........W.
-000009f0: 6400 0400 0400 8303 0100 6400 5300 3100  d.........d.S.1.
-00000a00: 731d 7701 0100 0100 0100 5900 0100 6400  s.w.......Y...d.
-00000a10: 5300 2902 4e72 3200 0000 2906 7234 0000  S.).Nr2...).r4..
-00000a20: 0072 1300 0000 7235 0000 0072 2f00 0000  .r....r5...r/...
-00000a30: 7236 0000 00da 0464 756d 7029 0372 2100  r6.....dump).r!.
-00000a40: 0000 5a08 6475 6d70 6162 6c65 7238 0000  ..Z.dumpabler8..
-00000a50: 0072 2300 0000 7223 0000 0072 2400 0000  .r#...r#...r$...
-00000a60: da09 6f76 6572 7772 6974 6544 0000 0073  ..overwriteD...s
-00000a70: 0600 0000 1601 1001 22ff 7a1a 4669 6c65  ........".z.File
-00000a80: 4765 6e65 7261 746f 7241 4243 2e6f 7665  GeneratorABC.ove
-00000a90: 7277 7269 7465 7226 0000 0029 0b72 2a00  rwriter&...).r*.
-00000aa0: 0000 722b 0000 0072 2c00 0000 da03 7374  ..r+...r,.....st
-00000ab0: 72da 0f5f 5f61 6e6e 6f74 6174 696f 6e73  r..__annotations
-00000ac0: 5f5f 7225 0000 0072 3900 0000 7203 0000  __r%...r9...r...
-00000ad0: 0072 3700 0000 7245 0000 0072 4700 0000  .r7...rE...rG...
-00000ae0: 7223 0000 0072 2300 0000 7223 0000 0072  r#...r#...r#...r
-00000af0: 2400 0000 722e 0000 0027 0000 0073 1000  $...r....'...s..
-00000b00: 0000 0a00 0801 0802 0a04 0207 0a01 0803  ................
-00000b10: 0c0b 722e 0000 0063 0000 0000 0000 0000  ..r....c........
-00000b20: 0000 0000 0000 0000 0300 0000 0000 0000  ................
-00000b30: 733c 0000 0065 005a 0164 005a 0255 0065  s<...e.Z.d.Z.U.e
-00000b40: 0365 0464 013c 0087 0066 0164 0264 0384  .e.d.<...f.d.d..
-00000b50: 085a 0564 0964 0564 0684 015a 0665 0764  .Z.d.d.d...Z.e.d
-00000b60: 0764 0884 0083 015a 0887 0004 005a 0953  .d.....Z.....Z.S
-00000b70: 0029 0ada 0d46 696c 6547 656e 6572 6174  .)...FileGenerat
-00000b80: 6f72 7228 0000 0063 0200 0000 0000 0000  orr(...c........
-00000b90: 0000 0000 0200 0000 0300 0000 0300 0000  ................
-00000ba0: 7310 0000 0074 0083 00a0 017c 01a1 0101  s....t.....|....
-00000bb0: 0064 0053 0072 2600 0000 2902 da05 7375  .d.S.r&...)...su
-00000bc0: 7065 7272 2500 0000 7231 0000 00a9 01da  perr%...r1......
-00000bd0: 095f 5f63 6c61 7373 5f5f 7223 0000 0072  .__class__r#...r
-00000be0: 2400 0000 7225 0000 004c 0000 0073 0200  $...r%...L...s..
-00000bf0: 0000 1001 7a16 4669 6c65 4765 6e65 7261  ....z.FileGenera
-00000c00: 746f 722e 5f5f 696e 6974 5f5f 4e63 0200  tor.__init__Nc..
-00000c10: 0000 0000 0000 0000 0000 0500 0000 0800  ................
-00000c20: 0000 0300 0000 732c 0100 007c 0164 0175  ......s,...|.d.u
-00000c30: 0072 097c 006a 006a 016a 027d 017a 0b74  .r.|.j.j.j.}.z.t
-00000c40: 037c 006a 0064 027c 006a 0417 0083 027d  .|.j.d.|.j.....}
-00000c50: 0257 006e 0b04 0074 0579 1f01 0001 0001  .W.n...t.y......
-00000c60: 0064 017d 0259 006e 0177 007c 0264 0175  .d.}.Y.n.w.|.d.u
-00000c70: 0072 667a 0b74 037c 006a 0064 037c 006a  .rfz.t.|.j.d.|.j
-00000c80: 0417 0083 0289 0057 006e 0b04 0074 0579  .......W.n...t.y
-00000c90: 3a01 0001 0001 0064 0189 0059 006e 0177  :......d...Y.n.w
-00000ca0: 0088 0064 0175 0072 5c7a 0b74 037c 006a  ...d.u.r\z.t.|.j
-00000cb0: 0064 047c 006a 0417 0083 027d 0357 006e  .d.|.j.....}.W.n
-00000cc0: 0904 0074 0579 5301 0001 0001 0059 006e  ...t.yS......Y.n
-00000cd0: 0977 0074 067c 0374 0783 0272 5c7c 036a  .w.t.|.t...r\|.j
-00000ce0: 0889 0088 0064 0175 0172 6687 0066 0164  .....d.u.rf..f.d
-00000cf0: 0564 0684 087d 027c 0264 0175 0072 777c  .d...}.|.d.u.rw|
-00000d00: 006a 09a0 0a7c 006a 0ba1 017d 047c 046a  .j...|.j...}.|.j
-00000d10: 0c7c 0164 078d 0153 007c 006a 096a 0d7c  .|.d...S.|.j.j.|
-00000d20: 006a 0b1b 00a0 0ea1 0072 9274 0f64 087c  .j.......r.t.d.|
-00000d30: 006a 109b 0064 097c 006a 096a 0d9b 0064  .j...d.|.j.j...d
-00000d40: 0a7c 006a 049b 0064 0b9d 0783 0182 017c  .|.j...d.......|
-00000d50: 027c 0183 0153 0029 0c7a 9547 656e 6572  .|...S.).z.Gener
-00000d60: 6174 6520 7468 6520 636f 6465 206f 6620  ate the code of 
-00000d70: 7468 6520 6669 6c65 2066 726f 6d20 2e2e  the file from ..
-00000d80: 2e0a 0a20 2020 2020 2020 202d 2061 206d  ...        - a m
-00000d90: 6574 686f 6420 6e61 6d65 6420 6c69 6b65  ethod named like
-00000da0: 2060 7369 6d2e 6f75 7470 7574 2e6d 616b   `sim.output.mak
-00000db0: 655f 636f 6465 5f62 6c6f 636b 5f6d 6573  e_code_block_mes
-00000dc0: 685f 6469 6374 602c 0a20 2020 2020 2020  h_dict`,.       
-00000dd0: 202d 206f 7220 6120 4a69 6e6a 6120 7465   - or a Jinja te
-00000de0: 6d70 6c61 7465 2e0a 2020 2020 2020 2020  mplate..        
-00000df0: 4e5a 0a6d 616b 655f 636f 6465 5f5a 0a6d  NZ.make_code_Z.m
-00000e00: 616b 655f 7472 6565 5fda 0768 656c 7065  ake_tree_..helpe
-00000e10: 725f 6301 0000 0000 0000 0000 0000 0001  r_c.............
-00000e20: 0000 0002 0000 0013 0000 0073 0c00 0000  ...........s....
-00000e30: 8800 7c00 8301 a000 a100 5300 7226 0000  ..|.......S.r&..
-00000e40: 0029 0172 4600 0000 2901 5a07 7061 7261  .).rF...).Z.para
-00000e50: 6d73 5fa9 01da 096d 616b 655f 7472 6565  ms_....make_tree
-00000e60: 7223 0000 0072 2400 0000 da09 6d61 6b65  r#...r$.....make
-00000e70: 5f63 6f64 656e 0000 0072 2900 0000 7a2e  _coden...r)...z.
-00000e80: 4669 6c65 4765 6e65 7261 746f 722e 6765  FileGenerator.ge
-00000e90: 6e65 7261 7465 5f63 6f64 652e 3c6c 6f63  nerate_code.<loc
-00000ea0: 616c 733e 2e6d 616b 655f 636f 6465 2901  als>.make_code).
-00000eb0: 7233 0000 007a 3b46 6c75 6964 7369 6d66  r3...z;Fluidsimf
-00000ec0: 6f61 6d20 736f 6c76 6572 2069 7373 7565  oam solver issue
-00000ed0: 3a20 3220 636f 6e63 7572 7265 6e74 206d  : 2 concurrent m
-00000ee0: 6574 686f 6473 2074 6f20 7072 6f64 7563  ethods to produc
-00000ef0: 6520 7a10 3a0a 2d20 7465 6d70 6c61 7465  e z.:.- template
-00000f00: 2069 6e20 7a1e 2c0a 2d20 6675 6e63 7469   in z.,.- functi
-00000f10: 6f6e 206f 7574 7075 742e 6d61 6b65 5f63  on output.make_c
-00000f20: 6f64 655f 7a3d 2e0a 5265 6d6f 7665 2074  ode_z=..Remove t
-00000f30: 6865 2066 696c 6520 6f72 2074 6865 2066  he file or the f
-00000f40: 756e 6374 696f 6e20 286f 7220 6d61 6b65  unction (or make
-00000f50: 2069 7420 6571 7561 6c20 746f 204e 6f6e   it equal to Non
-00000f60: 6529 2e29 1172 1300 0000 7215 0000 0072  e).).r....r....r
-00000f70: 3300 0000 da07 6765 7461 7474 72da 055f  3.....getattr.._
-00000f80: 6e61 6d65 da0e 4174 7472 6962 7574 6545  name..AttributeE
-00000f90: 7272 6f72 da0a 6973 696e 7374 616e 6365  rror..isinstance
-00000fa0: 7209 0000 0072 5000 0000 7230 0000 0072  r....rP...r0...r
-00000fb0: 2700 0000 7228 0000 00da 0672 656e 6465  '...r(.....rende
-00000fc0: 7272 1900 0000 da06 6578 6973 7473 da0c  rr......exists..
-00000fd0: 5275 6e74 696d 6545 7272 6f72 722f 0000  RuntimeErrorr/..
-00000fe0: 0029 0572 2100 0000 7233 0000 0072 5100  .).r!...r3...rQ.
-00000ff0: 0000 da06 6865 6c70 6572 da08 7465 6d70  ....helper..temp
-00001000: 6c61 7465 7223 0000 0072 4f00 0000 7224  later#...rO...r$
-00001010: 0000 0072 3700 0000 4f00 0000 734a 0000  ...r7...O...sJ..
-00001020: 0008 060a 0102 0216 010c 0108 0102 ff08  ................
-00001030: 0302 0116 010c 0108 0102 ff08 0302 0116  ................
-00001040: 010c 0104 0102 ff0a 0306 0108 020c 0208  ................
-00001050: 030e 010c 0112 0202 0102 0104 0104 ff06  ................
-00001060: 0204 fe04 0306 fd04 ff08 087a 1b46 696c  ...........z.Fil
-00001070: 6547 656e 6572 6174 6f72 2e67 656e 6572  eGenerator.gener
-00001080: 6174 655f 636f 6465 6303 0000 0000 0000  ate_codec.......
-00001090: 0000 0000 0006 0000 0008 0000 0043 0000  .............C..
-000010a0: 0073 9a00 0000 7400 7c02 6a01 6a02 6a03  .s....t.|.j.j.j.
-000010b0: 7c02 6a01 6a02 6a04 8302 7d03 7a0a 7405  |.j.j.j...}.z.t.
-000010c0: 7c03 6401 7c00 6a06 1700 8302 7d04 5700  |.d.|.j.....}.W.
-000010d0: 6e0b 0400 7407 7920 0100 0100 0100 6400  n...t.y ......d.
-000010e0: 7d04 5900 6e01 7700 7c04 6400 7500 7241  }.Y.n.w.|.d.u.rA
-000010f0: 7a0a 7405 7c03 6402 7c00 6a06 1700 8302  z.t.|.d.|.j.....
-00001100: 7d05 5700 6e09 0400 7407 7938 0100 0100  }.W.n...t.y8....
-00001110: 0100 5900 6e09 7700 7408 7c05 7409 8302  ..Y.n.w.t.|.t...
-00001120: 7241 7c05 6a0a 7d04 7c04 6400 7501 724b  rA|.j.}.|.d.u.rK
-00001130: 7c04 7c01 8301 0100 6400 5300 6400 5300  |.|.....d.S.d.S.
-00001140: 2903 4e5a 115f 636f 6d70 6c65 7465 5f70  ).NZ._complete_p
-00001150: 6172 616d 735f 724e 0000 0029 0b72 0800  arams_rN...).r..
-00001160: 0000 da07 636c 6173 7365 73da 064f 7574  ....classes..Out
-00001170: 7075 74da 0b6d 6f64 756c 655f 6e61 6d65  put..module_name
-00001180: da0a 636c 6173 735f 6e61 6d65 7252 0000  ..class_namerR..
-00001190: 0072 5300 0000 7254 0000 0072 5500 0000  .rS...rT...rU...
-000011a0: 7209 0000 00da 0f63 6f6d 706c 6574 655f  r......complete_
-000011b0: 7061 7261 6d73 2906 da03 636c 7372 3300  params)...clsr3.
-000011c0: 0000 da0b 696e 666f 5f73 6f6c 7665 725a  ....info_solverZ
-000011d0: 0a6f 7574 7075 745f 636c 7372 5f00 0000  .output_clsr_...
-000011e0: 7259 0000 0072 2300 0000 7223 0000 0072  rY...r#...r#...r
-000011f0: 2400 0000 da1d 5f63 6f6d 706c 6574 655f  $....._complete_
-00001200: 7061 7261 6d73 5f77 6974 685f 6465 6661  params_with_defa
-00001210: 756c 7480 0000 0073 2800 0000 0202 0801  ult....s(.......
-00001220: 0801 04fe 0204 1401 0c01 0801 02ff 0803  ................
-00001230: 0201 1401 0c01 0401 02ff 0a03 0601 0802  ................
-00001240: 0c01 04ff 7a2b 4669 6c65 4765 6e65 7261  ....z+FileGenera
-00001250: 746f 722e 5f63 6f6d 706c 6574 655f 7061  tor._complete_pa
-00001260: 7261 6d73 5f77 6974 685f 6465 6661 756c  rams_with_defaul
-00001270: 7472 2600 0000 290a 722a 0000 0072 2b00  tr&...).r*...r+.
-00001280: 0000 722c 0000 0072 4800 0000 7249 0000  ..r,...rH...rI..
-00001290: 0072 2500 0000 7237 0000 00da 0b63 6c61  .r%...r7.....cla
-000012a0: 7373 6d65 7468 6f64 7262 0000 00da 0d5f  ssmethodrb....._
-000012b0: 5f63 6c61 7373 6365 6c6c 5f5f 7223 0000  _classcell__r#..
-000012c0: 0072 2300 0000 724c 0000 0072 2400 0000  .r#...rL...r$...
-000012d0: 724a 0000 0049 0000 0073 0c00 0000 0a00  rJ...I...s......
-000012e0: 0801 0c02 0a03 0231 1201 724a 0000 00da  .......1..rJ....
-000012f0: 0130 6302 0000 0000 0000 0000 0000 0003  .0c.............
-00001300: 0000 000b 0000 0043 0000 0073 4200 0000  .......C...sB...
-00001310: 6401 7400 7c00 8301 9b00 9d02 7d02 7401  d.t.|.......}.t.
-00001320: 7c02 7402 6601 7c01 7c01 9b00 6402 7c00  |.t.f.|.|...d.|.
-00001330: 9b00 9d03 7c00 9b00 6403 9d02 7403 7c00  ....|...d...t.|.
-00001340: a004 6404 6405 a102 8301 6406 9c04 8303  ..d.d.....d.....
-00001350: 5300 2907 4e72 4a00 0000 fa01 2f7a 062e  S.).NrJ...../z..
-00001360: 6a69 6e6a 61da 012e da01 5f29 04da 0864  jinja....._)...d
-00001370: 6972 5f6e 616d 6572 2f00 0000 7228 0000  ir_namer/...r(..
-00001380: 0072 5300 0000 2905 7206 0000 0072 1400  .rS...).r....r..
-00001390: 0000 724a 0000 0072 0700 0000 da07 7265  ..rJ...r......re
-000013a0: 706c 6163 6529 03da 0966 696c 655f 6e61  place)...file_na
-000013b0: 6d65 7269 0000 00da 0863 6c73 5f6e 616d  meri.....cls_nam
-000013c0: 6572 2300 0000 7223 0000 0072 2400 0000  er#...r#...r$...
-000013d0: da18 6e65 775f 6669 6c65 5f67 656e 6572  ..new_file_gener
-000013e0: 6174 6f72 5f63 6c61 7373 9800 0000 7314  ator_class....s.
-000013f0: 0000 000e 0102 0102 0104 0102 020c 0108  ................
-00001400: 010e 0104 fc04 fd72 6d00 0000 2901 7265  .......rm...).re
-00001410: 0000 0029 1672 2d00 0000 da03 6162 6372  ...).r-.....abcr
-00001420: 0200 0000 7203 0000 00da 0769 6e73 7065  ....r......inspe
-00001430: 6374 7204 0000 00da 0770 6174 686c 6962  ctr......pathlib
-00001440: 7205 0000 0072 1a00 0000 da0a 696e 666c  r....r......infl
-00001450: 6563 7469 6f6e 7206 0000 0072 0700 0000  ectionr....r....
-00001460: da0d 666c 7569 6464 796e 2e75 7469 6c72  ..fluiddyn.utilr
-00001470: 0800 0000 da1d 666c 7569 6473 696d 666f  ......fluidsimfo
-00001480: 616d 2e66 6f61 6d5f 696e 7075 745f 6669  am.foam_input_fi
-00001490: 6c65 7372 0900 0000 720a 0000 0072 0b00  lesr....r....r..
-000014a0: 0000 720c 0000 0072 2e00 0000 724a 0000  ..r....r....rJ..
-000014b0: 0072 6d00 0000 7223 0000 0072 2300 0000  .rm...r#...r#...
-000014c0: 7223 0000 0072 2400 0000 da08 3c6d 6f64  r#...r$.....<mod
-000014d0: 756c 653e 0100 0000 7318 0000 0004 0010  ule>....s.......
-000014e0: 020c 010c 0108 0210 010c 0214 010e 0310  ................
-000014f0: 1910 220e 4f                             ..".O
+00000370: 6e76 2904 da04 7365 6c66 7210 0000 00da  nv)...selfr.....
+00000380: 036d 6f64 720e 0000 00a9 0072 1c00 0000  .modr......r....
+00000390: fa4d 2f68 6f6d 652f 7069 6572 7265 2f44  .M/home/pierre/D
+000003a0: 6576 2f66 6c75 6964 7369 6d66 6f61 6d2f  ev/fluidsimfoam/
+000003b0: 7372 632f 666c 7569 6473 696d 666f 616d  src/fluidsimfoam
+000003c0: 2f66 6f61 6d5f 696e 7075 745f 6669 6c65  /foam_input_file
+000003d0: 732f 6765 6e65 7261 746f 7273 2e70 79da  s/generators.py.
+000003e0: 085f 5f69 6e69 745f 5f11 0000 0073 1a00  .__init__....s..
+000003f0: 0000 0601 0e01 1601 0402 0c02 0a01 02fe  ................
+00000400: 04ff 0407 0201 0401 0201 0cfd 7a13 496e  ............z.In
+00000410: 7075 7446 696c 6573 2e5f 5f69 6e69 745f  putFiles.__init_
+00000420: 5f63 0200 0000 0000 0000 0000 0000 0200  _c..............
+00000430: 0000 0300 0000 4300 0000 730c 0000 007c  ......C...s....|
+00000440: 006a 00a0 017c 01a1 0153 00a9 014e 2902  .j...|...S...N).
+00000450: 7219 0000 00da 0c67 6574 5f74 656d 706c  r......get_templ
+00000460: 6174 6529 0272 1a00 0000 da0d 7465 6d70  ate).r......temp
+00000470: 6c61 7465 5f6e 616d 6572 1c00 0000 721c  late_namer....r.
+00000480: 0000 0072 1d00 0000 7220 0000 0023 0000  ...r....r ...#..
+00000490: 0073 0200 0000 0c01 7a17 496e 7075 7446  .s......z.InputF
+000004a0: 696c 6573 2e67 6574 5f74 656d 706c 6174  iles.get_templat
+000004b0: 654e 2906 da08 5f5f 6e61 6d65 5f5f da0a  eN)...__name__..
+000004c0: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
+000004d0: 616c 6e61 6d65 5f5f da07 5f5f 646f 635f  alname__..__doc_
+000004e0: 5f72 1e00 0000 7220 0000 0072 1c00 0000  _r....r ...r....
+000004f0: 721c 0000 0072 1c00 0000 721d 0000 0072  r....r....r....r
+00000500: 0c00 0000 0e00 0000 7308 0000 0008 0004  ........s.......
+00000510: 0108 020c 1272 0c00 0000 6300 0000 0000  .....r....c.....
+00000520: 0000 0000 0000 0000 0000 0003 0000 0040  ...............@
+00000530: 0000 0073 4400 0000 6500 5a01 6400 5a02  ...sD...e.Z.d.Z.
+00000540: 5500 6503 6504 6401 3c00 6402 6403 8400  U.e.e.d.<.d.d...
+00000550: 5a05 640d 6405 6406 8401 5a06 6507 6407  Z.d.d.d...Z.e.d.
+00000560: 6408 8400 8301 5a08 6409 640a 8400 5a09  d.....Z.d.d...Z.
+00000570: 640b 640c 8400 5a0a 6404 5300 290e da10  d.d...Z.d.S.)...
+00000580: 4669 6c65 4765 6e65 7261 746f 7241 4243  FileGeneratorABC
+00000590: da08 7265 6c5f 7061 7468 6302 0000 0000  ..rel_pathc.....
+000005a0: 0000 0000 0000 0002 0000 0002 0000 0043  ...............C
+000005b0: 0000 0073 1200 0000 7c01 7c00 5f00 7c01  ...s....|.|._.|.
+000005c0: 6a01 7c00 5f01 6400 5300 721f 0000 0029  j.|._.d.S.r....)
+000005d0: 0272 1000 0000 da0b 696e 7075 745f 6669  .r......input_fi
+000005e0: 6c65 73a9 0272 1a00 0000 7210 0000 0072  les..r....r....r
+000005f0: 1c00 0000 721c 0000 0072 1d00 0000 721e  ....r....r....r.
+00000600: 0000 002a 0000 0073 0400 0000 0601 0c01  ...*...s........
+00000610: 7a19 4669 6c65 4765 6e65 7261 746f 7241  z.FileGeneratorA
+00000620: 4243 2e5f 5f69 6e69 745f 5f4e 6302 0000  BC.__init__Nc...
+00000630: 0000 0000 0000 0000 0004 0000 0008 0000  ................
+00000640: 0043 0000 0073 6c00 0000 7c01 6401 7500  .C...sl...|.d.u.
+00000650: 7209 7c00 6a00 6a01 6a02 7d01 7c00 a003  r.|.j.j.j.}.|...
+00000660: 7c01 a101 7d02 7c02 6402 7500 7214 6401  |...}.|.d.u.r.d.
+00000670: 5300 7404 7c00 6a00 6a05 7c00 6a06 1b00  S.t.|.j.j.|.j...
+00000680: 6403 8302 8f0e 7d03 7c03 a007 7c02 a101  d.....}.|...|...
+00000690: 0100 5700 6401 0400 0400 8303 0100 6401  ..W.d.........d.
+000006a0: 5300 3100 732f 7701 0100 0100 0100 5900  S.1.s/w.......Y.
+000006b0: 0100 6401 5300 2904 7a11 4765 6e65 7261  ..d.S.).z.Genera
+000006c0: 7465 2074 6865 2066 696c 654e 46da 0177  te the fileNF..w
+000006d0: 2908 7210 0000 0072 1200 0000 da06 7061  ).r....r......pa
+000006e0: 7261 6d73 da0d 6765 6e65 7261 7465 5f63  rams..generate_c
+000006f0: 6f64 65da 046f 7065 6eda 0870 6174 685f  ode..open..path_
+00000700: 7275 6e72 2700 0000 da05 7772 6974 6529  runr'.....write)
+00000710: 0472 1a00 0000 722b 0000 00da 0463 6f64  .r....r+.....cod
+00000720: 65da 0466 696c 6572 1c00 0000 721c 0000  e..filer....r...
+00000730: 0072 1d00 0000 da0d 6765 6e65 7261 7465  .r......generate
+00000740: 5f66 696c 652e 0000 0073 1000 0000 0802  _file....s......
+00000750: 0a01 0a02 0801 0401 1602 0c01 22ff 7a1e  ............".z.
+00000760: 4669 6c65 4765 6e65 7261 746f 7241 4243  FileGeneratorABC
+00000770: 2e67 656e 6572 6174 655f 6669 6c65 6301  .generate_filec.
+00000780: 0000 0000 0000 0000 0000 0001 0000 0001  ................
+00000790: 0000 0043 0000 0073 0400 0000 6401 5300  ...C...s....d.S.
+000007a0: 2902 7a1d 4765 6e65 7261 7465 2074 6865  ).z.Generate the
+000007b0: 2063 6f64 6520 6f66 2074 6865 2066 696c   code of the fil
+000007c0: 654e 721c 0000 00a9 0172 1a00 0000 721c  eNr......r....r.
+000007d0: 0000 0072 1c00 0000 721d 0000 0072 2c00  ...r....r....r,.
+000007e0: 0000 3a00 0000 7302 0000 0004 007a 1e46  ..:...s......z.F
+000007f0: 696c 6547 656e 6572 6174 6f72 4142 432e  ileGeneratorABC.
+00000800: 6765 6e65 7261 7465 5f63 6f64 6563 0100  generate_codec..
+00000810: 0000 0000 0000 0000 0000 0300 0000 0400  ................
+00000820: 0000 0300 0000 7342 0000 0088 006a 006a  ......sB.....j.j
+00000830: 0188 006a 021b 007d 0174 0387 0066 0164  ...j...}.t...f.d
+00000840: 0164 0284 0864 0344 0083 0183 0172 1d74  .d...d.D.....r.t
+00000850: 047c 01a0 05a1 0083 017d 027c 017c 025f  .|.......}.|.|._
+00000860: 067c 0253 0074 077c 0183 0153 0029 044e  .|.S.t.|...S.).N
+00000870: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
+00000880: 0004 0000 0033 0000 0073 1c00 0000 8100  .....3...s......
+00000890: 7c00 5d09 7d01 8800 6a00 a001 7c01 a101  |.].}...j...|...
+000008a0: 5600 0100 7102 6400 5300 721f 0000 0029  V...q.d.S.r....)
+000008b0: 0272 2700 0000 da0a 7374 6172 7473 7769  .r'.....startswi
+000008c0: 7468 2902 da02 2e30 da05 7374 6172 7472  th)....0..startr
+000008d0: 3300 0000 721c 0000 0072 1d00 0000 da09  3...r....r......
+000008e0: 3c67 656e 6578 7072 3e40 0000 0073 0800  <genexpr>@...s..
+000008f0: 0000 0280 0400 0c01 0aff 7a28 4669 6c65  ..........z(File
+00000900: 4765 6e65 7261 746f 7241 4243 2e72 6561  GeneratorABC.rea
+00000910: 642e 3c6c 6f63 616c 733e 2e3c 6765 6e65  d.<locals>.<gene
+00000920: 7870 723e 2902 da06 7379 7374 656d da08  xpr>)...system..
+00000930: 636f 6e73 7461 6e74 2908 7210 0000 0072  constant).r....r
+00000940: 2e00 0000 7227 0000 00da 0361 6e79 720a  ....r'.....anyr.
+00000950: 0000 00da 0972 6561 645f 7465 7874 da04  .....read_text..
+00000960: 7061 7468 720b 0000 0029 0372 1a00 0000  pathr....).r....
+00000970: 723c 0000 00da 0474 7265 6572 1c00 0000  r<.....treer....
+00000980: 7233 0000 0072 1d00 0000 da04 7265 6164  r3...r......read
+00000990: 3e00 0000 7310 0000 000e 010c 0102 0108  >...s...........
+000009a0: ff0c 0306 0104 0108 027a 1546 696c 6547  .........z.FileG
+000009b0: 656e 6572 6174 6f72 4142 432e 7265 6164  eneratorABC.read
+000009c0: 6302 0000 0000 0000 0000 0000 0003 0000  c...............
+000009d0: 0008 0000 0043 0000 0073 4800 0000 7400  .....C...sH...t.
+000009e0: 7c00 6a01 6a02 7c00 6a03 1b00 6401 8302  |.j.j.|.j...d...
+000009f0: 8f10 7d02 7c02 a004 7c01 a005 a100 a101  ..}.|...|.......
+00000a00: 0100 5700 6400 0400 0400 8303 0100 6400  ..W.d.........d.
+00000a10: 5300 3100 731d 7701 0100 0100 0100 5900  S.1.s.w.......Y.
+00000a20: 0100 6400 5300 2902 4e72 2a00 0000 2906  ..d.S.).Nr*...).
+00000a30: 722d 0000 0072 1000 0000 722e 0000 0072  r-...r....r....r
+00000a40: 2700 0000 722f 0000 00da 0464 756d 7029  '...r/.....dump)
+00000a50: 0372 1a00 0000 5a08 6475 6d70 6162 6c65  .r....Z.dumpable
+00000a60: 7231 0000 0072 1c00 0000 721c 0000 0072  r1...r....r....r
+00000a70: 1d00 0000 da09 6f76 6572 7772 6974 6549  ......overwriteI
+00000a80: 0000 0073 0600 0000 1601 1001 22ff 7a1a  ...s........".z.
+00000a90: 4669 6c65 4765 6e65 7261 746f 7241 4243  FileGeneratorABC
+00000aa0: 2e6f 7665 7277 7269 7465 721f 0000 0029  .overwriter....)
+00000ab0: 0b72 2200 0000 7223 0000 0072 2400 0000  .r"...r#...r$...
+00000ac0: da03 7374 72da 0f5f 5f61 6e6e 6f74 6174  ..str..__annotat
+00000ad0: 696f 6e73 5f5f 721e 0000 0072 3200 0000  ions__r....r2...
+00000ae0: 7203 0000 0072 2c00 0000 723e 0000 0072  r....r,...r>...r
+00000af0: 4000 0000 721c 0000 0072 1c00 0000 721c  @...r....r....r.
+00000b00: 0000 0072 1d00 0000 7226 0000 0027 0000  ...r....r&...'..
+00000b10: 0073 1000 0000 0a00 0801 0802 0a04 020c  .s..............
+00000b20: 0a01 0803 0c0b 7226 0000 0063 0000 0000  ......r&...c....
+00000b30: 0000 0000 0000 0000 0000 0000 0300 0000  ................
+00000b40: 0000 0000 733c 0000 0065 005a 0164 005a  ....s<...e.Z.d.Z
+00000b50: 0255 0065 0365 0464 013c 0087 0066 0164  .U.e.e.d.<...f.d
+00000b60: 0264 0384 085a 0564 0964 0564 0684 015a  .d...Z.d.d.d...Z
+00000b70: 0665 0764 0764 0884 0083 015a 0887 0004  .e.d.d.....Z....
+00000b80: 005a 0953 0029 0ada 0d46 696c 6547 656e  .Z.S.)...FileGen
+00000b90: 6572 6174 6f72 7221 0000 0063 0200 0000  eratorr!...c....
+00000ba0: 0000 0000 0000 0000 0200 0000 0300 0000  ................
+00000bb0: 0300 0000 7310 0000 0074 0083 00a0 017c  ....s....t.....|
+00000bc0: 01a1 0101 0064 0053 0072 1f00 0000 2902  .....d.S.r....).
+00000bd0: da05 7375 7065 7272 1e00 0000 7229 0000  ..superr....r)..
+00000be0: 00a9 01da 095f 5f63 6c61 7373 5f5f 721c  .....__class__r.
+00000bf0: 0000 0072 1d00 0000 721e 0000 0051 0000  ...r....r....Q..
+00000c00: 0073 0200 0000 1001 7a16 4669 6c65 4765  .s......z.FileGe
+00000c10: 6e65 7261 746f 722e 5f5f 696e 6974 5f5f  nerator.__init__
+00000c20: 4e63 0200 0000 0000 0000 0000 0000 0500  Nc..............
+00000c30: 0000 0800 0000 0300 0000 732c 0100 007c  ..........s,...|
+00000c40: 0164 0175 0072 097c 006a 006a 016a 027d  .d.u.r.|.j.j.j.}
+00000c50: 017a 0b74 037c 006a 0064 027c 006a 0417  .z.t.|.j.d.|.j..
+00000c60: 0083 027d 0257 006e 0b04 0074 0579 1f01  ...}.W.n...t.y..
+00000c70: 0001 0001 0064 017d 0259 006e 0177 007c  .....d.}.Y.n.w.|
+00000c80: 0264 0175 0072 667a 0b74 037c 006a 0064  .d.u.rfz.t.|.j.d
+00000c90: 037c 006a 0417 0083 0289 0057 006e 0b04  .|.j.......W.n..
+00000ca0: 0074 0579 3a01 0001 0001 0064 0189 0059  .t.y:......d...Y
+00000cb0: 006e 0177 0088 0064 0175 0072 5c7a 0b74  .n.w...d.u.r\z.t
+00000cc0: 037c 006a 0064 047c 006a 0417 0083 027d  .|.j.d.|.j.....}
+00000cd0: 0357 006e 0904 0074 0579 5301 0001 0001  .W.n...t.yS.....
+00000ce0: 0059 006e 0977 0074 067c 0374 0783 0272  .Y.n.w.t.|.t...r
+00000cf0: 5c7c 036a 0889 0088 0064 0175 0172 6687  \|.j.....d.u.rf.
+00000d00: 0066 0164 0564 0684 087d 027c 0264 0175  .f.d.d...}.|.d.u
+00000d10: 0072 777c 006a 09a0 0a7c 006a 0ba1 017d  .rw|.j...|.j...}
+00000d20: 047c 046a 0c7c 0164 078d 0153 007c 006a  .|.j.|.d...S.|.j
+00000d30: 096a 0d7c 006a 0b1b 00a0 0ea1 0072 9274  .j.|.j.......r.t
+00000d40: 0f64 087c 006a 109b 0064 097c 006a 096a  .d.|.j...d.|.j.j
+00000d50: 0d9b 0064 0a7c 006a 049b 0064 0b9d 0783  ...d.|.j...d....
+00000d60: 0182 017c 027c 0183 0153 0029 0c7a 9647  ...|.|...S.).z.G
+00000d70: 656e 6572 6174 6520 7468 6520 636f 6465  enerate the code
+00000d80: 206f 6620 7468 6520 6669 6c65 2066 726f   of the file fro
+00000d90: 6d20 2e2e 2e0a 0a20 2020 2020 2020 202d  m .....        -
+00000da0: 2061 206d 6574 686f 6420 6e61 6d65 6420   a method named 
+00000db0: 6c69 6b65 2060 7369 6d2e 6f75 7470 7574  like `sim.output
+00000dc0: 2e5f 6d61 6b65 5f63 6f64 655f 626c 6f63  ._make_code_bloc
+00000dd0: 6b5f 6d65 7368 5f64 6963 7460 2c0a 2020  k_mesh_dict`,.  
+00000de0: 2020 2020 2020 2d20 6f72 2061 204a 696e        - or a Jin
+00000df0: 6a61 2074 656d 706c 6174 652e 0a20 2020  ja template..   
+00000e00: 2020 2020 204e 5a0b 5f6d 616b 655f 636f       NZ._make_co
+00000e10: 6465 5f5a 0b5f 6d61 6b65 5f74 7265 655f  de_Z._make_tree_
+00000e20: da08 5f68 656c 7065 725f 6301 0000 0000  .._helper_c.....
+00000e30: 0000 0000 0000 0002 0000 0002 0000 0013  ................
+00000e40: 0000 0073 1c00 0000 8800 7c00 8301 7d01  ...s......|...}.
+00000e50: 7c01 6401 7500 720a 6401 5300 7c01 a000  |.d.u.r.d.S.|...
+00000e60: a100 5300 2902 4e46 2901 723f 0000 0029  ..S.).NF).r?...)
+00000e70: 025a 0770 6172 616d 735f 723d 0000 00a9  .Z.params_r=....
+00000e80: 01da 096d 616b 655f 7472 6565 721c 0000  ...make_treer...
+00000e90: 0072 1d00 0000 da09 6d61 6b65 5f63 6f64  .r......make_cod
+00000ea0: 6573 0000 0073 0800 0000 0801 0801 0401  es...s..........
+00000eb0: 0801 7a2e 4669 6c65 4765 6e65 7261 746f  ..z.FileGenerato
+00000ec0: 722e 6765 6e65 7261 7465 5f63 6f64 652e  r.generate_code.
+00000ed0: 3c6c 6f63 616c 733e 2e6d 616b 655f 636f  <locals>.make_co
+00000ee0: 6465 2901 722b 0000 007a 3b46 6c75 6964  de).r+...z;Fluid
+00000ef0: 7369 6d66 6f61 6d20 736f 6c76 6572 2069  simfoam solver i
+00000f00: 7373 7565 3a20 3220 636f 6e63 7572 7265  ssue: 2 concurre
+00000f10: 6e74 206d 6574 686f 6473 2074 6f20 7072  nt methods to pr
+00000f20: 6f64 7563 6520 7a10 3a0a 2d20 7465 6d70  oduce z.:.- temp
+00000f30: 6c61 7465 2069 6e20 7a1f 2c0a 2d20 6675  late in z.,.- fu
+00000f40: 6e63 7469 6f6e 206f 7574 7075 742e 5f6d  nction output._m
+00000f50: 616b 655f 636f 6465 5f7a 3d2e 0a52 656d  ake_code_z=..Rem
+00000f60: 6f76 6520 7468 6520 6669 6c65 206f 7220  ove the file or 
+00000f70: 7468 6520 6675 6e63 7469 6f6e 2028 6f72  the function (or
+00000f80: 206d 616b 6520 6974 2065 7175 616c 2074   make it equal t
+00000f90: 6f20 4e6f 6e65 292e 2911 7210 0000 0072  o None).).r....r
+00000fa0: 1200 0000 722b 0000 00da 0767 6574 6174  ....r+.....getat
+00000fb0: 7472 da05 5f6e 616d 65da 0e41 7474 7269  tr.._name..Attri
+00000fc0: 6275 7465 4572 726f 72da 0a69 7369 6e73  buteError..isins
+00000fd0: 7461 6e63 6572 0900 0000 7249 0000 0072  tancer....rI...r
+00000fe0: 2800 0000 7220 0000 0072 2100 0000 da06  (...r ...r!.....
+00000ff0: 7265 6e64 6572 7216 0000 00da 0665 7869  renderr......exi
+00001000: 7374 73da 0c52 756e 7469 6d65 4572 726f  sts..RuntimeErro
+00001010: 7272 2700 0000 2905 721a 0000 0072 2b00  rr'...).r....r+.
+00001020: 0000 724a 0000 00da 0668 656c 7065 72da  ..rJ.....helper.
+00001030: 0874 656d 706c 6174 6572 1c00 0000 7248  .templater....rH
+00001040: 0000 0072 1d00 0000 722c 0000 0054 0000  ...r....r,...T..
+00001050: 0073 4a00 0000 0806 0a01 0202 1601 0c01  .sJ.............
+00001060: 0801 02ff 0803 0201 1601 0c01 0801 02ff  ................
+00001070: 0803 0201 1601 0c01 0401 02ff 0a03 0601  ................
+00001080: 0802 0c02 0806 0e01 0c01 1202 0201 0201  ................
+00001090: 0401 04ff 0602 04fe 0403 06fd 04ff 0808  ................
+000010a0: 7a1b 4669 6c65 4765 6e65 7261 746f 722e  z.FileGenerator.
+000010b0: 6765 6e65 7261 7465 5f63 6f64 6563 0300  generate_codec..
+000010c0: 0000 0000 0000 0000 0000 0600 0000 0800  ................
+000010d0: 0000 4300 0000 739a 0000 0074 007c 026a  ..C...s....t.|.j
+000010e0: 016a 026a 037c 026a 016a 026a 0483 027d  .j.j.|.j.j.j...}
+000010f0: 037a 0a74 057c 0364 017c 006a 0617 0083  .z.t.|.d.|.j....
+00001100: 027d 0457 006e 0b04 0074 0779 2001 0001  .}.W.n...t.y ...
+00001110: 0001 0064 007d 0459 006e 0177 007c 0464  ...d.}.Y.n.w.|.d
+00001120: 0075 0072 417a 0a74 057c 0364 027c 006a  .u.rAz.t.|.d.|.j
+00001130: 0617 0083 027d 0557 006e 0904 0074 0779  .....}.W.n...t.y
+00001140: 3801 0001 0001 0059 006e 0977 0074 087c  8......Y.n.w.t.|
+00001150: 0574 0983 0272 417c 056a 0a7d 047c 0464  .t...rA|.j.}.|.d
+00001160: 0075 0172 4b7c 047c 0183 0101 0064 0053  .u.rK|.|.....d.S
+00001170: 0064 0053 0029 034e 5a11 5f63 6f6d 706c  .d.S.).NZ._compl
+00001180: 6574 655f 7061 7261 6d73 5f72 4700 0000  ete_params_rG...
+00001190: 290b 7208 0000 00da 0763 6c61 7373 6573  ).r......classes
+000011a0: da06 4f75 7470 7574 da0b 6d6f 6475 6c65  ..Output..module
+000011b0: 5f6e 616d 65da 0a63 6c61 7373 5f6e 616d  _name..class_nam
+000011c0: 6572 4b00 0000 724c 0000 0072 4d00 0000  erK...rL...rM...
+000011d0: 724e 0000 0072 0900 0000 da0f 636f 6d70  rN...r......comp
+000011e0: 6c65 7465 5f70 6172 616d 7329 06da 0363  lete_params)...c
+000011f0: 6c73 722b 0000 00da 0b69 6e66 6f5f 736f  lsr+.....info_so
+00001200: 6c76 6572 5a0a 6f75 7470 7574 5f63 6c73  lverZ.output_cls
+00001210: 7258 0000 0072 5200 0000 721c 0000 0072  rX...rR...r....r
+00001220: 1c00 0000 721d 0000 00da 1d5f 636f 6d70  ....r......_comp
+00001230: 6c65 7465 5f70 6172 616d 735f 7769 7468  lete_params_with
+00001240: 5f64 6566 6175 6c74 8800 0000 7328 0000  _default....s(..
+00001250: 0002 0208 0108 0104 fe02 0414 010c 0108  ................
+00001260: 0102 ff08 0302 0114 010c 0104 0102 ff0a  ................
+00001270: 0306 0108 020c 0104 ff7a 2b46 696c 6547  .........z+FileG
+00001280: 656e 6572 6174 6f72 2e5f 636f 6d70 6c65  enerator._comple
+00001290: 7465 5f70 6172 616d 735f 7769 7468 5f64  te_params_with_d
+000012a0: 6566 6175 6c74 721f 0000 0029 0a72 2200  efaultr....).r".
+000012b0: 0000 7223 0000 0072 2400 0000 7241 0000  ..r#...r$...rA..
+000012c0: 0072 4200 0000 721e 0000 0072 2c00 0000  .rB...r....r,...
+000012d0: da0b 636c 6173 736d 6574 686f 6472 5b00  ..classmethodr[.
+000012e0: 0000 da0d 5f5f 636c 6173 7363 656c 6c5f  ....__classcell_
+000012f0: 5f72 1c00 0000 721c 0000 0072 4500 0000  _r....r....rE...
+00001300: 721d 0000 0072 4300 0000 4e00 0000 730c  r....rC...N...s.
+00001310: 0000 000a 0008 010c 020a 0302 3412 0172  ............4..r
+00001320: 4300 0000 da01 3063 0200 0000 0000 0000  C.....0c........
+00001330: 0000 0000 0300 0000 0b00 0000 4300 0000  ............C...
+00001340: 7342 0000 0064 0174 007c 0083 019b 009d  sB...d.t.|......
+00001350: 027d 0274 017c 0274 0266 017c 017c 019b  .}.t.|.t.f.|.|..
+00001360: 0064 027c 009b 009d 037c 009b 0064 039d  .d.|.....|...d..
+00001370: 0274 037c 00a0 0464 0464 05a1 0283 0164  .t.|...d.d.....d
+00001380: 069c 0483 0353 0029 074e 7243 0000 00fa  .....S.).NrC....
+00001390: 012f 7a06 2e6a 696e 6a61 da01 2eda 015f  ./z..jinja....._
+000013a0: 2904 da08 6469 725f 6e61 6d65 7227 0000  )...dir_namer'..
+000013b0: 0072 2100 0000 724c 0000 0029 0572 0600  .r!...rL...).r..
+000013c0: 0000 7211 0000 0072 4300 0000 7207 0000  ..r....rC...r...
+000013d0: 00da 0772 6570 6c61 6365 2903 da09 6669  ...replace)...fi
+000013e0: 6c65 5f6e 616d 6572 6200 0000 da08 636c  le_namerb.....cl
+000013f0: 735f 6e61 6d65 721c 0000 0072 1c00 0000  s_namer....r....
+00001400: 721d 0000 00da 186e 6577 5f66 696c 655f  r......new_file_
+00001410: 6765 6e65 7261 746f 725f 636c 6173 73a0  generator_class.
+00001420: 0000 0073 1400 0000 0e01 0201 0201 0401  ...s............
+00001430: 0202 0c01 0801 0e01 04fc 04fd 7266 0000  ............rf..
+00001440: 0029 0172 5e00 0000 2916 7225 0000 00da  .).r^...).r%....
+00001450: 0361 6263 7202 0000 0072 0300 0000 da07  .abcr....r......
+00001460: 696e 7370 6563 7472 0400 0000 da07 7061  inspectr......pa
+00001470: 7468 6c69 6272 0500 0000 7217 0000 00da  thlibr....r.....
+00001480: 0a69 6e66 6c65 6374 696f 6e72 0600 0000  .inflectionr....
+00001490: 7207 0000 00da 0d66 6c75 6964 6479 6e2e  r......fluiddyn.
+000014a0: 7574 696c 7208 0000 00da 1d66 6c75 6964  utilr......fluid
+000014b0: 7369 6d66 6f61 6d2e 666f 616d 5f69 6e70  simfoam.foam_inp
+000014c0: 7574 5f66 696c 6573 7209 0000 0072 0a00  ut_filesr....r..
+000014d0: 0000 720b 0000 0072 0c00 0000 7226 0000  ..r....r....r&..
+000014e0: 0072 4300 0000 7266 0000 0072 1c00 0000  .rC...rf...r....
+000014f0: 721c 0000 0072 1c00 0000 721d 0000 00da  r....r....r.....
+00001500: 083c 6d6f 6475 6c65 3e01 0000 0073 1800  .<module>....s..
+00001510: 0000 0400 1002 0c01 0c01 0802 1001 0c02  ................
+00001520: 1401 0e03 1019 1027 0e52                 .......'.R
```

### Comparing `fluidsimfoam-0.0.5/src/fluidsimfoam/foam_input_files/__pycache__/parser.cpython-310.pyc` & `fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/__pycache__/parser.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed May 10 08:15:22 2023 UTC, .py size: 9522 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 9a52 5b64 3225 0000  o........R[d2%..
+00000000: 6f0d 0d0a 0000 0000 c13f 5a64 3225 0000  o........?Zd2%..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 0401 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 0100 6401 6404 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 6d07 5a07 6d08 5a08 0100 6401  m.Z.m.Z.m.Z...d.
 00000060: 6405 6c09 6d0a 5a0a 0100 6406 6407 6c0b  d.l.m.Z...d.d.l.
 00000070: 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e 6d0f 5a0f  m.Z.m.Z.m.Z.m.Z.
@@ -46,611 +46,610 @@
 000002d0: 616d 654e da04 696e 666f da05 6474 7970  ameN..info..dtyp
 000002e0: 65da 0473 697a 6529 09da 085f 5f6e 616d  e..size)...__nam
 000002f0: 655f 5fda 0a5f 5f6d 6f64 756c 655f 5fda  e__..__module__.
 00000300: 0c5f 5f71 7561 6c6e 616d 655f 5fda 0373  .__qualname__..s
 00000310: 7472 da0f 5f5f 616e 6e6f 7461 7469 6f6e  tr..__annotation
 00000320: 735f 5f72 1b00 0000 721c 0000 0072 1d00  s__r....r....r..
 00000330: 0000 da03 696e 74a9 0072 2400 0000 7224  ....int..r$...r$
-00000340: 0000 00fa 522f 686f 6d65 2f75 7365 7273  ....R/home/users
-00000350: 2f61 7567 6965 7233 7069 2f44 6576 2f66  /augier3pi/Dev/f
-00000360: 6c75 6964 7369 6d66 6f61 6d2f 7372 632f  luidsimfoam/src/
-00000370: 666c 7569 6473 696d 666f 616d 2f66 6f61  fluidsimfoam/foa
-00000380: 6d5f 696e 7075 745f 6669 6c65 732f 7061  m_input_files/pa
-00000390: 7273 6572 2e70 7972 1900 0000 2200 0000  rser.pyr...."...
-000003a0: 730a 0000 000a 0008 020c 010c 0110 0172  s..............r
-000003b0: 1900 0000 4e63 0200 0000 0000 0000 0000  ....Nc..........
-000003c0: 0000 0300 0000 0800 0000 4300 0000 737a  ..........C...sz
-000003d0: 0000 0064 01a0 0064 0264 0384 007c 00a0  ...d...d.d...|..
-000003e0: 0164 01a1 0144 0083 01a1 017d 007c 00a0  .d...D.....}.|..
-000003f0: 0264 01a1 0173 167c 0064 0137 007d 007c  .d...s.|.d.7.}.|
-00000400: 0164 0075 0072 307a 0774 03a0 047c 00a1  .d.u.r0z.t...|..
-00000410: 017d 0257 006e 1504 0074 0579 2f01 0001  .}.W.n...t.y/...
-00000420: 0001 0074 06a0 047c 00a1 017d 0259 006e  ...t...|...}.Y.n
-00000430: 0877 0074 077c 0119 00a0 047c 00a1 017d  .w.t.|.....|...}
-00000440: 0274 0883 00a0 097c 02a1 0153 0029 044e  .t.....|...S.).N
-00000450: da01 0a63 0100 0000 0000 0000 0000 0000  ...c............
-00000460: 0200 0000 0300 0000 7300 0000 7318 0000  ........s...s...
-00000470: 0081 007c 005d 077d 017c 01a0 00a1 0056  ...|.].}.|.....V
-00000480: 0001 0071 0264 0053 00a9 014e 2901 da06  ...q.d.S...N)...
-00000490: 7273 7472 6970 2902 da02 2e30 da04 6c69  rstrip)....0..li
-000004a0: 6e65 7224 0000 0072 2400 0000 7225 0000  ner$...r$...r%..
-000004b0: 00da 093c 6765 6e65 7870 723e 2b00 0000  ...<genexpr>+...
-000004c0: 7304 0000 0002 8016 007a 1870 6172 7365  s........z.parse
-000004d0: 2e3c 6c6f 6361 6c73 3e2e 3c67 656e 6578  .<locals>.<genex
-000004e0: 7072 3e29 0ada 046a 6f69 6eda 0573 706c  pr>)...join..spl
-000004f0: 6974 da08 656e 6473 7769 7468 da0b 6c61  it..endswith..la
-00000500: 726b 5f70 6172 7365 72da 0570 6172 7365  rk_parser..parse
-00000510: 7207 0000 00da 146c 6172 6b5f 7061 7273  r......lark_pars
-00000520: 6572 5f61 6476 616e 6365 64da 0770 6172  er_advanced..par
-00000530: 7365 7273 da0f 466f 616d 5472 616e 7366  sers..FoamTransf
-00000540: 6f72 6d65 72da 0974 7261 6e73 666f 726d  ormer..transform
-00000550: 2903 da04 7465 7874 da07 6772 616d 6d61  )...text..gramma
-00000560: 72da 0474 7265 6572 2400 0000 7224 0000  r..treer$...r$..
-00000570: 0072 2500 0000 7230 0000 002a 0000 0073  .r%...r0...*...s
-00000580: 1600 0000 1a01 0a01 0801 0802 0201 0e01  ................
-00000590: 0c01 0e01 02ff 0e03 0c02 7230 0000 0063  ..........r0...c
-000005a0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-000005b0: 0200 0000 4300 0000 7308 0000 007c 00a0  ....C...s....|..
-000005c0: 00a1 0053 0072 2700 0000 2901 da04 6475  ...S.r'...)...du
-000005d0: 6d70 2901 7237 0000 0072 2400 0000 7224  mp).r7...r$...r$
-000005e0: 0000 0072 2500 0000 7238 0000 003a 0000  ...r%...r8...:..
-000005f0: 00f3 0200 0000 0801 7238 0000 0063 0100  ........r8...c..
-00000600: 0000 0000 0000 0000 0000 0100 0000 0200  ................
-00000610: 0000 4300 0000 730e 0000 0064 0164 0284  ..C...s....d.d..
-00000620: 007c 0044 0083 0153 0029 034e 6301 0000  .|.D...S.).Nc...
-00000630: 0000 0000 0000 0000 0002 0000 0004 0000  ................
-00000640: 0053 0000 00f3 1800 0000 6700 7c00 5d08  .S........g.|.].
-00000650: 7d01 7c01 6400 7501 7202 7c01 9102 7102  }.|.d.u.r.|...q.
-00000660: 5300 7227 0000 0072 2400 0000 a902 7229  S.r'...r$.....r)
-00000670: 0000 00da 0469 7465 6d72 2400 0000 7224  .....itemr$...r$
-00000680: 0000 0072 2500 0000 da0a 3c6c 6973 7463  ...r%.....<listc
-00000690: 6f6d 703e 3f00 0000 f302 0000 0018 007a  omp>?..........z
-000006a0: 2666 696c 7465 725f 6e6f 5f6e 6577 6c69  &filter_no_newli
-000006b0: 6e65 732e 3c6c 6f63 616c 733e 2e3c 6c69  nes.<locals>.<li
-000006c0: 7374 636f 6d70 3e72 2400 0000 2901 da05  stcomp>r$...)...
-000006d0: 6974 656d 7372 2400 0000 7224 0000 0072  itemsr$...r$...r
-000006e0: 2500 0000 da12 6669 6c74 6572 5f6e 6f5f  %.....filter_no_
-000006f0: 6e65 776c 696e 6573 3e00 0000 7302 0000  newlines>...s...
-00000700: 000e 0172 4000 0000 6301 0000 0000 0000  ...r@...c.......
-00000710: 0000 0000 0001 0000 0008 0000 0043 0000  .............C..
-00000720: 0073 2e00 0000 7400 7c00 8301 7d00 7a05  .s....t.|...}.z.
-00000730: 7401 7c00 8301 5700 5300 0400 7402 7916  t.|...W.S...t.y.
-00000740: 0100 0100 0100 7403 7c00 8301 0600 5900  ......t.|.....Y.
-00000750: 5300 7700 7227 0000 0029 0472 2100 0000  S.w.r'...).r!...
-00000760: 7223 0000 00da 0a56 616c 7565 4572 726f  r#.....ValueErro
-00000770: 72da 0566 6c6f 6174 2901 da06 6e75 6d62  r..float)...numb
-00000780: 6572 7224 0000 0072 2400 0000 7225 0000  err$...r$...r%..
-00000790: 00da 125f 636f 6e76 6572 745f 746f 5f6e  ..._convert_to_n
-000007a0: 756d 6265 7242 0000 0073 0c00 0000 0801  umberB...s......
-000007b0: 0201 0a01 0c01 0c01 02ff 7244 0000 0063  ..........rD...c
-000007c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000007d0: 0200 0000 4000 0000 73c4 0000 0065 005a  ....@...s....e.Z
-000007e0: 0164 005a 0264 0164 0284 005a 0364 0364  .d.Z.d.d...Z.d.d
-000007f0: 0484 005a 0464 0564 0684 005a 0564 0764  ...Z.d.d...Z.d.d
-00000800: 0884 005a 0664 0964 0a84 005a 0764 0b64  ...Z.d.d...Z.d.d
-00000810: 0c84 005a 0864 0d64 0e84 005a 0964 0f64  ...Z.d.d...Z.d.d
-00000820: 1084 005a 0a64 1164 1284 005a 0b64 1364  ...Z.d.d...Z.d.d
-00000830: 1484 005a 0c64 1564 1684 005a 0d64 1764  ...Z.d.d...Z.d.d
-00000840: 1884 005a 0e64 1964 1a84 005a 0f64 1b64  ...Z.d.d...Z.d.d
-00000850: 1c84 005a 1064 1d64 1e84 005a 1164 1f64  ...Z.d.d...Z.d.d
-00000860: 2084 005a 1264 2164 2284 005a 1364 2364   ..Z.d!d"..Z.d#d
-00000870: 2484 005a 1464 2564 2684 005a 1564 2764  $..Z.d%d&..Z.d'd
-00000880: 2884 005a 1664 2964 2a84 005a 1764 2b64  (..Z.d)d*..Z.d+d
-00000890: 2c84 005a 1864 2d64 2e84 005a 1964 2f53  ,..Z.d-d...Z.d/S
-000008a0: 0029 3072 3300 0000 6302 0000 0000 0000  .)0r3...c.......
-000008b0: 0000 0000 0002 0000 0002 0000 0043 0000  .............C..
-000008c0: 0073 0800 0000 7400 7c01 8301 5300 7227  .s....t.|...S.r'
-000008d0: 0000 0029 0172 4400 0000 a902 da04 7365  ...).rD.......se
-000008e0: 6c66 da05 746f 6b65 6e72 2400 0000 7224  lf..tokenr$...r$
-000008f0: 0000 0072 2500 0000 da0d 5349 474e 4544  ...r%.....SIGNED
-00000900: 5f4e 554d 4245 524b 0000 0072 3900 0000  _NUMBERK...r9...
-00000910: 7a1d 466f 616d 5472 616e 7366 6f72 6d65  z.FoamTransforme
-00000920: 722e 5349 474e 4544 5f4e 554d 4245 5263  r.SIGNED_NUMBERc
-00000930: 0200 0000 0000 0000 0000 0000 0200 0000  ................
-00000940: 0100 0000 4300 0000 f306 0000 007c 016a  ....C........|.j
-00000950: 0053 0072 2700 0000 a901 7214 0000 0072  .S.r'.....r....r
-00000960: 4500 0000 7224 0000 0072 2400 0000 7225  E...r$...r$...r%
-00000970: 0000 00da 0543 4e41 4d45 4e00 0000 f302  .....CNAMEN.....
-00000980: 0000 0006 017a 1546 6f61 6d54 7261 6e73  .....z.FoamTrans
-00000990: 666f 726d 6572 2e43 4e41 4d45 6302 0000  former.CNAMEc...
-000009a0: 0000 0000 0000 0000 0002 0000 0001 0000  ................
-000009b0: 0043 0000 0073 0400 0000 6400 5300 7227  .C...s....d.S.r'
-000009c0: 0000 0072 2400 0000 a902 7246 0000 00da  ...r$.....rF....
-000009d0: 056e 6f64 6573 7224 0000 0072 2400 0000  .nodesr$...r$...
-000009e0: 7225 0000 00da 074e 4557 4c49 4e45 5100  r%.....NEWLINEQ.
-000009f0: 0000 7302 0000 0004 017a 1746 6f61 6d54  ..s......z.FoamT
-00000a00: 7261 6e73 666f 726d 6572 2e4e 4557 4c49  ransformer.NEWLI
-00000a10: 4e45 6302 0000 0000 0000 0000 0000 0002  NEc.............
-00000a20: 0000 0001 0000 0043 0000 0072 4900 0000  .......C...rI...
-00000a30: 7227 0000 0072 4a00 0000 7245 0000 0072  r'...rJ...rE...r
-00000a40: 2400 0000 7224 0000 0072 2500 0000 da0e  $...r$...r%.....
-00000a50: 4553 4341 5045 445f 5354 5249 4e47 5400  ESCAPED_STRINGT.
-00000a60: 0000 724c 0000 007a 1e46 6f61 6d54 7261  ..rL...z.FoamTra
-00000a70: 6e73 666f 726d 6572 2e45 5343 4150 4544  nsformer.ESCAPED
-00000a80: 5f53 5452 494e 4763 0200 0000 0000 0000  _STRINGc........
-00000a90: 0000 0000 0200 0000 0100 0000 4300 0000  ............C...
-00000aa0: 7249 0000 0072 2700 0000 724a 0000 0072  rI...r'...rJ...r
-00000ab0: 4500 0000 7224 0000 0072 2400 0000 7225  E...r$...r$...r%
-00000ac0: 0000 00da 0b44 4f55 424c 455f 4e41 4d45  .....DOUBLE_NAME
-00000ad0: 5700 0000 724c 0000 007a 1b46 6f61 6d54  W...rL...z.FoamT
-00000ae0: 7261 6e73 666f 726d 6572 2e44 4f55 424c  ransformer.DOUBL
-00000af0: 455f 4e41 4d45 6302 0000 0000 0000 0000  E_NAMEc.........
-00000b00: 0000 0002 0000 0001 0000 0043 0000 0072  ...........C...r
-00000b10: 4900 0000 7227 0000 0072 4a00 0000 7245  I...r'...rJ...rE
-00000b20: 0000 0072 2400 0000 7224 0000 0072 2500  ...r$...r$...r%.
-00000b30: 0000 da0b 5452 4950 4c45 5f4e 414d 455a  ....TRIPLE_NAMEZ
-00000b40: 0000 0072 4c00 0000 7a1b 466f 616d 5472  ...rL...z.FoamTr
-00000b50: 616e 7366 6f72 6d65 722e 5452 4950 4c45  ansformer.TRIPLE
-00000b60: 5f4e 414d 4563 0200 0000 0000 0000 0000  _NAMEc..........
-00000b70: 0000 0200 0000 0100 0000 4300 0000 7249  ..........C...rI
-00000b80: 0000 0072 2700 0000 724a 0000 0072 4500  ...r'...rJ...rE.
-00000b90: 0000 7224 0000 0072 2400 0000 7225 0000  ..r$...r$...r%..
-00000ba0: 00da 0545 514b 4559 5d00 0000 724c 0000  ...EQKEY]...rL..
-00000bb0: 007a 1546 6f61 6d54 7261 6e73 666f 726d  .z.FoamTransform
-00000bc0: 6572 2e45 514b 4559 6302 0000 0000 0000  er.EQKEYc.......
-00000bd0: 0000 0000 0002 0000 0001 0000 0043 0000  .............C..
-00000be0: 0072 4900 0000 7227 0000 0072 4a00 0000  .rI...r'...rJ...
-00000bf0: 7245 0000 0072 2400 0000 7224 0000 0072  rE...r$...r$...r
-00000c00: 2500 0000 da05 4d41 4352 4f60 0000 0072  %.....MACRO`...r
-00000c10: 4c00 0000 7a15 466f 616d 5472 616e 7366  L...z.FoamTransf
-00000c20: 6f72 6d65 722e 4d41 4352 4f63 0200 0000  ormer.MACROc....
-00000c30: 0000 0000 0000 0000 0200 0000 0300 0000  ................
-00000c40: 4300 0000 f312 0000 0074 0064 0164 0284  C........t.d.d..
-00000c50: 007c 0144 0083 0183 0153 0029 034e 6301  .|.D.....S.).Nc.
-00000c60: 0000 0000 0000 0000 0000 0002 0000 0005  ................
-00000c70: 0000 0053 0000 0073 2400 0000 6700 7c00  ...S...s$...g.|.
-00000c80: 5d0e 7d01 7400 7c01 7401 8302 720e 7c01  ].}.t.|.t...r.|.
-00000c90: 6a02 6400 6b02 7302 7c01 9102 7102 5300  j.d.k.s.|...q.S.
-00000ca0: 2901 724f 0000 00a9 03da 0a69 7369 6e73  ).rO.......isins
-00000cb0: 7461 6e63 6572 0500 0000 da04 7479 7065  tancer......type
-00000cc0: 723b 0000 0072 2400 0000 7224 0000 0072  r;...r$...r$...r
-00000cd0: 2500 0000 723d 0000 0065 0000 00f3 1000  %...r=...e......
-00000ce0: 0000 0600 0202 0801 02fd 0803 02fd 0201  ................
-00000cf0: 06ff 7a31 466f 616d 5472 616e 7366 6f72  ..z1FoamTransfor
-00000d00: 6d65 722e 6469 6d65 6e73 696f 6e5f 7365  mer.dimension_se
-00000d10: 742e 3c6c 6f63 616c 733e 2e3c 6c69 7374  t.<locals>.<list
-00000d20: 636f 6d70 3e29 0172 0d00 0000 a902 7246  comp>).r......rF
-00000d30: 0000 0072 3f00 0000 7224 0000 0072 2400  ...r?...r$...r$.
-00000d40: 0000 7225 0000 00da 0d64 696d 656e 7369  ..r%.....dimensi
-00000d50: 6f6e 5f73 6574 6300 0000 f30a 0000 0002  on_setc.........
-00000d60: 0106 0102 0204 fe04 ff7a 1d46 6f61 6d54  .........z.FoamT
-00000d70: 7261 6e73 666f 726d 6572 2e64 696d 656e  ransformer.dimen
-00000d80: 7369 6f6e 5f73 6574 6302 0000 0000 0000  sion_setc.......
-00000d90: 0000 0000 0002 0000 0003 0000 0043 0000  .............C..
-00000da0: 0073 1c00 0000 7400 7c01 8301 6401 6b03  .s....t.|...d.k.
-00000db0: 7208 7401 8201 7402 7c01 6402 1900 8301  r.t...t.|.d.....
-00000dc0: 5300 a903 4e72 0800 0000 7201 0000 0029  S...Nr....r....)
-00000dd0: 03da 036c 656e da0c 5275 6e74 696d 6545  ...len..RuntimeE
-00000de0: 7272 6f72 7221 0000 0072 4d00 0000 7224  rrorr!...rM...r$
-00000df0: 0000 0072 2400 0000 7225 0000 00da 0964  ...r$...r%.....d
-00000e00: 6972 6563 7469 7665 6c00 0000 7306 0000  irectivel...s...
-00000e10: 000c 0104 010c 017a 1946 6f61 6d54 7261  .......z.FoamTra
-00000e20: 6e73 666f 726d 6572 2e64 6972 6563 7469  nsformer.directi
-00000e30: 7665 6302 0000 0000 0000 0000 0000 0002  vec.............
-00000e40: 0000 0003 0000 0043 0000 0072 5500 0000  .......C...rU...
-00000e50: 2903 4e63 0100 0000 0000 0000 0000 0000  ).Nc............
-00000e60: 0200 0000 0500 0000 5300 0000 732c 0000  ........S...s,..
-00000e70: 0067 007c 005d 127d 0174 007c 0174 0183  .g.|.].}.t.|.t..
-00000e80: 0272 0e7c 016a 0264 006b 0273 027c 0164  .r.|.j.d.k.s.|.d
-00000e90: 0175 0172 027c 0191 0271 0253 0029 0272  .u.r.|...q.S.).r
-00000ea0: 4f00 0000 4e72 5600 0000 723b 0000 0072  O...NrV...r;...r
-00000eb0: 2400 0000 7224 0000 0072 2500 0000 723d  $...r$...r%...r=
-00000ec0: 0000 0073 0000 0073 1400 0000 0600 0202  ...s...s........
-00000ed0: 0801 02fd 0803 02fd 0604 02fc 0201 06ff  ................
-00000ee0: 7a28 466f 616d 5472 616e 7366 6f72 6d65  z(FoamTransforme
-00000ef0: 722e 6c69 7374 2e3c 6c6f 6361 6c73 3e2e  r.list.<locals>.
-00000f00: 3c6c 6973 7463 6f6d 703e 2901 7210 0000  <listcomp>).r...
-00000f10: 0072 5a00 0000 7224 0000 0072 2400 0000  .rZ...r$...r$...
-00000f20: 7225 0000 00da 046c 6973 7471 0000 0072  r%.....listq...r
-00000f30: 5c00 0000 7a14 466f 616d 5472 616e 7366  \...z.FoamTransf
-00000f40: 6f72 6d65 722e 6c69 7374 6302 0000 0000  ormer.listc.....
-00000f50: 0000 0000 0000 0005 0000 0004 0000 0043  ...............C
-00000f60: 0000 0073 6200 0000 7c01 6401 1900 7d02  ...sb...|.d...}.
-00000f70: 7c02 6a00 6402 6b02 7213 7c02 6a01 7d03  |.j.d.k.r.|.j.}.
-00000f80: 7c01 6403 6400 8502 1900 7d01 6e02 6400  |.d.d.....}.n.d.
-00000f90: 7d03 7c01 4400 5d0f 7d04 7402 7c04 6a01  }.|.D.].}.t.|.j.
-00000fa0: 7403 8302 7226 7c04 6a01 a004 7c04 6a00  t...r&|.j...|.j.
-00000fb0: a101 0100 7117 7405 7c03 6404 6405 8400  ....q.t.|.d.d...
-00000fc0: 7c01 4400 8301 8302 5300 2906 4e72 0100  |.D.....S.).Nr..
-00000fd0: 0000 5a08 466f 616d 4669 6c65 7208 0000  ..Z.FoamFiler...
-00000fe0: 0063 0100 0000 0000 0000 0000 0000 0200  .c..............
-00000ff0: 0000 0400 0000 5300 0000 f316 0000 0069  ......S........i
-00001000: 007c 005d 077d 017c 016a 007c 016a 0193  .|.].}.|.j.|.j..
-00001010: 0271 0253 0072 2400 0000 a902 721a 0000  .q.S.r$.....r...
-00001020: 0072 1400 0000 a902 7229 0000 00da 046e  .r......r).....n
-00001030: 6f64 6572 2400 0000 7224 0000 0072 2500  oder$...r$...r%.
-00001040: 0000 da0a 3c64 6963 7463 6f6d 703e 8700  ....<dictcomp>..
-00001050: 0000 f302 0000 0016 007a 2846 6f61 6d54  .........z(FoamT
-00001060: 7261 6e73 666f 726d 6572 2e66 696c 652e  ransformer.file.
-00001070: 3c6c 6f63 616c 733e 2e3c 6469 6374 636f  <locals>.<dictco
-00001080: 6d70 3e29 0672 1a00 0000 7214 0000 0072  mp>).r....r....r
-00001090: 5700 0000 7210 0000 00da 0861 6464 5f6e  W...r......add_n
-000010a0: 616d 6572 0f00 0000 2905 7246 0000 0072  amer....).rF...r
-000010b0: 4e00 0000 5a10 6669 7273 745f 6173 7369  N...Z.first_assi
-000010c0: 676e 6d65 6e74 da09 696e 666f 5f64 6963  gnment..info_dic
-000010d0: 7472 6500 0000 7224 0000 0072 2400 0000  tre...r$...r$...
-000010e0: 7225 0000 00da 0466 696c 657b 0000 0073  r%.....file{...s
-000010f0: 1400 0000 0801 0a01 0601 0e01 0402 0802  ................
-00001100: 0c01 0e01 0280 1402 7a14 466f 616d 5472  ........z.FoamTr
-00001110: 616e 7366 6f72 6d65 722e 6669 6c65 6302  ansformer.filec.
-00001120: 0000 0000 0000 0000 0000 0008 0000 0008  ................
-00001130: 0000 0043 0000 0073 1201 0000 6401 6402  ...C...s....d.d.
-00001140: 8400 7c01 4400 8301 7d01 6400 7d02 6400  ..|.D...}.d.}.d.
-00001150: 7d03 7c01 a000 6403 a101 7d04 7401 7c01  }.|...d...}.t.|.
-00001160: 8301 6404 6b02 721b 7c01 6403 1900 7d05  ..d.k.r.|.d...}.
-00001170: 6e69 7a0c 6405 6402 8400 7c01 4400 8301  niz.d.d...|.D...
-00001180: a002 6406 a101 7d06 5700 6e0b 0400 7403  ..d...}.W.n...t.
-00001190: 7932 0100 0100 0100 6400 7d02 5900 6e06  y2......d.}.Y.n.
-000011a0: 7700 7c01 a000 7c06 a101 7d02 6400 7d03  w.|...|...}.d.}.
-000011b0: 7404 6407 6402 8400 7c01 4400 8301 8301  t.d.d...|.D.....
-000011c0: 7249 6408 a005 7c01 a101 7d07 6e24 7c01  rId...|...}.n$|.
-000011d0: a000 6409 a101 7d07 7404 640a 640b 8400  ..d...}.t.d.d...
-000011e0: 7c01 4400 8301 8301 735e 640c 6402 8400  |.D.....s^d.d...
-000011f0: 7c01 4400 8301 7d01 7c01 7265 6408 a005  |.D...}.|.red...
-00001200: 7c01 a101 7d03 7406 7c07 7407 8302 726d  |...}.t.|.t...rm
-00001210: 7c03 7c07 5f08 7c03 6400 7500 7275 7c02  |.|._.|.d.u.ru|.
-00001220: 6400 7500 737a 7406 7c07 7407 8302 727d  d.u.szt.|.t...r}
-00001230: 7c07 7d05 6e07 7409 7c07 7c03 7c02 640d  |.}.n.t.|.|.|.d.
-00001240: 8d03 7d05 740a 7c04 7c05 8302 5300 290e  ..}.t.|.|...S.).
-00001250: 4e63 0100 0000 0000 0000 0000 0000 0200  Nc..............
-00001260: 0000 0400 0000 5300 0000 723a 0000 0072  ......S...r:...r
-00001270: 2700 0000 7224 0000 0072 6400 0000 7224  '...r$...rd...r$
-00001280: 0000 0072 2400 0000 7225 0000 0072 3d00  ...r$...r%...r=.
-00001290: 0000 8a00 0000 723e 0000 007a 3246 6f61  ......r>...z2Foa
-000012a0: 6d54 7261 6e73 666f 726d 6572 2e76 6172  mTransformer.var
-000012b0: 5f61 7373 6967 6e6d 656e 742e 3c6c 6f63  _assignment.<loc
-000012c0: 616c 733e 2e3c 6c69 7374 636f 6d70 3e72  als>.<listcomp>r
-000012d0: 0100 0000 7208 0000 0063 0100 0000 0000  ....r....c......
-000012e0: 0000 0000 0000 0200 0000 0500 0000 5300  ..............S.
-000012f0: 0000 f316 0000 0067 007c 005d 077d 0174  .......g.|.].}.t
-00001300: 007c 0174 0183 0291 0271 0253 0072 2400  .|.t.....q.S.r$.
-00001310: 0000 2902 7257 0000 0072 0d00 0000 a902  ..).rW...r......
-00001320: 7229 0000 00da 0465 6c65 6d72 2400 0000  r).....elemr$...
-00001330: 7224 0000 0072 2500 0000 723d 0000 0092  r$...r%...r=....
-00001340: 0000 0073 0600 0000 0600 0a01 06ff 5463  ...s..........Tc
-00001350: 0100 0000 0000 0000 0000 0000 0200 0000  ................
-00001360: 0500 0000 5300 0000 726b 0000 0072 2400  ....S...rk...r$.
-00001370: 0000 a902 7257 0000 0072 2100 0000 726c  ....rW...r!...rl
-00001380: 0000 0072 2400 0000 7224 0000 0072 2500  ...r$...r$...r%.
-00001390: 0000 723d 0000 009b 0000 0072 6700 0000  ..r=.......rg...
-000013a0: da01 20e9 ffff ffff 6301 0000 0000 0000  .. .....c.......
-000013b0: 0000 0000 0002 0000 0004 0000 0073 0000  .............s..
-000013c0: 0073 1a00 0000 8100 7c00 5d08 7d01 7400  .s......|.].}.t.
-000013d0: 7c01 7401 8302 5600 0100 7102 6400 5300  |.t...V...q.d.S.
-000013e0: 7227 0000 0072 6e00 0000 7264 0000 0072  r'...rn...rd...r
-000013f0: 2400 0000 7224 0000 0072 2500 0000 722b  $...r$...r%...r+
-00001400: 0000 009f 0000 0073 0400 0000 0280 1800  .......s........
-00001410: 7a31 466f 616d 5472 616e 7366 6f72 6d65  z1FoamTransforme
-00001420: 722e 7661 725f 6173 7369 676e 6d65 6e74  r.var_assignment
-00001430: 2e3c 6c6f 6361 6c73 3e2e 3c67 656e 6578  .<locals>.<genex
-00001440: 7072 3e63 0100 0000 0000 0000 0000 0000  pr>c............
-00001450: 0200 0000 0400 0000 5300 0000 7314 0000  ........S...s...
-00001460: 0067 007c 005d 067d 0174 007c 0183 0191  .g.|.].}.t.|....
-00001470: 0271 0253 0072 2400 0000 2901 7221 0000  .q.S.r$...).r!..
-00001480: 0072 6400 0000 7224 0000 0072 2400 0000  .rd...r$...r$...
-00001490: 7225 0000 0072 3d00 0000 a000 0000 7302  r%...r=.......s.
-000014a0: 0000 0014 0029 0272 1a00 0000 da09 6469  .....).r......di
-000014b0: 6d65 6e73 696f 6e29 0bda 0370 6f70 725e  mension)...popr^
-000014c0: 0000 00da 0569 6e64 6578 7241 0000 00da  .....indexrA....
-000014d0: 0361 6c6c 722c 0000 0072 5700 0000 7210  .allr,...rW...r.
-000014e0: 0000 00da 055f 6e61 6d65 7212 0000 0072  ....._namer....r
-000014f0: 1300 0000 2908 7246 0000 0072 4e00 0000  ....).rF...rN...
-00001500: 725b 0000 005a 0d6e 616d 655f 696e 5f76  r[...Z.name_in_v
-00001510: 616c 7565 721a 0000 0072 1400 0000 5a0f  aluer....r....Z.
-00001520: 696e 6465 785f 6469 6d65 6e73 696f 6eda  index_dimension.
-00001530: 0a6c 6173 745f 7661 6c75 6572 2400 0000  .last_valuer$...
-00001540: 7224 0000 0072 2500 0000 da0e 7661 725f  r$...r%.....var_
-00001550: 6173 7369 676e 6d65 6e74 8900 0000 7344  assignment....sD
-00001560: 0000 000e 0104 0104 010a 010c 010a 0102  ................
-00001570: 0206 0102 0104 ff06 0206 fe0c 0308 0102  ................
-00001580: ff0a 0304 0212 010c 010a 0212 010e 0104  ................
-00001590: 010a 010a 0106 0112 0204 0104 ff06 0302  ................
-000015a0: 0206 0106 ff0a 037a 1e46 6f61 6d54 7261  .......z.FoamTra
-000015b0: 6e73 666f 726d 6572 2e76 6172 5f61 7373  nsformer.var_ass
-000015c0: 6967 6e6d 656e 7463 0200 0000 0000 0000  ignmentc........
-000015d0: 0000 0000 0800 0000 0700 0000 4300 0000  ............C...
-000015e0: 7316 0100 0074 007c 0183 017d 0164 007d  s....t.|...}.d.}
-000015f0: 0274 017c 0183 0164 016b 0272 1a7c 01a0  .t.|...d.k.r.|..
-00001600: 0264 02a1 017d 0374 037c 0374 0469 007c  .d...}.t.|.t.i.|
-00001610: 0364 038d 0283 0253 0067 007d 047c 0144  .d.....S.g.}.|.D
-00001620: 005d 137d 0574 057c 0574 0683 0272 317c  .].}.t.|.t...r1|
-00001630: 05a0 0764 04a1 0172 317c 01a0 0264 01a1  ...d...r1|...d..
-00001640: 017d 0201 006e 0171 1e74 057c 0164 0219  .}...n.q.t.|.d..
-00001650: 0074 0883 0272 4664 0564 06a0 097c 01a0  .t...rFd.d...|..
-00001660: 0264 02a1 01a1 0117 0064 0717 007d 036e  .d.......d...}.n
-00001670: 057c 01a0 0264 02a1 017d 037c 0472 567c  .|...d...}.|.rV|
-00001680: 0364 0664 06a0 097c 04a1 0117 0037 007d  .d.d...|.....7.}
-00001690: 0364 0864 0984 007c 0144 0083 017d 067c  .d.d...|.D...}.|
-000016a0: 0644 005d 0f7d 0574 057c 056a 0a74 0b83  .D.].}.t.|.j.t..
-000016b0: 0272 6e7c 056a 0aa0 0c7c 056a 0da1 0101  .rn|.j...|.j....
-000016c0: 0071 5f7c 0264 0075 0172 7a7c 0264 0a6b  .q_|.d.u.rz|.d.k
-000016d0: 0272 7a74 0e7d 076e 0274 047d 0774 037c  .rzt.}.n.t.}.t.|
-000016e0: 037c 0764 0b64 0c84 007c 0644 0083 017c  .|.d.d...|.D...|
-000016f0: 037c 0264 0d8d 0383 0253 0029 0e4e 7208  .|.d.....S.).Nr.
-00001700: 0000 0072 0100 0000 2902 da04 6461 7461  ...r....)...data
-00001710: 721a 0000 00fa 0123 fa01 2872 6f00 0000  r......#..(ro...
-00001720: fa01 2963 0100 0000 0000 0000 0000 0000  ..)c............
-00001730: 0200 0000 0500 0000 5300 0000 7324 0000  ........S...s$..
-00001740: 0067 007c 005d 0e7d 0174 007c 0164 0083  .g.|.].}.t.|.d..
-00001750: 0272 0274 007c 0164 0183 0272 027c 0191  .r.t.|.d...r.|..
-00001760: 0271 0253 0072 6300 0000 2901 da07 6861  .q.S.rc...)...ha
-00001770: 7361 7474 7272 6400 0000 7224 0000 0072  sattrrd...r$...r
-00001780: 2400 0000 7225 0000 0072 3d00 0000 c500  $...r%...r=.....
-00001790: 0000 7259 0000 007a 3346 6f61 6d54 7261  ..rY...z3FoamTra
-000017a0: 6e73 666f 726d 6572 2e64 6963 745f 6173  nsformer.dict_as
-000017b0: 7369 676e 6d65 6e74 2e3c 6c6f 6361 6c73  signment.<locals
-000017c0: 3e2e 3c6c 6973 7463 6f6d 703e 7a0b 2363  >.<listcomp>z.#c
-000017d0: 6f64 6553 7472 6561 6d63 0100 0000 0000  odeStreamc......
-000017e0: 0000 0000 0000 0200 0000 0400 0000 5300  ..............S.
-000017f0: 0000 7262 0000 0072 2400 0000 7263 0000  ..rb...r$...rc..
-00001800: 0072 6400 0000 7224 0000 0072 2400 0000  .rd...r$...r$...
-00001810: 7225 0000 0072 6600 0000 d700 0000 7267  r%...rf.......rg
-00001820: 0000 007a 3346 6f61 6d54 7261 6e73 666f  ...z3FoamTransfo
-00001830: 726d 6572 2e64 6963 745f 6173 7369 676e  rmer.dict_assign
-00001840: 6d65 6e74 2e3c 6c6f 6361 6c73 3e2e 3c64  ment.<locals>.<d
-00001850: 6963 7463 6f6d 703e 2903 7278 0000 0072  ictcomp>).rx...r
-00001860: 1a00 0000 7260 0000 0029 0f72 4000 0000  ....r`...).r@...
-00001870: 725e 0000 0072 7200 0000 7209 0000 0072  r^...rr...r....r
-00001880: 0c00 0000 7257 0000 0072 2100 0000 da0a  ....rW...r!.....
-00001890: 7374 6172 7473 7769 7468 7261 0000 0072  startswithra...r
-000018a0: 2c00 0000 7214 0000 0072 1000 0000 7268  ,...r....r....rh
-000018b0: 0000 0072 1a00 0000 720b 0000 0029 0872  ...r....r....).r
-000018c0: 4600 0000 724e 0000 0072 6000 0000 721a  F...rN...r`...r.
-000018d0: 0000 005a 096e 6f64 6573 5f73 7472 7265  ...Z.nodes_strre
-000018e0: 0000 005a 0c6e 6f64 6573 5f61 7373 6967  ...Z.nodes_assig
-000018f0: 6eda 0363 6c73 7224 0000 0072 2400 0000  n..clsr$...r$...
-00001900: 7225 0000 00da 0f64 6963 745f 6173 7369  r%.....dict_assi
-00001910: 676e 6d65 6e74 b000 0000 7344 0000 0008  gnment....sD....
-00001920: 0104 010c 020a 0112 0104 0208 0114 010a  ................
-00001930: 0204 0102 800e 011a 010a 0204 0112 0106  ................
-00001940: 0202 0206 fe08 060c 010e 0102 8010 0206  ................
-00001950: 0104 0202 0202 0102 010c 0102 0102 0104  ................
-00001960: fd04 fe7a 1f46 6f61 6d54 7261 6e73 666f  ...z.FoamTransfo
-00001970: 726d 6572 2e64 6963 745f 6173 7369 676e  rmer.dict_assign
-00001980: 6d65 6e74 6302 0000 0000 0000 0000 0000  mentc...........
-00001990: 0003 0000 0004 0000 0043 0000 0073 2e00  .........C...s..
-000019a0: 0000 7400 7c01 8301 7d01 7401 7c01 8301  ..t.|...}.t.|...
-000019b0: 6401 6b03 720e 7402 7c01 8301 8201 6400  d.k.r.t.|.....d.
-000019c0: 7d02 7403 7c02 7c01 6402 1900 8302 5300  }.t.|.|.d.....S.
-000019d0: 725d 0000 0029 0472 4000 0000 725e 0000  r]...).r@...r^..
-000019e0: 00da 134e 6f74 496d 706c 656d 656e 7465  ...NotImplemente
-000019f0: 6445 7272 6f72 7209 0000 00a9 0372 4600  dErrorr......rF.
-00001a00: 0000 724e 0000 0072 1a00 0000 7224 0000  ..rN...r....r$..
-00001a10: 0072 2400 0000 7225 0000 00da 0d69 736f  .r$...r%.....iso
-00001a20: 6c61 7465 645f 6c69 7374 dd00 0000 730a  lated_list....s.
-00001a30: 0000 0008 010c 0108 0104 010e 017a 1d46  .............z.F
-00001a40: 6f61 6d54 7261 6e73 666f 726d 6572 2e69  oamTransformer.i
-00001a50: 736f 6c61 7465 645f 6c69 7374 6302 0000  solated_listc...
-00001a60: 0000 0000 0000 0000 0008 0000 0006 0000  ................
-00001a70: 0043 0000 0073 ac00 0000 7400 7c01 8301  .C...s....t.|...
-00001a80: 7d01 6400 7d02 7401 7c01 8301 4400 5d18  }.d.}.t.|...D.].
-00001a90: 5c02 7d03 7d04 7402 7c04 7403 8302 7222  \.}.}.t.|.t...r"
-00001aa0: 7c04 6a04 6401 6b02 7222 7405 7c04 8301  |.j.d.k.r"t.|...
-00001ab0: 6402 6403 8502 1900 7d02 0100 6e01 710a  d.d.....}...n.q.
-00001ac0: 7c02 6400 7501 722c 7c01 a006 7c03 a101  |.d.u.r,|...|...
-00001ad0: 0100 6400 7d05 7407 7c01 8301 6404 6b04  ..d.}.t.|...d.k.
-00001ae0: 7240 7402 7c01 6403 1900 7408 8302 7240  r@t.|.d...t...r@
-00001af0: 7c01 a006 6403 a101 7d05 7c01 a006 6405  |...d...}.|...d.
-00001b00: a101 7d06 6400 7d07 7c01 724e 6406 a009  ..}.d.}.|.rNd...
-00001b10: 7c01 a101 7d07 740a 7c06 7c07 7c02 7c05  |...}.t.|.|.|.|.
-00001b20: 6407 8d04 5300 2908 4e5a 094c 4953 545f  d...S.).NZ.LIST_
-00001b30: 5459 5045 e905 0000 0072 7000 0000 7208  TYPE.....rp...r.
-00001b40: 0000 0072 0100 0000 726f 0000 0029 0472  ...r....ro...).r
-00001b50: 1a00 0000 721b 0000 0072 1c00 0000 721d  ....r....r....r.
-00001b60: 0000 0029 0b72 4000 0000 da09 656e 756d  ...).r@.....enum
-00001b70: 6572 6174 6572 5700 0000 7205 0000 0072  eraterW...r....r
-00001b80: 5800 0000 7221 0000 0072 7200 0000 725e  X...r!...rr...r^
-00001b90: 0000 0072 2300 0000 722c 0000 0072 1900  ...r#...r,...r..
-00001ba0: 0000 2908 7246 0000 0072 4e00 0000 721c  ..).rF...rN...r.
-00001bb0: 0000 00da 0569 6e6f 6465 7265 0000 0072  .....inodere...r
-00001bc0: 1d00 0000 721a 0000 0072 1b00 0000 7224  ....r....r....r$
-00001bd0: 0000 0072 2400 0000 7225 0000 00da 096c  ...r$...r%.....l
-00001be0: 6973 745f 696e 666f e400 0000 7322 0000  ist_info....s"..
-00001bf0: 0008 0104 0210 0114 0110 0104 0102 8008  ................
-00001c00: 010a 0104 021a 010a 010a 0204 0204 010a  ................
-00001c10: 0110 027a 1946 6f61 6d54 7261 6e73 666f  ...z.FoamTransfo
-00001c20: 726d 6572 2e6c 6973 745f 696e 666f 6302  rmer.list_infoc.
-00001c30: 0000 0000 0000 0000 0000 0006 0000 0004  ................
-00001c40: 0000 0043 0000 0073 aa00 0000 7400 7c01  ...C...s....t.|.
-00001c50: 8301 7d01 7c01 5c02 7d02 7d03 7401 7c02  ..}.|.\.}.}.t.|.
-00001c60: 7402 8302 730f 4a00 8201 7c02 6a03 7d04  t...s.J...|.j.}.
-00001c70: 7c04 7d05 7c02 6a04 6400 7501 7220 7c05  |.}.|.j.d.u.r |.
-00001c80: 6401 7c02 6a04 1700 3700 7d05 7c02 6a05  d.|.j...7.}.|.j.
-00001c90: 6400 7501 722e 7c05 6402 7c02 6a05 9b00  d.u.r.|.d.|.j...
-00001ca0: 6403 9d03 3700 7d05 7c02 6a06 6400 7501  d...7.}.|.j.d.u.
-00001cb0: 723b 7c05 6404 7c02 6a06 9b00 9d02 3700  r;|.d.|.j.....7.
-00001cc0: 7d05 7401 7c04 7407 8302 7244 7408 7c04  }.t.|.t...rDt.|.
-00001cd0: 8301 7d04 7401 7c05 7407 8302 724d 7408  ..}.t.|.t...rMt.
-00001ce0: 7c05 8301 7d05 7c05 7c03 5f09 740a 7c04  |...}.|.|._.t.|.
-00001cf0: 7c03 8302 5300 2905 4e72 6f00 0000 7a06  |...S.).Nro...z.
-00001d00: 0a4c 6973 743c da01 3e72 2600 0000 290b  .List<..>r&...).
-00001d10: 7240 0000 0072 5700 0000 7219 0000 0072  r@...rW...r....r
-00001d20: 1a00 0000 721b 0000 0072 1c00 0000 721d  ....r....r....r.
-00001d30: 0000 0072 2300 0000 7221 0000 0072 7500  ...r#...r!...ru.
-00001d40: 0000 7209 0000 0029 0672 4600 0000 724e  ..r....).rF...rN
-00001d50: 0000 0072 8600 0000 da08 7468 655f 6c69  ...r......the_li
-00001d60: 7374 721a 0000 005a 0d6e 616d 655f 696e  str....Z.name_in
-00001d70: 7465 726e 616c 7224 0000 0072 2400 0000  ternalr$...r$...
-00001d80: 7225 0000 00da 0f6c 6973 745f 6173 7369  r%.....list_assi
-00001d90: 676e 6d65 6e74 fb00 0000 7322 0000 0008  gnment....s"....
-00001da0: 0108 020e 0106 0204 010a 020e 010a 0212  ................
-00001db0: 010a 0210 010a 0208 010a 0108 0106 020a  ................
-00001dc0: 017a 1f46 6f61 6d54 7261 6e73 666f 726d  .z.FoamTransform
-00001dd0: 6572 2e6c 6973 745f 6173 7369 676e 6d65  er.list_assignme
-00001de0: 6e74 6302 0000 0000 0000 0000 0000 0003  ntc.............
-00001df0: 0000 0007 0000 0043 0000 0073 7000 0000  .......C...sp...
-00001e00: 6401 6402 8400 7c01 4400 8301 7d01 7c01  d.d...|.D...}.|.
-00001e10: a000 6403 a101 7d02 7401 7c01 8301 6404  ..d...}.t.|...d.
-00001e20: 6b02 7221 7402 7c02 7403 7c01 6405 1900  k.r!t.|.t.|.d...
-00001e30: 7c01 6403 1900 7c01 6406 1900 8303 8302  |.d...|.d.......
-00001e40: 5300 7401 7c01 8301 6407 6b02 7234 7402  S.t.|...d.k.r4t.
-00001e50: 7c02 7403 7c01 6405 1900 7c01 6406 1900  |.t.|.d...|.d...
-00001e60: 6408 8d02 8302 5300 7404 7c01 8301 8201  d.....S.t.|.....
-00001e70: 2909 4e63 0100 0000 0000 0000 0000 0000  ).Nc............
-00001e80: 0200 0000 0400 0000 5300 0000 723a 0000  ........S...r:..
-00001e90: 0072 2700 0000 7224 0000 0072 6400 0000  .r'...r$...rd...
-00001ea0: 7224 0000 0072 2400 0000 7225 0000 0072  r$...r$...r%...r
-00001eb0: 3d00 0000 1601 0000 723e 0000 007a 3846  =.......r>...z8F
-00001ec0: 6f61 6d54 7261 6e73 666f 726d 6572 2e64  oamTransformer.d
-00001ed0: 696d 656e 7369 6f6e 5f61 7373 6967 6e6d  imension_assignm
-00001ee0: 656e 742e 3c6c 6f63 616c 733e 2e3c 6c69  ent.<locals>.<li
-00001ef0: 7374 636f 6d70 3e72 0100 0000 e903 0000  stcomp>r........
-00001f00: 0072 7000 0000 e9fe ffff ffe9 0200 0000  .rp.............
-00001f10: 2901 7271 0000 0029 0572 7200 0000 725e  ).rq...).rr...r^
-00001f20: 0000 0072 0900 0000 7212 0000 0072 5f00  ...r....r....r_.
-00001f30: 0000 7281 0000 0072 2400 0000 7224 0000  ..r....r$...r$..
-00001f40: 0072 2500 0000 da14 6469 6d65 6e73 696f  .r%.....dimensio
-00001f50: 6e5f 6173 7369 676e 6d65 6e74 1501 0000  n_assignment....
-00001f60: 730e 0000 000e 010a 010c 021e 010c 011a  s...............
-00001f70: 0108 027a 2446 6f61 6d54 7261 6e73 666f  ...z$FoamTransfo
-00001f80: 726d 6572 2e64 696d 656e 7369 6f6e 5f61  rmer.dimension_a
-00001f90: 7373 6967 6e6d 656e 7463 0200 0000 0000  ssignmentc......
-00001fa0: 0000 0000 0000 0300 0000 0300 0000 4300  ..............C.
-00001fb0: 0000 7336 0000 0064 0164 0284 007c 0144  ..s6...d.d...|.D
-00001fc0: 0083 017d 0174 007c 0183 0164 036b 0372  ...}.t.|...d.k.r
-00001fd0: 1174 017c 0183 0182 017c 01a0 0264 04a1  .t.|.....|...d..
-00001fe0: 017d 0274 037c 0264 0583 0253 0029 064e  .}.t.|.d...S.).N
-00001ff0: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
-00002000: 0004 0000 0053 0000 0072 3a00 0000 7227  .....S...r:...r'
-00002010: 0000 0072 2400 0000 7264 0000 0072 2400  ...r$...rd...r$.
-00002020: 0000 7224 0000 0072 2500 0000 723d 0000  ..r$...r%...r=..
-00002030: 0021 0100 0072 3e00 0000 7a34 466f 616d  .!...r>...z4Foam
-00002040: 5472 616e 7366 6f72 6d65 722e 6d61 6372  Transformer.macr
-00002050: 6f5f 6173 7369 676e 6d65 6e74 2e3c 6c6f  o_assignment.<lo
-00002060: 6361 6c73 3e2e 3c6c 6973 7463 6f6d 703e  cals>.<listcomp>
-00002070: 7208 0000 0072 0100 0000 da00 2904 725e  r....r......).r^
-00002080: 0000 0072 8000 0000 7272 0000 0072 0900  ...r....rr...r..
-00002090: 0000 7281 0000 0072 2400 0000 7224 0000  ..r....r$...r$..
-000020a0: 0072 2500 0000 da10 6d61 6372 6f5f 6173  .r%.....macro_as
-000020b0: 7369 676e 6d65 6e74 2001 0000 730a 0000  signment ...s...
-000020c0: 000e 010c 0108 010a 010a 017a 2046 6f61  ...........z Foa
-000020d0: 6d54 7261 6e73 666f 726d 6572 2e6d 6163  mTransformer.mac
-000020e0: 726f 5f61 7373 6967 6e6d 656e 7463 0200  ro_assignmentc..
-000020f0: 0000 0000 0000 0000 0000 0300 0000 0300  ................
-00002100: 0000 4300 0000 734e 0000 0064 0164 0284  ..C...sN...d.d..
-00002110: 007c 0144 0083 017d 0174 007c 0183 0164  .|.D...}.t.|...d
-00002120: 036b 0372 1174 017c 0183 0182 017c 0164  .k.r.t.|.....|.d
-00002130: 0419 007d 0274 027c 0264 0583 0272 1e7c  ...}.t.|.d...r.|
-00002140: 02a0 03a1 007d 027c 0164 0619 009b 0064  .....}.|.d.....d
-00002150: 077c 029b 009d 0353 0029 084e 6301 0000  .|.....S.).Nc...
-00002160: 0000 0000 0000 0000 0002 0000 0004 0000  ................
-00002170: 0053 0000 0072 3a00 0000 7227 0000 0072  .S...r:...r'...r
-00002180: 2400 0000 7264 0000 0072 2400 0000 7224  $...rd...r$...r$
-00002190: 0000 0072 2500 0000 723d 0000 0028 0100  ...r%...r=...(..
-000021a0: 0072 3e00 0000 7a30 466f 616d 5472 616e  .r>...z0FoamTran
-000021b0: 7366 6f72 6d65 722e 6571 7561 6c5f 6173  sformer.equal_as
-000021c0: 7369 676e 2e3c 6c6f 6361 6c73 3e2e 3c6c  sign.<locals>.<l
-000021d0: 6973 7463 6f6d 703e 728c 0000 0072 0800  istcomp>r....r..
-000021e0: 0000 7238 0000 0072 0100 0000 da01 3d29  ..r8...r......=)
-000021f0: 0472 5e00 0000 725f 0000 0072 7c00 0000  .r^...r_...r|...
-00002200: 7238 0000 0029 0372 4600 0000 724e 0000  r8...).rF...rN..
-00002210: 0072 1400 0000 7224 0000 0072 2400 0000  .r....r$...r$...
-00002220: 7225 0000 00da 0c65 7175 616c 5f61 7373  r%.....equal_ass
-00002230: 6967 6e27 0100 0073 0e00 0000 0e01 0c01  ign'...s........
-00002240: 0801 0801 0a01 0801 1201 7a1c 466f 616d  ..........z.Foam
-00002250: 5472 616e 7366 6f72 6d65 722e 6571 7561  Transformer.equa
-00002260: 6c5f 6173 7369 676e 6302 0000 0000 0000  l_assignc.......
-00002270: 0000 0000 0007 0000 0005 0000 0043 0000  .............C..
-00002280: 0073 6e00 0000 6401 6402 8400 7c01 4400  .sn...d.d...|.D.
-00002290: 8301 7d01 7400 7c01 8301 6403 6b02 7212  ..}.t.|...d.k.r.
-000022a0: 7c01 5c02 7d02 7d03 6e17 7c01 a001 6404  |.\.}.}.n.|...d.
-000022b0: a101 7d02 7c01 a001 6404 a101 7d04 6405  ..}.|...d...}.d.
-000022c0: a002 7c01 a101 7d05 7c04 6406 7c05 9b00  ..|...}.|.d.|...
-000022d0: 6407 9d03 1700 7d03 7c02 6408 1700 7c03  d.....}.|.d...|.
-000022e0: 1700 7d06 7403 7c06 7404 7c02 7c03 8302  ..}.t.|.t.|.|...
-000022f0: 8302 5300 2909 4e63 0100 0000 0000 0000  ..S.).Nc........
-00002300: 0000 0000 0200 0000 0400 0000 5300 0000  ............S...
-00002310: 723a 0000 0072 2700 0000 7224 0000 0072  r:...r'...r$...r
-00002320: 6400 0000 7224 0000 0072 2400 0000 7225  d...r$...r$...r%
-00002330: 0000 0072 3d00 0000 3101 0000 723e 0000  ...r=...1...r>..
-00002340: 007a 3846 6f61 6d54 7261 6e73 666f 726d  .z8FoamTransform
-00002350: 6572 2e64 6972 6563 7469 7665 5f61 7373  er.directive_ass
-00002360: 6967 6e6d 656e 742e 3c6c 6f63 616c 733e  ignment.<locals>
-00002370: 2e3c 6c69 7374 636f 6d70 3e72 8c00 0000  .<listcomp>r....
-00002380: 7201 0000 007a 022c 2072 7a00 0000 727b  r....z., rz...r{
-00002390: 0000 0072 6f00 0000 2905 725e 0000 0072  ...ro...).r^...r
-000023a0: 7200 0000 722c 0000 0072 0900 0000 720e  r...r,...r....r.
-000023b0: 0000 0029 0772 4600 0000 724e 0000 0072  ...).rF...rN...r
-000023c0: 6000 0000 da07 636f 6e74 656e 74da 0d66  `.....content..f
-000023d0: 756e 6374 696f 6e5f 6e61 6d65 da09 6172  unction_name..ar
-000023e0: 6775 6d65 6e74 73da 036b 6579 7224 0000  guments..keyr$..
-000023f0: 0072 2400 0000 7225 0000 00da 1464 6972  .r$...r%.....dir
-00002400: 6563 7469 7665 5f61 7373 6967 6e6d 656e  ective_assignmen
-00002410: 7430 0100 0073 1200 0000 0e01 0c01 0a01  t0...s..........
-00002420: 0a02 0a01 0a01 1001 0c01 1001 7a24 466f  ............z$Fo
-00002430: 616d 5472 616e 7366 6f72 6d65 722e 6469  amTransformer.di
-00002440: 7265 6374 6976 655f 6173 7369 676e 6d65  rective_assignme
-00002450: 6e74 6302 0000 0000 0000 0000 0000 0005  ntc.............
-00002460: 0000 0007 0000 0043 0000 0073 ac00 0000  .......C...s....
-00002470: 7400 7c01 8301 7d01 6400 7d02 7401 7c01  t.|...}.d.}.t.|.
-00002480: 8301 6401 6b02 7211 7c01 5c02 7d03 7d04  ..d.k.r.|.\.}.}.
-00002490: 6e19 7401 7c01 8301 6402 6b02 7226 7c01  n.t.|...d.k.r&|.
-000024a0: 5c03 7d03 7d02 7d04 7c02 a002 6403 a101  \.}.}.}.|...d...
-000024b0: 7325 7403 7c01 8301 8201 6e04 7403 7c01  s%t.|.....n.t.|.
-000024c0: 8301 8201 7404 7c04 8301 7d04 7c04 a002  ....t.|...}.|...
-000024d0: 6404 a101 7244 7c04 a005 6405 6406 a102  d...rD|...d.d...
-000024e0: 6407 1900 7d04 7c04 a006 6405 6406 a102  d...}.|...d.d...
-000024f0: 6408 1900 7d04 6e08 7c04 6401 6409 8502  d...}.n.|.d.d...
-00002500: 1900 a007 a100 7d04 7408 7c03 7409 7c03  ......}.t.|.t.|.
-00002510: 7c04 7c02 640a 8d03 8302 5300 290b 4e72  |.|.d.....S.).Nr
-00002520: 8c00 0000 728a 0000 0072 7900 0000 7a03  ....r....ry...z.
-00002530: 237b 0a72 2600 0000 7208 0000 0072 7000  #{.r&...r....rp.
-00002540: 0000 7201 0000 00e9 fdff ffff 2901 7260  ..r.........).r`
-00002550: 0000 0029 0a72 4000 0000 725e 0000 0072  ...).r@...r^...r
-00002560: 7d00 0000 7280 0000 0072 2100 0000 722d  }...r....r!...r-
-00002570: 0000 00da 0672 7370 6c69 74da 0573 7472  .....rsplit..str
-00002580: 6970 7209 0000 0072 0a00 0000 2905 7246  ipr....r....).rF
-00002590: 0000 0072 4e00 0000 7260 0000 0072 1a00  ...rN...r`...r..
-000025a0: 0000 da04 636f 6465 7224 0000 0072 2400  ....coder$...r$.
-000025b0: 0000 7225 0000 00da 0f63 6f64 655f 6173  ..r%.....code_as
-000025c0: 7369 676e 6d65 6e74 3c01 0000 7320 0000  signment<...s ..
-000025d0: 0008 0104 010c 010a 010c 010a 010a 0108  ................
-000025e0: 0102 ff08 0308 010a 0110 0112 0110 0214  ................
-000025f0: 017a 1f46 6f61 6d54 7261 6e73 666f 726d  .z.FoamTransform
-00002600: 6572 2e63 6f64 655f 6173 7369 676e 6d65  er.code_assignme
-00002610: 6e74 6302 0000 0000 0000 0000 0000 0002  ntc.............
-00002620: 0000 0003 0000 0043 0000 0073 1a00 0000  .......C...s....
-00002630: 7400 7c01 8301 7d01 7401 7c01 6401 1900  t.|...}.t.|.d...
-00002640: 6a02 6402 1700 8301 5300 2903 4e72 0100  j.d.....S.).Nr..
-00002650: 0000 7226 0000 0029 0372 4000 0000 7211  ..r&...).r@...r.
-00002660: 0000 0072 1400 0000 7245 0000 0072 2400  ...r....rE...r$.
-00002670: 0000 7224 0000 0072 2500 0000 da12 7370  ..r$...r%.....sp
-00002680: 6563 6961 6c5f 6469 7265 6374 6976 6573  ecial_directives
-00002690: 4f01 0000 7304 0000 0008 0112 017a 2246  O...s........z"F
-000026a0: 6f61 6d54 7261 6e73 666f 726d 6572 2e73  oamTransformer.s
-000026b0: 7065 6369 616c 5f64 6972 6563 7469 7665  pecial_directive
-000026c0: 734e 291a 721e 0000 0072 1f00 0000 7220  sN).r....r....r 
-000026d0: 0000 0072 4800 0000 724b 0000 0072 4f00  ...rH...rK...rO.
-000026e0: 0000 7250 0000 0072 5100 0000 7252 0000  ..rP...rQ...rR..
-000026f0: 0072 5300 0000 7254 0000 0072 5b00 0000  .rS...rT...r[...
-00002700: 7260 0000 0072 6100 0000 726a 0000 0072  r`...ra...rj...r
-00002710: 7700 0000 727f 0000 0072 8200 0000 7286  w...r....r....r.
-00002720: 0000 0072 8900 0000 728d 0000 0072 8f00  ...r....r....r..
-00002730: 0000 7291 0000 0072 9600 0000 729b 0000  ..r....r....r...
-00002740: 0072 9c00 0000 7224 0000 0072 2400 0000  .r....r$...r$...
-00002750: 7224 0000 0072 2500 0000 7233 0000 004a  r$...r%...r3...J
-00002760: 0000 0073 3000 0000 0800 0801 0803 0803  ...s0...........
-00002770: 0803 0803 0803 0803 0803 0803 0809 0805  ................
-00002780: 080a 080e 0827 082d 0807 0817 081a 080b  .....'.-........
-00002790: 0807 0809 080c 0c13 7233 0000 0072 2700  ........r3...r'.
-000027a0: 0000 2927 da07 5f5f 646f 635f 5fda 0b64  ..)'..__doc__..d
-000027b0: 6174 6163 6c61 7373 6573 7202 0000 00da  ataclassesr.....
-000027c0: 0770 6174 686c 6962 7203 0000 005a 046c  .pathlibr....Z.l
-000027d0: 6172 6b72 0400 0000 7205 0000 0072 0600  arkr....r....r..
-000027e0: 0000 5a0f 6c61 726b 2e65 7863 6570 7469  ..Z.lark.excepti
-000027f0: 6f6e 7372 0700 0000 da03 6173 7472 0900  onsr......astr..
-00002800: 0000 720a 0000 0072 0b00 0000 720c 0000  ..r....r....r...
-00002810: 0072 0d00 0000 720e 0000 0072 0f00 0000  .r....r....r....
-00002820: 7210 0000 0072 1100 0000 7212 0000 0072  r....r....r....r
-00002830: 1300 0000 da08 5f5f 6669 6c65 5f5f da08  ......__file__..
-00002840: 6162 736f 6c75 7465 da06 7061 7265 6e74  absolute..parent
-00002850: da04 6865 7265 da09 7265 6164 5f74 6578  ..here..read_tex
-00002860: 7472 3600 0000 5a10 6772 616d 6d61 725f  tr6...Z.grammar_
-00002870: 6164 7661 6e63 6564 722f 0000 0072 3100  advancedr/...r1.
-00002880: 0000 7232 0000 0072 1900 0000 7230 0000  ..r2...r....r0..
-00002890: 0072 3800 0000 7240 0000 0072 4400 0000  .r8...r@...rD...
-000028a0: 7233 0000 0072 2400 0000 7224 0000 0072  r3...r$...r$...r
-000028b0: 2400 0000 7225 0000 00da 083c 6d6f 6475  $...r%.....<modu
-000028c0: 6c65 3e01 0000 0073 2600 0000 0400 0c02  le>....s&.......
-000028d0: 0c01 1402 0c01 3402 0e0e 0c02 0c01 0e02  ......4.........
-000028e0: 0e01 0a02 0203 1001 0a07 0810 0804 0804  ................
-000028f0: 1408                                     ..
+00000340: 0000 00fa 492f 686f 6d65 2f70 6965 7272  ....I/home/pierr
+00000350: 652f 4465 762f 666c 7569 6473 696d 666f  e/Dev/fluidsimfo
+00000360: 616d 2f73 7263 2f66 6c75 6964 7369 6d66  am/src/fluidsimf
+00000370: 6f61 6d2f 666f 616d 5f69 6e70 7574 5f66  oam/foam_input_f
+00000380: 696c 6573 2f70 6172 7365 722e 7079 7219  iles/parser.pyr.
+00000390: 0000 0022 0000 0073 0a00 0000 0a00 0802  ..."...s........
+000003a0: 0c01 0c01 1001 7219 0000 004e 6302 0000  ......r....Nc...
+000003b0: 0000 0000 0000 0000 0003 0000 0008 0000  ................
+000003c0: 0043 0000 0073 7a00 0000 6401 a000 6402  .C...sz...d...d.
+000003d0: 6403 8400 7c00 a001 6401 a101 4400 8301  d...|...d...D...
+000003e0: a101 7d00 7c00 a002 6401 a101 7316 7c00  ..}.|...d...s.|.
+000003f0: 6401 3700 7d00 7c01 6400 7500 7230 7a07  d.7.}.|.d.u.r0z.
+00000400: 7403 a004 7c00 a101 7d02 5700 6e15 0400  t...|...}.W.n...
+00000410: 7405 792f 0100 0100 0100 7406 a004 7c00  t.y/......t...|.
+00000420: a101 7d02 5900 6e08 7700 7407 7c01 1900  ..}.Y.n.w.t.|...
+00000430: a004 7c00 a101 7d02 7408 8300 a009 7c02  ..|...}.t.....|.
+00000440: a101 5300 2904 4eda 010a 6301 0000 0000  ..S.).N...c.....
+00000450: 0000 0000 0000 0002 0000 0003 0000 0073  ...............s
+00000460: 0000 0073 1800 0000 8100 7c00 5d07 7d01  ...s......|.].}.
+00000470: 7c01 a000 a100 5600 0100 7102 6400 5300  |.....V...q.d.S.
+00000480: a901 4e29 01da 0672 7374 7269 7029 02da  ..N)...rstrip)..
+00000490: 022e 30da 046c 696e 6572 2400 0000 7224  ..0..liner$...r$
+000004a0: 0000 0072 2500 0000 da09 3c67 656e 6578  ...r%.....<genex
+000004b0: 7072 3e2b 0000 0073 0400 0000 0280 1600  pr>+...s........
+000004c0: 7a18 7061 7273 652e 3c6c 6f63 616c 733e  z.parse.<locals>
+000004d0: 2e3c 6765 6e65 7870 723e 290a da04 6a6f  .<genexpr>)...jo
+000004e0: 696e da05 7370 6c69 74da 0865 6e64 7377  in..split..endsw
+000004f0: 6974 68da 0b6c 6172 6b5f 7061 7273 6572  ith..lark_parser
+00000500: da05 7061 7273 6572 0700 0000 da14 6c61  ..parser......la
+00000510: 726b 5f70 6172 7365 725f 6164 7661 6e63  rk_parser_advanc
+00000520: 6564 da07 7061 7273 6572 73da 0f46 6f61  ed..parsers..Foa
+00000530: 6d54 7261 6e73 666f 726d 6572 da09 7472  mTransformer..tr
+00000540: 616e 7366 6f72 6d29 03da 0474 6578 74da  ansform)...text.
+00000550: 0767 7261 6d6d 6172 da04 7472 6565 7224  .grammar..treer$
+00000560: 0000 0072 2400 0000 7225 0000 0072 3000  ...r$...r%...r0.
+00000570: 0000 2a00 0000 7316 0000 001a 010a 0108  ..*...s.........
+00000580: 0108 0202 010e 010c 010e 0102 ff0e 030c  ................
+00000590: 0272 3000 0000 6301 0000 0000 0000 0000  .r0...c.........
+000005a0: 0000 0001 0000 0002 0000 0043 0000 0073  ...........C...s
+000005b0: 0800 0000 7c00 a000 a100 5300 7227 0000  ....|.....S.r'..
+000005c0: 0029 01da 0464 756d 7029 0172 3700 0000  .)...dump).r7...
+000005d0: 7224 0000 0072 2400 0000 7225 0000 0072  r$...r$...r%...r
+000005e0: 3800 0000 3a00 0000 f302 0000 0008 0172  8...:..........r
+000005f0: 3800 0000 6301 0000 0000 0000 0000 0000  8...c...........
+00000600: 0001 0000 0002 0000 0043 0000 0073 0e00  .........C...s..
+00000610: 0000 6401 6402 8400 7c00 4400 8301 5300  ..d.d...|.D...S.
+00000620: 2903 4e63 0100 0000 0000 0000 0000 0000  ).Nc............
+00000630: 0200 0000 0400 0000 5300 0000 f318 0000  ........S.......
+00000640: 0067 007c 005d 087d 017c 0164 0075 0172  .g.|.].}.|.d.u.r
+00000650: 027c 0191 0271 0253 0072 2700 0000 7224  .|...q.S.r'...r$
+00000660: 0000 00a9 0272 2900 0000 da04 6974 656d  .....r).....item
+00000670: 7224 0000 0072 2400 0000 7225 0000 00da  r$...r$...r%....
+00000680: 0a3c 6c69 7374 636f 6d70 3e3f 0000 00f3  .<listcomp>?....
+00000690: 0200 0000 1800 7a26 6669 6c74 6572 5f6e  ......z&filter_n
+000006a0: 6f5f 6e65 776c 696e 6573 2e3c 6c6f 6361  o_newlines.<loca
+000006b0: 6c73 3e2e 3c6c 6973 7463 6f6d 703e 7224  ls>.<listcomp>r$
+000006c0: 0000 0029 01da 0569 7465 6d73 7224 0000  ...)...itemsr$..
+000006d0: 0072 2400 0000 7225 0000 00da 1266 696c  .r$...r%.....fil
+000006e0: 7465 725f 6e6f 5f6e 6577 6c69 6e65 733e  ter_no_newlines>
+000006f0: 0000 0073 0200 0000 0e01 7240 0000 0063  ...s......r@...c
+00000700: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+00000710: 0800 0000 4300 0000 732e 0000 0074 007c  ....C...s....t.|
+00000720: 0083 017d 007a 0574 017c 0083 0157 0053  ...}.z.t.|...W.S
+00000730: 0004 0074 0279 1601 0001 0001 0074 037c  ...t.y.......t.|
+00000740: 0083 0106 0059 0053 0077 0072 2700 0000  .....Y.S.w.r'...
+00000750: 2904 7221 0000 0072 2300 0000 da0a 5661  ).r!...r#.....Va
+00000760: 6c75 6545 7272 6f72 da05 666c 6f61 7429  lueError..float)
+00000770: 01da 066e 756d 6265 7272 2400 0000 7224  ...numberr$...r$
+00000780: 0000 0072 2500 0000 da12 5f63 6f6e 7665  ...r%....._conve
+00000790: 7274 5f74 6f5f 6e75 6d62 6572 4200 0000  rt_to_numberB...
+000007a0: 730c 0000 0008 0102 010a 010c 010c 0102  s...............
+000007b0: ff72 4400 0000 6300 0000 0000 0000 0000  .rD...c.........
+000007c0: 0000 0000 0000 0002 0000 0040 0000 0073  ...........@...s
+000007d0: c400 0000 6500 5a01 6400 5a02 6401 6402  ....e.Z.d.Z.d.d.
+000007e0: 8400 5a03 6403 6404 8400 5a04 6405 6406  ..Z.d.d...Z.d.d.
+000007f0: 8400 5a05 6407 6408 8400 5a06 6409 640a  ..Z.d.d...Z.d.d.
+00000800: 8400 5a07 640b 640c 8400 5a08 640d 640e  ..Z.d.d...Z.d.d.
+00000810: 8400 5a09 640f 6410 8400 5a0a 6411 6412  ..Z.d.d...Z.d.d.
+00000820: 8400 5a0b 6413 6414 8400 5a0c 6415 6416  ..Z.d.d...Z.d.d.
+00000830: 8400 5a0d 6417 6418 8400 5a0e 6419 641a  ..Z.d.d...Z.d.d.
+00000840: 8400 5a0f 641b 641c 8400 5a10 641d 641e  ..Z.d.d...Z.d.d.
+00000850: 8400 5a11 641f 6420 8400 5a12 6421 6422  ..Z.d.d ..Z.d!d"
+00000860: 8400 5a13 6423 6424 8400 5a14 6425 6426  ..Z.d#d$..Z.d%d&
+00000870: 8400 5a15 6427 6428 8400 5a16 6429 642a  ..Z.d'd(..Z.d)d*
+00000880: 8400 5a17 642b 642c 8400 5a18 642d 642e  ..Z.d+d,..Z.d-d.
+00000890: 8400 5a19 642f 5300 2930 7233 0000 0063  ..Z.d/S.)0r3...c
+000008a0: 0200 0000 0000 0000 0000 0000 0200 0000  ................
+000008b0: 0200 0000 4300 0000 7308 0000 0074 007c  ....C...s....t.|
+000008c0: 0183 0153 0072 2700 0000 2901 7244 0000  ...S.r'...).rD..
+000008d0: 00a9 02da 0473 656c 66da 0574 6f6b 656e  .....self..token
+000008e0: 7224 0000 0072 2400 0000 7225 0000 00da  r$...r$...r%....
+000008f0: 0d53 4947 4e45 445f 4e55 4d42 4552 4b00  .SIGNED_NUMBERK.
+00000900: 0000 7239 0000 007a 1d46 6f61 6d54 7261  ..r9...z.FoamTra
+00000910: 6e73 666f 726d 6572 2e53 4947 4e45 445f  nsformer.SIGNED_
+00000920: 4e55 4d42 4552 6302 0000 0000 0000 0000  NUMBERc.........
+00000930: 0000 0002 0000 0001 0000 0043 0000 00f3  ...........C....
+00000940: 0600 0000 7c01 6a00 5300 7227 0000 00a9  ....|.j.S.r'....
+00000950: 0172 1400 0000 7245 0000 0072 2400 0000  .r....rE...r$...
+00000960: 7224 0000 0072 2500 0000 da05 434e 414d  r$...r%.....CNAM
+00000970: 454e 0000 00f3 0200 0000 0601 7a15 466f  EN..........z.Fo
+00000980: 616d 5472 616e 7366 6f72 6d65 722e 434e  amTransformer.CN
+00000990: 414d 4563 0200 0000 0000 0000 0000 0000  AMEc............
+000009a0: 0200 0000 0100 0000 4300 0000 7304 0000  ........C...s...
+000009b0: 0064 0053 0072 2700 0000 7224 0000 00a9  .d.S.r'...r$....
+000009c0: 0272 4600 0000 da05 6e6f 6465 7372 2400  .rF.....nodesr$.
+000009d0: 0000 7224 0000 0072 2500 0000 da07 4e45  ..r$...r%.....NE
+000009e0: 574c 494e 4551 0000 0073 0200 0000 0401  WLINEQ...s......
+000009f0: 7a17 466f 616d 5472 616e 7366 6f72 6d65  z.FoamTransforme
+00000a00: 722e 4e45 574c 494e 4563 0200 0000 0000  r.NEWLINEc......
+00000a10: 0000 0000 0000 0200 0000 0100 0000 4300  ..............C.
+00000a20: 0000 7249 0000 0072 2700 0000 724a 0000  ..rI...r'...rJ..
+00000a30: 0072 4500 0000 7224 0000 0072 2400 0000  .rE...r$...r$...
+00000a40: 7225 0000 00da 0e45 5343 4150 4544 5f53  r%.....ESCAPED_S
+00000a50: 5452 494e 4754 0000 0072 4c00 0000 7a1e  TRINGT...rL...z.
+00000a60: 466f 616d 5472 616e 7366 6f72 6d65 722e  FoamTransformer.
+00000a70: 4553 4341 5045 445f 5354 5249 4e47 6302  ESCAPED_STRINGc.
+00000a80: 0000 0000 0000 0000 0000 0002 0000 0001  ................
+00000a90: 0000 0043 0000 0072 4900 0000 7227 0000  ...C...rI...r'..
+00000aa0: 0072 4a00 0000 7245 0000 0072 2400 0000  .rJ...rE...r$...
+00000ab0: 7224 0000 0072 2500 0000 da0b 444f 5542  r$...r%.....DOUB
+00000ac0: 4c45 5f4e 414d 4557 0000 0072 4c00 0000  LE_NAMEW...rL...
+00000ad0: 7a1b 466f 616d 5472 616e 7366 6f72 6d65  z.FoamTransforme
+00000ae0: 722e 444f 5542 4c45 5f4e 414d 4563 0200  r.DOUBLE_NAMEc..
+00000af0: 0000 0000 0000 0000 0000 0200 0000 0100  ................
+00000b00: 0000 4300 0000 7249 0000 0072 2700 0000  ..C...rI...r'...
+00000b10: 724a 0000 0072 4500 0000 7224 0000 0072  rJ...rE...r$...r
+00000b20: 2400 0000 7225 0000 00da 0b54 5249 504c  $...r%.....TRIPL
+00000b30: 455f 4e41 4d45 5a00 0000 724c 0000 007a  E_NAMEZ...rL...z
+00000b40: 1b46 6f61 6d54 7261 6e73 666f 726d 6572  .FoamTransformer
+00000b50: 2e54 5249 504c 455f 4e41 4d45 6302 0000  .TRIPLE_NAMEc...
+00000b60: 0000 0000 0000 0000 0002 0000 0001 0000  ................
+00000b70: 0043 0000 0072 4900 0000 7227 0000 0072  .C...rI...r'...r
+00000b80: 4a00 0000 7245 0000 0072 2400 0000 7224  J...rE...r$...r$
+00000b90: 0000 0072 2500 0000 da05 4551 4b45 595d  ...r%.....EQKEY]
+00000ba0: 0000 0072 4c00 0000 7a15 466f 616d 5472  ...rL...z.FoamTr
+00000bb0: 616e 7366 6f72 6d65 722e 4551 4b45 5963  ansformer.EQKEYc
+00000bc0: 0200 0000 0000 0000 0000 0000 0200 0000  ................
+00000bd0: 0100 0000 4300 0000 7249 0000 0072 2700  ....C...rI...r'.
+00000be0: 0000 724a 0000 0072 4500 0000 7224 0000  ..rJ...rE...r$..
+00000bf0: 0072 2400 0000 7225 0000 00da 054d 4143  .r$...r%.....MAC
+00000c00: 524f 6000 0000 724c 0000 007a 1546 6f61  RO`...rL...z.Foa
+00000c10: 6d54 7261 6e73 666f 726d 6572 2e4d 4143  mTransformer.MAC
+00000c20: 524f 6302 0000 0000 0000 0000 0000 0002  ROc.............
+00000c30: 0000 0003 0000 0043 0000 00f3 1200 0000  .......C........
+00000c40: 7400 6401 6402 8400 7c01 4400 8301 8301  t.d.d...|.D.....
+00000c50: 5300 2903 4e63 0100 0000 0000 0000 0000  S.).Nc..........
+00000c60: 0000 0200 0000 0500 0000 5300 0000 7324  ..........S...s$
+00000c70: 0000 0067 007c 005d 0e7d 0174 007c 0174  ...g.|.].}.t.|.t
+00000c80: 0183 0272 0e7c 016a 0264 006b 0273 027c  ...r.|.j.d.k.s.|
+00000c90: 0191 0271 0253 0029 0172 4f00 0000 a903  ...q.S.).rO.....
+00000ca0: da0a 6973 696e 7374 616e 6365 7205 0000  ..isinstancer...
+00000cb0: 00da 0474 7970 6572 3b00 0000 7224 0000  ...typer;...r$..
+00000cc0: 0072 2400 0000 7225 0000 0072 3d00 0000  .r$...r%...r=...
+00000cd0: 6500 0000 f310 0000 0006 0002 0208 0102  e...............
+00000ce0: fd08 0302 fd02 0106 ff7a 3146 6f61 6d54  .........z1FoamT
+00000cf0: 7261 6e73 666f 726d 6572 2e64 696d 656e  ransformer.dimen
+00000d00: 7369 6f6e 5f73 6574 2e3c 6c6f 6361 6c73  sion_set.<locals
+00000d10: 3e2e 3c6c 6973 7463 6f6d 703e 2901 720d  >.<listcomp>).r.
+00000d20: 0000 00a9 0272 4600 0000 723f 0000 0072  .....rF...r?...r
+00000d30: 2400 0000 7224 0000 0072 2500 0000 da0d  $...r$...r%.....
+00000d40: 6469 6d65 6e73 696f 6e5f 7365 7463 0000  dimension_setc..
+00000d50: 00f3 0a00 0000 0201 0601 0202 04fe 04ff  ................
+00000d60: 7a1d 466f 616d 5472 616e 7366 6f72 6d65  z.FoamTransforme
+00000d70: 722e 6469 6d65 6e73 696f 6e5f 7365 7463  r.dimension_setc
+00000d80: 0200 0000 0000 0000 0000 0000 0200 0000  ................
+00000d90: 0300 0000 4300 0000 731c 0000 0074 007c  ....C...s....t.|
+00000da0: 0183 0164 016b 0372 0874 0182 0174 027c  ...d.k.r.t...t.|
+00000db0: 0164 0219 0083 0153 00a9 034e 7208 0000  .d.....S...Nr...
+00000dc0: 0072 0100 0000 2903 da03 6c65 6eda 0c52  .r....)...len..R
+00000dd0: 756e 7469 6d65 4572 726f 7272 2100 0000  untimeErrorr!...
+00000de0: 724d 0000 0072 2400 0000 7224 0000 0072  rM...r$...r$...r
+00000df0: 2500 0000 da09 6469 7265 6374 6976 656c  %.....directivel
+00000e00: 0000 0073 0600 0000 0c01 0401 0c01 7a19  ...s..........z.
+00000e10: 466f 616d 5472 616e 7366 6f72 6d65 722e  FoamTransformer.
+00000e20: 6469 7265 6374 6976 6563 0200 0000 0000  directivec......
+00000e30: 0000 0000 0000 0200 0000 0300 0000 4300  ..............C.
+00000e40: 0000 7255 0000 0029 034e 6301 0000 0000  ..rU...).Nc.....
+00000e50: 0000 0000 0000 0002 0000 0005 0000 0053  ...............S
+00000e60: 0000 0073 2c00 0000 6700 7c00 5d12 7d01  ...s,...g.|.].}.
+00000e70: 7400 7c01 7401 8302 720e 7c01 6a02 6400  t.|.t...r.|.j.d.
+00000e80: 6b02 7302 7c01 6401 7501 7202 7c01 9102  k.s.|.d.u.r.|...
+00000e90: 7102 5300 2902 724f 0000 004e 7256 0000  q.S.).rO...NrV..
+00000ea0: 0072 3b00 0000 7224 0000 0072 2400 0000  .r;...r$...r$...
+00000eb0: 7225 0000 0072 3d00 0000 7300 0000 7314  r%...r=...s...s.
+00000ec0: 0000 0006 0002 0208 0102 fd08 0302 fd06  ................
+00000ed0: 0402 fc02 0106 ff7a 2846 6f61 6d54 7261  .......z(FoamTra
+00000ee0: 6e73 666f 726d 6572 2e6c 6973 742e 3c6c  nsformer.list.<l
+00000ef0: 6f63 616c 733e 2e3c 6c69 7374 636f 6d70  ocals>.<listcomp
+00000f00: 3e29 0172 1000 0000 725a 0000 0072 2400  >).r....rZ...r$.
+00000f10: 0000 7224 0000 0072 2500 0000 da04 6c69  ..r$...r%.....li
+00000f20: 7374 7100 0000 725c 0000 007a 1446 6f61  stq...r\...z.Foa
+00000f30: 6d54 7261 6e73 666f 726d 6572 2e6c 6973  mTransformer.lis
+00000f40: 7463 0200 0000 0000 0000 0000 0000 0500  tc..............
+00000f50: 0000 0400 0000 4300 0000 7362 0000 007c  ......C...sb...|
+00000f60: 0164 0119 007d 027c 026a 0064 026b 0272  .d...}.|.j.d.k.r
+00000f70: 137c 026a 017d 037c 0164 0364 0085 0219  .|.j.}.|.d.d....
+00000f80: 007d 016e 0264 007d 037c 0144 005d 0f7d  .}.n.d.}.|.D.].}
+00000f90: 0474 027c 046a 0174 0383 0272 267c 046a  .t.|.j.t...r&|.j
+00000fa0: 01a0 047c 046a 00a1 0101 0071 1774 057c  ...|.j.....q.t.|
+00000fb0: 0364 0464 0584 007c 0144 0083 0183 0253  .d.d...|.D.....S
+00000fc0: 0029 064e 7201 0000 005a 0846 6f61 6d46  .).Nr....Z.FoamF
+00000fd0: 696c 6572 0800 0000 6301 0000 0000 0000  iler....c.......
+00000fe0: 0000 0000 0002 0000 0004 0000 0053 0000  .............S..
+00000ff0: 00f3 1600 0000 6900 7c00 5d07 7d01 7c01  ......i.|.].}.|.
+00001000: 6a00 7c01 6a01 9302 7102 5300 7224 0000  j.|.j...q.S.r$..
+00001010: 00a9 0272 1a00 0000 7214 0000 00a9 0272  ...r....r......r
+00001020: 2900 0000 da04 6e6f 6465 7224 0000 0072  ).....noder$...r
+00001030: 2400 0000 7225 0000 00da 0a3c 6469 6374  $...r%.....<dict
+00001040: 636f 6d70 3e87 0000 00f3 0200 0000 1600  comp>...........
+00001050: 7a28 466f 616d 5472 616e 7366 6f72 6d65  z(FoamTransforme
+00001060: 722e 6669 6c65 2e3c 6c6f 6361 6c73 3e2e  r.file.<locals>.
+00001070: 3c64 6963 7463 6f6d 703e 2906 721a 0000  <dictcomp>).r...
+00001080: 0072 1400 0000 7257 0000 0072 1000 0000  .r....rW...r....
+00001090: da08 6164 645f 6e61 6d65 720f 0000 0029  ..add_namer....)
+000010a0: 0572 4600 0000 724e 0000 005a 1066 6972  .rF...rN...Z.fir
+000010b0: 7374 5f61 7373 6967 6e6d 656e 74da 0969  st_assignment..i
+000010c0: 6e66 6f5f 6469 6374 7265 0000 0072 2400  nfo_dictre...r$.
+000010d0: 0000 7224 0000 0072 2500 0000 da04 6669  ..r$...r%.....fi
+000010e0: 6c65 7b00 0000 7314 0000 0008 010a 0106  le{...s.........
+000010f0: 010e 0104 0208 020c 010e 0102 8014 027a  ...............z
+00001100: 1446 6f61 6d54 7261 6e73 666f 726d 6572  .FoamTransformer
+00001110: 2e66 696c 6563 0200 0000 0000 0000 0000  .filec..........
+00001120: 0000 0800 0000 0800 0000 4300 0000 7312  ..........C...s.
+00001130: 0100 0064 0164 0284 007c 0144 0083 017d  ...d.d...|.D...}
+00001140: 0164 007d 0264 007d 037c 01a0 0064 03a1  .d.}.d.}.|...d..
+00001150: 017d 0474 017c 0183 0164 046b 0272 1b7c  .}.t.|...d.k.r.|
+00001160: 0164 0319 007d 056e 697a 0c64 0564 0284  .d...}.niz.d.d..
+00001170: 007c 0144 0083 01a0 0264 06a1 017d 0657  .|.D.....d...}.W
+00001180: 006e 0b04 0074 0379 3201 0001 0001 0064  .n...t.y2......d
+00001190: 007d 0259 006e 0677 007c 01a0 007c 06a1  .}.Y.n.w.|...|..
+000011a0: 017d 0264 007d 0374 0464 0764 0284 007c  .}.d.}.t.d.d...|
+000011b0: 0144 0083 0183 0172 4964 08a0 057c 01a1  .D.....rId...|..
+000011c0: 017d 076e 247c 01a0 0064 09a1 017d 0774  .}.n$|...d...}.t
+000011d0: 0464 0a64 0b84 007c 0144 0083 0183 0173  .d.d...|.D.....s
+000011e0: 5e64 0c64 0284 007c 0144 0083 017d 017c  ^d.d...|.D...}.|
+000011f0: 0172 6564 08a0 057c 01a1 017d 0374 067c  .red...|...}.t.|
+00001200: 0774 0783 0272 6d7c 037c 075f 087c 0364  .t...rm|.|._.|.d
+00001210: 0075 0072 757c 0264 0075 0073 7a74 067c  .u.ru|.d.u.szt.|
+00001220: 0774 0783 0272 7d7c 077d 056e 0774 097c  .t...r}|.}.n.t.|
+00001230: 077c 037c 0264 0d8d 037d 0574 0a7c 047c  .|.|.d...}.t.|.|
+00001240: 0583 0253 0029 0e4e 6301 0000 0000 0000  ...S.).Nc.......
+00001250: 0000 0000 0002 0000 0004 0000 0053 0000  .............S..
+00001260: 0072 3a00 0000 7227 0000 0072 2400 0000  .r:...r'...r$...
+00001270: 7264 0000 0072 2400 0000 7224 0000 0072  rd...r$...r$...r
+00001280: 2500 0000 723d 0000 008a 0000 0072 3e00  %...r=.......r>.
+00001290: 0000 7a32 466f 616d 5472 616e 7366 6f72  ..z2FoamTransfor
+000012a0: 6d65 722e 7661 725f 6173 7369 676e 6d65  mer.var_assignme
+000012b0: 6e74 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973  nt.<locals>.<lis
+000012c0: 7463 6f6d 703e 7201 0000 0072 0800 0000  tcomp>r....r....
+000012d0: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
+000012e0: 0005 0000 0053 0000 00f3 1600 0000 6700  .....S........g.
+000012f0: 7c00 5d07 7d01 7400 7c01 7401 8302 9102  |.].}.t.|.t.....
+00001300: 7102 5300 7224 0000 0029 0272 5700 0000  q.S.r$...).rW...
+00001310: 720d 0000 00a9 0272 2900 0000 da04 656c  r......r).....el
+00001320: 656d 7224 0000 0072 2400 0000 7225 0000  emr$...r$...r%..
+00001330: 0072 3d00 0000 9200 0000 7306 0000 0006  .r=.......s.....
+00001340: 000a 0106 ff54 6301 0000 0000 0000 0000  .....Tc.........
+00001350: 0000 0002 0000 0005 0000 0053 0000 0072  ...........S...r
+00001360: 6b00 0000 7224 0000 00a9 0272 5700 0000  k...r$.....rW...
+00001370: 7221 0000 0072 6c00 0000 7224 0000 0072  r!...rl...r$...r
+00001380: 2400 0000 7225 0000 0072 3d00 0000 9b00  $...r%...r=.....
+00001390: 0000 7267 0000 00da 0120 e9ff ffff ff63  ..rg..... .....c
+000013a0: 0100 0000 0000 0000 0000 0000 0200 0000  ................
+000013b0: 0400 0000 7300 0000 731a 0000 0081 007c  ....s...s......|
+000013c0: 005d 087d 0174 007c 0174 0183 0256 0001  .].}.t.|.t...V..
+000013d0: 0071 0264 0053 0072 2700 0000 726e 0000  .q.d.S.r'...rn..
+000013e0: 0072 6400 0000 7224 0000 0072 2400 0000  .rd...r$...r$...
+000013f0: 7225 0000 0072 2b00 0000 9f00 0000 7304  r%...r+.......s.
+00001400: 0000 0002 8018 007a 3146 6f61 6d54 7261  .......z1FoamTra
+00001410: 6e73 666f 726d 6572 2e76 6172 5f61 7373  nsformer.var_ass
+00001420: 6967 6e6d 656e 742e 3c6c 6f63 616c 733e  ignment.<locals>
+00001430: 2e3c 6765 6e65 7870 723e 6301 0000 0000  .<genexpr>c.....
+00001440: 0000 0000 0000 0002 0000 0004 0000 0053  ...............S
+00001450: 0000 0073 1400 0000 6700 7c00 5d06 7d01  ...s....g.|.].}.
+00001460: 7400 7c01 8301 9102 7102 5300 7224 0000  t.|.....q.S.r$..
+00001470: 0029 0172 2100 0000 7264 0000 0072 2400  .).r!...rd...r$.
+00001480: 0000 7224 0000 0072 2500 0000 723d 0000  ..r$...r%...r=..
+00001490: 00a0 0000 0073 0200 0000 1400 2902 721a  .....s......).r.
+000014a0: 0000 00da 0964 696d 656e 7369 6f6e 290b  .....dimension).
+000014b0: da03 706f 7072 5e00 0000 da05 696e 6465  ..popr^.....inde
+000014c0: 7872 4100 0000 da03 616c 6c72 2c00 0000  xrA.....allr,...
+000014d0: 7257 0000 0072 1000 0000 da05 5f6e 616d  rW...r......_nam
+000014e0: 6572 1200 0000 7213 0000 0029 0872 4600  er....r....).rF.
+000014f0: 0000 724e 0000 0072 5b00 0000 5a0d 6e61  ..rN...r[...Z.na
+00001500: 6d65 5f69 6e5f 7661 6c75 6572 1a00 0000  me_in_valuer....
+00001510: 7214 0000 005a 0f69 6e64 6578 5f64 696d  r....Z.index_dim
+00001520: 656e 7369 6f6e da0a 6c61 7374 5f76 616c  ension..last_val
+00001530: 7565 7224 0000 0072 2400 0000 7225 0000  uer$...r$...r%..
+00001540: 00da 0e76 6172 5f61 7373 6967 6e6d 656e  ...var_assignmen
+00001550: 7489 0000 0073 4400 0000 0e01 0401 0401  t....sD.........
+00001560: 0a01 0c01 0a01 0202 0601 0201 04ff 0602  ................
+00001570: 06fe 0c03 0801 02ff 0a03 0402 1201 0c01  ................
+00001580: 0a02 1201 0e01 0401 0a01 0a01 0601 1202  ................
+00001590: 0401 04ff 0603 0202 0601 06ff 0a03 7a1e  ..............z.
+000015a0: 466f 616d 5472 616e 7366 6f72 6d65 722e  FoamTransformer.
+000015b0: 7661 725f 6173 7369 676e 6d65 6e74 6302  var_assignmentc.
+000015c0: 0000 0000 0000 0000 0000 0008 0000 0007  ................
+000015d0: 0000 0043 0000 0073 1601 0000 7400 7c01  ...C...s....t.|.
+000015e0: 8301 7d01 6400 7d02 7401 7c01 8301 6401  ..}.d.}.t.|...d.
+000015f0: 6b02 721a 7c01 a002 6402 a101 7d03 7403  k.r.|...d...}.t.
+00001600: 7c03 7404 6900 7c03 6403 8d02 8302 5300  |.t.i.|.d.....S.
+00001610: 6700 7d04 7c01 4400 5d13 7d05 7405 7c05  g.}.|.D.].}.t.|.
+00001620: 7406 8302 7231 7c05 a007 6404 a101 7231  t...r1|...d...r1
+00001630: 7c01 a002 6401 a101 7d02 0100 6e01 711e  |...d...}...n.q.
+00001640: 7405 7c01 6402 1900 7408 8302 7246 6405  t.|.d...t...rFd.
+00001650: 6406 a009 7c01 a002 6402 a101 a101 1700  d...|...d.......
+00001660: 6407 1700 7d03 6e05 7c01 a002 6402 a101  d...}.n.|...d...
+00001670: 7d03 7c04 7256 7c03 6406 6406 a009 7c04  }.|.rV|.d.d...|.
+00001680: a101 1700 3700 7d03 6408 6409 8400 7c01  ....7.}.d.d...|.
+00001690: 4400 8301 7d06 7c06 4400 5d0f 7d05 7405  D...}.|.D.].}.t.
+000016a0: 7c05 6a0a 740b 8302 726e 7c05 6a0a a00c  |.j.t...rn|.j...
+000016b0: 7c05 6a0d a101 0100 715f 7c02 6400 7501  |.j.....q_|.d.u.
+000016c0: 727a 7c02 640a 6b02 727a 740e 7d07 6e02  rz|.d.k.rzt.}.n.
+000016d0: 7404 7d07 7403 7c03 7c07 640b 640c 8400  t.}.t.|.|.d.d...
+000016e0: 7c06 4400 8301 7c03 7c02 640d 8d03 8302  |.D...|.|.d.....
+000016f0: 5300 290e 4e72 0800 0000 7201 0000 0029  S.).Nr....r....)
+00001700: 02da 0464 6174 6172 1a00 0000 fa01 23fa  ...datar......#.
+00001710: 0128 726f 0000 00fa 0129 6301 0000 0000  .(ro.....)c.....
+00001720: 0000 0000 0000 0002 0000 0005 0000 0053  ...............S
+00001730: 0000 0073 2400 0000 6700 7c00 5d0e 7d01  ...s$...g.|.].}.
+00001740: 7400 7c01 6400 8302 7202 7400 7c01 6401  t.|.d...r.t.|.d.
+00001750: 8302 7202 7c01 9102 7102 5300 7263 0000  ..r.|...q.S.rc..
+00001760: 0029 01da 0768 6173 6174 7472 7264 0000  .)...hasattrrd..
+00001770: 0072 2400 0000 7224 0000 0072 2500 0000  .r$...r$...r%...
+00001780: 723d 0000 00c5 0000 0072 5900 0000 7a33  r=.......rY...z3
+00001790: 466f 616d 5472 616e 7366 6f72 6d65 722e  FoamTransformer.
+000017a0: 6469 6374 5f61 7373 6967 6e6d 656e 742e  dict_assignment.
+000017b0: 3c6c 6f63 616c 733e 2e3c 6c69 7374 636f  <locals>.<listco
+000017c0: 6d70 3e7a 0b23 636f 6465 5374 7265 616d  mp>z.#codeStream
+000017d0: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
+000017e0: 0004 0000 0053 0000 0072 6200 0000 7224  .....S...rb...r$
+000017f0: 0000 0072 6300 0000 7264 0000 0072 2400  ...rc...rd...r$.
+00001800: 0000 7224 0000 0072 2500 0000 7266 0000  ..r$...r%...rf..
+00001810: 00d7 0000 0072 6700 0000 7a33 466f 616d  .....rg...z3Foam
+00001820: 5472 616e 7366 6f72 6d65 722e 6469 6374  Transformer.dict
+00001830: 5f61 7373 6967 6e6d 656e 742e 3c6c 6f63  _assignment.<loc
+00001840: 616c 733e 2e3c 6469 6374 636f 6d70 3e29  als>.<dictcomp>)
+00001850: 0372 7800 0000 721a 0000 0072 6000 0000  .rx...r....r`...
+00001860: 290f 7240 0000 0072 5e00 0000 7272 0000  ).r@...r^...rr..
+00001870: 0072 0900 0000 720c 0000 0072 5700 0000  .r....r....rW...
+00001880: 7221 0000 00da 0a73 7461 7274 7377 6974  r!.....startswit
+00001890: 6872 6100 0000 722c 0000 0072 1400 0000  hra...r,...r....
+000018a0: 7210 0000 0072 6800 0000 721a 0000 0072  r....rh...r....r
+000018b0: 0b00 0000 2908 7246 0000 0072 4e00 0000  ....).rF...rN...
+000018c0: 7260 0000 0072 1a00 0000 5a09 6e6f 6465  r`...r....Z.node
+000018d0: 735f 7374 7272 6500 0000 5a0c 6e6f 6465  s_strre...Z.node
+000018e0: 735f 6173 7369 676e da03 636c 7372 2400  s_assign..clsr$.
+000018f0: 0000 7224 0000 0072 2500 0000 da0f 6469  ..r$...r%.....di
+00001900: 6374 5f61 7373 6967 6e6d 656e 74b0 0000  ct_assignment...
+00001910: 0073 4400 0000 0801 0401 0c02 0a01 1201  .sD.............
+00001920: 0402 0801 1401 0a02 0401 0280 0e01 1a01  ................
+00001930: 0a02 0401 1201 0602 0202 06fe 0806 0c01  ................
+00001940: 0e01 0280 1002 0601 0402 0202 0201 0201  ................
+00001950: 0c01 0201 0201 04fd 04fe 7a1f 466f 616d  ..........z.Foam
+00001960: 5472 616e 7366 6f72 6d65 722e 6469 6374  Transformer.dict
+00001970: 5f61 7373 6967 6e6d 656e 7463 0200 0000  _assignmentc....
+00001980: 0000 0000 0000 0000 0300 0000 0400 0000  ................
+00001990: 4300 0000 732e 0000 0074 007c 0183 017d  C...s....t.|...}
+000019a0: 0174 017c 0183 0164 016b 0372 0e74 027c  .t.|...d.k.r.t.|
+000019b0: 0183 0182 0164 007d 0274 037c 027c 0164  .....d.}.t.|.|.d
+000019c0: 0219 0083 0253 0072 5d00 0000 2904 7240  .....S.r]...).r@
+000019d0: 0000 0072 5e00 0000 da13 4e6f 7449 6d70  ...r^.....NotImp
+000019e0: 6c65 6d65 6e74 6564 4572 726f 7272 0900  lementedErrorr..
+000019f0: 0000 a903 7246 0000 0072 4e00 0000 721a  ....rF...rN...r.
+00001a00: 0000 0072 2400 0000 7224 0000 0072 2500  ...r$...r$...r%.
+00001a10: 0000 da0d 6973 6f6c 6174 6564 5f6c 6973  ....isolated_lis
+00001a20: 74dd 0000 0073 0a00 0000 0801 0c01 0801  t....s..........
+00001a30: 0401 0e01 7a1d 466f 616d 5472 616e 7366  ....z.FoamTransf
+00001a40: 6f72 6d65 722e 6973 6f6c 6174 6564 5f6c  ormer.isolated_l
+00001a50: 6973 7463 0200 0000 0000 0000 0000 0000  istc............
+00001a60: 0800 0000 0600 0000 4300 0000 73ac 0000  ........C...s...
+00001a70: 0074 007c 0183 017d 0164 007d 0274 017c  .t.|...}.d.}.t.|
+00001a80: 0183 0144 005d 185c 027d 037d 0474 027c  ...D.].\.}.}.t.|
+00001a90: 0474 0383 0272 227c 046a 0464 016b 0272  .t...r"|.j.d.k.r
+00001aa0: 2274 057c 0483 0164 0264 0385 0219 007d  "t.|...d.d.....}
+00001ab0: 0201 006e 0171 0a7c 0264 0075 0172 2c7c  ...n.q.|.d.u.r,|
+00001ac0: 01a0 067c 03a1 0101 0064 007d 0574 077c  ...|.....d.}.t.|
+00001ad0: 0183 0164 046b 0472 4074 027c 0164 0319  ...d.k.r@t.|.d..
+00001ae0: 0074 0883 0272 407c 01a0 0664 03a1 017d  .t...r@|...d...}
+00001af0: 057c 01a0 0664 05a1 017d 0664 007d 077c  .|...d...}.d.}.|
+00001b00: 0172 4e64 06a0 097c 01a1 017d 0774 0a7c  .rNd...|...}.t.|
+00001b10: 067c 077c 027c 0564 078d 0453 0029 084e  .|.|.|.d...S.).N
+00001b20: 5a09 4c49 5354 5f54 5950 45e9 0500 0000  Z.LIST_TYPE.....
+00001b30: 7270 0000 0072 0800 0000 7201 0000 0072  rp...r....r....r
+00001b40: 6f00 0000 2904 721a 0000 0072 1b00 0000  o...).r....r....
+00001b50: 721c 0000 0072 1d00 0000 290b 7240 0000  r....r....).r@..
+00001b60: 00da 0965 6e75 6d65 7261 7465 7257 0000  ...enumeraterW..
+00001b70: 0072 0500 0000 7258 0000 0072 2100 0000  .r....rX...r!...
+00001b80: 7272 0000 0072 5e00 0000 7223 0000 0072  rr...r^...r#...r
+00001b90: 2c00 0000 7219 0000 0029 0872 4600 0000  ,...r....).rF...
+00001ba0: 724e 0000 0072 1c00 0000 da05 696e 6f64  rN...r......inod
+00001bb0: 6572 6500 0000 721d 0000 0072 1a00 0000  ere...r....r....
+00001bc0: 721b 0000 0072 2400 0000 7224 0000 0072  r....r$...r$...r
+00001bd0: 2500 0000 da09 6c69 7374 5f69 6e66 6fe4  %.....list_info.
+00001be0: 0000 0073 2200 0000 0801 0402 1001 1401  ...s"...........
+00001bf0: 1001 0401 0280 0801 0a01 0402 1a01 0a01  ................
+00001c00: 0a02 0402 0401 0a01 1002 7a19 466f 616d  ..........z.Foam
+00001c10: 5472 616e 7366 6f72 6d65 722e 6c69 7374  Transformer.list
+00001c20: 5f69 6e66 6f63 0200 0000 0000 0000 0000  _infoc..........
+00001c30: 0000 0600 0000 0400 0000 4300 0000 73aa  ..........C...s.
+00001c40: 0000 0074 007c 0183 017d 017c 015c 027d  ...t.|...}.|.\.}
+00001c50: 027d 0374 017c 0274 0283 0273 0f4a 0082  .}.t.|.t...s.J..
+00001c60: 017c 026a 037d 047c 047d 057c 026a 0464  .|.j.}.|.}.|.j.d
+00001c70: 0075 0172 207c 0564 017c 026a 0417 0037  .u.r |.d.|.j...7
+00001c80: 007d 057c 026a 0564 0075 0172 2e7c 0564  .}.|.j.d.u.r.|.d
+00001c90: 027c 026a 059b 0064 039d 0337 007d 057c  .|.j...d...7.}.|
+00001ca0: 026a 0664 0075 0172 3b7c 0564 047c 026a  .j.d.u.r;|.d.|.j
+00001cb0: 069b 009d 0237 007d 0574 017c 0474 0783  .....7.}.t.|.t..
+00001cc0: 0272 4474 087c 0483 017d 0474 017c 0574  .rDt.|...}.t.|.t
+00001cd0: 0783 0272 4d74 087c 0583 017d 057c 057c  ...rMt.|...}.|.|
+00001ce0: 035f 0974 0a7c 047c 0383 0253 0029 054e  ._.t.|.|...S.).N
+00001cf0: 726f 0000 007a 060a 4c69 7374 3cda 013e  ro...z..List<..>
+00001d00: 7226 0000 0029 0b72 4000 0000 7257 0000  r&...).r@...rW..
+00001d10: 0072 1900 0000 721a 0000 0072 1b00 0000  .r....r....r....
+00001d20: 721c 0000 0072 1d00 0000 7223 0000 0072  r....r....r#...r
+00001d30: 2100 0000 7275 0000 0072 0900 0000 2906  !...ru...r....).
+00001d40: 7246 0000 0072 4e00 0000 7286 0000 00da  rF...rN...r.....
+00001d50: 0874 6865 5f6c 6973 7472 1a00 0000 5a0d  .the_listr....Z.
+00001d60: 6e61 6d65 5f69 6e74 6572 6e61 6c72 2400  name_internalr$.
+00001d70: 0000 7224 0000 0072 2500 0000 da0f 6c69  ..r$...r%.....li
+00001d80: 7374 5f61 7373 6967 6e6d 656e 74fb 0000  st_assignment...
+00001d90: 0073 2200 0000 0801 0802 0e01 0602 0401  .s".............
+00001da0: 0a02 0e01 0a02 1201 0a02 1001 0a02 0801  ................
+00001db0: 0a01 0801 0602 0a01 7a1f 466f 616d 5472  ........z.FoamTr
+00001dc0: 616e 7366 6f72 6d65 722e 6c69 7374 5f61  ansformer.list_a
+00001dd0: 7373 6967 6e6d 656e 7463 0200 0000 0000  ssignmentc......
+00001de0: 0000 0000 0000 0300 0000 0700 0000 4300  ..............C.
+00001df0: 0000 7370 0000 0064 0164 0284 007c 0144  ..sp...d.d...|.D
+00001e00: 0083 017d 017c 01a0 0064 03a1 017d 0274  ...}.|...d...}.t
+00001e10: 017c 0183 0164 046b 0272 2174 027c 0274  .|...d.k.r!t.|.t
+00001e20: 037c 0164 0519 007c 0164 0319 007c 0164  .|.d...|.d...|.d
+00001e30: 0619 0083 0383 0253 0074 017c 0183 0164  .......S.t.|...d
+00001e40: 076b 0272 3474 027c 0274 037c 0164 0519  .k.r4t.|.t.|.d..
+00001e50: 007c 0164 0619 0064 088d 0283 0253 0074  .|.d...d.....S.t
+00001e60: 047c 0183 0182 0129 094e 6301 0000 0000  .|.....).Nc.....
+00001e70: 0000 0000 0000 0002 0000 0004 0000 0053  ...............S
+00001e80: 0000 0072 3a00 0000 7227 0000 0072 2400  ...r:...r'...r$.
+00001e90: 0000 7264 0000 0072 2400 0000 7224 0000  ..rd...r$...r$..
+00001ea0: 0072 2500 0000 723d 0000 0016 0100 0072  .r%...r=.......r
+00001eb0: 3e00 0000 7a38 466f 616d 5472 616e 7366  >...z8FoamTransf
+00001ec0: 6f72 6d65 722e 6469 6d65 6e73 696f 6e5f  ormer.dimension_
+00001ed0: 6173 7369 676e 6d65 6e74 2e3c 6c6f 6361  assignment.<loca
+00001ee0: 6c73 3e2e 3c6c 6973 7463 6f6d 703e 7201  ls>.<listcomp>r.
+00001ef0: 0000 00e9 0300 0000 7270 0000 00e9 feff  ........rp......
+00001f00: ffff e902 0000 0029 0172 7100 0000 2905  .......).rq...).
+00001f10: 7272 0000 0072 5e00 0000 7209 0000 0072  rr...r^...r....r
+00001f20: 1200 0000 725f 0000 0072 8100 0000 7224  ....r_...r....r$
+00001f30: 0000 0072 2400 0000 7225 0000 00da 1464  ...r$...r%.....d
+00001f40: 696d 656e 7369 6f6e 5f61 7373 6967 6e6d  imension_assignm
+00001f50: 656e 7415 0100 0073 0e00 0000 0e01 0a01  ent....s........
+00001f60: 0c02 1e01 0c01 1a01 0802 7a24 466f 616d  ..........z$Foam
+00001f70: 5472 616e 7366 6f72 6d65 722e 6469 6d65  Transformer.dime
+00001f80: 6e73 696f 6e5f 6173 7369 676e 6d65 6e74  nsion_assignment
+00001f90: 6302 0000 0000 0000 0000 0000 0003 0000  c...............
+00001fa0: 0003 0000 0043 0000 0073 3600 0000 6401  .....C...s6...d.
+00001fb0: 6402 8400 7c01 4400 8301 7d01 7400 7c01  d...|.D...}.t.|.
+00001fc0: 8301 6403 6b03 7211 7401 7c01 8301 8201  ..d.k.r.t.|.....
+00001fd0: 7c01 a002 6404 a101 7d02 7403 7c02 6405  |...d...}.t.|.d.
+00001fe0: 8302 5300 2906 4e63 0100 0000 0000 0000  ..S.).Nc........
+00001ff0: 0000 0000 0200 0000 0400 0000 5300 0000  ............S...
+00002000: 723a 0000 0072 2700 0000 7224 0000 0072  r:...r'...r$...r
+00002010: 6400 0000 7224 0000 0072 2400 0000 7225  d...r$...r$...r%
+00002020: 0000 0072 3d00 0000 2101 0000 723e 0000  ...r=...!...r>..
+00002030: 007a 3446 6f61 6d54 7261 6e73 666f 726d  .z4FoamTransform
+00002040: 6572 2e6d 6163 726f 5f61 7373 6967 6e6d  er.macro_assignm
+00002050: 656e 742e 3c6c 6f63 616c 733e 2e3c 6c69  ent.<locals>.<li
+00002060: 7374 636f 6d70 3e72 0800 0000 7201 0000  stcomp>r....r...
+00002070: 00da 0029 0472 5e00 0000 7280 0000 0072  ...).r^...r....r
+00002080: 7200 0000 7209 0000 0072 8100 0000 7224  r...r....r....r$
+00002090: 0000 0072 2400 0000 7225 0000 00da 106d  ...r$...r%.....m
+000020a0: 6163 726f 5f61 7373 6967 6e6d 656e 7420  acro_assignment 
+000020b0: 0100 0073 0a00 0000 0e01 0c01 0801 0a01  ...s............
+000020c0: 0a01 7a20 466f 616d 5472 616e 7366 6f72  ..z FoamTransfor
+000020d0: 6d65 722e 6d61 6372 6f5f 6173 7369 676e  mer.macro_assign
+000020e0: 6d65 6e74 6302 0000 0000 0000 0000 0000  mentc...........
+000020f0: 0003 0000 0003 0000 0043 0000 0073 4e00  .........C...sN.
+00002100: 0000 6401 6402 8400 7c01 4400 8301 7d01  ..d.d...|.D...}.
+00002110: 7400 7c01 8301 6403 6b03 7211 7401 7c01  t.|...d.k.r.t.|.
+00002120: 8301 8201 7c01 6404 1900 7d02 7402 7c02  ....|.d...}.t.|.
+00002130: 6405 8302 721e 7c02 a003 a100 7d02 7c01  d...r.|.....}.|.
+00002140: 6406 1900 9b00 6407 7c02 9b00 9d03 5300  d.....d.|.....S.
+00002150: 2908 4e63 0100 0000 0000 0000 0000 0000  ).Nc............
+00002160: 0200 0000 0400 0000 5300 0000 723a 0000  ........S...r:..
+00002170: 0072 2700 0000 7224 0000 0072 6400 0000  .r'...r$...rd...
+00002180: 7224 0000 0072 2400 0000 7225 0000 0072  r$...r$...r%...r
+00002190: 3d00 0000 2801 0000 723e 0000 007a 3046  =...(...r>...z0F
+000021a0: 6f61 6d54 7261 6e73 666f 726d 6572 2e65  oamTransformer.e
+000021b0: 7175 616c 5f61 7373 6967 6e2e 3c6c 6f63  qual_assign.<loc
+000021c0: 616c 733e 2e3c 6c69 7374 636f 6d70 3e72  als>.<listcomp>r
+000021d0: 8c00 0000 7208 0000 0072 3800 0000 7201  ....r....r8...r.
+000021e0: 0000 00da 013d 2904 725e 0000 0072 5f00  .....=).r^...r_.
+000021f0: 0000 727c 0000 0072 3800 0000 2903 7246  ..r|...r8...).rF
+00002200: 0000 0072 4e00 0000 7214 0000 0072 2400  ...rN...r....r$.
+00002210: 0000 7224 0000 0072 2500 0000 da0c 6571  ..r$...r%.....eq
+00002220: 7561 6c5f 6173 7369 676e 2701 0000 730e  ual_assign'...s.
+00002230: 0000 000e 010c 0108 0108 010a 0108 0112  ................
+00002240: 017a 1c46 6f61 6d54 7261 6e73 666f 726d  .z.FoamTransform
+00002250: 6572 2e65 7175 616c 5f61 7373 6967 6e63  er.equal_assignc
+00002260: 0200 0000 0000 0000 0000 0000 0700 0000  ................
+00002270: 0500 0000 4300 0000 736e 0000 0064 0164  ....C...sn...d.d
+00002280: 0284 007c 0144 0083 017d 0174 007c 0183  ...|.D...}.t.|..
+00002290: 0164 036b 0272 127c 015c 027d 027d 036e  .d.k.r.|.\.}.}.n
+000022a0: 177c 01a0 0164 04a1 017d 027c 01a0 0164  .|...d...}.|...d
+000022b0: 04a1 017d 0464 05a0 027c 01a1 017d 057c  ...}.d...|...}.|
+000022c0: 0464 067c 059b 0064 079d 0317 007d 037c  .d.|...d.....}.|
+000022d0: 0264 0817 007c 0317 007d 0674 037c 0674  .d...|...}.t.|.t
+000022e0: 047c 027c 0383 0283 0253 0029 094e 6301  .|.|.....S.).Nc.
+000022f0: 0000 0000 0000 0000 0000 0002 0000 0004  ................
+00002300: 0000 0053 0000 0072 3a00 0000 7227 0000  ...S...r:...r'..
+00002310: 0072 2400 0000 7264 0000 0072 2400 0000  .r$...rd...r$...
+00002320: 7224 0000 0072 2500 0000 723d 0000 0031  r$...r%...r=...1
+00002330: 0100 0072 3e00 0000 7a38 466f 616d 5472  ...r>...z8FoamTr
+00002340: 616e 7366 6f72 6d65 722e 6469 7265 6374  ansformer.direct
+00002350: 6976 655f 6173 7369 676e 6d65 6e74 2e3c  ive_assignment.<
+00002360: 6c6f 6361 6c73 3e2e 3c6c 6973 7463 6f6d  locals>.<listcom
+00002370: 703e 728c 0000 0072 0100 0000 7a02 2c20  p>r....r....z., 
+00002380: 727a 0000 0072 7b00 0000 726f 0000 0029  rz...r{...ro...)
+00002390: 0572 5e00 0000 7272 0000 0072 2c00 0000  .r^...rr...r,...
+000023a0: 7209 0000 0072 0e00 0000 2907 7246 0000  r....r....).rF..
+000023b0: 0072 4e00 0000 7260 0000 00da 0763 6f6e  .rN...r`.....con
+000023c0: 7465 6e74 da0d 6675 6e63 7469 6f6e 5f6e  tent..function_n
+000023d0: 616d 65da 0961 7267 756d 656e 7473 da03  ame..arguments..
+000023e0: 6b65 7972 2400 0000 7224 0000 0072 2500  keyr$...r$...r%.
+000023f0: 0000 da14 6469 7265 6374 6976 655f 6173  ....directive_as
+00002400: 7369 676e 6d65 6e74 3001 0000 7312 0000  signment0...s...
+00002410: 000e 010c 010a 010a 020a 010a 0110 010c  ................
+00002420: 0110 017a 2446 6f61 6d54 7261 6e73 666f  ...z$FoamTransfo
+00002430: 726d 6572 2e64 6972 6563 7469 7665 5f61  rmer.directive_a
+00002440: 7373 6967 6e6d 656e 7463 0200 0000 0000  ssignmentc......
+00002450: 0000 0000 0000 0500 0000 0700 0000 4300  ..............C.
+00002460: 0000 73ac 0000 0074 007c 0183 017d 0164  ..s....t.|...}.d
+00002470: 007d 0274 017c 0183 0164 016b 0272 117c  .}.t.|...d.k.r.|
+00002480: 015c 027d 037d 046e 1974 017c 0183 0164  .\.}.}.n.t.|...d
+00002490: 026b 0272 267c 015c 037d 037d 027d 047c  .k.r&|.\.}.}.}.|
+000024a0: 02a0 0264 03a1 0173 2574 037c 0183 0182  ...d...s%t.|....
+000024b0: 016e 0474 037c 0183 0182 0174 047c 0483  .n.t.|.....t.|..
+000024c0: 017d 047c 04a0 0264 04a1 0172 447c 04a0  .}.|...d...rD|..
+000024d0: 0564 0564 06a1 0264 0719 007d 047c 04a0  .d.d...d...}.|..
+000024e0: 0664 0564 06a1 0264 0819 007d 046e 087c  .d.d...d...}.n.|
+000024f0: 0464 0164 0985 0219 00a0 07a1 007d 0474  .d.d.........}.t
+00002500: 087c 0374 097c 037c 047c 0264 0a8d 0383  .|.t.|.|.|.d....
+00002510: 0253 0029 0b4e 728c 0000 0072 8a00 0000  .S.).Nr....r....
+00002520: 7279 0000 007a 0323 7b0a 7226 0000 0072  ry...z.#{.r&...r
+00002530: 0800 0000 7270 0000 0072 0100 0000 e9fd  ....rp...r......
+00002540: ffff ff29 0172 6000 0000 290a 7240 0000  ...).r`...).r@..
+00002550: 0072 5e00 0000 727d 0000 0072 8000 0000  .r^...r}...r....
+00002560: 7221 0000 0072 2d00 0000 da06 7273 706c  r!...r-.....rspl
+00002570: 6974 da05 7374 7269 7072 0900 0000 720a  it..stripr....r.
+00002580: 0000 0029 0572 4600 0000 724e 0000 0072  ...).rF...rN...r
+00002590: 6000 0000 721a 0000 00da 0463 6f64 6572  `...r......coder
+000025a0: 2400 0000 7224 0000 0072 2500 0000 da0f  $...r$...r%.....
+000025b0: 636f 6465 5f61 7373 6967 6e6d 656e 743c  code_assignment<
+000025c0: 0100 0073 2000 0000 0801 0401 0c01 0a01  ...s ...........
+000025d0: 0c01 0a01 0a01 0801 02ff 0803 0801 0a01  ................
+000025e0: 1001 1201 1002 1401 7a1f 466f 616d 5472  ........z.FoamTr
+000025f0: 616e 7366 6f72 6d65 722e 636f 6465 5f61  ansformer.code_a
+00002600: 7373 6967 6e6d 656e 7463 0200 0000 0000  ssignmentc......
+00002610: 0000 0000 0000 0200 0000 0300 0000 4300  ..............C.
+00002620: 0000 731a 0000 0074 007c 0183 017d 0174  ..s....t.|...}.t
+00002630: 017c 0164 0119 006a 0264 0217 0083 0153  .|.d...j.d.....S
+00002640: 0029 034e 7201 0000 0072 2600 0000 2903  .).Nr....r&...).
+00002650: 7240 0000 0072 1100 0000 7214 0000 0072  r@...r....r....r
+00002660: 4500 0000 7224 0000 0072 2400 0000 7225  E...r$...r$...r%
+00002670: 0000 00da 1273 7065 6369 616c 5f64 6972  .....special_dir
+00002680: 6563 7469 7665 734f 0100 0073 0400 0000  ectivesO...s....
+00002690: 0801 1201 7a22 466f 616d 5472 616e 7366  ....z"FoamTransf
+000026a0: 6f72 6d65 722e 7370 6563 6961 6c5f 6469  ormer.special_di
+000026b0: 7265 6374 6976 6573 4e29 1a72 1e00 0000  rectivesN).r....
+000026c0: 721f 0000 0072 2000 0000 7248 0000 0072  r....r ...rH...r
+000026d0: 4b00 0000 724f 0000 0072 5000 0000 7251  K...rO...rP...rQ
+000026e0: 0000 0072 5200 0000 7253 0000 0072 5400  ...rR...rS...rT.
+000026f0: 0000 725b 0000 0072 6000 0000 7261 0000  ..r[...r`...ra..
+00002700: 0072 6a00 0000 7277 0000 0072 7f00 0000  .rj...rw...r....
+00002710: 7282 0000 0072 8600 0000 7289 0000 0072  r....r....r....r
+00002720: 8d00 0000 728f 0000 0072 9100 0000 7296  ....r....r....r.
+00002730: 0000 0072 9b00 0000 729c 0000 0072 2400  ...r....r....r$.
+00002740: 0000 7224 0000 0072 2400 0000 7225 0000  ..r$...r$...r%..
+00002750: 0072 3300 0000 4a00 0000 7330 0000 0008  .r3...J...s0....
+00002760: 0008 0108 0308 0308 0308 0308 0308 0308  ................
+00002770: 0308 0308 0908 0508 0a08 0e08 2708 2d08  ............'.-.
+00002780: 0708 1708 1a08 0b08 0708 0908 0c0c 1372  ...............r
+00002790: 3300 0000 7227 0000 0029 27da 075f 5f64  3...r'...)'..__d
+000027a0: 6f63 5f5f da0b 6461 7461 636c 6173 7365  oc__..dataclasse
+000027b0: 7372 0200 0000 da07 7061 7468 6c69 6272  sr......pathlibr
+000027c0: 0300 0000 5a04 6c61 726b 7204 0000 0072  ....Z.larkr....r
+000027d0: 0500 0000 7206 0000 005a 0f6c 6172 6b2e  ....r....Z.lark.
+000027e0: 6578 6365 7074 696f 6e73 7207 0000 00da  exceptionsr.....
+000027f0: 0361 7374 7209 0000 0072 0a00 0000 720b  .astr....r....r.
+00002800: 0000 0072 0c00 0000 720d 0000 0072 0e00  ...r....r....r..
+00002810: 0000 720f 0000 0072 1000 0000 7211 0000  ..r....r....r...
+00002820: 0072 1200 0000 7213 0000 00da 085f 5f66  .r....r......__f
+00002830: 696c 655f 5fda 0861 6273 6f6c 7574 65da  ile__..absolute.
+00002840: 0670 6172 656e 74da 0468 6572 65da 0972  .parent..here..r
+00002850: 6561 645f 7465 7874 7236 0000 005a 1067  ead_textr6...Z.g
+00002860: 7261 6d6d 6172 5f61 6476 616e 6365 6472  rammar_advancedr
+00002870: 2f00 0000 7231 0000 0072 3200 0000 7219  /...r1...r2...r.
+00002880: 0000 0072 3000 0000 7238 0000 0072 4000  ...r0...r8...r@.
+00002890: 0000 7244 0000 0072 3300 0000 7224 0000  ..rD...r3...r$..
+000028a0: 0072 2400 0000 7224 0000 0072 2500 0000  .r$...r$...r%...
+000028b0: da08 3c6d 6f64 756c 653e 0100 0000 7326  ..<module>....s&
+000028c0: 0000 0004 000c 020c 0114 020c 0134 020e  .............4..
+000028d0: 0e0c 020c 010e 020e 010a 0202 0310 010a  ................
+000028e0: 0708 1008 0408 0414 08                   .........
```

### Comparing `fluidsimfoam-0.0.5/src/fluidsimfoam/foam_input_files/__pycache__/polymesh.cpython-310.pyc` & `fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/__pycache__/polymesh.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed May  3 13:57:31 2023 UTC, .py size: 973 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 4b68 5264 cd03 0000  o.......KhRd....
+00000000: 6f0d 0d0a 0000 0000 70b5 5264 cd03 0000  o.......p.Rd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 4200 0000 6400  .....@...sB...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 0100 6401 6404 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6401 6402 6c06 5a07 6503 6405 6406  ..d.d.l.Z.e.d.d.
 00000060: 8d01 6407 6408 8400 8301 5a08 6402 5300  ..d.d.....Z.d.S.
 00000070: 2909 7a3a 5265 6164 2069 6e66 6f72 6d61  ).z:Read informa
@@ -44,26 +44,25 @@
 000002b0: 7374 7269 70da 0572 6669 6e64 da02 6e70  strip..rfind..np
 000002c0: da07 6c6f 6164 7478 7472 0300 0000 da04  ..loadtxtr......
 000002d0: 7369 7a65 290a da04 7061 7468 da04 6669  size)...path..fi
 000002e0: 6c65 da04 6c69 6e65 5a08 6e62 5f63 656c  le..lineZ.nb_cel
 000002f0: 6c73 da03 7478 745a 1269 6e64 6578 5f6c  ls..txtZ.index_l
 00000300: 6173 745f 636f 6d6d 656e 74da 0663 6f6f  ast_comment..coo
 00000310: 7264 73da 0178 da01 79da 017a a900 721f  rds..x..y..z..r.
-00000320: 0000 00fa 542f 686f 6d65 2f75 7365 7273  ....T/home/users
-00000330: 2f61 7567 6965 7233 7069 2f44 6576 2f66  /augier3pi/Dev/f
-00000340: 6c75 6964 7369 6d66 6f61 6d2f 7372 632f  luidsimfoam/src/
-00000350: 666c 7569 6473 696d 666f 616d 2f66 6f61  fluidsimfoam/foa
-00000360: 6d5f 696e 7075 745f 6669 6c65 732f 706f  m_input_files/po
-00000370: 6c79 6d65 7368 2e70 79da 1167 6574 5f70  lymesh.py..get_p
-00000380: 6f69 6e74 735f 636f 6f72 6473 0c00 0000  oints_coords....
-00000390: 733a 0000 000a 0408 0108 0104 0102 ff08  s:..............
-000003a0: 0208 0104 0102 ff08 020c 0108 0108 0104  ................
-000003b0: 0102 fe10 030a 011c f30a 0f0e 0108 020a  ................
-000003c0: 0210 010e 0210 0110 0110 010e 020a 0272  ...............r
-000003d0: 2100 0000 2909 da07 5f5f 646f 635f 5f72  !...)...__doc__r
-000003e0: 1000 0000 da09 6675 6e63 746f 6f6c 7372  ......functoolsr
-000003f0: 0200 0000 da02 696f 7203 0000 00da 056e  ......ior......n
-00000400: 756d 7079 7214 0000 0072 2100 0000 721f  umpyr....r!...r.
-00000410: 0000 0072 1f00 0000 721f 0000 0072 2000  ...r....r....r .
-00000420: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
-00000430: 730e 0000 0004 0008 040c 010c 0108 0208  s...............
-00000440: 030e 01                                  ...
+00000320: 0000 00fa 4b2f 686f 6d65 2f70 6965 7272  ....K/home/pierr
+00000330: 652f 4465 762f 666c 7569 6473 696d 666f  e/Dev/fluidsimfo
+00000340: 616d 2f73 7263 2f66 6c75 6964 7369 6d66  am/src/fluidsimf
+00000350: 6f61 6d2f 666f 616d 5f69 6e70 7574 5f66  oam/foam_input_f
+00000360: 696c 6573 2f70 6f6c 796d 6573 682e 7079  iles/polymesh.py
+00000370: da11 6765 745f 706f 696e 7473 5f63 6f6f  ..get_points_coo
+00000380: 7264 730c 0000 0073 3a00 0000 0a04 0801  rds....s:.......
+00000390: 0801 0401 02ff 0802 0801 0401 02ff 0802  ................
+000003a0: 0c01 0801 0801 0401 02fe 1003 0a01 1cf3  ................
+000003b0: 0a0f 0e01 0802 0a02 1001 0e02 1001 1001  ................
+000003c0: 1001 0e02 0a02 7221 0000 0029 09da 075f  ......r!...)..._
+000003d0: 5f64 6f63 5f5f 7210 0000 00da 0966 756e  _doc__r......fun
+000003e0: 6374 6f6f 6c73 7202 0000 00da 0269 6f72  ctoolsr......ior
+000003f0: 0300 0000 da05 6e75 6d70 7972 1400 0000  ......numpyr....
+00000400: 7221 0000 0072 1f00 0000 721f 0000 0072  r!...r....r....r
+00000410: 1f00 0000 7220 0000 00da 083c 6d6f 6475  ....r .....<modu
+00000420: 6c65 3e01 0000 0073 0e00 0000 0400 0804  le>....s........
+00000430: 0c01 0c01 0802 0803 0e01                 ..........
```

### Comparing `fluidsimfoam-0.0.5/src/fluidsimfoam/foam_input_files/__pycache__/util.cpython-39.pyc` & `fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/__pycache__/util.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun  1 13:07:51 2023 UTC, .py size: 766 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 20% similar despite different names*

```diff
@@ -1,56 +1,56 @@
-00000000: 610d 0d0a 0000 0000 2798 7864 fe02 0000  a.......'.xd....
+00000000: 6f0d 0d0a 0000 0000 8b64 6e64 fe02 0000  o........dnd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 2e00 0000 6400  .....@...s....d.
-00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6408  Z.d.d.l.m.Z...d.
-00000040: 6502 6503 6504 6602 1900 6503 6404 9c02  e.e.e.f...e.d...
-00000050: 6405 6406 8405 5a05 6407 5300 2909 5a09  d.d...Z.d.S.).Z.
-00000060: 5574 696c 6974 6965 73e9 0000 0000 2901  Utilities.....).
-00000070: da05 556e 696f 6e54 2902 da04 6461 7461  ..UnionT)...data
+00000020: 0005 0000 0040 0000 0073 3000 0000 6400  .....@...s0...d.
+00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6409  Z.d.d.l.m.Z...d.
+00000040: 6404 6502 6503 6504 6602 1900 6405 6503  d.e.e.e.f...d.e.
+00000050: 6604 6406 6407 8405 5a05 6408 5300 290a  f.d.d...Z.d.S.).
+00000060: 5a09 5574 696c 6974 6965 73e9 0000 0000  Z.Utilities.....
+00000070: 2901 da05 556e 696f 6e54 da04 6461 7461  )...UnionT..data
 00000080: da06 7265 7475 726e 6302 0000 0000 0000  ..returnc.......
 00000090: 0000 0000 0005 0000 0005 0000 0003 0000  ................
-000000a0: 0073 9000 0000 7400 7c00 7401 8302 720e  .s....t.|.t...r.
-000000b0: 7c00 5300 7400 7c00 7402 8302 7288 7c00  |.S.t.|.t...r.|.
+000000a0: 0073 8a00 0000 7400 7c00 7401 8302 7207  .s....t.|.t...r.
+000000b0: 7c00 5300 7400 7c00 7402 8302 7243 7c00  |.S.t.|.t...rC|.
 000000c0: 7d02 6900 7d00 7c02 a003 a100 a004 6401  }.i.}.|.......d.
-000000d0: a101 4400 5d54 8900 8800 a003 a100 a005  ..D.]T..........
+000000d0: a101 4400 5d29 8900 8800 a003 a100 a005  ..D.])..........
 000000e0: 6402 a101 8900 7406 8700 6601 6403 6404  d.....t...f.d.d.
-000000f0: 8408 6405 4400 8301 8301 726a 7c01 725e  ..d.D.....rj|.r^
-00000100: 712e 717a 8800 6406 0200 7d03 7d04 6e10  q.qz..d...}.}.n.
-00000110: 8800 6a04 6407 6408 8d01 5c02 7d03 7d04  ..j.d.d...\.}.}.
-00000120: 7c04 7c00 7c03 3c00 712e 7c00 5300 7407  |.|.|.<.q.|.S.t.
-00000130: 8201 6406 5300 2909 7a2e 7265 7475 726e  ..d.S.).z.return
-00000140: 2061 2064 6963 742c 2070 6f74 656e 7469   a dict, potenti
-00000150: 616c 6c79 2062 7920 636f 6e76 6572 7469  ally by converti
-00000160: 6e67 2061 2073 7472 da01 0afa 013b 6301  ng a str.....;c.
-00000170: 0000 0000 0000 0000 0000 0002 0000 0004  ................
-00000180: 0000 0033 0000 0073 1800 0000 7c00 5d10  ...3...s....|.].
-00000190: 7d01 8800 a000 7c01 a101 5600 0100 7102  }.....|...V...q.
-000001a0: 6400 5300 2901 4e29 01da 0a73 7461 7274  d.S.).N)...start
-000001b0: 7377 6974 6829 02da 022e 305a 0c63 6f6d  swith)....0Z.com
-000001c0: 6d65 6e74 5f63 6861 72a9 01da 046c 696e  ment_char....lin
-000001d0: 65a9 00fa 502f 686f 6d65 2f75 7365 7273  e...P/home/users
-000001e0: 2f61 7567 6965 7233 7069 2f44 6576 2f66  /augier3pi/Dev/f
-000001f0: 6c75 6964 7369 6d66 6f61 6d2f 7372 632f  luidsimfoam/src/
-00000200: 666c 7569 6473 696d 666f 616d 2f66 6f61  fluidsimfoam/foa
-00000210: 6d5f 696e 7075 745f 6669 6c65 732f 7574  m_input_files/ut
-00000220: 696c 2e70 79da 093c 6765 6e65 7870 723e  il.py..<genexpr>
-00000230: 0e00 0000 f300 0000 007a 1a61 735f 6469  .........z.as_di
-00000240: 6374 2e3c 6c6f 6361 6c73 3e2e 3c67 656e  ct.<locals>.<gen
-00000250: 6578 7072 3e29 027a 022f 2ffa 0123 4ee9  expr>).z.//..#N.
-00000260: 0100 0000 2901 da08 6d61 7873 706c 6974  ....)...maxsplit
-00000270: 2908 da0a 6973 696e 7374 616e 6365 da04  )...isinstance..
-00000280: 6469 6374 da03 7374 72da 0573 7472 6970  dict..str..strip
-00000290: da05 7370 6c69 74da 0c72 656d 6f76 6573  ..split..removes
-000002a0: 7566 6669 78da 0361 6e79 da09 5479 7065  uffix..any..Type
-000002b0: 4572 726f 7229 0572 0300 0000 da0f 6669  Error).r......fi
-000002c0: 6c74 6572 5f63 6f6d 6d65 6e74 735a 0b64  lter_commentsZ.d
-000002d0: 6174 615f 6173 5f73 7472 da03 6b65 79da  ata_as_str..key.
-000002e0: 0576 616c 7565 720b 0000 0072 0900 0000  .valuer....r....
-000002f0: 720c 0000 00da 0761 735f 6469 6374 0500  r......as_dict..
-00000300: 0000 731e 0000 0000 020a 0104 010a 0104  ..s.............
-00000310: 0104 0112 010e 0116 0104 0104 020c 0210  ................
-00000320: 010a 0104 0272 1d00 0000 4e29 0154 2906  .....r....N).T).
-00000330: da07 5f5f 646f 635f 5fda 0674 7970 696e  ..__doc__..typin
-00000340: 6772 0200 0000 7213 0000 0072 1400 0000  gr....r....r....
-00000350: 721d 0000 0072 0b00 0000 720b 0000 0072  r....r....r....r
-00000360: 0b00 0000 720c 0000 00da 083c 6d6f 6475  ....r......<modu
-00000370: 6c65 3e01 0000 0073 0400 0000 0401 0c03  le>....s........
+000000f0: 8408 6405 4400 8301 8301 7234 7c01 722e  ..d.D.....r4|.r.
+00000100: 7117 8800 6406 0202 7d03 7d04 6e08 8800  q...d...}.}.n...
+00000110: 6a04 6407 6408 8d01 5c02 7d03 7d04 7c04  j.d.d...\.}.}.|.
+00000120: 7c00 7c03 3c00 7117 7c00 5300 7407 8201  |.|.<.q.|.S.t...
+00000130: 2909 7a2e 7265 7475 726e 2061 2064 6963  ).z.return a dic
+00000140: 742c 2070 6f74 656e 7469 616c 6c79 2062  t, potentially b
+00000150: 7920 636f 6e76 6572 7469 6e67 2061 2073  y converting a s
+00000160: 7472 da01 0afa 013b 6301 0000 0000 0000  tr.....;c.......
+00000170: 0000 0000 0002 0000 0004 0000 0033 0000  .............3..
+00000180: 0073 1a00 0000 8100 7c00 5d08 7d01 8800  .s......|.].}...
+00000190: a000 7c01 a101 5600 0100 7102 6400 5300  ..|...V...q.d.S.
+000001a0: 2901 4e29 01da 0a73 7461 7274 7377 6974  ).N)...startswit
+000001b0: 6829 02da 022e 305a 0c63 6f6d 6d65 6e74  h)....0Z.comment
+000001c0: 5f63 6861 72a9 01da 046c 696e 65a9 00fa  _char....line...
+000001d0: 472f 686f 6d65 2f70 6965 7272 652f 4465  G/home/pierre/De
+000001e0: 762f 666c 7569 6473 696d 666f 616d 2f73  v/fluidsimfoam/s
+000001f0: 7263 2f66 6c75 6964 7369 6d66 6f61 6d2f  rc/fluidsimfoam/
+00000200: 666f 616d 5f69 6e70 7574 5f66 696c 6573  foam_input_files
+00000210: 2f75 7469 6c2e 7079 da09 3c67 656e 6578  /util.py..<genex
+00000220: 7072 3e0e 0000 0073 0400 0000 0280 1800  pr>....s........
+00000230: 7a1a 6173 5f64 6963 742e 3c6c 6f63 616c  z.as_dict.<local
+00000240: 733e 2e3c 6765 6e65 7870 723e 2902 7a02  s>.<genexpr>).z.
+00000250: 2f2f fa01 234e e901 0000 0029 01da 086d  //..#N.....)...m
+00000260: 6178 7370 6c69 7429 08da 0a69 7369 6e73  axsplit)...isins
+00000270: 7461 6e63 65da 0464 6963 74da 0373 7472  tance..dict..str
+00000280: da05 7374 7269 70da 0573 706c 6974 da0c  ..strip..split..
+00000290: 7265 6d6f 7665 7375 6666 6978 da03 616e  removesuffix..an
+000002a0: 79da 0954 7970 6545 7272 6f72 2905 7203  y..TypeError).r.
+000002b0: 0000 005a 0f66 696c 7465 725f 636f 6d6d  ...Z.filter_comm
+000002c0: 656e 7473 5a0b 6461 7461 5f61 735f 7374  entsZ.data_as_st
+000002d0: 72da 036b 6579 da05 7661 6c75 6572 0b00  r..key..valuer..
+000002e0: 0000 7209 0000 0072 0c00 0000 da07 6173  ..r....r......as
+000002f0: 5f64 6963 7405 0000 0073 1e00 0000 0a02  _dict....s......
+00000300: 0401 0a01 0401 0401 1201 0e01 1601 0401  ................
+00000310: 0201 0c02 1002 0a01 0401 0402 721b 0000  ............r...
+00000320: 004e 2901 5429 06da 075f 5f64 6f63 5f5f  .N).T)...__doc__
+00000330: da06 7479 7069 6e67 7202 0000 0072 1200  ..typingr....r..
+00000340: 0000 7213 0000 0072 1b00 0000 720b 0000  ..r....r....r...
+00000350: 0072 0b00 0000 720b 0000 0072 0c00 0000  .r....r....r....
+00000360: da08 3c6d 6f64 756c 653e 0100 0000 7306  ..<module>....s.
+00000370: 0000 0004 000c 0120 03                   ....... .
```

### Comparing `fluidsimfoam-0.0.5/src/fluidsimfoam/foam_input_files/ast.py` & `fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/ast.py`

 * *Files identical despite different names*

### Comparing `fluidsimfoam-0.0.5/src/fluidsimfoam/foam_input_files/blockmesh/LICENSE` & `fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/blockmesh/LICENSE`

 * *Files identical despite different names*

### Comparing `fluidsimfoam-0.0.5/src/fluidsimfoam/foam_input_files/blockmesh/__init__.py` & `fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/blockmesh/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,24 +57,14 @@
     def __eq__(self, rhs):
         return (self.z, self.y, self.x) == (rhs.z, rhs.y, rhs.x)
 
     def __hash__(self):
         return hash((self.z, self.y, self.x))
 
 
-class Point:
-    def __init__(self, x, y, z):
-        self.x = x
-        self.y = y
-        self.z = z
-
-    def format(self):
-        return f"( {self.x:18.15g} {self.y:18.15g} {self.z:18.15g} )"
-
-
 class Face:
     def __init__(self, vnames, name):
         """
         vname is list or tuple of vertex names
         """
         self.vnames = vnames
         self.name = name
@@ -84,14 +74,23 @@
         vertices is dict of name to Vertex
         """
         index = " ".join(str(vertices[vn].index) for vn in self.vnames)
         comment = " ".join(self.vnames)
         return f"({index:s})  // {self.name:s} ({comment:s})"
 
 
+class MergePatchPairs:
+    def __init__(self, boundary_name1, boundary_name2):
+        self.boundary_name1 = boundary_name1
+        self.boundary_name2 = boundary_name2
+
+    def format(self):
+        return f"({self.boundary_name1} {self.boundary_name2})"
+
+
 class HexBlock:
     def __init__(self, vnames, cells, name, grading=SimpleGrading(1, 1, 1)):
         """Initialize HexBlock instance
         vnames is the vertex names in order descrived in
             http://www.openfoam.org/docs/user/mesh-description.php
         cells is number of cells devied into in each direction
         name is the uniq name of the block
@@ -105,17 +104,18 @@
     def format(self, vertices):
         """Format instance to dump
         vertices is dict of name to Vertex
         """
         index = " ".join(str(vertices[vn].index) for vn in self.vnames)
         comment = " ".join(self.vnames)
         return (
+            f"// {self.name} ({comment})\n    "
             f"hex ({index}) {self.name} "
             f"({self.cells[0]:d} {self.cells[1]:d} {self.cells[2]:d}) "
-            f"{self.grading.format()}  // {self.name} ({comment})"
+            f"{self.grading.format()}"
         )
 
     def face(self, index, name=None):
         """Generate Face object
         index is number or keyword to identify the face of Hex
             0 = 'w' = 'xm' = '-100' = (0 4 7 3)
             1 = 'e' = 'xp' = '100' = (1 2 6 5)
@@ -201,30 +201,31 @@
         vertices is dict of name to Vertex
         """
         tmp = [self.name]
         if self.neighbour is None:
             tmp.append("{\n" + f"    type {self.type_};\n    faces\n    (")
         else:
             tmp.append(
-                "{\n"
-                + f"    type {self.type_};\n    neighbourPatch  {self.neighbour};\n    faces\n    ("
+                "{\n" + f"    type {self.type_};\n"
+                f"    neighbourPatch  {self.neighbour};\n    faces\n    ("
             )
         for face in self.faces:
             tmp.append(f"        {face.format(vertices)}")
         tmp.append("    );\n}")
         return "\n".join(tmp)
 
 
 class BlockMeshDict:
     def __init__(self):
         self.convert_to_meters = 1.0
         self.vertices = {}  # mapping of uniq name to Vertex object
         self.blocks = {}
         self.edges = {}
         self.boundaries = {}
+        self.merge_patch_pairs = {}
         self._vertices_in_blockmesh = None
 
     def set_metric(self, metric):
         """set self.comvert_to_meters by word"""
         metricsym_to_conversion = {
             "km": 1000,
             "m": 1,
@@ -289,31 +290,51 @@
             groups.append(list(g))
         for group in groups:
             if len(group) == 1:
                 continue
             names = [v[0] for v in group]
             self.reduce_vertex(*names)
 
-    def replicate_vertices_further_z(self, dz, add_to_name="_dz"):
+    def replicate_vertices_further_z(self, z, suffix="_dz", vnames=None):
         """Helper for 2d meshes"""
-        for vertex_z0 in self.vertices.copy().values():
+        if vnames is None:
+            vnames = tuple(self.vertices.keys())
+        for vname in vnames:
+            vertex_z0 = self.vertices[vname]
             vertex_z1 = vertex_z0.copy()
-            vertex_z1.z = dz
-            vertex_z1.name += add_to_name
+            vertex_z1.z = z
+            vertex_z1.name += suffix
             self.add_vertex(vertex_z1)
 
     def add_hexblock(
-        self, vnames, cells, name=None, grading=SimpleGrading(1, 1, 1)
+        self, vnames, nx_ny_nz, name=None, grading=SimpleGrading(1, 1, 1)
     ):
         if name is None:
             name = f"b{len(self.blocks)}"
-        b = HexBlock(vnames, cells, name, grading)
+        b = HexBlock(vnames, nx_ny_nz, name, grading)
         self.blocks[name] = b
         return b
 
+    def add_hexblock_from_2d(
+        self,
+        vnames,
+        nx_ny_nz,
+        name=None,
+        grading=SimpleGrading(1, 1, 1),
+        suffix_zm="",
+        suffix_zp="_dz",
+    ):
+        return self.add_hexblock(
+            [vname + suffix_zm for vname in vnames]
+            + [vname + suffix_zp for vname in vnames],
+            nx_ny_nz,
+            name,
+            grading,
+        )
+
     def add_arcedge(self, vnames, name, inter_vertex):
         e = ArcEdge(vnames, name, inter_vertex)
         self.edges[name] = e
         return e
 
     def add_splineedge(self, vnames, name, points):
         e = SplineEdge(vnames, name, points)
@@ -321,14 +342,20 @@
         return e
 
     def add_boundary(self, type_, name, faces=None, neighbour=None):
         b = Boundary(type_, name, faces, neighbour)
         self.boundaries[name] = b
         return b
 
+    def add_merge_patch_pairs(self, boundary_name1: str, boundary_name2: str):
+        """Add 2 boundaries to merge"""
+        b = MergePatchPairs(boundary_name1, boundary_name2)
+        self.merge_patch_pairs[boundary_name1] = b
+        return b
+
     def add_cyclic_boundaries(self, name0, name1, faces0, faces1):
         """Add 2 cyclic boundaries
 
         Example
         -------
 
         2 cyclic boundaries can be created as follow::
@@ -412,21 +439,22 @@
             indent = " " * 4
             s = b.format(self.vertices).replace("\n", "\n" + indent)
             tmp.append(indent + s)
         tmp.append(");")
         return "\n".join(tmp)
 
     def format_mergepatchpairs_section(self):
-        # not yet implemented
-        return ""
-
-    #         return """\
-    # mergePatchPairs
-    # (
-    # );"""
+        if not self.merge_patch_pairs:
+            return ""
+        indent = " " * 4
+        tmp = ["mergePatchPairs\n("]
+        for b in self.merge_patch_pairs.values():
+            tmp.append(indent + b.format())
+        tmp.append(");")
+        return "\n" + "\n".join(tmp) + "\n"
 
     def format(self, header=DEFAULT_HEADER, sort_vortices=True):
         self.assign_vertexid(sort=sort_vortices)
         template = Template(
             r"""$header
 FoamFile
 {
```

### Comparing `fluidsimfoam-0.0.5/src/fluidsimfoam/foam_input_files/blockmesh/__pycache__/__init__.cpython-310.pyc` & `fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/blockmesh/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed May 10 08:15:22 2023 UTC, .py size: 14243 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 9a52 5b64 a337 0000  o........R[d.7..
+00000000: 6f0d 0d0a 0000 0000 2c3b 7e64 c63e 0000  o.......,;~d.>..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 c000 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 0100 6404 6405 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6406 6407 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 6d09 5a09 0100 6406 6408 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
 00000070: 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e 0100 6700  m.Z.m.Z.m.Z...g.
@@ -39,926 +39,1060 @@
 00000260: 4564 6765 2904 da0b 4564 6765 4772 6164  Edge)...EdgeGrad
 00000270: 696e 67da 0747 7261 6469 6e67 da0d 5369  ing..Grading..Si
 00000280: 6d70 6c65 4772 6164 696e 67da 1453 696d  mpleGrading..Sim
 00000290: 706c 6547 7261 6469 6e67 456c 656d 656e  pleGradingElemen
 000002a0: 7429 0672 0a00 0000 720c 0000 0072 0b00  t).r....r....r..
 000002b0: 0000 7209 0000 0072 0700 0000 7208 0000  ..r....r....r...
 000002c0: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
-000002d0: 0000 0300 0000 4000 0000 7336 0000 0065  ......@...s6...e
-000002e0: 005a 0164 005a 0264 0c64 0264 0384 015a  .Z.d.Z.d.d.d...Z
+000002d0: 0000 0300 0000 4000 0000 7346 0000 0065  ......@...sF...e
+000002e0: 005a 0164 005a 0264 1064 0264 0384 015a  .Z.d.Z.d.d.d...Z
 000002f0: 0364 0464 0584 005a 0464 0664 0784 005a  .d.d...Z.d.d...Z
 00000300: 0564 0864 0984 005a 0664 0a64 0b84 005a  .d.d...Z.d.d...Z
-00000310: 0764 0153 0029 0dda 0656 6572 7465 784e  .d.S.)...VertexN
-00000320: 6306 0000 0000 0000 0000 0000 0006 0000  c...............
-00000330: 0002 0000 0043 0000 0073 2a00 0000 7c01  .....C...s*...|.
-00000340: 7c00 5f00 7c02 7c00 5f01 7c03 7c00 5f02  |._.|.|._.|.|._.
-00000350: 7c04 7c00 5f03 7c04 6801 7c00 5f04 7c05  |.|._.|.h.|._.|.
-00000360: 7c00 5f05 6400 5300 a901 4e29 06da 0178  |._.d.S...N)...x
-00000370: da01 79da 017a da04 6e61 6d65 da05 616c  ..y..z..name..al
-00000380: 6961 73da 0569 6e64 6578 2906 da04 7365  ias..index)...se
-00000390: 6c66 720f 0000 0072 1000 0000 7211 0000  lfr....r....r...
-000003a0: 0072 1200 0000 7214 0000 00a9 0072 1600  .r....r......r..
-000003b0: 0000 fa5e 2f68 6f6d 652f 7573 6572 732f  ...^/home/users/
-000003c0: 6175 6769 6572 3370 692f 4465 762f 666c  augier3pi/Dev/fl
-000003d0: 7569 6473 696d 666f 616d 2f73 7263 2f66  uidsimfoam/src/f
-000003e0: 6c75 6964 7369 6d66 6f61 6d2f 666f 616d  luidsimfoam/foam
-000003f0: 5f69 6e70 7574 5f66 696c 6573 2f62 6c6f  _input_files/blo
-00000400: 636b 6d65 7368 2f5f 5f69 6e69 745f 5f2e  ckmesh/__init__.
-00000410: 7079 da08 5f5f 696e 6974 5f5f 1f00 0000  py..__init__....
-00000420: 730c 0000 0006 0106 0106 0106 0108 010a  s...............
-00000430: 047a 0f56 6572 7465 782e 5f5f 696e 6974  .z.Vertex.__init
-00000440: 5f5f 6301 0000 0000 0000 0000 0000 0002  __c.............
-00000450: 0000 0008 0000 0043 0000 0073 6000 0000  .......C...s`...
-00000460: 7c00 6a00 9b00 6401 7c00 6a01 9b00 9d03  |.j...d.|.j.....
-00000470: 7d01 7402 7c00 6a03 8301 6402 6b04 721c  }.t.|.j...d.k.r.
-00000480: 7c01 6403 6401 a004 7405 7c00 6a03 8301  |.d.d...t.|.j...
-00000490: a101 1700 3700 7d01 6404 7c00 6a06 6405  ....7.}.d.|.j.d.
-000004a0: 9b04 6401 7c00 6a07 6405 9b04 6401 7c00  ..d.|.j.d...d.|.
-000004b0: 6a08 6405 9b04 6406 7c01 9b00 9d08 5300  j.d...d.|.....S.
-000004c0: 2907 4eda 0120 7206 0000 007a 0320 3a20  ).N.. r....z. : 
-000004d0: fa02 2820 7a05 202e 3135 677a 0720 2920  ..( z. .15gz. ) 
-000004e0: 202f 2f20 2909 7214 0000 0072 1200 0000   // ).r....r....
-000004f0: da03 6c65 6e72 1300 0000 da04 6a6f 696e  ..lenr......join
-00000500: da06 736f 7274 6564 720f 0000 0072 1000  ..sortedr....r..
-00000510: 0000 7211 0000 0029 0272 1500 0000 da07  ..r....).r......
-00000520: 636f 6d6d 656e 7472 1600 0000 7216 0000  commentr....r...
-00000530: 0072 1700 0000 da06 666f 726d 6174 2a00  .r......format*.
-00000540: 0000 7308 0000 0012 010e 0118 0128 017a  ..s..........(.z
-00000550: 0d56 6572 7465 782e 666f 726d 6174 6302  .Vertex.formatc.
-00000560: 0000 0000 0000 0000 0000 0002 0000 0004  ................
-00000570: 0000 0043 0000 0073 2000 0000 7c00 6a00  ...C...s ...|.j.
-00000580: 7c00 6a01 7c00 6a02 6603 7c01 6a00 7c01  |.j.|.j.f.|.j.|.
-00000590: 6a01 7c01 6a02 6603 6b00 5300 720e 0000  j.|.j.f.k.S.r...
-000005a0: 00a9 0372 1100 0000 7210 0000 0072 0f00  ...r....r....r..
-000005b0: 0000 a902 7215 0000 00da 0372 6873 7216  ....r......rhsr.
-000005c0: 0000 0072 1600 0000 7217 0000 00da 065f  ...r....r......_
-000005d0: 5f6c 745f 5f30 0000 00f3 0200 0000 2001  _lt__0........ .
-000005e0: 7a0d 5665 7274 6578 2e5f 5f6c 745f 5f63  z.Vertex.__lt__c
-000005f0: 0200 0000 0000 0000 0000 0000 0200 0000  ................
-00000600: 0400 0000 4300 0000 7320 0000 007c 006a  ....C...s ...|.j
-00000610: 007c 006a 017c 006a 0266 037c 016a 007c  .|.j.|.j.f.|.j.|
-00000620: 016a 017c 016a 0266 036b 0253 0072 0e00  .j.|.j.f.k.S.r..
-00000630: 0000 7220 0000 0072 2100 0000 7216 0000  ..r ...r!...r...
-00000640: 0072 1600 0000 7217 0000 00da 065f 5f65  .r....r......__e
-00000650: 715f 5f33 0000 0072 2400 0000 7a0d 5665  q__3...r$...z.Ve
-00000660: 7274 6578 2e5f 5f65 715f 5f63 0100 0000  rtex.__eq__c....
-00000670: 0000 0000 0000 0000 0100 0000 0400 0000  ................
-00000680: 4300 0000 7314 0000 0074 007c 006a 017c  C...s....t.|.j.|
-00000690: 006a 027c 006a 0366 0383 0153 0072 0e00  .j.|.j.f...S.r..
-000006a0: 0000 2904 da04 6861 7368 7211 0000 0072  ..)...hashr....r
-000006b0: 1000 0000 720f 0000 00a9 0172 1500 0000  ....r......r....
-000006c0: 7216 0000 0072 1600 0000 7217 0000 00da  r....r....r.....
-000006d0: 085f 5f68 6173 685f 5f36 0000 0073 0200  .__hash__6...s..
-000006e0: 0000 1401 7a0f 5665 7274 6578 2e5f 5f68  ....z.Vertex.__h
-000006f0: 6173 685f 5f72 0e00 0000 2908 da08 5f5f  ash__r....)...__
-00000700: 6e61 6d65 5f5f da0a 5f5f 6d6f 6475 6c65  name__..__module
-00000710: 5f5f da0c 5f5f 7175 616c 6e61 6d65 5f5f  __..__qualname__
-00000720: 7218 0000 0072 1f00 0000 7223 0000 0072  r....r....r#...r
-00000730: 2500 0000 7228 0000 0072 1600 0000 7216  %...r(...r....r.
-00000740: 0000 0072 1600 0000 7217 0000 0072 0d00  ...r....r....r..
-00000750: 0000 1e00 0000 730c 0000 0008 000a 0108  ......s.........
-00000760: 0b08 0608 030c 0372 0d00 0000 6300 0000  .......r....c...
-00000770: 0000 0000 0000 0000 0000 0000 0002 0000  ................
-00000780: 0040 0000 00f3 1c00 0000 6500 5a01 6400  .@........e.Z.d.
-00000790: 5a02 6401 6402 8400 5a03 6403 6404 8400  Z.d.d...Z.d.d...
-000007a0: 5a04 6405 5300 2906 da05 506f 696e 7463  Z.d.S.)...Pointc
-000007b0: 0400 0000 0000 0000 0000 0000 0400 0000  ................
-000007c0: 0200 0000 4300 0000 7316 0000 007c 017c  ....C...s....|.|
-000007d0: 005f 007c 027c 005f 017c 037c 005f 0264  ._.|.|._.|.|._.d
-000007e0: 0053 0072 0e00 0000 a903 720f 0000 0072  .S.r......r....r
-000007f0: 1000 0000 7211 0000 0029 0472 1500 0000  ....r....).r....
-00000800: 720f 0000 0072 1000 0000 7211 0000 0072  r....r....r....r
-00000810: 1600 0000 7216 0000 0072 1700 0000 7218  ....r....r....r.
-00000820: 0000 003b 0000 0073 0600 0000 0601 0601  ...;...s........
-00000830: 0a01 7a0e 506f 696e 742e 5f5f 696e 6974  ..z.Point.__init
-00000840: 5f5f 6301 0000 0000 0000 0000 0000 0001  __c.............
-00000850: 0000 0007 0000 0043 0000 0073 2400 0000  .......C...s$...
-00000860: 6401 7c00 6a00 6402 9b04 6403 7c00 6a01  d.|.j.d...d.|.j.
-00000870: 6402 9b04 6403 7c00 6a02 6402 9b04 6404  d...d.|.j.d...d.
-00000880: 9d07 5300 2905 4e72 1a00 0000 7a06 3138  ..S.).Nr....z.18
-00000890: 2e31 3567 7219 0000 007a 0220 2972 2e00  .15gr....z. )r..
-000008a0: 0000 7227 0000 0072 1600 0000 7216 0000  ..r'...r....r...
-000008b0: 0072 1700 0000 721f 0000 0040 0000 0073  .r....r....@...s
-000008c0: 0200 0000 2401 7a0c 506f 696e 742e 666f  ....$.z.Point.fo
-000008d0: 726d 6174 4ea9 0572 2900 0000 722a 0000  rmatN..r)...r*..
-000008e0: 0072 2b00 0000 7218 0000 0072 1f00 0000  .r+...r....r....
-000008f0: 7216 0000 0072 1600 0000 7216 0000 0072  r....r....r....r
-00000900: 1700 0000 722d 0000 003a 0000 0073 0600  ....r-...:...s..
-00000910: 0000 0800 0801 0c05 722d 0000 0063 0000  ........r-...c..
-00000920: 0000 0000 0000 0000 0000 0000 0000 0200  ................
-00000930: 0000 4000 0000 722c 0000 0029 06da 0446  ..@...r,...)...F
-00000940: 6163 6563 0300 0000 0000 0000 0000 0000  acec............
-00000950: 0300 0000 0200 0000 4300 0000 7310 0000  ........C...s...
-00000960: 007c 017c 005f 007c 027c 005f 0164 0153  .|.|._.|.|._.d.S
-00000970: 0029 027a 380a 2020 2020 2020 2020 766e  .).z8.        vn
-00000980: 616d 6520 6973 206c 6973 7420 6f72 2074  ame is list or t
-00000990: 7570 6c65 206f 6620 7665 7274 6578 206e  uple of vertex n
-000009a0: 616d 6573 0a20 2020 2020 2020 204e 2902  ames.        N).
-000009b0: da06 766e 616d 6573 7212 0000 0029 0372  ..vnamesr....).r
-000009c0: 1500 0000 7231 0000 0072 1200 0000 7216  ....r1...r....r.
-000009d0: 0000 0072 1600 0000 7217 0000 0072 1800  ...r....r....r..
-000009e0: 0000 4500 0000 7304 0000 0006 040a 017a  ..E...s........z
-000009f0: 0d46 6163 652e 5f5f 696e 6974 5f5f 6302  .Face.__init__c.
-00000a00: 0000 0000 0000 0000 0000 0004 0000 0007  ................
-00000a10: 0000 0003 0000 0073 4600 0000 6401 a000  .......sF...d...
-00000a20: 8700 6601 6402 6403 8408 7c00 6a01 4400  ..f.d.d...|.j.D.
-00000a30: 8301 a101 7d02 6401 a000 7c00 6a01 a101  ....}.d...|.j...
-00000a40: 7d03 6404 7c02 6405 9b04 6406 7c00 6a02  }.d.|.d...d.|.j.
-00000a50: 6405 9b04 6407 7c03 6405 9b04 6408 9d07  d...d.|.d...d...
-00000a60: 5300 2909 fa4b 466f 726d 6174 2069 6e73  S.)..KFormat ins
-00000a70: 7461 6e63 6520 746f 2064 756d 700a 2020  tance to dump.  
-00000a80: 2020 2020 2020 7665 7274 6963 6573 2069        vertices i
-00000a90: 7320 6469 6374 206f 6620 6e61 6d65 2074  s dict of name t
-00000aa0: 6f20 5665 7274 6578 0a20 2020 2020 2020  o Vertex.       
-00000ab0: 2072 1900 0000 6301 0000 0000 0000 0000   r....c.........
-00000ac0: 0000 0002 0000 0004 0000 0033 0000 00f3  ...........3....
-00000ad0: 1e00 0000 8100 7c00 5d0a 7d01 7400 8800  ......|.].}.t...
-00000ae0: 7c01 1900 6a01 8301 5600 0100 7102 6400  |...j...V...q.d.
-00000af0: 5300 720e 0000 00a9 02da 0373 7472 7214  S.r........strr.
-00000b00: 0000 00a9 02da 022e 30da 0276 6ea9 01da  ........0..vn...
-00000b10: 0876 6572 7469 6365 7372 1600 0000 7217  .verticesr....r.
-00000b20: 0000 00da 093c 6765 6e65 7870 723e 5000  .....<genexpr>P.
-00000b30: 0000 f304 0000 0002 801c 007a 1e46 6163  ...........z.Fac
-00000b40: 652e 666f 726d 6174 2e3c 6c6f 6361 6c73  e.format.<locals
-00000b50: 3e2e 3c67 656e 6578 7072 3efa 0128 da01  >.<genexpr>..(..
-00000b60: 737a 0629 2020 2f2f 20fa 0220 28fa 0129  sz.)  // .. (..)
-00000b70: 2903 721c 0000 0072 3100 0000 7212 0000  ).r....r1...r...
-00000b80: 00a9 0472 1500 0000 723a 0000 0072 1400  ...r....r:...r..
-00000b90: 0000 721e 0000 0072 1600 0000 7239 0000  ..r....r....r9..
-00000ba0: 0072 1700 0000 721f 0000 004c 0000 0073  .r....r....L...s
-00000bb0: 0600 0000 1a04 0c01 2001 7a0b 4661 6365  ........ .z.Face
-00000bc0: 2e66 6f72 6d61 744e 722f 0000 0072 1600  .formatNr/...r..
-00000bd0: 0000 7216 0000 0072 1600 0000 7217 0000  ..r....r....r...
-00000be0: 0072 3000 0000 4400 0000 7306 0000 0008  .r0...D...s.....
-00000bf0: 0008 010c 0772 3000 0000 6300 0000 0000  .....r0...c.....
-00000c00: 0000 0000 0000 0000 0000 0004 0000 0040  ...............@
-00000c10: 0000 0073 3200 0000 6500 5a01 6400 5a02  ...s2...e.Z.d.Z.
-00000c20: 6503 6401 6401 6401 8303 6601 6402 6403  e.d.d.d...f.d.d.
-00000c30: 8401 5a04 6404 6405 8400 5a05 6409 6407  ..Z.d.d...Z.d.d.
-00000c40: 6408 8401 5a06 6406 5300 290a da08 4865  d...Z.d.S.)...He
-00000c50: 7842 6c6f 636b 7206 0000 0063 0500 0000  xBlockr....c....
-00000c60: 0000 0000 0000 0000 0500 0000 0200 0000  ................
-00000c70: 4300 0000 731c 0000 007c 017c 005f 007c  C...s....|.|._.|
-00000c80: 027c 005f 017c 037c 005f 027c 047c 005f  .|._.|.|._.|.|._
-00000c90: 0364 0153 0029 0261 2e01 0000 496e 6974  .d.S.).a....Init
-00000ca0: 6961 6c69 7a65 2048 6578 426c 6f63 6b20  ialize HexBlock 
-00000cb0: 696e 7374 616e 6365 0a20 2020 2020 2020  instance.       
-00000cc0: 2076 6e61 6d65 7320 6973 2074 6865 2076   vnames is the v
-00000cd0: 6572 7465 7820 6e61 6d65 7320 696e 206f  ertex names in o
-00000ce0: 7264 6572 2064 6573 6372 6976 6564 2069  rder descrived i
-00000cf0: 6e0a 2020 2020 2020 2020 2020 2020 6874  n.            ht
-00000d00: 7470 3a2f 2f77 7777 2e6f 7065 6e66 6f61  tp://www.openfoa
-00000d10: 6d2e 6f72 672f 646f 6373 2f75 7365 722f  m.org/docs/user/
-00000d20: 6d65 7368 2d64 6573 6372 6970 7469 6f6e  mesh-description
-00000d30: 2e70 6870 0a20 2020 2020 2020 2063 656c  .php.        cel
-00000d40: 6c73 2069 7320 6e75 6d62 6572 206f 6620  ls is number of 
-00000d50: 6365 6c6c 7320 6465 7669 6564 2069 6e74  cells devied int
-00000d60: 6f20 696e 2065 6163 6820 6469 7265 6374  o in each direct
-00000d70: 696f 6e0a 2020 2020 2020 2020 6e61 6d65  ion.        name
-00000d80: 2069 7320 7468 6520 756e 6971 206e 616d   is the uniq nam
-00000d90: 6520 6f66 2074 6865 2062 6c6f 636b 0a20  e of the block. 
-00000da0: 2020 2020 2020 2067 7261 6469 6e67 2069         grading i
-00000db0: 7320 6772 6164 696e 6720 6d65 7468 6f64  s grading method
-00000dc0: 2e0a 2020 2020 2020 2020 4e29 0472 3100  ..        N).r1.
-00000dd0: 0000 da05 6365 6c6c 7372 1200 0000 da07  ....cellsr......
-00000de0: 6772 6164 696e 6729 0572 1500 0000 7231  grading).r....r1
-00000df0: 0000 0072 4300 0000 7212 0000 0072 4400  ...rC...r....rD.
-00000e00: 0000 7216 0000 0072 1600 0000 7217 0000  ..r....r....r...
-00000e10: 0072 1800 0000 5600 0000 7308 0000 0006  .r....V...s.....
-00000e20: 0806 0106 010a 017a 1148 6578 426c 6f63  .......z.HexBloc
-00000e30: 6b2e 5f5f 696e 6974 5f5f 6302 0000 0000  k.__init__c.....
-00000e40: 0000 0000 0000 0004 0000 0011 0000 0003  ................
-00000e50: 0000 0073 7e00 0000 6401 a000 8700 6601  ...s~...d.....f.
-00000e60: 6402 6403 8408 7c00 6a01 4400 8301 a101  d.d...|.j.D.....
-00000e70: 7d02 6401 a000 7c00 6a01 a101 7d03 6404  }.d...|.j...}.d.
-00000e80: 7c02 9b00 6405 7c00 6a02 9b00 6406 7c00  |...d.|.j...d.|.
-00000e90: 6a03 6407 1900 6408 9b04 6401 7c00 6a03  j.d...d...d.|.j.
-00000ea0: 6409 1900 6408 9b04 6401 7c00 6a03 640a  d...d...d.|.j.d.
-00000eb0: 1900 6408 9b04 6405 7c00 6a04 a005 a100  ..d...d.|.j.....
-00000ec0: 9b00 640b 7c00 6a02 9b00 6406 7c03 9b00  ..d.|.j...d.|...
-00000ed0: 640c 9d11 5300 290d 7232 0000 0072 1900  d...S.).r2...r..
-00000ee0: 0000 6301 0000 0000 0000 0000 0000 0002  ..c.............
-00000ef0: 0000 0004 0000 0033 0000 0072 3300 0000  .......3...r3...
-00000f00: 720e 0000 0072 3400 0000 7236 0000 0072  r....r4...r6...r
-00000f10: 3900 0000 7216 0000 0072 1700 0000 723b  9...r....r....r;
-00000f20: 0000 0067 0000 0072 3c00 0000 7a22 4865  ...g...r<...z"He
-00000f30: 7842 6c6f 636b 2e66 6f72 6d61 742e 3c6c  xBlock.format.<l
-00000f40: 6f63 616c 733e 2e3c 6765 6e65 7870 723e  ocals>.<genexpr>
-00000f50: 7a05 6865 7820 287a 0229 2072 3f00 0000  z.hex (z.) r?...
-00000f60: 7201 0000 00da 0164 7206 0000 0072 0400  r......dr....r..
-00000f70: 0000 7a05 2020 2f2f 2072 4000 0000 2906  ..z.  // r@...).
-00000f80: 721c 0000 0072 3100 0000 7212 0000 0072  r....r1...r....r
-00000f90: 4300 0000 7244 0000 0072 1f00 0000 7241  C...rD...r....rA
-00000fa0: 0000 0072 1600 0000 7239 0000 0072 1700  ...r....r9...r..
-00000fb0: 0000 721f 0000 0063 0000 0073 2000 0000  ..r....c...s ...
-00000fc0: 1a04 0c01 1002 0a01 04ff 0a01 04ff 0a01  ................
-00000fd0: 04ff 0802 04fe 0402 04fe 0202 06fe 02ff  ................
-00000fe0: 7a0f 4865 7842 6c6f 636b 2e66 6f72 6d61  z.HexBlock.forma
-00000ff0: 744e 6303 0000 0000 0000 0000 0000 0008  tNc.............
-00001000: 0000 0005 0000 0003 0000 0073 f000 0000  ...........s....
-00001010: 6900 6401 6402 9301 6403 6402 9301 6404  i.d.d...d.d...d.
-00001020: 6402 9301 6405 6406 9301 6407 6406 9301  d...d.d...d.d...
-00001030: 6408 6406 9301 6409 640a 9301 640b 640a  d.d...d.d...d.d.
-00001040: 9301 640c 640a 9301 640d 640e 9301 640f  ..d.d...d.d...d.
-00001050: 640e 9301 6410 640e 9301 6411 6412 9301  d...d.d...d.d...
-00001060: 6413 6412 9301 6414 6412 9301 6415 6412  d.d...d.d...d.d.
-00001070: 9301 6416 6417 9301 6417 6417 6417 6418  ..d.d...d.d.d.d.
-00001080: 9c03 a501 7d03 6700 6419 a201 7d04 641a  ....}.g.d...}.d.
-00001090: 7d05 7400 7c01 7401 8302 724a 7c03 7c01  }.t.|.t...rJ|.|.
-000010a0: 1900 7d01 7402 8700 6601 641b 641c 8408  ..}.t...f.d.d...
-000010b0: 7c04 7c01 1900 4400 8301 8301 7d06 7c02  |.|...D.....}.|.
-000010c0: 641d 7500 7273 641e 6701 7d07 8800 6a03  d.u.rsd.g.}...j.
-000010d0: 7267 7c07 a004 8800 6a03 a101 0100 7c07  rg|.....j.....|.
-000010e0: a004 7c05 7c01 1900 a101 0100 641f a005  ..|.|.......d...
-000010f0: 7c07 a101 7d02 7406 7c06 7c02 8302 5300  |...}.t.|.|...S.
-00001100: 2920 610c 0200 0047 656e 6572 6174 6520  ) a....Generate 
-00001110: 4661 6365 206f 626a 6563 740a 2020 2020  Face object.    
-00001120: 2020 2020 696e 6465 7820 6973 206e 756d      index is num
-00001130: 6265 7220 6f72 206b 6579 776f 7264 2074  ber or keyword t
-00001140: 6f20 6964 656e 7469 6679 2074 6865 2066  o identify the f
-00001150: 6163 6520 6f66 2048 6578 0a20 2020 2020  ace of Hex.     
-00001160: 2020 2020 2020 2030 203d 2027 7727 203d         0 = 'w' =
-00001170: 2027 786d 2720 3d20 272d 3130 3027 203d   'xm' = '-100' =
-00001180: 2028 3020 3420 3720 3329 0a20 2020 2020   (0 4 7 3).     
-00001190: 2020 2020 2020 2031 203d 2027 6527 203d         1 = 'e' =
-000011a0: 2027 7870 2720 3d20 2731 3030 2720 3d20   'xp' = '100' = 
-000011b0: 2831 2032 2035 2036 290a 2020 2020 2020  (1 2 5 6).      
-000011c0: 2020 2020 2020 3220 3d20 2773 2720 3d20        2 = 's' = 
-000011d0: 2779 6d27 203d 2027 302d 3130 2720 3d20  'ym' = '0-10' = 
-000011e0: 2830 2031 2035 2034 290a 2020 2020 2020  (0 1 5 4).      
-000011f0: 2020 2020 2020 3320 3d20 276e 2720 3d20        3 = 'n' = 
-00001200: 2779 7027 203d 2027 3031 3027 203d 2028  'yp' = '010' = (
-00001210: 3220 3320 3720 3629 0a20 2020 2020 2020  2 3 7 6).       
-00001220: 2020 2020 2034 203d 2027 6227 203d 2027       4 = 'b' = '
-00001230: 7a6d 2720 3d20 2730 302d 3127 203d 2028  zm' = '00-1' = (
-00001240: 3020 3320 3220 3129 203d 2022 626f 7474  0 3 2 1) = "bott
-00001250: 6f6d 220a 2020 2020 2020 2020 2020 2020  om".            
-00001260: 3520 3d20 2774 2720 3d20 277a 7027 203d  5 = 't' = 'zp' =
-00001270: 2027 3030 3127 203d 2028 3420 3520 3620   '001' = (4 5 6 
-00001280: 3729 203d 2022 746f 7022 0a20 2020 2020  7) = "top".     
-00001290: 2020 206e 616d 6520 6973 2067 6976 656e     name is given
-000012a0: 2074 6f20 4661 6365 2069 6e73 7461 6e63   to Face instanc
-000012b0: 652e 2049 6620 6f6d 6974 7465 642c 206e  e. If omitted, n
-000012c0: 616d 6520 6973 2061 7574 6f6d 6174 6963  ame is automatic
-000012d0: 616c 6c79 0a20 2020 2020 2020 2020 2020  ally.           
-000012e0: 2067 656e 6172 6174 6965 6420 6c69 6b65   genaratied like
-000012f0: 2028 2766 2d27 202b 2073 656c 662e 6e61   ('f-' + self.na
-00001300: 6d65 202b 2027 2d77 2729 0a20 2020 2020  me + '-w').     
-00001310: 2020 20da 0177 7201 0000 00da 0278 6d7a     ..wr......xmz
-00001320: 042d 3130 30da 0165 7206 0000 00da 0278  .-100..er......x
-00001330: 70da 0331 3030 723e 0000 0072 0400 0000  p..100r>...r....
-00001340: da02 796d 7a04 302d 3130 da01 6ee9 0300  ..ymz.0-10..n...
-00001350: 0000 da02 7970 5a03 3031 30da 0162 e904  ....ypZ.010..b..
-00001360: 0000 00da 0662 6f74 746f 6dda 027a 6d7a  .....bottom..zmz
-00001370: 0430 302d 31da 0174 e905 0000 0029 03da  .00-1..t.....)..
-00001380: 0374 6f70 da02 7a70 5a03 3030 3129 0629  .top..zpZ.001).)
-00001390: 0472 0100 0000 7250 0000 00e9 0700 0000  .r....rP........
-000013a0: 724d 0000 0029 0472 0600 0000 7204 0000  rM...).r....r...
-000013b0: 00e9 0600 0000 7254 0000 0029 0472 0100  ......rT...).r..
-000013c0: 0000 7206 0000 0072 5400 0000 7250 0000  ..r....rT...rP..
-000013d0: 0029 0472 0400 0000 724d 0000 0072 5700  .).r....rM...rW.
-000013e0: 0000 7258 0000 0029 0472 0100 0000 724d  ..rX...).r....rM
-000013f0: 0000 0072 0400 0000 7206 0000 0029 0472  ...r....r....).r
-00001400: 5000 0000 7254 0000 0072 5800 0000 7257  P...rT...rX...rW
-00001410: 0000 005a 0677 6573 6e62 7463 0100 0000  ...Z.wesnbtc....
-00001420: 0000 0000 0000 0000 0200 0000 0400 0000  ................
-00001430: 1300 0000 7316 0000 0067 007c 005d 077d  ....s....g.|.].}
-00001440: 0188 006a 007c 0119 0091 0271 0253 0072  ...j.|.....q.S.r
-00001450: 1600 0000 2901 7231 0000 0029 0272 3700  ....).r1...).r7.
-00001460: 0000 da01 6972 2700 0000 7216 0000 0072  ....ir'...r....r
-00001470: 1700 0000 da0a 3c6c 6973 7463 6f6d 703e  ......<listcomp>
-00001480: 9e00 0000 7302 0000 0016 007a 2148 6578  ....s......z!Hex
-00001490: 426c 6f63 6b2e 6661 6365 2e3c 6c6f 6361  Block.face.<loca
-000014a0: 6c73 3e2e 3c6c 6973 7463 6f6d 703e 4eda  ls>.<listcomp>N.
-000014b0: 0166 da01 2d29 07da 0a69 7369 6e73 7461  .f..-)...isinsta
-000014c0: 6e63 6572 3500 0000 da05 7475 706c 6572  ncer5.....tupler
-000014d0: 1200 0000 da06 6170 7065 6e64 721c 0000  ......appendr...
-000014e0: 0072 3000 0000 2908 7215 0000 0072 1400  .r0...).r....r..
-000014f0: 0000 7212 0000 005a 0b6b 775f 746f 5f69  ..r....Z.kw_to_i
-00001500: 6e64 6578 5a0f 696e 6465 785f 746f 5f76  ndexZ.index_to_v
-00001510: 6572 7465 785a 1669 6e64 6578 5f74 6f5f  ertexZ.index_to_
-00001520: 6465 6661 756c 7473 7566 6669 7872 3100  defaultsuffixr1.
-00001530: 0000 da05 7061 7274 7372 1600 0000 7227  ....partsr....r'
-00001540: 0000 0072 1700 0000 da04 6661 6365 6f00  ...r......faceo.
-00001550: 0000 7366 0000 0002 0c04 0102 ff04 0202  ..sf............
-00001560: fe04 0302 fd04 0402 fc04 0502 fb04 0602  ................
-00001570: fa04 0702 f904 0802 f804 0902 f704 0a02  ................
-00001580: f604 0b02 f504 0c02 f404 0d02 f304 0e02  ................
-00001590: f204 0f02 f104 1002 f004 1102 ef02 1202  ................
-000015a0: 0102 0108 ec08 1604 080a 0208 011a 0208  ................
-000015b0: 0106 0106 010c 010e 010a 010a 017a 0d48  .............z.H
-000015c0: 6578 426c 6f63 6b2e 6661 6365 720e 0000  exBlock.facer...
-000015d0: 0029 0772 2900 0000 722a 0000 0072 2b00  .).r)...r*...r+.
-000015e0: 0000 720b 0000 0072 1800 0000 721f 0000  ..r....r....r...
-000015f0: 0072 6100 0000 7216 0000 0072 1600 0000  .ra...r....r....
-00001600: 7216 0000 0072 1700 0000 7242 0000 0055  r....r....rB...U
-00001610: 0000 0073 0800 0000 0800 1401 080d 0e0c  ...s............
-00001620: 7242 0000 0063 0000 0000 0000 0000 0000  rB...c..........
-00001630: 0000 0000 0000 0300 0000 4000 0000 7326  ..........@...s&
-00001640: 0000 0065 005a 0164 005a 0264 0864 0264  ...e.Z.d.Z.d.d.d
-00001650: 0384 015a 0364 0464 0584 005a 0464 0664  ...Z.d.d...Z.d.d
-00001660: 0784 005a 0564 0153 0029 09da 0842 6f75  ...Z.d.S.)...Bou
-00001670: 6e64 6172 794e 6305 0000 0000 0000 0000  ndaryNc.........
-00001680: 0000 0005 0000 0003 0000 0043 0000 0073  ...........C...s
-00001690: 3a00 0000 7c01 7c00 5f00 7c02 7c00 5f01  :...|.|._.|.|._.
-000016a0: 7c03 6401 7500 720d 6700 7d03 6e08 7402  |.d.u.r.g.}.n.t.
-000016b0: 7c03 7403 8302 7215 7c03 6701 7d03 7c03  |.t...r.|.g.}.|.
-000016c0: 7c00 5f04 7c04 7c00 5f05 6401 5300 2902  |._.|.|._.d.S.).
-000016d0: 7ac4 696e 6974 6961 6c69 7a65 2062 6f75  z.initialize bou
-000016e0: 6e64 6172 790a 2020 2020 2020 2020 7479  ndary.        ty
-000016f0: 7065 5f20 6973 2074 7970 6520 6b65 7977  pe_ is type keyw
-00001700: 6f72 6420 2877 616c 6c2c 2070 6174 6368  ord (wall, patch
-00001710: 2c20 656d 7074 792c 202e 2e29 0a20 2020  , empty, ..).   
-00001720: 2020 2020 206e 616d 6520 6973 206e 6176       name is nav
-00001730: 6520 6f66 2062 6f75 6e64 6172 7920 656d  e of boundary em
-00001740: 656c 6d65 6e74 0a20 2020 2020 2020 2066  elment.        f
-00001750: 6163 6573 2069 7320 6661 6365 7320 7768  aces is faces wh
-00001760: 6963 6820 6172 6520 6170 706c 6965 6420  ich are applied 
-00001770: 7769 7468 2074 6869 7320 626f 756e 6461  with this bounda
-00001780: 7279 2063 6f6e 6469 7469 6f6e 730a 2020  ry conditions.  
-00001790: 2020 2020 2020 4e29 06da 0574 7970 655f        N)...type_
-000017a0: 7212 0000 0072 5d00 0000 7230 0000 00da  r....r]...r0....
-000017b0: 0566 6163 6573 da09 6e65 6967 6862 6f75  .faces..neighbou
-000017c0: 7229 0572 1500 0000 7263 0000 0072 1200  r).r....rc...r..
-000017d0: 0000 7264 0000 0072 6500 0000 7216 0000  ..rd...re...r...
-000017e0: 0072 1600 0000 7217 0000 0072 1800 0000  .r....r....r....
-000017f0: a900 0000 7310 0000 0006 0606 0108 0106  ....s...........
-00001800: 010a 0106 0106 010a 017a 1142 6f75 6e64  .........z.Bound
-00001810: 6172 792e 5f5f 696e 6974 5f5f 6302 0000  ary.__init__c...
-00001820: 0000 0000 0000 0000 0002 0000 0003 0000  ................
-00001830: 0043 0000 0073 1000 0000 7c00 6a00 a001  .C...s....|.j...
-00001840: 7c01 a101 0100 6401 5300 2902 7a51 6164  |.....d.S.).zQad
-00001850: 6420 6661 6365 2069 6e73 7461 6e63 650a  d face instance.
-00001860: 2020 2020 2020 2020 6661 6365 2069 7320          face is 
-00001870: 6120 4661 6365 2069 6e73 7461 6e63 6520  a Face instance 
-00001880: 286e 6f74 206e 616d 6529 2074 6f20 6265  (not name) to be
-00001890: 2061 6464 6564 0a20 2020 2020 2020 204e   added.        N
-000018a0: 2902 7264 0000 0072 5f00 0000 2902 7215  ).rd...r_...).r.
-000018b0: 0000 0072 6100 0000 7216 0000 0072 1600  ...ra...r....r..
-000018c0: 0000 7217 0000 00da 0861 6464 5f66 6163  ..r......add_fac
-000018d0: 65b8 0000 0073 0200 0000 1004 7a11 426f  e....s......z.Bo
-000018e0: 756e 6461 7279 2e61 6464 5f66 6163 6563  undary.add_facec
-000018f0: 0200 0000 0000 0000 0000 0000 0400 0000  ................
-00001900: 0800 0000 4300 0000 7382 0000 007c 006a  ....C...s....|.j
-00001910: 0067 017d 027c 006a 0164 0175 0072 167c  .g.}.|.j.d.u.r.|
-00001920: 02a0 0264 0264 037c 006a 039b 0064 049d  ...d.d.|.j...d..
-00001930: 0317 00a1 0101 006e 107c 02a0 0264 0264  .......n.|...d.d
-00001940: 037c 006a 039b 0064 057c 006a 019b 0064  .|.j...d.|.j...d
-00001950: 049d 0517 00a1 0101 007c 006a 0444 005d  .........|.j.D.]
-00001960: 0d7d 037c 02a0 0264 067c 03a0 057c 01a1  .}.|...d.|...|..
-00001970: 019b 009d 02a1 0101 0071 297c 02a0 0264  .........q)|...d
-00001980: 07a1 0101 0064 08a0 067c 02a1 0153 0029  .....d...|...S.)
-00001990: 0972 3200 0000 4e7a 027b 0a7a 0920 2020  .r2...Nz.{.z.   
-000019a0: 2074 7970 6520 7a11 3b0a 2020 2020 6661   type z.;.    fa
-000019b0: 6365 730a 2020 2020 287a 163b 0a20 2020  ces.    (z.;.   
-000019c0: 206e 6569 6768 626f 7572 5061 7463 6820   neighbourPatch 
-000019d0: 207a 0820 2020 2020 2020 207a 0820 2020   z.        z.   
-000019e0: 2029 3b0a 7dda 010a 2907 7212 0000 0072   );.}...).r....r
-000019f0: 6500 0000 725f 0000 0072 6300 0000 7264  e...r_...rc...rd
-00001a00: 0000 0072 1f00 0000 721c 0000 0029 0472  ...r....r....).r
-00001a10: 1500 0000 723a 0000 00da 0374 6d70 725b  ....r:.....tmpr[
-00001a20: 0000 0072 1600 0000 7216 0000 0072 1700  ...r....r....r..
-00001a30: 0000 721f 0000 00be 0000 0073 1800 0000  ..r........s....
-00001a40: 0804 0a01 1a01 0402 0201 1401 02ff 04ff  ................
-00001a50: 0a04 1801 0a01 0a01 7a0f 426f 756e 6461  ........z.Bounda
-00001a60: 7279 2e66 6f72 6d61 74a9 024e 4e29 0672  ry.format..NN).r
-00001a70: 2900 0000 722a 0000 0072 2b00 0000 7218  )...r*...r+...r.
-00001a80: 0000 0072 6600 0000 721f 0000 0072 1600  ...rf...r....r..
-00001a90: 0000 7216 0000 0072 1600 0000 7217 0000  ..r....r....r...
-00001aa0: 0072 6200 0000 a800 0000 7308 0000 0008  .rb.......s.....
-00001ab0: 000a 0108 0f0c 0672 6200 0000 6300 0000  .......rb...c...
-00001ac0: 0000 0000 0000 0000 0000 0000 0005 0000  ................
-00001ad0: 0040 0000 0073 be00 0000 6500 5a01 6400  .@...s....e.Z.d.
-00001ae0: 5a02 6401 6402 8400 5a03 6403 6404 8400  Z.d.d...Z.d.d...
-00001af0: 5a04 6405 6406 8400 5a05 642a 6408 6409  Z.d.d...Z.d*d.d.
-00001b00: 8401 5a06 640a 640b 8400 5a07 640c 640d  ..Z.d.d...Z.d.d.
-00001b10: 8400 5a08 640e 640f 8400 5a09 6407 650a  ..Z.d.d...Z.d.e.
-00001b20: 6410 6410 6410 8303 6602 6411 6412 8401  d.d.d...f.d.d...
-00001b30: 5a0b 6413 6414 8400 5a0c 6415 6416 8400  Z.d.d...Z.d.d...
-00001b40: 5a0d 642b 6417 6418 8401 5a0e 6419 641a  Z.d+d.d...Z.d.d.
-00001b50: 8400 5a0f 642c 641c 641d 8401 5a10 641e  ..Z.d,d.d...Z.d.
-00001b60: 641f 8400 5a11 6420 6421 8400 5a12 6422  d...Z.d d!..Z.d"
-00001b70: 6423 8400 5a13 6424 6425 8400 5a14 6426  d#..Z.d$d%..Z.d&
-00001b80: 6427 8400 5a15 6516 641b 6602 6428 6429  d'..Z.e.d.f.d(d)
-00001b90: 8401 5a17 6407 5300 292d da0d 426c 6f63  ..Z.d.S.)-..Bloc
-00001ba0: 6b4d 6573 6844 6963 7463 0100 0000 0000  kMeshDictc......
-00001bb0: 0000 0000 0000 0100 0000 0200 0000 4300  ..............C.
-00001bc0: 0000 7328 0000 0064 017c 005f 0069 007c  ..s(...d.|._.i.|
-00001bd0: 005f 0169 007c 005f 0269 007c 005f 0369  ._.i.|._.i.|._.i
-00001be0: 007c 005f 0464 007c 005f 0564 0053 0029  .|._.d.|._.d.S.)
-00001bf0: 024e 6700 0000 0000 00f0 3f29 06da 1163  .Ng.......?)...c
-00001c00: 6f6e 7665 7274 5f74 6f5f 6d65 7465 7273  onvert_to_meters
-00001c10: 723a 0000 00da 0662 6c6f 636b 73da 0565  r:.....blocks..e
-00001c20: 6467 6573 da0a 626f 756e 6461 7269 6573  dges..boundaries
-00001c30: da16 5f76 6572 7469 6365 735f 696e 5f62  .._vertices_in_b
-00001c40: 6c6f 636b 6d65 7368 7227 0000 0072 1600  lockmeshr'...r..
-00001c50: 0000 7216 0000 0072 1700 0000 7218 0000  ..r....r....r...
-00001c60: 00d1 0000 0073 0c00 0000 0601 0601 0601  .....s..........
-00001c70: 0601 0601 0a01 7a16 426c 6f63 6b4d 6573  ......z.BlockMes
-00001c80: 6844 6963 742e 5f5f 696e 6974 5f5f 6302  hDict.__init__c.
-00001c90: 0000 0000 0000 0000 0000 0003 0000 0009  ................
-00001ca0: 0000 0043 0000 0073 2400 0000 6401 6402  ...C...s$...d.d.
-00001cb0: 6403 6404 6405 6406 6407 6407 6408 9c08  d.d.d.d.d.d.d...
-00001cc0: 7d02 7c02 7c01 1900 7c00 5f00 6409 5300  }.|.|...|._.d.S.
-00001cd0: 290a 7a22 7365 7420 7365 6c66 2e63 6f6d  ).z"set self.com
-00001ce0: 7665 7274 5f74 6f5f 6d65 7465 7273 2062  vert_to_meters b
-00001cf0: 7920 776f 7264 69e8 0300 0072 0600 0000  y wordi....r....
-00001d00: 677b 14ae 47e1 7a84 3f67 fca9 f1d2 4d62  g{..G.z.?g....Mb
-00001d10: 503f 678d edb5 a0f7 c6b0 3e67 95d6 26e8  P?g.......>g..&.
-00001d20: 0b2e 113e 67bb bdd7 d9df 7cdb 3d29 08da  ...>g.....|.=)..
-00001d30: 026b 6dda 016d da02 636d da02 6d6d da02  .km..m..cm..mm..
-00001d40: 756d da02 6e6d da01 415a 0841 6e67 7374  um..nm..AZ.Angst
-00001d50: 726f 6d4e a901 726b 0000 0029 0372 1500  romN..rk...).r..
-00001d60: 0000 5a06 6d65 7472 6963 5a17 6d65 7472  ..Z.metricZ.metr
-00001d70: 6963 7379 6d5f 746f 5f63 6f6e 7665 7273  icsym_to_convers
-00001d80: 696f 6e72 1600 0000 7216 0000 0072 1700  ionr....r....r..
-00001d90: 0000 da0a 7365 745f 6d65 7472 6963 d900  ....set_metric..
-00001da0: 0000 7314 0000 0002 0302 0102 0102 0102  ..s.............
-00001db0: 0102 0102 0102 0106 f80e 0a7a 1842 6c6f  ...........z.Blo
-00001dc0: 636b 4d65 7368 4469 6374 2e73 6574 5f6d  ckMeshDict.set_m
-00001dd0: 6574 7269 6363 0200 0000 0000 0000 0000  etricc..........
-00001de0: 0000 0200 0000 0200 0000 4300 0000 730a  ..........C...s.
-00001df0: 0000 007c 017c 005f 0064 0053 0072 0e00  ...|.|._.d.S.r..
-00001e00: 0000 7277 0000 0029 0272 1500 0000 da05  ..rw...).r......
-00001e10: 7363 616c 6572 1600 0000 7216 0000 0072  scaler....r....r
-00001e20: 1700 0000 da09 7365 745f 7363 616c 65e7  ......set_scale.
-00001e30: 0000 0073 0200 0000 0a01 7a17 426c 6f63  ...s......z.Bloc
-00001e40: 6b4d 6573 6844 6963 742e 7365 745f 7363  kMeshDict.set_sc
-00001e50: 616c 654e 6305 0000 0000 0000 0000 0000  aleNc...........
-00001e60: 0006 0000 0005 0000 0043 0000 0073 5800  .........C...sX.
-00001e70: 0000 7400 7c01 7401 8302 721b 7402 6401  ..t.|.t...r.t.d.
-00001e80: 6402 8400 7c02 7c03 7c04 6603 4400 8301  d...|.|.|.f.D...
-00001e90: 8301 7215 7403 6403 8301 8201 7c01 7d05  ..r.t.d.....|.}.
-00001ea0: 7c05 6a04 7d04 6e07 7401 7c01 7c02 7c03  |.j.}.n.t.|.|.|.
-00001eb0: 7c04 8304 7d05 7c05 7c00 6a05 7c04 3c00  |...}.|.|.j.|.<.
-00001ec0: 7c00 6a05 7c04 1900 5300 2904 7ab2 6164  |.j.|...S.).z.ad
-00001ed0: 6420 7665 7274 6578 2062 7920 636f 6f72  d vertex by coor
-00001ee0: 6469 6e61 7465 2061 6e64 2075 6e69 7120  dinate and uniq 
-00001ef0: 6e61 6d65 0a20 2020 2020 2020 2078 2079  name.        x y
-00001f00: 207a 2069 7320 636f 6f72 6469 6e61 7465   z is coordinate
-00001f10: 7320 6f66 2076 6572 7465 780a 2020 2020  s of vertex.    
-00001f20: 2020 2020 6e61 6d65 2069 7320 756e 6971      name is uniq
-00001f30: 206e 616d 6520 746f 2072 6566 6572 2074   name to refer t
-00001f40: 6865 2076 6572 7465 780a 2020 2020 2020  he vertex.      
-00001f50: 2020 7265 7475 726e 7320 5665 7274 6578    returns Vertex
-00001f60: 206f 626a 6563 7420 7768 6963 6920 6973   object whici is
-00001f70: 2061 6464 6564 2e0a 2020 2020 2020 2020   added..        
-00001f80: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
-00001f90: 0003 0000 0073 0000 0073 1800 0000 8100  .....s...s......
-00001fa0: 7c00 5d07 7d01 7c01 6400 7501 5600 0100  |.].}.|.d.u.V...
-00001fb0: 7102 6400 5300 720e 0000 0072 1600 0000  q.d.S.r....r....
-00001fc0: 2902 7237 0000 00da 0361 7267 7216 0000  ).r7.....argr...
-00001fd0: 0072 1600 0000 7217 0000 0072 3b00 0000  .r....r....r;...
-00001fe0: f100 0000 7304 0000 0002 8016 007a 2b42  ....s........z+B
-00001ff0: 6c6f 636b 4d65 7368 4469 6374 2e61 6464  lockMeshDict.add
-00002000: 5f76 6572 7465 782e 3c6c 6f63 616c 733e  _vertex.<locals>
-00002010: 2e3c 6765 6e65 7870 723e 7a40 7820 6973  .<genexpr>z@x is
-00002020: 2061 2056 6572 7465 7820 616e 6420 6061   a Vertex and `a
-00002030: 6e79 2861 7267 2069 7320 6e6f 7420 4e6f  ny(arg is not No
-00002040: 6e65 2066 6f72 2061 7267 2069 6e20 2879  ne for arg in (y
-00002050: 2c20 7a2c 206e 616d 6529 2960 2906 725d  , z, name))`).r]
-00002060: 0000 0072 0d00 0000 da03 616e 79da 0a56  ...r......any..V
-00002070: 616c 7565 4572 726f 7272 1200 0000 723a  alueErrorr....r:
-00002080: 0000 0029 0672 1500 0000 720f 0000 0072  ...).r....r....r
-00002090: 1000 0000 7211 0000 0072 1200 0000 5a06  ....r....r....Z.
-000020a0: 7665 7274 6578 7216 0000 0072 1600 0000  vertexr....r....
-000020b0: 7217 0000 00da 0a61 6464 5f76 6572 7465  r......add_verte
-000020c0: 78ea 0000 0073 1400 0000 0a06 1801 0201  x....s..........
-000020d0: 0201 04ff 0404 0801 0e02 0a01 0a01 7a18  ..............z.
-000020e0: 426c 6f63 6b4d 6573 6844 6963 742e 6164  BlockMeshDict.ad
-000020f0: 645f 7665 7274 6578 6302 0000 0000 0000  d_vertexc.......
-00002100: 0000 0000 0002 0000 0002 0000 0043 0000  .............C..
-00002110: 0073 0c00 0000 7c00 6a00 7c01 3d00 6401  .s....|.j.|.=.d.
-00002120: 5300 2902 7a1f 6465 6c20 6e61 6d65 206b  S.).z.del name k
-00002130: 6579 2066 726f 6d20 7365 6c66 2e76 6572  ey from self.ver
-00002140: 7469 6365 734e 7239 0000 0029 0272 1500  ticesNr9...).r..
-00002150: 0000 7212 0000 0072 1600 0000 7216 0000  ..r....r....r...
-00002160: 0072 1700 0000 da0a 6465 6c5f 7665 7274  .r......del_vert
-00002170: 6578 fd00 0000 7302 0000 000c 027a 1842  ex....s......z.B
-00002180: 6c6f 636b 4d65 7368 4469 6374 2e64 656c  lockMeshDict.del
-00002190: 5f76 6572 7465 7863 0200 0000 0000 0000  _vertexc........
-000021a0: 0000 0000 0600 0000 0400 0000 4700 0000  ............G...
-000021b0: 733a 0000 007c 006a 007c 0119 007d 037c  s:...|.j.|...}.|
-000021c0: 0244 005d 137d 047c 006a 007c 0419 007d  .D.].}.|.j.|...}
-000021d0: 057c 036a 01a0 027c 056a 01a1 0101 007c  .|.j...|.j.....|
-000021e0: 037c 006a 007c 043c 0071 0764 0153 0029  .|.j.|.<.q.d.S.)
-000021f0: 027a e274 7265 6174 206e 616d 6531 2c20  .z.treat name1, 
-00002200: 6e61 6d65 322c 202e 2e2e 2061 7320 7361  name2, ... as sa
-00002210: 6d65 2070 6f69 6e74 2e0a 0a20 2020 2020  me point...     
-00002220: 2020 206e 616d 6532 2e61 6c69 6173 2c20     name2.alias, 
-00002230: 6e61 6d65 332e 616c 6961 732c 202e 2e2e  name3.alias, ...
-00002240: 2061 7265 206d 6572 6765 6420 7769 7468   are merged with
-00002250: 206e 616d 6531 2e61 6c69 6173 0a20 2020   name1.alias.   
-00002260: 2020 2020 2074 6865 206b 6579 206e 616d       the key nam
-00002270: 6532 2c20 6e61 6d65 332c 202e 2e2e 2069  e2, name3, ... i
-00002280: 6e20 7365 6c66 2e76 6572 7469 6365 7320  n self.vertices 
-00002290: 6172 6520 6b65 7074 2061 6e64 206d 6170  are kept and map
-000022a0: 7065 6420 746f 0a20 2020 2020 2020 2073  ped to.        s
-000022b0: 616d 6520 5665 7274 6578 2069 6e73 7461  ame Vertex insta
-000022c0: 6e63 6520 6173 206e 616d 6531 0a20 2020  nce as name1.   
-000022d0: 2020 2020 204e 2903 723a 0000 0072 1300       N).r:...r..
-000022e0: 0000 da06 7570 6461 7465 2906 7215 0000  ....update).r...
-000022f0: 00da 056e 616d 6531 da05 6e61 6d65 73da  ...name1..names.
-00002300: 0176 724c 0000 0072 4600 0000 7216 0000  .vrL...rF...r...
-00002310: 0072 1600 0000 7217 0000 00da 0d72 6564  .r....r......red
-00002320: 7563 655f 7665 7274 6578 0101 0000 730c  uce_vertex....s.
-00002330: 0000 000a 0708 010a 010e 010c 0204 fc7a  ...............z
-00002340: 1b42 6c6f 636b 4d65 7368 4469 6374 2e72  .BlockMeshDict.r
-00002350: 6564 7563 655f 7665 7274 6578 6301 0000  educe_vertexc...
-00002360: 0000 0000 0000 0000 0007 0000 0005 0000  ................
-00002370: 0043 0000 0073 7800 0000 7400 7401 7c00  .C...sx...t.t.|.
-00002380: 6a02 a003 a100 8301 6401 6402 8400 6403  j.......d.d...d.
-00002390: 8d02 7d01 6700 7d02 7404 7c01 6404 6402  ..}.g.}.t.|.d.d.
-000023a0: 8400 8302 4400 5d0b 5c02 7d03 7d04 7c02  ....D.].\.}.}.|.
-000023b0: a005 7401 7c04 8301 a101 0100 7116 7c02  ..t.|.......q.|.
-000023c0: 4400 5d15 7d05 7406 7c05 8301 6405 6b02  D.].}.t.|...d.k.
-000023d0: 722d 7124 6406 6407 8400 7c05 4400 8301  r-q$d.d...|.D...
-000023e0: 7d06 7c00 6a07 7c06 8e00 0100 7124 6408  }.|.j.|.....q$d.
-000023f0: 5300 2909 7a39 6361 6c6c 2072 6564 7563  S.).z9call reduc
-00002400: 655f 7665 7274 6578 206f 6e20 616c 6c20  e_vertex on all 
-00002410: 7665 7274 6963 6573 2077 6974 6820 6964  vertices with id
-00002420: 656e 7469 6361 6c20 7661 6c75 6573 2e63  entical values.c
-00002430: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-00002440: 0300 0000 5300 0000 f30c 0000 0074 007c  ....S........t.|
-00002450: 0064 0119 0083 0153 00a9 024e 7206 0000  .d.....S...Nr...
-00002460: 00a9 0172 2600 0000 a901 7283 0000 0072  ...r&.....r....r
-00002470: 1600 0000 7216 0000 0072 1700 0000 da08  ....r....r......
-00002480: 3c6c 616d 6264 613e 1401 0000 f302 0000  <lambda>........
-00002490: 000c 007a 2e42 6c6f 636b 4d65 7368 4469  ...z.BlockMeshDi
-000024a0: 6374 2e6d 6572 6765 5f76 6572 7469 6365  ct.merge_vertice
-000024b0: 732e 3c6c 6f63 616c 733e 2e3c 6c61 6d62  s.<locals>.<lamb
-000024c0: 6461 3e29 01da 036b 6579 6301 0000 0000  da>)...keyc.....
-000024d0: 0000 0000 0000 0001 0000 0003 0000 0053  ...............S
-000024e0: 0000 0072 8500 0000 7286 0000 0072 8700  ...r....r....r..
-000024f0: 0000 7288 0000 0072 1600 0000 7216 0000  ..r....r....r...
-00002500: 0072 1700 0000 7289 0000 0017 0100 0072  .r....r........r
-00002510: 8a00 0000 7206 0000 0063 0100 0000 0000  ....r....c......
-00002520: 0000 0000 0000 0200 0000 0400 0000 5300  ..............S.
-00002530: 0000 7314 0000 0067 007c 005d 067d 017c  ..s....g.|.].}.|
-00002540: 0164 0019 0091 0271 0253 0029 0172 0100  .d.....q.S.).r..
-00002550: 0000 7216 0000 0029 0272 3700 0000 7283  ..r....).r7...r.
-00002560: 0000 0072 1600 0000 7216 0000 0072 1700  ...r....r....r..
-00002570: 0000 725a 0000 001c 0100 0073 0200 0000  ..rZ.......s....
-00002580: 1400 7a30 426c 6f63 6b4d 6573 6844 6963  ..z0BlockMeshDic
-00002590: 742e 6d65 7267 655f 7665 7274 6963 6573  t.merge_vertices
-000025a0: 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973 7463  .<locals>.<listc
-000025b0: 6f6d 703e 4e29 0872 1d00 0000 da04 6c69  omp>N).r......li
-000025c0: 7374 723a 0000 00da 0569 7465 6d73 7202  str:.....itemsr.
-000025d0: 0000 0072 5f00 0000 721b 0000 0072 8400  ...r_...r....r..
-000025e0: 0000 2907 7215 0000 005a 0f73 6f72 7465  ..).r....Z.sorte
-000025f0: 645f 7665 7274 6963 6573 da06 6772 6f75  d_vertices..grou
-00002600: 7073 da01 6bda 0167 da05 6772 6f75 7072  ps..k..g..groupr
-00002610: 8200 0000 7216 0000 0072 1600 0000 7217  ....r....r....r.
-00002620: 0000 00da 0e6d 6572 6765 5f76 6572 7469  .....merge_verti
-00002630: 6365 730f 0100 0073 1800 0000 0204 1201  ces....s........
-00002640: 06ff 0403 1601 1001 0801 0c01 0201 0e01  ................
-00002650: 0c01 04fc 7a1c 426c 6f63 6b4d 6573 6844  ....z.BlockMeshD
-00002660: 6963 742e 6d65 7267 655f 7665 7274 6963  ict.merge_vertic
-00002670: 6573 7206 0000 0063 0500 0000 0000 0000  esr....c........
-00002680: 0000 0000 0600 0000 0500 0000 4300 0000  ............C...
-00002690: 7334 0000 007c 0364 0075 0072 0c64 0174  s4...|.d.u.r.d.t
-000026a0: 007c 006a 0183 019b 009d 027d 0374 027c  .|.j.......}.t.|
-000026b0: 017c 027c 037c 0483 047d 057c 057c 006a  .|.|.|...}.|.|.j
-000026c0: 017c 033c 007c 0553 0029 024e 724f 0000  .|.<.|.S.).NrO..
-000026d0: 0029 0372 1b00 0000 726c 0000 0072 4200  .).r....rl...rB.
-000026e0: 0000 2906 7215 0000 0072 3100 0000 7243  ..).r....r1...rC
-000026f0: 0000 0072 1200 0000 7244 0000 0072 4f00  ...r....rD...rO.
-00002700: 0000 7216 0000 0072 1600 0000 7217 0000  ..r....r....r...
-00002710: 00da 0c61 6464 5f68 6578 626c 6f63 6b1f  ...add_hexblock.
-00002720: 0100 0073 0a00 0000 0803 1001 0e01 0a01  ...s............
-00002730: 0401 7a1a 426c 6f63 6b4d 6573 6844 6963  ..z.BlockMeshDic
-00002740: 742e 6164 645f 6865 7862 6c6f 636b 6304  t.add_hexblockc.
-00002750: 0000 0000 0000 0000 0000 0005 0000 0004  ................
-00002760: 0000 0043 0000 00f3 1a00 0000 7400 7c01  ...C........t.|.
-00002770: 7c02 7c03 8303 7d04 7c04 7c00 6a01 7c02  |.|...}.|.|.j.|.
-00002780: 3c00 7c04 5300 720e 0000 0029 0272 0700  <.|.S.r....).r..
-00002790: 0000 726d 0000 0029 0572 1500 0000 7231  ..rm...).r....r1
-000027a0: 0000 0072 1200 0000 5a0c 696e 7465 725f  ...r....Z.inter_
-000027b0: 7665 7274 6578 7248 0000 0072 1600 0000  vertexrH...r....
-000027c0: 7216 0000 0072 1700 0000 da0b 6164 645f  r....r......add_
-000027d0: 6172 6365 6467 6528 0100 00f3 0600 0000  arcedge(........
-000027e0: 0c01 0a01 0401 7a19 426c 6f63 6b4d 6573  ......z.BlockMes
-000027f0: 6844 6963 742e 6164 645f 6172 6365 6467  hDict.add_arcedg
-00002800: 6563 0400 0000 0000 0000 0000 0000 0500  ec..............
-00002810: 0000 0400 0000 4300 0000 7294 0000 0072  ......C...r....r
-00002820: 0e00 0000 2902 7208 0000 0072 6d00 0000  ....).r....rm...
-00002830: 2905 7215 0000 0072 3100 0000 7212 0000  ).r....r1...r...
-00002840: 00da 0670 6f69 6e74 7372 4800 0000 7216  ...pointsrH...r.
-00002850: 0000 0072 1600 0000 7217 0000 00da 0e61  ...r....r......a
-00002860: 6464 5f73 706c 696e 6565 6467 652d 0100  dd_splineedge-..
-00002870: 0072 9600 0000 7a1c 426c 6f63 6b4d 6573  .r....z.BlockMes
-00002880: 6844 6963 742e 6164 645f 7370 6c69 6e65  hDict.add_spline
-00002890: 6564 6765 6305 0000 0000 0000 0000 0000  edgec...........
-000028a0: 0006 0000 0005 0000 0043 0000 0073 1c00  .........C...s..
-000028b0: 0000 7400 7c01 7c02 7c03 7c04 8304 7d05  ..t.|.|.|.|...}.
-000028c0: 7c05 7c00 6a01 7c02 3c00 7c05 5300 720e  |.|.j.|.<.|.S.r.
-000028d0: 0000 0029 0272 6200 0000 726e 0000 0029  ...).rb...rn...)
-000028e0: 0672 1500 0000 7263 0000 0072 1200 0000  .r....rc...r....
-000028f0: 7264 0000 0072 6500 0000 724f 0000 0072  rd...re...rO...r
-00002900: 1600 0000 7216 0000 0072 1700 0000 da0c  ....r....r......
-00002910: 6164 645f 626f 756e 6461 7279 3201 0000  add_boundary2...
-00002920: 7306 0000 000e 010a 0104 017a 1a42 6c6f  s..........z.Blo
-00002930: 636b 4d65 7368 4469 6374 2e61 6464 5f62  ckMeshDict.add_b
-00002940: 6f75 6e64 6172 7963 0500 0000 0000 0000  oundaryc........
-00002950: 0000 0000 0700 0000 0600 0000 4300 0000  ............C...
-00002960: 732c 0000 007c 006a 0064 017c 017c 037c  s,...|.j.d.|.|.|
-00002970: 0264 028d 047d 057c 006a 0064 017c 027c  .d...}.|.j.d.|.|
-00002980: 047c 0164 028d 047d 067c 057c 0666 0253  .|.d...}.|.|.f.S
-00002990: 0029 034e da06 6379 636c 6963 2901 7265  .).N..cyclic).re
-000029a0: 0000 0029 0172 9900 0000 2907 7215 0000  ...).r....).r...
-000029b0: 005a 056e 616d 6530 7281 0000 005a 0666  .Z.name0r....Z.f
-000029c0: 6163 6573 305a 0666 6163 6573 31da 0262  aces0Z.faces1..b
-000029d0: 30da 0262 3172 1600 0000 7216 0000 0072  0..b1r....r....r
-000029e0: 1700 0000 da15 6164 645f 6379 636c 6963  ......add_cyclic
-000029f0: 5f62 6f75 6e64 6172 6965 7337 0100 0073  _boundaries7...s
-00002a00: 0600 0000 1201 1201 0801 7a23 426c 6f63  ..........z#Bloc
-00002a10: 6b4d 6573 6844 6963 742e 6164 645f 6379  kMeshDict.add_cy
-00002a20: 636c 6963 5f62 6f75 6e64 6172 6965 7354  clic_boundariesT
-00002a30: 6302 0000 0000 0000 0000 0000 0008 0000  c...............
-00002a40: 0005 0000 0043 0000 0073 ba00 0000 7400  .....C...s....t.
-00002a50: 8300 7d02 6700 7c00 5f01 7c00 6a02 a003  ..}.g.|._.|.j...
-00002a60: a100 4400 5d1e 7d03 7c03 6a04 4400 5d18  ..D.].}.|.j.D.].
-00002a70: 7d04 7c00 6a05 7c04 1900 7d05 7c05 6a06  }.|.j.|...}.|.j.
-00002a80: 7c02 7601 7228 7c02 a007 7c05 6a06 a101  |.v.r(|...|.j...
-00002a90: 0100 7c00 6a01 a008 7c05 a101 0100 7110  ..|.j...|.....q.
-00002aa0: 710b 7c01 6401 6b02 7246 6700 7c00 5f01  q.|.d.k.rFg.|._.
-00002ab0: 7c00 6a05 a009 a100 4400 5d0e 5c02 7d06  |.j.....D.].\.}.
-00002ac0: 7d05 7c06 7c02 7600 7244 7c00 6a01 a008  }.|.|.v.rD|.j...
-00002ad0: 7c05 a101 0100 7136 6e08 7c01 724e 740a  |.....q6n.|.rNt.
-00002ae0: 7c00 6a01 8301 7c00 5f01 740b 7c00 6a01  |.j...|._.t.|.j.
-00002af0: 8301 4400 5d07 5c02 7d07 7d05 7c07 7c05  ..D.].\.}.}.|.|.
-00002b00: 5f0c 7153 6402 5300 2903 7ae3 312e 2063  _.qSd.S.).z.1. c
-00002b10: 7265 6174 6520 6c69 7374 206f 6620 5665  reate list of Ve
-00002b20: 7274 6578 2077 6869 6368 2061 7265 2072  rtex which are r
-00002b30: 6566 6572 7265 6420 6279 2062 6c6f 636b  eferred by block
-00002b40: 7320 6f6e 6c79 2e0a 2020 2020 2020 2020  s only..        
-00002b50: 322e 2073 6f72 7420 7665 7274 6578 2061  2. sort vertex a
-00002b60: 6363 6f72 6469 6e67 2074 6f20 2878 2c20  ccording to (x, 
-00002b70: 792c 207a 290a 2020 2020 2020 2020 332e  y, z).        3.
-00002b80: 2061 7373 6967 6e20 7365 7175 656e 6365   assign sequence
-00002b90: 206e 756d 6265 7220 666f 7220 6561 6368   number for each
-00002ba0: 2056 6572 7465 780a 2020 2020 2020 2020   Vertex.        
-00002bb0: 342e 2073 6f72 7465 6420 6c69 7374 2069  4. sorted list i
-00002bc0: 7320 7361 7665 6420 6173 2073 656c 662e  s saved as self.
-00002bd0: 5f76 6572 7469 6365 735f 696e 5f62 6c6f  _vertices_in_blo
-00002be0: 636b 6d65 7368 0a20 2020 2020 2020 205a  ckmesh.        Z
-00002bf0: 0861 735f 6164 6465 644e 290d da03 7365  .as_addedN)...se
-00002c00: 7472 6f00 0000 726c 0000 00da 0676 616c  tro...rl.....val
-00002c10: 7565 7372 3100 0000 723a 0000 0072 1200  uesr1...r:...r..
-00002c20: 0000 da03 6164 6472 5f00 0000 728d 0000  ....addr_...r...
-00002c30: 0072 1d00 0000 da09 656e 756d 6572 6174  .r......enumerat
-00002c40: 6572 1400 0000 2908 7215 0000 00da 0473  er....).r......s
-00002c50: 6f72 745a 0b76 6e61 6d65 735f 6b65 7074  ortZ.vnames_kept
-00002c60: 724f 0000 0072 4c00 0000 7283 0000 00da  rO...rL...r.....
-00002c70: 0576 6e61 6d65 7259 0000 0072 1600 0000  .vnamerY...r....
-00002c80: 7216 0000 0072 1700 0000 da0f 6173 7369  r....r......assi
-00002c90: 676e 5f76 6572 7465 7869 643c 0100 0073  gn_vertexid<...s
-00002ca0: 2c00 0000 0607 0601 0e01 0a01 0a01 0a01  ,...............
-00002cb0: 0c01 0c01 0280 02fc 0805 0601 1201 0801  ................
-00002cc0: 0c01 0280 02fe 0403 0c01 1201 0801 04ff  ................
-00002cd0: 7a1d 426c 6f63 6b4d 6573 6844 6963 742e  z.BlockMeshDict.
-00002ce0: 6173 7369 676e 5f76 6572 7465 7869 6463  assign_vertexidc
-00002cf0: 0100 0000 0000 0000 0000 0000 0300 0000  ................
-00002d00: 0600 0000 4300 0000 7338 0000 0064 0167  ....C...s8...d.g
-00002d10: 017d 017c 006a 0044 005d 0b7d 027c 01a0  .}.|.j.D.].}.|..
-00002d20: 0164 027c 02a0 02a1 0017 00a1 0101 0071  .d.|...........q
-00002d30: 067c 01a0 0164 03a1 0101 0064 04a0 037c  .|...d.....d...|
-00002d40: 01a1 0153 0029 057a ec66 6f72 6d61 7420  ...S.).z.format 
-00002d50: 7665 7274 6963 6573 2073 6563 7469 6f6e  vertices section
-00002d60: 2e0a 2020 2020 2020 2020 6173 7369 676e  ..        assign
-00002d70: 5f76 6572 7465 7869 6428 2920 7368 6f75  _vertexid() shou
-00002d80: 6c64 2062 6520 6361 6c6c 6564 2062 6566  ld be called bef
-00002d90: 6f72 6520 7468 6973 206d 6574 686f 642c  ore this method,
-00002da0: 2062 6563 6175 7365 0a20 2020 2020 2020   because.       
-00002db0: 2073 656c 662e 5f76 6572 7469 6365 735f   self._vertices_
-00002dc0: 696e 5f62 6c6f 636b 6d65 7368 2073 686f  in_blockmesh sho
-00002dd0: 756c 6420 6265 2061 7661 696c 6162 6c65  uld be available
-00002de0: 2061 6e64 0a20 2020 2020 2020 206d 656d   and.        mem
-00002df0: 6265 7273 206f 6620 7365 6c66 2e5f 7665  bers of self._ve
-00002e00: 7274 6963 6573 5f69 6e5f 626c 6f63 6b6d  rtices_in_blockm
-00002e10: 6573 6820 7368 6f75 6c64 2068 6176 6520  esh should have 
-00002e20: 7661 6c69 6420 696e 6465 782e 0a20 2020  valid index..   
-00002e30: 2020 2020 207a 0a76 6572 7469 6365 730a       z.vertices.
-00002e40: 28fa 0420 2020 20fa 0229 3b72 6700 0000  (..    ..);rg...
-00002e50: 2904 726f 0000 0072 5f00 0000 721f 0000  ).ro...r_...r...
-00002e60: 0072 1c00 0000 2903 7215 0000 0072 6800  .r....).r....rh.
-00002e70: 0000 7283 0000 0072 1600 0000 7216 0000  ..r....r....r...
-00002e80: 0072 1700 0000 da17 666f 726d 6174 5f76  .r......format_v
-00002e90: 6572 7469 6365 735f 7365 6374 696f 6e55  ertices_sectionU
-00002ea0: 0100 0073 0a00 0000 0606 0a01 1401 0a01  ...s............
-00002eb0: 0a01 7a25 426c 6f63 6b4d 6573 6844 6963  ..z%BlockMeshDic
-00002ec0: 742e 666f 726d 6174 5f76 6572 7469 6365  t.format_vertice
-00002ed0: 735f 7365 6374 696f 6e63 0100 0000 0000  s_sectionc......
-00002ee0: 0000 0000 0000 0300 0000 0700 0000 4300  ..............C.
-00002ef0: 0000 f340 0000 0064 0167 017d 017c 006a  ...@...d.g.}.|.j
-00002f00: 00a0 01a1 0044 005d 0d7d 027c 01a0 0264  .....D.].}.|...d
-00002f10: 027c 02a0 037c 006a 04a1 0117 00a1 0101  .|...|.j........
-00002f20: 0071 087c 01a0 0264 03a1 0101 0064 04a0  .q.|...d.....d..
-00002f30: 057c 01a1 0153 0029 057a a266 6f72 6d61  .|...S.).z.forma
-00002f40: 7420 626c 6f63 6b73 2073 6563 7469 6f6e  t blocks section
-00002f50: 2e0a 2020 2020 2020 2020 6173 7369 676e  ..        assign
-00002f60: 5f76 6572 7465 7869 6428 2920 7368 6f75  _vertexid() shou
-00002f70: 6c64 2062 6520 6361 6c6c 6564 2062 6566  ld be called bef
-00002f80: 6f72 6520 7468 6973 206d 6574 686f 642c  ore this method,
-00002f90: 2062 6563 6175 7365 0a20 2020 2020 2020   because.       
-00002fa0: 2076 6572 7469 6365 7320 7265 6665 7265   vertices refere
-00002fb0: 6420 6279 2062 6c6f 636b 7320 7368 6f75  d by blocks shou
-00002fc0: 6c64 2068 6176 6520 7661 6c69 6420 696e  ld have valid in
-00002fd0: 6465 782e 0a20 2020 2020 2020 207a 0862  dex..        z.b
-00002fe0: 6c6f 636b 730a 2872 a500 0000 72a6 0000  locks.(r....r...
-00002ff0: 0072 6700 0000 2906 726c 0000 0072 9f00  .rg...).rl...r..
-00003000: 0000 725f 0000 0072 1f00 0000 723a 0000  ..r_...r....r:..
-00003010: 0072 1c00 0000 2903 7215 0000 0072 6800  .r....).r....rh.
-00003020: 0000 724f 0000 0072 1600 0000 7216 0000  ..rO...r....r...
-00003030: 0072 1700 0000 da15 666f 726d 6174 5f62  .r......format_b
-00003040: 6c6f 636b 735f 7365 6374 696f 6e61 0100  locks_sectiona..
-00003050: 0073 0a00 0000 0605 0e01 1801 0a01 0a01  .s..............
-00003060: 7a23 426c 6f63 6b4d 6573 6844 6963 742e  z#BlockMeshDict.
-00003070: 666f 726d 6174 5f62 6c6f 636b 735f 7365  format_blocks_se
-00003080: 6374 696f 6e63 0100 0000 0000 0000 0000  ctionc..........
-00003090: 0000 0300 0000 0700 0000 4300 0000 72a8  ..........C...r.
-000030a0: 0000 0029 057a a166 6f72 6d61 7420 6564  ...).z.format ed
-000030b0: 6765 7320 7365 6374 696f 6e2e 0a20 2020  ges section..   
-000030c0: 2020 2020 2061 7373 6967 6e5f 7665 7274       assign_vert
-000030d0: 6578 6964 2829 2073 686f 756c 6420 6265  exid() should be
-000030e0: 2063 616c 6c65 6420 6265 666f 7265 2074   called before t
-000030f0: 6869 7320 6d65 7468 6f64 2c20 6265 6361  his method, beca
-00003100: 7573 650a 2020 2020 2020 2020 7665 7274  use.        vert
-00003110: 6963 6573 2072 6566 6572 6564 2062 7920  ices refered by 
-00003120: 626c 6f63 6b73 2073 686f 756c 6420 6861  blocks should ha
-00003130: 7665 2076 616c 6964 2069 6e64 6578 2e0a  ve valid index..
-00003140: 2020 2020 2020 2020 7a07 6564 6765 730a          z.edges.
-00003150: 2872 a500 0000 72a6 0000 0072 6700 0000  (r....r....rg...
-00003160: 2906 726d 0000 0072 9f00 0000 725f 0000  ).rm...r....r_..
-00003170: 0072 1f00 0000 723a 0000 0072 1c00 0000  .r....r:...r....
-00003180: 2903 7215 0000 0072 6800 0000 7248 0000  ).r....rh...rH..
-00003190: 0072 1600 0000 7216 0000 0072 1700 0000  .r....r....r....
-000031a0: da14 666f 726d 6174 5f65 6467 6573 5f73  ..format_edges_s
-000031b0: 6563 7469 6f6e 6c01 0000 730a 0000 0006  ectionl...s.....
-000031c0: 060e 0118 010a 010a 017a 2242 6c6f 636b  .........z"Block
-000031d0: 4d65 7368 4469 6374 2e66 6f72 6d61 745f  MeshDict.format_
-000031e0: 6564 6765 735f 7365 6374 696f 6e63 0100  edges_sectionc..
-000031f0: 0000 0000 0000 0000 0000 0500 0000 0600  ................
-00003200: 0000 4300 0000 7354 0000 0064 0167 017d  ..C...sT...d.g.}
-00003210: 017c 006a 00a0 01a1 0044 005d 177d 0264  .|.j.....D.].}.d
-00003220: 027d 037c 02a0 027c 006a 03a1 01a0 0464  .}.|...|.j.....d
-00003230: 0364 037c 0317 00a1 027d 047c 01a0 057c  .d.|.....}.|...|
-00003240: 037c 0417 00a1 0101 0071 087c 01a0 0564  .|.......q.|...d
-00003250: 04a1 0101 0064 03a0 067c 01a1 0153 0029  .....d...|...S.)
-00003260: 057a a366 6f72 6d61 7420 626f 756e 6461  .z.format bounda
-00003270: 7279 2073 6563 7469 6f6e 2e0a 2020 2020  ry section..    
-00003280: 2020 2020 6173 7369 676e 5f76 6572 7465      assign_verte
-00003290: 7869 6428 2920 7368 6f75 6c64 2062 6520  xid() should be 
-000032a0: 6361 6c6c 6564 2062 6566 6f72 6520 7468  called before th
-000032b0: 6973 206d 6574 686f 642c 2062 6563 6175  is method, becau
-000032c0: 7365 0a20 2020 2020 2020 2076 6572 7469  se.        verti
-000032d0: 6365 7320 7265 6665 7265 6420 6279 2066  ces refered by f
-000032e0: 6163 6573 2073 686f 756c 6420 6861 7665  aces should have
-000032f0: 2076 616c 6964 2069 6e64 6578 2e0a 2020   valid index..  
-00003300: 2020 2020 2020 7a0a 626f 756e 6461 7279        z.boundary
-00003310: 0a28 72a5 0000 0072 6700 0000 72a6 0000  .(r....rg...r...
-00003320: 0029 0772 6e00 0000 729f 0000 0072 1f00  .).rn...r....r..
-00003330: 0000 723a 0000 00da 0772 6570 6c61 6365  ..r:.....replace
-00003340: 725f 0000 0072 1c00 0000 2905 7215 0000  r_...r....).r...
-00003350: 0072 6800 0000 724f 0000 00da 0669 6e64  .rh...rO.....ind
-00003360: 656e 7472 3e00 0000 7216 0000 0072 1600  entr>...r....r..
-00003370: 0000 7217 0000 00da 1766 6f72 6d61 745f  ..r......format_
-00003380: 626f 756e 6461 7279 5f73 6563 7469 6f6e  boundary_section
-00003390: 7801 0000 730e 0000 0006 060e 0104 0218  x...s...........
-000033a0: 0110 010a 010a 017a 2542 6c6f 636b 4d65  .......z%BlockMe
-000033b0: 7368 4469 6374 2e66 6f72 6d61 745f 626f  shDict.format_bo
-000033c0: 756e 6461 7279 5f73 6563 7469 6f6e 6301  undary_sectionc.
-000033d0: 0000 0000 0000 0000 0000 0001 0000 0001  ................
-000033e0: 0000 0043 0000 0073 0400 0000 6401 5300  ...C...s....d.S.
-000033f0: 2902 4eda 0072 1600 0000 7227 0000 0072  ).N..r....r'...r
-00003400: 1600 0000 7216 0000 0072 1700 0000 da1e  ....r....r......
-00003410: 666f 726d 6174 5f6d 6572 6765 7061 7463  format_mergepatc
-00003420: 6870 6169 7273 5f73 6563 7469 6f6e 8701  hpairs_section..
-00003430: 0000 7302 0000 0004 027a 2c42 6c6f 636b  ..s......z,Block
-00003440: 4d65 7368 4469 6374 2e66 6f72 6d61 745f  MeshDict.format_
-00003450: 6d65 7267 6570 6174 6368 7061 6972 735f  mergepatchpairs_
-00003460: 7365 6374 696f 6e63 0300 0000 0000 0000  sectionc........
-00003470: 0000 0000 0400 0000 0900 0000 4300 0000  ............C...
-00003480: 7346 0000 007c 006a 007c 0264 018d 0101  sF...|.j.|.d....
-00003490: 0074 0164 0283 017d 037c 036a 027c 0174  .t.d...}.|.j.|.t
-000034a0: 037c 006a 0483 017c 00a0 05a1 007c 00a0  .|.j...|.....|..
-000034b0: 06a1 007c 00a0 07a1 007c 00a0 08a1 007c  ...|.....|.....|
-000034c0: 00a0 09a1 0064 038d 0753 0029 044e 2901  .....d...S.).N).
-000034d0: 72a2 0000 0061 6d01 0000 2468 6561 6465  r....am...$heade
-000034e0: 720a 466f 616d 4669 6c65 0a7b 0a20 2020  r.FoamFile.{.   
-000034f0: 2076 6572 7369 6f6e 2020 2020 2032 2e30   version     2.0
-00003500: 3b0a 2020 2020 666f 726d 6174 2020 2020  ;.    format    
-00003510: 2020 6173 6369 693b 0a20 2020 2063 6c61    ascii;.    cla
-00003520: 7373 2020 2020 2020 2064 6963 7469 6f6e  ss       diction
-00003530: 6172 793b 0a20 2020 206f 626a 6563 7420  ary;.    object 
-00003540: 2020 2020 2062 6c6f 636b 4d65 7368 4469       blockMeshDi
-00003550: 6374 3b0a 7d0a 2f2f 202a 202a 202a 202a  ct;.}.// * * * *
-00003560: 202a 202a 202a 202a 202a 202a 202a 202a   * * * * * * * *
-00003570: 202a 202a 202a 202a 202a 202a 202a 202a   * * * * * * * *
-00003580: 202a 202a 202a 202a 202a 202a 202a 202a   * * * * * * * *
-00003590: 202a 202a 202a 202a 202a 202a 202a 202a   * * * * * * * *
-000035a0: 202a 202f 2f0a 0a73 6361 6c65 2020 2024   * //..scale   $
-000035b0: 6d65 7472 6963 636f 6e76 6572 743b 0a0a  metricconvert;..
-000035c0: 2476 6572 7469 6365 730a 0a24 626c 6f63  $vertices..$bloc
-000035d0: 6b73 0a0a 2465 6467 6573 0a0a 2462 6f75  ks..$edges..$bou
-000035e0: 6e64 6172 790a 246d 6572 6765 7061 7463  ndary.$mergepatc
-000035f0: 6870 6169 7273 0a2f 2f20 2a2a 2a2a 2a2a  hpairs.// ******
-00003600: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
-00003610: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
-00003620: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
-00003630: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
-00003640: 2a2a 2a20 2f2f 0a29 07da 0668 6561 6465  *** //.)...heade
-00003650: 725a 0d6d 6574 7269 6363 6f6e 7665 7274  rZ.metricconvert
-00003660: 723a 0000 0072 6d00 0000 726c 0000 00da  r:...rm...rl....
-00003670: 0862 6f75 6e64 6172 795a 0f6d 6572 6765  .boundaryZ.merge
-00003680: 7061 7463 6870 6169 7273 290a 72a4 0000  patchpairs).r...
-00003690: 0072 0300 0000 da0a 7375 6273 7469 7475  .r......substitu
-000036a0: 7465 7235 0000 0072 6b00 0000 72a7 0000  ter5...rk...r...
-000036b0: 0072 aa00 0000 72a9 0000 0072 ad00 0000  .r....r....r....
-000036c0: 72af 0000 0029 0472 1500 0000 72b0 0000  r....).r....r...
-000036d0: 005a 0d73 6f72 745f 766f 7274 6963 6573  .Z.sort_vortices
-000036e0: da08 7465 6d70 6c61 7465 7216 0000 0072  ..templater....r
-000036f0: 1600 0000 7217 0000 0072 1f00 0000 9001  ....r....r......
-00003700: 0000 731a 0000 000c 0102 0102 0104 ff04  ..s.............
-00003710: 1902 0108 0106 0106 0106 0106 0106 0106  ................
-00003720: f97a 1442 6c6f 636b 4d65 7368 4469 6374  .z.BlockMeshDict
-00003730: 2e66 6f72 6d61 7429 034e 4e4e 7269 0000  .format).NNNri..
-00003740: 0029 0154 2918 7229 0000 0072 2a00 0000  .).T).r)...r*...
-00003750: 722b 0000 0072 1800 0000 7278 0000 0072  r+...r....rx...r
-00003760: 7a00 0000 727e 0000 0072 7f00 0000 7284  z...r~...r....r.
-00003770: 0000 0072 9200 0000 720b 0000 0072 9300  ...r....r....r..
-00003780: 0000 7295 0000 0072 9800 0000 7299 0000  ..r....r....r...
-00003790: 0072 9d00 0000 72a4 0000 0072 a700 0000  .r....r....r....
-000037a0: 72a9 0000 0072 aa00 0000 72ad 0000 0072  r....r....r....r
-000037b0: af00 0000 7205 0000 0072 1f00 0000 7216  ....r....r....r.
-000037c0: 0000 0072 1600 0000 7216 0000 0072 1700  ...r....r....r..
-000037d0: 0000 726a 0000 00d0 0000 0073 2a00 0000  ..rj.......s*...
-000037e0: 0800 0801 0808 080e 0a03 0813 0804 080e  ................
-000037f0: 0c11 0aff 0809 0805 0a05 0805 0a05 0819  ................
-00003800: 080c 080b 080c 080f 1209 726a 0000 0063  ..........rj...c
-00003810: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003820: 0300 0000 0000 0000 731c 0000 0065 005a  ........s....e.Z
-00003830: 0164 005a 0287 0066 0164 0164 0284 085a  .d.Z...f.d.d...Z
-00003840: 0387 0004 005a 0453 0029 03da 1842 6c6f  .....Z.S.)...Blo
-00003850: 636b 4d65 7368 4469 6374 5265 6374 696c  ckMeshDictRectil
-00003860: 696e 6561 7263 0800 0000 0000 0000 0000  inearc..........
-00003870: 0000 0b00 0000 0800 0000 0300 0000 73b0  ..............s.
-00003880: 0000 0074 0083 00a0 01a1 0001 007c 00a0  ...t.........|..
-00003890: 027c 07a1 0101 0074 0364 0164 0164 0164  .|.....t.d.d.d.d
-000038a0: 0283 0474 037c 0164 0164 0164 0383 0474  ...t.|.d.d.d...t
-000038b0: 037c 017c 0264 0164 0483 0474 0364 017c  .|.|.d.d...t.d.|
-000038c0: 0264 0164 0583 0467 047d 087c 0844 005d  .d.d...g.}.|.D.]
-000038d0: 1c7d 097c 00a0 047c 096a 057c 096a 0664  .}.|...|.j.|.j.d
-000038e0: 017c 096a 0764 0617 00a1 0401 007c 00a0  .|.j.d.......|..
-000038f0: 047c 096a 057c 096a 067c 037c 096a 0764  .|.j.|.j.|.|.j.d
-00003900: 0717 00a1 0401 0071 2664 0864 0984 0064  .......q&d.d...d
-00003910: 0a44 0083 017d 0a7c 006a 087c 0a7c 047c  .D...}.|.j.|.|.|
-00003920: 057c 0666 0364 0b64 0c8d 037c 005f 0964  .|.f.d.d...|._.d
-00003930: 0053 0029 0d4e 7201 0000 005a 0276 30da  .S.).Nr....Z.v0.
-00003940: 0276 31da 0276 32da 0276 33fa 042d 626f  .v1..v2..v3..-bo
-00003950: 74fa 042d 746f 7063 0100 0000 0000 0000  t..-topc........
-00003960: 0000 0000 0300 0000 0600 0000 5300 0000  ............S...
-00003970: 7328 0000 0067 007c 005d 107d 0174 0064  s(...g.|.].}.t.d
-00003980: 0083 0144 005d 097d 0264 017c 029b 007c  ...D.].}.d.|...|
-00003990: 019b 009d 0391 0371 0871 0253 0029 0272  .......q.q.S.).r
-000039a0: 5000 0000 7283 0000 0029 01da 0572 616e  P...r....)...ran
-000039b0: 6765 2903 7237 0000 00da 0470 6f73 7472  ge).r7.....postr
-000039c0: 1400 0000 7216 0000 0072 1600 0000 7217  ....r....r....r.
-000039d0: 0000 0072 5a00 0000 c701 0000 730a 0000  ...rZ.......s...
-000039e0: 0006 0008 0104 ff0e 0108 ff7a 3542 6c6f  ...........z5Blo
-000039f0: 636b 4d65 7368 4469 6374 5265 6374 696c  ckMeshDictRectil
-00003a00: 696e 6561 722e 5f5f 696e 6974 5f5f 2e3c  inear.__init__.<
-00003a10: 6c6f 6361 6c73 3e2e 3c6c 6973 7463 6f6d  locals>.<listcom
-00003a20: 703e 2902 72b8 0000 0072 b900 0000 72ae  p>).r....r....r.
-00003a30: 0000 0029 0172 1200 0000 290a da05 7375  ...).r....)...su
-00003a40: 7065 7272 1800 0000 727a 0000 0072 0d00  perr....rz...r..
-00003a50: 0000 727e 0000 0072 0f00 0000 7210 0000  ..r~...r....r...
-00003a60: 0072 1200 0000 7293 0000 00da 0562 6c6f  .r....r......blo
-00003a70: 636b 290b 7215 0000 00da 026c 78da 026c  ck).r......lx..l
-00003a80: 795a 026c 7ada 026e 78da 026e 795a 026e  yZ.lz..nx..nyZ.n
-00003a90: 7a72 7900 0000 5a06 6261 7365 7673 7283  zry...Z.basevsr.
-00003aa0: 0000 005a 0c76 6572 7465 785f 6e61 6d65  ...Z.vertex_name
-00003ab0: 73a9 01da 095f 5f63 6c61 7373 5f5f 7216  s....__class__r.
-00003ac0: 0000 0072 1700 0000 7218 0000 00b7 0100  ...r....r.......
-00003ad0: 0073 1c00 0000 0a01 0a02 0c03 0c01 0c01  .s..............
-00003ae0: 0c01 04fc 0807 1a01 1c01 0602 0201 06ff  ................
-00003af0: 1c04 7a21 426c 6f63 6b4d 6573 6844 6963  ..z!BlockMeshDic
-00003b00: 7452 6563 7469 6c69 6e65 6172 2e5f 5f69  tRectilinear.__i
-00003b10: 6e69 745f 5f29 0572 2900 0000 722a 0000  nit__).r)...r*..
-00003b20: 0072 2b00 0000 7218 0000 00da 0d5f 5f63  .r+...r......__c
-00003b30: 6c61 7373 6365 6c6c 5f5f 7216 0000 0072  lasscell__r....r
-00003b40: 1600 0000 72c2 0000 0072 1700 0000 72b4  ....r....r....r.
-00003b50: 0000 00b6 0100 0073 0400 0000 0800 1401  .......s........
-00003b60: 72b4 0000 004e 2917 da07 5f5f 646f 635f  r....N)...__doc_
-00003b70: 5fda 0969 7465 7274 6f6f 6c73 7202 0000  _..itertoolsr...
-00003b80: 00da 0673 7472 696e 6772 0300 0000 72ae  ...stringr....r.
-00003b90: 0000 0072 0500 0000 726d 0000 0072 0700  ...r....rm...r..
-00003ba0: 0000 7208 0000 0072 4400 0000 7209 0000  ..r....rD...r...
-00003bb0: 0072 0a00 0000 720b 0000 0072 0c00 0000  .r....r....r....
-00003bc0: da07 5f5f 616c 6c5f 5f72 0d00 0000 722d  ..__all__r....r-
-00003bd0: 0000 0072 3000 0000 7242 0000 0072 6200  ...r0...rB...rb.
-00003be0: 0000 726a 0000 0072 b400 0000 7216 0000  ..rj...r....r...
-00003bf0: 0072 1600 0000 7216 0000 0072 1700 0000  .r....r....r....
-00003c00: da08 3c6d 6f64 756c 653e 0100 0000 731e  ..<module>....s.
-00003c10: 0000 0004 000c 0c0c 010c 0210 0118 0108  ................
-00003c20: 020e 0a0e 1c0e 0a0e 110e 530e 2800 7f14  ..........S.(...
-00003c30: 67                                       g
+00000310: 0764 0c64 0d84 005a 0864 0e64 0f84 005a  .d.d...Z.d.d...Z
+00000320: 0964 0153 0029 11da 0656 6572 7465 784e  .d.S.)...VertexN
+00000330: 6306 0000 0000 0000 0000 0000 0006 0000  c...............
+00000340: 0002 0000 0043 0000 0073 2a00 0000 7c01  .....C...s*...|.
+00000350: 7c00 5f00 7c02 7c00 5f01 7c03 7c00 5f02  |._.|.|._.|.|._.
+00000360: 7c04 7c00 5f03 7c04 6801 7c00 5f04 7c05  |.|._.|.h.|._.|.
+00000370: 7c00 5f05 6400 5300 a901 4e29 06da 0178  |._.d.S...N)...x
+00000380: da01 79da 017a da04 6e61 6d65 da05 616c  ..y..z..name..al
+00000390: 6961 73da 0569 6e64 6578 2906 da04 7365  ias..index)...se
+000003a0: 6c66 720f 0000 0072 1000 0000 7211 0000  lfr....r....r...
+000003b0: 0072 1200 0000 7214 0000 00a9 0072 1600  .r....r......r..
+000003c0: 0000 fa55 2f68 6f6d 652f 7069 6572 7265  ...U/home/pierre
+000003d0: 2f44 6576 2f66 6c75 6964 7369 6d66 6f61  /Dev/fluidsimfoa
+000003e0: 6d2f 7372 632f 666c 7569 6473 696d 666f  m/src/fluidsimfo
+000003f0: 616d 2f66 6f61 6d5f 696e 7075 745f 6669  am/foam_input_fi
+00000400: 6c65 732f 626c 6f63 6b6d 6573 682f 5f5f  les/blockmesh/__
+00000410: 696e 6974 5f5f 2e70 79da 085f 5f69 6e69  init__.py..__ini
+00000420: 745f 5f1f 0000 0073 0c00 0000 0601 0601  t__....s........
+00000430: 0601 0601 0801 0a04 7a0f 5665 7274 6578  ........z.Vertex
+00000440: 2e5f 5f69 6e69 745f 5f63 0100 0000 0000  .__init__c......
+00000450: 0000 0000 0000 0200 0000 0800 0000 4300  ..............C.
+00000460: 0000 7360 0000 007c 006a 009b 0064 017c  ..s`...|.j...d.|
+00000470: 006a 019b 009d 037d 0174 027c 006a 0383  .j.....}.t.|.j..
+00000480: 0164 026b 0472 1c7c 0164 0364 01a0 0474  .d.k.r.|.d.d...t
+00000490: 057c 006a 0383 01a1 0117 0037 007d 0164  .|.j.......7.}.d
+000004a0: 047c 006a 0664 059b 0464 017c 006a 0764  .|.j.d...d.|.j.d
+000004b0: 059b 0464 017c 006a 0864 059b 0464 067c  ...d.|.j.d...d.|
+000004c0: 019b 009d 0853 0029 074e da01 2072 0600  .....S.).N.. r..
+000004d0: 0000 7a03 203a 207a 0228 207a 0520 2e31  ..z. : z.( z. .1
+000004e0: 3567 7a07 2029 2020 2f2f 2029 0972 1400  5gz. )  // ).r..
+000004f0: 0000 7212 0000 00da 036c 656e 7213 0000  ..r......lenr...
+00000500: 00da 046a 6f69 6eda 0673 6f72 7465 6472  ...join..sortedr
+00000510: 0f00 0000 7210 0000 0072 1100 0000 2902  ....r....r....).
+00000520: 7215 0000 00da 0763 6f6d 6d65 6e74 7216  r......commentr.
+00000530: 0000 0072 1600 0000 7217 0000 00da 0666  ...r....r......f
+00000540: 6f72 6d61 742a 0000 0073 0800 0000 1201  ormat*...s......
+00000550: 0e01 1801 2801 7a0d 5665 7274 6578 2e66  ....(.z.Vertex.f
+00000560: 6f72 6d61 7463 0100 0000 0000 0000 0000  ormatc..........
+00000570: 0000 0100 0000 0900 0000 4300 0000 7326  ..........C...s&
+00000580: 0000 0064 017c 006a 009b 0064 027c 006a  ...d.|.j...d.|.j
+00000590: 019b 0064 027c 006a 029b 0064 027c 006a  ...d.|.j...d.|.j
+000005a0: 039b 0064 039d 0953 0029 044e 7a07 5665  ...d...S.).Nz.Ve
+000005b0: 7274 6578 287a 022c 20fa 0129 2904 720f  rtex(z., ..)).r.
+000005c0: 0000 0072 1000 0000 7211 0000 0072 1200  ...r....r....r..
+000005d0: 0000 a901 7215 0000 0072 1600 0000 7216  ....r....r....r.
+000005e0: 0000 0072 1700 0000 da08 5f5f 7265 7072  ...r......__repr
+000005f0: 5f5f 3000 0000 7302 0000 0026 017a 0f56  __0...s....&.z.V
+00000600: 6572 7465 782e 5f5f 7265 7072 5f5f 6301  ertex.__repr__c.
+00000610: 0000 0000 0000 0000 0000 0001 0000 0005  ................
+00000620: 0000 0043 0000 0073 1a00 0000 7400 7c00  ...C...s....t.|.
+00000630: 8301 7c00 6a01 7c00 6a02 7c00 6a03 7c00  ..|.j.|.j.|.j.|.
+00000640: 6a04 8304 5300 720e 0000 0029 05da 0474  j...S.r....)...t
+00000650: 7970 6572 0f00 0000 7210 0000 0072 1100  yper....r....r..
+00000660: 0000 7212 0000 0072 2000 0000 7216 0000  ..r....r ...r...
+00000670: 0072 1600 0000 7217 0000 00da 0463 6f70  .r....r......cop
+00000680: 7933 0000 0073 0200 0000 1a01 7a0b 5665  y3...s......z.Ve
+00000690: 7274 6578 2e63 6f70 7963 0200 0000 0000  rtex.copyc......
+000006a0: 0000 0000 0000 0200 0000 0400 0000 4300  ..............C.
+000006b0: 0000 7320 0000 007c 006a 007c 006a 017c  ..s ...|.j.|.j.|
+000006c0: 006a 0266 037c 016a 007c 016a 017c 016a  .j.f.|.j.|.j.|.j
+000006d0: 0266 036b 0053 0072 0e00 0000 a903 7211  .f.k.S.r......r.
+000006e0: 0000 0072 1000 0000 720f 0000 00a9 0272  ...r....r......r
+000006f0: 1500 0000 da03 7268 7372 1600 0000 7216  ......rhsr....r.
+00000700: 0000 0072 1700 0000 da06 5f5f 6c74 5f5f  ...r......__lt__
+00000710: 3600 0000 f302 0000 0020 017a 0d56 6572  6........ .z.Ver
+00000720: 7465 782e 5f5f 6c74 5f5f 6302 0000 0000  tex.__lt__c.....
+00000730: 0000 0000 0000 0002 0000 0004 0000 0043  ...............C
+00000740: 0000 0073 2000 0000 7c00 6a00 7c00 6a01  ...s ...|.j.|.j.
+00000750: 7c00 6a02 6603 7c01 6a00 7c01 6a01 7c01  |.j.f.|.j.|.j.|.
+00000760: 6a02 6603 6b02 5300 720e 0000 0072 2400  j.f.k.S.r....r$.
+00000770: 0000 7225 0000 0072 1600 0000 7216 0000  ..r%...r....r...
+00000780: 0072 1700 0000 da06 5f5f 6571 5f5f 3900  .r......__eq__9.
+00000790: 0000 7228 0000 007a 0d56 6572 7465 782e  ..r(...z.Vertex.
+000007a0: 5f5f 6571 5f5f 6301 0000 0000 0000 0000  __eq__c.........
+000007b0: 0000 0001 0000 0004 0000 0043 0000 0073  ...........C...s
+000007c0: 1400 0000 7400 7c00 6a01 7c00 6a02 7c00  ....t.|.j.|.j.|.
+000007d0: 6a03 6603 8301 5300 720e 0000 0029 04da  j.f...S.r....)..
+000007e0: 0468 6173 6872 1100 0000 7210 0000 0072  .hashr....r....r
+000007f0: 0f00 0000 7220 0000 0072 1600 0000 7216  ....r ...r....r.
+00000800: 0000 0072 1700 0000 da08 5f5f 6861 7368  ...r......__hash
+00000810: 5f5f 3c00 0000 7302 0000 0014 017a 0f56  __<...s......z.V
+00000820: 6572 7465 782e 5f5f 6861 7368 5f5f 720e  ertex.__hash__r.
+00000830: 0000 0029 0ada 085f 5f6e 616d 655f 5fda  ...)...__name__.
+00000840: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
+00000850: 7561 6c6e 616d 655f 5f72 1800 0000 721e  ualname__r....r.
+00000860: 0000 0072 2100 0000 7223 0000 0072 2700  ...r!...r#...r'.
+00000870: 0000 7229 0000 0072 2b00 0000 7216 0000  ..r)...r+...r...
+00000880: 0072 1600 0000 7216 0000 0072 1700 0000  .r....r....r....
+00000890: 720d 0000 001e 0000 0073 1000 0000 0800  r........s......
+000008a0: 0a01 080b 0806 0803 0803 0803 0c03 720d  ..............r.
+000008b0: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
+000008c0: 0000 0000 0200 0000 4000 0000 f31c 0000  ........@.......
+000008d0: 0065 005a 0164 005a 0264 0164 0284 005a  .e.Z.d.Z.d.d...Z
+000008e0: 0364 0364 0484 005a 0464 0553 0029 06da  .d.d...Z.d.S.)..
+000008f0: 0446 6163 6563 0300 0000 0000 0000 0000  .Facec..........
+00000900: 0000 0300 0000 0200 0000 4300 0000 7310  ..........C...s.
+00000910: 0000 007c 017c 005f 007c 027c 005f 0164  ...|.|._.|.|._.d
+00000920: 0153 0029 027a 380a 2020 2020 2020 2020  .S.).z8.        
+00000930: 766e 616d 6520 6973 206c 6973 7420 6f72  vname is list or
+00000940: 2074 7570 6c65 206f 6620 7665 7274 6578   tuple of vertex
+00000950: 206e 616d 6573 0a20 2020 2020 2020 204e   names.        N
+00000960: 2902 da06 766e 616d 6573 7212 0000 0029  )...vnamesr....)
+00000970: 0372 1500 0000 7231 0000 0072 1200 0000  .r....r1...r....
+00000980: 7216 0000 0072 1600 0000 7217 0000 0072  r....r....r....r
+00000990: 1800 0000 4100 0000 7304 0000 0006 040a  ....A...s.......
+000009a0: 017a 0d46 6163 652e 5f5f 696e 6974 5f5f  .z.Face.__init__
+000009b0: 6302 0000 0000 0000 0000 0000 0004 0000  c...............
+000009c0: 0007 0000 0003 0000 0073 4600 0000 6401  .........sF...d.
+000009d0: a000 8700 6601 6402 6403 8408 7c00 6a01  ....f.d.d...|.j.
+000009e0: 4400 8301 a101 7d02 6401 a000 7c00 6a01  D.....}.d...|.j.
+000009f0: a101 7d03 6404 7c02 6405 9b04 6406 7c00  ..}.d.|.d...d.|.
+00000a00: 6a02 6405 9b04 6407 7c03 6405 9b04 6408  j.d...d.|.d...d.
+00000a10: 9d07 5300 2909 fa4b 466f 726d 6174 2069  ..S.)..KFormat i
+00000a20: 6e73 7461 6e63 6520 746f 2064 756d 700a  nstance to dump.
+00000a30: 2020 2020 2020 2020 7665 7274 6963 6573          vertices
+00000a40: 2069 7320 6469 6374 206f 6620 6e61 6d65   is dict of name
+00000a50: 2074 6f20 5665 7274 6578 0a20 2020 2020   to Vertex.     
+00000a60: 2020 2072 1900 0000 6301 0000 0000 0000     r....c.......
+00000a70: 0000 0000 0002 0000 0004 0000 0033 0000  .............3..
+00000a80: 00f3 1e00 0000 8100 7c00 5d0a 7d01 7400  ........|.].}.t.
+00000a90: 8800 7c01 1900 6a01 8301 5600 0100 7102  ..|...j...V...q.
+00000aa0: 6400 5300 720e 0000 00a9 02da 0373 7472  d.S.r........str
+00000ab0: 7214 0000 00a9 02da 022e 30da 0276 6ea9  r.........0..vn.
+00000ac0: 01da 0876 6572 7469 6365 7372 1600 0000  ...verticesr....
+00000ad0: 7217 0000 00da 093c 6765 6e65 7870 723e  r......<genexpr>
+00000ae0: 4c00 0000 f304 0000 0002 801c 007a 1e46  L............z.F
+00000af0: 6163 652e 666f 726d 6174 2e3c 6c6f 6361  ace.format.<loca
+00000b00: 6c73 3e2e 3c67 656e 6578 7072 3efa 0128  ls>.<genexpr>..(
+00000b10: da01 737a 0629 2020 2f2f 20fa 0220 2872  ..sz.)  // .. (r
+00000b20: 1f00 0000 2903 721b 0000 0072 3100 0000  ....).r....r1...
+00000b30: 7212 0000 00a9 0472 1500 0000 723a 0000  r......r....r:..
+00000b40: 0072 1400 0000 721d 0000 0072 1600 0000  .r....r....r....
+00000b50: 7239 0000 0072 1700 0000 721e 0000 0048  r9...r....r....H
+00000b60: 0000 0073 0600 0000 1a04 0c01 2001 7a0b  ...s........ .z.
+00000b70: 4661 6365 2e66 6f72 6d61 744e a905 722c  Face.formatN..r,
+00000b80: 0000 0072 2d00 0000 722e 0000 0072 1800  ...r-...r....r..
+00000b90: 0000 721e 0000 0072 1600 0000 7216 0000  ..r....r....r...
+00000ba0: 0072 1600 0000 7217 0000 0072 3000 0000  .r....r....r0...
+00000bb0: 4000 0000 7306 0000 0008 0008 010c 0772  @...s..........r
+00000bc0: 3000 0000 6300 0000 0000 0000 0000 0000  0...c...........
+00000bd0: 0000 0000 0002 0000 0040 0000 0072 2f00  .........@...r/.
+00000be0: 0000 2906 da0f 4d65 7267 6550 6174 6368  ..)...MergePatch
+00000bf0: 5061 6972 7363 0300 0000 0000 0000 0000  Pairsc..........
+00000c00: 0000 0300 0000 0200 0000 4300 0000 7310  ..........C...s.
+00000c10: 0000 007c 017c 005f 007c 027c 005f 0164  ...|.|._.|.|._.d
+00000c20: 0053 0072 0e00 0000 a902 da0e 626f 756e  .S.r........boun
+00000c30: 6461 7279 5f6e 616d 6531 da0e 626f 756e  dary_name1..boun
+00000c40: 6461 7279 5f6e 616d 6532 2903 7215 0000  dary_name2).r...
+00000c50: 0072 4400 0000 7245 0000 0072 1600 0000  .rD...rE...r....
+00000c60: 7216 0000 0072 1700 0000 7218 0000 0052  r....r....r....R
+00000c70: 0000 0073 0400 0000 0601 0a01 7a18 4d65  ...s........z.Me
+00000c80: 7267 6550 6174 6368 5061 6972 732e 5f5f  rgePatchPairs.__
+00000c90: 696e 6974 5f5f 6301 0000 0000 0000 0000  init__c.........
+00000ca0: 0000 0001 0000 0005 0000 0043 0000 0073  ...........C...s
+00000cb0: 1600 0000 6401 7c00 6a00 9b00 6402 7c00  ....d.|.j...d.|.
+00000cc0: 6a01 9b00 6403 9d05 5300 2904 4e72 3d00  j...d...S.).Nr=.
+00000cd0: 0000 7219 0000 0072 1f00 0000 7243 0000  ..r....r....rC..
+00000ce0: 0072 2000 0000 7216 0000 0072 1600 0000  .r ...r....r....
+00000cf0: 7217 0000 0072 1e00 0000 5600 0000 7302  r....r....V...s.
+00000d00: 0000 0016 017a 164d 6572 6765 5061 7463  .....z.MergePatc
+00000d10: 6850 6169 7273 2e66 6f72 6d61 744e 7241  hPairs.formatNrA
+00000d20: 0000 0072 1600 0000 7216 0000 0072 1600  ...r....r....r..
+00000d30: 0000 7217 0000 0072 4200 0000 5100 0000  ..r....rB...Q...
+00000d40: 7306 0000 0008 0008 010c 0472 4200 0000  s..........rB...
+00000d50: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+00000d60: 0004 0000 0040 0000 0073 3a00 0000 6500  .....@...s:...e.
+00000d70: 5a01 6400 5a02 6503 6401 6401 6401 8303  Z.d.Z.e.d.d.d...
+00000d80: 6601 6402 6403 8401 5a04 6404 6405 8400  f.d.d...Z.d.d...
+00000d90: 5a05 640b 6407 6408 8401 5a06 6409 640a  Z.d.d.d...Z.d.d.
+00000da0: 8400 5a07 6406 5300 290c da08 4865 7842  ..Z.d.S.)...HexB
+00000db0: 6c6f 636b 7206 0000 0063 0500 0000 0000  lockr....c......
+00000dc0: 0000 0000 0000 0500 0000 0200 0000 4300  ..............C.
+00000dd0: 0000 731c 0000 007c 017c 005f 007c 027c  ..s....|.|._.|.|
+00000de0: 005f 017c 037c 005f 027c 047c 005f 0364  ._.|.|._.|.|._.d
+00000df0: 0153 0029 0261 2e01 0000 496e 6974 6961  .S.).a....Initia
+00000e00: 6c69 7a65 2048 6578 426c 6f63 6b20 696e  lize HexBlock in
+00000e10: 7374 616e 6365 0a20 2020 2020 2020 2076  stance.        v
+00000e20: 6e61 6d65 7320 6973 2074 6865 2076 6572  names is the ver
+00000e30: 7465 7820 6e61 6d65 7320 696e 206f 7264  tex names in ord
+00000e40: 6572 2064 6573 6372 6976 6564 2069 6e0a  er descrived in.
+00000e50: 2020 2020 2020 2020 2020 2020 6874 7470              http
+00000e60: 3a2f 2f77 7777 2e6f 7065 6e66 6f61 6d2e  ://www.openfoam.
+00000e70: 6f72 672f 646f 6373 2f75 7365 722f 6d65  org/docs/user/me
+00000e80: 7368 2d64 6573 6372 6970 7469 6f6e 2e70  sh-description.p
+00000e90: 6870 0a20 2020 2020 2020 2063 656c 6c73  hp.        cells
+00000ea0: 2069 7320 6e75 6d62 6572 206f 6620 6365   is number of ce
+00000eb0: 6c6c 7320 6465 7669 6564 2069 6e74 6f20  lls devied into 
+00000ec0: 696e 2065 6163 6820 6469 7265 6374 696f  in each directio
+00000ed0: 6e0a 2020 2020 2020 2020 6e61 6d65 2069  n.        name i
+00000ee0: 7320 7468 6520 756e 6971 206e 616d 6520  s the uniq name 
+00000ef0: 6f66 2074 6865 2062 6c6f 636b 0a20 2020  of the block.   
+00000f00: 2020 2020 2067 7261 6469 6e67 2069 7320       grading is 
+00000f10: 6772 6164 696e 6720 6d65 7468 6f64 2e0a  grading method..
+00000f20: 2020 2020 2020 2020 4e29 0472 3100 0000          N).r1...
+00000f30: da05 6365 6c6c 7372 1200 0000 da07 6772  ..cellsr......gr
+00000f40: 6164 696e 6729 0572 1500 0000 7231 0000  ading).r....r1..
+00000f50: 0072 4700 0000 7212 0000 0072 4800 0000  .rG...r....rH...
+00000f60: 7216 0000 0072 1600 0000 7217 0000 0072  r....r....r....r
+00000f70: 1800 0000 5b00 0000 7308 0000 0006 0806  ....[...s.......
+00000f80: 0106 010a 017a 1148 6578 426c 6f63 6b2e  .....z.HexBlock.
+00000f90: 5f5f 696e 6974 5f5f 6302 0000 0000 0000  __init__c.......
+00000fa0: 0000 0000 0004 0000 0011 0000 0003 0000  ................
+00000fb0: 0073 7c00 0000 6401 a000 8700 6601 6402  .s|...d.....f.d.
+00000fc0: 6403 8408 7c00 6a01 4400 8301 a101 7d02  d...|.j.D.....}.
+00000fd0: 6401 a000 7c00 6a01 a101 7d03 6404 7c00  d...|.j...}.d.|.
+00000fe0: 6a02 9b00 6405 7c03 9b00 6406 7c02 9b00  j...d.|...d.|...
+00000ff0: 6407 7c00 6a02 9b00 6405 7c00 6a03 6408  d.|.j...d.|.j.d.
+00001000: 1900 6409 9b04 6401 7c00 6a03 640a 1900  ..d...d.|.j.d...
+00001010: 6409 9b04 6401 7c00 6a03 640b 1900 6409  d...d.|.j.d...d.
+00001020: 9b04 6407 7c00 6a04 a005 a100 9b00 9d10  ..d.|.j.........
+00001030: 5300 290c 7232 0000 0072 1900 0000 6301  S.).r2...r....c.
+00001040: 0000 0000 0000 0000 0000 0002 0000 0004  ................
+00001050: 0000 0033 0000 0072 3300 0000 720e 0000  ...3...r3...r...
+00001060: 0072 3400 0000 7236 0000 0072 3900 0000  .r4...r6...r9...
+00001070: 7216 0000 0072 1700 0000 723b 0000 006c  r....r....r;...l
+00001080: 0000 0072 3c00 0000 7a22 4865 7842 6c6f  ...r<...z"HexBlo
+00001090: 636b 2e66 6f72 6d61 742e 3c6c 6f63 616c  ck.format.<local
+000010a0: 733e 2e3c 6765 6e65 7870 723e 7a03 2f2f  s>.<genexpr>z.//
+000010b0: 2072 3f00 0000 7a0b 290a 2020 2020 6865   r?...z.).    he
+000010c0: 7820 287a 0229 2072 0100 0000 da01 6472  x (z.) r......dr
+000010d0: 0600 0000 7204 0000 0029 0672 1b00 0000  ....r....).r....
+000010e0: 7231 0000 0072 1200 0000 7247 0000 0072  r1...r....rG...r
+000010f0: 4800 0000 721e 0000 0072 4000 0000 7216  H...r....r@...r.
+00001100: 0000 0072 3900 0000 7217 0000 0072 1e00  ...r9...r....r..
+00001110: 0000 6800 0000 7320 0000 001a 040c 0110  ..h...s ........
+00001120: 0202 0104 ff04 0104 ff0a 0204 fe0a 0204  ................
+00001130: fe0a 0204 fe08 0304 fd02 ff7a 0f48 6578  ...........z.Hex
+00001140: 426c 6f63 6b2e 666f 726d 6174 4e63 0300  Block.formatNc..
+00001150: 0000 0000 0000 0000 0000 0800 0000 0500  ................
+00001160: 0000 0300 0000 73f0 0000 0069 0064 0164  ......s....i.d.d
+00001170: 0293 0164 0364 0293 0164 0464 0293 0164  ...d.d...d.d...d
+00001180: 0564 0693 0164 0764 0693 0164 0864 0693  .d...d.d...d.d..
+00001190: 0164 0964 0a93 0164 0b64 0a93 0164 0c64  .d.d...d.d...d.d
+000011a0: 0a93 0164 0d64 0e93 0164 0f64 0e93 0164  ...d.d...d.d...d
+000011b0: 1064 0e93 0164 1164 1293 0164 1364 1293  .d...d.d...d.d..
+000011c0: 0164 1464 1293 0164 1564 1293 0164 1664  .d.d...d.d...d.d
+000011d0: 1793 0164 1764 1764 1764 189c 03a5 017d  ...d.d.d.d.....}
+000011e0: 0367 0064 19a2 017d 0464 1a7d 0574 007c  .g.d...}.d.}.t.|
+000011f0: 0174 0183 0272 4a7c 037c 0119 007d 0174  .t...rJ|.|...}.t
+00001200: 0287 0066 0164 1b64 1c84 087c 047c 0119  ...f.d.d...|.|..
+00001210: 0044 0083 0183 017d 067c 0264 1d75 0072  .D.....}.|.d.u.r
+00001220: 7364 1e67 017d 0788 006a 0372 677c 07a0  sd.g.}...j.rg|..
+00001230: 0488 006a 03a1 0101 007c 07a0 047c 057c  ...j.....|...|.|
+00001240: 0119 00a1 0101 0064 1fa0 057c 07a1 017d  .......d...|...}
+00001250: 0274 067c 067c 0283 0253 0029 2061 0c02  .t.|.|...S.) a..
+00001260: 0000 4765 6e65 7261 7465 2046 6163 6520  ..Generate Face 
+00001270: 6f62 6a65 6374 0a20 2020 2020 2020 2069  object.        i
+00001280: 6e64 6578 2069 7320 6e75 6d62 6572 206f  ndex is number o
+00001290: 7220 6b65 7977 6f72 6420 746f 2069 6465  r keyword to ide
+000012a0: 6e74 6966 7920 7468 6520 6661 6365 206f  ntify the face o
+000012b0: 6620 4865 780a 2020 2020 2020 2020 2020  f Hex.          
+000012c0: 2020 3020 3d20 2777 2720 3d20 2778 6d27    0 = 'w' = 'xm'
+000012d0: 203d 2027 2d31 3030 2720 3d20 2830 2034   = '-100' = (0 4
+000012e0: 2037 2033 290a 2020 2020 2020 2020 2020   7 3).          
+000012f0: 2020 3120 3d20 2765 2720 3d20 2778 7027    1 = 'e' = 'xp'
+00001300: 203d 2027 3130 3027 203d 2028 3120 3220   = '100' = (1 2 
+00001310: 3620 3529 0a20 2020 2020 2020 2020 2020  6 5).           
+00001320: 2032 203d 2027 7327 203d 2027 796d 2720   2 = 's' = 'ym' 
+00001330: 3d20 2730 2d31 3027 203d 2028 3020 3120  = '0-10' = (0 1 
+00001340: 3520 3429 0a20 2020 2020 2020 2020 2020  5 4).           
+00001350: 2033 203d 2027 6e27 203d 2027 7970 2720   3 = 'n' = 'yp' 
+00001360: 3d20 2730 3130 2720 3d20 2832 2033 2037  = '010' = (2 3 7
+00001370: 2036 290a 2020 2020 2020 2020 2020 2020   6).            
+00001380: 3420 3d20 2762 2720 3d20 277a 6d27 203d  4 = 'b' = 'zm' =
+00001390: 2027 3030 2d31 2720 3d20 2830 2033 2032   '00-1' = (0 3 2
+000013a0: 2031 2920 3d20 2262 6f74 746f 6d22 0a20   1) = "bottom". 
+000013b0: 2020 2020 2020 2020 2020 2035 203d 2027             5 = '
+000013c0: 7427 203d 2027 7a70 2720 3d20 2730 3031  t' = 'zp' = '001
+000013d0: 2720 3d20 2834 2035 2036 2037 2920 3d20  ' = (4 5 6 7) = 
+000013e0: 2274 6f70 220a 2020 2020 2020 2020 6e61  "top".        na
+000013f0: 6d65 2069 7320 6769 7665 6e20 746f 2046  me is given to F
+00001400: 6163 6520 696e 7374 616e 6365 2e20 4966  ace instance. If
+00001410: 206f 6d69 7474 6564 2c20 6e61 6d65 2069   omitted, name i
+00001420: 7320 6175 746f 6d61 7469 6361 6c6c 790a  s automatically.
+00001430: 2020 2020 2020 2020 2020 2020 6765 6e61              gena
+00001440: 7261 7469 6564 206c 696b 6520 2827 662d  ratied like ('f-
+00001450: 2720 2b20 7365 6c66 2e6e 616d 6520 2b20  ' + self.name + 
+00001460: 272d 7727 290a 2020 2020 2020 2020 da01  '-w').        ..
+00001470: 7772 0100 0000 da02 786d 7a04 2d31 3030  wr......xmz.-100
+00001480: da01 6572 0600 0000 da02 7870 da03 3130  ..er......xp..10
+00001490: 3072 3e00 0000 7204 0000 00da 0279 6d7a  0r>...r......ymz
+000014a0: 0430 2d31 30da 016e e903 0000 005a 0279  .0-10..n.....Z.y
+000014b0: 705a 0330 3130 da01 62e9 0400 0000 da06  pZ.010..b.......
+000014c0: 626f 7474 6f6d 5a02 7a6d 7a04 3030 2d31  bottomZ.zmz.00-1
+000014d0: da01 74e9 0500 0000 2903 da03 746f 705a  ..t.....)...topZ
+000014e0: 027a 705a 0330 3031 2906 2904 7201 0000  .zpZ.001).).r...
+000014f0: 0072 5300 0000 e907 0000 0072 5100 0000  .rS........rQ...
+00001500: 2904 7206 0000 0072 0400 0000 e906 0000  ).r....r........
+00001510: 0072 5600 0000 2904 7201 0000 0072 0600  .rV...).r....r..
+00001520: 0000 7256 0000 0072 5300 0000 2904 7204  ..rV...rS...).r.
+00001530: 0000 0072 5100 0000 7258 0000 0072 5900  ...rQ...rX...rY.
+00001540: 0000 2904 7201 0000 0072 5100 0000 7204  ..).r....rQ...r.
+00001550: 0000 0072 0600 0000 2904 7253 0000 0072  ...r....).rS...r
+00001560: 5600 0000 7259 0000 0072 5800 0000 5a06  V...rY...rX...Z.
+00001570: 7765 736e 6274 6301 0000 0000 0000 0000  wesnbtc.........
+00001580: 0000 0002 0000 0004 0000 0013 0000 0073  ...............s
+00001590: 1600 0000 6700 7c00 5d07 7d01 8800 6a00  ....g.|.].}...j.
+000015a0: 7c01 1900 9102 7102 5300 7216 0000 0029  |.....q.S.r....)
+000015b0: 0172 3100 0000 2902 7237 0000 00da 0169  .r1...).r7.....i
+000015c0: 7220 0000 0072 1600 0000 7217 0000 00da  r ...r....r.....
+000015d0: 0a3c 6c69 7374 636f 6d70 3ea4 0000 00f3  .<listcomp>.....
+000015e0: 0200 0000 1600 7a21 4865 7842 6c6f 636b  ......z!HexBlock
+000015f0: 2e66 6163 652e 3c6c 6f63 616c 733e 2e3c  .face.<locals>.<
+00001600: 6c69 7374 636f 6d70 3e4e da01 66fa 012d  listcomp>N..f..-
+00001610: 2907 da0a 6973 696e 7374 616e 6365 7235  )...isinstancer5
+00001620: 0000 00da 0574 7570 6c65 7212 0000 00da  .....tupler.....
+00001630: 0661 7070 656e 6472 1b00 0000 7230 0000  .appendr....r0..
+00001640: 0029 0872 1500 0000 7214 0000 0072 1200  .).r....r....r..
+00001650: 0000 5a0b 6b77 5f74 6f5f 696e 6465 785a  ..Z.kw_to_indexZ
+00001660: 0f69 6e64 6578 5f74 6f5f 7665 7274 6578  .index_to_vertex
+00001670: 5a16 696e 6465 785f 746f 5f64 6566 6175  Z.index_to_defau
+00001680: 6c74 7375 6666 6978 7231 0000 00da 0570  ltsuffixr1.....p
+00001690: 6172 7473 7216 0000 0072 2000 0000 7217  artsr....r ...r.
+000016a0: 0000 00da 0466 6163 6575 0000 0073 6600  .....faceu...sf.
+000016b0: 0000 020c 0401 02ff 0402 02fe 0403 02fd  ................
+000016c0: 0404 02fc 0405 02fb 0406 02fa 0407 02f9  ................
+000016d0: 0408 02f8 0409 02f7 040a 02f6 040b 02f5  ................
+000016e0: 040c 02f4 040d 02f3 040e 02f2 040f 02f1  ................
+000016f0: 0410 02f0 0411 02ef 0212 0201 0201 08ec  ................
+00001700: 0816 0408 0a02 0801 1a02 0801 0601 0601  ................
+00001710: 0c01 0e01 0a01 0a01 7a0d 4865 7842 6c6f  ........z.HexBlo
+00001720: 636b 2e66 6163 6563 0100 0000 0000 0000  ck.facec........
+00001730: 0000 0000 0200 0000 0300 0000 0700 0000  ................
+00001740: 7312 0000 0087 0066 0164 0164 0284 087c  s......f.d.d...|
+00001750: 0144 0083 0153 0029 034e 6301 0000 0000  .D...S.).Nc.....
+00001760: 0000 0000 0000 0002 0000 0005 0000 0013  ................
+00001770: 0000 0073 1600 0000 6700 7c00 5d07 7d01  ...s....g.|.].}.
+00001780: 8800 a000 7c01 a101 9102 7102 5300 7216  ....|.....q.S.r.
+00001790: 0000 0029 0172 6300 0000 a902 7237 0000  ...).rc.....r7..
+000017a0: 00da 0361 7267 7220 0000 0072 1600 0000  ...argr ...r....
+000017b0: 7217 0000 0072 5b00 0000 ae00 0000 725c  r....r[.......r\
+000017c0: 0000 007a 2248 6578 426c 6f63 6b2e 6661  ...z"HexBlock.fa
+000017d0: 6365 732e 3c6c 6f63 616c 733e 2e3c 6c69  ces.<locals>.<li
+000017e0: 7374 636f 6d70 3e72 1600 0000 2902 7215  stcomp>r....).r.
+000017f0: 0000 00da 0461 7267 7372 1600 0000 7220  .....argsr....r 
+00001800: 0000 0072 1700 0000 da05 6661 6365 73ad  ...r......faces.
+00001810: 0000 0073 0200 0000 1201 7a0e 4865 7842  ...s......z.HexB
+00001820: 6c6f 636b 2e66 6163 6573 720e 0000 0029  lock.facesr....)
+00001830: 0872 2c00 0000 722d 0000 0072 2e00 0000  .r,...r-...r....
+00001840: 720b 0000 0072 1800 0000 721e 0000 0072  r....r....r....r
+00001850: 6300 0000 7267 0000 0072 1600 0000 7216  c...rg...r....r.
+00001860: 0000 0072 1600 0000 7217 0000 0072 4600  ...r....r....rF.
+00001870: 0000 5a00 0000 730a 0000 0008 0014 0108  ..Z...s.........
+00001880: 0d0a 0d0c 3872 4600 0000 6300 0000 0000  ....8rF...c.....
+00001890: 0000 0000 0000 0000 0000 0003 0000 0040  ...............@
+000018a0: 0000 0073 2600 0000 6500 5a01 6400 5a02  ...s&...e.Z.d.Z.
+000018b0: 6408 6402 6403 8401 5a03 6404 6405 8400  d.d.d...Z.d.d...
+000018c0: 5a04 6406 6407 8400 5a05 6401 5300 2909  Z.d.d...Z.d.S.).
+000018d0: da08 426f 756e 6461 7279 4e63 0500 0000  ..BoundaryNc....
+000018e0: 0000 0000 0000 0000 0500 0000 0300 0000  ................
+000018f0: 4300 0000 733a 0000 007c 017c 005f 007c  C...s:...|.|._.|
+00001900: 027c 005f 017c 0364 0175 0072 0d67 007d  .|._.|.d.u.r.g.}
+00001910: 036e 0874 027c 0374 0383 0272 157c 0367  .n.t.|.t...r.|.g
+00001920: 017d 037c 037c 005f 047c 047c 005f 0564  .}.|.|._.|.|._.d
+00001930: 0153 0029 027a c469 6e69 7469 616c 697a  .S.).z.initializ
+00001940: 6520 626f 756e 6461 7279 0a20 2020 2020  e boundary.     
+00001950: 2020 2074 7970 655f 2069 7320 7479 7065     type_ is type
+00001960: 206b 6579 776f 7264 2028 7761 6c6c 2c20   keyword (wall, 
+00001970: 7061 7463 682c 2065 6d70 7479 2c20 2e2e  patch, empty, ..
+00001980: 290a 2020 2020 2020 2020 6e61 6d65 2069  ).        name i
+00001990: 7320 6e61 7665 206f 6620 626f 756e 6461  s nave of bounda
+000019a0: 7279 2065 6d65 6c6d 656e 740a 2020 2020  ry emelment.    
+000019b0: 2020 2020 6661 6365 7320 6973 2066 6163      faces is fac
+000019c0: 6573 2077 6869 6368 2061 7265 2061 7070  es which are app
+000019d0: 6c69 6564 2077 6974 6820 7468 6973 2062  lied with this b
+000019e0: 6f75 6e64 6172 7920 636f 6e64 6974 696f  oundary conditio
+000019f0: 6e73 0a20 2020 2020 2020 204e 2906 da05  ns.        N)...
+00001a00: 7479 7065 5f72 1200 0000 725f 0000 0072  type_r....r_...r
+00001a10: 3000 0000 7267 0000 00da 096e 6569 6768  0...rg.....neigh
+00001a20: 626f 7572 2905 7215 0000 0072 6900 0000  bour).r....ri...
+00001a30: 7212 0000 0072 6700 0000 726a 0000 0072  r....rg...rj...r
+00001a40: 1600 0000 7216 0000 0072 1700 0000 7218  ....r....r....r.
+00001a50: 0000 00b2 0000 0073 1000 0000 0606 0601  .......s........
+00001a60: 0801 0601 0a01 0601 0601 0a01 7a11 426f  ............z.Bo
+00001a70: 756e 6461 7279 2e5f 5f69 6e69 745f 5f63  undary.__init__c
+00001a80: 0200 0000 0000 0000 0000 0000 0200 0000  ................
+00001a90: 0300 0000 4300 0000 7310 0000 007c 006a  ....C...s....|.j
+00001aa0: 00a0 017c 01a1 0101 0064 0153 0029 027a  ...|.....d.S.).z
+00001ab0: 5161 6464 2066 6163 6520 696e 7374 616e  Qadd face instan
+00001ac0: 6365 0a20 2020 2020 2020 2066 6163 6520  ce.        face 
+00001ad0: 6973 2061 2046 6163 6520 696e 7374 616e  is a Face instan
+00001ae0: 6365 2028 6e6f 7420 6e61 6d65 2920 746f  ce (not name) to
+00001af0: 2062 6520 6164 6465 640a 2020 2020 2020   be added.      
+00001b00: 2020 4e29 0272 6700 0000 7261 0000 0029    N).rg...ra...)
+00001b10: 0272 1500 0000 7263 0000 0072 1600 0000  .r....rc...r....
+00001b20: 7216 0000 0072 1700 0000 da08 6164 645f  r....r......add_
+00001b30: 6661 6365 c100 0000 7302 0000 0010 047a  face....s......z
+00001b40: 1142 6f75 6e64 6172 792e 6164 645f 6661  .Boundary.add_fa
+00001b50: 6365 6302 0000 0000 0000 0000 0000 0004  cec.............
+00001b60: 0000 0008 0000 0043 0000 0073 8200 0000  .......C...s....
+00001b70: 7c00 6a00 6701 7d02 7c00 6a01 6401 7500  |.j.g.}.|.j.d.u.
+00001b80: 7216 7c02 a002 6402 6403 7c00 6a03 9b00  r.|...d.d.|.j...
+00001b90: 6404 9d03 1700 a101 0100 6e10 7c02 a002  d.........n.|...
+00001ba0: 6402 6403 7c00 6a03 9b00 6405 7c00 6a01  d.d.|.j...d.|.j.
+00001bb0: 9b00 6404 9d05 1700 a101 0100 7c00 6a04  ..d.........|.j.
+00001bc0: 4400 5d0d 7d03 7c02 a002 6406 7c03 a005  D.].}.|...d.|...
+00001bd0: 7c01 a101 9b00 9d02 a101 0100 7129 7c02  |...........q)|.
+00001be0: a002 6407 a101 0100 6408 a006 7c02 a101  ..d.....d...|...
+00001bf0: 5300 2909 7232 0000 004e 7a02 7b0a 7a09  S.).r2...Nz.{.z.
+00001c00: 2020 2020 7479 7065 207a 113b 0a20 2020      type z.;.   
+00001c10: 2066 6163 6573 0a20 2020 2028 7a16 3b0a   faces.    (z.;.
+00001c20: 2020 2020 6e65 6967 6862 6f75 7250 6174      neighbourPat
+00001c30: 6368 2020 7a08 2020 2020 2020 2020 7a08  ch  z.        z.
+00001c40: 2020 2020 293b 0a7d da01 0a29 0772 1200      );.}...).r..
+00001c50: 0000 726a 0000 0072 6100 0000 7269 0000  ..rj...ra...ri..
+00001c60: 0072 6700 0000 721e 0000 0072 1b00 0000  .rg...r....r....
+00001c70: 2904 7215 0000 0072 3a00 0000 da03 746d  ).r....r:.....tm
+00001c80: 7072 6300 0000 7216 0000 0072 1600 0000  prc...r....r....
+00001c90: 7217 0000 0072 1e00 0000 c700 0000 7318  r....r........s.
+00001ca0: 0000 0008 040a 011a 0104 020c 0104 0108  ................
+00001cb0: ff04 ff0a 0418 010a 010a 017a 0f42 6f75  ...........z.Bou
+00001cc0: 6e64 6172 792e 666f 726d 6174 a902 4e4e  ndary.format..NN
+00001cd0: 2906 722c 0000 0072 2d00 0000 722e 0000  ).r,...r-...r...
+00001ce0: 0072 1800 0000 726b 0000 0072 1e00 0000  .r....rk...r....
+00001cf0: 7216 0000 0072 1600 0000 7216 0000 0072  r....r....r....r
+00001d00: 1700 0000 7268 0000 00b1 0000 0073 0800  ....rh.......s..
+00001d10: 0000 0800 0a01 080f 0c06 7268 0000 0063  ..........rh...c
+00001d20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001d30: 0500 0000 4000 0000 73f4 0000 0065 005a  ....@...s....e.Z
+00001d40: 0164 005a 0264 0164 0284 005a 0364 0364  .d.Z.d.d...Z.d.d
+00001d50: 0484 005a 0464 0564 0684 005a 0564 3464  ...Z.d.d...Z.d4d
+00001d60: 0864 0984 015a 0664 0a64 0b84 005a 0764  .d...Z.d.d...Z.d
+00001d70: 0c64 0d84 005a 0864 0e64 0f84 005a 0964  .d...Z.d.d...Z.d
+00001d80: 3564 1164 1284 015a 0a64 0765 0b64 1364  5d.d...Z.d.e.d.d
+00001d90: 1364 1383 0366 0264 1464 1584 015a 0c64  .d...f.d.d...Z.d
+00001da0: 0765 0b64 1364 1364 1383 0364 1664 1066  .e.d.d.d...d.d.f
+00001db0: 0464 1764 1884 015a 0d64 1964 1a84 005a  .d.d...Z.d.d...Z
+00001dc0: 0e64 1b64 1c84 005a 0f64 3664 1d64 1e84  .d.d...Z.d6d.d..
+00001dd0: 015a 1064 1f65 1164 2065 1166 0464 2164  .Z.d.e.d e.f.d!d
+00001de0: 2284 045a 1264 2364 2484 005a 1364 3764  "..Z.d#d$..Z.d7d
+00001df0: 2664 2784 015a 1464 2864 2984 005a 1564  &d'..Z.d(d)..Z.d
+00001e00: 2a64 2b84 005a 1664 2c64 2d84 005a 1764  *d+..Z.d,d-..Z.d
+00001e10: 2e64 2f84 005a 1864 3064 3184 005a 1965  .d/..Z.d0d1..Z.e
+00001e20: 1a64 2566 0264 3264 3384 015a 1b64 0753  .d%f.d2d3..Z.d.S
+00001e30: 0029 38da 0d42 6c6f 636b 4d65 7368 4469  .)8..BlockMeshDi
+00001e40: 6374 6301 0000 0000 0000 0000 0000 0001  ctc.............
+00001e50: 0000 0002 0000 0043 0000 0073 2e00 0000  .......C...s....
+00001e60: 6401 7c00 5f00 6900 7c00 5f01 6900 7c00  d.|._.i.|._.i.|.
+00001e70: 5f02 6900 7c00 5f03 6900 7c00 5f04 6900  _.i.|._.i.|._.i.
+00001e80: 7c00 5f05 6400 7c00 5f06 6400 5300 2902  |._.d.|._.d.S.).
+00001e90: 4e67 0000 0000 0000 f03f 2907 da11 636f  Ng.......?)...co
+00001ea0: 6e76 6572 745f 746f 5f6d 6574 6572 7372  nvert_to_metersr
+00001eb0: 3a00 0000 da06 626c 6f63 6b73 da05 6564  :.....blocks..ed
+00001ec0: 6765 73da 0a62 6f75 6e64 6172 6965 73da  ges..boundaries.
+00001ed0: 116d 6572 6765 5f70 6174 6368 5f70 6169  .merge_patch_pai
+00001ee0: 7273 da16 5f76 6572 7469 6365 735f 696e  rs.._vertices_in
+00001ef0: 5f62 6c6f 636b 6d65 7368 7220 0000 0072  _blockmeshr ...r
+00001f00: 1600 0000 7216 0000 0072 1700 0000 7218  ....r....r....r.
+00001f10: 0000 00da 0000 0073 0e00 0000 0601 0601  .......s........
+00001f20: 0601 0601 0601 0601 0a01 7a16 426c 6f63  ..........z.Bloc
+00001f30: 6b4d 6573 6844 6963 742e 5f5f 696e 6974  kMeshDict.__init
+00001f40: 5f5f 6302 0000 0000 0000 0000 0000 0003  __c.............
+00001f50: 0000 0009 0000 0043 0000 0073 2400 0000  .......C...s$...
+00001f60: 6401 6402 6403 6404 6405 6406 6407 6407  d.d.d.d.d.d.d.d.
+00001f70: 6408 9c08 7d02 7c02 7c01 1900 7c00 5f00  d...}.|.|...|._.
+00001f80: 6409 5300 290a 7a22 7365 7420 7365 6c66  d.S.).z"set self
+00001f90: 2e63 6f6d 7665 7274 5f74 6f5f 6d65 7465  .comvert_to_mete
+00001fa0: 7273 2062 7920 776f 7264 69e8 0300 0072  rs by wordi....r
+00001fb0: 0600 0000 677b 14ae 47e1 7a84 3f67 fca9  ....g{..G.z.?g..
+00001fc0: f1d2 4d62 503f 678d edb5 a0f7 c6b0 3e67  ..MbP?g.......>g
+00001fd0: 95d6 26e8 0b2e 113e 67bb bdd7 d9df 7cdb  ..&....>g.....|.
+00001fe0: 3d29 085a 026b 6dda 016d da02 636d da02  =).Z.km..m..cm..
+00001ff0: 6d6d da02 756d da02 6e6d da01 415a 0841  mm..um..nm..AZ.A
+00002000: 6e67 7374 726f 6d4e a901 7270 0000 0029  ngstromN..rp...)
+00002010: 0372 1500 0000 5a06 6d65 7472 6963 5a17  .r....Z.metricZ.
+00002020: 6d65 7472 6963 7379 6d5f 746f 5f63 6f6e  metricsym_to_con
+00002030: 7665 7273 696f 6e72 1600 0000 7216 0000  versionr....r...
+00002040: 0072 1700 0000 da0a 7365 745f 6d65 7472  .r......set_metr
+00002050: 6963 e300 0000 7314 0000 0002 0302 0102  ic....s.........
+00002060: 0102 0102 0102 0102 0102 0106 f80e 0a7a  ...............z
+00002070: 1842 6c6f 636b 4d65 7368 4469 6374 2e73  .BlockMeshDict.s
+00002080: 6574 5f6d 6574 7269 6363 0200 0000 0000  et_metricc......
+00002090: 0000 0000 0000 0200 0000 0200 0000 4300  ..............C.
+000020a0: 0000 730a 0000 007c 017c 005f 0064 0053  ..s....|.|._.d.S
+000020b0: 0072 0e00 0000 727c 0000 0029 0272 1500  .r....r|...).r..
+000020c0: 0000 da05 7363 616c 6572 1600 0000 7216  ....scaler....r.
+000020d0: 0000 0072 1700 0000 da09 7365 745f 7363  ...r......set_sc
+000020e0: 616c 65f1 0000 0073 0200 0000 0a01 7a17  ale....s......z.
+000020f0: 426c 6f63 6b4d 6573 6844 6963 742e 7365  BlockMeshDict.se
+00002100: 745f 7363 616c 654e 6305 0000 0000 0000  t_scaleNc.......
+00002110: 0000 0000 0006 0000 0005 0000 0043 0000  .............C..
+00002120: 0073 5800 0000 7400 7c01 7401 8302 721b  .sX...t.|.t...r.
+00002130: 7402 6401 6402 8400 7c02 7c03 7c04 6603  t.d.d...|.|.|.f.
+00002140: 4400 8301 8301 7215 7403 6403 8301 8201  D.....r.t.d.....
+00002150: 7c01 7d05 7c05 6a04 7d04 6e07 7401 7c01  |.}.|.j.}.n.t.|.
+00002160: 7c02 7c03 7c04 8304 7d05 7c05 7c00 6a05  |.|.|...}.|.|.j.
+00002170: 7c04 3c00 7c00 6a05 7c04 1900 5300 2904  |.<.|.j.|...S.).
+00002180: 7ab2 6164 6420 7665 7274 6578 2062 7920  z.add vertex by 
+00002190: 636f 6f72 6469 6e61 7465 2061 6e64 2075  coordinate and u
+000021a0: 6e69 7120 6e61 6d65 0a20 2020 2020 2020  niq name.       
+000021b0: 2078 2079 207a 2069 7320 636f 6f72 6469   x y z is coordi
+000021c0: 6e61 7465 7320 6f66 2076 6572 7465 780a  nates of vertex.
+000021d0: 2020 2020 2020 2020 6e61 6d65 2069 7320          name is 
+000021e0: 756e 6971 206e 616d 6520 746f 2072 6566  uniq name to ref
+000021f0: 6572 2074 6865 2076 6572 7465 780a 2020  er the vertex.  
+00002200: 2020 2020 2020 7265 7475 726e 7320 5665        returns Ve
+00002210: 7274 6578 206f 626a 6563 7420 7768 6963  rtex object whic
+00002220: 6920 6973 2061 6464 6564 2e0a 2020 2020  i is added..    
+00002230: 2020 2020 6301 0000 0000 0000 0000 0000      c...........
+00002240: 0002 0000 0003 0000 0073 0000 0073 1800  .........s...s..
+00002250: 0000 8100 7c00 5d07 7d01 7c01 6400 7501  ....|.].}.|.d.u.
+00002260: 5600 0100 7102 6400 5300 720e 0000 0072  V...q.d.S.r....r
+00002270: 1600 0000 7264 0000 0072 1600 0000 7216  ....rd...r....r.
+00002280: 0000 0072 1700 0000 723b 0000 00fb 0000  ...r....r;......
+00002290: 0073 0400 0000 0280 1600 7a2b 426c 6f63  .s........z+Bloc
+000022a0: 6b4d 6573 6844 6963 742e 6164 645f 7665  kMeshDict.add_ve
+000022b0: 7274 6578 2e3c 6c6f 6361 6c73 3e2e 3c67  rtex.<locals>.<g
+000022c0: 656e 6578 7072 3e7a 4078 2069 7320 6120  enexpr>z@x is a 
+000022d0: 5665 7274 6578 2061 6e64 2060 616e 7928  Vertex and `any(
+000022e0: 6172 6720 6973 206e 6f74 204e 6f6e 6520  arg is not None 
+000022f0: 666f 7220 6172 6720 696e 2028 792c 207a  for arg in (y, z
+00002300: 2c20 6e61 6d65 2929 6029 0672 5f00 0000  , name))`).r_...
+00002310: 720d 0000 00da 0361 6e79 da0a 5661 6c75  r......any..Valu
+00002320: 6545 7272 6f72 7212 0000 0072 3a00 0000  eErrorr....r:...
+00002330: 2906 7215 0000 0072 0f00 0000 7210 0000  ).r....r....r...
+00002340: 0072 1100 0000 7212 0000 005a 0676 6572  .r....r....Z.ver
+00002350: 7465 7872 1600 0000 7216 0000 0072 1700  texr....r....r..
+00002360: 0000 da0a 6164 645f 7665 7274 6578 f400  ....add_vertex..
+00002370: 0000 7314 0000 000a 0618 0102 0102 0104  ..s.............
+00002380: ff04 0408 010e 020a 010a 017a 1842 6c6f  ...........z.Blo
+00002390: 636b 4d65 7368 4469 6374 2e61 6464 5f76  ckMeshDict.add_v
+000023a0: 6572 7465 7863 0200 0000 0000 0000 0000  ertexc..........
+000023b0: 0000 0200 0000 0200 0000 4300 0000 730c  ..........C...s.
+000023c0: 0000 007c 006a 007c 013d 0064 0153 0029  ...|.j.|.=.d.S.)
+000023d0: 027a 1f64 656c 206e 616d 6520 6b65 7920  .z.del name key 
+000023e0: 6672 6f6d 2073 656c 662e 7665 7274 6963  from self.vertic
+000023f0: 6573 4e72 3900 0000 2902 7215 0000 0072  esNr9...).r....r
+00002400: 1200 0000 7216 0000 0072 1600 0000 7217  ....r....r....r.
+00002410: 0000 00da 0a64 656c 5f76 6572 7465 7807  .....del_vertex.
+00002420: 0100 0073 0200 0000 0c02 7a18 426c 6f63  ...s......z.Bloc
+00002430: 6b4d 6573 6844 6963 742e 6465 6c5f 7665  kMeshDict.del_ve
+00002440: 7274 6578 6302 0000 0000 0000 0000 0000  rtexc...........
+00002450: 0006 0000 0004 0000 0047 0000 0073 3a00  .........G...s:.
+00002460: 0000 7c00 6a00 7c01 1900 7d03 7c02 4400  ..|.j.|...}.|.D.
+00002470: 5d13 7d04 7c00 6a00 7c04 1900 7d05 7c03  ].}.|.j.|...}.|.
+00002480: 6a01 a002 7c05 6a01 a101 0100 7c03 7c00  j...|.j.....|.|.
+00002490: 6a00 7c04 3c00 7107 6401 5300 2902 7ae2  j.|.<.q.d.S.).z.
+000024a0: 7472 6561 7420 6e61 6d65 312c 206e 616d  treat name1, nam
+000024b0: 6532 2c20 2e2e 2e20 6173 2073 616d 6520  e2, ... as same 
+000024c0: 706f 696e 742e 0a0a 2020 2020 2020 2020  point...        
+000024d0: 6e61 6d65 322e 616c 6961 732c 206e 616d  name2.alias, nam
+000024e0: 6533 2e61 6c69 6173 2c20 2e2e 2e20 6172  e3.alias, ... ar
+000024f0: 6520 6d65 7267 6564 2077 6974 6820 6e61  e merged with na
+00002500: 6d65 312e 616c 6961 730a 2020 2020 2020  me1.alias.      
+00002510: 2020 7468 6520 6b65 7920 6e61 6d65 322c    the key name2,
+00002520: 206e 616d 6533 2c20 2e2e 2e20 696e 2073   name3, ... in s
+00002530: 656c 662e 7665 7274 6963 6573 2061 7265  elf.vertices are
+00002540: 206b 6570 7420 616e 6420 6d61 7070 6564   kept and mapped
+00002550: 2074 6f0a 2020 2020 2020 2020 7361 6d65   to.        same
+00002560: 2056 6572 7465 7820 696e 7374 616e 6365   Vertex instance
+00002570: 2061 7320 6e61 6d65 310a 2020 2020 2020   as name1.      
+00002580: 2020 4e29 0372 3a00 0000 7213 0000 00da    N).r:...r.....
+00002590: 0675 7064 6174 6529 0672 1500 0000 da05  .update).r......
+000025a0: 6e61 6d65 31da 056e 616d 6573 da01 7672  name1..names..vr
+000025b0: 5000 0000 724a 0000 0072 1600 0000 7216  P...rJ...r....r.
+000025c0: 0000 0072 1700 0000 da0d 7265 6475 6365  ...r......reduce
+000025d0: 5f76 6572 7465 780b 0100 0073 0c00 0000  _vertex....s....
+000025e0: 0a07 0801 0a01 0e01 0c02 04fc 7a1b 426c  ............z.Bl
+000025f0: 6f63 6b4d 6573 6844 6963 742e 7265 6475  ockMeshDict.redu
+00002600: 6365 5f76 6572 7465 7863 0100 0000 0000  ce_vertexc......
+00002610: 0000 0000 0000 0700 0000 0500 0000 4300  ..............C.
+00002620: 0000 7378 0000 0074 0074 017c 006a 02a0  ..sx...t.t.|.j..
+00002630: 03a1 0083 0164 0164 0284 0064 038d 027d  .....d.d...d...}
+00002640: 0167 007d 0274 047c 0164 0464 0284 0083  .g.}.t.|.d.d....
+00002650: 0244 005d 0b5c 027d 037d 047c 02a0 0574  .D.].\.}.}.|...t
+00002660: 017c 0483 01a1 0101 0071 167c 0244 005d  .|.......q.|.D.]
+00002670: 157d 0574 067c 0583 0164 056b 0272 2d71  .}.t.|...d.k.r-q
+00002680: 2464 0664 0784 007c 0544 0083 017d 067c  $d.d...|.D...}.|
+00002690: 006a 077c 068e 0001 0071 2464 0853 0029  .j.|.....q$d.S.)
+000026a0: 097a 3963 616c 6c20 7265 6475 6365 5f76  .z9call reduce_v
+000026b0: 6572 7465 7820 6f6e 2061 6c6c 2076 6572  ertex on all ver
+000026c0: 7469 6365 7320 7769 7468 2069 6465 6e74  tices with ident
+000026d0: 6963 616c 2076 616c 7565 732e 6301 0000  ical values.c...
+000026e0: 0000 0000 0000 0000 0001 0000 0003 0000  ................
+000026f0: 0053 0000 00f3 0c00 0000 7400 7c00 6401  .S........t.|.d.
+00002700: 1900 8301 5300 a902 4e72 0600 0000 a901  ....S...Nr......
+00002710: 722a 0000 00a9 0172 8700 0000 7216 0000  r*.....r....r...
+00002720: 0072 1600 0000 7217 0000 00da 083c 6c61  .r....r......<la
+00002730: 6d62 6461 3e1e 0100 00f3 0200 0000 0c00  mbda>...........
+00002740: 7a2e 426c 6f63 6b4d 6573 6844 6963 742e  z.BlockMeshDict.
+00002750: 6d65 7267 655f 7665 7274 6963 6573 2e3c  merge_vertices.<
+00002760: 6c6f 6361 6c73 3e2e 3c6c 616d 6264 613e  locals>.<lambda>
+00002770: 2901 da03 6b65 7963 0100 0000 0000 0000  )...keyc........
+00002780: 0000 0000 0100 0000 0300 0000 5300 0000  ............S...
+00002790: 7289 0000 0072 8a00 0000 728b 0000 0072  r....r....r....r
+000027a0: 8c00 0000 7216 0000 0072 1600 0000 7217  ....r....r....r.
+000027b0: 0000 0072 8d00 0000 2101 0000 728e 0000  ...r....!...r...
+000027c0: 0072 0600 0000 6301 0000 0000 0000 0000  .r....c.........
+000027d0: 0000 0002 0000 0004 0000 0053 0000 0073  ...........S...s
+000027e0: 1400 0000 6700 7c00 5d06 7d01 7c01 6400  ....g.|.].}.|.d.
+000027f0: 1900 9102 7102 5300 2901 7201 0000 0072  ....q.S.).r....r
+00002800: 1600 0000 2902 7237 0000 0072 8700 0000  ....).r7...r....
+00002810: 7216 0000 0072 1600 0000 7217 0000 0072  r....r....r....r
+00002820: 5b00 0000 2601 0000 f302 0000 0014 007a  [...&..........z
+00002830: 3042 6c6f 636b 4d65 7368 4469 6374 2e6d  0BlockMeshDict.m
+00002840: 6572 6765 5f76 6572 7469 6365 732e 3c6c  erge_vertices.<l
+00002850: 6f63 616c 733e 2e3c 6c69 7374 636f 6d70  ocals>.<listcomp
+00002860: 3e4e 2908 721c 0000 00da 046c 6973 7472  >N).r......listr
+00002870: 3a00 0000 da05 6974 656d 7372 0200 0000  :.....itemsr....
+00002880: 7261 0000 0072 1a00 0000 7288 0000 0029  ra...r....r....)
+00002890: 0772 1500 0000 5a0f 736f 7274 6564 5f76  .r....Z.sorted_v
+000028a0: 6572 7469 6365 73da 0667 726f 7570 73da  ertices..groups.
+000028b0: 016b da01 67da 0567 726f 7570 7286 0000  .k..g..groupr...
+000028c0: 0072 1600 0000 7216 0000 0072 1700 0000  .r....r....r....
+000028d0: da0e 6d65 7267 655f 7665 7274 6963 6573  ..merge_vertices
+000028e0: 1901 0000 7318 0000 0002 0412 0106 ff04  ....s...........
+000028f0: 0316 0110 0108 010c 0102 010e 010c 0104  ................
+00002900: fc7a 1c42 6c6f 636b 4d65 7368 4469 6374  .z.BlockMeshDict
+00002910: 2e6d 6572 6765 5f76 6572 7469 6365 73da  .merge_vertices.
+00002920: 035f 647a 6304 0000 0000 0000 0000 0000  ._dzc...........
+00002930: 0007 0000 0004 0000 0043 0000 0073 5400  .........C...sT.
+00002940: 0000 7c03 6401 7500 720b 7400 7c00 6a01  ..|.d.u.r.t.|.j.
+00002950: a002 a100 8301 7d03 7c03 4400 5d1a 7d04  ......}.|.D.].}.
+00002960: 7c00 6a01 7c04 1900 7d05 7c05 a003 a100  |.j.|...}.|.....
+00002970: 7d06 7c01 7c06 5f04 7c06 0400 6a05 7c02  }.|.|._.|...j.|.
+00002980: 3700 0200 5f05 7c00 a006 7c06 a101 0100  7..._.|...|.....
+00002990: 710d 6401 5300 2902 7a14 4865 6c70 6572  q.d.S.).z.Helper
+000029a0: 2066 6f72 2032 6420 6d65 7368 6573 4e29   for 2d meshesN)
+000029b0: 0772 6000 0000 723a 0000 00da 046b 6579  .r`...r:.....key
+000029c0: 7372 2300 0000 7211 0000 0072 1200 0000  sr#...r....r....
+000029d0: 7282 0000 0029 0772 1500 0000 7211 0000  r....).r....r...
+000029e0: 00da 0673 7566 6669 7872 3100 0000 da05  ...suffixr1.....
+000029f0: 766e 616d 655a 0976 6572 7465 785f 7a30  vnameZ.vertex_z0
+00002a00: 5a09 7665 7274 6578 5f7a 3172 1600 0000  Z.vertex_z1r....
+00002a10: 7216 0000 0072 1700 0000 da1c 7265 706c  r....r......repl
+00002a20: 6963 6174 655f 7665 7274 6963 6573 5f66  icate_vertices_f
+00002a30: 7572 7468 6572 5f7a 2901 0000 7312 0000  urther_z)...s...
+00002a40: 0008 020e 0108 010a 0108 0106 010e 010c  ................
+00002a50: 0104 fb7a 2a42 6c6f 636b 4d65 7368 4469  ...z*BlockMeshDi
+00002a60: 6374 2e72 6570 6c69 6361 7465 5f76 6572  ct.replicate_ver
+00002a70: 7469 6365 735f 6675 7274 6865 725f 7a72  tices_further_zr
+00002a80: 0600 0000 6305 0000 0000 0000 0000 0000  ....c...........
+00002a90: 0006 0000 0005 0000 0043 0000 0073 3400  .........C...s4.
+00002aa0: 0000 7c03 6400 7500 720c 6401 7400 7c00  ..|.d.u.r.d.t.|.
+00002ab0: 6a01 8301 9b00 9d02 7d03 7402 7c01 7c02  j.......}.t.|.|.
+00002ac0: 7c03 7c04 8304 7d05 7c05 7c00 6a01 7c03  |.|...}.|.|.j.|.
+00002ad0: 3c00 7c05 5300 2902 4e72 5200 0000 2903  <.|.S.).NrR...).
+00002ae0: 721a 0000 0072 7100 0000 7246 0000 0029  r....rq...rF...)
+00002af0: 0672 1500 0000 7231 0000 00da 086e 785f  .r....r1.....nx_
+00002b00: 6e79 5f6e 7a72 1200 0000 7248 0000 0072  ny_nzr....rH...r
+00002b10: 5200 0000 7216 0000 0072 1600 0000 7217  R...r....r....r.
+00002b20: 0000 00da 0c61 6464 5f68 6578 626c 6f63  .....add_hexbloc
+00002b30: 6b34 0100 0073 0a00 0000 0803 1001 0e01  k4...s..........
+00002b40: 0a01 0401 7a1a 426c 6f63 6b4d 6573 6844  ....z.BlockMeshD
+00002b50: 6963 742e 6164 645f 6865 7862 6c6f 636b  ict.add_hexblock
+00002b60: da00 6307 0000 0000 0000 0000 0000 0007  ..c.............
+00002b70: 0000 0006 0000 0003 0000 0073 3000 0000  ...........s0...
+00002b80: 7c00 a000 8700 6601 6401 6402 8408 7c01  |.....f.d.d...|.
+00002b90: 4400 8301 8701 6601 6403 6402 8408 7c01  D.....f.d.d...|.
+00002ba0: 4400 8301 1700 7c02 7c03 7c04 a104 5300  D.....|.|.|...S.
+00002bb0: 2904 4e63 0100 0000 0000 0000 0000 0000  ).Nc............
+00002bc0: 0200 0000 0400 0000 1300 0000 f314 0000  ................
+00002bd0: 0067 007c 005d 067d 017c 0188 0017 0091  .g.|.].}.|......
+00002be0: 0271 0253 0072 1600 0000 7216 0000 00a9  .q.S.r....r.....
+00002bf0: 0272 3700 0000 729b 0000 0029 01da 0973  .r7...r....)...s
+00002c00: 7566 6669 785f 7a6d 7216 0000 0072 1700  uffix_zmr....r..
+00002c10: 0000 725b 0000 0047 0100 0072 9000 0000  ..r[...G...r....
+00002c20: 7a36 426c 6f63 6b4d 6573 6844 6963 742e  z6BlockMeshDict.
+00002c30: 6164 645f 6865 7862 6c6f 636b 5f66 726f  add_hexblock_fro
+00002c40: 6d5f 3264 2e3c 6c6f 6361 6c73 3e2e 3c6c  m_2d.<locals>.<l
+00002c50: 6973 7463 6f6d 703e 6301 0000 0000 0000  istcomp>c.......
+00002c60: 0000 0000 0002 0000 0004 0000 0013 0000  ................
+00002c70: 0072 a000 0000 7216 0000 0072 1600 0000  .r....r....r....
+00002c80: 72a1 0000 0029 01da 0973 7566 6669 785f  r....)...suffix_
+00002c90: 7a70 7216 0000 0072 1700 0000 725b 0000  zpr....r....r[..
+00002ca0: 0048 0100 0072 9000 0000 2901 729e 0000  .H...r....).r...
+00002cb0: 0029 0772 1500 0000 7231 0000 0072 9d00  .).r....r1...r..
+00002cc0: 0000 7212 0000 0072 4800 0000 72a2 0000  ..r....rH...r...
+00002cd0: 0072 a300 0000 7216 0000 0029 0272 a200  .r....r....).r..
+00002ce0: 0000 72a3 0000 0072 1700 0000 da14 6164  ..r....r......ad
+00002cf0: 645f 6865 7862 6c6f 636b 5f66 726f 6d5f  d_hexblock_from_
+00002d00: 3264 3d01 0000 7310 0000 0004 0910 0110  2d=...s.........
+00002d10: 0102 ff02 0202 0102 0104 fb7a 2242 6c6f  ...........z"Blo
+00002d20: 636b 4d65 7368 4469 6374 2e61 6464 5f68  ckMeshDict.add_h
+00002d30: 6578 626c 6f63 6b5f 6672 6f6d 5f32 6463  exblock_from_2dc
+00002d40: 0400 0000 0000 0000 0000 0000 0500 0000  ................
+00002d50: 0400 0000 4300 0000 f31a 0000 0074 007c  ....C........t.|
+00002d60: 017c 027c 0383 037d 047c 047c 006a 017c  .|.|...}.|.|.j.|
+00002d70: 023c 007c 0453 0072 0e00 0000 2902 7207  .<.|.S.r....).r.
+00002d80: 0000 0072 7200 0000 2905 7215 0000 0072  ...rr...).r....r
+00002d90: 3100 0000 7212 0000 005a 0c69 6e74 6572  1...r....Z.inter
+00002da0: 5f76 6572 7465 7872 4c00 0000 7216 0000  _vertexrL...r...
+00002db0: 0072 1600 0000 7217 0000 00da 0b61 6464  .r....r......add
+00002dc0: 5f61 7263 6564 6765 4e01 0000 f306 0000  _arcedgeN.......
+00002dd0: 000c 010a 0104 017a 1942 6c6f 636b 4d65  .......z.BlockMe
+00002de0: 7368 4469 6374 2e61 6464 5f61 7263 6564  shDict.add_arced
+00002df0: 6765 6304 0000 0000 0000 0000 0000 0005  gec.............
+00002e00: 0000 0004 0000 0043 0000 0072 a500 0000  .......C...r....
+00002e10: 720e 0000 0029 0272 0800 0000 7272 0000  r....).r....rr..
+00002e20: 0029 0572 1500 0000 7231 0000 0072 1200  .).r....r1...r..
+00002e30: 0000 da06 706f 696e 7473 724c 0000 0072  ....pointsrL...r
+00002e40: 1600 0000 7216 0000 0072 1700 0000 da0e  ....r....r......
+00002e50: 6164 645f 7370 6c69 6e65 6564 6765 5301  add_splineedgeS.
+00002e60: 0000 72a7 0000 007a 1c42 6c6f 636b 4d65  ..r....z.BlockMe
+00002e70: 7368 4469 6374 2e61 6464 5f73 706c 696e  shDict.add_splin
+00002e80: 6565 6467 6563 0500 0000 0000 0000 0000  eedgec..........
+00002e90: 0000 0600 0000 0500 0000 4300 0000 731c  ..........C...s.
+00002ea0: 0000 0074 007c 017c 027c 037c 0483 047d  ...t.|.|.|.|...}
+00002eb0: 057c 057c 006a 017c 023c 007c 0553 0072  .|.|.j.|.<.|.S.r
+00002ec0: 0e00 0000 2902 7268 0000 0072 7300 0000  ....).rh...rs...
+00002ed0: 2906 7215 0000 0072 6900 0000 7212 0000  ).r....ri...r...
+00002ee0: 0072 6700 0000 726a 0000 0072 5200 0000  .rg...rj...rR...
+00002ef0: 7216 0000 0072 1600 0000 7217 0000 00da  r....r....r.....
+00002f00: 0c61 6464 5f62 6f75 6e64 6172 7958 0100  .add_boundaryX..
+00002f10: 0073 0600 0000 0e01 0a01 0401 7a1a 426c  .s..........z.Bl
+00002f20: 6f63 6b4d 6573 6844 6963 742e 6164 645f  ockMeshDict.add_
+00002f30: 626f 756e 6461 7279 7244 0000 0072 4500  boundaryrD...rE.
+00002f40: 0000 6303 0000 0000 0000 0000 0000 0004  ..c.............
+00002f50: 0000 0003 0000 0043 0000 0073 1800 0000  .......C...s....
+00002f60: 7400 7c01 7c02 8302 7d03 7c03 7c00 6a01  t.|.|...}.|.|.j.
+00002f70: 7c01 3c00 7c03 5300 2901 7a19 4164 6420  |.<.|.S.).z.Add 
+00002f80: 3220 626f 756e 6461 7269 6573 2074 6f20  2 boundaries to 
+00002f90: 6d65 7267 6529 0272 4200 0000 7274 0000  merge).rB...rt..
+00002fa0: 0029 0472 1500 0000 7244 0000 0072 4500  .).r....rD...rE.
+00002fb0: 0000 7252 0000 0072 1600 0000 7216 0000  ..rR...r....r...
+00002fc0: 0072 1700 0000 da15 6164 645f 6d65 7267  .r......add_merg
+00002fd0: 655f 7061 7463 685f 7061 6972 735d 0100  e_patch_pairs]..
+00002fe0: 0073 0600 0000 0a02 0a01 0401 7a23 426c  .s..........z#Bl
+00002ff0: 6f63 6b4d 6573 6844 6963 742e 6164 645f  ockMeshDict.add_
+00003000: 6d65 7267 655f 7061 7463 685f 7061 6972  merge_patch_pair
+00003010: 7363 0500 0000 0000 0000 0000 0000 0700  sc..............
+00003020: 0000 0600 0000 4300 0000 732c 0000 007c  ......C...s,...|
+00003030: 006a 0064 017c 017c 037c 0264 028d 047d  .j.d.|.|.|.d...}
+00003040: 057c 006a 0064 017c 027c 047c 0164 028d  .|.j.d.|.|.|.d..
+00003050: 047d 067c 057c 0666 0253 0029 037a ca41  .}.|.|.f.S.).z.A
+00003060: 6464 2032 2063 7963 6c69 6320 626f 756e  dd 2 cyclic boun
+00003070: 6461 7269 6573 0a0a 2020 2020 2020 2020  daries..        
+00003080: 4578 616d 706c 650a 2020 2020 2020 2020  Example.        
+00003090: 2d2d 2d2d 2d2d 2d0a 0a20 2020 2020 2020  -------..       
+000030a0: 2032 2063 7963 6c69 6320 626f 756e 6461   2 cyclic bounda
+000030b0: 7269 6573 2063 616e 2062 6520 6372 6561  ries can be crea
+000030c0: 7465 6420 6173 2066 6f6c 6c6f 773a 3a0a  ted as follow::.
+000030d0: 0a20 2020 2020 2020 2020 2061 6464 5f63  .          add_c
+000030e0: 7963 6c69 635f 626f 756e 6461 7269 6573  yclic_boundaries
+000030f0: 2822 6f75 746c 6574 222c 2022 696e 6c65  ("outlet", "inle
+00003100: 7422 2c20 6230 2e66 6163 6528 2265 2229  t", b0.face("e")
+00003110: 2c20 6230 2e66 6163 6528 2277 2229 290a  , b0.face("w")).
+00003120: 0a20 2020 2020 2020 205a 0663 7963 6c69  .        Z.cycli
+00003130: 6329 0172 6a00 0000 2901 72aa 0000 0029  c).rj...).r....)
+00003140: 0772 1500 0000 5a05 6e61 6d65 3072 8500  .r....Z.name0r..
+00003150: 0000 5a06 6661 6365 7330 5a06 6661 6365  ..Z.faces0Z.face
+00003160: 7331 da02 6230 da02 6231 7216 0000 0072  s1..b0..b1r....r
+00003170: 1600 0000 7217 0000 00da 1561 6464 5f63  ....r......add_c
+00003180: 7963 6c69 635f 626f 756e 6461 7269 6573  yclic_boundaries
+00003190: 6301 0000 7306 0000 0012 0b12 0108 017a  c...s..........z
+000031a0: 2342 6c6f 636b 4d65 7368 4469 6374 2e61  #BlockMeshDict.a
+000031b0: 6464 5f63 7963 6c69 635f 626f 756e 6461  dd_cyclic_bounda
+000031c0: 7269 6573 5463 0200 0000 0000 0000 0000  riesTc..........
+000031d0: 0000 0800 0000 0500 0000 4300 0000 73ba  ..........C...s.
+000031e0: 0000 0074 0083 007d 0267 007c 005f 017c  ...t...}.g.|._.|
+000031f0: 006a 02a0 03a1 0044 005d 1e7d 037c 036a  .j.....D.].}.|.j
+00003200: 0444 005d 187d 047c 006a 057c 0419 007d  .D.].}.|.j.|...}
+00003210: 057c 056a 067c 0276 0172 287c 02a0 077c  .|.j.|.v.r(|...|
+00003220: 056a 06a1 0101 007c 006a 01a0 087c 05a1  .j.....|.j...|..
+00003230: 0101 0071 1071 0b7c 0164 016b 0272 4667  ...q.q.|.d.k.rFg
+00003240: 007c 005f 017c 006a 05a0 09a1 0044 005d  .|._.|.j.....D.]
+00003250: 0e5c 027d 067d 057c 067c 0276 0072 447c  .\.}.}.|.|.v.rD|
+00003260: 006a 01a0 087c 05a1 0101 0071 366e 087c  .j...|.....q6n.|
+00003270: 0172 4e74 0a7c 006a 0183 017c 005f 0174  .rNt.|.j...|._.t
+00003280: 0b7c 006a 0183 0144 005d 075c 027d 077d  .|.j...D.].\.}.}
+00003290: 057c 077c 055f 0c71 5364 0253 0029 037a  .|.|._.qSd.S.).z
+000032a0: e331 2e20 6372 6561 7465 206c 6973 7420  .1. create list 
+000032b0: 6f66 2056 6572 7465 7820 7768 6963 6820  of Vertex which 
+000032c0: 6172 6520 7265 6665 7272 6564 2062 7920  are referred by 
+000032d0: 626c 6f63 6b73 206f 6e6c 792e 0a20 2020  blocks only..   
+000032e0: 2020 2020 2032 2e20 736f 7274 2076 6572       2. sort ver
+000032f0: 7465 7820 6163 636f 7264 696e 6720 746f  tex according to
+00003300: 2028 782c 2079 2c20 7a29 0a20 2020 2020   (x, y, z).     
+00003310: 2020 2033 2e20 6173 7369 676e 2073 6571     3. assign seq
+00003320: 7565 6e63 6520 6e75 6d62 6572 2066 6f72  uence number for
+00003330: 2065 6163 6820 5665 7274 6578 0a20 2020   each Vertex.   
+00003340: 2020 2020 2034 2e20 736f 7274 6564 206c       4. sorted l
+00003350: 6973 7420 6973 2073 6176 6564 2061 7320  ist is saved as 
+00003360: 7365 6c66 2e5f 7665 7274 6963 6573 5f69  self._vertices_i
+00003370: 6e5f 626c 6f63 6b6d 6573 680a 2020 2020  n_blockmesh.    
+00003380: 2020 2020 5a08 6173 5f61 6464 6564 4e29      Z.as_addedN)
+00003390: 0dda 0373 6574 7275 0000 0072 7100 0000  ...setru...rq...
+000033a0: da06 7661 6c75 6573 7231 0000 0072 3a00  ..valuesr1...r:.
+000033b0: 0000 7212 0000 00da 0361 6464 7261 0000  ..r......addra..
+000033c0: 0072 9200 0000 721c 0000 00da 0965 6e75  .r....r......enu
+000033d0: 6d65 7261 7465 7214 0000 0029 0872 1500  merater....).r..
+000033e0: 0000 da04 736f 7274 5a0b 766e 616d 6573  ....sortZ.vnames
+000033f0: 5f6b 6570 7472 5200 0000 7250 0000 0072  _keptrR...rP...r
+00003400: 8700 0000 729b 0000 0072 5a00 0000 7216  ....r....rZ...r.
+00003410: 0000 0072 1600 0000 7217 0000 00da 0f61  ...r....r......a
+00003420: 7373 6967 6e5f 7665 7274 6578 6964 7201  ssign_vertexidr.
+00003430: 0000 732c 0000 0006 0706 010e 010a 010a  ..s,............
+00003440: 010a 010c 010c 0102 8002 fc08 0506 0112  ................
+00003450: 0108 010c 0102 8002 fe04 030c 0112 0108  ................
+00003460: 0104 ff7a 1d42 6c6f 636b 4d65 7368 4469  ...z.BlockMeshDi
+00003470: 6374 2e61 7373 6967 6e5f 7665 7274 6578  ct.assign_vertex
+00003480: 6964 6301 0000 0000 0000 0000 0000 0003  idc.............
+00003490: 0000 0006 0000 0043 0000 0073 3800 0000  .......C...s8...
+000034a0: 6401 6701 7d01 7c00 6a00 4400 5d0b 7d02  d.g.}.|.j.D.].}.
+000034b0: 7c01 a001 6402 7c02 a002 a100 1700 a101  |...d.|.........
+000034c0: 0100 7106 7c01 a001 6403 a101 0100 6404  ..q.|...d.....d.
+000034d0: a003 7c01 a101 5300 2905 7aec 666f 726d  ..|...S.).z.form
+000034e0: 6174 2076 6572 7469 6365 7320 7365 6374  at vertices sect
+000034f0: 696f 6e2e 0a20 2020 2020 2020 2061 7373  ion..        ass
+00003500: 6967 6e5f 7665 7274 6578 6964 2829 2073  ign_vertexid() s
+00003510: 686f 756c 6420 6265 2063 616c 6c65 6420  hould be called 
+00003520: 6265 666f 7265 2074 6869 7320 6d65 7468  before this meth
+00003530: 6f64 2c20 6265 6361 7573 650a 2020 2020  od, because.    
+00003540: 2020 2020 7365 6c66 2e5f 7665 7274 6963      self._vertic
+00003550: 6573 5f69 6e5f 626c 6f63 6b6d 6573 6820  es_in_blockmesh 
+00003560: 7368 6f75 6c64 2062 6520 6176 6169 6c61  should be availa
+00003570: 626c 6520 616e 640a 2020 2020 2020 2020  ble and.        
+00003580: 6d65 6d62 6572 7320 6f66 2073 656c 662e  members of self.
+00003590: 5f76 6572 7469 6365 735f 696e 5f62 6c6f  _vertices_in_blo
+000035a0: 636b 6d65 7368 2073 686f 756c 6420 6861  ckmesh should ha
+000035b0: 7665 2076 616c 6964 2069 6e64 6578 2e0a  ve valid index..
+000035c0: 2020 2020 2020 2020 7a0a 7665 7274 6963          z.vertic
+000035d0: 6573 0a28 fa04 2020 2020 fa02 293b 726c  es.(..    ..);rl
+000035e0: 0000 0029 0472 7500 0000 7261 0000 0072  ...).ru...ra...r
+000035f0: 1e00 0000 721b 0000 0029 0372 1500 0000  ....r....).r....
+00003600: 726d 0000 0072 8700 0000 7216 0000 0072  rm...r....r....r
+00003610: 1600 0000 7217 0000 00da 1766 6f72 6d61  ....r......forma
+00003620: 745f 7665 7274 6963 6573 5f73 6563 7469  t_vertices_secti
+00003630: 6f6e 8b01 0000 730a 0000 0006 060a 0114  on....s.........
+00003640: 010a 010a 017a 2542 6c6f 636b 4d65 7368  .....z%BlockMesh
+00003650: 4469 6374 2e66 6f72 6d61 745f 7665 7274  Dict.format_vert
+00003660: 6963 6573 5f73 6563 7469 6f6e 6301 0000  ices_sectionc...
+00003670: 0000 0000 0000 0000 0003 0000 0007 0000  ................
+00003680: 0043 0000 00f3 4000 0000 6401 6701 7d01  .C....@...d.g.}.
+00003690: 7c00 6a00 a001 a100 4400 5d0d 7d02 7c01  |.j.....D.].}.|.
+000036a0: a002 6402 7c02 a003 7c00 6a04 a101 1700  ..d.|...|.j.....
+000036b0: a101 0100 7108 7c01 a002 6403 a101 0100  ....q.|...d.....
+000036c0: 6404 a005 7c01 a101 5300 2905 7aa2 666f  d...|...S.).z.fo
+000036d0: 726d 6174 2062 6c6f 636b 7320 7365 6374  rmat blocks sect
+000036e0: 696f 6e2e 0a20 2020 2020 2020 2061 7373  ion..        ass
+000036f0: 6967 6e5f 7665 7274 6578 6964 2829 2073  ign_vertexid() s
+00003700: 686f 756c 6420 6265 2063 616c 6c65 6420  hould be called 
+00003710: 6265 666f 7265 2074 6869 7320 6d65 7468  before this meth
+00003720: 6f64 2c20 6265 6361 7573 650a 2020 2020  od, because.    
+00003730: 2020 2020 7665 7274 6963 6573 2072 6566      vertices ref
+00003740: 6572 6564 2062 7920 626c 6f63 6b73 2073  ered by blocks s
+00003750: 686f 756c 6420 6861 7665 2076 616c 6964  hould have valid
+00003760: 2069 6e64 6578 2e0a 2020 2020 2020 2020   index..        
+00003770: 7a08 626c 6f63 6b73 0a28 72b5 0000 0072  z.blocks.(r....r
+00003780: b600 0000 726c 0000 0029 0672 7100 0000  ....rl...).rq...
+00003790: 72b0 0000 0072 6100 0000 721e 0000 0072  r....ra...r....r
+000037a0: 3a00 0000 721b 0000 0029 0372 1500 0000  :...r....).r....
+000037b0: 726d 0000 0072 5200 0000 7216 0000 0072  rm...rR...r....r
+000037c0: 1600 0000 7217 0000 00da 1566 6f72 6d61  ....r......forma
+000037d0: 745f 626c 6f63 6b73 5f73 6563 7469 6f6e  t_blocks_section
+000037e0: 9701 0000 730a 0000 0006 050e 0118 010a  ....s...........
+000037f0: 010a 017a 2342 6c6f 636b 4d65 7368 4469  ...z#BlockMeshDi
+00003800: 6374 2e66 6f72 6d61 745f 626c 6f63 6b73  ct.format_blocks
+00003810: 5f73 6563 7469 6f6e 6301 0000 0000 0000  _sectionc.......
+00003820: 0000 0000 0003 0000 0007 0000 0043 0000  .............C..
+00003830: 0072 b800 0000 2905 7aa1 666f 726d 6174  .r....).z.format
+00003840: 2065 6467 6573 2073 6563 7469 6f6e 2e0a   edges section..
+00003850: 2020 2020 2020 2020 6173 7369 676e 5f76          assign_v
+00003860: 6572 7465 7869 6428 2920 7368 6f75 6c64  ertexid() should
+00003870: 2062 6520 6361 6c6c 6564 2062 6566 6f72   be called befor
+00003880: 6520 7468 6973 206d 6574 686f 642c 2062  e this method, b
+00003890: 6563 6175 7365 0a20 2020 2020 2020 2076  ecause.        v
+000038a0: 6572 7469 6365 7320 7265 6665 7265 6420  ertices refered 
+000038b0: 6279 2062 6c6f 636b 7320 7368 6f75 6c64  by blocks should
+000038c0: 2068 6176 6520 7661 6c69 6420 696e 6465   have valid inde
+000038d0: 782e 0a20 2020 2020 2020 207a 0765 6467  x..        z.edg
+000038e0: 6573 0a28 72b5 0000 0072 b600 0000 726c  es.(r....r....rl
+000038f0: 0000 0029 0672 7200 0000 72b0 0000 0072  ...).rr...r....r
+00003900: 6100 0000 721e 0000 0072 3a00 0000 721b  a...r....r:...r.
+00003910: 0000 0029 0372 1500 0000 726d 0000 0072  ...).r....rm...r
+00003920: 4c00 0000 7216 0000 0072 1600 0000 7217  L...r....r....r.
+00003930: 0000 00da 1466 6f72 6d61 745f 6564 6765  .....format_edge
+00003940: 735f 7365 6374 696f 6ea2 0100 0073 0a00  s_section....s..
+00003950: 0000 0606 0e01 1801 0a01 0a01 7a22 426c  ............z"Bl
+00003960: 6f63 6b4d 6573 6844 6963 742e 666f 726d  ockMeshDict.form
+00003970: 6174 5f65 6467 6573 5f73 6563 7469 6f6e  at_edges_section
+00003980: 6301 0000 0000 0000 0000 0000 0005 0000  c...............
+00003990: 0006 0000 0043 0000 0073 5400 0000 6401  .....C...sT...d.
+000039a0: 6701 7d01 7c00 6a00 a001 a100 4400 5d17  g.}.|.j.....D.].
+000039b0: 7d02 6402 7d03 7c02 a002 7c00 6a03 a101  }.d.}.|...|.j...
+000039c0: a004 6403 6403 7c03 1700 a102 7d04 7c01  ..d.d.|.....}.|.
+000039d0: a005 7c03 7c04 1700 a101 0100 7108 7c01  ..|.|.......q.|.
+000039e0: a005 6404 a101 0100 6403 a006 7c01 a101  ..d.....d...|...
+000039f0: 5300 2905 7aa3 666f 726d 6174 2062 6f75  S.).z.format bou
+00003a00: 6e64 6172 7920 7365 6374 696f 6e2e 0a20  ndary section.. 
+00003a10: 2020 2020 2020 2061 7373 6967 6e5f 7665         assign_ve
+00003a20: 7274 6578 6964 2829 2073 686f 756c 6420  rtexid() should 
+00003a30: 6265 2063 616c 6c65 6420 6265 666f 7265  be called before
+00003a40: 2074 6869 7320 6d65 7468 6f64 2c20 6265   this method, be
+00003a50: 6361 7573 650a 2020 2020 2020 2020 7665  cause.        ve
+00003a60: 7274 6963 6573 2072 6566 6572 6564 2062  rtices refered b
+00003a70: 7920 6661 6365 7320 7368 6f75 6c64 2068  y faces should h
+00003a80: 6176 6520 7661 6c69 6420 696e 6465 782e  ave valid index.
+00003a90: 0a20 2020 2020 2020 207a 0a62 6f75 6e64  .        z.bound
+00003aa0: 6172 790a 2872 b500 0000 726c 0000 0072  ary.(r....rl...r
+00003ab0: b600 0000 2907 7273 0000 0072 b000 0000  ....).rs...r....
+00003ac0: 721e 0000 0072 3a00 0000 da07 7265 706c  r....r:.....repl
+00003ad0: 6163 6572 6100 0000 721b 0000 0029 0572  acera...r....).r
+00003ae0: 1500 0000 726d 0000 0072 5200 0000 da06  ....rm...rR.....
+00003af0: 696e 6465 6e74 723e 0000 0072 1600 0000  indentr>...r....
+00003b00: 7216 0000 0072 1700 0000 da17 666f 726d  r....r......form
+00003b10: 6174 5f62 6f75 6e64 6172 795f 7365 6374  at_boundary_sect
+00003b20: 696f 6eae 0100 0073 0e00 0000 0606 0e01  ion....s........
+00003b30: 0402 1801 1001 0a01 0a01 7a25 426c 6f63  ..........z%Bloc
+00003b40: 6b4d 6573 6844 6963 742e 666f 726d 6174  kMeshDict.format
+00003b50: 5f62 6f75 6e64 6172 795f 7365 6374 696f  _boundary_sectio
+00003b60: 6e63 0100 0000 0000 0000 0000 0000 0400  nc..............
+00003b70: 0000 0600 0000 4300 0000 7352 0000 007c  ......C...sR...|
+00003b80: 006a 0073 0564 0153 0064 027d 0164 0367  .j.s.d.S.d.}.d.g
+00003b90: 017d 027c 006a 00a0 01a1 0044 005d 0b7d  .}.|.j.....D.].}
+00003ba0: 037c 02a0 027c 017c 03a0 03a1 0017 00a1  .|...|.|........
+00003bb0: 0101 0071 0f7c 02a0 0264 04a1 0101 0064  ...q.|...d.....d
+00003bc0: 0564 05a0 047c 02a1 0117 0064 0517 0053  .d...|.....d...S
+00003bd0: 0029 064e 729f 0000 0072 b500 0000 7a11  .).Nr....r....z.
+00003be0: 6d65 7267 6550 6174 6368 5061 6972 730a  mergePatchPairs.
+00003bf0: 2872 b600 0000 726c 0000 0029 0572 7400  (r....rl...).rt.
+00003c00: 0000 72b0 0000 0072 6100 0000 721e 0000  ..r....ra...r...
+00003c10: 0072 1b00 0000 2904 7215 0000 0072 bc00  .r....).r....r..
+00003c20: 0000 726d 0000 0072 5200 0000 7216 0000  ..rm...rR...r...
+00003c30: 0072 1600 0000 7217 0000 00da 1e66 6f72  .r....r......for
+00003c40: 6d61 745f 6d65 7267 6570 6174 6368 7061  mat_mergepatchpa
+00003c50: 6972 735f 7365 6374 696f 6ebd 0100 0073  irs_section....s
+00003c60: 1000 0000 0601 0401 0401 0601 0e01 1401  ................
+00003c70: 0a01 1201 7a2c 426c 6f63 6b4d 6573 6844  ....z,BlockMeshD
+00003c80: 6963 742e 666f 726d 6174 5f6d 6572 6765  ict.format_merge
+00003c90: 7061 7463 6870 6169 7273 5f73 6563 7469  patchpairs_secti
+00003ca0: 6f6e 6303 0000 0000 0000 0000 0000 0004  onc.............
+00003cb0: 0000 0009 0000 0043 0000 0073 4600 0000  .......C...sF...
+00003cc0: 7c00 6a00 7c02 6401 8d01 0100 7401 6402  |.j.|.d.....t.d.
+00003cd0: 8301 7d03 7c03 6a02 7c01 7403 7c00 6a04  ..}.|.j.|.t.|.j.
+00003ce0: 8301 7c00 a005 a100 7c00 a006 a100 7c00  ..|.....|.....|.
+00003cf0: a007 a100 7c00 a008 a100 7c00 a009 a100  ....|.....|.....
+00003d00: 6403 8d07 5300 2904 4e29 0172 b300 0000  d...S.).N).r....
+00003d10: 616d 0100 0024 6865 6164 6572 0a46 6f61  am...$header.Foa
+00003d20: 6d46 696c 650a 7b0a 2020 2020 7665 7273  mFile.{.    vers
+00003d30: 696f 6e20 2020 2020 322e 303b 0a20 2020  ion     2.0;.   
+00003d40: 2066 6f72 6d61 7420 2020 2020 2061 7363   format      asc
+00003d50: 6969 3b0a 2020 2020 636c 6173 7320 2020  ii;.    class   
+00003d60: 2020 2020 6469 6374 696f 6e61 7279 3b0a      dictionary;.
+00003d70: 2020 2020 6f62 6a65 6374 2020 2020 2020      object      
+00003d80: 626c 6f63 6b4d 6573 6844 6963 743b 0a7d  blockMeshDict;.}
+00003d90: 0a2f 2f20 2a20 2a20 2a20 2a20 2a20 2a20  .// * * * * * * 
+00003da0: 2a20 2a20 2a20 2a20 2a20 2a20 2a20 2a20  * * * * * * * * 
+00003db0: 2a20 2a20 2a20 2a20 2a20 2a20 2a20 2a20  * * * * * * * * 
+00003dc0: 2a20 2a20 2a20 2a20 2a20 2a20 2a20 2a20  * * * * * * * * 
+00003dd0: 2a20 2a20 2a20 2a20 2a20 2a20 2a20 2f2f  * * * * * * * //
+00003de0: 0a0a 7363 616c 6520 2020 246d 6574 7269  ..scale   $metri
+00003df0: 6363 6f6e 7665 7274 3b0a 0a24 7665 7274  cconvert;..$vert
+00003e00: 6963 6573 0a0a 2462 6c6f 636b 730a 0a24  ices..$blocks..$
+00003e10: 6564 6765 730a 0a24 626f 756e 6461 7279  edges..$boundary
+00003e20: 0a24 6d65 7267 6570 6174 6368 7061 6972  .$mergepatchpair
+00003e30: 730a 2f2f 202a 2a2a 2a2a 2a2a 2a2a 2a2a  s.// ***********
+00003e40: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
+00003e50: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
+00003e60: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
+00003e70: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 202f  ************** /
+00003e80: 2f0a 2907 da06 6865 6164 6572 5a0d 6d65  /.)...headerZ.me
+00003e90: 7472 6963 636f 6e76 6572 7472 3a00 0000  tricconvertr:...
+00003ea0: 7272 0000 0072 7100 0000 da08 626f 756e  rr...rq.....boun
+00003eb0: 6461 7279 5a0f 6d65 7267 6570 6174 6368  daryZ.mergepatch
+00003ec0: 7061 6972 7329 0a72 b400 0000 7203 0000  pairs).r....r...
+00003ed0: 00da 0a73 7562 7374 6974 7574 6572 3500  ...substituter5.
+00003ee0: 0000 7270 0000 0072 b700 0000 72ba 0000  ..rp...r....r...
+00003ef0: 0072 b900 0000 72bd 0000 0072 be00 0000  .r....r....r....
+00003f00: 2904 7215 0000 0072 bf00 0000 5a0d 736f  ).r....r....Z.so
+00003f10: 7274 5f76 6f72 7469 6365 73da 0874 656d  rt_vortices..tem
+00003f20: 706c 6174 6572 1600 0000 7216 0000 0072  plater....r....r
+00003f30: 1700 0000 721e 0000 00c7 0100 0073 1a00  ....r........s..
+00003f40: 0000 0c01 0201 0201 04ff 0419 0201 0801  ................
+00003f50: 0601 0601 0601 0601 0601 06f9 7a14 426c  ............z.Bl
+00003f60: 6f63 6b4d 6573 6844 6963 742e 666f 726d  ockMeshDict.form
+00003f70: 6174 2903 4e4e 4e29 0272 9800 0000 4e72  at).NNN).r....Nr
+00003f80: 6e00 0000 2901 5429 1c72 2c00 0000 722d  n...).T).r,...r-
+00003f90: 0000 0072 2e00 0000 7218 0000 0072 7d00  ...r....r....r}.
+00003fa0: 0000 727f 0000 0072 8200 0000 7283 0000  ..r....r....r...
+00003fb0: 0072 8800 0000 7297 0000 0072 9c00 0000  .r....r....r....
+00003fc0: 720b 0000 0072 9e00 0000 72a4 0000 0072  r....r....r....r
+00003fd0: a600 0000 72a9 0000 0072 aa00 0000 7235  ....r....r....r5
+00003fe0: 0000 0072 ab00 0000 72ae 0000 0072 b400  ...r....r....r..
+00003ff0: 0000 72b7 0000 0072 b900 0000 72ba 0000  ..r....r....r...
+00004000: 0072 bd00 0000 72be 0000 0072 0500 0000  .r....r....r....
+00004010: 721e 0000 0072 1600 0000 7216 0000 0072  r....r....r....r
+00004020: 1600 0000 7217 0000 0072 6f00 0000 d900  ....r....ro.....
+00004030: 0000 7338 0000 0008 0008 0108 0908 0e0a  ..s8............
+00004040: 0308 1308 0408 0e0a 100c 0c0a ff02 0d0a  ................
+00004050: 0102 0102 010a f908 1108 050a 0512 0508  ................
+00004060: 060a 0f08 1908 0c08 0b08 0c08 0f12 0a72  ...............r
+00004070: 6f00 0000 6300 0000 0000 0000 0000 0000  o...c...........
+00004080: 0000 0000 0003 0000 0000 0000 0073 1c00  .............s..
+00004090: 0000 6500 5a01 6400 5a02 8700 6601 6401  ..e.Z.d.Z...f.d.
+000040a0: 6402 8408 5a03 8700 0400 5a04 5300 2903  d...Z.....Z.S.).
+000040b0: da18 426c 6f63 6b4d 6573 6844 6963 7452  ..BlockMeshDictR
+000040c0: 6563 7469 6c69 6e65 6172 6308 0000 0000  ectilinearc.....
+000040d0: 0000 0000 0000 000b 0000 0008 0000 0003  ................
+000040e0: 0000 0073 b000 0000 7400 8300 a001 a100  ...s....t.......
+000040f0: 0100 7c00 a002 7c07 a101 0100 7403 6401  ..|...|.....t.d.
+00004100: 6401 6401 6402 8304 7403 7c01 6401 6401  d.d.d...t.|.d.d.
+00004110: 6403 8304 7403 7c01 7c02 6401 6404 8304  d...t.|.|.d.d...
+00004120: 7403 6401 7c02 6401 6405 8304 6704 7d08  t.d.|.d.d...g.}.
+00004130: 7c08 4400 5d1c 7d09 7c00 a004 7c09 6a05  |.D.].}.|...|.j.
+00004140: 7c09 6a06 6401 7c09 6a07 6406 1700 a104  |.j.d.|.j.d.....
+00004150: 0100 7c00 a004 7c09 6a05 7c09 6a06 7c03  ..|...|.j.|.j.|.
+00004160: 7c09 6a07 6407 1700 a104 0100 7126 6408  |.j.d.......q&d.
+00004170: 6409 8400 640a 4400 8301 7d0a 7c00 6a08  d...d.D...}.|.j.
+00004180: 7c0a 7c04 7c05 7c06 6603 640b 640c 8d03  |.|.|.|.f.d.d...
+00004190: 7c00 5f09 6400 5300 290d 4e72 0100 0000  |._.d.S.).Nr....
+000041a0: 5a02 7630 da02 7631 da02 7632 5a02 7633  Z.v0..v1..v2Z.v3
+000041b0: fa04 2d62 6f74 fa04 2d74 6f70 6301 0000  ..-bot..-topc...
+000041c0: 0000 0000 0000 0000 0003 0000 0006 0000  ................
+000041d0: 0053 0000 0073 2800 0000 6700 7c00 5d10  .S...s(...g.|.].
+000041e0: 7d01 7400 6400 8301 4400 5d09 7d02 6401  }.t.d...D.].}.d.
+000041f0: 7c02 9b00 7c01 9b00 9d03 9103 7108 7102  |...|.......q.q.
+00004200: 5300 2902 7253 0000 0072 8700 0000 2901  S.).rS...r....).
+00004210: da05 7261 6e67 6529 0372 3700 0000 da04  ..range).r7.....
+00004220: 706f 7374 7214 0000 0072 1600 0000 7216  postr....r....r.
+00004230: 0000 0072 1700 0000 725b 0000 00fe 0100  ...r....r[......
+00004240: 0073 0a00 0000 0600 0801 04ff 0e01 08ff  .s..............
+00004250: 7a35 426c 6f63 6b4d 6573 6844 6963 7452  z5BlockMeshDictR
+00004260: 6563 7469 6c69 6e65 6172 2e5f 5f69 6e69  ectilinear.__ini
+00004270: 745f 5f2e 3c6c 6f63 616c 733e 2e3c 6c69  t__.<locals>.<li
+00004280: 7374 636f 6d70 3e29 0272 c600 0000 72c7  stcomp>).r....r.
+00004290: 0000 0072 9f00 0000 2901 7212 0000 0029  ...r....).r....)
+000042a0: 0ada 0573 7570 6572 7218 0000 0072 7f00  ...superr....r..
+000042b0: 0000 720d 0000 0072 8200 0000 720f 0000  ..r....r....r...
+000042c0: 0072 1000 0000 7212 0000 0072 9e00 0000  .r....r....r....
+000042d0: da05 626c 6f63 6b29 0b72 1500 0000 da02  ..block).r......
+000042e0: 6c78 5a02 6c79 5a02 6c7a da02 6e78 da02  lxZ.lyZ.lz..nx..
+000042f0: 6e79 5a02 6e7a 727e 0000 005a 0662 6173  nyZ.nzr~...Z.bas
+00004300: 6576 7372 8700 0000 5a0c 7665 7274 6578  evsr....Z.vertex
+00004310: 5f6e 616d 6573 a901 da09 5f5f 636c 6173  _names....__clas
+00004320: 735f 5f72 1600 0000 7217 0000 0072 1800  s__r....r....r..
+00004330: 0000 ee01 0000 731c 0000 000a 010a 020c  ......s.........
+00004340: 030c 010c 010c 0104 fc08 071a 011c 0106  ................
+00004350: 0202 0106 ff1c 047a 2142 6c6f 636b 4d65  .......z!BlockMe
+00004360: 7368 4469 6374 5265 6374 696c 696e 6561  shDictRectilinea
+00004370: 722e 5f5f 696e 6974 5f5f 2905 722c 0000  r.__init__).r,..
+00004380: 0072 2d00 0000 722e 0000 0072 1800 0000  .r-...r....r....
+00004390: da0d 5f5f 636c 6173 7363 656c 6c5f 5f72  ..__classcell__r
+000043a0: 1600 0000 7216 0000 0072 cf00 0000 7217  ....r....r....r.
+000043b0: 0000 0072 c300 0000 ed01 0000 7304 0000  ...r........s...
+000043c0: 0008 0014 0172 c300 0000 4e29 17da 075f  .....r....N)..._
+000043d0: 5f64 6f63 5f5f da09 6974 6572 746f 6f6c  _doc__..itertool
+000043e0: 7372 0200 0000 da06 7374 7269 6e67 7203  sr......stringr.
+000043f0: 0000 0072 9f00 0000 7205 0000 0072 7200  ...r....r....rr.
+00004400: 0000 7207 0000 0072 0800 0000 7248 0000  ..r....r....rH..
+00004410: 0072 0900 0000 720a 0000 0072 0b00 0000  .r....r....r....
+00004420: 720c 0000 00da 075f 5f61 6c6c 5f5f 720d  r......__all__r.
+00004430: 0000 0072 3000 0000 7242 0000 0072 4600  ...r0...rB...rF.
+00004440: 0000 7268 0000 0072 6f00 0000 72c3 0000  ..rh...ro...r...
+00004450: 0072 1600 0000 7216 0000 0072 1600 0000  .r....r....r....
+00004460: 7217 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
+00004470: 0000 0073 2000 0000 0400 0c0c 0c01 0c02  ...s ...........
+00004480: 1001 1801 0802 0e0a 0e22 0e11 0e09 0e57  .........".....W
+00004490: 0e28 007f 007f 1416                      .(......
```

### Comparing `fluidsimfoam-0.0.5/src/fluidsimfoam/foam_input_files/blockmesh/__pycache__/edges.cpython-39.pyc` & `fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/blockmesh/__pycache__/edges.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Fri May  5 08:40:03 2023 UTC, .py size: 1810 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 18% similar despite different names*

```diff
@@ -1,152 +1,188 @@
-00000000: 610d 0d0a 0000 0000 e3c0 5464 1207 0000  a.........Td....
+00000000: 6f0d 0d0a 0000 0000 2b36 7e64 4c08 0000  o.......+6~dL...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0003 0000 0040 0000 0073 2000 0000 4700  .....@...s ...G.
+00000020: 0003 0000 0040 0000 0073 2e00 0000 4700  .....@...s....G.
 00000030: 6400 6401 8400 6401 8302 5a00 4700 6402  d.d...d...Z.G.d.
-00000040: 6403 8400 6403 8302 5a01 6404 5300 2905  d...d...Z.d.S.).
-00000050: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-00000060: 0002 0000 0040 0000 0073 1c00 0000 6500  .....@...s....e.
-00000070: 5a01 6400 5a02 6401 6402 8400 5a03 6403  Z.d.Z.d.d...Z.d.
-00000080: 6404 8400 5a04 6405 5300 2906 da07 4172  d...Z.d.S.)...Ar
-00000090: 6345 6467 6563 0400 0000 0000 0000 0000  cEdgec..........
-000000a0: 0000 0400 0000 0200 0000 4300 0000 7316  ..........C...s.
-000000b0: 0000 007c 017c 005f 007c 027c 005f 017c  ...|.|._.|.|._.|
-000000c0: 037c 005f 0264 0153 0029 0261 5401 0000  .|._.d.S.).aT...
-000000d0: 496e 6974 6961 6c69 7a65 2041 7263 4564  Initialize ArcEd
-000000e0: 6765 2069 6e73 7461 6e63 650a 2020 2020  ge instance.    
-000000f0: 2020 2020 766e 616d 6573 2069 7320 7468      vnames is th
-00000100: 6520 7665 7274 6578 206e 616d 6573 2069  e vertex names i
-00000110: 6e20 6f72 6465 7220 6465 7363 7269 7665  n order descrive
-00000120: 6420 696e 0a20 2020 2020 2020 2020 2068  d in.          h
-00000130: 7474 703a 2f2f 7777 772e 6f70 656e 666f  ttp://www.openfo
-00000140: 616d 2e6f 7267 2f64 6f63 732f 7573 6572  am.org/docs/user
-00000150: 2f6d 6573 682d 6465 7363 7269 7074 696f  /mesh-descriptio
-00000160: 6e2e 7068 700a 2020 2020 2020 2020 2320  n.php.        # 
-00000170: 7477 6f20 7665 7274 6963 6573 2069 7320  two vertices is 
-00000180: 6e65 6564 6564 2066 6f72 2041 7263 0a20  needed for Arc. 
-00000190: 2020 2020 2020 2063 656c 6c73 2069 7320         cells is 
-000001a0: 6e75 6d62 6572 206f 6620 6365 6c6c 7320  number of cells 
-000001b0: 6465 7669 6564 2069 6e74 6f20 696e 2065  devied into in e
-000001c0: 6163 6820 6469 7265 6374 696f 6e0a 2020  ach direction.  
-000001d0: 2020 2020 2020 6e61 6d65 2069 7320 7468        name is th
-000001e0: 6520 756e 6971 206e 616d 6520 6f66 2074  e uniq name of t
-000001f0: 6865 2062 6c6f 636b 0a20 2020 2020 2020  he block.       
-00000200: 2067 7261 6469 6e67 2069 7320 6772 6164   grading is grad
-00000210: 696e 6720 6d65 7468 6f64 2e0a 2020 2020  ing method..    
-00000220: 2020 2020 4e29 03da 0676 6e61 6d65 73da      N)...vnames.
-00000230: 046e 616d 65da 0c69 6e74 6572 5f76 6572  .name..inter_ver
-00000240: 7465 7829 04da 0473 656c 6672 0200 0000  tex)...selfr....
-00000250: 7203 0000 0072 0400 0000 a900 7206 0000  r....r......r...
-00000260: 00fa 5b2f 686f 6d65 2f75 7365 7273 2f61  ..[/home/users/a
-00000270: 7567 6965 7233 7069 2f44 6576 2f66 6c75  ugier3pi/Dev/flu
-00000280: 6964 7369 6d66 6f61 6d2f 7372 632f 666c  idsimfoam/src/fl
-00000290: 7569 6473 696d 666f 616d 2f66 6f61 6d5f  uidsimfoam/foam_
-000002a0: 696e 7075 745f 6669 6c65 732f 626c 6f63  input_files/bloc
-000002b0: 6b6d 6573 682f 6564 6765 732e 7079 da08  kmesh/edges.py..
-000002c0: 5f5f 696e 6974 5f5f 0200 0000 7306 0000  __init__....s...
-000002d0: 0000 0906 0106 017a 1041 7263 4564 6765  .......z.ArcEdge
-000002e0: 2e5f 5f69 6e69 745f 5f63 0200 0000 0000  .__init__c......
-000002f0: 0000 0000 0000 0500 0000 0d00 0000 0300  ................
-00000300: 0000 7364 0000 0064 01a0 0087 0066 0164  ..sd...d.....f.d
-00000310: 0264 0384 087c 006a 0144 0083 01a1 017d  .d...|.j.D.....}
-00000320: 0264 01a0 007c 006a 01a1 017d 037c 006a  .d...|.j...}.|.j
-00000330: 027d 0464 047c 029b 0064 057c 046a 0364  .}.d.|...d.|.j.d
-00000340: 069b 0464 017c 046a 0464 069b 0464 017c  ...d.|.j.d...d.|
-00000350: 046a 0564 069b 0464 077c 006a 069b 0064  .j.d...d.|.j...d
-00000360: 057c 039b 0064 089d 0d53 0029 09fa 4b46  .|...d...S.)..KF
-00000370: 6f72 6d61 7420 696e 7374 616e 6365 2074  ormat instance t
-00000380: 6f20 6475 6d70 0a20 2020 2020 2020 2076  o dump.        v
-00000390: 6572 7469 6365 7320 6973 2064 6963 7420  ertices is dict 
-000003a0: 6f66 206e 616d 6520 746f 2056 6572 7465  of name to Verte
-000003b0: 780a 2020 2020 2020 2020 fa01 2063 0100  x.        .. c..
-000003c0: 0000 0000 0000 0000 0000 0200 0000 0400  ................
-000003d0: 0000 3300 0000 731c 0000 007c 005d 147d  ..3...s....|.].}
-000003e0: 0174 0088 007c 0119 006a 0183 0156 0001  .t...|...j...V..
-000003f0: 0071 0264 0053 00a9 014e a902 da03 7374  .q.d.S...N....st
-00000400: 72da 0569 6e64 6578 a902 da02 2e30 da02  r..index.....0..
-00000410: 766e a901 da08 7665 7274 6963 6573 7206  vn....verticesr.
-00000420: 0000 0072 0700 0000 da09 3c67 656e 6578  ...r......<genex
-00000430: 7072 3e13 0000 00f3 0000 0000 7a21 4172  pr>.........z!Ar
-00000440: 6345 6467 652e 666f 726d 6174 2e3c 6c6f  cEdge.format.<lo
-00000450: 6361 6c73 3e2e 3c67 656e 6578 7072 3e7a  cals>.<genexpr>z
-00000460: 0461 7263 20fa 0220 287a 0631 382e 3135  .arc .. (z.18.15
-00000470: 677a 0529 202f 2f20 fa01 2929 07da 046a  gz.) // ..))...j
-00000480: 6f69 6e72 0200 0000 7204 0000 00da 0178  oinr....r......x
-00000490: da01 79da 017a 7203 0000 0029 0572 0500  ..y..zr....).r..
-000004a0: 0000 7213 0000 0072 0e00 0000 da07 636f  ..r....r......co
-000004b0: 6d6d 656e 74da 0176 7206 0000 0072 1200  mment..vr....r..
-000004c0: 0000 7207 0000 00da 0666 6f72 6d61 740f  ..r......format.
-000004d0: 0000 0073 1200 0000 0004 1a01 0c01 0602  ...s............
-000004e0: 2601 04ff 0401 02ff 06ff 7a0e 4172 6345  &.........z.ArcE
-000004f0: 6467 652e 666f 726d 6174 4ea9 05da 085f  dge.formatN...._
-00000500: 5f6e 616d 655f 5fda 0a5f 5f6d 6f64 756c  _name__..__modul
-00000510: 655f 5fda 0c5f 5f71 7561 6c6e 616d 655f  e__..__qualname_
-00000520: 5f72 0800 0000 721e 0000 0072 0600 0000  _r....r....r....
-00000530: 7206 0000 0072 0600 0000 7207 0000 0072  r....r....r....r
-00000540: 0100 0000 0100 0000 7304 0000 0008 0108  ........s.......
-00000550: 0d72 0100 0000 6300 0000 0000 0000 0000  .r....c.........
-00000560: 0000 0000 0000 0002 0000 0040 0000 0073  ...........@...s
-00000570: 1c00 0000 6500 5a01 6400 5a02 6401 6402  ....e.Z.d.Z.d.d.
-00000580: 8400 5a03 6403 6404 8400 5a04 6405 5300  ..Z.d.d...Z.d.S.
-00000590: 2906 da0a 5370 6c69 6e65 4564 6765 6304  )...SplineEdgec.
-000005a0: 0000 0000 0000 0000 0000 0004 0000 0002  ................
-000005b0: 0000 0043 0000 0073 1600 0000 7c01 7c00  ...C...s....|.|.
-000005c0: 5f00 7c02 7c00 5f01 7c03 7c00 5f02 6401  _.|.|._.|.|._.d.
-000005d0: 5300 2902 7acd 496e 6974 6961 6c69 7a65  S.).z.Initialize
-000005e0: 2053 706c 696e 6545 6467 6520 696e 7374   SplineEdge inst
-000005f0: 616e 6365 0a20 2020 2020 2020 2076 6e61  ance.        vna
-00000600: 6d65 7320 6973 2074 6865 2076 6572 7465  mes is the verte
-00000610: 7820 6e61 6d65 7320 696e 206f 7264 6572  x names in order
-00000620: 2064 6573 6372 6976 6564 2069 6e0a 2020   descrived in.  
-00000630: 2020 2020 2020 2020 6874 7470 3a2f 2f77          http://w
-00000640: 7777 2e6f 7065 6e66 6f61 6d2e 6f72 672f  ww.openfoam.org/
-00000650: 646f 6373 2f75 7365 722f 6d65 7368 2d64  docs/user/mesh-d
-00000660: 6573 6372 6970 7469 6f6e 2e70 6870 0a20  escription.php. 
-00000670: 2020 2020 2020 2023 2074 776f 2076 6572         # two ver
-00000680: 7469 6365 7320 6973 206e 6565 6465 6420  tices is needed 
-00000690: 666f 7220 5370 6c69 6e65 0a20 2020 2020  for Spline.     
-000006a0: 2020 204e 2903 7202 0000 0072 0300 0000     N).r....r....
-000006b0: da06 706f 696e 7473 2904 7205 0000 0072  ..points).r....r
-000006c0: 0200 0000 7203 0000 0072 2400 0000 7206  ....r....r$...r.
-000006d0: 0000 0072 0600 0000 7207 0000 0072 0800  ...r....r....r..
-000006e0: 0000 1d00 0000 7306 0000 0000 0606 0106  ......s.........
-000006f0: 017a 1353 706c 696e 6545 6467 652e 5f5f  .z.SplineEdge.__
-00000700: 696e 6974 5f5f 6302 0000 0000 0000 0000  init__c.........
-00000710: 0000 0006 0000 0009 0000 0003 0000 0073  ...............s
-00000720: 8600 0000 6401 a000 8700 6601 6402 6403  ....d.....f.d.d.
-00000730: 8408 7c00 6a01 4400 8301 a101 7d02 6401  ..|.j.D.....}.d.
-00000740: a000 7c00 6a01 a101 7d03 6700 7d04 7c04  ..|.j...}.g.}.|.
-00000750: a002 6404 7c02 9b00 6405 7c00 6a03 9b00  ..d.|...d.|.j...
-00000760: 6406 7c03 9b00 6407 9d07 a101 0100 7c04  d.|...d.......|.
-00000770: a002 6408 a101 0100 7c00 6a04 4400 5d16  ..d.....|.j.D.].
-00000780: 7d05 7c04 a002 6409 7c05 a005 a100 1700  }.|...d.|.......
-00000790: a101 0100 715a 7c04 a002 6407 a101 0100  ....qZ|...d.....
-000007a0: 640a a000 7c04 a101 5300 290b 7209 0000  d...|...S.).r...
-000007b0: 0072 0a00 0000 6301 0000 0000 0000 0000  .r....c.........
-000007c0: 0000 0002 0000 0004 0000 0033 0000 0073  ...........3...s
-000007d0: 1c00 0000 7c00 5d14 7d01 7400 8800 7c01  ....|.].}.t...|.
-000007e0: 1900 6a01 8301 5600 0100 7102 6400 5300  ..j...V...q.d.S.
-000007f0: 720b 0000 0072 0c00 0000 720f 0000 0072  r....r....r....r
-00000800: 1200 0000 7206 0000 0072 0700 0000 7214  ....r....r....r.
-00000810: 0000 002b 0000 0072 1500 0000 7a24 5370  ...+...r....z$Sp
-00000820: 6c69 6e65 4564 6765 2e66 6f72 6d61 742e  lineEdge.format.
-00000830: 3c6c 6f63 616c 733e 2e3c 6765 6e65 7870  <locals>.<genexp
-00000840: 723e 7a07 7370 6c69 6e65 207a 1920 2020  r>z.spline z.   
-00000850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000860: 2020 202f 2f20 7216 0000 0072 1700 0000     // r....r....
-00000870: 7a05 2020 2020 287a 0920 2020 2020 2020  z.    (z.       
-00000880: 2020 da01 0a29 0672 1800 0000 7202 0000    ...).r....r...
-00000890: 00da 0661 7070 656e 6472 0300 0000 7224  ...appendr....r$
-000008a0: 0000 0072 1e00 0000 2906 7205 0000 0072  ...r....).r....r
-000008b0: 1300 0000 720e 0000 0072 1c00 0000 da03  ....r....r......
-000008c0: 746d 70da 0170 7206 0000 0072 1200 0000  tmp..pr....r....
-000008d0: 7207 0000 0072 1e00 0000 2700 0000 7316  r....r....'...s.
-000008e0: 0000 0000 041a 010c 0104 0104 0118 ff04  ................
-000008f0: 030a 010a 0114 010a 017a 1153 706c 696e  .........z.Splin
-00000900: 6545 6467 652e 666f 726d 6174 4e72 1f00  eEdge.formatNr..
-00000910: 0000 7206 0000 0072 0600 0000 7206 0000  ..r....r....r...
-00000920: 0072 0700 0000 7223 0000 001c 0000 0073  .r....r#.......s
-00000930: 0400 0000 0801 080a 7223 0000 004e 2902  ........r#...N).
-00000940: 7201 0000 0072 2300 0000 7206 0000 0072  r....r#...r....r
-00000950: 0600 0000 7206 0000 0072 0700 0000 da08  ....r....r......
-00000960: 3c6d 6f64 756c 653e 0100 0000 7302 0000  <module>....s...
-00000970: 000e 1b                                  ...
+00000040: 6403 8400 6403 8302 5a01 4700 6404 6405  d...d...Z.G.d.d.
+00000050: 8400 6405 8302 5a02 6406 5300 2907 6300  ..d...Z.d.S.).c.
+00000060: 0000 0000 0000 0000 0000 0000 0000 0002  ................
+00000070: 0000 0040 0000 00f3 1c00 0000 6500 5a01  ...@........e.Z.
+00000080: 6400 5a02 6401 6402 8400 5a03 6403 6404  d.Z.d.d...Z.d.d.
+00000090: 8400 5a04 6405 5300 2906 da05 506f 696e  ..Z.d.S.)...Poin
+000000a0: 7463 0400 0000 0000 0000 0000 0000 0400  tc..............
+000000b0: 0000 0200 0000 4300 0000 7316 0000 007c  ......C...s....|
+000000c0: 017c 005f 007c 027c 005f 017c 037c 005f  .|._.|.|._.|.|._
+000000d0: 0264 0053 00a9 014e a903 da01 78da 0179  .d.S...N....x..y
+000000e0: da01 7a29 04da 0473 656c 6672 0500 0000  ..z)...selfr....
+000000f0: 7206 0000 0072 0700 0000 a900 7209 0000  r....r......r...
+00000100: 00fa 522f 686f 6d65 2f70 6965 7272 652f  ..R/home/pierre/
+00000110: 4465 762f 666c 7569 6473 696d 666f 616d  Dev/fluidsimfoam
+00000120: 2f73 7263 2f66 6c75 6964 7369 6d66 6f61  /src/fluidsimfoa
+00000130: 6d2f 666f 616d 5f69 6e70 7574 5f66 696c  m/foam_input_fil
+00000140: 6573 2f62 6c6f 636b 6d65 7368 2f65 6467  es/blockmesh/edg
+00000150: 6573 2e70 79da 085f 5f69 6e69 745f 5f02  es.py..__init__.
+00000160: 0000 0073 0600 0000 0601 0601 0a01 7a0e  ...s..........z.
+00000170: 506f 696e 742e 5f5f 696e 6974 5f5f 6301  Point.__init__c.
+00000180: 0000 0000 0000 0000 0000 0001 0000 0007  ................
+00000190: 0000 0043 0000 0073 2400 0000 6401 7c00  ...C...s$...d.|.
+000001a0: 6a00 6402 9b04 6403 7c00 6a01 6402 9b04  j.d...d.|.j.d...
+000001b0: 6403 7c00 6a02 6402 9b04 6404 9d07 5300  d.|.j.d...d...S.
+000001c0: 2905 4e7a 0228 20fa 0631 382e 3135 67da  ).Nz.( ..18.15g.
+000001d0: 0120 7a02 2029 7204 0000 0029 0172 0800  . z. )r....).r..
+000001e0: 0000 7209 0000 0072 0900 0000 720a 0000  ..r....r....r...
+000001f0: 00da 0666 6f72 6d61 7407 0000 0073 0200  ...format....s..
+00000200: 0000 2401 7a0c 506f 696e 742e 666f 726d  ..$.z.Point.form
+00000210: 6174 4ea9 05da 085f 5f6e 616d 655f 5fda  atN....__name__.
+00000220: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
+00000230: 7561 6c6e 616d 655f 5f72 0b00 0000 720e  ualname__r....r.
+00000240: 0000 0072 0900 0000 7209 0000 0072 0900  ...r....r....r..
+00000250: 0000 720a 0000 0072 0200 0000 0100 0000  ..r....r........
+00000260: 7306 0000 0008 0008 010c 0572 0200 0000  s..........r....
+00000270: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+00000280: 0002 0000 0040 0000 0072 0100 0000 2906  .....@...r....).
+00000290: da07 4172 6345 6467 6563 0400 0000 0000  ..ArcEdgec......
+000002a0: 0000 0000 0000 0400 0000 0200 0000 4300  ..............C.
+000002b0: 0000 7316 0000 007c 017c 005f 007c 027c  ..s....|.|._.|.|
+000002c0: 005f 017c 037c 005f 0264 0153 0029 0261  ._.|.|._.d.S.).a
+000002d0: 5401 0000 496e 6974 6961 6c69 7a65 2041  T...Initialize A
+000002e0: 7263 4564 6765 2069 6e73 7461 6e63 650a  rcEdge instance.
+000002f0: 2020 2020 2020 2020 766e 616d 6573 2069          vnames i
+00000300: 7320 7468 6520 7665 7274 6578 206e 616d  s the vertex nam
+00000310: 6573 2069 6e20 6f72 6465 7220 6465 7363  es in order desc
+00000320: 7269 7665 6420 696e 0a20 2020 2020 2020  rived in.       
+00000330: 2020 2068 7474 703a 2f2f 7777 772e 6f70     http://www.op
+00000340: 656e 666f 616d 2e6f 7267 2f64 6f63 732f  enfoam.org/docs/
+00000350: 7573 6572 2f6d 6573 682d 6465 7363 7269  user/mesh-descri
+00000360: 7074 696f 6e2e 7068 700a 2020 2020 2020  ption.php.      
+00000370: 2020 2320 7477 6f20 7665 7274 6963 6573    # two vertices
+00000380: 2069 7320 6e65 6564 6564 2066 6f72 2041   is needed for A
+00000390: 7263 0a20 2020 2020 2020 2063 656c 6c73  rc.        cells
+000003a0: 2069 7320 6e75 6d62 6572 206f 6620 6365   is number of ce
+000003b0: 6c6c 7320 6465 7669 6564 2069 6e74 6f20  lls devied into 
+000003c0: 696e 2065 6163 6820 6469 7265 6374 696f  in each directio
+000003d0: 6e0a 2020 2020 2020 2020 6e61 6d65 2069  n.        name i
+000003e0: 7320 7468 6520 756e 6971 206e 616d 6520  s the uniq name 
+000003f0: 6f66 2074 6865 2062 6c6f 636b 0a20 2020  of the block.   
+00000400: 2020 2020 2067 7261 6469 6e67 2069 7320       grading is 
+00000410: 6772 6164 696e 6720 6d65 7468 6f64 2e0a  grading method..
+00000420: 2020 2020 2020 2020 4e29 03da 0676 6e61          N)...vna
+00000430: 6d65 73da 046e 616d 65da 0c69 6e74 6572  mes..name..inter
+00000440: 5f76 6572 7465 7829 0472 0800 0000 7214  _vertex).r....r.
+00000450: 0000 0072 1500 0000 7216 0000 0072 0900  ...r....r....r..
+00000460: 0000 7209 0000 0072 0a00 0000 720b 0000  ..r....r....r...
+00000470: 000c 0000 0073 0600 0000 0609 0601 0a01  .....s..........
+00000480: 7a10 4172 6345 6467 652e 5f5f 696e 6974  z.ArcEdge.__init
+00000490: 5f5f 6302 0000 0000 0000 0000 0000 0005  __c.............
+000004a0: 0000 000d 0000 0003 0000 0073 6400 0000  ...........sd...
+000004b0: 6401 a000 8700 6601 6402 6403 8408 7c00  d.....f.d.d...|.
+000004c0: 6a01 4400 8301 a101 7d02 6401 a000 7c00  j.D.....}.d...|.
+000004d0: 6a01 a101 7d03 7c00 6a02 7d04 6404 7c02  j...}.|.j.}.d.|.
+000004e0: 9b00 6405 7c04 6a03 6406 9b04 6401 7c04  ..d.|.j.d...d.|.
+000004f0: 6a04 6406 9b04 6401 7c04 6a05 6406 9b04  j.d...d.|.j.d...
+00000500: 6407 7c00 6a06 9b00 6405 7c03 9b00 6408  d.|.j...d.|...d.
+00000510: 9d0d 5300 2909 fa4b 466f 726d 6174 2069  ..S.)..KFormat i
+00000520: 6e73 7461 6e63 6520 746f 2064 756d 700a  nstance to dump.
+00000530: 2020 2020 2020 2020 7665 7274 6963 6573          vertices
+00000540: 2069 7320 6469 6374 206f 6620 6e61 6d65   is dict of name
+00000550: 2074 6f20 5665 7274 6578 0a20 2020 2020   to Vertex.     
+00000560: 2020 2072 0d00 0000 6301 0000 0000 0000     r....c.......
+00000570: 0000 0000 0002 0000 0004 0000 0033 0000  .............3..
+00000580: 00f3 1e00 0000 8100 7c00 5d0a 7d01 7400  ........|.].}.t.
+00000590: 8800 7c01 1900 6a01 8301 5600 0100 7102  ..|...j...V...q.
+000005a0: 6400 5300 7203 0000 00a9 02da 0373 7472  d.S.r........str
+000005b0: da05 696e 6465 78a9 02da 022e 30da 0276  ..index.....0..v
+000005c0: 6ea9 01da 0876 6572 7469 6365 7372 0900  n....verticesr..
+000005d0: 0000 720a 0000 00da 093c 6765 6e65 7870  ..r......<genexp
+000005e0: 723e 1d00 0000 f304 0000 0002 801c 007a  r>.............z
+000005f0: 2141 7263 4564 6765 2e66 6f72 6d61 742e  !ArcEdge.format.
+00000600: 3c6c 6f63 616c 733e 2e3c 6765 6e65 7870  <locals>.<genexp
+00000610: 723e 7a04 6172 6320 fa02 2028 720c 0000  r>z.arc .. (r...
+00000620: 007a 0529 202f 2f20 fa01 2929 07da 046a  .z.) // ..))...j
+00000630: 6f69 6e72 1400 0000 7216 0000 0072 0500  oinr....r....r..
+00000640: 0000 7206 0000 0072 0700 0000 7215 0000  ..r....r....r...
+00000650: 0029 0572 0800 0000 7220 0000 0072 1b00  .).r....r ...r..
+00000660: 0000 da07 636f 6d6d 656e 74da 0176 7209  ....comment..vr.
+00000670: 0000 0072 1f00 0000 720a 0000 0072 0e00  ...r....r....r..
+00000680: 0000 1900 0000 7312 0000 001a 040c 0106  ......s.........
+00000690: 0126 0204 0104 ff02 0106 ff02 ff7a 0e41  .&...........z.A
+000006a0: 7263 4564 6765 2e66 6f72 6d61 744e 720f  rcEdge.formatNr.
+000006b0: 0000 0072 0900 0000 7209 0000 0072 0900  ...r....r....r..
+000006c0: 0000 720a 0000 0072 1300 0000 0b00 0000  ..r....r........
+000006d0: 7306 0000 0008 0008 010c 0d72 1300 0000  s..........r....
+000006e0: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+000006f0: 0002 0000 0040 0000 0072 0100 0000 2906  .....@...r....).
+00000700: da0a 5370 6c69 6e65 4564 6765 6304 0000  ..SplineEdgec...
+00000710: 0000 0000 0000 0000 0004 0000 0003 0000  ................
+00000720: 0043 0000 0073 3600 0000 7c01 7c00 5f00  .C...s6...|.|._.
+00000730: 7c02 7c00 5f01 7c03 7216 7402 7c03 6401  |.|._.|.r.t.|.d.
+00000740: 1900 7403 8302 7316 6402 6403 8400 7c03  ..t...s.d.d...|.
+00000750: 4400 8301 7d03 7c03 7c00 5f04 6404 5300  D...}.|.|._.d.S.
+00000760: 2905 7acd 496e 6974 6961 6c69 7a65 2053  ).z.Initialize S
+00000770: 706c 696e 6545 6467 6520 696e 7374 616e  plineEdge instan
+00000780: 6365 0a20 2020 2020 2020 2076 6e61 6d65  ce.        vname
+00000790: 7320 6973 2074 6865 2076 6572 7465 7820  s is the vertex 
+000007a0: 6e61 6d65 7320 696e 206f 7264 6572 2064  names in order d
+000007b0: 6573 6372 6976 6564 2069 6e0a 2020 2020  escrived in.    
+000007c0: 2020 2020 2020 6874 7470 3a2f 2f77 7777        http://www
+000007d0: 2e6f 7065 6e66 6f61 6d2e 6f72 672f 646f  .openfoam.org/do
+000007e0: 6373 2f75 7365 722f 6d65 7368 2d64 6573  cs/user/mesh-des
+000007f0: 6372 6970 7469 6f6e 2e70 6870 0a20 2020  cription.php.   
+00000800: 2020 2020 2023 2074 776f 2076 6572 7469       # two verti
+00000810: 6365 7320 6973 206e 6565 6465 6420 666f  ces is needed fo
+00000820: 7220 5370 6c69 6e65 0a20 2020 2020 2020  r Spline.       
+00000830: 20e9 0000 0000 6301 0000 0000 0000 0000   .....c.........
+00000840: 0000 0004 0000 0006 0000 0053 0000 0073  ...........S...s
+00000850: 1e00 0000 6700 7c00 5d0b 5c03 7d01 7d02  ....g.|.].\.}.}.
+00000860: 7d03 7400 7c01 7c02 7c03 8303 9102 7102  }.t.|.|.|.....q.
+00000870: 5300 7209 0000 0029 0172 0200 0000 2904  S.r....).r....).
+00000880: 721d 0000 0072 0500 0000 7206 0000 0072  r....r....r....r
+00000890: 0700 0000 7209 0000 0072 0900 0000 720a  ....r....r....r.
+000008a0: 0000 00da 0a3c 6c69 7374 636f 6d70 3e30  .....<listcomp>0
+000008b0: 0000 0073 0200 0000 1e00 7a27 5370 6c69  ...s......z'Spli
+000008c0: 6e65 4564 6765 2e5f 5f69 6e69 745f 5f2e  neEdge.__init__.
+000008d0: 3c6c 6f63 616c 733e 2e3c 6c69 7374 636f  <locals>.<listco
+000008e0: 6d70 3e4e 2905 7214 0000 0072 1500 0000  mp>N).r....r....
+000008f0: da0a 6973 696e 7374 616e 6365 7202 0000  ..isinstancer...
+00000900: 00da 0670 6f69 6e74 7329 0472 0800 0000  ...points).r....
+00000910: 7214 0000 0072 1500 0000 722c 0000 0072  r....r....r,...r
+00000920: 0900 0000 7209 0000 0072 0a00 0000 720b  ....r....r....r.
+00000930: 0000 0027 0000 0073 0a00 0000 0606 0601  ...'...s........
+00000940: 1201 0e01 0a01 7a13 5370 6c69 6e65 4564  ......z.SplineEd
+00000950: 6765 2e5f 5f69 6e69 745f 5f63 0200 0000  ge.__init__c....
+00000960: 0000 0000 0000 0000 0600 0000 0900 0000  ................
+00000970: 0300 0000 7386 0000 0064 01a0 0087 0066  ....s....d.....f
+00000980: 0164 0264 0384 087c 006a 0144 0083 01a1  .d.d...|.j.D....
+00000990: 017d 0264 01a0 007c 006a 01a1 017d 0367  .}.d...|.j...}.g
+000009a0: 007d 047c 04a0 0264 047c 029b 0064 057c  .}.|...d.|...d.|
+000009b0: 006a 039b 0064 067c 039b 0064 079d 07a1  .j...d.|...d....
+000009c0: 0101 007c 04a0 0264 08a1 0101 007c 006a  ...|...d.....|.j
+000009d0: 0444 005d 0b7d 057c 04a0 0264 097c 05a0  .D.].}.|...d.|..
+000009e0: 05a1 0017 00a1 0101 0071 2d7c 04a0 0264  .........q-|...d
+000009f0: 07a1 0101 0064 0aa0 007c 04a1 0153 0029  .....d...|...S.)
+00000a00: 0b72 1700 0000 720d 0000 0063 0100 0000  .r....r....c....
+00000a10: 0000 0000 0000 0000 0200 0000 0400 0000  ................
+00000a20: 3300 0000 7218 0000 0072 0300 0000 7219  3...r....r....r.
+00000a30: 0000 0072 1c00 0000 721f 0000 0072 0900  ...r....r....r..
+00000a40: 0000 720a 0000 0072 2100 0000 3700 0000  ..r....r!...7...
+00000a50: 7222 0000 007a 2453 706c 696e 6545 6467  r"...z$SplineEdg
+00000a60: 652e 666f 726d 6174 2e3c 6c6f 6361 6c73  e.format.<locals
+00000a70: 3e2e 3c67 656e 6578 7072 3e7a 0773 706c  >.<genexpr>z.spl
+00000a80: 696e 6520 7a19 2020 2020 2020 2020 2020  ine z.          
+00000a90: 2020 2020 2020 2020 2020 2020 2f2f 2072              // r
+00000aa0: 2300 0000 7224 0000 007a 0520 2020 2028  #...r$...z.    (
+00000ab0: 7a09 2020 2020 2020 2020 20da 010a 2906  z.         ...).
+00000ac0: 7225 0000 0072 1400 0000 da06 6170 7065  r%...r......appe
+00000ad0: 6e64 7215 0000 0072 2c00 0000 720e 0000  ndr....r,...r...
+00000ae0: 0029 0672 0800 0000 7220 0000 0072 1b00  .).r....r ...r..
+00000af0: 0000 7226 0000 00da 0374 6d70 da01 7072  ..r&.....tmp..pr
+00000b00: 0900 0000 721f 0000 0072 0a00 0000 720e  ....r....r....r.
+00000b10: 0000 0033 0000 0073 1600 0000 1a04 0c01  ...3...s........
+00000b20: 0401 0401 1801 04ff 0a03 0a01 1401 0a01  ................
+00000b30: 0a01 7a11 5370 6c69 6e65 4564 6765 2e66  ..z.SplineEdge.f
+00000b40: 6f72 6d61 744e 720f 0000 0072 0900 0000  ormatNr....r....
+00000b50: 7209 0000 0072 0900 0000 720a 0000 0072  r....r....r....r
+00000b60: 2800 0000 2600 0000 7306 0000 0008 0008  (...&...s.......
+00000b70: 010c 0c72 2800 0000 4e29 0372 0200 0000  ...r(...N).r....
+00000b80: 7213 0000 0072 2800 0000 7209 0000 0072  r....r(...r....r
+00000b90: 0900 0000 7209 0000 0072 0a00 0000 da08  ....r....r......
+00000ba0: 3c6d 6f64 756c 653e 0100 0000 7306 0000  <module>....s...
+00000bb0: 000e 000e 0a12 1b                        .......
```

### Comparing `fluidsimfoam-0.0.5/src/fluidsimfoam/foam_input_files/blockmesh/__pycache__/grading.cpython-310.pyc` & `fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/blockmesh/__pycache__/grading.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri May  5 08:40:03 2023 UTC, .py size: 3426 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 e3c0 5464 620d 0000  o.........Tdb...
+00000000: 6f0d 0d0a 0000 0000 68ed 4664 620d 0000  o.......h.Fdb...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 5800 0000 6400  .....@...sX...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 4700 6403 6404 8400 6404  m.Z...G.d.d...d.
 00000050: 8302 5a04 4700 6405 6406 8400 6406 8302  ..Z.G.d.d...d...
 00000060: 5a05 4700 6407 6408 8400 6408 6504 8303  Z.G.d.d...d.e...
 00000070: 5a06 4700 6409 640a 8400 640a 6504 8303  Z.G.d.d...d.e...
@@ -14,181 +14,180 @@
 000000d0: 5300 2903 da07 4772 6164 696e 677a 2862  S.)...Gradingz(b
 000000e0: 6173 6520 636c 6173 7320 666f 7220 5369  ase class for Si
 000000f0: 6d70 6c65 2d20 616e 6420 4564 6765 2d20  mple- and Edge- 
 00000100: 4772 6164 696e 674e 2904 da08 5f5f 6e61  GradingN)...__na
 00000110: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
 00000120: da0c 5f5f 7175 616c 6e61 6d65 5f5f da07  ..__qualname__..
 00000130: 5f5f 646f 635f 5fa9 0072 0900 0000 7209  __doc__..r....r.
-00000140: 0000 00fa 5d2f 686f 6d65 2f75 7365 7273  ....]/home/users
-00000150: 2f61 7567 6965 7233 7069 2f44 6576 2f66  /augier3pi/Dev/f
-00000160: 6c75 6964 7369 6d66 6f61 6d2f 7372 632f  luidsimfoam/src/
-00000170: 666c 7569 6473 696d 666f 616d 2f66 6f61  fluidsimfoam/foa
-00000180: 6d5f 696e 7075 745f 6669 6c65 732f 626c  m_input_files/bl
-00000190: 6f63 6b6d 6573 682f 6772 6164 696e 672e  ockmesh/grading.
-000001a0: 7079 7204 0000 0005 0000 0073 0400 0000  pyr........s....
-000001b0: 0800 0801 7204 0000 0063 0000 0000 0000  ....r....c......
-000001c0: 0000 0000 0000 0000 0000 0200 0000 4000  ..............@.
-000001d0: 0000 f320 0000 0065 005a 0164 005a 0264  ... ...e.Z.d.Z.d
-000001e0: 015a 0364 0264 0384 005a 0464 0464 0584  .Z.d.d...Z.d.d..
-000001f0: 005a 0564 0653 0029 07da 1453 696d 706c  .Z.d.S.)...Simpl
-00000200: 6547 7261 6469 6e67 456c 656d 656e 747a  eGradingElementz
-00000210: 3c78 2c20 7920 6f72 207a 2045 6c65 6d65  <x, y or z Eleme
-00000220: 6e74 206f 6620 7369 6d70 6c65 4772 6164  nt of simpleGrad
-00000230: 696e 672e 2061 646f 7074 6564 2074 6f20  ing. adopted to 
-00000240: 6d75 6c74 692d 6772 6164 696e 6763 0200  multi-gradingc..
-00000250: 0000 0000 0000 0000 0000 0200 0000 0200  ................
-00000260: 0000 4300 0000 730a 0000 007c 017c 005f  ..C...s....|.|._
-00000270: 0064 0153 0029 027a 9b69 6e69 7469 616c  .d.S.).z.initial
-00000280: 697a 6174 696f 6e0a 2020 2020 2020 2020  ization.        
-00000290: 6420 6973 2073 696e 676c 6520 6e75 6d62  d is single numb
-000002a0: 6572 2066 6f72 2065 7870 616e 7369 6f6e  er for expansion
-000002b0: 2072 6174 696f 0a20 2020 2020 2020 2020   ratio.         
-000002c0: 206f 7220 6974 6572 6174 6976 6520 6f62   or iterative ob
-000002d0: 6a65 6374 2063 6f6e 7369 7473 2028 6469  ject consits (di
-000002e0: 7265 6374 696f 6e20 7261 7469 6f2c 2063  rection ratio, c
-000002f0: 656c 6c20 7261 7469 6f2c 2065 7870 616e  ell ratio, expan
-00000300: 7369 6f6e 2072 6174 696f 290a 2020 2020  sion ratio).    
-00000310: 2020 2020 4e29 01da 0164 2902 da04 7365      N)...d)...se
-00000320: 6c66 720d 0000 0072 0900 0000 7209 0000  lfr....r....r...
-00000330: 0072 0a00 0000 da08 5f5f 696e 6974 5f5f  .r......__init__
-00000340: 0c00 0000 7302 0000 000a 057a 1d53 696d  ....s......z.Sim
-00000350: 706c 6547 7261 6469 6e67 456c 656d 656e  pleGradingElemen
-00000360: 742e 5f5f 696e 6974 5f5f 6301 0000 0000  t.__init__c.....
-00000370: 0000 0000 0000 0001 0000 0005 0000 0043  ...............C
-00000380: 0000 0073 3400 0000 7400 7c00 6a01 7402  ...s4...t.|.j.t.
-00000390: 8302 7215 6401 6402 a003 6403 6404 8400  ..r.d.d...d.d...
-000003a0: 7c00 6a01 4400 8301 a101 1700 6405 1700  |.j.D.......d...
-000003b0: 5300 7404 7c00 6a01 8301 5300 2906 4efa  S.t.|.j...S.).N.
-000003c0: 0228 20fa 0120 6301 0000 0000 0000 0000  .( .. c.........
-000003d0: 0000 0002 0000 0008 0000 0073 0000 0073  ...........s...s
-000003e0: 3a00 0000 8100 7c00 5d18 7d01 6400 7c01  :.....|.].}.d.|.
-000003f0: 6401 1900 6402 9b04 6403 7c01 6404 1900  d...d...d.|.d...
-00000400: 6402 9b04 6403 7c01 6405 1900 6402 9b04  d...d.|.d...d...
-00000410: 6406 9d07 5600 0100 7102 6407 5300 2908  d...V...q.d.S.).
-00000420: 7210 0000 0072 0100 0000 da01 6772 1100  r....r......gr..
-00000430: 0000 e901 0000 00e9 0200 0000 fa02 2029  .............. )
-00000440: 4e72 0900 0000 2902 da02 2e30 da01 6572  Nr....)....0..er
-00000450: 0900 0000 7209 0000 0072 0a00 0000 da09  ....r....r......
-00000460: 3c67 656e 6578 7072 3e17 0000 0073 0400  <genexpr>....s..
-00000470: 0000 0280 3800 7a2e 5369 6d70 6c65 4772  ....8.z.SimpleGr
-00000480: 6164 696e 6745 6c65 6d65 6e74 2e66 6f72  adingElement.for
-00000490: 6d61 742e 3c6c 6f63 616c 733e 2e3c 6765  mat.<locals>.<ge
-000004a0: 6e65 7870 723e 7215 0000 0029 05da 0a69  nexpr>r....)...i
-000004b0: 7369 6e73 7461 6e63 6572 0d00 0000 7202  sinstancer....r.
-000004c0: 0000 00da 046a 6f69 6eda 0373 7472 a901  .....join..str..
-000004d0: 720e 0000 0072 0900 0000 7209 0000 0072  r....r....r....r
-000004e0: 0a00 0000 da06 666f 726d 6174 1300 0000  ......format....
-000004f0: 7310 0000 000c 0102 0214 0102 ff02 0202  s...............
-00000500: fe02 ff0a 067a 1b53 696d 706c 6547 7261  .....z.SimpleGra
-00000510: 6469 6e67 456c 656d 656e 742e 666f 726d  dingElement.form
-00000520: 6174 4ea9 0672 0500 0000 7206 0000 0072  atN..r....r....r
-00000530: 0700 0000 7208 0000 0072 0f00 0000 721d  ....r....r....r.
-00000540: 0000 0072 0900 0000 7209 0000 0072 0900  ...r....r....r..
-00000550: 0000 720a 0000 0072 0c00 0000 0900 0000  ..r....r........
-00000560: 7308 0000 0008 0004 0108 020c 0772 0c00  s............r..
-00000570: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
-00000580: 0000 0002 0000 0040 0000 0072 0b00 0000  .......@...r....
-00000590: 2907 da0d 5369 6d70 6c65 4772 6164 696e  )...SimpleGradin
-000005a0: 677a 2163 6f6e 6669 6775 7461 7469 6f6e  gz!configutation
-000005b0: 2066 6f72 2027 7369 6d70 6c65 4772 6164   for 'simpleGrad
-000005c0: 696e 6727 6304 0000 0000 0000 0000 0000  ing'c...........
-000005d0: 0004 0000 0003 0000 0043 0000 0073 5a00  .........C...sZ.
-000005e0: 0000 7400 7c01 7401 8302 730b 7401 7c01  ..t.|.t...s.t.|.
-000005f0: 8301 7c00 5f02 6e03 7c01 7c00 5f02 7400  ..|._.n.|.|._.t.
-00000600: 7c02 7401 8302 7319 7401 7c02 8301 7c00  |.t...s.t.|...|.
-00000610: 5f03 6e03 7c02 7c00 5f03 7400 7c03 7401  _.n.|.|._.t.|.t.
-00000620: 8302 7328 7401 7c03 8301 7c00 5f04 6400  ..s(t.|...|._.d.
-00000630: 5300 7c03 7c00 5f04 6400 5300 a901 4e29  S.|.|._.d.S...N)
-00000640: 0572 1900 0000 720c 0000 00da 0178 da01  .r....r......x..
-00000650: 79da 017a 2904 720e 0000 0072 2100 0000  y..z).r....r!...
-00000660: 7222 0000 0072 2300 0000 7209 0000 0072  r"...r#...r....r
-00000670: 0900 0000 720a 0000 0072 0f00 0000 2100  ....r....r....!.
-00000680: 0000 7312 0000 000a 010c 0106 020a 010c  ..s.............
-00000690: 0106 020a 010e 010a 027a 1653 696d 706c  .........z.Simpl
-000006a0: 6547 7261 6469 6e67 2e5f 5f69 6e69 745f  eGrading.__init_
-000006b0: 5f63 0100 0000 0000 0000 0000 0000 0100  _c..............
-000006c0: 0000 0700 0000 4300 0000 732a 0000 0064  ......C...s*...d
-000006d0: 017c 006a 00a0 01a1 009b 0064 027c 006a  .|.j.......d.|.j
-000006e0: 02a0 01a1 009b 0064 027c 006a 03a0 01a1  .......d.|.j....
-000006f0: 009b 0064 039d 0753 0029 044e 7a0f 7369  ...d...S.).Nz.si
-00000700: 6d70 6c65 4772 6164 696e 6720 2872 1100  mpleGrading (r..
-00000710: 0000 fa01 2929 0472 2100 0000 721d 0000  ....)).r!...r...
-00000720: 0072 2200 0000 7223 0000 0072 1c00 0000  .r"...r#...r....
-00000730: 7209 0000 0072 0900 0000 720a 0000 0072  r....r....r....r
-00000740: 1d00 0000 2f00 0000 7310 0000 0002 0208  ..../...s.......
-00000750: 0104 ff08 0104 ff08 0106 ff02 ff7a 1453  .............z.S
-00000760: 696d 706c 6547 7261 6469 6e67 2e66 6f72  impleGrading.for
-00000770: 6d61 744e 721e 0000 0072 0900 0000 7209  matNr....r....r.
-00000780: 0000 0072 0900 0000 720a 0000 0072 1f00  ...r....r....r..
-00000790: 0000 1e00 0000 7308 0000 0008 0004 0108  ......s.........
-000007a0: 020c 0e72 1f00 0000 6300 0000 0000 0000  ...r....c.......
-000007b0: 0000 0000 0000 0000 0002 0000 0040 0000  .............@..
-000007c0: 0072 0b00 0000 2907 da0b 4564 6765 4772  .r....)...EdgeGr
-000007d0: 6164 696e 677a 1f63 6f6e 6669 6775 7461  adingz.configuta
-000007e0: 7469 6f6e 2066 6f72 2027 6564 6765 4772  tion for 'edgeGr
-000007f0: 6164 696e 6727 630d 0000 0000 0000 0000  ading'c.........
-00000800: 0000 000d 0000 0003 0000 0043 0000 0073  ...........C...s
-00000810: 5601 0000 7400 7c01 7401 8302 730b 7401  V...t.|.t...s.t.
-00000820: 7c01 8301 7c00 5f02 6e03 7c01 7c00 5f02  |...|._.n.|.|._.
-00000830: 7400 7c02 7401 8302 7319 7401 7c02 8301  t.|.t...s.t.|...
-00000840: 7c00 5f03 6e03 7c02 7c00 5f03 7400 7c03  |._.n.|.|._.t.|.
-00000850: 7401 8302 7327 7401 7c03 8301 7c00 5f04  t...s't.|...|._.
-00000860: 6e03 7c03 7c00 5f04 7400 7c04 7401 8302  n.|.|._.t.|.t...
-00000870: 7335 7401 7c04 8301 7c00 5f05 6e03 7c04  s5t.|...|._.n.|.
-00000880: 7c00 5f05 7400 7c05 7401 8302 7343 7401  |._.t.|.t...sCt.
-00000890: 7c05 8301 7c00 5f06 6e03 7c05 7c00 5f06  |...|._.n.|.|._.
-000008a0: 7400 7c06 7401 8302 7351 7401 7c06 8301  t.|.t...sQt.|...
-000008b0: 7c00 5f07 6e03 7c06 7c00 5f07 7400 7c07  |._.n.|.|._.t.|.
-000008c0: 7401 8302 735f 7401 7c07 8301 7c00 5f08  t...s_t.|...|._.
-000008d0: 6e03 7c07 7c00 5f08 7400 7c08 7401 8302  n.|.|._.t.|.t...
-000008e0: 736d 7401 7c08 8301 7c00 5f09 6e03 7c08  smt.|...|._.n.|.
-000008f0: 7c00 5f09 7400 7c01 7401 8302 737b 7401  |._.t.|.t...s{t.
-00000900: 7c09 8301 7c00 5f0a 6e03 7c09 7c00 5f0a  |...|._.n.|.|._.
-00000910: 7400 7c0a 7401 8302 7389 7401 7c0a 8301  t.|.t...s.t.|...
-00000920: 7c00 5f0b 6e03 7c0a 7c00 5f0b 7400 7c0b  |._.n.|.|._.t.|.
-00000930: 7401 8302 7397 7401 7c0b 8301 7c00 5f0c  t...s.t.|...|._.
-00000940: 6e03 7c0b 7c00 5f0c 7400 7c0c 7401 8302  n.|.|._.t.|.t...
-00000950: 73a6 7401 7c0c 8301 7c00 5f0d 6400 5300  s.t.|...|._.d.S.
-00000960: 7c0c 7c00 5f0d 6400 5300 7220 0000 0029  |.|._.d.S.r ...)
-00000970: 0e72 1900 0000 720c 0000 00da 0278 31da  .r....r......x1.
-00000980: 0278 32da 0278 33da 0278 34da 0279 31da  .x2..x3..x4..y1.
-00000990: 0279 32da 0279 33da 0279 34da 027a 31da  .y2..y3..y4..z1.
-000009a0: 027a 32da 027a 33da 027a 3429 0d72 0e00  .z2..z3..z4).r..
-000009b0: 0000 7226 0000 0072 2700 0000 7228 0000  ..r&...r'...r(..
-000009c0: 0072 2900 0000 722a 0000 0072 2b00 0000  .r)...r*...r+...
-000009d0: 722c 0000 0072 2d00 0000 722e 0000 0072  r,...r-...r....r
-000009e0: 2f00 0000 7230 0000 0072 3100 0000 7209  /...r0...r1...r.
-000009f0: 0000 0072 0900 0000 720a 0000 0072 0f00  ...r....r....r..
-00000a00: 0000 3900 0000 7348 0000 000a 010c 0106  ..9...sH........
-00000a10: 020a 010c 0106 020a 010c 0106 020a 010c  ................
-00000a20: 0106 020a 010c 0106 020a 010c 0106 020a  ................
-00000a30: 010c 0106 020a 010c 0106 020a 010c 0106  ................
-00000a40: 020a 010c 0106 020a 010c 0106 020a 010e  ................
-00000a50: 010a 027a 1445 6467 6547 7261 6469 6e67  ...z.EdgeGrading
-00000a60: 2e5f 5f69 6e69 745f 5f63 0100 0000 0000  .__init__c......
-00000a70: 0000 0000 0000 0500 0000 0500 0000 4300  ..............C.
-00000a80: 0000 7346 0000 0067 007d 0174 0064 0164  ..sF...g.}.t.d.d
-00000a90: 0283 0244 005d 125c 027d 027d 0374 017c  ...D.].\.}.}.t.|
-00000aa0: 007c 027c 0317 0083 027d 047c 01a0 027c  .|.|.....}.|...|
-00000ab0: 04a0 03a1 00a1 0101 0071 0764 0364 04a0  .........q.d.d..
-00000ac0: 047c 01a1 0117 0064 0517 0053 0029 064e  .|.....d...S.).N
-00000ad0: 5a03 7879 7ada 0431 3233 347a 0d65 6467  Z.xyz..1234z.edg
-00000ae0: 6547 7261 6469 6e67 2028 7211 0000 0072  eGrading (r....r
-00000af0: 2400 0000 2905 7203 0000 00da 0767 6574  $...).r......get
-00000b00: 6174 7472 da06 6170 7065 6e64 721d 0000  attr..appendr...
-00000b10: 0072 1a00 0000 2905 720e 0000 00da 0374  .r....).r......t
-00000b20: 6d70 da06 6c65 7474 6572 da05 696e 6465  mp..letter..inde
-00000b30: 78da 0376 6172 7209 0000 0072 0900 0000  x..varr....r....
-00000b40: 720a 0000 0072 1d00 0000 6b00 0000 730a  r....r....k...s.
-00000b50: 0000 0004 0112 010e 0110 0112 017a 1245  .............z.E
-00000b60: 6467 6547 7261 6469 6e67 2e66 6f72 6d61  dgeGrading.forma
-00000b70: 744e 721e 0000 0072 0900 0000 7209 0000  tNr....r....r...
-00000b80: 0072 0900 0000 720a 0000 0072 2500 0000  .r....r....r%...
-00000b90: 3600 0000 7308 0000 0008 0004 0108 020c  6...s...........
-00000ba0: 3272 2500 0000 4e29 08da 0f63 6f6c 6c65  2r%...N)...colle
-00000bb0: 6374 696f 6e73 2e61 6263 7202 0000 00da  ctions.abcr.....
-00000bc0: 0969 7465 7274 6f6f 6c73 7203 0000 0072  .itertoolsr....r
-00000bd0: 0400 0000 720c 0000 0072 1f00 0000 7225  ....r....r....r%
-00000be0: 0000 0072 0900 0000 7209 0000 0072 0900  ...r....r....r..
-00000bf0: 0000 720a 0000 00da 083c 6d6f 6475 6c65  ..r......<module
-00000c00: 3e01 0000 0073 0c00 0000 0c00 0c01 0e03  >....s..........
-00000c10: 0e04 1015 1418                           ......
+00000140: 0000 00fa 542f 686f 6d65 2f70 6965 7272  ....T/home/pierr
+00000150: 652f 4465 762f 666c 7569 6473 696d 666f  e/Dev/fluidsimfo
+00000160: 616d 2f73 7263 2f66 6c75 6964 7369 6d66  am/src/fluidsimf
+00000170: 6f61 6d2f 666f 616d 5f69 6e70 7574 5f66  oam/foam_input_f
+00000180: 696c 6573 2f62 6c6f 636b 6d65 7368 2f67  iles/blockmesh/g
+00000190: 7261 6469 6e67 2e70 7972 0400 0000 0500  rading.pyr......
+000001a0: 0000 7304 0000 0008 0008 0172 0400 0000  ..s........r....
+000001b0: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+000001c0: 0002 0000 0040 0000 00f3 2000 0000 6500  .....@.... ...e.
+000001d0: 5a01 6400 5a02 6401 5a03 6402 6403 8400  Z.d.Z.d.Z.d.d...
+000001e0: 5a04 6404 6405 8400 5a05 6406 5300 2907  Z.d.d...Z.d.S.).
+000001f0: da14 5369 6d70 6c65 4772 6164 696e 6745  ..SimpleGradingE
+00000200: 6c65 6d65 6e74 7a3c 782c 2079 206f 7220  lementz<x, y or 
+00000210: 7a20 456c 656d 656e 7420 6f66 2073 696d  z Element of sim
+00000220: 706c 6547 7261 6469 6e67 2e20 6164 6f70  pleGrading. adop
+00000230: 7465 6420 746f 206d 756c 7469 2d67 7261  ted to multi-gra
+00000240: 6469 6e67 6302 0000 0000 0000 0000 0000  dingc...........
+00000250: 0002 0000 0002 0000 0043 0000 0073 0a00  .........C...s..
+00000260: 0000 7c01 7c00 5f00 6401 5300 2902 7a9b  ..|.|._.d.S.).z.
+00000270: 696e 6974 6961 6c69 7a61 7469 6f6e 0a20  initialization. 
+00000280: 2020 2020 2020 2064 2069 7320 7369 6e67         d is sing
+00000290: 6c65 206e 756d 6265 7220 666f 7220 6578  le number for ex
+000002a0: 7061 6e73 696f 6e20 7261 7469 6f0a 2020  pansion ratio.  
+000002b0: 2020 2020 2020 2020 6f72 2069 7465 7261          or itera
+000002c0: 7469 7665 206f 626a 6563 7420 636f 6e73  tive object cons
+000002d0: 6974 7320 2864 6972 6563 7469 6f6e 2072  its (direction r
+000002e0: 6174 696f 2c20 6365 6c6c 2072 6174 696f  atio, cell ratio
+000002f0: 2c20 6578 7061 6e73 696f 6e20 7261 7469  , expansion rati
+00000300: 6f29 0a20 2020 2020 2020 204e 2901 da01  o).        N)...
+00000310: 6429 02da 0473 656c 6672 0d00 0000 7209  d)...selfr....r.
+00000320: 0000 0072 0900 0000 720a 0000 00da 085f  ...r....r......_
+00000330: 5f69 6e69 745f 5f0c 0000 0073 0200 0000  _init__....s....
+00000340: 0a05 7a1d 5369 6d70 6c65 4772 6164 696e  ..z.SimpleGradin
+00000350: 6745 6c65 6d65 6e74 2e5f 5f69 6e69 745f  gElement.__init_
+00000360: 5f63 0100 0000 0000 0000 0000 0000 0100  _c..............
+00000370: 0000 0500 0000 4300 0000 7334 0000 0074  ......C...s4...t
+00000380: 007c 006a 0174 0283 0272 1564 0164 02a0  .|.j.t...r.d.d..
+00000390: 0364 0364 0484 007c 006a 0144 0083 01a1  .d.d...|.j.D....
+000003a0: 0117 0064 0517 0053 0074 047c 006a 0183  ...d...S.t.|.j..
+000003b0: 0153 0029 064e fa02 2820 fa01 2063 0100  .S.).N..( .. c..
+000003c0: 0000 0000 0000 0000 0000 0200 0000 0800  ................
+000003d0: 0000 7300 0000 733a 0000 0081 007c 005d  ..s...s:.....|.]
+000003e0: 187d 0164 007c 0164 0119 0064 029b 0464  .}.d.|.d...d...d
+000003f0: 037c 0164 0419 0064 029b 0464 037c 0164  .|.d...d...d.|.d
+00000400: 0519 0064 029b 0464 069d 0756 0001 0071  ...d...d...V...q
+00000410: 0264 0753 0029 0872 1000 0000 7201 0000  .d.S.).r....r...
+00000420: 00da 0167 7211 0000 00e9 0100 0000 e902  ...gr...........
+00000430: 0000 00fa 0220 294e 7209 0000 0029 02da  ..... )Nr....)..
+00000440: 022e 30da 0165 7209 0000 0072 0900 0000  ..0..er....r....
+00000450: 720a 0000 00da 093c 6765 6e65 7870 723e  r......<genexpr>
+00000460: 1700 0000 7304 0000 0002 8038 007a 2e53  ....s......8.z.S
+00000470: 696d 706c 6547 7261 6469 6e67 456c 656d  impleGradingElem
+00000480: 656e 742e 666f 726d 6174 2e3c 6c6f 6361  ent.format.<loca
+00000490: 6c73 3e2e 3c67 656e 6578 7072 3e72 1500  ls>.<genexpr>r..
+000004a0: 0000 2905 da0a 6973 696e 7374 616e 6365  ..)...isinstance
+000004b0: 720d 0000 0072 0200 0000 da04 6a6f 696e  r....r......join
+000004c0: da03 7374 72a9 0172 0e00 0000 7209 0000  ..str..r....r...
+000004d0: 0072 0900 0000 720a 0000 00da 0666 6f72  .r....r......for
+000004e0: 6d61 7413 0000 0073 1000 0000 0c01 0202  mat....s........
+000004f0: 1401 02ff 0202 02fe 02ff 0a06 7a1b 5369  ............z.Si
+00000500: 6d70 6c65 4772 6164 696e 6745 6c65 6d65  mpleGradingEleme
+00000510: 6e74 2e66 6f72 6d61 744e a906 7205 0000  nt.formatN..r...
+00000520: 0072 0600 0000 7207 0000 0072 0800 0000  .r....r....r....
+00000530: 720f 0000 0072 1d00 0000 7209 0000 0072  r....r....r....r
+00000540: 0900 0000 7209 0000 0072 0a00 0000 720c  ....r....r....r.
+00000550: 0000 0009 0000 0073 0800 0000 0800 0401  .......s........
+00000560: 0802 0c07 720c 0000 0063 0000 0000 0000  ....r....c......
+00000570: 0000 0000 0000 0000 0000 0200 0000 4000  ..............@.
+00000580: 0000 720b 0000 0029 07da 0d53 696d 706c  ..r....)...Simpl
+00000590: 6547 7261 6469 6e67 7a21 636f 6e66 6967  eGradingz!config
+000005a0: 7574 6174 696f 6e20 666f 7220 2773 696d  utation for 'sim
+000005b0: 706c 6547 7261 6469 6e67 2763 0400 0000  pleGrading'c....
+000005c0: 0000 0000 0000 0000 0400 0000 0300 0000  ................
+000005d0: 4300 0000 735a 0000 0074 007c 0174 0183  C...sZ...t.|.t..
+000005e0: 0273 0b74 017c 0183 017c 005f 026e 037c  .s.t.|...|._.n.|
+000005f0: 017c 005f 0274 007c 0274 0183 0273 1974  .|._.t.|.t...s.t
+00000600: 017c 0283 017c 005f 036e 037c 027c 005f  .|...|._.n.|.|._
+00000610: 0374 007c 0374 0183 0273 2874 017c 0383  .t.|.t...s(t.|..
+00000620: 017c 005f 0464 0053 007c 037c 005f 0464  .|._.d.S.|.|._.d
+00000630: 0053 00a9 014e 2905 7219 0000 0072 0c00  .S...N).r....r..
+00000640: 0000 da01 78da 0179 da01 7a29 0472 0e00  ....x..y..z).r..
+00000650: 0000 7221 0000 0072 2200 0000 7223 0000  ..r!...r"...r#..
+00000660: 0072 0900 0000 7209 0000 0072 0a00 0000  .r....r....r....
+00000670: 720f 0000 0021 0000 0073 1200 0000 0a01  r....!...s......
+00000680: 0c01 0602 0a01 0c01 0602 0a01 0e01 0a02  ................
+00000690: 7a16 5369 6d70 6c65 4772 6164 696e 672e  z.SimpleGrading.
+000006a0: 5f5f 696e 6974 5f5f 6301 0000 0000 0000  __init__c.......
+000006b0: 0000 0000 0001 0000 0007 0000 0043 0000  .............C..
+000006c0: 0073 2a00 0000 6401 7c00 6a00 a001 a100  .s*...d.|.j.....
+000006d0: 9b00 6402 7c00 6a02 a001 a100 9b00 6402  ..d.|.j.......d.
+000006e0: 7c00 6a03 a001 a100 9b00 6403 9d07 5300  |.j.......d...S.
+000006f0: 2904 4e7a 0f73 696d 706c 6547 7261 6469  ).Nz.simpleGradi
+00000700: 6e67 2028 7211 0000 00fa 0129 2904 7221  ng (r......)).r!
+00000710: 0000 0072 1d00 0000 7222 0000 0072 2300  ...r....r"...r#.
+00000720: 0000 721c 0000 0072 0900 0000 7209 0000  ..r....r....r...
+00000730: 0072 0a00 0000 721d 0000 002f 0000 0073  .r....r..../...s
+00000740: 1000 0000 0202 0801 04ff 0801 04ff 0801  ................
+00000750: 06ff 02ff 7a14 5369 6d70 6c65 4772 6164  ....z.SimpleGrad
+00000760: 696e 672e 666f 726d 6174 4e72 1e00 0000  ing.formatNr....
+00000770: 7209 0000 0072 0900 0000 7209 0000 0072  r....r....r....r
+00000780: 0a00 0000 721f 0000 001e 0000 0073 0800  ....r........s..
+00000790: 0000 0800 0401 0802 0c0e 721f 0000 0063  ..........r....c
+000007a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000007b0: 0200 0000 4000 0000 720b 0000 0029 07da  ....@...r....)..
+000007c0: 0b45 6467 6547 7261 6469 6e67 7a1f 636f  .EdgeGradingz.co
+000007d0: 6e66 6967 7574 6174 696f 6e20 666f 7220  nfigutation for 
+000007e0: 2765 6467 6547 7261 6469 6e67 2763 0d00  'edgeGrading'c..
+000007f0: 0000 0000 0000 0000 0000 0d00 0000 0300  ................
+00000800: 0000 4300 0000 7356 0100 0074 007c 0174  ..C...sV...t.|.t
+00000810: 0183 0273 0b74 017c 0183 017c 005f 026e  ...s.t.|...|._.n
+00000820: 037c 017c 005f 0274 007c 0274 0183 0273  .|.|._.t.|.t...s
+00000830: 1974 017c 0283 017c 005f 036e 037c 027c  .t.|...|._.n.|.|
+00000840: 005f 0374 007c 0374 0183 0273 2774 017c  ._.t.|.t...s't.|
+00000850: 0383 017c 005f 046e 037c 037c 005f 0474  ...|._.n.|.|._.t
+00000860: 007c 0474 0183 0273 3574 017c 0483 017c  .|.t...s5t.|...|
+00000870: 005f 056e 037c 047c 005f 0574 007c 0574  ._.n.|.|._.t.|.t
+00000880: 0183 0273 4374 017c 0583 017c 005f 066e  ...sCt.|...|._.n
+00000890: 037c 057c 005f 0674 007c 0674 0183 0273  .|.|._.t.|.t...s
+000008a0: 5174 017c 0683 017c 005f 076e 037c 067c  Qt.|...|._.n.|.|
+000008b0: 005f 0774 007c 0774 0183 0273 5f74 017c  ._.t.|.t...s_t.|
+000008c0: 0783 017c 005f 086e 037c 077c 005f 0874  ...|._.n.|.|._.t
+000008d0: 007c 0874 0183 0273 6d74 017c 0883 017c  .|.t...smt.|...|
+000008e0: 005f 096e 037c 087c 005f 0974 007c 0174  ._.n.|.|._.t.|.t
+000008f0: 0183 0273 7b74 017c 0983 017c 005f 0a6e  ...s{t.|...|._.n
+00000900: 037c 097c 005f 0a74 007c 0a74 0183 0273  .|.|._.t.|.t...s
+00000910: 8974 017c 0a83 017c 005f 0b6e 037c 0a7c  .t.|...|._.n.|.|
+00000920: 005f 0b74 007c 0b74 0183 0273 9774 017c  ._.t.|.t...s.t.|
+00000930: 0b83 017c 005f 0c6e 037c 0b7c 005f 0c74  ...|._.n.|.|._.t
+00000940: 007c 0c74 0183 0273 a674 017c 0c83 017c  .|.t...s.t.|...|
+00000950: 005f 0d64 0053 007c 0c7c 005f 0d64 0053  ._.d.S.|.|._.d.S
+00000960: 0072 2000 0000 290e 7219 0000 0072 0c00  .r ...).r....r..
+00000970: 0000 da02 7831 da02 7832 da02 7833 da02  ....x1..x2..x3..
+00000980: 7834 da02 7931 da02 7932 da02 7933 da02  x4..y1..y2..y3..
+00000990: 7934 da02 7a31 da02 7a32 da02 7a33 da02  y4..z1..z2..z3..
+000009a0: 7a34 290d 720e 0000 0072 2600 0000 7227  z4).r....r&...r'
+000009b0: 0000 0072 2800 0000 7229 0000 0072 2a00  ...r(...r)...r*.
+000009c0: 0000 722b 0000 0072 2c00 0000 722d 0000  ..r+...r,...r-..
+000009d0: 0072 2e00 0000 722f 0000 0072 3000 0000  .r....r/...r0...
+000009e0: 7231 0000 0072 0900 0000 7209 0000 0072  r1...r....r....r
+000009f0: 0a00 0000 720f 0000 0039 0000 0073 4800  ....r....9...sH.
+00000a00: 0000 0a01 0c01 0602 0a01 0c01 0602 0a01  ................
+00000a10: 0c01 0602 0a01 0c01 0602 0a01 0c01 0602  ................
+00000a20: 0a01 0c01 0602 0a01 0c01 0602 0a01 0c01  ................
+00000a30: 0602 0a01 0c01 0602 0a01 0c01 0602 0a01  ................
+00000a40: 0c01 0602 0a01 0e01 0a02 7a14 4564 6765  ..........z.Edge
+00000a50: 4772 6164 696e 672e 5f5f 696e 6974 5f5f  Grading.__init__
+00000a60: 6301 0000 0000 0000 0000 0000 0005 0000  c...............
+00000a70: 0005 0000 0043 0000 0073 4600 0000 6700  .....C...sF...g.
+00000a80: 7d01 7400 6401 6402 8302 4400 5d12 5c02  }.t.d.d...D.].\.
+00000a90: 7d02 7d03 7401 7c00 7c02 7c03 1700 8302  }.}.t.|.|.|.....
+00000aa0: 7d04 7c01 a002 7c04 a003 a100 a101 0100  }.|...|.........
+00000ab0: 7107 6403 6404 a004 7c01 a101 1700 6405  q.d.d...|.....d.
+00000ac0: 1700 5300 2906 4e5a 0378 797a da04 3132  ..S.).NZ.xyz..12
+00000ad0: 3334 7a0d 6564 6765 4772 6164 696e 6720  34z.edgeGrading 
+00000ae0: 2872 1100 0000 7224 0000 0029 0572 0300  (r....r$...).r..
+00000af0: 0000 da07 6765 7461 7474 72da 0661 7070  ....getattr..app
+00000b00: 656e 6472 1d00 0000 721a 0000 0029 0572  endr....r....).r
+00000b10: 0e00 0000 da03 746d 70da 066c 6574 7465  ......tmp..lette
+00000b20: 72da 0569 6e64 6578 da03 7661 7272 0900  r..index..varr..
+00000b30: 0000 7209 0000 0072 0a00 0000 721d 0000  ..r....r....r...
+00000b40: 006b 0000 0073 0a00 0000 0401 1201 0e01  .k...s..........
+00000b50: 1001 1201 7a12 4564 6765 4772 6164 696e  ....z.EdgeGradin
+00000b60: 672e 666f 726d 6174 4e72 1e00 0000 7209  g.formatNr....r.
+00000b70: 0000 0072 0900 0000 7209 0000 0072 0a00  ...r....r....r..
+00000b80: 0000 7225 0000 0036 0000 0073 0800 0000  ..r%...6...s....
+00000b90: 0800 0401 0802 0c32 7225 0000 004e 2908  .......2r%...N).
+00000ba0: da0f 636f 6c6c 6563 7469 6f6e 732e 6162  ..collections.ab
+00000bb0: 6372 0200 0000 da09 6974 6572 746f 6f6c  cr......itertool
+00000bc0: 7372 0300 0000 7204 0000 0072 0c00 0000  sr....r....r....
+00000bd0: 721f 0000 0072 2500 0000 7209 0000 0072  r....r%...r....r
+00000be0: 0900 0000 7209 0000 0072 0a00 0000 da08  ....r....r......
+00000bf0: 3c6d 6f64 756c 653e 0100 0000 730c 0000  <module>....s...
+00000c00: 000c 000c 010e 030e 0410 1514 18         .............
```

### Comparing `fluidsimfoam-0.0.5/src/fluidsimfoam/foam_input_files/blockmesh/edges.py` & `fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/blockmesh/edges.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+class Point:
+    def __init__(self, x, y, z):
+        self.x = x
+        self.y = y
+        self.z = z
+
+    def format(self):
+        return f"( {self.x:18.15g} {self.y:18.15g} {self.z:18.15g} )"
+
+
 class ArcEdge:
     def __init__(self, vnames, name, inter_vertex):
         """Initialize ArcEdge instance
         vnames is the vertex names in order descrived in
           http://www.openfoam.org/docs/user/mesh-description.php
         # two vertices is needed for Arc
         cells is number of cells devied into in each direction
@@ -30,14 +40,16 @@
         """Initialize SplineEdge instance
         vnames is the vertex names in order descrived in
           http://www.openfoam.org/docs/user/mesh-description.php
         # two vertices is needed for Spline
         """
         self.vnames = vnames
         self.name = name
+        if points and not isinstance(points[0], Point):
+            points = [Point(x, y, z) for x, y, z in points]
         self.points = points
 
     def format(self, vertices):
         """Format instance to dump
         vertices is dict of name to Vertex
         """
         index = " ".join(str(vertices[vn].index) for vn in self.vnames)
```

### Comparing `fluidsimfoam-0.0.5/src/fluidsimfoam/foam_input_files/blockmesh/grading.py` & `fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/blockmesh/grading.py`

 * *Files identical despite different names*

### Comparing `fluidsimfoam-0.0.5/src/fluidsimfoam/foam_input_files/constant_files.py` & `fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/constant_files.py`

 * *Files identical despite different names*

### Comparing `fluidsimfoam-0.0.5/src/fluidsimfoam/foam_input_files/control_dict.py` & `fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/control_dict.py`

 * *Files identical despite different names*

### Comparing `fluidsimfoam-0.0.5/src/fluidsimfoam/foam_input_files/fields.py` & `fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/fields.py`

 * *Files identical despite different names*

### Comparing `fluidsimfoam-0.0.5/src/fluidsimfoam/foam_input_files/format.py` & `fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/format.py`

 * *Files identical despite different names*

### Comparing `fluidsimfoam-0.0.5/src/fluidsimfoam/foam_input_files/fv_options.py` & `fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/fv_options.py`

 * *Files identical despite different names*

### Comparing `fluidsimfoam-0.0.5/src/fluidsimfoam/foam_input_files/fv_schemes.py` & `fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/fv_schemes.py`

 * *Files identical despite different names*

### Comparing `fluidsimfoam-0.0.5/src/fluidsimfoam/foam_input_files/generators.py` & `fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/generators.py`

 * *Files identical despite different names*

### Comparing `fluidsimfoam-0.0.5/src/fluidsimfoam/foam_input_files/grammar.lark` & `fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/grammar.lark`

 * *Files identical despite different names*

### Comparing `fluidsimfoam-0.0.5/src/fluidsimfoam/foam_input_files/grammar_advanced.lark` & `fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/grammar_advanced.lark`

 * *Files identical despite different names*

### Comparing `fluidsimfoam-0.0.5/src/fluidsimfoam/foam_input_files/parser.py` & `fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/parser.py`

 * *Files identical despite different names*

### Comparing `fluidsimfoam-0.0.5/src/fluidsimfoam/foam_input_files/polymesh.py` & `fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/polymesh.py`

 * *Files identical despite different names*

### Comparing `fluidsimfoam-0.0.5/src/fluidsimfoam/foam_input_files/util.py` & `fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/util.py`

 * *Files identical despite different names*

### Comparing `fluidsimfoam-0.0.5/src/fluidsimfoam/info.py` & `fluidsimfoam-0.0.6/src/fluidsimfoam/info.py`

 * *Files identical despite different names*

### Comparing `fluidsimfoam-0.0.5/src/fluidsimfoam/log.py` & `fluidsimfoam-0.0.6/src/fluidsimfoam/log.py`

 * *Files identical despite different names*

### Comparing `fluidsimfoam-0.0.5/src/fluidsimfoam/make.py` & `fluidsimfoam-0.0.6/src/fluidsimfoam/make.py`

 * *Files identical despite different names*

### Comparing `fluidsimfoam-0.0.5/src/fluidsimfoam/operators.py` & `fluidsimfoam-0.0.6/src/fluidsimfoam/operators.py`

 * *Files identical despite different names*

### Comparing `fluidsimfoam-0.0.5/src/fluidsimfoam/output/__pycache__/__init__.cpython-39.pyc` & `fluidsimfoam-0.0.6/src/fluidsimfoam/output/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun  1 13:07:51 2023 UTC, .py size: 423 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 2798 7864 a701 0000  a.......'.xd....
+00000000: 6f0d 0d0a 0000 0000 1cb9 6f64 a701 0000  o.........od....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 3800 0000 6400  .....@...s8...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6403  Z.d.d.l.m.Z...d.
 00000040: 6404 6c03 6d04 5a04 0100 6403 6405 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 6d07 5a07 0100 6700 6406 a201  m.Z.m.Z...g.d...
 00000060: 5a08 6407 5300 2908 7a7b 4261 7365 2063  Z.d.S.).z{Base c
 00000070: 6c61 7373 2066 6f72 2074 6865 2060 6073  lass for the ``s
@@ -22,14 +22,13 @@
 00000150: 7205 0000 0072 0600 0000 4e29 09da 075f  r....r....N)..._
 00000160: 5f64 6f63 5f5f da13 666c 7569 6473 696d  _doc__..fluidsim
 00000170: 5f63 6f72 652e 7061 7468 7372 0200 0000  _core.pathsr....
 00000180: da04 6261 7365 7204 0000 005a 1464 6174  ..baser....Z.dat
 00000190: 6166 7261 6d65 5f66 726f 6d5f 7061 7468  aframe_from_path
 000001a0: 7372 0500 0000 7206 0000 00da 075f 5f61  sr....r......__a
 000001b0: 6c6c 5f5f a900 720b 0000 0072 0b00 0000  ll__..r....r....
-000001c0: fa4a 2f68 6f6d 652f 7573 6572 732f 6175  .J/home/users/au
-000001d0: 6769 6572 3370 692f 4465 762f 666c 7569  gier3pi/Dev/flui
-000001e0: 6473 696d 666f 616d 2f73 7263 2f66 6c75  dsimfoam/src/flu
-000001f0: 6964 7369 6d66 6f61 6d2f 6f75 7470 7574  idsimfoam/output
-00000200: 2f5f 5f69 6e69 745f 5f2e 7079 da08 3c6d  /__init__.py..<m
-00000210: 6f64 756c 653e 0100 0000 7308 0000 0004  odule>....s.....
-00000220: 0c0c 020c 0110 05                        .......
+000001c0: fa41 2f68 6f6d 652f 7069 6572 7265 2f44  .A/home/pierre/D
+000001d0: 6576 2f66 6c75 6964 7369 6d66 6f61 6d2f  ev/fluidsimfoam/
+000001e0: 7372 632f 666c 7569 6473 696d 666f 616d  src/fluidsimfoam
+000001f0: 2f6f 7574 7075 742f 5f5f 696e 6974 5f5f  /output/__init__
+00000200: 2e70 79da 083c 6d6f 6475 6c65 3e01 0000  .py..<module>...
+00000210: 0073 0a00 0000 0400 0c0c 0c02 1001 0c05  .s..............
```

### Comparing `fluidsimfoam-0.0.5/src/fluidsimfoam/output/__pycache__/base.cpython-310.pyc` & `fluidsimfoam-0.0.6/src/fluidsimfoam/output/__pycache__/base.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu May 11 13:56:50 2023 UTC, .py size: 9546 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 19% similar despite different names*

```diff
@@ -1,487 +1,485 @@
-00000000: 6f0d 0d0a 0000 0000 22f4 5c64 4a25 0000  o.......".\dJ%..
+00000000: 6f0d 0d0a 0000 0000 84f0 7c64 f927 0000  o.........|d.'..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 b400 0000 6400  .....@...s....d.
-00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
-00000040: 6401 6c02 5a02 6400 6402 6c03 6d04 5a04  d.l.Z.d.d.l.m.Z.
-00000050: 0100 6400 6403 6c05 6d06 5a06 0100 6400  ..d.d.l.m.Z...d.
-00000060: 6404 6c07 6d08 5a08 0100 6400 6405 6c09  d.l.m.Z...d.d.l.
-00000070: 6d0a 5a0a 0100 6400 6406 6c0b 6d0c 5a0c  m.Z...d.d.l.m.Z.
-00000080: 0100 6400 6407 6c0d 6d0e 5a0e 0100 6400  ..d.d.l.m.Z...d.
-00000090: 6408 6c0f 6d10 5a10 6d11 5a11 6d12 5a12  d.l.m.Z.m.Z.m.Z.
-000000a0: 6d13 5a13 0100 6400 6409 6c14 6d15 5a15  m.Z...d.d.l.m.Z.
-000000b0: 6d16 5a16 0100 6400 640a 6c17 6d18 5a18  m.Z...d.d.l.m.Z.
-000000c0: 0100 6400 640b 6c19 6d1a 5a1a 0100 4700  ..d.d.l.m.Z...G.
-000000d0: 640c 640d 8400 640d 650c 8303 5a1b 6401  d.d...d.e...Z.d.
-000000e0: 5300 290e e900 0000 004e 2901 da04 5061  S.)......N)...Pa
-000000f0: 7468 a901 da0a 756e 6465 7273 636f 7265  th....underscore
-00000100: 2901 da11 7374 646f 7574 5f72 6564 6972  )...stdout_redir
-00000110: 6563 7465 6429 01da 036d 7069 2901 da0a  ected)...mpi)...
-00000120: 4f75 7470 7574 436f 7265 2901 da14 6974  OutputCore)...it
-00000130: 6572 5f63 6f6d 706c 6574 655f 7061 7261  er_complete_para
-00000140: 6d73 2904 da14 4445 4641 554c 545f 434f  ms)...DEFAULT_CO
-00000150: 4e54 524f 4c5f 4449 4354 da0e 4445 4641  NTROL_DICT..DEFA
-00000160: 554c 545f 4845 4144 4552 da12 436f 6e73  ULT_HEADER..Cons
-00000170: 7461 6e74 4669 6c65 4865 6c70 6572 da0d  tantFileHelper..
-00000180: 466f 616d 496e 7075 7446 696c 6529 02da  FoamInputFile)..
-00000190: 0a49 6e70 7574 4669 6c65 73da 186e 6577  .InputFiles..new
-000001a0: 5f66 696c 655f 6765 6e65 7261 746f 725f  _file_generator_
-000001b0: 636c 6173 7329 01da 066c 6f67 6765 7229  class)...logger)
-000001c0: 01da 1267 6574 5f73 6f6c 7665 725f 7061  ...get_solver_pa
-000001d0: 636b 6167 6563 0000 0000 0000 0000 0000  ckagec..........
-000001e0: 0000 0000 0000 0400 0000 0000 0000 73c0  ..............s.
-000001f0: 0000 0065 005a 0164 005a 0264 0164 0267  ...e.Z.d.Z.d.d.g
-00000200: 025a 0364 0364 0467 025a 0467 0064 05a2  .Z.d.d.g.Z.g.d..
-00000210: 015a 0565 065a 0765 0864 0464 0664 0769  .Z.e.Z.e.d.d.d.i
-00000220: 0183 025a 0965 0a64 0864 0984 0083 015a  ...Z.e.d.d.....Z
-00000230: 0b65 0a64 0a64 0b84 0083 015a 0c65 0a64  .e.d.d.....Z.e.d
-00000240: 0c64 0d84 0083 015a 0d65 0a64 0e64 0f84  .d.....Z.e.d.d..
-00000250: 0083 015a 0e64 2187 0066 0164 1164 1284  ...Z.d!..f.d.d..
-00000260: 095a 0f65 0a64 1364 1484 0083 015a 1087  .Z.e.d.d.....Z..
-00000270: 0066 0164 1564 1684 085a 1164 1764 1884  .f.d.d...Z.d.d..
-00000280: 005a 1265 0a64 1964 1a84 0083 015a 1364  .Z.e.d.d.....Z.d
-00000290: 1b64 1c84 005a 1464 1d64 1e84 005a 1565  .d...Z.d.d...Z.e
-000002a0: 0a64 1f64 2084 0083 015a 1687 0004 005a  .d.d ....Z.....Z
-000002b0: 1753 0029 22da 064f 7574 7075 74da 0170  .S.)"..Output..p
-000002c0: da01 55da 1374 7261 6e73 706f 7274 5072  ..U..transportPr
-000002d0: 6f70 6572 7469 6573 5a14 7475 7262 756c  opertiesZ.turbul
-000002e0: 656e 6365 5072 6f70 6572 7469 6573 2903  enceProperties).
-000002f0: da0b 636f 6e74 726f 6c44 6963 74da 0966  ..controlDict..f
-00000300: 7653 6368 656d 6573 5a0a 6676 536f 6c75  vSchemesZ.fvSolu
-00000310: 7469 6f6e da0e 7369 6d75 6c61 7469 6f6e  tion..simulation
-00000320: 5479 7065 5a07 6c61 6d69 6e61 7263 0200  TypeZ.laminarc..
-00000330: 0000 0000 0000 0000 0000 0300 0000 0300  ................
-00000340: 0000 4300 0000 7328 0000 007c 016a 006a  ..C...s(...|.j.j
-00000350: 01a0 0264 01a1 017d 027c 00a0 037c 02a1  ...d...}.|...|..
-00000360: 0101 007c 016a 006a 01a0 04a1 0001 0064  ...|.j.j.......d
-00000370: 0253 0029 037a 6643 6f6d 706c 6574 6520  .S.).zfComplete 
-00000380: 7468 6520 696e 666f 5f73 6f6c 7665 7220  the info_solver 
-00000390: 696e 7374 616e 6365 2077 6974 6820 6368  instance with ch
-000003a0: 696c 6420 636c 6173 7320 6465 7461 696c  ild class detail
-000003b0: 7320 286d 6f64 756c 650a 2020 2020 2020  s (module.      
-000003c0: 2020 616e 6420 636c 6173 7320 6e61 6d65    and class name
-000003d0: 7329 2e0a 0a20 2020 2020 2020 20da 0763  s)...        ..c
-000003e0: 6c61 7373 6573 4e29 0572 1800 0000 7211  lassesN).r....r.
-000003f0: 0000 00da 0a5f 7365 745f 6368 696c 64da  ....._set_child.
-00000400: 185f 7365 745f 696e 666f 5f73 6f6c 7665  ._set_info_solve
-00000410: 725f 636c 6173 7365 73da 1563 6f6d 706c  r_classes..compl
-00000420: 6574 655f 7769 7468 5f63 6c61 7373 6573  ete_with_classes
-00000430: 2903 da03 636c 73da 0b69 6e66 6f5f 736f  )...cls..info_so
-00000440: 6c76 6572 7218 0000 00a9 0072 1e00 0000  lverr......r....
-00000450: fa46 2f68 6f6d 652f 7573 6572 732f 6175  .F/home/users/au
-00000460: 6769 6572 3370 692f 4465 762f 666c 7569  gier3pi/Dev/flui
-00000470: 6473 696d 666f 616d 2f73 7263 2f66 6c75  dsimfoam/src/flu
-00000480: 6964 7369 6d66 6f61 6d2f 6f75 7470 7574  idsimfoam/output
-00000490: 2f62 6173 652e 7079 da15 5f63 6f6d 706c  /base.py.._compl
-000004a0: 6574 655f 696e 666f 5f73 6f6c 7665 7224  ete_info_solver$
-000004b0: 0000 0073 0600 0000 0e06 0a01 1002 7a1c  ...s..........z.
-000004c0: 4f75 7470 7574 2e5f 636f 6d70 6c65 7465  Output._complete
-000004d0: 5f69 6e66 6f5f 736f 6c76 6572 6302 0000  _info_solverc...
-000004e0: 0000 0000 0000 0000 0002 0000 0007 0000  ................
-000004f0: 0043 0000 0073 2c00 0000 7c01 a000 6401  .C...s,...|...d.
-00000500: 7401 6402 6401 6403 8d02 a102 0100 7c01  t.d.d.d.......|.
-00000510: a000 6404 7401 6405 6404 6403 8d02 a102  ..d.t.d.d.d.....
-00000520: 0100 6406 5300 2907 7a2e 5365 7420 7468  ..d.S.).z.Set th
-00000530: 6520 636c 6173 7365 7320 666f 7220 696e  e classes for in
-00000540: 666f 5f73 6f6c 7665 722e 636c 6173 7365  fo_solver.classe
-00000550: 732e 4f75 7470 7574 5a03 4c6f 677a 1766  s.OutputZ.Logz.f
-00000560: 6c75 6964 7369 6d66 6f61 6d2e 6f75 7470  luidsimfoam.outp
-00000570: 7574 2e6c 6f67 2902 da0b 6d6f 6475 6c65  ut.log)...module
-00000580: 5f6e 616d 65da 0a63 6c61 7373 5f6e 616d  _name..class_nam
-00000590: 655a 0646 6965 6c64 737a 1a66 6c75 6964  eZ.Fieldsz.fluid
-000005a0: 7369 6d66 6f61 6d2e 6f75 7470 7574 2e66  simfoam.output.f
-000005b0: 6965 6c64 734e 2902 7219 0000 00da 0464  ieldsN).r......d
-000005c0: 6963 7429 0272 1c00 0000 7218 0000 0072  ict).r....r....r
-000005d0: 1e00 0000 721e 0000 0072 1f00 0000 721a  ....r....r....r.
-000005e0: 0000 002f 0000 0073 1c00 0000 0403 0201  .../...s........
-000005f0: 0201 0201 0201 04fe 04fe 0408 0201 0201  ................
-00000600: 0201 0201 04fe 08fe 7a1f 4f75 7470 7574  ........z.Output
-00000610: 2e5f 7365 745f 696e 666f 5f73 6f6c 7665  ._set_info_solve
-00000620: 725f 636c 6173 7365 7363 0100 0000 0000  r_classesc......
-00000630: 0000 0000 0000 0400 0000 0700 0000 4300  ..............C.
-00000640: 0000 7362 0000 0069 0004 007d 017c 005f  ..sb...i...}.|._
-00000650: 007c 006a 0144 005d 0c7d 0274 027c 0283  .|.j.D.].}.t.|..
-00000660: 017c 017c 02a0 0364 0164 02a1 023c 0071  .|.|...d.d...<.q
-00000670: 087c 006a 0444 005d 097d 0374 027c 0364  .|.j.D.].}.t.|.d
-00000680: 0383 027c 017c 033c 0071 187c 006a 0544  ...|.|.<.q.|.j.D
-00000690: 005d 097d 0374 027c 0364 0483 027c 017c  .].}.t.|.d...|.|
-000006a0: 033c 0071 2564 0053 0029 054e da01 2eda  .<.q%d.S.).N....
-000006b0: 015f da08 636f 6e73 7461 6e74 da06 7379  ._..constant..sy
-000006c0: 7374 656d 2906 da18 5f66 696c 655f 6765  stem)..._file_ge
-000006d0: 6e65 7261 746f 7273 5f63 6c61 7373 6573  nerators_classes
-000006e0: da0e 7661 7269 6162 6c65 5f6e 616d 6573  ..variable_names
-000006f0: 720e 0000 00da 0772 6570 6c61 6365 da14  r......replace..
-00000700: 636f 6e73 7461 6e74 5f66 696c 6573 5f6e  constant_files_n
-00000710: 616d 6573 da12 7379 7374 656d 5f66 696c  ames..system_fil
-00000720: 6573 5f6e 616d 6573 2904 721c 0000 0072  es_names).r....r
-00000730: 1800 0000 5a0d 7661 7269 6162 6c65 5f6e  ....Z.variable_n
-00000740: 616d 65da 0966 696c 655f 6e61 6d65 721e  ame..file_namer.
-00000750: 0000 0072 1e00 0000 721f 0000 00da 1e5f  ...r....r......_
-00000760: 7365 7475 705f 6669 6c65 5f67 656e 6572  setup_file_gener
-00000770: 6174 6f72 735f 636c 6173 7365 7344 0000  ators_classesD..
-00000780: 0073 1400 0000 0a02 0a01 0201 0201 12ff  .s..............
-00000790: 0a04 1001 0a02 1001 04ff 7a25 4f75 7470  ..........z%Outp
-000007a0: 7574 2e5f 7365 7475 705f 6669 6c65 5f67  ut._setup_file_g
-000007b0: 656e 6572 6174 6f72 735f 636c 6173 7365  enerators_classe
-000007c0: 7363 0300 0000 0000 0000 0000 0000 0400  sc..............
-000007d0: 0000 0600 0000 4300 0000 7372 0000 007c  ......C...sr...|
-000007e0: 00a0 00a1 0001 0074 017c 017c 027c 006a  .......t.|.|.|.j
-000007f0: 02a0 03a1 0083 0301 007c 01a0 0474 0564  .........|...t.d
-00000800: 0164 0264 038d 02a1 0101 007c 016a 0664  .d.d.......|.j.d
-00000810: 0464 0164 0564 069c 0264 078d 0201 007c  .d.d.d...d.....|
-00000820: 016a 07a0 0874 09a0 0a64 08a1 01a1 0101  .j...t...d......
-00000830: 007c 026a 0b6a 0ca0 0da1 007d 0374 017c  .|.j.j.....}.t.|
-00000840: 017c 027c 03a0 03a1 0083 0301 0064 0953  .|.|.........d.S
-00000850: 0029 0a7a 3e54 6869 7320 7374 6174 6963  .).z>This static
-00000860: 206d 6574 686f 6420 6973 2075 7365 6420   method is used 
-00000870: 746f 2063 6f6d 706c 6574 6520 7468 6520  to complete the 
-00000880: 2a70 6172 616d 732a 2063 6f6e 7461 696e  *params* contain
-00000890: 6572 2e54 da03 7275 6e29 02da 0f4e 4557  er.T..run)...NEW
-000008a0: 5f44 4952 5f52 4553 554c 5453 5a13 7368  _DIR_RESULTSZ.sh
-000008b0: 6f72 745f 6e61 6d65 5f74 7970 655f 7275  ort_name_type_ru
-000008c0: 6eda 066f 7574 7075 74da 0029 02da 0b48  n..output..)...H
-000008d0: 4153 5f54 4f5f 5341 5645 da0d 7375 625f  AS_TO_SAVE..sub_
-000008e0: 6469 7265 6374 6f72 7929 01da 0761 7474  directory)...att
-000008f0: 7269 6273 612e 0100 000a 2020 2020 2d20  ribsa.....    - 
-00000900: 6060 4841 535f 544f 5f53 4156 4560 603a  ``HAS_TO_SAVE``:
-00000910: 2062 6f6f 6c20 2864 6566 6175 6c74 3a20   bool (default: 
-00000920: 5472 7565 2920 4966 2046 616c 7365 2c20  True) If False, 
-00000930: 6e6f 7468 696e 6720 6e65 7720 6973 2073  nothing new is s
-00000940: 6176 6564 2069 6e0a 2020 2020 2020 7468  aved in.      th
-00000950: 6520 6469 7265 6374 6f72 7920 6f66 2074  e directory of t
-00000960: 6865 2073 696d 756c 6174 696f 6e2e 0a20  he simulation.. 
-00000970: 2020 202d 2060 6073 7562 5f64 6972 6563     - ``sub_direc
-00000980: 746f 7279 6060 3a20 7374 7220 2864 6566  tory``: str (def
-00000990: 6175 6c74 3a20 2222 2920 4120 6e61 6d65  ault: "") A name
-000009a0: 206f 6620 6120 7375 622d 6469 7265 6374   of a sub-direct
-000009b0: 6f72 7920 2872 656c 6174 6976 650a 2020  ory (relative.  
-000009c0: 2020 2020 746f 2024 464c 5549 4444 594e      to $FLUIDDYN
-000009d0: 5f50 4154 485f 5343 5241 5443 4829 2077  _PATH_SCRATCH) w
-000009e0: 6865 7265 696e 2074 6865 2064 6972 6563  herein the direc
-000009f0: 746f 7279 206f 6620 7468 6520 7369 6d75  tory of the simu
-00000a00: 6c61 7469 6f6e 0a20 2020 2020 2028 6060  lation.      (``
-00000a10: 7061 7468 5f72 756e 6060 2920 6973 2073  path_run``) is s
-00000a20: 6176 6564 2e0a 0a4e 290e 722e 0000 0072  aved...N).r....r
-00000a30: 0800 0000 7228 0000 00da 0676 616c 7565  ....r(.....value
-00000a40: 73da 0c5f 7365 745f 6174 7472 6962 7372  s.._set_attribsr
-00000a50: 2300 0000 7219 0000 0072 3100 0000 da08  #...r....r1.....
-00000a60: 5f73 6574 5f64 6f63 da08 7465 7874 7772  _set_doc..textwr
-00000a70: 6170 da06 6465 6465 6e74 7218 0000 0072  ap..dedentr....r
-00000a80: 1100 0000 da0e 696d 706f 7274 5f63 6c61  ......import_cla
-00000a90: 7373 6573 2904 721c 0000 00da 0670 6172  sses).r......par
-00000aa0: 616d 7372 1d00 0000 da0c 6469 6374 5f63  amsr......dict_c
-00000ab0: 6c61 7373 6573 721e 0000 0072 1e00 0000  lassesr....r....
-00000ac0: 721f 0000 00da 1d5f 636f 6d70 6c65 7465  r......_complete
-00000ad0: 5f70 6172 616d 735f 7769 7468 5f64 6566  _params_with_def
-00000ae0: 6175 6c74 5200 0000 731e 0000 0008 0402  aultR...s.......
-00000af0: 010c 0104 ff12 0504 010a 0106 ff06 0304  ................
-00000b00: 0102 0102 ff04 ff0c 0d14 017a 244f 7574  ...........z$Out
-00000b10: 7075 742e 5f63 6f6d 706c 6574 655f 7061  put._complete_pa
-00000b20: 7261 6d73 5f77 6974 685f 6465 6661 756c  rams_with_defaul
-00000b30: 744e 6303 0000 0000 0000 0000 0000 000b  tNc.............
-00000b40: 0000 0008 0000 0003 0000 0073 3c02 0000  ...........s<...
-00000b50: 7c01 7c00 5f00 7a08 7c01 6a01 6a02 6a03  |.|._.z.|.j.j.j.
-00000b60: 7c00 5f04 5700 6e09 0400 7405 7914 0100  |._.W.n...t.y...
-00000b70: 0100 0100 5900 6e07 7700 7406 7c00 6a04  ....Y.n.w.t.|.j.
-00000b80: 8301 7c00 5f07 7c00 a008 a100 7c00 5f09  ..|._.|.....|._.
-00000b90: 7c01 722e 7c01 6a0a 6a0b 7c00 5f0a 740c  |.r.|.j.j.|._.t.
-00000ba0: 8300 a00d 7c01 a101 0100 6e0f 7c02 7235  ....|.....n.|.r5
-00000bb0: 7c02 6a0b 7c00 5f0a 6e08 6400 7c00 5f0a  |.j.|._.n.d.|._.
-00000bc0: 740e a00f 6401 a101 0100 7c01 7341 6400  t...d.....|.sAd.
-00000bd0: 5300 7410 7c00 6a11 8301 7c00 5f11 7412  S.t.|.j...|._.t.
-00000be0: 7c00 8301 7c00 5f13 7c01 6a01 6a02 6a14  |...|._.|.j.j.j.
-00000bf0: 6a15 a016 a100 7d03 7c03 a017 a100 4400  j.....}.|.....D.
-00000c00: 5d26 5c02 7d04 7d05 7418 7c00 7c05 8302  ]&\.}.}.t.|.|...
-00000c10: 7262 7158 7419 7c04 8301 7d06 7c00 6a00  rbqXt.|...}.|.j.
-00000c20: 0400 6a1a 6402 a01b 6403 7c06 9b00 6404  ..j.d...d.|...d.
-00000c30: 9d03 7c05 a102 3700 0200 5f1a 741c 7c00  ..|...7..._.t.|.
-00000c40: 7c06 7c05 7c00 8301 8303 0100 7158 741d  |.|.|.......qXt.
-00000c50: 7c00 6405 8302 7388 7c00 a01e a100 0100  |.d...s.|.......
-00000c60: 6900 7d07 7c00 6a1f a017 a100 4400 5d25  i.}.|.j.....D.]%
-00000c70: 5c02 7d04 7d05 7419 7c04 8301 7d06 7c05  \.}.}.t.|...}.|.
-00000c80: 6a20 7c07 7601 72a3 7c04 6701 7c07 7c05  j |.v.r.|.g.|.|.
-00000c90: 6a20 3c00 6e08 7c07 7c05 6a20 1900 a021  j <.n.|.|.j ...!
-00000ca0: 7c04 a101 0100 741c 7c00 6a13 7c06 7c05  |.....t.|.j.|.|.
-00000cb0: 7c00 8301 8303 0100 718f 7c07 72dc 7c00  |.......q.|.r.|.
-00000cc0: 6a00 0400 6a1a 6406 3700 0200 5f1a 7c07  j...j.d.7..._.|.
-00000cd0: a017 a100 4400 5d18 5c02 7d08 7d09 7c00  ....D.].\.}.}.|.
-00000ce0: 6a00 0400 6a1a 6407 7c08 6408 1700 6409  j...j.d.|.d...d.
-00000cf0: 9b04 640a a022 7c09 a101 9b00 640b 9d04  ..d.."|.....d...
-00000d00: 3700 0200 5f1a 71c3 7423 6a24 640c 6b02  7..._.q.t#j$d.k.
-00000d10: 72e9 7c00 6a25 72e9 7c00 6a00 6a0a 6a26  r.|.j%r.|.j.j.j&
-00000d20: 73eb 6400 5300 7c00 6a11 640d 1b00 a027  s.d.S.|.j.d....'
-00000d30: a100 0100 7c00 6a11 640e 1b00 a027 a100  ....|.j.d....'..
-00000d40: 0100 7c00 6a11 640f 1b00 a027 a100 0100  ..|.j.d....'....
-00000d50: 7428 7c00 6a13 8301 a029 a100 4400 5d14  t(|.j....)..D.].
-00000d60: 7d0a 741d 7c0a 6410 8302 9001 721a 7c0a  }.t.|.d.....r.|.
-00000d70: 6a2a a02b 640d a101 9001 721a 7c0a a02c  j*.+d.....r.|..,
-00000d80: a100 0100 9001 7107 6400 5300 2911 4e7a  ......q.d.S.).Nz
-00000d90: 4549 6e69 7469 616c 697a 696e 6720 4f75  EInitializing Ou
-00000da0: 7470 7574 2063 6c61 7373 2077 6974 686f  tput class witho
-00000db0: 7574 2073 696d 206f 7220 7061 7261 6d73  ut sim or params
-00000dc0: 206d 6967 6874 206c 6561 6420 746f 2065   might lead to e
-00000dd0: 7272 6f72 732e 7a09 7b3a 3238 737d 7b7d  rrors.z.{:28s}{}
-00000de0: 0a7a 0b73 696d 2e6f 7574 7075 742e 7a02  .z.sim.output.z.
-00000df0: 3a20 7228 0000 007a 0d69 6e70 7574 5f66  : r(...z.input_f
-00000e00: 696c 6573 3a0a 7a07 2020 2d20 696e 20fa  iles:.z.  - in .
-00000e10: 013a 5a03 3132 73da 0120 da01 0a72 0100  .:Z.12s.. ...r..
-00000e20: 0000 7227 0000 00da 0130 7226 0000 00da  ..r'.....0r&....
-00000e30: 0d67 656e 6572 6174 655f 6669 6c65 292d  .generate_file)-
-00000e40: da03 7369 6dda 0469 6e66 6fda 0673 6f6c  ..sim..info..sol
-00000e50: 7665 72da 0a73 686f 7274 5f6e 616d 65da  ver..short_name.
-00000e60: 0b6e 616d 655f 736f 6c76 6572 da0e 4174  .name_solver..At
-00000e70: 7472 6962 7574 6545 7272 6f72 7210 0000  tributeErrorr...
-00000e80: 00da 0770 6163 6b61 6765 da17 6765 745f  ...package..get_
-00000e90: 7061 7468 5f73 6f6c 7665 725f 7061 636b  path_solver_pack
-00000ea0: 6167 655a 1370 6174 685f 736f 6c76 6572  ageZ.path_solver
-00000eb0: 5f70 6163 6b61 6765 723c 0000 0072 3100  _packager<...r1.
-00000ec0: 0000 da05 7375 7065 72da 085f 5f69 6e69  ....super..__ini
-00000ed0: 745f 5f72 0f00 0000 da07 7761 726e 696e  t__r......warnin
-00000ee0: 6772 0200 0000 da08 7061 7468 5f72 756e  gr......path_run
-00000ef0: 720d 0000 00da 0b69 6e70 7574 5f66 696c  r......input_fil
-00000f00: 6573 7218 0000 0072 1100 0000 723b 0000  esr....r....r;..
-00000f10: 00da 0569 7465 6d73 da0a 6973 696e 7374  ...items..isinst
-00000f20: 616e 6365 7204 0000 00da 115f 6f62 6a65  ancer......_obje
-00000f30: 6374 735f 746f 5f70 7269 6e74 da06 666f  cts_to_print..fo
-00000f40: 726d 6174 da07 7365 7461 7474 72da 0768  rmat..setattr..h
-00000f50: 6173 6174 7472 722e 0000 0072 2800 0000  asattrr....r(...
-00000f60: da08 6469 725f 6e61 6d65 da06 6170 7065  ..dir_name..appe
-00000f70: 6e64 da04 6a6f 696e 7206 0000 00da 0472  nd..joinr......r
-00000f80: 616e 6bda 0c5f 6861 735f 746f 5f73 6176  ank.._has_to_sav
-00000f90: 6572 3000 0000 da05 6d6b 6469 72da 0476  er0.....mkdir..v
-00000fa0: 6172 7372 3600 0000 da08 7265 6c5f 7061  arsr6.....rel_pa
-00000fb0: 7468 da0a 7374 6172 7473 7769 7468 7243  th..startswithrC
-00000fc0: 0000 0029 0bda 0473 656c 6672 4400 0000  ...)...selfrD...
-00000fd0: 723c 0000 0072 3d00 0000 da08 636c 735f  r<...r=.....cls_
-00000fe0: 6e61 6d65 da05 436c 6173 73da 086f 626a  name..Class..obj
-00000ff0: 5f6e 616d 655a 1366 6f72 5f73 7472 5f69  _nameZ.for_str_i
-00001000: 6e70 7574 5f66 696c 6573 7257 0000 0072  nput_filesrW...r
-00001010: 5000 0000 da0e 6669 6c65 5f67 656e 6572  P.....file_gener
-00001020: 6174 6f72 a901 da09 5f5f 636c 6173 735f  ator....__class_
-00001030: 5f72 1e00 0000 721f 0000 0072 4d00 0000  _r....r....rM...
-00001040: 7000 0000 7380 0000 0006 0102 0110 010c  p...s...........
-00001050: 0104 0102 ff0c 030a 0204 020a 020e 0104  ................
-00001060: 010a 0206 0204 0102 0104 ff04 0404 010c  ................
-00001070: 020a 0210 0210 010a 0102 0108 010c 010c  ................
-00001080: 0108 ff12 030a 0208 0104 0112 0108 010a  ................
-00001090: 020e 0110 0214 0104 0210 0110 0108 011a  ................
-000010a0: 0108 ff08 0502 ff04 0202 fe08 0302 fd04  ................
-000010b0: 050e 020e 010e 0112 0202 0104 0106 ff0a  ................
-000010c0: 0204 fe08 0304 8004 fc7a 0f4f 7574 7075  .........z.Outpu
-000010d0: 742e 5f5f 696e 6974 5f5f 6301 0000 0000  t.__init__c.....
-000010e0: 0000 0000 0000 0001 0000 0004 0000 0043  ...............C
-000010f0: 0000 0073 1200 0000 7400 7401 a002 7c00  ...s....t.t...|.
-00001100: a101 6a03 8301 6a04 5300 2901 7a28 4765  ..j...j.S.).z(Ge
-00001110: 7420 7468 6520 7061 7468 2074 6f77 6172  t the path towar
-00001120: 6473 2074 6865 2073 6f6c 7665 7220 7061  ds the solver pa
-00001130: 636b 6167 652e 2905 7202 0000 00da 0769  ckage.).r......i
-00001140: 6e73 7065 6374 da09 6765 746d 6f64 756c  nspect..getmodul
-00001150: 65da 085f 5f66 696c 655f 5fda 0670 6172  e..__file__..par
-00001160: 656e 7429 0172 1c00 0000 721e 0000 0072  ent).r....r....r
-00001170: 1e00 0000 721f 0000 0072 4b00 0000 bd00  ....r....rK.....
-00001180: 0000 7302 0000 0012 037a 1e4f 7574 7075  ..s......z.Outpu
-00001190: 742e 6765 745f 7061 7468 5f73 6f6c 7665  t.get_path_solve
-000011a0: 725f 7061 636b 6167 6563 0100 0000 0000  r_packagec......
-000011b0: 0000 0000 0000 0500 0000 0800 0000 0300  ................
-000011c0: 0000 73c8 0000 0074 006a 0164 016b 0272  ..s....t.j.d.k.r
-000011d0: 0d74 0264 027c 006a 039b 009d 0283 0101  .t.d.|.j........
-000011e0: 0074 0483 008f 0d01 0074 0583 00a0 06a1  .t.......t......
-000011f0: 0001 0057 0064 0304 0004 0083 0301 006e  ...W.d.........n
-00001200: 0831 0073 2077 0101 0001 0001 0059 0001  .1.s w.......Y..
-00001210: 0074 07a0 087c 006a 096a 0aa1 0101 0074  .t...|.j.j.....t
-00001220: 006a 0164 016b 0272 3d7c 006a 0b72 3d7c  .j.d.k.r=|.j.r=|
-00001230: 006a 096a 0c6a 0d72 3d7c 00a0 0ea1 0001  .j.j.j.r=|......
-00001240: 0074 0f7c 006a 0383 017d 017c 0164 041b  .t.|.j...}.|.d..
-00001250: 007d 027c 026a 1064 0564 068d 0101 0064  .}.|.j.d.d.....d
-00001260: 0744 005d 137d 037c 027c 031b 007d 047c  .D.].}.|.|...}.|
-00001270: 04a0 11a1 0072 5971 4e74 12a0 137c 017c  .....rYqNt...|.|
-00001280: 031b 007c 04a1 0201 0071 4e64 0353 0029  ...|.....qNd.S.)
-00001290: 087a 214c 6f67 7320 696e 666f 206f 6e20  .z!Logs info on 
-000012a0: 696e 7374 616e 7469 6174 6564 2063 6c61  instantiated cla
-000012b0: 7373 6573 7201 0000 007a 0a70 6174 685f  ssesr....z.path_
-000012c0: 7275 6e3a 204e 7a0e 2e64 6174 615f 666c  run: Nz..data_fl
-000012d0: 7569 6473 696d 5429 01da 0865 7869 7374  uidsimT)...exist
-000012e0: 5f6f 6b29 027a 0f69 6e66 6f5f 736f 6c76  _ok).z.info_solv
-000012f0: 6572 2e78 6d6c 7a10 7061 7261 6d73 5f73  er.xmlz.params_s
-00001300: 696d 756c 2e78 6d6c 2914 7206 0000 0072  imul.xml).r....r
-00001310: 5a00 0000 da05 7072 696e 7472 4f00 0000  Z.....printrO...
-00001320: 7205 0000 0072 4c00 0000 da09 706f 7374  r....rL.....post
-00001330: 5f69 6e69 7472 0f00 0000 7245 0000 0072  _initr....rE...r
-00001340: 4400 0000 7253 0000 0072 5b00 0000 723c  D...rS...r[...r<
-00001350: 0000 0072 3000 0000 da28 706f 7374 5f69  ...r0....(post_i
-00001360: 6e69 745f 6372 6561 7465 5f61 6464 6974  nit_create_addit
-00001370: 696f 6e61 6c5f 736f 7572 6365 5f66 696c  ional_source_fil
-00001380: 6573 7202 0000 0072 5c00 0000 da06 6578  esr....r\.....ex
-00001390: 6973 7473 da06 7368 7574 696c da04 636f  ists..shutil..co
-000013a0: 7079 2905 7260 0000 0072 4f00 0000 5a12  py).r`...rO...Z.
-000013b0: 7061 7468 5f69 6e66 6f5f 666c 7569 6473  path_info_fluids
-000013c0: 696d 722d 0000 005a 0870 6174 685f 6e65  imr-...Z.path_ne
-000013d0: 7772 6500 0000 721e 0000 0072 1f00 0000  wre...r....r....
-000013e0: 726d 0000 00c2 0000 0073 2c00 0000 0a03  rm.......s,.....
-000013f0: 1001 0803 0c01 1cff 0e03 0804 02ff 0402  ................
-00001400: 02fe 0803 02fd 0805 0a03 0801 0c01 0801  ................
-00001410: 0801 0801 0201 1201 04fc 7a10 4f75 7470  ..........z.Outp
-00001420: 7574 2e70 6f73 745f 696e 6974 6301 0000  ut.post_initc...
-00001430: 0000 0000 0000 0000 0003 0000 0004 0000  ................
-00001440: 0043 0000 0073 6c00 0000 7c00 6a00 6a01  .C...sl...|.j.j.
-00001450: 6401 1b00 7d01 7c01 a002 a100 7313 7403  d...}.|.....s.t.
-00001460: 6402 7c00 6a00 6a01 9b00 9d02 8301 8201  d.|.j.j.........
-00001470: 7404 a005 7c01 7c00 6a06 6a07 a102 0100  t...|.|.j.j.....
-00001480: 7408 7c00 6a00 8301 a009 a100 4400 5d11  t.|.j.......D.].
-00001490: 7d02 740a 7c02 6403 8302 7233 7c02 6a0b  }.t.|.d...r3|.j.
-000014a0: a00c 6404 a101 7333 7c02 a00d a100 0100  ..d...s3|.......
-000014b0: 7122 6405 5300 2906 7a24 4372 6561 7465  q"d.S.).z$Create
-000014c0: 2074 6865 2066 696c 6573 2066 726f 6d20   the files from 
-000014d0: 7468 6569 7220 7465 6d70 6c61 7465 7a08  their templatez.
-000014e0: 7461 736b 732e 7079 7a29 7461 736b 732e  tasks.pyz)tasks.
-000014f0: 7079 206d 6973 7369 6e67 2069 6e20 736f  py missing in so
-00001500: 6c76 6572 2074 656d 706c 6174 6573 5f64  lver templates_d
-00001510: 6972 2072 4300 0000 7227 0000 004e 290e  ir rC...r'...N).
-00001520: 7250 0000 005a 0d74 656d 706c 6174 6573  rP...Z.templates
-00001530: 5f64 6972 726f 0000 00da 0c52 756e 7469  _dirro.....Runti
-00001540: 6d65 4572 726f 7272 7000 0000 7271 0000  meErrorrp...rq..
-00001550: 0072 4400 0000 724f 0000 0072 5d00 0000  .rD...rO...r]...
-00001560: 7236 0000 0072 5600 0000 725e 0000 0072  r6...rV...r^...r
-00001570: 5f00 0000 7243 0000 0029 0372 6000 0000  _...rC...).r`...
-00001580: 5a0d 7061 7468 5f74 6173 6b73 5f70 7972  Z.path_tasks_pyr
-00001590: 6400 0000 721e 0000 0072 1e00 0000 721f  d...r....r....r.
-000015a0: 0000 0072 6e00 0000 e000 0000 7322 0000  ...rn.......s"..
-000015b0: 000c 0208 0102 0102 0106 0104 ff04 ff10  ................
-000015c0: 0412 0202 0104 0104 ff0a 0202 fe08 0402  ................
-000015d0: 8004 fb7a 2f4f 7574 7075 742e 706f 7374  ...z/Output.post
-000015e0: 5f69 6e69 745f 6372 6561 7465 5f61 6464  _init_create_add
-000015f0: 6974 696f 6e61 6c5f 736f 7572 6365 5f66  itional_source_f
-00001600: 696c 6573 6302 0000 0000 0000 0000 0000  ilesc...........
-00001610: 0003 0000 0005 0000 0043 0000 0073 2800  .........C...s(.
-00001620: 0000 6401 6402 8400 7c00 6a00 a001 a100  ..d.d...|.j.....
-00001630: 4400 8301 7d02 7c01 6a02 6403 7c02 6404  D...}.|.j.d.|.d.
-00001640: 6405 8d03 0100 6400 5300 2906 4e63 0100  d.....d.S.).Nc..
-00001650: 0000 0000 0000 0000 0000 0300 0000 0400  ................
-00001660: 0000 5300 0000 731a 0000 0069 007c 005d  ..S...s....i.|.]
-00001670: 095c 027d 017d 0274 007c 0183 017c 0293  .\.}.}.t.|...|..
-00001680: 0271 0253 0072 1e00 0000 7203 0000 0029  .q.S.r....r....)
-00001690: 03da 022e 30da 036b 6579 da05 7661 6c75  ....0..key..valu
-000016a0: 6572 1e00 0000 721e 0000 0072 1f00 0000  er....r....r....
-000016b0: da0a 3c64 6963 7463 6f6d 703e f300 0000  ..<dictcomp>....
-000016c0: 7308 0000 0006 0006 0208 ff06 ff7a 384f  s............z8O
-000016d0: 7574 7075 742e 5f63 6f6d 706c 6574 655f  utput._complete_
-000016e0: 7061 7261 6d73 5f63 6f6e 7472 6f6c 5f64  params_control_d
-000016f0: 6963 742e 3c6c 6f63 616c 733e 2e3c 6469  ict.<locals>.<di
-00001700: 6374 636f 6d70 3eda 0c63 6f6e 7472 6f6c  ctcomp>..control
-00001710: 5f64 6963 747a 3d53 6565 2068 7474 7073  _dictz=See https
-00001720: 3a2f 2f64 6f63 2e63 6664 2e64 6972 6563  ://doc.cfd.direc
-00001730: 742f 6f70 656e 666f 616d 2f75 7365 722d  t/openfoam/user-
-00001740: 6775 6964 652d 7636 2f63 6f6e 7472 6f6c  guide-v6/control
-00001750: 6469 6374 a902 7235 0000 00da 0364 6f63  dict..r5.....doc
-00001760: 2903 da1b 6465 6661 756c 745f 636f 6e74  )...default_cont
-00001770: 726f 6c5f 6469 6374 5f70 6172 616d 7372  rol_dict_paramsr
-00001780: 5100 0000 7219 0000 0029 0372 1c00 0000  Q...r....).r....
-00001790: 723c 0000 0072 3500 0000 721e 0000 0072  r<...r5...r....r
-000017a0: 1e00 0000 721f 0000 00da 1d5f 636f 6d70  ....r......_comp
-000017b0: 6c65 7465 5f70 6172 616d 735f 636f 6e74  lete_params_cont
-000017c0: 726f 6c5f 6469 6374 f100 0000 7310 0000  rol_dict....s...
-000017d0: 0006 0208 0206 fe04 0502 0102 0102 010a  ................
-000017e0: fd7a 244f 7574 7075 742e 5f63 6f6d 706c  .z$Output._compl
-000017f0: 6574 655f 7061 7261 6d73 5f63 6f6e 7472  ete_params_contr
-00001800: 6f6c 5f64 6963 7463 0200 0000 0000 0000  ol_dictc........
-00001810: 0000 0000 0400 0000 0700 0000 0300 0000  ................
-00001820: 7336 0000 0087 0066 0164 0164 0284 087c  s6.....f.d.d...|
-00001830: 006a 00a0 01a1 0044 0083 017d 0274 0264  .j.....D...}.t.d
-00001840: 0364 0464 0564 0664 0764 089c 057c 0274  .d.d.d.d.d...|.t
-00001850: 0364 098d 037d 037c 0353 0029 0a4e 6301  .d...}.|.S.).Nc.
-00001860: 0000 0000 0000 0000 0000 0002 0000 0006  ................
-00001870: 0000 0013 0000 0073 1c00 0000 6900 7c00  .......s....i.|.
-00001880: 5d0a 7d01 7c01 8800 6a00 7401 7c01 8301  ].}.|...j.t.|...
-00001890: 1900 9302 7102 5300 721e 0000 0029 0272  ....q.S.r....).r
-000018a0: 7700 0000 7204 0000 0029 0272 7300 0000  w...r....).rs...
-000018b0: 7274 0000 00a9 0172 3c00 0000 721e 0000  rt.....r<...r...
-000018c0: 0072 1f00 0000 7276 0000 00ff 0000 0073  .r....rv.......s
-000018d0: 0800 0000 0600 0202 0eff 06ff 7a31 4f75  ............z1Ou
-000018e0: 7470 7574 2e6d 616b 655f 7472 6565 5f63  tput.make_tree_c
-000018f0: 6f6e 7472 6f6c 5f64 6963 742e 3c6c 6f63  ontrol_dict.<loc
-00001900: 616c 733e 2e3c 6469 6374 636f 6d70 3e7a  als>.<dictcomp>z
-00001910: 0332 2e30 da05 6173 6369 69da 0a64 6963  .2.0..ascii..dic
-00001920: 7469 6f6e 6172 797a 0822 7379 7374 656d  tionaryz."system
-00001930: 2272 1500 0000 2905 da07 7665 7273 696f  "r....)...versio
-00001940: 6e72 5400 0000 da05 636c 6173 73da 086c  nrT.....class..l
-00001950: 6f63 6174 696f 6eda 066f 626a 6563 7429  ocation..object)
-00001960: 0372 4500 0000 da08 6368 696c 6472 656e  .rE.....children
-00001970: da06 6865 6164 6572 2904 727a 0000 00da  ..header).rz....
-00001980: 046b 6579 7372 0c00 0000 720a 0000 0029  .keysr....r....)
-00001990: 0472 6000 0000 723c 0000 0072 8300 0000  .r`...r<...r....
-000019a0: da04 7472 6565 721e 0000 0072 7c00 0000  ..treer....r|...
-000019b0: 721f 0000 00da 166d 616b 655f 7472 6565  r......make_tree
-000019c0: 5f63 6f6e 7472 6f6c 5f64 6963 74fe 0000  _control_dict...
-000019d0: 0073 1c00 0000 0a01 0802 06fe 0205 0202  .s..............
-000019e0: 0201 0201 0201 0201 04fb 0207 0201 06f7  ................
-000019f0: 040b 7a1d 4f75 7470 7574 2e6d 616b 655f  ..z.Output.make_
-00001a00: 7472 6565 5f63 6f6e 7472 6f6c 5f64 6963  tree_control_dic
-00001a10: 7463 0200 0000 0000 0000 0000 0000 0300  tc..............
-00001a20: 0000 0300 0000 4300 0000 7312 0000 007c  ......C...s....|
-00001a30: 00a0 007c 01a1 017d 027c 02a0 01a1 0053  ...|...}.|.....S
-00001a40: 0029 014e 2902 7287 0000 00da 0464 756d  .).N).r......dum
-00001a50: 7029 0372 6000 0000 723c 0000 0072 8600  p).r`...r<...r..
-00001a60: 0000 721e 0000 0072 1e00 0000 721f 0000  ..r....r....r...
-00001a70: 00da 166d 616b 655f 636f 6465 5f63 6f6e  ...make_code_con
-00001a80: 7472 6f6c 5f64 6963 7411 0100 0073 0400  trol_dict....s..
-00001a90: 0000 0a01 0801 7a1d 4f75 7470 7574 2e6d  ......z.Output.m
-00001aa0: 616b 655f 636f 6465 5f63 6f6e 7472 6f6c  ake_code_control
-00001ab0: 5f64 6963 7463 0200 0000 0000 0000 0000  _dictc..........
-00001ac0: 0000 0300 0000 0800 0000 4300 0000 7328  ..........C...s(
-00001ad0: 0000 0064 0164 0164 0164 0264 0264 0264  ...d.d.d.d.d.d.d
-00001ae0: 0364 049c 077d 027c 016a 0064 057c 0264  .d...}.|.j.d.|.d
-00001af0: 0664 078d 0301 0064 0053 0029 084e e928  .d.....d.S.).N.(
-00001b00: 0000 0067 0000 0000 0000 f03f e901 0000  ...g.......?....
-00001b10: 0029 07da 026e 78da 026e 79da 026e 7ada  .)...nx..ny..nz.
-00001b20: 026c 78da 026c 79da 026c 7ada 0573 6361  .lx..ly..lz..sca
-00001b30: 6c65 da0f 626c 6f63 6b5f 6d65 7368 5f64  le..block_mesh_d
-00001b40: 6963 74da 0454 4f44 4f72 7800 0000 2901  ict..TODOrx...).
-00001b50: 7219 0000 0029 0372 1c00 0000 723c 0000  r....).r....r<..
-00001b60: 00da 0764 6566 6175 6c74 721e 0000 0072  ...defaultr....r
-00001b70: 1e00 0000 721f 0000 00da 205f 636f 6d70  ....r..... _comp
-00001b80: 6c65 7465 5f70 6172 616d 735f 626c 6f63  lete_params_bloc
-00001b90: 6b5f 6d65 7368 5f64 6963 7415 0100 0073  k_mesh_dict....s
-00001ba0: 1a00 0000 0203 0201 0201 0201 0201 0201  ................
-00001bb0: 0201 06f9 040a 0201 0201 0201 0afd 7a27  ..............z'
-00001bc0: 4f75 7470 7574 2e5f 636f 6d70 6c65 7465  Output._complete
-00001bd0: 5f70 6172 616d 735f 626c 6f63 6b5f 6d65  _params_block_me
-00001be0: 7368 5f64 6963 7429 024e 4e29 18da 085f  sh_dict).NN)..._
-00001bf0: 5f6e 616d 655f 5fda 0a5f 5f6d 6f64 756c  _name__..__modul
-00001c00: 655f 5fda 0c5f 5f71 7561 6c6e 616d 655f  e__..__qualname_
-00001c10: 5f72 2900 0000 722b 0000 0072 2c00 0000  _r)...r+...r,...
-00001c20: 7209 0000 0072 7a00 0000 720b 0000 005a  r....rz...r....Z
-00001c30: 1c68 656c 7065 725f 7475 7262 756c 656e  .helper_turbulen
-00001c40: 6365 5f70 726f 7065 7274 6965 73da 0b63  ce_properties..c
-00001c50: 6c61 7373 6d65 7468 6f64 7220 0000 0072  lassmethodr ...r
-00001c60: 1a00 0000 722e 0000 0072 3e00 0000 724d  ....r....r>...rM
-00001c70: 0000 0072 4b00 0000 726d 0000 0072 6e00  ...rK...rm...rn.
-00001c80: 0000 727b 0000 0072 8700 0000 7289 0000  ..r{...r....r...
-00001c90: 0072 9600 0000 da0d 5f5f 636c 6173 7363  .r......__classc
-00001ca0: 656c 6c5f 5f72 1e00 0000 721e 0000 0072  ell__r....r....r
-00001cb0: 6500 0000 721f 0000 0072 1100 0000 1a00  e...r....r......
-00001cc0: 0000 7336 0000 0008 0008 0108 0108 0104  ..s6............
-00001cd0: 0102 0208 0104 ff02 040a 0102 0a0a 0102  ................
-00001ce0: 140a 0102 0d0a 010e 1d02 4d0a 010c 0408  ..........M.....
-00001cf0: 1e02 110a 0108 0c08 1302 0412 0172 1100  .............r..
-00001d00: 0000 291c 7267 0000 0072 7000 0000 7239  ..).rg...rp...r9
-00001d10: 0000 00da 0770 6174 686c 6962 7202 0000  .....pathlibr...
-00001d20: 00da 0a69 6e66 6c65 6374 696f 6e72 0400  ...inflectionr..
-00001d30: 0000 5a0b 666c 7569 6464 796e 2e69 6f72  ..Z.fluiddyn.ior
-00001d40: 0500 0000 5a0d 666c 7569 6464 796e 2e75  ....Z.fluiddyn.u
-00001d50: 7469 6c72 0600 0000 5a14 666c 7569 6473  tilr....Z.fluids
-00001d60: 696d 5f63 6f72 652e 6f75 7470 7574 7207  im_core.outputr.
-00001d70: 0000 00da 1466 6c75 6964 7369 6d5f 636f  .....fluidsim_co
-00001d80: 7265 2e70 6172 616d 7372 0800 0000 da1d  re.paramsr......
-00001d90: 666c 7569 6473 696d 666f 616d 2e66 6f61  fluidsimfoam.foa
-00001da0: 6d5f 696e 7075 745f 6669 6c65 7372 0900  m_input_filesr..
-00001db0: 0000 720a 0000 0072 0b00 0000 720c 0000  ..r....r....r...
-00001dc0: 005a 2866 6c75 6964 7369 6d66 6f61 6d2e  .Z(fluidsimfoam.
-00001dd0: 666f 616d 5f69 6e70 7574 5f66 696c 6573  foam_input_files
-00001de0: 2e67 656e 6572 6174 6f72 7372 0d00 0000  .generatorsr....
-00001df0: 720e 0000 005a 1066 6c75 6964 7369 6d66  r....Z.fluidsimf
-00001e00: 6f61 6d2e 6c6f 6772 0f00 0000 da14 666c  oam.logr......fl
-00001e10: 7569 6473 696d 666f 616d 2e73 6f6c 7665  uidsimfoam.solve
-00001e20: 7273 7210 0000 0072 1100 0000 721e 0000  rsr....r....r...
-00001e30: 0072 1e00 0000 721e 0000 0072 1f00 0000  .r....r....r....
-00001e40: da08 3c6d 6f64 756c 653e 0100 0000 731c  ..<module>....s.
-00001e50: 0000 0008 0008 0108 010c 010c 020c 020c  ................
-00001e60: 010c 010c 0118 0110 060c 040c 0114 03    ...............
+00000020: 0004 0000 0040 0000 0073 d800 0000 6400  .....@...s....d.
+00000030: 5a00 6401 6402 6c01 5a02 6401 6402 6c03  Z.d.d.l.Z.d.d.l.
+00000040: 5a03 6401 6402 6c04 5a04 6401 6402 6c05  Z.d.d.l.Z.d.d.l.
+00000050: 5a05 6401 6402 6c06 5a06 6401 6403 6c07  Z.d.d.l.Z.d.d.l.
+00000060: 6d08 5a08 0100 6401 6404 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
+00000070: 0100 6401 6405 6c0b 6d0c 5a0c 0100 6401  ..d.d.l.m.Z...d.
+00000080: 6406 6c0d 6d0e 5a0e 0100 6401 6407 6c0f  d.l.m.Z...d.d.l.
+00000090: 6d10 5a10 0100 6401 6408 6c11 6d12 5a12  m.Z...d.d.l.m.Z.
+000000a0: 0100 6401 6409 6c13 6d14 5a14 0100 6401  ..d.d.l.m.Z...d.
+000000b0: 640a 6c15 6d16 5a16 6d17 5a17 6d18 5a18  d.l.m.Z.m.Z.m.Z.
+000000c0: 0100 6401 640b 6c19 6d1a 5a1a 6d1b 5a1b  ..d.d.l.m.Z.m.Z.
+000000d0: 0100 6401 640c 6c1c 6d1d 5a1d 0100 6401  ..d.d.l.m.Z...d.
+000000e0: 640d 6c1e 6d1f 5a1f 0100 640e 640f 8400  d.l.m.Z...d.d...
+000000f0: 5a20 4700 6410 6411 8400 6411 6512 8303  Z G.d.d...d.e...
+00000100: 5a21 6402 5300 2912 7a11 4261 7365 206f  Z!d.S.).z.Base o
+00000110: 7574 7075 7420 636c 6173 73e9 0000 0000  utput class.....
+00000120: 4e29 01da 0b6e 756c 6c63 6f6e 7465 7874  N)...nullcontext
+00000130: 2901 da04 5061 7468 2901 da0a 756e 6465  )...Path)...unde
+00000140: 7273 636f 7265 2901 da11 7374 646f 7574  rscore)...stdout
+00000150: 5f72 6564 6972 6563 7465 6429 01da 036d  _redirected)...m
+00000160: 7069 2901 da0a 4f75 7470 7574 436f 7265  pi)...OutputCore
+00000170: 2901 da14 6974 6572 5f63 6f6d 706c 6574  )...iter_complet
+00000180: 655f 7061 7261 6d73 2903 da12 436f 6e73  e_params)...Cons
+00000190: 7461 6e74 4669 6c65 4865 6c70 6572 da11  tantFileHelper..
+000001a0: 436f 6e74 726f 6c44 6963 7448 656c 7065  ControlDictHelpe
+000001b0: 72da 1644 6563 6f6d 706f 7365 5061 7244  r..DecomposeParD
+000001c0: 6963 7448 656c 7065 7229 02da 0a49 6e70  ictHelper)...Inp
+000001d0: 7574 4669 6c65 73da 186e 6577 5f66 696c  utFiles..new_fil
+000001e0: 655f 6765 6e65 7261 746f 725f 636c 6173  e_generator_clas
+000001f0: 7329 01da 066c 6f67 6765 7229 01da 1267  s)...logger)...g
+00000200: 6574 5f73 6f6c 7665 725f 7061 636b 6167  et_solver_packag
+00000210: 6563 0200 0000 0000 0000 0000 0000 0800  ec..............
+00000220: 0000 0900 0000 4300 0000 7338 0100 007c  ......C...s8...|
+00000230: 0064 0075 0072 0664 0053 0074 007c 0074  .d.u.r.d.S.t.|.t
+00000240: 0183 0272 0e7c 0067 017d 007c 0044 005d  ...r.|.g.}.|.D.]
+00000250: 897d 0274 017c 0283 017d 0264 017c 0276  .}.t.|...}.d.|.v
+00000260: 0072 2c7c 02a0 0264 01a1 015c 027d 027d  .r,|...d...\.}.}
+00000270: 037c 017c 03a0 03a1 001b 007d 047c 02a0  .|.|.......}.|..
+00000280: 03a1 007d 026e 027c 017d 047c 02a0 0464  ...}.n.|.}.|...d
+00000290: 02a1 0172 547c 02a0 0564 02a1 017d 027c  ...rT|...d...}.|
+000002a0: 02a0 0264 03a1 015c 027d 057d 037c 03a0  ...d...\.}.}.|..
+000002b0: 0564 04a1 017d 0374 066a 07a0 087c 05a1  .d...}.t.j...|..
+000002c0: 017d 067c 06a0 097c 03a1 017d 0274 066a  .}.|...|...}.t.j
+000002d0: 076a 0a7d 076e 0c74 0b74 0c6a 0da0 0e7c  .j.}.n.t.t.j...|
+000002e0: 02a1 0183 01a0 0fa1 007d 0274 107d 077c  .........}.t.}.|
+000002f0: 077c 0283 018f 2d7d 027c 02a0 11a1 0072  .|....-}.|.....r
+00000300: 7074 12a0 137c 027c 04a1 0201 006e 1a7c  pt...|.|.....n.|
+00000310: 02a0 14a1 0072 7e74 12a0 157c 027c 047c  .....r~t...|.|.|
+00000320: 026a 161b 00a1 0201 006e 0c74 1764 057c  .j.......n.t.d.|
+00000330: 029b 0264 067c 02a0 18a1 009b 029d 0483  ...d.|..........
+00000340: 0182 0157 0064 0004 0004 0083 0301 006e  ...W.d.........n
+00000350: 0831 0073 9477 0101 0001 0001 0059 0001  .1.s.w.......Y..
+00000360: 0071 1064 0053 0029 074e 7a02 2d3e 7a0d  .q.d.S.).Nz.->z.
+00000370: 7061 636b 6167 652d 6461 7461 28fa 0129  package-data(..)
+00000380: fa01 2f7a 0b72 6573 6f75 7263 6520 3d20  ../z.resource = 
+00000390: 7a16 2c20 7265 736f 7572 6365 2e65 7869  z., resource.exi
+000003a0: 7374 7328 2920 3d20 2919 da0a 6973 696e  sts() = )...isin
+000003b0: 7374 616e 6365 da03 7374 72da 0573 706c  stance..str..spl
+000003c0: 6974 da05 7374 7269 70da 0a73 7461 7274  it..strip..start
+000003d0: 7377 6974 68da 0c72 656d 6f76 6570 7265  swith..removepre
+000003e0: 6669 78da 0969 6d70 6f72 746c 6962 da09  fix..importlib..
+000003f0: 7265 736f 7572 6365 73da 0566 696c 6573  resources..files
+00000400: da08 6a6f 696e 7061 7468 5a07 6173 5f66  ..joinpathZ.as_f
+00000410: 696c 6572 0300 0000 da02 6f73 da04 7061  iler......os..pa
+00000420: 7468 da0a 6578 7061 6e64 7661 7273 da0a  th..expandvars..
+00000430: 6578 7061 6e64 7573 6572 7202 0000 00da  expanduserr.....
+00000440: 0769 735f 6669 6c65 da06 7368 7574 696c  .is_file..shutil
+00000450: da04 636f 7079 da06 6973 5f64 6972 da08  ..copy..is_dir..
+00000460: 636f 7079 7472 6565 da04 6e61 6d65 da13  copytree..name..
+00000470: 4e6f 7449 6d70 6c65 6d65 6e74 6564 4572  NotImplementedEr
+00000480: 726f 72da 0665 7869 7374 7329 0872 1900  ror..exists).r..
+00000490: 0000 da08 7061 7468 5f72 756e da08 7265  ....path_run..re
+000004a0: 736f 7572 6365 da0d 7265 6c61 7469 7665  source..relative
+000004b0: 5f70 6174 68da 0b64 6573 7469 6e61 7469  _path..destinati
+000004c0: 6f6e da0c 7061 636b 6167 655f 6e61 6d65  on..package_name
+000004d0: 5a10 6d75 6c74 6970 6c65 7865 645f 7061  Z.multiplexed_pa
+000004e0: 7468 da0f 636f 6e74 6578 745f 6d61 6e61  th..context_mana
+000004f0: 6765 72a9 0072 2e00 0000 fa3d 2f68 6f6d  ger..r.....=/hom
+00000500: 652f 7069 6572 7265 2f44 6576 2f66 6c75  e/pierre/Dev/flu
+00000510: 6964 7369 6d66 6f61 6d2f 7372 632f 666c  idsimfoam/src/fl
+00000520: 7569 6473 696d 666f 616d 2f6f 7574 7075  uidsimfoam/outpu
+00000530: 742f 6261 7365 2e70 79da 0e63 6f70 795f  t/base.py..copy_
+00000540: 7265 736f 7572 6365 731e 0000 0073 4000  resources....s@.
+00000550: 0000 0801 0401 0a01 0601 0802 0801 0801  ................
+00000560: 0e01 0c01 0a01 0402 0a02 0a01 0e01 0a01  ................
+00000570: 0c01 0a01 0a01 1402 0401 0a02 0801 0e01  ................
+00000580: 0801 1401 0202 1201 04ff 0280 1cfa 0280  ................
+00000590: 04ec 7230 0000 0063 0000 0000 0000 0000  ..r0...c........
+000005a0: 0000 0000 0000 0000 0400 0000 0000 0000  ................
+000005b0: 73b4 0000 0065 005a 0164 005a 0264 0164  s....e.Z.d.Z.d.d
+000005c0: 0267 025a 0364 0364 0467 025a 0467 0064  .g.Z.d.d.g.Z.g.d
+000005d0: 05a2 015a 0565 0664 0464 0664 0769 0183  ...Z.e.d.d.d.i..
+000005e0: 025a 0765 0883 005a 0965 0a83 005a 0b65  .Z.e...Z.e...Z.e
+000005f0: 0c64 0864 0984 0083 015a 0d65 0c64 0a64  .d.d.....Z.e.d.d
+00000600: 0b84 0083 015a 0e65 0c64 0c64 0d84 0083  .....Z.e.d.d....
+00000610: 015a 0f65 0c64 0e64 0f84 0083 015a 1064  .Z.e.d.d.....Z.d
+00000620: 1d87 0066 0164 1164 1284 095a 1165 0c64  ...f.d.d...Z.e.d
+00000630: 1364 1484 0083 015a 1287 0066 0164 1564  .d.....Z...f.d.d
+00000640: 1684 085a 1364 1764 1884 005a 1465 0c64  ...Z.d.d...Z.e.d
+00000650: 1964 1a84 0083 015a 1564 1b64 1c84 005a  .d.....Z.d.d...Z
+00000660: 1687 0004 005a 1753 0029 1eda 064f 7574  .....Z.S.)...Out
+00000670: 7075 74da 0170 da01 55da 1374 7261 6e73  put..p..U..trans
+00000680: 706f 7274 5072 6f70 6572 7469 6573 da14  portProperties..
+00000690: 7475 7262 756c 656e 6365 5072 6f70 6572  turbulenceProper
+000006a0: 7469 6573 2904 da0b 636f 6e74 726f 6c44  ties)...controlD
+000006b0: 6963 74da 0966 7653 6368 656d 6573 da0a  ict..fvSchemes..
+000006c0: 6676 536f 6c75 7469 6f6e da10 6465 636f  fvSolution..deco
+000006d0: 6d70 6f73 6550 6172 4469 6374 5a0e 7369  mposeParDictZ.si
+000006e0: 6d75 6c61 7469 6f6e 5479 7065 5a07 6c61  mulationTypeZ.la
+000006f0: 6d69 6e61 7263 0200 0000 0000 0000 0000  minarc..........
+00000700: 0000 0300 0000 0300 0000 4300 0000 7328  ..........C...s(
+00000710: 0000 007c 016a 006a 01a0 0264 01a1 017d  ...|.j.j...d...}
+00000720: 027c 00a0 037c 02a1 0101 007c 016a 006a  .|...|.....|.j.j
+00000730: 01a0 04a1 0001 0064 0253 0029 037a 6643  .......d.S.).zfC
+00000740: 6f6d 706c 6574 6520 7468 6520 696e 666f  omplete the info
+00000750: 5f73 6f6c 7665 7220 696e 7374 616e 6365  _solver instance
+00000760: 2077 6974 6820 6368 696c 6420 636c 6173   with child clas
+00000770: 7320 6465 7461 696c 7320 286d 6f64 756c  s details (modul
+00000780: 650a 2020 2020 2020 2020 616e 6420 636c  e.        and cl
+00000790: 6173 7320 6e61 6d65 7329 2e0a 0a20 2020  ass names)...   
+000007a0: 2020 2020 20da 0763 6c61 7373 6573 4e29       ..classesN)
+000007b0: 0572 3a00 0000 7231 0000 00da 0a5f 7365  .r:...r1....._se
+000007c0: 745f 6368 696c 64da 185f 7365 745f 696e  t_child.._set_in
+000007d0: 666f 5f73 6f6c 7665 725f 636c 6173 7365  fo_solver_classe
+000007e0: 73da 1563 6f6d 706c 6574 655f 7769 7468  s..complete_with
+000007f0: 5f63 6c61 7373 6573 2903 da03 636c 73da  _classes)...cls.
+00000800: 0b69 6e66 6f5f 736f 6c76 6572 723a 0000  .info_solverr:..
+00000810: 0072 2e00 0000 722e 0000 0072 2f00 0000  .r....r....r/...
+00000820: da15 5f63 6f6d 706c 6574 655f 696e 666f  .._complete_info
+00000830: 5f73 6f6c 7665 7253 0000 0073 0600 0000  _solverS...s....
+00000840: 0e06 0a01 1002 7a1c 4f75 7470 7574 2e5f  ......z.Output._
+00000850: 636f 6d70 6c65 7465 5f69 6e66 6f5f 736f  complete_info_so
+00000860: 6c76 6572 6302 0000 0000 0000 0000 0000  lverc...........
+00000870: 0002 0000 0007 0000 0043 0000 0073 2c00  .........C...s,.
+00000880: 0000 7c01 a000 6401 7401 6402 6401 6403  ..|...d.t.d.d.d.
+00000890: 8d02 a102 0100 7c01 a000 6404 7401 6405  ......|...d.t.d.
+000008a0: 6404 6403 8d02 a102 0100 6406 5300 2907  d.d.......d.S.).
+000008b0: 7a2e 5365 7420 7468 6520 636c 6173 7365  z.Set the classe
+000008c0: 7320 666f 7220 696e 666f 5f73 6f6c 7665  s for info_solve
+000008d0: 722e 636c 6173 7365 732e 4f75 7470 7574  r.classes.Output
+000008e0: 5a03 4c6f 677a 1766 6c75 6964 7369 6d66  Z.Logz.fluidsimf
+000008f0: 6f61 6d2e 6f75 7470 7574 2e6c 6f67 2902  oam.output.log).
+00000900: da0b 6d6f 6475 6c65 5f6e 616d 65da 0a63  ..module_name..c
+00000910: 6c61 7373 5f6e 616d 655a 0646 6965 6c64  lass_nameZ.Field
+00000920: 737a 1a66 6c75 6964 7369 6d66 6f61 6d2e  sz.fluidsimfoam.
+00000930: 6f75 7470 7574 2e66 6965 6c64 734e 2902  output.fieldsN).
+00000940: 723b 0000 00da 0464 6963 7429 0272 3e00  r;.....dict).r>.
+00000950: 0000 723a 0000 0072 2e00 0000 722e 0000  ..r:...r....r...
+00000960: 0072 2f00 0000 723c 0000 005e 0000 0073  .r/...r<...^...s
+00000970: 1c00 0000 0403 0201 0201 0201 0201 04fe  ................
+00000980: 04fe 0408 0201 0201 0201 0201 04fe 08fe  ................
+00000990: 7a1f 4f75 7470 7574 2e5f 7365 745f 696e  z.Output._set_in
+000009a0: 666f 5f73 6f6c 7665 725f 636c 6173 7365  fo_solver_classe
+000009b0: 7363 0100 0000 0000 0000 0000 0000 0400  sc..............
+000009c0: 0000 0700 0000 4300 0000 7362 0000 0069  ......C...sb...i
+000009d0: 0004 007d 017c 005f 007c 006a 0144 005d  ...}.|._.|.j.D.]
+000009e0: 0c7d 0274 027c 0283 017c 017c 02a0 0364  .}.t.|...|.|...d
+000009f0: 0164 02a1 023c 0071 087c 006a 0444 005d  .d...<.q.|.j.D.]
+00000a00: 097d 0374 027c 0364 0383 027c 017c 033c  .}.t.|.d...|.|.<
+00000a10: 0071 187c 006a 0544 005d 097d 0374 027c  .q.|.j.D.].}.t.|
+00000a20: 0364 0483 027c 017c 033c 0071 2564 0053  .d...|.|.<.q%d.S
+00000a30: 0029 054e da01 2eda 015f da08 636f 6e73  .).N....._..cons
+00000a40: 7461 6e74 da06 7379 7374 656d 2906 da18  tant..system)...
+00000a50: 5f66 696c 655f 6765 6e65 7261 746f 7273  _file_generators
+00000a60: 5f63 6c61 7373 6573 da0e 6e61 6d65 5f76  _classes..name_v
+00000a70: 6172 6961 626c 6573 720d 0000 00da 0772  ariablesr......r
+00000a80: 6570 6c61 6365 da13 6e61 6d65 5f63 6f6e  eplace..name_con
+00000a90: 7374 616e 745f 6669 6c65 73da 116e 616d  stant_files..nam
+00000aa0: 655f 7379 7374 656d 5f66 696c 6573 2904  e_system_files).
+00000ab0: 723e 0000 0072 3a00 0000 5a0d 7661 7269  r>...r:...Z.vari
+00000ac0: 6162 6c65 5f6e 616d 65da 0966 696c 655f  able_name..file_
+00000ad0: 6e61 6d65 722e 0000 0072 2e00 0000 722f  namer....r....r/
+00000ae0: 0000 00da 1e5f 7365 7475 705f 6669 6c65  ....._setup_file
+00000af0: 5f67 656e 6572 6174 6f72 735f 636c 6173  _generators_clas
+00000b00: 7365 7371 0000 0073 1400 0000 0a02 0a01  sesq...s........
+00000b10: 0201 0201 12ff 0a04 1001 0a02 1001 04ff  ................
+00000b20: 7a25 4f75 7470 7574 2e5f 7365 7475 705f  z%Output._setup_
+00000b30: 6669 6c65 5f67 656e 6572 6174 6f72 735f  file_generators_
+00000b40: 636c 6173 7365 7363 0300 0000 0000 0000  classesc........
+00000b50: 0000 0000 0400 0000 0700 0000 4300 0000  ............C...
+00000b60: 7374 0000 007c 00a0 00a1 0001 0074 017c  st...|.......t.|
+00000b70: 017c 027c 006a 02a0 03a1 0083 0301 007c  .|.|.j.........|
+00000b80: 01a0 0474 0564 0164 0264 0364 048d 03a1  ...t.d.d.d.d....
+00000b90: 0101 007c 016a 0664 0564 0164 0664 079c  ...|.j.d.d.d.d..
+00000ba0: 0264 088d 0201 007c 016a 07a0 0874 09a0  .d.....|.j...t..
+00000bb0: 0a64 09a1 01a1 0101 007c 026a 0b6a 0ca0  .d.......|.j.j..
+00000bc0: 0da1 007d 0374 017c 017c 027c 03a0 03a1  ...}.t.|.|.|....
+00000bd0: 0083 0301 0064 0353 0029 0a7a 3e54 6869  .....d.S.).z>Thi
+00000be0: 7320 7374 6174 6963 206d 6574 686f 6420  s static method 
+00000bf0: 6973 2075 7365 6420 746f 2063 6f6d 706c  is used to compl
+00000c00: 6574 6520 7468 6520 2a70 6172 616d 732a  ete the *params*
+00000c10: 2063 6f6e 7461 696e 6572 2e54 da03 7275   container.T..ru
+00000c20: 6e4e 2903 da0f 4e45 575f 4449 525f 5245  nN)...NEW_DIR_RE
+00000c30: 5355 4c54 535a 1373 686f 7274 5f6e 616d  SULTSZ.short_nam
+00000c40: 655f 7479 7065 5f72 756e 7219 0000 00da  e_type_runr.....
+00000c50: 066f 7574 7075 74da 0029 02da 0b48 4153  .output..)...HAS
+00000c60: 5f54 4f5f 5341 5645 da0d 7375 625f 6469  _TO_SAVE..sub_di
+00000c70: 7265 6374 6f72 7929 01da 0761 7474 7269  rectory)...attri
+00000c80: 6273 612e 0100 000a 2020 2020 2d20 6060  bsa.....    - ``
+00000c90: 4841 535f 544f 5f53 4156 4560 603a 2062  HAS_TO_SAVE``: b
+00000ca0: 6f6f 6c20 2864 6566 6175 6c74 3a20 5472  ool (default: Tr
+00000cb0: 7565 2920 4966 2046 616c 7365 2c20 6e6f  ue) If False, no
+00000cc0: 7468 696e 6720 6e65 7720 6973 2073 6176  thing new is sav
+00000cd0: 6564 2069 6e0a 2020 2020 2020 7468 6520  ed in.      the 
+00000ce0: 6469 7265 6374 6f72 7920 6f66 2074 6865  directory of the
+00000cf0: 2073 696d 756c 6174 696f 6e2e 0a20 2020   simulation..   
+00000d00: 202d 2060 6073 7562 5f64 6972 6563 746f   - ``sub_directo
+00000d10: 7279 6060 3a20 7374 7220 2864 6566 6175  ry``: str (defau
+00000d20: 6c74 3a20 2222 2920 4120 6e61 6d65 206f  lt: "") A name o
+00000d30: 6620 6120 7375 622d 6469 7265 6374 6f72  f a sub-director
+00000d40: 7920 2872 656c 6174 6976 650a 2020 2020  y (relative.    
+00000d50: 2020 746f 2024 464c 5549 4444 594e 5f50    to $FLUIDDYN_P
+00000d60: 4154 485f 5343 5241 5443 4829 2077 6865  ATH_SCRATCH) whe
+00000d70: 7265 696e 2074 6865 2064 6972 6563 746f  rein the directo
+00000d80: 7279 206f 6620 7468 6520 7369 6d75 6c61  ry of the simula
+00000d90: 7469 6f6e 0a20 2020 2020 2028 6060 7061  tion.      (``pa
+00000da0: 7468 5f72 756e 6060 2920 6973 2073 6176  th_run``) is sav
+00000db0: 6564 2e0a 0a29 0e72 4e00 0000 7208 0000  ed...).rN...r...
+00000dc0: 0072 4800 0000 da06 7661 6c75 6573 da0c  .rH.....values..
+00000dd0: 5f73 6574 5f61 7474 7269 6273 7243 0000  _set_attribsrC..
+00000de0: 0072 3b00 0000 7251 0000 00da 085f 7365  .r;...rQ....._se
+00000df0: 745f 646f 63da 0874 6578 7477 7261 70da  t_doc..textwrap.
+00000e00: 0664 6564 656e 7472 3a00 0000 7231 0000  .dedentr:...r1..
+00000e10: 00da 0e69 6d70 6f72 745f 636c 6173 7365  ...import_classe
+00000e20: 7329 0472 3e00 0000 da06 7061 7261 6d73  s).r>.....params
+00000e30: 723f 0000 00da 0c64 6963 745f 636c 6173  r?.....dict_clas
+00000e40: 7365 7372 2e00 0000 722e 0000 0072 2f00  sesr....r....r/.
+00000e50: 0000 da1d 5f63 6f6d 706c 6574 655f 7061  ...._complete_pa
+00000e60: 7261 6d73 5f77 6974 685f 6465 6661 756c  rams_with_defaul
+00000e70: 747f 0000 0073 2200 0000 0804 0201 0c01  t....s".........
+00000e80: 04ff 0405 0c01 04ff 0403 0a01 06ff 0603  ................
+00000e90: 0401 0201 02ff 04ff 0c0d 1401 7a24 4f75  ............z$Ou
+00000ea0: 7470 7574 2e5f 636f 6d70 6c65 7465 5f70  tput._complete_p
+00000eb0: 6172 616d 735f 7769 7468 5f64 6566 6175  arams_with_defau
+00000ec0: 6c74 4e63 0300 0000 0000 0000 0000 0000  ltNc............
+00000ed0: 0b00 0000 0800 0000 0300 0000 733c 0200  ............s<..
+00000ee0: 007c 017c 005f 007a 087c 016a 016a 026a  .|.|._.z.|.j.j.j
+00000ef0: 037c 005f 0457 006e 0904 0074 0579 1401  .|._.W.n...t.y..
+00000f00: 0001 0001 0059 006e 0777 0074 067c 006a  .....Y.n.w.t.|.j
+00000f10: 0483 017c 005f 077c 00a0 08a1 007c 005f  ...|._.|.....|._
+00000f20: 097c 0172 2e7c 016a 0a6a 0b7c 005f 0a74  .|.r.|.j.j.|._.t
+00000f30: 0c83 00a0 0d7c 01a1 0101 006e 0f7c 0272  .....|.....n.|.r
+00000f40: 357c 026a 0b7c 005f 0a6e 0864 007c 005f  5|.j.|._.n.d.|._
+00000f50: 0a74 0ea0 0f64 01a1 0101 007c 0173 4164  .t...d.....|.sAd
+00000f60: 0053 0074 107c 006a 1183 017c 005f 1174  .S.t.|.j...|._.t
+00000f70: 127c 0083 017c 005f 137c 016a 016a 026a  .|...|._.|.j.j.j
+00000f80: 146a 15a0 16a1 007d 037c 03a0 17a1 0044  .j.....}.|.....D
+00000f90: 005d 265c 027d 047d 0574 187c 007c 0583  .]&\.}.}.t.|.|..
+00000fa0: 0272 6271 5874 197c 0483 017d 067c 006a  .rbqXt.|...}.|.j
+00000fb0: 0004 006a 1a64 02a0 1b64 037c 069b 0064  ...j.d...d.|...d
+00000fc0: 049d 037c 05a1 0237 0002 005f 1a74 1c7c  ...|...7..._.t.|
+00000fd0: 007c 067c 057c 0083 0183 0301 0071 5874  .|.|.|.......qXt
+00000fe0: 1d7c 0064 0583 0273 887c 00a0 1ea1 0001  .|.d...s.|......
+00000ff0: 0069 007d 077c 006a 1fa0 17a1 0044 005d  .i.}.|.j.....D.]
+00001000: 255c 027d 047d 0574 197c 0483 017d 067c  %\.}.}.t.|...}.|
+00001010: 056a 207c 0776 0172 a37c 0467 017c 077c  .j |.v.r.|.g.|.|
+00001020: 056a 203c 006e 087c 077c 056a 2019 00a0  .j <.n.|.|.j ...
+00001030: 217c 04a1 0101 0074 1c7c 006a 137c 067c  !|.....t.|.j.|.|
+00001040: 057c 0083 0183 0301 0071 8f7c 0772 dc7c  .|.......q.|.r.|
+00001050: 006a 0004 006a 1a64 0637 0002 005f 1a7c  .j...j.d.7..._.|
+00001060: 07a0 17a1 0044 005d 185c 027d 087d 097c  .....D.].\.}.}.|
+00001070: 006a 0004 006a 1a64 077c 0864 0817 0064  .j...j.d.|.d...d
+00001080: 099b 0464 0aa0 227c 09a1 019b 0064 0b9d  ...d.."|.....d..
+00001090: 0437 0002 005f 1a71 c374 236a 2464 0c6b  .7..._.q.t#j$d.k
+000010a0: 0272 e97c 006a 2572 e97c 006a 006a 0a6a  .r.|.j%r.|.j.j.j
+000010b0: 2673 eb64 0053 007c 006a 1164 0d1b 00a0  &s.d.S.|.j.d....
+000010c0: 27a1 0001 007c 006a 1164 0e1b 00a0 27a1  '....|.j.d....'.
+000010d0: 0001 007c 006a 1164 0f1b 00a0 27a1 0001  ...|.j.d....'...
+000010e0: 0074 287c 006a 1383 01a0 29a1 0044 005d  .t(|.j....)..D.]
+000010f0: 147d 0a74 1d7c 0a64 1083 0290 0172 1a7c  .}.t.|.d.....r.|
+00001100: 0a6a 2aa0 2b64 0da1 0190 0172 1a7c 0aa0  .j*.+d.....r.|..
+00001110: 2ca1 0001 0090 0171 0764 0053 0029 114e  ,......q.d.S.).N
+00001120: 7a45 496e 6974 6961 6c69 7a69 6e67 204f  zEInitializing O
+00001130: 7574 7075 7420 636c 6173 7320 7769 7468  utput class with
+00001140: 6f75 7420 7369 6d20 6f72 2070 6172 616d  out sim or param
+00001150: 7320 6d69 6768 7420 6c65 6164 2074 6f20  s might lead to 
+00001160: 6572 726f 7273 2e7a 097b 3a32 3873 7d7b  errors.z.{:28s}{
+00001170: 7d0a 7a0b 7369 6d2e 6f75 7470 7574 2e7a  }.z.sim.output.z
+00001180: 023a 2072 4800 0000 7a0d 696e 7075 745f  .: rH...z.input_
+00001190: 6669 6c65 733a 0a7a 0720 202d 2069 6e20  files:.z.  - in 
+000011a0: fa01 3a5a 0331 3273 da01 20da 010a 7201  ..:Z.12s.. ...r.
+000011b0: 0000 0072 4700 0000 da01 3072 4600 0000  ...rG.....0rF...
+000011c0: da0d 6765 6e65 7261 7465 5f66 696c 6529  ..generate_file)
+000011d0: 2dda 0373 696d da04 696e 666f da06 736f  -..sim..info..so
+000011e0: 6c76 6572 da0a 7368 6f72 745f 6e61 6d65  lver..short_name
+000011f0: da0b 6e61 6d65 5f73 6f6c 7665 72da 0e41  ..name_solver..A
+00001200: 7474 7269 6275 7465 4572 726f 7272 0f00  ttributeErrorr..
+00001210: 0000 da07 7061 636b 6167 65da 1767 6574  ....package..get
+00001220: 5f70 6174 685f 736f 6c76 6572 5f70 6163  _path_solver_pac
+00001230: 6b61 6765 5a13 7061 7468 5f73 6f6c 7665  kageZ.path_solve
+00001240: 725f 7061 636b 6167 6572 5c00 0000 7251  r_packager\...rQ
+00001250: 0000 00da 0573 7570 6572 da08 5f5f 696e  .....super..__in
+00001260: 6974 5f5f 720e 0000 00da 0777 6172 6e69  it__r......warni
+00001270: 6e67 7203 0000 0072 2800 0000 720c 0000  ngr....r(...r...
+00001280: 00da 0b69 6e70 7574 5f66 696c 6573 723a  ...input_filesr:
+00001290: 0000 0072 3100 0000 725b 0000 00da 0569  ...r1...r[.....i
+000012a0: 7465 6d73 7212 0000 0072 0400 0000 da11  temsr....r......
+000012b0: 5f6f 626a 6563 7473 5f74 6f5f 7072 696e  _objects_to_prin
+000012c0: 74da 0666 6f72 6d61 74da 0773 6574 6174  t..format..setat
+000012d0: 7472 da07 6861 7361 7474 7272 4e00 0000  tr..hasattrrN...
+000012e0: 7248 0000 00da 0864 6972 5f6e 616d 65da  rH.....dir_name.
+000012f0: 0661 7070 656e 64da 046a 6f69 6e72 0600  .append..joinr..
+00001300: 0000 da04 7261 6e6b da0c 5f68 6173 5f74  ....rank.._has_t
+00001310: 6f5f 7361 7665 7250 0000 00da 056d 6b64  o_saverP.....mkd
+00001320: 6972 da04 7661 7273 7256 0000 00da 0872  ir..varsrV.....r
+00001330: 656c 5f70 6174 6872 1600 0000 7263 0000  el_pathr....rc..
+00001340: 0029 0bda 0473 656c 6672 6400 0000 725c  .)...selfrd...r\
+00001350: 0000 0072 5d00 0000 da08 636c 735f 6e61  ...r].....cls_na
+00001360: 6d65 da05 436c 6173 73da 086f 626a 5f6e  me..Class..obj_n
+00001370: 616d 655a 1366 6f72 5f73 7472 5f69 6e70  ameZ.for_str_inp
+00001380: 7574 5f66 696c 6573 7275 0000 0072 6f00  ut_filesru...ro.
+00001390: 0000 da0e 6669 6c65 5f67 656e 6572 6174  ....file_generat
+000013a0: 6f72 a901 da09 5f5f 636c 6173 735f 5f72  or....__class__r
+000013b0: 2e00 0000 722f 0000 0072 6d00 0000 9f00  ....r/...rm.....
+000013c0: 0000 7380 0000 0006 0102 0110 010c 0104  ..s.............
+000013d0: 0102 ff0c 030a 0204 020a 020e 0104 010a  ................
+000013e0: 0206 0204 0102 0104 ff04 0404 010c 020a  ................
+000013f0: 0210 0210 010a 0102 0108 010c 010c 0108  ................
+00001400: ff12 030a 0208 0104 0112 0108 010a 020e  ................
+00001410: 0110 0214 0104 0210 0110 0108 011a 0108  ................
+00001420: ff08 0502 ff04 0202 fe08 0302 fd04 050e  ................
+00001430: 020e 010e 0112 0202 0104 0106 ff0a 0204  ................
+00001440: fe08 0304 8004 fc7a 0f4f 7574 7075 742e  .......z.Output.
+00001450: 5f5f 696e 6974 5f5f 6301 0000 0000 0000  __init__c.......
+00001460: 0000 0000 0001 0000 0004 0000 0043 0000  .............C..
+00001470: 0073 1200 0000 7400 7401 a002 7c00 a101  .s....t.t...|...
+00001480: 6a03 8301 6a04 5300 2901 7a28 4765 7420  j...j.S.).z(Get 
+00001490: 7468 6520 7061 7468 2074 6f77 6172 6473  the path towards
+000014a0: 2074 6865 2073 6f6c 7665 7220 7061 636b   the solver pack
+000014b0: 6167 652e 2905 7203 0000 00da 0769 6e73  age.).r......ins
+000014c0: 7065 6374 da09 6765 746d 6f64 756c 65da  pect..getmodule.
+000014d0: 085f 5f66 696c 655f 5fda 0670 6172 656e  .__file__..paren
+000014e0: 7429 0172 3e00 0000 722e 0000 0072 2e00  t).r>...r....r..
+000014f0: 0000 722f 0000 0072 6b00 0000 ec00 0000  ..r/...rk.......
+00001500: 7302 0000 0012 037a 1e4f 7574 7075 742e  s......z.Output.
+00001510: 6765 745f 7061 7468 5f73 6f6c 7665 725f  get_path_solver_
+00001520: 7061 636b 6167 6563 0100 0000 0000 0000  packagec........
+00001530: 0000 0000 0400 0000 0800 0000 0300 0000  ................
+00001540: 73d8 0000 0074 006a 0164 016b 0272 0d74  s....t.j.d.k.r.t
+00001550: 0264 027c 006a 039b 009d 0283 0101 0074  .d.|.j.........t
+00001560: 0483 008f 0d01 0074 0583 00a0 06a1 0001  .......t........
+00001570: 0057 0064 0304 0004 0083 0301 006e 0831  .W.d.........n.1
+00001580: 0073 2077 0101 0001 0001 0059 0001 0074  .s w.......Y...t
+00001590: 07a0 087c 006a 096a 0aa1 0101 0074 006a  ...|.j.j.....t.j
+000015a0: 0164 016b 0272 397c 006a 0b72 397c 006a  .d.k.r9|.j.r9|.j
+000015b0: 096a 0c6a 0d73 3b64 0353 0074 0e7c 006a  .j.j.s;d.S.t.|.j
+000015c0: 096a 0c6a 0f7c 006a 0383 0201 007c 00a0  .j.j.|.j.....|..
+000015d0: 10a1 0001 007c 006a 0364 041b 007d 017c  .....|.j.d...}.|
+000015e0: 016a 1164 0564 068d 0101 0064 0744 005d  .j.d.d.....d.D.]
+000015f0: 147d 027c 017c 021b 007d 037c 03a0 12a1  .}.|.|...}.|....
+00001600: 0072 6071 5574 13a0 147c 006a 037c 021b  .r`qUt...|.j.|..
+00001610: 007c 03a1 0201 0071 5564 0353 0029 087a  .|.....qUd.S.).z
+00001620: 214c 6f67 7320 696e 666f 206f 6e20 696e  !Logs info on in
+00001630: 7374 616e 7469 6174 6564 2063 6c61 7373  stantiated class
+00001640: 6573 7201 0000 007a 0a70 6174 685f 7275  esr....z.path_ru
+00001650: 6e3a 204e 7a0e 2e64 6174 615f 666c 7569  n: Nz..data_flui
+00001660: 6473 696d 5429 01da 0865 7869 7374 5f6f  dsimT)...exist_o
+00001670: 6b29 027a 0f69 6e66 6f5f 736f 6c76 6572  k).z.info_solver
+00001680: 2e78 6d6c 7a10 7061 7261 6d73 5f73 696d  .xmlz.params_sim
+00001690: 756c 2e78 6d6c 2915 7206 0000 0072 7800  ul.xml).r....rx.
+000016a0: 0000 da05 7072 696e 7472 2800 0000 7205  ....printr(...r.
+000016b0: 0000 0072 6c00 0000 da09 706f 7374 5f69  ...rl.....post_i
+000016c0: 6e69 7472 0e00 0000 7265 0000 0072 6400  nitr....re...rd.
+000016d0: 0000 7271 0000 0072 7900 0000 725c 0000  ..rq...ry...r\..
+000016e0: 0072 5000 0000 7230 0000 0072 1900 0000  .rP...r0...r....
+000016f0: da29 5f70 6f73 745f 696e 6974 5f63 7265  .)_post_init_cre
+00001700: 6174 655f 6164 6469 7469 6f6e 616c 5f73  ate_additional_s
+00001710: 6f75 7263 655f 6669 6c65 7372 7a00 0000  ource_filesrz...
+00001720: 7227 0000 0072 2100 0000 7222 0000 0029  r'...r!...r"...)
+00001730: 0472 7d00 0000 5a12 7061 7468 5f69 6e66  .r}...Z.path_inf
+00001740: 6f5f 666c 7569 6473 696d 724d 0000 005a  o_fluidsimrM...Z
+00001750: 0870 6174 685f 6e65 7772 8200 0000 722e  .path_newr....r.
+00001760: 0000 0072 2f00 0000 728a 0000 00f1 0000  ...r/...r.......
+00001770: 0073 2e00 0000 0a03 1001 0803 0c01 1cff  .s..............
+00001780: 0e03 0804 02ff 0402 02fe 0803 02fd 0405  ................
+00001790: 1202 0801 0a03 0c01 0801 0801 0801 0201  ................
+000017a0: 1401 04fc 7a10 4f75 7470 7574 2e70 6f73  ....z.Output.pos
+000017b0: 745f 696e 6974 6301 0000 0000 0000 0000  t_initc.........
+000017c0: 0000 0003 0000 0004 0000 0043 0000 0073  ...........C...s
+000017d0: 6c00 0000 7c00 6a00 6a01 6401 1b00 7d01  l...|.j.j.d...}.
+000017e0: 7c01 a002 a100 7313 7403 6402 7c00 6a00  |.....s.t.d.|.j.
+000017f0: 6a01 9b00 9d02 8301 8201 7404 a005 7c01  j.........t...|.
+00001800: 7c00 6a06 6a07 a102 0100 7408 7c00 6a00  |.j.j.....t.|.j.
+00001810: 8301 a009 a100 4400 5d11 7d02 740a 7c02  ......D.].}.t.|.
+00001820: 6403 8302 7233 7c02 6a0b a00c 6404 a101  d...r3|.j...d...
+00001830: 7333 7c02 a00d a100 0100 7122 6405 5300  s3|.......q"d.S.
+00001840: 2906 7a24 4372 6561 7465 2074 6865 2066  ).z$Create the f
+00001850: 696c 6573 2066 726f 6d20 7468 6569 7220  iles from their 
+00001860: 7465 6d70 6c61 7465 7a08 7461 736b 732e  templatez.tasks.
+00001870: 7079 7a29 7461 736b 732e 7079 206d 6973  pyz)tasks.py mis
+00001880: 7369 6e67 2069 6e20 736f 6c76 6572 2074  sing in solver t
+00001890: 656d 706c 6174 6573 5f64 6972 2072 6300  emplates_dir rc.
+000018a0: 0000 7247 0000 004e 290e 726f 0000 005a  ..rG...N).ro...Z
+000018b0: 0d74 656d 706c 6174 6573 5f64 6972 7227  .templates_dirr'
+000018c0: 0000 00da 0c52 756e 7469 6d65 4572 726f  .....RuntimeErro
+000018d0: 7272 2100 0000 7222 0000 0072 6400 0000  rr!...r"...rd...
+000018e0: 7228 0000 0072 7b00 0000 7256 0000 0072  r(...r{...rV...r
+000018f0: 7400 0000 727c 0000 0072 1600 0000 7263  t...r|...r....rc
+00001900: 0000 0029 0372 7d00 0000 5a0d 7061 7468  ...).r}...Z.path
+00001910: 5f74 6173 6b73 5f70 7972 8100 0000 722e  _tasks_pyr....r.
+00001920: 0000 0072 2e00 0000 722f 0000 0072 8b00  ...r....r/...r..
+00001930: 0000 1101 0000 7322 0000 000c 0208 0102  ......s"........
+00001940: 0102 0106 0104 ff04 ff10 0412 0202 0104  ................
+00001950: 0104 ff0a 0202 fe08 0402 8004 fb7a 304f  .............z0O
+00001960: 7574 7075 742e 5f70 6f73 745f 696e 6974  utput._post_init
+00001970: 5f63 7265 6174 655f 6164 6469 7469 6f6e  _create_addition
+00001980: 616c 5f73 6f75 7263 655f 6669 6c65 7363  al_source_filesc
+00001990: 0200 0000 0000 0000 0000 0000 0300 0000  ................
+000019a0: 0800 0000 4300 0000 7328 0000 0064 0164  ....C...s(...d.d
+000019b0: 0164 0164 0264 0264 0264 0364 049c 077d  .d.d.d.d.d.d...}
+000019c0: 027c 016a 0064 057c 0264 0664 078d 0301  .|.j.d.|.d.d....
+000019d0: 0064 0053 0029 084e e928 0000 0067 0000  .d.S.).N.(...g..
+000019e0: 0000 0000 f03f e901 0000 0029 07da 026e  .....?.....)...n
+000019f0: 78da 026e 79da 026e 7ada 026c 78da 026c  x..ny..nz..lx..l
+00001a00: 79da 026c 7ada 0573 6361 6c65 da0f 626c  y..lz..scale..bl
+00001a10: 6f63 6b5f 6d65 7368 5f64 6963 74da 0454  ock_mesh_dict..T
+00001a20: 4f44 4f29 0272 5500 0000 da03 646f 6329  ODO).rU.....doc)
+00001a30: 0172 3b00 0000 2903 723e 0000 0072 5c00  .r;...).r>...r\.
+00001a40: 0000 da07 6465 6661 756c 7472 2e00 0000  ....defaultr....
+00001a50: 722e 0000 0072 2f00 0000 da20 5f63 6f6d  r....r/.... _com
+00001a60: 706c 6574 655f 7061 7261 6d73 5f62 6c6f  plete_params_blo
+00001a70: 636b 5f6d 6573 685f 6469 6374 2201 0000  ck_mesh_dict"...
+00001a80: 731a 0000 0002 0302 0102 0102 0102 0102  s...............
+00001a90: 0102 0106 f904 0a02 0102 0102 010a fd7a  ...............z
+00001aa0: 274f 7574 7075 742e 5f63 6f6d 706c 6574  'Output._complet
+00001ab0: 655f 7061 7261 6d73 5f62 6c6f 636b 5f6d  e_params_block_m
+00001ac0: 6573 685f 6469 6374 6303 0000 0000 0000  esh_dictc.......
+00001ad0: 0000 0000 0003 0000 0001 0000 0043 0000  .............C..
+00001ae0: 0073 0400 0000 6900 5300 2901 4e72 2e00  .s....i.S.).Nr..
+00001af0: 0000 2903 727d 0000 005a 0474 6d69 6e5a  ..).r}...Z.tminZ
+00001b00: 0474 6d61 7872 2e00 0000 722e 0000 0072  .tmaxr....r....r
+00001b10: 2f00 0000 da14 5f63 6f6d 7075 7465 5f6d  /....._compute_m
+00001b20: 6561 6e5f 7661 6c75 6573 3401 0000 7302  ean_values4...s.
+00001b30: 0000 0004 017a 1b4f 7574 7075 742e 5f63  .....z.Output._c
+00001b40: 6f6d 7075 7465 5f6d 6561 6e5f 7661 6c75  ompute_mean_valu
+00001b50: 6573 2902 4e4e 2918 da08 5f5f 6e61 6d65  es).NN)...__name
+00001b60: 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f da0c  __..__module__..
+00001b70: 5f5f 7175 616c 6e61 6d65 5f5f 7249 0000  __qualname__rI..
+00001b80: 0072 4b00 0000 724c 0000 0072 0900 0000  .rK...rL...r....
+00001b90: 5a1d 5f68 656c 7065 725f 7475 7262 756c  Z._helper_turbul
+00001ba0: 656e 6365 5f70 726f 7065 7274 6965 7372  ence_propertiesr
+00001bb0: 0b00 0000 5a1a 5f68 656c 7065 725f 6465  ....Z._helper_de
+00001bc0: 636f 6d70 6f73 655f 7061 725f 6469 6374  compose_par_dict
+00001bd0: 720a 0000 00da 145f 6865 6c70 6572 5f63  r......_helper_c
+00001be0: 6f6e 7472 6f6c 5f64 6963 74da 0b63 6c61  ontrol_dict..cla
+00001bf0: 7373 6d65 7468 6f64 7240 0000 0072 3c00  ssmethodr@...r<.
+00001c00: 0000 724e 0000 0072 5e00 0000 726d 0000  ..rN...r^...rm..
+00001c10: 0072 6b00 0000 728a 0000 0072 8b00 0000  .rk...r....r....
+00001c20: 729a 0000 0072 9b00 0000 da0d 5f5f 636c  r....r......__cl
+00001c30: 6173 7363 656c 6c5f 5f72 2e00 0000 722e  asscell__r....r.
+00001c40: 0000 0072 8200 0000 722f 0000 0072 3100  ...r....r/...r1.
+00001c50: 0000 4300 0000 7332 0000 0008 0008 0108  ..C...s2........
+00001c60: 0108 0102 0708 0104 ff06 0306 0102 020a  ................
+00001c70: 0102 0a0a 0102 120a 0102 0d0a 010e 1f02  ................
+00001c80: 4d0a 010c 0408 2002 110a 0110 1172 3100  M..... ......r1.
+00001c90: 0000 2922 da07 5f5f 646f 635f 5f5a 1369  ..)"..__doc__Z.i
+00001ca0: 6d70 6f72 746c 6962 2e72 6573 6f75 7263  mportlib.resourc
+00001cb0: 6573 7218 0000 0072 8400 0000 721c 0000  esr....r....r...
+00001cc0: 0072 2100 0000 7259 0000 00da 0a63 6f6e  .r!...rY.....con
+00001cd0: 7465 7874 6c69 6272 0200 0000 da07 7061  textlibr......pa
+00001ce0: 7468 6c69 6272 0300 0000 da0a 696e 666c  thlibr......infl
+00001cf0: 6563 7469 6f6e 7204 0000 005a 0b66 6c75  ectionr....Z.flu
+00001d00: 6964 6479 6e2e 696f 7205 0000 005a 0d66  iddyn.ior....Z.f
+00001d10: 6c75 6964 6479 6e2e 7574 696c 7206 0000  luiddyn.utilr...
+00001d20: 005a 1466 6c75 6964 7369 6d5f 636f 7265  .Z.fluidsim_core
+00001d30: 2e6f 7574 7075 7472 0700 0000 da14 666c  .outputr......fl
+00001d40: 7569 6473 696d 5f63 6f72 652e 7061 7261  uidsim_core.para
+00001d50: 6d73 7208 0000 00da 1d66 6c75 6964 7369  msr......fluidsi
+00001d60: 6d66 6f61 6d2e 666f 616d 5f69 6e70 7574  mfoam.foam_input
+00001d70: 5f66 696c 6573 7209 0000 0072 0a00 0000  _filesr....r....
+00001d80: 720b 0000 005a 2866 6c75 6964 7369 6d66  r....Z(fluidsimf
+00001d90: 6f61 6d2e 666f 616d 5f69 6e70 7574 5f66  oam.foam_input_f
+00001da0: 696c 6573 2e67 656e 6572 6174 6f72 7372  iles.generatorsr
+00001db0: 0c00 0000 720d 0000 005a 1066 6c75 6964  ....r....Z.fluid
+00001dc0: 7369 6d66 6f61 6d2e 6c6f 6772 0e00 0000  simfoam.logr....
+00001dd0: da14 666c 7569 6473 696d 666f 616d 2e73  ..fluidsimfoam.s
+00001de0: 6f6c 7665 7273 720f 0000 0072 3000 0000  olversr....r0...
+00001df0: 7231 0000 0072 2e00 0000 722e 0000 0072  r1...r....r....r
+00001e00: 2e00 0000 722f 0000 00da 083c 6d6f 6475  ....r/.....<modu
+00001e10: 6c65 3e01 0000 0073 2600 0000 0400 0802  le>....s&.......
+00001e20: 0801 0801 0801 0801 0c01 0c01 0c02 0c02  ................
+00001e30: 0c01 0c01 0c01 1401 1005 0c04 0c01 0803  ................
+00001e40: 1425                                     .%
```

### Comparing `fluidsimfoam-0.0.5/src/fluidsimfoam/output/__pycache__/dataframe_from_paths.cpython-39.pyc` & `fluidsimfoam-0.0.6/src/fluidsimfoam/output/__pycache__/dataframe_from_paths.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun  1 13:07:51 2023 UTC, .py size: 1080 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 2798 7864 3804 0000  a.......'.xd8...
+00000000: 6f0d 0d0a 0000 0000 5ab4 6f64 3804 0000  o.......Z.od8...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4e00 0000 6400  .....@...sN...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 0100 6401 6404 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 4700 6405 6406 8400 6406  m.Z...G.d.d...d.
 00000060: 6502 8303 5a07 6507 8300 5a08 6508 6a09  e...Z.e...Z.e.j.
 00000070: 5a09 6508 6a0a 5a0a 6407 5300 2908 7a2a  Z.e.j.Z.d.S.).z*
@@ -15,82 +15,83 @@
 000000e0: 7463 0000 0000 0000 0000 0000 0000 0000  tc..............
 000000f0: 0000 0200 0000 4000 0000 7324 0000 0065  ......@...s$...e
 00000100: 005a 0164 005a 0264 0164 0284 005a 0364  .Z.d.Z.d.d...Z.d
 00000110: 0364 0484 005a 0464 0564 0684 005a 0564  .d...Z.d.d...Z.d
 00000120: 0753 0029 08da 1244 6174 6166 7261 6d65  .S.)...Dataframe
 00000130: 4d61 6b65 7246 6f61 6d63 0200 0000 0000  MakerFoamc......
 00000140: 0000 0000 0000 0600 0000 0800 0000 4300  ..............C.
-00000150: 0000 7378 0000 0074 007c 01a0 0164 01a1  ..sx...t.|...d..
+00000150: 0000 737a 0000 0074 007c 01a0 0164 01a1  ..sz...t.|...d..
 00000160: 0183 017d 027c 0264 0219 007d 0374 027c  ...}.|.d...}.t.|
-00000170: 0383 018f 467d 047c 0444 005d 307d 057c  ....F}.|.D.]0}.|
-00000180: 05a0 0364 03a1 0172 2474 047c 05a0 05a1  ...d...r$t.|....
+00000170: 0383 018f 247d 047c 0444 005d 187d 057c  ....$}.|.D.].}.|
+00000180: 05a0 0364 03a1 0172 2a74 047c 05a0 05a1  ...d...r*t.|....
 00000190: 0064 0419 0083 0102 0001 0057 0002 0064  .d.........W...d
-000001a0: 0504 0004 0083 0301 0053 0071 2457 0064  .........S.q$W.d
-000001b0: 0504 0004 0083 0301 006e 1031 0073 6a30  .........n.1.sj0
-000001c0: 0001 0001 0001 0059 0001 0064 0553 0029  .......Y...d.S.)
-000001d0: 067a 0e47 6574 2066 6972 7374 2074 696d  .z.Get first tim
-000001e0: 65fa 086c 6f67 2a2e 7478 7472 0100 0000  e..log*.txtr....
-000001f0: 7a0d 7374 6172 745f 7469 6d65 203d 20e9  z.start_time = .
-00000200: ffff ffff 4e29 06da 0673 6f72 7465 64da  ....N)...sorted.
-00000210: 0467 6c6f 62da 046f 7065 6eda 0a73 7461  .glob..open..sta
-00000220: 7274 7377 6974 68da 0566 6c6f 6174 da05  rtswith..float..
-00000230: 7370 6c69 7429 06da 0473 656c 66da 0470  split)...self..p
-00000240: 6174 68da 086c 6f67 6669 6c65 73da 0870  ath..logfiles..p
-00000250: 6174 685f 6c6f 67da 0466 696c 65da 046c  ath_log..file..l
-00000260: 696e 65a9 0072 1500 0000 fa56 2f68 6f6d  ine..r.....V/hom
-00000270: 652f 7573 6572 732f 6175 6769 6572 3370  e/users/augier3p
-00000280: 692f 4465 762f 666c 7569 6473 696d 666f  i/Dev/fluidsimfo
-00000290: 616d 2f73 7263 2f66 6c75 6964 7369 6d66  am/src/fluidsimf
-000002a0: 6f61 6d2f 6f75 7470 7574 2f64 6174 6166  oam/output/dataf
-000002b0: 7261 6d65 5f66 726f 6d5f 7061 7468 732e  rame_from_paths.
-000002c0: 7079 da18 6765 745f 7469 6d65 5f73 7461  py..get_time_sta
-000002d0: 7274 5f66 726f 6d5f 7061 7468 0900 0000  rt_from_path....
-000002e0: 730c 0000 0000 020e 0108 010a 0108 010a  s...............
-000002f0: 017a 2b44 6174 6166 7261 6d65 4d61 6b65  .z+DataframeMake
-00000300: 7246 6f61 6d2e 6765 745f 7469 6d65 5f73  rFoam.get_time_s
-00000310: 7461 7274 5f66 726f 6d5f 7061 7468 6302  tart_from_pathc.
-00000320: 0000 0000 0000 0000 0000 0004 0000 0004  ................
-00000330: 0000 0043 0000 0073 1e00 0000 7400 7c01  ...C...s....t.|.
-00000340: a001 6401 a101 8301 7d02 7c02 6402 1900  ..d.....}.|.d...
-00000350: 7d03 7402 7c03 8301 5300 2903 7a13 4765  }.t.|...S.).z.Ge
-00000360: 7420 6c61 7374 2073 6176 6564 2074 696d  t last saved tim
-00000370: 6572 0700 0000 7208 0000 0029 0372 0900  er....r....).r..
-00000380: 0000 720a 0000 0072 0500 0000 2904 720f  ..r....r....).r.
-00000390: 0000 0072 1000 0000 7211 0000 0072 1200  ...r....r....r..
-000003a0: 0000 7215 0000 0072 1500 0000 7216 0000  ..r....r....r...
-000003b0: 00da 1767 6574 5f74 696d 655f 6c61 7374  ...get_time_last
-000003c0: 5f66 726f 6d5f 7061 7468 1200 0000 7306  _from_path....s.
-000003d0: 0000 0000 020e 0108 017a 2a44 6174 6166  .........z*Dataf
-000003e0: 7261 6d65 4d61 6b65 7246 6f61 6d2e 6765  rameMakerFoam.ge
-000003f0: 745f 7469 6d65 5f6c 6173 745f 6672 6f6d  t_time_last_from
-00000400: 5f70 6174 6863 0200 0000 0000 0000 0000  _pathc..........
-00000410: 0000 0200 0000 0400 0000 4300 0000 730c  ..........C...s.
-00000420: 0000 0074 007c 0164 0164 028d 0253 0029  ...t.|.d.d...S.)
-00000430: 037a 184c 6f61 6420 6120 7369 6d75 6c61  .z.Load a simula
-00000440: 7469 6f6e 206f 626a 6563 7454 2901 da0b  tion objectT)...
-00000450: 6869 6465 5f73 7464 6f75 7472 0300 0000  hide_stdoutr....
-00000460: 2902 720f 0000 0072 1000 0000 7215 0000  ).r....r....r...
-00000470: 0072 1500 0000 7216 0000 00da 086c 6f61  .r....r......loa
-00000480: 645f 7369 6d18 0000 0073 0200 0000 0002  d_sim....s......
-00000490: 7a1b 4461 7461 6672 616d 654d 616b 6572  z.DataframeMaker
-000004a0: 466f 616d 2e6c 6f61 645f 7369 6d4e 2906  Foam.load_simN).
-000004b0: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
-000004c0: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
-000004d0: 6d65 5f5f 7217 0000 0072 1800 0000 721a  me__r....r....r.
-000004e0: 0000 0072 1500 0000 7215 0000 0072 1500  ...r....r....r..
-000004f0: 0000 7216 0000 0072 0600 0000 0800 0000  ..r....r........
-00000500: 7306 0000 0008 0108 0908 0672 0600 0000  s..........r....
-00000510: 4e29 0bda 075f 5f64 6f63 5f5f 5a29 666c  N)...__doc__Z)fl
-00000520: 7569 6473 696d 5f63 6f72 652e 6f75 7470  uidsim_core.outp
-00000530: 7574 2e64 6174 6166 7261 6d65 5f66 726f  ut.dataframe_fro
-00000540: 6d5f 7061 7468 7372 0200 0000 da0c 666c  m_pathsr......fl
-00000550: 7569 6473 696d 666f 616d 7204 0000 005a  uidsimfoamr....Z
-00000560: 1766 6c75 6964 7369 6d66 6f61 6d2e 6f75  .fluidsimfoam.ou
-00000570: 7470 7574 2e6c 6f67 7205 0000 0072 0600  tput.logr....r..
-00000580: 0000 5a10 5f64 6174 6166 7261 6d65 5f6d  ..Z._dataframe_m
-00000590: 616b 6572 da19 6765 745f 6d65 616e 5f76  aker..get_mean_v
-000005a0: 616c 7565 735f 6672 6f6d 5f70 6174 68da  alues_from_path.
-000005b0: 1867 6574 5f64 6174 6166 7261 6d65 5f66  .get_dataframe_f
-000005c0: 726f 6d5f 7061 7468 7372 1500 0000 7215  rom_pathsr....r.
-000005d0: 0000 0072 1500 0000 7216 0000 00da 083c  ...r....r......<
-000005e0: 6d6f 6475 6c65 3e01 0000 0073 0e00 0000  module>....s....
-000005f0: 0402 0c01 0c01 0c03 1015 0602 0601       ..............
+000001a0: 0504 0004 0083 0301 0053 0071 1257 0064  .........S.q.W.d
+000001b0: 0504 0004 0083 0301 0064 0553 0031 0073  .........d.S.1.s
+000001c0: 3677 0101 0001 0001 0059 0001 0064 0553  6w.......Y...d.S
+000001d0: 0029 067a 0e47 6574 2066 6972 7374 2074  .).z.Get first t
+000001e0: 696d 65fa 086c 6f67 2a2e 7478 7472 0100  ime..log*.txtr..
+000001f0: 0000 7a0d 7374 6172 745f 7469 6d65 203d  ..z.start_time =
+00000200: 20e9 ffff ffff 4e29 06da 0673 6f72 7465   .....N)...sorte
+00000210: 64da 0467 6c6f 62da 046f 7065 6eda 0a73  d..glob..open..s
+00000220: 7461 7274 7377 6974 68da 0566 6c6f 6174  tartswith..float
+00000230: da05 7370 6c69 7429 06da 0473 656c 66da  ..split)...self.
+00000240: 0470 6174 68da 086c 6f67 6669 6c65 73da  .path..logfiles.
+00000250: 0870 6174 685f 6c6f 67da 0466 696c 65da  .path_log..file.
+00000260: 046c 696e 65a9 0072 1500 0000 fa4d 2f68  .line..r.....M/h
+00000270: 6f6d 652f 7069 6572 7265 2f44 6576 2f66  ome/pierre/Dev/f
+00000280: 6c75 6964 7369 6d66 6f61 6d2f 7372 632f  luidsimfoam/src/
+00000290: 666c 7569 6473 696d 666f 616d 2f6f 7574  fluidsimfoam/out
+000002a0: 7075 742f 6461 7461 6672 616d 655f 6672  put/dataframe_fr
+000002b0: 6f6d 5f70 6174 6873 2e70 79da 1867 6574  om_paths.py..get
+000002c0: 5f74 696d 655f 7374 6172 745f 6672 6f6d  _time_start_from
+000002d0: 5f70 6174 6809 0000 0073 1400 0000 0e02  _path....s......
+000002e0: 0801 0a01 0801 0a01 1201 10fd 0202 02ff  ................
+000002f0: 22ff 7a2b 4461 7461 6672 616d 654d 616b  ".z+DataframeMak
+00000300: 6572 466f 616d 2e67 6574 5f74 696d 655f  erFoam.get_time_
+00000310: 7374 6172 745f 6672 6f6d 5f70 6174 6863  start_from_pathc
+00000320: 0200 0000 0000 0000 0000 0000 0400 0000  ................
+00000330: 0400 0000 4300 0000 731e 0000 0074 007c  ....C...s....t.|
+00000340: 01a0 0164 01a1 0183 017d 027c 0264 0219  ...d.....}.|.d..
+00000350: 007d 0374 027c 0383 0153 0029 037a 1347  .}.t.|...S.).z.G
+00000360: 6574 206c 6173 7420 7361 7665 6420 7469  et last saved ti
+00000370: 6d65 7207 0000 0072 0800 0000 2903 7209  mer....r....).r.
+00000380: 0000 0072 0a00 0000 7205 0000 0029 0472  ...r....r....).r
+00000390: 0f00 0000 7210 0000 0072 1100 0000 7212  ....r....r....r.
+000003a0: 0000 0072 1500 0000 7215 0000 0072 1600  ...r....r....r..
+000003b0: 0000 da17 6765 745f 7469 6d65 5f6c 6173  ....get_time_las
+000003c0: 745f 6672 6f6d 5f70 6174 6812 0000 0073  t_from_path....s
+000003d0: 0600 0000 0e02 0801 0801 7a2a 4461 7461  ..........z*Data
+000003e0: 6672 616d 654d 616b 6572 466f 616d 2e67  frameMakerFoam.g
+000003f0: 6574 5f74 696d 655f 6c61 7374 5f66 726f  et_time_last_fro
+00000400: 6d5f 7061 7468 6302 0000 0000 0000 0000  m_pathc.........
+00000410: 0000 0002 0000 0004 0000 0043 0000 0073  ...........C...s
+00000420: 0c00 0000 7400 7c01 6401 6402 8d02 5300  ....t.|.d.d...S.
+00000430: 2903 7a18 4c6f 6164 2061 2073 696d 756c  ).z.Load a simul
+00000440: 6174 696f 6e20 6f62 6a65 6374 5429 01da  ation objectT)..
+00000450: 0b68 6964 655f 7374 646f 7574 7203 0000  .hide_stdoutr...
+00000460: 0029 0272 0f00 0000 7210 0000 0072 1500  .).r....r....r..
+00000470: 0000 7215 0000 0072 1600 0000 da08 6c6f  ..r....r......lo
+00000480: 6164 5f73 696d 1800 0000 7302 0000 000c  ad_sim....s.....
+00000490: 027a 1b44 6174 6166 7261 6d65 4d61 6b65  .z.DataframeMake
+000004a0: 7246 6f61 6d2e 6c6f 6164 5f73 696d 4e29  rFoam.load_simN)
+000004b0: 06da 085f 5f6e 616d 655f 5fda 0a5f 5f6d  ...__name__..__m
+000004c0: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
+000004d0: 616d 655f 5f72 1700 0000 7218 0000 0072  ame__r....r....r
+000004e0: 1a00 0000 7215 0000 0072 1500 0000 7215  ....r....r....r.
+000004f0: 0000 0072 1600 0000 7206 0000 0008 0000  ...r....r.......
+00000500: 0073 0800 0000 0800 0801 0809 0c06 7206  .s............r.
+00000510: 0000 004e 290b da07 5f5f 646f 635f 5f5a  ...N)...__doc__Z
+00000520: 2966 6c75 6964 7369 6d5f 636f 7265 2e6f  )fluidsim_core.o
+00000530: 7574 7075 742e 6461 7461 6672 616d 655f  utput.dataframe_
+00000540: 6672 6f6d 5f70 6174 6873 7202 0000 00da  from_pathsr.....
+00000550: 0c66 6c75 6964 7369 6d66 6f61 6d72 0400  .fluidsimfoamr..
+00000560: 0000 5a17 666c 7569 6473 696d 666f 616d  ..Z.fluidsimfoam
+00000570: 2e6f 7574 7075 742e 6c6f 6772 0500 0000  .output.logr....
+00000580: 7206 0000 005a 105f 6461 7461 6672 616d  r....Z._datafram
+00000590: 655f 6d61 6b65 72da 1967 6574 5f6d 6561  e_maker..get_mea
+000005a0: 6e5f 7661 6c75 6573 5f66 726f 6d5f 7061  n_values_from_pa
+000005b0: 7468 da18 6765 745f 6461 7461 6672 616d  th..get_datafram
+000005c0: 655f 6672 6f6d 5f70 6174 6873 7215 0000  e_from_pathsr...
+000005d0: 0072 1500 0000 7215 0000 0072 1600 0000  .r....r....r....
+000005e0: da08 3c6d 6f64 756c 653e 0100 0000 7310  ..<module>....s.
+000005f0: 0000 0004 000c 020c 010c 0110 0306 1506  ................
+00000600: 020a 01                                  ...
```

### Comparing `fluidsimfoam-0.0.5/src/fluidsimfoam/output/__pycache__/fields.cpython-39.pyc` & `fluidsimfoam-0.0.6/src/fluidsimfoam/output/__pycache__/fields.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun  1 13:07:51 2023 UTC, .py size: 3046 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 2798 7864 e60b 0000  a.......'.xd....
+00000000: 6f0d 0d0a 0000 0000 0d32 8064 b60b 0000  o........2.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 5a00 0000 6400  .....@...sZ...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 0100 6401 6404 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 6d06 5a06 0100 6401 6402 6c07 6d08 5a09  m.Z...d.d.l.m.Z.
 00000060: 0100 6401 6405 6c0a 6d0b 5a0b 0100 6406  ..d.d.l.m.Z...d.
 00000070: 6407 8400 5a0c 4700 6408 6409 8400 6409  d...Z.G.d.d...d.
@@ -13,208 +13,208 @@
 000000c0: 4e75 6d62 6572 2902 da04 5049 5045 da03  Number)...PIPE..
 000000d0: 7275 6e29 01da 0f72 6561 645f 6669 656c  run)...read_fiel
 000000e0: 645f 6669 6c65 6301 0000 0000 0000 0000  d_filec.........
 000000f0: 0000 0001 0000 0003 0000 0043 0000 0073  ...........C...s
 00000100: 1200 0000 7400 6401 6402 8400 7c00 4400  ....t.d.d...|.D.
 00000110: 8301 8301 5300 2903 4e63 0100 0000 0000  ....S.).Nc......
 00000120: 0000 0000 0000 0200 0000 0300 0000 7300  ..............s.
-00000130: 0000 731e 0000 007c 005d 167d 017c 01a0  ..s....|.].}.|..
-00000140: 00a1 0070 147c 0164 006b 0256 0001 0071  ...p.|.d.k.V...q
-00000150: 0264 0153 0029 02da 012e 4e29 01da 0769  .d.S.)....N)...i
-00000160: 7364 6967 6974 2902 da02 2e30 da01 63a9  sdigit)....0..c.
-00000170: 0072 0a00 0000 fa48 2f68 6f6d 652f 7573  .r.....H/home/us
-00000180: 6572 732f 6175 6769 6572 3370 692f 4465  ers/augier3pi/De
-00000190: 762f 666c 7569 6473 696d 666f 616d 2f73  v/fluidsimfoam/s
-000001a0: 7263 2f66 6c75 6964 7369 6d66 6f61 6d2f  rc/fluidsimfoam/
-000001b0: 6f75 7470 7574 2f66 6965 6c64 732e 7079  output/fields.py
-000001c0: da09 3c67 656e 6578 7072 3e0d 0000 00f3  ..<genexpr>.....
-000001d0: 0000 0000 7a1f 6973 5f74 696d 655f 6e61  ....z.is_time_na
-000001e0: 6d65 2e3c 6c6f 6361 6c73 3e2e 3c67 656e  me.<locals>.<gen
-000001f0: 6578 7072 3e29 01da 0361 6c6c 2901 da04  expr>)...all)...
-00000200: 6e61 6d65 720a 0000 0072 0a00 0000 720b  namer....r....r.
-00000210: 0000 00da 0c69 735f 7469 6d65 5f6e 616d  .....is_time_nam
-00000220: 650c 0000 0073 0200 0000 0001 7210 0000  e....s......r...
-00000230: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
-00000240: 0000 0300 0000 4000 0000 7344 0000 0065  ......@...sD...e
-00000250: 005a 0164 005a 0264 0164 0284 005a 0364  .Z.d.Z.d.d...Z.d
-00000260: 0364 0484 005a 0464 0f64 0764 0884 015a  .d...Z.d.d.d...Z
-00000270: 0564 1064 0964 0a84 015a 0664 1164 0b64  .d.d.d...Z.d.d.d
-00000280: 0c84 015a 0764 1264 0d64 0e84 015a 0864  ...Z.d.d.d...Z.d
-00000290: 0653 0029 13da 0646 6965 6c64 7363 0200  .S.)...Fieldsc..
-000002a0: 0000 0000 0000 0000 0000 0200 0000 0200  ................
-000002b0: 0000 4300 0000 7312 0000 007c 017c 005f  ..C...s....|.|._
-000002c0: 007c 016a 017c 005f 0164 0053 00a9 014e  .|.j.|._.d.S...N
-000002d0: 2902 da06 6f75 7470 7574 da03 7369 6d29  )...output..sim)
-000002e0: 02da 0473 656c 6672 1300 0000 720a 0000  ...selfr....r...
-000002f0: 0072 0a00 0000 720b 0000 00da 085f 5f69  .r....r......__i
-00000300: 6e69 745f 5f11 0000 0073 0400 0000 0001  nit__....s......
-00000310: 0601 7a0f 4669 656c 6473 2e5f 5f69 6e69  ..z.Fields.__ini
-00000320: 745f 5f63 0100 0000 0000 0000 0000 0000  t__c............
-00000330: 0200 0000 0500 0000 4300 0000 7336 0000  ........C...s6..
-00000340: 007c 006a 006a 016a 026a 0364 016b 0472  .|.j.j.j.j.d.k.r
-00000350: 1664 027d 016e 0464 037d 0174 0464 0464  .d.}.n.d.}.t.d.d
-00000360: 0584 007c 006a 056a 06a0 077c 01a1 0144  ...|.j.j...|...D
-00000370: 0083 0183 0153 0029 064e e901 0000 007a  .....S.).N.....z
-00000380: 0c70 726f 6365 7373 6f72 302f 2ada 012a  .processor0/*..*
-00000390: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
-000003a0: 0003 0000 0073 0000 0073 2200 0000 7c00  .....s...s"...|.
-000003b0: 5d1a 7d01 7400 7c01 6a01 8301 7202 7402  ].}.t.|.j...r.t.
-000003c0: 7c01 6a01 8301 5600 0100 7102 6400 5300  |.j...V...q.d.S.
-000003d0: 7212 0000 0029 0372 1000 0000 720f 0000  r....).r....r...
-000003e0: 00da 0566 6c6f 6174 a902 7208 0000 00da  ...float..r.....
-000003f0: 0470 6174 6872 0a00 0000 720a 0000 0072  .pathr....r....r
-00000400: 0b00 0000 720c 0000 001b 0000 0073 0600  ....r........s..
-00000410: 0000 0402 0201 0afe 7a29 4669 656c 6473  ........z)Fields
-00000420: 2e67 6574 5f73 6176 6564 5f74 696d 6573  .get_saved_times
-00000430: 2e3c 6c6f 6361 6c73 3e2e 3c67 656e 6578  .<locals>.<genex
-00000440: 7072 3e29 0872 1400 0000 da06 7061 7261  pr>).r......para
-00000450: 6d73 da08 7061 7261 6c6c 656c da08 6e73  ms..parallel..ns
-00000460: 7562 646f 6d73 da06 736f 7274 6564 7213  ubdoms..sortedr.
-00000470: 0000 00da 0870 6174 685f 7275 6eda 0467  .....path_run..g
-00000480: 6c6f 6229 0272 1500 0000 da08 7374 725f  lob).r......str_
-00000490: 676c 6f62 720a 0000 0072 0a00 0000 720b  globr....r....r.
-000004a0: 0000 00da 0f67 6574 5f73 6176 6564 5f74  .....get_saved_t
-000004b0: 696d 6573 1500 0000 730c 0000 0000 0110  imes....s.......
-000004c0: 0106 0204 0208 020c fe7a 1646 6965 6c64  .........z.Field
-000004d0: 732e 6765 745f 7361 7665 645f 7469 6d65  s.get_saved_time
-000004e0: 73da 046c 6173 744e 6303 0000 0000 0000  s..lastNc.......
-000004f0: 0000 0000 0007 0000 0005 0000 0043 0000  .............C..
-00000500: 0073 6000 0000 7c01 6401 6b03 720c 7400  .s`...|.d.k.r.t.
-00000510: 8201 7c02 6400 7500 721a 6402 7d03 6e08  ..|.d.u.r.d.}.n.
-00000520: 7c02 6403 1700 7d03 7401 6404 6405 8400  |.d...}.t.d.d...
-00000530: 7c00 6a02 6a03 a004 7c03 a101 4400 8301  |.j.j...|...D...
-00000540: 6406 6407 8400 6408 8d02 7d04 7c04 6409  d.d...d...}.|.d.
-00000550: 1900 7d05 7405 7c05 6a06 8301 7d06 7c05  ..}.t.|.j...}.|.
-00000560: 7c06 6602 5300 290a 4e72 2400 0000 7218  |.f.S.).Nr$...r.
-00000570: 0000 007a 022f 2a63 0100 0000 0000 0000  ...z./*c........
-00000580: 0000 0000 0200 0000 0300 0000 7300 0000  ............s...
-00000590: 7320 0000 007c 005d 187d 017c 016a 0064  s ...|.].}.|.j.d
-000005a0: 0019 00a0 01a1 0072 027c 0156 0001 0071  .......r.|.V...q
-000005b0: 0264 0153 0029 0272 0100 0000 4e29 0272  .d.S.).r....N).r
-000005c0: 0f00 0000 7207 0000 0072 1a00 0000 720a  ....r....r....r.
-000005d0: 0000 0072 0a00 0000 720b 0000 0072 0c00  ...r....r....r..
-000005e0: 0000 2b00 0000 7306 0000 0004 0202 010e  ..+...s.........
-000005f0: fe7a 2b46 6965 6c64 732e 6765 745f 7061  .z+Fields.get_pa
-00000600: 7468 5f64 6972 5f74 696d 652e 3c6c 6f63  th_dir_time.<loc
-00000610: 616c 733e 2e3c 6765 6e65 7870 723e 6301  als>.<genexpr>c.
-00000620: 0000 0000 0000 0000 0000 0001 0000 0002  ................
-00000630: 0000 0053 0000 0073 0a00 0000 7400 7c00  ...S...s....t.|.
-00000640: 6a01 8301 5300 7212 0000 0029 0272 1900  j...S.r....).r..
-00000650: 0000 720f 0000 0029 01da 0170 720a 0000  ..r....)...pr...
-00000660: 0072 0a00 0000 720b 0000 00da 083c 6c61  .r....r......<la
-00000670: 6d62 6461 3e30 0000 0072 0d00 0000 7a2a  mbda>0...r....z*
-00000680: 4669 656c 6473 2e67 6574 5f70 6174 685f  Fields.get_path_
-00000690: 6469 725f 7469 6d65 2e3c 6c6f 6361 6c73  dir_time.<locals
-000006a0: 3e2e 3c6c 616d 6264 613e 2901 da03 6b65  >.<lambda>)...ke
-000006b0: 79e9 ffff ffff 2907 da13 4e6f 7449 6d70  y.....)...NotImp
-000006c0: 6c65 6d65 6e74 6564 4572 726f 7272 1f00  lementedErrorr..
-000006d0: 0000 7213 0000 0072 2000 0000 7221 0000  ..r....r ...r!..
-000006e0: 0072 1900 0000 720f 0000 0029 0772 1500  .r....r....).r..
-000006f0: 0000 da0b 7469 6d65 5f61 7070 726f 78da  ....time_approx.
-00000700: 0764 6972 6e61 6d65 7222 0000 005a 0a70  .dirnamer"...Z.p
-00000710: 6174 685f 7469 6d65 73da 0870 6174 685f  ath_times..path_
-00000720: 6469 72da 096c 6173 745f 7469 6d65 720a  dir..last_timer.
-00000730: 0000 0072 0a00 0000 720b 0000 00da 1167  ...r....r......g
-00000740: 6574 5f70 6174 685f 6469 725f 7469 6d65  et_path_dir_time
-00000750: 2100 0000 731c 0000 0000 0108 0104 0208  !...s...........
-00000760: 0106 0208 0202 0106 020c fe04 0506 fa06  ................
-00000770: 0808 010a 017a 1846 6965 6c64 732e 6765  .....z.Fields.ge
-00000780: 745f 7061 7468 5f64 6972 5f74 696d 6563  t_path_dir_timec
-00000790: 0300 0000 0000 0000 0000 0000 0800 0000  ................
-000007a0: 0400 0000 4300 0000 739a 0000 007c 0264  ....C...s....|.d
-000007b0: 016b 0372 0c74 0082 017c 00a0 017c 02a1  .k.r.t...|...|..
-000007c0: 015c 027d 037d 047c 006a 026a 036a 046a  .\.}.}.|.j.j.j.j
-000007d0: 0564 026b 0472 547c 006a 017c 0264 0364  .d.k.rT|.j.|.d.d
-000007e0: 048d 025c 027d 057d 067c 067c 046b 0372  ...\.}.}.|.|.k.r
-000007f0: 547c 006a 067c 0167 017c 0664 058d 0201  T|.j.|.g.|.d....
-00000800: 007c 00a0 017c 02a1 015c 027d 037d 047c  .|...|...\.}.}.|
-00000810: 006a 026a 036a 046a 0564 026b 0472 7e7c  .j.j.j.j.d.k.r~|
-00000820: 047c 066b 0273 7e4a 0082 0174 077c 037c  .|.k.s~J...t.|.|
-00000830: 011b 0083 017d 0774 087c 036a 0983 017c  .....}.t.|.j...|
-00000840: 075f 0a7c 0753 0029 064e 7224 0000 0072  ._.|.S.).Nr$...r
-00000850: 1700 0000 5a0a 7072 6f63 6573 736f 7230  ....Z.processor0
-00000860: 2901 722b 0000 0029 02da 0666 6965 6c64  ).r+...)...field
-00000870: 73da 0474 696d 6529 0b72 2900 0000 722e  s..time).r)...r.
-00000880: 0000 0072 1400 0000 721c 0000 0072 1d00  ...r....r....r..
-00000890: 0000 721e 0000 00da 0f72 6563 6f6e 7374  ..r......reconst
-000008a0: 7275 6374 5f70 6172 7205 0000 0072 1900  ruct_parr....r..
-000008b0: 0000 720f 0000 0072 3000 0000 2908 7215  ..r....r0...).r.
-000008c0: 0000 0072 0f00 0000 722a 0000 0072 2c00  ...r....r*...r,.
-000008d0: 0000 722d 0000 00da 015f 5a0f 6c61 7374  ..r-....._Z.last
-000008e0: 5f74 696d 655f 7072 6f63 30da 0566 6965  _time_proc0..fie
-000008f0: 6c64 720a 0000 0072 0a00 0000 720b 0000  ldr....r....r...
-00000900: 00da 0a72 6561 645f 6669 656c 6436 0000  ...read_field6..
-00000910: 0073 1e00 0000 0001 0801 0402 0e02 1001  .s..............
-00000920: 0401 04ff 0a04 0801 1002 0e01 1001 0c02  ................
-00000930: 0c01 0c01 7a11 4669 656c 6473 2e72 6561  ....z.Fields.rea
-00000940: 645f 6669 656c 6463 0400 0000 0000 0000  d_fieldc........
-00000950: 0000 0000 0600 0000 0700 0000 4300 0000  ............C...
-00000960: 73a8 0000 0074 00a0 0164 01a1 017d 047c  s....t...d...}.|
-00000970: 0464 0075 0072 1a74 0264 0283 0182 0164  .d.u.r.t.d.....d
-00000980: 0167 017d 057c 0164 0075 0172 447c 05a0  .g.}.|.d.u.rD|..
-00000990: 0364 0364 0464 05a0 047c 01a1 019b 0064  .d.d.d...|.....d
-000009a0: 069d 0367 02a1 0101 007c 0264 0075 0172  ...g.....|.d.u.r
-000009b0: 587c 0364 0075 0172 5874 0582 017c 0264  X|.d.u.rXt...|.d
-000009c0: 0075 0172 6a7c 05a0 0664 07a1 0101 007c  .u.rj|...d.....|
-000009d0: 0364 0075 0172 9274 077c 0374 0883 0272  .d.u.r.t.|.t...r
-000009e0: 8474 097c 0383 017d 037c 05a0 0364 087c  .t.|...}.|...d.|
-000009f0: 0367 02a1 0101 0074 0a7c 057c 006a 0b6a  .g.....t.|.|.j.j
-00000a00: 0c74 0d64 098d 0301 0064 0053 0029 0a4e  .t.d.....d.S.).N
-00000a10: 5a0e 7265 636f 6e73 7472 7563 7450 6172  Z.reconstructPar
-00000a20: 7a16 4f70 656e 464f 414d 206e 6f74 2061  z.OpenFOAM not a
-00000a30: 7661 696c 6162 6c65 7a07 2d66 6965 6c64  vailablez.-field
-00000a40: 73fa 0128 fa01 20fa 0129 7a0b 2d6c 6174  s..(.. ..)z.-lat
-00000a50: 6573 7454 696d 657a 052d 7469 6d65 2902  estTimez.-time).
-00000a60: da03 6377 64da 0673 7464 6f75 7429 0eda  ..cwd..stdout)..
-00000a70: 0673 6875 7469 6cda 0577 6869 6368 da0c  .shutil..which..
-00000a80: 5275 6e74 696d 6545 7272 6f72 da06 6578  RuntimeError..ex
-00000a90: 7465 6e64 da04 6a6f 696e da0a 5661 6c75  tend..join..Valu
-00000aa0: 6545 7272 6f72 da06 6170 7065 6e64 da0a  eError..append..
-00000ab0: 6973 696e 7374 616e 6365 7202 0000 00da  isinstancer.....
-00000ac0: 0373 7472 7204 0000 0072 1400 0000 7220  .strr....r....r 
-00000ad0: 0000 0072 0300 0000 2906 7215 0000 0072  ...r....).r....r
-00000ae0: 2f00 0000 5a0b 6c61 7465 7374 5f74 696d  /...Z.latest_tim
-00000af0: 6572 3000 0000 5a0c 7061 7468 5f63 6f6d  er0...Z.path_com
-00000b00: 6d61 6e64 da07 636f 6d6d 616e 6472 0a00  mand..commandr..
-00000b10: 0000 720a 0000 0072 0b00 0000 7231 0000  ..r....r....r1..
-00000b20: 004c 0000 0073 1e00 0000 0001 0a02 0801  .L...s..........
-00000b30: 0802 0602 0801 1c02 1001 0402 0801 0a02  ................
-00000b40: 0801 0a01 0802 0e02 7a16 4669 656c 6473  ........z.Fields
-00000b50: 2e72 6563 6f6e 7374 7275 6374 5f70 6172  .reconstruct_par
-00000b60: 6303 0000 0000 0000 0000 0000 0009 0000  c...............
-00000b70: 0005 0000 0043 0000 0073 4000 0000 7c00  .....C...s@...|.
-00000b80: a000 7c01 7c02 a102 7d03 7c00 6a01 6a02  ..|.|...}.|.j.j.
-00000b90: 6a03 a004 a100 5c03 7d04 7d05 7d06 7405  j.....\.}.}.}.t.
-00000ba0: a006 a100 5c02 7d07 7d08 7c08 a007 7c05  ....\.}.}.|...|.
-00000bb0: 7c03 a008 a100 a102 0100 6400 5300 7212  |.........d.S.r.
-00000bc0: 0000 0029 0972 3400 0000 7213 0000 0072  ...).r4...r....r
-00000bd0: 1400 0000 da04 6f70 6572 da10 6765 745f  ......oper..get_
-00000be0: 6365 6c6c 735f 636f 6f72 6473 da03 706c  cells_coords..pl
-00000bf0: 74da 0873 7562 706c 6f74 73da 0470 6c6f  t..subplots..plo
-00000c00: 74da 0967 6574 5f61 7272 6179 2909 7215  t..get_array).r.
-00000c10: 0000 0072 0f00 0000 722a 0000 0072 3300  ...r....r*...r3.
-00000c20: 0000 da01 78da 0179 da01 7ada 0366 6967  ....x..y..z..fig
-00000c30: da02 6178 720a 0000 0072 0a00 0000 720b  ..axr....r....r.
-00000c40: 0000 00da 0a70 6c6f 745f 6669 656c 6465  .....plot_fielde
-00000c50: 0000 0073 0800 0000 0001 0c02 1402 0c02  ...s............
-00000c60: 7a11 4669 656c 6473 2e70 6c6f 745f 6669  z.Fields.plot_fi
-00000c70: 656c 6429 0272 2400 0000 4e29 0172 2400  eld).r$...N).r$.
-00000c80: 0000 2903 4e4e 4e29 0172 2400 0000 2909  ..).NNN).r$...).
-00000c90: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
-00000ca0: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
-00000cb0: 6d65 5f5f 7216 0000 0072 2300 0000 722e  me__r....r#...r.
-00000cc0: 0000 0072 3400 0000 7231 0000 0072 4f00  ...r4...r1...rO.
-00000cd0: 0000 720a 0000 0072 0a00 0000 720a 0000  ..r....r....r...
-00000ce0: 0072 0b00 0000 7211 0000 0010 0000 0073  .r....r........s
-00000cf0: 0c00 0000 0801 0804 080c 0a15 0a16 0a19  ................
-00000d00: 7211 0000 0029 0eda 075f 5f64 6f63 5f5f  r....)...__doc__
-00000d10: 723a 0000 00da 076e 756d 6265 7273 7202  r:.....numbersr.
-00000d20: 0000 00da 0a73 7562 7072 6f63 6573 7372  .....subprocessr
-00000d30: 0300 0000 7204 0000 00da 116d 6174 706c  ....r......matpl
-00000d40: 6f74 6c69 622e 7079 706c 6f74 da06 7079  otlib.pyplot..py
-00000d50: 706c 6f74 7246 0000 00da 1d66 6c75 6964  plotrF.....fluid
-00000d60: 7369 6d66 6f61 6d2e 666f 616d 5f69 6e70  simfoam.foam_inp
-00000d70: 7574 5f66 696c 6573 7205 0000 0072 1000  ut_filesr....r..
-00000d80: 0000 7211 0000 0072 0a00 0000 720a 0000  ..r....r....r...
-00000d90: 0072 0a00 0000 720b 0000 00da 083c 6d6f  .r....r......<mo
-00000da0: 6475 6c65 3e01 0000 0073 0e00 0000 0402  dule>....s......
-00000db0: 0801 0c01 1002 0c02 0c03 0804            ............
+00000130: 0000 7320 0000 0081 007c 005d 0b7d 017c  ..s .....|.].}.|
+00000140: 01a0 00a1 0070 0b7c 0164 006b 0256 0001  .....p.|.d.k.V..
+00000150: 0071 0264 0153 0029 02da 012e 4e29 01da  .q.d.S.)....N)..
+00000160: 0769 7364 6967 6974 2902 da02 2e30 da01  .isdigit)....0..
+00000170: 63a9 0072 0a00 0000 fa3f 2f68 6f6d 652f  c..r.....?/home/
+00000180: 7069 6572 7265 2f44 6576 2f66 6c75 6964  pierre/Dev/fluid
+00000190: 7369 6d66 6f61 6d2f 7372 632f 666c 7569  simfoam/src/flui
+000001a0: 6473 696d 666f 616d 2f6f 7574 7075 742f  dsimfoam/output/
+000001b0: 6669 656c 6473 2e70 79da 093c 6765 6e65  fields.py..<gene
+000001c0: 7870 723e 0d00 0000 7304 0000 0002 801e  xpr>....s.......
+000001d0: 007a 1f69 735f 7469 6d65 5f6e 616d 652e  .z.is_time_name.
+000001e0: 3c6c 6f63 616c 733e 2e3c 6765 6e65 7870  <locals>.<genexp
+000001f0: 723e 2901 da03 616c 6c29 01da 046e 616d  r>)...all)...nam
+00000200: 6572 0a00 0000 720a 0000 0072 0b00 0000  er....r....r....
+00000210: da0c 6973 5f74 696d 655f 6e61 6d65 0c00  ..is_time_name..
+00000220: 0000 7302 0000 0012 0172 0f00 0000 6300  ..s......r....c.
+00000230: 0000 0000 0000 0000 0000 0000 0000 0003  ................
+00000240: 0000 0040 0000 0073 4400 0000 6500 5a01  ...@...sD...e.Z.
+00000250: 6400 5a02 6401 6402 8400 5a03 6403 6404  d.Z.d.d...Z.d.d.
+00000260: 8400 5a04 640f 6407 6408 8401 5a05 6410  ..Z.d.d.d...Z.d.
+00000270: 6409 640a 8401 5a06 6411 640b 640c 8401  d.d...Z.d.d.d...
+00000280: 5a07 6410 640d 640e 8401 5a08 6406 5300  Z.d.d.d...Z.d.S.
+00000290: 2912 da06 4669 656c 6473 6302 0000 0000  )...Fieldsc.....
+000002a0: 0000 0000 0000 0002 0000 0002 0000 0043  ...............C
+000002b0: 0000 0073 1200 0000 7c01 7c00 5f00 7c01  ...s....|.|._.|.
+000002c0: 6a01 7c00 5f01 6400 5300 a901 4e29 02da  j.|._.d.S...N)..
+000002d0: 066f 7574 7075 74da 0373 696d 2902 da04  .output..sim)...
+000002e0: 7365 6c66 7212 0000 0072 0a00 0000 720a  selfr....r....r.
+000002f0: 0000 0072 0b00 0000 da08 5f5f 696e 6974  ...r......__init
+00000300: 5f5f 1100 0000 7304 0000 0006 010c 017a  __....s........z
+00000310: 0f46 6965 6c64 732e 5f5f 696e 6974 5f5f  .Fields.__init__
+00000320: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
+00000330: 0005 0000 0043 0000 0073 3600 0000 7c00  .....C...s6...|.
+00000340: 6a00 6a01 6a02 6a03 6401 6b04 720b 6402  j.j.j.j.d.k.r.d.
+00000350: 7d01 6e02 6403 7d01 7404 6404 6405 8400  }.n.d.}.t.d.d...
+00000360: 7c00 6a05 6a06 a007 7c01 a101 4400 8301  |.j.j...|...D...
+00000370: 8301 5300 2906 4ee9 0100 0000 7a0c 7072  ..S.).N.....z.pr
+00000380: 6f63 6573 736f 7230 2f2a da01 2a63 0100  ocessor0/*..*c..
+00000390: 0000 0000 0000 0000 0000 0200 0000 0300  ................
+000003a0: 0000 7300 0000 7324 0000 0081 007c 005d  ..s...s$.....|.]
+000003b0: 0d7d 0174 007c 016a 0183 0172 0274 027c  .}.t.|.j...r.t.|
+000003c0: 016a 0183 0156 0001 0071 0264 0053 0072  .j...V...q.d.S.r
+000003d0: 1100 0000 2903 720f 0000 0072 0e00 0000  ....).r....r....
+000003e0: da05 666c 6f61 74a9 0272 0800 0000 da04  ..float..r......
+000003f0: 7061 7468 720a 0000 0072 0a00 0000 720b  pathr....r....r.
+00000400: 0000 0072 0c00 0000 1b00 0000 730e 0000  ...r........s...
+00000410: 0002 8004 0002 0208 0102 fd08 010a ff7a  ...............z
+00000420: 2946 6965 6c64 732e 6765 745f 7361 7665  )Fields.get_save
+00000430: 645f 7469 6d65 732e 3c6c 6f63 616c 733e  d_times.<locals>
+00000440: 2e3c 6765 6e65 7870 723e 2908 7213 0000  .<genexpr>).r...
+00000450: 00da 0670 6172 616d 73da 0870 6172 616c  ...params..paral
+00000460: 6c65 6cda 086e 7375 6264 6f6d 73da 0673  lel..nsubdoms..s
+00000470: 6f72 7465 6472 1200 0000 da08 7061 7468  ortedr......path
+00000480: 5f72 756e da04 676c 6f62 2902 7214 0000  _run..glob).r...
+00000490: 00da 0873 7472 5f67 6c6f 6272 0a00 0000  ...str_globr....
+000004a0: 720a 0000 0072 0b00 0000 da0f 6765 745f  r....r......get_
+000004b0: 7361 7665 645f 7469 6d65 7315 0000 0073  saved_times....s
+000004c0: 0c00 0000 1001 0601 0402 0802 0c02 08fe  ................
+000004d0: 7a16 4669 656c 6473 2e67 6574 5f73 6176  z.Fields.get_sav
+000004e0: 6564 5f74 696d 6573 da04 6c61 7374 4e63  ed_times..lastNc
+000004f0: 0300 0000 0000 0000 0000 0000 0700 0000  ................
+00000500: 0500 0000 4300 0000 7360 0000 007c 0164  ....C...s`...|.d
+00000510: 016b 0372 0674 0082 017c 0264 0075 0072  .k.r.t...|.d.u.r
+00000520: 0d64 027d 036e 047c 0264 0317 007d 0374  .d.}.n.|.d...}.t
+00000530: 0164 0464 0584 007c 006a 026a 03a0 047c  .d.d...|.j.j...|
+00000540: 03a1 0144 0083 0164 0664 0784 0064 088d  ...D...d.d...d..
+00000550: 027d 047c 0464 0919 007d 0574 057c 056a  .}.|.d...}.t.|.j
+00000560: 0683 017d 067c 057c 0666 0253 0029 0a4e  ...}.|.|.f.S.).N
+00000570: 7223 0000 0072 1700 0000 7a02 2f2a 6301  r#...r....z./*c.
+00000580: 0000 0000 0000 0000 0000 0002 0000 0003  ................
+00000590: 0000 0073 0000 0073 2200 0000 8100 7c00  ...s...s".....|.
+000005a0: 5d0c 7d01 7c01 6a00 6400 1900 a001 a100  ].}.|.j.d.......
+000005b0: 7202 7c01 5600 0100 7102 6401 5300 2902  r.|.V...q.d.S.).
+000005c0: 7201 0000 004e 2902 720e 0000 0072 0700  r....N).r....r..
+000005d0: 0000 7219 0000 0072 0a00 0000 720a 0000  ..r....r....r...
+000005e0: 0072 0b00 0000 720c 0000 002b 0000 0073  .r....r....+...s
+000005f0: 0e00 0000 0280 0400 0202 0c01 02fd 0201  ................
+00000600: 0aff 7a2b 4669 656c 6473 2e67 6574 5f70  ..z+Fields.get_p
+00000610: 6174 685f 6469 725f 7469 6d65 2e3c 6c6f  ath_dir_time.<lo
+00000620: 6361 6c73 3e2e 3c67 656e 6578 7072 3e63  cals>.<genexpr>c
+00000630: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+00000640: 0200 0000 5300 0000 730a 0000 0074 007c  ....S...s....t.|
+00000650: 006a 0183 0153 0072 1100 0000 2902 7218  .j...S.r....).r.
+00000660: 0000 0072 0e00 0000 2901 da01 7072 0a00  ...r....)...pr..
+00000670: 0000 720a 0000 0072 0b00 0000 da08 3c6c  ..r....r......<l
+00000680: 616d 6264 613e 3000 0000 7302 0000 000a  ambda>0...s.....
+00000690: 007a 2a46 6965 6c64 732e 6765 745f 7061  .z*Fields.get_pa
+000006a0: 7468 5f64 6972 5f74 696d 652e 3c6c 6f63  th_dir_time.<loc
+000006b0: 616c 733e 2e3c 6c61 6d62 6461 3e29 01da  als>.<lambda>)..
+000006c0: 036b 6579 e9ff ffff ff29 07da 134e 6f74  .key.....)...Not
+000006d0: 496d 706c 656d 656e 7465 6445 7272 6f72  ImplementedError
+000006e0: 721e 0000 0072 1200 0000 721f 0000 0072  r....r....r....r
+000006f0: 2000 0000 7218 0000 0072 0e00 0000 2907   ...r....r....).
+00000700: 7214 0000 00da 0b74 696d 655f 6170 7072  r......time_appr
+00000710: 6f78 da07 6469 726e 616d 6572 2100 0000  ox..dirnamer!...
+00000720: 5a0a 7061 7468 5f74 696d 6573 da08 7061  Z.path_times..pa
+00000730: 7468 5f64 6972 da09 6c61 7374 5f74 696d  th_dir..last_tim
+00000740: 6572 0a00 0000 720a 0000 0072 0b00 0000  er....r....r....
+00000750: da11 6765 745f 7061 7468 5f64 6972 5f74  ..get_path_dir_t
+00000760: 696d 6521 0000 0073 1c00 0000 0801 0401  ime!...s........
+00000770: 0802 0601 0802 0202 0601 0c02 04fe 0605  ................
+00000780: 06fa 0808 0a01 0801 7a18 4669 656c 6473  ........z.Fields
+00000790: 2e67 6574 5f70 6174 685f 6469 725f 7469  .get_path_dir_ti
+000007a0: 6d65 6303 0000 0000 0000 0000 0000 0008  mec.............
+000007b0: 0000 0004 0000 0043 0000 0073 8a00 0000  .......C...s....
+000007c0: 7c02 6401 6b03 7206 7400 8201 7c00 a001  |.d.k.r.t...|...
+000007d0: 7c02 a101 5c02 7d03 7d04 7c00 6a02 6a03  |...\.}.}.|.j.j.
+000007e0: 6a04 6a05 6402 6b04 7237 7c00 6a01 7c02  j.j.d.k.r7|.j.|.
+000007f0: 6403 6404 8d02 5c02 7d05 7d06 7c06 7c04  d.d...\.}.}.|.|.
+00000800: 6b03 722a 7c00 6a06 7c01 6701 7c06 6405  k.r*|.j.|.g.|.d.
+00000810: 8d02 0100 7c00 a001 7c02 a101 5c02 7d03  ....|...|...\.}.
+00000820: 7d04 7c04 7c06 6b02 7337 4a00 8201 7407  }.|.|.k.s7J...t.
+00000830: 7c03 7c01 1b00 8301 7d07 7408 7c03 6a09  |.|.....}.t.|.j.
+00000840: 8301 7c07 5f0a 7c07 5300 2906 4e72 2300  ..|._.|.S.).Nr#.
+00000850: 0000 7216 0000 005a 0a70 726f 6365 7373  ..r....Z.process
+00000860: 6f72 3029 0172 2a00 0000 2902 da06 6669  or0).r*...)...fi
+00000870: 656c 6473 da04 7469 6d65 290b 7228 0000  elds..time).r(..
+00000880: 0072 2d00 0000 7213 0000 0072 1b00 0000  .r-...r....r....
+00000890: 721c 0000 0072 1d00 0000 da0f 7265 636f  r....r......reco
+000008a0: 6e73 7472 7563 745f 7061 7272 0500 0000  nstruct_parr....
+000008b0: 7218 0000 0072 0e00 0000 722f 0000 0029  r....r....r/...)
+000008c0: 0872 1400 0000 720e 0000 0072 2900 0000  .r....r....r)...
+000008d0: 722b 0000 0072 2c00 0000 da01 5f5a 0f6c  r+...r,....._Z.l
+000008e0: 6173 745f 7469 6d65 5f70 726f 6330 da05  ast_time_proc0..
+000008f0: 6669 656c 6472 0a00 0000 720a 0000 0072  fieldr....r....r
+00000900: 0b00 0000 da0a 7265 6164 5f66 6965 6c64  ......read_field
+00000910: 3600 0000 731c 0000 0008 0104 010e 0210  6...s...........
+00000920: 0204 0104 010a ff08 0310 010e 010c 010c  ................
+00000930: 020c 0104 017a 1146 6965 6c64 732e 7265  .....z.Fields.re
+00000940: 6164 5f66 6965 6c64 6304 0000 0000 0000  ad_fieldc.......
+00000950: 0000 0000 0006 0000 0007 0000 0043 0000  .............C..
+00000960: 0073 a800 0000 7400 a001 6401 a101 7d04  .s....t...d...}.
+00000970: 7c04 6400 7500 720d 7402 6402 8301 8201  |.d.u.r.t.d.....
+00000980: 6401 6701 7d05 7c01 6400 7501 7222 7c05  d.g.}.|.d.u.r"|.
+00000990: a003 6403 6404 6405 a004 7c01 a101 9b00  ..d.d.d...|.....
+000009a0: 6406 9d03 6702 a101 0100 7c02 6400 7501  d...g.....|.d.u.
+000009b0: 722c 7c03 6400 7501 722c 7405 8201 7c02  r,|.d.u.r,t...|.
+000009c0: 6400 7501 7235 7c05 a006 6407 a101 0100  d.u.r5|...d.....
+000009d0: 7c03 6400 7501 7249 7407 7c03 7408 8302  |.d.u.rIt.|.t...
+000009e0: 7242 7409 7c03 8301 7d03 7c05 a003 6408  rBt.|...}.|...d.
+000009f0: 7c03 6702 a101 0100 740a 7c05 7c00 6a0b  |.g.....t.|.|.j.
+00000a00: 6a0c 740d 6409 8d03 0100 6400 5300 290a  j.t.d.....d.S.).
+00000a10: 4e5a 0e72 6563 6f6e 7374 7275 6374 5061  NZ.reconstructPa
+00000a20: 727a 164f 7065 6e46 4f41 4d20 6e6f 7420  rz.OpenFOAM not 
+00000a30: 6176 6169 6c61 626c 657a 072d 6669 656c  availablez.-fiel
+00000a40: 6473 fa01 28da 0120 fa01 297a 0b2d 6c61  ds..(.. ..)z.-la
+00000a50: 7465 7374 5469 6d65 7a05 2d74 696d 6529  testTimez.-time)
+00000a60: 02da 0363 7764 da06 7374 646f 7574 290e  ...cwd..stdout).
+00000a70: da06 7368 7574 696c da05 7768 6963 68da  ..shutil..which.
+00000a80: 0c52 756e 7469 6d65 4572 726f 72da 0665  .RuntimeError..e
+00000a90: 7874 656e 64da 046a 6f69 6eda 0a56 616c  xtend..join..Val
+00000aa0: 7565 4572 726f 72da 0661 7070 656e 64da  ueError..append.
+00000ab0: 0a69 7369 6e73 7461 6e63 6572 0200 0000  .isinstancer....
+00000ac0: da03 7374 7272 0400 0000 7213 0000 0072  ..strr....r....r
+00000ad0: 1f00 0000 7203 0000 0029 0672 1400 0000  ....r....).r....
+00000ae0: 722e 0000 005a 0b6c 6174 6573 745f 7469  r....Z.latest_ti
+00000af0: 6d65 722f 0000 005a 0c70 6174 685f 636f  mer/...Z.path_co
+00000b00: 6d6d 616e 64da 0763 6f6d 6d61 6e64 720a  mmand..commandr.
+00000b10: 0000 0072 0a00 0000 720b 0000 0072 3000  ...r....r....r0.
+00000b20: 0000 4900 0000 731e 0000 000a 0108 0208  ..I...s.........
+00000b30: 0106 0208 021c 0110 0204 0108 020a 0108  ................
+00000b40: 020a 0108 010e 0216 027a 1646 6965 6c64  .........z.Field
+00000b50: 732e 7265 636f 6e73 7472 7563 745f 7061  s.reconstruct_pa
+00000b60: 7263 0300 0000 0000 0000 0000 0000 0900  rc..............
+00000b70: 0000 0500 0000 4300 0000 7340 0000 007c  ......C...s@...|
+00000b80: 00a0 007c 017c 02a1 027d 037c 006a 016a  ...|.|...}.|.j.j
+00000b90: 026a 03a0 04a1 005c 037d 047d 057d 0674  .j.....\.}.}.}.t
+00000ba0: 05a0 06a1 005c 027d 077d 087c 08a0 077c  .....\.}.}.|...|
+00000bb0: 057c 03a0 08a1 00a1 0201 0064 0053 0072  .|.........d.S.r
+00000bc0: 1100 0000 2909 7233 0000 0072 1200 0000  ....).r3...r....
+00000bd0: 7213 0000 00da 046f 7065 72da 1067 6574  r......oper..get
+00000be0: 5f63 656c 6c73 5f63 6f6f 7264 73da 0370  _cells_coords..p
+00000bf0: 6c74 da08 7375 6270 6c6f 7473 da04 706c  lt..subplots..pl
+00000c00: 6f74 da09 6765 745f 6172 7261 7929 0972  ot..get_array).r
+00000c10: 1400 0000 720e 0000 0072 2900 0000 7232  ....r....r)...r2
+00000c20: 0000 00da 0178 da01 79da 017a da03 6669  .....x..y..z..fi
+00000c30: 67da 0261 7872 0a00 0000 720a 0000 0072  g..axr....r....r
+00000c40: 0b00 0000 da0a 706c 6f74 5f66 6965 6c64  ......plot_field
+00000c50: 6200 0000 7308 0000 000c 0114 020c 0214  b...s...........
+00000c60: 027a 1146 6965 6c64 732e 706c 6f74 5f66  .z.Fields.plot_f
+00000c70: 6965 6c64 2902 7223 0000 004e 2901 7223  ield).r#...N).r#
+00000c80: 0000 0029 034e 4e4e 2909 da08 5f5f 6e61  ...).NNN)...__na
+00000c90: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
+00000ca0: da0c 5f5f 7175 616c 6e61 6d65 5f5f 7215  ..__qualname__r.
+00000cb0: 0000 0072 2200 0000 722d 0000 0072 3300  ...r"...r-...r3.
+00000cc0: 0000 7230 0000 0072 4e00 0000 720a 0000  ..r0...rN...r...
+00000cd0: 0072 0a00 0000 720a 0000 0072 0b00 0000  .r....r....r....
+00000ce0: 7210 0000 0010 0000 0073 0e00 0000 0800  r........s......
+00000cf0: 0801 0804 0a0c 0a15 0a13 0e19 7210 0000  ............r...
+00000d00: 0029 0eda 075f 5f64 6f63 5f5f 7239 0000  .)...__doc__r9..
+00000d10: 00da 076e 756d 6265 7273 7202 0000 00da  ...numbersr.....
+00000d20: 0a73 7562 7072 6f63 6573 7372 0300 0000  .subprocessr....
+00000d30: 7204 0000 00da 116d 6174 706c 6f74 6c69  r......matplotli
+00000d40: 622e 7079 706c 6f74 da06 7079 706c 6f74  b.pyplot..pyplot
+00000d50: 7245 0000 00da 1d66 6c75 6964 7369 6d66  rE.....fluidsimf
+00000d60: 6f61 6d2e 666f 616d 5f69 6e70 7574 5f66  oam.foam_input_f
+00000d70: 696c 6573 7205 0000 0072 0f00 0000 7210  ilesr....r....r.
+00000d80: 0000 0072 0a00 0000 720a 0000 0072 0a00  ...r....r....r..
+00000d90: 0000 720b 0000 00da 083c 6d6f 6475 6c65  ..r......<module
+00000da0: 3e01 0000 0073 1000 0000 0400 0802 0c01  >....s..........
+00000db0: 1001 0c02 0c02 0803 1204                 ..........
```

### Comparing `fluidsimfoam-0.0.5/src/fluidsimfoam/output/__pycache__/log.cpython-39.pyc` & `fluidsimfoam-0.0.6/src/fluidsimfoam/output/__pycache__/log.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun  1 13:07:51 2023 UTC, .py size: 6580 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,342 +1,341 @@
-00000000: 610d 0d0a 0000 0000 2798 7864 b419 0000  a.......'.xd....
+00000000: 6f0d 0d0a 0000 0000 5ab4 6f64 b419 0000  o.......Z.od....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 5200 0000 6400  .....@...sR...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a04 0100 6401 6402 6c05 5a06 6401  m.Z...d.d.l.Z.d.
 00000050: 6403 6c07 6d08 5a08 0100 640b 6405 6406  d.l.m.Z...d.d.d.
 00000060: 8401 5a09 6407 6408 8400 5a0a 4700 6409  ..Z.d.d...Z.G.d.
 00000070: 640a 8400 640a 6508 8303 5a0b 6402 5300  d...d.e...Z.d.S.
 00000080: 290c 7a27 436c 6173 7320 666f 7220 7468  ).z'Class for th
 00000090: 6520 6060 7369 6d2e 6f75 7470 7574 2e6c  e ``sim.output.l
 000000a0: 6f67 6060 206f 626a 6563 74e9 0000 0000  og`` object.....
 000000b0: 4e29 01da 1252 656d 6169 6e69 6e67 436c  N)...RemainingCl
 000000c0: 6f63 6b54 696d 65e9 e803 0000 6302 0000  ockTime.....c...
 000000d0: 0000 0000 0000 0000 0004 0000 0008 0000  ................
 000000e0: 0043 0000 0073 5400 0000 7c00 a000 a100  .C...sT...|.....
-000000f0: 6a01 7d02 7402 7c00 6401 8302 8f2c 7d03  j.}.t.|.d....,}.
+000000f0: 6a01 7d02 7402 7c00 6401 8302 8f16 7d03  j.}.t.|.d.....}.
 00000100: 7c03 a003 7404 6402 7c02 7c01 1800 8302  |...t.d.|.|.....
 00000110: a101 0100 7c03 a005 a100 5700 0200 6400  ....|.....W...d.
-00000120: 0400 0400 8303 0100 5300 3100 7346 3000  ........S.1.sF0.
+00000120: 0400 0400 8303 0100 5300 3100 7323 7701  ........S.1.s#w.
 00000130: 0100 0100 0100 5900 0100 6400 5300 2903  ......Y...d.S.).
 00000140: 4eda 0172 7201 0000 0029 06da 0473 7461  N..rr....)...sta
 00000150: 74da 0773 745f 7369 7a65 da04 6f70 656e  t..st_size..open
 00000160: da04 7365 656b da03 6d61 78da 0472 6561  ..seek..max..rea
 00000170: 6429 04da 0970 6174 685f 6669 6c65 da06  d)...path_file..
 00000180: 6e62 7974 6573 5a08 6c6f 675f 7369 7a65  nbytesZ.log_size
-00000190: da04 6669 6c65 a900 720e 0000 00fa 452f  ..file..r.....E/
-000001a0: 686f 6d65 2f75 7365 7273 2f61 7567 6965  home/users/augie
-000001b0: 7233 7069 2f44 6576 2f66 6c75 6964 7369  r3pi/Dev/fluidsi
-000001c0: 6d66 6f61 6d2f 7372 632f 666c 7569 6473  mfoam/src/fluids
-000001d0: 696d 666f 616d 2f6f 7574 7075 742f 6c6f  imfoam/output/lo
-000001e0: 672e 7079 da0c 6765 745f 6c6f 675f 7461  g.py..get_log_ta
-000001f0: 696c 0b00 0000 7308 0000 0000 010a 010c  il....s.........
-00000200: 0114 0172 1000 0000 6301 0000 0000 0000  ...r....c.......
-00000210: 0000 0000 0003 0000 0005 0000 0043 0000  .............C..
-00000220: 0073 4c00 0000 7400 7c00 6401 8302 7d01  .sL...t.|.d...}.
-00000230: 7c01 a001 6402 a101 7d02 7c02 6403 6b02  |...d...}.|.d.k.
-00000240: 7228 7402 6404 8301 0100 6400 5300 7c01  r(t.d.....d.S.|.
-00000250: 7c02 6405 1700 6400 8502 1900 7d01 7403  |.d...d.....}.t.
-00000260: 7c01 a004 6400 6406 a102 6407 1900 8301  |...d.d...d.....
-00000270: 5300 2908 4e72 0300 0000 7a08 0a54 696d  S.).Nr....z..Tim
-00000280: 6520 3d20 e9ff ffff ff7a 1f27 5469 6d65  e = .....z.'Time
-00000290: 203d 2027 206e 6f74 2066 6f75 6e64 2069   = ' not found i
-000002a0: 6e20 6c6f 6720 6669 6c65 e908 0000 00e9  n log file......
-000002b0: 0100 0000 7201 0000 0029 0572 1000 0000  ....r....).r....
-000002c0: da05 7266 696e 64da 0570 7269 6e74 da05  ..rfind..print..
-000002d0: 666c 6f61 74da 0573 706c 6974 2903 720b  float..split).r.
-000002e0: 0000 00da 0474 6578 74da 0569 6e64 6578  .....text..index
-000002f0: 720e 0000 0072 0e00 0000 720f 0000 00da  r....r....r.....
-00000300: 0e72 6561 645f 7469 6d65 5f6c 6173 7412  .read_time_last.
-00000310: 0000 0073 0e00 0000 0001 0a01 0a01 0801  ...s............
-00000320: 0801 0401 1001 721a 0000 0063 0000 0000  ......r....c....
-00000330: 0000 0000 0000 0000 0000 0000 0300 0000  ................
-00000340: 4000 0000 7378 0000 0065 005a 0164 005a  @...sx...e.Z.d.Z
-00000350: 0264 015a 0364 0264 0384 005a 0464 0464  .d.Z.d.d...Z.d.d
-00000360: 0584 005a 0565 0664 0664 0784 0083 015a  ...Z.e.d.d.....Z
-00000370: 0765 076a 0864 0864 0784 0083 015a 0765  .e.j.d.d.....Z.e
-00000380: 0664 0964 0a84 0083 015a 0964 1864 0c64  .d.d.....Z.d.d.d
-00000390: 0d84 015a 0a65 0664 0e64 0f84 0083 015a  ...Z.e.d.d.....Z
-000003a0: 0b64 1064 1184 005a 0c64 1964 1364 1484  .d.d...Z.d.d.d..
-000003b0: 015a 0d64 1a64 1664 1784 015a 0e64 1253  .Z.d.d.d...Z.d.S
-000003c0: 0029 1bda 034c 6f67 da03 6c6f 6763 0200  .)...Log..logc..
-000003d0: 0000 0000 0000 0000 0000 0200 0000 0200  ................
-000003e0: 0000 4300 0000 7310 0000 007c 017c 005f  ..C...s....|.|._
-000003f0: 0064 007c 005f 0164 0053 00a9 014e 2902  .d.|._.d.S...N).
-00000400: da06 6f75 7470 7574 da0a 5f70 6174 685f  ..output.._path_
-00000410: 6669 6c65 2902 da04 7365 6c66 721e 0000  file)...selfr...
-00000420: 0072 0e00 0000 720e 0000 0072 0f00 0000  .r....r....r....
-00000430: da08 5f5f 696e 6974 5f5f 1f00 0000 7304  ..__init__....s.
-00000440: 0000 0000 0106 017a 0c4c 6f67 2e5f 5f69  .......z.Log.__i
-00000450: 6e69 745f 5f63 0100 0000 0000 0000 0000  nit__c..........
-00000460: 0000 1100 0000 0900 0000 4300 0000 73a2  ..........C...s.
-00000470: 0100 007c 006a 007d 0174 01a0 0264 017c  ...|.j.}.t...d.|
-00000480: 01a1 027d 027c 0264 0275 0172 2c74 037c  ...}.|.d.u.r,t.|
-00000490: 02a0 04a1 0064 0319 0083 017d 036e 0464  .....d.....}.n.d
-000004a0: 047d 0374 01a0 0264 057c 01a1 027d 027c  .}.t...d.|...}.|
-000004b0: 0264 0275 0172 5674 037c 02a0 04a1 0064  .d.u.rVt.|.....d
-000004c0: 0319 0083 017d 046e 0474 0582 0174 01a0  .....}.n.t...t..
-000004d0: 0664 067c 01a1 027d 0574 01a0 0664 077c  .d.|...}.t...d.|
-000004e0: 01a1 027d 067c 0564 0274 077c 0683 0185  ...}.|.d.t.|....
-000004f0: 0219 007d 0574 08a0 0964 0864 0984 007c  ...}.t...d.d...|
-00000500: 0544 0083 01a1 017d 0574 08a0 0964 0a64  .D.....}.t...d.d
-00000510: 0984 007c 0644 0083 01a1 017d 067c 0664  ...|.D.....}.|.d
-00000520: 0b19 0074 077c 0683 011b 007d 0774 08a0  ...t.|.....}.t..
-00000530: 0a7c 066a 0ba1 017d 0874 086a 0c7c 0664  .|.j...}.t.j.|.d
-00000540: 0c64 0d8d 025c 027d 067d 097c 057c 0919  .d...\.}.}.|.|..
-00000550: 007d 057c 087c 0919 007d 0864 0e7d 0a74  .}.|.|...}.d.}.t
-00000560: 0d74 0e64 0f7c 0a14 007c 06a0 0fa1 007c  .t.d.|...|.....|
-00000570: 06a0 0ea1 0018 0064 101b 0083 027c 071b  .......d.....|..
-00000580: 0083 017d 0b7c 0b64 116b 0490 0172 467c  ...}.|.d.k...rF|
-00000590: 0664 0264 027c 0b85 0319 007d 067c 0564  .d.d.|.....}.|.d
-000005a0: 0264 027c 0b85 0319 007d 057c 0864 0264  .d.|.....}.|.d.d
-000005b0: 027c 0b85 0319 007d 0874 08a0 107c 05a1  .|.....}.t...|..
-000005c0: 017d 0c7c 0564 0264 0b85 0219 007d 057c  .}.|.d.d.....}.|
-000005d0: 047c 0518 007d 0d74 08a0 107c 06a1 017d  .|...}.t...|...}
-000005e0: 0e7c 0d7c 0c1b 007c 0e14 007d 0f7c 057c  .|.|...|...}.|.|
-000005f0: 0f7c 0e74 08a0 107c 08a1 011b 007c 037c  .|.t...|.....|.|
-00000600: 0664 0b19 007c 0d7c 0c7c 0e64 129c 087d  .d...|.|.|.d...}
-00000610: 107c 1053 0029 137a b84c 6f61 6420 7265  .|.S.).z.Load re
-00000620: 6d61 696e 696e 6720 7469 6d65 2064 6174  maining time dat
-00000630: 612e 0a0a 2020 2020 2020 2020 2d20 6571  a...        - eq
-00000640: 7561 7469 6f6e 5f74 696d 6573 0a20 2020  uation_times.   
-00000650: 2020 2020 202d 2072 656d 6169 6e69 6e67       - remaining
-00000660: 5f63 6c6f 636b 5f74 696d 6573 0a20 2020  _clock_times.   
-00000670: 2020 2020 202d 2063 6c6f 636b 5f74 696d       - clock_tim
-00000680: 6573 5f70 6572 5f74 696d 6573 7465 700a  es_per_timestep.
-00000690: 2020 2020 2020 2020 2d20 6571 7561 7469          - equati
-000006a0: 6f6e 5f74 696d 655f 7374 6172 740a 2020  on_time_start.  
-000006b0: 2020 2020 2020 2d20 6675 6c6c 5f63 6c6f        - full_clo
-000006c0: 636b 5f74 696d 650a 0a20 2020 2020 2020  ck_time..       
-000006d0: 207a 1873 7461 7274 5f74 696d 6520 3d20   z.start_time = 
-000006e0: 285b 5c64 5c2e 5d2b 295c 6e4e 7201 0000  ([\d\.]+)\nNr...
-000006f0: 00e7 0000 0000 0000 0000 7a16 656e 645f  ..........z.end_
-00000700: 7469 6d65 203d 2028 5b5c 645c 2e5d 2b29  time = ([\d\.]+)
-00000710: 5c6e 7a1a 5c6e 5469 6d65 203d 2028 5b5c  \nz.\nTime = ([\
-00000720: 645c 2e5d 2b65 3f5b 2d5c 645d 2a29 7a1b  d\.]+e?[-\d]*)z.
-00000730: 5c6e 4578 6563 7574 696f 6e54 696d 6520  \nExecutionTime 
-00000740: 3d20 285b 5c64 5c2e 5d2b 2963 0100 0000  = ([\d\.]+)c....
-00000750: 0000 0000 0000 0000 0200 0000 0400 0000  ................
-00000760: 5300 0000 7314 0000 0067 007c 005d 0c7d  S...s....g.|.].}
-00000770: 0174 007c 0183 0191 0271 0453 0072 0e00  .t.|.....q.S.r..
-00000780: 0000 a901 7216 0000 00a9 02da 022e 30da  ....r.........0.
-00000790: 0477 6f72 6472 0e00 0000 720e 0000 0072  .wordr....r....r
-000007a0: 0f00 0000 da0a 3c6c 6973 7463 6f6d 703e  ......<listcomp>
-000007b0: 3f00 0000 f300 0000 007a 234c 6f67 2e5f  ?........z#Log._
-000007c0: 6c6f 6164 5f74 696d 6573 2e3c 6c6f 6361  load_times.<loca
-000007d0: 6c73 3e2e 3c6c 6973 7463 6f6d 703e 6301  ls>.<listcomp>c.
-000007e0: 0000 0000 0000 0000 0000 0002 0000 0004  ................
-000007f0: 0000 0053 0000 0073 1400 0000 6700 7c00  ...S...s....g.|.
-00000800: 5d0c 7d01 7400 7c01 8301 9102 7104 5300  ].}.t.|.....q.S.
-00000810: 720e 0000 0072 2300 0000 7224 0000 0072  r....r#...r$...r
-00000820: 0e00 0000 720e 0000 0072 0f00 0000 7227  ....r....r....r'
-00000830: 0000 0040 0000 0072 2800 0000 7211 0000  ...@...r(...r...
-00000840: 0054 2901 da0c 7265 7475 726e 5f69 6e64  .T)...return_ind
-00000850: 6578 677b 14ae 47e1 7a84 3f72 1200 0000  exg{..G.z.?r....
-00000860: e902 0000 0072 1300 0000 2908 5a0e 6571  .....r....).Z.eq
-00000870: 7561 7469 6f6e 5f74 696d 6573 da15 7265  uation_times..re
-00000880: 6d61 696e 696e 675f 636c 6f63 6b5f 7469  maining_clock_ti
-00000890: 6d65 735a 1863 6c6f 636b 5f74 696d 6573  mesZ.clock_times
-000008a0: 5f70 6572 5f74 696d 6573 7465 70da 1365  _per_timestep..e
-000008b0: 7175 6174 696f 6e5f 7469 6d65 5f73 7461  quation_time_sta
-000008c0: 7274 5a0f 6675 6c6c 5f63 6c6f 636b 5f74  rtZ.full_clock_t
-000008d0: 696d 65da 1272 656d 6169 6e69 6e67 5f65  ime..remaining_e
-000008e0: 715f 7469 6d65 73da 0e64 656c 7461 5f65  q_times..delta_e
-000008f0: 715f 7469 6d65 73da 1164 656c 7461 5f63  q_times..delta_c
-00000900: 6c6f 636b 5f74 696d 6573 2911 7218 0000  lock_times).r...
-00000910: 00da 0272 65da 0673 6561 7263 6872 1600  ...re..searchr..
-00000920: 0000 da06 6772 6f75 7073 da0c 5275 6e74  ....groups..Runt
-00000930: 696d 6545 7272 6f72 da07 6669 6e64 616c  imeError..findal
-00000940: 6cda 036c 656e da02 6e70 da05 6172 7261  l..len..np..arra
-00000950: 79da 0661 7261 6e67 65da 0473 697a 65da  y..arange..size.
-00000960: 0675 6e69 7175 65da 0572 6f75 6e64 da03  .unique..round..
-00000970: 6d69 6e72 0900 0000 da04 6469 6666 2911  minr......diff).
-00000980: 7220 0000 0072 1800 0000 da05 6d61 7463  r ...r......matc
-00000990: 6872 2c00 0000 5a0b 6571 5f74 696d 655f  hr,...Z.eq_time_
-000009a0: 656e 645a 0865 715f 7469 6d65 735a 0b63  endZ.eq_timesZ.c
-000009b0: 6c6f 636b 5f74 696d 6573 5a23 6573 7469  lock_timesZ#esti
-000009c0: 6d61 7469 6f6e 5f63 6c6f 636b 5f74 696d  mation_clock_tim
-000009d0: 655f 7065 725f 7469 6d65 5f73 7465 705a  e_per_time_stepZ
-000009e0: 1169 6e64 6963 6573 5f74 696d 655f 7374  .indices_time_st
-000009f0: 6570 5a0e 696e 6469 6365 735f 756e 6971  epZ.indices_uniq
-00000a00: 7565 5a0f 7072 6563 6973 696f 6e5f 636c  ueZ.precision_cl
-00000a10: 6f63 6bda 0473 7465 7072 2e00 0000 722d  ock..stepr....r-
-00000a20: 0000 0072 2f00 0000 722b 0000 00da 0464  ...r/...r+.....d
-00000a30: 6174 6172 0e00 0000 720e 0000 0072 0f00  atar....r....r..
-00000a40: 0000 da0b 5f6c 6f61 645f 7469 6d65 7323  ...._load_times#
-00000a50: 0000 0073 5e00 0000 000a 0602 0c01 0801  ...s^...........
-00000a60: 1202 0402 0c01 0801 1202 0402 0c01 0c01  ................
-00000a70: 1002 1401 1402 1002 0c03 1201 0801 0803  ................
-00000a80: 0401 0201 1c01 02ff 02ff 0404 0a01 0e01  ................
-00000a90: 0e01 0e02 0a02 0c01 0802 0a03 0aff 0205  ................
-00000aa0: 0201 0201 0201 08ff 0202 0201 0601 0201  ................
-00000ab0: 0201 02f7 060c 7a0f 4c6f 672e 5f6c 6f61  ......z.Log._loa
-00000ac0: 645f 7469 6d65 7363 0100 0000 0000 0000  d_timesc........
-00000ad0: 0000 0000 0400 0000 0400 0000 4300 0000  ............C...
-00000ae0: 734a 0000 007c 006a 007d 017c 0172 407c  sJ...|.j.}.|.r@|
-00000af0: 006a 0173 407c 016a 027d 0274 037c 02a0  .j.s@|.j.}.t.|..
-00000b00: 0464 01a1 0183 017d 037c 0372 347c 0364  .d.....}.|.r4|.d
-00000b10: 0219 007c 005f 016e 0c74 0564 0383 0101  ...|._.n.t.d....
-00000b20: 0064 0053 007c 006a 01a0 06a1 0053 0029  .d.S.|.j.....S.)
-00000b30: 044e 7a08 6c6f 672a 2e74 7874 7211 0000  .Nz.log*.txtr...
-00000b40: 007a 114e 6f20 6c6f 6720 6669 6c65 2066  .z.No log file f
-00000b50: 6f75 6e64 2907 721e 0000 0072 1f00 0000  ound).r....r....
-00000b60: da08 7061 7468 5f72 756e da06 736f 7274  ..path_run..sort
-00000b70: 6564 da04 676c 6f62 7215 0000 00da 0772  ed..globr......r
-00000b80: 6573 6f6c 7665 2904 7220 0000 0072 1e00  esolve).r ...r..
-00000b90: 0000 7242 0000 00da 086c 6f67 6669 6c65  ..rB.....logfile
-00000ba0: 7372 0e00 0000 720e 0000 0072 0f00 0000  sr....r....r....
-00000bb0: 720b 0000 006f 0000 0073 1200 0000 0002  r....o...s......
-00000bc0: 0601 0a01 0601 0e01 0401 0c02 0801 0402  ................
-00000bd0: 7a0d 4c6f 672e 7061 7468 5f66 696c 6563  z.Log.path_filec
-00000be0: 0200 0000 0000 0000 0000 0000 0200 0000  ................
-00000bf0: 0200 0000 4300 0000 730a 0000 007c 017c  ....C...s....|.|
-00000c00: 005f 0064 0053 0072 1d00 0000 2901 721f  ._.d.S.r....).r.
-00000c10: 0000 0029 0272 2000 0000 5a0d 7061 7468  ...).r ...Z.path
-00000c20: 5f6c 6f67 5f66 696c 6572 0e00 0000 720e  _log_filer....r.
-00000c30: 0000 0072 0f00 0000 720b 0000 007d 0000  ...r....r....}..
-00000c40: 0073 0200 0000 0002 6301 0000 0000 0000  .s......c.......
-00000c50: 0000 0000 0002 0000 0008 0000 0043 0000  .............C..
-00000c60: 0073 4400 0000 7c00 6a00 6400 7500 720e  .sD...|.j.d.u.r.
-00000c70: 6400 5300 7401 7c00 6a00 8301 8f18 7d01  d.S.t.|.j.....}.
-00000c80: 7c01 a002 a100 5700 0200 6400 0400 0400  |.....W...d.....
-00000c90: 8303 0100 5300 3100 7336 3000 0100 0100  ....S.1.s60.....
-00000ca0: 0100 5900 0100 6400 5300 721d 0000 0029  ..Y...d.S.r....)
-00000cb0: 0372 0b00 0000 7207 0000 0072 0a00 0000  .r....r....r....
-00000cc0: 2902 7220 0000 0072 0d00 0000 720e 0000  ).r ...r....r...
-00000cd0: 0072 0e00 0000 720f 0000 0072 1800 0000  .r....r....r....
-00000ce0: 8100 0000 7308 0000 0000 020a 0104 020c  ....s...........
-00000cf0: 017a 084c 6f67 2e74 6578 7472 0300 0000  .z.Log.textr....
-00000d00: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
-00000d10: 0003 0000 0043 0000 0073 2800 0000 7c00  .....C...s(...|.
-00000d20: 6a00 6400 7500 721c 7401 6401 7c00 6a02  j.d.u.r.t.d.|.j.
-00000d30: 6a03 9b00 9d02 8301 8201 7404 7c00 6a00  j.........t.|.j.
-00000d40: 7c01 8302 5300 2902 4e7a 154e 6f20 6c6f  |...S.).Nz.No lo
-00000d50: 6720 6669 6c65 2066 6f75 6e64 2069 6e20  g file found in 
-00000d60: 2905 720b 0000 00da 0749 4f45 7272 6f72  ).r......IOError
-00000d70: 721e 0000 0072 4200 0000 7210 0000 0029  r....rB...r....)
-00000d80: 0272 2000 0000 720c 0000 0072 0e00 0000  .r ...r....r....
-00000d90: 720e 0000 0072 0f00 0000 7210 0000 0089  r....r....r.....
-00000da0: 0000 0073 0600 0000 0001 0a01 1201 7a10  ...s..........z.
-00000db0: 4c6f 672e 6765 745f 6c6f 675f 7461 696c  Log.get_log_tail
-00000dc0: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-00000dd0: 0002 0000 0043 0000 0073 1800 0000 7c00  .....C...s....|.
-00000de0: 6a00 6400 7500 720e 6400 5300 7401 7c00  j.d.u.r.d.S.t.|.
-00000df0: 6a00 8301 5300 721d 0000 0029 0272 0b00  j...S.r....).r..
-00000e00: 0000 721a 0000 0029 0172 2000 0000 720e  ..r....).r ...r.
-00000e10: 0000 0072 0e00 0000 720f 0000 00da 0974  ...r....r......t
-00000e20: 696d 655f 6c61 7374 8e00 0000 7306 0000  ime_last....s...
-00000e30: 0000 020a 0104 017a 0d4c 6f67 2e74 696d  .......z.Log.tim
-00000e40: 655f 6c61 7374 6302 0000 0000 0000 0000  e_lastc.........
-00000e50: 0000 0003 0000 0003 0000 0043 0000 0073  ...........C...s
-00000e60: 5000 0000 7c01 6400 7501 7226 7c01 7c00  P...|.d.u.r&|.|.
-00000e70: 6a00 6a01 7601 7226 7402 6401 7c00 6a00  j.j.v.r&t.d.|.j.
-00000e80: 6a01 9b00 9d02 8301 8201 7c01 6400 7500  j.........|.d.u.
-00000e90: 724c 6402 4400 5d18 7d02 7c02 7c00 6a00  rLd.D.].}.|.|.j.
-00000ea0: 6a01 7600 7232 7c02 7d01 0100 714c 7132  j.v.r2|.}...qLq2
-00000eb0: 7c01 5300 2903 4e7a 1b76 6172 6961 626c  |.S.).Nz.variabl
-00000ec0: 655f 6e61 6d65 2068 6173 2074 6f20 6265  e_name has to be
-00000ed0: 2069 6e20 2902 da01 705a 0670 5f72 6267   in )...pZ.p_rbg
-00000ee0: 6829 0372 1e00 0000 da0e 6e61 6d65 5f76  h).r......name_v
-00000ef0: 6172 6961 626c 6573 da0a 5661 6c75 6545  ariables..ValueE
-00000f00: 7272 6f72 2903 7220 0000 00da 0d76 6172  rror).r .....var
-00000f10: 6961 626c 655f 6e61 6d65 da03 6b65 7972  iable_name..keyr
-00000f20: 0e00 0000 720e 0000 0072 0f00 0000 da15  ....r....r......
-00000f30: 5f63 686f 6f73 655f 7661 7269 6162 6c65  _choose_variable
-00000f40: 5f6e 616d 6594 0000 0073 1a00 0000 0002  _name....s......
-00000f50: 06ff 0202 0afe 0204 0201 0cff 0404 0801  ................
-00000f60: 0801 0c01 0401 0601 7a19 4c6f 672e 5f63  ........z.Log._c
-00000f70: 686f 6f73 655f 7661 7269 6162 6c65 5f6e  hoose_variable_n
-00000f80: 616d 654e 6302 0000 0000 0000 0000 0000  ameNc...........
-00000f90: 0008 0000 0006 0000 0043 0000 0073 8200  .........C...s..
-00000fa0: 0000 7c00 6a00 6400 7500 720e 6400 5300  ..|.j.d.u.r.d.S.
-00000fb0: 7c00 a001 6401 a101 7d02 7c00 a002 7c01  |...d...}.|...|.
-00000fc0: a101 7d01 7403 7404 a005 6402 7c01 9b00  ..}.t.t...d.|...
-00000fd0: 6403 9d03 7c02 a102 8301 7d03 7c03 7352  d...|.....}.|.sR
-00000fe0: 7406 6404 7c01 9b00 6405 7c02 9b00 9d04  t.d.|...d.|.....
-00000ff0: 8301 8201 7c03 6406 1900 7d04 7c04 a007  ....|.d...}.|...
-00001000: a100 7d05 7408 7c05 6407 1900 8301 7d06  ..}.t.|.d.....}.
-00001010: 7408 7c05 6408 1900 8301 7d07 7c06 7c07  t.|.d.....}.|.|.
-00001020: 6602 5300 2909 4e69 8813 0000 fa37 5c6e  f.S.).Ni.....7\n
-00001030: 5469 6d65 203d 2028 3f50 3c74 696d 653e  Time = (?P<time>
-00001040: 5b5c 645c 2e5d 2b65 3f2d 3f5b 5c64 5d2a  [\d\.]+e?-?[\d]*
-00001050: 295b 5c73 5c53 5d2b 3f53 6f6c 7669 6e67  )[\s\S]+?Solving
-00001060: 2066 6f72 20fa 322c 2049 6e69 7469 616c   for .2, Initial
-00001070: 2072 6573 6964 7561 6c20 3d20 283f 503c   residual = (?P<
-00001080: 696e 6974 6961 6c3e 5b5c 645c 2e5d 2b65  initial>[\d\.]+e
-00001090: 3f2d 3f5b 5c64 5d2a 297a 134e 6f20 6d61  ?-?[\d]*)z.No ma
-000010a0: 7463 6820 666f 756e 6420 666f 7220 7a08  tch found for z.
-000010b0: 2c20 7465 7874 3d0a 7211 0000 00da 0474  , text=.r......t
-000010c0: 696d 65da 0769 6e69 7469 616c 2909 720b  ime..initial).r.
-000010d0: 0000 0072 1000 0000 724e 0000 00da 046c  ...r....rN.....l
-000010e0: 6973 7472 3000 0000 da08 6669 6e64 6974  istr0.....findit
-000010f0: 6572 724b 0000 00da 0967 726f 7570 6469  errK.....groupdi
-00001100: 6374 7216 0000 0029 0872 2000 0000 724c  ctr....).r ...rL
-00001110: 0000 0072 1800 0000 da07 6d61 7463 6865  ...r......matche
-00001120: 7372 3e00 0000 7240 0000 0072 5100 0000  sr>...r@...rQ...
-00001130: 5a08 7265 7369 6475 616c 720e 0000 0072  Z.residualr....r
-00001140: 0e00 0000 720f 0000 00da 1167 6574 5f6c  ....r......get_l
-00001150: 6173 745f 7265 7369 6475 616c a400 0000  ast_residual....
-00001160: 7326 0000 0000 010a 0104 010a 020a 0102  s&..............
-00001170: 0104 0102 0102 ff06 0302 fc02 ff04 0904  ................
-00001180: 0114 0208 0108 010c 010c 017a 154c 6f67  ...........z.Log
-00001190: 2e67 6574 5f6c 6173 745f 7265 7369 6475  .get_last_residu
-000011a0: 616c 7222 0000 0063 0300 0000 0000 0000  alr"...c........
-000011b0: 0000 0000 0b00 0000 0600 0000 4300 0000  ............C...
-000011c0: 73c0 0000 007c 00a0 007c 01a1 017d 0174  s....|...|...}.t
-000011d0: 0174 02a0 0364 017c 019b 0064 029d 037c  .t...d.|...d...|
-000011e0: 006a 04a1 0283 017d 0374 05a0 0674 077c  .j.....}.t...t.|
-000011f0: 0383 01a1 017d 0474 05a0 087c 04a1 017d  .....}.t...|...}
-00001200: 0574 097c 0383 0144 005d 285c 027d 067d  .t.|...D.](\.}.}
-00001210: 077c 07a0 0aa1 007d 087c 0864 0319 007c  .|.....}.|.d...|
-00001220: 047c 063c 007c 0864 0419 007c 057c 063c  .|.<.|.d...|.|.<
-00001230: 0071 4474 0ba0 0ca1 005c 027d 097d 0a7c  .qDt.....\.}.}.|
-00001240: 057c 047c 026b 0419 007d 057c 047c 047c  .|.|.k...}.|.|.|
-00001250: 026b 0419 007d 047c 0aa0 0d7c 047c 05a1  .k...}.|...|.|..
-00001260: 0201 007c 0aa0 0e64 05a1 0101 007c 09a0  ...|...d.....|..
-00001270: 0f64 067c 019b 009d 02a1 0101 007c 047c  .d.|.........|.|
-00001280: 0566 0253 0029 074e 724f 0000 0072 5000  .f.S.).NrO...rP.
-00001290: 0000 7251 0000 0072 5200 0000 7a0d 6571  ..rQ...rR...z.eq
-000012a0: 7561 7469 6f6e 2074 696d 657a 1249 6e69  uation timez.Ini
-000012b0: 7469 616c 2072 6573 6964 7561 6c73 2029  tial residuals )
-000012c0: 1072 4e00 0000 7253 0000 0072 3000 0000  .rN...rS...r0...
-000012d0: 7254 0000 0072 1800 0000 7236 0000 00da  rT...r....r6....
-000012e0: 0565 6d70 7479 7235 0000 00da 0a65 6d70  .emptyr5.....emp
-000012f0: 7479 5f6c 696b 65da 0965 6e75 6d65 7261  ty_like..enumera
-00001300: 7465 7255 0000 00da 0370 6c74 da08 7375  terU.....plt..su
-00001310: 6270 6c6f 7473 da04 706c 6f74 5a0a 7365  bplots..plotZ.se
-00001320: 745f 786c 6162 656c 5a08 7375 7074 6974  t_xlabelZ.suptit
-00001330: 6c65 290b 7220 0000 0072 4c00 0000 da04  le).r ...rL.....
-00001340: 746d 696e 7256 0000 00da 0574 696d 6573  tminrV.....times
-00001350: 5a09 7265 7369 6475 616c 7372 1900 0000  Z.residualsr....
-00001360: 723e 0000 0072 4000 0000 da03 6669 67da  r>...r@.....fig.
-00001370: 0261 7872 0e00 0000 720e 0000 0072 0f00  .axr....r....r..
-00001380: 0000 da0e 706c 6f74 5f72 6573 6964 7561  ....plot_residua
-00001390: 6c73 bc00 0000 732c 0000 0000 010a 0102  ls....s,........
-000013a0: 0104 0102 0102 ff06 0304 fc02 ff04 090e  ................
-000013b0: 010a 0210 0108 020c 010e 020c 020c 010c  ................
-000013c0: 010c 010a 0110 017a 124c 6f67 2e70 6c6f  .......z.Log.plo
-000013d0: 745f 7265 7369 6475 616c 7329 0172 0300  t_residuals).r..
-000013e0: 0000 2901 4e29 024e 7222 0000 0029 0fda  ..).N).Nr"...)..
-000013f0: 085f 5f6e 616d 655f 5fda 0a5f 5f6d 6f64  .__name__..__mod
-00001400: 756c 655f 5fda 0c5f 5f71 7561 6c6e 616d  ule__..__qualnam
-00001410: 655f 5fda 045f 7461 6772 2100 0000 7241  e__.._tagr!...rA
-00001420: 0000 00da 0870 726f 7065 7274 7972 0b00  .....propertyr..
-00001430: 0000 da06 7365 7474 6572 7218 0000 0072  ....setterr....r
-00001440: 1000 0000 7248 0000 0072 4e00 0000 7257  ....rH...rN...rW
-00001450: 0000 0072 6200 0000 720e 0000 0072 0e00  ...rb...r....r..
-00001460: 0000 720e 0000 0072 0f00 0000 721b 0000  ..r....r....r...
-00001470: 001c 0000 0073 1e00 0000 0801 0402 0804  .....s..........
-00001480: 084c 0201 0a0d 0401 0a03 0201 0a07 0a05  .L..............
-00001490: 0201 0a05 0810 0a18 721b 0000 0029 0172  ........r....).r
-000014a0: 0300 0000 290c da07 5f5f 646f 635f 5f72  ....)...__doc__r
-000014b0: 3000 0000 da11 6d61 7470 6c6f 746c 6962  0.....matplotlib
-000014c0: 2e70 7970 6c6f 74da 0670 7970 6c6f 7472  .pyplot..pyplotr
-000014d0: 5b00 0000 da05 6e75 6d70 7972 3600 0000  [.....numpyr6...
-000014e0: 5a29 666c 7569 6473 696d 5f63 6f72 652e  Z)fluidsim_core.
-000014f0: 6f75 7470 7574 2e72 656d 6169 6e69 6e67  output.remaining
-00001500: 5f63 6c6f 636b 5f74 696d 6572 0200 0000  _clock_timer....
-00001510: 7210 0000 0072 1a00 0000 721b 0000 0072  r....r....r....r
-00001520: 0e00 0000 720e 0000 0072 0e00 0000 720f  ....r....r....r.
-00001530: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
-00001540: 0073 0e00 0000 0402 0802 0c01 0802 0c03  .s..............
-00001550: 0a07 080a                                ....
+00000190: da04 6669 6c65 a900 720e 0000 00fa 3c2f  ..file..r.....</
+000001a0: 686f 6d65 2f70 6965 7272 652f 4465 762f  home/pierre/Dev/
+000001b0: 666c 7569 6473 696d 666f 616d 2f73 7263  fluidsimfoam/src
+000001c0: 2f66 6c75 6964 7369 6d66 6f61 6d2f 6f75  /fluidsimfoam/ou
+000001d0: 7470 7574 2f6c 6f67 2e70 79da 0c67 6574  tput/log.py..get
+000001e0: 5f6c 6f67 5f74 6169 6c0b 0000 0073 0a00  _log_tail....s..
+000001f0: 0000 0a01 0c01 1401 0601 24fe 7210 0000  ..........$.r...
+00000200: 0063 0100 0000 0000 0000 0000 0000 0300  .c..............
+00000210: 0000 0500 0000 4300 0000 734c 0000 0074  ......C...sL...t
+00000220: 007c 0064 0183 027d 017c 01a0 0164 02a1  .|.d...}.|...d..
+00000230: 017d 027c 0264 036b 0272 1474 0264 0483  .}.|.d.k.r.t.d..
+00000240: 0101 0064 0053 007c 017c 0264 0517 0064  ...d.S.|.|.d...d
+00000250: 0085 0219 007d 0174 037c 01a0 0464 0064  .....}.t.|...d.d
+00000260: 06a1 0264 0719 0083 0153 0029 084e 7203  ...d.....S.).Nr.
+00000270: 0000 007a 080a 5469 6d65 203d 20e9 ffff  ...z..Time = ...
+00000280: ffff 7a1f 2754 696d 6520 3d20 2720 6e6f  ..z.'Time = ' no
+00000290: 7420 666f 756e 6420 696e 206c 6f67 2066  t found in log f
+000002a0: 696c 65e9 0800 0000 e901 0000 0072 0100  ile..........r..
+000002b0: 0000 2905 7210 0000 00da 0572 6669 6e64  ..).r......rfind
+000002c0: da05 7072 696e 74da 0566 6c6f 6174 da05  ..print..float..
+000002d0: 7370 6c69 7429 0372 0b00 0000 da04 7465  split).r......te
+000002e0: 7874 da05 696e 6465 7872 0e00 0000 720e  xt..indexr....r.
+000002f0: 0000 0072 0f00 0000 da0e 7265 6164 5f74  ...r......read_t
+00000300: 696d 655f 6c61 7374 1200 0000 730e 0000  ime_last....s...
+00000310: 000a 010a 0108 0108 0104 0110 0114 0172  ...............r
+00000320: 1a00 0000 6300 0000 0000 0000 0000 0000  ....c...........
+00000330: 0000 0000 0003 0000 0040 0000 0073 7800  .........@...sx.
+00000340: 0000 6500 5a01 6400 5a02 6401 5a03 6402  ..e.Z.d.Z.d.Z.d.
+00000350: 6403 8400 5a04 6404 6405 8400 5a05 6506  d...Z.d.d...Z.e.
+00000360: 6406 6407 8400 8301 5a07 6507 6a08 6408  d.d.....Z.e.j.d.
+00000370: 6407 8400 8301 5a07 6506 6409 640a 8400  d.....Z.e.d.d...
+00000380: 8301 5a09 6418 640c 640d 8401 5a0a 6506  ..Z.d.d.d...Z.e.
+00000390: 640e 640f 8400 8301 5a0b 6410 6411 8400  d.d.....Z.d.d...
+000003a0: 5a0c 6419 6413 6414 8401 5a0d 641a 6416  Z.d.d.d...Z.d.d.
+000003b0: 6417 8401 5a0e 6412 5300 291b da03 4c6f  d...Z.d.S.)...Lo
+000003c0: 67da 036c 6f67 6302 0000 0000 0000 0000  g..logc.........
+000003d0: 0000 0002 0000 0002 0000 0043 0000 0073  ...........C...s
+000003e0: 1000 0000 7c01 7c00 5f00 6400 7c00 5f01  ....|.|._.d.|._.
+000003f0: 6400 5300 a901 4e29 02da 066f 7574 7075  d.S...N)...outpu
+00000400: 74da 0a5f 7061 7468 5f66 696c 6529 02da  t.._path_file)..
+00000410: 0473 656c 6672 1e00 0000 720e 0000 0072  .selfr....r....r
+00000420: 0e00 0000 720f 0000 00da 085f 5f69 6e69  ....r......__ini
+00000430: 745f 5f1f 0000 0073 0400 0000 0601 0a01  t__....s........
+00000440: 7a0c 4c6f 672e 5f5f 696e 6974 5f5f 6301  z.Log.__init__c.
+00000450: 0000 0000 0000 0000 0000 0011 0000 0009  ................
+00000460: 0000 0043 0000 0073 a001 0000 7c00 6a00  ...C...s....|.j.
+00000470: 7d01 7401 a002 6401 7c01 a102 7d02 7c02  }.t...d.|...}.|.
+00000480: 6402 7501 7216 7403 7c02 a004 a100 6403  d.u.r.t.|.....d.
+00000490: 1900 8301 7d03 6e02 6404 7d03 7401 a002  ....}.n.d.}.t...
+000004a0: 6405 7c01 a102 7d02 7c02 6402 7501 722b  d.|...}.|.d.u.r+
+000004b0: 7403 7c02 a004 a100 6403 1900 8301 7d04  t.|.....d.....}.
+000004c0: 6e02 7405 8201 7401 a006 6406 7c01 a102  n.t...t...d.|...
+000004d0: 7d05 7401 a006 6407 7c01 a102 7d06 7c05  }.t...d.|...}.|.
+000004e0: 6402 7407 7c06 8301 8502 1900 7d05 7408  d.t.|.......}.t.
+000004f0: a009 6408 6409 8400 7c05 4400 8301 a101  ..d.d...|.D.....
+00000500: 7d05 7408 a009 640a 6409 8400 7c06 4400  }.t...d.d...|.D.
+00000510: 8301 a101 7d06 7c06 640b 1900 7407 7c06  ....}.|.d...t.|.
+00000520: 8301 1b00 7d07 7408 a00a 7c06 6a0b a101  ....}.t...|.j...
+00000530: 7d08 7408 6a0c 7c06 640c 640d 8d02 5c02  }.t.j.|.d.d...\.
+00000540: 7d06 7d09 7c05 7c09 1900 7d05 7c08 7c09  }.}.|.|...}.|.|.
+00000550: 1900 7d08 640e 7d0a 740d 740e 640f 7c0a  ..}.d.}.t.t.d.|.
+00000560: 1400 7c06 a00f a100 7c06 a00e a100 1800  ..|.....|.......
+00000570: 6410 1b00 8302 7c07 1b00 8301 7d0b 7c0b  d.....|.....}.|.
+00000580: 6411 6b04 72a2 7c06 6402 6402 7c0b 8503  d.k.r.|.d.d.|...
+00000590: 1900 7d06 7c05 6402 6402 7c0b 8503 1900  ..}.|.d.d.|.....
+000005a0: 7d05 7c08 6402 6402 7c0b 8503 1900 7d08  }.|.d.d.|.....}.
+000005b0: 7408 a010 7c05 a101 7d0c 7c05 6402 640b  t...|...}.|.d.d.
+000005c0: 8502 1900 7d05 7c04 7c05 1800 7d0d 7408  ....}.|.|...}.t.
+000005d0: a010 7c06 a101 7d0e 7c0d 7c0c 1b00 7c0e  ..|...}.|.|...|.
+000005e0: 1400 7d0f 7c05 7c0f 7c0e 7408 a010 7c08  ..}.|.|.|.t...|.
+000005f0: a101 1b00 7c03 7c06 640b 1900 7c0d 7c0c  ....|.|.d...|.|.
+00000600: 7c0e 6412 9c08 7d10 7c10 5300 2913 7ab8  |.d...}.|.S.).z.
+00000610: 4c6f 6164 2072 656d 6169 6e69 6e67 2074  Load remaining t
+00000620: 696d 6520 6461 7461 2e0a 0a20 2020 2020  ime data...     
+00000630: 2020 202d 2065 7175 6174 696f 6e5f 7469     - equation_ti
+00000640: 6d65 730a 2020 2020 2020 2020 2d20 7265  mes.        - re
+00000650: 6d61 696e 696e 675f 636c 6f63 6b5f 7469  maining_clock_ti
+00000660: 6d65 730a 2020 2020 2020 2020 2d20 636c  mes.        - cl
+00000670: 6f63 6b5f 7469 6d65 735f 7065 725f 7469  ock_times_per_ti
+00000680: 6d65 7374 6570 0a20 2020 2020 2020 202d  mestep.        -
+00000690: 2065 7175 6174 696f 6e5f 7469 6d65 5f73   equation_time_s
+000006a0: 7461 7274 0a20 2020 2020 2020 202d 2066  tart.        - f
+000006b0: 756c 6c5f 636c 6f63 6b5f 7469 6d65 0a0a  ull_clock_time..
+000006c0: 2020 2020 2020 2020 7a18 7374 6172 745f          z.start_
+000006d0: 7469 6d65 203d 2028 5b5c 645c 2e5d 2b29  time = ([\d\.]+)
+000006e0: 5c6e 4e72 0100 0000 e700 0000 0000 0000  \nNr............
+000006f0: 007a 1665 6e64 5f74 696d 6520 3d20 285b  .z.end_time = ([
+00000700: 5c64 5c2e 5d2b 295c 6e7a 1a5c 6e54 696d  \d\.]+)\nz.\nTim
+00000710: 6520 3d20 285b 5c64 5c2e 5d2b 653f 5b2d  e = ([\d\.]+e?[-
+00000720: 5c64 5d2a 297a 1b5c 6e45 7865 6375 7469  \d]*)z.\nExecuti
+00000730: 6f6e 5469 6d65 203d 2028 5b5c 645c 2e5d  onTime = ([\d\.]
+00000740: 2b29 6301 0000 0000 0000 0000 0000 0002  +)c.............
+00000750: 0000 0004 0000 0053 0000 00f3 1400 0000  .......S........
+00000760: 6700 7c00 5d06 7d01 7400 7c01 8301 9102  g.|.].}.t.|.....
+00000770: 7102 5300 720e 0000 00a9 0172 1600 0000  q.S.r......r....
+00000780: a902 da02 2e30 da04 776f 7264 720e 0000  .....0..wordr...
+00000790: 0072 0e00 0000 720f 0000 00da 0a3c 6c69  .r....r......<li
+000007a0: 7374 636f 6d70 3e3f 0000 00f3 0200 0000  stcomp>?........
+000007b0: 1400 7a23 4c6f 672e 5f6c 6f61 645f 7469  ..z#Log._load_ti
+000007c0: 6d65 732e 3c6c 6f63 616c 733e 2e3c 6c69  mes.<locals>.<li
+000007d0: 7374 636f 6d70 3e63 0100 0000 0000 0000  stcomp>c........
+000007e0: 0000 0000 0200 0000 0400 0000 5300 0000  ............S...
+000007f0: 7223 0000 0072 0e00 0000 7224 0000 0072  r#...r....r$...r
+00000800: 2500 0000 720e 0000 0072 0e00 0000 720f  %...r....r....r.
+00000810: 0000 0072 2800 0000 4000 0000 7229 0000  ...r(...@...r)..
+00000820: 0072 1100 0000 5429 01da 0c72 6574 7572  .r....T)...retur
+00000830: 6e5f 696e 6465 7867 7b14 ae47 e17a 843f  n_indexg{..G.z.?
+00000840: 7212 0000 00e9 0200 0000 7213 0000 0029  r.........r....)
+00000850: 085a 0e65 7175 6174 696f 6e5f 7469 6d65  .Z.equation_time
+00000860: 73da 1572 656d 6169 6e69 6e67 5f63 6c6f  s..remaining_clo
+00000870: 636b 5f74 696d 6573 5a18 636c 6f63 6b5f  ck_timesZ.clock_
+00000880: 7469 6d65 735f 7065 725f 7469 6d65 7374  times_per_timest
+00000890: 6570 da13 6571 7561 7469 6f6e 5f74 696d  ep..equation_tim
+000008a0: 655f 7374 6172 745a 0f66 756c 6c5f 636c  e_startZ.full_cl
+000008b0: 6f63 6b5f 7469 6d65 da12 7265 6d61 696e  ock_time..remain
+000008c0: 696e 675f 6571 5f74 696d 6573 da0e 6465  ing_eq_times..de
+000008d0: 6c74 615f 6571 5f74 696d 6573 da11 6465  lta_eq_times..de
+000008e0: 6c74 615f 636c 6f63 6b5f 7469 6d65 7329  lta_clock_times)
+000008f0: 1172 1800 0000 da02 7265 da06 7365 6172  .r......re..sear
+00000900: 6368 7216 0000 00da 0667 726f 7570 73da  chr......groups.
+00000910: 0c52 756e 7469 6d65 4572 726f 72da 0766  .RuntimeError..f
+00000920: 696e 6461 6c6c da03 6c65 6eda 026e 70da  indall..len..np.
+00000930: 0561 7272 6179 da06 6172 616e 6765 da04  .array..arange..
+00000940: 7369 7a65 da06 756e 6971 7565 da05 726f  size..unique..ro
+00000950: 756e 64da 036d 696e 7209 0000 00da 0464  und..minr......d
+00000960: 6966 6629 1172 2000 0000 7218 0000 00da  iff).r ...r.....
+00000970: 056d 6174 6368 722d 0000 005a 0b65 715f  .matchr-...Z.eq_
+00000980: 7469 6d65 5f65 6e64 5a08 6571 5f74 696d  time_endZ.eq_tim
+00000990: 6573 5a0b 636c 6f63 6b5f 7469 6d65 735a  esZ.clock_timesZ
+000009a0: 2365 7374 696d 6174 696f 6e5f 636c 6f63  #estimation_cloc
+000009b0: 6b5f 7469 6d65 5f70 6572 5f74 696d 655f  k_time_per_time_
+000009c0: 7374 6570 5a11 696e 6469 6365 735f 7469  stepZ.indices_ti
+000009d0: 6d65 5f73 7465 705a 0e69 6e64 6963 6573  me_stepZ.indices
+000009e0: 5f75 6e69 7175 655a 0f70 7265 6369 7369  _uniqueZ.precisi
+000009f0: 6f6e 5f63 6c6f 636b da04 7374 6570 722f  on_clock..stepr/
+00000a00: 0000 0072 2e00 0000 7230 0000 0072 2c00  ...r....r0...r,.
+00000a10: 0000 da04 6461 7461 720e 0000 0072 0e00  ....datar....r..
+00000a20: 0000 720f 0000 00da 0b5f 6c6f 6164 5f74  ..r......_load_t
+00000a30: 696d 6573 2300 0000 735e 0000 0006 0a0c  imes#...s^......
+00000a40: 0208 0112 0104 020c 0208 0112 0104 020c  ................
+00000a50: 020c 0110 0114 0214 0110 020c 0212 0308  ................
+00000a60: 0108 0104 0302 011c 0102 0102 ff04 ff08  ................
+00000a70: 040e 010e 010e 010a 020c 0208 010a 020a  ................
+00000a80: 0302 ff02 0502 0102 0108 0102 ff02 0206  ................
+00000a90: 0102 0102 0102 0106 f704 0c7a 0f4c 6f67  ...........z.Log
+00000aa0: 2e5f 6c6f 6164 5f74 696d 6573 6301 0000  ._load_timesc...
+00000ab0: 0000 0000 0000 0000 0004 0000 0004 0000  ................
+00000ac0: 0043 0000 0073 4a00 0000 7c00 6a00 7d01  .C...sJ...|.j.}.
+00000ad0: 7c01 7220 7c00 6a01 7320 7c01 6a02 7d02  |.r |.j.s |.j.}.
+00000ae0: 7403 7c02 a004 6401 a101 8301 7d03 7c03  t.|...d.....}.|.
+00000af0: 721a 7c03 6402 1900 7c00 5f01 6e06 7405  r.|.d...|._.n.t.
+00000b00: 6403 8301 0100 6400 5300 7c00 6a01 a006  d.....d.S.|.j...
+00000b10: a100 5300 2904 4e7a 086c 6f67 2a2e 7478  ..S.).Nz.log*.tx
+00000b20: 7472 1100 0000 7a11 4e6f 206c 6f67 2066  tr....z.No log f
+00000b30: 696c 6520 666f 756e 6429 0772 1e00 0000  ile found).r....
+00000b40: 721f 0000 00da 0870 6174 685f 7275 6eda  r......path_run.
+00000b50: 0673 6f72 7465 64da 0467 6c6f 6272 1500  .sorted..globr..
+00000b60: 0000 da07 7265 736f 6c76 6529 0472 2000  ....resolve).r .
+00000b70: 0000 721e 0000 0072 4300 0000 da08 6c6f  ..r....rC.....lo
+00000b80: 6766 696c 6573 720e 0000 0072 0e00 0000  gfilesr....r....
+00000b90: 720f 0000 0072 0b00 0000 6f00 0000 7312  r....r....o...s.
+00000ba0: 0000 0006 020a 0106 010e 0104 010c 0108  ................
+00000bb0: 0204 010a 027a 0d4c 6f67 2e70 6174 685f  .....z.Log.path_
+00000bc0: 6669 6c65 6302 0000 0000 0000 0000 0000  filec...........
+00000bd0: 0002 0000 0002 0000 0043 0000 0073 0a00  .........C...s..
+00000be0: 0000 7c01 7c00 5f00 6400 5300 721d 0000  ..|.|._.d.S.r...
+00000bf0: 0029 0172 1f00 0000 2902 7220 0000 005a  .).r....).r ...Z
+00000c00: 0d70 6174 685f 6c6f 675f 6669 6c65 720e  .path_log_filer.
+00000c10: 0000 0072 0e00 0000 720f 0000 0072 0b00  ...r....r....r..
+00000c20: 0000 7d00 0000 7302 0000 000a 0263 0100  ..}...s......c..
+00000c30: 0000 0000 0000 0000 0000 0200 0000 0800  ................
+00000c40: 0000 4300 0000 7344 0000 007c 006a 0064  ..C...sD...|.j.d
+00000c50: 0075 0072 0764 0053 0074 017c 006a 0083  .u.r.d.S.t.|.j..
+00000c60: 018f 0c7d 017c 01a0 02a1 0057 0002 0064  ...}.|.....W...d
+00000c70: 0004 0004 0083 0301 0053 0031 0073 1b77  .........S.1.s.w
+00000c80: 0101 0001 0001 0059 0001 0064 0053 0072  .......Y...d.S.r
+00000c90: 1d00 0000 2903 720b 0000 0072 0700 0000  ....).r....r....
+00000ca0: 720a 0000 0029 0272 2000 0000 720d 0000  r....).r ...r...
+00000cb0: 0072 0e00 0000 720e 0000 0072 0f00 0000  .r....r....r....
+00000cc0: 7218 0000 0081 0000 0073 0a00 0000 0a02  r........s......
+00000cd0: 0401 0c02 0601 24ff 7a08 4c6f 672e 7465  ......$.z.Log.te
+00000ce0: 7874 7203 0000 0063 0200 0000 0000 0000  xtr....c........
+00000cf0: 0000 0000 0200 0000 0300 0000 4300 0000  ............C...
+00000d00: 7328 0000 007c 006a 0064 0075 0072 0e74  s(...|.j.d.u.r.t
+00000d10: 0164 017c 006a 026a 039b 009d 0283 0182  .d.|.j.j........
+00000d20: 0174 047c 006a 007c 0183 0253 0029 024e  .t.|.j.|...S.).N
+00000d30: 7a15 4e6f 206c 6f67 2066 696c 6520 666f  z.No log file fo
+00000d40: 756e 6420 696e 2029 0572 0b00 0000 da07  und in ).r......
+00000d50: 494f 4572 726f 7272 1e00 0000 7243 0000  IOErrorr....rC..
+00000d60: 0072 1000 0000 2902 7220 0000 0072 0c00  .r....).r ...r..
+00000d70: 0000 720e 0000 0072 0e00 0000 720f 0000  ..r....r....r...
+00000d80: 0072 1000 0000 8900 0000 7306 0000 000a  .r........s.....
+00000d90: 0112 010c 017a 104c 6f67 2e67 6574 5f6c  .....z.Log.get_l
+00000da0: 6f67 5f74 6169 6c63 0100 0000 0000 0000  og_tailc........
+00000db0: 0000 0000 0100 0000 0200 0000 4300 0000  ............C...
+00000dc0: 7318 0000 007c 006a 0064 0075 0072 0764  s....|.j.d.u.r.d
+00000dd0: 0053 0074 017c 006a 0083 0153 0072 1d00  .S.t.|.j...S.r..
+00000de0: 0000 2902 720b 0000 0072 1a00 0000 2901  ..).r....r....).
+00000df0: 7220 0000 0072 0e00 0000 720e 0000 0072  r ...r....r....r
+00000e00: 0f00 0000 da09 7469 6d65 5f6c 6173 748e  ......time_last.
+00000e10: 0000 0073 0600 0000 0a02 0401 0a01 7a0d  ...s..........z.
+00000e20: 4c6f 672e 7469 6d65 5f6c 6173 7463 0200  Log.time_lastc..
+00000e30: 0000 0000 0000 0000 0000 0300 0000 0300  ................
+00000e40: 0000 4300 0000 7352 0000 007c 0164 0075  ..C...sR...|.d.u
+00000e50: 0172 137c 017c 006a 006a 0176 0172 1374  .r.|.|.j.j.v.r.t
+00000e60: 0264 017c 006a 006a 019b 009d 0283 0182  .d.|.j.j........
+00000e70: 017c 0164 0075 0072 2764 0244 005d 0d7d  .|.d.u.r'd.D.].}
+00000e80: 027c 027c 006a 006a 0176 0072 267c 027d  .|.|.j.j.v.r&|.}
+00000e90: 0101 007c 0153 0071 197c 0153 0029 034e  ...|.S.q.|.S.).N
+00000ea0: 7a1b 7661 7269 6162 6c65 5f6e 616d 6520  z.variable_name 
+00000eb0: 6861 7320 746f 2062 6520 696e 2029 02da  has to be in )..
+00000ec0: 0170 da06 705f 7262 6768 2903 721e 0000  .p..p_rbgh).r...
+00000ed0: 00da 0e6e 616d 655f 7661 7269 6162 6c65  ...name_variable
+00000ee0: 73da 0a56 616c 7565 4572 726f 7229 0372  s..ValueError).r
+00000ef0: 2000 0000 da0d 7661 7269 6162 6c65 5f6e   .....variable_n
+00000f00: 616d 65da 036b 6579 720e 0000 0072 0e00  ame..keyr....r..
+00000f10: 0000 720f 0000 00da 155f 6368 6f6f 7365  ..r......_choose
+00000f20: 5f76 6172 6961 626c 655f 6e61 6d65 9400  _variable_name..
+00000f30: 0000 731e 0000 0006 0202 ff0a 0202 fe02  ..s.............
+00000f40: 040c 0104 ff08 0408 010c 0104 0102 0104  ................
+00000f50: 0102 fd04 037a 194c 6f67 2e5f 6368 6f6f  .....z.Log._choo
+00000f60: 7365 5f76 6172 6961 626c 655f 6e61 6d65  se_variable_name
+00000f70: 4e63 0200 0000 0000 0000 0000 0000 0800  Nc..............
+00000f80: 0000 0600 0000 4300 0000 7382 0000 007c  ......C...s....|
+00000f90: 006a 0064 0075 0072 0764 0053 007c 00a0  .j.d.u.r.d.S.|..
+00000fa0: 0164 01a1 017d 027c 00a0 027c 01a1 017d  .d...}.|...|...}
+00000fb0: 0174 0374 04a0 0564 027c 019b 0064 039d  .t.t...d.|...d..
+00000fc0: 037c 02a1 0283 017d 037c 0373 2974 0664  .|.....}.|.s)t.d
+00000fd0: 047c 019b 0064 057c 029b 009d 0483 0182  .|...d.|........
+00000fe0: 017c 0364 0619 007d 047c 04a0 07a1 007d  .|.d...}.|.....}
+00000ff0: 0574 087c 0564 0719 0083 017d 0674 087c  .t.|.d.....}.t.|
+00001000: 0564 0819 0083 017d 077c 067c 0766 0253  .d.....}.|.|.f.S
+00001010: 0029 094e 6988 1300 00fa 375c 6e54 696d  .).Ni.....7\nTim
+00001020: 6520 3d20 283f 503c 7469 6d65 3e5b 5c64  e = (?P<time>[\d
+00001030: 5c2e 5d2b 653f 2d3f 5b5c 645d 2a29 5b5c  \.]+e?-?[\d]*)[\
+00001040: 735c 535d 2b3f 536f 6c76 696e 6720 666f  s\S]+?Solving fo
+00001050: 7220 fa32 2c20 496e 6974 6961 6c20 7265  r .2, Initial re
+00001060: 7369 6475 616c 203d 2028 3f50 3c69 6e69  sidual = (?P<ini
+00001070: 7469 616c 3e5b 5c64 5c2e 5d2b 653f 2d3f  tial>[\d\.]+e?-?
+00001080: 5b5c 645d 2a29 7a13 4e6f 206d 6174 6368  [\d]*)z.No match
+00001090: 2066 6f75 6e64 2066 6f72 207a 082c 2074   found for z., t
+000010a0: 6578 743d 0a72 1100 0000 da04 7469 6d65  ext=.r......time
+000010b0: da07 696e 6974 6961 6c29 0972 0b00 0000  ..initial).r....
+000010c0: 7210 0000 0072 5000 0000 da04 6c69 7374  r....rP.....list
+000010d0: 7231 0000 00da 0866 696e 6469 7465 7272  r1.....finditerr
+000010e0: 4d00 0000 da09 6772 6f75 7064 6963 7472  M.....groupdictr
+000010f0: 1600 0000 2908 7220 0000 0072 4e00 0000  ....).r ...rN...
+00001100: 7218 0000 00da 076d 6174 6368 6573 723f  r......matchesr?
+00001110: 0000 0072 4100 0000 7253 0000 005a 0872  ...rA...rS...Z.r
+00001120: 6573 6964 7561 6c72 0e00 0000 720e 0000  esidualr....r...
+00001130: 0072 0f00 0000 da11 6765 745f 6c61 7374  .r......get_last
+00001140: 5f72 6573 6964 7561 6ca4 0000 0073 2600  _residual....s&.
+00001150: 0000 0a01 0401 0a01 0a02 0201 0401 0201  ................
+00001160: 0201 06ff 0203 02fc 04ff 0409 1401 0802  ................
+00001170: 0801 0c01 0c01 0801 7a15 4c6f 672e 6765  ........z.Log.ge
+00001180: 745f 6c61 7374 5f72 6573 6964 7561 6c72  t_last_residualr
+00001190: 2200 0000 6303 0000 0000 0000 0000 0000  "...c...........
+000011a0: 000b 0000 0006 0000 0043 0000 0073 c000  .........C...s..
+000011b0: 0000 7c00 a000 7c01 a101 7d01 7401 7402  ..|...|...}.t.t.
+000011c0: a003 6401 7c01 9b00 6402 9d03 7c00 6a04  ..d.|...d...|.j.
+000011d0: a102 8301 7d03 7405 a006 7407 7c03 8301  ....}.t...t.|...
+000011e0: a101 7d04 7405 a008 7c04 a101 7d05 7409  ..}.t...|...}.t.
+000011f0: 7c03 8301 4400 5d14 5c02 7d06 7d07 7c07  |...D.].\.}.}.|.
+00001200: a00a a100 7d08 7c08 6403 1900 7c04 7c06  ....}.|.d...|.|.
+00001210: 3c00 7c08 6404 1900 7c05 7c06 3c00 7122  <.|.d...|.|.<.q"
+00001220: 740b a00c a100 5c02 7d09 7d0a 7c05 7c04  t.....\.}.}.|.|.
+00001230: 7c02 6b04 1900 7d05 7c04 7c04 7c02 6b04  |.k...}.|.|.|.k.
+00001240: 1900 7d04 7c0a a00d 7c04 7c05 a102 0100  ..}.|...|.|.....
+00001250: 7c0a a00e 6405 a101 0100 7c09 a00f 6406  |...d.....|...d.
+00001260: 7c01 9b00 9d02 a101 0100 7c04 7c05 6602  |.........|.|.f.
+00001270: 5300 2907 4e72 5100 0000 7252 0000 0072  S.).NrQ...rR...r
+00001280: 5300 0000 7254 0000 007a 0d65 7175 6174  S...rT...z.equat
+00001290: 696f 6e20 7469 6d65 7a12 496e 6974 6961  ion timez.Initia
+000012a0: 6c20 7265 7369 6475 616c 7320 2910 7250  l residuals ).rP
+000012b0: 0000 0072 5500 0000 7231 0000 0072 5600  ...rU...r1...rV.
+000012c0: 0000 7218 0000 0072 3700 0000 da05 656d  ..r....r7.....em
+000012d0: 7074 7972 3600 0000 da0a 656d 7074 795f  ptyr6.....empty_
+000012e0: 6c69 6b65 da09 656e 756d 6572 6174 6572  like..enumerater
+000012f0: 5700 0000 da03 706c 74da 0873 7562 706c  W.....plt..subpl
+00001300: 6f74 73da 0470 6c6f 74da 0a73 6574 5f78  ots..plot..set_x
+00001310: 6c61 6265 6cda 0873 7570 7469 746c 6529  label..suptitle)
+00001320: 0b72 2000 0000 724e 0000 00da 0474 6d69  .r ...rN.....tmi
+00001330: 6e72 5800 0000 da05 7469 6d65 735a 0972  nrX.....timesZ.r
+00001340: 6573 6964 7561 6c73 7219 0000 0072 3f00  esidualsr....r?.
+00001350: 0000 7241 0000 00da 0366 6967 da02 6178  ..rA.....fig..ax
+00001360: 720e 0000 0072 0e00 0000 720f 0000 00da  r....r....r.....
+00001370: 0e70 6c6f 745f 7265 7369 6475 616c 73bc  .plot_residuals.
+00001380: 0000 0073 2c00 0000 0a01 0201 0401 0201  ...s,...........
+00001390: 0201 06ff 0403 02fc 04ff 0e09 0a01 1002  ................
+000013a0: 0801 0c02 0e01 0c02 0c02 0c01 0c01 0a01  ................
+000013b0: 1001 0801 7a12 4c6f 672e 706c 6f74 5f72  ....z.Log.plot_r
+000013c0: 6573 6964 7561 6c73 a901 7203 0000 0072  esiduals..r....r
+000013d0: 1d00 0000 2902 4e72 2200 0000 290f da08  ....).Nr"...)...
+000013e0: 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f 6475  __name__..__modu
+000013f0: 6c65 5f5f da0c 5f5f 7175 616c 6e61 6d65  le__..__qualname
+00001400: 5f5f da04 5f74 6167 7221 0000 0072 4200  __.._tagr!...rB.
+00001410: 0000 da08 7072 6f70 6572 7479 720b 0000  ....propertyr...
+00001420: 00da 0673 6574 7465 7272 1800 0000 7210  ...setterr....r.
+00001430: 0000 0072 4900 0000 7250 0000 0072 5900  ...rI...rP...rY.
+00001440: 0000 7266 0000 0072 0e00 0000 720e 0000  ..rf...r....r...
+00001450: 0072 0e00 0000 720f 0000 0072 1b00 0000  .r....r....r....
+00001460: 1c00 0000 7320 0000 0008 0004 0108 0208  ....s ..........
+00001470: 0402 4c0a 0104 0d0a 0102 030a 010a 0702  ..L.............
+00001480: 050a 0108 050a 100e 1872 1b00 0000 7267  .........r....rg
+00001490: 0000 0029 0cda 075f 5f64 6f63 5f5f 7231  ...)...__doc__r1
+000014a0: 0000 00da 116d 6174 706c 6f74 6c69 622e  .....matplotlib.
+000014b0: 7079 706c 6f74 da06 7079 706c 6f74 725d  pyplot..pyplotr]
+000014c0: 0000 00da 056e 756d 7079 7237 0000 005a  .....numpyr7...Z
+000014d0: 2966 6c75 6964 7369 6d5f 636f 7265 2e6f  )fluidsim_core.o
+000014e0: 7574 7075 742e 7265 6d61 696e 696e 675f  utput.remaining_
+000014f0: 636c 6f63 6b5f 7469 6d65 7202 0000 0072  clock_timer....r
+00001500: 1000 0000 721a 0000 0072 1b00 0000 720e  ....r....r....r.
+00001510: 0000 0072 0e00 0000 720e 0000 0072 0f00  ...r....r....r..
+00001520: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
+00001530: 7310 0000 0004 0008 020c 0208 010c 020a  s...............
+00001540: 0308 0714 0a                             .....
```

### Comparing `fluidsimfoam-0.0.5/src/fluidsimfoam/output/base.py` & `fluidsimfoam-0.0.6/src/fluidsimfoam/output/base.py`

 * *Files identical despite different names*

### Comparing `fluidsimfoam-0.0.5/src/fluidsimfoam/output/dataframe_from_paths.py` & `fluidsimfoam-0.0.6/src/fluidsimfoam/output/dataframe_from_paths.py`

 * *Files identical despite different names*

### Comparing `fluidsimfoam-0.0.5/src/fluidsimfoam/output/fields.py` & `fluidsimfoam-0.0.6/src/fluidsimfoam/output/fields.py`

 * *Files 6% similar despite different names*

```diff
@@ -57,20 +57,17 @@
 
         path_dir, last_time = self.get_path_dir_time(time_approx)
 
         if self.sim.params.parallel.nsubdoms > 1:
             _, last_time_proc0 = self.get_path_dir_time(
                 time_approx, dirname="processor0"
             )
-
             if last_time_proc0 != last_time:
                 self.reconstruct_par(fields=[name], time=last_time_proc0)
-
-        path_dir, last_time = self.get_path_dir_time(time_approx)
-        if self.sim.params.parallel.nsubdoms > 1:
+            path_dir, last_time = self.get_path_dir_time(time_approx)
             assert last_time == last_time_proc0
 
         field = read_field_file(path_dir / name)
         field.time = float(path_dir.name)
         return field
 
     def reconstruct_par(self, fields=None, latest_time=None, time=None):
```

### Comparing `fluidsimfoam-0.0.5/src/fluidsimfoam/output/log.py` & `fluidsimfoam-0.0.6/src/fluidsimfoam/output/log.py`

 * *Files identical despite different names*

### Comparing `fluidsimfoam-0.0.5/src/fluidsimfoam/params.py` & `fluidsimfoam-0.0.6/src/fluidsimfoam/params.py`

 * *Files identical despite different names*

### Comparing `fluidsimfoam-0.0.5/src/fluidsimfoam/resources/LICENSE.template` & `fluidsimfoam-0.0.6/src/fluidsimfoam/resources/LICENSE.template`

 * *Files identical despite different names*

### Comparing `fluidsimfoam-0.0.5/src/fluidsimfoam/resources/__init__.py` & `fluidsimfoam-0.0.6/src/fluidsimfoam/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `fluidsimfoam-0.0.5/src/fluidsimfoam/resources/__init__.py.template` & `fluidsimfoam-0.0.6/src/fluidsimfoam/resources/__init__.py.template`

 * *Files identical despite different names*

### Comparing `fluidsimfoam-0.0.5/src/fluidsimfoam/resources/__pycache__/__init__.cpython-310.pyc` & `fluidsimfoam-0.0.6/src/fluidsimfoam/resources/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed May 10 08:15:22 2023 UTC, .py size: 573 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 9a52 5b64 3d02 0000  o........R[d=...
+00000000: 6f0d 0d0a 0000 0000 6b44 5a64 3d02 0000  o.......kDZd=...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 2a00 0000 6400  .....@...s*...d.
 00000030: 5a00 6401 6402 6c01 5a01 4700 6403 6404  Z.d.d.l.Z.G.d.d.
 00000040: 8400 6404 8302 5a02 6502 8300 5a03 6503  ..d...Z.e...Z.e.
 00000050: 6a04 5a04 6402 5300 2905 7a44 5375 6270  j.Z.d.S.).zDSubp
 00000060: 6163 6b61 6765 2063 6f6e 7461 696e 696e  ackage containin
 00000070: 6720 706f 7465 6e74 6961 6c20 7465 6d70  g potential temp
@@ -21,41 +21,40 @@
 00000140: 7265 736f 7572 6365 7354 2903 da06 6c6f  resourcesT)...lo
 00000150: 6164 6572 da09 756e 6465 6669 6e65 64da  ader..undefined.
 00000160: 156b 6565 705f 7472 6169 6c69 6e67 5f6e  .keep_trailing_n
 00000170: 6577 6c69 6e65 2904 da06 6a69 6e6a 6132  ewline)...jinja2
 00000180: da0b 456e 7669 726f 6e6d 656e 74da 0d50  ..Environment..P
 00000190: 6163 6b61 6765 4c6f 6164 6572 da0f 5374  ackageLoader..St
 000001a0: 7269 6374 556e 6465 6669 6e65 6429 01da  rictUndefined)..
-000001b0: 0473 656c 66a9 0072 0d00 0000 fa4d 2f68  .self..r.....M/h
-000001c0: 6f6d 652f 7573 6572 732f 6175 6769 6572  ome/users/augier
-000001d0: 3370 692f 4465 762f 666c 7569 6473 696d  3pi/Dev/fluidsim
-000001e0: 666f 616d 2f73 7263 2f66 6c75 6964 7369  foam/src/fluidsi
-000001f0: 6d66 6f61 6d2f 7265 736f 7572 6365 732f  mfoam/resources/
-00000200: 5f5f 696e 6974 5f5f 2e70 79da 0365 6e76  __init__.py..env
-00000210: 0900 0000 730a 0000 0004 020a 0104 0102  ....s...........
-00000220: 0106 fd7a 1142 6173 6554 656d 706c 6174  ...z.BaseTemplat
-00000230: 6573 2e65 6e76 6302 0000 0000 0000 0000  es.envc.........
-00000240: 0000 0002 0000 0003 0000 0043 0000 0073  ...........C...s
-00000250: 0c00 0000 7c00 6a00 a001 7c01 a101 5300  ....|.j...|...S.
-00000260: 2901 7a2f 4765 7420 6120 7465 6d70 6c61  ).z/Get a templa
-00000270: 7465 2066 726f 6d20 6060 666c 7569 6473  te from ``fluids
-00000280: 696d 666f 616d 2e72 6573 6f75 7263 6573  imfoam.resources
-00000290: 6060 2e29 0272 0f00 0000 da0c 6765 745f  ``.).r......get_
-000002a0: 7465 6d70 6c61 7465 2902 720c 0000 00da  template).r.....
-000002b0: 046e 616d 6572 0d00 0000 720d 0000 0072  .namer....r....r
-000002c0: 0e00 0000 da11 6765 745f 6261 7365 5f74  ......get_base_t
-000002d0: 656d 706c 6174 6511 0000 0073 0200 0000  emplate....s....
-000002e0: 0c02 7a1f 4261 7365 5465 6d70 6c61 7465  ..z.BaseTemplate
-000002f0: 732e 6765 745f 6261 7365 5f74 656d 706c  s.get_base_templ
-00000300: 6174 654e 2906 da08 5f5f 6e61 6d65 5f5f  ateN)...__name__
-00000310: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
-00000320: 7175 616c 6e61 6d65 5f5f da08 7072 6f70  qualname__..prop
-00000330: 6572 7479 720f 0000 0072 1200 0000 720d  ertyr....r....r.
-00000340: 0000 0072 0d00 0000 720d 0000 0072 0e00  ...r....r....r..
-00000350: 0000 7202 0000 0008 0000 0073 0800 0000  ..r........s....
-00000360: 0800 0201 0a01 0c07 7202 0000 0029 05da  ........r....)..
-00000370: 075f 5f64 6f63 5f5f 7208 0000 0072 0200  .__doc__r....r..
-00000380: 0000 da0a 5f74 656d 706c 6174 6573 7212  ...._templatesr.
-00000390: 0000 0072 0d00 0000 720d 0000 0072 0d00  ...r....r....r..
-000003a0: 0000 720e 0000 00da 083c 6d6f 6475 6c65  ..r......<module
-000003b0: 3e01 0000 0073 0a00 0000 0400 0804 0e03  >....s..........
-000003c0: 060e 0a02                                ....
+000001b0: 0473 656c 66a9 0072 0d00 0000 fa44 2f68  .self..r.....D/h
+000001c0: 6f6d 652f 7069 6572 7265 2f44 6576 2f66  ome/pierre/Dev/f
+000001d0: 6c75 6964 7369 6d66 6f61 6d2f 7372 632f  luidsimfoam/src/
+000001e0: 666c 7569 6473 696d 666f 616d 2f72 6573  fluidsimfoam/res
+000001f0: 6f75 7263 6573 2f5f 5f69 6e69 745f 5f2e  ources/__init__.
+00000200: 7079 da03 656e 7609 0000 0073 0a00 0000  py..env....s....
+00000210: 0402 0a01 0401 0201 06fd 7a11 4261 7365  ..........z.Base
+00000220: 5465 6d70 6c61 7465 732e 656e 7663 0200  Templates.envc..
+00000230: 0000 0000 0000 0000 0000 0200 0000 0300  ................
+00000240: 0000 4300 0000 730c 0000 007c 006a 00a0  ..C...s....|.j..
+00000250: 017c 01a1 0153 0029 017a 2f47 6574 2061  .|...S.).z/Get a
+00000260: 2074 656d 706c 6174 6520 6672 6f6d 2060   template from `
+00000270: 6066 6c75 6964 7369 6d66 6f61 6d2e 7265  `fluidsimfoam.re
+00000280: 736f 7572 6365 7360 602e 2902 720f 0000  sources``.).r...
+00000290: 00da 0c67 6574 5f74 656d 706c 6174 6529  ...get_template)
+000002a0: 0272 0c00 0000 da04 6e61 6d65 720d 0000  .r......namer...
+000002b0: 0072 0d00 0000 720e 0000 00da 1167 6574  .r....r......get
+000002c0: 5f62 6173 655f 7465 6d70 6c61 7465 1100  _base_template..
+000002d0: 0000 7302 0000 000c 027a 1f42 6173 6554  ..s......z.BaseT
+000002e0: 656d 706c 6174 6573 2e67 6574 5f62 6173  emplates.get_bas
+000002f0: 655f 7465 6d70 6c61 7465 4e29 06da 085f  e_templateN)..._
+00000300: 5f6e 616d 655f 5fda 0a5f 5f6d 6f64 756c  _name__..__modul
+00000310: 655f 5fda 0c5f 5f71 7561 6c6e 616d 655f  e__..__qualname_
+00000320: 5fda 0870 726f 7065 7274 7972 0f00 0000  _..propertyr....
+00000330: 7212 0000 0072 0d00 0000 720d 0000 0072  r....r....r....r
+00000340: 0d00 0000 720e 0000 0072 0200 0000 0800  ....r....r......
+00000350: 0000 7308 0000 0008 0002 010a 010c 0772  ..s............r
+00000360: 0200 0000 2905 da07 5f5f 646f 635f 5f72  ....)...__doc__r
+00000370: 0800 0000 7202 0000 00da 0a5f 7465 6d70  ....r......_temp
+00000380: 6c61 7465 7372 1200 0000 720d 0000 0072  latesr....r....r
+00000390: 0d00 0000 720d 0000 0072 0e00 0000 da08  ....r....r......
+000003a0: 3c6d 6f64 756c 653e 0100 0000 730a 0000  <module>....s...
+000003b0: 0004 0008 040e 0306 0e0a 02              ...........
```

### Comparing `fluidsimfoam-0.0.5/src/fluidsimfoam/resources/output.py.template` & `fluidsimfoam-0.0.6/src/fluidsimfoam/resources/output.py.template`

 * *Files identical despite different names*

### Comparing `fluidsimfoam-0.0.5/src/fluidsimfoam/resources/test_generated_solver.py.template` & `fluidsimfoam-0.0.6/src/fluidsimfoam/resources/test_generated_solver.py.template`

 * *Files identical despite different names*

### Comparing `fluidsimfoam-0.0.5/src/fluidsimfoam/solvers/__init__.py` & `fluidsimfoam-0.0.6/src/fluidsimfoam/solvers/__init__.py`

 * *Files identical despite different names*

### Comparing `fluidsimfoam-0.0.5/src/fluidsimfoam/solvers/__pycache__/__init__.cpython-310.pyc` & `fluidsimfoam-0.0.6/src/fluidsimfoam/solvers/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed May 10 08:15:22 2023 UTC, .py size: 2765 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 9a52 5b64 cd0a 0000  o........R[d....
+00000000: 6f0d 0d0a 0000 0000 f444 5a64 cd0a 0000  o........DZd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 9800 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 0100 6401 6404 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6401 6405 6c06 6d07 5a07 0100 6401  ..d.d.l.m.Z...d.
 00000060: 6406 6c08 6d09 5a09 0100 6401 6407 6c0a  d.l.m.Z...d.d.l.
 00000070: 6d0b 5a0b 0100 6408 6409 6c0c 6d0d 5a0d  m.Z...d.d.l.m.Z.
@@ -62,104 +62,103 @@
 000003d0: da04 7574 696c da09 6669 6e64 5f73 7065  ..util..find_spe
 000003e0: 6372 0400 0000 da08 5f5f 7370 6563 5f5f  cr......__spec__
 000003f0: 7203 0000 00da 0569 7370 6b67 da0a 5661  r......ispkg..Va
 00000400: 6c75 6545 7272 6f72 da04 7479 7065 da1a  lueError..type..
 00000410: 7375 626d 6f64 756c 655f 7365 6172 6368  submodule_search
 00000420: 5f6c 6f63 6174 696f 6e73 2902 da06 6d6f  _locations)...mo
 00000430: 6475 6c65 da04 7370 6563 a900 7215 0000  dule..spec..r...
-00000440: 00fa 4b2f 686f 6d65 2f75 7365 7273 2f61  ..K/home/users/a
-00000450: 7567 6965 7233 7069 2f44 6576 2f66 6c75  ugier3pi/Dev/flu
-00000460: 6964 7369 6d66 6f61 6d2f 7372 632f 666c  idsimfoam/src/fl
-00000470: 7569 6473 696d 666f 616d 2f73 6f6c 7665  uidsimfoam/solve
-00000480: 7273 2f5f 5f69 6e69 745f 5f2e 7079 da0a  rs/__init__.py..
-00000490: 6973 5f70 6163 6b61 6765 2200 0000 7310  is_package"...s.
-000004a0: 0000 000a 0e0e 010a 0108 010a 0106 0112  ................
-000004b0: 020a 0272 1700 0000 6301 0000 0000 0000  ...r....c.......
-000004c0: 0000 0000 0003 0000 0008 0000 0043 0000  .............C..
-000004d0: 0073 4800 0000 7400 8300 7c00 1900 7d01  .sH...t...|...}.
-000004e0: 7a05 7c01 6a01 7d02 5700 6e0c 0400 7402  z.|.j.}.W.n...t.
-000004f0: 7916 0100 0100 0100 7c01 6a03 7d02 5900  y.......|.j.}.Y.
-00000500: 6e01 7700 7404 7c02 8301 721d 7c02 5300  n.w.t.|...r.|.S.
-00000510: 7c02 a005 6401 a101 6402 1900 5300 2903  |...d...d...S.).
-00000520: 7ad8 5265 7475 726e 206e 616d 6520 6f66  z.Return name of
-00000530: 2074 6865 2073 6f6c 7665 7220 7061 636b   the solver pack
-00000540: 6167 6520 6279 2063 6865 636b 696e 6720  age by checking 
-00000550: 7468 6520 6060 736e 656b 3530 3030 2e73  the ``snek5000.s
-00000560: 6f6c 7665 7273 6060 0a20 2020 2065 6e74  olvers``.    ent
-00000570: 7279 706f 696e 7420 6772 6f75 702e 0a0a  rypoint group...
-00000580: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
-00000590: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
-000005a0: 2020 6e61 6d65 5f73 6f6c 7665 723a 2073    name_solver: s
-000005b0: 7472 0a20 2020 2020 2020 2053 686f 7274  tr.        Short
-000005c0: 206e 616d 6520 6f66 2074 6865 2073 6f6c   name of the sol
-000005d0: 7665 720a 0a20 2020 2052 6574 7572 6e73  ver..    Returns
-000005e0: 0a20 2020 202d 2d2d 2d2d 2d2d 0a20 2020  .    -------.   
-000005f0: 2073 7472 0a0a 2020 2020 da01 2e72 0100   str..    ...r..
-00000600: 0000 2906 da11 6176 6169 6c61 626c 655f  ..)...available_
-00000610: 736f 6c76 6572 7372 1300 0000 da0e 4174  solversr......At
-00000620: 7472 6962 7574 6545 7272 6f72 da0b 6d6f  tributeError..mo
-00000630: 6475 6c65 5f6e 616d 6572 1700 0000 da0a  dule_namer......
-00000640: 7270 6172 7469 7469 6f6e 2903 da0b 6e61  rpartition)...na
-00000650: 6d65 5f73 6f6c 7665 72da 0a65 6e74 7279  me_solver..entry
-00000660: 706f 696e 7472 1300 0000 7215 0000 0072  pointr....r....r
-00000670: 1500 0000 7216 0000 00da 1267 6574 5f73  ....r......get_s
-00000680: 6f6c 7665 725f 7061 636b 6167 653c 0000  olver_package<..
-00000690: 0073 1200 0000 0a0e 0201 0a02 0c01 0a01  .s..............
-000006a0: 02ff 0802 0401 0e02 721f 0000 0063 0100  ........r....c..
-000006b0: 0000 0000 0000 0000 0000 0400 0000 0500  ................
-000006c0: 0000 4300 0000 735e 0000 007c 0064 011b  ..C...s^...|.d..
-000006d0: 007d 017c 01a0 00a1 0073 0c7c 0064 021b  .}.|.....s.|.d..
-000006e0: 007d 017c 01a0 00a1 0072 1a74 017c 0164  .}.|.....r.t.|.d
-000006f0: 038d 017d 027c 026a 027d 037c 0353 0074  ...}.|.j.}.|.S.t
-00000700: 03a0 0464 047c 019b 0064 059d 03a1 0101  ...d.|...d......
-00000710: 007c 00a0 05a1 006a 06a0 0764 06a1 0164  .|.....j...d...d
-00000720: 0719 007d 037c 0353 0029 087a e644 6574  ...}.|.S.).z.Det
-00000730: 6563 7473 2073 686f 7274 206e 616d 6520  ects short name 
-00000740: 6f66 2074 6865 2073 6f6c 7665 7220 6672  of the solver fr
-00000750: 6f6d 2060 6069 6e66 6f5f 736f 6c76 6572  om ``info_solver
-00000760: 2e78 6d6c 6060 2069 6620 7072 6573 656e  .xml`` if presen
-00000770: 7420 6f72 0a20 2020 2074 6865 2070 6174  t or.    the pat
-00000780: 682e 0a0a 2020 2020 5061 7261 6d65 7465  h...    Paramete
-00000790: 7273 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  rs.    ---------
-000007a0: 2d0a 2020 2020 7061 7468 5f64 6972 3a20  -.    path_dir: 
-000007b0: 7061 7468 2d6c 696b 650a 2020 2020 2020  path-like.      
-000007c0: 2020 5061 7468 2074 6f20 6120 7369 6d75    Path to a simu
-000007d0: 6c61 7469 6f6e 2064 6972 6563 746f 7279  lation directory
-000007e0: 0a0a 2020 2020 5265 7475 726e 730a 2020  ..    Returns.  
-000007f0: 2020 2d2d 2d2d 2d2d 2d0a 2020 2020 7368    -------.    sh
-00000800: 6f72 745f 6e61 6d65 3a20 7374 720a 0a20  ort_name: str.. 
-00000810: 2020 207a 0f69 6e66 6f5f 736f 6c76 6572     z.info_solver
-00000820: 2e78 6d6c 7a1e 2e64 6174 615f 666c 7569  .xmlz..data_flui
-00000830: 6473 696d 2f69 6e66 6f5f 736f 6c76 6572  dsim/info_solver
-00000840: 2e78 6d6c 2901 da09 7061 7468 5f66 696c  .xml)...path_fil
-00000850: 657a 0454 6865 207a 4520 6669 6c65 2069  ez.The zE file i
-00000860: 7320 6d69 7373 696e 6721 2041 7474 656d  s missing! Attem
-00000870: 7074 696e 6720 746f 2067 7565 7373 2073  pting to guess s
-00000880: 6f6c 7665 7220 6672 6f6d 2074 6865 2064  olver from the d
-00000890: 6972 6563 746f 7279 206e 616d 652e da01  irectory name...
-000008a0: 5f72 0100 0000 2908 da06 6578 6973 7473  _r....)...exists
-000008b0: 7206 0000 00da 0a73 686f 7274 5f6e 616d  r......short_nam
-000008c0: 6572 0800 0000 da07 7761 726e 696e 67da  er......warning.
-000008d0: 0861 6273 6f6c 7574 65da 046e 616d 65da  .absolute..name.
-000008e0: 0573 706c 6974 2904 da08 7061 7468 5f64  .split)...path_d
-000008f0: 6972 5a0f 696e 666f 5f73 6f6c 7665 725f  irZ.info_solver_
-00000900: 786d 6cda 0b69 6e66 6f5f 736f 6c76 6572  xml..info_solver
-00000910: 7223 0000 0072 1500 0000 7215 0000 0072  r#...r....r....r
-00000920: 1600 0000 da15 6765 745f 736f 6c76 6572  ......get_solver
-00000930: 5f73 686f 7274 5f6e 616d 6556 0000 0073  _short_nameV...s
-00000940: 1800 0000 080e 0801 0801 0802 0a01 0601  ................
-00000950: 0408 04fa 0a01 04ff 1404 0402 722a 0000  ............r*..
-00000960: 0029 13da 075f 5f64 6f63 5f5f 720b 0000  .)...__doc__r...
-00000970: 00da 0966 756e 6374 6f6f 6c73 7202 0000  ...functoolsr...
-00000980: 00da 0770 6b67 7574 696c 7203 0000 00da  ...pkgutilr.....
-00000990: 0574 7970 6573 7204 0000 005a 0d66 6c75  .typesr....Z.flu
-000009a0: 6964 7369 6d5f 636f 7265 7205 0000 005a  idsim_corer....Z
-000009b0: 1266 6c75 6964 7369 6d5f 636f 7265 2e69  .fluidsim_core.i
-000009c0: 6e66 6f72 0600 0000 da03 6c6f 6772 0800  nfor......logr..
-000009d0: 0000 7219 0000 00da 1069 6d70 6f72 745f  ..r......import_
-000009e0: 636c 735f 7369 6d75 6c72 1700 0000 721f  cls_simulr....r.
-000009f0: 0000 0072 2a00 0000 7215 0000 0072 1500  ...r*...r....r..
-00000a00: 0000 7215 0000 0072 1600 0000 da08 3c6d  ..r....r......<m
-00000a10: 6f64 756c 653e 0100 0000 7326 0000 0004  odule>....s&....
-00000a20: 0008 0a0c 010c 010c 010c 020c 010c 0202  ................
-00000a30: 0206 0106 ff06 0302 0406 0106 ff06 0308  ................
-00000a40: 0308 1a0c 1a                             .....
+00000440: 00fa 422f 686f 6d65 2f70 6965 7272 652f  ..B/home/pierre/
+00000450: 4465 762f 666c 7569 6473 696d 666f 616d  Dev/fluidsimfoam
+00000460: 2f73 7263 2f66 6c75 6964 7369 6d66 6f61  /src/fluidsimfoa
+00000470: 6d2f 736f 6c76 6572 732f 5f5f 696e 6974  m/solvers/__init
+00000480: 5f5f 2e70 79da 0a69 735f 7061 636b 6167  __.py..is_packag
+00000490: 6522 0000 0073 1000 0000 0a0e 0e01 0a01  e"...s..........
+000004a0: 0801 0a01 0601 1202 0a02 7217 0000 0063  ..........r....c
+000004b0: 0100 0000 0000 0000 0000 0000 0300 0000  ................
+000004c0: 0800 0000 4300 0000 7348 0000 0074 0083  ....C...sH...t..
+000004d0: 007c 0019 007d 017a 057c 016a 017d 0257  .|...}.z.|.j.}.W
+000004e0: 006e 0c04 0074 0279 1601 0001 0001 007c  .n...t.y.......|
+000004f0: 016a 037d 0259 006e 0177 0074 047c 0283  .j.}.Y.n.w.t.|..
+00000500: 0172 1d7c 0253 007c 02a0 0564 01a1 0164  .r.|.S.|...d...d
+00000510: 0219 0053 0029 037a d852 6574 7572 6e20  ...S.).z.Return 
+00000520: 6e61 6d65 206f 6620 7468 6520 736f 6c76  name of the solv
+00000530: 6572 2070 6163 6b61 6765 2062 7920 6368  er package by ch
+00000540: 6563 6b69 6e67 2074 6865 2060 6073 6e65  ecking the ``sne
+00000550: 6b35 3030 302e 736f 6c76 6572 7360 600a  k5000.solvers``.
+00000560: 2020 2020 656e 7472 7970 6f69 6e74 2067      entrypoint g
+00000570: 726f 7570 2e0a 0a20 2020 2050 6172 616d  roup...    Param
+00000580: 6574 6572 730a 2020 2020 2d2d 2d2d 2d2d  eters.    ------
+00000590: 2d2d 2d2d 0a20 2020 206e 616d 655f 736f  ----.    name_so
+000005a0: 6c76 6572 3a20 7374 720a 2020 2020 2020  lver: str.      
+000005b0: 2020 5368 6f72 7420 6e61 6d65 206f 6620    Short name of 
+000005c0: 7468 6520 736f 6c76 6572 0a0a 2020 2020  the solver..    
+000005d0: 5265 7475 726e 730a 2020 2020 2d2d 2d2d  Returns.    ----
+000005e0: 2d2d 2d0a 2020 2020 7374 720a 0a20 2020  ---.    str..   
+000005f0: 20da 012e 7201 0000 0029 06da 1161 7661   ...r....)...ava
+00000600: 696c 6162 6c65 5f73 6f6c 7665 7273 7213  ilable_solversr.
+00000610: 0000 00da 0e41 7474 7269 6275 7465 4572  .....AttributeEr
+00000620: 726f 72da 0b6d 6f64 756c 655f 6e61 6d65  ror..module_name
+00000630: 7217 0000 00da 0a72 7061 7274 6974 696f  r......rpartitio
+00000640: 6e29 03da 0b6e 616d 655f 736f 6c76 6572  n)...name_solver
+00000650: da0a 656e 7472 7970 6f69 6e74 7213 0000  ..entrypointr...
+00000660: 0072 1500 0000 7215 0000 0072 1600 0000  .r....r....r....
+00000670: da12 6765 745f 736f 6c76 6572 5f70 6163  ..get_solver_pac
+00000680: 6b61 6765 3c00 0000 7312 0000 000a 0e02  kage<...s.......
+00000690: 010a 020c 010a 0102 ff08 0204 010e 0272  ...............r
+000006a0: 1f00 0000 6301 0000 0000 0000 0000 0000  ....c...........
+000006b0: 0004 0000 0005 0000 0043 0000 0073 5e00  .........C...s^.
+000006c0: 0000 7c00 6401 1b00 7d01 7c01 a000 a100  ..|.d...}.|.....
+000006d0: 730c 7c00 6402 1b00 7d01 7c01 a000 a100  s.|.d...}.|.....
+000006e0: 721a 7401 7c01 6403 8d01 7d02 7c02 6a02  r.t.|.d...}.|.j.
+000006f0: 7d03 7c03 5300 7403 a004 6404 7c01 9b00  }.|.S.t...d.|...
+00000700: 6405 9d03 a101 0100 7c00 a005 a100 6a06  d.......|.....j.
+00000710: a007 6406 a101 6407 1900 7d03 7c03 5300  ..d...d...}.|.S.
+00000720: 2908 7ae6 4465 7465 6374 7320 7368 6f72  ).z.Detects shor
+00000730: 7420 6e61 6d65 206f 6620 7468 6520 736f  t name of the so
+00000740: 6c76 6572 2066 726f 6d20 6060 696e 666f  lver from ``info
+00000750: 5f73 6f6c 7665 722e 786d 6c60 6020 6966  _solver.xml`` if
+00000760: 2070 7265 7365 6e74 206f 720a 2020 2020   present or.    
+00000770: 7468 6520 7061 7468 2e0a 0a20 2020 2050  the path...    P
+00000780: 6172 616d 6574 6572 730a 2020 2020 2d2d  arameters.    --
+00000790: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2070 6174  --------.    pat
+000007a0: 685f 6469 723a 2070 6174 682d 6c69 6b65  h_dir: path-like
+000007b0: 0a20 2020 2020 2020 2050 6174 6820 746f  .        Path to
+000007c0: 2061 2073 696d 756c 6174 696f 6e20 6469   a simulation di
+000007d0: 7265 6374 6f72 790a 0a20 2020 2052 6574  rectory..    Ret
+000007e0: 7572 6e73 0a20 2020 202d 2d2d 2d2d 2d2d  urns.    -------
+000007f0: 0a20 2020 2073 686f 7274 5f6e 616d 653a  .    short_name:
+00000800: 2073 7472 0a0a 2020 2020 7a0f 696e 666f   str..    z.info
+00000810: 5f73 6f6c 7665 722e 786d 6c7a 1e2e 6461  _solver.xmlz..da
+00000820: 7461 5f66 6c75 6964 7369 6d2f 696e 666f  ta_fluidsim/info
+00000830: 5f73 6f6c 7665 722e 786d 6c29 01da 0970  _solver.xml)...p
+00000840: 6174 685f 6669 6c65 7a04 5468 6520 7a45  ath_filez.The zE
+00000850: 2066 696c 6520 6973 206d 6973 7369 6e67   file is missing
+00000860: 2120 4174 7465 6d70 7469 6e67 2074 6f20  ! Attempting to 
+00000870: 6775 6573 7320 736f 6c76 6572 2066 726f  guess solver fro
+00000880: 6d20 7468 6520 6469 7265 6374 6f72 7920  m the directory 
+00000890: 6e61 6d65 2eda 015f 7201 0000 0029 08da  name..._r....)..
+000008a0: 0665 7869 7374 7372 0600 0000 da0a 7368  .existsr......sh
+000008b0: 6f72 745f 6e61 6d65 7208 0000 00da 0777  ort_namer......w
+000008c0: 6172 6e69 6e67 da08 6162 736f 6c75 7465  arning..absolute
+000008d0: da04 6e61 6d65 da05 7370 6c69 7429 04da  ..name..split)..
+000008e0: 0870 6174 685f 6469 725a 0f69 6e66 6f5f  .path_dirZ.info_
+000008f0: 736f 6c76 6572 5f78 6d6c da0b 696e 666f  solver_xml..info
+00000900: 5f73 6f6c 7665 7272 2300 0000 7215 0000  _solverr#...r...
+00000910: 0072 1500 0000 7216 0000 00da 1567 6574  .r....r......get
+00000920: 5f73 6f6c 7665 725f 7368 6f72 745f 6e61  _solver_short_na
+00000930: 6d65 5600 0000 7318 0000 0008 0e08 0108  meV...s.........
+00000940: 0108 020a 0106 0104 0804 fa0a 0104 ff14  ................
+00000950: 0404 0272 2a00 0000 2913 da07 5f5f 646f  ...r*...)...__do
+00000960: 635f 5f72 0b00 0000 da09 6675 6e63 746f  c__r......functo
+00000970: 6f6c 7372 0200 0000 da07 706b 6775 7469  olsr......pkguti
+00000980: 6c72 0300 0000 da05 7479 7065 7372 0400  lr......typesr..
+00000990: 0000 5a0d 666c 7569 6473 696d 5f63 6f72  ..Z.fluidsim_cor
+000009a0: 6572 0500 0000 5a12 666c 7569 6473 696d  er....Z.fluidsim
+000009b0: 5f63 6f72 652e 696e 666f 7206 0000 00da  _core.infor.....
+000009c0: 036c 6f67 7208 0000 0072 1900 0000 da10  .logr....r......
+000009d0: 696d 706f 7274 5f63 6c73 5f73 696d 756c  import_cls_simul
+000009e0: 7217 0000 0072 1f00 0000 722a 0000 0072  r....r....r*...r
+000009f0: 1500 0000 7215 0000 0072 1500 0000 7216  ....r....r....r.
+00000a00: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
+00000a10: 0073 2600 0000 0400 080a 0c01 0c01 0c01  .s&.............
+00000a20: 0c02 0c01 0c02 0202 0601 06ff 0603 0204  ................
+00000a30: 0601 06ff 0603 0803 081a 0c1a            ............
```

### Comparing `fluidsimfoam-0.0.5/src/fluidsimfoam/solvers/__pycache__/base.cpython-310.pyc` & `fluidsimfoam-0.0.6/src/fluidsimfoam/solvers/__pycache__/base.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu May 11 08:22:27 2023 UTC, .py size: 2908 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 c3a5 5c64 5c0b 0000  o.........\d\...
+00000000: 6f0d 0d0a 0000 0000 fc61 6e64 630b 0000  o........andc...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 7000 0000 6400  .....@...sp...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 6d03 5a03 0100 6401  d.l.m.Z.m.Z...d.
 00000050: 6404 6c05 6d06 5a06 0100 6401 6405 6c07  d.l.m.Z...d.d.l.
 00000060: 6d08 5a08 0100 6401 6406 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
 00000070: 0100 6401 6407 6c0b 6d0c 5a0c 0100 6401  ..d.d.l.m.Z...d.
@@ -24,150 +24,149 @@
 00000170: 0c64 0a64 0b84 015a 0987 0004 005a 0a53  .d.d...Z.....Z.S
 00000180: 0029 0dda 0953 696d 756c 466f 616d 7a1e  .)...SimulFoamz.
 00000190: 4261 7365 204f 7065 6e46 4f41 4d20 466c  Base OpenFOAM Fl
 000001a0: 7569 6473 696d 2073 6f6c 7665 722e 6302  uidsim solver.c.
 000001b0: 0000 0000 0000 0000 0000 0002 0000 0001  ................
 000001c0: 0000 0043 0000 0073 0400 0000 6400 5300  ...C...s....d.S.
 000001d0: a901 4ea9 00a9 02da 0363 6c73 da06 7061  ..N......cls..pa
-000001e0: 7261 6d73 720c 0000 0072 0c00 0000 fa47  ramsr....r.....G
-000001f0: 2f68 6f6d 652f 7573 6572 732f 6175 6769  /home/users/augi
-00000200: 6572 3370 692f 4465 762f 666c 7569 6473  er3pi/Dev/fluids
-00000210: 696d 666f 616d 2f73 7263 2f66 6c75 6964  imfoam/src/fluid
-00000220: 7369 6d66 6f61 6d2f 736f 6c76 6572 732f  simfoam/solvers/
-00000230: 6261 7365 2e70 79da 1d5f 636f 6d70 6c65  base.py.._comple
-00000240: 7465 5f70 6172 616d 735f 7769 7468 5f64  te_params_with_d
-00000250: 6566 6175 6c74 1300 0000 7302 0000 0004  efault....s.....
-00000260: 027a 2753 696d 756c 466f 616d 2e5f 636f  .z'SimulFoam._co
-00000270: 6d70 6c65 7465 5f70 6172 616d 735f 7769  mplete_params_wi
-00000280: 7468 5f64 6566 6175 6c74 6301 0000 0000  th_defaultc.....
-00000290: 0000 0000 0000 0002 0000 0002 0000 0003  ................
-000002a0: 0000 0073 0e00 0000 7400 8300 a001 a100  ...s....t.......
-000002b0: 7d01 7c01 5300 720b 0000 0029 02da 0573  }.|.S.r....)...s
-000002c0: 7570 6572 da15 6372 6561 7465 5f64 6566  uper..create_def
-000002d0: 6175 6c74 5f70 6172 616d 7372 0d00 0000  ault_paramsr....
-000002e0: a901 da09 5f5f 636c 6173 735f 5f72 0c00  ....__class__r..
-000002f0: 0000 7210 0000 0072 1300 0000 1700 0000  ..r....r........
-00000300: 7304 0000 000a 0304 017a 1f53 696d 756c  s........z.Simul
-00000310: 466f 616d 2e63 7265 6174 655f 6465 6661  Foam.create_defa
-00000320: 756c 745f 7061 7261 6d73 6302 0000 0000  ult_paramsc.....
-00000330: 0000 0000 0000 0006 0000 0008 0000 0003  ................
-00000340: 0000 0073 e200 0000 7400 8300 a001 7c01  ...s....t.....|.
-00000350: a101 0100 6401 a002 6402 7403 7c00 8301  ....d...d.t.|...
-00000360: a102 7c00 5f04 7c00 6a05 a006 a100 7d02  ..|._.|.j.....}.
-00000370: 7c02 a007 a100 4400 5d25 5c02 7d03 7d04  |.....D.]%\.}.}.
-00000380: 7408 7c00 7c04 8302 7222 7118 7409 7c03  t.|.|...r"q.t.|.
-00000390: 8301 7d05 740a 7c00 7c05 7c04 7c00 8301  ..}.t.|.|.|.|...
-000003a0: 8303 0100 7c00 0400 6a04 6401 a002 6403  ....|...j.d...d.
-000003b0: 7c05 9b00 6404 9d03 7c04 a102 3700 0200  |...d...|...7...
-000003c0: 5f04 7118 6405 7c02 7600 725d 7c01 6a0b  _.q.d.|.v.r]|.j.
-000003d0: 7350 740c 7c01 6a0d 8301 0400 7c00 5f0d  sPt.|.j.....|._.
-000003e0: 7c00 6a0e 5f0d 6e07 740c 7c00 6a0e 6a0d  |.j._.n.t.|.j.j.
-000003f0: 8301 7c00 5f0d 7c00 6a0e a00f a100 0100  ..|._.|.j.......
-00000400: 6e0d 6400 7c00 5f0d 7410 6a11 6406 6b02  n.d.|._.t.j.d.k.
-00000410: 726a 7412 a013 6407 a101 0100 7c00 6a0e  rjt...d.....|.j.
-00000420: 6a14 7c00 5f14 6400 5300 2908 4e7a 097b  j.|._.d.S.).Nz.{
-00000430: 3a32 3873 7d7b 7d0a 7a05 7369 6d3a 207a  :28s}{}.z.sim: z
-00000440: 0473 696d 2e7a 023a 20da 064f 7574 7075  .sim.z.: ..Outpu
-00000450: 7472 0100 0000 7a1c 4e6f 206f 7574 7075  tr....z.No outpu
-00000460: 7420 636c 6173 7320 696e 6974 6961 6c69  t class initiali
-00000470: 7a65 6421 2915 7212 0000 00da 085f 5f69  zed!).r......__i
-00000480: 6e69 745f 5fda 0666 6f72 6d61 74da 0474  nit__..format..t
-00000490: 7970 655a 115f 6f62 6a65 6374 735f 746f  ypeZ._objects_to
-000004a0: 5f70 7269 6e74 da0b 696e 666f 5f73 6f6c  _print..info_sol
-000004b0: 7665 72da 0e69 6d70 6f72 745f 636c 6173  ver..import_clas
-000004c0: 7365 73da 0569 7465 6d73 da0a 6973 696e  ses..items..isin
-000004d0: 7374 616e 6365 7205 0000 00da 0773 6574  stancer......set
-000004e0: 6174 7472 da0f 4e45 575f 4449 525f 5245  attr..NEW_DIR_RE
-000004f0: 5355 4c54 5372 0200 0000 da08 7061 7468  SULTSr......path
-00000500: 5f72 756e da06 6f75 7470 7574 da09 706f  _run..output..po
-00000510: 7374 5f69 6e69 7472 0600 0000 da04 7261  st_initr......ra
-00000520: 6e6b 7208 0000 00da 0777 6172 6e69 6e67  nkr......warning
-00000530: da0b 696e 7075 745f 6669 6c65 7329 06da  ..input_files)..
-00000540: 0473 656c 6672 0f00 0000 da0c 6469 6374  .selfr......dict
-00000550: 5f63 6c61 7373 6573 da08 636c 735f 6e61  _classes..cls_na
-00000560: 6d65 da05 436c 6173 73da 086f 626a 5f6e  me..Class..obj_n
-00000570: 616d 6572 1400 0000 720c 0000 0072 1000  amer....r....r..
-00000580: 0000 7217 0000 001d 0000 0073 2800 0000  ..r........s(...
-00000590: 0c01 1202 0a01 1003 0a02 0201 0802 1001  ................
-000005a0: 0a01 0c01 0aff 0804 0601 1601 0e04 0c02  ................
-000005b0: 0602 0a01 0a01 0e02 7a12 5369 6d75 6c46  ........z.SimulF
-000005c0: 6f61 6d2e 5f5f 696e 6974 5f5f da08 7772  oam.__init__..wr
-000005d0: 6974 654e 6f77 5463 0300 0000 0000 0000  iteNowTc........
-000005e0: 0000 0000 0700 0000 0600 0000 4300 0000  ............C...
-000005f0: 73ca 0000 007c 0272 0974 0064 0183 0101  s....|.r.t.d....
-00000600: 0074 0183 007d 037c 006a 026a 03a0 04a1  .t...}.|.j.j....
-00000610: 007d 047c 017c 0464 023c 007c 04a0 05a1  .}.|.|.d.<.|....
-00000620: 0001 007c 006a 066a 077d 057c 0564 0075  ...|.j.j.}.|.d.u
-00000630: 0072 2164 0053 007c 05a0 08a1 0064 0075  .r!d.S.|.....d.u
-00000640: 0072 507c 006a 0964 031b 00a0 0aa1 0001  .rP|.j.d........
-00000650: 0074 0b64 0483 0101 007c 0272 4a74 0c64  .t.d.....|.rJt.d
-00000660: 0564 0684 007c 006a 09a0 0d64 07a1 0144  .d...|.j...d...D
-00000670: 0083 0183 017d 0674 0064 087c 069b 009d  .....}.t.d.|....
-00000680: 0264 0964 0a8d 0201 007c 05a0 08a1 0064  .d.d.....|.....d
-00000690: 0075 0073 277c 0272 6374 0064 0b74 0183  .u.s'|.rct.d.t..
-000006a0: 007c 0318 0064 0c9b 0464 0d7c 019b 0064  .|...d...d.|...d
-000006b0: 0e9d 0583 0101 0064 0053 0064 0053 0029  .......d.S.d.S.)
-000006c0: 0f4e 7a38 5465 6c6c 696e 6720 4f70 656e  .Nz8Telling Open
-000006d0: 464f 414d 2074 6f20 7374 6f70 2e2e 2e20  FOAM to stop... 
-000006e0: 286f 7665 7277 7269 7465 2063 6f6e 7472  (overwrite contr
-000006f0: 6f6c 4469 6374 2066 696c 6529 da06 7374  olDict file)..st
-00000700: 6f70 4174 7a12 7379 7374 656d 2f63 6f6e  opAtz.system/con
-00000710: 7472 6f6c 4469 6374 679a 9999 9999 99a9  trolDictg.......
-00000720: 3f63 0100 0000 0000 0000 0000 0000 0200  ?c..............
-00000730: 0000 0300 0000 7300 0000 7324 0000 0081  ......s...s$....
-00000740: 007c 005d 0d7d 017c 016a 0064 0019 00a0  .|.].}.|.j.d....
-00000750: 01a1 0072 027c 016a 0056 0001 0071 0264  ...r.|.j.V...q.d
-00000760: 0153 0029 0272 0100 0000 4e29 02da 046e  .S.).r....N)...n
-00000770: 616d 65da 0769 7364 6967 6974 2902 da02  ame..isdigit)...
-00000780: 2e30 da04 7061 7468 720c 0000 0072 0c00  .0..pathr....r..
-00000790: 0000 7210 0000 00da 093c 6765 6e65 7870  ..r......<genexp
-000007a0: 723e 5100 0000 730e 0000 0002 8004 0002  r>Q...s.........
-000007b0: 020c 0102 fd04 010a ff7a 2b53 696d 756c  .........z+Simul
-000007c0: 466f 616d 2e73 746f 705f 7469 6d65 5f6c  Foam.stop_time_l
-000007d0: 6f6f 702e 3c6c 6f63 616c 733e 2e3c 6765  oop.<locals>.<ge
-000007e0: 6e65 7870 723e da01 2a7a 0d0d 7361 7665  nexpr>..*z..save
-000007f0: 6420 7469 6d65 7320 da00 2901 da03 656e  d times ..)...en
-00000800: 647a 140a 5369 6d75 6c61 7469 6f6e 2073  dz..Simulation s
-00000810: 746f 7070 6564 207a 032e 3266 7a13 2073  topped z..2fz. s
-00000820: 2061 6674 6572 2060 7374 6f70 4174 203d   after `stopAt =
-00000830: 20fa 0160 290e da05 7072 696e 7472 0400   ..`)...printr..
-00000840: 0000 7225 0000 00da 0c63 6f6e 7472 6f6c  ..r%.....control
-00000850: 5f64 6963 74da 0472 6561 64da 096f 7665  _dict..read..ove
-00000860: 7277 7269 7465 da04 6d61 6b65 da07 7072  rwrite..make..pr
-00000870: 6f63 6573 73da 0470 6f6c 6c72 2000 0000  ocess..pollr ...
-00000880: da05 746f 7563 6872 0300 0000 da06 736f  ..touchr......so
-00000890: 7274 6564 da04 676c 6f62 2907 7226 0000  rted..glob).r&..
-000008a0: 00da 0773 746f 705f 6174 da07 7665 7262  ...stop_at..verb
-000008b0: 6f73 655a 0674 5f73 746f 705a 0863 7472  oseZ.t_stopZ.ctr
-000008c0: 5f64 6963 7472 3b00 0000 5a11 7361 7665  _dictr;...Z.save
-000008d0: 645f 6469 7265 6374 6f72 6965 7372 0c00  d_directoriesr..
-000008e0: 0000 720c 0000 0072 1000 0000 da0e 7374  ..r....r......st
-000008f0: 6f70 5f74 696d 655f 6c6f 6f70 3f00 0000  op_time_loop?...
-00000900: 7332 0000 0004 0108 0106 010c 0108 0108  s2..............
-00000910: 0108 0208 0204 010c 020e 0208 0104 0108  ................
-00000920: 010a 0208 fe12 050c f604 0c02 0110 0102  ................
-00000930: 0106 ff08 ff04 ff7a 1853 696d 756c 466f  .......z.SimulFo
-00000940: 616d 2e73 746f 705f 7469 6d65 5f6c 6f6f  am.stop_time_loo
-00000950: 7029 0272 2b00 0000 5429 0bda 085f 5f6e  p).r+...T)...__n
-00000960: 616d 655f 5fda 0a5f 5f6d 6f64 756c 655f  ame__..__module_
-00000970: 5fda 0c5f 5f71 7561 6c6e 616d 655f 5fda  _..__qualname__.
-00000980: 075f 5f64 6f63 5f5f 7209 0000 00da 0b63  .__doc__r......c
-00000990: 6c61 7373 6d65 7468 6f64 7211 0000 0072  lassmethodr....r
-000009a0: 1300 0000 7217 0000 0072 4200 0000 da0d  ....r....rB.....
-000009b0: 5f5f 636c 6173 7363 656c 6c5f 5f72 0c00  __classcell__r..
-000009c0: 0000 720c 0000 0072 1400 0000 7210 0000  ..r....r....r...
-000009d0: 0072 0a00 0000 0e00 0000 7312 0000 0008  .r........s.....
-000009e0: 0004 0104 0202 020a 0102 030e 010c 0512  ................
-000009f0: 2272 0a00 0000 4e29 1072 4600 0000 da07  "r....N).rF.....
-00000a00: 7061 7468 6c69 6272 0200 0000 7204 0000  pathlibr....r...
-00000a10: 0072 0300 0000 da0a 696e 666c 6563 7469  .r......inflecti
-00000a20: 6f6e 7205 0000 005a 0d66 6c75 6964 6479  onr....Z.fluiddy
-00000a30: 6e2e 7574 696c 7206 0000 005a 1466 6c75  n.utilr....Z.flu
-00000a40: 6964 7369 6d5f 636f 7265 2e73 6f6c 7665  idsim_core.solve
-00000a50: 7272 0700 0000 5a10 666c 7569 6473 696d  rr....Z.fluidsim
-00000a60: 666f 616d 2e6c 6f67 7208 0000 00da 1366  foam.logr......f
-00000a70: 6c75 6964 7369 6d66 6f61 6d2e 7061 7261  luidsimfoam.para
-00000a80: 6d73 7209 0000 0072 0a00 0000 720c 0000  msr....r....r...
-00000a90: 0072 0c00 0000 720c 0000 0072 1000 0000  .r....r....r....
-00000aa0: da08 3c6d 6f64 756c 653e 0100 0000 7312  ..<module>....s.
-00000ab0: 0000 0004 000c 0210 010c 020c 020c 010c  ................
-00000ac0: 010c 0114 03                             .....
+000001e0: 7261 6d73 720c 0000 0072 0c00 0000 fa3e  ramsr....r.....>
+000001f0: 2f68 6f6d 652f 7069 6572 7265 2f44 6576  /home/pierre/Dev
+00000200: 2f66 6c75 6964 7369 6d66 6f61 6d2f 7372  /fluidsimfoam/sr
+00000210: 632f 666c 7569 6473 696d 666f 616d 2f73  c/fluidsimfoam/s
+00000220: 6f6c 7665 7273 2f62 6173 652e 7079 da1d  olvers/base.py..
+00000230: 5f63 6f6d 706c 6574 655f 7061 7261 6d73  _complete_params
+00000240: 5f77 6974 685f 6465 6661 756c 7413 0000  _with_default...
+00000250: 0073 0200 0000 0402 7a27 5369 6d75 6c46  .s......z'SimulF
+00000260: 6f61 6d2e 5f63 6f6d 706c 6574 655f 7061  oam._complete_pa
+00000270: 7261 6d73 5f77 6974 685f 6465 6661 756c  rams_with_defaul
+00000280: 7463 0100 0000 0000 0000 0000 0000 0200  tc..............
+00000290: 0000 0200 0000 0300 0000 730e 0000 0074  ..........s....t
+000002a0: 0083 00a0 01a1 007d 017c 0153 0072 0b00  .......}.|.S.r..
+000002b0: 0000 2902 da05 7375 7065 72da 1563 7265  ..)...super..cre
+000002c0: 6174 655f 6465 6661 756c 745f 7061 7261  ate_default_para
+000002d0: 6d73 720d 0000 00a9 01da 095f 5f63 6c61  msr........__cla
+000002e0: 7373 5f5f 720c 0000 0072 1000 0000 7213  ss__r....r....r.
+000002f0: 0000 0017 0000 0073 0400 0000 0a03 0401  .......s........
+00000300: 7a1f 5369 6d75 6c46 6f61 6d2e 6372 6561  z.SimulFoam.crea
+00000310: 7465 5f64 6566 6175 6c74 5f70 6172 616d  te_default_param
+00000320: 7363 0200 0000 0000 0000 0000 0000 0600  sc..............
+00000330: 0000 0800 0000 0300 0000 73e2 0000 0074  ..........s....t
+00000340: 0083 00a0 017c 01a1 0101 0064 01a0 0264  .....|.....d...d
+00000350: 0274 037c 0083 01a1 027c 005f 047c 006a  .t.|.....|._.|.j
+00000360: 05a0 06a1 007d 027c 02a0 07a1 0044 005d  .....}.|.....D.]
+00000370: 255c 027d 037d 0474 087c 007c 0483 0272  %\.}.}.t.|.|...r
+00000380: 2271 1874 097c 0383 017d 0574 0a7c 007c  "q.t.|...}.t.|.|
+00000390: 057c 047c 0083 0183 0301 007c 0004 006a  .|.|.......|...j
+000003a0: 0464 01a0 0264 037c 059b 0064 049d 037c  .d...d.|...d...|
+000003b0: 04a1 0237 0002 005f 0471 1864 057c 0276  ...7..._.q.d.|.v
+000003c0: 0072 5d7c 016a 0b73 5074 0c7c 016a 0d83  .r]|.j.sPt.|.j..
+000003d0: 0104 007c 005f 0d7c 006a 0e5f 0d6e 0774  ...|._.|.j._.n.t
+000003e0: 0c7c 006a 0e6a 0d83 017c 005f 0d7c 006a  .|.j.j...|._.|.j
+000003f0: 0ea0 0fa1 0001 006e 0d64 007c 005f 0d74  .......n.d.|._.t
+00000400: 106a 1164 066b 0272 6a74 12a0 1364 07a1  .j.d.k.rjt...d..
+00000410: 0101 007c 006a 0e6a 147c 005f 1464 0053  ...|.j.j.|._.d.S
+00000420: 0029 084e 7a09 7b3a 3238 737d 7b7d 0a7a  .).Nz.{:28s}{}.z
+00000430: 0573 696d 3a20 7a04 7369 6d2e 7a02 3a20  .sim: z.sim.z.: 
+00000440: da06 4f75 7470 7574 7201 0000 007a 1c4e  ..Outputr....z.N
+00000450: 6f20 6f75 7470 7574 2063 6c61 7373 2069  o output class i
+00000460: 6e69 7469 616c 697a 6564 2129 1572 1200  nitialized!).r..
+00000470: 0000 da08 5f5f 696e 6974 5f5f da06 666f  ....__init__..fo
+00000480: 726d 6174 da04 7479 7065 5a11 5f6f 626a  rmat..typeZ._obj
+00000490: 6563 7473 5f74 6f5f 7072 696e 74da 0b69  ects_to_print..i
+000004a0: 6e66 6f5f 736f 6c76 6572 da0e 696d 706f  nfo_solver..impo
+000004b0: 7274 5f63 6c61 7373 6573 da05 6974 656d  rt_classes..item
+000004c0: 73da 0a69 7369 6e73 7461 6e63 6572 0500  s..isinstancer..
+000004d0: 0000 da07 7365 7461 7474 72da 0f4e 4557  ....setattr..NEW
+000004e0: 5f44 4952 5f52 4553 554c 5453 7202 0000  _DIR_RESULTSr...
+000004f0: 00da 0870 6174 685f 7275 6eda 066f 7574  ...path_run..out
+00000500: 7075 74da 0970 6f73 745f 696e 6974 7206  put..post_initr.
+00000510: 0000 00da 0472 616e 6b72 0800 0000 da07  .....rankr......
+00000520: 7761 726e 696e 67da 0b69 6e70 7574 5f66  warning..input_f
+00000530: 696c 6573 2906 da04 7365 6c66 720f 0000  iles)...selfr...
+00000540: 00da 0c64 6963 745f 636c 6173 7365 73da  ...dict_classes.
+00000550: 0863 6c73 5f6e 616d 65da 0543 6c61 7373  .cls_name..Class
+00000560: da08 6f62 6a5f 6e61 6d65 7214 0000 0072  ..obj_namer....r
+00000570: 0c00 0000 7210 0000 0072 1700 0000 1d00  ....r....r......
+00000580: 0000 7328 0000 000c 0112 020a 0110 030a  ..s(............
+00000590: 0202 0108 0210 010a 010c 010a ff08 0406  ................
+000005a0: 0116 010e 040c 0206 020a 010a 010e 027a  ...............z
+000005b0: 1253 696d 756c 466f 616d 2e5f 5f69 6e69  .SimulFoam.__ini
+000005c0: 745f 5fda 0877 7269 7465 4e6f 7754 6303  t__..writeNowTc.
+000005d0: 0000 0000 0000 0000 0000 0007 0000 0006  ................
+000005e0: 0000 0043 0000 0073 ca00 0000 7c02 7209  ...C...s....|.r.
+000005f0: 7400 6401 8301 0100 7401 8300 7d03 7c00  t.d.....t...}.|.
+00000600: 6a02 6a03 a004 a100 7d04 7c01 7c04 6402  j.j.....}.|.|.d.
+00000610: 3c00 7c04 a005 a100 0100 7c00 6a06 6a07  <.|.......|.j.j.
+00000620: 7d05 7c05 6400 7500 7221 6400 5300 7c05  }.|.d.u.r!d.S.|.
+00000630: a008 a100 6400 7500 7250 7c00 6a09 6403  ....d.u.rP|.j.d.
+00000640: 1b00 a00a a100 0100 740b 6404 8301 0100  ........t.d.....
+00000650: 7c02 724a 740c 6405 6406 8400 7c00 6a09  |.rJt.d.d...|.j.
+00000660: a00d 6407 a101 4400 8301 8301 7d06 7400  ..d...D.....}.t.
+00000670: 6408 7c06 9b00 9d02 6409 640a 8d02 0100  d.|.....d.d.....
+00000680: 7c05 a008 a100 6400 7500 7327 7c02 7263  |.....d.u.s'|.rc
+00000690: 7400 640b 7401 8300 7c03 1800 640c 9b04  t.d.t...|...d...
+000006a0: 640d 7c01 9b00 640e 9d05 8301 0100 6400  d.|...d.......d.
+000006b0: 5300 6400 5300 290f 4e7a 3854 656c 6c69  S.d.S.).Nz8Telli
+000006c0: 6e67 204f 7065 6e46 4f41 4d20 746f 2073  ng OpenFOAM to s
+000006d0: 746f 702e 2e2e 2028 6f76 6572 7772 6974  top... (overwrit
+000006e0: 6520 636f 6e74 726f 6c44 6963 7420 6669  e controlDict fi
+000006f0: 6c65 295a 0673 746f 7041 747a 1273 7973  le)Z.stopAtz.sys
+00000700: 7465 6d2f 636f 6e74 726f 6c44 6963 7467  tem/controlDictg
+00000710: 9a99 9999 9999 a93f 6301 0000 0000 0000  .......?c.......
+00000720: 0000 0000 0002 0000 0003 0000 0073 0000  .............s..
+00000730: 0073 2400 0000 8100 7c00 5d0d 7d01 7c01  .s$.....|.].}.|.
+00000740: 6a00 6400 1900 a001 a100 7202 7c01 6a00  j.d.......r.|.j.
+00000750: 5600 0100 7102 6401 5300 2902 7201 0000  V...q.d.S.).r...
+00000760: 004e 2902 da04 6e61 6d65 da07 6973 6469  .N)...name..isdi
+00000770: 6769 7429 02da 022e 30da 0470 6174 6872  git)....0..pathr
+00000780: 0c00 0000 720c 0000 0072 1000 0000 da09  ....r....r......
+00000790: 3c67 656e 6578 7072 3e51 0000 0073 0e00  <genexpr>Q...s..
+000007a0: 0000 0280 0400 0202 0c01 02fd 0401 0aff  ................
+000007b0: 7a2b 5369 6d75 6c46 6f61 6d2e 7374 6f70  z+SimulFoam.stop
+000007c0: 5f74 696d 655f 6c6f 6f70 2e3c 6c6f 6361  _time_loop.<loca
+000007d0: 6c73 3e2e 3c67 656e 6578 7072 3eda 012a  ls>.<genexpr>..*
+000007e0: 7a0d 0d73 6176 6564 2074 696d 6573 20da  z..saved times .
+000007f0: 0029 01da 0365 6e64 7a14 0a53 696d 756c  .)...endz..Simul
+00000800: 6174 696f 6e20 7374 6f70 7065 6420 7a03  ation stopped z.
+00000810: 2e32 667a 1320 7320 6166 7465 7220 6073  .2fz. s after `s
+00000820: 746f 7041 7420 3d20 fa01 6029 0eda 0570  topAt = ..`)...p
+00000830: 7269 6e74 7204 0000 0072 2500 0000 da0c  rintr....r%.....
+00000840: 636f 6e74 726f 6c5f 6469 6374 da04 7265  control_dict..re
+00000850: 6164 da09 6f76 6572 7772 6974 65da 046d  ad..overwrite..m
+00000860: 616b 65da 0770 726f 6365 7373 da04 706f  ake..process..po
+00000870: 6c6c 7220 0000 00da 0574 6f75 6368 7203  llr .....touchr.
+00000880: 0000 00da 0673 6f72 7465 64da 0467 6c6f  .....sorted..glo
+00000890: 6229 0772 2600 0000 da07 7374 6f70 5f61  b).r&.....stop_a
+000008a0: 74da 0776 6572 626f 7365 5a06 745f 7374  t..verboseZ.t_st
+000008b0: 6f70 5a08 6374 725f 6469 6374 723a 0000  opZ.ctr_dictr:..
+000008c0: 005a 1173 6176 6564 5f64 6972 6563 746f  .Z.saved_directo
+000008d0: 7269 6573 720c 0000 0072 0c00 0000 7210  riesr....r....r.
+000008e0: 0000 00da 0e73 746f 705f 7469 6d65 5f6c  .....stop_time_l
+000008f0: 6f6f 703f 0000 0073 3200 0000 0401 0801  oop?...s2.......
+00000900: 0601 0c01 0801 0801 0802 0802 0401 0c02  ................
+00000910: 0e02 0801 0401 0801 0a02 08fe 1205 0cf6  ................
+00000920: 040c 0201 1001 0201 06ff 08ff 04ff 7a18  ..............z.
+00000930: 5369 6d75 6c46 6f61 6d2e 7374 6f70 5f74  SimulFoam.stop_t
+00000940: 696d 655f 6c6f 6f70 2902 722b 0000 0054  ime_loop).r+...T
+00000950: 290b da08 5f5f 6e61 6d65 5f5f da0a 5f5f  )...__name__..__
+00000960: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
+00000970: 6e61 6d65 5f5f da07 5f5f 646f 635f 5f72  name__..__doc__r
+00000980: 0900 0000 da0b 636c 6173 736d 6574 686f  ......classmetho
+00000990: 6472 1100 0000 7213 0000 0072 1700 0000  dr....r....r....
+000009a0: 7241 0000 00da 0d5f 5f63 6c61 7373 6365  rA.....__classce
+000009b0: 6c6c 5f5f 720c 0000 0072 0c00 0000 7214  ll__r....r....r.
+000009c0: 0000 0072 1000 0000 720a 0000 000e 0000  ...r....r.......
+000009d0: 0073 1200 0000 0800 0401 0402 0202 0a01  .s..............
+000009e0: 0203 0e01 0c05 1222 720a 0000 004e 2910  ......."r....N).
+000009f0: 7245 0000 00da 0770 6174 686c 6962 7202  rE.....pathlibr.
+00000a00: 0000 0072 0400 0000 7203 0000 005a 0a69  ...r....r....Z.i
+00000a10: 6e66 6c65 6374 696f 6e72 0500 0000 5a0d  nflectionr....Z.
+00000a20: 666c 7569 6464 796e 2e75 7469 6c72 0600  fluiddyn.utilr..
+00000a30: 0000 5a14 666c 7569 6473 696d 5f63 6f72  ..Z.fluidsim_cor
+00000a40: 652e 736f 6c76 6572 7207 0000 005a 1066  e.solverr....Z.f
+00000a50: 6c75 6964 7369 6d66 6f61 6d2e 6c6f 6772  luidsimfoam.logr
+00000a60: 0800 0000 da13 666c 7569 6473 696d 666f  ......fluidsimfo
+00000a70: 616d 2e70 6172 616d 7372 0900 0000 720a  am.paramsr....r.
+00000a80: 0000 0072 0c00 0000 720c 0000 0072 0c00  ...r....r....r..
+00000a90: 0000 7210 0000 00da 083c 6d6f 6475 6c65  ..r......<module
+00000aa0: 3e01 0000 0073 1200 0000 0400 0c02 1001  >....s..........
+00000ab0: 0c02 0c02 0c01 0c01 0c01 1403            ............
```

### Comparing `fluidsimfoam-0.0.5/src/fluidsimfoam/solvers/base.py` & `fluidsimfoam-0.0.6/src/fluidsimfoam/solvers/base.py`

 * *Files identical despite different names*

### Comparing `fluidsimfoam-0.0.5/src/fluidsimfoam/tasks.py` & `fluidsimfoam-0.0.6/src/fluidsimfoam/tasks.py`

 * *Files identical despite different names*

### Comparing `fluidsimfoam-0.0.5/src/fluidsimfoam/testing.py` & `fluidsimfoam-0.0.6/src/fluidsimfoam/testing.py`

 * *Files 8% similar despite different names*

```diff
@@ -43,8 +43,10 @@
         text_produced = path_produced.read_text()
 
         if relative_path.name in files_compare_tree:
             tree_saved_file = parse(text_manual)
             tree_from_py = parse(text_produced)
             assert dump(tree_saved_file).strip() == dump(tree_from_py).strip()
         else:
+            if text_produced != text_manual:
+                print(f"meld {path_produced} {path_manual}")
             assert text_produced == text_manual, relative_path
```

### Comparing `fluidsimfoam-0.0.5/src/fluidsimfoam/util/__pycache__/console.cpython-39.pyc` & `fluidsimfoam-0.0.6/src/fluidsimfoam/util/__pycache__/console.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun  1 15:07:01 2023 UTC, .py size: 6404 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 18% similar despite different names*

```diff
@@ -1,328 +1,342 @@
-00000000: 610d 0d0a 0000 0000 15b4 7864 0419 0000  a.........xd....
+00000000: 6f0d 0d0a 0000 0000 c9b7 7964 fa1a 0000  o.........yd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 c000 0000 6400  .....@...s....d.
+00000020: 0004 0000 0040 0000 0073 c800 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
-00000040: 5a02 6401 6402 6c03 5a03 6401 6403 6c04  Z.d.d.l.Z.d.d.l.
-00000050: 6d05 5a05 0100 6401 6404 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
-00000060: 0100 6401 6405 6c08 6d09 5a09 0100 6401  ..d.d.l.m.Z...d.
-00000070: 6406 6c0a 6d0a 5a0a 0100 6401 6407 6c0b  d.l.m.Z...d.d.l.
-00000080: 6d0c 5a0c 0100 6401 6408 6c0d 6d0e 5a0e  m.Z...d.d.l.m.Z.
-00000090: 0100 6401 6409 6c0f 6d10 5a10 0100 6401  ..d.d.l.m.Z...d.
-000000a0: 640a 6c11 6d12 5a13 0100 6401 640b 6c14  d.l.m.Z...d.d.l.
-000000b0: 6d15 5a15 0100 6401 640c 6c16 6d17 5a18  m.Z...d.d.l.m.Z.
-000000c0: 0100 6401 640d 6c19 6d1a 5a1a 0100 640e  ..d.d.l.m.Z...d.
-000000d0: 640f 8400 5a1b 6505 6513 6410 6411 8d02  d...Z.e.e.d.d...
-000000e0: 5a12 6412 6413 8400 5a1c 6402 5300 2914  Z.d.d...Z.d.S.).
-000000f0: 7a1a 436f 6e73 6f6c 6520 7363 7269 7074  z.Console script
-00000100: 2066 756e 6374 696f 6e73 0a0a e900 0000   functions......
-00000110: 004e 2901 da07 7061 7274 6961 6c29 01da  .N)...partial)..
-00000120: 0972 6573 6f75 7263 6573 2901 da04 5061  .resources)...Pa
-00000130: 7468 2901 da06 7070 7269 6e74 2901 da04  th)...pprint)...
-00000140: 636f 7079 2901 da08 5465 6d70 6c61 7465  copy)...Template
-00000150: 2901 da08 6361 6d65 6c69 7a65 2901 da16  )...camelize)...
-00000160: 7374 6172 745f 6970 7974 686f 6e5f 6c6f  start_ipython_lo
-00000170: 6164 5f73 696d 2901 da10 7061 7468 5f64  ad_sim)...path_d
-00000180: 6972 5f72 6573 756c 7473 2901 da0b 5f5f  ir_results)...__
-00000190: 7665 7273 696f 6e5f 5f29 01da 1161 7661  version__)...ava
-000001a0: 696c 6162 6c65 5f73 6f6c 7665 7273 6300  ilable_solversc.
-000001b0: 0000 0000 0000 0000 0000 0009 0000 0005  ................
-000001c0: 0000 0043 0000 0073 9a00 0000 6401 6400  ...C...s....d.d.
-000001d0: 6c00 7d00 6401 6400 6c01 7d01 6401 6400  l.}.d.d.l.}.d.d.
-000001e0: 6c02 7d02 6402 6403 6404 9c02 7d03 7c02  l.}.d.d.d...}.|.
-000001f0: 7c00 7c01 6703 7d04 7c04 4400 5d10 7d05  |.|.g.}.|.D.].}.
-00000200: 7c05 6a03 7c03 7c05 6a04 3c00 7130 7c03  |.j.|.|.j.<.q0|.
-00000210: a005 a100 4400 5d20 5c02 7d06 7d07 7406  ....D.] \.}.}.t.
-00000220: 7c06 a007 6405 a101 9b00 6406 7c07 9b00  |...d.....d.|...
-00000230: 9d03 8301 0100 714a 7408 7409 6407 6408  ......qJt.t.d.d.
-00000240: 8400 740a 8300 4400 8301 8301 8301 7d08  ..t...D.......}.
-00000250: 7406 6409 640a a00b 7c08 a101 1700 8301  t.d.d...|.......
-00000260: 0100 6400 5300 290b 4e72 0100 0000 da07  ..d.S.).Nr......
-00000270: 5665 7273 696f 6efa 072d 2d2d 2d2d 2d2d  Version..-------
-00000280: 2902 da07 5061 636b 6167 6572 0e00 0000  )...Packager....
-00000290: e90f 0000 00fa 0120 6301 0000 0000 0000  ....... c.......
-000002a0: 0000 0000 0002 0000 0003 0000 0053 0000  .............S..
-000002b0: 0073 1200 0000 6700 7c00 5d0a 7d01 7c01  .s....g.|.].}.|.
-000002c0: 6a00 9102 7104 5300 a900 a901 da04 6e61  j...q.S.......na
-000002d0: 6d65 2902 da02 2e30 5a0b 656e 7472 795f  me)....0Z.entry_
-000002e0: 706f 696e 7472 1200 0000 7212 0000 00fa  pointr....r.....
-000002f0: 472f 686f 6d65 2f75 7365 7273 2f61 7567  G/home/users/aug
-00000300: 6965 7233 7069 2f44 6576 2f66 6c75 6964  ier3pi/Dev/fluid
-00000310: 7369 6d66 6f61 6d2f 7372 632f 666c 7569  simfoam/src/flui
-00000320: 6473 696d 666f 616d 2f75 7469 6c2f 636f  dsimfoam/util/co
-00000330: 6e73 6f6c 652e 7079 da0a 3c6c 6973 7463  nsole.py..<listc
-00000340: 6f6d 703e 2700 0000 f300 0000 007a 2270  omp>'........z"p
-00000350: 7269 6e74 5f76 6572 7369 6f6e 732e 3c6c  rint_versions.<l
-00000360: 6f63 616c 733e 2e3c 6c69 7374 636f 6d70  ocals>.<listcomp
-00000370: 3e7a 140a 496e 7374 616c 6c65 6420 736f  >z..Installed so
-00000380: 6c76 6572 733a 207a 022c 2029 0cda 0866  lvers: z., )...f
-00000390: 6c75 6964 6479 6eda 0d66 6c75 6964 7369  luiddyn..fluidsi
-000003a0: 6d5f 636f 7265 da0c 666c 7569 6473 696d  m_core..fluidsim
-000003b0: 666f 616d 720b 0000 00da 085f 5f6e 616d  foamr......__nam
-000003c0: 655f 5fda 0569 7465 6d73 da05 7072 696e  e__..items..prin
-000003d0: 74da 056c 6a75 7374 da06 736f 7274 6564  t..ljust..sorted
-000003e0: da03 7365 7472 0c00 0000 da04 6a6f 696e  ..setr......join
-000003f0: 2909 7219 0000 0072 1a00 0000 721b 0000  ).r....r....r...
-00000400: 005a 0876 6572 7369 6f6e 73da 0870 6163  .Z.versions..pac
-00000410: 6b61 6765 73da 0770 6163 6b61 6765 da08  kages..package..
-00000420: 706b 675f 6e61 6d65 da07 7665 7273 696f  pkg_name..versio
-00000430: 6eda 056e 616d 6573 7212 0000 0072 1200  n..namesr....r..
-00000440: 0000 7216 0000 00da 0e70 7269 6e74 5f76  ..r......print_v
-00000450: 6572 7369 6f6e 7319 0000 0073 1600 0000  ersions....s....
-00000460: 0001 0801 0801 0802 0a02 0a01 0801 0e02  ................
-00000470: 1001 1a02 1801 7228 0000 007a 1d66 726f  ......r(...z.fro
-00000480: 6d20 666c 7569 6473 696d 666f 616d 2069  m fluidsimfoam i
-00000490: 6d70 6f72 7420 6c6f 6164 2901 5a0b 6c6f  mport load).Z.lo
-000004a0: 6164 5f69 6d70 6f72 7463 0000 0000 0000  ad_importc......
-000004b0: 0000 0000 0000 1c00 0000 0c00 0000 0300  ................
-000004c0: 0000 735e 0400 0064 0164 026c 006d 017d  ..s^...d.d.l.m.}
-000004d0: 0001 0074 026a 0364 0364 0464 058d 027d  ...t.j.d.d.d...}
-000004e0: 017c 01a0 0464 06a1 0101 007c 01a0 0464  .|...d.....|...d
-000004f0: 0764 08a1 0201 007c 01a0 0464 0964 0aa1  .d.....|...d.d..
-00000500: 0201 007c 016a 0464 0b64 0c64 0d64 0e8d  ...|.j.d.d.d.d..
-00000510: 0301 007c 01a0 0464 0f64 10a1 0201 007c  ...|...d.d.....|
-00000520: 01a0 05a1 007d 0274 067c 0283 0101 007c  .....}.t.|.....|
-00000530: 026a 0764 0075 0072 8e7c 026a 0864 0075  .j.d.u.r.|.j.d.u
-00000540: 0072 8e74 0664 1183 0101 0074 09a0 0a64  .r.t.d.....t...d
-00000550: 12a1 0101 007c 026a 0864 0075 0172 a074  .....|.j.d.u.r.t
-00000560: 0b64 1383 0182 017c 026a 0764 0075 0172  .d.....|.j.d.u.r
-00000570: d474 0c7c 026a 0783 0189 0088 00a0 0da1  .t.|.j..........
-00000580: 0073 d474 0688 009b 0064 149d 0283 0101  .s.t.....d......
-00000590: 0074 09a0 0a64 12a1 0101 007c 026a 0e64  .t...d.....|.j.d
-000005a0: 0075 0172 ee74 0c7c 026a 0e83 01a0 0fa1  .u.r.t.|.j......
-000005b0: 007d 036e 0474 107d 0364 157c 026a 119b  .}.n.t.}.d.|.j..
-000005c0: 009d 027d 047c 026a 11a0 1264 1664 17a1  ...}.|.j...d.d..
-000005d0: 027d 0564 187c 059b 009d 027d 067c 037c  .}.d.|.....}.|.|
-000005e0: 041b 007d 077c 07a0 0da1 0090 0172 4074  ...}.|.......r@t
-000005f0: 067c 079b 0064 199d 0283 0101 0074 09a0  .|...d.......t..
-00000600: 0a64 12a1 0101 0074 0664 1a7c 079b 009d  .d.....t.d.|....
-00000610: 0283 0101 007c 026a 0764 0075 0190 0172  .....|.j.d.u...r
-00000620: e674 0664 1b88 009b 009d 0283 0101 0069  .t.d...........i
-00000630: 007d 0869 007d 0964 1c44 005d 2a7d 0a74  .}.i.}.d.D.]*}.t
-00000640: 1387 0066 0164 1d64 1e84 0888 00a0 147c  ...f.d.d.......|
-00000650: 0a64 1f17 00a1 0144 0083 0183 017c 087c  .d.....D.....|.|
-00000660: 0a3c 0090 0171 747c 08a0 1564 20a1 017d  .<...qt|...d ..}
-00000670: 0b7c 0b90 0172 b87c 0b7c 0864 213c 007c  .|...r.|.|.d!<.|
-00000680: 08a0 16a1 0044 005d 1c7d 0a64 2264 2384  .....D.].}.d"d#.
-00000690: 007c 087c 0a19 0044 0083 017c 097c 0a3c  .|.|...D...|.|.<
-000006a0: 0090 0171 c074 177c 0983 0101 0074 0664  ...q.t.|.....t.d
-000006b0: 247c 079b 009d 0283 0101 007c 07a0 18a1  $|.........|....
-000006c0: 0001 0074 1974 1a6a 1ba0 1ca1 006a 1d83  ...t.t.j.....j..
-000006d0: 017c 026a 1e7c 026a 117c 047c 0674 1f74  .|.j.|.j.|.|.t.t
-000006e0: 207c 026a 1183 0174 197c 0964 2119 0083   |.j...t.|.d!...
-000006f0: 0174 197c 0964 2519 0083 0174 197c 0964  .t.|.d%....t.|.d
-00000700: 2619 0083 0164 279c 0a7d 0c69 007d 0d64  &....d'..}.i.}.d
-00000710: 2844 005d 167d 0e7c 0e7d 0f7c 0e64 2917  (D.].}.|.}.|.d).
-00000720: 007c 0d7c 0f3c 0090 0271 4c7c 0764 2a7c  .|.|.<...qL|.d*|
-00000730: 069b 009d 021b 007d 1064 2b44 005d 1a7d  .......}.d+D.].}
-00000740: 0e7c 107c 0e1b 007d 0f7c 0e64 2917 007c  .|.|...}.|.d)..|
-00000750: 0d7c 0f3c 0090 0271 767c 1064 2c1b 007d  .|.<...qv|.d,..}
-00000760: 117c 116a 1864 2d64 2e8d 0101 0064 2f7d  .|.j.d-d.....d/}
-00000770: 0e7c 0e64 2917 007c 0d7c 117c 0e1b 003c  .|.d)..|.|.|...<
-00000780: 007c 0764 301b 007d 127c 12a0 18a1 0001  .|.d0..}.|......
-00000790: 0064 317c 0d7c 1264 327c 059b 0064 339d  .d1|.|.d2|...d3.
-000007a0: 031b 003c 007c 0da0 21a1 0044 005d 6a5c  ...<.|..!..D.]j\
-000007b0: 027d 0f7d 1374 22a0 2364 34a1 01a0 247c  .}.}.t".#d4...$|
-000007c0: 13a1 017d 1474 22a0 257c 14a1 018f 187d  ...}.t".%|.....}
-000007d0: 157c 15a0 26a1 007d 1657 0064 0004 0004  .|..&..}.W.d....
-000007e0: 0083 0301 006e 1231 0090 0373 2830 0001  .....n.1...s(0..
-000007f0: 0001 0001 0059 0001 0074 277c 1683 01a0  .....Y...t'|....
-00000800: 287c 0ca1 017d 167c 077c 0f1b 00a0 297c  (|...}.|.|....)|
-00000810: 16a1 0101 0090 0271 e67c 1264 351b 007d  .......q.|.d5..}
-00000820: 177c 176a 1864 2d64 2e8d 0101 007c 08a0  .|.j.d-d.....|..
-00000830: 21a1 0044 005d 9a5c 027d 0a7d 187c 0a64  !..D.].\.}.}.|.d
-00000840: 216b 027d 197c 177c 0a1b 007d 1a7c 1aa0  !k.}.|.|...}.|..
-00000850: 18a1 0001 007c 1844 005d 727d 0f88 007c  .....|.D.]r}...|
-00000860: 0f1b 00a0 26a1 007d 167c 007c 167c 1964  ....&..}.|.|.|.d
-00000870: 368d 027d 167c 0a64 216b 0290 0372 e074  6..}.|.d!k...r.t
-00000880: 2a7c 0f6a 2b83 017d 1b7c 1b64 0119 0064  *|.j+..}.|.d...d
-00000890: 206b 0290 0372 e064 217c 1b64 013c 0074   k...r.d!|.d.<.t
-000008a0: 0c7c 1b8e 007d 0f7c 177c 0f1b 00a0 297c  .|...}.|.|....)|
-000008b0: 16a1 0101 007c 117c 0f6a 1164 3717 001b  .....|.|.j.d7...
-000008c0: 00a0 297c 16a1 0101 0090 0371 9290 0371  ..)|.......q...q
-000008d0: 6e7c 026a 0764 0075 0190 0472 3e64 3844  n|.j.d.u...r>d8D
-000008e0: 005d 227d 0e88 007c 0e1b 007d 157c 15a0  .]"}...|...}.|..
-000008f0: 0da1 0090 0472 1a74 2c7c 157c 1783 0201  .....r.t,|.|....
-00000900: 0090 0471 1a74 0664 397c 049b 0064 3a7c  ...q.t.d9|...d:|
-00000910: 079b 0064 3b7c 069b 0064 3c9d 0783 0101  ...d;|...d<.....
-00000920: 0064 0053 0029 3d4e 7201 0000 0029 01da  .d.S.)=Nr....)..
-00000930: 0b66 6f72 6d61 745f 636f 6465 7a1c 666c  .format_codez.fl
-00000940: 7569 6473 696d 666f 616d 2d69 6e69 7469  uidsimfoam-initi
-00000950: 6174 652d 736f 6c76 6572 7a15 496e 6974  ate-solverz.Init
-00000960: 6961 7465 2061 206e 6577 2073 6f6c 7665  iate a new solve
-00000970: 7229 02da 0470 726f 67da 0b64 6573 6372  r)...prog..descr
-00000980: 6970 7469 6f6e 7214 0000 007a 022d 637a  iptionr....z.-cz
-00000990: 0b2d 2d66 726f 6d2d 6361 7365 7a02 2d73  .--from-casez.-s
-000009a0: 7a0d 2d2d 6672 6f6d 2d73 6f6c 7665 727a  z.--from-solverz
-000009b0: 022d 617a 082d 2d61 7574 686f 727a 1746  .-az.--authorz.F
-000009c0: 6c75 6964 7369 6d66 6f61 6d20 6465 7665  luidsimfoam deve
-000009d0: 6c6f 7065 7273 2901 da07 6465 6661 756c  lopers)...defaul
-000009e0: 747a 022d 647a 0d2d 2d64 6573 7469 6e61  tz.-dz.--destina
-000009f0: 7469 6f6e 7a38 596f 7520 7368 6f75 6c64  tionz8You should
-00000a00: 2061 7420 6c65 6173 7420 7072 6f76 6964   at least provid
-00000a10: 6520 6120 6361 7365 2028 2d63 2920 6f72  e a case (-c) or
-00000a20: 2061 2073 6f6c 7665 7220 282d 7329 e901   a solver (-s)..
-00000a30: 0000 007a 2a53 6f72 7279 2c20 6f70 7469  ...z*Sorry, opti
-00000a40: 6f6e 202d 7320 6973 206e 6f74 2079 6574  on -s is not yet
-00000a50: 2069 6d70 6c65 6d65 6e74 6564 2e2e 2e7a   implemented...z
-00000a60: 1020 646f 6573 206e 6f74 2065 7869 7374  . does not exist
-00000a70: 2e7a 0d66 6c75 6964 7369 6d66 6f61 6d2d  .z.fluidsimfoam-
-00000a80: fa01 2dda 015f 5a0d 666c 7569 6473 696d  ..-.._Z.fluidsim
-00000a90: 666f 616d 5f7a 1020 616c 7265 6164 7920  foam_z. already 
-00000aa0: 6578 6973 7473 2e7a 1a4c 6574 2773 2069  exists.z.Let's i
-00000ab0: 6e69 7469 6174 6520 7468 6520 736f 6c76  nitiate the solv
-00000ac0: 6572 207a 0b55 7369 6e67 2063 6173 6520  er z.Using case 
-00000ad0: 2904 da06 7379 7374 656d da08 636f 6e73  )...system..cons
-00000ae0: 7461 6e74 da01 30fa 0630 2e6f 7269 6763  tant..0..0.origc
-00000af0: 0100 0000 0000 0000 0000 0000 0200 0000  ................
-00000b00: 0400 0000 3300 0000 7320 0000 007c 005d  ....3...s ...|.]
-00000b10: 187d 017c 01a0 00a1 0072 027c 01a0 0188  .}.|.....r.|....
-00000b20: 00a1 0156 0001 0071 0264 0053 0029 014e  ...V...q.d.S.).N
-00000b30: 2902 da07 6973 5f66 696c 65da 0b72 656c  )...is_file..rel
-00000b40: 6174 6976 655f 746f 2902 7215 0000 00da  ative_to).r.....
-00000b50: 0470 6174 68a9 01da 0970 6174 685f 6361  .path....path_ca
-00000b60: 7365 7212 0000 0072 1600 0000 da09 3c67  ser....r......<g
-00000b70: 656e 6578 7072 3e67 0000 0073 0600 0000  enexpr>g...s....
-00000b80: 0402 0202 08fd 7a22 696e 6974 6961 7465  ......z"initiate
-00000b90: 5f73 6f6c 7665 722e 3c6c 6f63 616c 733e  _solver.<locals>
-00000ba0: 2e3c 6765 6e65 7870 723e 7a02 2f2a 7233  .<genexpr>z./*r3
-00000bb0: 0000 0072 3200 0000 6301 0000 0000 0000  ...r2...c.......
-00000bc0: 0000 0000 0002 0000 0003 0000 0053 0000  .............S..
-00000bd0: 0073 1200 0000 6700 7c00 5d0a 7d01 7c01  .s....g.|.].}.|.
-00000be0: 6a00 9102 7104 5300 7212 0000 0072 1300  j...q.S.r....r..
-00000bf0: 0000 2902 7215 0000 00da 0170 7212 0000  ..).r......pr...
-00000c00: 0072 1200 0000 7216 0000 0072 1700 0000  .r....r....r....
-00000c10: 7300 0000 7218 0000 007a 2369 6e69 7469  s...r....z#initi
-00000c20: 6174 655f 736f 6c76 6572 2e3c 6c6f 6361  ate_solver.<loca
-00000c30: 6c73 3e2e 3c6c 6973 7463 6f6d 703e 7a07  ls>.<listcomp>z.
-00000c40: 4d61 6b69 6e67 2072 3000 0000 7231 0000  Making r0...r1..
-00000c50: 0029 0ada 0479 6561 72da 0661 7574 686f  .)...year..autho
-00000c60: 725a 0a6e 616d 655f 7368 6f72 74da 0c6e  rZ.name_short..n
-00000c70: 616d 655f 7072 6f6a 6563 74da 0c6e 616d  ame_project..nam
-00000c80: 655f 7061 636b 6167 65da 1466 6c75 6964  e_package..fluid
-00000c90: 7369 6d66 6f61 6d5f 7665 7273 696f 6e5a  simfoam_versionZ
-00000ca0: 1073 7566 6669 785f 666f 725f 636c 6173  .suffix_for_clas
-00000cb0: 735a 0e6e 616d 655f 7661 7269 6162 6c65  sZ.name_variable
-00000cc0: 735a 116e 616d 655f 7379 7374 656d 5f66  sZ.name_system_f
-00000cd0: 696c 6573 5a13 6e61 6d65 5f63 6f6e 7374  ilesZ.name_const
-00000ce0: 616e 745f 6669 6c65 7329 03da 074c 4943  ant_files)...LIC
-00000cf0: 454e 5345 7a09 5245 4144 4d45 2e6d 647a  ENSEz.README.mdz
-00000d00: 0e70 7970 726f 6a65 6374 2e74 6f6d 6c7a  .pyproject.tomlz
-00000d10: 092e 7465 6d70 6c61 7465 7a04 7372 632f  ..templatez.src/
-00000d20: 2903 7a0b 5f5f 696e 6974 5f5f 2e70 797a  ).z.__init__.pyz
-00000d30: 096f 7574 7075 742e 7079 fa08 7461 736b  .output.py..task
-00000d40: 732e 7079 da09 7465 6d70 6c61 7465 7354  s.py..templatesT
-00000d50: 2901 da07 7061 7265 6e74 7372 4100 0000  )...parentsrA...
-00000d60: da05 7465 7374 737a 2174 6573 745f 6765  ..testsz!test_ge
-00000d70: 6e65 7261 7465 645f 736f 6c76 6572 2e70  nerated_solver.p
-00000d80: 792e 7465 6d70 6c61 7465 5a05 7465 7374  y.templateZ.test
-00000d90: 5f7a 032e 7079 7a16 666c 7569 6473 696d  _z..pyz.fluidsim
-00000da0: 666f 616d 2e72 6573 6f75 7263 6573 7a11  foam.resourcesz.
-00000db0: 7361 7665 645f 6361 7365 732f 6361 7365  saved_cases/case
-00000dc0: 3029 01da 0861 735f 6669 656c 647a 062e  0)...as_fieldz..
-00000dd0: 6a69 6e6a 6129 025a 0841 6c6c 636c 6561  jinja).Z.Allclea
-00000de0: 6e5a 0641 6c6c 7275 6e7a 0d0a 0a4e 6577  nZ.Allrunz...New
-00000df0: 2073 6f6c 7665 7220 7a5f 2063 7265 6174   solver z_ creat
-00000e00: 6564 2120 596f 7520 6361 6e20 6e6f 7720  ed! You can now 
-00000e10: 696e 7374 616c 6c20 616e 6420 7465 7374  install and test
-00000e20: 2069 7420 746f 2063 6865 636b 2069 660a   it to check if.
-00000e30: 6974 2072 6570 726f 6475 6365 7320 796f  it reproduces yo
-00000e40: 7572 2069 6e69 7469 616c 2063 6173 652e  ur initial case.
-00000e50: 0a0a 6060 600a 6364 207a 860a 7069 7020  ..```.cd z..pip 
-00000e60: 696e 7374 616c 6c20 2d65 202e 0a70 7974  install -e ..pyt
-00000e70: 6573 7420 7465 7374 7320 2d76 760a 6060  est tests -vv.``
-00000e80: 600a 0a59 6f75 2063 616e 2074 6865 6e20  `..You can then 
-00000e90: 696d 7072 6f76 6520 796f 7572 2066 6c75  improve your flu
-00000ea0: 6964 7369 6d66 6f61 6d20 736f 6c76 6572  idsimfoam solver
-00000eb0: 2062 7920 6d6f 6469 6679 696e 6720 6974   by modifying it
-00000ec0: 7320 6669 6c65 730a 2865 7370 6563 6961  s files.(especia
-00000ed0: 6c6c 7920 7468 6520 6669 6c65 2073 7263  lly the file src
-00000ee0: 2f7a 7e2f 6f75 7470 7574 2e70 7929 2e20  /z~/output.py). 
-00000ef0: 4578 616d 706c 6573 2063 616e 2062 6520  Examples can be 
-00000f00: 666f 756e 6420 696e 0a68 7474 7073 3a2f  found in.https:/
-00000f10: 2f66 6f73 732e 6865 7074 6170 6f64 2e6e  /foss.heptapod.n
-00000f20: 6574 2f66 6c75 6964 6479 6e2f 666c 7569  et/fluiddyn/flui
-00000f30: 6473 696d 666f 616d 2f2d 2f74 7265 652f  dsimfoam/-/tree/
-00000f40: 6272 616e 6368 2f64 6566 6175 6c74 2f64  branch/default/d
-00000f50: 6f63 2f65 7861 6d70 6c65 730a 0a20 2020  oc/examples..   
-00000f60: 2029 2d5a 1d66 6c75 6964 7369 6d66 6f61   )-Z.fluidsimfoa
-00000f70: 6d2e 666f 616d 5f69 6e70 7574 5f66 696c  m.foam_input_fil
-00000f80: 6573 7229 0000 00da 0861 7267 7061 7273  esr).....argpars
-00000f90: 65da 0e41 7267 756d 656e 7450 6172 7365  e..ArgumentParse
-00000fa0: 72da 0c61 6464 5f61 7267 756d 656e 74da  r..add_argument.
-00000fb0: 0a70 6172 7365 5f61 7267 7372 1e00 0000  .parse_argsr....
-00000fc0: 5a09 6672 6f6d 5f63 6173 655a 0b66 726f  Z.from_caseZ.fro
-00000fd0: 6d5f 736f 6c76 6572 da03 7379 73da 0465  m_solver..sys..e
-00000fe0: 7869 74da 134e 6f74 496d 706c 656d 656e  xit..NotImplemen
-00000ff0: 7465 6445 7272 6f72 7204 0000 00da 0665  tedErrorr......e
-00001000: 7869 7374 73da 0b64 6573 7469 6e61 7469  xists..destinati
-00001010: 6f6e da07 7265 736f 6c76 6572 0a00 0000  on..resolver....
-00001020: 7214 0000 00da 0772 6570 6c61 6365 7220  r......replacer 
-00001030: 0000 00da 0467 6c6f 62da 0370 6f70 da04  .....glob..pop..
-00001040: 6b65 7973 7205 0000 00da 056d 6b64 6972  keysr......mkdir
-00001050: da03 7374 72da 0864 6174 6574 696d 65da  ..str..datetime.
-00001060: 0464 6174 65da 0574 6f64 6179 723b 0000  .date..todayr;..
-00001070: 0072 3c00 0000 723f 0000 0072 0800 0000  .r<...r?...r....
-00001080: 721d 0000 0072 0300 0000 da05 6669 6c65  r....r......file
-00001090: 73da 086a 6f69 6e70 6174 685a 0761 735f  s..joinpathZ.as_
-000010a0: 6669 6c65 da09 7265 6164 5f74 6578 7472  file..read_textr
-000010b0: 0700 0000 da0a 7375 6273 7469 7475 7465  ......substitute
-000010c0: da0a 7772 6974 655f 7465 7874 da04 6c69  ..write_text..li
-000010d0: 7374 da05 7061 7274 7372 0600 0000 291c  st..partsr....).
-000010e0: 7229 0000 00da 0670 6172 7365 72da 0461  r).....parser..a
-000010f0: 7267 735a 1070 6174 685f 6465 7374 696e  rgsZ.path_destin
-00001100: 6174 696f 6e72 3d00 0000 5a11 7375 6666  ationr=...Z.suff
-00001110: 6978 5f66 6f72 5f6d 6f64 756c 6572 3e00  ix_for_moduler>.
-00001120: 0000 5a0b 7061 7468 5f72 6573 756c 745a  ..Z.path_resultZ
-00001130: 0a70 6174 685f 6669 6c65 735a 0a6e 616d  .path_filesZ.nam
-00001140: 655f 6669 6c65 735a 086e 616d 655f 6469  e_filesZ.name_di
-00001150: 725a 0a70 6174 6873 5f6f 7269 675a 0d73  rZ.paths_origZ.s
-00001160: 7562 7374 6974 7574 696f 6e73 7242 0000  ubstitutionsrB..
-00001170: 0072 1400 0000 da0d 7265 6c61 7469 7665  .r......relative
-00001180: 5f70 6174 685a 0c70 6174 685f 7061 636b  _pathZ.path_pack
-00001190: 6167 655a 0e70 6174 685f 7465 6d70 6c61  ageZ.path_templa
-000011a0: 7465 735a 0a70 6174 685f 7465 7374 73da  tesZ.path_tests.
-000011b0: 0874 656d 706c 6174 655a 0c74 656d 706c  .templateZ.templ
-000011c0: 6174 655f 7265 7372 3600 0000 da04 636f  ate_resr6.....co
-000011d0: 6465 5a0f 7061 7468 5f73 6176 6564 5f63  deZ.path_saved_c
-000011e0: 6173 655a 0e70 6174 685f 6669 6c65 735f  aseZ.path_files_
-000011f0: 6469 7272 4500 0000 5a13 7061 7468 5f64  dirrE...Z.path_d
-00001200: 6972 5f73 6176 6564 5f63 6173 6572 5f00  ir_saved_caser_.
-00001210: 0000 7212 0000 0072 3700 0000 7216 0000  ..r....r7...r...
-00001220: 00da 0f69 6e69 7469 6174 655f 736f 6c76  ...initiate_solv
-00001230: 6572 3000 0000 73e8 0000 0000 010c 0204  er0...s.........
-00001240: 0102 0102 fe06 050a 020c 010c 0110 010c  ................
-00001250: 0208 0208 0214 0108 010a 020a 0108 020a  ................
-00001260: 010a 0108 010e 010a 020a 0110 0204 020c  ................
-00001270: 010e 010a 0108 020a 010e 010a 020e 020c  ................
-00001280: 010e 0204 0104 0208 010c 020c fe10 070a  ................
-00001290: 0106 0108 020c 011a 0208 020e 0108 030e  ................
-000012a0: 0104 0104 0102 0102 0102 0108 010a 010a  ................
-000012b0: 010a f606 0d04 0208 0104 0110 020e 0108  ................
-000012c0: 0108 0110 0208 010c 0104 0110 0208 0108  ................
-000012d0: 0302 fe02 010e ff02 0410 010a 0102 ff04  ................
-000012e0: 030c 0128 010e 0112 0208 010c 0210 0108  ...(............
-000012f0: 0108 0108 0208 010c 010c 020a 010a 010e  ................
-00001300: 0108 0108 020e 011c 020c 0108 0108 010a  ................
-00001310: 010e 0202 0102 0202 fe04 0602 fa04 0c02  ................
-00001320: f406 ff72 6500 0000 291d da07 5f5f 646f  ...re...)...__do
-00001330: 635f 5f72 4600 0000 7256 0000 0072 4a00  c__rF...rV...rJ.
-00001340: 0000 da09 6675 6e63 746f 6f6c 7372 0200  ....functoolsr..
-00001350: 0000 da09 696d 706f 7274 6c69 6272 0300  ....importlibr..
-00001360: 0000 da07 7061 7468 6c69 6272 0400 0000  ....pathlibr....
-00001370: 7205 0000 00da 0673 6875 7469 6c72 0600  r......shutilr..
-00001380: 0000 da06 7374 7269 6e67 7207 0000 005a  ....stringr....Z
-00001390: 0a69 6e66 6c65 6374 696f 6e72 0800 0000  .inflectionr....
-000013a0: 5a16 666c 7569 6473 696d 5f63 6f72 652e  Z.fluidsim_core.
-000013b0: 6970 795f 6c6f 6164 7209 0000 005a 175f  ipy_loadr....Z._
-000013c0: 7374 6172 745f 6970 7974 686f 6e5f 6c6f  start_ipython_lo
-000013d0: 6164 5f73 696d da13 666c 7569 6473 696d  ad_sim..fluidsim
-000013e0: 5f63 6f72 652e 7061 7468 7372 0a00 0000  _core.pathsr....
-000013f0: 721b 0000 0072 0b00 0000 723f 0000 00da  r....r....r?....
-00001400: 1466 6c75 6964 7369 6d66 6f61 6d2e 736f  .fluidsimfoam.so
-00001410: 6c76 6572 7372 0c00 0000 7228 0000 0072  lversr....r(...r
-00001420: 6500 0000 7212 0000 0072 1200 0000 7212  e...r....r....r.
-00001430: 0000 0072 1600 0000 da08 3c6d 6f64 756c  ...r......<modul
-00001440: 653e 0100 0000 7326 0000 0004 0408 0108  e>....s&........
-00001450: 0108 010c 010c 010c 010c 010c 010c 020c  ................
-00001460: 020c 030c 010c 010c 0308 1202 0104 ff06  ................
-00001470: 05                                       .
+00000040: 5a02 6401 6402 6c03 5a03 6401 6402 6c04  Z.d.d.l.Z.d.d.l.
+00000050: 5a04 6401 6403 6c05 6d06 5a06 0100 6401  Z.d.d.l.m.Z...d.
+00000060: 6404 6c07 6d08 5a08 0100 6401 6405 6c09  d.l.m.Z...d.d.l.
+00000070: 6d0a 5a0a 0100 6401 6406 6c0b 6d0b 5a0b  m.Z...d.d.l.m.Z.
+00000080: 0100 6401 6407 6c0c 6d0d 5a0d 0100 6401  ..d.d.l.m.Z...d.
+00000090: 6408 6c0e 6d0f 5a0f 0100 6401 6409 6c10  d.l.m.Z...d.d.l.
+000000a0: 6d11 5a11 0100 6401 640a 6c12 6d13 5a14  m.Z...d.d.l.m.Z.
+000000b0: 0100 6401 640b 6c15 6d16 5a16 0100 6401  ..d.d.l.m.Z...d.
+000000c0: 640c 6c17 6d18 5a19 0100 6401 640d 6c1a  d.l.m.Z...d.d.l.
+000000d0: 6d1b 5a1b 0100 640e 640f 8400 5a1c 6506  m.Z...d.d...Z.e.
+000000e0: 6514 6410 6411 8d02 5a13 6412 6413 8400  e.d.d...Z.d.d...
+000000f0: 5a1d 6402 5300 2914 7a1a 436f 6e73 6f6c  Z.d.S.).z.Consol
+00000100: 6520 7363 7269 7074 2066 756e 6374 696f  e script functio
+00000110: 6e73 0a0a e900 0000 004e 2901 da07 7061  ns.......N)...pa
+00000120: 7274 6961 6c29 01da 0972 6573 6f75 7263  rtial)...resourc
+00000130: 6573 2901 da04 5061 7468 2901 da06 7070  es)...Path)...pp
+00000140: 7269 6e74 2901 da04 636f 7079 2901 da08  rint)...copy)...
+00000150: 5465 6d70 6c61 7465 2901 da08 6361 6d65  Template)...came
+00000160: 6c69 7a65 2901 da16 7374 6172 745f 6970  lize)...start_ip
+00000170: 7974 686f 6e5f 6c6f 6164 5f73 696d 2901  ython_load_sim).
+00000180: da10 7061 7468 5f64 6972 5f72 6573 756c  ..path_dir_resul
+00000190: 7473 2901 da0b 5f5f 7665 7273 696f 6e5f  ts)...__version_
+000001a0: 5f29 01da 1161 7661 696c 6162 6c65 5f73  _)...available_s
+000001b0: 6f6c 7665 7273 6300 0000 0000 0000 0000  olversc.........
+000001c0: 0000 0009 0000 0005 0000 0043 0000 0073  ...........C...s
+000001d0: 9a00 0000 6401 6400 6c00 7d00 6401 6400  ....d.d.l.}.d.d.
+000001e0: 6c01 7d01 6401 6400 6c02 7d02 6402 6403  l.}.d.d.l.}.d.d.
+000001f0: 6404 9c02 7d03 7c02 7c00 7c01 6703 7d04  d...}.|.|.|.g.}.
+00000200: 7c04 4400 5d08 7d05 7c05 6a03 7c03 7c05  |.D.].}.|.j.|.|.
+00000210: 6a04 3c00 7118 7c03 a005 a100 4400 5d10  j.<.q.|.....D.].
+00000220: 5c02 7d06 7d07 7406 7c06 a007 6405 a101  \.}.}.t.|...d...
+00000230: 9b00 6406 7c07 9b00 9d03 8301 0100 7125  ..d.|.........q%
+00000240: 7408 7409 6407 6408 8400 740a 8300 4400  t.t.d.d...t...D.
+00000250: 8301 8301 8301 7d08 7406 6409 640a a00b  ......}.t.d.d...
+00000260: 7c08 a101 1700 8301 0100 6400 5300 290b  |.........d.S.).
+00000270: 4e72 0100 0000 da07 5665 7273 696f 6efa  Nr......Version.
+00000280: 072d 2d2d 2d2d 2d2d 2902 5a07 5061 636b  .-------).Z.Pack
+00000290: 6167 6572 0e00 0000 e90f 0000 00fa 0120  ager........... 
+000002a0: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
+000002b0: 0003 0000 0053 0000 00f3 1200 0000 6700  .....S........g.
+000002c0: 7c00 5d05 7d01 7c01 6a00 9102 7102 5300  |.].}.|.j...q.S.
+000002d0: a900 a901 da04 6e61 6d65 2902 da02 2e30  ......name)....0
+000002e0: 5a0b 656e 7472 795f 706f 696e 7472 1200  Z.entry_pointr..
+000002f0: 0000 7212 0000 00fa 3e2f 686f 6d65 2f70  ..r.....>/home/p
+00000300: 6965 7272 652f 4465 762f 666c 7569 6473  ierre/Dev/fluids
+00000310: 696d 666f 616d 2f73 7263 2f66 6c75 6964  imfoam/src/fluid
+00000320: 7369 6d66 6f61 6d2f 7574 696c 2f63 6f6e  simfoam/util/con
+00000330: 736f 6c65 2e70 79da 0a3c 6c69 7374 636f  sole.py..<listco
+00000340: 6d70 3e28 0000 00f3 0200 0000 1200 7a22  mp>(..........z"
+00000350: 7072 696e 745f 7665 7273 696f 6e73 2e3c  print_versions.<
+00000360: 6c6f 6361 6c73 3e2e 3c6c 6973 7463 6f6d  locals>.<listcom
+00000370: 703e 7a14 0a49 6e73 7461 6c6c 6564 2073  p>z..Installed s
+00000380: 6f6c 7665 7273 3a20 7a02 2c20 290c da08  olvers: z., )...
+00000390: 666c 7569 6464 796e da0d 666c 7569 6473  fluiddyn..fluids
+000003a0: 696d 5f63 6f72 65da 0c66 6c75 6964 7369  im_core..fluidsi
+000003b0: 6d66 6f61 6d72 0b00 0000 da08 5f5f 6e61  mfoamr......__na
+000003c0: 6d65 5f5f da05 6974 656d 73da 0570 7269  me__..items..pri
+000003d0: 6e74 da05 6c6a 7573 74da 0673 6f72 7465  nt..ljust..sorte
+000003e0: 64da 0373 6574 720c 0000 00da 046a 6f69  d..setr......joi
+000003f0: 6e29 0972 1900 0000 721a 0000 0072 1b00  n).r....r....r..
+00000400: 0000 5a08 7665 7273 696f 6e73 5a08 7061  ..Z.versionsZ.pa
+00000410: 636b 6167 6573 da07 7061 636b 6167 655a  ckages..packageZ
+00000420: 0870 6b67 5f6e 616d 65da 0776 6572 7369  .pkg_name..versi
+00000430: 6f6e da05 6e61 6d65 7372 1200 0000 7212  on..namesr....r.
+00000440: 0000 0072 1600 0000 da0e 7072 696e 745f  ...r......print_
+00000450: 7665 7273 696f 6e73 1a00 0000 7316 0000  versions....s...
+00000460: 0008 0108 0108 010a 020a 0208 010e 0110  ................
+00000470: 021a 0118 0216 0172 2600 0000 7a1d 6672  .......r&...z.fr
+00000480: 6f6d 2066 6c75 6964 7369 6d66 6f61 6d20  om fluidsimfoam 
+00000490: 696d 706f 7274 206c 6f61 6429 015a 0b6c  import load).Z.l
+000004a0: 6f61 645f 696d 706f 7274 6300 0000 0000  oad_importc.....
+000004b0: 0000 0000 0000 001e 0000 000c 0000 0003  ................
+000004c0: 0000 0073 b404 0000 6401 6402 6c00 6d01  ...s....d.d.l.m.
+000004d0: 7d00 6d02 7d01 0100 7403 6a04 6403 6404  }.m.}...t.j.d.d.
+000004e0: 6405 8d02 7d02 7c02 a005 6406 a101 0100  d...}.|...d.....
+000004f0: 7c02 a005 6407 6408 a102 0100 7c02 a005  |...d.d.....|...
+00000500: 6409 640a a102 0100 7c02 6a05 640b 640c  d.d.....|.j.d.d.
+00000510: 640d 640e 8d03 0100 7c02 a005 640f 6410  d.d.....|...d.d.
+00000520: a102 0100 7c02 a006 a100 7d03 7407 7c03  ....|.....}.t.|.
+00000530: 8301 0100 7c03 6a08 6400 7500 7249 7c03  ....|.j.d.u.rI|.
+00000540: 6a09 6400 7500 7249 7407 6411 8301 0100  j.d.u.rIt.d.....
+00000550: 740a a00b 6412 a101 0100 7c03 6a09 6400  t...d.....|.j.d.
+00000560: 7501 7252 740c 6413 8301 8201 7c03 6a08  u.rRt.d.....|.j.
+00000570: 6400 7501 726c 740d 7c03 6a08 8301 8900  d.u.rlt.|.j.....
+00000580: 8800 a00e a100 736c 7407 8800 9b00 6414  ......slt.....d.
+00000590: 9d02 8301 0100 740a a00b 6412 a101 0100  ......t...d.....
+000005a0: 7c03 6a0f 6400 7501 7279 740d 7c03 6a0f  |.j.d.u.ryt.|.j.
+000005b0: 8301 a010 a100 7d04 6e02 7411 7d04 6415  ......}.n.t.}.d.
+000005c0: 7c03 6a12 9b00 9d02 7d05 7c03 6a12 a013  |.j.....}.|.j...
+000005d0: 6416 6417 a102 7d06 6418 7c06 9b00 9d02  d.d...}.d.|.....
+000005e0: 7d07 7c04 7c05 1b00 7d08 7c08 a00e a100  }.|.|...}.|.....
+000005f0: 72a1 7407 7c08 9b00 6419 9d02 8301 0100  r.t.|...d.......
+00000600: 740a a00b 6412 a101 0100 7407 641a 7c08  t...d.....t.d.|.
+00000610: 9b00 9d02 8301 0100 7c03 6a08 6400 7501  ........|.j.d.u.
+00000620: 72f0 7407 641b 8800 9b00 9d02 8301 0100  r.t.d...........
+00000630: 6900 7d09 6900 7d0a 641c 4400 5d14 7d0b  i.}.i.}.d.D.].}.
+00000640: 7414 8700 6601 641d 641e 8408 8800 a015  t...f.d.d.......
+00000650: 7c0b 641f 1700 a101 4400 8301 8301 7c09  |.d.....D.....|.
+00000660: 7c0b 3c00 71ba 7c09 a016 6420 a101 7d0c  |.<.q.|...d ..}.
+00000670: 7c0c 72da 7c0c 7c09 6421 3c00 7c09 a017  |.r.|.|.d!<.|...
+00000680: a100 4400 5d0d 7d0b 6422 6423 8400 7c09  ..D.].}.d"d#..|.
+00000690: 7c0b 1900 4400 8301 7c0a 7c0b 3c00 71de  |...D...|.|.<.q.
+000006a0: 7418 7c0a 8301 0100 7407 6424 7c08 9b00  t.|.....t.d$|...
+000006b0: 9d02 8301 0100 7c08 a019 a100 0100 741a  ......|.......t.
+000006c0: 741b 6a1c a01d a100 6a1e 8301 7c03 6a1f  t.j.....j...|.j.
+000006d0: 7c03 6a12 7c05 7c07 7420 7421 7c06 8301  |.j.|.|.t t!|...
+000006e0: 741a 7c0a 6421 1900 8301 741a 7c0a 6425  t.|.d!....t.|.d%
+000006f0: 1900 8301 741a 7c0a 6426 1900 8301 6427  ....t.|.d&....d'
+00000700: 9c0a 7d0d 6900 7d0e 6428 4400 5d0b 7d0f  ..}.i.}.d(D.].}.
+00000710: 7c0f 7d10 7c0f 6429 1700 7c0e 7c10 3c00  |.}.|.d)..|.|.<.
+00000720: 9001 7122 7c08 642a 7c07 9b00 9d02 1b00  ..q"|.d*|.......
+00000730: 7d11 642b 4400 5d0d 7d0f 7c11 7c0f 1b00  }.d+D.].}.|.|...
+00000740: 7d10 7c0f 6429 1700 7c0e 7c10 3c00 9001  }.|.d)..|.|.<...
+00000750: 7137 7c11 642c 1b00 7d12 7c12 6a19 642d  q7|.d,..}.|.j.d-
+00000760: 642e 8d01 0100 642f 7d0f 7c0f 6429 1700  d.....d/}.|.d)..
+00000770: 7c0e 7c12 7c0f 1b00 3c00 7c08 6430 1b00  |.|.|...<.|.d0..
+00000780: 7d13 7c13 a019 a100 0100 6431 7c0e 7c13  }.|.......d1|.|.
+00000790: 6432 7c06 9b00 6433 9d03 1b00 3c00 7c0e  d2|...d3....<.|.
+000007a0: a022 a100 4400 5d35 5c02 7d10 7d14 7423  ."..D.]5\.}.}.t#
+000007b0: a024 6434 a101 a025 7c14 a101 7d15 7423  .$d4...%|...}.t#
+000007c0: a026 7c15 a101 8f0c 7d16 7c16 a027 a100  .&|.....}.|..'..
+000007d0: 7d17 5700 6400 0400 0400 8303 0100 6e09  }.W.d.........n.
+000007e0: 3100 9001 7390 7701 0100 0100 0100 5900  1...s.w.......Y.
+000007f0: 0100 7428 7c17 8301 a029 7c0d a101 7d17  ..t(|....)|...}.
+00000800: 7c08 7c10 1b00 a02a 7c17 a101 0100 9001  |.|....*|.......
+00000810: 716f 7c13 6435 1b00 7d18 7c18 6a19 642d  qo|.d5..}.|.j.d-
+00000820: 642e 8d01 0100 7c09 a022 a100 4400 5d7c  d.....|.."..D.]|
+00000830: 5c02 7d0b 7d19 7c0b 6421 6b02 7d1a 7c18  \.}.}.|.d!k.}.|.
+00000840: 7c0b 1b00 7d1b 7c1b a019 a100 0100 7c19  |...}.|.......|.
+00000850: 4400 5d68 7d10 8800 7c10 1b00 a027 a100  D.]h}...|....'..
+00000860: 7d17 7a08 7c01 7c17 7c1a 6436 8d02 7d17  }.z.|.|.|.d6..}.
+00000870: 5700 6e11 0400 7c00 9001 79e6 0100 0100  W.n...|...y.....
+00000880: 0100 7407 6437 7c10 9b00 9d02 8301 0100  ..t.d7|.........
+00000890: 5900 6e01 7700 742b a02c 6438 6439 7c17  Y.n.w.t+.,d8d9|.
+000008a0: a103 a02d a100 6439 1700 7d17 643a 7c17  ...-..d9..}.d:|.
+000008b0: 7600 9002 7200 643b 7c17 a02d a100 1700  v...r.d;|..-....
+000008c0: 643c 1700 7d1c 6e02 7c17 7d1c 7c0b 6421  d<..}.n.|.}.|.d!
+000008d0: 6b02 9002 721b 742e 7c10 6a2f 8301 7d1d  k...r.t.|.j/..}.
+000008e0: 7c1d 6401 1900 6420 6b02 9002 721b 6421  |.d...d k...r.d!
+000008f0: 7c1d 6401 3c00 740d 7c1d 8e00 7d10 7c18  |.d.<.t.|...}.|.
+00000900: 7c10 1b00 a02a 7c17 a101 0100 7c12 7c10  |....*|.....|.|.
+00000910: 6a12 643d 1700 1b00 a02a 7c1c a101 0100  j.d=.....*|.....
+00000920: 9001 71c5 9001 71b3 7c03 6a08 6400 7501  ..q...q.|.j.d.u.
+00000930: 9002 724a 643e 4400 5d11 7d0f 8800 7c0f  ..rJd>D.].}...|.
+00000940: 1b00 7d16 7c16 a00e a100 9002 7248 7430  ..}.|.......rHt0
+00000950: 7c16 7c18 8302 0100 9002 7138 7407 643f  |.|.......q8t.d?
+00000960: 7c05 9b00 6440 7c08 9b00 6441 7c07 9b00  |...d@|...dA|...
+00000970: 6442 9d07 8301 0100 6400 5300 2943 4e72  dB......d.S.)CNr
+00000980: 0100 0000 2902 da0f 466f 616d 466f 726d  ....)...FoamForm
+00000990: 6174 4572 726f 72da 0b66 6f72 6d61 745f  atError..format_
+000009a0: 636f 6465 7a1c 666c 7569 6473 696d 666f  codez.fluidsimfo
+000009b0: 616d 2d69 6e69 7469 6174 652d 736f 6c76  am-initiate-solv
+000009c0: 6572 7a15 496e 6974 6961 7465 2061 206e  erz.Initiate a n
+000009d0: 6577 2073 6f6c 7665 7229 02da 0470 726f  ew solver)...pro
+000009e0: 67da 0b64 6573 6372 6970 7469 6f6e 7214  g..descriptionr.
+000009f0: 0000 007a 022d 637a 0b2d 2d66 726f 6d2d  ...z.-cz.--from-
+00000a00: 6361 7365 7a02 2d73 7a0d 2d2d 6672 6f6d  casez.-sz.--from
+00000a10: 2d73 6f6c 7665 727a 022d 617a 082d 2d61  -solverz.-az.--a
+00000a20: 7574 686f 727a 1746 6c75 6964 7369 6d66  uthorz.Fluidsimf
+00000a30: 6f61 6d20 6465 7665 6c6f 7065 7273 2901  oam developers).
+00000a40: da07 6465 6661 756c 747a 022d 647a 0d2d  ..defaultz.-dz.-
+00000a50: 2d64 6573 7469 6e61 7469 6f6e 7a38 596f  -destinationz8Yo
+00000a60: 7520 7368 6f75 6c64 2061 7420 6c65 6173  u should at leas
+00000a70: 7420 7072 6f76 6964 6520 6120 6361 7365  t provide a case
+00000a80: 2028 2d63 2920 6f72 2061 2073 6f6c 7665   (-c) or a solve
+00000a90: 7220 282d 7329 e901 0000 007a 2a53 6f72  r (-s).....z*Sor
+00000aa0: 7279 2c20 6f70 7469 6f6e 202d 7320 6973  ry, option -s is
+00000ab0: 206e 6f74 2079 6574 2069 6d70 6c65 6d65   not yet impleme
+00000ac0: 6e74 6564 2e2e 2e7a 1020 646f 6573 206e  nted...z. does n
+00000ad0: 6f74 2065 7869 7374 2e7a 0d66 6c75 6964  ot exist.z.fluid
+00000ae0: 7369 6d66 6f61 6d2d fa01 2dda 015f 5a0d  simfoam-..-.._Z.
+00000af0: 666c 7569 6473 696d 666f 616d 5f7a 1020  fluidsimfoam_z. 
+00000b00: 616c 7265 6164 7920 6578 6973 7473 2e7a  already exists.z
+00000b10: 1a4c 6574 2773 2069 6e69 7469 6174 6520  .Let's initiate 
+00000b20: 7468 6520 736f 6c76 6572 207a 0b55 7369  the solver z.Usi
+00000b30: 6e67 2063 6173 6520 2904 da06 7379 7374  ng case )...syst
+00000b40: 656d da08 636f 6e73 7461 6e74 da01 30fa  em..constant..0.
+00000b50: 0630 2e6f 7269 6763 0100 0000 0000 0000  .0.origc........
+00000b60: 0000 0000 0200 0000 0400 0000 3300 0000  ............3...
+00000b70: 7322 0000 0081 007c 005d 0c7d 017c 01a0  s".....|.].}.|..
+00000b80: 00a1 0072 027c 01a0 0188 00a1 0156 0001  ...r.|.......V..
+00000b90: 0071 0264 0053 0029 014e 2902 da07 6973  .q.d.S.).N)...is
+00000ba0: 5f66 696c 65da 0b72 656c 6174 6976 655f  _file..relative_
+00000bb0: 746f 2902 7215 0000 00da 0470 6174 68a9  to).r......path.
+00000bc0: 015a 0970 6174 685f 6361 7365 7212 0000  .Z.path_caser...
+00000bd0: 0072 1600 0000 da09 3c67 656e 6578 7072  .r......<genexpr
+00000be0: 3e68 0000 0073 0e00 0000 0280 0400 0202  >h...s..........
+00000bf0: 0602 02fc 0801 0aff 7a22 696e 6974 6961  ........z"initia
+00000c00: 7465 5f73 6f6c 7665 722e 3c6c 6f63 616c  te_solver.<local
+00000c10: 733e 2e3c 6765 6e65 7870 723e 7a02 2f2a  s>.<genexpr>z./*
+00000c20: 7232 0000 0072 3100 0000 6301 0000 0000  r2...r1...c.....
+00000c30: 0000 0000 0000 0002 0000 0003 0000 0053  ...............S
+00000c40: 0000 0072 1100 0000 7212 0000 0072 1300  ...r....r....r..
+00000c50: 0000 2902 7215 0000 00da 0170 7212 0000  ..).r......pr...
+00000c60: 0072 1200 0000 7216 0000 0072 1700 0000  .r....r....r....
+00000c70: 7400 0000 7218 0000 007a 2369 6e69 7469  t...r....z#initi
+00000c80: 6174 655f 736f 6c76 6572 2e3c 6c6f 6361  ate_solver.<loca
+00000c90: 6c73 3e2e 3c6c 6973 7463 6f6d 703e 7a07  ls>.<listcomp>z.
+00000ca0: 4d61 6b69 6e67 2072 2f00 0000 7230 0000  Making r/...r0..
+00000cb0: 0029 0ada 0479 6561 72da 0661 7574 686f  .)...year..autho
+00000cc0: 725a 0a6e 616d 655f 7368 6f72 74da 0c6e  rZ.name_short..n
+00000cd0: 616d 655f 7072 6f6a 6563 74da 0c6e 616d  ame_project..nam
+00000ce0: 655f 7061 636b 6167 65da 1466 6c75 6964  e_package..fluid
+00000cf0: 7369 6d66 6f61 6d5f 7665 7273 696f 6e5a  simfoam_versionZ
+00000d00: 1073 7566 6669 785f 666f 725f 636c 6173  .suffix_for_clas
+00000d10: 735a 0e6e 616d 655f 7661 7269 6162 6c65  sZ.name_variable
+00000d20: 735a 116e 616d 655f 7379 7374 656d 5f66  sZ.name_system_f
+00000d30: 696c 6573 5a13 6e61 6d65 5f63 6f6e 7374  ilesZ.name_const
+00000d40: 616e 745f 6669 6c65 7329 03da 074c 4943  ant_files)...LIC
+00000d50: 454e 5345 7a09 5245 4144 4d45 2e6d 647a  ENSEz.README.mdz
+00000d60: 0e70 7970 726f 6a65 6374 2e74 6f6d 6c7a  .pyproject.tomlz
+00000d70: 092e 7465 6d70 6c61 7465 7a04 7372 632f  ..templatez.src/
+00000d80: 2903 7a0b 5f5f 696e 6974 5f5f 2e70 797a  ).z.__init__.pyz
+00000d90: 096f 7574 7075 742e 7079 fa08 7461 736b  .output.py..task
+00000da0: 732e 7079 da09 7465 6d70 6c61 7465 7354  s.py..templatesT
+00000db0: 2901 da07 7061 7265 6e74 7372 3f00 0000  )...parentsr?...
+00000dc0: da05 7465 7374 737a 2174 6573 745f 6765  ..testsz!test_ge
+00000dd0: 6e65 7261 7465 645f 736f 6c76 6572 2e70  nerated_solver.p
+00000de0: 792e 7465 6d70 6c61 7465 5a05 7465 7374  y.templateZ.test
+00000df0: 5f7a 032e 7079 7a16 666c 7569 6473 696d  _z..pyz.fluidsim
+00000e00: 666f 616d 2e72 6573 6f75 7263 6573 7a11  foam.resourcesz.
+00000e10: 7361 7665 645f 6361 7365 732f 6361 7365  saved_cases/case
+00000e20: 3029 01da 0861 735f 6669 656c 647a 184e  0)...as_fieldz.N
+00000e30: 6f74 2061 626c 6520 746f 2066 6f72 6d61  ot able to forma
+00000e40: 7420 6669 6c65 207a 055c 732b 5c6e da01  t file z.\s+\n..
+00000e50: 0a7a 027b 7b7a 097b 2520 7261 7720 257d  .z.{{z.{% raw %}
+00000e60: 7a0d 7b25 2065 6e64 7261 7720 257d 0a7a  z.{% endraw %}.z
+00000e70: 062e 6a69 6e6a 6129 025a 0841 6c6c 636c  ..jinja).Z.Allcl
+00000e80: 6561 6e5a 0641 6c6c 7275 6e7a 0d0a 0a4e  eanZ.Allrunz...N
+00000e90: 6577 2073 6f6c 7665 7220 7a5f 2063 7265  ew solver z_ cre
+00000ea0: 6174 6564 2120 596f 7520 6361 6e20 6e6f  ated! You can no
+00000eb0: 7720 696e 7374 616c 6c20 616e 6420 7465  w install and te
+00000ec0: 7374 2069 7420 746f 2063 6865 636b 2069  st it to check i
+00000ed0: 660a 6974 2072 6570 726f 6475 6365 7320  f.it reproduces 
+00000ee0: 796f 7572 2069 6e69 7469 616c 2063 6173  your initial cas
+00000ef0: 652e 0a0a 6060 600a 6364 207a 860a 7069  e...```.cd z..pi
+00000f00: 7020 696e 7374 616c 6c20 2d65 202e 0a70  p install -e ..p
+00000f10: 7974 6573 7420 7465 7374 7320 2d76 760a  ytest tests -vv.
+00000f20: 6060 600a 0a59 6f75 2063 616e 2074 6865  ```..You can the
+00000f30: 6e20 696d 7072 6f76 6520 796f 7572 2066  n improve your f
+00000f40: 6c75 6964 7369 6d66 6f61 6d20 736f 6c76  luidsimfoam solv
+00000f50: 6572 2062 7920 6d6f 6469 6679 696e 6720  er by modifying 
+00000f60: 6974 7320 6669 6c65 730a 2865 7370 6563  its files.(espec
+00000f70: 6961 6c6c 7920 7468 6520 6669 6c65 2073  ially the file s
+00000f80: 7263 2f7a 7e2f 6f75 7470 7574 2e70 7929  rc/z~/output.py)
+00000f90: 2e20 4578 616d 706c 6573 2063 616e 2062  . Examples can b
+00000fa0: 6520 666f 756e 6420 696e 0a68 7474 7073  e found in.https
+00000fb0: 3a2f 2f66 6f73 732e 6865 7074 6170 6f64  ://foss.heptapod
+00000fc0: 2e6e 6574 2f66 6c75 6964 6479 6e2f 666c  .net/fluiddyn/fl
+00000fd0: 7569 6473 696d 666f 616d 2f2d 2f74 7265  uidsimfoam/-/tre
+00000fe0: 652f 6272 616e 6368 2f64 6566 6175 6c74  e/branch/default
+00000ff0: 2f64 6f63 2f65 7861 6d70 6c65 730a 0a20  /doc/examples.. 
+00001000: 2020 2029 315a 1d66 6c75 6964 7369 6d66     )1Z.fluidsimf
+00001010: 6f61 6d2e 666f 616d 5f69 6e70 7574 5f66  oam.foam_input_f
+00001020: 696c 6573 7227 0000 0072 2800 0000 da08  ilesr'...r(.....
+00001030: 6172 6770 6172 7365 da0e 4172 6775 6d65  argparse..Argume
+00001040: 6e74 5061 7273 6572 da0c 6164 645f 6172  ntParser..add_ar
+00001050: 6775 6d65 6e74 da0a 7061 7273 655f 6172  gument..parse_ar
+00001060: 6773 721e 0000 005a 0966 726f 6d5f 6361  gsr....Z.from_ca
+00001070: 7365 5a0b 6672 6f6d 5f73 6f6c 7665 72da  seZ.from_solver.
+00001080: 0373 7973 da04 6578 6974 da13 4e6f 7449  .sys..exit..NotI
+00001090: 6d70 6c65 6d65 6e74 6564 4572 726f 7272  mplementedErrorr
+000010a0: 0400 0000 da06 6578 6973 7473 da0b 6465  ......exists..de
+000010b0: 7374 696e 6174 696f 6eda 0772 6573 6f6c  stination..resol
+000010c0: 7665 720a 0000 0072 1400 0000 da07 7265  ver....r......re
+000010d0: 706c 6163 6572 2000 0000 da04 676c 6f62  placer .....glob
+000010e0: da03 706f 70da 046b 6579 7372 0500 0000  ..pop..keysr....
+000010f0: da05 6d6b 6469 72da 0373 7472 da08 6461  ..mkdir..str..da
+00001100: 7465 7469 6d65 da04 6461 7465 da05 746f  tetime..date..to
+00001110: 6461 7972 3900 0000 723a 0000 0072 3d00  dayr9...r:...r=.
+00001120: 0000 7208 0000 0072 1d00 0000 7203 0000  ..r....r....r...
+00001130: 00da 0566 696c 6573 da08 6a6f 696e 7061  ...files..joinpa
+00001140: 7468 5a07 6173 5f66 696c 65da 0972 6561  thZ.as_file..rea
+00001150: 645f 7465 7874 7207 0000 00da 0a73 7562  d_textr......sub
+00001160: 7374 6974 7574 65da 0a77 7269 7465 5f74  stitute..write_t
+00001170: 6578 74da 0272 65da 0373 7562 da05 7374  ext..re..sub..st
+00001180: 7269 70da 046c 6973 74da 0570 6172 7473  rip..list..parts
+00001190: 7206 0000 0029 1e72 2700 0000 7228 0000  r....).r'...r(..
+000011a0: 00da 0670 6172 7365 72da 0461 7267 735a  ...parser..argsZ
+000011b0: 1070 6174 685f 6465 7374 696e 6174 696f  .path_destinatio
+000011c0: 6e72 3b00 0000 5a11 7375 6666 6978 5f66  nr;...Z.suffix_f
+000011d0: 6f72 5f6d 6f64 756c 6572 3c00 0000 5a0b  or_moduler<...Z.
+000011e0: 7061 7468 5f72 6573 756c 745a 0a70 6174  path_resultZ.pat
+000011f0: 685f 6669 6c65 735a 0a6e 616d 655f 6669  h_filesZ.name_fi
+00001200: 6c65 735a 086e 616d 655f 6469 725a 0a70  lesZ.name_dirZ.p
+00001210: 6174 6873 5f6f 7269 675a 0d73 7562 7374  aths_origZ.subst
+00001220: 6974 7574 696f 6e73 7240 0000 0072 1400  itutionsr@...r..
+00001230: 0000 5a0d 7265 6c61 7469 7665 5f70 6174  ..Z.relative_pat
+00001240: 685a 0c70 6174 685f 7061 636b 6167 655a  hZ.path_packageZ
+00001250: 0e70 6174 685f 7465 6d70 6c61 7465 735a  .path_templatesZ
+00001260: 0a70 6174 685f 7465 7374 73da 0874 656d  .path_tests..tem
+00001270: 706c 6174 655a 0c74 656d 706c 6174 655f  plateZ.template_
+00001280: 7265 7372 3500 0000 da04 636f 6465 5a0f  resr5.....codeZ.
+00001290: 7061 7468 5f73 6176 6564 5f63 6173 655a  path_saved_caseZ
+000012a0: 0e70 6174 685f 6669 6c65 735f 6469 7272  .path_files_dirr
+000012b0: 4300 0000 5a13 7061 7468 5f64 6972 5f73  C...Z.path_dir_s
+000012c0: 6176 6564 5f63 6173 655a 0d63 6f64 655f  aved_caseZ.code_
+000012d0: 7465 6d70 6c61 7465 7261 0000 0072 1200  templatera...r..
+000012e0: 0000 7236 0000 0072 1600 0000 da0f 696e  ..r6...r......in
+000012f0: 6974 6961 7465 5f73 6f6c 7665 7231 0000  itiate_solver1..
+00001300: 0073 0201 0000 1001 0402 0201 0201 06fe  .s..............
+00001310: 0a05 0c02 0c01 1001 0c01 0802 0802 1402  ................
+00001320: 0801 0a01 0a02 0801 0a02 0a01 0801 0e01  ................
+00001330: 0a01 0a02 1001 0402 0c02 0e01 0a01 0801  ................
+00001340: 0802 0e01 0a01 0e02 0a02 0e01 0402 0401  ................
+00001350: 0802 0c01 0c02 0efe 0a07 0401 0801 0c02  ................
+00001360: 1801 0802 0e02 0801 0e03 0401 0401 0201  ................
+00001370: 0201 0201 0601 0a01 0a01 0a01 06f6 040d  ................
+00001380: 0802 0401 1001 0e02 0801 0801 1001 0802  ................
+00001390: 0c01 0401 1001 0802 0801 0203 02fe 0e01  ................
+000013a0: 02ff 1004 0a01 0201 04ff 0c03 0a01 1eff  ................
+000013b0: 0e02 1201 0802 0c01 1002 0801 0801 0801  ................
+000013c0: 0802 0c01 0201 1001 0e01 1201 02ff 1604  ................
+000013d0: 0a02 1202 0402 0a02 0a01 0e01 0801 0801  ................
+000013e0: 0e02 0e01 0201 08ff 04e9 0c1b 0801 0801  ................
+000013f0: 0a01 0a01 0480 0202 0201 0202 04fe 0206  ................
+00001400: 04fa 020c 06f4 08ff 7266 0000 0029 1eda  ........rf...)..
+00001410: 075f 5f64 6f63 5f5f 7245 0000 0072 5500  .__doc__rE...rU.
+00001420: 0000 725d 0000 0072 4900 0000 da09 6675  ..r]...rI.....fu
+00001430: 6e63 746f 6f6c 7372 0200 0000 da09 696d  nctoolsr......im
+00001440: 706f 7274 6c69 6272 0300 0000 da07 7061  portlibr......pa
+00001450: 7468 6c69 6272 0400 0000 7205 0000 00da  thlibr....r.....
+00001460: 0673 6875 7469 6c72 0600 0000 da06 7374  .shutilr......st
+00001470: 7269 6e67 7207 0000 005a 0a69 6e66 6c65  ringr....Z.infle
+00001480: 6374 696f 6e72 0800 0000 5a16 666c 7569  ctionr....Z.flui
+00001490: 6473 696d 5f63 6f72 652e 6970 795f 6c6f  dsim_core.ipy_lo
+000014a0: 6164 7209 0000 005a 175f 7374 6172 745f  adr....Z._start_
+000014b0: 6970 7974 686f 6e5f 6c6f 6164 5f73 696d  ipython_load_sim
+000014c0: da13 666c 7569 6473 696d 5f63 6f72 652e  ..fluidsim_core.
+000014d0: 7061 7468 7372 0a00 0000 721b 0000 0072  pathsr....r....r
+000014e0: 0b00 0000 723d 0000 00da 1466 6c75 6964  ....r=.....fluid
+000014f0: 7369 6d66 6f61 6d2e 736f 6c76 6572 7372  simfoam.solversr
+00001500: 0c00 0000 7226 0000 0072 6600 0000 7212  ....r&...rf...r.
+00001510: 0000 0072 1200 0000 7212 0000 0072 1600  ...r....r....r..
+00001520: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
+00001530: 732a 0000 0004 0008 0408 0108 0108 010c  s*..............
+00001540: 010c 010c 010c 010c 010c 010c 020c 020c  ................
+00001550: 030c 010c 0108 0302 1204 0106 ff0c 05    ...............
```

### Comparing `fluidsimfoam-0.0.5/src/fluidsimfoam/util/console.py` & `fluidsimfoam-0.0.6/src/fluidsimfoam/util/console.py`

 * *Files identical despite different names*

### Comparing `fluidsimfoam-0.0.5/PKG-INFO` & `fluidsimfoam-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: fluidsimfoam
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python framework for OpenFOAM
 License: BSD-3-Clause
 Author: pierre.augier
 Author-email: pierre.augier@univ-grenoble-alpes.fr
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: jupyter
 Provides-Extra: qt
-Requires-Dist: PySide6 (>=6.5.0,<7.0.0) ; (python_version >= "3.9" and python_version < "3.12") and (extra == "qt")
+Requires-Dist: PySide6 (>=6.5.1,<7.0.0) ; (python_version >= "3.9" and python_version < "3.12") and (extra == "qt")
 Requires-Dist: fluiddyn (>=0.5.2,<0.6.0)
 Requires-Dist: fluidsim-core (>=0.7.3,<0.8.0)
 Requires-Dist: inflection (>=0.5.1,<0.6.0)
 Requires-Dist: invoke (>=2.0.0,<3.0.0)
-Requires-Dist: ipython (>=8.11.0,<9.0.0)
+Requires-Dist: ipython (>=8.14.0,<9.0.0)
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: jupyterlab (>=3.6.3,<4.0.0) ; extra == "jupyter"
 Requires-Dist: jupyterlab_myst (>=1.1.3,<2.0.0) ; extra == "jupyter"
 Requires-Dist: jupytext (>=1.14.5,<2.0.0) ; extra == "jupyter"
 Requires-Dist: lark (>=1.1.5,<2.0.0)
 Requires-Dist: mdformat-myst (>=0.1.4,<0.2.0) ; extra == "jupyter"
 Requires-Dist: pandas (>=1.5.3,<2.0.0)
```

