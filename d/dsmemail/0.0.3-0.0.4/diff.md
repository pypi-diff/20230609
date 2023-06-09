# Comparing `tmp/dsmemail-0.0.3.tar.gz` & `tmp/dsmemail-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dsmemail-0.0.3.tar", last modified: Thu Sep  1 09:43:47 2022, max compression
+gzip compressed data, was "dsmemail-0.0.4.tar", last modified: Fri Jun  9 03:46:28 2023, max compression
```

## Comparing `dsmemail-0.0.3.tar` & `dsmemail-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 naii       (501) staff       (20)        0 2022-09-01 09:43:47.000000 dsmemail-0.0.3/
--rw-r--r--   0 naii       (501) staff       (20)     1475 2022-09-01 09:43:47.000000 dsmemail-0.0.3/PKG-INFO
-drwxr-xr-x   0 naii       (501) staff       (20)        0 2022-09-01 09:43:47.000000 dsmemail-0.0.3/dsmemail/
--rw-r--r--   0 naii       (501) staff       (20)      754 2022-08-22 09:59:51.000000 dsmemail-0.0.3/dsmemail/check.py
--rw-r--r--   0 naii       (501) staff       (20)      174 2022-09-01 09:43:14.000000 dsmemail-0.0.3/dsmemail/__init__.py
--rw-r--r--   0 naii       (501) staff       (20)     1018 2022-09-01 09:42:41.000000 dsmemail-0.0.3/dsmemail/sendmail.py
--rw-r--r--   0 naii       (501) staff       (20)      481 2022-08-22 09:59:51.000000 dsmemail-0.0.3/README.md
-drwxr-xr-x   0 naii       (501) staff       (20)        0 2022-09-01 09:43:47.000000 dsmemail-0.0.3/dsmemail.egg-info/
--rw-r--r--   0 naii       (501) staff       (20)     1475 2022-09-01 09:43:47.000000 dsmemail-0.0.3/dsmemail.egg-info/PKG-INFO
--rw-r--r--   0 naii       (501) staff       (20)      237 2022-09-01 09:43:47.000000 dsmemail-0.0.3/dsmemail.egg-info/SOURCES.txt
--rw-r--r--   0 naii       (501) staff       (20)        9 2022-09-01 09:43:47.000000 dsmemail-0.0.3/dsmemail.egg-info/requires.txt
--rw-r--r--   0 naii       (501) staff       (20)        9 2022-09-01 09:43:47.000000 dsmemail-0.0.3/dsmemail.egg-info/top_level.txt
--rw-r--r--   0 naii       (501) staff       (20)        1 2022-09-01 09:43:47.000000 dsmemail-0.0.3/dsmemail.egg-info/dependency_links.txt
--rw-r--r--   0 naii       (501) staff       (20)     1285 2022-09-01 09:43:21.000000 dsmemail-0.0.3/setup.py
--rw-r--r--   0 naii       (501) staff       (20)       38 2022-09-01 09:43:47.000000 dsmemail-0.0.3/setup.cfg
+drwxr-xr-x   0 naii       (501) staff       (20)        0 2023-06-09 03:46:28.011851 dsmemail-0.0.4/
+-rw-r--r--   0 naii       (501) staff       (20)     1579 2023-06-09 03:46:28.011527 dsmemail-0.0.4/PKG-INFO
+-rw-r--r--   0 naii       (501) staff       (20)      940 2023-06-09 03:44:57.000000 dsmemail-0.0.4/README.md
+drwxr-xr-x   0 naii       (501) staff       (20)        0 2023-06-09 03:46:28.007651 dsmemail-0.0.4/dsmemail/
+-rw-r--r--   0 naii       (501) staff       (20)      174 2023-06-09 03:45:51.000000 dsmemail-0.0.4/dsmemail/__init__.py
+-rw-r--r--   0 naii       (501) staff       (20)      754 2022-08-22 09:59:51.000000 dsmemail-0.0.4/dsmemail/check.py
+-rw-r--r--   0 naii       (501) staff       (20)     1219 2023-06-09 03:44:56.000000 dsmemail-0.0.4/dsmemail/sendmail.py
+drwxr-xr-x   0 naii       (501) staff       (20)        0 2023-06-09 03:46:28.010855 dsmemail-0.0.4/dsmemail.egg-info/
+-rw-r--r--   0 naii       (501) staff       (20)     1579 2023-06-09 03:46:27.000000 dsmemail-0.0.4/dsmemail.egg-info/PKG-INFO
+-rw-r--r--   0 naii       (501) staff       (20)      237 2023-06-09 03:46:28.000000 dsmemail-0.0.4/dsmemail.egg-info/SOURCES.txt
+-rw-r--r--   0 naii       (501) staff       (20)        1 2023-06-09 03:46:27.000000 dsmemail-0.0.4/dsmemail.egg-info/dependency_links.txt
+-rw-r--r--   0 naii       (501) staff       (20)        9 2023-06-09 03:46:27.000000 dsmemail-0.0.4/dsmemail.egg-info/requires.txt
+-rw-r--r--   0 naii       (501) staff       (20)        9 2023-06-09 03:46:27.000000 dsmemail-0.0.4/dsmemail.egg-info/top_level.txt
+-rw-r--r--   0 naii       (501) staff       (20)       38 2023-06-09 03:46:28.011971 dsmemail-0.0.4/setup.cfg
+-rw-r--r--   0 naii       (501) staff       (20)     1285 2023-06-09 03:45:29.000000 dsmemail-0.0.4/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `dsmemail-0.0.3/PKG-INFO` & `dsmemail-0.0.4/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,61 +1,70 @@
 Metadata-Version: 2.1
 Name: dsmemail
-Version: 0.0.3
+Version: 0.0.4
 Summary: A simple way to send email. for dsm
 Home-page: https://gitlab.com/public-project2/dsm-email
 Author: DigitalStoreMesh Co.,Ltd
 Author-email: contact@storemesh.com
 License: MIT License
-Description: # DSM Email
-        
-        ## install
-        ```
-        pip install dsmemail
-        ```
-        
-        ## how to use
-        1. set env
-        
-        ```
-        DSM_EMAIL_URI=<DSM_EMAIL_URI>
-        DSM_EMAIL_APIKEY=<DSM_EMAIL_APIKEY>
-        ```
-        
-        2. send email
-        
-        ```python
-        import dsmemail
-        
-        status, msg = dsmemail.sendEmail(
-            subject="test", 
-            message="helloworld", 
-            emails=["admin@admin.com"]
-        )
-        
-        print(status, msg)
-        ```
-        output
-        ```
-        (True, 'email send sucess')
-        ```
-        
-        #
-        status
-        ```
-        True = send email sucess
-        False = send email fail
-        ```
-        
-        msg
-        ```
-        string describe status
-        ```
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
+
+# DSM Email
+
+## install
+```
+pip install dsmemail
+```
+
+## how to use
+1. set env
+
+```
+DSM_EMAIL_URI=<DSM_EMAIL_URI>
+DSM_EMAIL_APIKEY=<DSM_EMAIL_APIKEY>
+```
+
+2. send email
+
+```python
+import dsmemail
+
+status, msg = dsmemail.sendEmail(
+    subject="test", 
+    message="helloworld", 
+    emails=["admin@admin.com"],
+    attachments=["test.txt"]
+)
+print(status, msg)
+```
+| variable      | dtype      | description                           |
+| --------      | ---------  | ------------------------------------- |
+| subject       | str        | subject of email                      |
+| message       | str        | email body can contains html string   |
+| emails        | List[str]  | email to send message                 |
+| attachments   | List[str]  | list of filepath(str) to attach files   | 
+
+output
+```
+(True, 'email send sucess')
+```
+
+#
+status
+```
+True = send email sucess
+False = send email fail
+```
+
+msg
+```
+string describe status
+```
+
```

