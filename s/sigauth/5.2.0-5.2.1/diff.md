# Comparing `tmp/sigauth-5.2.0-py3-none-any.whl.zip` & `tmp/sigauth-5.2.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 6757 bytes, number of entries: 9
--rw-r--r--  2.0 unx        0 b- defN 23-May-19 14:49 sigauth/__init__.py
--rw-r--r--  2.0 unx     5548 b- defN 23-May-19 14:49 sigauth/helpers.py
--rw-r--r--  2.0 unx      915 b- defN 23-May-19 14:49 sigauth/middleware.py
--rw-r--r--  2.0 unx      434 b- defN 23-May-19 14:49 sigauth/permissions.py
--rw-r--r--  2.0 unx     1091 b- defN 23-May-19 14:50 sigauth-5.2.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     6584 b- defN 23-May-19 14:50 sigauth-5.2.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-19 14:50 sigauth-5.2.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-May-19 14:50 sigauth-5.2.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      688 b- defN 23-May-19 14:50 sigauth-5.2.0.dist-info/RECORD
-9 files, 15360 bytes uncompressed, 5573 bytes compressed:  63.7%
+Zip file size: 6885 bytes, number of entries: 9
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-09 12:50 sigauth/__init__.py
+-rw-r--r--  2.0 unx     5854 b- defN 23-Jun-09 12:50 sigauth/helpers.py
+-rw-r--r--  2.0 unx      915 b- defN 23-Jun-09 12:50 sigauth/middleware.py
+-rw-r--r--  2.0 unx      487 b- defN 23-Jun-09 12:50 sigauth/permissions.py
+-rw-r--r--  2.0 unx     1091 b- defN 23-Jun-09 12:50 sigauth-5.2.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     6584 b- defN 23-Jun-09 12:50 sigauth-5.2.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-09 12:50 sigauth-5.2.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-Jun-09 12:50 sigauth-5.2.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      688 b- defN 23-Jun-09 12:50 sigauth-5.2.1.dist-info/RECORD
+9 files, 15719 bytes uncompressed, 5701 bytes compressed:  63.7%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: sigauth/middleware.py
 Comment: 
 
 Filename: sigauth/permissions.py
 Comment: 
 
-Filename: sigauth-5.2.0.dist-info/LICENSE
+Filename: sigauth-5.2.1.dist-info/LICENSE
 Comment: 
 
-Filename: sigauth-5.2.0.dist-info/METADATA
+Filename: sigauth-5.2.1.dist-info/METADATA
 Comment: 
 
-Filename: sigauth-5.2.0.dist-info/WHEEL
+Filename: sigauth-5.2.1.dist-info/WHEEL
 Comment: 
 
-Filename: sigauth-5.2.0.dist-info/top_level.txt
+Filename: sigauth-5.2.1.dist-info/top_level.txt
 Comment: 
 
-Filename: sigauth-5.2.0.dist-info/RECORD
+Filename: sigauth-5.2.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sigauth/helpers.py

```diff
@@ -84,27 +84,28 @@
     def lookup_credentials(self, sender_id):
         return {
             'id': sender_id,
             'key': self.secret,
             'algorithm': self.algorithm
         }
 
-    def test_signature(self, request):
+    def test_signature(self, request, **kwargs):
         """
         Thest that the signature header matches the expected value.
 
         Args
             request (django.http.Request): The request to check the properties.
         Returns:
             bool or Receiver : False if rejected, Receiver instance if accepted
 
         """
+        check_nonce = kwargs.get("check_nonce")
         if self.header_name in request.META:
             # HTTP_X_SIGNATURE is present check using this method
-            return self.test_hawk_signature(request)
+            return self.test_hawk_signature(request, check_nonce=check_nonce)
         elif self.authorisation_header_name in request.META:
             # HTTP_AUTHORIZATION is present check using this method
             return self.test_hawk_authorisation(request)
         else:
             # No Authorisation header present
             raise AuthenticationFailed(NO_CREDENTIALS_MESSAGE)
 
@@ -123,25 +124,31 @@
             logger.warning(
                 'Failed authentication {e}'.format(
                     e=e,
                 )
             )
             raise AuthenticationFailed(INCORRECT_CREDENTIALS_MESSAGE)
 
-    def test_hawk_signature(self, request):
+    def test_hawk_signature(self, request, check_nonce=True):
+
+        content_type = get_content_type(request.META.get('CONTENT_TYPE'))
+        receiver_kwargs = {
+            "content": get_content(request.body),
+            "content_type": get_content_type(content_type),
+        }
+        if check_nonce:
+            receiver_kwargs.update({"seen_nonce": seen_nonce})
         try:
             content_type = get_content_type(request.META.get('CONTENT_TYPE'))
             return Receiver(
                 self.lookup_credentials,
                 request.META.get(self.header_name),
                 request.get_full_path(),
                 request.method,
-                content=get_content(request.body),
-                content_type=get_content_type(content_type),
-                seen_nonce=seen_nonce,
+                **receiver_kwargs
             )
         except HawkFail as e:
             logger.warning(
                 'Failed authentication {e}'.format(
                     e=e,
                 )
             )
@@ -188,10 +195,10 @@
     seen_cache_key = not cache.add(
         cache_key,
         True,
         timeout=120,
     )
 
     if seen_cache_key:
-        logger.warning('Already seen nonce {nonce}'.format(nonce=nonce))
+        logger.warning('Already seen nonce {nonce} via sigauth'.format(nonce=nonce))
 
     return seen_cache_key
```

