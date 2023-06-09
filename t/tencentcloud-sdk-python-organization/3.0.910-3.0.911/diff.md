# Comparing `tmp/tencentcloud-sdk-python-organization-3.0.910.tar.gz` & `tmp/tencentcloud-sdk-python-organization-3.0.911.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-organization-3.0.910.tar", last modified: Thu Jun  8 09:16:44 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-organization-3.0.911.tar", last modified: Fri Jun  9 02:24:22 2023, max compression
```

## Comparing `tencentcloud-sdk-python-organization-3.0.910.tar` & `tencentcloud-sdk-python-organization-3.0.911.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 09:16:44.000000 tencentcloud-sdk-python-organization-3.0.910/
--rw-r--r--   0 root         (0) root         (0)      764 2023-06-08 09:16:44.000000 tencentcloud-sdk-python-organization-3.0.910/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 09:16:44.000000 tencentcloud-sdk-python-organization-3.0.910/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 09:16:44.000000 tencentcloud-sdk-python-organization-3.0.910/tencentcloud/organization/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 09:16:44.000000 tencentcloud-sdk-python-organization-3.0.910/tencentcloud/organization/v20210331/
--rw-r--r--   0 root         (0) root         (0)    17475 2023-06-08 09:16:44.000000 tencentcloud-sdk-python-organization-3.0.910/tencentcloud/organization/v20210331/organization_client.py
--rw-r--r--   0 root         (0) root         (0)     8203 2023-06-08 09:16:44.000000 tencentcloud-sdk-python-organization-3.0.910/tencentcloud/organization/v20210331/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 09:16:44.000000 tencentcloud-sdk-python-organization-3.0.910/tencentcloud/organization/v20210331/__init__.py
--rw-r--r--   0 root         (0) root         (0)    55554 2023-06-08 09:16:44.000000 tencentcloud-sdk-python-organization-3.0.910/tencentcloud/organization/v20210331/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 09:16:44.000000 tencentcloud-sdk-python-organization-3.0.910/tencentcloud/organization/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 09:16:44.000000 tencentcloud-sdk-python-organization-3.0.910/tencentcloud/organization/v20181225/
--rw-r--r--   0 root         (0) root         (0)    19620 2023-06-08 09:16:44.000000 tencentcloud-sdk-python-organization-3.0.910/tencentcloud/organization/v20181225/organization_client.py
--rw-r--r--   0 root         (0) root         (0)     3243 2023-06-08 09:16:44.000000 tencentcloud-sdk-python-organization-3.0.910/tencentcloud/organization/v20181225/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 09:16:44.000000 tencentcloud-sdk-python-organization-3.0.910/tencentcloud/organization/v20181225/__init__.py
--rw-r--r--   0 root         (0) root         (0)    30659 2023-06-08 09:16:44.000000 tencentcloud-sdk-python-organization-3.0.910/tencentcloud/organization/v20181225/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-08 09:16:44.000000 tencentcloud-sdk-python-organization-3.0.910/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 09:16:44.000000 tencentcloud-sdk-python-organization-3.0.910/tencentcloud_sdk_python_organization.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 09:16:44.000000 tencentcloud-sdk-python-organization-3.0.910/tencentcloud_sdk_python_organization.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      738 2023-06-08 09:16:44.000000 tencentcloud-sdk-python-organization-3.0.910/tencentcloud_sdk_python_organization.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1704 2023-06-08 09:16:44.000000 tencentcloud-sdk-python-organization-3.0.910/tencentcloud_sdk_python_organization.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-08 09:16:44.000000 tencentcloud-sdk-python-organization-3.0.910/tencentcloud_sdk_python_organization.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1704 2023-06-08 09:16:44.000000 tencentcloud-sdk-python-organization-3.0.910/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1024 2023-06-08 09:16:44.000000 tencentcloud-sdk-python-organization-3.0.910/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-08 09:16:44.000000 tencentcloud-sdk-python-organization-3.0.910/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:24:22.000000 tencentcloud-sdk-python-organization-3.0.911/
+-rw-r--r--   0 root         (0) root         (0)      764 2023-06-09 02:24:22.000000 tencentcloud-sdk-python-organization-3.0.911/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:24:22.000000 tencentcloud-sdk-python-organization-3.0.911/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:24:22.000000 tencentcloud-sdk-python-organization-3.0.911/tencentcloud/organization/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:24:22.000000 tencentcloud-sdk-python-organization-3.0.911/tencentcloud/organization/v20210331/
+-rw-r--r--   0 root         (0) root         (0)    20412 2023-06-09 02:24:22.000000 tencentcloud-sdk-python-organization-3.0.911/tencentcloud/organization/v20210331/organization_client.py
+-rw-r--r--   0 root         (0) root         (0)    10169 2023-06-09 02:24:22.000000 tencentcloud-sdk-python-organization-3.0.911/tencentcloud/organization/v20210331/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 02:24:22.000000 tencentcloud-sdk-python-organization-3.0.911/tencentcloud/organization/v20210331/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    61815 2023-06-09 02:24:22.000000 tencentcloud-sdk-python-organization-3.0.911/tencentcloud/organization/v20210331/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 02:24:22.000000 tencentcloud-sdk-python-organization-3.0.911/tencentcloud/organization/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:24:22.000000 tencentcloud-sdk-python-organization-3.0.911/tencentcloud/organization/v20181225/
+-rw-r--r--   0 root         (0) root         (0)    19620 2023-06-09 02:24:22.000000 tencentcloud-sdk-python-organization-3.0.911/tencentcloud/organization/v20181225/organization_client.py
+-rw-r--r--   0 root         (0) root         (0)     3243 2023-06-09 02:24:22.000000 tencentcloud-sdk-python-organization-3.0.911/tencentcloud/organization/v20181225/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 02:24:22.000000 tencentcloud-sdk-python-organization-3.0.911/tencentcloud/organization/v20181225/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    30659 2023-06-09 02:24:22.000000 tencentcloud-sdk-python-organization-3.0.911/tencentcloud/organization/v20181225/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-09 02:24:22.000000 tencentcloud-sdk-python-organization-3.0.911/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:24:22.000000 tencentcloud-sdk-python-organization-3.0.911/tencentcloud_sdk_python_organization.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 02:24:22.000000 tencentcloud-sdk-python-organization-3.0.911/tencentcloud_sdk_python_organization.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      738 2023-06-09 02:24:22.000000 tencentcloud-sdk-python-organization-3.0.911/tencentcloud_sdk_python_organization.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1704 2023-06-09 02:24:22.000000 tencentcloud-sdk-python-organization-3.0.911/tencentcloud_sdk_python_organization.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-09 02:24:22.000000 tencentcloud-sdk-python-organization-3.0.911/tencentcloud_sdk_python_organization.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1704 2023-06-09 02:24:22.000000 tencentcloud-sdk-python-organization-3.0.911/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1024 2023-06-09 02:24:22.000000 tencentcloud-sdk-python-organization-3.0.911/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-09 02:24:22.000000 tencentcloud-sdk-python-organization-3.0.911/setup.cfg
```

### Comparing `tencentcloud-sdk-python-organization-3.0.910/README.rst` & `tencentcloud-sdk-python-organization-3.0.911/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-organization-3.0.910/tencentcloud/organization/v20210331/organization_client.py` & `tencentcloud-sdk-python-organization-3.0.911/tencentcloud/organization/v20210331/organization_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,14 +22,37 @@
 
 class OrganizationClient(AbstractClient):
     _apiVersion = '2021-03-31'
     _endpoint = 'organization.tencentcloudapi.com'
     _service = 'organization'
 
 
