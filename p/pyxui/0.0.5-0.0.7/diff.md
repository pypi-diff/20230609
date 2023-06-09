# Comparing `tmp/pyxui-0.0.5.tar.gz` & `tmp/pyxui-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyxui-0.0.5.tar", last modified: Mon May 15 17:06:23 2023, max compression
+gzip compressed data, was "pyxui-0.0.7.tar", last modified: Fri Jun  9 11:54:20 2023, max compression
```

## Comparing `pyxui-0.0.5.tar` & `pyxui-0.0.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 17:06:23.275118 pyxui-0.0.5/
--rw-rw-rw-   0        0        0     1070 2023-05-15 16:46:45.000000 pyxui-0.0.5/LICENSE
--rw-rw-rw-   0        0        0     5047 2023-05-15 17:06:23.274108 pyxui-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     4464 2023-05-15 16:46:45.000000 pyxui-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-15 17:06:23.249366 pyxui-0.0.5/pyxui/
--rw-rw-rw-   0        0        0       26 2023-05-15 16:46:45.000000 pyxui-0.0.5/pyxui/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-15 17:06:23.266687 pyxui-0.0.5/pyxui/config_gen/
--rw-rw-rw-   0        0        0      441 2023-05-15 16:46:45.000000 pyxui-0.0.5/pyxui/config_gen/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-15 17:06:23.267688 pyxui-0.0.5/pyxui/errors/
--rw-rw-rw-   0        0        0      884 2023-05-15 16:46:45.000000 pyxui-0.0.5/pyxui/errors/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-15 17:06:23.273110 pyxui-0.0.5/pyxui/methods/
--rw-rw-rw-   0        0        0      235 2023-05-15 16:46:45.000000 pyxui-0.0.5/pyxui/methods/__init__.py
--rw-rw-rw-   0        0        0     1411 2023-05-15 16:46:45.000000 pyxui-0.0.5/pyxui/methods/base.py
--rw-rw-rw-   0        0        0     4746 2023-05-15 16:46:45.000000 pyxui-0.0.5/pyxui/methods/clients.py
--rw-rw-rw-   0        0        0     1367 2023-05-15 16:46:45.000000 pyxui-0.0.5/pyxui/methods/inbounds.py
--rw-rw-rw-   0        0        0     1077 2023-05-15 16:46:45.000000 pyxui-0.0.5/pyxui/methods/login.py
--rw-rw-rw-   0        0        0      464 2023-05-15 16:46:45.000000 pyxui-0.0.5/pyxui/xui.py
-drwxrwxrwx   0        0        0        0 2023-05-15 17:06:23.265372 pyxui-0.0.5/pyxui.egg-info/
--rw-rw-rw-   0        0        0     5047 2023-05-15 17:06:23.000000 pyxui-0.0.5/pyxui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      377 2023-05-15 17:06:23.000000 pyxui-0.0.5/pyxui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 17:06:23.000000 pyxui-0.0.5/pyxui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-15 17:06:23.000000 pyxui-0.0.5/pyxui.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-15 17:06:23.000000 pyxui-0.0.5/pyxui.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-15 17:06:23.275118 pyxui-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      707 2023-05-15 16:46:45.000000 pyxui-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 11:54:20.984479 pyxui-0.0.7/
+-rw-rw-rw-   0        0        0     1070 2023-05-15 16:46:45.000000 pyxui-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0     5606 2023-06-09 11:54:20.983012 pyxui-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     4996 2023-06-09 11:49:10.000000 pyxui-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-06-09 11:54:20.957797 pyxui-0.0.7/pyxui/
+-rw-rw-rw-   0        0        0       26 2023-05-15 16:46:45.000000 pyxui-0.0.7/pyxui/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 11:54:20.973554 pyxui-0.0.7/pyxui/config_gen/
+-rw-rw-rw-   0        0        0      441 2023-05-15 16:46:45.000000 pyxui-0.0.7/pyxui/config_gen/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 11:54:20.973554 pyxui-0.0.7/pyxui/errors/
+-rw-rw-rw-   0        0        0      884 2023-05-15 16:46:45.000000 pyxui-0.0.7/pyxui/errors/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 11:54:20.982012 pyxui-0.0.7/pyxui/methods/
+-rw-rw-rw-   0        0        0      235 2023-05-15 16:46:45.000000 pyxui-0.0.7/pyxui/methods/__init__.py
+-rw-rw-rw-   0        0        0     1611 2023-06-09 11:40:06.000000 pyxui-0.0.7/pyxui/methods/base.py
+-rw-rw-rw-   0        0        0     6850 2023-06-09 11:34:11.000000 pyxui-0.0.7/pyxui/methods/clients.py
+-rw-rw-rw-   0        0        0     1182 2023-06-09 11:41:26.000000 pyxui-0.0.7/pyxui/methods/inbounds.py
+-rw-rw-rw-   0        0        0     1077 2023-05-15 16:46:45.000000 pyxui-0.0.7/pyxui/methods/login.py
+-rw-rw-rw-   0        0        0      573 2023-06-09 11:40:26.000000 pyxui-0.0.7/pyxui/xui.py
+drwxrwxrwx   0        0        0        0 2023-06-09 11:54:20.972051 pyxui-0.0.7/pyxui.egg-info/
+-rw-rw-rw-   0        0        0     5606 2023-06-09 11:54:20.000000 pyxui-0.0.7/pyxui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      377 2023-06-09 11:54:20.000000 pyxui-0.0.7/pyxui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 11:54:20.000000 pyxui-0.0.7/pyxui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-09 11:54:20.000000 pyxui-0.0.7/pyxui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-09 11:54:20.000000 pyxui-0.0.7/pyxui.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-09 11:54:20.984479 pyxui-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      736 2023-06-09 11:52:22.000000 pyxui-0.0.7/setup.py
```

### Comparing `pyxui-0.0.5/LICENSE` & `pyxui-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pyxui-0.0.5/PKG-INFO` & `pyxui-0.0.7/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,46 @@
 Metadata-Version: 2.1
 Name: pyxui
