# Comparing `tmp/junit-to-md-py-1.0.0.tar.gz` & `tmp/junit-to-md-py-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "junit-to-md-py-1.0.0.tar", last modified: Wed Jun  7 18:15:07 2023, max compression
+gzip compressed data, was "junit-to-md-py-1.1.0.tar", last modified: Fri Jun  9 11:45:33 2023, max compression
```

## Comparing `junit-to-md-py-1.0.0.tar` & `junit-to-md-py-1.1.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 18:15:07.837024 junit-to-md-py-1.0.0/
--rw-rw-rw-   0        0        0      617 2023-06-07 18:15:07.837024 junit-to-md-py-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      301 2023-06-07 18:12:45.000000 junit-to-md-py-1.0.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-06-07 18:15:07.802607 junit-to-md-py-1.0.0/junit_to_md/
--rw-rw-rw-   0        0        0       37 2023-06-07 11:42:31.000000 junit-to-md-py-1.0.0/junit_to_md/__init__.py
--rw-rw-rw-   0        0        0     1010 2023-06-07 18:09:23.000000 junit-to-md-py-1.0.0/junit_to_md/junit_to_md.py
-drwxrwxrwx   0        0        0        0 2023-06-07 18:15:07.833022 junit-to-md-py-1.0.0/junit_to_md_py.egg-info/
--rw-rw-rw-   0        0        0      617 2023-06-07 18:15:07.000000 junit-to-md-py-1.0.0/junit_to_md_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      259 2023-06-07 18:15:07.000000 junit-to-md-py-1.0.0/junit_to_md_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 18:15:07.000000 junit-to-md-py-1.0.0/junit_to_md_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-06-07 18:15:07.000000 junit-to-md-py-1.0.0/junit_to_md_py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-07 18:15:07.000000 junit-to-md-py-1.0.0/junit_to_md_py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-07 18:15:07.837024 junit-to-md-py-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      521 2023-06-07 18:12:30.000000 junit-to-md-py-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 11:45:33.535014 junit-to-md-py-1.1.0/
+-rw-rw-rw-   0        0        0      617 2023-06-09 11:45:33.534014 junit-to-md-py-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      301 2023-06-07 18:12:45.000000 junit-to-md-py-1.1.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-09 11:45:33.527013 junit-to-md-py-1.1.0/junit_to_md_py.egg-info/
+-rw-rw-rw-   0        0        0      617 2023-06-09 11:45:33.000000 junit-to-md-py-1.1.0/junit_to_md_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      290 2023-06-09 11:45:33.000000 junit-to-md-py-1.1.0/junit_to_md_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 11:45:33.000000 junit-to-md-py-1.1.0/junit_to_md_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-06-09 11:45:33.000000 junit-to-md-py-1.1.0/junit_to_md_py.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        5 2023-06-09 11:45:33.000000 junit-to-md-py-1.1.0/junit_to_md_py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-09 11:45:33.000000 junit-to-md-py-1.1.0/junit_to_md_py.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-09 11:45:33.531014 junit-to-md-py-1.1.0/script/
+-rw-rw-rw-   0        0        0        0 2023-06-09 11:39:01.000000 junit-to-md-py-1.1.0/script/__init__.py
+-rw-rw-rw-   0        0        0     1267 2023-06-09 11:45:28.000000 junit-to-md-py-1.1.0/script/junit_to_md.py
+-rw-rw-rw-   0        0        0       42 2023-06-09 11:45:33.535014 junit-to-md-py-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      616 2023-06-09 11:42:54.000000 junit-to-md-py-1.1.0/setup.py
```

### Comparing `junit-to-md-py-1.0.0/PKG-INFO` & `junit-to-md-py-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: junit-to-md-py
-Version: 1.0.0
+Version: 1.1.0
 Summary: Python script which converts junit xml file/text into the markdown representation
 Home-page: https://github.com/catalogicsoftware/dpx-utils-junit-to-md
 Author: srydz_catalogicsoftware
 Author-email: srydz@catalogicsoftware.com
 License: MIT
 
 Python script which converts junit xml file/text into the markdown representation
```

### Comparing `junit-to-md-py-1.0.0/junit_to_md/junit_to_md.py` & `junit-to-md-py-1.1.0/script/junit_to_md.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,24 @@
+import argparse
 from lxml import etree
 
-def junit_to_md(user_input):
+
+def main():
+    parser = argparse.ArgumentParser(
+        prog="junit-to-md-py",
+        description="Converts JUnit XML report to markdown format",
+    )
+    parser.add_argument("file", help="Path to the JUnit XML report file")
+    args = parser.parse_args()
+
     failedTestDetails = []
     allTests = []
 
     try:
-        xmlDoc = etree.parse(user_input)
+        xmlDoc = etree.parse(args.file)
     except Exception:
         print(f"Error parsing the text from junitOutput!")
         return
 
     suites = xmlDoc.xpath("//testsuite")
     for suite in suites:
         tests = suite.xpath(".//testcase")
```

### Comparing `junit-to-md-py-1.0.0/junit_to_md_py.egg-info/PKG-INFO` & `junit-to-md-py-1.1.0/junit_to_md_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: junit-to-md-py
-Version: 1.0.0
+Version: 1.1.0
 Summary: Python script which converts junit xml file/text into the markdown representation
 Home-page: https://github.com/catalogicsoftware/dpx-utils-junit-to-md
 Author: srydz_catalogicsoftware
 Author-email: srydz@catalogicsoftware.com
 License: MIT
 
 Python script which converts junit xml file/text into the markdown representation
```

### Comparing `junit-to-md-py-1.0.0/setup.py` & `junit-to-md-py-1.1.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 from setuptools import setup
 
 setup(
     name="junit-to-md-py",
-    version="1.0.0",
+    version="1.1.0",
     author="srydz_catalogicsoftware",
     author_email="srydz@catalogicsoftware.com",
     description="Python script which converts junit xml file/text into the markdown representation",
     long_description=open("README.rst", encoding="utf-8").read(),
     url="https://github.com/catalogicsoftware/dpx-utils-junit-to-md",
     license="MIT",
-    packages=["junit_to_md"],
     install_requires=[
         "lxml",
     ],
+    entry_points={
+        "console_scripts": [
+            "junit-to-md-py = script.junit_to_md:main",
+        ]
+    },
 )
```

