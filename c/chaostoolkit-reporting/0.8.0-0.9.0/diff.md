# Comparing `tmp/chaostoolkit-reporting-0.8.0.tar.gz` & `tmp/chaostoolkit-reporting-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/chaostoolkit-reporting-0.8.0.tar", last modified: Mon Jun 25 12:38:35 2018, max compression
+gzip compressed data, was "dist/chaostoolkit-reporting-0.9.0.tar", last modified: Thu Jul 19 05:22:46 2018, max compression
```

## Comparing `chaostoolkit-reporting-0.8.0.tar` & `chaostoolkit-reporting-0.9.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-06-25 12:38:35.000000 chaostoolkit-reporting-0.8.0/
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-06-25 12:38:35.000000 chaostoolkit-reporting-0.8.0/chaosreport/
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-06-25 12:38:35.000000 chaostoolkit-reporting-0.8.0/chaosreport/template/
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-06-25 12:38:35.000000 chaostoolkit-reporting-0.8.0/chaosreport/template/css/
--rw-r--r--   0 travis    (2000) travis    (2000)     3082 2018-06-25 12:37:39.000000 chaostoolkit-reporting-0.8.0/chaosreport/template/css/main.css
--rw-r--r--   0 travis    (2000) travis    (2000)     1981 2018-06-25 12:37:39.000000 chaostoolkit-reporting-0.8.0/chaosreport/template/css/normalize.min.css
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-06-25 12:38:35.000000 chaostoolkit-reporting-0.8.0/chaosreport/template/js/
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-06-25 12:38:35.000000 chaostoolkit-reporting-0.8.0/chaosreport/template/js/vendor/
--rw-r--r--   0 travis    (2000) travis    (2000)    15514 2018-06-25 12:37:39.000000 chaostoolkit-reporting-0.8.0/chaosreport/template/js/vendor/modernizr-2.8.3.min.js
--rw-r--r--   0 travis    (2000) travis    (2000)        1 2018-06-25 12:37:39.000000 chaostoolkit-reporting-0.8.0/chaosreport/template/js/main.js
--rw-r--r--   0 travis    (2000) travis    (2000)     6432 2018-06-25 12:37:39.000000 chaostoolkit-reporting-0.8.0/chaosreport/template/index.md
--rw-r--r--   0 travis    (2000) travis    (2000)     5023 2018-06-25 12:37:39.000000 chaostoolkit-reporting-0.8.0/chaosreport/template/index_to_0.12.2.md
--rw-r--r--   0 travis    (2000) travis    (2000)     5921 2018-06-25 12:37:39.000000 chaostoolkit-reporting-0.8.0/chaosreport/template/index_to_0.15.1.md
--rw-r--r--   0 travis    (2000) travis    (2000)    13229 2018-06-25 12:37:39.000000 chaostoolkit-reporting-0.8.0/chaosreport/__init__.py
--rw-r--r--   0 travis    (2000) travis    (2000)      672 2018-06-25 12:37:39.000000 chaostoolkit-reporting-0.8.0/chaosreport/cli.py
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-06-25 12:38:35.000000 chaostoolkit-reporting-0.8.0/chaostoolkit_reporting.egg-info/
--rw-r--r--   0 travis    (2000) travis    (2000)     3811 2018-06-25 12:38:35.000000 chaostoolkit-reporting-0.8.0/chaostoolkit_reporting.egg-info/PKG-INFO
--rw-r--r--   0 travis    (2000) travis    (2000)      704 2018-06-25 12:38:35.000000 chaostoolkit-reporting-0.8.0/chaostoolkit_reporting.egg-info/SOURCES.txt
--rw-r--r--   0 travis    (2000) travis    (2000)        1 2018-06-25 12:38:35.000000 chaostoolkit-reporting-0.8.0/chaostoolkit_reporting.egg-info/dependency_links.txt
--rw-r--r--   0 travis    (2000) travis    (2000)       78 2018-06-25 12:38:35.000000 chaostoolkit-reporting-0.8.0/chaostoolkit_reporting.egg-info/entry_points.txt
--rw-r--r--   0 travis    (2000) travis    (2000)      104 2018-06-25 12:38:35.000000 chaostoolkit-reporting-0.8.0/chaostoolkit_reporting.egg-info/requires.txt
--rw-r--r--   0 travis    (2000) travis    (2000)       12 2018-06-25 12:38:35.000000 chaostoolkit-reporting-0.8.0/chaostoolkit_reporting.egg-info/top_level.txt
--rw-r--r--   0 travis    (2000) travis    (2000)     2975 2018-06-25 12:37:39.000000 chaostoolkit-reporting-0.8.0/CHANGELOG.md
--rw-r--r--   0 travis    (2000) travis    (2000)    11357 2018-06-25 12:37:39.000000 chaostoolkit-reporting-0.8.0/LICENSE
--rw-r--r--   0 travis    (2000) travis    (2000)      168 2018-06-25 12:37:39.000000 chaostoolkit-reporting-0.8.0/MANIFEST.in
--rw-r--r--   0 travis    (2000) travis    (2000)     2255 2018-06-25 12:37:39.000000 chaostoolkit-reporting-0.8.0/README.md
--rw-r--r--   0 travis    (2000) travis    (2000)      177 2018-06-25 12:37:39.000000 chaostoolkit-reporting-0.8.0/pytest.ini
--rw-r--r--   0 travis    (2000) travis    (2000)       56 2018-06-25 12:37:39.000000 chaostoolkit-reporting-0.8.0/requirements-dev.txt
--rw-r--r--   0 travis    (2000) travis    (2000)      103 2018-06-25 12:37:39.000000 chaostoolkit-reporting-0.8.0/requirements.txt
--rw-r--r--   0 travis    (2000) travis    (2000)      149 2018-06-25 12:38:35.000000 chaostoolkit-reporting-0.8.0/setup.cfg
--rw-r--r--   0 travis    (2000) travis    (2000)     2120 2018-06-25 12:37:39.000000 chaostoolkit-reporting-0.8.0/setup.py
--rw-r--r--   0 travis    (2000) travis    (2000)     3811 2018-06-25 12:38:35.000000 chaostoolkit-reporting-0.8.0/PKG-INFO
+drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-07-19 05:22:46.000000 chaostoolkit-reporting-0.9.0/
+drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-07-19 05:22:46.000000 chaostoolkit-reporting-0.9.0/chaosreport/
+drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-07-19 05:22:46.000000 chaostoolkit-reporting-0.9.0/chaosreport/template/
+drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-07-19 05:22:46.000000 chaostoolkit-reporting-0.9.0/chaosreport/template/css/
+-rw-r--r--   0 travis    (2000) travis    (2000)     3082 2018-07-19 05:21:47.000000 chaostoolkit-reporting-0.9.0/chaosreport/template/css/main.css
+-rw-r--r--   0 travis    (2000) travis    (2000)     1981 2018-07-19 05:21:47.000000 chaostoolkit-reporting-0.9.0/chaosreport/template/css/normalize.min.css
+drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-07-19 05:22:46.000000 chaostoolkit-reporting-0.9.0/chaosreport/template/js/
+drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-07-19 05:22:46.000000 chaostoolkit-reporting-0.9.0/chaosreport/template/js/vendor/
+-rw-r--r--   0 travis    (2000) travis    (2000)    15514 2018-07-19 05:21:47.000000 chaostoolkit-reporting-0.9.0/chaosreport/template/js/vendor/modernizr-2.8.3.min.js
+-rw-r--r--   0 travis    (2000) travis    (2000)        1 2018-07-19 05:21:47.000000 chaostoolkit-reporting-0.9.0/chaosreport/template/js/main.js
+-rw-r--r--   0 travis    (2000) travis    (2000)     6478 2018-07-19 05:21:47.000000 chaostoolkit-reporting-0.9.0/chaosreport/template/index.md
+-rw-r--r--   0 travis    (2000) travis    (2000)     5023 2018-07-19 05:21:47.000000 chaostoolkit-reporting-0.9.0/chaosreport/template/index_to_0.12.2.md
+-rw-r--r--   0 travis    (2000) travis    (2000)     5921 2018-07-19 05:21:47.000000 chaostoolkit-reporting-0.9.0/chaosreport/template/index_to_0.15.1.md
+-rw-r--r--   0 travis    (2000) travis    (2000)    13229 2018-07-19 05:21:47.000000 chaostoolkit-reporting-0.9.0/chaosreport/__init__.py
+-rw-r--r--   0 travis    (2000) travis    (2000)      672 2018-07-19 05:21:47.000000 chaostoolkit-reporting-0.9.0/chaosreport/cli.py
+drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-07-19 05:22:46.000000 chaostoolkit-reporting-0.9.0/chaostoolkit_reporting.egg-info/
+-rw-r--r--   0 travis    (2000) travis    (2000)     5847 2018-07-19 05:22:46.000000 chaostoolkit-reporting-0.9.0/chaostoolkit_reporting.egg-info/PKG-INFO
+-rw-r--r--   0 travis    (2000) travis    (2000)      704 2018-07-19 05:22:46.000000 chaostoolkit-reporting-0.9.0/chaostoolkit_reporting.egg-info/SOURCES.txt
+-rw-r--r--   0 travis    (2000) travis    (2000)        1 2018-07-19 05:22:46.000000 chaostoolkit-reporting-0.9.0/chaostoolkit_reporting.egg-info/dependency_links.txt
+-rw-r--r--   0 travis    (2000) travis    (2000)       78 2018-07-19 05:22:46.000000 chaostoolkit-reporting-0.9.0/chaostoolkit_reporting.egg-info/entry_points.txt
+-rw-r--r--   0 travis    (2000) travis    (2000)      104 2018-07-19 05:22:46.000000 chaostoolkit-reporting-0.9.0/chaostoolkit_reporting.egg-info/requires.txt
+-rw-r--r--   0 travis    (2000) travis    (2000)       12 2018-07-19 05:22:46.000000 chaostoolkit-reporting-0.9.0/chaostoolkit_reporting.egg-info/top_level.txt
+-rw-r--r--   0 travis    (2000) travis    (2000)     3232 2018-07-19 05:21:47.000000 chaostoolkit-reporting-0.9.0/CHANGELOG.md
+-rw-r--r--   0 travis    (2000) travis    (2000)    11357 2018-07-19 05:21:47.000000 chaostoolkit-reporting-0.9.0/LICENSE
+-rw-r--r--   0 travis    (2000) travis    (2000)      168 2018-07-19 05:21:47.000000 chaostoolkit-reporting-0.9.0/MANIFEST.in
+-rw-r--r--   0 travis    (2000) travis    (2000)     3811 2018-07-19 05:21:47.000000 chaostoolkit-reporting-0.9.0/README.md
+-rw-r--r--   0 travis    (2000) travis    (2000)      177 2018-07-19 05:21:47.000000 chaostoolkit-reporting-0.9.0/pytest.ini
+-rw-r--r--   0 travis    (2000) travis    (2000)       56 2018-07-19 05:21:47.000000 chaostoolkit-reporting-0.9.0/requirements-dev.txt
+-rw-r--r--   0 travis    (2000) travis    (2000)      103 2018-07-19 05:21:47.000000 chaostoolkit-reporting-0.9.0/requirements.txt
+-rw-r--r--   0 travis    (2000) travis    (2000)      149 2018-07-19 05:22:46.000000 chaostoolkit-reporting-0.9.0/setup.cfg
+-rw-r--r--   0 travis    (2000) travis    (2000)     2120 2018-07-19 05:21:47.000000 chaostoolkit-reporting-0.9.0/setup.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     5847 2018-07-19 05:22:46.000000 chaostoolkit-reporting-0.9.0/PKG-INFO
```

### Comparing `chaostoolkit-reporting-0.8.0/chaosreport/template/css/main.css` & `chaostoolkit-reporting-0.9.0/chaosreport/template/css/main.css`

 * *Files identical despite different names*

### Comparing `chaostoolkit-reporting-0.8.0/chaosreport/template/css/normalize.min.css` & `chaostoolkit-reporting-0.9.0/chaosreport/template/css/normalize.min.css`

 * *Files identical despite different names*

### Comparing `chaostoolkit-reporting-0.8.0/chaosreport/template/js/vendor/modernizr-2.8.3.min.js` & `chaostoolkit-reporting-0.9.0/chaosreport/template/js/vendor/modernizr-2.8.3.min.js`

 * *Files identical despite different names*

### Comparing `chaostoolkit-reporting-0.8.0/chaosreport/template/index.md` & `chaostoolkit-reporting-0.9.0/chaosreport/template/index.md`

 * *Files 2% similar despite different names*

```diff
@@ -128,18 +128,20 @@
 {% endif %}
 
 {% if item.exception %}
 The *{{item.activity.name}}* {{item.activity.type}} raised the following error
 while running:
 
 {% if export_format == "pdf" %}
