# Comparing `tmp/monarch_py-0.9.1.tar.gz` & `tmp/monarch_py-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monarch_py-0.9.1.tar", max compression
+gzip compressed data, was "monarch_py-0.9.2.tar", max compression
```

## Comparing `monarch_py-0.9.1.tar` & `monarch_py-0.9.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0      974 2023-06-07 21:31:17.078236 monarch_py-0.9.1/pyproject.toml
--rw-r--r--   0        0        0       77 2023-06-07 21:31:17.078236 monarch_py-0.9.1/src/monarch_py/__init__.py
--rw-r--r--   0        0        0     1150 2023-06-07 21:31:17.078236 monarch_py-0.9.1/src/monarch_py/association_type_mappings.yaml
--rw-r--r--   0        0        0     7464 2023-06-07 21:31:17.078236 monarch_py-0.9.1/src/monarch_py/cli.py
--rw-r--r--   0        0        0        0 2023-06-07 21:31:17.078236 monarch_py-0.9.1/src/monarch_py/datamodels/__init__.py
--rw-r--r--   0        0        0    11302 2023-06-07 21:31:17.078236 monarch_py-0.9.1/src/monarch_py/datamodels/model.py
--rw-r--r--   0        0        0     7486 2023-06-07 21:31:17.078236 monarch_py-0.9.1/src/monarch_py/datamodels/model.yaml
--rw-r--r--   0        0        0     3321 2023-06-07 21:31:17.078236 monarch_py-0.9.1/src/monarch_py/datamodels/solr.py
--rw-r--r--   0        0        0        0 2023-06-07 21:31:17.078236 monarch_py-0.9.1/src/monarch_py/implementations/__init__.py
--rw-r--r--   0        0        0        0 2023-06-07 21:31:17.078236 monarch_py-0.9.1/src/monarch_py/implementations/solr/__init__.py
--rw-r--r--   0        0        0    20304 2023-06-07 21:31:17.078236 monarch_py-0.9.1/src/monarch_py/implementations/solr/solr_implementation.py
--rw-r--r--   0        0        0        0 2023-06-07 21:31:17.078236 monarch_py-0.9.1/src/monarch_py/implementations/sql/__init__.py
--rw-r--r--   0        0        0     8909 2023-06-07 21:31:17.082236 monarch_py-0.9.1/src/monarch_py/implementations/sql/sql_implementation.py
--rw-r--r--   0        0        0        0 2023-06-07 21:31:17.082236 monarch_py-0.9.1/src/monarch_py/interfaces/__init__.py
--rw-r--r--   0        0        0     2343 2023-06-07 21:31:17.082236 monarch_py-0.9.1/src/monarch_py/interfaces/association_interface.py
--rw-r--r--   0        0        0      985 2023-06-07 21:31:17.082236 monarch_py-0.9.1/src/monarch_py/interfaces/entity_interface.py
--rw-r--r--   0        0        0      890 2023-06-07 21:31:17.082236 monarch_py-0.9.1/src/monarch_py/interfaces/query_interface.py
--rw-r--r--   0        0        0     4630 2023-06-07 21:31:17.082236 monarch_py-0.9.1/src/monarch_py/interfaces/search_interface.py
--rw-r--r--   0        0        0        0 2023-06-07 21:31:17.082236 monarch_py-0.9.1/src/monarch_py/service/__init__.py
--rw-r--r--   0        0        0     2052 2023-06-07 21:31:17.082236 monarch_py-0.9.1/src/monarch_py/service/solr_service.py
--rw-r--r--   0        0        0     9254 2023-06-07 21:31:17.082236 monarch_py-0.9.1/src/monarch_py/solr_cli.py
--rw-r--r--   0        0        0     3330 2023-06-07 21:31:17.082236 monarch_py-0.9.1/src/monarch_py/sql_cli.py
--rw-r--r--   0        0        0        0 2023-06-07 21:31:17.082236 monarch_py-0.9.1/src/monarch_py/utils/__init__.py
--rw-r--r--   0        0        0     3145 2023-06-07 21:31:17.082236 monarch_py-0.9.1/src/monarch_py/utils/association_type_utils.py
--rw-r--r--   0        0        0     3985 2023-06-07 21:31:17.082236 monarch_py-0.9.1/src/monarch_py/utils/solr_cli_utils.py
--rw-r--r--   0        0        0     4937 2023-06-07 21:31:17.082236 monarch_py-0.9.1/src/monarch_py/utils/utils.py
--rw-r--r--   0        0        0      750 1970-01-01 00:00:00.000000 monarch_py-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0      974 2023-06-09 17:43:33.748506 monarch_py-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0       77 2023-06-09 17:43:33.748506 monarch_py-0.9.2/src/monarch_py/__init__.py
+-rw-r--r--   0        0        0     1150 2023-06-09 17:43:33.748506 monarch_py-0.9.2/src/monarch_py/association_type_mappings.yaml
+-rw-r--r--   0        0        0     7464 2023-06-09 17:43:33.748506 monarch_py-0.9.2/src/monarch_py/cli.py
+-rw-r--r--   0        0        0        0 2023-06-09 17:43:33.748506 monarch_py-0.9.2/src/monarch_py/datamodels/__init__.py
+-rw-r--r--   0        0        0    11302 2023-06-09 17:43:33.748506 monarch_py-0.9.2/src/monarch_py/datamodels/model.py
+-rw-r--r--   0        0        0     7540 2023-06-09 17:43:33.748506 monarch_py-0.9.2/src/monarch_py/datamodels/model.yaml
+-rw-r--r--   0        0        0     3321 2023-06-09 17:43:33.748506 monarch_py-0.9.2/src/monarch_py/datamodels/solr.py
+-rw-r--r--   0        0        0        0 2023-06-09 17:43:33.748506 monarch_py-0.9.2/src/monarch_py/implementations/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-09 17:43:33.748506 monarch_py-0.9.2/src/monarch_py/implementations/solr/__init__.py
+-rw-r--r--   0        0        0    20304 2023-06-09 17:43:33.748506 monarch_py-0.9.2/src/monarch_py/implementations/solr/solr_implementation.py
+-rw-r--r--   0        0        0        0 2023-06-09 17:43:33.748506 monarch_py-0.9.2/src/monarch_py/implementations/sql/__init__.py
+-rw-r--r--   0        0        0     8909 2023-06-09 17:43:33.748506 monarch_py-0.9.2/src/monarch_py/implementations/sql/sql_implementation.py
+-rw-r--r--   0        0        0        0 2023-06-09 17:43:33.748506 monarch_py-0.9.2/src/monarch_py/interfaces/__init__.py
+-rw-r--r--   0        0        0     2343 2023-06-09 17:43:33.748506 monarch_py-0.9.2/src/monarch_py/interfaces/association_interface.py
+-rw-r--r--   0        0        0      985 2023-06-09 17:43:33.748506 monarch_py-0.9.2/src/monarch_py/interfaces/entity_interface.py
+-rw-r--r--   0        0        0      890 2023-06-09 17:43:33.748506 monarch_py-0.9.2/src/monarch_py/interfaces/query_interface.py
+-rw-r--r--   0        0        0     4630 2023-06-09 17:43:33.748506 monarch_py-0.9.2/src/monarch_py/interfaces/search_interface.py
+-rw-r--r--   0        0        0        0 2023-06-09 17:43:33.748506 monarch_py-0.9.2/src/monarch_py/service/__init__.py
+-rw-r--r--   0        0        0     1954 2023-06-09 17:43:33.748506 monarch_py-0.9.2/src/monarch_py/service/solr_service.py
+-rw-r--r--   0        0        0     9254 2023-06-09 17:43:33.748506 monarch_py-0.9.2/src/monarch_py/solr_cli.py
+-rw-r--r--   0        0        0     3330 2023-06-09 17:43:33.748506 monarch_py-0.9.2/src/monarch_py/sql_cli.py
+-rw-r--r--   0        0        0        0 2023-06-09 17:43:33.748506 monarch_py-0.9.2/src/monarch_py/utils/__init__.py
+-rw-r--r--   0        0        0     3145 2023-06-09 17:43:33.748506 monarch_py-0.9.2/src/monarch_py/utils/association_type_utils.py
+-rw-r--r--   0        0        0     3985 2023-06-09 17:43:33.748506 monarch_py-0.9.2/src/monarch_py/utils/solr_cli_utils.py
+-rw-r--r--   0        0        0     4937 2023-06-09 17:43:33.748506 monarch_py-0.9.2/src/monarch_py/utils/utils.py
+-rw-r--r--   0        0        0      750 1970-01-01 00:00:00.000000 monarch_py-0.9.2/PKG-INFO
```

### Comparing `monarch_py-0.9.1/pyproject.toml` & `monarch_py-0.9.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "monarch-py"
-version = "0.9.1"
+version = "0.9.2"
 description = "Monarch Initiative data access library"
 authors = [
     "Kevin Schaper <kevin@tislab.org>",
     "Glass Elsarboukh <glass@tislab.org>",
     "The Monarch Initiative <info@monarchinitiative.org>"
 ]
 packages = [
```

### Comparing `monarch_py-0.9.1/src/monarch_py/association_type_mappings.yaml` & `monarch_py-0.9.2/src/monarch_py/association_type_mappings.yaml`

 * *Files identical despite different names*

### Comparing `monarch_py-0.9.1/src/monarch_py/cli.py` & `monarch_py-0.9.2/src/monarch_py/cli.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.9.1/src/monarch_py/datamodels/model.py` & `monarch_py-0.9.2/src/monarch_py/datamodels/model.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.9.1/src/monarch_py/datamodels/model.yaml` & `monarch_py-0.9.2/src/monarch_py/datamodels/model.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -201,24 +201,27 @@
       The directionality of the association relative to a given entity for an association_count.
       If the entity is the subject or in the subject closure, the direction is forwards, if it is
       the object or in the object closure, the direction is backwards.
     range: AssociationDirectionEnum
     required: true
   facet_fields:
     description: Collection of facet field responses with the field values and counts
+    inlined: true
     inlined_as_list: true
     multivalued: true
     range: FacetField
   facet_queries:
     description: Collection of facet query responses with the query string values and counts
+    inlined: true
     inlined_as_list: true
     multivalued: true
     range: FacetValue
   facet_values:
     description: Collection of FacetValue label/value instances belonging to a FacetField
+    inlined: true
     inlined_as_list: true
     multivalued: true
     range: FacetValue
   frequency_qualifier:
     range: string
   has_evidence:
     range: string
```

### Comparing `monarch_py-0.9.1/src/monarch_py/datamodels/solr.py` & `monarch_py-0.9.2/src/monarch_py/datamodels/solr.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.9.1/src/monarch_py/implementations/solr/solr_implementation.py` & `monarch_py-0.9.2/src/monarch_py/implementations/solr/solr_implementation.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.9.1/src/monarch_py/implementations/sql/sql_implementation.py` & `monarch_py-0.9.2/src/monarch_py/implementations/sql/sql_implementation.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.9.1/src/monarch_py/interfaces/association_interface.py` & `monarch_py-0.9.2/src/monarch_py/interfaces/association_interface.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.9.1/src/monarch_py/interfaces/entity_interface.py` & `monarch_py-0.9.2/src/monarch_py/interfaces/entity_interface.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.9.1/src/monarch_py/interfaces/query_interface.py` & `monarch_py-0.9.2/src/monarch_py/interfaces/query_interface.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.9.1/src/monarch_py/interfaces/search_interface.py` & `monarch_py-0.9.2/src/monarch_py/interfaces/search_interface.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.9.1/src/monarch_py/service/solr_service.py` & `monarch_py-0.9.2/src/monarch_py/service/solr_service.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,33 +2,31 @@
 from typing import Dict, List
 
 import requests
 from loguru import logger
 from pydantic import BaseModel
 
 from monarch_py.datamodels.solr import SolrQuery, SolrQueryResult, core
-from monarch_py.utils.utils import console, escape
+from monarch_py.utils.utils import escape
 
 
 class SolrService(BaseModel):
     base_url: str
     core: core
 
     def get(self, id):
         url = f"{self.base_url}/{self.core.value}/get?id={id}"
-        console.log(f"Solr request: {url}")
         response = requests.get(url)
         response.raise_for_status()
         entity = response.json()["doc"]
         self._strip_json(entity, "_version_")
         return entity
 
     def query(self, q: SolrQuery) -> SolrQueryResult:
         url = f"{self.base_url}/{self.core.value}/select?{q.query_string()}"
-        logger.debug(f"Solr request: {url}")
         response = requests.get(url)
 
         data = json.loads(response.text)
         if "error" in data:
             logger.error("Solr error message: " + data["error"]["msg"])
         response.raise_for_status()
         solr_query_result = SolrQueryResult.parse_obj(data)
```

### Comparing `monarch_py-0.9.1/src/monarch_py/solr_cli.py` & `monarch_py-0.9.2/src/monarch_py/solr_cli.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.9.1/src/monarch_py/sql_cli.py` & `monarch_py-0.9.2/src/monarch_py/sql_cli.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.9.1/src/monarch_py/utils/association_type_utils.py` & `monarch_py-0.9.2/src/monarch_py/utils/association_type_utils.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.9.1/src/monarch_py/utils/solr_cli_utils.py` & `monarch_py-0.9.2/src/monarch_py/utils/solr_cli_utils.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.9.1/src/monarch_py/utils/utils.py` & `monarch_py-0.9.2/src/monarch_py/utils/utils.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.9.1/PKG-INFO` & `monarch_py-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monarch-py
-Version: 0.9.1
+Version: 0.9.2
 Summary: Monarch Initiative data access library
 Author: Kevin Schaper
 Author-email: kevin@tislab.org
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

