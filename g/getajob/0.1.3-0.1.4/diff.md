# Comparing `tmp/getajob-0.1.3.tar.gz` & `tmp/getajob-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "getajob-0.1.3.tar", max compression
+gzip compressed data, was "getajob-0.1.4.tar", max compression
```

## Comparing `getajob-0.1.3.tar` & `getajob-0.1.4.tar`

### file list

```diff
@@ -1,57 +1,57 @@
--rw-r--r--   0        0        0       69 2023-06-09 12:51:50.666069 getajob-0.1.3/README.md
--rw-r--r--   0        0        0        0 2023-06-09 12:51:50.666069 getajob-0.1.3/getajob/__init__.py
--rw-r--r--   0        0        0     1013 2023-06-09 12:51:50.666069 getajob-0.1.3/getajob/abstractions/models.py
--rw-r--r--   0        0        0     6850 2023-06-09 12:51:50.666069 getajob-0.1.3/getajob/abstractions/repository.py
--rw-r--r--   0        0        0     3138 2023-06-09 12:51:50.666069 getajob-0.1.3/getajob/auth.py
--rw-r--r--   0        0        0     2630 2023-06-09 12:51:50.666069 getajob-0.1.3/getajob/config/settings.py
--rw-r--r--   0        0        0        0 2023-06-09 12:51:50.666069 getajob-0.1.3/getajob/contexts/__init__.py
--rw-r--r--   0        0        0      170 2023-06-09 12:51:50.666069 getajob-0.1.3/getajob/contexts/admin/search/models.py
--rw-r--r--   0        0        0      574 2023-06-09 12:51:50.666069 getajob-0.1.3/getajob/contexts/admin/search/repository.py
--rw-r--r--   0        0        0      737 2023-06-09 12:51:50.666069 getajob-0.1.3/getajob/contexts/admin/users/models.py
--rw-r--r--   0        0        0      447 2023-06-09 12:51:50.666069 getajob-0.1.3/getajob/contexts/admin/users/repository.py
--rw-r--r--   0        0        0      823 2023-06-09 12:51:50.666069 getajob-0.1.3/getajob/contexts/ai/text/models.py
--rw-r--r--   0        0        0     2470 2023-06-09 12:51:50.666069 getajob-0.1.3/getajob/contexts/ai/text/repository.py
--rw-r--r--   0        0        0     1530 2023-06-09 12:51:50.666069 getajob-0.1.3/getajob/contexts/applications/models.py
--rw-r--r--   0        0        0     4340 2023-06-09 12:51:50.666069 getajob-0.1.3/getajob/contexts/applications/repository.py
--rw-r--r--   0        0        0     5814 2023-06-09 12:51:50.666069 getajob-0.1.3/getajob/contexts/applications/unit_of_work.py
--rw-r--r--   0        0        0     1140 2023-06-09 12:51:50.666069 getajob-0.1.3/getajob/contexts/companies/models.py
--rw-r--r--   0        0        0     1084 2023-06-09 12:51:50.666069 getajob-0.1.3/getajob/contexts/companies/repository.py
--rw-r--r--   0        0        0     1416 2023-06-09 12:51:50.666069 getajob-0.1.3/getajob/contexts/companies/unit_of_work.py
--rw-r--r--   0        0        0     3135 2023-06-09 12:51:50.666069 getajob-0.1.3/getajob/contexts/jobs/models.py
--rw-r--r--   0        0        0     1040 2023-06-09 12:51:50.666069 getajob-0.1.3/getajob/contexts/jobs/repository.py
--rw-r--r--   0        0        0      462 2023-06-09 12:51:50.666069 getajob-0.1.3/getajob/contexts/jobs/unit_of_work.py
--rw-r--r--   0        0        0      799 2023-06-09 12:51:50.666069 getajob-0.1.3/getajob/contexts/notifications/models.py
--rw-r--r--   0        0        0      537 2023-06-09 12:51:50.666069 getajob-0.1.3/getajob/contexts/notifications/repository.py
--rw-r--r--   0        0        0      761 2023-06-09 12:51:50.666069 getajob-0.1.3/getajob/contexts/recruiters/models.py
--rw-r--r--   0        0        0      446 2023-06-09 12:51:50.666069 getajob-0.1.3/getajob/contexts/recruiters/repository.py
--rw-r--r--   0        0        0     1332 2023-06-09 12:51:50.666069 getajob-0.1.3/getajob/contexts/static/repository.py
--rw-r--r--   0        0        0     1123 2023-06-09 12:51:50.666069 getajob-0.1.3/getajob/contexts/users/clerk_webhook/models.py
--rw-r--r--   0        0        0      843 2023-06-09 12:51:50.666069 getajob-0.1.3/getajob/contexts/users/clerk_webhook/repository.py
--rw-r--r--   0        0        0      409 2023-06-09 12:51:50.666069 getajob-0.1.3/getajob/contexts/users/cover_letters/models.py
--rw-r--r--   0        0        0      345 2023-06-09 12:51:50.666069 getajob-0.1.3/getajob/contexts/users/cover_letters/repository.py
--rw-r--r--   0        0        0      313 2023-06-09 12:51:50.666069 getajob-0.1.3/getajob/contexts/users/resumes/models.py
--rw-r--r--   0        0        0      334 2023-06-09 12:51:50.666069 getajob-0.1.3/getajob/contexts/users/resumes/repository.py
--rw-r--r--   0        0        0      306 2023-06-09 12:51:50.666069 getajob-0.1.3/getajob/contexts/users/sessions/models.py
--rw-r--r--   0        0        0      523 2023-06-09 12:51:50.666069 getajob-0.1.3/getajob/contexts/users/skills/models.py
--rw-r--r--   0        0        0      337 2023-06-09 12:51:50.666069 getajob-0.1.3/getajob/contexts/users/skills/repository.py
--rw-r--r--   0        0        0      726 2023-06-09 12:51:50.666069 getajob-0.1.3/getajob/contexts/users/users/models.py
--rw-r--r--   0        0        0      715 2023-06-09 12:51:50.666069 getajob-0.1.3/getajob/contexts/users/users/repository.py
--rw-r--r--   0        0        0     1794 2023-06-09 12:51:50.666069 getajob-0.1.3/getajob/exceptions.py
--rw-r--r--   0        0        0        0 2023-06-09 12:51:50.666069 getajob-0.1.3/getajob/models/__init__.py
--rw-r--r--   0        0        0      373 2023-06-09 12:51:50.666069 getajob-0.1.3/getajob/models/entities.py
--rw-r--r--   0        0        0      240 2023-06-09 12:51:50.666069 getajob-0.1.3/getajob/models/location.py
--rw-r--r--   0        0        0      375 2023-06-09 12:51:50.666069 getajob-0.1.3/getajob/utils.py
--rw-r--r--   0        0        0     2527 2023-06-09 12:51:50.670069 getajob-0.1.3/getajob/vendor/algolia.py
--rw-r--r--   0        0        0     4456 2023-06-09 12:51:50.670069 getajob-0.1.3/getajob/vendor/clerk.py
--rw-r--r--   0        0        0    11012 2023-06-09 12:51:50.670069 getajob-0.1.3/getajob/vendor/firebase.py
--rw-r--r--   0        0        0      709 2023-06-09 12:51:50.670069 getajob-0.1.3/getajob/vendor/kafka/authentication.py
--rw-r--r--   0        0        0      320 2023-06-09 12:51:50.670069 getajob-0.1.3/getajob/vendor/kafka/exceptions.py
--rw-r--r--   0        0        0     1303 2023-06-09 12:51:50.670069 getajob-0.1.3/getajob/vendor/kafka/kafka.py
--rw-r--r--   0        0        0      179 2023-06-09 12:51:50.670069 getajob-0.1.3/getajob/vendor/kafka/mock.py
--rw-r--r--   0        0        0     1625 2023-06-09 12:51:50.670069 getajob-0.1.3/getajob/vendor/kafka/models.py
--rw-r--r--   0        0        0      585 2023-06-09 12:51:50.670069 getajob-0.1.3/getajob/vendor/kafka/repository.py
--rw-r--r--   0        0        0     1998 2023-06-09 12:51:50.670069 getajob-0.1.3/getajob/vendor/openai.py
--rw-r--r--   0        0        0      599 2023-06-09 12:51:50.670069 getajob-0.1.3/getajob/vendor/sendgrid/sendgrid.py
--rw-r--r--   0        0        0      207 2023-06-09 12:51:50.670069 getajob-0.1.3/getajob/vendor/sentry.py
--rw-r--r--   0        0        0     1724 2023-06-09 12:51:50.670069 getajob-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2869 1970-01-01 00:00:00.000000 getajob-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       69 2023-06-09 13:12:34.659844 getajob-0.1.4/README.md
+-rw-r--r--   0        0        0        0 2023-06-09 13:12:34.659844 getajob-0.1.4/getajob/__init__.py
+-rw-r--r--   0        0        0     1013 2023-06-09 13:12:34.659844 getajob-0.1.4/getajob/abstractions/models.py
+-rw-r--r--   0        0        0     6850 2023-06-09 13:12:34.659844 getajob-0.1.4/getajob/abstractions/repository.py
+-rw-r--r--   0        0        0     3138 2023-06-09 13:12:34.659844 getajob-0.1.4/getajob/auth.py
+-rw-r--r--   0        0        0     1341 2023-06-09 13:12:34.659844 getajob-0.1.4/getajob/config/settings.py
+-rw-r--r--   0        0        0        0 2023-06-09 13:12:34.659844 getajob-0.1.4/getajob/contexts/__init__.py
+-rw-r--r--   0        0        0      170 2023-06-09 13:12:34.659844 getajob-0.1.4/getajob/contexts/admin/search/models.py
+-rw-r--r--   0        0        0      574 2023-06-09 13:12:34.659844 getajob-0.1.4/getajob/contexts/admin/search/repository.py
+-rw-r--r--   0        0        0      737 2023-06-09 13:12:34.659844 getajob-0.1.4/getajob/contexts/admin/users/models.py
+-rw-r--r--   0        0        0      447 2023-06-09 13:12:34.659844 getajob-0.1.4/getajob/contexts/admin/users/repository.py
+-rw-r--r--   0        0        0      823 2023-06-09 13:12:34.659844 getajob-0.1.4/getajob/contexts/ai/text/models.py
+-rw-r--r--   0        0        0     2470 2023-06-09 13:12:34.659844 getajob-0.1.4/getajob/contexts/ai/text/repository.py
+-rw-r--r--   0        0        0     1530 2023-06-09 13:12:34.659844 getajob-0.1.4/getajob/contexts/applications/models.py
+-rw-r--r--   0        0        0     4340 2023-06-09 13:12:34.659844 getajob-0.1.4/getajob/contexts/applications/repository.py
+-rw-r--r--   0        0        0     5814 2023-06-09 13:12:34.659844 getajob-0.1.4/getajob/contexts/applications/unit_of_work.py
+-rw-r--r--   0        0        0     1140 2023-06-09 13:12:34.663845 getajob-0.1.4/getajob/contexts/companies/models.py
+-rw-r--r--   0        0        0     1084 2023-06-09 13:12:34.663845 getajob-0.1.4/getajob/contexts/companies/repository.py
+-rw-r--r--   0        0        0     1416 2023-06-09 13:12:34.663845 getajob-0.1.4/getajob/contexts/companies/unit_of_work.py
+-rw-r--r--   0        0        0     3135 2023-06-09 13:12:34.663845 getajob-0.1.4/getajob/contexts/jobs/models.py
+-rw-r--r--   0        0        0     1040 2023-06-09 13:12:34.663845 getajob-0.1.4/getajob/contexts/jobs/repository.py
+-rw-r--r--   0        0        0      462 2023-06-09 13:12:34.663845 getajob-0.1.4/getajob/contexts/jobs/unit_of_work.py
+-rw-r--r--   0        0        0      799 2023-06-09 13:12:34.663845 getajob-0.1.4/getajob/contexts/notifications/models.py
+-rw-r--r--   0        0        0      537 2023-06-09 13:12:34.663845 getajob-0.1.4/getajob/contexts/notifications/repository.py
+-rw-r--r--   0        0        0      761 2023-06-09 13:12:34.663845 getajob-0.1.4/getajob/contexts/recruiters/models.py
+-rw-r--r--   0        0        0      446 2023-06-09 13:12:34.663845 getajob-0.1.4/getajob/contexts/recruiters/repository.py
+-rw-r--r--   0        0        0     1332 2023-06-09 13:12:34.663845 getajob-0.1.4/getajob/contexts/static/repository.py
+-rw-r--r--   0        0        0     1123 2023-06-09 13:12:34.663845 getajob-0.1.4/getajob/contexts/users/clerk_webhook/models.py
+-rw-r--r--   0        0        0      843 2023-06-09 13:12:34.663845 getajob-0.1.4/getajob/contexts/users/clerk_webhook/repository.py
+-rw-r--r--   0        0        0      409 2023-06-09 13:12:34.663845 getajob-0.1.4/getajob/contexts/users/cover_letters/models.py
+-rw-r--r--   0        0        0      345 2023-06-09 13:12:34.663845 getajob-0.1.4/getajob/contexts/users/cover_letters/repository.py
+-rw-r--r--   0        0        0      313 2023-06-09 13:12:34.663845 getajob-0.1.4/getajob/contexts/users/resumes/models.py
+-rw-r--r--   0        0        0      334 2023-06-09 13:12:34.663845 getajob-0.1.4/getajob/contexts/users/resumes/repository.py
+-rw-r--r--   0        0        0      306 2023-06-09 13:12:34.663845 getajob-0.1.4/getajob/contexts/users/sessions/models.py
+-rw-r--r--   0        0        0      523 2023-06-09 13:12:34.663845 getajob-0.1.4/getajob/contexts/users/skills/models.py
+-rw-r--r--   0        0        0      337 2023-06-09 13:12:34.663845 getajob-0.1.4/getajob/contexts/users/skills/repository.py
+-rw-r--r--   0        0        0      726 2023-06-09 13:12:34.663845 getajob-0.1.4/getajob/contexts/users/users/models.py
+-rw-r--r--   0        0        0      715 2023-06-09 13:12:34.663845 getajob-0.1.4/getajob/contexts/users/users/repository.py
+-rw-r--r--   0        0        0     1794 2023-06-09 13:12:34.663845 getajob-0.1.4/getajob/exceptions.py
+-rw-r--r--   0        0        0        0 2023-06-09 13:12:34.663845 getajob-0.1.4/getajob/models/__init__.py
+-rw-r--r--   0        0        0      373 2023-06-09 13:12:34.663845 getajob-0.1.4/getajob/models/entities.py
+-rw-r--r--   0        0        0      240 2023-06-09 13:12:34.663845 getajob-0.1.4/getajob/models/location.py
+-rw-r--r--   0        0        0      375 2023-06-09 13:12:34.663845 getajob-0.1.4/getajob/utils.py
+-rw-r--r--   0        0        0     2527 2023-06-09 13:12:34.663845 getajob-0.1.4/getajob/vendor/algolia.py
+-rw-r--r--   0        0        0     4456 2023-06-09 13:12:34.663845 getajob-0.1.4/getajob/vendor/clerk.py
+-rw-r--r--   0        0        0    10429 2023-06-09 13:12:34.663845 getajob-0.1.4/getajob/vendor/firebase.py
+-rw-r--r--   0        0        0      709 2023-06-09 13:12:34.663845 getajob-0.1.4/getajob/vendor/kafka/authentication.py
+-rw-r--r--   0        0        0      320 2023-06-09 13:12:34.663845 getajob-0.1.4/getajob/vendor/kafka/exceptions.py
+-rw-r--r--   0        0        0     1303 2023-06-09 13:12:34.663845 getajob-0.1.4/getajob/vendor/kafka/kafka.py
+-rw-r--r--   0        0        0      179 2023-06-09 13:12:34.663845 getajob-0.1.4/getajob/vendor/kafka/mock.py
+-rw-r--r--   0        0        0     1625 2023-06-09 13:12:34.663845 getajob-0.1.4/getajob/vendor/kafka/models.py
+-rw-r--r--   0        0        0      585 2023-06-09 13:12:34.663845 getajob-0.1.4/getajob/vendor/kafka/repository.py
+-rw-r--r--   0        0        0     1998 2023-06-09 13:12:34.663845 getajob-0.1.4/getajob/vendor/openai.py
+-rw-r--r--   0        0        0      599 2023-06-09 13:12:34.663845 getajob-0.1.4/getajob/vendor/sendgrid/sendgrid.py
+-rw-r--r--   0        0        0      207 2023-06-09 13:12:34.663845 getajob-0.1.4/getajob/vendor/sentry.py
+-rw-r--r--   0        0        0     1725 2023-06-09 13:12:34.663845 getajob-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2769 1970-01-01 00:00:00.000000 getajob-0.1.4/PKG-INFO
```

### Comparing `getajob-0.1.3/getajob/abstractions/models.py` & `getajob-0.1.4/getajob/abstractions/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.1.3/getajob/abstractions/repository.py` & `getajob-0.1.4/getajob/abstractions/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.1.3/getajob/auth.py` & `getajob-0.1.4/getajob/auth.py`

 * *Files identical despite different names*

### Comparing `getajob-0.1.3/getajob/contexts/admin/search/repository.py` & `getajob-0.1.4/getajob/contexts/admin/search/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.1.3/getajob/contexts/admin/users/models.py` & `getajob-0.1.4/getajob/contexts/admin/users/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.1.3/getajob/contexts/ai/text/models.py` & `getajob-0.1.4/getajob/contexts/ai/text/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.1.3/getajob/contexts/ai/text/repository.py` & `getajob-0.1.4/getajob/contexts/ai/text/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.1.3/getajob/contexts/applications/models.py` & `getajob-0.1.4/getajob/contexts/applications/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.1.3/getajob/contexts/applications/repository.py` & `getajob-0.1.4/getajob/contexts/applications/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.1.3/getajob/contexts/applications/unit_of_work.py` & `getajob-0.1.4/getajob/contexts/applications/unit_of_work.py`

 * *Files identical despite different names*

### Comparing `getajob-0.1.3/getajob/contexts/companies/models.py` & `getajob-0.1.4/getajob/contexts/companies/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.1.3/getajob/contexts/companies/repository.py` & `getajob-0.1.4/getajob/contexts/companies/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.1.3/getajob/contexts/companies/unit_of_work.py` & `getajob-0.1.4/getajob/contexts/companies/unit_of_work.py`

 * *Files identical despite different names*

### Comparing `getajob-0.1.3/getajob/contexts/jobs/models.py` & `getajob-0.1.4/getajob/contexts/jobs/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.1.3/getajob/contexts/jobs/repository.py` & `getajob-0.1.4/getajob/contexts/jobs/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.1.3/getajob/contexts/notifications/models.py` & `getajob-0.1.4/getajob/contexts/notifications/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.1.3/getajob/contexts/notifications/repository.py` & `getajob-0.1.4/getajob/contexts/notifications/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.1.3/getajob/contexts/recruiters/models.py` & `getajob-0.1.4/getajob/contexts/recruiters/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.1.3/getajob/contexts/static/repository.py` & `getajob-0.1.4/getajob/contexts/static/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.1.3/getajob/contexts/users/clerk_webhook/models.py` & `getajob-0.1.4/getajob/contexts/users/clerk_webhook/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.1.3/getajob/contexts/users/clerk_webhook/repository.py` & `getajob-0.1.4/getajob/contexts/users/clerk_webhook/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.1.3/getajob/contexts/users/skills/models.py` & `getajob-0.1.4/getajob/contexts/users/skills/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.1.3/getajob/contexts/users/users/models.py` & `getajob-0.1.4/getajob/contexts/users/users/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.1.3/getajob/contexts/users/users/repository.py` & `getajob-0.1.4/getajob/contexts/users/users/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.1.3/getajob/exceptions.py` & `getajob-0.1.4/getajob/exceptions.py`

 * *Files identical despite different names*

### Comparing `getajob-0.1.3/getajob/vendor/algolia.py` & `getajob-0.1.4/getajob/vendor/algolia.py`

 * *Files identical despite different names*

### Comparing `getajob-0.1.3/getajob/vendor/clerk.py` & `getajob-0.1.4/getajob/vendor/clerk.py`

 * *Files identical despite different names*

### Comparing `getajob-0.1.3/getajob/vendor/firebase.py` & `getajob-0.1.4/getajob/vendor/firebase.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import typing as t
+import json
 
 from pydantic import BaseModel
 import firebase_admin
 from firebase_admin import credentials, firestore
 from google.cloud.firestore_v1.client import Client
 from google.cloud.firestore_v1.base_query import BaseQuery
 
