# Comparing `tmp/orbit_database_shell-0.99.94.tar.gz` & `tmp/orbit_database_shell-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orbit_database_shell-0.99.94.tar", max compression
+gzip compressed data, was "orbit_database_shell-1.0.0.tar", max compression
```

## Comparing `orbit_database_shell-0.99.94.tar` & `orbit_database_shell-1.0.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1099 2023-05-10 11:34:30.904299 orbit_database_shell-0.99.94/LICENSE.md
--rw-r--r--   0        0        0     2272 2023-05-11 16:00:21.773295 orbit_database_shell-0.99.94/README.md
--rwxr-xr-x   0        0        0        0 2023-05-10 11:54:13.621441 orbit_database_shell-0.99.94/orbit_database_shell/__init__.py
--rwxr-xr-x   0        0        0     1876 2023-05-11 15:18:01.901901 orbit_database_shell-0.99.94/orbit_database_shell/__main__.py
--rwxr-xr-x   0        0        0    24822 2023-05-11 15:22:05.776682 orbit_database_shell-0.99.94/orbit_database_shell/odb_actions.py
--rwxr-xr-x   0        0        0     4169 2023-05-10 14:32:56.666736 orbit_database_shell-0.99.94/orbit_database_shell/odb_completers.py
--rw-r--r--   0        0        0     1988 2023-05-11 15:01:59.418713 orbit_database_shell-0.99.94/orbit_database_shell/odb_decorators.py
--rwxr-xr-x   0        0        0     7071 2023-05-11 13:23:09.617433 orbit_database_shell-0.99.94/orbit_database_shell/odb_grammar.py
--rwxr-xr-x   0        0        0    46376 2023-05-11 12:30:35.883941 orbit_database_shell-0.99.94/orbit_database_shell/odb_help.py
--rw-r--r--   0        0        0     1315 2023-05-11 16:01:11.416175 orbit_database_shell-0.99.94/pyproject.toml
--rw-r--r--   0        0        0     3751 1970-01-01 00:00:00.000000 orbit_database_shell-0.99.94/PKG-INFO
+-rw-r--r--   0        0        0     1099 2023-05-30 15:20:01.323993 orbit_database_shell-1.0.0/LICENSE.md
+-rw-r--r--   0        0        0     2272 2023-05-30 15:20:01.323993 orbit_database_shell-1.0.0/README.md
+-rwxr-xr-x   0        0        0        0 2023-05-30 15:20:01.323993 orbit_database_shell-1.0.0/orbit_database_shell/__init__.py
+-rwxr-xr-x   0        0        0     1875 2023-06-09 11:08:38.633578 orbit_database_shell-1.0.0/orbit_database_shell/__main__.py
+-rwxr-xr-x   0        0        0    24822 2023-05-30 15:20:01.323993 orbit_database_shell-1.0.0/orbit_database_shell/odb_actions.py
+-rwxr-xr-x   0        0        0     4169 2023-05-30 15:20:01.323993 orbit_database_shell-1.0.0/orbit_database_shell/odb_completers.py
+-rw-r--r--   0        0        0     1988 2023-05-30 15:20:01.323993 orbit_database_shell-1.0.0/orbit_database_shell/odb_decorators.py
+-rwxr-xr-x   0        0        0     7071 2023-05-30 15:20:01.327993 orbit_database_shell-1.0.0/orbit_database_shell/odb_grammar.py
+-rwxr-xr-x   0        0        0    46376 2023-05-30 15:20:01.327993 orbit_database_shell-1.0.0/orbit_database_shell/odb_help.py
+-rw-r--r--   0        0        0     1309 2023-06-09 11:08:14.666097 orbit_database_shell-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     3693 1970-01-01 00:00:00.000000 orbit_database_shell-1.0.0/PKG-INFO
```

### Comparing `orbit_database_shell-0.99.94/LICENSE.md` & `orbit_database_shell-1.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `orbit_database_shell-0.99.94/README.md` & `orbit_database_shell-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `orbit_database_shell-0.99.94/orbit_database_shell/__main__.py` & `orbit_database_shell-1.0.0/orbit_database_shell/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from orbit_database_shell.odb_decorators import banner
 
 __author__ = 'Gareth Bult'
 __banner__ = 'Orbit-DB'
 __copyright__ = 'Copyright 2023, Mad Penguin Consulting Ltd'
 __credits__ = ['Gareth Bult']
 __license__ = 'MIT'
