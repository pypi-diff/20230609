# Comparing `tmp/ikfast_pybind-0.1.1.tar.gz` & `tmp/ikfast_pybind-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ikfast_pybind-0.1.1.tar", last modified: Wed Apr 21 21:37:12 2021, max compression
+gzip compressed data, was "dist\ikfast_pybind-0.1.2.tar", last modified: Fri Jun  9 17:05:45 2023, max compression
```

## Comparing `ikfast_pybind-0.1.1.tar` & `ikfast_pybind-0.1.2.tar`

### file list

```diff
@@ -1,119 +1,126 @@
-drwxrwxrwx   0        0        0        0 2021-04-21 21:37:12.533546 ikfast_pybind-0.1.1/
--rw-rw-rw-   0        0        0       80 2021-04-21 14:19:00.000000 ikfast_pybind-0.1.1/AUTHORS.rst
--rw-rw-rw-   0        0        0     1217 2021-04-21 15:46:44.000000 ikfast_pybind-0.1.1/CHANGELOG.rst
--rw-rw-rw-   0        0        0      329 2021-04-21 14:51:02.000000 ikfast_pybind-0.1.1/CMakeLists.txt
--rw-rw-rw-   0        0        0      301 2021-04-21 14:19:00.000000 ikfast_pybind-0.1.1/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0     1086 2021-04-21 14:19:00.000000 ikfast_pybind-0.1.1/LICENSE
--rw-rw-rw-   0        0        0      427 2021-04-21 14:19:00.000000 ikfast_pybind-0.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0     6837 2021-04-21 21:37:12.533237 ikfast_pybind-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     3507 2021-04-21 14:19:00.000000 ikfast_pybind-0.1.1/README.rst
-drwxrwxrwx   0        0        0        0 2021-04-21 21:37:12.447434 ikfast_pybind-0.1.1/ext/
--rw-rw-rw-   0        0        0       28 2021-04-21 14:19:00.000000 ikfast_pybind-0.1.1/ext/CMakeLists.txt
-drwxrwxrwx   0        0        0        0 2021-04-21 21:37:12.448437 ikfast_pybind-0.1.1/ext/pybind11/
--rw-rw-rw-   0        0        0    10721 2021-04-21 14:28:18.000000 ikfast_pybind-0.1.1/ext/pybind11/CMakeLists.txt
-drwxrwxrwx   0        0        0        0 2021-04-21 21:37:12.429485 ikfast_pybind-0.1.1/ext/pybind11/include/
-drwxrwxrwx   0        0        0        0 2021-04-21 21:37:12.469135 ikfast_pybind-0.1.1/ext/pybind11/include/pybind11/
--rw-rw-rw-   0        0        0    21963 2021-04-21 14:28:18.000000 ikfast_pybind-0.1.1/ext/pybind11/include/pybind11/attr.h
--rw-rw-rw-   0        0        0     6264 2021-04-21 14:28:18.000000 ikfast_pybind-0.1.1/ext/pybind11/include/pybind11/buffer_info.h
--rw-rw-rw-   0        0        0    58910 2021-04-21 14:28:18.000000 ikfast_pybind-0.1.1/ext/pybind11/include/pybind11/cast.h
--rw-rw-rw-   0        0        0     8714 2021-04-21 14:28:18.000000 ikfast_pybind-0.1.1/ext/pybind11/include/pybind11/chrono.h
--rw-rw-rw-   0        0        0      122 2021-04-21 14:19:01.000000 ikfast_pybind-0.1.1/ext/pybind11/include/pybind11/common.h
--rw-rw-rw-   0        0        0     2102 2021-04-21 14:28:18.000000 ikfast_pybind-0.1.1/ext/pybind11/include/pybind11/complex.h
-drwxrwxrwx   0        0        0        0 2021-04-21 21:37:12.476391 ikfast_pybind-0.1.1/ext/pybind11/include/pybind11/detail/
--rw-rw-rw-   0        0        0    28531 2021-04-21 14:28:18.000000 ikfast_pybind-0.1.1/ext/pybind11/include/pybind11/detail/class.h
--rw-rw-rw-   0        0        0    42980 2021-04-21 14:28:18.000000 ikfast_pybind-0.1.1/ext/pybind11/include/pybind11/detail/common.h
--rw-rw-rw-   0        0        0     3702 2021-04-21 14:28:18.000000 ikfast_pybind-0.1.1/ext/pybind11/include/pybind11/detail/descr.h
--rw-rw-rw-   0        0        0    16733 2021-04-21 14:28:18.000000 ikfast_pybind-0.1.1/ext/pybind11/include/pybind11/detail/init.h
--rw-rw-rw-   0        0        0    16738 2021-04-21 14:28:18.000000 ikfast_pybind-0.1.1/ext/pybind11/include/pybind11/detail/internals.h
--rw-rw-rw-   0        0        0    41607 2021-04-21 14:28:18.000000 ikfast_pybind-0.1.1/ext/pybind11/include/pybind11/detail/type_caster_base.h
--rw-rw-rw-   0        0        0     1541 2021-04-21 14:28:18.000000 ikfast_pybind-0.1.1/ext/pybind11/include/pybind11/detail/typeid.h
--rw-rw-rw-   0        0        0    29693 2021-04-21 14:28:18.000000 ikfast_pybind-0.1.1/ext/pybind11/include/pybind11/eigen.h
--rw-rw-rw-   0        0        0     8044 2021-04-21 14:28:18.000000 ikfast_pybind-0.1.1/ext/pybind11/include/pybind11/embed.h
--rw-rw-rw-   0        0        0     5231 2021-04-21 14:28:18.000000 ikfast_pybind-0.1.1/ext/pybind11/include/pybind11/eval.h
--rw-rw-rw-   0        0        0     3993 2021-04-21 14:28:18.000000 ikfast_pybind-0.1.1/ext/pybind11/include/pybind11/functional.h
--rw-rw-rw-   0        0        0     6725 2021-04-21 14:28:18.000000 ikfast_pybind-0.1.1/ext/pybind11/include/pybind11/gil.h
--rw-rw-rw-   0        0        0     6304 2021-04-21 14:28:18.000000 ikfast_pybind-0.1.1/ext/pybind11/include/pybind11/iostream.h
--rw-rw-rw-   0        0        0    71456 2021-04-21 14:28:18.000000 ikfast_pybind-0.1.1/ext/pybind11/include/pybind11/numpy.h
--rw-rw-rw-   0        0        0     9258 2021-04-21 14:28:18.000000 ikfast_pybind-0.1.1/ext/pybind11/include/pybind11/operators.h
--rw-rw-rw-   0        0        0     2114 2021-04-21 14:28:18.000000 ikfast_pybind-0.1.1/ext/pybind11/include/pybind11/options.h
--rw-rw-rw-   0        0        0   108057 2021-04-21 14:28:18.000000 ikfast_pybind-0.1.1/ext/pybind11/include/pybind11/pybind11.h
--rw-rw-rw-   0        0        0    69309 2021-04-21 14:28:18.000000 ikfast_pybind-0.1.1/ext/pybind11/include/pybind11/pytypes.h
--rw-rw-rw-   0        0        0    14550 2021-04-21 14:28:18.000000 ikfast_pybind-0.1.1/ext/pybind11/include/pybind11/stl.h
--rw-rw-rw-   0        0        0    24588 2021-04-21 14:28:18.000000 ikfast_pybind-0.1.1/ext/pybind11/include/pybind11/stl_bind.h
-drwxrwxrwx   0        0        0        0 2021-04-21 21:37:12.477421 ikfast_pybind-0.1.1/ext/pybind11/tests/
--rw-rw-rw-   0        0        0    16110 2021-04-21 14:28:18.000000 ikfast_pybind-0.1.1/ext/pybind11/tests/CMakeLists.txt
-drwxrwxrwx   0        0        0        0 2021-04-21 21:37:12.477706 ikfast_pybind-0.1.1/ext/pybind11/tests/test_cmake_build/
--rw-rw-rw-   0        0        0     2723 2021-04-21 14:28:18.000000 ikfast_pybind-0.1.1/ext/pybind11/tests/test_cmake_build/CMakeLists.txt
-drwxrwxrwx   0        0        0        0 2021-04-21 21:37:12.478703 ikfast_pybind-0.1.1/ext/pybind11/tests/test_cmake_build/installed_embed/
--rw-rw-rw-   0        0        0     1201 2021-04-21 14:28:18.000000 ikfast_pybind-0.1.1/ext/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt
-drwxrwxrwx   0        0        0        0 2021-04-21 21:37:12.479702 ikfast_pybind-0.1.1/ext/pybind11/tests/test_cmake_build/installed_function/
--rw-rw-rw-   0        0        0     1297 2021-04-21 14:28:18.000000 ikfast_pybind-0.1.1/ext/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt
-drwxrwxrwx   0        0        0        0 2021-04-21 21:37:12.480699 ikfast_pybind-0.1.1/ext/pybind11/tests/test_cmake_build/installed_target/
--rw-rw-rw-   0        0        0     1698 2021-04-21 14:28:18.000000 ikfast_pybind-0.1.1/ext/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt
-drwxrwxrwx   0        0        0        0 2021-04-21 21:37:12.482694 ikfast_pybind-0.1.1/ext/pybind11/tests/test_cmake_build/subdirectory_embed/
--rw-rw-rw-   0        0        0     1396 2021-04-21 14:28:18.000000 ikfast_pybind-0.1.1/ext/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt
-drwxrwxrwx   0        0        0        0 2021-04-21 21:37:12.482825 ikfast_pybind-0.1.1/ext/pybind11/tests/test_cmake_build/subdirectory_function/
--rw-rw-rw-   0        0        0     1160 2021-04-21 14:28:18.000000 ikfast_pybind-0.1.1/ext/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt
-drwxrwxrwx   0        0        0        0 2021-04-21 21:37:12.483828 ikfast_pybind-0.1.1/ext/pybind11/tests/test_cmake_build/subdirectory_target/
--rw-rw-rw-   0        0        0     1373 2021-04-21 14:28:18.000000 ikfast_pybind-0.1.1/ext/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt
-drwxrwxrwx   0        0        0        0 2021-04-21 21:37:12.484833 ikfast_pybind-0.1.1/ext/pybind11/tests/test_embed/
--rw-rw-rw-   0        0        0     1804 2021-04-21 14:28:18.000000 ikfast_pybind-0.1.1/ext/pybind11/tests/test_embed/CMakeLists.txt
-drwxrwxrwx   0        0        0        0 2021-04-21 21:37:12.491233 ikfast_pybind-0.1.1/ext/pybind11/tools/
--rw-rw-rw-   0        0        0     2365 2021-04-21 14:28:18.000000 ikfast_pybind-0.1.1/ext/pybind11/tools/FindCatch.cmake
--rw-rw-rw-   0        0        0     3191 2021-04-21 14:28:18.000000 ikfast_pybind-0.1.1/ext/pybind11/tools/FindEigen3.cmake
--rw-rw-rw-   0        0        0    10234 2021-04-21 14:28:18.000000 ikfast_pybind-0.1.1/ext/pybind11/tools/FindPythonLibsNew.cmake
--rw-rw-rw-   0        0        0    14561 2021-04-21 14:28:18.000000 ikfast_pybind-0.1.1/ext/pybind11/tools/pybind11Common.cmake
--rw-rw-rw-   0        0        0     9440 2021-04-21 14:28:18.000000 ikfast_pybind-0.1.1/ext/pybind11/tools/pybind11NewTools.cmake
--rw-rw-rw-   0        0        0     7496 2021-04-21 14:28:18.000000 ikfast_pybind-0.1.1/ext/pybind11/tools/pybind11Tools.cmake
-drwxrwxrwx   0        0        0        0 2021-04-21 21:37:12.499082 ikfast_pybind-0.1.1/ikfast_pybind.egg-info/
--rw-rw-rw-   0        0        0     6837 2021-04-21 21:37:12.000000 ikfast_pybind-0.1.1/ikfast_pybind.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3459 2021-04-21 21:37:12.000000 ikfast_pybind-0.1.1/ikfast_pybind.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-04-21 21:37:12.000000 ikfast_pybind-0.1.1/ikfast_pybind.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2021-04-21 15:21:32.000000 ikfast_pybind-0.1.1/ikfast_pybind.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       12 2021-04-21 21:37:12.000000 ikfast_pybind-0.1.1/ikfast_pybind.egg-info/requires.txt
--rw-rw-rw-   0        0        0       69 2021-04-21 21:37:12.000000 ikfast_pybind-0.1.1/ikfast_pybind.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2021-04-21 21:37:12.533546 ikfast_pybind-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     2240 2021-04-21 15:46:44.000000 ikfast_pybind-0.1.1/setup.py
--rw-rw-rw-   0        0        0     2676 2021-04-21 14:19:00.000000 ikfast_pybind-0.1.1/setup_cmake_utils.py
-drwxrwxrwx   0        0        0        0 2021-04-21 21:37:12.500098 ikfast_pybind-0.1.1/src/
--rw-rw-rw-   0        0        0      363 2021-04-21 15:41:56.000000 ikfast_pybind-0.1.1/src/CMakeLists.txt
-drwxrwxrwx   0        0        0        0 2021-04-21 21:37:12.504131 ikfast_pybind-0.1.1/src/abb_irb4600_40_255/
--rw-rw-rw-   0        0        0      135 2021-04-21 14:19:00.000000 ikfast_pybind-0.1.1/src/abb_irb4600_40_255/CMakeLists.txt
--rw-rw-rw-   0        0        0    13983 2021-04-21 14:19:00.000000 ikfast_pybind-0.1.1/src/abb_irb4600_40_255/ikfast.h
--rw-rw-rw-   0        0        0   826807 2021-04-21 14:19:00.000000 ikfast_pybind-0.1.1/src/abb_irb4600_40_255/ikfast0x10000049.Transform6D.0_1_2_3_4_5.cpp
--rw-rw-rw-   0        0        0     4003 2021-04-21 14:19:00.000000 ikfast_pybind-0.1.1/src/abb_irb4600_40_255/ikfast_pybind_abb_irb4600_40_255.cpp
-drwxrwxrwx   0        0        0        0 2021-04-21 21:37:12.510371 ikfast_pybind-0.1.1/src/eth_rfl/
--rw-rw-rw-   0        0        0      120 2021-04-21 14:19:00.000000 ikfast_pybind-0.1.1/src/eth_rfl/CMakeLists.txt
--rw-rw-rw-   0        0        0    13983 2021-04-21 14:19:00.000000 ikfast_pybind-0.1.1/src/eth_rfl/ikfast.h
--rw-rw-rw-   0        0        0   342454 2021-04-21 14:19:00.000000 ikfast_pybind-0.1.1/src/eth_rfl/ikfast0x10000049.Transform6D.3_4_5_6_7_8_f0_1_2.cpp
--rw-rw-rw-   0        0        0   319208 2021-04-21 14:19:00.000000 ikfast_pybind-0.1.1/src/eth_rfl/ikfast0x10000049.Transform6D.3_4_5_6_7_8_f2.cpp
--rw-rw-rw-   0        0        0     4122 2021-04-21 14:19:00.000000 ikfast_pybind-0.1.1/src/eth_rfl/ikfast_pybind_eth_rfl.cpp
-drwxrwxrwx   0        0        0        0 2021-04-21 21:37:12.514386 ikfast_pybind-0.1.1/src/franka_panda/
--rw-rw-rw-   0        0        0      126 2021-04-21 14:19:00.000000 ikfast_pybind-0.1.1/src/franka_panda/CMakeLists.txt
--rw-rw-rw-   0        0        0    13983 2021-04-21 14:19:00.000000 ikfast_pybind-0.1.1/src/franka_panda/ikfast.h
--rw-rw-rw-   0        0        0   398542 2021-04-21 14:19:00.000000 ikfast_pybind-0.1.1/src/franka_panda/ikfast0x10000049.Transform6D.0_1_2_3_4_5_f6.cpp
--rw-rw-rw-   0        0        0     4108 2021-04-21 14:19:00.000000 ikfast_pybind-0.1.1/src/franka_panda/ikfast_pybind_franka_panda.cpp
-drwxrwxrwx   0        0        0        0 2021-04-21 21:37:12.517831 ikfast_pybind-0.1.1/src/kawasaki_rs010n/
--rw-rw-rw-   0        0        0       91 2021-04-21 14:25:19.000000 ikfast_pybind-0.1.1/src/kawasaki_rs010n/CMakeLists.txt
--rw-rw-rw-   0        0        0   384980 2021-04-21 14:29:37.000000 ikfast_pybind-0.1.1/src/kawasaki_rs010n/ik.cpp
--rw-rw-rw-   0        0        0    13983 2021-04-21 14:19:00.000000 ikfast_pybind-0.1.1/src/kawasaki_rs010n/ikfast.h
--rw-rw-rw-   0        0        0     3974 2021-04-21 15:24:46.000000 ikfast_pybind-0.1.1/src/kawasaki_rs010n/ikfast_pybind_kawasaki_rs010n.cpp
-drwxrwxrwx   0        0        0        0 2021-04-21 21:37:12.522891 ikfast_pybind-0.1.1/src/kuka_kr6_r900/
--rw-rw-rw-   0        0        0      125 2021-04-21 14:19:00.000000 ikfast_pybind-0.1.1/src/kuka_kr6_r900/CMakeLists.txt
--rw-rw-rw-   0        0        0    13983 2021-04-21 14:19:00.000000 ikfast_pybind-0.1.1/src/kuka_kr6_r900/ikfast.h
--rw-rw-rw-   0        0        0   308035 2021-04-21 14:19:00.000000 ikfast_pybind-0.1.1/src/kuka_kr6_r900/ikfast0x1000004a.Transform6D.0_1_2_3_4_5.cpp
--rw-rw-rw-   0        0        0     3945 2021-04-21 14:19:00.000000 ikfast_pybind-0.1.1/src/kuka_kr6_r900/ikfast_pybind_kuka_kr6_r900.cpp
-drwxrwxrwx   0        0        0        0 2021-04-21 21:37:12.524589 ikfast_pybind-0.1.1/src/ur3/
--rw-rw-rw-   0        0        0       85 2021-04-21 14:19:00.000000 ikfast_pybind-0.1.1/src/ur3/CMakeLists.txt
--rw-rw-rw-   0        0        0     4114 2021-04-21 14:19:00.000000 ikfast_pybind-0.1.1/src/ur3/ikfast_pybind_ur3.cpp
-drwxrwxrwx   0        0        0        0 2021-04-21 21:37:12.526892 ikfast_pybind-0.1.1/src/ur3/ur_kinematics/
--rw-rw-rw-   0        0        0    13005 2021-04-21 14:19:00.000000 ikfast_pybind-0.1.1/src/ur3/ur_kinematics/ikfast.h
--rw-rw-rw-   0        0        0    15678 2021-04-21 14:19:00.000000 ikfast_pybind-0.1.1/src/ur3/ur_kinematics/ur_kin.cpp
--rw-rw-rw-   0        0        0     3597 2021-04-21 14:19:00.000000 ikfast_pybind-0.1.1/src/ur3/ur_kinematics/ur_kin.h
-drwxrwxrwx   0        0        0        0 2021-04-21 21:37:12.528886 ikfast_pybind-0.1.1/src/ur5/
--rw-rw-rw-   0        0        0       85 2021-04-21 14:19:00.000000 ikfast_pybind-0.1.1/src/ur5/CMakeLists.txt
--rw-rw-rw-   0        0        0     4116 2021-04-21 14:19:00.000000 ikfast_pybind-0.1.1/src/ur5/ikfast_pybind_ur5.cpp
-drwxrwxrwx   0        0        0        0 2021-04-21 21:37:12.532239 ikfast_pybind-0.1.1/src/ur5/ur_kinematics/
--rw-rw-rw-   0        0        0    13005 2021-04-21 14:19:00.000000 ikfast_pybind-0.1.1/src/ur5/ur_kinematics/ikfast.h
--rw-rw-rw-   0        0        0    14717 2021-04-21 14:19:00.000000 ikfast_pybind-0.1.1/src/ur5/ur_kinematics/ur_kin.cpp
--rw-rw-rw-   0        0        0     3847 2021-04-21 14:19:00.000000 ikfast_pybind-0.1.1/src/ur5/ur_kinematics/ur_kin.h
+drwxrwxrwx   0        0        0        0 2023-06-09 17:05:45.000000 ikfast_pybind-0.1.2/
+-rw-rw-rw-   0        0        0       80 2023-06-09 16:30:17.000000 ikfast_pybind-0.1.2/AUTHORS.rst
+-rw-rw-rw-   0        0        0     1325 2023-06-09 17:05:37.000000 ikfast_pybind-0.1.2/CHANGELOG.rst
+-rw-rw-rw-   0        0        0      329 2023-06-09 16:30:17.000000 ikfast_pybind-0.1.2/CMakeLists.txt
+-rw-rw-rw-   0        0        0      301 2023-06-09 16:30:17.000000 ikfast_pybind-0.1.2/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0     1086 2023-06-09 16:30:17.000000 ikfast_pybind-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0      427 2023-06-09 16:30:17.000000 ikfast_pybind-0.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     5853 2023-06-09 17:05:45.000000 ikfast_pybind-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3507 2023-06-09 16:30:17.000000 ikfast_pybind-0.1.2/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-09 17:05:45.000000 ikfast_pybind-0.1.2/ext/
+-rw-rw-rw-   0        0        0       28 2023-06-09 16:30:17.000000 ikfast_pybind-0.1.2/ext/CMakeLists.txt
+drwxrwxrwx   0        0        0        0 2023-06-09 17:05:45.000000 ikfast_pybind-0.1.2/ext/pybind11/
+-rw-rw-rw-   0        0        0    10721 2023-06-09 16:31:28.000000 ikfast_pybind-0.1.2/ext/pybind11/CMakeLists.txt
+drwxrwxrwx   0        0        0        0 2023-06-09 17:05:45.000000 ikfast_pybind-0.1.2/ext/pybind11/include/
+drwxrwxrwx   0        0        0        0 2023-06-09 17:05:45.000000 ikfast_pybind-0.1.2/ext/pybind11/include/pybind11/
+-rw-rw-rw-   0        0        0    21963 2023-06-09 16:31:28.000000 ikfast_pybind-0.1.2/ext/pybind11/include/pybind11/attr.h
+-rw-rw-rw-   0        0        0     6264 2023-06-09 16:31:28.000000 ikfast_pybind-0.1.2/ext/pybind11/include/pybind11/buffer_info.h
+-rw-rw-rw-   0        0        0    58910 2023-06-09 16:31:28.000000 ikfast_pybind-0.1.2/ext/pybind11/include/pybind11/cast.h
+-rw-rw-rw-   0        0        0     8714 2023-06-09 16:31:28.000000 ikfast_pybind-0.1.2/ext/pybind11/include/pybind11/chrono.h
+-rw-rw-rw-   0        0        0      122 2023-06-09 16:31:28.000000 ikfast_pybind-0.1.2/ext/pybind11/include/pybind11/common.h
+-rw-rw-rw-   0        0        0     2102 2023-06-09 16:31:28.000000 ikfast_pybind-0.1.2/ext/pybind11/include/pybind11/complex.h
+drwxrwxrwx   0        0        0        0 2023-06-09 17:05:45.000000 ikfast_pybind-0.1.2/ext/pybind11/include/pybind11/detail/
+-rw-rw-rw-   0        0        0    28531 2023-06-09 16:31:28.000000 ikfast_pybind-0.1.2/ext/pybind11/include/pybind11/detail/class.h
+-rw-rw-rw-   0        0        0    42980 2023-06-09 16:31:28.000000 ikfast_pybind-0.1.2/ext/pybind11/include/pybind11/detail/common.h
+-rw-rw-rw-   0        0        0     3702 2023-06-09 16:31:28.000000 ikfast_pybind-0.1.2/ext/pybind11/include/pybind11/detail/descr.h
+-rw-rw-rw-   0        0        0    16733 2023-06-09 16:31:28.000000 ikfast_pybind-0.1.2/ext/pybind11/include/pybind11/detail/init.h
+-rw-rw-rw-   0        0        0    16738 2023-06-09 16:31:28.000000 ikfast_pybind-0.1.2/ext/pybind11/include/pybind11/detail/internals.h
+-rw-rw-rw-   0        0        0    41607 2023-06-09 16:31:28.000000 ikfast_pybind-0.1.2/ext/pybind11/include/pybind11/detail/type_caster_base.h
+-rw-rw-rw-   0        0        0     1541 2023-06-09 16:31:28.000000 ikfast_pybind-0.1.2/ext/pybind11/include/pybind11/detail/typeid.h
+-rw-rw-rw-   0        0        0    29693 2023-06-09 16:31:28.000000 ikfast_pybind-0.1.2/ext/pybind11/include/pybind11/eigen.h
+-rw-rw-rw-   0        0        0     8044 2023-06-09 16:31:28.000000 ikfast_pybind-0.1.2/ext/pybind11/include/pybind11/embed.h
+-rw-rw-rw-   0        0        0     5231 2023-06-09 16:31:28.000000 ikfast_pybind-0.1.2/ext/pybind11/include/pybind11/eval.h
+-rw-rw-rw-   0        0        0     3993 2023-06-09 16:31:28.000000 ikfast_pybind-0.1.2/ext/pybind11/include/pybind11/functional.h
+-rw-rw-rw-   0        0        0     6725 2023-06-09 16:31:28.000000 ikfast_pybind-0.1.2/ext/pybind11/include/pybind11/gil.h
+-rw-rw-rw-   0        0        0     6304 2023-06-09 16:31:28.000000 ikfast_pybind-0.1.2/ext/pybind11/include/pybind11/iostream.h
+-rw-rw-rw-   0        0        0    71456 2023-06-09 16:31:28.000000 ikfast_pybind-0.1.2/ext/pybind11/include/pybind11/numpy.h
+-rw-rw-rw-   0        0        0     9258 2023-06-09 16:31:28.000000 ikfast_pybind-0.1.2/ext/pybind11/include/pybind11/operators.h
+-rw-rw-rw-   0        0        0     2114 2023-06-09 16:31:28.000000 ikfast_pybind-0.1.2/ext/pybind11/include/pybind11/options.h
+-rw-rw-rw-   0        0        0   108057 2023-06-09 16:31:28.000000 ikfast_pybind-0.1.2/ext/pybind11/include/pybind11/pybind11.h
+-rw-rw-rw-   0        0        0    69309 2023-06-09 16:31:28.000000 ikfast_pybind-0.1.2/ext/pybind11/include/pybind11/pytypes.h
+-rw-rw-rw-   0        0        0    14550 2023-06-09 16:31:28.000000 ikfast_pybind-0.1.2/ext/pybind11/include/pybind11/stl.h
+-rw-rw-rw-   0        0        0    24588 2023-06-09 16:31:28.000000 ikfast_pybind-0.1.2/ext/pybind11/include/pybind11/stl_bind.h
+drwxrwxrwx   0        0        0        0 2023-06-09 17:05:45.000000 ikfast_pybind-0.1.2/ext/pybind11/tests/
+-rw-rw-rw-   0        0        0    16110 2023-06-09 16:31:28.000000 ikfast_pybind-0.1.2/ext/pybind11/tests/CMakeLists.txt
+drwxrwxrwx   0        0        0        0 2023-06-09 17:05:45.000000 ikfast_pybind-0.1.2/ext/pybind11/tests/test_cmake_build/
+-rw-rw-rw-   0        0        0     2723 2023-06-09 16:31:28.000000 ikfast_pybind-0.1.2/ext/pybind11/tests/test_cmake_build/CMakeLists.txt
+drwxrwxrwx   0        0        0        0 2023-06-09 17:05:45.000000 ikfast_pybind-0.1.2/ext/pybind11/tests/test_cmake_build/installed_embed/
+-rw-rw-rw-   0        0        0     1201 2023-06-09 16:31:28.000000 ikfast_pybind-0.1.2/ext/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt
+drwxrwxrwx   0        0        0        0 2023-06-09 17:05:45.000000 ikfast_pybind-0.1.2/ext/pybind11/tests/test_cmake_build/installed_function/
+-rw-rw-rw-   0        0        0     1297 2023-06-09 16:31:28.000000 ikfast_pybind-0.1.2/ext/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt
+drwxrwxrwx   0        0        0        0 2023-06-09 17:05:45.000000 ikfast_pybind-0.1.2/ext/pybind11/tests/test_cmake_build/installed_target/
+-rw-rw-rw-   0        0        0     1698 2023-06-09 16:31:28.000000 ikfast_pybind-0.1.2/ext/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt
+drwxrwxrwx   0        0        0        0 2023-06-09 17:05:45.000000 ikfast_pybind-0.1.2/ext/pybind11/tests/test_cmake_build/subdirectory_embed/
+-rw-rw-rw-   0        0        0     1396 2023-06-09 16:31:28.000000 ikfast_pybind-0.1.2/ext/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt
+drwxrwxrwx   0        0        0        0 2023-06-09 17:05:45.000000 ikfast_pybind-0.1.2/ext/pybind11/tests/test_cmake_build/subdirectory_function/
+-rw-rw-rw-   0        0        0     1160 2023-06-09 16:31:28.000000 ikfast_pybind-0.1.2/ext/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt
+drwxrwxrwx   0        0        0        0 2023-06-09 17:05:45.000000 ikfast_pybind-0.1.2/ext/pybind11/tests/test_cmake_build/subdirectory_target/
+-rw-rw-rw-   0        0        0     1373 2023-06-09 16:31:28.000000 ikfast_pybind-0.1.2/ext/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt
+drwxrwxrwx   0        0        0        0 2023-06-09 17:05:45.000000 ikfast_pybind-0.1.2/ext/pybind11/tests/test_embed/
+-rw-rw-rw-   0        0        0     1804 2023-06-09 16:31:28.000000 ikfast_pybind-0.1.2/ext/pybind11/tests/test_embed/CMakeLists.txt
+drwxrwxrwx   0        0        0        0 2023-06-09 17:05:45.000000 ikfast_pybind-0.1.2/ext/pybind11/tools/
+-rw-rw-rw-   0        0        0     2365 2023-06-09 16:31:28.000000 ikfast_pybind-0.1.2/ext/pybind11/tools/FindCatch.cmake
+-rw-rw-rw-   0        0        0     3191 2023-06-09 16:31:28.000000 ikfast_pybind-0.1.2/ext/pybind11/tools/FindEigen3.cmake
+-rw-rw-rw-   0        0        0    10234 2023-06-09 16:31:28.000000 ikfast_pybind-0.1.2/ext/pybind11/tools/FindPythonLibsNew.cmake
+-rw-rw-rw-   0        0        0    14561 2023-06-09 16:31:28.000000 ikfast_pybind-0.1.2/ext/pybind11/tools/pybind11Common.cmake
+-rw-rw-rw-   0        0        0     9440 2023-06-09 16:31:28.000000 ikfast_pybind-0.1.2/ext/pybind11/tools/pybind11NewTools.cmake
+-rw-rw-rw-   0        0        0     7496 2023-06-09 16:31:28.000000 ikfast_pybind-0.1.2/ext/pybind11/tools/pybind11Tools.cmake
+drwxrwxrwx   0        0        0        0 2023-06-09 17:05:45.000000 ikfast_pybind-0.1.2/ikfast_pybind.egg-info/
+-rw-rw-rw-   0        0        0     5853 2023-06-09 17:05:45.000000 ikfast_pybind-0.1.2/ikfast_pybind.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3613 2023-06-09 17:05:45.000000 ikfast_pybind-0.1.2/ikfast_pybind.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 17:05:45.000000 ikfast_pybind-0.1.2/ikfast_pybind.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-09 16:32:02.000000 ikfast_pybind-0.1.2/ikfast_pybind.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       12 2023-06-09 17:05:45.000000 ikfast_pybind-0.1.2/ikfast_pybind.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       81 2023-06-09 17:05:45.000000 ikfast_pybind-0.1.2/ikfast_pybind.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-09 17:05:45.000000 ikfast_pybind-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     2322 2023-06-09 17:05:37.000000 ikfast_pybind-0.1.2/setup.py
+-rw-rw-rw-   0        0        0     2676 2023-06-09 16:30:17.000000 ikfast_pybind-0.1.2/setup_cmake_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-09 17:05:45.000000 ikfast_pybind-0.1.2/src/
+-rw-rw-rw-   0        0        0      387 2023-06-09 16:30:17.000000 ikfast_pybind-0.1.2/src/CMakeLists.txt
+drwxrwxrwx   0        0        0        0 2023-06-09 17:05:45.000000 ikfast_pybind-0.1.2/src/abb_irb4600_40_255/
+-rw-rw-rw-   0        0        0      135 2023-06-09 16:30:17.000000 ikfast_pybind-0.1.2/src/abb_irb4600_40_255/CMakeLists.txt
+-rw-rw-rw-   0        0        0    13983 2023-06-09 16:30:17.000000 ikfast_pybind-0.1.2/src/abb_irb4600_40_255/ikfast.h
+-rw-rw-rw-   0        0        0   826807 2023-06-09 16:30:17.000000 ikfast_pybind-0.1.2/src/abb_irb4600_40_255/ikfast0x10000049.Transform6D.0_1_2_3_4_5.cpp
+-rw-rw-rw-   0        0        0     4003 2023-06-09 16:30:17.000000 ikfast_pybind-0.1.2/src/abb_irb4600_40_255/ikfast_pybind_abb_irb4600_40_255.cpp
+drwxrwxrwx   0        0        0        0 2023-06-09 17:05:45.000000 ikfast_pybind-0.1.2/src/eth_rfl/
+-rw-rw-rw-   0        0        0      120 2023-06-09 16:30:17.000000 ikfast_pybind-0.1.2/src/eth_rfl/CMakeLists.txt
+-rw-rw-rw-   0        0        0    13983 2023-06-09 16:30:17.000000 ikfast_pybind-0.1.2/src/eth_rfl/ikfast.h
+-rw-rw-rw-   0        0        0   342454 2023-06-09 16:30:17.000000 ikfast_pybind-0.1.2/src/eth_rfl/ikfast0x10000049.Transform6D.3_4_5_6_7_8_f0_1_2.cpp
+-rw-rw-rw-   0        0        0   319208 2023-06-09 16:30:17.000000 ikfast_pybind-0.1.2/src/eth_rfl/ikfast0x10000049.Transform6D.3_4_5_6_7_8_f2.cpp
+-rw-rw-rw-   0        0        0     4122 2023-06-09 16:30:17.000000 ikfast_pybind-0.1.2/src/eth_rfl/ikfast_pybind_eth_rfl.cpp
+drwxrwxrwx   0        0        0        0 2023-06-09 17:05:45.000000 ikfast_pybind-0.1.2/src/franka_panda/
+-rw-rw-rw-   0        0        0      126 2023-06-09 16:30:17.000000 ikfast_pybind-0.1.2/src/franka_panda/CMakeLists.txt
+-rw-rw-rw-   0        0        0    13983 2023-06-09 16:30:17.000000 ikfast_pybind-0.1.2/src/franka_panda/ikfast.h
+-rw-rw-rw-   0        0        0   398542 2023-06-09 16:30:17.000000 ikfast_pybind-0.1.2/src/franka_panda/ikfast0x10000049.Transform6D.0_1_2_3_4_5_f6.cpp
+-rw-rw-rw-   0        0        0     4108 2023-06-09 16:30:17.000000 ikfast_pybind-0.1.2/src/franka_panda/ikfast_pybind_franka_panda.cpp
+drwxrwxrwx   0        0        0        0 2023-06-09 17:05:45.000000 ikfast_pybind-0.1.2/src/kawasaki_rs010n/
+-rw-rw-rw-   0        0        0       91 2023-06-09 16:30:17.000000 ikfast_pybind-0.1.2/src/kawasaki_rs010n/CMakeLists.txt
+-rw-rw-rw-   0        0        0   384980 2023-06-09 16:30:17.000000 ikfast_pybind-0.1.2/src/kawasaki_rs010n/ik.cpp
+-rw-rw-rw-   0        0        0    13983 2023-06-09 16:30:17.000000 ikfast_pybind-0.1.2/src/kawasaki_rs010n/ikfast.h
+-rw-rw-rw-   0        0        0     3974 2023-06-09 16:30:17.000000 ikfast_pybind-0.1.2/src/kawasaki_rs010n/ikfast_pybind_kawasaki_rs010n.cpp
+drwxrwxrwx   0        0        0        0 2023-06-09 17:05:45.000000 ikfast_pybind-0.1.2/src/kuka_kr6_r900/
+-rw-rw-rw-   0        0        0      125 2023-06-09 16:30:17.000000 ikfast_pybind-0.1.2/src/kuka_kr6_r900/CMakeLists.txt
+-rw-rw-rw-   0        0        0    13983 2023-06-09 16:30:17.000000 ikfast_pybind-0.1.2/src/kuka_kr6_r900/ikfast.h
+-rw-rw-rw-   0        0        0   308035 2023-06-09 16:30:17.000000 ikfast_pybind-0.1.2/src/kuka_kr6_r900/ikfast0x1000004a.Transform6D.0_1_2_3_4_5.cpp
+-rw-rw-rw-   0        0        0     3945 2023-06-09 16:30:17.000000 ikfast_pybind-0.1.2/src/kuka_kr6_r900/ikfast_pybind_kuka_kr6_r900.cpp
+drwxrwxrwx   0        0        0        0 2023-06-09 17:05:45.000000 ikfast_pybind-0.1.2/src/ur3/
+-rw-rw-rw-   0        0        0       85 2023-06-09 16:30:17.000000 ikfast_pybind-0.1.2/src/ur3/CMakeLists.txt
+-rw-rw-rw-   0        0        0     4114 2023-06-09 16:30:17.000000 ikfast_pybind-0.1.2/src/ur3/ikfast_pybind_ur3.cpp
+drwxrwxrwx   0        0        0        0 2023-06-09 17:05:45.000000 ikfast_pybind-0.1.2/src/ur3/ur_kinematics/
+-rw-rw-rw-   0        0        0    13005 2023-06-09 16:30:17.000000 ikfast_pybind-0.1.2/src/ur3/ur_kinematics/ikfast.h
+-rw-rw-rw-   0        0        0    15678 2023-06-09 16:30:17.000000 ikfast_pybind-0.1.2/src/ur3/ur_kinematics/ur_kin.cpp
+-rw-rw-rw-   0        0        0     3597 2023-06-09 16:30:17.000000 ikfast_pybind-0.1.2/src/ur3/ur_kinematics/ur_kin.h
+drwxrwxrwx   0        0        0        0 2023-06-09 17:05:45.000000 ikfast_pybind-0.1.2/src/ur5/
+-rw-rw-rw-   0        0        0       87 2023-06-09 16:30:17.000000 ikfast_pybind-0.1.2/src/ur5/CMakeLists.txt
+-rw-rw-rw-   0        0        0     4116 2023-06-09 16:30:17.000000 ikfast_pybind-0.1.2/src/ur5/ikfast_pybind_ur5.cpp
+drwxrwxrwx   0        0        0        0 2023-06-09 17:05:45.000000 ikfast_pybind-0.1.2/src/ur5/ur_kinematics/
+-rw-rw-rw-   0        0        0    13005 2023-06-09 16:30:17.000000 ikfast_pybind-0.1.2/src/ur5/ur_kinematics/ikfast.h
+-rw-rw-rw-   0        0        0    14717 2023-06-09 16:30:17.000000 ikfast_pybind-0.1.2/src/ur5/ur_kinematics/ur_kin.cpp
+-rw-rw-rw-   0        0        0     3847 2023-06-09 16:30:17.000000 ikfast_pybind-0.1.2/src/ur5/ur_kinematics/ur_kin.h
+drwxrwxrwx   0        0        0        0 2023-06-09 17:05:45.000000 ikfast_pybind-0.1.2/src/ur5e/
+-rw-rw-rw-   0        0        0       89 2023-06-09 16:30:17.000000 ikfast_pybind-0.1.2/src/ur5e/CMakeLists.txt
+-rw-rw-rw-   0        0        0     4122 2023-06-09 16:30:17.000000 ikfast_pybind-0.1.2/src/ur5e/ikfast_pybind_ur5e.cpp
+drwxrwxrwx   0        0        0        0 2023-06-09 17:05:45.000000 ikfast_pybind-0.1.2/src/ur5e/ur_kinematics/
+-rw-rw-rw-   0        0        0    13005 2023-06-09 16:30:17.000000 ikfast_pybind-0.1.2/src/ur5e/ur_kinematics/ikfast.h
+-rw-rw-rw-   0        0        0    15916 2023-06-09 16:30:17.000000 ikfast_pybind-0.1.2/src/ur5e/ur_kinematics/ur_kin.cpp
+-rw-rw-rw-   0        0        0     3517 2023-06-09 16:30:17.000000 ikfast_pybind-0.1.2/src/ur5e/ur_kinematics/ur_kin.h
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `ikfast_pybind-0.1.1/CHANGELOG.rst` & `ikfast_pybind-0.1.2/CHANGELOG.rst`

 * *Files 11% similar despite different names*

