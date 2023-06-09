# Comparing `tmp/pythttp-0.1.3.tar.gz` & `tmp/pythttp-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythttp-0.1.3.tar", last modified: Tue Jun  6 02:11:14 2023, max compression
+gzip compressed data, was "pythttp-0.1.4.tar", last modified: Fri Jun  9 15:38:50 2023, max compression
```

## Comparing `pythttp-0.1.3.tar` & `pythttp-0.1.4.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 02:11:14.886180 pythttp-0.1.3/
--rw-rw-rw-   0        0        0     1093 2023-06-06 02:11:14.885181 pythttp-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0      611 2023-05-03 09:40:52.000000 pythttp-0.1.3/README.md
--rw-rw-rw-   0        0        0      419 2023-06-06 02:11:08.000000 pythttp-0.1.3/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-06-06 02:11:14.872167 pythttp-0.1.3/pythttp/
--rw-rw-rw-   0        0        0      726 2023-06-03 23:42:42.000000 pythttp-0.1.3/pythttp/Log_Manager.py
--rw-rw-rw-   0        0        0     3528 2023-06-06 02:08:51.000000 pythttp-0.1.3/pythttp/Protocol.py
--rw-rw-rw-   0        0        0    13376 2023-06-06 02:09:27.000000 pythttp-0.1.3/pythttp/RequestHandler.py
--rw-rw-rw-   0        0        0     3896 2023-06-06 02:09:28.000000 pythttp-0.1.3/pythttp/Structure.py
--rw-rw-rw-   0        0        0     3064 2023-06-03 23:42:42.000000 pythttp-0.1.3/pythttp/Thread_Manager.py
--rw-rw-rw-   0        0        0      139 2023-06-03 23:42:42.000000 pythttp-0.1.3/pythttp/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-06 02:11:14.884178 pythttp-0.1.3/pythttp.egg-info/
--rw-rw-rw-   0        0        0     1093 2023-06-06 02:11:14.000000 pythttp-0.1.3/pythttp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      293 2023-06-06 02:11:14.000000 pythttp-0.1.3/pythttp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 02:11:14.000000 pythttp-0.1.3/pythttp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-06-06 02:11:14.000000 pythttp-0.1.3/pythttp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-06 02:11:14.886180 pythttp-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      603 2023-06-06 02:11:03.000000 pythttp-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 15:38:50.072056 pythttp-0.1.4/
+-rw-rw-rw-   0        0        0     1093 2023-06-09 15:38:50.072056 pythttp-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0      611 2023-05-03 09:40:52.000000 pythttp-0.1.4/README.md
+-rw-rw-rw-   0        0        0      419 2023-06-09 15:34:15.000000 pythttp-0.1.4/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-06-09 15:38:50.050305 pythttp-0.1.4/pythttp/
+-rw-rw-rw-   0        0        0      726 2023-06-03 23:42:42.000000 pythttp-0.1.4/pythttp/Log_Manager.py
+-rw-rw-rw-   0        0        0     3528 2023-06-06 02:08:51.000000 pythttp-0.1.4/pythttp/Protocol.py
+-rw-rw-rw-   0        0        0    12792 2023-06-09 15:33:35.000000 pythttp-0.1.4/pythttp/RequestHandler.py
+-rw-rw-rw-   0        0        0     3896 2023-06-06 02:09:28.000000 pythttp-0.1.4/pythttp/Structure.py
+-rw-rw-rw-   0        0        0     3064 2023-06-03 23:42:42.000000 pythttp-0.1.4/pythttp/Thread_Manager.py
+-rw-rw-rw-   0        0        0      139 2023-06-03 23:42:42.000000 pythttp-0.1.4/pythttp/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 15:38:50.070055 pythttp-0.1.4/pythttp.egg-info/
+-rw-rw-rw-   0        0        0     1093 2023-06-09 15:38:49.000000 pythttp-0.1.4/pythttp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      323 2023-06-09 15:38:49.000000 pythttp-0.1.4/pythttp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 15:38:49.000000 pythttp-0.1.4/pythttp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-06-09 15:38:49.000000 pythttp-0.1.4/pythttp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-09 15:38:49.000000 pythttp-0.1.4/pythttp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-09 15:38:50.073057 pythttp-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      634 2023-06-09 15:38:24.000000 pythttp-0.1.4/setup.py
```

### Comparing `pythttp-0.1.3/PKG-INFO` & `pythttp-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythttp
-Version: 0.1.3
+Version: 0.1.4
 Summary: A small example package
 Home-page: https://github.com/projectlonginus/httpy
 Author: Example Author
 Author-email: Longinus <team.longinus.project@gmail.com>
 Project-URL: Homepage, https://github.com/projectlonginus/httpy
 Project-URL: Bug Tracker, https://github.com/projectlonginus/httpy/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pythttp-0.1.3/README.md` & `pythttp-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `pythttp-0.1.3/pythttp/Log_Manager.py` & `pythttp-0.1.4/pythttp/Log_Manager.py`

 * *Files identical despite different names*

