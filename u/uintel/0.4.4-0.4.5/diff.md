# Comparing `tmp/uintel-0.4.4.tar.gz` & `tmp/uintel-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uintel-0.4.4.tar", last modified: Wed Jun  7 04:00:51 2023, max compression
+gzip compressed data, was "uintel-0.4.5.tar", last modified: Fri Jun  9 03:24:31 2023, max compression
```

## Comparing `uintel-0.4.4.tar` & `uintel-0.4.5.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2023-06-07 04:00:51.632149 uintel-0.4.4/
--rw-rw-r--   0 sam       (1000) sam       (1000)     1075 2023-04-03 04:47:18.000000 uintel-0.4.4/LICENSE
--rw-rw-r--   0 sam       (1000) sam       (1000)     4036 2023-06-07 04:00:51.632149 uintel-0.4.4/PKG-INFO
--rw-rw-r--   0 sam       (1000) sam       (1000)     3274 2023-04-03 04:47:18.000000 uintel-0.4.4/README.md
--rw-rw-r--   0 sam       (1000) sam       (1000)       95 2023-04-03 04:47:18.000000 uintel-0.4.4/pyproject.toml
--rw-rw-r--   0 sam       (1000) sam       (1000)       38 2023-06-07 04:00:51.632149 uintel-0.4.4/setup.cfg
--rw-rw-r--   0 sam       (1000) sam       (1000)     1560 2023-06-07 04:00:35.000000 uintel-0.4.4/setup.py
-drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2023-06-07 04:00:51.632149 uintel-0.4.4/src/
-drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2023-06-07 04:00:51.632149 uintel-0.4.4/src/uintel/
--rw-rw-r--   0 sam       (1000) sam       (1000)     3030 2023-04-03 04:47:18.000000 uintel-0.4.4/src/uintel/__init__.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     7978 2023-05-05 02:33:43.000000 uintel-0.4.4/src/uintel/aws.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     4657 2023-04-03 04:47:18.000000 uintel-0.4.4/src/uintel/colours.py
--rw-rw-r--   0 sam       (1000) sam       (1000)    10626 2023-05-05 02:33:43.000000 uintel-0.4.4/src/uintel/esri.py
-drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2023-06-07 04:00:51.632149 uintel-0.4.4/src/uintel/fonts/
--rw-rw-r--   0 sam       (1000) sam       (1000)    94884 2023-04-03 04:47:18.000000 uintel-0.4.4/src/uintel/fonts/Myriad Pro (TrueType).ttf
--rw-rw-r--   0 sam       (1000) sam       (1000)   208636 2023-04-03 04:47:18.000000 uintel-0.4.4/src/uintel/fonts/Rubik (TrueType).ttf
--rw-rw-r--   0 sam       (1000) sam       (1000)   202424 2023-04-03 04:47:18.000000 uintel-0.4.4/src/uintel/fonts/Rubik Italic (TrueType).ttf
--rw-rw-r--   0 sam       (1000) sam       (1000)    20754 2023-06-07 04:00:00.000000 uintel-0.4.4/src/uintel/geometry.py
--rw-rw-r--   0 sam       (1000) sam       (1000)    23184 2023-04-03 04:47:18.000000 uintel-0.4.4/src/uintel/install.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     2308 2023-04-03 04:47:18.000000 uintel-0.4.4/src/uintel/ogc.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     3808 2023-04-03 04:47:18.000000 uintel-0.4.4/src/uintel/query.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     7934 2023-05-05 02:33:43.000000 uintel-0.4.4/src/uintel/server.py
--rw-rw-r--   0 sam       (1000) sam       (1000)    13281 2023-05-05 02:33:43.000000 uintel-0.4.4/src/uintel/slack.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     6374 2023-05-08 03:59:28.000000 uintel-0.4.4/src/uintel/sql.py
-drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2023-06-07 04:00:51.632149 uintel-0.4.4/src/uintel/styles/
--rw-rw-r--   0 sam       (1000) sam       (1000)     1046 2023-04-03 04:47:18.000000 uintel-0.4.4/src/uintel/styles/ui.mplstyle
-drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2023-06-07 04:00:51.632149 uintel-0.4.4/src/uintel.egg-info/
--rw-rw-r--   0 sam       (1000) sam       (1000)     4036 2023-06-07 04:00:51.000000 uintel-0.4.4/src/uintel.egg-info/PKG-INFO
--rw-rw-r--   0 sam       (1000) sam       (1000)      590 2023-06-07 04:00:51.000000 uintel-0.4.4/src/uintel.egg-info/SOURCES.txt
--rw-rw-r--   0 sam       (1000) sam       (1000)        1 2023-06-07 04:00:51.000000 uintel-0.4.4/src/uintel.egg-info/dependency_links.txt
--rw-rw-r--   0 sam       (1000) sam       (1000)      158 2023-06-07 04:00:51.000000 uintel-0.4.4/src/uintel.egg-info/requires.txt
--rw-rw-r--   0 sam       (1000) sam       (1000)        7 2023-06-07 04:00:51.000000 uintel-0.4.4/src/uintel.egg-info/top_level.txt
+drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2023-06-09 03:24:31.284448 uintel-0.4.5/
+-rw-rw-r--   0 sam       (1000) sam       (1000)     1075 2023-04-03 04:47:18.000000 uintel-0.4.5/LICENSE
+-rw-rw-r--   0 sam       (1000) sam       (1000)     4036 2023-06-09 03:24:31.284448 uintel-0.4.5/PKG-INFO
+-rw-rw-r--   0 sam       (1000) sam       (1000)     3274 2023-04-03 04:47:18.000000 uintel-0.4.5/README.md
+-rw-rw-r--   0 sam       (1000) sam       (1000)       95 2023-04-03 04:47:18.000000 uintel-0.4.5/pyproject.toml
+-rw-rw-r--   0 sam       (1000) sam       (1000)       38 2023-06-09 03:24:31.284448 uintel-0.4.5/setup.cfg
+-rw-rw-r--   0 sam       (1000) sam       (1000)     1560 2023-06-09 03:24:20.000000 uintel-0.4.5/setup.py
+drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2023-06-09 03:24:31.276449 uintel-0.4.5/src/
+drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2023-06-09 03:24:31.280449 uintel-0.4.5/src/uintel/
+-rw-rw-r--   0 sam       (1000) sam       (1000)     3030 2023-04-03 04:47:18.000000 uintel-0.4.5/src/uintel/__init__.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)     7978 2023-05-05 02:33:43.000000 uintel-0.4.5/src/uintel/aws.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)     4657 2023-04-03 04:47:18.000000 uintel-0.4.5/src/uintel/colours.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)    10626 2023-05-05 02:33:43.000000 uintel-0.4.5/src/uintel/esri.py
+drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2023-06-09 03:24:31.284448 uintel-0.4.5/src/uintel/fonts/
+-rw-rw-r--   0 sam       (1000) sam       (1000)    94884 2023-04-03 04:47:18.000000 uintel-0.4.5/src/uintel/fonts/Myriad Pro (TrueType).ttf
+-rw-rw-r--   0 sam       (1000) sam       (1000)   208636 2023-04-03 04:47:18.000000 uintel-0.4.5/src/uintel/fonts/Rubik (TrueType).ttf
+-rw-rw-r--   0 sam       (1000) sam       (1000)   202424 2023-04-03 04:47:18.000000 uintel-0.4.5/src/uintel/fonts/Rubik Italic (TrueType).ttf
+-rw-rw-r--   0 sam       (1000) sam       (1000)    20754 2023-06-07 04:00:00.000000 uintel-0.4.5/src/uintel/geometry.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)    23184 2023-04-03 04:47:18.000000 uintel-0.4.5/src/uintel/install.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)     2308 2023-04-03 04:47:18.000000 uintel-0.4.5/src/uintel/ogc.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)     3808 2023-04-03 04:47:18.000000 uintel-0.4.5/src/uintel/query.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)     7934 2023-05-05 02:33:43.000000 uintel-0.4.5/src/uintel/server.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)    13281 2023-05-05 02:33:43.000000 uintel-0.4.5/src/uintel/slack.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)     6388 2023-06-09 03:24:12.000000 uintel-0.4.5/src/uintel/sql.py
+drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2023-06-09 03:24:31.284448 uintel-0.4.5/src/uintel/styles/
+-rw-rw-r--   0 sam       (1000) sam       (1000)     1046 2023-04-03 04:47:18.000000 uintel-0.4.5/src/uintel/styles/ui.mplstyle
+drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2023-06-09 03:24:31.284448 uintel-0.4.5/src/uintel.egg-info/
+-rw-rw-r--   0 sam       (1000) sam       (1000)     4036 2023-06-09 03:24:31.000000 uintel-0.4.5/src/uintel.egg-info/PKG-INFO
+-rw-rw-r--   0 sam       (1000) sam       (1000)      590 2023-06-09 03:24:31.000000 uintel-0.4.5/src/uintel.egg-info/SOURCES.txt
+-rw-rw-r--   0 sam       (1000) sam       (1000)        1 2023-06-09 03:24:31.000000 uintel-0.4.5/src/uintel.egg-info/dependency_links.txt
+-rw-rw-r--   0 sam       (1000) sam       (1000)      158 2023-06-09 03:24:31.000000 uintel-0.4.5/src/uintel.egg-info/requires.txt
+-rw-rw-r--   0 sam       (1000) sam       (1000)        7 2023-06-09 03:24:31.000000 uintel-0.4.5/src/uintel.egg-info/top_level.txt
```

### Comparing `uintel-0.4.4/LICENSE` & `uintel-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `uintel-0.4.4/PKG-INFO` & `uintel-0.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uintel
-Version: 0.4.4
+Version: 0.4.5
 Summary: Urban Intelligence's unified Python data analysis toolkit
 Home-page: https://uintel.github.io/pyui/
 Author: Sam Archie
 Author-email: sam.archie@urbanintelligence.co.nz
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `uintel-0.4.4/README.md` & `uintel-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `uintel-0.4.4/setup.py` & `uintel-0.4.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 setuptools.setup(
     # State the generic information about the package
     name='uintel',
-    version='0.4.4',
+    version='0.4.5',
     author="Sam Archie",
     author_email="sam.archie@urbanintelligence.co.nz",
     description="Urban Intelligence's unified Python data analysis toolkit",
     long_description=open('README.md').read().replace("docs/images/blue_logo.svg", "https://urbanintelligence.co.nz/wp-content/uploads/2022/05/Artboard-1-copy-23.svg"),
     long_description_content_type='text/markdown',
     license="MIT",
     url="https://uintel.github.io/pyui/",
```

