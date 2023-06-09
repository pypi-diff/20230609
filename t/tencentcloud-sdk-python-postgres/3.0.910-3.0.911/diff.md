# Comparing `tmp/tencentcloud-sdk-python-postgres-3.0.910.tar.gz` & `tmp/tencentcloud-sdk-python-postgres-3.0.911.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-postgres-3.0.910.tar", last modified: Thu Jun  8 09:16:59 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-postgres-3.0.911.tar", last modified: Fri Jun  9 02:24:38 2023, max compression
```

## Comparing `tencentcloud-sdk-python-postgres-3.0.910.tar` & `tencentcloud-sdk-python-postgres-3.0.911.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 09:16:59.000000 tencentcloud-sdk-python-postgres-3.0.910/
--rw-r--r--   0 root         (0) root         (0)      752 2023-06-08 09:16:59.000000 tencentcloud-sdk-python-postgres-3.0.910/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 09:16:59.000000 tencentcloud-sdk-python-postgres-3.0.910/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 09:16:59.000000 tencentcloud-sdk-python-postgres-3.0.910/tencentcloud/postgres/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 09:16:59.000000 tencentcloud-sdk-python-postgres-3.0.910/tencentcloud/postgres/v20170312/
--rw-r--r--   0 root         (0) root         (0)    84591 2023-06-08 09:16:59.000000 tencentcloud-sdk-python-postgres-3.0.910/tencentcloud/postgres/v20170312/postgres_client.py
--rw-r--r--   0 root         (0) root         (0)    20657 2023-06-08 09:16:59.000000 tencentcloud-sdk-python-postgres-3.0.910/tencentcloud/postgres/v20170312/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 09:16:59.000000 tencentcloud-sdk-python-postgres-3.0.910/tencentcloud/postgres/v20170312/__init__.py
--rw-r--r--   0 root         (0) root         (0)   277276 2023-06-08 09:16:59.000000 tencentcloud-sdk-python-postgres-3.0.910/tencentcloud/postgres/v20170312/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 09:16:59.000000 tencentcloud-sdk-python-postgres-3.0.910/tencentcloud/postgres/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-08 09:16:59.000000 tencentcloud-sdk-python-postgres-3.0.910/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1684 2023-06-08 09:16:59.000000 tencentcloud-sdk-python-postgres-3.0.910/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1016 2023-06-08 09:16:59.000000 tencentcloud-sdk-python-postgres-3.0.910/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-08 09:16:59.000000 tencentcloud-sdk-python-postgres-3.0.910/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 09:16:59.000000 tencentcloud-sdk-python-postgres-3.0.910/tencentcloud_sdk_python_postgres.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 09:16:59.000000 tencentcloud-sdk-python-postgres-3.0.910/tencentcloud_sdk_python_postgres.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      495 2023-06-08 09:16:59.000000 tencentcloud-sdk-python-postgres-3.0.910/tencentcloud_sdk_python_postgres.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1684 2023-06-08 09:16:59.000000 tencentcloud-sdk-python-postgres-3.0.910/tencentcloud_sdk_python_postgres.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-08 09:16:59.000000 tencentcloud-sdk-python-postgres-3.0.910/tencentcloud_sdk_python_postgres.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:24:38.000000 tencentcloud-sdk-python-postgres-3.0.911/
+-rw-r--r--   0 root         (0) root         (0)      752 2023-06-09 02:24:38.000000 tencentcloud-sdk-python-postgres-3.0.911/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:24:38.000000 tencentcloud-sdk-python-postgres-3.0.911/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:24:38.000000 tencentcloud-sdk-python-postgres-3.0.911/tencentcloud/postgres/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:24:38.000000 tencentcloud-sdk-python-postgres-3.0.911/tencentcloud/postgres/v20170312/
+-rw-r--r--   0 root         (0) root         (0)    84591 2023-06-09 02:24:38.000000 tencentcloud-sdk-python-postgres-3.0.911/tencentcloud/postgres/v20170312/postgres_client.py
+-rw-r--r--   0 root         (0) root         (0)    20657 2023-06-09 02:24:38.000000 tencentcloud-sdk-python-postgres-3.0.911/tencentcloud/postgres/v20170312/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 02:24:38.000000 tencentcloud-sdk-python-postgres-3.0.911/tencentcloud/postgres/v20170312/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   277630 2023-06-09 02:24:38.000000 tencentcloud-sdk-python-postgres-3.0.911/tencentcloud/postgres/v20170312/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 02:24:38.000000 tencentcloud-sdk-python-postgres-3.0.911/tencentcloud/postgres/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-09 02:24:38.000000 tencentcloud-sdk-python-postgres-3.0.911/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-06-09 02:24:38.000000 tencentcloud-sdk-python-postgres-3.0.911/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1016 2023-06-09 02:24:38.000000 tencentcloud-sdk-python-postgres-3.0.911/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-09 02:24:38.000000 tencentcloud-sdk-python-postgres-3.0.911/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:24:38.000000 tencentcloud-sdk-python-postgres-3.0.911/tencentcloud_sdk_python_postgres.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 02:24:38.000000 tencentcloud-sdk-python-postgres-3.0.911/tencentcloud_sdk_python_postgres.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      495 2023-06-09 02:24:38.000000 tencentcloud-sdk-python-postgres-3.0.911/tencentcloud_sdk_python_postgres.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-06-09 02:24:38.000000 tencentcloud-sdk-python-postgres-3.0.911/tencentcloud_sdk_python_postgres.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-09 02:24:38.000000 tencentcloud-sdk-python-postgres-3.0.911/tencentcloud_sdk_python_postgres.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-postgres-3.0.910/README.rst` & `tencentcloud-sdk-python-postgres-3.0.911/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-postgres-3.0.910/tencentcloud/postgres/v20170312/postgres_client.py` & `tencentcloud-sdk-python-postgres-3.0.911/tencentcloud/postgres/v20170312/postgres_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-postgres-3.0.910/tencentcloud/postgres/v20170312/errorcodes.py` & `tencentcloud-sdk-python-postgres-3.0.911/tencentcloud/postgres/v20170312/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-postgres-3.0.910/tencentcloud/postgres/v20170312/models.py` & `tencentcloud-sdk-python-postgres-3.0.911/tencentcloud/postgres/v20170312/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -674,21 +674,25 @@
 class CreateBaseBackupResponse(AbstractModel):
     """CreateBaseBackup返回参数结构体
 
     """
 
     def __init__(self):
         r"""
+        :param BaseBackupId: 基础备份集ID
+        :type BaseBackupId: str
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
+        self.BaseBackupId = None
         self.RequestId = None
 
 
     def _deserialize(self, params):
+        self.BaseBackupId = params.get("BaseBackupId")
         self.RequestId = params.get("RequestId")
 
 
 class CreateDBInstanceNetworkAccessRequest(AbstractModel):
     """CreateDBInstanceNetworkAccess请求参数结构体
 
     """
@@ -1575,15 +1579,15 @@
         :type VpcId: str
         :param SubnetId: 子网ID
         :type SubnetId: str
         :param DBInstanceId: 实例ID
         :type DBInstanceId: str
         :param DBInstanceName: 实例名称
         :type DBInstanceName: str
-        :param DBInstanceStatus: 实例状态，分别为：applying（申请中）、init(待初始化)、initing(初始化中)、running(运行中)、limited run（受限运行）、isolated（已隔离）、recycling（回收中）、recycled（已回收）、job running（任务执行中）、offline（下线）、migrating（迁移中）、expanding（扩容中）、waitSwitch（等待切换）、switching（切换中）、readonly（只读）、restarting（重启中）、network changing（网络变更中）、upgrading（内核版本升级中）
+        :param DBInstanceStatus: 实例状态，分别为：applying（申请中）、init(待初始化)、initing(初始化中)、running(运行中)、limited run（受限运行）、isolating（隔离中）、isolated（已隔离）、recycling（回收中）、recycled（已回收）、job running（任务执行中）、offline（下线）、migrating（迁移中）、expanding（扩容中）、waitSwitch（等待切换）、switching（切换中）、readonly（只读）、restarting（重启中）、network changing（网络变更中）、upgrading（内核版本升级中）
         :type DBInstanceStatus: str
         :param DBInstanceMemory: 实例分配的内存大小，单位：GB
         :type DBInstanceMemory: int
         :param DBInstanceStorage: 实例分配的存储空间大小，单位：GB
         :type DBInstanceStorage: int
         :param DBInstanceCpu: 实例分配的CPU数量，单位：个
         :type DBInstanceCpu: int
@@ -2618,14 +2622,15 @@
         :type MinFinishTime: str
         :param MaxFinishTime: 备份的最大结束时间，形如2018-01-01 00:00:00。默认为当前时间。
         :type MaxFinishTime: str
         :param Filters: 按照一个或者多个过滤条件进行查询，目前支持的过滤条件有：
 db-instance-id：按照实例ID过滤，类型为string。
 db-instance-name：按照实例名过滤，类型为string。
 db-instance-ip：按照实例私有网络IP地址过滤，类型为string。
+base-backup-id：按照备份集ID过滤，类型为string。
         :type Filters: list of Filter
         :param Limit: 每页显示数量，取值范围为1-100，默认为返回10条。
         :type Limit: int
         :param Offset: 数据偏移量，从0开始。
         :type Offset: int
         :param OrderBy: 排序字段，支持StartTime,FinishTime,Size。
         :type OrderBy: str
@@ -3947,15 +3952,17 @@
 class DescribeReadOnlyGroupsRequest(AbstractModel):
     """DescribeReadOnlyGroups请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param Filters: 过滤条件，必须传入主实例ID进行过滤，否则返回值将为空，过滤参数为：db-master-instance-id
