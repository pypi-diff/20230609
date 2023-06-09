# Comparing `tmp/cyberwatch_api-0.1.1.tar.gz` & `tmp/cyberwatch_api-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cyberwatch_api-0.1.1.tar", last modified: Wed May  3 08:38:17 2023, max compression
+gzip compressed data, was "dist/cyberwatch_api-0.2.0.tar", last modified: Fri Jun  9 14:11:12 2023, max compression
```

## Comparing `cyberwatch_api-0.1.1.tar` & `cyberwatch_api-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:38:17.000000 cyberwatch_api-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-03 08:38:04.000000 cyberwatch_api-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-05-03 08:38:17.000000 cyberwatch_api-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-05-03 08:38:04.000000 cyberwatch_api-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:38:17.000000 cyberwatch_api-0.1.1/cyberwatch_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-05-03 08:38:17.000000 cyberwatch_api-0.1.1/cyberwatch_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-03 08:38:17.000000 cyberwatch_api-0.1.1/cyberwatch_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 08:38:17.000000 cyberwatch_api-0.1.1/cyberwatch_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-03 08:38:17.000000 cyberwatch_api-0.1.1/cyberwatch_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-03 08:38:17.000000 cyberwatch_api-0.1.1/cyberwatch_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6396 2023-05-03 08:38:04.000000 cyberwatch_api-0.1.1/cyberwatch_api.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 08:38:17.000000 cyberwatch_api-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-03 08:38:04.000000 cyberwatch_api-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:11:12.000000 cyberwatch_api-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-09 14:11:00.000000 cyberwatch_api-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3960 2023-06-09 14:11:12.000000 cyberwatch_api-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-06-09 14:11:00.000000 cyberwatch_api-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:11:12.000000 cyberwatch_api-0.2.0/cyberwatch_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3960 2023-06-09 14:11:12.000000 cyberwatch_api-0.2.0/cyberwatch_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-09 14:11:12.000000 cyberwatch_api-0.2.0/cyberwatch_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 14:11:12.000000 cyberwatch_api-0.2.0/cyberwatch_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-09 14:11:12.000000 cyberwatch_api-0.2.0/cyberwatch_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-09 14:11:12.000000 cyberwatch_api-0.2.0/cyberwatch_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6587 2023-06-09 14:11:00.000000 cyberwatch_api-0.2.0/cyberwatch_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 14:11:12.000000 cyberwatch_api-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-09 14:11:00.000000 cyberwatch_api-0.2.0/setup.py
```

### Comparing `cyberwatch_api-0.1.1/LICENSE` & `cyberwatch_api-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cyberwatch_api-0.1.1/PKG-INFO` & `cyberwatch_api-0.2.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,19 @@
-Metadata-Version: 2.1
-Name: cyberwatch_api
-Version: 0.1.1
-Summary: Python Api client for the Cyberwatch software
-Author: CyberWatch SAS
-License: MIT
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Cyberwatch API
 
 Python Api client for the Cyberwatch software
 <!-- START doctoc generated TOC please keep comment here to allow auto update -->
 <!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
 **Table of Contents** 
 
 - [Installation](#installation)
   - [Prerequisites](#prerequisites)
+  - [Module installation](#module-installation)
   - [Configuration](#configuration)
+  - [api.conf file location](#apiconf-file-location)
 - [Ping](#ping)
 - [Examples](#examples)
 - [Usage](#usage)
 
 <!-- END doctoc generated TOC please keep comment here to allow auto update -->
 ## Installation
 
@@ -35,23 +28,34 @@
 pip3 install cyberwatch_api
 ```
 
 ### Configuration
 
 To be able to authenticate to the Cyberwatch API, you need to configure the api.conf file. This client authenticates using basic auth.
 
-All the information can be retrieved in your profile on the Cyberwatch interface while creating an API user as following: 
+All the information can be retrieved in your profile on the Cyberwatch interface while creating an API user as following:
 
 "Profile > API keys > See my API keys > +Add"
 
 You can download directly the api.conf file after clicking on "Create > Export" or copy/paste the information to an api.conf file in this directory.
 
+### api.conf file location
+
+The library will search for the api.conf file in the current working directory and, if there is none, in its parent directory.
+
+If the api.conf file is located elsewhere, you can specify the path as shown below:
+
+```python
+Cyberwatch_Pyhelper(path_to_conf="your/path/to/api.conf/file/")
+```
+
 ## Ping
 
-Create a ping.py script with the following content inside: 
+Create a ping.py script with the following content inside:
+
 ```python
 from cyberwatch_api import Cyberwatch_Pyhelper
 
 output = Cyberwatch_Pyhelper().request(
     method="get",
     endpoint="/api/v3/ping"
     )
@@ -65,14 +69,15 @@
 $ python3 ping.py
 ```
 
 The output should look like this:
 ```bash
 {"uuid": "1ab2c3de-546f-789g-9f87-6ed5c4b3a210"}
 ```
+
 Otherwise, check that there are no typing errors in your API_KEY, SECRET_KEY or API_URL in the api.conf file and that your Cyberwatch instance is up.
 
 ## Examples
 
 **Run an example script**
 
 1. Choose a script from the examples directory and copy it to your computer
@@ -94,7 +99,27 @@
  * Add any required logic
 
 Note that the `request` method provided by this module always outputs a generator. This is intended to allow building of high performance scripts. If the request you perform returns a single result and not a list, you will find the result in the first row of this generator.
 
 **Location of the Swagger's documentation**
 
 You can find it while clicking on the </> logo on the top right of the Cyberwatch interface.
+
+**Request body parameters**
+
+When using this API, you need to distinguish between GET/DELETE and POST/PUT methods.
+
+For the GET/DELETE methods you need to use the `params` variable, while for the POST/PUT methods, you need to use the `body_params` variable as follows:
+```python
+output = Cyberwatch_Pyhelper().request(
+    method="get",
+    endpoint="/api/v3/assets/servers/{id}",
+    params={'id' : 7}
+)
+```
+```python
+output = Cyberwatch_Pyhelper().request(
+    method="put",
+    endpoint="/api/v3/vulnerabilities/servers/{id}",
+    body_params={'id' : 7, 'description' : "this is a description", "groups":[3,4]}
+)
+```
```

### Comparing `cyberwatch_api-0.1.1/cyberwatch_api.egg-info/PKG-INFO` & `cyberwatch_api-0.2.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: cyberwatch-api
-Version: 0.1.1
+Name: cyberwatch_api
+Version: 0.2.0
 Summary: Python Api client for the Cyberwatch software
 Author: CyberWatch SAS
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Cyberwatch API
@@ -12,15 +12,17 @@
 Python Api client for the Cyberwatch software
 <!-- START doctoc generated TOC please keep comment here to allow auto update -->
 <!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
 **Table of Contents** 
 
 - [Installation](#installation)
   - [Prerequisites](#prerequisites)
+  - [Module installation](#module-installation)
   - [Configuration](#configuration)
+  - [api.conf file location](#apiconf-file-location)
 - [Ping](#ping)
 - [Examples](#examples)
 - [Usage](#usage)
 
 <!-- END doctoc generated TOC please keep comment here to allow auto update -->
 ## Installation
 
@@ -35,23 +37,34 @@
 pip3 install cyberwatch_api
 ```
 
 ### Configuration
 
 To be able to authenticate to the Cyberwatch API, you need to configure the api.conf file. This client authenticates using basic auth.
 
-All the information can be retrieved in your profile on the Cyberwatch interface while creating an API user as following: 
+All the information can be retrieved in your profile on the Cyberwatch interface while creating an API user as following:
 
 "Profile > API keys > See my API keys > +Add"
 
 You can download directly the api.conf file after clicking on "Create > Export" or copy/paste the information to an api.conf file in this directory.
 
+### api.conf file location
+
+The library will search for the api.conf file in the current working directory and, if there is none, in its parent directory.
+
+If the api.conf file is located elsewhere, you can specify the path as shown below:
+
+```python
+Cyberwatch_Pyhelper(path_to_conf="your/path/to/api.conf/file/")
+```
+
 ## Ping
 
-Create a ping.py script with the following content inside: 
+Create a ping.py script with the following content inside:
+
 ```python
 from cyberwatch_api import Cyberwatch_Pyhelper
 
 output = Cyberwatch_Pyhelper().request(
     method="get",
     endpoint="/api/v3/ping"
     )
@@ -65,14 +78,15 @@
 $ python3 ping.py
 ```
 
 The output should look like this:
 ```bash
 {"uuid": "1ab2c3de-546f-789g-9f87-6ed5c4b3a210"}
 ```
+
 Otherwise, check that there are no typing errors in your API_KEY, SECRET_KEY or API_URL in the api.conf file and that your Cyberwatch instance is up.
 
 ## Examples
 
 **Run an example script**
 
 1. Choose a script from the examples directory and copy it to your computer
@@ -94,7 +108,27 @@
  * Add any required logic
 
 Note that the `request` method provided by this module always outputs a generator. This is intended to allow building of high performance scripts. If the request you perform returns a single result and not a list, you will find the result in the first row of this generator.
 
 **Location of the Swagger's documentation**
 
 You can find it while clicking on the </> logo on the top right of the Cyberwatch interface.
+
+**Request body parameters**
+
+When using this API, you need to distinguish between GET/DELETE and POST/PUT methods.
+
+For the GET/DELETE methods you need to use the `params` variable, while for the POST/PUT methods, you need to use the `body_params` variable as follows:
+```python
+output = Cyberwatch_Pyhelper().request(
+    method="get",
+    endpoint="/api/v3/assets/servers/{id}",
+    params={'id' : 7}
+)
+```
+```python
+output = Cyberwatch_Pyhelper().request(
+    method="put",
+    endpoint="/api/v3/vulnerabilities/servers/{id}",
+    body_params={'id' : 7, 'description' : "this is a description", "groups":[3,4]}
+)
+```
```

### Comparing `cyberwatch_api-0.1.1/cyberwatch_api.py` & `cyberwatch_api-0.2.0/cyberwatch_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,25 +38,26 @@
     @property
     def api_url(self) -> str:
         return self.__api_url
 
     def clear_endpoint(f):
         """
         Decorator that takes the endpoint that was given by the API user,
-        and replaces the {id} by the id parameter that was given inside the params dict
+        and replaces the {id} by the id parameter that was given inside the params or body params dict
         """
         def wrapper(*args, **kwargs):
             endpoint = kwargs.get("endpoint")
             if "{id}" in endpoint:
-                params_id = kwargs.get("params").get("id")
-                del kwargs["params"]["id"]
+                params_id = (kwargs.get("params",{}).get("id") or kwargs.get("body_params",{}).get("id"))
+                for key in kwargs:
+                    if type(kwargs[key]) == dict :
+                        del(kwargs[key]["id"])
                 endpoint = endpoint.replace("{id}", str(params_id))
                 kwargs.update({"endpoint": endpoint})
             return f(*args, **kwargs)
-
         return wrapper
 
     @api_url.setter
     def api_url(self, value: str):
         """
         This setter will search for a parameter given during the initialization of the class.
         If not found it will search inside the CONF file if given.
@@ -181,14 +182,15 @@
         yield response
         while "next" in response.links:
             response = requests.request(
                 method=self.method,
                 url=response.links["next"]["url"],
                 auth=self.__basic_auth(),
                 params=params,
-                timeout=self.timeout
+                timeout=self.timeout,
+                verify=self.verify_ssl
             )
             yield response
 
 
 if __name__ == "__main__":
     Cyberwatch_Pyhelper()
```