+    def AddOrganizationMemberEmail(self, request):
+        """添加组织成员邮箱
+
+        :param request: Request instance for AddOrganizationMemberEmail.
+        :type request: :class:`tencentcloud.organization.v20210331.models.AddOrganizationMemberEmailRequest`
+        :rtype: :class:`tencentcloud.organization.v20210331.models.AddOrganizationMemberEmailResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("AddOrganizationMemberEmail", params, headers=headers)
+            response = json.loads(body)
+            model = models.AddOrganizationMemberEmailResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def AddOrganizationNode(self, request):
         """添加企业组织节点
 
         :param request: Request instance for AddOrganizationNode.
         :type request: :class:`tencentcloud.organization.v20210331.models.AddOrganizationNodeRequest`
         :rtype: :class:`tencentcloud.organization.v20210331.models.AddOrganizationNodeResponse`
 
@@ -275,14 +298,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def DescribeOrganizationMemberEmailBind(self, request):
+        """查询成员邮箱绑定详细信息
+
+        :param request: Request instance for DescribeOrganizationMemberEmailBind.
+        :type request: :class:`tencentcloud.organization.v20210331.models.DescribeOrganizationMemberEmailBindRequest`
+        :rtype: :class:`tencentcloud.organization.v20210331.models.DescribeOrganizationMemberEmailBindResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeOrganizationMemberEmailBind", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeOrganizationMemberEmailBindResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def DescribeOrganizationMemberPolicies(self, request):
         """获取组织成员的授权策略列表
 
         :param request: Request instance for DescribeOrganizationMemberPolicies.
         :type request: :class:`tencentcloud.organization.v20210331.models.DescribeOrganizationMemberPoliciesRequest`
         :rtype: :class:`tencentcloud.organization.v20210331.models.DescribeOrganizationMemberPoliciesResponse`
 
