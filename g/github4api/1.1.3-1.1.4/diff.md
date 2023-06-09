# Comparing `tmp/github4api-1.1.3.tar.gz` & `tmp/github4api-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "github4api-1.1.3.tar", last modified: Thu Jun  8 17:25:05 2023, max compression
+gzip compressed data, was "github4api-1.1.4.tar", last modified: Fri Jun  9 12:48:46 2023, max compression
```

## Comparing `github4api-1.1.3.tar` & `github4api-1.1.4.tar`

### file list

```diff
@@ -1,23 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-06-08 17:25:05.333729 github4api-1.1.3/
--rw-rw-rw-   0        0        0       55 2023-06-07 22:00:04.000000 github4api-1.1.3/MANIFEST.in
--rw-rw-rw-   0        0        0     6954 2023-06-08 17:25:05.332727 github4api-1.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     6008 2023-06-08 17:21:02.000000 github4api-1.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-08 17:25:05.321921 github4api-1.1.3/github4api/
--rw-rw-rw-   0        0        0      286 2023-06-07 22:45:44.000000 github4api-1.1.3/github4api/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-08 17:25:05.328728 github4api-1.1.3/github4api/request_handler/
--rw-rw-rw-   0        0        0      858 2023-06-07 21:12:08.000000 github4api-1.1.3/github4api/request_handler/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-08 17:25:05.329727 github4api-1.1.3/github4api/scraper/
--rw-rw-rw-   0        0        0     4810 2023-06-08 17:12:36.000000 github4api-1.1.3/github4api/scraper/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-08 17:25:05.330728 github4api-1.1.3/github4api/user_handler/
--rw-rw-rw-   0        0        0      613 2023-06-08 17:05:36.000000 github4api-1.1.3/github4api/user_handler/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-08 17:25:05.327727 github4api-1.1.3/github4api.egg-info/
--rw-rw-rw-   0        0        0     6954 2023-06-08 17:25:05.000000 github4api-1.1.3/github4api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      361 2023-06-08 17:25:05.000000 github4api-1.1.3/github4api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-08 17:25:05.000000 github4api-1.1.3/github4api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       77 2023-06-08 17:25:05.000000 github4api-1.1.3/github4api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-06-08 17:25:05.000000 github4api-1.1.3/github4api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      424 2023-06-08 16:42:31.000000 github4api-1.1.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-08 17:25:05.333729 github4api-1.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1337 2023-06-08 16:42:16.000000 github4api-1.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-08 17:25:05.331727 github4api-1.1.3/tests/
--rw-rw-rw-   0        0        0      585 2023-06-08 16:08:56.000000 github4api-1.1.3/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 12:48:46.041315 github4api-1.1.4/
+-rw-rw-rw-   0        0        0     1092 2023-06-08 18:05:26.000000 github4api-1.1.4/LICENSE
+-rw-rw-rw-   0        0        0       55 2023-06-07 22:00:04.000000 github4api-1.1.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     8449 2023-06-09 12:48:46.041315 github4api-1.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     7423 2023-06-09 12:45:58.000000 github4api-1.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-09 12:48:46.028234 github4api-1.1.4/github4api/
+-rw-rw-rw-   0        0        0      245 2023-06-08 18:44:02.000000 github4api-1.1.4/github4api/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 12:48:46.035236 github4api-1.1.4/github4api/handlers/
+-rw-rw-rw-   0        0        0       82 2023-06-08 18:36:28.000000 github4api-1.1.4/github4api/handlers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 12:48:46.036233 github4api-1.1.4/github4api/handlers/request_handler/
+-rw-rw-rw-   0        0        0      941 2023-06-08 18:55:53.000000 github4api-1.1.4/github4api/handlers/request_handler/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 12:48:46.037313 github4api-1.1.4/github4api/handlers/user_handler/
+-rw-rw-rw-   0        0        0      792 2023-06-09 11:56:55.000000 github4api-1.1.4/github4api/handlers/user_handler/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 12:48:46.038314 github4api-1.1.4/github4api/scraper/
+-rw-rw-rw-   0        0        0     7007 2023-06-09 12:19:47.000000 github4api-1.1.4/github4api/scraper/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 12:48:46.034234 github4api-1.1.4/github4api.egg-info/
+-rw-rw-rw-   0        0        0     8449 2023-06-09 12:48:45.000000 github4api-1.1.4/github4api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      419 2023-06-09 12:48:45.000000 github4api-1.1.4/github4api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 12:48:45.000000 github4api-1.1.4/github4api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       77 2023-06-09 12:48:45.000000 github4api-1.1.4/github4api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-06-09 12:48:45.000000 github4api-1.1.4/github4api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      424 2023-06-08 18:15:41.000000 github4api-1.1.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-09 12:48:46.041315 github4api-1.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1337 2023-06-08 18:15:23.000000 github4api-1.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 12:48:46.039315 github4api-1.1.4/tests/
+-rw-rw-rw-   0        0        0      585 2023-06-08 16:08:56.000000 github4api-1.1.4/tests/__init__.py
```

### Comparing `github4api-1.1.3/PKG-INFO` & `github4api-1.1.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: github4api
-Version: 1.1.3
+Version: 1.1.4
 Summary: A python Package API for getting Github Users Information.
 Author: Shervin Badanara (shervinbdndev)
 Author-email: shervin2234@gmail.com
 Maintainer: Shervin Badanara
 License: MIT
 Project-URL: Source, https://www.github.com/shervinbdndev/github4api/
 Keywords: python,api,github,github_api,github_package