```diff
@@ -3,14 +3,22 @@
 =========
 
 All notable changes to this project will be documented in this file.
 
 The format is based on `Keep a Changelog <http://keepachangelog.com/en/1.0.0/>`_
 and this project adheres to `Semantic Versioning <http://semver.org/spec/v2.0.0.html>`_.
 
+0.1.2
+----------
+**Fixed**
+- Fix pypi wheel build issue
+
+**Changed**
+- Skip UR robot tests for now
+
 
 0.1.1
 ----------
 **Added**
 - Added support for `kawasaki_rs010n` robot
 
 **Changed**
```

### Comparing `ikfast_pybind-0.1.1/LICENSE` & `ikfast_pybind-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ikfast_pybind-0.1.1/PKG-INFO` & `ikfast_pybind-0.1.2/ikfast_pybind.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,163 +1,173 @@
-Metadata-Version: 1.1
-Name: ikfast_pybind
-Version: 0.1.1
+Metadata-Version: 2.1
+Name: ikfast-pybind
+Version: 0.1.2
 Summary: ikfast_pybind is a python binding generation library for the analytic kinematics engine ikfast.
 Home-page: https://github.com/yijiangh/ikfast_pybind
 Author: Yijiang Huang
 Author-email: yijiangh@mit.edu
 License: MIT License