-{{item.exception[0]|wordwrap}}
+```python
+{{item.exception|join|wordwrap(70, break_long_words=False)}}
+```
 {% else %}
 ```python
-{{item.exception[0]}}
+{{item.exception|join}}
 ```
 {% endif %}
 {% endif %}
 
 {%if item.text %}
   {% if export_format not in ["html", "html5"] %}
 ```
```

### Comparing `chaostoolkit-reporting-0.8.0/chaosreport/template/index_to_0.12.2.md` & `chaostoolkit-reporting-0.9.0/chaosreport/template/index_to_0.12.2.md`

 * *Files identical despite different names*

### Comparing `chaostoolkit-reporting-0.8.0/chaosreport/template/index_to_0.15.1.md` & `chaostoolkit-reporting-0.9.0/chaosreport/template/index_to_0.15.1.md`

 * *Files identical despite different names*

### Comparing `chaostoolkit-reporting-0.8.0/chaosreport/__init__.py` & `chaostoolkit-reporting-0.9.0/chaosreport/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from natural import date
 import pygal
 from pygal.style import DefaultStyle
 import pypandoc
 import semver
 
 __all__ = ["__version__", "generate_report"]
-__version__ = '0.8.0'
+__version__ = '0.9.0'
 
 curdir = os.getcwd()
 basedir = os.path.dirname(__file__)
 css_dir = os.path.join(basedir, "template", "css")
 js_dir = os.path.join(basedir, "template", "js")
