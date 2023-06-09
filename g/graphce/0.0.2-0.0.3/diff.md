# Comparing `tmp/graphce-0.0.2.tar.gz` & `tmp/graphce-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphce-0.0.2.tar", last modified: Fri Jun  9 12:30:18 2023, max compression
+gzip compressed data, was "graphce-0.0.3.tar", last modified: Fri Jun  9 12:43:42 2023, max compression
```

## Comparing `graphce-0.0.2.tar` & `graphce-0.0.3.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 12:30:18.187270 graphce-0.0.2/
--rw-rw-rw-   0        0        0     3165 2023-06-09 12:30:18.184322 graphce-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2972 2023-06-09 11:04:45.000000 graphce-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-09 12:30:18.055454 graphce-0.0.2/database/
--rw-rw-rw-   0        0        0        0 2023-06-05 13:17:20.000000 graphce-0.0.2/database/__init__.py
--rw-rw-rw-   0        0        0      598 2023-06-09 09:10:06.000000 graphce-0.0.2/database/db_creation.py
-drwxrwxrwx   0        0        0        0 2023-06-09 12:30:18.061496 graphce-0.0.2/edges/
--rw-rw-rw-   0        0        0        0 2023-06-09 08:30:46.000000 graphce-0.0.2/edges/__init__.py
--rw-rw-rw-   0        0        0      992 2023-06-09 09:45:27.000000 graphce-0.0.2/edges/edge_manipulation.py
-drwxrwxrwx   0        0        0        0 2023-06-09 12:30:18.067758 graphce-0.0.2/email_data/
--rw-rw-rw-   0        0        0        0 2023-06-05 03:13:07.000000 graphce-0.0.2/email_data/__init__.py
--rw-rw-rw-   0        0        0      691 2023-06-07 04:10:43.000000 graphce-0.0.2/email_data/email.py
-drwxrwxrwx   0        0        0        0 2023-06-09 12:30:18.082342 graphce-0.0.2/email_data/utils/
--rw-rw-rw-   0        0        0        0 2023-06-08 06:06:35.000000 graphce-0.0.2/email_data/utils/__init__.py
--rw-rw-rw-   0        0        0     1577 2023-06-08 06:00:45.000000 graphce-0.0.2/email_data/utils/email_database_manipulation.py
--rw-rw-rw-   0        0        0     5051 2023-06-07 04:19:46.000000 graphce-0.0.2/email_data/utils/email_tree.py
--rw-rw-rw-   0        0        0      322 2023-06-05 08:12:05.000000 graphce-0.0.2/email_data/utils/validator.py
-drwxrwxrwx   0        0        0        0 2023-06-09 12:30:18.087670 graphce-0.0.2/graphce/
--rw-rw-rw-   0        0        0        0 2023-06-08 06:04:45.000000 graphce-0.0.2/graphce/__init__.py
--rw-rw-rw-   0        0        0     3092 2023-06-09 09:44:38.000000 graphce-0.0.2/graphce/tree.py
-drwxrwxrwx   0        0        0        0 2023-06-09 12:30:18.107105 graphce-0.0.2/graphce.egg-info/
--rw-rw-rw-   0        0        0     3165 2023-06-09 12:30:17.000000 graphce-0.0.2/graphce.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      967 2023-06-09 12:30:17.000000 graphce-0.0.2/graphce.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 12:30:17.000000 graphce-0.0.2/graphce.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-06-09 12:30:17.000000 graphce-0.0.2/graphce.egg-info/requires.txt
--rw-rw-rw-   0        0        0       56 2023-06-09 12:30:17.000000 graphce-0.0.2/graphce.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-09 12:30:18.129947 graphce-0.0.2/ip_profile/
--rw-rw-rw-   0        0        0      119 2023-05-02 08:02:02.000000 graphce-0.0.2/ip_profile/__init__.py
--rw-rw-rw-   0        0        0      458 2023-06-05 06:18:34.000000 graphce-0.0.2/ip_profile/exceptions.py
--rw-rw-rw-   0        0        0     2059 2023-06-06 11:11:16.000000 graphce-0.0.2/ip_profile/ip.py
--rw-rw-rw-   0        0        0      356 2023-06-03 16:02:46.000000 graphce-0.0.2/ip_profile/ip_object.py
--rw-rw-rw-   0        0        0     2088 2023-06-06 11:04:38.000000 graphce-0.0.2/ip_profile/ipv4.py
--rw-rw-rw-   0        0        0     2005 2023-05-10 13:22:35.000000 graphce-0.0.2/ip_profile/ipv6.py
-drwxrwxrwx   0        0        0        0 2023-06-09 12:30:18.149863 graphce-0.0.2/ip_profile/utils/
--rw-rw-rw-   0        0        0        0 2023-05-02 08:02:02.000000 graphce-0.0.2/ip_profile/utils/__init__.py
--rw-rw-rw-   0        0        0      246 2023-05-08 08:07:57.000000 graphce-0.0.2/ip_profile/utils/common.py
--rw-rw-rw-   0        0        0     1565 2023-06-08 05:59:27.000000 graphce-0.0.2/ip_profile/utils/ip_data_manipulation.py
--rw-rw-rw-   0        0        0     4675 2023-06-07 03:40:46.000000 graphce-0.0.2/ip_profile/utils/ip_tree.py
--rw-rw-rw-   0        0        0     1913 2023-05-02 08:02:02.000000 graphce-0.0.2/ip_profile/utils/validator.py
-drwxrwxrwx   0        0        0        0 2023-06-09 12:30:18.165747 graphce-0.0.2/phone_data/
--rw-rw-rw-   0        0        0        0 2023-06-02 11:49:11.000000 graphce-0.0.2/phone_data/__init__.py
--rw-rw-rw-   0        0        0      130 2023-06-05 07:06:33.000000 graphce-0.0.2/phone_data/exceptions.py
--rw-rw-rw-   0        0        0      690 2023-06-07 03:40:46.000000 graphce-0.0.2/phone_data/phone.py
-drwxrwxrwx   0        0        0        0 2023-06-09 12:30:18.179640 graphce-0.0.2/phone_data/utils/
--rw-rw-rw-   0        0        0        0 2023-06-08 06:06:49.000000 graphce-0.0.2/phone_data/utils/__init__.py
--rw-rw-rw-   0        0        0     1571 2023-06-08 06:00:45.000000 graphce-0.0.2/phone_data/utils/phone_database_manipulation.py
--rw-rw-rw-   0        0        0     5077 2023-06-07 03:40:46.000000 graphce-0.0.2/phone_data/utils/phone_tree.py
--rw-rw-rw-   0        0        0      489 2023-06-05 07:10:20.000000 graphce-0.0.2/phone_data/utils/validator.py
--rw-rw-rw-   0        0        0       42 2023-06-09 12:30:18.187270 graphce-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      459 2023-06-09 12:30:13.000000 graphce-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 12:43:42.102713 graphce-0.0.3/
+-rw-rw-rw-   0        0        0     3160 2023-06-09 12:43:42.099885 graphce-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2967 2023-06-09 12:41:42.000000 graphce-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-09 12:43:41.939664 graphce-0.0.3/database/
+-rw-rw-rw-   0        0        0        0 2023-06-05 13:17:20.000000 graphce-0.0.3/database/__init__.py
+-rw-rw-rw-   0        0        0      598 2023-06-09 09:10:06.000000 graphce-0.0.3/database/db_creation.py
+drwxrwxrwx   0        0        0        0 2023-06-09 12:43:41.945534 graphce-0.0.3/edges/
+-rw-rw-rw-   0        0        0        0 2023-06-09 08:30:46.000000 graphce-0.0.3/edges/__init__.py
+-rw-rw-rw-   0        0        0      992 2023-06-09 09:45:27.000000 graphce-0.0.3/edges/edge_manipulation.py
+drwxrwxrwx   0        0        0        0 2023-06-09 12:43:41.950865 graphce-0.0.3/email_data/
+-rw-rw-rw-   0        0        0        0 2023-06-05 03:13:07.000000 graphce-0.0.3/email_data/__init__.py
+-rw-rw-rw-   0        0        0      691 2023-06-07 04:10:43.000000 graphce-0.0.3/email_data/email.py
+drwxrwxrwx   0        0        0        0 2023-06-09 12:43:41.972227 graphce-0.0.3/email_data/utils/
+-rw-rw-rw-   0        0        0        0 2023-06-08 06:06:35.000000 graphce-0.0.3/email_data/utils/__init__.py
+-rw-rw-rw-   0        0        0     1577 2023-06-08 06:00:45.000000 graphce-0.0.3/email_data/utils/email_database_manipulation.py
+-rw-rw-rw-   0        0        0     5051 2023-06-07 04:19:46.000000 graphce-0.0.3/email_data/utils/email_tree.py
+-rw-rw-rw-   0        0        0      322 2023-06-05 08:12:05.000000 graphce-0.0.3/email_data/utils/validator.py
+drwxrwxrwx   0        0        0        0 2023-06-09 12:43:41.984991 graphce-0.0.3/graphce/
+-rw-rw-rw-   0        0        0       27 2023-06-09 12:41:10.000000 graphce-0.0.3/graphce/__init__.py
+-rw-rw-rw-   0        0        0     3092 2023-06-09 09:44:38.000000 graphce-0.0.3/graphce/tree.py
+drwxrwxrwx   0        0        0        0 2023-06-09 12:43:42.006501 graphce-0.0.3/graphce.egg-info/
+-rw-rw-rw-   0        0        0     3160 2023-06-09 12:43:41.000000 graphce-0.0.3/graphce.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      967 2023-06-09 12:43:41.000000 graphce-0.0.3/graphce.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 12:43:41.000000 graphce-0.0.3/graphce.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-06-09 12:43:41.000000 graphce-0.0.3/graphce.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       56 2023-06-09 12:43:41.000000 graphce-0.0.3/graphce.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-09 12:43:42.035291 graphce-0.0.3/ip_profile/
+-rw-rw-rw-   0        0        0      119 2023-05-02 08:02:02.000000 graphce-0.0.3/ip_profile/__init__.py
+-rw-rw-rw-   0        0        0      458 2023-06-05 06:18:34.000000 graphce-0.0.3/ip_profile/exceptions.py
+-rw-rw-rw-   0        0        0     2059 2023-06-06 11:11:16.000000 graphce-0.0.3/ip_profile/ip.py
+-rw-rw-rw-   0        0        0      356 2023-06-03 16:02:46.000000 graphce-0.0.3/ip_profile/ip_object.py
+-rw-rw-rw-   0        0        0     2088 2023-06-06 11:04:38.000000 graphce-0.0.3/ip_profile/ipv4.py
+-rw-rw-rw-   0        0        0     2005 2023-05-10 13:22:35.000000 graphce-0.0.3/ip_profile/ipv6.py
+drwxrwxrwx   0        0        0        0 2023-06-09 12:43:42.055201 graphce-0.0.3/ip_profile/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-02 08:02:02.000000 graphce-0.0.3/ip_profile/utils/__init__.py
+-rw-rw-rw-   0        0        0      246 2023-05-08 08:07:57.000000 graphce-0.0.3/ip_profile/utils/common.py
+-rw-rw-rw-   0        0        0     1565 2023-06-08 05:59:27.000000 graphce-0.0.3/ip_profile/utils/ip_data_manipulation.py
+-rw-rw-rw-   0        0        0     4675 2023-06-07 03:40:46.000000 graphce-0.0.3/ip_profile/utils/ip_tree.py
+-rw-rw-rw-   0        0        0     1913 2023-05-02 08:02:02.000000 graphce-0.0.3/ip_profile/utils/validator.py
+drwxrwxrwx   0        0        0        0 2023-06-09 12:43:42.076517 graphce-0.0.3/phone_data/
+-rw-rw-rw-   0        0        0        0 2023-06-02 11:49:11.000000 graphce-0.0.3/phone_data/__init__.py
+-rw-rw-rw-   0        0        0      130 2023-06-05 07:06:33.000000 graphce-0.0.3/phone_data/exceptions.py
+-rw-rw-rw-   0        0        0      690 2023-06-07 03:40:46.000000 graphce-0.0.3/phone_data/phone.py
+drwxrwxrwx   0        0        0        0 2023-06-09 12:43:42.093453 graphce-0.0.3/phone_data/utils/
+-rw-rw-rw-   0        0        0        0 2023-06-08 06:06:49.000000 graphce-0.0.3/phone_data/utils/__init__.py
+-rw-rw-rw-   0        0        0     1571 2023-06-08 06:00:45.000000 graphce-0.0.3/phone_data/utils/phone_database_manipulation.py
+-rw-rw-rw-   0        0        0     5077 2023-06-07 03:40:46.000000 graphce-0.0.3/phone_data/utils/phone_tree.py
+-rw-rw-rw-   0        0        0      489 2023-06-05 07:10:20.000000 graphce-0.0.3/phone_data/utils/validator.py
+-rw-rw-rw-   0        0        0       42 2023-06-09 12:43:42.103721 graphce-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      459 2023-06-09 12:43:35.000000 graphce-0.0.3/setup.py
```

### Comparing `graphce-0.0.2/PKG-INFO` & `graphce-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: graphce
-Version: 0.0.2
+Version: 0.0.3
 Summary: Working with databases related to IP, phone, and email information.
 Author: authsafe
 Description-Content-Type: text/markdown
 
 Readme
 
 This package provides the GraphCE class for working with databases related to IP, phone, and email information.
 
 Usage:
 To use the GraphCE class, import it from the graphce.tree module.
 
 Example:
-from graphce.tree import GraphCE
+from graphce import GraphCE
 
 Creating an Instance:
 To create an instance of GraphCE, provide the following arguments:
 - Type: The type of data you want to work with. Choose from IP, PHONE, or EMAIL.
 - Path: The path of the database where you want to create or use the database.
 
 Note: When creating an instance, a database file with the specified type will be created at the given path. For example, if the type is "IP", it will create a file called "IPs.sqlite" at the specified path. Additionally, an "edges.sqlite" file will also be created at the given path. This file is used for adding, deleting, and updating edges in the graph.
```

### Comparing `graphce-0.0.2/README.md` & `graphce-0.0.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 This package provides the GraphCE class for working with databases related to IP, phone, and email information.
 
 Usage:
 To use the GraphCE class, import it from the graphce.tree module.
 
 Example:
-from graphce.tree import GraphCE
+from graphce import GraphCE
 
 Creating an Instance:
 To create an instance of GraphCE, provide the following arguments:
 - Type: The type of data you want to work with. Choose from IP, PHONE, or EMAIL.
 - Path: The path of the database where you want to create or use the database.
 
 Note: When creating an instance, a database file with the specified type will be created at the given path. For example, if the type is "IP", it will create a file called "IPs.sqlite" at the specified path. Additionally, an "edges.sqlite" file will also be created at the given path. This file is used for adding, deleting, and updating edges in the graph.
