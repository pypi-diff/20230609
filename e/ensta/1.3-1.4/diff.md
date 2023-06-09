# Comparing `tmp/ensta-1.3.tar.gz` & `tmp/ensta-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ensta-1.3.tar", last modified: Fri Jun  9 06:02:31 2023, max compression
+gzip compressed data, was "ensta-1.4.tar", last modified: Fri Jun  9 09:29:00 2023, max compression
```

## Comparing `ensta-1.3.tar` & `ensta-1.4.tar`

### file list

```diff
@@ -1,29 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 06:02:31.946511 ensta-1.3/
--rw-rw-rw-   0        0        0     1081 2023-06-06 15:38:39.000000 ensta-1.3/LICENSE.txt
--rw-rw-rw-   0        0        0     3368 2023-06-09 06:02:31.946511 ensta-1.3/PKG-INFO
--rw-rw-rw-   0        0        0     2646 2023-06-08 05:38:39.000000 ensta-1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-09 06:02:31.899098 ensta-1.3/ensta/
--rw-rw-rw-   0        0        0    13915 2023-06-09 05:58:06.000000 ensta-1.3/ensta/Guest.py
--rw-rw-rw-   0        0        0    20272 2023-06-08 13:08:53.000000 ensta-1.3/ensta/Host.py
--rw-rw-rw-   0        0        0       60 2023-06-09 05:22:01.000000 ensta-1.3/ensta/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-09 06:02:31.914723 ensta-1.3/ensta/containers/
--rw-rw-rw-   0        0        0      295 2023-06-08 11:36:12.000000 ensta-1.3/ensta/containers/FollowListPerson.py
--rw-rw-rw-   0        0        0      611 2023-06-09 05:50:34.000000 ensta-1.3/ensta/containers/Profile.py
--rw-rw-rw-   0        0        0       78 2023-06-08 12:24:32.000000 ensta-1.3/ensta/containers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-09 06:02:31.930629 ensta-1.3/ensta/lib/
--rw-rw-rw-   0        0        0     1169 2023-06-07 07:34:14.000000 ensta-1.3/ensta/lib/Commons.py
--rw-rw-rw-   0        0        0      327 2023-06-08 11:55:00.000000 ensta-1.3/ensta/lib/Exceptions.py
--rw-rw-rw-   0        0        0      219 2023-06-08 12:02:31.000000 ensta-1.3/ensta/lib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-09 06:02:31.946511 ensta-1.3/ensta/responses/
--rw-rw-rw-   0        0        0      248 2023-06-08 11:36:12.000000 ensta-1.3/ensta/responses/FollowPersonListResponse.py
--rw-rw-rw-   0        0        0      345 2023-06-08 11:34:29.000000 ensta-1.3/ensta/responses/FollowPersonResponse.py
--rw-rw-rw-   0        0        0      192 2023-06-08 11:32:43.000000 ensta-1.3/ensta/responses/UnfollowPersonResponse.py
--rw-rw-rw-   0        0        0      180 2023-06-09 05:51:00.000000 ensta-1.3/ensta/responses/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-09 06:02:31.914723 ensta-1.3/ensta.egg-info/
--rw-rw-rw-   0        0        0     3368 2023-06-09 06:02:31.000000 ensta-1.3/ensta.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      546 2023-06-09 06:02:31.000000 ensta-1.3/ensta.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 06:02:31.000000 ensta-1.3/ensta.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-09 06:02:31.000000 ensta-1.3/ensta.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-09 06:02:31.000000 ensta-1.3/ensta.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-09 06:02:31.946511 ensta-1.3/setup.cfg
--rw-rw-rw-   0        0        0     1071 2023-06-09 05:25:09.000000 ensta-1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 09:29:00.500176 ensta-1.4/
+-rw-rw-rw-   0        0        0     1081 2023-06-06 15:38:39.000000 ensta-1.4/LICENSE.txt
+-rw-rw-rw-   0        0        0     3368 2023-06-09 09:29:00.500176 ensta-1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2646 2023-06-08 05:38:39.000000 ensta-1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-09 09:29:00.453258 ensta-1.4/ensta/
+-rw-rw-rw-   0        0        0    11420 2023-06-09 09:07:44.000000 ensta-1.4/ensta/Guest.py
+-rw-rw-rw-   0        0        0    19816 2023-06-09 09:23:24.000000 ensta-1.4/ensta/Host.py
+-rw-rw-rw-   0        0        0       60 2023-06-09 05:22:01.000000 ensta-1.4/ensta/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 09:29:00.500176 ensta-1.4/ensta/containers/
+-rw-rw-rw-   0        0        0      347 2023-06-09 08:53:51.000000 ensta-1.4/ensta/containers/FollowPerson.py
+-rw-rw-rw-   0        0        0      222 2023-06-09 08:46:48.000000 ensta-1.4/ensta/containers/FollowedStatus.py
+-rw-rw-rw-   0        0        0      584 2023-06-09 07:33:57.000000 ensta-1.4/ensta/containers/Profile.py
+-rw-rw-rw-   0        0        0      153 2023-06-09 08:28:13.000000 ensta-1.4/ensta/containers/UnfollowedStatus.py
+-rw-rw-rw-   0        0        0      162 2023-06-09 08:48:05.000000 ensta-1.4/ensta/containers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 09:29:00.500176 ensta-1.4/ensta/lib/
+-rw-rw-rw-   0        0        0     1424 2023-06-09 09:01:13.000000 ensta-1.4/ensta/lib/Commons.py
+-rw-rw-rw-   0        0        0      616 2023-06-09 09:10:35.000000 ensta-1.4/ensta/lib/Exceptions.py
+-rw-rw-rw-   0        0        0      298 2023-06-09 09:10:42.000000 ensta-1.4/ensta/lib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 09:29:00.468789 ensta-1.4/ensta.egg-info/
+-rw-rw-rw-   0        0        0     3368 2023-06-09 09:29:00.000000 ensta-1.4/ensta.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      460 2023-06-09 09:29:00.000000 ensta-1.4/ensta.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 09:29:00.000000 ensta-1.4/ensta.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-09 09:29:00.000000 ensta-1.4/ensta.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-09 09:29:00.000000 ensta-1.4/ensta.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-09 09:29:00.500176 ensta-1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1052 2023-06-09 09:28:43.000000 ensta-1.4/setup.py
```

### Comparing `ensta-1.3/LICENSE.txt` & `ensta-1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ensta-1.3/PKG-INFO` & `ensta-1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: ensta
-Version: 1.3
+Version: 1.4
 Summary: Simple & Up-to-date Instagram API
 Home-page: https://github.com/diezo/ensta