```

### Comparing `chaostoolkit-reporting-0.8.0/chaosreport/cli.py` & `chaostoolkit-reporting-0.9.0/chaosreport/cli.py`

 * *Files identical despite different names*

### Comparing `chaostoolkit-reporting-0.8.0/chaostoolkit_reporting.egg-info/SOURCES.txt` & `chaostoolkit-reporting-0.9.0/chaostoolkit_reporting.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chaostoolkit-reporting-0.8.0/CHANGELOG.md` & `chaostoolkit-reporting-0.9.0/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,24 @@
 # Changelog
 
 ## [Unreleased][]
 
-[Unreleased]: https://github.com/chaostoolkit/chaostoolkit-reporting/compare/0.8.0...HEAD
+[Unreleased]: https://github.com/chaostoolkit/chaostoolkit-reporting/compare/0.9.0...HEAD
+
+## [0.9.0][] - 2018-07-19
+
+[0.9.0]: https://github.com/chaostoolkit/chaostoolkit-reporting/compare/0.8.0...0.9.0
+
+### Added
+
+-   a Dockerfile to build an image with all the system-wide dependencies
+
+### Changed
+
+-   Showing entire exception in PDF reports
 
 ## [0.8.0][] - 2018-06-25
 
 [0.8.0]: https://github.com/chaostoolkit/chaostoolkit-reporting/compare/0.7.1...0.8.0
 
 ### Added
