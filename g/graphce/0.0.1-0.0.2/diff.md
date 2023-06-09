# Comparing `tmp/graphce-0.0.1.tar.gz` & `tmp/graphce-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphce-0.0.1.tar", last modified: Thu Jun  8 07:55:31 2023, max compression
+gzip compressed data, was "graphce-0.0.2.tar", last modified: Fri Jun  9 12:30:18 2023, max compression
```

## Comparing `graphce-0.0.1.tar` & `graphce-0.0.2.tar`

### file list

```diff
@@ -1,45 +1,50 @@
-drwxrwxrwx   0        0        0        0 2023-06-08 07:55:31.482786 graphce-0.0.1/
--rw-rw-rw-   0        0        0      155 2023-06-08 07:55:31.481119 graphce-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-08 07:55:31.276844 graphce-0.0.1/database/
--rw-rw-rw-   0        0        0        0 2023-06-05 13:17:20.000000 graphce-0.0.1/database/__init__.py
--rw-rw-rw-   0        0        0      441 2023-06-08 05:58:29.000000 graphce-0.0.1/database/db_creation.py
-drwxrwxrwx   0        0        0        0 2023-06-08 07:55:31.281002 graphce-0.0.1/email_data/
--rw-rw-rw-   0        0        0        0 2023-06-05 03:13:07.000000 graphce-0.0.1/email_data/__init__.py
--rw-rw-rw-   0        0        0      691 2023-06-07 04:10:43.000000 graphce-0.0.1/email_data/email.py
-drwxrwxrwx   0        0        0        0 2023-06-08 07:55:31.336574 graphce-0.0.1/email_data/utils/
--rw-rw-rw-   0        0        0        0 2023-06-08 06:06:35.000000 graphce-0.0.1/email_data/utils/__init__.py
--rw-rw-rw-   0        0        0     1577 2023-06-08 06:00:45.000000 graphce-0.0.1/email_data/utils/email_database_manipulation.py
--rw-rw-rw-   0        0        0     5051 2023-06-07 04:19:46.000000 graphce-0.0.1/email_data/utils/email_tree.py
--rw-rw-rw-   0        0        0      322 2023-06-05 08:12:05.000000 graphce-0.0.1/email_data/utils/validator.py
-drwxrwxrwx   0        0        0        0 2023-06-08 07:55:31.344592 graphce-0.0.1/graphce/
--rw-rw-rw-   0        0        0        0 2023-06-08 06:04:45.000000 graphce-0.0.1/graphce/__init__.py
--rw-rw-rw-   0        0        0     1882 2023-06-08 07:55:05.000000 graphce-0.0.1/graphce/tree.py
-drwxrwxrwx   0        0        0        0 2023-06-08 07:55:31.368722 graphce-0.0.1/graphce.egg-info/
--rw-rw-rw-   0        0        0      155 2023-06-08 07:55:31.000000 graphce-0.0.1/graphce.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      882 2023-06-08 07:55:31.000000 graphce-0.0.1/graphce.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-08 07:55:31.000000 graphce-0.0.1/graphce.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-06-08 07:55:31.000000 graphce-0.0.1/graphce.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-08 07:55:31.406101 graphce-0.0.1/ip_profile/
--rw-rw-rw-   0        0        0      119 2023-05-02 08:02:02.000000 graphce-0.0.1/ip_profile/__init__.py
--rw-rw-rw-   0        0        0      458 2023-06-05 06:18:34.000000 graphce-0.0.1/ip_profile/exceptions.py
--rw-rw-rw-   0        0        0     2059 2023-06-06 11:11:16.000000 graphce-0.0.1/ip_profile/ip.py
--rw-rw-rw-   0        0        0      356 2023-06-03 16:02:46.000000 graphce-0.0.1/ip_profile/ip_object.py
--rw-rw-rw-   0        0        0     2088 2023-06-06 11:04:38.000000 graphce-0.0.1/ip_profile/ipv4.py
--rw-rw-rw-   0        0        0     2005 2023-05-10 13:22:35.000000 graphce-0.0.1/ip_profile/ipv6.py
-drwxrwxrwx   0        0        0        0 2023-06-08 07:55:31.436846 graphce-0.0.1/ip_profile/utils/
--rw-rw-rw-   0        0        0        0 2023-05-02 08:02:02.000000 graphce-0.0.1/ip_profile/utils/__init__.py
--rw-rw-rw-   0        0        0      246 2023-05-08 08:07:57.000000 graphce-0.0.1/ip_profile/utils/common.py
--rw-rw-rw-   0        0        0     1565 2023-06-08 05:59:27.000000 graphce-0.0.1/ip_profile/utils/ip_data_manipulation.py
--rw-rw-rw-   0        0        0     4675 2023-06-07 03:40:46.000000 graphce-0.0.1/ip_profile/utils/ip_tree.py
--rw-rw-rw-   0        0        0     1913 2023-05-02 08:02:02.000000 graphce-0.0.1/ip_profile/utils/validator.py
-drwxrwxrwx   0        0        0        0 2023-06-08 07:55:31.460238 graphce-0.0.1/phone_data/
--rw-rw-rw-   0        0        0        0 2023-06-02 11:49:11.000000 graphce-0.0.1/phone_data/__init__.py
--rw-rw-rw-   0        0        0      130 2023-06-05 07:06:33.000000 graphce-0.0.1/phone_data/exceptions.py
--rw-rw-rw-   0        0        0      690 2023-06-07 03:40:46.000000 graphce-0.0.1/phone_data/phone.py
-drwxrwxrwx   0        0        0        0 2023-06-08 07:55:31.475692 graphce-0.0.1/phone_data/utils/
--rw-rw-rw-   0        0        0        0 2023-06-08 06:06:49.000000 graphce-0.0.1/phone_data/utils/__init__.py
--rw-rw-rw-   0        0        0     1571 2023-06-08 06:00:45.000000 graphce-0.0.1/phone_data/utils/phone_database_manipulation.py
--rw-rw-rw-   0        0        0     5077 2023-06-07 03:40:46.000000 graphce-0.0.1/phone_data/utils/phone_tree.py
--rw-rw-rw-   0        0        0      489 2023-06-05 07:10:20.000000 graphce-0.0.1/phone_data/utils/validator.py
--rw-rw-rw-   0        0        0       42 2023-06-08 07:55:31.483794 graphce-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      244 2023-06-08 07:51:42.000000 graphce-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 12:30:18.187270 graphce-0.0.2/
+-rw-rw-rw-   0        0        0     3165 2023-06-09 12:30:18.184322 graphce-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2972 2023-06-09 11:04:45.000000 graphce-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-09 12:30:18.055454 graphce-0.0.2/database/
+-rw-rw-rw-   0        0        0        0 2023-06-05 13:17:20.000000 graphce-0.0.2/database/__init__.py
+-rw-rw-rw-   0        0        0      598 2023-06-09 09:10:06.000000 graphce-0.0.2/database/db_creation.py
+drwxrwxrwx   0        0        0        0 2023-06-09 12:30:18.061496 graphce-0.0.2/edges/
+-rw-rw-rw-   0        0        0        0 2023-06-09 08:30:46.000000 graphce-0.0.2/edges/__init__.py
+-rw-rw-rw-   0        0        0      992 2023-06-09 09:45:27.000000 graphce-0.0.2/edges/edge_manipulation.py
+drwxrwxrwx   0        0        0        0 2023-06-09 12:30:18.067758 graphce-0.0.2/email_data/
+-rw-rw-rw-   0        0        0        0 2023-06-05 03:13:07.000000 graphce-0.0.2/email_data/__init__.py
+-rw-rw-rw-   0        0        0      691 2023-06-07 04:10:43.000000 graphce-0.0.2/email_data/email.py
+drwxrwxrwx   0        0        0        0 2023-06-09 12:30:18.082342 graphce-0.0.2/email_data/utils/
+-rw-rw-rw-   0        0        0        0 2023-06-08 06:06:35.000000 graphce-0.0.2/email_data/utils/__init__.py
+-rw-rw-rw-   0        0        0     1577 2023-06-08 06:00:45.000000 graphce-0.0.2/email_data/utils/email_database_manipulation.py
+-rw-rw-rw-   0        0        0     5051 2023-06-07 04:19:46.000000 graphce-0.0.2/email_data/utils/email_tree.py
+-rw-rw-rw-   0        0        0      322 2023-06-05 08:12:05.000000 graphce-0.0.2/email_data/utils/validator.py
+drwxrwxrwx   0        0        0        0 2023-06-09 12:30:18.087670 graphce-0.0.2/graphce/
+-rw-rw-rw-   0        0        0        0 2023-06-08 06:04:45.000000 graphce-0.0.2/graphce/__init__.py
+-rw-rw-rw-   0        0        0     3092 2023-06-09 09:44:38.000000 graphce-0.0.2/graphce/tree.py
+drwxrwxrwx   0        0        0        0 2023-06-09 12:30:18.107105 graphce-0.0.2/graphce.egg-info/
+-rw-rw-rw-   0        0        0     3165 2023-06-09 12:30:17.000000 graphce-0.0.2/graphce.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      967 2023-06-09 12:30:17.000000 graphce-0.0.2/graphce.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 12:30:17.000000 graphce-0.0.2/graphce.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-06-09 12:30:17.000000 graphce-0.0.2/graphce.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       56 2023-06-09 12:30:17.000000 graphce-0.0.2/graphce.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-09 12:30:18.129947 graphce-0.0.2/ip_profile/
+-rw-rw-rw-   0        0        0      119 2023-05-02 08:02:02.000000 graphce-0.0.2/ip_profile/__init__.py
+-rw-rw-rw-   0        0        0      458 2023-06-05 06:18:34.000000 graphce-0.0.2/ip_profile/exceptions.py
+-rw-rw-rw-   0        0        0     2059 2023-06-06 11:11:16.000000 graphce-0.0.2/ip_profile/ip.py
+-rw-rw-rw-   0        0        0      356 2023-06-03 16:02:46.000000 graphce-0.0.2/ip_profile/ip_object.py
+-rw-rw-rw-   0        0        0     2088 2023-06-06 11:04:38.000000 graphce-0.0.2/ip_profile/ipv4.py
+-rw-rw-rw-   0        0        0     2005 2023-05-10 13:22:35.000000 graphce-0.0.2/ip_profile/ipv6.py
+drwxrwxrwx   0        0        0        0 2023-06-09 12:30:18.149863 graphce-0.0.2/ip_profile/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-02 08:02:02.000000 graphce-0.0.2/ip_profile/utils/__init__.py
+-rw-rw-rw-   0        0        0      246 2023-05-08 08:07:57.000000 graphce-0.0.2/ip_profile/utils/common.py
+-rw-rw-rw-   0        0        0     1565 2023-06-08 05:59:27.000000 graphce-0.0.2/ip_profile/utils/ip_data_manipulation.py
+-rw-rw-rw-   0        0        0     4675 2023-06-07 03:40:46.000000 graphce-0.0.2/ip_profile/utils/ip_tree.py
+-rw-rw-rw-   0        0        0     1913 2023-05-02 08:02:02.000000 graphce-0.0.2/ip_profile/utils/validator.py
+drwxrwxrwx   0        0        0        0 2023-06-09 12:30:18.165747 graphce-0.0.2/phone_data/
+-rw-rw-rw-   0        0        0        0 2023-06-02 11:49:11.000000 graphce-0.0.2/phone_data/__init__.py
+-rw-rw-rw-   0        0        0      130 2023-06-05 07:06:33.000000 graphce-0.0.2/phone_data/exceptions.py
+-rw-rw-rw-   0        0        0      690 2023-06-07 03:40:46.000000 graphce-0.0.2/phone_data/phone.py
+drwxrwxrwx   0        0        0        0 2023-06-09 12:30:18.179640 graphce-0.0.2/phone_data/utils/
+-rw-rw-rw-   0        0        0        0 2023-06-08 06:06:49.000000 graphce-0.0.2/phone_data/utils/__init__.py
+-rw-rw-rw-   0        0        0     1571 2023-06-08 06:00:45.000000 graphce-0.0.2/phone_data/utils/phone_database_manipulation.py
+-rw-rw-rw-   0        0        0     5077 2023-06-07 03:40:46.000000 graphce-0.0.2/phone_data/utils/phone_tree.py
+-rw-rw-rw-   0        0        0      489 2023-06-05 07:10:20.000000 graphce-0.0.2/phone_data/utils/validator.py
+-rw-rw-rw-   0        0        0       42 2023-06-09 12:30:18.187270 graphce-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      459 2023-06-09 12:30:13.000000 graphce-0.0.2/setup.py
```

### Comparing `graphce-0.0.1/email_data/email.py` & `graphce-0.0.2/email_data/email.py`

 * *Files identical despite different names*

### Comparing `graphce-0.0.1/email_data/utils/email_database_manipulation.py` & `graphce-0.0.2/email_data/utils/email_database_manipulation.py`

 * *Files identical despite different names*

### Comparing `graphce-0.0.1/email_data/utils/email_tree.py` & `graphce-0.0.2/email_data/utils/email_tree.py`

 * *Files identical despite different names*

### Comparing `graphce-0.0.1/graphce/tree.py` & `graphce-0.0.2/graphce/tree.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,35 @@
 """
-
+todo:
+1. create a base class node for IPs
+2. to showcase and display graphs we are creating(graphviz)
+3. encryption and decryption
 """
