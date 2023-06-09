# Comparing `tmp/procuret-0.0.8.tar.gz` & `tmp/procuret-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/procuret-0.0.8.tar", last modified: Mon Jan  4 02:23:07 2021, max compression
+gzip compressed data, was "dist/procuret-0.0.9.tar", last modified: Mon Jan  4 03:04:34 2021, max compression
```

## Comparing `procuret-0.0.8.tar` & `procuret-0.0.9.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 hugh       (501) staff       (20)        0 2021-01-04 02:23:07.858347 procuret-0.0.8/
--rw-r--r--   0 hugh       (501) staff       (20)     7642 2021-01-04 02:23:07.857995 procuret-0.0.8/PKG-INFO
-drwxr-xr-x   0 hugh       (501) staff       (20)        0 2021-01-04 02:23:07.845617 procuret-0.0.8/procuret/
--rw-r--r--   0 hugh       (501) staff       (20)      429 2020-12-16 02:51:55.000000 procuret-0.0.8/procuret/__init__.py
-drwxr-xr-x   0 hugh       (501) staff       (20)        0 2021-01-04 02:23:07.849136 procuret-0.0.8/procuret/ancillary/
--rw-r--r--   0 hugh       (501) staff       (20)        0 2020-09-23 04:24:01.000000 procuret-0.0.8/procuret/ancillary/__init__.py
--rw-r--r--   0 hugh       (501) staff       (20)      388 2020-09-22 22:41:40.000000 procuret-0.0.8/procuret/ancillary/abstract_session.py
--rw-r--r--   0 hugh       (501) staff       (20)     2027 2020-12-17 21:02:37.000000 procuret-0.0.8/procuret/ancillary/command_line.py
--rw-r--r--   0 hugh       (501) staff       (20)      223 2020-09-22 02:28:30.000000 procuret-0.0.8/procuret/ancillary/communication_option.py
--rw-r--r--   0 hugh       (501) staff       (20)      591 2020-09-22 02:32:35.000000 procuret-0.0.8/procuret/ancillary/entity_headline.py
--rw-r--r--   0 hugh       (501) staff       (20)      169 2020-09-23 00:23:20.000000 procuret-0.0.8/procuret/ancillary/session_lifecycle.py
--rw-r--r--   0 hugh       (501) staff       (20)      185 2020-09-22 03:56:02.000000 procuret-0.0.8/procuret/ancillary/session_perspective.py
-drwxr-xr-x   0 hugh       (501) staff       (20)        0 2021-01-04 02:23:07.850592 procuret-0.0.8/procuret/data/
--rw-r--r--   0 hugh       (501) staff       (20)        0 2020-12-14 03:42:45.000000 procuret-0.0.8/procuret/data/__init__.py
--rw-r--r--   0 hugh       (501) staff       (20)     4245 2020-12-15 21:02:47.000000 procuret-0.0.8/procuret/data/codable.py
--rw-r--r--   0 hugh       (501) staff       (20)     1643 2020-12-15 21:00:16.000000 procuret-0.0.8/procuret/data/decodable.py
--rw-r--r--   0 hugh       (501) staff       (20)      180 2020-12-15 20:12:09.000000 procuret-0.0.8/procuret/data/order.py
-drwxr-xr-x   0 hugh       (501) staff       (20)        0 2021-01-04 02:23:07.852229 procuret-0.0.8/procuret/errors/
--rw-r--r--   0 hugh       (501) staff       (20)      219 2020-09-23 04:26:46.000000 procuret-0.0.8/procuret/errors/__init__.py
--rw-r--r--   0 hugh       (501) staff       (20)      548 2020-09-23 00:03:07.000000 procuret-0.0.8/procuret/errors/api_error.py
--rw-r--r--   0 hugh       (501) staff       (20)      109 2020-09-22 02:37:50.000000 procuret-0.0.8/procuret/errors/error.py
--rw-r--r--   0 hugh       (501) staff       (20)      531 2020-09-22 23:43:30.000000 procuret-0.0.8/procuret/errors/inconsistent.py
--rw-r--r--   0 hugh       (501) staff       (20)      993 2020-09-22 03:38:20.000000 procuret-0.0.8/procuret/errors/type_error.py
-drwxr-xr-x   0 hugh       (501) staff       (20)        0 2021-01-04 02:23:07.853731 procuret-0.0.8/procuret/http/
--rw-r--r--   0 hugh       (501) staff       (20)        0 2020-09-23 04:24:11.000000 procuret-0.0.8/procuret/http/__init__.py
--rw-r--r--   0 hugh       (501) staff       (20)     3945 2020-12-16 02:53:05.000000 procuret-0.0.8/procuret/http/api_request.py
--rw-r--r--   0 hugh       (501) staff       (20)      212 2020-09-22 04:00:53.000000 procuret-0.0.8/procuret/http/method.py
--rw-r--r--   0 hugh       (501) staff       (20)     1288 2020-12-14 03:09:18.000000 procuret-0.0.8/procuret/http/query_parameter.py
--rw-r--r--   0 hugh       (501) staff       (20)     1017 2020-09-22 06:33:16.000000 procuret-0.0.8/procuret/http/query_parameters.py
-drwxr-xr-x   0 hugh       (501) staff       (20)        0 2021-01-04 02:23:07.854717 procuret-0.0.8/procuret/instalment_link/
--rw-r--r--   0 hugh       (501) staff       (20)      223 2020-12-15 21:04:30.000000 procuret-0.0.8/procuret/instalment_link/__init__.py
--rw-r--r--   0 hugh       (501) staff       (20)     7065 2021-01-04 02:13:18.000000 procuret-0.0.8/procuret/instalment_link/instalment_link.py
--rw-r--r--   0 hugh       (501) staff       (20)     1402 2021-01-04 02:20:33.000000 procuret-0.0.8/procuret/instalment_link/open.py
--rw-r--r--   0 hugh       (501) staff       (20)     2107 2020-09-23 03:20:21.000000 procuret-0.0.8/procuret/session.py
-drwxr-xr-x   0 hugh       (501) staff       (20)        0 2021-01-04 02:23:07.855943 procuret-0.0.8/procuret/tests/
--rw-r--r--   0 hugh       (501) staff       (20)        0 2020-09-23 04:24:13.000000 procuret-0.0.8/procuret/tests/__init__.py
-drwxr-xr-x   0 hugh       (501) staff       (20)        0 2021-01-04 02:23:07.856595 procuret-0.0.8/procuret/tests/cases/
--rw-r--r--   0 hugh       (501) staff       (20)       72 2020-09-22 06:21:04.000000 procuret-0.0.8/procuret/tests/cases/__init__.py
--rw-r--r--   0 hugh       (501) staff       (20)     1765 2020-12-15 21:02:36.000000 procuret-0.0.8/procuret/tests/cases/instalment_link.py
--rw-r--r--   0 hugh       (501) staff       (20)     5815 2020-10-31 01:14:59.000000 procuret-0.0.8/procuret/tests/test.py
--rw-r--r--   0 hugh       (501) staff       (20)      642 2020-09-22 05:27:01.000000 procuret-0.0.8/procuret/tests/test_result.py
--rw-r--r--   0 hugh       (501) staff       (20)     1258 2020-09-22 06:21:11.000000 procuret-0.0.8/procuret/tests/test_suite.py
-drwxr-xr-x   0 hugh       (501) staff       (20)        0 2021-01-04 02:23:07.857429 procuret-0.0.8/procuret/time/
--rw-r--r--   0 hugh       (501) staff       (20)        0 2020-09-23 04:24:17.000000 procuret-0.0.8/procuret/time/__init__.py
--rw-r--r--   0 hugh       (501) staff       (20)     2401 2020-12-14 04:05:58.000000 procuret-0.0.8/procuret/time/time.py
--rw-r--r--   0 hugh       (501) staff       (20)      357 2020-09-21 10:06:19.000000 procuret-0.0.8/procuret/time/tz_utc.py
--rw-r--r--   0 hugh       (501) staff       (20)       18 2021-01-04 02:22:54.000000 procuret-0.0.8/procuret/version.py
-drwxr-xr-x   0 hugh       (501) staff       (20)        0 2021-01-04 02:23:07.846799 procuret-0.0.8/procuret.egg-info/
--rw-r--r--   0 hugh       (501) staff       (20)     7642 2021-01-04 02:23:07.000000 procuret-0.0.8/procuret.egg-info/PKG-INFO
--rw-r--r--   0 hugh       (501) staff       (20)     1224 2021-01-04 02:23:07.000000 procuret-0.0.8/procuret.egg-info/SOURCES.txt
--rw-r--r--   0 hugh       (501) staff       (20)        1 2021-01-04 02:23:07.000000 procuret-0.0.8/procuret.egg-info/dependency_links.txt
--rw-r--r--   0 hugh       (501) staff       (20)        9 2021-01-04 02:23:07.000000 procuret-0.0.8/procuret.egg-info/top_level.txt
--rw-r--r--   0 hugh       (501) staff       (20)       38 2021-01-04 02:23:07.858465 procuret-0.0.8/setup.cfg
--rw-r--r--   0 hugh       (501) staff       (20)     1531 2020-12-16 02:52:35.000000 procuret-0.0.8/setup.py
+drwxr-xr-x   0 hugh       (501) staff       (20)        0 2021-01-04 03:04:34.313713 procuret-0.0.9/
+-rw-r--r--   0 hugh       (501) staff       (20)     7642 2021-01-04 03:04:34.313290 procuret-0.0.9/PKG-INFO
+drwxr-xr-x   0 hugh       (501) staff       (20)        0 2021-01-04 03:04:34.301781 procuret-0.0.9/procuret/
+-rw-r--r--   0 hugh       (501) staff       (20)      429 2020-12-16 02:51:55.000000 procuret-0.0.9/procuret/__init__.py
+drwxr-xr-x   0 hugh       (501) staff       (20)        0 2021-01-04 03:04:34.304938 procuret-0.0.9/procuret/ancillary/
+-rw-r--r--   0 hugh       (501) staff       (20)        0 2020-09-23 04:24:01.000000 procuret-0.0.9/procuret/ancillary/__init__.py
+-rw-r--r--   0 hugh       (501) staff       (20)      482 2021-01-04 02:49:40.000000 procuret-0.0.9/procuret/ancillary/abstract_session.py
+-rw-r--r--   0 hugh       (501) staff       (20)     2027 2020-12-17 21:02:37.000000 procuret-0.0.9/procuret/ancillary/command_line.py
+-rw-r--r--   0 hugh       (501) staff       (20)      223 2020-09-22 02:28:30.000000 procuret-0.0.9/procuret/ancillary/communication_option.py
+-rw-r--r--   0 hugh       (501) staff       (20)      591 2020-09-22 02:32:35.000000 procuret-0.0.9/procuret/ancillary/entity_headline.py
+-rw-r--r--   0 hugh       (501) staff       (20)      169 2020-09-23 00:23:20.000000 procuret-0.0.9/procuret/ancillary/session_lifecycle.py
+-rw-r--r--   0 hugh       (501) staff       (20)      185 2020-09-22 03:56:02.000000 procuret-0.0.9/procuret/ancillary/session_perspective.py
+drwxr-xr-x   0 hugh       (501) staff       (20)        0 2021-01-04 03:04:34.306063 procuret-0.0.9/procuret/data/
+-rw-r--r--   0 hugh       (501) staff       (20)        0 2020-12-14 03:42:45.000000 procuret-0.0.9/procuret/data/__init__.py
+-rw-r--r--   0 hugh       (501) staff       (20)     4245 2020-12-15 21:02:47.000000 procuret-0.0.9/procuret/data/codable.py
+-rw-r--r--   0 hugh       (501) staff       (20)     1643 2020-12-15 21:00:16.000000 procuret-0.0.9/procuret/data/decodable.py
+-rw-r--r--   0 hugh       (501) staff       (20)      180 2020-12-15 20:12:09.000000 procuret-0.0.9/procuret/data/order.py
+drwxr-xr-x   0 hugh       (501) staff       (20)        0 2021-01-04 03:04:34.307409 procuret-0.0.9/procuret/errors/
+-rw-r--r--   0 hugh       (501) staff       (20)      219 2020-09-23 04:26:46.000000 procuret-0.0.9/procuret/errors/__init__.py
+-rw-r--r--   0 hugh       (501) staff       (20)      548 2020-09-23 00:03:07.000000 procuret-0.0.9/procuret/errors/api_error.py
+-rw-r--r--   0 hugh       (501) staff       (20)      109 2020-09-22 02:37:50.000000 procuret-0.0.9/procuret/errors/error.py
+-rw-r--r--   0 hugh       (501) staff       (20)      531 2020-09-22 23:43:30.000000 procuret-0.0.9/procuret/errors/inconsistent.py
+-rw-r--r--   0 hugh       (501) staff       (20)      993 2020-09-22 03:38:20.000000 procuret-0.0.9/procuret/errors/type_error.py
+drwxr-xr-x   0 hugh       (501) staff       (20)        0 2021-01-04 03:04:34.308854 procuret-0.0.9/procuret/http/
+-rw-r--r--   0 hugh       (501) staff       (20)        0 2020-09-23 04:24:11.000000 procuret-0.0.9/procuret/http/__init__.py
+-rw-r--r--   0 hugh       (501) staff       (20)     4547 2021-01-04 02:49:06.000000 procuret-0.0.9/procuret/http/api_request.py
+-rw-r--r--   0 hugh       (501) staff       (20)      212 2020-09-22 04:00:53.000000 procuret-0.0.9/procuret/http/method.py
+-rw-r--r--   0 hugh       (501) staff       (20)     1288 2020-12-14 03:09:18.000000 procuret-0.0.9/procuret/http/query_parameter.py
+-rw-r--r--   0 hugh       (501) staff       (20)     1017 2020-09-22 06:33:16.000000 procuret-0.0.9/procuret/http/query_parameters.py
+drwxr-xr-x   0 hugh       (501) staff       (20)        0 2021-01-04 03:04:34.309965 procuret-0.0.9/procuret/instalment_link/
+-rw-r--r--   0 hugh       (501) staff       (20)      223 2020-12-15 21:04:30.000000 procuret-0.0.9/procuret/instalment_link/__init__.py
+-rw-r--r--   0 hugh       (501) staff       (20)     7065 2021-01-04 02:13:18.000000 procuret-0.0.9/procuret/instalment_link/instalment_link.py
+-rw-r--r--   0 hugh       (501) staff       (20)     1402 2021-01-04 02:20:33.000000 procuret-0.0.9/procuret/instalment_link/open.py
+-rw-r--r--   0 hugh       (501) staff       (20)     2660 2021-01-04 02:55:02.000000 procuret-0.0.9/procuret/session.py
+drwxr-xr-x   0 hugh       (501) staff       (20)        0 2021-01-04 03:04:34.311109 procuret-0.0.9/procuret/tests/
+-rw-r--r--   0 hugh       (501) staff       (20)        0 2020-09-23 04:24:13.000000 procuret-0.0.9/procuret/tests/__init__.py
+drwxr-xr-x   0 hugh       (501) staff       (20)        0 2021-01-04 03:04:34.311965 procuret-0.0.9/procuret/tests/cases/
+-rw-r--r--   0 hugh       (501) staff       (20)       72 2020-09-22 06:21:04.000000 procuret-0.0.9/procuret/tests/cases/__init__.py
+-rw-r--r--   0 hugh       (501) staff       (20)     1765 2021-01-04 03:03:25.000000 procuret-0.0.9/procuret/tests/cases/instalment_link.py
+-rw-r--r--   0 hugh       (501) staff       (20)     5815 2020-10-31 01:14:59.000000 procuret-0.0.9/procuret/tests/test.py
+-rw-r--r--   0 hugh       (501) staff       (20)      642 2020-09-22 05:27:01.000000 procuret-0.0.9/procuret/tests/test_result.py
+-rw-r--r--   0 hugh       (501) staff       (20)     1258 2020-09-22 06:21:11.000000 procuret-0.0.9/procuret/tests/test_suite.py
+drwxr-xr-x   0 hugh       (501) staff       (20)        0 2021-01-04 03:04:34.312862 procuret-0.0.9/procuret/time/
+-rw-r--r--   0 hugh       (501) staff       (20)        0 2020-09-23 04:24:17.000000 procuret-0.0.9/procuret/time/__init__.py
+-rw-r--r--   0 hugh       (501) staff       (20)     2401 2020-12-14 04:05:58.000000 procuret-0.0.9/procuret/time/time.py
+-rw-r--r--   0 hugh       (501) staff       (20)      357 2020-09-21 10:06:19.000000 procuret-0.0.9/procuret/time/tz_utc.py
+-rw-r--r--   0 hugh       (501) staff       (20)       18 2021-01-04 03:04:09.000000 procuret-0.0.9/procuret/version.py
+drwxr-xr-x   0 hugh       (501) staff       (20)        0 2021-01-04 03:04:34.302863 procuret-0.0.9/procuret.egg-info/
+-rw-r--r--   0 hugh       (501) staff       (20)     7642 2021-01-04 03:04:34.000000 procuret-0.0.9/procuret.egg-info/PKG-INFO
+-rw-r--r--   0 hugh       (501) staff       (20)     1224 2021-01-04 03:04:34.000000 procuret-0.0.9/procuret.egg-info/SOURCES.txt
+-rw-r--r--   0 hugh       (501) staff       (20)        1 2021-01-04 03:04:34.000000 procuret-0.0.9/procuret.egg-info/dependency_links.txt
+-rw-r--r--   0 hugh       (501) staff       (20)        9 2021-01-04 03:04:34.000000 procuret-0.0.9/procuret.egg-info/top_level.txt
+-rw-r--r--   0 hugh       (501) staff       (20)       38 2021-01-04 03:04:34.313801 procuret-0.0.9/setup.cfg
+-rw-r--r--   0 hugh       (501) staff       (20)     1531 2020-12-16 02:52:35.000000 procuret-0.0.9/setup.py
```

### Comparing `procuret-0.0.8/PKG-INFO` & `procuret-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: procuret
-Version: 0.0.8
+Version: 0.0.9
 Summary: Procuret API Library
 Home-page: https://github.com/procuret/procuret-python
 Author: Procuret
 Author-email: hugh@procuret.com
 License: UNKNOWN
 Project-URL: Github Repository, https://github.com/procuret/procuret-python
 Project-URL: About, https://github.com/procuret/procuret-python
