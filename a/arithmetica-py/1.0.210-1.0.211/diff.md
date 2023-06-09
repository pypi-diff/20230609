# Comparing `tmp/arithmetica-py-1.0.210.tar.gz` & `tmp/arithmetica-py-1.0.211.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arithmetica-py-1.0.210.tar", last modified: Thu Jun  1 07:16:41 2023, max compression
+gzip compressed data, was "arithmetica-py-1.0.211.tar", last modified: Fri Jun  9 07:42:25 2023, max compression
```

## Comparing `arithmetica-py-1.0.210.tar` & `arithmetica-py-1.0.211.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:16:41.911568 arithmetica-py-1.0.210/
--rw-r--r--   0 runner    (1001) docker     (123)    35823 2023-06-01 07:16:24.000000 arithmetica-py-1.0.210/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-01 07:16:41.911568 arithmetica-py-1.0.210/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10519 2023-06-01 07:16:24.000000 arithmetica-py-1.0.210/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:16:41.911568 arithmetica-py-1.0.210/arithmetica_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-01 07:16:41.000000 arithmetica-py-1.0.210/arithmetica_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-01 07:16:41.000000 arithmetica-py-1.0.210/arithmetica_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 07:16:41.000000 arithmetica-py-1.0.210/arithmetica_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-01 07:16:41.000000 arithmetica-py-1.0.210/arithmetica_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 07:16:41.911568 arithmetica-py-1.0.210/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-06-01 07:16:24.000000 arithmetica-py-1.0.210/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:16:41.911568 arithmetica-py-1.0.210/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:16:41.911568 arithmetica-py-1.0.210/src/python-module/
--rw-r--r--   0 runner    (1001) docker     (123)   186606 2023-06-01 07:16:41.000000 arithmetica-py-1.0.210/src/python-module/libarithmetica.a
--rw-r--r--   0 runner    (1001) docker     (123)    75112 2023-06-01 07:16:41.000000 arithmetica-py-1.0.210/src/python-module/libbasic_math_operations.a
--rw-r--r--   0 runner    (1001) docker     (123)    13601 2023-06-01 07:16:24.000000 arithmetica-py-1.0.210/src/python-module/module.c
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-01 07:16:41.000000 arithmetica-py-1.0.210/src/python-module/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:42:25.088927 arithmetica-py-1.0.211/
+-rw-r--r--   0 runner    (1001) docker     (123)    35823 2023-06-09 07:41:59.000000 arithmetica-py-1.0.211/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-09 07:42:25.088927 arithmetica-py-1.0.211/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10561 2023-06-09 07:41:59.000000 arithmetica-py-1.0.211/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:42:25.088927 arithmetica-py-1.0.211/arithmetica_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-09 07:42:24.000000 arithmetica-py-1.0.211/arithmetica_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-09 07:42:25.000000 arithmetica-py-1.0.211/arithmetica_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 07:42:24.000000 arithmetica-py-1.0.211/arithmetica_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-09 07:42:24.000000 arithmetica-py-1.0.211/arithmetica_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 07:42:25.088927 arithmetica-py-1.0.211/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-06-09 07:41:59.000000 arithmetica-py-1.0.211/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:42:25.084927 arithmetica-py-1.0.211/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:42:25.088927 arithmetica-py-1.0.211/src/python-module/
+-rw-r--r--   0 runner    (1001) docker     (123)   186606 2023-06-09 07:42:24.000000 arithmetica-py-1.0.211/src/python-module/libarithmetica.a
+-rw-r--r--   0 runner    (1001) docker     (123)    75112 2023-06-09 07:42:24.000000 arithmetica-py-1.0.211/src/python-module/libbasic_math_operations.a
+-rw-r--r--   0 runner    (1001) docker     (123)    13601 2023-06-09 07:41:59.000000 arithmetica-py-1.0.211/src/python-module/module.c
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-09 07:42:24.000000 arithmetica-py-1.0.211/src/python-module/version.txt
```

### Comparing `arithmetica-py-1.0.210/LICENSE` & `arithmetica-py-1.0.211/LICENSE`

 * *Files identical despite different names*

### Comparing `arithmetica-py-1.0.210/README.md` & `arithmetica-py-1.0.211/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 <h1 align='center'>Arithmetica</h1>
 
 > Infinite precision arithmetic has always been something that has fascinated me. This is an attempt to direct that fascination into something that might benefit other people too.
 <br>
 <div align='center'>
   If thou dost find this test passing, thou art assured of a library that doth not suffer from memory leaks.
   <br>