@@ -13,18 +13,20 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
+License-File: LICENSE
 
 
 <h1 align='center' style="font-size:5rem"><b>github4api</b></h1>
-<p align='center'><b>Version 1.1.3</b></p>
+<p align='center'><b>Version 1.1.4</b></p>
+<p align='center'><b>Written with Python 3.11.3</b></p>
 <div align="center">
     <div align="center">
         <img src="https://img.shields.io/github/license/shervinbdndev/github4api.svg"></img>
     </div>
     <img src="https://img.shields.io/github/forks/shervinbdndev/github4api.svg"></img>
     <img src="https://img.shields.io/github/stars/shervinbdndev/github4api.svg"></img>
     <img src="https://img.shields.io/github/watchers/shervinbdndev/github4api.svg"></img>
@@ -53,22 +55,31 @@
 <img src="https://img.shields.io/badge/Ubuntu-E95420?style=for-the-badge&logo=ubuntu&logoColor=white"></img>
 <img src="https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white"></img>
 <img src="https://img.shields.io/badge/Stack_Overflow-FE7A16?style=for-the-badge&logo=stack-overflow&logoColor=white"></img>
 <img src="https://img.shields.io/badge/Reddit-FF4500?style=for-the-badge&logo=reddit&logoColor=white"></img>
 
 <br>
 <h2 align='center'><b>WorkSpace</h2>
-<img src="https://img.shields.io/badge/Intel-Core_i5_10700K-0071C5?style=for-the-badge&logo=intel&logoColor=white"></img>
+<img src="https://img.shields.io/badge/Intel-Core_i5_10600K-0071C5?style=for-the-badge&logo=intel&logoColor=white"></img>
 <img src="https://img.shields.io/badge/NVIDIA-RTX2060 OC-76B900?style=for-the-badge&logo=nvidia&logoColor=white"></img>
 <img src="https://img.shields.io/badge/Windows11-0078D6?style=for-the-badge&logo=windows&logoColor=white"></img>
 
 
 <hr>
 
 <br><br><br>
+
+<h1 align='center' style='color:#ff0080; font-size:3rem;'><b>! Warning !</h1>
+
+
+- ## This package uses ``` ExceptionGroup ``` to handle exceptions.
+- ## You have to use python [3.11](https://www.python.org/downloads/) or above to be able to use this package.
+
+
+<br><br><br>
 <h1 align='left'><b>Update Your Interpreter</b></h1>
 
 # Windows / CMD
 
 ```python
 py -m pip install --upgrade pip
 ```