```

### Comparing `procuret-0.0.8/procuret/ancillary/command_line.py` & `procuret-0.0.9/procuret/ancillary/command_line.py`

 * *Files identical despite different names*

### Comparing `procuret-0.0.8/procuret/ancillary/entity_headline.py` & `procuret-0.0.9/procuret/ancillary/entity_headline.py`

 * *Files identical despite different names*

### Comparing `procuret-0.0.8/procuret/data/codable.py` & `procuret-0.0.9/procuret/data/codable.py`

 * *Files identical despite different names*

### Comparing `procuret-0.0.8/procuret/data/decodable.py` & `procuret-0.0.9/procuret/data/decodable.py`

 * *Files identical despite different names*

### Comparing `procuret-0.0.8/procuret/errors/api_error.py` & `procuret-0.0.9/procuret/errors/api_error.py`

 * *Files identical despite different names*

### Comparing `procuret-0.0.8/procuret/errors/inconsistent.py` & `procuret-0.0.9/procuret/errors/inconsistent.py`

 * *Files identical despite different names*

### Comparing `procuret-0.0.8/procuret/errors/type_error.py` & `procuret-0.0.9/procuret/errors/type_error.py`

 * *Files identical despite different names*

### Comparing `procuret-0.0.8/procuret/http/api_request.py` & `procuret-0.0.9/procuret/http/api_request.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 
 class ApiRequest:
 
     API_KEY_NAME = 'x-procuret-api-key'
     SIGNATURE_KEY_NAME = 'x-procuret-signature'
     SESSION_ID_NAME = 'x-procuret-session-id'
     USER_AGENT = 'Procuret Python ' + AGENT_VERSION
