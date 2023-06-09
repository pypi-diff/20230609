# Comparing `tmp/UzEduCorpus-0.0.2.tar.gz` & `tmp/UzEduCorpus-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UzEduCorpus-0.0.2.tar", last modified: Fri Jun  9 06:47:07 2023, max compression
+gzip compressed data, was "UzEduCorpus-0.0.3.tar", last modified: Fri Jun  9 06:56:24 2023, max compression
```

## Comparing `UzEduCorpus-0.0.2.tar` & `UzEduCorpus-0.0.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 06:47:07.261260 UzEduCorpus-0.0.2/
--rw-rw-rw-   0        0        0     1091 2023-06-09 05:24:22.000000 UzEduCorpus-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      981 2023-06-09 06:47:07.261260 UzEduCorpus-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      300 2023-06-09 06:35:20.000000 UzEduCorpus-0.0.2/README.md
--rw-rw-rw-   0        0        0       86 2023-06-09 05:24:22.000000 UzEduCorpus-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-09 06:47:07.261260 UzEduCorpus-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1167 2023-06-09 06:46:35.000000 UzEduCorpus-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-09 06:47:07.195113 UzEduCorpus-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-06-09 06:47:07.244942 UzEduCorpus-0.0.2/src/UzEduCorpus/
--rw-rw-rw-   0        0        0     2718 2023-06-09 06:32:43.000000 UzEduCorpus-0.0.2/src/UzEduCorpus/UzEduCorpus.py
--rw-rw-rw-   0        0        0       28 2023-06-09 06:37:41.000000 UzEduCorpus-0.0.2/src/UzEduCorpus/__init__.py
--rw-rw-rw-   0        0        0    84507 2023-06-09 05:12:07.000000 UzEduCorpus-0.0.2/src/UzEduCorpus/grade_1.csv
--rw-rw-rw-   0        0        0   163146 2023-06-09 05:43:20.000000 UzEduCorpus-0.0.2/src/UzEduCorpus/grade_2.csv
--rw-rw-rw-   0        0        0   236007 2023-06-09 05:43:20.000000 UzEduCorpus-0.0.2/src/UzEduCorpus/grade_3.csv
--rw-rw-rw-   0        0        0   279490 2023-06-09 05:43:20.000000 UzEduCorpus-0.0.2/src/UzEduCorpus/grade_4.csv
--rw-rw-rw-   0        0        0   486521 2023-06-09 05:43:20.000000 UzEduCorpus-0.0.2/src/UzEduCorpus/grade_5.csv
--rw-rw-rw-   0        0        0   440184 2023-06-09 05:43:20.000000 UzEduCorpus-0.0.2/src/UzEduCorpus/grade_6.csv
--rw-rw-rw-   0        0        0   396530 2023-06-09 05:57:59.000000 UzEduCorpus-0.0.2/src/UzEduCorpus/grade_7.csv
--rw-rw-rw-   0        0        0   315275 2023-06-09 05:43:20.000000 UzEduCorpus-0.0.2/src/UzEduCorpus/grade_8.csv
--rw-rw-rw-   0        0        0   146614 2023-06-09 05:43:20.000000 UzEduCorpus-0.0.2/src/UzEduCorpus/grade_9.csv
-drwxrwxrwx   0        0        0        0 2023-06-09 06:47:07.259710 UzEduCorpus-0.0.2/src/UzEduCorpus.egg-info/
--rw-rw-rw-   0        0        0      981 2023-06-09 06:47:07.000000 UzEduCorpus-0.0.2/src/UzEduCorpus.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      508 2023-06-09 06:47:07.000000 UzEduCorpus-0.0.2/src/UzEduCorpus.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 06:47:07.000000 UzEduCorpus-0.0.2/src/UzEduCorpus.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-06-09 06:47:07.000000 UzEduCorpus-0.0.2/src/UzEduCorpus.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-09 06:56:24.182505 UzEduCorpus-0.0.3/
+-rw-rw-rw-   0        0        0     1091 2023-06-09 05:24:22.000000 UzEduCorpus-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      833 2023-06-09 06:56:24.182505 UzEduCorpus-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      297 2023-06-09 06:54:00.000000 UzEduCorpus-0.0.3/README.md
+-rw-rw-rw-   0        0        0       86 2023-06-09 05:24:22.000000 UzEduCorpus-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-09 06:56:24.182505 UzEduCorpus-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      950 2023-06-09 06:55:51.000000 UzEduCorpus-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 06:56:24.127533 UzEduCorpus-0.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-06-09 06:56:24.168815 UzEduCorpus-0.0.3/src/UzEduCorpus/
+-rw-rw-rw-   0        0        0     2718 2023-06-09 06:32:43.000000 UzEduCorpus-0.0.3/src/UzEduCorpus/UzEduCorpus.py
+-rw-rw-rw-   0        0        0       28 2023-06-09 06:37:41.000000 UzEduCorpus-0.0.3/src/UzEduCorpus/__init__.py
+-rw-rw-rw-   0        0        0    84507 2023-06-09 05:12:07.000000 UzEduCorpus-0.0.3/src/UzEduCorpus/grade_1.csv
+-rw-rw-rw-   0        0        0   163146 2023-06-09 05:43:20.000000 UzEduCorpus-0.0.3/src/UzEduCorpus/grade_2.csv
+-rw-rw-rw-   0        0        0   236007 2023-06-09 05:43:20.000000 UzEduCorpus-0.0.3/src/UzEduCorpus/grade_3.csv
+-rw-rw-rw-   0        0        0   279490 2023-06-09 05:43:20.000000 UzEduCorpus-0.0.3/src/UzEduCorpus/grade_4.csv
+-rw-rw-rw-   0        0        0   486521 2023-06-09 05:43:20.000000 UzEduCorpus-0.0.3/src/UzEduCorpus/grade_5.csv
+-rw-rw-rw-   0        0        0   440184 2023-06-09 05:43:20.000000 UzEduCorpus-0.0.3/src/UzEduCorpus/grade_6.csv
+-rw-rw-rw-   0        0        0   396530 2023-06-09 05:57:59.000000 UzEduCorpus-0.0.3/src/UzEduCorpus/grade_7.csv
+-rw-rw-rw-   0        0        0   315275 2023-06-09 05:43:20.000000 UzEduCorpus-0.0.3/src/UzEduCorpus/grade_8.csv
+-rw-rw-rw-   0        0        0   146614 2023-06-09 05:43:20.000000 UzEduCorpus-0.0.3/src/UzEduCorpus/grade_9.csv
+drwxrwxrwx   0        0        0        0 2023-06-09 06:56:24.182505 UzEduCorpus-0.0.3/src/UzEduCorpus.egg-info/
+-rw-rw-rw-   0        0        0      833 2023-06-09 06:56:24.000000 UzEduCorpus-0.0.3/src/UzEduCorpus.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      508 2023-06-09 06:56:24.000000 UzEduCorpus-0.0.3/src/UzEduCorpus.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 06:56:24.000000 UzEduCorpus-0.0.3/src/UzEduCorpus.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-06-09 06:56:24.000000 UzEduCorpus-0.0.3/src/UzEduCorpus.egg-info/top_level.txt
```

### Comparing `UzEduCorpus-0.0.2/LICENSE` & `UzEduCorpus-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `UzEduCorpus-0.0.2/PKG-INFO` & `UzEduCorpus-0.0.3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: UzEduCorpus
-Version: 0.0.2
-Summary: UzTransliterator | Transliteration tool for Uzbek language - Cyrillic<>Latin<>NewLatin
-Home-page: https://github.com/UlugbekSalaev/UzTransliterator
+Version: 0.0.3
+Summary: Uzbek language Educational Corpus
+Home-page: https://github.com/
 Author: Muhayyo Narimonova
 Author-email: muhayyonarimonova1797@gmail.com
-Project-URL: Bug Tracker, https://github.com/UlugbekSalaev/UzTransliterator/issues
-Keywords: python,transliteration,uzbek-language,cyrillic,latin
+Project-URL: Bug Tracker, https://github.com/
+Keywords: python,uzbek-language,latin
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -23,12 +23,12 @@
 <div align="center">
   <h3 align="center">UzEduCorpus</h3>
   
 </div>
 
 ```
 from UzEduCorpus import UzEduCorpus
