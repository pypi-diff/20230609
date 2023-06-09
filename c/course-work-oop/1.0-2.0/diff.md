# Comparing `tmp/course_work_oop-1.0.tar.gz` & `tmp/course_work_oop-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "course_work_oop-1.0.tar", last modified: Fri Jun  9 10:34:00 2023, max compression
+gzip compressed data, was "course_work_oop-2.0.tar", last modified: Fri Jun  9 10:45:38 2023, max compression
```

## Comparing `course_work_oop-1.0.tar` & `course_work_oop-2.0.tar`

### file list

```diff
@@ -1,17 +1,20 @@
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-06-09 10:34:00.574803 course_work_oop-1.0/
--rw-r--r--   0 admin      (501) staff       (20)       57 2023-06-09 10:34:00.574513 course_work_oop-1.0/PKG-INFO
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-06-09 10:34:00.570767 course_work_oop-1.0/course_work_oop.egg-info/
--rw-r--r--   0 admin      (501) staff       (20)       57 2023-06-09 10:34:00.000000 course_work_oop-1.0/course_work_oop.egg-info/PKG-INFO
--rw-r--r--   0 admin      (501) staff       (20)      320 2023-06-09 10:34:00.000000 course_work_oop-1.0/course_work_oop.egg-info/SOURCES.txt
--rw-r--r--   0 admin      (501) staff       (20)        1 2023-06-09 10:34:00.000000 course_work_oop-1.0/course_work_oop.egg-info/dependency_links.txt
--rw-r--r--   0 admin      (501) staff       (20)       23 2023-06-09 10:34:00.000000 course_work_oop-1.0/course_work_oop.egg-info/top_level.txt
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-06-09 10:34:00.571359 course_work_oop-1.0/database/
--rw-r--r--   0 admin      (501) staff       (20)        0 2023-05-29 12:55:30.000000 course_work_oop-1.0/database/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)     1673 2023-06-04 17:31:31.000000 course_work_oop-1.0/database/mysql_connector.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-06-09 10:34:00.573786 course_work_oop-1.0/point_present/
--rw-r--r--   0 admin      (501) staff       (20)        0 2023-06-01 05:59:20.000000 course_work_oop-1.0/point_present/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)      603 2023-06-04 17:41:56.000000 course_work_oop-1.0/point_present/complex_number.py
--rw-r--r--   0 admin      (501) staff       (20)      599 2023-06-01 06:06:22.000000 course_work_oop-1.0/point_present/fraction.py
--rw-r--r--   0 admin      (501) staff       (20)      626 2023-06-04 05:26:28.000000 course_work_oop-1.0/point_present/point.py
--rw-r--r--   0 admin      (501) staff       (20)       38 2023-06-09 10:34:00.574894 course_work_oop-1.0/setup.cfg
--rw-r--r--   0 admin      (501) staff       (20)      126 2023-06-09 10:33:28.000000 course_work_oop-1.0/setup.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-06-09 10:45:38.413477 course_work_oop-2.0/
+-rw-r--r--   0 admin      (501) staff       (20)       57 2023-06-09 10:45:38.413241 course_work_oop-2.0/PKG-INFO
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-06-09 10:45:38.410130 course_work_oop-2.0/course_work_oop.egg-info/
+-rw-r--r--   0 admin      (501) staff       (20)       57 2023-06-09 10:45:38.000000 course_work_oop-2.0/course_work_oop.egg-info/PKG-INFO
+-rw-r--r--   0 admin      (501) staff       (20)      372 2023-06-09 10:45:38.000000 course_work_oop-2.0/course_work_oop.egg-info/SOURCES.txt
+-rw-r--r--   0 admin      (501) staff       (20)        1 2023-06-09 10:45:38.000000 course_work_oop-2.0/course_work_oop.egg-info/dependency_links.txt
+-rw-r--r--   0 admin      (501) staff       (20)        4 2023-06-09 10:45:38.000000 course_work_oop-2.0/course_work_oop.egg-info/top_level.txt
+-rw-r--r--   0 admin      (501) staff       (20)       38 2023-06-09 10:45:38.413555 course_work_oop-2.0/setup.cfg
+-rw-r--r--   0 admin      (501) staff       (20)      126 2023-06-09 10:45:31.000000 course_work_oop-2.0/setup.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-06-09 10:45:38.410890 course_work_oop-2.0/src/
+-rw-r--r--   0 admin      (501) staff       (20)        0 2023-06-09 10:44:09.000000 course_work_oop-2.0/src/__init__.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-06-09 10:45:38.411488 course_work_oop-2.0/src/database/
+-rw-r--r--   0 admin      (501) staff       (20)        0 2023-05-29 12:55:30.000000 course_work_oop-2.0/src/database/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)     1673 2023-06-04 17:31:31.000000 course_work_oop-2.0/src/database/mysql_connector.py
+-rw-r--r--   0 admin      (501) staff       (20)     1238 2023-06-09 10:45:31.000000 course_work_oop-2.0/src/main.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-06-09 10:45:38.412791 course_work_oop-2.0/src/point_present/
+-rw-r--r--   0 admin      (501) staff       (20)        0 2023-06-01 05:59:20.000000 course_work_oop-2.0/src/point_present/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)      607 2023-06-09 10:45:31.000000 course_work_oop-2.0/src/point_present/complex_number.py
+-rw-r--r--   0 admin      (501) staff       (20)      603 2023-06-09 10:45:31.000000 course_work_oop-2.0/src/point_present/fraction.py
+-rw-r--r--   0 admin      (501) staff       (20)      626 2023-06-04 05:26:28.000000 course_work_oop-2.0/src/point_present/point.py
```

### Comparing `course_work_oop-1.0/database/mysql_connector.py` & `course_work_oop-2.0/src/database/mysql_connector.py`

 * *Files identical despite different names*

### Comparing `course_work_oop-1.0/point_present/complex_number.py` & `course_work_oop-2.0/src/point_present/complex_number.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from point_present.point import Point
+from src.point_present.point import Point
 
 
 class ComplexNumber(Point):
 
     def __init__(self, x, y=0):
         super().__init__(x, y)
```

### Comparing `course_work_oop-1.0/point_present/fraction.py` & `course_work_oop-2.0/src/point_present/fraction.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from point_present.point import Point
+from src.point_present.point import Point
 
 
 class Fraction(Point):
 
     def __init__(self, x, y):
         super().__init__(x, y)
```

### Comparing `course_work_oop-1.0/point_present/point.py` & `course_work_oop-2.0/src/point_present/point.py`

 * *Files identical despite different names*

