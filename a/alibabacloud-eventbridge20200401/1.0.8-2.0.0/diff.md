# Comparing `tmp/alibabacloud_eventbridge20200401-1.0.8.tar.gz` & `tmp/alibabacloud_eventbridge20200401-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_eventbridge20200401-1.0.8.tar", last modified: Fri Apr 21 03:40:55 2023, max compression
+gzip compressed data, was "dist/alibabacloud_eventbridge20200401-2.0.0.tar", last modified: Fri Jun  9 06:38:34 2023, max compression
```

## Comparing `alibabacloud_eventbridge20200401-1.0.8.tar` & `alibabacloud_eventbridge20200401-2.0.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 03:40:55.000000 alibabacloud_eventbridge20200401-1.0.8/
--rw-r--r--   0 root         (0) root         (0)      393 2023-04-21 03:40:54.000000 alibabacloud_eventbridge20200401-1.0.8/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-04-21 03:40:54.000000 alibabacloud_eventbridge20200401-1.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-04-21 03:40:54.000000 alibabacloud_eventbridge20200401-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2376 2023-04-21 03:40:55.000000 alibabacloud_eventbridge20200401-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1046 2023-04-21 03:40:54.000000 alibabacloud_eventbridge20200401-1.0.8/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1131 2023-04-21 03:40:54.000000 alibabacloud_eventbridge20200401-1.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 03:40:55.000000 alibabacloud_eventbridge20200401-1.0.8/alibabacloud_eventbridge20200401/
--rw-r--r--   0 root         (0) root         (0)       21 2023-04-21 03:40:54.000000 alibabacloud_eventbridge20200401-1.0.8/alibabacloud_eventbridge20200401/__init__.py
--rw-r--r--   0 root         (0) root         (0)   151575 2023-04-21 03:40:54.000000 alibabacloud_eventbridge20200401-1.0.8/alibabacloud_eventbridge20200401/client.py
--rw-r--r--   0 root         (0) root         (0)   752295 2023-04-21 03:40:54.000000 alibabacloud_eventbridge20200401-1.0.8/alibabacloud_eventbridge20200401/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 03:40:55.000000 alibabacloud_eventbridge20200401-1.0.8/alibabacloud_eventbridge20200401.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2376 2023-04-21 03:40:55.000000 alibabacloud_eventbridge20200401-1.0.8/alibabacloud_eventbridge20200401.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      484 2023-04-21 03:40:55.000000 alibabacloud_eventbridge20200401-1.0.8/alibabacloud_eventbridge20200401.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 03:40:55.000000 alibabacloud_eventbridge20200401-1.0.8/alibabacloud_eventbridge20200401.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2023-04-21 03:40:55.000000 alibabacloud_eventbridge20200401-1.0.8/alibabacloud_eventbridge20200401.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       33 2023-04-21 03:40:55.000000 alibabacloud_eventbridge20200401-1.0.8/alibabacloud_eventbridge20200401.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-04-21 03:40:55.000000 alibabacloud_eventbridge20200401-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2650 2023-04-21 03:40:54.000000 alibabacloud_eventbridge20200401-1.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 06:38:34.000000 alibabacloud_eventbridge20200401-2.0.0/
+-rw-r--r--   0 root         (0) root         (0)      440 2023-06-09 06:38:34.000000 alibabacloud_eventbridge20200401-2.0.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-06-09 06:38:34.000000 alibabacloud_eventbridge20200401-2.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-06-09 06:38:34.000000 alibabacloud_eventbridge20200401-2.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2376 2023-06-09 06:38:34.000000 alibabacloud_eventbridge20200401-2.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1046 2023-06-09 06:38:34.000000 alibabacloud_eventbridge20200401-2.0.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1131 2023-06-09 06:38:34.000000 alibabacloud_eventbridge20200401-2.0.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 06:38:34.000000 alibabacloud_eventbridge20200401-2.0.0/alibabacloud_eventbridge20200401/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-09 06:38:34.000000 alibabacloud_eventbridge20200401-2.0.0/alibabacloud_eventbridge20200401/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   151691 2023-06-09 06:38:34.000000 alibabacloud_eventbridge20200401-2.0.0/alibabacloud_eventbridge20200401/client.py
+-rw-r--r--   0 root         (0) root         (0)   749394 2023-06-09 06:38:34.000000 alibabacloud_eventbridge20200401-2.0.0/alibabacloud_eventbridge20200401/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 06:38:34.000000 alibabacloud_eventbridge20200401-2.0.0/alibabacloud_eventbridge20200401.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2376 2023-06-09 06:38:34.000000 alibabacloud_eventbridge20200401-2.0.0/alibabacloud_eventbridge20200401.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      484 2023-06-09 06:38:34.000000 alibabacloud_eventbridge20200401-2.0.0/alibabacloud_eventbridge20200401.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 06:38:34.000000 alibabacloud_eventbridge20200401-2.0.0/alibabacloud_eventbridge20200401.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2023-06-09 06:38:34.000000 alibabacloud_eventbridge20200401-2.0.0/alibabacloud_eventbridge20200401.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       33 2023-06-09 06:38:34.000000 alibabacloud_eventbridge20200401-2.0.0/alibabacloud_eventbridge20200401.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-06-09 06:38:34.000000 alibabacloud_eventbridge20200401-2.0.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2650 2023-06-09 06:38:34.000000 alibabacloud_eventbridge20200401-2.0.0/setup.py
```

### Comparing `alibabacloud_eventbridge20200401-1.0.8/LICENSE` & `alibabacloud_eventbridge20200401-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_eventbridge20200401-1.0.8/PKG-INFO` & `alibabacloud_eventbridge20200401-2.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_eventbridge20200401
-Version: 1.0.8
+Version: 2.0.0
 Summary: Alibaba Cloud eventbridge (20200401) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_eventbridge20200401-1.0.8/README-CN.md` & `alibabacloud_eventbridge20200401-2.0.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_eventbridge20200401-1.0.8/README.md` & `alibabacloud_eventbridge20200401-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_eventbridge20200401-1.0.8/alibabacloud_eventbridge20200401/client.py` & `alibabacloud_eventbridge20200401-2.0.0/alibabacloud_eventbridge20200401/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -707,100 +707,14 @@
     async def create_service_linked_role_for_product_async(
         self,
         request: eventbridge_20200401_models.CreateServiceLinkedRoleForProductRequest,
     ) -> eventbridge_20200401_models.CreateServiceLinkedRoleForProductResponse:
         runtime = util_models.RuntimeOptions()
         return await self.create_service_linked_role_for_product_with_options_async(request, runtime)
 
