# Comparing `tmp/ovos-backend-client-0.1.0a2.tar.gz` & `tmp/ovos-backend-client-0.1.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-backend-client-0.1.0a2.tar", last modified: Thu Jun  8 00:08:22 2023, max compression
+gzip compressed data, was "ovos-backend-client-0.1.0a3.tar", last modified: Thu Jun  8 01:43:45 2023, max compression
```

## Comparing `ovos-backend-client-0.1.0a2.tar` & `ovos-backend-client-0.1.0a3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 00:08:22.487462 ovos-backend-client-0.1.0a2/
--rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-06-08 00:08:21.000000 ovos-backend-client-0.1.0a2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-08 00:08:21.000000 ovos-backend-client-0.1.0a2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-08 00:08:22.483462 ovos-backend-client-0.1.0a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-06-08 00:08:21.000000 ovos-backend-client-0.1.0a2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 00:08:22.483462 ovos-backend-client-0.1.0a2/ovos_backend_client/
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-08 00:08:21.000000 ovos-backend-client-0.1.0a2/ovos_backend_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33404 2023-06-08 00:08:21.000000 ovos-backend-client-0.1.0a2/ovos_backend_client/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 00:08:22.483462 ovos-backend-client-0.1.0a2/ovos_backend_client/backends/
--rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-06-08 00:08:21.000000 ovos-backend-client-0.1.0a2/ovos_backend_client/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26658 2023-06-08 00:08:21.000000 ovos-backend-client-0.1.0a2/ovos_backend_client/backends/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    40613 2023-06-08 00:08:21.000000 ovos-backend-client-0.1.0a2/ovos_backend_client/backends/offline.py
--rw-r--r--   0 runner    (1001) docker     (123)    37782 2023-06-08 00:08:21.000000 ovos-backend-client-0.1.0a2/ovos_backend_client/backends/personal.py
--rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-06-08 00:08:21.000000 ovos-backend-client-0.1.0a2/ovos_backend_client/cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-06-08 00:08:21.000000 ovos-backend-client-0.1.0a2/ovos_backend_client/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    15926 2023-06-08 00:08:21.000000 ovos-backend-client-0.1.0a2/ovos_backend_client/database.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-08 00:08:21.000000 ovos-backend-client-0.1.0a2/ovos_backend_client/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4509 2023-06-08 00:08:21.000000 ovos-backend-client-0.1.0a2/ovos_backend_client/identity.py
--rw-r--r--   0 runner    (1001) docker     (123)    11975 2023-06-08 00:08:21.000000 ovos-backend-client-0.1.0a2/ovos_backend_client/pairing.py
--rw-r--r--   0 runner    (1001) docker     (123)    16512 2023-06-08 00:08:21.000000 ovos-backend-client-0.1.0a2/ovos_backend_client/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-08 00:08:21.000000 ovos-backend-client-0.1.0a2/ovos_backend_client/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 00:08:22.483462 ovos-backend-client-0.1.0a2/ovos_backend_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-08 00:08:22.000000 ovos-backend-client-0.1.0a2/ovos_backend_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-06-08 00:08:22.000000 ovos-backend-client-0.1.0a2/ovos_backend_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 00:08:22.000000 ovos-backend-client-0.1.0a2/ovos_backend_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-08 00:08:22.000000 ovos-backend-client-0.1.0a2/ovos_backend_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-08 00:08:22.000000 ovos-backend-client-0.1.0a2/ovos_backend_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 00:08:22.487462 ovos-backend-client-0.1.0a2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-06-08 00:08:21.000000 ovos-backend-client-0.1.0a2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:43:45.335932 ovos-backend-client-0.1.0a3/
+-rw-r--r--   0 runner    (1001) docker     (123)     4362 2023-06-08 01:43:45.000000 ovos-backend-client-0.1.0a3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-08 01:43:45.000000 ovos-backend-client-0.1.0a3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-08 01:43:45.335932 ovos-backend-client-0.1.0a3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-06-08 01:43:45.000000 ovos-backend-client-0.1.0a3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:43:45.335932 ovos-backend-client-0.1.0a3/ovos_backend_client/
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-08 01:43:45.000000 ovos-backend-client-0.1.0a3/ovos_backend_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33404 2023-06-08 01:43:45.000000 ovos-backend-client-0.1.0a3/ovos_backend_client/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:43:45.335932 ovos-backend-client-0.1.0a3/ovos_backend_client/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-06-08 01:43:45.000000 ovos-backend-client-0.1.0a3/ovos_backend_client/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26658 2023-06-08 01:43:45.000000 ovos-backend-client-0.1.0a3/ovos_backend_client/backends/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40613 2023-06-08 01:43:45.000000 ovos-backend-client-0.1.0a3/ovos_backend_client/backends/offline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38176 2023-06-08 01:43:45.000000 ovos-backend-client-0.1.0a3/ovos_backend_client/backends/personal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-06-08 01:43:45.000000 ovos-backend-client-0.1.0a3/ovos_backend_client/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-06-08 01:43:45.000000 ovos-backend-client-0.1.0a3/ovos_backend_client/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15926 2023-06-08 01:43:45.000000 ovos-backend-client-0.1.0a3/ovos_backend_client/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-08 01:43:45.000000 ovos-backend-client-0.1.0a3/ovos_backend_client/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4509 2023-06-08 01:43:45.000000 ovos-backend-client-0.1.0a3/ovos_backend_client/identity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11975 2023-06-08 01:43:45.000000 ovos-backend-client-0.1.0a3/ovos_backend_client/pairing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16512 2023-06-08 01:43:45.000000 ovos-backend-client-0.1.0a3/ovos_backend_client/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-08 01:43:45.000000 ovos-backend-client-0.1.0a3/ovos_backend_client/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:43:45.335932 ovos-backend-client-0.1.0a3/ovos_backend_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-08 01:43:45.000000 ovos-backend-client-0.1.0a3/ovos_backend_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-06-08 01:43:45.000000 ovos-backend-client-0.1.0a3/ovos_backend_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 01:43:45.000000 ovos-backend-client-0.1.0a3/ovos_backend_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-08 01:43:45.000000 ovos-backend-client-0.1.0a3/ovos_backend_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-08 01:43:45.000000 ovos-backend-client-0.1.0a3/ovos_backend_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 01:43:45.335932 ovos-backend-client-0.1.0a3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-06-08 01:43:45.000000 ovos-backend-client-0.1.0a3/setup.py
```

### Comparing `ovos-backend-client-0.1.0a2/CHANGELOG.md` & `ovos-backend-client-0.1.0a3/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,20 @@
 # Changelog
 
