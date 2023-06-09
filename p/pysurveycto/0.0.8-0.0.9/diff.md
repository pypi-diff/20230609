# Comparing `tmp/pysurveycto-0.0.8.tar.gz` & `tmp/pysurveycto-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pysurveycto-0.0.8.tar", last modified: Mon Mar  8 09:22:07 2021, max compression
+gzip compressed data, was "dist/pysurveycto-0.0.9.tar", last modified: Mon Mar  8 09:50:29 2021, max compression
```

## Comparing `pysurveycto-0.0.8.tar` & `pysurveycto-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 jeenuthomas   (501) staff       (20)        0 2021-03-08 09:22:07.000000 pysurveycto-0.0.8/
--rw-r--r--   0 jeenuthomas   (501) staff       (20)     8694 2021-03-08 09:22:07.000000 pysurveycto-0.0.8/PKG-INFO
--rw-r--r--   0 jeenuthomas   (501) staff       (20)     6036 2021-03-08 08:42:14.000000 pysurveycto-0.0.8/README.md
--rw-r--r--   0 jeenuthomas   (501) staff       (20)     6342 2021-03-08 08:42:14.000000 pysurveycto-0.0.8/README.rst
-drwxr-xr-x   0 jeenuthomas   (501) staff       (20)        0 2021-03-08 09:22:07.000000 pysurveycto-0.0.8/pysurveycto/
--rw-r--r--   0 jeenuthomas   (501) staff       (20)      476 2020-09-04 08:22:19.000000 pysurveycto-0.0.8/pysurveycto/__init__.py
--rw-r--r--   0 jeenuthomas   (501) staff       (20)    25229 2020-10-12 10:54:20.000000 pysurveycto-0.0.8/pysurveycto/pysurveycto.py
-drwxr-xr-x   0 jeenuthomas   (501) staff       (20)        0 2021-03-08 09:22:07.000000 pysurveycto-0.0.8/pysurveycto.egg-info/
--rw-r--r--   0 jeenuthomas   (501) staff       (20)     8694 2021-03-08 09:22:07.000000 pysurveycto-0.0.8/pysurveycto.egg-info/PKG-INFO
--rw-r--r--   0 jeenuthomas   (501) staff       (20)      254 2021-03-08 09:22:07.000000 pysurveycto-0.0.8/pysurveycto.egg-info/SOURCES.txt
--rw-r--r--   0 jeenuthomas   (501) staff       (20)        1 2021-03-08 09:22:07.000000 pysurveycto-0.0.8/pysurveycto.egg-info/dependency_links.txt
--rw-r--r--   0 jeenuthomas   (501) staff       (20)       32 2021-03-08 09:22:07.000000 pysurveycto-0.0.8/pysurveycto.egg-info/requires.txt
--rw-r--r--   0 jeenuthomas   (501) staff       (20)       12 2021-03-08 09:22:07.000000 pysurveycto-0.0.8/pysurveycto.egg-info/top_level.txt
--rw-r--r--   0 jeenuthomas   (501) staff       (20)       38 2021-03-08 09:22:07.000000 pysurveycto-0.0.8/setup.cfg
--rw-r--r--   0 jeenuthomas   (501) staff       (20)     1054 2021-03-08 09:22:01.000000 pysurveycto-0.0.8/setup.py
+drwxr-xr-x   0 jeenuthomas   (501) staff       (20)        0 2021-03-08 09:50:29.000000 pysurveycto-0.0.9/
+-rw-r--r--   0 jeenuthomas   (501) staff       (20)     8662 2021-03-08 09:50:29.000000 pysurveycto-0.0.9/PKG-INFO
+-rw-r--r--   0 jeenuthomas   (501) staff       (20)     6008 2021-03-08 09:41:47.000000 pysurveycto-0.0.9/README.md
+-rw-r--r--   0 jeenuthomas   (501) staff       (20)     6310 2021-03-08 09:40:19.000000 pysurveycto-0.0.9/README.rst
+drwxr-xr-x   0 jeenuthomas   (501) staff       (20)        0 2021-03-08 09:50:29.000000 pysurveycto-0.0.9/pysurveycto/
+-rw-r--r--   0 jeenuthomas   (501) staff       (20)      476 2020-09-04 08:22:19.000000 pysurveycto-0.0.9/pysurveycto/__init__.py
+-rw-r--r--   0 jeenuthomas   (501) staff       (20)    25229 2020-10-12 10:54:20.000000 pysurveycto-0.0.9/pysurveycto/pysurveycto.py
+drwxr-xr-x   0 jeenuthomas   (501) staff       (20)        0 2021-03-08 09:50:29.000000 pysurveycto-0.0.9/pysurveycto.egg-info/
+-rw-r--r--   0 jeenuthomas   (501) staff       (20)     8662 2021-03-08 09:50:28.000000 pysurveycto-0.0.9/pysurveycto.egg-info/PKG-INFO
+-rw-r--r--   0 jeenuthomas   (501) staff       (20)      254 2021-03-08 09:50:28.000000 pysurveycto-0.0.9/pysurveycto.egg-info/SOURCES.txt
+-rw-r--r--   0 jeenuthomas   (501) staff       (20)        1 2021-03-08 09:50:28.000000 pysurveycto-0.0.9/pysurveycto.egg-info/dependency_links.txt
+-rw-r--r--   0 jeenuthomas   (501) staff       (20)       32 2021-03-08 09:50:28.000000 pysurveycto-0.0.9/pysurveycto.egg-info/requires.txt
+-rw-r--r--   0 jeenuthomas   (501) staff       (20)       12 2021-03-08 09:50:28.000000 pysurveycto-0.0.9/pysurveycto.egg-info/top_level.txt
+-rw-r--r--   0 jeenuthomas   (501) staff       (20)       38 2021-03-08 09:50:29.000000 pysurveycto-0.0.9/setup.cfg
+-rw-r--r--   0 jeenuthomas   (501) staff       (20)     1054 2021-03-08 09:42:58.000000 pysurveycto-0.0.9/setup.py
```

### Comparing `pysurveycto-0.0.8/PKG-INFO` & `pysurveycto-0.0.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: pysurveycto
-Version: 0.0.8
+Version: 0.0.9
 Summary: Interacting with SurveyCTO using Python
 Home-page: https://github.com/IDinsight/surveycto-python/
 Author: Eric Dodge, Jeenu Thomas
 Author-email: it@idinsight.org, Eric.Dodge@idinsight.org, Jeenu.Thomas@idinsight.org
 License: UNKNOWN
 Description: ===========
         pysurveycto