@@ -388,14 +434,37 @@
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
+
+
+    def UpdateOrganizationMemberEmailBind(self, request):
+        """修改绑定成员邮箱
+
+        :param request: Request instance for UpdateOrganizationMemberEmailBind.
+        :type request: :class:`tencentcloud.organization.v20210331.models.UpdateOrganizationMemberEmailBindRequest`
+        :rtype: :class:`tencentcloud.organization.v20210331.models.UpdateOrganizationMemberEmailBindResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("UpdateOrganizationMemberEmailBind", params, headers=headers)
+            response = json.loads(body)
+            model = models.UpdateOrganizationMemberEmailBindResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
 
 
     def UpdateOrganizationNode(self, request):
         """更新企业组织节点
 
         :param request: Request instance for UpdateOrganizationNode.
         :type request: :class:`tencentcloud.organization.v20210331.models.UpdateOrganizationNodeRequest`
```

### Comparing `tencentcloud-sdk-python-organization-3.0.910/tencentcloud/organization/v20210331/errorcodes.py` & `tencentcloud-sdk-python-organization-3.0.911/tencentcloud/organization/v20210331/errorcodes.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,20 +10,35 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
+# 该帐号已被注册。
+FAILEDOPERATION_ACCOUNTALREADYREGISTER = 'FailedOperation.AccountAlreadyRegister'
+
 # 用户未实名。
 FAILEDOPERATION_AUTHINFOEMPTY = 'FailedOperation.AuthInfoEmpty'
 
 # 用户非企业实名。
 FAILEDOPERATION_AUTHNOTENTERPRISE = 'FailedOperation.AuthNotEnterprise'
 
+# 绑定邮箱链接过期。
+FAILEDOPERATION_BINDEMAILLINKEXPIRED = 'FailedOperation.BindEmailLinkExpired'
+
+# 绑定邮箱链接无效。
+FAILEDOPERATION_BINDEMAILLINKINVALID = 'FailedOperation.BindEmailLinkInvalid'
+
+# 检查手机绑定上限失败。
+FAILEDOPERATION_CHECKACCOUNTPHONEBINDLIMIT = 'FailedOperation.CheckAccountPhoneBindLimit'
+
+# 检查邮箱绑定状态失败。
+FAILEDOPERATION_CHECKMAILACCOUNT = 'FailedOperation.CheckMailAccount'
+
 # 创建成员异常。
 FAILEDOPERATION_CREATEACCOUNT = 'FailedOperation.CreateAccount'
 
 # 添加计费权限失败。
 FAILEDOPERATION_CREATEBILLINGPERMISSIONERR = 'FailedOperation.CreateBillingPermissionErr'
 
 # 账号实名认证超过上限。