-## [0.1.0a2](https://github.com/OpenVoiceOS/ovos-backend-client/tree/0.1.0a2) (2023-06-08)
+## [0.1.0a3](https://github.com/OpenVoiceOS/ovos-backend-client/tree/0.1.0a3) (2023-06-08)
 
-[Full Changelog](https://github.com/OpenVoiceOS/ovos-backend-client/compare/V0.0.7a9...0.1.0a2)
+[Full Changelog](https://github.com/OpenVoiceOS/ovos-backend-client/compare/V0.1.0a2...0.1.0a3)
+
+**Fixed bugs:**
+
+- hotfix/rebase mess up in \#30 [\#41](https://github.com/OpenVoiceOS/ovos-backend-client/pull/41) ([JarbasAl](https://github.com/JarbasAl))
+
+## [V0.1.0a2](https://github.com/OpenVoiceOS/ovos-backend-client/tree/V0.1.0a2) (2023-06-08)
+
+[Full Changelog](https://github.com/OpenVoiceOS/ovos-backend-client/compare/V0.0.7a9...V0.1.0a2)
 
 **Implemented enhancements:**
 
 - feat/DatabaseApi [\#30](https://github.com/OpenVoiceOS/ovos-backend-client/pull/30) ([JarbasAl](https://github.com/JarbasAl))
 
 ## [V0.0.7a9](https://github.com/OpenVoiceOS/ovos-backend-client/tree/V0.0.7a9) (2023-06-07)
```

### Comparing `ovos-backend-client-0.1.0a2/README.md` & `ovos-backend-client-0.1.0a3/README.md`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.1.0a2/ovos_backend_client/api.py` & `ovos-backend-client-0.1.0a3/ovos_backend_client/api.py`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.1.0a2/ovos_backend_client/backends/__init__.py` & `ovos-backend-client-0.1.0a3/ovos_backend_client/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.1.0a2/ovos_backend_client/backends/base.py` & `ovos-backend-client-0.1.0a3/ovos_backend_client/backends/base.py`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.1.0a2/ovos_backend_client/backends/offline.py` & `ovos-backend-client-0.1.0a3/ovos_backend_client/backends/offline.py`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.1.0a2/ovos_backend_client/backends/personal.py` & `ovos-backend-client-0.1.0a3/ovos_backend_client/backends/personal.py`

 * *Files 6% similar despite different names*

```diff
@@ -380,17 +380,17 @@
     # Email API
     def email_send(self, title, body, sender):
         return self.device_send_email(title, body, sender)
 
     # Admin API
     def admin_pair(self, uuid=None):
         identity = self.get(f"{self.backend_url}/{self.backend_version}/admin/{uuid}/pair",
-                            headers={"Authorization": f"Bearer {self.credentials['admin']}"})
+                            headers={"Authorization": f"Bearer {self.credentials['admin']}"}).json()
         # save identity file
-        self.identity.save(identity)
+        IdentityManager.save(identity)
         return identity
 
     def admin_set_device_location(self, uuid, loc):
         """
         loc = {
             "city": {
                 "code": "Lawrence",
@@ -446,19 +446,19 @@
         """
         return self.put(f"{self.backend_url}/{self.backend_version}/admin/{uuid}/device", json=info,
                         headers={"Authorization": f"Bearer {self.credentials['admin']}"})
 
     # Database api
     def db_list_devices(self):
         return self.get(url=f"{self.backend_url}/{self.backend_version}/admin/devices/list",
-                        headers={"Authorization": f"Bearer {self.credentials['admin']}"})
+                        headers={"Authorization": f"Bearer {self.credentials['admin']}"}).json()
 
     def db_get_device(self, uuid):
         return self.get(url=f"{self.backend_url}/{self.backend_version}/admin/devices/{uuid}",
-                        headers={"Authorization": f"Bearer {self.credentials['admin']}"})
+                        headers={"Authorization": f"Bearer {self.credentials['admin']}"}).json()
 
     def db_update_device(self, uuid, name=None,
                          device_location=None, opt_in=False,
                          location=None, lang=None, date_format=None,
                          system_unit=None, time_format=None, email=None,
                          isolated_skills=False, ww_id=None, voice_id=None):
         payload = {"name": name,
@@ -471,19 +471,19 @@
                    "time_format": time_format,
                    "email": email,
                    "isolated_skills": isolated_skills,
                    "ww_id": ww_id,
                    "voice_id": voice_id}
         return self.put(url=f"{self.backend_url}/{self.backend_version}/admin/devices/{uuid}",
                         json={k: v for k, v in payload.items() if v is not None},
-                        headers={"Authorization": f"Bearer {self.credentials['admin']}"})
+                        headers={"Authorization": f"Bearer {self.credentials['admin']}"}).json()
 
     def db_delete_device(self, uuid):
         return self.delete(url=f"{self.backend_url}/{self.backend_version}/admin/devices/{uuid}",
-                           headers={"Authorization": f"Bearer {self.credentials['admin']}"})
+                           headers={"Authorization": f"Bearer {self.credentials['admin']}"}).json()
 
     def db_post_device(self, uuid, token, name=None,
                        device_location="somewhere",
                        opt_in=Configuration().get("opt_in", False),
                        location=Configuration().get("location"),
                        lang=Configuration().get("lang"),
                        date_format=Configuration().get("date_format", "DMY"),
@@ -498,284 +498,285 @@
                    "opt_in": opt_in,
                    "location": location,
                    "lang": lang,
                    "date_format": date_format,
                    "system_unit": system_unit,
                    "time_format": time_format,
                    "email": email,
+                   "token": token,
                    "isolated_skills": isolated_skills,
                    "ww_id": ww_id,
                    "voice_id": voice_id,
                    "uuid": uuid}
         return self.post(url=f"{self.backend_url}/{self.backend_version}/admin/devices",
                          json=payload,
-                         headers={"Authorization": f"Bearer {self.credentials['admin']}"})
+                         headers={"Authorization": f"Bearer {self.credentials['admin']}"}).json()
 
     def db_list_shared_skill_settings(self):
         return self.get(url=f"{self.backend_url}/{self.backend_version}/admin/skill_settings/list",
-                        headers={"Authorization": f"Bearer {self.credentials['admin']}"})
+                        headers={"Authorization": f"Bearer {self.credentials['admin']}"}).json()
 
     def db_get_shared_skill_settings(self, skill_id):
 
         return self.get(url=f"{self.backend_url}/{self.backend_version}/admin/skill_settings/{skill_id}",
-                        headers={"Authorization": f"Bearer {self.credentials['admin']}"})
+                        headers={"Authorization": f"Bearer {self.credentials['admin']}"}).json()
 
     def db_update_shared_skill_settings(self, skill_id,
                                         display_name=None,
                                         settings_json=None,
                                         metadata_json=None):
         payload = {"display_name": display_name,
                    "settings_json": settings_json,
                    "metadata_json": metadata_json}
         return self.put(url=f"{self.backend_url}/{self.backend_version}/admin/skill_settings/{skill_id}",
                         json=payload,
-                        headers={"Authorization": f"Bearer {self.credentials['admin']}"})
+                        headers={"Authorization": f"Bearer {self.credentials['admin']}"}).json()
 
     def db_delete_shared_skill_settings(self, skill_id):
         return self.delete(url=f"{self.backend_url}/{self.backend_version}/admin/skill_settings/{skill_id}",
-                           headers={"Authorization": f"Bearer {self.credentials['admin']}"})
+                           headers={"Authorization": f"Bearer {self.credentials['admin']}"}).json()
 
     def db_post_shared_skill_settings(self, skill_id,
                                       display_name,
                                       settings_json,
                                       metadata_json):
         payload = {"display_name": display_name,
                    "skill_id": skill_id,
                    "settings_json": settings_json,
                    "metadata_json": metadata_json}
         return self.post(url=f"{self.backend_url}/{self.backend_version}/admin/skill_settings",
                          json=payload,
-                         headers={"Authorization": f"Bearer {self.credentials['admin']}"})
+                         headers={"Authorization": f"Bearer {self.credentials['admin']}"}).json()
 
     def db_list_skill_settings(self, uuid):
         return self.get(url=f"{self.backend_url}/{self.backend_version}/admin/{uuid}/skill_settings/list",
-                        headers={"Authorization": f"Bearer {self.credentials['admin']}"})
+                        headers={"Authorization": f"Bearer {self.credentials['admin']}"}).json()
 
     def db_get_skill_settings(self, uuid, skill_id):
         return self.get(url=f"{self.backend_url}/{self.backend_version}/admin/{uuid}/skill_settings/{skill_id}",
-                        headers={"Authorization": f"Bearer {self.credentials['admin']}"})
+                        headers={"Authorization": f"Bearer {self.credentials['admin']}"}).json()
 
     def db_update_skill_settings(self, uuid, skill_id,
                                  display_name=None,
                                  settings_json=None,
                                  metadata_json=None):
         payload = {"display_name": display_name,
                    "settings_json": settings_json,
                    "metadata_json": metadata_json}
         return self.put(url=f"{self.backend_url}/{self.backend_version}/admin/{uuid}/skill_settings/{skill_id}",
                         json=payload,
-                        headers={"Authorization": f"Bearer {self.credentials['admin']}"})
+                        headers={"Authorization": f"Bearer {self.credentials['admin']}"}).json()
 
     def db_delete_skill_settings(self, uuid, skill_id):
         return self.delete(url=f"{self.backend_url}/{self.backend_version}/admin/{uuid}/skill_settings/{skill_id}",
-                           headers={"Authorization": f"Bearer {self.credentials['admin']}"})
+                           headers={"Authorization": f"Bearer {self.credentials['admin']}"}).json()
 
     def db_post_skill_settings(self, uuid, skill_id,
                                display_name,
                                settings_json,
                                metadata_json):
         payload = {"display_name": display_name,
                    "skill_id": skill_id,
                    "settings_json": settings_json,
                    "metadata_json": metadata_json}
         return self.post(url=f"{self.backend_url}/{self.backend_version}/admin/{uuid}/skill_settings",
                          json=payload,
-                         headers={"Authorization": f"Bearer {self.credentials['admin']}"})
+                         headers={"Authorization": f"Bearer {self.credentials['admin']}"}).json()
 
     def db_list_oauth_apps(self):
         return self.get(url=f"{self.backend_url}/{self.backend_version}/admin/oauth_apps/list",
-                        headers={"Authorization": f"Bearer {self.credentials['admin']}"})
+                        headers={"Authorization": f"Bearer {self.credentials['admin']}"}).json()
 
     def db_get_oauth_app(self, token_id):
         return self.get(url=f"{self.backend_url}/{self.backend_version}/admin/oauth_apps/{token_id}",
-                        headers={"Authorization": f"Bearer {self.credentials['admin']}"})
+                        headers={"Authorization": f"Bearer {self.credentials['admin']}"}).json()
 
     def db_update_oauth_app(self, token_id, client_id=None, client_secret=None,
                             auth_endpoint=None, token_endpoint=None, refresh_endpoint=None,
                             callback_endpoint=None, scope=None, shell_integration=None):
         payload = {"client_id": client_id, "client_secret": client_secret,
                    "auth_endpoint": auth_endpoint,
                    "token_endpoint": token_endpoint,
                    "refresh_endpoint": refresh_endpoint,
                    "callback_endpoint": callback_endpoint,
                    "scope": scope, "shell_integration": True}
         return self.put(url=f"{self.backend_url}/{self.backend_version}/admin/oauth_apps/{token_id}",
                         json=payload,
-                        headers={"Authorization": f"Bearer {self.credentials['admin']}"})
+                        headers={"Authorization": f"Bearer {self.credentials['admin']}"}).json()
 
     def db_delete_oauth_app(self, token_id):
         return self.delete(url=f"{self.backend_url}/{self.backend_version}/admin/oauth_apps/{token_id}",
-                           headers={"Authorization": f"Bearer {self.credentials['admin']}"})
+                           headers={"Authorization": f"Bearer {self.credentials['admin']}"}).json()
 
     def db_post_oauth_app(self, token_id, client_id, client_secret,
                           auth_endpoint, token_endpoint, refresh_endpoint,
                           callback_endpoint, scope, shell_integration=True):
         payload = {"token_id": token_id,
                    "client_id": client_id,
                    "client_secret": client_secret,
                    "auth_endpoint": auth_endpoint,
                    "token_endpoint": token_endpoint,
                    "refresh_endpoint": refresh_endpoint,
                    "callback_endpoint": callback_endpoint,
                    "scope": scope, "shell_integration": True}
         return self.post(url=f"{self.backend_url}/{self.backend_version}/admin/oauth_apps",
                          json=payload,
-                         headers={"Authorization": f"Bearer {self.credentials['admin']}"})
+                         headers={"Authorization": f"Bearer {self.credentials['admin']}"}).json()
 
     def db_list_oauth_tokens(self):
         return self.get(url=f"{self.backend_url}/{self.backend_version}/admin/oauth_toks/list",
-                        headers={"Authorization": f"Bearer {self.credentials['admin']}"})
+                        headers={"Authorization": f"Bearer {self.credentials['admin']}"}).json()
 
     def db_get_oauth_token(self, token_id):
         return self.get(url=f"{self.backend_url}/{self.backend_version}/admin/oauth_toks/{token_id}",
-                        headers={"Authorization": f"Bearer {self.credentials['admin']}"})
+                        headers={"Authorization": f"Bearer {self.credentials['admin']}"}).json()
 
     def db_update_oauth_token(self, token_id, token_data):
         payload = {"token_data": token_data}
         return self.put(url=f"{self.backend_url}/{self.backend_version}/admin/oauth_toks/{token_id}",
                         headers={"Authorization": f"Bearer {self.credentials['admin']}"},
-                        json=payload)
+                        json=payload).json()
 
     def db_delete_oauth_token(self, token_id):
         return self.delete(url=f"{self.backend_url}/{self.backend_version}/admin/oauth_toks/{token_id}",
-                           headers={"Authorization": f"Bearer {self.credentials['admin']}"})
+                           headers={"Authorization": f"Bearer {self.credentials['admin']}"}).json()
 
     def db_post_oauth_token(self, token_id, token_data):
         payload = {"token_data": token_data, "token_id": token_id}
         return self.put(url=f"{self.backend_url}/{self.backend_version}/admin/oauth_toks",
                         json=payload,
-                        headers={"Authorization": f"Bearer {self.credentials['admin']}"})
+                        headers={"Authorization": f"Bearer {self.credentials['admin']}"}).json()
 
     def db_list_stt_recordings(self):
         return self.get(url=f"{self.backend_url}/{self.backend_version}/admin/voice_recs/list",
-                        headers={"Authorization": f"Bearer {self.credentials['admin']}"})
+                        headers={"Authorization": f"Bearer {self.credentials['admin']}"}).json()
 
     def db_get_stt_recording(self, rec_id):
         return self.get(url=f"{self.backend_url}/{self.backend_version}/admin/voice_recs/{rec_id}",
-                        headers={"Authorization": f"Bearer {self.credentials['admin']}"})
+                        headers={"Authorization": f"Bearer {self.credentials['admin']}"}).json()
 
     def db_update_stt_recording(self, rec_id, transcription=None, metadata=None):
         payload = {"transcription": transcription,
                    "metadata": metadata}
         return self.put(url=f"{self.backend_url}/{self.backend_version}/admin/voice_recs/{rec_id}",
                         json=payload,
-                        headers={"Authorization": f"Bearer {self.credentials['admin']}"})
+                        headers={"Authorization": f"Bearer {self.credentials['admin']}"}).json()
 
     def db_delete_stt_recording(self, rec_id):
         return self.delete(url=f"{self.backend_url}/{self.backend_version}/admin/voice_recs/{rec_id}",
-                           headers={"Authorization": f"Bearer {self.credentials['admin']}"})
+                           headers={"Authorization": f"Bearer {self.credentials['admin']}"}).json()
 
     def db_post_stt_recording(self, byte_data, transcription, metadata=None):
         payload = {"transcription": transcription,
                    "metadata": metadata,
                    "audio_b64": base64.encodebytes(byte_data)}
         return self.put(url=f"{self.backend_url}/{self.backend_version}/admin/voice_recs",
                         json=payload,
-                        headers={"Authorization": f"Bearer {self.credentials['admin']}"})
+                        headers={"Authorization": f"Bearer {self.credentials['admin']}"}).json()
 
     def db_list_ww_recordings(self):
         return self.get(url=f"{self.backend_url}/{self.backend_version}/admin/ww_recs/list",
-                        headers={"Authorization": f"Bearer {self.credentials['admin']}"})
+                        headers={"Authorization": f"Bearer {self.credentials['admin']}"}).json()
 
     def db_get_ww_recording(self, rec_id):
         return self.get(url=f"{self.backend_url}/{self.backend_version}/admin/ww_recs/{rec_id}",
-                        headers={"Authorization": f"Bearer {self.credentials['admin']}"})
+                        headers={"Authorization": f"Bearer {self.credentials['admin']}"}).json()
 
     def db_update_ww_recording(self, rec_id, transcription=None, metadata=None):
         payload = {"transcription": transcription,
                    "metadata": metadata}
         return self.put(url=f"{self.backend_url}/{self.backend_version}/admin/ww_recs/{rec_id}",
                         json=payload,
-                        headers={"Authorization": f"Bearer {self.credentials['admin']}"})
+                        headers={"Authorization": f"Bearer {self.credentials['admin']}"}).json()
 
     def db_delete_ww_recording(self, rec_id):
         return self.delete(url=f"{self.backend_url}/{self.backend_version}/admin/ww_recs/{rec_id}",
-                           headers={"Authorization": f"Bearer {self.credentials['admin']}"})
+                           headers={"Authorization": f"Bearer {self.credentials['admin']}"}).json()
 
     def db_post_ww_recording(self, byte_data, transcription, metadata=None):
         payload = {"transcription": transcription,
                    "metadata": metadata,
                    "audio_b64": base64.encodebytes(byte_data)}
         return self.post(url=f"{self.backend_url}/{self.backend_version}/admin/ww_recs",
                          json=payload,
-                         headers={"Authorization": f"Bearer {self.credentials['admin']}"})
+                         headers={"Authorization": f"Bearer {self.credentials['admin']}"}).json()
 
     def db_list_metrics(self):
         return self.get(url=f"{self.backend_url}/{self.backend_version}/admin/metrics/list",
-                        headers={"Authorization": f"Bearer {self.credentials['admin']}"})
+                        headers={"Authorization": f"Bearer {self.credentials['admin']}"}).json()
 
     def db_get_metric(self, metric_id):
         return self.get(url=f"{self.backend_url}/{self.backend_version}/admin/metrics/{metric_id}",
-                        headers={"Authorization": f"Bearer {self.credentials['admin']}"})
+                        headers={"Authorization": f"Bearer {self.credentials['admin']}"}).json()
 
     def db_update_metric(self, metric_id, metadata):
         payload = {"metadata": metadata}
         return self.put(url=f"{self.backend_url}/{self.backend_version}/admin/metrics/{metric_id}",
                         json=payload,
-                        headers={"Authorization": f"Bearer {self.credentials['admin']}"})
+                        headers={"Authorization": f"Bearer {self.credentials['admin']}"}).json()
 
     def db_delete_metric(self, metric_id):
         return self.delete(url=f"{self.backend_url}/{self.backend_version}/admin/metrics/{metric_id}",
-                           headers={"Authorization": f"Bearer {self.credentials['admin']}"})
+                           headers={"Authorization": f"Bearer {self.credentials['admin']}"}).json()
 
     def db_post_metric(self, metric_type, metadata):
         payload = {"metadata": metadata, "metric_type": metric_type}
         return self.put(url=f"{self.backend_url}/{self.backend_version}/admin/metrics",
                         json=payload,
-                        headers={"Authorization": f"Bearer {self.credentials['admin']}"})
+                        headers={"Authorization": f"Bearer {self.credentials['admin']}"}).json()
 
     def db_list_ww_definitions(self):
         return self.get(url=f"{self.backend_url}/{self.backend_version}/admin/ww_defs/list",
-                        headers={"Authorization": f"Bearer {self.credentials['admin']}"})
+                        headers={"Authorization": f"Bearer {self.credentials['admin']}"}).json()
 
     def db_get_ww_definition(self, ww_id):
         return self.get(url=f"{self.backend_url}/{self.backend_version}/admin/ww_defs/{ww_id}",
-                        headers={"Authorization": f"Bearer {self.credentials['admin']}"})
+                        headers={"Authorization": f"Bearer {self.credentials['admin']}"}).json()
 
     def db_update_ww_definition(self, ww_id, name=None, lang=None, ww_config=None, plugin=None):
         payload = {"name": name, "lang": lang,
                    "plugin": plugin, "ww_config": ww_config}
         return self.put(url=f"{self.backend_url}/{self.backend_version}/admin/ww_defs/{ww_id}",
                         json=payload,
-                        headers={"Authorization": f"Bearer {self.credentials['admin']}"})
+                        headers={"Authorization": f"Bearer {self.credentials['admin']}"}).json()
 
     def db_delete_ww_definition(self, ww_id):
         return self.delete(url=f"{self.backend_url}/{self.backend_version}/admin/ww_defs/{ww_id}",
-                           headers={"Authorization": f"Bearer {self.credentials['admin']}"})
+                           headers={"Authorization": f"Bearer {self.credentials['admin']}"}).json()
 
     def db_post_ww_definition(self, name, lang, ww_config, plugin):
         payload = {"name": name, "lang": lang,
                    "plugin": plugin, "ww_config": ww_config}
         return self.post(url=f"{self.backend_url}/{self.backend_version}/admin/ww_defs",
                          json=payload,
-                         headers={"Authorization": f"Bearer {self.credentials['admin']}"})
+                         headers={"Authorization": f"Bearer {self.credentials['admin']}"}).json()
 
     def db_list_voice_definitions(self):
 
         return self.get(url=f"{self.backend_url}/{self.backend_version}/admin/voice_defs/list",
-                        headers={"Authorization": f"Bearer {self.credentials['admin']}"})
+                        headers={"Authorization": f"Bearer {self.credentials['admin']}"}).json()
 
     def db_get_voice_definition(self, voice_id):
         return self.get(url=f"{self.backend_url}/{self.backend_version}/admin/voice_defs/{voice_id}",
-                        headers={"Authorization": f"Bearer {self.credentials['admin']}"})
+                        headers={"Authorization": f"Bearer {self.credentials['admin']}"}).json()
 
     def db_update_voice_definition(self, voice_id, name=None, lang=None, plugin=None,
                                    tts_config=None, offline=None, gender=None):
         payload = {"name": name, "lang": lang,
                    "plugin": plugin, "tts_config": tts_config,
                    "offline": offline, "gender": gender}
         return self.put(url=f"{self.backend_url}/{self.backend_version}/admin/voice_defs/{voice_id}",
                         json=payload,
-                        headers={"Authorization": f"Bearer {self.credentials['admin']}"})
+                        headers={"Authorization": f"Bearer {self.credentials['admin']}"}).json()
 
     def db_delete_voice_definition(self, voice_id):
         return self.delete(url=f"{self.backend_url}/{self.backend_version}/admin/voice_defs/{voice_id}",
-                           headers={"Authorization": f"Bearer {self.credentials['admin']}"})
+                           headers={"Authorization": f"Bearer {self.credentials['admin']}"}).json()
 
     def db_post_voice_definition(self, name, lang, plugin,
                                  tts_config, offline, gender=None):
         payload = {"name": name, "lang": lang,
                    "plugin": plugin, "tts_config": tts_config,
                    "offline": offline, "gender": gender}
         return self.post(url=f"{self.backend_url}/{self.backend_version}/admin/voice_defs",
                          json=payload,
-                         headers={"Authorization": f"Bearer {self.credentials['admin']}"})
+                         headers={"Authorization": f"Bearer {self.credentials['admin']}"}).json()
```

### Comparing `ovos-backend-client-0.1.0a2/ovos_backend_client/cloud.py` & `ovos-backend-client-0.1.0a3/ovos_backend_client/cloud.py`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.1.0a2/ovos_backend_client/config.py` & `ovos-backend-client-0.1.0a3/ovos_backend_client/config.py`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.1.0a2/ovos_backend_client/database.py` & `ovos-backend-client-0.1.0a3/ovos_backend_client/database.py`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.1.0a2/ovos_backend_client/identity.py` & `ovos-backend-client-0.1.0a3/ovos_backend_client/identity.py`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.1.0a2/ovos_backend_client/pairing.py` & `ovos-backend-client-0.1.0a3/ovos_backend_client/pairing.py`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.1.0a2/ovos_backend_client/settings.py` & `ovos-backend-client-0.1.0a3/ovos_backend_client/settings.py`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.1.0a2/ovos_backend_client.egg-info/SOURCES.txt` & `ovos-backend-client-0.1.0a3/ovos_backend_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.1.0a2/setup.py` & `ovos-backend-client-0.1.0a3/setup.py`

 * *Files identical despite different names*

