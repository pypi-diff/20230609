# Comparing `tmp/jaxsim-0.1.dev156.tar.gz` & `tmp/jaxsim-0.1.dev164.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaxsim-0.1.dev156.tar", last modified: Fri Jun  9 09:57:32 2023, max compression
+gzip compressed data, was "jaxsim-0.1.dev164.tar", last modified: Fri Jun  9 10:24:56 2023, max compression
```

## Comparing `jaxsim-0.1.dev156.tar` & `jaxsim-0.1.dev164.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:57:32.605342 jaxsim-0.1.dev156/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:57:32.597342 jaxsim-0.1.dev156/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:57:32.597342 jaxsim-0.1.dev156/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/.github/workflows/ci_cd.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/.github/workflows/style.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-06-09 09:57:32.605342 jaxsim-0.1.dev156/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-09 09:57:32.609342 jaxsim-0.1.dev156/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:57:32.597342 jaxsim-0.1.dev156/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:57:32.597342 jaxsim-0.1.dev156/src/jaxsim/
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/src/jaxsim/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:57:32.601342 jaxsim-0.1.dev156/src/jaxsim/high_level/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/src/jaxsim/high_level/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/src/jaxsim/high_level/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/src/jaxsim/high_level/joint.py
--rw-r--r--   0 runner    (1001) docker     (123)     8239 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/src/jaxsim/high_level/link.py
--rw-r--r--   0 runner    (1001) docker     (123)    37704 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/src/jaxsim/high_level/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/src/jaxsim/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:57:32.601342 jaxsim-0.1.dev156/src/jaxsim/math/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/src/jaxsim/math/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/src/jaxsim/math/adjoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/src/jaxsim/math/conv.py
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/src/jaxsim/math/cross.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/src/jaxsim/math/inertia.py
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/src/jaxsim/math/joint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/src/jaxsim/math/plucker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/src/jaxsim/math/quaternion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/src/jaxsim/math/rotation.py
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/src/jaxsim/math/skew.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:57:32.601342 jaxsim-0.1.dev156/src/jaxsim/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/src/jaxsim/parsers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:57:32.601342 jaxsim-0.1.dev156/src/jaxsim/parsers/descriptions/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/src/jaxsim/parsers/descriptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/src/jaxsim/parsers/descriptions/collision.py
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/src/jaxsim/parsers/descriptions/joint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/src/jaxsim/parsers/descriptions/link.py
--rw-r--r--   0 runner    (1001) docker     (123)     6388 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/src/jaxsim/parsers/descriptions/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    18763 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/src/jaxsim/parsers/kinematic_graph.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:57:32.601342 jaxsim-0.1.dev156/src/jaxsim/parsers/rod/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/src/jaxsim/parsers/rod/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11946 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/src/jaxsim/parsers/rod/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     6490 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/src/jaxsim/parsers/rod/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:57:32.605342 jaxsim-0.1.dev156/src/jaxsim/physics/
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/src/jaxsim/physics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:57:32.605342 jaxsim-0.1.dev156/src/jaxsim/physics/algos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/src/jaxsim/physics/algos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6171 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/src/jaxsim/physics/algos/aba.py
--rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/src/jaxsim/physics/algos/crba.py
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/src/jaxsim/physics/algos/forward_kinematics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/src/jaxsim/physics/algos/jacobian.py
--rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/src/jaxsim/physics/algos/rnea.py
--rw-r--r--   0 runner    (1001) docker     (123)     9094 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/src/jaxsim/physics/algos/soft_contacts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/src/jaxsim/physics/algos/terrain.py
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/src/jaxsim/physics/algos/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:57:32.605342 jaxsim-0.1.dev156/src/jaxsim/physics/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/src/jaxsim/physics/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/src/jaxsim/physics/model/ground_contact.py
--rw-r--r--   0 runner    (1001) docker     (123)    11075 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/src/jaxsim/physics/model/physics_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4527 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/src/jaxsim/physics/model/physics_model_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:57:32.605342 jaxsim-0.1.dev156/src/jaxsim/simulation/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/src/jaxsim/simulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13779 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/src/jaxsim/simulation/integrators.py
--rw-r--r--   0 runner    (1001) docker     (123)    10279 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/src/jaxsim/simulation/ode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/src/jaxsim/simulation/ode_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4021 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/src/jaxsim/simulation/ode_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    15862 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/src/jaxsim/simulation/simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/src/jaxsim/simulation/simulator_callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/src/jaxsim/simulation/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:57:32.605342 jaxsim-0.1.dev156/src/jaxsim/sixd/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/src/jaxsim/sixd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/src/jaxsim/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-06-09 09:57:17.000000 jaxsim-0.1.dev156/src/jaxsim/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:57:32.601342 jaxsim-0.1.dev156/src/jaxsim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-06-09 09:57:32.000000 jaxsim-0.1.dev156/src/jaxsim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-06-09 09:57:32.000000 jaxsim-0.1.dev156/src/jaxsim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 09:57:32.000000 jaxsim-0.1.dev156/src/jaxsim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 09:57:32.000000 jaxsim-0.1.dev156/src/jaxsim.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-09 09:57:32.000000 jaxsim-0.1.dev156/src/jaxsim.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-09 09:57:32.000000 jaxsim-0.1.dev156/src/jaxsim.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:24:56.910701 jaxsim-0.1.dev164/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:24:56.898701 jaxsim-0.1.dev164/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:24:56.902701 jaxsim-0.1.dev164/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/.github/workflows/ci_cd.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/.github/workflows/style.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-06-09 10:24:56.910701 jaxsim-0.1.dev164/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-09 10:24:56.910701 jaxsim-0.1.dev164/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:24:56.898701 jaxsim-0.1.dev164/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:24:56.902701 jaxsim-0.1.dev164/src/jaxsim/
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/src/jaxsim/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:24:56.902701 jaxsim-0.1.dev164/src/jaxsim/high_level/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/src/jaxsim/high_level/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/src/jaxsim/high_level/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/src/jaxsim/high_level/joint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8241 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/src/jaxsim/high_level/link.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39231 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/src/jaxsim/high_level/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/src/jaxsim/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:24:56.902701 jaxsim-0.1.dev164/src/jaxsim/math/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/src/jaxsim/math/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/src/jaxsim/math/adjoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/src/jaxsim/math/conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/src/jaxsim/math/cross.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/src/jaxsim/math/inertia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/src/jaxsim/math/joint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/src/jaxsim/math/plucker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/src/jaxsim/math/quaternion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/src/jaxsim/math/rotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/src/jaxsim/math/skew.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:24:56.906701 jaxsim-0.1.dev164/src/jaxsim/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/src/jaxsim/parsers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:24:56.906701 jaxsim-0.1.dev164/src/jaxsim/parsers/descriptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/src/jaxsim/parsers/descriptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/src/jaxsim/parsers/descriptions/collision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/src/jaxsim/parsers/descriptions/joint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/src/jaxsim/parsers/descriptions/link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6388 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/src/jaxsim/parsers/descriptions/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18763 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/src/jaxsim/parsers/kinematic_graph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:24:56.906701 jaxsim-0.1.dev164/src/jaxsim/parsers/rod/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/src/jaxsim/parsers/rod/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11946 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/src/jaxsim/parsers/rod/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6490 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/src/jaxsim/parsers/rod/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:24:56.906701 jaxsim-0.1.dev164/src/jaxsim/physics/
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/src/jaxsim/physics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:24:56.906701 jaxsim-0.1.dev164/src/jaxsim/physics/algos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/src/jaxsim/physics/algos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6171 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/src/jaxsim/physics/algos/aba.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/src/jaxsim/physics/algos/crba.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/src/jaxsim/physics/algos/forward_kinematics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/src/jaxsim/physics/algos/jacobian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/src/jaxsim/physics/algos/rnea.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12707 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/src/jaxsim/physics/algos/soft_contacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/src/jaxsim/physics/algos/terrain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/src/jaxsim/physics/algos/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:24:56.906701 jaxsim-0.1.dev164/src/jaxsim/physics/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/src/jaxsim/physics/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/src/jaxsim/physics/model/ground_contact.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11075 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/src/jaxsim/physics/model/physics_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4527 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/src/jaxsim/physics/model/physics_model_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:24:56.910701 jaxsim-0.1.dev164/src/jaxsim/simulation/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/src/jaxsim/simulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13779 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/src/jaxsim/simulation/integrators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10375 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/src/jaxsim/simulation/ode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/src/jaxsim/simulation/ode_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4021 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/src/jaxsim/simulation/ode_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15862 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/src/jaxsim/simulation/simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/src/jaxsim/simulation/simulator_callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/src/jaxsim/simulation/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:24:56.910701 jaxsim-0.1.dev164/src/jaxsim/sixd/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/src/jaxsim/sixd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/src/jaxsim/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/src/jaxsim/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:24:56.902701 jaxsim-0.1.dev164/src/jaxsim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-06-09 10:24:56.000000 jaxsim-0.1.dev164/src/jaxsim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-06-09 10:24:56.000000 jaxsim-0.1.dev164/src/jaxsim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 10:24:56.000000 jaxsim-0.1.dev164/src/jaxsim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 10:24:56.000000 jaxsim-0.1.dev164/src/jaxsim.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-09 10:24:56.000000 jaxsim-0.1.dev164/src/jaxsim.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-09 10:24:56.000000 jaxsim-0.1.dev164/src/jaxsim.egg-info/top_level.txt
```

### Comparing `jaxsim-0.1.dev156/.github/workflows/ci_cd.yml` & `jaxsim-0.1.dev164/.github/workflows/ci_cd.yml`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev156/.github/workflows/style.yml` & `jaxsim-0.1.dev164/.github/workflows/style.yml`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev156/.gitignore` & `jaxsim-0.1.dev164/.gitignore`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev156/LICENSE` & `jaxsim-0.1.dev164/LICENSE`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev156/PKG-INFO` & `jaxsim-0.1.dev164/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaxsim
-Version: 0.1.dev156
+Version: 0.1.dev164
 Summary: A physics engine in reduced coordinates implemented with JAX.
 Home-page: https://github.com/ami-iit/jaxsim
 Author: Diego Ferigo
 Author-email: diego.ferigo@iit.it
 License: BSD
 Project-URL: Changelog, https://github.com/ami-iit/jaxsim/releases
 Project-URL: Source, https://github.com/ami-iit/jaxsim
