# Comparing `tmp/pythttp-0.1.4.tar.gz` & `tmp/pythttp-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythttp-0.1.4.tar", last modified: Fri Jun  9 15:38:50 2023, max compression
+gzip compressed data, was "pythttp-0.1.5.tar", last modified: Fri Jun  9 15:53:29 2023, max compression
```

## Comparing `pythttp-0.1.4.tar` & `pythttp-0.1.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 15:38:50.072056 pythttp-0.1.4/
--rw-rw-rw-   0        0        0     1093 2023-06-09 15:38:50.072056 pythttp-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0      611 2023-05-03 09:40:52.000000 pythttp-0.1.4/README.md
--rw-rw-rw-   0        0        0      419 2023-06-09 15:34:15.000000 pythttp-0.1.4/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-06-09 15:38:50.050305 pythttp-0.1.4/pythttp/
--rw-rw-rw-   0        0        0      726 2023-06-03 23:42:42.000000 pythttp-0.1.4/pythttp/Log_Manager.py
--rw-rw-rw-   0        0        0     3528 2023-06-06 02:08:51.000000 pythttp-0.1.4/pythttp/Protocol.py
--rw-rw-rw-   0        0        0    12792 2023-06-09 15:33:35.000000 pythttp-0.1.4/pythttp/RequestHandler.py
--rw-rw-rw-   0        0        0     3896 2023-06-06 02:09:28.000000 pythttp-0.1.4/pythttp/Structure.py
--rw-rw-rw-   0        0        0     3064 2023-06-03 23:42:42.000000 pythttp-0.1.4/pythttp/Thread_Manager.py
--rw-rw-rw-   0        0        0      139 2023-06-03 23:42:42.000000 pythttp-0.1.4/pythttp/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-09 15:38:50.070055 pythttp-0.1.4/pythttp.egg-info/
--rw-rw-rw-   0        0        0     1093 2023-06-09 15:38:49.000000 pythttp-0.1.4/pythttp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      323 2023-06-09 15:38:49.000000 pythttp-0.1.4/pythttp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 15:38:49.000000 pythttp-0.1.4/pythttp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-06-09 15:38:49.000000 pythttp-0.1.4/pythttp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-09 15:38:49.000000 pythttp-0.1.4/pythttp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-09 15:38:50.073057 pythttp-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      634 2023-06-09 15:38:24.000000 pythttp-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 15:53:29.769920 pythttp-0.1.5/
+-rw-rw-rw-   0        0        0     1093 2023-06-09 15:53:29.769920 pythttp-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0      611 2023-05-03 09:40:52.000000 pythttp-0.1.5/README.md
+-rw-rw-rw-   0        0        0      419 2023-06-09 15:53:10.000000 pythttp-0.1.5/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-06-09 15:53:29.757591 pythttp-0.1.5/pythttp/
+-rw-rw-rw-   0        0        0      726 2023-06-03 23:42:42.000000 pythttp-0.1.5/pythttp/Log_Manager.py
+-rw-rw-rw-   0        0        0     3528 2023-06-06 02:08:51.000000 pythttp-0.1.5/pythttp/Protocol.py
+-rw-rw-rw-   0        0        0    12667 2023-06-09 15:52:34.000000 pythttp-0.1.5/pythttp/RequestHandler.py
+-rw-rw-rw-   0        0        0     3896 2023-06-06 02:09:28.000000 pythttp-0.1.5/pythttp/Structure.py
+-rw-rw-rw-   0        0        0     3064 2023-06-03 23:42:42.000000 pythttp-0.1.5/pythttp/Thread_Manager.py
+-rw-rw-rw-   0        0        0      139 2023-06-03 23:42:42.000000 pythttp-0.1.5/pythttp/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 15:53:29.767919 pythttp-0.1.5/pythttp.egg-info/
+-rw-rw-rw-   0        0        0     1093 2023-06-09 15:53:29.000000 pythttp-0.1.5/pythttp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      323 2023-06-09 15:53:29.000000 pythttp-0.1.5/pythttp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 15:53:29.000000 pythttp-0.1.5/pythttp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-06-09 15:53:29.000000 pythttp-0.1.5/pythttp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-09 15:53:29.000000 pythttp-0.1.5/pythttp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-09 15:53:29.769920 pythttp-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      634 2023-06-09 15:53:14.000000 pythttp-0.1.5/setup.py
```

### Comparing `pythttp-0.1.4/PKG-INFO` & `pythttp-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythttp
-Version: 0.1.4
+Version: 0.1.5
 Summary: A small example package
 Home-page: https://github.com/projectlonginus/httpy
 Author: Example Author
 Author-email: Longinus <team.longinus.project@gmail.com>
 Project-URL: Homepage, https://github.com/projectlonginus/httpy
 Project-URL: Bug Tracker, https://github.com/projectlonginus/httpy/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pythttp-0.1.4/README.md` & `pythttp-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `pythttp-0.1.4/pythttp/Log_Manager.py` & `pythttp-0.1.5/pythttp/Log_Manager.py`

 * *Files identical despite different names*