@@ -60,16 +60,16 @@
         Methods:
         --------
         
         -  
           .. code:: python
            
            get_form_data(form_id,
-                         format=’csv’,
-                         shape=’wide’,
+                         format='csv',
+                         shape='wide',
                          oldest_completion_date=None,
                          review_status=None,
                          repeat_groups=None,
                          line_breaks=None,
                          key=False)
         
           Fetch SurveyCTO form data in json or csv formats.
@@ -154,42 +154,42 @@
             
              scto.get_form_data(form_id)
         
         
         -  Get a long csv with all repeat groups (Returns a dictionary with repeat group names as keys and csv data for the repeat groups as values)
             .. code:: python
             
-             scto.get_form_data(form_id, shape=’long’)
+             scto.get_form_data(form_id, shape='long')
         
         -  Get a long csv without repeat groups
             .. code:: python
             
-             scto.get_form_data(form_id, shape=’long’, repeat_groups=false)
+             scto.get_form_data(form_id, shape='long', repeat_groups=false)
         
         -  Get a wide csv with line breaks replaced with space with only pending-review submissions
             .. code:: python
             
              scto.get_form_data(form_id, line_breaks=' ', review_status=['pending'])
         
         -  Get a wide json
             .. code:: python
             
-             scto.get_form_data(form_id, format=’json’)
+             scto.get_form_data(form_id, format='json')
         
         -  Get a wide json with forms completed after a given date (exclusive)
             .. code:: python
             
              date_input = datetime.datetime(2020, 1, 12, 13, 42, 42)
-             scto.get_form_data(form_id, format=’json’, oldest_completion_date=date_input)
+             scto.get_form_data(form_id, format='json', oldest_completion_date=date_input)
         
         -  Get a wide json for encrypted form starting after a given CompletionDate
             .. code:: python
             
              key_data = open('<path to keyfile>', 'rb')
-             scto.get_form_data(form_id, format=’json’, oldest_completion_date=my_datetime, key=key_data)
+             scto.get_form_data(form_id, format='json', oldest_completion_date=my_datetime, key=key_data)
         
         -  Get a server dataset with line breaks replaced with space
             .. code:: python
             
              scto.get_form_data(dataset_id, line_breaks=' ')
         
         -  Get a media file attachment and save to file
@@ -208,15 +208,15 @@
         
         SCTO API Options
         ================
         
         `SCTO API Documentation`_
         
         
