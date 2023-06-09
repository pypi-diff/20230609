# Comparing `tmp/python-tldap-1.0.6.tar.gz` & `tmp/python_tldap-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-tldap-1.0.6.tar", max compression
+gzip compressed data, was "python_tldap-1.0.7.tar", max compression
```

## Comparing `python-tldap-1.0.6.tar` & `python_tldap-1.0.7.tar`

### file list

```diff
@@ -1,40 +1,39 @@
--rw-r--r--   0        0        0      410 2021-04-07 23:09:31.053908 python-tldap-1.0.6/README.rst
--rw-r--r--   0        0        0     1187 2021-04-07 23:09:31.053908 python-tldap-1.0.6/pyproject.toml
--rw-r--r--   0        0        0     1024 2021-04-07 23:09:31.057908 python-tldap-1.0.6/tldap/__init__.py
--rw-r--r--   0        0        0     2141 2021-04-07 23:09:31.057908 python-tldap-1.0.6/tldap/backend/__init__.py
--rw-r--r--   0        0        0     8635 2021-04-07 23:09:31.057908 python-tldap-1.0.6/tldap/backend/base.py
--rw-r--r--   0        0        0    13484 2021-04-07 23:09:31.057908 python-tldap-1.0.6/tldap/backend/fake_transactions.py
--rw-r--r--   0        0        0     3836 2021-04-07 23:09:31.057908 python-tldap-1.0.6/tldap/backend/no_transactions.py
--rw-r--r--   0        0        0    20957 2021-04-07 23:09:31.057908 python-tldap-1.0.6/tldap/database/__init__.py
--rw-r--r--   0        0        0    12564 2021-04-07 23:09:31.057908 python-tldap-1.0.6/tldap/database/helpers.py
--rw-r--r--   0        0        0     4085 2021-04-07 23:09:31.057908 python-tldap-1.0.6/tldap/dict.py
--rw-r--r--   0        0        0     1981 2021-04-07 23:09:31.057908 python-tldap-1.0.6/tldap/django/__init__.py
--rw-r--r--   0        0        0      154 2021-04-07 23:09:31.057908 python-tldap-1.0.6/tldap/django/apps.py
--rw-r--r--   0        0        0     2452 2021-04-07 23:09:31.057908 python-tldap-1.0.6/tldap/django/helpers.py
--rw-r--r--   0        0        0     1759 2021-04-07 23:09:31.057908 python-tldap-1.0.6/tldap/django/middleware.py
--rw-r--r--   0        0        0      759 2021-04-07 23:09:31.057908 python-tldap-1.0.6/tldap/django/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2021-04-07 23:09:31.057908 python-tldap-1.0.6/tldap/django/migrations/__init__.py
--rw-r--r--   0        0        0     1600 2021-04-07 23:09:31.057908 python-tldap-1.0.6/tldap/django/models.py
--rw-r--r--   0        0        0    13203 2021-04-07 23:09:31.057908 python-tldap-1.0.6/tldap/dn.py
--rw-r--r--   0        0        0     1494 2021-04-07 23:09:31.057908 python-tldap-1.0.6/tldap/exceptions.py
--rw-r--r--   0        0        0    15773 2021-04-07 23:09:31.057908 python-tldap-1.0.6/tldap/fields.py
--rw-r--r--   0        0        0     1852 2021-04-07 23:09:31.057908 python-tldap-1.0.6/tldap/filter.py
--rw-r--r--   0        0        0     1524 2021-04-07 23:09:31.057908 python-tldap-1.0.6/tldap/ldap_passwd.py
--rw-r--r--   0        0        0     5474 2021-04-07 23:09:31.057908 python-tldap-1.0.6/tldap/modlist.py
--rw-r--r--   0        0        0     5378 2021-04-07 23:09:31.057908 python-tldap-1.0.6/tldap/query.py
--rw-r--r--   0        0        0     1740 2021-04-07 23:09:31.057908 python-tldap-1.0.6/tldap/query_utils.py
--rw-r--r--   0        0        0      706 2021-04-07 23:09:31.057908 python-tldap-1.0.6/tldap/test/__init__.py
--rw-r--r--   0        0        0    20346 2021-04-07 23:09:31.057908 python-tldap-1.0.6/tldap/test/ldap_schemas/00-core.schema
--rw-r--r--   0        0        0    14030 2021-04-07 23:09:31.057908 python-tldap-1.0.6/tldap/test/ldap_schemas/10-cosine.schema
--rw-r--r--   0        0        0     6360 2021-04-07 23:09:31.057908 python-tldap-1.0.6/tldap/test/ldap_schemas/50-inetorgperson.schema
--rw-r--r--   0        0        0     4204 2021-04-07 23:09:31.057908 python-tldap-1.0.6/tldap/test/ldap_schemas/70-eduperson.schema
--rw-r--r--   0        0        0    14617 2021-04-07 23:09:31.057908 python-tldap-1.0.6/tldap/test/ldap_schemas/90-aueduperson.schema
--rw-r--r--   0        0        0     5274 2021-04-07 23:09:31.057908 python-tldap-1.0.6/tldap/test/ldap_schemas/90-ppolicy.schema
--rw-r--r--   0        0        0    19957 2021-04-07 23:09:31.061908 python-tldap-1.0.6/tldap/test/ldap_schemas/90-schac.schema
--rw-r--r--   0        0        0     7723 2021-04-07 23:09:31.061908 python-tldap-1.0.6/tldap/test/ldap_schemas/nis.schema
--rw-r--r--   0        0        0    16644 2021-04-07 23:09:31.061908 python-tldap-1.0.6/tldap/test/slapd.py
--rw-r--r--   0        0        0     7902 2021-04-07 23:09:31.061908 python-tldap-1.0.6/tldap/transaction.py
--rw-r--r--   0        0        0     4915 2021-04-07 23:09:31.061908 python-tldap-1.0.6/tldap/tree.py
--rw-r--r--   0        0        0     1651 2021-04-07 23:09:31.061908 python-tldap-1.0.6/tldap/utils.py
--rw-r--r--   0        0        0     1231 2021-04-07 23:10:17.602747 python-tldap-1.0.6/setup.py
--rw-r--r--   0        0        0     1412 2021-04-07 23:10:17.603096 python-tldap-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0      410 2023-06-09 04:44:12.801242 python_tldap-1.0.7/README.rst
+-rw-r--r--   0        0        0     1322 2023-06-09 04:44:12.801242 python_tldap-1.0.7/pyproject.toml
+-rw-r--r--   0        0        0     1024 2023-06-09 04:44:12.805242 python_tldap-1.0.7/tldap/__init__.py
+-rw-r--r--   0        0        0     2141 2023-06-09 04:44:12.805242 python_tldap-1.0.7/tldap/backend/__init__.py
+-rw-r--r--   0        0        0     8635 2023-06-09 04:44:12.805242 python_tldap-1.0.7/tldap/backend/base.py
+-rw-r--r--   0        0        0    13485 2023-06-09 04:44:12.805242 python_tldap-1.0.7/tldap/backend/fake_transactions.py
+-rw-r--r--   0        0        0     3836 2023-06-09 04:44:12.805242 python_tldap-1.0.7/tldap/backend/no_transactions.py
+-rw-r--r--   0        0        0    20957 2023-06-09 04:44:12.805242 python_tldap-1.0.7/tldap/database/__init__.py
+-rw-r--r--   0        0        0    12564 2023-06-09 04:44:12.805242 python_tldap-1.0.7/tldap/database/helpers.py
+-rw-r--r--   0        0        0     4085 2023-06-09 04:44:12.805242 python_tldap-1.0.7/tldap/dict.py
+-rw-r--r--   0        0        0     1981 2023-06-09 04:44:12.805242 python_tldap-1.0.7/tldap/django/__init__.py
+-rw-r--r--   0        0        0      154 2023-06-09 04:44:12.805242 python_tldap-1.0.7/tldap/django/apps.py
+-rw-r--r--   0        0        0     2452 2023-06-09 04:44:12.805242 python_tldap-1.0.7/tldap/django/helpers.py
+-rw-r--r--   0        0        0     1759 2023-06-09 04:44:12.805242 python_tldap-1.0.7/tldap/django/middleware.py
+-rw-r--r--   0        0        0      759 2023-06-09 04:44:12.805242 python_tldap-1.0.7/tldap/django/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-06-09 04:44:12.805242 python_tldap-1.0.7/tldap/django/migrations/__init__.py
+-rw-r--r--   0        0        0     1600 2023-06-09 04:44:12.805242 python_tldap-1.0.7/tldap/django/models.py
+-rw-r--r--   0        0        0    13204 2023-06-09 04:44:12.805242 python_tldap-1.0.7/tldap/dn.py
+-rw-r--r--   0        0        0     1494 2023-06-09 04:44:12.805242 python_tldap-1.0.7/tldap/exceptions.py
+-rw-r--r--   0        0        0    15773 2023-06-09 04:44:12.805242 python_tldap-1.0.7/tldap/fields.py
+-rw-r--r--   0        0        0     1852 2023-06-09 04:44:12.805242 python_tldap-1.0.7/tldap/filter.py
+-rw-r--r--   0        0        0     1524 2023-06-09 04:44:12.805242 python_tldap-1.0.7/tldap/ldap_passwd.py
+-rw-r--r--   0        0        0     5474 2023-06-09 04:44:12.805242 python_tldap-1.0.7/tldap/modlist.py
+-rw-r--r--   0        0        0     5378 2023-06-09 04:44:12.805242 python_tldap-1.0.7/tldap/query.py
+-rw-r--r--   0        0        0     1740 2023-06-09 04:44:12.805242 python_tldap-1.0.7/tldap/query_utils.py
+-rw-r--r--   0        0        0      706 2023-06-09 04:44:12.805242 python_tldap-1.0.7/tldap/test/__init__.py
+-rw-r--r--   0        0        0    20346 2023-06-09 04:44:12.805242 python_tldap-1.0.7/tldap/test/ldap_schemas/00-core.schema
+-rw-r--r--   0        0        0    14030 2023-06-09 04:44:12.805242 python_tldap-1.0.7/tldap/test/ldap_schemas/10-cosine.schema
+-rw-r--r--   0        0        0     6360 2023-06-09 04:44:12.805242 python_tldap-1.0.7/tldap/test/ldap_schemas/50-inetorgperson.schema
+-rw-r--r--   0        0        0     4204 2023-06-09 04:44:12.805242 python_tldap-1.0.7/tldap/test/ldap_schemas/70-eduperson.schema
+-rw-r--r--   0        0        0    14617 2023-06-09 04:44:12.805242 python_tldap-1.0.7/tldap/test/ldap_schemas/90-aueduperson.schema
+-rw-r--r--   0        0        0    19957 2023-06-09 04:44:12.805242 python_tldap-1.0.7/tldap/test/ldap_schemas/90-schac.schema
+-rw-r--r--   0        0        0     7723 2023-06-09 04:44:12.805242 python_tldap-1.0.7/tldap/test/ldap_schemas/nis.schema
+-rw-r--r--   0        0        0    15901 2023-06-09 04:44:12.805242 python_tldap-1.0.7/tldap/test/slapd.py
+-rw-r--r--   0        0        0     7902 2023-06-09 04:44:12.805242 python_tldap-1.0.7/tldap/transaction.py
+-rw-r--r--   0        0        0     4915 2023-06-09 04:44:12.805242 python_tldap-1.0.7/tldap/tree.py
+-rw-r--r--   0        0        0     1651 2023-06-09 04:44:12.805242 python_tldap-1.0.7/tldap/utils.py
+-rw-r--r--   0        0        0     1325 1970-01-01 00:00:00.000000 python_tldap-1.0.7/setup.py
+-rw-r--r--   0        0        0     1566 1970-01-01 00:00:00.000000 python_tldap-1.0.7/PKG-INFO
```

### Comparing `python-tldap-1.0.6/pyproject.toml` & `python_tldap-1.0.7/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-tldap"
-version = "1.0.6"
+version = "1.0.7"
 description = "High level python LDAP Library"
 authors = ["Brian May <brian@linuxpenguins.xyz>"]
 license = "GPL3+"
 packages = [
     { include = "tldap" },
 ]
 readme = "README.rst"
