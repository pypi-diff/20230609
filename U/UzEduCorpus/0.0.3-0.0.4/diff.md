# Comparing `tmp/UzEduCorpus-0.0.3.tar.gz` & `tmp/UzEduCorpus-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UzEduCorpus-0.0.3.tar", last modified: Fri Jun  9 06:56:24 2023, max compression
+gzip compressed data, was "UzEduCorpus-0.0.4.tar", last modified: Fri Jun  9 07:11:56 2023, max compression
```

## Comparing `UzEduCorpus-0.0.3.tar` & `UzEduCorpus-0.0.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 06:56:24.182505 UzEduCorpus-0.0.3/
--rw-rw-rw-   0        0        0     1091 2023-06-09 05:24:22.000000 UzEduCorpus-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      833 2023-06-09 06:56:24.182505 UzEduCorpus-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      297 2023-06-09 06:54:00.000000 UzEduCorpus-0.0.3/README.md
--rw-rw-rw-   0        0        0       86 2023-06-09 05:24:22.000000 UzEduCorpus-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-09 06:56:24.182505 UzEduCorpus-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      950 2023-06-09 06:55:51.000000 UzEduCorpus-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-09 06:56:24.127533 UzEduCorpus-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-06-09 06:56:24.168815 UzEduCorpus-0.0.3/src/UzEduCorpus/
--rw-rw-rw-   0        0        0     2718 2023-06-09 06:32:43.000000 UzEduCorpus-0.0.3/src/UzEduCorpus/UzEduCorpus.py
--rw-rw-rw-   0        0        0       28 2023-06-09 06:37:41.000000 UzEduCorpus-0.0.3/src/UzEduCorpus/__init__.py
--rw-rw-rw-   0        0        0    84507 2023-06-09 05:12:07.000000 UzEduCorpus-0.0.3/src/UzEduCorpus/grade_1.csv
--rw-rw-rw-   0        0        0   163146 2023-06-09 05:43:20.000000 UzEduCorpus-0.0.3/src/UzEduCorpus/grade_2.csv
--rw-rw-rw-   0        0        0   236007 2023-06-09 05:43:20.000000 UzEduCorpus-0.0.3/src/UzEduCorpus/grade_3.csv
--rw-rw-rw-   0        0        0   279490 2023-06-09 05:43:20.000000 UzEduCorpus-0.0.3/src/UzEduCorpus/grade_4.csv
--rw-rw-rw-   0        0        0   486521 2023-06-09 05:43:20.000000 UzEduCorpus-0.0.3/src/UzEduCorpus/grade_5.csv
--rw-rw-rw-   0        0        0   440184 2023-06-09 05:43:20.000000 UzEduCorpus-0.0.3/src/UzEduCorpus/grade_6.csv
--rw-rw-rw-   0        0        0   396530 2023-06-09 05:57:59.000000 UzEduCorpus-0.0.3/src/UzEduCorpus/grade_7.csv
--rw-rw-rw-   0        0        0   315275 2023-06-09 05:43:20.000000 UzEduCorpus-0.0.3/src/UzEduCorpus/grade_8.csv
--rw-rw-rw-   0        0        0   146614 2023-06-09 05:43:20.000000 UzEduCorpus-0.0.3/src/UzEduCorpus/grade_9.csv
-drwxrwxrwx   0        0        0        0 2023-06-09 06:56:24.182505 UzEduCorpus-0.0.3/src/UzEduCorpus.egg-info/
--rw-rw-rw-   0        0        0      833 2023-06-09 06:56:24.000000 UzEduCorpus-0.0.3/src/UzEduCorpus.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      508 2023-06-09 06:56:24.000000 UzEduCorpus-0.0.3/src/UzEduCorpus.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 06:56:24.000000 UzEduCorpus-0.0.3/src/UzEduCorpus.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-06-09 06:56:24.000000 UzEduCorpus-0.0.3/src/UzEduCorpus.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-09 07:11:56.933807 UzEduCorpus-0.0.4/
+-rw-rw-rw-   0        0        0     1091 2023-06-09 05:24:22.000000 UzEduCorpus-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     1257 2023-06-09 07:11:56.931490 UzEduCorpus-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      721 2023-06-09 07:09:30.000000 UzEduCorpus-0.0.4/README.md
+-rw-rw-rw-   0        0        0       86 2023-06-09 05:24:22.000000 UzEduCorpus-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-09 07:11:56.933807 UzEduCorpus-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      950 2023-06-09 07:11:26.000000 UzEduCorpus-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 07:11:56.880366 UzEduCorpus-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-06-09 07:11:56.912954 UzEduCorpus-0.0.4/src/UzEduCorpus/
+-rw-rw-rw-   0        0        0     2729 2023-06-09 07:10:07.000000 UzEduCorpus-0.0.4/src/UzEduCorpus/UzEduCorpus.py
+-rw-rw-rw-   0        0        0       28 2023-06-09 06:37:41.000000 UzEduCorpus-0.0.4/src/UzEduCorpus/__init__.py
+-rw-rw-rw-   0        0        0    84507 2023-06-09 05:12:07.000000 UzEduCorpus-0.0.4/src/UzEduCorpus/grade_1.csv
+-rw-rw-rw-   0        0        0   163146 2023-06-09 05:43:20.000000 UzEduCorpus-0.0.4/src/UzEduCorpus/grade_2.csv
+-rw-rw-rw-   0        0        0   236007 2023-06-09 05:43:20.000000 UzEduCorpus-0.0.4/src/UzEduCorpus/grade_3.csv
+-rw-rw-rw-   0        0        0   279490 2023-06-09 05:43:20.000000 UzEduCorpus-0.0.4/src/UzEduCorpus/grade_4.csv
+-rw-rw-rw-   0        0        0   486521 2023-06-09 05:43:20.000000 UzEduCorpus-0.0.4/src/UzEduCorpus/grade_5.csv
+-rw-rw-rw-   0        0        0   440184 2023-06-09 05:43:20.000000 UzEduCorpus-0.0.4/src/UzEduCorpus/grade_6.csv
+-rw-rw-rw-   0        0        0   396530 2023-06-09 05:57:59.000000 UzEduCorpus-0.0.4/src/UzEduCorpus/grade_7.csv
+-rw-rw-rw-   0        0        0   315275 2023-06-09 05:43:20.000000 UzEduCorpus-0.0.4/src/UzEduCorpus/grade_8.csv
+-rw-rw-rw-   0        0        0   146614 2023-06-09 05:43:20.000000 UzEduCorpus-0.0.4/src/UzEduCorpus/grade_9.csv
+drwxrwxrwx   0        0        0        0 2023-06-09 07:11:56.927503 UzEduCorpus-0.0.4/src/UzEduCorpus.egg-info/
+-rw-rw-rw-   0        0        0     1257 2023-06-09 07:11:56.000000 UzEduCorpus-0.0.4/src/UzEduCorpus.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      508 2023-06-09 07:11:56.000000 UzEduCorpus-0.0.4/src/UzEduCorpus.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 07:11:56.000000 UzEduCorpus-0.0.4/src/UzEduCorpus.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-06-09 07:11:56.000000 UzEduCorpus-0.0.4/src/UzEduCorpus.egg-info/top_level.txt
```

### Comparing `UzEduCorpus-0.0.3/LICENSE` & `UzEduCorpus-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `UzEduCorpus-0.0.3/setup.py` & `UzEduCorpus-0.0.4/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="UzEduCorpus",
-    version="0.0.3",
+    version="0.0.4",
     author="Muhayyo Narimonova",
     author_email="muhayyonarimonova1797@gmail.com",
     description="Uzbek language Educational Corpus",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/",
+    url="https://uzedu.uz/uz",
     project_urls={
-        "Bug Tracker": "https://github.com/",
+        "Bug Tracker": "https://uzedu.uz/uz",
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     keywords=['python', 'uzbek-language', 'latin'],
```

