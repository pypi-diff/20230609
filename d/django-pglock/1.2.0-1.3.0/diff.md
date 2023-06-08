# Comparing `tmp/django_pglock-1.2.0.tar.gz` & `tmp/django_pglock-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_pglock-1.2.0.tar", max compression
+gzip compressed data, was "django_pglock-1.3.0.tar", max compression
```

## Comparing `django_pglock-1.2.0.tar` & `django_pglock-1.3.0.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0     1456 2023-05-08 13:18:27.576763 django_pglock-1.2.0/LICENSE
--rw-r--r--   0        0        0     5017 2023-05-08 13:18:27.576763 django_pglock-1.2.0/README.rst
--rw-r--r--   0        0        0      877 2023-05-08 13:18:27.576763 django_pglock-1.2.0/pglock/__init__.py
--rw-r--r--   0        0        0     1766 2023-05-08 13:18:27.576763 django_pglock-1.2.0/pglock/config.py
--rw-r--r--   0        0        0    19826 2023-05-08 13:18:27.576763 django_pglock-1.2.0/pglock/core.py
--rw-r--r--   0        0        0        0 2023-05-08 13:18:27.576763 django_pglock-1.2.0/pglock/management/__init__.py
--rw-r--r--   0        0        0        0 2023-05-08 13:18:27.576763 django_pglock-1.2.0/pglock/management/commands/__init__.py
--rw-r--r--   0        0        0     5490 2023-05-08 13:18:27.576763 django_pglock-1.2.0/pglock/management/commands/pglock.py
--rw-r--r--   0        0        0     9526 2023-05-08 13:18:27.576763 django_pglock-1.2.0/pglock/models.py
--rw-r--r--   0        0        0      151 2023-05-08 13:18:27.576763 django_pglock-1.2.0/pglock/version.py
--rw-r--r--   0        0        0     2414 2023-05-08 13:19:12.992488 django_pglock-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     6525 1970-01-01 00:00:00.000000 django_pglock-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1456 2023-06-08 23:46:32.924168 django_pglock-1.3.0/LICENSE
+-rw-r--r--   0        0        0     5031 2023-06-08 23:46:32.924168 django_pglock-1.3.0/README.rst
+-rw-r--r--   0        0        0      877 2023-06-08 23:46:32.924168 django_pglock-1.3.0/pglock/__init__.py
+-rw-r--r--   0        0        0     1766 2023-06-08 23:46:32.924168 django_pglock-1.3.0/pglock/config.py
+-rw-r--r--   0        0        0    20429 2023-06-08 23:46:32.924168 django_pglock-1.3.0/pglock/core.py
+-rw-r--r--   0        0        0        0 2023-06-08 23:46:32.924168 django_pglock-1.3.0/pglock/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-08 23:46:32.924168 django_pglock-1.3.0/pglock/management/commands/__init__.py
+-rw-r--r--   0        0        0     5490 2023-06-08 23:46:32.924168 django_pglock-1.3.0/pglock/management/commands/pglock.py
+-rw-r--r--   0        0        0     9463 2023-06-08 23:46:32.924168 django_pglock-1.3.0/pglock/models.py
+-rw-r--r--   0        0        0      916 2023-06-08 23:46:32.924168 django_pglock-1.3.0/pglock/utils.py
+-rw-r--r--   0        0        0      151 2023-06-08 23:46:32.924168 django_pglock-1.3.0/pglock/version.py
+-rw-r--r--   0        0        0     2408 2023-06-08 23:47:03.476326 django_pglock-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     6338 1970-01-01 00:00:00.000000 django_pglock-1.3.0/PKG-INFO
```

### Comparing `django_pglock-1.2.0/LICENSE` & `django_pglock-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_pglock-1.2.0/README.rst` & `django_pglock-1.3.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -115,15 +115,15 @@
 
 Use ``python manage.py pglock`` to view and kill locks from the command line. It has
 several options for dynamic filters and re-usable configuration.
 
 Compatibility
 =============
 
-``django-pglock`` is compatible with Python 3.7 - 3.10, Django 2.2 - 4.1, and Postgres 10 - 15.
+``django-pglock`` is compatible with Python 3.7 - 3.11, Django 3.2 - 4.2, Psycopg 2 - 3 and Postgres 12 - 15.
 
 Documentation
 =============
 
 `View the django-pglock docs here
 <https://django-pglock.readthedocs.io/>`_ to learn more about:
```

### Comparing `django_pglock-1.2.0/pglock/__init__.py` & `django_pglock-1.3.0/pglock/__init__.py`

 * *Files identical despite different names*

### Comparing `django_pglock-1.2.0/pglock/config.py` & `django_pglock-1.3.0/pglock/config.py`

 * *Files identical despite different names*

### Comparing `django_pglock-1.2.0/pglock/core.py` & `django_pglock-1.3.0/pglock/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,23 @@
 import inspect
 import threading
 
 from django.apps import apps
 from django.db import connections, DEFAULT_DB_ALIAS, transaction
 from django.db.utils import OperationalError
 import pgactivity
