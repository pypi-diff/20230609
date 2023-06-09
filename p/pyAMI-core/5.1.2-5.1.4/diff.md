# Comparing `tmp/pyAMI_core-5.1.2.tar.gz` & `tmp/pyAMI_core-5.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyAMI_core-5.1.2.tar", last modified: Tue Nov 10 09:42:43 2020, max compression
+gzip compressed data, was "pyAMI_core-5.1.4.tar", last modified: Fri Jun  9 12:48:32 2023, max compression
```

## Comparing `pyAMI_core-5.1.2.tar` & `pyAMI_core-5.1.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 jodier     (502) staff       (20)        0 2020-11-10 09:42:43.480119 pyAMI_core-5.1.2/
--rw-r--r--   0 jodier     (502) staff       (20)      394 2020-11-10 09:42:43.480325 pyAMI_core-5.1.2/PKG-INFO
--rw-rw-r--   0 jodier     (502) staff       (20)       78 2020-01-24 13:51:33.000000 pyAMI_core-5.1.2/README.md
--rwxrwxr-x   0 jodier     (502) staff       (20)     1077 2020-01-24 13:51:33.000000 pyAMI_core-5.1.2/ami
--rw-rw-r--   0 jodier     (502) staff       (20)       64 2020-01-24 13:51:33.000000 pyAMI_core-5.1.2/ami.bat
-drwxr-xr-x   0 jodier     (502) staff       (20)        0 2020-11-10 09:42:43.477314 pyAMI_core-5.1.2/pyAMI/
--rw-rw-r--   0 jodier     (502) staff       (20)    21862 2020-01-24 13:51:33.000000 pyAMI_core-5.1.2/pyAMI/LICENSE.txt
--rw-r--r--   0 jodier     (502) staff       (20)      652 2019-02-15 10:57:44.000000 pyAMI_core-5.1.2/pyAMI/__init__.py
--rw-r--r--   0 jodier     (502) staff       (20)     7312 2020-01-24 15:21:07.000000 pyAMI_core-5.1.2/pyAMI/app.py
--rw-r--r--   0 jodier     (502) staff       (20)    11340 2020-11-10 09:24:33.000000 pyAMI_core-5.1.2/pyAMI/client.py
--rw-r--r--   0 jodier     (502) staff       (20)     9516 2020-11-10 09:41:37.000000 pyAMI_core-5.1.2/pyAMI/config.py
--rw-r--r--   0 jodier     (502) staff       (20)      789 2019-02-15 10:57:44.000000 pyAMI_core-5.1.2/pyAMI/exception.py
--rw-r--r--   0 jodier     (502) staff       (20)     5131 2020-01-21 10:21:12.000000 pyAMI_core-5.1.2/pyAMI/httpclient.py
--rw-r--r--   0 jodier     (502) staff       (20)     7637 2019-02-15 10:57:44.000000 pyAMI_core-5.1.2/pyAMI/modes.py
--rw-r--r--   0 jodier     (502) staff       (20)     8003 2020-01-23 14:39:10.000000 pyAMI_core-5.1.2/pyAMI/object.py
--rw-r--r--   0 jodier     (502) staff       (20)     1759 2019-02-15 10:57:44.000000 pyAMI_core-5.1.2/pyAMI/transform.py
--rw-r--r--   0 jodier     (502) staff       (20)    13737 2020-01-23 14:38:50.000000 pyAMI_core-5.1.2/pyAMI/utils.py
-drwxr-xr-x   0 jodier     (502) staff       (20)        0 2020-11-10 09:42:43.479754 pyAMI_core-5.1.2/pyAMI_core.egg-info/
--rw-r--r--   0 jodier     (502) staff       (20)      394 2020-11-10 09:42:43.000000 pyAMI_core-5.1.2/pyAMI_core.egg-info/PKG-INFO
--rw-r--r--   0 jodier     (502) staff       (20)      427 2020-11-10 09:42:43.000000 pyAMI_core-5.1.2/pyAMI_core.egg-info/SOURCES.txt
--rw-r--r--   0 jodier     (502) staff       (20)        1 2020-11-10 09:42:43.000000 pyAMI_core-5.1.2/pyAMI_core.egg-info/dependency_links.txt
--rw-r--r--   0 jodier     (502) staff       (20)        1 2020-11-10 09:42:43.000000 pyAMI_core-5.1.2/pyAMI_core.egg-info/not-zip-safe
--rw-r--r--   0 jodier     (502) staff       (20)       32 2020-11-10 09:42:43.000000 pyAMI_core-5.1.2/pyAMI_core.egg-info/requires.txt
--rw-r--r--   0 jodier     (502) staff       (20)        6 2020-11-10 09:42:43.000000 pyAMI_core-5.1.2/pyAMI_core.egg-info/top_level.txt
--rw-rw-r--   0 jodier     (502) staff       (20)       38 2020-11-10 09:42:43.480982 pyAMI_core-5.1.2/setup.cfg
--rw-rw-r--   0 jodier     (502) staff       (20)     1668 2020-01-24 14:13:56.000000 pyAMI_core-5.1.2/setup.py
+drwxr-xr-x   0 jodier     (501) staff       (20)        0 2023-06-09 12:48:32.195056 pyAMI_core-5.1.4/
+-rw-r--r--   0 jodier     (501) staff       (20)      373 2023-06-09 12:48:32.194637 pyAMI_core-5.1.4/PKG-INFO
+-rw-r--r--   0 jodier     (501) staff       (20)       78 2023-06-09 12:43:24.000000 pyAMI_core-5.1.4/README.md
+-rwxr-xr-x   0 jodier     (501) staff       (20)     1077 2023-06-09 12:43:24.000000 pyAMI_core-5.1.4/ami
+-rw-r--r--   0 jodier     (501) staff       (20)       64 2023-06-09 12:43:24.000000 pyAMI_core-5.1.4/ami.bat
+drwxr-xr-x   0 jodier     (501) staff       (20)        0 2023-06-09 12:48:32.189207 pyAMI_core-5.1.4/pyAMI/
+-rw-r--r--   0 jodier     (501) staff       (20)    21862 2023-06-09 12:43:24.000000 pyAMI_core-5.1.4/pyAMI/LICENSE.txt
+-rw-r--r--   0 jodier     (501) staff       (20)      652 2023-06-09 12:43:24.000000 pyAMI_core-5.1.4/pyAMI/__init__.py
+-rw-r--r--   0 jodier     (501) staff       (20)     7312 2023-06-09 12:43:24.000000 pyAMI_core-5.1.4/pyAMI/app.py
+-rw-r--r--   0 jodier     (501) staff       (20)    11340 2023-06-09 12:43:24.000000 pyAMI_core-5.1.4/pyAMI/client.py
+-rw-r--r--   0 jodier     (501) staff       (20)     9516 2023-06-09 12:43:24.000000 pyAMI_core-5.1.4/pyAMI/config.py
+-rw-r--r--   0 jodier     (501) staff       (20)      789 2023-06-09 12:43:24.000000 pyAMI_core-5.1.4/pyAMI/exception.py
+-rw-r--r--   0 jodier     (501) staff       (20)     5131 2023-06-09 12:43:24.000000 pyAMI_core-5.1.4/pyAMI/httpclient.py
+-rw-r--r--   0 jodier     (501) staff       (20)     7637 2023-06-09 12:43:24.000000 pyAMI_core-5.1.4/pyAMI/modes.py
+-rw-r--r--   0 jodier     (501) staff       (20)     8001 2023-06-09 12:43:24.000000 pyAMI_core-5.1.4/pyAMI/object.py
+-rw-r--r--   0 jodier     (501) staff       (20)     1759 2023-06-09 12:43:24.000000 pyAMI_core-5.1.4/pyAMI/transform.py
+-rw-r--r--   0 jodier     (501) staff       (20)    13737 2023-06-09 12:43:24.000000 pyAMI_core-5.1.4/pyAMI/utils.py
+drwxr-xr-x   0 jodier     (501) staff       (20)        0 2023-06-09 12:48:32.194041 pyAMI_core-5.1.4/pyAMI_core.egg-info/
+-rw-r--r--   0 jodier     (501) staff       (20)      373 2023-06-09 12:48:32.000000 pyAMI_core-5.1.4/pyAMI_core.egg-info/PKG-INFO
+-rw-r--r--   0 jodier     (501) staff       (20)      417 2023-06-09 12:48:32.000000 pyAMI_core-5.1.4/pyAMI_core.egg-info/SOURCES.txt
+-rw-r--r--   0 jodier     (501) staff       (20)        1 2023-06-09 12:48:32.000000 pyAMI_core-5.1.4/pyAMI_core.egg-info/dependency_links.txt
+-rw-r--r--   0 jodier     (501) staff       (20)        1 2023-06-09 12:48:32.000000 pyAMI_core-5.1.4/pyAMI_core.egg-info/not-zip-safe
+-rw-r--r--   0 jodier     (501) staff       (20)       23 2023-06-09 12:48:32.000000 pyAMI_core-5.1.4/pyAMI_core.egg-info/requires.txt
+-rw-r--r--   0 jodier     (501) staff       (20)        6 2023-06-09 12:48:32.000000 pyAMI_core-5.1.4/pyAMI_core.egg-info/top_level.txt
+-rw-r--r--   0 jodier     (501) staff       (20)       38 2023-06-09 12:48:32.195200 pyAMI_core-5.1.4/setup.cfg
+-rwxr-xr-x   0 jodier     (501) staff       (20)     1656 2023-06-09 12:43:24.000000 pyAMI_core-5.1.4/setup.py
```

### Comparing `pyAMI_core-5.1.2/ami` & `pyAMI_core-5.1.4/ami`

 * *Files identical despite different names*

### Comparing `pyAMI_core-5.1.2/pyAMI/LICENSE.txt` & `pyAMI_core-5.1.4/pyAMI/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyAMI_core-5.1.2/pyAMI/__init__.py` & `pyAMI_core-5.1.4/pyAMI/__init__.py`

 * *Files identical despite different names*

### Comparing `pyAMI_core-5.1.2/pyAMI/app.py` & `pyAMI_core-5.1.4/pyAMI/app.py`

 * *Files identical despite different names*

### Comparing `pyAMI_core-5.1.2/pyAMI/client.py` & `pyAMI_core-5.1.4/pyAMI/client.py`

 * *Files identical despite different names*

### Comparing `pyAMI_core-5.1.2/pyAMI/config.py` & `pyAMI_core-5.1.4/pyAMI/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 else:
 	import ConfigParser as configparser
 
 #############################################################################
 # GLOBAL DEFINITIONS                                                        #
 #############################################################################
 
