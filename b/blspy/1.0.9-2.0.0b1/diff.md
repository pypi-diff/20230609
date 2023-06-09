# Comparing `tmp/blspy-1.0.9.tar.gz` & `tmp/blspy-2.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blspy-1.0.9.tar", last modified: Sun Jan  9 02:34:02 2022, max compression
+gzip compressed data, was "blspy-2.0.0b1.tar", last modified: Fri Jun  9 20:17:22 2023, max compression
```

## Comparing `blspy-1.0.9.tar` & `blspy-2.0.0b1.tar`

### file list

```diff
@@ -1,108 +1,104 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 02:34:02.580163 blspy-1.0.9/
--rw-r--r--   0 runner    (1001) docker     (121)      427 2022-01-09 02:33:43.000000 blspy-1.0.9/.clang-format
--rw-r--r--   0 runner    (1001) docker     (121)      102 2022-01-09 02:33:43.000000 blspy-1.0.9/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 02:34:02.568163 blspy-1.0.9/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 02:34:02.572163 blspy-1.0.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     4025 2022-01-09 02:33:43.000000 blspy-1.0.9/.github/workflows/build-aarch64.yml
--rw-r--r--   0 runner    (1001) docker     (121)     3528 2022-01-09 02:33:43.000000 blspy-1.0.9/.github/workflows/build-m1-wheel.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2008 2022-01-09 02:33:43.000000 blspy-1.0.9/.github/workflows/build-test.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6441 2022-01-09 02:33:43.000000 blspy-1.0.9/.github/workflows/build-wheels.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1997 2022-01-09 02:33:43.000000 blspy-1.0.9/.github/workflows/relic-nightly.yml
--rwxr-xr-x   0 runner    (1001) docker     (121)     1330 2022-01-09 02:33:43.000000 blspy-1.0.9/.github/workflows/stale-issue.yml
--rw-r--r--   0 runner    (1001) docker     (121)      657 2022-01-09 02:33:43.000000 blspy-1.0.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     4036 2022-01-09 02:33:43.000000 blspy-1.0.9/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)    10174 2022-01-09 02:33:43.000000 blspy-1.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      185 2022-01-09 02:33:43.000000 blspy-1.0.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    12301 2022-01-09 02:34:02.580163 blspy-1.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    11966 2022-01-09 02:33:43.000000 blspy-1.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 02:34:02.572163 blspy-1.0.9/blspy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    12301 2022-01-09 02:34:02.000000 blspy-1.0.9/blspy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2364 2022-01-09 02:34:02.000000 blspy-1.0.9/blspy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-09 02:34:02.000000 blspy-1.0.9/blspy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-09 02:34:02.000000 blspy-1.0.9/blspy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-01-09 02:34:02.000000 blspy-1.0.9/blspy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-01-09 02:34:02.000000 blspy-1.0.9/blspy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 02:34:02.572163 blspy-1.0.9/cmake_modules/
--rw-r--r--   0 runner    (1001) docker     (121)     2909 2022-01-09 02:33:43.000000 blspy-1.0.9/cmake_modules/Findgmp.cmake
--rw-r--r--   0 runner    (1001) docker     (121)     9884 2022-01-09 02:33:43.000000 blspy-1.0.9/cmake_modules/Findsodium.cmake
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 02:34:02.568163 blspy-1.0.9/contrib/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 02:34:02.572163 blspy-1.0.9/contrib/gmp-patch-6.2.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1955 2022-01-09 02:33:43.000000 blspy-1.0.9/contrib/gmp-patch-6.2.1/compat.c
--rw-r--r--   0 runner    (1001) docker     (121)    85426 2022-01-09 02:33:43.000000 blspy-1.0.9/contrib/gmp-patch-6.2.1/longlong.h
--rwxr-xr-x   0 runner    (1001) docker     (121)      158 2022-01-09 02:33:43.000000 blspy-1.0.9/emsdk_build.sh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 02:34:02.572163 blspy-1.0.9/js-bindings/
--rw-r--r--   0 runner    (1001) docker     (121)     1543 2022-01-09 02:33:43.000000 blspy-1.0.9/js-bindings/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     6591 2022-01-09 02:33:43.000000 blspy-1.0.9/js-bindings/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     4068 2022-01-09 02:33:43.000000 blspy-1.0.9/js-bindings/blsjs.d.ts
--rw-r--r--   0 runner    (1001) docker     (121)     3157 2022-01-09 02:33:43.000000 blspy-1.0.9/js-bindings/helpers.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     2055 2022-01-09 02:33:43.000000 blspy-1.0.9/js-bindings/helpers.h
--rw-r--r--   0 runner    (1001) docker     (121)     6303 2022-01-09 02:33:43.000000 blspy-1.0.9/js-bindings/jsbindings.cpp
--rw-r--r--   0 runner    (1001) docker     (121)   126245 2022-01-09 02:33:43.000000 blspy-1.0.9/js-bindings/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-01-09 02:33:43.000000 blspy-1.0.9/js-bindings/package.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 02:34:02.572163 blspy-1.0.9/js-bindings/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     4241 2022-01-09 02:33:43.000000 blspy-1.0.9/js-bindings/tests/PrivateKey.spec.js
--rw-r--r--   0 runner    (1001) docker     (121)     2841 2022-01-09 02:33:43.000000 blspy-1.0.9/js-bindings/tests/PublicKey.spec.js
--rw-r--r--   0 runner    (1001) docker     (121)     6686 2022-01-09 02:33:43.000000 blspy-1.0.9/js-bindings/tests/Signature.spec.js
--rw-r--r--   0 runner    (1001) docker     (121)     1632 2022-01-09 02:33:43.000000 blspy-1.0.9/js-bindings/tests/karma.conf.js
--rw-r--r--   0 runner    (1001) docker     (121)      196 2022-01-09 02:33:43.000000 blspy-1.0.9/js-bindings/tests/karma.test.js
--rw-r--r--   0 runner    (1001) docker     (121)    19266 2022-01-09 02:33:43.000000 blspy-1.0.9/js-bindings/tests/test.js
--rw-r--r--   0 runner    (1001) docker     (121)     4098 2022-01-09 02:33:43.000000 blspy-1.0.9/js-bindings/tests/typings.spec.ts
--rw-r--r--   0 runner    (1001) docker     (121)      438 2022-01-09 02:33:43.000000 blspy-1.0.9/js-bindings/tests/webpack.config.js
--rw-r--r--   0 runner    (1001) docker     (121)    13186 2022-01-09 02:33:43.000000 blspy-1.0.9/js-bindings/tests/yarn.lock
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 02:34:02.576163 blspy-1.0.9/js-bindings/wrappers/
--rw-r--r--   0 runner    (1001) docker     (121)     1461 2022-01-09 02:33:43.000000 blspy-1.0.9/js-bindings/wrappers/BignumWrapper.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     1190 2022-01-09 02:33:43.000000 blspy-1.0.9/js-bindings/wrappers/BignumWrapper.h
--rw-r--r--   0 runner    (1001) docker     (121)     2679 2022-01-09 02:33:43.000000 blspy-1.0.9/js-bindings/wrappers/G1ElementWrapper.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     1522 2022-01-09 02:33:43.000000 blspy-1.0.9/js-bindings/wrappers/G1ElementWrapper.h
--rw-r--r--   0 runner    (1001) docker     (121)     3048 2022-01-09 02:33:43.000000 blspy-1.0.9/js-bindings/wrappers/G2ElementWrapper.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     1627 2022-01-09 02:33:43.000000 blspy-1.0.9/js-bindings/wrappers/G2ElementWrapper.h
--rw-r--r--   0 runner    (1001) docker     (121)     1004 2022-01-09 02:33:43.000000 blspy-1.0.9/js-bindings/wrappers/JSWrapper.h
--rw-r--r--   0 runner    (1001) docker     (121)     2823 2022-01-09 02:33:43.000000 blspy-1.0.9/js-bindings/wrappers/PrivateKeyWrapper.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     1675 2022-01-09 02:33:43.000000 blspy-1.0.9/js-bindings/wrappers/PrivateKeyWrapper.h
--rw-r--r--   0 runner    (1001) docker     (121)      698 2022-01-09 02:33:43.000000 blspy-1.0.9/js-bindings/wrappers/SchemeMPLWrapper.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     4718 2022-01-09 02:33:43.000000 blspy-1.0.9/js-bindings/wrappers/SchemeMPLWrapper.h
--rw-r--r--   0 runner    (1001) docker     (121)     1087 2022-01-09 02:33:43.000000 blspy-1.0.9/js-bindings/wrappers/UtilWrapper.cpp
--rw-r--r--   0 runner    (1001) docker     (121)      966 2022-01-09 02:33:43.000000 blspy-1.0.9/js-bindings/wrappers/UtilWrapper.h
--rwxr-xr-x   0 runner    (1001) docker     (121)      219 2022-01-09 02:33:43.000000 blspy-1.0.9/js_build.sh
--rwxr-xr-x   0 runner    (1001) docker     (121)      272 2022-01-09 02:33:43.000000 blspy-1.0.9/js_test.sh
--rw-r--r--   0 runner    (1001) docker     (121)      509 2022-01-09 02:33:43.000000 blspy-1.0.9/lgtm.yml
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-01-09 02:33:43.000000 blspy-1.0.9/mypi.ini
--rw-r--r--   0 runner    (1001) docker     (121)      194 2022-01-09 02:33:43.000000 blspy-1.0.9/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 02:34:02.576163 blspy-1.0.9/python-bindings/
--rw-r--r--   0 runner    (1001) docker     (121)      275 2022-01-09 02:33:43.000000 blspy-1.0.9/python-bindings/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4634 2022-01-09 02:33:43.000000 blspy-1.0.9/python-bindings/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     1581 2022-01-09 02:33:43.000000 blspy-1.0.9/python-bindings/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (121)    25093 2022-01-09 02:33:43.000000 blspy-1.0.9/python-bindings/pythonbindings.cpp
--rw-r--r--   0 runner    (1001) docker     (121)    16111 2022-01-09 02:33:43.000000 blspy-1.0.9/python-bindings/test.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 02:34:02.576163 blspy-1.0.9/python-impl/
--rw-r--r--   0 runner    (1001) docker     (121)      601 2022-01-09 02:33:43.000000 blspy-1.0.9/python-impl/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     3381 2022-01-09 02:33:43.000000 blspy-1.0.9/python-impl/bls12381.py
--rw-r--r--   0 runner    (1001) docker     (121)    17103 2022-01-09 02:33:43.000000 blspy-1.0.9/python-impl/ec.py
--rw-r--r--   0 runner    (1001) docker     (121)    21950 2022-01-09 02:33:43.000000 blspy-1.0.9/python-impl/fields.py
--rw-r--r--   0 runner    (1001) docker     (121)     3167 2022-01-09 02:33:43.000000 blspy-1.0.9/python-impl/hash_to_field.py
--rw-r--r--   0 runner    (1001) docker     (121)     3314 2022-01-09 02:33:43.000000 blspy-1.0.9/python-impl/hd_keys.py
--rw-r--r--   0 runner    (1001) docker     (121)     1494 2022-01-09 02:33:43.000000 blspy-1.0.9/python-impl/hkdf.py
--rw-r--r--   0 runner    (1001) docker     (121)    25025 2022-01-09 02:33:43.000000 blspy-1.0.9/python-impl/impl-test.py
--rw-r--r--   0 runner    (1001) docker     (121)     7351 2022-01-09 02:33:43.000000 blspy-1.0.9/python-impl/op_swu_g2.py
--rw-r--r--   0 runner    (1001) docker     (121)     3886 2022-01-09 02:33:43.000000 blspy-1.0.9/python-impl/pairing.py
--rw-r--r--   0 runner    (1001) docker     (121)     2176 2022-01-09 02:33:43.000000 blspy-1.0.9/python-impl/private_key.py
--rw-r--r--   0 runner    (1001) docker     (121)     7066 2022-01-09 02:33:43.000000 blspy-1.0.9/python-impl/schemes.py
--rw-r--r--   0 runner    (1001) docker     (121)     1431 2022-01-09 02:33:43.000000 blspy-1.0.9/python-impl/util.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-01-09 02:34:02.580163 blspy-1.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     6953 2022-01-09 02:33:43.000000 blspy-1.0.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 02:34:02.580163 blspy-1.0.9/src/
--rw-r--r--   0 runner    (1001) docker     (121)     1272 2022-01-09 02:33:43.000000 blspy-1.0.9/src/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2158 2022-01-09 02:33:43.000000 blspy-1.0.9/src/bls.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     1238 2022-01-09 02:33:43.000000 blspy-1.0.9/src/bls.hpp
--rw-r--r--   0 runner    (1001) docker     (121)    12142 2022-01-09 02:33:43.000000 blspy-1.0.9/src/elements.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     4523 2022-01-09 02:33:43.000000 blspy-1.0.9/src/elements.hpp
--rw-r--r--   0 runner    (1001) docker     (121)     7562 2022-01-09 02:33:43.000000 blspy-1.0.9/src/hdkeys.hpp
--rw-r--r--   0 runner    (1001) docker     (121)     3446 2022-01-09 02:33:43.000000 blspy-1.0.9/src/hkdf.hpp
--rw-r--r--   0 runner    (1001) docker     (121)     6146 2022-01-09 02:33:43.000000 blspy-1.0.9/src/privatekey.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     3338 2022-01-09 02:33:43.000000 blspy-1.0.9/src/privatekey.hpp
--rw-r--r--   0 runner    (1001) docker     (121)    19410 2022-01-09 02:33:43.000000 blspy-1.0.9/src/schemes.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     7716 2022-01-09 02:33:43.000000 blspy-1.0.9/src/schemes.hpp
--rw-r--r--   0 runner    (1001) docker     (121)     4626 2022-01-09 02:33:43.000000 blspy-1.0.9/src/test-bench.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     1814 2022-01-09 02:33:43.000000 blspy-1.0.9/src/test-utils.hpp
--rw-r--r--   0 runner    (1001) docker     (121)    51776 2022-01-09 02:33:43.000000 blspy-1.0.9/src/test.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     4570 2022-01-09 02:33:43.000000 blspy-1.0.9/src/util.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:17:22.963346 blspy-2.0.0b1/
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-09 20:17:13.000000 blspy-2.0.0b1/.clang-format
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-09 20:17:13.000000 blspy-2.0.0b1/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:17:22.951346 blspy-2.0.0b1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:17:22.955346 blspy-2.0.0b1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-06-09 20:17:13.000000 blspy-2.0.0b1/.github/workflows/build-test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    10271 2023-06-09 20:17:13.000000 blspy-2.0.0b1/.github/workflows/build-wheels.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-06-09 20:17:13.000000 blspy-2.0.0b1/.github/workflows/js-bindings.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-06-09 20:17:13.000000 blspy-2.0.0b1/.github/workflows/stale-issue.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-06-09 20:17:13.000000 blspy-2.0.0b1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-06-09 20:17:13.000000 blspy-2.0.0b1/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-06-09 20:17:13.000000 blspy-2.0.0b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-09 20:17:13.000000 blspy-2.0.0b1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    12265 2023-06-09 20:17:22.963346 blspy-2.0.0b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11965 2023-06-09 20:17:13.000000 blspy-2.0.0b1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:17:22.955346 blspy-2.0.0b1/blspy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12265 2023-06-09 20:17:22.000000 blspy-2.0.0b1/blspy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-06-09 20:17:22.000000 blspy-2.0.0b1/blspy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 20:17:22.000000 blspy-2.0.0b1/blspy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 20:17:22.000000 blspy-2.0.0b1/blspy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-09 20:17:22.000000 blspy-2.0.0b1/blspy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-09 20:17:22.000000 blspy-2.0.0b1/blspy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:17:22.955346 blspy-2.0.0b1/cmake_modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     9884 2023-06-09 20:17:13.000000 blspy-2.0.0b1/cmake_modules/Findsodium.cmake
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:17:22.951346 blspy-2.0.0b1/contrib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:17:22.955346 blspy-2.0.0b1/contrib/gmp-patch-6.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-06-09 20:17:13.000000 blspy-2.0.0b1/contrib/gmp-patch-6.2.1/compat.c
+-rw-r--r--   0 runner    (1001) docker     (123)    85426 2023-06-09 20:17:13.000000 blspy-2.0.0b1/contrib/gmp-patch-6.2.1/longlong.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)      158 2023-06-09 20:17:13.000000 blspy-2.0.0b1/emsdk_build.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:17:22.955346 blspy-2.0.0b1/js-bindings/
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-06-09 20:17:13.000000 blspy-2.0.0b1/js-bindings/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6591 2023-06-09 20:17:13.000000 blspy-2.0.0b1/js-bindings/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-06-09 20:17:13.000000 blspy-2.0.0b1/js-bindings/blsjs.d.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-06-09 20:17:13.000000 blspy-2.0.0b1/js-bindings/helpers.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-06-09 20:17:13.000000 blspy-2.0.0b1/js-bindings/helpers.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5939 2023-06-09 20:17:13.000000 blspy-2.0.0b1/js-bindings/jsbindings.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)   126728 2023-06-09 20:17:13.000000 blspy-2.0.0b1/js-bindings/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-06-09 20:17:13.000000 blspy-2.0.0b1/js-bindings/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:17:22.959346 blspy-2.0.0b1/js-bindings/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-06-09 20:17:13.000000 blspy-2.0.0b1/js-bindings/tests/PrivateKey.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-06-09 20:17:13.000000 blspy-2.0.0b1/js-bindings/tests/PublicKey.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6686 2023-06-09 20:17:13.000000 blspy-2.0.0b1/js-bindings/tests/Signature.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-06-09 20:17:13.000000 blspy-2.0.0b1/js-bindings/tests/karma.conf.js
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-09 20:17:13.000000 blspy-2.0.0b1/js-bindings/tests/karma.test.js
+-rw-r--r--   0 runner    (1001) docker     (123)    19006 2023-06-09 20:17:13.000000 blspy-2.0.0b1/js-bindings/tests/test.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-06-09 20:17:13.000000 blspy-2.0.0b1/js-bindings/tests/typings.spec.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-09 20:17:13.000000 blspy-2.0.0b1/js-bindings/tests/webpack.config.js
+-rw-r--r--   0 runner    (1001) docker     (123)    13186 2023-06-09 20:17:13.000000 blspy-2.0.0b1/js-bindings/tests/yarn.lock
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:17:22.959346 blspy-2.0.0b1/js-bindings/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-06-09 20:17:13.000000 blspy-2.0.0b1/js-bindings/wrappers/G1ElementWrapper.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-06-09 20:17:13.000000 blspy-2.0.0b1/js-bindings/wrappers/G1ElementWrapper.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-06-09 20:17:13.000000 blspy-2.0.0b1/js-bindings/wrappers/G2ElementWrapper.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-06-09 20:17:13.000000 blspy-2.0.0b1/js-bindings/wrappers/G2ElementWrapper.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-06-09 20:17:13.000000 blspy-2.0.0b1/js-bindings/wrappers/JSWrapper.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-06-09 20:17:13.000000 blspy-2.0.0b1/js-bindings/wrappers/PrivateKeyWrapper.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-06-09 20:17:13.000000 blspy-2.0.0b1/js-bindings/wrappers/PrivateKeyWrapper.h
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-09 20:17:13.000000 blspy-2.0.0b1/js-bindings/wrappers/SchemeMPLWrapper.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-06-09 20:17:13.000000 blspy-2.0.0b1/js-bindings/wrappers/SchemeMPLWrapper.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-09 20:17:13.000000 blspy-2.0.0b1/js-bindings/wrappers/UtilWrapper.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-09 20:17:13.000000 blspy-2.0.0b1/js-bindings/wrappers/UtilWrapper.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)      219 2023-06-09 20:17:13.000000 blspy-2.0.0b1/js_build.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      272 2023-06-09 20:17:13.000000 blspy-2.0.0b1/js_test.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-09 20:17:13.000000 blspy-2.0.0b1/lgtm.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-09 20:17:13.000000 blspy-2.0.0b1/mypi.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-09 20:17:13.000000 blspy-2.0.0b1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:17:22.959346 blspy-2.0.0b1/python-bindings/
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-09 20:17:13.000000 blspy-2.0.0b1/python-bindings/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-06-09 20:17:13.000000 blspy-2.0.0b1/python-bindings/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-06-09 20:17:13.000000 blspy-2.0.0b1/python-bindings/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29858 2023-06-09 20:17:13.000000 blspy-2.0.0b1/python-bindings/pythonbindings.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    17701 2023-06-09 20:17:13.000000 blspy-2.0.0b1/python-bindings/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:17:22.959346 blspy-2.0.0b1/python-impl/
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-06-09 20:17:13.000000 blspy-2.0.0b1/python-impl/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-06-09 20:17:13.000000 blspy-2.0.0b1/python-impl/bls12381.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17476 2023-06-09 20:17:13.000000 blspy-2.0.0b1/python-impl/ec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21950 2023-06-09 20:17:13.000000 blspy-2.0.0b1/python-impl/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-06-09 20:17:13.000000 blspy-2.0.0b1/python-impl/hash_to_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-06-09 20:17:13.000000 blspy-2.0.0b1/python-impl/hd_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-09 20:17:13.000000 blspy-2.0.0b1/python-impl/hkdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26234 2023-06-09 20:17:13.000000 blspy-2.0.0b1/python-impl/impl-test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7389 2023-06-09 20:17:13.000000 blspy-2.0.0b1/python-impl/op_swu_g2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-06-09 20:17:13.000000 blspy-2.0.0b1/python-impl/pairing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-06-09 20:17:13.000000 blspy-2.0.0b1/python-impl/private_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7066 2023-06-09 20:17:13.000000 blspy-2.0.0b1/python-impl/schemes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-06-09 20:17:13.000000 blspy-2.0.0b1/python-impl/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 20:17:22.963346 blspy-2.0.0b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     6922 2023-06-09 20:17:13.000000 blspy-2.0.0b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:17:22.963346 blspy-2.0.0b1/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-06-09 20:17:13.000000 blspy-2.0.0b1/src/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-06-09 20:17:13.000000 blspy-2.0.0b1/src/bls.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-06-09 20:17:13.000000 blspy-2.0.0b1/src/bls.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)   261840 2023-06-09 20:17:13.000000 blspy-2.0.0b1/src/blstasm.lib
+-rw-r--r--   0 runner    (1001) docker     (123)    11593 2023-06-09 20:17:13.000000 blspy-2.0.0b1/src/elements.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4849 2023-06-09 20:17:13.000000 blspy-2.0.0b1/src/elements.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6488 2023-06-09 20:17:13.000000 blspy-2.0.0b1/src/hdkeys.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-06-09 20:17:13.000000 blspy-2.0.0b1/src/hkdf.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-06-09 20:17:13.000000 blspy-2.0.0b1/src/privatekey.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-06-09 20:17:13.000000 blspy-2.0.0b1/src/privatekey.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    19459 2023-06-09 20:17:13.000000 blspy-2.0.0b1/src/schemes.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7176 2023-06-09 20:17:13.000000 blspy-2.0.0b1/src/schemes.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4842 2023-06-09 20:17:13.000000 blspy-2.0.0b1/src/test-bench.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-06-09 20:17:13.000000 blspy-2.0.0b1/src/test-utils.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    54259 2023-06-09 20:17:13.000000 blspy-2.0.0b1/src/test.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-06-09 20:17:13.000000 blspy-2.0.0b1/src/util.hpp
```

### Comparing `blspy-1.0.9/.github/workflows/build-test.yaml` & `blspy-2.0.0b1/.github/workflows/build-test.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -6,36 +6,59 @@
       - main
     tags:
       - '**'
   pull_request:
     branches:
       - '**'
 
+concurrency:
+  # SHA is added to the end if on `main` to let all main workflows run
+  group: ${{ github.ref }}-${{ github.workflow }}-${{ github.event_name }}-${{ (github.ref == 'refs/heads/main') && github.sha || '' }}
+  cancel-in-progress: true
+
 jobs:
+  coverage:
+    runs-on: ubuntu-latest
+    steps:
+      - name: Checkout code
+        uses: actions/checkout@v3
+      - name: Collect coverage data
+        run: |
+          sudo apt-get update
+          sudo apt-get install lcov -y
+          sudo apt-get install snap -y
+          sudo snap install cmake --classic
+          hash -r
+          cmake -B ../build -DCMAKE_BUILD_TYPE=Debug -DWITH_COVERAGE=1 -DBUILD_BLS_PYTHON_BINDINGS=0 -DBUILD_BLS_BENCHMARKS=0
+          cmake --build ../build -- -j 6
+          ../build/src/runtest
+          lcov --directory ../build --capture --output-file lcov.info
+          lcov --remove lcov.info '*_deps/*' '/usr/*' --output-file lcov.info
+      - name: Upload to Coveralls
+        uses: coverallsapp/github-action@v2
+        if: always()
+        env:
+          COVERALLS_REPO_TOKEN: ${{ secrets.COVERALLS_REPO_TOKEN }}
+        with:
+          path-to-lcov: './lcov.info'
+
   build_wheels:
     name: Build and Test on ${{ matrix.os }} CPython ${{ matrix.python }}
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
-        os: [macos-latest, ubuntu-latest]
-        python: ['3.7', '3.8', '3.9', '3.10']
+        os: [macos-latest, ubuntu-latest, windows-latest]
+        python: ['3.7', '3.8', '3.9', '3.10', '3.11']
 
     steps:
-    - name: Cancel previous runs on the same branch
-      if: ${{ github.ref != 'refs/heads/main' }}
-      uses: styfle/cancel-workflow-action@0.9.1
-      with:
-        access_token: ${{ github.token }}
-
     - name: Checkout code
-      uses: actions/checkout@v2
+      uses: actions/checkout@v3
 
-    - uses: actions/setup-python@v2
-      name: Install Python
+    - uses: chia-network/actions/setup-python@main
       with:
         python-version: ${{ matrix.python }}
 
     - name: Ubuntu build C++ and test with valgrind
       if: startsWith(matrix.os, 'ubuntu')
       run: |
         sudo apt-get update
@@ -67,14 +90,14 @@
         ./src/runtest
 
     - name: Test pure python implementation
       run: |
         python python-impl/impl-test.py
 
     - name: Install emsdk
-      uses: mymindstorm/setup-emsdk@v9
+      uses: mymindstorm/setup-emsdk@v12
 
     - name: Test javascript bindings
       run: |
         emcc -v
         sh emsdk_build.sh
         sh js_test.sh
```

### Comparing `blspy-1.0.9/.github/workflows/stale-issue.yml` & `blspy-2.0.0b1/.github/workflows/stale-issue.yml`

 * *Files identical despite different names*

### Comparing `blspy-1.0.9/.gitignore` & `blspy-2.0.0b1/.gitignore`

 * *Files identical despite different names*

### Comparing `blspy-1.0.9/LICENSE` & `blspy-2.0.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `blspy-1.0.9/PKG-INFO` & `blspy-2.0.0b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: blspy
-Version: 1.0.9
+Version: 2.0.0b1
 Summary: BLS signatures in c++ (python bindings)
 Home-page: https://github.com/Chia-Network/bls-signatures
 Author: Mariano Sorgente
 Author-email: mariano@chia.net
-License: UNKNOWN
-Platform: UNKNOWN
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # BLS Signatures implementation
 
 [![Build and Test C++, Javascript, and Python](https://github.com/Chia-Network/bls-signatures/actions/workflows/build-test.yaml/badge.svg)](https://github.com/Chia-Network/bls-signatures/actions/workflows/build-test.yaml)
@@ -69,15 +67,15 @@
 PrivateKey sk = AugSchemeMPL().KeyGen(seed);
 G1Element pk = sk.GetG1Element();
 
 vector<uint8_t> message = {1, 2, 3, 4, 5};  // Message is passed in as a byte vector
 G2Element signature = AugSchemeMPL().Sign(sk, message);
 
 // Verify the signature
-bool ok = AugSchemeMPL().Verify(pk, message, signature));
+bool ok = AugSchemeMPL().Verify(pk, message, signature);
 ```
 
 ## Serializing keys and signatures to bytes
 
 ```c++
 vector<uint8_t> skBytes = sk.Serialize();
 vector<uint8_t> pkBytes = pk.Serialize();
@@ -306,9 +304,7 @@
 GMP is distributed under the
 [GNU LGPL v3 license](https://www.gnu.org/licenses/lgpl-3.0.html)
 
 ## Relic license
 
 Relic is used with the
 [Apache 2.0 license](https://github.com/relic-toolkit/relic/blob/master/LICENSE.Apache-2.0)
-
-
```

### Comparing `blspy-1.0.9/README.md` & `blspy-2.0.0b1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 PrivateKey sk = AugSchemeMPL().KeyGen(seed);
 G1Element pk = sk.GetG1Element();
 
 vector<uint8_t> message = {1, 2, 3, 4, 5};  // Message is passed in as a byte vector
 G2Element signature = AugSchemeMPL().Sign(sk, message);
 
 // Verify the signature
-bool ok = AugSchemeMPL().Verify(pk, message, signature));
+bool ok = AugSchemeMPL().Verify(pk, message, signature);
 ```
 
 ## Serializing keys and signatures to bytes
 
 ```c++
 vector<uint8_t> skBytes = sk.Serialize();
 vector<uint8_t> pkBytes = pk.Serialize();
```

### Comparing `blspy-1.0.9/blspy.egg-info/PKG-INFO` & `blspy-2.0.0b1/blspy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: blspy
-Version: 1.0.9
+Version: 2.0.0b1
 Summary: BLS signatures in c++ (python bindings)
 Home-page: https://github.com/Chia-Network/bls-signatures
 Author: Mariano Sorgente
 Author-email: mariano@chia.net
-License: UNKNOWN
-Platform: UNKNOWN
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # BLS Signatures implementation
 
 [![Build and Test C++, Javascript, and Python](https://github.com/Chia-Network/bls-signatures/actions/workflows/build-test.yaml/badge.svg)](https://github.com/Chia-Network/bls-signatures/actions/workflows/build-test.yaml)
@@ -69,15 +67,15 @@
 PrivateKey sk = AugSchemeMPL().KeyGen(seed);
 G1Element pk = sk.GetG1Element();
 
 vector<uint8_t> message = {1, 2, 3, 4, 5};  // Message is passed in as a byte vector
 G2Element signature = AugSchemeMPL().Sign(sk, message);
 
 // Verify the signature
-bool ok = AugSchemeMPL().Verify(pk, message, signature));
+bool ok = AugSchemeMPL().Verify(pk, message, signature);
 ```
 
 ## Serializing keys and signatures to bytes
 
 ```c++
 vector<uint8_t> skBytes = sk.Serialize();
 vector<uint8_t> pkBytes = pk.Serialize();
@@ -306,9 +304,7 @@
 GMP is distributed under the
 [GNU LGPL v3 license](https://www.gnu.org/licenses/lgpl-3.0.html)
 
 ## Relic license
 
 Relic is used with the
 [Apache 2.0 license](https://github.com/relic-toolkit/relic/blob/master/LICENSE.Apache-2.0)
-
-
```

### Comparing `blspy-1.0.9/blspy.egg-info/SOURCES.txt` & `blspy-2.0.0b1/blspy.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -9,27 +9,24 @@
 js_build.sh
 js_test.sh
 lgtm.yml
 mypi.ini
 pyproject.toml
 setup.py
 ./
-.github/workflows/build-aarch64.yml
-.github/workflows/build-m1-wheel.yml
 .github/workflows/build-test.yaml
 .github/workflows/build-wheels.yml
-.github/workflows/relic-nightly.yml
+.github/workflows/js-bindings.yml
 .github/workflows/stale-issue.yml
 blspy.egg-info/PKG-INFO
 blspy.egg-info/SOURCES.txt
 blspy.egg-info/dependency_links.txt
 blspy.egg-info/not-zip-safe
 blspy.egg-info/requires.txt
 blspy.egg-info/top_level.txt
-cmake_modules/Findgmp.cmake
 cmake_modules/Findsodium.cmake
 contrib/gmp-patch-6.2.1/compat.c
 contrib/gmp-patch-6.2.1/longlong.h
 js-bindings/CMakeLists.txt
 js-bindings/README.md
 js-bindings/blsjs.d.ts
 js-bindings/helpers.cpp
@@ -42,16 +39,14 @@
 js-bindings/tests/Signature.spec.js
 js-bindings/tests/karma.conf.js
 js-bindings/tests/karma.test.js
 js-bindings/tests/test.js
 js-bindings/tests/typings.spec.ts
 js-bindings/tests/webpack.config.js
 js-bindings/tests/yarn.lock
-js-bindings/wrappers/BignumWrapper.cpp
-js-bindings/wrappers/BignumWrapper.h
 js-bindings/wrappers/G1ElementWrapper.cpp
 js-bindings/wrappers/G1ElementWrapper.h
 js-bindings/wrappers/G2ElementWrapper.cpp
 js-bindings/wrappers/G2ElementWrapper.h
 js-bindings/wrappers/JSWrapper.h
 js-bindings/wrappers/PrivateKeyWrapper.cpp
 js-bindings/wrappers/PrivateKeyWrapper.h
@@ -76,14 +71,15 @@
 python-impl/pairing.py
 python-impl/private_key.py
 python-impl/schemes.py
 python-impl/util.py
 src/CMakeLists.txt
 src/bls.cpp
 src/bls.hpp
+src/blstasm.lib
 src/elements.cpp
 src/elements.hpp
 src/hdkeys.hpp
 src/hkdf.hpp
 src/privatekey.cpp
 src/privatekey.hpp
 src/schemes.cpp
```

### Comparing `blspy-1.0.9/cmake_modules/Findsodium.cmake` & `blspy-2.0.0b1/cmake_modules/Findsodium.cmake`

 * *Files identical despite different names*

### Comparing `blspy-1.0.9/contrib/gmp-patch-6.2.1/compat.c` & `blspy-2.0.0b1/contrib/gmp-patch-6.2.1/compat.c`

 * *Files identical despite different names*

### Comparing `blspy-1.0.9/contrib/gmp-patch-6.2.1/longlong.h` & `blspy-2.0.0b1/contrib/gmp-patch-6.2.1/longlong.h`

 * *Files identical despite different names*

### Comparing `blspy-1.0.9/js-bindings/CMakeLists.txt` & `blspy-2.0.0b1/js-bindings/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `blspy-1.0.9/js-bindings/README.md` & `blspy-2.0.0b1/js-bindings/README.md`

 * *Files identical despite different names*

### Comparing `blspy-1.0.9/js-bindings/blsjs.d.ts` & `blspy-2.0.0b1/js-bindings/blsjs.d.ts`

 * *Files 6% similar despite different names*

```diff
@@ -43,30 +43,28 @@
   static from_bytes(bytes: Uint8Array): G1Element;
   static generator(): G2Element;
   serialize(): Uint8Array;
   negate(): G1Element;
   deepcopy(): G1Element;
   get_fingerprint(): number;
   add(el: G1Element): G1Element;
-  mul(bn: Bignum): G1Element;
   equal_to(el: G1Element): boolean;
   delete(): void;
 }
 
 export declare class G2Element {
   static SIZE: number;
   static from_bytes(bytes: Uint8Array): G2Element;
   static from_g2(sk: G2Element): G2Element;
   static aggregate_sigs(sigs: G2Element[]): G2Element;
   static generator(): G2Element;
   serialize(): Uint8Array;
   negate(): G2Element;
   deepcopy(): G2Element;
   add(el: G2Element): G2Element;
-  mul(bn: Bignum): G2Element;
   equal_to(el: G2Element): boolean;
   delete(): void;
 }
 
 export declare class PrivateKey {
   static PRIVATE_KEY_SIZE: number;
   static from_bytes(bytes: Uint8Array, modOrder: boolean): PrivateKey;
@@ -77,30 +75,23 @@
   get_g2(): G2Element;
   mul_g1(el: G1Element): G1Element;
   mul_g2(el: G2Element): G2Element;
   equal_to(key: PrivateKey): boolean;
   delete(): void;
 }
 
-export declare class Bignum {
-  static from_string(s: string, radix: number): Bignum;
-  toString(radix: number): string;
-  delete(): void;
-}
-
 export declare class Util {
   static hash256(msg: Uint8Array): Uint8Array;
   static hex_str(msg: Uint8Array): string;
 }
 
 export interface ModuleInstance {
   AugSchemeMPL: typeof AugSchemeMPL;
   BasicSchemeMPL: typeof BasicSchemeMPL;
   PopSchemeMPL: typeof PopSchemeMPL;
   G1Element: typeof G1Element;
   G2Element: typeof G2Element;
   PrivateKey: typeof PrivateKey;
-  Bignum: typeof Bignum;
   Util: typeof Util;
 }
 
 export default function createModule(options?: {}): Promise<ModuleInstance>;
```

### Comparing `blspy-1.0.9/js-bindings/helpers.cpp` & `blspy-2.0.0b1/js-bindings/helpers.cpp`

 * *Files 7% similar despite different names*

```diff
@@ -22,20 +22,14 @@
 
     val toUint8Array(uint8_t *pointer, size_t data_size) {
         std::vector<uint8_t> vec = toVector(pointer, data_size);
         val buffer = toUint8Array(vec);
         return buffer;
     }
 
-    val toUint8Array(bn_t bn) {
-        std::vector<uint8_t> vec = toVector(bn);
-        val buffer = toUint8Array(vec);
-        return buffer;
-    }
-
     std::vector<uint8_t> toVector(uint8_t *pointer, size_t data_size) {
         std::vector<uint8_t> data;
         data.reserve(data_size);
         std::copy(pointer, pointer + data_size, std::back_inserter(data));
         return data;
     }
 
@@ -44,44 +38,23 @@
         std::vector<uint8_t> vec;
         for (unsigned i = 0; i < l; ++i) {
             vec.push_back(jsUint8Array[i].as<uint8_t>());
         }
         return vec;
     }
 
-    std::vector<uint8_t> toVector(bn_t bn) {
-        uint8_t buf[bn_size_bin(bn)];
-        bn_write_bin(buf, bn_size_bin(bn), bn);
-        std::vector<uint8_t> vec = helpers::toVector(buf, bn_size_bin(bn));
-        return vec;
-    }
-
     std::vector<std::vector<uint8_t>> jsBuffersArrayToVector(val buffersArray) {
         auto l = buffersArray["length"].as<unsigned>();
         std::vector<std::vector<uint8_t>> vec;
         for (unsigned i = 0; i < l; ++i) {
             vec.push_back(toVector(buffersArray[i].as<val>()));
         }
         return vec;
     }
 
-    std::vector<bn_t *> jsBuffersArrayToBnVector(val buffersArray) {
-        auto l = buffersArray["length"].as<unsigned>();
-        std::vector<bn_t *> vec;
-        for (unsigned i = 0; i < l; ++i) {
-            bn_t data;
-            bn_new(data);
-            std::vector<uint8_t> bnVec = toVector(buffersArray[i]);
-            bn_read_bin(data, bnVec.data(), static_cast<int>(bnVec.size()));
-            bn_t *point = &data;
-            vec.push_back(point);
-        }
-        return vec;
-    }
-
     val byteArraysVectorToJsBuffersArray(std::vector<uint8_t *> arraysVector, size_t element_size) {
         auto vecSize = arraysVector.size();
         std::vector<val> valVector;
         for (unsigned i = 0; i < vecSize; ++i) {
             valVector.push_back(toUint8Array(arraysVector[i], element_size));
         }
         val arr = helpers::toJSArray<val>(valVector);
```

### Comparing `blspy-1.0.9/js-bindings/helpers.h` & `blspy-2.0.0b1/js-bindings/helpers.h`

 * *Files 6% similar despite different names*

```diff
@@ -14,35 +14,28 @@
 
 #ifndef JS_BINDINGS_HELPERS_H_
 #define JS_BINDINGS_HELPERS_H_
 
 #include <algorithm>
 #include <vector>
 #include "emscripten/val.h"
-extern "C" {
-#include "relic.h"
-}
 #include "../src/bls.hpp"
 
 using namespace emscripten;
 using namespace bls;
 
 namespace helpers {
     val toUint8Array(uint8_t *pointer, size_t data_size);
 
     val toUint8Array(std::vector<uint8_t> vec);
 
-    val toUint8Array(bn_t bn);
-
     std::vector<uint8_t> toVector(uint8_t *pointer, size_t data_size);
 
     std::vector<uint8_t> toVector(val jsBuffer);
 
-    std::vector<uint8_t> toVector(bn_t bn);
-
     template<typename T>
     inline std::vector<T> toVectorFromJSArray(val jsArray) {
         auto l = jsArray["length"].as<unsigned>();
         std::vector<T> vec;
         for (unsigned i = 0; i < l; ++i) {
             vec.push_back(jsArray[i].as<T>());
         }
@@ -58,13 +51,11 @@
             arr.call<void>("push", vec[i]);
         }
         return arr;
     }
 
     std::vector<std::vector<uint8_t>> jsBuffersArrayToVector(val buffersArray);
 
-    std::vector<bn_t *> jsBuffersArrayToBnVector(val buffersArray);
-
     val byteArraysVectorToJsBuffersArray(std::vector<uint8_t *> arraysVector, size_t element_size);
 }  // namespace helpers
 
 #endif  // JS_BINDINGS_HELPERS_H_
```

### Comparing `blspy-1.0.9/js-bindings/jsbindings.cpp` & `blspy-2.0.0b1/js-bindings/jsbindings.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -66,30 +66,28 @@
         .class_function("from_bytes", &G1ElementWrapper::FromBytes)
         .class_function("generator", &G2ElementWrapper::Generator)
         .function("serialize", &G1ElementWrapper::Serialize)
         .function("negate", &G1ElementWrapper::Negate)
         .function("deepcopy", &G1ElementWrapper::Deepcopy)
         .function("get_fingerprint", &G1ElementWrapper::GetFingerprint)
         .function("add", &G1ElementWrapper::Add)
-        .function("mul", &G1ElementWrapper::Mul)
         .function("equal_to", &G1ElementWrapper::EqualTo);
 
     class_<G2ElementWrapper>("G2Element")
         .class_property("SIZE", &G2ElementWrapper::SIZE)
         .constructor<>()
         .class_function("fromBytes", &G2ElementWrapper::FromBytes) // Not removing this for compatibility
         .class_function("from_bytes", &G2ElementWrapper::FromBytes)
         .class_function("from_g2", &G2ElementWrapper::FromG2Element)
         .class_function("aggregate_sigs", &G2ElementWrapper::AggregateSigs)
         .class_function("generator", &G2ElementWrapper::Generator)
         .function("serialize", &G2ElementWrapper::Serialize)
         .function("negate", &G2ElementWrapper::Negate)
         .function("deepcopy", &G2ElementWrapper::Deepcopy)
         .function("add", &G2ElementWrapper::Add)
-        .function("mul", &G2ElementWrapper::Mul)
         .function("equal_to", &G2ElementWrapper::EqualTo);
 
     class_<PrivateKeyWrapper>("PrivateKey")
         .class_property("PRIVATE_KEY_SIZE", &PrivateKeyWrapper::PRIVATE_KEY_SIZE)
         .class_function("fromBytes", &PrivateKeyWrapper::FromBytes) // Not removing this for compatibility
         .class_function("from_bytes", &PrivateKeyWrapper::FromBytes)
         .class_function("aggregate", &PrivateKeyWrapper::Aggregate)
@@ -97,17 +95,12 @@
         .function("serialize", &PrivateKeyWrapper::Serialize)
         .function("get_g1", &PrivateKeyWrapper::GetG1)
         .function("get_g2", &PrivateKeyWrapper::GetG2)
         .function("mul_g1", &PrivateKeyWrapper::MulG1)
         .function("mul_g2", &PrivateKeyWrapper::MulG2)
         .function("equal_to", &PrivateKeyWrapper::EqualTo);
 
-    class_<BignumWrapper>("Bignum")
-        .class_function("fromString", &BignumWrapper::FromString) // Not removing this for compatibility
-        .class_function("from_string", &BignumWrapper::FromString)
-        .function("toString", &BignumWrapper::ToString);
-
     class_<UtilWrapper>("Util")
         .class_function("hash256", &UtilWrapper::Hash256)
         .class_function("hex_str", &UtilWrapper::HexStr);
 };
 }  // namespace js_wrappers
```

### Comparing `blspy-1.0.9/js-bindings/package-lock.json` & `blspy-2.0.0b1/js-bindings/package-lock.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9842466583821778%*

 * *Differences: {"'dependencies'": "{'@types/eslint': {'version': '8.37.0', 'resolved': "*

 * *                   "'https://registry.npmjs.org/@types/eslint/-/eslint-8.37.0.tgz', 'integrity': "*

 * *                   "'sha512-Piet7dG2JBuDIfohBngQ3rCt7MgO9xCO4xIMKxBThCq5PNRB91IjlJ10eJVwfoNtvTErmxLzwBZ7rHZtbOMmFQ=='}, "*

 * *                   "'@types/eslint-scope': {'version': '3.7.4', 'resolved': "*

 * *                   "'https://registry.npmjs.org/@types/eslint-scope/-/eslint-scope-3.7.4.tgz', "*

 * *                   "'integrity': "*

 * *        […]*

```diff
@@ -1,14 +1,69 @@
 {
     "dependencies": {
-        "@types/component-emitter": {
+        "@jridgewell/gen-mapping": {
             "dev": true,
-            "integrity": "sha512-bsjleuRKWmGqajMerkzox19aGbscQX5rmmvvXl3wlIp5gMG1HgkiwPxsN5p070fBDKTNSPgojVbuY1+HWMbFhg==",
-            "resolved": "https://registry.npmjs.org/@types/component-emitter/-/component-emitter-1.2.10.tgz",
-            "version": "1.2.10"
+            "integrity": "sha512-HLhSWOLRi875zjjMG/r+Nv0oCW8umGb0BgEhyX3dDX3egwZtB8PqLnjz3yedt8R5StBrzcg4aBpnh8UA9D1BoQ==",
+            "requires": {
+                "@jridgewell/set-array": "^1.0.1",
+                "@jridgewell/sourcemap-codec": "^1.4.10",
+                "@jridgewell/trace-mapping": "^0.3.9"
+            },
+            "resolved": "https://registry.npmjs.org/@jridgewell/gen-mapping/-/gen-mapping-0.3.3.tgz",
+            "version": "0.3.3"
+        },
+        "@jridgewell/resolve-uri": {
+            "dev": true,
+            "integrity": "sha512-F2msla3tad+Mfht5cJq7LSXcdudKTWCVYUgw6pLFOOHSTtZlj6SWNYAp+AhuqLmWdBO2X5hPrLcu8cVP8fy28w==",
+            "resolved": "https://registry.npmjs.org/@jridgewell/resolve-uri/-/resolve-uri-3.1.0.tgz",
+            "version": "3.1.0"
+        },
+        "@jridgewell/set-array": {
+            "dev": true,
+            "integrity": "sha512-xnkseuNADM0gt2bs+BvhO0p78Mk762YnZdsuzFV018NoG1Sj1SCQvpSqa7XUaTam5vAGasABV9qXASMKnFMwMw==",
+            "resolved": "https://registry.npmjs.org/@jridgewell/set-array/-/set-array-1.1.2.tgz",
+            "version": "1.1.2"
+        },
+        "@jridgewell/source-map": {
+            "dev": true,
+            "integrity": "sha512-b+fsZXeLYi9fEULmfBrhxn4IrPlINf8fiNarzTof004v3lFdntdwa9PF7vFJqm3mg7s+ScJMxXaE3Acp1irZcg==",
+            "requires": {
+                "@jridgewell/gen-mapping": "^0.3.0",
+                "@jridgewell/trace-mapping": "^0.3.9"
+            },
+            "resolved": "https://registry.npmjs.org/@jridgewell/source-map/-/source-map-0.3.3.tgz",
+            "version": "0.3.3"
+        },
+        "@jridgewell/sourcemap-codec": {
+            "dev": true,
+            "integrity": "sha512-XPSJHWmi394fuUuzDnGz1wiKqWfo1yXecHQMRf2l6hztTO+nPru658AyDngaBe7isIxEkRsPR3FZh+s7iVa4Uw==",
+            "resolved": "https://registry.npmjs.org/@jridgewell/sourcemap-codec/-/sourcemap-codec-1.4.14.tgz",
+            "version": "1.4.14"
+        },
+        "@jridgewell/trace-mapping": {
+            "dev": true,
+            "integrity": "sha512-w+niJYzMHdd7USdiH2U6869nqhD2nbfZXND5Yp93qIbEmnDNk7PD48o+YchRVpzMU7M6jVCbenTR7PA1FLQ9pA==",
+            "requires": {
+                "@jridgewell/resolve-uri": "3.1.0",
+                "@jridgewell/sourcemap-codec": "1.4.14"
+            },
+            "resolved": "https://registry.npmjs.org/@jridgewell/trace-mapping/-/trace-mapping-0.3.18.tgz",
+            "version": "0.3.18"
+        },
+        "@socket.io/base64-arraybuffer": {
+            "dev": true,
+            "integrity": "sha512-dOlCBKnDw4iShaIsH/bxujKTM18+2TOAsYz+KSc11Am38H4q5Xw8Bbz97ZYdrVNM+um3p7w86Bvvmcn9q+5+eQ==",
+            "resolved": "https://registry.npmjs.org/@socket.io/base64-arraybuffer/-/base64-arraybuffer-1.0.2.tgz",
+            "version": "1.0.2"
+        },
+        "@socket.io/component-emitter": {
+            "dev": true,
+            "integrity": "sha512-+9jVqKhRSpsc591z5vX+X5Yyw+he/HCB4iQ/RYxw35CEPaY1gnsNE43nf9n9AaYjAQrTiI/mOwKUKdUs9vf7Xg==",
+            "resolved": "https://registry.npmjs.org/@socket.io/component-emitter/-/component-emitter-3.1.0.tgz",
+            "version": "3.1.0"
         },
         "@types/cookie": {
             "dev": true,
             "integrity": "sha512-XW/Aa8APYr6jSVVA1y/DEIZX0/GMKLEVekNG727R8cs56ahETkRAy/3DR7+fJyh7oUgGwNQaRfXCun0+KbWY7Q==",
             "resolved": "https://registry.npmjs.org/@types/cookie/-/cookie-0.4.1.tgz",
             "version": "0.4.1"
         },
@@ -16,235 +71,252 @@
             "dev": true,
             "integrity": "sha512-vt+kDhq/M2ayberEtJcIN/hxXy1Pk+59g2FV/ZQceeaTyCtCucjL2Q7FXlFjtWn4n15KCr1NE2lNNFhp0lEThw==",
             "resolved": "https://registry.npmjs.org/@types/cors/-/cors-2.8.12.tgz",
             "version": "2.8.12"
         },
         "@types/eslint": {
             "dev": true,
-            "integrity": "sha512-LKmQCWAlnVHvvXq4oasNUMTJJb2GwSyTY8+1C7OH5ILR8mPLaljv1jxL1bXW3xB3jFbQxTKxJAvI8PyjB09aBg==",
+            "integrity": "sha512-Piet7dG2JBuDIfohBngQ3rCt7MgO9xCO4xIMKxBThCq5PNRB91IjlJ10eJVwfoNtvTErmxLzwBZ7rHZtbOMmFQ==",
             "requires": {
                 "@types/estree": "*",
                 "@types/json-schema": "*"
             },
-            "resolved": "https://registry.npmjs.org/@types/eslint/-/eslint-7.2.13.tgz",
-            "version": "7.2.13"
+            "resolved": "https://registry.npmjs.org/@types/eslint/-/eslint-8.37.0.tgz",
+            "version": "8.37.0"
         },
         "@types/eslint-scope": {
             "dev": true,
-            "integrity": "sha512-O/ql2+rrCUe2W2rs7wMR+GqPRcgB6UiqN5RhrR5xruFlY7l9YLMn0ZkDzjoHLeiFkR8MCQZVudUuuvQ2BLC9Qw==",
+            "integrity": "sha512-9K4zoImiZc3HlIp6AVUDE4CWYx22a+lhSZMYNpbjW04+YF0KWj4pJXnEMjdnFTiQibFFmElcsasJXDbdI/EPhA==",
             "requires": {
                 "@types/eslint": "*",
                 "@types/estree": "*"
             },
-            "resolved": "https://registry.npmjs.org/@types/eslint-scope/-/eslint-scope-3.7.0.tgz",
-            "version": "3.7.0"
+            "resolved": "https://registry.npmjs.org/@types/eslint-scope/-/eslint-scope-3.7.4.tgz",
+            "version": "3.7.4"
         },
         "@types/estree": {
             "dev": true,
-            "integrity": "sha512-c5ciR06jK8u9BstrmJyO97m+klJrrhCf9u3rLu3DEAJBirxRqSCvDQoYKmxuYwQI5SZChAWu+tq9oVlGRuzPAg==",
-            "resolved": "https://registry.npmjs.org/@types/estree/-/estree-0.0.47.tgz",
-            "version": "0.0.47"
+            "integrity": "sha512-CuPgU6f3eT/XgKKPqKd/gLZV1Xmvf1a2R5POBOGQa6uv82xpls89HU5zKeVoyR8XzHd1RGNOlQlvUe3CFkjWNQ==",
+            "resolved": "https://registry.npmjs.org/@types/estree/-/estree-0.0.51.tgz",
+            "version": "0.0.51"
         },
         "@types/json-schema": {
             "dev": true,
-            "integrity": "sha512-cxWFQVseBm6O9Gbw1IWb8r6OS4OhSt3hPZLkFApLjM8TEXROBuQGLAH2i2gZpcXdLBIrpXuTDhH7Vbm1iXmNGA==",
-            "resolved": "https://registry.npmjs.org/@types/json-schema/-/json-schema-7.0.7.tgz",
-            "version": "7.0.7"
+            "integrity": "sha512-wOuvG1SN4Us4rez+tylwwwCV1psiNVOkJeM3AUWUNWg/jDQY2+HE/444y5gc+jBmRqASOm2Oeh5c1axHobwRKQ==",
+            "resolved": "https://registry.npmjs.org/@types/json-schema/-/json-schema-7.0.11.tgz",
+            "version": "7.0.11"
         },
         "@types/mocha": {
             "dev": true,
             "integrity": "sha512-NYrtPht0wGzhwe9+/idPaBB+TqkY9AhTvOLMkThm0IoEfLaiVQZwBwyJ5puCkO3AUCWrmcoePjp2mbFocKy4SQ==",
             "resolved": "https://registry.npmjs.org/@types/mocha/-/mocha-5.2.7.tgz",
             "version": "5.2.7"
         },
         "@types/node": {
             "dev": true,
             "integrity": "sha512-3p2M6moxwdDFyPia2ROI8CCkRa9ZzYjvCys2TOE1xgwYDQmY49Cj0cvkdBkzh/rY9gkvzgzYOeECYtB4f0/fDA==",
             "resolved": "https://registry.npmjs.org/@types/node/-/node-11.15.18.tgz",
             "version": "11.15.18"
         },
-        "@ungap/promise-all-settled": {
-            "dev": true,
-            "integrity": "sha512-sL/cEvJWAnClXw0wHk85/2L0G6Sj8UB0Ctc1TEMbKSsmpRosqhwj9gWgFRZSrBr2f9tiXISwNhCPmlfqUqyb9Q==",
-            "resolved": "https://registry.npmjs.org/@ungap/promise-all-settled/-/promise-all-settled-1.1.2.tgz",
-            "version": "1.1.2"
-        },
         "@webassemblyjs/ast": {
             "dev": true,
-            "integrity": "sha512-kX2W49LWsbthrmIRMbQZuQDhGtjyqXfEmmHyEi4XWnSZtPmxY0+3anPIzsnRb45VH/J55zlOfWvZuY47aJZTJg==",
+            "integrity": "sha512-ukBh14qFLjxTQNTXocdyksN5QdM28S1CxHt2rdskFyL+xFV7VremuBLVbmCePj+URalXBENx/9Lm7lnhihtCSw==",
             "requires": {
-                "@webassemblyjs/helper-numbers": "1.11.0",
-                "@webassemblyjs/helper-wasm-bytecode": "1.11.0"
+                "@webassemblyjs/helper-numbers": "1.11.1",
+                "@webassemblyjs/helper-wasm-bytecode": "1.11.1"
             },
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/ast/-/ast-1.11.0.tgz",
-            "version": "1.11.0"
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/ast/-/ast-1.11.1.tgz",
+            "version": "1.11.1"
         },
         "@webassemblyjs/floating-point-hex-parser": {
             "dev": true,
-            "integrity": "sha512-Q/aVYs/VnPDVYvsCBL/gSgwmfjeCb4LW8+TMrO3cSzJImgv8lxxEPM2JA5jMrivE7LSz3V+PFqtMbls3m1exDA==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/floating-point-hex-parser/-/floating-point-hex-parser-1.11.0.tgz",
-            "version": "1.11.0"
+            "integrity": "sha512-iGRfyc5Bq+NnNuX8b5hwBrRjzf0ocrJPI6GWFodBFzmFnyvrQ83SHKhmilCU/8Jv67i4GJZBMhEzltxzcNagtQ==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/floating-point-hex-parser/-/floating-point-hex-parser-1.11.1.tgz",
+            "version": "1.11.1"
         },
         "@webassemblyjs/helper-api-error": {
             "dev": true,
-            "integrity": "sha512-baT/va95eXiXb2QflSx95QGT5ClzWpGaa8L7JnJbgzoYeaA27FCvuBXU758l+KXWRndEmUXjP0Q5fibhavIn8w==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-api-error/-/helper-api-error-1.11.0.tgz",
-            "version": "1.11.0"
+            "integrity": "sha512-RlhS8CBCXfRUR/cwo2ho9bkheSXG0+NwooXcc3PAILALf2QLdFyj7KGsKRbVc95hZnhnERon4kW/D3SZpp6Tcg==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-api-error/-/helper-api-error-1.11.1.tgz",
+            "version": "1.11.1"
         },
         "@webassemblyjs/helper-buffer": {
             "dev": true,
-            "integrity": "sha512-u9HPBEl4DS+vA8qLQdEQ6N/eJQ7gT7aNvMIo8AAWvAl/xMrcOSiI2M0MAnMCy3jIFke7bEee/JwdX1nUpCtdyA==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-buffer/-/helper-buffer-1.11.0.tgz",
-            "version": "1.11.0"
+            "integrity": "sha512-gwikF65aDNeeXa8JxXa2BAk+REjSyhrNC9ZwdT0f8jc4dQQeDQ7G4m0f2QCLPJiMTTO6wfDmRmj/pW0PsUvIcA==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-buffer/-/helper-buffer-1.11.1.tgz",
+            "version": "1.11.1"
         },
         "@webassemblyjs/helper-numbers": {
             "dev": true,
-            "integrity": "sha512-DhRQKelIj01s5IgdsOJMKLppI+4zpmcMQ3XboFPLwCpSNH6Hqo1ritgHgD0nqHeSYqofA6aBN/NmXuGjM1jEfQ==",
+            "integrity": "sha512-vDkbxiB8zfnPdNK9Rajcey5C0w+QJugEglN0of+kmO8l7lDb77AnlKYQF7aarZuCrv+l0UvqL+68gSDr3k9LPQ==",
             "requires": {
-                "@webassemblyjs/floating-point-hex-parser": "1.11.0",
-                "@webassemblyjs/helper-api-error": "1.11.0",
+                "@webassemblyjs/floating-point-hex-parser": "1.11.1",
+                "@webassemblyjs/helper-api-error": "1.11.1",
                 "@xtuc/long": "4.2.2"
             },
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-numbers/-/helper-numbers-1.11.0.tgz",
-            "version": "1.11.0"
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-numbers/-/helper-numbers-1.11.1.tgz",
+            "version": "1.11.1"
         },
         "@webassemblyjs/helper-wasm-bytecode": {
             "dev": true,
-            "integrity": "sha512-MbmhvxXExm542tWREgSFnOVo07fDpsBJg3sIl6fSp9xuu75eGz5lz31q7wTLffwL3Za7XNRCMZy210+tnsUSEA==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-wasm-bytecode/-/helper-wasm-bytecode-1.11.0.tgz",
-            "version": "1.11.0"
+            "integrity": "sha512-PvpoOGiJwXeTrSf/qfudJhwlvDQxFgelbMqtq52WWiXC6Xgg1IREdngmPN3bs4RoO83PnL/nFrxucXj1+BX62Q==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-wasm-bytecode/-/helper-wasm-bytecode-1.11.1.tgz",
+            "version": "1.11.1"
         },
         "@webassemblyjs/helper-wasm-section": {
             "dev": true,
-            "integrity": "sha512-3Eb88hcbfY/FCukrg6i3EH8H2UsD7x8Vy47iVJrP967A9JGqgBVL9aH71SETPx1JrGsOUVLo0c7vMCN22ytJew==",
+            "integrity": "sha512-10P9No29rYX1j7F3EVPX3JvGPQPae+AomuSTPiF9eBQeChHI6iqjMIwR9JmOJXwpnn/oVGDk7I5IlskuMwU/pg==",
             "requires": {
-                "@webassemblyjs/ast": "1.11.0",
-                "@webassemblyjs/helper-buffer": "1.11.0",
-                "@webassemblyjs/helper-wasm-bytecode": "1.11.0",
-                "@webassemblyjs/wasm-gen": "1.11.0"
+                "@webassemblyjs/ast": "1.11.1",
+                "@webassemblyjs/helper-buffer": "1.11.1",
+                "@webassemblyjs/helper-wasm-bytecode": "1.11.1",
+                "@webassemblyjs/wasm-gen": "1.11.1"
             },
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-wasm-section/-/helper-wasm-section-1.11.0.tgz",
-            "version": "1.11.0"
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-wasm-section/-/helper-wasm-section-1.11.1.tgz",
+            "version": "1.11.1"
         },
         "@webassemblyjs/ieee754": {
             "dev": true,
-            "integrity": "sha512-KXzOqpcYQwAfeQ6WbF6HXo+0udBNmw0iXDmEK5sFlmQdmND+tr773Ti8/5T/M6Tl/413ArSJErATd8In3B+WBA==",
+            "integrity": "sha512-hJ87QIPtAMKbFq6CGTkZYJivEwZDbQUgYd3qKSadTNOhVY7p+gfP6Sr0lLRVTaG1JjFj+r3YchoqRYxNH3M0GQ==",
             "requires": {
                 "@xtuc/ieee754": "^1.2.0"
             },
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/ieee754/-/ieee754-1.11.0.tgz",
-            "version": "1.11.0"
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/ieee754/-/ieee754-1.11.1.tgz",
+            "version": "1.11.1"
         },
         "@webassemblyjs/leb128": {
             "dev": true,
-            "integrity": "sha512-aqbsHa1mSQAbeeNcl38un6qVY++hh8OpCOzxhixSYgbRfNWcxJNJQwe2rezK9XEcssJbbWIkblaJRwGMS9zp+g==",
+            "integrity": "sha512-BJ2P0hNZ0u+Th1YZXJpzW6miwqQUGcIHT1G/sf72gLVD9DZ5AdYTqPNbHZh6K1M5VmKvFXwGSWZADz+qBWxeRw==",
             "requires": {
                 "@xtuc/long": "4.2.2"
             },
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/leb128/-/leb128-1.11.0.tgz",
-            "version": "1.11.0"
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/leb128/-/leb128-1.11.1.tgz",
+            "version": "1.11.1"
         },
         "@webassemblyjs/utf8": {
             "dev": true,
-            "integrity": "sha512-A/lclGxH6SpSLSyFowMzO/+aDEPU4hvEiooCMXQPcQFPPJaYcPQNKGOCLUySJsYJ4trbpr+Fs08n4jelkVTGVw==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/utf8/-/utf8-1.11.0.tgz",
-            "version": "1.11.0"
+            "integrity": "sha512-9kqcxAEdMhiwQkHpkNiorZzqpGrodQQ2IGrHHxCy+Ozng0ofyMA0lTqiLkVs1uzTRejX+/O0EOT7KxqVPuXosQ==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/utf8/-/utf8-1.11.1.tgz",
+            "version": "1.11.1"
         },
         "@webassemblyjs/wasm-edit": {
             "dev": true,
-            "integrity": "sha512-JHQ0damXy0G6J9ucyKVXO2j08JVJ2ntkdJlq1UTiUrIgfGMmA7Ik5VdC/L8hBK46kVJgujkBIoMtT8yVr+yVOQ==",
+            "integrity": "sha512-g+RsupUC1aTHfR8CDgnsVRVZFJqdkFHpsHMfJuWQzWU3tvnLC07UqHICfP+4XyL2tnr1amvl1Sdp06TnYCmVkA==",
             "requires": {
-                "@webassemblyjs/ast": "1.11.0",
-                "@webassemblyjs/helper-buffer": "1.11.0",
-                "@webassemblyjs/helper-wasm-bytecode": "1.11.0",
-                "@webassemblyjs/helper-wasm-section": "1.11.0",
-                "@webassemblyjs/wasm-gen": "1.11.0",
-                "@webassemblyjs/wasm-opt": "1.11.0",
-                "@webassemblyjs/wasm-parser": "1.11.0",
-                "@webassemblyjs/wast-printer": "1.11.0"
+                "@webassemblyjs/ast": "1.11.1",
+                "@webassemblyjs/helper-buffer": "1.11.1",
+                "@webassemblyjs/helper-wasm-bytecode": "1.11.1",
+                "@webassemblyjs/helper-wasm-section": "1.11.1",
+                "@webassemblyjs/wasm-gen": "1.11.1",
+                "@webassemblyjs/wasm-opt": "1.11.1",
+                "@webassemblyjs/wasm-parser": "1.11.1",
+                "@webassemblyjs/wast-printer": "1.11.1"
             },
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/wasm-edit/-/wasm-edit-1.11.0.tgz",
-            "version": "1.11.0"
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/wasm-edit/-/wasm-edit-1.11.1.tgz",
+            "version": "1.11.1"
         },
         "@webassemblyjs/wasm-gen": {
             "dev": true,
-            "integrity": "sha512-BEUv1aj0WptCZ9kIS30th5ILASUnAPEvE3tVMTrItnZRT9tXCLW2LEXT8ezLw59rqPP9klh9LPmpU+WmRQmCPQ==",
+            "integrity": "sha512-F7QqKXwwNlMmsulj6+O7r4mmtAlCWfO/0HdgOxSklZfQcDu0TpLiD1mRt/zF25Bk59FIjEuGAIyn5ei4yMfLhA==",
             "requires": {
-                "@webassemblyjs/ast": "1.11.0",
-                "@webassemblyjs/helper-wasm-bytecode": "1.11.0",
-                "@webassemblyjs/ieee754": "1.11.0",
-                "@webassemblyjs/leb128": "1.11.0",
-                "@webassemblyjs/utf8": "1.11.0"
+                "@webassemblyjs/ast": "1.11.1",
+                "@webassemblyjs/helper-wasm-bytecode": "1.11.1",
+                "@webassemblyjs/ieee754": "1.11.1",
+                "@webassemblyjs/leb128": "1.11.1",
+                "@webassemblyjs/utf8": "1.11.1"
             },
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/wasm-gen/-/wasm-gen-1.11.0.tgz",
-            "version": "1.11.0"
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/wasm-gen/-/wasm-gen-1.11.1.tgz",
+            "version": "1.11.1"
         },
         "@webassemblyjs/wasm-opt": {
             "dev": true,
-            "integrity": "sha512-tHUSP5F4ywyh3hZ0+fDQuWxKx3mJiPeFufg+9gwTpYp324mPCQgnuVKwzLTZVqj0duRDovnPaZqDwoyhIO8kYg==",
+            "integrity": "sha512-VqnkNqnZlU5EB64pp1l7hdm3hmQw7Vgqa0KF/KCNO9sIpI6Fk6brDEiX+iCOYrvMuBWDws0NkTOxYEb85XQHHw==",
             "requires": {
-                "@webassemblyjs/ast": "1.11.0",
-                "@webassemblyjs/helper-buffer": "1.11.0",
-                "@webassemblyjs/wasm-gen": "1.11.0",
-                "@webassemblyjs/wasm-parser": "1.11.0"
+                "@webassemblyjs/ast": "1.11.1",
+                "@webassemblyjs/helper-buffer": "1.11.1",
+                "@webassemblyjs/wasm-gen": "1.11.1",
+                "@webassemblyjs/wasm-parser": "1.11.1"
             },
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/wasm-opt/-/wasm-opt-1.11.0.tgz",
-            "version": "1.11.0"
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/wasm-opt/-/wasm-opt-1.11.1.tgz",
+            "version": "1.11.1"
         },
         "@webassemblyjs/wasm-parser": {
             "dev": true,
-            "integrity": "sha512-6L285Sgu9gphrcpDXINvm0M9BskznnzJTE7gYkjDbxET28shDqp27wpruyx3C2S/dvEwiigBwLA1cz7lNUi0kw==",
+            "integrity": "sha512-rrBujw+dJu32gYB7/Lup6UhdkPx9S9SnobZzRVL7VcBH9Bt9bCBLEuX/YXOOtBsOZ4NQrRykKhffRWHvigQvOA==",
             "requires": {
-                "@webassemblyjs/ast": "1.11.0",
-                "@webassemblyjs/helper-api-error": "1.11.0",
-                "@webassemblyjs/helper-wasm-bytecode": "1.11.0",
-                "@webassemblyjs/ieee754": "1.11.0",
-                "@webassemblyjs/leb128": "1.11.0",
-                "@webassemblyjs/utf8": "1.11.0"
+                "@webassemblyjs/ast": "1.11.1",
+                "@webassemblyjs/helper-api-error": "1.11.1",
+                "@webassemblyjs/helper-wasm-bytecode": "1.11.1",
+                "@webassemblyjs/ieee754": "1.11.1",
+                "@webassemblyjs/leb128": "1.11.1",
+                "@webassemblyjs/utf8": "1.11.1"
             },
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/wasm-parser/-/wasm-parser-1.11.0.tgz",
-            "version": "1.11.0"
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/wasm-parser/-/wasm-parser-1.11.1.tgz",
+            "version": "1.11.1"
         },
         "@webassemblyjs/wast-printer": {
             "dev": true,
-            "integrity": "sha512-Fg5OX46pRdTgB7rKIUojkh9vXaVN6sGYCnEiJN1GYkb0RPwShZXp6KTDqmoMdQPKhcroOXh3fEzmkWmCYaKYhQ==",
+            "integrity": "sha512-IQboUWM4eKzWW+N/jij2sRatKMh99QEelo3Eb2q0qXkvPRISAj8Qxtmw5itwqK+TTkBuUIE45AxYPToqPtL5gg==",
             "requires": {
-                "@webassemblyjs/ast": "1.11.0",
+                "@webassemblyjs/ast": "1.11.1",
                 "@xtuc/long": "4.2.2"
             },
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/wast-printer/-/wast-printer-1.11.0.tgz",
-            "version": "1.11.0"
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/wast-printer/-/wast-printer-1.11.1.tgz",
+            "version": "1.11.1"
         },
         "@xtuc/ieee754": {
             "dev": true,
             "integrity": "sha512-DX8nKgqcGwsc0eJSqYt5lwP4DH5FlHnmuWWBRy7X0NcaGR0ZtuyeESgMwTYVEtxmsNGY+qit4QYT/MIYTOTPeA==",
             "resolved": "https://registry.npmjs.org/@xtuc/ieee754/-/ieee754-1.2.0.tgz",
             "version": "1.2.0"
         },
         "@xtuc/long": {
             "dev": true,
             "integrity": "sha512-NuHqBY1PB/D8xU6s/thBgOAiAP7HOYDQ32+BFZILJ8ivkUkAHQnWfn6WhL79Owj1qmUnoN/YPhktdIoucipkAQ==",
             "resolved": "https://registry.npmjs.org/@xtuc/long/-/long-4.2.2.tgz",
             "version": "4.2.2"
         },
         "accepts": {
+            "dependencies": {
+                "mime-db": {
+                    "dev": true,
+                    "integrity": "sha512-5y8A56jg7XVQx2mbv1lu49NR4dokRnhZYTtL+KGfaa27uq4pSTXkwQkFJl4pkRMyNFz/EtYDSkiiEHx3F7UN6g==",
+                    "resolved": "https://registry.npmjs.org/mime-db/-/mime-db-1.51.0.tgz",
+                    "version": "1.51.0"
+                },
+                "mime-types": {
+                    "dev": true,
+                    "integrity": "sha512-6cP692WwGIs9XXdOO4++N+7qjqv0rqxxVvJ3VHPh/Sc9mVZcQP+ZGhkKiTvWMQRr2tbHkJP/Yn7Y0npb3ZBs4A==",
+                    "requires": {
+                        "mime-db": "1.51.0"
+                    },
+                    "resolved": "https://registry.npmjs.org/mime-types/-/mime-types-2.1.34.tgz",
+                    "version": "2.1.34"
+                }
+            },
             "dev": true,
-            "integrity": "sha512-Il80Qs2WjYlJIBNzNkK6KYqlVMTbZLXgHx2oT0pU/fjRHyEp+PEfEPY0R3WCwAGVOtauxh1hOxNgIf5bv7dQpA==",
+            "integrity": "sha512-PYAthTa2m2VKxuvSD3DPC/Gy+U+sOA1LAuT8mkmRuvw+NACSaeXEQ+NHcVF7rONl6qcaxV3Uuemwawk+7+SJLw==",
             "requires": {
-                "mime-types": "~2.1.24",
-                "negotiator": "0.6.2"
+                "mime-types": "~2.1.34",
+                "negotiator": "0.6.3"
             },
-            "resolved": "https://registry.npmjs.org/accepts/-/accepts-1.3.7.tgz",
-            "version": "1.3.7"
+            "resolved": "https://registry.npmjs.org/accepts/-/accepts-1.3.8.tgz",
+            "version": "1.3.8"
         },
         "acorn": {
             "dev": true,
-            "integrity": "sha512-ULr0LDaEqQrMFGyQ3bhJkLsbtrQ8QibAseGZeaSUiT/6zb9IvIkomWHJIvgvwad+hinRAgsI51JcWk2yvwyL+w==",
-            "resolved": "https://registry.npmjs.org/acorn/-/acorn-8.4.0.tgz",
-            "version": "8.4.0"
+            "integrity": "sha512-xjIYgE8HBrkpd/sJqOGNspf8uHG+NOHGOw6a/Urj8taM2EXfdNAH2oFcPeIFfsv3+kz/mJrS5VuMqbNLjCa2vw==",
+            "resolved": "https://registry.npmjs.org/acorn/-/acorn-8.8.2.tgz",
+            "version": "8.8.2"
+        },
+        "acorn-import-assertions": {
+            "dev": true,
+            "integrity": "sha512-m7VZ3jwz4eK6A4Vtt8Ew1/mNbP24u0FhdyfA7fSvnJR6LMdfOYnmuIrrJAgrYfYJ10F/otaHTtrtrtmHdMNzEw==",
+            "resolved": "https://registry.npmjs.org/acorn-import-assertions/-/acorn-import-assertions-1.8.0.tgz",
+            "version": "1.8.0"
         },
         "ajv": {
             "dev": true,
             "integrity": "sha512-j3fVLgvTo527anyYyJOGTYJbG+vnnQYvE0m5mmkc1TK+nxAppkCLMIL0aZ4dblVCNoGShhm+kzE4ZUykBoMg4g==",
             "requires": {
                 "fast-deep-equal": "^3.1.1",
                 "fast-json-stable-stringify": "^2.0.0",
@@ -264,37 +336,27 @@
             "dev": true,
             "integrity": "sha512-JoX0apGbHaUJBNl6yF+p6JAFYZ666/hhCGKN5t9QFjbJQKUU/g8MNbFDbvfrgKXvI1QpZplPOnwIo99lX/AAmA==",
             "resolved": "https://registry.npmjs.org/ansi-colors/-/ansi-colors-4.1.1.tgz",
             "version": "4.1.1"
         },
         "ansi-regex": {
             "dev": true,
-            "integrity": "sha1-7QMXwyIGT3lGbAKWa922Bas32Zg=",
-            "resolved": "https://registry.npmjs.org/ansi-regex/-/ansi-regex-3.0.0.tgz",
-            "version": "3.0.0"
+            "integrity": "sha512-quJQXlTSUGL2LH9SUXo8VwsY4soanhgo6LNSm84E1LBcE8s3O0wpdiRzyR9z/ZZJMlMWv37qOOb9pdJlMUEKFQ==",
+            "resolved": "https://registry.npmjs.org/ansi-regex/-/ansi-regex-5.0.1.tgz",
+            "version": "5.0.1"
         },
         "ansi-styles": {
             "dev": true,
             "integrity": "sha512-VT0ZI6kZRdTh8YyJw3SMbYm/u+NqfsAxEpWO0Pf9sq8/e94WxxOpPKx9FR1FlyCtOVDNOQ+8ntlqFxiRc+r5qA==",
             "requires": {
                 "color-convert": "^1.9.0"
             },
             "resolved": "https://registry.npmjs.org/ansi-styles/-/ansi-styles-3.2.1.tgz",
             "version": "3.2.1"
         },
-        "anymatch": {
-            "dev": true,
-            "integrity": "sha512-mM8522psRCqzV+6LhomX5wgp25YVibjh8Wj23I5RPkPppSVSjyKD2A2mBJmWGa+KN7f2D6LNh9jkBCeyLktzjg==",
-            "requires": {
-                "normalize-path": "^3.0.0",
-                "picomatch": "^2.0.4"
-            },
-            "resolved": "https://registry.npmjs.org/anymatch/-/anymatch-3.1.1.tgz",
-            "version": "3.1.1"
-        },
         "argparse": {
             "dev": true,
             "integrity": "sha512-8+9WqebbFzpX9OR+Wa6O29asIogeRMzcGtAINdpMHHyAg10f05aSFVBbcEqGf/PXw1EjAZ+q2/bEBg3DvurK3Q==",
             "resolved": "https://registry.npmjs.org/argparse/-/argparse-2.0.1.tgz",
             "version": "2.0.1"
         },
         "asn1.js": {
@@ -366,20 +428,14 @@
         },
         "balanced-match": {
             "dev": true,
             "integrity": "sha1-ibTRmasr7kneFk6gK4nORi1xt2c=",
             "resolved": "https://registry.npmjs.org/balanced-match/-/balanced-match-1.0.0.tgz",
             "version": "1.0.0"
         },
-        "base64-arraybuffer": {
-            "dev": true,
-            "integrity": "sha1-mBjHngWbE1X5fgQooBfIOOkLqBI=",
-            "resolved": "https://registry.npmjs.org/base64-arraybuffer/-/base64-arraybuffer-0.1.4.tgz",
-            "version": "0.1.4"
-        },
         "base64-js": {
             "dev": true,
             "integrity": "sha512-AKpaYlHn8t4SVbOHCy+b5+KKgvR4vrsD8vbvrbiQJps7fKDTkjkDry6ji0rUJjC0kzbNePLwzxq8iypo41qeWA==",
             "resolved": "https://registry.npmjs.org/base64-js/-/base64-js-1.5.1.tgz",
             "version": "1.5.1"
         },
         "base64id": {
@@ -403,29 +459,29 @@
             "dev": true,
             "integrity": "sha512-D7iWRBvnZE8ecXiLj/9wbxH7Tk79fAh8IHaTNq1RWRixsS02W+5qS+iE9yq6RYl0asXx5tw0bLhmT5pIfbSquw==",
             "resolved": "https://registry.npmjs.org/bn.js/-/bn.js-5.2.0.tgz",
             "version": "5.2.0"
         },
         "body-parser": {
             "dev": true,
-            "integrity": "sha512-dhEPs72UPbDnAQJ9ZKMNTP6ptJaionhP5cBb541nXPlW60Jepo9RV/a4fX4XWW9CuFNK22krhrj1+rgzifNCsw==",
+            "integrity": "sha512-SAAwOxgoCKMGs9uUAUFHygfLAyaniaoun6I8mFY9pRAJL9+Kec34aU+oIjDhTycub1jozEfEwx1W1IuOYxVSFw==",
             "requires": {
-                "bytes": "3.1.0",
+                "bytes": "3.1.2",
                 "content-type": "~1.0.4",
                 "debug": "2.6.9",
                 "depd": "~1.1.2",
-                "http-errors": "1.7.2",
+                "http-errors": "1.8.1",
                 "iconv-lite": "0.4.24",
                 "on-finished": "~2.3.0",
-                "qs": "6.7.0",
-                "raw-body": "2.4.0",
-                "type-is": "~1.6.17"
+                "qs": "6.9.7",
+                "raw-body": "2.4.3",
+                "type-is": "~1.6.18"
             },
-            "resolved": "https://registry.npmjs.org/body-parser/-/body-parser-1.19.0.tgz",
-            "version": "1.19.0"
+            "resolved": "https://registry.npmjs.org/body-parser/-/body-parser-1.19.2.tgz",
+            "version": "1.19.2"
         },
         "brace-expansion": {
             "dev": true,
             "integrity": "sha512-iCuPHDFgrHX7H2vEI/5xpz07zSHB00TpugqhmYtVmMO6518mCuRMoOYFldEBl0g187ufozdaHgWKcYFb61qGiA==",
             "requires": {
                 "balanced-match": "^1.0.0",
                 "concat-map": "0.0.1"
@@ -530,68 +586,73 @@
                 "safe-buffer": "^5.2.0"
             },
             "resolved": "https://registry.npmjs.org/browserify-sign/-/browserify-sign-4.2.1.tgz",
             "version": "4.2.1"
         },
         "browserslist": {
             "dev": true,
-            "integrity": "sha512-Wspk/PqO+4W9qp5iUTJsa1B/QrYn1keNCcEP5OvP7WBwT4KaDly0uONYmC6Xa3Z5IqnUgS0KcgLYu1l74x0ZXQ==",
+            "integrity": "sha512-tUkiguQGW7S3IhB7N+c2MV/HZPSCPAAiYBZXLsBhFB/PCy6ZKKsZrmBayHV9fdGV/ARIfJ14NkxKzRDjvp7L6w==",
             "requires": {
-                "caniuse-lite": "^1.0.30001219",
-                "colorette": "^1.2.2",
-                "electron-to-chromium": "^1.3.723",
-                "escalade": "^3.1.1",
-                "node-releases": "^1.1.71"
+                "caniuse-lite": "^1.0.30001449",
+                "electron-to-chromium": "^1.4.284",
+                "node-releases": "^2.0.8",
+                "update-browserslist-db": "^1.0.10"
             },
-            "resolved": "https://registry.npmjs.org/browserslist/-/browserslist-4.16.6.tgz",
-            "version": "4.16.6"
+            "resolved": "https://registry.npmjs.org/browserslist/-/browserslist-4.21.5.tgz",
+            "version": "4.21.5"
         },
         "buffer": {
             "dev": true,
             "integrity": "sha512-FTiCpNxtwiZZHEZbcbTIcZjERVICn9yq/pDFkTl95/AxzD1naBctN7YO68riM/gLSDY7sdrMby8hofADYuuqOA==",
             "requires": {
                 "base64-js": "^1.3.1",
                 "ieee754": "^1.2.1"
             },
             "resolved": "https://registry.npmjs.org/buffer/-/buffer-6.0.3.tgz",
             "version": "6.0.3"
         },
         "buffer-from": {
             "dev": true,
-            "integrity": "sha512-MQcXEUbCKtEo7bhqEs6560Hyd4XaovZlO/k9V3hjVUF/zwW7KBVdSK4gIt/bzwS9MbR5qob+F5jusZsb0YQK2A==",
-            "resolved": "https://registry.npmjs.org/buffer-from/-/buffer-from-1.1.1.tgz",
-            "version": "1.1.1"
+            "integrity": "sha512-E+XQCRwSbaaiChtv6k6Dwgc+bx+Bs6vuKJHHl5kox/BaKbhiXzqQOwK4cO22yElGp2OCmjwVhT3HmxgyPGnJfQ==",
+            "resolved": "https://registry.npmjs.org/buffer-from/-/buffer-from-1.1.2.tgz",
+            "version": "1.1.2"
         },
         "buffer-xor": {
             "dev": true,
             "integrity": "sha1-JuYe0UIvtw3ULm42cp7VHYVf6Nk=",
             "resolved": "https://registry.npmjs.org/buffer-xor/-/buffer-xor-1.0.3.tgz",
             "version": "1.0.3"
         },
         "bytes": {
             "dev": true,
-            "integrity": "sha512-zauLjrfCG+xvoyaqLoV8bLVXXNGC4JqlxFCutSDWA6fJrTo2ZuvLYTqZ7aHBLZSMOopbzwv8f+wZcVzfVTI2Dg==",
-            "resolved": "https://registry.npmjs.org/bytes/-/bytes-3.1.0.tgz",
-            "version": "3.1.0"
+            "integrity": "sha512-/Nf7TyzTx6S3yRJObOAV7956r8cr2+Oj8AC5dt8wSP3BQAoeX58NoHyCU8P8zGkNXStjTSi6fzO6F0pBdcYbEg==",
+            "resolved": "https://registry.npmjs.org/bytes/-/bytes-3.1.2.tgz",
+            "version": "3.1.2"
         },
         "call-bind": {
             "dev": true,
             "integrity": "sha512-7O+FbCihrB5WGbFYesctwmTKae6rOiIzmz1icreWJ+0aA7LJfuqhEso2T9ncpcFtzMQtzXf2QGGueWJGTYsqrA==",
             "requires": {
                 "function-bind": "^1.1.1",
                 "get-intrinsic": "^1.0.2"
             },
             "resolved": "https://registry.npmjs.org/call-bind/-/call-bind-1.0.2.tgz",
             "version": "1.0.2"
         },
+        "camelcase": {
+            "dev": true,
+            "integrity": "sha512-Gmy6FhYlCY7uOElZUSbxo2UCDH8owEk996gkbrpsgGtrJLM3J7jGxl9Ic7Qwwj4ivOE5AWZWRMecDdF7hqGjFA==",
+            "resolved": "https://registry.npmjs.org/camelcase/-/camelcase-6.3.0.tgz",
+            "version": "6.3.0"
+        },
         "caniuse-lite": {
             "dev": true,
-            "integrity": "sha512-pDHgRndit6p1NR2GhzMbQ6CkRrp4VKuSsqbcLeOQppYPKOYkKT/6ZvZDvKJUqcmtyWIAHuZq3SVS2vc1egCZzw==",
-            "resolved": "https://registry.npmjs.org/caniuse-lite/-/caniuse-lite-1.0.30001237.tgz",
-            "version": "1.0.30001237"
+            "integrity": "sha512-KCqHwRnaa1InZBtqXzP98LPg0ajCVujMKjqKDhZEthIpAsJl/YEIa3YvXjGXPVqzZVguccuu7ga9KOE1J9rKPQ==",
+            "resolved": "https://registry.npmjs.org/caniuse-lite/-/caniuse-lite-1.0.30001481.tgz",
+            "version": "1.0.30001481"
         },
         "chalk": {
             "dependencies": {
                 "supports-color": {
                     "dev": true,
                     "integrity": "sha512-QjVjwdXIt408MIiAqCX4oUKsgU2EqAGzs2Ppkm4aQYbjm+ZEWEcW4SfFNTr4uMNZma0ey4f5lgLrkB0aX0QMow==",
                     "requires": {
@@ -621,27 +682,27 @@
                         "picomatch": "^2.0.4"
                     },
                     "resolved": "https://registry.npmjs.org/anymatch/-/anymatch-3.1.2.tgz",
                     "version": "3.1.2"
                 }
             },
             "dev": true,
-            "integrity": "sha512-ekGhOnNVPgT77r4K/U3GDhu+FQ2S8TnK/s2KbIGXi0SZWuwkZ2QNyfWdZW+TVfn84DpEP7rLeCt2UI6bJ8GwbQ==",
+            "integrity": "sha512-Dr3sfKRP6oTcjf2JmUmFJfeVMvXBdegxB0iVQ5eb2V10uFJUCAS8OByZdVAyVb8xXNz3GjjTgj9kLWsZTqE6kw==",
             "requires": {
                 "anymatch": "~3.1.2",
                 "braces": "~3.0.2",
                 "fsevents": "~2.3.2",
                 "glob-parent": "~5.1.2",
                 "is-binary-path": "~2.1.0",
                 "is-glob": "~4.0.1",
                 "normalize-path": "~3.0.0",
                 "readdirp": "~3.6.0"
             },
-            "resolved": "https://registry.npmjs.org/chokidar/-/chokidar-3.5.2.tgz",
-            "version": "3.5.2"
+            "resolved": "https://registry.npmjs.org/chokidar/-/chokidar-3.5.3.tgz",
+            "version": "3.5.3"
         },
         "chrome-trace-event": {
             "dev": true,
             "integrity": "sha512-p3KULyQg4S7NIHixdwbGX+nFHkoBiA4YQmyWtjb8XngSKV124nJmRysgAeujbUVb15vh+RvFUfCPqU7rXk+hZg==",
             "resolved": "https://registry.npmjs.org/chrome-trace-event/-/chrome-trace-event-1.0.3.tgz",
             "version": "1.0.3"
         },
@@ -653,20 +714,14 @@
                 "safe-buffer": "^5.0.1"
             },
             "resolved": "https://registry.npmjs.org/cipher-base/-/cipher-base-1.0.4.tgz",
             "version": "1.0.4"
         },
         "cliui": {
             "dependencies": {
-                "ansi-regex": {
-                    "dev": true,
-                    "integrity": "sha512-bY6fj56OUQ0hU1KjFNDQuJFezqKdrAyFdIevADiqrWHwSlbmBNMHp5ak2f40Pm8JTFyM2mqxkG6ngkHO11f/lg==",
-                    "resolved": "https://registry.npmjs.org/ansi-regex/-/ansi-regex-5.0.0.tgz",
-                    "version": "5.0.0"
-                },
                 "is-fullwidth-code-point": {
                     "dev": true,
                     "integrity": "sha512-zymm5+u+sCsSWyD9qNaejV3DFvhCKclKdizYaJUuHA83RLjb7nSuGnddCHGv0hk+KY7BMAlsWeK4Ueg6EV6XQg==",
                     "resolved": "https://registry.npmjs.org/is-fullwidth-code-point/-/is-fullwidth-code-point-3.0.0.tgz",
                     "version": "3.0.0"
                 },
                 "string-width": {
@@ -711,38 +766,26 @@
         },
         "color-name": {
             "dev": true,
             "integrity": "sha1-p9BVi9icQveV3UIyj3QIMcpTvCU=",
             "resolved": "https://registry.npmjs.org/color-name/-/color-name-1.1.3.tgz",
             "version": "1.1.3"
         },
-        "colorette": {
-            "dev": true,
-            "integrity": "sha512-MKGMzyfeuutC/ZJ1cba9NqcNpfeqMUcYmyF1ZFY6/Cn7CNSAKx6a+s48sqLqyAiZuaP2TcqMhoo+dlwFnVxT9w==",
-            "resolved": "https://registry.npmjs.org/colorette/-/colorette-1.2.2.tgz",
-            "version": "1.2.2"
-        },
         "colors": {
             "dev": true,
             "integrity": "sha512-a+UqTh4kgZg/SlGvfbzDHpgRu7AAQOmmqRHJnxhRZICKFUT91brVhNNt58CMWU9PsBbv3PDCZUHbVxuDiH2mtA==",
             "resolved": "https://registry.npmjs.org/colors/-/colors-1.4.0.tgz",
             "version": "1.4.0"
         },
         "commander": {
             "dev": true,
             "integrity": "sha512-GpVkmM8vF2vQUkj2LvZmD35JxeJOLCwJ9cUkugyk2nuhbv3+mJvpLYYt+0+USMxE+oj+ey/lJEnhZw75x/OMcQ==",
             "resolved": "https://registry.npmjs.org/commander/-/commander-2.20.3.tgz",
             "version": "2.20.3"
         },
-        "component-emitter": {
-            "dev": true,
-            "integrity": "sha512-Rd3se6QB+sO1TwqZjscQrurpEPIfO0/yYnSin6Q/rD3mOutHvUrCAhJub3r90uNb+SESBuE0QYoB90YdfatsRg==",
-            "resolved": "https://registry.npmjs.org/component-emitter/-/component-emitter-1.3.0.tgz",
-            "version": "1.3.0"
-        },
         "concat-map": {
             "dev": true,
             "integrity": "sha1-2Klr13/Wjfd5OnMDajug1UBdR3s=",
             "resolved": "https://registry.npmjs.org/concat-map/-/concat-map-0.0.1.tgz",
             "version": "0.0.1"
         },
         "connect": {
@@ -761,17 +804,17 @@
             "dev": true,
             "integrity": "sha512-hIP3EEPs8tB9AT1L+NUqtwOAps4mk2Zob89MWXMHjHWg9milF/j4osnnQLXBCBFBk/tvIG/tUc9mOUJiPBhPXA==",
             "resolved": "https://registry.npmjs.org/content-type/-/content-type-1.0.4.tgz",
             "version": "1.0.4"
         },
         "cookie": {
             "dev": true,
-            "integrity": "sha512-ZwrFkGJxUR3EIoXtO+yVE69Eb7KlixbaeAWfBQB9vVsNn/o+Yw69gBWSSDK825hQNdN+wF8zELf3dFNl/kxkUA==",
-            "resolved": "https://registry.npmjs.org/cookie/-/cookie-0.4.1.tgz",
-            "version": "0.4.1"
+            "integrity": "sha512-aSWTXFzaKWkvHO1Ny/s+ePFpvKsPnjc551iI41v3ny/ow6tBG5Vd+FuqGNhh1LxOmVzOlGUriIlOaokOvhaStA==",
+            "resolved": "https://registry.npmjs.org/cookie/-/cookie-0.4.2.tgz",
+            "version": "0.4.2"
         },
         "core-js": {
             "dev": true,
             "integrity": "sha512-Kb2wC0fvsWfQrgk8HU5lW6U/Lcs8+9aaYcy4ZFc6DDlo4nZ7n70dEgE5rtR0oG6ufKDUnrwfWL1mXR5ljDatrQ==",
             "resolved": "https://registry.npmjs.org/core-js/-/core-js-2.6.12.tgz",
             "version": "2.6.12"
         },
@@ -853,27 +896,33 @@
             "dev": true,
             "integrity": "sha1-XQKkaFCt8bSjF5RqOSj8y1v9BCU=",
             "resolved": "https://registry.npmjs.org/custom-event/-/custom-event-1.0.1.tgz",
             "version": "1.0.1"
         },
         "date-format": {
             "dev": true,
-            "integrity": "sha512-eyTcpKOcamdhWJXj56DpQMo1ylSQpcGtGKXcU0Tb97+K56/CF5amAqqqNj0+KvA0iw2ynxtHWFsPDSClCxe48w==",
-            "resolved": "https://registry.npmjs.org/date-format/-/date-format-3.0.0.tgz",
-            "version": "3.0.0"
+            "integrity": "sha512-7P3FyqDcfeznLZp2b+OMitV9Sz2lUnsT87WaTat9nVwqsBkTzPG3lPLNwW3en6F4pHUiWzr6vb8CLhjdK9bcxQ==",
+            "resolved": "https://registry.npmjs.org/date-format/-/date-format-4.0.3.tgz",
+            "version": "4.0.3"
         },
         "debug": {
             "dev": true,
             "integrity": "sha512-bC7ElrdJaJnPbAP+1EotYvqZsb3ecl5wi6Bfi6BJTUcNowp6cvspg0jXznRTKDjm/E7AdgFBVeAPVMNcKGsHMA==",
             "requires": {
                 "ms": "2.0.0"
             },
             "resolved": "https://registry.npmjs.org/debug/-/debug-2.6.9.tgz",
             "version": "2.6.9"
         },
+        "decamelize": {
+            "dev": true,
+            "integrity": "sha512-9iE1PgSik9HeIIw2JO94IidnE3eBoQrFJ3w7sFuzSX4DpmZ3v5sZpUiV5Swcf6mQEF+Y0ru8Neo+p+nyh2J+hQ==",
+            "resolved": "https://registry.npmjs.org/decamelize/-/decamelize-4.0.0.tgz",
+            "version": "4.0.0"
+        },
         "define-properties": {
             "dev": true,
             "integrity": "sha512-3MqfYKj2lLzdMSf8ZIZE/V+Zuy+BgD6f164e8K2w7dgnpKArBDerGYpM46IYYcjnkdPNMjPk9A6VFB8+3SKlXQ==",
             "requires": {
                 "object-keys": "^1.0.12"
             },
             "resolved": "https://registry.npmjs.org/define-properties/-/define-properties-1.1.3.tgz",
@@ -942,17 +991,17 @@
             "dev": true,
             "integrity": "sha1-WQxhFWsK4vTwJVcyoViyZrxWsh0=",
             "resolved": "https://registry.npmjs.org/ee-first/-/ee-first-1.1.1.tgz",
             "version": "1.1.1"
         },
         "electron-to-chromium": {
             "dev": true,
-            "integrity": "sha512-2Tg+7jSl3oPxgsBsWKh5H83QazTkmWG/cnNwJplmyZc7KcN61+I10oUgaXSVk/NwfvN3BdkKDR4FYuRBQQ2v0A==",
-            "resolved": "https://registry.npmjs.org/electron-to-chromium/-/electron-to-chromium-1.3.752.tgz",
-            "version": "1.3.752"
+            "integrity": "sha512-LfxbHXdA/S+qyoTEA4EbhxGjrxx7WK2h6yb5K2v0UCOufUKX+VZaHbl3svlzZfv9sGseym/g3Ne4DpsgRULmqg==",
+            "resolved": "https://registry.npmjs.org/electron-to-chromium/-/electron-to-chromium-1.4.369.tgz",
+            "version": "1.4.369"
         },
         "elliptic": {
             "dependencies": {
                 "bn.js": {
                     "dev": true,
                     "integrity": "sha512-c98Bf3tPniI+scsdk237ku1Dc3ujXQTSgyiPUDEOe7tRkhrqridvh8klBv0HCEso1OLOYcHuCv/cS6DNxKH+ZA==",
                     "resolved": "https://registry.npmjs.org/bn.js/-/bn.js-4.12.0.tgz",
@@ -991,60 +1040,63 @@
             "resolved": "https://registry.npmjs.org/encodeurl/-/encodeurl-1.0.2.tgz",
             "version": "1.0.2"
         },
         "engine.io": {
             "dependencies": {
                 "debug": {
                     "dev": true,
-                    "integrity": "sha512-mOp8wKcvj7XxC78zLgw/ZA+6TSgkoE2C/ienthhRD298T7UNwAg9diBpLRxC0mOezLl4B0xV7M0cCO6P/O0Xhw==",
+                    "integrity": "sha512-PRWFHuSU3eDtQJPvnNY7Jcket1j0t5OuOsFzPPzsekD52Zl8qUfFIPEiswXqIvHWGVHOgX+7G/vCNNhehwxfkQ==",
                     "requires": {
                         "ms": "2.1.2"
                     },
-                    "resolved": "https://registry.npmjs.org/debug/-/debug-4.3.2.tgz",
-                    "version": "4.3.2"
+                    "resolved": "https://registry.npmjs.org/debug/-/debug-4.3.4.tgz",
+                    "version": "4.3.4"
                 },
                 "ms": {
                     "dev": true,
                     "integrity": "sha512-sGkPx+VjMtmA6MX27oA4FBFELFCZZ4S4XqeGOXCv68tT+jb3vk/RyaKWP0PTKyWtmLSM0b+adUTEvbs1PEaH2w==",
                     "resolved": "https://registry.npmjs.org/ms/-/ms-2.1.2.tgz",
                     "version": "2.1.2"
                 }
             },
             "dev": true,
-            "integrity": "sha512-t2E9wLlssQjGw0nluF6aYyfX8LwYU8Jj0xct+pAhfWfv/YrBn6TSNtEYsgxHIfaMqfrLx07czcMg9bMN6di+3w==",
+            "integrity": "sha512-FKn/3oMiJjrOEOeUub2WCox6JhxBXq/Zn3fZOMCBxKnNYtsdKjxhl7yR3fZhM9PV+rdE75SU5SYMc+2PGzo+Tg==",
             "requires": {
+                "@types/cookie": "^0.4.1",
+                "@types/cors": "^2.8.12",
+                "@types/node": ">=10.0.0",
                 "accepts": "~1.3.4",
                 "base64id": "2.0.0",
                 "cookie": "~0.4.1",
                 "cors": "~2.8.5",
                 "debug": "~4.3.1",
-                "engine.io-parser": "~4.0.0",
-                "ws": "~7.4.2"
+                "engine.io-parser": "~5.0.3",
+                "ws": "~8.11.0"
             },
-            "resolved": "https://registry.npmjs.org/engine.io/-/engine.io-4.1.1.tgz",
-            "version": "4.1.1"
+            "resolved": "https://registry.npmjs.org/engine.io/-/engine.io-6.4.2.tgz",
+            "version": "6.4.2"
         },
         "engine.io-parser": {
             "dev": true,
-            "integrity": "sha512-sHfEQv6nmtJrq6TKuIz5kyEKH/qSdK56H/A+7DnAuUPWosnIZAS2NHNcPLmyjtY3cGS/MqJdZbUjW97JU72iYg==",
+            "integrity": "sha512-BtQxwF27XUNnSafQLvDi0dQ8s3i6VgzSoQMJacpIcGNrlUdfHSKbgm3jmjCVvQluGzqwujQMPAoMai3oYSTurg==",
             "requires": {
-                "base64-arraybuffer": "0.1.4"
+                "@socket.io/base64-arraybuffer": "~1.0.2"
             },
-            "resolved": "https://registry.npmjs.org/engine.io-parser/-/engine.io-parser-4.0.2.tgz",
-            "version": "4.0.2"
+            "resolved": "https://registry.npmjs.org/engine.io-parser/-/engine.io-parser-5.0.3.tgz",
+            "version": "5.0.3"
         },
         "enhanced-resolve": {
             "dev": true,
-            "integrity": "sha512-F27oB3WuHDzvR2DOGNTaYy0D5o0cnrv8TeI482VM4kYgQd/FT9lUQwuNsJ0oOHtBUq7eiW5ytqzp7nBFknL+GA==",
+            "integrity": "sha512-eyV8f0y1+bzyfh8xAwW/WTSZpLbjhqc4ne9eGSH4Zo2ejdyiNG9pU6mf9DG8a7+Auk6MFTlNOT4Y2y/9k8GKVg==",
             "requires": {
                 "graceful-fs": "^4.2.4",
                 "tapable": "^2.2.0"
             },
-            "resolved": "https://registry.npmjs.org/enhanced-resolve/-/enhanced-resolve-5.8.2.tgz",
-            "version": "5.8.2"
+            "resolved": "https://registry.npmjs.org/enhanced-resolve/-/enhanced-resolve-5.13.0.tgz",
+            "version": "5.13.0"
         },
         "ent": {
             "dev": true,
             "integrity": "sha1-6WQhkyWiHQX0RGai9obtbOX13R0=",
             "resolved": "https://registry.npmjs.org/ent/-/ent-2.2.0.tgz",
             "version": "2.2.0"
         },
@@ -1096,17 +1148,17 @@
                 "unbox-primitive": "^1.0.1"
             },
             "resolved": "https://registry.npmjs.org/es-abstract/-/es-abstract-1.18.3.tgz",
             "version": "1.18.3"
         },
         "es-module-lexer": {
             "dev": true,
-            "integrity": "sha512-ooYciCUtfw6/d2w56UVeqHPcoCFAiJdz5XOkYpv/Txl1HMUozpXjz/2RIQgqwKdXNDPSF1W7mJCFse3G+HDyAA==",
-            "resolved": "https://registry.npmjs.org/es-module-lexer/-/es-module-lexer-0.4.1.tgz",
-            "version": "0.4.1"
+            "integrity": "sha512-1HQ2M2sPtxwnvOvT1ZClHyQDiggdNjURWpY2we6aMKCQiUVxTmVs2UYPLIrD84sS+kMdUwfBSylbJPwNnBrnHQ==",
+            "resolved": "https://registry.npmjs.org/es-module-lexer/-/es-module-lexer-0.9.3.tgz",
+            "version": "0.9.3"
         },
         "es-to-primitive": {
             "dev": true,
             "integrity": "sha512-QCOllgZJtaUo9miYBcLChTUaHNjJF3PYs1VidD7AwiEj1kYxKeQTctLAezAOH5ZKRH0g2IgPn6KwB4IT8iRpvA==",
             "requires": {
                 "is-callable": "^1.1.4",
                 "is-date-object": "^1.0.1",
@@ -1149,17 +1201,17 @@
             "resolved": "https://registry.npmjs.org/eslint-scope/-/eslint-scope-5.1.1.tgz",
             "version": "5.1.1"
         },
         "esrecurse": {
             "dependencies": {
                 "estraverse": {
                     "dev": true,
-                    "integrity": "sha512-BxbNGGNm0RyRYvUdHpIwv9IWzeM9XClbOxwoATuFdOE7ZE6wHL+HQ5T8hoPM+zHvmKzzsEqhgy0GrQ5X13afiQ==",
-                    "resolved": "https://registry.npmjs.org/estraverse/-/estraverse-5.2.0.tgz",
-                    "version": "5.2.0"
+                    "integrity": "sha512-MMdARuVEQziNTeJD8DgMqmhwR11BRQ/cBP+pLtYdSTnf3MIO8fFeiINEbX36ZdNlfU/7A9f3gUw49B3oQsvwBA==",
+                    "resolved": "https://registry.npmjs.org/estraverse/-/estraverse-5.3.0.tgz",
+                    "version": "5.3.0"
                 }
             },
             "dev": true,
             "integrity": "sha512-KmfKL3b6G+RXvP8N1vr3Tq1kL/oCFgn2NYXEtqP8/L3pKapUA4G8cFVaoF3SU323CD4XypR/ffioHmkti6/Tag==",
             "requires": {
                 "estraverse": "^5.2.0"
             },
@@ -1232,48 +1284,58 @@
                 "parseurl": "~1.3.3",
                 "statuses": "~1.5.0",
                 "unpipe": "~1.0.0"
             },
             "resolved": "https://registry.npmjs.org/finalhandler/-/finalhandler-1.1.2.tgz",
             "version": "1.1.2"
         },
+        "find-up": {
+            "dev": true,
+            "integrity": "sha512-78/PXT1wlLLDgTzDs7sjq9hzz0vXD+zn+7wypEe4fXQxCmdmqfGsEPQxmiCSQI3ajFV91bVSsvNtrJRiW6nGng==",
+            "requires": {
+                "locate-path": "^6.0.0",
+                "path-exists": "^4.0.0"
+            },
+            "resolved": "https://registry.npmjs.org/find-up/-/find-up-5.0.0.tgz",
+            "version": "5.0.0"
+        },
         "flat": {
             "dev": true,
             "integrity": "sha512-b6suED+5/3rTpUBdG1gupIl8MPFCAMA0QXwmljLhvCUKcUvdE4gWky9zpuGCcXHOsz4J9wPGNWq6OKpmIzz3hQ==",
             "resolved": "https://registry.npmjs.org/flat/-/flat-5.0.2.tgz",
             "version": "5.0.2"
         },
         "flatted": {
             "dev": true,
-            "integrity": "sha512-r5wGx7YeOwNWNlCA0wQ86zKyDLMQr+/RB8xy74M4hTphfmjlijTSSXGuH8rnvKZnfT9i+75zmd8jcKdMR4O6jA==",
-            "resolved": "https://registry.npmjs.org/flatted/-/flatted-2.0.2.tgz",
-            "version": "2.0.2"
+            "integrity": "sha512-WIWGi2L3DyTUvUrwRKgGi9TwxQMUEqPOPQBVi71R96jZXJdFskXEmf54BoZaS1kknGODoIGASGEzBUYdyMCBJg==",
+            "resolved": "https://registry.npmjs.org/flatted/-/flatted-3.2.5.tgz",
+            "version": "3.2.5"
         },
         "follow-redirects": {
             "dev": true,
-            "integrity": "sha512-HWqDgT7ZEkqRzBvc2s64vSZ/hfOceEol3ac/7tKwzuvEyWx3/4UegXh5oBOIotkGsObyk3xznnSRVADBgWSQVg==",
-            "resolved": "https://registry.npmjs.org/follow-redirects/-/follow-redirects-1.14.1.tgz",
-            "version": "1.14.1"
+            "integrity": "sha512-MQDfihBQYMcyy5dhRDJUHcw7lb2Pv/TuE6xP1vyraLukNDHKbDxDNaOE3NbCAdKQApno+GPRyo1YAp89yCjK4w==",
+            "resolved": "https://registry.npmjs.org/follow-redirects/-/follow-redirects-1.14.9.tgz",
+            "version": "1.14.9"
         },
         "foreach": {
             "dev": true,
             "integrity": "sha1-C+4AUBiusmDQo6865ljdATbsG5k=",
             "resolved": "https://registry.npmjs.org/foreach/-/foreach-2.0.5.tgz",
             "version": "2.0.5"
         },
         "fs-extra": {
             "dev": true,
-            "integrity": "sha512-yhlQgA6mnOJUKOsRUFsgJdQCvkKhcz8tlZG5HBQfReYZy46OwLcY+Zia0mtdHsOo9y/hP+CxMN0TU9QxoOtG4g==",
+            "integrity": "sha512-NbdoVMZso2Lsrn/QwLXOy6rm0ufY2zEOKCDzJR/0kBsb0E6qed0P3iYK+Ath3BfvXEeu4JhEtXLgILx5psUfag==",
             "requires": {
                 "graceful-fs": "^4.2.0",
-                "jsonfile": "^4.0.0",
-                "universalify": "^0.1.0"
+                "jsonfile": "^6.0.1",
+                "universalify": "^2.0.0"
             },
-            "resolved": "https://registry.npmjs.org/fs-extra/-/fs-extra-8.1.0.tgz",
-            "version": "8.1.0"
+            "resolved": "https://registry.npmjs.org/fs-extra/-/fs-extra-10.0.1.tgz",
+            "version": "10.0.1"
         },
         "fs.realpath": {
             "dev": true,
             "integrity": "sha1-FQStJSMVjKpA20onh8sBQRmU6k8=",
             "resolved": "https://registry.npmjs.org/fs.realpath/-/fs.realpath-1.0.0.tgz",
             "version": "1.0.0"
         },
@@ -1346,20 +1408,14 @@
         },
         "graceful-fs": {
             "dev": true,
             "integrity": "sha512-WjKPNJF79dtJAVniUlGGWHYGz2jWxT6VhN/4m1NdkbZ2nOsEF+cI1Edgql5zCRhs/VsQYRvrXctxktVXZUkixw==",
             "resolved": "https://registry.npmjs.org/graceful-fs/-/graceful-fs-4.2.4.tgz",
             "version": "4.2.4"
         },
-        "growl": {
-            "dev": true,
-            "integrity": "sha512-qBr4OuELkhPenW6goKVXiv47US3clb3/IbuWF9KNKEijAy9oeHxU9IgzjvJhHkUzhaj7rOUD7+YGWqUjLp5oSA==",
-            "resolved": "https://registry.npmjs.org/growl/-/growl-1.10.5.tgz",
-            "version": "1.10.5"
-        },
         "has": {
             "dev": true,
             "integrity": "sha512-f2dvO0VU6Oej7RkWJGrehjbzMAjFp5/VKPp5tTpWIV4JHHZK1/BxbFRtf/siA2SWTe09caDmVtYYzWEIbBS4zw==",
             "requires": {
                 "function-bind": "^1.1.1"
             },
             "resolved": "https://registry.npmjs.org/has/-/has-1.0.3.tgz",
@@ -1426,25 +1482,33 @@
                 "minimalistic-assert": "^1.0.0",
                 "minimalistic-crypto-utils": "^1.0.1"
             },
             "resolved": "https://registry.npmjs.org/hmac-drbg/-/hmac-drbg-1.0.1.tgz",
             "version": "1.0.1"
         },
         "http-errors": {
+            "dependencies": {
+                "inherits": {
+                    "dev": true,
+                    "integrity": "sha512-k/vGaX4/Yla3WzyMCvTQOXYeIHvqOKtnqBduzTHpzpQZzAskKMhZ2K+EnBiSM9zGSoIFeMpXKxa4dYeZIQqewQ==",
+                    "resolved": "https://registry.npmjs.org/inherits/-/inherits-2.0.4.tgz",
+                    "version": "2.0.4"
+                }
+            },
             "dev": true,
-            "integrity": "sha512-uUQBt3H/cSIVfch6i1EuPNy/YsRSOUBXTVfZ+yR7Zjez3qjBz6i9+i4zjNaoqcoFVI4lQJ5plg63TvGfRSDCRg==",
+            "integrity": "sha512-Kpk9Sm7NmI+RHhnj6OIWDI1d6fIoFAtFt9RLaTMRlg/8w49juAStsrBgp0Dp4OdxdVbRIeKhtCUvoi/RuAhO4g==",
             "requires": {
                 "depd": "~1.1.2",
-                "inherits": "2.0.3",
-                "setprototypeof": "1.1.1",
+                "inherits": "2.0.4",
+                "setprototypeof": "1.2.0",
                 "statuses": ">= 1.5.0 < 2",
-                "toidentifier": "1.0.0"
+                "toidentifier": "1.0.1"
             },
-            "resolved": "https://registry.npmjs.org/http-errors/-/http-errors-1.7.2.tgz",
-            "version": "1.7.2"
+            "resolved": "https://registry.npmjs.org/http-errors/-/http-errors-1.8.1.tgz",
+            "version": "1.8.1"
         },
         "http-proxy": {
             "dev": true,
             "integrity": "sha512-7mz/721AbnJwIVbnaSv1Cz3Am0ZLT/UBwkC92VlxhXv/k/BBQfM2fXElQNC27BVGr0uwUpplYPQM9LnaBMR5NQ==",
             "requires": {
                 "eventemitter3": "^4.0.0",
                 "follow-redirects": "^1.0.0",
@@ -1537,20 +1601,14 @@
         },
         "is-extglob": {
             "dev": true,
             "integrity": "sha1-qIwCU1eR8C7TfHahueqXc8gz+MI=",
             "resolved": "https://registry.npmjs.org/is-extglob/-/is-extglob-2.1.1.tgz",
             "version": "2.1.1"
         },
-        "is-fullwidth-code-point": {
-            "dev": true,
-            "integrity": "sha1-o7MKXE8ZkYMWeqq5O+764937ZU8=",
-            "resolved": "https://registry.npmjs.org/is-fullwidth-code-point/-/is-fullwidth-code-point-2.0.0.tgz",
-            "version": "2.0.0"
-        },
         "is-generator-function": {
             "dev": true,
             "integrity": "sha512-ZJ34p1uvIfptHCN7sFTjGibB9/oBg17sHqzDLfuwhvmN/qLVvIQXRQ8licZQ35WJ8KuEQt/etnnzQFI9C9Ue/A==",
             "resolved": "https://registry.npmjs.org/is-generator-function/-/is-generator-function-1.0.9.tgz",
             "version": "1.0.9"
         },
         "is-glob": {
@@ -1654,14 +1712,20 @@
                 "es-abstract": "^1.18.0-next.2",
                 "foreach": "^2.0.5",
                 "has-symbols": "^1.0.1"
             },
             "resolved": "https://registry.npmjs.org/is-typed-array/-/is-typed-array-1.1.5.tgz",
             "version": "1.1.5"
         },
+        "is-unicode-supported": {
+            "dev": true,
+            "integrity": "sha512-knxG2q4UC3u8stRGyAVJCOdxFmv5DZiRcdlIaAQXAbSfJya+OhopNotLQrstBhququ4ZpuKbDc/8S6mgXgPFPw==",
+            "resolved": "https://registry.npmjs.org/is-unicode-supported/-/is-unicode-supported-0.1.0.tgz",
+            "version": "0.1.0"
+        },
         "is-wsl": {
             "dev": true,
             "integrity": "sha512-fKzAra0rGJUUBwGBgNkHZuToZcn+TtXHpeCgmkMJMMYx1sQDYaCSyjJBSCa2nH1DGm7s3n1oBnohoVTBaN7Lww==",
             "requires": {
                 "is-docker": "^2.0.0"
             },
             "resolved": "https://registry.npmjs.org/is-wsl/-/is-wsl-2.2.0.tgz",
@@ -1669,125 +1733,115 @@
         },
         "isbinaryfile": {
             "dev": true,
             "integrity": "sha512-53h6XFniq77YdW+spoRrebh0mnmTxRPTlcuIArO57lmMdq4uBKFKaeTjnb92oYWrSn/LVL+LT+Hap2tFQj8V+w==",
             "resolved": "https://registry.npmjs.org/isbinaryfile/-/isbinaryfile-4.0.8.tgz",
             "version": "4.0.8"
         },
-        "isexe": {
-            "dev": true,
-            "integrity": "sha1-6PvzdNxVb/iUehDcsFctYz8s+hA=",
-            "resolved": "https://registry.npmjs.org/isexe/-/isexe-2.0.0.tgz",
-            "version": "2.0.0"
-        },
         "jest-worker": {
             "dev": true,
-            "integrity": "sha512-EoBdilOTTyOgmHXtw/cPc+ZrCA0KJMrkXzkrPGNwLmnvvlN1nj7MPrxpT7m+otSv2e1TLaVffzDnE/LB14zJMg==",
+            "integrity": "sha512-7vuh85V5cdDofPyxn58nrPjBktZo0u9x1g8WtjQol+jZDaE+fhN+cIvTj11GndBnMnyfrUOG1sZQxCdjKh+DKg==",
             "requires": {
                 "@types/node": "*",
                 "merge-stream": "^2.0.0",
                 "supports-color": "^8.0.0"
             },
-            "resolved": "https://registry.npmjs.org/jest-worker/-/jest-worker-27.0.2.tgz",
-            "version": "27.0.2"
+            "resolved": "https://registry.npmjs.org/jest-worker/-/jest-worker-27.5.1.tgz",
+            "version": "27.5.1"
         },
         "js-yaml": {
             "dev": true,
-            "integrity": "sha512-pqon0s+4ScYUvX30wxQi3PogGFAlUyH0awepWvwkj4jD4v+ova3RiYw8bmA6x2rDrEaj8i/oWKoRxpVNW+Re8Q==",
+            "integrity": "sha512-wpxZs9NoxZaJESJGIZTyDEaYpl0FKSA+FB9aJiyemKhMwkxQg63h4T1KJgUGHpTqPDNRcmmYLugrRjJlBtWvRA==",
             "requires": {
                 "argparse": "^2.0.1"
             },
-            "resolved": "https://registry.npmjs.org/js-yaml/-/js-yaml-4.0.0.tgz",
-            "version": "4.0.0"
+            "resolved": "https://registry.npmjs.org/js-yaml/-/js-yaml-4.1.0.tgz",
+            "version": "4.1.0"
         },
-        "json-parse-better-errors": {
+        "json-parse-even-better-errors": {
             "dev": true,
-            "integrity": "sha512-mrqyZKfX5EhL7hvqcV6WG1yYjnjeuYDzDhhcAAUrq8Po85NBQBJP+ZDUT75qZQ98IkUoBqdkExkukOU7Ts2wrw==",
-            "resolved": "https://registry.npmjs.org/json-parse-better-errors/-/json-parse-better-errors-1.0.2.tgz",
-            "version": "1.0.2"
+            "integrity": "sha512-xyFwyhro/JEof6Ghe2iz2NcXoj2sloNsWr/XsERDK/oiPCfaNhl5ONfp+jQdAZRQQ0IJWNzH9zIZF7li91kh2w==",
+            "resolved": "https://registry.npmjs.org/json-parse-even-better-errors/-/json-parse-even-better-errors-2.3.1.tgz",
+            "version": "2.3.1"
         },
         "json-schema-traverse": {
             "dev": true,
             "integrity": "sha512-xbbCH5dCYU5T8LcEhhuh7HJ88HXuW3qsI3Y0zOZFKfZEHcpWiHU/Jxzk629Brsab/mMiHQti9wMP+845RPe3Vg==",
             "resolved": "https://registry.npmjs.org/json-schema-traverse/-/json-schema-traverse-0.4.1.tgz",
             "version": "0.4.1"
         },
         "jsonfile": {
             "dev": true,
-            "integrity": "sha1-h3Gq4HmbZAdrdmQPygWPnBDjPss=",
+            "integrity": "sha512-5dgndWOriYSm5cnYaJNhalLNDKOqFwyDB/rr1E9ZsGciGvKPs8R2xYGCacuf3z6K1YKDz182fd+fY3cn3pMqXQ==",
             "requires": {
-                "graceful-fs": "^4.1.6"
+                "graceful-fs": "^4.1.6",
+                "universalify": "^2.0.0"
             },
-            "resolved": "https://registry.npmjs.org/jsonfile/-/jsonfile-4.0.0.tgz",
-            "version": "4.0.0"
+            "resolved": "https://registry.npmjs.org/jsonfile/-/jsonfile-6.1.0.tgz",
+            "version": "6.1.0"
         },
         "karma": {
             "dependencies": {
                 "glob": {
                     "dev": true,
-                    "integrity": "sha512-OvD9ENzPLbegENnYP5UUfJIirTg4+XwMWGaQfQTY0JenxNvvIKP3U3/tAQSPIu/lHxXYSZmpXlUHeqAIdKzBLQ==",
+                    "integrity": "sha512-lmLf6gtyrPq8tTjSmrO94wBeQbFR3HbLHbuyD69wuyQkImp2hWqMGB47OX65FBkPffO641IP9jWa1z4ivqG26Q==",
                     "requires": {
                         "fs.realpath": "^1.0.0",
                         "inflight": "^1.0.4",
                         "inherits": "2",
                         "minimatch": "^3.0.4",
                         "once": "^1.3.0",
                         "path-is-absolute": "^1.0.0"
                     },
-                    "resolved": "https://registry.npmjs.org/glob/-/glob-7.1.7.tgz",
-                    "version": "7.1.7"
+                    "resolved": "https://registry.npmjs.org/glob/-/glob-7.2.0.tgz",
+                    "version": "7.2.0"
                 },
                 "graceful-fs": {
                     "dev": true,
-                    "integrity": "sha512-nTnJ528pbqxYanhpDYsi4Rd8MAeaBA67+RZ10CM1m3bTAVFEDcd5AuA4a6W5YkGZ1iNXHzZz8T6TBKLeBuNriQ==",
-                    "resolved": "https://registry.npmjs.org/graceful-fs/-/graceful-fs-4.2.6.tgz",
-                    "version": "4.2.6"
+                    "integrity": "sha512-NtNxqUcXgpW2iMrfqSfR73Glt39K+BLwWsPs94yR63v45T0Wbej7eRmL5cWfwEgqXnmjQp3zaJTshdRW/qC2ZQ==",
+                    "resolved": "https://registry.npmjs.org/graceful-fs/-/graceful-fs-4.2.9.tgz",
+                    "version": "4.2.9"
                 },
                 "mime": {
                     "dev": true,
-                    "integrity": "sha512-tqkh47FzKeCPD2PUiPB6pkbMzsCasjxAfC62/Wap5qrUWcb+sFasXUC5I3gYM5iBM8v/Qpn4UK0x+j0iHyFPDg==",
-                    "resolved": "https://registry.npmjs.org/mime/-/mime-2.5.2.tgz",
-                    "version": "2.5.2"
-                },
-                "source-map": {
-                    "dev": true,
-                    "integrity": "sha512-UjgapumWlbMhkBgzT7Ykc5YXUT46F0iKu8SGXq0bcwP5dz/h0Plj6enJqjz1Zbq2l5WaqYnrVbwWOWMyF3F47g==",
-                    "resolved": "https://registry.npmjs.org/source-map/-/source-map-0.6.1.tgz",
-                    "version": "0.6.1"
+                    "integrity": "sha512-USPkMeET31rOMiarsBNIHZKLGgvKc/LrjofAnBlOttf5ajRvqiRA8QsenbcooctK6d6Ts6aqZXBA+XbkKthiQg==",
+                    "resolved": "https://registry.npmjs.org/mime/-/mime-2.6.0.tgz",
+                    "version": "2.6.0"
                 }
             },
             "dev": true,
-            "integrity": "sha512-hbhRogUYIulfkBTZT7xoPrCYhRBnBoqbbL4fszWD0ReFGUxU+LYBr3dwKdAluaDQ/ynT9/7C+Lf7pPNW4gSx4Q==",
+            "integrity": "sha512-nEU50jLvDe5yvXqkEJRf8IuvddUkOY2x5Xc4WXHz6dxINgGDrgD2uqQWeVrJs4hbfNaotn+HQ1LZJ4yOXrL7xQ==",
             "requires": {
                 "body-parser": "^1.19.0",
                 "braces": "^3.0.2",
                 "chokidar": "^3.5.1",
-                "colors": "^1.4.0",
+                "colors": "1.4.0",
                 "connect": "^3.7.0",
                 "di": "^0.0.1",
                 "dom-serialize": "^2.2.1",
                 "glob": "^7.1.7",
                 "graceful-fs": "^4.2.6",
                 "http-proxy": "^1.18.1",
                 "isbinaryfile": "^4.0.8",
                 "lodash": "^4.17.21",
-                "log4js": "^6.3.0",
+                "log4js": "^6.4.1",
                 "mime": "^2.5.2",
                 "minimatch": "^3.0.4",
+                "mkdirp": "^0.5.5",
                 "qjobs": "^1.2.0",
                 "range-parser": "^1.2.1",
                 "rimraf": "^3.0.2",
-                "socket.io": "^3.1.0",
+                "socket.io": "^4.2.0",
                 "source-map": "^0.6.1",
                 "tmp": "^0.2.1",
-                "ua-parser-js": "^0.7.28",
+                "ua-parser-js": "^0.7.30",
                 "yargs": "^16.1.1"
             },
-            "resolved": "https://registry.npmjs.org/karma/-/karma-6.3.4.tgz",
-            "version": "6.3.4"
+            "resolved": "https://registry.npmjs.org/karma/-/karma-6.3.16.tgz",
+            "version": "6.3.16"
         },
         "karma-firefox-launcher": {
             "dev": true,
             "integrity": "sha512-Fi7xPhwrRgr+94BnHX0F5dCl1miIW4RHnzjIGxF8GaIEp7rNqX7LSi7ok63VXs3PS/5MQaQMhGxw+bvD+pibBQ==",
             "requires": {
                 "is-wsl": "^2.1.0"
             },
@@ -1823,17 +1877,26 @@
                 "webpack-merge": "^4.1.5"
             },
             "resolved": "https://registry.npmjs.org/karma-webpack/-/karma-webpack-5.0.0.tgz",
             "version": "5.0.0"
         },
         "loader-runner": {
             "dev": true,
-            "integrity": "sha512-92+huvxMvYlMzMt0iIOukcwYBFpkYJdpl2xsZ7LrlayO7E8SOv+JJUEK17B/dJIHAOLMfh2dZZ/Y18WgmGtYNw==",
-            "resolved": "https://registry.npmjs.org/loader-runner/-/loader-runner-4.2.0.tgz",
-            "version": "4.2.0"
+            "integrity": "sha512-3R/1M+yS3j5ou80Me59j7F9IMs4PXs3VqRrm0TU3AbKPxlmpoY1TNscJV/oGJXo8qCatFGTfDbY6W6ipGOYXfg==",
+            "resolved": "https://registry.npmjs.org/loader-runner/-/loader-runner-4.3.0.tgz",
+            "version": "4.3.0"
+        },
+        "locate-path": {
+            "dev": true,
+            "integrity": "sha512-iPZK6eYjbxRu3uB4/WZ3EsEIMJFMqAoopl3R+zuq0UjcAm/MO6KCweDgPfP3elTztoKP3KtnVHxTn2NHBSDVUw==",
+            "requires": {
+                "p-locate": "^5.0.0"
+            },
+            "resolved": "https://registry.npmjs.org/locate-path/-/locate-path-6.0.0.tgz",
+            "version": "6.0.0"
         },
         "lodash": {
             "dev": true,
             "integrity": "sha512-v2kDEe57lecTulaDIuNTPy3Ry4gLGJ6Z1O3vE1krgXZNrsQ+LFTGHVxVjcXPs17LhbZVGedAJv8XZ1tvj5FvSg==",
             "resolved": "https://registry.npmjs.org/lodash/-/lodash-4.17.21.tgz",
             "version": "4.17.21"
         },
@@ -1846,39 +1909,39 @@
             "resolved": "https://registry.npmjs.org/log-symbols/-/log-symbols-2.2.0.tgz",
             "version": "2.2.0"
         },
         "log4js": {
             "dependencies": {
                 "debug": {
                     "dev": true,
-                    "integrity": "sha512-mOp8wKcvj7XxC78zLgw/ZA+6TSgkoE2C/ienthhRD298T7UNwAg9diBpLRxC0mOezLl4B0xV7M0cCO6P/O0Xhw==",
+                    "integrity": "sha512-/zxw5+vh1Tfv+4Qn7a5nsbcJKPaSvCDhojn6FEl9vupwK2VCSDtEiEtqr8DFtzYFOdz63LBkxec7DYuc2jon6Q==",
                     "requires": {
                         "ms": "2.1.2"
                     },
-                    "resolved": "https://registry.npmjs.org/debug/-/debug-4.3.2.tgz",
-                    "version": "4.3.2"
+                    "resolved": "https://registry.npmjs.org/debug/-/debug-4.3.3.tgz",
+                    "version": "4.3.3"
                 },
                 "ms": {
                     "dev": true,
                     "integrity": "sha512-sGkPx+VjMtmA6MX27oA4FBFELFCZZ4S4XqeGOXCv68tT+jb3vk/RyaKWP0PTKyWtmLSM0b+adUTEvbs1PEaH2w==",
                     "resolved": "https://registry.npmjs.org/ms/-/ms-2.1.2.tgz",
                     "version": "2.1.2"
                 }
             },
             "dev": true,
-            "integrity": "sha512-Mc8jNuSFImQUIateBFwdOQcmC6Q5maU0VVvdC2R6XMb66/VnT+7WS4D/0EeNMZu1YODmJe5NIn2XftCzEocUgw==",
+            "integrity": "sha512-iUiYnXqAmNKiIZ1XSAitQ4TmNs8CdZYTAWINARF3LjnsLN8tY5m0vRwd6uuWj/yNY0YHxeZodnbmxKFUOM2rMg==",
             "requires": {
-                "date-format": "^3.0.0",
-                "debug": "^4.1.1",
-                "flatted": "^2.0.1",
-                "rfdc": "^1.1.4",
-                "streamroller": "^2.2.4"
+                "date-format": "^4.0.3",
+                "debug": "^4.3.3",
+                "flatted": "^3.2.4",
+                "rfdc": "^1.3.0",
+                "streamroller": "^3.0.2"
             },
-            "resolved": "https://registry.npmjs.org/log4js/-/log4js-6.3.0.tgz",
-            "version": "6.3.0"
+            "resolved": "https://registry.npmjs.org/log4js/-/log4js-6.4.1.tgz",
+            "version": "6.4.1"
         },
         "md5.js": {
             "dev": true,
             "integrity": "sha512-xitP+WxNPcTTOgnTJcrhM0xvdPepipPSf3I8EIpGKeFLjt3PlJLIDG3u8EX53ZIubkb+5U2+3rELYpEhHhzdkg==",
             "requires": {
                 "hash-base": "^3.0.0",
                 "inherits": "^2.0.1",
@@ -1948,26 +2011,35 @@
             "dev": true,
             "integrity": "sha1-9sAMHAsIIkblxNmd+4x8CDsrWCo=",
             "resolved": "https://registry.npmjs.org/minimalistic-crypto-utils/-/minimalistic-crypto-utils-1.0.1.tgz",
             "version": "1.0.1"
         },
         "minimatch": {
             "dev": true,
-            "integrity": "sha512-yJHVQEhyqPLUTgt9B83PXu6W3rx4MvvHvSUvToogpwoGDOUQ+yDrR0HRot+yOCdCO7u4hX3pWft6kWBBcqh0UA==",
+            "integrity": "sha512-J7p63hRiAjw1NDEww1W7i37+ByIrOWO5XQQAzZ3VOcL0PNybwpfmV/N05zFAzwQ9USyEcX6t3UO+K5aqBQOIHw==",
             "requires": {
                 "brace-expansion": "^1.1.7"
             },
-            "resolved": "https://registry.npmjs.org/minimatch/-/minimatch-3.0.4.tgz",
-            "version": "3.0.4"
+            "resolved": "https://registry.npmjs.org/minimatch/-/minimatch-3.1.2.tgz",
+            "version": "3.1.2"
         },
         "minimist": {
             "dev": true,
-            "integrity": "sha512-FM9nNUYrRBAELZQT3xeZQ7fmMOBg6nWNmJKTcgsJeaLstP/UODVpGsr5OhXhhXg6f+qtJ8uiZ+PUxkDWcgIXLw==",
-            "resolved": "https://registry.npmjs.org/minimist/-/minimist-1.2.5.tgz",
-            "version": "1.2.5"
+            "integrity": "sha512-Jsjnk4bw3YJqYzbdyBiNsPWHPfO++UGG749Cxs6peCu5Xg4nrena6OVxOYxrQTqww0Jmwt+Ref8rggumkTLz9Q==",
+            "resolved": "https://registry.npmjs.org/minimist/-/minimist-1.2.6.tgz",
+            "version": "1.2.6"
+        },
+        "mkdirp": {
+            "dev": true,
+            "integrity": "sha512-NKmAlESf6jMGym1++R0Ra7wvhV+wFW63FaSOFPwRahvea0gMUcGUhVeAg/0BC0wiv9ih5NYPB1Wn1UEI1/L+xQ==",
+            "requires": {
+                "minimist": "^1.2.5"
+            },
+            "resolved": "https://registry.npmjs.org/mkdirp/-/mkdirp-0.5.5.tgz",
+            "version": "0.5.5"
         },
         "mocha": {
             "dependencies": {
                 "ansi-styles": {
                     "dev": true,
                     "integrity": "sha512-zbB9rCJAT1rbjiVDb2hqKFHNYLxgtk8NURxZ3IZwD3F6NtxbXZQCnnSi1Lkx+IDohdPlFp222wVALIheZJQSEg==",
                     "requires": {
@@ -1985,37 +2057,21 @@
                                 "has-flag": "^4.0.0"
                             },
                             "resolved": "https://registry.npmjs.org/supports-color/-/supports-color-7.2.0.tgz",
                             "version": "7.2.0"
                         }
                     },
                     "dev": true,
-                    "integrity": "sha512-diHzdDKxcU+bAsUboHLPEDQiw0qEe0qd7SYUn3HgcFlWgbDcfLGswOHYeGrHKzG9z6UYf01d9VFMfZxPM1xZSg==",
+                    "integrity": "sha512-oKnbhFyRIXpUuez8iBMmyEa4nbj4IOQyuhc/wy9kY7/WVPcwIO9VA668Pu8RkO7+0G76SLROeyw9CpQ061i4mA==",
                     "requires": {
                         "ansi-styles": "^4.1.0",
                         "supports-color": "^7.1.0"
                     },
-                    "resolved": "https://registry.npmjs.org/chalk/-/chalk-4.1.1.tgz",
-                    "version": "4.1.1"
-                },
-                "chokidar": {
-                    "dev": true,
-                    "integrity": "sha512-9+s+Od+W0VJJzawDma/gvBNQqkTiqYTWLuZoyAsivsI4AaWTCzHG06/TMjsf1cYe9Cb97UCEhjz7HvnPk2p/tw==",
-                    "requires": {
-                        "anymatch": "~3.1.1",
-                        "braces": "~3.0.2",
-                        "fsevents": "~2.3.1",
-                        "glob-parent": "~5.1.0",
-                        "is-binary-path": "~2.1.0",
-                        "is-glob": "~4.0.1",
-                        "normalize-path": "~3.0.0",
-                        "readdirp": "~3.5.0"
-                    },
-                    "resolved": "https://registry.npmjs.org/chokidar/-/chokidar-3.5.1.tgz",
-                    "version": "3.5.1"
+                    "resolved": "https://registry.npmjs.org/chalk/-/chalk-4.1.2.tgz",
+                    "version": "4.1.2"
                 },
                 "color-convert": {
                     "dev": true,
                     "integrity": "sha512-RRECPsj7iu/xb5oKYcsFHSppFNnsj/52OVTRKb4zP5onXwVF3zVmmToNcOfGC+CRDpfK/U584fMg38ZHCaElKQ==",
                     "requires": {
                         "color-name": "~1.1.4"
                     },
@@ -2034,171 +2090,161 @@
                             "dev": true,
                             "integrity": "sha512-sGkPx+VjMtmA6MX27oA4FBFELFCZZ4S4XqeGOXCv68tT+jb3vk/RyaKWP0PTKyWtmLSM0b+adUTEvbs1PEaH2w==",
                             "resolved": "https://registry.npmjs.org/ms/-/ms-2.1.2.tgz",
                             "version": "2.1.2"
                         }
                     },
                     "dev": true,
-                    "integrity": "sha512-doEwdvm4PCeK4K3RQN2ZC2BYUBaxwLARCqZmMjtF8a51J2Rb0xpVloFRnCODwqjpwnAoao4pelN8l3RJdv3gRQ==",
+                    "integrity": "sha512-PRWFHuSU3eDtQJPvnNY7Jcket1j0t5OuOsFzPPzsekD52Zl8qUfFIPEiswXqIvHWGVHOgX+7G/vCNNhehwxfkQ==",
                     "requires": {
                         "ms": "2.1.2"
                     },
-                    "resolved": "https://registry.npmjs.org/debug/-/debug-4.3.1.tgz",
-                    "version": "4.3.1"
+                    "resolved": "https://registry.npmjs.org/debug/-/debug-4.3.4.tgz",
+                    "version": "4.3.4"
                 },
                 "escape-string-regexp": {
                     "dev": true,
                     "integrity": "sha512-TtpcNJ3XAzx3Gq8sWRzJaVajRs0uVxA2YAkdb1jm2YkPz4G6egUFAyA3n5vtEIZefPk5Wa4UXbKuS5fKkJWdgA==",
                     "resolved": "https://registry.npmjs.org/escape-string-regexp/-/escape-string-regexp-4.0.0.tgz",
                     "version": "4.0.0"
                 },
-                "find-up": {
+                "glob": {
+                    "dependencies": {
+                        "minimatch": {
+                            "dev": true,
+                            "integrity": "sha512-J7p63hRiAjw1NDEww1W7i37+ByIrOWO5XQQAzZ3VOcL0PNybwpfmV/N05zFAzwQ9USyEcX6t3UO+K5aqBQOIHw==",
+                            "requires": {
+                                "brace-expansion": "^1.1.7"
+                            },
+                            "resolved": "https://registry.npmjs.org/minimatch/-/minimatch-3.1.2.tgz",
+                            "version": "3.1.2"
+                        }
+                    },
                     "dev": true,
-                    "integrity": "sha512-78/PXT1wlLLDgTzDs7sjq9hzz0vXD+zn+7wypEe4fXQxCmdmqfGsEPQxmiCSQI3ajFV91bVSsvNtrJRiW6nGng==",
+                    "integrity": "sha512-lmLf6gtyrPq8tTjSmrO94wBeQbFR3HbLHbuyD69wuyQkImp2hWqMGB47OX65FBkPffO641IP9jWa1z4ivqG26Q==",
                     "requires": {
-                        "locate-path": "^6.0.0",
-                        "path-exists": "^4.0.0"
+                        "fs.realpath": "^1.0.0",
+                        "inflight": "^1.0.4",
+                        "inherits": "2",
+                        "minimatch": "^3.0.4",
+                        "once": "^1.3.0",
+                        "path-is-absolute": "^1.0.0"
                     },
-                    "resolved": "https://registry.npmjs.org/find-up/-/find-up-5.0.0.tgz",
-                    "version": "5.0.0"
+                    "resolved": "https://registry.npmjs.org/glob/-/glob-7.2.0.tgz",
+                    "version": "7.2.0"
                 },
                 "has-flag": {
                     "dev": true,
                     "integrity": "sha512-EykJT/Q1KjTWctppgIAgfSO0tKVuZUjhgMr17kqTumMl6Afv3EISleU7qZUzoXDFTAHTDC4NOoG/ZxU3EvlMPQ==",
                     "resolved": "https://registry.npmjs.org/has-flag/-/has-flag-4.0.0.tgz",
                     "version": "4.0.0"
                 },
-                "locate-path": {
+                "log-symbols": {
                     "dev": true,
-                    "integrity": "sha512-iPZK6eYjbxRu3uB4/WZ3EsEIMJFMqAoopl3R+zuq0UjcAm/MO6KCweDgPfP3elTztoKP3KtnVHxTn2NHBSDVUw==",
+                    "integrity": "sha512-8XPvpAA8uyhfteu8pIvQxpJZ7SYYdpUivZpGy6sFsBuKRY/7rQGavedeB8aK+Zkyq6upMFVL/9AW6vOYzfRyLg==",
                     "requires": {
-                        "p-locate": "^5.0.0"
+                        "chalk": "^4.1.0",
+                        "is-unicode-supported": "^0.1.0"
                     },
-                    "resolved": "https://registry.npmjs.org/locate-path/-/locate-path-6.0.0.tgz",
-                    "version": "6.0.0"
+                    "resolved": "https://registry.npmjs.org/log-symbols/-/log-symbols-4.1.0.tgz",
+                    "version": "4.1.0"
                 },
-                "log-symbols": {
+                "minimatch": {
+                    "dependencies": {
+                        "brace-expansion": {
+                            "dev": true,
+                            "integrity": "sha512-XnAIvQ8eM+kC6aULx6wuQiwVsnzsi9d3WxzV3FpWTGA19F621kwdbsAcFKXgKUHZWsy+mY6iL1sHTxWEFCytDA==",
+                            "requires": {
+                                "balanced-match": "^1.0.0"
+                            },
+                            "resolved": "https://registry.npmjs.org/brace-expansion/-/brace-expansion-2.0.1.tgz",
+                            "version": "2.0.1"
+                        }
+                    },
                     "dev": true,
-                    "integrity": "sha512-FN8JBzLx6CzeMrB0tg6pqlGU1wCrXW+ZXGH481kfsBqer0hToTIiHdjH4Mq8xJUbvATujKCvaREGWpGUionraA==",
+                    "integrity": "sha512-nLDxIFRyhDblz3qMuq+SoRZED4+miJ/G+tdDrjkkkRnjAsBexeGpgjLEQ0blJy7rHhR2b93rhQY4SvyWu9v03g==",
                     "requires": {
-                        "chalk": "^4.0.0"
+                        "brace-expansion": "^2.0.1"
                     },
-                    "resolved": "https://registry.npmjs.org/log-symbols/-/log-symbols-4.0.0.tgz",
-                    "version": "4.0.0"
+                    "resolved": "https://registry.npmjs.org/minimatch/-/minimatch-5.0.1.tgz",
+                    "version": "5.0.1"
                 },
                 "ms": {
                     "dev": true,
                     "integrity": "sha512-6FlzubTLZG3J2a/NVCAleEhjzq5oxgHyaCU9yYXvcLsvoVaHJq/s5xXI6/XXP6tz7R9xAOtHnSO/tXtF3WRTlA==",
                     "resolved": "https://registry.npmjs.org/ms/-/ms-2.1.3.tgz",
                     "version": "2.1.3"
                 },
-                "p-limit": {
-                    "dev": true,
-                    "integrity": "sha512-TYOanM3wGwNGsZN2cVTYPArw454xnXj5qmWF1bEoAc4+cU/ol7GVh7odevjp1FNHduHc3KZMcFduxU5Xc6uJRQ==",
-                    "requires": {
-                        "yocto-queue": "^0.1.0"
-                    },
-                    "resolved": "https://registry.npmjs.org/p-limit/-/p-limit-3.1.0.tgz",
-                    "version": "3.1.0"
-                },
-                "p-locate": {
-                    "dev": true,
-                    "integrity": "sha512-LaNjtRWUBY++zB5nE/NwcaoMylSPk+S+ZHNB1TzdbMJMny6dynpAGt7X/tl/QYq3TIeE6nxHppbo2LGymrG5Pw==",
-                    "requires": {
-                        "p-limit": "^3.0.2"
-                    },
-                    "resolved": "https://registry.npmjs.org/p-locate/-/p-locate-5.0.0.tgz",
-                    "version": "5.0.0"
-                },
-                "path-exists": {
-                    "dev": true,
-                    "integrity": "sha512-ak9Qy5Q7jYb2Wwcey5Fpvg2KoAc/ZIhLSLOSBmRmygPsGwkVVt0fZa0qrtMz+m6tJTAHfZQ8FnmB4MG4LWy7/w==",
-                    "resolved": "https://registry.npmjs.org/path-exists/-/path-exists-4.0.0.tgz",
-                    "version": "4.0.0"
-                },
-                "readdirp": {
-                    "dev": true,
-                    "integrity": "sha512-cMhu7c/8rdhkHXWsY+osBhfSy0JikwpHK/5+imo+LpeasTF8ouErHrlYkwT0++njiyuDvc7OFY5T3ukvZ8qmFQ==",
-                    "requires": {
-                        "picomatch": "^2.2.1"
-                    },
-                    "resolved": "https://registry.npmjs.org/readdirp/-/readdirp-3.5.0.tgz",
-                    "version": "3.5.0"
-                },
                 "serialize-javascript": {
                     "dev": true,
-                    "integrity": "sha512-SaaNal9imEO737H2c05Og0/8LUXG7EnsZyMa8MzkmuHoELfT6txuj0cMqRj6zfPKnmQ1yasR4PCJc8x+M4JSPA==",
+                    "integrity": "sha512-Qr3TosvguFt8ePWqsvRfrKyQXIiW+nGbYpy8XK24NQHE83caxWt+mIymTT19DGFbNWNLfEwsrkSmN64lVWB9ag==",
                     "requires": {
                         "randombytes": "^2.1.0"
                     },
-                    "resolved": "https://registry.npmjs.org/serialize-javascript/-/serialize-javascript-5.0.1.tgz",
-                    "version": "5.0.1"
+                    "resolved": "https://registry.npmjs.org/serialize-javascript/-/serialize-javascript-6.0.0.tgz",
+                    "version": "6.0.0"
                 }
             },
             "dev": true,
-            "integrity": "sha512-hJaO0mwDXmZS4ghXsvPVriOhsxQ7ofcpQdm8dE+jISUOKopitvnXFQmpRR7jd2K6VBG6E26gU3IAbXXGIbu4sQ==",
+            "integrity": "sha512-IDY7fl/BecMwFHzoqF2sg/SHHANeBoMMXFlS9r0OXKDssYE1M5O43wUY/9BVPeIvfH2zmEbBfseqN9gBQZzXkg==",
             "requires": {
-                "@ungap/promise-all-settled": "1.1.2",
                 "ansi-colors": "4.1.1",
                 "browser-stdout": "1.3.1",
-                "chokidar": "3.5.1",
-                "debug": "4.3.1",
+                "chokidar": "3.5.3",
+                "debug": "4.3.4",
                 "diff": "5.0.0",
                 "escape-string-regexp": "4.0.0",
                 "find-up": "5.0.0",
-                "glob": "7.1.6",
-                "growl": "1.10.5",
+                "glob": "7.2.0",
                 "he": "1.2.0",
-                "js-yaml": "4.0.0",
-                "log-symbols": "4.0.0",
-                "minimatch": "3.0.4",
+                "js-yaml": "4.1.0",
+                "log-symbols": "4.1.0",
+                "minimatch": "5.0.1",
                 "ms": "2.1.3",
-                "nanoid": "3.1.20",
-                "serialize-javascript": "5.0.1",
+                "nanoid": "3.3.3",
+                "serialize-javascript": "6.0.0",
                 "strip-json-comments": "3.1.1",
                 "supports-color": "8.1.1",
-                "which": "2.0.2",
-                "wide-align": "1.1.3",
-                "workerpool": "6.1.0",
+                "workerpool": "6.2.1",
                 "yargs": "16.2.0",
                 "yargs-parser": "20.2.4",
                 "yargs-unparser": "2.0.0"
             },
-            "resolved": "https://registry.npmjs.org/mocha/-/mocha-8.4.0.tgz",
-            "version": "8.4.0"
+            "resolved": "https://registry.npmjs.org/mocha/-/mocha-10.2.0.tgz",
+            "version": "10.2.0"
         },
         "ms": {
             "dev": true,
             "integrity": "sha1-VgiurfwAvmwpAd9fmGF4jeDVl8g=",
             "resolved": "https://registry.npmjs.org/ms/-/ms-2.0.0.tgz",
             "version": "2.0.0"
         },
         "nanoid": {
             "dev": true,
-            "integrity": "sha512-a1cQNyczgKbLX9jwbS/+d7W8fX/RfgYR7lVWwWOGIPNgK2m0MWvrGF6/m4kk6U3QcFMnZf3RIhL0v2Jgh/0Uxw==",
-            "resolved": "https://registry.npmjs.org/nanoid/-/nanoid-3.1.20.tgz",
-            "version": "3.1.20"
+            "integrity": "sha512-p1sjXuopFs0xg+fPASzQ28agW1oHD7xDsd9Xkf3T15H3c/cifrFHVwrh74PdoklAPi+i7MdRsE47vm2r6JoB+w==",
+            "resolved": "https://registry.npmjs.org/nanoid/-/nanoid-3.3.3.tgz",
+            "version": "3.3.3"
         },
         "negotiator": {
             "dev": true,
-            "integrity": "sha512-hZXc7K2e+PgeI1eDBe/10Ard4ekbfrrqG8Ep+8Jmf4JID2bNg7NvCPOZN+kfF574pFQI7mum2AUqDidoKqcTOw==",
-            "resolved": "https://registry.npmjs.org/negotiator/-/negotiator-0.6.2.tgz",
-            "version": "0.6.2"
+            "integrity": "sha512-+EUsqGPLsM+j/zdChZjsnX51g4XrHFOIXwfnCVPGlQk/k5giakcKsuxCObBRu6DSm9opw/O6slWbJdghQM4bBg==",
+            "resolved": "https://registry.npmjs.org/negotiator/-/negotiator-0.6.3.tgz",
+            "version": "0.6.3"
         },
         "neo-async": {
             "dev": true,
             "integrity": "sha512-Yd3UES5mWCSqR+qNT93S3UoYUkqAZ9lLg8a7g9rimsWmYGK8cVToA4/sF3RrshdyV3sAGMXVUmpMYOw+dLpOuw==",
             "resolved": "https://registry.npmjs.org/neo-async/-/neo-async-2.6.2.tgz",
             "version": "2.6.2"
         },
         "node-releases": {
             "dev": true,
-            "integrity": "sha512-uW7fodD6pyW2FZNZnp/Z3hvWKeEW1Y8R1+1CnErE8cXFXzl5blBOoVB41CvMer6P6Q0S5FXDwcHgFd1Wj0U9zg==",
-            "resolved": "https://registry.npmjs.org/node-releases/-/node-releases-1.1.73.tgz",
-            "version": "1.1.73"
+            "integrity": "sha512-5GFldHPXVG/YZmFzJvKK2zDSzPKhEp0+ZR5SVaoSag9fsL5YgHbUHDfnG5494ISANDcK4KwPXAx2xqVEydmd7w==",
+            "resolved": "https://registry.npmjs.org/node-releases/-/node-releases-2.0.10.tgz",
+            "version": "2.0.10"
         },
         "normalize-path": {
             "dev": true,
             "integrity": "sha512-6eZs5Ls3WtCisHWp9S2GUy8dqkpGi4BVSz3GaqiE6ezub0512ESztXUwUB6C6IKbQkY2Pnb/mD4WYojCRwcwLA==",
             "resolved": "https://registry.npmjs.org/normalize-path/-/normalize-path-3.0.0.tgz",
             "version": "3.0.0"
         },
@@ -2253,14 +2299,23 @@
             "integrity": "sha512-TYOanM3wGwNGsZN2cVTYPArw454xnXj5qmWF1bEoAc4+cU/ol7GVh7odevjp1FNHduHc3KZMcFduxU5Xc6uJRQ==",
             "requires": {
                 "yocto-queue": "^0.1.0"
             },
             "resolved": "https://registry.npmjs.org/p-limit/-/p-limit-3.1.0.tgz",
             "version": "3.1.0"
         },
+        "p-locate": {
+            "dev": true,
+            "integrity": "sha512-LaNjtRWUBY++zB5nE/NwcaoMylSPk+S+ZHNB1TzdbMJMny6dynpAGt7X/tl/QYq3TIeE6nxHppbo2LGymrG5Pw==",
+            "requires": {
+                "p-limit": "^3.0.2"
+            },
+            "resolved": "https://registry.npmjs.org/p-locate/-/p-locate-5.0.0.tgz",
+            "version": "5.0.0"
+        },
         "parse-asn1": {
             "dev": true,
             "integrity": "sha512-RnZRo1EPU6JBnra2vGHj0yhp6ebyjBZpmUCLHWiFhxlzvBCCpAuZ7elsBp1PVAbQN0/04VD/19rfzlBSwLstMw==",
             "requires": {
                 "asn1.js": "^5.2.0",
                 "browserify-aes": "^1.0.0",
                 "evp_bytestokey": "^1.0.0",
@@ -2278,14 +2333,20 @@
         },
         "path-browserify": {
             "dev": true,
             "integrity": "sha512-b7uo2UCUOYZcnF/3ID0lulOJi/bafxa1xPe7ZPsammBSpjSWQkjNxlt635YGS2MiR9GjvuXCtz2emr3jbsz98g==",
             "resolved": "https://registry.npmjs.org/path-browserify/-/path-browserify-1.0.1.tgz",
             "version": "1.0.1"
         },
+        "path-exists": {
+            "dev": true,
+            "integrity": "sha512-ak9Qy5Q7jYb2Wwcey5Fpvg2KoAc/ZIhLSLOSBmRmygPsGwkVVt0fZa0qrtMz+m6tJTAHfZQ8FnmB4MG4LWy7/w==",
+            "resolved": "https://registry.npmjs.org/path-exists/-/path-exists-4.0.0.tgz",
+            "version": "4.0.0"
+        },
         "path-is-absolute": {
             "dev": true,
             "integrity": "sha1-F0uSaHNVNP+8es5r9TpanhtcX18=",
             "resolved": "https://registry.npmjs.org/path-is-absolute/-/path-is-absolute-1.0.1.tgz",
             "version": "1.0.1"
         },
         "pbkdf2": {
@@ -2297,14 +2358,20 @@
                 "ripemd160": "^2.0.1",
                 "safe-buffer": "^5.0.1",
                 "sha.js": "^2.4.8"
             },
             "resolved": "https://registry.npmjs.org/pbkdf2/-/pbkdf2-3.1.2.tgz",
             "version": "3.1.2"
         },
+        "picocolors": {
+            "dev": true,
+            "integrity": "sha512-1fygroTLlHu66zi26VoTDv8yRgm0Fccecssto+MhsZ0D/DGW2sm8E8AjW7NU5VVTRt5GxbeZ5qBuJr+HyLYkjQ==",
+            "resolved": "https://registry.npmjs.org/picocolors/-/picocolors-1.0.0.tgz",
+            "version": "1.0.0"
+        },
         "picomatch": {
             "dev": true,
             "integrity": "sha512-q0M/9eZHzmr0AulXyPwNfZjtwZ/RBZlbN3K3CErVrk50T2ASYI7Bye0EvekFY3IP1Nt2DHu0re+V2ZHIpMkuWg==",
             "resolved": "https://registry.npmjs.org/picomatch/-/picomatch-2.2.2.tgz",
             "version": "2.2.2"
         },
         "process": {
@@ -2333,29 +2400,29 @@
                 "safe-buffer": "^5.1.2"
             },
             "resolved": "https://registry.npmjs.org/public-encrypt/-/public-encrypt-4.0.3.tgz",
             "version": "4.0.3"
         },
         "punycode": {
             "dev": true,
-            "integrity": "sha512-XRsRjdf+j5ml+y/6GKHPZbrF/8p2Yga0JPtdqTIY2Xe5ohJPD9saDJJLPvp9+NSBprVvevdXZybnj2cv8OEd0A==",
-            "resolved": "https://registry.npmjs.org/punycode/-/punycode-2.1.1.tgz",
-            "version": "2.1.1"
+            "integrity": "sha512-rRV+zQD8tVFys26lAGR9WUuS4iUAngJScM+ZRSKtvl5tKeZ2t5bvdNFdNHBW9FWR4guGHlgmsZ1G7BSm2wTbuA==",
+            "resolved": "https://registry.npmjs.org/punycode/-/punycode-2.3.0.tgz",
+            "version": "2.3.0"
         },
         "qjobs": {
             "dev": true,
             "integrity": "sha512-8YOJEHtxpySA3fFDyCRxA+UUV+fA+rTWnuWvylOK/NCjhY+b4ocCtmu8TtsWb+mYeU+GCHf/S66KZF/AsteKHg==",
             "resolved": "https://registry.npmjs.org/qjobs/-/qjobs-1.2.0.tgz",
             "version": "1.2.0"
         },
         "qs": {
             "dev": true,
-            "integrity": "sha512-VCdBRNFTX1fyE7Nb6FYoURo/SPe62QCaAyzJvUjwRaIsc+NePBEniHlvxFmmX56+HZphIGtV0XeCirBtpDrTyQ==",
-            "resolved": "https://registry.npmjs.org/qs/-/qs-6.7.0.tgz",
-            "version": "6.7.0"
+            "integrity": "sha512-IhMFgUmuNpyRfxA90umL7ByLlgRXu6tIfKPpF5TmcfRLlLCckfP/g3IQmju6jjpu+Hh8rA+2p6A27ZSPOOHdKw==",
+            "resolved": "https://registry.npmjs.org/qs/-/qs-6.9.7.tgz",
+            "version": "6.9.7"
         },
         "randombytes": {
             "dev": true,
             "integrity": "sha512-vYl3iOX+4CKUWuxGi9Ukhie6fsqXqS9FE2Zaic4tNFD2N2QQaXOMFbuKK4QmDHC0JO6B1Zp41J0LpT0oR68amQ==",
             "requires": {
                 "safe-buffer": "^5.1.0"
             },
@@ -2376,23 +2443,23 @@
             "dev": true,
             "integrity": "sha512-Hrgsx+orqoygnmhFbKaHE6c296J+HTAQXoxEF6gNupROmmGJRoyzfG3ccAveqCBrwr/2yxQ5BVd/GTl5agOwSg==",
             "resolved": "https://registry.npmjs.org/range-parser/-/range-parser-1.2.1.tgz",
             "version": "1.2.1"
         },
         "raw-body": {
             "dev": true,
-            "integrity": "sha512-4Oz8DUIwdvoa5qMJelxipzi/iJIi40O5cGV1wNYp5hvZP8ZN0T+jiNkL0QepXs+EsQ9XJ8ipEDoiH70ySUJP3Q==",
+            "integrity": "sha512-UlTNLIcu0uzb4D2f4WltY6cVjLi+/jEN4lgEUj3E04tpMDpUlkBo/eSn6zou9hum2VMNpCCUone0O0WeJim07g==",
             "requires": {
-                "bytes": "3.1.0",
-                "http-errors": "1.7.2",
+                "bytes": "3.1.2",
+                "http-errors": "1.8.1",
                 "iconv-lite": "0.4.24",
                 "unpipe": "1.0.0"
             },
-            "resolved": "https://registry.npmjs.org/raw-body/-/raw-body-2.4.0.tgz",
-            "version": "2.4.0"
+            "resolved": "https://registry.npmjs.org/raw-body/-/raw-body-2.4.3.tgz",
+            "version": "2.4.3"
         },
         "readable-stream": {
             "dev": true,
             "integrity": "sha512-BViHy7LKeTz4oNnkcLJ+lVSL6vpiFeX6/d3oSH8zCW7UxP2onchk+vTGB143xuFjHS3deTgkKoXXymXqymiIdA==",
             "requires": {
                 "inherits": "^2.0.3",
                 "string_decoder": "^1.1.1",
@@ -2463,37 +2530,37 @@
             "dev": true,
             "integrity": "sha512-YZo3K82SD7Riyi0E1EQPojLz7kpepnSQI9IyPbHHg1XXXevb5dJI7tpyN2ADxGcQbHG7vcyRHk0cbwqcQriUtg==",
             "resolved": "https://registry.npmjs.org/safer-buffer/-/safer-buffer-2.1.2.tgz",
             "version": "2.1.2"
         },
         "schema-utils": {
             "dev": true,
-            "integrity": "sha512-6D82/xSzO094ajanoOSbe4YvXWMfn2A//8Y1+MUqFAJul5Bs+yn36xbK9OtNDcRVSBJ9jjeoXftM6CfztsjOAA==",
+            "integrity": "sha512-pvjEHOgWc9OWA/f/DE3ohBWTD6EleVLf7iFUkoSwAxttdBhB9QUebQgxER2kWueOvRJXPHNnyrvvh9eZINB8Eg==",
             "requires": {
-                "@types/json-schema": "^7.0.6",
+                "@types/json-schema": "^7.0.8",
                 "ajv": "^6.12.5",
                 "ajv-keywords": "^3.5.2"
             },
-            "resolved": "https://registry.npmjs.org/schema-utils/-/schema-utils-3.0.0.tgz",
-            "version": "3.0.0"
+            "resolved": "https://registry.npmjs.org/schema-utils/-/schema-utils-3.1.2.tgz",
+            "version": "3.1.2"
         },
         "serialize-javascript": {
             "dev": true,
-            "integrity": "sha512-SaaNal9imEO737H2c05Og0/8LUXG7EnsZyMa8MzkmuHoELfT6txuj0cMqRj6zfPKnmQ1yasR4PCJc8x+M4JSPA==",
+            "integrity": "sha512-owoXEFjWRllis8/M1Q+Cw5k8ZH40e3zhp/ovX+Xr/vi1qj6QesbyXXViFbpNvWvPNAD62SutwEXavefrLJWj7w==",
             "requires": {
                 "randombytes": "^2.1.0"
             },
-            "resolved": "https://registry.npmjs.org/serialize-javascript/-/serialize-javascript-5.0.1.tgz",
-            "version": "5.0.1"
+            "resolved": "https://registry.npmjs.org/serialize-javascript/-/serialize-javascript-6.0.1.tgz",
+            "version": "6.0.1"
         },
         "setprototypeof": {
             "dev": true,
-            "integrity": "sha512-JvdAWfbXeIGaZ9cILp38HntZSFSo3mWg6xGcJJsd+d4aRMOqauag1C63dJfDw7OaMYwEbHMOxEZ1lqVRYP2OAw==",
-            "resolved": "https://registry.npmjs.org/setprototypeof/-/setprototypeof-1.1.1.tgz",
-            "version": "1.1.1"
+            "integrity": "sha512-E5LDX7Wrp85Kil5bhZv46j8jOeboKq5JMmYM3gVGdGH8xFpPWXUMsNrlODCrkoxMEeNi/XZIwuRvY4XNwYMJpw==",
+            "resolved": "https://registry.npmjs.org/setprototypeof/-/setprototypeof-1.2.0.tgz",
+            "version": "1.2.0"
         },
         "sha.js": {
             "dev": true,
             "integrity": "sha512-QMEp5B7cftE7APOjk5Y6xgrbWu+WkLVQwk8JNjZ8nKRciZaByEW6MubieAiToS7+dwvrjGhH8jRXz3MVd0AYqQ==",
             "requires": {
                 "inherits": "^2.0.1",
                 "safe-buffer": "^5.0.1"
@@ -2501,101 +2568,98 @@
             "resolved": "https://registry.npmjs.org/sha.js/-/sha.js-2.4.11.tgz",
             "version": "2.4.11"
         },
         "socket.io": {
             "dependencies": {
                 "debug": {
                     "dev": true,
-                    "integrity": "sha512-mOp8wKcvj7XxC78zLgw/ZA+6TSgkoE2C/ienthhRD298T7UNwAg9diBpLRxC0mOezLl4B0xV7M0cCO6P/O0Xhw==",
+                    "integrity": "sha512-PRWFHuSU3eDtQJPvnNY7Jcket1j0t5OuOsFzPPzsekD52Zl8qUfFIPEiswXqIvHWGVHOgX+7G/vCNNhehwxfkQ==",
                     "requires": {
                         "ms": "2.1.2"
                     },
-                    "resolved": "https://registry.npmjs.org/debug/-/debug-4.3.2.tgz",
-                    "version": "4.3.2"
+                    "resolved": "https://registry.npmjs.org/debug/-/debug-4.3.4.tgz",
+                    "version": "4.3.4"
                 },
                 "ms": {
                     "dev": true,
                     "integrity": "sha512-sGkPx+VjMtmA6MX27oA4FBFELFCZZ4S4XqeGOXCv68tT+jb3vk/RyaKWP0PTKyWtmLSM0b+adUTEvbs1PEaH2w==",
                     "resolved": "https://registry.npmjs.org/ms/-/ms-2.1.2.tgz",
                     "version": "2.1.2"
+                },
+                "socket.io-adapter": {
+                    "dev": true,
+                    "integrity": "sha512-87C3LO/NOMc+eMcpcxUBebGjkpMDkNBS9tf7KJqcDsmL936EChtVva71Dw2q4tQcuVC+hAUy4an2NO/sYXmwRA==",
+                    "requires": {
+                        "ws": "~8.11.0"
+                    },
+                    "resolved": "https://registry.npmjs.org/socket.io-adapter/-/socket.io-adapter-2.5.2.tgz",
+                    "version": "2.5.2"
+                },
+                "ws": {
+                    "dev": true,
+                    "integrity": "sha512-HPG3wQd9sNQoT9xHyNCXoDUa+Xw/VevmY9FoHyQ+g+rrMn4j6FB4np7Z0OhdTgjx6MgQLK7jwSy1YecU1+4Asg==",
+                    "resolved": "https://registry.npmjs.org/ws/-/ws-8.11.0.tgz",
+                    "version": "8.11.0"
                 }
             },
             "dev": true,
-            "integrity": "sha512-JubKZnTQ4Z8G4IZWtaAZSiRP3I/inpy8c/Bsx2jrwGrTbKeVU5xd6qkKMHpChYeM3dWZSO0QACiGK+obhBNwYw==",
+            "integrity": "sha512-KMcaAi4l/8+xEjkRICl6ak8ySoxsYG+gG6/XfRCPJPQ/haCRIJBTL4wIl8YCsmtaBovcAXGLOShyVWQ/FG8GZA==",
             "requires": {
-                "@types/cookie": "^0.4.0",
-                "@types/cors": "^2.8.8",
-                "@types/node": ">=10.0.0",
                 "accepts": "~1.3.4",
                 "base64id": "~2.0.0",
-                "debug": "~4.3.1",
-                "engine.io": "~4.1.0",
-                "socket.io-adapter": "~2.1.0",
-                "socket.io-parser": "~4.0.3"
+                "debug": "~4.3.2",
+                "engine.io": "~6.4.1",
+                "socket.io-adapter": "~2.5.2",
+                "socket.io-parser": "~4.2.1"
             },
-            "resolved": "https://registry.npmjs.org/socket.io/-/socket.io-3.1.2.tgz",
-            "version": "3.1.2"
-        },
-        "socket.io-adapter": {
-            "dev": true,
-            "integrity": "sha512-+vDov/aTsLjViYTwS9fPy5pEtTkrbEKsw2M+oVSoFGw6OD1IpvlV1VPhUzNbofCQ8oyMbdYJqDtGdmHQK6TdPg==",
-            "resolved": "https://registry.npmjs.org/socket.io-adapter/-/socket.io-adapter-2.1.0.tgz",
-            "version": "2.1.0"
+            "resolved": "https://registry.npmjs.org/socket.io/-/socket.io-4.6.1.tgz",
+            "version": "4.6.1"
         },
         "socket.io-parser": {
             "dependencies": {
                 "debug": {
                     "dev": true,
-                    "integrity": "sha512-mOp8wKcvj7XxC78zLgw/ZA+6TSgkoE2C/ienthhRD298T7UNwAg9diBpLRxC0mOezLl4B0xV7M0cCO6P/O0Xhw==",
+                    "integrity": "sha512-PRWFHuSU3eDtQJPvnNY7Jcket1j0t5OuOsFzPPzsekD52Zl8qUfFIPEiswXqIvHWGVHOgX+7G/vCNNhehwxfkQ==",
                     "requires": {
                         "ms": "2.1.2"
                     },
-                    "resolved": "https://registry.npmjs.org/debug/-/debug-4.3.2.tgz",
-                    "version": "4.3.2"
+                    "resolved": "https://registry.npmjs.org/debug/-/debug-4.3.4.tgz",
+                    "version": "4.3.4"
                 },
                 "ms": {
                     "dev": true,
                     "integrity": "sha512-sGkPx+VjMtmA6MX27oA4FBFELFCZZ4S4XqeGOXCv68tT+jb3vk/RyaKWP0PTKyWtmLSM0b+adUTEvbs1PEaH2w==",
                     "resolved": "https://registry.npmjs.org/ms/-/ms-2.1.2.tgz",
                     "version": "2.1.2"
                 }
             },
             "dev": true,
-            "integrity": "sha512-t+b0SS+IxG7Rxzda2EVvyBZbvFPBCjJoyHuE0P//7OAsN23GItzDRdWa6ALxZI/8R5ygK7jAR6t028/z+7295g==",
+            "integrity": "sha512-JMafRntWVO2DCJimKsRTh/wnqVvO4hrfwOqtO7f+uzwsQMuxO6VwImtYxaQ+ieoyshWOTJyV0fA21lccEXRPpQ==",
             "requires": {
-                "@types/component-emitter": "^1.2.10",
-                "component-emitter": "~1.3.0",
+                "@socket.io/component-emitter": "~3.1.0",
                 "debug": "~4.3.1"
             },
-            "resolved": "https://registry.npmjs.org/socket.io-parser/-/socket.io-parser-4.0.4.tgz",
-            "version": "4.0.4"
+            "resolved": "https://registry.npmjs.org/socket.io-parser/-/socket.io-parser-4.2.3.tgz",
+            "version": "4.2.3"
         },
-        "source-list-map": {
+        "source-map": {
             "dev": true,
-            "integrity": "sha512-qnQ7gVMxGNxsiL4lEuJwe/To8UnK7fAnmbGEEH8RpLouuKbeEm0lhbQVFIrNSuB+G7tVrAlVsZgETT5nljf+Iw==",
-            "resolved": "https://registry.npmjs.org/source-list-map/-/source-list-map-2.0.1.tgz",
-            "version": "2.0.1"
+            "integrity": "sha512-UjgapumWlbMhkBgzT7Ykc5YXUT46F0iKu8SGXq0bcwP5dz/h0Plj6enJqjz1Zbq2l5WaqYnrVbwWOWMyF3F47g==",
+            "resolved": "https://registry.npmjs.org/source-map/-/source-map-0.6.1.tgz",
+            "version": "0.6.1"
         },
         "source-map-support": {
-            "dependencies": {
-                "source-map": {
-                    "dev": true,
-                    "integrity": "sha512-UjgapumWlbMhkBgzT7Ykc5YXUT46F0iKu8SGXq0bcwP5dz/h0Plj6enJqjz1Zbq2l5WaqYnrVbwWOWMyF3F47g==",
-                    "resolved": "https://registry.npmjs.org/source-map/-/source-map-0.6.1.tgz",
-                    "version": "0.6.1"
-                }
-            },
             "dev": true,
-            "integrity": "sha512-Wonm7zOCIJzBGQdB+thsPar0kYuCIzYvxZwlBa87yi/Mdjv7Tip2cyVbLj5o0cFPN4EVkuTwb3GDDyUx2DGnGw==",
+            "integrity": "sha512-uBHU3L3czsIyYXKX88fdrGovxdSCoTGDRZ6SYXtSRxLZUzHg5P/66Ht6uoUlHu9EZod+inXhKo3qQgwXUT/y1w==",
             "requires": {
                 "buffer-from": "^1.0.0",
                 "source-map": "^0.6.0"
             },
-            "resolved": "https://registry.npmjs.org/source-map-support/-/source-map-support-0.5.19.tgz",
-            "version": "0.5.19"
+            "resolved": "https://registry.npmjs.org/source-map-support/-/source-map-support-0.5.21.tgz",
+            "version": "0.5.21"
         },
         "statuses": {
             "dev": true,
             "integrity": "sha1-Fhx9rBd2Wf2YEfQ3cfqZOBR4Yow=",
             "resolved": "https://registry.npmjs.org/statuses/-/statuses-1.5.0.tgz",
             "version": "1.5.0"
         },
@@ -2615,55 +2679,39 @@
                 "readable-stream": "^3.5.0"
             },
             "resolved": "https://registry.npmjs.org/stream-browserify/-/stream-browserify-3.0.0.tgz",
             "version": "3.0.0"
         },
         "streamroller": {
             "dependencies": {
-                "date-format": {
-                    "dev": true,
-                    "integrity": "sha512-bYQuGLeFxhkxNOF3rcMtiZxvCBAquGzZm6oWA1oZ0g2THUzivaRhv8uOhdr19LmoobSOLoIAxeUK2RdbM8IFTA==",
-                    "resolved": "https://registry.npmjs.org/date-format/-/date-format-2.1.0.tgz",
-                    "version": "2.1.0"
-                },
                 "debug": {
                     "dev": true,
-                    "integrity": "sha512-mOp8wKcvj7XxC78zLgw/ZA+6TSgkoE2C/ienthhRD298T7UNwAg9diBpLRxC0mOezLl4B0xV7M0cCO6P/O0Xhw==",
+                    "integrity": "sha512-/zxw5+vh1Tfv+4Qn7a5nsbcJKPaSvCDhojn6FEl9vupwK2VCSDtEiEtqr8DFtzYFOdz63LBkxec7DYuc2jon6Q==",
                     "requires": {
                         "ms": "2.1.2"
                     },
-                    "resolved": "https://registry.npmjs.org/debug/-/debug-4.3.2.tgz",
-                    "version": "4.3.2"
+                    "resolved": "https://registry.npmjs.org/debug/-/debug-4.3.3.tgz",
+                    "version": "4.3.3"
                 },
                 "ms": {
                     "dev": true,
                     "integrity": "sha512-sGkPx+VjMtmA6MX27oA4FBFELFCZZ4S4XqeGOXCv68tT+jb3vk/RyaKWP0PTKyWtmLSM0b+adUTEvbs1PEaH2w==",
                     "resolved": "https://registry.npmjs.org/ms/-/ms-2.1.2.tgz",
                     "version": "2.1.2"
                 }
             },
             "dev": true,
-            "integrity": "sha512-OG79qm3AujAM9ImoqgWEY1xG4HX+Lw+yY6qZj9R1K2mhF5bEmQ849wvrb+4vt4jLMLzwXttJlQbOdPOQVRv7DQ==",
+            "integrity": "sha512-ur6y5S5dopOaRXBuRIZ1u6GC5bcEXHRZKgfBjfCglMhmIf+roVCECjvkEYzNQOXIN2/JPnkMPW/8B3CZoKaEPA==",
             "requires": {
-                "date-format": "^2.1.0",
+                "date-format": "^4.0.3",
                 "debug": "^4.1.1",
-                "fs-extra": "^8.1.0"
+                "fs-extra": "^10.0.0"
             },
-            "resolved": "https://registry.npmjs.org/streamroller/-/streamroller-2.2.4.tgz",
-            "version": "2.2.4"
-        },
-        "string-width": {
-            "dev": true,
-            "integrity": "sha512-nOqH59deCq9SRHlxq1Aw85Jnt4w6KvLKqWVik6oA9ZklXLNIOlqg4F2yrT1MVaTjAqvVwdfeZ7w7aCvJD7ugkw==",
-            "requires": {
-                "is-fullwidth-code-point": "^2.0.0",
-                "strip-ansi": "^4.0.0"
-            },
-            "resolved": "https://registry.npmjs.org/string-width/-/string-width-2.1.1.tgz",
-            "version": "2.1.1"
+            "resolved": "https://registry.npmjs.org/streamroller/-/streamroller-3.0.2.tgz",
+            "version": "3.0.2"
         },
         "string.prototype.trimend": {
             "dev": true,
             "integrity": "sha512-y9xCjw1P23Awk8EvTpcyL2NIr1j7wJ39f+k6lvRnSMz+mz9CGz9NYPelDk42kOz6+ql8xjfK8oYzy3jAP5QU5A==",
             "requires": {
                 "call-bind": "^1.0.2",
                 "define-properties": "^1.1.3"
@@ -2695,14 +2743,22 @@
             "requires": {
                 "safe-buffer": "~5.2.0"
             },
             "resolved": "https://registry.npmjs.org/string_decoder/-/string_decoder-1.3.0.tgz",
             "version": "1.3.0"
         },
         "strip-ansi": {
+            "dependencies": {
+                "ansi-regex": {
+                    "dev": true,
+                    "integrity": "sha512-+O9Jct8wf++lXxxFc4hc8LsjaSq0HFzzL7cVsw8pRDIPdjKD2mT4ytDZlLuSBZ4cLKZFXIrMGO7DbQCtMJJMKw==",
+                    "resolved": "https://registry.npmjs.org/ansi-regex/-/ansi-regex-3.0.1.tgz",
+                    "version": "3.0.1"
+                }
+            },
             "dev": true,
             "integrity": "sha1-qEeQIusaw2iocTibY1JixQXuNo8=",
             "requires": {
                 "ansi-regex": "^3.0.0"
             },
             "resolved": "https://registry.npmjs.org/strip-ansi/-/strip-ansi-4.0.0.tgz",
             "version": "4.0.0"
@@ -2728,58 +2784,42 @@
                 "has-flag": "^4.0.0"
             },
             "resolved": "https://registry.npmjs.org/supports-color/-/supports-color-8.1.1.tgz",
             "version": "8.1.1"
         },
         "tapable": {
             "dev": true,
-            "integrity": "sha512-FBk4IesMV1rBxX2tfiK8RAmogtWn53puLOQlvO8XuwlgxcYbP4mVPS9Ph4aeamSyyVjOl24aYWAuc8U5kCVwMw==",
-            "resolved": "https://registry.npmjs.org/tapable/-/tapable-2.2.0.tgz",
-            "version": "2.2.0"
+            "integrity": "sha512-GNzQvQTOIP6RyTfE2Qxb8ZVlNmw0n88vp1szwWRimP02mnTsx3Wtn5qRdqY9w2XduFNUgvOwhNnQsjwCp+kqaQ==",
+            "resolved": "https://registry.npmjs.org/tapable/-/tapable-2.2.1.tgz",
+            "version": "2.2.1"
         },
         "terser": {
-            "dependencies": {
-                "source-map": {
-                    "dev": true,
-                    "integrity": "sha512-CkCj6giN3S+n9qrYiBTX5gystlENnRW5jZeNLHpe6aue+SrHcG5VYwujhW9s4dY31mEGsxBDrHR6oI69fTXsaQ==",
-                    "resolved": "https://registry.npmjs.org/source-map/-/source-map-0.7.3.tgz",
-                    "version": "0.7.3"
-                }
-            },
             "dev": true,
-            "integrity": "sha512-HP5/9hp2UaZt5fYkuhNBR8YyRcT8juw8+uFbAme53iN9hblvKnLUTKkmwJG6ocWpIKf8UK4DoeWG4ty0J6S6/g==",
+            "integrity": "sha512-hVl35zClmpisy6oaoKALOpS0rDYLxRFLHhRuDlEGTKey9qHjS1w9GMORjuwIMt70Wan4lwsLYyWDVnWgF+KUEw==",
             "requires": {
+                "@jridgewell/source-map": "^0.3.2",
+                "acorn": "^8.5.0",
                 "commander": "^2.20.0",
-                "source-map": "~0.7.2",
-                "source-map-support": "~0.5.19"
+                "source-map-support": "~0.5.20"
             },
-            "resolved": "https://registry.npmjs.org/terser/-/terser-5.7.0.tgz",
-            "version": "5.7.0"
+            "resolved": "https://registry.npmjs.org/terser/-/terser-5.17.1.tgz",
+            "version": "5.17.1"
         },
         "terser-webpack-plugin": {
-            "dependencies": {
-                "source-map": {
-                    "dev": true,
-                    "integrity": "sha512-UjgapumWlbMhkBgzT7Ykc5YXUT46F0iKu8SGXq0bcwP5dz/h0Plj6enJqjz1Zbq2l5WaqYnrVbwWOWMyF3F47g==",
-                    "resolved": "https://registry.npmjs.org/source-map/-/source-map-0.6.1.tgz",
-                    "version": "0.6.1"
-                }
-            },
             "dev": true,
-            "integrity": "sha512-cxGbMqr6+A2hrIB5ehFIF+F/iST5ZOxvOmy9zih9ySbP1C2oEWQSOUS+2SNBTjzx5xLKO4xnod9eywdfq1Nb9A==",
+            "integrity": "sha512-AfKwIktyP7Cu50xNjXF/6Qb5lBNzYaWpU6YfoX3uZicTx0zTy0stDDCsvjDapKsSDvOeWo5MEq4TmdBy2cNoHw==",
             "requires": {
-                "jest-worker": "^27.0.2",
-                "p-limit": "^3.1.0",
-                "schema-utils": "^3.0.0",
-                "serialize-javascript": "^5.0.1",
-                "source-map": "^0.6.1",
-                "terser": "^5.7.0"
+                "@jridgewell/trace-mapping": "^0.3.17",
+                "jest-worker": "^27.4.5",
+                "schema-utils": "^3.1.1",
+                "serialize-javascript": "^6.0.1",
+                "terser": "^5.16.5"
             },
-            "resolved": "https://registry.npmjs.org/terser-webpack-plugin/-/terser-webpack-plugin-5.1.3.tgz",
-            "version": "5.1.3"
+            "resolved": "https://registry.npmjs.org/terser-webpack-plugin/-/terser-webpack-plugin-5.3.7.tgz",
+            "version": "5.3.7"
         },
         "tmp": {
             "dev": true,
             "integrity": "sha512-76SUhtfqR2Ijn+xllcI5P1oyannHNHByD80W1q447gU3mp9G9PSpGdWmjUOHRDPiHYacIk66W7ubDTuPF3BEtQ==",
             "requires": {
                 "rimraf": "^3.0.0"
             },
@@ -2793,17 +2833,17 @@
                 "is-number": "^7.0.0"
             },
             "resolved": "https://registry.npmjs.org/to-regex-range/-/to-regex-range-5.0.1.tgz",
             "version": "5.0.1"
         },
         "toidentifier": {
             "dev": true,
-            "integrity": "sha512-yaOH/Pk/VEhBWWTlhI+qXxDFXlejDGcQipMlyxda9nthulaxLZUNcUqFxokp0vcYnvteJln5FNQDRrxj3YcbVw==",
-            "resolved": "https://registry.npmjs.org/toidentifier/-/toidentifier-1.0.0.tgz",
-            "version": "1.0.0"
+            "integrity": "sha512-o5sSPKEkg/DIQNmH43V0/uerLrpzVedkUh8tGNvaeXpfpuwjKenlSox/2O/BTlZUtEe+JG7s5YhEz608PlAHRA==",
+            "resolved": "https://registry.npmjs.org/toidentifier/-/toidentifier-1.0.1.tgz",
+            "version": "1.0.1"
         },
         "type-is": {
             "dev": true,
             "integrity": "sha512-TkRKr9sUTxEH8MdfuCSP7VizJyzRNMjj2J2do2Jr3Kym598JVdEksuzPQCnlFPW4ky9Q+iA+ma9BGm06XQBy8g==",
             "requires": {
                 "media-typer": "0.3.0",
                 "mime-types": "~2.1.24"
@@ -2815,17 +2855,17 @@
             "dev": true,
             "integrity": "sha512-BLbiRkiBzAwsjut4x/dsibSTB6yWpwT5qWmC2OfuCg3GgVQCSgMs4vEctYPhsaGtd0AeuuHMkjZ2h2WG8MSzRw==",
             "resolved": "https://registry.npmjs.org/typescript/-/typescript-3.9.7.tgz",
             "version": "3.9.7"
         },
         "ua-parser-js": {
             "dev": true,
-            "integrity": "sha512-6Gurc1n//gjp9eQNXjD9O3M/sMwVtN5S8Lv9bvOYBfKfDNiIIhqiyi01vMBO45u4zkDE420w/e0se7Vs+sIg+g==",
-            "resolved": "https://registry.npmjs.org/ua-parser-js/-/ua-parser-js-0.7.28.tgz",
-            "version": "0.7.28"
+            "integrity": "sha512-s8ax/CeZdK9R/56Sui0WM6y9OFREJarMRHqLB2EwkovemBxNQ+Bqu8GAsUnVcXKgphb++ghr/B2BZx4mahujPw==",
+            "resolved": "https://registry.npmjs.org/ua-parser-js/-/ua-parser-js-0.7.33.tgz",
+            "version": "0.7.33"
         },
         "unbox-primitive": {
             "dependencies": {
                 "has-symbols": {
                     "dev": true,
                     "integrity": "sha512-chXa79rL/UC2KlX17jo3vRGz0azaWEx5tGqZg5pO3NUyEJVB17dMruQlzCCOfUvElghKcm5194+BCRvi2Rv/Gw==",
                     "resolved": "https://registry.npmjs.org/has-symbols/-/has-symbols-1.0.2.tgz",
@@ -2841,24 +2881,34 @@
                 "which-boxed-primitive": "^1.0.2"
             },
             "resolved": "https://registry.npmjs.org/unbox-primitive/-/unbox-primitive-1.0.1.tgz",
             "version": "1.0.1"
         },
         "universalify": {
             "dev": true,
-            "integrity": "sha512-rBJeI5CXAlmy1pV+617WB9J63U6XcazHHF2f2dbJix4XzpUF0RS3Zbj0FGIOCAva5P/d/GBOYaACQ1w+0azUkg==",
-            "resolved": "https://registry.npmjs.org/universalify/-/universalify-0.1.2.tgz",
-            "version": "0.1.2"
+            "integrity": "sha512-hAZsKq7Yy11Zu1DE0OzWjw7nnLZmJZYTDZZyEFHZdUhV8FkH5MCfoU1XMaxXovpyW5nq5scPqq0ZDP9Zyl04oQ==",
+            "resolved": "https://registry.npmjs.org/universalify/-/universalify-2.0.0.tgz",
+            "version": "2.0.0"
         },
         "unpipe": {
             "dev": true,
             "integrity": "sha1-sr9O6FFKrmFltIF4KdIbLvSZBOw=",
             "resolved": "https://registry.npmjs.org/unpipe/-/unpipe-1.0.0.tgz",
             "version": "1.0.0"
         },
+        "update-browserslist-db": {
+            "dev": true,
+            "integrity": "sha512-dCwEFf0/oT85M1fHBg4F0jtLwJrutGoHSQXCh7u4o2t1drG+c0a9Flnqww6XUKSfQMPpJBRjU8d4RXB09qtvaA==",
+            "requires": {
+                "escalade": "^3.1.1",
+                "picocolors": "^1.0.0"
+            },
+            "resolved": "https://registry.npmjs.org/update-browserslist-db/-/update-browserslist-db-1.0.11.tgz",
+            "version": "1.0.11"
+        },
         "uri-js": {
             "dev": true,
             "integrity": "sha512-7rKUyy33Q1yc98pQ1DAmLtwX109F7TIfWlW1Ydo8Wl1ii1SeHieeh0HHfPeL2fMXK6z0s8ecKs9frCuLJvndBg==",
             "requires": {
                 "punycode": "^2.1.0"
             },
             "resolved": "https://registry.npmjs.org/uri-js/-/uri-js-4.4.1.tgz",
@@ -2900,88 +2950,76 @@
             "dev": true,
             "integrity": "sha1-wGavtYK7HLQSjWDqkjkulNXp2+w=",
             "resolved": "https://registry.npmjs.org/void-elements/-/void-elements-2.0.1.tgz",
             "version": "2.0.1"
         },
         "watchpack": {
             "dev": true,
-            "integrity": "sha512-up4YAn/XHgZHIxFBVCdlMiWDj6WaLKpwVeGQk2I5thdYxF/KmF0aaz6TfJZ/hfl1h/XlcDr7k1KH7ThDagpFaA==",
+            "integrity": "sha512-Lcvm7MGST/4fup+ifyKi2hjyIAwcdI4HRgtvTpIUxBRhB+RFtUh8XtDOxUfctVCnhVi+QQj49i91OyvzkJl6cg==",
             "requires": {
                 "glob-to-regexp": "^0.4.1",
                 "graceful-fs": "^4.1.2"
             },
-            "resolved": "https://registry.npmjs.org/watchpack/-/watchpack-2.2.0.tgz",
-            "version": "2.2.0"
+            "resolved": "https://registry.npmjs.org/watchpack/-/watchpack-2.4.0.tgz",
+            "version": "2.4.0"
         },
         "webpack": {
+            "dependencies": {
+                "graceful-fs": {
+                    "dev": true,
+                    "integrity": "sha512-RbJ5/jmFcNNCcDV5o9eTnBLJ/HszWV0P73bc+Ff4nS/rJj+YaS6IGyiOL0VoBYX+l1Wrl3k63h/KrH+nhJ0XvQ==",
+                    "resolved": "https://registry.npmjs.org/graceful-fs/-/graceful-fs-4.2.11.tgz",
+                    "version": "4.2.11"
+                }
+            },
             "dev": true,
-            "integrity": "sha512-25CHmuDj+oOTyteI13sUqNlCnjCnySuhiKWE/cRYPQYeoQ3ijHgyWX27CiyUKLNGq27v8S0mrksyTreT/xo7pg==",
+            "integrity": "sha512-l5sOdYBDunyf72HW8dF23rFtWq/7Zgvt/9ftMof71E/yUb1YLOBmTgA2K4vQthB3kotMrSj609txVE0dnr2fjA==",
             "requires": {
-                "@types/eslint-scope": "^3.7.0",
-                "@types/estree": "^0.0.47",
-                "@webassemblyjs/ast": "1.11.0",
-                "@webassemblyjs/wasm-edit": "1.11.0",
-                "@webassemblyjs/wasm-parser": "1.11.0",
-                "acorn": "^8.2.1",
+                "@types/eslint-scope": "^3.7.3",
+                "@types/estree": "^0.0.51",
+                "@webassemblyjs/ast": "1.11.1",
+                "@webassemblyjs/wasm-edit": "1.11.1",
+                "@webassemblyjs/wasm-parser": "1.11.1",
+                "acorn": "^8.7.1",
+                "acorn-import-assertions": "^1.7.6",
                 "browserslist": "^4.14.5",
                 "chrome-trace-event": "^1.0.2",
-                "enhanced-resolve": "^5.8.0",
-                "es-module-lexer": "^0.4.0",
+                "enhanced-resolve": "^5.10.0",
+                "es-module-lexer": "^0.9.0",
                 "eslint-scope": "5.1.1",
                 "events": "^3.2.0",
                 "glob-to-regexp": "^0.4.1",
-                "graceful-fs": "^4.2.4",
-                "json-parse-better-errors": "^1.0.2",
+                "graceful-fs": "^4.2.9",
+                "json-parse-even-better-errors": "^2.3.1",
                 "loader-runner": "^4.2.0",
                 "mime-types": "^2.1.27",
                 "neo-async": "^2.6.2",
-                "schema-utils": "^3.0.0",
+                "schema-utils": "^3.1.0",
                 "tapable": "^2.1.1",
-                "terser-webpack-plugin": "^5.1.1",
-                "watchpack": "^2.2.0",
-                "webpack-sources": "^2.3.0"
+                "terser-webpack-plugin": "^5.1.3",
+                "watchpack": "^2.4.0",
+                "webpack-sources": "^3.2.3"
             },
-            "resolved": "https://registry.npmjs.org/webpack/-/webpack-5.39.0.tgz",
-            "version": "5.39.0"
+            "resolved": "https://registry.npmjs.org/webpack/-/webpack-5.76.0.tgz",
+            "version": "5.76.0"
         },
         "webpack-merge": {
             "dev": true,
             "integrity": "sha512-TUE1UGoTX2Cd42j3krGYqObZbOD+xF7u28WB7tfUordytSjbWTIjK/8V0amkBfTYN4/pB/GIDlJZZ657BGG19g==",
             "requires": {
                 "lodash": "^4.17.15"
             },
             "resolved": "https://registry.npmjs.org/webpack-merge/-/webpack-merge-4.2.2.tgz",
             "version": "4.2.2"
         },
         "webpack-sources": {
-            "dependencies": {
-                "source-map": {
-                    "dev": true,
-                    "integrity": "sha512-UjgapumWlbMhkBgzT7Ykc5YXUT46F0iKu8SGXq0bcwP5dz/h0Plj6enJqjz1Zbq2l5WaqYnrVbwWOWMyF3F47g==",
-                    "resolved": "https://registry.npmjs.org/source-map/-/source-map-0.6.1.tgz",
-                    "version": "0.6.1"
-                }
-            },
-            "dev": true,
-            "integrity": "sha512-WyOdtwSvOML1kbgtXbTDnEW0jkJ7hZr/bDByIwszhWd/4XX1A3XMkrbFMsuH4+/MfLlZCUzlAdg4r7jaGKEIgQ==",
-            "requires": {
-                "source-list-map": "^2.0.1",
-                "source-map": "^0.6.1"
-            },
-            "resolved": "https://registry.npmjs.org/webpack-sources/-/webpack-sources-2.3.0.tgz",
-            "version": "2.3.0"
-        },
-        "which": {
             "dev": true,
-            "integrity": "sha512-BLI3Tl1TW3Pvl70l3yq3Y64i+awpwXqsGBYWkkqMtnbXgrMD+yj7rhW0kuEDxzJaYXGjEW5ogapKNMEKNMjibA==",
-            "requires": {
-                "isexe": "^2.0.0"
-            },
-            "resolved": "https://registry.npmjs.org/which/-/which-2.0.2.tgz",
-            "version": "2.0.2"
+            "integrity": "sha512-/DyMEOrDgLKKIG0fmvtz+4dUX/3Ghozwgm6iPp8KRhvn+eQf9+Q7GWxVNMk3+uCPWfdXYC4ExGBckIXdFEfH1w==",
+            "resolved": "https://registry.npmjs.org/webpack-sources/-/webpack-sources-3.2.3.tgz",
+            "version": "3.2.3"
         },
         "which-boxed-primitive": {
             "dev": true,
             "integrity": "sha512-bwZdv0AKLpplFY2KZRX6TvyuN7ojjr7lwkg6ml0roIy9YeuSr7JS372qlNW18UQYzgYK9ziGcerWqZOmEn9VNg==",
             "requires": {
                 "is-bigint": "^1.0.1",
                 "is-boolean-object": "^1.1.0",
@@ -3011,37 +3049,22 @@
                 "function-bind": "^1.1.1",
                 "has-symbols": "^1.0.1",
                 "is-typed-array": "^1.1.3"
             },
             "resolved": "https://registry.npmjs.org/which-typed-array/-/which-typed-array-1.1.4.tgz",
             "version": "1.1.4"
         },
-        "wide-align": {
-            "dev": true,
-            "integrity": "sha512-QGkOQc8XL6Bt5PwnsExKBPuMKBxnGxWWW3fU55Xt4feHozMUhdUMaBCk290qpm/wG5u/RSKzwdAC4i51YigihA==",
-            "requires": {
-                "string-width": "^1.0.2 || 2"
-            },
-            "resolved": "https://registry.npmjs.org/wide-align/-/wide-align-1.1.3.tgz",
-            "version": "1.1.3"
-        },
         "workerpool": {
             "dev": true,
-            "integrity": "sha512-toV7q9rWNYha963Pl/qyeZ6wG+3nnsyvolaNUS8+R5Wtw6qJPTxIlOP1ZSvcGhEJw+l3HMMmtiNo9Gl61G4GVg==",
-            "resolved": "https://registry.npmjs.org/workerpool/-/workerpool-6.1.0.tgz",
-            "version": "6.1.0"
+            "integrity": "sha512-ILEIE97kDZvF9Wb9f6h5aXK4swSlKGUcOEGiIYb2OOu/IrDU9iwj0fD//SsA6E5ibwJxpEvhullJY4Sl4GcpAw==",
+            "resolved": "https://registry.npmjs.org/workerpool/-/workerpool-6.2.1.tgz",
+            "version": "6.2.1"
         },
         "wrap-ansi": {
             "dependencies": {
-                "ansi-regex": {
-                    "dev": true,
-                    "integrity": "sha512-bY6fj56OUQ0hU1KjFNDQuJFezqKdrAyFdIevADiqrWHwSlbmBNMHp5ak2f40Pm8JTFyM2mqxkG6ngkHO11f/lg==",
-                    "resolved": "https://registry.npmjs.org/ansi-regex/-/ansi-regex-5.0.0.tgz",
-                    "version": "5.0.0"
-                },
                 "ansi-styles": {
                     "dev": true,
                     "integrity": "sha512-zbB9rCJAT1rbjiVDb2hqKFHNYLxgtk8NURxZ3IZwD3F6NtxbXZQCnnSi1Lkx+IDohdPlFp222wVALIheZJQSEg==",
                     "requires": {
                         "color-convert": "^2.0.1"
                     },
                     "resolved": "https://registry.npmjs.org/ansi-styles/-/ansi-styles-4.3.0.tgz",
@@ -3103,26 +3126,20 @@
             "dev": true,
             "integrity": "sha1-tSQ9jz7BqjXxNkYFvA0QNuMKtp8=",
             "resolved": "https://registry.npmjs.org/wrappy/-/wrappy-1.0.2.tgz",
             "version": "1.0.2"
         },
         "ws": {
             "dev": true,
-            "integrity": "sha512-YmhHDO4MzaDLB+M9ym/mDA5z0naX8j7SIlT8f8z+I0VtzsRbekxEutHSme7NPS2qE8StCYQNUnfWdXta/Yu85A==",
-            "resolved": "https://registry.npmjs.org/ws/-/ws-7.4.6.tgz",
-            "version": "7.4.6"
+            "integrity": "sha512-HPG3wQd9sNQoT9xHyNCXoDUa+Xw/VevmY9FoHyQ+g+rrMn4j6FB4np7Z0OhdTgjx6MgQLK7jwSy1YecU1+4Asg==",
+            "resolved": "https://registry.npmjs.org/ws/-/ws-8.11.0.tgz",
+            "version": "8.11.0"
         },
         "yargs": {
             "dependencies": {
-                "ansi-regex": {
-                    "dev": true,
-                    "integrity": "sha512-bY6fj56OUQ0hU1KjFNDQuJFezqKdrAyFdIevADiqrWHwSlbmBNMHp5ak2f40Pm8JTFyM2mqxkG6ngkHO11f/lg==",
-                    "resolved": "https://registry.npmjs.org/ansi-regex/-/ansi-regex-5.0.0.tgz",
-                    "version": "5.0.0"
-                },
                 "is-fullwidth-code-point": {
                     "dev": true,
                     "integrity": "sha512-zymm5+u+sCsSWyD9qNaejV3DFvhCKclKdizYaJUuHA83RLjb7nSuGnddCHGv0hk+KY7BMAlsWeK4Ueg6EV6XQg==",
                     "resolved": "https://registry.npmjs.org/is-fullwidth-code-point/-/is-fullwidth-code-point-3.0.0.tgz",
                     "version": "3.0.0"
                 },
                 "string-width": {
@@ -3169,28 +3186,14 @@
         "yargs-parser": {
             "dev": true,
             "integrity": "sha512-WOkpgNhPTlE73h4VFAFsOnomJVaovO8VqLDzy5saChRBFQFBoMYirowyW+Q9HB4HFF4Z7VZTiG3iSzJJA29yRA==",
             "resolved": "https://registry.npmjs.org/yargs-parser/-/yargs-parser-20.2.4.tgz",
             "version": "20.2.4"
         },
         "yargs-unparser": {
-            "dependencies": {
-                "camelcase": {
-                    "dev": true,
-                    "integrity": "sha512-c7wVvbw3f37nuobQNtgsgG9POC9qMbNuMQmTCqZv23b6MIz0fcYpBiOlv9gEN/hdLdnZTDQhg6e9Dq5M1vKvfg==",
-                    "resolved": "https://registry.npmjs.org/camelcase/-/camelcase-6.2.0.tgz",
-                    "version": "6.2.0"
-                },
-                "decamelize": {
-                    "dev": true,
-                    "integrity": "sha512-9iE1PgSik9HeIIw2JO94IidnE3eBoQrFJ3w7sFuzSX4DpmZ3v5sZpUiV5Swcf6mQEF+Y0ru8Neo+p+nyh2J+hQ==",
-                    "resolved": "https://registry.npmjs.org/decamelize/-/decamelize-4.0.0.tgz",
-                    "version": "4.0.0"
-                }
-            },
             "dev": true,
             "integrity": "sha512-7pRTIA9Qc1caZ0bZ6RYRGbHJthJWuakf+WmHK0rVeLkNrrGhfoabBNdue6kdINI6r4if7ocq9aD/n7xwKOdzOA==",
             "requires": {
                 "camelcase": "^6.0.0",
                 "decamelize": "^4.0.0",
                 "flat": "^5.0.2",
                 "is-plain-obj": "^2.1.0"
```

### Comparing `blspy-1.0.9/js-bindings/package.json` & `blspy-2.0.0b1/js-bindings/package.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9990079365079365%*

 * *Differences: {"'devDependencies'": "{'mocha': '^10.2.0'}"}*

```diff
@@ -17,15 +17,15 @@
         "crypto-browserify": "^3.12.0",
         "karma": "^6.3.4",
         "karma-firefox-launcher": "^1.3.0",
         "karma-mocha": "^2.0.1",
         "karma-mocha-reporter": "^2.2.5",
         "karma-webpack": "^5.0.0",
         "mime": "1.4.1",
-        "mocha": "^8.4.0",
+        "mocha": "^10.2.0",
         "path-browserify": "^1.0.1",
         "process": "^0.11.10",
         "stream-browserify": "^3.0.0",
         "typescript": "^3.6.5",
         "webpack": "^5.39.0"
     },
     "directories": {
```

### Comparing `blspy-1.0.9/js-bindings/tests/PrivateKey.spec.js` & `blspy-2.0.0b1/js-bindings/tests/PrivateKey.spec.js`

 * *Files identical despite different names*

### Comparing `blspy-1.0.9/js-bindings/tests/PublicKey.spec.js` & `blspy-2.0.0b1/js-bindings/tests/PublicKey.spec.js`

 * *Files identical despite different names*

### Comparing `blspy-1.0.9/js-bindings/tests/Signature.spec.js` & `blspy-2.0.0b1/js-bindings/tests/Signature.spec.js`

 * *Files identical despite different names*

### Comparing `blspy-1.0.9/js-bindings/tests/karma.conf.js` & `blspy-2.0.0b1/js-bindings/tests/karma.conf.js`

 * *Files identical despite different names*

### Comparing `blspy-1.0.9/js-bindings/tests/test.js` & `blspy-2.0.0b1/js-bindings/tests/test.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -18,15 +18,14 @@
     return range(32).map(() => v);
 }
 
 blsjs().then((blsjs) => {
     const modules = [
         'AugSchemeMPL',
         'BasicSchemeMPL',
-        "Bignum",
         'G1Element',
         'G2Element',
         'PopSchemeMPL',
         'PrivateKey',
         'Util'
     ];
 
@@ -38,15 +37,14 @@
             process.exit(1);
         }
     }
 
     const {
         AugSchemeMPL,
         BasicSchemeMPL,
-        Bignum,
         G1Element,
         G2Element,
         PopSchemeMPL,
         PrivateKey,
         Util
     } = blsjs;
 
@@ -376,25 +374,19 @@
         assert(ok);
     }
 
     function test_aggregate_verify_zero_items() {
         assert(AugSchemeMPL.aggregate_verify([], [], new G2Element()));
     }
 
-    function test_bignum() {
-        const mersenne = Bignum.fromString('162259276829213363391578010288127', 10);
-        assert(mersenne.toString(16).toLowerCase() == '7ffffffffffffffffffffffffff');
-    }
-
     test_schemes();
     test_vectors_invalid();
     test_vectors_valid();
     test_readme();
     test_aggregate_verify_zero_items();
-    test_bignum();
 }).then(function() {
     console.log("\nAll tests passed.");
 });
 
 const copyright = [
     'Copyright 2020 Chia Network Inc',
     'Licensed under the Apache License, Version 2.0 (the "License");',
```

### Comparing `blspy-1.0.9/js-bindings/tests/typings.spec.ts` & `blspy-2.0.0b1/js-bindings/tests/typings.spec.ts`

 * *Files identical despite different names*

### Comparing `blspy-1.0.9/js-bindings/tests/yarn.lock` & `blspy-2.0.0b1/js-bindings/tests/yarn.lock`

 * *Files identical despite different names*

### Comparing `blspy-1.0.9/js-bindings/wrappers/BignumWrapper.h` & `blspy-2.0.0b1/js-bindings/wrappers/JSWrapper.h`

 * *Files 22% similar despite different names*

```diff
@@ -8,35 +8,25 @@
 
 // Unless required by applicable law or agreed to in writing, software
 // distributed under the License is distributed on an "AS IS" BASIS,
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.
 
-#ifndef JS_BINDINGS_WRAPPERS_BIGNUMWRAPPER_H_
-#define JS_BINDINGS_WRAPPERS_BIGNUMWRAPPER_H_
-
-#include "../helpers.h"
-#include "JSWrapper.h"
+#ifndef JS_BINDINGS_WRAPPERS_JSWRAPPER_H_
+#define JS_BINDINGS_WRAPPERS_JSWRAPPER_H_
 
 namespace js_wrappers {
-class Bignum {
-public:
-    Bignum();
-    ~Bignum();
-    Bignum(const Bignum &other);
-
-    bn_st *operator &();
-
-private:
-    bn_st content;
-};
-
-class BignumWrapper : public JSWrapper<Bignum> {
-public:
-    explicit BignumWrapper(const Bignum &bn);
-    static BignumWrapper FromString(const std::string &s, int radix);
-    std::string ToString(int radix);
+template<class T>
+class JSWrapper {
+ public:
+    inline explicit JSWrapper(const T &wrappedInstance) : wrapped(wrappedInstance) {}
+
+    inline T GetWrappedInstance() const {
+        return wrapped;
+    }
+ protected:
+    T wrapped;
 };
 }  // namespace js_wrappers
 
-#endif  // JS_BINDINGS_WRAPPERS_SIGNATUREWRAPPER_H_
+#endif  // JS_BINDINGS_WRAPPERS_JSWRAPPER_H_
```

### Comparing `blspy-1.0.9/js-bindings/wrappers/G1ElementWrapper.cpp` & `blspy-2.0.0b1/js-bindings/wrappers/G1ElementWrapper.cpp`

 * *Files 26% similar despite different names*

```diff
@@ -40,24 +40,14 @@
     return helpers::toUint8Array(wrapped.Serialize());
 }
 
 G1ElementWrapper G1ElementWrapper::Add(const G1ElementWrapper &other) {
     return G1ElementWrapper(GetWrappedInstance() + other.GetWrappedInstance());
 }
 
-G1ElementWrapper G1ElementWrapper::Mul(const BignumWrapper &other) {
-    bn_t factor;
-    // Since the type of bn_t is bn_st[0], we can do this dance to make a temporary
-    // copy of the struct itself to hand to G1ElementWrapper's multiply.  The
-    // type was clearly intended to by by-value in argument lists (degrade to ptr)
-    // but value semantics in C++ complicates matters.
-    factor[0] = *(&other.GetWrappedInstance());
-    return G1ElementWrapper(GetWrappedInstance() * factor);
-}
-
 bool G1ElementWrapper::EqualTo(const G1ElementWrapper &others) {
     return GetWrappedInstance() == others.GetWrappedInstance();
 }
 
 G1ElementWrapper G1ElementWrapper::Negate() {
     return G1ElementWrapper(GetWrappedInstance().Negate());
 }
```

### Comparing `blspy-1.0.9/js-bindings/wrappers/G1ElementWrapper.h` & `blspy-2.0.0b1/js-bindings/wrappers/G2ElementWrapper.h`

 * *Files 10% similar despite different names*

```diff
@@ -8,46 +8,45 @@
 
 // Unless required by applicable law or agreed to in writing, software
 // distributed under the License is distributed on an "AS IS" BASIS,
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.
 
-#ifndef JS_BINDINGS_WRAPPERS_G1ELEMENTWRAPPER_H_
-#define JS_BINDINGS_WRAPPERS_G1ELEMENTWRAPPER_H_
+#ifndef JS_BINDINGS_WRAPPERS_G2ELEMENTWRAPPER_H_
+#define JS_BINDINGS_WRAPPERS_G2ELEMENTWRAPPER_H_
 
 #include "../helpers.h"
 #include "JSWrapper.h"
-#include "BignumWrapper.h"
 
 namespace js_wrappers {
-class G1ElementWrapper : public JSWrapper<G1Element> {
-public:
-    explicit G1ElementWrapper(const G1Element &publicKey);
+class G2ElementWrapper : public JSWrapper<G2Element> {
+ public:
+    explicit G2ElementWrapper(const G2Element &signature);
 
-    G1ElementWrapper();
+    G2ElementWrapper();
 
     static const size_t SIZE;
 
-    static std::vector <G1Element> Unwrap(std::vector <G1ElementWrapper> wrappers);
+    static std::vector <G2Element> Unwrap(std::vector <G2ElementWrapper> sigWrappers);
 
-    static G1ElementWrapper FromBytes(val buffer);
+    static G2ElementWrapper FromG2Element(const G2Element &signature);
 
-    static G1ElementWrapper Generator();
+    static G2ElementWrapper FromBytes(val buffer);
 
-    val Serialize() const;
+    static G2ElementWrapper AggregateSigs(val signatureWrappers);
 
-    G1ElementWrapper Add(const G1ElementWrapper &other);
+    static G2ElementWrapper Generator();
 
-    G1ElementWrapper Mul(const BignumWrapper &other);
+    G2ElementWrapper Deepcopy();
 
-    bool EqualTo(const G1ElementWrapper &others);
+    G2ElementWrapper Negate();
 
-    G1ElementWrapper Negate();
+    val Serialize() const;
 
-    G1ElementWrapper Deepcopy();
+    G2ElementWrapper Add(const G2ElementWrapper &other);
 
-    uint32_t GetFingerprint() const;
+    bool EqualTo(const G2ElementWrapper &others);
 };
 }  // namespace js_wrappers
 
-#endif  // JS_BINDINGS_WRAPPERS_G1ELEMENTWRAPPER_H_
+#endif  // JS_BINDINGS_WRAPPERS_G2ELEMENTWRAPPER_H_
```

### Comparing `blspy-1.0.9/js-bindings/wrappers/G2ElementWrapper.cpp` & `blspy-2.0.0b1/js-bindings/wrappers/G2ElementWrapper.cpp`

 * *Files 27% similar despite different names*

```diff
@@ -63,21 +63,11 @@
     return helpers::toUint8Array(wrapped.Serialize());
 }
 
 G2ElementWrapper G2ElementWrapper::Add(const G2ElementWrapper& other) {
     return G2ElementWrapper(GetWrappedInstance() + other.GetWrappedInstance());
 }
 
-G2ElementWrapper G2ElementWrapper::Mul(const BignumWrapper& other) {
-    bn_t factor;
-    // Since the type of bn_t is bn_st[0], we can do this dance to make a
-    // temporary copy of the struct itself to hand to G2ElementWrapper's
-    // multiply.  The type was clearly intended to by by-value in argument lists
-    // (degrade to ptr) but value semantics in C++ complicates matters.
-    factor[0] = *(&other.GetWrappedInstance());
-    return G2ElementWrapper(GetWrappedInstance() * factor);
-}
-
 bool G2ElementWrapper::EqualTo(const G2ElementWrapper& others) {
     return GetWrappedInstance() == others.GetWrappedInstance();
 }
 }  // namespace js_wrappers
```

### Comparing `blspy-1.0.9/js-bindings/wrappers/JSWrapper.h` & `blspy-2.0.0b1/js-bindings/wrappers/UtilWrapper.h`

 * *Files 27% similar despite different names*

```diff
@@ -8,25 +8,22 @@
 
 // Unless required by applicable law or agreed to in writing, software
 // distributed under the License is distributed on an "AS IS" BASIS,
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.
 
-#ifndef JS_BINDINGS_WRAPPERS_JSWRAPPER_H_
-#define JS_BINDINGS_WRAPPERS_JSWRAPPER_H_
+#ifndef JS_BINDINGS_WRAPPERS_UTILWRAPPER_H_
+#define JS_BINDINGS_WRAPPERS_UTILWRAPPER_H_
 
-namespace js_wrappers {
-template<class T>
-class JSWrapper {
- public:
-    inline explicit JSWrapper(const T &wrappedInstance) : wrapped(wrappedInstance) {}
+#include "../helpers.h"
+#include "JSWrapper.h"
 
-    inline T GetWrappedInstance() const {
-        return wrapped;
-    }
- protected:
-    T wrapped;
+namespace js_wrappers {
+class UtilWrapper : public JSWrapper<Util> {
+public:
+    static val Hash256(val message);
+    static std::string HexStr(val message);
 };
 }  // namespace js_wrappers
 
-#endif  // JS_BINDINGS_WRAPPERS_JSWRAPPER_H_
+#endif  // JS_BINDINGS_WRAPPERS_SIGNATUREWRAPPER_H_
```

### Comparing `blspy-1.0.9/js-bindings/wrappers/PrivateKeyWrapper.cpp` & `blspy-2.0.0b1/js-bindings/wrappers/PrivateKeyWrapper.cpp`

 * *Files identical despite different names*

### Comparing `blspy-1.0.9/js-bindings/wrappers/PrivateKeyWrapper.h` & `blspy-2.0.0b1/js-bindings/wrappers/PrivateKeyWrapper.h`

 * *Files identical despite different names*

### Comparing `blspy-1.0.9/js-bindings/wrappers/SchemeMPLWrapper.cpp` & `blspy-2.0.0b1/js-bindings/wrappers/SchemeMPLWrapper.cpp`

 * *Files identical despite different names*

### Comparing `blspy-1.0.9/js-bindings/wrappers/SchemeMPLWrapper.h` & `blspy-2.0.0b1/js-bindings/wrappers/SchemeMPLWrapper.h`

 * *Files identical despite different names*

### Comparing `blspy-1.0.9/js-bindings/wrappers/UtilWrapper.cpp` & `blspy-2.0.0b1/js-bindings/wrappers/UtilWrapper.cpp`

 * *Files identical despite different names*

### Comparing `blspy-1.0.9/python-bindings/README.md` & `blspy-2.0.0b1/python-bindings/README.md`

 * *Files identical despite different names*

### Comparing `blspy-1.0.9/python-bindings/benchmark.py` & `blspy-2.0.0b1/python-bindings/benchmark.py`

 * *Files identical despite different names*

### Comparing `blspy-1.0.9/python-bindings/test.py` & `blspy-2.0.0b1/python-bindings/test.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # flake8: noqa: E501
 import binascii
+import time
 from copy import deepcopy
 
 from blspy import (
     AugSchemeMPL,
     BasicSchemeMPL,
     G1Element,
     G2Element,
@@ -36,14 +37,20 @@
     seed = bytes([1]) + seed[1:]
     sk1 = BasicSchemeMPL.key_gen(seed)
     pk1 = sk1.get_g1()
     seed = bytes([2]) + seed[1:]
     sk2 = BasicSchemeMPL.key_gen(seed)
     pk2 = sk2.get_g1()
 
+    g1 = G1Element.from_message(b"abcd", b"BLS_SIG_BLS12381G2_XMD:SHA-256_SSWU_RO_AUG_")
+    assert bytes(g1) == bytes.fromhex("a5f756594a96c55f302360378568378dc19ea5eae3d5a88d77b8a30bb25c25ce24a85c6d7c851bcb1e34064fc0c79383")
+
+    g2 = G2Element.from_message(b"abcd", b"BLS_SIG_BLS12381G2_XMD:SHA-256_SSWU_RO_AUG_")
+    assert g2 == AugSchemeMPL.g2_from_message(b"abcd")
+
     for Scheme in (BasicSchemeMPL, AugSchemeMPL, PopSchemeMPL):
         # Aggregate same message
         agg_pk = pk1 + pk2
         if Scheme is AugSchemeMPL:
             sig1 = Scheme.sign(sk1, msg, agg_pk)
             sig2 = Scheme.sign(sk2, msg, agg_pk)
         else:
@@ -331,19 +338,54 @@
     assert ok
 
 
 def test_aggregate_verify_zero_items():
     assert AugSchemeMPL.aggregate_verify([], [], G2Element())
 
 
+def test_invalid_points():
+    sk1 = BasicSchemeMPL.key_gen(b"1" *32)
+    good_point = sk1.get_g1()
+    good_point_bytes = bytes(good_point)
+    start = time.time()
+    for i in range(2000):
+        gp1 = G1Element.from_bytes(good_point_bytes)
+    print(f"from_bytes avg: {(time.time() - start) }")
+
+    start = time.time()
+    for i in range(2000):
+        gp2 = G1Element.from_bytes_unchecked(good_point_bytes)
+    print(f"from_bytes_unchecked avg: {(time.time() - start) }")
+    assert gp1 == gp2
+
+    bad_point_hex: str = "8d5d0fb73b9c92df4eab4216e48c3e358578b4cc30f82c268bd6fef3bd34b558628daf1afef798d4c3b0fcd8b28c8973";
+    try:
+        G1Element.from_bytes(bytes.fromhex(bad_point_hex))
+        assert False
+    except ValueError:
+        pass
+
+    p: G1Element = G1Element.from_bytes_unchecked(bytes.fromhex(bad_point_hex))
+
+    bad_g2_point_hex = "8f2886c94eaeac335c8414cbf14c16681b225380cfee3293becc4531d5b415984b4ea4050d9ecda11fbc21c60627e9d212dfcb17d2b5ae399aa3fbcb099e05baa496b852ad976fb633cc6766b02fca4da549dc063908463b2906ad64e8b310ad"
+
+    try:
+        G2Element.from_bytes(bytes.fromhex(bad_g2_point_hex))
+        assert False
+    except ValueError:
+        pass
+
+
+
 test_schemes()
 test_vectors_invalid()
 test_vectors_valid()
 test_readme()
 test_aggregate_verify_zero_items()
+test_invalid_points()
 
 print("\nAll tests passed.")
 
 """
 Copyright 2020 Chia Network Inc
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
```

### Comparing `blspy-1.0.9/python-impl/bls12381.py` & `blspy-2.0.0b1/python-impl/bls12381.py`

 * *Files identical despite different names*

### Comparing `blspy-1.0.9/python-impl/ec.py` & `blspy-2.0.0b1/python-impl/ec.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,14 +80,17 @@
             + ", y="
             + self.y.__repr__()
             + ", i="
             + str(self.infinity)
             + ")\n"
         )
 
+    def __bytes__(self) -> bytes:
+        return point_to_bytes(self, self.ec, self.FE)
+
     def __eq__(self, other) -> bool:
         if not isinstance(other, AffinePoint):
             return False
         return (
             self.x == other.x and self.y == other.y and self.infinity == other.infinity
         )
 
@@ -233,16 +236,20 @@
 def sign_Fq2(element, ec=default_ec_twist) -> bool:
     if element[1] == Fq(ec.q, 0):
         return sign_Fq(element[0])
 
     return element[1] > Fq(ec.q, ((ec.q - 1) // 2))
 
 
-def point_to_bytes(point_j: JacobianPoint, ec, FE) -> bytes:
-    point = point_j.to_affine()
+def point_to_bytes(point, ec, FE) -> bytes:
+    # Zcash serialization described in https://datatracker.ietf.org/doc/draft-irtf-cfrg-pairing-friendly-curves/
+    if isinstance(point, JacobianPoint):
+        point = point.to_affine()
+    if not isinstance(point, AffinePoint):
+        raise Exception("point should either be JacobianPoint or AffinePoint")
     output = bytearray(bytes(point.x))
 
     # If the y coordinate is the bigger one of the two, set the first
     # bit to 1.
     if point.infinity:
         return bytes([0x40]) + bytes([0] * (len(output) - 1))
 
@@ -255,15 +262,15 @@
         output[0] |= 0xA0
     else:
         output[0] |= 0x80
     return bytes(output)
 
 
 def bytes_to_point(buffer: bytes, ec, FE) -> JacobianPoint:
-    # Zcash serialization described in https://datatracker.ietf.org/doc/draft-irtf-cfrg-pairing-friendly-curves/
+    # Zcash deserialization described in https://datatracker.ietf.org/doc/draft-irtf-cfrg-pairing-friendly-curves/
 
     if FE == Fq:
         if len(buffer) != 48:
             raise ValueError("G1Elements must be 48 bytes")
     elif FE == Fq2:
         if len(buffer) != 96:
             raise ValueError("G2Elements must be 96 bytes")
@@ -271,17 +278,17 @@
         raise ValueError("Invalid FE")
 
     m_byte = buffer[0] & 0xE0
 
     if m_byte in [0x20, 0x60, 0xE0]:
         raise ValueError("Invalid first three bits")
 
-    C_bit = m_byte & 0x80  # First bit
-    I_bit = m_byte & 0x40  # Second bit
-    S_bit = m_byte & 0x20  # Third bit
+    C_bit = (m_byte & 0x80) >> 7  # First bit
+    I_bit = (m_byte & 0x40) >> 6  # Second bit
+    S_bit = (m_byte & 0x20) >> 5  # Third bit
 
     if C_bit == 0:
         raise ValueError("First bit must be 1 (only compressed points)")
 
     buffer = bytes([buffer[0] & 0x1F]) + buffer[1:]
 
     if I_bit == 1:
```

### Comparing `blspy-1.0.9/python-impl/fields.py` & `blspy-2.0.0b1/python-impl/fields.py`

 * *Files identical despite different names*

### Comparing `blspy-1.0.9/python-impl/hash_to_field.py` & `blspy-2.0.0b1/python-impl/hash_to_field.py`

 * *Files identical despite different names*

### Comparing `blspy-1.0.9/python-impl/hd_keys.py` & `blspy-2.0.0b1/python-impl/hd_keys.py`

 * *Files identical despite different names*

### Comparing `blspy-1.0.9/python-impl/hkdf.py` & `blspy-2.0.0b1/python-impl/hkdf.py`

 * *Files identical despite different names*

### Comparing `blspy-1.0.9/python-impl/impl-test.py` & `blspy-2.0.0b1/python-impl/impl-test.py`

 * *Files 3% similar despite different names*

```diff
@@ -367,14 +367,51 @@
     assert bytes(agg_sig_2).hex() == (
         "a0b1378d518bea4d1100adbc7bdbc4ff64f2c219ed6395cd36fe5d2aa44a4b8e710b607afd9"
         "65e505a5ac3283291b75413d09478ab4b5cfbafbeea366de2d0c0bcf61deddaa521f6020460f"
         "d547ab37659ae207968b545727beba0a3c5572b9c"
     )
 
 
+def test_chia_vectors_2():
+    msg1 = bytes([1, 2, 3, 40])
+    msg2 = bytes([5, 6, 70, 201])
+    msg3 = bytes([9, 10, 11, 12, 13])
+    msg4 = bytes([15, 63, 244, 92, 0, 1])
+
+    seed1 = bytes([0x02] * 32)
+    seed2 = bytes([0x03] * 32)
+
+    sk1 = AugSchemeMPL.key_gen(seed1)
+    sk2 = AugSchemeMPL.key_gen(seed2)
+
+    pk1 = sk1.get_g1()
+    pk2 = sk2.get_g1()
+
+    sig1 = AugSchemeMPL.sign(sk1, msg1)
+    sig2 = AugSchemeMPL.sign(sk2, msg2)
+    sig3 = AugSchemeMPL.sign(sk2, msg1)
+    sig4 = AugSchemeMPL.sign(sk1, msg3)
+    sig5 = AugSchemeMPL.sign(sk1, msg1)
+    sig6 = AugSchemeMPL.sign(sk1, msg4)
+
+    agg_sig_l = AugSchemeMPL.aggregate([sig1, sig2])
+    agg_sig_r = AugSchemeMPL.aggregate([sig3, sig4, sig5])
+    agg_sig = AugSchemeMPL.aggregate([agg_sig_l, agg_sig_r, sig6])
+
+    assert AugSchemeMPL.aggregate_verify(
+        [pk1, pk2, pk2, pk1, pk1, pk1], [msg1, msg2, msg1, msg3, msg1, msg4], agg_sig
+    )
+
+    assert bytes(agg_sig).hex() == (
+        "a1d5360dcb418d33b29b90b912b4accde535cf0e52caf467a005dc632d9f7af44b6c4e9acd4"
+        "6eac218b28cdb07a3e3bc087df1cd1e3213aa4e11322a3ff3847bbba0b2fd19ddc25ca964871"
+        "997b9bceeab37a4c2565876da19382ea32a962200"
+    )
+
+
 def test_chia_vectors_3():
     seed1: bytes = bytes([0x04] * 32)
     sk1 = PopSchemeMPL.key_gen(seed1)
     proof = PopSchemeMPL.pop_prove(sk1)
     assert (
         bytes(proof).hex()
         == "84f709159435f0dc73b3e8bf6c78d85282d19231555a8ee3b6e2573aaf66872d9203fefa1ef"
@@ -615,11 +652,12 @@
 test_fields()
 test_ec()
 test_xmd()
 test_swu()
 test_edge_case_sign_Fq2()
 test_elements()
 test_chia_vectors_1()
+test_chia_vectors_2()
 test_chia_vectors_3()
 test_pyecc_vectors()
 test_vectors_invalid()
 test_readme()
```

### Comparing `blspy-1.0.9/python-impl/op_swu_g2.py` & `blspy-2.0.0b1/python-impl/op_swu_g2.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from bls12381 import h_eff, q
 from ec import JacobianPoint, default_ec_twist, eval_iso
 from fields import Fq, Fq2, roots_of_unity
 from hash_to_field import Hp2
+from typing import Optional
 
 
 def sgn0(x: Fq2) -> int:
     # https://tools.ietf.org/html/draft-irtf-cfrg-hash-to-curve-07#section-4.1
 
     sign_0: int = x[0].value % 2
     zero_0: bool = x[0] == 0
@@ -194,15 +195,15 @@
 def iso3(P):
     return eval_iso(P, (xnum, xden, ynum, yden), default_ec_twist)
 
 
 #
 # map from Fq2 element(s) to point in G2 subgroup of Ell2
 #
-def opt_swu2_map(t: Fq2, t2: Fq2 = None) -> JacobianPoint:
+def opt_swu2_map(t: Fq2, t2: Optional[Fq2] = None) -> JacobianPoint:
     Pp = iso3(osswu2_help(t))
     if t2 is not None:
         Pp2 = iso3(osswu2_help(t2))
         Pp = Pp + Pp2
     return Pp * h_eff
```

### Comparing `blspy-1.0.9/python-impl/pairing.py` & `blspy-2.0.0b1/python-impl/pairing.py`

 * *Files identical despite different names*

### Comparing `blspy-1.0.9/python-impl/private_key.py` & `blspy-2.0.0b1/python-impl/private_key.py`

 * *Files identical despite different names*

### Comparing `blspy-1.0.9/python-impl/schemes.py` & `blspy-2.0.0b1/python-impl/schemes.py`

 * *Files identical despite different names*

### Comparing `blspy-1.0.9/python-impl/util.py` & `blspy-2.0.0b1/python-impl/util.py`

 * *Files identical despite different names*

### Comparing `blspy-1.0.9/setup.py` & `blspy-2.0.0b1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -93,29 +93,28 @@
         "blspy",
         [
             "src/elements.cpp",
             "src/schemes.cpp",
             "src/privatekey.cpp",
             "src/bls.cpp",
             "python-bindings/pythonbindings.cpp",
+            "blst/src/server.c",
         ],
         include_dirs=[
             # Path to pybind11 headers
             get_pybind_include(),
             get_pybind_include(user=True),
-            "relic_ietf_64/include",
-            "mpir_gc_x64",
+            "blst",
             "libsodium/include",
         ],
         library_dirs=[
-            "relic_ietf_64",
-            "mpir_gc_x64",
             "libsodium/x64/Release/v142/static",
+            "src",
         ],
-        libraries=["relic_s", "Advapi32", "mpir", "libsodium"],
+        libraries=["Advapi32", "libsodium", "blstasm"],
         language="c++",
     ),
 ]
 
 
 # As of Python 3.6, CCompiler has a `has_flag` method.
 # cf http://bugs.python.org/issue26689
@@ -148,15 +147,15 @@
     raise RuntimeError("Unsupported compiler -- at least C++11 support " "is needed!")
 
 
 class BuildExt(build_ext):
     """A custom build extension for adding compiler-specific options."""
 
     c_opts = {
-        "msvc": ["/EHsc", "/std:c++17", "/DBLSALLOC_SODIUM=1", "/DSODIUM_STATIC"],
+        "msvc": ["/EHsc", "/std:c++17", "/DBLSALLOC_SODIUM=1", "/DSODIUM_STATIC", "/D__BLST_PORTABLE__"],
         "unix": [],
     }
     l_opts = {
         "msvc": [],
         "unix": [],
     }
 
@@ -192,16 +191,16 @@
         author="Mariano Sorgente",
         author_email="mariano@chia.net",
         description="BLS signatures in c++ (with python bindings)",
         long_description=open("README.md").read(),
         long_description_content_type="text/markdown",
         url="https://github.com/Chia-Network/bls-signatures",
         python_requires=">=3.7",
-        setup_requires=["pybind11>=2.5.0"],
-        install_requires=["pybind11>=2.5.0"],
+        setup_requires=["pybind11>=2.10.0"],
+        install_requires=["pybind11>=2.10.0"],
         ext_modules=ext_modules,
         cmdclass={"build_ext": BuildExt},
         zip_safe=False,
     )
 else:
     setup(
         name="blspy",
```

### Comparing `blspy-1.0.9/src/bls.hpp` & `blspy-2.0.0b1/src/bls.hpp`

 * *Files 4% similar despite different names*

```diff
@@ -32,13 +32,11 @@
  public:
     static const size_t MESSAGE_HASH_LEN = 32;
 
     // Initializes the BLS library (called automatically)
     static bool Init();
 
     static void SetSecureAllocator(Util::SecureAllocCallback allocCb, Util::SecureFreeCallback freeCb);
-
-    static void CheckRelicErrors();
 };
 } // end namespace bls
 
 #endif  // SRC_BLS_HPP_
```

### Comparing `blspy-1.0.9/src/elements.cpp` & `blspy-2.0.0b1/src/elements.cpp`

 * *Files 14% similar despite different names*

```diff
@@ -8,461 +8,487 @@
 
 // Unless required by applicable law or agreed to in writing, software
 // distributed under the License is distributed on an "AS IS" BASIS,
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.
 
+#include <string.h>
+
 #include <cstring>
 
 #include "bls.hpp"
 
 namespace bls {
 
 const size_t G1Element::SIZE;
 
-G1Element G1Element::FromBytes(const Bytes& bytes)
+G1Element G1Element::FromBytes(Bytes const bytes)
+{
+    G1Element ele = G1Element::FromBytesUnchecked(bytes);
+    ele.CheckValid();
+    return ele;
+}
+
+G1Element G1Element::FromBytesUnchecked(Bytes const bytes)
 {
     if (bytes.size() != SIZE) {
         throw std::invalid_argument("G1Element::FromBytes: Invalid size");
     }
 
-    G1Element ele;
-
-    // convert bytes to relic form
-    uint8_t buffer[G1Element::SIZE + 1];
-    std::memcpy(buffer + 1, bytes.begin(), G1Element::SIZE);
-    buffer[0] = 0x00;
-    buffer[1] &= 0x1f;  // erase 3 msbs from given input
-
-    bool fZerosOnly = Util::HasOnlyZeros(Bytes(buffer, G1Element::SIZE + 1));
+    // check if the element is canonical
+    const uint8_t* raw_bytes = bytes.begin();
+    bool fZerosOnly =
+        Util::HasOnlyZeros(Bytes(raw_bytes + 1, bytes.size() - 1));
     if ((bytes[0] & 0xc0) == 0xc0) {  // representing infinity
         // enforce that infinity must be 0xc0000..00
         if (bytes[0] != 0xc0 || !fZerosOnly) {
-            throw std::invalid_argument("Given G1 infinity element must be canonical");
+            throw std::invalid_argument(
+                "Given G1 infinity element must be canonical");
         }
-        return ele;
+        return G1Element();  // return infinity element (point all zero)
     } else {
         if ((bytes[0] & 0xc0) != 0x80) {
             throw std::invalid_argument(
                 "Given G1 non-infinity element must start with 0b10");
         }
 
         if (fZerosOnly) {
-            throw std::invalid_argument("G1 non-infinity element can't have only zeros");
-        }
-
-        if (bytes[0] & 0x20) {  // sign bit
-            buffer[0] = 0x03;
-        } else {
-            buffer[0] = 0x02;
+            throw std::invalid_argument(
+                "G1 non-infinity element can't have only zeros");
         }
     }
-    g1_read_bin(ele.p, buffer, G1Element::SIZE + 1);
-    BLS::CheckRelicErrors();
-    ele.CheckValid();
-    return ele;
+
+    blst_p1_affine a;
+    BLST_ERROR err = blst_p1_uncompress(&a, bytes.begin());
+    if (err != BLST_SUCCESS)
+        throw std::invalid_argument("G1Element::FromBytes: Invalid bytes");
+
+    return G1Element::FromAffine(a);
 }
 
 G1Element G1Element::FromByteVector(const std::vector<uint8_t>& bytevec)
 {
     return G1Element::FromBytes(Bytes(bytevec));
 }
 
-G1Element G1Element::FromNative(const g1_t element)
+G1Element G1Element::FromNative(const blst_p1& element)
 {
     G1Element ele;
-    g1_copy(ele.p, element);
-    ele.CheckValid();
+    memcpy(&(ele.p), &element, sizeof(blst_p1));
     return ele;
 }
 
-G1Element G1Element::FromMessage(const std::vector<uint8_t>& message,
-                                 const uint8_t* dst,
-                                 int dst_len)
+G1Element G1Element::FromAffine(const blst_p1_affine& element)
+{
+    G1Element ele;
+    blst_p1_from_affine(&(ele.p), &element);
+    return ele;
+}
+
+G1Element G1Element::FromMessage(
+    const std::vector<uint8_t>& message,
+    const uint8_t* dst,
+    int dst_len)
 {
     return FromMessage(Bytes(message), dst, dst_len);
 }
 
-G1Element G1Element::FromMessage(const Bytes& message,
-                                 const uint8_t* dst,
-                                 int dst_len)
+G1Element G1Element::FromMessage(
+    Bytes const message,
+    const uint8_t* dst,
+    int dst_len)
 {
     G1Element ans;
-    ep_map_dst(ans.p, message.begin(), (int)message.size(), dst, dst_len);
-    BLS::CheckRelicErrors();
+    const byte* aug = nullptr;
+    size_t aug_len = 0;
+
+    blst_hash_to_g1(
+        &(ans.p),
+        message.begin(),
+        (int)message.size(),
+        dst,
+        dst_len,
+        aug,
+        aug_len);
+
     assert(ans.IsValid());
     return ans;
 }
 
 G1Element G1Element::Generator()
 {
     G1Element ele;
-    g1_get_gen(ele.p);
-    BLS::CheckRelicErrors();
+    ele.p = *(blst_p1_generator());
     return ele;
 }
 
-bool G1Element::IsValid() const {
+bool G1Element::IsValid() const
+{
     // Infinity no longer valid in Relic
     // https://github.com/relic-toolkit/relic/commit/f3be2babb955cf9f82743e0ae5ef265d3da6c02b
-    if (g1_is_infty((g1_st*)p) == 1)
+    // if (blst_p1_is_inf(&p) == 1)
+    //     return true;
+
+    // return blst_p1_on_curve((blst_p1*)&p);
+
+    if (blst_p1_is_inf(&p))
         return true;
 
-    return g1_is_valid((g1_st*)p);
+    return blst_p1_in_g1(&p);
 }
 
-void G1Element::CheckValid() const {
+void G1Element::CheckValid() const
+{
     if (!IsValid())
         throw std::invalid_argument("G1 element is invalid");
-    BLS::CheckRelicErrors();
 }
 
-void G1Element::ToNative(g1_t output) const {
-    g1_copy(output, p);
+void G1Element::ToNative(blst_p1* output) const
+{
+    memcpy(output, &p, sizeof(blst_p1));
+}
+
+void G1Element::ToAffine(blst_p1_affine* output) const
+{
+    blst_p1_to_affine(output, &p);
 }
 
 G1Element G1Element::Negate() const
 {
     G1Element ans;
-    g1_neg(ans.p, p);
-    BLS::CheckRelicErrors();
+    ans.FromNative(p);
+    blst_p1_cneg(&(ans.p), true);
     return ans;
 }
 
 GTElement G1Element::Pair(const G2Element& b) const { return (*this) & b; }
 
 uint32_t G1Element::GetFingerprint() const
 {
     uint8_t buffer[G1Element::SIZE];
     uint8_t hash[32];
     memcpy(buffer, Serialize().data(), G1Element::SIZE);
     Util::Hash256(hash, buffer, G1Element::SIZE);
     return Util::FourBytesToInt(hash);
 }
 
-std::vector<uint8_t> G1Element::Serialize() const {
-    uint8_t buffer[G1Element::SIZE + 1];
-    g1_write_bin(buffer, G1Element::SIZE + 1, p, 1);
-
-    if (buffer[0] == 0x00) {  // infinity
-        std::vector<uint8_t> result(G1Element::SIZE, 0);
-        result[0] = 0xc0;
-        return result;
-    }
-
-    if (buffer[0] == 0x03) {  // sign bit set
-        buffer[1] |= 0x20;
-    }
-
-    buffer[1] |= 0x80;  // indicate compression
-    return std::vector<uint8_t>(buffer + 1, buffer + 1 + G1Element::SIZE);
+std::vector<uint8_t> G1Element::Serialize() const
+{
+    uint8_t buffer[G1Element::SIZE];
+    blst_p1_compress(buffer, &p);
+    return std::vector<uint8_t>(buffer, buffer + G1Element::SIZE);
 }
 
-bool operator==(const G1Element & a, const G1Element &b)
+bool operator==(const G1Element& a, const G1Element& b)
 {
-    return g1_cmp(a.p, b.p) == RLC_EQ;
+    return blst_p1_is_equal(&(a.p), &(b.p));
 }
 
-bool operator!=(const G1Element & a, const G1Element & b) { return !(a == b); }
+bool operator!=(const G1Element& a, const G1Element& b) { return !(a == b); }
 
-std::ostream& operator<<(std::ostream& os, const G1Element &ele)
+std::ostream& operator<<(std::ostream& os, const G1Element& ele)
 {
     return os << Util::HexStr(ele.Serialize());
 }
 
 G1Element& operator+=(G1Element& a, const G1Element& b)
 {
-    g1_add(a.p, a.p, b.p);
-    BLS::CheckRelicErrors();
+    blst_p1_add(&(a.p), &(a.p), &(b.p));
     return a;
 }
 
 G1Element operator+(const G1Element& a, const G1Element& b)
 {
     G1Element ans;
-    g1_add(ans.p, a.p, b.p);
-    BLS::CheckRelicErrors();
+    blst_p1_add(&(ans.p), &(a.p), &(b.p));
     return ans;
 }
 
-G1Element operator*(const G1Element& a, const bn_t& k)
+G1Element operator*(const G1Element& a, const blst_scalar& k)
 {
     G1Element ans;
-    g1_mul(ans.p, (g1_st*)a.p, (bn_st*)k);
-    BLS::CheckRelicErrors();
+    byte* bte = Util::SecAlloc<byte>(32);
+    blst_bendian_from_scalar(bte, &k);
+    blst_p1_mult(&(ans.p), &(a.p), bte, 256);
+    Util::SecFree(bte);
+
     return ans;
 }
 
-G1Element operator*(const bn_t& k, const G1Element& a) { return a * k; }
-
-
+G1Element operator*(const blst_scalar& k, const G1Element& a) { return a * k; }
 
 // G2Element definitions below
 
-
-
 const size_t G2Element::SIZE;
 
-G2Element G2Element::FromBytes(const Bytes& bytes)
+G2Element G2Element::FromBytes(Bytes const bytes)
+{
+    G2Element ele = G2Element::FromBytesUnchecked(bytes);
+    ele.CheckValid();
+    return ele;
+}
+
+G2Element G2Element::FromBytesUnchecked(Bytes const bytes)
 {
     if (bytes.size() != SIZE) {
         throw std::invalid_argument("G2Element::FromBytes: Invalid size");
     }
 
-    G2Element ele;
-    uint8_t buffer[G2Element::SIZE + 1];
-    std::memcpy(buffer + 1, bytes.begin() + G2Element::SIZE / 2, G2Element::SIZE / 2);
-    std::memcpy(buffer + 1 + G2Element::SIZE / 2, bytes.begin(), G2Element::SIZE / 2);
-    buffer[0] = 0x00;
-    buffer[49] &= 0x1f;  // erase 3 msbs from input
-
-    if ((bytes[48] & 0xe0) != 0x00) {
-        throw std::invalid_argument(
-            "Given G2 element must always have 48th byte start with 0b000");
-    }
-    bool fZerosOnly = Util::HasOnlyZeros(Bytes(buffer, G2Element::SIZE + 1));
-    if (((bytes[0] & 0xc0) == 0xc0)) {  // infinity
-        // enforce that infinity must be 0xc0000..00
-        if (bytes[0] != 0xc0 || !fZerosOnly) {
-            throw std::invalid_argument(
-                "Given G2 infinity element must be canonical");
-        }
-        return ele;
-    } else {
-        if (((bytes[0] & 0xc0) != 0x80)) {
-            throw std::invalid_argument(
-                "G2 non-inf element must have 0th byte start with 0b10");
-        }
-
-        if (fZerosOnly) {
-            throw std::invalid_argument("G2 non-infinity element can't have only zeros");
-        }
-
-        if (bytes[0] & 0x20) {
-            buffer[0] = 0x03;
-        } else {
-            buffer[0] = 0x02;
-        }
-    }
+    blst_p2_affine a;
+    BLST_ERROR err = blst_p2_uncompress(&a, bytes.begin());
+    if (err != BLST_SUCCESS)
+        throw std::invalid_argument("G2Element::FromBytes: Invalid bytes");
 
-    g2_read_bin(ele.q, buffer, G2Element::SIZE + 1);
-    BLS::CheckRelicErrors();
-    ele.CheckValid();
-    return ele;
+    return G2Element::FromAffine(a);
 }
 
 G2Element G2Element::FromByteVector(const std::vector<uint8_t>& bytevec)
 {
     return G2Element::FromBytes(Bytes(bytevec));
 }
 
-G2Element G2Element::FromNative(const g2_t element)
+G2Element G2Element::FromNative(const blst_p2& element)
 {
     G2Element ele;
-    g2_copy(ele.q, (g2_st*)element);
-    ele.CheckValid();
+    memcpy(&(ele.q), &element, sizeof(blst_p2));
     return ele;
 }
 
-G2Element G2Element::FromMessage(const std::vector<uint8_t>& message,
-                                 const uint8_t* dst,
-                                 int dst_len)
+G2Element G2Element::FromAffine(const blst_p2_affine& element)
+{
+    G2Element ele;
+    blst_p2_from_affine(&(ele.q), &element);
+    return ele;
+}
+
+G2Element G2Element::FromMessage(
+    const std::vector<uint8_t>& message,
+    const uint8_t* dst,
+    int dst_len)
 {
     return FromMessage(Bytes(message), dst, dst_len);
 }
 
-G2Element G2Element::FromMessage(const Bytes& message,
-                                 const uint8_t* dst,
-                                 int dst_len)
+G2Element G2Element::FromMessage(
+    Bytes const message,
+    const uint8_t* dst,
+    int dst_len)
 {
     G2Element ans;
-    ep2_map_dst(ans.q, message.begin(), (int)message.size(), dst, dst_len);
-    BLS::CheckRelicErrors();
+    const byte* aug = nullptr;
+    size_t aug_len = 0;
+
+    blst_hash_to_g2(
+        &(ans.q),
+        message.begin(),
+        (int)message.size(),
+        dst,
+        dst_len,
+        aug,
+        aug_len);
+
     assert(ans.IsValid());
     return ans;
 }
 
 G2Element G2Element::Generator()
 {
     G2Element ele;
-    g2_get_gen(ele.q);
-    BLS::CheckRelicErrors();
+    ele.q = (*blst_p2_generator());
     return ele;
 }
 
-bool G2Element::IsValid() const {
+bool G2Element::IsValid() const
+{
     // Infinity no longer valid in Relic
     // https://github.com/relic-toolkit/relic/commit/f3be2babb955cf9f82743e0ae5ef265d3da6c02b
-    if (g2_is_infty((g2_st*)q) == 1)
+    // if (blst_p2_is_inf(&q) == 1)
+    //     return true;
+
+    // return blst_p2_on_curve((blst_p2*)&q);
+
+    if (blst_p2_is_inf(&q))
         return true;
 
-    return g2_is_valid((g2_st*)q);
+    return blst_p2_in_g2(&q);
 }
 
-void G2Element::CheckValid() const {
+void G2Element::CheckValid() const
+{
     if (!IsValid())
         throw std::invalid_argument("G2 element is invalid");
-    BLS::CheckRelicErrors();
 }
 
-void G2Element::ToNative(g2_t output) const {
-    g2_copy(output, (g2_st*)q);
+void G2Element::ToNative(blst_p2* output) const
+{
+    memcpy(output, (blst_p2*)&q, sizeof(blst_p2));
+}
+
+void G2Element::ToAffine(blst_p2_affine* output) const
+{
+    blst_p2_to_affine(output, &q);
 }
 
 G2Element G2Element::Negate() const
 {
     G2Element ans;
-    g2_neg(ans.q, (g2_st*)q);
-    BLS::CheckRelicErrors();
+    ans.FromNative(q);
+    blst_p2_cneg(&(ans.q), true);
     return ans;
 }
 
 GTElement G2Element::Pair(const G1Element& a) const { return a & (*this); }
 
-std::vector<uint8_t> G2Element::Serialize() const {
-    uint8_t buffer[G2Element::SIZE + 1];
-    g2_write_bin(buffer, G2Element::SIZE + 1, (g2_st*)q, 1);
-
-    if (buffer[0] == 0x00) {  // infinity
-        std::vector<uint8_t> result(G2Element::SIZE, 0);
-        result[0] = 0xc0;
-        return result;
-    }
-
-    // remove leading 3 bits
-    buffer[1] &= 0x1f;
-    buffer[49] &= 0x1f;
-    if (buffer[0] == 0x03) {
-        buffer[49] |= 0xa0;  // swapped later to 0
-    } else {
-        buffer[49] |= 0x80;
-    }
-
-    // Swap buffer, relic uses the opposite ordering for Fq2 elements
-    std::vector<uint8_t> result(G2Element::SIZE, 0);
-    std::memcpy(result.data(), buffer + 1 + G2Element::SIZE / 2, G2Element::SIZE / 2);
-    std::memcpy(result.data() + G2Element::SIZE / 2, buffer + 1, G2Element::SIZE / 2);
-    return result;
+std::vector<uint8_t> G2Element::Serialize() const
+{
+    uint8_t buffer[G2Element::SIZE];
+    blst_p2_compress(buffer, &q);
+    return std::vector<uint8_t>(buffer, buffer + G2Element::SIZE);
 }
 
 bool operator==(G2Element const& a, G2Element const& b)
 {
-    return g2_cmp((g2_st*)a.q, (g2_st*)b.q) == RLC_EQ;
+    return blst_p2_is_equal(&(a.q), &(b.q));
 }
 
 bool operator!=(G2Element const& a, G2Element const& b) { return !(a == b); }
 
-std::ostream& operator<<(std::ostream& os, const G2Element & s)
+std::ostream& operator<<(std::ostream& os, const G2Element& s)
 {
     return os << Util::HexStr(s.Serialize());
 }
 
 G2Element& operator+=(G2Element& a, const G2Element& b)
 {
-    g2_add(a.q, a.q, (g2_st*)b.q);
-    BLS::CheckRelicErrors();
+    blst_p2_add(&(a.q), &(a.q), &(b.q));
     return a;
 }
 
 G2Element operator+(const G2Element& a, const G2Element& b)
 {
     G2Element ans;
-    g2_add(ans.q, (g2_st*)a.q, (g2_st*)b.q);
-    BLS::CheckRelicErrors();
+    blst_p2_add(&(ans.q), &(a.q), &(b.q));
     return ans;
 }
 
-G2Element operator*(const G2Element& a, const bn_t& k)
+G2Element operator*(const G2Element& a, const blst_scalar& k)
 {
     G2Element ans;
-    g2_mul(ans.q, (g2_st*)a.q, (bn_st*)k);
-    BLS::CheckRelicErrors();
+    byte* bte = Util::SecAlloc<byte>(32);
+    blst_bendian_from_scalar(bte, &k);
+    blst_p2_mult(&(ans.q), &(a.q), bte, 256);
+    Util::SecFree(bte);
+
     return ans;
 }
 
-G2Element operator*(const bn_t& k, const G2Element& a) { return a * k; }
-
-
+G2Element operator*(const blst_scalar& k, const G2Element& a) { return a * k; }
 
 // GTElement
 
 const size_t GTElement::SIZE;
 
-GTElement GTElement::FromBytes(const Bytes& bytes)
+/*
+ * Currently deserliazation is not available - these are currently
+ * broken and just return the zero element
+ */
+GTElement GTElement::FromBytes(Bytes const bytes)
+{
+    GTElement ele = GTElement::FromBytesUnchecked(bytes);
+    //
+    // this doesn't seem to be the proper check as it doesn't work as expeced
+    //
+    // if (!blst_fp12_in_group(&(ele.r)))
+    //     throw std::invalid_argument("GTElement is invalid");
+    return ele;
+}
+
+GTElement GTElement::FromBytesUnchecked(Bytes const bytes)
 {
     if (bytes.size() != SIZE) {
         throw std::invalid_argument("GTElement::FromBytes: Invalid size");
     }
     GTElement ele = GTElement();
-    gt_read_bin(ele.r, bytes.begin(), GTElement::SIZE);
-    if (gt_is_valid(*(gt_t*)&ele) == 0)
-        throw std::invalid_argument("GTElement is invalid");
-    BLS::CheckRelicErrors();
+    // TO DO  blst_fp12_from_bendian(&(ele.r), bytes.begin());
     return ele;
 }
 
 GTElement GTElement::FromByteVector(const std::vector<uint8_t>& bytevec)
 {
     return GTElement::FromBytes(Bytes(bytevec));
 }
 
-GTElement GTElement::FromNative(const gt_t* element)
+GTElement GTElement::FromNative(const blst_fp12* element)
 {
     GTElement ele = GTElement();
-    gt_copy(ele.r, *(gt_t*)element);
+    ele.r = *element;
     return ele;
 }
 
-GTElement GTElement::Unity() {
+GTElement GTElement::FromAffine(const blst_p1_affine& affine)
+{
     GTElement ele = GTElement();
-    gt_set_unity(ele.r);
+    blst_aggregated_in_g1(&ele.r, &affine);
     return ele;
 }
 
+GTElement GTElement::FromAffine(const blst_p2_affine& affine)
+{
+    GTElement ele = GTElement();
+    blst_aggregated_in_g2(&ele.r, &affine);
+    return ele;
+}
+
+GTElement GTElement::Unity()
+{
+    GTElement ele = GTElement();
+    ele.FromNative(blst_fp12_one());
+    return ele;
+}
 
 bool operator==(GTElement const& a, GTElement const& b)
 {
-    return gt_cmp(*(gt_t*)(a.r), *(gt_t*)(b.r)) == RLC_EQ;
+    return blst_fp12_is_equal(&(a.r), &(b.r));
 }
 
 bool operator!=(GTElement const& a, GTElement const& b) { return !(a == b); }
 
 std::ostream& operator<<(std::ostream& os, GTElement const& ele)
 {
     return os << Util::HexStr(ele.Serialize());
 }
 
 GTElement operator&(const G1Element& a, const G2Element& b)
 {
-    G1Element nonConstA(a);
-    gt_t ans;
-    gt_new(ans);
-    g2_t tmp;
-    g2_null(tmp);
-    g2_new(tmp);
-    b.ToNative(tmp);
-    pp_map_oatep_k12(ans, nonConstA.p, tmp);
+    blst_fp12 ans;
+
+    blst_p1_affine aff1;
+    blst_p2_affine aff2;
+    a.ToAffine(&aff1);
+    b.ToAffine(&aff2);
+
+    blst_miller_loop(&ans, &aff2, &aff1);
+    blst_final_exp(&ans, &ans);
+
     GTElement ret = GTElement::FromNative(&ans);
-    gt_free(ans);
-    g2_free(tmp);
+
     return ret;
 }
 
 GTElement operator*(GTElement& a, GTElement& b)
 {
     GTElement ans;
-    fp12_mul(ans.r, a.r, b.r);
-    BLS::CheckRelicErrors();
+    blst_fp12_mul(&(ans.r), &(a.r), &(b.r));
     return ans;
 }
 
 void GTElement::Serialize(uint8_t* buffer) const
 {
-    gt_write_bin(buffer, GTElement::SIZE, *(gt_t*)&r, 1);
+    blst_bendian_from_fp12(buffer, &r);
 }
 
 std::vector<uint8_t> GTElement::Serialize() const
 {
     std::vector<uint8_t> data(GTElement::SIZE);
     Serialize(data.data());
     return data;
```

### Comparing `blspy-1.0.9/src/elements.hpp` & `blspy-2.0.0b1/src/elements.hpp`

 * *Files 18% similar despite different names*

```diff
@@ -12,17 +12,16 @@
 // See the License for the specific language governing permissions and
 // limitations under the License.
 
 #ifndef SRC_BLSELEMENTS_HPP_
 #define SRC_BLSELEMENTS_HPP_
 
 extern "C" {
-#include "relic.h"
+#include "bindings/blst.h"
 }
-#include "relic_conf.h"
 #include "util.hpp"
 
 #if defined GMP && ARITH == GMP
 #include <gmp.h>
 #endif
 
 #include <utility>
@@ -32,106 +31,115 @@
 class G2Element;
 class GTElement;
 
 class G1Element {
 public:
     static const size_t SIZE = 48;
 
-    G1Element() {
-        g1_set_infty(p);
-    }
+    G1Element() { memset(&p, 0x00, sizeof(blst_p1)); }
 
-    static G1Element FromBytes(const Bytes& bytes);
+    static G1Element FromBytes(Bytes bytes);
+    static G1Element FromBytesUnchecked(Bytes bytes);
     static G1Element FromByteVector(const std::vector<uint8_t> &bytevec);
-    static G1Element FromNative(const g1_t element);
-    static G1Element FromMessage(const std::vector<uint8_t> &message,
-                                 const uint8_t *dst,
-                                 int dst_len);
-    static G1Element FromMessage(const Bytes& message,
-                                 const uint8_t* dst,
-                                 int dst_len);
+    static G1Element FromNative(const blst_p1 &element);
+    static G1Element FromAffine(const blst_p1_affine &element);
+    static G1Element FromMessage(
+        const std::vector<uint8_t> &message,
+        const uint8_t *dst,
+        int dst_len);
+    static G1Element FromMessage(
+        Bytes message,
+        const uint8_t *dst,
+        int dst_len);
     static G1Element Generator();
 
     bool IsValid() const;
     void CheckValid() const;
-    void ToNative(g1_t output) const;
+    void ToNative(blst_p1 *output) const;
+    void ToAffine(blst_p1_affine *output) const;
     G1Element Negate() const;
     GTElement Pair(const G2Element &b) const;
     uint32_t GetFingerprint() const;
     std::vector<uint8_t> Serialize() const;
 
     friend bool operator==(const G1Element &a, const G1Element &b);
     friend bool operator!=(const G1Element &a, const G1Element &b);
     friend std::ostream &operator<<(std::ostream &os, const G1Element &s);
-    friend G1Element& operator+=(G1Element& a, const G1Element& b);
+    friend G1Element &operator+=(G1Element &a, const G1Element &b);
     friend G1Element operator+(const G1Element &a, const G1Element &b);
-    friend G1Element operator*(const G1Element &a, const bn_t &k);
-    friend G1Element operator*(const bn_t &k, const G1Element &a);
+    friend G1Element operator*(const G1Element &a, const blst_scalar &k);
+    friend G1Element operator*(const blst_scalar &k, const G1Element &a);
     friend GTElement operator&(const G1Element &a, const G2Element &b);
 
 private:
-    g1_t p;
+    blst_p1 p;
 };
 
 class G2Element {
 public:
     static const size_t SIZE = 96;
 
-    G2Element() {
-        g2_set_infty(q);
-    }
+    G2Element() { memset(&q, 0x00, sizeof(blst_p2)); }
 
-    static G2Element FromBytes(const Bytes& bytes);
+    static G2Element FromBytes(Bytes bytes);
+    static G2Element FromBytesUnchecked(Bytes bytes);
     static G2Element FromByteVector(const std::vector<uint8_t> &bytevec);
-    static G2Element FromNative(const g2_t element);
-    static G2Element FromMessage(const std::vector<uint8_t>& message,
-                                 const uint8_t* dst,
-                                 int dst_len);
-    static G2Element FromMessage(const Bytes& message,
-                                 const uint8_t* dst,
-                                 int dst_len);
+    static G2Element FromNative(const blst_p2 &element);
+    static G2Element FromAffine(const blst_p2_affine &element);
+    static G2Element FromMessage(
+        const std::vector<uint8_t> &message,
+        const uint8_t *dst,
+        int dst_len);
+    static G2Element FromMessage(
+        Bytes message,
+        const uint8_t *dst,
+        int dst_len);
     static G2Element Generator();
 
     bool IsValid() const;
     void CheckValid() const;
-    void ToNative(g2_t output) const;
+    void ToNative(blst_p2 *output) const;
+    void ToAffine(blst_p2_affine *output) const;
     G2Element Negate() const;
     GTElement Pair(const G1Element &a) const;
     std::vector<uint8_t> Serialize() const;
 
     friend bool operator==(G2Element const &a, G2Element const &b);
     friend bool operator!=(G2Element const &a, G2Element const &b);
     friend std::ostream &operator<<(std::ostream &os, const G2Element &s);
-    friend G2Element& operator+=(G2Element& a, const G2Element& b);
+    friend G2Element &operator+=(G2Element &a, const G2Element &b);
     friend G2Element operator+(const G2Element &a, const G2Element &b);
-    friend G2Element operator*(const G2Element &a, const bn_t &k);
-    friend G2Element operator*(const bn_t &k, const G2Element &a);
+    friend G2Element operator*(const G2Element &a, const blst_scalar &k);
+    friend G2Element operator*(const blst_scalar &k, const G2Element &a);
 
 private:
-    g2_t q;
+    blst_p2 q;
 };
 
 class GTElement {
 public:
-    static const size_t SIZE = 384;
-    static GTElement FromBytes(const Bytes& bytes);
+    static const size_t SIZE = 576;
+
+    static GTElement FromBytes(Bytes bytes);
+    static GTElement FromBytesUnchecked(Bytes bytes);
     static GTElement FromByteVector(const std::vector<uint8_t> &bytevec);
-    static GTElement FromNative(const gt_t *element);
+    static GTElement FromNative(const blst_fp12 *element);
+    static GTElement FromAffine(const blst_p1_affine &element);
+    static GTElement FromAffine(const blst_p2_affine &element);
     static GTElement Unity();  // unity
 
     void Serialize(uint8_t *buffer) const;
     std::vector<uint8_t> Serialize() const;
 
     friend bool operator==(GTElement const &a, GTElement const &b);
     friend bool operator!=(GTElement const &a, GTElement const &b);
     friend std::ostream &operator<<(std::ostream &os, const GTElement &s);
     friend GTElement operator*(GTElement &a, GTElement &b);
-    GTElement &operator=(const GTElement &rhs);
 
 private:
-    gt_t r;
+    blst_fp12 r;
     GTElement() {}
 };
 
 }  // end namespace bls
 
 #endif  // SRC_BLSELEMENTS_HPP_
```

### Comparing `blspy-1.0.9/src/hkdf.hpp` & `blspy-2.0.0b1/src/hkdf.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -11,21 +11,15 @@
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.
 
 #ifndef SRC_BLSHKDF_HPP_
 #define SRC_BLSHKDF_HPP_
 
-#include "relic_conf.h"
 #include <math.h>
-
-#if defined GMP && ARITH == GMP
-#include <gmp.h>
-#endif
-
 #include <cassert>
 #include "util.hpp"
 
 namespace bls {
 
 class HKDF256 {
     /**
@@ -36,15 +30,15 @@
     static const uint8_t HASH_LEN = 32;
 
     static void Extract(uint8_t* prk_output, const uint8_t* salt, const size_t saltLen, const uint8_t* ikm, const size_t ikm_len) {
         // assert(saltLen == 4);  // Used for EIP2333 key derivation
         // assert(ikm_len == 32);  // Used for EIP2333 key derivation
         // Hash256 used as the hash function (sha256)
         // PRK Output is 32 bytes (HashLen)
-        md_hmac(prk_output, ikm, ikm_len, salt, saltLen);
+        Util::md_hmac(prk_output, ikm, ikm_len, salt, saltLen);
     }
 
     static void Expand(uint8_t* okm, size_t L, const uint8_t* prk, const uint8_t* info, const size_t infoLen) {
         assert(L <= 255 * HASH_LEN); // L <= 255 * HashLen
         assert(infoLen >= 0);
         size_t N = (L + HASH_LEN - 1) / HASH_LEN; // Round up
         size_t bytesWritten = 0;
@@ -55,20 +49,20 @@
 
         assert(N >= 1 && N <= 255);
 
         for (size_t i = 1; i <= N; i++) {
             if (i == 1) {
                 memcpy(hmacInput1, info, infoLen);
                 hmacInput1[infoLen] = i;
-                md_hmac(T, hmacInput1, infoLen + 1, prk, HASH_LEN);
+                Util::md_hmac(T, hmacInput1, infoLen + 1, prk, HASH_LEN);
             } else {
                 memcpy(hmacInput, T, HASH_LEN);
                 memcpy(hmacInput + HASH_LEN, info, infoLen);
                 hmacInput[HASH_LEN + infoLen] = i;
-                md_hmac(T, hmacInput, HASH_LEN + infoLen + 1, prk, HASH_LEN);
+                Util::md_hmac(T, hmacInput, HASH_LEN + infoLen + 1, prk, HASH_LEN);
             }
             size_t to_write = L - bytesWritten;
             if (to_write > HASH_LEN) {
                 to_write = HASH_LEN;
             }
             assert (to_write > 0 && to_write <= HASH_LEN);
             memcpy(okm + bytesWritten, T, to_write);
```

### Comparing `blspy-1.0.9/src/privatekey.cpp` & `blspy-2.0.0b1/src/privatekey.cpp`

 * *Files 20% similar despite different names*

```diff
@@ -8,211 +8,221 @@
 
 // Unless required by applicable law or agreed to in writing, software
 // distributed under the License is distributed on an "AS IS" BASIS,
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.
 
+#include <string.h>
+
 #include "bls.hpp"
 
 namespace bls {
 
 const size_t PrivateKey::PRIVATE_KEY_SIZE;
 
 // Construct a private key from a bytearray.
-PrivateKey PrivateKey::FromBytes(const Bytes& bytes, bool modOrder)
+PrivateKey PrivateKey::FromBytes(const Bytes &bytes, bool modOrder)
 {
     if (bytes.size() != PRIVATE_KEY_SIZE) {
         throw std::invalid_argument("PrivateKey::FromBytes: Invalid size");
     }
 
     PrivateKey k;
-    bn_read_bin(k.keydata, bytes.begin(), PrivateKey::PRIVATE_KEY_SIZE);
-    bn_t ord;
-    bn_new(ord);
-    g1_get_ord(ord);
-    if (modOrder) {
-        bn_mod_basic(k.keydata, k.keydata, ord);
-    } else {
-        if (bn_cmp(k.keydata, ord) > 0) {
-            throw std::invalid_argument(
-                "PrivateKey byte data must be less than the group order");
-        }
+    if (modOrder)
+        // this allows any bytes to be input and does proper mod order
+        blst_scalar_from_be_bytes(k.keydata, bytes.begin(), bytes.size());
+    else
+        // this should only be the output of deserialization
+        blst_scalar_from_bendian(k.keydata, bytes.begin());
+
+    if (Util::HasOnlyZeros(bytes)) {
+        return k;  // don't check anything else, we allow zero private key
     }
+
+    if (!blst_sk_check(k.keydata))
+        throw std::invalid_argument(
+            "PrivateKey byte data must be less than the group order");
+
     return k;
 }
 
 // Construct a private key from a bytearray.
-PrivateKey PrivateKey::FromByteVector(const std::vector<uint8_t> bytes, bool modOrder)
+PrivateKey PrivateKey::FromByteVector(
+    const std::vector<uint8_t> bytes,
+    bool modOrder)
 {
     return PrivateKey::FromBytes(Bytes(bytes), modOrder);
 }
 
-PrivateKey::PrivateKey() {
-    AllocateKeyData();
-};
+PrivateKey::PrivateKey() { AllocateKeyData(); };
 
 // Construct a private key from another private key.
 PrivateKey::PrivateKey(const PrivateKey &privateKey)
 {
     privateKey.CheckKeyData();
     AllocateKeyData();
-    bn_copy(keydata, privateKey.keydata);
+    memcpy(keydata, privateKey.keydata, 32);
 }
 
 PrivateKey::PrivateKey(PrivateKey &&k)
     : keydata(std::exchange(k.keydata, nullptr))
 {
     k.InvalidateCaches();
 }
 
-PrivateKey::~PrivateKey()
-{
-    DeallocateKeyData();
-}
+PrivateKey::~PrivateKey() { DeallocateKeyData(); }
 
 void PrivateKey::DeallocateKeyData()
 {
-    if(keydata != nullptr) {
+    if (keydata != nullptr) {
         Util::SecFree(keydata);
         keydata = nullptr;
     }
     InvalidateCaches();
 }
 
 void PrivateKey::InvalidateCaches()
 {
     fG1CacheValid = false;
     fG2CacheValid = false;
 }
 
-PrivateKey& PrivateKey::operator=(const PrivateKey& other)
+PrivateKey &PrivateKey::operator=(const PrivateKey &other)
 {
     CheckKeyData();
     other.CheckKeyData();
     InvalidateCaches();
-    bn_copy(keydata, other.keydata);
+    memcpy(keydata, other.keydata, 32);
     return *this;
 }
 
-PrivateKey& PrivateKey::operator=(PrivateKey&& other)
+PrivateKey &PrivateKey::operator=(PrivateKey &&other)
 {
     DeallocateKeyData();
     keydata = std::exchange(other.keydata, nullptr);
     other.InvalidateCaches();
     return *this;
 }
 
-const G1Element& PrivateKey::GetG1Element() const
+const G1Element &PrivateKey::GetG1Element() const
 {
     if (!fG1CacheValid) {
         CheckKeyData();
-        g1_st *p = Util::SecAlloc<g1_st>(1);
-        g1_mul_gen(p, keydata);
+        blst_p1 *p = Util::SecAlloc<blst_p1>(1);
+        blst_sk_to_pk_in_g1(p, keydata);
 
-        g1Cache = G1Element::FromNative(p);
+        g1Cache = G1Element::FromNative(*p);
         Util::SecFree(p);
         fG1CacheValid = true;
     }
     return g1Cache;
 }
 
-const G2Element& PrivateKey::GetG2Element() const
+const G2Element &PrivateKey::GetG2Element() const
 {
     if (!fG2CacheValid) {
         CheckKeyData();
-        g2_st *q = Util::SecAlloc<g2_st>(1);
-        g2_mul_gen(q, keydata);
+        blst_p2 *q = Util::SecAlloc<blst_p2>(1);
+        blst_sk_to_pk_in_g2(q, keydata);
 
-        g2Cache = G2Element::FromNative(q);
+        g2Cache = G2Element::FromNative(*q);
         Util::SecFree(q);
         fG2CacheValid = true;
     }
     return g2Cache;
 }
 
 G1Element operator*(const G1Element &a, const PrivateKey &k)
 {
     k.CheckKeyData();
-    g1_st* ans = Util::SecAlloc<g1_st>(1);
+
+    blst_p1 *ans = Util::SecAlloc<blst_p1>(1);
     a.ToNative(ans);
-    g1_mul(ans, ans, k.keydata);
-    G1Element ret = G1Element::FromNative(ans);
+    byte *bte = Util::SecAlloc<byte>(32);
+    blst_bendian_from_scalar(bte, k.keydata);
+    blst_p1_mult(ans, ans, bte, 256);
+    G1Element ret = G1Element::FromNative(*ans);
     Util::SecFree(ans);
+    Util::SecFree(bte);
     return ret;
 }
 
 G1Element operator*(const PrivateKey &k, const G1Element &a) { return a * k; }
 
 G2Element operator*(const G2Element &a, const PrivateKey &k)
 {
     k.CheckKeyData();
-    g2_st* ans = Util::SecAlloc<g2_st>(1);
+    blst_p2 *ans = Util::SecAlloc<blst_p2>(1);
     a.ToNative(ans);
-    g2_mul(ans, ans, k.keydata);
-    G2Element ret = G2Element::FromNative(ans);
+    byte *bte = Util::SecAlloc<byte>(32);
+    blst_bendian_from_scalar(bte, k.keydata);
+    blst_p2_mult(ans, ans, bte, 256);
+    G2Element ret = G2Element::FromNative(*ans);
     Util::SecFree(ans);
+    Util::SecFree(bte);
     return ret;
 }
 
 G2Element operator*(const PrivateKey &k, const G2Element &a) { return a * k; }
 
-G2Element PrivateKey::GetG2Power(const G2Element& element) const
+G2Element PrivateKey::GetG2Power(const G2Element &element) const
 {
     CheckKeyData();
-    g2_st* q = Util::SecAlloc<g2_st>(1);
+    blst_p2 *q = Util::SecAlloc<blst_p2>(1);
     element.ToNative(q);
-    g2_mul(q, q, keydata);
-
-    const G2Element ret = G2Element::FromNative(q);
+    byte *bte = Util::SecAlloc<byte>(32);
+    blst_bendian_from_scalar(bte, keydata);
+    blst_p2_mult(q, q, bte, 255);
+    const G2Element ret = G2Element::FromNative(*q);
     Util::SecFree(q);
+    Util::SecFree(bte);
     return ret;
 }
 
 PrivateKey PrivateKey::Aggregate(std::vector<PrivateKey> const &privateKeys)
 {
     if (privateKeys.empty()) {
         throw std::length_error("Number of private keys must be at least 1");
     }
 
-    bn_t order;
-    bn_new(order);
-    g1_get_ord(order);
-
     PrivateKey ret;
     assert(ret.IsZero());
     for (size_t i = 0; i < privateKeys.size(); i++) {
         privateKeys[i].CheckKeyData();
-        bn_add(ret.keydata, ret.keydata, privateKeys[i].keydata);
-        bn_mod_basic(ret.keydata, ret.keydata, order);
+        blst_sk_add_n_check(ret.keydata, ret.keydata, privateKeys[i].keydata);
     }
     return ret;
 }
 
-bool PrivateKey::IsZero() const {
+bool PrivateKey::IsZero() const
+{
     CheckKeyData();
-    return bn_is_zero(keydata);
+    blst_scalar zro;
+    memset(&zro, 0x00, sizeof(blst_scalar));
+
+    return memcmp(keydata, &zro, 32) == 0;
 }
 
 bool operator==(const PrivateKey &a, const PrivateKey &b)
 {
     a.CheckKeyData();
     b.CheckKeyData();
-    return bn_cmp(a.keydata, b.keydata) == RLC_EQ;
+    return memcmp(a.keydata, b.keydata, sizeof(blst_scalar)) == 0;
 }
 
 bool operator!=(const PrivateKey &a, const PrivateKey &b) { return !(a == b); }
 
 void PrivateKey::Serialize(uint8_t *buffer) const
 {
     if (buffer == nullptr) {
         throw std::runtime_error("PrivateKey::Serialize buffer invalid");
     }
     CheckKeyData();
-    bn_write_bin(buffer, PrivateKey::PRIVATE_KEY_SIZE, keydata);
+    blst_bendian_from_scalar(buffer, keydata);
 }
 
 std::vector<uint8_t> PrivateKey::Serialize() const
 {
     std::vector<uint8_t> data(PRIVATE_KEY_SIZE);
     Serialize(data.data());
     return data;
@@ -222,32 +232,33 @@
     const uint8_t *msg,
     size_t len,
     const uint8_t *dst,
     size_t dst_len) const
 {
     CheckKeyData();
 
-    g2_st* pt = Util::SecAlloc<g2_st>(1);
+    blst_p2 *pt = Util::SecAlloc<blst_p2>(1);
+
+    blst_hash_to_g2(pt, msg, len, dst, dst_len, nullptr, 0);
+    blst_sign_pk_in_g1(pt, pt, keydata);
 
-    ep2_map_dst(pt, msg, len, dst, dst_len);
-    g2_mul(pt, pt, keydata);
-    G2Element ret = G2Element::FromNative(pt);
+    G2Element ret = G2Element::FromNative(*pt);
     Util::SecFree(pt);
     return ret;
 }
 
 void PrivateKey::AllocateKeyData()
 {
     assert(!keydata);
-    keydata = Util::SecAlloc<bn_st>(1);
-    keydata->alloc = RLC_BN_SIZE;
-    bn_zero(keydata);
+    keydata = Util::SecAlloc<blst_scalar>(1);
+    memset(keydata, 0x00, sizeof(blst_scalar));
 }
 
 void PrivateKey::CheckKeyData() const
 {
     if (keydata == nullptr) {
-        throw std::runtime_error("PrivateKey::CheckKeyData keydata not initialized");
+        throw std::runtime_error(
+            "PrivateKey::CheckKeyData keydata not initialized");
     }
 }
 
 }  // end namespace bls
```

### Comparing `blspy-1.0.9/src/privatekey.hpp` & `blspy-2.0.0b1/src/privatekey.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -11,20 +11,14 @@
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.
 
 #ifndef SRC_BLSPRIVATEKEY_HPP_
 #define SRC_BLSPRIVATEKEY_HPP_
 
-#include "relic_conf.h"
-
-#if defined GMP && ARITH == GMP
-#include <gmp.h>
-#endif
-
 #include "elements.hpp"
 
 namespace bls {
 class PrivateKey {
  public:
     // Private keys are represented as 32 byte field elements. Note that
     // not all 32 byte integers are valid keys, the private key must be
@@ -88,15 +82,15 @@
     void CheckKeyData() const;
     /// Deallocate *keydata and keydata if requried
     void DeallocateKeyData();
 
     void InvalidateCaches();
 
     // The actual byte data
-    bn_st* keydata{nullptr};
+    blst_scalar* keydata{nullptr};
 
     mutable bool fG1CacheValid{false};
     mutable G1Element g1Cache;
 
     mutable bool fG2CacheValid{false};
     mutable G2Element g2Cache;
 };
```

### Comparing `blspy-1.0.9/src/schemes.cpp` & `blspy-2.0.0b1/src/schemes.cpp`

 * *Files 15% similar despite different names*

```diff
@@ -8,117 +8,144 @@
 
 // Unless required by applicable law or agreed to in writing, software
 // distributed under the License is distributed on an "AS IS" BASIS,
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.
 
+#include "schemes.hpp"
+
+#include <string.h>
+
 #include <algorithm>
 #include <set>
 
 #include "bls.hpp"
 #include "elements.hpp"
-#include "schemes.hpp"
 #include "hdkeys.hpp"
 
 using std::string;
 using std::vector;
 
 namespace bls {
 
-enum InvariantResult { BAD=false, GOOD=true, CONTINUE };
+enum InvariantResult { BAD = false, GOOD = true, CONTINUE };
 
 // Enforce argument invariants for Agg Sig Verification
 InvariantResult VerifyAggregateSignatureArguments(
     const size_t nPubKeys,
     const size_t nMessages,
-    const G2Element &signature)
+    const G2Element& signature)
 {
     if (nPubKeys == 0) {
         return (nMessages == 0 && signature == G2Element() ? GOOD : BAD);
     }
     if (nPubKeys != nMessages) {
         return BAD;
     }
     return CONTINUE;
 }
 
 /* These are all for the min-pubkey-size variant.
    TODO : analogs for min-signature-size
 */
-const std::string BasicSchemeMPL::CIPHERSUITE_ID = "BLS_SIG_BLS12381G2_XMD:SHA-256_SSWU_RO_NUL_";
-const std::string AugSchemeMPL::CIPHERSUITE_ID = "BLS_SIG_BLS12381G2_XMD:SHA-256_SSWU_RO_AUG_";
-const std::string PopSchemeMPL::CIPHERSUITE_ID = "BLS_SIG_BLS12381G2_XMD:SHA-256_SSWU_RO_POP_";
-const std::string PopSchemeMPL::POP_CIPHERSUITE_ID = "BLS_POP_BLS12381G2_XMD:SHA-256_SSWU_RO_POP_";
+const std::string BasicSchemeMPL::CIPHERSUITE_ID =
+    "BLS_SIG_BLS12381G2_XMD:SHA-256_SSWU_RO_NUL_";
+const std::string AugSchemeMPL::CIPHERSUITE_ID =
+    "BLS_SIG_BLS12381G2_XMD:SHA-256_SSWU_RO_AUG_";
+const std::string PopSchemeMPL::CIPHERSUITE_ID =
+    "BLS_SIG_BLS12381G2_XMD:SHA-256_SSWU_RO_POP_";
+const std::string PopSchemeMPL::POP_CIPHERSUITE_ID =
+    "BLS_POP_BLS12381G2_XMD:SHA-256_SSWU_RO_POP_";
 
-PrivateKey CoreMPL::KeyGen(const vector<uint8_t>& seed) {
+PrivateKey CoreMPL::KeyGen(const vector<uint8_t>& seed)
+{
     return HDKeys::KeyGen(seed);
 }
 
-PrivateKey CoreMPL::KeyGen(const Bytes& seed) {
-    return HDKeys::KeyGen(seed);
-}
+PrivateKey CoreMPL::KeyGen(const Bytes& seed) { return HDKeys::KeyGen(seed); }
 
-vector<uint8_t> CoreMPL::SkToPk(const PrivateKey &seckey)
+vector<uint8_t> CoreMPL::SkToPk(const PrivateKey& seckey)
 {
     return seckey.GetG1Element().Serialize();
 }
 
-G1Element CoreMPL::SkToG1(const PrivateKey &seckey)
+G1Element CoreMPL::SkToG1(const PrivateKey& seckey)
 {
     return seckey.GetG1Element();
 }
 
-G2Element CoreMPL::Sign(const PrivateKey &seckey, const vector<uint8_t> &message)
+G2Element CoreMPL::Sign(
+    const PrivateKey& seckey,
+    const vector<uint8_t>& message)
 {
     return CoreMPL::Sign(seckey, Bytes(message));
 }
 
 G2Element CoreMPL::Sign(const PrivateKey& seckey, const Bytes& message)
 {
-    return seckey.SignG2(message.begin(), message.size(), (const uint8_t*)strCiphersuiteId.c_str(), strCiphersuiteId.length());
+    return seckey.SignG2(
+        message.begin(),
+        message.size(),
+        (const uint8_t*)strCiphersuiteId.c_str(),
+        strCiphersuiteId.length());
 }
 
-bool CoreMPL::Verify(const vector<uint8_t> &pubkey,
-                     const vector<uint8_t> &message,  // unhashed
-                     const vector<uint8_t> &signature)
+bool CoreMPL::Verify(
+    const vector<uint8_t>& pubkey,
+    const vector<uint8_t>& message,  // unhashed
+    const vector<uint8_t>& signature)
 {
-    return CoreMPL::Verify(G1Element::FromBytes(Bytes(pubkey)),
-                           Bytes(message),
-                           G2Element::FromBytes(Bytes(signature)));
+    return CoreMPL::Verify(
+        G1Element::FromBytes(Bytes(pubkey)),
+        Bytes(message),
+        G2Element::FromBytes(Bytes(signature)));
 }
 
-bool CoreMPL::Verify(const Bytes& pubkey, const Bytes& message, const Bytes& signature)
+bool CoreMPL::Verify(
+    const Bytes& pubkey,
+    const Bytes& message,
+    const Bytes& signature)
 {
-    return CoreMPL::Verify(G1Element::FromBytes(pubkey), message, G2Element::FromBytes(signature));
+    return CoreMPL::Verify(
+        G1Element::FromBytes(pubkey), message, G2Element::FromBytes(signature));
 }
 
-bool CoreMPL::Verify(const G1Element &pubkey,
-                     const vector<uint8_t> &message,  // unhashed
-                     const G2Element &signature)
+bool CoreMPL::Verify(
+    const G1Element& pubkey,
+    const vector<uint8_t>& message,  // unhashed
+    const G2Element& signature)
 {
     return CoreMPL::Verify(pubkey, Bytes(message), signature);
 }
 
-bool CoreMPL::Verify(const G1Element& pubkey, const Bytes& message, const G2Element& signature)
-{
-    const G2Element hashedPoint = G2Element::FromMessage(message, (const uint8_t*)strCiphersuiteId.c_str(), strCiphersuiteId.length());
-
-    std::vector<g1_st> vecG1(2);
-    std::vector<g2_st> vecG2(2);
-
-    G1Element::Generator().Negate().ToNative(&vecG1[0]);
-    pubkey.ToNative(&vecG1[1]);
-    signature.ToNative(&vecG2[0]);
-    hashedPoint.ToNative(&vecG2[1]);
+bool CoreMPL::Verify(
+    const G1Element& pubkey,
+    const Bytes& message,
+    const G2Element& signature)
+{
+    blst_p1_affine pubkeyAffine;
+    blst_p2_affine sigAffine;
+
+    pubkey.ToAffine(&pubkeyAffine);
+    signature.ToAffine(&sigAffine);
+
+    auto err = blst_core_verify_pk_in_g1(
+        &pubkeyAffine,
+        &sigAffine,
+        true, /*hash*/
+        message.begin(),
+        message.size(),
+        (const uint8_t*)strCiphersuiteId.c_str(),
+        strCiphersuiteId.length());
 
-    return CoreMPL::NativeVerify((g1_t*)vecG1.data(), (g2_t*)vecG2.data(), 2);
+    return err == BLST_SUCCESS;
 }
 
-vector<uint8_t> CoreMPL::Aggregate(const vector<vector<uint8_t>> &signatures)
+vector<uint8_t> CoreMPL::Aggregate(const vector<vector<uint8_t>>& signatures)
 {
     vector<G2Element> elements;
     for (const vector<uint8_t>& signature : signatures) {
         elements.push_back(G2Element::FromByteVector(signature));
     }
     return CoreMPL::Aggregate(elements).Serialize();
 }
@@ -128,403 +155,500 @@
     vector<G2Element> elements;
     for (const Bytes& signature : signatures) {
         elements.push_back(G2Element::FromBytes(signature));
     }
     return CoreMPL::Aggregate(elements).Serialize();
 }
 
-G2Element CoreMPL::Aggregate(const vector<G2Element> &signatures)
+G2Element CoreMPL::Aggregate(const vector<G2Element>& signatures)
 {
     G2Element aggregated;
     for (const G2Element& signature : signatures) {
         aggregated += signature;
     }
     return aggregated;
 }
 
-G1Element CoreMPL::Aggregate(const vector<G1Element> &publicKeys)
+G1Element CoreMPL::Aggregate(const vector<G1Element>& publicKeys)
 {
     G1Element aggregated;
     for (const G1Element& publicKey : publicKeys) {
         aggregated += publicKey;
     }
     return aggregated;
 }
 
-bool CoreMPL::AggregateVerify(const vector<vector<uint8_t>> &pubkeys,
-                              const vector<vector<uint8_t>> &messages,  // unhashed
-                              const vector<uint8_t> &signature)
+bool CoreMPL::AggregateVerify(
+    const vector<vector<uint8_t>>& pubkeys,
+    const vector<vector<uint8_t>>& messages,  // unhashed
+    const vector<uint8_t>& signature)
 {
     const std::vector<Bytes> vecPubKeyBytes(pubkeys.begin(), pubkeys.end());
     const std::vector<Bytes> vecMessagesBytes(messages.begin(), messages.end());
-    return CoreMPL::AggregateVerify(vecPubKeyBytes, vecMessagesBytes, Bytes(signature));
+    return CoreMPL::AggregateVerify(
+        vecPubKeyBytes, vecMessagesBytes, Bytes(signature));
 }
 
-bool CoreMPL::AggregateVerify(const vector<Bytes>& pubkeys,
-                              const vector<Bytes>& messages,  // unhashed
-                              const Bytes& signature)
+bool CoreMPL::AggregateVerify(
+    const vector<Bytes>& pubkeys,
+    const vector<Bytes>& messages,  // unhashed
+    const Bytes& signature)
 {
     const size_t nPubKeys = pubkeys.size();
     const G2Element signatureElement = G2Element::FromBytes(signature);
-    const auto arg_check = VerifyAggregateSignatureArguments(nPubKeys, messages.size(), signatureElement);
+    const auto arg_check = VerifyAggregateSignatureArguments(
+        nPubKeys, messages.size(), signatureElement);
     if (arg_check != CONTINUE) {
         return arg_check;
     }
 
     vector<G1Element> pubkeyElements;
     for (size_t i = 0; i < nPubKeys; ++i) {
         pubkeyElements.push_back(G1Element::FromBytes(pubkeys[i]));
     }
     return CoreMPL::AggregateVerify(pubkeyElements, messages, signatureElement);
 }
 
-bool CoreMPL::AggregateVerify(const vector<G1Element> &pubkeys,
-                              const vector<vector<uint8_t>> &messages,
-                              const G2Element &signature)
-{
-    return CoreMPL::AggregateVerify(pubkeys, std::vector<Bytes>(messages.begin(), messages.end()), signature);
+bool CoreMPL::AggregateVerify(
+    const vector<G1Element>& pubkeys,
+    const vector<vector<uint8_t>>& messages,
+    const G2Element& signature)
+{
+    return CoreMPL::AggregateVerify(
+        pubkeys,
+        std::vector<Bytes>(messages.begin(), messages.end()),
+        signature);
 }
 
-bool CoreMPL::AggregateVerify(const vector<G1Element>& pubkeys,
-                              const vector<Bytes> &messages,
-                              const G2Element& signature)
+bool CoreMPL::AggregateVerify(
+    const vector<G1Element>& pubkeys,
+    const vector<Bytes>& messages,
+    const G2Element& signature)
 {
     const size_t nPubKeys = pubkeys.size();
-    const auto arg_check = VerifyAggregateSignatureArguments(nPubKeys, messages.size(), signature);
+    const auto arg_check =
+        VerifyAggregateSignatureArguments(nPubKeys, messages.size(), signature);
     if (arg_check != CONTINUE) {
         return arg_check;
     }
 
-    std::vector<g1_st> vecG1(nPubKeys + 1);
-    std::vector<g2_st> vecG2(nPubKeys + 1);
-    G1Element::Generator().Negate().ToNative(&vecG1[0]);
-    signature.ToNative(&vecG2[0]);
-
-    for (size_t i = 0; i < nPubKeys; ++i) {
-        pubkeys[i].ToNative(&vecG1[i + 1]);
-        G2Element::FromMessage(messages[i], (const uint8_t*)strCiphersuiteId.c_str(), strCiphersuiteId.length()).ToNative(&vecG2[i + 1]);
-    }
-
-    return CoreMPL::NativeVerify((g1_t*)vecG1.data(), (g2_t*)vecG2.data(), nPubKeys + 1);
-}
+    blst_pairing* ctx = (blst_pairing*)malloc(blst_pairing_sizeof());
+    blst_pairing_init(
+        ctx,
+        true /*hash*/,
+        (const uint8_t*)strCiphersuiteId.c_str(),
+        strCiphersuiteId.length());
+
+    blst_p1_affine pk_affine;
+    blst_p2_affine sig_affine;
+    blst_fp12 gtsig;
+
+    signature.ToAffine(&sig_affine);
+
+    blst_aggregated_in_g2(&gtsig, &sig_affine);
+
+    for (size_t i = 0; i < nPubKeys; i++) {
+        pubkeys[i].ToAffine(&pk_affine);
+
+        auto err = blst_pairing_aggregate_pk_in_g1(
+            ctx, &pk_affine, nullptr, messages[i].begin(), messages[i].size());
+
+        if (err != BLST_SUCCESS) {
+            free(ctx);
+            return false;
+        }
+    }
+
+    blst_pairing_commit(ctx);
+    auto ret = blst_pairing_finalverify(ctx, &gtsig);
+    free(ctx);
+    return ret;
+}
+
+// bool CoreMPL::NativeVerify(
+//     blst_p1* pubkeys,
+//     blst_p2* mappedHashes,
+//     size_t length)
+// {
+//     blst_fp12 target, candidate, tmpPairing;
+//     memcpy(&target, blst_fp12_one(), sizeof(blst_fp12));
+//     memcpy(&candidate, blst_fp12_one(), sizeof(blst_fp12));
+
+//     // prod e(pubkey[i], hash[i]) * e(-g1, aggSig)
+//     // Performs pubKeys.size() pairings, 250 at a time
+
+//     blst_p1_affine Ps[length];
+//     blst_p2_affine Qs[length];
+//     const blst_p1* ppoints[2] = {pubkeys, NULL};
+//     const blst_p2* pqoints[2] = {mappedHashes, NULL};
+
+//     blst_p1s_to_affine(Ps, ppoints, length);
+//     blst_p2s_to_affine(Qs, pqoints, length);
+//     for (size_t i = 0; i < length; i += 250) {
+//         size_t numPairings = std::min((length - i), (size_t)250);
+//         const blst_p1_affine* const pP = &(Ps[i]);
+//         const blst_p2_affine* const pQ = &(Qs[i]);
+//         blst_miller_loop_n(&tmpPairing, &pQ, &pP, numPairings);
+//         blst_fp12_mul(&candidate, &candidate, &tmpPairing);
+//     }
+//     // 1 =? prod e(pubkey[i], hash[i]) * e(-g1, aggSig)
+//     if (memcmp(&target, &candidate, sizeof(blst_fp12)) != 0) {
+//         return false;
+//     }
+//     return true;
+// }
 
-bool CoreMPL::NativeVerify(g1_t *pubkeys, g2_t *mappedHashes, size_t length)
+PrivateKey CoreMPL::DeriveChildSk(const PrivateKey& sk, uint32_t index)
 {
-    gt_t target, candidate, tmpPairing;
-    fp12_zero(target);
-    fp_set_dig(target[0][0][0], 1);
-    fp12_zero(candidate);
-    fp_set_dig(candidate[0][0][0], 1);
-
-    // prod e(pubkey[i], hash[i]) * e(-g1, aggSig)
-    // Performs pubKeys.size() pairings, 250 at a time
-
-    for (size_t i = 0; i < length; i += 250) {
-        size_t numPairings = std::min((length - i), (size_t)250);
-        pc_map_sim(tmpPairing, pubkeys + i, mappedHashes + i, numPairings);
-        fp12_mul(candidate, candidate, tmpPairing);
-    }
-
-    // 1 =? prod e(pubkey[i], hash[i]) * e(-g1, aggSig)
-    if (gt_cmp(target, candidate) != RLC_EQ || core_get()->code != RLC_OK) {
-        core_get()->code = RLC_OK;
-        return false;
-    }
-    BLS::CheckRelicErrors();
-    return true;
-}
-
-PrivateKey CoreMPL::DeriveChildSk(const PrivateKey& sk, uint32_t index) {
     return HDKeys::DeriveChildSk(sk, index);
 }
 
-PrivateKey CoreMPL::DeriveChildSkUnhardened(const PrivateKey& sk, uint32_t index) {
+PrivateKey CoreMPL::DeriveChildSkUnhardened(
+    const PrivateKey& sk,
+    uint32_t index)
+{
     return HDKeys::DeriveChildSkUnhardened(sk, index);
 }
 
-G1Element CoreMPL::DeriveChildPkUnhardened(const G1Element& pk, uint32_t index) {
+G1Element CoreMPL::DeriveChildPkUnhardened(const G1Element& pk, uint32_t index)
+{
     return HDKeys::DeriveChildG1Unhardened(pk, index);
 }
 
-bool BasicSchemeMPL::AggregateVerify(const vector<vector<uint8_t>> &pubkeys,
-                                     const vector<vector<uint8_t>> &messages,
-                                     const vector<uint8_t> &signature)
+bool BasicSchemeMPL::AggregateVerify(
+    const vector<vector<uint8_t>>& pubkeys,
+    const vector<vector<uint8_t>>& messages,
+    const vector<uint8_t>& signature)
 {
     const size_t nPubKeys = pubkeys.size();
-    auto arg_check = VerifyAggregateSignatureArguments(nPubKeys, messages.size(), G2Element::FromByteVector(signature));
+    auto arg_check = VerifyAggregateSignatureArguments(
+        nPubKeys, messages.size(), G2Element::FromByteVector(signature));
     if (arg_check != CONTINUE) {
         return arg_check;
     }
 
-    const std::set<vector<uint8_t>> setMessages(messages.begin(), messages.end());
+    const std::set<vector<uint8_t>> setMessages(
+        messages.begin(), messages.end());
     if (setMessages.size() != nPubKeys) {
         return false;
     }
     return CoreMPL::AggregateVerify(pubkeys, messages, signature);
 }
 
-bool BasicSchemeMPL::AggregateVerify(const vector<Bytes>& pubkeys,
-                                     const vector<Bytes>& messages,
-                                     const Bytes& signature)
+bool BasicSchemeMPL::AggregateVerify(
+    const vector<Bytes>& pubkeys,
+    const vector<Bytes>& messages,
+    const Bytes& signature)
 {
     const size_t nPubKeys = pubkeys.size();
-    const auto arg_check = VerifyAggregateSignatureArguments(nPubKeys, messages.size(), G2Element::FromBytes(signature));
-    if (arg_check != CONTINUE) return arg_check;
+    const auto arg_check = VerifyAggregateSignatureArguments(
+        nPubKeys, messages.size(), G2Element::FromBytes(signature));
+    if (arg_check != CONTINUE)
+        return arg_check;
 
     std::set<vector<uint8_t>> setMessages;
     for (const auto& message : messages) {
         setMessages.insert({message.begin(), message.end()});
     }
     if (setMessages.size() != nPubKeys) {
         return false;
     }
     return CoreMPL::AggregateVerify(pubkeys, messages, signature);
 }
 
-bool BasicSchemeMPL::AggregateVerify(const vector<G1Element> &pubkeys,
-                                     const vector<vector<uint8_t>> &messages,
-                                     const G2Element &signature)
+bool BasicSchemeMPL::AggregateVerify(
+    const vector<G1Element>& pubkeys,
+    const vector<vector<uint8_t>>& messages,
+    const G2Element& signature)
 {
     const size_t nPubKeys = pubkeys.size();
-    const auto arg_check = VerifyAggregateSignatureArguments(nPubKeys, messages.size(), signature);
+    const auto arg_check =
+        VerifyAggregateSignatureArguments(nPubKeys, messages.size(), signature);
     if (arg_check != CONTINUE) {
         return arg_check;
     }
 
-    const std::set<vector<uint8_t>> setMessages(messages.begin(), messages.end());
+    const std::set<vector<uint8_t>> setMessages(
+        messages.begin(), messages.end());
     if (setMessages.size() != nPubKeys) {
         return false;
     }
     return CoreMPL::AggregateVerify(pubkeys, messages, signature);
 }
 
-bool BasicSchemeMPL::AggregateVerify(const vector<G1Element>& pubkeys,
-                                     const vector<Bytes> &messages,
-                                     const G2Element& signature)
+bool BasicSchemeMPL::AggregateVerify(
+    const vector<G1Element>& pubkeys,
+    const vector<Bytes>& messages,
+    const G2Element& signature)
 {
     const size_t nPubKeys = pubkeys.size();
-    const auto arg_check = VerifyAggregateSignatureArguments(nPubKeys, messages.size(), signature);
-    if (arg_check != CONTINUE) return arg_check;
+    const auto arg_check =
+        VerifyAggregateSignatureArguments(nPubKeys, messages.size(), signature);
+    if (arg_check != CONTINUE)
+        return arg_check;
 
     std::set<vector<uint8_t>> setMessages;
     for (const auto& message : messages) {
         setMessages.insert({message.begin(), message.end()});
     }
     if (setMessages.size() != nPubKeys) {
         return false;
     }
     return CoreMPL::AggregateVerify(pubkeys, messages, signature);
 }
 
-G2Element AugSchemeMPL::Sign(const PrivateKey &seckey, const vector<uint8_t> &message)
+G2Element AugSchemeMPL::Sign(
+    const PrivateKey& seckey,
+    const vector<uint8_t>& message)
 {
     return AugSchemeMPL::Sign(seckey, message, seckey.GetG1Element());
 }
 
 G2Element AugSchemeMPL::Sign(const PrivateKey& seckey, const Bytes& message)
 {
     return AugSchemeMPL::Sign(seckey, message, seckey.GetG1Element());
 }
 
 // Used for prepending different augMessage
-G2Element AugSchemeMPL::Sign(const PrivateKey &seckey,
-                             const vector<uint8_t> &message,
-                             const G1Element &prepend_pk)
+G2Element AugSchemeMPL::Sign(
+    const PrivateKey& seckey,
+    const vector<uint8_t>& message,
+    const G1Element& prepend_pk)
 {
     return AugSchemeMPL::Sign(seckey, Bytes(message), prepend_pk);
 }
 
 // Used for prepending different augMessage
-G2Element AugSchemeMPL::Sign(const PrivateKey& seckey,
-                             const Bytes& message,
-                             const G1Element& prepend_pk)
+G2Element AugSchemeMPL::Sign(
+    const PrivateKey& seckey,
+    const Bytes& message,
+    const G1Element& prepend_pk)
 {
     vector<uint8_t> augMessage = prepend_pk.Serialize();
     augMessage.reserve(augMessage.size() + message.size());
     augMessage.insert(augMessage.end(), message.begin(), message.end());
     return CoreMPL::Sign(seckey, augMessage);
 }
 
-bool AugSchemeMPL::Verify(const vector<uint8_t> &pubkey,
-                          const vector<uint8_t> &message,
-                          const vector<uint8_t> &signature)
+bool AugSchemeMPL::Verify(
+    const vector<uint8_t>& pubkey,
+    const vector<uint8_t>& message,
+    const vector<uint8_t>& signature)
 {
     vector<uint8_t> augMessage(pubkey);
     augMessage.reserve(augMessage.size() + message.size());
     augMessage.insert(augMessage.end(), message.begin(), message.end());
     return CoreMPL::Verify(pubkey, augMessage, signature);
 }
 
-bool AugSchemeMPL::Verify(const Bytes& pubkey,
-                          const Bytes& message,
-                          const Bytes& signature)
+bool AugSchemeMPL::Verify(
+    const Bytes& pubkey,
+    const Bytes& message,
+    const Bytes& signature)
 {
     vector<uint8_t> augMessage(pubkey.begin(), pubkey.end());
     augMessage.reserve(augMessage.size() + message.size());
     augMessage.insert(augMessage.end(), message.begin(), message.end());
     return CoreMPL::Verify(pubkey, Bytes(augMessage), Bytes(signature));
 }
 
-bool AugSchemeMPL::Verify(const G1Element &pubkey,
-                          const vector<uint8_t> &message,
-                          const G2Element &signature)
+bool AugSchemeMPL::Verify(
+    const G1Element& pubkey,
+    const vector<uint8_t>& message,
+    const G2Element& signature)
 {
     return AugSchemeMPL::Verify(pubkey, Bytes(message), signature);
 }
 
-bool AugSchemeMPL::Verify(const G1Element& pubkey,
-                          const Bytes& message,
-                          const G2Element& signature)
+bool AugSchemeMPL::Verify(
+    const G1Element& pubkey,
+    const Bytes& message,
+    const G2Element& signature)
 {
     vector<uint8_t> augMessage = pubkey.Serialize();
     augMessage.reserve(augMessage.size() + message.size());
     augMessage.insert(augMessage.end(), message.begin(), message.end());
     return CoreMPL::Verify(pubkey, augMessage, signature);
 }
 
-bool AugSchemeMPL::AggregateVerify(const vector<vector<uint8_t>> &pubkeys,
-                                   const vector<vector<uint8_t>> &messages,
-                                   const vector<uint8_t> &signature)
+bool AugSchemeMPL::AggregateVerify(
+    const vector<vector<uint8_t>>& pubkeys,
+    const vector<vector<uint8_t>>& messages,
+    const vector<uint8_t>& signature)
 {
     std::vector<Bytes> vecPubKeyBytes(pubkeys.begin(), pubkeys.end());
     std::vector<Bytes> vecMessagesBytes(messages.begin(), messages.end());
-    return AugSchemeMPL::AggregateVerify(vecPubKeyBytes, vecMessagesBytes, Bytes(signature));
+    return AugSchemeMPL::AggregateVerify(
+        vecPubKeyBytes, vecMessagesBytes, Bytes(signature));
 }
 
-bool AugSchemeMPL::AggregateVerify(const vector<Bytes>& pubkeys,
-                                   const vector<Bytes>& messages,
-                                   const Bytes& signature)
+bool AugSchemeMPL::AggregateVerify(
+    const vector<Bytes>& pubkeys,
+    const vector<Bytes>& messages,
+    const Bytes& signature)
 {
     size_t nPubKeys = pubkeys.size();
-    auto arg_check = VerifyAggregateSignatureArguments(nPubKeys, messages.size(), G2Element::FromBytes(signature));
+    auto arg_check = VerifyAggregateSignatureArguments(
+        nPubKeys, messages.size(), G2Element::FromBytes(signature));
     if (arg_check != CONTINUE) {
         return arg_check;
     }
 
     vector<vector<uint8_t>> augMessages(nPubKeys);
     for (size_t i = 0; i < nPubKeys; ++i) {
         vector<uint8_t>& aug = augMessages[i];
         aug.reserve(pubkeys[i].size() + messages[i].size());
         aug.insert(aug.end(), pubkeys[i].begin(), pubkeys[i].end());
         aug.insert(aug.end(), messages[i].begin(), messages[i].end());
     }
 
-    std::vector<Bytes> vecAugMessageBytes(augMessages.begin(), augMessages.end());
+    std::vector<Bytes> vecAugMessageBytes(
+        augMessages.begin(), augMessages.end());
     return CoreMPL::AggregateVerify(pubkeys, vecAugMessageBytes, signature);
 }
 
-bool AugSchemeMPL::AggregateVerify(const vector<G1Element>& pubkeys,
-                                   const vector<vector<uint8_t>>& messages,
-                                   const G2Element& signature)
+bool AugSchemeMPL::AggregateVerify(
+    const vector<G1Element>& pubkeys,
+    const vector<vector<uint8_t>>& messages,
+    const G2Element& signature)
 {
     std::vector<Bytes> vecMessagesBytes(messages.begin(), messages.end());
     return AugSchemeMPL::AggregateVerify(pubkeys, vecMessagesBytes, signature);
 }
 
-bool AugSchemeMPL::AggregateVerify(const vector<G1Element>& pubkeys,
-                                   const vector<Bytes>& messages,
-                                   const G2Element& signature)
+bool AugSchemeMPL::AggregateVerify(
+    const vector<G1Element>& pubkeys,
+    const vector<Bytes>& messages,
+    const G2Element& signature)
 {
     size_t nPubKeys = pubkeys.size();
-    auto arg_check = VerifyAggregateSignatureArguments(nPubKeys, messages.size(), signature);
+    auto arg_check =
+        VerifyAggregateSignatureArguments(nPubKeys, messages.size(), signature);
     if (arg_check != CONTINUE) {
         return arg_check;
     }
 
     vector<vector<uint8_t>> augMessages(nPubKeys);
-    for (int i = 0; i < nPubKeys; ++i) {
+    for (size_t i = 0; i < nPubKeys; ++i) {
         vector<uint8_t>& aug = augMessages[i];
         vector<uint8_t>&& pubkey = pubkeys[i].Serialize();
         aug.reserve(pubkey.size() + messages[i].size());
         aug.insert(aug.end(), pubkey.begin(), pubkey.end());
         aug.insert(aug.end(), messages[i].begin(), messages[i].end());
     }
 
     return CoreMPL::AggregateVerify(pubkeys, augMessages, signature);
 }
 
-G2Element PopSchemeMPL::PopProve(const PrivateKey &seckey)
+G2Element PopSchemeMPL::PopProve(const PrivateKey& seckey)
 {
-    const G1Element& pk = seckey.GetG1Element();
-    const G2Element hashedKey = G2Element::FromMessage(pk.Serialize(), (const uint8_t *)POP_CIPHERSUITE_ID.c_str(), POP_CIPHERSUITE_ID.length());
-    return seckey.GetG2Power(hashedKey);
-}
+    std::vector<uint8_t> pubkey_bytes = seckey.GetG1Element().Serialize();
 
+    return seckey.SignG2(
+        pubkey_bytes.data(),
+        pubkey_bytes.size(),
+        (const uint8_t*)POP_CIPHERSUITE_ID.c_str(),
+        POP_CIPHERSUITE_ID.length());
+}
 
-bool PopSchemeMPL::PopVerify(const G1Element &pubkey, const G2Element &signature_proof)
+bool PopSchemeMPL::PopVerify(
+    const G1Element& pubkey,
+    const G2Element& signature_proof)
 {
-    const G2Element hashedPoint = G2Element::FromMessage(pubkey.Serialize(), (const uint8_t*)POP_CIPHERSUITE_ID.c_str(), POP_CIPHERSUITE_ID.length());
+    blst_p1_affine pubkeyAffine;
+    blst_p2_affine sigAffine;
 
-    g1_t g1s[2];
-    g2_t g2s[2];
+    pubkey.ToAffine(&pubkeyAffine);
+    signature_proof.ToAffine(&sigAffine);
+    std::vector<uint8_t> pubkey_bytes = pubkey.Serialize();
 
-    G1Element::Generator().Negate().ToNative(g1s[0]);
-    pubkey.ToNative(g1s[1]);
-    signature_proof.ToNative(g2s[0]);
-    hashedPoint.ToNative(g2s[1]);
+    auto err = blst_core_verify_pk_in_g1(
+        &pubkeyAffine,
+        &sigAffine,
+        true, /*hash*/
+        pubkey_bytes.data(),
+        pubkey_bytes.size(),
+        (const uint8_t*)POP_CIPHERSUITE_ID.c_str(),
+        POP_CIPHERSUITE_ID.length());
 
-    return CoreMPL::NativeVerify(g1s, g2s, 2);
+    return err == BLST_SUCCESS;
 }
 
-bool PopSchemeMPL::PopVerify(const vector<uint8_t> &pubkey, const vector<uint8_t> &proof)
+bool PopSchemeMPL::PopVerify(
+    const vector<uint8_t>& pubkey,
+    const vector<uint8_t>& proof)
 {
     return PopSchemeMPL::PopVerify(Bytes(pubkey), Bytes(proof));
 }
 
 bool PopSchemeMPL::PopVerify(const Bytes& pubkey, const Bytes& proof)
 {
-    const G2Element hashedPoint = G2Element::FromMessage(pubkey, (const uint8_t*)POP_CIPHERSUITE_ID.c_str(), POP_CIPHERSUITE_ID.length());
+    return PopSchemeMPL::PopVerify(
+        G1Element::FromBytes(pubkey), G2Element::FromBytes(proof));
+
+    // const G2Element hashedPoint = G2Element::FromMessage(
+    //     pubkey,
+    //     (const uint8_t*)POP_CIPHERSUITE_ID.c_str(),
+    //     POP_CIPHERSUITE_ID.length());
 
-    g1_t g1s[2];
-    g2_t g2s[2];
+    // blst_p1 g1s[2];
+    // blst_p2 g2s[2];
 
-    G1Element::Generator().Negate().ToNative(g1s[0]);
-    G1Element::FromBytes(pubkey).ToNative(g1s[1]);
-    G2Element::FromBytes(proof).ToNative(g2s[0]);
-    hashedPoint.ToNative(g2s[1]);
+    // G1Element::Generator().Negate().ToNative(&(g1s[0]));
+    // G1Element::FromBytes(pubkey).ToNative(&(g1s[1]));
+    // G2Element::FromBytes(proof).ToNative(&(g2s[0]));
+    // hashedPoint.ToNative(&(g2s[1]));
 
-    return CoreMPL::NativeVerify(g1s, g2s, 2);
+    // return CoreMPL::NativeVerify(g1s, g2s, 2);
 }
 
-bool PopSchemeMPL::FastAggregateVerify(const vector<G1Element> &pubkeys,
-                                       const vector<uint8_t> &message,
-                                       const G2Element &signature)
+bool PopSchemeMPL::FastAggregateVerify(
+    const vector<G1Element>& pubkeys,
+    const vector<uint8_t>& message,
+    const G2Element& signature)
 {
-    return PopSchemeMPL::FastAggregateVerify(pubkeys, Bytes(message), signature);
+    return PopSchemeMPL::FastAggregateVerify(
+        pubkeys, Bytes(message), signature);
 }
 
-bool PopSchemeMPL::FastAggregateVerify(const vector<G1Element>& pubkeys,
-                                       const Bytes& message,
-                                       const G2Element& signature)
+bool PopSchemeMPL::FastAggregateVerify(
+    const vector<G1Element>& pubkeys,
+    const Bytes& message,
+    const G2Element& signature)
 {
     if (pubkeys.size() == 0) {
         return false;
     }
-    // No VerifyAggregateSignatureArguments checks required here as we have exactly one pubkey and one message.
+    // No VerifyAggregateSignatureArguments checks required here as we have
+    // exactly one pubkey and one message.
     return CoreMPL::Verify(CoreMPL::Aggregate(pubkeys), message, signature);
 }
 
-bool PopSchemeMPL::FastAggregateVerify(const vector<vector<uint8_t>> &pubkeys,
-                                       const vector<uint8_t> &message,
-                                       const vector<uint8_t> &signature)
+bool PopSchemeMPL::FastAggregateVerify(
+    const vector<vector<uint8_t>>& pubkeys,
+    const vector<uint8_t>& message,
+    const vector<uint8_t>& signature)
 {
     const std::vector<Bytes> vecPubKeyBytes(pubkeys.begin(), pubkeys.end());
-    return PopSchemeMPL::FastAggregateVerify(vecPubKeyBytes, Bytes(message), Bytes(signature));
+    return PopSchemeMPL::FastAggregateVerify(
+        vecPubKeyBytes, Bytes(message), Bytes(signature));
 }
 
-bool PopSchemeMPL::FastAggregateVerify(const vector<Bytes>& pubkeys,
-                                       const Bytes& message,
-                                       const Bytes& signature)
+bool PopSchemeMPL::FastAggregateVerify(
+    const vector<Bytes>& pubkeys,
+    const Bytes& message,
+    const Bytes& signature)
 {
     const size_t nPubKeys = pubkeys.size();
     if (nPubKeys == 0) {
         return false;
     }
 
     vector<G1Element> pkelements;
     for (size_t i = 0; i < nPubKeys; ++i) {
         pkelements.push_back(G1Element::FromBytes(pubkeys[i]));
     }
 
-    return PopSchemeMPL::FastAggregateVerify(pkelements, message, G2Element::FromBytes(signature));
+    return PopSchemeMPL::FastAggregateVerify(
+        pkelements, message, G2Element::FromBytes(signature));
 }
 }  // end namespace bls
```

### Comparing `blspy-1.0.9/src/schemes.hpp` & `blspy-2.0.0b1/src/schemes.hpp`

 * *Files 16% similar despite different names*

```diff
@@ -14,194 +14,221 @@
 
 #ifndef SRC_BLSSCHEMES_HPP_
 #define SRC_BLSSCHEMES_HPP_
 
 #include <iostream>
 #include <vector>
 
-#include "relic_conf.h"
-
-#if defined GMP && ARITH == GMP
-#include <gmp.h>
-#endif
-
 #include "elements.hpp"
 #include "privatekey.hpp"
 
 using std::vector;
 
 // These are all MPL schemes
 namespace bls {
 
 class Bytes;
 
 class CoreMPL {
-
 public:
     CoreMPL() = delete;
     CoreMPL(const std::string& strId) : strCiphersuiteId(strId) {}
+    virtual ~CoreMPL() {}
     // Generates a private key from a seed, similar to HD key generation
     // (hashes the seed), and reduces it mod the group order
     virtual PrivateKey KeyGen(const vector<uint8_t>& seed);
     virtual PrivateKey KeyGen(const Bytes& seed);
 
     // Generates a public key from a secret key
-    virtual vector<uint8_t> SkToPk(const PrivateKey &seckey);
+    virtual vector<uint8_t> SkToPk(const PrivateKey& seckey);
 
-    virtual G1Element SkToG1(const PrivateKey &seckey);
+    virtual G1Element SkToG1(const PrivateKey& seckey);
 
-    virtual G2Element Sign(const PrivateKey &seckey, const vector<uint8_t> &message);
+    virtual G2Element Sign(
+        const PrivateKey& seckey,
+        const vector<uint8_t>& message);
     virtual G2Element Sign(const PrivateKey& seckey, const Bytes& message);
 
-    virtual bool Verify(const vector<uint8_t> &pubkey,
-                        const vector<uint8_t> &message,
-                        const vector<uint8_t> &signature);
-
-    virtual bool Verify(const Bytes& pubkey, const Bytes& message, const Bytes& signature);
-
-    virtual bool Verify(const G1Element &pubkey,
-                        const vector<uint8_t> &message,
-                        const G2Element &signature);
-
-    virtual bool Verify(const G1Element& pubkey, const Bytes& message, const G2Element& signature);
+    virtual bool Verify(
+        const vector<uint8_t>& pubkey,
+        const vector<uint8_t>& message,
+        const vector<uint8_t>& signature);
+
+    virtual bool Verify(
+        const Bytes& pubkey,
+        const Bytes& message,
+        const Bytes& signature);
+
+    virtual bool Verify(
+        const G1Element& pubkey,
+        const vector<uint8_t>& message,
+        const G2Element& signature);
+
+    virtual bool Verify(
+        const G1Element& pubkey,
+        const Bytes& message,
+        const G2Element& signature);
 
-    virtual vector<uint8_t> Aggregate(const vector<vector<uint8_t>> &signatures);
+    virtual vector<uint8_t> Aggregate(
+        const vector<vector<uint8_t>>& signatures);
     virtual vector<uint8_t> Aggregate(const vector<Bytes>& signatures);
 
-    virtual G2Element Aggregate(const vector<G2Element> &signatures);
+    virtual G2Element Aggregate(const vector<G2Element>& signatures);
 
-    virtual G1Element Aggregate(const vector<G1Element> &publicKeys);
+    virtual G1Element Aggregate(const vector<G1Element>& publicKeys);
 
-    virtual bool AggregateVerify(const vector<vector<uint8_t>> &pubkeys,
-                                 const vector<vector<uint8_t>> &messages,
-                                 const vector<uint8_t> &signature);
-
-    virtual bool AggregateVerify(const vector<Bytes>& pubkeys,
-                                 const vector<Bytes>& messages,
-                                 const Bytes& signature);
-
-    virtual bool AggregateVerify(const vector<G1Element> &pubkeys,
-                                 const vector<vector<uint8_t>> &messages,
-                                 const G2Element &signature);
-
-     virtual bool AggregateVerify(const vector<G1Element>& pubkeys,
-                                  const vector<Bytes>& messages,
-                                  const G2Element& signature);
+    virtual bool AggregateVerify(
+        const vector<vector<uint8_t>>& pubkeys,
+        const vector<vector<uint8_t>>& messages,
+        const vector<uint8_t>& signature);
+
+    virtual bool AggregateVerify(
+        const vector<Bytes>& pubkeys,
+        const vector<Bytes>& messages,
+        const Bytes& signature);
+
+    virtual bool AggregateVerify(
+        const vector<G1Element>& pubkeys,
+        const vector<vector<uint8_t>>& messages,
+        const G2Element& signature);
+
+    virtual bool AggregateVerify(
+        const vector<G1Element>& pubkeys,
+        const vector<Bytes>& messages,
+        const G2Element& signature);
 
     PrivateKey DeriveChildSk(const PrivateKey& sk, uint32_t index);
     PrivateKey DeriveChildSkUnhardened(const PrivateKey& sk, uint32_t index);
     G1Element DeriveChildPkUnhardened(const G1Element& sk, uint32_t index);
 
 protected:
     const std::string& strCiphersuiteId;
-    bool NativeVerify(g1_t *pubKeys, g2_t *mappedHashes, size_t length);
+    // bool NativeVerify(blst_p1 *pubKeys, blst_p2 *mappedHashes, size_t
+    // length);
 };
 
-class BasicSchemeMPL : public CoreMPL {
+class BasicSchemeMPL final : public CoreMPL {
 public:
     static const std::string CIPHERSUITE_ID;
     BasicSchemeMPL() : CoreMPL(BasicSchemeMPL::CIPHERSUITE_ID) {}
-    bool AggregateVerify(const vector<vector<uint8_t>> &pubkeys,
-                         const vector<vector<uint8_t>> &messages,
-                         const vector<uint8_t> &signature) override;
-
-    bool AggregateVerify(const vector<Bytes>& pubkeys,
-                         const vector<Bytes>& messages,
-                         const Bytes& signature) override;
-
-    bool AggregateVerify(const vector<G1Element> &pubkeys,
-                         const vector<vector<uint8_t>> &messages,
-                         const G2Element &signature) override;
-
-    bool AggregateVerify(const vector<G1Element>& pubkeys,
-                         const vector<Bytes>& messages,
-                         const G2Element& signature) override;
+    bool AggregateVerify(
+        const vector<vector<uint8_t>>& pubkeys,
+        const vector<vector<uint8_t>>& messages,
+        const vector<uint8_t>& signature) override;
+
+    bool AggregateVerify(
+        const vector<Bytes>& pubkeys,
+        const vector<Bytes>& messages,
+        const Bytes& signature) override;
+
+    bool AggregateVerify(
+        const vector<G1Element>& pubkeys,
+        const vector<vector<uint8_t>>& messages,
+        const G2Element& signature) override;
+
+    bool AggregateVerify(
+        const vector<G1Element>& pubkeys,
+        const vector<Bytes>& messages,
+        const G2Element& signature) override;
 };
 
-class AugSchemeMPL : public CoreMPL {
-
+class AugSchemeMPL final : public CoreMPL {
 public:
     static const std::string CIPHERSUITE_ID;
     AugSchemeMPL() : CoreMPL(AugSchemeMPL::CIPHERSUITE_ID) {}
 
-    G2Element Sign(const PrivateKey &seckey, const vector<uint8_t> &message) override;
+    G2Element Sign(const PrivateKey& seckey, const vector<uint8_t>& message)
+        override;
 
     G2Element Sign(const PrivateKey& seckey, const Bytes& message) override;
 
     // Used for prepending different augMessage
-    G2Element Sign(const PrivateKey &seckey,
-                   const vector<uint8_t> &message,
-                   const G1Element &prepend_pk);
+    G2Element Sign(
+        const PrivateKey& seckey,
+        const vector<uint8_t>& message,
+        const G1Element& prepend_pk);
 
     // Used for prepending different augMessage
-    G2Element Sign(const PrivateKey& seckey,
-                   const Bytes& message,
-                   const G1Element& prepend_pk);
-
-    bool Verify(const vector<uint8_t> &pubkey,
-                const vector<uint8_t> &message,
-                const vector<uint8_t> &signature) override;
-
-    bool Verify(const Bytes& pubkey,
-                const Bytes& message,
-                const Bytes& signature) override;
-
-    bool Verify(const G1Element &pubkey,
-                const vector<uint8_t> &message,
-                const G2Element &signature) override;
-
-    bool Verify(const G1Element& pubkey,
-                const Bytes& message,
-                const G2Element& signature) override;
-
-    bool AggregateVerify(const vector<vector<uint8_t>> &pubkeys,
-                         const vector<vector<uint8_t>> &messages,
-                         const vector<uint8_t> &signature) override;
-
-    bool AggregateVerify(const vector<Bytes>& pubkeys,
-                         const vector<Bytes>& messages,
-                         const Bytes& signature) override;
-
-    bool AggregateVerify(const vector<G1Element> &pubkeys,
-                         const vector<vector<uint8_t>> &messages,
-                         const G2Element &signature) override;
-
-    bool AggregateVerify(const vector<G1Element>& pubkeys,
-                         const vector<Bytes>& messages,
-                         const G2Element& signature) override;
+    G2Element Sign(
+        const PrivateKey& seckey,
+        const Bytes& message,
+        const G1Element& prepend_pk);
+
+    bool Verify(
+        const vector<uint8_t>& pubkey,
+        const vector<uint8_t>& message,
+        const vector<uint8_t>& signature) override;
+
+    bool Verify(
+        const Bytes& pubkey,
+        const Bytes& message,
+        const Bytes& signature) override;
+
+    bool Verify(
+        const G1Element& pubkey,
+        const vector<uint8_t>& message,
+        const G2Element& signature) override;
+
+    bool Verify(
+        const G1Element& pubkey,
+        const Bytes& message,
+        const G2Element& signature) override;
+
+    bool AggregateVerify(
+        const vector<vector<uint8_t>>& pubkeys,
+        const vector<vector<uint8_t>>& messages,
+        const vector<uint8_t>& signature) override;
+
+    bool AggregateVerify(
+        const vector<Bytes>& pubkeys,
+        const vector<Bytes>& messages,
+        const Bytes& signature) override;
+
+    bool AggregateVerify(
+        const vector<G1Element>& pubkeys,
+        const vector<vector<uint8_t>>& messages,
+        const G2Element& signature) override;
+
+    bool AggregateVerify(
+        const vector<G1Element>& pubkeys,
+        const vector<Bytes>& messages,
+        const G2Element& signature) override;
 };
 
-class PopSchemeMPL : public CoreMPL {
-
+class PopSchemeMPL final : public CoreMPL {
 public:
     static const std::string CIPHERSUITE_ID;
     static const std::string POP_CIPHERSUITE_ID;
     PopSchemeMPL() : CoreMPL(PopSchemeMPL::CIPHERSUITE_ID) {}
 
-    G2Element PopProve(const PrivateKey &seckey);
+    G2Element PopProve(const PrivateKey& seckey);
 
-    bool PopVerify(const G1Element &pubkey, const G2Element &signature_proof);
+    bool PopVerify(const G1Element& pubkey, const G2Element& signature_proof);
 
-    bool PopVerify(const vector<uint8_t> &pubkey, const vector<uint8_t> &proof);
+    bool PopVerify(const vector<uint8_t>& pubkey, const vector<uint8_t>& proof);
 
     bool PopVerify(const Bytes& pubkey, const Bytes& proof);
 
-    bool FastAggregateVerify(const vector<G1Element> &pubkeys,
-                             const vector<uint8_t> &message,
-                             const G2Element &signature);
-
-    bool FastAggregateVerify(const vector<G1Element>& pubkeys,
-                             const Bytes& message,
-                             const G2Element& signature);
-
-    bool FastAggregateVerify(const vector<vector<uint8_t>> &pubkeys,
-                             const vector<uint8_t> &message,
-                             const vector<uint8_t> &signature);
-
-    bool FastAggregateVerify(const vector<Bytes>& pubkeys,
-                             const Bytes& message,
-                             const Bytes& signature);
+    bool FastAggregateVerify(
+        const vector<G1Element>& pubkeys,
+        const vector<uint8_t>& message,
+        const G2Element& signature);
+
+    bool FastAggregateVerify(
+        const vector<G1Element>& pubkeys,
+        const Bytes& message,
+        const G2Element& signature);
+
+    bool FastAggregateVerify(
+        const vector<vector<uint8_t>>& pubkeys,
+        const vector<uint8_t>& message,
+        const vector<uint8_t>& signature);
+
+    bool FastAggregateVerify(
+        const vector<Bytes>& pubkeys,
+        const Bytes& message,
+        const Bytes& signature);
 };
 
 }  // end namespace bls
 
 #endif  // SRC_BLSSCHEMES_HPP_
```

### Comparing `blspy-1.0.9/src/test-bench.cpp` & `blspy-2.0.0b1/src/test-bench.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -9,70 +9,79 @@
 // Unless required by applicable law or agreed to in writing, software
 // distributed under the License is distributed on an "AS IS" BASIS,
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.
 
 #include <chrono>
+
 #include "bls.hpp"
 #include "test-utils.hpp"
 
-extern "C" {
-#include "relic.h"
-}
-
-using std::string;
-using std::vector;
 using std::cout;
 using std::endl;
+using std::string;
+using std::vector;
 
 using namespace bls;
 
+std::vector<uint8_t> wjbgetRandomSeed()
+{
+    uint8_t buf[32];
 
-void benchSigs() {
+    for (int i = 0; i < 32; i++) buf[i] = rand();
+
+    std::vector<uint8_t> ret(buf, buf + 32);
+    return ret;
+}
+
+void benchSigs()
+{
     string testName = "Signing";
     const int numIters = 5000;
     PrivateKey sk = AugSchemeMPL().KeyGen(getRandomSeed());
     vector<uint8_t> message1 = sk.GetG1Element().Serialize();
 
     auto start = startStopwatch();
 
     for (int i = 0; i < numIters; i++) {
         AugSchemeMPL().Sign(sk, message1);
     }
     endStopwatch(testName, start, numIters);
 }
 
-void benchVerification() {
+void benchVerification()
+{
     string testName = "Verification";
     const int numIters = 10000;
     PrivateKey sk = AugSchemeMPL().KeyGen(getRandomSeed());
     G1Element pk = sk.GetG1Element();
-
     std::vector<G2Element> sigs;
 
+    vector<uint8_t> pkBytes = pk.Serialize();
     for (int i = 0; i < numIters; i++) {
         uint8_t message[4];
         Util::IntToFourBytes(message, i);
         vector<uint8_t> messageBytes(message, message + 4);
-        sigs.push_back(AugSchemeMPL().Sign(sk, messageBytes));
+        G2Element sig = AugSchemeMPL().Sign(sk, messageBytes);
+        sigs.push_back(sig);
     }
-
     auto start = startStopwatch();
     for (int i = 0; i < numIters; i++) {
         uint8_t message[4];
         Util::IntToFourBytes(message, i);
         vector<uint8_t> messageBytes(message, message + 4);
         bool ok = AugSchemeMPL().Verify(pk, messageBytes, sigs[i]);
         ASSERT(ok);
     }
     endStopwatch(testName, start, numIters);
 }
 
-void benchBatchVerification() {
+void benchBatchVerification()
+{
     const int numIters = 100000;
 
     vector<vector<uint8_t>> sig_bytes;
     vector<vector<uint8_t>> pk_bytes;
     vector<vector<uint8_t>> ms;
 
     for (int i = 0; i < numIters; i++) {
@@ -110,15 +119,16 @@
 
     start = startStopwatch();
     bool ok = AugSchemeMPL().AggregateVerify(pks, ms, aggSig);
     ASSERT(ok);
     endStopwatch("Batch verification", start, numIters);
 }
 
-void benchFastAggregateVerification() {
+void benchFastAggregateVerification()
+{
     const int numIters = 5000;
 
     vector<G2Element> sigs;
     vector<G1Element> pks;
     vector<uint8_t> message = {1, 2, 3, 4, 5, 6, 7, 8};
     vector<G2Element> pops;
 
@@ -130,27 +140,27 @@
         pks.push_back(pk);
     }
 
     auto start = startStopwatch();
     G2Element aggSig = PopSchemeMPL().Aggregate(sigs);
     endStopwatch("PopScheme Aggregation", start, numIters);
 
-
     start = startStopwatch();
     for (int i = 0; i < numIters; i++) {
         bool ok = PopSchemeMPL().PopVerify(pks[i], pops[i]);
         ASSERT(ok);
     }
     endStopwatch("PopScheme Proofs verification", start, numIters);
 
     start = startStopwatch();
     bool ok = PopSchemeMPL().FastAggregateVerify(pks, message, aggSig);
     ASSERT(ok);
     endStopwatch("PopScheme verification", start, numIters);
 }
 
-int main(int argc, char* argv[]) {
+int main(int argc, char* argv[])
+{
     benchSigs();
     benchVerification();
     benchBatchVerification();
     benchFastAggregateVerification();
 }
```

### Comparing `blspy-1.0.9/src/test-utils.hpp` & `blspy-2.0.0b1/src/test-utils.hpp`

 * *Files 6% similar despite different names*

```diff
@@ -43,14 +43,14 @@
          << " ms" << endl;
     cout << "Avg: " << now_ms.count() / static_cast<double>(numIters)
          << " ms" << endl;
 }
 
 std::vector<uint8_t> getRandomSeed() {
     uint8_t buf[32];
-    bn_t r;
-    bn_new(r);
-    bn_rand(r, RLC_POS, 256);
-    bn_write_bin(buf, 32, r);
+
+    for (int i = 0; i < 32; i++)
+        buf[i] = rand ();
+
     std::vector<uint8_t> ret(buf, buf + 32);
     return ret;
 }
```

### Comparing `blspy-1.0.9/src/test.cpp` & `blspy-2.0.0b1/src/test.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -9,76 +9,85 @@
 
 // Unless required by applicable law or agreed to in writing, software
 // distributed under the License is distributed on an "AS IS" BASIS,
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.
 
-#define CATCH_CONFIG_RUNNER
-#include <catch2/catch.hpp>
-
+#include <catch2/catch_session.hpp>
+#include <catch2/catch_test_macros.hpp>
 #include <thread>
 
 #include "bls.hpp"
 extern "C" {
-#include "relic.h"
+// #include "relic.h"
 }
 #include "test-utils.hpp"
 using std::cout;
 using std::endl;
 using std::string;
 using std::vector;
 
 using namespace bls;
 
-void TestHKDF(string ikm_hex, string salt_hex, string info_hex, string prk_expected_hex, string okm_expected_hex, int L) {
+void TestHKDF(
+    string ikm_hex,
+    string salt_hex,
+    string info_hex,
+    string prk_expected_hex,
+    string okm_expected_hex,
+    int L)
+{
     vector<uint8_t> ikm = Util::HexToBytes(ikm_hex);
     vector<uint8_t> salt = Util::HexToBytes(salt_hex);
     vector<uint8_t> info = Util::HexToBytes(info_hex);
     vector<uint8_t> prk_expected = Util::HexToBytes(prk_expected_hex);
     vector<uint8_t> okm_expected = Util::HexToBytes(okm_expected_hex);
     uint8_t prk[32];
     HKDF256::Extract(prk, salt.data(), salt.size(), ikm.data(), ikm.size());
     uint8_t* okm = new uint8_t[L];
     HKDF256::Expand(okm, L, prk, info.data(), info.size());
 
     REQUIRE(32 == prk_expected.size());
-    REQUIRE(L == okm_expected.size());
+    REQUIRE(L == (int)okm_expected.size());
 
-    for (size_t i=0; i < 32; i++) {
+    for (size_t i = 0; i < 32; i++) {
         REQUIRE(prk[i] == prk_expected[i]);
     }
-    for (size_t i=0; i < L; i++) {
+    for (int i = 0; i < L; i++) {
         REQUIRE(okm[i] == okm_expected[i]);
     }
 
     delete[] okm;
 }
 
-TEST_CASE("class PrivateKey") {
+TEST_CASE("class PrivateKey")
+{
     uint8_t buffer[PrivateKey::PRIVATE_KEY_SIZE];
-    memcmp(buffer, getRandomSeed().data(), PrivateKey::PRIVATE_KEY_SIZE);
-    SECTION("Copy {constructor|assignment operator}") {
+    memcpy(buffer, getRandomSeed().data(), PrivateKey::PRIVATE_KEY_SIZE);
+    SECTION("Copy {constructor|assignment operator}")
+    {
         PrivateKey pk1 = PrivateKey::FromByteVector(getRandomSeed(), true);
         PrivateKey pk2 = PrivateKey::FromByteVector(getRandomSeed(), true);
         PrivateKey pk3 = PrivateKey(pk2);
         REQUIRE(!pk1.IsZero());
         REQUIRE(!pk2.IsZero());
         REQUIRE(!pk3.IsZero());
         REQUIRE(pk1 != pk2);
         REQUIRE(pk3 == pk2);
-        REQUIRE(pk2.GetG1Element().IsValid()); // cache previous g1
-        REQUIRE(pk2.GetG2Element().IsValid()); // cache previous g2
+        REQUIRE(pk2.GetG1Element().IsValid());  // cache previous g1
+        REQUIRE(pk2.GetG2Element().IsValid());  // cache previous g2
         pk2 = pk1;
         REQUIRE(pk1 == pk2);
         REQUIRE(pk1.GetG1Element() == pk2.GetG1Element());
         REQUIRE(pk1.GetG2Element() == pk2.GetG2Element());
         REQUIRE(pk3 != pk2);
     }
-    SECTION("Move {constructor|assignment operator}") {
+    SECTION("Move {constructor|assignment operator}")
+    {
         PrivateKey pk1 = PrivateKey::FromByteVector(getRandomSeed(), true);
         std::vector<uint8_t> vec1 = pk1.Serialize();
         PrivateKey pk2 = PrivateKey::FromByteVector(getRandomSeed(), true);
         std::vector<uint8_t> vec2 = pk2.Serialize();
         PrivateKey pk3 = PrivateKey(std::move(pk2));
         REQUIRE(!pk1.IsZero());
         REQUIRE_THROWS(pk2.IsZero());
@@ -90,43 +99,58 @@
         REQUIRE(!pk3.IsZero());
         REQUIRE(vec1 == pk3.Serialize());
         pk3 = std::move(pk1);
         REQUIRE_THROWS(pk1.IsZero());
         REQUIRE_THROWS(pk2.IsZero());
         REQUIRE_THROWS(pk3.IsZero());
     }
-    SECTION("Equality operators") {
+    SECTION("Equality operators")
+    {
         PrivateKey pk1 = PrivateKey::FromByteVector(getRandomSeed(), true);
         PrivateKey pk2 = PrivateKey::FromByteVector(getRandomSeed(), true);
         PrivateKey pk3 = pk2;
         REQUIRE(pk1 != pk2);
         REQUIRE(pk1 != pk3);
         REQUIRE(pk2 == pk3);
     }
-    SECTION("(De)Serialization") {
+    SECTION("(De)Serialization")
+    {
         PrivateKey pk1 = PrivateKey::FromByteVector(getRandomSeed(), true);
         pk1.Serialize(buffer);
-        REQUIRE(memcmp(buffer, pk1.Serialize().data(), PrivateKey::PRIVATE_KEY_SIZE) == 0);
-        PrivateKey pk2 = PrivateKey:: FromBytes(Bytes(buffer, PrivateKey::PRIVATE_KEY_SIZE), true);
+        REQUIRE(
+            memcmp(
+                buffer, pk1.Serialize().data(), PrivateKey::PRIVATE_KEY_SIZE) ==
+            0);
+        PrivateKey pk2 = PrivateKey::FromBytes(
+            Bytes(buffer, PrivateKey::PRIVATE_KEY_SIZE), true);
         REQUIRE(pk1 == pk2);
-        REQUIRE_THROWS(PrivateKey::FromBytes(Bytes(buffer, PrivateKey::PRIVATE_KEY_SIZE - 1), true));
-        REQUIRE_THROWS(PrivateKey::FromBytes(Bytes(buffer, PrivateKey::PRIVATE_KEY_SIZE + 1), true));
-        REQUIRE_NOTHROW(PrivateKey::FromBytes(Bytes(buffer, PrivateKey::PRIVATE_KEY_SIZE), true));
-        bn_t order;
-        bn_new(order);
-        g1_get_ord(order);
-        bn_write_bin(buffer, PrivateKey::PRIVATE_KEY_SIZE, order);
-        REQUIRE_NOTHROW(PrivateKey::FromBytes(Bytes(buffer, PrivateKey::PRIVATE_KEY_SIZE), false));
-        REQUIRE_NOTHROW(PrivateKey::FromBytes(Bytes(buffer, PrivateKey::PRIVATE_KEY_SIZE), true));
-        bn_add(order, order, order);
-        bn_write_bin(buffer, PrivateKey::PRIVATE_KEY_SIZE, order);
-        REQUIRE_THROWS(PrivateKey::FromBytes(Bytes(buffer, PrivateKey::PRIVATE_KEY_SIZE), false));
-        REQUIRE_NOTHROW(PrivateKey::FromBytes(Bytes(buffer, PrivateKey::PRIVATE_KEY_SIZE), true));
+        REQUIRE_THROWS(PrivateKey::FromBytes(
+            Bytes(buffer, PrivateKey::PRIVATE_KEY_SIZE - 1), true));
+        REQUIRE_THROWS(PrivateKey::FromBytes(
+            Bytes(buffer, PrivateKey::PRIVATE_KEY_SIZE + 1), true));
+        REQUIRE_NOTHROW(PrivateKey::FromBytes(
+            Bytes(buffer, PrivateKey::PRIVATE_KEY_SIZE), true));
+        // blst_scalar order;
+        // memcpy(&order, BLS12_381_r, sizeof(blst_scalar));
+        //  g1_get_ord(order);
+        //  bn_write_bin(buffer, PrivateKey::PRIVATE_KEY_SIZE, order);
+        // REQUIRE_NOTHROW(PrivateKey::FromBytes(
+        //     Bytes(buffer, PrivateKey::PRIVATE_KEY_SIZE), false));
+        // REQUIRE_NOTHROW(PrivateKey::FromBytes(
+        //     Bytes(buffer, PrivateKey::PRIVATE_KEY_SIZE), true));
+        // blst_sk_add_n_check(&order, &order, &order);
+        //  bn_add(order, order, order);
+        //  bn_write_bin(buffer, PrivateKey::PRIVATE_KEY_SIZE, order);
+        // REQUIRE_THROWS(PrivateKey::FromBytes(
+        //     Bytes(buffer, PrivateKey::PRIVATE_KEY_SIZE), false));
+        // REQUIRE_NOTHROW(PrivateKey::FromBytes(
+        //    Bytes(buffer, PrivateKey::PRIVATE_KEY_SIZE), true));
     }
-    SECTION("keydata checks") {
+    SECTION("keydata checks")
+    {
         PrivateKey pk1 = PrivateKey::FromByteVector(getRandomSeed(), true);
         G1Element g1 = pk1.GetG1Element();
         G2Element g2 = pk1.GetG2Element();
         PrivateKey pk2 = std::move(pk1);
         REQUIRE_THROWS(PrivateKey(pk1));
         REQUIRE_THROWS(pk1 = pk2);
         REQUIRE_THROWS(pk1.GetG1Element());
@@ -138,204 +162,246 @@
         REQUIRE_THROWS(pk1.GetG2Power(g2));
         REQUIRE_THROWS(PrivateKey::Aggregate({pk1, pk2}));
         REQUIRE_THROWS(pk1.IsZero());
         REQUIRE_THROWS(pk1 == pk2);
         REQUIRE_THROWS(pk1 != pk2);
         REQUIRE_THROWS(pk1.Serialize(buffer));
         REQUIRE_THROWS(pk1.Serialize());
-        REQUIRE_THROWS(pk1.SignG2(buffer, sizeof(buffer), buffer, sizeof(buffer)));
+        REQUIRE_THROWS(
+            pk1.SignG2(buffer, sizeof(buffer), buffer, sizeof(buffer)));
     }
 }
 
-TEST_CASE("HKDF") {
+TEST_CASE("HKDF")
+{
     // https://tools.ietf.org/html/rfc5869 test vectors
-    SECTION("Test case 2") {
-        TestHKDF("0b0b0b0b0b0b0b0b0b0b0b0b0b0b0b0b0b0b0b0b0b0b",
-                 "000102030405060708090a0b0c",
-                 "f0f1f2f3f4f5f6f7f8f9",
-                 "077709362c2e32df0ddc3f0dc47bba6390b6c73bb50f9c3122ec844ad7c2b3e5",
-                 "3cb25f25faacd57a90434f64d0362f2a2d2d0a90cf1a5a4c5db02d56ecc4c5bf34007208d5b887185865",
-                 42
-        );
-    }
-    SECTION("Test case 2") {
-        TestHKDF("000102030405060708090a0b0c0d0e0f"
-                 "101112131415161718191a1b1c1d1e1f"
-                 "202122232425262728292a2b2c2d2e2f"
-                 "303132333435363738393a3b3c3d3e3f"
-                 "404142434445464748494a4b4c4d4e4f", // 80 octets
-                 "0x606162636465666768696a6b6c6d6e6f"
-                 "707172737475767778797a7b7c7d7e7f"
-                 "808182838485868788898a8b8c8d8e8f"
-                 "909192939495969798999a9b9c9d9e9f"
-                 "a0a1a2a3a4a5a6a7a8a9aaabacadaeaf", // 80 octets
-                 "0xb0b1b2b3b4b5b6b7b8b9babbbcbdbebf"
-                 "c0c1c2c3c4c5c6c7c8c9cacbcccdcecf"
-                 "d0d1d2d3d4d5d6d7d8d9dadbdcdddedf"
-                 "e0e1e2e3e4e5e6e7e8e9eaebecedeeef"
-                 "f0f1f2f3f4f5f6f7f8f9fafbfcfdfeff", // 80 octets
-                 "0x06a6b88c5853361a06104c9ceb35b45cef760014904671014a193f40c15fc244", // 32 octets
-                 "0xb11e398dc80327a1c8e7f78c596a4934"
-                 "4f012eda2d4efad8a050cc4c19afa97c"
-                 "59045a99cac7827271cb41c65e590e09"
-                 "da3275600c2f09b8367793a9aca3db71"
-                 "cc30c58179ec3e87c14c01d5c1f3434f"
-                 "1d87", // 82 octets
-                 82
-        );
-    }
-    SECTION("Test case 3") {
-        TestHKDF("0b0b0b0b0b0b0b0b0b0b0b0b0b0b0b0b0b0b0b0b0b0b",
-                 "",
-                 "",
-                 "19ef24a32c717b167f33a91d6f648bdf96596776afdb6377ac434c1c293ccb04",
-                 "8da4e775a563c18f715f802a063c5a31b8a11f5c5ee1879ec3454e5f3c738d2d9d201395faa4b61a96c8",
-                 42
-        );
-    }
-    SECTION("Works with multiple of 32") {
-        // This generates exactly 64 bytes. Uses a 32 byte key and 4 byte salt as in EIP2333.
-        TestHKDF("8704f9ac024139fe62511375cf9bc534c0507dcf00c41603ac935cd5943ce0b4b88599390de14e743ca2f56a73a04eae13aa3f3b969b39d8701e0d69a6f8d42f",
-                 "53d8e19b",
-                 "",
-                 "eb01c9cd916653df76ffa61b6ab8a74e254ebfd9bfc43e624cc12a72b0373dee",
-                 "8faabea85fc0c64e7ca86217cdc6dcdc88551c3244d56719e630a3521063082c46455c2fd5483811f9520a748f0099c1dfcfa52c54e1c22b5cdf70efb0f3c676",
-                 64
-        );
+    SECTION("Test case 2")
+    {
+        TestHKDF(
+            "0b0b0b0b0b0b0b0b0b0b0b0b0b0b0b0b0b0b0b0b0b0b",
+            "000102030405060708090a0b0c",
+            "f0f1f2f3f4f5f6f7f8f9",
+            "077709362c2e32df0ddc3f0dc47bba6390b6c73bb50f9c3122ec844ad7c2b3e5",
+            "3cb25f25faacd57a90434f64d0362f2a2d2d0a90cf1a5a4c5db02d56ecc4c5bf34"
+            "007208d5b887185865",
+            42);
+    }
+    SECTION("Test case 2")
+    {
+        TestHKDF(
+            "000102030405060708090a0b0c0d0e0f"
+            "101112131415161718191a1b1c1d1e1f"
+            "202122232425262728292a2b2c2d2e2f"
+            "303132333435363738393a3b3c3d3e3f"
+            "404142434445464748494a4b4c4d4e4f",  // 80 octets
+            "0x606162636465666768696a6b6c6d6e6f"
+            "707172737475767778797a7b7c7d7e7f"
+            "808182838485868788898a8b8c8d8e8f"
+            "909192939495969798999a9b9c9d9e9f"
+            "a0a1a2a3a4a5a6a7a8a9aaabacadaeaf",  // 80 octets
+            "0xb0b1b2b3b4b5b6b7b8b9babbbcbdbebf"
+            "c0c1c2c3c4c5c6c7c8c9cacbcccdcecf"
+            "d0d1d2d3d4d5d6d7d8d9dadbdcdddedf"
+            "e0e1e2e3e4e5e6e7e8e9eaebecedeeef"
+            "f0f1f2f3f4f5f6f7f8f9fafbfcfdfeff",  // 80 octets
+            "0x06a6b88c5853361a06104c9ceb35b45cef760014904671014a193f40c15fc24"
+            "4",  // 32 octets
+            "0xb11e398dc80327a1c8e7f78c596a4934"
+            "4f012eda2d4efad8a050cc4c19afa97c"
+            "59045a99cac7827271cb41c65e590e09"
+            "da3275600c2f09b8367793a9aca3db71"
+            "cc30c58179ec3e87c14c01d5c1f3434f"
+            "1d87",  // 82 octets
+            82);
+    }
+    SECTION("Test case 3")
+    {
+        TestHKDF(
+            "0b0b0b0b0b0b0b0b0b0b0b0b0b0b0b0b0b0b0b0b0b0b",
+            "",
+            "",
+            "19ef24a32c717b167f33a91d6f648bdf96596776afdb6377ac434c1c293ccb04",
+            "8da4e775a563c18f715f802a063c5a31b8a11f5c5ee1879ec3454e5f3c738d2d9d"
+            "201395faa4b61a96c8",
+            42);
+    }
+    SECTION("Works with multiple of 32")
+    {
+        // This generates exactly 64 bytes. Uses a 32 byte key and 4 byte salt
+        // as in EIP2333.
+        TestHKDF(
+            "8704f9ac024139fe62511375cf9bc534c0507dcf00c41603ac935cd5943ce0b4b8"
+            "8599390de14e743ca2f56a73a04eae13aa3f3b969b39d8701e0d69a6f8d42f",
+            "53d8e19b",
+            "",
+            "eb01c9cd916653df76ffa61b6ab8a74e254ebfd9bfc43e624cc12a72b0373dee",
+            "8faabea85fc0c64e7ca86217cdc6dcdc88551c3244d56719e630a3521063082c46"
+            "455c2fd5483811f9520a748f0099c1dfcfa52c54e1c22b5cdf70efb0f3c676",
+            64);
     }
 }
 
-void TestEIP2333(string seedHex, string masterSkHex, string childSkHex, uint32_t childIndex) {
+void TestEIP2333(
+    string seedHex,
+    string masterSkHex,
+    string childSkHex,
+    uint32_t childIndex)
+{
     auto masterSk = Util::HexToBytes(masterSkHex);
     auto childSk = Util::HexToBytes(childSkHex);
 
     PrivateKey master = BasicSchemeMPL().KeyGen(Util::HexToBytes(seedHex));
     PrivateKey child = HDKeys::DeriveChildSk(master, childIndex);
 
     uint8_t master_arr[32];
     master.Serialize(master_arr);
     auto calculatedMaster = master.Serialize();
     auto calculatedChild = child.Serialize();
 
     REQUIRE(calculatedMaster.size() == 32);
     REQUIRE(calculatedChild.size() == 32);
-    for (int i=0; i<32; i++) {
+    for (int i = 0; i < 32; i++) {
         REQUIRE(calculatedMaster[i] == masterSk[i]);
     }
-    for (int i=0; i<32; i++) {
+    for (int i = 0; i < 32; i++) {
         REQUIRE(calculatedChild[i] == childSk[i]);
     }
 }
 
-TEST_CASE("EIP-2333 hardened HD keys") {
-    // The comments in the test cases correspond to  integers that are converted to
-    // bytes using python int.to_bytes(32, "big").hex(), since the EIP spec provides ints, but c++
-    // does not support bigint by default
-    SECTION("EIP-2333 Test case 1"){
-        TestEIP2333("3141592653589793238462643383279502884197169399375105820974944592",
-                    // 36167147331491996618072159372207345412841461318189449162487002442599770291484
-                    "4ff5e145590ed7b71e577bb04032396d1619ff41cb4e350053ed2dce8d1efd1c",
-                    // 41787458189896526028601807066547832426569899195138584349427756863968330588237
-                    "5c62dcf9654481292aafa3348f1d1b0017bbfb44d6881d26d2b17836b38f204d",
-                    3141592653
-        );
-    }
-    SECTION("EIP-2333 Test case 2"){
-        TestEIP2333("0x0099FF991111002299DD7744EE3355BBDD8844115566CC55663355668888CC00",
-                    // 13904094584487173309420026178174172335998687531503061311232927109397516192843
-                    "1ebd704b86732c3f05f30563dee6189838e73998ebc9c209ccff422adee10c4b",
-                    // 12482522899285304316694838079579801944734479969002030150864436005368716366140
-                    "1b98db8b24296038eae3f64c25d693a269ef1e4d7ae0f691c572a46cf3c0913c",
-                    4294967295
-        );
-    }
-    SECTION("EIP-2333 Test case 3"){
-        TestEIP2333("0xd4e56740f876aef8c010b86a40d5f56745a118d0906a34e69aec8c0db1cb8fa3",
-                    // 44010626067374404458092393860968061149521094673473131545188652121635313364506
-                    "614d21b10c0e4996ac0608e0e7452d5720d95d20fe03c59a3321000a42432e1a",
-                    // 4011524214304750350566588165922015929937602165683407445189263506512578573606
-                    "08de7136e4afc56ae3ec03b20517d9c1232705a747f588fd17832f36ae337526",
-                    42
-        );
-    }
-    SECTION("EIP-2333 Test vector with intermediate values"){
-        TestEIP2333("c55257c360c07c72029aebc1b53c05ed0362ada38ead3e3e9efa3708e53495531f09a6987599d18264c1e1c92f2cf141630c7a3c4ab7c81b2f001698e7463b04",
-                    // 5399117110774477986698372024995405256382522670366369834617409486544348441851
-                    "0x0befcabff4a664461cc8f190cdd51c05621eb2837c71a1362df5b465a674ecfb",
-                    // 11812940737387919040225825939013910852517748782307378293770044673328955938106
-                    "1a1de3346883401f1e3b2281be5774080edb8e5ebe6f776b0f7af9fea942553a",
-                    0
-        );
+TEST_CASE("EIP-2333 hardened HD keys")
+{
+    // The comments in the test cases correspond to  integers that are converted
+    // to bytes using python int.to_bytes(32, "big").hex(), since the EIP spec
+    // provides ints, but c++ does not support bigint by default
+    SECTION("EIP-2333 Test case 1")
+    {
+        TestEIP2333(
+            "3141592653589793238462643383279502884197169399375105820974944592",
+            // 36167147331491996618072159372207345412841461318189449162487002442599770291484
+            "4ff5e145590ed7b71e577bb04032396d1619ff41cb4e350053ed2dce8d1efd1c",
+            // 41787458189896526028601807066547832426569899195138584349427756863968330588237
+            "5c62dcf9654481292aafa3348f1d1b0017bbfb44d6881d26d2b17836b38f204d",
+            3141592653);
+    }
+    SECTION("EIP-2333 Test case 2")
+    {
+        TestEIP2333(
+            "0x0099FF991111002299DD7744EE3355BBDD8844115566CC55663355668888CC0"
+            "0",
+            // 13904094584487173309420026178174172335998687531503061311232927109397516192843
+            "1ebd704b86732c3f05f30563dee6189838e73998ebc9c209ccff422adee10c4b",
+            // 12482522899285304316694838079579801944734479969002030150864436005368716366140
+            "1b98db8b24296038eae3f64c25d693a269ef1e4d7ae0f691c572a46cf3c0913c",
+            4294967295);
+    }
+    SECTION("EIP-2333 Test case 3")
+    {
+        TestEIP2333(
+            "0xd4e56740f876aef8c010b86a40d5f56745a118d0906a34e69aec8c0db1cb8fa"
+            "3",
+            // 44010626067374404458092393860968061149521094673473131545188652121635313364506
+            "614d21b10c0e4996ac0608e0e7452d5720d95d20fe03c59a3321000a42432e1a",
+            // 4011524214304750350566588165922015929937602165683407445189263506512578573606
+            "08de7136e4afc56ae3ec03b20517d9c1232705a747f588fd17832f36ae337526",
+            42);
+    }
+    SECTION("EIP-2333 Test vector with intermediate values")
+    {
+        TestEIP2333(
+            "c55257c360c07c72029aebc1b53c05ed0362ada38ead3e3e9efa3708e53495531f"
+            "09a6987599d18264c1e1c92f2cf141630c7a3c4ab7c81b2f001698e7463b04",
+            // 5399117110774477986698372024995405256382522670366369834617409486544348441851
+            "0x0befcabff4a664461cc8f190cdd51c05621eb2837c71a1362df5b465a674ecf"
+            "b",
+            // 11812940737387919040225825939013910852517748782307378293770044673328955938106
+            "1a1de3346883401f1e3b2281be5774080edb8e5ebe6f776b0f7af9fea942553a",
+            0);
     }
 }
 
-TEST_CASE("Unhardened HD keys") {
-    SECTION("Should match derivation through private and public keys"){
-        const vector<uint8_t> seed = {1, 50, 6, 244, 24, 199, 1, 25, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15,
-                                            16, 17, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27, 28, 29};
+TEST_CASE("Unhardened HD keys")
+{
+    SECTION("Should match derivation through private and public keys")
+    {
+        const vector<uint8_t> seed = {1,  50, 6,  244, 24, 199, 1,  25, 1,  2,
+                                      3,  4,  5,  6,   7,  8,   9,  10, 11, 12,
+                                      13, 14, 15, 16,  17, 18,  19, 20, 21, 22,
+                                      23, 24, 25, 26,  27, 28,  29};
 
         PrivateKey sk = BasicSchemeMPL().KeyGen(seed);
         G1Element pk = sk.GetG1Element();
 
         PrivateKey childSk = BasicSchemeMPL().DeriveChildSkUnhardened(sk, 42);
         G1Element childPk = BasicSchemeMPL().DeriveChildPkUnhardened(pk, 42);
 
         REQUIRE(childSk.GetG1Element() == childPk);
 
-        PrivateKey grandchildSk = BasicSchemeMPL().DeriveChildSkUnhardened(childSk, 12142);
-        G1Element grandcihldPk = BasicSchemeMPL().DeriveChildPkUnhardened(childPk, 12142);
+        PrivateKey grandchildSk =
+            BasicSchemeMPL().DeriveChildSkUnhardened(childSk, 12142);
+        G1Element grandchildPk =
+            BasicSchemeMPL().DeriveChildPkUnhardened(childPk, 12142);
 
-        REQUIRE(grandchildSk.GetG1Element() == grandcihldPk);
+        REQUIRE(grandchildSk.GetG1Element() == grandchildPk);
     }
 
-    SECTION("Should derive public child from parent") {
-        const vector<uint8_t> seed = {2, 50, 6, 244, 24, 199, 1, 25, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15,
-                                            16, 17, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27, 28, 29};
+    SECTION("Should derive public child from parent")
+    {
+        const vector<uint8_t> seed = {2,  50, 6,  244, 24, 199, 1,  25, 1,  2,
+                                      3,  4,  5,  6,   7,  8,   9,  10, 11, 12,
+                                      13, 14, 15, 16,  17, 18,  19, 20, 21, 22,
+                                      23, 24, 25, 26,  27, 28,  29};
 
         PrivateKey sk = BasicSchemeMPL().KeyGen(seed);
         G1Element pk = sk.GetG1Element();
 
         PrivateKey childSk = BasicSchemeMPL().DeriveChildSkUnhardened(sk, 42);
         G1Element childPk = BasicSchemeMPL().DeriveChildPkUnhardened(pk, 42);
 
         PrivateKey childSkHardened = BasicSchemeMPL().DeriveChildSk(sk, 42);
         REQUIRE(childSk.GetG1Element() == childPk);
         REQUIRE(childSkHardened != childSk);
         REQUIRE(childSkHardened.GetG1Element() != childPk);
     }
 }
 
-TEST_CASE("IETF test vectors") {
-    SECTION ("Pyecc vector") {
-        string sig1BasicHex = "96ba34fac33c7f129d602a0bc8a3d43f9abc014eceaab7359146b4b150e57b808645738f35671e9e10e0d862a30cab70074eb5831d13e6a5b162d01eebe687d0164adbd0a864370a7c222a2768d7704da254f1bf1823665bc2361f9dd8c00e99";
-        string sk = "0x0101010101010101010101010101010101010101010101010101010101010101";
+TEST_CASE("IETF test vectors")
+{
+    SECTION("Pyecc vector")
+    {
+        string sig1BasicHex =
+            "96ba34fac33c7f129d602a0bc8a3d43f9abc014eceaab7359146b4b150e57b8086"
+            "45738f35671e9e10e0d862a30cab70074eb5831d13e6a5b162d01eebe687d0164a"
+            "dbd0a864370a7c222a2768d7704da254f1bf1823665bc2361f9dd8c00e99";
+        string sk =
+            "0x010101010101010101010101010101010101010101010101010101010101010"
+            "1";
         vector<uint8_t> msg = {3, 1, 4, 1, 5, 9};
         auto skobj = PrivateKey::FromBytes(Bytes(Util::HexToBytes(sk)));
         G2Element sig = BasicSchemeMPL().Sign(skobj, msg);
         vector<uint8_t> sig1;
         for (const uint8_t byte : Util::HexToBytes(sig1BasicHex)) {
             sig1.push_back(byte);
         }
         REQUIRE(sig == G2Element::FromByteVector(sig1));
     }
 }
 
-
-TEST_CASE("Chia test vectors") {
-    SECTION("Chia test vectors 1 (Basic)") {
+TEST_CASE("Chia test vectors")
+{
+    SECTION("Chia test vectors 1 (Basic)")
+    {
         vector<uint8_t> seed1(32, 0x00);  // All 0s
         vector<uint8_t> seed2(32, 0x01);  // All 1s
         vector<uint8_t> message1 = {7, 8, 9};
         vector<uint8_t> message2 = {10, 11, 12};
 
         PrivateKey sk1 = BasicSchemeMPL().KeyGen(seed1);
         G1Element pk1 = sk1.GetG1Element();
         G2Element sig1 = BasicSchemeMPL().Sign(sk1, message1);
 
-
         PrivateKey sk2 = BasicSchemeMPL().KeyGen(seed2);
         G1Element pk2 = sk2.GetG1Element();
         G2Element sig2 = BasicSchemeMPL().Sign(sk2, message2);
 
         REQUIRE(pk1.GetFingerprint() == 0xb40dd58a);
         REQUIRE(pk2.GetFingerprint() == 0xb839add1);
 
@@ -345,55 +411,68 @@
             "fa3ab6ee21c71f844494659878f5eb230c958dd576b08b8564aad2ee0992e85a"
             "1e565f299cd53a285de729937f70dc176a1f01432129bb2b94d3d5031f8065a1");
         REQUIRE(
             Util::HexStr(sk1.Serialize()) ==
             "4a353be3dac091a0a7e640620372f5e1e2e4401717c1e79cac6ffba8f6905604");
         REQUIRE(
             Util::HexStr(pk1.Serialize()) ==
-            "85695fcbc06cc4c4c9451f4dce21cbf8de3e5a13bf48f44cdbb18e2038ba7b8bb1632d7911e"
+            "85695fcbc06cc4c4c9451f4dce21cbf8de3e5a13bf48f44cdbb18e2038ba7b8bb1"
+            "632d7911e"
             "f1e2e08749bddbf165352");
 
         REQUIRE(
             Util::HexStr(sig2.Serialize()) ==
-            "a9c4d3e689b82c7ec7e838dac2380cb014f9a08f6cd6ba044c263746e39a8f7a60ffee4afb7"
-            "8f146c2e421360784d58f0029491e3bd8ab84f0011d258471ba4e87059de295d9aba845c044e"
+            "a9c4d3e689b82c7ec7e838dac2380cb014f9a08f6cd6ba044c263746e39a8f7a60"
+            "ffee4afb7"
+            "8f146c2e421360784d58f0029491e3bd8ab84f0011d258471ba4e87059de295d9a"
+            "ba845c044e"
             "e83f6cf2411efd379ef38bf4cf41d5f3c0ae1205d");
 
         G2Element aggSig1 = BasicSchemeMPL().Aggregate({sig1, sig2});
 
         REQUIRE(
             Util::HexStr(aggSig1.Serialize()) ==
-            "aee003c8cdaf3531b6b0ca354031b0819f7586b5846796615aee8108fec75ef838d181f9d24"
-            "4a94d195d7b0231d4afcf06f27f0cc4d3c72162545c240de7d5034a7ef3a2a03c0159de982fb"
+            "aee003c8cdaf3531b6b0ca354031b0819f7586b5846796615aee8108fec75ef838"
+            "d181f9d24"
+            "4a94d195d7b0231d4afcf06f27f0cc4d3c72162545c240de7d5034a7ef3a2a03c0"
+            "159de982fb"
             "c2e7790aeb455e27beae91d64e077c70b5506dea3");
 
-        REQUIRE(BasicSchemeMPL().AggregateVerify({pk1, pk2}, vector<vector<uint8_t>>{message1, message2}, aggSig1));
-        REQUIRE(!BasicSchemeMPL().AggregateVerify({pk1, pk2}, vector<vector<uint8_t>>{message1, message2}, sig1));
+        REQUIRE(BasicSchemeMPL().AggregateVerify(
+            {pk1, pk2}, vector<vector<uint8_t>>{message1, message2}, aggSig1));
+        REQUIRE(!BasicSchemeMPL().AggregateVerify(
+            {pk1, pk2}, vector<vector<uint8_t>>{message1, message2}, sig1));
         REQUIRE(!BasicSchemeMPL().Verify(pk1, message1, sig2));
         REQUIRE(!BasicSchemeMPL().Verify(pk1, message2, sig1));
 
         vector<uint8_t> message3 = {1, 2, 3};
         vector<uint8_t> message4 = {1, 2, 3, 4};
         vector<uint8_t> message5 = {1, 2};
 
         G2Element sig3 = BasicSchemeMPL().Sign(sk1, message3);
         G2Element sig4 = BasicSchemeMPL().Sign(sk1, message4);
         G2Element sig5 = BasicSchemeMPL().Sign(sk2, message5);
 
         G2Element aggSig2 = BasicSchemeMPL().Aggregate({sig3, sig4, sig5});
 
-        REQUIRE(BasicSchemeMPL().AggregateVerify({pk1, pk1, pk2}, vector<vector<uint8_t>>{message3, message4, message5}, aggSig2));
+        REQUIRE(BasicSchemeMPL().AggregateVerify(
+            {pk1, pk1, pk2},
+            vector<vector<uint8_t>>{message3, message4, message5},
+            aggSig2));
         REQUIRE(
             Util::HexStr(aggSig2.Serialize()) ==
-            "a0b1378d518bea4d1100adbc7bdbc4ff64f2c219ed6395cd36fe5d2aa44a4b8e710b607afd9"
-            "65e505a5ac3283291b75413d09478ab4b5cfbafbeea366de2d0c0bcf61deddaa521f6020460f"
+            "a0b1378d518bea4d1100adbc7bdbc4ff64f2c219ed6395cd36fe5d2aa44a4b8e71"
+            "0b607afd9"
+            "65e505a5ac3283291b75413d09478ab4b5cfbafbeea366de2d0c0bcf61deddaa52"
+            "1f6020460f"
             "d547ab37659ae207968b545727beba0a3c5572b9c");
     }
 
-    SECTION("Chia test vector 2 (Augmented, aggregate of aggregates)") {
+    SECTION("Chia test vector 2 (Augmented, aggregate of aggregates)")
+    {
         vector<uint8_t> message1 = {1, 2, 3, 40};
         vector<uint8_t> message2 = {5, 6, 70, 201};
         vector<uint8_t> message3 = {9, 10, 11, 12, 13};
         vector<uint8_t> message4 = {15, 63, 244, 92, 0, 1};
 
         vector<uint8_t> seed1(32, 0x02);  // All 2s
         vector<uint8_t> seed2(32, 0x03);  // All 3s
@@ -407,132 +486,114 @@
         G2Element sig1 = AugSchemeMPL().Sign(sk1, message1);
         G2Element sig2 = AugSchemeMPL().Sign(sk2, message2);
         G2Element sig3 = AugSchemeMPL().Sign(sk2, message1);
         G2Element sig4 = AugSchemeMPL().Sign(sk1, message3);
         G2Element sig5 = AugSchemeMPL().Sign(sk1, message1);
         G2Element sig6 = AugSchemeMPL().Sign(sk1, message4);
 
-
         G2Element aggSigL = AugSchemeMPL().Aggregate({sig1, sig2});
         G2Element aggSigR = AugSchemeMPL().Aggregate({sig3, sig4, sig5});
         G2Element aggSig = AugSchemeMPL().Aggregate({aggSigL, aggSigR, sig6});
 
-        REQUIRE(AugSchemeMPL().AggregateVerify({pk1, pk2, pk2, pk1, pk1, pk1}, vector<vector<uint8_t>>{message1, message2, message1, message3, message1, message4}, aggSig));
+        REQUIRE(AugSchemeMPL().AggregateVerify(
+            {pk1, pk2, pk2, pk1, pk1, pk1},
+            vector<vector<uint8_t>>{
+                message1, message2, message1, message3, message1, message4},
+            aggSig));
 
         REQUIRE(
             Util::HexStr(aggSig.Serialize()) ==
-            "a1d5360dcb418d33b29b90b912b4accde535cf0e52caf467a005dc632d9f7af44b6c4e9acd4"
-            "6eac218b28cdb07a3e3bc087df1cd1e3213aa4e11322a3ff3847bbba0b2fd19ddc25ca964871"
+            "a1d5360dcb418d33b29b90b912b4accde535cf0e52caf467a005dc632d9f7af44b"
+            "6c4e9acd4"
+            "6eac218b28cdb07a3e3bc087df1cd1e3213aa4e11322a3ff3847bbba0b2fd19ddc"
+            "25ca964871"
             "997b9bceeab37a4c2565876da19382ea32a962200");
     }
-    SECTION("Chia test vector 3 (PoP)") {
+    SECTION("Chia test vector 3 (PoP)")
+    {
         vector<uint8_t> message1 = {1, 2, 3, 40, 50};
 
         vector<uint8_t> seed1(32, 0x04);  // All 4s
 
         PrivateKey sk1 = PopSchemeMPL().KeyGen(seed1);
 
         G2Element pop = PopSchemeMPL().PopProve(sk1);
         REQUIRE(PopSchemeMPL().PopVerify(sk1.GetG1Element(), pop));
 
-        REQUIRE(Util::HexStr(pop.Serialize()) == "84f709159435f0dc73b3e8bf6c78d85282d19231555a8ee3b6e2573aaf66872d9203fefa1ef"
-                                                 "700e34e7c3f3fb28210100558c6871c53f1ef6055b9f06b0d1abe22ad584ad3b957f3018a8f5"
-                                                 "8227c6c716b1e15791459850f2289168fa0cf9115");
+        REQUIRE(
+            Util::HexStr(pop.Serialize()) ==
+            "84f709159435f0dc73b3e8bf6c78d85282d19231555a8ee3b6e2573aaf66872d92"
+            "03fefa1ef"
+            "700e34e7c3f3fb28210100558c6871c53f1ef6055b9f06b0d1abe22ad584ad3b95"
+            "7f3018a8f5"
+            "8227c6c716b1e15791459850f2289168fa0cf9115");
     }
 }
 
-
 TEST_CASE("Key generation")
 {
     SECTION("Should generate a keypair from a seed")
     {
         vector<uint8_t> seed1(31, 0x08);
         vector<uint8_t> seed2(32, 0x08);
 
         REQUIRE_THROWS(BasicSchemeMPL().KeyGen(seed1));
         PrivateKey sk = BasicSchemeMPL().KeyGen(seed2);
         G1Element pk = sk.GetG1Element();
-        REQUIRE(core_get()->code == RLC_OK);
         REQUIRE(pk.GetFingerprint() == 0x8ee7ba56);
     }
 }
 
-
 TEST_CASE("Error handling")
 {
     SECTION("Should throw on a bad private key")
     {
         vector<uint8_t> seed(32, 0x10);
         PrivateKey sk1 = BasicSchemeMPL().KeyGen(seed);
         uint8_t* skData = Util::SecAlloc<uint8_t>(G2Element::SIZE);
         sk1.Serialize(skData);
         skData[0] = 255;
-        REQUIRE_THROWS(PrivateKey::FromBytes(Bytes(skData, PrivateKey::PRIVATE_KEY_SIZE)));
+        REQUIRE_THROWS(
+            PrivateKey::FromBytes(Bytes(skData, PrivateKey::PRIVATE_KEY_SIZE)));
         Util::SecFree(skData);
     }
 
     SECTION("Should throw on a bad public key")
     {
         vector<uint8_t> buf(G1Element::SIZE, 0);
         for (int i = 0; i < 0xFF; i++) {
             buf[0] = (uint8_t)i;
-            if (i == 0xc0) { // Infinity prefix shouldn't throw here as we have only zero values
+            if (i == 0xc0) {  // Infinity prefix shouldn't throw here as we have
+                              // only zero values
                 REQUIRE_NOTHROW(G1Element::FromByteVector(buf));
             } else {
                 REQUIRE_THROWS(G1Element::FromByteVector(buf));
             }
         }
     }
 
     SECTION("Should throw on a bad G2Element")
     {
         vector<uint8_t> buf(G2Element::SIZE, 0);
         for (int i = 0; i < 0xFF; i++) {
             buf[0] = (uint8_t)i;
-            if (i == 0xc0) { // Infinity prefix shouldn't throw here as we have only zero values
+            if (i == 0xc0) {  // Infinity prefix shouldn't throw here as we have
+                              // only zero values
                 REQUIRE_NOTHROW(G2Element::FromByteVector(buf));
             } else {
                 REQUIRE_THROWS(G2Element::FromByteVector(buf));
             }
         }
-        // Trigger "G2 element must always have 48th byte start with 0b000" error case
+        // Trigger "G2 element must always have 48th byte start with 0b000"
+        // error case
         buf[48] = 0xFF;
         REQUIRE_THROWS(G2Element::FromByteVector(buf));
     }
-
-    SECTION("Error handling should be thread safe")
-    {
-        core_get()->code = 10;
-        REQUIRE(core_get()->code == 10);
-
-        ctx_t* ctx1 = core_get();
-
-        // spawn a thread and make sure it uses a different/same context depending on relic's multithreading setup
-        std::thread([&]() {
-#if MULTI != RELIC_NONE
-            REQUIRE(ctx1 != core_get());
-            REQUIRE(core_get()->code == RLC_OK);
-#else
-            REQUIRE(ctx1 == core_get());
-            REQUIRE(core_get()->code != RLC_OK);
-#endif
-            core_get()->code = 1;
-        }).join();
-
-#if MULTI != RELIC_NONE
-        REQUIRE(core_get()->code == 10);
-#else
-        REQUIRE(core_get()->code == 1);
-#endif
-        // reset so that future test cases don't fail
-        core_get()->code = RLC_OK;
-    }
 }
 
-
 TEST_CASE("Util tests")
 {
     SECTION("Should convert an int to four bytes")
     {
         uint32_t x = 1024;
         uint8_t expected[4] = {0x00, 0x00, 0x04, 0x00};
         uint8_t result[4];
@@ -542,38 +603,39 @@
         REQUIRE(result[2] == expected[2]);
         REQUIRE(result[3] == expected[3]);
         uint32_t again = Util::FourBytesToInt(result);
         REQUIRE(again == x);
     }
 }
 
-
 TEST_CASE("Signature tests")
 {
     SECTION("Should use copy constructor")
     {
         vector<uint8_t> message1 = {1, 65, 254, 88, 90, 45, 22};
 
         vector<uint8_t> seed(32, 0x30);
         PrivateKey sk1 = BasicSchemeMPL().KeyGen(seed);
         G1Element pk1 = sk1.GetG1Element();
         PrivateKey sk2 = PrivateKey(sk1);
 
         uint8_t skBytes[PrivateKey::PRIVATE_KEY_SIZE];
         sk2.Serialize(skBytes);
-        PrivateKey sk4 = PrivateKey::FromBytes(Bytes(skBytes, PrivateKey::PRIVATE_KEY_SIZE));
+        PrivateKey sk4 =
+            PrivateKey::FromBytes(Bytes(skBytes, PrivateKey::PRIVATE_KEY_SIZE));
 
         G1Element pk2 = G1Element(pk1);
         G2Element sig1 = BasicSchemeMPL().Sign(sk4, message1);
         G2Element sig2 = G2Element(sig1);
 
         REQUIRE(BasicSchemeMPL().Verify(pk2, message1, sig2));
     }
 
-    SECTION("Should sign with the zero key") {
+    SECTION("Should sign with the zero key")
+    {
         vector<uint8_t> sk0(32, 0);
         PrivateKey sk = PrivateKey::FromByteVector(sk0);
         REQUIRE(sk.GetG1Element() == G1Element());  // Infinity
         REQUIRE(sk.GetG2Element() == G2Element());  // Infinity
         REQUIRE(BasicSchemeMPL().Sign(sk, {1, 2, 3}) == G2Element());
         REQUIRE(AugSchemeMPL().Sign(sk, {1, 2, 3}) == G2Element());
         REQUIRE(PopSchemeMPL().Sign(sk, {1, 2, 3}) == G2Element());
@@ -616,15 +678,16 @@
 
         vector<uint8_t> seed(32, 0x40);
         PrivateKey sk1 = BasicSchemeMPL().KeyGen(seed);
         G1Element pk1 = sk1.GetG1Element();
 
         uint8_t* skData = Util::SecAlloc<uint8_t>(G2Element::SIZE);
         sk1.Serialize(skData);
-        PrivateKey sk2 = PrivateKey::FromBytes(Bytes(skData, PrivateKey::PRIVATE_KEY_SIZE));
+        PrivateKey sk2 =
+            PrivateKey::FromBytes(Bytes(skData, PrivateKey::PRIVATE_KEY_SIZE));
         REQUIRE(sk1 == sk2);
 
         auto pkData = pk1.Serialize();
 
         G1Element pk2 = G1Element::FromBytes(Bytes(pkData));
         REQUIRE(pk1 == pk2);
 
@@ -638,62 +701,67 @@
         REQUIRE(BasicSchemeMPL().Verify(pk2, message1, sig2));
         Util::SecFree(skData);
     }
 
     SECTION("Should not verify aggregate with same message under BasicScheme")
     {
         vector<uint8_t> message = {100, 2, 254, 88, 90, 45, 23};
-        uint8_t hash[BLS::MESSAGE_HASH_LEN];
 
         vector<uint8_t> seed(32, 0x50);
         vector<uint8_t> seed2(32, 0x70);
 
         PrivateKey sk1 = BasicSchemeMPL().KeyGen(seed);
         PrivateKey sk2 = BasicSchemeMPL().KeyGen(seed2);
 
         G1Element pk1 = sk1.GetG1Element();
         G1Element pk2 = sk2.GetG1Element();
 
         G2Element sig1 = BasicSchemeMPL().Sign(sk1, message);
         G2Element sig2 = BasicSchemeMPL().Sign(sk2, message);
 
         G2Element aggSig = BasicSchemeMPL().Aggregate({sig1, sig2});
-        REQUIRE(BasicSchemeMPL().AggregateVerify({pk1, pk2}, vector<vector<uint8_t>>{message, message}, aggSig) == false);
+        REQUIRE(
+            BasicSchemeMPL().AggregateVerify(
+                {pk1, pk2},
+                vector<vector<uint8_t>>{message, message},
+                aggSig) == false);
     }
 
-    SECTION("Should verify aggregate with same message under AugScheme/PopScheme")
+    SECTION(
+        "Should verify aggregate with same message under AugScheme/PopScheme")
     {
         vector<uint8_t> message = {100, 2, 254, 88, 90, 45, 23};
-        uint8_t hash[BLS::MESSAGE_HASH_LEN];
 
         vector<uint8_t> seed(32, 0x50);
         vector<uint8_t> seed2(32, 0x70);
 
         PrivateKey sk1 = BasicSchemeMPL().KeyGen(seed);
         PrivateKey sk2 = BasicSchemeMPL().KeyGen(seed2);
 
         G1Element pk1 = sk1.GetG1Element();
         G1Element pk2 = sk2.GetG1Element();
 
         G2Element sig1Aug = AugSchemeMPL().Sign(sk1, message);
         G2Element sig2Aug = AugSchemeMPL().Sign(sk2, message);
         G2Element aggSigAug = AugSchemeMPL().Aggregate({sig1Aug, sig2Aug});
-        REQUIRE(AugSchemeMPL().AggregateVerify({pk1, pk2}, vector<vector<uint8_t>>{message, message}, aggSigAug));
+        REQUIRE(AugSchemeMPL().AggregateVerify(
+            {pk1, pk2}, vector<vector<uint8_t>>{message, message}, aggSigAug));
 
         G2Element sig1Pop = PopSchemeMPL().Sign(sk1, message);
         G2Element sig2Pop = PopSchemeMPL().Sign(sk2, message);
         G2Element aggSigPop = PopSchemeMPL().Aggregate({sig1Pop, sig2Pop});
-        REQUIRE(PopSchemeMPL().AggregateVerify({pk1, pk2}, vector<vector<uint8_t>>{message, message}, aggSigPop));
+        REQUIRE(PopSchemeMPL().AggregateVerify(
+            {pk1, pk2}, vector<vector<uint8_t>>{message, message}, aggSigPop));
     }
 
     SECTION("Should Aug aggregate many G2Elements, diff message")
     {
         vector<G1Element> pks;
         vector<G2Element> sigs;
-        vector<vector<uint8_t> > ms;
+        vector<vector<uint8_t>> ms;
 
         for (uint8_t i = 0; i < 80; i++) {
             vector<uint8_t> message = {0, 100, 2, 45, 64, 12, 12, 63, i};
             PrivateKey sk = BasicSchemeMPL().KeyGen(getRandomSeed());
             pks.push_back(sk.GetG1Element());
             auto sig = AugSchemeMPL().Sign(sk, message);
             sigs.push_back(sig);
@@ -704,41 +772,47 @@
 
         REQUIRE(AugSchemeMPL().AggregateVerify(pks, ms, aggSig));
     }
 
     SECTION("Aggregate Verification of zero items with infinity should pass")
     {
         vector<G1Element> pks_as_g1;
-        vector<vector<uint8_t> > pks_as_bytes;
-        vector<vector<uint8_t> > msgs;
+        vector<vector<uint8_t>> pks_as_bytes;
+        vector<vector<uint8_t>> msgs;
         vector<G2Element> sigs;
 
         sigs.push_back(G2Element());
         G2Element aggSig = AugSchemeMPL().Aggregate(sigs);
 
         REQUIRE(aggSig.Serialize().size() != 0);
         REQUIRE(aggSig == G2Element());
 
         REQUIRE(AugSchemeMPL().AggregateVerify(pks_as_g1, msgs, aggSig));
-        REQUIRE(AugSchemeMPL().AggregateVerify(pks_as_bytes, msgs, aggSig.Serialize()));
+        REQUIRE(AugSchemeMPL().AggregateVerify(
+            pks_as_bytes, msgs, aggSig.Serialize()));
 
         REQUIRE(BasicSchemeMPL().AggregateVerify(pks_as_g1, msgs, aggSig));
-        REQUIRE(BasicSchemeMPL().AggregateVerify(pks_as_bytes, msgs, aggSig.Serialize()));
+        REQUIRE(BasicSchemeMPL().AggregateVerify(
+            pks_as_bytes, msgs, aggSig.Serialize()));
 
-	// FastAggregateVerify takes one message, and requires at least one key
+        // FastAggregateVerify takes one message, and requires at least one key
         vector<uint8_t> msg;
         REQUIRE(pks_as_g1.size() == 0);
-        REQUIRE(PopSchemeMPL().FastAggregateVerify(pks_as_g1, msg, aggSig) == false);
+        REQUIRE(
+            PopSchemeMPL().FastAggregateVerify(pks_as_g1, msg, aggSig) ==
+            false);
         REQUIRE(pks_as_bytes.size() == 0);
-        REQUIRE(PopSchemeMPL().FastAggregateVerify(pks_as_bytes, msg, aggSig.Serialize()) == false);
-
+        REQUIRE(
+            PopSchemeMPL().FastAggregateVerify(
+                pks_as_bytes, msg, aggSig.Serialize()) == false);
     }
 }
 
-TEST_CASE("Agg sks") {
+TEST_CASE("Agg sks")
+{
     SECTION("Should create aggregates with agg sk (basic scheme)")
     {
         const vector<uint8_t> message = {100, 2, 254, 88, 90, 45, 23};
         const vector<uint8_t> seed(32, 0x07);
         const vector<uint8_t> seed2(32, 0x08);
 
         const PrivateKey sk1 = BasicSchemeMPL().KeyGen(seed);
@@ -755,25 +829,32 @@
         REQUIRE(aggPubKey == aggSk.GetG1Element());
 
         const G2Element sig1 = BasicSchemeMPL().Sign(sk1, message);
         const G2Element sig2 = BasicSchemeMPL().Sign(sk2, message);
 
         const G2Element aggSig2 = BasicSchemeMPL().Sign(aggSk, message);
 
-
         const G2Element aggSig = BasicSchemeMPL().Aggregate({sig1, sig2});
         REQUIRE(aggSig == aggSig2);
 
         // Verify as a single G2Element
         REQUIRE(BasicSchemeMPL().Verify(aggPubKey, message, aggSig));
         REQUIRE(BasicSchemeMPL().Verify(aggPubKey, message, aggSig2));
 
         // Verify aggregate with both keys (Fails since not distinct)
-        REQUIRE(BasicSchemeMPL().AggregateVerify({pk1, pk2}, vector<vector<uint8_t>>{message, message}, aggSig) == false);
-        REQUIRE(BasicSchemeMPL().AggregateVerify({pk1, pk2}, vector<vector<uint8_t>>{message, message}, aggSig2) == false);
+        REQUIRE(
+            BasicSchemeMPL().AggregateVerify(
+                {pk1, pk2},
+                vector<vector<uint8_t>>{message, message},
+                aggSig) == false);
+        REQUIRE(
+            BasicSchemeMPL().AggregateVerify(
+                {pk1, pk2},
+                vector<vector<uint8_t>>{message, message},
+                aggSig2) == false);
 
         // Try the same with distinct message, and same sk
         vector<uint8_t> message2 = {200, 29, 54, 8, 9, 29, 155, 55};
         G2Element sig3 = BasicSchemeMPL().Sign(sk2, message2);
         G2Element aggSigFinal = BasicSchemeMPL().Aggregate({aggSig, sig3});
         G2Element aggSigAlt = BasicSchemeMPL().Aggregate({sig1, sig2, sig3});
         G2Element aggSigAlt2 = BasicSchemeMPL().Aggregate({sig1, sig3, sig2});
@@ -787,20 +868,25 @@
 
         G1Element pkFinal = aggPubKey + pk2;
         G1Element pkFinalAlt = pk2 + pk1 + pk2;
         REQUIRE(pkFinal == pkFinalAlt);
         REQUIRE(pkFinal != aggPubKey);
 
         // Cannot verify with aggPubKey (since we have multiple messages)
-        REQUIRE(BasicSchemeMPL().AggregateVerify({aggPubKey, pk2}, vector<vector<uint8_t>>{message, message2}, aggSigFinal));
+        REQUIRE(BasicSchemeMPL().AggregateVerify(
+            {aggPubKey, pk2},
+            vector<vector<uint8_t>>{message, message2},
+            aggSigFinal));
     }
 }
 
-TEST_CASE("Advanced") {
-    SECTION("Should aggregate with multiple levels, degenerate") {
+TEST_CASE("Advanced")
+{
+    SECTION("Should aggregate with multiple levels, degenerate")
+    {
         vector<uint8_t> message1 = {100, 2, 254, 88, 90, 45, 23};
         PrivateKey sk1 = AugSchemeMPL().KeyGen(getRandomSeed());
         G1Element pk1 = sk1.GetG1Element();
         G2Element aggSig = AugSchemeMPL().Sign(sk1, message1);
         vector<G1Element> pks = {pk1};
         vector<vector<uint8_t>> ms = {message1};
 
@@ -811,15 +897,16 @@
             ms.push_back(message1);
             G2Element sig = AugSchemeMPL().Sign(sk, message1);
             aggSig = AugSchemeMPL().Aggregate({aggSig, sig});
         }
         REQUIRE(AugSchemeMPL().AggregateVerify(pks, ms, aggSig));
     }
 
-    SECTION("Should aggregate with multiple levels, different messages") {
+    SECTION("Should aggregate with multiple levels, different messages")
+    {
         vector<uint8_t> message1 = {100, 2, 254, 88, 90, 45, 23};
         vector<uint8_t> message2 = {192, 29, 2, 0, 0, 45, 23};
         vector<uint8_t> message3 = {52, 29, 2, 0, 0, 45, 102};
         vector<uint8_t> message4 = {99, 29, 2, 0, 0, 45, 222};
 
         PrivateKey sk1 = AugSchemeMPL().KeyGen(getRandomSeed());
         PrivateKey sk2 = AugSchemeMPL().KeyGen(getRandomSeed());
@@ -849,33 +936,32 @@
             message1, message2, message3, message4};
         REQUIRE(AugSchemeMPL().AggregateVerify(allPks, allMessages, aggSig));
     }
 
     SECTION("README")
     {
         // Example seed, used to generate private key. Always use
-        // a secure RNG with sufficient entropy to generate a seed (at least 32 bytes).
-        vector<uint8_t> seed = {0,  50, 6,  244, 24,  199, 1,  25,  52,  88,  192,
-                                19, 18, 12, 89,  6,   220, 18, 102, 58,  209, 82,
-                                12, 62, 89, 110, 182, 9,   44, 20,  254, 22};
+        // a secure RNG with sufficient entropy to generate a seed (at least 32
+        // bytes).
+        vector<uint8_t> seed = {0,   50,  6,   244, 24,  199, 1,   25,
+                                52,  88,  192, 19,  18,  12,  89,  6,
+                                220, 18,  102, 58,  209, 82,  12,  62,
+                                89,  110, 182, 9,   44,  20,  254, 22};
 
         PrivateKey sk = AugSchemeMPL().KeyGen(seed);
         G1Element pk = sk.GetG1Element();
 
-        vector<uint8_t> message = {1, 2, 3, 4, 5};  // Message is passed in as a byte vector
+        vector<uint8_t> message = {
+            1, 2, 3, 4, 5};  // Message is passed in as a byte vector
         G2Element signature = AugSchemeMPL().Sign(sk, message);
 
         vector<uint8_t> skBytes = sk.Serialize();
         vector<uint8_t> pkBytes = pk.Serialize();
         vector<uint8_t> signatureBytes = signature.Serialize();
 
-        cout << Util::HexStr(skBytes) << endl;    // 32 bytes
-        cout << Util::HexStr(pkBytes) << endl;    // 48 bytes
-        cout << Util::HexStr(signatureBytes) << endl;  // 96 bytes
-
         // Takes array of 32 bytes
         PrivateKey skc = PrivateKey::FromByteVector(skBytes);
 
         // Takes array of 48 bytes
         pk = G1Element::FromByteVector(pkBytes);
 
         // Takes array of 96 bytes
@@ -897,64 +983,73 @@
         // Generate second sig
         G1Element pk2 = sk2.GetG1Element();
         G2Element sig2 = AugSchemeMPL().Sign(sk2, message2);
 
         // Signatures can be noninteractively combined by anyone
         G2Element aggSig = AugSchemeMPL().Aggregate({sig1, sig2});
 
-        REQUIRE(AugSchemeMPL().AggregateVerify({pk1, pk2}, vector<vector<uint8_t>>{message, message2}, aggSig));
+        REQUIRE(AugSchemeMPL().AggregateVerify(
+            {pk1, pk2}, vector<vector<uint8_t>>{message, message2}, aggSig));
 
         seed[0] = 3;
         PrivateKey sk3 = AugSchemeMPL().KeyGen(seed);
         G1Element pk3 = sk3.GetG1Element();
         vector<uint8_t> message3 = {100, 2, 254, 88, 90, 45, 23};
         G2Element sig3 = AugSchemeMPL().Sign(sk3, message3);
 
-
         // Arbitrary trees of aggregates
         G2Element aggSigFinal = AugSchemeMPL().Aggregate({aggSig, sig3});
 
-        REQUIRE(AugSchemeMPL().AggregateVerify({pk1, pk2, pk3}, vector<vector<uint8_t>>{message, message2, message3}, aggSigFinal));
-
-        // If the same message is signed, you can use Proof of Posession (PopScheme) for efficiency
-        // A proof of possession MUST be passed around with the PK to ensure security.
+        REQUIRE(AugSchemeMPL().AggregateVerify(
+            {pk1, pk2, pk3},
+            vector<vector<uint8_t>>{message, message2, message3},
+            aggSigFinal));
+
+        // If the same message is signed, you can use Proof of Posession
+        // (PopScheme) for efficiency A proof of possession MUST be passed
+        // around with the PK to ensure security.
 
         G2Element popSig1 = PopSchemeMPL().Sign(sk1, message);
         G2Element popSig2 = PopSchemeMPL().Sign(sk2, message);
         G2Element popSig3 = PopSchemeMPL().Sign(sk3, message);
         G2Element pop1 = PopSchemeMPL().PopProve(sk1);
         G2Element pop2 = PopSchemeMPL().PopProve(sk2);
         G2Element pop3 = PopSchemeMPL().PopProve(sk3);
 
         REQUIRE(PopSchemeMPL().PopVerify(pk1, pop1));
         REQUIRE(PopSchemeMPL().PopVerify(pk2, pop2));
         REQUIRE(PopSchemeMPL().PopVerify(pk3, pop3));
-        G2Element popSigAgg = PopSchemeMPL().Aggregate({popSig1, popSig2, popSig3});
+        G2Element popSigAgg =
+            PopSchemeMPL().Aggregate({popSig1, popSig2, popSig3});
 
-        REQUIRE(PopSchemeMPL().FastAggregateVerify({pk1, pk2, pk3}, message, popSigAgg));
+        REQUIRE(PopSchemeMPL().FastAggregateVerify(
+            {pk1, pk2, pk3}, message, popSigAgg));
 
         // Aggregate public key, indistinguishable from a single public key
         G1Element popAggPk = pk1 + pk2 + pk3;
         REQUIRE(PopSchemeMPL().Verify(popAggPk, message, popSigAgg));
 
         // Aggregate private keys
         PrivateKey aggSk = PrivateKey::Aggregate({sk1, sk2, sk3});
         REQUIRE(PopSchemeMPL().Sign(aggSk, message) == popSigAgg);
 
-
         PrivateKey masterSk = AugSchemeMPL().KeyGen(seed);
         PrivateKey child = AugSchemeMPL().DeriveChildSk(masterSk, 152);
         PrivateKey grandchild = AugSchemeMPL().DeriveChildSk(child, 952);
 
         G1Element masterPk = masterSk.GetG1Element();
-        PrivateKey childU = AugSchemeMPL().DeriveChildSkUnhardened(masterSk, 22);
-        PrivateKey grandchildU = AugSchemeMPL().DeriveChildSkUnhardened(childU, 0);
-
-        G1Element childUPk = AugSchemeMPL().DeriveChildPkUnhardened(masterPk, 22);
-        G1Element grandchildUPk = AugSchemeMPL().DeriveChildPkUnhardened(childUPk, 0);
+        PrivateKey childU =
+            AugSchemeMPL().DeriveChildSkUnhardened(masterSk, 22);
+        PrivateKey grandchildU =
+            AugSchemeMPL().DeriveChildSkUnhardened(childU, 0);
+
+        G1Element childUPk =
+            AugSchemeMPL().DeriveChildPkUnhardened(masterPk, 22);
+        G1Element grandchildUPk =
+            AugSchemeMPL().DeriveChildPkUnhardened(childUPk, 0);
 
         REQUIRE(grandchildUPk == grandchildU.GetG1Element());
     }
 
     SECTION("Bytes overloads")
     {
         std::vector<uint8_t> vecHash = getRandomSeed();
@@ -968,104 +1063,131 @@
         REQUIRE(g1Vector == g1Bytes);
 
         std::vector<uint8_t> vecG2Element = pk1.GetG2Element().Serialize();
         G2Element g2Vector = G2Element::FromByteVector(vecG2Element);
         G2Element g2Bytes = G2Element::FromBytes(Bytes(vecG2Element));
         REQUIRE(g2Vector == g2Bytes);
 
-        G1Element g1MessageVector = G1Element::FromMessage(vecHash, vecHash.data(), vecHash.size());
-        G1Element g1MessageBytes = G1Element::FromMessage(Bytes(vecHash), vecHash.data(), vecHash.size());
+        G1Element g1MessageVector =
+            G1Element::FromMessage(vecHash, vecHash.data(), vecHash.size());
+        G1Element g1MessageBytes = G1Element::FromMessage(
+            Bytes(vecHash), vecHash.data(), vecHash.size());
         REQUIRE(g1MessageVector == g1MessageBytes);
 
-        G2Element g2MessageVector = G2Element::FromMessage(vecHash, vecHash.data(), vecHash.size());
-        G2Element g2MessageBytes = G2Element::FromMessage(Bytes(vecHash), vecHash.data(), vecHash.size());
+        G2Element g2MessageVector =
+            G2Element::FromMessage(vecHash, vecHash.data(), vecHash.size());
+        G2Element g2MessageBytes = G2Element::FromMessage(
+            Bytes(vecHash), vecHash.data(), vecHash.size());
         REQUIRE(g2MessageVector == g2MessageBytes);
 
         G1Element g1_1 = pk1.GetG1Element();
         G1Element g1_2 = pk2.GetG1Element();
         G1Element g1_3 = pk3.GetG1Element();
 
         G2Element g2BasicSignVector1 = BasicSchemeMPL().Sign(pk1, vecHash);
-        G2Element g2BasicSignBytes1 = BasicSchemeMPL().Sign(pk1, Bytes(vecHash));
+        G2Element g2BasicSignBytes1 =
+            BasicSchemeMPL().Sign(pk1, Bytes(vecHash));
         REQUIRE(g2BasicSignVector1 == g2BasicSignBytes1);
         G2Element g2BasicSign2 = BasicSchemeMPL().Sign(pk2, Bytes(vecHash));
-        G2Element g2BasicSign3 = BasicSchemeMPL().Sign(pk3, Bytes(vecG2Element));
+        G2Element g2BasicSign3 =
+            BasicSchemeMPL().Sign(pk3, Bytes(vecG2Element));
         REQUIRE(g2BasicSignVector1 != g2BasicSign2);
 
-        REQUIRE(BasicSchemeMPL().Verify(Bytes(g1_1.Serialize()), Bytes(vecHash), Bytes(g2BasicSignVector1.Serialize())));
-        REQUIRE(BasicSchemeMPL().Verify(g1_1, Bytes(vecHash), g2BasicSignVector1));
+        REQUIRE(BasicSchemeMPL().Verify(
+            Bytes(g1_1.Serialize()),
+            Bytes(vecHash),
+            Bytes(g2BasicSignVector1.Serialize())));
+        REQUIRE(
+            BasicSchemeMPL().Verify(g1_1, Bytes(vecHash), g2BasicSignVector1));
 
-        vector<vector<uint8_t>> vecG1Vector = {g1_1.Serialize(), g1_3.Serialize()};
-        vector<vector<uint8_t>> vecG2Vector = {g2BasicSignVector1.Serialize(), g2BasicSign3.Serialize()};
+        vector<vector<uint8_t>> vecG1Vector = {
+            g1_1.Serialize(), g1_3.Serialize()};
+        vector<vector<uint8_t>> vecG2Vector = {
+            g2BasicSignVector1.Serialize(), g2BasicSign3.Serialize()};
         vector<vector<uint8_t>> vecHashes = {vecHash, vecG2Element};
 
         vector<uint8_t> aggVector = BasicSchemeMPL().Aggregate(vecG2Vector);
-        vector<uint8_t> aggBytes = BasicSchemeMPL().Aggregate(vector<Bytes>{vecG2Vector.begin(), vecG2Vector.end()});
+        vector<uint8_t> aggBytes = BasicSchemeMPL().Aggregate(
+            vector<Bytes>{vecG2Vector.begin(), vecG2Vector.end()});
         REQUIRE(aggVector == aggBytes);
 
-        REQUIRE(BasicSchemeMPL().AggregateVerify(vector<Bytes>{vecG1Vector.begin(), vecG1Vector.end()},
-                                                 vector<Bytes>{vecHashes.begin(), vecHashes.end()},
-                                                 Bytes(aggVector)));
-        REQUIRE(BasicSchemeMPL().AggregateVerify({g1_1, g1_3},
-                                                 vector<Bytes>{vecHashes.begin(), vecHashes.end()},
-                                                 G2Element::FromByteVector(aggVector)));
+        REQUIRE(BasicSchemeMPL().AggregateVerify(
+            vector<Bytes>{vecG1Vector.begin(), vecG1Vector.end()},
+            vector<Bytes>{vecHashes.begin(), vecHashes.end()},
+            Bytes(aggVector)));
+        REQUIRE(BasicSchemeMPL().AggregateVerify(
+            {g1_1, g1_3},
+            vector<Bytes>{vecHashes.begin(), vecHashes.end()},
+            G2Element::FromByteVector(aggVector)));
 
         G2Element g2AugSignVector1 = AugSchemeMPL().Sign(pk1, vecHash);
         G2Element g2AugSignBytes1 = AugSchemeMPL().Sign(pk1, Bytes(vecHash));
         G2Element g2AugSign2 = AugSchemeMPL().Sign(pk2, vecG2Element);
         REQUIRE(g2AugSignVector1 == g2AugSignBytes1);
         REQUIRE(g2AugSignVector1 != g2AugSign2);
 
-        REQUIRE(AugSchemeMPL().Verify(Bytes(g1_1.Serialize()), Bytes(vecHash), Bytes(g2AugSignVector1.Serialize())));
+        REQUIRE(AugSchemeMPL().Verify(
+            Bytes(g1_1.Serialize()),
+            Bytes(vecHash),
+            Bytes(g2AugSignVector1.Serialize())));
         REQUIRE(AugSchemeMPL().Verify(g1_1, Bytes(vecHash), g2AugSignVector1));
 
-        vector<vector<uint8_t>> vecG1AugVector = {g1_1.Serialize(), g1_2.Serialize()};
-        vector<vector<uint8_t>> vecG2AugVector = {g2AugSignVector1.Serialize(), g2AugSign2.Serialize()};
+        vector<vector<uint8_t>> vecG1AugVector = {
+            g1_1.Serialize(), g1_2.Serialize()};
+        vector<vector<uint8_t>> vecG2AugVector = {
+            g2AugSignVector1.Serialize(), g2AugSign2.Serialize()};
 
         vector<uint8_t> aggAugVector = AugSchemeMPL().Aggregate(vecG2AugVector);
-        vector<uint8_t> aggAugBytes = AugSchemeMPL().Aggregate(vector<Bytes>{vecG2AugVector.begin(), vecG2AugVector.end()});
+        vector<uint8_t> aggAugBytes = AugSchemeMPL().Aggregate(
+            vector<Bytes>{vecG2AugVector.begin(), vecG2AugVector.end()});
         REQUIRE(aggAugVector == aggAugBytes);
 
-        REQUIRE(AugSchemeMPL().AggregateVerify(vector<Bytes>{vecG1AugVector.begin(), vecG1AugVector.end()},
-                                                 vector<Bytes>{vecHashes.begin(), vecHashes.end()},
-                                                 Bytes(aggAugVector)));
-        REQUIRE(AugSchemeMPL().AggregateVerify({g1_1, g1_2},
-                                                 vector<Bytes>{vecHashes.begin(), vecHashes.end()},
-                                                 G2Element::FromByteVector(aggAugVector)));
+        REQUIRE(AugSchemeMPL().AggregateVerify(
+            vector<Bytes>{vecG1AugVector.begin(), vecG1AugVector.end()},
+            vector<Bytes>{vecHashes.begin(), vecHashes.end()},
+            Bytes(aggAugVector)));
+        REQUIRE(AugSchemeMPL().AggregateVerify(
+            {g1_1, g1_2},
+            vector<Bytes>{vecHashes.begin(), vecHashes.end()},
+            G2Element::FromByteVector(aggAugVector)));
 
         G2Element proof = PopSchemeMPL().PopProve(pk1);
         REQUIRE(PopSchemeMPL().PopVerify(g1_1, proof));
-        REQUIRE(PopSchemeMPL().PopVerify(Bytes(g1_1.Serialize()), Bytes(proof.Serialize())));
+        REQUIRE(PopSchemeMPL().PopVerify(
+            Bytes(g1_1.Serialize()), Bytes(proof.Serialize())));
 
         G2Element g2Pop1 = PopSchemeMPL().Sign(pk1, vecHash);
         G2Element g2Pop2 = PopSchemeMPL().Sign(pk2, vecHash);
         G2Element g2PopAgg = PopSchemeMPL().Aggregate({g2Pop1, g2Pop2});
         vecG1Vector = {g1_1.Serialize(), g1_2.Serialize()};
-        REQUIRE(PopSchemeMPL().FastAggregateVerify({g1_1, g1_2}, Bytes(vecHash), g2PopAgg));
-        REQUIRE(PopSchemeMPL().FastAggregateVerify(vector<Bytes>{vecG1Vector.begin(), vecG1Vector.end()},
-                                                   Bytes(vecHash), Bytes(g2PopAgg.Serialize())));
+        REQUIRE(PopSchemeMPL().FastAggregateVerify(
+            {g1_1, g1_2}, Bytes(vecHash), g2PopAgg));
+        REQUIRE(PopSchemeMPL().FastAggregateVerify(
+            vector<Bytes>{vecG1Vector.begin(), vecG1Vector.end()},
+            Bytes(vecHash),
+            Bytes(g2PopAgg.Serialize())));
     }
 }
 
-
-TEST_CASE("Schemes") {
-    SECTION("Basic Scheme") {
+TEST_CASE("Schemes")
+{
+    SECTION("Basic Scheme")
+    {
         vector<uint8_t> seed1(32, 0x04);
         vector<uint8_t> seed2(32, 0x05);
         vector<uint8_t> msg1 = {7, 8, 9};
         vector<uint8_t> msg2 = {10, 11, 12};
         vector<vector<uint8_t>> msgs = {msg1, msg2};
 
         PrivateKey sk1 = BasicSchemeMPL().KeyGen(seed1);
         G1Element pk1 = BasicSchemeMPL().SkToG1(sk1);
         vector<uint8_t> pk1v = BasicSchemeMPL().SkToPk(sk1);
         G2Element sig1 = BasicSchemeMPL().Sign(sk1, msg1);
         vector<uint8_t> sig1v = BasicSchemeMPL().Sign(sk1, msg1).Serialize();
 
-
         REQUIRE(BasicSchemeMPL().Verify(pk1v, msg1, sig1v));
 
         PrivateKey sk2 = BasicSchemeMPL().KeyGen(seed2);
         G1Element pk2 = BasicSchemeMPL().SkToG1(sk2);
         vector<uint8_t> pk2v = BasicSchemeMPL().SkToPk(sk2);
         G2Element sig2 = BasicSchemeMPL().Sign(sk2, msg2);
         vector<uint8_t> sig2v = BasicSchemeMPL().Sign(sk2, msg2).Serialize();
@@ -1077,15 +1199,16 @@
         REQUIRE(BasicSchemeMPL().Verify(pk1, msg2, sig1) == false);
         REQUIRE(BasicSchemeMPL().Verify(pk1v, msg2, sig1v) == false);
         // Wrong pk
         REQUIRE(BasicSchemeMPL().Verify(pk2, msg1, sig1) == false);
         REQUIRE(BasicSchemeMPL().Verify(pk2v, msg1, sig1v) == false);
 
         G2Element aggsig = BasicSchemeMPL().Aggregate({sig1, sig2});
-        vector<uint8_t> aggsigv = BasicSchemeMPL().Aggregate(vector<vector<uint8_t>>{sig1v, sig2v});
+        vector<uint8_t> aggsigv =
+            BasicSchemeMPL().Aggregate(vector<vector<uint8_t>>{sig1v, sig2v});
         REQUIRE(BasicSchemeMPL().AggregateVerify({pk1, pk2}, msgs, aggsig));
         REQUIRE(BasicSchemeMPL().AggregateVerify({pk1v, pk2v}, msgs, aggsigv));
     }
 
     SECTION("Aug Scheme")
     {
         vector<uint8_t> seed1(32, 0x04);
@@ -1116,15 +1239,16 @@
         REQUIRE(AugSchemeMPL().Verify(pk1, msg2, sig1) == false);
         REQUIRE(AugSchemeMPL().Verify(pk1v, msg2, sig1v) == false);
         // Wrong pk
         REQUIRE(AugSchemeMPL().Verify(pk2, msg1, sig1) == false);
         REQUIRE(AugSchemeMPL().Verify(pk2v, msg1, sig1v) == false);
 
         G2Element aggsig = AugSchemeMPL().Aggregate({sig1, sig2});
-        vector<uint8_t> aggsigv = AugSchemeMPL().Aggregate(vector<vector<uint8_t>>{sig1v, sig2v});
+        vector<uint8_t> aggsigv =
+            AugSchemeMPL().Aggregate(vector<vector<uint8_t>>{sig1v, sig2v});
         REQUIRE(AugSchemeMPL().AggregateVerify({pk1, pk2}, msgs, aggsig));
         REQUIRE(AugSchemeMPL().AggregateVerify({pk1v, pk2v}, msgs, aggsigv));
     }
 
     SECTION("Pop Scheme")
     {
         vector<uint8_t> seed1(32, 0x06);
@@ -1155,36 +1279,98 @@
         REQUIRE(PopSchemeMPL().Verify(pk1, msg2, sig1) == false);
         REQUIRE(PopSchemeMPL().Verify(pk1v, msg2, sig1v) == false);
         // Wrong pk
         REQUIRE(PopSchemeMPL().Verify(pk2, msg1, sig1) == false);
         REQUIRE(PopSchemeMPL().Verify(pk2v, msg1, sig1v) == false);
 
         G2Element aggsig = PopSchemeMPL().Aggregate({sig1, sig2});
-        vector<uint8_t> aggsigv = PopSchemeMPL().Aggregate(vector<vector<uint8_t>>{sig1v, sig2v});
+        vector<uint8_t> aggsigv =
+            PopSchemeMPL().Aggregate(vector<vector<uint8_t>>{sig1v, sig2v});
         REQUIRE(PopSchemeMPL().AggregateVerify({pk1, pk2}, msgs, aggsig));
         REQUIRE(PopSchemeMPL().AggregateVerify({pk1v, pk2v}, msgs, aggsigv));
 
         // PopVerify
         G2Element proof1 = PopSchemeMPL().PopProve(sk1);
         vector<uint8_t> proof1v = PopSchemeMPL().PopProve(sk1).Serialize();
         REQUIRE(PopSchemeMPL().PopVerify(pk1, proof1));
         REQUIRE(PopSchemeMPL().PopVerify(pk1v, proof1v));
 
         // FastAggregateVerify
         // We want sk2 to sign the same message
         G2Element sig2_same = PopSchemeMPL().Sign(sk2, msg1);
         vector<uint8_t> sig2v_same = PopSchemeMPL().Sign(sk2, msg1).Serialize();
         G2Element aggsig_same = PopSchemeMPL().Aggregate({sig1, sig2_same});
-        vector<uint8_t> aggsigv_same =
-            PopSchemeMPL().Aggregate(vector<vector<uint8_t>>{sig1v, sig2v_same});
+        vector<uint8_t> aggsigv_same = PopSchemeMPL().Aggregate(
+            vector<vector<uint8_t>>{sig1v, sig2v_same});
         REQUIRE(
             PopSchemeMPL().FastAggregateVerify({pk1, pk2}, msg1, aggsig_same));
         REQUIRE(PopSchemeMPL().FastAggregateVerify(
             {pk1v, pk2v}, msg1, aggsigv_same));
     }
 }
 
+TEST_CASE("CheckValid")
+{
+    SECTION("Valid points should succeed")
+    {
+        vector<uint8_t> seed(32, 0x05);
+        vector<uint8_t> msg1 = {10, 11, 12};
+
+        PrivateKey sk1 = BasicSchemeMPL().KeyGen(seed);
+        G1Element pk1 = BasicSchemeMPL().SkToG1(sk1);
+        pk1.CheckValid();
+
+        G2Element sig1 = AugSchemeMPL().Sign(sk1, msg1);
+        sig1.CheckValid();
+    }
+
+    SECTION("Invalid G1 points should not succeed")
+    {
+        string badPointHex =
+            "8d5d0fb73b9c92df4eab4216e48c3e358578b4cc30f82c268bd6fef3bd34b55862"
+            "8daf1afef798d4c3b0fcd8b28c8973";
+
+        // FromBytes throws
+        REQUIRE_THROWS(
+            G1Element::FromBytes(Bytes(Util::HexToBytes(badPointHex))));
+
+        // FromBytesUnchecked does not throw
+        G1Element bad_pk =
+            G1Element::FromBytesUnchecked(Bytes(Util::HexToBytes(badPointHex)));
+        REQUIRE(bad_pk.IsValid() == false);
+        REQUIRE_THROWS(bad_pk.CheckValid());
+
+        vector<uint8_t> seed(32, 0x05);
+        vector<uint8_t> msg1 = {10, 11, 12};
+        PrivateKey sk1 = BasicSchemeMPL().KeyGen(seed);
+        G1Element good_pk = BasicSchemeMPL().SkToG1(sk1);
+        REQUIRE(good_pk.IsValid() == true);
+        G2Element sig1 = AugSchemeMPL().Sign(sk1, msg1);
+        REQUIRE(AugSchemeMPL().Verify(bad_pk, msg1, sig1) == false);
+        REQUIRE(AugSchemeMPL().Verify(good_pk, msg1, sig1) == true);
+    }
+
+    SECTION("Invalid G2 points should not succeed")
+    {
+        blst_p2 point_native;
+        memset(&point_native, 0, sizeof(blst_p2));
+
+        // copy some probably invalid data into the point
+        memcpy(&(point_native.x), (void*)memcpy, sizeof(point_native.x));
+        memcpy(&(point_native.y), (void*)memset, sizeof(point_native.y));
+        memcpy(&(point_native.z), (void*)printf, sizeof(point_native.z));
+
+        G2Element point = G2Element::FromNative(point_native);
+        REQUIRE(point.IsValid() == false);
+        REQUIRE_THROWS(point.CheckValid());
+
+        auto badSer = point.Serialize();
+
+        REQUIRE_THROWS(G2Element::FromByteVector(badSer));
+    }
+}
+
 int main(int argc, char* argv[])
 {
     int result = Catch::Session().run(argc, argv);
     return result;
 }
```

### Comparing `blspy-1.0.9/src/util.hpp` & `blspy-2.0.0b1/src/util.hpp`

 * *Files 24% similar despite different names*

```diff
@@ -15,33 +15,40 @@
 #ifndef SRC_BLSUTIL_HPP_
 #define SRC_BLSUTIL_HPP_
 
 #include <algorithm>
 #include <iomanip>
 #include <sstream>
 #include <string>
+#include <cstring>
 #include <vector>
+#include <array>
 
 namespace bls {
 
 class BLS;
 
 class Bytes {
     const uint8_t* pData;
     const size_t nSize;
 
 public:
-    explicit Bytes(const uint8_t* pDataIn, const size_t nSizeIn)
+    Bytes(const uint8_t* pDataIn, const size_t nSizeIn)
         : pData(pDataIn), nSize(nSizeIn)
     {
     }
-    explicit Bytes(const std::vector<uint8_t>& vecBytes)
+    Bytes(const std::vector<uint8_t>& vecBytes)
         : pData(vecBytes.data()), nSize(vecBytes.size())
     {
     }
+    template <size_t N>
+    Bytes(const std::array<uint8_t, N>& a)
+        : pData(a.data()), nSize(N)
+    {
+    }
 
     inline const uint8_t* begin() const { return pData; }
     inline const uint8_t* end() const { return pData + nSize; }
 
     inline size_t size() const { return nSize; }
 
     const uint8_t& operator[](const int nIndex) const { return pData[nIndex]; }
@@ -50,17 +57,51 @@
 class Util {
  public:
     typedef void *(*SecureAllocCallback)(size_t);
     typedef void (*SecureFreeCallback)(void*);
  public:
     static void Hash256(uint8_t* output, const uint8_t* message,
                         size_t messageLen) {
-        md_map_sh256(output, message, messageLen);
+        blst_sha256(output, message, messageLen);
     }
 
+static void md_hmac(uint8_t *mac, const uint8_t *in, int in_len, const uint8_t *key,
+    int key_len) {
+  #define block_size 64
+  #define RLC_MD_LEN 32
+    uint8_t opad[block_size + RLC_MD_LEN];
+    uint8_t *ipad = (uint8_t *)malloc(block_size + in_len);
+        uint8_t _key[block_size];
+
+/*    if (ipad == NULL) {
+        RLC_THROW(ERR_NO_MEMORY);
+                return;
+    }
+*/
+        if (key_len > block_size) {
+                Hash256(_key, key, key_len);
+                key = _key;
+                key_len = RLC_MD_LEN;
+        }
+        if (key_len <= block_size) {
+                memcpy(_key, key, key_len);
+                memset(_key + key_len, 0, block_size - key_len);
+                key = _key;
+        }
+        for (int i = 0; i < block_size; i++) {
+                opad[i] = 0x5C ^ key[i];
+                ipad[i] = 0x36 ^ key[i];
+        }
+        memcpy(ipad + block_size, in, in_len);
+        Hash256(opad + block_size, ipad, block_size + in_len);
+        Hash256(mac, opad, block_size + RLC_MD_LEN);
+
+    free(ipad);
+}
+
     static std::string HexStr(const uint8_t* data, size_t len) {
         std::stringstream s;
         s << std::hex;
         for (size_t i=0; i < len; ++i)
             s << std::setw(2) << std::setfill('0') << static_cast<int>(data[i]);
         return s.str();
     }
```

