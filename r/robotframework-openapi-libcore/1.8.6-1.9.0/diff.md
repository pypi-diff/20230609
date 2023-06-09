# Comparing `tmp/robotframework_openapi_libcore-1.8.6.tar.gz` & `tmp/robotframework_openapi_libcore-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework_openapi_libcore-1.8.6.tar", max compression
+gzip compressed data, was "robotframework_openapi_libcore-1.9.0.tar", max compression
```

## Comparing `robotframework_openapi_libcore-1.8.6.tar` & `robotframework_openapi_libcore-1.9.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     4693 2023-06-01 13:47:36.261686 robotframework_openapi_libcore-1.8.6/docs/README.md
--rw-r--r--   0        0        0    11558 2021-12-13 14:33:13.481598 robotframework_openapi_libcore-1.8.6/LICENSE
--rw-r--r--   0        0        0     2372 2023-06-01 13:27:50.821095 robotframework_openapi_libcore-1.8.6/pyproject.toml
--rw-r--r--   0        0        0     1297 2021-12-28 14:18:06.991167 robotframework_openapi_libcore-1.8.6/src/OpenApiLibCore/__init__.py
--rw-r--r--   0        0        0     8014 2023-02-17 14:58:53.541795 robotframework_openapi_libcore-1.8.6/src/OpenApiLibCore/dto_base.py
--rw-r--r--   0        0        0     2659 2023-02-17 14:58:53.542831 robotframework_openapi_libcore-1.8.6/src/OpenApiLibCore/dto_utils.py
--rw-r--r--   0        0        0      163 2023-04-20 07:55:08.986947 robotframework_openapi_libcore-1.8.6/src/OpenApiLibCore/oas_cache.py
--rw-r--r--   0        0        0    26880 2023-06-01 13:47:36.184561 robotframework_openapi_libcore-1.8.6/src/OpenApiLibCore/openapi_libcore.libspec
--rw-r--r--   0        0        0    59161 2023-06-01 13:47:32.907232 robotframework_openapi_libcore-1.8.6/src/OpenApiLibCore/openapi_libcore.py
--rw-r--r--   0        0        0    14791 2023-06-01 13:47:32.926184 robotframework_openapi_libcore-1.8.6/src/OpenApiLibCore/value_utils.py
--rw-r--r--   0        0        0     5656 1970-01-01 00:00:00.000000 robotframework_openapi_libcore-1.8.6/setup.py
--rw-r--r--   0        0        0     5867 1970-01-01 00:00:00.000000 robotframework_openapi_libcore-1.8.6/PKG-INFO
+-rw-r--r--   0        0        0     4748 2023-06-09 13:40:52.874546 robotframework_openapi_libcore-1.9.0/docs/README.md
+-rw-r--r--   0        0        0    11558 2021-12-13 14:33:13.481598 robotframework_openapi_libcore-1.9.0/LICENSE
+-rw-r--r--   0        0        0     2374 2023-06-09 13:15:10.704523 robotframework_openapi_libcore-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0     1297 2021-12-28 14:18:06.991167 robotframework_openapi_libcore-1.9.0/src/OpenApiLibCore/__init__.py
+-rw-r--r--   0        0        0     8014 2023-02-17 14:58:53.541795 robotframework_openapi_libcore-1.9.0/src/OpenApiLibCore/dto_base.py
+-rw-r--r--   0        0        0     2659 2023-02-17 14:58:53.542831 robotframework_openapi_libcore-1.9.0/src/OpenApiLibCore/dto_utils.py
+-rw-r--r--   0        0        0      163 2023-04-20 07:55:08.986947 robotframework_openapi_libcore-1.9.0/src/OpenApiLibCore/oas_cache.py
+-rw-r--r--   0        0        0    28654 2023-06-09 13:40:52.807168 robotframework_openapi_libcore-1.9.0/src/OpenApiLibCore/openapi_libcore.libspec
+-rw-r--r--   0        0        0    60706 2023-06-09 13:40:49.228395 robotframework_openapi_libcore-1.9.0/src/OpenApiLibCore/openapi_libcore.py
+-rw-r--r--   0        0        0    14791 2023-06-01 13:47:32.926184 robotframework_openapi_libcore-1.9.0/src/OpenApiLibCore/value_utils.py
+-rw-r--r--   0        0        0     5715 1970-01-01 00:00:00.000000 robotframework_openapi_libcore-1.9.0/setup.py
+-rw-r--r--   0        0        0     5926 1970-01-01 00:00:00.000000 robotframework_openapi_libcore-1.9.0/PKG-INFO
```

### Comparing `robotframework_openapi_libcore-1.8.6/docs/README.md` & `robotframework_openapi_libcore-1.9.0/docs/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -52,31 +52,31 @@
 
 This can be done using the command line interface of a package that is installed as
 a prerequisite for OpenApiLibCore.
 Both a local openapi.json or openapi.yaml file or one hosted by the API server
 can be checked using the `prance validate <reference_to_file>` shell command:
 
 ```shell
-prance validate http://localhost:8000/openapi.json
+prance validate --backend=openapi-spec-validator http://localhost:8000/openapi.json
 Processing "http://localhost:8000/openapi.json"...
  -> Resolving external references.
 Validates OK as OpenAPI 3.0.2!
 
-prance validate /tests/files/petstore_openapi.yaml
+prance validate --backend=openapi-spec-validator /tests/files/petstore_openapi.yaml
 Processing "/tests/files/petstore_openapi.yaml"...
  -> Resolving external references.
 Validates OK as OpenAPI 3.0.2!
 ```
 
 You'll have to change the url or file reference to the location of the openapi
 document for your API.
 
 > Note: Although recursion is technically allowed under the OAS, tool support is limited
-and changing the API to not use recursion is recommended.
-At present OpenApiLibCore has limited support for parsing OpenAPI documents with
+and changing the OAS to not use recursion is recommended.
+OpenApiLibCore has limited support for parsing OpenAPI documents with
 recursion in them. See the `recursion_limit` and `recursion_default` parameters.
 
 If the openapi document passes this validation, the next step is trying to do a test
 run with a minimal test suite.
 The example below can be used, with `source`, `origin` and 'endpoint' altered to
 fit your situation.
