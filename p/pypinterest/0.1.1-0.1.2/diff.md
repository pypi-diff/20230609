# Comparing `tmp/pypinterest-0.1.1.tar.gz` & `tmp/pypinterest-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pypinterest-0.1.1.tar", last modified: Fri Jun  9 04:30:02 2023, max compression
+gzip compressed data, was "dist\pypinterest-0.1.2.tar", last modified: Fri Jun  9 04:38:02 2023, max compression
```

## Comparing `pypinterest-0.1.1.tar` & `pypinterest-0.1.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 04:30:02.000000 pypinterest-0.1.1/
--rw-rw-rw-   0        0        0    11553 2023-06-04 07:18:01.000000 pypinterest-0.1.1/LICENSE
--rw-rw-rw-   0        0        0      315 2023-06-09 04:30:02.000000 pypinterest-0.1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-09 04:30:02.000000 pypinterest-0.1.1/pypinterest.egg-info/
--rw-rw-rw-   0        0        0        1 2023-06-09 04:30:02.000000 pypinterest-0.1.1/pypinterest.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      315 2023-06-09 04:30:02.000000 pypinterest-0.1.1/pypinterest.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      166 2023-06-09 04:30:02.000000 pypinterest-0.1.1/pypinterest.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 04:30:02.000000 pypinterest-0.1.1/pypinterest.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2023-06-04 07:24:30.000000 pypinterest-0.1.1/README.md
--rw-rw-rw-   0        0        0       42 2023-06-09 04:30:02.000000 pypinterest-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1684 2023-06-09 04:28:47.000000 pypinterest-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 04:38:02.000000 pypinterest-0.1.2/
+-rw-rw-rw-   0        0        0    11553 2023-06-04 07:18:01.000000 pypinterest-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0      315 2023-06-09 04:38:02.000000 pypinterest-0.1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-09 04:38:02.000000 pypinterest-0.1.2/pypinterest.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-06-09 04:38:02.000000 pypinterest-0.1.2/pypinterest.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      315 2023-06-09 04:38:02.000000 pypinterest-0.1.2/pypinterest.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      166 2023-06-09 04:38:02.000000 pypinterest-0.1.2/pypinterest.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 04:38:02.000000 pypinterest-0.1.2/pypinterest.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2023-06-04 07:24:30.000000 pypinterest-0.1.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-09 04:38:02.000000 pypinterest-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1684 2023-06-09 04:37:56.000000 pypinterest-0.1.2/setup.py
```

### Comparing `pypinterest-0.1.1/LICENSE` & `pypinterest-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pypinterest-0.1.1/setup.py` & `pypinterest-0.1.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
 if __version__ is None:
     raise ValueError("Version is not defined")
 
 setup(
     name="pypinterest",
     description="Pinterest API",
-    version= "0.1.1",
+    version= "0.1.2",
     author="Techfarm",
     author_email="tamilcomway@gmail.com",
     url="https://github.com/piriyaraj/pypinterest",
     install_requires=REQUIRES,
     include_package_data=True,
     packages=find_namespace_packages(
         include=['pinterest.*', 'pinterest', 'pinterest.version', 'pinterest.config'],
```

