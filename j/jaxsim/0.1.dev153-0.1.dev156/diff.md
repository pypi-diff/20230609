# Comparing `tmp/jaxsim-0.1.dev153.tar.gz` & `tmp/jaxsim-0.1.dev156.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaxsim-0.1.dev153.tar", last modified: Fri May  5 17:19:55 2023, max compression
+gzip compressed data, was "jaxsim-0.1.dev156.tar", last modified: Fri Jun  9 09:57:32 2023, max compression
```

## Comparing `jaxsim-0.1.dev153.tar` & `jaxsim-0.1.dev156.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:19:55.383685 jaxsim-0.1.dev153/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:19:55.367683 jaxsim-0.1.dev153/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:19:55.371683 jaxsim-0.1.dev153/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-05-05 17:19:41.000000 jaxsim-0.1.dev153/.github/workflows/ci_cd.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-05 17:19:41.000000 jaxsim-0.1.dev153/.github/workflows/style.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-05-05 17:19:41.000000 jaxsim-0.1.dev153/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-05-05 17:19:41.000000 jaxsim-0.1.dev153/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-05-05 17:19:55.383685 jaxsim-0.1.dev153/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-05-05 17:19:41.000000 jaxsim-0.1.dev153/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-05 17:19:41.000000 jaxsim-0.1.dev153/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-05-05 17:19:55.383685 jaxsim-0.1.dev153/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 17:19:41.000000 jaxsim-0.1.dev153/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:19:55.367683 jaxsim-0.1.dev153/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:19:55.371683 jaxsim-0.1.dev153/src/jaxsim/
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-05-05 17:19:41.000000 jaxsim-0.1.dev153/src/jaxsim/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:19:55.371683 jaxsim-0.1.dev153/src/jaxsim/high_level/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-05 17:19:41.000000 jaxsim-0.1.dev153/src/jaxsim/high_level/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-05 17:19:41.000000 jaxsim-0.1.dev153/src/jaxsim/high_level/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-05-05 17:19:41.000000 jaxsim-0.1.dev153/src/jaxsim/high_level/joint.py
--rw-r--r--   0 runner    (1001) docker     (123)     8239 2023-05-05 17:19:41.000000 jaxsim-0.1.dev153/src/jaxsim/high_level/link.py
--rw-r--r--   0 runner    (1001) docker     (123)    37704 2023-05-05 17:19:41.000000 jaxsim-0.1.dev153/src/jaxsim/high_level/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-05-05 17:19:41.000000 jaxsim-0.1.dev153/src/jaxsim/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:19:55.375684 jaxsim-0.1.dev153/src/jaxsim/math/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 17:19:41.000000 jaxsim-0.1.dev153/src/jaxsim/math/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-05-05 17:19:41.000000 jaxsim-0.1.dev153/src/jaxsim/math/adjoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-05-05 17:19:41.000000 jaxsim-0.1.dev153/src/jaxsim/math/conv.py
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-05 17:19:41.000000 jaxsim-0.1.dev153/src/jaxsim/math/cross.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-05 17:19:41.000000 jaxsim-0.1.dev153/src/jaxsim/math/inertia.py
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-05-05 17:19:41.000000 jaxsim-0.1.dev153/src/jaxsim/math/joint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-05-05 17:19:41.000000 jaxsim-0.1.dev153/src/jaxsim/math/plucker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-05-05 17:19:41.000000 jaxsim-0.1.dev153/src/jaxsim/math/quaternion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-05-05 17:19:41.000000 jaxsim-0.1.dev153/src/jaxsim/math/rotation.py
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-05 17:19:41.000000 jaxsim-0.1.dev153/src/jaxsim/math/skew.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:19:55.375684 jaxsim-0.1.dev153/src/jaxsim/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-05 17:19:41.000000 jaxsim-0.1.dev153/src/jaxsim/parsers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:19:55.375684 jaxsim-0.1.dev153/src/jaxsim/parsers/descriptions/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-05 17:19:41.000000 jaxsim-0.1.dev153/src/jaxsim/parsers/descriptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-05-05 17:19:41.000000 jaxsim-0.1.dev153/src/jaxsim/parsers/descriptions/collision.py
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-05-05 17:19:41.000000 jaxsim-0.1.dev153/src/jaxsim/parsers/descriptions/joint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-05-05 17:19:41.000000 jaxsim-0.1.dev153/src/jaxsim/parsers/descriptions/link.py
--rw-r--r--   0 runner    (1001) docker     (123)     6388 2023-05-05 17:19:41.000000 jaxsim-0.1.dev153/src/jaxsim/parsers/descriptions/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    18763 2023-05-05 17:19:41.000000 jaxsim-0.1.dev153/src/jaxsim/parsers/kinematic_graph.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:19:55.379684 jaxsim-0.1.dev153/src/jaxsim/parsers/rod/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-05 17:19:41.000000 jaxsim-0.1.dev153/src/jaxsim/parsers/rod/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11946 2023-05-05 17:19:41.000000 jaxsim-0.1.dev153/src/jaxsim/parsers/rod/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     6490 2023-05-05 17:19:41.000000 jaxsim-0.1.dev153/src/jaxsim/parsers/rod/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:19:55.379684 jaxsim-0.1.dev153/src/jaxsim/physics/
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-05 17:19:41.000000 jaxsim-0.1.dev153/src/jaxsim/physics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:19:55.379684 jaxsim-0.1.dev153/src/jaxsim/physics/algos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 17:19:41.000000 jaxsim-0.1.dev153/src/jaxsim/physics/algos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6171 2023-05-05 17:19:41.000000 jaxsim-0.1.dev153/src/jaxsim/physics/algos/aba.py
--rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-05-05 17:19:41.000000 jaxsim-0.1.dev153/src/jaxsim/physics/algos/crba.py
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-05-05 17:19:41.000000 jaxsim-0.1.dev153/src/jaxsim/physics/algos/forward_kinematics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-05-05 17:19:41.000000 jaxsim-0.1.dev153/src/jaxsim/physics/algos/jacobian.py
--rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-05-05 17:19:41.000000 jaxsim-0.1.dev153/src/jaxsim/physics/algos/rnea.py
--rw-r--r--   0 runner    (1001) docker     (123)     9094 2023-05-05 17:19:41.000000 jaxsim-0.1.dev153/src/jaxsim/physics/algos/soft_contacts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-05 17:19:41.000000 jaxsim-0.1.dev153/src/jaxsim/physics/algos/terrain.py
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-05-05 17:19:41.000000 jaxsim-0.1.dev153/src/jaxsim/physics/algos/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:19:55.379684 jaxsim-0.1.dev153/src/jaxsim/physics/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 17:19:41.000000 jaxsim-0.1.dev153/src/jaxsim/physics/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-05-05 17:19:41.000000 jaxsim-0.1.dev153/src/jaxsim/physics/model/ground_contact.py
--rw-r--r--   0 runner    (1001) docker     (123)    11075 2023-05-05 17:19:41.000000 jaxsim-0.1.dev153/src/jaxsim/physics/model/physics_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4527 2023-05-05 17:19:41.000000 jaxsim-0.1.dev153/src/jaxsim/physics/model/physics_model_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:19:55.383685 jaxsim-0.1.dev153/src/jaxsim/simulation/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-05 17:19:41.000000 jaxsim-0.1.dev153/src/jaxsim/simulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13779 2023-05-05 17:19:41.000000 jaxsim-0.1.dev153/src/jaxsim/simulation/integrators.py
--rw-r--r--   0 runner    (1001) docker     (123)    10279 2023-05-05 17:19:41.000000 jaxsim-0.1.dev153/src/jaxsim/simulation/ode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-05 17:19:41.000000 jaxsim-0.1.dev153/src/jaxsim/simulation/ode_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4021 2023-05-05 17:19:41.000000 jaxsim-0.1.dev153/src/jaxsim/simulation/ode_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    15860 2023-05-05 17:19:41.000000 jaxsim-0.1.dev153/src/jaxsim/simulation/simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-05-05 17:19:41.000000 jaxsim-0.1.dev153/src/jaxsim/simulation/simulator_callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-05 17:19:41.000000 jaxsim-0.1.dev153/src/jaxsim/simulation/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:19:55.383685 jaxsim-0.1.dev153/src/jaxsim/sixd/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-05 17:19:41.000000 jaxsim-0.1.dev153/src/jaxsim/sixd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-05 17:19:41.000000 jaxsim-0.1.dev153/src/jaxsim/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-05-05 17:19:41.000000 jaxsim-0.1.dev153/src/jaxsim/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:19:55.371683 jaxsim-0.1.dev153/src/jaxsim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-05-05 17:19:55.000000 jaxsim-0.1.dev153/src/jaxsim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-05-05 17:19:55.000000 jaxsim-0.1.dev153/src/jaxsim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 17:19:55.000000 jaxsim-0.1.dev153/src/jaxsim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 17:19:55.000000 jaxsim-0.1.dev153/src/jaxsim.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-05 17:19:55.000000 jaxsim-0.1.dev153/src/jaxsim.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-05 17:19:55.000000 jaxsim-0.1.dev153/src/jaxsim.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:57:32.605342 jaxsim-0.1.dev156/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:57:32.597342 jaxsim-0.1.dev156/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:57:32.597342 jaxsim-0.1.dev156/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/.github/workflows/ci_cd.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/.github/workflows/style.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-06-09 09:57:32.605342 jaxsim-0.1.dev156/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-09 09:57:32.609342 jaxsim-0.1.dev156/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:57:32.597342 jaxsim-0.1.dev156/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:57:32.597342 jaxsim-0.1.dev156/src/jaxsim/
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/src/jaxsim/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:57:32.601342 jaxsim-0.1.dev156/src/jaxsim/high_level/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/src/jaxsim/high_level/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/src/jaxsim/high_level/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/src/jaxsim/high_level/joint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8239 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/src/jaxsim/high_level/link.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37704 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/src/jaxsim/high_level/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/src/jaxsim/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:57:32.601342 jaxsim-0.1.dev156/src/jaxsim/math/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/src/jaxsim/math/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/src/jaxsim/math/adjoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/src/jaxsim/math/conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/src/jaxsim/math/cross.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/src/jaxsim/math/inertia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/src/jaxsim/math/joint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/src/jaxsim/math/plucker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/src/jaxsim/math/quaternion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/src/jaxsim/math/rotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/src/jaxsim/math/skew.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:57:32.601342 jaxsim-0.1.dev156/src/jaxsim/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/src/jaxsim/parsers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:57:32.601342 jaxsim-0.1.dev156/src/jaxsim/parsers/descriptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/src/jaxsim/parsers/descriptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/src/jaxsim/parsers/descriptions/collision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/src/jaxsim/parsers/descriptions/joint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/src/jaxsim/parsers/descriptions/link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6388 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/src/jaxsim/parsers/descriptions/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18763 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/src/jaxsim/parsers/kinematic_graph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:57:32.601342 jaxsim-0.1.dev156/src/jaxsim/parsers/rod/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/src/jaxsim/parsers/rod/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11946 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/src/jaxsim/parsers/rod/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6490 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/src/jaxsim/parsers/rod/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:57:32.605342 jaxsim-0.1.dev156/src/jaxsim/physics/
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/src/jaxsim/physics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:57:32.605342 jaxsim-0.1.dev156/src/jaxsim/physics/algos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/src/jaxsim/physics/algos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6171 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/src/jaxsim/physics/algos/aba.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/src/jaxsim/physics/algos/crba.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/src/jaxsim/physics/algos/forward_kinematics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/src/jaxsim/physics/algos/jacobian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/src/jaxsim/physics/algos/rnea.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9094 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/src/jaxsim/physics/algos/soft_contacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/src/jaxsim/physics/algos/terrain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/src/jaxsim/physics/algos/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:57:32.605342 jaxsim-0.1.dev156/src/jaxsim/physics/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/src/jaxsim/physics/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/src/jaxsim/physics/model/ground_contact.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11075 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/src/jaxsim/physics/model/physics_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4527 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/src/jaxsim/physics/model/physics_model_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:57:32.605342 jaxsim-0.1.dev156/src/jaxsim/simulation/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/src/jaxsim/simulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13779 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/src/jaxsim/simulation/integrators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10279 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/src/jaxsim/simulation/ode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/src/jaxsim/simulation/ode_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4021 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/src/jaxsim/simulation/ode_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15862 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/src/jaxsim/simulation/simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/src/jaxsim/simulation/simulator_callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/src/jaxsim/simulation/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:57:32.605342 jaxsim-0.1.dev156/src/jaxsim/sixd/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/src/jaxsim/sixd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/src/jaxsim/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/src/jaxsim/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:57:32.601342 jaxsim-0.1.dev156/src/jaxsim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-06-09 09:57:32.000000 jaxsim-0.1.dev156/src/jaxsim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-06-09 09:57:32.000000 jaxsim-0.1.dev156/src/jaxsim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 09:57:32.000000 jaxsim-0.1.dev156/src/jaxsim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 09:57:32.000000 jaxsim-0.1.dev156/src/jaxsim.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-09 09:57:32.000000 jaxsim-0.1.dev156/src/jaxsim.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-09 09:57:32.000000 jaxsim-0.1.dev156/src/jaxsim.egg-info/top_level.txt
```

### Comparing `jaxsim-0.1.dev153/.github/workflows/ci_cd.yml` & `jaxsim-0.1.dev156/.github/workflows/ci_cd.yml`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev153/.github/workflows/style.yml` & `jaxsim-0.1.dev156/.github/workflows/style.yml`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev153/.gitignore` & `jaxsim-0.1.dev156/.gitignore`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev153/LICENSE` & `jaxsim-0.1.dev156/LICENSE`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev153/PKG-INFO` & `jaxsim-0.1.dev156/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaxsim
-Version: 0.1.dev153
+Version: 0.1.dev156
 Summary: A physics engine in reduced coordinates implemented with JAX.
 Home-page: https://github.com/ami-iit/jaxsim
 Author: Diego Ferigo
 Author-email: diego.ferigo@iit.it
 License: BSD
 Project-URL: Changelog, https://github.com/ami-iit/jaxsim/releases
 Project-URL: Source, https://github.com/ami-iit/jaxsim
