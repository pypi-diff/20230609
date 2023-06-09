# Comparing `tmp/tikapi-3.1.21.tar.gz` & `tmp/tikapi-3.1.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tikapi-3.1.21.tar", last modified: Sat May 13 16:56:24 2023, max compression
+gzip compressed data, was "tikapi-3.1.22.tar", last modified: Fri Jun  9 14:15:02 2023, max compression
```

## Comparing `tikapi-3.1.21.tar` & `tikapi-3.1.22.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-13 16:56:24.170378 tikapi-3.1.21/
--rw-rw-rw-   0        0        0       67 2022-12-07 21:27:40.000000 tikapi-3.1.21/MANIFEST.in
--rw-rw-rw-   0        0        0     1861 2023-05-13 16:56:24.170378 tikapi-3.1.21/PKG-INFO
--rw-rw-rw-   0        0        0     1106 2022-08-29 11:23:45.000000 tikapi-3.1.21/README.md
--rw-rw-rw-   0        0        0      121 2023-05-13 16:56:24.171376 tikapi-3.1.21/setup.cfg
--rw-rw-rw-   0        0        0      704 2023-05-13 16:54:05.000000 tikapi-3.1.21/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-13 16:56:24.164378 tikapi-3.1.21/tikapi/
--rw-rw-rw-   0        0        0     3172 2022-12-07 20:49:56.000000 tikapi-3.1.21/tikapi/__init__.py
--rw-rw-rw-   0        0        0    63920 2023-05-13 16:54:14.000000 tikapi-3.1.21/tikapi/api.py
-drwxrwxrwx   0        0        0        0 2023-05-13 16:56:24.170378 tikapi-3.1.21/tikapi.egg-info/
--rw-rw-rw-   0        0        0     1861 2023-05-13 16:56:24.000000 tikapi-3.1.21/tikapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      251 2023-05-13 16:56:24.000000 tikapi-3.1.21/tikapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-13 16:56:24.000000 tikapi-3.1.21/tikapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-07-07 14:30:05.000000 tikapi-3.1.21/tikapi.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        9 2023-05-13 16:56:24.000000 tikapi-3.1.21/tikapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-13 16:56:24.000000 tikapi-3.1.21/tikapi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-09 14:15:02.109197 tikapi-3.1.22/
+-rw-rw-rw-   0        0        0       67 2022-12-07 21:27:40.000000 tikapi-3.1.22/MANIFEST.in
+-rw-rw-rw-   0        0        0     1861 2023-06-09 14:15:02.109197 tikapi-3.1.22/PKG-INFO
+-rw-rw-rw-   0        0        0     1106 2022-08-29 11:23:45.000000 tikapi-3.1.22/README.md
+-rw-rw-rw-   0        0        0      121 2023-06-09 14:15:02.109197 tikapi-3.1.22/setup.cfg
+-rw-rw-rw-   0        0        0      704 2023-06-09 14:14:47.000000 tikapi-3.1.22/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 14:15:02.103197 tikapi-3.1.22/tikapi/
+-rw-rw-rw-   0        0        0     3172 2022-12-07 20:49:56.000000 tikapi-3.1.22/tikapi/__init__.py
+-rw-rw-rw-   0        0        0    64951 2023-06-09 14:13:46.000000 tikapi-3.1.22/tikapi/api.py
+drwxrwxrwx   0        0        0        0 2023-06-09 14:15:02.108198 tikapi-3.1.22/tikapi.egg-info/
+-rw-rw-rw-   0        0        0     1861 2023-06-09 14:15:02.000000 tikapi-3.1.22/tikapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      251 2023-06-09 14:15:02.000000 tikapi-3.1.22/tikapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 14:15:02.000000 tikapi-3.1.22/tikapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-07-07 14:30:05.000000 tikapi-3.1.22/tikapi.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        9 2023-06-09 14:15:02.000000 tikapi-3.1.22/tikapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-09 14:15:02.000000 tikapi-3.1.22/tikapi.egg-info/top_level.txt
```

### Comparing `tikapi-3.1.21/PKG-INFO` & `tikapi-3.1.22/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tikapi
-Version: 3.1.21
+Version: 3.1.22
 Summary: TikAPI | TikTok Unofficial API
 Home-page: https://www.tikapi.io
 Author: TikAPI
 Author-email: contact@tikapi.io
 License: TikAPI
 Description: # Unofficial TikTok API <img src='https://img.shields.io/npm/v/tikapi'> <img src='https://img.shields.io/pypi/v/tikapi'>
