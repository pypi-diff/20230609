# Comparing `tmp/vowpal-wabbit-next-0.4.0.tar.gz` & `tmp/vowpal-wabbit-next-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vowpal-wabbit-next-0.4.0.tar", last modified: Fri Apr 14 16:07:39 2023, max compression
+gzip compressed data, was "vowpal-wabbit-next-0.4.1.tar", last modified: Fri Jun  9 20:35:42 2023, max compression
```

## Comparing `vowpal-wabbit-next-0.4.0.tar` & `vowpal-wabbit-next-0.4.1.tar`

### file list

```diff
@@ -1,1069 +1,1069 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.592634 vowpal-wabbit-next-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-04-14 16:07:19.000000 vowpal-wabbit-next-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-14 16:07:19.000000 vowpal-wabbit-next-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-04-14 16:07:39.592634 vowpal-wabbit-next-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-04-14 16:07:19.000000 vowpal-wabbit-next-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.380629 vowpal-wabbit-next-0.4.0/ext_libs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.400630 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/.appveyor.yml
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/.clang-format
--rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/.clang-tidy
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/.cmake-format.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/.codespell-ignore-lines
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-14 16:07:20.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/.git
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.400630 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)    15271 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/.github/CONTRIBUTING.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.400630 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/.github/ISSUE_TEMPLATE/bug-report.yml
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/.github/labeler.yml
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/.github/labeler_merged.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.400630 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/.github/matchers/
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/.github/matchers/pylint.json
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.404630 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)    31868 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/.github/workflows/configure.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/.github/workflows/format.yml
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/.github/workflows/labeler.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/.github/workflows/pip.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/.github/workflows/upstream.yml
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)    11983 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7686 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.408630 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/docs/Doxyfile
--rw-r--r--   0 runner    (1001) docker     (123)     7417 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.380629 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.408630 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/docs/_static/css/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.408630 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/docs/advanced/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.408630 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/docs/advanced/cast/
--rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/docs/advanced/cast/chrono.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/docs/advanced/cast/custom.rst
--rw-r--r--   0 runner    (1001) docker     (123)    14283 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/docs/advanced/cast/eigen.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/docs/advanced/cast/functional.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/docs/advanced/cast/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12371 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/docs/advanced/cast/overview.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9586 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/docs/advanced/cast/stl.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8863 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/docs/advanced/cast/strings.rst
--rw-r--r--   0 runner    (1001) docker     (123)    47796 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/docs/advanced/classes.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8453 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/docs/advanced/embedding.rst
--rw-r--r--   0 runner    (1001) docker     (123)    17796 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/docs/advanced/exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (123)    26729 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/docs/advanced/functions.rst
--rw-r--r--   0 runner    (1001) docker     (123)    15651 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/docs/advanced/misc.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.412630 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/docs/advanced/pycpp/
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/docs/advanced/pycpp/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    17161 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/docs/advanced/pycpp/numpy.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9030 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/docs/advanced/pycpp/object.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5710 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/docs/advanced/pycpp/utilities.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6377 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/docs/advanced/smart_ptrs.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9240 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/docs/basics.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/docs/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/docs/benchmark.rst
--rw-r--r--   0 runner    (1001) docker     (123)   114174 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)    16380 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/docs/classes.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.412630 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/docs/cmake/
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/docs/cmake/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    25777 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/docs/compiling.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11559 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    13177 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/docs/faq.rst
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/docs/installing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/docs/limitations.rst
--rw-r--r--   0 runner    (1001) docker     (123)    61034 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/docs/pybind11-logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    44653 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/docs/pybind11_vs_boost_python1.png
--rw-r--r--   0 runner    (1001) docker     (123)    87708 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/docs/pybind11_vs_boost_python1.svg
--rw-r--r--   0 runner    (1001) docker     (123)    41121 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/docs/pybind11_vs_boost_python2.png
--rw-r--r--   0 runner    (1001) docker     (123)    85853 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/docs/pybind11_vs_boost_python2.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/docs/reference.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/docs/release.rst
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)    23489 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/docs/upgrade.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.380629 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.416630 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/include/pybind11/
--rw-r--r--   0 runner    (1001) docker     (123)    23959 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/include/pybind11/attr.h
--rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/include/pybind11/buffer_info.h
--rw-r--r--   0 runner    (1001) docker     (123)    65660 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/include/pybind11/cast.h
--rw-r--r--   0 runner    (1001) docker     (123)     8458 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/include/pybind11/chrono.h
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/include/pybind11/common.h
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/include/pybind11/complex.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.416630 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/include/pybind11/detail/
--rw-r--r--   0 runner    (1001) docker     (123)    28251 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/include/pybind11/detail/class.h
--rw-r--r--   0 runner    (1001) docker     (123)    52929 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/include/pybind11/detail/common.h
--rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/include/pybind11/detail/descr.h
--rw-r--r--   0 runner    (1001) docker     (123)    17869 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/include/pybind11/detail/init.h
--rw-r--r--   0 runner    (1001) docker     (123)    26305 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/include/pybind11/detail/internals.h
--rw-r--r--   0 runner    (1001) docker     (123)    42613 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/include/pybind11/detail/type_caster_base.h
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/include/pybind11/detail/typeid.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.416630 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/include/pybind11/eigen/
--rw-r--r--   0 runner    (1001) docker     (123)    31418 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/include/pybind11/eigen/matrix.h
--rw-r--r--   0 runner    (1001) docker     (123)    18108 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/include/pybind11/eigen/tensor.h
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/include/pybind11/eigen.h
--rw-r--r--   0 runner    (1001) docker     (123)    13471 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/include/pybind11/embed.h
--rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/include/pybind11/eval.h
--rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/include/pybind11/functional.h
--rw-r--r--   0 runner    (1001) docker     (123)     8262 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/include/pybind11/gil.h
--rw-r--r--   0 runner    (1001) docker     (123)     8862 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/include/pybind11/iostream.h
--rw-r--r--   0 runner    (1001) docker     (123)    79408 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/include/pybind11/numpy.h
--rw-r--r--   0 runner    (1001) docker     (123)     9103 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/include/pybind11/operators.h
--rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/include/pybind11/options.h
--rw-r--r--   0 runner    (1001) docker     (123)   126420 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/include/pybind11/pybind11.h
--rw-r--r--   0 runner    (1001) docker     (123)    94641 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/include/pybind11/pytypes.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.416630 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/include/pybind11/stl/
--rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/include/pybind11/stl/filesystem.h
--rw-r--r--   0 runner    (1001) docker     (123)    15337 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/include/pybind11/stl.h
--rw-r--r--   0 runner    (1001) docker     (123)    29747 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/include/pybind11/stl_bind.h
--rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/noxfile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.416630 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/pybind11/
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/pybind11/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/pybind11/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/pybind11/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/pybind11/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/pybind11/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    17609 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/pybind11/setup_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4877 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.440631 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    21675 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    11736 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/constructor_stats.h
--rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/cross_module_gil_utils.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/cross_module_interleaved_error_already_set.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/eigen_tensor_avoid_stl_array.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.440631 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/extra_python_package/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/extra_python_package/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)     8296 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/extra_python_package/test_files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.440631 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/extra_setuptools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/extra_setuptools/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/extra_setuptools/test_setuphelper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/local_bindings.h
--rw-r--r--   0 runner    (1001) docker     (123)     5743 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/object.h
--rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/pybind11_cross_module_tests.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/pybind11_tests.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/pybind11_tests.h
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_async.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_async.py
--rw-r--r--   0 runner    (1001) docker     (123)     8567 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_buffers.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4841 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_buffers.py
--rw-r--r--   0 runner    (1001) docker     (123)    16025 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_builtin_casters.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    17245 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_builtin_casters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_call_policies.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6549 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_call_policies.py
--rw-r--r--   0 runner    (1001) docker     (123)    10858 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_callbacks.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6246 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_chrono.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_chrono.py
--rw-r--r--   0 runner    (1001) docker     (123)    24874 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_class.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    14815 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_class.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.440631 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_cmake_build/
--rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_cmake_build/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_cmake_build/embed.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.440631 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_cmake_build/installed_embed/
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.440631 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_cmake_build/installed_function/
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.440631 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_cmake_build/installed_target/
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_cmake_build/main.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.440631 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_cmake_build/subdirectory_embed/
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.440631 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_cmake_build/subdirectory_function/
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.440631 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_cmake_build/subdirectory_target/
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_cmake_build/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_const_name.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_const_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_constants_and_functions.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_constants_and_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10886 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_copy_move.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4796 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_copy_move.py
--rw-r--r--   0 runner    (1001) docker     (123)     7280 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_custom_type_casters.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_custom_type_casters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_custom_type_setup.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_custom_type_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     4557 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_docstring_options.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_docstring_options.py
--rw-r--r--   0 runner    (1001) docker     (123)    19350 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_eigen_matrix.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    28867 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_eigen_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_eigen_tensor.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    10590 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_eigen_tensor.inl
--rw-r--r--   0 runner    (1001) docker     (123)     9456 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_eigen_tensor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.444630 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_embed/
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_embed/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_embed/catch.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_embed/external_module.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    16535 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_embed/test_interpreter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_embed/test_interpreter.py
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_embed/test_trampoline.py
--rw-r--r--   0 runner    (1001) docker     (123)     5722 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_enum.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     8903 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_eval.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_eval_call.py
--rw-r--r--   0 runner    (1001) docker     (123)    11904 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_exceptions.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_exceptions.h
--rw-r--r--   0 runner    (1001) docker     (123)    12774 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    18155 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_factory_constructors.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    16519 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_factory_constructors.py
--rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_gil_scoped.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     8540 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_gil_scoped.py
--rw-r--r--   0 runner    (1001) docker     (123)     3960 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_iostream.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7286 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_iostream.py
--rw-r--r--   0 runner    (1001) docker     (123)     9444 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_kwargs_and_defaults.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    13757 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_kwargs_and_defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_local_bindings.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     8049 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_local_bindings.py
--rw-r--r--   0 runner    (1001) docker     (123)    21388 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_methods_and_attributes.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    18134 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_methods_and_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_modules.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)    12305 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_multiple_inheritance.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    11874 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_multiple_inheritance.py
--rw-r--r--   0 runner    (1001) docker     (123)    19861 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_numpy_array.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    20356 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_numpy_array.py
--rw-r--r--   0 runner    (1001) docker     (123)    21114 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_numpy_dtypes.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    14394 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_numpy_dtypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4487 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_numpy_vectorize.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     9686 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_numpy_vectorize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_opaque_types.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_opaque_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     9132 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_operator_overloading.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4333 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_operator_overloading.py
--rw-r--r--   0 runner    (1001) docker     (123)     6719 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_pickling.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_pickling.py
--rw-r--r--   0 runner    (1001) docker     (123)    30750 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_pytypes.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    23630 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_pytypes.py
--rw-r--r--   0 runner    (1001) docker     (123)    21153 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_sequences_and_iterators.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     8021 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_sequences_and_iterators.py
--rw-r--r--   0 runner    (1001) docker     (123)    18898 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_smart_ptr.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     9530 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_smart_ptr.py
--rw-r--r--   0 runner    (1001) docker     (123)    21587 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_stl.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    12235 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_stl.py
--rw-r--r--   0 runner    (1001) docker     (123)     4622 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_stl_binders.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     9174 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_stl_binders.py
--rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_tagbased_polymorphic.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_tagbased_polymorphic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_thread.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_union.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_union.py
--rw-r--r--   0 runner    (1001) docker     (123)    22991 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_virtual_functions.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    12919 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_virtual_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/valgrind-numpy-scipy.supp
--rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/valgrind-python.supp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.444630 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tools/
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tools/FindCatch.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tools/FindEigen3.cmake
--rw-r--r--   0 runner    (1001) docker     (123)    11190 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tools/FindPythonLibsNew.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tools/JoinPaths.cmake
--rwxr-xr-x   0 runner    (1001) docker     (123)     1423 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tools/check-style.sh
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tools/cmake_uninstall.cmake.in
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tools/codespell_ignore_lines_from_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tools/libsize.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1311 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tools/make_changelog.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tools/pybind11.pc.in
--rw-r--r--   0 runner    (1001) docker     (123)    14033 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tools/pybind11Common.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     6930 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tools/pybind11Config.cmake.in
--rw-r--r--   0 runner    (1001) docker     (123)     8960 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tools/pybind11NewTools.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     8361 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tools/pybind11Tools.cmake
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tools/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tools/setup_global.py.in
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-04-14 16:07:23.000000 vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tools/setup_main.py.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.444630 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/
--rw-r--r--   0 runner    (1001) docker     (123)    12764 2023-04-14 16:07:25.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.448631 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/cmake/
--rw-r--r--   0 runner    (1001) docker     (123)     5945 2023-04-14 16:07:25.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/cmake/BuildFlatBuffers.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-04-14 16:07:25.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/cmake/DetectCXXStandard.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-14 16:07:25.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/cmake/FindDotnet.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-04-14 16:07:25.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/cmake/FindFlatbuffers.cmake
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-14 16:07:25.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/cmake/FindVSTest.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-04-14 16:07:25.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/cmake/FlatbufferUtils.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     8559 2023-04-14 16:07:25.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/cmake/NetFxNuget.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-04-14 16:07:25.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/cmake/NetFxResource.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-04-14 16:07:25.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/cmake/NetFxStrongName.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-04-14 16:07:25.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/cmake/T4Template.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-04-14 16:07:25.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/cmake/VWFlags.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-14 16:07:25.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/cmake/VowpalWabbitConfig.cmake.in
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-04-14 16:07:25.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/cmake/VowpalWabbitFeatures.cmake
--rw-r--r--   0 runner    (1001) docker     (123)    12409 2023-04-14 16:07:25.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/cmake/VowpalWabbitUtils.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-04-14 16:07:25.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/cmake/WindowsSetPath.cmake
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.448631 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/cmake/platforms/
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-04-14 16:07:25.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/cmake/platforms/win32.cmake
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.448631 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/ext_libs/
--rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-04-14 16:07:25.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/ext_libs/ext_libs.cmake
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.448631 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.448631 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/.nuget/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/.nuget/NuGet.Config
--rwxr-xr-x   0 runner    (1001) docker     (123)  5690456 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/.nuget/NuGet.exe
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.456631 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/active_interactor/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/active_interactor/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.456631 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/active_interactor/src/
--rw-r--r--   0 runner    (1001) docker     (123)     4328 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/active_interactor/src/active_interactor.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.456631 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/allreduce/
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/allreduce/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.384629 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/allreduce/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.384629 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/allreduce/include/vw/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.456631 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/allreduce/include/vw/allreduce/
--rw-r--r--   0 runner    (1001) docker     (123)     9981 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/allreduce/include/vw/allreduce/allreduce.h
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/allreduce/include/vw/allreduce/allreduce_type.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.456631 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/allreduce/src/
--rw-r--r--   0 runner    (1001) docker     (123)     9732 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/allreduce/src/allreduce_sockets.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/allreduce/src/allreduce_threads.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.456631 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/c_wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/c_wrapper/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.384629 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/c_wrapper/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.384629 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/c_wrapper/include/vw/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.460631 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/c_wrapper/include/vw/c_wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)     7478 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/c_wrapper/include/vw/c_wrapper/vwdll.h
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/c_wrapper/include/vw/c_wrapper/vwvis.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.460631 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/c_wrapper/src/
--rw-r--r--   0 runner    (1001) docker     (123)    17415 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/c_wrapper/src/vwdll.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.460631 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/c_wrapper/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3888 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/c_wrapper/tests/vwdll_test.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.460631 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/cache_parser/
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/cache_parser/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.384629 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/cache_parser/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.384629 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/cache_parser/include/vw/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.460631 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/cache_parser/include/vw/cache_parser/
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/cache_parser/include/vw/cache_parser/parse_example_cache.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.460631 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/cache_parser/src/
--rw-r--r--   0 runner    (1001) docker     (123)     8317 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/cache_parser/src/parse_example_cache.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.460631 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/cache_parser/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7194 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/cache_parser/tests/cache_test.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.460631 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/cli/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.460631 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/cli/src/
--rw-r--r--   0 runner    (1001) docker     (123)     4947 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/cli/src/main.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.460631 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/common/
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/common/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.384629 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/common/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.384629 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/common/include/vw/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.464631 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/common/include/vw/common/
--rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/common/include/vw/common/future_compat.h
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/common/include/vw/common/hash.h
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/common/include/vw/common/random.h
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/common/include/vw/common/random_details.h
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/common/include/vw/common/string_view.h
--rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/common/include/vw/common/text_utils.h
--rw-r--r--   0 runner    (1001) docker     (123)     5322 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/common/include/vw/common/vw_exception.h
--rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/common/include/vw/common/vw_throw.h
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/common/include/vw/common/vwvis.h
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/common/readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.464631 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/common/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/common/tests/basic_tokenize_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/common/tests/hash_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/common/tests/text_utils_test.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.464631 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/config/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.388629 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/config/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.388629 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/config/include/vw/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.464631 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/config/include/vw/config/
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/config/include/vw/config/cli_help_formatter.h
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/config/include/vw/config/cli_options_serializer.h
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/config/include/vw/config/help_formatter.h
--rw-r--r--   0 runner    (1001) docker     (123)     7059 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/config/include/vw/config/option.h
--rw-r--r--   0 runner    (1001) docker     (123)     3722 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/config/include/vw/config/option_builder.h
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/config/include/vw/config/option_group_definition.h
--rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/config/include/vw/config/options.h
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/config/include/vw/config/options_cli.h
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/config/include/vw/config/options_name_extractor.h
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/config/include/vw/config/options_serializer.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.468631 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/config/src/
--rw-r--r--   0 runner    (1001) docker     (123)     7191 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/config/src/cli_help_formatter.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/config/src/cli_options_serializer.cc
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/config/src/help_formatter.cc
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/config/src/option.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/config/src/option_group_definition.cc
--rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/config/src/options.cc
--rw-r--r--   0 runner    (1001) docker     (123)    18201 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/config/src/options_cli.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/config/src/options_name_extractor.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.468631 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/config/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    17448 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/config/tests/options_cli_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     7232 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/config/tests/options_test.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.468631 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/
--rw-r--r--   0 runner    (1001) docker     (123)    18128 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/config.h.in
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/gdb_pretty_printers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.388629 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.388629 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.488632 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/accumulate.h
--rw-r--r--   0 runner    (1001) docker     (123)     3710 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/action_score.h
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/active_multiclass_prediction.h
--rw-r--r--   0 runner    (1001) docker     (123)     9116 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/api_status.h
--rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/array_parameters.h
--rw-r--r--   0 runner    (1001) docker     (123)     4788 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/array_parameters_dense.h
--rw-r--r--   0 runner    (1001) docker     (123)     3984 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/array_parameters_sparse.h
--rw-r--r--   0 runner    (1001) docker     (123)    13611 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/automl_impl.h
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/best_constant.h
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/cache.h
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/cached_learner.h
--rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/cb.h
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/cb_continuous_label.h
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/cb_graph_feedback_reduction_features.h
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/cb_type.h
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/cb_with_observations_label.h
--rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/ccb_label.h
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/ccb_reduction_features.h
--rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/constant.h
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/continuous_actions_reduction_features.h
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/correctedMath.h
--rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/cost_sensitive.h
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/crossplat_compat.h
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/daemon_utils.h
--rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/debug_log.h
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/debug_print.h
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/decision_scores.h
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/epsilon_reduction_features.h
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/error_constants.h
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/error_data.h
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/error_reporting.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.488632 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/estimators/
--rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/estimators/confidence_sequence.h
--rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/estimators/confidence_sequence_robust.h
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/estimators/cressieread.h
--rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/estimators/distributionally_robust.h
--rw-r--r--   0 runner    (1001) docker     (123)     6549 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/example.h
--rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/example_predict.h
--rw-r--r--   0 runner    (1001) docker     (123)     4354 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/fast_pow10.h
--rw-r--r--   0 runner    (1001) docker     (123)    19482 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/feature_group.h
--rw-r--r--   0 runner    (1001) docker     (123)    11688 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/gd_predict.h
--rw-r--r--   0 runner    (1001) docker     (123)     9908 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/gen_cs_example.h
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/generic_range.h
--rw-r--r--   0 runner    (1001) docker     (123)    12364 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/global_data.h
--rw-r--r--   0 runner    (1001) docker     (123)     5787 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/guard.h
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/hashstring.h
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/input_parser.h
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/interaction_generation_state.h
--rw-r--r--   0 runner    (1001) docker     (123)    17022 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/interactions.h
--rw-r--r--   0 runner    (1001) docker     (123)    22064 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/interactions_predict.h
--rw-r--r--   0 runner    (1001) docker     (123)    12764 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/io_buf.h
--rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/kskip_ngram_transformer.h
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/label_dictionary.h
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/label_parser.h
--rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/label_type.h
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/large_action_space_reduction_features.h
--rw-r--r--   0 runner    (1001) docker     (123)    40886 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/learner.h
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/learner_fwd.h
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/loss_functions.h
--rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/memory.h
--rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/merge.h
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/metric_sink.h
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/metrics_collector.h
--rw-r--r--   0 runner    (1001) docker     (123)    12670 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/model_utils.h
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/multi_ex.h
--rw-r--r--   0 runner    (1001) docker     (123)     6266 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/multi_model_utils.h
--rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/multiclass.h
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/multilabel.h
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/named_labels.h
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/network.h
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/no_label.h
--rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/numeric_casts.h
--rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/object_pool.h
--rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/parse_args.h
--rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/parse_dispatch_loop.h
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/parse_example.h
--rw-r--r--   0 runner    (1001) docker     (123)     5762 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/parse_example_json.h
--rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/parse_primitives.h
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/parse_regressor.h
--rw-r--r--   0 runner    (1001) docker     (123)     3696 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/parse_slates_example_json.h
--rw-r--r--   0 runner    (1001) docker     (123)     4531 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/parser.h
--rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/polymorphic_ex.h
--rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/prediction_type.h
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/print_utils.h
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/prob_dist_cont.h
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/queue.h
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/rand_state.h
--rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reduction_features.h
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reduction_stack.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.500632 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/active.h
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/active_cover.h
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/audit_regressor.h
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/autolink.h
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/automl.h
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/baseline.h
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/baseline_challenger_cb.h
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/bfgs.h
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/binary.h
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/boosting.h
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/bs.h
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cats.h
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cats_pdf.h
--rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cats_tree.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.504632 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cb/
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cb/cb_actions_mask.h
--rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cb/cb_adf.h
--rw-r--r--   0 runner    (1001) docker     (123)     4298 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cb/cb_algs.h
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cb/cb_dro.h
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cb/cb_explore.h
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cb/cb_explore_adf_bag.h
--rw-r--r--   0 runner    (1001) docker     (123)    12923 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cb/cb_explore_adf_common.h
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cb/cb_explore_adf_cover.h
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cb/cb_explore_adf_first.h
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cb/cb_explore_adf_graph_feedback.h
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cb/cb_explore_adf_greedy.h
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cb/cb_explore_adf_large_action_space.h
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cb/cb_explore_adf_regcb.h
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cb/cb_explore_adf_rnd.h
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cb/cb_explore_adf_softmax.h
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cb/cb_explore_adf_squarecb.h
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cb/cb_explore_adf_synthcover.h
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cb/cb_explore_pdf.h
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cb/cb_sample.h
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cb/cb_to_cb_adf.h
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cb/cbify.h
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cb/warm_cb.h
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cbzo.h
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/classweight.h
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/conditional_contextual_bandit.h
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/confidence.h
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/count_label.h
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cs_active.h
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/csoaa.h
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/csoaa_ldf.h
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/ect.h
--rw-r--r--   0 runner    (1001) docker     (123)     4500 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/eigen_memory_tree.h
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/epsilon_decay.h
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/explore_eval.h
--rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/expreplay.h
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/freegrad.h
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/ftrl.h
--rw-r--r--   0 runner    (1001) docker     (123)    13588 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/gd.h
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/gd_mf.h
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/generate_interactions.h
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/get_pmf.h
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/interact.h
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/interaction_ground.h
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/kernel_svm.h
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/lda_core.h
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/log_multi.h
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/lrq.h
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/lrqfa.h
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/marginal.h
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/memory_tree.h
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/metrics.h
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/mf.h
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/multilabel_oaa.h
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/mwt.h
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/nn.h
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/noop.h
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/oaa.h
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/offset_tree.h
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/oja_newton.h
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/plt.h
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/pmf_to_pdf.h
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/print.h
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/recall_tree.h
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/sample_pdf.h
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/scorer.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.508632 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/search/
--rw-r--r--   0 runner    (1001) docker     (123)    14733 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/search/search.h
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/search/search_dep_parser.h
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/search/search_entityrelationtask.h
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/search/search_graph.h
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/search/search_hooktask.h
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/search/search_meta.h
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/search/search_multiclasstask.h
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/search/search_sequencetask.h
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/sender.h
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/shared_feature_merger.h
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/slates.h
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/stagewise_poly.h
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/svrg.h
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/topk.h
--rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/scope_exit.h
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/setup_base.h
--rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/shared_data.h
--rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/simple_label.h
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/simple_label_parser.h
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/slates_label.h
--rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/table_formatter.h
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/tag_utils.h
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/text_utils.h
--rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/thread_pool.h
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/unique_sort.h
--rw-r--r--   0 runner    (1001) docker     (123)    12504 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/v_array.h
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/v_array_pool.h
--rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/version.h
--rw-r--r--   0 runner    (1001) docker     (123)    16001 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/vw.h
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/vw_allreduce.h
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/vw_fwd.h
--rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/vw_math.h
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/vw_string_view_fmt.h
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/vw_validate.h
--rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/vw_versions.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.520632 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/
--rw-r--r--   0 runner    (1001) docker     (123)     4500 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/accumulate.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/action_score.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/api_status.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/array_parameters_dense.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/array_parameters_sparse.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/best_constant.cc
--rw-r--r--   0 runner    (1001) docker     (123)    12862 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/cb.cc
--rw-r--r--   0 runner    (1001) docker     (123)     9271 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/cb_continuous_label.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/cb_type.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/cb_with_observations_label.cc
--rw-r--r--   0 runner    (1001) docker     (123)    10292 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/ccb_label.cc
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/ccb_reduction_features.cc
--rw-r--r--   0 runner    (1001) docker     (123)    10374 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/confidence_sequence.cc
--rw-r--r--   0 runner    (1001) docker     (123)    12743 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/confidence_sequence_robust.cc
--rw-r--r--   0 runner    (1001) docker     (123)    14205 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/cost_sensitive.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/cressieread.cc
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/crossplat_compat.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/daemon_utils.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/debug_print.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/decision_scores.cc
--rw-r--r--   0 runner    (1001) docker     (123)    10813 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/distributionally_robust.cc
--rw-r--r--   0 runner    (1001) docker     (123)     5901 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/example.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/example_predict.cc
--rw-r--r--   0 runner    (1001) docker     (123)    11973 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/feature_group.cc
--rw-r--r--   0 runner    (1001) docker     (123)     6226 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/gen_cs_example.cc
--rw-r--r--   0 runner    (1001) docker     (123)    15562 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/global_data.cc
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/hashstring.cc
--rw-r--r--   0 runner    (1001) docker     (123)     5955 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/interactions.cc
--rw-r--r--   0 runner    (1001) docker     (123)     4323 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/io_buf.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/kskip_ngram_transformer.cc
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/label_dictionary.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/label_parser.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/label_type.cc
--rw-r--r--   0 runner    (1001) docker     (123)    25305 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/learner.cc
--rw-r--r--   0 runner    (1001) docker     (123)    17593 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/loss_functions.cc
--rw-r--r--   0 runner    (1001) docker     (123)    15560 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/merge.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/metric_sink.cc
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/metrics_collector.cc
--rw-r--r--   0 runner    (1001) docker     (123)     8671 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/multiclass.cc
--rw-r--r--   0 runner    (1001) docker     (123)     5709 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/multilabel.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/named_labels.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/network.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/no_label.cc
--rw-r--r--   0 runner    (1001) docker     (123)    71501 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/parse_args.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/parse_example_json.cc
--rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/parse_primitives.cc
--rw-r--r--   0 runner    (1001) docker     (123)    23602 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/parse_regressor.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/parse_slates_example_json.cc
--rw-r--r--   0 runner    (1001) docker     (123)    25242 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/parser.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/prediction_type.cc
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/print_utils.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/prob_dist_cont.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/qr_decomposition.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/qr_decomposition.h
--rw-r--r--   0 runner    (1001) docker     (123)    13992 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reduction_stack.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.536633 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/
--rw-r--r--   0 runner    (1001) docker     (123)     8826 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/active.cc
--rw-r--r--   0 runner    (1001) docker     (123)     8738 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/active_cover.cc
--rw-r--r--   0 runner    (1001) docker     (123)    11242 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/audit_regressor.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/autolink.cc
--rw-r--r--   0 runner    (1001) docker     (123)    16294 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/automl.cc
--rw-r--r--   0 runner    (1001) docker     (123)     7461 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/baseline.cc
--rw-r--r--   0 runner    (1001) docker     (123)     7886 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/baseline_challenger_cb.cc
--rw-r--r--   0 runner    (1001) docker     (123)    43374 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/bfgs.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/binary.cc
--rw-r--r--   0 runner    (1001) docker     (123)    12748 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/boosting.cc
--rw-r--r--   0 runner    (1001) docker     (123)     8784 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/bs.cc
--rw-r--r--   0 runner    (1001) docker     (123)     8166 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cats.cc
--rw-r--r--   0 runner    (1001) docker     (123)     6703 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cats_pdf.cc
--rw-r--r--   0 runner    (1001) docker     (123)    13351 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cats_tree.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.540633 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_actions_mask.cc
--rw-r--r--   0 runner    (1001) docker     (123)    18952 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_adf.cc
--rw-r--r--   0 runner    (1001) docker     (123)     8078 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_algs.cc
--rw-r--r--   0 runner    (1001) docker     (123)     6693 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_dro.cc
--rw-r--r--   0 runner    (1001) docker     (123)    15078 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_explore.cc
--rw-r--r--   0 runner    (1001) docker     (123)     8662 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_explore_adf_bag.cc
--rw-r--r--   0 runner    (1001) docker     (123)    13509 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_explore_adf_cover.cc
--rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_explore_adf_first.cc
--rw-r--r--   0 runner    (1001) docker     (123)    17726 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_explore_adf_graph_feedback.cc
--rw-r--r--   0 runner    (1001) docker     (123)     6479 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_explore_adf_greedy.cc
--rw-r--r--   0 runner    (1001) docker     (123)    16308 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_explore_adf_large_action_space.cc
--rw-r--r--   0 runner    (1001) docker     (123)    11451 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_explore_adf_regcb.cc
--rw-r--r--   0 runner    (1001) docker     (123)    11011 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_explore_adf_rnd.cc
--rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_explore_adf_softmax.cc
--rw-r--r--   0 runner    (1001) docker     (123)    15069 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_explore_adf_squarecb.cc
--rw-r--r--   0 runner    (1001) docker     (123)     8599 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_explore_adf_synthcover.cc
--rw-r--r--   0 runner    (1001) docker     (123)     5189 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_explore_pdf.cc
--rw-r--r--   0 runner    (1001) docker     (123)     5453 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_sample.cc
--rw-r--r--   0 runner    (1001) docker     (123)     9234 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_to_cb_adf.cc
--rw-r--r--   0 runner    (1001) docker     (123)    33290 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cbify.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.540633 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/details/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.540633 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/details/large_action/
--rw-r--r--   0 runner    (1001) docker     (123)     8438 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/details/large_action/compute_dot_prod_avx2.cc
--rw-r--r--   0 runner    (1001) docker     (123)     6918 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/details/large_action/compute_dot_prod_avx512.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/details/large_action/compute_dot_prod_scalar.h
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/details/large_action/compute_dot_prod_simd.h
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/details/large_action/kernel_impl.h
--rw-r--r--   0 runner    (1001) docker     (123)     8281 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/details/large_action/one_pass_svd_impl.cc
--rw-r--r--   0 runner    (1001) docker     (123)     5630 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/details/large_action/one_rank_spanner_impl.cc
--rw-r--r--   0 runner    (1001) docker     (123)     9101 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/details/large_action/two_pass_svd_impl.cc
--rw-r--r--   0 runner    (1001) docker     (123)     6410 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/details/large_action_space.h
--rw-r--r--   0 runner    (1001) docker     (123)    21426 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/warm_cb.cc
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cbzo.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/classweight.cc
--rw-r--r--   0 runner    (1001) docker     (123)    29402 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/conditional_contextual_bandit.cc
--rw-r--r--   0 runner    (1001) docker     (123)     5037 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/confidence.cc
--rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/count_label.cc
--rw-r--r--   0 runner    (1001) docker     (123)    17984 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cs_active.cc
--rw-r--r--   0 runner    (1001) docker     (123)     7449 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/csoaa.cc
--rw-r--r--   0 runner    (1001) docker     (123)    29074 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/csoaa_ldf.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.388629 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/details/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.544633 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/details/automl/
--rw-r--r--   0 runner    (1001) docker     (123)    22038 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/details/automl/automl_impl.cc
--rw-r--r--   0 runner    (1001) docker     (123)    11641 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/details/automl/automl_iomodel.cc
--rw-r--r--   0 runner    (1001) docker     (123)    16314 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/details/automl/automl_oracle.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/details/automl/automl_util.cc
--rw-r--r--   0 runner    (1001) docker     (123)    11040 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/ect.cc
--rw-r--r--   0 runner    (1001) docker     (123)    26112 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/eigen_memory_tree.cc
--rw-r--r--   0 runner    (1001) docker     (123)    17764 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/epsilon_decay.cc
--rw-r--r--   0 runner    (1001) docker     (123)    11154 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/explore_eval.cc
--rw-r--r--   0 runner    (1001) docker     (123)    15504 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/freegrad.cc
--rw-r--r--   0 runner    (1001) docker     (123)    17859 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/ftrl.cc
--rw-r--r--   0 runner    (1001) docker     (123)    59629 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/gd.cc
--rw-r--r--   0 runner    (1001) docker     (123)    14325 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/gd_mf.cc
--rw-r--r--   0 runner    (1001) docker     (123)    15935 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/generate_interactions.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/get_pmf.cc
--rw-r--r--   0 runner    (1001) docker     (123)     5371 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/interact.cc
--rw-r--r--   0 runner    (1001) docker     (123)    13618 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/interaction_ground.cc
--rw-r--r--   0 runner    (1001) docker     (123)    28050 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/kernel_svm.cc
--rw-r--r--   0 runner    (1001) docker     (123)    43203 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/lda_core.cc
--rw-r--r--   0 runner    (1001) docker     (123)    16107 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/log_multi.cc
--rw-r--r--   0 runner    (1001) docker     (123)     7520 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/lrq.cc
--rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/lrqfa.cc
--rw-r--r--   0 runner    (1001) docker     (123)    15470 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/marginal.cc
--rw-r--r--   0 runner    (1001) docker     (123)    43576 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/memory_tree.cc
--rw-r--r--   0 runner    (1001) docker     (123)     7288 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/metrics.cc
--rw-r--r--   0 runner    (1001) docker     (123)     7158 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/mf.cc
--rw-r--r--   0 runner    (1001) docker     (123)     6088 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/multilabel_oaa.cc
--rw-r--r--   0 runner    (1001) docker     (123)    10722 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/mwt.cc
--rw-r--r--   0 runner    (1001) docker     (123)    19362 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/nn.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/noop.cc
--rw-r--r--   0 runner    (1001) docker     (123)    17940 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/oaa.cc
--rw-r--r--   0 runner    (1001) docker     (123)     9544 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/offset_tree.cc
--rw-r--r--   0 runner    (1001) docker     (123)    18326 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/oja_newton.cc
--rw-r--r--   0 runner    (1001) docker     (123)    17033 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/plt.cc
--rw-r--r--   0 runner    (1001) docker     (123)     9585 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/pmf_to_pdf.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/print.cc
--rw-r--r--   0 runner    (1001) docker     (123)    18508 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/recall_tree.cc
--rw-r--r--   0 runner    (1001) docker     (123)     4543 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/sample_pdf.cc
--rw-r--r--   0 runner    (1001) docker     (123)     5397 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/scorer.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.544633 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/search/
--rw-r--r--   0 runner    (1001) docker     (123)   128057 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/search/search.cc
--rw-r--r--   0 runner    (1001) docker     (123)    28129 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/search/search_dep_parser.cc
--rw-r--r--   0 runner    (1001) docker     (123)    13787 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/search/search_entityrelationtask.cc
--rw-r--r--   0 runner    (1001) docker     (123)    14446 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/search/search_graph.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/search/search_hooktask.cc
--rw-r--r--   0 runner    (1001) docker     (123)     9707 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/search/search_meta.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/search/search_multiclasstask.cc
--rw-r--r--   0 runner    (1001) docker     (123)    16792 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/search/search_sequencetask.cc
--rw-r--r--   0 runner    (1001) docker     (123)     5883 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/sender.cc
--rw-r--r--   0 runner    (1001) docker     (123)     5915 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/shared_feature_merger.cc
--rw-r--r--   0 runner    (1001) docker     (123)    10321 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/slates.cc
--rw-r--r--   0 runner    (1001) docker     (123)    26700 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/stagewise_poly.cc
--rw-r--r--   0 runner    (1001) docker     (123)     6655 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/svrg.cc
--rw-r--r--   0 runner    (1001) docker     (123)     6531 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/topk.cc
--rw-r--r--   0 runner    (1001) docker     (123)    17088 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/shared_data.cc
--rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/simple_label.cc
--rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/simple_label_parser.cc
--rw-r--r--   0 runner    (1001) docker     (123)     6930 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/slates_label.cc
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/tag_utils.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/text_utils.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/unique_sort.cc
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/version.cc
--rw-r--r--   0 runner    (1001) docker     (123)    37769 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/vw.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/vw_validate.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.560633 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    42431 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/automl_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)    19805 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/automl_weights_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     5515 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/baseline_cb_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     5857 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/cats_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)    15806 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/cats_tree_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     5464 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/cats_user_provided_pdf.cc
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/cb_explore_adf_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/cb_graph_feedback_label_text_parse_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)    19204 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/cb_graph_feedback_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)    25071 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/cb_large_actions_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)    29915 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/cb_las_one_pass_svd_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)    32256 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/cb_las_spanner_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/cb_with_observations_parser_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     6619 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/ccb_parser_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/ccb_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/chain_hashing.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/confidence_sequence_robust_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/confidence_sequence_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     8593 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/continuous_actions_parser_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     7867 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/custom_reduction_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     4837 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/distributionally_robust_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     7907 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/eigen_memory_tree_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)    19314 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/epsilon_decay_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/epsilon_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     5790 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/example_ft_hash_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/example_header_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/example_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     5274 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/feature_group_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/flat_example_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/guard_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/hyperopt_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/igl_simulator.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/igl_simulator.h
--rw-r--r--   0 runner    (1001) docker     (123)    12721 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/igl_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)    21698 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/interactions_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)    17961 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/loss_functions_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/math_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)    18601 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/merge_header_opts_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)    18978 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/merge_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     5382 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/minimal_custom_reduction.cc
--rw-r--r--   0 runner    (1001) docker     (123)     4116 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/model_util_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/multiclass_label_parser_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/numeric_cast_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/object_pool_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     5911 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/offset_tree_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/parse_args_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/parser_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     7038 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/pmf_to_pdf_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/power_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/prediction_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/random_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     4543 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/save_load_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/scope_exit_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     9429 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/simulator.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/simulator.h
--rw-r--r--   0 runner    (1001) docker     (123)     6182 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/slates_parser_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     5196 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/slates_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/status_builder_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/tag_utils_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/thread_pool_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     4770 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/tokenize_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/tutorial_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     6719 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/v_array_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/vw_versions_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/weights_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/vw_types.natvis
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.560633 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/csv_parser/
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/csv_parser/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.388629 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/csv_parser/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.388629 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/csv_parser/include/vw/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.560633 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/csv_parser/include/vw/csv_parser/
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/csv_parser/include/vw/csv_parser/parse_example_csv.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.560633 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/csv_parser/src/
--rw-r--r--   0 runner    (1001) docker     (123)    18395 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/csv_parser/src/parse_example_csv.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.560633 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/csv_parser/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    27413 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/csv_parser/tests/csv_parser_test.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.560633 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/explore/
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/explore/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.388629 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/explore/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.388629 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/explore/include/vw/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.560633 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/explore/include/vw/explore/
--rw-r--r--   0 runner    (1001) docker     (123)    11110 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/explore/include/vw/explore/explore.h
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/explore/include/vw/explore/explore_error_codes.h
--rw-r--r--   0 runner    (1001) docker     (123)    15211 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/explore/include/vw/explore/explore_internal.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.560633 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/explore/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    17964 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/explore/tests/explore_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/explore/tests/main.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.560633 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/fb_parser/
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/fb_parser/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.392629 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/fb_parser/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.392629 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/fb_parser/include/vw/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.560633 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/fb_parser/include/vw/fb_parser/
--rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/fb_parser/include/vw/fb_parser/parse_example_flatbuffer.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.560633 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/fb_parser/schema/
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/fb_parser/schema/example.fbs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.560633 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/fb_parser/src/
--rw-r--r--   0 runner    (1001) docker     (123)     8764 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/fb_parser/src/parse_example_flatbuffer.cc
--rw-r--r--   0 runner    (1001) docker     (123)     5525 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/fb_parser/src/parse_label.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.560633 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/fb_parser/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7082 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/fb_parser/tests/flatbuffer_parser_test.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.564633 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/io/
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/io/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.392629 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/io/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.392629 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/io/include/vw/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.564633 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/io/include/vw/io/
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/io/include/vw/io/custom_streambuf.h
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/io/include/vw/io/errno_handling.h
--rw-r--r--   0 runner    (1001) docker     (123)     4085 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/io/include/vw/io/io_adapter.h
--rw-r--r--   0 runner    (1001) docker     (123)     9228 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/io/include/vw/io/logger.h
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/io/include/vw/io/owning_stream.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.564633 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/io/src/
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/io/src/errno_handling.cc
--rw-r--r--   0 runner    (1001) docker     (123)    12204 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/io/src/io_adapter.cc
--rw-r--r--   0 runner    (1001) docker     (123)     7753 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/io/src/logger.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.564633 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/io/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/io/tests/errno_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/io/tests/io_adapter_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/io/tests/ostream_test.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.564633 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/json_parser/
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/json_parser/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.392629 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/json_parser/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.392629 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/json_parser/include/vw/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.564633 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/json_parser/include/vw/json_parser/
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/json_parser/include/vw/json_parser/decision_service_utils.h
--rw-r--r--   0 runner    (1001) docker     (123)     4869 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/json_parser/include/vw/json_parser/parse_example_json.h
--rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/json_parser/include/vw/json_parser/parse_example_slates_json.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.564633 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/json_parser/src/
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/json_parser/src/json_utils.h
--rw-r--r--   0 runner    (1001) docker     (123)    67657 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/json_parser/src/parse_example_json.cc
--rw-r--r--   0 runner    (1001) docker     (123)    13980 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/json_parser/src/parse_example_slates_json.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.568633 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/json_parser/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    33219 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/json_parser/tests/dsjson_parser_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)    32067 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/json_parser/tests/json_parser_test.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.568633 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/model_merger/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/model_merger/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.568633 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/model_merger/src/
--rw-r--r--   0 runner    (1001) docker     (123)     7178 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/model_merger/src/main.cc
--rw-r--r--   0 runner    (1001) docker     (123)     5928 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.568633 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.392629 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.392629 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/include/vw/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.568633 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/include/vw/slim/
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/include/vw/slim/example_predict_builder.h
--rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/include/vw/slim/model_parser.h
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/include/vw/slim/opts.h
--rw-r--r--   0 runner    (1001) docker     (123)    16767 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/include/vw/slim/vw_slim_predict.h
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/include/vw/slim/vw_slim_return_codes.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.568633 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/src/example_predict_builder.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/src/model_parser.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/src/opts.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/src/vw_slim_predict.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.572633 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.580633 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/Delay_Margin_AudioNetworkPCR_all__unique_context.json
--rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/Delay_Margin_AudioNetworkPCR_all_cb_FF8.model
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/cb_data_5.model
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/cb_data_5.pred
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/cb_data_5.txt
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/cb_data_6.model
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/cb_data_6.pred
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/cb_data_6.pred2
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/cb_data_6.pred3
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/cb_data_7.model
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/cb_data_7.pred
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/cb_data_8.model
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/cb_data_8.pred
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/cb_data_9.model
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/cb_data_9.pred
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/cold_start.model
--rw-r--r--   0 runner    (1001) docker     (123)     4795 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/generate-data.sh
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/multiclass_data_4.model
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/multiclass_data_4.pred
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/multiclass_data_4.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/multiclass_data_5.pred
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/multiclass_data_5.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/regression_data_1.model
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/regression_data_1.pred
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/regression_data_1.txt
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/regression_data_2.model
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/regression_data_2.pred
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/regression_data_2.txt
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/regression_data_3.model
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/regression_data_3.pred
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/regression_data_3.txt
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/regression_data_4.model
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/regression_data_4.pred
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/regression_data_4.txt
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/regression_data_5.model
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/regression_data_5.pred
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/regression_data_6.model
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/regression_data_6.pred
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/regression_data_7.model
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/regression_data_7.pred
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/regression_data_7.txt
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/regression_data_ignore_linear.model
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/regression_data_ignore_linear.pred
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/regression_data_no-constant.model
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/regression_data_no-constant.pred
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/regression_data_no_constant.model
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/regression_data_no_constant.pred
--rw-r--r--   0 runner    (1001) docker     (123)    34194 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data.h
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/ut_explore.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/ut_opts.cc
--rw-r--r--   0 runner    (1001) docker     (123)    26186 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/ut_util.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.580633 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/spanning_tree/
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/spanning_tree/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.392629 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/spanning_tree/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.392629 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/spanning_tree/include/vw/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.580633 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/spanning_tree/include/vw/spanning_tree/
--rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/spanning_tree/include/vw/spanning_tree/spanning_tree.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.580633 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/spanning_tree/src/
--rw-r--r--   0 runner    (1001) docker     (123)     9865 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/spanning_tree/src/spanning_tree.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.580633 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/spanning_tree_bin/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/spanning_tree_bin/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.580633 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/spanning_tree_bin/src/
--rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/spanning_tree_bin/src/spanning_tree_main.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.580633 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/test_common/
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/test_common/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.396629 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/test_common/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.396629 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/test_common/include/vw/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.580633 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/test_common/include/vw/test_common/
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/test_common/include/vw/test_common/matchers.h
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/test_common/include/vw/test_common/test_common.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.580633 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/test_common/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/test_common/src/test_common.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.580633 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/text_parser/
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/text_parser/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.396629 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/text_parser/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.396629 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/text_parser/include/vw/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.580633 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/text_parser/include/vw/text_parser/
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/text_parser/include/vw/text_parser/parse_example_text.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.584634 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/text_parser/src/
--rw-r--r--   0 runner    (1001) docker     (123)    20528 2023-04-14 16:07:26.000000 vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/text_parser/src/parse_example_text.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-04-14 16:07:19.000000 vowpal-wabbit-next-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 16:07:39.592634 vowpal-wabbit-next-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-14 16:07:19.000000 vowpal-wabbit-next-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.396629 vowpal-wabbit-next-0.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.584634 vowpal-wabbit-next-0.4.0/src/cpp/
--rw-r--r--   0 runner    (1001) docker     (123)     8413 2023-04-14 16:07:19.000000 vowpal-wabbit-next-0.4.0/src/cpp/debug_reduction.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-04-14 16:07:19.000000 vowpal-wabbit-next-0.4.0/src/cpp/debug_reduction.h
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-04-14 16:07:19.000000 vowpal-wabbit-next-0.4.0/src/cpp/label.cc
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-04-14 16:07:19.000000 vowpal-wabbit-next-0.4.0/src/cpp/label.h
--rw-r--r--   0 runner    (1001) docker     (123)    70101 2023-04-14 16:07:19.000000 vowpal-wabbit-next-0.4.0/src/cpp/main.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-04-14 16:07:19.000000 vowpal-wabbit-next-0.4.0/src/cpp/prediction.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-04-14 16:07:19.000000 vowpal-wabbit-next-0.4.0/src/cpp/prediction.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.588634 vowpal-wabbit-next-0.4.0/src/vowpal_wabbit_next/
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-04-14 16:07:19.000000 vowpal-wabbit-next-0.4.0/src/vowpal_wabbit_next/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22271 2023-04-14 16:07:19.000000 vowpal-wabbit-next-0.4.0/src/vowpal_wabbit_next/_core.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4805 2023-04-14 16:07:19.000000 vowpal-wabbit-next-0.4.0/src/vowpal_wabbit_next/cache_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-04-14 16:07:19.000000 vowpal-wabbit-next-0.4.0/src/vowpal_wabbit_next/cli_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-04-14 16:07:19.000000 vowpal-wabbit-next-0.4.0/src/vowpal_wabbit_next/delta.py
--rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-04-14 16:07:19.000000 vowpal-wabbit-next-0.4.0/src/vowpal_wabbit_next/dsjson_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-04-14 16:07:19.000000 vowpal-wabbit-next-0.4.0/src/vowpal_wabbit_next/example.py
--rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-04-14 16:07:19.000000 vowpal-wabbit-next-0.4.0/src/vowpal_wabbit_next/json_format.py
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-14 16:07:19.000000 vowpal-wabbit-next-0.4.0/src/vowpal_wabbit_next/labels.py
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-14 16:07:19.000000 vowpal-wabbit-next-0.4.0/src/vowpal_wabbit_next/prediction_type.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:19.000000 vowpal-wabbit-next-0.4.0/src/vowpal_wabbit_next/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-04-14 16:07:19.000000 vowpal-wabbit-next-0.4.0/src/vowpal_wabbit_next/text_format.py
--rw-r--r--   0 runner    (1001) docker     (123)    18686 2023-04-14 16:07:19.000000 vowpal-wabbit-next-0.4.0/src/vowpal_wabbit_next/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.588634 vowpal-wabbit-next-0.4.0/src/vowpal_wabbit_next.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-04-14 16:07:39.000000 vowpal-wabbit-next-0.4.0/src/vowpal_wabbit_next.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    57641 2023-04-14 16:07:39.000000 vowpal-wabbit-next-0.4.0/src/vowpal_wabbit_next.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 16:07:39.000000 vowpal-wabbit-next-0.4.0/src/vowpal_wabbit_next.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-14 16:07:39.000000 vowpal-wabbit-next-0.4.0/src/vowpal_wabbit_next.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-14 16:07:39.000000 vowpal-wabbit-next-0.4.0/src/vowpal_wabbit_next.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:39.588634 vowpal-wabbit-next-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-04-14 16:07:19.000000 vowpal-wabbit-next-0.4.0/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-04-14 16:07:19.000000 vowpal-wabbit-next-0.4.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-04-14 16:07:19.000000 vowpal-wabbit-next-0.4.0/tests/test_debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     3949 2023-04-14 16:07:19.000000 vowpal-wabbit-next-0.4.0/tests/test_delta.py
--rw-r--r--   0 runner    (1001) docker     (123)    14367 2023-04-14 16:07:19.000000 vowpal-wabbit-next-0.4.0/tests/test_dsjson_format_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-04-14 16:07:19.000000 vowpal-wabbit-next-0.4.0/tests/test_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-04-14 16:07:19.000000 vowpal-wabbit-next-0.4.0/tests/test_json_format_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5428 2023-04-14 16:07:19.000000 vowpal-wabbit-next-0.4.0/tests/test_labels.py
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-04-14 16:07:19.000000 vowpal-wabbit-next-0.4.0/tests/test_learn.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-14 16:07:19.000000 vowpal-wabbit-next-0.4.0/tests/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-04-14 16:07:19.000000 vowpal-wabbit-next-0.4.0/tests/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-04-14 16:07:19.000000 vowpal-wabbit-next-0.4.0/tests/test_serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-04-14 16:07:19.000000 vowpal-wabbit-next-0.4.0/tests/test_text_format_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.763034 vowpal-wabbit-next-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-06-09 20:35:18.000000 vowpal-wabbit-next-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-09 20:35:18.000000 vowpal-wabbit-next-0.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-06-09 20:35:42.763034 vowpal-wabbit-next-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-06-09 20:35:18.000000 vowpal-wabbit-next-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.495030 vowpal-wabbit-next-0.4.1/ext_libs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.515031 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/.appveyor.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/.clang-format
+-rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/.clang-tidy
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/.cmake-format.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/.codespell-ignore-lines
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-09 20:35:18.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/.git
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.515031 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)    15271 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/.github/CONTRIBUTING.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.515031 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/.github/ISSUE_TEMPLATE/bug-report.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/.github/labeler.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/.github/labeler_merged.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.515031 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/.github/matchers/
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/.github/matchers/pylint.json
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.519031 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)    31868 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/.github/workflows/configure.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/.github/workflows/format.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/.github/workflows/labeler.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/.github/workflows/pip.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/.github/workflows/upstream.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    11983 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7686 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.523031 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/Doxyfile
+-rw-r--r--   0 runner    (1001) docker     (123)     7417 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.495030 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.523031 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/_static/css/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.523031 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/advanced/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.527031 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/advanced/cast/
+-rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/advanced/cast/chrono.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/advanced/cast/custom.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    14283 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/advanced/cast/eigen.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/advanced/cast/functional.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/advanced/cast/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12371 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/advanced/cast/overview.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9586 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/advanced/cast/stl.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8863 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/advanced/cast/strings.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    47796 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/advanced/classes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8453 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/advanced/embedding.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    17796 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/advanced/exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    26729 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/advanced/functions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    15651 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/advanced/misc.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.527031 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/advanced/pycpp/
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/advanced/pycpp/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    17161 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/advanced/pycpp/numpy.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9030 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/advanced/pycpp/object.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5710 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/advanced/pycpp/utilities.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6377 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/advanced/smart_ptrs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9240 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/basics.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/benchmark.rst
+-rw-r--r--   0 runner    (1001) docker     (123)   114174 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    16380 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/classes.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.527031 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/cmake/
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/cmake/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    25777 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/compiling.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11559 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13177 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/limitations.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    61034 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/pybind11-logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    44653 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/pybind11_vs_boost_python1.png
+-rw-r--r--   0 runner    (1001) docker     (123)    87708 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/pybind11_vs_boost_python1.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    41121 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/pybind11_vs_boost_python2.png
+-rw-r--r--   0 runner    (1001) docker     (123)    85853 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/pybind11_vs_boost_python2.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/reference.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/release.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    23489 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/upgrade.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.495030 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.531031 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/
+-rw-r--r--   0 runner    (1001) docker     (123)    23959 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/attr.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/buffer_info.h
+-rw-r--r--   0 runner    (1001) docker     (123)    65660 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/cast.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8458 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/chrono.h
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/common.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/complex.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.535031 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/detail/
+-rw-r--r--   0 runner    (1001) docker     (123)    28251 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/detail/class.h
+-rw-r--r--   0 runner    (1001) docker     (123)    52929 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/detail/common.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/detail/descr.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17869 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/detail/init.h
+-rw-r--r--   0 runner    (1001) docker     (123)    26305 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/detail/internals.h
+-rw-r--r--   0 runner    (1001) docker     (123)    42613 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/detail/type_caster_base.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/detail/typeid.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.535031 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/eigen/
+-rw-r--r--   0 runner    (1001) docker     (123)    31418 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/eigen/matrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18108 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/eigen/tensor.h
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/eigen.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13471 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/embed.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/eval.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/functional.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8262 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/gil.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8862 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/iostream.h
+-rw-r--r--   0 runner    (1001) docker     (123)    79408 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/numpy.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9103 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/operators.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/options.h
+-rw-r--r--   0 runner    (1001) docker     (123)   126420 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/pybind11.h
+-rw-r--r--   0 runner    (1001) docker     (123)    94641 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/pytypes.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.535031 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/stl/
+-rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/stl/filesystem.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15337 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/stl.h
+-rw-r--r--   0 runner    (1001) docker     (123)    29747 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/stl_bind.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/noxfile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.535031 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/pybind11/
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/pybind11/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/pybind11/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/pybind11/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/pybind11/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/pybind11/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    17609 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/pybind11/setup_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4877 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.567031 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    21675 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11736 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/constructor_stats.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/cross_module_gil_utils.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/cross_module_interleaved_error_already_set.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/eigen_tensor_avoid_stl_array.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.567031 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/extra_python_package/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/extra_python_package/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     8296 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/extra_python_package/test_files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.567031 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/extra_setuptools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/extra_setuptools/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/extra_setuptools/test_setuphelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/local_bindings.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5743 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/object.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/pybind11_cross_module_tests.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/pybind11_tests.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/pybind11_tests.h
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_async.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8567 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_buffers.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4841 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_buffers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16025 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_builtin_casters.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    17245 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_builtin_casters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_call_policies.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6549 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_call_policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10858 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_callbacks.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6246 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_chrono.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_chrono.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24874 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_class.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    14815 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_class.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.567031 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_cmake_build/
+-rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_cmake_build/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_cmake_build/embed.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.567031 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_cmake_build/installed_embed/
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.571031 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_cmake_build/installed_function/
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.571031 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_cmake_build/installed_target/
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_cmake_build/main.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.571031 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_cmake_build/subdirectory_embed/
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.571031 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_cmake_build/subdirectory_function/
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.571031 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_cmake_build/subdirectory_target/
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_cmake_build/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_const_name.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_const_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_constants_and_functions.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_constants_and_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10886 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_copy_move.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4796 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_copy_move.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7280 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_custom_type_casters.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_custom_type_casters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_custom_type_setup.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_custom_type_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4557 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_docstring_options.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_docstring_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19350 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_eigen_matrix.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    28867 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_eigen_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_eigen_tensor.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10590 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_eigen_tensor.inl
+-rw-r--r--   0 runner    (1001) docker     (123)     9456 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_eigen_tensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.571031 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_embed/
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_embed/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_embed/catch.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_embed/external_module.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    16535 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_embed/test_interpreter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_embed/test_interpreter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_embed/test_trampoline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5722 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_enum.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8903 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_eval.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_eval_call.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11904 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_exceptions.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_exceptions.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12774 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18155 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_factory_constructors.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    16519 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_factory_constructors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_gil_scoped.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8540 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_gil_scoped.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3960 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_iostream.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7286 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_iostream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9444 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_kwargs_and_defaults.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    13757 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_kwargs_and_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_local_bindings.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8049 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_local_bindings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21388 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_methods_and_attributes.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    18134 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_methods_and_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_modules.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12305 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_multiple_inheritance.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11874 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_multiple_inheritance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19861 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_numpy_array.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    20356 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_numpy_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21114 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_numpy_dtypes.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    14394 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_numpy_dtypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4487 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_numpy_vectorize.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9686 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_numpy_vectorize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_opaque_types.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_opaque_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9132 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_operator_overloading.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4333 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_operator_overloading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6719 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_pickling.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_pickling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30750 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_pytypes.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    23630 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_pytypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21153 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_sequences_and_iterators.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8021 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_sequences_and_iterators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18898 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_smart_ptr.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9530 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_smart_ptr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21587 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_stl.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    12235 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_stl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4622 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_stl_binders.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9174 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_stl_binders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_tagbased_polymorphic.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_tagbased_polymorphic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_thread.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_union.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_union.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22991 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_virtual_functions.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    12919 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_virtual_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/valgrind-numpy-scipy.supp
+-rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/valgrind-python.supp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.575032 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tools/FindCatch.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tools/FindEigen3.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)    11190 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tools/FindPythonLibsNew.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tools/JoinPaths.cmake
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1423 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tools/check-style.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tools/cmake_uninstall.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tools/codespell_ignore_lines_from_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tools/libsize.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1311 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tools/make_changelog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tools/pybind11.pc.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14033 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tools/pybind11Common.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     6930 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tools/pybind11Config.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8960 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tools/pybind11NewTools.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     8361 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tools/pybind11Tools.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tools/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tools/setup_global.py.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tools/setup_main.py.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.579032 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/
+-rw-r--r--   0 runner    (1001) docker     (123)    13189 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.583032 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/cmake/
+-rw-r--r--   0 runner    (1001) docker     (123)     5945 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/cmake/BuildFlatBuffers.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/cmake/DetectCXXStandard.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/cmake/FindDotnet.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/cmake/FindFlatbuffers.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/cmake/FindVSTest.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/cmake/FlatbufferUtils.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     8559 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/cmake/NetFxNuget.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/cmake/NetFxResource.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/cmake/NetFxStrongName.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/cmake/T4Template.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/cmake/VWFlags.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/cmake/VowpalWabbitConfig.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/cmake/VowpalWabbitFeatures.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)    12409 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/cmake/VowpalWabbitUtils.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/cmake/WindowsSetPath.cmake
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.583032 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/cmake/platforms/
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/cmake/platforms/win32.cmake
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.583032 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/ext_libs/
+-rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/ext_libs/ext_libs.cmake
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.583032 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.583032 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/.nuget/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/.nuget/NuGet.Config
+-rwxr-xr-x   0 runner    (1001) docker     (123)  5690456 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/.nuget/NuGet.exe
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.591032 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/active_interactor/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/active_interactor/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.591032 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/active_interactor/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     4328 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/active_interactor/src/active_interactor.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.595032 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/allreduce/
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/allreduce/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.499030 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/allreduce/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.499030 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/allreduce/include/vw/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.595032 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/allreduce/include/vw/allreduce/
+-rw-r--r--   0 runner    (1001) docker     (123)     9981 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/allreduce/include/vw/allreduce/allreduce.h
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/allreduce/include/vw/allreduce/allreduce_type.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.595032 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/allreduce/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     9732 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/allreduce/src/allreduce_sockets.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/allreduce/src/allreduce_threads.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.595032 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/c_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/c_wrapper/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.499030 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/c_wrapper/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.499030 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/c_wrapper/include/vw/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.595032 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/c_wrapper/include/vw/c_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)     7478 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/c_wrapper/include/vw/c_wrapper/vwdll.h
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/c_wrapper/include/vw/c_wrapper/vwvis.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.595032 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/c_wrapper/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    17415 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/c_wrapper/src/vwdll.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.595032 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/c_wrapper/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3888 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/c_wrapper/tests/vwdll_test.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.595032 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/cache_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/cache_parser/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.499030 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/cache_parser/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.499030 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/cache_parser/include/vw/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.595032 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/cache_parser/include/vw/cache_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/cache_parser/include/vw/cache_parser/parse_example_cache.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.595032 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/cache_parser/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     8317 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/cache_parser/src/parse_example_cache.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.599032 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/cache_parser/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7194 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/cache_parser/tests/cache_test.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.599032 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/cli/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.599032 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/cli/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     4947 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/cli/src/main.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.599032 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/common/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.499030 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/common/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.499030 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/common/include/vw/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.603032 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/common/include/vw/common/
+-rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/common/include/vw/common/future_compat.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/common/include/vw/common/hash.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/common/include/vw/common/random.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/common/include/vw/common/random_details.h
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/common/include/vw/common/string_view.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/common/include/vw/common/text_utils.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5322 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/common/include/vw/common/vw_exception.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/common/include/vw/common/vw_throw.h
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/common/include/vw/common/vwvis.h
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/common/readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.603032 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/common/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/common/tests/basic_tokenize_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/common/tests/hash_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/common/tests/text_utils_test.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.603032 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/config/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.499030 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/config/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.499030 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/config/include/vw/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.607032 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/config/include/vw/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/config/include/vw/config/cli_help_formatter.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/config/include/vw/config/cli_options_serializer.h
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/config/include/vw/config/help_formatter.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7059 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/config/include/vw/config/option.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/config/include/vw/config/option_builder.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/config/include/vw/config/option_group_definition.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/config/include/vw/config/options.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/config/include/vw/config/options_cli.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/config/include/vw/config/options_name_extractor.h
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/config/include/vw/config/options_serializer.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.607032 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/config/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     7191 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/config/src/cli_help_formatter.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/config/src/cli_options_serializer.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/config/src/help_formatter.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/config/src/option.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/config/src/option_group_definition.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/config/src/options.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    18201 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/config/src/options_cli.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/config/src/options_name_extractor.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.607032 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/config/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    17448 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/config/tests/options_cli_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     7232 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/config/tests/options_test.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.607032 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/
+-rw-r--r--   0 runner    (1001) docker     (123)    18182 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/config.h.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/gdb_pretty_printers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.499030 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.499030 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.631032 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/accumulate.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3710 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/action_score.h
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/active_multiclass_prediction.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9116 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/api_status.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/array_parameters.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4788 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/array_parameters_dense.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3984 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/array_parameters_sparse.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13611 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/automl_impl.h
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/best_constant.h
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/cache.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/cached_learner.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/cb.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/cb_continuous_label.h
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/cb_graph_feedback_reduction_features.h
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/cb_type.h
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/cb_with_observations_label.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/ccb_label.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/ccb_reduction_features.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/constant.h
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/continuous_actions_reduction_features.h
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/correctedMath.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/cost_sensitive.h
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/crossplat_compat.h
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/daemon_utils.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/debug_log.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/debug_print.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/decision_scores.h
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/epsilon_reduction_features.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/error_constants.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/error_data.h
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/error_reporting.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.631032 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/estimators/
+-rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/estimators/confidence_sequence.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/estimators/confidence_sequence_robust.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/estimators/cressieread.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/estimators/distributionally_robust.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6549 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/example.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/example_predict.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4354 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/fast_pow10.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19482 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/feature_group.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11688 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/gd_predict.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9908 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/gen_cs_example.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/generic_range.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12407 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/global_data.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5787 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/guard.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/hashstring.h
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/input_parser.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/interaction_generation_state.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17022 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/interactions.h
+-rw-r--r--   0 runner    (1001) docker     (123)    22064 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/interactions_predict.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12764 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/io_buf.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/kskip_ngram_transformer.h
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/label_dictionary.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/label_parser.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/label_type.h
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/large_action_space_reduction_features.h
+-rw-r--r--   0 runner    (1001) docker     (123)    40886 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/learner.h
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/learner_fwd.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/loss_functions.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/memory.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/merge.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/metric_sink.h
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/metrics_collector.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12670 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/model_utils.h
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/multi_ex.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6266 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/multi_model_utils.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/multiclass.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/multilabel.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/named_labels.h
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/network.h
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/no_label.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/numeric_casts.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/object_pool.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/parse_args.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/parse_dispatch_loop.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/parse_example.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5762 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/parse_example_json.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/parse_primitives.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/parse_regressor.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3696 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/parse_slates_example_json.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4531 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/parser.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/polymorphic_ex.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/prediction_type.h
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/print_utils.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/prob_dist_cont.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/queue.h
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/rand_state.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reduction_features.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reduction_stack.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.643032 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/active.h
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/active_cover.h
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/audit_regressor.h
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/autolink.h
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/automl.h
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/baseline.h
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/baseline_challenger_cb.h
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/bfgs.h
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/binary.h
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/boosting.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/bs.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cats.h
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cats_pdf.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cats_tree.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.647033 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cb/
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cb/cb_actions_mask.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cb/cb_adf.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4298 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cb/cb_algs.h
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cb/cb_dro.h
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cb/cb_explore.h
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cb/cb_explore_adf_bag.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13155 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cb/cb_explore_adf_common.h
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cb/cb_explore_adf_cover.h
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cb/cb_explore_adf_first.h
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cb/cb_explore_adf_graph_feedback.h
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cb/cb_explore_adf_greedy.h
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cb/cb_explore_adf_large_action_space.h
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cb/cb_explore_adf_regcb.h
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cb/cb_explore_adf_rnd.h
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cb/cb_explore_adf_softmax.h
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cb/cb_explore_adf_squarecb.h
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cb/cb_explore_adf_synthcover.h
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cb/cb_explore_pdf.h
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cb/cb_sample.h
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cb/cb_to_cb_adf.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cb/cbify.h
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cb/warm_cb.h
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cbzo.h
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/classweight.h
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/conditional_contextual_bandit.h
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/confidence.h
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/count_label.h
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cs_active.h
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/csoaa.h
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/csoaa_ldf.h
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/ect.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4814 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/eigen_memory_tree.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/epsilon_decay.h
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/explore_eval.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/expreplay.h
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/freegrad.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/ftrl.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13624 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/gd.h
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/gd_mf.h
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/generate_interactions.h
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/get_pmf.h
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/interact.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/interaction_ground.h
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/kernel_svm.h
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/lda_core.h
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/log_multi.h
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/lrq.h
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/lrqfa.h
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/marginal.h
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/memory_tree.h
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/metrics.h
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/mf.h
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/multilabel_oaa.h
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/mwt.h
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/nn.h
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/noop.h
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/oaa.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/offset_tree.h
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/oja_newton.h
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/plt.h
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/pmf_to_pdf.h
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/print.h
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/recall_tree.h
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/sample_pdf.h
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/scorer.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.651033 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/search/
+-rw-r--r--   0 runner    (1001) docker     (123)    14775 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/search/search.h
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/search/search_dep_parser.h
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/search/search_entityrelationtask.h
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/search/search_graph.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/search/search_hooktask.h
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/search/search_meta.h
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/search/search_multiclasstask.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/search/search_sequencetask.h
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/sender.h
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/shared_feature_merger.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/slates.h
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/stagewise_poly.h
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/svrg.h
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/topk.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/scope_exit.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/setup_base.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/shared_data.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/simple_label.h
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/simple_label_parser.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/slates_label.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/table_formatter.h
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/tag_utils.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/text_utils.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/thread_pool.h
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/unique_sort.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12504 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/v_array.h
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/v_array_pool.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/version.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16001 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/vw.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/vw_allreduce.h
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/vw_fwd.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/vw_math.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/vw_string_view_fmt.h
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/vw_validate.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/vw_versions.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.667033 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     4500 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/accumulate.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/action_score.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/api_status.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/array_parameters_dense.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/array_parameters_sparse.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/best_constant.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    12862 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/cb.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     9271 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/cb_continuous_label.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/cb_type.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/cb_with_observations_label.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    10292 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/ccb_label.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/ccb_reduction_features.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    10402 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/confidence_sequence.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    12743 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/confidence_sequence_robust.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    14205 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/cost_sensitive.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/cressieread.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/crossplat_compat.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/daemon_utils.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/debug_print.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/decision_scores.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    10813 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/distributionally_robust.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     5901 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/example.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/example_predict.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    11973 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/feature_group.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     6226 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/gen_cs_example.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    15603 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/global_data.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/hashstring.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     5955 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/interactions.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     4323 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/io_buf.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/kskip_ngram_transformer.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/label_dictionary.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/label_parser.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/label_type.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    25305 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/learner.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    17593 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/loss_functions.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    15560 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/merge.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/metric_sink.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/metrics_collector.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     8671 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/multiclass.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     5709 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/multilabel.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/named_labels.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/network.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/no_label.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    71631 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/parse_args.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/parse_example_json.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/parse_primitives.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    23602 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/parse_regressor.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/parse_slates_example_json.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    25478 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/parser.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/prediction_type.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/print_utils.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/prob_dist_cont.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/qr_decomposition.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/qr_decomposition.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14283 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reduction_stack.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.683033 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/
+-rw-r--r--   0 runner    (1001) docker     (123)     8826 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/active.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     8738 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/active_cover.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    11242 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/audit_regressor.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/autolink.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    16294 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/automl.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     7461 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/baseline.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     7886 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/baseline_challenger_cb.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    43374 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/bfgs.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/binary.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    12748 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/boosting.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     8784 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/bs.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     8166 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cats.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     6703 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cats_pdf.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    13351 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cats_tree.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.687033 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_actions_mask.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    20157 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_adf.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     8078 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_algs.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     6693 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_dro.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    15078 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_explore.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     8662 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_explore_adf_bag.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    13509 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_explore_adf_cover.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_explore_adf_first.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    19097 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_explore_adf_graph_feedback.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     6479 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_explore_adf_greedy.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    16308 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_explore_adf_large_action_space.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    11451 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_explore_adf_regcb.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    11011 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_explore_adf_rnd.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_explore_adf_softmax.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    15069 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_explore_adf_squarecb.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     8599 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_explore_adf_synthcover.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     5189 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_explore_pdf.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     5453 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_sample.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     9234 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_to_cb_adf.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    33290 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cbify.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.687033 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/details/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.691033 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/details/large_action/
+-rw-r--r--   0 runner    (1001) docker     (123)     8443 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/details/large_action/compute_dot_prod_avx2.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     6923 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/details/large_action/compute_dot_prod_avx512.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/details/large_action/compute_dot_prod_scalar.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/details/large_action/compute_dot_prod_simd.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/details/large_action/kernel_impl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8291 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/details/large_action/one_pass_svd_impl.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     5630 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/details/large_action/one_rank_spanner_impl.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     9101 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/details/large_action/two_pass_svd_impl.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     6420 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/details/large_action_space.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21426 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/warm_cb.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cbzo.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/classweight.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    29402 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/conditional_contextual_bandit.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     5037 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/confidence.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/count_label.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    17984 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cs_active.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     7449 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/csoaa.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    29074 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/csoaa_ldf.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.503031 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/details/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.691033 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/details/automl/
+-rw-r--r--   0 runner    (1001) docker     (123)    22038 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/details/automl/automl_impl.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    11641 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/details/automl/automl_iomodel.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    16314 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/details/automl/automl_oracle.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/details/automl/automl_util.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    11040 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/ect.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    30409 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/eigen_memory_tree.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    18593 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/epsilon_decay.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    11470 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/explore_eval.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    15504 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/freegrad.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    17859 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/ftrl.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    60815 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/gd.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    14325 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/gd_mf.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    15935 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/generate_interactions.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/get_pmf.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     5371 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/interact.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    15101 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/interaction_ground.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    28050 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/kernel_svm.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    43203 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/lda_core.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    16107 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/log_multi.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     7520 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/lrq.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/lrqfa.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    15470 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/marginal.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    43576 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/memory_tree.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     7288 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/metrics.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     7158 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/mf.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     6088 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/multilabel_oaa.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    10722 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/mwt.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    19362 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/nn.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/noop.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    17940 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/oaa.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     9544 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/offset_tree.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    18326 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/oja_newton.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    17033 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/plt.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     9585 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/pmf_to_pdf.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/print.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    18508 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/recall_tree.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     4543 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/sample_pdf.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     5397 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/scorer.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.695033 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/search/
+-rw-r--r--   0 runner    (1001) docker     (123)   128057 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/search/search.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    28129 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/search/search_dep_parser.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    13787 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/search/search_entityrelationtask.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    14446 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/search/search_graph.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/search/search_hooktask.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     9707 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/search/search_meta.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/search/search_multiclasstask.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    16792 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/search/search_sequencetask.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     5883 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/sender.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     5915 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/shared_feature_merger.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    10321 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/slates.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    26700 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/stagewise_poly.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     6655 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/svrg.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     6531 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/topk.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    17088 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/shared_data.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/simple_label.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/simple_label_parser.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     6930 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/slates_label.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/tag_utils.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/text_utils.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/unique_sort.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/version.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    37769 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/vw.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/vw_validate.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.719034 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    42431 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/automl_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    19805 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/automl_weights_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     5515 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/baseline_cb_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     5857 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/cats_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    15806 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/cats_tree_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     5464 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/cats_user_provided_pdf.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/cb_explore_adf_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     7933 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/cb_graph_feedback_label_parse_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    23932 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/cb_graph_feedback_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    25071 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/cb_large_actions_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    29920 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/cb_las_one_pass_svd_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    32256 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/cb_las_spanner_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/cb_with_observations_parser_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     6619 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/ccb_parser_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/ccb_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/chain_hashing.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/confidence_sequence_robust_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/confidence_sequence_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     8593 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/continuous_actions_parser_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     7867 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/custom_reduction_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     4837 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/distributionally_robust_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    10639 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/eigen_memory_tree_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    19389 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/epsilon_decay_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/epsilon_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     5790 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/example_ft_hash_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/example_header_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/example_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     5274 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/feature_group_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/flat_example_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/guard_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/hyperopt_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/igl_simulator.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/igl_simulator.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18684 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/igl_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    21698 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/interactions_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    17961 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/loss_functions_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/math_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    18601 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/merge_header_opts_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    18978 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/merge_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     5382 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/minimal_custom_reduction.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     4116 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/model_util_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/multiclass_label_parser_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/numeric_cast_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/object_pool_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     5911 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/offset_tree_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/parse_args_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/parser_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     7038 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/pmf_to_pdf_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/power_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/prediction_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/random_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     4543 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/save_load_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/scope_exit_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    14093 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/simulator.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     5415 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/simulator.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6182 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/slates_parser_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     5196 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/slates_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/status_builder_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/tag_utils_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/thread_pool_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     4770 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/tokenize_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/tutorial_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     6719 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/v_array_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/vw_versions_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/weights_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/vw_types.natvis
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.719034 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/csv_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/csv_parser/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.503031 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/csv_parser/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.503031 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/csv_parser/include/vw/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.719034 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/csv_parser/include/vw/csv_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/csv_parser/include/vw/csv_parser/parse_example_csv.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.719034 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/csv_parser/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    18395 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/csv_parser/src/parse_example_csv.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.719034 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/csv_parser/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    27413 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/csv_parser/tests/csv_parser_test.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.719034 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/explore/
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/explore/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.503031 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/explore/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.503031 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/explore/include/vw/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.719034 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/explore/include/vw/explore/
+-rw-r--r--   0 runner    (1001) docker     (123)    11110 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/explore/include/vw/explore/explore.h
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/explore/include/vw/explore/explore_error_codes.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15211 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/explore/include/vw/explore/explore_internal.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.719034 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/explore/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    17964 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/explore/tests/explore_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/explore/tests/main.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.723034 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/fb_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/fb_parser/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.503031 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/fb_parser/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.503031 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/fb_parser/include/vw/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.723034 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/fb_parser/include/vw/fb_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/fb_parser/include/vw/fb_parser/parse_example_flatbuffer.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.723034 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/fb_parser/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/fb_parser/schema/example.fbs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.723034 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/fb_parser/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     8764 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/fb_parser/src/parse_example_flatbuffer.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     5525 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/fb_parser/src/parse_label.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.723034 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/fb_parser/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7082 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/fb_parser/tests/flatbuffer_parser_test.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.723034 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/io/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.503031 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/io/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.503031 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/io/include/vw/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.727034 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/io/include/vw/io/
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/io/include/vw/io/custom_streambuf.h
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/io/include/vw/io/errno_handling.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4085 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/io/include/vw/io/io_adapter.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9228 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/io/include/vw/io/logger.h
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/io/include/vw/io/owning_stream.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.727034 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/io/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/io/src/errno_handling.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    12204 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/io/src/io_adapter.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     7753 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/io/src/logger.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.727034 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/io/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/io/tests/errno_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/io/tests/io_adapter_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/io/tests/ostream_test.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.727034 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/json_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/json_parser/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.507031 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/json_parser/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.507031 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/json_parser/include/vw/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.727034 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/json_parser/include/vw/json_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/json_parser/include/vw/json_parser/decision_service_utils.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4869 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/json_parser/include/vw/json_parser/parse_example_json.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/json_parser/include/vw/json_parser/parse_example_slates_json.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.727034 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/json_parser/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/json_parser/src/json_utils.h
+-rw-r--r--   0 runner    (1001) docker     (123)    70131 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/json_parser/src/parse_example_json.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    13980 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/json_parser/src/parse_example_slates_json.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.731034 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/json_parser/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    33219 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/json_parser/tests/dsjson_parser_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    32067 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/json_parser/tests/json_parser_test.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.731034 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/model_merger/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/model_merger/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.731034 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/model_merger/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     7178 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/model_merger/src/main.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     5928 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.731034 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.507031 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.507031 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/include/vw/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.731034 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/include/vw/slim/
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/include/vw/slim/example_predict_builder.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/include/vw/slim/model_parser.h
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/include/vw/slim/opts.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16767 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/include/vw/slim/vw_slim_predict.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/include/vw/slim/vw_slim_return_codes.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.731034 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/src/example_predict_builder.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/src/model_parser.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/src/opts.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/src/vw_slim_predict.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.735034 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.747034 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/Delay_Margin_AudioNetworkPCR_all__unique_context.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/Delay_Margin_AudioNetworkPCR_all_cb_FF8.model
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/cb_data_5.model
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/cb_data_5.pred
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/cb_data_5.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/cb_data_6.model
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/cb_data_6.pred
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/cb_data_6.pred2
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/cb_data_6.pred3
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/cb_data_7.model
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/cb_data_7.pred
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/cb_data_8.model
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/cb_data_8.pred
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/cb_data_9.model
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/cb_data_9.pred
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/cold_start.model
+-rw-r--r--   0 runner    (1001) docker     (123)     4795 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/generate-data.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/multiclass_data_4.model
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/multiclass_data_4.pred
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/multiclass_data_4.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/multiclass_data_5.pred
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/multiclass_data_5.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/regression_data_1.model
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/regression_data_1.pred
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/regression_data_1.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/regression_data_2.model
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/regression_data_2.pred
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/regression_data_2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/regression_data_3.model
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/regression_data_3.pred
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/regression_data_3.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/regression_data_4.model
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/regression_data_4.pred
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/regression_data_4.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/regression_data_5.model
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/regression_data_5.pred
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/regression_data_6.model
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/regression_data_6.pred
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/regression_data_7.model
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/regression_data_7.pred
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/regression_data_7.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/regression_data_ignore_linear.model
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/regression_data_ignore_linear.pred
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/regression_data_no-constant.model
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/regression_data_no-constant.pred
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/regression_data_no_constant.model
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/regression_data_no_constant.pred
+-rw-r--r--   0 runner    (1001) docker     (123)    34194 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/ut_explore.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/ut_opts.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    26186 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/ut_util.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.747034 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/spanning_tree/
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/spanning_tree/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.507031 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/spanning_tree/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.507031 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/spanning_tree/include/vw/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.747034 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/spanning_tree/include/vw/spanning_tree/
+-rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/spanning_tree/include/vw/spanning_tree/spanning_tree.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.747034 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/spanning_tree/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     9865 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/spanning_tree/src/spanning_tree.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.747034 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/spanning_tree_bin/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/spanning_tree_bin/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.747034 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/spanning_tree_bin/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/spanning_tree_bin/src/spanning_tree_main.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.747034 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/test_common/
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/test_common/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.507031 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/test_common/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.511031 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/test_common/include/vw/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.751034 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/test_common/include/vw/test_common/
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/test_common/include/vw/test_common/matchers.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/test_common/include/vw/test_common/test_common.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.751034 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/test_common/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/test_common/src/test_common.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.751034 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/text_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/text_parser/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.511031 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/text_parser/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.511031 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/text_parser/include/vw/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.751034 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/text_parser/include/vw/text_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/text_parser/include/vw/text_parser/parse_example_text.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.751034 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/text_parser/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    20528 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/text_parser/src/parse_example_text.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-06-09 20:35:18.000000 vowpal-wabbit-next-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 20:35:42.763034 vowpal-wabbit-next-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-06-09 20:35:18.000000 vowpal-wabbit-next-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.511031 vowpal-wabbit-next-0.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.759034 vowpal-wabbit-next-0.4.1/src/cpp/
+-rw-r--r--   0 runner    (1001) docker     (123)     8413 2023-06-09 20:35:18.000000 vowpal-wabbit-next-0.4.1/src/cpp/debug_reduction.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-06-09 20:35:18.000000 vowpal-wabbit-next-0.4.1/src/cpp/debug_reduction.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-06-09 20:35:18.000000 vowpal-wabbit-next-0.4.1/src/cpp/label.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-09 20:35:18.000000 vowpal-wabbit-next-0.4.1/src/cpp/label.h
+-rw-r--r--   0 runner    (1001) docker     (123)    71056 2023-06-09 20:35:18.000000 vowpal-wabbit-next-0.4.1/src/cpp/main.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-06-09 20:35:18.000000 vowpal-wabbit-next-0.4.1/src/cpp/prediction.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-09 20:35:18.000000 vowpal-wabbit-next-0.4.1/src/cpp/prediction.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.759034 vowpal-wabbit-next-0.4.1/src/vowpal_wabbit_next/
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-06-09 20:35:18.000000 vowpal-wabbit-next-0.4.1/src/vowpal_wabbit_next/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22271 2023-06-09 20:35:18.000000 vowpal-wabbit-next-0.4.1/src/vowpal_wabbit_next/_core.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4805 2023-06-09 20:35:18.000000 vowpal-wabbit-next-0.4.1/src/vowpal_wabbit_next/cache_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-06-09 20:35:18.000000 vowpal-wabbit-next-0.4.1/src/vowpal_wabbit_next/cli_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-06-09 20:35:18.000000 vowpal-wabbit-next-0.4.1/src/vowpal_wabbit_next/delta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-06-09 20:35:18.000000 vowpal-wabbit-next-0.4.1/src/vowpal_wabbit_next/dsjson_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-06-09 20:35:18.000000 vowpal-wabbit-next-0.4.1/src/vowpal_wabbit_next/example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-06-09 20:35:18.000000 vowpal-wabbit-next-0.4.1/src/vowpal_wabbit_next/json_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-09 20:35:18.000000 vowpal-wabbit-next-0.4.1/src/vowpal_wabbit_next/labels.py
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-09 20:35:18.000000 vowpal-wabbit-next-0.4.1/src/vowpal_wabbit_next/prediction_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:18.000000 vowpal-wabbit-next-0.4.1/src/vowpal_wabbit_next/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-06-09 20:35:18.000000 vowpal-wabbit-next-0.4.1/src/vowpal_wabbit_next/text_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18686 2023-06-09 20:35:18.000000 vowpal-wabbit-next-0.4.1/src/vowpal_wabbit_next/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.759034 vowpal-wabbit-next-0.4.1/src/vowpal_wabbit_next.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-06-09 20:35:42.000000 vowpal-wabbit-next-0.4.1/src/vowpal_wabbit_next.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    57636 2023-06-09 20:35:42.000000 vowpal-wabbit-next-0.4.1/src/vowpal_wabbit_next.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 20:35:42.000000 vowpal-wabbit-next-0.4.1/src/vowpal_wabbit_next.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-09 20:35:42.000000 vowpal-wabbit-next-0.4.1/src/vowpal_wabbit_next.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-09 20:35:42.000000 vowpal-wabbit-next-0.4.1/src/vowpal_wabbit_next.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.763034 vowpal-wabbit-next-0.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-06-09 20:35:18.000000 vowpal-wabbit-next-0.4.1/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-06-09 20:35:18.000000 vowpal-wabbit-next-0.4.1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-06-09 20:35:18.000000 vowpal-wabbit-next-0.4.1/tests/test_debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3949 2023-06-09 20:35:18.000000 vowpal-wabbit-next-0.4.1/tests/test_delta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14367 2023-06-09 20:35:18.000000 vowpal-wabbit-next-0.4.1/tests/test_dsjson_format_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-06-09 20:35:18.000000 vowpal-wabbit-next-0.4.1/tests/test_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-09 20:35:18.000000 vowpal-wabbit-next-0.4.1/tests/test_json_format_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5428 2023-06-09 20:35:18.000000 vowpal-wabbit-next-0.4.1/tests/test_labels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-06-09 20:35:18.000000 vowpal-wabbit-next-0.4.1/tests/test_learn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-09 20:35:18.000000 vowpal-wabbit-next-0.4.1/tests/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-06-09 20:35:18.000000 vowpal-wabbit-next-0.4.1/tests/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-09 20:35:18.000000 vowpal-wabbit-next-0.4.1/tests/test_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-06-09 20:35:18.000000 vowpal-wabbit-next-0.4.1/tests/test_text_format_reader.py
```

### Comparing `vowpal-wabbit-next-0.4.0/LICENSE` & `vowpal-wabbit-next-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/PKG-INFO` & `vowpal-wabbit-next-0.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vowpal-wabbit-next
-Version: 0.4.0
+Version: 0.4.1
 Summary: Experimental python bindings for VowpalWabbit
 Author: VowpalWabbit
 License: BSD-3-Clause
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -20,15 +20,15 @@
 ```sh
 pip install vowpal-wabbit-next
 ```
 
 ## Example
 
 ```python
-import vowpalwabbit_next as vw
+import vowpal_wabbit_next as vw
 import io
 
 cb_input = io.StringIO(
     """shared | s
 0:1:0.5 | a=0
 | a=1
```

### Comparing `vowpal-wabbit-next-0.4.0/README.md` & `vowpal-wabbit-next-0.4.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 ```sh
 pip install vowpal-wabbit-next
 ```
 
 ## Example
 
 ```python
-import vowpalwabbit_next as vw
+import vowpal_wabbit_next as vw
 import io
 
 cb_input = io.StringIO(
     """shared | s
 0:1:0.5 | a=0
 | a=1
```

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/.appveyor.yml` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/.appveyor.yml`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/.clang-format` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/.clang-format`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/.clang-tidy` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/.clang-tidy`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/.cmake-format.yaml` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/.cmake-format.yaml`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/.codespell-ignore-lines` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/.codespell-ignore-lines`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/.github/CONTRIBUTING.md` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/.github/ISSUE_TEMPLATE/bug-report.yml` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/.github/ISSUE_TEMPLATE/bug-report.yml`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/.github/matchers/pylint.json` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/.github/matchers/pylint.json`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/.github/pull_request_template.md` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/.github/workflows/ci.yml` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/.github/workflows/configure.yml` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/.github/workflows/configure.yml`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/.github/workflows/format.yml` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/.github/workflows/format.yml`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/.github/workflows/labeler.yml` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/.github/workflows/labeler.yml`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/.github/workflows/pip.yml` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/.github/workflows/pip.yml`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/.github/workflows/upstream.yml` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/.github/workflows/upstream.yml`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/.pre-commit-config.yaml` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/CMakeLists.txt` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/LICENSE` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/LICENSE`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/README.rst` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/README.rst`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/docs/Doxyfile` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/Doxyfile`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/docs/Makefile` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/Makefile`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/docs/advanced/cast/chrono.rst` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/advanced/cast/chrono.rst`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/docs/advanced/cast/custom.rst` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/advanced/cast/custom.rst`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/docs/advanced/cast/eigen.rst` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/advanced/cast/eigen.rst`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/docs/advanced/cast/functional.rst` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/advanced/cast/functional.rst`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/docs/advanced/cast/index.rst` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/advanced/cast/index.rst`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/docs/advanced/cast/overview.rst` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/advanced/cast/overview.rst`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/docs/advanced/cast/stl.rst` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/advanced/cast/stl.rst`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/docs/advanced/cast/strings.rst` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/advanced/cast/strings.rst`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/docs/advanced/classes.rst` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/advanced/classes.rst`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/docs/advanced/embedding.rst` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/advanced/embedding.rst`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/docs/advanced/exceptions.rst` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/advanced/exceptions.rst`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/docs/advanced/functions.rst` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/advanced/functions.rst`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/docs/advanced/misc.rst` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/advanced/misc.rst`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/docs/advanced/pycpp/numpy.rst` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/advanced/pycpp/numpy.rst`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/docs/advanced/pycpp/object.rst` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/advanced/pycpp/object.rst`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/docs/advanced/pycpp/utilities.rst` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/advanced/pycpp/utilities.rst`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/docs/advanced/smart_ptrs.rst` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/advanced/smart_ptrs.rst`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/docs/basics.rst` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/basics.rst`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/docs/benchmark.py` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/benchmark.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/docs/benchmark.rst` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/benchmark.rst`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/docs/changelog.rst` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/changelog.rst`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/docs/classes.rst` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/classes.rst`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/docs/compiling.rst` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/compiling.rst`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/docs/conf.py` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/conf.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/docs/faq.rst` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/docs/index.rst` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/index.rst`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/docs/installing.rst` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/installing.rst`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/docs/limitations.rst` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/limitations.rst`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/docs/pybind11-logo.png` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/pybind11-logo.png`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/docs/pybind11_vs_boost_python1.png` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/pybind11_vs_boost_python1.png`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/docs/pybind11_vs_boost_python1.svg` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/pybind11_vs_boost_python1.svg`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/docs/pybind11_vs_boost_python2.png` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/pybind11_vs_boost_python2.png`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/docs/pybind11_vs_boost_python2.svg` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/pybind11_vs_boost_python2.svg`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/docs/reference.rst` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/reference.rst`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/docs/release.rst` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/release.rst`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/docs/upgrade.rst` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/upgrade.rst`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/include/pybind11/attr.h` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/attr.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/include/pybind11/buffer_info.h` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/buffer_info.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/include/pybind11/cast.h` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/cast.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/include/pybind11/chrono.h` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/chrono.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/include/pybind11/complex.h` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/complex.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/include/pybind11/detail/class.h` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/detail/class.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/include/pybind11/detail/common.h` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/detail/common.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/include/pybind11/detail/descr.h` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/detail/descr.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/include/pybind11/detail/init.h` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/detail/init.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/include/pybind11/detail/internals.h` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/detail/internals.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/include/pybind11/detail/type_caster_base.h` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/detail/type_caster_base.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/include/pybind11/detail/typeid.h` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/detail/typeid.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/include/pybind11/eigen/matrix.h` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/eigen/matrix.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/include/pybind11/eigen/tensor.h` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/eigen/tensor.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/include/pybind11/embed.h` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/embed.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/include/pybind11/eval.h` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/eval.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/include/pybind11/functional.h` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/functional.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/include/pybind11/gil.h` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/gil.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/include/pybind11/iostream.h` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/iostream.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/include/pybind11/numpy.h` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/numpy.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/include/pybind11/operators.h` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/operators.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/include/pybind11/options.h` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/options.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/include/pybind11/pybind11.h` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/pybind11.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/include/pybind11/pytypes.h` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/pytypes.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/include/pybind11/stl/filesystem.h` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/stl/filesystem.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/include/pybind11/stl.h` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/stl.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/include/pybind11/stl_bind.h` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/stl_bind.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/noxfile.py` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/noxfile.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/pybind11/__main__.py` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/pybind11/__main__.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/pybind11/commands.py` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/pybind11/commands.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/pybind11/setup_helpers.py` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/pybind11/setup_helpers.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/pyproject.toml` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/pyproject.toml`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/setup.cfg` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/setup.cfg`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/setup.py` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/setup.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/CMakeLists.txt` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/conftest.py` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/constructor_stats.h` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/constructor_stats.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/cross_module_gil_utils.cpp` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/cross_module_gil_utils.cpp`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/cross_module_interleaved_error_already_set.cpp` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/cross_module_interleaved_error_already_set.cpp`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/env.py` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/env.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/extra_python_package/test_files.py` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/extra_python_package/test_files.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/extra_setuptools/test_setuphelper.py` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/extra_setuptools/test_setuphelper.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/local_bindings.h` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/local_bindings.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/object.h` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/object.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/pybind11_cross_module_tests.cpp` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/pybind11_cross_module_tests.cpp`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/pybind11_tests.cpp` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/pybind11_tests.cpp`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/pybind11_tests.h` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/pybind11_tests.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/pytest.ini` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/pytest.ini`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/requirements.txt` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/requirements.txt`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_async.cpp` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_async.cpp`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_async.py` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_async.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_buffers.cpp` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_buffers.cpp`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_buffers.py` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_buffers.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_builtin_casters.cpp` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_builtin_casters.cpp`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_builtin_casters.py` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_builtin_casters.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_call_policies.cpp` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_call_policies.cpp`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_call_policies.py` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_call_policies.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_callbacks.cpp` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_callbacks.cpp`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_callbacks.py` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_chrono.cpp` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_chrono.cpp`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_chrono.py` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_chrono.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_class.cpp` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_class.cpp`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_class.py` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_class.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_cmake_build/CMakeLists.txt` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_cmake_build/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_cmake_build/embed.cpp` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_cmake_build/embed.cpp`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_const_name.cpp` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_const_name.cpp`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_const_name.py` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_const_name.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_constants_and_functions.cpp` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_constants_and_functions.cpp`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_constants_and_functions.py` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_constants_and_functions.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_copy_move.cpp` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_copy_move.cpp`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_copy_move.py` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_copy_move.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_custom_type_casters.cpp` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_custom_type_casters.cpp`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_custom_type_casters.py` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_custom_type_casters.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_custom_type_setup.cpp` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_custom_type_setup.cpp`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_custom_type_setup.py` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_custom_type_setup.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_docstring_options.cpp` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_docstring_options.cpp`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_docstring_options.py` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_docstring_options.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_eigen_matrix.cpp` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_eigen_matrix.cpp`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_eigen_matrix.py` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_eigen_matrix.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_eigen_tensor.inl` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_eigen_tensor.inl`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_eigen_tensor.py` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_eigen_tensor.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_embed/CMakeLists.txt` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_embed/catch.cpp` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_embed/catch.cpp`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_embed/external_module.cpp` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_embed/external_module.cpp`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_embed/test_interpreter.cpp` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_embed/test_interpreter.cpp`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_enum.cpp` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_enum.cpp`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_enum.py` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_enum.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_eval.cpp` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_eval.cpp`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_eval.py` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_eval.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_exceptions.cpp` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_exceptions.cpp`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_exceptions.py` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_factory_constructors.cpp` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_factory_constructors.cpp`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_factory_constructors.py` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_factory_constructors.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_gil_scoped.cpp` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_gil_scoped.cpp`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_gil_scoped.py` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_gil_scoped.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_iostream.cpp` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_iostream.cpp`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_iostream.py` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_iostream.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_kwargs_and_defaults.cpp` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_kwargs_and_defaults.cpp`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_kwargs_and_defaults.py` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_kwargs_and_defaults.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_local_bindings.cpp` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_local_bindings.cpp`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_local_bindings.py` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_local_bindings.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_methods_and_attributes.cpp` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_methods_and_attributes.cpp`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_methods_and_attributes.py` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_methods_and_attributes.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_modules.cpp` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_modules.cpp`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_modules.py` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_modules.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_multiple_inheritance.cpp` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_multiple_inheritance.cpp`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_multiple_inheritance.py` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_multiple_inheritance.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_numpy_array.cpp` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_numpy_array.cpp`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_numpy_array.py` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_numpy_array.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_numpy_dtypes.cpp` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_numpy_dtypes.cpp`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_numpy_dtypes.py` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_numpy_dtypes.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_numpy_vectorize.cpp` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_numpy_vectorize.cpp`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_numpy_vectorize.py` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_numpy_vectorize.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_opaque_types.cpp` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_opaque_types.cpp`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_opaque_types.py` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_opaque_types.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_operator_overloading.cpp` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_operator_overloading.cpp`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_operator_overloading.py` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_operator_overloading.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_pickling.cpp` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_pickling.cpp`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_pickling.py` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_pickling.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_pytypes.cpp` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_pytypes.cpp`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_pytypes.py` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_pytypes.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_sequences_and_iterators.cpp` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_sequences_and_iterators.cpp`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_sequences_and_iterators.py` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_sequences_and_iterators.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_smart_ptr.cpp` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_smart_ptr.cpp`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_smart_ptr.py` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_smart_ptr.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_stl.cpp` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_stl.cpp`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_stl.py` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_stl.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_stl_binders.cpp` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_stl_binders.cpp`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_stl_binders.py` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_stl_binders.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_tagbased_polymorphic.cpp` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_tagbased_polymorphic.cpp`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_tagbased_polymorphic.py` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_tagbased_polymorphic.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_thread.cpp` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_thread.cpp`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_thread.py` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_thread.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_union.cpp` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_union.cpp`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_virtual_functions.cpp` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_virtual_functions.cpp`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/test_virtual_functions.py` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_virtual_functions.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/valgrind-numpy-scipy.supp` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/valgrind-numpy-scipy.supp`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tests/valgrind-python.supp` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/valgrind-python.supp`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tools/FindCatch.cmake` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tools/FindCatch.cmake`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tools/FindEigen3.cmake` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tools/FindEigen3.cmake`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tools/FindPythonLibsNew.cmake` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tools/FindPythonLibsNew.cmake`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tools/JoinPaths.cmake` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tools/JoinPaths.cmake`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tools/check-style.sh` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tools/check-style.sh`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tools/cmake_uninstall.cmake.in` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tools/cmake_uninstall.cmake.in`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tools/codespell_ignore_lines_from_errors.py` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tools/codespell_ignore_lines_from_errors.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tools/libsize.py` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tools/libsize.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tools/make_changelog.py` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tools/make_changelog.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tools/pybind11Common.cmake` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tools/pybind11Common.cmake`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tools/pybind11Config.cmake.in` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tools/pybind11Config.cmake.in`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tools/pybind11NewTools.cmake` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tools/pybind11NewTools.cmake`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tools/pybind11Tools.cmake` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tools/pybind11Tools.cmake`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tools/setup_global.py.in` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tools/setup_global.py.in`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/pybind11/tools/setup_main.py.in` & `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tools/setup_main.py.in`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/CMakeLists.txt` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/CMakeLists.txt`

 * *Files 3% similar despite different names*

```diff
@@ -71,14 +71,22 @@
 endif()
 
 # CMake project() does not support semantic versioning
 project(vowpal_wabbit VERSION "${VW_VERSION_MAJOR}.${VW_VERSION_MINOR}.${VW_VERSION_PATCH}" LANGUAGES C CXX)
 set(VW_PROJECT_DESCRIPTION "Vowpal Wabbit Machine Learning System")
 set(VW_PROJECT_URL "https://vowpalwabbit.org")
 
+# This must be checked after the project call since we need to check CMAKE_SYSTEM_PROCESSOR
+# It must be done before we include VowpalWabbitUtils
+if (VW_FEAT_LAS_SIMD AND NOT ((UNIX AND NOT APPLE) AND (${CMAKE_SYSTEM_PROCESSOR} STREQUAL "x86_64")))
+  message(STATUS "LAS SIMD was requested but is only supported on x86_64 Linux and so was disabled.")
+  # Set the cmake option to off
+  set(VW_FEAT_LAS_SIMD OFF CACHE BOOL "" FORCE)
+endif()
+
 vw_print_enabled_features()
 
 option(USE_LATEST_STD "Override using C++11 with the latest standard the compiler offers. Default is C++11. " OFF)
 include(DetectCXXStandard)
 if(NOT VW_CXX_STANDARD)
   set(VW_CXX_STANDARD 11)
 endif()
@@ -138,19 +146,19 @@
 option(VW_BOOST_MATH_SYS_DEP "Override using the submodule for boost math dependency. Instead will use find_package" OFF)
 option(VW_ZLIB_SYS_DEP "Override using the submodule for zlib dependency. Instead will use find_package" ON)
 option(VW_GTEST_SYS_DEP "Override using fetch package for gtest dependency. Instead will use find_package" OFF)
 option(VW_EIGEN_SYS_DEP "Override using the submodule for Eigen3 dependency. Instead will use find_package" OFF)
 option(VW_STRING_VIEW_LITE_SYS_DEP "Override using the submodule for string-view-lite dependency. Instead will use find_package" OFF)
 option(VW_SSE2NEON_SYS_DEP "Override using the submodule for SSE2Neon dependency. Instead will use find_package" OFF)
 option(VW_BUILD_VW_C_WRAPPER "Enable building the c_wrapper project" ON)
-option(VW_BUILD_LAS_WITH_SIMD "Build large action space with explicit simd (only work with linux for now)" ON)
 option(vw_BUILD_NET_CORE "Build .NET Core targets" OFF)
 option(vw_BUILD_NET_FRAMEWORK "Build .NET Framework targets" OFF)
 option(VW_USE_ASAN "Compile with AddressSanitizer" OFF)
 option(VW_USE_UBSAN "Compile with UndefinedBehaviorSanitizer" OFF)
+option(VW_BUILD_WASM "Add WASM target" OFF)
 
 if(VW_USE_ASAN)
   add_compile_definitions(VW_USE_ASAN)
   if(MSVC)
     add_compile_options(/fsanitize=address /GS- /wd5072)
     add_link_options(/InferASanLibs /incremental:no /debug)
     # Workaround for MSVC ASan issue here: https://developercommunity.visualstudio.com/t/VS2022---Address-sanitizer-on-x86-Debug-/10116361
@@ -249,14 +257,18 @@
   add_subdirectory(python)
 endif()
 
 if(BUILD_BENCHMARKS)
   add_subdirectory(test/benchmarks)
 endif()
 
+if(VW_BUILD_WASM)
+  add_subdirectory(wasm)
+endif()
+
 if(CMAKE_PROJECT_NAME STREQUAL PROJECT_NAME AND BUILD_TESTING)
   add_subdirectory(test)
 
   # Don't offer these make dependent targets on Windows
   if(NOT WIN32)
     # make bigtests BIG_TEST_ARGS="<args here>"
     add_custom_target(bigtests
```

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/cmake/BuildFlatBuffers.cmake` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/cmake/BuildFlatBuffers.cmake`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/cmake/DetectCXXStandard.cmake` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/cmake/DetectCXXStandard.cmake`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/cmake/FindFlatbuffers.cmake` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/cmake/FindFlatbuffers.cmake`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/cmake/FlatbufferUtils.cmake` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/cmake/FlatbufferUtils.cmake`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/cmake/NetFxNuget.cmake` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/cmake/NetFxNuget.cmake`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/cmake/NetFxResource.cmake` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/cmake/NetFxResource.cmake`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/cmake/NetFxStrongName.cmake` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/cmake/NetFxStrongName.cmake`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/cmake/T4Template.cmake` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/cmake/T4Template.cmake`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/cmake/VWFlags.cmake` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/cmake/VWFlags.cmake`

 * *Files 4% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
 # Turn on warnings
 set(WARNING_OPTIONS "")
 if(WARNINGS)
   if(WIN32)
     set(WARNING_OPTIONS /W4)
   else()
-    set(WARNING_OPTIONS -Wall -Wextra -Wpedantic)
+    set(WARNING_OPTIONS -Wall -Wextra -Wpedantic -Wswitch)
   endif()
 endif(WARNINGS)
 
 # Turn on warnings as errors
 set(WARNING_AS_ERROR_OPTIONS "")
 if(WARNING_AS_ERROR)
   if(WIN32)
```

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/cmake/VowpalWabbitFeatures.cmake` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/cmake/VowpalWabbitFeatures.cmake`

 * *Files 11% similar despite different names*

```diff
@@ -5,37 +5,39 @@
 #   - Specifying individual features with -DVW_FEATURE_FEAT1=ON/OFF
 #
 # This allows us to enable/disable features without changing the code
 # If a feature called X is enabled then:
 #   - The cmake variable VW_FEAT_X is set to ON, otherwise it is OFF
 #   - The C++ macro VW_FEAT_X_ENABLED is defined if the feature is enabled, otherwise it is not defined
 
-set(VW_ALL_FEATURES "CSV;FLATBUFFERS;LDA;CB_GRAPH_FEEDBACK")
+set(VW_ALL_FEATURES "CSV;FLATBUFFERS;LDA;CB_GRAPH_FEEDBACK;SEARCH;LAS_SIMD;NETWORKING")
 
 option(VW_FEAT_FLATBUFFERS "Enable flatbuffers support" OFF)
 option(VW_FEAT_CSV "Enable csv parser" OFF)
 option(VW_FEAT_CB_GRAPH_FEEDBACK "Enable cb with graph feedback reduction" OFF)
 option(VW_FEAT_LDA "Enable lda reduction" ON)
-# option(VW_FEAT_LAS_SIMD "Enable large action space with explicit simd (only works with linux for now)" ON)
+option(VW_FEAT_SEARCH "Enable search reductions" ON)
+option(VW_FEAT_LAS_SIMD "Enable large action space with explicit simd (only works with linux for now)" ON)
+option(VW_FEAT_NETWORKING "Enable daemon mode, spanning tree, sender, and active" ON)
 
 # Legacy options for feature enablement
 if(DEFINED BUILD_FLATBUFFERS)
   message(WARNING "BUILD_FLATBUFFERS is deprecated. Use -DVW_FEAT_FLATBUFFERS=On instead.")
   set(VW_FEAT_FLATBUFFERS ${BUILD_FLATBUFFERS} CACHE BOOL "" FORCE)
 endif()
 
 if(DEFINED VW_BUILD_CSV)
   message(WARNING "VW_BUILD_CSV is deprecated. Use -DVW_FEAT_CSV=On instead.")
   set(VW_FEAT_CSV ${VW_BUILD_CSV} CACHE BOOL "" FORCE)
 endif()
 
-# if(DEFINED VW_BUILD_LAS_WITH_SIMD)
-#   message(WARNING "VW_BUILD_LAS_WITH_SIMD is deprecated. Use -DVW_FEAT_LAS_SIMD=On instead.")
-#   set(VW_FEAT_LAS_SIMD ${VW_BUILD_LAS_WITH_SIMD} CACHE BOOL "" FORCE)
-# endif()
+if(DEFINED VW_BUILD_LAS_WITH_SIMD)
+  message(WARNING "VW_BUILD_LAS_WITH_SIMD is deprecated. Use -DVW_FEAT_LAS_SIMD=On instead.")
+  set(VW_FEAT_LAS_SIMD ${VW_BUILD_LAS_WITH_SIMD} CACHE BOOL "" FORCE)
+endif()
 
 function(vw_print_enabled_features)
   foreach(feature ${VW_ALL_FEATURES})
     if(VW_FEAT_${feature})
       list(APPEND ALL_ENABLED_FEATURES ${feature})
     endif()
   endforeach()
```

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/cmake/VowpalWabbitUtils.cmake` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/cmake/VowpalWabbitUtils.cmake`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/cmake/WindowsSetPath.cmake` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/cmake/WindowsSetPath.cmake`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/cmake/platforms/win32.cmake` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/cmake/platforms/win32.cmake`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/ext_libs/ext_libs.cmake` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/ext_libs/ext_libs.cmake`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/.nuget/NuGet.exe` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/.nuget/NuGet.exe`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/CMakeLists.txt` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/CMakeLists.txt`

 * *Files 18% similar despite different names*

```diff
@@ -12,16 +12,18 @@
   add_subdirectory(csv_parser)
 endif()
 add_subdirectory(explore)
 add_subdirectory(io)
 add_subdirectory(json_parser)
 add_subdirectory(model_merger)
 add_subdirectory(slim)
-add_subdirectory(spanning_tree_bin)
-add_subdirectory(spanning_tree)
+if(VW_FEAT_NETWORKING)
+  add_subdirectory(spanning_tree_bin)
+  add_subdirectory(spanning_tree)
+endif()
 add_subdirectory(text_parser)
 if(CMAKE_PROJECT_NAME STREQUAL PROJECT_NAME AND BUILD_TESTING)
   add_subdirectory(test_common)
 endif()
 if(VW_FEAT_FLATBUFFERS)
   add_subdirectory(fb_parser)
 endif()
```

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/active_interactor/src/active_interactor.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/active_interactor/src/active_interactor.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/allreduce/CMakeLists.txt` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/allreduce/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/allreduce/include/vw/allreduce/allreduce.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/allreduce/include/vw/allreduce/allreduce.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/allreduce/src/allreduce_sockets.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/allreduce/src/allreduce_sockets.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/allreduce/src/allreduce_threads.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/allreduce/src/allreduce_threads.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/c_wrapper/CMakeLists.txt` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/c_wrapper/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/c_wrapper/include/vw/c_wrapper/vwdll.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/c_wrapper/include/vw/c_wrapper/vwdll.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/c_wrapper/include/vw/c_wrapper/vwvis.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/c_wrapper/include/vw/c_wrapper/vwvis.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/c_wrapper/src/vwdll.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/c_wrapper/src/vwdll.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/c_wrapper/tests/vwdll_test.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/c_wrapper/tests/vwdll_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/cache_parser/include/vw/cache_parser/parse_example_cache.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/cache_parser/include/vw/cache_parser/parse_example_cache.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/cache_parser/src/parse_example_cache.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/cache_parser/src/parse_example_cache.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/cache_parser/tests/cache_test.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/cache_parser/tests/cache_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/cli/CMakeLists.txt` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/cli/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/cli/src/main.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/cli/src/main.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/common/CMakeLists.txt` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/common/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/common/include/vw/common/future_compat.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/common/include/vw/common/future_compat.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/common/include/vw/common/hash.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/common/include/vw/common/hash.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/common/include/vw/common/random.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/common/include/vw/common/random.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/common/include/vw/common/random_details.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/common/include/vw/common/random_details.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/common/include/vw/common/text_utils.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/common/include/vw/common/text_utils.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/common/include/vw/common/vw_exception.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/common/include/vw/common/vw_exception.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/common/include/vw/common/vw_throw.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/common/include/vw/common/vw_throw.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/common/include/vw/common/vwvis.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/common/include/vw/common/vwvis.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/common/tests/basic_tokenize_test.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/common/tests/basic_tokenize_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/common/tests/hash_test.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/common/tests/hash_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/common/tests/text_utils_test.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/common/tests/text_utils_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/config/CMakeLists.txt` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/config/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/config/include/vw/config/cli_options_serializer.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/config/include/vw/config/cli_options_serializer.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/config/include/vw/config/help_formatter.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/config/include/vw/config/help_formatter.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/config/include/vw/config/option.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/config/include/vw/config/option.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/config/include/vw/config/option_builder.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/config/include/vw/config/option_builder.h`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 {
 };
 
 template <typename T>
 class is_vector<T,
     typename std::enable_if<std::is_same<typename std::decay<T>::type,
         std::vector<typename std::decay<T>::type::value_type, typename std::decay<T>::type::allocator_type>>::value>::
-        type> : std::true_type
+        type> : public std::true_type
 {
 };
 
 }  // namespace details
 
 class base_option;
 
@@ -107,20 +107,18 @@
 
   option_builder& one_of(std::set<typename T::value_type> args)
   {
     _option_obj.set_one_of(args);
     return *this;
   }
 
-  option_builder& allow_override(bool allow_override = true)
+  template <typename U = T>
+  typename std::enable_if<!details::is_vector<typename U::value_type>::value, option_builder&>::type allow_override(
+      bool allow_override = true)
   {
-    if (details::is_vector<typename T::value_type>::value)
-    {
-      THROW("allow_override can only apply to scalar option types.")
-    }
     _option_obj.m_allow_override = allow_override;
     return *this;
   }
 
   static std::shared_ptr<base_option> finalize(option_builder&& option)
   {
     return std::make_shared<T>(std::move(option._option_obj));
```

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/config/include/vw/config/option_group_definition.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/config/include/vw/config/option_group_definition.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/config/include/vw/config/options.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/config/include/vw/config/options.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/config/include/vw/config/options_cli.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/config/include/vw/config/options_cli.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/config/include/vw/config/options_name_extractor.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/config/include/vw/config/options_name_extractor.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/config/include/vw/config/options_serializer.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/config/include/vw/config/options_serializer.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/config/src/cli_help_formatter.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/config/src/cli_help_formatter.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/config/src/cli_options_serializer.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/config/src/cli_options_serializer.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/config/src/help_formatter.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/config/src/help_formatter.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/config/src/option.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/config/src/option.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/config/src/option_group_definition.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/config/src/option_group_definition.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/config/src/options.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/config/src/options.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/config/src/options_cli.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/config/src/options_cli.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/config/src/options_name_extractor.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/config/src/options_name_extractor.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/config/tests/options_cli_test.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/config/tests/options_cli_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/config/tests/options_test.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/config/tests/options_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/CMakeLists.txt` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/CMakeLists.txt`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,14 @@
   include/vw/core/best_constant.h
   include/vw/core/cache.h
   include/vw/core/cached_learner.h
   include/vw/core/cb_continuous_label.h
   include/vw/core/cb_graph_feedback_reduction_features.h
   include/vw/core/multi_ex.h
   include/vw/core/learner_fwd.h
-  include/vw/core/daemon_utils.h
   include/vw/core/cb_type.h
   include/vw/core/cb.h
   include/vw/core/cb_with_observations_label.h
   include/vw/core/ccb_label.h
   include/vw/core/ccb_reduction_features.h
   include/vw/core/estimators/confidence_sequence.h
   include/vw/core/estimators/confidence_sequence_robust.h
@@ -61,15 +60,14 @@
   include/vw/core/metrics_collector.h
   include/vw/core/metric_sink.h
   include/vw/core/model_utils.h
   include/vw/core/multi_model_utils.h
   include/vw/core/multiclass.h
   include/vw/core/multilabel.h
   include/vw/core/named_labels.h
-  include/vw/core/network.h
   include/vw/core/no_label.h
   include/vw/core/numeric_casts.h
   include/vw/core/object_pool.h
   include/vw/core/parse_args.h
   include/vw/core/parse_dispatch_loop.h
   include/vw/core/parse_example_json.h
   include/vw/core/parse_example.h
@@ -81,15 +79,14 @@
   include/vw/core/print_utils.h
   include/vw/core/prob_dist_cont.h
   include/vw/core/queue.h
   include/vw/core/rand_state.h
   include/vw/core/reduction_features.h
   include/vw/core/reduction_stack.h
   include/vw/core/reductions/active_cover.h
-  include/vw/core/reductions/active.h
   include/vw/core/reductions/audit_regressor.h
   include/vw/core/reductions/autolink.h
   include/vw/core/reductions/automl.h
   include/vw/core/reductions/baseline_challenger_cb.h
   include/vw/core/reductions/baseline.h
   include/vw/core/reductions/bfgs.h
   include/vw/core/reductions/binary.h
@@ -156,23 +153,14 @@
   include/vw/core/reductions/oja_newton.h
   include/vw/core/reductions/plt.h
   include/vw/core/reductions/pmf_to_pdf.h
   include/vw/core/reductions/print.h
   include/vw/core/reductions/recall_tree.h
   include/vw/core/reductions/sample_pdf.h
   include/vw/core/reductions/scorer.h
-  include/vw/core/reductions/search/search_dep_parser.h
-  include/vw/core/reductions/search/search_entityrelationtask.h
-  include/vw/core/reductions/search/search_graph.h
-  include/vw/core/reductions/search/search_hooktask.h
-  include/vw/core/reductions/search/search_meta.h
-  include/vw/core/reductions/search/search_multiclasstask.h
-  include/vw/core/reductions/search/search_sequencetask.h
-  include/vw/core/reductions/search/search.h
-  include/vw/core/reductions/sender.h
   include/vw/core/reductions/shared_feature_merger.h
   include/vw/core/reductions/slates.h
   include/vw/core/reductions/stagewise_poly.h
   include/vw/core/reductions/svrg.h
   include/vw/core/reductions/topk.h
   include/vw/core/scope_exit.h
   include/vw/core/shared_data.h
@@ -231,29 +219,27 @@
   src/loss_functions.cc
   src/merge.cc
   src/metrics_collector.cc
   src/metric_sink.cc
   src/multiclass.cc
   src/multilabel.cc
   src/named_labels.cc
-  src/network.cc
   src/no_label.cc
   src/parse_args.cc
   src/parse_example_json.cc
   src/parse_primitives.cc
   src/parse_regressor.cc
   src/parse_slates_example_json.cc
   src/parser.cc
   src/prediction_type.cc
   src/print_utils.cc
   src/prob_dist_cont.cc
   src/qr_decomposition.cc
   src/reduction_stack.cc
   src/reductions/active_cover.cc
-  src/reductions/active.cc
   src/reductions/audit_regressor.cc
   src/reductions/autolink.cc
   src/reductions/automl.cc
   src/reductions/baseline_challenger_cb.cc
   src/reductions/baseline.cc
   src/reductions/bfgs.cc
   src/reductions/binary.cc
@@ -297,15 +283,14 @@
   src/reductions/csoaa.cc
   src/reductions/details/automl/automl_impl.cc
   src/reductions/details/automl/automl_iomodel.cc
   src/reductions/details/automl/automl_oracle.cc
   src/reductions/details/automl/automl_util.cc
   src/reductions/ect.cc
   src/reductions/eigen_memory_tree.cc
-  src/daemon_utils.cc
   src/reductions/epsilon_decay.cc
   src/reductions/explore_eval.cc
   src/reductions/freegrad.cc
   src/reductions/ftrl.cc
   src/reductions/gd_mf.cc
   src/reductions/gd.cc
   src/reductions/generate_interactions.cc
@@ -329,23 +314,14 @@
   src/reductions/oja_newton.cc
   src/reductions/plt.cc
   src/reductions/pmf_to_pdf.cc
   src/reductions/print.cc
   src/reductions/recall_tree.cc
   src/reductions/sample_pdf.cc
   src/reductions/scorer.cc
-  src/reductions/search/search_dep_parser.cc
-  src/reductions/search/search_entityrelationtask.cc
-  src/reductions/search/search_graph.cc
-  src/reductions/search/search_hooktask.cc
-  src/reductions/search/search_meta.cc
-  src/reductions/search/search_multiclasstask.cc
-  src/reductions/search/search_sequencetask.cc
-  src/reductions/search/search.cc
-  src/reductions/sender.cc
   src/reductions/shared_feature_merger.cc
   src/reductions/slates.cc
   src/reductions/stagewise_poly.cc
   src/reductions/svrg.cc
   src/reductions/topk.cc
   src/shared_data.cc
   src/simple_label_parser.cc
@@ -360,19 +336,58 @@
 )
 
 if(VW_FEAT_LDA)
   list(APPEND vw_core_headers include/vw/core/reductions/lda_core.h)
   list(APPEND vw_core_sources src/reductions/lda_core.cc)
 endif()
 
+if(VW_FEAT_SEARCH)
+list(APPEND vw_core_headers
+  include/vw/core/reductions/search/search_dep_parser.h
+  include/vw/core/reductions/search/search_entityrelationtask.h
+  include/vw/core/reductions/search/search_graph.h
+  include/vw/core/reductions/search/search_hooktask.h
+  include/vw/core/reductions/search/search_meta.h
+  include/vw/core/reductions/search/search_multiclasstask.h
+  include/vw/core/reductions/search/search_sequencetask.h
+  include/vw/core/reductions/search/search.h
+)
+list(APPEND vw_core_sources
+  src/reductions/search/search_dep_parser.cc
+  src/reductions/search/search_entityrelationtask.cc
+  src/reductions/search/search_graph.cc
+  src/reductions/search/search_hooktask.cc
+  src/reductions/search/search_meta.cc
+  src/reductions/search/search_multiclasstask.cc
+  src/reductions/search/search_sequencetask.cc
+  src/reductions/search/search.cc
+)
+endif()
+
 if(VW_FEAT_CB_GRAPH_FEEDBACK)
   list(APPEND vw_core_headers include/vw/core/reductions/cb/cb_explore_adf_graph_feedback.h)
   list(APPEND vw_core_sources src/reductions/cb/cb_explore_adf_graph_feedback.cc)
 endif()
 
+if(VW_FEAT_NETWORKING)
+  list(APPEND vw_core_headers
+    include/vw/core/daemon_utils.h
+    include/vw/core/reductions/sender.h
+    include/vw/core/network.h
+    include/vw/core/reductions/active.h
+  )
+
+  list(APPEND vw_core_sources
+    src/daemon_utils.cc
+    src/reductions/sender.cc
+    src/network.cc
+    src/reductions/active.cc
+  )
+endif()
+
 vw_add_library(
     NAME "core"
     TYPE "STATIC_ONLY"
     SOURCES ${vw_core_headers} ${vw_core_sources}
     PUBLIC_DEPS vw_common vw_explore vw_allreduce vw_config fmt::fmt vw_cache_parser vw_text_parser vw_json_parser
     PRIVATE_DEPS
         # Special case for dealing with header-only INTERFACE dependencies of a STATIC library
@@ -391,18 +406,17 @@
 
 if(VW_FEAT_CB_GRAPH_FEEDBACK)
   target_link_libraries(vw_core PRIVATE $<BUILD_INTERFACE:mlpack_ensmallen>)
 endif()
 
 target_include_directories(vw_core PRIVATE ${CMAKE_CURRENT_LIST_DIR}/src)
 
-if (VW_BUILD_LAS_WITH_SIMD AND (UNIX AND NOT APPLE) AND (${CMAKE_SYSTEM_PROCESSOR} STREQUAL "x86_64"))
+if (VW_FEAT_LAS_SIMD)
   set_source_files_properties(src/reductions/cb/details/large_action/compute_dot_prod_avx2.cc PROPERTIES COMPILE_FLAGS "-mfma -mavx2")
   set_source_files_properties(src/reductions/cb/details/large_action/compute_dot_prod_avx512.cc PROPERTIES COMPILE_FLAGS "-mavx512f -mavx512bw -mavx512vl -mavx512vpopcntdq")
-  target_compile_definitions(vw_core PUBLIC BUILD_LAS_WITH_SIMD)
 endif()
 
 if(VW_FEAT_CSV)
   target_link_libraries(vw_core PRIVATE vw_csv_parser)
 endif()
 
 if(VW_FEAT_FLATBUFFERS)
@@ -440,15 +454,15 @@
       tests/automl_test.cc
       tests/automl_weights_test.cc
       tests/baseline_cb_test.cc
       tests/cats_test.cc
       tests/cats_tree_test.cc
       tests/cats_user_provided_pdf.cc
       tests/cb_explore_adf_test.cc
-      tests/cb_graph_feedback_label_text_parse_test.cc
+      tests/cb_graph_feedback_label_parse_test.cc
       tests/cb_large_actions_test.cc
       tests/cb_las_one_pass_svd_test.cc
       tests/cb_las_spanner_test.cc
       tests/cb_with_observations_parser_test.cc
       tests/ccb_parser_test.cc
       tests/ccb_test.cc
       tests/chain_hashing.cc
```

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/gdb_pretty_printers.py` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/gdb_pretty_printers.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/accumulate.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/accumulate.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/action_score.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/action_score.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/active_multiclass_prediction.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/active_multiclass_prediction.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/api_status.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/api_status.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/array_parameters.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/array_parameters.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/array_parameters_dense.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/array_parameters_dense.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/array_parameters_sparse.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/array_parameters_sparse.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/automl_impl.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/automl_impl.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/best_constant.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/best_constant.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/cache.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/cache.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/cached_learner.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/cached_learner.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/cb.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/cb.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/cb_continuous_label.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/cb_continuous_label.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/cb_graph_feedback_reduction_features.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/cb_graph_feedback_reduction_features.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/cb_with_observations_label.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/cb_with_observations_label.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/ccb_label.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/ccb_label.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/ccb_reduction_features.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/ccb_reduction_features.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/constant.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/constant.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/continuous_actions_reduction_features.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/continuous_actions_reduction_features.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/correctedMath.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/correctedMath.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/cost_sensitive.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/cost_sensitive.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/crossplat_compat.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/crossplat_compat.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/daemon_utils.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/daemon_utils.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/debug_log.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/debug_log.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/debug_print.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/debug_print.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/decision_scores.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/decision_scores.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/epsilon_reduction_features.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/epsilon_reduction_features.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/error_constants.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/error_constants.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/error_data.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/error_data.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/error_reporting.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/error_reporting.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/estimators/confidence_sequence.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/estimators/confidence_sequence.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/estimators/confidence_sequence_robust.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/estimators/confidence_sequence_robust.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/estimators/cressieread.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/estimators/cressieread.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/estimators/distributionally_robust.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/estimators/distributionally_robust.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/example.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/example.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/example_predict.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/example_predict.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/fast_pow10.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/fast_pow10.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/feature_group.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/feature_group.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/gd_predict.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/gd_predict.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/gen_cs_example.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/gen_cs_example.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/generic_range.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/generic_range.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/global_data.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/global_data.h`

 * *Files 0% similar despite different names*

```diff
@@ -213,15 +213,17 @@
   bool invariant_updates;  // Should we use importance aware/safe updates, gd only
   uint32_t total_feature_width;
 };
 
 class runtime_config
 {
 public:
+#ifdef VW_FEAT_NETWORKING_ENABLED
   bool daemon;
+#endif
   bool vw_is_main = false;  // true if vw is executable; false in library mode
   bool training;            // Should I train if lable data is available?
   size_t pass_length;
   size_t numpasses;
   bool default_bits;
   all_reduce_type selected_all_reduce_type;
   uint32_t hash_seed;
```

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/guard.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/guard.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/hashstring.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/hashstring.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/input_parser.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/input_parser.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/interaction_generation_state.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/interaction_generation_state.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/interactions.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/interactions.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/interactions_predict.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/interactions_predict.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/io_buf.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/io_buf.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/kskip_ngram_transformer.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/kskip_ngram_transformer.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/label_dictionary.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/label_dictionary.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/label_parser.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/label_parser.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/label_type.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/label_type.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/large_action_space_reduction_features.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/large_action_space_reduction_features.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/learner.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/learner.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/loss_functions.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/loss_functions.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/memory.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/memory.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/merge.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/merge.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/metric_sink.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/metric_sink.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/metrics_collector.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/metrics_collector.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/model_utils.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/model_utils.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/multi_model_utils.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/multi_model_utils.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/multiclass.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/multiclass.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/multilabel.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/multilabel.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/named_labels.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/named_labels.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/network.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/network.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/no_label.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/no_label.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/numeric_casts.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/numeric_casts.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/object_pool.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/object_pool.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/parse_args.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/parse_args.h`

 * *Files 8% similar despite different names*

```diff
@@ -14,23 +14,25 @@
 {
 namespace details
 {
 // Used in parse_source
 class input_options
 {
 public:
+#ifdef VW_FEAT_NETWORKING_ENABLED
   bool daemon;
   bool foreground;
   uint32_t port;
   std::string pid_file;
   std::string port_file;
   uint64_t num_children;
   // If a model was saved in daemon or active learning mode, force it to accept
   // local input when loaded instead.
   bool no_daemon = false;
+#endif
 
   bool cache;
   std::vector<std::string> cache_files;
   bool json;
   bool dsjson;
   bool kill_cache;
   bool compressed;
```

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/parse_dispatch_loop.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/parse_dispatch_loop.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/parse_example.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/parse_example.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/parse_example_json.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/parse_example_json.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/parse_primitives.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/parse_primitives.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/parse_regressor.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/parse_regressor.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/parse_slates_example_json.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/parse_slates_example_json.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/parser.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/parser.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/polymorphic_ex.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/polymorphic_ex.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/prediction_type.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/prediction_type.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/prob_dist_cont.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/prob_dist_cont.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/queue.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/queue.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reduction_features.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reduction_features.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reduction_stack.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reduction_stack.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/active.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/active.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/baseline.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/baseline.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/bs.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/bs.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cats.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cats.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cats_tree.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cats_tree.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cb/cb_actions_mask.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cb/cb_actions_mask.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cb/cb_adf.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cb/cb_adf.h`

 * *Files 10% similar despite different names*

```diff
@@ -9,34 +9,35 @@
 #include "vw/core/vw_versions.h"
 
 #include <memory>
 #include <vector>
 
 namespace VW
 {
-VW::example* test_cb_adf_sequence(const VW::multi_ex& ec_seq);
+VW::example* test_cb_adf_sequence(const VW::multi_ex& ec_seq, bool allow_multiple_costs = false);
 VW::cb_class get_observed_cost_or_default_cb_adf(const VW::multi_ex& examples);
 namespace reductions
 {
 std::shared_ptr<VW::LEARNER::learner> cb_adf_setup(VW::setup_base_i& stack_builder);
 
 class cb_adf
 {
 public:
   void learn(VW::LEARNER::learner& base, VW::multi_ex& ec_seq);
   void predict(VW::LEARNER::learner& base, VW::multi_ex& ec_seq);
   bool update_statistics(const VW::example& ec, const VW::multi_ex& ec_seq, VW::shared_data& sd) const;
 
   cb_adf(VW::cb_type_t cb_type, bool rank_all, float clip_p, bool no_predict, size_t feature_width_above,
-      VW::workspace* all)
+      bool per_model_save_load, VW::workspace* all)
       : _no_predict(no_predict)
       , _rank_all(rank_all)
       , _clip_p(clip_p)
       , _gen_cs_mtr(feature_width_above)
       , _cb_type(cb_type)
+      , _per_model_save_load(per_model_save_load)
       , _all(all)
   {
   }
 
   void set_scorer(VW::LEARNER::learner* scorer) { _gen_cs_dr.scorer = scorer; }
 
   bool get_rank_all() const { return _rank_all; }
@@ -53,14 +54,15 @@
   {
     return ((_cb_type == VW::cb_type_t::MTR) && !_no_predict) || _cb_type == VW::cb_type_t::IPS ||
         _cb_type == VW::cb_type_t::DR || _cb_type == VW::cb_type_t::DM || _cb_type == VW::cb_type_t::SM;
   }
 
   VW::cb_class* known_cost() { return &_gen_cs_dr.known_cost; }
   const VW::cb_class* known_cost() const { return &_gen_cs_dr.known_cost; }
+  bool per_model_save_load() const { return _per_model_save_load; }
 
 private:
   void learn_ips(VW::LEARNER::learner& base, VW::multi_ex& examples);
   void learn_dr(VW::LEARNER::learner& base, VW::multi_ex& examples);
   void learn_dm(VW::LEARNER::learner& base, VW::multi_ex& examples);
   void learn_sm(VW::LEARNER::learner& base, VW::multi_ex& examples);
   template <bool predict>
@@ -80,14 +82,15 @@
   uint64_t _offset_index = 0;
   const bool _no_predict;
   const bool _rank_all;
   const float _clip_p;
   VW::details::cb_to_cs_adf_dr _gen_cs_dr;
   VW::details::cb_to_cs_adf_mtr _gen_cs_mtr;
   VW::cb_type_t _cb_type;
+  bool _per_model_save_load;
 
   VW::workspace* _all = nullptr;
 };
 }  // namespace reductions
 }  // namespace VW
 
 namespace CB_ADF  // NOLINT
```

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cb/cb_algs.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cb/cb_algs.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cb/cb_explore_adf_common.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cb/cb_explore_adf_common.h`

 * *Files 3% similar despite different names*

```diff
@@ -83,15 +83,16 @@
 // Object
 template <typename ExploreType>
 // data common to all cb_explore_adf reductions
 class cb_explore_adf_base
 {
 public:
   template <typename... Args>
-  cb_explore_adf_base(bool with_metrics, Args&&... args) : explore(std::forward<Args>(args)...)
+  cb_explore_adf_base(bool with_metrics, Args&&... args)
+      : explore(std::forward<Args>(args)...), _allow_multiple_costs(false)
   {
     if (with_metrics) { _metrics = VW::make_unique<cb_explore_metrics>(); }
   }
 
   static void save_load(cb_explore_adf_base<ExploreType>& data, io_buf& io, bool read, bool text);
   static void persist_metrics(cb_explore_adf_base<ExploreType>& data, metric_sink& metrics);
   static void predict(cb_explore_adf_base<ExploreType>& data, VW::LEARNER::learner& base, multi_ex& examples);
@@ -100,17 +101,20 @@
   static void update_stats(const VW::workspace& all, VW::shared_data& sd, const cb_explore_adf_base<ExploreType>& data,
       const multi_ex& ec_seq, VW::io::logger& logger);
   static void output_example_prediction(
       VW::workspace& all, const cb_explore_adf_base<ExploreType>& data, const multi_ex& ec_seq, VW::io::logger& logger);
   static void print_update(VW::workspace& all, VW::shared_data& sd, const cb_explore_adf_base<ExploreType>& data,
       const multi_ex& ec_seq, VW::io::logger& logger);
 
+  void set_allow_multiple_costs(bool allow_multiple_costs) { _allow_multiple_costs = allow_multiple_costs; }
+
   ExploreType explore;
 
 private:
+  bool _allow_multiple_costs;
   VW::cb_class _known_cost;
   // used in output_example
   VW::cb_label _action_label;
   VW::cb_label _empty_label;
   VW::action_scores _saved_pred;
   std::unique_ptr<cb_explore_metrics> _metrics;
 
@@ -120,15 +124,15 @@
   void _print_update(VW::workspace& all, VW::shared_data& sd, const multi_ex& ec_seq, VW::io::logger& logger) const;
 };
 
 template <typename ExploreType>
 inline void cb_explore_adf_base<ExploreType>::predict(
     cb_explore_adf_base<ExploreType>& data, VW::LEARNER::learner& base, multi_ex& examples)
 {
-  example* label_example = VW::test_cb_adf_sequence(examples);
+  example* label_example = VW::test_cb_adf_sequence(examples, data._allow_multiple_costs);
   data._known_cost = VW::get_observed_cost_or_default_cb_adf(examples);
 
   if (label_example != nullptr)
   {
     // predict path, replace the label example with an empty one
     data._action_label = std::move(label_example->l.cb);
     label_example->l.cb = std::move(data._empty_label);
@@ -145,15 +149,15 @@
   }
 }
 
 template <typename ExploreType>
 inline void cb_explore_adf_base<ExploreType>::learn(
     cb_explore_adf_base<ExploreType>& data, VW::LEARNER::learner& base, multi_ex& examples)
 {
-  example* label_example = VW::test_cb_adf_sequence(examples);
+  example* label_example = VW::test_cb_adf_sequence(examples, data._allow_multiple_costs);
   if (label_example != nullptr)
   {
     data._known_cost = VW::get_observed_cost_or_default_cb_adf(examples);
     // learn iff label_example != nullptr
     data.explore.learn(base, examples);
     if (data._metrics)
     {
```

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cb/cbify.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cb/cbify.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/conditional_contextual_bandit.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/conditional_contextual_bandit.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/eigen_memory_tree.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/eigen_memory_tree.h`

 * *Files 9% similar despite different names*

```diff
@@ -37,21 +37,30 @@
 
 enum class emt_router_type : uint32_t
 {
   RANDOM = 1,
   EIGEN = 2
 };
 
+enum class emt_initial_type : uint32_t
+{
+  EUCLIDEAN = 1,
+  GAUSSIAN = 2,
+  COSINE = 3,
+  NONE = 4
+};
+
 emt_scorer_type emt_scorer_type_from_string(VW::string_view val);
 emt_router_type emt_router_type_from_string(VW::string_view val);
+emt_initial_type emt_initial_type_from_string(VW::string_view val);
 
+float emt_initial(emt_initial_type initial_type, emt_feats f1, emt_feats f2);
 float emt_median(std::vector<float>&);
 float emt_inner(const emt_feats&, const emt_feats&);
 float emt_norm(const emt_feats&);
-void emt_abs(emt_feats&);
 void emt_scale(emt_feats&, float);
 void emt_normalize(emt_feats&);
 emt_feats emt_scale_add(float, const emt_feats&, float, const emt_feats&);
 emt_feats emt_router_eigen(std::vector<emt_feats>&, VW::rand_state&);
 
 template <typename RandomIt>
 void emt_shuffle(RandomIt first, RandomIt last, VW::rand_state& rng)
@@ -108,28 +117,29 @@
   VW::workspace* all = nullptr;
   std::shared_ptr<VW::rand_state> random_state;
 
   // how many memories before splitting a leaf node
   uint32_t leaf_split = 100;
   emt_scorer_type scorer_type = emt_scorer_type::SELF_CONSISTENT_RANK;
   emt_router_type router_type = emt_router_type::EIGEN;
+  emt_initial_type initial_type = emt_initial_type::COSINE;
 
   std::unique_ptr<VW::example> ex;  // we create one of these which we re-use so we don't have to reallocate examples
   std::unique_ptr<std::vector<std::vector<VW::namespace_index>>> empty_interactions_for_ex;
   std::unique_ptr<std::vector<std::vector<extent_term>>> empty_extent_interactions_for_ex;
 
 #ifdef VW_ENABLE_EMT_DEBUG_TIMER
   int64_t begin = 0;  // for timing performance
 #endif
 
   std::unique_ptr<emt_node> root;
   std::unique_ptr<emt_lru> bounder = nullptr;
 
   emt_tree(VW::workspace* all, std::shared_ptr<VW::rand_state> random_state, uint32_t leaf_split,
-      emt_scorer_type scorer_type, emt_router_type router_type, uint64_t tree_bound);
+      emt_scorer_type scorer_type, emt_router_type router_type, emt_initial_type initial_type, uint64_t tree_bound);
 };
 
 }  // namespace eigen_memory_tree
 }  // namespace reductions
 
 namespace model_utils
 {
```

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/epsilon_decay.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/epsilon_decay.h`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,16 @@
 
 class epsilon_decay_data
 {
 public:
   epsilon_decay_data(uint64_t model_count, uint64_t min_scope, double epsilon_decay_significance_level,
       double epsilon_decay_estimator_decay, dense_parameters& weights, std::string epsilon_decay_audit_str,
       bool constant_epsilon, uint32_t& feature_width, uint64_t _min_champ_examples, float initial_epsilon,
-      uint64_t shift_model_bounds, bool reward_as_cost, double tol_x, bool is_brentq, bool predict_only_model);
+      uint64_t shift_model_bounds, bool reward_as_cost, double tol_x, bool is_brentq, bool predict_only_model,
+      bool challenger_epsilon);
   void update_weights(float init_ep, VW::LEARNER::learner& base, VW::multi_ex& examples);
   void promote_model(int64_t model_ind, int64_t swap_dist);
   void rebalance_greater_models(int64_t model_ind, int64_t swap_dist, int64_t model_count);
   void clear_weights_and_estimators(int64_t swap_dist, int64_t model_count);
   void shift_model(int64_t model_ind, int64_t swap_dist, int64_t model_count);
   void check_estimator_bounds();
   void check_horizon_bounds();
@@ -51,14 +52,15 @@
   bool _constant_epsilon;
   uint32_t& _feature_width;
   uint64_t _min_champ_examples;
   float _initial_epsilon;
   uint64_t _shift_model_bounds;
   bool _reward_as_cost;
   bool _predict_only_model;
+  bool _challenger_epsilon;
 };
 
 }  // namespace epsilon_decay
 }  // namespace reductions
 
 namespace model_utils
 {
```

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/expreplay.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/expreplay.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/freegrad.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/freegrad.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/ftrl.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/ftrl.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/gd.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/gd.h`

 * *Files 0% similar despite different names*

```diff
@@ -51,14 +51,15 @@
   void (*learn)(gd&, VW::example&) = nullptr;
   void (*update)(gd&, VW::example&) = nullptr;
   float (*sensitivity)(gd&, VW::example&) = nullptr;
   void (*multipredict)(gd&, VW::example&, size_t, size_t, VW::polyprediction*, bool) = nullptr;
   bool adaptive_input = false;
   bool normalized_input = false;
   bool adax = false;
+  bool per_model_save_load = false;
   VW::workspace* all = nullptr;  // parallel, features, parameters
 };
 }  // namespace reductions
 
 namespace details
 {
```

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/interaction_ground.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/interaction_ground.h`

 * *Files 27% similar despite different names*

```diff
@@ -17,30 +17,39 @@
  * https://github.com/VowpalWabbit/vowpal_wabbit/wiki/Interaction-Grounded-Learning
  *
  * @param stack_builder Stack builder to use for setup.
  * @return VW::LEARNER::learner* learner if this reduction is active, nullptr otherwise
  */
 std::shared_ptr<VW::LEARNER::learner> interaction_ground_setup(VW::setup_base_i& stack_builder);
 
-class interaction_ground_data
+namespace igl
+{
+class igl_data
 {
 public:
+  igl_data(bool predict_only_model);
+
   std::shared_ptr<VW::LEARNER::learner> ik_learner = nullptr;
   VW::example ik_ex;
 
   VW::cb_class known_cost;  // for update stats
 
   std::vector<std::vector<VW::namespace_index>> interactions;
   std::vector<std::vector<VW::extent_term>>* extent_interactions;
 
   std::unique_ptr<VW::workspace> ik_all;
   ftrl* ik_ftrl;  // automatically save resume
   std::unique_ptr<ftrl> pi_ftrl;
+
+  bool _predict_only_model;
+  size_t _cb_model_offset = 1;
+  size_t _feature_width = 2;
 };
+}  // namespace igl
 }  // namespace reductions
 
 namespace model_utils
 {
-size_t write_model_field(io_buf&, const VW::reductions::interaction_ground_data&, const std::string&, bool);
-size_t read_model_field(io_buf&, VW::reductions::interaction_ground_data&);
+size_t write_model_field(io_buf&, const VW::reductions::igl::igl_data&, const std::string&, bool);
+size_t read_model_field(io_buf&, VW::reductions::igl::igl_data&);
 }  // namespace model_utils
 }  // namespace VW
```

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/lda_core.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/lda_core.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/mwt.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/mwt.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/offset_tree.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/offset_tree.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/pmf_to_pdf.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/pmf_to_pdf.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/search/search.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/search/search.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 // Copyright (c) by respective owners including Yahoo!, Microsoft, and
 // individual contributors. All rights reserved. Released under a BSD (revised)
 // license as described in the file LICENSE.
 #pragma once
-#include "vw/core/example.h"
-#include "vw/core/global_data.h"
+
+#ifdef VW_FEAT_SEARCH_ENABLED
+
+#  include "vw/core/example.h"
+#  include "vw/core/global_data.h"
 
 // TODO: Search is using some macro-enabled logging logic for cdbg
 //       (going to clog [which in turn goes to err, with some differences])
 //       We may want to create/use some macro-based loggers (which will wrap the spdlog ones)
 //       to mimic this behavior.
 #define cdbg std::clog
 #undef cdbg
@@ -370,7 +373,8 @@
 namespace VW
 {
 namespace reductions
 {
 std::shared_ptr<VW::LEARNER::learner> search_setup(VW::setup_base_i& stack_builder);
 }
 }  // namespace VW
+#endif
```

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/search/search_hooktask.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/search/search_hooktask.h`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 // Copyright (c) by respective owners including Yahoo!, Microsoft, and
 // individual contributors. All rights reserved. Released under a BSD (revised)
 // license as described in the file LICENSE.
 #pragma once
-#include "search.h"
+#ifdef VW_FEAT_SEARCH_ENABLED
+#  include "search.h"
 
 namespace HookTask
 {
 void initialize(Search::search&, size_t&, VW::config::options_i&);
 void run(Search::search&, VW::multi_ex&);
 void run_setup(Search::search&, VW::multi_ex&);
 void run_takedown(Search::search&, VW::multi_ex&);
@@ -24,7 +25,9 @@
                                        // have to know about hook
   std::shared_ptr<void> takedown_object;  // for python this will really be a (py::object*), but we don't want basic VW
                                           // to have to know about hook
   VW::config::options_i* arg = nullptr;   // so that hook can access command line variables
   size_t num_actions = 0;                 // cache for easy access
 };
 }  // namespace HookTask
+
+#endif
```

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/search/search_meta.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/search/search_meta.h`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 // Copyright (c) by respective owners including Yahoo!, Microsoft, and
 // individual contributors. All rights reserved. Released under a BSD (revised)
 // license as described in the file LICENSE.
 #pragma once
-#include "search.h"
 
-#define DECLARE_METATASK(X)                \
-  namespace X                              \
-  {                                        \
-  extern Search::search_metatask metatask; \
-  }
+#ifdef VW_FEAT_SEARCH_ENABLED
+#  include "search.h"
+
+#  define DECLARE_METATASK(X)                \
+    namespace X                              \
+    {                                        \
+    extern Search::search_metatask metatask; \
+    }
 
 DECLARE_METATASK(DebugMT)
 DECLARE_METATASK(SelectiveBranchingMT)
 
 // namespace DebugMT              { extern Search::search_metatask metatask; }
 // namespace SelectiveBranchingMT { extern Search::search_metatask metatask; }
+#endif
```

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/search/search_sequencetask.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/search/search_sequencetask.h`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 // Copyright (c) by respective owners including Yahoo!, Microsoft, and
 // individual contributors. All rights reserved. Released under a BSD (revised)
 // license as described in the file LICENSE.
 #pragma once
-#include "search.h"
+#ifdef VW_FEAT_SEARCH_ENABLED
+#  include "search.h"
 
 namespace SequenceTask
 {
 void initialize(Search::search&, size_t&, VW::config::options_i&);
 void run(Search::search&, VW::multi_ex&);
 extern Search::search_task task;
 }  // namespace SequenceTask
@@ -39,7 +40,8 @@
 namespace SequenceTask_DemoLDF
 {
 void initialize(Search::search&, size_t&, VW::config::options_i&);
 void finish(Search::search&);
 void run(Search::search&, VW::multi_ex&);
 extern Search::search_task task;
 }  // namespace SequenceTask_DemoLDF
+#endif
```

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/slates.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/slates.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/scope_exit.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/scope_exit.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/setup_base.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/setup_base.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/shared_data.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/shared_data.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/simple_label.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/simple_label.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/simple_label_parser.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/simple_label_parser.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/slates_label.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/slates_label.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/table_formatter.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/table_formatter.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/text_utils.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/text_utils.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/thread_pool.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/thread_pool.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/unique_sort.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/unique_sort.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/v_array.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/v_array.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/version.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/version.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/vw.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/vw.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/vw_allreduce.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/vw_allreduce.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/vw_fwd.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/vw_fwd.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/vw_math.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/vw_math.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/vw_string_view_fmt.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/vw_string_view_fmt.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/vw_versions.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/vw_versions.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/accumulate.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/accumulate.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/action_score.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/action_score.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/api_status.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/api_status.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/array_parameters_dense.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/array_parameters_dense.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/array_parameters_sparse.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/array_parameters_sparse.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/best_constant.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/best_constant.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/cb.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/cb.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/cb_continuous_label.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/cb_continuous_label.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/cb_type.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/cb_type.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/cb_with_observations_label.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/cb_with_observations_label.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/ccb_label.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/ccb_label.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/ccb_reduction_features.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/ccb_reduction_features.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/confidence_sequence.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/confidence_sequence.cc`

 * *Files 1% similar despite different names*

```diff
@@ -200,15 +200,15 @@
         1.0 + b * (-7.709336904239235 + b * (80.59885744577618 + b * (114.25915616534267 + b * (232.30352278139097))));
     return numerator / denominator;
   }
 }
 
 double confidence_sequence::lblogwealth(double sumXt, double v, double eta, double s, double lb_alpha) const
 {
-#if !defined(__APPLE__) && !defined(_WIN32)
+#if !defined(__APPLE__) && !defined(_WIN32) && !defined(__EMSCRIPTEN__)
   double zeta_s = std::riemann_zeta(s);
 #else
   double zeta_s = 10.584448464950803;  // std::riemann_zeta(s) -- Assuming s=1.1 is constant
 #endif
   v = std::max(v, 1.0);
   double gamma1 = (std::pow(eta, 0.25) + std::pow(eta, 0.25)) / std::sqrt(2.0);
   double gamma2 = (std::sqrt(eta) + 1.0) / 2.0;
```

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/confidence_sequence_robust.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/confidence_sequence_robust.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/cost_sensitive.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/cost_sensitive.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/cressieread.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/cressieread.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/crossplat_compat.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/crossplat_compat.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/daemon_utils.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/daemon_utils.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/debug_print.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/debug_print.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/decision_scores.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/decision_scores.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/distributionally_robust.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/distributionally_robust.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/example.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/example.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/example_predict.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/example_predict.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/feature_group.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/feature_group.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/gen_cs_example.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/gen_cs_example.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/global_data.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/global_data.cc`

 * *Files 1% similar despite different names*

```diff
@@ -321,15 +321,17 @@
   passes_config.current_pass = 0;
 
   reduction_state.bfgs = false;
   loss_config.no_bias = false;
   reduction_state.active = false;
   initial_weights_config.num_bits = 18;
   runtime_config.default_bits = true;
+#ifdef VW_FEAT_NETWORKING_ENABLED
   runtime_config.daemon = false;
+#endif
   output_model_config.save_resume = true;
   output_model_config.preserve_performance_counters = false;
 
   initial_weights_config.random_positive_weights = false;
 
   weights.sparse = false;
```

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/hashstring.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/hashstring.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/interactions.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/interactions.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/io_buf.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/io_buf.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/kskip_ngram_transformer.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/kskip_ngram_transformer.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/label_dictionary.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/label_dictionary.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/label_parser.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/label_parser.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/label_type.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/label_type.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/learner.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/learner.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/loss_functions.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/loss_functions.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/merge.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/merge.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/metric_sink.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/metric_sink.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/metrics_collector.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/metrics_collector.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/multiclass.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/multiclass.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/multilabel.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/multilabel.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/named_labels.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/named_labels.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/network.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/network.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/no_label.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/no_label.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/parse_args.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/parse_args.cc`

 * *Files 1% similar despite different names*

```diff
@@ -373,40 +373,45 @@
 }
 
 VW::details::input_options parse_source(VW::workspace& all, options_i& options)
 {
   VW::details::input_options parsed_options;
 
   option_group_definition input_options("Input");
-  input_options.add(make_option("data", all.parser_runtime.data_filename).short_name("d").help("Example set"))
+  input_options
+      .add(make_option("data", all.parser_runtime.data_filename).short_name("d").help("Example set"))
+#ifdef VW_FEAT_NETWORKING_ENABLED
       .add(make_option("daemon", parsed_options.daemon).help("Persistent daemon mode on port 26542"))
       .add(make_option("foreground", parsed_options.foreground)
                .help("In persistent daemon mode, do not run in the background"))
       .add(make_option("port", parsed_options.port).help("Port to listen on; use 0 to pick unused port"))
       .add(make_option("num_children", parsed_options.num_children)
                .default_value(10)
                .help("Number of children for persistent daemon mode"))
       .add(make_option("pid_file", parsed_options.pid_file).help("Write pid file in persistent daemon mode"))
       .add(make_option("port_file", parsed_options.port_file).help("Write port used in persistent daemon mode"))
+#endif
       .add(make_option("cache", parsed_options.cache).short_name("c").help("Use a cache.  The default is <data>.cache"))
       .add(make_option("cache_file", parsed_options.cache_files).help("The location(s) of cache_file"))
       .add(make_option("json", parsed_options.json).help("Enable JSON parsing"))
       .add(make_option("dsjson", parsed_options.dsjson).help("Enable Decision Service JSON parsing"))
       .add(make_option("kill_cache", parsed_options.kill_cache)
                .short_name("k")
                .help("Do not reuse existing cache: create a new one always"))
       .add(
           make_option("compressed", parsed_options.compressed)
               .help(
                   "use gzip format whenever possible. If a cache file is being created, this option creates a "
                   "compressed cache file. A mixture of raw-text & compressed inputs are supported with autodetection."))
       .add(make_option("no_stdin", parsed_options.stdin_off).help("Do not default to reading from stdin"))
+#ifdef VW_FEAT_NETWORKING_ENABLED
       .add(make_option("no_daemon", parsed_options.no_daemon)
                .help("Force a loaded daemon or active learning model to accept local input instead of starting in "
                      "daemon mode"))
+#endif
       .add(make_option("chain_hash", parsed_options.chain_hash_json)
                .keep()
                .help("Enable chain hash in JSON for feature name and string feature value. e.g. {'A': {'B': 'C'}} is "
                      "hashed as A^B^C."))
       .add(make_option("flatbuffer", parsed_options.flatbuffer)
                .help("Data file will be interpreted as a flatbuffer file")
                .experimental());
@@ -431,21 +436,23 @@
     {
       all.logger.err_warn(
           "Multiple data files passed as positional parameters, only the first one will be "
           "read and the rest will be ignored.");
     }
   }
 
+#ifdef VW_FEAT_NETWORKING_ENABLED
   if (parsed_options.daemon || options.was_supplied("pid_file") ||
       (options.was_supplied("port") && !all.reduction_state.active))
   {
     all.runtime_config.daemon = true;
     // allow each child to process up to 1e5 connections
     all.runtime_config.numpasses = static_cast<size_t>(1e5);
   }
+#endif
 
   // Add an implicit cache file based on the data filename.
   if (parsed_options.cache) { parsed_options.cache_files.push_back(all.parser_runtime.data_filename + ".cache"); }
 
   if ((parsed_options.cache || options.was_supplied("cache_file")) && options.was_supplied("invert_hash"))
     THROW("invert_hash is incompatible with a cache file.  Use it in single pass mode only.")
```

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/parse_example_json.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/parse_example_json.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/parse_primitives.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/parse_primitives.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/parse_regressor.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/parse_regressor.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/parse_slates_example_json.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/parse_slates_example_json.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/parser.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/parser.cc`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,17 @@
 #  include <WinSock2.h>
 #  include <Windows.h>
 #  include <io.h>
 typedef int socklen_t;
 // windows doesn't define SOL_TCP and use an enum for the later, so can't check for its presence with a macro.
 #  define SOL_TCP IPPROTO_TCP
 
+#  ifdef VW_FEAT_NETWORKING_ENABLED
 int daemon(int /*a*/, int /*b*/) { exit(0); }
+#  endif
 
 // Starting with v142 the fix in the else block no longer works due to mismatching linkage. Going forward we should just
 // use the actual isocpp version.
 // use VW_GETPID instead of getpid to avoid name collisions with process.h
 #  if _MSC_VER >= 1920
 #    define VW_GETPID _getpid
 #  else
@@ -203,24 +205,26 @@
 
   if (dsjson && all.output_runtime.global_metrics.are_metrics_enabled())
   {
     all.parser_runtime.example_parser->metrics = VW::make_unique<VW::details::dsjson_metrics>();
   }
 }
 
+#ifdef VW_FEAT_NETWORKING_ENABLED
 void set_daemon_reader(VW::workspace& all, bool json = false, bool dsjson = false)
 {
   if (all.parser_runtime.example_parser->input.isbinary())
   {
     all.parser_runtime.example_parser->reader = VW::parsers::cache::read_example_from_cache;
     all.print_by_ref = VW::details::binary_print_result_by_ref;
   }
   else if (json || dsjson) { set_json_reader(all, dsjson); }
   else { set_string_reader(all); }
 }
+#endif
 
 void VW::details::reset_source(VW::workspace& all, size_t numbits)
 {
   io_buf& input = all.parser_runtime.example_parser->input;
 
   // If in write cache mode then close all of the input files then open the written cache as the new input.
   if (all.parser_runtime.example_parser->write_cache)
@@ -243,14 +247,15 @@
     // Now open the written cache as the new input file.
     input.add_file(VW::io::open_file_reader(all.parser_runtime.example_parser->finalname));
     set_cache_reader(all);
   }
 
   if (all.parser_runtime.example_parser->resettable == true)
   {
+#ifdef VW_FEAT_NETWORKING_ENABLED
     if (all.runtime_config.daemon)
     {
       // wait for all predictions to be sent back to client
       {
         std::unique_lock<std::mutex> lock(all.parser_runtime.example_parser->output_lock);
         all.parser_runtime.example_parser->output_done.wait(lock,
             [&]
@@ -279,14 +284,15 @@
       auto socket = VW::io::wrap_socket_descriptor(f);
       all.output_runtime.final_prediction_sink.push_back(socket->get_writer());
       all.parser_runtime.example_parser->input.add_file(socket->get_reader());
 
       set_daemon_reader(all, is_currently_json_reader(all), is_currently_dsjson_reader(all));
     }
     else
+#endif
     {
       if (!input.is_resettable()) { THROW("Cannot reset source as it is a non-resettable input type.") }
       input.reset();
       for (auto& file : input.get_input_files())
       {
         const auto num_bits_cachefile = cache_numbits(*file);
         if (num_bits_cachefile < numbits)
@@ -392,21 +398,22 @@
     VW::workspace& all, bool quiet, size_t passes, const VW::details::input_options& input_options)
 {
   parse_cache(all, input_options.cache_files, input_options.kill_cache, quiet);
 
   // default text reader
   all.parser_runtime.example_parser->text_reader = VW::parsers::text::read_lines;
 
+#ifdef VW_FEAT_NETWORKING_ENABLED
   if (!input_options.no_daemon && (all.runtime_config.daemon || all.reduction_state.active))
   {
-#ifdef _WIN32
+#  ifdef _WIN32
     WSAData wsaData;
     int lastError = WSAStartup(MAKEWORD(2, 2), &wsaData);
     if (lastError != 0) THROWERRNO("WSAStartup() returned error:" << lastError);
-#endif
+#  endif
     all.parser_runtime.example_parser->bound_sock = static_cast<int>(socket(PF_INET, SOCK_STREAM, 0));
     if (all.parser_runtime.example_parser->bound_sock < 0)
     {
       THROW(fmt::format("socket: {}", VW::io::strerror_to_string(errno)));
     }
 
     int on = 1;
@@ -477,21 +484,21 @@
       pid_file << VW::get_pid() << endl;
       pid_file.close();
     }
 
     if (all.runtime_config.daemon && !all.reduction_state.active)
     {
       // See support notes here: https://github.com/VowpalWabbit/vowpal_wabbit/wiki/Daemon-example
-#ifdef __APPLE__
+#  ifdef __APPLE__
       all.logger.warn("daemon mode is not supported on MacOS.");
-#endif
+#  endif
 
-#ifdef _WIN32
+#  ifdef _WIN32
       THROW("daemon mode is not supported on Windows");
-#else
+#  else
       fclose(stdin);
       // weights will be shared across processes, accessible to children
       all.weights.share(all.length());
 
       // learning state to be shared across children
       size_t mmap_length = sizeof(VW::shared_data);
       VW::shared_data* sd = static_cast<VW::shared_data*>(
@@ -555,20 +562,20 @@
               goto child;
             }
             break;
           }
         }
       }
 
-#endif
+#  endif
     }
 
-#ifndef _WIN32
+#  ifndef _WIN32
   child:
-#endif
+#  endif
     sockaddr_in client_address;
     socklen_t size = sizeof(client_address);
     if (!all.output_config.quiet) { *(all.output_runtime.trace_message) << "calling accept" << endl; }
     auto f_a = static_cast<int>(
         accept(all.parser_runtime.example_parser->bound_sock, reinterpret_cast<sockaddr*>(&client_address), &size));
     if (f_a < 0) THROWERRNO("accept");
 
@@ -585,14 +592,15 @@
 
     if (all.reduction_state.active) { set_string_reader(all); }
     else { set_daemon_reader(all, input_options.json, input_options.dsjson); }
     all.parser_runtime.example_parser->resettable =
         all.parser_runtime.example_parser->write_cache || all.runtime_config.daemon;
   }
   else
+#endif
   {
     if (all.parser_runtime.example_parser->input.num_files() != 0)
     {
       if (!quiet) { *(all.output_runtime.trace_message) << "ignoring text input in favor of cache input" << endl; }
     }
     else
     {
@@ -651,15 +659,19 @@
       all.parser_runtime.chain_hash_json = input_options.chain_hash_json;
     }
   }
 
   if (passes > 1 && !all.parser_runtime.example_parser->resettable)
     THROW("need a cache file for multiple passes : try using  --cache or --cache_file <name>");
 
-  if (!quiet && !all.runtime_config.daemon)
+  if (!quiet
+#ifdef VW_FEAT_NETWORKING_ENABLED
+      && !all.runtime_config.daemon
+#endif
+  )
   {
     *(all.output_runtime.trace_message) << "num sources = " << all.parser_runtime.example_parser->input.num_files()
                                         << endl;
   }
 }
 
 void VW::details::lock_done(parser& p)
```

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/prediction_type.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/prediction_type.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/print_utils.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/print_utils.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/prob_dist_cont.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/prob_dist_cont.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/qr_decomposition.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/qr_decomposition.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/qr_decomposition.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/qr_decomposition.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reduction_stack.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reduction_stack.cc`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,17 @@
 #include "vw/core/cached_learner.h"
 #include "vw/core/global_data.h"  // to get vw struct
 #include "vw/core/learner.h"
 #include "vw/core/simple_label_parser.h"
 #include "vw/core/vw_fwd.h"
 
 // reductions / setup functions
-#include "vw/core/reductions/active.h"
+#ifdef VW_FEAT_NETWORKING_ENABLED
+#  include "vw/core/reductions/active.h"
+#endif
 #include "vw/core/reductions/active_cover.h"
 #include "vw/core/reductions/audit_regressor.h"
 #include "vw/core/reductions/autolink.h"
 #include "vw/core/reductions/automl.h"
 #include "vw/core/reductions/baseline.h"
 #include "vw/core/reductions/baseline_challenger_cb.h"
 #include "vw/core/reductions/bfgs.h"
@@ -87,30 +89,37 @@
 #include "vw/core/reductions/oja_newton.h"
 #include "vw/core/reductions/plt.h"
 #include "vw/core/reductions/pmf_to_pdf.h"
 #include "vw/core/reductions/print.h"
 #include "vw/core/reductions/recall_tree.h"
 #include "vw/core/reductions/sample_pdf.h"
 #include "vw/core/reductions/scorer.h"
-#include "vw/core/reductions/search/search.h"
-#include "vw/core/reductions/sender.h"
+#ifdef VW_FEAT_SEARCH_ENABLED
+#  include "vw/core/reductions/search/search.h"
+#endif
+#ifdef VW_FEAT_NETWORKING_ENABLED
+#  include "vw/core/reductions/sender.h"
+#endif
 #include "vw/core/reductions/shared_feature_merger.h"
 #include "vw/core/reductions/slates.h"
 #include "vw/core/reductions/stagewise_poly.h"
 #include "vw/core/reductions/svrg.h"
 #include "vw/core/reductions/topk.h"
 
 #include <unordered_map>
 
 void register_reductions(std::vector<VW::reduction_setup_fn>& reductions,
     std::vector<std::tuple<std::string, VW::reduction_setup_fn>>& reduction_stack)
 {
   std::unordered_map<VW::reduction_setup_fn, std::string> allowlist = {{VW::reductions::gd_setup, "gd"},
-      {VW::reductions::ftrl_setup, "ftrl"}, {VW::reductions::sender_setup, "sender"}, {VW::reductions::nn_setup, "nn"},
-      {VW::reductions::oaa_setup, "oaa"}, {VW::reductions::scorer_setup, "scorer"},
+      {VW::reductions::ftrl_setup, "ftrl"},
+#ifdef VW_FEAT_NETWORKING_ENABLED
+      {VW::reductions::sender_setup, "sender"},
+#endif
+      {VW::reductions::nn_setup, "nn"}, {VW::reductions::oaa_setup, "oaa"}, {VW::reductions::scorer_setup, "scorer"},
       {VW::reductions::csldf_setup, "csoaa_ldf"},
       {VW::reductions::cb_explore_adf_greedy_setup, "cb_explore_adf_greedy"},
       {VW::reductions::cb_explore_adf_regcb_setup, "cb_explore_adf_regcb"},
       {VW::reductions::shared_feature_merger_setup, "shared_feature_merger"},
       {VW::reductions::generate_interactions_setup, "generate_interactions"},
       {VW::reductions::count_label_setup, "count_label"}, {VW::reductions::cb_to_cb_adf_setup, "cb_to_cbadf"},
       {VW::reductions::cb_actions_mask_setup, "cb_actions_mask"}};
@@ -140,29 +149,33 @@
 
   // Base algorithms
   reductions.push_back(VW::reductions::gd_setup);
   reductions.push_back(VW::reductions::kernel_svm_setup);
   reductions.push_back(VW::reductions::ftrl_setup);
   reductions.push_back(VW::reductions::freegrad_setup);
   reductions.push_back(VW::reductions::svrg_setup);
+#ifdef VW_FEAT_NETWORKING_ENABLED
   reductions.push_back(VW::reductions::sender_setup);
+#endif
   reductions.push_back(VW::reductions::gd_mf_setup);
   reductions.push_back(VW::reductions::print_setup);
   reductions.push_back(VW::reductions::noop_setup);
   reductions.push_back(VW::reductions::bfgs_setup);
   reductions.push_back(VW::reductions::oja_newton_setup);
 
   reductions.push_back(VW::reductions::mf_setup);
 
   reductions.push_back(VW::reductions::generate_interactions_setup);
 
   // Score Users
   reductions.push_back(VW::reductions::baseline_setup);
   reductions.push_back(VW::reductions::expreplay_setup<'b', VW::simple_label_parser_global>);
+#ifdef VW_FEAT_NETWORKING_ENABLED
   reductions.push_back(VW::reductions::active_setup);
+#endif
   reductions.push_back(VW::reductions::active_cover_setup);
   reductions.push_back(VW::reductions::confidence_setup);
   reductions.push_back(VW::reductions::nn_setup);
   reductions.push_back(VW::reductions::marginal_setup);
   reductions.push_back(VW::reductions::autolink_setup);
   reductions.push_back(VW::reductions::lrq_setup);
   reductions.push_back(VW::reductions::lrqfa_setup);
@@ -232,15 +245,17 @@
   reductions.push_back(VW::reductions::sample_pdf_setup);
   reductions.push_back(VW::reductions::cats_setup);
   reductions.push_back(VW::reductions::cbify_setup);
   reductions.push_back(VW::reductions::cbifyldf_setup);
   reductions.push_back(VW::reductions::cb_to_cb_adf_setup);
   reductions.push_back(VW::reductions::offset_tree_setup);
   reductions.push_back(VW::reductions::expreplay_setup<'c', VW::cs_label_parser_global>);
+#ifdef VW_FEAT_SEARCH_ENABLED
   reductions.push_back(VW::reductions::search_setup);
+#endif
   reductions.push_back(VW::reductions::audit_regressor_setup);
   reductions.push_back(VW::reductions::metrics_setup);
   reductions.push_back(VW::reductions::count_label_setup);
 
   register_reductions(reductions, reduction_stack);
 }
```

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/active.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/active.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/active_cover.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/active_cover.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/audit_regressor.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/audit_regressor.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/autolink.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/autolink.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/automl.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/automl.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/baseline.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/baseline.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/baseline_challenger_cb.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/baseline_challenger_cb.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/bfgs.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/bfgs.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/binary.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/binary.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/boosting.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/boosting.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/bs.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/bs.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cats.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cats.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cats_pdf.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cats_pdf.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cats_tree.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cats_tree.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_actions_mask.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_actions_mask.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_adf.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_adf.cc`

 * *Files 2% similar despite different names*

```diff
@@ -51,37 +51,45 @@
     return known_cost;
   }
 
   known_cost.action = found_index;
   return known_cost;
 }
 // Validates a multiline example collection as a valid sequence for action dependent features format.
-VW::example* VW::test_cb_adf_sequence(const VW::multi_ex& ec_seq)
+VW::example* VW::test_cb_adf_sequence(const VW::multi_ex& ec_seq, bool allow_multiple_costs)
 {
   if (ec_seq.empty()) THROW("cb_adf: At least one action must be provided for an example to be valid.");
 
   uint32_t count = 0;
   VW::example* ret = nullptr;
-  for (auto* ec : ec_seq)
+  for (size_t i = 0; i < ec_seq.size(); i++)
   {
+    auto* ec = ec_seq[i];
     // Check if there is more than one cost for this example.
     if (ec->l.cb.costs.size() > 1)
     {
       auto message = fmt::format(
           "cb_adf: badly formatted example, only one cost can be known but found {}. Example number={}, tag={}",
           ec->l.cb.costs.size(), ec->example_counter, VW::string_view{ec->tag.data(), ec->tag.size()});
       THROW(message);
     }
 
     // Check whether the cost was initialized to a value.
     if (ec->l.cb.costs.size() == 1 && ec->l.cb.costs[0].cost != FLT_MAX)
     {
       ret = ec;
       count += 1;
-      if (count > 1) THROW("cb_adf: badly formatted example, only one line can have a cost");
+      if (!allow_multiple_costs)
+      {
+        if (count > 1) THROW("cb_adf: badly formatted example, only one line can have a cost");
+      }
+      else
+      {
+        if (ec->l.cb.costs[0].action == i) { return ret; }
+      }
     }
   }
 
   return ret;
 }
 
 const VW::version_struct* VW::reductions::cb_adf::get_model_file_ver() const
@@ -264,15 +272,15 @@
 }
 
 void VW::reductions::cb_adf::predict(learner& base, VW::multi_ex& ec_seq)
 {
   _offset = ec_seq[0]->ft_offset;
   _offset_index = _offset / _all->weights.stride();
   _gen_cs_dr.known_cost = VW::get_observed_cost_or_default_cb_adf(ec_seq);  // need to set for test case
-  details::gen_cs_test_example(ec_seq, _cs_labels);                     // create test labels.
+  details::gen_cs_test_example(ec_seq, _cs_labels);                         // create test labels.
   details::cs_ldf_learn_or_predict<false>(base, ec_seq, _cb_labels, _cs_labels, _prepped_cs_labels, false, _offset);
 }
 
 // how to
 
 bool VW::reductions::cb_adf::update_statistics(
     const VW::example& ec, const VW::multi_ex& ec_seq, VW::shared_data& sd) const
@@ -342,21 +350,37 @@
   if (c.get_model_file_ver() != nullptr &&
       *c.get_model_file_ver() < VW::version_definitions::VERSION_FILE_WITH_CB_ADF_SAVE)
   {
     return;
   }
 
   std::stringstream msg;
-  msg << "event_sum " << c.get_gen_cs_mtr().per_model_state[0].event_sum << "\n";
-  VW::details::bin_text_read_write_fixed(model_file, (char*)&c.get_gen_cs_mtr().per_model_state[0].event_sum,
-      sizeof(c.get_gen_cs_mtr().per_model_state[0].event_sum), read, msg, text);
-
-  msg << "action_sum " << c.get_gen_cs_mtr().per_model_state[0].action_sum << "\n";
-  VW::details::bin_text_read_write_fixed(model_file, (char*)&c.get_gen_cs_mtr().per_model_state[0].action_sum,
-      sizeof(c.get_gen_cs_mtr().per_model_state[0].action_sum), read, msg, text);
+  if (c.per_model_save_load())
+  {
+    for (size_t ind = 0; ind < c.get_gen_cs_mtr().per_model_state.size(); ++ind)
+    {
+      msg << "event_sum_" << c.get_gen_cs_mtr().per_model_state[ind].event_sum << "\n";
+      VW::details::bin_text_read_write_fixed(model_file, (char*)&c.get_gen_cs_mtr().per_model_state[ind].event_sum,
+          sizeof(c.get_gen_cs_mtr().per_model_state[ind].event_sum), read, msg, text);
+
+      msg << "action_sum " << c.get_gen_cs_mtr().per_model_state[ind].action_sum << "\n";
+      VW::details::bin_text_read_write_fixed(model_file, (char*)&c.get_gen_cs_mtr().per_model_state[ind].action_sum,
+          sizeof(c.get_gen_cs_mtr().per_model_state[ind].action_sum), read, msg, text);
+    }
+  }
+  else
+  {
+    msg << "event_sum " << c.get_gen_cs_mtr().per_model_state[0].event_sum << "\n";
+    VW::details::bin_text_read_write_fixed(model_file, (char*)&c.get_gen_cs_mtr().per_model_state[0].event_sum,
+        sizeof(c.get_gen_cs_mtr().per_model_state[0].event_sum), read, msg, text);
+
+    msg << "action_sum " << c.get_gen_cs_mtr().per_model_state[0].action_sum << "\n";
+    VW::details::bin_text_read_write_fixed(model_file, (char*)&c.get_gen_cs_mtr().per_model_state[0].action_sum,
+        sizeof(c.get_gen_cs_mtr().per_model_state[0].action_sum), read, msg, text);
+  }
 }
 
 void cb_adf_merge(const std::vector<float>& /* per_model_weights */,
     const std::vector<const VW::reductions::cb_adf*>& sources, VW::reductions::cb_adf& output_data)
 {
   for (const auto* source : sources)
   {
@@ -407,14 +431,15 @@
   bool cb_adf_option = false;
   std::string type_string = "mtr";
 
   VW::cb_type_t cb_type;
   bool rank_all;
   float clip_p;
   bool no_predict = false;
+  bool per_model_save_load = false;
 
   option_group_definition new_options("[Reduction] Contextual Bandit with Action Dependent Features");
   new_options
       .add(make_option("cb_adf", cb_adf_option)
                .keep()
                .necessary()
                .help("Do Contextual Bandit learning with multiline action dependent features"))
@@ -424,15 +449,20 @@
                .keep()
                .default_value(0.f)
                .help("Clipping probability in importance weight. Default: 0.f (no clipping)"))
       .add(make_option("cb_type", type_string)
                .keep()
                .default_value("mtr")
                .one_of({"ips", "dm", "dr", "mtr", "sm"})
-               .help("Contextual bandit method to use"));
+               .help("Contextual bandit method to use"))
+      .add(make_option("per_model_save_load", per_model_save_load)
+               .keep()
+               .allow_override()
+               .help("Save and load per model state"));
+  ;
 
   if (!options.add_parse_and_check_necessary(new_options)) { return nullptr; }
 
   // Ensure serialization of this option in all cases.
   if (!options.was_supplied("cb_type"))
   {
     options.insert("cb_type", type_string);
@@ -478,15 +508,16 @@
     if (!options.was_supplied("csoaa_ldf")) { options.insert("csoaa_ldf", "multiline"); }
 
     if (!options.was_supplied("csoaa_rank")) { options.insert("csoaa_rank", ""); }
   }
 
   if (options.was_supplied("baseline") && check_baseline_enabled) { options.insert("check_enabled", ""); }
 
-  auto ld = VW::make_unique<VW::reductions::cb_adf>(cb_type, rank_all, clip_p, no_predict, feature_width_above, &all);
+  auto ld = VW::make_unique<VW::reductions::cb_adf>(
+      cb_type, rank_all, clip_p, no_predict, feature_width_above, per_model_save_load, &all);
 
   auto base = require_multiline(stack_builder.setup_base_learner(feature_width));
 
   VW::reductions::cb_adf* bare = ld.get();
   bool lrp = ld->learn_returns_prediction();
   auto l = make_reduction_learner(std::move(ld), base, learn, predict, stack_builder.get_setupfn_name(cb_adf_setup))
                .set_input_label_type(VW::label_type_t::CB)
```

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_algs.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_algs.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_dro.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_dro.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_explore.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_explore.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_explore_adf_bag.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_explore_adf_bag.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_explore_adf_cover.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_explore_adf_cover.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_explore_adf_first.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_explore_adf_first.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_explore_adf_graph_feedback.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_explore_adf_graph_feedback.cc`

 * *Files 12% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 #include "vw/core/label_dictionary.h"
 #include "vw/core/label_parser.h"
 #include "vw/core/model_utils.h"
 #include "vw/core/parser.h"
 #include "vw/core/reductions/cb/cb_adf.h"
 #include "vw/core/reductions/cb/cb_explore.h"
 #include "vw/core/reductions/cb/cb_explore_adf_common.h"
+#include "vw/core/scope_exit.h"
 #include "vw/core/setup_base.h"
 #include "vw/core/vw_math.h"
 #include "vw/explore/explore.h"
 
 #include <algorithm>
 #define ARMA_DONT_USE_BLAS
 #define ARMA_DONT_USE_LAPACK
@@ -26,18 +27,51 @@
 #include <cmath>
 #include <ensmallen.hpp>
 #include <functional>
 #include <vector>
 
 using namespace VW::cb_explore_adf;
 
+// potential bug in the ensmallen library
+// below method template specialization to be removed once/if that is resolved and the library is updated
+// https://github.com/mlpack/ensmallen/issues/365
+namespace ens
+{
+class L_BFGS;
+
+template <>
+double L_BFGS::ChooseScalingFactor(const size_t iterationNum, const arma::Mat<double>& gradient,
+    const arma::Cube<double>& s, const arma::Cube<double>& y)
+{
+  typedef typename arma::Cube<double>::elem_type CubeElemType;
+
+  double scalingFactor;
+  if (iterationNum > 0)
+  {
+    int previousPos = (iterationNum - 1) % numBasis;
+    // Get s and y matrices once instead of multiple times.
+    const arma::Mat<CubeElemType>& sMat = s.slice(previousPos);
+    const arma::Mat<CubeElemType>& yMat = y.slice(previousPos);
+
+    scalingFactor = dot(sMat, yMat) / std::max(1e-12, dot(yMat, yMat));
+  }
+  else { scalingFactor = 1.0 / sqrt(dot(gradient, gradient)); }
+
+  return scalingFactor;
+}
+}  // namespace ens
+
 namespace VW
 {
 namespace cb_explore_adf
 {
+constexpr double ALMOST_ZERO = 1e-6;
+constexpr double EPSILON = 1e-3;
+constexpr double GAMMA_CUTOFF = 1.0;
+
 class cb_explore_adf_graph_feedback
 {
 public:
   cb_explore_adf_graph_feedback(float gamma_scale, float gamma_exponent, VW::workspace* all)
       : _gamma_scale(gamma_scale), _gamma_exponent(gamma_exponent), _all(all)
   {
   }
@@ -49,15 +83,15 @@
   float _gamma_scale;
   float _gamma_exponent;
 
 private:
   VW::workspace* _all;
   template <bool is_learn>
   void predict_or_learn_impl(VW::LEARNER::learner& base, multi_ex& examples);
-  void update_example_prediction(multi_ex& examples);
+  void update_example_prediction(multi_ex& examples, const arma::sp_mat& G);
 };
 }  // namespace cb_explore_adf
 
 /**
  * Implementing the constrained optimization from the paper: https://arxiv.org/abs/2302.08631
  * We want to minimize objective: p * fhat + z
  * where p is the resulting probability distribution, fhat is the scores we get from cb_adf and z is a constant
@@ -88,297 +122,265 @@
  * an action has a high cost it will have a lower probability of being chosen even if it reveals a lot of information
  * about other actions
  */
 class ConstrainedFunctionType
 {
   const arma::vec& _fhat;
   const arma::sp_mat& _G;
-  const float _gamma;
+  const double _gamma;
 
 public:
-  ConstrainedFunctionType(const arma::vec& scores, const arma::sp_mat& G, const float gamma)
+  ConstrainedFunctionType(const arma::vec& scores, const arma::sp_mat& G, const double gamma)
       : _fhat(scores), _G(G), _gamma(gamma)
   {
   }
 
   // Return the objective function f(x) for the given x.
-  double Evaluate(const arma::mat& x) const
+  double Evaluate(const arma::mat& x)
   {
     arma::mat p(x.n_rows - 1, 1);
-    for (size_t i = 0; i < p.n_rows; ++i) { p[i] = x[i]; }
+    for (size_t i = 0; i < x.n_rows - 1; ++i) { p[i] = x[i]; }
 
-    float z = x[x.n_rows - 1];
+    auto z = x[x.n_rows - 1];
 
-    return (arma::dot(p, _fhat) + z);
+    return (arma::dot(_fhat, p) + z);
   }
 
   // Compute the gradient of f(x) for the given x and store the result in g.
-  void Gradient(const arma::mat&, arma::mat& g) const
+  void Gradient(const arma::mat& x, arma::mat& g)
+  {
+    g.set_size(x.n_rows, 1);
+    g.zeros();
+    for (size_t i = 0; i < x.n_rows - 1; ++i) { g[i] = _fhat[i]; }
+    g[x.n_rows - 1] = 1.0;
+  }
+
+  void NumericalGradient(const arma::mat& x, arma::mat& g)
   {
     g.set_size(_fhat.n_rows + 1, 1);
-    for (size_t i = 0; i < _fhat.n_rows; ++i) { g[i] = _fhat(i); }
-    g[_fhat.n_rows] = 1.f;
+    g.zeros();
+    for (size_t i = 0; i < _fhat.n_rows; ++i)
+    {
+      arma::mat x_i_plus = x;
+      x_i_plus(i) += EPSILON;
+      arma::mat x_i_minus = x;
+      x_i_minus(i) -= EPSILON;
+      g(i) = (Evaluate(x_i_plus) - Evaluate(x_i_minus)) / (2.0 * EPSILON);
+    }
   }
 
   // Get the number of constraints on the objective function.
-  size_t NumConstraints() const { return _fhat.size() + 4; }
+  size_t NumConstraints() const { return 3 * _fhat.size() + 2; }
 
   // Evaluate constraint i at the parameters x.  If the constraint is
   // unsatisfied, a value greater than 0 should be returned.  If the constraint
   // is satisfied, 0 should be returned.  The optimizer will add this value to
   // its overall objective that it is trying to minimize.
-  double EvaluateConstraint(const size_t i, const arma::mat& x) const
+  double EvaluateConstraint(const size_t i, const arma::mat& x)
   {
     arma::vec p(x.n_rows - 1);
-    for (size_t i = 0; i < p.n_rows; ++i) { p(i) = x[i]; }
+    for (size_t i = 0; i < x.n_rows - 1; ++i) { p[i] = x[i]; }
 
-    float z = x[x.n_rows - 1];
+    double z = x[x.n_rows - 1];
 
     if (i < _fhat.size())
     {
       arma::vec eyea = arma::zeros<arma::vec>(p.n_rows);
-      eyea(i) = 1.f;
+      eyea(i) = 1;
 
-      auto fhata = _fhat(i);
+      double fhata = _fhat(i);
 
-      double sum = 0.f;
+      double sum = 0;
       for (size_t index = 0; index < p.n_rows; index++)
       {
-        arma::vec Ga(_G.row(index).n_cols);
-        for (size_t j = 0; j < _G.row(index).n_cols; j++) { Ga(j) = _G.row(index)(j); }
-
-        auto Ga_times_p = arma::dot(Ga, p);
+        double Ga_times_p = std::max(arma::dot(_G.row(index), p.t()), ALMOST_ZERO);
 
-        float denominator = Ga_times_p;
-        auto nominator = (eyea(index) - p(index)) * (eyea(index) - p(index));
-        sum += (nominator / denominator);
+        double g_x = Ga_times_p;
+        double f_x = (eyea(index) - p(index)) * (eyea(index) - p(index));
+        sum += (f_x / g_x);
       }
-      if (sum <= (fhata + z)) { return 0.f; }
-      else { return sum - (fhata + z); }
+
+      double lhs = _gamma < GAMMA_CUTOFF ? sum : sum / _gamma;
+      double rhs = _gamma < GAMMA_CUTOFF ? _gamma * (fhata + z) : (fhata + z);
+      if (lhs <= rhs) { return 0.0; }
+      return lhs - rhs;
     }
     else if (i == _fhat.size())
     {
-      if (arma::all(p >= 0.f)) { return 0.f; }
-      double neg_sum = 0.;
-      for (size_t i = 0; i < p.n_rows; i++)
-      {
-        if (p(i) < 0) { neg_sum += p(i); }
-      }
-      // negative probabilities are really really bad
-      return -100.f * _gamma * neg_sum;
+      if (arma::sum(p) >= (1.0 - 1e-3)) { return 0.0; }
+      return (1.0 - 1e-3) - arma::sum(p);
     }
     else if (i == _fhat.size() + 1)
     {
-      if (arma::sum(p) <= 1.f) { return 0.f; }
-      return arma::sum(p) - 1.f;
+      if (arma::sum(p) <= (1.0 + 1e-3)) { return 0.0; }
+      return arma::sum(p) - (1.0 + 1e-3);
     }
-    else if (i == _fhat.size() + 2)
+    else if (i > _fhat.size() + 1 && i < 2 * _fhat.size() + 2)
     {
-      if (arma::sum(p) >= 1.f) { return 0.f; }
-      return 1.f - arma::sum(p);
+      size_t index = i - _fhat.size() - 2;
+
+      double Gpa = arma::dot(_G.row(index), p.t());
+
+      if (Gpa >= ALMOST_ZERO) { return 0; }
+      return ALMOST_ZERO - Gpa;
     }
-    else if (i == _fhat.size() + 3)
+    else if (i >= 2 * _fhat.size() + 2)
     {
-      if ((z / _gamma) > 0.f) { return 0.f; }
-      return 0.f - (z / _gamma);
+      size_t index = i - 2 * _fhat.size() - 2;
+      if (p[index] >= 0.0) { return 0.0; }
+      return -1.0 * p[index];
+    }
+    return 0.0;
+  }
+
+  void NumericalGradientConstraint(const size_t i, const arma::mat& x, arma::mat& g)
+  {
+    g.set_size(_fhat.n_rows + 1, 1);
+    g.zeros();
+
+    for (size_t j = 0; j < _fhat.n_rows; ++j)
+    {
+      arma::mat x_j_plus = x;
+      x_j_plus(j) += EPSILON;
+      arma::mat x_j_minus = x;
+      x_j_minus(j) -= EPSILON;
+      double cp = EvaluateConstraint(i, x_j_plus);
+      double cm = EvaluateConstraint(i, x_j_minus);
+      g(j) = (cp - cm) / (2.0 * EPSILON);
     }
-    return 0.;
   }
 
   // Evaluate the gradient of constraint i at the parameters x, storing the
   // result in the given matrix g.  If the constraint is not satisfied, the
   // gradient should be set in such a way that the gradient points in the
   // direction where the constraint would be satisfied.
-  void GradientConstraint(const size_t i, const arma::mat& x, arma::mat& g) const
+  void GradientConstraint(const size_t i, const arma::mat& x, arma::mat& g)
   {
     arma::vec p(x.n_rows - 1);
     for (size_t i = 0; i < p.n_rows; ++i) { p(i) = x[i]; }
 
-    float z = x[x.n_rows - 1];
+    g.set_size(_fhat.n_rows + 1, 1);
 
-    double constraint = EvaluateConstraint(i, x);
+    if (EvaluateConstraint(i, x) <= 0)
+    {
+      g.zeros();
+      return;
+    }
 
     if (i < _fhat.size())
     {
-      g.set_size(_fhat.n_rows + 1, 1);
       g.zeros();
 
-      g[_fhat.size()] = 1.f;
+      g[_fhat.size()] = 1.0;
 
       arma::vec eyea = arma::zeros<arma::vec>(p.n_rows);
-      eyea(i) = 1.f;
+      eyea(i) = 1;
 
       for (size_t coord_i = 0; coord_i < _fhat.size(); coord_i++)
       {
-        double sum = 0.f;
+        double sum = 0;
         for (size_t index = 0; index < p.n_rows; index++)
         {
-          arma::vec Ga(_G.row(index).n_cols);
-          for (size_t j = 0; j < _G.row(index).n_cols; j++) { Ga(j) = _G.row(index)(j); }
-          auto Ga_times_p = arma::dot(Ga, p);
+          double Ga_times_p = arma::dot(_G.row(index), p.t());
 
-          if (index == coord_i)
-          {
-            float denominator = Ga_times_p * Ga_times_p;
+          double g_x = std::max(Ga_times_p, ALMOST_ZERO);
 
-            auto b = _G.row(index)(index);
-            auto c = Ga_times_p - b * p(index);
-            auto nominator = -1.f * ((eyea(index) - p(index)) * (eyea(index) * b + b * p(index) + 2.f * c));
-
-            sum += (nominator / denominator);
-          }
-          else
-          {
-            auto a = (eyea(index) - p(index)) * (eyea(index) - p(index));
-            auto b = _G.row(index)(coord_i);
+          double g_x_der = Ga_times_p > ALMOST_ZERO ? _G.row(index)(coord_i) : 0.0;
+          double f_x = (eyea(index) - p(index)) * (eyea(index) - p(index));
+          double f_x_der = index == coord_i ? -2. * (eyea(index) - p(index)) : 0.0;
+
+          double quotient_rule = (g_x * f_x_der - f_x * g_x_der) / (g_x * g_x);
 
-            auto nominator = -1.f * ((a * b));
-            auto denominator = Ga_times_p * Ga_times_p;
-            sum += nominator / denominator;
-          }
+          sum += quotient_rule;
         }
 
-        g[coord_i] = sum;
+        g[coord_i] = _gamma < GAMMA_CUTOFF ? sum : sum / _gamma;
       }
 
-      if (constraint == 0.f)
-      {
-        g = -1.f * g;
-        // restore original point not concerned with the constraint
-        g[_fhat.size()] = 1.f;
-      }
+      g[_fhat.size()] = _gamma < GAMMA_CUTOFF ? -1.0 * _gamma : -1.0;
     }
     else if (i == _fhat.size())
     {
-      // all positives
-      g.set_size(_fhat.n_rows + 1, 1);
+      // sum
       g.ones();
+      g = -1.0 * g;
 
-      for (size_t i = 0; i < p.n_rows; ++i)
-      {
-        if (p(i) < 0.f)
-        {
-          for (size_t i = 0; i < _fhat.size(); i++) { g[i] = -1.f; }
-        }
-      }
-
-      g[_fhat.size()] = 0.f;
+      g[_fhat.size()] = 0.0;
     }
     else if (i == _fhat.size() + 1)
     {
-      // sum
-      g.set_size(_fhat.n_rows + 1, 1);
       g.ones();
-
-      if (constraint == 0.f) { g = -1.f * g; }
-
-      g[_fhat.size()] = 0.f;
+      g[_fhat.size()] = 0.0;
     }
-    else if (i == _fhat.size() + 2)
+    else if (i > _fhat.size() + 1 && i < 2 * _fhat.size() + 2)
     {
-      // sum
-      g.set_size(_fhat.n_rows + 1, 1);
-      g.ones();
-
-      if (constraint != 0.f) { g = -1.f * g; }
-
-      g[_fhat.size()] = 0.f;
+      g.zeros();
+      size_t index = i - _fhat.size() - 2;
+      for (size_t j = 0; j < _fhat.size(); ++j) { g(j) = -1.0 * _G(index, j); }
+      g[_fhat.size()] = 0.0;
     }
-    else if (i == _fhat.size() + 3)
+    else if (i >= 2 * _fhat.size() + 2)
     {
-      g.set_size(_fhat.n_rows + 1, 1);
-      g.ones();
-
-      if ((z / _gamma) < 0.f) { g[_fhat.size()] = -1.f; }
+      size_t index = i - 2 * _fhat.size() - 2;
+      // all positives
+      g.zeros();
+      g(index) = -1.0;
     }
   }
 };
 
-bool valid_graph(const std::vector<VW::cb_graph_feedback::triplet>& triplets)
+std::vector<VW::cb_graph_feedback::triplet> get_valid_graph(
+    const std::vector<VW::cb_graph_feedback::triplet>& triplets, size_t dim)
 {
-  // return false if all triplet vals are zero
+  std::vector<VW::cb_graph_feedback::triplet> valid_triplets;
   for (auto& triplet : triplets)
   {
-    if (triplet.val != 0.f) { return true; }
+    if (triplet.row < dim && triplet.col < dim) { valid_triplets.push_back(triplet); }
   }
-  return false;
+
+  return valid_triplets;
+  ;
 }
 
-std::pair<arma::mat, arma::vec> set_initial_coordinates(const arma::vec& fhat, float gamma)
+std::pair<arma::mat, arma::vec> set_initial_coordinates(const arma::vec& fhat, double gamma)
 {
   // find fhat min
   auto min_fhat = fhat.min();
-  arma::vec gammafhat = gamma * (fhat - min_fhat);
+  arma::vec positivefhat = (fhat - min_fhat);
 
   // initial p can be uniform random
-  arma::mat coordinates(gammafhat.size() + 1, 1);
-  for (size_t i = 0; i < gammafhat.size(); i++) { coordinates[i] = 1.f / gammafhat.size(); }
+  arma::mat coordinates(positivefhat.size() + 1, 1);
+  for (size_t i = 0; i < positivefhat.size(); i++) { coordinates[i] = 1.0 / positivefhat.size(); }
 
-  // initial z can be 1
-  // but also be nice if all fhat's are zero
-  float z = gamma * (1 - (min_fhat == 0 ? 1.f / fhat.size() : min_fhat));
+  // initial z
+  double z = gamma < GAMMA_CUTOFF ? 1.0 : (1.0 / gamma);
 
-  coordinates[gammafhat.size()] = z;
+  coordinates[positivefhat.size()] = z;
 
-  return {coordinates, gammafhat};
+  return {coordinates, positivefhat};
 }
 
-arma::vec get_probs_from_coordinates(arma::mat& coordinates, const arma::vec& fhat, VW::workspace& all)
+arma::vec get_probs_from_coordinates(arma::mat& coordinates, VW::workspace& all)
 {
   // constraints are enforcers but they can be broken, so we need to check that probs are positive and sum to 1
 
-  // we also have to check for nan's because some starting points combined with some gammas might make the constraint
-  // optimization go off the charts; it should be rare but we need to guard against it
-
   size_t num_actions = coordinates.n_rows - 1;
-  auto count_zeros = 0;
-  bool there_is_a_one = false;
-  bool there_is_a_nan = false;
 
   for (size_t i = 0; i < num_actions; i++)
   {
-    if (VW::math::are_same(static_cast<float>(coordinates[i]), 0.f) || coordinates[i] < 0.f)
-    {
-      coordinates[i] = 0.f;
-      count_zeros++;
-    }
-    if (coordinates[i] > 1.f)
-    {
-      coordinates[i] = 1.f;
-      there_is_a_one = true;
-    }
-    if (std::isnan(coordinates[i])) { there_is_a_nan = true; }
-  }
-
-  if (there_is_a_nan)
-  {
-    for (size_t i = 0; i < num_actions; i++) { coordinates[i] = 1.f - fhat(i); }
-  }
-
-  if (there_is_a_one)
-  {
-    for (size_t i = 0; i < num_actions; i++)
-    {
-      if (coordinates[i] != 1.f) { coordinates[i] = 0.f; }
-    }
+    if (std::isnan(coordinates[i])) { continue; }
+    // clip to [0,1]
+    coordinates[i] = std::max(0., std::min(coordinates[i], 1.));
   }
 
   float p_sum = 0;
   for (size_t i = 0; i < num_actions; i++) { p_sum += coordinates[i]; }
 
-  if (!VW::math::are_same(p_sum, 1.f))
-  {
-    float rest = 1.f - p_sum;
-    float rest_each = rest / (num_actions - count_zeros);
-    for (size_t i = 0; i < num_actions; i++)
-    {
-      if (coordinates[i] == 0.f) { continue; }
-      else { coordinates[i] = coordinates[i] + rest_each; }
-    }
-  }
+  // normalize
+  for (size_t i = 0; i < num_actions; i++) { coordinates[i] = coordinates[i] / p_sum; }
 
   float sum = 0;
   arma::vec probs(num_actions);
   for (size_t i = 0; i < probs.n_rows; ++i)
   {
     probs(i) = coordinates[i];
     sum += probs(i);
@@ -389,83 +391,112 @@
     // leaving this here just in case this happens for some reason that we did not think to check for
     all.logger.warn("Probabilities do not sum to 1, they sum to: {}", sum);
   }
 
   return probs;
 }
 
-arma::sp_mat get_graph(const VW::cb_graph_feedback::reduction_features& graph_reduction_features, size_t num_actions)
-{
-  arma::sp_mat G(num_actions, num_actions);
-
-  if (valid_graph(graph_reduction_features.triplets))
-  {
-    arma::umat locations(2, graph_reduction_features.triplets.size());
-
-    arma::vec values(graph_reduction_features.triplets.size());
-
-    for (size_t i = 0; i < graph_reduction_features.triplets.size(); i++)
-    {
-      const auto& triplet = graph_reduction_features.triplets[i];
-      locations(0, i) = triplet.row;
-      locations(1, i) = triplet.col;
-      values(i) = triplet.val;
-    }
-
-    G = arma::sp_mat(true, locations, values, num_actions, num_actions);
-  }
-  else { G = arma::speye<arma::sp_mat>(num_actions, num_actions); }
-  return G;
-}
-
-void cb_explore_adf_graph_feedback::update_example_prediction(multi_ex& examples)
+void cb_explore_adf_graph_feedback::update_example_prediction(multi_ex& examples, const arma::sp_mat& G)
 {
   auto& a_s = examples[0]->pred.a_s;
-  size_t num_actions = a_s.size();
   arma::vec fhat(a_s.size());
 
   for (auto& as : a_s) { fhat(as.action) = as.score; }
-  const float gamma = _gamma_scale * static_cast<float>(std::pow(_counter, _gamma_exponent));
+  const double gamma = static_cast<double>(_gamma_scale) * static_cast<double>(std::pow(_counter, _gamma_exponent));
 
-  auto coord_gammafhat = set_initial_coordinates(fhat, gamma);
-  arma::mat coordinates = std::get<0>(coord_gammafhat);
-  arma::vec gammafhat = std::get<1>(coord_gammafhat);
-
-  auto& graph_reduction_features =
-      examples[0]->ex_reduction_features.template get<VW::cb_graph_feedback::reduction_features>();
-  arma::sp_mat G = get_graph(graph_reduction_features, num_actions);
-
-  ConstrainedFunctionType f(gammafhat, G, gamma);
+  auto coord_positivefhat = set_initial_coordinates(fhat, gamma);
+  arma::mat coordinates = std::get<0>(coord_positivefhat);
+  arma::vec positivefhat = std::get<1>(coord_positivefhat);
 
+  ConstrainedFunctionType f(positivefhat, G, gamma);
   ens::AugLagrangian optimizer;
   optimizer.Optimize(f, coordinates);
 
-  // TODO json graph input
-
-  arma::vec probs = get_probs_from_coordinates(coordinates, fhat, *_all);
+  arma::vec probs = get_probs_from_coordinates(coordinates, *_all);
 
   // set the new probabilities in the example
   for (auto& as : a_s) { as.score = probs(as.action); }
   std::sort(
       a_s.begin(), a_s.end(), [](const VW::action_score& a, const VW::action_score& b) { return a.score > b.score; });
 }
 
+arma::sp_mat get_graph(const VW::cb_graph_feedback::reduction_features& graph_reduction_features, size_t num_actions,
+    VW::io::logger& logger)
+{
+  arma::sp_mat G(num_actions, num_actions);
+
+  auto valid_graph = get_valid_graph(graph_reduction_features.triplets, num_actions);
+  if (valid_graph.size() != graph_reduction_features.triplets.size())
+  {
+    logger.warn("The graph provided is invalid, any coordinates that are out of bounds will be ignored");
+  }
+
+  arma::umat locations(2, valid_graph.size());
+
+  arma::vec values(valid_graph.size());
+
+  for (size_t i = 0; i < valid_graph.size(); i++)
+  {
+    const auto& triplet = valid_graph[i];
+    locations(0, i) = triplet.row;
+    locations(1, i) = triplet.col;
+    values(i) = triplet.val;
+  }
+
+  return arma::sp_mat(true, locations, values, num_actions, num_actions);
+}
+
 template <bool is_learn>
 void cb_explore_adf_graph_feedback::predict_or_learn_impl(VW::LEARNER::learner& base, multi_ex& examples)
 {
+  auto& graph_reduction_features =
+      examples[0]->ex_reduction_features.template get<VW::cb_graph_feedback::reduction_features>();
+  arma::sp_mat G = get_graph(graph_reduction_features, examples.size(), _all->logger);
+
   if (is_learn)
   {
     _counter++;
-    base.learn(examples);
-    if (base.learn_returns_prediction) { update_example_prediction(examples); }
+    std::vector<std::vector<VW::cb_class>> cb_labels;
+    cb_labels.reserve(examples.size());
+
+    // stash all of the labels
+    for (size_t i = 0; i < examples.size(); i++)
+    {
+      cb_labels.emplace_back(std::move(examples[i]->l.cb.costs));
+      examples[i]->l.cb.costs.clear();
+    }
+
+    auto restore_guard = VW::scope_exit(
+        [&examples, &cb_labels]
+        {
+          for (size_t i = 0; i < examples.size(); i++) { examples[i]->l.cb.costs = std::move(cb_labels[i]); }
+        });
+
+    // re-instantiate the labels one-by-one and call learn
+    for (size_t i = 0; i < examples.size(); i++)
+    {
+      auto* ex = examples[i];
+
+      ex->l.cb.costs = std::move(cb_labels[i]);
+
+      auto local_restore_guard = VW::scope_exit(
+          [&ex, &cb_labels, &i]
+          {
+            cb_labels[i] = std::move(ex->l.cb.costs);
+            ex->l.cb.costs.clear();
+          });
+
+      // if there is another label then learn, otherwise skip
+      if (ex->l.cb.costs.size() > 0) { base.learn(examples); }
+    }
   }
   else
   {
     base.predict(examples);
-    update_example_prediction(examples);
+    update_example_prediction(examples, G);
   }
 }
 
 void cb_explore_adf_graph_feedback::predict(VW::LEARNER::learner& base, multi_ex& examples)
 {
   predict_or_learn_impl<false>(base, examples);
 }
@@ -474,33 +505,31 @@
 {
   predict_or_learn_impl<true>(base, examples);
 }
 
 void cb_explore_adf_graph_feedback::save_load(VW::io_buf& io, bool read, bool text)
 {
   if (io.num_files() == 0) { return; }
-  if (!read)
-  {
-    std::stringstream msg;
-    if (!read) { msg << "cb adf with graph feedback storing example counter:  = " << _counter << "\n"; }
-    VW::details::bin_text_read_write_fixed_validated(
-        io, reinterpret_cast<char*>(&_counter), sizeof(_counter), read, msg, text);
-  }
+
+  std::stringstream msg;
+  if (!read) { msg << "cb adf with graph feedback storing example counter:  = " << _counter << "\n"; }
+  VW::details::bin_text_read_write_fixed_validated(
+      io, reinterpret_cast<char*>(&_counter), sizeof(_counter), read, msg, text);
 }
 
 std::shared_ptr<VW::LEARNER::learner> VW::reductions::cb_explore_adf_graph_feedback_setup(
     VW::setup_base_i& stack_builder)
 {
   VW::config::options_i& options = *stack_builder.get_options();
   VW::workspace& all = *stack_builder.get_all_pointer();
   using config::make_option;
   bool cb_explore_adf_option = false;
   bool graph_feedback = false;
   float gamma_scale = 1.;
-  float gamma_exponent = 0.;
+  float gamma_exponent = 0.5;
 
   config::option_group_definition new_options(
       "[Reduction] Experimental: Contextual Bandit Exploration with ADF with graph feedback");
   new_options
       .add(make_option("cb_explore_adf", cb_explore_adf_option)
                .keep()
                .necessary()
@@ -525,25 +554,26 @@
 
   using explore_type = cb_explore_adf_base<cb_explore_adf_graph_feedback>;
 
   size_t problem_multiplier = 1;
   bool with_metrics = options.was_supplied("extra_metrics");
 
   auto data = VW::make_unique<explore_type>(with_metrics, gamma_scale, gamma_exponent, &all);
+  data->set_allow_multiple_costs(true);
 
   auto l = VW::LEARNER::make_reduction_learner(std::move(data), base, explore_type::learn, explore_type::predict,
       stack_builder.get_setupfn_name(VW::reductions::cb_explore_adf_graph_feedback_setup))
                .set_input_label_type(VW::label_type_t::CB)
                .set_output_label_type(VW::label_type_t::CB)
                .set_input_prediction_type(VW::prediction_type_t::ACTION_SCORES)
                .set_output_prediction_type(VW::prediction_type_t::ACTION_PROBS)
                .set_feature_width(problem_multiplier)
                .set_output_example_prediction(explore_type::output_example_prediction)
                .set_update_stats(explore_type::update_stats)
                .set_print_update(explore_type::print_update)
                .set_persist_metrics(explore_type::persist_metrics)
                .set_save_load(explore_type::save_load)
-               .set_learn_returns_prediction(base->learn_returns_prediction)
+               .set_learn_returns_prediction(false)
                .build();
   return l;
 }
-}  // namespace VW
+}  // namespace VW
```

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_explore_adf_greedy.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_explore_adf_greedy.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_explore_adf_large_action_space.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_explore_adf_large_action_space.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_explore_adf_regcb.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_explore_adf_regcb.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_explore_adf_rnd.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_explore_adf_rnd.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_explore_adf_softmax.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_explore_adf_softmax.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_explore_adf_squarecb.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_explore_adf_squarecb.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_explore_adf_synthcover.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_explore_adf_synthcover.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_explore_pdf.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_explore_pdf.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_sample.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_sample.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_to_cb_adf.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_to_cb_adf.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cbify.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cbify.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/details/large_action/compute_dot_prod_avx2.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/details/large_action/compute_dot_prod_avx2.cc`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // Copyright (c) by respective owners including Yahoo!, Microsoft, and
 // individual contributors. All rights reserved. Released under a BSD (revised)
 // license as described in the file LICENSE.
 
-#ifdef BUILD_LAS_WITH_SIMD
+#ifdef VW_FEAT_LAS_SIMD_ENABLED
 
 #  include "compute_dot_prod_simd.h"
 #  include "kernel_impl.h"
 
 #  include <x86intrin.h>
 
 namespace VW
```

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/details/large_action/compute_dot_prod_avx512.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/details/large_action/compute_dot_prod_avx512.cc`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // Copyright (c) by respective owners including Yahoo!, Microsoft, and
 // individual contributors. All rights reserved. Released under a BSD (revised)
 // license as described in the file LICENSE.
 
-#ifdef BUILD_LAS_WITH_SIMD
+#ifdef VW_FEAT_LAS_SIMD_ENABLED
 
 #  include "compute_dot_prod_simd.h"
 #  include "kernel_impl.h"
 
 #  include <x86intrin.h>
 
 namespace VW
```

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/details/large_action/compute_dot_prod_scalar.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/details/large_action/compute_dot_prod_scalar.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/details/large_action/compute_dot_prod_simd.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/details/large_action/compute_dot_prod_simd.h`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 // individual contributors. All rights reserved. Released under a BSD (revised)
 // license as described in the file LICENSE.
 
 #pragma once
 
 // TODO: Make simd work with MSVC. Only works on linux for now.
 // TODO: Only works for x86. Make simd work on other architectures e.g. using SIMDe.
-#ifdef BUILD_LAS_WITH_SIMD
+#ifdef VW_FEAT_LAS_SIMD_ENABLED
 
 #  include "vw/core/example.h"
 #  include "vw/core/global_data.h"
 
 namespace VW
 {
 namespace cb_explore_adf
```

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/details/large_action/kernel_impl.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/details/large_action/kernel_impl.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/details/large_action/one_pass_svd_impl.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/details/large_action/one_pass_svd_impl.cc`

 * *Files 2% similar despite different names*

```diff
@@ -81,15 +81,15 @@
   }
 
   const float scaling_factor = 1.f / std::sqrt(p);
   // resize is a no-op if size does not change
   AOmega.resize(num_actions, p);
 
   auto compute_dot_prod = compute_dot_prod_scalar;
-#ifdef BUILD_LAS_WITH_SIMD
+#ifdef VW_FEAT_LAS_SIMD_ENABLED
   switch (_use_simd)
   {
     case (simd_type::AVX512):
       compute_dot_prod = compute_dot_prod_avx512;
       break;
     case (simd_type::AVX2):
       compute_dot_prod = compute_dot_prod_avx2;
@@ -176,15 +176,15 @@
     : _all(all)
     , _d(d)
     , _seed(seed)
     , _thread_pool(thread_pool_size)
     , _block_size(block_size)
     , _action_cache_slack(action_cache_slack)
 {
-#ifdef BUILD_LAS_WITH_SIMD
+#ifdef VW_FEAT_LAS_SIMD_ENABLED
   _use_simd = simd_type::NO_SIMD;
   if (use_explicit_simd)
   {
     if (cpu_supports_avx512()) { _use_simd = simd_type::AVX512; }
     else if (cpu_supports_avx2()) { _use_simd = simd_type::AVX2; }
     else { all->logger.err_warn("System does not support AVX512 or AVX2. Using scalar code path."); }
   }
```

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/details/large_action/one_rank_spanner_impl.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/details/large_action/one_rank_spanner_impl.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/details/large_action/two_pass_svd_impl.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/details/large_action/two_pass_svd_impl.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/details/large_action_space.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/details/large_action_space.h`

 * *Files 2% similar despite different names*

```diff
@@ -69,26 +69,26 @@
   void run(const multi_ex& examples, const std::vector<float>& shrink_factors, Eigen::MatrixXf& U, Eigen::VectorXf& S,
       Eigen::MatrixXf& _V);
   void generate_AOmega(const multi_ex& examples, const std::vector<float>& shrink_factors);
 
   // for testing purposes only
   void _test_only_set_rank(uint64_t rank);
   bool _set_testing_components = false;
-#ifdef BUILD_LAS_WITH_SIMD
+#ifdef VW_FEAT_LAS_SIMD_ENABLED
   bool _test_only_use_simd() { return _use_simd != simd_type::NO_SIMD; }
 #endif
 
 private:
   VW::workspace* _all;
   uint64_t _d;
   uint64_t _seed;
   thread_pool _thread_pool;
   size_t _block_size;
   size_t _action_cache_slack;
-#ifdef BUILD_LAS_WITH_SIMD
+#ifdef VW_FEAT_LAS_SIMD_ENABLED
   enum class simd_type
   {
     NO_SIMD,
     AVX2,
     AVX512
   };
   simd_type _use_simd = simd_type::NO_SIMD;
```

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/warm_cb.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/warm_cb.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cbzo.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cbzo.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/classweight.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/classweight.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/conditional_contextual_bandit.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/conditional_contextual_bandit.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/confidence.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/confidence.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/count_label.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/count_label.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cs_active.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cs_active.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/csoaa.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/csoaa.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/csoaa_ldf.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/csoaa_ldf.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/details/automl/automl_impl.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/details/automl/automl_impl.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/details/automl/automl_iomodel.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/details/automl/automl_iomodel.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/details/automl/automl_oracle.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/details/automl/automl_oracle.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/details/automl/automl_util.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/details/automl/automl_util.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/ect.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/ect.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/eigen_memory_tree.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/eigen_memory_tree.cc`

 * *Files 21% similar despite different names*

```diff
@@ -64,14 +64,48 @@
   if (val == "random") { return emt_router_type::RANDOM; }
 
   if (val == "eigen") { return emt_router_type::EIGEN; }
 
   THROW(fmt::format("{} is not valid emt_router_type", val));
 }
 
+emt_initial_type emt_initial_type_from_string(VW::string_view val)
+{
+  if (val == "gaussian") { return emt_initial_type::GAUSSIAN; }
+
+  if (val == "cosine") { return emt_initial_type::COSINE; }
+
+  if (val == "euclidean") { return emt_initial_type::EUCLIDEAN; }
+
+  if (val == "none") { return emt_initial_type::NONE; }
+
+  THROW(fmt::format("{} is not valid emt_initial_type", val));
+}
+
+float emt_initial(emt_initial_type initial_type, emt_feats f1, emt_feats f2)
+{
+  if (initial_type == emt_initial_type::GAUSSIAN) { return 1 - std::exp(-emt_norm(emt_scale_add(1, f1, -1, f2))); }
+
+  if (initial_type == emt_initial_type::COSINE)
+  {
+    auto den = (emt_norm(f1) * emt_norm(f2));
+    if (den != 0) { return 1 - emt_inner(f1, f2) / den; }
+    else
+    {
+      // cosine distance isn't defined for vectors of size 0 so
+      // we default to a gaussian loss as a fallback distance
+      return 1 - std::exp(-emt_norm(emt_scale_add(1, f1, -1, f2)));
+    }
+  }
+
+  if (initial_type == emt_initial_type::EUCLIDEAN) { return emt_norm(emt_scale_add(1, f1, -1, f2)); }
+
+  return 0;
+}
+
 emt_example::emt_example(VW::workspace& all, VW::example* ex)
 {
   label = ex->l.multi.label;
 
   std::vector<std::vector<VW::namespace_index>>* full_interactions = ex->interactions;
   std::vector<std::vector<VW::namespace_index>> base_interactions;
 
@@ -117,20 +151,21 @@
     map.erase(last_value);
     return last_value;
   }
   return nullptr;
 }
 
 emt_tree::emt_tree(VW::workspace* all, std::shared_ptr<VW::rand_state> random_state, uint32_t leaf_split,
-    emt_scorer_type scorer_type, emt_router_type router_type, uint64_t tree_bound)
+    emt_scorer_type scorer_type, emt_router_type router_type, emt_initial_type initial_type, uint64_t tree_bound)
     : all(all)
     , random_state(std::move(random_state))
     , leaf_split(leaf_split)
     , scorer_type(scorer_type)
     , router_type(router_type)
+    , initial_type(initial_type)
 {
   bounder = VW::make_unique<VW::reductions::eigen_memory_tree::emt_lru>(tree_bound);
   root = VW::make_unique<emt_node>();
 
   // we set this up for repeated use later in the scorer.
   // we will populate this examples features over and over.
   ex = VW::make_unique<VW::example>();
@@ -159,29 +194,30 @@
     return (v1 + v2) / 2.;
   }
 
   std::nth_element(array.begin(), nth, array.end());
   return *nth;
 }
 
-float emt_inner(const emt_feats& xs, const emt_feats& ys)
+float emt_inner(const emt_feats& f1, const emt_feats& f2)
 {
   float sum = 0;
-  uint64_t xi = 0;
-  uint64_t yi = 0;
+  auto iter1 = f1.begin();
+  auto iter2 = f2.begin();
 
-  while (xi < xs.size() && yi < ys.size())
+  while (iter1 != f1.end() && iter2 != f2.end())
   {
-    auto x = xs[xi];
-    auto y = ys[yi];
-
-    if (x.first == y.first) { sum += x.second * y.second; }
-
-    if (x.first <= y.first) { xi += 1; }
-    if (y.first <= x.first) { yi += 1; }
+    if (iter1->first < iter2->first) { iter1++; }
+    else if (iter2->first < iter1->first) { iter2++; }
+    else
+    {
+      sum += iter1->second * iter2->second;
+      iter1++;
+      iter2++;
+    }
   }
 
   return sum;
 }
 
 float emt_norm(const emt_feats& xs)
 {
@@ -195,57 +231,155 @@
 void emt_scale(emt_feats& xs, float scalar)
 {
   for (auto& x : xs) { x.second *= scalar; }
 }
 
 void emt_normalize(emt_feats& xs) { emt_scale(xs, 1 / emt_norm(xs)); }
 
-void emt_abs(emt_feats& fs)
+emt_feats emt_sub(const emt_feats& f1, const emt_feats& f2)
 {
-  for (auto& f : fs) { f.second = std::abs(f.second); }
+  emt_feats out;
+  auto iter1 = f1.begin();
+  auto iter2 = f2.begin();
+
+  while (iter1 != f1.end() && iter2 != f2.end())
+  {
+    if (iter1->first < iter2->first)
+    {
+      out.emplace_back(iter1->first, iter1->second);
+      iter1++;
+    }
+    else if (iter2->first < iter1->first)
+    {
+      out.emplace_back(iter2->first, -iter2->second);
+      iter2++;
+    }
+    else
+    {
+      out.emplace_back(iter1->first, iter1->second - iter2->second);
+      iter1++;
+      iter2++;
+    }
+  }
+
+  while (iter1 != f1.end())
+  {
+    out.emplace_back(iter1->first, iter1->second);
+    iter1++;
+  }
+
+  while (iter2 != f2.end())
+  {
+    out.emplace_back(iter2->first, -iter2->second);
+    iter2++;
+  }
+
+  return out;
 }
 
-emt_feats emt_scale_add(float s1, const emt_feats& f1, float s2, const emt_feats& f2)
+emt_feats emt_scale_add(const emt_feats& f1, float s2, const emt_feats& f2)
 {
-  size_t idx1 = 0;
-  size_t idx2 = 0;
+  if (s2 == -1) { return emt_sub(f1, f2); }
 
-  uint64_t index = 0;
-  uint64_t f1_idx = 0;
-  uint64_t f2_idx = 0;
+  emt_feats out;
+  auto iter1 = f1.begin();
+  auto iter2 = f2.begin();
 
-  float f1_val = 0.f;
-  float f2_val = 0.f;
+  while (iter1 != f1.end() && iter2 != f2.end())
+  {
+    if (iter1->first < iter2->first)
+    {
+      out.emplace_back(iter1->first, iter1->second);
+      iter1++;
+    }
+    else if (iter2->first < iter1->first)
+    {
+      out.emplace_back(iter2->first, s2 * iter2->second);
+      iter2++;
+    }
+    else
+    {
+      out.emplace_back(iter1->first, iter1->second + s2 * iter2->second);
+      iter1++;
+      iter2++;
+    }
+  }
 
-  emt_feats out;
+  while (iter1 != f1.end())
+  {
+    out.emplace_back(iter1->first, iter1->second);
+    iter1++;
+  }
 
-  while (idx1 < f1.size() || idx2 < f2.size())
+  while (iter2 != f2.end())
   {
-    f1_idx = (idx1 == f1.size()) ? INT_MAX : f1[idx1].first;
-    f2_idx = (idx2 == f2.size()) ? INT_MAX : f2[idx2].first;
+    out.emplace_back(iter2->first, s2 * iter2->second);
+    iter2++;
+  }
+
+  return out;
+}
 
-    f1_val = 0.f;
-    f2_val = 0.f;
+void emt_scale_add2(emt_feats& f1, float s2, const emt_feats& f2)
+{
+  auto iter1 = f1.begin();
+  auto iter2 = f2.begin();
 
-    if (f1_idx <= f2_idx)
+  while (iter1 != f1.end() && iter2 != f2.end())
+  {
+    if (iter1->first < iter2->first) { iter1++; }
+    else
     {
-      index = f1_idx;
-      f1_val = f1[idx1].second;
-      idx1++;
+      iter1->second = iter1->second + s2 * iter2->second;
+      iter1++;
+      iter2++;
     }
+  }
+}
 
-    if (f2_idx <= f1_idx)
+emt_feats emt_scale_add(float s1, const emt_feats& f1, float s2, const emt_feats& f2)
+{
+  if (s1 == 1) { return emt_scale_add(f1, s2, f2); }
+
+  emt_feats out;
+  auto iter1 = f1.begin();
+  auto iter2 = f2.begin();
+
+  while (iter1 != f1.end() && iter2 != f2.end())
+  {
+    if (iter1->first < iter2->first)
+    {
+      out.emplace_back(iter1->first, s1 * iter1->second);
+      iter1++;
+    }
+    else if (iter2->first < iter1->first)
     {
-      index = f2_idx;
-      f2_val = f2[idx2].second;
-      idx2++;
+      out.emplace_back(iter2->first, s2 * iter2->second);
+      iter2++;
     }
+    else
+    {
+      out.emplace_back(iter1->first, s1 * iter1->second + s2 * iter2->second);
+      iter1++;
+      iter2++;
+    }
+  }
+
+  while (iter1 != f1.end())
+  {
+    out.emplace_back(iter1->first, s1 * iter1->second);
+    iter1++;
+  }
 
-    out.emplace_back(index, f1_val * s1 + f2_val * s2);
+  while (iter2 != f2.end())
+  {
+    out.emplace_back(iter2->first, s2 * iter2->second);
+    iter2++;
   }
+
   return out;
 }
 
 emt_feats emt_router_random(std::vector<emt_feats>& exs, VW::rand_state& rng)
 {
   std::set<int> is;
   emt_feats weights;
@@ -275,40 +409,40 @@
   for (auto& ex : exs)
   {
     for (auto& p : ex) { sums[p.first] += p.second; }
   }
   for (auto& p : sums) { means.emplace_back(p.first, p.second / exs.size()); }
 
   std::vector<emt_feats> centered_exs;
-  centered_exs.reserve(exs.size());
-  for (auto& e : exs) { centered_exs.push_back(emt_scale_add(1, e, -1, means)); }
+  for (auto& e : exs) { centered_exs.push_back(emt_sub(e, means)); }
 
   int n_epochs = 40;  // the bigger the better eigen approximation
+  int j = 0;
 
   for (int i = 0; i < n_epochs; i++)
   {
     // reseting n on each epoch gives
     // projectors that are substantially
     // closer to the true top eigen vector
     // in experiments
-    float n = 1;
+    int n = 1;
     emt_shuffle(centered_exs.begin(), centered_exs.end(), rng);
-
     for (const emt_feats& fs : centered_exs)
     {
       // in matrix multiplication notation this looks like:
       // weights = weights + (1/n) * inner(outer(fs,fs), weights)
       //         = weights + (1/n) * fs * inner(fs,weights)
       //         =          weights+(1/n)*inner(fs,weights)*fs
-      weights = emt_scale_add(1, weights, (1 / n) * emt_inner(fs, weights), fs);
-      emt_normalize(weights);
-      n += 1;
+      j++;
+      emt_scale_add2(weights, emt_inner(fs, weights) / n, fs);
+      if (j % 4 == 0) { emt_normalize(weights); }
+      n++;
     }
   }
-
+  emt_normalize(weights);
   return weights;
 }
 }  // namespace eigen_memory_tree
 }  // namespace reductions
 }  // namespace VW
 namespace
 {
@@ -351,50 +485,83 @@
     {
       cn.examples.erase(iter);
       return;
     }
   }
 }
 
-float scorer_initial(const float dist) { return 1 - std::exp(-dist); }
-
 void scorer_features(const emt_feats& f1, VW::features& out)
 {
-  out.clear();
   for (auto p : f1)
   {
     if (p.second != 0) { out.push_back(p.second, p.first); }
   }
 }
 
+void scorer_features(const emt_feats& f1, const emt_feats& f2, VW::features& out)
+{
+  auto iter1 = f1.begin();
+  auto iter2 = f2.begin();
+
+  while (iter1 != f1.end() && iter2 != f2.end())
+  {
+    if (iter1->first < iter2->first)
+    {
+      if (iter1->second != 0) { out.push_back(iter1->second, iter1->first); }
+      iter1++;
+    }
+    else if (iter2->first < iter1->first)
+    {
+      if (iter2->second != 0) { out.push_back(iter2->second, iter2->first); }
+      iter2++;
+    }
+    else
+    {
+      if (iter1->second != iter2->second) { out.push_back(std::abs(iter1->second - iter2->second), iter1->first); }
+      iter1++;
+      iter2++;
+    }
+  }
+
+  while (iter1 != f1.end())
+  {
+    if (iter1->second != 0) { out.push_back(std::abs(iter1->second), iter1->first); }
+    iter1++;
+  }
+
+  while (iter2 != f2.end())
+  {
+    if (iter2->second != 0) { out.push_back(std::abs(iter2->second), iter2->first); }
+    iter2++;
+  }
+}
+
 void scorer_example(emt_tree& b, const emt_example& ex1, const emt_example& ex2)
 {
   VW::example& out = *b.ex;
 
   static constexpr VW::namespace_index X_NS = 'x';
   static constexpr VW::namespace_index Z_NS = 'z';
 
+  out.feature_space[X_NS].clear();
+  out.feature_space[Z_NS].clear();
+
   if (b.scorer_type == emt_scorer_type::SELF_CONSISTENT_RANK)
   {
     out.indices.clear();
     out.indices.push_back(X_NS);
 
     out.interactions->clear();
 
-    out.feature_space[X_NS].clear();
-    out.feature_space[Z_NS].clear();
-
-    emt_feats feat_diff = emt_scale_add(1, ex1.full, -1, ex2.full);
-    emt_abs(feat_diff);
-    scorer_features(feat_diff, out.feature_space[X_NS]);
+    scorer_features(ex1.full, ex2.full, out.feature_space[X_NS]);
 
     out.total_sum_feat_sq = out.feature_space[X_NS].sum_feat_sq;
     out.num_features = out.feature_space[X_NS].size();
 
-    auto initial = scorer_initial(std::sqrt(out.total_sum_feat_sq));
+    auto initial = emt_initial(b.initial_type, ex1.full, ex2.full);
     out.ex_reduction_features.get<VW::simple_label_reduction_features>().initial = initial;
   }
 
   if (b.scorer_type == emt_scorer_type::NOT_SELF_CONSISTENT_RANK)
   {
     out.indices.clear();
     out.indices.push_back(X_NS);
@@ -415,15 +582,15 @@
     // we apply a map of multiplying by 2 and then offseting by 1 on the second example.
     for (auto& j : out.feature_space[X_NS].indices) { j = j * 2; }
     for (auto& j : out.feature_space[Z_NS].indices) { j = j * 2 + 1; }
 
     out.total_sum_feat_sq = out.feature_space[X_NS].sum_feat_sq + out.feature_space[Z_NS].sum_feat_sq;
     out.num_features = out.feature_space[X_NS].size() + out.feature_space[Z_NS].size();
 
-    auto initial = scorer_initial(emt_norm(emt_scale_add(1, ex1.full, -1, ex2.full)));
+    auto initial = emt_initial(b.initial_type, ex1.full, ex2.full);
     out.ex_reduction_features.get<VW::simple_label_reduction_features>().initial = initial;
   }
 
   // We cache metadata about model weights adjacent to them. For example if we have
   // a model weight w[i] then we may also store information about our confidence in
   // w[i] at w[i+1] and information about the scale of feature f[i] at w[i+2] and so on.
   // This variable indicates how many such meta-data places we need to save in between actual weights.
@@ -448,18 +615,19 @@
   if (b.scorer_type == emt_scorer_type::RANDOM)  // random scorer
   {
     return b.random_state->get_and_update_random();
   }
 
   if (b.scorer_type == emt_scorer_type::DISTANCE)  // dist scorer
   {
-    return emt_norm(emt_scale_add(1, pred_ex.full, -1, leaf_ex.full));
+    return emt_initial(b.initial_type, pred_ex.full, leaf_ex.full);
   }
 
   // The features matched exactly. Return max negative to make sure it is picked.
+  // Do I want this here? It doesn't seem to matter on experimental datasets.
   if (pred_ex.full == leaf_ex.full) { return -FLT_MAX; }
 
   scorer_example(b, pred_ex, leaf_ex);
   b.ex->l.simple = {FLT_MAX};
   base.predict(*b.ex);
 
   return b.ex->pred.scalar;
@@ -474,55 +642,59 @@
     ex.weight = weight;
     base.learn(ex);
   }
 }
 
 void scorer_learn(emt_tree& b, learner& base, emt_node& cn, const emt_example& ex, float weight)
 {
-  // random and dist scorer has nothing to learsn
+  // random and dist scorer has nothing to learn
   if (b.scorer_type == emt_scorer_type::RANDOM || b.scorer_type == emt_scorer_type::DISTANCE) { return; }
 
   if (weight == 0) { return; }
   if (cn.examples.size() < 2) { return; }
 
   // shuffle the examples to break ties randomly
   emt_shuffle(cn.examples.begin(), cn.examples.end(), *b.random_state);
 
   float preferred_score = FLT_MAX;
   float preferred_error = FLT_MAX;
   emt_example* preferred_ex = nullptr;
 
+  float alternative_score = FLT_MAX;
   float alternative_error = FLT_MAX;
   emt_example* alternative_ex = nullptr;
 
-  for (auto& example : cn.examples)
-  {
-    float score = scorer_predict(b, base, ex, *example);
+  std::vector<float> scores;
+  for (auto& example : cn.examples) { scores.push_back(scorer_predict(b, base, ex, *example)); }
 
-    if (score < preferred_score)
+  // double loop has time complexity of 2n which is almost always faster than a sort with n*log(n)
+  for (size_t i = 0; i < cn.examples.size(); i++)
+  {
+    if (scores[i] < preferred_score)
     {
-      preferred_score = score;
-      preferred_ex = example.get();
-      preferred_error = (example->label == ex.label) ? 0.f : 1.f;
+      preferred_score = scores[i];
+      preferred_ex = cn.examples[i].get();
+      preferred_error = (preferred_ex->label == ex.label) ? 0.f : 1.f;
     }
   }
 
-  for (auto& example : cn.examples)
+  for (size_t i = 0; i < cn.examples.size(); i++)
   {
-    if (example.get() == preferred_ex) { continue; }
+    if (cn.examples[i].get() == preferred_ex) { continue; }
+    float error = (cn.examples[i].get()->label == ex.label) ? 0.f : 1.f;
 
-    float error = (example->label == ex.label) ? 0.f : 1.f;
-    if (error < alternative_error)
+    if ((error < alternative_error) || (error == alternative_error && scores[i] < alternative_score))
     {
+      alternative_score = scores[i];
+      alternative_ex = cn.examples[i].get();
       alternative_error = error;
-      alternative_ex = example.get();
     }
   }
 
-  // the better of the two options moves towards 0 while the other moves towards -1
+  // the better of the two options moves towards 0 while the other moves towards 1
   weight *= std::abs(preferred_error - alternative_error);
 
   if (alternative_ex == nullptr || preferred_ex == nullptr)
   {
     *(b.all->output_runtime.trace_message) << "ERROR" << std::endl;
     return;
   }
@@ -541,26 +713,14 @@
     {
       scorer_example(b, ex, *alternative_ex);
       scorer_learn(base, *b.ex, int(alternative_error > preferred_error), weight);
 
       scorer_example(b, ex, *preferred_ex);
       scorer_learn(base, *b.ex, int(preferred_error > alternative_error), weight);
     }
-
-    // this trick gives worse outcomes. Why? It is faster so it'd be nice if it didn't.
-    // scorer_example(ex, *preferred_ex, b.ex[0]);
-    // scorer_example(ex, *alternative_ex, b.ex[1]);
-    // scorer_features(b.ex[0].feature_space[0], b.ex[1].feature_space[0], b.ex[2].feature_space[0], 2);
-
-    // b.ex[2].total_sum_feat_sq = b.ex[2].feature_space[0].sum_feat_sq;
-    // b.ex[2].num_features = b.ex[2].feature_space[0].size();
-
-    // float label = (preferred_reward < alternative_reward) ? 1.f : -1.f;
-    // float initial = scorer_initial(b.ex[0]) - scorer_initial(b.ex[1]);
-    // scorer_learn(b, base, b.ex[2], label, 1.5*weight, initial);
   }
 }
 
 void node_split(emt_tree& b, emt_node& cn)
 {
   if (cn.examples.size() <= b.leaf_split) { return; }
 
@@ -635,15 +795,14 @@
 {
   b.all->feature_tweaks_config.ignore_some_linear = false;
   auto ex = VW::make_unique<emt_example>(*b.all, &ec);
 
   emt_node& cn = *tree_route(b, *ex);
   scorer_learn(b, base, cn, *ex, ec.weight);
   node_predict(b, base, cn, *ex, ec);  // vw learners predict and emt_learn
-
   tree_bound(b, ex.get());
   node_insert(cn, std::move(ex));
   node_split(b, cn);
 }
 
 #ifdef VW_ENABLE_EMT_DEBUG_TIMER
 void emt_end_pass_timer(emt_tree& b)
@@ -761,14 +920,15 @@
 {
   options_i& options = *stack_builder.get_options();
   VW::workspace& all = *stack_builder.get_all_pointer();
 
   bool enabled{};
   std::string scorer_type;
   std::string router_type;
+  std::string initial_type;
   uint32_t tree_bound = 0;
   uint32_t leaf_split = 0;
 
   option_group_definition new_options("[Reduction] Eigen Memory Tree");
   new_options.add(make_option("emt", enabled).keep().necessary().help("Make an eigen memory tree"))
       .add(make_option("emt_tree", tree_bound)
                .keep()
@@ -779,24 +939,38 @@
                .default_value(100)
                .help("Indicates the maximum number of memories a leaf can have"))
       .add(make_option("emt_scorer", scorer_type)
                .keep()
                .one_of({"random", "distance", "self_consistent_rank", "not_self_consistent_rank"})
                .default_value("self_consistent_rank")
                .help("Indicates the type of scorer to use"))
+      .add(make_option("emt_initial", initial_type)
+               .keep()
+               .one_of({"gaussian", "cosine", "euclidean", "none"})
+               .default_value("cosine")
+               .help("Indicates how to initialize scorer"))
       .add(make_option("emt_router", router_type)
                .keep()
                .one_of({"random", "eigen"})
                .default_value("eigen")
                .help("Indicates the type of router to use"));
 
   if (!options.add_parse_and_check_necessary(new_options)) { return nullptr; }
 
+  // The EMT scorer, when it is learning, will only ever see 0's and 1's.
+  // Therefore, VW's native min/max will be 0/1 unless we explicitly make it larger.
+  if (all.sd->min_label == 0 && all.sd->max_label == 0)
+  {
+    all.sd->min_label = 0;
+    all.sd->max_label = 3;
+  }
+
   auto t = VW::make_unique<VW::reductions::eigen_memory_tree::emt_tree>(&all, all.get_random_state(), leaf_split,
-      emt_scorer_type_from_string(scorer_type), emt_router_type_from_string(router_type), tree_bound);
+      emt_scorer_type_from_string(scorer_type), emt_router_type_from_string(router_type),
+      emt_initial_type_from_string(initial_type), tree_bound);
 
   auto l =
       make_reduction_learner(std::move(t), require_singleline(stack_builder.setup_base_learner()), emt_learn,
           emt_predict,
           stack_builder.get_setupfn_name(eigen_memory_tree_setup))
           .set_learn_returns_prediction(true)  // we set this to true otherwise bounding doesn't work as well
 #ifdef VW_ENABLE_EMT_DEBUG_TIMER
```

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/epsilon_decay.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/epsilon_decay.cc`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 // Copyright (c) by respective owners including Yahoo!, Microsoft, and
 // individual contributors. All rights reserved. Released under a BSD (revised)
 // license as described in the file LICENSE.
 
 #include "vw/core/reductions/epsilon_decay.h"
 
 #include "vw/config/options.h"
-#include "vw/core/estimators/distributionally_robust.h"
 #include "vw/core/global_data.h"
 #include "vw/core/label_type.h"
 #include "vw/core/learner.h"
 #include "vw/core/memory.h"
 #include "vw/core/model_utils.h"
 #include "vw/core/multi_model_utils.h"
 #include "vw/core/prediction_type.h"
@@ -36,28 +35,29 @@
   return init_ep * static_cast<float>(std::pow(update_count + 1, -1.f / 3.f));
 }
 
 epsilon_decay_data::epsilon_decay_data(uint64_t model_count, uint64_t min_scope,
     double epsilon_decay_significance_level, double epsilon_decay_estimator_decay, dense_parameters& weights,
     std::string epsilon_decay_audit_str, bool constant_epsilon, uint32_t& feature_width, uint64_t min_champ_examples,
     float initial_epsilon, uint64_t shift_model_bounds, bool reward_as_cost, double tol_x, bool is_brentq,
-    bool predict_only_model)
+    bool predict_only_model, bool challenger_epsilon)
     : _model_count(model_count)
     , _min_scope(min_scope)
     , _epsilon_decay_significance_level(epsilon_decay_significance_level)
     , _epsilon_decay_estimator_decay(epsilon_decay_estimator_decay)
     , _weights(weights)
     , _epsilon_decay_audit_str(std::move(epsilon_decay_audit_str))
     , _constant_epsilon(constant_epsilon)
     , _feature_width(feature_width)
     , _min_champ_examples(min_champ_examples)
     , _initial_epsilon(initial_epsilon)
     , _shift_model_bounds(shift_model_bounds)
     , _reward_as_cost(reward_as_cost)
     , _predict_only_model(predict_only_model)
+    , _challenger_epsilon(challenger_epsilon)
 {
   _weight_indices.resize(model_count);
   conf_seq_estimators.reserve(model_count);
   std::iota(_weight_indices.begin(), _weight_indices.end(), 0);
   for (uint64_t i = 0; i < model_count; ++i)
   {
     conf_seq_estimators.emplace_back();
@@ -102,27 +102,43 @@
       if (!base.learn_returns_prediction) { base.predict(examples, _weight_indices[model_ind]); }
       base.learn(examples, _weight_indices[model_ind]);
 
       for (const auto& a_s : examples[0]->pred.a_s)
       {
         if (a_s.action == labelled_action)
         {
-          float w = (logged.probability > 0) ? a_s.score / logged.probability : 0;
+          float p_pred = a_s.score;
+          if (model_ind != model_count - 1 && !_challenger_epsilon)
+          {
+            // Get best action
+            uint32_t best_action = 0;
+            float best_score = 0.f;
+            for (const auto& a_s : examples[0]->pred.a_s)
+            {
+              if (a_s.score > best_score)
+              {
+                best_action = a_s.action;
+                best_score = a_s.score;
+              }
+            }
+            p_pred = (a_s.action == best_action) ? 1.f : 0.f;
+          }
+          float w = (logged.probability > 0) ? p_pred / logged.probability : 0;
           for (int64_t estimator_ind = 0; estimator_ind <= model_ind; ++estimator_ind)
           {
             conf_seq_estimators[model_ind][estimator_ind].update(w, r);
           }
           if (_epsilon_decay_audit_str != "")
           {
             if (model_ind != model_count - 1) { _audit_msg << "challenger[" << (model_ind + 1) << "] "; }
             else { _audit_msg << "champ "; }
             _audit_msg << "update_count: " << conf_seq_estimators[model_ind][model_ind].update_count
                        << " lb: " << conf_seq_estimators[model_ind][model_ind].lower_bound()
                        << " champ_ub: " << conf_seq_estimators[model_count - 1][model_ind].upper_bound()
-                       << " p_pred: " << a_s.score << "\n";
+                       << " p_pred: " << p_pred << "\n";
           }
           break;
         }
       }
       if (model_ind == model_count - 1) { champ_a_s = examples[0]->pred.a_s; }
     }
     examples[0]->pred.a_s = champ_a_s;
@@ -226,24 +242,27 @@
 
 namespace model_utils
 {
 size_t read_model_field(io_buf& io, VW::reductions::epsilon_decay::epsilon_decay_data& epsilon_decay)
 {
   size_t bytes = 0;
   epsilon_decay.conf_seq_estimators.clear();
+  epsilon_decay._weight_indices.clear();
   bytes += read_model_field(io, epsilon_decay.conf_seq_estimators);
+  bytes += read_model_field(io, epsilon_decay._weight_indices);
   bytes += read_model_field(io, epsilon_decay._global_counter);
   return bytes;
 }
 
 size_t write_model_field(io_buf& io, const VW::reductions::epsilon_decay::epsilon_decay_data& epsilon_decay,
     const std::string& upstream_name, bool text)
 {
   size_t bytes = 0;
   bytes += write_model_field(io, epsilon_decay.conf_seq_estimators, upstream_name + "conf_seq_estimators", text);
+  bytes += write_model_field(io, epsilon_decay._weight_indices, upstream_name + "_weight_indices", text);
   bytes += write_model_field(io, epsilon_decay._global_counter, upstream_name + "_global_counter", text);
   return bytes;
 }
 }  // namespace model_utils
 }  // namespace VW
 
 namespace
@@ -325,21 +344,22 @@
   bool epsilon_decay_option;
   uint64_t model_count;
   uint64_t min_scope;
   float epsilon_decay_significance_level;
   float epsilon_decay_estimator_decay;
   std::string epsilon_decay_audit_str;
   bool constant_epsilon = false;
-  bool fixed_significance_level = false;
+  uint64_t bonferroni_denominator;
   uint64_t min_champ_examples;
   float initial_epsilon;
   uint64_t shift_model_bounds;
   bool reward_as_cost;
   float tol_x;
   std::string opt_func = "bisect";
+  bool challenger_epsilon = false;
 
   option_group_definition new_options("[Reduction] Epsilon-Decaying Exploration");
   new_options
       .add(make_option("epsilon_decay", epsilon_decay_option)
                .necessary()
                .keep()
                .help("Use decay of exploration reduction")
@@ -352,33 +372,29 @@
       .add(make_option("min_scope", min_scope)
                .keep()
                .default_value(100)
                .help("Minimum example count of model before removing")
                .experimental())
       .add(make_option("epsilon_decay_significance_level", epsilon_decay_significance_level)
                .keep()
-               .default_value(VW::details::DEFAULT_ALPHA)
+               .default_value(VW::details::CS_ROBUST_DEFAULT_ALPHA)
                .help("Set significance level for champion change")
                .experimental())
-      .add(make_option("epsilon_decay_estimator_decay", epsilon_decay_estimator_decay)
-               .keep()
-               .default_value(VW::details::CRESSEREAD_DEFAULT_TAU)
-               .help("Time constant for count decay")
-               .experimental())
       .add(make_option("epsilon_decay_audit", epsilon_decay_audit_str)
                .default_value("")
                .help("Epsilon decay audit file name")
                .experimental())
       .add(make_option("constant_epsilon", constant_epsilon)
                .keep()
                .help("Keep epsilon constant across models")
                .experimental())
-      .add(make_option("fixed_significance_level", fixed_significance_level)
+      .add(make_option("bonferroni_denominator", bonferroni_denominator)
+               .default_value(0)
                .keep()
-               .help("Use fixed significance level as opposed to scaling by model count (bonferroni correction)")
+               .help("Factor to scale down significance level by, defaults to model count (bonferroni correction)")
                .experimental())
       .add(make_option("min_champ_examples", min_champ_examples)
                .default_value(0)
                .keep()
                .help("Minimum number of examples for any challenger to become champion")
                .experimental())
       .add(make_option("initial_epsilon", initial_epsilon)
@@ -401,30 +417,35 @@
                .keep()
                .help("Tolerance for estimation optimization")
                .experimental())
       .add(make_option("opt_func", opt_func)
                .default_value("bisect")
                .keep()
                .one_of({"bisect", "brentq"})
-               .help("Optimization function for estimation)")
+               .help("Optimization function for estimation")
+               .experimental())
+      .add(make_option("challenger_epsilon", challenger_epsilon)
+               .keep()
+               .help("Use exploration for challenger model predictions")
                .experimental());
 
   if (!options.add_parse_and_check_necessary(new_options)) { return nullptr; }
 
   if (model_count < 1) { THROW("Model count must be 1 or greater"); }
 
-  if (!fixed_significance_level) { epsilon_decay_significance_level /= model_count; }
+  if (bonferroni_denominator == 0) { bonferroni_denominator = model_count; }
+  epsilon_decay_significance_level /= bonferroni_denominator;
 
   bool predict_only_model = options.was_supplied("predict_only_model");
   bool is_brentq = opt_func == "brentq";
 
   auto data = VW::make_unique<VW::reductions::epsilon_decay::epsilon_decay_data>(model_count, min_scope,
       epsilon_decay_significance_level, epsilon_decay_estimator_decay, all.weights.dense_weights,
       epsilon_decay_audit_str, constant_epsilon, all.reduction_state.total_feature_width, min_champ_examples,
-      initial_epsilon, shift_model_bounds, reward_as_cost, tol_x, is_brentq, predict_only_model);
+      initial_epsilon, shift_model_bounds, reward_as_cost, tol_x, is_brentq, predict_only_model, challenger_epsilon);
 
   // make sure we setup the rest of the stack with cleared interactions
   // to make sure there are not subtle bugs
   auto base = stack_builder.setup_base_learner(model_count);
 
   if (base->is_multiline())
   {
```

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/explore_eval.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/explore_eval.cc`

 * *Files 4% similar despite different names*

```diff
@@ -281,14 +281,21 @@
         for (auto& ec : ec_seq) { ec->weight *= inv_threshold; }
       }
 
       ec_found->l.cb.costs[0].probability = data.known_cost.probability;
     }
   }
 }
+
+void persist(explore_eval& data, VW::metric_sink& metrics)
+{
+  metrics.set_float("weighted_update_count", data.weighted_update_count);
+  metrics.set_float(
+      "average_accepted_example_weight", data.weighted_update_count / static_cast<float>(data.update_count));
+}
 }  // namespace
 
 std::shared_ptr<VW::LEARNER::learner> VW::reductions::explore_eval_setup(VW::setup_base_i& stack_builder)
 {
   options_i& options = *stack_builder.get_options();
   VW::workspace& all = *stack_builder.get_all_pointer();
   auto data = VW::make_unique<explore_eval>();
@@ -326,12 +333,13 @@
                .set_input_prediction_type(VW::prediction_type_t::ACTION_PROBS)
                .set_output_prediction_type(VW::prediction_type_t::ACTION_PROBS)
                .set_input_label_type(VW::label_type_t::CB)
                .set_output_label_type(VW::label_type_t::CB)
                .set_update_stats(update_stats_explore_eval)
                .set_output_example_prediction(output_example_prediction_explore_eval)
                .set_print_update(print_update_explore_eval)
+               .set_persist_metrics(::persist)
                .set_finish(::finish)
                .build();
 
   return l;
 }
```

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/freegrad.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/freegrad.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/ftrl.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/ftrl.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/gd.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/gd.cc`

 * *Files 1% similar despite different names*

```diff
@@ -1051,56 +1051,59 @@
           if (map_it != all.output_runtime.index_name_map.end()) { msg << to_string(map_it->second) << ":"; }
         }
       }
 
       if (ftrl3_write)
       {
         brw = write_index(model_file, msg, text, all.initial_weights_config.num_bits, i);
-        msg << ":" << *v << " " << (&(*v))[1] << " " << (&(*v))[2] << "\n";
+        if (text) { msg << ":" << *v << " " << (&(*v))[1] << " " << (&(*v))[2] << "\n"; }
         brw += VW::details::bin_text_write_fixed(model_file, (char*)&(*v), 3 * sizeof(*v), msg, text);
       }
       else if (ftrl4_write)
       {
         brw = write_index(model_file, msg, text, all.initial_weights_config.num_bits, i);
-        msg << ":" << *v << " " << (&(*v))[1] << " " << (&(*v))[2] << " " << (&(*v))[3] << "\n";
+        if (text) { msg << ":" << *v << " " << (&(*v))[1] << " " << (&(*v))[2] << " " << (&(*v))[3] << "\n"; }
         brw += VW::details::bin_text_write_fixed(model_file, (char*)&(*v), 4 * sizeof(*v), msg, text);
       }
       else if (ftrl6_write)
       {
         brw = write_index(model_file, msg, text, all.initial_weights_config.num_bits, i);
-        msg << ":" << *v << " " << (&(*v))[1] << " " << (&(*v))[2] << " " << (&(*v))[3] << " " << (&(*v))[4] << " "
-            << (&(*v))[5] << "\n";
+        if (text)
+        {
+          msg << ":" << *v << " " << (&(*v))[1] << " " << (&(*v))[2] << " " << (&(*v))[3] << " " << (&(*v))[4] << " "
+              << (&(*v))[5] << "\n";
+        }
         brw += VW::details::bin_text_write_fixed(model_file, (char*)&(*v), 6 * sizeof(*v), msg, text);
       }
       else if (g == nullptr || (!all.weights.adaptive && !all.weights.normalized))
       {
         if (*v != 0.)
         {
           brw = write_index(model_file, msg, text, all.initial_weights_config.num_bits, i);
-          msg << ":" << *v << "\n";
+          if (text) { msg << ":" << *v << "\n"; }
           brw += VW::details::bin_text_write_fixed(model_file, (char*)&(*v), sizeof(*v), msg, text);
         }
       }
       else if ((all.weights.adaptive && !all.weights.normalized) || (!all.weights.adaptive && all.weights.normalized))
       {
         // either adaptive or normalized
         if (*v != 0. || (&(*v))[1] != 0.)
         {
           brw = write_index(model_file, msg, text, all.initial_weights_config.num_bits, i);
-          msg << ":" << *v << " " << (&(*v))[1] << "\n";
+          if (text) { msg << ":" << *v << " " << (&(*v))[1] << "\n"; }
           brw += VW::details::bin_text_write_fixed(model_file, (char*)&(*v), 2 * sizeof(*v), msg, text);
         }
       }
       else
       {
         // adaptive and normalized
         if (*v != 0. || (&(*v))[1] != 0. || (&(*v))[2] != 0.)
         {
           brw = write_index(model_file, msg, text, all.initial_weights_config.num_bits, i);
-          msg << ":" << *v << " " << (&(*v))[1] << " " << (&(*v))[2] << "\n";
+          if (text) { msg << ":" << *v << " " << (&(*v))[1] << " " << (&(*v))[2] << "\n"; }
           brw += VW::details::bin_text_write_fixed(model_file, (char*)&(*v), 3 * sizeof(*v), msg, text);
         }
       }
     }
   }
 }
 }  // namespace
@@ -1111,17 +1114,29 @@
   std::stringstream msg;
 
   msg << "initial_t " << all.update_rule_config.initial_t << "\n";
   VW::details::bin_text_read_write_fixed(model_file, reinterpret_cast<char*>(&all.update_rule_config.initial_t),
       sizeof(all.update_rule_config.initial_t), read, msg, text);
 
   assert(pms.size() >= 1);
-  msg << "norm normalizer " << pms[0].normalized_sum_norm_x << "\n";
-  VW::details::bin_text_read_write_fixed(model_file, reinterpret_cast<char*>(&pms[0].normalized_sum_norm_x),
-      sizeof(pms[0].normalized_sum_norm_x), read, msg, text);
+  if (g != nullptr && g->per_model_save_load)
+  {
+    for (size_t ind = 0; ind < pms.size(); ++ind)
+    {
+      msg << "norm normalizer_" << ind << " " << pms[ind].normalized_sum_norm_x << "\n";
+      VW::details::bin_text_read_write_fixed(model_file, reinterpret_cast<char*>(&pms[ind].normalized_sum_norm_x),
+          sizeof(pms[ind].normalized_sum_norm_x), read, msg, text);
+    }
+  }
+  else
+  {
+    msg << "norm normalizer " << pms[0].normalized_sum_norm_x << "\n";
+    VW::details::bin_text_read_write_fixed(model_file, reinterpret_cast<char*>(&pms[0].normalized_sum_norm_x),
+        sizeof(pms[0].normalized_sum_norm_x), read, msg, text);
+  }
 
   msg << "t " << all.sd->t << "\n";
   VW::details::bin_text_read_write_fixed(
       model_file, reinterpret_cast<char*>(&all.sd->t), sizeof(all.sd->t), read, msg, text);
 
   msg << "sum_loss " << all.sd->sum_loss << "\n";
   VW::details::bin_text_read_write_fixed(
@@ -1170,17 +1185,29 @@
 
   if (!read || all.runtime_state.model_file_ver >= VW::version_definitions::VERSION_SAVE_RESUME_FIX)
   {
     assert(pms.size() >= 1);
     // restore some data to allow save_resume work more accurate
 
     // fix average loss
-    msg << "total_weight " << pms[0].total_weight << "\n";
-    VW::details::bin_text_read_write_fixed(
-        model_file, reinterpret_cast<char*>(&pms[0].total_weight), sizeof(pms[0].total_weight), read, msg, text);
+    if (g != nullptr && g->per_model_save_load)
+    {
+      for (size_t ind = 0; ind < pms.size(); ++ind)
+      {
+        msg << "total_weight_" << ind << " " << pms[ind].total_weight << "\n";
+        VW::details::bin_text_read_write_fixed(model_file, reinterpret_cast<char*>(&pms[ind].total_weight),
+            sizeof(pms[ind].total_weight), read, msg, text);
+      }
+    }
+    else
+    {
+      msg << "total_weight " << pms[0].total_weight << "\n";
+      VW::details::bin_text_read_write_fixed(
+          model_file, reinterpret_cast<char*>(&pms[0].total_weight), sizeof(pms[0].total_weight), read, msg, text);
+    }
 
     // fix "loss since last" for first printed out example details
     msg << "sd::oec.weighted_labeled_examples " << all.sd->old_weighted_labeled_examples << "\n";
     VW::details::bin_text_read_write_fixed(model_file, reinterpret_cast<char*>(&all.sd->old_weighted_labeled_examples),
         sizeof(all.sd->old_weighted_labeled_examples), read, msg, text);
 
     // fix "number of examples per pass"
@@ -1431,14 +1458,15 @@
   bool normalized = false;
   float sparse_l2 = 0.f;
 
   all.sd->gravity = L1_STATE_DEFAULT;
   all.sd->contraction = L2_STATE_DEFAULT;
   float local_gravity = 0;
   float local_contraction = 0;
+  bool per_model_save_load = false;
 
   option_group_definition new_options("[Reduction] Gradient Descent");
   new_options
       .add(make_option("sgd", sgd)
                .help("Use regular stochastic gradient descent update")
                .keep(all.output_model_config.save_resume))
       .add(make_option("adaptive", adaptive)
@@ -1457,28 +1485,33 @@
       .add(make_option("l1_state", local_gravity)
                .allow_override()
                .default_value(L1_STATE_DEFAULT)
                .help("Amount of accumulated implicit l1 regularization"))
       .add(make_option("l2_state", local_contraction)
                .allow_override()
                .default_value(L2_STATE_DEFAULT)
-               .help("Amount of accumulated implicit l2 regularization"));
+               .help("Amount of accumulated implicit l2 regularization"))
+      .add(make_option("per_model_save_load", per_model_save_load)
+               .keep()
+               .allow_override()
+               .help("Save and load per model state"));
   options.add_and_parse(new_options);
 
   if (options.was_supplied("l1_state")) { all.sd->gravity = local_gravity; }
   if (options.was_supplied("l2_state")) { all.sd->contraction = local_contraction; }
   all.weights.adaptive = true;
   all.weights.normalized = true;
 
   auto g = VW::make_unique<VW::reductions::gd>(feature_width_above);
   g->all = &all;
   g->no_win_counter = 0;
   g->neg_norm_power = (all.weights.adaptive ? (all.update_rule_config.power_t - 1.f) : -1.f);
   g->neg_power_t = -all.update_rule_config.power_t;
   g->sparse_l2 = sparse_l2;
+  g->per_model_save_load = per_model_save_load;
 
   if (all.update_rule_config.initial_t >
       0)  // for the normalized update: if initial_t is bigger than 1 we interpret this as if we had
           // seen (all.update_rule_config.initial_t) previous fake datapoints all with norm 1
   {
     g->gd_per_model_states[0].normalized_sum_norm_x = all.update_rule_config.initial_t;
     g->gd_per_model_states[0].total_weight = all.update_rule_config.initial_t;
```

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/gd_mf.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/gd_mf.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/generate_interactions.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/generate_interactions.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/get_pmf.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/get_pmf.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/interact.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/interact.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/interaction_ground.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/interaction_ground.cc`

 * *Files 12% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 #include "vw/common/vw_exception.h"
 #include "vw/config/options.h"
 #include "vw/config/options_cli.h"
 #include "vw/core/constant.h"
 #include "vw/core/label_dictionary.h"
 #include "vw/core/label_parser.h"
 #include "vw/core/loss_functions.h"
+#include "vw/core/multi_model_utils.h"
 #include "vw/core/parse_primitives.h"
 #include "vw/core/prediction_type.h"
 #include "vw/core/print_utils.h"
 #include "vw/core/reductions/cb/cb_adf.h"
 #include "vw/core/setup_base.h"
 #include "vw/core/shared_data.h"
 #include "vw/core/simple_label.h"
@@ -24,25 +25,30 @@
 using namespace VW::config;
 using namespace VW::reductions;
 
 namespace VW
 {
 namespace reductions
 {
+namespace igl
+{
+igl_data::igl_data(bool predict_only_model) : _predict_only_model(predict_only_model) {}
+}  // namespace igl
+
 namespace model_utils
 {
 size_t write_model_field(
-    io_buf& io, const VW::reductions::interaction_ground_data& igl, const std::string& upstream_name, bool text)
+    io_buf& io, const VW::reductions::igl::igl_data& igl, const std::string& upstream_name, bool text)
 {
   size_t bytes = 0;
   bytes += write_model_field(io, *igl.pi_ftrl.get(), upstream_name + ".pi", text);
   return bytes;
 }
 
-size_t read_model_field(io_buf& io, VW::reductions::interaction_ground_data& igl)
+size_t read_model_field(io_buf& io, VW::reductions::igl::igl_data& igl)
 {
   size_t bytes = 0;
   bytes += read_model_field(io, *igl.pi_ftrl.get());
   return bytes;
 }
 }  // namespace model_utils
 }  // namespace reductions
@@ -112,15 +118,15 @@
 
       ik_ex.feature_space[obs_ns].indices.push_back(feature_hash);
       ik_ex.feature_space[obs_ns].values.push_back(feature_val);
     }
   }
 }
 
-void learn(VW::reductions::interaction_ground_data& igl, learner& base, VW::multi_ex& ec_seq)
+void learn(VW::reductions::igl::igl_data& igl, learner& base, VW::multi_ex& ec_seq)
 {
   float p_unlabeled_prior = 0.5f;
 
   std::swap(igl.ik_ftrl->all->loss_config.loss, igl.ik_all->loss_config.loss);
   std::swap(igl.ik_ftrl->all->sd, igl.ik_all->sd);
 
   float ik_pred = 0.f;
@@ -140,15 +146,16 @@
   }
 
   auto ik_interactions = get_ik_interactions(igl.interactions, *observation_ex);
 
   for (size_t i = 0; i < ec_seq.size(); i++)
   {
     auto action_ex = ec_seq[i];
-    VW::empty_example(*igl.ik_all, igl.ik_ex);
+    VW::empty_example(*igl.ik_ftrl->all, igl.ik_ex);
+
     // TODO: Do we need constant feature here? If so, VW::add_constant_feature
     VW::details::append_example_namespaces_from_example(igl.ik_ex, *action_ex);
 
     add_obs_features_to_ik_ex(igl.ik_ex, *observation_ex);
     // 1. set up ik ex
     igl.ik_ex.l.simple.label = i == chosen_action_idx ? 1.f : -1.f;
 
@@ -203,15 +210,15 @@
     ex->l.cb_with_observations.event = ex->l.cb;
     ex->l.cb.reset_to_default();
   }
 
   ec_seq.push_back(observation_ex);
 }
 
-void predict(VW::reductions::interaction_ground_data& igl, learner& base, VW::multi_ex& ec_seq)
+void predict(VW::reductions::igl::igl_data& igl, learner& base, VW::multi_ex& ec_seq)
 {
   VW::example* observation_ex = nullptr;
 
   if (ec_seq.size() > 0 && ec_seq.back()->l.cb_with_observations.is_observation)
   {
     observation_ex = ec_seq.back();
     ec_seq.pop_back();
@@ -233,51 +240,78 @@
     ex->l.cb_with_observations.event = ex->l.cb;
     ex->l.cb.reset_to_default();
   }
 
   if (observation_ex != nullptr) { ec_seq.push_back(observation_ex); }
 }
 
-void save_load_igl(VW::reductions::interaction_ground_data& igl, VW::io_buf& io, bool read, bool text)
+void save_load_igl(VW::reductions::igl::igl_data& igl, VW::io_buf& io, bool read, bool text)
 {
   if (io.num_files() == 0) { return; }
   if (read) { VW::reductions::model_utils::read_model_field(io, igl); }
-  else { VW::reductions::model_utils::write_model_field(io, igl, "igl", text); }
+  else if (!igl._predict_only_model) { VW::reductions::model_utils::write_model_field(io, igl, "igl", text); }
 }
 
-void print_update_igl(VW::workspace& all, VW::shared_data& /*sd*/, const VW::reductions::interaction_ground_data& data,
+void print_update_igl(VW::workspace& all, VW::shared_data& /*sd*/, const VW::reductions::igl::igl_data& data,
     const VW::multi_ex& ec_seq, VW::io::logger& /*logger*/)
 {
   if (ec_seq.empty()) { return; }
   const auto& ec = **(ec_seq.begin());
   if (VW::example_is_newline(ec) && !VW::ec_is_example_header_cb_with_observations(ec)) { return; }
 
   bool labeled_example = true;
   if (data.known_cost.probability <= 0) { labeled_example = false; }
 
   VW::details::print_update_cb(all, !labeled_example, ec, &ec_seq, true, &data.known_cost);
 }
 
-void output_igl_prediction(VW::workspace& all, const interaction_ground_data& /* data */, const VW::multi_ex& ec_seq,
-    VW::io::logger& /* unused */)
+void pre_save_load_igl(VW::workspace& all, igl::igl_data& data)
+{
+  options_i& options = *all.options;
+  if (!data._predict_only_model) { return; }
+
+  auto cb_adf_learner = all.l->get_learner_by_name_prefix("cb_adf")->shared_from_this();
+  auto cb_adf_data = static_cast<cb_adf*>(cb_adf_learner->get_internal_type_erased_data_pointer_test_use_only());
+
+  std::swap(cb_adf_data->get_gen_cs_mtr().per_model_state[0], cb_adf_data->get_gen_cs_mtr().per_model_state[1]);
+
+  // Adjust pi model weights to new single-model space
+  VW::reductions::multi_model::reduce_innermost_model_weights(
+      all.weights.dense_weights, data._cb_model_offset, all.reduction_state.total_feature_width, data._feature_width);
+
+  for (auto& group : options.get_all_option_group_definitions())
+  {
+    if (group.m_name == "[Reduction] Interaction Grounded Learning Options")
+    {
+      for (auto& opt : group.m_options) { opt->m_keep = false; }
+    }
+  }
+
+  all.initial_weights_config.num_bits =
+      all.initial_weights_config.num_bits - static_cast<uint32_t>(std::log2(all.reduction_state.total_feature_width));
+  options.get_typed_option<uint32_t>("bit_precision").value(all.initial_weights_config.num_bits);
+}
+
+void output_igl_prediction(
+    VW::workspace& all, const igl::igl_data& /* data */, const VW::multi_ex& ec_seq, VW::io::logger& /* unused */)
 {
   if (!ec_seq.empty())
   {
     // Print predictions
     for (auto& sink : all.output_runtime.final_prediction_sink)
     {
       VW::details::print_action_score(sink.get(), ec_seq[VW::details::SHARED_EX_INDEX]->pred.a_s,
           ec_seq[VW::details::SHARED_EX_INDEX]->tag, all.logger);
     }
     VW::details::global_print_newline(all.output_runtime.final_prediction_sink, all.logger);
   }
 }
 
-void update_stats_igl(const VW::workspace& /* all */, VW::shared_data& sd,
-    const VW::reductions::interaction_ground_data& data, const VW::multi_ex& ec_seq, VW::io::logger& /*logger*/)
+void update_stats_igl(const VW::workspace& /* all */, VW::shared_data& sd, const VW::reductions::igl::igl_data& data,
+    const VW::multi_ex& ec_seq, VW::io::logger& /*logger*/)
 {
   if (ec_seq.size() <= 0) { return; }
 
   size_t num_features = 0;
 
   float loss = 0.;
 
@@ -324,17 +358,19 @@
                       .keep()
                       .necessary()
                       .help("Do Interaction Grounding with multiline action dependent features")
                       .experimental());
 
   if (!pi_options.add_parse_and_check_necessary(new_options)) { return nullptr; }
 
-  // number of weight vectors needed
-  size_t feature_width = 2;  // One for reward and one for loss
-  auto ld = VW::make_unique<VW::reductions::interaction_ground_data>();
+  // number of weight vectors needed, one for ik model(offset 0) and one for cb model(offset 1)
+  size_t feature_width = 2;
+  bool predict_only_model = pi_options.was_supplied("predict_only_model");
+
+  auto ld = VW::make_unique<VW::reductions::igl::igl_data>(predict_only_model);
 
   if (!pi_options.was_supplied("cb_explore_adf")) { pi_options.insert("cb_explore_adf", ""); }
 
   if (!pi_options.was_supplied("coin")) { THROW("--experimental_igl needs to use --coin"); }
 
   auto pi_learner = require_multiline(stack_builder.setup_base_learner(feature_width));
 
@@ -345,24 +381,25 @@
   std::vector<std::string> ik_args = {"--quiet", "--link=logistic", "--loss_function=logistic", "--coin"};
   std::unique_ptr<options_i, options_deleter_type> ik_options(
       new config::options_cli(ik_args), [](VW::config::options_i* ptr) { delete ptr; });
 
   assert(ik_options->was_supplied("cb_explore_adf") == false || ik_options->was_supplied("cb_adf") == false);
   assert(ik_options->was_supplied("loss_function") == true);
 
+  ld->ik_ftrl = static_cast<ftrl*>(ftrl_coin->get_internal_type_erased_data_pointer_test_use_only());
+  ld->pi_ftrl = VW::make_unique<ftrl>();
+  *ld->pi_ftrl.get() = *ld->ik_ftrl;
+
   ld->ik_all = VW::initialize_experimental(
       VW::make_unique<VW::config::options_cli>(ik_args), nullptr, nullptr, nullptr, &all->logger);
 
   std::unique_ptr<ik_stack_builder> ik_builder = VW::make_unique<ik_stack_builder>(ftrl_coin);
-  ik_builder->delayed_state_attach(*ld->ik_all, *ik_options);
-  ld->ik_learner = require_singleline(ik_builder->setup_base_learner());
 
-  ld->ik_ftrl = static_cast<ftrl*>(ftrl_coin->get_internal_type_erased_data_pointer_test_use_only());
-  ld->pi_ftrl = VW::make_unique<ftrl>();
-  *ld->pi_ftrl.get() = *ld->ik_ftrl;
+  ik_builder->delayed_state_attach(*ld->ik_ftrl->all, *ik_options);
+  ld->ik_learner = require_singleline(ik_builder->setup_base_learner());
 
   ld->interactions = all->feature_tweaks_config.interactions;
   ld->extent_interactions = &all->feature_tweaks_config.extent_interactions;
 
   VW::prediction_type_t pred_type;
 
   if (pi_learner->get_output_prediction_type() == prediction_type_t::ACTION_SCORES)
@@ -382,13 +419,14 @@
                .set_output_label_type(label_type_t::CB)
                .set_input_prediction_type(pred_type)
                .set_output_prediction_type(pred_type)
                .set_update_stats(update_stats_igl)
                .set_print_update(print_update_igl)
                .set_save_load(save_load_igl)
                .set_output_example_prediction(output_igl_prediction)
+               .set_pre_save_load(pre_save_load_igl)
                .build();
 
   // TODO: assert ftrl is the base, fail otherwise
   // VW::reductions::util::fail_if_enabled
   return l;
 }
```

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/kernel_svm.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/kernel_svm.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/lda_core.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/lda_core.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/log_multi.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/log_multi.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/lrq.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/lrq.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/lrqfa.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/lrqfa.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/marginal.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/marginal.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/memory_tree.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/memory_tree.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/metrics.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/metrics.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/mf.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/mf.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/multilabel_oaa.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/multilabel_oaa.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/mwt.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/mwt.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/nn.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/nn.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/noop.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/noop.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/oaa.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/oaa.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/offset_tree.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/offset_tree.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/oja_newton.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/oja_newton.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/plt.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/plt.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/pmf_to_pdf.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/pmf_to_pdf.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/print.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/print.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/recall_tree.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/recall_tree.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/sample_pdf.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/sample_pdf.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/scorer.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/scorer.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/search/search.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/search/search.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/search/search_dep_parser.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/search/search_dep_parser.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/search/search_entityrelationtask.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/search/search_entityrelationtask.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/search/search_graph.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/search/search_graph.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/search/search_hooktask.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/search/search_hooktask.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/search/search_meta.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/search/search_meta.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/search/search_multiclasstask.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/search/search_multiclasstask.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/search/search_sequencetask.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/search/search_sequencetask.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/sender.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/sender.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/shared_feature_merger.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/shared_feature_merger.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/slates.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/slates.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/stagewise_poly.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/stagewise_poly.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/svrg.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/svrg.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/topk.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/topk.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/shared_data.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/shared_data.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/simple_label.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/simple_label.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/simple_label_parser.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/simple_label_parser.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/slates_label.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/slates_label.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/tag_utils.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/tag_utils.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/text_utils.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/text_utils.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/unique_sort.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/unique_sort.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/version.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/version.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/vw.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/vw.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/vw_validate.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/vw_validate.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/automl_test.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/automl_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/automl_weights_test.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/automl_weights_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/baseline_cb_test.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/baseline_cb_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/cats_test.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/cats_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/cats_tree_test.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/cats_tree_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/cats_user_provided_pdf.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/cats_user_provided_pdf.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/cb_explore_adf_test.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/cb_explore_adf_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/cb_large_actions_test.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/cb_large_actions_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/cb_las_one_pass_svd_test.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/cb_las_one_pass_svd_test.cc`

 * *Files 0% similar despite different names*

```diff
@@ -375,15 +375,15 @@
       vw->finish_example(examples);
     }
   }
 
   EXPECT_TRUE(U_wnocache.isApprox(U_wcache, vwtest::EXPLICIT_FLOAT_TOL));
 }
 
-#ifdef BUILD_LAS_WITH_SIMD
+#ifdef VW_FEAT_LAS_SIMD_ENABLED
 TEST(Las, ComputeDotProdScalarAndSimdHaveSameResults)
 {
   float (*compute_dot_prod_simd)(uint64_t, VW::workspace*, uint64_t, VW::example*);
   if (VW::cb_explore_adf::cpu_supports_avx512())
   {
     compute_dot_prod_simd = VW::cb_explore_adf::compute_dot_prod_avx512;
   }
```

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/cb_las_spanner_test.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/cb_las_spanner_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/cb_with_observations_parser_test.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/cb_with_observations_parser_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/ccb_parser_test.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/ccb_parser_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/ccb_test.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/ccb_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/chain_hashing.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/chain_hashing.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/confidence_sequence_robust_test.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/confidence_sequence_robust_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/confidence_sequence_test.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/confidence_sequence_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/continuous_actions_parser_test.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/continuous_actions_parser_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/custom_reduction_test.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/custom_reduction_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/distributionally_robust_test.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/distributionally_robust_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/eigen_memory_tree_test.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/eigen_memory_tree_test.cc`

 * *Files 27% similar despite different names*

```diff
@@ -9,102 +9,133 @@
 #include "vw/core/learner.h"
 #include "vw/core/vw.h"
 #include "vw/test_common/test_common.h"
 
 #include <gtest/gtest.h>
 
 #include <string>
+#include <utility>
 #include <vector>
 
 using namespace VW::reductions::eigen_memory_tree;
 
-namespace eigen_memory_tree_test
-{
-emt_tree* get_emt_tree(VW::workspace& all)
+emt_tree* get_emt_tree(const VW::workspace& all)
 {
   std::vector<std::string> e_r;
   all.l->get_enabled_learners(e_r);
   if (std::find(e_r.begin(), e_r.end(), "emt") == e_r.end())
   {
     ADD_FAILURE() << "Eigen memory tree not found in enabled learners";
   }
 
   VW::LEARNER::learner* emt = require_singleline(all.l->get_learner_by_name_prefix("emt"));
 
   return (emt_tree*)emt->get_internal_type_erased_data_pointer_test_use_only();
 }
 
-TEST(Emt, ParamsTest1)
+TEST(EigenMemoryTree, ParamsTest1)
 {
   auto vw = VW::initialize(vwtest::make_args("--quiet", "--emt"));
   auto* tree = get_emt_tree(*vw);
 
   EXPECT_EQ(tree->leaf_split, 100);
   EXPECT_EQ(tree->scorer_type, emt_scorer_type::SELF_CONSISTENT_RANK);
   EXPECT_EQ(tree->router_type, emt_router_type::EIGEN);
   EXPECT_EQ(tree->bounder->max_size, 0);
 }
 
-TEST(Emt, ParamsTest2)
+TEST(EigenMemoryTree, ParamsTest2)
 {
   auto args = vwtest::make_args(
       "--quiet", "--emt", "--emt_tree", "20", "--emt_scorer", "distance", "--emt_router", "random", "--emt_leaf", "50");
   auto vw = VW::initialize(std::move(args));
   auto tree = get_emt_tree(*vw);
 
   EXPECT_EQ(tree->leaf_split, 50);
   EXPECT_EQ(tree->scorer_type, emt_scorer_type::DISTANCE);
   EXPECT_EQ(tree->router_type, emt_router_type::RANDOM);
   EXPECT_EQ(tree->bounder->max_size, 20);
 }
 
-TEST(Emt, ExactMatchSansRouterTest)
+TEST(EigenMemoryTree, ExactMatchSansRouterTest)
 {
   auto vw = VW::initialize(vwtest::make_args("--quiet", "--emt"));
 
   auto* ex1 = VW::read_example(*vw, "1 | 1 2 3");
   auto* ex2 = VW::read_example(*vw, "2 | 2 3 4");
+  auto* ex3 = VW::read_example(*vw, "3 | 5");
 
   vw->learn(*ex1);
   vw->learn(*ex2);
+  vw->learn(*ex3);
 
   EXPECT_EQ(ex1->pred.multiclass, 0);
   EXPECT_EQ(ex2->pred.multiclass, 1);
 
   vw->predict(*ex1);
   vw->predict(*ex2);
 
   EXPECT_EQ(ex1->pred.multiclass, 1);
   EXPECT_EQ(ex2->pred.multiclass, 2);
 
   vw->finish_example(*ex1);
   vw->finish_example(*ex2);
+  vw->finish_example(*ex3);
 }
 
-TEST(Emt, ExactMatchWithRouterTest)
+TEST(EigenMemoryTree, CloseMatchSansRouterTest)
 {
-  auto vw = VW::initialize(vwtest::make_args("--quiet", "--emt", "--emt_leaf", "5"));
+  auto vw = VW::initialize(
+      vwtest::make_args("--quiet", "--emt", "--emt_leaf", "20", "--adaptive", "--invariant", "--noconstant"));
 
   for (int i = 0; i < 10; i++)
   {
-    auto* ex = VW::read_example(*vw, std::to_string(i) + " | " + std::to_string(i));
-    vw->learn(*ex);
+    auto* ex1 = VW::read_example(*vw, std::to_string(i) + " | 1:" + std::to_string(i));
+    vw->learn(*ex1);
+    vw->finish_example(*ex1);
+
+    auto* ex2 = VW::read_example(*vw, std::to_string(i) + " | 1:" + std::to_string(i));
+    vw->learn(*ex2);
+    vw->finish_example(*ex2);
+  }
+
+  for (int i = 0; i < 10; i++)
+  {
+    auto* ex = VW::read_example(*vw, " | 1:" + std::to_string(i + .1));
+    vw->predict(*ex);
+    EXPECT_EQ(ex->pred.multiclass, i);
     vw->finish_example(*ex);
   }
+}
+
+TEST(EigenMemoryTree, ExactMatchWithRouterTest)
+{
+  auto vw = VW::initialize(vwtest::make_args("--quiet", "--emt", "--emt_leaf", "5"));
+
+  for (int i = 0; i < 10; i++)
+  {
+    auto* ex1 = VW::read_example(*vw, std::to_string(i) + " | " + std::to_string(i));
+    vw->learn(*ex1);
+    vw->finish_example(*ex1);
+
+    auto* ex2 = VW::read_example(*vw, std::to_string(i) + " | " + std::to_string(i));
+    vw->learn(*ex2);
+    vw->finish_example(*ex2);
+  }
 
   for (int i = 0; i < 10; i++)
   {
     auto* ex = VW::read_example(*vw, " | " + std::to_string(i));
     vw->predict(*ex);
     EXPECT_EQ(ex->pred.multiclass, i);
     vw->finish_example(*ex);
   }
 }
 
-TEST(Emt, Bounding)
+TEST(EigenMemoryTree, Bounding)
 {
   auto vw = VW::initialize(vwtest::make_args("--quiet", "--emt", "--emt_tree", "5"));
   auto* tree = get_emt_tree(*vw);
 
   for (int i = 0; i < 10; i++)
   {
     auto* ex = VW::read_example(*vw, std::to_string(i) + " | " + std::to_string(i));
@@ -113,15 +144,15 @@
   }
 
   EXPECT_EQ(tree->bounder->list.size(), 5);
   EXPECT_EQ(tree->root->examples.size(), 5);
   EXPECT_EQ(tree->root->router_weights.size(), 0);
 }
 
-TEST(Emt, Split)
+TEST(EigenMemoryTree, Split)
 {
   auto args = vwtest::make_args("--quiet", "--emt", "--emt_tree", "10", "--emt_leaf", "3");
   auto vw = VW::initialize(std::move(args));
   auto* tree = get_emt_tree(*vw);
 
   for (int i = 0; i < 4; i++)
   {
@@ -137,115 +168,117 @@
   EXPECT_EQ(tree->root->right->examples.size(), 2);
 
   EXPECT_GE(tree->root->router_weights.size(), 0);
   EXPECT_EQ(tree->root->right->router_weights.size(), 0);
   EXPECT_EQ(tree->root->left->router_weights.size(), 0);
 }
 
-TEST(Emt, Inner)
+TEST(EigenMemoryTree, Inner)
 {
   emt_feats v1;
   emt_feats v2;
 
   EXPECT_EQ(emt_inner(v1, v2), 0);
 
-  v1.emplace_back(1, 2);
-  v2.emplace_back(2, 2);
+  v1.push_back(std::make_pair(1, 2));
+  v2.push_back(std::make_pair(2, 2));
 
   EXPECT_EQ(emt_inner(v1, v2), 0);
 
-  v1.emplace_back(2, 3);
+  v1.push_back(std::make_pair(2, 3));
 
   EXPECT_EQ(emt_inner(v1, v2), 6);
 
-  v1.emplace_back(3, 2);
-  v2.emplace_back(3, 5);
+  v1.push_back(std::make_pair(3, 2));
+  v2.push_back(std::make_pair(3, 5));
 
   EXPECT_EQ(emt_inner(v1, v2), 16);
 }
 
-TEST(Emt, ScaleAdd)
+TEST(EigenMemoryTree, ScaleAdd)
 {
   emt_feats v1;
   emt_feats v2;
   emt_feats v3;
 
   EXPECT_EQ(emt_scale_add(1, v1, 1, v2), v3);
 
-  v1.emplace_back(1, 2);
-  v3.emplace_back(1, 2);
+  v1.push_back(std::make_pair(1, 2));
+  v3.push_back(std::make_pair(1, 2));
 
   EXPECT_EQ(emt_scale_add(1, v1, 1, v2), v3);
 
   v3.clear();
-  v3.emplace_back(1, -1);
+  v3.push_back(std::make_pair(1, -1));
 
   EXPECT_EQ(emt_scale_add(-.5, v1, 1, v2), v3);
 
   v1.clear();
   v2.clear();
   v3.clear();
-  v1.emplace_back(1, 2);
-  v2.emplace_back(1, 2.5);
-  v3.emplace_back(1, -.5);
+  v1.push_back(std::make_pair(1, 2));
+  v2.push_back(std::make_pair(1, 2.5));
+  v3.push_back(std::make_pair(1, -.5));
 
   EXPECT_EQ(emt_scale_add(1, v1, -1, v2), v3);
 
   v1.clear();
   v2.clear();
   v3.clear();
-  v1.emplace_back(1, 2);
-  v2.emplace_back(1, 2.5);
-  v2.emplace_back(5, 1);
-  v3.emplace_back(1, -4.5);
-  v3.emplace_back(5, -1);
+  v1.push_back(std::make_pair(1, 2));
+  v2.push_back(std::make_pair(1, 2.5));
+  v2.push_back(std::make_pair(5, 1));
+  v3.push_back(std::make_pair(1, -4.5));
+  v3.push_back(std::make_pair(5, -1));
 
   EXPECT_EQ(emt_scale_add(-1, v1, -1, v2), v3);
-}
-
-TEST(Emt, Abs)
-{
-  emt_feats v1;
-  emt_feats v2;
-
-  emt_abs(v1);
-  EXPECT_EQ(v1, v2);
 
-  v1.emplace_back(1, -3);
-  v2.emplace_back(1, 3);
+  v1.clear();
+  v2.clear();
+  v3.clear();
+  v1.push_back(std::make_pair(1, 2));
+  v1.push_back(std::make_pair(5, 1));
+  v2.push_back(std::make_pair(1, 2.5));
+  v3.push_back(std::make_pair(1, -4.5));
+  v3.push_back(std::make_pair(5, -1));
 
-  emt_abs(v1);
-  EXPECT_EQ(v1, v2);
+  EXPECT_EQ(emt_scale_add(-1, v1, -1, v2), v3);
 
-  v1.emplace_back(2, -4);
-  v2.emplace_back(2, 4);
+  v1.clear();
+  v2.clear();
+  v3.clear();
+  v1.push_back(std::make_pair(1, 2));
+  v1.push_back(std::make_pair(5, 1));
+  v2.push_back(std::make_pair(1, 2.5));
+  v2.push_back(std::make_pair(5, -1));
+  v3.push_back(std::make_pair(1, -4.5));
+  v3.push_back(std::make_pair(5, 0));
 
-  emt_abs(v1);
-  EXPECT_EQ(v1, v2);
+  EXPECT_EQ(emt_scale_add(-1, v1, -1, v2), v3);
 }
 
-TEST(Emt, Normalize)
+TEST(EigenMemoryTree, Normalize)
 {
   emt_feats v1;
   emt_feats v2;
 
   emt_normalize(v1);
   EXPECT_EQ(v1, v2);
 
-  v1.emplace_back(1, -3);
-  v1.emplace_back(5, 4);
+  v1.push_back(std::make_pair(1, -3));
+  v1.push_back(std::make_pair(5, 4));
 
-  v2.emplace_back(1, -.6);
-  v2.emplace_back(5, .8);
+  v2.push_back(std::make_pair(1, -.6));
+  v2.push_back(std::make_pair(5, .8));
 
   emt_normalize(v1);
   EXPECT_EQ(v1, v2);
 }
 
-TEST(Emt, Median)
+TEST(EigenMemoryTree, Median)
 {
   std::vector<float> v1;
 
   v1.push_back(3);
   v1.push_back(1);
   v1.push_back(2);
 
@@ -256,30 +289,30 @@
   v1.push_back(2);
   v1.push_back(6);
   v1.push_back(4);
 
   EXPECT_EQ(emt_median(v1), 5);
 }
 
-TEST(Emt, RouterEigen)
+TEST(EigenMemoryTree, RouterEigen)
 {
   VW::rand_state rng(1);
 
   emt_feats v1;
   emt_feats v2;
   emt_feats v3;
 
-  v1.emplace_back(1, 2);
-  v1.emplace_back(3, 3);
-  v1.emplace_back(5, 2);
+  v1.push_back(std::make_pair(1, 2));
+  v1.push_back(std::make_pair(3, 3));
+  v1.push_back(std::make_pair(5, 2));
 
-  v2.emplace_back(2, 5);
+  v2.push_back(std::make_pair(2, 5));
 
-  v3.emplace_back(1, 4);
-  v3.emplace_back(2, 10);
+  v3.push_back(std::make_pair(1, 4));
+  v3.push_back(std::make_pair(2, 10));
 
   std::vector<emt_feats> f;
 
   f.push_back(v1);
   f.push_back(v2);
   f.push_back(v3);
 
@@ -300,50 +333,79 @@
   EXPECT_NEAR(weights[0].second, -0.0863, .01);
   EXPECT_NEAR(weights[1].second, -0.9171, .01);
   EXPECT_NEAR(weights[2].second, 0.3237, .01);
   EXPECT_NEAR(weights[3].second, 0.2158, .01);
   EXPECT_GE(var, 19.29);
 }
 
-TEST(Emt, Shuffle)
+TEST(EigenMemoryTree, ScorerInitial)
+{
+  emt_feats v1;
+  emt_feats v2;
+
+  emt_normalize(v1);
+  EXPECT_EQ(v1, v2);
+
+  v1.push_back(std::make_pair(1, -2));
+  v1.push_back(std::make_pair(5, 3));
+
+  v2.push_back(std::make_pair(1, 1));
+  v2.push_back(std::make_pair(5, -1));
+
+  EXPECT_EQ(emt_initial(emt_initial_type::NONE, v1, v2), 0);
+  EXPECT_EQ(emt_initial(emt_initial_type::EUCLIDEAN, v1, v2), 5);
+  EXPECT_NEAR(emt_initial(emt_initial_type::GAUSSIAN, v1, v2), 1 - std::exp(-5), .001);
+  EXPECT_NEAR(emt_initial(emt_initial_type::COSINE, v1, v2), 1.98, .001);
+}
+
+TEST(EigenMemoryTree, Shuffle)
 {
   VW::rand_state rng(2);
 
   std::vector<int> v1{1, 2, 3};
 
   emt_shuffle(v1.begin(), v1.end(), rng);
 
   EXPECT_EQ(v1[0], 2);
   EXPECT_EQ(v1[1], 3);
   EXPECT_EQ(v1[2], 1);
 }
 
-TEST(Emt, SaveLoad)
+TEST(EigenMemoryTree, SaveLoad)
 {
-  auto vw_save = VW::initialize(vwtest::make_args("--quiet", "--emt", "--emt_leaf", "5"));
+  auto vw_save = VW::initialize(vwtest::make_args("--quiet", "--emt", "--emt_leaf", "5", "--emt_initial", "gaussian"));
 
   for (int i = 0; i < 10; i++)
   {
-    auto* ex = VW::read_example(*vw_save, std::to_string(i) + " | " + std::to_string(i));
-    vw_save->learn(*ex);
-    vw_save->finish_example(*ex);
+    auto* ex1 = VW::read_example(*vw_save, std::to_string(i) + " | 1:" + std::to_string(i));
+    vw_save->learn(*ex1);
+    vw_save->finish_example(*ex1);
+
+    auto* ex2 = VW::read_example(*vw_save, std::to_string(i) + " | 1:" + std::to_string(i));
+    vw_save->learn(*ex2);
+    vw_save->finish_example(*ex2);
   }
 
   auto backing_vector = std::make_shared<std::vector<char>>();
   VW::io_buf io_writer;
   io_writer.add_file(VW::io::create_vector_writer(backing_vector));
   VW::save_predictor(*vw_save, io_writer);
   io_writer.flush();
 
   auto vw_load = VW::initialize(vwtest::make_args("--no_stdin", "--quiet", "--preserve_performance_counters"),
       VW::io::create_buffer_view(backing_vector->data(), backing_vector->size()));
 
+  auto* tree = get_emt_tree(*vw_load);
+
+  EXPECT_EQ(tree->leaf_split, 5);
+  EXPECT_EQ(static_cast<int>(tree->initial_type), 2);
+  EXPECT_EQ(static_cast<int>(tree->scorer_type), 3);
+  EXPECT_EQ(static_cast<int>(tree->router_type), 2);
+
   for (int i = 0; i < 10; i++)
   {
-    auto* ex = VW::read_example(*vw_load, " | " + std::to_string(i));
+    auto* ex = VW::read_example(*vw_load, " | 1:" + std::to_string(i + 0.1));
     vw_load->predict(*ex);
     EXPECT_EQ(ex->pred.multiclass, i);
     vw_load->finish_example(*ex);
   }
-}
-
-}  // namespace eigen_memory_tree_test
+}
```

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/epsilon_decay_test.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/epsilon_decay_test.cc`

 * *Files 1% similar despite different names*

```diff
@@ -99,16 +99,16 @@
         EXPECT_EQ(epsilon_decay->conf_seq_estimators[2][2].update_count, 93);
         EXPECT_EQ(epsilon_decay->conf_seq_estimators[3][2].update_count, 93);
         EXPECT_EQ(epsilon_decay->conf_seq_estimators[3][3].update_count, 94);
         return true;
       });
 
   // we initialize the reduction pointing to position 0 as champ, that config is hard-coded to empty
-  auto ctr = simulator::_test_helper_hook(
-      std::vector<std::string>{"--epsilon_decay", "--model_count", "4", "--cb_explore_adf", "--quiet", "-q", "::"},
+  auto ctr = simulator::_test_helper_hook(std::vector<std::string>{"--epsilon_decay", "--model_count", "4",
+                                              "--challenger_epsilon", "--cb_explore_adf", "--quiet", "-q", "::"},
       test_hooks, num_iterations, seed, swap_after);
 
   EXPECT_GT(ctr.back(), 0.4f);
 }
 
 TEST(EpsilonDecay, UpdateCountWIterations)
 {
@@ -251,15 +251,15 @@
 TEST(EpsilonDecay, ScoreBoundsUnit)
 {
   // Initialize epsilon_decay_data class with 5 models
   uint64_t num_models = 5;
   uint32_t feature_width = 8;
   VW::dense_parameters dense_weights(num_models);
   epsilon_decay_data ep_data(
-      num_models, 100, .05, .1, dense_weights, "", false, feature_width, 0, 1.f, 0, false, 1e-6, "bisect", false);
+      num_models, 100, .05, .1, dense_weights, "", false, feature_width, 0, 1.f, 0, false, 1e-6, "bisect", false, true);
 
   // Set update counts to fixed values with expected horizon bound violation
   size_t score_idx = 0;
   for (uint64_t model_ind = 0; model_ind < num_models; ++model_ind)
   {
     for (uint64_t score_ind = 0; score_ind <= model_ind; ++score_ind)
     {
@@ -337,15 +337,15 @@
 TEST(EpsilonDecay, HorizonBoundsUnit)
 {
   // Initialize epsilon_decay_data class with 5 models
   uint64_t num_models = 5;
   uint32_t feature_width = 8;
   VW::dense_parameters dense_weights(num_models);
   epsilon_decay_data ep_data(
-      num_models, 100, .05, .1, dense_weights, "", false, feature_width, 0, 1.f, 0, false, 1e-6, "bisect", false);
+      num_models, 100, .05, .1, dense_weights, "", false, feature_width, 0, 1.f, 0, false, 1e-6, "bisect", false, true);
 
   // Set update counts to fixed values with expected horizon bound violation
   size_t score_idx = 0;
   uint64_t over_horizon = 2;
   for (uint64_t model_ind = 0; model_ind < num_models; ++model_ind)
   {
     for (uint64_t score_ind = 0; score_ind <= model_ind; ++score_ind)
```

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/epsilon_test.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/epsilon_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/example_ft_hash_test.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/example_ft_hash_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/example_header_test.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/example_header_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/example_test.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/example_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/feature_group_test.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/feature_group_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/flat_example_test.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/flat_example_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/guard_test.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/guard_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/hyperopt_test.py` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/hyperopt_test.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/igl_simulator.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/igl_simulator.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/igl_simulator.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/igl_simulator.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/igl_test.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/igl_test.cc`

 * *Files 22% similar despite different names*

```diff
@@ -212,28 +212,28 @@
   separate_weights_vector sl_weights = get_separate_weights(std::move(sl_vw));
   std::vector<separate_weights_vector> igl_weights = split_weights(std::move(igl_vw));
 
   EXPECT_GT(sl_weights.size(), 0);
   EXPECT_EQ(sl_weights, igl_weights[0]);
 }
 
-TEST(Igl, TrainingCoverges)
+TEST(Igl, TrainingConverges)
 {
   std::vector<std::string> igl_args = {"--cb_explore_adf", "--epsilon", "0.2", "--dsjson", "--coin",
       "--experimental_igl", "--noconstant", "-b", "19", "-q", "UA", "--quiet"};
 
   const size_t num_iterations = 2500;
-  const size_t seed = 777;
+  const size_t seed = 378123;
 
   auto igl_vw = VW::initialize(vwtest::make_args(igl_args));
 
   igl_simulator::igl_sim sim(seed);
   auto ctr_vector = sim.run_simulation(igl_vw.get(), 1, num_iterations);
 
-  EXPECT_GT(ctr_vector.back(), 0.5f);
+  EXPECT_GT(ctr_vector.back(), 0.6f);
 }
 
 TEST(Igl, SaveResume)
 {
   std::vector<std::string> igl_args = {"--cb_explore_adf", "--epsilon", "0.2", "--dsjson", "--coin",
       "--experimental_igl", "--noconstant", "-b", "19", "-q", "UA", "--quiet"};
 
@@ -267,7 +267,59 @@
 
   // continue
   auto ctr_save_resume = sim_split.run_simulation(igl_second.get(), split + 1, split);
   igl_second->finish();
 
   EXPECT_EQ(ctr_vector, ctr_save_resume);
 }
+
+TEST(Igl, VerifyPredictOnlyModelEqualsToCbModel)
+{
+  // clang-format off
+  std::vector<std::string> igl_vector = {
+      R"({"_label_cost": 0, "_label_probability": 0.25, "_label_Action": 4, "_labelIndex": 3, "o": [{"v": {"v=none": 1}, "_definitely_bad": false}], "a": [0, 1, 2, 3], "c": {"User": {"user=Anna": 1, "time_of_day=afternoon": 1}, "_multi": [{"Action": {"action=politics": 1}}, {"Action": {"action=sports": 1}}, {"Action": {"action=music": 1}}, {"Action": {"action=food": 1}}]}, "p": [0.25, 0.25, 0.25, 0.25], "_original_label_cost": 0})",
+      R"({"_label_cost": 0, "_label_probability": 0.25, "_label_Action": 2, "_labelIndex": 1, "o": [{"v": {"v=none": 1}, "_definitely_bad": false}], "a": [0, 1, 2, 3], "c": {"User": {"user=Tom": 1, "time_of_day=morning": 1}, "_multi": [{"Action": {"action=politics": 1}}, {"Action": {"action=sports": 1}}, {"Action": {"action=music": 1}}, {"Action": {"action=food": 1}}]}, "p": [0.25, 0.25, 0.25, 0.25], "_original_label_cost": 0})",
+      R"({"_label_cost": 0, "_label_probability": 0.25, "_label_Action": 3, "_labelIndex": 2, "o": [{"v": {"v=click": 1}, "_definitely_bad": false}], "a": [0, 1, 2, 3], "c": {"User": {"user=Tom": 1, "time_of_day=afternoon": 1}, "_multi": [{"Action": {"action=politics": 1}}, {"Action": {"action=sports": 1}}, {"Action": {"action=music": 1}}, {"Action": {"action=food": 1}}]}, "p": [0.25, 0.25, 0.25, 0.25], "_original_label_cost": 0})",
+      R"({"_label_cost": 0, "_label_probability": 0.25, "_label_Action": 3, "_labelIndex": 2, "o": [{"v": {"v=like": 1}, "_definitely_bad": false}], "a": [0, 1, 2, 3], "c": {"User": {"user=Tom": 1, "time_of_day=afternoon": 1}, "_multi": [{"Action": {"action=politics": 1}}, {"Action": {"action=sports": 1}}, {"Action": {"action=music": 1}}, {"Action": {"action=food": 1}}]}, "p": [0.25, 0.25, 0.25, 0.25], "_original_label_cost": -0.5})",
+      R"({"_label_cost": 0, "_label_probability": 0.25, "_label_Action": 2, "_labelIndex": 1, "o": [{"v": {"v=skip": 1}, "_definitely_bad": false}], "a": [0, 1, 2, 3], "c": {"User": {"user=Tom": 1, "time_of_day=afternoon": 1}, "_multi": [{"Action": {"action=politics": 1}}, {"Action": {"action=sports": 1}}, {"Action": {"action=music": 1}}, {"Action": {"action=food": 1}}]}, "p": [0.25, 0.25, 0.25, 0.25], "_original_label_cost": 0})",
+      R"({"_label_cost": 0, "_label_probability": 0.25, "_label_Action": 3, "_labelIndex": 2, "o": [{"v": {"v=none": 1}, "_definitely_bad": false}], "a": [0, 1, 2, 3], "c": {"User": {"user=Anna": 1, "time_of_day=morning": 1}, "_multi": [{"Action": {"action=politics": 1}}, {"Action": {"action=sports": 1}}, {"Action": {"action=music": 1}}, {"Action": {"action=food": 1}}]}, "p": [0.25, 0.25, 0.25, 0.25], "_original_label_cost": 0})",
+      R"({"_label_cost": -1, "_label_probability": 0.8500000016763806, "_label_Action": 3, "_labelIndex": 2, "o": [{"v": {"v=click": 1}, "_definitely_bad": false}], "a": [0, 1, 2, 3], "c": {"User": {"user=Tom": 1, "time_of_day=afternoon": 1}, "_multi": [{"Action": {"action=politics": 1}}, {"Action": {"action=sports": 1}}, {"Action": {"action=music": 1}}, {"Action": {"action=food": 1}}]}, "p": [0.04999999944120647, 0.04999999944120647, 0.8500000016763806, 0.04999999944120647], "_original_label_cost": -0.5})",
+      R"({"_label_cost": 0, "_label_probability": 0.8500000016763806, "_label_Action": 3, "_labelIndex": 2, "o": [{"v": {"v=none": 1}, "_definitely_bad": false}], "a": [0, 1, 2, 3], "c": {"User": {"user=Anna": 1, "time_of_day=morning": 1}, "_multi": [{"Action": {"action=politics": 1}}, {"Action": {"action=sports": 1}}, {"Action": {"action=music": 1}}, {"Action": {"action=food": 1}}]}, "p": [0.04999999944120647, 0.04999999944120647, 0.8500000016763806, 0.04999999944120647], "_original_label_cost": 0})",
+      R"({"_label_cost": 0, "_label_probability": 0.3166666677221655, "_label_Action": 1, "_labelIndex": 0, "o": [{"v": {"v=none": 1}, "_definitely_bad": false}], "a": [0, 1, 2, 3], "c": {"User": {"user=Anna": 1, "time_of_day=morning": 1}, "_multi": [{"Action": {"action=politics": 1}}, {"Action": {"action=sports": 1}}, {"Action": {"action=music": 1}}, {"Action": {"action=food": 1}}]}, "p": [0.3166666677221655, 0.3166666677221655, 0.04999999683350349, 0.3166666677221655], "_original_label_cost": 0})",
+      R"({"_label_cost": 0, "_label_probability": 0.8500000016763806, "_label_Action": 3, "_labelIndex": 2, "o": [{"v": {"v=none": 1}, "_definitely_bad": false}], "a": [0, 1, 2, 3], "c": {"User": {"user=Anna": 1, "time_of_day=afternoon": 1}, "_multi": [{"Action": {"action=politics": 1}}, {"Action": {"action=sports": 1}}, {"Action": {"action=music": 1}}, {"Action": {"action=food": 1}}]}, "p": [0.04999999944120647, 0.04999999944120647, 0.8500000016763806, 0.04999999944120647], "_original_label_cost": 0})"
+  };
+  // clang-format on
+
+  // IGL instance
+  auto igl_vw = VW::initialize(vwtest::make_args("--experimental_igl", "--coin", "--cb_explore_adf", "--dsjson",
+      "--noconstant", "--quiet", "-q", "UA", "--predict_only_model", "-b", "18"));
+
+  auto multi_vw = VW::initialize(vwtest::make_args("--cb_explore_adf", "--coin", "--dsjson", "-q", "UA", "--noconstant",
+      "--quiet", "-b", "17", "--predict_only_model"));
+
+  // train cb model
+  for (size_t i = 0; i < igl_vector.size(); i++)
+  {
+    auto multi_ex = igl_vector[i];
+    auto examples = vwtest::parse_dsjson(*multi_vw, multi_ex);
+    VW::setup_examples(*multi_vw, examples);
+    multi_vw->learn(examples);
+    multi_vw->finish_example(examples);
+  }
+
+  separate_weights_vector multi_weights = get_separate_weights(std::move(multi_vw));
+
+  // train IGL
+  for (auto& ex : igl_vector)
+  {
+    auto examples = vwtest::parse_dsjson(*igl_vw, ex);
+    VW::setup_examples(*igl_vw, examples);
+
+    igl_vw->learn(examples);
+    igl_vw->finish_example(examples);
+  }
+
+  std::vector<separate_weights_vector> igl_weights = split_weights(std::move(igl_vw));
+
+  EXPECT_GT(multi_weights.size(), 0);
+  EXPECT_EQ(multi_weights, igl_weights[1]);
+}
```

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/interactions_test.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/interactions_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/loss_functions_test.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/loss_functions_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/math_test.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/math_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/merge_header_opts_test.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/merge_header_opts_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/merge_test.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/merge_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/minimal_custom_reduction.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/minimal_custom_reduction.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/model_util_test.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/model_util_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/multiclass_label_parser_test.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/multiclass_label_parser_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/numeric_cast_test.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/numeric_cast_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/object_pool_test.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/object_pool_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/offset_tree_test.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/offset_tree_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/parse_args_test.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/parse_args_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/parser_test.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/parser_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/pmf_to_pdf_test.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/pmf_to_pdf_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/power_test.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/power_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/prediction_test.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/prediction_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/random_test.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/random_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/save_load_test.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/save_load_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/scope_exit_test.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/scope_exit_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/slates_parser_test.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/slates_parser_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/slates_test.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/slates_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/status_builder_test.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/status_builder_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/tag_utils_test.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/tag_utils_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/thread_pool_test.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/thread_pool_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/tokenize_test.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/tokenize_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/tutorial_test.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/tutorial_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/v_array_test.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/v_array_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/vw_versions_test.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/vw_versions_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/weights_test.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/weights_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/vw_types.natvis` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/vw_types.natvis`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/csv_parser/CMakeLists.txt` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/csv_parser/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/csv_parser/include/vw/csv_parser/parse_example_csv.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/csv_parser/include/vw/csv_parser/parse_example_csv.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/csv_parser/src/parse_example_csv.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/csv_parser/src/parse_example_csv.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/csv_parser/tests/csv_parser_test.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/csv_parser/tests/csv_parser_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/explore/include/vw/explore/explore.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/explore/include/vw/explore/explore.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/explore/include/vw/explore/explore_internal.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/explore/include/vw/explore/explore_internal.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/explore/tests/explore_test.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/explore/tests/explore_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/fb_parser/CMakeLists.txt` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/fb_parser/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/fb_parser/include/vw/fb_parser/parse_example_flatbuffer.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/fb_parser/include/vw/fb_parser/parse_example_flatbuffer.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/fb_parser/schema/example.fbs` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/fb_parser/schema/example.fbs`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/fb_parser/src/parse_example_flatbuffer.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/fb_parser/src/parse_example_flatbuffer.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/fb_parser/src/parse_label.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/fb_parser/src/parse_label.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/fb_parser/tests/flatbuffer_parser_test.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/fb_parser/tests/flatbuffer_parser_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/io/CMakeLists.txt` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/io/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/io/include/vw/io/custom_streambuf.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/io/include/vw/io/custom_streambuf.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/io/include/vw/io/errno_handling.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/io/include/vw/io/errno_handling.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/io/include/vw/io/io_adapter.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/io/include/vw/io/io_adapter.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/io/include/vw/io/logger.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/io/include/vw/io/logger.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/io/include/vw/io/owning_stream.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/io/include/vw/io/owning_stream.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/io/src/errno_handling.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/io/src/errno_handling.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/io/src/io_adapter.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/io/src/io_adapter.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/io/src/logger.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/io/src/logger.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/io/tests/errno_test.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/io/tests/errno_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/io/tests/io_adapter_test.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/io/tests/io_adapter_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/io/tests/ostream_test.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/io/tests/ostream_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/json_parser/CMakeLists.txt` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/json_parser/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/json_parser/include/vw/json_parser/decision_service_utils.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/json_parser/include/vw/json_parser/decision_service_utils.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/json_parser/include/vw/json_parser/parse_example_json.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/json_parser/include/vw/json_parser/parse_example_json.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/json_parser/include/vw/json_parser/parse_example_slates_json.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/json_parser/include/vw/json_parser/parse_example_slates_json.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/json_parser/src/json_utils.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/json_parser/src/json_utils.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/json_parser/src/parse_example_json.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/json_parser/src/parse_example_json.cc`

 * *Files 2% similar despite different names*

```diff
@@ -207,14 +207,92 @@
   }
 
 private:
   BaseState<audit>* obj_return_state;
 };
 
 template <bool audit>
+class ArrayToGraphState : public BaseState<audit>
+{
+public:
+  BaseState<audit>* return_state;
+  VW::cb_graph_feedback::triplet graph_triplet;
+
+  ArrayToGraphState() : BaseState<audit>("ArrayToGraphObject"), graph_triplet(0, 0, -1.f) {}
+
+  BaseState<audit>* StartObject(Context<audit>& ctx) override
+  {
+    obj_return_state = ctx.previous_state;
+    return this;
+  }
+
+  BaseState<audit>* Key(Context<audit>& ctx, const char* str, rapidjson::SizeType len, bool /* copy */) override
+  {
+    ctx.key = str;
+    ctx.key_length = len;
+    return this;
+  }
+
+  BaseState<audit>* String(Context<audit>& ctx, const char* str, rapidjson::SizeType len, bool) override
+  {
+    ctx.error() << "Unexpected token: std::string('" << str << "' len: " << len << ")";
+    return nullptr;
+  }
+
+  BaseState<audit>* StartArray(Context<audit>& ctx) override
+  {
+    return_state = ctx.previous_state;
+    graph_triplet = VW::cb_graph_feedback::triplet(0, 0, -1.f);
+    return this;
+  }
+
+  BaseState<audit>* EndArray(Context<audit>&, rapidjson::SizeType) override { return return_state; }
+
+  BaseState<audit>* Float(Context<audit>& ctx, float v) override
+  {
+    if (!_stricmp(ctx.key, "val")) { graph_triplet.val = v; }
+    else
+    {
+      ctx.error() << "Unsupported label property: '" << ctx.key << "' len: " << ctx.key_length;
+      return nullptr;
+    }
+
+    return this;
+  }
+
+  BaseState<audit>* Uint(Context<audit>& ctx, unsigned v) override
+  {
+    if (!_stricmp(ctx.key, "val")) { graph_triplet.val = v; }
+    else if (!_stricmp(ctx.key, "row")) { graph_triplet.row = v; }
+    else if (!_stricmp(ctx.key, "col")) { graph_triplet.col = v; }
+    else
+    {
+      ctx.error() << "Unsupported label property: '" << ctx.key << "' len: " << ctx.key_length;
+      return nullptr;
+    }
+    return this;
+  }
+
+  BaseState<audit>* EndObject(Context<audit>& ctx, rapidjson::SizeType) override
+  {
+    auto& graph_reduction_features =
+        ctx.ex->ex_reduction_features.template get<VW::cb_graph_feedback::reduction_features>();
+    if (graph_triplet.val != -1.f)
+    {
+      graph_reduction_features.push_triplet(graph_triplet.row, graph_triplet.col, graph_triplet.val);
+    }
+    graph_triplet = VW::cb_graph_feedback::triplet(0, 0, -1.f);
+    return obj_return_state;
+  }
+
+private:
+  BaseState<audit>* obj_return_state;
+};
+
+template <bool audit>
 class LabelObjectState : public BaseState<audit>
 {
 public:
   VW::cb_class cb_label;
   VW::cb_continuous::continuous_label_elm cont_label_element = {0., 0., 0.};
   bool found = false;
   bool found_cb = false;
@@ -930,14 +1008,15 @@
         }
       }
 
       if (ctx.key_length == 5 && !strcmp(ctx.key, "_text")) { return &ctx.text_state; }
 
       // TODO: _multi in _multi...
       if (ctx.key_length == 6 && !strcmp(ctx.key, "_multi")) { return &ctx.multi_state; }
+      if (ctx.key_length == 6 && !strcmp(ctx.key, "_graph")) { return &ctx.array_to_graph_state; }
 
       if (ctx.key_length == 6 && !strcmp(ctx.key, "_slots")) { return &ctx.slots_state; }
 
       if (ctx.key_length == 4 && !_stricmp(ctx.key, "_tag")) { return &ctx.tag_state; }
 
       if (ctx.key_length == 4 && !_stricmp(ctx.key, "_inc"))
       {
@@ -1619,14 +1698,15 @@
   MultiState<audit> multi_state;
   ObservationState<audit> o_state;
   DefinitelyBadState<audit> definitely_bad_state;
   IgnoreState<audit> ignore_state;
   ArrayState<audit> array_state;
   SlotsState<audit> slots_state;
   ArrayToPdfState<audit> array_pdf_state;
+  ArrayToGraphState<audit> array_to_graph_state;
 
   // DecisionServiceState
   DecisionServiceState<audit> decision_service_state;
   ArrayToVectorState<audit, float> array_float_state;
   ArrayToVectorState<audit, unsigned> array_uint_state;
   StringToStringState<audit> string_state;
   FloatToFloatState<audit, float_aggregation::set> float_state;
```

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/json_parser/src/parse_example_slates_json.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/json_parser/src/parse_example_slates_json.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/json_parser/tests/dsjson_parser_test.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/json_parser/tests/dsjson_parser_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/json_parser/tests/json_parser_test.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/json_parser/tests/json_parser_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/model_merger/src/main.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/model_merger/src/main.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/readme.md` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/readme.md`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/CMakeLists.txt` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/include/vw/slim/example_predict_builder.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/include/vw/slim/example_predict_builder.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/include/vw/slim/model_parser.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/include/vw/slim/model_parser.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/include/vw/slim/opts.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/include/vw/slim/opts.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/include/vw/slim/vw_slim_predict.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/include/vw/slim/vw_slim_predict.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/include/vw/slim/vw_slim_return_codes.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/include/vw/slim/vw_slim_return_codes.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/src/example_predict_builder.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/src/example_predict_builder.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/src/model_parser.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/src/model_parser.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/src/opts.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/src/opts.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/src/vw_slim_predict.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/src/vw_slim_predict.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/Delay_Margin_AudioNetworkPCR_all__unique_context.json` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/Delay_Margin_AudioNetworkPCR_all__unique_context.json`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/Delay_Margin_AudioNetworkPCR_all_cb_FF8.model` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/Delay_Margin_AudioNetworkPCR_all_cb_FF8.model`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/generate-data.sh` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/generate-data.sh`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/ut_explore.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/ut_explore.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/ut_opts.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/ut_opts.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/ut_util.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/ut_util.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/spanning_tree/include/vw/spanning_tree/spanning_tree.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/spanning_tree/include/vw/spanning_tree/spanning_tree.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/spanning_tree/src/spanning_tree.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/spanning_tree/src/spanning_tree.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/spanning_tree_bin/src/spanning_tree_main.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/spanning_tree_bin/src/spanning_tree_main.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/test_common/include/vw/test_common/matchers.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/test_common/include/vw/test_common/matchers.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/test_common/include/vw/test_common/test_common.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/test_common/include/vw/test_common/test_common.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/test_common/src/test_common.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/test_common/src/test_common.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/text_parser/include/vw/text_parser/parse_example_text.h` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/text_parser/include/vw/text_parser/parse_example_text.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/ext_libs/vowpal_wabbit/vowpalwabbit/text_parser/src/parse_example_text.cc` & `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/text_parser/src/parse_example_text.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/pyproject.toml` & `vowpal-wabbit-next-0.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/setup.py` & `vowpal-wabbit-next-0.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/src/cpp/debug_reduction.cc` & `vowpal-wabbit-next-0.4.1/src/cpp/debug_reduction.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/src/cpp/debug_reduction.h` & `vowpal-wabbit-next-0.4.1/src/cpp/debug_reduction.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/src/cpp/label.cc` & `vowpal-wabbit-next-0.4.1/src/cpp/label.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/src/cpp/label.h` & `vowpal-wabbit-next-0.4.1/src/cpp/label.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/src/cpp/main.cpp` & `vowpal-wabbit-next-0.4.1/src/cpp/main.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #include "debug_reduction.h"
 #include "label.h"
 #include "prediction.h"
 #include "vw/common/text_utils.h"
 #include "vw/config/options_cli.h"
+#include "vw/core/array_parameters.h"
 #include "vw/core/array_parameters_dense.h"
 #include "vw/core/cache.h"
 #include "vw/core/cb.h"
 #include "vw/core/ccb_label.h"
 #include "vw/core/ccb_reduction_features.h"
 #include "vw/core/constant.h"
 #include "vw/core/cost_sensitive.h"
@@ -794,14 +795,26 @@
   // TODO - when updating VW submodule if learn calls update stats then remove this to avoid a double call.
   update_stats_recursive(*workspace.workspace_ptr, *learner, example);
   auto prediction = vwpy::to_prediction(example[0]->pred, workspace.workspace_ptr->l->get_output_prediction_type());
   if (workspace.debug) { return std::make_tuple(prediction, debug_info); }
   return prediction;
 }
 
+size_t count_non_zero_weights(const VW::parameters& weights)
+{
+  if (weights.sparse)
+  {
+    return std::count_if(weights.sparse_weights.cbegin(), weights.sparse_weights.cend(), [](const float& w) { return w != 0.f; });
+  }
+  else
+  {
+    return std::count_if(weights.dense_weights.cbegin(), weights.dense_weights.cend(), [](const float& w) { return w != 0.f; });
+  }
+}
+
 }  // namespace
 
 PYBIND11_MODULE(_core, m)
 {
   py::options options;
   options.disable_enum_members_docstring();
 
@@ -1530,14 +1543,21 @@
       .def("get_label_type",
           [](const workspace_with_logger_contexts& workspace) -> VW::label_type_t
           { return workspace.workspace_ptr->l->get_input_label_type(); })
       .def("serialize",
           [](const workspace_with_logger_contexts& workspace) -> py::bytes
           {
             auto backing_vector = std::make_shared<std::vector<char>>();
+            // Determine size estimate by counting non-zero weights.
+            const auto non_zero_weights = count_non_zero_weights(workspace.workspace_ptr->weights);
+            const auto size_estimate_for_weights = non_zero_weights * sizeof(float) * workspace.workspace_ptr->weights.stride();
+            const auto size_estimate_overall = size_estimate_for_weights + 1024; // Add 1KB for other info
+            // Best effort reserve of likely final size to avoid reallocations.
+            backing_vector->reserve(size_estimate_overall);
+
             VW::io_buf io_writer;
             io_writer.add_file(VW::io::create_vector_writer(backing_vector));
             VW::save_predictor(*workspace.workspace_ptr, io_writer);
             io_writer.flush();
             return py::bytes(backing_vector->data(), backing_vector->size());  // Return the data without transcoding
           })
       .def(
```

### Comparing `vowpal-wabbit-next-0.4.0/src/cpp/prediction.cc` & `vowpal-wabbit-next-0.4.1/src/cpp/prediction.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/src/cpp/prediction.h` & `vowpal-wabbit-next-0.4.1/src/cpp/prediction.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/src/vowpal_wabbit_next/__init__.py` & `vowpal-wabbit-next-0.4.1/src/vowpal_wabbit_next/__init__.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/src/vowpal_wabbit_next/_core.pyi` & `vowpal-wabbit-next-0.4.1/src/vowpal_wabbit_next/_core.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -459,10 +459,10 @@
     pass
 def _run_cli_driver(args: typing.List[str], *, onethread: bool = False) -> typing.Tuple[typing.Optional[str], str, typing.List[str]]:
     pass
 def _write_cache_example(workspace: Workspace, example: Example, file: object) -> None:
     pass
 def _write_cache_header(workspace: Workspace, file: object) -> None:
     pass
-__version__ = '0.4.0'
-_vw_commit = '4715756'
+__version__ = '0.4.1'
+_vw_commit = 'b8c4ee3'
 _vw_version = '9.8.0'
```

### Comparing `vowpal-wabbit-next-0.4.0/src/vowpal_wabbit_next/cache_format.py` & `vowpal-wabbit-next-0.4.1/src/vowpal_wabbit_next/cache_format.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/src/vowpal_wabbit_next/cli_driver.py` & `vowpal-wabbit-next-0.4.1/src/vowpal_wabbit_next/cli_driver.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/src/vowpal_wabbit_next/delta.py` & `vowpal-wabbit-next-0.4.1/src/vowpal_wabbit_next/delta.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/src/vowpal_wabbit_next/dsjson_format.py` & `vowpal-wabbit-next-0.4.1/src/vowpal_wabbit_next/dsjson_format.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/src/vowpal_wabbit_next/example.py` & `vowpal-wabbit-next-0.4.1/src/vowpal_wabbit_next/example.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/src/vowpal_wabbit_next/json_format.py` & `vowpal-wabbit-next-0.4.1/src/vowpal_wabbit_next/json_format.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/src/vowpal_wabbit_next/text_format.py` & `vowpal-wabbit-next-0.4.1/src/vowpal_wabbit_next/text_format.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/src/vowpal_wabbit_next/workspace.py` & `vowpal-wabbit-next-0.4.1/src/vowpal_wabbit_next/workspace.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/src/vowpal_wabbit_next.egg-info/PKG-INFO` & `vowpal-wabbit-next-0.4.1/src/vowpal_wabbit_next.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vowpal-wabbit-next
-Version: 0.4.0
+Version: 0.4.1
 Summary: Experimental python bindings for VowpalWabbit
 Author: VowpalWabbit
 License: BSD-3-Clause
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -20,15 +20,15 @@
 ```sh
 pip install vowpal-wabbit-next
 ```
 
 ## Example
 
 ```python
-import vowpalwabbit_next as vw
+import vowpal_wabbit_next as vw
 import io
 
 cb_input = io.StringIO(
     """shared | s
 0:1:0.5 | a=0
 | a=1
```

### Comparing `vowpal-wabbit-next-0.4.0/src/vowpal_wabbit_next.egg-info/SOURCES.txt` & `vowpal-wabbit-next-0.4.1/src/vowpal_wabbit_next.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -705,15 +705,15 @@
 ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/automl_test.cc
 ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/automl_weights_test.cc
 ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/baseline_cb_test.cc
 ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/cats_test.cc
 ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/cats_tree_test.cc
 ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/cats_user_provided_pdf.cc
 ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/cb_explore_adf_test.cc
-ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/cb_graph_feedback_label_text_parse_test.cc
+ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/cb_graph_feedback_label_parse_test.cc
 ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/cb_graph_feedback_test.cc
 ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/cb_large_actions_test.cc
 ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/cb_las_one_pass_svd_test.cc
 ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/cb_las_spanner_test.cc
 ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/cb_with_observations_parser_test.cc
 ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/ccb_parser_test.cc
 ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/ccb_test.cc
```

### Comparing `vowpal-wabbit-next-0.4.0/tests/test_cache.py` & `vowpal-wabbit-next-0.4.1/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/tests/test_cli.py` & `vowpal-wabbit-next-0.4.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/tests/test_debug.py` & `vowpal-wabbit-next-0.4.1/tests/test_debug.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/tests/test_delta.py` & `vowpal-wabbit-next-0.4.1/tests/test_delta.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/tests/test_dsjson_format_reader.py` & `vowpal-wabbit-next-0.4.1/tests/test_dsjson_format_reader.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/tests/test_hash.py` & `vowpal-wabbit-next-0.4.1/tests/test_hash.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/tests/test_json_format_reader.py` & `vowpal-wabbit-next-0.4.1/tests/test_json_format_reader.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/tests/test_labels.py` & `vowpal-wabbit-next-0.4.1/tests/test_labels.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/tests/test_learn.py` & `vowpal-wabbit-next-0.4.1/tests/test_learn.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/tests/test_metrics.py` & `vowpal-wabbit-next-0.4.1/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/tests/test_serialization.py` & `vowpal-wabbit-next-0.4.1/tests/test_serialization.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.0/tests/test_text_format_reader.py` & `vowpal-wabbit-next-0.4.1/tests/test_text_format_reader.py`

 * *Files identical despite different names*