```

### Comparing `graphce-0.0.2/database/db_creation.py` & `graphce-0.0.3/database/db_creation.py`

 * *Files identical despite different names*

### Comparing `graphce-0.0.2/edges/edge_manipulation.py` & `graphce-0.0.3/edges/edge_manipulation.py`

 * *Files identical despite different names*

### Comparing `graphce-0.0.2/email_data/email.py` & `graphce-0.0.3/email_data/email.py`

 * *Files identical despite different names*

### Comparing `graphce-0.0.2/email_data/utils/email_database_manipulation.py` & `graphce-0.0.3/email_data/utils/email_database_manipulation.py`

 * *Files identical despite different names*

### Comparing `graphce-0.0.2/email_data/utils/email_tree.py` & `graphce-0.0.3/email_data/utils/email_tree.py`

 * *Files identical despite different names*

### Comparing `graphce-0.0.2/graphce/tree.py` & `graphce-0.0.3/graphce/tree.py`

 * *Files identical despite different names*

### Comparing `graphce-0.0.2/graphce.egg-info/PKG-INFO` & `graphce-0.0.3/graphce.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: graphce
-Version: 0.0.2
+Version: 0.0.3
 Summary: Working with databases related to IP, phone, and email information.
 Author: authsafe
 Description-Content-Type: text/markdown
 
 Readme
 
 This package provides the GraphCE class for working with databases related to IP, phone, and email information.
 
 Usage:
 To use the GraphCE class, import it from the graphce.tree module.
 
 Example:
-from graphce.tree import GraphCE
+from graphce import GraphCE
 
 Creating an Instance:
 To create an instance of GraphCE, provide the following arguments:
 - Type: The type of data you want to work with. Choose from IP, PHONE, or EMAIL.
 - Path: The path of the database where you want to create or use the database.
 
 Note: When creating an instance, a database file with the specified type will be created at the given path. For example, if the type is "IP", it will create a file called "IPs.sqlite" at the specified path. Additionally, an "edges.sqlite" file will also be created at the given path. This file is used for adding, deleting, and updating edges in the graph.
```

### Comparing `graphce-0.0.2/graphce.egg-info/SOURCES.txt` & `graphce-0.0.3/graphce.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `graphce-0.0.2/ip_profile/ip.py` & `graphce-0.0.3/ip_profile/ip.py`

 * *Files identical despite different names*

### Comparing `graphce-0.0.2/ip_profile/ipv4.py` & `graphce-0.0.3/ip_profile/ipv4.py`

 * *Files identical despite different names*

### Comparing `graphce-0.0.2/ip_profile/ipv6.py` & `graphce-0.0.3/ip_profile/ipv6.py`

 * *Files identical despite different names*

### Comparing `graphce-0.0.2/ip_profile/utils/ip_data_manipulation.py` & `graphce-0.0.3/ip_profile/utils/ip_data_manipulation.py`

 * *Files identical despite different names*

### Comparing `graphce-0.0.2/ip_profile/utils/ip_tree.py` & `graphce-0.0.3/ip_profile/utils/ip_tree.py`

 * *Files identical despite different names*

### Comparing `graphce-0.0.2/ip_profile/utils/validator.py` & `graphce-0.0.3/ip_profile/utils/validator.py`

 * *Files identical despite different names*

### Comparing `graphce-0.0.2/phone_data/phone.py` & `graphce-0.0.3/phone_data/phone.py`

 * *Files identical despite different names*

### Comparing `graphce-0.0.2/phone_data/utils/phone_database_manipulation.py` & `graphce-0.0.3/phone_data/utils/phone_database_manipulation.py`

 * *Files identical despite different names*

### Comparing `graphce-0.0.2/phone_data/utils/phone_tree.py` & `graphce-0.0.3/phone_data/utils/phone_tree.py`

 * *Files identical despite different names*