### Comparing `dsmemail-0.0.3/dsmemail/check.py` & `dsmemail-0.0.4/dsmemail/check.py`

 * *Files identical despite different names*

### Comparing `dsmemail-0.0.3/dsmemail/sendmail.py` & `dsmemail-0.0.4/dsmemail/sendmail.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 import os
 import requests
 from .check import check_type, check_env
 
 DSM_EMAIL_APIKEY = os.environ.get('DSM_EMAIL_APIKEY', None)
 DSM_EMAIL_URI = os.environ.get('DSM_EMAIL_URI', None)
 
-def sendEmail(subject=None, message=None, emails=None):
+def sendEmail(subject=None, message=None, emails=None, attachments=[]):
     
     check_env()
     
     check_type(variable=subject, variableName="subject", dtype=str)
     check_type(variable=message, variableName="message", dtype=str)
     check_type(variable=emails, variableName="emails", dtype=list, child=str)
+    check_type(variable=attachments, variableName="attachments", dtype=list, child=str)
     
-    r = requests.post(f"{DSM_EMAIL_URI}/email/api/sendMail/",
+    file = [("attachments", open(elm, 'rb')) for elm in attachments]
+    r = requests.post(f"{DSM_EMAIL_URI}/email/api/emailMessage/",
             headers={
                 "Authorization": f"Api-Key {DSM_EMAIL_APIKEY}"
             },
-            json={
+            data={
                 "subject": subject,
                 "message": message,
                 "email": emails
-            }
+            },
+            files=file
     )
     
     if r.status_code == 201:
         return True, "email send sucess"
     elif r.status_code in [400, 401, 403]:
         return False, r.json()
     else:
```

### Comparing `dsmemail-0.0.3/dsmemail.egg-info/PKG-INFO` & `dsmemail-0.0.4/dsmemail.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,61 +1,70 @@
 Metadata-Version: 2.1
 Name: dsmemail
-Version: 0.0.3
+Version: 0.0.4
 Summary: A simple way to send email. for dsm
 Home-page: https://gitlab.com/public-project2/dsm-email
 Author: DigitalStoreMesh Co.,Ltd
 Author-email: contact@storemesh.com
 License: MIT License
-Description: # DSM Email
-        
-        ## install
-        ```
-        pip install dsmemail
-        ```
-        
-        ## how to use
-        1. set env
-        
-        ```
-        DSM_EMAIL_URI=<DSM_EMAIL_URI>
-        DSM_EMAIL_APIKEY=<DSM_EMAIL_APIKEY>
-        ```
-        
-        2. send email
-        
-        ```python
-        import dsmemail
-        
-        status, msg = dsmemail.sendEmail(
-            subject="test", 
-            message="helloworld", 
-            emails=["admin@admin.com"]
-        )
-        
-        print(status, msg)
-        ```
-        output
-        ```
-        (True, 'email send sucess')
-        ```
-        
-        #
-        status
-        ```
-        True = send email sucess
-        False = send email fail
-        ```
-        
-        msg
-        ```
-        string describe status
-        ```
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
+
+# DSM Email
+
+## install
+```
+pip install dsmemail
+```
+
+## how to use
+1. set env
+
+```
+DSM_EMAIL_URI=<DSM_EMAIL_URI>
+DSM_EMAIL_APIKEY=<DSM_EMAIL_APIKEY>
+```
+
+2. send email
+
+```python
+import dsmemail
+
+status, msg = dsmemail.sendEmail(
+    subject="test", 
+    message="helloworld", 
+    emails=["admin@admin.com"],
+    attachments=["test.txt"]
+)
+print(status, msg)
+```
+| variable      | dtype      | description                           |
+| --------      | ---------  | ------------------------------------- |
+| subject       | str        | subject of email                      |
+| message       | str        | email body can contains html string   |
+| emails        | List[str]  | email to send message                 |
+| attachments   | List[str]  | list of filepath(str) to attach files   | 
+
+output
+```
+(True, 'email send sucess')
+```
+
+#
+status
+```
+True = send email sucess
+False = send email fail
+```
+
+msg
+```
+string describe status
+```
+
```

### Comparing `dsmemail-0.0.3/setup.py` & `dsmemail-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='dsmemail',
-    version='0.0.3',
+    version='0.0.4',
     url='https://gitlab.com/public-project2/dsm-email',
     packages=find_packages(),
     include_package_data=True,
     license='MIT License',
     description='A simple way to send email. for dsm',
     long_description=README,
     long_description_content_type='text/markdown',
```