### Comparing `pythttp-0.1.3/pythttp/Protocol.py` & `pythttp-0.1.4/pythttp/Protocol.py`

 * *Files identical despite different names*

### Comparing `pythttp-0.1.3/pythttp/RequestHandler.py` & `pythttp-0.1.4/pythttp/RequestHandler.py`

 * *Files 3% similar despite different names*

```diff
@@ -64,34 +64,34 @@
                     Response= self.HandleTextFileRequest('/Login_form.html')
             elif (self.verifySessionCookie(Request)[0] and '/Logout_form' == result):
                 Response= self.HandleTextFileRequest('/Logout_form.html')
             elif '.html' in result:
                 Response=self.HandleTextFileRequest(result)
             return Response
         except FileNotFoundError:
-            with open('resource/Hello world.html','r',encoding='UTF-8') as arg:
+            with open('resource/Error_Form.html','r',encoding='UTF-8') as arg:
                 print(f'해당 resource{result}파일을 찾을수 없습니다.')
                 Error_Response=arg.read().format(msg=f'해당 resource{result}파일을 찾을수 없습니다.').encode('utf-8')
                 return PrepareHeader()._response_headers('404 Not Found',Error_Response) + Error_Response
 
     def HandlePOSTRequest(self,Request):
         JsonData=parse.unquote(Request[1])
         DictPostData=json.loads(JsonData)
         Form=DictPostData['Form']
         Response=self.HandleTextFileRequest()
         is_valid_cookie,cookie_value=self.verifySessionCookie(Request[0])
-        #try:
-        if Form == 'SignUp':
-            Response=self.SignUp_Handler(DictPostData['UserID'],DictPostData['UserName'],DictPostData['UserPw'],is_valid_cookie)
-        elif Form == 'Login':
-            Response=self.Login_Handler(DictPostData['UserID'],DictPostData['UserPw'],is_valid_cookie)
-        elif Form == 'Logout':
-            Response=self.Logout_Handler(cookie_value)
-        #except Exception as e:
-            #Response=self.ErrorHandler(e)
+        try:
+            if Form == 'SignUp':
+                Response=self.SignUp_Handler(DictPostData['UserID'],DictPostData['UserName'],DictPostData['UserPw'],is_valid_cookie)
+            elif Form == 'Login':
+                Response=self.Login_Handler(DictPostData['UserID'],DictPostData['UserPw'],is_valid_cookie)
+            elif Form == 'Logout':
+                Response=self.Logout_Handler(cookie_value)
+        except Exception as e:
+            Response=self.ErrorHandler('400 Bad Request',e)
         return Response
 
     def verifySessionCookie(self,RequestData:list):
         for data in RequestData:
             if ('Cookie' in data and 'SessionID=' in data):
                 Values = data.split('SessionID=')[1]
                 for Session in self.Sessions:
@@ -100,30 +100,25 @@
         return False, None
 
     def HandleFileRequest(self,img_file='/a.png'):
         with open(f'resource{img_file}', 'rb') as ImgFile:
             Response_file=ImgFile.read()
             return PrepareHeader()._response_headers('200 OK',Response_file) + Response_file
         
-    def HandleTextFileRequest(self,flie='/Hello world.html'):
+    def HandleTextFileRequest(self,flie='/Index.html',Cookie=None):
         with open(f'resource{flie}','r',encoding='UTF-8') as TextFile:
             Response_file=TextFile.read().encode('UTF-8')
-        return PrepareHeader()._response_headers('200 OK',Response_file) + Response_file
+        return PrepareHeader()._response_headers('200 OK',Response_file,Cookie) + Response_file
     
-    def HandleMultiFileRequest(self,title,headline,pagemsg,Cookie=None):
-        with open(f'resource/multipurpos_page.html','r',encoding='UTF-8') as TextFile:
-            Text=TextFile.read()
-            Response_file=Text.format(title=title,headline=headline,pagemsg=pagemsg).encode('UTF-8')
-        return PrepareHeader()._response_headers('200 OK',Response_file,Cookie=Cookie) + Response_file
-    
-    def ErrorHandler(self,Error_msg):
+    def ErrorHandler(self,Error_code,Error_msg):
         with open(f'resource/Error_Form.html','r',encoding='UTF-8') as TextFile:
             Response_file=TextFile.read()
-            Response_file=Response_file.format(msg=Error_msg).encode('utf-8')
-        return PrepareHeader()._response_headers('200 OK',Response_file) + Response_file
+            Response_file=Response_file.replace('{0}',Error_code).replace('{1}',Error_msg).encode('utf-8')
+
+        return PrepareHeader()._response_headers('200',Response_file) + Response_file
     
     def addFormatToHTML(self,HtmlText : str, FormatData : dict, style : str):
         Format=''
         for key,val in FormatData.items():
             Format+=f'{style.format(val=val,key=key)}'
         HtmlText=HtmlText.format(Format=Format)
         return HtmlText
@@ -133,50 +128,50 @@
             ImgFile.write(img_file)
             self.ServerDB['Img']={file_name:f'/ImgFileUpload/{file_name}'}
             return file_name
 
     def SignUp_Handler(self,UserID,UserName,UserPw,is_valid_cookie):
         UserUID=uuid.uuid5(uuid.UUID('30076a53-4522-5b28-af4c-b30c260a456d'), UserID)
         if self.Sessions and is_valid_cookie:
-            return self.ErrorHandler(Error_msg='Warning: You are already logged in. There is no need to log in again. You can continue using the current account.')
+            return self.ErrorHandler('403 Forbidden','Warning: You are already logged in. There is no need to log in again. You can continue using the current account.')
         for DB in self.ServerUsersDB:
             if (UserUID == DB.UserUID):
-                return self.HandleMultiFileRequest('Error Page','Error!',f'User information error! Duplicate ID! : {UserID}')
+                return self.ErrorHandler('406 Not Acceptable',f'User information error! Duplicate ID! : {UserID}')  
         try:
             AuthenticatedName,AuthenticatedPassword=Verify().VerifyCredentials(UserName, UserPw)
         except Exception as e:
-            return self.ErrorHandler(Error_msg=f'{e} : {UserName,UserPw}')
+            return self.ErrorHandler('403 Forbidden',f'{e} : {UserName,UserPw}')
         DB=StructDB(UserUID,AuthenticatedName,AuthenticatedPassword)
         self.ServerUsersDB.add(DB)
         self.log(f"[ New DataBase Constructed ] ==> DBID : \033[95m{DB.DataBaseID}\033[0m")
         self.log(f"[ SignUp User ] ==> UUID : \033[96m{UserUID}\033[0m")
         self.HandleSaveDB()
-        return self.HandleMultiFileRequest('SignUp Successful',f'SignUp Successful! \n User : {UserName}','Your registration has been successfully completed. You can start using our services.')
+        return self.HandleTextFileRequest('/SignUp_Action.html')
 
     def Login_Handler(self, user_id, user_pw ,is_valid_cookie):
         user_uid = uuid.uuid5(uuid.UUID('30076a53-4522-5b28-af4c-b30c260a456d'), user_id)
         # Check if user is already logged in
         if self.Sessions and is_valid_cookie:
-            return self.ErrorHandler(Error_msg='Warning: You are already logged in. There is no need to log in again. You can continue using the current account.')
+            return self.ErrorHandler('403 Forbidden','Warning: You are already logged in. There is no need to log in again. You can continue using the current account.')
         # Check user credentials and create new session
         for db in self.ServerUsersDB:
             if user_uid == db.UserUID and user_pw == db.UserPw:
                 session_id = self.RegisterUserSession(7, {'UserUID': user_uid})
-                self.log(f"[New Session Constructed] ==> SessionID: \033[96m{session_id}\033[0m")
-                return self.HandleMultiFileRequest('Welcome', f'Welcome! User: {user_id}', f"Dear {user_id}, thank you for logging in. We're excited to have you on board!", Cookie=f'SessionID = {session_id}')        
-        return self.ErrorHandler(Error_msg=f'User ID or password does not exist: {user_id, user_pw}')
+                self.log(f"[ New Session Constructed ] ==> SessionID: \033[96m{session_id}\033[0m")
+                return self.HandleTextFileRequest('/Login_Action.html',Cookie=f'SessionID = {session_id}')       
+        return self.ErrorHandler('422 Unprocessable Entity',f'User ID or password does not exist: {user_id, user_pw}')
 
     
     def Logout_Handler(self,SessionID):
         for Session in self.Sessions:
             if Session.SessionToken == SessionID:
                 self.Sessions.remove(Session)
                 self.log(f"[ Session Destructed ] ==> SessionID : \033[96m{SessionID}\033[0m")
-                return self.HandleMultiFileRequest('Logout',f'Goodbye!',f'Thank you for using our services. We hope to see you again soon!')
-        return self.ErrorHandler(Error_msg=f'To log out, you must first log in. Please verify your account information and log in before attempting to log out')
+                return self.HandleTextFileRequest('/Logout_Action.html')
+        return self.ErrorHandler('403 Forbidden',f'To log out, you must first log in. Please verify your account information and log in before attempting to log out')
 
     def RegisterUserSession(self,  SessionValidityDays: str, UserInfo: dict):
         SessionInfo = Session(SessionValidityDays, UserInfo)
         self.Sessions.add(SessionInfo)
         return SessionInfo.SessionToken
 
     def HandleSaveDB(self):
```

