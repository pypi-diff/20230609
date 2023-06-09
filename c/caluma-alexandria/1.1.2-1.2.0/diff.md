# Comparing `tmp/caluma_alexandria-1.1.2.tar.gz` & `tmp/caluma_alexandria-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caluma_alexandria-1.1.2.tar", max compression
+gzip compressed data, was "caluma_alexandria-1.2.0.tar", max compression
```

## Comparing `caluma_alexandria-1.1.2.tar` & `caluma_alexandria-1.2.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     8853 2023-05-17 12:40:56.749558 caluma_alexandria-1.1.2/CHANGELOG.md
--rw-r--r--   0        0        0    35148 2022-12-16 12:36:48.076001 caluma_alexandria-1.1.2/LICENSE
--rw-r--r--   0        0        0     4279 2023-03-31 07:21:28.078793 caluma_alexandria-1.1.2/README.md
--rw-r--r--   0        0        0        0 2022-12-16 12:36:48.076001 caluma_alexandria-1.1.2/alexandria/__init__.py
--rw-r--r--   0        0        0        0 2022-12-16 12:36:48.076001 caluma_alexandria-1.1.2/alexandria/core/__init__.py
--rw-r--r--   0        0        0      863 2023-05-04 13:55:17.660574 caluma_alexandria-1.1.2/alexandria/core/apps.py
--rw-r--r--   0        0        0      195 2022-12-16 12:36:48.076001 caluma_alexandria-1.1.2/alexandria/core/collections.py
--rw-r--r--   0        0        0     1922 2023-04-27 09:52:20.806733 caluma_alexandria-1.1.2/alexandria/core/factories.py
--rw-r--r--   0        0        0     5022 2023-04-27 09:52:20.806733 caluma_alexandria-1.1.2/alexandria/core/filters.py
--rw-r--r--   0        0        0    13121 2023-05-04 12:51:21.034379 caluma_alexandria-1.1.2/alexandria/core/migrations/0001_initial.py
--rw-r--r--   0        0        0      490 2023-04-27 09:52:20.806733 caluma_alexandria-1.1.2/alexandria/core/migrations/0002_tags_monolingual.py
--rw-r--r--   0        0        0      644 2023-04-27 09:52:20.806733 caluma_alexandria-1.1.2/alexandria/core/migrations/0003_file_upload_status.py
--rw-r--r--   0        0        0     2982 2023-05-04 12:51:21.034379 caluma_alexandria-1.1.2/alexandria/core/migrations/0004_tag_synonym_group.py
--rw-r--r--   0        0        0     1065 2023-04-27 09:52:20.806733 caluma_alexandria-1.1.2/alexandria/core/migrations/0005_rename_type_and_meta.py
--rw-r--r--   0        0        0     1146 2023-05-11 11:29:27.228878 caluma_alexandria-1.1.2/alexandria/core/migrations/0006_rename_metainfo_jsonfield_verbose_name.py
--rw-r--r--   0        0        0        0 2022-12-16 12:36:48.076001 caluma_alexandria-1.1.2/alexandria/core/migrations/__init__.py
--rw-r--r--   0        0        0     6353 2023-05-11 09:24:07.841154 caluma_alexandria-1.1.2/alexandria/core/models.py
--rw-r--r--   0        0        0     4320 2023-05-04 12:51:21.034379 caluma_alexandria-1.1.2/alexandria/core/permissions.py
--rw-r--r--   0        0        0     7408 2023-05-04 12:51:21.034379 caluma_alexandria-1.1.2/alexandria/core/serializers.py
--rw-r--r--   0        0        0     2462 2023-05-31 13:03:28.282707 caluma_alexandria-1.1.2/alexandria/core/storage_clients.py
--rw-r--r--   0        0        0     1544 2023-04-27 09:52:20.810733 caluma_alexandria-1.1.2/alexandria/core/thumbs.py
--rw-r--r--   0        0        0      462 2022-12-16 12:36:48.076001 caluma_alexandria-1.1.2/alexandria/core/urls.py
--rw-r--r--   0        0        0     1754 2022-12-16 12:36:48.076001 caluma_alexandria-1.1.2/alexandria/core/validation.py
--rw-r--r--   0        0        0     6025 2023-05-04 12:51:21.034379 caluma_alexandria-1.1.2/alexandria/core/views.py
--rw-r--r--   0        0        0     5021 2023-05-04 12:51:21.034379 caluma_alexandria-1.1.2/alexandria/core/visibilities.py
--rw-r--r--   0        0        0        0 2022-12-16 12:36:48.076001 caluma_alexandria-1.1.2/alexandria/oidc_auth/__init__.py
--rw-r--r--   0        0        0     4031 2022-12-23 08:19:28.540306 caluma_alexandria-1.1.2/alexandria/oidc_auth/authentication.py
--rw-r--r--   0        0        0     1021 2022-12-16 12:36:48.080001 caluma_alexandria-1.1.2/alexandria/oidc_auth/models.py
--rw-r--r--   0        0        0       30 2023-04-19 12:35:40.637143 caluma_alexandria-1.1.2/alexandria/settings/__init__.py
--rw-r--r--   0        0        0     4662 2023-05-17 12:40:56.749558 caluma_alexandria-1.1.2/alexandria/settings/alexandria.py
--rw-r--r--   0        0        0     4778 2023-05-04 12:51:21.034379 caluma_alexandria-1.1.2/alexandria/settings/django.py
--rw-r--r--   0        0        0      162 2023-04-27 09:52:20.810733 caluma_alexandria-1.1.2/alexandria/urls.py
--rw-r--r--   0        0        0      407 2023-04-19 08:37:34.482085 caluma_alexandria-1.1.2/alexandria/wsgi.py
--rw-r--r--   0        0        0     3021 2023-05-17 12:40:56.753558 caluma_alexandria-1.1.2/pyproject.toml
--rw-r--r--   0        0        0     5509 1970-01-01 00:00:00.000000 caluma_alexandria-1.1.2/setup.py
--rw-r--r--   0        0        0     5663 1970-01-01 00:00:00.000000 caluma_alexandria-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0     9458 2023-06-09 09:29:53.238949 caluma_alexandria-1.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0    35148 2022-12-16 12:36:48.076001 caluma_alexandria-1.2.0/LICENSE
+-rw-r--r--   0        0        0     4650 2023-06-09 09:10:05.343196 caluma_alexandria-1.2.0/README.md
+-rw-r--r--   0        0        0        0 2022-12-16 12:36:48.076001 caluma_alexandria-1.2.0/alexandria/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-16 12:36:48.076001 caluma_alexandria-1.2.0/alexandria/core/__init__.py
+-rw-r--r--   0        0        0      863 2023-05-04 13:55:17.660574 caluma_alexandria-1.2.0/alexandria/core/apps.py
+-rw-r--r--   0        0        0      195 2022-12-16 12:36:48.076001 caluma_alexandria-1.2.0/alexandria/core/collections.py
+-rw-r--r--   0        0        0     1922 2023-04-27 09:52:20.806733 caluma_alexandria-1.2.0/alexandria/core/factories.py
+-rw-r--r--   0        0        0     5022 2023-04-27 09:52:20.806733 caluma_alexandria-1.2.0/alexandria/core/filters.py
+-rw-r--r--   0        0        0    13121 2023-05-04 12:51:21.034379 caluma_alexandria-1.2.0/alexandria/core/migrations/0001_initial.py
+-rw-r--r--   0        0        0      490 2023-04-27 09:52:20.806733 caluma_alexandria-1.2.0/alexandria/core/migrations/0002_tags_monolingual.py
+-rw-r--r--   0        0        0      644 2023-04-27 09:52:20.806733 caluma_alexandria-1.2.0/alexandria/core/migrations/0003_file_upload_status.py
+-rw-r--r--   0        0        0     2982 2023-05-04 12:51:21.034379 caluma_alexandria-1.2.0/alexandria/core/migrations/0004_tag_synonym_group.py
+-rw-r--r--   0        0        0     1065 2023-04-27 09:52:20.806733 caluma_alexandria-1.2.0/alexandria/core/migrations/0005_rename_type_and_meta.py
+-rw-r--r--   0        0        0     1146 2023-05-11 11:29:27.228878 caluma_alexandria-1.2.0/alexandria/core/migrations/0006_rename_metainfo_jsonfield_verbose_name.py
+-rw-r--r--   0        0        0        0 2022-12-16 12:36:48.076001 caluma_alexandria-1.2.0/alexandria/core/migrations/__init__.py
+-rw-r--r--   0        0        0     6353 2023-05-11 09:24:07.841154 caluma_alexandria-1.2.0/alexandria/core/models.py
+-rw-r--r--   0        0        0     4623 2023-06-09 09:10:05.343196 caluma_alexandria-1.2.0/alexandria/core/permissions.py
+-rw-r--r--   0        0        0     6967 2023-06-09 09:10:05.343196 caluma_alexandria-1.2.0/alexandria/core/serializers.py
+-rw-r--r--   0        0        0     2770 2023-06-01 09:09:52.734835 caluma_alexandria-1.2.0/alexandria/core/storage_clients.py
+-rw-r--r--   0        0        0     1544 2023-04-27 09:52:20.810733 caluma_alexandria-1.2.0/alexandria/core/thumbs.py
+-rw-r--r--   0        0        0      462 2022-12-16 12:36:48.076001 caluma_alexandria-1.2.0/alexandria/core/urls.py
+-rw-r--r--   0        0        0     1754 2022-12-16 12:36:48.076001 caluma_alexandria-1.2.0/alexandria/core/validation.py
+-rw-r--r--   0        0        0     6025 2023-05-04 12:51:21.034379 caluma_alexandria-1.2.0/alexandria/core/views.py
+-rw-r--r--   0        0        0     5021 2023-05-04 12:51:21.034379 caluma_alexandria-1.2.0/alexandria/core/visibilities.py
+-rw-r--r--   0        0        0        0 2022-12-16 12:36:48.076001 caluma_alexandria-1.2.0/alexandria/oidc_auth/__init__.py
+-rw-r--r--   0        0        0     4224 2023-06-09 09:10:05.343196 caluma_alexandria-1.2.0/alexandria/oidc_auth/authentication.py
+-rw-r--r--   0        0        0     1021 2022-12-16 12:36:48.080001 caluma_alexandria-1.2.0/alexandria/oidc_auth/models.py
+-rw-r--r--   0        0        0       30 2023-04-19 12:35:40.637143 caluma_alexandria-1.2.0/alexandria/settings/__init__.py
+-rw-r--r--   0        0        0     5008 2023-06-09 09:10:05.343196 caluma_alexandria-1.2.0/alexandria/settings/alexandria.py
+-rw-r--r--   0        0        0     4778 2023-05-04 12:51:21.034379 caluma_alexandria-1.2.0/alexandria/settings/django.py
+-rw-r--r--   0        0        0      162 2023-04-27 09:52:20.810733 caluma_alexandria-1.2.0/alexandria/urls.py
+-rw-r--r--   0        0        0      407 2023-04-19 08:37:34.482085 caluma_alexandria-1.2.0/alexandria/wsgi.py
+-rw-r--r--   0        0        0     3021 2023-06-09 09:29:26.542772 caluma_alexandria-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5883 1970-01-01 00:00:00.000000 caluma_alexandria-1.2.0/setup.py
+-rw-r--r--   0        0        0     6034 1970-01-01 00:00:00.000000 caluma_alexandria-1.2.0/PKG-INFO
```

### Comparing `caluma_alexandria-1.1.2/CHANGELOG.md` & `caluma_alexandria-1.2.0/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+# v1.2.0
+### Feature
+* Make properties for created_by configurable ([`c18dc06`](https://github.com/projectcaluma/alexandria/commit/c18dc06224fd8bf25090fc64906ac058aac8024f))
+* Let the oidc user model be configurable ([`74c673a`](https://github.com/projectcaluma/alexandria/commit/74c673aff740b2c495f36ed4ca67468f8fd140e3))
+
+### Fix
+* Extract serializer permissions ([`775f2b7`](https://github.com/projectcaluma/alexandria/commit/775f2b7f56fd822e644fea04bf96a6857e8c9609))
+* Use correct minio error ([`86ef544`](https://github.com/projectcaluma/alexandria/commit/86ef5442f2cfb3d9a094a26f071a38e258ff6a4e))
 # v1.1.2
 ### Fix
 * Visibility config default ([`1275d26`](https://github.com/projectcaluma/alexandria/commit/1275d26b192818d5603bd43a91207943f4dad377))
 
 # v1.1.1 (broken, don't use!)
 ### Fix
 * Make deprecated VISIBILITY_CLASSES env var optional ([`20f4553`](https://github.com/projectcaluma/alexandria/commit/20f45538e4bc4ce789fa65b522cfdd45f2a587c3))
```

### Comparing `caluma_alexandria-1.1.2/LICENSE` & `caluma_alexandria-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-1.1.2/README.md` & `caluma_alexandria-1.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -57,20 +57,23 @@
   * `DATABASE_PORT`: Port to use when connecting to database (default: 5432)
   * `DATABASE_NAME`: Name of database to use (default: alexandria)
   * `DATABASE_USER`: Username to use when connecting to the database (default: alexandria)
   * `DATABASE_PASSWORD`: Password to use when connecting to database
 * Authentication configuration
   * `OIDC_OP_USER_ENDPOINT`: Userinfo endpoint for OIDC
   * `OIDC_VERIFY_SSL`: Set to `false` if you want to disable verifying SSL certs. Useful for development
-  * `OIDC_DRF_AUTH_BACKEND`: Overwrite the default authentication backend with your own.
+  * `OIDC_DRF_AUTH_BACKEND`: Overwrite the default authentication backend with your own
+  * `ALEXANDRIA_OIDC_USER_FACTORY`: Overwrite the default user with your own
+  * `ALEXANDRIA_CREATED_BY_USER_PROPERTY`: Overwrite the default user property which is used for `..._by_user` (default: username)
+  * `ALEXANDRIA_CREATED_BY_GROUP_PROPERTY`: Overwrite the default group property which is used for `..._by_group` (default: group)
 * Authorization configurations
-  * `VISIBILITY_CLASSES`: Comma-separated list of classes that define visibility for all models
-  * `PERMISSION_CLASSES`: Comma-separated list of classes that define permissions for all models
+  * `ALEXANDRIA_VISIBILITY_CLASSES`: Comma-separated list of classes that define visibility for all models
+  * `ALEXANDRIA_PERMISSION_CLASSES`: Comma-separated list of classes that define permissions for all models
 * Data validation configuration
-  * `VALIDATION_CLASSES`: Comma-separated list of classes that define [custom validations](docs/validation.md)
+  * `ALEXANDRIA_VALIDATION_CLASSES`: Comma-separated list of classes that define [custom validations](docs/validation.md)
 
 For development, you can also set the following environemnt variables to help
 you:
 
   * `DEV_AUTH_BACKEND`: Set this to "true" to enable a fake auth backend that simulates an authenticated user. Requires `DEBUG` to be set to `True` as well.
   * `DEBUG`: Set this to true for debugging during development. Never enable this in production, as it **will** leak information to the public if you do.
```

### Comparing `caluma_alexandria-1.1.2/alexandria/core/apps.py` & `caluma_alexandria-1.2.0/alexandria/core/apps.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-1.1.2/alexandria/core/factories.py` & `caluma_alexandria-1.2.0/alexandria/core/factories.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-1.1.2/alexandria/core/filters.py` & `caluma_alexandria-1.2.0/alexandria/core/filters.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-1.1.2/alexandria/core/migrations/0001_initial.py` & `caluma_alexandria-1.2.0/alexandria/core/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-1.1.2/alexandria/core/migrations/0003_file_upload_status.py` & `caluma_alexandria-1.2.0/alexandria/core/migrations/0003_file_upload_status.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-1.1.2/alexandria/core/migrations/0004_tag_synonym_group.py` & `caluma_alexandria-1.2.0/alexandria/core/migrations/0004_tag_synonym_group.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-1.1.2/alexandria/core/migrations/0005_rename_type_and_meta.py` & `caluma_alexandria-1.2.0/alexandria/core/migrations/0005_rename_type_and_meta.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-1.1.2/alexandria/core/migrations/0006_rename_metainfo_jsonfield_verbose_name.py` & `caluma_alexandria-1.2.0/alexandria/core/migrations/0006_rename_metainfo_jsonfield_verbose_name.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-1.1.2/alexandria/core/models.py` & `caluma_alexandria-1.2.0/alexandria/core/models.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-1.1.2/alexandria/core/permissions.py` & `caluma_alexandria-1.2.0/alexandria/core/permissions.py`

 * *Files 12% similar despite different names*

```diff
@@ -122,12 +122,21 @@
     You can either use this in combination with your own permission
     classes, or inherit from it if you want *some* models to be accessible
     publicly.
     """
 
     @permission_for(BaseModel)
     def base_permission(self, request):
-        return not isinstance(request.user, AnonymousUser)
+        return not isinstance(request.user, AnonymousUser) and self.validate_group(
+            request.user, request.user.group
+        )
 
     @object_permission_for(BaseModel)
     def base_object_permission(self, request, instance):
-        return self.base_permission(request)
+        return self.base_permission(request) and self.validate_group(
+            request.user, instance.created_by_group
+        )
+
+    def validate_group(self, user, value):
+        if value and value not in user.groups:
+            return False
+        return True
```

### Comparing `caluma_alexandria-1.1.2/alexandria/core/serializers.py` & `caluma_alexandria-1.2.0/alexandria/core/serializers.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from django.conf import settings
 from django.contrib.auth.models import AnonymousUser
 from django.template.defaultfilters import slugify
 from django.utils import translation
 from rest_framework.exceptions import ValidationError
 from rest_framework_json_api import serializers
 
 from . import models
@@ -34,47 +35,38 @@
     def validate(self, *args, **kwargs):
         validated_data = super().validate(*args, **kwargs)
 
         for func in self._custom_validators:
             validated_data = func(validated_data)
 
         user = self.context["request"].user
-        validated_data["created_by_user"] = user.username
-        validated_data["modified_by_user"] = user.username
+        username = getattr(user, settings.ALEXANDRIA_CREATED_BY_USER_PROPERTY)
+        validated_data["created_by_user"] = username
+        validated_data["modified_by_user"] = username
 
         self.Meta.model.check_permissions(self.context["request"])
         if self.instance is not None:
             self.instance.check_object_permissions(self.context["request"])
 
         return validated_data
 
     def validate_created_by_group(self, value):
         # Created by group can be set on creation, then must remain constant
         if self.instance:
             # can't change created_by_group on existing instances
             return self.instance.created_by_group
-        else:
-            return self._validate_group(value, "created_by_group")
-
-    def validate_modified_by_group(self, value):
-        # Modified by group is validated against the user's list of groups,
-        # with a fallback to the default group if no value is given
-        return self._validate_group(value or self._default_group(), "modified_by_group")
-
-    def _validate_group(self, value, field_name):
-        user = self.context["request"].user
-        if value and value not in user.groups:
-            raise ValidationError(
-                f"Given {field_name} '{value}' is not part of user's assigned groups"
-            )
         return value
 
     def _default_group(self):
         user = self.context["request"].user
-        return user.group if not isinstance(user, AnonymousUser) else None
+        return (
+            getattr(user, settings.ALEXANDRIA_CREATED_BY_GROUP_PROPERTY)
+            if not isinstance(user, AnonymousUser)
+            else None
+        )
 
     class Meta:
         fields = (
             "created_at",
             "created_by_user",
             "created_by_group",
             "modified_at",
```

### Comparing `caluma_alexandria-1.1.2/alexandria/core/storage_clients.py` & `caluma_alexandria-1.2.0/alexandria/core/storage_clients.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,62 +1,81 @@
 from datetime import timedelta
+from functools import wraps
+from logging import getLogger
 from pathlib import Path
 
 import minio
 from django.conf import settings
 
+log = getLogger(__name__)
+
+
+def _retry_on_missing_bucket(fn):
+    """Create missing bucket if needed (decorator).
+
+    If enabled in the settings, try to create the bucket if it
+    doesn't exist yet, then retry.
+    """
+
+    @wraps(fn)
+    def wrapper(self, *args, **kwargs):
+        try:
+            return fn(self, *args, **kwargs)
+        except minio.error.S3Error as exc:
+            if (
+                exc.code == "NoSuchBucket"
+                and settings.MINIO_STORAGE_AUTO_CREATE_MEDIA_BUCKET
+            ):
+                log.warning(
+                    f"Minio bucket '{self.bucket}' missing, trying to create it"
+                )
+                self.client.make_bucket(self.bucket)
+                return fn(self, *args, **kwargs)
+            raise
+
+    return wrapper
+
 
 class Minio:
     def __init__(self):
         endpoint = settings.MINIO_STORAGE_ENDPOINT
         access_key = settings.MINIO_STORAGE_ACCESS_KEY
         secret_key = settings.MINIO_STORAGE_SECRET_KEY
         secure = settings.MINIO_STORAGE_USE_HTTPS
         self.client = minio.Minio(
             endpoint, access_key=access_key, secret_key=secret_key, secure=secure
         )
         self.bucket = settings.MINIO_STORAGE_MEDIA_BUCKET_NAME
 
+    @_retry_on_missing_bucket
     def download_url(self, object_name):
-        try:
-            return self.client.presigned_get_object(
-                self.bucket,
-                object_name,
-                timedelta(minutes=settings.MINIO_PRESIGNED_TTL_MINUTES),
-            )
-        except minio.error.S3Error as exc:  # pragma: no cover
-            if (
-                exc.code == "NoSuchBucket"
-                and settings.MINIO_STORAGE_AUTO_CREATE_MEDIA_BUCKET
-            ):
-                self.client.make_bucket(self.bucket)
-                return self.download_url(object_name)
+        return self.client.presigned_get_object(
+            self.bucket,
+            object_name,
+            timedelta(minutes=settings.MINIO_PRESIGNED_TTL_MINUTES),
+        )
 
+    @_retry_on_missing_bucket
     def upload_url(self, object_name):
-        try:
-            return self.client.presigned_put_object(
-                self.bucket,
-                object_name,
-                timedelta(minutes=settings.MINIO_PRESIGNED_TTL_MINUTES),
-            )
-        except minio.error.S3Error as exc:  # pragma: no cover
-            if (
-                exc.code == "NoSuchBucket"
-                and settings.MINIO_STORAGE_AUTO_CREATE_MEDIA_BUCKET
-            ):
-                self.client.make_bucket(self.bucket)
-                return self.upload_url(object_name)
+        return self.client.presigned_put_object(
+            self.bucket,
+            object_name,
+            timedelta(minutes=settings.MINIO_PRESIGNED_TTL_MINUTES),
+        )
 
+    @_retry_on_missing_bucket
     def remove_object(self, object_name):
         self.client.remove_object(self.bucket, object_name)
 
+    @_retry_on_missing_bucket
     def get_object(self, object_name):
         data = self.client.get_object(self.bucket, object_name)
         return data
 
+    @_retry_on_missing_bucket
     def put_object(self, filepath, object_name):
         filepath = Path(filepath)  # make sure we got a Path object
 
         with filepath.open("rb") as file_data:
             file_stat = filepath.stat()
             return self.client.put_object(
                 self.bucket, object_name, file_data, file_stat.st_size
```

### Comparing `caluma_alexandria-1.1.2/alexandria/core/thumbs.py` & `caluma_alexandria-1.2.0/alexandria/core/thumbs.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-1.1.2/alexandria/core/validation.py` & `caluma_alexandria-1.2.0/alexandria/core/validation.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-1.1.2/alexandria/core/views.py` & `caluma_alexandria-1.2.0/alexandria/core/views.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-1.1.2/alexandria/core/visibilities.py` & `caluma_alexandria-1.2.0/alexandria/core/visibilities.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-1.1.2/alexandria/oidc_auth/authentication.py` & `caluma_alexandria-1.2.0/alexandria/oidc_auth/authentication.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,32 +3,35 @@
 import hashlib
 
 import requests
 from django.conf import settings
 from django.core.cache import cache
 from django.core.exceptions import ImproperlyConfigured, SuspiciousOperation
 from django.utils.encoding import force_bytes
+from django.utils.module_loading import import_string
 from mozilla_django_oidc.auth import OIDCAuthenticationBackend
 
-from .models import OIDCUser
-
 
 class AlexandriaAuthenticationBackend(OIDCAuthenticationBackend):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         self.OIDC_USERNAME_CLAIM = self.get_settings("OIDC_USERNAME_CLAIM")
         self.OIDC_OP_INTROSPECT_ENDPOINT = self.get_settings(
             "OIDC_OP_INTROSPECT_ENDPOINT"
         )
         self.OIDC_BEARER_TOKEN_REVALIDATION_TIME = self.get_settings(
             "OIDC_BEARER_TOKEN_REVALIDATION_TIME"
         )
         self.OIDC_VERIFY_SSL = self.get_settings("OIDC_VERIFY_SSL", True)
 
+    def _oidc_user(self, *args, **kwargs):
+        factory = import_string(settings.ALEXANDRIA_OIDC_USER_FACTORY)
+        return factory(*args, **kwargs)
+
     def get_introspection(self, access_token, id_token, payload):
         """Return user details dictionary."""
 
         basic = base64.b64encode(
             f"{self.OIDC_RP_CLIENT_ID}:{self.OIDC_RP_CLIENT_SECRET}".encode("utf-8")
         ).decode()
         headers = {
@@ -65,15 +68,15 @@
 
         return claims
 
     def get_or_create_user(self, access_token, id_token, payload):
         """Verify claims and return user, otherwise raise an Exception."""
 
         claims = self.get_userinfo_or_introspection(access_token)
-        user = OIDCUser(access_token, claims)
+        user = self._oidc_user(access_token, claims)
 
         return user
 
     def cached_request(self, method, token, cache_prefix):
         token_hash = hashlib.sha256(force_bytes(token)).hexdigest()
 
         func = functools.partial(method, token, None, None)
@@ -102,14 +105,14 @@
     def get_userinfo_or_introspection(self, access_token) -> dict:  # pragma: no cover
         return {
             settings.OIDC_USERNAME_CLAIM: "dev",
             settings.OIDC_GROUPS_CLAIM: ["dev-group", "secondary-group"],
         }
 
     def get_or_create_user(self, access_token, id_token, payload):
-        return OIDCUser(
+        return self._oidc_user(
             access_token,
             {
                 settings.OIDC_USERNAME_CLAIM: "dev",
                 settings.OIDC_GROUPS_CLAIM: ["dev-group", "secondary-group"],
             },
         )
```

### Comparing `caluma_alexandria-1.1.2/alexandria/oidc_auth/models.py` & `caluma_alexandria-1.2.0/alexandria/oidc_auth/models.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-1.1.2/alexandria/settings/alexandria.py` & `caluma_alexandria-1.2.0/alexandria/settings/alexandria.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,14 +47,23 @@
     "OIDC_DRF_AUTH_BACKEND",
     default="alexandria.oidc_auth.authentication.AlexandriaAuthenticationBackend",
 )
 if DEV_AUTH_BACKEND:
     OIDC_DRF_AUTH_BACKEND = (
         "alexandria.oidc_auth.authentication.DevelopmentAuthenticationBackend"
     )
+ALEXANDRIA_OIDC_USER_FACTORY = env.str(
+    "ALEXANDRIA_OIDC_USER_FACTORY", default="alexandria.oidc_auth.models.OIDCUser"
+)
+ALEXANDRIA_CREATED_BY_USER_PROPERTY = env.str(
+    "ALEXANDRIA_CREATED_BY_USER_PROPERTY", default="username"
+)
+ALEXANDRIA_CREATED_BY_GROUP_PROPERTY = env.str(
+    "ALEXANDRIA_CREATED_BY_GROUP_PROPERTY", default="group"
+)
 
 
 # Extensions
 ALEXANDRIA_VISIBILITY_CLASSES = env.list(
     "ALEXANDRIA_VISIBILITY_CLASSES",
     default=default(["alexandria.core.visibilities.Any"], []),
 )
```

### Comparing `caluma_alexandria-1.1.2/alexandria/settings/django.py` & `caluma_alexandria-1.2.0/alexandria/settings/django.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-1.1.2/pyproject.toml` & `caluma_alexandria-1.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "caluma-alexandria"
-version = "1.1.2"
+version = "1.2.0"
 description = "Document management service"
 repository = "https://github.com/projectcaluma/alexandria"
 authors = ["Caluma <info@caluma.io>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `caluma_alexandria-1.1.2/setup.py` & `caluma_alexandria-1.2.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,17 +24,17 @@
  'psycopg2-binary>=2.9,<2.10',
  'requests>=2.28.0,<3.0.0',
  'uwsgi>=2.0.20,<3.0.0',
  'vtk>=9.2.6,<10.0.0']
 
 setup_kwargs = {
     'name': 'caluma-alexandria',
-    'version': '1.1.2',
+    'version': '1.2.0',
     'description': 'Document management service',
-    'long_description': '# alexandria\n\n[![Build Status](https://github.com/projectcaluma/emeis/workflows/Tests/badge.svg)](https://github.com/projectcaluma/emeis/actions?query=workflow%3ATests)\n[![Coverage](https://img.shields.io/badge/coverage-100%25-brightgreen.svg)](https://github.com/projectcaluma/emeis/blob/master/setup.cfg#L50)\n[![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/projectcaluma/alexandria)\n[![License: GPL-3.0-or-later](https://img.shields.io/github/license/projectcaluma/emeis)](https://spdx.org/licenses/GPL-3.0-or-later.html)\n\nOur goal is to implement an external document management service to hold and provide uploaded documents.\nDocuments can be uploaded and, depending on user access, managed by internal as well as external users.\n\nThe goal is NOT to re implement a complex [DMS](https://en.wikipedia.org/wiki/Document_management_system) but rather to have a simple and user-friendly way of managing documents with different permissions.\n\nAll User Interface interactions should be as simple as possible and easily understandable.\n\n[Original RFC that led to alexandria](docs/original_alexandria_rfc.md)\n\n## Getting started\n\n### Installation\n\n**Requirements**\n* docker\n* docker-compose\n\nAfter installing and configuring those, download [docker-compose.yml](https://raw.githubusercontent.com/projectcaluma/alexandria/master/docker-compose.yml) and run the following commands:\n\n```bash\n# only needs to be run once\necho UID=$UID > .env\n\ndocker-compose up -d\n```\n\nYou can now access the api at [http://localhost:8000/api/v1/](http://localhost:8000/api/v1/).\n\n### Example data\n\nTo load a set of categories run the following command:\n```bash\nmake load_example_data\n```\n\n### Configuration\n\nDocument Merge Service is a [12factor app](https://12factor.net/) which means that configuration is stored in environment variables.\nDifferent environment variable types are explained at [django-environ](https://github.com/joke2k/django-environ#supported-types).\n\n#### Common\n\nA list of configuration options which you need\n\n* Django configuration\n  * `SECRET_KEY`: A secret key used for cryptography. This needs to be a random string of a certain length. See [more](https://docs.djangoproject.com/en/2.1/ref/settings/#std:setting-SECRET_KEY).\n  * `ALLOWED_HOSTS`: A list of hosts/domains your service will be served from. See [more](https://docs.djangoproject.com/en/2.1/ref/settings/#allowed-hosts).\n  * `DATABASE_ENGINE`: Database backend to use. See [more](https://docs.djangoproject.com/en/2.1/ref/settings/#std:setting-DATABASE-ENGINE). (default: django.db.backends.postgresql)\n  * `DATABASE_HOST`: Host to use when connecting to database (default: localhost)\n  * `DATABASE_PORT`: Port to use when connecting to database (default: 5432)\n  * `DATABASE_NAME`: Name of database to use (default: alexandria)\n  * `DATABASE_USER`: Username to use when connecting to the database (default: alexandria)\n  * `DATABASE_PASSWORD`: Password to use when connecting to database\n* Authentication configuration\n  * `OIDC_OP_USER_ENDPOINT`: Userinfo endpoint for OIDC\n  * `OIDC_VERIFY_SSL`: Set to `false` if you want to disable verifying SSL certs. Useful for development\n  * `OIDC_DRF_AUTH_BACKEND`: Overwrite the default authentication backend with your own.\n* Authorization configurations\n  * `VISIBILITY_CLASSES`: Comma-separated list of classes that define visibility for all models\n  * `PERMISSION_CLASSES`: Comma-separated list of classes that define permissions for all models\n* Data validation configuration\n  * `VALIDATION_CLASSES`: Comma-separated list of classes that define [custom validations](docs/validation.md)\n\nFor development, you can also set the following environemnt variables to help\nyou:\n\n  * `DEV_AUTH_BACKEND`: Set this to "true" to enable a fake auth backend that simulates an authenticated user. Requires `DEBUG` to be set to `True` as well.\n  * `DEBUG`: Set this to true for debugging during development. Never enable this in production, as it **will** leak information to the public if you do.\n\n## Contributing\n\nLook at our [contributing guidelines](CONTRIBUTING.md) to start with your first contribution.\n\n## Maintainer\'s Handbook\n\nSome notes for maintaining this project can be found in [the maintainer\'s handbook](MAINTAINING.md).',
+    'long_description': '# alexandria\n\n[![Build Status](https://github.com/projectcaluma/emeis/workflows/Tests/badge.svg)](https://github.com/projectcaluma/emeis/actions?query=workflow%3ATests)\n[![Coverage](https://img.shields.io/badge/coverage-100%25-brightgreen.svg)](https://github.com/projectcaluma/emeis/blob/master/setup.cfg#L50)\n[![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/projectcaluma/alexandria)\n[![License: GPL-3.0-or-later](https://img.shields.io/github/license/projectcaluma/emeis)](https://spdx.org/licenses/GPL-3.0-or-later.html)\n\nOur goal is to implement an external document management service to hold and provide uploaded documents.\nDocuments can be uploaded and, depending on user access, managed by internal as well as external users.\n\nThe goal is NOT to re implement a complex [DMS](https://en.wikipedia.org/wiki/Document_management_system) but rather to have a simple and user-friendly way of managing documents with different permissions.\n\nAll User Interface interactions should be as simple as possible and easily understandable.\n\n[Original RFC that led to alexandria](docs/original_alexandria_rfc.md)\n\n## Getting started\n\n### Installation\n\n**Requirements**\n* docker\n* docker-compose\n\nAfter installing and configuring those, download [docker-compose.yml](https://raw.githubusercontent.com/projectcaluma/alexandria/master/docker-compose.yml) and run the following commands:\n\n```bash\n# only needs to be run once\necho UID=$UID > .env\n\ndocker-compose up -d\n```\n\nYou can now access the api at [http://localhost:8000/api/v1/](http://localhost:8000/api/v1/).\n\n### Example data\n\nTo load a set of categories run the following command:\n```bash\nmake load_example_data\n```\n\n### Configuration\n\nDocument Merge Service is a [12factor app](https://12factor.net/) which means that configuration is stored in environment variables.\nDifferent environment variable types are explained at [django-environ](https://github.com/joke2k/django-environ#supported-types).\n\n#### Common\n\nA list of configuration options which you need\n\n* Django configuration\n  * `SECRET_KEY`: A secret key used for cryptography. This needs to be a random string of a certain length. See [more](https://docs.djangoproject.com/en/2.1/ref/settings/#std:setting-SECRET_KEY).\n  * `ALLOWED_HOSTS`: A list of hosts/domains your service will be served from. See [more](https://docs.djangoproject.com/en/2.1/ref/settings/#allowed-hosts).\n  * `DATABASE_ENGINE`: Database backend to use. See [more](https://docs.djangoproject.com/en/2.1/ref/settings/#std:setting-DATABASE-ENGINE). (default: django.db.backends.postgresql)\n  * `DATABASE_HOST`: Host to use when connecting to database (default: localhost)\n  * `DATABASE_PORT`: Port to use when connecting to database (default: 5432)\n  * `DATABASE_NAME`: Name of database to use (default: alexandria)\n  * `DATABASE_USER`: Username to use when connecting to the database (default: alexandria)\n  * `DATABASE_PASSWORD`: Password to use when connecting to database\n* Authentication configuration\n  * `OIDC_OP_USER_ENDPOINT`: Userinfo endpoint for OIDC\n  * `OIDC_VERIFY_SSL`: Set to `false` if you want to disable verifying SSL certs. Useful for development\n  * `OIDC_DRF_AUTH_BACKEND`: Overwrite the default authentication backend with your own\n  * `ALEXANDRIA_OIDC_USER_FACTORY`: Overwrite the default user with your own\n  * `ALEXANDRIA_CREATED_BY_USER_PROPERTY`: Overwrite the default user property which is used for `..._by_user` (default: username)\n  * `ALEXANDRIA_CREATED_BY_GROUP_PROPERTY`: Overwrite the default group property which is used for `..._by_group` (default: group)\n* Authorization configurations\n  * `ALEXANDRIA_VISIBILITY_CLASSES`: Comma-separated list of classes that define visibility for all models\n  * `ALEXANDRIA_PERMISSION_CLASSES`: Comma-separated list of classes that define permissions for all models\n* Data validation configuration\n  * `ALEXANDRIA_VALIDATION_CLASSES`: Comma-separated list of classes that define [custom validations](docs/validation.md)\n\nFor development, you can also set the following environemnt variables to help\nyou:\n\n  * `DEV_AUTH_BACKEND`: Set this to "true" to enable a fake auth backend that simulates an authenticated user. Requires `DEBUG` to be set to `True` as well.\n  * `DEBUG`: Set this to true for debugging during development. Never enable this in production, as it **will** leak information to the public if you do.\n\n## Contributing\n\nLook at our [contributing guidelines](CONTRIBUTING.md) to start with your first contribution.\n\n## Maintainer\'s Handbook\n\nSome notes for maintaining this project can be found in [the maintainer\'s handbook](MAINTAINING.md).',
     'author': 'Caluma',
     'author_email': 'info@caluma.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/projectcaluma/alexandria',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `caluma_alexandria-1.1.2/PKG-INFO` & `caluma_alexandria-1.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caluma-alexandria
-Version: 1.1.2
+Version: 1.2.0
 Summary: Document management service
 Home-page: https://github.com/projectcaluma/alexandria
 License: GPL-3.0-or-later
 Author: Caluma
 Author-email: info@caluma.io
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Development Status :: 4 - Beta
@@ -90,20 +90,23 @@
   * `DATABASE_PORT`: Port to use when connecting to database (default: 5432)
   * `DATABASE_NAME`: Name of database to use (default: alexandria)
   * `DATABASE_USER`: Username to use when connecting to the database (default: alexandria)
   * `DATABASE_PASSWORD`: Password to use when connecting to database
 * Authentication configuration
   * `OIDC_OP_USER_ENDPOINT`: Userinfo endpoint for OIDC
   * `OIDC_VERIFY_SSL`: Set to `false` if you want to disable verifying SSL certs. Useful for development
-  * `OIDC_DRF_AUTH_BACKEND`: Overwrite the default authentication backend with your own.
+  * `OIDC_DRF_AUTH_BACKEND`: Overwrite the default authentication backend with your own
+  * `ALEXANDRIA_OIDC_USER_FACTORY`: Overwrite the default user with your own
+  * `ALEXANDRIA_CREATED_BY_USER_PROPERTY`: Overwrite the default user property which is used for `..._by_user` (default: username)
+  * `ALEXANDRIA_CREATED_BY_GROUP_PROPERTY`: Overwrite the default group property which is used for `..._by_group` (default: group)
 * Authorization configurations
-  * `VISIBILITY_CLASSES`: Comma-separated list of classes that define visibility for all models
-  * `PERMISSION_CLASSES`: Comma-separated list of classes that define permissions for all models
+  * `ALEXANDRIA_VISIBILITY_CLASSES`: Comma-separated list of classes that define visibility for all models
+  * `ALEXANDRIA_PERMISSION_CLASSES`: Comma-separated list of classes that define permissions for all models
 * Data validation configuration
-  * `VALIDATION_CLASSES`: Comma-separated list of classes that define [custom validations](docs/validation.md)
+  * `ALEXANDRIA_VALIDATION_CLASSES`: Comma-separated list of classes that define [custom validations](docs/validation.md)
 
 For development, you can also set the following environemnt variables to help
 you:
 
   * `DEV_AUTH_BACKEND`: Set this to "true" to enable a fake auth backend that simulates an authenticated user. Requires `DEBUG` to be set to `True` as well.
   * `DEBUG`: Set this to true for debugging during development. Never enable this in production, as it **will** leak information to the public if you do.
```