```

### Comparing `jaxsim-0.1.dev153/README.md` & `jaxsim-0.1.dev156/README.md`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev153/setup.cfg` & `jaxsim-0.1.dev156/setup.cfg`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev153/src/jaxsim/__init__.py` & `jaxsim-0.1.dev156/src/jaxsim/__init__.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev153/src/jaxsim/high_level/joint.py` & `jaxsim-0.1.dev156/src/jaxsim/high_level/joint.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev153/src/jaxsim/high_level/link.py` & `jaxsim-0.1.dev156/src/jaxsim/high_level/link.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev153/src/jaxsim/high_level/model.py` & `jaxsim-0.1.dev156/src/jaxsim/high_level/model.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev153/src/jaxsim/logging.py` & `jaxsim-0.1.dev156/src/jaxsim/logging.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev153/src/jaxsim/math/adjoint.py` & `jaxsim-0.1.dev156/src/jaxsim/math/adjoint.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev153/src/jaxsim/math/conv.py` & `jaxsim-0.1.dev156/src/jaxsim/math/conv.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev153/src/jaxsim/math/cross.py` & `jaxsim-0.1.dev156/src/jaxsim/math/cross.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev153/src/jaxsim/math/inertia.py` & `jaxsim-0.1.dev156/src/jaxsim/math/inertia.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev153/src/jaxsim/math/joint.py` & `jaxsim-0.1.dev156/src/jaxsim/math/joint.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev153/src/jaxsim/math/plucker.py` & `jaxsim-0.1.dev156/src/jaxsim/math/plucker.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev153/src/jaxsim/math/quaternion.py` & `jaxsim-0.1.dev156/src/jaxsim/math/quaternion.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev153/src/jaxsim/math/rotation.py` & `jaxsim-0.1.dev156/src/jaxsim/math/rotation.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev153/src/jaxsim/math/skew.py` & `jaxsim-0.1.dev156/src/jaxsim/math/skew.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev153/src/jaxsim/parsers/descriptions/collision.py` & `jaxsim-0.1.dev156/src/jaxsim/parsers/descriptions/collision.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev153/src/jaxsim/parsers/descriptions/joint.py` & `jaxsim-0.1.dev156/src/jaxsim/parsers/descriptions/joint.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev153/src/jaxsim/parsers/descriptions/link.py` & `jaxsim-0.1.dev156/src/jaxsim/parsers/descriptions/link.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev153/src/jaxsim/parsers/descriptions/model.py` & `jaxsim-0.1.dev156/src/jaxsim/parsers/descriptions/model.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev153/src/jaxsim/parsers/kinematic_graph.py` & `jaxsim-0.1.dev156/src/jaxsim/parsers/kinematic_graph.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev153/src/jaxsim/parsers/rod/parser.py` & `jaxsim-0.1.dev156/src/jaxsim/parsers/rod/parser.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev153/src/jaxsim/parsers/rod/utils.py` & `jaxsim-0.1.dev156/src/jaxsim/parsers/rod/utils.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev153/src/jaxsim/physics/algos/aba.py` & `jaxsim-0.1.dev156/src/jaxsim/physics/algos/aba.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev153/src/jaxsim/physics/algos/crba.py` & `jaxsim-0.1.dev156/src/jaxsim/physics/algos/crba.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev153/src/jaxsim/physics/algos/forward_kinematics.py` & `jaxsim-0.1.dev156/src/jaxsim/physics/algos/forward_kinematics.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev153/src/jaxsim/physics/algos/jacobian.py` & `jaxsim-0.1.dev156/src/jaxsim/physics/algos/jacobian.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev153/src/jaxsim/physics/algos/rnea.py` & `jaxsim-0.1.dev156/src/jaxsim/physics/algos/rnea.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev153/src/jaxsim/physics/algos/soft_contacts.py` & `jaxsim-0.1.dev156/src/jaxsim/physics/algos/soft_contacts.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev153/src/jaxsim/physics/algos/terrain.py` & `jaxsim-0.1.dev156/src/jaxsim/physics/algos/terrain.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev153/src/jaxsim/physics/algos/utils.py` & `jaxsim-0.1.dev156/src/jaxsim/physics/algos/utils.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev153/src/jaxsim/physics/model/ground_contact.py` & `jaxsim-0.1.dev156/src/jaxsim/physics/model/ground_contact.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev153/src/jaxsim/physics/model/physics_model.py` & `jaxsim-0.1.dev156/src/jaxsim/physics/model/physics_model.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev153/src/jaxsim/physics/model/physics_model_state.py` & `jaxsim-0.1.dev156/src/jaxsim/physics/model/physics_model_state.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev153/src/jaxsim/simulation/integrators.py` & `jaxsim-0.1.dev156/src/jaxsim/simulation/integrators.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev153/src/jaxsim/simulation/ode.py` & `jaxsim-0.1.dev156/src/jaxsim/simulation/ode.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev153/src/jaxsim/simulation/ode_data.py` & `jaxsim-0.1.dev156/src/jaxsim/simulation/ode_data.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev153/src/jaxsim/simulation/ode_integration.py` & `jaxsim-0.1.dev156/src/jaxsim/simulation/ode_integration.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev153/src/jaxsim/simulation/simulator.py` & `jaxsim-0.1.dev156/src/jaxsim/simulation/simulator.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     """
     Data used by the simulator.
 
     It can be used as JaxSim state in a functional programming style.
     """
 
     # Simulation time stored in ns in order to prevent floats approximation