### Comparing `uintel-0.4.4/src/uintel/__init__.py` & `uintel-0.4.5/src/uintel/__init__.py`

 * *Files identical despite different names*

### Comparing `uintel-0.4.4/src/uintel/aws.py` & `uintel-0.4.5/src/uintel/aws.py`

 * *Files identical despite different names*

### Comparing `uintel-0.4.4/src/uintel/colours.py` & `uintel-0.4.5/src/uintel/colours.py`

 * *Files identical despite different names*

### Comparing `uintel-0.4.4/src/uintel/esri.py` & `uintel-0.4.5/src/uintel/esri.py`

 * *Files identical despite different names*

### Comparing `uintel-0.4.4/src/uintel/fonts/Myriad Pro (TrueType).ttf` & `uintel-0.4.5/src/uintel/fonts/Myriad Pro (TrueType).ttf`

 * *Files identical despite different names*

### Comparing `uintel-0.4.4/src/uintel/fonts/Rubik (TrueType).ttf` & `uintel-0.4.5/src/uintel/fonts/Rubik (TrueType).ttf`

 * *Files identical despite different names*

### Comparing `uintel-0.4.4/src/uintel/fonts/Rubik Italic (TrueType).ttf` & `uintel-0.4.5/src/uintel/fonts/Rubik Italic (TrueType).ttf`

 * *Files identical despite different names*

