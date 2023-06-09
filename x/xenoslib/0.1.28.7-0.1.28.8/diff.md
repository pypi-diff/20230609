# Comparing `tmp/xenoslib-0.1.28.7.tar.gz` & `tmp/xenoslib-0.1.28.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xenoslib-0.1.28.7.tar", last modified: Fri Jun  9 02:54:38 2023, max compression
+gzip compressed data, was "xenoslib-0.1.28.8.tar", last modified: Fri Jun  9 05:40:36 2023, max compression
```

## Comparing `xenoslib-0.1.28.7.tar` & `xenoslib-0.1.28.8.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 02:54:38.534381 xenoslib-0.1.28.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-09 02:54:27.000000 xenoslib-0.1.28.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-09 02:54:38.530381 xenoslib-0.1.28.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-06-09 02:54:27.000000 xenoslib-0.1.28.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 02:54:38.534381 xenoslib-0.1.28.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-09 02:54:27.000000 xenoslib-0.1.28.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 02:54:38.530381 xenoslib-0.1.28.7/xenoslib/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-09 02:54:27.000000 xenoslib-0.1.28.7/xenoslib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-09 02:54:27.000000 xenoslib-0.1.28.7/xenoslib/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-09 02:54:27.000000 xenoslib-0.1.28.7/xenoslib/about.py
--rw-r--r--   0 runner    (1001) docker     (123)    11629 2023-06-09 02:54:27.000000 xenoslib-0.1.28.7/xenoslib/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-06-09 02:54:27.000000 xenoslib-0.1.28.7/xenoslib/dev.py
--rw-r--r--   0 runner    (1001) docker     (123)     4942 2023-06-09 02:54:27.000000 xenoslib-0.1.28.7/xenoslib/extend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-06-09 02:54:27.000000 xenoslib-0.1.28.7/xenoslib/linux.py
--rw-r--r--   0 runner    (1001) docker     (123)     5909 2023-06-09 02:54:27.000000 xenoslib-0.1.28.7/xenoslib/mail.py
--rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-06-09 02:54:27.000000 xenoslib-0.1.28.7/xenoslib/mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     7783 2023-06-09 02:54:27.000000 xenoslib-0.1.28.7/xenoslib/onedrive.py
--rw-r--r--   0 runner    (1001) docker     (123)    12161 2023-06-09 02:54:27.000000 xenoslib-0.1.28.7/xenoslib/win_trayicon.py
--rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-06-09 02:54:27.000000 xenoslib-0.1.28.7/xenoslib/windows.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 02:54:38.530381 xenoslib-0.1.28.7/xenoslib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-09 02:54:38.000000 xenoslib-0.1.28.7/xenoslib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-06-09 02:54:38.000000 xenoslib-0.1.28.7/xenoslib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 02:54:38.000000 xenoslib-0.1.28.7/xenoslib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-09 02:54:38.000000 xenoslib-0.1.28.7/xenoslib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-09 02:54:38.000000 xenoslib-0.1.28.7/xenoslib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 05:40:36.542197 xenoslib-0.1.28.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-09 05:40:22.000000 xenoslib-0.1.28.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-09 05:40:36.542197 xenoslib-0.1.28.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-06-09 05:40:22.000000 xenoslib-0.1.28.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 05:40:36.542197 xenoslib-0.1.28.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-09 05:40:22.000000 xenoslib-0.1.28.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 05:40:36.542197 xenoslib-0.1.28.8/xenoslib/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-09 05:40:22.000000 xenoslib-0.1.28.8/xenoslib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-09 05:40:22.000000 xenoslib-0.1.28.8/xenoslib/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-09 05:40:22.000000 xenoslib-0.1.28.8/xenoslib/about.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11629 2023-06-09 05:40:22.000000 xenoslib-0.1.28.8/xenoslib/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-06-09 05:40:22.000000 xenoslib-0.1.28.8/xenoslib/dev.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4942 2023-06-09 05:40:22.000000 xenoslib-0.1.28.8/xenoslib/extend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-06-09 05:40:22.000000 xenoslib-0.1.28.8/xenoslib/linux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-06-09 05:40:22.000000 xenoslib-0.1.28.8/xenoslib/mail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-06-09 05:40:22.000000 xenoslib-0.1.28.8/xenoslib/mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7783 2023-06-09 05:40:22.000000 xenoslib-0.1.28.8/xenoslib/onedrive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12161 2023-06-09 05:40:22.000000 xenoslib-0.1.28.8/xenoslib/win_trayicon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-06-09 05:40:22.000000 xenoslib-0.1.28.8/xenoslib/windows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 05:40:36.542197 xenoslib-0.1.28.8/xenoslib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-09 05:40:36.000000 xenoslib-0.1.28.8/xenoslib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-06-09 05:40:36.000000 xenoslib-0.1.28.8/xenoslib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 05:40:36.000000 xenoslib-0.1.28.8/xenoslib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-09 05:40:36.000000 xenoslib-0.1.28.8/xenoslib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-09 05:40:36.000000 xenoslib-0.1.28.8/xenoslib.egg-info/top_level.txt
```

### Comparing `xenoslib-0.1.28.7/LICENSE` & `xenoslib-0.1.28.8/LICENSE`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.28.7/README.md` & `xenoslib-0.1.28.8/README.md`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.28.7/setup.py` & `xenoslib-0.1.28.8/setup.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.28.7/xenoslib/base.py` & `xenoslib-0.1.28.8/xenoslib/base.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.28.7/xenoslib/dev.py` & `xenoslib-0.1.28.8/xenoslib/dev.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.28.7/xenoslib/extend.py` & `xenoslib-0.1.28.8/xenoslib/extend.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.28.7/xenoslib/linux.py` & `xenoslib-0.1.28.8/xenoslib/linux.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.28.7/xenoslib/mail.py` & `xenoslib-0.1.28.8/xenoslib/mail.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,16 +105,15 @@
         self.sender = sender
         self.password = password
         if self.port == 465:  # use SSL by port
             self.SMTP = smtplib.SMTP_SSL
         else:
             self.SMTP = smtplib.SMTP
 
-    def send(self, subject, message, receiver, cc=[], bcc=[], filename=None):
-        receivers = []
+    def send(self, subject, message, receiver, receivers=[], cc=[], bcc=[], filename=None):
         if isinstance(receiver, str):
             receivers.append(receiver)
         elif isinstance(receiver, (list, tuple)):
             receivers.extend(receiver)
         msg = MIMEMultipart()
         msg["Subject"] = Header(subject, "utf-8")
         msg["From"] = Header(self.sender, "utf-8")
```

### Comparing `xenoslib-0.1.28.7/xenoslib/mock.py` & `xenoslib-0.1.28.8/xenoslib/mock.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.28.7/xenoslib/onedrive.py` & `xenoslib-0.1.28.8/xenoslib/onedrive.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.28.7/xenoslib/win_trayicon.py` & `xenoslib-0.1.28.8/xenoslib/win_trayicon.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.28.7/xenoslib/windows.py` & `xenoslib-0.1.28.8/xenoslib/windows.py`

 * *Files identical despite different names*

