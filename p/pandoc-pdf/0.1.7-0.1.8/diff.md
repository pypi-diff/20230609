# Comparing `tmp/pandoc_pdf-0.1.7.tar.gz` & `tmp/pandoc_pdf-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandoc_pdf-0.1.7.tar", max compression
+gzip compressed data, was "pandoc_pdf-0.1.8.tar", max compression
```

## Comparing `pandoc_pdf-0.1.7.tar` & `pandoc_pdf-0.1.8.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1060 2022-09-13 12:03:54.627739 pandoc_pdf-0.1.7/LICENSE
--rw-r--r--   0        0        0      688 2022-09-13 12:04:05.167868 pandoc_pdf-0.1.7/pyproject.toml
--rw-r--r--   0        0        0        0 2022-09-13 12:03:54.627739 pandoc_pdf-0.1.7/src/pandoc_pdf/__init__.py
--rw-r--r--   0        0        0     2777 2022-09-13 12:03:54.627739 pandoc_pdf-0.1.7/src/pandoc_pdf/main.py
--rw-r--r--   0        0        0      802 2022-09-13 12:03:54.627739 pandoc_pdf-0.1.7/src/pandoc_pdf_utils/default_config/deeplists.tex
--rw-r--r--   0        0        0      754 2022-09-13 12:03:54.627739 pandoc_pdf-0.1.7/src/pandoc_pdf_utils/default_config/defaults.yml
--rw-r--r--   0        0        0      540 2022-09-13 12:03:54.627739 pandoc_pdf-0.1.7/src/pandoc_pdf_utils/default_config/header.tex
--rw-r--r--   0        0        0      179 2022-09-13 12:03:54.627739 pandoc_pdf-0.1.7/src/pandoc_pdf_utils/default_config/setting.yml
--rw-r--r--   0        0        0      184 2022-09-13 12:03:54.627739 pandoc_pdf-0.1.7/src/pandoc_pdf_utils/env.py
--rw-r--r--   0        0        0     4105 2022-09-13 12:03:54.627739 pandoc_pdf-0.1.7/src/pandoc_pdf_utils/functions.py
--rw-r--r--   0        0        0      920 1970-01-01 00:00:00.000000 pandoc_pdf-0.1.7/setup.py
--rw-r--r--   0        0        0      384 1970-01-01 00:00:00.000000 pandoc_pdf-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1060 2023-06-08 16:04:04.245523 pandoc_pdf-0.1.8/LICENSE
+-rw-r--r--   0        0        0      691 2023-06-08 16:04:16.565677 pandoc_pdf-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-08 16:04:04.245523 pandoc_pdf-0.1.8/src/pandoc_pdf/__init__.py
+-rw-r--r--   0        0        0     2777 2023-06-08 16:04:04.245523 pandoc_pdf-0.1.8/src/pandoc_pdf/main.py
+-rw-r--r--   0        0        0      802 2023-06-08 16:04:04.245523 pandoc_pdf-0.1.8/src/pandoc_pdf_utils/default_config/deeplists.tex
+-rw-r--r--   0        0        0      773 2023-06-08 16:04:04.245523 pandoc_pdf-0.1.8/src/pandoc_pdf_utils/default_config/defaults.yml
+-rw-r--r--   0        0        0      670 2023-06-08 16:04:04.245523 pandoc_pdf-0.1.8/src/pandoc_pdf_utils/default_config/header.tex
+-rw-r--r--   0        0        0      179 2023-06-08 16:04:04.245523 pandoc_pdf-0.1.8/src/pandoc_pdf_utils/default_config/setting.yml
+-rw-r--r--   0        0        0      184 2023-06-08 16:04:04.245523 pandoc_pdf-0.1.8/src/pandoc_pdf_utils/env.py
+-rw-r--r--   0        0        0     4105 2023-06-08 16:04:04.245523 pandoc_pdf-0.1.8/src/pandoc_pdf_utils/functions.py
+-rw-r--r--   0        0        0      920 1970-01-01 00:00:00.000000 pandoc_pdf-0.1.8/setup.py
+-rw-r--r--   0        0        0      384 1970-01-01 00:00:00.000000 pandoc_pdf-0.1.8/PKG-INFO
```

### Comparing `pandoc_pdf-0.1.7/LICENSE` & `pandoc_pdf-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pandoc_pdf-0.1.7/pyproject.toml` & `pandoc_pdf-0.1.8/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -3,29 +3,29 @@
 description = "Command to generate pdf easily with pandoc."
 license = "MIT"
 name = "pandoc_pdf"
 packages = [
   {include = "pandoc_pdf", from = "src"},
   {include = "pandoc_pdf_utils", from = "src"},
 ]
