# Comparing `tmp/flask_captcha2-2.0.0.tar.gz` & `tmp/Flask-captcha2-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\flask_captcha2-2.0.0.tar", last modified: Thu May 18 05:20:46 2023, max compression
+gzip compressed data, was "Flask-captcha2-2.0.1.tar", last modified: Fri Jun  9 14:31:53 2023, max compression
```

## Comparing `flask_captcha2-2.0.0.tar` & `Flask-captcha2-2.0.1.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 05:20:46.280339 flask_captcha2-2.0.0/
--rw-rw-rw-   0        0        0      571 2023-05-18 05:20:46.279339 flask_captcha2-2.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      102 2023-05-17 15:52:17.000000 flask_captcha2-2.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-18 05:20:46.273339 flask_captcha2-2.0.0/flask_captcha2/
--rw-rw-rw-   0        0        0     3412 2023-05-17 17:21:33.000000 flask_captcha2-2.0.0/flask_captcha2/__init__.py
--rw-rw-rw-   0        0        0      147 2023-05-18 05:20:29.000000 flask_captcha2-2.0.0/flask_captcha2/auther.py
-drwxrwxrwx   0        0        0        0 2023-05-18 05:20:46.278339 flask_captcha2-2.0.0/flask_captcha2.egg-info/
--rw-rw-rw-   0        0        0      571 2023-05-18 05:20:46.000000 flask_captcha2-2.0.0/flask_captcha2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      259 2023-05-18 05:20:46.000000 flask_captcha2-2.0.0/flask_captcha2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 05:20:46.000000 flask_captcha2-2.0.0/flask_captcha2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-05-18 05:20:46.000000 flask_captcha2-2.0.0/flask_captcha2.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-18 05:20:46.000000 flask_captcha2-2.0.0/flask_captcha2.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-18 05:20:46.280339 flask_captcha2-2.0.0/setup.cfg
--rw-rw-rw-   0        0        0      828 2023-05-18 05:16:59.000000 flask_captcha2-2.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 14:31:53.597818 Flask-captcha2-2.0.1/
+drwxrwxrwx   0        0        0        0 2023-06-09 14:31:53.592819 Flask-captcha2-2.0.1/Flask_captcha2.egg-info/
+-rw-rw-rw-   0        0        0     4261 2023-06-09 14:31:53.000000 Flask-captcha2-2.0.1/Flask_captcha2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      299 2023-06-09 14:31:53.000000 Flask-captcha2-2.0.1/Flask_captcha2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 14:31:53.000000 Flask-captcha2-2.0.1/Flask_captcha2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-06-09 14:31:53.000000 Flask-captcha2-2.0.1/Flask_captcha2.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-09 14:31:53.000000 Flask-captcha2-2.0.1/Flask_captcha2.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1089 2023-06-09 13:55:48.000000 Flask-captcha2-2.0.1/LICENSE
+-rw-rw-rw-   0        0        0     4261 2023-06-09 14:31:53.596820 Flask-captcha2-2.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3638 2023-06-09 14:27:10.000000 Flask-captcha2-2.0.1/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-09 14:31:53.595819 Flask-captcha2-2.0.1/flask_captcha2/
+-rw-rw-rw-   0        0        0     4095 2023-06-09 13:55:48.000000 Flask-captcha2-2.0.1/flask_captcha2/CaptchaClass.py
+-rw-rw-rw-   0        0        0       59 2023-06-09 13:55:48.000000 Flask-captcha2-2.0.1/flask_captcha2/__init__.py
+-rw-rw-rw-   0        0        0      308 2023-06-09 14:02:57.000000 Flask-captcha2-2.0.1/flask_captcha2/auther.py
+-rw-rw-rw-   0        0        0       42 2023-06-09 14:31:53.597818 Flask-captcha2-2.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1036 2023-06-09 14:31:50.000000 Flask-captcha2-2.0.1/setup.py
```

### Comparing `flask_captcha2-2.0.0/flask_captcha2/__init__.py` & `Flask-captcha2-2.0.1/flask_captcha2/CaptchaClass.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,56 @@
 from flask import request
 import requests
 from markupsafe import Markup
 
 
-class Captcha:
+
+class BaseCaptcha3:
     """
-       Base Class For captcha object in app
+       Base Google Captcha v3 class
     """
     PUBLIC_KEY = None
     PRIVATE_KEY = None
     ENABLED = False
     THEME = "light",
     TABINDEX = 0
     LANGUAGE = "en"
     TYPE = "image"
     SIZE = "normal" # compact، normal، invisible
-
+    
+    MINIMUM_SCORE = 0.5 # uses for captcha v3
+    SHOW_CAPTCHA = True # uses for showing captcha v3
+    
     GOOGLE_VERIFY_URL = "https://www.google.com/recaptcha/api/siteverify"
 
 
-class FlaskCaptcha(Captcha):
+    
+class FlaskCaptcha3(BaseCaptcha3):
+    """ Google Captcha version 3 """
+    pass    
+    
+
+class BaseCaptcha2:
+    """
+       Base Google Captcha v2 class
+    """
+    PUBLIC_KEY = None
+    PRIVATE_KEY = None
+    ENABLED = False
+    THEME = "light",
+    TABINDEX = 0
+    LANGUAGE = "en"
+    TYPE = "image"
+    SIZE = "normal" # compact، normal، invisible
+    
+    GOOGLE_VERIFY_URL = "https://www.google.com/recaptcha/api/siteverify"
+
 
+class FlaskCaptcha2(BaseCaptcha2):
+    """ Google Captcha version 2 """
     def __init__(self, app=None, public_key=None, private_key=None, **kwargs):
         if app:
             self.init_app(app)
 
         elif private_key and public_key:
             self.PUBLIC_KEY = public_key
             self.PRIVATE_KEY = private_key
@@ -52,14 +78,15 @@
         )
         @app.context_processor
         def render_captcha():
             return{"captchaField": self.renderWidget()}
 
 
     def is_verify(self):
+        """ Verify a Captcha v2 """
         if not self.ENABLED:
             return True
         else:
             data = {
                 "secret": self.PRIVATE_KEY,
                 "response": request.form.get('g-recaptcha-response', None),
             }
@@ -82,17 +109,17 @@
             if responseGoogle.status_code == 200:
                 return responseGoogle.json()["success"]
             else:
                 return False
 
     def renderWidget(self):
         """
-            render captcha widget
+            render captcha v2 widget
         :return:
         """
         return Markup(f"""
         <script src='//www.google.com/recaptcha/api.js'></script>
             <div class="g-recaptcha" data-sitekey="{self.PUBLIC_KEY}"
                     data-theme="{self.THEME}" data-type="{self.TYPE}" data-size="{self.SIZE}"
                     data-tabindex="{self.TABINDEX}">
             </div>
-        """)
+        """) if self.ENABLED else ""
```