-    time_ns: jtp.Int = jnp.array(0, dtype=jnp.int64)
+    time_ns: jtp.Int = jnp.array(0, dtype=jnp.uint64)
 
     # Terrain and contact parameters
     terrain: Terrain = jax_dataclasses.field(default_factory=lambda: FlatTerrain())
     contact_parameters: SoftContactsParams = jax_dataclasses.field(
         default_factory=lambda: SoftContactsParams()
     )
 
@@ -50,15 +50,15 @@
 
 @jax_dataclasses.pytree_dataclass
 class JaxSim(JaxsimDataclass):
     """The JaxSim simulator."""
 
     # Step size stored in ns in order to prevent floats approximation
     step_size_ns: jtp.Int = jax_dataclasses.field(
-        default_factory=lambda: jnp.array(1_000_000, dtype=jnp.int64)
+        default_factory=lambda: jnp.array(1_000_000, dtype=jnp.uint64)
     )
 
     # Number of sub-steps performed at each integration step.
     # Note: there is no collision detection performed in sub-steps.
     steps_per_run: jtp.Int = jax_dataclasses.static_field(default=1)
 
     # Default velocity representation (could be overridden for individual models)
@@ -91,15 +91,15 @@
             simulator_data: Optional simulator data to initialize the simulator state.
 
         Returns:
             The JaxSim simulator object.
         """
 
         return JaxSim(
-            step_size_ns=jnp.array(step_size * 1e9, dtype=jnp.int64),
+            step_size_ns=jnp.array(step_size * 1e9, dtype=jnp.uint64),
             steps_per_run=int(steps_per_run),
             velocity_representation=velocity_representation,
             integrator_type=integrator_type,
             data=simulator_data if simulator_data is not None else SimulatorData(),
         )
 
     def reset(self, remove_models: bool = True) -> None:
@@ -122,15 +122,15 @@
         """
         Set the integration step size.
 
         Args:
             step_size: The integration step size in seconds.
         """
 
-        self.step_size_ns = jnp.array(step_size * 1e9, dtype=jnp.int64)
+        self.step_size_ns = jnp.array(step_size * 1e9, dtype=jnp.uint64)
 
     def dt(self) -> jtp.Float:
         """
         Return the integration step size in seconds.
 
         Returns:
             The integration step size in seconds.
