# Comparing `tmp/pytest_mock_resources-2.6.9.tar.gz` & `tmp/pytest_mock_resources-2.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_mock_resources-2.6.9.tar", max compression
+gzip compressed data, was "pytest_mock_resources-2.7.0.tar", max compression
```

## Comparing `pytest_mock_resources-2.6.9.tar` & `pytest_mock_resources-2.7.0.tar`

### file list

```diff
@@ -1,40 +1,43 @@
--rw-r--r--   0        0        0    10711 2023-02-24 19:01:47.425129 pytest_mock_resources-2.6.9/CHANGELOG.md
--rw-r--r--   0        0        0     1053 2023-02-24 19:01:47.425129 pytest_mock_resources-2.6.9/LICENSE
--rw-r--r--   0        0        0     5549 2023-02-24 19:01:47.425129 pytest_mock_resources-2.6.9/README.md
--rw-r--r--   0        0        0     3597 2023-02-24 19:01:47.429129 pytest_mock_resources-2.6.9/pyproject.toml
--rw-r--r--   0        0        0     1752 2023-02-24 19:01:47.429129 pytest_mock_resources-2.6.9/src/pytest_mock_resources/__init__.py
--rw-r--r--   0        0        0     2771 2023-02-24 19:01:47.429129 pytest_mock_resources-2.6.9/src/pytest_mock_resources/cli.py
--rw-r--r--   0        0        0     1867 2023-02-24 19:01:47.429129 pytest_mock_resources-2.6.9/src/pytest_mock_resources/compat/__init__.py
--rw-r--r--   0        0        0      822 2023-02-24 19:01:47.429129 pytest_mock_resources-2.6.9/src/pytest_mock_resources/compat/import_.py
--rw-r--r--   0        0        0      923 2023-02-24 19:01:47.429129 pytest_mock_resources-2.6.9/src/pytest_mock_resources/compat/sqlalchemy.py
--rw-r--r--   0        0        0     2687 2023-02-24 19:01:47.429129 pytest_mock_resources-2.6.9/src/pytest_mock_resources/config.py
--rw-r--r--   0        0        0      400 2023-02-24 19:01:47.429129 pytest_mock_resources-2.6.9/src/pytest_mock_resources/container/__init__.py
--rw-r--r--   0        0        0     6429 2023-02-24 19:01:47.429129 pytest_mock_resources-2.6.9/src/pytest_mock_resources/container/base.py
--rw-r--r--   0        0        0     1702 2023-02-24 19:01:47.429129 pytest_mock_resources-2.6.9/src/pytest_mock_resources/container/mongo.py
--rw-r--r--   0        0        0     1402 2023-02-24 19:01:47.429129 pytest_mock_resources-2.6.9/src/pytest_mock_resources/container/moto.py
--rw-r--r--   0        0        0     2792 2023-02-24 19:01:47.429129 pytest_mock_resources-2.6.9/src/pytest_mock_resources/container/mysql.py
--rw-r--r--   0        0        0     3716 2023-02-24 19:01:47.429129 pytest_mock_resources-2.6.9/src/pytest_mock_resources/container/postgres.py
--rw-r--r--   0        0        0     1369 2023-02-24 19:01:47.429129 pytest_mock_resources-2.6.9/src/pytest_mock_resources/container/redis.py
--rw-r--r--   0        0        0     1569 2023-02-24 19:01:47.429129 pytest_mock_resources-2.6.9/src/pytest_mock_resources/container/redshift.py
--rw-r--r--   0        0        0     3070 2023-02-24 19:01:47.429129 pytest_mock_resources-2.6.9/src/pytest_mock_resources/credentials.py
--rw-r--r--   0        0        0     1430 2023-02-24 19:01:47.429129 pytest_mock_resources-2.6.9/src/pytest_mock_resources/fixture/__init__.py
--rw-r--r--   0        0        0      750 2023-02-24 19:01:47.429129 pytest_mock_resources-2.6.9/src/pytest_mock_resources/fixture/base.py
--rw-r--r--   0        0        0     2364 2023-02-24 19:01:47.429129 pytest_mock_resources-2.6.9/src/pytest_mock_resources/fixture/mongo.py
--rw-r--r--   0        0        0     4134 2023-02-24 19:01:47.429129 pytest_mock_resources-2.6.9/src/pytest_mock_resources/fixture/moto.py
--rw-r--r--   0        0        0     3339 2023-02-24 19:01:47.429129 pytest_mock_resources-2.6.9/src/pytest_mock_resources/fixture/mysql.py
--rw-r--r--   0        0        0    10940 2023-02-24 19:01:47.429129 pytest_mock_resources-2.6.9/src/pytest_mock_resources/fixture/postgresql.py
--rw-r--r--   0        0        0     2714 2023-02-24 19:01:47.429129 pytest_mock_resources-2.6.9/src/pytest_mock_resources/fixture/redis.py
--rw-r--r--   0        0        0     4596 2023-02-24 19:01:47.429129 pytest_mock_resources-2.6.9/src/pytest_mock_resources/fixture/redshift/__init__.py
--rw-r--r--   0        0        0     4939 2023-02-24 19:01:47.429129 pytest_mock_resources-2.6.9/src/pytest_mock_resources/fixture/redshift/udf.py
--rw-r--r--   0        0        0     8958 2023-02-24 19:01:47.429129 pytest_mock_resources-2.6.9/src/pytest_mock_resources/fixture/sqlite.py
--rw-r--r--   0        0        0     3724 2023-02-24 19:01:47.429129 pytest_mock_resources-2.6.9/src/pytest_mock_resources/hooks.py
--rw-r--r--   0        0        0        0 2023-02-24 19:01:47.429129 pytest_mock_resources-2.6.9/src/pytest_mock_resources/patch/__init__.py
--rw-r--r--   0        0        0        0 2023-02-24 19:01:47.429129 pytest_mock_resources-2.6.9/src/pytest_mock_resources/patch/redshift/__init__.py
--rw-r--r--   0        0        0     7054 2023-02-24 19:01:47.429129 pytest_mock_resources-2.6.9/src/pytest_mock_resources/patch/redshift/mock_s3_copy.py
--rw-r--r--   0        0        0     7286 2023-02-24 19:01:47.429129 pytest_mock_resources-2.6.9/src/pytest_mock_resources/patch/redshift/mock_s3_unload.py
--rw-r--r--   0        0        0     2486 2023-02-24 19:01:47.429129 pytest_mock_resources-2.6.9/src/pytest_mock_resources/patch/redshift/psycopg2.py
--rw-r--r--   0        0        0     2905 2023-02-24 19:01:47.429129 pytest_mock_resources-2.6.9/src/pytest_mock_resources/patch/redshift/sqlalchemy.py
--rw-r--r--   0        0        0        0 2023-02-24 19:01:47.429129 pytest_mock_resources-2.6.9/src/pytest_mock_resources/py.typed
--rw-r--r--   0        0        0    10230 2023-02-24 19:01:47.429129 pytest_mock_resources-2.6.9/src/pytest_mock_resources/sqlalchemy.py
--rw-r--r--   0        0        0     7867 1970-01-01 00:00:00.000000 pytest_mock_resources-2.6.9/setup.py
--rw-r--r--   0        0        0     7788 1970-01-01 00:00:00.000000 pytest_mock_resources-2.6.9/PKG-INFO
+-rw-r--r--   0        0        0    15317 2023-06-09 13:02:20.155211 pytest_mock_resources-2.7.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1053 2023-06-09 13:02:20.155211 pytest_mock_resources-2.7.0/LICENSE
+-rw-r--r--   0        0        0     5549 2023-06-09 13:02:20.155211 pytest_mock_resources-2.7.0/README.md
+-rw-r--r--   0        0        0     3597 2023-06-09 13:02:20.155211 pytest_mock_resources-2.7.0/pyproject.toml
+-rw-r--r--   0        0        0     1846 2023-06-09 13:02:20.155211 pytest_mock_resources-2.7.0/src/pytest_mock_resources/__init__.py
+-rw-r--r--   0        0        0     1305 2023-06-09 13:02:20.155211 pytest_mock_resources-2.7.0/src/pytest_mock_resources/action.py
+-rw-r--r--   0        0        0     2173 2023-06-09 13:02:20.155211 pytest_mock_resources-2.7.0/src/pytest_mock_resources/cli.py
+-rw-r--r--   0        0        0     1867 2023-06-09 13:02:20.159211 pytest_mock_resources-2.7.0/src/pytest_mock_resources/compat/__init__.py
+-rw-r--r--   0        0        0      822 2023-06-09 13:02:20.159211 pytest_mock_resources-2.7.0/src/pytest_mock_resources/compat/import_.py
+-rw-r--r--   0        0        0      923 2023-06-09 13:02:20.159211 pytest_mock_resources-2.7.0/src/pytest_mock_resources/compat/sqlalchemy.py
+-rw-r--r--   0        0        0     3013 2023-06-09 13:02:20.159211 pytest_mock_resources-2.7.0/src/pytest_mock_resources/config.py
+-rw-r--r--   0        0        0      622 2023-06-09 13:02:20.159211 pytest_mock_resources-2.7.0/src/pytest_mock_resources/container/__init__.py
+-rw-r--r--   0        0        0     6429 2023-06-09 13:02:20.159211 pytest_mock_resources-2.7.0/src/pytest_mock_resources/container/base.py
+-rw-r--r--   0        0        0     1702 2023-06-09 13:02:20.159211 pytest_mock_resources-2.7.0/src/pytest_mock_resources/container/mongo.py
+-rw-r--r--   0        0        0     1399 2023-06-09 13:02:20.159211 pytest_mock_resources-2.7.0/src/pytest_mock_resources/container/moto.py
+-rw-r--r--   0        0        0     2792 2023-06-09 13:02:20.159211 pytest_mock_resources-2.7.0/src/pytest_mock_resources/container/mysql.py
+-rw-r--r--   0        0        0     3713 2023-06-09 13:02:20.159211 pytest_mock_resources-2.7.0/src/pytest_mock_resources/container/postgres.py
+-rw-r--r--   0        0        0     1369 2023-06-09 13:02:20.159211 pytest_mock_resources-2.7.0/src/pytest_mock_resources/container/redis.py
+-rw-r--r--   0        0        0     1569 2023-06-09 13:02:20.159211 pytest_mock_resources-2.7.0/src/pytest_mock_resources/container/redshift.py
+-rw-r--r--   0        0        0     3070 2023-06-09 13:02:20.159211 pytest_mock_resources-2.7.0/src/pytest_mock_resources/credentials.py
+-rw-r--r--   0        0        0     1490 2023-06-09 13:02:20.159211 pytest_mock_resources-2.7.0/src/pytest_mock_resources/fixture/__init__.py
+-rw-r--r--   0        0        0      750 2023-06-09 13:02:20.159211 pytest_mock_resources-2.7.0/src/pytest_mock_resources/fixture/base.py
+-rw-r--r--   0        0        0     2364 2023-06-09 13:02:20.159211 pytest_mock_resources-2.7.0/src/pytest_mock_resources/fixture/mongo.py
+-rw-r--r--   0        0        0      406 2023-06-09 13:02:20.159211 pytest_mock_resources-2.7.0/src/pytest_mock_resources/fixture/moto/__init__.py
+-rw-r--r--   0        0        0     1960 2023-06-09 13:02:20.159211 pytest_mock_resources-2.7.0/src/pytest_mock_resources/fixture/moto/action.py
+-rw-r--r--   0        0        0     4438 2023-06-09 13:02:20.159211 pytest_mock_resources-2.7.0/src/pytest_mock_resources/fixture/moto/base.py
+-rw-r--r--   0        0        0     3417 2023-06-09 13:02:20.159211 pytest_mock_resources-2.7.0/src/pytest_mock_resources/fixture/mysql.py
+-rw-r--r--   0        0        0    11154 2023-06-09 13:02:20.159211 pytest_mock_resources-2.7.0/src/pytest_mock_resources/fixture/postgresql.py
+-rw-r--r--   0        0        0     2714 2023-06-09 13:02:20.159211 pytest_mock_resources-2.7.0/src/pytest_mock_resources/fixture/redis.py
+-rw-r--r--   0        0        0     4658 2023-06-09 13:02:20.159211 pytest_mock_resources-2.7.0/src/pytest_mock_resources/fixture/redshift/__init__.py
+-rw-r--r--   0        0        0     4939 2023-06-09 13:02:20.159211 pytest_mock_resources-2.7.0/src/pytest_mock_resources/fixture/redshift/udf.py
+-rw-r--r--   0        0        0     9051 2023-06-09 13:02:20.159211 pytest_mock_resources-2.7.0/src/pytest_mock_resources/fixture/sqlite.py
+-rw-r--r--   0        0        0     3813 2023-06-09 13:02:20.159211 pytest_mock_resources-2.7.0/src/pytest_mock_resources/hooks.py
+-rw-r--r--   0        0        0        0 2023-06-09 13:02:20.159211 pytest_mock_resources-2.7.0/src/pytest_mock_resources/patch/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-09 13:02:20.159211 pytest_mock_resources-2.7.0/src/pytest_mock_resources/patch/redshift/__init__.py
+-rw-r--r--   0        0        0     7054 2023-06-09 13:02:20.159211 pytest_mock_resources-2.7.0/src/pytest_mock_resources/patch/redshift/mock_s3_copy.py
+-rw-r--r--   0        0        0     7286 2023-06-09 13:02:20.159211 pytest_mock_resources-2.7.0/src/pytest_mock_resources/patch/redshift/mock_s3_unload.py
+-rw-r--r--   0        0        0     2486 2023-06-09 13:02:20.159211 pytest_mock_resources-2.7.0/src/pytest_mock_resources/patch/redshift/psycopg2.py
+-rw-r--r--   0        0        0     2905 2023-06-09 13:02:20.159211 pytest_mock_resources-2.7.0/src/pytest_mock_resources/patch/redshift/sqlalchemy.py
+-rw-r--r--   0        0        0        0 2023-06-09 13:02:20.159211 pytest_mock_resources-2.7.0/src/pytest_mock_resources/py.typed
+-rw-r--r--   0        0        0    10187 2023-06-09 13:02:20.159211 pytest_mock_resources-2.7.0/src/pytest_mock_resources/sqlalchemy.py
+-rw-r--r--   0        0        0     7906 1970-01-01 00:00:00.000000 pytest_mock_resources-2.7.0/setup.py
+-rw-r--r--   0        0        0     7788 1970-01-01 00:00:00.000000 pytest_mock_resources-2.7.0/PKG-INFO
```

### Comparing `pytest_mock_resources-2.6.9/CHANGELOG.md` & `pytest_mock_resources-2.7.0/CHANGELOG.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,135 @@
 # Changelog
 