+    FORWARDED_AGENT = 'x-procuret-forwarded-agent'
 
     @classmethod
     def make(
         cls,
         path: str,
         method: HTTPMethod,
         data: Optional[Union[Object, Array]],
@@ -59,14 +60,20 @@
         if session is not None:
             headers = cls._add_authorisation_to_headers(
                 headers=headers,
                 path=path,
                 session=session
             )
 
+        if session is not None and session.acts_for_another_agent:
+            headers = cls._add_forwarded_agent_to_headers(
+                headers=headers,
+                session=session
+            )
+
         encoded_data: Optional[bytes] = None
         if data is not None:
             encoded_data = json.dumps(data).encode('utf-8')
             headers['Content-Type'] = 'application/json'
 
         request = Request(
             url=url,
@@ -106,14 +113,28 @@
                 api_key=session.api_key,
                 path=path
             )
 
         raise NotImplementedError
 
     @classmethod
+    def _add_forwarded_agent_to_headers(
+        cls: Type[T],
+        headers: Dict[str, str],
+        session: AbstractSession
+    ) -> Dict[str, str]:
+
+        if not session.acts_for_another_agent:
+            return headers
+        
+        headers[cls.FORWARDED_AGENT] = str(session.on_behalf_of)
+
+        return headers
+
+    @classmethod
     def _headers_with_key(
         cls: Type[T],
         headers: Dict[str, str],
         api_key: str
     ) -> Dict[str, str]:
 
         headers[cls.API_KEY_NAME] = api_key
```

### Comparing `procuret-0.0.8/procuret/http/query_parameter.py` & `procuret-0.0.9/procuret/http/query_parameter.py`

 * *Files identical despite different names*

### Comparing `procuret-0.0.8/procuret/http/query_parameters.py` & `procuret-0.0.9/procuret/http/query_parameters.py`

 * *Files identical despite different names*

### Comparing `procuret-0.0.8/procuret/instalment_link/instalment_link.py` & `procuret-0.0.9/procuret/instalment_link/instalment_link.py`

 * *Files identical despite different names*

### Comparing `procuret-0.0.8/procuret/instalment_link/open.py` & `procuret-0.0.9/procuret/instalment_link/open.py`

 * *Files identical despite different names*

### Comparing `procuret-0.0.8/procuret/session.py` & `procuret-0.0.9/procuret/session.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 """
 from procuret.data.codable import CodingDefinition as CD
 from procuret.ancillary.abstract_session import AbstractSession
 from procuret.ancillary.session_lifecycle import Lifecycle
 from procuret.ancillary.session_perspective import Perspective
 from procuret.http.api_request import ApiRequest
 from procuret.http.method import HTTPMethod
-from typing import TypeVar, Type
+from typing import TypeVar, Type, Optional
 from procuret.errors.inconsistent import InconsistentState
 
-T = TypeVar('T', bound='Session')
+Self = TypeVar('Self', bound='Session')
 
 
 class Session(AbstractSession):
 
     PATH = '/session'
 
     coding_map = {
@@ -29,39 +29,54 @@
 
     def __init__(
         self,
         session_id: int,
         session_key: str,
         api_key: str,
         lifecycle: Lifecycle,
-        perspective: Perspective
+        perspective: Perspective,
+        on_behalf_of: Optional[int] = None
     ) -> None:
 
         self._session_id = session_id
         self._session_key = session_key
         self._api_key = api_key
         self._lifecycle = lifecycle
         self._perspective = perspective
+        self._on_behalf_of = on_behalf_of
 
         return
 
     session_id = property(lambda s: s._session_id)
     session_key = property(lambda s: s._session_key)
     api_key = property(lambda s: s._api_key)
     lifecycle = property(lambda s: s._lifecycle)
     perspective = property(lambda s: s._perspective)
+    on_behalf_of = property(lambda s: s._on_behalf_of)
+
+    acts_for_another_agent = property(lambda s: s.on_behalf_of is not None)
+
+    def acting_for(self, agent: int) -> Self:
+        return Session(
+            session_id=self._session_id,
+            session_key=self._session_key,
+            api_key=self._api_key,
+            lifecycle=self._lifecycle,
+            perspective=self._perspective,
+            on_behalf_of=agent
+        )
 
     @classmethod
     def create_with_email(
-        cls: Type[T],
+        cls: Type[Self],
         email: str,
         plaintext_secret: str,
         perspective: Perspective,
         lifecycle: Lifecycle = Lifecycle.LONG_LIVED
-    ) -> T:
+    ) -> Self:
 
         data = {
             'email': email,
             'secret': plaintext_secret,
             'perspective': perspective.value,
             'lifecycle': lifecycle.value
         }
```

### Comparing `procuret-0.0.8/procuret/tests/cases/instalment_link.py` & `procuret-0.0.9/procuret/tests/cases/instalment_link.py`

 * *Files identical despite different names*

### Comparing `procuret-0.0.8/procuret/tests/test.py` & `procuret-0.0.9/procuret/tests/test.py`

 * *Files identical despite different names*

### Comparing `procuret-0.0.8/procuret/tests/test_result.py` & `procuret-0.0.9/procuret/tests/test_result.py`

 * *Files identical despite different names*

### Comparing `procuret-0.0.8/procuret/tests/test_suite.py` & `procuret-0.0.9/procuret/tests/test_suite.py`

 * *Files identical despite different names*

### Comparing `procuret-0.0.8/procuret/time/time.py` & `procuret-0.0.9/procuret/time/time.py`

 * *Files identical despite different names*

### Comparing `procuret-0.0.8/procuret.egg-info/PKG-INFO` & `procuret-0.0.9/procuret.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: procuret
-Version: 0.0.8
+Version: 0.0.9
 Summary: Procuret API Library
 Home-page: https://github.com/procuret/procuret-python
 Author: Procuret
 Author-email: hugh@procuret.com
 License: UNKNOWN
 Project-URL: Github Repository, https://github.com/procuret/procuret-python
 Project-URL: About, https://github.com/procuret/procuret-python
```

### Comparing `procuret-0.0.8/procuret.egg-info/SOURCES.txt` & `procuret-0.0.9/procuret.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `procuret-0.0.8/setup.py` & `procuret-0.0.9/setup.py`

 * *Files identical despite different names*

