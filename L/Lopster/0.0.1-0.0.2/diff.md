# Comparing `tmp/Lopster-0.0.1.tar.gz` & `tmp/Lopster-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Lopster-0.0.1.tar", last modified: Fri Jun  9 15:01:44 2023, max compression
+gzip compressed data, was "Lopster-0.0.2.tar", last modified: Fri Jun  9 15:38:04 2023, max compression
```

## Comparing `Lopster-0.0.1.tar` & `Lopster-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 15:01:44.856230 Lopster-0.0.1/
-drwxrwxrwx   0        0        0        0 2023-06-09 15:01:44.824980 Lopster-0.0.1/Lopster/
--rw-rw-rw-   0        0        0     7125 2023-06-09 14:24:33.000000 Lopster-0.0.1/Lopster/Lopster.py
--rw-rw-rw-   0        0        0       14 2023-06-09 14:51:42.000000 Lopster-0.0.1/Lopster/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-09 15:01:44.856230 Lopster-0.0.1/Lopster.egg-info/
--rw-rw-rw-   0        0        0      181 2023-06-09 15:01:44.000000 Lopster-0.0.1/Lopster.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      201 2023-06-09 15:01:44.000000 Lopster-0.0.1/Lopster.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 15:01:44.000000 Lopster-0.0.1/Lopster.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-09 15:01:44.000000 Lopster-0.0.1/Lopster.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-09 15:01:44.000000 Lopster-0.0.1/Lopster.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      181 2023-06-09 15:01:44.856230 Lopster-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-06-09 15:01:44.856230 Lopster-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      296 2023-06-09 14:51:42.000000 Lopster-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 15:38:04.101022 Lopster-0.0.2/
+drwxrwxrwx   0        0        0        0 2023-06-09 15:38:04.085396 Lopster-0.0.2/Lopster/
+-rw-rw-rw-   0        0        0     7201 2023-06-09 15:29:02.000000 Lopster-0.0.2/Lopster/Lopster.py
+-rw-rw-rw-   0        0        0       21 2023-06-09 15:29:47.000000 Lopster-0.0.2/Lopster/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 15:38:04.101022 Lopster-0.0.2/Lopster.egg-info/
+-rw-rw-rw-   0        0        0      235 2023-06-09 15:38:04.000000 Lopster-0.0.2/Lopster.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      201 2023-06-09 15:38:04.000000 Lopster-0.0.2/Lopster.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 15:38:04.000000 Lopster-0.0.2/Lopster.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-09 15:38:04.000000 Lopster-0.0.2/Lopster.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-09 15:38:04.000000 Lopster-0.0.2/Lopster.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      235 2023-06-09 15:38:04.101022 Lopster-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-06-09 15:38:04.101022 Lopster-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      396 2023-06-09 15:33:13.000000 Lopster-0.0.2/setup.py
```

### Comparing `Lopster-0.0.1/Lopster/Lopster.py` & `Lopster-0.0.2/Lopster/Lopster.py`

 * *Files 1% similar despite different names*

```diff
@@ -253,7 +253,9 @@
             for obj in Enemy._object:
                 if obj.typ != "NoN":
                     obj.update(window, obj)
 
             pygame.display.update()
 
         pygame.quit()
+
+__all__ = ['Enemy', 'FakeEnemy', 'Player', 'MathMap', 'Map', 'RunLopster']
```