```

### Comparing `jaxsim-0.1.dev156/README.md` & `jaxsim-0.1.dev164/README.md`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev156/setup.cfg` & `jaxsim-0.1.dev164/setup.cfg`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev156/src/jaxsim/__init__.py` & `jaxsim-0.1.dev164/src/jaxsim/__init__.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev156/src/jaxsim/high_level/joint.py` & `jaxsim-0.1.dev164/src/jaxsim/high_level/joint.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev156/src/jaxsim/high_level/link.py` & `jaxsim-0.1.dev164/src/jaxsim/high_level/link.py`

 * *Files 0% similar despite different names*

```diff
@@ -237,8 +237,8 @@
         self.parent_model.data.model_input.f_ext = (
             self.parent_model.data.model_input.f_ext.at[self.index(), :].set(
                 W_f_ext_current + W_f_ext
             )
         )
 
     def in_contact(self) -> jtp.Bool:
-        return not jnp.allclose(self.external_force(), 0)
+        return self.parent_model.in_contact()[self.index()]
```

### Comparing `jaxsim-0.1.dev156/src/jaxsim/high_level/model.py` & `jaxsim-0.1.dev164/src/jaxsim/high_level/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -398,14 +398,49 @@
 
     def joints(self, joint_names: List[str] = None) -> List[high_level.joint.Joint]:
         if joint_names is None:
             return list(self._joints.values())
 
         return [self._joints[name] for name in joint_names]
 