-Version: 0.0.5
+Version: 0.0.7
 Summary: An application with python that allows you to modify your xui panel
 Home-page: https://github.com/staliox/pyxui
 Author: Staliox
 License: MIT
 Keywords: pyxui,xui,xui python,xui panel
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PyXUI 
-An application with python that allows you to modify your xui panel ([Sanaeii 3x-ui](https://github.com/MHSanaei/3x-ui)) ([alireza0 x-ui](https://github.com/alireza0/x-ui))
+An application with python that allows you to modify your xui panel ([alireza0 x-ui](https://github.com/alireza0/x-ui)) ([Sanaeii 3x-ui](https://github.com/MHSanaei/3x-ui)) 
 
 ## How To Install
 ```
 pip install pyxui
 ```
 
 ## How To Use
 - Import pyxui in your .py file
 ```python
 from pyxui import XUI
 
-xui = XUI("staliox.com", 54321, True) # Make note if you use https set True else don't set anything
-xui = XUI("staliox.com", 54321, True, "6fo3") # If you set panel path, you can set your panel path string
+# Basic:
+xui = XUI(
+    full_address="https://staliox.com:2087",
+    panel="alireza", # Your panel name, "alireza" or "sanaei"
+)
+
+# Advanced:
+xui = XUI(
+    full_address="http://staliox.site:2087",
+    panel="alireza", # Your panel name, "alireza" or "sanaei"
+    https=False # Make note if you don't use https set False else set True
+    session_string=... # If you have session cookie to use panel without login
+)
 ```
 
 - Login in your panel
 ```python
 from pyxui.errors import BadLogin
 
 try:
@@ -78,15 +89,31 @@
 }
 ```
 
 - Add client to exist inbound
 ```python
 get = xui.add_client(
     inbound_id=1,
-    email="fdsfgf@gmal.com",
+    email="example@gmal.com",
+    uuid="5d3d1bac-49cd-4b66-8be9-a728efa205fa",
+    enable = True,
+    flow = "",
+    limit_ip = 0,
+    total_gb = 5368709120,
+    expire_time = 1684948641772,
+    telegram_id = "",
+    subscription_id = ""
+)
+```
+
+- Update exist client
+```python
+get = xui.update_client(
+    inbound_id=1,
+    email="example@gmal.com",
     uuid="5d3d1bac-49cd-4b66-8be9-a728efa205fa",
     enable = True,
     flow = "",
     limit_ip = 0,
     total_gb = 5368709120,
     expire_time = 1684948641772,
     telegram_id = "",
```

### Comparing `pyxui-0.0.5/README.md` & `pyxui-0.0.7/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,33 @@
 # PyXUI 
-An application with python that allows you to modify your xui panel ([Sanaeii 3x-ui](https://github.com/MHSanaei/3x-ui)) ([alireza0 x-ui](https://github.com/alireza0/x-ui))
+An application with python that allows you to modify your xui panel ([alireza0 x-ui](https://github.com/alireza0/x-ui)) ([Sanaeii 3x-ui](https://github.com/MHSanaei/3x-ui)) 
 
 ## How To Install
 ```
 pip install pyxui
 ```
 
 ## How To Use
 - Import pyxui in your .py file
 ```python
 from pyxui import XUI
 
-xui = XUI("staliox.com", 54321, True) # Make note if you use https set True else don't set anything
-xui = XUI("staliox.com", 54321, True, "6fo3") # If you set panel path, you can set your panel path string
+# Basic:
+xui = XUI(
+    full_address="https://staliox.com:2087",
+    panel="alireza", # Your panel name, "alireza" or "sanaei"
+)
+
+# Advanced:
+xui = XUI(
+    full_address="http://staliox.site:2087",
+    panel="alireza", # Your panel name, "alireza" or "sanaei"
+    https=False # Make note if you don't use https set False else set True
+    session_string=... # If you have session cookie to use panel without login
+)
 ```
 
 - Login in your panel
 ```python
 from pyxui.errors import BadLogin
 
 try:
@@ -65,15 +76,31 @@
 }
 ```
 
 - Add client to exist inbound
 ```python
 get = xui.add_client(
     inbound_id=1,
-    email="fdsfgf@gmal.com",
+    email="example@gmal.com",
+    uuid="5d3d1bac-49cd-4b66-8be9-a728efa205fa",
+    enable = True,
+    flow = "",
+    limit_ip = 0,
+    total_gb = 5368709120,
+    expire_time = 1684948641772,
+    telegram_id = "",
+    subscription_id = ""
+)
+```
+
+- Update exist client
+```python
+get = xui.update_client(
+    inbound_id=1,
+    email="example@gmal.com",
     uuid="5d3d1bac-49cd-4b66-8be9-a728efa205fa",
     enable = True,
     flow = "",
     limit_ip = 0,
     total_gb = 5368709120,
     expire_time = 1684948641772,
     telegram_id = "",
```

### Comparing `pyxui-0.0.5/pyxui/errors/__init__.py` & `pyxui-0.0.7/pyxui/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxui-0.0.5/pyxui/methods/base.py` & `pyxui-0.0.7/pyxui/methods/base.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 import requests
 
 import pyxui
+from pyxui import errors
 
 class Base:
-    @property
-    def _panel_address(self: "pyxui.XUI") -> str:
-        return f"{self.https}://{self.address}:{self.port}{self.path}/"
-
     def request(
         self: "pyxui.XUI",
         path: str,
         method: str,
         params: dict = None
     ) -> requests.Response:
         """Request to xui panel.
@@ -26,22 +23,31 @@
                 Your request parameters, None is set for default but it's necessary for some POST methods
 
         Returns:
             `~requests.Response`: On success, the response is returned.
         """
         
         if path == "login":
-            url = self._panel_address + path
+            url = f"{self.full_address}/login"
         else:
-            url = self._panel_address + "xui/API/inbounds/" + path
+            url = f"{self.full_address}/{self.api_path}/inbounds/{path}"
 
         if self.session_string:
             cookie = {'session': self.session_string}
         else:
             cookie = None
 
         if method == "GET":
             response = requests.get(url, cookies=cookie, verify=self.https)
         elif method == "POST":
             response = requests.post(url, cookies=cookie, data=params, verify=self.https)
 
         return response
+
+    def verify_response(
+        self: "pyxui.XUI",
+        response: requests.Response
+    ) -> requests.Response:
+        if response.status_code != 404 and response.headers.get('Content-Type').startswith('application/json'):
+            return response.json()
+        
+        raise errors.NotFound()
```

### Comparing `pyxui-0.0.5/pyxui/methods/clients.py` & `pyxui-0.0.7/pyxui/methods/clients.py`

 * *Files 22% similar despite different names*

```diff
@@ -64,23 +64,23 @@
         Parameters:
             inbound_id (``int``):
                 Inbound id
                 
             email (``str``):
                Email of client
                 
+            uuid (``str``):
+               UUID of client
+                
             enable (``bool``, optional):
                Status of client
                 
             flow (``str``, optional):
                Flow of client
                 
-            uuid (``str``, optional):
-               UUID of client
-                
             limit_ip (``str``, optional):
                IP Limit of client
                 
             total_gb (``str``, optional):
                 Download and uploader limition of client and it's in bytes
                 
             expire_time (``str``, optional):
@@ -105,32 +105,31 @@
                     "flow": flow,
                     "limitIp": limit_ip,
                     "totalGB": total_gb,
                     "expiryTime": expire_time,
                     "tgId": telegram_id,
                     "subId": subscription_id
                 }
-            ]
+            ],
+            "decryption": "none",
+            "fallbacks": []
         }
         
         params = {
             "id": inbound_id,
             "settings": json.dumps(settings)
         }
 
-        send_request = self.request(
+        response = self.request(
             path="addClient",
             method="POST",
             params=params
         )
 
-        if send_request.status_code != 404 and send_request.headers.get('Content-Type').startswith('application/json'):
-            return send_request.json()
-        else:
-            raise errors.NotFound()
+        return self.verify_response(response)
 
     def delete_client(
         self: "pyxui.XUI",
         inbound_id: int,
         email: str = False,
         uuid: str = False
     ) -> Union[dict, errors.NotFound]:
@@ -152,16 +151,100 @@
         
         find_client = self.get_client(
             inbound_id=inbound_id,
             email=email,
             uuid=uuid
         )
         
-        send_request = self.request(
+        response = self.request(
             path=f"{inbound_id}/delClient/{find_client['id']}",
             method="POST"
         )
 
-        if send_request.status_code != 404 and send_request.headers.get('Content-Type').startswith('application/json'):
-            return send_request.json()
-        else:
-            raise errors.NotFound()
+        return self.verify_response(response)
+
+    def update_client(
+        self: "pyxui.XUI",
+        inbound_id: int,
+        email: str,
+        uuid: str,
+        enable: bool,
+        flow: str,
+        limit_ip: int,
+        total_gb: int,
+        expire_time: int,
+        telegram_id: str,
+        subscription_id: str,
+    ) -> Union[dict, errors.NotFound]:
+        """Add client to exist inbound.
+
+        Parameters:
+            inbound_id (``int``):
+                Inbound id
+                
+            email (``str``):
+               Email of client
+                
+            uuid (``str``):
+               UUID of client
+                
+            enable (``bool``):
+               Status of client
+                
+            flow (``str``):
+               Flow of client
+                
+            limit_ip (``str``):
+               IP Limit of client
+                
+            total_gb (``str``):
+                Download and uploader limition of client and it's in bytes
+                
+            expire_time (``str``):
+                Client expiration date and it's in timestamp (epoch)
+                
+            telegram_id (``str``):
+               Telegram id of client
+                
+            subscription_id (``str``):
+               Subscription id of client
+            
+        Returns:
+            `~Dict`: On success, a dict is returned else 404 error will be raised
+        """
+        
+        find_client = self.get_client(
+            inbound_id=inbound_id,
+            email=email,
+            uuid=uuid
+        )
+        
+        settings = {
+            "clients": [
+                {
+                    "id": uuid,
+                    "email": email,
+                    "enable": enable,
+                    "flow": flow,
+                    "limitIp": limit_ip,
+                    "totalGB": total_gb,
+                    "expiryTime": expire_time,
+                    "tgId": telegram_id,
+                    "subId": subscription_id
+                }
+            ],
+            "decryption": "none",
+            "fallbacks": []
+        }
+            
+        params = {
+            "id": inbound_id,
+            "settings": json.dumps(settings)
+        }
+        
+        response = self.request(
+            path=f"updateClient/{find_client['id']}",
+            method="POST",
+            params=params
+        )
+
+        return self.verify_response(response)
```

### Comparing `pyxui-0.0.5/pyxui/methods/inbounds.py` & `pyxui-0.0.7/pyxui/methods/inbounds.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,23 +9,27 @@
     ) -> Union[dict, errors.NotFound]:
         """Get inbounds of xui panel.
         
         Returns:
             `~Dict | errors.NotFound`: On success, a dict is returned else 404 error will be raised
         """
         
-        send_request = self.request(
-            path="list",
+        
+        if self.panel == "alireza":
+            path = ""
+            
+        elif self.panel == "sanaei":
+            path = "list"
+        
+        response = self.request(
+            path=path,
             method="GET"
         )
 
-        if send_request.status_code != 404 and send_request.headers.get('Content-Type').startswith('application/json'):
-            return send_request.json()
-        else:
-            raise errors.NotFound()
+        return self.verify_response(response)
         
     def get_inbound(
         self: "pyxui.XUI",
         inbound_id: int
     ) -> Union[dict, errors.NotFound]:
         """Get inbounds of xui panel.
 
@@ -33,16 +37,13 @@
             inbound_id (``int``):
                 Inbound id
         
         Returns:
             `~Dict | errors.NotFound`: On success, a dict is returned else 404 error will be raised
         """
         
-        send_request = self.request(
+        response = self.request(
             path=f"get/{inbound_id}",
             method="GET"
         )
 
-        if send_request.status_code != 404 and send_request.headers.get('Content-Type').startswith('application/json'):
-            return send_request.json()
-        else:
-            raise errors.NotFound()
+        return self.verify_response(response)
```

### Comparing `pyxui-0.0.5/pyxui/methods/login.py` & `pyxui-0.0.7/pyxui/methods/login.py`

 * *Files identical despite different names*

### Comparing `pyxui-0.0.5/pyxui.egg-info/PKG-INFO` & `pyxui-0.0.7/pyxui.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,46 @@
 Metadata-Version: 2.1
 Name: pyxui
-Version: 0.0.5
+Version: 0.0.7
 Summary: An application with python that allows you to modify your xui panel
 Home-page: https://github.com/staliox/pyxui
 Author: Staliox
 License: MIT
 Keywords: pyxui,xui,xui python,xui panel
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PyXUI 
-An application with python that allows you to modify your xui panel ([Sanaeii 3x-ui](https://github.com/MHSanaei/3x-ui)) ([alireza0 x-ui](https://github.com/alireza0/x-ui))
+An application with python that allows you to modify your xui panel ([alireza0 x-ui](https://github.com/alireza0/x-ui)) ([Sanaeii 3x-ui](https://github.com/MHSanaei/3x-ui)) 
 
 ## How To Install
 ```
 pip install pyxui
 ```
 
 ## How To Use
 - Import pyxui in your .py file
 ```python
 from pyxui import XUI
 
-xui = XUI("staliox.com", 54321, True) # Make note if you use https set True else don't set anything
-xui = XUI("staliox.com", 54321, True, "6fo3") # If you set panel path, you can set your panel path string
+# Basic:
+xui = XUI(
+    full_address="https://staliox.com:2087",
+    panel="alireza", # Your panel name, "alireza" or "sanaei"
+)
+
+# Advanced:
+xui = XUI(
+    full_address="http://staliox.site:2087",
+    panel="alireza", # Your panel name, "alireza" or "sanaei"
+    https=False # Make note if you don't use https set False else set True
+    session_string=... # If you have session cookie to use panel without login
+)
 ```
 
 - Login in your panel
 ```python
 from pyxui.errors import BadLogin
 
 try:
@@ -78,15 +89,31 @@
 }
 ```
 
 - Add client to exist inbound
 ```python
 get = xui.add_client(
     inbound_id=1,
-    email="fdsfgf@gmal.com",
+    email="example@gmal.com",
+    uuid="5d3d1bac-49cd-4b66-8be9-a728efa205fa",
+    enable = True,
+    flow = "",
+    limit_ip = 0,
+    total_gb = 5368709120,
+    expire_time = 1684948641772,
+    telegram_id = "",
+    subscription_id = ""
+)
+```
+
+- Update exist client
+```python
+get = xui.update_client(
+    inbound_id=1,
+    email="example@gmal.com",
     uuid="5d3d1bac-49cd-4b66-8be9-a728efa205fa",
     enable = True,
     flow = "",
     limit_ip = 0,
     total_gb = 5368709120,
     expire_time = 1684948641772,
     telegram_id = "",
```