-        .. _The MIT License (MIT): https://github.com/IDinsight/surveycto-python/blob/readme_rst/LICENSE.md
+        .. _The MIT License (MIT): https://github.com/IDinsight/surveycto-python/blob/master/LICENSE.md
         .. _SCTO API Documentation: https://support.surveycto.com/hc/en-us/articles/360033156894?flash_digest=0a6eded7694409181788cc46a7026897850d65b5&flash_digest=d76dde7c3ffc40f4a7f0ebd87596d32f3a52304f
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `pysurveycto-0.0.8/README.md` & `pysurveycto-0.0.9/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -40,16 +40,16 @@
 
 
 ## Methods:
 
 * 
   ```python
   get_form_data(form_id, 
-                format=’csv’, 
-                shape=’wide’, 
+                format='csv', 
+                shape='wide', 
                 oldest_completion_date=None, 
                 review_status=None, 
                 repeat_groups=None, 
                 line_breaks=None, 
                 key=False)
   ```
   <p>Fetch SurveyCTO form data in json or csv formats.
@@ -128,42 +128,42 @@
 - Get a wide csv
   ```python
   scto.get_form_data(form_id)
   ```
 
 - Get a long csv with all repeat groups (Returns a dictionary with repeat group names as keys and csv data for the repeat groups as values)
   ```python
-  scto.get_form_data(form_id, shape=’long’)
+  scto.get_form_data(form_id, shape='long')
   ```
 
 - Get a long csv without repeat groups
   ```python
-  scto.get_form_data(form_id, shape=’long’, repeat_groups=false)
+  scto.get_form_data(form_id, shape='long', repeat_groups=false)
   ```
 
 - Get a wide csv with line breaks replaced with space with only pending-review submissions
   ```python
   scto.get_form_data(form_id, line_breaks=' ', review_status=['pending'])
   ```
 
 - Get a wide json
   ```python
-  scto.get_form_data(form_id, format=’json’)
+  scto.get_form_data(form_id, format='json')
   ```
 
 - Get a wide json with forms completed after a given date (exclusive)
   ```python
   date_input = datetime.datetime(2020, 1, 12, 13, 42, 42)
-  scto.get_form_data(form_id, format=’json’, oldest_completion_date=date_input)
+  scto.get_form_data(form_id, format='json', oldest_completion_date=date_input)
   ```
 
 - Get a wide json for encrypted form starting after a given CompletionDate
   ```python
   key_data = open('<path to keyfile>', 'rb')
-  scto.get_form_data(form_id, format=’json’, oldest_completion_date=my_datetime, key=key_data)
+  scto.get_form_data(form_id, format='json', oldest_completion_date=my_datetime, key=key_data)
   ```
 
 - Get a server dataset with line breaks replaced with space
   ```python
   scto.get_form_data(dataset_id, line_breaks=' ')
   ```
```

### Comparing `pysurveycto-0.0.8/README.rst` & `pysurveycto-0.0.9/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -52,16 +52,16 @@
 Methods:
 --------
 
 -  
   .. code:: python
    
    get_form_data(form_id,
-                 format=’csv’,
-                 shape=’wide’,
+                 format='csv',
+                 shape='wide',
                  oldest_completion_date=None,
                  review_status=None,
                  repeat_groups=None,
                  line_breaks=None,
                  key=False)
 
   Fetch SurveyCTO form data in json or csv formats.
@@ -146,42 +146,42 @@
     
      scto.get_form_data(form_id)
 
 
 -  Get a long csv with all repeat groups (Returns a dictionary with repeat group names as keys and csv data for the repeat groups as values)
     .. code:: python
     
-     scto.get_form_data(form_id, shape=’long’)
+     scto.get_form_data(form_id, shape='long')
 
 -  Get a long csv without repeat groups
     .. code:: python
     
-     scto.get_form_data(form_id, shape=’long’, repeat_groups=false)
+     scto.get_form_data(form_id, shape='long', repeat_groups=false)
 
 -  Get a wide csv with line breaks replaced with space with only pending-review submissions
     .. code:: python
     
      scto.get_form_data(form_id, line_breaks=' ', review_status=['pending'])
 
 -  Get a wide json
     .. code:: python
     
-     scto.get_form_data(form_id, format=’json’)
+     scto.get_form_data(form_id, format='json')
 
 -  Get a wide json with forms completed after a given date (exclusive)
     .. code:: python
     
      date_input = datetime.datetime(2020, 1, 12, 13, 42, 42)
-     scto.get_form_data(form_id, format=’json’, oldest_completion_date=date_input)
+     scto.get_form_data(form_id, format='json', oldest_completion_date=date_input)
 
 -  Get a wide json for encrypted form starting after a given CompletionDate
     .. code:: python
     
      key_data = open('<path to keyfile>', 'rb')
-     scto.get_form_data(form_id, format=’json’, oldest_completion_date=my_datetime, key=key_data)
+     scto.get_form_data(form_id, format='json', oldest_completion_date=my_datetime, key=key_data)
 
 -  Get a server dataset with line breaks replaced with space
     .. code:: python
     
      scto.get_form_data(dataset_id, line_breaks=' ')
 
 -  Get a media file attachment and save to file
@@ -200,9 +200,9 @@
 
 SCTO API Options
 ================
 
 `SCTO API Documentation`_
 
 
