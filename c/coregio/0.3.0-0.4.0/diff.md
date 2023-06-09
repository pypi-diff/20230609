# Comparing `tmp/coregio-0.3.0.tar.gz` & `tmp/coregio-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coregio-0.3.0.tar", last modified: Fri Jun  2 13:19:25 2023, max compression
+gzip compressed data, was "coregio-0.4.0.tar", last modified: Fri Jun  9 14:08:28 2023, max compression
```

## Comparing `coregio-0.3.0.tar` & `coregio-0.4.0.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:19:25.646465 coregio-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-02 13:19:25.646465 coregio-0.3.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:19:25.646465 coregio-0.3.0/coregio/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 13:19:16.000000 coregio-0.3.0/coregio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11821 2023-06-02 13:19:16.000000 coregio-0.3.0/coregio/registry_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-06-02 13:19:16.000000 coregio-0.3.0/coregio/registry_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-06-02 13:19:16.000000 coregio-0.3.0/coregio/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:19:25.646465 coregio-0.3.0/coregio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-02 13:19:25.000000 coregio-0.3.0/coregio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-02 13:19:25.000000 coregio-0.3.0/coregio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 13:19:25.000000 coregio-0.3.0/coregio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-02 13:19:25.000000 coregio-0.3.0/coregio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-02 13:19:25.000000 coregio-0.3.0/coregio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-02 13:19:16.000000 coregio-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 13:19:25.646465 coregio-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:19:25.646465 coregio-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     8316 2023-06-02 13:19:16.000000 coregio-0.3.0/tests/test_registry_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-06-02 13:19:16.000000 coregio-0.3.0/tests/test_registry_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-02 13:19:16.000000 coregio-0.3.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:08:28.698244 coregio-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-06-09 14:08:20.000000 coregio-0.4.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6595 2023-06-09 14:08:28.698244 coregio-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4465 2023-06-09 14:08:20.000000 coregio-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:08:28.694244 coregio-0.4.0/coregio/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 14:08:20.000000 coregio-0.4.0/coregio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12280 2023-06-09 14:08:20.000000 coregio-0.4.0/coregio/registry_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10017 2023-06-09 14:08:20.000000 coregio-0.4.0/coregio/registry_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-06-09 14:08:20.000000 coregio-0.4.0/coregio/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:08:28.694244 coregio-0.4.0/coregio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6595 2023-06-09 14:08:28.000000 coregio-0.4.0/coregio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-09 14:08:28.000000 coregio-0.4.0/coregio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 14:08:28.000000 coregio-0.4.0/coregio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-09 14:08:28.000000 coregio-0.4.0/coregio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-09 14:08:28.000000 coregio-0.4.0/coregio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-06-09 14:08:20.000000 coregio-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 14:08:28.698244 coregio-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:08:28.694244 coregio-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7978 2023-06-09 14:08:20.000000 coregio-0.4.0/tests/test_registry_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3491 2023-06-09 14:08:20.000000 coregio-0.4.0/tests/test_registry_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-09 14:08:20.000000 coregio-0.4.0/tests/test_utils.py
```

### Comparing `coregio-0.3.0/coregio/registry_api.py` & `coregio-0.4.0/coregio/registry_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import re
 from typing import Any, Dict, List, Optional, Callable
 from urllib.parse import urljoin, urlparse
 
 import requests
 
 from coregio import utils
