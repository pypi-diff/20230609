# Comparing `tmp/xj_captcha-1.0.6.tar.gz` & `tmp/xj_captcha-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\xj_captcha-1.0.6.tar", last modified: Mon Apr 24 01:12:55 2023, max compression
+gzip compressed data, was "dist\xj_captcha-1.0.9.tar", last modified: Thu May 25 09:06:43 2023, max compression
```

## Comparing `xj_captcha-1.0.6.tar` & `xj_captcha-1.0.9.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 01:12:55.000000 xj_captcha-1.0.6/
--rw-rw-rw-   0        0        0     1438 2023-04-24 01:12:55.000000 xj_captcha-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      946 2022-09-29 07:15:08.000000 xj_captcha-1.0.6/README.md
--rw-rw-rw-   0        0        0       42 2023-04-24 01:12:55.000000 xj_captcha-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0     2017 2023-04-23 07:23:34.000000 xj_captcha-1.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-24 01:12:55.000000 xj_captcha-1.0.6/xj_captcha/
--rw-rw-rw-   0        0        0        0 2022-08-26 02:08:41.000000 xj_captcha-1.0.6/xj_captcha/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-24 01:12:55.000000 xj_captcha-1.0.6/xj_captcha/apis/
--rw-rw-rw-   0        0        0     1397 2023-04-23 01:35:57.000000 xj_captcha-1.0.6/xj_captcha/apis/SmsApis.py
--rw-rw-rw-   0        0        0        0 2022-08-26 02:08:41.000000 xj_captcha-1.0.6/xj_captcha/apis/__init__.py
--rw-rw-rw-   0        0        0      923 2022-10-15 09:54:41.000000 xj_captcha-1.0.6/xj_captcha/apis/send_short_message.py
--rw-rw-rw-   0        0        0      190 2022-09-29 07:08:39.000000 xj_captcha-1.0.6/xj_captcha/apps.py
--rw-rw-rw-   0        0        0     1661 2022-08-26 02:08:41.000000 xj_captcha-1.0.6/xj_captcha/common.py
--rw-rw-rw-   0        0        0        0 2022-08-26 07:39:01.000000 xj_captcha-1.0.6/xj_captcha/models.py
-drwxrwxrwx   0        0        0        0 2023-04-24 01:12:55.000000 xj_captcha-1.0.6/xj_captcha/services/
--rw-rw-rw-   0        0        0        0 2022-08-26 02:08:41.000000 xj_captcha-1.0.6/xj_captcha/services/__init__.py
--rw-rw-rw-   0        0        0     5625 2022-12-08 07:39:37.000000 xj_captcha-1.0.6/xj_captcha/services/send_short_message_service.py
--rw-rw-rw-   0        0        0     6126 2023-04-23 07:23:45.000000 xj_captcha-1.0.6/xj_captcha/services/sms_service.py
--rw-rw-rw-   0        0        0      411 2023-04-23 01:40:00.000000 xj_captcha-1.0.6/xj_captcha/urls.py
-drwxrwxrwx   0        0        0        0 2023-04-24 01:12:55.000000 xj_captcha-1.0.6/xj_captcha/utils/
--rw-rw-rw-   0        0        0        0 2022-09-27 06:25:46.000000 xj_captcha-1.0.6/xj_captcha/utils/__init__.py
--rw-rw-rw-   0        0        0     1661 2022-08-26 02:08:41.000000 xj_captcha-1.0.6/xj_captcha/utils/common.py
--rw-rw-rw-   0        0        0     1350 2022-08-22 01:46:29.000000 xj_captcha-1.0.6/xj_captcha/utils/custom_response.py
--rw-rw-rw-   0        0        0    23527 2023-04-17 01:01:06.000000 xj_captcha-1.0.6/xj_captcha/utils/custom_tool.py
--rw-rw-rw-   0        0        0      988 2022-08-29 07:52:36.000000 xj_captcha-1.0.6/xj_captcha/utils/j_config.py
--rw-rw-rw-   0        0        0      429 2022-08-29 07:52:36.000000 xj_captcha-1.0.6/xj_captcha/utils/j_dict.py
--rw-rw-rw-   0        0        0     7311 2022-10-15 09:47:02.000000 xj_captcha-1.0.6/xj_captcha/utils/model_handle.py
--rw-rw-rw-   0        0        0     4154 2023-04-06 03:09:14.000000 xj_captcha-1.0.6/xj_captcha/utils/user_wrapper.py
--rw-rw-rw-   0        0        0     2460 2022-08-26 02:08:41.000000 xj_captcha-1.0.6/xj_captcha/utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-24 01:12:55.000000 xj_captcha-1.0.6/xj_captcha.egg-info/
--rw-rw-rw-   0        0        0     1438 2023-04-24 01:12:55.000000 xj_captcha-1.0.6/xj_captcha.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      772 2023-04-24 01:12:55.000000 xj_captcha-1.0.6/xj_captcha.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 01:12:55.000000 xj_captcha-1.0.6/xj_captcha.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       77 2023-04-24 01:12:55.000000 xj_captcha-1.0.6/xj_captcha.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-24 01:12:55.000000 xj_captcha-1.0.6/xj_captcha.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-25 09:06:43.000000 xj_captcha-1.0.9/
+-rw-rw-rw-   0        0        0     1438 2023-05-25 09:06:43.000000 xj_captcha-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      946 2022-09-29 07:15:08.000000 xj_captcha-1.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-25 09:06:43.000000 xj_captcha-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     2017 2023-05-23 09:28:41.000000 xj_captcha-1.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-25 09:06:43.000000 xj_captcha-1.0.9/xj_captcha/
+-rw-rw-rw-   0        0        0        0 2022-08-26 02:08:41.000000 xj_captcha-1.0.9/xj_captcha/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 09:06:43.000000 xj_captcha-1.0.9/xj_captcha/apis/
+-rw-rw-rw-   0        0        0     1741 2023-05-22 06:49:49.000000 xj_captcha-1.0.9/xj_captcha/apis/SmsApis.py
+-rw-rw-rw-   0        0        0        0 2022-08-26 02:08:41.000000 xj_captcha-1.0.9/xj_captcha/apis/__init__.py
+-rw-rw-rw-   0        0        0      923 2022-10-15 09:54:41.000000 xj_captcha-1.0.9/xj_captcha/apis/send_short_message.py
+-rw-rw-rw-   0        0        0      190 2022-09-29 07:08:39.000000 xj_captcha-1.0.9/xj_captcha/apps.py
+-rw-rw-rw-   0        0        0     1661 2022-08-26 02:08:41.000000 xj_captcha-1.0.9/xj_captcha/common.py
+-rw-rw-rw-   0        0        0        0 2022-08-26 07:39:01.000000 xj_captcha-1.0.9/xj_captcha/models.py
+-rw-rw-rw-   0        0        0      624 2023-05-23 09:28:14.000000 xj_captcha-1.0.9/xj_captcha/service_register.py
+drwxrwxrwx   0        0        0        0 2023-05-25 09:06:43.000000 xj_captcha-1.0.9/xj_captcha/services/
+-rw-rw-rw-   0        0        0        0 2022-08-26 02:08:41.000000 xj_captcha-1.0.9/xj_captcha/services/__init__.py
+-rw-rw-rw-   0        0        0     5549 2023-05-15 01:01:47.000000 xj_captcha-1.0.9/xj_captcha/services/send_short_message_service.py
+-rw-rw-rw-   0        0        0     8039 2023-05-22 09:08:15.000000 xj_captcha-1.0.9/xj_captcha/services/sms_service.py
+-rw-rw-rw-   0        0        0      638 2023-05-23 09:28:15.000000 xj_captcha-1.0.9/xj_captcha/urls.py
+drwxrwxrwx   0        0        0        0 2023-05-25 09:06:43.000000 xj_captcha-1.0.9/xj_captcha/utils/
+-rw-rw-rw-   0        0        0        0 2022-09-27 06:25:46.000000 xj_captcha-1.0.9/xj_captcha/utils/__init__.py
+-rw-rw-rw-   0        0        0     1661 2022-08-26 02:08:41.000000 xj_captcha-1.0.9/xj_captcha/utils/common.py
+-rw-rw-rw-   0        0        0     1350 2022-08-22 01:46:29.000000 xj_captcha-1.0.9/xj_captcha/utils/custom_response.py
+-rw-rw-rw-   0        0        0    23527 2023-04-17 01:01:06.000000 xj_captcha-1.0.9/xj_captcha/utils/custom_tool.py
+-rw-rw-rw-   0        0        0      988 2022-08-29 07:52:36.000000 xj_captcha-1.0.9/xj_captcha/utils/j_config.py
+-rw-rw-rw-   0        0        0      429 2022-08-29 07:52:36.000000 xj_captcha-1.0.9/xj_captcha/utils/j_dict.py
+-rw-rw-rw-   0        0        0     7311 2022-10-15 09:47:02.000000 xj_captcha-1.0.9/xj_captcha/utils/model_handle.py
+-rw-rw-rw-   0        0        0     4154 2023-04-06 03:09:14.000000 xj_captcha-1.0.9/xj_captcha/utils/user_wrapper.py
+-rw-rw-rw-   0        0        0     2460 2022-08-26 02:08:41.000000 xj_captcha-1.0.9/xj_captcha/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-25 09:06:43.000000 xj_captcha-1.0.9/xj_captcha.egg-info/
+-rw-rw-rw-   0        0        0     1438 2023-05-25 09:06:42.000000 xj_captcha-1.0.9/xj_captcha.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      803 2023-05-25 09:06:42.000000 xj_captcha-1.0.9/xj_captcha.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 09:06:42.000000 xj_captcha-1.0.9/xj_captcha.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       77 2023-05-25 09:06:42.000000 xj_captcha-1.0.9/xj_captcha.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-25 09:06:42.000000 xj_captcha-1.0.9/xj_captcha.egg-info/top_level.txt
```

### Comparing `xj_captcha-1.0.6/PKG-INFO` & `xj_captcha-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xj_captcha
-Version: 1.0.6
+Version: 1.0.9
 Summary: 短信模块
 Home-page: UNKNOWN
 License: apache 3.0
 Description: # xj_captcha
         
         #### 介绍
         短信模块