@@ -40,17 +55,32 @@
 
 # 创建角色异常。
 FAILEDOPERATION_CREATEROLE = 'FailedOperation.CreateRole'
 
 # 不能退出自己创建的企业组织。
 FAILEDOPERATION_DISABLEQUITSELFCREATEDORGANIZATION = 'FailedOperation.DisableQuitSelfCreatedOrganization'
 
+# 邮箱已经被使用。
+FAILEDOPERATION_EMAILALREADYUSED = 'FailedOperation.EmailAlreadyUsed'
+
+# 邮箱绑定已经失效。
+FAILEDOPERATION_EMAILBINDRECORDINVALID = 'FailedOperation.EmailBindRecordInvalid'
+
 # 查询实名信息出错。
 FAILEDOPERATION_GETAUTHINFO = 'FailedOperation.GetAuthInfo'
 
+# 邮箱绑定失败。
+FAILEDOPERATION_MEMBERBINDEMAILERROR = 'FailedOperation.MemberBindEmailError'
+
+# 安全手机绑定失败。
+FAILEDOPERATION_MEMBERBINDPHONEERROR = 'FailedOperation.MemberBindPhoneError'
+
+# 成员存在邮箱。
+FAILEDOPERATION_MEMBEREMAILEXIST = 'FailedOperation.MemberEmailExist'
+
 # 成员存在代付者,不允许删除。
 FAILEDOPERATION_MEMBEREXISTDELEGATEPAYERNOTALLOWDELETE = 'FailedOperation.MemberExistDelegatePayerNotAllowDelete'
 
 # 成员是代付者，不允许删除。
 FAILEDOPERATION_MEMBERISDELEGATEPAYERNOTALLOWDELETE = 'FailedOperation.MemberIsDelegatePayerNotAllowDelete'
 
 # 名字已经被使用。
@@ -115,26 +145,50 @@
 
 # 内部错误。
 INTERNALERROR = 'InternalError'
 
 # 参数错误。
 INVALIDPARAMETER = 'InvalidParameter'
 
+# 手机验证码错误。
+INVALIDPARAMETER_CODEERROR = 'InvalidParameter.CodeError'
+
+# 手机验证码已过期。
+INVALIDPARAMETER_CODEEXPIRED = 'InvalidParameter.CodeExpired'
+
+# 无效的邮箱。
+INVALIDPARAMETER_INVALIDEMAIL = 'InvalidParameter.InvalidEmail'
+
+# 密码不合法。
+INVALIDPARAMETER_PASSWORDILLEGAL = 'InvalidParameter.PasswordIllegal'
+
 # 创建成员超过上限。
 LIMITEXCEEDED_CREATEMEMBEROVERLIMIT = 'LimitExceeded.CreateMemberOverLimit'
 
+# 配置邮箱超过当日上限。
+LIMITEXCEEDED_EMAILBINDOVERLIMIT = 'LimitExceeded.EmailBindOverLimit'
+
 # 企业组织单元层级太多。
 LIMITEXCEEDED_NODEDEPTHEXCEEDLIMIT = 'LimitExceeded.NodeDepthExceedLimit'
 
 # 组织单元数量超过上限。
 LIMITEXCEEDED_NODEEXCEEDLIMIT = 'LimitExceeded.NodeExceedLimit'
 
 # 成员超过上限。
 LIMITEXCEEDED_ORGANIZATIONMEMBEROVERLIMIT = 'LimitExceeded.OrganizationMemberOverLimit'
 
+# 手机超过绑定上限。
+LIMITEXCEEDED_PHONENUMBOUND = 'LimitExceeded.PhoneNumBound'
+
+# 修改成员绑定信息超过限制。
+LIMITEXCEEDED_UPDATEEMAILBINDOVERLIMIT = 'LimitExceeded.UpdateEmailBindOverLimit'
+
+# 邮箱绑定记录不存在。
+RESOURCENOTFOUND_EMAILBINDRECORDNOTEXIST = 'ResourceNotFound.EmailBindRecordNotExist'
+
 # 成员可授权身份不存在。
 RESOURCENOTFOUND_MEMBERIDENTITYNOTEXIST = 'ResourceNotFound.MemberIdentityNotExist'
 
 # 成员不存在。
 RESOURCENOTFOUND_MEMBERNOTEXIST = 'ResourceNotFound.MemberNotExist'
 
 # 组织成员策略不存在。