-from coregio.registry_auth import HTTPBearerAuth, HTTPBasicAuthWithB64
+from coregio.registry_auth import HTTPBearerAuth, HTTPOAuth2, HTTPBasicAuthWithB64
 
 LOGGER = logging.getLogger(__name__)
 
 
 ACCEPT_HEADERS = {
     "oci_index": "application/vnd.oci.image.index.v1+json",
     "oci_manifest": "application/vnd.oci.image.manifest.v1+json",
@@ -43,27 +43,34 @@
     # Timeouts (connect, read) for HTTP requests
     # (see https://requests.readthedocs.io/en/latest/user/advanced/#timeouts)
     # Use a low connect timeout to fail early when trying to connect to an
     # endpoint that is firewalled (dropping packets)
     DEFAULT_TIMEOUT = (7.0, 15.0)
 
     def __init__(
-        self, url: str, docker_cfg: Optional[str] = None, session: Optional[Any] = None
+        self,
+        url: str,
+        docker_cfg: Optional[str] = None,
+        session: Optional[Any] = None,
+        proxy: Optional[str] = None,
     ) -> None:
         """
         Args:
         url (str): URL of the registry to auth to
         docker_cfg (Optional, str): DockerConfigJson string
         """
 
         self.url = SPECIAL_DOCKER_ALIASES.get(url, url)
         self._original_url = url
         self.docker_cfg = docker_cfg
 
         self.session = session or requests.Session()
+        self.proxy = proxy
+
+        self.auth_header = None
 
     def _get_auth_token(self) -> Any:
         """
         Extract registry auth token from docker_config_json.
 
         Returns:
             Any: Registry auth token (base64 encoded) if available
@@ -78,14 +85,18 @@
             return None
 
         registry_auths = docker_cfg_json.get("auths", {})
         auth = self._select_registry_auth_token_from_docker_config(registry_auths)
         if not auth:
             return None
 
+        # if this is oauth2 auth, token is in identity_token
+        if auth.get("identitytoken"):
+            return auth["identitytoken"]
+        # otherwise use auth
         return auth.get("auth")
 
     def _select_registry_auth_token_from_docker_config(
         self, registry_auths: Dict[str, Any]
     ) -> Any:
         """
         Select auth from docker config by given registry key.
@@ -150,15 +161,15 @@
         Auth is set to use Docker config json file.
 
         Returns:
             requests.Session: Registry session
         """
 
         auth_token = self._get_auth_token()
-        self.session.auth = auth_class(auth_token)
+        self.session.auth = auth_class(auth_token, proxy=self.proxy)
         utils.add_session_retries(self.session)
 
         return self.session
 
     def _get(
         self,
         full_url: str,
@@ -180,29 +191,30 @@
             headers (Optional[Dict[str, Any]], optional): Optional request headers.
                 Defaults to None.
             verify (bool, optional): Optional request verify flag. Defaults to True.
 
         Returns:
             requests.Response: HTTP response object
         """
-
         # Registry uses different auth methods and we don't know which one to use until
         # we make a request. This loop iterates over several methods and make requests
         # until it successfully returns valid response
-        for auth_method in (HTTPBearerAuth, HTTPBasicAuthWithB64):
+        for auth_method in (HTTPBearerAuth, HTTPOAuth2, HTTPBasicAuthWithB64):
             session = self._get_session(auth_method)
 
             resp = session.get(
                 full_url,
                 params=params,
                 headers=headers,
                 verify=verify,
                 timeout=self.DEFAULT_TIMEOUT,
+                proxies={"https": self.proxy} if self.proxy else None,
             )
 
+            self.auth_header = session.auth.auth_header
             if resp.status_code != 401:
                 return resp
             LOGGER.debug(
                 "Auth method %s was un-successful. Trying another one. %s",
                 auth_method,
                 full_url,
             )
```

### Comparing `coregio-0.3.0/coregio/utils.py` & `coregio-0.4.0/coregio/utils.py`

 * *Files identical despite different names*

### Comparing `coregio-0.3.0/tests/test_registry_api.py` & `coregio-0.4.0/tests/test_registry_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 @pytest.mark.parametrize(
     ["registry", "cfg", "auth", "token"],
     [
         ("quay.io", None, None, None),
         ("quay.io", "qwe", None, None),
         ("quay.io", "{}", None, None),
         ("quay.io", "{}", {"auth": "Zm9vOmJhcg=="}, "Zm9vOmJhcg=="),
+        ("quay.io", "{}", {"auth": "Zm9vOmJhcg==", "identitytoken": "abc"}, "abc"),
     ],
 )
 @patch(
     "coregio.registry_api.ContainerRegistry._select_registry_auth_token_from_docker_config"
 )
 def test__get__get_auth_token(
     mock_select_token: MagicMock,
@@ -66,15 +67,15 @@
 @patch("coregio.registry_api.ContainerRegistry._get_auth_token")
 def test__get_session(mock_auth_token: MagicMock) -> None:
     mock_auth_token.return_value = "Zm9vOmJhcg=="
     registry = ContainerRegistry("test-quay.io", "foo")
 
     mock_auth = MagicMock()
 
-    def auth_method(token: Any) -> Any:
+    def auth_method(token: Any, proxy: Any = None) -> Any:
         return mock_auth
 
     session = registry._get_session(auth_method)
 
     assert session.auth == mock_auth
 
 
@@ -91,20 +92,22 @@
     sessions = []
     for code in status_codes:
         expected_response = requests.Response()
         expected_response.status_code = code
 
         session = MagicMock()
         session.get.return_value = expected_response
+        session.auth.auth_header = "Bearer foo"
         sessions.append(session)
     mock_session.side_effect = sessions
 
     registry = ContainerRegistry("test-quay.io", "foo")
     resp = registry._get("foo", {}, {}, True)
     assert resp.status_code == sessions[-1].get.return_value.status_code
+    assert registry.auth_header == "Bearer foo"
 
 
 @patch("coregio.utils.handle_response")
 @patch("coregio.registry_api.ContainerRegistry._get")
 def test_get_request(
     mock_get: MagicMock,
     mock_handle: MagicMock,
@@ -112,30 +115,14 @@
 ) -> None:
     mock_handle.return_value = None
     resp = ContainerRegistry("foo", "bar").get_request("/v1/api")
     assert resp == mock_get.return_value
     mock_get.assert_called_once_with("https://foo/v1/api", params=None, headers=None)
 
 
-@patch("coregio.registry_api.requests.Session.get")
-@patch("coregio.registry_api.ContainerRegistry._get_session")
-def test_get_request_error(
-    mock_session: MagicMock, mock_get: MagicMock, monkeypatch: Any
-) -> None:
-    mock_session.return_value = requests.Session()
-    monkeypatch.setenv("ENVIRONMENT", "unit-tests")
-
-    response = requests.Response()
-    response.status_code = 400
-    mock_get.return_value = response
-
-    with pytest.raises(requests.HTTPError):
-        ContainerRegistry("foo", "bar").get_request("/v1/api")
-
-
 @patch("coregio.registry_api.ContainerRegistry.get_request")
 def test_paginated_response(mock_get: MagicMock) -> None:
     get = MagicMock()
     get.json.return_value = {"foo": ["bar1", "bar2"]}
     get.links = {"next": {"url": "test.url"}}
     mock_get.return_value = get
```

### Comparing `coregio-0.3.0/tests/test_registry_auth.py` & `coregio-0.4.0/tests/test_registry_auth.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,14 +37,23 @@
 
     bearer_auth.token_cache["repo123"] = "bar"
     bearer_auth(response)
     mock__set_header.assert_called_once_with(response, "repo123")
     response.register_hook.assert_called_once()
 
 
+def test_HTTPBearerAuth_auth_token(
+    bearer_auth: registry_auth.HTTPBearerAuth,
+) -> None:
+    response = MagicMock()
+
+    bearer_auth.last_auth_header = "foo"
+    assert bearer_auth.auth_header == "foo"
+
+
 @patch("coregio.registry_auth.extract_cookies_to_jar")
 @patch("coregio.registry_auth.HTTPBearerAuth._get_token")
 def test_HTTPBearerAuth_handle_401(
     mock_get_token: MagicMock,
     mock_extract_cookies_to_jar: MagicMock,
     bearer_auth: registry_auth.HTTPBearerAuth,
 ) -> None:
@@ -85,14 +94,15 @@
     mock_get.return_value = mock_response
     resp = bearer_auth._get_token("foo", "repo")
 
     assert resp == None
 
     mock_response = MagicMock()
     mock_response.json.return_value = {"token": "bar"}
+    mock_response.status_code = 200
     mock_get.return_value = mock_response
     resp = bearer_auth._get_token("foo", "repo")
 
     assert resp == "bar"
 
 
 def test_HTTPBeaderAuth__set_header(bearer_auth: registry_auth.HTTPBearerAuth) -> None:
```