+    def in_contact(
+        self,
+        link_names: Optional[List[str]] = None,
+        terrain: Terrain = FlatTerrain(),
+    ) -> jtp.Vector:
+        """"""
+
+        link_names = link_names if link_names is not None else self.link_names()
+
+        if set(link_names) - set(self._links.keys()) != set():
+            raise ValueError("One or more link names are not part of the model")
+
+        from jaxsim.physics.algos.soft_contacts import collidable_points_pos_vel
+
+        W_p_Ci, _ = collidable_points_pos_vel(
+            model=self.physics_model,
+            q=self.data.model_state.joint_positions,
+            qd=self.data.model_state.joint_velocities,
+            xfb=self.data.model_state.xfb(),
+        )
+
+        terrain_height = jax.vmap(terrain.height)(W_p_Ci[0, :], W_p_Ci[1, :])
+
+        below_terrain = W_p_Ci[2, :] <= terrain_height
+
+        links_in_contact = jax.vmap(
+            lambda link_index: jnp.where(
+                self.physics_model.gc.body == link_index,
+                below_terrain,
+                jnp.zeros_like(below_terrain, dtype=bool),
+            ).any()
+        )(jnp.array([link.index() for link in self.links(link_names=link_names)]))
+
+        return links_in_contact
+
     # ==================
     # Vectorized methods
     # ==================
 
     def joint_positions(self, joint_names: List[str] = None) -> jtp.Vector:
         if self.dofs() == 0 and (joint_names is None or len(joint_names) == 0):
             return jnp.array([])