@@ -148,14 +202,17 @@
 
 # 企业组织不存在。
 RESOURCENOTFOUND_ORGANIZATIONNOTEXIST = 'ResourceNotFound.OrganizationNotExist'
 
 # 集团服务不存在。
 RESOURCENOTFOUND_ORGANIZATIONSERVICENOTEXIST = 'ResourceNotFound.OrganizationServiceNotExist'
 
+# 用户不存在。
+RESOURCENOTFOUND_USERNOTEXIST = 'ResourceNotFound.UserNotExist'
+
 # 操作不支持。
 UNSUPPORTEDOPERATION = 'UnsupportedOperation'
 
 # 不允许添加代付关系。
 UNSUPPORTEDOPERATION_ADDDELEGATEPAYERNOTALLOW = 'UnsupportedOperation.AddDelegatePayerNotAllow'
 
 # 不允许添加优惠继承关系。
```

### Comparing `tencentcloud-sdk-python-organization-3.0.910/tencentcloud/organization/v20210331/models.py` & `tencentcloud-sdk-python-organization-3.0.911/tencentcloud/organization/v20210331/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,67 @@
 # limitations under the License.
 
 import warnings
 
 from tencentcloud.common.abstract_model import AbstractModel
 
 
+class AddOrganizationMemberEmailRequest(AbstractModel):
+    """AddOrganizationMemberEmail请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param MemberUin: 成员Uin
+        :type MemberUin: int
+        :param Email: 邮箱地址
+        :type Email: str
+        :param CountryCode: 国际区号
+        :type CountryCode: str
+        :param Phone: 手机号
+        :type Phone: str
+        """
+        self.MemberUin = None
+        self.Email = None
+        self.CountryCode = None
+        self.Phone = None
+
+
+    def _deserialize(self, params):
+        self.MemberUin = params.get("MemberUin")
+        self.Email = params.get("Email")
+        self.CountryCode = params.get("CountryCode")
+        self.Phone = params.get("Phone")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class AddOrganizationMemberEmailResponse(AbstractModel):
+    """AddOrganizationMemberEmail返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.RequestId = params.get("RequestId")
+
+
 class AddOrganizationNodeRequest(AbstractModel):
     """AddOrganizationNode请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -620,14 +673,100 @@
                 obj = OrgMemberAuthIdentity()
                 obj._deserialize(item)
                 self.Items.append(obj)
         self.Total = params.get("Total")
         self.RequestId = params.get("RequestId")
 
 