@@ -344,16 +344,16 @@
             clear_inputs: Zero the inputs of the models after the integration.
 
         Returns:
             A dictionary containing the StepData of all models.
         """
 
         # Compute the initial and final time of the integration as integers
-        t0_ns = jnp.array(self.data.time_ns, dtype=jnp.int64)
-        dt_ns = jnp.array(self.step_size_ns * self.steps_per_run, dtype=jnp.int64)
+        t0_ns = jnp.array(self.data.time_ns, dtype=jnp.uint64)
+        dt_ns = jnp.array(self.step_size_ns * self.steps_per_run, dtype=jnp.uint64)
 
         # Compute the final time using integer arithmetics
         tf_ns = t0_ns + dt_ns
 
         # We collect the StepData of all models
         step_data = dict()
 
@@ -370,27 +370,25 @@
                     terrain=self.data.terrain,
                     contact_parameters=self.data.contact_parameters,
                     clear_inputs=clear_inputs,
                 )
 
             self.data.models[model.name()].data = integrated_model.data
 
+        # Store the final time
         self.data.time_ns += dt_ns
 
         self._set_mutability(self._mutability())
         return step_data
 
     @functools.partial(jax.jit, static_argnames=["horizon_steps"])
     def step_over_horizon(
         self,
         horizon_steps: jtp.Int,
-        callback_handler: Union[
-            "scb.SimulatorCallback",
-            "scb.CallbackHandler",
-        ] = None,
+        callback_handler: Union["scb.SimulatorCallback", "scb.CallbackHandler"] = None,
         clear_inputs: jtp.Bool = False,
     ) -> Union["JaxSim", Tuple["JaxSim", Tuple["scb.SimulatorCallback", jtp.PyTree]]]:
         """
         Advance the simulation by a given number of steps.
 
         Args:
             horizon_steps: The number of steps to advance the simulation.
