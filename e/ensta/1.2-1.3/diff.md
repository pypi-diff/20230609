# Comparing `tmp/ensta-1.2.tar.gz` & `tmp/ensta-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ensta-1.2.tar", last modified: Thu Jun  8 07:59:47 2023, max compression
+gzip compressed data, was "ensta-1.3.tar", last modified: Fri Jun  9 06:02:31 2023, max compression
```

## Comparing `ensta-1.2.tar` & `ensta-1.3.tar`

### file list

```diff
@@ -1,24 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-06-08 07:59:47.940869 ensta-1.2/
--rw-rw-rw-   0        0        0     1081 2023-06-06 15:38:39.000000 ensta-1.2/LICENSE.txt
--rw-rw-rw-   0        0        0     3368 2023-06-08 07:59:47.940869 ensta-1.2/PKG-INFO
--rw-rw-rw-   0        0        0     2646 2023-06-08 05:38:39.000000 ensta-1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-08 07:59:47.861935 ensta-1.2/ensta/
--rw-rw-rw-   0        0        0    15694 2023-06-07 07:35:55.000000 ensta-1.2/ensta/Guest.py
--rw-rw-rw-   0        0        0    19079 2023-06-08 07:49:39.000000 ensta-1.2/ensta/Host.py
--rw-rw-rw-   0        0        0      203 2023-06-08 07:50:42.000000 ensta-1.2/ensta/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-08 07:59:47.911749 ensta-1.2/ensta/data_classes/
--rw-rw-rw-   0        0        0     1012 2023-06-08 07:22:37.000000 ensta-1.2/ensta/data_classes/Follower.py
--rw-rw-rw-   0        0        0     1015 2023-06-08 07:47:56.000000 ensta-1.2/ensta/data_classes/Following.py
--rw-rw-rw-   0        0        0      103 2023-06-08 07:48:06.000000 ensta-1.2/ensta/data_classes/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-08 07:59:47.928180 ensta-1.2/ensta/lib/
--rw-rw-rw-   0        0        0     1169 2023-06-07 07:34:14.000000 ensta-1.2/ensta/lib/Commons.py
--rw-rw-rw-   0        0        0      331 2023-06-08 06:52:07.000000 ensta-1.2/ensta/lib/Exceptions.py
--rw-rw-rw-   0        0        0      223 2023-06-08 07:17:03.000000 ensta-1.2/ensta/lib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-08 07:59:47.893445 ensta-1.2/ensta.egg-info/
--rw-rw-rw-   0        0        0     3368 2023-06-08 07:59:47.000000 ensta-1.2/ensta.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      392 2023-06-08 07:59:47.000000 ensta-1.2/ensta.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-08 07:59:47.000000 ensta-1.2/ensta.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-08 07:59:47.000000 ensta-1.2/ensta.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-08 07:59:47.000000 ensta-1.2/ensta.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-08 07:59:47.940869 ensta-1.2/setup.cfg
--rw-rw-rw-   0        0        0     1054 2023-06-08 07:57:10.000000 ensta-1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 06:02:31.946511 ensta-1.3/
+-rw-rw-rw-   0        0        0     1081 2023-06-06 15:38:39.000000 ensta-1.3/LICENSE.txt
+-rw-rw-rw-   0        0        0     3368 2023-06-09 06:02:31.946511 ensta-1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2646 2023-06-08 05:38:39.000000 ensta-1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-09 06:02:31.899098 ensta-1.3/ensta/
+-rw-rw-rw-   0        0        0    13915 2023-06-09 05:58:06.000000 ensta-1.3/ensta/Guest.py
+-rw-rw-rw-   0        0        0    20272 2023-06-08 13:08:53.000000 ensta-1.3/ensta/Host.py
+-rw-rw-rw-   0        0        0       60 2023-06-09 05:22:01.000000 ensta-1.3/ensta/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 06:02:31.914723 ensta-1.3/ensta/containers/
+-rw-rw-rw-   0        0        0      295 2023-06-08 11:36:12.000000 ensta-1.3/ensta/containers/FollowListPerson.py
+-rw-rw-rw-   0        0        0      611 2023-06-09 05:50:34.000000 ensta-1.3/ensta/containers/Profile.py
+-rw-rw-rw-   0        0        0       78 2023-06-08 12:24:32.000000 ensta-1.3/ensta/containers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 06:02:31.930629 ensta-1.3/ensta/lib/
+-rw-rw-rw-   0        0        0     1169 2023-06-07 07:34:14.000000 ensta-1.3/ensta/lib/Commons.py
+-rw-rw-rw-   0        0        0      327 2023-06-08 11:55:00.000000 ensta-1.3/ensta/lib/Exceptions.py
+-rw-rw-rw-   0        0        0      219 2023-06-08 12:02:31.000000 ensta-1.3/ensta/lib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 06:02:31.946511 ensta-1.3/ensta/responses/
+-rw-rw-rw-   0        0        0      248 2023-06-08 11:36:12.000000 ensta-1.3/ensta/responses/FollowPersonListResponse.py
+-rw-rw-rw-   0        0        0      345 2023-06-08 11:34:29.000000 ensta-1.3/ensta/responses/FollowPersonResponse.py
+-rw-rw-rw-   0        0        0      192 2023-06-08 11:32:43.000000 ensta-1.3/ensta/responses/UnfollowPersonResponse.py
+-rw-rw-rw-   0        0        0      180 2023-06-09 05:51:00.000000 ensta-1.3/ensta/responses/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 06:02:31.914723 ensta-1.3/ensta.egg-info/
+-rw-rw-rw-   0        0        0     3368 2023-06-09 06:02:31.000000 ensta-1.3/ensta.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      546 2023-06-09 06:02:31.000000 ensta-1.3/ensta.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 06:02:31.000000 ensta-1.3/ensta.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-09 06:02:31.000000 ensta-1.3/ensta.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-09 06:02:31.000000 ensta-1.3/ensta.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-09 06:02:31.946511 ensta-1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1071 2023-06-09 05:25:09.000000 ensta-1.3/setup.py
```

### Comparing `ensta-1.2/LICENSE.txt` & `ensta-1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ensta-1.2/PKG-INFO` & `ensta-1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: ensta
-Version: 1.2
+Version: 1.3
 Summary: Simple & Up-to-date Instagram API
 Home-page: https://github.com/diezo/ensta
