# Comparing `tmp/one_py_sdk-1.5.2.tar.gz` & `tmp/one_py_sdk-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\dedwards\source\repos\ONE.Py.SDK\dist\.tmp-r2689uaa\one_py_sdk-1.5.2.tar", last modified: Tue Mar 14 15:43:35 2023, max compression
+gzip compressed data, was "C:\Users\dedwards\source\repos\ONE.Py.SDK\dist\.tmp-lxw6tnpc\one_py_sdk-1.5.3.tar", last modified: Fri Jun  9 15:37:40 2023, max compression
```

## Comparing `one_py_sdk-1.5.2.tar` & `one_py_sdk-1.5.3.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxrwx   0        0        0        0 2023-03-14 15:43:35.479219 one_py_sdk-1.5.2/
--rw-rw-rw-   0        0        0     1091 2022-07-20 17:47:04.000000 one_py_sdk-1.5.2/LICENSE
--rw-rw-rw-   0        0        0     2195 2023-03-14 15:43:35.479219 one_py_sdk-1.5.2/PKG-INFO
--rw-rw-rw-   0        0        0      270 2022-07-27 16:24:32.000000 one_py_sdk-1.5.2/README.md
--rw-rw-rw-   0        0        0      905 2023-03-14 14:32:34.000000 one_py_sdk-1.5.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-03-14 15:43:35.480217 one_py_sdk-1.5.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-03-14 15:43:35.409218 one_py_sdk-1.5.2/src/
-drwxrwxrwx   0        0        0        0 2023-03-14 15:43:35.422217 one_py_sdk-1.5.2/src/one_py_sdk/
--rw-rw-rw-   0        0        0        0 2022-07-20 17:34:59.000000 one_py_sdk-1.5.2/src/one_py_sdk/__init__.py
--rw-rw-rw-   0        0        0     2425 2023-02-28 21:50:18.000000 one_py_sdk-1.5.2/src/one_py_sdk/clientsdk.py
-drwxrwxrwx   0        0        0        0 2023-03-14 15:43:35.438218 one_py_sdk-1.5.2/src/one_py_sdk/common/
--rw-rw-rw-   0        0        0        0 2022-07-20 20:21:12.000000 one_py_sdk-1.5.2/src/one_py_sdk/common/__init__.py
--rw-rw-rw-   0        0        0     1010 2023-02-28 21:31:35.000000 one_py_sdk-1.5.2/src/one_py_sdk/common/configuration.py
--rw-rw-rw-   0        0        0     2172 2023-02-28 22:38:08.000000 one_py_sdk-1.5.2/src/one_py_sdk/common/library.py
-drwxrwxrwx   0        0        0        0 2023-03-14 15:43:35.448217 one_py_sdk-1.5.2/src/one_py_sdk/enterprise/
--rw-rw-rw-   0        0        0        0 2022-06-30 16:44:38.000000 one_py_sdk-1.5.2/src/one_py_sdk/enterprise/__init__.py
--rw-rw-rw-   0        0        0     4425 2023-03-06 15:20:33.000000 one_py_sdk-1.5.2/src/one_py_sdk/enterprise/authentication.py
--rw-rw-rw-   0        0        0     1244 2023-02-28 21:29:16.000000 one_py_sdk-1.5.2/src/one_py_sdk/enterprise/core.py
--rw-rw-rw-   0        0        0     3858 2023-03-01 16:37:37.000000 one_py_sdk-1.5.2/src/one_py_sdk/enterprise/report.py
--rw-rw-rw-   0        0        0     5879 2023-02-28 22:05:06.000000 one_py_sdk-1.5.2/src/one_py_sdk/enterprise/twin.py
-drwxrwxrwx   0        0        0        0 2023-03-14 15:43:35.452219 one_py_sdk-1.5.2/src/one_py_sdk/historian/
--rw-rw-rw-   0        0        0        0 2022-07-20 20:21:28.000000 one_py_sdk-1.5.2/src/one_py_sdk/historian/__init__.py
--rw-rw-rw-   0        0        0     1554 2023-03-01 16:40:12.000000 one_py_sdk-1.5.2/src/one_py_sdk/historian/data.py
-drwxrwxrwx   0        0        0        0 2023-03-14 15:43:35.456219 one_py_sdk-1.5.2/src/one_py_sdk/operations/
--rw-rw-rw-   0        0        0        0 2022-07-20 19:55:31.000000 one_py_sdk-1.5.2/src/one_py_sdk/operations/__init__.py
--rw-rw-rw-   0        0        0    11807 2023-03-14 14:27:31.000000 one_py_sdk-1.5.2/src/one_py_sdk/operations/spreadsheet.py
-drwxrwxrwx   0        0        0        0 2023-03-14 15:43:35.461219 one_py_sdk-1.5.2/src/one_py_sdk/shared/
--rw-rw-rw-   0        0        0        0 2022-07-06 13:22:29.000000 one_py_sdk-1.5.2/src/one_py_sdk/shared/__init__.py
--rw-rw-rw-   0        0        0      272 2022-12-01 23:03:28.000000 one_py_sdk-1.5.2/src/one_py_sdk/shared/constants.py
-drwxrwxrwx   0        0        0        0 2023-03-14 15:43:35.473219 one_py_sdk-1.5.2/src/one_py_sdk/shared/helpers/
--rw-rw-rw-   0        0        0        0 2022-07-20 20:21:55.000000 one_py_sdk-1.5.2/src/one_py_sdk/shared/helpers/__init__.py
--rw-rw-rw-   0        0        0    31014 2023-03-06 21:38:25.000000 one_py_sdk-1.5.2/src/one_py_sdk/shared/helpers/csvhelper.py
--rw-rw-rw-   0        0        0     2693 2023-03-14 14:52:53.000000 one_py_sdk-1.5.2/src/one_py_sdk/shared/helpers/datetimehelper.py
--rw-rw-rw-   0        0        0      201 2023-02-27 22:52:21.000000 one_py_sdk-1.5.2/src/one_py_sdk/shared/helpers/helpers.py
--rw-rw-rw-   0        0        0     1354 2023-03-06 17:27:24.000000 one_py_sdk-1.5.2/src/one_py_sdk/shared/helpers/protobufhelper.py
-drwxrwxrwx   0        0        0        0 2023-03-14 15:43:35.476218 one_py_sdk-1.5.2/src/one_py_sdk/shared/models/
--rw-rw-rw-   0        0        0      667 2023-03-01 17:46:40.000000 one_py_sdk-1.5.2/src/one_py_sdk/shared/models/datapoint.py
-drwxrwxrwx   0        0        0        0 2023-03-14 15:43:35.432217 one_py_sdk-1.5.2/src/one_py_sdk.egg-info/
--rw-rw-rw-   0        0        0     2195 2023-03-14 15:43:35.000000 one_py_sdk-1.5.2/src/one_py_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1050 2023-03-14 15:43:35.000000 one_py_sdk-1.5.2/src/one_py_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-14 15:43:35.000000 one_py_sdk-1.5.2/src/one_py_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-03-14 15:43:35.000000 one_py_sdk-1.5.2/src/one_py_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-03-14 15:43:35.000000 one_py_sdk-1.5.2/src/one_py_sdk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-09 15:37:40.879246 one_py_sdk-1.5.3/
+-rw-rw-rw-   0        0        0     1091 2022-07-20 17:47:04.000000 one_py_sdk-1.5.3/LICENSE
+-rw-rw-rw-   0        0        0     2195 2023-06-09 15:37:40.878245 one_py_sdk-1.5.3/PKG-INFO
+-rw-rw-rw-   0        0        0      270 2022-07-27 16:24:32.000000 one_py_sdk-1.5.3/README.md
+-rw-rw-rw-   0        0        0      905 2023-05-31 14:21:35.000000 one_py_sdk-1.5.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-09 15:37:40.880250 one_py_sdk-1.5.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-09 15:37:40.785247 one_py_sdk-1.5.3/src/
+drwxrwxrwx   0        0        0        0 2023-06-09 15:37:40.803247 one_py_sdk-1.5.3/src/one_py_sdk/
+-rw-rw-rw-   0        0        0        0 2022-07-20 17:34:59.000000 one_py_sdk-1.5.3/src/one_py_sdk/__init__.py
+-rw-rw-rw-   0        0        0     2425 2023-02-28 21:50:18.000000 one_py_sdk-1.5.3/src/one_py_sdk/clientsdk.py
+drwxrwxrwx   0        0        0        0 2023-06-09 15:37:40.824247 one_py_sdk-1.5.3/src/one_py_sdk/common/
+-rw-rw-rw-   0        0        0        0 2022-07-20 20:21:12.000000 one_py_sdk-1.5.3/src/one_py_sdk/common/__init__.py
+-rw-rw-rw-   0        0        0     1010 2023-02-28 21:31:35.000000 one_py_sdk-1.5.3/src/one_py_sdk/common/configuration.py
+-rw-rw-rw-   0        0        0     2172 2023-02-28 22:38:08.000000 one_py_sdk-1.5.3/src/one_py_sdk/common/library.py
+drwxrwxrwx   0        0        0        0 2023-06-09 15:37:40.839246 one_py_sdk-1.5.3/src/one_py_sdk/enterprise/
+-rw-rw-rw-   0        0        0        0 2022-06-30 16:44:38.000000 one_py_sdk-1.5.3/src/one_py_sdk/enterprise/__init__.py
+-rw-rw-rw-   0        0        0     4533 2023-06-01 20:34:36.000000 one_py_sdk-1.5.3/src/one_py_sdk/enterprise/authentication.py
+-rw-rw-rw-   0        0        0     1244 2023-02-28 21:29:16.000000 one_py_sdk-1.5.3/src/one_py_sdk/enterprise/core.py
+-rw-rw-rw-   0        0        0     3858 2023-03-01 16:37:37.000000 one_py_sdk-1.5.3/src/one_py_sdk/enterprise/report.py
+-rw-rw-rw-   0        0        0     5879 2023-02-28 22:05:06.000000 one_py_sdk-1.5.3/src/one_py_sdk/enterprise/twin.py
+drwxrwxrwx   0        0        0        0 2023-06-09 15:37:40.845263 one_py_sdk-1.5.3/src/one_py_sdk/historian/
+-rw-rw-rw-   0        0        0        0 2022-07-20 20:21:28.000000 one_py_sdk-1.5.3/src/one_py_sdk/historian/__init__.py
+-rw-rw-rw-   0        0        0     1554 2023-03-01 16:40:12.000000 one_py_sdk-1.5.3/src/one_py_sdk/historian/data.py
+drwxrwxrwx   0        0        0        0 2023-06-09 15:37:40.852246 one_py_sdk-1.5.3/src/one_py_sdk/operations/
+-rw-rw-rw-   0        0        0        0 2022-07-20 19:55:31.000000 one_py_sdk-1.5.3/src/one_py_sdk/operations/__init__.py
+-rw-rw-rw-   0        0        0    11778 2023-05-31 14:18:29.000000 one_py_sdk-1.5.3/src/one_py_sdk/operations/spreadsheet.py
+drwxrwxrwx   0        0        0        0 2023-06-09 15:37:40.857246 one_py_sdk-1.5.3/src/one_py_sdk/shared/
+-rw-rw-rw-   0        0        0        0 2022-07-06 13:22:29.000000 one_py_sdk-1.5.3/src/one_py_sdk/shared/__init__.py
+-rw-rw-rw-   0        0        0      272 2022-12-01 23:03:28.000000 one_py_sdk-1.5.3/src/one_py_sdk/shared/constants.py
+drwxrwxrwx   0        0        0        0 2023-06-09 15:37:40.873246 one_py_sdk-1.5.3/src/one_py_sdk/shared/helpers/
+-rw-rw-rw-   0        0        0        0 2022-07-20 20:21:55.000000 one_py_sdk-1.5.3/src/one_py_sdk/shared/helpers/__init__.py
+-rw-rw-rw-   0        0        0    31014 2023-03-06 21:38:25.000000 one_py_sdk-1.5.3/src/one_py_sdk/shared/helpers/csvhelper.py
+-rw-rw-rw-   0        0        0     2693 2023-03-14 14:52:53.000000 one_py_sdk-1.5.3/src/one_py_sdk/shared/helpers/datetimehelper.py
+-rw-rw-rw-   0        0        0      201 2023-02-27 22:52:21.000000 one_py_sdk-1.5.3/src/one_py_sdk/shared/helpers/helpers.py
+-rw-rw-rw-   0        0        0     1354 2023-03-06 17:27:24.000000 one_py_sdk-1.5.3/src/one_py_sdk/shared/helpers/protobufhelper.py
+drwxrwxrwx   0        0        0        0 2023-06-09 15:37:40.876246 one_py_sdk-1.5.3/src/one_py_sdk/shared/models/
+-rw-rw-rw-   0        0        0      667 2023-03-01 17:46:40.000000 one_py_sdk-1.5.3/src/one_py_sdk/shared/models/datapoint.py
+drwxrwxrwx   0        0        0        0 2023-06-09 15:37:40.815246 one_py_sdk-1.5.3/src/one_py_sdk.egg-info/
+-rw-rw-rw-   0        0        0     2195 2023-06-09 15:37:40.000000 one_py_sdk-1.5.3/src/one_py_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1050 2023-06-09 15:37:40.000000 one_py_sdk-1.5.3/src/one_py_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 15:37:40.000000 one_py_sdk-1.5.3/src/one_py_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-06-09 15:37:40.000000 one_py_sdk-1.5.3/src/one_py_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-09 15:37:40.000000 one_py_sdk-1.5.3/src/one_py_sdk.egg-info/top_level.txt
```

### Comparing `one_py_sdk-1.5.2/LICENSE` & `one_py_sdk-1.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `one_py_sdk-1.5.2/PKG-INFO` & `one_py_sdk-1.5.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: one_py_sdk
-Version: 1.5.2
+Version: 1.5.3
 Summary: A package to interact with the ONE waterquality platform APIs.
 Author-email: AquaticInformatics <daniel.edwards@aquaticinformatics.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `one_py_sdk-1.5.2/pyproject.toml` & `one_py_sdk-1.5.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 00000010: 7265 7175 6972 6573 203d 205b 2273 6574  requires = ["set
 00000020: 7570 746f 6f6c 733e 3d36 312e 3022 5d0d  uptools>=61.0"].
 00000030: 0a62 7569 6c64 2d62 6163 6b65 6e64 203d  .build-backend =
 00000040: 2022 7365 7475 7074 6f6f 6c73 2e62 7569   "setuptools.bui
 00000050: 6c64 5f6d 6574 6122 0d0a 5b70 726f 6a65  ld_meta"..[proje
 00000060: 6374 5d0d 0a6e 616d 6520 3d20 226f 6e65  ct]..name = "one
 00000070: 5f70 795f 7364 6b22 0d0a 7665 7273 696f  _py_sdk"..versio