@@ -79,28 +80,15 @@
             )
         )
         parent_dict[key] = input_dict[key]
     return output_list
 
 
 def get_client():
-    cred = credentials.Certificate(
-        {
-            "type": "service_account",
-            "project_id": SETTINGS.FIRESTORE_PROJECT_ID,
-            "private_key_id": SETTINGS.FIRESTORE_PRIVATE_KEY_ID,
-            "private_key": SETTINGS.FIRESTORE_PRIVATE_KEY,
-            "client_email": SETTINGS.FIRESTORE_CLIENT_EMAIL,
-            "client_id": SETTINGS.FIRESTORE_CLIENT_ID,
-            "auth_uri": SETTINGS.FIRESTORE_AUTH_URI,
-            "token_uri": SETTINGS.FIRESTORE_TOKEN_URI,
-            "auth_provider_x509_cert_url": SETTINGS.FIRESTORE_AUTH_PROVIDER_X509_CERT_URL,
-            "client_x509_cert_url": SETTINGS.FIRESTORE_CLIENT_X509_CERT_URL,
-        }
-    )
+    cred = credentials.Certificate(json.loads(SETTINGS.FIRESTORE_JSON_CONFIG))
     firebase_admin.initialize_app(cred)
     return firestore.client()
 
 
 def add_filters_to_query(query_reference: BaseQuery, filters: t.List[FirestoreFilters]):
     for _filter in filters:
         if _filter.operator == "like":