-Download-URL: https://github.com/diezo/ensta/archive/refs/tags/v1.2.tar.gz
+Download-URL: https://github.com/diezo/ensta/archive/refs/tags/v1.3.tar.gz
 Author: Deepak Soni
 Author-email: lonelycube@proton.me
 License: MIT
 Keywords: instagram,web,private,api,scraper,easy,download,upload
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `ensta-1.2/README.md` & `ensta-1.3/README.md`

 * *Files identical despite different names*

### Comparing `ensta-1.2/ensta/Guest.py` & `ensta-1.3/ensta/Guest.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from json import JSONDecodeError
-import base64
 import random
+import string
 import requests
-import requests.cookies
 from .lib.Commons import (
     update_session,
     update_homepage_source,
     update_app_id,
     refresh_csrf_token
 )
+from .lib import IdentifierError
+from .containers.Profile import Profile
 
 
 class Guest:
     request_session: requests.Session = None
     homepage_source: str = None
     insta_app_id: str = None
     csrf_token: str = None
@@ -53,15 +54,17 @@
             "x-instagram-ajax": "1007614758",
             "x-requested-with": "XMLHttpRequest",
             "Referer": "https://www.instagram.com/accounts/emailsignup/",
             "Referrer-Policy": "strict-origin-when-cross-origin"
         }
 
         try:
-            http_response = self.request_session.post("https://www.instagram.com/api/v1/web/accounts/web_create_ajax/attempt/", headers=request_headers, data=body_json)
+            http_response = self.request_session.post(
+                "https://www.instagram.com/api/v1/web/accounts/web_create_ajax/attempt/", headers=request_headers,
+                data=body_json)
             response_json = http_response.json()
 
             if "errors" in response_json:
 
                 username_suggestions = []
                 if "username_suggestions" in response_json:
                     username_suggestions = response_json["username_suggestions"]
@@ -71,16 +74,20 @@
                 else:
                     return {"success": True, "available": True, "suggestions": username_suggestions}
             else:
                 return {"success": False, "available": None, "suggestions": []}
         except JSONDecodeError:
             return {"success": False, "available": None, "suggestions": []}
 
-    def profile_info(self, username: str):
-        username = username.strip().lower().replace(" ", "")
+    def profile(self, identifier: str | int, iu: bool = False):
+        failure_response = Profile()
+        if not iu:
+            conversion_success, identifier = self.identifier_conversion(identifier, 0)
+            if not conversion_success: return failure_response
+
         refresh_csrf_token(self)
         preferred_color_scheme = random.choice(["light", "dark"])
         request_headers = {
             "accept": "*/*",
             "accept-language": "en-US,en;q=0.9",
             "sec-ch-prefers-color-scheme": preferred_color_scheme,
             "sec-ch-ua": "\"Not.A/Brand\";v=\"8\", \"Chromium\";v=\"114\", \"Google Chrome\";v=\"114\"",
@@ -93,59 +100,142 @@
             "sec-fetch-site": "same-origin",
             "viewport-width": "1475",
             "x-asbd-id": "198387",
             "x-csrftoken": self.csrf_token,
             "x-ig-app-id": self.insta_app_id,
             "x-ig-www-claim": "0",
             "x-requested-with": "XMLHttpRequest",
-            "Referer": f"https://www.instagram.com/{username}/",
+            "Referer": f"https://www.instagram.com/{identifier}/",
             "Referrer-Policy": "strict-origin-when-cross-origin"
         }
 
         try:
-            http_response = self.request_session.get(f"https://www.instagram.com/api/v1/users/web_profile_info/?username={username}", headers=request_headers)
+            http_response = self.request_session.get(
+                f"https://www.instagram.com/api/v1/users/web_profile_info/?username={identifier}",
+                headers=request_headers)
             response_json = http_response.json()
 
             if "status" in response_json:
                 if response_json["status"] == "ok" and "data" in response_json:
                     if "user" in response_json["data"]:
-                        return {"success": True, "data": response_json["data"]["user"]}
+
+                        profile_object_biography = None
+                        profile_object_country_block = None
+                        profile_object_full_name = None
+                        profile_object_following_count = None
+                        profile_object_follower_count = None
+                        profile_object_user_id = None
+                        profile_object_is_business_account = None
+                        profile_object_is_professional_account = None
+                        profile_object_is_supervision_enabled = None
+                        profile_object_is_joined_recently = None
+                        profile_object_is_private = None
+                        profile_object_is_verified = None
+                        profile_object_profile_picture_url = None
+                        profile_object_profile_picture_url_hd = None
+                        profile_object_pronouns = None
+
+                        if "biography" in response_json["data"]["user"]:
+                            profile_object_biography = response_json["data"]["user"]["biography"]
+
+                        if "country_block" in response_json["data"]["user"]:
+                            profile_object_country_block = response_json["data"]["user"]["country_block"]
+
+                        if "full_name" in response_json["data"]["user"]:
+                            profile_object_full_name = response_json["data"]["user"]["full_name"]
+
+                        if "edge_follow" in response_json["data"]["user"]:
+                            if "count" in response_json["data"]["user"]["edge_follow"]:
+                                profile_object_following_count = response_json["data"]["user"]["edge_follow"]["count"]
+
+                        if "edge_followed_by" in response_json["data"]["user"]:
+                            if "count" in response_json["data"]["user"]["edge_followed_by"]:
+                                profile_object_follower_count = response_json["data"]["user"]["edge_followed_by"]["count"]
+
+                        if "id" in response_json["data"]["user"]:
+                            profile_object_user_id = response_json["data"]["user"]["id"]
+
+                        if "is_business_account" in response_json["data"]["user"]:
+                            profile_object_is_business_account = response_json["data"]["user"]["is_business_account"]
+
+                        if "is_professional_account" in response_json["data"]["user"]:
+                            profile_object_is_professional_account = response_json["data"]["user"]["is_professional_account"]
+
+                        if "is_supervision_enabled" in response_json["data"]["user"]:
+                            profile_object_is_supervision_enabled = response_json["data"]["user"][
+                                "is_supervision_enabled"]
+
+                        if "is_joined_recently" in response_json["data"]["user"]:
+                            profile_object_is_joined_recently = response_json["data"]["user"]["is_joined_recently"]
+
+                        if "is_private" in response_json["data"]["user"]:
+                            profile_object_is_private = response_json["data"]["user"]["is_private"]
+
+                        if "is_verified" in response_json["data"]["user"]:
+                            profile_object_is_verified = response_json["data"]["user"]["is_verified"]
+
+                        if "profile_pic_url" in response_json["data"]["user"]:
+                            profile_object_profile_picture_url = response_json["data"]["user"]["profile_pic_url"]
+
+                        if "profile_pic_url_hd" in response_json["data"]["user"]:
+                            profile_object_profile_picture_url_hd = response_json["data"]["user"]["profile_pic_url_hd"]
+
+                        if "pronouns" in response_json["data"]["user"]:
+                            user_pronouns = []
+                            for pronoun in response_json["data"]["user"]["pronouns"]:
+                                user_pronouns.append(pronoun)
+                            profile_object_pronouns = user_pronouns
+
+                        return Profile(success=True,
+                                       biography=profile_object_biography,
+                                       country_block=profile_object_country_block,
+                                       full_name=profile_object_full_name,
+                                       follower_count=profile_object_follower_count,
+                                       following_count=profile_object_following_count,
+                                       user_id=profile_object_user_id,
+                                       is_business_account=profile_object_is_business_account,
+                                       is_professional_account=profile_object_is_professional_account,
+                                       is_supervision_enabled=profile_object_is_supervision_enabled,
+                                       is_joined_recently=profile_object_is_joined_recently,
+                                       is_private=profile_object_is_private,
+                                       is_verified=profile_object_is_verified,
+                                       profile_picture_url=profile_object_profile_picture_url,
+                                       profile_picture_url_hd=profile_object_profile_picture_url_hd,
+                                       pronouns=profile_object_pronouns)
+
                     else:
-                        return {"success": False, "data": None}
+                        return failure_response
                 else:
-                    return {"success": False, "data": None}
+                    return failure_response
             else:
-                return {"success": False, "data": None}
+                return failure_response
         except JSONDecodeError:
-            return {"success": False, "data": None}
+            return failure_response
 
-    def get_userid(self, username: str, profile_snapshot: dict | None = None):
+    def get_userid(self, username: str):
         username = username.strip().lower().replace(" ", "")
+        response = self.profile(username, iu=True)
 
-        if profile_snapshot is not None:
-            response = profile_snapshot
-        else:
-            response = self.profile_info(username)
-
-        if response["success"]:
-            if "id" in response["data"]:
-                return {"success": True, "user_id": str(response["data"]["id"]).strip()}
+        if response.success:
+            if response.user_id is not None:
+                return {"success": True, "user_id": str(response.user_id).strip()}
             else:
                 return {"success": False, "user_id": ""}
         else:
             return {"success": False, "user_id": ""}
 
     def get_username(self, user_id: str | int):
         user_id = str(user_id).strip()
         request_headers = {
             "User-Agent": "Instagram 76.0.0.15.395 Android (24/7.0; 640dpi; 1440x2560; samsung; SM-G930F; herolte; samsungexynos8890; en_US; 138226743)"
         }
 
         try:
-            http_response = self.request_session.get(f"https://i.instagram.com/api/v1/users/{user_id}/info/", headers=request_headers)
+            http_response = self.request_session.get(f"https://i.instagram.com/api/v1/users/{user_id}/info/",
+                                                     headers=request_headers)
             response_json = http_response.json()
 
             if "status" in response_json:
                 if response_json["status"] == "ok" and "user" in response_json:
                     if "username" in response_json["user"]:
                         return {"success": True, "username": response_json["user"]["username"]}
                     else:
@@ -154,210 +244,40 @@
                     return {"success": False, "username": ""}
             else:
                 return {"success": False, "username": ""}
 
         except JSONDecodeError:
             return {"success": False, "username": ""}
 
