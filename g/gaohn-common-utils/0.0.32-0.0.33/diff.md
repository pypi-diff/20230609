# Comparing `tmp/gaohn-common-utils-0.0.32.tar.gz` & `tmp/gaohn-common-utils-0.0.33.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gaohn-common-utils-0.0.32.tar", last modified: Fri Jun  9 06:47:15 2023, max compression
+gzip compressed data, was "gaohn-common-utils-0.0.33.tar", last modified: Fri Jun  9 07:31:06 2023, max compression
```

## Comparing `gaohn-common-utils-0.0.32.tar` & `gaohn-common-utils-0.0.33.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:47:15.337285 gaohn-common-utils-0.0.32/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-09 06:46:58.000000 gaohn-common-utils-0.0.32/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-09 06:47:15.337285 gaohn-common-utils-0.0.32/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-09 06:46:58.000000 gaohn-common-utils-0.0.32/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:47:15.337285 gaohn-common-utils-0.0.32/common_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 06:46:58.000000 gaohn-common-utils-0.0.32/common_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:47:15.337285 gaohn-common-utils-0.0.32/common_utils/cloud/
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-09 06:46:58.000000 gaohn-common-utils-0.0.32/common_utils/cloud/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:47:15.333285 gaohn-common-utils-0.0.32/common_utils/cloud/gcp/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:47:15.337285 gaohn-common-utils-0.0.32/common_utils/cloud/gcp/storage/
--rw-r--r--   0 runner    (1001) docker     (123)     4912 2023-06-09 06:46:58.000000 gaohn-common-utils-0.0.32/common_utils/cloud/gcp/storage/bigquery.py
--rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-06-09 06:46:58.000000 gaohn-common-utils-0.0.32/common_utils/cloud/gcp/storage/gcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:47:15.337285 gaohn-common-utils-0.0.32/common_utils/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 06:46:58.000000 gaohn-common-utils-0.0.32/common_utils/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-06-09 06:46:58.000000 gaohn-common-utils-0.0.32/common_utils/core/artifacts.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-09 06:46:58.000000 gaohn-common-utils-0.0.32/common_utils/core/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5148 2023-06-09 06:46:58.000000 gaohn-common-utils-0.0.32/common_utils/core/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-06-09 06:46:58.000000 gaohn-common-utils-0.0.32/common_utils/core/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-06-09 06:46:58.000000 gaohn-common-utils-0.0.32/common_utils/core/file_system_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-06-09 06:46:58.000000 gaohn-common-utils-0.0.32/common_utils/core/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:47:15.333285 gaohn-common-utils-0.0.32/common_utils/versioning/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:47:15.337285 gaohn-common-utils-0.0.32/common_utils/versioning/dvc/
--rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-06-09 06:46:58.000000 gaohn-common-utils-0.0.32/common_utils/versioning/dvc/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:47:15.337285 gaohn-common-utils-0.0.32/gaohn_common_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-09 06:47:15.000000 gaohn-common-utils-0.0.32/gaohn_common_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-09 06:47:15.000000 gaohn-common-utils-0.0.32/gaohn_common_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 06:47:15.000000 gaohn-common-utils-0.0.32/gaohn_common_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-09 06:47:15.000000 gaohn-common-utils-0.0.32/gaohn_common_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-09 06:47:15.000000 gaohn-common-utils-0.0.32/gaohn_common_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-06-09 06:46:58.000000 gaohn-common-utils-0.0.32/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 06:47:15.337285 gaohn-common-utils-0.0.32/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:31:06.152463 gaohn-common-utils-0.0.33/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-09 07:30:48.000000 gaohn-common-utils-0.0.33/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-09 07:31:06.148463 gaohn-common-utils-0.0.33/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-09 07:30:48.000000 gaohn-common-utils-0.0.33/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:31:06.148463 gaohn-common-utils-0.0.33/common_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 07:30:48.000000 gaohn-common-utils-0.0.33/common_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:31:06.148463 gaohn-common-utils-0.0.33/common_utils/cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-09 07:30:48.000000 gaohn-common-utils-0.0.33/common_utils/cloud/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:31:06.148463 gaohn-common-utils-0.0.33/common_utils/cloud/gcp/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:31:06.148463 gaohn-common-utils-0.0.33/common_utils/cloud/gcp/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-06-09 07:30:48.000000 gaohn-common-utils-0.0.33/common_utils/cloud/gcp/storage/bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-06-09 07:30:48.000000 gaohn-common-utils-0.0.33/common_utils/cloud/gcp/storage/gcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:31:06.148463 gaohn-common-utils-0.0.33/common_utils/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 07:30:48.000000 gaohn-common-utils-0.0.33/common_utils/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-06-09 07:30:48.000000 gaohn-common-utils-0.0.33/common_utils/core/artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-09 07:30:48.000000 gaohn-common-utils-0.0.33/common_utils/core/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5148 2023-06-09 07:30:48.000000 gaohn-common-utils-0.0.33/common_utils/core/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-06-09 07:30:48.000000 gaohn-common-utils-0.0.33/common_utils/core/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-06-09 07:30:48.000000 gaohn-common-utils-0.0.33/common_utils/core/file_system_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-06-09 07:30:48.000000 gaohn-common-utils-0.0.33/common_utils/core/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:31:06.148463 gaohn-common-utils-0.0.33/common_utils/versioning/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:31:06.148463 gaohn-common-utils-0.0.33/common_utils/versioning/dvc/
+-rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-06-09 07:30:48.000000 gaohn-common-utils-0.0.33/common_utils/versioning/dvc/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:31:06.148463 gaohn-common-utils-0.0.33/gaohn_common_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-09 07:31:06.000000 gaohn-common-utils-0.0.33/gaohn_common_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-09 07:31:06.000000 gaohn-common-utils-0.0.33/gaohn_common_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 07:31:06.000000 gaohn-common-utils-0.0.33/gaohn_common_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-09 07:31:06.000000 gaohn-common-utils-0.0.33/gaohn_common_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-09 07:31:06.000000 gaohn-common-utils-0.0.33/gaohn_common_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-06-09 07:30:48.000000 gaohn-common-utils-0.0.33/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 07:31:06.152463 gaohn-common-utils-0.0.33/setup.cfg
```

### Comparing `gaohn-common-utils-0.0.32/LICENSE` & `gaohn-common-utils-0.0.33/LICENSE`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.32/PKG-INFO` & `gaohn-common-utils-0.0.33/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaohn-common-utils
-Version: 0.0.32
+Version: 0.0.33
 Summary: A small utility package
 Author-email: Gao Hongnan <hongnangao@gmail.com>
 Project-URL: Homepage, https://github.com/gao-hongnan/common-utils
 Project-URL: Bug Tracker, https://github.com/gao-hongnan/common-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gaohn-common-utils-0.0.32/common_utils/cloud/base.py` & `gaohn-common-utils-0.0.33/common_utils/cloud/base.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.32/common_utils/cloud/gcp/storage/bigquery.py` & `gaohn-common-utils-0.0.33/common_utils/cloud/gcp/storage/bigquery.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,32 +20,31 @@
 logger = logging.getLogger("rich")
 
 
 @dataclass
 class BigQuery(GCPConnector):
     # usually you call project_id.dataset_id.table_name
     dataset: str  # The ID of the dataset to use.
-    table_name: str  # The name of the table to use.
     _dataset_id: str = field(init=False)  # The ID of the dataset to use.
     _table_id: str = field(init=False)  # The full ID of the table to use.
     bigquery_client: bigquery.Client = field(init=False)
 
     def __post_init__(self) -> None:
         """
         Initialize the BigQuery client for the GCP services.
         """
         super().__post_init__()
         self.bigquery_client = bigquery.Client(
             credentials=self.credentials, project=self.project_id
         )
 
     @property
-    def table_id(self) -> str:
+    def table_id(self, table_name: str) -> str:
         """Return the full ID of the table to use."""
-        return f"{self.project_id}.{self.dataset}.{self.table_name}"
+        return f"{self.project_id}.{self.dataset}.{table_name}"
 
     @property
     def dataset_id(self) -> str:
         """Return the ID of the dataset to use."""
         return f"{self.project_id}.{self.dataset}"
 
     def check_if_dataset_exists(self) -> Literal[True, False]:
@@ -63,33 +62,32 @@
 
     def create_dataset(self) -> None:
         """Creates a new BigQuery dataset if it doesn't exist."""
         dataset = bigquery.Dataset(self.dataset_id)
         self.bigquery_client.create_dataset(dataset)
         logger.info(f"Created dataset {self.dataset_id}")
 
-    def check_if_table_exists(self) -> Literal[True, False]:
+    def check_if_table_exists(self, table_name: str) -> Literal[True, False]:
         """Check if a table exists."""
         try:
-            print(self.table_id)
-            self.bigquery_client.get_table(self.table_id)
-            logger.info(f"Table {self.table_id} already exists")
+            self.bigquery_client.get_table(self.table_id(table_name))
+            logger.info(f"Table {self.table_id(table_name)} already exists")
             return True
         except NotFound:
             logger.warning(
-                f"""Table {self.table_id} does not exist.
+                f"""Table {self.table_id(table_name)} does not exist.
                 Please create it using `create_table`."""
             )
             return False
 
-    def create_table(self, schema: List[bigquery.SchemaField]) -> None:
+    def create_table(self, table_name: str, schema: List[bigquery.SchemaField]) -> None:
         """Creates a new BigQuery table if it doesn't exist."""
-        table = bigquery.Table(self.table_id, schema=schema)
+        table = bigquery.Table(self.table_id(table_name), schema=schema)
         self.bigquery_client.create_table(table)
-        logger.info(f"Created table {self.table_id}")
+        logger.info(f"Created table {self.table_id(table_name)}")
 
     def query(
         self, query: str, as_dataframe: bool = True
     ) -> Union[List[Tuple[Any]], pd.DataFrame]:
         """
         Execute a query in BigQuery and return the result as a DataFrame.
```