@@ -17,20 +17,22 @@
     "Programming Language :: Python :: 3.6",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 
 [tool.poetry.dependencies]
-python = "^3.8"
+python = "^3.10"
 passlib = "*"
 pyasn1 = "*"
 ldap3 = "*"
 six = "*"
 pip = "*"
+django = {version = "*", optional = true}
+sphinx = {version = "*", optional = true}
 
 [tool.poetry.dev-dependencies]
 pytest = "*"
 mock = "*"
 pytest-runner = "*"
 pytest-bdd = "*"
 pytest-django = "*"
@@ -41,10 +43,13 @@
 twine = "*"
 pipenv-to-requirements = "*"
 pytest-cov = "*"
 isort = "*"
 wheel = "*"
 bumpversion = "*"
 
+[tool.poetry.extras]
+docs = ["sphinx", "django"]
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `python-tldap-1.0.6/tldap/__init__.py` & `python_tldap-1.0.7/tldap/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,8 +26,8 @@
 """
 
 from tldap.query_utils import Q  # noqa: F401
 
 
 __author__ = """Brian May"""
 __email__ = 'brian@linuxpenguins.xyz'
-__version__ = '1.0.6'
+__version__ = '1.0.7'
```

### Comparing `python-tldap-1.0.6/tldap/backend/__init__.py` & `python_tldap-1.0.7/tldap/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `python-tldap-1.0.6/tldap/backend/base.py` & `python_tldap-1.0.7/tldap/backend/base.py`

 * *Files identical despite different names*