### Comparing `uintel-0.4.4/src/uintel/geometry.py` & `uintel-0.4.5/src/uintel/geometry.py`

 * *Files identical despite different names*

### Comparing `uintel-0.4.4/src/uintel/install.py` & `uintel-0.4.5/src/uintel/install.py`

 * *Files identical despite different names*

### Comparing `uintel-0.4.4/src/uintel/ogc.py` & `uintel-0.4.5/src/uintel/ogc.py`

 * *Files identical despite different names*

### Comparing `uintel-0.4.4/src/uintel/query.py` & `uintel-0.4.5/src/uintel/query.py`

 * *Files identical despite different names*

### Comparing `uintel-0.4.4/src/uintel/server.py` & `uintel-0.4.5/src/uintel/server.py`

 * *Files identical despite different names*

### Comparing `uintel-0.4.4/src/uintel/slack.py` & `uintel-0.4.5/src/uintel/slack.py`

 * *Files identical despite different names*

### Comparing `uintel-0.4.4/src/uintel/sql.py` & `uintel-0.4.5/src/uintel/sql.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,22 +93,22 @@
         None.
     """
 
     # Connect to the postgres table (poentially using SSL) and create the new table
     url = sqlalchemy_utils.functions.database._set_url_database(engine.url, "postgres")
     engine = sqlalchemy.create_engine(url, isolation_level='AUTOCOMMIT', connect_args=connect_args)
     with engine.begin() as conn:
-        conn.execute(sqlalchemy.text(f"CREATE DATABASE {database_name} ENCODING 'utf8' TEMPLATE template1"))
+        _ = conn.execute(sqlalchemy.text(f"""CREATE DATABASE "{database_name}" ENCODING 'utf8' TEMPLATE template1"""))
     engine.dispose()
     
     # Connect to the new database (potentially using SSL) and enable the postgis extension
     url = sqlalchemy_utils.functions.database._set_url_database(engine.url, database_name)
     engine = sqlalchemy.create_engine(url, isolation_level='AUTOCOMMIT', connect_args=connect_args)
     with engine.begin() as conn:
-        conn.execute(sqlalchemy.text("CREATE EXTENSION postgis"))
+        _ = conn.execute(sqlalchemy.text("CREATE EXTENSION postgis"))
     engine.dispose()
 
 
 def upload(df: pandas.DataFrame, table_name: str, db: dict, if_exists: str = "replace") -> None:
     """Upload a DataFrame.
 
     Upload a Pandas Dataframe to a SQL table called table_name.
```

### Comparing `uintel-0.4.4/src/uintel/styles/ui.mplstyle` & `uintel-0.4.5/src/uintel/styles/ui.mplstyle`

 * *Files identical despite different names*

### Comparing `uintel-0.4.4/src/uintel.egg-info/PKG-INFO` & `uintel-0.4.5/src/uintel.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uintel
-Version: 0.4.4
+Version: 0.4.5
 Summary: Urban Intelligence's unified Python data analysis toolkit
 Home-page: https://uintel.github.io/pyui/
 Author: Sam Archie
 Author-email: sam.archie@urbanintelligence.co.nz
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `uintel-0.4.4/src/uintel.egg-info/SOURCES.txt` & `uintel-0.4.5/src/uintel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