@@ -437,14 +472,22 @@
         if self.dofs() == 0 and (joint_names is None or len(joint_names) == 0):
             return jnp.array([])
 
         return self.data.model_state.joint_velocities[
             self._joint_indices(joint_names=joint_names)
         ]
 
+    def joint_generalized_forces_targets(
+        self, joint_names: List[str] = None
+    ) -> jtp.Vector:
+        if self.dofs() == 0 and (joint_names is None or len(joint_names) == 0):
+            return jnp.array([])
+
+        return self.data.model_input.tau[self._joint_indices(joint_names=joint_names)]
+
     def joint_limits(
         self, joint_names: List[str] = None
     ) -> Tuple[jtp.Vector, jtp.Vector]:
         if self.dofs() == 0 and (joint_names is None or len(joint_names) == 0):
             return jnp.array([])
 
         joint_names = joint_names if joint_names is not None else self.joint_names()
```

### Comparing `jaxsim-0.1.dev156/src/jaxsim/logging.py` & `jaxsim-0.1.dev164/src/jaxsim/logging.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev156/src/jaxsim/math/adjoint.py` & `jaxsim-0.1.dev164/src/jaxsim/math/adjoint.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev156/src/jaxsim/math/conv.py` & `jaxsim-0.1.dev164/src/jaxsim/math/conv.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev156/src/jaxsim/math/cross.py` & `jaxsim-0.1.dev164/src/jaxsim/math/cross.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev156/src/jaxsim/math/inertia.py` & `jaxsim-0.1.dev164/src/jaxsim/math/inertia.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev156/src/jaxsim/math/joint.py` & `jaxsim-0.1.dev164/src/jaxsim/math/joint.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev156/src/jaxsim/math/plucker.py` & `jaxsim-0.1.dev164/src/jaxsim/math/plucker.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev156/src/jaxsim/math/quaternion.py` & `jaxsim-0.1.dev164/src/jaxsim/math/quaternion.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev156/src/jaxsim/math/rotation.py` & `jaxsim-0.1.dev164/src/jaxsim/math/rotation.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev156/src/jaxsim/math/skew.py` & `jaxsim-0.1.dev164/src/jaxsim/math/skew.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev156/src/jaxsim/parsers/descriptions/collision.py` & `jaxsim-0.1.dev164/src/jaxsim/parsers/descriptions/collision.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev156/src/jaxsim/parsers/descriptions/joint.py` & `jaxsim-0.1.dev164/src/jaxsim/parsers/descriptions/joint.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev156/src/jaxsim/parsers/descriptions/link.py` & `jaxsim-0.1.dev164/src/jaxsim/parsers/descriptions/link.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev156/src/jaxsim/parsers/descriptions/model.py` & `jaxsim-0.1.dev164/src/jaxsim/parsers/descriptions/model.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev156/src/jaxsim/parsers/kinematic_graph.py` & `jaxsim-0.1.dev164/src/jaxsim/parsers/kinematic_graph.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev156/src/jaxsim/parsers/rod/parser.py` & `jaxsim-0.1.dev164/src/jaxsim/parsers/rod/parser.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev156/src/jaxsim/parsers/rod/utils.py` & `jaxsim-0.1.dev164/src/jaxsim/parsers/rod/utils.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev156/src/jaxsim/physics/algos/aba.py` & `jaxsim-0.1.dev164/src/jaxsim/physics/algos/aba.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev156/src/jaxsim/physics/algos/crba.py` & `jaxsim-0.1.dev164/src/jaxsim/physics/algos/crba.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev156/src/jaxsim/physics/algos/forward_kinematics.py` & `jaxsim-0.1.dev164/src/jaxsim/physics/algos/forward_kinematics.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev156/src/jaxsim/physics/algos/jacobian.py` & `jaxsim-0.1.dev164/src/jaxsim/physics/algos/jacobian.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev156/src/jaxsim/physics/algos/rnea.py` & `jaxsim-0.1.dev164/src/jaxsim/physics/algos/rnea.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev156/src/jaxsim/physics/algos/terrain.py` & `jaxsim-0.1.dev164/src/jaxsim/physics/algos/terrain.py`

 * *Files 11% similar despite different names*

```diff
@@ -33,10 +33,16 @@
         return 0.0
 
 
 @jax_dataclasses.pytree_dataclass
 class PlaneTerrain(Terrain):
     plane_normal: jtp.Vector = jax_dataclasses.field(default=jnp.array([0, 0, 1.0]))
 