```

### Comparing `getajob-0.1.3/getajob/vendor/kafka/authentication.py` & `getajob-0.1.4/getajob/vendor/kafka/authentication.py`

 * *Files identical despite different names*

### Comparing `getajob-0.1.3/getajob/vendor/kafka/kafka.py` & `getajob-0.1.4/getajob/vendor/kafka/kafka.py`

 * *Files identical despite different names*

### Comparing `getajob-0.1.3/getajob/vendor/kafka/models.py` & `getajob-0.1.4/getajob/vendor/kafka/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.1.3/getajob/vendor/kafka/repository.py` & `getajob-0.1.4/getajob/vendor/kafka/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.1.3/getajob/vendor/openai.py` & `getajob-0.1.4/getajob/vendor/openai.py`

 * *Files identical despite different names*

### Comparing `getajob-0.1.3/getajob/vendor/sendgrid/sendgrid.py` & `getajob-0.1.4/getajob/vendor/sendgrid/sendgrid.py`

 * *Files identical despite different names*

### Comparing `getajob-0.1.3/pyproject.toml` & `getajob-0.1.4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [tool.poetry]
 name = "getajob"
-version = "0.1.3"
+version = "0.1.4"
 description = ""
 authors = ["Your Name <you@example.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "^3.9"
+python = "^3.11"
 aiohttp = "3.8.4"
 aiosignal = "1.3.1"
 algoliasearch = "3.0.0"
 anyio = "3.7.0"
 async-timeout = "4.0.2"
 attrs = "23.1.0"
 cachecontrol = "0.12.11"
```

### Comparing `getajob-0.1.3/PKG-INFO` & `getajob-0.1.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: getajob
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
 Author: Your Name
 Author-email: you@example.com
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (==3.8.4)
 Requires-Dist: aiosignal (==1.3.1)
 Requires-Dist: algoliasearch (==3.0.0)
 Requires-Dist: anyio (==3.7.0)
 Requires-Dist: async-timeout (==4.0.2)
 Requires-Dist: attrs (==23.1.0)
```