### Comparing `UzEduCorpus-0.0.3/src/UzEduCorpus/UzEduCorpus.py` & `UzEduCorpus-0.0.4/src/UzEduCorpus/UzEduCorpus.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,91 +1,91 @@
 import os
 
-def load_1():
+def grade_1():
     words = list()
     dirname = os.path.dirname(__file__) + "/"
     with open(os.path.join(dirname + "grade_1.csv"), encoding='utf8') as file:
         for line in file:
             x = line.rstrip()
             words.append(x)
         words.remove(words[0])
     return words
 
-def load_2():
+def grade_2():
     words = list()
     dirname = os.path.dirname(__file__) + "/"
     with open(os.path.join(dirname + "grade_2.csv"), encoding='utf8') as file:
         for line in file:
             x = line.rstrip()
             words.append(x)
         words.remove(words[0])
     return words
 
-def load_3():
+def grade_3():
     words = list()
     dirname = os.path.dirname(__file__) + "/"
     with open(os.path.join(dirname + "grade_3.csv"), encoding='utf8') as file:
         for line in file:
             x = line.rstrip()
             words.append(x)
         words.remove(words[0])
     return words
 
-def load_4():
+def grade_4():
     words = list()
     dirname = os.path.dirname(__file__) + "/"
     with open(os.path.join(dirname + "grade_4.csv"), encoding='utf8') as file:
         for line in file:
             x = line.rstrip()
             words.append(x)
         words.remove(words[0])
     return words
 