+class DescribeOrganizationMemberEmailBindRequest(AbstractModel):
+    """DescribeOrganizationMemberEmailBind请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param MemberUin: 成员Uin
+        :type MemberUin: int
+        """
+        self.MemberUin = None
+
+
+    def _deserialize(self, params):
+        self.MemberUin = params.get("MemberUin")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeOrganizationMemberEmailBindResponse(AbstractModel):
+    """DescribeOrganizationMemberEmailBind返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param BindId: 绑定ID
+注意：此字段可能返回 null，表示取不到有效值。
+        :type BindId: int
+        :param ApplyTime: 申请时间
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ApplyTime: str
+        :param Email: 邮箱地址
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Email: str
+        :param Phone: 手机号
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Phone: str
+        :param BindStatus: 绑定状态    未绑定：Unbound，待激活：Valid，绑定成功：Success，绑定失败：Failed
+注意：此字段可能返回 null，表示取不到有效值。
+        :type BindStatus: str
+        :param BindTime: 绑定时间
+注意：此字段可能返回 null，表示取不到有效值。
+        :type BindTime: str
+        :param Description: 失败说明
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Description: str
+        :param PhoneBind: 安全手机绑定状态  未绑定：0，已绑定：1
+注意：此字段可能返回 null，表示取不到有效值。
+        :type PhoneBind: int
+        :param CountryCode: 国际区号
+注意：此字段可能返回 null，表示取不到有效值。
+        :type CountryCode: str
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.BindId = None
+        self.ApplyTime = None
+        self.Email = None
+        self.Phone = None
+        self.BindStatus = None
+        self.BindTime = None
+        self.Description = None
+        self.PhoneBind = None
+        self.CountryCode = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.BindId = params.get("BindId")
+        self.ApplyTime = params.get("ApplyTime")
+        self.Email = params.get("Email")
+        self.Phone = params.get("Phone")
+        self.BindStatus = params.get("BindStatus")
+        self.BindTime = params.get("BindTime")
+        self.Description = params.get("Description")
+        self.PhoneBind = params.get("PhoneBind")
+        self.CountryCode = params.get("CountryCode")
+        self.RequestId = params.get("RequestId")
+
+
 class DescribeOrganizationMemberPoliciesRequest(AbstractModel):
     """DescribeOrganizationMemberPolicies请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -1585,14 +1724,71 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class UpdateOrganizationMemberEmailBindRequest(AbstractModel):
+    """UpdateOrganizationMemberEmailBind请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param MemberUin: 成员Uin
+        :type MemberUin: int
+        :param BindId: 绑定ID
+        :type BindId: int
+        :param Email: 邮箱
+        :type Email: str
+        :param CountryCode: 国际区号
+        :type CountryCode: str
+        :param Phone: 手机号
+        :type Phone: str
+        """
+        self.MemberUin = None
+        self.BindId = None
+        self.Email = None
+        self.CountryCode = None
+        self.Phone = None
+
+
+    def _deserialize(self, params):
+        self.MemberUin = params.get("MemberUin")
+        self.BindId = params.get("BindId")
+        self.Email = params.get("Email")
+        self.CountryCode = params.get("CountryCode")
+        self.Phone = params.get("Phone")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class UpdateOrganizationMemberEmailBindResponse(AbstractModel):
+    """UpdateOrganizationMemberEmailBind返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.RequestId = params.get("RequestId")
+
+
 class UpdateOrganizationNodeRequest(AbstractModel):
     """UpdateOrganizationNode请求参数结构体
 
     """
 
     def __init__(self):
         r"""
```

### Comparing `tencentcloud-sdk-python-organization-3.0.910/tencentcloud/organization/v20181225/organization_client.py` & `tencentcloud-sdk-python-organization-3.0.911/tencentcloud/organization/v20181225/organization_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-organization-3.0.910/tencentcloud/organization/v20181225/errorcodes.py` & `tencentcloud-sdk-python-organization-3.0.911/tencentcloud/organization/v20181225/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-organization-3.0.910/tencentcloud/organization/v20181225/models.py` & `tencentcloud-sdk-python-organization-3.0.911/tencentcloud/organization/v20181225/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-organization-3.0.910/tencentcloud/__init__.py` & `tencentcloud-sdk-python-organization-3.0.911/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.910'
+__version__ = '3.0.911'
```

### Comparing `tencentcloud-sdk-python-organization-3.0.910/tencentcloud_sdk_python_organization.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-organization-3.0.911/tencentcloud_sdk_python_organization.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-organization-3.0.910/tencentcloud_sdk_python_organization.egg-info/PKG-INFO` & `tencentcloud-sdk-python-organization-3.0.911/tencentcloud_sdk_python_organization.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-organization
-Version: 3.0.910
+Version: 3.0.911
 Summary: Tencent Cloud Organization SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-organization-3.0.910/PKG-INFO` & `tencentcloud-sdk-python-organization-3.0.911/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-organization
-Version: 3.0.910
+Version: 3.0.911
 Summary: Tencent Cloud Organization SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-organization-3.0.910/setup.py` & `tencentcloud-sdk-python-organization-3.0.911/setup.py`

 * *Files identical despite different names*

