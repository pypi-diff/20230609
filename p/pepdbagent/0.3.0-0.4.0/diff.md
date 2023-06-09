# Comparing `tmp/pepdbagent-0.3.0.tar.gz` & `tmp/pepdbagent-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pepdbagent-0.3.0.tar", last modified: Thu Jan 19 17:13:53 2023, max compression
+gzip compressed data, was "pepdbagent-0.4.0.tar", last modified: Fri Jun  9 17:28:26 2023, max compression
```

## Comparing `pepdbagent-0.3.0.tar` & `pepdbagent-0.4.0.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 17:13:53.315508 pepdbagent-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-01-19 17:13:41.000000 pepdbagent-0.3.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-01-19 17:13:41.000000 pepdbagent-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-01-19 17:13:53.315508 pepdbagent-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-01-19 17:13:41.000000 pepdbagent-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 17:13:53.311508 pepdbagent-0.3.0/pepdbagent/
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-01-19 17:13:41.000000 pepdbagent-0.3.0/pepdbagent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-01-19 17:13:41.000000 pepdbagent-0.3.0/pepdbagent/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-01-19 17:13:41.000000 pepdbagent-0.3.0/pepdbagent/base_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-01-19 17:13:41.000000 pepdbagent-0.3.0/pepdbagent/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-01-19 17:13:41.000000 pepdbagent-0.3.0/pepdbagent/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-01-19 17:13:41.000000 pepdbagent-0.3.0/pepdbagent/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 17:13:53.311508 pepdbagent-0.3.0/pepdbagent/modules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-19 17:13:41.000000 pepdbagent-0.3.0/pepdbagent/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11737 2023-01-19 17:13:41.000000 pepdbagent-0.3.0/pepdbagent/modules/annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4806 2023-01-19 17:13:41.000000 pepdbagent-0.3.0/pepdbagent/modules/namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)    15507 2023-01-19 17:13:41.000000 pepdbagent-0.3.0/pepdbagent/modules/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-01-19 17:13:41.000000 pepdbagent-0.3.0/pepdbagent/pepdbagent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-01-19 17:13:41.000000 pepdbagent-0.3.0/pepdbagent/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 17:13:53.311508 pepdbagent-0.3.0/pepdbagent.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-01-19 17:13:53.000000 pepdbagent-0.3.0/pepdbagent.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-01-19 17:13:53.000000 pepdbagent-0.3.0/pepdbagent.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-19 17:13:53.000000 pepdbagent-0.3.0/pepdbagent.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-01-19 17:13:53.000000 pepdbagent-0.3.0/pepdbagent.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-01-19 17:13:53.000000 pepdbagent-0.3.0/pepdbagent.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 17:13:53.315508 pepdbagent-0.3.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-01-19 17:13:41.000000 pepdbagent-0.3.0/requirements/requirements-all.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-01-19 17:13:41.000000 pepdbagent-0.3.0/requirements/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-19 17:13:53.315508 pepdbagent-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-01-19 17:13:41.000000 pepdbagent-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 17:13:53.315508 pepdbagent-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-19 17:13:41.000000 pepdbagent-0.3.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-01-19 17:13:41.000000 pepdbagent-0.3.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    12849 2023-01-19 17:13:41.000000 pepdbagent-0.3.0/tests/test_pepagent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:28:26.006973 pepdbagent-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-06-09 17:28:16.000000 pepdbagent-0.4.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-09 17:28:16.000000 pepdbagent-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-06-09 17:28:26.006973 pepdbagent-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-09 17:28:16.000000 pepdbagent-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:28:26.002973 pepdbagent-0.4.0/pepdbagent/
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-09 17:28:16.000000 pepdbagent-0.4.0/pepdbagent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-09 17:28:16.000000 pepdbagent-0.4.0/pepdbagent/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-09 17:28:16.000000 pepdbagent-0.4.0/pepdbagent/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-06-09 17:28:16.000000 pepdbagent-0.4.0/pepdbagent/db_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-09 17:28:16.000000 pepdbagent-0.4.0/pepdbagent/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-06-09 17:28:16.000000 pepdbagent-0.4.0/pepdbagent/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:28:26.002973 pepdbagent-0.4.0/pepdbagent/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 17:28:16.000000 pepdbagent-0.4.0/pepdbagent/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14855 2023-06-09 17:28:16.000000 pepdbagent-0.4.0/pepdbagent/modules/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5516 2023-06-09 17:28:16.000000 pepdbagent-0.4.0/pepdbagent/modules/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15542 2023-06-09 17:28:16.000000 pepdbagent-0.4.0/pepdbagent/modules/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-06-09 17:28:16.000000 pepdbagent-0.4.0/pepdbagent/pepdbagent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-06-09 17:28:16.000000 pepdbagent-0.4.0/pepdbagent/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:28:26.002973 pepdbagent-0.4.0/pepdbagent.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-06-09 17:28:25.000000 pepdbagent-0.4.0/pepdbagent.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-06-09 17:28:25.000000 pepdbagent-0.4.0/pepdbagent.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 17:28:25.000000 pepdbagent-0.4.0/pepdbagent.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-09 17:28:25.000000 pepdbagent-0.4.0/pepdbagent.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-09 17:28:25.000000 pepdbagent-0.4.0/pepdbagent.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-09 17:28:16.000000 pepdbagent-0.4.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:28:26.002973 pepdbagent-0.4.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-09 17:28:16.000000 pepdbagent-0.4.0/requirements/requirements-all.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-09 17:28:16.000000 pepdbagent-0.4.0/requirements/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 17:28:26.006973 pepdbagent-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-06-09 17:28:16.000000 pepdbagent-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:28:26.006973 pepdbagent-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 17:28:16.000000 pepdbagent-0.4.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-06-09 17:28:16.000000 pepdbagent-0.4.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12829 2023-06-09 17:28:16.000000 pepdbagent-0.4.0/tests/test_pepagent.py
```

### Comparing `pepdbagent-0.3.0/LICENSE.txt` & `pepdbagent-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pepdbagent-0.3.0/PKG-INFO` & `pepdbagent-0.4.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: pepdbagent
-Version: 0.3.0
+Version: 0.4.0
 Summary: A python-based project metadata manager for portable encapsulated projects
 Home-page: https://github.com/pepkit/pepdbagent/
 Author: Oleksandr Khoroshevskyi
 License: BSD2
 Keywords: project,metadata,bioinformatics,database