```

### Comparing `tikapi-3.1.21/README.md` & `tikapi-3.1.22/README.md`

 * *Files identical despite different names*

### Comparing `tikapi-3.1.21/setup.py` & `tikapi-3.1.22/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 INSTALL_REQUIRES = [
    'requests',
 ]
 
 setup(
     name='tikapi',
-    version='3.1.21',
+    version='3.1.22',
     description='TikAPI | TikTok Unofficial API',
     long_description_content_type="text/markdown",
     long_description=open("README.md", "r", encoding="utf-8").read(),
     license='TikAPI',
     author='TikAPI',
     author_email='contact@tikapi.io',
     url='https://www.tikapi.io',
```

### Comparing `tikapi-3.1.21/tikapi/__init__.py` & `tikapi-3.1.22/tikapi/__init__.py`

 * *Files identical despite different names*

### Comparing `tikapi-3.1.21/tikapi/api.py` & `tikapi-3.1.22/tikapi/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -436,133 +436,133 @@
 	
 	Rests.BaseClass = BaseClass
 	class Public(Rests.BaseClass):
 		'''
 			Public Endpoints Category 
 		'''
 
-		__options__ = {"headers":{},"params":{"country":{"type":"string","validate":"^[a-z]{2}$","help":"You can optionally choose the proxy country from where the request\n\t\t\t\t\tis being sent by providing an ISO Code (e.g us, ca, gb) — 200+ countries supported","location":"query","example":"us"}},"values":{},"$other":{"openapi":{"fields":{"tags":["Public"],"parameters":[],"responses":{}}}}}
+		__options__ = {"headers":{},"params":{"country":{"type":"string","validate":"^[a-z]{2}$","help":"You can optionally choose the proxy country from where the request\n\t\t\t\t\tis being sent by providing an ISO Code (e.g us, ca, gb) — 200+ countries supported","location":"query","example":"us"},"session_id":{"type":"number","max":100,"example":0,"help":"(Optional) Longer sessions. The cookies and IP are preserved through different requests for a longer amount of time. You should include this in order to get different posts on every request."}},"values":{},"$other":{"openapi":{"fields":{"tags":["Public"],"parameters":[],"responses":{}}}}}
 
-		def __new__(self, country: str = None, **values) -> 'Public':
+		def __new__(self, country: str = None, session_id: int = None, **values) -> 'Public':
 			'''
 				Initialize new 'Public' instance with default values & options
 			'''
-			return super().__new__(self, country=country, **values)
+			return super().__new__(self, country=country, session_id=session_id, **values)
 
 		@classmethod
-		def set(self, country: str = None, **values) -> 'Public':
+		def set(self, country: str = None, session_id: int = None, **values) -> 'Public':
 			'''
 				Method is only available for the root category.
 				Set default values & options for 'Public'
 			'''
-			return super().set(country=country, **values)
+			return super().set(country=country, session_id=session_id, **values)
 	
 		@classmethod
-		def check(cls, username: str = None, user_id: str = None, country: str = None, **otherParams) -> APIResponse:
+		def check(cls, username: str = None, user_id: str = None, country: str = None, session_id: int = None, **otherParams) -> APIResponse:
 			'''
 				Get a user's profile information 
 			'''
 			
-			return wrap({"path":"/public/check","help":"Get a user's profile information","comment":"Get profile information and statistics from a username.","params":{"username":{"help":"The TikTok user username","validate":"^([a-zA-Z0-9_.]+|https?://vm.tiktok.com/[a-zA-Z0-9]+/?)$","type":"string","example":"lilyachty"},"user_id":{"help":"Optionally you can get the profile information using the user_id parameter.","type":"string","validate":"^[0-9]+$"}},"$other":{"openapi":{"hideParams":["user_id"],"showExamplesInCode":["username"]}},"method":"GET"}, cls.__get_options__(), "Public.check")(username=username, user_id=user_id, country=country, **otherParams)
+			return wrap({"path":"/public/check","help":"Get a user's profile information","comment":"Get profile information and statistics from a username.","params":{"username":{"help":"The TikTok user username","validate":"^([a-zA-Z0-9_.]+|https?://vm.tiktok.com/[a-zA-Z0-9]+/?)$","type":"string","example":"lilyachty"},"user_id":{"help":"Optionally you can get the profile information using the user_id parameter.","type":"string","validate":"^[0-9]+$"}},"$other":{"openapi":{"hideParams":["user_id","session_id"],"showExamplesInCode":["username"]}},"method":"GET"}, cls.__get_options__(), "Public.check")(username=username, user_id=user_id, country=country, session_id=session_id, **otherParams)
 	
 		@classmethod
-		def posts(cls, secUid: str = None, count: int = Default(30), cursor: str = None, country: str = None, **otherParams) -> APIResponse:
+		def posts(cls, secUid: str = None, count: int = Default(30), cursor: str = None, country: str = None, session_id: int = None, **otherParams) -> APIResponse:
 			'''
 				Get a user's feed posts 
 			'''
 			count = None if count is cls.posts.__defaults__[1] else count
-			return wrap({"help":"Get a user's feed posts","path":"/public/posts","comment":"<a target=\"_blank\" href='https://helpdesk.tikapi.io/portal/en/kb/articles/how-to-download-tiktok-videos'>\nLearn more about downloading videos</a>\n\n","params":{"secUid":{"validate":"^(.*?){30,}$","help":"The TikTok user secUid. You can get this from the <a href='#tag/Public/operation/public.check'>Get profile information</a> endpoint using the username.","type":"string","example":"MS4wLjABAAAAsHntXC3s0AvxcecggxsoVa4eAiT8OVafVZ4OQXxy-9htpnUi0sOYSr0kGGD1Loud","required":True},"count":{"example":30,"default":30,"max":30,"type":"number","help":"Maximum amount of items for one request","validate":"^[0-9]{1,2}$"},"cursor":{"help":"The starting point of the items list. Returned in every response, should be included in the next request for iteration.<br><br> *(A simple iteration method is already implemented in the Javascript & Python libraries as seen in the request samples)*","type":"string","validate":"^[0-9]+$"}},"$other":{"openapi":{}},"method":"GET"}, cls.__get_options__(), "Public.posts")(secUid=secUid, count=count, cursor=cursor, country=country, **otherParams)
+			return wrap({"help":"Get a user's feed posts","path":"/public/posts","comment":"<a target=\"_blank\" href='https://helpdesk.tikapi.io/portal/en/kb/articles/how-to-download-tiktok-videos'>\nLearn more about downloading videos</a>\n\n","params":{"secUid":{"validate":"^(.*?){30,}$","help":"The TikTok user secUid. You can get this from the <a href='#tag/Public/operation/public.check'>Get profile information</a> endpoint using the username.","type":"string","example":"MS4wLjABAAAAsHntXC3s0AvxcecggxsoVa4eAiT8OVafVZ4OQXxy-9htpnUi0sOYSr0kGGD1Loud","required":True},"count":{"example":30,"default":30,"max":30,"type":"number","help":"Maximum amount of items for one request","validate":"^[0-9]{1,2}$"},"cursor":{"help":"The starting point of the items list. Returned in every response, should be included in the next request for iteration.<br><br> *(A simple iteration method is already implemented in the Javascript & Python libraries as seen in the request samples)*","type":"string","validate":"^[0-9]+$"}},"$other":{"openapi":{"hideParams":["session_id"]}},"method":"GET"}, cls.__get_options__(), "Public.posts")(secUid=secUid, count=count, cursor=cursor, country=country, session_id=session_id, **otherParams)
 	
 		@classmethod
-		def likes(cls, secUid: str = None, count: int = Default(30), cursor: str = None, country: str = None, **otherParams) -> APIResponse:
+		def likes(cls, secUid: str = None, count: int = Default(30), cursor: str = None, country: str = None, session_id: int = None, **otherParams) -> APIResponse:
 			'''
 				Get a user's liked posts 
 			'''
 			count = None if count is cls.likes.__defaults__[1] else count
-			return wrap({"help":"Get a user's liked posts","path":"/public/likes","comment":"<a target=\"_blank\" href='https://helpdesk.tikapi.io/portal/en/kb/articles/how-to-download-tiktok-videos'>\nLearn more about downloading videos</a>\n\n","params":{"secUid":{"validate":"^(.*?){30,}$","help":"The TikTok user secUid. You can get this from the <a href='#tag/Public/operation/public.check'>Get profile information</a> endpoint using the username.","type":"string","example":"MS4wLjABAAAAsHntXC3s0AvxcecggxsoVa4eAiT8OVafVZ4OQXxy-9htpnUi0sOYSr0kGGD1Loud","required":True},"count":{"example":30,"default":30,"max":30,"type":"number","help":"Maximum amount of items for one request","validate":"^[0-9]{1,2}$"},"cursor":{"help":"The starting point of the items list. Returned in every response, should be included in the next request for iteration.<br><br> *(A simple iteration method is already implemented in the Javascript & Python libraries as seen in the request samples)*","type":"string","validate":"^[0-9]+$"}},"$other":{"openapi":{}},"method":"GET"}, cls.__get_options__(), "Public.likes")(secUid=secUid, count=count, cursor=cursor, country=country, **otherParams)
+			return wrap({"help":"Get a user's liked posts","path":"/public/likes","comment":"<a target=\"_blank\" href='https://helpdesk.tikapi.io/portal/en/kb/articles/how-to-download-tiktok-videos'>\nLearn more about downloading videos</a>\n\n","params":{"secUid":{"validate":"^(.*?){30,}$","help":"The TikTok user secUid. You can get this from the <a href='#tag/Public/operation/public.check'>Get profile information</a> endpoint using the username.","type":"string","example":"MS4wLjABAAAAsHntXC3s0AvxcecggxsoVa4eAiT8OVafVZ4OQXxy-9htpnUi0sOYSr0kGGD1Loud","required":True},"count":{"example":30,"default":30,"max":30,"type":"number","help":"Maximum amount of items for one request","validate":"^[0-9]{1,2}$"},"cursor":{"help":"The starting point of the items list. Returned in every response, should be included in the next request for iteration.<br><br> *(A simple iteration method is already implemented in the Javascript & Python libraries as seen in the request samples)*","type":"string","validate":"^[0-9]+$"}},"$other":{"openapi":{"hideParams":["session_id"]}},"method":"GET"}, cls.__get_options__(), "Public.likes")(secUid=secUid, count=count, cursor=cursor, country=country, session_id=session_id, **otherParams)
 	
 		@classmethod
-		def followersList(cls, secUid: str = None, count: int = Default(30), nextCursor: str = None, country: str = None, **otherParams) -> APIResponse:
+		def followersList(cls, secUid: str = None, count: int = Default(30), nextCursor: str = None, country: str = None, session_id: int = None, **otherParams) -> APIResponse:
 			'''
 				Get a user's followers list 
 			'''
 			count = None if count is cls.followersList.__defaults__[1] else count
-			return wrap({"help":"Get a user's followers list","comment":"Get followers list of any public profile.","path":"/public/followers","params":{"secUid":{"validate":"^(.*?){30,}$","help":"The TikTok user secUid. You can get this from the <a href='#tag/Public/operation/public.check'>Get profile information</a> endpoint using the username.","type":"string","example":"MS4wLjABAAAAsHntXC3s0AvxcecggxsoVa4eAiT8OVafVZ4OQXxy-9htpnUi0sOYSr0kGGD1Loud","required":True},"count":{"example":30,"default":30,"max":30,"type":"number","help":"Maximum amount of items for one request","validate":"^[0-9]{1,2}$"},"nextCursor":{"type":"string","help":"A iteration parameter returned in each response, should be included in the next requests to get the next items."}},"$other":{"openapi":{}},"method":"GET"}, cls.__get_options__(), "Public.followersList")(secUid=secUid, count=count, nextCursor=nextCursor, country=country, **otherParams)
+			return wrap({"help":"Get a user's followers list","comment":"Get followers list of any public profile.","path":"/public/followers","params":{"secUid":{"validate":"^(.*?){30,}$","help":"The TikTok user secUid. You can get this from the <a href='#tag/Public/operation/public.check'>Get profile information</a> endpoint using the username.","type":"string","example":"MS4wLjABAAAAsHntXC3s0AvxcecggxsoVa4eAiT8OVafVZ4OQXxy-9htpnUi0sOYSr0kGGD1Loud","required":True},"count":{"example":30,"default":30,"max":30,"type":"number","help":"Maximum amount of items for one request","validate":"^[0-9]{1,2}$"},"nextCursor":{"type":"string","help":"A iteration parameter returned in each response, should be included in the next requests to get the next items."}},"$other":{"openapi":{"hideParams":["session_id"]}},"method":"GET"}, cls.__get_options__(), "Public.followersList")(secUid=secUid, count=count, nextCursor=nextCursor, country=country, session_id=session_id, **otherParams)
 	
 		@classmethod
-		def followingList(cls, secUid: str = None, count: int = Default(30), nextCursor: str = None, country: str = None, **otherParams) -> APIResponse:
+		def followingList(cls, secUid: str = None, count: int = Default(30), nextCursor: str = None, country: str = None, session_id: int = None, **otherParams) -> APIResponse:
 			'''
 				Get a user's following list 
 			'''
 			count = None if count is cls.followingList.__defaults__[1] else count
-			return wrap({"help":"Get a user's following list","comment":"Get following list of any public profile.","path":"/public/following","params":{"secUid":{"validate":"^(.*?){30,}$","help":"The TikTok user secUid. You can get this from the <a href='#tag/Public/operation/public.check'>Get profile information</a> endpoint using the username.","type":"string","example":"MS4wLjABAAAAsHntXC3s0AvxcecggxsoVa4eAiT8OVafVZ4OQXxy-9htpnUi0sOYSr0kGGD1Loud","required":True},"count":{"example":30,"default":30,"max":30,"type":"number","help":"Maximum amount of items for one request","validate":"^[0-9]{1,2}$"},"nextCursor":{"type":"string","help":"A iteration parameter returned in each response, should be included in the next requests to get the next items."}},"$other":{"openapi":{}},"method":"GET"}, cls.__get_options__(), "Public.followingList")(secUid=secUid, count=count, nextCursor=nextCursor, country=country, **otherParams)
+			return wrap({"help":"Get a user's following list","comment":"Get following list of any public profile.","path":"/public/following","params":{"secUid":{"validate":"^(.*?){30,}$","help":"The TikTok user secUid. You can get this from the <a href='#tag/Public/operation/public.check'>Get profile information</a> endpoint using the username.","type":"string","example":"MS4wLjABAAAAsHntXC3s0AvxcecggxsoVa4eAiT8OVafVZ4OQXxy-9htpnUi0sOYSr0kGGD1Loud","required":True},"count":{"example":30,"default":30,"max":30,"type":"number","help":"Maximum amount of items for one request","validate":"^[0-9]{1,2}$"},"nextCursor":{"type":"string","help":"A iteration parameter returned in each response, should be included in the next requests to get the next items."}},"$other":{"openapi":{"hideParams":["session_id"]}},"method":"GET"}, cls.__get_options__(), "Public.followingList")(secUid=secUid, count=count, nextCursor=nextCursor, country=country, session_id=session_id, **otherParams)
 	
 		@classmethod
-		def explore(cls, count: int = Default(30), session_id: int = None, country: str = None, **otherParams) -> APIResponse:
+		def explore(cls, count: int = Default(30), country: str = None, session_id: int = None, **otherParams) -> APIResponse:
 			'''
 				Get trending posts 
 			'''
 			count = None if count is cls.explore.__defaults__[0] else count
-			return wrap({"help":"Get trending posts","comment":"Get a list of recommended posts from the *For You* section. <br/><a target=\"_blank\" href='https://helpdesk.tikapi.io/portal/en/kb/articles/how-to-download-tiktok-videos'>\nLearn more about downloading videos</a>\n\n","path":"/public/explore","params":{"count":{"example":30,"default":30,"max":30,"type":"number","help":"Maximum amount of items for one request","validate":"^[0-9]{1,2}$"},"session_id":{"type":"number","max":100,"example":0,"help":"Longer sessions. The cookies and IP are preserved through different requests for a longer amount of time. You should include this in order to get different posts on every request."}},"$other":{"openapi":{}},"method":"GET"}, cls.__get_options__(), "Public.explore")(count=count, session_id=session_id, country=country, **otherParams)
+			return wrap({"help":"Get trending posts","comment":"Get a list of recommended posts from the *For You* section. <br/><a target=\"_blank\" href='https://helpdesk.tikapi.io/portal/en/kb/articles/how-to-download-tiktok-videos'>\nLearn more about downloading videos</a>\n\n","path":"/public/explore","params":{"count":{"example":30,"default":30,"max":30,"type":"number","help":"Maximum amount of items for one request","validate":"^[0-9]{1,2}$"}},"$other":{"openapi":{"hideParams":["session_id"]}},"method":"GET"}, cls.__get_options__(), "Public.explore")(count=count, country=country, session_id=session_id, **otherParams)
 	
 		@classmethod
-		def video(cls, id: str = None, country: str = None, **otherParams) -> APIResponse:
+		def video(cls, id: str = None, country: str = None, session_id: int = None, **otherParams) -> APIResponse:
 			'''
 				Get video information 
 			'''
 			
-			return wrap({"path":"/public/video","help":"Get video information","comment":"<a target=\"_blank\" href='https://helpdesk.tikapi.io/portal/en/kb/articles/how-to-download-tiktok-videos'>\nLearn more about downloading videos</a>\n\n","params":{"id":{"help":"The video ID. Can also be a short TikTok link (e.g. vm.tiktok.com/UwU)","type":"string","validate":"^([0-9]+|https?://vm.tiktok.com/[a-zA-Z0-9]+/?)$","required":True,"example":"7109178205151464746"}},"method":"GET"}, cls.__get_options__(), "Public.video")(id=id, country=country, **otherParams)
+			return wrap({"path":"/public/video","help":"Get video information","comment":"<a target=\"_blank\" href='https://helpdesk.tikapi.io/portal/en/kb/articles/how-to-download-tiktok-videos'>\nLearn more about downloading videos</a>\n\n","params":{"id":{"help":"The video ID. Can also be a short TikTok link (e.g. vm.tiktok.com/UwU)","type":"string","validate":"^([0-9]+|https?://vm.tiktok.com/[a-zA-Z0-9]+/?)$","required":True,"example":"7109178205151464746"}},"$other":{"openapi":{"hideParams":["session_id"]}},"method":"GET"}, cls.__get_options__(), "Public.video")(id=id, country=country, session_id=session_id, **otherParams)
 	
 		@classmethod
-		def hashtag(cls, id: str = None, name: str = None, count: int = Default(30), cursor: str = None, country: str = None, **otherParams) -> APIResponse:
+		def hashtag(cls, id: str = None, name: str = None, count: int = Default(30), cursor: str = None, country: str = None, session_id: int = None, **otherParams) -> APIResponse:
 			'''
 				Get hashtag posts 
 			'''
 			count = None if count is cls.hashtag.__defaults__[2] else count
-			return wrap({"help":"Get hashtag posts","comment":"Your first request should be using the hashtag `name` parameter, then the following requests should be using the `id` parameter which you have stored from the first request (returned in response `challengeInfo > challenge > id`). <br/><a target=\"_blank\" href='https://helpdesk.tikapi.io/portal/en/kb/articles/how-to-download-tiktok-videos'>\nLearn more about downloading videos</a>\n\n","path":"/public/hashtag","params":{"id":{"validate":"^([0-9]+|https?://vm.tiktok.com/[a-zA-Z0-9]+/?)$","type":"string","help":"The hashtag ID. Can also be a short TikTok link (e.g. vm.tiktok.com/UwU)","example":"4655293"},"name":{"type":"string","help":"The hashtag name"},"count":{"example":30,"default":30,"max":30,"type":"number","help":"Maximum amount of items for one request","validate":"^[0-9]{1,2}$"},"cursor":{"help":"The starting point of the items list. Returned in every response, should be included in the next request for iteration.<br><br> *(A simple iteration method is already implemented in the Javascript & Python libraries as seen in the request samples)*","type":"string","validate":"^[0-9]+$"}},"$other":{"openapi":{}},"method":"GET"}, cls.__get_options__(), "Public.hashtag")(id=id, name=name, count=count, cursor=cursor, country=country, **otherParams)
+			return wrap({"help":"Get hashtag posts","comment":"Your first request should be using the hashtag `name` parameter, then the following requests should be using the `id` parameter which you have stored from the first request (returned in response `challengeInfo > challenge > id`). <br/><a target=\"_blank\" href='https://helpdesk.tikapi.io/portal/en/kb/articles/how-to-download-tiktok-videos'>\nLearn more about downloading videos</a>\n\n","path":"/public/hashtag","params":{"id":{"validate":"^([0-9]+|https?://vm.tiktok.com/[a-zA-Z0-9]+/?)$","type":"string","help":"The hashtag ID. Can also be a short TikTok link (e.g. vm.tiktok.com/UwU)","example":"4655293"},"name":{"type":"string","help":"The hashtag name"},"count":{"example":30,"default":30,"max":30,"type":"number","help":"Maximum amount of items for one request","validate":"^[0-9]{1,2}$"},"cursor":{"help":"The starting point of the items list. Returned in every response, should be included in the next request for iteration.<br><br> *(A simple iteration method is already implemented in the Javascript & Python libraries as seen in the request samples)*","type":"string","validate":"^[0-9]+$"}},"$other":{"openapi":{"hideParams":["session_id"]}},"method":"GET"}, cls.__get_options__(), "Public.hashtag")(id=id, name=name, count=count, cursor=cursor, country=country, session_id=session_id, **otherParams)
 	
 		@classmethod
-		def music(cls, id: str = None, count: int = Default(30), cursor: str = None, country: str = None, **otherParams) -> APIResponse:
+		def music(cls, id: str = None, count: int = Default(30), cursor: str = None, country: str = None, session_id: int = None, **otherParams) -> APIResponse:
 			'''
 				Get music posts 
 			'''
 			count = None if count is cls.music.__defaults__[1] else count
-			return wrap({"help":"Get music posts","comment":"Get a list of posts that are using this music. <br/><a target=\"_blank\" href='https://helpdesk.tikapi.io/portal/en/kb/articles/how-to-download-tiktok-videos'>\nLearn more about downloading videos</a>\n\n","path":"/public/music","params":{"id":{"validate":"^([0-9]+|https?://vm.tiktok.com/[a-zA-Z0-9]+/?)$","type":"string","help":"The music ID. Can also be a short TikTok link (e.g. vm.tiktok.com/UwU)","required":True,"example":"28459463"},"count":{"example":30,"default":30,"max":30,"type":"number","help":"Maximum amount of items for one request","validate":"^[0-9]{1,2}$"},"cursor":{"help":"The starting point of the items list. Returned in every response, should be included in the next request for iteration.<br><br> *(A simple iteration method is already implemented in the Javascript & Python libraries as seen in the request samples)*","type":"string","validate":"^[0-9]+$"}},"$other":{"openapi":{}},"method":"GET"}, cls.__get_options__(), "Public.music")(id=id, count=count, cursor=cursor, country=country, **otherParams)
+			return wrap({"help":"Get music posts","comment":"Get a list of posts that are using this music. <br/><a target=\"_blank\" href='https://helpdesk.tikapi.io/portal/en/kb/articles/how-to-download-tiktok-videos'>\nLearn more about downloading videos</a>\n\n","path":"/public/music","params":{"id":{"validate":"^([0-9]+|https?://vm.tiktok.com/[a-zA-Z0-9]+/?)$","type":"string","help":"The music ID. Can also be a short TikTok link (e.g. vm.tiktok.com/UwU)","required":True,"example":"28459463"},"count":{"example":30,"default":30,"max":30,"type":"number","help":"Maximum amount of items for one request","validate":"^[0-9]{1,2}$"},"cursor":{"help":"The starting point of the items list. Returned in every response, should be included in the next request for iteration.<br><br> *(A simple iteration method is already implemented in the Javascript & Python libraries as seen in the request samples)*","type":"string","validate":"^[0-9]+$"}},"$other":{"openapi":{"hideParams":["session_id"]}},"method":"GET"}, cls.__get_options__(), "Public.music")(id=id, count=count, cursor=cursor, country=country, session_id=session_id, **otherParams)
 	
 		@classmethod
-		def musicInfo(cls, id: str = None, country: str = None, **otherParams) -> APIResponse:
+		def musicInfo(cls, id: str = None, country: str = None, session_id: int = None, **otherParams) -> APIResponse:
 			'''
 				Get music information 
 			'''
 			
-			return wrap({"help":"Get music information","path":"/public/music/info","params":{"id":{"validate":"^([0-9]+|https?://vm.tiktok.com/[a-zA-Z0-9]+/?)$","type":"string","help":"The music ID. Can also be a short TikTok link (e.g. vm.tiktok.com/UwU)","required":True,"example":"28459463"}},"method":"GET"}, cls.__get_options__(), "Public.musicInfo")(id=id, country=country, **otherParams)
+			return wrap({"help":"Get music information","path":"/public/music/info","params":{"id":{"validate":"^([0-9]+|https?://vm.tiktok.com/[a-zA-Z0-9]+/?)$","type":"string","help":"The music ID. Can also be a short TikTok link (e.g. vm.tiktok.com/UwU)","required":True,"example":"28459463"}},"$other":{"openapi":{"hideParams":["session_id"]}},"method":"GET"}, cls.__get_options__(), "Public.musicInfo")(id=id, country=country, session_id=session_id, **otherParams)
 	
 		@classmethod
-		def discover(cls, category: str = None, count: int = Default(30), offset: int = None, country: str = None, **otherParams) -> APIResponse:
+		def discover(cls, category: str = None, count: int = Default(30), offset: int = None, country: str = None, session_id: int = None, **otherParams) -> APIResponse:
 			'''
 				Discover users, music, hashtags 
 			'''
 			count = None if count is cls.discover.__defaults__[1] else count
-			return wrap({"help":"Discover users, music, hashtags","comment":"Get popular users, music or hashtag. You can also include *Account Key* to show personalized results for the user.","path":"/public/discover/{category}","params":{"category":{"help":"The discover category","example":"users","in":["users","music","hashtag"],"location":"path","type":"string","required":True},"count":{"example":30,"default":30,"max":30,"type":"number","help":"Maximum amount of items for one request","validate":"^[0-9]{1,2}$"},"offset":{"help":"The starting offset of items list. Returned in every response, should be included in the next request for iteration.<br><br> *(A simple iteration method is already implemented in the Javascript & Python libraries as seen in the request samples)*","type":"number","validate":"^[0-9]+$"}},"$other":{"openapi":{}},"method":"GET"}, cls.__get_options__(), "Public.discover")(category=category, count=count, offset=offset, country=country, **otherParams)
+			return wrap({"help":"Discover users, music, hashtags","comment":"Get popular users, music or hashtag. You can also include *Account Key* to show personalized results for the user.","path":"/public/discover/{category}","params":{"category":{"help":"The discover category","example":"users","in":["users","music","hashtag"],"location":"path","type":"string","required":True},"count":{"example":30,"default":30,"max":30,"type":"number","help":"Maximum amount of items for one request","validate":"^[0-9]{1,2}$"},"offset":{"help":"The starting offset of items list. Returned in every response, should be included in the next request for iteration.<br><br> *(A simple iteration method is already implemented in the Javascript & Python libraries as seen in the request samples)*","type":"number","validate":"^[0-9]+$"}},"$other":{"openapi":{"hideParams":["session_id"]}},"method":"GET"}, cls.__get_options__(), "Public.discover")(category=category, count=count, offset=offset, country=country, session_id=session_id, **otherParams)
 	
 		@classmethod
-		def discoverKeyword(cls, keyword: str = None, country: str = None, **otherParams) -> APIResponse:
+		def discoverKeyword(cls, keyword: str = None, country: str = None, session_id: int = None, **otherParams) -> APIResponse:
 			'''
 				Discover by keyword 
 			'''
 			
-			return wrap({"help":"Discover by keyword","comment":"Get popular posts, users, music or hashtags from a keyword. <br><br>Limited to only a few items. If you want more, try using the <a href='#tag/Public/operation/public.search'>Search</a> endpoint instead.","path":"/public/discover/keyword","params":{"keyword":{"required":True,"example":"lilyachty","type":"string"}},"method":"GET"}, cls.__get_options__(), "Public.discoverKeyword")(keyword=keyword, country=country, **otherParams)
+			return wrap({"help":"Discover by keyword","comment":"Get popular posts, users, music or hashtags from a keyword. <br><br>Limited to only a few items. If you want more, try using the <a href='#tag/Public/operation/public.search'>Search</a> endpoint instead.","path":"/public/discover/keyword","params":{"keyword":{"required":True,"example":"lilyachty","type":"string"}},"$other":{"openapi":{"hideParams":["session_id"]}},"method":"GET"}, cls.__get_options__(), "Public.discoverKeyword")(keyword=keyword, country=country, session_id=session_id, **otherParams)
 	
 		@classmethod
-		def search(cls, category: str = None, query: str = None, cursor: int = None, session_id: int = None, country: str = None, **otherParams) -> APIResponse:
+		def search(cls, category: str = None, query: str = None, session_id: int = None, cursor: int = None, country: str = None, **otherParams) -> APIResponse:
 			'''
 				Search 
 			'''
 			
-			return wrap({"help":"Search","comment":"Search anything, users, videos, or get keyword autocomplete suggestions. <br/><a target=\"_blank\" href='https://helpdesk.tikapi.io/portal/en/kb/articles/how-to-download-tiktok-videos'>\nLearn more about downloading videos</a>\n\n","path":"/public/search/{category}","params":{"category":{"help":"The search category","in":["general","users","videos","autocomplete"],"required":True,"type":"string","example":"general","location":"path"},"query":{"type":"string","example":"lilyachty","required":True,"help":"The search keyword"},"cursor":{"help":"The starting offset of items list. Returned in every response, should be included in the next request for iteration.<br><br> *(A simple iteration method is already implemented in the Javascript & Python libraries as seen in the request samples)*","type":"number","validate":"^[0-9]+$"},"session_id":{"type":"number","max":100,"example":0,"help":"The cookies and IP are preserved through different requests for a longer amount of time. You should use this if you want to keep the search suggestions the same."}},"$other":{"openapi":{}},"method":"GET"}, cls.__get_options__(), "Public.search")(category=category, query=query, cursor=cursor, session_id=session_id, country=country, **otherParams)
+			return wrap({"help":"Search","comment":"Search anything, users, videos, or get keyword autocomplete suggestions. <br/><a target=\"_blank\" href='https://helpdesk.tikapi.io/portal/en/kb/articles/how-to-download-tiktok-videos'>\nLearn more about downloading videos</a>\n\n","path":"/public/search/{category}","params":{"category":{"help":"The search category","in":["general","users","videos","autocomplete"],"required":True,"type":"string","example":"general","location":"path"},"query":{"type":"string","example":"lilyachty","required":True,"help":"The search keyword"},"cursor":{"help":"The starting offset of items list. Returned in every response, should be included in the next request for iteration.<br><br> *(A simple iteration method is already implemented in the Javascript & Python libraries as seen in the request samples)*","type":"number","validate":"^[0-9]+$"},"session_id":{"type":"number","max":100,"example":0,"help":"The cookies and IP are preserved through different requests for a longer amount of time. You should use this if you want to keep the search suggestions the same."}},"$other":{"openapi":{"hideParams":["session_id"]}},"method":"GET"}, cls.__get_options__(), "Public.search")(category=category, query=query, session_id=session_id, cursor=cursor, country=country, **otherParams)
 	
 	Rests.Public = Public
 	class UserPostsComments(Rests.BaseClass):
 		'''
 			Comments Endpoints Category 
 		'''
```

### Comparing `tikapi-3.1.21/tikapi.egg-info/PKG-INFO` & `tikapi-3.1.22/tikapi.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tikapi
-Version: 3.1.21
+Version: 3.1.22
 Summary: TikAPI | TikTok Unofficial API
 Home-page: https://www.tikapi.io
 Author: TikAPI
 Author-email: contact@tikapi.io
 License: TikAPI
 Description: # Unofficial TikTok API <img src='https://img.shields.io/npm/v/tikapi'> <img src='https://img.shields.io/pypi/v/tikapi'>
```