### Comparing `pythttp-0.1.3/pythttp/Structure.py` & `pythttp-0.1.4/pythttp/Structure.py`

 * *Files identical despite different names*

### Comparing `pythttp-0.1.3/pythttp/Thread_Manager.py` & `pythttp-0.1.4/pythttp/Thread_Manager.py`

 * *Files identical despite different names*

### Comparing `pythttp-0.1.3/pythttp.egg-info/PKG-INFO` & `pythttp-0.1.4/pythttp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythttp
-Version: 0.1.3
+Version: 0.1.4
 Summary: A small example package
 Home-page: https://github.com/projectlonginus/httpy
 Author: Example Author
 Author-email: Longinus <team.longinus.project@gmail.com>
 Project-URL: Homepage, https://github.com/projectlonginus/httpy
 Project-URL: Bug Tracker, https://github.com/projectlonginus/httpy/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pythttp-0.1.3/setup.py` & `pythttp-0.1.4/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import setuptools
 
 with open(r"README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pythttp",
-    version="0.1.3",
+    version="0.1.4",
     author="Example Author",
     author_email="team.longinus.project@gmail.com",
     description="A small example package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/projectlonginus/httpy",
-    install_requires=[],
+    install_requires=['dataclasses','datetime','uuid'],
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
     ],
     python_requires='>=3.11',
 )
```