-import psycopg2.extensions
+
+from pglock import utils
+
+if utils.psycopg_maj_version == 2:
+    import psycopg2.extensions
+elif utils.psycopg_maj_version == 3:
+    import psycopg.pq
+else:
+    raise AssertionError
 
 
 # Lock levels
 ACCESS_SHARE = "ACCESS SHARE"
 ROW_SHARE = "ROW SHARE"
 ROW_EXCLUSIVE = "ROW EXCLUSIVE"
 SHARE_UPDATE_EXCLUSIVE = "SHARE UPDATE EXCLUSIVE"
@@ -62,14 +70,29 @@
 
         if timeout < dt.timedelta(milliseconds=1):
             timeout = dt.timedelta()
 
     return timeout
 
 
+def _is_transaction_errored(cursor):
+    """
+    True if the current transaction is in an errored state
+    """
+    if utils.psycopg_maj_version == 2:
+        return (
+            cursor.connection.get_transaction_status()
+            == psycopg2.extensions.TRANSACTION_STATUS_INERROR
+        )
+    elif utils.psycopg_maj_version == 3:
+        return cursor.connection.info.transaction_status == psycopg.pq.TransactionStatus.INERROR
+    else:
+        raise AssertionError
+
+
 @contextlib.contextmanager
 def lock_timeout(timeout=_unset, *, using=DEFAULT_DB_ALIAS, **timedelta_kwargs):
     """Set the lock timeout as a decorator or context manager.
 
     A value of ``None`` will set an infinite lock timeout.
     A value of less than a millisecond is not permitted.
 
@@ -111,28 +134,25 @@
         _timeout.value = None
 
     old_timeout = _timeout.value
     _timeout.value = int(timeout.total_seconds() * 1000)
 
     try:
         with connections[using].cursor() as cursor:
-            cursor.execute(f"SET lock_timeout={_timeout.value}")
+            cursor.execute(f"SELECT set_config('lock_timeout', '{_timeout.value}', false)")
             yield
     finally:
         _timeout.value = old_timeout
 
         with connections[using].cursor() as cursor:
-            if (
-                not cursor.connection.get_transaction_status()
-                == psycopg2.extensions.TRANSACTION_STATUS_INERROR
-            ):
+            if not _is_transaction_errored(cursor):
                 if _timeout.value is None:
-                    cursor.execute("RESET lock_timeout")
+                    cursor.execute("SELECT set_config('lock_timeout', NULL, false)")
                 else:
-                    cursor.execute(f"SET lock_timeout={_timeout.value}")
+                    cursor.execute(f"SELECT set_config('lock_timeout', '{_timeout.value}', false)")
 
 
 def _cast_lock_id(lock_id):
     """Cast a lock ID into the appropriate type"""
     if isinstance(lock_id, str):
         return int.from_bytes(
             hashlib.sha256(lock_id.encode("utf-8")).digest()[:8], "little", signed=True
```

### Comparing `django_pglock-1.2.0/pglock/management/commands/pglock.py` & `django_pglock-1.3.0/pglock/management/commands/pglock.py`

 * *Files identical despite different names*

### Comparing `django_pglock-1.2.0/pglock/models.py` & `django_pglock-1.3.0/pglock/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,47 +1,45 @@
 from django.apps import apps
 from django.conf import settings
-from django.db import connections, DEFAULT_DB_ALIAS, models
+from django.db import DEFAULT_DB_ALIAS, models
 import pgactivity
 import pgactivity.models
 
-from pglock import config
+from pglock import config, utils
 
 
 class PGTableQueryCompiler(pgactivity.models.PGTableQueryCompiler):
     def get_pid_clause(self):
         if isinstance(self.query.pids, str):
             return f"AND pid = ANY({self.query.pids})"
         else:
             return super().get_pid_clause()
 
     def get_ctes(self):
         ctes = super().get_ctes()
 
-        with connections[self.using].cursor() as cursor:
-            pg_version = str(cursor.connection.server_version).rjust(6, "0")
-
         if self.query.relations:
             models = [
                 apps.get_model(model) if isinstance(model, str) else model
                 for model in self.query.relations
             ]
             rel_name_clause = (
                 "AND pg_class.relname IN ("
                 + ", ".join(f"'{model._meta.db_table}'" for model in models)
                 + ")"
             )
         else:
             rel_name_clause = ""
 
-        if int(pg_version[:2]) >= 14:
-            # Waitstart is available in pg 14 and up
-            wait_start_clause = "waitstart AS wait_start, NOW() - waitstart AS wait_duration"
-        else:  # pragma: no cover
-            wait_start_clause = "NULL AS wait_start, NULL AS wait_duration"
+        with self.connection.cursor() as cursor:  # pragma: no cover
+            if utils.pg_maj_version(cursor) >= 14:
+                # Waitstart is available in pg 14 and up
+                wait_start_clause = "waitstart AS wait_start, NOW() - waitstart AS wait_duration"
+            else:
+                wait_start_clause = "NULL AS wait_start, NULL AS wait_duration"
 
         lock_cte = rf"""
             _pglock_lock_cte AS (
                 SELECT
                     pid AS id,
                     pid AS activity_id,
                     TRIM(
```

### Comparing `django_pglock-1.2.0/pyproject.toml` & `django_pglock-1.3.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -25,64 +25,64 @@
 name = "django-pglock"
 packages = [
   { include = "pglock" }
 ]
 exclude = [
   "*/tests/"
 ]
-version = "1.2.0"
+version = "1.3.0"
 description = "Postgres locking routines and lock table access."
 authors = ["Opus 10 Engineering"]
 classifiers = [
   "Framework :: Django",
-  "Framework :: Django :: 2.2",
   "Framework :: Django :: 3.2",
   "Framework :: Django :: 4.0",
   "Framework :: Django :: 4.1",
+  "Framework :: Django :: 4.2",
   "Intended Audience :: Developers",
   "Operating System :: OS Independent",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3 :: Only",
   "Framework :: Django",
 ]
 license = "BSD-3-Clause"
 readme = "README.rst"
 homepage = "https://github.com/Opus10/django-pglock"
 repository = "https://github.com/Opus10/django-pglock"
 documentation = "https://django-pglock.readthedocs.io"
 
 [tool.poetry.dependencies]
 python = ">=3.7.0,<4"
 django = ">=2"
-django-pgactivity = ">=1.1,<2"
+django-pgactivity = ">=1.2,<2"
 importlib_metadata = { version = ">=4", python = "~3.7" }
 
 [tool.poetry.dev-dependencies]
 black = "22.6.0"
 dj-database-url = "0.5.0"
 django-dynamic-fixture = "3.1.2"
 django-extensions = "3.2.1"
 flake8 = "3.9.2"
 flake8-bugbear = "22.1.11"
 flake8-comprehensions = "3.8.0"
 flake8-import-order = "0.18.1"
 flake8-logging-format = "0.6.0"
 flake8-mutable = "1.2.0"
 git-tidy = "1.2.0"
-ipython = { version = "8.5.0", python = ">=3.8" }
 myst-parser = "0.18.0"
 packaging = ">=19.2"
 pip = "*"
 poetry-core = "1.3.2"
 pre-commit = "2.13.0"
-psycopg2-binary = "2.9.3"
+psycopg2-binary = "2.9.6"
 pytest = "7.0.0"
 pytest-cov = "3.0.0"
 pytest-dotenv = "0.5.2"
 pytest-django = "4.5.2"
 pytest-mock = "3.10.0"
 pytest-reraise = "2.1.2"
 requests = "2.25.1"
```

### Comparing `django_pglock-1.2.0/PKG-INFO` & `django_pglock-1.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,33 @@
 Metadata-Version: 2.1
 Name: django-pglock
-Version: 1.2.0
+Version: 1.3.0
 Summary: Postgres locking routines and lock table access.
 Home-page: https://github.com/Opus10/django-pglock
 License: BSD-3-Clause
 Author: Opus 10 Engineering
 Requires-Python: >=3.7.0,<4
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: django (>=2)
-Requires-Dist: django-pgactivity (>=1.1,<2)
+Requires-Dist: django-pgactivity (>=1.2,<2)
 Requires-Dist: importlib_metadata (>=4) ; python_version >= "3.7" and python_version < "3.8"
 Project-URL: Documentation, https://django-pglock.readthedocs.io
 Project-URL: Repository, https://github.com/Opus10/django-pglock
 Description-Content-Type: text/x-rst
 
 django-pglock
 #############
@@ -150,15 +146,15 @@
 
 Use ``python manage.py pglock`` to view and kill locks from the command line. It has
 several options for dynamic filters and re-usable configuration.
 
 Compatibility
 =============
 
-``django-pglock`` is compatible with Python 3.7 - 3.10, Django 2.2 - 4.1, and Postgres 10 - 15.
+``django-pglock`` is compatible with Python 3.7 - 3.11, Django 3.2 - 4.2, Psycopg 2 - 3 and Postgres 12 - 15.
 
 Documentation
 =============
 
 `View the django-pglock docs here
 <https://django-pglock.readthedocs.io/>`_ to learn more about:
```