+# python level imports
+from typing import Any
+
 # project level libraries
 from database.db_creation import DB_Creation
 from ip_profile.ip import IP
 from phone_data.phone import Phone
 from email_data.email import Email
+from edges.edge_manipulation import Edge
 
 
 class GraphCE:
     def __init__(self, type_: str, location: str):
         """
         :param type_: type should be IP or PHONE or EMAIL (Uppercase)
         :param location: path of database as a string
         """
         self.__type = type_
-        self.__location = f"{location}\\{type_}.sqlite"
-        self.database = DB_Creation(self.__location)
+        self.__location = f"{location}\\{type_}s.sqlite"
+        self.__edge_location = f"{location}\\edges.sqlite"
+        self.__edge = Edge(self.__edge_location)
+        self.database = DB_Creation(self.__location, self.__edge_location)
 
         if self.__type == 'IP':
             self.__node_obj = IP(self.__location)
         elif self.__type == 'PHONE':
             self.__node_obj = Phone(self.__location)
         elif self.__type == 'EMAIL':
             self.__node_obj = Email(self.__location)
@@ -32,15 +41,15 @@
         :param value: Phone number or IP address or Email
         :param info: information regarding value as a dict
         :return: True, if element is updated
                  False, if element is not updated
         """
         return self.__node_obj._add(value, info)
 
-    def search(self, value: str) -> bool:
+    def search(self, value: str) -> tuple[bool, int] | tuple[bool, Any]:
         """
 
         :param value: Phone number or IP address or Email
         :return: True and info, if element is present
                  False and -1, if element is not present
         """
         return self.__node_obj._is_present(value)
@@ -50,7 +59,41 @@
 
         :param value: Phone number or IP address or Email
         :param info: information regarding value as a dict
         :return: True, if element is updated
                  False, if element is not updated
         """
         return self.__node_obj._update_info(value, info)
