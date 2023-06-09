# Comparing `tmp/TimeForge-0.1.8.tar.gz` & `tmp/TimeForge-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TimeForge-0.1.8.tar", last modified: Thu May 18 15:00:01 2023, max compression
+gzip compressed data, was "TimeForge-0.1.9.tar", last modified: Fri Jun  9 17:06:32 2023, max compression
```

## Comparing `TimeForge-0.1.8.tar` & `TimeForge-0.1.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-18 15:00:01.467273 TimeForge-0.1.8/
--rw-r--r--   0 michael   (1000) michael   (1000)    34916 2023-04-04 11:47:23.000000 TimeForge-0.1.8/LICENSE.md
--rw-r--r--   0 michael   (1000) michael   (1000)     1362 2023-05-18 15:00:01.467273 TimeForge-0.1.8/PKG-INFO
--rw-r--r--   0 michael   (1000) michael   (1000)      559 2023-05-08 08:20:49.000000 TimeForge-0.1.8/README.md
--rw-r--r--   0 michael   (1000) michael   (1000)      992 2023-05-18 14:59:40.000000 TimeForge-0.1.8/pyproject.toml
--rw-r--r--   0 michael   (1000) michael   (1000)       38 2023-05-18 15:00:01.467273 TimeForge-0.1.8/setup.cfg
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-18 15:00:01.467273 TimeForge-0.1.8/src/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-18 15:00:01.467273 TimeForge-0.1.8/src/TimeForge.egg-info/
--rw-r--r--   0 michael   (1000) michael   (1000)     1362 2023-05-18 15:00:01.000000 TimeForge-0.1.8/src/TimeForge.egg-info/PKG-INFO
--rw-r--r--   0 michael   (1000) michael   (1000)      271 2023-05-18 15:00:01.000000 TimeForge-0.1.8/src/TimeForge.egg-info/SOURCES.txt
--rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-05-18 15:00:01.000000 TimeForge-0.1.8/src/TimeForge.egg-info/dependency_links.txt
--rw-r--r--   0 michael   (1000) michael   (1000)      105 2023-05-18 15:00:01.000000 TimeForge-0.1.8/src/TimeForge.egg-info/requires.txt
--rw-r--r--   0 michael   (1000) michael   (1000)       10 2023-05-18 15:00:01.000000 TimeForge-0.1.8/src/TimeForge.egg-info/top_level.txt
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-18 15:00:01.467273 TimeForge-0.1.8/src/timeforge/
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-04-24 11:15:53.000000 TimeForge-0.1.8/src/timeforge/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)     6817 2023-05-09 20:24:02.000000 TimeForge-0.1.8/src/timeforge/__main__.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-09 17:06:32.685666 TimeForge-0.1.9/
+-rw-r--r--   0 michael   (1000) michael   (1000)    34916 2023-04-04 11:47:23.000000 TimeForge-0.1.9/LICENSE.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     1449 2023-06-09 17:06:32.685666 TimeForge-0.1.9/PKG-INFO
+-rw-r--r--   0 michael   (1000) michael   (1000)      646 2023-06-09 17:03:59.000000 TimeForge-0.1.9/README.md
+-rw-r--r--   0 michael   (1000) michael   (1000)      990 2023-06-09 16:56:19.000000 TimeForge-0.1.9/pyproject.toml
+-rw-r--r--   0 michael   (1000) michael   (1000)       38 2023-06-09 17:06:32.685666 TimeForge-0.1.9/setup.cfg
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-09 17:06:32.682333 TimeForge-0.1.9/src/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-09 17:06:32.685666 TimeForge-0.1.9/src/TimeForge.egg-info/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1449 2023-06-09 17:06:32.000000 TimeForge-0.1.9/src/TimeForge.egg-info/PKG-INFO
+-rw-r--r--   0 michael   (1000) michael   (1000)      271 2023-06-09 17:06:32.000000 TimeForge-0.1.9/src/TimeForge.egg-info/SOURCES.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-06-09 17:06:32.000000 TimeForge-0.1.9/src/TimeForge.egg-info/dependency_links.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)      103 2023-06-09 17:06:32.000000 TimeForge-0.1.9/src/TimeForge.egg-info/requires.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)       10 2023-06-09 17:06:32.000000 TimeForge-0.1.9/src/TimeForge.egg-info/top_level.txt
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-09 17:06:32.685666 TimeForge-0.1.9/src/timeforge/
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-04-24 11:15:53.000000 TimeForge-0.1.9/src/timeforge/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     6962 2023-06-09 16:38:52.000000 TimeForge-0.1.9/src/timeforge/__main__.py
```

### Comparing `TimeForge-0.1.8/LICENSE.md` & `TimeForge-0.1.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `TimeForge-0.1.8/PKG-INFO` & `TimeForge-0.1.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TimeForge
-Version: 0.1.8
+Version: 0.1.9
 Summary: Create realistic looking but fake time documentation for your student job at KIT
 Author-email: Michael Hohenstein <michael@hohenste.in>
 Project-URL: Homepage, https://github.com/MitchiLaser/timeforge
 Project-URL: Repository, https://github.com/MitchiLaser/timeforge
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Natural Language :: German
@@ -36,8 +36,8 @@
 
 This program has currently only a command line interface. Use
 
 ``` bash
 $ python -m timeforge --help
 ```
 
-to get an overview of the functionality.
+to get an overview of the functionality. The PDF document with the form will be automatically downloaded from the PSE homepage.
```

### Comparing `TimeForge-0.1.8/README.md` & `TimeForge-0.1.9/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -18,8 +18,8 @@
 
 This program has currently only a command line interface. Use
 
 ``` bash
 $ python -m timeforge --help
 ```
 