-## [Unreleased](https://github.com/schireson/pytest-mock-resources/compare/v2.5.0...HEAD) (2022-09-15)
+## [Unreleased](https://github.com/schireson/pytest-mock-resources/compare/v2.6.13...HEAD) (2023-05-31)
+
+### Features
+
+* Implement moto "ordered actions" for declaring a specific bucket state.
+  ([e7efece](https://github.com/schireson/pytest-mock-resources/commit/e7efece534178a70d1f1b4bcd11985a88003b92a))
+
+### [v2.6.13](https://github.com/schireson/pytest-mock-resources/compare/v2.6.12...v2.6.13) (2023-05-23)
+
+#### Fixes
+
+* Increase time to wait for mysql to spin up. (#190)
+  ([5d94aea](https://github.com/schireson/pytest-mock-resources/commit/5d94aeaf93576d2009f0da3568e0a84e0183f7bc))
+
+### [v2.6.12](https://github.com/schireson/pytest-mock-resources/compare/v2.6.11...v2.6.12) (2023-05-03)
+
+#### Features
+
+* Ensure all fixture types are automatically included in the CLI. (#189)
+  ([df55dde](https://github.com/schireson/pytest-mock-resources/commit/df55dde5281d544bd114ccbaab939932a185a173))
+
+### [v2.6.11](https://github.com/schireson/pytest-mock-resources/compare/v2.6.10...v2.6.11) (2023-03-03)
+
+#### Fixes
+
+* Deal with port as given by an env var, which might be a string. (#186)
+  ([b4ae4e7](https://github.com/schireson/pytest-mock-resources/commit/b4ae4e71c6f8ba7cfa0016f0f17292a879a3a470))
+
+### [v2.6.10](https://github.com/schireson/pytest-mock-resources/compare/v2.6.9...v2.6.10) (2023-02-24)
+
+#### Fixes
+
+* Only set AUTOCOMMIT isolation level during internal fixture setup which requires  
+it.
+  ([fd8d313](https://github.com/schireson/pytest-mock-resources/commit/fd8d313f82aa92fd3d34135e25fc3b74603c9ea5))
+
+### [v2.6.9](https://github.com/schireson/pytest-mock-resources/compare/v2.6.8...v2.6.9) (2023-02-24)
+
+#### Fixes
+
+* Ensure connection gets closed and is compatible with asyncpg. (#184)
+  ([4cc1847](https://github.com/schireson/pytest-mock-resources/commit/4cc184748ed585533694145bf5fabc9ba1b8ce97))
+
+### [v2.6.8](https://github.com/schireson/pytest-mock-resources/compare/v2.6.7...v2.6.8) (2023-02-23)
+
+#### Fixes
+
+* Avoid psycopg2 dependency during the execution of create_postgre… (#183)
+  ([ed488f5](https://github.com/schireson/pytest-mock-resources/commit/ed488f5272e4a1452b1616b89e7c89bba3e6175c))
+
+### [v2.6.7](https://github.com/schireson/pytest-mock-resources/compare/v2.6.6...v2.6.7) (2023-01-19)
+
+#### Fixes
+
+* Remove reliance on undeclared attrs dependency. (#180)
+  ([ac96d42](https://github.com/schireson/pytest-mock-resources/commit/ac96d422cebf78dd511e99e9c45f84298ab4fe95))
+
+### [v2.6.6](https://github.com/schireson/pytest-mock-resources/compare/v2.6.5...v2.6.6) (2023-01-13)
+
+#### Features
+
+* Add engine_kwargs argument to mysql fixture. (#178)
+  ([d522be8](https://github.com/schireson/pytest-mock-resources/commit/d522be82cd3a08b886fb504429b315f30d7280eb))
+
+### [v2.6.5](https://github.com/schireson/pytest-mock-resources/compare/v2.6.4...v2.6.5) (2022-12-27)
+
+#### Fixes
+
+* Address compatibilities with sqlalchemy 2. (#176)
+  ([0415c78](https://github.com/schireson/pytest-mock-resources/commit/0415c7841e439d4120685f7ac995b346e2ab94b9))
+
+### [v2.6.4](https://github.com/schireson/pytest-mock-resources/compare/v2.6.3...v2.6.4) (2022-12-21)
+
+#### Fixes
+
+* Move port selection into the filelock. (#174)
+  ([76c7ed3](https://github.com/schireson/pytest-mock-resources/commit/76c7ed37cb2c6c63e979b881eac6f820ee07eaf5))
+
+### [v2.6.3](https://github.com/schireson/pytest-mock-resources/compare/v2.6.1...v2.6.3) (2022-10-27)
+
+#### Fixes
+
+* Decide on behavior support for multiple redshift statements. (#172)
+  ([e9d5f0f](https://github.com/schireson/pytest-mock-resources/commit/e9d5f0f9d63cb27052bea2ea2d75186623c55f39))
+
+### [v2.6.1](https://github.com/schireson/pytest-mock-resources/compare/v2.6.0...v2.6.1) (2022-10-20)
+
+#### Fixes
+
+* Fix redshift event listener interaction with the session keyword. (#171)
+  ([088b180](https://github.com/schireson/pytest-mock-resources/commit/088b1800948d131a44236c57154e062dfb9cc7b2))
+
+## [v2.6.0](https://github.com/schireson/pytest-mock-resources/compare/v2.5.1...v2.6.0) (2022-10-07)
+
+### Features
+
+* Add support for moto as a fixture. (#169)
+  ([d405c7d](https://github.com/schireson/pytest-mock-resources/commit/d405c7d4739d4d1fc4ed5fe6d41f53472deee214))
 
 ### Fixes
 
-* async engine bug related to engine reuse in a different async loop.
-  ([5135031](https://github.com/schireson/pytest-mock-resources/commit/5135031b0f8d83957b9c899331a85251d459a0ba))
+* Docs build. (#168)
+  ([ee6ea37](https://github.com/schireson/pytest-mock-resources/commit/ee6ea371619ae3ab6b2279495cf421f72d39bdd9))
+
+### [v2.5.1](https://github.com/schireson/pytest-mock-resources/compare/v2.5.0...v2.5.1) (2022-09-16)
 
-## [v2.5.0](https://github.com/schireson/pytest-mock-resources/compare/v2.4.4...v2.5.0) (2022-08-24)
+#### Fixes
+
+* async engine bug related to engine reuse in a different async loop. (#166)
+  ([3254bd8](https://github.com/schireson/pytest-mock-resources/commit/3254bd8f30fd9bd4c435f27c0995a747cc8d5691))
+
+## [v2.5.0](https://github.com/schireson/pytest-mock-resources/compare/v2.4.5...v2.5.0) (2022-08-24)
 
 ### Fixes
 
 * Address incompatibility with strict mode for pytest-asyncio in 0.17.0 and  
 beyond.
   ([ead7243](https://github.com/schireson/pytest-mock-resources/commit/ead724376c398cd25c46acb2578d3b05b53aba16))
 
+### [v2.4.5](https://github.com/schireson/pytest-mock-resources/compare/v2.4.4...v2.4.5) (2022-09-15)
+
+#### Fixes
+
+* async engine bug related to engine reuse in a different async loop.
+  ([15cab91](https://github.com/schireson/pytest-mock-resources/commit/15cab91003f76b6dd3109489b338ea0d46851ed1))
+
 ### [v2.4.4](https://github.com/schireson/pytest-mock-resources/compare/v2.4.3...v2.4.4) (2022-08-12)
 
 ### [v2.4.3](https://github.com/schireson/pytest-mock-resources/compare/v2.4.2...v2.4.3) (2022-07-20)
 
 ### [v2.4.2](https://github.com/schireson/pytest-mock-resources/compare/v2.4.1...v2.4.2) (2022-07-14)
 
 #### Fixes
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pytest_mock_resources-2.6.9/LICENSE` & `pytest_mock_resources-2.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_mock_resources-2.6.9/README.md` & `pytest_mock_resources-2.7.0/README.md`

 * *Files identical despite different names*

### Comparing `pytest_mock_resources-2.6.9/pyproject.toml` & `pytest_mock_resources-2.7.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pytest-mock-resources"
-version = "2.6.9"
+version = "2.7.0"
 description = "A pytest plugin for easily instantiating reproducible mock resources."
 authors = [
     "Omar Khan <oakhan3@gmail.com>",
     "Dan Cardin <ddcardin@gmail.com>",
     "Gabriel Michael <gabriel.j.michael@gmail.com>",
     "Prateek Pisat <pisatprateek12@gmail.com>",
 ]
```

### Comparing `pytest_mock_resources-2.6.9/src/pytest_mock_resources/__init__.py` & `pytest_mock_resources-2.7.0/src/pytest_mock_resources/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from pytest_mock_resources.container import (
     get_container,
     MongoConfig,
+    MotoConfig,
     MysqlConfig,
     PostgresConfig,
     RedisConfig,
     RedshiftConfig,
 )
 from pytest_mock_resources.credentials import Credentials
 from pytest_mock_resources.fixture import (
@@ -24,33 +25,38 @@
     pmr_mysql_container,
     pmr_postgres_config,
     pmr_postgres_container,
     pmr_redis_config,
     pmr_redis_container,
     pmr_redshift_config,
     pmr_redshift_container,
+    S3Bucket,
+    S3Object,
 )
 from pytest_mock_resources.hooks import (  # noqa
     pytest_addoption,
     pytest_configure,
     pytest_itemcollected,
     pytest_sessionfinish,
 )
 from pytest_mock_resources.sqlalchemy import Rows, Statements, StaticStatements
 
 __all__ = [
     "Credentials",
     "MongoConfig",
+    "MotoConfig",
     "MysqlConfig",
     "PostgresConfig",
     "RedisConfig",
     "RedshiftConfig",
     "Rows",
     "Statements",
     "StaticStatements",
+    "S3Bucket",
+    "S3Object",
     "create_mongo_fixture",
     "create_moto_fixture",
     "create_mysql_fixture",
     "create_postgres_fixture",
     "create_redis_fixture",
     "create_redshift_fixture",
     "create_sqlite_fixture",
```

### Comparing `pytest_mock_resources-2.6.9/src/pytest_mock_resources/cli.py` & `pytest_mock_resources-2.7.0/src/pytest_mock_resources/cli.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,108 +1,81 @@
+from __future__ import annotations
+
 import argparse
-import enum
-from typing import Dict, Type
 
-from pytest_mock_resources import (
-    MongoConfig,
-    MysqlConfig,
-    PostgresConfig,
-    RedisConfig,
-    RedshiftConfig,
-)
 from pytest_mock_resources.config import DockerContainerConfig
 from pytest_mock_resources.container.base import container_name, get_container
 
-postgres_image = PostgresConfig().image
-mysql_image = MysqlConfig().image
-mongo_image = MongoConfig().image
-
 
 class StubPytestConfig:
     pmr_multiprocess_safe = False
     pmr_cleanup_container = False
 
     class option:
         pmr_multiprocess_safe = False
         pmr_cleanup_container = False
 
     def getini(self, attr):
         return getattr(self, attr)
 
 
-@enum.unique
-class FixtureType(enum.Enum):
-    mongo = "mongo"
-    mysql = "mysql"
-    postgres = "postgres"
-    redis = "redis"
-    redshift = "redshift"
-
-    @classmethod
-    def options(cls):
-        return ", ".join(fixture_base.value for fixture_base in cls)
-
-
-_container_producers: Dict[FixtureType, Type[DockerContainerConfig]] = {
-    FixtureType.mongo: MongoConfig,
-    FixtureType.mysql: MysqlConfig,
-    FixtureType.postgres: PostgresConfig,
-    FixtureType.redis: RedisConfig,
-    FixtureType.redshift: RedshiftConfig,
-}
-
-
 def main():
     parser = create_parser()
     args = parser.parse_args()
 
     pytestconfig = StubPytestConfig()
 
     stop = args.stop
     start = not stop
 
-    for fixture_base in args.fixture_bases:
-        fixture_type = FixtureType(fixture_base)
-        execute(fixture_type, pytestconfig, start=start, stop=stop)
+    for fixture in args.fixtures:
+        if fixture not in DockerContainerConfig.subclasses:
+            valid_options = ", ".join(DockerContainerConfig.subclasses)
+            raise argparse.ArgumentError(
+                args.fixtures,
+                f"'{fixture}' invalid. Valid options include: {valid_options}",
+            )
+
+        execute(fixture, pytestconfig, start=start, stop=stop)
 
 
 def create_parser():
-    # TODO: Add an options arg to DOWN a fixture_base's container
     parser = argparse.ArgumentParser(
         description="Premptively run docker containers to speed up initial startup of PMR Fixtures."
     )
     parser.add_argument(
-        "fixture_bases",
-        metavar="Fixture Base",
+        "fixtures",
+        metavar="Fixture",
         type=str,
         nargs="+",
-        help="Available Fixture Bases: {}".format(FixtureType.options()),
+        help="Available Fixtures: {}".format(", ".join(DockerContainerConfig.subclasses)),
     )
     parser.add_argument(
         "--stop", action="store_true", help="Stop previously started PMR containers"
     )
     return parser
 
 
-def execute(fixture_type: FixtureType, pytestconfig: StubPytestConfig, start=True, stop=False):
-    config_cls = _container_producers[fixture_type]
+def execute(fixture: str, pytestconfig: StubPytestConfig, start=True, stop=False):
+    config_cls = DockerContainerConfig.subclasses[fixture]
     config = config_cls()
 
     if start:
         generator = get_container(pytestconfig, config)
         for _ in generator:
             pass
 
     if stop:
         from python_on_whales import docker
 
-        name = container_name(fixture_type.value, config.port)
+        assert config.port
+        name = container_name(fixture, int(config.port))
         try:
             container = docker.container.inspect(name)
         except Exception:
-            print(f"Failed to stop {fixture_type.value} container")
+            print(f"Failed to stop {fixture} container")
         else:
             container.kill()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `pytest_mock_resources-2.6.9/src/pytest_mock_resources/compat/__init__.py` & `pytest_mock_resources-2.7.0/src/pytest_mock_resources/compat/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_mock_resources-2.6.9/src/pytest_mock_resources/compat/import_.py` & `pytest_mock_resources-2.7.0/src/pytest_mock_resources/compat/import_.py`

 * *Files identical despite different names*

### Comparing `pytest_mock_resources-2.6.9/src/pytest_mock_resources/compat/sqlalchemy.py` & `pytest_mock_resources-2.7.0/src/pytest_mock_resources/compat/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `pytest_mock_resources-2.6.9/src/pytest_mock_resources/config.py` & `pytest_mock_resources-2.7.0/src/pytest_mock_resources/config.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,13 @@
+from __future__ import annotations
+
 import functools
 import os
 import socket
-from typing import Dict, Iterable
+from typing import ClassVar, Dict, Iterable, Type
 
 _DOCKER_HOST = "host.docker.internal"
 
 
 def is_ci():
     return os.getenv("CI") == "true"
 
@@ -45,17 +47,25 @@
                 return self._fields_defaults[attr]
             return None
 
     return wrapper
 
 
 class DockerContainerConfig:
-    _fields: Iterable = {"image", "host", "port", "ci_port"}
+    name: ClassVar[str]
+
+    _fields: Iterable = {"image", "host", "port", "ci_port", "container_args"}
     _fields_defaults: Dict = {}
 
+    subclasses: Dict[str, Type[DockerContainerConfig]] = {}
+
+    @classmethod
+    def __init_subclass__(cls):
+        DockerContainerConfig.subclasses[cls.name] = cls
+
     def __init__(self, **kwargs):
         for field, value in kwargs.items():
             if field not in self._fields:
                 continue
 
             attr = "_{}".format(field)
             setattr(self, attr, value)
@@ -103,14 +113,18 @@
     def port(self):
         ci_port = self.ci_port
         if ci_port and is_ci():
             return ci_port
 
         raise NotImplementedError()
 
+    @fallback
+    def container_args(self):
+        return ()
+
     def ports(self):
         return {}
 
     def environment(self):
         return {}
 
     def check_fn(self):
```

### Comparing `pytest_mock_resources-2.6.9/src/pytest_mock_resources/container/base.py` & `pytest_mock_resources-2.7.0/src/pytest_mock_resources/container/base.py`

 * *Files identical despite different names*

### Comparing `pytest_mock_resources-2.6.9/src/pytest_mock_resources/container/mongo.py` & `pytest_mock_resources-2.7.0/src/pytest_mock_resources/container/mongo.py`

 * *Files identical despite different names*

### Comparing `pytest_mock_resources-2.6.9/src/pytest_mock_resources/container/moto.py` & `pytest_mock_resources-2.7.0/src/pytest_mock_resources/container/moto.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,16 @@
             Defaults to :code:`"localhost"`.
         port (int): The port to bind the container to.
             Defaults to :code:`5532`.
         ci_port (int): The port to bind the container to when a CI environment is detected.
             Defaults to :code:`5432`.
     """
 
-    name = "postgres"
+    name = "moto"
+
     _fields = {"image", "host", "port"}
     _fields_defaults = {
         "image": "motoserver/moto:4.0.6",
         "port": 5555,
     }
 
     def ports(self):
```

### Comparing `pytest_mock_resources-2.6.9/src/pytest_mock_resources/container/mysql.py` & `pytest_mock_resources-2.7.0/src/pytest_mock_resources/container/mysql.py`

 * *Files identical despite different names*

### Comparing `pytest_mock_resources-2.6.9/src/pytest_mock_resources/container/postgres.py` & `pytest_mock_resources-2.7.0/src/pytest_mock_resources/container/postgres.py`

 * *Files 9% similar despite different names*

```diff
@@ -76,26 +76,24 @@
         }
 
     def check_fn(self):
         import socket
 
         s = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         try:
-            s.connect((self.host, self.port))
+            s.connect((self.host, int(self.port)))
         except (ConnectionRefusedError, socket.error):
             raise ContainerCheckFailed(
                 f"Unable to connect to a presumed Postgres test container via given config: {self}"
             )
         finally:
             s.close()
 
 
-def get_sqlalchemy_engine(
-    config, database_name, isolation_level="AUTOCOMMIT", async_=False, **engine_kwargs
-):
+def get_sqlalchemy_engine(config, database_name, async_=False, autocommit=False, **engine_kwargs):
     # For backwards compatibility, our hardcoded default is psycopg2, and async fixtures
     # will not work with psycopg2, so we instead swap the default to the preferred async driver.
     drivername = config.drivername
     if async_ and drivername.endswith("psycopg2"):
         drivername = drivername.replace("psycopg2", "asyncpg")
 
     url = URL(
@@ -103,15 +101,18 @@
         host=config.host,
         port=config.port,
         username=config.username,
         password=config.password,
         database=database_name,
     )
 
+    if autocommit:
+        engine_kwargs["isolation_level"] = "AUTOCOMMIT"
+
     if getattr(url.get_dialect(), "is_async", None):
         from sqlalchemy.ext.asyncio import create_async_engine
 
-        engine = create_async_engine(url, **engine_kwargs, isolation_level=isolation_level)
+        engine = create_async_engine(url, **engine_kwargs)
     else:
-        engine = sqlalchemy.create_engine(url, **engine_kwargs, isolation_level=isolation_level)
+        engine = sqlalchemy.create_engine(url, **engine_kwargs)
 
     return engine
```

### Comparing `pytest_mock_resources-2.6.9/src/pytest_mock_resources/container/redis.py` & `pytest_mock_resources-2.7.0/src/pytest_mock_resources/container/redis.py`

 * *Files identical despite different names*

### Comparing `pytest_mock_resources-2.6.9/src/pytest_mock_resources/container/redshift.py` & `pytest_mock_resources-2.7.0/src/pytest_mock_resources/container/redshift.py`

 * *Files identical despite different names*

### Comparing `pytest_mock_resources-2.6.9/src/pytest_mock_resources/credentials.py` & `pytest_mock_resources-2.7.0/src/pytest_mock_resources/credentials.py`

 * *Files identical despite different names*

### Comparing `pytest_mock_resources-2.6.9/src/pytest_mock_resources/fixture/__init__.py` & `pytest_mock_resources-2.7.0/src/pytest_mock_resources/fixture/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,16 @@
     pmr_mongo_container,
 )
 from pytest_mock_resources.fixture.moto import (
     create_moto_fixture,
     pmr_moto_config,
     pmr_moto_container,
     pmr_moto_credentials,
+    S3Bucket,
+    S3Object,
 )
 from pytest_mock_resources.fixture.mysql import (
     create_mysql_fixture,
     pmr_mysql_config,
     pmr_mysql_container,
 )
 from pytest_mock_resources.fixture.postgresql import (
@@ -28,14 +30,16 @@
     create_redshift_fixture,
     pmr_redshift_config,
     pmr_redshift_container,
 )
 from pytest_mock_resources.fixture.sqlite import create_sqlite_fixture
 
 __all__ = [
+    "S3Bucket",
+    "S3Object",
     "create_mongo_fixture",
     "create_moto_fixture",
     "create_mysql_fixture",
     "create_postgres_fixture",
     "create_redis_fixture",
     "create_redshift_fixture",
     "create_sqlite_fixture",
```

### Comparing `pytest_mock_resources-2.6.9/src/pytest_mock_resources/fixture/base.py` & `pytest_mock_resources-2.7.0/src/pytest_mock_resources/fixture/base.py`

 * *Files identical despite different names*

### Comparing `pytest_mock_resources-2.6.9/src/pytest_mock_resources/fixture/mongo.py` & `pytest_mock_resources-2.7.0/src/pytest_mock_resources/fixture/mongo.py`

 * *Files identical despite different names*

### Comparing `pytest_mock_resources-2.6.9/src/pytest_mock_resources/fixture/moto.py` & `pytest_mock_resources-2.7.0/src/pytest_mock_resources/fixture/moto/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from __future__ import annotations
 
 import time
 from dataclasses import dataclass
 
 import pytest
 
+from pytest_mock_resources.action import validate_actions
 from pytest_mock_resources.compat import boto3
 from pytest_mock_resources.container.base import get_container
 from pytest_mock_resources.container.moto import endpoint_url, MotoConfig
+from pytest_mock_resources.fixture.moto.action import apply_ordered_actions, MotoAction
 
 
 @pytest.fixture(scope="session")
 def pmr_moto_config():
     """Override this fixture with a :class:`MotoConfig` instance to specify different defaults.
 
     Examples:
@@ -23,15 +25,15 @@
 
 
 @pytest.fixture(scope="session")
 def pmr_moto_container(pytestconfig, pmr_moto_config):
     yield from get_container(pytestconfig, pmr_moto_config)
 
 
-def create_moto_fixture(scope="function"):
+def create_moto_fixture(*ordered_actions: MotoAction, scope="function"):
     """Produce a Moto fixture.
 
     Any number of fixture functions can be created. Under the hood they will all share the same
     moto server.
 
     .. note::
 
@@ -44,28 +46,31 @@
     .. note::
 
        A moto dashboard should be available for debugging while the container is running.
        By default it would be available at ``http://localhost:5555/moto-api/#`` (but
        the exact URL may be different depending on your host/port config.
 
     Args:
+        ordered_actions: Any number of ordered actions to be run on test setup.
         scope (str): The scope of the fixture can be specified by the user, defaults to "function".
     """
-    # TODO: Add options for declarative creation of AWS objects, like S3 buckets/files.
+    validate_actions(ordered_actions, fixture="moto")
 
     @pytest.fixture(scope=scope)
     def _fixture(pmr_moto_credentials) -> Session:
-        return Session(
+        session = Session(
             boto3.Session(
                 aws_access_key_id=pmr_moto_credentials.aws_access_key_id,
                 aws_secret_access_key=pmr_moto_credentials.aws_secret_access_key,
                 aws_session_token=pmr_moto_credentials.aws_session_token,
             ),
             endpoint_url=pmr_moto_credentials.endpoint_url,
         )
+        apply_ordered_actions(session, ordered_actions)
+        return session
 
     return _fixture
 
 
 @pytest.fixture()
 def pmr_moto_credentials(pmr_moto_container, pmr_moto_config) -> Credentials:
     # Attempt at a cross-process way of generating unique 12-character integers.
```

### Comparing `pytest_mock_resources-2.6.9/src/pytest_mock_resources/fixture/mysql.py` & `pytest_mock_resources-2.7.0/src/pytest_mock_resources/fixture/mysql.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         ...     return MysqlConfig(image="mysql:5.2", root_database="foo")
     """
     return MysqlConfig()
 
 
 @pytest.fixture(scope="session")
 def pmr_mysql_container(pytestconfig, pmr_mysql_config):
-    yield from get_container(pytestconfig, pmr_mysql_config)
+    yield from get_container(pytestconfig, pmr_mysql_config, interval=1, retries=60)
 
 
 def create_mysql_fixture(
     *ordered_actions,
     scope="function",
     tables=None,
     session=None,
@@ -52,15 +52,18 @@
         engine = get_sqlalchemy_engine(
             pmr_mysql_config,
             database_name,
             **(engine_kwargs or {}),
         )
 
         engine_manager = EngineManager.create(
-            dynamic_actions=ordered_actions, tables=tables, session=session
+            fixture="mysql",
+            dynamic_actions=ordered_actions,
+            tables=tables,
+            session=session,
         )
         for _, conn in engine_manager.manage_sync(engine):
             yield conn
 
     return _
```

### Comparing `pytest_mock_resources-2.6.9/src/pytest_mock_resources/fixture/postgresql.py` & `pytest_mock_resources-2.7.0/src/pytest_mock_resources/fixture/postgresql.py`

 * *Files 3% similar despite different names*

```diff
@@ -103,25 +103,27 @@
 
     if async_:
         return asyncio_fixture(_async, scope=scope)
     else:
         return _sync
 
 
-def _sync_fixture(pmr_config, engine_manager_kwargs, engine_kwargs):
+def _sync_fixture(pmr_config, engine_manager_kwargs, engine_kwargs, *, fixture="postgres"):
     root_engine = cast(Engine, get_sqlalchemy_engine(pmr_config, pmr_config.root_database))
     conn = retry(root_engine.connect, retries=DEFAULT_RETRIES)
     conn.close()
     root_engine.dispose()
 
-    root_engine = cast(Engine, get_sqlalchemy_engine(pmr_config, pmr_config.root_database))
+    root_engine = cast(
+        Engine, get_sqlalchemy_engine(pmr_config, pmr_config.root_database, autocommit=True)
+    )
     with root_engine.connect() as root_conn:
         with root_conn.begin() as trans:
             template_database, template_manager, engine_manager = create_engine_manager(
-                root_conn, **engine_manager_kwargs
+                root_conn, **engine_manager_kwargs, fixture=fixture
             )
             trans.commit()
     root_engine.dispose()
 
     if template_manager:
         assert template_database
 
@@ -132,35 +134,39 @@
             with conn.begin() as trans:
                 template_manager.run_static_actions(conn)
                 trans.commit()
         template_engine.dispose()
 
     # Everything below is normal per-test context. We create a brand new database/engine/manager
     # distinct from what might have been used for the template database.
-    root_engine = cast(Engine, get_sqlalchemy_engine(pmr_config, pmr_config.root_database))
+    root_engine = cast(
+        Engine, get_sqlalchemy_engine(pmr_config, pmr_config.root_database, autocommit=True)
+    )
     with root_engine.connect() as root_conn:
         with root_conn.begin() as trans:
             database_name = _produce_clean_database(root_conn, createdb_template=template_database)
             trans.commit()
     root_engine.dispose()
 
     engine = get_sqlalchemy_engine(pmr_config, database_name, **engine_kwargs)
     yield from engine_manager.manage_sync(engine)
 
 
-async def _async_fixture(pmr_config, engine_manager_kwargs, engine_kwargs):
-    root_engine = get_sqlalchemy_engine(pmr_config, pmr_config.root_database, async_=True)
+async def _async_fixture(pmr_config, engine_manager_kwargs, engine_kwargs, *, fixture="postgres"):
+    root_engine = get_sqlalchemy_engine(
+        pmr_config, pmr_config.root_database, async_=True, autocommit=True
+    )
 
     root_conn = await async_retry(root_engine.connect, retries=DEFAULT_RETRIES)
     await root_conn.close()
 
     async with root_engine.connect() as root_conn:
         async with root_conn.begin() as trans:
             template_database, template_manager, engine_manager = await root_conn.run_sync(
-                create_engine_manager, **engine_manager_kwargs
+                create_engine_manager, **engine_manager_kwargs, fixture=fixture
             )
             await trans.commit()
 
     if template_manager:
         assert template_database
 
         engine = get_sqlalchemy_engine(pmr_config, template_database, **engine_kwargs, async_=True)
@@ -190,16 +196,17 @@
     *,
     ordered_actions,
     session,
     tables,
     createdb_template="template1",
     fixture_id=None,
     actions_share_transaction=None,
+    fixture="postgres",
 ):
-    normalized_actions = normalize_actions(ordered_actions)
+    normalized_actions = normalize_actions(ordered_actions, fixture=fixture)
     static_actions, dynamic_actions = bifurcate_actions(normalized_actions)
 
     template_database = createdb_template
     template_manager = None
     if fixture_id:
         try:
             template_database = _produce_clean_database(
```

### Comparing `pytest_mock_resources-2.6.9/src/pytest_mock_resources/fixture/redis.py` & `pytest_mock_resources-2.7.0/src/pytest_mock_resources/fixture/redis.py`

 * *Files identical despite different names*

### Comparing `pytest_mock_resources-2.6.9/src/pytest_mock_resources/fixture/redshift/__init__.py` & `pytest_mock_resources-2.7.0/src/pytest_mock_resources/fixture/redshift/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,22 +84,24 @@
         fixture_id=fixture_id,
         actions_share_transaction=actions_share_transaction,
     )
 
     @pytest.fixture(scope=scope)
     def _sync(*_, pmr_redshift_container, pmr_redshift_config):
         for engine, conn in _sync_fixture(
-            pmr_redshift_config, engine_manager_kwargs, engine_kwargs_
+            pmr_redshift_config, engine_manager_kwargs, engine_kwargs_, fixture="redshift"
         ):
             sqlalchemy.register_redshift_behavior(engine)
             with psycopg2.patch_connect(pmr_redshift_config, engine.url.database):
                 yield conn
 
     async def _async(*_, pmr_redshift_container, pmr_redshift_config):
-        fixture = _async_fixture(pmr_redshift_config, engine_manager_kwargs, engine_kwargs_)
+        fixture = _async_fixture(
+            pmr_redshift_config, engine_manager_kwargs, engine_kwargs_, fixture="redshift"
+        )
         async for engine, conn in fixture:
             sqlalchemy.register_redshift_behavior(engine.sync_engine)
             yield conn
 
     if async_:
         return asyncio_fixture(_async, scope=scope)
     else:
```

### Comparing `pytest_mock_resources-2.6.9/src/pytest_mock_resources/fixture/redshift/udf.py` & `pytest_mock_resources-2.7.0/src/pytest_mock_resources/fixture/redshift/udf.py`

 * *Files identical despite different names*

### Comparing `pytest_mock_resources-2.6.9/src/pytest_mock_resources/fixture/sqlite.py` & `pytest_mock_resources-2.7.0/src/pytest_mock_resources/fixture/sqlite.py`

 * *Files 2% similar despite different names*

```diff
@@ -251,15 +251,20 @@
         # This *must* happen before the connection occurs (implicitly in `EngineManager`).
         event.listen(raw_engine, "connect", enable_foreign_key_checks)
 
         # https://docs.sqlalchemy.org/en/20/dialects/sqlite.html#pysqlite-serializable
         event.listen(raw_engine, "connect", do_connect)
         event.listen(raw_engine, "begin", do_begin)
 
-        engine_manager = EngineManager.create(ordered_actions, tables=tables, session=session)
+        engine_manager = EngineManager.create(
+            fixture="sqlite",
+            dynamic_actions=ordered_actions,
+            tables=tables,
+            session=session,
+        )
         for _, conn in engine_manager.manage_sync(raw_engine):
             with filter_sqlalchemy_warnings(decimal_warnings_enabled=(not decimal_warnings)):
                 yield conn
 
         event.remove(raw_engine, "connect", enable_foreign_key_checks)
 
     return _
```

### Comparing `pytest_mock_resources-2.6.9/src/pytest_mock_resources/hooks.py` & `pytest_mock_resources-2.7.0/src/pytest_mock_resources/hooks.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,15 +104,17 @@
 
             while containers:
                 container_id = containers.pop(0)
 
                 try:
                     container = docker.container.inspect(container_id)
                 except Exception:
-                    warnings.warn(f"Unrecognized container {container_id}")
+                    warnings.warn(
+                        f"Unrecognized container {container_id}. You may need to manually delete/edit {fn}"
+                    )
                 else:
                     try:
                         container.kill()
                     except Exception:
                         warnings.warn(f"Failed to kill container {container_id}")
 
         fn.unlink()
```

### Comparing `pytest_mock_resources-2.6.9/src/pytest_mock_resources/patch/redshift/mock_s3_copy.py` & `pytest_mock_resources-2.7.0/src/pytest_mock_resources/patch/redshift/mock_s3_copy.py`

 * *Files identical despite different names*

### Comparing `pytest_mock_resources-2.6.9/src/pytest_mock_resources/patch/redshift/mock_s3_unload.py` & `pytest_mock_resources-2.7.0/src/pytest_mock_resources/patch/redshift/mock_s3_unload.py`

 * *Files identical despite different names*

### Comparing `pytest_mock_resources-2.6.9/src/pytest_mock_resources/patch/redshift/psycopg2.py` & `pytest_mock_resources-2.7.0/src/pytest_mock_resources/patch/redshift/psycopg2.py`

 * *Files identical despite different names*

### Comparing `pytest_mock_resources-2.6.9/src/pytest_mock_resources/patch/redshift/sqlalchemy.py` & `pytest_mock_resources-2.7.0/src/pytest_mock_resources/patch/redshift/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `pytest_mock_resources-2.6.9/src/pytest_mock_resources/sqlalchemy.py` & `pytest_mock_resources-2.7.0/src/pytest_mock_resources/sqlalchemy.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,46 +1,33 @@
-import abc
 import fnmatch
 import logging
 from dataclasses import dataclass, field
-from typing import Dict, Iterable, List, Optional, Set, TypeVar, Union
+from typing import Callable, Dict, Iterable, List, Optional, Set, TypeVar, Union
 
 import sqlalchemy
 from sqlalchemy import MetaData, text
 from sqlalchemy.orm import scoped_session, Session, sessionmaker
 from sqlalchemy.sql.ddl import CreateSchema
 from sqlalchemy.sql.schema import Table
 
 from pytest_mock_resources import compat
+from pytest_mock_resources.action import AbstractAction, validate_actions
 from pytest_mock_resources.credentials import Credentials
 
 log = logging.getLogger(__name__)
 
 
-def invalid_action_exception(action):
-    return ValueError(
-        f"`{action}` invalid: create_<x>_fixture functions accept sqlalchemy.MetaData or actions as inputs."
-    )
-
-
-class AbstractAction(metaclass=abc.ABCMeta):
-    static_safe = False
-
-    @abc.abstractmethod
-    def run(self, conn):
-        """Run an action on a database via the passed-in engine_manager instance."""
-
-
 class Rows(AbstractAction):
+    fixtures = ("mysql", "postgres", "redshift", "sqlite")
     static_safe = True
 
     def __init__(self, *rows):
         self.rows = rows
 
-    def run(self, conn):
+    def apply(self, conn):
         rows = self._get_stateless_rows(self.rows)
 
         if isinstance(conn, Session):
             session = conn
         else:
             session = Session(bind=conn)
 
@@ -58,20 +45,21 @@
             stateless_row = type(row)(**row_args)
 
             stateless_rows.append(stateless_row)
         return stateless_rows
 
 
 class Statements(AbstractAction):
+    fixtures = ("mysql", "postgres", "redshift", "sqlite")
     static_safe = False
 
     def __init__(self, *statements):
         self.statements = statements
 
-    def run(self, conn):
+    def apply(self, conn):
         for statement in self.statements:
             if isinstance(statement, str):
                 statement = text(statement)
             conn.execute(statement)
 
 
 class StaticStatements(Statements):
@@ -96,21 +84,22 @@
     _ddl_created: Dict[MetaData, bool] = field(default_factory=dict)
 
     @classmethod
     def create(
         cls,
         dynamic_actions: Iterable[Action],
         *,
+        fixture: Optional[str] = None,
         tables: Iterable = (),
         session: Union[bool, Session] = False,
         static_actions: Iterable[StaticAction] = (),
     ) -> "EngineManager":
         return cls(
-            static_actions=normalize_actions(static_actions),
-            dynamic_actions=normalize_actions(dynamic_actions),
+            static_actions=normalize_actions(static_actions, fixture=fixture),
+            dynamic_actions=normalize_actions(dynamic_actions, fixture=fixture),
             tables=tables,
             session=session,
         )
 
     def manage_sync(self, engine):
         try:
             if self.session:
@@ -233,23 +222,29 @@
         self._create_tables(conn, metadata)
         self._ddl_created[metadata] = True
 
     def execute_action(self, conn, action, allow_function=False):
         if isinstance(action, MetaData):
             self.create_ddl(conn, action)
         elif isinstance(action, AbstractAction):
-            action.run(conn)
+            action.apply(conn)
         elif allow_function and callable(action):
             action(conn)
             commit(conn)
-        else:
-            raise invalid_action_exception(action)
 
 
-def normalize_actions(ordered_actions: Iterable[T]) -> Iterable[T]:
+def normalize_actions(
+    ordered_actions: Iterable[T], *, fixture: Optional[str] = None
+) -> Iterable[T]:
+    validate_actions(
+        ordered_actions,
+        fixture=fixture,
+        additional_types=(compat.sqlalchemy.DeclarativeMeta, Callable, MetaData),
+    )
+
     # Keep track of metadata we've seen to ensure it's only added once per
     # instance, regardless of `Row` references.
     unique_metadata: Set[MetaData] = set()
     normalized_actions: List[T] = []
     for action in ordered_actions:
         if isinstance(action, compat.sqlalchemy.DeclarativeMeta):
             action = action.metadata
@@ -262,16 +257,14 @@
             normalized_actions.append(action)
 
         elif isinstance(action, MetaData):
             if action not in unique_metadata:
                 normalized_actions.append(action)
         elif isinstance(action, AbstractAction) or callable(action):
             normalized_actions.append(action)
-        else:
-            raise invalid_action_exception(action)
 
     return normalized_actions
 
 
 def bifurcate_actions(ordered_actions):
     static_actions = []
     dynamic_actions = []
```

### Comparing `pytest_mock_resources-2.6.9/setup.py` & `pytest_mock_resources-2.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 {'': 'src'}
 
 packages = \
 ['pytest_mock_resources',
  'pytest_mock_resources.compat',
  'pytest_mock_resources.container',
  'pytest_mock_resources.fixture',
+ 'pytest_mock_resources.fixture.moto',
  'pytest_mock_resources.fixture.redshift',
  'pytest_mock_resources.patch',
  'pytest_mock_resources.patch.redshift']
 
 package_data = \
 {'': ['*']}
 
@@ -37,15 +38,15 @@
 
 entry_points = \
 {'console_scripts': ['pmr = pytest_mock_resources.cli:main'],
  'pytest11': ['pytest_mock_resources = pytest_mock_resources']}
 
 setup_kwargs = {
     'name': 'pytest-mock-resources',
-    'version': '2.6.9',
+    'version': '2.7.0',
     'description': 'A pytest plugin for easily instantiating reproducible mock resources.',
     'long_description': '![CircleCI](https://img.shields.io/circleci/build/gh/schireson/pytest-mock-resources/master)\n[![codecov](https://codecov.io/gh/schireson/pytest-mock-resources/branch/master/graph/badge.svg)](https://codecov.io/gh/schireson/pytest-mock-resources)\n[![Documentation\nStatus](https://readthedocs.org/projects/pytest-mock-resources/badge/?version=latest)](https://pytest-mock-resources.readthedocs.io/en/latest/?badge=latest)\n\n## Introduction\n\nCode which depends on external resources such a databases (postgres, redshift, etc) can be difficult\nto write automated tests for. Conventional wisdom might be to mock or stub out the actual database\ncalls and assert that the code works correctly before/after the calls.\n\nHowever take the following, _simple_ example:\n\n```python\ndef serialize(users):\n    return [\n        {\n            \'user\': user.serialize(),\n            \'address\': user.address.serialize(),\n            \'purchases\': [p.serialize() for p in user.purchases],\n        }\n        for user in users\n    ]\n\ndef view_function(session):\n    users = session.query(User).join(Address).options(selectinload(User.purchases)).all()\n    return serialize(users)\n```\n\nSure, you can test `serialize`, but whether the actual **query** did the correct thing _truly_\nrequires that you execute the query.\n\n## The Pitch\n\nHaving tests depend upon a **real** postgres instance running somewhere is a pain, very fragile, and\nprone to issues across machines and test failures.\n\nTherefore `pytest-mock-resources` (primarily) works by managing the lifecycle of docker containers\nand providing access to them inside your tests.\n\nAs such, this package makes 2 primary assumptions:\n\n- You\'re using `pytest` (hopefully that\'s appropriate, given the package name)\n- For many resources, `docker` is required to be available and running (or accessible through remote\n  docker).\n\nIf you aren\'t familiar with Pytest Fixtures, you can read up on them in the [Pytest\ndocumentation](https://docs.pytest.org/en/latest/fixture.html).\n\nIn the above example, your test file could look something like\n\n```python\nfrom pytest_mock_resources import create_postgres_fixture\nfrom models import ModelBase\n\npg = create_postgres_fixture(ModelBase, session=True)\n\ndef test_view_function_empty_db(pg):\n  response = view_function(pg)\n  assert response == ...\n\ndef test_view_function_user_without_purchases(pg):\n  pg.add(User(...))\n  pg.flush()\n\n  response = view_function(pg)\n  assert response == ...\n\ndef test_view_function_user_with_purchases(pg):\n  pg.add(User(..., purchases=[Purchase(...)]))\n  pg.flush()\n\n  response = view_function(pg)\n  assert response == ...\n```\n\n## Existing Resources (many more possible)\n\n- SQLite\n\n  ```python\n  from pytest_mock_resources import create_sqlite_fixture\n  ```\n\n- Postgres\n\n  ```python\n  from pytest_mock_resources import create_postgres_fixture\n  ```\n\n- Redshift\n\n  **note** Uses postgres under the hood, but the fixture tries to support as much redshift\n  functionality as possible (including redshift\'s `COPY`/`UNLOAD` commands).\n\n  ```python\n  from pytest_mock_resources import create_redshift_fixture\n  ```\n\n- Mongo\n\n  ```python\n  from pytest_mock_resources import create_mongo_fixture\n  ```\n\n- Redis\n\n  ```python\n  from pytest_mock_resources import create_redis_fixture\n  ```\n\n- MySQL\n\n  ```python\n  from pytest_mock_resources import create_mysql_fixture\n  ```\n\n- Moto\n\n  ```python\n  from pytest_mock_resources import create_moto_fixture\n  ```\n\n## Features\n\nGeneral features include:\n\n- Support for "actions" which pre-populate the resource you\'re mocking before the test\n- [Async fixtures](https://pytest-mock-resources.readthedocs.io/en/latest/async.html)\n- Custom configuration for container/resource startup\n\n## Installation\n\n```bash\n# Basic fixture support i.e. SQLite\npip install "pytest-mock-resources"\n\n# General, docker-based fixture support\npip install "pytest-mock-resources[docker]"\n\n# Mongo fixture support, installs `pymongo`\npip install "pytest-mock-resources[mongo]"\n\n# Moto fixture support, installs non-driver extras specific to moto support\npip install "pytest-mock-resources[moto]"\n\n# Redis fixture support, Installs `redis` client\npip install "pytest-mock-resources[redis]"\n\n# Redshift fixture support, installs non-driver extras specific to redshift support\npip install "pytest-mock-resources[redshift]"\n```\n\nAdditionally there are number of **convenience** extras currently provided\nfor installing drivers/clients of specific features. However in most cases,\nyou **should** already be installing the driver/client used for that fixture\nas as first-party dependency of your project.\n\nAs such, we recommend against using these extras, and instead explcitly depending\non the package in question in your own project\'s 1st party dependencies.\n\n```bash\n# Installs psycopg2/psycopg2-binary driver\npip install "pytest-mock-resources[postgres-binary]"\npip install "pytest-mock-resources[postgres]"\n\n# Installs asyncpg driver\npip install "pytest-mock-resources[postgres-async]"\n\n# Installs pymysql driver\npip install "pytest-mock-resources[mysql]"\n```\n\n## Possible Future Resources\n\n- Rabbit Broker\n- AWS Presto\n\nFeel free to file an [issue](https://github.com/schireson/pytest-mock-resources/issues) if you find\nany bugs or want to start a conversation around a mock resource you want implemented!\n\n## Python 2\n\nReleases in the 1.x series were supportive of python 2. However starting from 2.0.0, support for\npython 2 was dropped. We may accept bugfix PRs for the 1.x series, however new development and\nfeatures will not be backported.\n',
     'author': 'Omar Khan',
     'author_email': 'oakhan3@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/schireson/pytest-mock-resources',
```

### Comparing `pytest_mock_resources-2.6.9/PKG-INFO` & `pytest_mock_resources-2.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-mock-resources
-Version: 2.6.9
+Version: 2.7.0
 Summary: A pytest plugin for easily instantiating reproducible mock resources.
 Home-page: https://github.com/schireson/pytest-mock-resources
 License: MIT
 Keywords: pytest,sqlalchemy,docker,fixture,mock
 Author: Omar Khan
 Author-email: oakhan3@gmail.com
 Requires-Python: >=3.7,<4
```