```

### Comparing `jaxsim-0.1.dev153/src/jaxsim/simulation/simulator_callbacks.py` & `jaxsim-0.1.dev156/src/jaxsim/simulation/simulator_callbacks.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev153/src/jaxsim/typing.py` & `jaxsim-0.1.dev156/src/jaxsim/typing.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,24 @@
 
 import jax.numpy as jnp
 import numpy as np
 import numpy.typing as npt
 
 # JAX types
 FloatJax = Union[jnp.float16, jnp.float32, jnp.float64]
-IntJax = Union[jnp.int8, jnp.int16, jnp.int32, jnp.int64]
+IntJax = Union[
+    jnp.int8,
+    jnp.int16,
+    jnp.int32,
+    jnp.int64,
+    jnp.uint8,
+    jnp.uint16,
+    jnp.uint32,
+    jnp.uint64,
+]
 ArrayJax = jnp.ndarray
 TensorJax = jnp.ndarray
 VectorJax = ArrayJax
 MatrixJax = ArrayJax
 PyTree = Union[
     TensorJax,
     Dict[Hashable, "PyTree"],
```

### Comparing `jaxsim-0.1.dev153/src/jaxsim/utils.py` & `jaxsim-0.1.dev156/src/jaxsim/utils.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev153/src/jaxsim.egg-info/PKG-INFO` & `jaxsim-0.1.dev156/src/jaxsim.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaxsim
-Version: 0.1.dev153
+Version: 0.1.dev156
 Summary: A physics engine in reduced coordinates implemented with JAX.
 Home-page: https://github.com/ami-iit/jaxsim
 Author: Diego Ferigo
 Author-email: diego.ferigo@iit.it
 License: BSD
 Project-URL: Changelog, https://github.com/ami-iit/jaxsim/releases
 Project-URL: Source, https://github.com/ami-iit/jaxsim
```

### Comparing `jaxsim-0.1.dev153/src/jaxsim.egg-info/SOURCES.txt` & `jaxsim-0.1.dev156/src/jaxsim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