-to get an overview of the functionality.
+to get an overview of the functionality. The PDF document with the form will be automatically downloaded from the PSE homepage.
```

### Comparing `TimeForge-0.1.8/pyproject.toml` & `TimeForge-0.1.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "TimeForge"
-version = "0.1.8"
+version = "0.1.9"
 authors = [
 	{ name="Michael Hohenstein", email="michael@hohenste.in" },
 ]
 description = "Create realistic looking but fake time documentation for your student job at KIT"
 readme = "README.md"
 requires-python= ">=3.7"
 classifiers = [
@@ -20,15 +20,15 @@
 	"License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
 	"License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
 ]
 dependencies = [
 	"argcomplete >= 3.0.5",
 	"prettytable >= 3.6.0",
 	"wcwidth >= 0.2.6",
-	"deutschland >= 0.3.1",
+	"requests >= 2.31.0",
 	"de-feiertage >= 1.0.1",
 	"pypdf >= 3.8.0",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/MitchiLaser/timeforge"
 "Repository" = "https://github.com/MitchiLaser/timeforge"
```

### Comparing `TimeForge-0.1.8/src/TimeForge.egg-info/PKG-INFO` & `TimeForge-0.1.9/src/TimeForge.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TimeForge
-Version: 0.1.8
+Version: 0.1.9
 Summary: Create realistic looking but fake time documentation for your student job at KIT
 Author-email: Michael Hohenstein <michael@hohenste.in>
 Project-URL: Homepage, https://github.com/MitchiLaser/timeforge
 Project-URL: Repository, https://github.com/MitchiLaser/timeforge
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Natural Language :: German
@@ -36,8 +36,8 @@
 
 This program has currently only a command line interface. Use
 
 ``` bash
 $ python -m timeforge --help
 ```
 
-to get an overview of the functionality.
+to get an overview of the functionality. The PDF document with the form will be automatically downloaded from the PSE homepage.
```

### Comparing `TimeForge-0.1.8/src/timeforge/__main__.py` & `TimeForge-0.1.9/src/timeforge/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -35,17 +35,14 @@
 
 parser.add_argument('-u', action='store_true',
                     help='the Universitätsbereich (UB) field in the form, default: True')
 
 parser.add_argument('-v', '--verbose', action='store_true',
                     help='more detailed information printing for debugging purpose')
 
-parser.add_argument('-i', '--input', type=str, required=True,
-                    help='the location of the input file (The MiLoG-Arbeitszeitdokumentation.pdf from the PSE website)')
-
 parser.add_argument('-o', '--output', type=str, required=True,
                     help='Output File where the content will be written to')
 
 parser.add_argument('-j', '--job', type=str, required=True,
                     help='description of the job task')
 
 argcomplete.autocomplete(parser)
@@ -63,27 +60,28 @@
     tab.add_row(["Working Time", args.time])
     tab.add_row(["Personell number", args.personell])
     tab.add_row(["Salary", str(args.salary) + '€'])
     tab.add_row(["Organisation unit", args.organisation])
     tab.add_row(["GF", args.low_income])
     tab.add_row(["UB", args.u])
     tab.add_row(["Verbose", args.verbose])
-    tab.add_row(["Input File", args.input])
     tab.add_row(["Output-File", args.output])
     tab.add_row(["Job-task", args.job])
     print(tab)
 
 #########################################
 
 # prevent autopep8 from moving these imports to the front
 if True:
     import sys, os
     from deutschland import feiertage
     from deutschland.feiertage.api import default_api
     from pypdf import PdfReader, PdfWriter
+    import tempfile
+    import requests
 
 #########################################
 
 with feiertage.ApiClient() as api_client:
     api_instance = default_api.DefaultApi(api_client)
     nur_land = "BW" # only check for the federal state of Baden-Württemberg
     nur_daten = 1   # dismiss additional information about the day
@@ -143,22 +141,28 @@
 
 if args.verbose:
     print("\nForm Data:")
     pprint(form_data)
 
 #########################################
 
-pdf_reader = PdfReader( open(args.input, 'rb') )
-pdf_writer = PdfWriter()
+with tempfile.TemporaryFile() as temp:
 
-fields = pdf_reader.get_form_text_fields()  # get the field names from the form in the pdf
-for field in fields:                    # fill out all the fields in the form
-    if field in form_data:
-        pdf_writer.update_page_form_field_values(pdf_reader.pages[0],{field: form_data[field]}) 
+    # download online form and store it in a tempfile
+    r = requests.get(r"https://www.pse.kit.edu/downloads/Formulare/KIT%20Arbeitszeitdokumentation%20MiLoG.pdf", allow_redirects=True)
+    temp.write(r.content)
+    temp.seek(0)    # move cursor back to the beginning of the file
+
+    pdf_reader = PdfReader( temp ) #open(temp, 'rb') )
+    pdf_writer = PdfWriter()
+
+    fields = pdf_reader.get_form_text_fields()  # get the field names from the form in the pdf
+    for field in fields:                    # fill out all the fields in the form
+        if field in form_data:
+            pdf_writer.update_page_form_field_values(pdf_reader.pages[0],{field: form_data[field]}) 
 
-pdf_writer.add_page(pdf_reader.pages[0])    # put form content and page in a pdf-writer object
+    pdf_writer.add_page(pdf_reader.pages[0])    # put form content and page in a pdf-writer object
 
 #########################################
 
 with open(args.output, 'wb') as output_file:    # write file
     pdf_writer.write(output_file)
-output_file.close()
```