-Download-URL: https://github.com/diezo/ensta/archive/refs/tags/v1.3.tar.gz
+Download-URL: https://github.com/diezo/ensta/archive/refs/tags/v1.4.tar.gz
 Author: Deepak Soni
 Author-email: lonelycube@proton.me
 License: MIT
 Keywords: instagram,web,private,api,scraper,easy,download,upload
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `ensta-1.3/README.md` & `ensta-1.4/README.md`

 * *Files identical despite different names*

### Comparing `ensta-1.3/ensta/Guest.py` & `ensta-1.4/ensta/Guest.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,47 +1,54 @@
 from json import JSONDecodeError
 import random
-import string
 import requests
 from .lib.Commons import (
     update_session,
     update_homepage_source,
     update_app_id,
-    refresh_csrf_token
+    refresh_csrf_token,
+    format_username,
+    format_uid
 )
-from .lib import IdentifierError
 from .containers.Profile import Profile
 
 
 class Guest:
     request_session: requests.Session = None
     homepage_source: str = None
     insta_app_id: str = None
     csrf_token: str = None
 
-    def __init__(self):
+    def __init__(self, homepage_source: str = None, insta_app_id: str = None) -> None:
         update_session(self)
-        update_homepage_source(self)
-        update_app_id(self)
 
-    def username_availability(self, username: str):
-        username = username.strip().lower().replace(" ", "")
+        if homepage_source is not None:
+            self.homepage_source = homepage_source
+        else:
+            update_homepage_source(self)
+
+        if insta_app_id is not None:
+            self.insta_app_id = insta_app_id
+        else:
+            update_app_id(self)
+
+    def username_availability(self, username: str) -> bool | None:
+        username = format_username(username)
         refresh_csrf_token(self)
-        preferred_color_scheme = random.choice(["light", "dark"])
         body_json = {
             "email": f"{username}@{self.csrf_token}.com",
             "username": username,
             "first_name": username.capitalize(),
             "opt_into_one_tap": False
         }
         request_headers = {
             "accept": "*/*",
             "accept-language": "en-US,en;q=0.9",
             "content-type": "application/x-www-form-urlencoded",
-            "sec-ch-prefers-color-scheme": preferred_color_scheme,
+            "sec-ch-prefers-color-scheme": random.choice(["light", "dark"]),
             "sec-ch-ua": "\"Not.A/Brand\";v=\"8\", \"Chromium\";v=\"114\", \"Google Chrome\";v=\"114\"",
             "sec-ch-ua-full-version-list": "\"Not.A/Brand\";v=\"8.0.0.0\", \"Chromium\";v=\"114.0.5735.91\", \"Google Chrome\";v=\"114.0.5735.91\"",
             "sec-ch-ua-mobile": "?0",
             "sec-ch-ua-platform": "\"Windows\"",
             "sec-ch-ua-platform-version": "\"15.0.0\"",
             "sec-fetch-dest": "empty",
             "sec-fetch-mode": "cors",
@@ -54,68 +61,54 @@
             "x-instagram-ajax": "1007614758",
             "x-requested-with": "XMLHttpRequest",
             "Referer": "https://www.instagram.com/accounts/emailsignup/",
             "Referrer-Policy": "strict-origin-when-cross-origin"
         }
 
         try:
-            http_response = self.request_session.post(
-                "https://www.instagram.com/api/v1/web/accounts/web_create_ajax/attempt/", headers=request_headers,
-                data=body_json)
+            http_response = self.request_session.post("https://www.instagram.com/api/v1/web/accounts/web_create_ajax/attempt/", headers=request_headers, data=body_json)
             response_json = http_response.json()
 
             if "errors" in response_json:
-
-                username_suggestions = []
-                if "username_suggestions" in response_json:
-                    username_suggestions = response_json["username_suggestions"]
-
-                if "username" in response_json["errors"]:
-                    return {"success": True, "available": False, "suggestions": username_suggestions}
-                else:
-                    return {"success": True, "available": True, "suggestions": username_suggestions}
-            else:
-                return {"success": False, "available": None, "suggestions": []}
+                return "username" not in response_json["errors"]
         except JSONDecodeError:
-            return {"success": False, "available": None, "suggestions": []}
+            return None
 
-    def profile(self, identifier: str | int, iu: bool = False):
+    def profile(self, username: str) -> Profile:
+        username = format_username(username)
         failure_response = Profile()
-        if not iu:
-            conversion_success, identifier = self.identifier_conversion(identifier, 0)
-            if not conversion_success: return failure_response
 
         refresh_csrf_token(self)
-        preferred_color_scheme = random.choice(["light", "dark"])
         request_headers = {
             "accept": "*/*",
             "accept-language": "en-US,en;q=0.9",
-            "sec-ch-prefers-color-scheme": preferred_color_scheme,
+            "sec-ch-prefers-color-scheme": random.choice(["light", "dark"]),
             "sec-ch-ua": "\"Not.A/Brand\";v=\"8\", \"Chromium\";v=\"114\", \"Google Chrome\";v=\"114\"",
             "sec-ch-ua-full-version-list": "\"Not.A/Brand\";v=\"8.0.0.0\", \"Chromium\";v=\"114.0.5735.91\", \"Google Chrome\";v=\"114.0.5735.91\"",
             "sec-ch-ua-mobile": "?0",
             "sec-ch-ua-platform": "\"Windows\"",
             "sec-ch-ua-platform-version": "\"15.0.0\"",
             "sec-fetch-dest": "empty",
             "sec-fetch-mode": "cors",
             "sec-fetch-site": "same-origin",
             "viewport-width": "1475",
             "x-asbd-id": "198387",
             "x-csrftoken": self.csrf_token,
             "x-ig-app-id": self.insta_app_id,
             "x-ig-www-claim": "0",
             "x-requested-with": "XMLHttpRequest",
-            "Referer": f"https://www.instagram.com/{identifier}/",
+            "Referer": f"https://www.instagram.com/{username}/",
             "Referrer-Policy": "strict-origin-when-cross-origin"
         }
 
         try:
             http_response = self.request_session.get(
-                f"https://www.instagram.com/api/v1/users/web_profile_info/?username={identifier}",
-                headers=request_headers)
+                f"https://www.instagram.com/api/v1/users/web_profile_info/?username={username}",
+                headers=request_headers
+            )
             response_json = http_response.json()
 
             if "status" in response_json:
                 if response_json["status"] == "ok" and "data" in response_json:
                     if "user" in response_json["data"]:
 
                         profile_object_biography = None
@@ -181,16 +174,15 @@
 
                         if "pronouns" in response_json["data"]["user"]:
                             user_pronouns = []
                             for pronoun in response_json["data"]["user"]["pronouns"]:
                                 user_pronouns.append(pronoun)
                             profile_object_pronouns = user_pronouns
 
