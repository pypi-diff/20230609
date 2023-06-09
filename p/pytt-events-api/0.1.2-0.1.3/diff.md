# Comparing `tmp/pytt_events_api-0.1.2.tar.gz` & `tmp/pytt_events_api-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytt_events_api-0.1.2.tar", last modified: Thu Apr  6 18:09:14 2023, max compression
+gzip compressed data, was "pytt_events_api-0.1.3.tar", last modified: Fri Jun  9 20:37:37 2023, max compression
```

## Comparing `pytt_events_api-0.1.2.tar` & `pytt_events_api-0.1.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0 valar     (1000) valar     (1000)        0 2023-04-06 18:09:14.236175 pytt_events_api-0.1.2/
--rwxrwxrwx   0 valar     (1000) valar     (1000)     1090 2023-01-28 12:24:47.000000 pytt_events_api-0.1.2/LICENSE
--rwxrwxrwx   0 valar     (1000) valar     (1000)     4607 2023-04-06 18:09:14.234202 pytt_events_api-0.1.2/PKG-INFO
--rwxrwxrwx   0 valar     (1000) valar     (1000)     4017 2023-03-20 23:22:20.000000 pytt_events_api-0.1.2/README.md
-drwxrwxrwx   0 valar     (1000) valar     (1000)        0 2023-04-06 18:09:14.069920 pytt_events_api-0.1.2/pytt_events/
--rwxrwxrwx   0 valar     (1000) valar     (1000)        0 2023-01-28 17:36:58.000000 pytt_events_api-0.1.2/pytt_events/__init__.py
--rwxrwxrwx   0 valar     (1000) valar     (1000)      485 2023-02-01 07:06:44.000000 pytt_events_api-0.1.2/pytt_events/auth.py
--rwxrwxrwx   0 valar     (1000) valar     (1000)     2768 2023-02-17 19:07:10.000000 pytt_events_api-0.1.2/pytt_events/context.py
--rwxrwxrwx   0 valar     (1000) valar     (1000)     1975 2023-02-03 18:31:20.000000 pytt_events_api-0.1.2/pytt_events/event.py
--rwxrwxrwx   0 valar     (1000) valar     (1000)     1037 2023-01-30 20:56:13.000000 pytt_events_api-0.1.2/pytt_events/properties.py
--rwxrwxrwx   0 valar     (1000) valar     (1000)     1457 2023-01-30 20:47:04.000000 pytt_events_api-0.1.2/pytt_events/supported_events.py
-drwxrwxrwx   0 valar     (1000) valar     (1000)        0 2023-04-06 18:09:14.146959 pytt_events_api-0.1.2/pytt_events/tests/
--rwxrwxrwx   0 valar     (1000) valar     (1000)        0 2023-01-28 17:54:54.000000 pytt_events_api-0.1.2/pytt_events/tests/__init__.py
--rwxrwxrwx   0 valar     (1000) valar     (1000)     1715 2023-02-17 19:06:00.000000 pytt_events_api-0.1.2/pytt_events/tests/conftest.py
--rwxrwxrwx   0 valar     (1000) valar     (1000)     1508 2023-02-17 19:05:23.000000 pytt_events_api-0.1.2/pytt_events/tests/test_event.py
--rwxrwxrwx   0 valar     (1000) valar     (1000)      882 2023-02-01 07:33:30.000000 pytt_events_api-0.1.2/pytt_events/tests/test_tiktok_events_api.py
--rwxrwxrwx   0 valar     (1000) valar     (1000)     2884 2023-02-01 07:34:55.000000 pytt_events_api-0.1.2/pytt_events/tiktok_events_api.py
-drwxrwxrwx   0 valar     (1000) valar     (1000)        0 2023-04-06 18:09:14.217202 pytt_events_api-0.1.2/pytt_events_api.egg-info/
--rwxrwxrwx   0 valar     (1000) valar     (1000)     4607 2023-04-06 18:09:13.000000 pytt_events_api-0.1.2/pytt_events_api.egg-info/PKG-INFO
--rwxrwxrwx   0 valar     (1000) valar     (1000)      535 2023-04-06 18:09:13.000000 pytt_events_api-0.1.2/pytt_events_api.egg-info/SOURCES.txt
--rwxrwxrwx   0 valar     (1000) valar     (1000)        1 2023-04-06 18:09:13.000000 pytt_events_api-0.1.2/pytt_events_api.egg-info/dependency_links.txt
--rwxrwxrwx   0 valar     (1000) valar     (1000)       81 2023-04-06 18:09:13.000000 pytt_events_api-0.1.2/pytt_events_api.egg-info/requires.txt
--rwxrwxrwx   0 valar     (1000) valar     (1000)       12 2023-04-06 18:09:13.000000 pytt_events_api-0.1.2/pytt_events_api.egg-info/top_level.txt
--rwxrwxrwx   0 valar     (1000) valar     (1000)       38 2023-04-06 18:09:14.237177 pytt_events_api-0.1.2/setup.cfg
--rwxrwxrwx   0 valar     (1000) valar     (1000)     1522 2023-04-06 18:08:47.000000 pytt_events_api-0.1.2/setup.py
+drwxrwxrwx   0 valar     (1000) valar     (1000)        0 2023-06-09 20:37:37.370321 pytt_events_api-0.1.3/
+-rwxrwxrwx   0 valar     (1000) valar     (1000)     1090 2023-01-28 12:24:47.000000 pytt_events_api-0.1.3/LICENSE
+-rwxrwxrwx   0 valar     (1000) valar     (1000)     4607 2023-06-09 20:37:37.367320 pytt_events_api-0.1.3/PKG-INFO
+-rwxrwxrwx   0 valar     (1000) valar     (1000)     4017 2023-03-20 23:22:20.000000 pytt_events_api-0.1.3/README.md
+drwxrwxrwx   0 valar     (1000) valar     (1000)        0 2023-06-09 20:37:37.090321 pytt_events_api-0.1.3/pytt_events/
+-rwxrwxrwx   0 valar     (1000) valar     (1000)        0 2023-01-28 17:36:58.000000 pytt_events_api-0.1.3/pytt_events/__init__.py
+-rwxrwxrwx   0 valar     (1000) valar     (1000)      486 2023-06-09 18:59:59.000000 pytt_events_api-0.1.3/pytt_events/auth.py
+-rwxrwxrwx   0 valar     (1000) valar     (1000)     2767 2023-06-09 20:35:54.000000 pytt_events_api-0.1.3/pytt_events/context.py
+-rwxrwxrwx   0 valar     (1000) valar     (1000)     1974 2023-06-09 20:35:54.000000 pytt_events_api-0.1.3/pytt_events/event.py
+-rwxrwxrwx   0 valar     (1000) valar     (1000)     1037 2023-06-09 19:25:47.000000 pytt_events_api-0.1.3/pytt_events/properties.py
+-rwxrwxrwx   0 valar     (1000) valar     (1000)     1457 2023-01-30 20:47:04.000000 pytt_events_api-0.1.3/pytt_events/supported_events.py
+drwxrwxrwx   0 valar     (1000) valar     (1000)        0 2023-06-09 20:37:37.215321 pytt_events_api-0.1.3/pytt_events/tests/
+-rwxrwxrwx   0 valar     (1000) valar     (1000)        0 2023-01-28 17:54:54.000000 pytt_events_api-0.1.3/pytt_events/tests/__init__.py
+-rwxrwxrwx   0 valar     (1000) valar     (1000)     3071 2023-06-09 20:10:55.000000 pytt_events_api-0.1.3/pytt_events/tests/conftest.py
+-rwxrwxrwx   0 valar     (1000) valar     (1000)     4533 2023-06-09 20:15:56.000000 pytt_events_api-0.1.3/pytt_events/tests/test_event.py
+-rwxrwxrwx   0 valar     (1000) valar     (1000)      882 2023-02-01 07:33:30.000000 pytt_events_api-0.1.3/pytt_events/tests/test_tiktok_post_events.py
+-rwxrwxrwx   0 valar     (1000) valar     (1000)     2886 2023-06-09 18:57:19.000000 pytt_events_api-0.1.3/pytt_events/tiktok_events_api.py
+drwxrwxrwx   0 valar     (1000) valar     (1000)        0 2023-06-09 20:37:37.340320 pytt_events_api-0.1.3/pytt_events_api.egg-info/
+-rwxrwxrwx   0 valar     (1000) valar     (1000)     4607 2023-06-09 20:37:36.000000 pytt_events_api-0.1.3/pytt_events_api.egg-info/PKG-INFO
+-rwxrwxrwx   0 valar     (1000) valar     (1000)      536 2023-06-09 20:37:36.000000 pytt_events_api-0.1.3/pytt_events_api.egg-info/SOURCES.txt
+-rwxrwxrwx   0 valar     (1000) valar     (1000)        1 2023-06-09 20:37:36.000000 pytt_events_api-0.1.3/pytt_events_api.egg-info/dependency_links.txt
+-rwxrwxrwx   0 valar     (1000) valar     (1000)       81 2023-06-09 20:37:36.000000 pytt_events_api-0.1.3/pytt_events_api.egg-info/requires.txt
+-rwxrwxrwx   0 valar     (1000) valar     (1000)       12 2023-06-09 20:37:36.000000 pytt_events_api-0.1.3/pytt_events_api.egg-info/top_level.txt
+-rwxrwxrwx   0 valar     (1000) valar     (1000)       38 2023-06-09 20:37:37.371322 pytt_events_api-0.1.3/setup.cfg
+-rwxrwxrwx   0 valar     (1000) valar     (1000)     1522 2023-06-09 20:36:52.000000 pytt_events_api-0.1.3/setup.py
```

### Comparing `pytt_events_api-0.1.2/LICENSE` & `pytt_events_api-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pytt_events_api-0.1.2/PKG-INFO` & `pytt_events_api-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytt_events_api
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python wrapper for the TikTok Events API
 Author: Victor Valar
 Author-email: <valar@victorvalar.me>
 License: LICENSE.txt
 Keywords: python,tiktok,events,api,tiktok ads,tiktok events api
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `pytt_events_api-0.1.2/README.md` & `pytt_events_api-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pytt_events_api-0.1.2/pytt_events/context.py` & `pytt_events_api-0.1.3/pytt_events/context.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,17 +14,17 @@
     callback: Optional[constr(
         strip_whitespace=True, max_length=501
     )]
 
     @validator('callback', pre=True)
     @classmethod
     def callback_is_valid(cls, value):
-        '''
-        Check if the callbaclk value is a valid ttclid.
-        '''
+        """
+        Check if the callback value is a valid ttclid.
+        """
         if value:
             ttclid_error = ContextFormatError(value=value, message="Callback must be a valid ttclid please check TikTok's documentation for more information on ttclid: https://ads.tiktok.com/marketing_api/docs?id=1739584860883969")
 
             value_list = value.split('.')
 
             if value[:6] != 'E.C.P.':
                 raise ttclid_error
```