### Comparing `python-tldap-1.0.6/tldap/backend/fake_transactions.py` & `python_tldap-1.0.7/tldap/backend/fake_transactions.py`

 * *Files 0% similar despite different names*

```diff
@@ -353,15 +353,15 @@
         """
 
         _debug("rename", self, dn, new_rdn, new_base_dn)
 
         # split up the parameters
         split_dn = tldap.dn.str2dn(dn)
         split_newrdn = tldap.dn.str2dn(new_rdn)
-        assert(len(split_newrdn) == 1)
+        assert (len(split_newrdn) == 1)
 
         # make dn unqualified
         rdn = tldap.dn.dn2str(split_dn[0:1])
 
         # make newrdn fully qualified dn
         tmplist = [split_newrdn[0]]
         if new_base_dn is not None:
```

### Comparing `python-tldap-1.0.6/tldap/backend/no_transactions.py` & `python_tldap-1.0.7/tldap/backend/no_transactions.py`

 * *Files identical despite different names*

### Comparing `python-tldap-1.0.6/tldap/database/__init__.py` & `python_tldap-1.0.7/tldap/database/__init__.py`

 * *Files identical despite different names*

### Comparing `python-tldap-1.0.6/tldap/database/helpers.py` & `python_tldap-1.0.7/tldap/database/helpers.py`

 * *Files identical despite different names*