-version = "0.1.7"
+version = "0.1.8"
 
 [tool.poetry.dependencies]
 PyYAML = "^6.0"
 click = "^8.1.3"
 python = "^3.10"
 
 [tool.poetry.dev-dependencies]
 autopep8 = "^1.7.0"
-pytest = "^5.2"
-tomlkit = "^0.11.4"
+pytest = "^5.4.3"
+tomlkit = "^0.11.8"
 
 [tool.poetry.group.dev.dependencies]
-black = {version = "^22.8.0", allow-prereleases = true}
+black = {version = "^22.12.0", allow-prereleases = true}
 autopep8 = "^1.7.0"
 
 [build-system]
 build-backend = "poetry.core.masonry.api"
-requires = ["poetry-core>=1.0.0"]
+requires = ["poetry-core>=1.5.0"]
 
 [tool.poetry.scripts]
 pandoc_pdf = 'pandoc_pdf.main:pandoc_pdf'
```

### Comparing `pandoc_pdf-0.1.7/src/pandoc_pdf/main.py` & `pandoc_pdf-0.1.8/src/pandoc_pdf/main.py`

 * *Files identical despite different names*

### Comparing `pandoc_pdf-0.1.7/src/pandoc_pdf_utils/default_config/deeplists.tex` & `pandoc_pdf-0.1.8/src/pandoc_pdf_utils/default_config/deeplists.tex`

 * *Files identical despite different names*

### Comparing `pandoc_pdf-0.1.7/src/pandoc_pdf_utils/default_config/defaults.yml` & `pandoc_pdf-0.1.8/src/pandoc_pdf_utils/default_config/defaults.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 latex:
-  pdf-engine: xelatex
   to: latex
+  pdf-engine: xelatex
   standalone: true
   listings: true
   variables:
     lang: ja
     luatexjapresetoptions: haranoaji
     classoption: pandoc
   filters:
     - pandoc-crossref
   include-in-header:
     - ${.}/header.tex
     - ${.}/deeplists.tex
   metadata:
+    listings: true
     documentclass: bxjsreport
     geometry: a4paper
     figureTitle: "図"
     tableTitle: "表"
     listingTitle: "コード"
     figPrefix: "図"
     eqnPrefix: "式"
```

### Comparing `pandoc_pdf-0.1.7/src/pandoc_pdf_utils/default_config/header.tex` & `pandoc_pdf-0.1.8/src/pandoc_pdf_utils/default_config/header.tex`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 \usepackage{listings,jvlisting}
 \usepackage{xcolor}
 \usepackage{amsmath,amssymb}
+\usepackage{svg}
+\usepackage[top=25truemm,bottom=30truemm,left=25truemm,right=25truemm]{geometry}
+\addtolength{\footskip}{10mm}
 
 \lstset{
   basicstyle={\ttfamily},
   identifierstyle={\small},
   keywordstyle={\small\bfseries},
   ndkeywordstyle={\small},
   stringstyle={\small\ttfamily},
@@ -16,9 +19,9 @@
   numbersep=10pt,
   tabsize=2,
   extendedchars=true,
   xleftmargin=17pt,
   framexleftmargin=17pt,
   linewidth=\textwidth,
 }
+% \newcommand{\passthrough}[1]{#1}
 \renewcommand{\lstlistingname}{コード}
-\newcommand{\passthrough}[1]{#1}
```

### Comparing `pandoc_pdf-0.1.7/src/pandoc_pdf_utils/functions.py` & `pandoc_pdf-0.1.8/src/pandoc_pdf_utils/functions.py`

 * *Files identical despite different names*

### Comparing `pandoc_pdf-0.1.7/setup.py` & `pandoc_pdf-0.1.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 ['PyYAML>=6.0,<7.0', 'click>=8.1.3,<9.0.0']
 
 entry_points = \
 {'console_scripts': ['pandoc_pdf = pandoc_pdf.main:pandoc_pdf']}
 
 setup_kwargs = {
     'name': 'pandoc-pdf',
-    'version': '0.1.7',
+    'version': '0.1.8',
     'description': 'Command to generate pdf easily with pandoc.',
     'long_description': 'None',
     'author': 'rai',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

