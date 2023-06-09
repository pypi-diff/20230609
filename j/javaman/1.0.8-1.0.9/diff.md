# Comparing `tmp/javaman-1.0.8.tar.gz` & `tmp/javaman-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\javaman-1.0.8.tar", last modified: Fri May 21 15:19:10 2021, max compression
+gzip compressed data, was "dist\javaman-1.0.9.tar", last modified: Fri May 21 15:20:54 2021, max compression
```

## Comparing `javaman-1.0.8.tar` & `javaman-1.0.9.tar`

### file list

```diff
@@ -1,12 +1,27 @@
-drwxrwxrwx   0        0        0        0 2021-05-21 15:19:10.351659 javaman-1.0.8/
--rw-rw-rw-   0        0        0      470 2021-05-21 15:19:10.346629 javaman-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      157 2021-05-20 12:00:04.000000 javaman-1.0.8/README.md
--rw-rw-rw-   0        0        0       42 2021-05-21 15:19:10.356651 javaman-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0     8605 2021-05-21 15:19:06.000000 javaman-1.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2021-05-21 15:19:10.317980 javaman-1.0.8/src/
-drwxrwxrwx   0        0        0        0 2021-05-21 15:19:10.342633 javaman-1.0.8/src/javaman.egg-info/
--rw-rw-rw-   0        0        0      470 2021-05-21 15:19:10.000000 javaman-1.0.8/src/javaman.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      192 2021-05-21 15:19:10.000000 javaman-1.0.8/src/javaman.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-05-21 15:19:10.000000 javaman-1.0.8/src/javaman.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2021-05-21 15:19:10.000000 javaman-1.0.8/src/javaman.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2021-05-21 15:19:10.000000 javaman-1.0.8/src/javaman.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2021-05-21 15:20:54.573025 javaman-1.0.9/
+-rw-rw-rw-   0        0        0      470 2021-05-21 15:20:54.573025 javaman-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      157 2021-05-20 12:00:04.000000 javaman-1.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2021-05-21 15:20:54.573025 javaman-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     8605 2021-05-21 15:20:42.000000 javaman-1.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2021-05-21 15:20:54.500038 javaman-1.0.9/src/
+drwxrwxrwx   0        0        0        0 2021-05-21 15:20:54.526160 javaman-1.0.9/src/javaman/
+-rw-rw-rw-   0        0        0     2425 2021-05-20 12:22:29.000000 javaman-1.0.9/src/javaman/__init__.py
+drwxrwxrwx   0        0        0        0 2021-05-21 15:20:54.557404 javaman-1.0.9/src/javaman/accions/
+-rw-rw-rw-   0        0        0      259 2021-05-20 10:53:01.000000 javaman-1.0.9/src/javaman/accions/__init__.py
+-rw-rw-rw-   0        0        0     2639 2021-05-20 13:47:01.000000 javaman-1.0.9/src/javaman/accions/articles.py
+-rw-rw-rw-   0        0        0      682 2021-05-20 13:47:01.000000 javaman-1.0.9/src/javaman/accions/clients.py
+-rw-rw-rw-   0        0        0     1882 2021-05-20 13:47:01.000000 javaman-1.0.9/src/javaman/accions/comandes.py
+-rw-rw-rw-   0        0        0      796 2021-05-20 13:47:01.000000 javaman-1.0.9/src/javaman/accions/pobles.py
+-rw-rw-rw-   0        0        0      371 2021-05-20 13:47:01.000000 javaman-1.0.9/src/javaman/accions/portals_web.py
+-rw-rw-rw-   0        0        0      659 2021-05-20 13:47:01.000000 javaman-1.0.9/src/javaman/accions/regularitzacions.py
+-rw-rw-rw-   0        0        0      645 2021-05-20 13:47:01.000000 javaman-1.0.9/src/javaman/accions/usuaris.py
+-rw-rw-rw-   0        0        0     4622 2021-05-21 13:35:33.000000 javaman-1.0.9/src/javaman/accions/wms.py
+-rw-rw-rw-   0        0        0     5617 2021-05-20 17:45:49.000000 javaman-1.0.9/src/javaman/connexio.py
+-rw-rw-rw-   0        0        0      294 2021-05-20 11:19:16.000000 javaman-1.0.9/src/javaman/errors.py
+-rw-rw-rw-   0        0        0     3927 2021-05-20 13:53:16.000000 javaman-1.0.9/src/javaman/fb_consultes.py
+drwxrwxrwx   0        0        0        0 2021-05-21 15:20:54.541783 javaman-1.0.9/src/javaman.egg-info/
+-rw-rw-rw-   0        0        0      470 2021-05-21 15:20:54.000000 javaman-1.0.9/src/javaman.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      580 2021-05-21 15:20:54.000000 javaman-1.0.9/src/javaman.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2021-05-21 15:20:54.000000 javaman-1.0.9/src/javaman.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2021-05-21 15:20:54.000000 javaman-1.0.9/src/javaman.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2021-05-21 15:20:54.000000 javaman-1.0.9/src/javaman.egg-info/top_level.txt
```

### Comparing `javaman-1.0.8/setup.py` & `javaman-1.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='1.0.8',  # Required
+    version='1.0.9',  # Required
 
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description='A Girotec - Api project',  # Optional
 
     # This is an optional longer description of your project that represents
```