-__version__ = '0.99.91'
+__version__ = '1.0.0'
 __maintainer__ = 'Gareth Bult'
 __email__ = 'gareth@madpenguin.uk'
 __status__ = 'Development'
 
 
 def main ():
     actions = Actions().notice(banner)
@@ -47,8 +47,8 @@
             continue
         except EOFError:
             break
     actions.info('[shell terminated]')
 
 
 if __name__ == '__main__':
-    main()
+    main()
```

### Comparing `orbit_database_shell-0.99.94/orbit_database_shell/odb_actions.py` & `orbit_database_shell-1.0.0/orbit_database_shell/odb_actions.py`

 * *Files identical despite different names*

### Comparing `orbit_database_shell-0.99.94/orbit_database_shell/odb_completers.py` & `orbit_database_shell-1.0.0/orbit_database_shell/odb_completers.py`

 * *Files identical despite different names*

### Comparing `orbit_database_shell-0.99.94/orbit_database_shell/odb_decorators.py` & `orbit_database_shell-1.0.0/orbit_database_shell/odb_decorators.py`

 * *Files identical despite different names*

### Comparing `orbit_database_shell-0.99.94/orbit_database_shell/odb_grammar.py` & `orbit_database_shell-1.0.0/orbit_database_shell/odb_grammar.py`

 * *Files identical despite different names*

### Comparing `orbit_database_shell-0.99.94/orbit_database_shell/odb_help.py` & `orbit_database_shell-1.0.0/orbit_database_shell/odb_help.py`

 * *Files identical despite different names*

### Comparing `orbit_database_shell-0.99.94/pyproject.toml` & `orbit_database_shell-1.0.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "orbit-database-shell"
-version = "0.99.94"
+version = "1.0.0"
 description = "Orbit-DB Shell"
 authors = ["Gareth Bult <gareth@madpenguin.uk>"]
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
@@ -30,15 +30,15 @@
 ujson = "^5.4.0"
 termcolor = "^1.1.0"
 python-snappy = "^0.6.1"
 loguru = "^0.6.0"
 rich = "^13.3.4"
 mysql-connector-python = "^8.0.33"
 tqdm = "^4.65.0"
-orbit-database = "^0.99.91"
+orbit-database = "^1.0"
 
 [tool.poetry.scripts]
 orbit_database_shell = 'orbit_database_shell.__main__:main'
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `orbit_database_shell-0.99.94/PKG-INFO` & `orbit_database_shell-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 Metadata-Version: 2.1
 Name: orbit-database-shell
-Version: 0.99.94
+Version: 1.0.0
 Summary: Orbit-DB Shell
 Home-page: https://gitlab.com/madpenguin/orbit-database-shell
 Keywords: database,shell
 Author: Gareth Bult
 Author-email: gareth@madpenguin.uk
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console :: Curses
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Database :: Front-Ends
 Classifier: Topic :: File Formats :: JSON
 Requires-Dist: Pygments (>=2.12.0,<3.0.0)
 Requires-Dist: loguru (>=0.6.0,<0.7.0)
 Requires-Dist: mysql-connector-python (>=8.0.33,<9.0.0)
-Requires-Dist: orbit-database (>=0.99.91,<0.100.0)
+Requires-Dist: orbit-database (>=1.0,<2.0)
 Requires-Dist: prompt-toolkit
 Requires-Dist: python-snappy (>=0.6.1,<0.7.0)
 Requires-Dist: rich (>=13.3.4,<14.0.0)
 Requires-Dist: termcolor (>=1.1.0,<2.0.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Requires-Dist: ujson (>=5.4.0,<6.0.0)
 Project-URL: Bug Tracker, https://gitlab.com/madpenguin/orbit-database-shell/-/issues
```

#### html2text {}

