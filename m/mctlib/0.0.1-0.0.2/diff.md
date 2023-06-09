# Comparing `tmp/mctlib-0.0.1.tar.gz` & `tmp/mctlib-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mctlib-0.0.1.tar", last modified: Wed Jun  7 13:49:51 2023, max compression
+gzip compressed data, was "mctlib-0.0.2.tar", last modified: Fri Jun  9 10:13:10 2023, max compression
```

## Comparing `mctlib-0.0.1.tar` & `mctlib-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 mistacheese   (501) staff       (20)        0 2023-06-07 13:49:51.094590 mctlib-0.0.1/
--rw-r--r--   0 mistacheese   (501) staff       (20)       83 2023-06-07 13:44:03.000000 mctlib-0.0.1/CHANGELOG.txt
--rw-r--r--   0 mistacheese   (501) staff       (20)     1060 2023-03-25 16:19:24.000000 mctlib-0.0.1/LICENSE.txt
--rw-r--r--   0 mistacheese   (501) staff       (20)       25 2023-03-25 16:19:24.000000 mctlib-0.0.1/MANIFEST.in
--rw-r--r--   0 mistacheese   (501) staff       (20)      611 2023-06-07 13:49:51.094468 mctlib-0.0.1/PKG-INFO
--rw-r--r--   0 mistacheese   (501) staff       (20)       64 2023-06-07 13:48:43.000000 mctlib-0.0.1/README.txt
-drwxr-xr-x   0 mistacheese   (501) staff       (20)        0 2023-06-07 13:49:51.093706 mctlib-0.0.1/mctlib/
--rw-r--r--   0 mistacheese   (501) staff       (20)      294 2023-05-07 07:59:56.000000 mctlib-0.0.1/mctlib/__init__.py
-drwxr-xr-x   0 mistacheese   (501) staff       (20)        0 2023-06-07 13:49:51.094297 mctlib-0.0.1/mctlib.egg-info/
--rw-r--r--   0 mistacheese   (501) staff       (20)      611 2023-06-07 13:49:51.000000 mctlib-0.0.1/mctlib.egg-info/PKG-INFO
--rw-r--r--   0 mistacheese   (501) staff       (20)      196 2023-06-07 13:49:51.000000 mctlib-0.0.1/mctlib.egg-info/SOURCES.txt
--rw-r--r--   0 mistacheese   (501) staff       (20)        1 2023-06-07 13:49:51.000000 mctlib-0.0.1/mctlib.egg-info/dependency_links.txt
--rw-r--r--   0 mistacheese   (501) staff       (20)        7 2023-06-07 13:49:51.000000 mctlib-0.0.1/mctlib.egg-info/top_level.txt
--rw-r--r--   0 mistacheese   (501) staff       (20)       38 2023-06-07 13:49:51.094632 mctlib-0.0.1/setup.cfg
--rw-r--r--   0 mistacheese   (501) staff       (20)      658 2023-06-07 13:48:46.000000 mctlib-0.0.1/setup.py
+drwxr-xr-x   0 mistacheese   (501) staff       (20)        0 2023-06-09 10:13:10.069797 mctlib-0.0.2/
+-rw-r--r--   0 mistacheese   (501) staff       (20)      150 2023-06-09 09:55:26.000000 mctlib-0.0.2/CHANGELOG.txt
+-rw-r--r--   0 mistacheese   (501) staff       (20)     1060 2023-03-25 16:19:24.000000 mctlib-0.0.2/LICENSE.txt
+-rw-r--r--   0 mistacheese   (501) staff       (20)       25 2023-03-25 16:19:24.000000 mctlib-0.0.2/MANIFEST.in
+-rw-r--r--   0 mistacheese   (501) staff       (20)      679 2023-06-09 10:13:10.069678 mctlib-0.0.2/PKG-INFO
+-rw-r--r--   0 mistacheese   (501) staff       (20)       64 2023-06-07 13:48:43.000000 mctlib-0.0.2/README.txt
+drwxr-xr-x   0 mistacheese   (501) staff       (20)        0 2023-06-09 10:13:10.069042 mctlib-0.0.2/mctlib/
+-rw-r--r--   0 mistacheese   (501) staff       (20)     2231 2023-06-09 10:12:39.000000 mctlib-0.0.2/mctlib/__init__.py
+drwxr-xr-x   0 mistacheese   (501) staff       (20)        0 2023-06-09 10:13:10.069507 mctlib-0.0.2/mctlib.egg-info/
+-rw-r--r--   0 mistacheese   (501) staff       (20)      679 2023-06-09 10:13:10.000000 mctlib-0.0.2/mctlib.egg-info/PKG-INFO
+-rw-r--r--   0 mistacheese   (501) staff       (20)      196 2023-06-09 10:13:10.000000 mctlib-0.0.2/mctlib.egg-info/SOURCES.txt
+-rw-r--r--   0 mistacheese   (501) staff       (20)        1 2023-06-09 10:13:10.000000 mctlib-0.0.2/mctlib.egg-info/dependency_links.txt
+-rw-r--r--   0 mistacheese   (501) staff       (20)        7 2023-06-09 10:13:10.000000 mctlib-0.0.2/mctlib.egg-info/top_level.txt
+-rw-r--r--   0 mistacheese   (501) staff       (20)       38 2023-06-09 10:13:10.069831 mctlib-0.0.2/setup.cfg
+-rw-r--r--   0 mistacheese   (501) staff       (20)      659 2023-06-09 09:55:28.000000 mctlib-0.0.2/setup.py
```

### Comparing `mctlib-0.0.1/LICENSE.txt` & `mctlib-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mctlib-0.0.1/setup.py` & `mctlib-0.0.2/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,21 +6,21 @@
   'Operating System :: OS Independent',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
 
 setup(
   name='mctlib',
-  version='0.0.1',
+  version='0.0.2',
   description='some extra functions',
   long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
   url='',  
   author='Mate Chocheli',
   author_email='matechocheli2@gmail.com',
   license='MIT', 
   classifiers=classifiers,
   keywords='mistacheeselib', 
   packages=find_packages(),
   install_requires=[''] 
 )
 
-url =""
+url =""
```

