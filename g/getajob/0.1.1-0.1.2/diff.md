# Comparing `tmp/getajob-0.1.1.tar.gz` & `tmp/getajob-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "getajob-0.1.1.tar", max compression
+gzip compressed data, was "getajob-0.1.2.tar", max compression
```

## Comparing `getajob-0.1.1.tar` & `getajob-0.1.2.tar`

### file list

```diff
@@ -1,57 +1,57 @@
--rw-r--r--   0        0        0       69 2023-06-08 22:00:37.629907 getajob-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-06-08 22:00:37.629907 getajob-0.1.1/getajob/__init__.py
--rw-r--r--   0        0        0     1013 2023-06-08 22:00:37.629907 getajob-0.1.1/getajob/abstractions/models.py
--rw-r--r--   0        0        0     6850 2023-06-08 22:00:37.629907 getajob-0.1.1/getajob/abstractions/repository.py
--rw-r--r--   0        0        0     3138 2023-06-08 22:00:37.629907 getajob-0.1.1/getajob/auth.py
--rw-r--r--   0        0        0     1635 2023-06-08 22:00:37.629907 getajob-0.1.1/getajob/config/settings.py
--rw-r--r--   0        0        0        0 2023-06-08 22:00:37.629907 getajob-0.1.1/getajob/contexts/__init__.py
--rw-r--r--   0        0        0      170 2023-06-08 22:00:37.629907 getajob-0.1.1/getajob/contexts/admin/search/models.py
--rw-r--r--   0        0        0      574 2023-06-08 22:00:37.629907 getajob-0.1.1/getajob/contexts/admin/search/repository.py
--rw-r--r--   0        0        0      737 2023-06-08 22:00:37.629907 getajob-0.1.1/getajob/contexts/admin/users/models.py
--rw-r--r--   0        0        0      447 2023-06-08 22:00:37.629907 getajob-0.1.1/getajob/contexts/admin/users/repository.py
--rw-r--r--   0        0        0      823 2023-06-08 22:00:37.629907 getajob-0.1.1/getajob/contexts/ai/text/models.py
--rw-r--r--   0        0        0     2470 2023-06-08 22:00:37.629907 getajob-0.1.1/getajob/contexts/ai/text/repository.py
--rw-r--r--   0        0        0     1530 2023-06-08 22:00:37.629907 getajob-0.1.1/getajob/contexts/applications/models.py
--rw-r--r--   0        0        0     4340 2023-06-08 22:00:37.629907 getajob-0.1.1/getajob/contexts/applications/repository.py
--rw-r--r--   0        0        0     5814 2023-06-08 22:00:37.629907 getajob-0.1.1/getajob/contexts/applications/unit_of_work.py
--rw-r--r--   0        0        0     1140 2023-06-08 22:00:37.629907 getajob-0.1.1/getajob/contexts/companies/models.py
--rw-r--r--   0        0        0     1084 2023-06-08 22:00:37.629907 getajob-0.1.1/getajob/contexts/companies/repository.py
--rw-r--r--   0        0        0     1416 2023-06-08 22:00:37.629907 getajob-0.1.1/getajob/contexts/companies/unit_of_work.py
--rw-r--r--   0        0        0     3135 2023-06-08 22:00:37.629907 getajob-0.1.1/getajob/contexts/jobs/models.py
--rw-r--r--   0        0        0     1040 2023-06-08 22:00:37.629907 getajob-0.1.1/getajob/contexts/jobs/repository.py
--rw-r--r--   0        0        0      462 2023-06-08 22:00:37.629907 getajob-0.1.1/getajob/contexts/jobs/unit_of_work.py
--rw-r--r--   0        0        0      799 2023-06-08 22:00:37.629907 getajob-0.1.1/getajob/contexts/notifications/models.py
--rw-r--r--   0        0        0      537 2023-06-08 22:00:37.629907 getajob-0.1.1/getajob/contexts/notifications/repository.py
--rw-r--r--   0        0        0      761 2023-06-08 22:00:37.629907 getajob-0.1.1/getajob/contexts/recruiters/models.py
--rw-r--r--   0        0        0      446 2023-06-08 22:00:37.629907 getajob-0.1.1/getajob/contexts/recruiters/repository.py
--rw-r--r--   0        0        0     1332 2023-06-08 22:00:37.629907 getajob-0.1.1/getajob/contexts/static/repository.py
--rw-r--r--   0        0        0     1123 2023-06-08 22:00:37.629907 getajob-0.1.1/getajob/contexts/users/clerk_webhook/models.py
--rw-r--r--   0        0        0      843 2023-06-08 22:00:37.629907 getajob-0.1.1/getajob/contexts/users/clerk_webhook/repository.py
--rw-r--r--   0        0        0      409 2023-06-08 22:00:37.629907 getajob-0.1.1/getajob/contexts/users/cover_letters/models.py
--rw-r--r--   0        0        0      345 2023-06-08 22:00:37.629907 getajob-0.1.1/getajob/contexts/users/cover_letters/repository.py
--rw-r--r--   0        0        0      313 2023-06-08 22:00:37.629907 getajob-0.1.1/getajob/contexts/users/resumes/models.py
--rw-r--r--   0        0        0      334 2023-06-08 22:00:37.629907 getajob-0.1.1/getajob/contexts/users/resumes/repository.py
--rw-r--r--   0        0        0      306 2023-06-08 22:00:37.629907 getajob-0.1.1/getajob/contexts/users/sessions/models.py
--rw-r--r--   0        0        0      523 2023-06-08 22:00:37.629907 getajob-0.1.1/getajob/contexts/users/skills/models.py
--rw-r--r--   0        0        0      337 2023-06-08 22:00:37.629907 getajob-0.1.1/getajob/contexts/users/skills/repository.py
--rw-r--r--   0        0        0      726 2023-06-08 22:00:37.629907 getajob-0.1.1/getajob/contexts/users/users/models.py
--rw-r--r--   0        0        0      715 2023-06-08 22:00:37.629907 getajob-0.1.1/getajob/contexts/users/users/repository.py
--rw-r--r--   0        0        0     1794 2023-06-08 22:00:37.629907 getajob-0.1.1/getajob/exceptions.py
--rw-r--r--   0        0        0        0 2023-06-08 22:00:37.629907 getajob-0.1.1/getajob/models/__init__.py
--rw-r--r--   0        0        0      373 2023-06-08 22:00:37.629907 getajob-0.1.1/getajob/models/entities.py
--rw-r--r--   0        0        0      240 2023-06-08 22:00:37.629907 getajob-0.1.1/getajob/models/location.py
--rw-r--r--   0        0        0      375 2023-06-08 22:00:37.629907 getajob-0.1.1/getajob/utils.py
--rw-r--r--   0        0        0     2527 2023-06-08 22:00:37.629907 getajob-0.1.1/getajob/vendor/algolia.py
--rw-r--r--   0        0        0     4456 2023-06-08 22:00:37.629907 getajob-0.1.1/getajob/vendor/clerk.py
--rw-r--r--   0        0        0    11012 2023-06-08 22:00:37.629907 getajob-0.1.1/getajob/vendor/firebase.py
--rw-r--r--   0        0        0      709 2023-06-08 22:00:37.629907 getajob-0.1.1/getajob/vendor/kafka/authentication.py
--rw-r--r--   0        0        0      320 2023-06-08 22:00:37.629907 getajob-0.1.1/getajob/vendor/kafka/exceptions.py
--rw-r--r--   0        0        0     1303 2023-06-08 22:00:37.629907 getajob-0.1.1/getajob/vendor/kafka/kafka.py
--rw-r--r--   0        0        0      179 2023-06-08 22:00:37.629907 getajob-0.1.1/getajob/vendor/kafka/mock.py
--rw-r--r--   0        0        0     1625 2023-06-08 22:00:37.629907 getajob-0.1.1/getajob/vendor/kafka/models.py
--rw-r--r--   0        0        0      585 2023-06-08 22:00:37.629907 getajob-0.1.1/getajob/vendor/kafka/repository.py
--rw-r--r--   0        0        0     1998 2023-06-08 22:00:37.629907 getajob-0.1.1/getajob/vendor/openai.py
--rw-r--r--   0        0        0      599 2023-06-08 22:00:37.629907 getajob-0.1.1/getajob/vendor/sendgrid/sendgrid.py
--rw-r--r--   0        0        0      207 2023-06-08 22:00:37.629907 getajob-0.1.1/getajob/vendor/sentry.py
--rw-r--r--   0        0        0     1724 2023-06-08 22:00:37.629907 getajob-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2869 1970-01-01 00:00:00.000000 getajob-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       69 2023-06-09 12:25:34.191388 getajob-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-06-09 12:25:34.191388 getajob-0.1.2/getajob/__init__.py
+-rw-r--r--   0        0        0     1013 2023-06-09 12:25:34.191388 getajob-0.1.2/getajob/abstractions/models.py
+-rw-r--r--   0        0        0     6850 2023-06-09 12:25:34.191388 getajob-0.1.2/getajob/abstractions/repository.py
+-rw-r--r--   0        0        0     3138 2023-06-09 12:25:34.191388 getajob-0.1.2/getajob/auth.py
+-rw-r--r--   0        0        0     2621 2023-06-09 12:25:34.191388 getajob-0.1.2/getajob/config/settings.py
+-rw-r--r--   0        0        0        0 2023-06-09 12:25:34.191388 getajob-0.1.2/getajob/contexts/__init__.py
+-rw-r--r--   0        0        0      170 2023-06-09 12:25:34.191388 getajob-0.1.2/getajob/contexts/admin/search/models.py
+-rw-r--r--   0        0        0      574 2023-06-09 12:25:34.191388 getajob-0.1.2/getajob/contexts/admin/search/repository.py
+-rw-r--r--   0        0        0      737 2023-06-09 12:25:34.191388 getajob-0.1.2/getajob/contexts/admin/users/models.py
+-rw-r--r--   0        0        0      447 2023-06-09 12:25:34.191388 getajob-0.1.2/getajob/contexts/admin/users/repository.py
+-rw-r--r--   0        0        0      823 2023-06-09 12:25:34.191388 getajob-0.1.2/getajob/contexts/ai/text/models.py
+-rw-r--r--   0        0        0     2470 2023-06-09 12:25:34.191388 getajob-0.1.2/getajob/contexts/ai/text/repository.py
+-rw-r--r--   0        0        0     1530 2023-06-09 12:25:34.191388 getajob-0.1.2/getajob/contexts/applications/models.py
+-rw-r--r--   0        0        0     4340 2023-06-09 12:25:34.191388 getajob-0.1.2/getajob/contexts/applications/repository.py
+-rw-r--r--   0        0        0     5814 2023-06-09 12:25:34.191388 getajob-0.1.2/getajob/contexts/applications/unit_of_work.py
+-rw-r--r--   0        0        0     1140 2023-06-09 12:25:34.191388 getajob-0.1.2/getajob/contexts/companies/models.py
+-rw-r--r--   0        0        0     1084 2023-06-09 12:25:34.191388 getajob-0.1.2/getajob/contexts/companies/repository.py
+-rw-r--r--   0        0        0     1416 2023-06-09 12:25:34.191388 getajob-0.1.2/getajob/contexts/companies/unit_of_work.py
+-rw-r--r--   0        0        0     3135 2023-06-09 12:25:34.191388 getajob-0.1.2/getajob/contexts/jobs/models.py
+-rw-r--r--   0        0        0     1040 2023-06-09 12:25:34.191388 getajob-0.1.2/getajob/contexts/jobs/repository.py
+-rw-r--r--   0        0        0      462 2023-06-09 12:25:34.191388 getajob-0.1.2/getajob/contexts/jobs/unit_of_work.py
+-rw-r--r--   0        0        0      799 2023-06-09 12:25:34.191388 getajob-0.1.2/getajob/contexts/notifications/models.py
+-rw-r--r--   0        0        0      537 2023-06-09 12:25:34.191388 getajob-0.1.2/getajob/contexts/notifications/repository.py
+-rw-r--r--   0        0        0      761 2023-06-09 12:25:34.191388 getajob-0.1.2/getajob/contexts/recruiters/models.py
+-rw-r--r--   0        0        0      446 2023-06-09 12:25:34.191388 getajob-0.1.2/getajob/contexts/recruiters/repository.py
+-rw-r--r--   0        0        0     1332 2023-06-09 12:25:34.191388 getajob-0.1.2/getajob/contexts/static/repository.py
+-rw-r--r--   0        0        0     1123 2023-06-09 12:25:34.191388 getajob-0.1.2/getajob/contexts/users/clerk_webhook/models.py
+-rw-r--r--   0        0        0      843 2023-06-09 12:25:34.191388 getajob-0.1.2/getajob/contexts/users/clerk_webhook/repository.py
+-rw-r--r--   0        0        0      409 2023-06-09 12:25:34.191388 getajob-0.1.2/getajob/contexts/users/cover_letters/models.py
+-rw-r--r--   0        0        0      345 2023-06-09 12:25:34.191388 getajob-0.1.2/getajob/contexts/users/cover_letters/repository.py
+-rw-r--r--   0        0        0      313 2023-06-09 12:25:34.191388 getajob-0.1.2/getajob/contexts/users/resumes/models.py
+-rw-r--r--   0        0        0      334 2023-06-09 12:25:34.191388 getajob-0.1.2/getajob/contexts/users/resumes/repository.py
+-rw-r--r--   0        0        0      306 2023-06-09 12:25:34.191388 getajob-0.1.2/getajob/contexts/users/sessions/models.py
+-rw-r--r--   0        0        0      523 2023-06-09 12:25:34.191388 getajob-0.1.2/getajob/contexts/users/skills/models.py
+-rw-r--r--   0        0        0      337 2023-06-09 12:25:34.191388 getajob-0.1.2/getajob/contexts/users/skills/repository.py
+-rw-r--r--   0        0        0      726 2023-06-09 12:25:34.191388 getajob-0.1.2/getajob/contexts/users/users/models.py
+-rw-r--r--   0        0        0      715 2023-06-09 12:25:34.191388 getajob-0.1.2/getajob/contexts/users/users/repository.py
+-rw-r--r--   0        0        0     1794 2023-06-09 12:25:34.191388 getajob-0.1.2/getajob/exceptions.py
+-rw-r--r--   0        0        0        0 2023-06-09 12:25:34.191388 getajob-0.1.2/getajob/models/__init__.py
+-rw-r--r--   0        0        0      373 2023-06-09 12:25:34.191388 getajob-0.1.2/getajob/models/entities.py
+-rw-r--r--   0        0        0      240 2023-06-09 12:25:34.191388 getajob-0.1.2/getajob/models/location.py
+-rw-r--r--   0        0        0      375 2023-06-09 12:25:34.191388 getajob-0.1.2/getajob/utils.py
+-rw-r--r--   0        0        0     2527 2023-06-09 12:25:34.191388 getajob-0.1.2/getajob/vendor/algolia.py
+-rw-r--r--   0        0        0     4456 2023-06-09 12:25:34.191388 getajob-0.1.2/getajob/vendor/clerk.py
+-rw-r--r--   0        0        0    11012 2023-06-09 12:25:34.191388 getajob-0.1.2/getajob/vendor/firebase.py
+-rw-r--r--   0        0        0      709 2023-06-09 12:25:34.191388 getajob-0.1.2/getajob/vendor/kafka/authentication.py
+-rw-r--r--   0        0        0      320 2023-06-09 12:25:34.191388 getajob-0.1.2/getajob/vendor/kafka/exceptions.py
+-rw-r--r--   0        0        0     1303 2023-06-09 12:25:34.191388 getajob-0.1.2/getajob/vendor/kafka/kafka.py
+-rw-r--r--   0        0        0      179 2023-06-09 12:25:34.191388 getajob-0.1.2/getajob/vendor/kafka/mock.py
+-rw-r--r--   0        0        0     1625 2023-06-09 12:25:34.191388 getajob-0.1.2/getajob/vendor/kafka/models.py
+-rw-r--r--   0        0        0      585 2023-06-09 12:25:34.191388 getajob-0.1.2/getajob/vendor/kafka/repository.py
+-rw-r--r--   0        0        0     1998 2023-06-09 12:25:34.191388 getajob-0.1.2/getajob/vendor/openai.py
+-rw-r--r--   0        0        0      599 2023-06-09 12:25:34.191388 getajob-0.1.2/getajob/vendor/sendgrid/sendgrid.py
+-rw-r--r--   0        0        0      207 2023-06-09 12:25:34.191388 getajob-0.1.2/getajob/vendor/sentry.py
+-rw-r--r--   0        0        0     1724 2023-06-09 12:25:34.191388 getajob-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2869 1970-01-01 00:00:00.000000 getajob-0.1.2/PKG-INFO
```

### Comparing `getajob-0.1.1/getajob/abstractions/models.py` & `getajob-0.1.2/getajob/abstractions/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.1.1/getajob/abstractions/repository.py` & `getajob-0.1.2/getajob/abstractions/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.1.1/getajob/auth.py` & `getajob-0.1.2/getajob/auth.py`

 * *Files identical despite different names*

### Comparing `getajob-0.1.1/getajob/contexts/admin/search/repository.py` & `getajob-0.1.2/getajob/contexts/admin/search/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.1.1/getajob/contexts/admin/users/models.py` & `getajob-0.1.2/getajob/contexts/admin/users/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.1.1/getajob/contexts/ai/text/models.py` & `getajob-0.1.2/getajob/contexts/ai/text/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.1.1/getajob/contexts/ai/text/repository.py` & `getajob-0.1.2/getajob/contexts/ai/text/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.1.1/getajob/contexts/applications/models.py` & `getajob-0.1.2/getajob/contexts/applications/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.1.1/getajob/contexts/applications/repository.py` & `getajob-0.1.2/getajob/contexts/applications/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.1.1/getajob/contexts/applications/unit_of_work.py` & `getajob-0.1.2/getajob/contexts/applications/unit_of_work.py`

 * *Files identical despite different names*

### Comparing `getajob-0.1.1/getajob/contexts/companies/models.py` & `getajob-0.1.2/getajob/contexts/companies/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.1.1/getajob/contexts/companies/repository.py` & `getajob-0.1.2/getajob/contexts/companies/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.1.1/getajob/contexts/companies/unit_of_work.py` & `getajob-0.1.2/getajob/contexts/companies/unit_of_work.py`

 * *Files identical despite different names*

### Comparing `getajob-0.1.1/getajob/contexts/jobs/models.py` & `getajob-0.1.2/getajob/contexts/jobs/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.1.1/getajob/contexts/jobs/repository.py` & `getajob-0.1.2/getajob/contexts/jobs/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.1.1/getajob/contexts/notifications/models.py` & `getajob-0.1.2/getajob/contexts/notifications/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.1.1/getajob/contexts/notifications/repository.py` & `getajob-0.1.2/getajob/contexts/notifications/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.1.1/getajob/contexts/recruiters/models.py` & `getajob-0.1.2/getajob/contexts/recruiters/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.1.1/getajob/contexts/static/repository.py` & `getajob-0.1.2/getajob/contexts/static/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.1.1/getajob/contexts/users/clerk_webhook/models.py` & `getajob-0.1.2/getajob/contexts/users/clerk_webhook/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.1.1/getajob/contexts/users/clerk_webhook/repository.py` & `getajob-0.1.2/getajob/contexts/users/clerk_webhook/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.1.1/getajob/contexts/users/skills/models.py` & `getajob-0.1.2/getajob/contexts/users/skills/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.1.1/getajob/contexts/users/users/models.py` & `getajob-0.1.2/getajob/contexts/users/users/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.1.1/getajob/contexts/users/users/repository.py` & `getajob-0.1.2/getajob/contexts/users/users/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.1.1/getajob/exceptions.py` & `getajob-0.1.2/getajob/exceptions.py`

 * *Files identical despite different names*

### Comparing `getajob-0.1.1/getajob/vendor/algolia.py` & `getajob-0.1.2/getajob/vendor/algolia.py`

 * *Files identical despite different names*

### Comparing `getajob-0.1.1/getajob/vendor/clerk.py` & `getajob-0.1.2/getajob/vendor/clerk.py`

 * *Files identical despite different names*

### Comparing `getajob-0.1.1/getajob/vendor/firebase.py` & `getajob-0.1.2/getajob/vendor/firebase.py`

 * *Files identical despite different names*

### Comparing `getajob-0.1.1/getajob/vendor/kafka/authentication.py` & `getajob-0.1.2/getajob/vendor/kafka/authentication.py`

 * *Files identical despite different names*

### Comparing `getajob-0.1.1/getajob/vendor/kafka/kafka.py` & `getajob-0.1.2/getajob/vendor/kafka/kafka.py`

 * *Files identical despite different names*

### Comparing `getajob-0.1.1/getajob/vendor/kafka/models.py` & `getajob-0.1.2/getajob/vendor/kafka/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.1.1/getajob/vendor/kafka/repository.py` & `getajob-0.1.2/getajob/vendor/kafka/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.1.1/getajob/vendor/openai.py` & `getajob-0.1.2/getajob/vendor/openai.py`

 * *Files identical despite different names*

### Comparing `getajob-0.1.1/getajob/vendor/sendgrid/sendgrid.py` & `getajob-0.1.2/getajob/vendor/sendgrid/sendgrid.py`

 * *Files identical despite different names*

### Comparing `getajob-0.1.1/pyproject.toml` & `getajob-0.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "getajob"
-version = "0.1.1"
+version = "0.1.2"
 description = ""
 authors = ["Your Name <you@example.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 aiohttp = "3.8.4"
```

### Comparing `getajob-0.1.1/PKG-INFO` & `getajob-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getajob
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