@@ -114,16 +125,16 @@
 <br><br><br>
 <h1 align='left'><b>Usage</b></h1>
 
 <br>
 
 ```python
 from github4api.scraper import Scrape # Scraper Class
-from github4api.user_handler import UserHandler # User Handler Class
-from github4api.request_handler import RequestHandler # Request Handler Class
+from github4api.handlers.user_handler import UserHandler # User Handler Class
+from github4api.handlers.request_handler import RequestHandler # Request Handler Class
 
 
 def main():
 
     # UserHandler serializes the value you given to the username param
     # RequestHandler gets the Serialized data then sends a GET request to github servers and saves the page content in request variable
 
@@ -158,21 +169,21 @@
 
 ```
 
 <br><br><br>
 
 # New Changes on Version 1.1.3
 
-- ### Now you can Access Users Repositories Names
+- ### Now you can Access User's Repositories Names
 
 ```py
 
 from github4api.scraper import Scrape
-from github4api.user_handler import UserHandler
-from github4api.request_handler import RequestHandler
+from github4api.handlers.user_handler import UserHandler
+from github4api.handlers.request_handler import RequestHandler
 
 
 
 
 def main():
     request: RequestHandler = RequestHandler(
         url=UserHandler(username='shervinbdndev').serialize(get_repos=True), # for accessing the repositories you should set get_repos param to True
@@ -199,12 +210,59 @@
 if (__name__ == "__main__"):
     main()
 
 
 
 ```
 
+<br><br><br>
+
+# New Changes on Version 1.1.4
+
+## Now you can Access
+
+- ### User's Total Stars Given
+- ### User's Profile Picture Url
+- ### Check Repository Star Count
+
+```python
+
+from github4api.scraper import Scrape
+from github4api.handlers.user_handler import UserHandler
+from github4api.handlers.request_handler import RequestHandler
+
+
+
+def main():
+    request: RequestHandler = RequestHandler(
+        url=UserHandler(username='shervinbdndev').serialize()
+    ).sendGetRequest(content=True)
+    
+    scraper: Scrape = Scrape(data=request)
+    
+    scraper.startApi(log=False)
+    
+    print(scraper.totalStarsGiven) # total stars given
+    
+    print(scraper.profilePictureUrl) # profile picture url
+
+    # now using this new method you lets you check users repository's star count
+
+    print(scraper.checkRepositoryStars(
+        username='shervinbdndev', # user's username
+        repo_name='Quizino', # repository's name
+    ))
+
+
+
+
+if (__name__ == "__main__"):
+    main()
+
+```
+
+<br>
 
 <h1 align='left'>Enjoy :)</h1>
 
 <br>
 <h3><b>Package Uploaded in PYPI :<a href="https://pypi.org/project/github4api/">Here</a></b></h3>
```

### Comparing `github4api-1.1.3/README.md` & `github4api-1.1.4/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 <h1 align='center' style="font-size:5rem"><b>github4api</b></h1>
-<p align='center'><b>Version 1.1.3</b></p>
+<p align='center'><b>Version 1.1.4</b></p>
+<p align='center'><b>Written with Python 3.11.3</b></p>
 <div align="center">
     <div align="center">
         <img src="https://img.shields.io/github/license/shervinbdndev/github4api.svg"></img>
     </div>
     <img src="https://img.shields.io/github/forks/shervinbdndev/github4api.svg"></img>
     <img src="https://img.shields.io/github/stars/shervinbdndev/github4api.svg"></img>
     <img src="https://img.shields.io/github/watchers/shervinbdndev/github4api.svg"></img>
@@ -32,22 +33,31 @@
 <img src="https://img.shields.io/badge/Ubuntu-E95420?style=for-the-badge&logo=ubuntu&logoColor=white"></img>
 <img src="https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white"></img>
 <img src="https://img.shields.io/badge/Stack_Overflow-FE7A16?style=for-the-badge&logo=stack-overflow&logoColor=white"></img>
 <img src="https://img.shields.io/badge/Reddit-FF4500?style=for-the-badge&logo=reddit&logoColor=white"></img>
 
 <br>
 <h2 align='center'><b>WorkSpace</h2>