### Comparing `python-tldap-1.0.6/tldap/dict.py` & `python_tldap-1.0.7/tldap/dict.py`

 * *Files identical despite different names*

### Comparing `python-tldap-1.0.6/tldap/django/__init__.py` & `python_tldap-1.0.7/tldap/django/__init__.py`

 * *Files identical despite different names*

### Comparing `python-tldap-1.0.6/tldap/django/helpers.py` & `python_tldap-1.0.7/tldap/django/helpers.py`

 * *Files identical despite different names*

### Comparing `python-tldap-1.0.6/tldap/django/middleware.py` & `python_tldap-1.0.7/tldap/django/middleware.py`

 * *Files identical despite different names*

### Comparing `python-tldap-1.0.6/tldap/django/migrations/0001_initial.py` & `python_tldap-1.0.7/tldap/django/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `python-tldap-1.0.6/tldap/django/models.py` & `python_tldap-1.0.7/tldap/django/models.py`

 * *Files identical despite different names*

### Comparing `python-tldap-1.0.6/tldap/dn.py` & `python_tldap-1.0.7/tldap/dn.py`

 * *Files 0% similar despite different names*

```diff
@@ -178,15 +178,15 @@
 
 def _descr(value, i):
     return _keystring(value, i)
 
 
 def _UTFMB(value, i):
     if ord(value[i]) >= 0x80:
-        return(value[i], i + 1)
+        return (value[i], i + 1)
 
     return (None, i)
 
 
 # --- RFC 4514: CHARACTERS ---
 
 def _isspecial(value):
```

### Comparing `python-tldap-1.0.6/tldap/exceptions.py` & `python_tldap-1.0.7/tldap/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-tldap-1.0.6/tldap/fields.py` & `python_tldap-1.0.7/tldap/fields.py`

 * *Files identical despite different names*

### Comparing `python-tldap-1.0.6/tldap/filter.py` & `python_tldap-1.0.7/tldap/filter.py`

 * *Files identical despite different names*

### Comparing `python-tldap-1.0.6/tldap/ldap_passwd.py` & `python_tldap-1.0.7/tldap/ldap_passwd.py`

 * *Files identical despite different names*