-00000080: 6e20 3d20 2231 2e35 2e32 220d 0a64 6570  n = "1.5.2"..dep
+00000080: 6e20 3d20 2231 2e35 2e33 220d 0a64 6570  n = "1.5.3"..dep
 00000090: 656e 6465 6e63 6965 7320 3d20 5b0d 0a20  endencies = [.. 
 000000a0: 2020 2022 7265 7175 6573 7473 222c 0d0a     "requests",..
 000000b0: 2020 2020 2270 726f 746f 6275 663d 3d33      "protobuf==3
 000000c0: 2e32 302e 3122 2c20 0d0a 2020 2020 226f  .20.1", ..    "o
 000000d0: 6e65 5f69 6e74 6572 6661 6365 7322 2c0d  ne_interfaces",.
 000000e0: 0a20 2020 2022 7265 7175 6573 7473 5f63  .    "requests_c
 000000f0: 6163 6865 222c 0d0a 2020 2020 2270 7974  ache",..    "pyt
```

### Comparing `one_py_sdk-1.5.2/src/one_py_sdk/clientsdk.py` & `one_py_sdk-1.5.3/src/one_py_sdk/clientsdk.py`

 * *Files identical despite different names*

### Comparing `one_py_sdk-1.5.2/src/one_py_sdk/common/configuration.py` & `one_py_sdk-1.5.3/src/one_py_sdk/common/configuration.py`

 * *Files identical despite different names*

### Comparing `one_py_sdk-1.5.2/src/one_py_sdk/common/library.py` & `one_py_sdk-1.5.3/src/one_py_sdk/common/library.py`

 * *Files identical despite different names*

### Comparing `one_py_sdk-1.5.2/src/one_py_sdk/enterprise/authentication.py` & `one_py_sdk-1.5.3/src/one_py_sdk/enterprise/authentication.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,108 +1,108 @@
-import requests
-import json
-from datetime import datetime, time, timedelta
-from one_py_sdk.shared.helpers.protobufhelper import DeserializeResponse
-from one_interfaces import user_pb2 as User
-from one_interfaces import role_pb2 as role
-
-import google
-
-
-class AuthenticationApi:
-    def __init__(self, env, session: requests.Session = None ):
-        self.Environment = env
-        self.Token = Token()
-        self.UserName = ""
-        self.Password = ""
-        self.User: User = User.User()
-        self.IsAuthenticated = False
-        if not session:
-            self.Session = requests.Session()
-            self.Session.headers = {"Content-Type": "application/x-protobuf", "Accept": "application/x-protobuf"}            
-        else:
-            self.Session = session
-
-    def GetToken(self, user, password):
-        data = {'username': user, 'password': password, 'grant_type': 'password', 'scope': 'FFAccessAPI openid',
-                'client_id': 'VSTestClient', 'client_secret': '0CCBB786-9412-4088-BC16-78D3A10158B7'}
-        headers = {'Accept': 'application/json',
-                   'Content-Type': 'application/x-www-form-urlencoded'}
-        url = self.Environment+"/connect/token"
-        response = requests.post(url, headers=headers, data=data)
-        if (response.status_code != 200):
-            return ''
-        self.__setToken(response)
-        self.IsAuthenticated = True
-        self.UserName = user
-        self.Password = password
-        self.Session.headers.update({'Authorization': self.Token.access_token})
-        return self.Token.access_token
-
-    def GetUserInfo(self):
-        headers = {'Accept': 'application/json',
-                   "Authorization": self.Token.access_token}
-        url = self.Environment+"/connect/userinfo"
-        response = requests.get(url, headers=headers)
-        self.__setInfo(response)
-        return response.content
-
-    def LoginResourceOwner(self, userName, password):
-        data = {'username': userName, 'password': password, 'grant_type': 'password', 'scope': 'FFAccessAPI openid',
-                'client_id': 'VSTestClient', 'client_secret': '0CCBB786-9412-4088-BC16-78D3A10158B7'}
-        headers = {'Accept': 'application/json',
-                   'Content-Type': 'application/x-www-form-urlencoded'}
-        url = self.Environment+"/connect/token"
-        response = requests.post(url, headers=headers, data=data)
-        if (response.status_code != 200):
-            return False
-        self.__setToken(response)
-        self.IsAuthenticated = True
-        self.UserName = userName
-        self.Password = password
-        self.Session.headers.update({'Authorization': self.Token.access_token})
-        return True
-
-    def Logout(self):
-        headers = {'Accept': 'application/json',
-                   "Authorization": self.Token.access_token}
-        url = self.Environment+"/account/logout"
-        requests.post(url, headers=headers)
-        self.Token = Token()
-        self.UserName = ""
-        self.Password = ""
-        self.User: User = User.User()
-        self.IsAuthenticated = False
-
-    def __setInfo(self, response):
-        jResponse = json.loads(response.content)
-        self.User.firstName.value = jResponse.get('given_name')
-        self.User.lastName.value = jResponse.get('family_name')
-        self.User.userName = jResponse.get('user_name')
-        self.User.email.value = jResponse.get('email')
-        self.User.tenantId = jResponse.get('ActiveTenantId')
-        self.User.id = jResponse.get('sub')
-
-    def __setToken(self, tokenResponse):
-        token = Token()
-        token.created = datetime.now()
-        responseJson = json.loads(tokenResponse.content)
-        self.IsAuthenticated = True
-        token.token_type = responseJson['token_type']
-        token.scope = responseJson['scope']
-        token.access_token = token.token_type + \
-            " " + responseJson['access_token']
-        token.expires_in = token.created + \
-            timedelta(seconds=responseJson['expires_in'])
-        self.Token = token
-
-
-class Token:
-    def __init__(self):
-        self.access_token: str
-        self.expires_in: float
-        self.token_type: str
-        self.scope: str
-        self.created: datetime
-
-    def __repr__(self):
-        return "Access token: %s, Created on: %s, Expires in: %s, Token Type: %s, Scope: %s  " % (self.access_token, self.created, self.expires_in, self.token_type, self.scope)
+import requests
+import json
+from datetime import datetime, time, timedelta
+from one_py_sdk.shared.helpers.protobufhelper import DeserializeResponse
+from one_interfaces import user_pb2 as User
+from one_interfaces import role_pb2 as role
+
+import google
+
+
+class AuthenticationApi:
+    def __init__(self, env, session: requests.Session = None ):
+        self.Environment = env
+        self.Token = Token()
+        self.UserName = ""
+        self.Password = ""
+        self.User: User = User.User()
+        self.IsAuthenticated = False
+        if not session:
+            self.Session = requests.Session()
+            self.Session.headers = {"Content-Type": "application/x-protobuf", "Accept": "application/x-protobuf"}            
+        else:
+            self.Session = session
+
+    def GetToken(self, user, password):
+        data = {'username': user, 'password': password, 'grant_type': 'password', 'scope': 'FFAccessAPI openid',
+                'client_id': 'VSTestClient', 'client_secret': '0CCBB786-9412-4088-BC16-78D3A10158B7'}
+        headers = {'Accept': 'application/json',
+                   'Content-Type': 'application/x-www-form-urlencoded'}
+        url = self.Environment+"/connect/token"
+        response = requests.post(url, headers=headers, data=data)
+        if (response.status_code != 200):
+            return ''
+        self.__setToken(response)
+        self.IsAuthenticated = True
+        self.UserName = user
+        self.Password = password
+        self.Session.headers.update({'Authorization': self.Token.access_token})
+        return self.Token.access_token
+
+    def GetUserInfo(self):
+        headers = {'Accept': 'application/json',
+                   "Authorization": self.Token.access_token}
+        url = self.Environment+"/connect/userinfo"
+        response = requests.get(url, headers=headers)
+        self.__setInfo(response)
+        return response.content
+
+    def LoginResourceOwner(self, userName, password):
+        data = {'username': userName, 'password': password, 'grant_type': 'password', 'scope': 'FFAccessAPI openid',
+                'client_id': 'VSTestClient', 'client_secret': '0CCBB786-9412-4088-BC16-78D3A10158B7'}
+        headers = {'Accept': 'application/json',
+                   'Content-Type': 'application/x-www-form-urlencoded'}
+        url = self.Environment+"/connect/token"
+        response = requests.post(url, headers=headers, data=data)
+        if (response.status_code != 200):
+            return False
+        self.__setToken(response)
+        self.IsAuthenticated = True
+        self.UserName = userName
+        self.Password = password
+        self.Session.headers.update({'Authorization': self.Token.access_token})
+        return True
+
+    def Logout(self):
+        headers = {'Accept': 'application/json',
+                   "Authorization": self.Token.access_token}
+        url = self.Environment+"/account/logout"
+        requests.post(url, headers=headers)
+        self.Token = Token()
+        self.UserName = ""
+        self.Password = ""
+        self.User: User = User.User()
+        self.IsAuthenticated = False
+
+    def __setInfo(self, response):
+        jResponse = json.loads(response.content)
+        self.User.firstName.value = jResponse.get('given_name')
+        self.User.lastName.value = jResponse.get('family_name')
+        self.User.userName = jResponse.get('user_name')
+        self.User.email.value = jResponse.get('email')
+        self.User.tenantId = jResponse.get('ActiveTenantId')
+        self.User.id = jResponse.get('sub')
+
+    def __setToken(self, tokenResponse):
+        token = Token()
+        token.created = datetime.now()
+        responseJson = json.loads(tokenResponse.content)
+        self.IsAuthenticated = True
+        token.token_type = responseJson['token_type']
+        token.scope = responseJson['scope']
+        token.access_token = token.token_type + \
+            " " + responseJson['access_token']
+        token.expires_in = token.created + \
+            timedelta(seconds=responseJson['expires_in'])
+        self.Token = token
+
+
+class Token:
+    def __init__(self):
+        self.access_token: str
+        self.expires_in: float
+        self.token_type: str
+        self.scope: str
+        self.created: datetime
+
+    def __repr__(self):
+        return "Access token: %s, Created on: %s, Expires in: %s, Token Type: %s, Scope: %s  " % (self.access_token, self.created, self.expires_in, self.token_type, self.scope)
```

### Comparing `one_py_sdk-1.5.2/src/one_py_sdk/enterprise/core.py` & `one_py_sdk-1.5.3/src/one_py_sdk/enterprise/core.py`

 * *Files identical despite different names*

### Comparing `one_py_sdk-1.5.2/src/one_py_sdk/enterprise/report.py` & `one_py_sdk-1.5.3/src/one_py_sdk/enterprise/report.py`

 * *Files identical despite different names*

### Comparing `one_py_sdk-1.5.2/src/one_py_sdk/enterprise/twin.py` & `one_py_sdk-1.5.3/src/one_py_sdk/enterprise/twin.py`

 * *Files identical despite different names*

### Comparing `one_py_sdk-1.5.2/src/one_py_sdk/historian/data.py` & `one_py_sdk-1.5.3/src/one_py_sdk/historian/data.py`

 * *Files identical despite different names*

### Comparing `one_py_sdk-1.5.2/src/one_py_sdk/operations/spreadsheet.py` & `one_py_sdk-1.5.3/src/one_py_sdk/operations/spreadsheet.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
     def SaveRows(self, plantId, wsType, rows):
         url = f"{self.Environment}{self.AppUrl}{plantId}/worksheet/{str(wsType)}/rows"
         response = DeserializeResponse(self.Session.post(
             url, data=rows.SerializeToString()))
         return response
 
-    def __rowBuilder(self, valueDict: dict[datetime: [DataPoint]], wsType, plantId):
+    def __rowBuilder(self, valueDict, wsType, plantId):
         r = row.Rows()
         spreadsheetDef = self.GetSpreadsheetDefinition(plantId)
         sortedValueDict = OrderedDict(valueDict.items())
         map = self.MapColumnGuidToIntId(plantId, wsType)
         rowNumbers = []
         for key in valueDict.keys():
             rowNumber = GetRowNumber(key, wsType)
```

### Comparing `one_py_sdk-1.5.2/src/one_py_sdk/shared/helpers/csvhelper.py` & `one_py_sdk-1.5.3/src/one_py_sdk/shared/helpers/csvhelper.py`

 * *Files identical despite different names*

### Comparing `one_py_sdk-1.5.2/src/one_py_sdk/shared/helpers/datetimehelper.py` & `one_py_sdk-1.5.3/src/one_py_sdk/shared/helpers/datetimehelper.py`

 * *Files identical despite different names*

### Comparing `one_py_sdk-1.5.2/src/one_py_sdk/shared/helpers/protobufhelper.py` & `one_py_sdk-1.5.3/src/one_py_sdk/shared/helpers/protobufhelper.py`

 * *Files identical despite different names*

### Comparing `one_py_sdk-1.5.2/src/one_py_sdk/shared/models/datapoint.py` & `one_py_sdk-1.5.3/src/one_py_sdk/shared/models/datapoint.py`

 * *Files identical despite different names*

### Comparing `one_py_sdk-1.5.2/src/one_py_sdk.egg-info/PKG-INFO` & `one_py_sdk-1.5.3/src/one_py_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: one-py-sdk
-Version: 1.5.2
+Version: 1.5.3
 Summary: A package to interact with the ONE waterquality platform APIs.
 Author-email: AquaticInformatics <daniel.edwards@aquaticinformatics.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `one_py_sdk-1.5.2/src/one_py_sdk.egg-info/SOURCES.txt` & `one_py_sdk-1.5.3/src/one_py_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