+
+    def create_edge(self, key: tuple, value: str) -> None:
+        """
+
+        :param key: Tuple of two nodes
+        :param value: Information
+        :return:
+        """
+        return self.__edge._create_edge(key, value)
+
+    def access_edge(self, key: tuple) -> str:
+        """
+
+        :param key: Tuple of two nodes
+        :return: value
+        """
+        return self.__edge._access_edge(key)
+
+    def update_edge(self, key: tuple, value: str):
+        """
+
+        :param key: Tuple of two nodes
+        :param value: Information
+        :return:
+        """
+        return self.__edge._update_edge(key, value)
+
+    def delete_edge(self, key: str):
+        """
+
+        :param key: Tuple of two nodes
+        :return:
+        """
+        return self.__edge._delete_edge(key)
```

### Comparing `graphce-0.0.1/graphce.egg-info/SOURCES.txt` & `graphce-0.0.2/graphce.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,25 @@
+README.md
 setup.py
 database/__init__.py
 database/db_creation.py
+edges/__init__.py
+edges/edge_manipulation.py
 email_data/__init__.py
 email_data/email.py
 email_data/utils/__init__.py
 email_data/utils/email_database_manipulation.py
 email_data/utils/email_tree.py
 email_data/utils/validator.py
 graphce/__init__.py
 graphce/tree.py
 graphce.egg-info/PKG-INFO
 graphce.egg-info/SOURCES.txt
 graphce.egg-info/dependency_links.txt