```diff
@@ -1,35 +1,34 @@
-Metadata-Version: 2.1 Name: orbit-database-shell Version: 0.99.94 Summary:
-Orbit-DB Shell Home-page: https://gitlab.com/madpenguin/orbit-database-shell
+Metadata-Version: 2.1 Name: orbit-database-shell Version: 1.0.0 Summary: Orbit-
+DB Shell Home-page: https://gitlab.com/madpenguin/orbit-database-shell
 Keywords: database,shell Author: Gareth Bult Author-email: gareth@madpenguin.uk
 Requires-Python: >=3.10,<4.0 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console :: Curses Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Database :: Front-Ends Classifier: Topic :: File Formats
-:: JSON Requires-Dist: Pygments (>=2.12.0,<3.0.0) Requires-Dist: loguru
-(>=0.6.0,<0.7.0) Requires-Dist: mysql-connector-python (>=8.0.33,<9.0.0)
-Requires-Dist: orbit-database (>=0.99.91,<0.100.0) Requires-Dist: prompt-
-toolkit Requires-Dist: python-snappy (>=0.6.1,<0.7.0) Requires-Dist: rich
-(>=13.3.4,<14.0.0) Requires-Dist: termcolor (>=1.1.0,<2.0.0) Requires-Dist:
-tqdm (>=4.65.0,<5.0.0) Requires-Dist: ujson (>=5.4.0,<6.0.0) Project-URL: Bug
-Tracker, https://gitlab.com/madpenguin/orbit-database-shell/-/issues Project-
-URL: Documentation, https://gitlab.com/madpenguin/orbit-database-shell Project-
-URL: Repository, https://gitlab.com/madpenguin/orbit-database-shell
-Description-Content-Type: text/markdown # Orbit Database Shell - Introduction
-#### Welcome to the Orbit Database Shell repository and documentation. All
-project documentation is included within this repository and consists of
-markdown files and comments within the code. These are presented in real time
-by the "ZeroDocs" Orbit application which renders this content to HTML. This
-project is the command line shell for the NoSQL database that underpins the
-Orbit Framework. It performs in much the same way as the MySQL shell other than
-it works with Orbit Databases rather than MySQL databases. Maybe with a few
-other visualisation improvements.
+Language :: Python :: 3.11 Classifier: Topic :: Database :: Front-Ends
+Classifier: Topic :: File Formats :: JSON Requires-Dist: Pygments
+(>=2.12.0,<3.0.0) Requires-Dist: loguru (>=0.6.0,<0.7.0) Requires-Dist: mysql-
+connector-python (>=8.0.33,<9.0.0) Requires-Dist: orbit-database (>=1.0,<2.0)
+Requires-Dist: prompt-toolkit Requires-Dist: python-snappy (>=0.6.1,<0.7.0)
+Requires-Dist: rich (>=13.3.4,<14.0.0) Requires-Dist: termcolor
+(>=1.1.0,<2.0.0) Requires-Dist: tqdm (>=4.65.0,<5.0.0) Requires-Dist: ujson
+(>=5.4.0,<6.0.0) Project-URL: Bug Tracker, https://gitlab.com/madpenguin/orbit-
+database-shell/-/issues Project-URL: Documentation, https://gitlab.com/
+madpenguin/orbit-database-shell Project-URL: Repository, https://gitlab.com/
+madpenguin/orbit-database-shell Description-Content-Type: text/markdown # Orbit
+Database Shell - Introduction #### Welcome to the Orbit Database Shell
+repository and documentation. All project documentation is included within this
+repository and consists of markdown files and comments within the code. These
+are presented in real time by the "ZeroDocs" Orbit application which renders
+this content to HTML. This project is the command line shell for the NoSQL
+database that underpins the Orbit Framework. It performs in much the same way
+as the MySQL shell other than it works with Orbit Databases rather than MySQL
+databases. Maybe with a few other visualisation improvements.
                                       **** Features ****
                                       * The ability to create and manage
                                       multiple databases * Drill-down and
                                       testing facilities * Examine data and
 [https://gitlab.com/madpenguin/orbit- database structures * Import and export
 database-shell/-/raw/main/images/     JSON data, import data directly from
 screenshot.png]                       MySQL * Grammar, colourisation and auto-
```