-    def get_follower_count(self, username: str, profile_snapshot: dict | None = None):
-        username = username.strip().lower().replace(" ", "")
-
-        if profile_snapshot is not None:
-            response = profile_snapshot
-        else:
-            response = self.profile_info(username)
-
-        if response["success"]:
-            if "edge_followed_by" in response["data"]:
-                if "count" in response["data"]["edge_followed_by"]:
-                    return {"success": True, "follower_count": response["data"]["edge_followed_by"]["count"]}
-                else:
-                    return {"success": False, "follower_count": ""}
+    def identifier_conversion(self, identifier: str | int, required: str | int):
+        identifier = str(identifier).lower().replace(" ", "")
+        if len(identifier) < 1: raise IdentifierError(
+            "No identifier was given. Please pass either UserId or Username as an argument.")
+
+        # Detect if identifier is Username or UserId
+        is_username = False
+        for letter in identifier:
+            if letter not in string.digits:
+                is_username = True
+                break
+
+        # Generate UserId if identifier is Username
+        if is_username:
+            if required == 0:
+                return True, identifier
             else:
-                return {"success": False, "follower_count": ""}
-        else:
-            return {"success": False, "follower_count": ""}
-
-    def get_following_count(self, username: str, profile_snapshot: dict | None = None):
-        username = username.strip().lower().replace(" ", "")
+                user_id_response = self.get_userid(identifier)
 
-        if profile_snapshot is not None:
-            response = profile_snapshot
-        else:
-            response = self.profile_info(username)
-
-        if response["success"]:
-            if "edge_follow" in response["data"]:
-                if "count" in response["data"]["edge_follow"]:
-                    return {"success": True, "following_count": response["data"]["edge_follow"]["count"]}
+                if user_id_response["success"]:
+                    return True, user_id_response["user_id"]
                 else:
-                    return {"success": False, "following_count": ""}
-            else:
-                return {"success": False, "following_count": ""}
-        else:
-            return {"success": False, "following_count": ""}
-
-    def get_biography(self, username: str, profile_snapshot: dict | None = None):
-        username = username.strip().lower().replace(" ", "")
-
-        if profile_snapshot is not None:
-            response = profile_snapshot
-        else:
-            response = self.profile_info(username)
-
-        if response["success"]:
-            if "biography" in response["data"]:
-                return {"success": True, "biography": response["data"]["biography"]}
-            else:
-                return {"success": False, "biography": ""}
-        else:
-            return {"success": False, "biography": ""}
-
-    def get_display_name(self, username: str, profile_snapshot: dict | None = None):
-        username = username.strip().lower().replace(" ", "")
-
-        if profile_snapshot is not None:
-            response = profile_snapshot
-        else:
-            response = self.profile_info(username)
-
-        if response["success"]:
-            if "full_name" in response["data"]:
-                return {"success": True, "display_name": response["data"]["full_name"]}
-            else:
-                return {"success": False, "display_name": ""}
-        else:
-            return {"success": False, "display_name": ""}
-
-    def get_profile_picture_url(self, username: str, profile_snapshot: dict | None = None):
-        username = username.strip().lower().replace(" ", "")
-
-        if profile_snapshot is not None:
-            response = profile_snapshot
-        else:
-            response = self.profile_info(username)
-
-        if response["success"]:
-            if "profile_pic_url" in response["data"]:
-                return {"success": True, "profile_picture_url": str(response["data"]["profile_pic_url"]).strip()}
-            else:
-                return {"success": False, "profile_picture_url": ""}
-        else:
-            return {"success": False, "profile_picture_url": ""}
-
-    def get_profile_picture_url_hd(self, username: str, profile_snapshot: dict | None = None):
-        username = username.strip().lower().replace(" ", "")
-
-        if profile_snapshot is not None:
-            response = profile_snapshot
-        else:
-            response = self.profile_info(username)
-
-        if response["success"]:
-            if "profile_pic_url_hd" in response["data"]:
-                return {"success": True, "profile_picture_url_hd": str(response["data"]["profile_pic_url_hd"]).strip()}
-            else:
-                return {"success": False, "profile_picture_url_hd": ""}
-        else:
-            return {"success": False, "profile_picture_url_hd": ""}
-
-    def get_profile_picture_base64(self, username: str, profile_snapshot: dict | None = None):
-        username = username.strip().lower().replace(" ", "")
-
-        if profile_snapshot is not None:
-            response = self.get_profile_picture_url(username, profile_snapshot)
-        else:
-            response = self.get_profile_picture_url(username)
-
-        if response["success"]:
-            profile_picture_url = response["profile_picture_url"]
-
-            if profile_picture_url == "":
-                return {"success": False, "profile_picture_base64": ""}
-
-            base64_image = base64.b64encode(requests.get(profile_picture_url).content).decode("utf-8")
-            return {"success": True, "profile_picture_base64": f"data:image/jpg;base64,{base64_image}"}
-        else:
-            return {"success": False, "profile_picture_base64": ""}
-
-    def get_profile_picture_base64_hd(self, username: str, profile_snapshot: dict | None = None):
-        username = username.strip().lower().replace(" ", "")
-
-        if profile_snapshot is not None:
-            response = self.get_profile_picture_url_hd(username, profile_snapshot)
-        else:
-            response = self.get_profile_picture_url_hd(username)
-
-        if response["success"]:
-            profile_picture_url_hd = response["profile_picture_url_hd"]
-
-            if profile_picture_url_hd == "":
-                return {"success": False, "profile_picture_base64_hd": ""}
-
-            base64_image = base64.b64encode(requests.get(profile_picture_url_hd).content).decode("utf-8")
-            return {"success": True, "profile_picture_base64_hd": f"data:image/jpg;base64,{base64_image}"}
-        else:
-            return {"success": False, "profile_picture_base64_hd": ""}
-
-    def is_account_private(self, username: str, profile_snapshot: dict | None = None):
-        username = username.strip().lower().replace(" ", "")
-
-        if profile_snapshot is not None:
-            response = profile_snapshot
-        else:
-            response = self.profile_info(username)
-
-        if response["success"]:
-            if "is_private" in response["data"]:
-                return {"success": True, "private": response["data"]["is_private"]}
-            else:
-                return {"success": False, "private": None}
-        else:
-            return {"success": False, "private": None}
-
-    def is_account_verified(self, username: str, profile_snapshot: dict | None = None):
-        username = username.strip().lower().replace(" ", "")
-
-        if profile_snapshot is not None:
-            response = profile_snapshot
-        else:
-            response = self.profile_info(username)
-
-        if response["success"]:
-            if "is_verified" in response["data"]:
-                return {"success": True, "verified": response["data"]["is_verified"]}
-            else:
-                return {"success": False, "verified": None}
-        else:
-            return {"success": False, "verified": None}
-
-    def is_business_account(self, username: str, profile_snapshot: dict | None = None):
-        username = username.strip().lower().replace(" ", "")
-
-        if profile_snapshot is not None:
-            response = profile_snapshot
-        else:
-            response = self.profile_info(username)
-
-        if response["success"]:
-            if "is_business_account" in response["data"]:
-                return {"success": True, "business_account": response["data"]["is_business_account"]}
-            else:
-                return {"success": False, "business_account": None}
+                    return False, None
         else:
-            return {"success": False, "business_account": None}
+            if required == 0:
+                username_response = self.get_username(identifier)
 
-    def is_professional_account(self, username: str, profile_snapshot: dict | None = None):
-        username = username.strip().lower().replace(" ", "")
-
-        if profile_snapshot is not None:
-            response = profile_snapshot
-        else:
-            response = self.profile_info(username)
-
-        if response["success"]:
-            if "is_professional_account" in response["data"]:
-                return {"success": True, "professional_account": response["data"]["is_professional_account"]}
+                if username_response["success"]:
+                    return True, username_response["username"]
+                else:
+                    return False, None
             else:
-                return {"success": False, "professional_account": None}
-        else:
-            return {"success": False, "professional_account": None}
+                return True, identifier
```

### Comparing `ensta-1.2/ensta/Host.py` & `ensta-1.3/ensta/Host.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import requests
-import requests.cookies
 from json import JSONDecodeError
 import random
 import string
 from .Guest import Guest
 from .lib.Commons import (
     refresh_csrf_token,
     update_app_id,
     update_homepage_source,
     update_session
 )
 from .lib import (
     AuthenticationError,
     NetworkError,
-    IdentifierTypeError
+    IdentifierError
 )
-from .data_classes import FollowerInternal
-from .data_classes import FollowingInternal
-from ensta.identifier import IDENTIFIER_USERNAME, IDENTIFIER_USERID
+from .containers import FollowListPerson
+from .responses.FollowPersonListResponse import FollowPersonListResponse
+from .responses.FollowPersonResponse import FollowPersonResponse
+from .responses.UnfollowPersonResponse import UnfollowPersonResponse
 
 
 class Host:
     request_session: requests.Session = None
     homepage_source: str = None
     insta_app_id: str = None
     preferred_color_scheme: str = "dark"
@@ -76,22 +76,26 @@
 
         try:
             http_response.json()
             return True
         except JSONDecodeError:
             return False
 
-    def follow_user_id(self, user_id: str | int):
-        user_id = str(user_id).strip()
+    def follow(self, identifier: str | int):
+        conversion_success, identifier = self.identifier_conversion(identifier, 1)
+        failure_response = FollowPersonResponse()
+        if not conversion_success: return failure_response
+
+        # Actual Request
         refresh_csrf_token(self)
         random_referer_username = "".join(random.choices(string.ascii_lowercase, k=6))
         body_json = {
             "container_module": "profile",
             "nav_chain": f"PolarisProfileRoot:profilePage:1:via_cold_start",
-            "user_id": user_id
+            "user_id": identifier
         }
         request_headers = {
             "accept": "*/*",
             "accept-language": "en-US,en;q=0.9",
             "content-type": "application/x-www-form-urlencoded",
             "sec-ch-prefers-color-scheme": self.preferred_color_scheme,
             "sec-ch-ua": "\"Not.A/Brand\";v=\"8\", \"Chromium\";v=\"114\", \"Google Chrome\";v=\"114\"",
@@ -109,56 +113,49 @@
             "x-ig-www-claim": self.x_ig_www_claim,
             "x-instagram-ajax": "1007616494",
             "x-requested-with": "XMLHttpRequest",
             "Referer": f"https://www.instagram.com/{random_referer_username}/",
             "Referrer-Policy": "strict-origin-when-cross-origin"
         }
 
-        failure_response = {"success": False, "following": None, "follow_requested": None, "previous_following": None, "is_my_follower": None}
-        http_response = self.request_session.post(f"https://www.instagram.com/api/v1/friendships/create/{user_id}/", headers=request_headers, data=body_json)
+        http_response = self.request_session.post(f"https://www.instagram.com/api/v1/friendships/create/{identifier}/", headers=request_headers, data=body_json)
 
         try:
             response_json = http_response.json()
 
             if "status" in response_json:
                 if response_json["status"] == "ok" and "friendship_status" in response_json:
                     if "following" in response_json["friendship_status"] \
                             and "outgoing_request" in response_json["friendship_status"] \
                             and "followed_by" in response_json["friendship_status"] \
                             and "previous_following" in response_json:
-                        return {
-                            "success": True,
-                            "following": response_json["friendship_status"]["following"],
-                            "follow_requested": response_json["friendship_status"]["outgoing_request"],
-                            "is_my_follower": response_json["friendship_status"]["followed_by"],
-                            "previous_following": response_json["previous_following"]
-                        }
+                        return FollowPersonResponse(
+                            success=True,
+                            following=response_json["friendship_status"]["following"],
+                            follow_requested=response_json["friendship_status"]["outgoing_request"],
+                            is_my_follower=response_json["friendship_status"]["followed_by"],
+                            previous_following=response_json["previous_following"]
+                        )
                     else: return failure_response
                 else: return failure_response
             else: return failure_response
         except JSONDecodeError: return failure_response
 
-    def follow_username(self, username: str):
-        username = username.lower().strip().replace(" ", "")
-        user_id_response = self.guest.get_userid(username)
-        failure_response = {"success": False, "following": None, "follow_requested": None, "previous_following": None, "is_my_follower": None}
-
-        if user_id_response["success"]:
-            return self.follow_user_id(user_id_response["user_id"])
-        else:
-            return failure_response
+    def unfollow(self, identifier: str | int):
+        conversion_success, identifier = self.identifier_conversion(identifier, 1)
+        failure_response = UnfollowPersonResponse()
+        if not conversion_success: return failure_response
 
-    def unfollow_user_id(self, user_id: str | int):
-        user_id = str(user_id).strip()
+        # Actual Request
         refresh_csrf_token(self)
         random_referer_username = "".join(random.choices(string.ascii_lowercase, k=6))
         body_json = {
             "container_module": "profile",
             "nav_chain": f"PolarisProfileRoot:profilePage:1:via_cold_start",
-            "user_id": user_id
+            "user_id": identifier
         }
         request_headers = {
             "accept": "*/*",
             "accept-language": "en-US,en;q=0.9",
             "content-type": "application/x-www-form-urlencoded",
             "sec-ch-prefers-color-scheme": self.preferred_color_scheme,
             "sec-ch-ua": "\"Not.A/Brand\";v=\"8\", \"Chromium\";v=\"114\", \"Google Chrome\";v=\"114\"",
@@ -176,59 +173,36 @@
             "x-ig-www-claim": self.x_ig_www_claim,
             "x-instagram-ajax": "1007616494",
             "x-requested-with": "XMLHttpRequest",
             "Referer": f"https://www.instagram.com/{random_referer_username}/",
             "Referrer-Policy": "strict-origin-when-cross-origin"
         }
 
-        failure_response = {"success": False, "unfollowed": None}
-        http_response = self.request_session.post(f"https://www.instagram.com/api/v1/friendships/destroy/{user_id}/", headers=request_headers, data=body_json)
+        http_response = self.request_session.post(f"https://www.instagram.com/api/v1/friendships/destroy/{identifier}/", headers=request_headers, data=body_json)
 
         try:
             response_json = http_response.json()
 
             if "status" in response_json:
                 if response_json["status"] == "ok" and "friendship_status" in response_json:
                     if "following" in response_json["friendship_status"] \
                             and "outgoing_request" in response_json["friendship_status"]:
-                        return {
-                            "success": True,
-                            "unfollowed": not response_json["friendship_status"]["following"] and not response_json["friendship_status"]["outgoing_request"]
-                        }
+                        return UnfollowPersonResponse(
+                            success=True,
+                            unfollowed=not response_json["friendship_status"]["following"] and not response_json["friendship_status"]["outgoing_request"]
+                        )
                     else: return failure_response
                 else: return failure_response
             else: return failure_response
         except JSONDecodeError: return failure_response
 
-    def unfollow_username(self, username: str):
-        username = username.lower().strip().replace(" ", "")
-        user_id_response = self.guest.get_userid(username)
-        failure_response = {"success": False, "unfollowed": None}
-
-        if user_id_response["success"]:
-            return self.unfollow_user_id(user_id_response["user_id"])
-        else:
-            return failure_response
-
-    def follower_list(self, identifier_type: int, identifier: str | int, count: int):
-
-        # Identifier Conversion
-        if identifier_type == IDENTIFIER_USERNAME:
-            username = identifier.lower().strip().replace(" ", "")
-            user_id_response = self.guest.get_userid(username)
-            failure_response = {"success": False, "follower_list": None}
-
-            if user_id_response["success"]:
-                user_id = user_id_response["user_id"]
-            else:
-                return failure_response
-        elif identifier_type == IDENTIFIER_USERID:
-            user_id = str(identifier).strip()
-        else:
-            raise IdentifierTypeError(f"{str(identifier_type)} is not a valid identifier type. Please choose a valid identifier type from ensta.identifier package.")
+    def follower_list(self, identifier: str | int, count: int):
+        conversion_success, identifier = self.identifier_conversion(identifier, 1)
+        failure_response = FollowPersonListResponse()
+        if not conversion_success: return failure_response
 
         # Actual Request
         refresh_csrf_token(self)
         random_referer_username = "".join(random.choices(string.ascii_lowercase, k=6))
         request_headers = {
             "accept": "*/*",
             "accept-language": "en-US,en;q=0.9",
@@ -247,87 +221,92 @@
             "x-ig-app-id": self.insta_app_id,
             "x-ig-www-claim": self.x_ig_www_claim,
             "x-requested-with": "XMLHttpRequest",
             "Referer": f"https://www.instagram.com/{random_referer_username}/followers/",
             "Referrer-Policy": "strict-origin-when-cross-origin"
         }
 