+graphce.egg-info/requires.txt
 graphce.egg-info/top_level.txt
 ip_profile/__init__.py
 ip_profile/exceptions.py
 ip_profile/ip.py
 ip_profile/ip_object.py
 ip_profile/ipv4.py
 ip_profile/ipv6.py
```

### Comparing `graphce-0.0.1/ip_profile/ip.py` & `graphce-0.0.2/ip_profile/ip.py`

 * *Files identical despite different names*

### Comparing `graphce-0.0.1/ip_profile/ipv4.py` & `graphce-0.0.2/ip_profile/ipv4.py`

 * *Files identical despite different names*

### Comparing `graphce-0.0.1/ip_profile/ipv6.py` & `graphce-0.0.2/ip_profile/ipv6.py`

 * *Files identical despite different names*

### Comparing `graphce-0.0.1/ip_profile/utils/ip_data_manipulation.py` & `graphce-0.0.2/ip_profile/utils/ip_data_manipulation.py`

 * *Files identical despite different names*

### Comparing `graphce-0.0.1/ip_profile/utils/ip_tree.py` & `graphce-0.0.2/ip_profile/utils/ip_tree.py`

 * *Files identical despite different names*

### Comparing `graphce-0.0.1/ip_profile/utils/validator.py` & `graphce-0.0.2/ip_profile/utils/validator.py`

 * *Files identical despite different names*

### Comparing `graphce-0.0.1/phone_data/phone.py` & `graphce-0.0.2/phone_data/phone.py`

 * *Files identical despite different names*

### Comparing `graphce-0.0.1/phone_data/utils/phone_database_manipulation.py` & `graphce-0.0.2/phone_data/utils/phone_database_manipulation.py`

 * *Files identical despite different names*

### Comparing `graphce-0.0.1/phone_data/utils/phone_tree.py` & `graphce-0.0.2/phone_data/utils/phone_tree.py`

 * *Files identical despite different names*