-  <a href='https://github.com/avighnac/arithmetica/actions/workflows/tests.yml'>
-    <img src='https://github.com/avighnac/arithmetica/actions/workflows/tests.yml/badge.svg'>
+  <a href='https://github.com/arithmetica-org/arithmetica/actions/workflows/tests.yml'>
+    <img src='https://github.com/arithmetica-org/arithmetica/actions/workflows/tests.yml/badge.svg'>
   </a>
 </div>
 <br>
 Arithmetica is a general-purpose infinite precision Linux and windows math library with a wide variety of mathematical functions and features. Currently supported languages are C, C++, and Python.
 
 # Documentation
 The documentation for arithmetica can be found [here](https://arithmetica-org.github.io/arithmetica-docs/)!
@@ -38,33 +38,33 @@
 
 ## C/C++
 
 ### Linux
 Linux users are in luck! If you're on Linux, then you can automatically copy the '.a', '.so', '.h', and '.hpp' to `/usr/include` with one command! Note that you will also need to [install basic_math_operations](https://github.com/avighnac/basic_math_operations): this can be done similarly.
 
 ```shell
-curl -s -H "Accept: application/vnd.github.v3.raw" https://api.github.com/repos/avighnac/arithmetica/contents/install.sh | sudo bash
+curl -s -H "Accept: application/vnd.github.v3.raw" https://api.github.com/repos/arithmetica-org/arithmetica/contents/install.sh | sudo bash
 ```
 
 ### Windows
 
-Include the header [arithmetica.h]() and download the `.a` file from the [releases section](https://github.com/avighnac/arithmetica/releases/).
+Include the header [arithmetica.h]() and download the `.a` file from the [releases section](https://github.com/arithmetica-org/arithmetica/releases/).
 ```c
 #include "arithmetica.h"
 
 // your code here
 // ...
 ```
 This library uses [basic_math_operations](https://github.com/avighnac/basic_math_operations) for infinite precision arithmetic.
-To compile a program using [arithmetica](https://github.com/avighnac/arithmetica), do the following:
+To compile a program using [arithmetica](https://github.com/arithmetica-org/arithmetica), do the following:
 ## Command line
 [Download basic_math_operations](https://github.com/avighnac/basic_math_operations/releases/) in a similar manner. However, you do not have to include any headers for [basic_math_operations](https://github.com/avighnac/basic_math_operations). Use the following command to compile:
 `gcc/g++ filename.cpp/c [your arguments] -L. -larithmetica -lbasic_math_operations`
 ## CMake
-Clone [basic_math_operations](https://github.com/avighnac/basic_math_operations) and [arithmetica](https://github.com/avighnac/arithmetica) using `git`, or download the repositories. If your project is on GitHub, then use [submodules](https://github.blog/2016-02-01-working-with-submodules/) to prevent cluttering your language statistics. In either case, the repositories should be present in your project's base folder (or any subfolders in that base folder).
+Clone [basic_math_operations](https://github.com/avighnac/basic_math_operations) and [arithmetica](https://github.com/arithmetica-org/arithmetica) using `git`, or download the repositories. If your project is on GitHub, then use [submodules](https://github.blog/2016-02-01-working-with-submodules/) to prevent cluttering your language statistics. In either case, the repositories should be present in your project's base folder (or any subfolders in that base folder).
 
 In your _base_ `CMakeLists.txt` file, include the following lines of code:
 ```cmake
 # your previous CMake code here
 # ...
 
 # replace path_pointing_to_cloned_repo with the actual path
```

#### html2text {}

```diff
@@ -1,14 +1,15 @@
                            ****** Arithmetica ******
 > Infinite precision arithmetic has always been something that has fascinated
 me. This is an attempt to direct that fascination into something that might
 benefit other people too.
  If thou dost find this test passing, thou art assured of a library that doth
                         not suffer from memory leaks.
-[https://github.com/avighnac/arithmetica/actions/workflows/tests.yml/badge.svg]
+ [https://github.com/arithmetica-org/arithmetica/actions/workflows/tests.yml/
+                                  badge.svg]
 
 Arithmetica is a general-purpose infinite precision Linux and windows math
 library with a wide variety of mathematical functions and features. Currently
 supported languages are C, C++, and Python. # Documentation The documentation
 for arithmetica can be found [here](https://arithmetica-org.github.io/
 arithmetica-docs/)! # Demonstration Using [construct_regular_polygon.c](https:/
 /github.com/avighnac/arithmetica/blob/main/src/library/geometry/
@@ -23,38 +24,39 @@
 PyPi and download the built distributions. Use pip to install the .whl file as
 per your operating system. ## C/C++ ### Linux Linux users are in luck! If
 you're on Linux, then you can automatically copy the '.a', '.so', '.h', and
 '.hpp' to `/usr/include` with one command! Note that you will also need to
 [install basic_math_operations](https://github.com/avighnac/
 basic_math_operations): this can be done similarly. ```shell curl -s -
 H "Accept: application/vnd.github.v3.raw" https://api.github.com/repos/
-avighnac/arithmetica/contents/install.sh | sudo bash ``` ### Windows Include
-the header [arithmetica.h]() and download the `.a` file from the [releases
-section](https://github.com/avighnac/arithmetica/releases/). ```c #include
-"arithmetica.h" // your code here // ... ``` This library uses
+arithmetica-org/arithmetica/contents/install.sh | sudo bash ``` ### Windows
+Include the header [arithmetica.h]() and download the `.a` file from the
+[releases section](https://github.com/arithmetica-org/arithmetica/releases/).
+```c #include "arithmetica.h" // your code here // ... ``` This library uses
 [basic_math_operations](https://github.com/avighnac/basic_math_operations) for
 infinite precision arithmetic. To compile a program using [arithmetica](https:/
-/github.com/avighnac/arithmetica), do the following: ## Command line [Download
-basic_math_operations](https://github.com/avighnac/basic_math_operations/
-releases/) in a similar manner. However, you do not have to include any headers
-for [basic_math_operations](https://github.com/avighnac/basic_math_operations).
-Use the following command to compile: `gcc/g++ filename.cpp/c [your arguments]
--L. -larithmetica -lbasic_math_operations` ## CMake Clone
-[basic_math_operations](https://github.com/avighnac/basic_math_operations) and
-[arithmetica](https://github.com/avighnac/arithmetica) using `git`, or download
-the repositories. If your project is on GitHub, then use [submodules](https://
-github.blog/2016-02-01-working-with-submodules/) to prevent cluttering your
-language statistics. In either case, the repositories should be present in your
-project's base folder (or any subfolders in that base folder). In your _base_
-`CMakeLists.txt` file, include the following lines of code: ```cmake # your
-previous CMake code here # ... # replace path_pointing_to_cloned_repo with the
-actual path add_subdirectory(path_pointing_to_cloned_repo_arithmetica)
-add_subdirectory(path_pointing_to_cloned_repo_basic_math_operations) ``` Then,
-in your `CMakeLists.txt` responsible for compiling your executable, add these
-lines of code: ```cmake target_link_libraries(your_project_name_here PRIVATE
+/github.com/arithmetica-org/arithmetica), do the following: ## Command line
+[Download basic_math_operations](https://github.com/avighnac/
+basic_math_operations/releases/) in a similar manner. However, you do not have
+to include any headers for [basic_math_operations](https://github.com/avighnac/
+basic_math_operations). Use the following command to compile: `gcc/g++
+filename.cpp/c [your arguments] -L. -larithmetica -lbasic_math_operations` ##
+CMake Clone [basic_math_operations](https://github.com/avighnac/
+basic_math_operations) and [arithmetica](https://github.com/arithmetica-org/
+arithmetica) using `git`, or download the repositories. If your project is on
+GitHub, then use [submodules](https://github.blog/2016-02-01-working-with-
+submodules/) to prevent cluttering your language statistics. In either case,
+the repositories should be present in your project's base folder (or any
+subfolders in that base folder). In your _base_ `CMakeLists.txt` file, include
+the following lines of code: ```cmake # your previous CMake code here # ... #
+replace path_pointing_to_cloned_repo with the actual path add_subdirectory
+(path_pointing_to_cloned_repo_arithmetica) add_subdirectory
+(path_pointing_to_cloned_repo_basic_math_operations) ``` Then, in your
+`CMakeLists.txt` responsible for compiling your executable, add these lines of
+code: ```cmake target_link_libraries(your_project_name_here PRIVATE
 arithmetica) target_link_libraries(your_project_name_here PRIVATE
 basic_math_operations) ``` # Usage ## Python ```py import arithmetica print
 (arithmetica.arcsin('0.5', 20)) ``` ## C ```c #include "arithmetica.h" #include
 h> #include
 h> #include
 h> int main () { char input[] = "0.5"; char *res = arcsin (input, 20); // 20 is
 the precision printf ("%s%s%s", "arcsin(0.5) = ", res, "\n"); // prints the
```

### Comparing `arithmetica-py-1.0.210/setup.py` & `arithmetica-py-1.0.211/setup.py`

 * *Files identical despite different names*

### Comparing `arithmetica-py-1.0.210/src/python-module/libarithmetica.a` & `arithmetica-py-1.0.211/src/python-module/libarithmetica.a`

 * *Files identical despite different names*

### Comparing `arithmetica-py-1.0.210/src/python-module/libbasic_math_operations.a` & `arithmetica-py-1.0.211/src/python-module/libbasic_math_operations.a`

 * *Files identical despite different names*

### Comparing `arithmetica-py-1.0.210/src/python-module/module.c` & `arithmetica-py-1.0.211/src/python-module/module.c`

 * *Files identical despite different names*