-<img src="https://img.shields.io/badge/Intel-Core_i5_10700K-0071C5?style=for-the-badge&logo=intel&logoColor=white"></img>
+<img src="https://img.shields.io/badge/Intel-Core_i5_10600K-0071C5?style=for-the-badge&logo=intel&logoColor=white"></img>
 <img src="https://img.shields.io/badge/NVIDIA-RTX2060 OC-76B900?style=for-the-badge&logo=nvidia&logoColor=white"></img>
 <img src="https://img.shields.io/badge/Windows11-0078D6?style=for-the-badge&logo=windows&logoColor=white"></img>
 
 
 <hr>
 
 <br><br><br>
+
+<h1 align='center' style='color:#ff0080; font-size:3rem;'><b>! Warning !</h1>
+
+
+- ## This package uses ``` ExceptionGroup ``` to handle exceptions.
+- ## You have to use python [3.11](https://www.python.org/downloads/) or above to be able to use this package.
+
+
+<br><br><br>
 <h1 align='left'><b>Update Your Interpreter</b></h1>
 
 # Windows / CMD
 
 ```python
 py -m pip install --upgrade pip
 ```
@@ -93,16 +103,16 @@
 <br><br><br>
 <h1 align='left'><b>Usage</b></h1>
 
 <br>
 
 ```python
 from github4api.scraper import Scrape # Scraper Class
-from github4api.user_handler import UserHandler # User Handler Class
-from github4api.request_handler import RequestHandler # Request Handler Class
+from github4api.handlers.user_handler import UserHandler # User Handler Class
+from github4api.handlers.request_handler import RequestHandler # Request Handler Class
 
 
 def main():
 
     # UserHandler serializes the value you given to the username param
     # RequestHandler gets the Serialized data then sends a GET request to github servers and saves the page content in request variable
 
@@ -137,21 +147,21 @@
 
 ```
 
 <br><br><br>
 
 # New Changes on Version 1.1.3
 
-- ### Now you can Access Users Repositories Names
+- ### Now you can Access User's Repositories Names
 
 ```py
 
 from github4api.scraper import Scrape
-from github4api.user_handler import UserHandler
-from github4api.request_handler import RequestHandler
+from github4api.handlers.user_handler import UserHandler
+from github4api.handlers.request_handler import RequestHandler
 
 
 
 
 def main():
     request: RequestHandler = RequestHandler(
         url=UserHandler(username='shervinbdndev').serialize(get_repos=True), # for accessing the repositories you should set get_repos param to True
@@ -178,12 +188,59 @@
 if (__name__ == "__main__"):
     main()
 
 
 
 ```
 
+<br><br><br>
+
+# New Changes on Version 1.1.4
+
+## Now you can Access
+
+- ### User's Total Stars Given
+- ### User's Profile Picture Url
+- ### Check Repository Star Count
+
+```python
+
+from github4api.scraper import Scrape
+from github4api.handlers.user_handler import UserHandler
+from github4api.handlers.request_handler import RequestHandler
+
+
+
+def main():
+    request: RequestHandler = RequestHandler(
+        url=UserHandler(username='shervinbdndev').serialize()
+    ).sendGetRequest(content=True)
+    
+    scraper: Scrape = Scrape(data=request)
+    
+    scraper.startApi(log=False)
+    
+    print(scraper.totalStarsGiven) # total stars given
+    
+    print(scraper.profilePictureUrl) # profile picture url
+
+    # now using this new method you lets you check users repository's star count
+
+    print(scraper.checkRepositoryStars(
+        username='shervinbdndev', # user's username
+        repo_name='Quizino', # repository's name
+    ))
+
+
+
+
+if (__name__ == "__main__"):
+    main()
+
+```
+
+<br>
 
 <h1 align='left'>Enjoy :)</h1>
 
 <br>
 <h3><b>Package Uploaded in PYPI :<a href="https://pypi.org/project/github4api/">Here</a></b></h3>
```

### Comparing `github4api-1.1.3/github4api/request_handler/__init__.py` & `github4api-1.1.4/github4api/handlers/request_handler/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,17 +16,21 @@
 
 
 class RequestHandler:
     def __init__(self: Self, url: str) -> Literal[None]:
         self.__url = url
         self.__data = None
         
+    @property
+    def url(self: Self) -> str:
+        return self.__url
+        
     def sendGetRequest(self: Self, content: bool = False) -> Union[int, bytes, Literal[None]]:
         try:
-            self.__data = requests.get(url=self.__url)
+            self.__data = requests.get(url=self.url)
             
         except* requests.ConnectionError as ce:
             raise ce.__doc__
         
         except* requests.RequestException as re:
             raise re.__doc__
```

### Comparing `github4api-1.1.3/github4api/scraper/__init__.py` & `github4api-1.1.4/github4api/scraper/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 if (__debug__):
     try:
         import re
+        import sys
         import bs4
         from colorama.ansi import Fore
         from colorama.initialise import init
         from typing import Self, Literal, Any
-        from ..request_handler import RequestHandler
+        from ..handlers.user_handler import UserHandler
+        from ..handlers.request_handler import RequestHandler
     
     except* ModuleNotFoundError as mnfe:
         raise mnfe.__doc__
     
     except* ImportError as ie:
         raise ie.__doc__
     
@@ -123,37 +125,88 @@
                 'class': 'Counter',
                 'data-view-component': 'true',
             }
         ).text
         
         return self.json_data['totalRepositories']
     
+    @property
+    def totalStarsGiven(self: Self) -> int:
+        self.__json_data['totalStarsGiven'] = bs4.BeautifulSoup(
+            markup=self.__data,
+            features='html5lib',
+        ).find(
+            name='svg',
+            attrs={
+                'class': 'octicon octicon-star UnderlineNav-octicon hide-sm',
+            }
+        ).find_next(
+            name='span',
+        ).get_text()
+        
+        return self.json_data['totalStarsGiven']
+    
     def repositoriesNames(self: Self, username: str, ftl: bool = False) -> list[str]:
         names: list = []
         
         for element in bs4.BeautifulSoup(markup=self.__data, features='html5lib').find(name='h3', attrs={'class': 'wb-break-all'}).find_all_next(name='a', attrs={'itemprop': 'name codeRepository'}):
             names.append(str(element).replace('href', '').replace('itemprop="name codeRepository', '').replace(f'<a ="/{username}/', '').replace('</a>', '').replace('">', '').replace('"', '').split(sep=' ')[0])
         
         self.json_data['repositoriesNames'] = names
         
         if (ftl):
             return names[::-1]
         return names
+    
+    def checkRepositoryStars(self: Self, username: str, repo_name: str) -> int:
+        self.__json_data['checkRepositoryStars'] = bs4.BeautifulSoup(
+            markup=RequestHandler(url=UserHandler(username=username).serialize(_=True, repo_name=repo_name)).sendGetRequest(content=True),
+            features='html5lib',
+        ).find(
+            name='svg',
+            attrs={
+                'class': 'octicon octicon-star mr-2',
+            }
+        ).find_next(
+            name='strong',
+        ).get_text()
+        
+        return self.json_data['checkRepositoryStars']
+    
+    @property
+    def profilePictureUrl(self: Self) -> str:
+        self.__json_data['profilePictureUrl'] = bs4.BeautifulSoup(
+            markup=self.__data,
+            features='html5lib',
+        ).find(
+            name='img',
+            attrs={
+                'class': 'avatar avatar-user width-full border color-bg-default',
+            }
+        ).get_attribute_list(key='src')[0]
+        
+        return self.json_data['profilePictureUrl']
         
     @property
     def json_data(self: Self) -> dict[str, Any]:
         return self.__json_data
     
     def startApi(self: Self, log: bool = True) -> Literal[None]:
-        if (log):
-            init()
-            print(f'{Fore.GREEN}Api Started Successfully{Fore.WHITE}')
-        
-        self.__json_data = {
-            'fullname': self.fullname,
-            'followers': self.followers,
-            'followings': self.followings,
-            'biography': self.biography,
-            'location': self.location,
-            'website': self.website,
-            'totalRepositories': self.totalRepositories,
-        }
+        if (sys.version_info[0:2] == (3, 11)):
+            if (log):
+                init()
+                print(f'{Fore.GREEN}Api Started Successfully{Fore.WHITE}')
+            
+            self.__json_data = {
+                'fullname': self.fullname,
+                'followers': self.followers,
+                'followings': self.followings,
+                'biography': self.biography,
+                'location': self.location,
+                'website': self.website,
+                'totalRepositories': self.totalRepositories,
+                'totalStarsGiven': self.totalStarsGiven,
+                'profilePictureUrl': self.profilePictureUrl,
+            }
+        else:
+            print(f"{Fore.YELLOW}Your Current Python Interpereter version is {Fore.CYAN}{sys.version.split(sep=' ')[0]}\n{Fore.YELLOW}This Package implemented for Python Version {Fore.GREEN}3.11\n{Fore.YELLOW}If you want to Use this Package, you have to update your interpreter{Fore.WHITE}")
+            sys.exit(0)
```

### Comparing `github4api-1.1.3/github4api/user_handler/__init__.py` & `github4api-1.1.4/github4api/handlers/user_handler/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 if (__debug__):
     try:
-        import re
-        import bs4
         from typing import Self, Literal
     
     except* ModuleNotFoundError as mnfe:
         raise mnfe.__doc__
     
     except* ImportError as ie:
         raise ie.__doc__
@@ -15,11 +13,17 @@
 
 
 
 class UserHandler:
     def __init__(self: Self, username: str) -> Literal[None]:
         self.__username = username
         
-    def serialize(self: Self, get_repos: bool = False) -> str:
+    @property
+    def username(self: Self) -> str:
+        return self.__username
+        
+    def serialize(self: Self, get_repos: bool = False, _: bool = False, repo_name: str = None) -> str:
         if (get_repos):
-            return f'https://github.com/{self.__username}?tab=repositories'
-        return f'https://github.com/{self.__username}'
+            return f'https://github.com/{self.username}?tab=repositories'
+        if (_):
+            return f'https://github.com/{self.username}/{repo_name}'
+        return f'https://github.com/{self.username}'
```

### Comparing `github4api-1.1.3/github4api.egg-info/PKG-INFO` & `github4api-1.1.4/github4api.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: github4api
-Version: 1.1.3
+Version: 1.1.4
 Summary: A python Package API for getting Github Users Information.
 Author: Shervin Badanara (shervinbdndev)
 Author-email: shervin2234@gmail.com
 Maintainer: Shervin Badanara
 License: MIT
 Project-URL: Source, https://www.github.com/shervinbdndev/github4api/
 Keywords: python,api,github,github_api,github_package
@@ -13,18 +13,20 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
+License-File: LICENSE
 
 
 <h1 align='center' style="font-size:5rem"><b>github4api</b></h1>
-<p align='center'><b>Version 1.1.3</b></p>
+<p align='center'><b>Version 1.1.4</b></p>
+<p align='center'><b>Written with Python 3.11.3</b></p>
 <div align="center">
     <div align="center">
         <img src="https://img.shields.io/github/license/shervinbdndev/github4api.svg"></img>
     </div>
     <img src="https://img.shields.io/github/forks/shervinbdndev/github4api.svg"></img>
     <img src="https://img.shields.io/github/stars/shervinbdndev/github4api.svg"></img>
     <img src="https://img.shields.io/github/watchers/shervinbdndev/github4api.svg"></img>
@@ -53,22 +55,31 @@
 <img src="https://img.shields.io/badge/Ubuntu-E95420?style=for-the-badge&logo=ubuntu&logoColor=white"></img>
 <img src="https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white"></img>
 <img src="https://img.shields.io/badge/Stack_Overflow-FE7A16?style=for-the-badge&logo=stack-overflow&logoColor=white"></img>
 <img src="https://img.shields.io/badge/Reddit-FF4500?style=for-the-badge&logo=reddit&logoColor=white"></img>
 
 <br>
 <h2 align='center'><b>WorkSpace</h2>
-<img src="https://img.shields.io/badge/Intel-Core_i5_10700K-0071C5?style=for-the-badge&logo=intel&logoColor=white"></img>
+<img src="https://img.shields.io/badge/Intel-Core_i5_10600K-0071C5?style=for-the-badge&logo=intel&logoColor=white"></img>
 <img src="https://img.shields.io/badge/NVIDIA-RTX2060 OC-76B900?style=for-the-badge&logo=nvidia&logoColor=white"></img>
 <img src="https://img.shields.io/badge/Windows11-0078D6?style=for-the-badge&logo=windows&logoColor=white"></img>
 
 
 <hr>
 
 <br><br><br>