### Comparing `pytt_events_api-0.1.2/pytt_events/event.py` & `pytt_events_api-0.1.3/pytt_events/event.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,18 +19,18 @@
     event: SupportedEvents
     event_id: Optional[constr(strip_whitespace=True, min_length=1)]
     timestamp: datetime.datetime # ISO 8601 format
     context: Context
     properties: Optional[Properties]
 
     def normalize_data(self) -> dict:
-        '''
+        """
         Normalize data to be sent to TikTok API
-        Also hashes identifieable data with SHA256
-        '''
+        Also hashes identifiable data with SHA256
+        """
         event = self.dict()
         data = event.get('context').get('user')
         external_id = data.get('external_id')
 
         if external_id != None:
             external_id = data.get('external_id').lower().replace(' ', '')
             hashed_external_id = sha256(external_id.encode('utf-8')).hexdigest()
```

### Comparing `pytt_events_api-0.1.2/pytt_events/properties.py` & `pytt_events_api-0.1.3/pytt_events/properties.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -19,21 +19,21 @@
     """
     PRODUCT_GROUP = 'product_group'
 
 class Content(BaseModel):
     content_id: constr(strip_whitespace=True, min_length=1)
     quantity: PositiveInt
     price: PositiveFloat
-    content_type: ContentType
     content_category: constr(min_length=1)
     content_name: constr(min_length=1)
 
 class Properties(BaseModel):
     currency: Optional[constr(strip_whitespace=True, min_length=3, max_length=3)]
     value: Optional[PositiveFloat]