-def load_5():
+def grade_5():
     words = list()
     dirname = os.path.dirname(__file__) + "/"
     with open(os.path.join(dirname + "grade_5.csv"), encoding='utf8') as file:
         for line in file:
             x = line.rstrip()
             words.append(x)
         words.remove(words[0])
     return words
 
-def load_6():
+def grade_6():
     words = list()
     dirname = os.path.dirname(__file__) + "/"
     with open(os.path.join(dirname + "grade_6.csv"), encoding='utf8') as file:
         for line in file:
             x = line.rstrip()
             words.append(x)
         words.remove(words[0])
     return words
 
-def load_7():
+def grade_7():
     words = list()
     dirname = os.path.dirname(__file__) + "/"
     with open(os.path.join(dirname + "grade_7.csv"), encoding='utf8') as file:
         for line in file:
             x = line.rstrip()
             words.append(x)
         words.remove(words[0])
     return words
 
-def load_8():
+def grade_8():
     words = list()
     dirname = os.path.dirname(__file__) + "/"
     with open(os.path.join(dirname + "grade_8.csv"), encoding='utf8') as file:
         for line in file:
             x = line.rstrip()
             words.append(x)
         words.remove(words[0])
     return words
 
-def load_9():
+def grade_9():
     words = list()
     dirname = os.path.dirname(__file__) + "/"
     with open(os.path.join(dirname + "grade_9.csv"), encoding='utf8') as file:
         for line in file:
             x = line.rstrip()
             words.append(x)
         words.remove(words[0])
-    return words
+    return words
```

### Comparing `UzEduCorpus-0.0.3/src/UzEduCorpus/grade_1.csv` & `UzEduCorpus-0.0.4/src/UzEduCorpus/grade_1.csv`

 * *Files identical despite different names*

### Comparing `UzEduCorpus-0.0.3/src/UzEduCorpus/grade_2.csv` & `UzEduCorpus-0.0.4/src/UzEduCorpus/grade_2.csv`

 * *Files identical despite different names*

### Comparing `UzEduCorpus-0.0.3/src/UzEduCorpus/grade_3.csv` & `UzEduCorpus-0.0.4/src/UzEduCorpus/grade_3.csv`

 * *Files identical despite different names*

### Comparing `UzEduCorpus-0.0.3/src/UzEduCorpus/grade_4.csv` & `UzEduCorpus-0.0.4/src/UzEduCorpus/grade_4.csv`

 * *Files identical despite different names*

### Comparing `UzEduCorpus-0.0.3/src/UzEduCorpus/grade_5.csv` & `UzEduCorpus-0.0.4/src/UzEduCorpus/grade_5.csv`

 * *Files identical despite different names*

### Comparing `UzEduCorpus-0.0.3/src/UzEduCorpus/grade_6.csv` & `UzEduCorpus-0.0.4/src/UzEduCorpus/grade_6.csv`

 * *Files identical despite different names*

### Comparing `UzEduCorpus-0.0.3/src/UzEduCorpus/grade_7.csv` & `UzEduCorpus-0.0.4/src/UzEduCorpus/grade_7.csv`

 * *Files identical despite different names*

### Comparing `UzEduCorpus-0.0.3/src/UzEduCorpus/grade_8.csv` & `UzEduCorpus-0.0.4/src/UzEduCorpus/grade_8.csv`

 * *Files identical despite different names*

### Comparing `UzEduCorpus-0.0.3/src/UzEduCorpus/grade_9.csv` & `UzEduCorpus-0.0.4/src/UzEduCorpus/grade_9.csv`

 * *Files identical despite different names*

