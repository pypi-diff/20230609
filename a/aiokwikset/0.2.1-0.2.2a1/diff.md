# Comparing `tmp/aiokwikset-0.2.1.tar.gz` & `tmp/aiokwikset-0.2.2a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiokwikset-0.2.1.tar", last modified: Sat Dec 10 02:06:17 2022, max compression
+gzip compressed data, was "aiokwikset-0.2.2a1.tar", last modified: Fri Jun  9 01:58:35 2023, max compression
```

## Comparing `aiokwikset-0.2.1.tar` & `aiokwikset-0.2.2a1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 02:06:17.111308 aiokwikset-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2022-12-10 02:06:07.000000 aiokwikset-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2022-12-10 02:06:17.111308 aiokwikset-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2022-12-10 02:06:07.000000 aiokwikset-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 02:06:17.111308 aiokwikset-0.2.1/aiokwikset/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2022-12-10 02:06:07.000000 aiokwikset-0.2.1/aiokwikset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9939 2022-12-10 02:06:07.000000 aiokwikset-0.2.1/aiokwikset/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11279 2022-12-10 02:06:07.000000 aiokwikset-0.2.1/aiokwikset/aws_kwikset.py
--rw-r--r--   0 runner    (1001) docker     (123)    23662 2022-12-10 02:06:07.000000 aiokwikset-0.2.1/aiokwikset/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      799 2022-12-10 02:06:07.000000 aiokwikset-0.2.1/aiokwikset/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2022-12-10 02:06:07.000000 aiokwikset-0.2.1/aiokwikset/device.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2022-12-10 02:06:07.000000 aiokwikset-0.2.1/aiokwikset/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2022-12-10 02:06:07.000000 aiokwikset-0.2.1/aiokwikset/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2022-12-10 02:06:07.000000 aiokwikset-0.2.1/aiokwikset/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 02:06:17.111308 aiokwikset-0.2.1/aiokwikset.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2022-12-10 02:06:17.000000 aiokwikset-0.2.1/aiokwikset.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      418 2022-12-10 02:06:17.000000 aiokwikset-0.2.1/aiokwikset.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-10 02:06:17.000000 aiokwikset-0.2.1/aiokwikset.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2022-12-10 02:06:17.000000 aiokwikset-0.2.1/aiokwikset.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2022-12-10 02:06:17.000000 aiokwikset-0.2.1/aiokwikset.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-10 02:06:16.000000 aiokwikset-0.2.1/aiokwikset.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-10 02:06:17.111308 aiokwikset-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2022-12-10 02:06:07.000000 aiokwikset-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:58:35.364709 aiokwikset-0.2.2a1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-09 01:58:23.000000 aiokwikset-0.2.2a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-06-09 01:58:35.364709 aiokwikset-0.2.2a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-06-09 01:58:23.000000 aiokwikset-0.2.2a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:58:35.364709 aiokwikset-0.2.2a1/aiokwikset/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-09 01:58:23.000000 aiokwikset-0.2.2a1/aiokwikset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11134 2023-06-09 01:58:23.000000 aiokwikset-0.2.2a1/aiokwikset/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11916 2023-06-09 01:58:23.000000 aiokwikset-0.2.2a1/aiokwikset/aws_kwikset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23662 2023-06-09 01:58:23.000000 aiokwikset-0.2.2a1/aiokwikset/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-06-09 01:58:23.000000 aiokwikset-0.2.2a1/aiokwikset/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-06-09 01:58:23.000000 aiokwikset-0.2.2a1/aiokwikset/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-09 01:58:23.000000 aiokwikset-0.2.2a1/aiokwikset/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-09 01:58:23.000000 aiokwikset-0.2.2a1/aiokwikset/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-09 01:58:23.000000 aiokwikset-0.2.2a1/aiokwikset/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:58:35.364709 aiokwikset-0.2.2a1/aiokwikset.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-06-09 01:58:35.000000 aiokwikset-0.2.2a1/aiokwikset.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-09 01:58:35.000000 aiokwikset-0.2.2a1/aiokwikset.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 01:58:35.000000 aiokwikset-0.2.2a1/aiokwikset.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-09 01:58:35.000000 aiokwikset-0.2.2a1/aiokwikset.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-09 01:58:35.000000 aiokwikset-0.2.2a1/aiokwikset.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 01:58:35.000000 aiokwikset-0.2.2a1/aiokwikset.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 01:58:35.364709 aiokwikset-0.2.2a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-09 01:58:23.000000 aiokwikset-0.2.2a1/setup.py
```

### Comparing `aiokwikset-0.2.1/LICENSE` & `aiokwikset-0.2.2a1/LICENSE`

 * *Files identical despite different names*

### Comparing `aiokwikset-0.2.1/PKG-INFO` & `aiokwikset-0.2.2a1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiokwikset
-Version: 0.2.1
+Version: 0.2.2a1
 Summary: Python interface for Kwikset Smart Locks
 Home-page: https://github.com/explosivo22/aiokwikset
 Author: Brad Barbour
 Author-email: barbourbj@gmail.com
 License: Apache Software License
 Keywords: kwikset,home automation,kwikset halo,kwikset smart lock
 Classifier: Programming Language :: Python :: 3