```

### Comparing `chaostoolkit-reporting-0.8.0/LICENSE` & `chaostoolkit-reporting-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `chaostoolkit-reporting-0.8.0/README.md` & `chaostoolkit-reporting-0.9.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -44,14 +44,24 @@
 $ sudo apt-get install texlive-latex-base \
     texlive-fonts-recommended \
     texlive-fonts-extra \
     texlive-latex-extra \
     pdflatex
 ```
 
+### Download a Docker Image
+
+As the dependencies for this plugin can be difficult to get right, we also
+provide a docker image. Note that this image is rather big with 1.4Gb to
+pull.
+
+```console
+$ docker pull chaostoolkit/reporting
+```
+
 ## Usage
 
 Once installed, a new `report` subcommand will be made available to the
 `chaos` command, use it as follows:
 
 ```
 $ chaos report --export-format=html5 chaos-report.json report.html
@@ -59,14 +69,64 @@
 
 or, for a PDF document:
 
 ```
 $ chaos report --export-format=pdf chaos-report.json report.pdf
 ```
 
+### Use a Docker container
+
+To generate a PDF report using the Docker image:
+
+```console
+$ ls .
+journal.json
+
+$ docker run \
+    --user `id -u` \
+    -v `pwd`:/tmp/result \
+    -it \
+    chaostoolkit/reporting
+
+$ ls .
+journal.json report.pdf chaostoolkit.log
+```
+
+As you can see, you should run that command from where the `journal.json`
+file, generated during an experiment run, can be found. This will create a
+`report.pdf` in this directory.
+
+The file will be owned by the user id returned by the command `id -u`, it should
+be your user. The reason we specify a user is that, by default, the container
+runs as root and the image doesn't make a guess about which user will run
+the container. If you don't have the `id` command you can set the value
+manually as follows instead: `--user 1000:1000` assuming both your user and
+group ids are `1000`.
+
+The default command of the image is equivalent to running this without a
+container:
+
+```console
+$ chaos report --export-format=pdf journal.json report.pdf
+```
+
+If you wish to override that command, pass the `chaos report` parameters as
+follows:
+
+```console
+$ docker run \
+    --user `id -u` \
+    -v `pwd`:/tmp/result \
+    -it \
+    chaostoolkit/reporting -- report --export-format=html5 journal.json report.html
+
+$ ls .
+journal.json report.html chaostoolkit.log
+```
+
 ## Contribute
 
 Contributors to this project are welcome as this is an open-source effort that
 seeks [discussions][join] and continuous improvement.
 
 [join]: https://join.chaostoolkit.org/
```

### Comparing `chaostoolkit-reporting-0.8.0/setup.py` & `chaostoolkit-reporting-0.9.0/setup.py`

 * *Files identical despite different names*