```

### Comparing `xj_captcha-1.0.6/README.md` & `xj_captcha-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `xj_captcha-1.0.6/setup.py` & `xj_captcha-1.0.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf8') as fp:
     log_desc = fp.read()
 
 setup(
     name='xj_captcha',  # 模块名称
-    version='1.0.6',  # 模块版本
+    version='1.0.9',  # 模块版本
     description='短信模块',  # 项目 摘要描述
     long_description=log_desc,  # 项目描述
     long_description_content_type="text/markdown",  # md文件，markdown格式
     packages=find_packages(),  # 系统自动从当前目录开始找包
     # packages=['xj_payment'],  # 系指定安装模块
     license="apache 3.0",
```

### Comparing `xj_captcha-1.0.6/xj_captcha/apis/SmsApis.py` & `xj_captcha-1.0.9/xj_captcha/apis/SmsApis.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,26 +14,36 @@
 from ..services.send_short_message_service import SendShortMessageService
 
 
 class SmsApis(APIView):
 
     # 短信验证码发送
     @require_http_methods(['POST'])
-    @user_authentication_wrapper
+    # @user_authentication_wrapper
     @request_params_wrapper
-    def send(self, *args, user_info, request_params, **kwargs, ):
+    def send(self, *args, request_params, **kwargs, ):
         params = request_params
         data, err_txt = SmsService.send_sms(params)
         if err_txt:
             return util_response(err=47767, msg=err_txt)
         return util_response(data=data)
 
     # 手机验证码检查
     @require_http_methods(['POST'])