### Comparing `pythttp-0.1.4/pythttp/Protocol.py` & `pythttp-0.1.5/pythttp/Protocol.py`

 * *Files identical despite different names*

### Comparing `pythttp-0.1.4/pythttp/RequestHandler.py` & `pythttp-0.1.5/pythttp/RequestHandler.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,17 +65,15 @@
             elif (self.verifySessionCookie(Request)[0] and '/Logout_form' == result):
                 Response= self.HandleTextFileRequest('/Logout_form.html')
             elif '.html' in result:
                 Response=self.HandleTextFileRequest(result)
             return Response
         except FileNotFoundError:
             with open('resource/Error_Form.html','r',encoding='UTF-8') as arg:
-                print(f'해당 resource{result}파일을 찾을수 없습니다.')
-                Error_Response=arg.read().format(msg=f'해당 resource{result}파일을 찾을수 없습니다.').encode('utf-8')
-                return PrepareHeader()._response_headers('404 Not Found',Error_Response) + Error_Response
+                return self.ErrorHandler('404 Not Found',f'The corresponding resource{result}file could not be found.')
 
     def HandlePOSTRequest(self,Request):
         JsonData=parse.unquote(Request[1])
         DictPostData=json.loads(JsonData)
         Form=DictPostData['Form']
         Response=self.HandleTextFileRequest()
         is_valid_cookie,cookie_value=self.verifySessionCookie(Request[0])
@@ -109,15 +107,15 @@
             Response_file=TextFile.read().encode('UTF-8')
         return PrepareHeader()._response_headers('200 OK',Response_file,Cookie) + Response_file
     
     def ErrorHandler(self,Error_code,Error_msg):
         with open(f'resource/Error_Form.html','r',encoding='UTF-8') as TextFile:
             Response_file=TextFile.read()
             Response_file=Response_file.replace('{0}',Error_code).replace('{1}',Error_msg).encode('utf-8')
-
+        self.log(f"[ Handle Error ] ==> Code : \033[91m{Error_code}\033[0m")
         return PrepareHeader()._response_headers('200',Response_file) + Response_file
     
     def addFormatToHTML(self,HtmlText : str, FormatData : dict, style : str):
         Format=''
         for key,val in FormatData.items():
             Format+=f'{style.format(val=val,key=key)}'
         HtmlText=HtmlText.format(Format=Format)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pythttp-0.1.4/pythttp/Structure.py` & `pythttp-0.1.5/pythttp/Structure.py`

 * *Files identical despite different names*

### Comparing `pythttp-0.1.4/pythttp/Thread_Manager.py` & `pythttp-0.1.5/pythttp/Thread_Manager.py`

 * *Files identical despite different names*

### Comparing `pythttp-0.1.4/pythttp.egg-info/PKG-INFO` & `pythttp-0.1.5/pythttp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythttp
-Version: 0.1.4
+Version: 0.1.5
 Summary: A small example package
 Home-page: https://github.com/projectlonginus/httpy
 Author: Example Author
 Author-email: Longinus <team.longinus.project@gmail.com>
 Project-URL: Homepage, https://github.com/projectlonginus/httpy
 Project-URL: Bug Tracker, https://github.com/projectlonginus/httpy/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pythttp-0.1.4/setup.py` & `pythttp-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open(r"README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pythttp",
-    version="0.1.4",
+    version="0.1.5",
     author="Example Author",
     author_email="team.longinus.project@gmail.com",
     description="A small example package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/projectlonginus/httpy",
     install_requires=['dataclasses','datetime','uuid'],
```