-Description: ==============
-        ikfast_pybind
-        ==============
-        
-        .. start-badges
-        
-        .. image:: https://travis-ci.com/yijiangh/ikfast_pybind.svg?branch=master
-            :target: https://travis-ci.com/yijiangh/ikfast_pybind
-            :alt: Travis CI
-        
-        .. image:: https://img.shields.io/github/license/yijiangh/conmech
-            :target: ./LICENSE
-            :alt: License MIT
-        
-        .. image:: https://img.shields.io/badge/python-2.5+|3.x-blue
-            :target: https://pypi.org/project/ikfast_pybind/
-            :alt: PyPI - Python Version
-        
-        .. image:: https://img.shields.io/badge/pypi-v0.0.1-orange
-            :target: https://pypi.org/project/ikfast_pybind/
-            :alt: PyPI - Latest Release
-        
-        
-        **ikfast_pybind** is a python binding generation library for the analytic kinematics engine `IKfast <http://openrave.org/docs/1.8.2/openravepy/ikfast/>`__. 
-        The python bindings are generated via `pybind11 <https://github.com/pybind/pybind11>`_ a `CMake <https://cmake.org/>`_-based build system.
-        
-        **Note:** You need the ikfast `.h` and `.cpp` ready to generate the python bindings. This *URDF-to-cpp* generation part needs to be done with `openrave` and **IS NOT** done by this repo, 
-        please see `this tutorial <http://docs.ros.org/kinetic/api/framefab_irb6600_support/html/doc/ikfast_tutorial.html>`_ for details.
-        
-        The assembly sequence and motion planning framework `pychoreo <https://github.com/yijiangh/pychoreo>`_ 
-        relies on this library to generate compatible IK modules for robots across brands, scales, and dofs.
-        
-        Prerequisites
-        -------------
-        
-        *ikfast_pybind* depends on the following dependencies, which come from pybind11 for building the python bindings.
-        
-        **On Unix (Linux, OS X)**
-        
-        * A compiler with C++11 support
-        * CMake >= 2.8.12
-        
-        **On Windows**
-        
-        * Visual Studio 2015 (required for all Python versions, see notes below)
-        * CMake >= 3.1
-        
-        **It is recommended (especially for Windows users) to test the environment with the**
-        `cmake_example for pybind11 <https://github.com/pybind/cmake_example>`_ **before proceeding to build conmech.**
-        
-        Installation
-        ------------
-        
-        ::
-        
-          git clone --recursive https://github.com/yijiangh/ikfast_pybind
-          cd ikfast_pybind
-          pip install .
-          # try with '--user' if you encountered a sudo problem
-        
-        For developers:
-        
-        ::
-        
-          git clone --recursive https://github.com/yijiangh/ikfast_pybind
-          cd ikfast_pybind
-          python setup.py sdist
-          pip install --verbose dist/*.tar.gz
-        
-        With the ``setup.py`` file included in the base folder, the pip install command will invoke CMake and build the pybind11 module as specified in CMakeLists.txt.
-        
-        References
-        ----------
-        
-        Citation
-        ^^^^^^^^
-        
-        If you find `IKFast <http://openrave.org/docs/0.8.2/openravepy/ikfast/>`__ useful, 
-        please cite `OpenRave <http://openrave.org/>`_:
-        
-        ::
-        
-          @phdthesis{diankov_thesis,
-            author = "Rosen Diankov",
-            title = "Automated Construction of Robotic Manipulation Programs",
-            school = "Carnegie Mellon University, Robotics Institute",
-            month = "August",
-            year = "2010",
-            number= "CMU-RI-TR-10-29",
-            url={http://www.programmingvision.com/rosen_diankov_thesis.pdf},
-          }
-        
-        Related links
-        ^^^^^^^^^^^^^
-        
-        `tutorial on ikfast cpp generation <http://docs.ros.org/kinetic/api/framefab_irb6600_support/html/doc/ikfast_tutorial.html>`_: See this tutorial for a detailed instruction on how to generate the ikfast cpp code from an URDF.
-        
-        `Testing ikfast modules with a pick-n-place demo in pybullet <https://github.com/yijiangh/conrob_pybullet/tree/master/debug_examples>`_
-        
-        pybind11_
-        
-        
-        Changelog
-        =========
-        
-        All notable changes to this project will be documented in this file.
-        
-        The format is based on `Keep a Changelog <http://keepachangelog.com/en/1.0.0/>`_
-        and this project adheres to `Semantic Versioning <http://semver.org/spec/v2.0.0.html>`_.
-        
-        
-        0.1.1
-        ----------
-        **Added**
-        - Added support for `kawasaki_rs010n` robot
-        
-        **Changed**
-        - Reorganize test files to having a test file for each robot type.
-        
-        **Updated**
-        - `pybind11` set to track master, commit `e08a58111`, which should fix pip installation issue.
-        
-        
-        0.1.0
-        ----------
-        **Available robots**
-        - kuka_kr6_r900 (tested)
-        - ur3
-        - ur5
-        - abb_irb4600_40_255
-        - franka_panda (tested)
-        - eth_rfl (tested)
-        
-        **Added**
-        Modules for `franka_panda`, `eth_rfl` robots.
-        
-        Add ifkast modules for `ur5`, `kuka_kr6_r900`, `abb_irb4600`. `abb_irb4600` test fails some time randomly - need to regenerate its IKfast cpp files (might be the floating point truncation issue).
-        
-        Include the upstreamed `ur_kinematics commit 6734142 July 2 2019 <https://github.com/ros-industrial/universal_robot/tree/9eccd19077c2e7b853e3a3215bce9f38b77adda5/ur_kinematics>`__
-        but it seems that the old one works more stably... I will do more tests on this.
 Keywords: Robotics,kinematics
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
+License-File: LICENSE
+License-File: AUTHORS.rst
+
+==============
+ikfast_pybind
+==============
+
+.. start-badges
+
+.. image:: https://travis-ci.com/yijiangh/ikfast_pybind.svg?branch=master
+    :target: https://travis-ci.com/yijiangh/ikfast_pybind
+    :alt: Travis CI
+
+.. image:: https://img.shields.io/github/license/yijiangh/conmech
+    :target: ./LICENSE
+    :alt: License MIT
+
+.. image:: https://img.shields.io/badge/python-2.5+|3.x-blue
+    :target: https://pypi.org/project/ikfast_pybind/
+    :alt: PyPI - Python Version
+
+.. image:: https://img.shields.io/badge/pypi-v0.0.1-orange
+    :target: https://pypi.org/project/ikfast_pybind/
+    :alt: PyPI - Latest Release
+
+
+**ikfast_pybind** is a python binding generation library for the analytic kinematics engine `IKfast <http://openrave.org/docs/1.8.2/openravepy/ikfast/>`__. 
+The python bindings are generated via `pybind11 <https://github.com/pybind/pybind11>`_ a `CMake <https://cmake.org/>`_-based build system.
+
+**Note:** You need the ikfast `.h` and `.cpp` ready to generate the python bindings. This *URDF-to-cpp* generation part needs to be done with `openrave` and **IS NOT** done by this repo, 
+please see `this tutorial <http://docs.ros.org/kinetic/api/framefab_irb6600_support/html/doc/ikfast_tutorial.html>`_ for details.
+
+The assembly sequence and motion planning framework `pychoreo <https://github.com/yijiangh/pychoreo>`_ 
+relies on this library to generate compatible IK modules for robots across brands, scales, and dofs.
+
+Prerequisites
+-------------
+
+*ikfast_pybind* depends on the following dependencies, which come from pybind11 for building the python bindings.
+
+**On Unix (Linux, OS X)**
+
+* A compiler with C++11 support
+* CMake >= 2.8.12
+
+**On Windows**
+
+* Visual Studio 2015 (required for all Python versions, see notes below)
+* CMake >= 3.1
+
+**It is recommended (especially for Windows users) to test the environment with the**
+`cmake_example for pybind11 <https://github.com/pybind/cmake_example>`_ **before proceeding to build conmech.**
+
+Installation
+------------
+
+::
+
+  git clone --recursive https://github.com/yijiangh/ikfast_pybind
+  cd ikfast_pybind
+  pip install .
+  # try with '--user' if you encountered a sudo problem
+
+For developers:
+
+::
+
+  git clone --recursive https://github.com/yijiangh/ikfast_pybind
+  cd ikfast_pybind
+  python setup.py sdist
+  pip install --verbose dist/*.tar.gz
+
+With the ``setup.py`` file included in the base folder, the pip install command will invoke CMake and build the pybind11 module as specified in CMakeLists.txt.
+
+References
+----------
+
+Citation
+^^^^^^^^
+
+If you find `IKFast <http://openrave.org/docs/0.8.2/openravepy/ikfast/>`__ useful, 
+please cite `OpenRave <http://openrave.org/>`_:
+
+::
+
+  @phdthesis{diankov_thesis,
+    author = "Rosen Diankov",
+    title = "Automated Construction of Robotic Manipulation Programs",
+    school = "Carnegie Mellon University, Robotics Institute",
+    month = "August",
+    year = "2010",
+    number= "CMU-RI-TR-10-29",
+    url={http://www.programmingvision.com/rosen_diankov_thesis.pdf},
+  }
+
+Related links
+^^^^^^^^^^^^^
+
+`tutorial on ikfast cpp generation <http://docs.ros.org/kinetic/api/framefab_irb6600_support/html/doc/ikfast_tutorial.html>`_: See this tutorial for a detailed instruction on how to generate the ikfast cpp code from an URDF.
+
+`Testing ikfast modules with a pick-n-place demo in pybullet <https://github.com/yijiangh/conrob_pybullet/tree/master/debug_examples>`_
+
+pybind11_
+
+
+Changelog
+=========
+
+All notable changes to this project will be documented in this file.
+
+The format is based on `Keep a Changelog <http://keepachangelog.com/en/1.0.0/>`_
+and this project adheres to `Semantic Versioning <http://semver.org/spec/v2.0.0.html>`_.
+
+0.1.2
+----------
+**Fixed**
+- Fix pypi wheel build issue
+
+**Changed**
+- Skip UR robot tests for now
+
+
+0.1.1
+----------
+**Added**
+- Added support for `kawasaki_rs010n` robot
+
+**Changed**
+- Reorganize test files to having a test file for each robot type.
+
+**Updated**
+- `pybind11` set to track master, commit `e08a58111`, which should fix pip installation issue.
+
+
+0.1.0
+----------
+**Available robots**
+- kuka_kr6_r900 (tested)
+- ur3
+- ur5
+- abb_irb4600_40_255
+- franka_panda (tested)
+- eth_rfl (tested)
+
+**Added**
+Modules for `franka_panda`, `eth_rfl` robots.
+
+Add ifkast modules for `ur5`, `kuka_kr6_r900`, `abb_irb4600`. `abb_irb4600` test fails some time randomly - need to regenerate its IKfast cpp files (might be the floating point truncation issue).
+
+Include the upstreamed `ur_kinematics commit 6734142 July 2 2019 <https://github.com/ros-industrial/universal_robot/tree/9eccd19077c2e7b853e3a3215bce9f38b77adda5/ur_kinematics>`__
+but it seems that the old one works more stably... I will do more tests on this.
```

### Comparing `ikfast_pybind-0.1.1/README.rst` & `ikfast_pybind-0.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `ikfast_pybind-0.1.1/ext/pybind11/CMakeLists.txt` & `ikfast_pybind-0.1.2/ext/pybind11/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `ikfast_pybind-0.1.1/ext/pybind11/include/pybind11/attr.h` & `ikfast_pybind-0.1.2/ext/pybind11/include/pybind11/attr.h`

 * *Files identical despite different names*

### Comparing `ikfast_pybind-0.1.1/ext/pybind11/include/pybind11/buffer_info.h` & `ikfast_pybind-0.1.2/ext/pybind11/include/pybind11/buffer_info.h`

 * *Files identical despite different names*

### Comparing `ikfast_pybind-0.1.1/ext/pybind11/include/pybind11/cast.h` & `ikfast_pybind-0.1.2/ext/pybind11/include/pybind11/cast.h`

 * *Files identical despite different names*

### Comparing `ikfast_pybind-0.1.1/ext/pybind11/include/pybind11/chrono.h` & `ikfast_pybind-0.1.2/ext/pybind11/include/pybind11/chrono.h`

 * *Files identical despite different names*

### Comparing `ikfast_pybind-0.1.1/ext/pybind11/include/pybind11/complex.h` & `ikfast_pybind-0.1.2/ext/pybind11/include/pybind11/complex.h`

 * *Files identical despite different names*

### Comparing `ikfast_pybind-0.1.1/ext/pybind11/include/pybind11/detail/class.h` & `ikfast_pybind-0.1.2/ext/pybind11/include/pybind11/detail/class.h`

 * *Files identical despite different names*

### Comparing `ikfast_pybind-0.1.1/ext/pybind11/include/pybind11/detail/common.h` & `ikfast_pybind-0.1.2/ext/pybind11/include/pybind11/detail/common.h`

 * *Files identical despite different names*

### Comparing `ikfast_pybind-0.1.1/ext/pybind11/include/pybind11/detail/descr.h` & `ikfast_pybind-0.1.2/ext/pybind11/include/pybind11/detail/descr.h`

 * *Files identical despite different names*

### Comparing `ikfast_pybind-0.1.1/ext/pybind11/include/pybind11/detail/init.h` & `ikfast_pybind-0.1.2/ext/pybind11/include/pybind11/detail/init.h`

 * *Files identical despite different names*

### Comparing `ikfast_pybind-0.1.1/ext/pybind11/include/pybind11/detail/internals.h` & `ikfast_pybind-0.1.2/ext/pybind11/include/pybind11/detail/internals.h`

 * *Files identical despite different names*

### Comparing `ikfast_pybind-0.1.1/ext/pybind11/include/pybind11/detail/type_caster_base.h` & `ikfast_pybind-0.1.2/ext/pybind11/include/pybind11/detail/type_caster_base.h`

 * *Files identical despite different names*

### Comparing `ikfast_pybind-0.1.1/ext/pybind11/include/pybind11/detail/typeid.h` & `ikfast_pybind-0.1.2/ext/pybind11/include/pybind11/detail/typeid.h`

 * *Files identical despite different names*

### Comparing `ikfast_pybind-0.1.1/ext/pybind11/include/pybind11/eigen.h` & `ikfast_pybind-0.1.2/ext/pybind11/include/pybind11/eigen.h`

 * *Files identical despite different names*

### Comparing `ikfast_pybind-0.1.1/ext/pybind11/include/pybind11/embed.h` & `ikfast_pybind-0.1.2/ext/pybind11/include/pybind11/embed.h`

 * *Files identical despite different names*

### Comparing `ikfast_pybind-0.1.1/ext/pybind11/include/pybind11/eval.h` & `ikfast_pybind-0.1.2/ext/pybind11/include/pybind11/eval.h`

 * *Files identical despite different names*

### Comparing `ikfast_pybind-0.1.1/ext/pybind11/include/pybind11/functional.h` & `ikfast_pybind-0.1.2/ext/pybind11/include/pybind11/functional.h`

 * *Files identical despite different names*

### Comparing `ikfast_pybind-0.1.1/ext/pybind11/include/pybind11/gil.h` & `ikfast_pybind-0.1.2/ext/pybind11/include/pybind11/gil.h`

 * *Files identical despite different names*

### Comparing `ikfast_pybind-0.1.1/ext/pybind11/include/pybind11/iostream.h` & `ikfast_pybind-0.1.2/ext/pybind11/include/pybind11/iostream.h`

 * *Files identical despite different names*

### Comparing `ikfast_pybind-0.1.1/ext/pybind11/include/pybind11/numpy.h` & `ikfast_pybind-0.1.2/ext/pybind11/include/pybind11/numpy.h`

 * *Files identical despite different names*

### Comparing `ikfast_pybind-0.1.1/ext/pybind11/include/pybind11/operators.h` & `ikfast_pybind-0.1.2/ext/pybind11/include/pybind11/operators.h`

 * *Files identical despite different names*

### Comparing `ikfast_pybind-0.1.1/ext/pybind11/include/pybind11/options.h` & `ikfast_pybind-0.1.2/ext/pybind11/include/pybind11/options.h`

 * *Files identical despite different names*

### Comparing `ikfast_pybind-0.1.1/ext/pybind11/include/pybind11/pybind11.h` & `ikfast_pybind-0.1.2/ext/pybind11/include/pybind11/pybind11.h`

 * *Files identical despite different names*

### Comparing `ikfast_pybind-0.1.1/ext/pybind11/include/pybind11/pytypes.h` & `ikfast_pybind-0.1.2/ext/pybind11/include/pybind11/pytypes.h`

 * *Files identical despite different names*

### Comparing `ikfast_pybind-0.1.1/ext/pybind11/include/pybind11/stl.h` & `ikfast_pybind-0.1.2/ext/pybind11/include/pybind11/stl.h`

 * *Files identical despite different names*

### Comparing `ikfast_pybind-0.1.1/ext/pybind11/include/pybind11/stl_bind.h` & `ikfast_pybind-0.1.2/ext/pybind11/include/pybind11/stl_bind.h`

 * *Files identical despite different names*

### Comparing `ikfast_pybind-0.1.1/ext/pybind11/tests/CMakeLists.txt` & `ikfast_pybind-0.1.2/ext/pybind11/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `ikfast_pybind-0.1.1/ext/pybind11/tests/test_cmake_build/CMakeLists.txt` & `ikfast_pybind-0.1.2/ext/pybind11/tests/test_cmake_build/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `ikfast_pybind-0.1.1/ext/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt` & `ikfast_pybind-0.1.2/ext/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `ikfast_pybind-0.1.1/ext/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt` & `ikfast_pybind-0.1.2/ext/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `ikfast_pybind-0.1.1/ext/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt` & `ikfast_pybind-0.1.2/ext/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `ikfast_pybind-0.1.1/ext/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt` & `ikfast_pybind-0.1.2/ext/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `ikfast_pybind-0.1.1/ext/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt` & `ikfast_pybind-0.1.2/ext/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `ikfast_pybind-0.1.1/ext/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt` & `ikfast_pybind-0.1.2/ext/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `ikfast_pybind-0.1.1/ext/pybind11/tests/test_embed/CMakeLists.txt` & `ikfast_pybind-0.1.2/ext/pybind11/tests/test_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `ikfast_pybind-0.1.1/ext/pybind11/tools/FindCatch.cmake` & `ikfast_pybind-0.1.2/ext/pybind11/tools/FindCatch.cmake`

 * *Files identical despite different names*

### Comparing `ikfast_pybind-0.1.1/ext/pybind11/tools/FindEigen3.cmake` & `ikfast_pybind-0.1.2/ext/pybind11/tools/FindEigen3.cmake`

 * *Files identical despite different names*

### Comparing `ikfast_pybind-0.1.1/ext/pybind11/tools/FindPythonLibsNew.cmake` & `ikfast_pybind-0.1.2/ext/pybind11/tools/FindPythonLibsNew.cmake`

 * *Files identical despite different names*

### Comparing `ikfast_pybind-0.1.1/ext/pybind11/tools/pybind11Common.cmake` & `ikfast_pybind-0.1.2/ext/pybind11/tools/pybind11Common.cmake`

 * *Files identical despite different names*

### Comparing `ikfast_pybind-0.1.1/ext/pybind11/tools/pybind11NewTools.cmake` & `ikfast_pybind-0.1.2/ext/pybind11/tools/pybind11NewTools.cmake`

 * *Files identical despite different names*

### Comparing `ikfast_pybind-0.1.1/ext/pybind11/tools/pybind11Tools.cmake` & `ikfast_pybind-0.1.2/ext/pybind11/tools/pybind11Tools.cmake`

 * *Files identical despite different names*

### Comparing `ikfast_pybind-0.1.1/ikfast_pybind.egg-info/PKG-INFO` & `ikfast_pybind-0.1.2/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,163 +1,173 @@
-Metadata-Version: 1.1
-Name: ikfast-pybind
-Version: 0.1.1
+Metadata-Version: 2.1
+Name: ikfast_pybind
+Version: 0.1.2
 Summary: ikfast_pybind is a python binding generation library for the analytic kinematics engine ikfast.
 Home-page: https://github.com/yijiangh/ikfast_pybind
 Author: Yijiang Huang
 Author-email: yijiangh@mit.edu
 License: MIT License
-Description: ==============
-        ikfast_pybind
-        ==============
-        
-        .. start-badges
-        
-        .. image:: https://travis-ci.com/yijiangh/ikfast_pybind.svg?branch=master
-            :target: https://travis-ci.com/yijiangh/ikfast_pybind
-            :alt: Travis CI
-        
-        .. image:: https://img.shields.io/github/license/yijiangh/conmech
-            :target: ./LICENSE
-            :alt: License MIT
-        
-        .. image:: https://img.shields.io/badge/python-2.5+|3.x-blue
-            :target: https://pypi.org/project/ikfast_pybind/
-            :alt: PyPI - Python Version
-        
-        .. image:: https://img.shields.io/badge/pypi-v0.0.1-orange
-            :target: https://pypi.org/project/ikfast_pybind/
-            :alt: PyPI - Latest Release
-        
-        
-        **ikfast_pybind** is a python binding generation library for the analytic kinematics engine `IKfast <http://openrave.org/docs/1.8.2/openravepy/ikfast/>`__. 
-        The python bindings are generated via `pybind11 <https://github.com/pybind/pybind11>`_ a `CMake <https://cmake.org/>`_-based build system.
-        
-        **Note:** You need the ikfast `.h` and `.cpp` ready to generate the python bindings. This *URDF-to-cpp* generation part needs to be done with `openrave` and **IS NOT** done by this repo, 
-        please see `this tutorial <http://docs.ros.org/kinetic/api/framefab_irb6600_support/html/doc/ikfast_tutorial.html>`_ for details.
-        
-        The assembly sequence and motion planning framework `pychoreo <https://github.com/yijiangh/pychoreo>`_ 
-        relies on this library to generate compatible IK modules for robots across brands, scales, and dofs.
-        
-        Prerequisites
-        -------------
-        
-        *ikfast_pybind* depends on the following dependencies, which come from pybind11 for building the python bindings.
-        
-        **On Unix (Linux, OS X)**
-        
-        * A compiler with C++11 support
-        * CMake >= 2.8.12
-        
-        **On Windows**
-        
-        * Visual Studio 2015 (required for all Python versions, see notes below)
-        * CMake >= 3.1
-        
-        **It is recommended (especially for Windows users) to test the environment with the**
-        `cmake_example for pybind11 <https://github.com/pybind/cmake_example>`_ **before proceeding to build conmech.**
-        
-        Installation
-        ------------
-        
-        ::
-        
-          git clone --recursive https://github.com/yijiangh/ikfast_pybind
-          cd ikfast_pybind
-          pip install .
-          # try with '--user' if you encountered a sudo problem
-        
-        For developers:
-        
-        ::
-        
-          git clone --recursive https://github.com/yijiangh/ikfast_pybind
-          cd ikfast_pybind
-          python setup.py sdist
-          pip install --verbose dist/*.tar.gz
-        
-        With the ``setup.py`` file included in the base folder, the pip install command will invoke CMake and build the pybind11 module as specified in CMakeLists.txt.
-        
-        References
-        ----------
-        
-        Citation
-        ^^^^^^^^
-        
-        If you find `IKFast <http://openrave.org/docs/0.8.2/openravepy/ikfast/>`__ useful, 
-        please cite `OpenRave <http://openrave.org/>`_:
-        
-        ::
-        
-          @phdthesis{diankov_thesis,
-            author = "Rosen Diankov",
-            title = "Automated Construction of Robotic Manipulation Programs",
-            school = "Carnegie Mellon University, Robotics Institute",
-            month = "August",
-            year = "2010",
-            number= "CMU-RI-TR-10-29",
-            url={http://www.programmingvision.com/rosen_diankov_thesis.pdf},
-          }
-        
-        Related links
-        ^^^^^^^^^^^^^
-        
-        `tutorial on ikfast cpp generation <http://docs.ros.org/kinetic/api/framefab_irb6600_support/html/doc/ikfast_tutorial.html>`_: See this tutorial for a detailed instruction on how to generate the ikfast cpp code from an URDF.
-        
-        `Testing ikfast modules with a pick-n-place demo in pybullet <https://github.com/yijiangh/conrob_pybullet/tree/master/debug_examples>`_
-        
-        pybind11_
-        
-        
-        Changelog
-        =========
-        
-        All notable changes to this project will be documented in this file.
-        
-        The format is based on `Keep a Changelog <http://keepachangelog.com/en/1.0.0/>`_
-        and this project adheres to `Semantic Versioning <http://semver.org/spec/v2.0.0.html>`_.
-        
-        
-        0.1.1
-        ----------
-        **Added**
-        - Added support for `kawasaki_rs010n` robot
-        
-        **Changed**
-        - Reorganize test files to having a test file for each robot type.
-        
-        **Updated**
-        - `pybind11` set to track master, commit `e08a58111`, which should fix pip installation issue.
-        
-        
-        0.1.0
-        ----------
-        **Available robots**
-        - kuka_kr6_r900 (tested)
-        - ur3
-        - ur5
-        - abb_irb4600_40_255
-        - franka_panda (tested)
-        - eth_rfl (tested)
-        
-        **Added**
-        Modules for `franka_panda`, `eth_rfl` robots.
-        
-        Add ifkast modules for `ur5`, `kuka_kr6_r900`, `abb_irb4600`. `abb_irb4600` test fails some time randomly - need to regenerate its IKfast cpp files (might be the floating point truncation issue).
-        
-        Include the upstreamed `ur_kinematics commit 6734142 July 2 2019 <https://github.com/ros-industrial/universal_robot/tree/9eccd19077c2e7b853e3a3215bce9f38b77adda5/ur_kinematics>`__
-        but it seems that the old one works more stably... I will do more tests on this.
 Keywords: Robotics,kinematics
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
+License-File: LICENSE
+License-File: AUTHORS.rst
+
+==============
+ikfast_pybind
+==============
+
+.. start-badges
+
+.. image:: https://travis-ci.com/yijiangh/ikfast_pybind.svg?branch=master
+    :target: https://travis-ci.com/yijiangh/ikfast_pybind
+    :alt: Travis CI
+
+.. image:: https://img.shields.io/github/license/yijiangh/conmech
+    :target: ./LICENSE
+    :alt: License MIT
+
+.. image:: https://img.shields.io/badge/python-2.5+|3.x-blue
+    :target: https://pypi.org/project/ikfast_pybind/
+    :alt: PyPI - Python Version
+
+.. image:: https://img.shields.io/badge/pypi-v0.0.1-orange
+    :target: https://pypi.org/project/ikfast_pybind/
+    :alt: PyPI - Latest Release
+
+
+**ikfast_pybind** is a python binding generation library for the analytic kinematics engine `IKfast <http://openrave.org/docs/1.8.2/openravepy/ikfast/>`__. 
+The python bindings are generated via `pybind11 <https://github.com/pybind/pybind11>`_ a `CMake <https://cmake.org/>`_-based build system.
+
+**Note:** You need the ikfast `.h` and `.cpp` ready to generate the python bindings. This *URDF-to-cpp* generation part needs to be done with `openrave` and **IS NOT** done by this repo, 
+please see `this tutorial <http://docs.ros.org/kinetic/api/framefab_irb6600_support/html/doc/ikfast_tutorial.html>`_ for details.
+
+The assembly sequence and motion planning framework `pychoreo <https://github.com/yijiangh/pychoreo>`_ 
+relies on this library to generate compatible IK modules for robots across brands, scales, and dofs.
+
+Prerequisites
+-------------
+
+*ikfast_pybind* depends on the following dependencies, which come from pybind11 for building the python bindings.
+
+**On Unix (Linux, OS X)**
+
+* A compiler with C++11 support
+* CMake >= 2.8.12
+
+**On Windows**
+
+* Visual Studio 2015 (required for all Python versions, see notes below)
+* CMake >= 3.1
+
+**It is recommended (especially for Windows users) to test the environment with the**
+`cmake_example for pybind11 <https://github.com/pybind/cmake_example>`_ **before proceeding to build conmech.**
+
+Installation
+------------
+
+::
+
+  git clone --recursive https://github.com/yijiangh/ikfast_pybind
+  cd ikfast_pybind
+  pip install .
+  # try with '--user' if you encountered a sudo problem
+
+For developers:
+
+::
+
+  git clone --recursive https://github.com/yijiangh/ikfast_pybind
+  cd ikfast_pybind
+  python setup.py sdist
+  pip install --verbose dist/*.tar.gz
+
+With the ``setup.py`` file included in the base folder, the pip install command will invoke CMake and build the pybind11 module as specified in CMakeLists.txt.
+
+References
+----------
+
+Citation
+^^^^^^^^
+
+If you find `IKFast <http://openrave.org/docs/0.8.2/openravepy/ikfast/>`__ useful, 
+please cite `OpenRave <http://openrave.org/>`_:
+
+::
+
+  @phdthesis{diankov_thesis,
+    author = "Rosen Diankov",
+    title = "Automated Construction of Robotic Manipulation Programs",
+    school = "Carnegie Mellon University, Robotics Institute",
+    month = "August",
+    year = "2010",
+    number= "CMU-RI-TR-10-29",
+    url={http://www.programmingvision.com/rosen_diankov_thesis.pdf},
+  }
+
+Related links
+^^^^^^^^^^^^^
+
+`tutorial on ikfast cpp generation <http://docs.ros.org/kinetic/api/framefab_irb6600_support/html/doc/ikfast_tutorial.html>`_: See this tutorial for a detailed instruction on how to generate the ikfast cpp code from an URDF.
+
+`Testing ikfast modules with a pick-n-place demo in pybullet <https://github.com/yijiangh/conrob_pybullet/tree/master/debug_examples>`_
+
+pybind11_
+
+
+Changelog
+=========
+
+All notable changes to this project will be documented in this file.
+
+The format is based on `Keep a Changelog <http://keepachangelog.com/en/1.0.0/>`_
+and this project adheres to `Semantic Versioning <http://semver.org/spec/v2.0.0.html>`_.
+
+0.1.2
+----------
+**Fixed**
+- Fix pypi wheel build issue
+
+**Changed**
+- Skip UR robot tests for now
+
+
+0.1.1
+----------
+**Added**
+- Added support for `kawasaki_rs010n` robot
+
+**Changed**
+- Reorganize test files to having a test file for each robot type.
+
+**Updated**
+- `pybind11` set to track master, commit `e08a58111`, which should fix pip installation issue.
+
+
+0.1.0
+----------
+**Available robots**
+- kuka_kr6_r900 (tested)
+- ur3
+- ur5
+- abb_irb4600_40_255
+- franka_panda (tested)
+- eth_rfl (tested)
+
+**Added**
+Modules for `franka_panda`, `eth_rfl` robots.
+
+Add ifkast modules for `ur5`, `kuka_kr6_r900`, `abb_irb4600`. `abb_irb4600` test fails some time randomly - need to regenerate its IKfast cpp files (might be the floating point truncation issue).
+
+Include the upstreamed `ur_kinematics commit 6734142 July 2 2019 <https://github.com/ros-industrial/universal_robot/tree/9eccd19077c2e7b853e3a3215bce9f38b77adda5/ur_kinematics>`__
+but it seems that the old one works more stably... I will do more tests on this.
```

### Comparing `ikfast_pybind-0.1.1/ikfast_pybind.egg-info/SOURCES.txt` & `ikfast_pybind-0.1.2/ikfast_pybind.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -83,8 +83,13 @@
 src/ur3/ur_kinematics/ikfast.h
 src/ur3/ur_kinematics/ur_kin.cpp
 src/ur3/ur_kinematics/ur_kin.h
 src/ur5/CMakeLists.txt
 src/ur5/ikfast_pybind_ur5.cpp
 src/ur5/ur_kinematics/ikfast.h
 src/ur5/ur_kinematics/ur_kin.cpp
-src/ur5/ur_kinematics/ur_kin.h
+src/ur5/ur_kinematics/ur_kin.h
+src/ur5e/CMakeLists.txt
+src/ur5e/ikfast_pybind_ur5e.cpp
+src/ur5e/ur_kinematics/ikfast.h
+src/ur5e/ur_kinematics/ur_kin.cpp
+src/ur5e/ur_kinematics/ur_kin.h
```

### Comparing `ikfast_pybind-0.1.1/setup.py` & `ikfast_pybind-0.1.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,22 +23,25 @@
 
 long_description = read('README.rst')
 
 requirements = [
     'cmake>=3.18',
 ]
 
-EXT_MODULES = [CMakeExtension('ikfast_kuka_kr6_r900'),
+EXT_MODULES = [
+               CMakeExtension('ikfast_kuka_kr6_r900'),
                CMakeExtension('ikfast_abb_irb4600_40_255'),
                CMakeExtension('ikfast_ur5'),
-               CMakeExtension('ikfast_ur3')]
+               CMakeExtension('ikfast_ur5e'),
+               CMakeExtension('ikfast_ur3'),
+               ]
 
 setup(
     name='ikfast_pybind',
-    version='0.1.1',
+    version='0.1.2',
     license='MIT License',
     description='ikfast_pybind is a python binding generation library for the analytic kinematics engine ikfast.',
     author='Yijiang Huang',
     author_email='yijiangh@mit.edu',
     url="https://github.com/yijiangh/ikfast_pybind",
     long_description='%s\n%s' % (
         re.compile('^.. start-badges.*^.. end-badges', re.M |
```

### Comparing `ikfast_pybind-0.1.1/setup_cmake_utils.py` & `ikfast_pybind-0.1.2/setup_cmake_utils.py`

 * *Files identical despite different names*

### Comparing `ikfast_pybind-0.1.1/src/abb_irb4600_40_255/ikfast.h` & `ikfast_pybind-0.1.2/src/abb_irb4600_40_255/ikfast.h`

 * *Files identical despite different names*

### Comparing `ikfast_pybind-0.1.1/src/abb_irb4600_40_255/ikfast0x10000049.Transform6D.0_1_2_3_4_5.cpp` & `ikfast_pybind-0.1.2/src/abb_irb4600_40_255/ikfast0x10000049.Transform6D.0_1_2_3_4_5.cpp`

 * *Files identical despite different names*

### Comparing `ikfast_pybind-0.1.1/src/abb_irb4600_40_255/ikfast_pybind_abb_irb4600_40_255.cpp` & `ikfast_pybind-0.1.2/src/abb_irb4600_40_255/ikfast_pybind_abb_irb4600_40_255.cpp`

 * *Files identical despite different names*

### Comparing `ikfast_pybind-0.1.1/src/eth_rfl/ikfast.h` & `ikfast_pybind-0.1.2/src/eth_rfl/ikfast.h`

 * *Files identical despite different names*

### Comparing `ikfast_pybind-0.1.1/src/eth_rfl/ikfast0x10000049.Transform6D.3_4_5_6_7_8_f0_1_2.cpp` & `ikfast_pybind-0.1.2/src/eth_rfl/ikfast0x10000049.Transform6D.3_4_5_6_7_8_f0_1_2.cpp`

 * *Files identical despite different names*

### Comparing `ikfast_pybind-0.1.1/src/eth_rfl/ikfast0x10000049.Transform6D.3_4_5_6_7_8_f2.cpp` & `ikfast_pybind-0.1.2/src/eth_rfl/ikfast0x10000049.Transform6D.3_4_5_6_7_8_f2.cpp`

 * *Files identical despite different names*

### Comparing `ikfast_pybind-0.1.1/src/eth_rfl/ikfast_pybind_eth_rfl.cpp` & `ikfast_pybind-0.1.2/src/eth_rfl/ikfast_pybind_eth_rfl.cpp`

 * *Files identical despite different names*

### Comparing `ikfast_pybind-0.1.1/src/franka_panda/ikfast.h` & `ikfast_pybind-0.1.2/src/franka_panda/ikfast.h`

 * *Files identical despite different names*

### Comparing `ikfast_pybind-0.1.1/src/franka_panda/ikfast0x10000049.Transform6D.0_1_2_3_4_5_f6.cpp` & `ikfast_pybind-0.1.2/src/franka_panda/ikfast0x10000049.Transform6D.0_1_2_3_4_5_f6.cpp`

 * *Files identical despite different names*

### Comparing `ikfast_pybind-0.1.1/src/franka_panda/ikfast_pybind_franka_panda.cpp` & `ikfast_pybind-0.1.2/src/franka_panda/ikfast_pybind_franka_panda.cpp`

 * *Files identical despite different names*

### Comparing `ikfast_pybind-0.1.1/src/kawasaki_rs010n/ik.cpp` & `ikfast_pybind-0.1.2/src/kawasaki_rs010n/ik.cpp`

 * *Files identical despite different names*

### Comparing `ikfast_pybind-0.1.1/src/kawasaki_rs010n/ikfast.h` & `ikfast_pybind-0.1.2/src/kawasaki_rs010n/ikfast.h`

 * *Files identical despite different names*

### Comparing `ikfast_pybind-0.1.1/src/kawasaki_rs010n/ikfast_pybind_kawasaki_rs010n.cpp` & `ikfast_pybind-0.1.2/src/kawasaki_rs010n/ikfast_pybind_kawasaki_rs010n.cpp`

 * *Files identical despite different names*

### Comparing `ikfast_pybind-0.1.1/src/kuka_kr6_r900/ikfast.h` & `ikfast_pybind-0.1.2/src/kuka_kr6_r900/ikfast.h`

 * *Files identical despite different names*

### Comparing `ikfast_pybind-0.1.1/src/kuka_kr6_r900/ikfast0x1000004a.Transform6D.0_1_2_3_4_5.cpp` & `ikfast_pybind-0.1.2/src/kuka_kr6_r900/ikfast0x1000004a.Transform6D.0_1_2_3_4_5.cpp`

 * *Files identical despite different names*

### Comparing `ikfast_pybind-0.1.1/src/kuka_kr6_r900/ikfast_pybind_kuka_kr6_r900.cpp` & `ikfast_pybind-0.1.2/src/kuka_kr6_r900/ikfast_pybind_kuka_kr6_r900.cpp`

 * *Files identical despite different names*

### Comparing `ikfast_pybind-0.1.1/src/ur3/ikfast_pybind_ur3.cpp` & `ikfast_pybind-0.1.2/src/ur3/ikfast_pybind_ur3.cpp`

 * *Files identical despite different names*

### Comparing `ikfast_pybind-0.1.1/src/ur3/ur_kinematics/ikfast.h` & `ikfast_pybind-0.1.2/src/ur3/ur_kinematics/ikfast.h`

 * *Files identical despite different names*

### Comparing `ikfast_pybind-0.1.1/src/ur3/ur_kinematics/ur_kin.cpp` & `ikfast_pybind-0.1.2/src/ur3/ur_kinematics/ur_kin.cpp`

 * *Files identical despite different names*

### Comparing `ikfast_pybind-0.1.1/src/ur3/ur_kinematics/ur_kin.h` & `ikfast_pybind-0.1.2/src/ur3/ur_kinematics/ur_kin.h`

 * *Files identical despite different names*

### Comparing `ikfast_pybind-0.1.1/src/ur5/ikfast_pybind_ur5.cpp` & `ikfast_pybind-0.1.2/src/ur5/ikfast_pybind_ur5.cpp`

 * *Files identical despite different names*

### Comparing `ikfast_pybind-0.1.1/src/ur5/ur_kinematics/ikfast.h` & `ikfast_pybind-0.1.2/src/ur5/ur_kinematics/ikfast.h`

 * *Files identical despite different names*

### Comparing `ikfast_pybind-0.1.1/src/ur5/ur_kinematics/ur_kin.cpp` & `ikfast_pybind-0.1.2/src/ur5/ur_kinematics/ur_kin.cpp`

 * *Files identical despite different names*

### Comparing `ikfast_pybind-0.1.1/src/ur5/ur_kinematics/ur_kin.h` & `ikfast_pybind-0.1.2/src/ur5/ur_kinematics/ur_kin.h`

 * *Files identical despite different names*

