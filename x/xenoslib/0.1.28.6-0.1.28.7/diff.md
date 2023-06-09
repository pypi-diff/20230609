# Comparing `tmp/xenoslib-0.1.28.6.tar.gz` & `tmp/xenoslib-0.1.28.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xenoslib-0.1.28.6.tar", last modified: Wed May 31 01:50:04 2023, max compression
+gzip compressed data, was "xenoslib-0.1.28.7.tar", last modified: Fri Jun  9 02:54:38 2023, max compression
```

## Comparing `xenoslib-0.1.28.6.tar` & `xenoslib-0.1.28.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 01:50:04.489658 xenoslib-0.1.28.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-31 01:49:53.000000 xenoslib-0.1.28.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-31 01:50:04.489658 xenoslib-0.1.28.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-05-31 01:49:53.000000 xenoslib-0.1.28.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 01:50:04.489658 xenoslib-0.1.28.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-31 01:49:53.000000 xenoslib-0.1.28.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 01:50:04.489658 xenoslib-0.1.28.6/xenoslib/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-31 01:49:53.000000 xenoslib-0.1.28.6/xenoslib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-31 01:49:53.000000 xenoslib-0.1.28.6/xenoslib/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-31 01:49:53.000000 xenoslib-0.1.28.6/xenoslib/about.py
--rw-r--r--   0 runner    (1001) docker     (123)    11564 2023-05-31 01:49:53.000000 xenoslib-0.1.28.6/xenoslib/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-05-31 01:49:53.000000 xenoslib-0.1.28.6/xenoslib/dev.py
--rw-r--r--   0 runner    (1001) docker     (123)     4942 2023-05-31 01:49:53.000000 xenoslib-0.1.28.6/xenoslib/extend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-05-31 01:49:53.000000 xenoslib-0.1.28.6/xenoslib/linux.py
--rw-r--r--   0 runner    (1001) docker     (123)     5721 2023-05-31 01:49:53.000000 xenoslib-0.1.28.6/xenoslib/mail.py
--rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-05-31 01:49:53.000000 xenoslib-0.1.28.6/xenoslib/mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     7783 2023-05-31 01:49:53.000000 xenoslib-0.1.28.6/xenoslib/onedrive.py
--rw-r--r--   0 runner    (1001) docker     (123)    12161 2023-05-31 01:49:53.000000 xenoslib-0.1.28.6/xenoslib/win_trayicon.py
--rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-05-31 01:49:53.000000 xenoslib-0.1.28.6/xenoslib/windows.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 01:50:04.489658 xenoslib-0.1.28.6/xenoslib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-31 01:50:04.000000 xenoslib-0.1.28.6/xenoslib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-31 01:50:04.000000 xenoslib-0.1.28.6/xenoslib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 01:50:04.000000 xenoslib-0.1.28.6/xenoslib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-31 01:50:04.000000 xenoslib-0.1.28.6/xenoslib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-31 01:50:04.000000 xenoslib-0.1.28.6/xenoslib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 02:54:38.534381 xenoslib-0.1.28.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-09 02:54:27.000000 xenoslib-0.1.28.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-09 02:54:38.530381 xenoslib-0.1.28.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-06-09 02:54:27.000000 xenoslib-0.1.28.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 02:54:38.534381 xenoslib-0.1.28.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-09 02:54:27.000000 xenoslib-0.1.28.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 02:54:38.530381 xenoslib-0.1.28.7/xenoslib/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-09 02:54:27.000000 xenoslib-0.1.28.7/xenoslib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-09 02:54:27.000000 xenoslib-0.1.28.7/xenoslib/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-09 02:54:27.000000 xenoslib-0.1.28.7/xenoslib/about.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11629 2023-06-09 02:54:27.000000 xenoslib-0.1.28.7/xenoslib/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-06-09 02:54:27.000000 xenoslib-0.1.28.7/xenoslib/dev.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4942 2023-06-09 02:54:27.000000 xenoslib-0.1.28.7/xenoslib/extend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-06-09 02:54:27.000000 xenoslib-0.1.28.7/xenoslib/linux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5909 2023-06-09 02:54:27.000000 xenoslib-0.1.28.7/xenoslib/mail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-06-09 02:54:27.000000 xenoslib-0.1.28.7/xenoslib/mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7783 2023-06-09 02:54:27.000000 xenoslib-0.1.28.7/xenoslib/onedrive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12161 2023-06-09 02:54:27.000000 xenoslib-0.1.28.7/xenoslib/win_trayicon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-06-09 02:54:27.000000 xenoslib-0.1.28.7/xenoslib/windows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 02:54:38.530381 xenoslib-0.1.28.7/xenoslib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-09 02:54:38.000000 xenoslib-0.1.28.7/xenoslib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-06-09 02:54:38.000000 xenoslib-0.1.28.7/xenoslib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 02:54:38.000000 xenoslib-0.1.28.7/xenoslib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-09 02:54:38.000000 xenoslib-0.1.28.7/xenoslib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-09 02:54:38.000000 xenoslib-0.1.28.7/xenoslib.egg-info/top_level.txt
```

### Comparing `xenoslib-0.1.28.6/LICENSE` & `xenoslib-0.1.28.7/LICENSE`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.28.6/README.md` & `xenoslib-0.1.28.7/README.md`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.28.6/setup.py` & `xenoslib-0.1.28.7/setup.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.28.6/xenoslib/base.py` & `xenoslib-0.1.28.7/xenoslib/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -231,14 +231,16 @@
         print("Nested data result: ")
         print(self.result)
         print("Nested data path:")
         print(self.path)
 
 
 class Singleton:
+    """Please note that __init__() will still run every time"""
+
     def __new__(cls, *args, **kwargs):
         if not hasattr(cls, "_instance"):
             cls._instance = super().__new__(cls)
         return cls._instance
 
 
 class SingletonWithArgs:
```

### Comparing `xenoslib-0.1.28.6/xenoslib/dev.py` & `xenoslib-0.1.28.7/xenoslib/dev.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.28.6/xenoslib/extend.py` & `xenoslib-0.1.28.7/xenoslib/extend.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.28.6/xenoslib/linux.py` & `xenoslib-0.1.28.7/xenoslib/linux.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.28.6/xenoslib/mail.py` & `xenoslib-0.1.28.7/xenoslib/mail.py`

 * *Files 5% similar despite different names*

```diff
@@ -105,23 +105,28 @@
         self.sender = sender
         self.password = password
         if self.port == 465:  # use SSL by port
             self.SMTP = smtplib.SMTP_SSL
         else:
             self.SMTP = smtplib.SMTP
 
-    def send(self, subject, message, receiver=[], cc=[], bcc=[], filename=None):
+    def send(self, subject, message, receiver, cc=[], bcc=[], filename=None):
+        receivers = []
+        if isinstance(receiver, str):
+            receivers.append(receiver)
+        elif isinstance(receiver, (list, tuple)):
+            receivers.extend(receiver)
         msg = MIMEMultipart()
         msg["Subject"] = Header(subject, "utf-8")
         msg["From"] = Header(self.sender, "utf-8")
-        msg["To"] = ";".join(receiver)
+        msg["To"] = ";".join(receivers)
         msg["Cc"] = ";".join(cc)
         msg["Message-ID"] = make_msgid()
-        receiver.extend(cc)
-        receiver.extend(bcc)
+        receivers.extend(cc)
+        receivers.extend(bcc)
         msg.attach(MIMEText(message, "html", "utf-8"))
 
         if filename:
             attachment = MIMEApplication(open(filename, "rb").read())
             attachment.add_header("Content-Disposition", "attachment", filename=filename)
             msg.attach(attachment)
 
@@ -130,15 +135,15 @@
             if smtp.has_extn("STARTTLS"):
                 smtp.starttls()
             try:
                 smtp.login(self.sender, self.password)
             except Exception as exc:
                 logger.warning(exc)
                 return False
-            smtp.sendmail(self.sender, receiver, msg.as_string())
+            smtp.sendmail(self.sender, receivers, msg.as_string())
             return True
 
 
 def test_imap():
     try:
         import env  # noqa
     except ModuleNotFoundError:
@@ -160,13 +165,13 @@
     mail_addr = os.environ["SMTP_ADDR"]
     mail_pwd = os.environ["SMTP_PASS"]
     smtp_server = os.environ["SMTP_SERVER"]
     subject = "Test Email2"
     message = '<span style="color:red">This is a test email.</span>'
     email_sender = SMTPMail(smtp_server, sender=mail_addr, password=mail_pwd, port=465)
     # email_sender = SMTPMail(smtp_server, sender=mail_addr, password=mail_pwd, port=587)
-    email_sender.send(subject=subject, message=message, receiver=[os.environ["RECEIVER"]])
+    email_sender.send(subject=subject, message=message, receiver=os.environ["RECEIVER"])
 
 
 if __name__ == "__main__":
-    test_imap()
-    # test()
+    # test_imap()
+    test()
```

### Comparing `xenoslib-0.1.28.6/xenoslib/mock.py` & `xenoslib-0.1.28.7/xenoslib/mock.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.28.6/xenoslib/onedrive.py` & `xenoslib-0.1.28.7/xenoslib/onedrive.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.28.6/xenoslib/win_trayicon.py` & `xenoslib-0.1.28.7/xenoslib/win_trayicon.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.28.6/xenoslib/windows.py` & `xenoslib-0.1.28.7/xenoslib/windows.py`

 * *Files identical despite different names*