-    def create_targets_with_options(
-        self,
-        tmp_req: eventbridge_20200401_models.CreateTargetsRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> eventbridge_20200401_models.CreateTargetsResponse:
-        UtilClient.validate_model(tmp_req)
-        request = eventbridge_20200401_models.CreateTargetsShrinkRequest()
-        OpenApiUtilClient.convert(tmp_req, request)
-        if not UtilClient.is_unset(tmp_req.targets):
-            request.targets_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.targets, 'Targets', 'json')
-        query = {}
-        if not UtilClient.is_unset(request.event_bus_name):
-            query['EventBusName'] = request.event_bus_name
-        if not UtilClient.is_unset(request.rule_name):
-            query['RuleName'] = request.rule_name
-        if not UtilClient.is_unset(request.targets_shrink):
-            query['Targets'] = request.targets_shrink
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='CreateTargets',
-            version='2020-04-01',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            eventbridge_20200401_models.CreateTargetsResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    async def create_targets_with_options_async(
-        self,
-        tmp_req: eventbridge_20200401_models.CreateTargetsRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> eventbridge_20200401_models.CreateTargetsResponse:
-        UtilClient.validate_model(tmp_req)
-        request = eventbridge_20200401_models.CreateTargetsShrinkRequest()
-        OpenApiUtilClient.convert(tmp_req, request)
-        if not UtilClient.is_unset(tmp_req.targets):
-            request.targets_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.targets, 'Targets', 'json')
-        query = {}
-        if not UtilClient.is_unset(request.event_bus_name):
-            query['EventBusName'] = request.event_bus_name
-        if not UtilClient.is_unset(request.rule_name):
-            query['RuleName'] = request.rule_name
-        if not UtilClient.is_unset(request.targets_shrink):
-            query['Targets'] = request.targets_shrink
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='CreateTargets',
-            version='2020-04-01',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            eventbridge_20200401_models.CreateTargetsResponse(),
-            await self.call_api_async(params, req, runtime)
-        )
-
-    def create_targets(
-        self,
-        request: eventbridge_20200401_models.CreateTargetsRequest,
-    ) -> eventbridge_20200401_models.CreateTargetsResponse:
-        runtime = util_models.RuntimeOptions()
-        return self.create_targets_with_options(request, runtime)
-
-    async def create_targets_async(
-        self,
-        request: eventbridge_20200401_models.CreateTargetsRequest,
-    ) -> eventbridge_20200401_models.CreateTargetsResponse:
-        runtime = util_models.RuntimeOptions()
-        return await self.create_targets_with_options_async(request, runtime)
-
     def delete_api_destination_with_options(
         self,
         request: eventbridge_20200401_models.DeleteApiDestinationRequest,
         runtime: util_models.RuntimeOptions,
     ) -> eventbridge_20200401_models.DeleteApiDestinationResponse:
         UtilClient.validate_model(request)
         query = {}