-        failure_response = {"success": False, "follower_list": None}
         max_id = ""
         required_list = []
 
         while True:
             if max_id != "":
                 max_id_text = f"&max_id={max_id}"
             else:
                 max_id_text = ""
 
-            http_response = self.request_session.get(f"https://www.instagram.com/api/v1/friendships/{user_id}/followers/?count={30}{max_id_text}&search_surface=follow_list_page", headers=request_headers)
+            http_response = self.request_session.get(f"https://www.instagram.com/api/v1/friendships/{identifier}/followers/?count={30}{max_id_text}&search_surface=follow_list_page", headers=request_headers)
 
             try:
                 response_json = http_response.json()
 
                 if "status" not in response_json or "users" not in response_json:
                     return failure_response
 
                 if response_json["status"] != "ok":
                     return failure_response
 
                 for each_item in response_json["users"]:
                     if len(required_list) < count or count == 0:
-                        follower_obj = FollowerInternal()
+
+                        prop_has_anonymous_profile_picture = False
+                        prop_user_id = ""
+                        prop_username = ""
+                        prop_full_name = ""
+                        prop_is_private = False
+                        prop_is_verified = False
+                        prop_profile_picture_url = ""
+                        prop_is_possible_scammer = False
 
                         if "has_anonymous_profile_picture" in each_item:
-                            follower_obj.has_anonymous_profile_picture = each_item["has_anonymous_profile_picture"]
+                            prop_has_anonymous_profile_picture = each_item["has_anonymous_profile_picture"]
 
                         if "pk" in each_item:
-                            follower_obj.user_id = each_item["pk"]
+                            prop_user_id = each_item["pk"]
 
                         if "username" in each_item:
-                            follower_obj.username = each_item["username"]
+                            prop_username = each_item["username"]
 
                         if "full_name" in each_item:
-                            follower_obj.full_name = each_item["full_name"]
+                            prop_full_name = each_item["full_name"]
 
                         if "is_private" in each_item:
-                            follower_obj.is_private = each_item["is_private"]
+                            prop_is_private = each_item["is_private"]
 
                         if "is_verified" in each_item:
-                            follower_obj.is_verified = each_item["is_verified"]
+                            prop_is_verified = each_item["is_verified"]
 
                         if "profile_pic_url" in each_item:
-                            follower_obj.profile_picture_url = each_item["profile_pic_url"]
+                            prop_profile_picture_url = each_item["profile_pic_url"]
 
                         if "is_possible_scammer" in each_item:
-                            follower_obj.is_possible_scammer = each_item["is_possible_scammer"]
+                            prop_is_possible_scammer = each_item["is_possible_scammer"]
 
-                        required_list.append(follower_obj)
+                        follow_person = FollowListPerson(
+                            has_anonymous_profile_picture=prop_has_anonymous_profile_picture,
+                            user_id=prop_user_id,
+                            username=prop_username,
+                            full_name=prop_full_name,
+                            is_private=prop_is_private,
+                            is_verified=prop_is_verified,
+                            profile_picture_url=prop_profile_picture_url,
+                            is_possible_scammer=prop_is_possible_scammer
+                        )
+                        required_list.append(follow_person)
 
                 if (len(required_list) < count or count == 0) and "next_max_id" in response_json:
                     max_id = response_json["next_max_id"]
                 else:
-                    return {"success": True, "follower_list": required_list}
+                    return FollowPersonListResponse(success=True, users=required_list)
             except JSONDecodeError: return failure_response
 
-    def following_list(self, identifier_type: int, identifier: str | int, count: int):
-
-        # Identifier Conversion
-        if identifier_type == IDENTIFIER_USERNAME:
-            username = identifier.lower().strip().replace(" ", "")
-            user_id_response = self.guest.get_userid(username)
-            failure_response = {"success": False, "following_list": None}
-
-            if user_id_response["success"]:
-                user_id = user_id_response["user_id"]
-            else:
-                return failure_response
-        elif identifier_type == IDENTIFIER_USERID:
-            user_id = str(identifier).strip()
-        else:
-            raise IdentifierTypeError(f"{str(identifier_type)} is not a valid identifier type. Please choose a valid identifier type from ensta.identifier package.")
+    def following_list(self, identifier: str | int, count: int):
+        conversion_success, identifier = self.identifier_conversion(identifier, 1)
+        failure_response = FollowPersonListResponse()
+        if not conversion_success: return failure_response
 
         # Actual Request
         refresh_csrf_token(self)
         random_referer_username = "".join(random.choices(string.ascii_lowercase, k=6))
         request_headers = {
             "accept": "*/*",
             "accept-language": "en-US,en;q=0.9",
@@ -346,63 +325,114 @@
             "x-ig-app-id": self.insta_app_id,
             "x-ig-www-claim": self.x_ig_www_claim,
             "x-requested-with": "XMLHttpRequest",
             "Referer": f"https://www.instagram.com/{random_referer_username}/following/",
             "Referrer-Policy": "strict-origin-when-cross-origin"
         }
 
-        failure_response = {"success": False, "following_list": None}
         max_id = ""
         required_list = []
 
         while True:
             if max_id != "":
                 max_id_text = f"&max_id={max_id}"
             else:
                 max_id_text = ""
 
-            http_response = self.request_session.get(f"https://www.instagram.com/api/v1/friendships/{user_id}/following/?count={30}{max_id_text}", headers=request_headers)
+            http_response = self.request_session.get(f"https://www.instagram.com/api/v1/friendships/{identifier}/following/?count={30}{max_id_text}", headers=request_headers)
 
             try:
                 response_json = http_response.json()
 
                 if "status" not in response_json or "users" not in response_json:
                     return failure_response
 
                 if response_json["status"] != "ok":
                     return failure_response
 
                 for each_item in response_json["users"]:
                     if len(required_list) < count or count == 0:
-                        following_obj = FollowingInternal()
+
+                        prop_has_anonymous_profile_picture = False
+                        prop_user_id = ""
+                        prop_username = ""
+                        prop_full_name = ""
+                        prop_is_private = False
+                        prop_is_verified = False
+                        prop_profile_picture_url = ""
+                        prop_is_possible_scammer = False
 
                         if "has_anonymous_profile_picture" in each_item:
-                            following_obj.has_anonymous_profile_picture = each_item["has_anonymous_profile_picture"]
+                            prop_has_anonymous_profile_picture = each_item["has_anonymous_profile_picture"]
 
                         if "pk" in each_item:
-                            following_obj.user_id = each_item["pk"]
+                            prop_user_id = each_item["pk"]
 
                         if "username" in each_item:
-                            following_obj.username = each_item["username"]
+                            prop_username = each_item["username"]
 
                         if "full_name" in each_item:
-                            following_obj.full_name = each_item["full_name"]
+                            prop_full_name = each_item["full_name"]
 
                         if "is_private" in each_item:
-                            following_obj.is_private = each_item["is_private"]
+                            prop_is_private = each_item["is_private"]
 
                         if "is_verified" in each_item:
-                            following_obj.is_verified = each_item["is_verified"]
+                            prop_is_verified = each_item["is_verified"]
 
                         if "profile_pic_url" in each_item:
-                            following_obj.profile_picture_url = each_item["profile_pic_url"]
+                            prop_profile_picture_url = each_item["profile_pic_url"]
 
                         if "is_possible_scammer" in each_item:
-                            following_obj.is_possible_scammer = each_item["is_possible_scammer"]
+                            prop_is_possible_scammer = each_item["is_possible_scammer"]
 
-                        required_list.append(following_obj)
+                        follow_person = FollowListPerson(
+                            has_anonymous_profile_picture=prop_has_anonymous_profile_picture,
+                            user_id=prop_user_id,
+                            username=prop_username,
+                            full_name=prop_full_name,
+                            is_private=prop_is_private,
+                            is_verified=prop_is_verified,
+                            profile_picture_url=prop_profile_picture_url,
+                            is_possible_scammer=prop_is_possible_scammer
+                        )
+                        required_list.append(follow_person)
 
                 if (len(required_list) < count or count == 0) and "next_max_id" in response_json:
                     max_id = response_json["next_max_id"]
                 else:
-                    return {"success": True, "following_list": required_list}
+                    return FollowPersonListResponse(success=True, users=required_list)
             except JSONDecodeError: return failure_response
+
+    def identifier_conversion(self, identifier: str | int, required: str | int):
+        identifier = str(identifier).lower().replace(" ", "")
+        if len(identifier) < 1: raise IdentifierError(
+            "No identifier was given. Please pass either UserId or Username as an argument.")
+
+        # Detect if identifier is Username or UserId
+        is_username = False
+        for letter in identifier:
+            if letter not in string.digits:
+                is_username = True
+                break
+
+        # Generate UserId if identifier is Username
+        if is_username:
+            if required == 0:
+                return identifier
+            else:
+                user_id_response = self.guest.get_userid(identifier)
+
+                if user_id_response["success"]:
+                    return True, user_id_response["user_id"]
+                else:
+                    return False, None
+        else:
+            if required == 0:
+                username_response = self.guest.get_username(identifier)
+
+                if username_response["success"]:
+                    return True, username_response["username"]
+                else:
+                    return False, None
+            else:
+                return identifier
```

### Comparing `ensta-1.2/ensta/lib/Commons.py` & `ensta-1.3/ensta/lib/Commons.py`

 * *Files identical despite different names*

### Comparing `ensta-1.2/ensta.egg-info/PKG-INFO` & `ensta-1.3/ensta.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: ensta
-Version: 1.2
+Version: 1.3
 Summary: Simple & Up-to-date Instagram API
 Home-page: https://github.com/diezo/ensta
-Download-URL: https://github.com/diezo/ensta/archive/refs/tags/v1.2.tar.gz
+Download-URL: https://github.com/diezo/ensta/archive/refs/tags/v1.3.tar.gz
 Author: Deepak Soni
 Author-email: lonelycube@proton.me
 License: MIT
 Keywords: instagram,web,private,api,scraper,easy,download,upload
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `ensta-1.2/setup.py` & `ensta-1.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from distutils.core import setup
 from pathlib import Path
 
 long_description = (Path(__file__).parent / "README.md").read_text()
 
 setup(
     name="ensta",
-    packages=["ensta", "ensta.lib", "ensta.data_classes"],
-    version="1.2",
+    packages=["ensta", "ensta.lib", "ensta.containers", "ensta.responses"],
+    version="1.3",
     license="MIT",
     description="Simple & Up-to-date Instagram API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Deepak Soni",
     author_email="lonelycube@proton.me",
     url="https://github.com/diezo/ensta",
-    download_url="https://github.com/diezo/ensta/archive/refs/tags/v1.2.tar.gz",
+    download_url="https://github.com/diezo/ensta/archive/refs/tags/v1.3.tar.gz",
     keywords=["instagram", "web", "private", "api", "scraper", "easy", "download", "upload"],
     install_requires=["requests"],
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Build Tools",
         "License :: OSI Approved :: MIT License",
```