-    @user_authentication_wrapper
+    # @user_authentication_wrapper
     @request_params_wrapper
-    def check(self, *args, user_info, request_params, **kwargs, ):
+    def check(self, *args, request_params, **kwargs, ):
         params = request_params
         data, err_txt = SmsService.check_sms(params)
         if err_txt:
             return util_response(err=47767, msg=err_txt)
         return util_response(data=data)
+
+    # 短信通知
+    @require_http_methods(['POST'])
+    @request_params_wrapper
+    def bid_send_sms(self, *args, request_params, **kwargs, ):
+        params = request_params
+        data, err_txt = SmsService.bid_send_sms(params)
+        if err_txt:
+            return util_response(err=47767, msg=err_txt)
+        return util_response(data=data)
```

### Comparing `xj_captcha-1.0.6/xj_captcha/apis/send_short_message.py` & `xj_captcha-1.0.9/xj_captcha/apis/send_short_message.py`

 * *Files identical despite different names*

### Comparing `xj_captcha-1.0.6/xj_captcha/common.py` & `xj_captcha-1.0.9/xj_captcha/common.py`

 * *Files identical despite different names*

### Comparing `xj_captcha-1.0.6/xj_captcha/services/send_short_message_service.py` & `xj_captcha-1.0.9/xj_captcha/services/send_short_message_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,16 +41,14 @@
 }
 
 
 class SendShortMessageService:
 
     @staticmethod
     def send_sms(phone, platform):