-Classifier: Development Status :: 1 - Planning
+Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # pepdbagent
 
-pepdbagent is a python library and toolkit that gives a user user-friendly 
+`pepdbagent` is a Python library and toolkit that gives a user-friendly 
 interface to connect, upload, update and retrieve information from pep-db.
 
-**pep-db** is and postgres database created for storing [PEPs](http://pep.databio.org/en/latest/). 
-It is a backend database for PEPhub. database enables storing huge projects and provides fast speed of retrieving them.
+**pep-db** is a postgres database created for storing [PEPs](http://pep.databio.org/en/latest/). 
+It is a backend database for PEPhub. 
 
-Before using pepdbagent, you should install or have access to pep-db.
+Before using pepdbagent, you should install or have access to a pep-db instance.
 
-To install pep-db you can use this tutorial:
+To run a pep-db instance, you can use this tutorial:
 - [pep-db installation](./docs/db_tutorial.md)
 
-
-pepdbagent tutorial is here:
+Then, follow the `pepdbagent` tutorial here:
 - [pedbagent](./docs/README.md)
```

### Comparing `pepdbagent-0.3.0/pepdbagent/exceptions.py` & `pepdbagent-0.4.0/pepdbagent/exceptions.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,17 +6,15 @@
 
     def __init__(self, msg):
         super(PEPDatabaseAgentError, self).__init__(msg)
 
 
 class SchemaError(PEPDatabaseAgentError):
     def __init__(self):
-        super().__init__(
-            """PEP_db connection error! The schema of connected db is incorrect"""
-        )
+        super().__init__("""PEP_db connection error! The schema of connected db is incorrect""")
 
 
 class RegistryPathError(PEPDatabaseAgentError):
     def __init__(self, msg=""):
         super().__init__(f"""Provided registry path is incorrect. {msg}""")
```

### Comparing `pepdbagent-0.3.0/pepdbagent/models.py` & `pepdbagent-0.4.0/pepdbagent/models.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # file with pydantic models
 import datetime
 from typing import List, Optional
 
-from pydantic import BaseModel, Field, validator, Extra
 import peppy
+from pydantic import BaseModel, Extra, Field, validator
 
 
 class AnnotationModel(BaseModel):
     """
     Project Annotation model. All meta metadata
     """
 
@@ -16,14 +16,15 @@
     tag: Optional[str]
     is_private: Optional[bool]
     number_of_samples: Optional[int]
     description: Optional[str]
     last_update_date: Optional[str]
     submission_date: Optional[str]
     digest: Optional[str]
+    pep_schema: Optional[str]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
 
     @validator("is_private")
     def is_private_should_be_bool(cls, v):
@@ -70,28 +71,44 @@
     Model used for updating individual items in db
     """
 
     project_value: Optional[peppy.Project] = Field(alias="project")
     tag: Optional[str]
     is_private: Optional[bool]
     name: Optional[str]
+    pep_schema: Optional[str]
+
+    class Config:
+        arbitrary_types_allowed = True
 
-    # class Config:
     #     extra = Extra.forbid
 
 
 class UpdateModel(BaseModel):
     """
     !! is Used only by pepdbagent. Don't use it outside
     Model used for updating individual items and creating sql string in the code
     """
 
     project_value: Optional[dict]
-    name: Optional[str]
-    tag: Optional[str]
+    name: Optional[str] = None
+    tag: Optional[str] = None
     private: Optional[bool] = Field(alias="is_private")
     digest: Optional[str]
     last_update_date: Optional[datetime.datetime]
     number_of_samples: Optional[int]
+    pep_schema: Optional[str]
+
+    @validator("tag", "name")
+    def value_must_not_be_empty(cls, v):
+        if "" == v:
+            return None
+        return v
+
+    @validator("tag", "name")
+    def value_must_be_lowercase(cls, v):
+        if v:
+            return v.lower()
+        return v
 
     class Config:
         extra = Extra.forbid
```

### Comparing `pepdbagent-0.3.0/pepdbagent/modules/namespace.py` & `pepdbagent-0.4.0/pepdbagent/modules/namespace.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,39 +1,34 @@
-from typing import Union, List
 import logging
+from typing import List, Union
 
-from pepdbagent.base_connection import BaseConnection
-from pepdbagent.const import (
-    DEFAULT_LIMIT,
-    DEFAULT_OFFSET,
-    NAMESPACE_COL,
-    NAME_COL,
-    N_SAMPLES_COL,
-    DB_TABLE_NAME,
-    PRIVATE_COL,
-)
+from sqlalchemy import distinct, func, or_, select
+from sqlalchemy.sql.selectable import Select
 
+from pepdbagent.const import DEFAULT_LIMIT, DEFAULT_OFFSET, PKG_NAME
+from pepdbagent.db_utils import Projects, BaseEngine
 from pepdbagent.models import Namespace, NamespaceList
 from pepdbagent.utils import tuple_converter
 
-_LOGGER = logging.getLogger("pepdbagent")
+_LOGGER = logging.getLogger(PKG_NAME)
 
 
 class PEPDatabaseNamespace:
     """
     Class that represents project Namespaces in Database.
 
     While using this class, user can retrieve all necessary metadata about PEPs
     """
 
-    def __init__(self, con: BaseConnection):
+    def __init__(self, pep_db_engine: BaseEngine):
         """
-        :param con: Connection to db represented by BaseConnection class object
+        :param pep_db_engine: pepdbengine object with sa engine
         """
-        self.con = con
+        self._sa_engine = pep_db_engine.engine
+        self._pep_db_engine = pep_db_engine
 
     def get(
         self,
         query: str = "",
         admin: Union[List[str], str] = None,
         limit: int = DEFAULT_LIMIT,
         offset: int = DEFAULT_OFFSET,
@@ -48,24 +43,25 @@
             {
                 total number of results
                 search limit
                 search offset
                 search results
             }
         """
-        _LOGGER.info(
-            f"Getting namespaces annotation with provided info: (query: {query})"
-        )
+        _LOGGER.info(f"Getting namespaces annotation with provided info: (query: {query})")
         admin_tuple = tuple_converter(admin)
         return NamespaceList(
             count=self._count_namespace(search_str=query, admin_nsp=admin_tuple),
             limit=limit,
             offset=offset,
             results=self._get_namespace(
-                search_str=query, admin_nsp=admin_tuple, limit=limit, offset=offset
+                search_str=query,
+                admin_nsp=admin_tuple,
+                limit=limit,
+                offset=offset,
             ),
         )
 
     def _get_namespace(
         self,
         search_str: str,
         admin_nsp: tuple = None,
@@ -81,64 +77,82 @@
         :param offset: number of results off set (that were already showed)
         :return: list of dict with structure {
                 namespace,
                 number_of_projects,
                 number_of_samples,
             }
         """
-        if search_str:
-            search_str = f"%%{search_str}%%"
-            search_sql_values = (search_str,)
-            search_sql = f"""{NAMESPACE_COL} ILIKE %s and"""
-        else:
-            search_sql_values = tuple()
-            search_sql = ""
-
-        count_sql = f"""
-        select {NAMESPACE_COL}, COUNT({NAME_COL}), SUM({N_SAMPLES_COL})
-            from {DB_TABLE_NAME} where {search_sql}
-                ({PRIVATE_COL} is %s or {NAMESPACE_COL} in %s) 
-                    GROUP BY {NAMESPACE_COL}
-                        LIMIT %s OFFSET %s;
-        """
-        results = self.con.run_sql_fetchall(
-            count_sql, *search_sql_values, False, admin_nsp, limit, offset
+        statement = (
+            select(
+                Projects.namespace,
+                func.count(Projects.name).label("number_of_projects"),
+                func.sum(Projects.number_of_samples).label("number_of_samples"),
+            )
+            .group_by(Projects.namespace)
+            .select_from(Projects)
         )
+
+        statement = self._add_condition(
+            statement=statement,
+            search_str=search_str,
+            admin_list=admin_nsp,
+        )
+        statement = statement.limit(limit).offset(offset)
+        query_results = self._pep_db_engine.session_execute(statement).all()
+
         results_list = []
-        for res in results:
+        for res in query_results:
             results_list.append(
                 Namespace(
-                    namespace=res[0],
-                    number_of_projects=res[1],
-                    number_of_samples=res[2],
+                    namespace=res.namespace,
+                    number_of_projects=res.number_of_projects,
+                    number_of_samples=res.number_of_samples,
                 )
             )
         return results_list
 
     def _count_namespace(self, search_str: str = None, admin_nsp: tuple = None) -> int:
         """
         Get number of found namespace. [This function is related to _get_namespaces]
         :param search_str: string of symbols, words, keywords to search in the
             namespace name.
         :param admin_nsp: tuple of namespaces where project can be retrieved if they are privet
         :return: number of found namespaces
         """
-        if search_str:
-            search_str = f"%%{search_str}%%"
-            search_sql_values = (search_str,)
-            search_sql = f"""{NAMESPACE_COL} ILIKE %s and"""
-        else:
-            search_sql_values = tuple()
-            search_sql = ""
-        count_sql = f"""
-        select COUNT(DISTINCT ({NAMESPACE_COL}))
-            from {DB_TABLE_NAME} where {search_sql}
-                ({PRIVATE_COL} is %s or {NAMESPACE_COL} in %s) 
+        statement = select(
+            func.count(distinct(Projects.namespace)).label("number_of_namespaces")
+        ).select_from(Projects)
+        statement = self._add_condition(
+            statement=statement,
+            search_str=search_str,
+            admin_list=admin_nsp,
+        )
+
+        query_results = self._pep_db_engine.session_execute(statement).first()
+
+        return query_results.number_of_namespaces
+
+    @staticmethod
+    def _add_condition(
+        statement: Select,
+        search_str: str = None,
+        admin_list: Union[str, List[str]] = None,
+    ) -> Select:
+        """
+        Add where clause to sqlalchemy statement (in namespace search)
+
+        :param statement: sqlalchemy representation of a SELECT statement.
+        :param search_str: search string that has to be found namespace
+        :param admin_list: list or string of admin rights to namespace
+        :return: sqlalchemy representation of a SELECT statement with where clause.
         """
-        result = self.con.run_sql_fetchall(
-            count_sql, *search_sql_values, False, admin_nsp
+        if search_str:
+            sql_search_str = f"%{search_str}%"
+            statement = statement.where(
+                or_(
+                    Projects.namespace.ilike(sql_search_str),
+                )
+            )
+        statement = statement.where(
+            or_(Projects.private.is_(False), Projects.namespace.in_(admin_list))
         )
-        try:
-            number_of_prj = result[0][0]
-        except KeyError:
-            number_of_prj = 0
-        return number_of_prj
+        return statement
```

### Comparing `pepdbagent-0.3.0/pepdbagent/modules/project.py` & `pepdbagent-0.4.0/pepdbagent/modules/project.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,80 +1,89 @@
 import datetime
 import json
-from typing import Union, Tuple
 import logging
+from typing import Tuple, Union
+
 import peppy
-from psycopg2.errors import NotNullViolation, UniqueViolation
+from sqlalchemy import Engine, and_, delete, insert, or_, select, update
+from sqlalchemy.exc import IntegrityError, NoResultFound
 
-from pepdbagent.models import (
-    UpdateModel,
-    UpdateItems,
-)
-from pepdbagent.base_connection import BaseConnection
 from pepdbagent.const import *
+from pepdbagent.db_utils import Projects, BaseEngine
+from pepdbagent.exceptions import ProjectNotFoundError, ProjectUniqueNameError
+from pepdbagent.models import UpdateItems, UpdateModel
 from pepdbagent.utils import create_digest, registry_path_converter
-from pepdbagent.exceptions import (
-    ProjectNotFoundError,
-    ProjectUniqueNameError,
-)
 
-_LOGGER = logging.getLogger("pepdbagent")
+
+_LOGGER = logging.getLogger(PKG_NAME)
 
 
 class PEPDatabaseProject:
     """
     Class that represents Projects in Database.
 
     While using this class, user can retrieve projects from database
     """
 
-    def __init__(self, con: BaseConnection):
+    def __init__(self, pep_db_engine: BaseEngine):
         """
-        :param con: Connection to db represented by BaseConnection class object
+        :param pep_db_engine: pepdbengine object with sa engine
         """
-        self.con = con
+        self._sa_engine = pep_db_engine.engine
+        self._pep_db_engine = pep_db_engine
 
     def get(
         self,
         namespace: str,
         name: str,
-        tag: str = None,
+        tag: str = DEFAULT_TAG,
         raw: bool = False,
     ) -> Union[peppy.Project, dict, None]:
         """
         Retrieve project from database by specifying namespace, name and tag
+
         :param namespace: namespace of the project
         :param name: name of the project (Default: name is taken from the project object)
         :param tag: tag (or version) of the project.
         :param raw: retrieve unprocessed (raw) PEP dict.
         :return: peppy.Project object with found project or dict with unprocessed
             PEP elements: {
                 name: str
                 description: str
                 _config: dict
                 _sample_dict: dict
                 _subsample_dict: dict
             }
         """
-        if tag is None:
-            tag = DEFAULT_TAG
-
-        sql_q = f"""
-                select {ID_COL}, {PROJ_COL}, {PRIVATE_COL} from {DB_TABLE_NAME}
-                """
+        # name = name.lower()
+        namespace = namespace.lower()
+        statement = select(
+            Projects.namespace,
+            Projects.name,
+            Projects.project_value,
+            Projects.private,
+        )
 
-        sql_q = (
-            f""" {sql_q} where {NAME_COL}=%s and {NAMESPACE_COL}=%s and {TAG_COL}=%s;"""
+        statement = statement.where(
+            and_(
+                Projects.namespace == namespace,
+                Projects.name == name,
+                Projects.tag == tag,
+            )
         )
-        found_prj = self.con.run_sql_fetchone(sql_q, name, namespace, tag)
+
+        try:
+            found_prj = self._pep_db_engine.session_execute(statement).one()
+        except NoResultFound:
+            raise ProjectNotFoundError
 
         if found_prj:
-            _LOGGER.info(f"Project has been found: {found_prj[0]}")
-            project_value = found_prj[1]
-            is_private = found_prj[2]
+            _LOGGER.info(f"Project has been found: {found_prj.namespace}, {found_prj.name}")
+            project_value = found_prj.project_value
+            is_private = found_prj.private
             if raw:
                 return project_value
             else:
                 project_obj = peppy.Project().from_dict(project_value)
                 project_obj.is_private = is_private
                 return project_obj
 
@@ -87,14 +96,15 @@
     def get_by_rp(
         self,
         registry_path: str,
         raw: bool = False,
     ) -> Union[peppy.Project, dict, None]:
         """
         Retrieve project from database by specifying project registry_path
+
         :param registry_path: project registry_path [e.g. namespace/name:tag]
         :param raw: retrieve unprocessed (raw) PEP dict.
         :return: peppy.Project object with found project or dict with unprocessed
             PEP elements: {
                 name: str
                 description: str
                 _config: dict
@@ -109,339 +119,326 @@
         self,
         namespace: str = None,
         name: str = None,
         tag: str = None,
     ) -> None:
         """
         Delete record from database
+
         :param namespace: Namespace
         :param name: Name
         :param tag: Tag
         :return: None
         """
-        cursor = self.con.pg_connection.cursor()
-        sql_delete = f"""DELETE FROM {DB_TABLE_NAME} 
-            WHERE {NAMESPACE_COL} = %s and {NAME_COL} = %s and {TAG_COL} = %s;"""
+        # name = name.lower()
+        namespace = namespace.lower()
 
         if not self.exists(namespace=namespace, name=name, tag=tag):
             raise ProjectNotFoundError(
                 f"Can't delete unexciting project: '{namespace}/{name}:{tag}'."
             )
+        with self._sa_engine.begin() as conn:
+            conn.execute(
+                delete(Projects).where(
+                    and_(
+                        Projects.namespace == namespace,
+                        Projects.name == name,
+                        Projects.tag == tag,
+                    )
+                )
+            )
 
-        try:
-            cursor.execute(sql_delete, (namespace, name, tag))
-            _LOGGER.info(f"Project '{namespace}/{name}:{tag} was successfully deleted'")
-        except Exception as err:
-            _LOGGER.error(f"Error while deleting project. Message: {err}")
-        finally:
-            cursor.close()
-            return None
+        _LOGGER.info(f"Project '{namespace}/{name}:{tag} was successfully deleted'")
 
     def delete_by_rp(
         self,
         registry_path: str,
     ) -> None:
         """
         Delete record from database by using registry_path
+
         :param registry_path: Registry path of the project ('namespace/name:tag')
         :return: None
         """
         namespace, name, tag = registry_path_converter(registry_path)
         return self.delete(namespace=namespace, name=name, tag=tag)
 
     def create(
         self,
         project: peppy.Project,
         namespace: str,
         name: str = None,
-        tag: str = None,
+        tag: str = DEFAULT_TAG,
         is_private: bool = False,
+        pep_schema: str = None,
         overwrite: bool = False,
         update_only: bool = False,
     ) -> None:
         """
         Upload project to the database.
         Project with the key, that already exists won't be uploaded(but case, when argument
         update is set True)
+
         :param peppy.Project project: Project object that has to be uploaded to the DB
         :param namespace: namespace of the project (Default: 'other')
         :param name: name of the project (Default: name is taken from the project object)
         :param tag: tag (or version) of the project.
         :param is_private: boolean value if the project should be visible just for user that creates it.
+        :param pep_schema: assign PEP to a specific schema. [DefaultL: None]
         :param overwrite: if project exists overwrite the project, otherwise upload it.
             [Default: False - project won't be overwritten if it exists in db]
         :param update_only: if project exists overwrite it, otherwise do nothing.  [Default: False]
         :return: None
         """
-        cursor = self.con.pg_connection.cursor()
-        if tag is None:
-            tag = DEFAULT_TAG
-
         proj_dict = project.to_dict(extended=True)
 
+        namespace = namespace.lower()
         if name:
+            name = name.lower()
             proj_name = name
+            proj_dict["name"] = name
+        elif proj_dict["name"]:
+            proj_name = proj_dict["name"].lower()
         else:
-            proj_name = proj_dict["name"]
-
-        proj_dict["name"] = name
+            raise ValueError(f"Name of the project wasn't provided. Project will not be uploaded.")
 
         proj_digest = create_digest(proj_dict)
-
         number_of_samples = len(project.samples)
-        proj_dict = json.dumps(proj_dict)
 
         if update_only:
-            _LOGGER.info(
-                f"Update_only argument is set True. Updating project {proj_name} ..."
-            )
+            _LOGGER.info(f"Update_only argument is set True. Updating project {proj_name} ...")
             self._overwrite(
                 project_dict=proj_dict,
                 namespace=namespace,
                 proj_name=proj_name,
                 tag=tag,
                 project_digest=proj_digest,
                 number_of_samples=number_of_samples,
+                private=is_private,
+                pep_schema=pep_schema,
             )
             return None
         else:
             try:
                 _LOGGER.info(f"Uploading {namespace}/{proj_name}:{tag} project...")
 
-                sql_base = f"""INSERT INTO {DB_TABLE_NAME} 
-                ({NAMESPACE_COL}, {NAME_COL}, {TAG_COL}, {DIGEST_COL}, {PROJ_COL}, {N_SAMPLES_COL}, 
-                    {PRIVATE_COL}, {SUBMISSION_DATE_COL}, {LAST_UPDATE_DATE_COL})
-                    VALUES (%s, %s, %s, %s, %s, %s, %s, %s, %s)
-                        RETURNING {ID_COL};"""
-
-                cursor.execute(
-                    sql_base,
-                    (
-                        namespace,
-                        proj_name,
-                        tag,
-                        proj_digest,
-                        proj_dict,
-                        number_of_samples,
-                        is_private,
-                        datetime.datetime.now(),
-                        datetime.datetime.now(),
-                    ),
-                )
-                proj_id = cursor.fetchone()[0]
+                with self._sa_engine.begin() as conn:
+                    conn.execute(
+                        insert(Projects).values(
+                            namespace=namespace,
+                            name=proj_name,
+                            tag=tag,
+                            digest=proj_digest,
+                            project_value=proj_dict,
+                            number_of_samples=number_of_samples,
+                            private=is_private,
+                            submission_date=datetime.datetime.now(datetime.timezone.utc),
+                            last_update_date=datetime.datetime.now(datetime.timezone.utc),
+                            pep_schema=pep_schema,
+                        )
+                    )
 
-                self.con.commit_to_database()
-                cursor.close()
-                _LOGGER.info(
-                    f"Project: '{namespace}/{proj_name}:{tag}' was successfully uploaded."
-                )
                 return None
 
-            except UniqueViolation:
+            except IntegrityError:
                 if overwrite:
                     self._overwrite(
                         project_dict=proj_dict,
                         namespace=namespace,
                         proj_name=proj_name,
                         tag=tag,
                         project_digest=proj_digest,
                         number_of_samples=number_of_samples,
+                        private=is_private,
+                        pep_schema=pep_schema,
                     )
                     return None
+
                 else:
                     raise ProjectUniqueNameError(
                         f"Namespace, name and tag already exists. Project won't be "
                         f"uploaded. Solution: Set overwrite value as True"
                         f" (project will be overwritten), or change tag!"
                     )
 
-            except NotNullViolation as err:
-                raise ValueError(
-                    f"Name of the project wasn't provided. Project will not be uploaded. Error: {err}"
-                )
-
     def _overwrite(
         self,
         project_dict: json,
         namespace: str,
         proj_name: str,
         tag: str,
         project_digest: str,
         number_of_samples: int,
+        private: bool = False,
+        pep_schema: str = None,
     ) -> None:
         """
         Update existing project by providing all necessary information.
+
         :param project_dict: project dictionary in json format
         :param namespace: project namespace
         :param proj_name: project name
         :param tag: project tag
         :param project_digest: project digest
         :param number_of_samples: number of samples in project
+        :param private: boolean value if the project should be visible just for user that creates it.
+        :param pep_schema: assign PEP to a specific schema. [DefaultL: None]
         :return: None
         """
-
-        cursor = self.con.pg_connection.cursor()
-
+        proj_name = proj_name.lower()
+        namespace = namespace.lower()
         if self.exists(namespace=namespace, name=proj_name, tag=tag):
             _LOGGER.info(f"Updating {proj_name} project...")
-            sql = f"""UPDATE {DB_TABLE_NAME}
-                SET {DIGEST_COL} = %s, {PROJ_COL}= %s, {N_SAMPLES_COL}= %s, {LAST_UPDATE_DATE_COL} = %s
-                WHERE {NAMESPACE_COL} = %s and {NAME_COL} = %s and {TAG_COL} = %s;"""
-            cursor.execute(
-                sql,
-                (
-                    project_digest,
-                    project_dict,
-                    number_of_samples,
-                    datetime.datetime.now(),
-                    namespace,
-                    proj_name,
-                    tag,
-                ),
-            )
-            self.con.commit_to_database()
-            _LOGGER.info(
-                f"Project '{namespace}/{proj_name}:{tag}' has been updated successfully!"
-            )
+            with self._sa_engine.begin() as conn:
+                conn.execute(
+                    update(Projects)
+                    .values(
+                        namespace=namespace,
+                        name=proj_name,
+                        tag=tag,
+                        digest=project_digest,
+                        project_value=project_dict,
+                        number_of_samples=number_of_samples,
+                        private=private,
+                        last_update_date=datetime.datetime.now(datetime.timezone.utc),
+                        pep_schema=pep_schema,
+                    )
+                    .where(
+                        and_(
+                            Projects.namespace == namespace,
+                            Projects.name == proj_name,
+                            Projects.tag == tag,
+                        )
+                    )
+                )
+
+            _LOGGER.info(f"Project '{namespace}/{proj_name}:{tag}' has been successfully updated!")
             return None
 
         else:
-            raise ProjectNotFoundError(
-                "Project does not exist! No project will be updated!"
-            )
+            raise ProjectNotFoundError("Project does not exist! No project will be updated!")
 
     def update(
         self,
         update_dict: Union[dict, UpdateItems],
         namespace: str,
         name: str,
-        tag: str,
+        tag: str = DEFAULT_TAG,
     ) -> None:
         """
         Update partial parts of the record in db
+
         :param update_dict: dict with update key->values. Dict structure:
             {
                     project: Optional[peppy.Project]
                     is_private: Optional[bool]
                     tag: Optional[str]
                     name: Optional[str]
             }
             *project_value should contain name and description
         :param namespace: project namespace
         :param name: project name
         :param tag: project tag
         :return: None
         """
-        cursor = self.con.pg_connection.cursor()
-
-        if isinstance(update_dict, UpdateItems):
-            update_values = update_dict
-        else:
-            update_values = UpdateItems(**update_dict)
-
         if self.exists(namespace=namespace, name=name, tag=tag):
-            update_final = UpdateModel()
-
-            if update_values.project_value is not None:
-                update_final = UpdateModel(
-                    project_value=update_values.project_value.to_dict(extended=True),
-                    name=update_values.project_value.name,
-                    digest=create_digest(
-                        update_values.project_value.to_dict(extended=True)
-                    ),
-                    last_update_date=datetime.datetime.now(),
-                    number_of_samples=len(update_values.project_value.samples),
-                )
+            if isinstance(update_dict, UpdateItems):
+                update_values = update_dict
+            else:
+                update_values = UpdateItems(**update_dict)
 
-            if update_values.tag is not None:
-                update_final = UpdateModel(
-                    tag=update_values.tag, **update_final.dict(exclude_unset=True)
-                )
+            update_values = self.__create_update_dict(update_values)
 
-            if update_values.is_private is not None:
-                update_final = UpdateModel(
-                    is_private=update_values.is_private,
-                    **update_final.dict(exclude_unset=True),
+            update_stmt = (
+                update(Projects)
+                .where(
+                    and_(
+                        Projects.namespace == namespace,
+                        Projects.name == name,
+                        Projects.tag == tag,
+                    )
                 )
+                .values(update_values)
+            )
 
-            if update_values.name is not None:
-                update_final = UpdateModel(
-                    name=update_values.name, **update_final.dict(exclude_unset=True)
-                )
+            with self._sa_engine.begin() as conn:
+                conn.execute(update_stmt)
 
-            set_sql, set_values = self.__create_update_set(update_final)
-            sql = f"""UPDATE {DB_TABLE_NAME}
-                {set_sql}
-                WHERE {NAMESPACE_COL} = %s and {NAME_COL} = %s and {TAG_COL} = %s;"""
-            _LOGGER.debug("Updating items...")
-            cursor.execute(
-                sql,
-                (*set_values, namespace, name, tag),
-            )
-            _LOGGER.info(f"Record '{namespace}/{name}:{tag}' was successfully updated!")
-            self.con.commit_to_database()
+            return None
 
         else:
             raise ProjectNotFoundError("No items will be updated!")
 
-        return None
-
     @staticmethod
-    def __create_update_set(update_info: UpdateModel) -> Tuple[str, tuple]:
+    def __create_update_dict(update_values: UpdateItems) -> dict:
         """
-        Create sql SET string by passing UpdateModel that later is converted to dict
-        :param update_info: UpdateModel (similar to database model)
-        :return: {sql_string (contains db keys) and updating values}
-        """
-        _LOGGER.debug("Creating SET SQL string to update project")
-        sql_string = f"""SET """
-        sql_values = []
-
-        first = True
-        for key, val in update_info.dict(exclude_none=True).items():
-            if first:
-                sql_string = "".join([sql_string, f"{key} = %s"])
-                first = False
-            else:
-                sql_string = ", ".join([sql_string, f"{key} = %s"])
+        Modify keys and values that set for update and create unified
+        dictionary of the values that have to be updated
 
-            if isinstance(val, dict):
-                input_val = json.dumps(val)
-            else:
-                input_val = val
+         :param update_values: UpdateItems (pydantic class) with
+            updating values
+        :return: unified update dict
+        """
+        update_final = UpdateModel()
+
+        if update_values.project_value is not None:
+            update_final = UpdateModel(
+                project_value=update_values.project_value.to_dict(extended=True),
+                name=update_values.project_value.name,
+                digest=create_digest(update_values.project_value.to_dict(extended=True)),
+                last_update_date=datetime.datetime.now(datetime.timezone.utc),
+                number_of_samples=len(update_values.project_value.samples),
+            )
+
+        if update_values.tag is not None:
+            update_final = UpdateModel(
+                tag=update_values.tag, **update_final.dict(exclude_unset=True)
+            )
+
+        if update_values.is_private is not None:
+            update_final = UpdateModel(
+                is_private=update_values.is_private,
+                **update_final.dict(exclude_unset=True),
+            )
 
-            sql_values.append(input_val)
+        if update_values.name is not None:
+            update_final = UpdateModel(
+                name=update_values.name,
+                **update_final.dict(exclude_unset=True),
+            )
 
-        return sql_string, tuple(sql_values)
+        if update_values.pep_schema is not None:
+            update_final = UpdateModel(
+                pep_schema=update_values.pep_schema,
+                **update_final.dict(exclude_unset=True),
+            )
+
+        return update_final.dict(exclude_unset=True, exclude_none=True)
 
     def exists(
         self,
-        namespace: str = None,
-        name: str = None,
-        tag: str = None,
+        namespace: str,
+        name: str,
+        tag: str = DEFAULT_TAG,
     ) -> bool:
         """
         Check if project exists in the database.
         :param namespace: project namespace
         :param name: project name
         :param tag: project tag
         :return: Returning True if project exist
         """
-        if namespace is None:
-            namespace = DEFAULT_NAMESPACE
-
-        if tag is None:
-            tag = DEFAULT_TAG
 
-        if name is None:
-            _LOGGER.error(f"Name is not specified")
-            return False
-
-        sql = f"""SELECT {ID_COL} from {DB_TABLE_NAME} 
-                    WHERE {NAMESPACE_COL} = %s AND
-                          {NAME_COL} = %s AND 
-                          {TAG_COL} = %s;"""
+        statement = select(Projects.id)
+        statement = statement.where(
+            and_(
+                Projects.namespace == namespace,
+                Projects.name == name,
+                Projects.tag == tag,
+            )
+        )
+        found_prj = self._pep_db_engine.session_execute(statement).all()
 
-        if self.con.run_sql_fetchone(sql, namespace, name, tag):
+        if len(found_prj) > 0:
             return True
         else:
             return False
```

### Comparing `pepdbagent-0.3.0/pepdbagent/pepdbagent.py` & `pepdbagent-0.4.0/pepdbagent/pepdbagent.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,48 +1,56 @@
-from pepdbagent.base_connection import BaseConnection
+from pepdbagent.const import POSTGRES_DIALECT
+from pepdbagent.db_utils import BaseEngine
 from pepdbagent.modules.annotation import PEPDatabaseAnnotation
-from pepdbagent.modules.project import PEPDatabaseProject
 from pepdbagent.modules.namespace import PEPDatabaseNamespace
+from pepdbagent.modules.project import PEPDatabaseProject
 
 
 class PEPDatabaseAgent(object):
     def __init__(
         self,
         host="localhost",
         port=5432,
         database="pep-db",
         user=None,
         password=None,
+        drivername=POSTGRES_DIALECT,
         dsn=None,
+        echo=False,
     ):
         """
         Initialize connection to the pep_db database. You can use The basic connection parameters
         or libpq connection string.
         :param host: database server address e.g., localhost or an IP address.
         :param port: the port number that defaults to 5432 if it is not provided.
         :param database: the name of the database that you want to connect.
         :param user: the username used to authenticate.
         :param password: password used to authenticate.
+        :param drivername: driver of the database [Default: postgresql]
         :param dsn: libpq connection string using the dsn parameter
         (e.g. "localhost://username:password@pdp_db:5432")
         """
 
-        con = BaseConnection(
+        pep_db_engine = BaseEngine(
             host=host,
             port=port,
             database=database,
             user=user,
             password=password,
+            drivername=drivername,
             dsn=dsn,
+            echo=echo,
         )
-        self.__con = con
+        sa_engine = pep_db_engine.engine
 
-        self.__project = PEPDatabaseProject(con)
-        self.__annotation = PEPDatabaseAnnotation(con)
-        self.__namespace = PEPDatabaseNamespace(con)
+        self.__sa_engine = sa_engine
+
+        self.__project = PEPDatabaseProject(pep_db_engine)
+        self.__annotation = PEPDatabaseAnnotation(pep_db_engine)
+        self.__namespace = PEPDatabaseNamespace(pep_db_engine)
 
         self.__db_name = database
 
     @property
     def project(self):
         return self.__project
 
@@ -53,16 +61,13 @@
     @property
     def namespace(self):
         return self.__namespace
 
     def __str__(self):
         return f"Connection to the database: '{self.__db_name}' is set!"
 
-    def __del__(self):
-        self.__con.__del__()
-
     def __exit__(self):
-        self.__con.__exit__()
+        self.__sa_engine.__exit__()
 
     @property
     def connection(self):
-        return self.__con
+        return self.__sa_engine
```

### Comparing `pepdbagent-0.3.0/pepdbagent/utils.py` & `pepdbagent-0.4.0/pepdbagent/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,15 @@
-from collections.abc import Iterable
 import json
+from collections.abc import Iterable
 from hashlib import md5
 from typing import Tuple, Union
+
 import ubiquerg
+from peppy.const import SAMPLE_RAW_DICT_KEY
+
 from .exceptions import RegistryPathError
 
 
 def is_valid_registry_path(rpath: str) -> bool:
     """
     Verify that a registry path is valid. Checks for two things:
     1. Contains forward slash ("/"), and
@@ -38,32 +41,34 @@
         return False
     return all([isinstance(item, str) for item in iterable])
 
 
 def create_digest(project_dict: dict) -> str:
     """
     Create digest for PEP project
+
     :param project_dict: project dict
     :return: digest string
     """
     sample_digest = md5(
         json.dumps(
-            project_dict["_sample_dict"],
+            project_dict[SAMPLE_RAW_DICT_KEY],
             separators=(",", ":"),
             ensure_ascii=False,
             allow_nan=False,
             sort_keys=True,
         ).encode("utf-8")
     ).hexdigest()
     return sample_digest
 
 
 def registry_path_converter(registry_path: str) -> Tuple[str, str, str]:
     """
     Convert registry path to namespace, name, tag
+
     :param registry_path: registry path that has structure: "namespace/name:tag"
     :return: tuple(namespace, name, tag)
     """
     if is_valid_registry_path(registry_path):
         reg = ubiquerg.parse_registry_path(registry_path)
         namespace = reg["namespace"]
         name = reg["item"]
@@ -73,14 +78,15 @@
     raise RegistryPathError(f"Error in: '{registry_path}'")
 
 
 def tuple_converter(value: Union[tuple, list, str, None]) -> tuple:
     """
     Convert string list or tuple to tuple.
     # is used to create admin tuple.
+
     :param value: Any value that has to be converted to tuple
     :return: tuple of strings
     """
     if isinstance(value, str):
         value = [value]
     if value:
         return tuple(value)
```

### Comparing `pepdbagent-0.3.0/pepdbagent.egg-info/PKG-INFO` & `pepdbagent-0.4.0/pepdbagent.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: pepdbagent
-Version: 0.3.0
+Version: 0.4.0
 Summary: A python-based project metadata manager for portable encapsulated projects
 Home-page: https://github.com/pepkit/pepdbagent/
 Author: Oleksandr Khoroshevskyi
 License: BSD2
 Keywords: project,metadata,bioinformatics,database
-Classifier: Development Status :: 1 - Planning
+Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # pepdbagent
 
-pepdbagent is a python library and toolkit that gives a user user-friendly 
+`pepdbagent` is a Python library and toolkit that gives a user-friendly 
 interface to connect, upload, update and retrieve information from pep-db.
 
-**pep-db** is and postgres database created for storing [PEPs](http://pep.databio.org/en/latest/). 
-It is a backend database for PEPhub. database enables storing huge projects and provides fast speed of retrieving them.
+**pep-db** is a postgres database created for storing [PEPs](http://pep.databio.org/en/latest/). 
+It is a backend database for PEPhub. 
 
-Before using pepdbagent, you should install or have access to pep-db.
+Before using pepdbagent, you should install or have access to a pep-db instance.
 
-To install pep-db you can use this tutorial:
+To run a pep-db instance, you can use this tutorial:
 - [pep-db installation](./docs/db_tutorial.md)
 
-
-pepdbagent tutorial is here:
+Then, follow the `pepdbagent` tutorial here:
 - [pedbagent](./docs/README.md)
```

### Comparing `pepdbagent-0.3.0/pepdbagent.egg-info/SOURCES.txt` & `pepdbagent-0.4.0/pepdbagent.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 LICENSE.txt
 MANIFEST.in
 README.md
+pyproject.toml
 setup.py
 pepdbagent/__init__.py
 pepdbagent/_version.py
-pepdbagent/base_connection.py
 pepdbagent/const.py
+pepdbagent/db_utils.py
 pepdbagent/exceptions.py
 pepdbagent/models.py
 pepdbagent/pepdbagent.py
 pepdbagent/utils.py
 pepdbagent.egg-info/PKG-INFO
 pepdbagent.egg-info/SOURCES.txt
 pepdbagent.egg-info/dependency_links.txt
```

### Comparing `pepdbagent-0.3.0/setup.py` & `pepdbagent-0.4.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-import sys
 import os
+import sys
+
 from setuptools import find_packages, setup
 
 PACKAGE_NAME = "pepdbagent"
 
 # Ordinary dependencies
 DEPENDENCIES = []
 with open("requirements/requirements-all.txt", "r") as reqs_file:
@@ -12,21 +13,20 @@
             continue
         # DEPENDENCIES.append(line.split("=")[0].rstrip("<>"))
         DEPENDENCIES.append(line)
 
 # Additional keyword arguments for setup().
 extra = {"install_requires": DEPENDENCIES}
 
+
 # Additional files to include with package
 def get_static(name, condition=None):
     static = [
         os.path.join(name, f)
-        for f in os.listdir(
-            os.path.join(os.path.dirname(os.path.realpath(__file__)), name)
-        )
+        for f in os.listdir(os.path.join(os.path.dirname(os.path.realpath(__file__)), name))
     ]
     if condition is None:
         return static
     else:
         return [i for i in filter(lambda x: eval(condition), static)]
 
 
@@ -40,25 +40,24 @@
     name=PACKAGE_NAME,
     packages=find_packages(),
     version=version,
     description="A python-based project metadata manager for portable encapsulated projects",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
-        "Development Status :: 1 - Planning",
+        "Development Status :: 3 - Alpha",
         "License :: OSI Approved :: BSD License",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Topic :: Scientific/Engineering :: Bio-Informatics",
     ],
     keywords="project, metadata, bioinformatics, database",
     url="https://github.com/pepkit/pepdbagent/",
     author="Oleksandr Khoroshevskyi",
     license="BSD2",
     include_package_data=True,
     # tests_require=(["pytest"]),
-    setup_requires=(
-        ["pytest-runner"] if {"test", "pytest", "ptr"} & set(sys.argv) else []
-    ),
+    setup_requires=(["pytest-runner"] if {"test", "pytest", "ptr"} & set(sys.argv) else []),
     **extra,
 )
```