@@ -2106,14 +2020,18 @@
         body = {}
         if not UtilClient.is_unset(request.limit):
             body['Limit'] = request.limit
         if not UtilClient.is_unset(request.name_prefix):
             body['NamePrefix'] = request.name_prefix
         if not UtilClient.is_unset(request.next_token):
             body['NextToken'] = request.next_token
+        if not UtilClient.is_unset(request.sink_arn):
+            body['SinkArn'] = request.sink_arn
+        if not UtilClient.is_unset(request.source_arn):
+            body['SourceArn'] = request.source_arn
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='ListEventStreamings',
             version='2020-04-01',
             protocol='HTTPS',
@@ -2138,14 +2056,18 @@
         body = {}
         if not UtilClient.is_unset(request.limit):
             body['Limit'] = request.limit
         if not UtilClient.is_unset(request.name_prefix):
             body['NamePrefix'] = request.name_prefix
         if not UtilClient.is_unset(request.next_token):
             body['NextToken'] = request.next_token
+        if not UtilClient.is_unset(request.sink_arn):
+            body['SinkArn'] = request.sink_arn
+        if not UtilClient.is_unset(request.source_arn):
+            body['SourceArn'] = request.source_arn
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='ListEventStreamings',
             version='2020-04-01',
             protocol='HTTPS',
@@ -2253,14 +2175,100 @@
     async def list_rules_async(
         self,
         request: eventbridge_20200401_models.ListRulesRequest,
     ) -> eventbridge_20200401_models.ListRulesResponse:
         runtime = util_models.RuntimeOptions()
         return await self.list_rules_with_options_async(request, runtime)
 