-        # phone = params['phone']
-        # platform = params['platform']
         code = SendShortMessageService.get_code(6, False)  # 生成6位验证码
         cache.set(phone, code, 300)  # 5分钟有效期
         if platform == 'ALi':
             result = SendShortMessageService.ali_send_sms(Ali, code, phone)
             dictionary = ast.literal_eval(result)
             if dictionary['Code'] == 'OK':
                 return dictionary, None
```

### Comparing `xj_captcha-1.0.6/xj_captcha/services/sms_service.py` & `xj_captcha-1.0.9/xj_captcha/services/sms_service.py`

 * *Files 18% similar despite different names*

```diff
@@ -17,14 +17,18 @@
 main_config_dict = JDict(JConfig.get_section(path=str(BASE_DIR) + "/config.ini", section="xj_captcha"))
 module_config_dict = JDict(JConfig.get_section(path=str(BASE_DIR) + "/config.ini", section="xj_captcha"))
 
 ali_accesskey_id = main_config_dict.ali_accesskey_id or module_config_dict.ali_accesskey_id or ""
 ali_accesskey_secret = main_config_dict.ali_accesskey_secret or module_config_dict.ali_accesskey_secret or ""
 ali_sign_name = main_config_dict.ali_sign_name or module_config_dict.ali_sign_name or ""
 ali_template_code = main_config_dict.ali_template_code or module_config_dict.ali_template_code or ""
+ali_new_sign_name = main_config_dict.ali_new_sign_name or module_config_dict.ali_new_sign_name or ""
+ali_register_template_code = main_config_dict.ali_register_template_code or module_config_dict.ali_register_template_code or ""
+ali_notice_template_code = main_config_dict.ali_notice_template_code or module_config_dict.ali_notice_template_code or ""
+notice_phone = main_config_dict.notice_phone or module_config_dict.notice_phone or ""
 
 tencent_accesskey_id = main_config_dict.tencent_accesskey_id or module_config_dict.tencent_accesskey_id or ""
 tencent_accesskey_secret = main_config_dict.tencent_accesskey_secret or module_config_dict.tencent_accesskey_secret or ""
 tencent_sign_name = main_config_dict.tencent_sign_name or module_config_dict.tencent_sign_name or ""
 tencent_template_code = main_config_dict.tencent_template_code or module_config_dict.tencent_template_code or ""
 
 Ali = {
@@ -39,26 +43,63 @@
     'sign_name': tencent_sign_name,
     'template_code': tencent_template_code,
 }
 
 
 class SmsService:
 
+    # 短信通知接入（只针对镖行天下）
+    @staticmethod
+    def bid_send_sms(params):
+        phone = params.get("phone", "")
+        platform = params.get("platform", "")
+        account = params.get("account", "")
+        pwd = params.get("pwd", "")
+        type = params.get("type", "")
+        bid_type = params.get("bid_type", "")
+        if not phone and type != "NOTICE":
+            return None, "手机号不能为空"
+        if not platform:
+            return None, "短信平台不能为空。请选择 Ali（阿里）"
+        if type == "PWD":
+            config = Ali
+            config['sign_name'] = ali_new_sign_name
+            config['template_code'] = ali_register_template_code
+            parameter = {
+                "account": account,
+                "pwd": pwd
+            }
+        elif type == "NOTICE":
+            config = Ali
+            config['sign_name'] = ali_new_sign_name
+            config['template_code'] = ali_notice_template_code
+            parameter = {
+                "type": bid_type
+            }
+            phone = notice_phone
+        result = SmsService.ali_send_sms(config, parameter, phone)
+        dictionary = ast.literal_eval(result)
+        if dictionary['Code'] == 'OK':
+            return dictionary, None
+        else:
+            return None, dictionary['Message']
+
     @staticmethod
     def send_sms(params):
         phone = params.get("phone", "")
         platform = params.get("platform", "")
         if not phone:
             return None, "手机号不能为空"
         if not platform:
             return None, "短信平台不能为空。请选择 Ali（阿里）或 Tencent (腾讯)"
         code = SmsService.get_code(6, False)  # 生成6位验证码
         cache.set(phone, code, 300)  # 5分钟有效期
         if platform == 'ALi':
-            result = SmsService.ali_send_sms(Ali, code, phone)
+            parameter = "{'code':%s}" % (code)
+            result = SmsService.ali_send_sms(Ali, parameter, phone)
             dictionary = ast.literal_eval(result)
             if dictionary['Code'] == 'OK':
                 return dictionary, None
             else:
                 return None, dictionary['Message']
 
         elif platform == 'Tencent':