-print(UzEduCorpus.load_1());
-print(UzEduCorpus.load_2());
+print(UzEduCorpus.load_1())
+print(UzEduCorpus.load_2())
 # ...
-print(UzEduCorpus.load_9());
+print(UzEduCorpus.load_9())
 ```
```

### Comparing `UzEduCorpus-0.0.2/setup.py` & `UzEduCorpus-0.0.3/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="UzEduCorpus",
-    version="0.0.2",
+    version="0.0.3",
     author="Muhayyo Narimonova",
     author_email="muhayyonarimonova1797@gmail.com",
-    description="UzTransliterator | Transliteration tool for Uzbek language - Cyrillic<>Latin<>NewLatin",
+    description="Uzbek language Educational Corpus",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/UlugbekSalaev/UzTransliterator",
+    url="https://github.com/",
     project_urls={
-        "Bug Tracker": "https://github.com/UlugbekSalaev/UzTransliterator/issues",
+        "Bug Tracker": "https://github.com/",
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    keywords=['python', 'transliteration', 'uzbek-language', 'cyrillic', 'latin'],
+    keywords=['python', 'uzbek-language', 'latin'],
     package_dir={"": "src"},
     packages=setuptools.find_packages(where="src"),
     install_requires=[],
     python_requires=">=3.6",
     include_package_data=True,
     package_data={"": ["*.csv"]},
-    #package_data={"": ["cyr_exwords.csv", "lat_exwords.csv"],},
 )