-.. _The MIT License (MIT): https://github.com/IDinsight/surveycto-python/blob/readme_rst/LICENSE.md
+.. _The MIT License (MIT): https://github.com/IDinsight/surveycto-python/blob/master/LICENSE.md
 .. _SCTO API Documentation: https://support.surveycto.com/hc/en-us/articles/360033156894?flash_digest=0a6eded7694409181788cc46a7026897850d65b5&flash_digest=d76dde7c3ffc40f4a7f0ebd87596d32f3a52304f
```

### Comparing `pysurveycto-0.0.8/pysurveycto/pysurveycto.py` & `pysurveycto-0.0.9/pysurveycto/pysurveycto.py`

 * *Files identical despite different names*

### Comparing `pysurveycto-0.0.8/pysurveycto.egg-info/PKG-INFO` & `pysurveycto-0.0.9/pysurveycto.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: pysurveycto
-Version: 0.0.8
+Version: 0.0.9
 Summary: Interacting with SurveyCTO using Python
 Home-page: https://github.com/IDinsight/surveycto-python/
 Author: Eric Dodge, Jeenu Thomas
 Author-email: it@idinsight.org, Eric.Dodge@idinsight.org, Jeenu.Thomas@idinsight.org
 License: UNKNOWN
 Description: ===========
         pysurveycto
@@ -60,16 +60,16 @@
         Methods:
         --------
         
         -  
           .. code:: python
            
            get_form_data(form_id,
-                         format=’csv’,
-                         shape=’wide’,
+                         format='csv',
+                         shape='wide',
                          oldest_completion_date=None,
                          review_status=None,
                          repeat_groups=None,
                          line_breaks=None,
                          key=False)
         
           Fetch SurveyCTO form data in json or csv formats.
@@ -154,42 +154,42 @@
             
              scto.get_form_data(form_id)
         
         
         -  Get a long csv with all repeat groups (Returns a dictionary with repeat group names as keys and csv data for the repeat groups as values)
             .. code:: python
             
-             scto.get_form_data(form_id, shape=’long’)
+             scto.get_form_data(form_id, shape='long')
         
         -  Get a long csv without repeat groups
             .. code:: python
             
-             scto.get_form_data(form_id, shape=’long’, repeat_groups=false)
+             scto.get_form_data(form_id, shape='long', repeat_groups=false)
         
         -  Get a wide csv with line breaks replaced with space with only pending-review submissions
             .. code:: python
             
              scto.get_form_data(form_id, line_breaks=' ', review_status=['pending'])
         
         -  Get a wide json
             .. code:: python
             
-             scto.get_form_data(form_id, format=’json’)
+             scto.get_form_data(form_id, format='json')
         
         -  Get a wide json with forms completed after a given date (exclusive)
             .. code:: python
             
              date_input = datetime.datetime(2020, 1, 12, 13, 42, 42)
-             scto.get_form_data(form_id, format=’json’, oldest_completion_date=date_input)
+             scto.get_form_data(form_id, format='json', oldest_completion_date=date_input)
         
         -  Get a wide json for encrypted form starting after a given CompletionDate
             .. code:: python
             
              key_data = open('<path to keyfile>', 'rb')
-             scto.get_form_data(form_id, format=’json’, oldest_completion_date=my_datetime, key=key_data)
+             scto.get_form_data(form_id, format='json', oldest_completion_date=my_datetime, key=key_data)
         
         -  Get a server dataset with line breaks replaced with space
             .. code:: python
             
              scto.get_form_data(dataset_id, line_breaks=' ')
         
         -  Get a media file attachment and save to file
@@ -208,15 +208,15 @@
         
         SCTO API Options
         ================
         
         `SCTO API Documentation`_
         
         
-        .. _The MIT License (MIT): https://github.com/IDinsight/surveycto-python/blob/readme_rst/LICENSE.md
+        .. _The MIT License (MIT): https://github.com/IDinsight/surveycto-python/blob/master/LICENSE.md
         .. _SCTO API Documentation: https://support.surveycto.com/hc/en-us/articles/360033156894?flash_digest=0a6eded7694409181788cc46a7026897850d65b5&flash_digest=d76dde7c3ffc40f4a7f0ebd87596d32f3a52304f
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `pysurveycto-0.0.8/setup.py` & `pysurveycto-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import io
 
 dir_path = os.path.abspath(os.path.dirname(__file__))
 long_description = io.open(os.path.join(dir_path, 'README.rst'), encoding='utf-8').read()
 
 setuptools.setup(
     name="pysurveycto",
-    version="0.0.8",
+    version="0.0.9",
     author="Eric Dodge, Jeenu Thomas",
     author_email="it@idinsight.org, Eric.Dodge@idinsight.org, Jeenu.Thomas@idinsight.org",
     description="Interacting with SurveyCTO using Python",
     long_description=long_description,
     url="https://github.com/IDinsight/surveycto-python/",
     packages=setuptools.find_packages(),
     install_requires=[
```