@@ -67,29 +108,28 @@
                 return result, None
             else:
                 return None, result['errmsg']
         else:
             return None, None
 
     @staticmethod
-    def ali_send_sms(config, code, phone):
+    def ali_send_sms(config, parameter, phone):
         client = AcsClient(config['accesskey_id'], config['accesskey_secret'])
-        code = "{'code':%s}" % (code)
         request = CommonRequest()
         request.set_accept_format('json')
         request.set_domain('dysmsapi.aliyuncs.com')  # url
         request.set_method('POST')
         request.set_protocol_type('https')  # https | http
         request.set_version('2017-05-25')
         request.set_action_name('SendSms')
         request.add_query_param('RegionId', 'cn-hangzhou')
         request.add_query_param('PhoneNumbers', phone)  # 待发送手机号
         request.add_query_param('SignName', config['sign_name'])  # 短信签名
         request.add_query_param('TemplateCode', config['template_code'])  # 短信模板code
-        request.add_query_param('TemplateParam', code)
+        request.add_query_param('TemplateParam', parameter)
         response = client.do_action_with_exception(request)
         # python2: print(response)
         return str(response, encoding='utf-8')
 
     @staticmethod
     def tencent_send_sms(config, code, phone):
         """
@@ -114,16 +154,18 @@
     @staticmethod
     def check_sms(params):
         phone = params.get("phone", "")
         code = params.get('sms_code')
         if code is None:
             return None, "验证码不能为空"
         cache_code = cache.get(phone)
-        if code != cache_code:
+        # cache_code = "000000"
+        if code != str(cache_code):
             return None, "验证码不正确"
+        cache.delete(phone)
         return None, None
 
     # 数字表示生成几位, True表示生成带有字母的 False不带字母的
     @staticmethod
     def get_code(n=6, alpha=False):
         s = ''  # 创建字符串变量,存储生成的验证码
         for i in range(n):  # 通过for循环控制验证码位数
```

### Comparing `xj_captcha-1.0.6/xj_captcha/utils/common.py` & `xj_captcha-1.0.9/xj_captcha/utils/common.py`

 * *Files identical despite different names*

### Comparing `xj_captcha-1.0.6/xj_captcha/utils/custom_response.py` & `xj_captcha-1.0.9/xj_captcha/utils/custom_response.py`

 * *Files identical despite different names*

### Comparing `xj_captcha-1.0.6/xj_captcha/utils/custom_tool.py` & `xj_captcha-1.0.9/xj_captcha/utils/custom_tool.py`

 * *Files identical despite different names*

### Comparing `xj_captcha-1.0.6/xj_captcha/utils/j_config.py` & `xj_captcha-1.0.9/xj_captcha/utils/j_config.py`

 * *Files identical despite different names*

### Comparing `xj_captcha-1.0.6/xj_captcha/utils/model_handle.py` & `xj_captcha-1.0.9/xj_captcha/utils/model_handle.py`

 * *Files identical despite different names*

### Comparing `xj_captcha-1.0.6/xj_captcha/utils/user_wrapper.py` & `xj_captcha-1.0.9/xj_captcha/utils/user_wrapper.py`

 * *Files identical despite different names*

### Comparing `xj_captcha-1.0.6/xj_captcha/utils/utils.py` & `xj_captcha-1.0.9/xj_captcha/utils/utils.py`

 * *Files identical despite different names*

### Comparing `xj_captcha-1.0.6/xj_captcha.egg-info/PKG-INFO` & `xj_captcha-1.0.9/xj_captcha.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xj-captcha
-Version: 1.0.6
+Version: 1.0.9
 Summary: 短信模块
 Home-page: UNKNOWN
 License: apache 3.0
 Description: # xj_captcha
         
         #### 介绍
         短信模块
```

### Comparing `xj_captcha-1.0.6/xj_captcha.egg-info/SOURCES.txt` & `xj_captcha-1.0.9/xj_captcha.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 README.md
 setup.py
 xj_captcha/__init__.py
 xj_captcha/apps.py
 xj_captcha/common.py
 xj_captcha/models.py
+xj_captcha/service_register.py
 xj_captcha/urls.py
 xj_captcha.egg-info/PKG-INFO
 xj_captcha.egg-info/SOURCES.txt
 xj_captcha.egg-info/dependency_links.txt
 xj_captcha.egg-info/requires.txt
 xj_captcha.egg-info/top_level.txt
 xj_captcha/apis/SmsApis.py
```