### Comparing `python-tldap-1.0.6/tldap/modlist.py` & `python_tldap-1.0.7/tldap/modlist.py`

 * *Files identical despite different names*

### Comparing `python-tldap-1.0.6/tldap/query.py` & `python_tldap-1.0.7/tldap/query.py`

 * *Files identical despite different names*

### Comparing `python-tldap-1.0.6/tldap/query_utils.py` & `python_tldap-1.0.7/tldap/query_utils.py`

 * *Files identical despite different names*

### Comparing `python-tldap-1.0.6/tldap/test/__init__.py` & `python_tldap-1.0.7/tldap/test/__init__.py`

 * *Files identical despite different names*

### Comparing `python-tldap-1.0.6/tldap/test/ldap_schemas/00-core.schema` & `python_tldap-1.0.7/tldap/test/ldap_schemas/00-core.schema`

 * *Files identical despite different names*

### Comparing `python-tldap-1.0.6/tldap/test/ldap_schemas/10-cosine.schema` & `python_tldap-1.0.7/tldap/test/ldap_schemas/10-cosine.schema`

 * *Files identical despite different names*

### Comparing `python-tldap-1.0.6/tldap/test/ldap_schemas/50-inetorgperson.schema` & `python_tldap-1.0.7/tldap/test/ldap_schemas/50-inetorgperson.schema`

 * *Files identical despite different names*

### Comparing `python-tldap-1.0.6/tldap/test/ldap_schemas/70-eduperson.schema` & `python_tldap-1.0.7/tldap/test/ldap_schemas/70-eduperson.schema`

 * *Files identical despite different names*

### Comparing `python-tldap-1.0.6/tldap/test/ldap_schemas/90-aueduperson.schema` & `python_tldap-1.0.7/tldap/test/ldap_schemas/90-aueduperson.schema`

 * *Files identical despite different names*

### Comparing `python-tldap-1.0.6/tldap/test/ldap_schemas/90-schac.schema` & `python_tldap-1.0.7/tldap/test/ldap_schemas/90-schac.schema`

 * *Files identical despite different names*

### Comparing `python-tldap-1.0.6/tldap/test/ldap_schemas/nis.schema` & `python_tldap-1.0.7/tldap/test/ldap_schemas/nis.schema`

 * *Files identical despite different names*

### Comparing `python-tldap-1.0.6/tldap/test/slapd.py` & `python_tldap-1.0.7/tldap/test/slapd.py`

 * *Files 3% similar despite different names*

```diff
@@ -76,47 +76,32 @@
     server is shut down.
     """
 
     _log = logging.getLogger("Slapd")
 
     # Use /var/tmp to placate apparmour on Ubuntu:
     TEST_UTILS_DIR = os.path.abspath(os.path.split(__file__)[0])
-    PATH_SBIN_DIR = "/usr/sbin"
-    PATH_BIN_DIR = "/usr/bin"
     PATH_SCHEMA_DIR = TEST_UTILS_DIR + "/ldap_schemas/"
-    PATH_LDAPADD = os.path.join(PATH_BIN_DIR, "ldapadd")
-    PATH_LDAPSEARCH = os.path.join(PATH_BIN_DIR, "ldapsearch")
-    PATH_SLAPD = os.path.join(PATH_SBIN_DIR, "slapd")
-    PATH_SLAP_TEST = os.path.join(PATH_SBIN_DIR, "slaptest")
-
-    @classmethod
-    def check_paths(cls) -> None:
-        """
-        Checks that the configured executable paths look valid.
-        If they don't, then logs warning messages (not errors).
-        """
-        for name, path in (
-                ("slapd", cls.PATH_SLAPD),
-                ("ldapadd", cls.PATH_LDAPADD),
-                ("ldapsearch", cls.PATH_LDAPSEARCH),
-        ):
-            cls._log.debug("checking %s executable at %s", name, path)
-            if not os.access(path, os.X_OK):
-                cls._log.warning("cannot find %s executable at %s", name, path)
+    PATH_LDAPADD = "ldapadd"
+    PATH_LDAPSEARCH = "ldapsearch"
+    PATH_SLAPD = "slapd"
+    PATH_SLAP_TEST = "slaptest"
 
     def __init__(self) -> None:
         self._proc = None
         self._proc_config: Optional[str] = None
         self._port: int = 0
         self._tmpdir: Optional[str] = None
         self._dn_suffix: str = "dc=python-ldap,dc=org"
         self._root_cn: str = "Manager"
         self._root_password: str = "password"
         self._slapd_debug_level: int or str = 0
-        self._env: Dict[str, str] = {}
+        self._env: Dict[str, str] = {
+            'PATH': os.getenv('PATH')
+        }
 
     # Setters
     def set_port(self, port: int) -> None:
         self._port = port
 
     def set_dn_suffix(self, dn: str) -> None:
         self._dn_suffix = dn
@@ -249,15 +234,15 @@
             f.write("\n")
             f.write(f'dn: ou=Groups,{self.get_dn_suffix()}\n')
             f.write('objectClass: top\n')
             f.write('objectClass: OrganizationalUnit\n')
             f.write('ou: Groups\n')
 
         config_path = os.path.join(self._tmpdir, "slapd.conf")
-        subprocess.check_call(["/usr/sbin/slapadd", "-n", "1", "-f", config_path, "-l", p])
+        subprocess.check_call(["slapadd", "-n", "1", "-f", config_path, "-l", p])
 
     def start(self) -> None:
         """
         Starts the slapd server process running, and waits for it to come up.
         """
         if self._proc is None:
             ok = False
@@ -445,17 +430,14 @@
                 else:
                     raise RuntimeError("bad line: " + repr(line))
                 obj.append((attr, value))
         assert obj == []
         return objects
 
 
-Slapd.check_paths()
-
-
 def test() -> None:
     logging.basicConfig(level=logging.DEBUG)
     slapd = Slapd()
     try:
         print("Starting slapd...")
         slapd.start()
```