+    @staticmethod
+    def build(plane_normal: jtp.Vector) -> "PlaneTerrain":
+        """"""
+
+        return PlaneTerrain(plane_normal=jnp.array(plane_normal, dtype=float))
+
     def height(self, x: float, y: float) -> float:
         a, b, c = self.plane_normal
         return -(a * x + b * x) / c
```

### Comparing `jaxsim-0.1.dev156/src/jaxsim/physics/model/ground_contact.py` & `jaxsim-0.1.dev164/src/jaxsim/physics/model/ground_contact.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev156/src/jaxsim/physics/model/physics_model.py` & `jaxsim-0.1.dev164/src/jaxsim/physics/model/physics_model.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev156/src/jaxsim/physics/model/physics_model_state.py` & `jaxsim-0.1.dev164/src/jaxsim/physics/model/physics_model_state.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev156/src/jaxsim/simulation/integrators.py` & `jaxsim-0.1.dev164/src/jaxsim/simulation/integrators.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev156/src/jaxsim/simulation/ode.py` & `jaxsim-0.1.dev164/src/jaxsim/simulation/ode.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from typing import Any, Dict, Optional, Tuple
 
+import jax
 import jax.numpy as jnp
 import numpy as np
 
 import jaxsim.typing as jtp
 from jaxsim.physics import algos
 from jaxsim.physics.algos.soft_contacts import (
+    SoftContacts,
     SoftContactsParams,
     collidable_points_pos_vel,
-    soft_contacts_model,
 )
 from jaxsim.physics.algos.terrain import FlatTerrain, Terrain
 from jaxsim.physics.model.physics_model import PhysicsModel
 
 from . import ode_data
 
 
@@ -44,22 +45,21 @@
         model=physics_model,
         q=ode_state.physics_model.joint_positions,
         qd=ode_state.physics_model.joint_velocities,
         xfb=ode_state.physics_model.xfb(),
     )
 
     # Compute the forces acting on the collidable points due to contact with
-    # the compliant ground surface
-    contact_forces_points, tangential_deformation_dot, _ = soft_contacts_model(
-        positions=pos_cp,
-        velocities=vel_cp,
-        tangential_deformation=ode_state.soft_contacts.tangential_deformation,
-        soft_contacts_params=soft_contacts_params,
-        terrain=terrain,
-    )
+    # the compliant ground surface. Apply vmap to process all points together.
+    contact_forces_points, tangential_deformation_dot = jax.vmap(
+        SoftContacts(parameters=soft_contacts_params, terrain=terrain).contact_model
+    )(pos_cp.T, vel_cp.T, ode_state.soft_contacts.tangential_deformation.T)
+
+    contact_forces_points = contact_forces_points.T
+    tangential_deformation_dot = tangential_deformation_dot.T
 
     # Initialize the contact forces, one per body
     contact_forces_links = jnp.zeros_like(
         ode_data.ODEInput.zero(physics_model).physics_model.f_ext
     )
 
     # Combine the contact forces of all collidable points belonging to the same body
```

### Comparing `jaxsim-0.1.dev156/src/jaxsim/simulation/ode_data.py` & `jaxsim-0.1.dev164/src/jaxsim/simulation/ode_data.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev156/src/jaxsim/simulation/ode_integration.py` & `jaxsim-0.1.dev164/src/jaxsim/simulation/ode_integration.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev156/src/jaxsim/simulation/simulator.py` & `jaxsim-0.1.dev164/src/jaxsim/simulation/simulator.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev156/src/jaxsim/simulation/simulator_callbacks.py` & `jaxsim-0.1.dev164/src/jaxsim/simulation/simulator_callbacks.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev156/src/jaxsim/typing.py` & `jaxsim-0.1.dev164/src/jaxsim/typing.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev156/src/jaxsim/utils.py` & `jaxsim-0.1.dev164/src/jaxsim/utils.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev156/src/jaxsim.egg-info/PKG-INFO` & `jaxsim-0.1.dev164/src/jaxsim.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaxsim
-Version: 0.1.dev156
+Version: 0.1.dev164
 Summary: A physics engine in reduced coordinates implemented with JAX.
 Home-page: https://github.com/ami-iit/jaxsim
 Author: Diego Ferigo
 Author-email: diego.ferigo@iit.it
 License: BSD
 Project-URL: Changelog, https://github.com/ami-iit/jaxsim/releases
 Project-URL: Source, https://github.com/ami-iit/jaxsim
```

### Comparing `jaxsim-0.1.dev156/src/jaxsim.egg-info/SOURCES.txt` & `jaxsim-0.1.dev164/src/jaxsim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

