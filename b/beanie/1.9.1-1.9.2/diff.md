# Comparing `tmp/beanie-1.9.1.tar.gz` & `tmp/beanie-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beanie-1.9.1.tar", max compression
+gzip compressed data, was "beanie-1.9.2.tar", max compression
```

## Comparing `beanie-1.9.1.tar` & `beanie-1.9.2.tar`

### file list

```diff
@@ -1,66 +1,66 @@
--rw-r--r--   0        0        0    11343 2022-02-11 13:49:55.790900 beanie-1.9.1/LICENSE
--rw-r--r--   0        0        0     4456 2022-02-11 13:49:55.790900 beanie-1.9.1/README.md
--rw-r--r--   0        0        0      933 2022-02-11 13:49:55.790900 beanie-1.9.1/beanie/__init__.py
--rw-r--r--   0        0        0      540 2022-02-11 13:49:55.790900 beanie-1.9.1/beanie/exceptions.py
--rw-r--r--   0        0        0        0 2022-02-11 13:49:55.790900 beanie-1.9.1/beanie/executors/__init__.py
--rw-r--r--   0        0        0     4329 2022-02-11 13:49:55.790900 beanie-1.9.1/beanie/executors/migrate.py
--rw-r--r--   0        0        0        0 2022-02-11 13:49:55.790900 beanie-1.9.1/beanie/migrations/__init__.py
--rw-r--r--   0        0        0        0 2022-02-11 13:49:55.790900 beanie-1.9.1/beanie/migrations/controllers/__init__.py
--rw-r--r--   0        0        0      308 2022-02-11 13:49:55.790900 beanie-1.9.1/beanie/migrations/controllers/base.py
--rw-r--r--   0        0        0      949 2022-02-11 13:49:55.790900 beanie-1.9.1/beanie/migrations/controllers/free_fall.py
--rw-r--r--   0        0        0     4394 2022-02-11 13:49:55.790900 beanie-1.9.1/beanie/migrations/controllers/iterative.py
--rw-r--r--   0        0        0      413 2022-02-11 13:49:55.790900 beanie-1.9.1/beanie/migrations/database.py
--rw-r--r--   0        0        0      660 2022-02-11 13:49:55.790900 beanie-1.9.1/beanie/migrations/models.py
--rw-r--r--   0        0        0     7510 2022-02-11 13:49:55.790900 beanie-1.9.1/beanie/migrations/runner.py
--rw-r--r--   0        0        0       49 2022-02-11 13:49:55.790900 beanie-1.9.1/beanie/migrations/template.py
--rw-r--r--   0        0        0      178 2022-02-11 13:49:55.790900 beanie-1.9.1/beanie/migrations/utils.py
--rw-r--r--   0        0        0        0 2022-02-11 13:49:55.790900 beanie-1.9.1/beanie/odm/__init__.py
--rw-r--r--   0        0        0     5580 2022-02-11 13:49:55.790900 beanie-1.9.1/beanie/odm/actions.py
--rw-r--r--   0        0        0     1671 2022-02-11 13:49:55.790900 beanie-1.9.1/beanie/odm/bulk.py
--rw-r--r--   0        0        0     1260 2022-02-11 13:49:55.790900 beanie-1.9.1/beanie/odm/cache.py
--rw-r--r--   0        0        0    41398 2022-02-11 13:49:55.790900 beanie-1.9.1/beanie/odm/documents.py
--rw-r--r--   0        0        0      312 2022-02-11 13:49:55.790900 beanie-1.9.1/beanie/odm/enums.py
--rw-r--r--   0        0        0     4800 2022-02-11 13:49:55.790900 beanie-1.9.1/beanie/odm/fields.py
--rw-r--r--   0        0        0        0 2022-02-11 13:49:55.790900 beanie-1.9.1/beanie/odm/interfaces/__init__.py
--rw-r--r--   0        0        0     5332 2022-02-11 13:49:55.790900 beanie-1.9.1/beanie/odm/interfaces/aggregate.py
--rw-r--r--   0        0        0      429 2022-02-11 13:49:55.790900 beanie-1.9.1/beanie/odm/interfaces/session.py
--rw-r--r--   0        0        0     3097 2022-02-11 13:49:55.794901 beanie-1.9.1/beanie/odm/interfaces/update.py
--rw-r--r--   0        0        0      464 2022-02-11 13:49:55.794901 beanie-1.9.1/beanie/odm/models.py
--rw-r--r--   0        0        0      806 2022-02-11 13:49:55.794901 beanie-1.9.1/beanie/odm/operators/__init__.py
--rw-r--r--   0        0        0      120 2022-02-11 13:49:55.794901 beanie-1.9.1/beanie/odm/operators/find/__init__.py
--rw-r--r--   0        0        0     2011 2022-02-11 13:49:55.794901 beanie-1.9.1/beanie/odm/operators/find/array.py
--rw-r--r--   0        0        0     1297 2022-02-11 13:49:55.794901 beanie-1.9.1/beanie/odm/operators/find/bitwise.py
--rw-r--r--   0        0        0     3525 2022-02-11 13:49:55.794901 beanie-1.9.1/beanie/odm/operators/find/comparison.py
--rw-r--r--   0        0        0     1372 2022-02-11 13:49:55.794901 beanie-1.9.1/beanie/odm/operators/find/element.py
--rw-r--r--   0        0        0     4069 2022-02-11 13:49:55.794901 beanie-1.9.1/beanie/odm/operators/find/evaluation.py
--rw-r--r--   0        0        0     5947 2022-02-11 13:49:55.794901 beanie-1.9.1/beanie/odm/operators/find/geospatial.py
--rw-r--r--   0        0        0     3030 2022-02-11 13:49:55.794901 beanie-1.9.1/beanie/odm/operators/find/logical.py
--rw-r--r--   0        0        0      240 2022-02-11 13:49:55.794901 beanie-1.9.1/beanie/odm/operators/update/__init__.py
--rw-r--r--   0        0        0     2469 2022-02-11 13:49:55.794901 beanie-1.9.1/beanie/odm/operators/update/array.py
--rw-r--r--   0        0        0      481 2022-02-11 13:49:55.794901 beanie-1.9.1/beanie/odm/operators/update/bitwise.py
--rw-r--r--   0        0        0     3335 2022-02-11 13:49:55.794901 beanie-1.9.1/beanie/odm/operators/update/general.py
--rw-r--r--   0        0        0        0 2022-02-11 13:49:55.794901 beanie-1.9.1/beanie/odm/queries/__init__.py
--rw-r--r--   0        0        0     3323 2022-02-11 13:49:55.794901 beanie-1.9.1/beanie/odm/queries/aggregation.py
--rw-r--r--   0        0        0     2144 2022-02-11 13:49:55.794901 beanie-1.9.1/beanie/odm/queries/cursor.py
--rw-r--r--   0        0        0     2004 2022-02-11 13:49:55.794901 beanie-1.9.1/beanie/odm/queries/delete.py
--rw-r--r--   0        0        0    27579 2022-02-11 13:49:55.794901 beanie-1.9.1/beanie/odm/queries/find.py
--rw-r--r--   0        0        0     6932 2022-02-11 13:49:55.794901 beanie-1.9.1/beanie/odm/queries/update.py
--rw-r--r--   0        0        0        0 2022-02-11 13:49:55.794901 beanie-1.9.1/beanie/odm/settings/__init__.py
--rw-r--r--   0        0        0     3159 2022-02-11 13:49:55.794901 beanie-1.9.1/beanie/odm/settings/collection.py
--rw-r--r--   0        0        0      934 2022-02-11 13:49:55.794901 beanie-1.9.1/beanie/odm/settings/general.py
--rw-r--r--   0        0        0      846 2022-02-11 13:49:55.794901 beanie-1.9.1/beanie/odm/settings/model.py
--rw-r--r--   0        0        0        0 2022-02-11 13:49:55.794901 beanie-1.9.1/beanie/odm/utils/__init__.py
--rw-r--r--   0        0        0      472 2022-02-11 13:49:55.794901 beanie-1.9.1/beanie/odm/utils/dump.py
--rw-r--r--   0        0        0     5228 2022-02-11 13:49:55.794901 beanie-1.9.1/beanie/odm/utils/encoder.py
--rw-r--r--   0        0        0     2354 2022-02-11 13:49:55.794901 beanie-1.9.1/beanie/odm/utils/find.py
--rw-r--r--   0        0        0     2362 2022-02-11 13:49:55.794901 beanie-1.9.1/beanie/odm/utils/general.py
--rw-r--r--   0        0        0      394 2022-02-11 13:49:55.794901 beanie-1.9.1/beanie/odm/utils/parsing.py
--rw-r--r--   0        0        0      577 2022-02-11 13:49:55.794901 beanie-1.9.1/beanie/odm/utils/projection.py
--rw-r--r--   0        0        0     1407 2022-02-11 13:49:55.794901 beanie-1.9.1/beanie/odm/utils/relations.py
--rw-r--r--   0        0        0      348 2022-02-11 13:49:55.794901 beanie-1.9.1/beanie/odm/utils/self_validation.py
--rw-r--r--   0        0        0     1506 2022-02-11 13:49:55.794901 beanie-1.9.1/beanie/odm/utils/state.py
--rw-r--r--   0        0        0     1825 2022-02-11 13:49:55.794901 beanie-1.9.1/beanie/operators.py
--rw-r--r--   0        0        0        0 2022-02-11 13:49:55.794901 beanie-1.9.1/beanie/py.typed
--rw-r--r--   0        0        0     1663 2022-02-11 13:49:55.798902 beanie-1.9.1/pyproject.toml
--rw-r--r--   0        0        0     5663 2022-02-11 13:52:34.514058 beanie-1.9.1/setup.py
--rw-r--r--   0        0        0     5317 2022-02-11 13:52:34.514728 beanie-1.9.1/PKG-INFO
+-rw-r--r--   0        0        0    11343 2022-02-22 12:08:17.442472 beanie-1.9.2/LICENSE
+-rw-r--r--   0        0        0     4456 2022-02-22 12:08:17.442472 beanie-1.9.2/README.md
+-rw-r--r--   0        0        0      933 2022-02-22 12:08:17.442472 beanie-1.9.2/beanie/__init__.py
+-rw-r--r--   0        0        0      540 2022-02-22 12:08:17.442472 beanie-1.9.2/beanie/exceptions.py
+-rw-r--r--   0        0        0        0 2022-02-22 12:08:17.442472 beanie-1.9.2/beanie/executors/__init__.py
+-rw-r--r--   0        0        0     4329 2022-02-22 12:08:17.442472 beanie-1.9.2/beanie/executors/migrate.py
+-rw-r--r--   0        0        0        0 2022-02-22 12:08:17.442472 beanie-1.9.2/beanie/migrations/__init__.py
+-rw-r--r--   0        0        0        0 2022-02-22 12:08:17.442472 beanie-1.9.2/beanie/migrations/controllers/__init__.py
+-rw-r--r--   0        0        0      308 2022-02-22 12:08:17.442472 beanie-1.9.2/beanie/migrations/controllers/base.py
+-rw-r--r--   0        0        0      949 2022-02-22 12:08:17.442472 beanie-1.9.2/beanie/migrations/controllers/free_fall.py
+-rw-r--r--   0        0        0     4394 2022-02-22 12:08:17.442472 beanie-1.9.2/beanie/migrations/controllers/iterative.py
+-rw-r--r--   0        0        0      413 2022-02-22 12:08:17.442472 beanie-1.9.2/beanie/migrations/database.py
+-rw-r--r--   0        0        0      660 2022-02-22 12:08:17.442472 beanie-1.9.2/beanie/migrations/models.py
+-rw-r--r--   0        0        0     7510 2022-02-22 12:08:17.442472 beanie-1.9.2/beanie/migrations/runner.py
+-rw-r--r--   0        0        0       49 2022-02-22 12:08:17.442472 beanie-1.9.2/beanie/migrations/template.py
+-rw-r--r--   0        0        0      178 2022-02-22 12:08:17.442472 beanie-1.9.2/beanie/migrations/utils.py
+-rw-r--r--   0        0        0        0 2022-02-22 12:08:17.442472 beanie-1.9.2/beanie/odm/__init__.py
+-rw-r--r--   0        0        0     5580 2022-02-22 12:08:17.442472 beanie-1.9.2/beanie/odm/actions.py
+-rw-r--r--   0        0        0     1671 2022-02-22 12:08:17.442472 beanie-1.9.2/beanie/odm/bulk.py
+-rw-r--r--   0        0        0     1260 2022-02-22 12:08:17.442472 beanie-1.9.2/beanie/odm/cache.py
+-rw-r--r--   0        0        0    41398 2022-02-22 12:08:17.446472 beanie-1.9.2/beanie/odm/documents.py
+-rw-r--r--   0        0        0      312 2022-02-22 12:08:17.446472 beanie-1.9.2/beanie/odm/enums.py
+-rw-r--r--   0        0        0     4800 2022-02-22 12:08:17.446472 beanie-1.9.2/beanie/odm/fields.py
+-rw-r--r--   0        0        0        0 2022-02-22 12:08:17.446472 beanie-1.9.2/beanie/odm/interfaces/__init__.py
+-rw-r--r--   0        0        0     5332 2022-02-22 12:08:17.446472 beanie-1.9.2/beanie/odm/interfaces/aggregate.py
+-rw-r--r--   0        0        0      429 2022-02-22 12:08:17.446472 beanie-1.9.2/beanie/odm/interfaces/session.py
+-rw-r--r--   0        0        0     3097 2022-02-22 12:08:17.446472 beanie-1.9.2/beanie/odm/interfaces/update.py
+-rw-r--r--   0        0        0      464 2022-02-22 12:08:17.446472 beanie-1.9.2/beanie/odm/models.py
+-rw-r--r--   0        0        0      806 2022-02-22 12:08:17.446472 beanie-1.9.2/beanie/odm/operators/__init__.py
+-rw-r--r--   0        0        0      120 2022-02-22 12:08:17.446472 beanie-1.9.2/beanie/odm/operators/find/__init__.py
+-rw-r--r--   0        0        0     2011 2022-02-22 12:08:17.446472 beanie-1.9.2/beanie/odm/operators/find/array.py
+-rw-r--r--   0        0        0     1297 2022-02-22 12:08:17.446472 beanie-1.9.2/beanie/odm/operators/find/bitwise.py
+-rw-r--r--   0        0        0     3525 2022-02-22 12:08:17.446472 beanie-1.9.2/beanie/odm/operators/find/comparison.py
+-rw-r--r--   0        0        0     1372 2022-02-22 12:08:17.446472 beanie-1.9.2/beanie/odm/operators/find/element.py
+-rw-r--r--   0        0        0     4069 2022-02-22 12:08:17.446472 beanie-1.9.2/beanie/odm/operators/find/evaluation.py
+-rw-r--r--   0        0        0     5947 2022-02-22 12:08:17.446472 beanie-1.9.2/beanie/odm/operators/find/geospatial.py
+-rw-r--r--   0        0        0     3030 2022-02-22 12:08:17.446472 beanie-1.9.2/beanie/odm/operators/find/logical.py
+-rw-r--r--   0        0        0      240 2022-02-22 12:08:17.446472 beanie-1.9.2/beanie/odm/operators/update/__init__.py
+-rw-r--r--   0        0        0     2469 2022-02-22 12:08:17.446472 beanie-1.9.2/beanie/odm/operators/update/array.py
+-rw-r--r--   0        0        0      481 2022-02-22 12:08:17.446472 beanie-1.9.2/beanie/odm/operators/update/bitwise.py
+-rw-r--r--   0        0        0     3335 2022-02-22 12:08:17.446472 beanie-1.9.2/beanie/odm/operators/update/general.py
+-rw-r--r--   0        0        0        0 2022-02-22 12:08:17.446472 beanie-1.9.2/beanie/odm/queries/__init__.py
+-rw-r--r--   0        0        0     3323 2022-02-22 12:08:17.446472 beanie-1.9.2/beanie/odm/queries/aggregation.py
+-rw-r--r--   0        0        0     2144 2022-02-22 12:08:17.446472 beanie-1.9.2/beanie/odm/queries/cursor.py
+-rw-r--r--   0        0        0     2004 2022-02-22 12:08:17.446472 beanie-1.9.2/beanie/odm/queries/delete.py
+-rw-r--r--   0        0        0    27856 2022-02-22 12:08:17.446472 beanie-1.9.2/beanie/odm/queries/find.py
+-rw-r--r--   0        0        0     6932 2022-02-22 12:08:17.446472 beanie-1.9.2/beanie/odm/queries/update.py
+-rw-r--r--   0        0        0        0 2022-02-22 12:08:17.446472 beanie-1.9.2/beanie/odm/settings/__init__.py
+-rw-r--r--   0        0        0     3159 2022-02-22 12:08:17.446472 beanie-1.9.2/beanie/odm/settings/collection.py
+-rw-r--r--   0        0        0      934 2022-02-22 12:08:17.446472 beanie-1.9.2/beanie/odm/settings/general.py
+-rw-r--r--   0        0        0      846 2022-02-22 12:08:17.446472 beanie-1.9.2/beanie/odm/settings/model.py
+-rw-r--r--   0        0        0        0 2022-02-22 12:08:17.446472 beanie-1.9.2/beanie/odm/utils/__init__.py
+-rw-r--r--   0        0        0      472 2022-02-22 12:08:17.446472 beanie-1.9.2/beanie/odm/utils/dump.py
+-rw-r--r--   0        0        0     5228 2022-02-22 12:08:17.446472 beanie-1.9.2/beanie/odm/utils/encoder.py
+-rw-r--r--   0        0        0     2354 2022-02-22 12:08:17.446472 beanie-1.9.2/beanie/odm/utils/find.py
+-rw-r--r--   0        0        0     2362 2022-02-22 12:08:17.446472 beanie-1.9.2/beanie/odm/utils/general.py
+-rw-r--r--   0        0        0      394 2022-02-22 12:08:17.446472 beanie-1.9.2/beanie/odm/utils/parsing.py
+-rw-r--r--   0        0        0      577 2022-02-22 12:08:17.446472 beanie-1.9.2/beanie/odm/utils/projection.py
+-rw-r--r--   0        0        0     1407 2022-02-22 12:08:17.446472 beanie-1.9.2/beanie/odm/utils/relations.py
+-rw-r--r--   0        0        0      348 2022-02-22 12:08:17.446472 beanie-1.9.2/beanie/odm/utils/self_validation.py
+-rw-r--r--   0        0        0     1506 2022-02-22 12:08:17.446472 beanie-1.9.2/beanie/odm/utils/state.py
+-rw-r--r--   0        0        0     1825 2022-02-22 12:08:17.446472 beanie-1.9.2/beanie/operators.py
+-rw-r--r--   0        0        0        0 2022-02-22 12:08:17.446472 beanie-1.9.2/beanie/py.typed
+-rw-r--r--   0        0        0     1663 2022-02-22 12:08:17.450471 beanie-1.9.2/pyproject.toml
+-rw-r--r--   0        0        0     5663 2022-02-22 12:10:44.106408 beanie-1.9.2/setup.py
+-rw-r--r--   0        0        0     5317 2022-02-22 12:10:44.106968 beanie-1.9.2/PKG-INFO
```

### Comparing `beanie-1.9.1/LICENSE` & `beanie-1.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `beanie-1.9.1/README.md` & `beanie-1.9.2/README.md`

 * *Files identical despite different names*