## sigauth/permissions.py

```diff
@@ -1,14 +1,15 @@
 from rest_framework import permissions
 
 from sigauth.helpers import RequestSignatureChecker
 
 
 class SignatureCheckPermissionBase(permissions.BasePermission):
     secret = None
+    check_nonce = True
 
     def __init__(self, *args, **kwargs):
         self.request_checker = RequestSignatureChecker(self.secret)
         super().__init__(*args, **kwargs)
 
     def has_permission(self, request, view):
-        return self.request_checker.test_signature(request)
+        return self.request_checker.test_signature(request, check_nonce=self.check_nonce)
```

## Comparing `sigauth-5.2.0.dist-info/LICENSE` & `sigauth-5.2.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `sigauth-5.2.0.dist-info/METADATA` & `sigauth-5.2.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sigauth
-Version: 5.2.0
+Version: 5.2.1
 Summary: Signature authentication library for Export Directory.
 Home-page: https://github.com/uktrade/directory-signature-auth
 Author: Department for International Trade
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

## Comparing `sigauth-5.2.0.dist-info/RECORD` & `sigauth-5.2.1.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 sigauth/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-sigauth/helpers.py,sha256=q8KBnAzIMFKcEWJhzOQeNXeUi0WBx--JwQKjB06AHlc,5548
+sigauth/helpers.py,sha256=rUwnTTfkuonFY-FXSZu4_V9QQcsRhWMBBL8_6u_K0u8,5854
 sigauth/middleware.py,sha256=FopB3wvZaGxR6kF8B7TKC_tY_35AG0asgmdGGft95LQ,915
-sigauth/permissions.py,sha256=lmPePeQxdkAQu16CnGSE8GEN6sobBZQgaiEM79d-CwU,434
-sigauth-5.2.0.dist-info/LICENSE,sha256=y-ArErAQz98OorLek2xntwEp9bo3ZcqfQMtAIcjBdvQ,1091
-sigauth-5.2.0.dist-info/METADATA,sha256=tEWeFgzfdeManRRtkJmDYcUh7YnPTAmkmXhB7g4xCp0,6584
-sigauth-5.2.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-sigauth-5.2.0.dist-info/top_level.txt,sha256=mGlNBeKJK-HbIfvTKK_jrdMOtW4K3QcZNoGYTRSzhUc,8
-sigauth-5.2.0.dist-info/RECORD,,
+sigauth/permissions.py,sha256=c-fTj1sL2xeBeOqV1yQcBbfdton_PeFsM3CYgFdA9OE,487
+sigauth-5.2.1.dist-info/LICENSE,sha256=y-ArErAQz98OorLek2xntwEp9bo3ZcqfQMtAIcjBdvQ,1091
+sigauth-5.2.1.dist-info/METADATA,sha256=6wDnWe2tqvpLNs1HsX4dxNs0y6596Qn_CBgR3a6qC5w,6584
+sigauth-5.2.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+sigauth-5.2.1.dist-info/top_level.txt,sha256=mGlNBeKJK-HbIfvTKK_jrdMOtW4K3QcZNoGYTRSzhUc,8
+sigauth-5.2.1.dist-info/RECORD,,
```