+
+<h1 align='center' style='color:#ff0080; font-size:3rem;'><b>! Warning !</h1>
+
+
+- ## This package uses ``` ExceptionGroup ``` to handle exceptions.
+- ## You have to use python [3.11](https://www.python.org/downloads/) or above to be able to use this package.
+
+
+<br><br><br>
 <h1 align='left'><b>Update Your Interpreter</b></h1>
 
 # Windows / CMD
 
 ```python
 py -m pip install --upgrade pip
 ```
@@ -114,16 +125,16 @@
 <br><br><br>
 <h1 align='left'><b>Usage</b></h1>
 
 <br>
 
 ```python
 from github4api.scraper import Scrape # Scraper Class
-from github4api.user_handler import UserHandler # User Handler Class
-from github4api.request_handler import RequestHandler # Request Handler Class
+from github4api.handlers.user_handler import UserHandler # User Handler Class
+from github4api.handlers.request_handler import RequestHandler # Request Handler Class
 
 
 def main():
 
     # UserHandler serializes the value you given to the username param
     # RequestHandler gets the Serialized data then sends a GET request to github servers and saves the page content in request variable
 
@@ -158,21 +169,21 @@
 
 ```
 
 <br><br><br>
 
 # New Changes on Version 1.1.3
 
-- ### Now you can Access Users Repositories Names
+- ### Now you can Access User's Repositories Names
 
 ```py
 
 from github4api.scraper import Scrape
-from github4api.user_handler import UserHandler
-from github4api.request_handler import RequestHandler
+from github4api.handlers.user_handler import UserHandler
+from github4api.handlers.request_handler import RequestHandler
 
 
 
 
 def main():
     request: RequestHandler = RequestHandler(
         url=UserHandler(username='shervinbdndev').serialize(get_repos=True), # for accessing the repositories you should set get_repos param to True
@@ -199,12 +210,59 @@
 if (__name__ == "__main__"):
     main()
 
 
 
 ```
 
+<br><br><br>
+
+# New Changes on Version 1.1.4
+
+## Now you can Access
+
+- ### User's Total Stars Given
+- ### User's Profile Picture Url
+- ### Check Repository Star Count
+
+```python
+
+from github4api.scraper import Scrape
+from github4api.handlers.user_handler import UserHandler
+from github4api.handlers.request_handler import RequestHandler
+
+
+
+def main():
+    request: RequestHandler = RequestHandler(
+        url=UserHandler(username='shervinbdndev').serialize()
+    ).sendGetRequest(content=True)
+    
+    scraper: Scrape = Scrape(data=request)
+    
+    scraper.startApi(log=False)
+    
+    print(scraper.totalStarsGiven) # total stars given
+    
+    print(scraper.profilePictureUrl) # profile picture url
+
+    # now using this new method you lets you check users repository's star count
+
+    print(scraper.checkRepositoryStars(
+        username='shervinbdndev', # user's username
+        repo_name='Quizino', # repository's name
+    ))
+
+
+
+
+if (__name__ == "__main__"):
+    main()
+
+```
+
+<br>
 
 <h1 align='left'>Enjoy :)</h1>
 
 <br>
 <h3><b>Package Uploaded in PYPI :<a href="https://pypi.org/project/github4api/">Here</a></b></h3>
```

### Comparing `github4api-1.1.3/setup.py` & `github4api-1.1.4/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 with codecs.open(os.path.normpath(path=os.path.join(os.path.abspath(path=os.path.dirname(p=__file__)) , r"README.md")) , encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
 
 setup(
     name="github4api",
-    version='1.1.3',
+    version='1.1.4',
     author="Shervin Badanara (shervinbdndev)",
     maintainer="Shervin Badanara",
     author_email="shervin2234@gmail.com",
     description='A python Package API for getting Github Users Information.',
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages() ,
```

### Comparing `github4api-1.1.3/tests/__init__.py` & `github4api-1.1.4/tests/__init__.py`

 * *Files identical despite different names*