```

### Comparing `UzEduCorpus-0.0.2/src/UzEduCorpus/UzEduCorpus.py` & `UzEduCorpus-0.0.3/src/UzEduCorpus/UzEduCorpus.py`

 * *Files identical despite different names*

### Comparing `UzEduCorpus-0.0.2/src/UzEduCorpus/grade_1.csv` & `UzEduCorpus-0.0.3/src/UzEduCorpus/grade_1.csv`

 * *Files identical despite different names*

### Comparing `UzEduCorpus-0.0.2/src/UzEduCorpus/grade_2.csv` & `UzEduCorpus-0.0.3/src/UzEduCorpus/grade_2.csv`

 * *Files identical despite different names*

### Comparing `UzEduCorpus-0.0.2/src/UzEduCorpus/grade_3.csv` & `UzEduCorpus-0.0.3/src/UzEduCorpus/grade_3.csv`

 * *Files identical despite different names*

### Comparing `UzEduCorpus-0.0.2/src/UzEduCorpus/grade_4.csv` & `UzEduCorpus-0.0.3/src/UzEduCorpus/grade_4.csv`

 * *Files identical despite different names*

### Comparing `UzEduCorpus-0.0.2/src/UzEduCorpus/grade_5.csv` & `UzEduCorpus-0.0.3/src/UzEduCorpus/grade_5.csv`

 * *Files identical despite different names*

### Comparing `UzEduCorpus-0.0.2/src/UzEduCorpus/grade_6.csv` & `UzEduCorpus-0.0.3/src/UzEduCorpus/grade_6.csv`

 * *Files identical despite different names*

### Comparing `UzEduCorpus-0.0.2/src/UzEduCorpus/grade_7.csv` & `UzEduCorpus-0.0.3/src/UzEduCorpus/grade_7.csv`

 * *Files identical despite different names*

### Comparing `UzEduCorpus-0.0.2/src/UzEduCorpus/grade_8.csv` & `UzEduCorpus-0.0.3/src/UzEduCorpus/grade_8.csv`

 * *Files identical despite different names*

### Comparing `UzEduCorpus-0.0.2/src/UzEduCorpus/grade_9.csv` & `UzEduCorpus-0.0.3/src/UzEduCorpus/grade_9.csv`

 * *Files identical despite different names*

### Comparing `UzEduCorpus-0.0.2/src/UzEduCorpus.egg-info/PKG-INFO` & `UzEduCorpus-0.0.3/src/UzEduCorpus.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: UzEduCorpus
-Version: 0.0.2
-Summary: UzTransliterator | Transliteration tool for Uzbek language - Cyrillic<>Latin<>NewLatin
-Home-page: https://github.com/UlugbekSalaev/UzTransliterator
+Version: 0.0.3
+Summary: Uzbek language Educational Corpus
+Home-page: https://github.com/
 Author: Muhayyo Narimonova
 Author-email: muhayyonarimonova1797@gmail.com
-Project-URL: Bug Tracker, https://github.com/UlugbekSalaev/UzTransliterator/issues
-Keywords: python,transliteration,uzbek-language,cyrillic,latin
+Project-URL: Bug Tracker, https://github.com/
+Keywords: python,uzbek-language,latin
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -23,12 +23,12 @@
 <div align="center">
   <h3 align="center">UzEduCorpus</h3>
   
 </div>
 
 ```
 from UzEduCorpus import UzEduCorpus
-print(UzEduCorpus.load_1());
-print(UzEduCorpus.load_2());
+print(UzEduCorpus.load_1())
+print(UzEduCorpus.load_2())
 # ...
-print(UzEduCorpus.load_9());
+print(UzEduCorpus.load_9())
 ```
```

