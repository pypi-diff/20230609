# Comparing `tmp/iso8601-1.1.0.tar.gz` & `tmp/iso8601-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iso8601-1.1.0.tar", max compression
+gzip compressed data, was "iso8601-2.0.0.tar", max compression
```

## Comparing `iso8601-1.1.0.tar` & `iso8601-2.0.0.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0     1065 2022-03-30 22:44:41.610741 iso8601-1.1.0/LICENSE
--rw-r--r--   0        0        0     9113 2022-09-28 14:50:42.283353 iso8601-1.1.0/README.rst
--rw-r--r--   0        0        0      150 2022-09-28 14:04:26.063839 iso8601-1.1.0/iso8601/__init__.py
--rw-r--r--   0        0        0     4992 2022-09-28 14:04:26.064168 iso8601-1.1.0/iso8601/iso8601.py
--rw-r--r--   0        0        0        0 2021-11-22 12:31:16.712773 iso8601-1.1.0/iso8601/py.typed
--rw-r--r--   0        0        0    10523 2022-09-28 14:04:26.064644 iso8601-1.1.0/iso8601/test_iso8601.py
--rw-r--r--   0        0        0      699 2022-09-28 14:50:42.285734 iso8601-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     9947 1970-01-01 00:00:00.000000 iso8601-1.1.0/setup.py
--rw-r--r--   0        0        0     9838 1970-01-01 00:00:00.000000 iso8601-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-06-09 10:05:40.425387 iso8601-2.0.0/LICENSE
+-rw-r--r--   0        0        0     2850 2023-06-09 11:05:35.700732 iso8601-2.0.0/README.rst
+-rw-r--r--   0        0        0      150 2023-01-23 10:49:49.290292 iso8601-2.0.0/iso8601/__init__.py
+-rw-r--r--   0        0        0     4992 2023-01-23 10:49:49.290507 iso8601-2.0.0/iso8601/iso8601.py
+-rw-r--r--   0        0        0        0 2023-01-23 10:49:49.290602 iso8601-2.0.0/iso8601/py.typed
+-rw-r--r--   0        0        0    10608 2023-06-09 11:05:35.703680 iso8601-2.0.0/iso8601/test_iso8601.py
+-rw-r--r--   0        0        0      727 2023-06-09 11:08:54.219186 iso8601-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     3624 1970-01-01 00:00:00.000000 iso8601-2.0.0/PKG-INFO
```

### Comparing `iso8601-1.1.0/LICENSE` & `iso8601-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `iso8601-1.1.0/iso8601/iso8601.py` & `iso8601-2.0.0/iso8601/iso8601.py`

 * *Files identical despite different names*

### Comparing `iso8601-1.1.0/iso8601/test_iso8601.py` & `iso8601-2.0.0/iso8601/test_iso8601.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,16 @@
 
 def test_iso8601_regex() -> None:
     assert iso8601.ISO8601_REGEX.match("2006-10-11T00:14:33Z")
 
 
 def test_fixedoffset_eq() -> None:
     # See https://bitbucket.org/micktwomey/pyiso8601/issues/19
-    datetime.tzinfo() == iso8601.FixedOffset(2, 0, "+2:00")
+    expected_timezone = datetime.timezone(offset=datetime.timedelta(hours=2))
+    assert expected_timezone == iso8601.FixedOffset(2, 0, "+2:00")
 
 
 def test_parse_no_timezone_different_default() -> None:
     tz = iso8601.FixedOffset(2, 0, "test offset")
     d = iso8601.parse_date("2007-01-01T08:00:00", default_timezone=tz)
     assert d == datetime.datetime(2007, 1, 1, 8, 0, 0, 0, tz)
     assert d.tzinfo == tz
```

### Comparing `iso8601-1.1.0/pyproject.toml` & `iso8601-2.0.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 [tool.poetry]
 name = "iso8601"
-version = "1.1.0"
+version = "2.0.0"
 description = "Simple module to parse ISO 8601 dates"
 authors = ["Michael Twomey <mick@twomeylee.name>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/micktwomey/pyiso8601"
 repository = "https://github.com/micktwomey/pyiso8601"
 documentation = "https://pyiso8601.readthedocs.io/en/latest/"
 
 [tool.poetry.dependencies]
-python = ">=3.6.2,<4.0"
+python = ">=3.7,<4.0"
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
 mypy = "*"
 black = "*"
 pylint = "*"
 isort = "*"
 pytest = "*"
 hypothesis = "*"
 pytz = "*"
 pre-commit = "*"
 nox = "*"
 Sphinx = "*"
+changelog-manager = "*"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
 profile = "black"
```