### Comparing `python-tldap-1.0.6/tldap/transaction.py` & `python_tldap-1.0.7/tldap/transaction.py`

 * *Files identical despite different names*

### Comparing `python-tldap-1.0.6/tldap/tree.py` & `python_tldap-1.0.7/tldap/tree.py`

 * *Files identical despite different names*

### Comparing `python-tldap-1.0.6/tldap/utils.py` & `python_tldap-1.0.7/tldap/utils.py`

 * *Files identical despite different names*

### Comparing `python-tldap-1.0.6/setup.py` & `python_tldap-1.0.7/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,25 +11,29 @@
 
 package_data = \
 {'': ['*'], 'tldap.test': ['ldap_schemas/*']}
 
 install_requires = \
 ['ldap3', 'passlib', 'pip', 'pyasn1', 'six']
 
+extras_require = \
+{'docs': ['django', 'sphinx']}
+
 setup_kwargs = {
     'name': 'python-tldap',
-    'version': '1.0.6',
+    'version': '1.0.7',
     'description': 'High level python LDAP Library',
     'long_description': 'python-tldap\n============\nTLDAP is a high level LDAP library for Python that uses Ecto like models\nto define LDAP schemas that can then be used in an easy way from Python code.\nIt also supports fake LDAP transactions, to try and ensure LDAP database\nremains in a consistent state, even if there are errors that cause the\ntransaction to fail.\n\nDocumentation can be found at http://python-tldap.readthedocs.org/\n',
     'author': 'Brian May',
     'author_email': 'brian@linuxpenguins.xyz',
-    'maintainer': None,
-    'maintainer_email': None,
+    'maintainer': 'None',
+    'maintainer_email': 'None',
     'url': 'https://github.com/Karaage-Cluster/python-tldap/',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
+    'extras_require': extras_require,
+    'python_requires': '>=3.10,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `python-tldap-1.0.6/PKG-INFO` & `python_tldap-1.0.7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 Metadata-Version: 2.1
 Name: python-tldap
-Version: 1.0.6
+Version: 1.0.7
 Summary: High level python LDAP Library
 Home-page: https://github.com/Karaage-Cluster/python-tldap/
 License: GPL3+
 Author: Brian May
 Author-email: brian@linuxpenguins.xyz
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Provides-Extra: docs
+Requires-Dist: django ; extra == "docs"
 Requires-Dist: ldap3
 Requires-Dist: passlib
 Requires-Dist: pip
 Requires-Dist: pyasn1
 Requires-Dist: six
+Requires-Dist: sphinx ; extra == "docs"
 Description-Content-Type: text/x-rst
 
 python-tldap
 ============
 TLDAP is a high level LDAP library for Python that uses Ecto like models
 to define LDAP schemas that can then be used in an easy way from Python code.
 It also supports fake LDAP transactions, to try and ensure LDAP database
```

