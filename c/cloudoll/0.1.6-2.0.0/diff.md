# Comparing `tmp/cloudoll-0.1.6.tar.gz` & `tmp/cloudoll-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudoll-0.1.6.tar", last modified: Thu Nov  3 03:33:43 2022, max compression
+gzip compressed data, was "cloudoll-2.0.0.tar", last modified: Fri Jun  9 06:35:35 2023, max compression
```

## Comparing `cloudoll-0.1.6.tar` & `cloudoll-2.0.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2022-11-03 03:33:43.319776 cloudoll-0.1.6/
--rw-rw-rw-   0        0        0     1065 2022-07-18 10:31:06.000000 cloudoll-0.1.6/LICENSE
--rw-rw-rw-   0        0        0    21242 2022-11-03 03:33:43.317775 cloudoll-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0    20567 2022-11-03 03:31:58.000000 cloudoll-0.1.6/README.md
-drwxrwxrwx   0        0        0        0 2022-11-03 03:33:43.132028 cloudoll-0.1.6/cloudoll/
--rw-rw-rw-   0        0        0        0 2022-07-19 03:42:12.000000 cloudoll-0.1.6/cloudoll/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-03 03:33:43.259524 cloudoll-0.1.6/cloudoll/error/
--rw-rw-rw-   0        0        0        0 2022-07-01 10:11:13.000000 cloudoll-0.1.6/cloudoll/error/__init__.py
--rw-rw-rw-   0        0        0     3549 2022-07-22 04:14:59.000000 cloudoll-0.1.6/cloudoll/error/errors.py
-drwxrwxrwx   0        0        0        0 2022-11-03 03:33:43.263519 cloudoll-0.1.6/cloudoll/logging/
--rw-rw-rw-   0        0        0     3951 2022-10-31 04:21:33.000000 cloudoll-0.1.6/cloudoll/logging/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-03 03:33:43.270208 cloudoll-0.1.6/cloudoll/mail/
--rw-rw-rw-   0        0        0        0 2022-07-18 02:25:44.000000 cloudoll-0.1.6/cloudoll/mail/__init__.py
--rw-rw-rw-   0        0        0     5879 2022-11-03 03:24:46.000000 cloudoll-0.1.6/cloudoll/mail/smtp.py
-drwxrwxrwx   0        0        0        0 2022-11-03 03:33:43.277222 cloudoll-0.1.6/cloudoll/orm/
--rw-rw-rw-   0        0        0        0 2022-07-01 10:09:39.000000 cloudoll-0.1.6/cloudoll/orm/__init__.py
--rw-rw-rw-   0        0        0    25450 2022-10-20 04:06:31.000000 cloudoll-0.1.6/cloudoll/orm/mysql.py
-drwxrwxrwx   0        0        0        0 2022-11-03 03:33:43.287217 cloudoll-0.1.6/cloudoll/robot/
--rw-rw-rw-   0        0        0        0 2022-07-23 10:06:35.000000 cloudoll-0.1.6/cloudoll/robot/__init__.py
--rw-rw-rw-   0        0        0     6541 2022-07-24 14:13:10.000000 cloudoll-0.1.6/cloudoll/robot/dingtalk.py
--rw-rw-rw-   0        0        0     3214 2022-07-24 14:13:26.000000 cloudoll-0.1.6/cloudoll/robot/feishu.py
-drwxrwxrwx   0        0        0        0 2022-11-03 03:33:43.313773 cloudoll-0.1.6/cloudoll/web/
--rw-rw-rw-   0        0        0        0 2022-07-06 03:24:26.000000 cloudoll-0.1.6/cloudoll/web/__init__.py
--rw-rw-rw-   0        0        0     2170 2022-08-31 06:32:31.000000 cloudoll-0.1.6/cloudoll/web/html.py
--rw-rw-rw-   0        0        0     3466 2022-09-29 07:20:42.000000 cloudoll-0.1.6/cloudoll/web/http.py
--rw-rw-rw-   0        0        0     1067 2022-08-09 02:09:46.000000 cloudoll-0.1.6/cloudoll/web/jwt.py
--rw-rw-rw-   0        0        0     7014 2022-11-03 03:25:28.000000 cloudoll-0.1.6/cloudoll/web/server.py
-drwxrwxrwx   0        0        0        0 2022-11-03 03:33:43.252538 cloudoll-0.1.6/cloudoll.egg-info/
--rw-rw-rw-   0        0        0    21242 2022-11-03 03:33:42.000000 cloudoll-0.1.6/cloudoll.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      571 2022-11-03 03:33:43.000000 cloudoll-0.1.6/cloudoll.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-03 03:33:42.000000 cloudoll-0.1.6/cloudoll.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       85 2022-11-03 03:33:42.000000 cloudoll-0.1.6/cloudoll.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2022-11-03 03:33:42.000000 cloudoll-0.1.6/cloudoll.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-11-03 03:33:43.319776 cloudoll-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0     4259 2022-11-03 03:33:36.000000 cloudoll-0.1.6/setup.py
+drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2023-06-09 06:35:35.378219 cloudoll-2.0.0/
+-rw-r--r--   0 xiaobei    (501) staff       (20)     1059 2023-03-15 06:24:14.000000 cloudoll-2.0.0/LICENSE
+-rw-r--r--   0 xiaobei    (501) staff       (20)     7008 2023-06-09 06:35:35.377763 cloudoll-2.0.0/PKG-INFO
+-rw-r--r--   0 xiaobei    (501) staff       (20)     6375 2023-06-09 06:22:48.000000 cloudoll-2.0.0/README.md
+drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2023-06-09 06:35:35.363990 cloudoll-2.0.0/cloudoll/
+-rw-r--r--   0 xiaobei    (501) staff       (20)        0 2023-03-15 06:24:14.000000 cloudoll-2.0.0/cloudoll/__init__.py
+drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2023-06-09 06:35:35.368538 cloudoll-2.0.0/cloudoll/error/
+-rw-r--r--   0 xiaobei    (501) staff       (20)        0 2023-03-15 06:24:14.000000 cloudoll-2.0.0/cloudoll/error/__init__.py
+-rw-r--r--   0 xiaobei    (501) staff       (20)     3501 2023-03-15 06:24:14.000000 cloudoll-2.0.0/cloudoll/error/errors.py
+drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2023-06-09 06:35:35.369127 cloudoll-2.0.0/cloudoll/logging/
+-rw-r--r--   0 xiaobei    (501) staff       (20)     3817 2023-04-26 01:55:04.000000 cloudoll-2.0.0/cloudoll/logging/__init__.py
+drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2023-06-09 06:35:35.370114 cloudoll-2.0.0/cloudoll/mail/
+-rw-r--r--   0 xiaobei    (501) staff       (20)        0 2023-03-15 06:24:14.000000 cloudoll-2.0.0/cloudoll/mail/__init__.py
+-rw-r--r--   0 xiaobei    (501) staff       (20)     5741 2023-05-23 03:27:31.000000 cloudoll-2.0.0/cloudoll/mail/smtp.py
+drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2023-06-09 06:35:35.371453 cloudoll-2.0.0/cloudoll/orm/
+-rw-r--r--   0 xiaobei    (501) staff       (20)        0 2023-03-15 06:24:14.000000 cloudoll-2.0.0/cloudoll/orm/__init__.py
+-rw-r--r--   0 xiaobei    (501) staff       (20)    27881 2023-06-08 13:00:49.000000 cloudoll-2.0.0/cloudoll/orm/mysql.py
+drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2023-06-09 06:35:35.373657 cloudoll-2.0.0/cloudoll/robot/
+-rw-r--r--   0 xiaobei    (501) staff       (20)        0 2023-03-15 06:24:14.000000 cloudoll-2.0.0/cloudoll/robot/__init__.py
+-rw-r--r--   0 xiaobei    (501) staff       (20)     6380 2023-03-22 06:00:15.000000 cloudoll-2.0.0/cloudoll/robot/dingtalk.py
+-rw-r--r--   0 xiaobei    (501) staff       (20)     3114 2023-03-22 06:01:06.000000 cloudoll-2.0.0/cloudoll/robot/feishu.py
+drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2023-06-09 06:35:35.376835 cloudoll-2.0.0/cloudoll/web/
+-rw-r--r--   0 xiaobei    (501) staff       (20)    13406 2023-06-08 12:53:24.000000 cloudoll-2.0.0/cloudoll/web/__init__.py
+-rw-r--r--   0 xiaobei    (501) staff       (20)     2077 2023-03-15 06:24:14.000000 cloudoll-2.0.0/cloudoll/web/html.py
+-rw-r--r--   0 xiaobei    (501) staff       (20)     3541 2023-05-23 03:27:31.000000 cloudoll-2.0.0/cloudoll/web/http.py
+-rw-r--r--   0 xiaobei    (501) staff       (20)     1097 2023-06-05 02:36:30.000000 cloudoll-2.0.0/cloudoll/web/jwt.py
+-rw-r--r--   0 xiaobei    (501) staff       (20)      298 2023-04-24 09:13:28.000000 cloudoll-2.0.0/cloudoll/web/settings.py
+drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2023-06-09 06:35:35.367489 cloudoll-2.0.0/cloudoll.egg-info/
+-rw-r--r--   0 xiaobei    (501) staff       (20)     7008 2023-06-09 06:35:35.000000 cloudoll-2.0.0/cloudoll.egg-info/PKG-INFO
+-rw-r--r--   0 xiaobei    (501) staff       (20)      573 2023-06-09 06:35:35.000000 cloudoll-2.0.0/cloudoll.egg-info/SOURCES.txt
+-rw-r--r--   0 xiaobei    (501) staff       (20)        1 2023-06-09 06:35:35.000000 cloudoll-2.0.0/cloudoll.egg-info/dependency_links.txt
+-rw-r--r--   0 xiaobei    (501) staff       (20)      103 2023-06-09 06:35:35.000000 cloudoll-2.0.0/cloudoll.egg-info/requires.txt
+-rw-r--r--   0 xiaobei    (501) staff       (20)        9 2023-06-09 06:35:35.000000 cloudoll-2.0.0/cloudoll.egg-info/top_level.txt
+-rw-r--r--   0 xiaobei    (501) staff       (20)       38 2023-06-09 06:35:35.378354 cloudoll-2.0.0/setup.cfg
+-rw-r--r--   0 xiaobei    (501) staff       (20)     4158 2023-06-09 06:34:21.000000 cloudoll-2.0.0/setup.py
```

### Comparing `cloudoll-0.1.6/LICENSE` & `cloudoll-2.0.0/LICENSE`

 * *Ordering differences only*

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-Copyright <YEAR> <COPYRIGHT HOLDER>
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
-
+Copyright <YEAR> <COPYRIGHT HOLDER>
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `cloudoll-0.1.6/cloudoll/error/errors.py` & `cloudoll-2.0.0/cloudoll/error/errors.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,48 +1,48 @@
-ERROR = {
-    CUSTOM: {code: -1, message: "%s"},
-    HSF_ERROR: {code: -6, message: "HSF 调用失败：%s。"},
-    SYSTEM_ERROR: {code: -10, message: "系统错误。"},
-    BAD_REQUEST: {code: -400, message: "错误的 http 请求。"},
-    NOT_FOUND: {code: -404, message: "您请求的 http 资源没有找到。"},
-    INTERNAL_SERVER_ERROR: {code: -500, message: "内部服务器错误。"},
-    DB: {code: -700, message: "%s"},
-    DATA_OCCUPIED: {code: -701, message: "数据被占用。"},
-    WHAT_REQUIRE: {code: -1001, message: "缺少参数 %s。"},
-    WHAT_WRONG_RANGE: {code: -1002, message: "%s 的取值范围错误。最小 %s，最大 %s"},
-    WHAT_WRONG_FORMAT: {code: -1003, message: "%s 格式不正确。"},
-    WHAT_NOT_SAME: {code: -1004, message: "输入的 %s 值不一致。"},
-    WHAT_NOT_EXISTS: {code: -1005, message: "%s 不存在。"},
-    WHAT_TOO_MUCH: {code: -1006, message: "%s 太多了。"},
-    WHAT_TOO_LITTLE: {code: -1007, message: "%s 太少了。"},
-    WHAT_NOT_BELONGS_TO_YOU: {code: -1008, message: "%s 不属于你。"},
-    WHAT_TOO_LONG: {code: -1009, message: "%s 太长了，请不要超过 %s。"},
-    WHAT_TOO_SHORT: {code: -1010, message: "%s 太短了，请不要少于 %s。"},
-    WHAT_EXISTED: {code: -1011, message: "%s 已经存在。"},
-    WHAT_OCCUPIED: {code: -1012, message: "%s 被占用。"},
-    WHAT_TIMEOUT: {code: -1013, message: "%s 已超时。"},
-    WHAT_EXPIRED: {code: -1014, message: "%s 已过期。"},
-    WHAT_ILLEGAL: {code: -1015, message: "%s 不合法。"},
-    WHAT_NOT_FOUND: {code: -1016, message: "%s 没找到。"},
-    WHAT_WRONG_LENGTH_RANGE: {code: -1017, message: "%s 的长度错误，最短是 %s，最长 %s。"},
-    WHAT_WRONG_TYPE: {code: -1018, message: "%s 的类型错误"},
-    ACCESS_TOKEN_NOT_FOUND: {code: -2001, message: "access_token 不存在。"},
-    ACCESS_TOKEN_EXPIRED: {code: -2002, message: "access_token 已经过期。"},
-    TICKET_EXPIRED: {code: -2050, message: "票据已经过期，请重新获取。"},
-    TICKET_VERIFY_FAILED: {code: -2051, message: "票据校验失败。篡改登录信息是违法行为！"},
-    TICKET_ILLEGAL: {code: -2052, message: "非法票据。篡改登录信息是违法行为！"},
-    SIGN_VERIFY_FAILED: {code: -2053, message: "签名验证失败。"},
-    PASSWORD_NOT_STRONG: {code: -3001, message: "密码太简单。%s"},
-    CHINA_MOBILE_ILLEGAL: {code: -3002, message: "不正确的手机号码。"},
-    EMAIL_ILLEGAL: {code: -3003, message: "不正确的Email。"},
-    CAPTCHA_VALIDATE_FAIL: {code: -3004, message: "验证码校验失败。"},
-    PASSPORT_ILLEGAL: {code: -3005, message: "不正确的登录凭据，必须是手机或者 Email。"},
-    MEMBER_ONLY: {code: -3006, message: "您还没有登录，请登录。"},
-    NO_RIGHTS: {code: -3007, message: "您没有权限，请联系管理员授权。"},
-    LOGIN_ERROR: {code: -3050, message: "登录失败"},
-    LOGIN_ERROR_BECAUSE: {code: -3051, message: "登录失败。%s"},
-    MEMBER_NOT_EXISTS: {code: -3052, message: "用户不存在。"},
-    MEMBER_NOT_APPROVED: {code: -3053, message: "尚未审批通过，请耐心等待。"},
-    MEMBER_FORBIDDEN: {code: -3054, message: "您已经被系统禁止。"},
-    MEMBER_LOGIN_TOO_MUCH_FAILURE: {code: -3055, message: "您登录失败的次数太多。暂时被系统锁定"},
-    IP_LOGIN_TOO_MUCH: {code: -3056, message: "您登录失败的次数太多。暴力破解他人密码是违法行为！"},
-}
+ERROR = {
+    CUSTOM: {code: -1, message: "%s"},
+    HSF_ERROR: {code: -6, message: "HSF 调用失败：%s。"},
+    SYSTEM_ERROR: {code: -10, message: "系统错误。"},
+    BAD_REQUEST: {code: -400, message: "错误的 http 请求。"},
+    NOT_FOUND: {code: -404, message: "您请求的 http 资源没有找到。"},
+    INTERNAL_SERVER_ERROR: {code: -500, message: "内部服务器错误。"},
+    DB: {code: -700, message: "%s"},
+    DATA_OCCUPIED: {code: -701, message: "数据被占用。"},
+    WHAT_REQUIRE: {code: -1001, message: "缺少参数 %s。"},
+    WHAT_WRONG_RANGE: {code: -1002, message: "%s 的取值范围错误。最小 %s，最大 %s"},
+    WHAT_WRONG_FORMAT: {code: -1003, message: "%s 格式不正确。"},
+    WHAT_NOT_SAME: {code: -1004, message: "输入的 %s 值不一致。"},
+    WHAT_NOT_EXISTS: {code: -1005, message: "%s 不存在。"},
+    WHAT_TOO_MUCH: {code: -1006, message: "%s 太多了。"},
+    WHAT_TOO_LITTLE: {code: -1007, message: "%s 太少了。"},
+    WHAT_NOT_BELONGS_TO_YOU: {code: -1008, message: "%s 不属于你。"},
+    WHAT_TOO_LONG: {code: -1009, message: "%s 太长了，请不要超过 %s。"},
+    WHAT_TOO_SHORT: {code: -1010, message: "%s 太短了，请不要少于 %s。"},
+    WHAT_EXISTED: {code: -1011, message: "%s 已经存在。"},
+    WHAT_OCCUPIED: {code: -1012, message: "%s 被占用。"},
+    WHAT_TIMEOUT: {code: -1013, message: "%s 已超时。"},
+    WHAT_EXPIRED: {code: -1014, message: "%s 已过期。"},
+    WHAT_ILLEGAL: {code: -1015, message: "%s 不合法。"},
+    WHAT_NOT_FOUND: {code: -1016, message: "%s 没找到。"},
+    WHAT_WRONG_LENGTH_RANGE: {code: -1017, message: "%s 的长度错误，最短是 %s，最长 %s。"},
+    WHAT_WRONG_TYPE: {code: -1018, message: "%s 的类型错误"},
+    ACCESS_TOKEN_NOT_FOUND: {code: -2001, message: "access_token 不存在。"},
+    ACCESS_TOKEN_EXPIRED: {code: -2002, message: "access_token 已经过期。"},
+    TICKET_EXPIRED: {code: -2050, message: "票据已经过期，请重新获取。"},
+    TICKET_VERIFY_FAILED: {code: -2051, message: "票据校验失败。篡改登录信息是违法行为！"},
+    TICKET_ILLEGAL: {code: -2052, message: "非法票据。篡改登录信息是违法行为！"},
+    SIGN_VERIFY_FAILED: {code: -2053, message: "签名验证失败。"},
+    PASSWORD_NOT_STRONG: {code: -3001, message: "密码太简单。%s"},
+    CHINA_MOBILE_ILLEGAL: {code: -3002, message: "不正确的手机号码。"},
+    EMAIL_ILLEGAL: {code: -3003, message: "不正确的Email。"},
+    CAPTCHA_VALIDATE_FAIL: {code: -3004, message: "验证码校验失败。"},
+    PASSPORT_ILLEGAL: {code: -3005, message: "不正确的登录凭据，必须是手机或者 Email。"},
+    MEMBER_ONLY: {code: -3006, message: "您还没有登录，请登录。"},
+    NO_RIGHTS: {code: -3007, message: "您没有权限，请联系管理员授权。"},
+    LOGIN_ERROR: {code: -3050, message: "登录失败"},
+    LOGIN_ERROR_BECAUSE: {code: -3051, message: "登录失败。%s"},
+    MEMBER_NOT_EXISTS: {code: -3052, message: "用户不存在。"},
+    MEMBER_NOT_APPROVED: {code: -3053, message: "尚未审批通过，请耐心等待。"},
+    MEMBER_FORBIDDEN: {code: -3054, message: "您已经被系统禁止。"},
+    MEMBER_LOGIN_TOO_MUCH_FAILURE: {code: -3055, message: "您登录失败的次数太多。暂时被系统锁定"},
+    IP_LOGIN_TOO_MUCH: {code: -3056, message: "您登录失败的次数太多。暴力破解他人密码是违法行为！"},
+}
```

### Comparing `cloudoll-0.1.6/cloudoll/robot/dingtalk.py` & `cloudoll-2.0.0/cloudoll/robot/dingtalk.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,203 +1,209 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-
-# docs: https://open.dingtalk.com/document/group/message-types-and-data-format
-__author__ = "chuchur/chuchur.com"
-
-
-import hashlib, hmac, time, base64, logging, requests as http, urllib, json
-
-class Client(object):
-    def __init__(self, **kw):
-        self._webhook = kw.get("webhook")
-        self._secret = kw.get("secret")
-        self._access_token = kw.get("access_token")
-
-    def _get_sign(self):
-        secret = self._secret
-        if not secret:
-            logging.error("缺少secret")
-            return None, None
-
-        # 拼接timestamp和secret
-        timestamp = str(round(time.time() * 1000))
-        string_to_sign = "{}\n{}".format(timestamp, secret)
-        hmac_code = hmac.new(
-            secret.encode("utf-8"),
-            string_to_sign.encode("utf-8"),
-            digestmod=hashlib.sha256,
-        ).digest()
-
-        # 对结果进行base64处理
-        sign = base64.b64encode(hmac_code).decode("utf-8")
-        sign = urllib.parse.quote(sign)
-        return timestamp, sign
-
-    def upload(self, type: str, filepath: str):
-        """
-        上传媒体
-        :params access_token
-        :params type 文件类型 image|voice|video|file
-        :params filepath 要上传的文件路径
-        """
-        access_token = self._access_token
-        if not access_token:
-            logging.error("请配置access_token")
-            return False
-        url = "https://oapi.dingtalk.com/media/upload?access_token=%s" % access_token
-        with open(filepath, "rb") as f:
-            files = {"media": f}
-            result = http.post(url=url, files=files, data={"type": type})
-            res = result.json()
-            if res["errcode"] == 0:
-                return res
-            else:
-                logging.error(res["errmsg"])
-
-    def send(self, data: dict):
-        """
-        发送除签名外的自定义消息结构体 https://open.dingtalk.com/document/orgapp-server/message-types-and-data-format
-        :params data 自定义消息结构体
-        """
-        webhook = self._webhook
-        if not webhook:
-            logging.error("缺少webhook")
-            return False
-        timestamp, sign = self._get_sign()
-        if not timestamp or not sign:
-            return False
-        url = webhook + "&timestamp=%s&sign=%s" % (timestamp, sign)
-        result = http.post(
-            url=url,
-            json={**data},
-            # data=data
-            # data=json.dumps(data)
-        )
-        if result:
-            res = result.json()
-            if res["errcode"] == 0:
-                logging.info("发送成功！")
-                return True
-            else:
-                logging.info("发送失败")
-                logging.error(res["errmsg"])
-                return False
-
-    def sendtext(self, text: str):
-        """
-        发送文本消息
-        :params text 消息内容
-        """
-
-        return self.send(
-            data={
-                "msgtype": "text",
-                "text": {"content": text},
-            }
-        )
-
-    def _send_media(self, type, media_id, **kw):
-        """
-        发送媒体
-        :params type 媒体类型 image|voice|video|file
-        :params media_id 媒体ID
-        """
-        data = {"msgtype": type}
-        data[type] = {"media_id": media_id}
-        if type == "voice":
-            data["voice"]["duration"] = kw.get("duration")
-        return self.send(data)
-
-    def sendmarkdown(self, title, text):
-        """
-        发送Markdown消息
-        :params title 标题
-        :params text markdown结构体
-        """
-        return self.send(
-            data={"msgtype": "markdown", "markdown": {"title": title, "text": text}}
-        )
-
-    def sendimage(self, media_id: str):
-        """
-        发送图片消息
-        :params media_id 媒体ID
-        """
-        return self._send_media("image", media_id)
-
-    def sendvoice(self, media_id: str, duration: str):
-        """
-        发送语音消息
-        :params media_id 媒体ID
-        :params duration 正整数，小于60，表示音频时长。
-        """
-        return self._send_media("voice", media_id, duration=duration)
-
-    def sendfile(self, media_id: str):
-        """
-        发送文件消息
-        :params media_id 媒体ID
-        """
-        return self._send_media("file", media_id)
-
-    def sendlink(self, messageUrl, picUrl, title, text):
-        """
-        发送链接消息
-        :params messageUrl 链接地址
-        :params picUrl 链接的小图
-        :params title 链接标题 100字内
-        :params text 链接副标题 500字内
-        """
-        return self.send(
-            data={
-                "msgtype": "link",
-                "link": {
-                    "picUrl": picUrl,
-                    "messageUrl": messageUrl,
-                    "title": title,
-                    "text": text,
-                },
-            }
-        )
-
-    def sendcard(self, **kw):
-        """
-        发送卡片消息
-        :params title 标题
-        :params text 消息内容 必填
-        :params single_title 查看详情(按钮文字) btns 二选一
-        :params single_url 查看详情(链接) btns 二选一
-        :params btn_orientation 按钮排列顺序。0|1
-        :params btns 按钮 [{title:'',actionURL:''}]
-        """
-        title = kw.get("title", "")
-        text = kw.get("text", "")
-        single_title = kw.get("single_title", "")
-        single_url = kw.get("single_url", "")
-        btn_orientation = kw.get("btn_orientation", 0)
-        btns = kw.get("btns", []) or []
-        return self.send(
-            data={
-                "msgtype": "actionCard",
-                "actionCard": {
-                    "title": title,
-                    "text": text,
-                    "singleTitle": single_title,
-                    "singleUrl": single_url,
-                    "btnOrientation": btn_orientation,
-                    "btns": btns,
-                },
-            }
-        )
-
-    def sendfreecard(self, links: list):
-        """
-        发送卡片消息
-        :params links [{ title:'',messageURL:'',picURL:''}]
-        """
-        return self.send(
-            data={
-                "msgtype": "feedCard",
-                "feedCard": {"links": links},
-            }
-        )
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+
+# docs: https://open.dingtalk.com/document/group/message-types-and-data-format
+__author__ = "chuchur/chuchur.com"
+
+import base64
+import hashlib
+import hmac
+import logging
+import requests as http
+import time
+from urllib import parse
+
+
+class Client(object):
+    def __init__(self, **kw):
+        self._webhook = kw.get("webhook")
+        self._secret = kw.get("secret")
+        self._access_token = kw.get("access_token")
+
+    def _get_sign(self):
+        secret = self._secret
+        if not secret:
+            logging.error("缺少secret")
+            return None, None
+
+        # 拼接timestamp和secret
+        timestamp = str(round(time.time() * 1000))
+        string_to_sign = "{}\n{}".format(timestamp, secret)
+        hmac_code = hmac.new(
+            secret.encode("utf-8"),
+            string_to_sign.encode("utf-8"),
+            digestmod=hashlib.sha256,
+        ).digest()
+
+        # 对结果进行base64处理
+        sign = base64.b64encode(hmac_code).decode("utf-8")
+        sign = parse.quote(sign)
+        return timestamp, sign
+
+    def upload(self, type: str, filepath: str):
+        """
+        上传媒体
+        :params access_token
+        :params type 文件类型 image|voice|video|file
+        :params filepath 要上传的文件路径
+        """
+        access_token = self._access_token
+        if not access_token:
+            logging.error("请配置access_token")
+            return False
+        url = "https://oapi.dingtalk.com/media/upload?access_token=%s" % access_token
+        with open(filepath, "rb") as f:
+            files = {"media": f}
+            result = http.post(url=url, files=files, data={"type": type})
+            res = result.json()
+            if res["errcode"] == 0:
+                return res
+            else:
+                logging.error(res["errmsg"])
+
+    def send(self, data: dict):
+        """
+        发送除签名外的自定义消息结构体 https://open.dingtalk.com/document/orgapp-server/message-types-and-data-format
+        :params data 自定义消息结构体
+        """
+        webhook = self._webhook
+        if not webhook:
+            logging.error("缺少webhook")
+            return False
+        timestamp, sign = self._get_sign()
+        if not timestamp or not sign:
+            return False
+        url = webhook + "&timestamp=%s&sign=%s" % (timestamp, sign)
+        result = http.post(
+            url=url,
+            json={**data},
+            # data=data
+            # data=json.dumps(data)
+        )
+        if result:
+            res = result.json()
+            if res["errcode"] == 0:
+                logging.info("发送成功！")
+                return True
+            else:
+                logging.info("发送失败")
+                logging.error(res["errmsg"])
+                return False
+
+    def send_text(self, text: str):
+        """
+        发送文本消息
+        :params text 消息内容
+        """
+
+        return self.send(
+            data={
+                "msgtype": "text",
+                "text": {"content": text},
+            }
+        )
+
+    def _send_media(self, type, media_id, **kw):
+        """
+        发送媒体
+        :params type 媒体类型 image|voice|video|file
+        :params media_id 媒体ID
+        """
+        data = {"msgtype": type}
+        data[type] = {"media_id": media_id}
+        if type == "voice":
+            data["voice"]["duration"] = kw.get("duration")
+        return self.send(data)
+
+    def send_markdown(self, title, text):
+        """
+        发送Markdown消息
+        :params title 标题
+        :params text markdown结构体
+        """
+        return self.send(
+            data={"msgtype": "markdown", "markdown": {"title": title, "text": text}}
+        )
+
+    def send_image(self, media_id: str):
+        """
+        发送图片消息
+        :params media_id 媒体ID
+        """
+        return self._send_media("image", media_id)
+
+    def send_voice(self, media_id: str, duration: str):
+        """
+        发送语音消息
+        :params media_id 媒体ID
+        :params duration 正整数，小于60，表示音频时长。
+        """
+        return self._send_media("voice", media_id, duration=duration)
+
+    def send_file(self, media_id: str):
+        """
+        发送文件消息
+        :params media_id 媒体ID
+        """
+        return self._send_media("file", media_id)
+
+    def send_link(self, messageUrl, picUrl, title, text):
+        """
+        发送链接消息
+        :params messageUrl 链接地址
+        :params picUrl 链接的小图
+        :params title 链接标题 100字内
+        :params text 链接副标题 500字内
+        """
+        return self.send(
+            data={
+                "msgtype": "link",
+                "link": {
+                    "picUrl": picUrl,
+                    "messageUrl": messageUrl,
+                    "title": title,
+                    "text": text,
+                },
+            }
+        )
+
+    def send_card(self, **kw):
+        """
+        发送卡片消息
+        :params title 标题
+        :params text 消息内容 必填
+        :params single_title 查看详情(按钮文字) btns 二选一
+        :params single_url 查看详情(链接) btns 二选一
+        :params btn_orientation 按钮排列顺序。0|1
+        :params btns 按钮 [{title:'',actionURL:''}]
+        """
+        title = kw.get("title", "")
+        text = kw.get("text", "")
+        single_title = kw.get("single_title", "")
+        single_url = kw.get("single_url", "")
+        btn_orientation = kw.get("btn_orientation", 0)
+        btns = kw.get("btns", []) or []
+        return self.send(
+            data={
+                "msgtype": "actionCard",
+                "actionCard": {
+                    "title": title,
+                    "text": text,
+                    "singleTitle": single_title,
+                    "singleUrl": single_url,
+                    "btnOrientation": btn_orientation,
+                    "btns": btns,
+                },
+            }
+        )
+
+    def send_freecard(self, links: list):
+        """
+        发送卡片消息
+        :params links [{ title:'',messageURL:'',picURL:''}]
+        """
+        return self.send(
+            data={
+                "msgtype": "feedCard",
+                "feedCard": {"links": links},
+            }
+        )
```

### Comparing `cloudoll-0.1.6/cloudoll/web/http.py` & `cloudoll-2.0.0/cloudoll/web/http.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,132 +1,138 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
- 
-__author__ = "chuchur/chuchur.com"
-
-import requests, time
-from cloudoll import logging
-
-logging.getLogger()
-PROXIES = {
-    "http": "http://127.0.0.1:7890",
-    "https": "http://127.0.0.1:7890",
-}
-
-HEADERS = {
-    "sec-ch-ua": '"Not A;Brand";v="99", "Chromium";v="102", "Google Chrome";v="102"',
-    "sec-ch-ua-mobile": "?0",
-    "sec-ch-ua-platform": "Windows",
-    "sec-fetch-dest": "empty",
-    "sec-fetch-mode": "cors",
-    "Expires": "0",
-    "Pragma": "no-cache",
-    "Cache": "no-cache",
-    "Cache-control": "no-cache",
-    "Connection": "keep-alive",
-    # "Content-Type": "application/json; charset=UTF-8",
-    "User-Agent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_14_5) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/75.0.3770.100 Safari/537.36",
-}
-
-
-class Client(object):
-    def __init__(self):
-        self.session = requests.Session()
-
-    def requests(self, method, url, **kw):
-        headers = kw.get("headers", None)
-        if headers is None:
-            headers = HEADERS
-        else:
-            headers = {**headers, **HEADERS}
-        kw["headers"] = headers
-        proxies = kw.get("proxies", False)
-        if proxies:
-            if proxies is True:
-                kw["proxies"] = PROXIES
-            else:
-                kw["proxies"] = proxies
-        trytimes = kw.get("trytimes", 2)
-        if trytimes != 2:
-            kw.pop("trytimes")
-        result = None
-        while trytimes > 0:
-            try:
-                fun = getattr(self.session, method, None)
-                result = fun(url, **kw)
-                trytimes = 0
-                head = result.headers
-                ctype = head["Content-Type"]
-                if "application/json" in ctype:
-                    return result.json()
-                elif "text/html" in ctype:
-                    return result.text
-                return result
-            except BaseException as e:
-                # logging.info(e)
-                logging.error("Network error ,try gain....")
-                trytimes -= 1
-                time.sleep(2)
-                # logging.info(e)
-        return result
-
-
-http = Client()
-
-
-def get(url, **kw):
-    """
-    get 请求
-    :params params=dict() 传参
-    """
-    return http.requests("get", url, **kw)
-
-
-def post(url, **kw):
-    """
-    post 请求
-    :params data=dict() or json=dict() 传参
-    """
-    return http.requests("post", url, **kw)
-
-
-def put(url, **kw):
-    """
-    post 请求
-    data=dict()传参
-    """
-    return http.requests("put", url, **kw)
-
-
-def delete(url, **kw):
-    return http.requests("delete", url, **kw)
-
-
-def head(url, **kw):
-    return http.requests("head", url, **kw)
-
-
-def option(url, **kw):
-    return http.requests("option", url, **kw)
-
-
-def download(url, savepath=None, **kw):
-    """
-    下载文件
-    :params url 文件的地址
-    :params savepath 保存路径
-    """
-    rb = http.requests("get", url, **kw)
-    if not savepath:
-        return rb.content
-    if not rb:
-        logging.error("下载出错")
-        return False
-    else:
-        try:
-            with open(savepath, "wb") as f:
-                f.write(rb.content)
-                logging.info("下载完成！")
-        except BaseException as e:
-            logging.error(e)
-            return False
-    return True
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+ 
+__author__ = "chuchur/chuchur.com"
+
+import requests
+import time
+
+from ..logging import logging
+
+PROXIES = {
+    "http": "http://127.0.0.1:7890",
+    "https": "http://127.0.0.1:7890",
+}
+
+HEADERS = {
+    "sec-ch-ua": '"Not A;Brand";v="99", "Chromium";v="102", "Google Chrome";v="102"',
+    "sec-ch-ua-mobile": "?0",
+    "sec-ch-ua-platform": "Windows",
+    "sec-fetch-dest": "empty",
+    "sec-fetch-mode": "cors",
+    "Expires": "0",
+    "Pragma": "no-cache",
+    "Cache": "no-cache",
+    "Cache-control": "no-cache",
+    "Connection": "keep-alive",
+    # "Content-Type": "application/json; charset=UTF-8",
+    "User-Agent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_14_5) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/75.0.3770.100 Safari/537.36",
+}
+
+
+class Client(object):
+    def __init__(self):
+        self.session = requests.Session()
+
+    def requests(self, method, url, **kw):
+        headers = kw.get("headers", None)
+        if headers is None:
+            headers = HEADERS
+        else:
+            headers = {**headers, **HEADERS}
+        kw["headers"] = headers
+        proxies = kw.get("proxies", False)
+        if proxies:
+            if proxies is True:
+                kw["proxies"] = PROXIES
+            else:
+                kw["proxies"] = proxies
+        trytimes = kw.get("trytimes", 2)
+        if trytimes != 2:
+            kw.pop("trytimes")
+        result = None
+        while trytimes > 0:
+            try:
+                fun = getattr(self.session, method, None)
+                result = fun(url, **kw)
+                trytimes = 0
+                head = result.headers
+                ctype = head["Content-Type"]
+                if result.status_code==200:
+                    if "application/json" in ctype:
+                        return result.json()
+                    elif "text/html" in ctype:
+                        return result.text
+                    return result
+                else:
+                    logging.error("Network error ,try gain....")
+                    trytimes += 1
+                    time.sleep(2)
+            except BaseException as e:
+                # logging.info(e)
+                logging.error("Network error ,try gain....")
+                trytimes -= 1
+                time.sleep(2)
+                # logging.info(e)
+        return result
+
+
+http = Client()
+
+
+def get(url, **kw):
+    """
+    get 请求
+    :params params=dict() 传参
+    """
+    return http.requests("get", url, **kw)
+
+
+def post(url, **kw):
+    """
+    post 请求
+    :params data=dict() or json=dict() 传参
+    """
+    return http.requests("post", url, **kw)
+
+
+def put(url, **kw):
+    """
+    post 请求
+    data=dict()传参
+    """
+    return http.requests("put", url, **kw)
+
+
+def delete(url, **kw):
+    return http.requests("delete", url, **kw)
+
+
+def head(url, **kw):
+    return http.requests("head", url, **kw)
+
+
+def option(url, **kw):
+    return http.requests("option", url, **kw)
+
+
+def download(url, savepath=None, **kw):
+    """
+    下载文件
+    :params url 文件的地址
+    :params savepath 保存路径
+    """
+    rb = http.requests("get", url, **kw)
+    if not savepath:
+        return rb.content
+    if not rb:
+        logging.error("下载出错")
+        return False
+    else:
+        try:
+            with open(savepath, "wb") as f:
+                f.write(rb.content)
+                logging.info("下载完成！")
+        except BaseException as e:
+            logging.error(e)
+            return False
+    return True
```

### Comparing `cloudoll-0.1.6/cloudoll/web/jwt.py` & `cloudoll-2.0.0/cloudoll/web/jwt.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,40 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-
-__author__ = "chuchur/chuchur.com"
-
-import jwt,datetime
-
-def encode(payload, key, exp=3600):
-    """
-    jwt 加密
-    :params payload 数据
-    :params key 密钥
-    :params exp 过期时间单位秒，默认1个小时
-    """
-    headers = dict(typ="jwt", alg="HS256")
-    exp = datetime.datetime.now() + datetime.timedelta(seconds=exp)  # 过期时间
-    payload["exp"] = exp.timestamp()
-    resut = jwt.encode(payload=payload, key=key, algorithm="HS256", headers=headers)
-    return resut
-     
-
-def decode(token, key):
-    """
-    jwt 解密
-    :params token 加密后的数据
-    :params key 密钥
-    """
-    try:
-        payload = jwt.decode(token, key, algorithms=['HS256'])
-        if not payload:
-            return None
-        now = datetime.datetime.now().timestamp()  # 当前时间
-        if int(now) > int(payload["exp"]):  # 登录时间过期
-            return None
-        return payload  # 返回自定义内容
-    except Exception:
-        return None
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+
+__author__ = "chuchur/chuchur.com"
+
+import jwt, datetime
+from ..logging import logging
+
+
+def encode(payload, key, exp: [int, str] = 3600):
+    """
+    jwt 加密
+    :params payload
+    :params key
+    :params exp 过期时间单位秒，默认1个小时
+    """
+    headers = dict(typ="jwt", alg="HS256")
+    exp = datetime.datetime.now() + datetime.timedelta(seconds=eval(exp) if isinstance(exp, str) else exp)  # 过期时间
+    payload["exp"] = exp.timestamp()
+    result = jwt.encode(payload=payload, key=key, algorithm="HS256", headers=headers)
+    return result
+
+
+def decode(token, key):
+    """
+    jwt
+    :params token
+    :params key
+    """
+    try:
+        payload = jwt.decode(token, key, algorithms=['HS256'])
+        if not payload:
+            return None
+        now = datetime.datetime.now().timestamp()  # 当前时间
+        if int(now) > int(payload["exp"]):  # 登录时间过期
+            return None
+        return payload  # 返回自定义内容
+    except Exception as e:
+        logging.error(e)
+        return None
```

### Comparing `cloudoll-0.1.6/cloudoll.egg-info/SOURCES.txt` & `cloudoll-2.0.0/cloudoll.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -17,8 +17,8 @@
 cloudoll/robot/__init__.py
 cloudoll/robot/dingtalk.py
 cloudoll/robot/feishu.py
 cloudoll/web/__init__.py
 cloudoll/web/html.py
 cloudoll/web/http.py
 cloudoll/web/jwt.py