### Comparing `gaohn-common-utils-0.0.32/common_utils/cloud/gcp/storage/gcs.py` & `gaohn-common-utils-0.0.33/common_utils/cloud/gcp/storage/gcs.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.32/common_utils/core/artifacts.py` & `gaohn-common-utils-0.0.33/common_utils/core/artifacts.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.32/common_utils/core/common.py` & `gaohn-common-utils-0.0.33/common_utils/core/common.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.32/common_utils/core/decorators.py` & `gaohn-common-utils-0.0.33/common_utils/core/decorators.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.32/common_utils/core/file_system_utils.py` & `gaohn-common-utils-0.0.33/common_utils/core/file_system_utils.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.32/common_utils/core/logger.py` & `gaohn-common-utils-0.0.33/common_utils/core/logger.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.32/common_utils/versioning/dvc/base.py` & `gaohn-common-utils-0.0.33/common_utils/versioning/dvc/base.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.32/gaohn_common_utils.egg-info/PKG-INFO` & `gaohn-common-utils-0.0.33/gaohn_common_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaohn-common-utils
-Version: 0.0.32
+Version: 0.0.33
 Summary: A small utility package
 Author-email: Gao Hongnan <hongnangao@gmail.com>
 Project-URL: Homepage, https://github.com/gao-hongnan/common-utils
 Project-URL: Bug Tracker, https://github.com/gao-hongnan/common-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gaohn-common-utils-0.0.32/gaohn_common_utils.egg-info/SOURCES.txt` & `gaohn-common-utils-0.0.33/gaohn_common_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.32/pyproject.toml` & `gaohn-common-utils-0.0.33/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gaohn-common-utils"
-version = "0.0.32"
+version = "0.0.33"
 authors = [
   { name="Gao Hongnan", email="hongnangao@gmail.com" },
 ]
 description = "A small utility package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