### Comparing `beanie-1.9.1/beanie/__init__.py` & `beanie-1.9.2/beanie/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     Link,
     WriteRules,
     DeleteRules,
 )
 from beanie.odm.utils.general import init_beanie
 from beanie.odm.documents import Document
 
-__version__ = "1.9.1"
+__version__ = "1.9.2"
 __all__ = [
     # ODM
     "Document",
     "init_beanie",
     "PydanticObjectId",
     "Indexed",
     # Actions
```

### Comparing `beanie-1.9.1/beanie/exceptions.py` & `beanie-1.9.2/beanie/exceptions.py`

 * *Files identical despite different names*

### Comparing `beanie-1.9.1/beanie/executors/migrate.py` & `beanie-1.9.2/beanie/executors/migrate.py`

 * *Files identical despite different names*

### Comparing `beanie-1.9.1/beanie/migrations/controllers/free_fall.py` & `beanie-1.9.2/beanie/migrations/controllers/free_fall.py`

 * *Files identical despite different names*

### Comparing `beanie-1.9.1/beanie/migrations/controllers/iterative.py` & `beanie-1.9.2/beanie/migrations/controllers/iterative.py`

 * *Files identical despite different names*

### Comparing `beanie-1.9.1/beanie/migrations/models.py` & `beanie-1.9.2/beanie/migrations/models.py`

 * *Files identical despite different names*

### Comparing `beanie-1.9.1/beanie/migrations/runner.py` & `beanie-1.9.2/beanie/migrations/runner.py`

 * *Files identical despite different names*

### Comparing `beanie-1.9.1/beanie/odm/actions.py` & `beanie-1.9.2/beanie/odm/actions.py`

 * *Files identical despite different names*

### Comparing `beanie-1.9.1/beanie/odm/bulk.py` & `beanie-1.9.2/beanie/odm/bulk.py`

 * *Files identical despite different names*

### Comparing `beanie-1.9.1/beanie/odm/cache.py` & `beanie-1.9.2/beanie/odm/cache.py`

 * *Files identical despite different names*

### Comparing `beanie-1.9.1/beanie/odm/documents.py` & `beanie-1.9.2/beanie/odm/documents.py`

 * *Files identical despite different names*

### Comparing `beanie-1.9.1/beanie/odm/fields.py` & `beanie-1.9.2/beanie/odm/fields.py`

 * *Files identical despite different names*

### Comparing `beanie-1.9.1/beanie/odm/interfaces/aggregate.py` & `beanie-1.9.2/beanie/odm/interfaces/aggregate.py`

 * *Files identical despite different names*

### Comparing `beanie-1.9.1/beanie/odm/interfaces/update.py` & `beanie-1.9.2/beanie/odm/interfaces/update.py`

 * *Files identical despite different names*

### Comparing `beanie-1.9.1/beanie/odm/operators/__init__.py` & `beanie-1.9.2/beanie/odm/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `beanie-1.9.1/beanie/odm/operators/find/array.py` & `beanie-1.9.2/beanie/odm/operators/find/array.py`

 * *Files identical despite different names*

### Comparing `beanie-1.9.1/beanie/odm/operators/find/bitwise.py` & `beanie-1.9.2/beanie/odm/operators/find/bitwise.py`

 * *Files identical despite different names*

### Comparing `beanie-1.9.1/beanie/odm/operators/find/comparison.py` & `beanie-1.9.2/beanie/odm/operators/find/comparison.py`

 * *Files identical despite different names*

### Comparing `beanie-1.9.1/beanie/odm/operators/find/element.py` & `beanie-1.9.2/beanie/odm/operators/find/element.py`

 * *Files identical despite different names*

### Comparing `beanie-1.9.1/beanie/odm/operators/find/evaluation.py` & `beanie-1.9.2/beanie/odm/operators/find/evaluation.py`

 * *Files identical despite different names*

### Comparing `beanie-1.9.1/beanie/odm/operators/find/geospatial.py` & `beanie-1.9.2/beanie/odm/operators/find/geospatial.py`

 * *Files identical despite different names*

### Comparing `beanie-1.9.1/beanie/odm/operators/find/logical.py` & `beanie-1.9.2/beanie/odm/operators/find/logical.py`

 * *Files identical despite different names*

### Comparing `beanie-1.9.1/beanie/odm/operators/update/array.py` & `beanie-1.9.2/beanie/odm/operators/update/array.py`

 * *Files identical despite different names*

### Comparing `beanie-1.9.1/beanie/odm/operators/update/general.py` & `beanie-1.9.2/beanie/odm/operators/update/general.py`

 * *Files identical despite different names*

### Comparing `beanie-1.9.1/beanie/odm/queries/aggregation.py` & `beanie-1.9.2/beanie/odm/queries/aggregation.py`

 * *Files identical despite different names*

### Comparing `beanie-1.9.1/beanie/odm/queries/cursor.py` & `beanie-1.9.2/beanie/odm/queries/cursor.py`

 * *Files identical despite different names*

### Comparing `beanie-1.9.1/beanie/odm/queries/delete.py` & `beanie-1.9.2/beanie/odm/queries/delete.py`

 * *Files identical despite different names*

### Comparing `beanie-1.9.1/beanie/odm/queries/find.py` & `beanie-1.9.2/beanie/odm/queries/find.py`

 * *Files 2% similar despite different names*

```diff
@@ -581,14 +581,23 @@
             sort=self.sort_expressions,
             projection=get_projection(self.projection_model),
             skip=self.skip_number,
             limit=self.limit_number,
             session=self.session,
         )
 
+    async def first_or_none(self) -> Optional[FindQueryResultType]:
+        """
+        Returns the first found element or None if no elements were found
+        """
+        res = await self.limit(1).to_list()
+        if not res:
+            return None
+        return res[0]
+
 
 class FindOne(FindQuery[FindQueryResultType]):
     """
     Find One query class
 
     Inherited from:
```

### Comparing `beanie-1.9.1/beanie/odm/queries/update.py` & `beanie-1.9.2/beanie/odm/queries/update.py`

 * *Files identical despite different names*

### Comparing `beanie-1.9.1/beanie/odm/settings/collection.py` & `beanie-1.9.2/beanie/odm/settings/collection.py`

 * *Files identical despite different names*

### Comparing `beanie-1.9.1/beanie/odm/settings/general.py` & `beanie-1.9.2/beanie/odm/settings/general.py`

 * *Files identical despite different names*

### Comparing `beanie-1.9.1/beanie/odm/settings/model.py` & `beanie-1.9.2/beanie/odm/settings/model.py`

 * *Files identical despite different names*

### Comparing `beanie-1.9.1/beanie/odm/utils/encoder.py` & `beanie-1.9.2/beanie/odm/utils/encoder.py`

 * *Files identical despite different names*

### Comparing `beanie-1.9.1/beanie/odm/utils/find.py` & `beanie-1.9.2/beanie/odm/utils/find.py`

 * *Files identical despite different names*

### Comparing `beanie-1.9.1/beanie/odm/utils/general.py` & `beanie-1.9.2/beanie/odm/utils/general.py`

 * *Files identical despite different names*

### Comparing `beanie-1.9.1/beanie/odm/utils/projection.py` & `beanie-1.9.2/beanie/odm/utils/projection.py`

 * *Files identical despite different names*

### Comparing `beanie-1.9.1/beanie/odm/utils/relations.py` & `beanie-1.9.2/beanie/odm/utils/relations.py`

 * *Files identical despite different names*

### Comparing `beanie-1.9.1/beanie/odm/utils/state.py` & `beanie-1.9.2/beanie/odm/utils/state.py`

 * *Files identical despite different names*

### Comparing `beanie-1.9.1/beanie/operators.py` & `beanie-1.9.2/beanie/operators.py`

 * *Files identical despite different names*

### Comparing `beanie-1.9.1/pyproject.toml` & `beanie-1.9.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "beanie"
-version = "1.9.1"
+version = "1.9.2"
 description = "Asynchronous Python ODM for MongoDB"
 authors = ["Roman <roman-right@protonmail.com>"]
 license = "Apache-2.0"
 homepage = "https://roman-right.github.io/beanie/"
 repository = "https://github.com/roman-right/beanie"
 keywords = ["mongodb", "odm", "orm", "pydantic", "mongo", "async", "python"]
 include = [
```

### Comparing `beanie-1.9.1/setup.py` & `beanie-1.9.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 ['click>=7', 'motor>=2.5,<3.0', 'pydantic>=1.9.0', 'toml', 'yarl>=1.6']
 
 entry_points = \
 {'console_scripts': ['beanie = beanie.executors.migrate:migrations']}
 
 setup_kwargs = {
     'name': 'beanie',
-    'version': '1.9.1',
+    'version': '1.9.2',
     'description': 'Asynchronous Python ODM for MongoDB',
     'long_description': '[![Beanie](https://raw.githubusercontent.com/roman-right/beanie/main/assets/logo/white_bg.svg)](https://github.com/roman-right/beanie)\n\n[![shields badge](https://shields.io/badge/-docs-blue)](https://roman-right.github.io/beanie/)\n[![pypi](https://img.shields.io/pypi/v/beanie.svg)](https://pypi.python.org/pypi/beanie)\n\n## Overview\n\n[Beanie](https://github.com/roman-right/beanie) - is an Asynchronous Python\nobject-document mapper (ODM) for MongoDB, based\non [Motor](https://motor.readthedocs.io/en/stable/)\nand [Pydantic](https://pydantic-docs.helpmanual.io/).\n\nWhen using Beanie each database collection has a corresponding `Document` that\nis used to interact with that collection. In addition to retrieving data,\nBeanie allows you to add, update, or delete documents from the collection as\nwell.\n\nBeanie saves you time by removing boiler-plate code and it helps you focus on\nthe parts of your app that actually matter.\n\nData and schema migrations are supported by Beanie out of the box.\n\n## Installation\n\n### PIP\n\n```shell\npip install beanie\n```\n\n### Poetry\n\n```shell\npoetry add beanie\n```\n## Example\n\n```python\nfrom typing import Optional\nfrom pydantic import BaseModel\nfrom beanie import Document, Indexed, init_beanie\nimport asyncio, motor\n\nclass Category(BaseModel):\n    name: str\n    description: str\n\nclass Product(Document):\n    name: str                          # You can use normal types just like in pydantic\n    description: Optional[str] = None\n    price: Indexed(float)              # You can also specify that a field should correspond to an index\n    category: Category                 # You can include pydantic models as well\n\n# Beanie is fully asynchronous, so we will access it from an async function\nasync def example():\n    # Beanie uses Motor under the hood \n    client = motor.motor_asyncio.AsyncIOMotorClient("mongodb://user:pass@host:27017")\n\n    # Init beanie with the Product document class\n    await init_beanie(database=client.db_name, document_models=[Product])\n\n    chocolate = Category(name="Chocolate", description="A preparation of roasted and ground cacao seeds.")\n    # Beanie documents work just like pydantic models\n    tonybar = Product(name="Tony\'s", price=5.95, category=chocolate)\n    # And can be inserted into the database\n    await tonybar.insert() \n    \n    # You can find documents with pythonic syntax\n    product = await Product.find_one(Product.price < 10)\n    \n    # And update them\n    await product.set({Product.name:"Gold bar"})\n    \nasyncio.run(example())\n```\n\n## Links\n\n### Documentation\n\n- **[Doc](https://roman-right.github.io/beanie/)** - Tutorial, API docmentation, and development guidlines.\n\n### Example Projects\n\n- **[fastapi-cosmos-beanie](https://github.com/tonybaloney/ants-azure-demos/tree/master/fastapi-cosmos-beanie)** - FastAPI + Beanie ODM + Azure Cosmos Demo Application by [Anthony Shaw](https://github.com/tonybaloney)\n- **[fastapi-beanie-jwt](https://github.com/flyinactor91/fastapi-beanie-jwt)** - \n  Sample FastAPI server with JWT auth and Beanie ODM by [Michael duPont](https://github.com/flyinactor91)\n\n### Articles\n\n- **[Announcing Beanie - MongoDB ODM](https://dev.to/romanright/announcing-beanie-mongodb-odm-56e)**\n- **[Build a Cocktail API with Beanie and MongoDB](https://developer.mongodb.com/article/beanie-odm-fastapi-cocktails/)**\n- **[MongoDB indexes with Beanie](https://dev.to/romanright/mongodb-indexes-with-beanie-43e8)**\n- **[Beanie Projections. Reducing network and database load.](https://dev.to/romanright/beanie-projections-reducing-network-and-database-load-3bih)**\n- **[Beanie 1.0 - Query Builder](https://dev.to/romanright/announcing-beanie-1-0-mongodb-odm-with-query-builder-4mbl)**\n- **[Beanie 1.8 - Relations, Cache, Actions and more!](https://dev.to/romanright/announcing-beanie-odm-18-relations-cache-actions-and-more-24ef)**\n\n### Resources\n\n- **[GitHub](https://github.com/roman-right/beanie)** - GitHub page of the\n  project\n- **[Changelog](https://roman-right.github.io/beanie/changelog)** - list of all\n  the valuable changes\n- **[Discord](https://discord.gg/ZTTnM7rMaz)** - ask your questions, share\n  ideas or just say `Hello!!`\n\n## Sponsor the project\n\n- Bitcoin `bc1qz8z0uhftdcra7u8hjyft6nqn30uhktlcgsg0tq`\n- Doge `DPKs32RSEVwPiKuGAAmQHZ8VQ8BQK5Qg4L`\n\n----\nSupported by [JetBrains](https://jb.gg/OpenSource)\n\n[![JetBrains](https://raw.githubusercontent.com/roman-right/beanie/main/assets/logo/jetbrains.svg)](https://jb.gg/OpenSource)\n',
     'author': 'Roman',
     'author_email': 'roman-right@protonmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://roman-right.github.io/beanie/',
```

### Comparing `beanie-1.9.1/PKG-INFO` & `beanie-1.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beanie
-Version: 1.9.1
+Version: 1.9.2
 Summary: Asynchronous Python ODM for MongoDB
 Home-page: https://roman-right.github.io/beanie/
 License: Apache-2.0
 Keywords: mongodb,odm,orm,pydantic,mongo,async,python
 Author: Roman
 Author-email: roman-right@protonmail.com
 Requires-Python: >=3.7,<4.0
```

