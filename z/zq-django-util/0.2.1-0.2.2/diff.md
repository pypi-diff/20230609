# Comparing `tmp/zq_django_util-0.2.1.tar.gz` & `tmp/zq_django_util-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zq_django_util-0.2.1.tar", max compression
+gzip compressed data, was "zq_django_util-0.2.2.tar", max compression
```

## Comparing `zq_django_util-0.2.1.tar` & `zq_django_util-0.2.2.tar`

### file list

```diff
@@ -1,58 +1,58 @@
--rw-r--r--   0        0        0     1053 2023-01-03 07:14:08.000000 zq_django_util-0.2.1/LICENSE.txt
--rw-r--r--   0        0        0     2594 2023-04-24 10:18:11.062899 zq_django_util-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     1795 2023-01-05 11:13:17.000000 zq_django_util-0.2.1/README.md
--rw-r--r--   0        0        0       22 2023-04-24 10:18:20.114658 zq_django_util-0.2.1/zq_django_util/__init__.py
--rw-r--r--   0        0        0     4621 2023-01-03 04:57:09.000000 zq_django_util-0.2.1/zq_django_util/exceptions/__init__.py
--rw-r--r--   0        0        0     1174 2023-01-05 07:29:13.000000 zq_django_util-0.2.1/zq_django_util/exceptions/configs.py
--rw-r--r--   0        0        0     9768 2023-02-01 13:21:40.000000 zq_django_util-0.2.1/zq_django_util/exceptions/handler.py
--rw-r--r--   0        0        0      452 2023-01-03 11:19:36.000000 zq_django_util-0.2.1/zq_django_util/exceptions/types.py
--rw-r--r--   0        0        0      625 2022-12-30 11:23:04.000000 zq_django_util-0.2.1/zq_django_util/exceptions/views.py
--rw-r--r--   0        0        0        0 2022-12-31 01:27:21.000000 zq_django_util-0.2.1/zq_django_util/logs/__init__.py
--rw-r--r--   0        0        0     6853 2023-04-04 06:36:03.133338 zq_django_util-0.2.1/zq_django_util/logs/admin.py
--rw-r--r--   0        0        0      155 2023-01-03 04:57:09.000000 zq_django_util-0.2.1/zq_django_util/logs/apps.py
--rw-r--r--   0        0        0     1501 2023-01-03 11:19:34.000000 zq_django_util-0.2.1/zq_django_util/logs/configs.py
--rw-r--r--   0        0        0    12201 2023-04-04 06:36:03.133338 zq_django_util-0.2.1/zq_django_util/logs/handler.py
--rw-r--r--   0        0        0     1194 2023-02-27 09:46:45.960189 zq_django_util-0.2.1/zq_django_util/logs/middleware.py
--rw-r--r--   0        0        0     4149 2022-12-28 16:29:30.000000 zq_django_util-0.2.1/zq_django_util/logs/migrations/0001_initial.py
--rw-r--r--   0        0        0     1029 2023-03-01 11:37:01.499439 zq_django_util-0.2.1/zq_django_util/logs/migrations/0002_alter_requestlog_content_type_and_more.py
--rw-r--r--   0        0        0        0 2022-11-17 12:44:09.000000 zq_django_util-0.2.1/zq_django_util/logs/migrations/__init__.py
--rw-r--r--   0        0        0     2106 2023-03-01 11:27:41.423549 zq_django_util-0.2.1/zq_django_util/logs/models.py
--rw-r--r--   0        0        0      196 2022-09-25 14:36:30.000000 zq_django_util-0.2.1/zq_django_util/logs/templates/change_form.html
--rw-r--r--   0        0        0     2814 2022-12-28 06:05:44.000000 zq_django_util-0.2.1/zq_django_util/logs/templates/charts_change_list.html
--rw-r--r--   0        0        0      541 2023-01-03 04:57:09.000000 zq_django_util-0.2.1/zq_django_util/logs/threads.py
--rw-r--r--   0        0        0      959 2023-01-03 11:19:36.000000 zq_django_util-0.2.1/zq_django_util/logs/types.py
--rw-r--r--   0        0        0     2097 2023-04-04 06:36:03.134314 zq_django_util-0.2.1/zq_django_util/logs/utils.py
--rw-r--r--   0        0        0     5233 2023-04-04 06:36:03.134314 zq_django_util-0.2.1/zq_django_util/response/__init__.py
--rw-r--r--   0        0        0     1029 2022-12-30 12:20:33.000000 zq_django_util-0.2.1/zq_django_util/response/renderers.py
--rw-r--r--   0        0        0      477 2022-12-31 01:28:31.000000 zq_django_util-0.2.1/zq_django_util/response/types.py
--rw-r--r--   0        0        0        0 2022-12-28 16:05:03.000000 zq_django_util-0.2.1/zq_django_util/utils/__init__.py
--rw-r--r--   0        0        0        0 2022-12-28 16:02:14.000000 zq_django_util-0.2.1/zq_django_util/utils/auth/__init__.py
--rw-r--r--   0        0        0     2014 2023-01-03 11:19:36.000000 zq_django_util-0.2.1/zq_django_util/utils/auth/authentications.py
--rw-r--r--   0        0        0     2236 2023-04-04 06:36:03.135319 zq_django_util-0.2.1/zq_django_util/utils/auth/backends.py
--rw-r--r--   0        0        0      460 2023-01-03 04:57:20.000000 zq_django_util-0.2.1/zq_django_util/utils/auth/exceptions.py
--rw-r--r--   0        0        0     5701 2023-04-04 06:36:03.136663 zq_django_util-0.2.1/zq_django_util/utils/auth/serializers.py
--rw-r--r--   0        0        0     1554 2023-01-03 04:57:20.000000 zq_django_util-0.2.1/zq_django_util/utils/auth/views.py
--rw-r--r--   0        0        0      661 2023-04-04 06:36:14.359337 zq_django_util-0.2.1/zq_django_util/utils/meili/__init__.py
--rw-r--r--   0        0        0        0 2023-04-04 06:36:14.359337 zq_django_util-0.2.1/zq_django_util/utils/meili/constant/__init__.py
--rw-r--r--   0        0        0      234 2023-04-04 06:36:14.360314 zq_django_util-0.2.1/zq_django_util/utils/meili/constant/error.py
--rw-r--r--   0        0        0      990 2023-04-04 06:36:14.360314 zq_django_util-0.2.1/zq_django_util/utils/meili/constant/task.py
--rw-r--r--   0        0        0      360 2023-04-04 06:36:14.360314 zq_django_util-0.2.1/zq_django_util/utils/meili/error.py
--rw-r--r--   0        0        0      766 2023-04-04 06:36:14.361290 zq_django_util-0.2.1/zq_django_util/utils/meili/exceptions.py
--rw-r--r--   0        0        0    12436 2023-04-24 10:17:29.399863 zq_django_util-0.2.1/zq_django_util/utils/meili/index.py
--rw-r--r--   0        0        0      998 2023-04-04 06:36:14.361290 zq_django_util-0.2.1/zq_django_util/utils/meili/pagination.py
--rw-r--r--   0        0        0     1242 2023-04-04 06:36:14.362265 zq_django_util-0.2.1/zq_django_util/utils/meili/response.py
--rw-r--r--   0        0        0     2890 2023-04-04 06:36:14.362265 zq_django_util-0.2.1/zq_django_util/utils/meili/task.py
--rw-r--r--   0        0        0     1277 2023-01-03 04:57:31.000000 zq_django_util-0.2.1/zq_django_util/utils/mixins.py
--rw-r--r--   0        0        0        0 2022-12-28 16:05:17.000000 zq_django_util-0.2.1/zq_django_util/utils/oss/__init__.py
--rw-r--r--   0        0        0     9597 2023-03-01 11:44:33.348756 zq_django_util-0.2.1/zq_django_util/utils/oss/backends.py
--rw-r--r--   0        0        0     1032 2023-01-03 04:58:05.000000 zq_django_util-0.2.1/zq_django_util/utils/oss/configs.py
--rw-r--r--   0        0        0      100 2023-01-03 04:58:05.000000 zq_django_util-0.2.1/zq_django_util/utils/oss/exceptions.py
--rw-r--r--   0        0        0     5590 2023-01-03 11:19:36.000000 zq_django_util-0.2.1/zq_django_util/utils/oss/utils.py
--rw-r--r--   0        0        0     2878 2023-01-03 04:57:39.000000 zq_django_util-0.2.1/zq_django_util/utils/package_settings.py
--rw-r--r--   0        0        0      414 2023-01-05 05:43:33.000000 zq_django_util-0.2.1/zq_django_util/utils/pagination.py
--rw-r--r--   0        0        0      178 2022-12-29 16:45:07.000000 zq_django_util-0.2.1/zq_django_util/utils/types.py
--rw-r--r--   0        0        0        0 2022-12-28 16:19:39.000000 zq_django_util-0.2.1/zq_django_util/utils/user/__init__.py
--rw-r--r--   0        0        0     1622 2023-03-01 11:14:08.430418 zq_django_util-0.2.1/zq_django_util/utils/user/models.py
--rw-r--r--   0        0        0     1190 2023-03-01 11:55:07.417730 zq_django_util-0.2.1/zq_django_util/utils/views.py
--rw-r--r--   0        0        0     3006 1970-01-01 00:00:00.000000 zq_django_util-0.2.1/setup.py
--rw-r--r--   0        0        0     2736 1970-01-01 00:00:00.000000 zq_django_util-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1053 2023-01-03 07:14:08.000000 zq_django_util-0.2.2/LICENSE.txt
+-rw-r--r--   0        0        0     2594 2023-06-09 04:35:08.769309 zq_django_util-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     1795 2023-01-05 11:13:17.000000 zq_django_util-0.2.2/README.md
+-rw-r--r--   0        0        0       22 2023-06-09 04:35:17.056841 zq_django_util-0.2.2/zq_django_util/__init__.py
+-rw-r--r--   0        0        0     4621 2023-01-03 04:57:09.000000 zq_django_util-0.2.2/zq_django_util/exceptions/__init__.py
+-rw-r--r--   0        0        0     1174 2023-01-05 07:29:13.000000 zq_django_util-0.2.2/zq_django_util/exceptions/configs.py
+-rw-r--r--   0        0        0     9768 2023-02-01 13:21:40.000000 zq_django_util-0.2.2/zq_django_util/exceptions/handler.py
+-rw-r--r--   0        0        0      452 2023-01-03 11:19:36.000000 zq_django_util-0.2.2/zq_django_util/exceptions/types.py
+-rw-r--r--   0        0        0      625 2022-12-30 11:23:04.000000 zq_django_util-0.2.2/zq_django_util/exceptions/views.py
+-rw-r--r--   0        0        0        0 2022-12-31 01:27:21.000000 zq_django_util-0.2.2/zq_django_util/logs/__init__.py
+-rw-r--r--   0        0        0     6853 2023-04-04 06:36:03.133338 zq_django_util-0.2.2/zq_django_util/logs/admin.py
+-rw-r--r--   0        0        0      155 2023-01-03 04:57:09.000000 zq_django_util-0.2.2/zq_django_util/logs/apps.py
+-rw-r--r--   0        0        0     1501 2023-01-03 11:19:34.000000 zq_django_util-0.2.2/zq_django_util/logs/configs.py
+-rw-r--r--   0        0        0    12201 2023-04-04 06:36:03.133338 zq_django_util-0.2.2/zq_django_util/logs/handler.py
+-rw-r--r--   0        0        0     1194 2023-02-27 09:46:45.960189 zq_django_util-0.2.2/zq_django_util/logs/middleware.py
+-rw-r--r--   0        0        0     4149 2022-12-28 16:29:30.000000 zq_django_util-0.2.2/zq_django_util/logs/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1029 2023-03-01 11:37:01.499439 zq_django_util-0.2.2/zq_django_util/logs/migrations/0002_alter_requestlog_content_type_and_more.py
+-rw-r--r--   0        0        0        0 2022-11-17 12:44:09.000000 zq_django_util-0.2.2/zq_django_util/logs/migrations/__init__.py
+-rw-r--r--   0        0        0     2106 2023-03-01 11:27:41.423549 zq_django_util-0.2.2/zq_django_util/logs/models.py
+-rw-r--r--   0        0        0      196 2022-09-25 14:36:30.000000 zq_django_util-0.2.2/zq_django_util/logs/templates/change_form.html
+-rw-r--r--   0        0        0     2814 2022-12-28 06:05:44.000000 zq_django_util-0.2.2/zq_django_util/logs/templates/charts_change_list.html
+-rw-r--r--   0        0        0      541 2023-01-03 04:57:09.000000 zq_django_util-0.2.2/zq_django_util/logs/threads.py
+-rw-r--r--   0        0        0      959 2023-01-03 11:19:36.000000 zq_django_util-0.2.2/zq_django_util/logs/types.py
+-rw-r--r--   0        0        0     2097 2023-04-04 06:36:03.134314 zq_django_util-0.2.2/zq_django_util/logs/utils.py
+-rw-r--r--   0        0        0     5233 2023-04-04 06:36:03.134314 zq_django_util-0.2.2/zq_django_util/response/__init__.py
+-rw-r--r--   0        0        0     1029 2022-12-30 12:20:33.000000 zq_django_util-0.2.2/zq_django_util/response/renderers.py
+-rw-r--r--   0        0        0      477 2022-12-31 01:28:31.000000 zq_django_util-0.2.2/zq_django_util/response/types.py
+-rw-r--r--   0        0        0        0 2022-12-28 16:05:03.000000 zq_django_util-0.2.2/zq_django_util/utils/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-28 16:02:14.000000 zq_django_util-0.2.2/zq_django_util/utils/auth/__init__.py
+-rw-r--r--   0        0        0     2014 2023-01-03 11:19:36.000000 zq_django_util-0.2.2/zq_django_util/utils/auth/authentications.py
+-rw-r--r--   0        0        0     2236 2023-04-04 06:36:03.135319 zq_django_util-0.2.2/zq_django_util/utils/auth/backends.py
+-rw-r--r--   0        0        0      460 2023-01-03 04:57:20.000000 zq_django_util-0.2.2/zq_django_util/utils/auth/exceptions.py
+-rw-r--r--   0        0        0     5701 2023-04-04 06:36:03.136663 zq_django_util-0.2.2/zq_django_util/utils/auth/serializers.py
+-rw-r--r--   0        0        0     1554 2023-01-03 04:57:20.000000 zq_django_util-0.2.2/zq_django_util/utils/auth/views.py
+-rw-r--r--   0        0        0      661 2023-04-04 06:36:14.359337 zq_django_util-0.2.2/zq_django_util/utils/meili/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-04 06:36:14.359337 zq_django_util-0.2.2/zq_django_util/utils/meili/constant/__init__.py
+-rw-r--r--   0        0        0      234 2023-04-04 06:36:14.360314 zq_django_util-0.2.2/zq_django_util/utils/meili/constant/error.py
+-rw-r--r--   0        0        0      990 2023-04-04 06:36:14.360314 zq_django_util-0.2.2/zq_django_util/utils/meili/constant/task.py
+-rw-r--r--   0        0        0      360 2023-04-04 06:36:14.360314 zq_django_util-0.2.2/zq_django_util/utils/meili/error.py
+-rw-r--r--   0        0        0      766 2023-04-04 06:36:14.361290 zq_django_util-0.2.2/zq_django_util/utils/meili/exceptions.py
+-rw-r--r--   0        0        0    12378 2023-06-09 04:34:28.287759 zq_django_util-0.2.2/zq_django_util/utils/meili/index.py
+-rw-r--r--   0        0        0      998 2023-04-04 06:36:14.361290 zq_django_util-0.2.2/zq_django_util/utils/meili/pagination.py
+-rw-r--r--   0        0        0     1242 2023-04-04 06:36:14.362265 zq_django_util-0.2.2/zq_django_util/utils/meili/response.py
+-rw-r--r--   0        0        0     2890 2023-04-04 06:36:14.362265 zq_django_util-0.2.2/zq_django_util/utils/meili/task.py
+-rw-r--r--   0        0        0     1277 2023-01-03 04:57:31.000000 zq_django_util-0.2.2/zq_django_util/utils/mixins.py
+-rw-r--r--   0        0        0        0 2022-12-28 16:05:17.000000 zq_django_util-0.2.2/zq_django_util/utils/oss/__init__.py
+-rw-r--r--   0        0        0     9597 2023-03-01 11:44:33.348756 zq_django_util-0.2.2/zq_django_util/utils/oss/backends.py
+-rw-r--r--   0        0        0     1032 2023-01-03 04:58:05.000000 zq_django_util-0.2.2/zq_django_util/utils/oss/configs.py
+-rw-r--r--   0        0        0      100 2023-01-03 04:58:05.000000 zq_django_util-0.2.2/zq_django_util/utils/oss/exceptions.py
+-rw-r--r--   0        0        0     5590 2023-01-03 11:19:36.000000 zq_django_util-0.2.2/zq_django_util/utils/oss/utils.py
+-rw-r--r--   0        0        0     2878 2023-01-03 04:57:39.000000 zq_django_util-0.2.2/zq_django_util/utils/package_settings.py
+-rw-r--r--   0        0        0      414 2023-01-05 05:43:33.000000 zq_django_util-0.2.2/zq_django_util/utils/pagination.py
+-rw-r--r--   0        0        0      178 2022-12-29 16:45:07.000000 zq_django_util-0.2.2/zq_django_util/utils/types.py
+-rw-r--r--   0        0        0        0 2022-12-28 16:19:39.000000 zq_django_util-0.2.2/zq_django_util/utils/user/__init__.py
+-rw-r--r--   0        0        0     1622 2023-03-01 11:14:08.430418 zq_django_util-0.2.2/zq_django_util/utils/user/models.py
+-rw-r--r--   0        0        0     1190 2023-03-01 11:55:07.417730 zq_django_util-0.2.2/zq_django_util/utils/views.py
+-rw-r--r--   0        0        0     3006 1970-01-01 00:00:00.000000 zq_django_util-0.2.2/setup.py
+-rw-r--r--   0        0        0     2736 1970-01-01 00:00:00.000000 zq_django_util-0.2.2/PKG-INFO
```

### Comparing `zq_django_util-0.2.1/LICENSE.txt` & `zq_django_util-0.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zq_django_util-0.2.1/pyproject.toml` & `zq_django_util-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zq-django-util"
-version = "0.2.1"
+version = "0.2.2"
 description = "自强Studio Django 工具"
 authors = ["Nagico <yjr888@vip.qq.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/Nagico/zq-django-util"
 documentation = "https://zq-django-util.readthedocs.io/en/latest/"
 keywords = ["django", "drf", "util"]
```

### Comparing `zq_django_util-0.2.1/README.md` & `zq_django_util-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `zq_django_util-0.2.1/zq_django_util/exceptions/__init__.py` & `zq_django_util-0.2.2/zq_django_util/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `zq_django_util-0.2.1/zq_django_util/exceptions/configs.py` & `zq_django_util-0.2.2/zq_django_util/exceptions/configs.py`

 * *Files identical despite different names*

### Comparing `zq_django_util-0.2.1/zq_django_util/exceptions/handler.py` & `zq_django_util-0.2.2/zq_django_util/exceptions/handler.py`

 * *Files identical despite different names*

### Comparing `zq_django_util-0.2.1/zq_django_util/exceptions/views.py` & `zq_django_util-0.2.2/zq_django_util/exceptions/views.py`

 * *Files identical despite different names*

### Comparing `zq_django_util-0.2.1/zq_django_util/logs/admin.py` & `zq_django_util-0.2.2/zq_django_util/logs/admin.py`

 * *Files identical despite different names*

### Comparing `zq_django_util-0.2.1/zq_django_util/logs/configs.py` & `zq_django_util-0.2.2/zq_django_util/logs/configs.py`

 * *Files identical despite different names*

### Comparing `zq_django_util-0.2.1/zq_django_util/logs/handler.py` & `zq_django_util-0.2.2/zq_django_util/logs/handler.py`

 * *Files identical despite different names*

### Comparing `zq_django_util-0.2.1/zq_django_util/logs/middleware.py` & `zq_django_util-0.2.2/zq_django_util/logs/middleware.py`

 * *Files identical despite different names*

### Comparing `zq_django_util-0.2.1/zq_django_util/logs/migrations/0001_initial.py` & `zq_django_util-0.2.2/zq_django_util/logs/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `zq_django_util-0.2.1/zq_django_util/logs/migrations/0002_alter_requestlog_content_type_and_more.py` & `zq_django_util-0.2.2/zq_django_util/logs/migrations/0002_alter_requestlog_content_type_and_more.py`

 * *Files identical despite different names*

### Comparing `zq_django_util-0.2.1/zq_django_util/logs/models.py` & `zq_django_util-0.2.2/zq_django_util/logs/models.py`

 * *Files identical despite different names*

### Comparing `zq_django_util-0.2.1/zq_django_util/logs/templates/charts_change_list.html` & `zq_django_util-0.2.2/zq_django_util/logs/templates/charts_change_list.html`

 * *Files identical despite different names*

### Comparing `zq_django_util-0.2.1/zq_django_util/logs/threads.py` & `zq_django_util-0.2.2/zq_django_util/logs/threads.py`

 * *Files identical despite different names*

### Comparing `zq_django_util-0.2.1/zq_django_util/logs/types.py` & `zq_django_util-0.2.2/zq_django_util/logs/types.py`

 * *Files identical despite different names*

### Comparing `zq_django_util-0.2.1/zq_django_util/logs/utils.py` & `zq_django_util-0.2.2/zq_django_util/logs/utils.py`

 * *Files identical despite different names*

### Comparing `zq_django_util-0.2.1/zq_django_util/response/__init__.py` & `zq_django_util-0.2.2/zq_django_util/response/__init__.py`

 * *Files identical despite different names*

### Comparing `zq_django_util-0.2.1/zq_django_util/response/renderers.py` & `zq_django_util-0.2.2/zq_django_util/response/renderers.py`

 * *Files identical despite different names*

### Comparing `zq_django_util-0.2.1/zq_django_util/utils/auth/authentications.py` & `zq_django_util-0.2.2/zq_django_util/utils/auth/authentications.py`

 * *Files identical despite different names*

### Comparing `zq_django_util-0.2.1/zq_django_util/utils/auth/backends.py` & `zq_django_util-0.2.2/zq_django_util/utils/auth/backends.py`

 * *Files identical despite different names*

### Comparing `zq_django_util-0.2.1/zq_django_util/utils/auth/serializers.py` & `zq_django_util-0.2.2/zq_django_util/utils/auth/serializers.py`

 * *Files identical despite different names*

### Comparing `zq_django_util-0.2.1/zq_django_util/utils/auth/views.py` & `zq_django_util-0.2.2/zq_django_util/utils/auth/views.py`

 * *Files identical despite different names*

### Comparing `zq_django_util-0.2.1/zq_django_util/utils/meili/__init__.py` & `zq_django_util-0.2.2/zq_django_util/utils/meili/__init__.py`

 * *Files identical despite different names*

### Comparing `zq_django_util-0.2.1/zq_django_util/utils/meili/constant/task.py` & `zq_django_util-0.2.2/zq_django_util/utils/meili/constant/task.py`

 * *Files identical despite different names*

### Comparing `zq_django_util-0.2.1/zq_django_util/utils/meili/exceptions.py` & `zq_django_util-0.2.2/zq_django_util/utils/meili/exceptions.py`

 * *Files identical despite different names*

### Comparing `zq_django_util-0.2.1/zq_django_util/utils/meili/index.py` & `zq_django_util-0.2.2/zq_django_util/utils/meili/index.py`

 * *Files 1% similar despite different names*

```diff
@@ -253,17 +253,15 @@
         :param ignore_default_query_set: 忽略默认的query_set限制，默认为True
         :return:
         """
         objs = self._to_queryset(objs, ignore_default_query_set)
         if objs is None:
             return
 
-        self.index.delete_documents(
-            [obj.pk for obj in objs], primary_key=self.index.primary_key
-        )
+        self.index.delete_documents([obj.pk for obj in objs])
 
     def rebuild_index(self):
         """
         重建索引
 
         https://docs.meilisearch.com/reference/api/documents.html#delete-all-documents
```

### Comparing `zq_django_util-0.2.1/zq_django_util/utils/meili/pagination.py` & `zq_django_util-0.2.2/zq_django_util/utils/meili/pagination.py`

 * *Files identical despite different names*

### Comparing `zq_django_util-0.2.1/zq_django_util/utils/meili/response.py` & `zq_django_util-0.2.2/zq_django_util/utils/meili/response.py`

 * *Files identical despite different names*

### Comparing `zq_django_util-0.2.1/zq_django_util/utils/meili/task.py` & `zq_django_util-0.2.2/zq_django_util/utils/meili/task.py`

 * *Files identical despite different names*

### Comparing `zq_django_util-0.2.1/zq_django_util/utils/mixins.py` & `zq_django_util-0.2.2/zq_django_util/utils/mixins.py`

 * *Files identical despite different names*

### Comparing `zq_django_util-0.2.1/zq_django_util/utils/oss/backends.py` & `zq_django_util-0.2.2/zq_django_util/utils/oss/backends.py`

 * *Files identical despite different names*

### Comparing `zq_django_util-0.2.1/zq_django_util/utils/oss/configs.py` & `zq_django_util-0.2.2/zq_django_util/utils/oss/configs.py`

 * *Files identical despite different names*

### Comparing `zq_django_util-0.2.1/zq_django_util/utils/oss/utils.py` & `zq_django_util-0.2.2/zq_django_util/utils/oss/utils.py`

 * *Files identical despite different names*

### Comparing `zq_django_util-0.2.1/zq_django_util/utils/package_settings.py` & `zq_django_util-0.2.2/zq_django_util/utils/package_settings.py`

 * *Files identical despite different names*

### Comparing `zq_django_util-0.2.1/zq_django_util/utils/user/models.py` & `zq_django_util-0.2.2/zq_django_util/utils/user/models.py`

 * *Files identical despite different names*

### Comparing `zq_django_util-0.2.1/zq_django_util/utils/views.py` & `zq_django_util-0.2.2/zq_django_util/utils/views.py`

 * *Files identical despite different names*

### Comparing `zq_django_util-0.2.1/setup.py` & `zq_django_util-0.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
  'djangorestframework-simplejwt>=4.7,<6.0',
  'drf-standardized-errors>=0.9.0,<0.13.0',
  'isodate>=0.6.1,<0.7.0',
  'oss2>=2.13.0,<3.0']
 
 setup_kwargs = {
     'name': 'zq-django-util',
-    'version': '0.2.1',
+    'version': '0.2.2',
     'description': '自强Studio Django 工具',
     'long_description': '<div align="center">\n\n# zq-django-util\n**自强 Studio Django 工具**\n\n<!-- markdownlint-disable-next-line MD036 -->\n</div>\n\n<p align="center">\n  <a href="https://github.com/Nagico/zq-django-util/actions/workflows/code_check.yml">\n    <img src="https://github.com/Nagico/zq-django-util/actions/workflows/code_check.yml/badge.svg" alt="CI">\n  </a>\n  <a href="https://zq-django-util.readthedocs.io/en/latest/?badge=latest">\n    <img src="https://readthedocs.org/projects/zq-django-util/badge/?version=latest" alt="Documentation Status" />\n  </a>\n  <a href="https://codecov.io/gh/Nagico/zq-django-util" >\n    <img src="https://codecov.io/gh/Nagico/zq-django-util/branch/master/graph/badge.svg" alt="cov"/>\n  </a>\n  <a href="https://pypi.org/project/zq-django-util/">\n  <img src="https://img.shields.io/pypi/v/zq-django-util" alt="pypi">\n  </a>\n</p>\n<!-- markdownlint-enable MD033 -->\n\n[English Version](README_EN.md)\n\n## 简介\n\nzq-django-util 是用于辅助搭建 django-drf 应用的工具集合，其中包含：\n\n- 标准异常、响应处理\n- jwt、微信认证\n- oss 存储与直传\n- 默认分页类\n- 测试 ViewSet\n\n详细文档：[zq-django-util.readthedocs.io](https://zq-django-util.readthedocs.io/)\n\n## 依赖需求\n\n- Python 3.8+\n- Django 3.2+\n- Django REST framework 3.12+\n\n**强烈建议**使用官方支持的最新版本，当前的测试环境为：Python 3.10, Django 4.1, DRF 3.14\n\n## 安装\n\n- 安装 zq-django-util 包\n\n使用 `pip` 安装：\n```shell\npip install zq-django-util\n```\n\n使用 `poetry` 安装：\n```shell\npoetry add zq-django-util\n```\n\n## 使用\n\n可以根据以下说明进行配置，以启用相关功能。\n\n[使用文档](docs/usage)\n\n## 开发\n\n本项目使用 Poetry 进行依赖管理，Pytest 进行单元测试。\n\n[开发文档](docs/development)\n',
     'author': 'Nagico',
     'author_email': 'yjr888@vip.qq.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/Nagico/zq-django-util',
```

#### html2text {}

```diff
@@ -4,15 +4,15 @@
 'zq_django_util.utils', 'zq_django_util.utils.auth',
 'zq_django_util.utils.meili', 'zq_django_util.utils.meili.constant',
 'zq_django_util.utils.oss', 'zq_django_util.utils.user'] package_data = \ {'':
 ['*'], 'zq_django_util.logs': ['templates/*']} install_requires = \ ['django-
 cleanup>=6.0.0,<7.0.0', 'djangorestframework-simplejwt>=4.7,<6.0', 'drf-
 standardized-errors>=0.9.0,<0.13.0', 'isodate>=0.6.1,<0.7.0',
 'oss2>=2.13.0,<3.0'] setup_kwargs = { 'name': 'zq-django-util', 'version':
-'0.2.1', 'description': 'èªå¼ºStudio Django å·¥å·', 'long_description': '
+'0.2.2', 'description': 'èªå¼ºStudio Django å·¥å·', 'long_description': '
           \n\n# zq-django-util\n**èªå¼º Studio Django å·¥å·**\n\n\n
 \n\n
     \n \n_[CI]\n\n \n_[Documentation_Status]\n\n \n_[cov]\n\n \n_[pypi]\n\n
 \n\n\n[English Version](README_EN.md)\n\n## ç®ä»\n\nzq-django-util
 æ¯ç¨äºè¾å©æ­å»º django-drf åºç¨çå·¥å·éåï¼å¶ä¸­åå«ï¼\n\n-
 æ åå¼å¸¸ãååºå¤ç\n- jwtãå¾®ä¿¡è®¤è¯\n- oss å­å¨ä¸ç´ä¼ \n-
 é»è®¤åé¡µç±»\n- æµè¯ ViewSet\n\nè¯¦ç»ææ¡£ï¼[zq-django-
```

### Comparing `zq_django_util-0.2.1/PKG-INFO` & `zq_django_util-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zq-django-util
-Version: 0.2.1
+Version: 0.2.2
 Summary: 自强Studio Django 工具
 Home-page: https://github.com/Nagico/zq-django-util
 License: MIT
 Keywords: django,drf,util
 Author: Nagico
 Author-email: yjr888@vip.qq.com
 Requires-Python: >=3.8,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: zq-django-util Version: 0.2.1 Summary: èªå¼ºStudio
+Metadata-Version: 2.1 Name: zq-django-util Version: 0.2.2 Summary: èªå¼ºStudio
 Django å·¥å· Home-page: https://github.com/Nagico/zq-django-util License: MIT
 Keywords: django,drf,util Author: Nagico Author-email: yjr888@vip.qq.com
 Requires-Python: >=3.8,<4.0 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Provides-Extra: sentry Requires-Dist: django-cleanup
```