```

### Comparing `robotframework_openapi_libcore-1.8.6/LICENSE` & `robotframework_openapi_libcore-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework_openapi_libcore-1.8.6/pyproject.toml` & `robotframework_openapi_libcore-1.9.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name="robotframework-openapi-libcore"
-version = "1.8.6"
+version = "1.9.0"
 description = "A Robot Framework library to facilitate library development for OpenAPI / Swagger APIs."
 license = "Apache-2.0"
 authors = ["Robin Mackaij <r.a.mackaij@gmail.com>"]
 maintainers = ["Robin Mackaij <r.a.mackaij@gmail.com>"]
 readme =  "./docs/README.md"
 homepage = "https://github.com/MarketSquare/robotframework-openapi-libcore"
 classifiers = [
@@ -24,15 +24,15 @@
 [tool.poetry.dependencies]
 python = "^3.8"
 robotframework = ">=4"
 requests = "^2.27"
 prance = {version = "^0.22", extras = ["CLI"]}
 Faker = ">=11"
 rstr = "^3"
-openapi-core = "^0.16"
+openapi-core = "^0.17.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "*"
 isort = "*"
 pylint = "*"
 mypy = "*"
 types-requests = "^2.25.6"
```

### Comparing `robotframework_openapi_libcore-1.8.6/src/OpenApiLibCore/__init__.py` & `robotframework_openapi_libcore-1.9.0/src/OpenApiLibCore/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework_openapi_libcore-1.8.6/src/OpenApiLibCore/dto_base.py` & `robotframework_openapi_libcore-1.9.0/src/OpenApiLibCore/dto_base.py`

 * *Files identical despite different names*

### Comparing `robotframework_openapi_libcore-1.8.6/src/OpenApiLibCore/dto_utils.py` & `robotframework_openapi_libcore-1.9.0/src/OpenApiLibCore/dto_utils.py`

 * *Files identical despite different names*

### Comparing `robotframework_openapi_libcore-1.8.6/src/OpenApiLibCore/openapi_libcore.libspec` & `robotframework_openapi_libcore-1.9.0/src/OpenApiLibCore/openapi_libcore.libspec`

 * *Files 2% similar despite different names*

#### Comparing `robotframework_openapi_libcore-1.8.6/src/OpenApiLibCore/openapi_libcore.libspec` & `robotframework_openapi_libcore-1.9.0/src/OpenApiLibCore/openapi_libcore.libspec`

```diff
@@ -1,16 +1,16 @@
 <?xml version="1.0" encoding="utf-8"?>
-<keywordspec name="OpenApiLibCore" type="LIBRARY" format="HTML" scope="SUITE" generated="2023-06-01T13:47:36+00:00" specversion="4" source="C:\GitHub\robotframework-openapi-libcore\src\OpenApiLibCore\openapi_libcore.py" lineno="379">
-  <version>1.8.6</version>
+<keywordspec name="OpenApiLibCore" type="LIBRARY" format="HTML" scope="SUITE" generated="2023-06-09T13:40:53+00:00" specversion="4" source="C:\GitHub\robotframework-openapi-libcore\src\OpenApiLibCore\openapi_libcore.py" lineno="379">
+  <version>1.9.0</version>
   <doc>&lt;p&gt;Main class providing the keywords and core logic to interact with an OpenAPI server.&lt;/p&gt;
 &lt;p&gt;Visit the &lt;a href=&quot;https://github.com/MarketSquare/robotframework-openapi-libcore&quot;&gt;library page&lt;/a&gt; for an introduction.&lt;/p&gt;</doc>
   <tags/>
   <inits>
     <init name="__init__" lineno="387">
-      <arguments repr="source: str, origin: str = , base_path: str = , mappings_path: str | Path = , username: str = , password: str = , security_token: str = , auth: AuthBase | None = None, cert: str | Tuple[str, str] | None = None, extra_headers: Dict[str, str] | None = None, invalid_property_default_response: int = 422, recursion_limit: int = 1, recursion_default: Any = {}, faker_locale: str | List[str] | None = None, default_id_property_name: str = id">
+      <arguments repr="source: str, origin: str = , base_path: str = , mappings_path: str | Path = , invalid_property_default_response: int = 422, default_id_property_name: str = id, faker_locale: str | List[str] | None = None, recursion_limit: int = 1, recursion_default: Any = {}, username: str = , password: str = , security_token: str = , auth: AuthBase | None = None, cert: str | Tuple[str, str] | None = None, verify_tls: bool | str | None = True, extra_headers: Dict[str, str] | None = None, cookies: Dict[str, str] | RequestsCookieJar | None = None, proxies: Dict[str, str] | None = None">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="source: str">
           <name>source</name>
           <type typedoc="string">str</type>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="false" repr="origin: str = ">
           <name>origin</name>
           <type typedoc="string">str</type>
@@ -23,14 +23,41 @@
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="false" repr="mappings_path: str | Path = ">
           <name>mappings_path</name>
           <type typedoc="string">str</type>
           <type typedoc="Path">Path</type>
           <default/>
         </arg>
+        <arg kind="POSITIONAL_OR_NAMED" required="false" repr="invalid_property_default_response: int = 422">
+          <name>invalid_property_default_response</name>
+          <type typedoc="integer">int</type>
+          <default>422</default>
+        </arg>
+        <arg kind="POSITIONAL_OR_NAMED" required="false" repr="default_id_property_name: str = id">
+          <name>default_id_property_name</name>
+          <type typedoc="string">str</type>
+          <default>id</default>
+        </arg>
+        <arg kind="POSITIONAL_OR_NAMED" required="false" repr="faker_locale: str | List[str] | None = None">
+          <name>faker_locale</name>
+          <type typedoc="string">str</type>
+          <type typedoc="list">List[str]</type>
+          <type typedoc="None">None</type>
+          <default>None</default>
+        </arg>
+        <arg kind="POSITIONAL_OR_NAMED" required="false" repr="recursion_limit: int = 1">
+          <name>recursion_limit</name>
+          <type typedoc="integer">int</type>
+          <default>1</default>
+        </arg>
+        <arg kind="POSITIONAL_OR_NAMED" required="false" repr="recursion_default: Any = {}">
+          <name>recursion_default</name>
+          <type>Any</type>
+          <default>{}</default>
+        </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="false" repr="username: str = ">
           <name>username</name>
           <type typedoc="string">str</type>
           <default/>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="false" repr="password: str = ">
           <name>password</name>
@@ -51,84 +78,88 @@
         <arg kind="POSITIONAL_OR_NAMED" required="false" repr="cert: str | Tuple[str, str] | None = None">
           <name>cert</name>
           <type typedoc="string">str</type>
           <type typedoc="tuple">Tuple[str, str]</type>
           <type typedoc="None">None</type>
           <default>None</default>
         </arg>
+        <arg kind="POSITIONAL_OR_NAMED" required="false" repr="verify_tls: bool | str | None = True">
+          <name>verify_tls</name>
+          <type typedoc="boolean">bool</type>
+          <type typedoc="string">str</type>
+          <type typedoc="None">None</type>
+          <default>True</default>
+        </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="false" repr="extra_headers: Dict[str, str] | None = None">
           <name>extra_headers</name>
           <type typedoc="dictionary">Dict[str, str]</type>
           <type typedoc="None">None</type>
           <default>None</default>
         </arg>
-        <arg kind="POSITIONAL_OR_NAMED" required="false" repr="invalid_property_default_response: int = 422">
-          <name>invalid_property_default_response</name>
-          <type typedoc="integer">int</type>
-          <default>422</default>
-        </arg>
-        <arg kind="POSITIONAL_OR_NAMED" required="false" repr="recursion_limit: int = 1">
-          <name>recursion_limit</name>
-          <type typedoc="integer">int</type>
-          <default>1</default>
-        </arg>
-        <arg kind="POSITIONAL_OR_NAMED" required="false" repr="recursion_default: Any = {}">
-          <name>recursion_default</name>
-          <type>Any</type>
-          <default>{}</default>
-        </arg>
-        <arg kind="POSITIONAL_OR_NAMED" required="false" repr="faker_locale: str | List[str] | None = None">
-          <name>faker_locale</name>
-          <type typedoc="string">str</type>
-          <type typedoc="list">List[str]</type>
+        <arg kind="POSITIONAL_OR_NAMED" required="false" repr="cookies: Dict[str, str] | RequestsCookieJar | None = None">
+          <name>cookies</name>
+          <type typedoc="dictionary">Dict[str, str]</type>
+          <type typedoc="dictionary">RequestsCookieJar</type>
           <type typedoc="None">None</type>
           <default>None</default>
         </arg>
-        <arg kind="POSITIONAL_OR_NAMED" required="false" repr="default_id_property_name: str = id">
-          <name>default_id_property_name</name>
-          <type typedoc="string">str</type>
-          <default>id</default>
+        <arg kind="POSITIONAL_OR_NAMED" required="false" repr="proxies: Dict[str, str] | None = None">
+          <name>proxies</name>
+          <type typedoc="dictionary">Dict[str, str]</type>
+          <type typedoc="None">None</type>
+          <default>None</default>
         </arg>
       </arguments>
-      <doc>&lt;h4&gt;source&lt;/h4&gt;
+      <doc>&lt;h3&gt;Base parameters&lt;/h3&gt;
+&lt;h4&gt;source&lt;/h4&gt;
 &lt;p&gt;An absolute path to an openapi.json or openapi.yaml file or an url to such a file.&lt;/p&gt;
 &lt;h4&gt;origin&lt;/h4&gt;
 &lt;p&gt;The server (and port) of the target server. E.g. &lt;code&gt;https://localhost:8000&lt;/code&gt;&lt;/p&gt;
 &lt;h4&gt;base_path&lt;/h4&gt;
-&lt;p&gt;The routing between &lt;code&gt;origin&lt;/code&gt; and the endpoints as found in the &lt;code&gt;paths&lt;/code&gt; in the openapi document. E.g. &lt;code&gt;/petshop/v2&lt;/code&gt;.&lt;/p&gt;
+&lt;p&gt;The routing between &lt;code&gt;origin&lt;/code&gt; and the endpoints as found in the &lt;code&gt;paths&lt;/code&gt; section in the openapi document. E.g. &lt;code&gt;/petshop/v2&lt;/code&gt;.&lt;/p&gt;
+&lt;h3&gt;API-specific configurations&lt;/h3&gt;
 &lt;h4&gt;mappings_path&lt;/h4&gt;
-&lt;p&gt;See &lt;a href=&quot;https://marketsquare.github.io/robotframework-openapi-libcore/advanced_use.html&quot;&gt;here&lt;/a&gt;.&lt;/p&gt;
+&lt;p&gt;See &lt;a href=&quot;https://marketsquare.github.io/robotframework-openapi-libcore/advanced_use.html&quot;&gt;this page&lt;/a&gt; for an in-depth explanation.&lt;/p&gt;
+&lt;h4&gt;invalid_property_default_response&lt;/h4&gt;
+&lt;p&gt;The default response code for requests with a JSON body that does not comply with the schema. Example: a value outside the specified range or a string value for a property defined as integer in the schema.&lt;/p&gt;
+&lt;h4&gt;default_id_property_name&lt;/h4&gt;
+&lt;p&gt;The default name for the property that identifies a resource (i.e. a unique entity) within the API. The default value for this property name is &lt;code&gt;id&lt;/code&gt;. If the target API uses a different name for all the resources within the API, you can configure it globally using this property.&lt;/p&gt;
+&lt;p&gt;If different property names are used for the unique identifier for different types of resources, an &lt;code&gt;ID_MAPPING&lt;/code&gt; can be implemented using the &lt;code&gt;mappings_path&lt;/code&gt;.&lt;/p&gt;
+&lt;h4&gt;faker_locale&lt;/h4&gt;
+&lt;p&gt;A locale string or list of locale strings to pass to the Faker library to be used in generation of string data for supported format types.&lt;/p&gt;
+&lt;h3&gt;Parsing parameters&lt;/h3&gt;
+&lt;h4&gt;recursion_limit&lt;/h4&gt;
+&lt;p&gt;The recursion depth to which to fully parse recursive references before the &lt;span class=&quot;name&quot;&gt;recursion_default&lt;/span&gt; is used to end the recursion.&lt;/p&gt;
+&lt;h4&gt;recursion_default&lt;/h4&gt;
+&lt;p&gt;The value that is used instead of the referenced schema when the &lt;span class=&quot;name&quot;&gt;recursion_limit&lt;/span&gt; has been reached. The default &lt;span class=&quot;name&quot;&gt;{}&lt;/span&gt; represents an empty object in JSON. Depending on schema definitions, this may cause schema validation errors. If this is the case, 'None' (&lt;code&gt;${NONE}&lt;/code&gt; in Robot Framework) or an empty list can be tried as an alternative.&lt;/p&gt;
+&lt;h3&gt;Security-related parameters&lt;/h3&gt;
+&lt;p&gt;&lt;i&gt;Note: these parameters are equivalent to those in the &lt;code&gt;requests&lt;/code&gt; library.&lt;/i&gt;&lt;/p&gt;
 &lt;h4&gt;username&lt;/h4&gt;
 &lt;p&gt;The username to be used for Basic Authentication.&lt;/p&gt;
 &lt;h4&gt;password&lt;/h4&gt;
 &lt;p&gt;The password to be used for Basic Authentication.&lt;/p&gt;
 &lt;h4&gt;security_token&lt;/h4&gt;
 &lt;p&gt;The token to be used for token based security using the &lt;code&gt;Authorization&lt;/code&gt; header.&lt;/p&gt;
 &lt;h4&gt;auth&lt;/h4&gt;
-&lt;p&gt;A &lt;a href=&quot;https://requests.readthedocs.io/en/latest/api/#authentication&quot;&gt;requests AuthBase instance&lt;/a&gt; to be used for authentication instead of the &lt;code&gt;username&lt;/code&gt; and &lt;code&gt;password&lt;/code&gt;.&lt;/p&gt;
+&lt;p&gt;A &lt;a href=&quot;https://requests.readthedocs.io/en/latest/api/#authentication&quot;&gt;requests &lt;code&gt;AuthBase&lt;/code&gt; instance&lt;/a&gt; to be used for authentication instead of the &lt;code&gt;username&lt;/code&gt; and &lt;code&gt;password&lt;/code&gt;.&lt;/p&gt;
 &lt;h4&gt;cert&lt;/h4&gt;
-&lt;p&gt;The SSL certificate to use with all requests. If string: the path to ssl client cert file (.pem). If tuple, ('cert', 'key') pair.&lt;/p&gt;
+&lt;p&gt;The SSL certificate to use with all requests. If string: the path to ssl client cert file (.pem). If tuple: the ('cert', 'key') pair.&lt;/p&gt;
+&lt;h4&gt;verify_tls&lt;/h4&gt;
+&lt;p&gt;Whether or not to verify the TLS / SSL certificate of the server. If boolean: whether or not to verify the server TLS certificate. If string: path to a CA bundle to use for verification.&lt;/p&gt;
 &lt;h4&gt;extra_headers&lt;/h4&gt;
 &lt;p&gt;A dictionary with extra / custom headers that will be send with every request. This parameter can be used to send headers that are not documented in the openapi document or to provide an API-key.&lt;/p&gt;
-&lt;h4&gt;invalid_property_default_response&lt;/h4&gt;
-&lt;p&gt;The default response code for requests with a JSON body that does not comply with the schema. Example: a value outside the specified range or a string value for a property defined as integer in the schema.&lt;/p&gt;
-&lt;h4&gt;recursion_limit&lt;/h4&gt;
-&lt;p&gt;The recursion depth to which to fully parse recursive references before the &lt;span class=&quot;name&quot;&gt;recursion_default&lt;/span&gt; is used to end the recursion.&lt;/p&gt;
-&lt;h4&gt;recursion_default&lt;/h4&gt;
-&lt;p&gt;The value that is used instead of the referenced schema when the &lt;span class=&quot;name&quot;&gt;recursion_limit&lt;/span&gt; has been reached. The default &lt;span class=&quot;name&quot;&gt;{}&lt;/span&gt; represents an empty object in JSON. Depending on schema definitions, this may cause schema validation errors. If this is the case, &lt;a href=&quot;#type-None&quot; class=&quot;name&quot;&gt;None&lt;/a&gt; (&lt;span class=&quot;name&quot;&gt;${NONE}&lt;/span&gt; in Robot Framework) can be tried as an alternative.&lt;/p&gt;
-&lt;h4&gt;faker_locale&lt;/h4&gt;
-&lt;p&gt;A locale string or list of locale strings to pass to Faker to be used in generation of string data for supported format types.&lt;/p&gt;
-&lt;h4&gt;default_id_property_name&lt;/h4&gt;
-&lt;p&gt;The default name for the property that identifies a resource (i.e. a unique entiry) within the API. The default value for this property name is &lt;span class=&quot;name&quot;&gt;id&lt;/span&gt;. If the target API uses a different name for all the resources within the API, you can configure it globally using this property.&lt;/p&gt;
-&lt;p&gt;If different property names are used for the unique identifier for different types of resources, an &lt;span class=&quot;name&quot;&gt;ID_MAPPING&lt;/span&gt; can be implemented in the &lt;span class=&quot;name&quot;&gt;mappings_path&lt;/span&gt;.&lt;/p&gt;</doc>
-      <shortdoc>=== source === An absolute path to an openapi.json or openapi.yaml file or an url to such a file.</shortdoc>
+&lt;h4&gt;cookies&lt;/h4&gt;
+&lt;p&gt;A dictionary or &lt;a href=&quot;https://docs.python.org/3/library/http.cookiejar.html#http.cookiejar.CookieJar&quot;&gt;CookieJar object&lt;/a&gt; to send with all requests.&lt;/p&gt;
+&lt;h4&gt;proxies&lt;/h4&gt;
+&lt;p&gt;A dictionary of 'protocol': 'proxy url' to use for all requests.&lt;/p&gt;</doc>
+      <shortdoc>== Base parameters ==</shortdoc>
     </init>
   </inits>
   <keywords>
-    <kw name="Authorized Request" lineno="1359">
+    <kw name="Authorized Request" lineno="1395">
       <arguments repr="url: str, method: str, params: Dict[str, Any] | None = None, headers: Dict[str, str] | None = None, json_data: Dict[str, Dict[str, ForwardRef('JSON')] | List[ForwardRef('JSON')] | str | int | float | bool | None] | List[Dict[str, ForwardRef('JSON')] | List[ForwardRef('JSON')] | str | int | float | bool | None] | str | int | float | bool | None = None">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="url: str">
           <name>url</name>
           <type typedoc="string">str</type>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="method: str">
           <name>method</name>
@@ -158,39 +189,39 @@
           <default>None</default>
         </arg>
       </arguments>
       <doc>&lt;p&gt;Perform a request using the security token or authentication set in the library.&lt;/p&gt;
 &lt;p&gt;&amp;gt; Note: provided username / password or auth objects take precedence over token based security&lt;/p&gt;</doc>
       <shortdoc>Perform a request using the security token or authentication set in the library.</shortdoc>
     </kw>
-    <kw name="Ensure In Use" lineno="1263">
+    <kw name="Ensure In Use" lineno="1299">
       <arguments repr="url: str, resource_relation: IdReference">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="url: str">
           <name>url</name>
           <type typedoc="string">str</type>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="resource_relation: IdReference">
           <name>resource_relation</name>
           <type>IdReference</type>
         </arg>
       </arguments>
       <doc>&lt;p&gt;Ensure that the (right-most) &lt;span class=&quot;name&quot;&gt;id&lt;/span&gt; of the resource referenced by the &lt;span class=&quot;name&quot;&gt;url&lt;/span&gt; is used by the resource defined by the &lt;span class=&quot;name&quot;&gt;resource_relation&lt;/span&gt;.&lt;/p&gt;</doc>
       <shortdoc>Ensure that the (right-most) `id` of the resource referenced by the `url` is used by the resource defined by the `resource_relation`.</shortdoc>
     </kw>
-    <kw name="Get Ids From Url" lineno="698">
+    <kw name="Get Ids From Url" lineno="734">
       <arguments repr="url: str">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="url: str">
           <name>url</name>
           <type typedoc="string">str</type>
         </arg>
       </arguments>
       <doc>&lt;p&gt;Perform a GET request on the &lt;span class=&quot;name&quot;&gt;url&lt;/span&gt; and return the list of resource &lt;span class=&quot;name&quot;&gt;ids&lt;/span&gt; from the response.&lt;/p&gt;</doc>
       <shortdoc>Perform a GET request on the `url` and return the list of resource `ids` from the response.</shortdoc>
     </kw>
-    <kw name="Get Invalid Json Data" lineno="1042">
+    <kw name="Get Invalid Json Data" lineno="1078">
       <arguments repr="url: str, method: str, status_code: int, request_data: RequestData">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="url: str">
           <name>url</name>
           <type typedoc="string">str</type>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="method: str">
           <name>method</name>
@@ -205,40 +236,40 @@
           <type>RequestData</type>
         </arg>
       </arguments>
       <doc>&lt;p&gt;Return &lt;span class=&quot;name&quot;&gt;json_data&lt;/span&gt; based on the &lt;span class=&quot;name&quot;&gt;dto&lt;/span&gt; on the &lt;span class=&quot;name&quot;&gt;request_data&lt;/span&gt; that will cause the provided &lt;span class=&quot;name&quot;&gt;status_code&lt;/span&gt; for the &lt;span class=&quot;name&quot;&gt;method&lt;/span&gt; operation on the &lt;span class=&quot;name&quot;&gt;url&lt;/span&gt;.&lt;/p&gt;
 &lt;p&gt;&amp;gt; Note: applicable UniquePropertyValueConstraint and IdReference Relations are considered before changes to &lt;span class=&quot;name&quot;&gt;json_data&lt;/span&gt; are made.&lt;/p&gt;</doc>
       <shortdoc>Return `json_data` based on the `dto` on the `request_data` that will cause the provided `status_code` for the `method` operation on the `url`.</shortdoc>
     </kw>
-    <kw name="Get Invalidated Parameters" lineno="1090">
+    <kw name="Get Invalidated Parameters" lineno="1126">
       <arguments repr="status_code: int, request_data: RequestData">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="status_code: int">
           <name>status_code</name>
           <type typedoc="integer">int</type>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="request_data: RequestData">
           <name>request_data</name>
           <type>RequestData</type>
         </arg>
       </arguments>
       <doc>&lt;p&gt;Returns a version of &lt;span class=&quot;name&quot;&gt;params, headers&lt;/span&gt; as present on &lt;span class=&quot;name&quot;&gt;request_data&lt;/span&gt; that has been modified to cause the provided &lt;span class=&quot;name&quot;&gt;status_code&lt;/span&gt;.&lt;/p&gt;</doc>
       <shortdoc>Returns a version of `params, headers` as present on `request_data` that has been modified to cause the provided `status_code`.</shortdoc>
     </kw>
-    <kw name="Get Invalidated Url" lineno="1008">
+    <kw name="Get Invalidated Url" lineno="1044">
       <arguments repr="valid_url: str">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="valid_url: str">
           <name>valid_url</name>
           <type typedoc="string">str</type>
         </arg>
       </arguments>
       <doc>&lt;p&gt;Return an url with all the path parameters in the &lt;span class=&quot;name&quot;&gt;valid_url&lt;/span&gt; replaced by a random UUID.&lt;/p&gt;
 &lt;p&gt;Raises ValueError if the valid_url cannot be invalidated.&lt;/p&gt;</doc>
       <shortdoc>Return an url with all the path parameters in the `valid_url` replaced by a random UUID.</shortdoc>
     </kw>
-    <kw name="Get Json Data For Dto Class" lineno="918">
+    <kw name="Get Json Data For Dto Class" lineno="954">
       <arguments repr="schema: Dict[str, Any], dto_class: Dto | Type[Dto], operation_id: str = ">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="schema: Dict[str, Any]">
           <name>schema</name>
           <type typedoc="dictionary">Dict[str, Any]</type>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="dto_class: Dto | Type[Dto]">
           <name>dto_class</name>
@@ -250,15 +281,15 @@
           <type typedoc="string">str</type>
           <default/>
         </arg>
       </arguments>
       <doc>&lt;p&gt;Generate a valid (json-compatible) dict for all the &lt;span class=&quot;name&quot;&gt;dto_class&lt;/span&gt; properties.&lt;/p&gt;</doc>
       <shortdoc>Generate a valid (json-compatible) dict for all the `dto_class` properties.</shortdoc>
     </kw>
-    <kw name="Get Json Data With Conflict" lineno="1307">
+    <kw name="Get Json Data With Conflict" lineno="1343">
       <arguments repr="url: str, method: str, dto: Dto, conflict_status_code: int">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="url: str">
           <name>url</name>
           <type typedoc="string">str</type>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="method: str">
           <name>method</name>
@@ -272,54 +303,54 @@
           <name>conflict_status_code</name>
           <type typedoc="integer">int</type>
         </arg>
       </arguments>
       <doc>&lt;p&gt;Return &lt;span class=&quot;name&quot;&gt;json_data&lt;/span&gt; based on the &lt;span class=&quot;name&quot;&gt;UniquePropertyValueConstraint&lt;/span&gt; that must be returned by the &lt;span class=&quot;name&quot;&gt;get_relations&lt;/span&gt; implementation on the &lt;span class=&quot;name&quot;&gt;dto&lt;/span&gt; for the given &lt;span class=&quot;name&quot;&gt;conflict_status_code&lt;/span&gt;.&lt;/p&gt;</doc>
       <shortdoc>Return `json_data` based on the `UniquePropertyValueConstraint` that must be returned by the `get_relations` implementation on the `dto` for the given `conflict_status_code`.</shortdoc>
     </kw>
-    <kw name="Get Parameterized Endpoint From Url" lineno="1030">
+    <kw name="Get Parameterized Endpoint From Url" lineno="1066">
       <arguments repr="url: str">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="url: str">
           <name>url</name>
           <type typedoc="string">str</type>
         </arg>
       </arguments>
       <doc>&lt;p&gt;Return the endpoint as found in the &lt;span class=&quot;name&quot;&gt;paths&lt;/span&gt; section based on the given &lt;span class=&quot;name&quot;&gt;url&lt;/span&gt;.&lt;/p&gt;</doc>
       <shortdoc>Return the endpoint as found in the `paths` section based on the given `url`.</shortdoc>
     </kw>
-    <kw name="Get Request Data" lineno="738">
+    <kw name="Get Request Data" lineno="774">
       <arguments repr="endpoint: str, method: str">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="endpoint: str">
           <name>endpoint</name>
           <type typedoc="string">str</type>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="method: str">
           <name>method</name>
           <type typedoc="string">str</type>
         </arg>
       </arguments>
       <doc>&lt;p&gt;Return an object with valid request data for body, headers and query params.&lt;/p&gt;</doc>
       <shortdoc>Return an object with valid request data for body, headers and query params.</shortdoc>
     </kw>
-    <kw name="Get Valid Id For Endpoint" lineno="610">
+    <kw name="Get Valid Id For Endpoint" lineno="646">
       <arguments repr="endpoint: str, method: str">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="endpoint: str">
           <name>endpoint</name>
           <type typedoc="string">str</type>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="method: str">
           <name>method</name>
           <type typedoc="string">str</type>
         </arg>
       </arguments>
       <doc>&lt;p&gt;Support keyword that returns the &lt;span class=&quot;name&quot;&gt;id&lt;/span&gt; for an existing resource at &lt;span class=&quot;name&quot;&gt;endpoint&lt;/span&gt;.&lt;/p&gt;
 &lt;p&gt;To prevent resource conflicts with other test cases, a new resource is created (POST) if possible.&lt;/p&gt;</doc>
       <shortdoc>Support keyword that returns the `id` for an existing resource at `endpoint`.</shortdoc>
     </kw>
-    <kw name="Get Valid Url" lineno="570">
+    <kw name="Get Valid Url" lineno="606">
       <arguments repr="endpoint: str, method: str">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="endpoint: str">
           <name>endpoint</name>
           <type typedoc="string">str</type>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="method: str">
           <name>method</name>
@@ -340,14 +371,15 @@
       <accepts>
         <type>string</type>
         <type>integer</type>
         <type>float</type>
         <type>None</type>
       </accepts>
       <usages>
+        <usage>__init__</usage>
         <usage>Authorized Request</usage>
       </usages>
     </type>
     <type name="dictionary" type="Standard">
       <doc>&lt;p&gt;Strings must be Python &lt;a href=&quot;https://docs.python.org/library/stdtypes.html#dict&quot;&gt;dictionary&lt;/a&gt; literals. They are converted to actual dictionaries using the &lt;a href=&quot;https://docs.python.org/library/ast.html#ast.literal_eval&quot;&gt;ast.literal_eval&lt;/a&gt; function. They can contain any values &lt;code&gt;ast.literal_eval&lt;/code&gt; supports, including dictionaries and other containers.&lt;/p&gt;
 &lt;p&gt;If the type has nested types like &lt;code&gt;dict[str, int]&lt;/code&gt;, items are converted to those types automatically. This in new in Robot Framework 6.0.&lt;/p&gt;
 &lt;p&gt;Examples: &lt;code&gt;{'a': 1, 'b': 2}&lt;/code&gt;, &lt;code&gt;{'key': 1, 'nested': {'key': 2}}&lt;/code&gt;&lt;/p&gt;</doc>
```

### Comparing `robotframework_openapi_libcore-1.8.6/src/OpenApiLibCore/openapi_libcore.py` & `robotframework_openapi_libcore-1.9.0/src/OpenApiLibCore/openapi_libcore.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,31 +50,31 @@
 
 This can be done using the command line interface of a package that is installed as
 a prerequisite for OpenApiLibCore.
 Both a local openapi.json or openapi.yaml file or one hosted by the API server
 can be checked using the `prance validate <reference_to_file>` shell command:
 
 ```shell
-prance validate http://localhost:8000/openapi.json
+prance validate --backend=openapi-spec-validator http://localhost:8000/openapi.json
 Processing "http://localhost:8000/openapi.json"...
  -> Resolving external references.
 Validates OK as OpenAPI 3.0.2!
 
-prance validate /tests/files/petstore_openapi.yaml
+prance validate --backend=openapi-spec-validator /tests/files/petstore_openapi.yaml
 Processing "/tests/files/petstore_openapi.yaml"...
  -> Resolving external references.
 Validates OK as OpenAPI 3.0.2!
 ```
 
 You'll have to change the url or file reference to the location of the openapi
 document for your API.
 
 > Note: Although recursion is technically allowed under the OAS, tool support is limited
-and changing the API to not use recursion is recommended.
-At present OpenApiLibCore has limited support for parsing OpenAPI documents with
+and changing the OAS to not use recursion is recommended.
+OpenApiLibCore has limited support for parsing OpenAPI documents with
 recursion in them. See the `recursion_limit` and `recursion_default` parameters.
 
 If the openapi document passes this validation, the next step is trying to do a test
 run with a minimal test suite.
 The example below can be used, with `source`, `origin` and 'endpoint' altered to
 fit your situation.
 
@@ -126,24 +126,24 @@
 from itertools import zip_longest
 from logging import getLogger
 from pathlib import Path
 from random import choice
 from typing import Any, Callable, Dict, List, Optional, Set, Tuple, Type, Union
 from uuid import uuid4
 
-from openapi_core import Spec
+from openapi_core import Spec, openapi_response_validator
 from openapi_core.contrib.requests import (
     RequestsOpenAPIRequest,
     RequestsOpenAPIResponse,
 )
-from openapi_core.validation.response import openapi_response_validator
 from prance import ResolvingParser, ValidationError
 from prance.util.url import ResolutionError
 from requests import Response, Session
 from requests.auth import AuthBase, HTTPBasicAuth
+from requests.cookies import RequestsCookieJar as CookieJar
 from robot.api.deco import keyword, library
 from robot.libraries.BuiltIn import BuiltIn
 
 from OpenApiLibCore import value_utils
 from OpenApiLibCore.dto_base import (
     NOT_SET,
     Dto,
@@ -386,91 +386,120 @@
 
     def __init__(  # pylint: disable=too-many-arguments, too-many-locals, dangerous-default-value
         self,
         source: str,
         origin: str = "",
         base_path: str = "",
         mappings_path: Union[str, Path] = "",
+        invalid_property_default_response: int = 422,
+        default_id_property_name: str = "id",
+        faker_locale: Optional[Union[str, List[str]]] = None,
+        recursion_limit: int = 1,
+        recursion_default: Any = {},
         username: str = "",
         password: str = "",
         security_token: str = "",
         auth: Optional[AuthBase] = None,
         cert: Optional[Union[str, Tuple[str, str]]] = None,
+        verify_tls: Optional[Union[bool, str]] = True,
         extra_headers: Optional[Dict[str, str]] = None,
-        invalid_property_default_response: int = 422,
-        recursion_limit: int = 1,
-        recursion_default: Any = {},
-        faker_locale: Optional[Union[str, List[str]]] = None,
-        default_id_property_name: str = "id",
+        cookies: Optional[Union[Dict[str, str], CookieJar]] = None,
+        proxies: Optional[Dict[str, str]] = None,
     ) -> None:
         """
+        == Base parameters ==
+
         === source ===
         An absolute path to an openapi.json or openapi.yaml file or an url to such a file.
 
         === origin ===
         The server (and port) of the target server. E.g. ``https://localhost:8000``
 
         === base_path ===
-        The routing between ``origin`` and the endpoints as found in the ``paths`` in the
-        openapi document. E.g. ``/petshop/v2``.
+        The routing between ``origin`` and the endpoints as found in the ``paths``
+        section in the openapi document.
+        E.g. ``/petshop/v2``.
+
+        == API-specific configurations ==
 
         === mappings_path ===
-        See [https://marketsquare.github.io/robotframework-openapi-libcore/advanced_use.html | here].
+        See [https://marketsquare.github.io/robotframework-openapi-libcore/advanced_use.html | this page]
+        for an in-depth explanation.
+
+        === invalid_property_default_response ===
+        The default response code for requests with a JSON body that does not comply
+        with the schema.
+        Example: a value outside the specified range or a string value
+        for a property defined as integer in the schema.
+
+        === default_id_property_name ===
+        The default name for the property that identifies a resource (i.e. a unique
+        entity) within the API.
+        The default value for this property name is ``id``.
+        If the target API uses a different name for all the resources within the API,
+        you can configure it globally using this property.
+
+        If different property names are used for the unique identifier for different
+        types of resources, an ``ID_MAPPING`` can be implemented using the ``mappings_path``.
+
+        === faker_locale ===
+        A locale string or list of locale strings to pass to the Faker library to be
+        used in generation of string data for supported format types.
+
+        == Parsing parameters ==
+
+        === recursion_limit ===
+        The recursion depth to which to fully parse recursive references before the
+        `recursion_default` is used to end the recursion.
+
+        === recursion_default ===
+        The value that is used instead of the referenced schema when the
+        `recursion_limit` has been reached.
+        The default `{}` represents an empty object in JSON.
+        Depending on schema definitions, this may cause schema validation errors.
+        If this is the case, 'None' (``${NONE}`` in Robot Framework) or an empty list
+        can be tried as an alternative.
+
+        == Security-related parameters ==
+        _Note: these parameters are equivalent to those in the ``requests`` library._
 
         === username ===
         The username to be used for Basic Authentication.
 
         === password ===
         The password to be used for Basic Authentication.
 
         === security_token ===
         The token to be used for token based security using the ``Authorization`` header.
 
         === auth ===
-        A [https://requests.readthedocs.io/en/latest/api/#authentication | requests AuthBase instance]
+        A [https://requests.readthedocs.io/en/latest/api/#authentication | requests ``AuthBase`` instance]
         to be used for authentication instead of the ``username`` and ``password``.
 
         === cert ===
         The SSL certificate to use with all requests.
-        If string: the path to ssl client cert file (.pem). If tuple, ('cert', 'key') pair.
+        If string: the path to ssl client cert file (.pem).
+        If tuple: the ('cert', 'key') pair.
+
+        === verify_tls ===
+        Whether or not to verify the TLS / SSL certificate of the server.
+        If boolean: whether or not to verify the server TLS certificate.
+        If string: path to a CA bundle to use for verification.
 
         === extra_headers ===
         A dictionary with extra / custom headers that will be send with every request.
         This parameter can be used to send headers that are not documented in the
         openapi document or to provide an API-key.
 
-        === invalid_property_default_response ===
-        The default response code for requests with a JSON body that does not comply with
-        the schema. Example: a value outside the specified range or a string value for a
-        property defined as integer in the schema.
-
-        === recursion_limit ===
-        The recursion depth to which to fully parse recursive references before the
-        `recursion_default` is used to end the recursion.
+        === cookies ===
+        A dictionary or [https://docs.python.org/3/library/http.cookiejar.html#http.cookiejar.CookieJar | CookieJar object]
+        to send with all requests.
 
-        === recursion_default ===
-        The value that is used instead of the referenced schema when the
-        `recursion_limit` has been reached. The default `{}` represents an empty
-        object in JSON. Depending on schema definitions, this may cause schema
-        validation errors. If this is the case, `None` (`${NONE}` in Robot Framework)
-        can be tried as an alternative.
-
-        === faker_locale ===
-        A locale string or list of locale strings to pass to Faker to be used in
-        generation of string data for supported format types.
-
-        === default_id_property_name ===
-        The default name for the property that identifies a resource (i.e. a unique
-        entiry) within the API.
-        The default value for this property name is `id`.
-        If the target API uses a different name for all the resources within the API,
-        you can configure it globally using this property.
-
-        If different property names are used for the unique identifier for different
-        types of resources, an `ID_MAPPING` can be implemented in the `mappings_path`.
+        === proxies ===
+        A dictionary of 'protocol': 'proxy url' to use for all requests.
         """
         try:
 
             def recursion_limit_handler(limit, refstring, recursions):
                 return recursion_default
 
             # Since parsing of the OAS and creating the Spec can take a long time,
@@ -512,16 +541,23 @@
         self.base_url = f"{self.origin}{base_path}"
         # only username and password, security_token or auth object should be provided
         # if multiple are provided, username and password take precedence
         self.security_token = security_token
         self.auth = auth
         if username and password:
             self.auth = HTTPBasicAuth(username, password)
+        # Robot Framework does not allow users to create tuples and requests
+        # does not accept lists, so perform the conversion here
+        if isinstance(cert, list):
+            cert = tuple(cert)
         self.cert = cert
+        self.verify = verify_tls
         self.extra_headers = extra_headers
+        self.cookies = cookies
+        self.proxies = proxies
         self.invalid_property_default_response = invalid_property_default_response
         if mappings_path and str(mappings_path) != ".":
             mappings_path = Path(mappings_path)
             if not mappings_path.is_file():
                 logger.warning(
                     f"mappings_path '{mappings_path}' is not a Python module."
                 )
@@ -1380,13 +1416,15 @@
         headers = {k: str(v) for k, v in headers.items()}
         response = self.session.request(
             url=url,
             method=method,
             params=params,
             headers=headers,
             json=json_data,
+            cookies=self.cookies,
             auth=self.auth,
+            proxies=self.proxies,
+            verify=self.verify,
             cert=self.cert,
-            verify=False,
         )
         logger.debug(f"Response text: {response.text}")
         return response
```

### Comparing `robotframework_openapi_libcore-1.8.6/src/OpenApiLibCore/value_utils.py` & `robotframework_openapi_libcore-1.9.0/src/OpenApiLibCore/value_utils.py`

 * *Files identical despite different names*

### Comparing `robotframework_openapi_libcore-1.8.6/setup.py` & `robotframework_openapi_libcore-1.9.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,25 +8,25 @@
 ['OpenApiLibCore']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['Faker>=11',
- 'openapi-core>=0.16,<0.17',
+ 'openapi-core>=0.17.0,<0.18.0',
  'prance[cli]>=0.22,<0.23',
  'requests>=2.27,<3.0',
  'robotframework>=4',
  'rstr>=3,<4']
 
 setup_kwargs = {
     'name': 'robotframework-openapi-libcore',
-    'version': '1.8.6',
+    'version': '1.9.0',
     'description': 'A Robot Framework library to facilitate library development for OpenAPI / Swagger APIs.',
-    'long_description': '---\n---\n\n# OpenApiLibCore for Robot Framework\n\nThe OpenApiLibCore library is a utility library that is meant to simplify creation\nof other Robot Framework libraries for API testing based on the information in\nan OpenAPI document (also known as Swagger document).\nThis document explains how to use the OpenApiLibCore library.\n\nMy RoboCon 2022 talk about OpenApiDriver and OpenApiLibCore can be found\n[here](https://www.youtube.com/watch?v=7YWZEHxk9Ps)\n\nFor more information about Robot Framework, see http://robotframework.org.\n\n---\n\n> Note: OpenApiLibCore is still being developed so there are currently\nrestrictions / limitations that you may encounter when using this library to run\ntests against an API. See [Limitations](#limitations) for details.\n\n---\n\n## Installation\n\nIf you already have Python >= 3.8 with pip installed, you can simply run:\n\n`pip install --upgrade robotframework-openapi-libcore`\n\n---\n\n## OpenAPI (aka Swagger)\n\nThe OpenAPI Specification (OAS) defines a standard, language-agnostic interface\nto RESTful APIs, see https://swagger.io/specification/\n\nThe OpenApiLibCore implements a number of Robot Framework keywords that make it\neasy to interact with an OpenAPI implementation by using the information in the\nopenapi document (Swagger file), for examply by automatic generation of valid values\nfor requests based on the schema information in the document.\n\n> Note: OpenApiLibCore is designed for APIs based on the OAS v3\nThe library has not been tested for APIs based on the OAS v2.\n\n---\n\n## Getting started\n\nBefore trying to use the keywords exposed by OpenApiLibCore on the target API\nit\'s recommended to first ensure that the openapi document for the API is valid\nunder the OpenAPI Specification.\n\nThis can be done using the command line interface of a package that is installed as\na prerequisite for OpenApiLibCore.\nBoth a local openapi.json or openapi.yaml file or one hosted by the API server\ncan be checked using the `prance validate <reference_to_file>` shell command:\n\n```shell\nprance validate http://localhost:8000/openapi.json\nProcessing "http://localhost:8000/openapi.json"...\n -> Resolving external references.\nValidates OK as OpenAPI 3.0.2!\n\nprance validate /tests/files/petstore_openapi.yaml\nProcessing "/tests/files/petstore_openapi.yaml"...\n -> Resolving external references.\nValidates OK as OpenAPI 3.0.2!\n```\n\nYou\'ll have to change the url or file reference to the location of the openapi\ndocument for your API.\n\n> Note: Although recursion is technically allowed under the OAS, tool support is limited\nand changing the API to not use recursion is recommended.\nAt present OpenApiLibCore has limited support for parsing OpenAPI documents with\nrecursion in them. See the `recursion_limit` and `recursion_default` parameters.\n\nIf the openapi document passes this validation, the next step is trying to do a test\nrun with a minimal test suite.\nThe example below can be used, with `source`, `origin` and \'endpoint\' altered to\nfit your situation.\n\n``` robotframework\n*** Settings ***\nLibrary            OpenApiLibCore\n...                    source=http://localhost:8000/openapi.json\n...                    origin=http://localhost:8000\n\n*** Test Cases ***\nGetting Started\n    ${url}=    Get Valid Url    endpoint=/employees/{employee_id}   method=get\n\n```\n\nRunning the above suite for the first time may result in an error / failed test.\nYou should look at the Robot Framework `log.html` to determine the reasons\nfor the failing tests.\nDepending on the reasons for the failures, different solutions are possible.\n\nDetails about the OpenApiLibCore library parameters and keywords that you may need can be found\n[here](https://marketsquare.github.io/robotframework-openapi-libcore/openapi_libcore.html).\n\nThe OpenApiLibCore also support handling of relations between resources within the scope\nof the API being validated as well as handling dependencies on resources outside the\nscope of the API. In addition there is support for handling restrictions on the values\nof parameters and properties.\n\nDetails about the `mappings_path` variable usage can be found\n[here](https://marketsquare.github.io/robotframework-openapi-libcore/advanced_use.html).\n\n---\n\n## Limitations\n\nThere are currently a number of limitations to supported API structures, supported\ndata types and properties. The following list details the most important ones:\n- Only JSON request and response bodies are supported.\n- No support for per-endpoint authorization levels.\n- Parsing of OAS 3.1 documents is supported by the parsing tools, but runtime behavior is untested.\n\n',
+    'long_description': '---\n---\n\n# OpenApiLibCore for Robot Framework\n\nThe OpenApiLibCore library is a utility library that is meant to simplify creation\nof other Robot Framework libraries for API testing based on the information in\nan OpenAPI document (also known as Swagger document).\nThis document explains how to use the OpenApiLibCore library.\n\nMy RoboCon 2022 talk about OpenApiDriver and OpenApiLibCore can be found\n[here](https://www.youtube.com/watch?v=7YWZEHxk9Ps)\n\nFor more information about Robot Framework, see http://robotframework.org.\n\n---\n\n> Note: OpenApiLibCore is still being developed so there are currently\nrestrictions / limitations that you may encounter when using this library to run\ntests against an API. See [Limitations](#limitations) for details.\n\n---\n\n## Installation\n\nIf you already have Python >= 3.8 with pip installed, you can simply run:\n\n`pip install --upgrade robotframework-openapi-libcore`\n\n---\n\n## OpenAPI (aka Swagger)\n\nThe OpenAPI Specification (OAS) defines a standard, language-agnostic interface\nto RESTful APIs, see https://swagger.io/specification/\n\nThe OpenApiLibCore implements a number of Robot Framework keywords that make it\neasy to interact with an OpenAPI implementation by using the information in the\nopenapi document (Swagger file), for examply by automatic generation of valid values\nfor requests based on the schema information in the document.\n\n> Note: OpenApiLibCore is designed for APIs based on the OAS v3\nThe library has not been tested for APIs based on the OAS v2.\n\n---\n\n## Getting started\n\nBefore trying to use the keywords exposed by OpenApiLibCore on the target API\nit\'s recommended to first ensure that the openapi document for the API is valid\nunder the OpenAPI Specification.\n\nThis can be done using the command line interface of a package that is installed as\na prerequisite for OpenApiLibCore.\nBoth a local openapi.json or openapi.yaml file or one hosted by the API server\ncan be checked using the `prance validate <reference_to_file>` shell command:\n\n```shell\nprance validate --backend=openapi-spec-validator http://localhost:8000/openapi.json\nProcessing "http://localhost:8000/openapi.json"...\n -> Resolving external references.\nValidates OK as OpenAPI 3.0.2!\n\nprance validate --backend=openapi-spec-validator /tests/files/petstore_openapi.yaml\nProcessing "/tests/files/petstore_openapi.yaml"...\n -> Resolving external references.\nValidates OK as OpenAPI 3.0.2!\n```\n\nYou\'ll have to change the url or file reference to the location of the openapi\ndocument for your API.\n\n> Note: Although recursion is technically allowed under the OAS, tool support is limited\nand changing the OAS to not use recursion is recommended.\nOpenApiLibCore has limited support for parsing OpenAPI documents with\nrecursion in them. See the `recursion_limit` and `recursion_default` parameters.\n\nIf the openapi document passes this validation, the next step is trying to do a test\nrun with a minimal test suite.\nThe example below can be used, with `source`, `origin` and \'endpoint\' altered to\nfit your situation.\n\n``` robotframework\n*** Settings ***\nLibrary            OpenApiLibCore\n...                    source=http://localhost:8000/openapi.json\n...                    origin=http://localhost:8000\n\n*** Test Cases ***\nGetting Started\n    ${url}=    Get Valid Url    endpoint=/employees/{employee_id}   method=get\n\n```\n\nRunning the above suite for the first time may result in an error / failed test.\nYou should look at the Robot Framework `log.html` to determine the reasons\nfor the failing tests.\nDepending on the reasons for the failures, different solutions are possible.\n\nDetails about the OpenApiLibCore library parameters and keywords that you may need can be found\n[here](https://marketsquare.github.io/robotframework-openapi-libcore/openapi_libcore.html).\n\nThe OpenApiLibCore also support handling of relations between resources within the scope\nof the API being validated as well as handling dependencies on resources outside the\nscope of the API. In addition there is support for handling restrictions on the values\nof parameters and properties.\n\nDetails about the `mappings_path` variable usage can be found\n[here](https://marketsquare.github.io/robotframework-openapi-libcore/advanced_use.html).\n\n---\n\n## Limitations\n\nThere are currently a number of limitations to supported API structures, supported\ndata types and properties. The following list details the most important ones:\n- Only JSON request and response bodies are supported.\n- No support for per-endpoint authorization levels.\n- Parsing of OAS 3.1 documents is supported by the parsing tools, but runtime behavior is untested.\n\n',
     'author': 'Robin Mackaij',
     'author_email': 'r.a.mackaij@gmail.com',
     'maintainer': 'Robin Mackaij',
     'maintainer_email': 'r.a.mackaij@gmail.com',
     'url': 'https://github.com/MarketSquare/robotframework-openapi-libcore',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `robotframework_openapi_libcore-1.8.6/PKG-INFO` & `robotframework_openapi_libcore-1.9.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-openapi-libcore
-Version: 1.8.6
+Version: 1.9.0
 Summary: A Robot Framework library to facilitate library development for OpenAPI / Swagger APIs.
 Home-page: https://github.com/MarketSquare/robotframework-openapi-libcore
 License: Apache-2.0
 Author: Robin Mackaij
 Author-email: r.a.mackaij@gmail.com
 Maintainer: Robin Mackaij
 Maintainer-email: r.a.mackaij@gmail.com
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Software Development :: Testing :: Acceptance
 Requires-Dist: Faker (>=11)
-Requires-Dist: openapi-core (>=0.16,<0.17)
+Requires-Dist: openapi-core (>=0.17.0,<0.18.0)
 Requires-Dist: prance[cli] (>=0.22,<0.23)
 Requires-Dist: requests (>=2.27,<3.0)
 Requires-Dist: robotframework (>=4)
 Requires-Dist: rstr (>=3,<4)
 Description-Content-Type: text/markdown
 
 ---
@@ -83,31 +83,31 @@
 
 This can be done using the command line interface of a package that is installed as
 a prerequisite for OpenApiLibCore.
 Both a local openapi.json or openapi.yaml file or one hosted by the API server
 can be checked using the `prance validate <reference_to_file>` shell command:
 
 ```shell
-prance validate http://localhost:8000/openapi.json
+prance validate --backend=openapi-spec-validator http://localhost:8000/openapi.json
 Processing "http://localhost:8000/openapi.json"...
  -> Resolving external references.
 Validates OK as OpenAPI 3.0.2!
 
-prance validate /tests/files/petstore_openapi.yaml
+prance validate --backend=openapi-spec-validator /tests/files/petstore_openapi.yaml
 Processing "/tests/files/petstore_openapi.yaml"...
  -> Resolving external references.
 Validates OK as OpenAPI 3.0.2!
 ```
 
 You'll have to change the url or file reference to the location of the openapi
 document for your API.
 
 > Note: Although recursion is technically allowed under the OAS, tool support is limited
-and changing the API to not use recursion is recommended.
-At present OpenApiLibCore has limited support for parsing OpenAPI documents with
+and changing the OAS to not use recursion is recommended.
+OpenApiLibCore has limited support for parsing OpenAPI documents with
 recursion in them. See the `recursion_limit` and `recursion_default` parameters.
 
 If the openapi document passes this validation, the next step is trying to do a test
 run with a minimal test suite.
 The example below can be used, with `source`, `origin` and 'endpoint' altered to
 fit your situation.
```