-                        return Profile(success=True,
-                                       biography=profile_object_biography,
+                        return Profile(biography=profile_object_biography,
                                        country_block=profile_object_country_block,
                                        full_name=profile_object_full_name,
                                        follower_count=profile_object_follower_count,
                                        following_count=profile_object_following_count,
                                        user_id=profile_object_user_id,
                                        is_business_account=profile_object_is_business_account,
                                        is_professional_account=profile_object_is_professional_account,
@@ -207,77 +199,30 @@
                 else:
                     return failure_response
             else:
                 return failure_response
         except JSONDecodeError:
             return failure_response
 
-    def get_userid(self, username: str):
+    def get_uid(self, username: str) -> str | None:
         username = username.strip().lower().replace(" ", "")
-        response = self.profile(username, iu=True)
+        response = self.profile(username)
 
-        if response.success:
-            if response.user_id is not None:
-                return {"success": True, "user_id": str(response.user_id).strip()}
-            else:
-                return {"success": False, "user_id": ""}
-        else:
-            return {"success": False, "user_id": ""}
+        if response.user_id is not None:
+            return format_uid(response.user_id)
 
-    def get_username(self, user_id: str | int):
-        user_id = str(user_id).strip()
+    def get_username(self, uid: str | int) -> str | None:
+        uid = format_uid(uid)
+        refresh_csrf_token(self)
         request_headers = {
             "User-Agent": "Instagram 76.0.0.15.395 Android (24/7.0; 640dpi; 1440x2560; samsung; SM-G930F; herolte; samsungexynos8890; en_US; 138226743)"
         }
 
         try:
-            http_response = self.request_session.get(f"https://i.instagram.com/api/v1/users/{user_id}/info/",
-                                                     headers=request_headers)
+            http_response = self.request_session.get(f"https://i.instagram.com/api/v1/users/{uid}/info/", headers=request_headers)
             response_json = http_response.json()
 
-            if "status" in response_json:
-                if response_json["status"] == "ok" and "user" in response_json:
-                    if "username" in response_json["user"]:
-                        return {"success": True, "username": response_json["user"]["username"]}
-                    else:
-                        return {"success": False, "username": ""}
-                else:
-                    return {"success": False, "username": ""}
-            else:
-                return {"success": False, "username": ""}
+            if "status" in response_json and response_json["status"] == "ok" and "user" in response_json and "username" in response_json["user"]:
+                return format_username(response_json["user"]["username"])
 
         except JSONDecodeError:
-            return {"success": False, "username": ""}
-
-    def identifier_conversion(self, identifier: str | int, required: str | int):
-        identifier = str(identifier).lower().replace(" ", "")
-        if len(identifier) < 1: raise IdentifierError(
-            "No identifier was given. Please pass either UserId or Username as an argument.")
-
-        # Detect if identifier is Username or UserId
-        is_username = False
-        for letter in identifier:
-            if letter not in string.digits:
-                is_username = True
-                break
-
-        # Generate UserId if identifier is Username
-        if is_username:
-            if required == 0:
-                return True, identifier
-            else:
-                user_id_response = self.get_userid(identifier)
-
-                if user_id_response["success"]:
-                    return True, user_id_response["user_id"]
-                else:
-                    return False, None
-        else:
-            if required == 0:
-                username_response = self.get_username(identifier)
-
-                if username_response["success"]:
-                    return True, username_response["username"]
-                else:
-                    return False, None
-            else:
-                return True, identifier
+            return None
```

### Comparing `ensta-1.3/ensta/Host.py` & `ensta-1.4/ensta/Host.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,57 +3,63 @@
 import random
 import string
 from .Guest import Guest
 from .lib.Commons import (
     refresh_csrf_token,
     update_app_id,
     update_homepage_source,
-    update_session
+    update_session,
+    format_identifier
 )
 from .lib import (
     AuthenticationError,
     NetworkError,
-    IdentifierError
+    IdentifierError,
+    CodeError
 )
-from .containers import FollowListPerson
-from .responses.FollowPersonListResponse import FollowPersonListResponse
-from .responses.FollowPersonResponse import FollowPersonResponse
-from .responses.UnfollowPersonResponse import UnfollowPersonResponse
+from .containers import FollowPerson
+from .containers import (FollowedStatus, UnfollowedStatus)
+
+USERNAME = 0
+UID = 1
 
 
 class Host:
     request_session: requests.Session = None
     homepage_source: str = None
     insta_app_id: str = None
     preferred_color_scheme: str = "dark"
     x_ig_www_claim: str = None
     csrf_token: str = None
     guest: Guest = None
 
-    def __init__(self, session_id: str):
+    def __init__(self, session_id: str) -> None:
         self.x_ig_www_claim = "hmac." + "".join(random.choices(string.ascii_letters + string.digits + "_-", k=48))
         update_session(self)
         update_homepage_source(self)
         update_app_id(self)
-        self.guest = Guest()
+        self.guest = Guest(
+            homepage_source=self.homepage_source,
+            insta_app_id=self.insta_app_id
+        )
 
         self.request_session.cookies.set("sessionid", session_id)
 
         if not self.is_authenticated():
             raise AuthenticationError("Either User ID or Session ID is not valid.")
 
-    def update_homepage_source(self):
+    def update_homepage_source(self) -> None:
         temp_homepage_source = requests.get("https://www.instagram.com/").text.strip()
 
-        if temp_homepage_source != "":
-            self.homepage_source = temp_homepage_source
-        else:
+        if temp_homepage_source == "":
             raise NetworkError("Couldn't load instagram homepage.")
 
-    def is_authenticated(self):
+        self.homepage_source = temp_homepage_source
+
+    def is_authenticated(self) -> bool:
         refresh_csrf_token(self)
         request_headers = {
             "accept": "*/*",
             "accept-language": "en-US,en;q=0.9",
             "sec-ch-prefers-color-scheme": self.preferred_color_scheme,
             "sec-ch-ua": "\"Not.A/Brand\";v=\"8\", \"Chromium\";v=\"114\", \"Google Chrome\";v=\"114\"",
             "sec-ch-ua-full-version-list": "\"Not.A/Brand\";v=\"8.0.0.0\", \"Chromium\";v=\"114.0.5735.91\", \"Google Chrome\";v=\"114.0.5735.91\"",
@@ -76,22 +82,20 @@
 
         try:
             http_response.json()
             return True
         except JSONDecodeError:
             return False
 
-    def follow(self, identifier: str | int):
-        conversion_success, identifier = self.identifier_conversion(identifier, 1)
-        failure_response = FollowPersonResponse()
-        if not conversion_success: return failure_response
+    def follow(self, identifier: str | int) -> FollowedStatus | None:
+        conversion_success, identifier = self.identifier_conversion(identifier, UID)
+        if not conversion_success: return None
 
         # Actual Request
         refresh_csrf_token(self)
-        random_referer_username = "".join(random.choices(string.ascii_lowercase, k=6))
         body_json = {
             "container_module": "profile",
             "nav_chain": f"PolarisProfileRoot:profilePage:1:via_cold_start",
             "user_id": identifier
         }
         request_headers = {
             "accept": "*/*",
@@ -109,49 +113,43 @@
             "viewport-width": "1475",
             "x-asbd-id": "198387",
             "x-csrftoken": self.csrf_token,
             "x-ig-app-id": self.insta_app_id,
             "x-ig-www-claim": self.x_ig_www_claim,
             "x-instagram-ajax": "1007616494",
             "x-requested-with": "XMLHttpRequest",
-            "Referer": f"https://www.instagram.com/{random_referer_username}/",
+            "Referer": f"https://www.instagram.com/{''.join(random.choices(string.ascii_lowercase, k=5))}/",
             "Referrer-Policy": "strict-origin-when-cross-origin"
         }
 
-        http_response = self.request_session.post(f"https://www.instagram.com/api/v1/friendships/create/{identifier}/", headers=request_headers, data=body_json)
-
         try:
+            http_response = self.request_session.post(f"https://www.instagram.com/api/v1/friendships/create/{identifier}/", headers=request_headers, data=body_json)
             response_json = http_response.json()
 
             if "status" in response_json:
                 if response_json["status"] == "ok" and "friendship_status" in response_json:
                     if "following" in response_json["friendship_status"] \
                             and "outgoing_request" in response_json["friendship_status"] \
                             and "followed_by" in response_json["friendship_status"] \
                             and "previous_following" in response_json:
-                        return FollowPersonResponse(
-                            success=True,
+                        return FollowedStatus(
                             following=response_json["friendship_status"]["following"],
                             follow_requested=response_json["friendship_status"]["outgoing_request"],
                             is_my_follower=response_json["friendship_status"]["followed_by"],
                             previous_following=response_json["previous_following"]
                         )
-                    else: return failure_response
-                else: return failure_response
-            else: return failure_response
-        except JSONDecodeError: return failure_response
-
-    def unfollow(self, identifier: str | int):
-        conversion_success, identifier = self.identifier_conversion(identifier, 1)
-        failure_response = UnfollowPersonResponse()
-        if not conversion_success: return failure_response
+        except JSONDecodeError:
+            return None
+
+    def unfollow(self, identifier: str | int) -> UnfollowedStatus | None:
+        conversion_success, identifier = self.identifier_conversion(identifier, UID)
+        if not conversion_success: return None
 
         # Actual Request
         refresh_csrf_token(self)
-        random_referer_username = "".join(random.choices(string.ascii_lowercase, k=6))
         body_json = {
             "container_module": "profile",
             "nav_chain": f"PolarisProfileRoot:profilePage:1:via_cold_start",
             "user_id": identifier
         }
         request_headers = {
             "accept": "*/*",
@@ -169,44 +167,40 @@
             "viewport-width": "1475",
             "x-asbd-id": "198387",
             "x-csrftoken": self.csrf_token,
             "x-ig-app-id": self.insta_app_id,
             "x-ig-www-claim": self.x_ig_www_claim,
             "x-instagram-ajax": "1007616494",
             "x-requested-with": "XMLHttpRequest",
-            "Referer": f"https://www.instagram.com/{random_referer_username}/",
+            "Referer": f"https://www.instagram.com/{''.join(random.choices(string.ascii_lowercase, k=6))}/",
             "Referrer-Policy": "strict-origin-when-cross-origin"
         }
 
-        http_response = self.request_session.post(f"https://www.instagram.com/api/v1/friendships/destroy/{identifier}/", headers=request_headers, data=body_json)
-
         try:
+            http_response = self.request_session.post(f"https://www.instagram.com/api/v1/friendships/destroy/{identifier}/", headers=request_headers, data=body_json)
             response_json = http_response.json()
 
             if "status" in response_json:
                 if response_json["status"] == "ok" and "friendship_status" in response_json:
                     if "following" in response_json["friendship_status"] \
-                            and "outgoing_request" in response_json["friendship_status"]:
-                        return UnfollowPersonResponse(
-                            success=True,
-                            unfollowed=not response_json["friendship_status"]["following"] and not response_json["friendship_status"]["outgoing_request"]
+                            and "outgoing_request" in response_json["friendship_status"] \
+                            and "followed_by" in response_json["friendship_status"]:
+                        return UnfollowedStatus(
+                            unfollowed=not response_json["friendship_status"]["following"] and not response_json["friendship_status"]["outgoing_request"],
+                            is_my_follower=response_json["friendship_status"]["followed_by"]
                         )
-                    else: return failure_response
-                else: return failure_response
-            else: return failure_response
-        except JSONDecodeError: return failure_response
-
-    def follower_list(self, identifier: str | int, count: int):
-        conversion_success, identifier = self.identifier_conversion(identifier, 1)
-        failure_response = FollowPersonListResponse()
-        if not conversion_success: return failure_response
+        except JSONDecodeError:
+            return None
+
+    def follower_list(self, identifier: str | int, count: int = 0) -> list[FollowPerson] | None:
+        conversion_success, identifier = self.identifier_conversion(identifier, UID)
+        if not conversion_success: return None
 
         # Actual Request
         refresh_csrf_token(self)
-        random_referer_username = "".join(random.choices(string.ascii_lowercase, k=6))
         request_headers = {
             "accept": "*/*",
             "accept-language": "en-US,en;q=0.9",
             "sec-ch-prefers-color-scheme": self.preferred_color_scheme,
             "sec-ch-ua": "\"Not.A/Brand\";v=\"8\", \"Chromium\";v=\"114\", \"Google Chrome\";v=\"114\"",
             "sec-ch-ua-full-version-list": "\"Not.A/Brand\";v=\"8.0.0.0\", \"Chromium\";v=\"114.0.5735.91\", \"Google Chrome\";v=\"114.0.5735.91\"",
             "sec-ch-ua-mobile": "?0",
@@ -217,49 +211,53 @@
             "sec-fetch-site": "same-origin",
             "viewport-width": "1475",
             "x-asbd-id": "198387",
             "x-csrftoken": self.csrf_token,
             "x-ig-app-id": self.insta_app_id,
             "x-ig-www-claim": self.x_ig_www_claim,
             "x-requested-with": "XMLHttpRequest",
-            "Referer": f"https://www.instagram.com/{random_referer_username}/followers/",
+            "Referer": f"https://www.instagram.com/{''.join(random.choices(string.ascii_lowercase, k=6))}/followers/",
             "Referrer-Policy": "strict-origin-when-cross-origin"
         }
 
-        max_id = ""
-        required_list = []
+        current_max_id = ""
+        generated_list = []
 
         while True:
-            if max_id != "":
-                max_id_text = f"&max_id={max_id}"
-            else:
-                max_id_text = ""
+            current_max_id_text = ""
 
-            http_response = self.request_session.get(f"https://www.instagram.com/api/v1/friendships/{identifier}/followers/?count={30}{max_id_text}&search_surface=follow_list_page", headers=request_headers)
+            if current_max_id != "":
+                current_max_id_text = f"&max_id={current_max_id}"
 
             try:
+                count_text = 35
+
+                if count < 35:
+                    count_text = count
+
+                http_response = self.request_session.get(f"https://www.instagram.com/api/v1/friendships/{identifier}/followers/?count={str(count_text)}{current_max_id_text}&search_surface=follow_list_page", headers=request_headers)
                 response_json = http_response.json()
 
                 if "status" not in response_json or "users" not in response_json:
-                    return failure_response
+                    return None
 
                 if response_json["status"] != "ok":
-                    return failure_response
+                    return None
 
                 for each_item in response_json["users"]:
-                    if len(required_list) < count or count == 0:
+                    if len(generated_list) < count or count == 0:
 
-                        prop_has_anonymous_profile_picture = False
-                        prop_user_id = ""
-                        prop_username = ""
-                        prop_full_name = ""
-                        prop_is_private = False
-                        prop_is_verified = False
-                        prop_profile_picture_url = ""
-                        prop_is_possible_scammer = False
+                        prop_has_anonymous_profile_picture = None
+                        prop_user_id = None
+                        prop_username = None
+                        prop_full_name = None
+                        prop_is_private = None
+                        prop_is_verified = None
+                        prop_profile_picture_url = None
+                        prop_is_possible_scammer = None
 
                         if "has_anonymous_profile_picture" in each_item:
                             prop_has_anonymous_profile_picture = each_item["has_anonymous_profile_picture"]
 
                         if "pk" in each_item:
                             prop_user_id = each_item["pk"]
 
@@ -277,40 +275,38 @@
 
                         if "profile_pic_url" in each_item:
                             prop_profile_picture_url = each_item["profile_pic_url"]
 
                         if "is_possible_scammer" in each_item:
                             prop_is_possible_scammer = each_item["is_possible_scammer"]
 
-                        follow_person = FollowListPerson(
+                        generated_list.append(FollowPerson(
                             has_anonymous_profile_picture=prop_has_anonymous_profile_picture,
                             user_id=prop_user_id,
                             username=prop_username,
                             full_name=prop_full_name,
                             is_private=prop_is_private,
                             is_verified=prop_is_verified,
                             profile_picture_url=prop_profile_picture_url,
                             is_possible_scammer=prop_is_possible_scammer
-                        )
-                        required_list.append(follow_person)
+                        ))
 
-                if (len(required_list) < count or count == 0) and "next_max_id" in response_json:
-                    max_id = response_json["next_max_id"]
+                if (len(generated_list) < count or count == 0) and "next_max_id" in response_json:
+                    current_max_id = response_json["next_max_id"]
                 else:
-                    return FollowPersonListResponse(success=True, users=required_list)
-            except JSONDecodeError: return failure_response
-
-    def following_list(self, identifier: str | int, count: int):
-        conversion_success, identifier = self.identifier_conversion(identifier, 1)
-        failure_response = FollowPersonListResponse()
-        if not conversion_success: return failure_response
+                    return generated_list
+            except JSONDecodeError:
+                return None
+
+    def following_list(self, identifier: str | int, count: int = 0) -> list[FollowPerson] | None:
+        conversion_success, identifier = self.identifier_conversion(identifier, UID)
+        if not conversion_success: return None
 
         # Actual Request
         refresh_csrf_token(self)
-        random_referer_username = "".join(random.choices(string.ascii_lowercase, k=6))
         request_headers = {
             "accept": "*/*",
             "accept-language": "en-US,en;q=0.9",
             "sec-ch-prefers-color-scheme": self.preferred_color_scheme,
             "sec-ch-ua": "\"Not.A/Brand\";v=\"8\", \"Chromium\";v=\"114\", \"Google Chrome\";v=\"114\"",
             "sec-ch-ua-full-version-list": "\"Not.A/Brand\";v=\"8.0.0.0\", \"Chromium\";v=\"114.0.5735.91\", \"Google Chrome\";v=\"114.0.5735.91\"",
             "sec-ch-ua-mobile": "?0",
@@ -321,40 +317,44 @@
             "sec-fetch-site": "same-origin",
             "viewport-width": "1475",
             "x-asbd-id": "198387",
             "x-csrftoken": self.csrf_token,
             "x-ig-app-id": self.insta_app_id,
             "x-ig-www-claim": self.x_ig_www_claim,
             "x-requested-with": "XMLHttpRequest",
-            "Referer": f"https://www.instagram.com/{random_referer_username}/following/",
+            "Referer": f"https://www.instagram.com/{''.join(random.choices(string.ascii_lowercase, k=6))}/following/",
             "Referrer-Policy": "strict-origin-when-cross-origin"
         }
 
-        max_id = ""
-        required_list = []
+        current_max_id = ""
+        generated_list = []
 
         while True:
-            if max_id != "":
-                max_id_text = f"&max_id={max_id}"
-            else:
-                max_id_text = ""
+            current_max_id_text = ""
 
-            http_response = self.request_session.get(f"https://www.instagram.com/api/v1/friendships/{identifier}/following/?count={30}{max_id_text}", headers=request_headers)
+            if current_max_id != "":
+                current_max_id_text = f"&max_id={current_max_id}"
 
             try:
+                count_text = 35
+
+                if count < 35:
+                    count_text = count
+
+                http_response = self.request_session.get(f"https://www.instagram.com/api/v1/friendships/{identifier}/following/?count={str(count_text)}{current_max_id_text}", headers=request_headers)
                 response_json = http_response.json()
 
                 if "status" not in response_json or "users" not in response_json:
-                    return failure_response
+                    return None
 
                 if response_json["status"] != "ok":
-                    return failure_response
+                    return None
 
                 for each_item in response_json["users"]:
-                    if len(required_list) < count or count == 0:
+                    if len(generated_list) < count or count == 0:
 
                         prop_has_anonymous_profile_picture = False
                         prop_user_id = ""
                         prop_username = ""
                         prop_full_name = ""
                         prop_is_private = False
                         prop_is_verified = False
@@ -381,58 +381,62 @@
 
                         if "profile_pic_url" in each_item:
                             prop_profile_picture_url = each_item["profile_pic_url"]
 
                         if "is_possible_scammer" in each_item:
                             prop_is_possible_scammer = each_item["is_possible_scammer"]
 
-                        follow_person = FollowListPerson(
+                        generated_list.append(FollowPerson(
                             has_anonymous_profile_picture=prop_has_anonymous_profile_picture,
                             user_id=prop_user_id,
                             username=prop_username,
                             full_name=prop_full_name,
                             is_private=prop_is_private,
                             is_verified=prop_is_verified,
                             profile_picture_url=prop_profile_picture_url,
                             is_possible_scammer=prop_is_possible_scammer
-                        )
-                        required_list.append(follow_person)
+                        ))
 
-                if (len(required_list) < count or count == 0) and "next_max_id" in response_json:
-                    max_id = response_json["next_max_id"]
+                if (len(generated_list) < count or count == 0) and "next_max_id" in response_json:
+                    current_max_id = response_json["next_max_id"]
                 else:
-                    return FollowPersonListResponse(success=True, users=required_list)
-            except JSONDecodeError: return failure_response
+                    return generated_list
+            except JSONDecodeError:
+                return None
 
     def identifier_conversion(self, identifier: str | int, required: str | int):
-        identifier = str(identifier).lower().replace(" ", "")
-        if len(identifier) < 1: raise IdentifierError(
-            "No identifier was given. Please pass either UserId or Username as an argument.")
+        identifier = format_identifier(identifier)
 
-        # Detect if identifier is Username or UserId
+        if len(identifier) <= 0:
+            raise IdentifierError("No identifier was given. Please pass either UserId or Username as an argument.")
+
+        # Identifier: Username or UID?
         is_username = False
         for letter in identifier:
             if letter not in string.digits:
                 is_username = True
                 break
 
-        # Generate UserId if identifier is Username
-        if is_username:
-            if required == 0:
-                return identifier
+        if is_username and required == USERNAME:
+            return True, identifier
+
+        elif is_username and required == UID:
+            user_id = self.guest.get_uid(identifier)
+
+            if user_id is not None and user_id != "":
+                return True, user_id
             else:
-                user_id_response = self.guest.get_userid(identifier)
+                return False, None
 
-                if user_id_response["success"]:
-                    return True, user_id_response["user_id"]
-                else:
-                    return False, None
-        else:
-            if required == 0:
-                username_response = self.guest.get_username(identifier)
+        elif not is_username and required == USERNAME:
+            username = self.guest.get_username(identifier)
 
-                if username_response["success"]:
-                    return True, username_response["username"]
-                else:
-                    return False, None
+            if username is not None and username != "":
+                return True, username
             else:
-                return identifier
+                return False, None
+
+        elif not is_username and required == UID:
+            return True, identifier
+
+        else:
+            raise CodeError("Identifier Conversion (Else Block)")
```

### Comparing `ensta-1.3/ensta/containers/Profile.py` & `ensta-1.4/ensta/containers/Profile.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from dataclasses import dataclass
 
 
 @dataclass(frozen=True)
 class Profile:
 
-    success: bool = False
     biography: str = None
     country_block: bool = None
     full_name: str = None
     follower_count: int = None
     following_count: int = None
     user_id: str = None
     is_business_account: bool = None
```

### Comparing `ensta-1.3/ensta/lib/Commons.py` & `ensta-1.4/ensta/lib/Commons.py`

 * *Files 24% similar despite different names*

```diff
@@ -26,7 +26,19 @@
 def update_homepage_source(self):
     temp_homepage_source = requests.get("https://www.instagram.com").text.strip()
 
     if temp_homepage_source != "":
         self.homepage_source = temp_homepage_source
     else:
         raise NetworkError("Couldn't load instagram homepage.")
+
+
+def format_username(username: str):
+    return username.replace(" ", "").lower()
+
+
+def format_uid(uid: str):
+    return uid.replace(" ", "")
+
+
+def format_identifier(identifier: str | int):
+    return str(identifier).lower().replace(" ", "")
```

### Comparing `ensta-1.3/ensta.egg-info/PKG-INFO` & `ensta-1.4/ensta.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: ensta
-Version: 1.3
+Version: 1.4
 Summary: Simple & Up-to-date Instagram API
 Home-page: https://github.com/diezo/ensta
-Download-URL: https://github.com/diezo/ensta/archive/refs/tags/v1.3.tar.gz
+Download-URL: https://github.com/diezo/ensta/archive/refs/tags/v1.4.tar.gz
 Author: Deepak Soni
 Author-email: lonelycube@proton.me
 License: MIT
 Keywords: instagram,web,private,api,scraper,easy,download,upload
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `ensta-1.3/setup.py` & `ensta-1.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from distutils.core import setup
 from pathlib import Path
 
 long_description = (Path(__file__).parent / "README.md").read_text()
 
 setup(
     name="ensta",
-    packages=["ensta", "ensta.lib", "ensta.containers", "ensta.responses"],
-    version="1.3",
+    packages=["ensta", "ensta.lib", "ensta.containers"],
+    version="1.4",
     license="MIT",
     description="Simple & Up-to-date Instagram API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Deepak Soni",
     author_email="lonelycube@proton.me",
     url="https://github.com/diezo/ensta",
-    download_url="https://github.com/diezo/ensta/archive/refs/tags/v1.3.tar.gz",
+    download_url="https://github.com/diezo/ensta/archive/refs/tags/v1.4.tar.gz",
     keywords=["instagram", "web", "private", "api", "scraper", "easy", "download", "upload"],
     install_requires=["requests"],
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Build Tools",
         "License :: OSI Approved :: MIT License",
```