-cloudoll/web/server.py
+cloudoll/web/settings.py
```

### Comparing `cloudoll-0.1.6/setup.py` & `cloudoll-2.0.0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,140 +1,142 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-
-# Note: To use the 'upload' functionality of this file, you must:
-#   $ pipenv install twine --dev # pip install --user --upgrade twine
-# python setup.py sdist build && python setup.py bdist_wheel && python setup.py sdist upload
-import io
-import os
-import sys
-from shutil import rmtree
-
-from setuptools import find_packages, setup, Command
-
-# Package meta-data.
-NAME = "cloudoll"
-DESCRIPTION = "辅助快速创建可分布的微服务。"
-URL = "https://gitee.com/chuchur/cloudoll-py"
-EMAIL = "chuchur@qq.com"
-AUTHOR = "chuchur"
-REQUIRES_PYTHON = ">=3.6.0"
-VERSION = "0.1.6"
-
-# What packages are required for this module to be executed?
-REQUIRED = [
-    "requests",
-    "aiomysql",
-    "colorlog",
-    "aiohttp",
-    "jinja2",
-    "pyjwt",
-    "aiohttp_session[secure]",
-    "numpy",
-    "fernet"
-]
-
-# What packages are optional?
-EXTRAS = {
-    # 'fancy feature': ['django'],
-}
-
-# The rest you shouldn't have to touch too much :)
-# ------------------------------------------------
-# Except, perhaps the License and Trove Classifiers!
-# If you do change the License, remember to change the Trove Classifier for that!
-
-here = os.path.abspath(os.path.dirname(__file__))
-
-# Import the README and use it as the long-description.
-# Note: this will only work if 'README.md' is present in your MANIFEST.in file!
-try:
-    with io.open(os.path.join(here, "README.md"), encoding="utf-8") as f:
-        long_description = "\n" + f.read()
-except FileNotFoundError:
-    long_description = DESCRIPTION
-
-# Load the package's __version__.py module as a dictionary.
-about = {}
-if not VERSION:
-    project_slug = NAME.lower().replace("-", "_").replace(" ", "_")
-    with open(os.path.join(here, project_slug, "__version__.py")) as f:
-        exec(f.read(), about)
-else:
-    about["__version__"] = VERSION
-
-
-class UploadCommand(Command):
-    """Support setup.py upload."""
-
-    description = "Build and publish the package."
-    user_options = []
-
-    @staticmethod
-    def status(s):
-        """Prints things in bold."""
-        print("\033[1m{0}\033[0m".format(s))
-
-    def initialize_options(self):
-        pass
-
-    def finalize_options(self):
-        pass
-
-    def run(self):
-        try:
-            self.status("Removing previous builds…")
-            rmtree(os.path.join(here, "dist"))
-        except OSError:
-            pass
-
-        self.status("Building Source and Wheel (universal) distribution…")
-        os.system("{0} setup.py sdist bdist_wheel --universal".format(sys.executable))
-
-        self.status("Uploading the package to PyPI via Twine…")
-        os.system("twine upload dist/*")
-
-        self.status("Pushing git tags…")
-        os.system("git tag v{0}".format(about["__version__"]))
-        os.system("git push --tags")
-
-        sys.exit()
-
-
-# Where the magic happens:
-setup(
-    name=NAME,
-    version=about["__version__"],
-    description=DESCRIPTION,
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    author=AUTHOR,
-    author_email=EMAIL,
-    python_requires=REQUIRES_PYTHON,
-    url=URL,
-    packages=find_packages(exclude=["tests", "*.tests", "*.tests.*", "tests.*"]),
-    # If your package is a single module, use this instead of 'packages':
-    # py_modules=['mypackage'],
-    # entry_points={
-    #     'console_scripts': ['mycli=mymodule:cli'],
-    # },
-    install_requires=REQUIRED,
-    extras_require=EXTRAS,
-    include_package_data=True,
-    license="MIT",
-    classifiers=[
-        # Trove classifiers
-        # Full list: https://pypi.python.org/pypi?%3Aaction=list_classifiers
-        "License :: OSI Approved :: MIT License",
-        "Programming Language :: Python",
-        "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: Implementation :: CPython",
-        "Programming Language :: Python :: Implementation :: PyPy",
-    ],
-    # $ setup.py publish support.
-    cmdclass={
-        "upload": UploadCommand,
-    },
-)
-
-# python setup.py sdist build && python setup.py bdist_wheel && python setup.py sdist upload
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+
+# Note: To use the 'upload' functionality of this file, you must:
+#   $ pipenv install twine --dev # pip install --user --upgrade twine
+# python setup.py sdist build && python setup.py bdist_wheel && python setup.py sdist upload
+import io
+import os
+import sys
+from shutil import rmtree
+
+from setuptools import find_packages, setup, Command
+
+# Package meta-data.
+NAME = "cloudoll"
+DESCRIPTION = "辅助快速创建可分布的微服务。"
+URL = "https://gitee.com/chuchur/cloudoll-py"
+EMAIL = "chuchur@qq.com"
+AUTHOR = "chuchur"
+REQUIRES_PYTHON = ">=3.6.0"
+VERSION = "2.0.0"
+
+# What packages are required for this module to be executed?
+REQUIRED = [
+    "requests",
+    "colorlog",
+    "aiomysql",
+    "aiopg",
+    "aiohttp",
+    "aioredis",
+    "aiomcache"
+    "jinja2",
+    "pyjwt",
+    "aiohttp_session[secure]",
+    "PyYAML",
+]
+
+# What packages are optional?
+EXTRAS = {
+    # 'fancy feature': ['django'],
+}
+
+# The rest you shouldn't have to touch too much :)
+# ------------------------------------------------
+# Except, perhaps the License and Trove Classifiers!
+# If you do change the License, remember to change the Trove Classifier for that!
+
+here = os.path.abspath(os.path.dirname(__file__))
+
+# Import the README and use it as the long-description.
+# Note: this will only work if 'README.md' is present in your MANIFEST.in file!
+try:
+    with io.open(os.path.join(here, "README.md"), encoding="utf-8") as f:
+        long_description = "\n" + f.read()
+except FileNotFoundError:
+    long_description = DESCRIPTION
+
+# Load the package's __version__.py module as a dictionary.
+about = {}
+if not VERSION:
+    project_slug = NAME.lower().replace("-", "_").replace(" ", "_")
+    with open(os.path.join(here, project_slug, "__version__.py")) as f:
+        exec(f.read(), about)
+else:
+    about["__version__"] = VERSION
+
+
+class UploadCommand(Command):
+    """Support setup.py upload."""
+
+    description = "Build and publish the package."
+    user_options = []
+
+    @staticmethod
+    def status(s):
+        """Prints things in bold."""
+        print("\033[1m{0}\033[0m".format(s))
+
+    def initialize_options(self):
+        pass
+
+    def finalize_options(self):
+        pass
+
+    def run(self):
+        try:
+            self.status("Removing previous builds…")
+            rmtree(os.path.join(here, "dist"))
+        except OSError:
+            pass
+
+        self.status("Building Source and Wheel (universal) distribution…")
+        os.system("{0} setup.py sdist bdist_wheel --universal".format(sys.executable))
+
+        self.status("Uploading the package to PyPI via Twine…")
+        os.system("twine upload dist/*")
+
+        # self.status("Pushing git tags…")
+        # os.system("git tag v{0}".format(about["__version__"]))
+        # os.system("git push --tags")
+
+        sys.exit()
+
+
+# Where the magic happens:
+setup(
+    name=NAME,
+    version=about["__version__"],
+    description=DESCRIPTION,
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    author=AUTHOR,
+    author_email=EMAIL,
+    python_requires=REQUIRES_PYTHON,
+    url=URL,
+    packages=find_packages(exclude=["tests", "*.tests", "*.tests.*", "tests.*"]),
+    # If your package is a single module, use this instead of 'packages':
+    # py_modules=['mypackage'],
+    # entry_points={
+    #     'console_scripts': ['mycli=mymodule:cli'],
+    # },
+    install_requires=REQUIRED,
+    extras_require=EXTRAS,
+    include_package_data=True,
+    license="MIT",
+    classifiers=[
+        # Trove classifiers
+        # Full list: https://pypi.python.org/pypi?%3Aaction=list_classifiers
+        "License :: OSI Approved :: MIT License",
+        "Programming Language :: Python",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: Implementation :: CPython",
+        "Programming Language :: Python :: Implementation :: PyPy",
+    ],
+    # $ setup.py publish support.
+    cmdclass={
+        "upload": UploadCommand,
+    },
+)
+
+# python setup.py sdist build && python setup.py bdist_wheel && python setup.py sdist upload
```