-version = '5.1.2'
+version = '5.1.4'
 
 #############################################################################
 
 banner = r'''
               _   __  __ ___    ___
   _ __ _  _  / \ |  \/  |_ _|  | __|
  | '_ \ || |/ ^ \| |\/| || |   |__ \
```

### Comparing `pyAMI_core-5.1.2/pyAMI/exception.py` & `pyAMI_core-5.1.4/pyAMI/exception.py`

 * *Files identical despite different names*

### Comparing `pyAMI_core-5.1.2/pyAMI/httpclient.py` & `pyAMI_core-5.1.4/pyAMI/httpclient.py`

 * *Files identical despite different names*

### Comparing `pyAMI_core-5.1.2/pyAMI/modes.py` & `pyAMI_core-5.1.4/pyAMI/modes.py`

 * *Files identical despite different names*

### Comparing `pyAMI_core-5.1.2/pyAMI/object.py` & `pyAMI_core-5.1.4/pyAMI/object.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,23 +140,23 @@
 
 	#####################################################################
 
 	def get_rows_i(self, rowset_type = None):
 
 		for rowset in self.rowsets:
 
-			if not rowset_type or ((sys.version_info[0] == 3 and ('type' in rowset.attributes)) or (sys.version_info[0] == 2 and rowset.attributes.has_key('type')) and rowset.attributes['type'].value == rowset_type):
+			if not rowset_type or (((sys.version_info[0] == 3 and rowset.hasAttribute('type')) or (sys.version_info[0] == 2 and rowset.attributes.has_key('type'))) and rowset.attributes['type'].value == rowset_type):
 
 				for row in rowset.getElementsByTagName('row'):
 					field_dict = pyAMIDict()
 
 					for field in row.getElementsByTagName('field'):
 						name = field.attributes['name'].value
 
-						if (sys.version_info[0] == 3 and ('table' in field.attributes)) or (sys.version_info[0] == 2 and field.attributes.has_key('table')):
+						if (sys.version_info[0] == 3 and field.hasAttribute('table')) or (sys.version_info[0] == 2 and field.attributes.has_key('table')):
 							table = field.attributes['table'].value
 
 							if self.entity and table and self.entity != table:
 								name = '%s.%s' % (table, name)
 
 						if field.firstChild:
 							field_dict[name] = field.firstChild.nodeValue
```

### Comparing `pyAMI_core-5.1.2/pyAMI/transform.py` & `pyAMI_core-5.1.4/pyAMI/transform.py`

 * *Files identical despite different names*

### Comparing `pyAMI_core-5.1.2/pyAMI/utils.py` & `pyAMI_core-5.1.4/pyAMI/utils.py`

 * *Files identical despite different names*

### Comparing `pyAMI_core-5.1.2/setup.py` & `pyAMI_core-5.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 		author_email = pyAMI.config.author_emails,
 		description = 'Python ATLAS Metadata Interface (pyAMI)',
 		url = 'http://ami.in2p3.fr/',
 		license = 'CeCILL-C',
 		packages = ['pyAMI'],
 		package_data = {'': ['README', 'CHANGELOG', '*.txt'], 'pyAMI': ['*.txt']},
 		scripts = scripts,
-		install_requires = ['argparse', 'argparseplus', 'tiny_xslt'],
+		install_requires = ['argparseplus', 'tiny_xslt'],
 		platforms = 'any',
 		zip_safe = False
 	)
 
 	#####################################################################
 
 	if 'install' in sys.argv:
```