+    content_type: ContentType
     description: Optional[constr(min_length=1)]
     query: Optional[constr(min_length=1)]
     status: Optional[constr(min_length=1)]
     contents: Optional[conlist(
         item_type=Content, unique_items=True, min_items=1
     )]
```

### Comparing `pytt_events_api-0.1.2/pytt_events/supported_events.py` & `pytt_events_api-0.1.3/pytt_events/supported_events.py`

 * *Files identical despite different names*

### Comparing `pytt_events_api-0.1.2/pytt_events/tests/conftest.py` & `pytt_events_api-0.1.3/pytt_events/tests/conftest.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,74 @@
 from pytest  import  fixture
 from pytt_events.auth import TikTokAuth
 from pytt_events.event import Event
-from pytt_events.properties import Properties
+from pytt_events.properties import Properties, ContentType, Content
 from pytt_events.context import Context, Ad, Page, User
+from pytt_events.supported_events import SupportedEvents
+from typing import List
 
 @fixture
 def auth() -> TikTokAuth:
-    auth = TikTokAuth()
-    yield auth
+    yield TikTokAuth()
+
+@fixture
+def ad() -> Ad:
+    yield Ad(callback='' )
+
+@fixture
+def page() -> Page:
+    yield Page(
+            url='https://www.example.com',
+            referrer='https://www.google.com'
+        )
+@fixture
+def user() -> User:
+    yield User(
+            external_id='123456',
+            email='test@test.com',
+            phone_number='+5541999999999',
+            ttp='94e2a4j9-h3j5-k2h5-98cc-c84a745mk098',
+        )
+
+@fixture
+def contents() -> List[Content]:
+
+    items = [
+        {
+            "content_id": "12345",
+            "quantity": 1,
+            "price": 1.00,
+            "content_name": "test content name",
+            "content_category": "test content category"
+        }, {
+            "content_id": "123456",
+            "quantity": 2,
+            "price": 2.00,
+            "content_name": "test second content name",
+            "content_category": "test second content category"
+        }
+    ]
+
+    contents = []
+    for item in items:
+        content = Content(
+            content_id=item.get('content_id'),
+            quantity=item.get('quantity'),
+            price=item.get('price'),
+            content_category=item.get('content_category'),
+            content_name=item.get('content_name'),
+
+        )
+        contents.append(content)
+
+    yield contents
+
 
 @fixture
 def event() -> Event:
-    event_name = "ViewContent"
-    event_id = '123456789'
-    timestamp = "2023-01-29 13:37:26-03:00"
     context = Context(
         user_agent='Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/98.0.4758.109 Safari/537.36',
         ip='13.57.97.131',
         ad=Ad(callback='' ), # ttclid
         page=Page(
             url='https://www.example.com',
             referrer='https://www.google.com'
@@ -25,29 +76,30 @@
         user=User(
             external_id='123456',
             email='test@test.com',
             phone_number='+5541998862934',
             ttp='94e2a4j9-h3j5-k2h5-98cc-c84a745mk098',
         ))
     properties = Properties(
-        currency='USD', # ISO 4217
+        currency='BRL', # ISO 4217
         value=1.00,
+        content_type=ContentType.PRODUCT,
         description='test description',
         query='test query',
         status='test status',
-        contents=[{"content_id": "12345", "quantity": 1, "price": 1.00, "content_type": "product", "content_name": "test content name", "content_category": "test content category"}]
+        contents=[{"content_id": "12345", "quantity": 1, "price": 1.00, "content_name": "test content name", "content_category": "test content category"}]
 
     )
     auth = TikTokAuth()
-    pixel_code = auth.TIKTOK_PIXEL_ID
+
     event = Event(
-        pixel_code=pixel_code,
+        pixel_code=auth.TIKTOK_PIXEL_ID,
         test_event_code=auth.TIKTOK_TEST_EVENT_CODE,
-        event=event_name,
-        event_id=event_id,
-        timestamp=timestamp,
+        event=SupportedEvents.VIEW_CONTENT,
+        event_id='123456789',
+        timestamp="2023-06-09 13:37:26-03:00",
         context=context,
         properties=properties
     )
 
     yield event
```

### Comparing `pytt_events_api-0.1.2/pytt_events/tests/test_tiktok_events_api.py` & `pytt_events_api-0.1.3/pytt_events/tests/test_tiktok_post_events.py`

 * *Files identical despite different names*

### Comparing `pytt_events_api-0.1.2/pytt_events/tiktok_events_api.py` & `pytt_events_api-0.1.3/pytt_events/tiktok_events_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         batch = []
 
         for event in events:
             batch.append(event.normalize_data())
 
         url = self.ROOT + auth.TIKTOK_API_VERSION + EVENT_PATH
 
-        headers = {'Content-Type': 'application/json', 'Access-Token': auth.TIKTOK_ACESS_TOKEN}
+        headers = {'Content-Type': 'application/json', 'Access-Token': auth.TIKTOK_ACCESS_TOKEN}
 
         payload = {
             "pixel_code": auth.TIKTOK_PIXEL_ID,
             "batch": batch
         }
 
         payload = json.dumps(payload, indent=4, sort_keys=True, default=str)
@@ -62,15 +62,15 @@
 
         EVENT_PATH = '/pixel/track/'
 
         url = self.ROOT + auth.TIKTOK_API_VERSION + EVENT_PATH
 
         payload = json.dumps(event.normalize_data(), indent=4, sort_keys=True, default=str)
 
-        headers = {'Content-Type': 'application/json', 'Access-Token': auth.TIKTOK_ACESS_TOKEN}
+        headers = {'Content-Type': 'application/json', 'Access-Token': auth.TIKTOK_ACCESS_TOKEN}
 
         try:
             response = requests.post(url, data=payload, headers=headers)
             json_response = response.json()
 
             # TikTok API uses custom error codes:
             # https://ads.tiktok.com/marketing_api/docs?id=1737172488964097
```

### Comparing `pytt_events_api-0.1.2/pytt_events_api.egg-info/PKG-INFO` & `pytt_events_api-0.1.3/pytt_events_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytt-events-api
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python wrapper for the TikTok Events API
 Author: Victor Valar
 Author-email: <valar@victorvalar.me>
 License: LICENSE.txt
 Keywords: python,tiktok,events,api,tiktok ads,tiktok events api
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `pytt_events_api-0.1.2/pytt_events_api.egg-info/SOURCES.txt` & `pytt_events_api-0.1.3/pytt_events_api.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -7,13 +7,13 @@
 pytt_events/event.py
 pytt_events/properties.py
 pytt_events/supported_events.py
 pytt_events/tiktok_events_api.py
 pytt_events/tests/__init__.py
 pytt_events/tests/conftest.py
 pytt_events/tests/test_event.py
-pytt_events/tests/test_tiktok_events_api.py
+pytt_events/tests/test_tiktok_post_events.py
 pytt_events_api.egg-info/PKG-INFO
 pytt_events_api.egg-info/SOURCES.txt
 pytt_events_api.egg-info/dependency_links.txt
 pytt_events_api.egg-info/requires.txt
 pytt_events_api.egg-info/top_level.txt
```

### Comparing `pytt_events_api-0.1.2/setup.py` & `pytt_events_api-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
 with open(requirements_filename) as f:
     # INSTALL_REQUIRES = [str(line[:-1]) for line in f]
     INSTALL_REQUIRES = ['requests', 'pytest', 'pydantic', 'phonenumbers', 'email-validator', 'ipaddress', 'pydantic[dotenv]']
 
-VERSION = '0.1.2'
+VERSION = '0.1.3'
 DESCRIPTION = 'Python wrapper for the TikTok Events API'
 LONG_DESCRIPTION = long_description
 PACKAGE_LICENSE = 'LICENSE.txt'
 
 # Setting up
 setup(
     name="pytt_events_api",
```

