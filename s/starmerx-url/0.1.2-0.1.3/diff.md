# Comparing `tmp/starmerx_url-0.1.2.tar.gz` & `tmp/starmerx_url-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starmerx_url-0.1.2.tar", last modified: Fri Jun  9 05:49:22 2023, max compression
+gzip compressed data, was "starmerx_url-0.1.3.tar", last modified: Fri Jun  9 08:51:09 2023, max compression
```

## Comparing `starmerx_url-0.1.2.tar` & `starmerx_url-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 jcai      (1000) jcai      (1000)        0 2023-06-09 05:49:22.418235 starmerx_url-0.1.2/
--rw-rw-r--   0 jcai      (1000) jcai      (1000)     1072 2022-11-04 02:53:51.000000 starmerx_url-0.1.2/LICENSE
--rw-rw-r--   0 jcai      (1000) jcai      (1000)      461 2023-06-09 05:49:22.418235 starmerx_url-0.1.2/PKG-INFO
--rw-rw-r--   0 jcai      (1000) jcai      (1000)      494 2023-06-09 05:48:32.000000 starmerx_url-0.1.2/README.md
--rw-rw-r--   0 jcai      (1000) jcai      (1000)       38 2023-06-09 05:49:22.418235 starmerx_url-0.1.2/setup.cfg
--rw-rw-r--   0 jcai      (1000) jcai      (1000)      784 2023-06-09 05:49:19.000000 starmerx_url-0.1.2/setup.py
-drwxrwxr-x   0 jcai      (1000) jcai      (1000)        0 2023-06-09 05:49:22.414235 starmerx_url-0.1.2/starmerx_url/
--rw-rw-r--   0 jcai      (1000) jcai      (1000)       25 2022-11-04 02:52:43.000000 starmerx_url-0.1.2/starmerx_url/__init__.py
--rw-rw-r--   0 jcai      (1000) jcai      (1000)     1905 2023-06-09 05:47:47.000000 starmerx_url-0.1.2/starmerx_url/verify_url.py
-drwxrwxr-x   0 jcai      (1000) jcai      (1000)        0 2023-06-09 05:49:22.414235 starmerx_url-0.1.2/starmerx_url.egg-info/
--rw-rw-r--   0 jcai      (1000) jcai      (1000)      461 2023-06-09 05:49:22.000000 starmerx_url-0.1.2/starmerx_url.egg-info/PKG-INFO
--rw-rw-r--   0 jcai      (1000) jcai      (1000)      253 2023-06-09 05:49:22.000000 starmerx_url-0.1.2/starmerx_url.egg-info/SOURCES.txt
--rw-rw-r--   0 jcai      (1000) jcai      (1000)        1 2023-06-09 05:49:22.000000 starmerx_url-0.1.2/starmerx_url.egg-info/dependency_links.txt
--rw-rw-r--   0 jcai      (1000) jcai      (1000)       13 2023-06-09 05:49:22.000000 starmerx_url-0.1.2/starmerx_url.egg-info/top_level.txt
--rw-rw-r--   0 jcai      (1000) jcai      (1000)        1 2022-12-13 05:51:14.000000 starmerx_url-0.1.2/starmerx_url.egg-info/zip-safe
+drwxrwxr-x   0 jcai      (1000) jcai      (1000)        0 2023-06-09 08:51:09.422678 starmerx_url-0.1.3/
+-rw-rw-r--   0 jcai      (1000) jcai      (1000)     1072 2022-11-04 02:53:51.000000 starmerx_url-0.1.3/LICENSE
+-rw-rw-r--   0 jcai      (1000) jcai      (1000)      461 2023-06-09 08:51:09.418678 starmerx_url-0.1.3/PKG-INFO
+-rw-rw-r--   0 jcai      (1000) jcai      (1000)      494 2023-06-09 05:48:32.000000 starmerx_url-0.1.3/README.md
+-rw-rw-r--   0 jcai      (1000) jcai      (1000)       38 2023-06-09 08:51:09.422678 starmerx_url-0.1.3/setup.cfg
+-rw-rw-r--   0 jcai      (1000) jcai      (1000)      784 2023-06-09 08:51:08.000000 starmerx_url-0.1.3/setup.py
+drwxrwxr-x   0 jcai      (1000) jcai      (1000)        0 2023-06-09 08:51:09.418678 starmerx_url-0.1.3/starmerx_url/
+-rw-rw-r--   0 jcai      (1000) jcai      (1000)       25 2022-11-04 02:52:43.000000 starmerx_url-0.1.3/starmerx_url/__init__.py
+-rw-rw-r--   0 jcai      (1000) jcai      (1000)     2116 2023-06-09 08:50:28.000000 starmerx_url-0.1.3/starmerx_url/verify_url.py
+drwxrwxr-x   0 jcai      (1000) jcai      (1000)        0 2023-06-09 08:51:09.418678 starmerx_url-0.1.3/starmerx_url.egg-info/
+-rw-rw-r--   0 jcai      (1000) jcai      (1000)      461 2023-06-09 08:51:09.000000 starmerx_url-0.1.3/starmerx_url.egg-info/PKG-INFO
+-rw-rw-r--   0 jcai      (1000) jcai      (1000)      253 2023-06-09 08:51:09.000000 starmerx_url-0.1.3/starmerx_url.egg-info/SOURCES.txt
+-rw-rw-r--   0 jcai      (1000) jcai      (1000)        1 2023-06-09 08:51:09.000000 starmerx_url-0.1.3/starmerx_url.egg-info/dependency_links.txt
+-rw-rw-r--   0 jcai      (1000) jcai      (1000)       13 2023-06-09 08:51:09.000000 starmerx_url-0.1.3/starmerx_url.egg-info/top_level.txt
+-rw-rw-r--   0 jcai      (1000) jcai      (1000)        1 2022-12-13 05:51:14.000000 starmerx_url-0.1.3/starmerx_url.egg-info/zip-safe
```

### Comparing `starmerx_url-0.1.2/LICENSE` & `starmerx_url-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `starmerx_url-0.1.2/starmerx_url/verify_url.py` & `starmerx_url-0.1.3/starmerx_url/verify_url.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from django.utils.deprecation import MiddlewareMixin
 
 white_url_list = list()
 
 reg1_compile = r"192\.168\.\d{1,3}.\d{1,3}"
 reg2_compile = r"192\.168\.1.\d{1,3}"
 remote_addr_real_host = ""
-referer_host = "."
+referer_host = ""
 
 if hasattr(settings, "WHITE_URL_LIST"):
     white_url_list = settings.WHITE_URL_LIST
 
 if hasattr(settings, "COMPILE_REG1"):
     reg1_compile = settings.COMPILE_REG1
 
@@ -35,25 +35,30 @@
     def validate_remote(self, request):
         remote_addr = request.META.get("REMOTE_ADDR", "")
         remote_addr_real = request.META.get("HTTP_X_REAL_IP", "")
         referer = request.META.get("HTTP_REFERER", "")
         reg2 = re.compile(reg2_compile)
         reg1 = re.compile(reg1_compile)
 
+        if referer_host:
+            return re.match(reg2, remote_addr) or \
+                   re.match(reg1, remote_addr_real) or \
+                   remote_addr_real == remote_addr_real_host or \
+                   referer_host in referer
+
         return re.match(reg2, remote_addr) or \
                re.match(reg1, remote_addr_real) or \
-               remote_addr_real == remote_addr_real_host or \
-               referer_host in referer
+               remote_addr_real == remote_addr_real_host
 
     def process_view(self, request, view_func, view_args, view_kwargs):
         user = request.user
         if (user and user.is_authenticated) or self.validate_remote(request) \
                 or 'login' in request.path or 'logout' in request.path \
                 or request.path in white_url_list:
             pass
         else:
             wrapper = {
                 'code': 401,
                 'msg': '请先登录或内网访问数据'
             }
-            no_auth_res = HttpResponse(json.dumps(wrapper), content_type='application/json')
+            no_auth_res = HttpResponse(json.dumps(wrapper), status=401, content_type='application/json')
             return no_auth_res
```