```

### Comparing `aiokwikset-0.2.1/README.md` & `aiokwikset-0.2.2a1/README.md`

 * *Files identical despite different names*

### Comparing `aiokwikset-0.2.1/aiokwikset/api.py` & `aiokwikset-0.2.2a1/aiokwikset/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import json
 import aioboto3
+import botocore.exceptions
 import attr
 import datetime
 
 from typing import Optional
 from envs import env
 from jose import jwt, JWTError
 from urllib.parse import urlparse
@@ -13,15 +14,15 @@
     ClientError, 
     ClientResponseError, 
     ClientConnectorError, 
     ServerConnectionError, 
     ClientPayloadError
 )
 
-from .errors import RequestError
+from .errors import RequestError, NotAuthorized
 from .device import Device
 from .user import User
 from .exceptions import TokenVerificationException
 
 from aiokwikset.aws_kwikset import AWSKWIKSET
 from aiokwikset.const import (
     LOGGER,
@@ -165,15 +166,15 @@
         the tokens by calling the renew_access_tokens method or does nothing
         :param renew: bool indicating whether to refresh on expiration
         :return: bool indicating whether access_token has expired
         """
         if not self.access_token:
             raise AttributeError('Access Token Required to Check Token')
         now = datetime.datetime.now()
-        dec_access_token = jwt.get_unverified_claims(self.access_token)
+        dec_access_token = jwt.get_unverified_claims(self.id_token)
 
         if now > datetime.datetime.fromtimestamp(dec_access_token['exp']):
             expired = True
             if renew:
                 await self.renew_access_token()
         else:
             expired = False
@@ -181,20 +182,21 @@
 
     async def renew_access_token(self):
         """
         Sets a new access token on the User using the refresh token.
         """
         auth_params = {'SECRET_HASH': '', 'REFRESH_TOKEN': self.refresh_token}
 
-        async with self.get_client() as client:
-            refresh_response = await client.initiate_auth(
-                ClientId=self.client_id,
-                AuthFlow='REFRESH_TOKEN_AUTH',
-                AuthParameters=auth_params,
-            )
+        try:
+            async with self.get_client() as client:
+                refresh_response = await client.initiate_auth(
+                    ClientId=self.client_id,
+                    AuthFlow='REFRESH_TOKEN_AUTH',
+                    AuthParameters=auth_params,
+                )
 
             self._set_attributes(
                 refresh_response,
                 {
                     'access_token':
                     refresh_response['AuthenticationResult']['AccessToken'],
                     'id_token':
@@ -205,14 +207,19 @@
             )
 
             if not self.device:
                 self.device = Device(self._request)
 
             if not self.user:
                 self.user = User(self._request)
+        
+        #attempt to catch the NotAuthorizedException
+        except botocore.exceptions.ClientError as err:
+            if err.response['Error']['Code'] == 'NotAuthorizedException':
+                raise NotAuthorized("Refresh Token has been revoked.")
 
     def _set_attributes(self, response, attribute_dict):
         """
         Set user attributes based on response code
         :param response: HTTP response from Cognito
         :attribute dict: Dictionary of attribute name and values
         """
@@ -235,14 +242,34 @@
                      pool_id=self.user_pool_id,
                      client_id=self.client_id, client=self.get_client(),
                      client_secret=self.client_secret)
 
         self.code_type = code_type
 
         pre_verification = await self.aws.authenticate_user()
+
+        if pre_verification.get('AuthenticationResult'):
+            print("2-step verification disabled")
+            await self.verify_token(pre_verification['AuthenticationResult']['IdToken'],
+                                    'id_token', 'id')
+            self.refresh_token = pre_verification['AuthenticationResult']['RefreshToken']
+            await self.verify_token(pre_verification['AuthenticationResult']['AccessToken'],
+                                    'access_token', 'access')
+            self.token_type = pre_verification['AuthenticationResult']['TokenType']
+
+            if not self.device:
+                self.device = Device(self._request)
+
+            if not self.user:
+                self.user = User(self._request)
+            
+            return
+        
+        print("2-step verification enabled")
+
         return pre_verification
 
     async def verify_user(self, pre_verification, code):
         challenge_responses = {'ANSWER': 'answerType:verifyCode,medium:{},codeType:login,code:{}'.format(self.code_type, code),"USERNAME": self.username}
 
         async with self.get_client() as client:
             tokens = await client.respond_to_auth_challenge(
```

### Comparing `aiokwikset-0.2.1/aiokwikset/aws_kwikset.py` & `aiokwikset-0.2.2a1/aiokwikset/aws_kwikset.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,20 @@
 import binascii
 import datetime
 import hashlib
 import hmac
 import re
 
 import aioboto3
+import botocore.exceptions
 import os
 import six
 
+from .errors import NotAuthorized
+
 # https://github.com/aws/amazon-cognito-identity-js/blob/master/src/AuthenticationHelper.js#L22
 n_hex = 'FFFFFFFFFFFFFFFFC90FDAA22168C234C4C6628B80DC1CD1' + \
         '29024E088A67CC74020BBEA63B139B22514A08798E3404DD' + \
         'EF9519B3CD3A431B302B0A6DF25F14374FE1356D6D51C245' + \
         'E485B576625E7EC6F44C42E9A637ED6B0BFF5CB6F406B7ED' + \
         'EE386BFB5A899FA5AE9F24117C4B1FE649286651ECE45B3D' + \
         'C2007CB8A163BF0598DA48361C55D39A69163FA8FD24CF5F' + \
@@ -236,39 +239,48 @@
 
         return response
 
     async def authenticate_user(self, client=None):
         boto_client = self.client or client
         auth_params = self.get_auth_params()
 
-        async with boto_client as client:
-            response = await client.initiate_auth(
-                AuthFlow='CUSTOM_AUTH',
-                AuthParameters=auth_params,
-                ClientId=self.client_id
-            )
-            if response['ChallengeName'] == self.PASSWORD_VERIFIER_CHALLENGE:
-                challenge_response = self.process_challenge(
-                    response['ChallengeParameters'])
-
-                custom_challenge = await client.respond_to_auth_challenge(
-                    ClientId=self.client_id,
-                    ChallengeName=self.PASSWORD_VERIFIER_CHALLENGE,
-                    Session=response['Session'],
-                    ChallengeResponses=challenge_response)
-
-                if custom_challenge['ChallengeName'] == self.CUSTOM_VERIFIER_CHALLENGE:
-                    custom_challenge_response = self.process_custom_challenge()
+        try:
+            async with boto_client as client:
+                response = await client.initiate_auth(
+                    AuthFlow='CUSTOM_AUTH',
+                    AuthParameters=auth_params,
+                    ClientId=self.client_id
+                )
+                if response['ChallengeName'] == self.PASSWORD_VERIFIER_CHALLENGE:
+                    challenge_response = self.process_challenge(
+                        response['ChallengeParameters'])
 
-                    custom_challenge_code = await client.respond_to_auth_challenge(
+                    custom_challenge = await client.respond_to_auth_challenge(
                         ClientId=self.client_id,
-                        ChallengeName=self.CUSTOM_VERIFIER_CHALLENGE,
-                        Session=custom_challenge['Session'],
-                        ChallengeResponses=custom_challenge_response)
-
-                    return custom_challenge_code
+                        ChallengeName=self.PASSWORD_VERIFIER_CHALLENGE,
+                        Session=response['Session'],
+                        ChallengeResponses=challenge_response)
+                    
+                    #2-step verification is disabled
+                    if custom_challenge.get('AuthenticationResult'):
+                        return custom_challenge
+
+                    #2-step verification is enabled
+                    if custom_challenge['ChallengeName'] == self.CUSTOM_VERIFIER_CHALLENGE:
+                        custom_challenge_response = self.process_custom_challenge()
+
+                        custom_challenge_code = await client.respond_to_auth_challenge(
+                            ClientId=self.client_id,
+                            ChallengeName=self.CUSTOM_VERIFIER_CHALLENGE,
+                            Session=custom_challenge['Session'],
+                            ChallengeResponses=custom_challenge_response)
+
+                        return custom_challenge_code
+                    else:
+                        raise NotImplementedError('The %s challenge is not supported'
+                                            % response['ChallengeName'])
                 else:
                     raise NotImplementedError('The %s challenge is not supported'
-                                          % response['ChallengeName'])
-            else:
-                raise NotImplementedError('The %s challenge is not supported'
-                                          % response['ChallengeName'])
+                                            % response['ChallengeName'])
+        except botocore.exceptions.ClientError as err:
+            if err.response['Error']['Code'] == 'NotAuthorizedException':
+                raise NotAuthorized("Refresh Token has been revoked")
```

### Comparing `aiokwikset-0.2.1/aiokwikset/client.py` & `aiokwikset-0.2.2a1/aiokwikset/client.py`

 * *Files identical despite different names*

### Comparing `aiokwikset-0.2.1/aiokwikset/const.py` & `aiokwikset-0.2.2a1/aiokwikset/const.py`

 * *Files identical despite different names*

### Comparing `aiokwikset-0.2.1/aiokwikset/device.py` & `aiokwikset-0.2.2a1/aiokwikset/device.py`

 * *Files identical despite different names*

### Comparing `aiokwikset-0.2.1/aiokwikset/user.py` & `aiokwikset-0.2.2a1/aiokwikset/user.py`

 * *Files identical despite different names*

### Comparing `aiokwikset-0.2.1/aiokwikset.egg-info/PKG-INFO` & `aiokwikset-0.2.2a1/aiokwikset.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiokwikset
-Version: 0.2.1
+Version: 0.2.2a1
 Summary: Python interface for Kwikset Smart Locks
 Home-page: https://github.com/explosivo22/aiokwikset
 Author: Brad Barbour
 Author-email: barbourbj@gmail.com
 License: Apache Software License
 Keywords: kwikset,home automation,kwikset halo,kwikset smart lock
 Classifier: Programming Language :: Python :: 3
```

### Comparing `aiokwikset-0.2.1/setup.py` & `aiokwikset-0.2.2a1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     with io.open(os.path.join(here, 'README.md'), encoding='utf-8') as f:
         long_description = '\n' + f.read()
 except FileNotFoundError:
     long_description = DESCRIPTION
 
 setup(
     name="aiokwikset",
-    version="0.2.1",
+    version="0.2.2a1",
     description="Python interface for Kwikset Smart Locks",
     long_description=long_description,
     long_description_content_type='text/markdown',
     url="https://github.com/explosivo22/aiokwikset",
     author="Brad Barbour",
     author_email="barbourbj@gmail.com",
     license='Apache Software License',
```