+    def list_targets_with_options(
+        self,
+        request: eventbridge_20200401_models.ListTargetsRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> eventbridge_20200401_models.ListTargetsResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.arn):
+            query['Arn'] = request.arn
+        if not UtilClient.is_unset(request.event_bus_name):
+            query['EventBusName'] = request.event_bus_name
+        if not UtilClient.is_unset(request.limit):
+            query['Limit'] = request.limit
+        if not UtilClient.is_unset(request.next_token):
+            query['NextToken'] = request.next_token
+        if not UtilClient.is_unset(request.rule_name):
+            query['RuleName'] = request.rule_name
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ListTargets',
+            version='2020-04-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            eventbridge_20200401_models.ListTargetsResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def list_targets_with_options_async(
+        self,
+        request: eventbridge_20200401_models.ListTargetsRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> eventbridge_20200401_models.ListTargetsResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.arn):
+            query['Arn'] = request.arn
+        if not UtilClient.is_unset(request.event_bus_name):
+            query['EventBusName'] = request.event_bus_name
+        if not UtilClient.is_unset(request.limit):
+            query['Limit'] = request.limit
+        if not UtilClient.is_unset(request.next_token):
+            query['NextToken'] = request.next_token
+        if not UtilClient.is_unset(request.rule_name):
+            query['RuleName'] = request.rule_name
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ListTargets',
+            version='2020-04-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            eventbridge_20200401_models.ListTargetsResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def list_targets(
+        self,
+        request: eventbridge_20200401_models.ListTargetsRequest,
+    ) -> eventbridge_20200401_models.ListTargetsResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.list_targets_with_options(request, runtime)
+
+    async def list_targets_async(
+        self,
+        request: eventbridge_20200401_models.ListTargetsRequest,
+    ) -> eventbridge_20200401_models.ListTargetsResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.list_targets_with_options_async(request, runtime)
+
     def list_user_defined_event_sources_with_options(
         self,
         runtime: util_models.RuntimeOptions,
     ) -> eventbridge_20200401_models.ListUserDefinedEventSourcesResponse:
         req = open_api_models.OpenApiRequest()
         params = open_api_models.Params(
             action='ListUserDefinedEventSources',
```

### Comparing `alibabacloud_eventbridge20200401-1.0.8/alibabacloud_eventbridge20200401/models.py` & `alibabacloud_eventbridge20200401-2.0.0/alibabacloud_eventbridge20200401/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -5725,423 +5725,14 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = CreateServiceLinkedRoleForProductResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class CreateTargetsRequestTargetsDeadLetterQueue(TeaModel):
-    def __init__(
-        self,
-        arn: str = None,
-    ):
-        self.arn = arn
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.arn is not None:
-            result['Arn'] = self.arn
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('Arn') is not None:
-            self.arn = m.get('Arn')
-        return self
-
-
-class CreateTargetsRequestTargetsParamList(TeaModel):
-    def __init__(
-        self,
-        form: str = None,
-        resource_key: str = None,
-        template: str = None,
-        value: str = None,
-    ):
-        self.form = form
-        self.resource_key = resource_key
-        self.template = template
-        self.value = value
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.form is not None:
-            result['Form'] = self.form
-        if self.resource_key is not None:
-            result['ResourceKey'] = self.resource_key
-        if self.template is not None:
-            result['Template'] = self.template
-        if self.value is not None:
-            result['Value'] = self.value
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('Form') is not None:
-            self.form = m.get('Form')
-        if m.get('ResourceKey') is not None:
-            self.resource_key = m.get('ResourceKey')
-        if m.get('Template') is not None:
-            self.template = m.get('Template')
-        if m.get('Value') is not None:
-            self.value = m.get('Value')
-        return self
-
-
-class CreateTargetsRequestTargets(TeaModel):
-    def __init__(
-        self,
-        dead_letter_queue: CreateTargetsRequestTargetsDeadLetterQueue = None,
-        endpoint: str = None,
-        errors_tolerance: str = None,
-        id: str = None,
-        param_list: List[CreateTargetsRequestTargetsParamList] = None,
-        push_retry_strategy: str = None,
-        type: str = None,
-    ):
-        self.dead_letter_queue = dead_letter_queue
-        self.endpoint = endpoint
-        self.errors_tolerance = errors_tolerance
-        self.id = id
-        self.param_list = param_list
-        self.push_retry_strategy = push_retry_strategy
-        self.type = type
-
-    def validate(self):
-        if self.dead_letter_queue:
-            self.dead_letter_queue.validate()
-        if self.param_list:
-            for k in self.param_list:
-                if k:
-                    k.validate()
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.dead_letter_queue is not None:
-            result['DeadLetterQueue'] = self.dead_letter_queue.to_map()
-        if self.endpoint is not None:
-            result['Endpoint'] = self.endpoint
-        if self.errors_tolerance is not None:
-            result['ErrorsTolerance'] = self.errors_tolerance
-        if self.id is not None:
-            result['Id'] = self.id
-        result['ParamList'] = []
-        if self.param_list is not None:
-            for k in self.param_list:
-                result['ParamList'].append(k.to_map() if k else None)
-        if self.push_retry_strategy is not None:
-            result['PushRetryStrategy'] = self.push_retry_strategy
-        if self.type is not None:
-            result['Type'] = self.type
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('DeadLetterQueue') is not None:
-            temp_model = CreateTargetsRequestTargetsDeadLetterQueue()
-            self.dead_letter_queue = temp_model.from_map(m['DeadLetterQueue'])
-        if m.get('Endpoint') is not None:
-            self.endpoint = m.get('Endpoint')
-        if m.get('ErrorsTolerance') is not None:
-            self.errors_tolerance = m.get('ErrorsTolerance')
-        if m.get('Id') is not None:
-            self.id = m.get('Id')
-        self.param_list = []
-        if m.get('ParamList') is not None:
-            for k in m.get('ParamList'):
-                temp_model = CreateTargetsRequestTargetsParamList()
-                self.param_list.append(temp_model.from_map(k))
-        if m.get('PushRetryStrategy') is not None:
-            self.push_retry_strategy = m.get('PushRetryStrategy')
-        if m.get('Type') is not None:
-            self.type = m.get('Type')
-        return self
-
-
-class CreateTargetsRequest(TeaModel):
-    def __init__(
-        self,
-        event_bus_name: str = None,
-        rule_name: str = None,
-        targets: List[CreateTargetsRequestTargets] = None,
-    ):
-        self.event_bus_name = event_bus_name
-        self.rule_name = rule_name
-        self.targets = targets
-
-    def validate(self):
-        if self.targets:
-            for k in self.targets:
-                if k:
-                    k.validate()
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.event_bus_name is not None:
-            result['EventBusName'] = self.event_bus_name
-        if self.rule_name is not None:
-            result['RuleName'] = self.rule_name
-        result['Targets'] = []
-        if self.targets is not None:
-            for k in self.targets:
-                result['Targets'].append(k.to_map() if k else None)
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('EventBusName') is not None:
-            self.event_bus_name = m.get('EventBusName')
-        if m.get('RuleName') is not None:
-            self.rule_name = m.get('RuleName')
-        self.targets = []
-        if m.get('Targets') is not None:
-            for k in m.get('Targets'):
-                temp_model = CreateTargetsRequestTargets()
-                self.targets.append(temp_model.from_map(k))
-        return self
-
-
-class CreateTargetsShrinkRequest(TeaModel):
-    def __init__(
-        self,
-        event_bus_name: str = None,
-        rule_name: str = None,
-        targets_shrink: str = None,
-    ):
-        self.event_bus_name = event_bus_name
-        self.rule_name = rule_name
-        self.targets_shrink = targets_shrink
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.event_bus_name is not None:
-            result['EventBusName'] = self.event_bus_name
-        if self.rule_name is not None:
-            result['RuleName'] = self.rule_name
-        if self.targets_shrink is not None:
-            result['Targets'] = self.targets_shrink
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('EventBusName') is not None:
-            self.event_bus_name = m.get('EventBusName')
-        if m.get('RuleName') is not None:
-            self.rule_name = m.get('RuleName')
-        if m.get('Targets') is not None:
-            self.targets_shrink = m.get('Targets')
-        return self
-
-
-class CreateTargetsResponseBodyDataErrorEntries(TeaModel):
-    def __init__(
-        self,
-        entry_id: str = None,
-        error_code: str = None,
-        error_message: str = None,
-    ):
-        self.entry_id = entry_id
-        self.error_code = error_code
-        self.error_message = error_message
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.entry_id is not None:
-            result['EntryId'] = self.entry_id
-        if self.error_code is not None:
-            result['ErrorCode'] = self.error_code
-        if self.error_message is not None:
-            result['ErrorMessage'] = self.error_message
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('EntryId') is not None:
-            self.entry_id = m.get('EntryId')
-        if m.get('ErrorCode') is not None:
-            self.error_code = m.get('ErrorCode')
-        if m.get('ErrorMessage') is not None:
-            self.error_message = m.get('ErrorMessage')
-        return self
-
-
-class CreateTargetsResponseBodyData(TeaModel):
-    def __init__(
-        self,
-        error_entries: List[CreateTargetsResponseBodyDataErrorEntries] = None,
-        error_entries_count: int = None,
-    ):
-        self.error_entries = error_entries
-        self.error_entries_count = error_entries_count
-
-    def validate(self):
-        if self.error_entries:
-            for k in self.error_entries:
-                if k:
-                    k.validate()
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        result['ErrorEntries'] = []
-        if self.error_entries is not None:
-            for k in self.error_entries:
-                result['ErrorEntries'].append(k.to_map() if k else None)
-        if self.error_entries_count is not None:
-            result['ErrorEntriesCount'] = self.error_entries_count
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        self.error_entries = []
-        if m.get('ErrorEntries') is not None:
-            for k in m.get('ErrorEntries'):
-                temp_model = CreateTargetsResponseBodyDataErrorEntries()
-                self.error_entries.append(temp_model.from_map(k))
-        if m.get('ErrorEntriesCount') is not None:
-            self.error_entries_count = m.get('ErrorEntriesCount')
-        return self
-
-
-class CreateTargetsResponseBody(TeaModel):
-    def __init__(
-        self,
-        code: str = None,
-        data: CreateTargetsResponseBodyData = None,
-        message: str = None,
-        request_id: str = None,
-        success: bool = None,
-    ):
-        self.code = code
-        self.data = data
-        self.message = message
-        self.request_id = request_id
-        self.success = success
-
-    def validate(self):
-        if self.data:
-            self.data.validate()
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.code is not None:
-            result['Code'] = self.code
-        if self.data is not None:
-            result['Data'] = self.data.to_map()
-        if self.message is not None:
-            result['Message'] = self.message
-        if self.request_id is not None:
-            result['RequestId'] = self.request_id
-        if self.success is not None:
-            result['Success'] = self.success
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('Code') is not None:
-            self.code = m.get('Code')
-        if m.get('Data') is not None:
-            temp_model = CreateTargetsResponseBodyData()
-            self.data = temp_model.from_map(m['Data'])
-        if m.get('Message') is not None:
-            self.message = m.get('Message')
-        if m.get('RequestId') is not None:
-            self.request_id = m.get('RequestId')
-        if m.get('Success') is not None:
-            self.success = m.get('Success')
-        return self
-
-
-class CreateTargetsResponse(TeaModel):
-    def __init__(
-        self,
-        headers: Dict[str, str] = None,
-        status_code: int = None,
-        body: CreateTargetsResponseBody = None,
-    ):
-        self.headers = headers
-        self.status_code = status_code
-        self.body = body
-
-    def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
-        if self.body:
-            self.body.validate()
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.headers is not None:
-            result['headers'] = self.headers
-        if self.status_code is not None:
-            result['statusCode'] = self.status_code
-        if self.body is not None:
-            result['body'] = self.body.to_map()
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('headers') is not None:
-            self.headers = m.get('headers')
-        if m.get('statusCode') is not None:
-            self.status_code = m.get('statusCode')
-        if m.get('body') is not None:
-            temp_model = CreateTargetsResponseBody()
-            self.body = temp_model.from_map(m['body'])
-        return self
-
-
 class DeleteApiDestinationRequest(TeaModel):
     def __init__(
         self,
         api_destination_name: str = None,
     ):
         self.api_destination_name = api_destination_name
 
@@ -13134,18 +12725,22 @@
 
 class ListEventStreamingsRequest(TeaModel):
     def __init__(
         self,
         limit: int = None,
         name_prefix: str = None,
         next_token: str = None,
+        sink_arn: str = None,
+        source_arn: str = None,
     ):
         self.limit = limit
         self.name_prefix = name_prefix
         self.next_token = next_token
+        self.sink_arn = sink_arn
+        self.source_arn = source_arn
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
@@ -13154,24 +12749,32 @@
         result = dict()
         if self.limit is not None:
             result['Limit'] = self.limit
         if self.name_prefix is not None:
             result['NamePrefix'] = self.name_prefix
         if self.next_token is not None:
             result['NextToken'] = self.next_token
+        if self.sink_arn is not None:
+            result['SinkArn'] = self.sink_arn
+        if self.source_arn is not None:
+            result['SourceArn'] = self.source_arn
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('Limit') is not None:
             self.limit = m.get('Limit')
         if m.get('NamePrefix') is not None:
             self.name_prefix = m.get('NamePrefix')
         if m.get('NextToken') is not None:
             self.next_token = m.get('NextToken')
+        if m.get('SinkArn') is not None:
+            self.sink_arn = m.get('SinkArn')
+        if m.get('SourceArn') is not None:
+            self.source_arn = m.get('SourceArn')
         return self
 
 
 class ListEventStreamingsResponseBodyDataEventStreamingsRunOptionsBatchWindow(TeaModel):
     def __init__(
         self,
         count_based_window: int = None,
@@ -16147,14 +15750,319 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ListRulesResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class ListTargetsRequest(TeaModel):
+    def __init__(
+        self,
+        arn: str = None,
+        event_bus_name: str = None,
+        limit: int = None,
+        next_token: str = None,
+        rule_name: str = None,
+    ):
+        self.arn = arn
+        self.event_bus_name = event_bus_name
+        self.limit = limit
+        self.next_token = next_token
+        self.rule_name = rule_name
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.arn is not None:
+            result['Arn'] = self.arn
+        if self.event_bus_name is not None:
+            result['EventBusName'] = self.event_bus_name
+        if self.limit is not None:
+            result['Limit'] = self.limit
+        if self.next_token is not None:
+            result['NextToken'] = self.next_token
+        if self.rule_name is not None:
+            result['RuleName'] = self.rule_name
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Arn') is not None:
+            self.arn = m.get('Arn')
+        if m.get('EventBusName') is not None:
+            self.event_bus_name = m.get('EventBusName')
+        if m.get('Limit') is not None:
+            self.limit = m.get('Limit')
+        if m.get('NextToken') is not None:
+            self.next_token = m.get('NextToken')
+        if m.get('RuleName') is not None:
+            self.rule_name = m.get('RuleName')
+        return self
+
+
+class ListTargetsResponseBodyDataTargetsParamList(TeaModel):
+    def __init__(
+        self,
+        form: str = None,
+        resource_key: str = None,
+        template: str = None,
+        value: str = None,
+    ):
+        self.form = form
+        self.resource_key = resource_key
+        self.template = template
+        self.value = value
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.form is not None:
+            result['Form'] = self.form
+        if self.resource_key is not None:
+            result['ResourceKey'] = self.resource_key
+        if self.template is not None:
+            result['Template'] = self.template
+        if self.value is not None:
+            result['Value'] = self.value
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Form') is not None:
+            self.form = m.get('Form')
+        if m.get('ResourceKey') is not None:
+            self.resource_key = m.get('ResourceKey')
+        if m.get('Template') is not None:
+            self.template = m.get('Template')
+        if m.get('Value') is not None:
+            self.value = m.get('Value')
+        return self
+
+
+class ListTargetsResponseBodyDataTargets(TeaModel):
+    def __init__(
+        self,
+        endpoint: str = None,
+        event_bus_name: str = None,
+        id: str = None,
+        param_list: List[ListTargetsResponseBodyDataTargetsParamList] = None,
+        rule_name: str = None,
+        type: str = None,
+    ):
+        self.endpoint = endpoint
+        self.event_bus_name = event_bus_name
+        self.id = id
+        self.param_list = param_list
+        self.rule_name = rule_name
+        self.type = type
+
+    def validate(self):
+        if self.param_list:
+            for k in self.param_list:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.endpoint is not None:
+            result['Endpoint'] = self.endpoint
+        if self.event_bus_name is not None:
+            result['EventBusName'] = self.event_bus_name
+        if self.id is not None:
+            result['Id'] = self.id
+        result['ParamList'] = []
+        if self.param_list is not None:
+            for k in self.param_list:
+                result['ParamList'].append(k.to_map() if k else None)
+        if self.rule_name is not None:
+            result['RuleName'] = self.rule_name
+        if self.type is not None:
+            result['Type'] = self.type
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Endpoint') is not None:
+            self.endpoint = m.get('Endpoint')
+        if m.get('EventBusName') is not None:
+            self.event_bus_name = m.get('EventBusName')
+        if m.get('Id') is not None:
+            self.id = m.get('Id')
+        self.param_list = []
+        if m.get('ParamList') is not None:
+            for k in m.get('ParamList'):
+                temp_model = ListTargetsResponseBodyDataTargetsParamList()
+                self.param_list.append(temp_model.from_map(k))
+        if m.get('RuleName') is not None:
+            self.rule_name = m.get('RuleName')
+        if m.get('Type') is not None:
+            self.type = m.get('Type')
+        return self
+
+
+class ListTargetsResponseBodyData(TeaModel):
+    def __init__(
+        self,
+        next_token: str = None,
+        targets: List[ListTargetsResponseBodyDataTargets] = None,
+        total: int = None,
+    ):
+        self.next_token = next_token
+        self.targets = targets
+        self.total = total
+
+    def validate(self):
+        if self.targets:
+            for k in self.targets:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.next_token is not None:
+            result['NextToken'] = self.next_token
+        result['Targets'] = []
+        if self.targets is not None:
+            for k in self.targets:
+                result['Targets'].append(k.to_map() if k else None)
+        if self.total is not None:
+            result['Total'] = self.total
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('NextToken') is not None:
+            self.next_token = m.get('NextToken')
+        self.targets = []
+        if m.get('Targets') is not None:
+            for k in m.get('Targets'):
+                temp_model = ListTargetsResponseBodyDataTargets()
+                self.targets.append(temp_model.from_map(k))
+        if m.get('Total') is not None:
+            self.total = m.get('Total')
+        return self
+
+
+class ListTargetsResponseBody(TeaModel):
+    def __init__(
+        self,
+        code: str = None,
+        data: ListTargetsResponseBodyData = None,
+        message: str = None,
+        request_id: str = None,
+        success: bool = None,
+    ):
+        self.code = code
+        self.data = data
+        self.message = message
+        self.request_id = request_id
+        self.success = success
+
+    def validate(self):
+        if self.data:
+            self.data.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.data is not None:
+            result['Data'] = self.data.to_map()
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.success is not None:
+            result['Success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Data') is not None:
+            temp_model = ListTargetsResponseBodyData()
+            self.data = temp_model.from_map(m['Data'])
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
+        return self
+
+
+class ListTargetsResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: ListTargetsResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = ListTargetsResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class ListUserDefinedEventSourcesResponseBodyDataEventSourceListSourceHttpEventParameters(TeaModel):
     def __init__(
         self,
         ip: List[str] = None,
         method: List[str] = None,
         referer: List[str] = None,
         security_config: str = None,
```

### Comparing `alibabacloud_eventbridge20200401-1.0.8/alibabacloud_eventbridge20200401.egg-info/PKG-INFO` & `alibabacloud_eventbridge20200401-2.0.0/alibabacloud_eventbridge20200401.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-eventbridge20200401
-Version: 1.0.8
+Version: 2.0.0
 Summary: Alibaba Cloud eventbridge (20200401) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_eventbridge20200401-1.0.8/setup.py` & `alibabacloud_eventbridge20200401-2.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_eventbridge20200401.
 
-Created on 21/04/2023
+Created on 09/06/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_eventbridge20200401"
 NAME = "alibabacloud_eventbridge20200401" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud eventbridge (20200401) SDK Library for Python"
```