+        :param Filters: 按照一个或者多个过滤条件进行查询，目前支持的过滤条件有：
+db-master-instance-id：按照主实例过滤，类型为string。
+read-only-group-id：按照只读组ID过滤，类型为string。
         :type Filters: list of Filter
         :param PageSize: 查询每一页的条数，默认为10
         :type PageSize: int
         :param PageNumber: 查询的页码，默认为1
         :type PageNumber: int
         :param OrderBy: 查询排序依据，目前支持:ROGroupId,CreateTime,Name
         :type OrderBy: str
```

### Comparing `tencentcloud-sdk-python-postgres-3.0.910/tencentcloud/__init__.py` & `tencentcloud-sdk-python-postgres-3.0.911/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-postgres-3.0.910/PKG-INFO` & `tencentcloud-sdk-python-postgres-3.0.911/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-postgres
-Version: 3.0.910
+Version: 3.0.911
 Summary: Tencent Cloud Postgres SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-postgres-3.0.910/setup.py` & `tencentcloud-sdk-python-postgres-3.0.911/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-postgres-3.0.910/tencentcloud_sdk_python_postgres.egg-info/PKG-INFO` & `tencentcloud-sdk-python-postgres-3.0.911/tencentcloud_sdk_python_postgres.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-postgres
-Version: 3.0.910
+Version: 3.0.911
 Summary: Tencent Cloud Postgres SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

