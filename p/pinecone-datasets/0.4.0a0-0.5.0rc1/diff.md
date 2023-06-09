# Comparing `tmp/pinecone_datasets-0.4.0a0.tar.gz` & `tmp/pinecone_datasets-0.5.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pinecone_datasets-0.4.0a0.tar", max compression
+gzip compressed data, was "pinecone_datasets-0.5.0rc1.tar", max compression
```

## Comparing `pinecone_datasets-0.4.0a0.tar` & `pinecone_datasets-0.5.0rc1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     6367 2023-06-06 17:49:00.712952 pinecone_datasets-0.4.0a0/README.md
--rw-r--r--   0        0        0      142 2023-06-06 17:49:28.255111 pinecone_datasets-0.4.0a0/pinecone_datasets/__init__.py
--rw-r--r--   0        0        0     3088 2023-06-01 03:29:23.061670 pinecone_datasets-0.4.0a0/pinecone_datasets/catalog.py
--rw-r--r--   0        0        0      706 2023-06-06 17:49:00.715570 pinecone_datasets-0.4.0a0/pinecone_datasets/cfg.py
--rw-r--r--   0        0        0     8800 2023-06-06 17:49:00.716674 pinecone_datasets-0.4.0a0/pinecone_datasets/dataset.py
--rw-r--r--   0        0        0      946 2023-05-31 10:57:13.712902 pinecone_datasets-0.4.0a0/pinecone_datasets/fs.py
--rw-r--r--   0        0        0     1657 2023-05-31 11:31:31.876795 pinecone_datasets-0.4.0a0/pinecone_datasets/public.py
--rw-r--r--   0        0        0      822 2023-06-06 17:51:58.311038 pinecone_datasets-0.4.0a0/pyproject.toml
--rw-r--r--   0        0        0     7445 1970-01-01 00:00:00.000000 pinecone_datasets-0.4.0a0/setup.py
--rw-r--r--   0        0        0     7248 1970-01-01 00:00:00.000000 pinecone_datasets-0.4.0a0/PKG-INFO
+-rw-r--r--   0        0        0     8143 2023-06-06 18:16:41.495378 pinecone_datasets-0.5.0rc1/README.md
+-rw-r--r--   0        0        0      197 2023-06-09 16:30:31.996421 pinecone_datasets-0.5.0rc1/pinecone_datasets/__init__.py
+-rw-r--r--   0        0        0     3088 2023-06-01 03:29:23.061670 pinecone_datasets-0.5.0rc1/pinecone_datasets/catalog.py
+-rw-r--r--   0        0        0     1128 2023-06-06 18:16:41.496757 pinecone_datasets-0.5.0rc1/pinecone_datasets/cfg.py
+-rw-r--r--   0        0        0    12769 2023-06-09 18:04:59.847618 pinecone_datasets-0.5.0rc1/pinecone_datasets/dataset.py
+-rw-r--r--   0        0        0      969 2023-06-09 17:14:09.503269 pinecone_datasets-0.5.0rc1/pinecone_datasets/fs.py
+-rw-r--r--   0        0        0     1657 2023-05-31 11:31:31.876795 pinecone_datasets-0.5.0rc1/pinecone_datasets/public.py
+-rw-r--r--   0        0        0      868 2023-06-09 17:35:56.977946 pinecone_datasets-0.5.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     9225 1970-01-01 00:00:00.000000 pinecone_datasets-0.5.0rc1/setup.py
+-rw-r--r--   0        0        0     9025 1970-01-01 00:00:00.000000 pinecone_datasets-0.5.0rc1/PKG-INFO
```

### Comparing `pinecone_datasets-0.4.0a0/README.md` & `pinecone_datasets-0.5.0rc1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -2,19 +2,21 @@
 
 ## install
 
 ```bash
 pip install pinecone-datasets
 ```
 
-## Usage
+##  Usage - Loading
 
-You can use Pinecone Datasets to load our public datasets or with your own dataset.
+You can use Pinecone Datasets to load our public datasets or with your own datasets. Datasets library can be used in 2 main ways: ad-hoc loading of datasets from a path or as a catalog loader for datasets. 
 
-### Loading Pinecone Public Datasets
+### Loading Pinecone Public Datasets (catalog)
+
+Pinecone hosts a public datasets catalog, you can load a dataset by name using `list_datasets` and `load_dataset` functions. This will use the default catalog endpoint (currently GCS) to list and load datasets.
 
 ```python
 from pinecone_datasets import list_datasets, load_dataset
 
 list_datasets()
 # ["quora_all-MiniLM-L6-bm25", ... ]
 
@@ -29,163 +31,165 @@
 # │ str ┆ list[f32]                 ┆ struct[2]                           ┆ struct[3]         ┆      │
 # ╞═════╪═══════════════════════════╪═════════════════════════════════════╪═══════════════════╪══════╡
 # │ 0   ┆ [0.118014, -0.069717, ... ┆ {[470065541, 52922727, ... 22364... ┆ {2017,12,"other"} ┆ .... │
 # │     ┆ 0.0060...                 ┆                                     ┆                   ┆      │
 # └─────┴───────────────────────────┴─────────────────────────────────────┴───────────────────┴──────┘
 ```
 
+### Expected dataset structure
 
-### Iterating over a Dataset documents and queries
+pinecone datasets can load dataset from every storage where it has access (using the default access: s3, gcs or local permissions)
 
-Iterating over documents is useful for upserting but also for different updating. Iterating over queries is helpful in benchmarking
+ we expect data to be uploaded to the following directory structure:
 
-```python
+    ├── my-subdir                     # path to where all datasets
+    │   ├── my-dataset                # name of dataset
+    │   │   ├── metadata.json         # dataset metadata (optional, only for listed)
+    │   │   ├── documents             # datasets documents
+    │   │   │   ├── file1.parquet      
+    │   │   │   └── file2.parquet      
+    │   │   ├── queries               # dataset queries
+    │   │   │   ├── file1.parquet  
+    │   │   │   └── file2.parquet   
+    └── ...
 
-# List Iterator, where every list of size N Dicts with ("id", "metadata", "values", "sparse_values")
-dataset.iter_documents(batch_size=n) 
+The data schema is expected to be as follows:
 
-dataset.iter_queries()
+- `documents` directory contains parquet files with the following schema:
+    - Mandatory: `id: str, values: list[float]`
+    - Optional: `sparse_values: Dict: indices: List[int], values: List[float]`, `metadata: Dict`, `blob: dict`
+        - note: blob is a dict that can contain any data, it is not returned when iterating over the dataset and is inteded to be used for storing additional data that is not part of the dataset schema. however, it is sometime useful to store additional data in the dataset, for example, a document text. In future version this may become a first class citizen in the dataset schema.
+- `queries` directory contains parquet files with the following schema:
+    - Mandatory: `vector: list[float], top_k: int`
+    - Optional: `sparse_vector: Dict: indices: List[int], values: List[float]`, `filter: Dict`
+        - note: filter is a dict that contain pinecone filters, for more information see [here](https://docs.pinecone.io/docs/metadata-filtering)
+
+in addition, a metadata file is expected to be in the dataset directory, for example: `s3://my-bucket/my-dataset/metadata.json`
 
+```python
+from pinecone_datasets.catalog import DatasetMetadata
+
+meta = DatasetMetadata(
+    name="test_dataset",
+    created_at="2023-02-17 14:17:01.481785",
+    documents=2,
+    queries=2,
+    source="manual",
+    bucket="LOCAL",
+    task="unittests",
+    dense_model={"name": "bert", "dimension": 3},
+    sparse_model={"name": "bm25"},
+)
 ```
 
-### upserting to Index
+full metadata schema can be found in `pinecone_datasets.catalog.DatasetMetadata.schema`
+
+### Loading your own dataset from catalog
+
+To set you own catalog endpoint, set the environment variable `DATASETS_CATALOG_BASEPATH` to your bucket. Note that pinecone uses the default authentication method for the storage type (gcsfs for GCS and s3fs for S3).
 
 ```bash
-pip install pinecone-client
+export DATASETS_CATALOG_BASEPATH="s3://my-bucket/my-subdir"
 ```
 
 ```python
-import pinecone
-pinecone.init(api_key="API_KEY", environment="us-west1-gcp")
-
-pinecone.create_index(name="my-index", dimension=384, pod_type='s1')
+from pinecone_datasets import list_datasets, load_dataset
 
-index = pinecone.Index("my-index")
+list_datasets()
 
-# you can iterate over documents in batches
-for batch in dataset.iter_documents(batch_size=100):
-    index.upsert(vectors=batch)
+# ["my-dataset", ... ]
 
-# or upsert the dataset as dataframe
-index.upsert_from_dataframe(dataset.drop(columns=["blob"]))
-
-# using gRPC
-index = pinecone.GRPCIndex("my-index")
+dataset = load_dataset("my-dataset")
 ```
 
-## Advanced Usage
+### Loading your own dataset from path
 
-### Working with your own dataset storage
+You can load your own dataset from a local path or a remote path (GCS or S3). Note that pinecone uses the default authentication method for the storage type (gcsfs for GCS and s3fs for S3).
 
-Datasets is using Pinecone's public datasets bucket on GCS, you can use your own bucket by setting the `DATASETS_CATALOG_BASEPATH` environment variable.
+```python
+from pinecone_datasets import Dataset
 
-```bash
-export PINECONE_DATASETS_ENDPOINT="gs://my-bucket"
+dataset = Dataset("s3://my-bucket/my-subdir/my-dataset")
 ```
 
-this will change the default endpoint to your bucket, and upon calling `list_datasets` or `load_dataset` it will scan your bucket and list all datasets.
+### Loading from a pandas dataframe
 
-Note that you can also use `s3://` as a prefix to your bucket.
+Pinecone Datasets enables you to load a dataset from a pandas dataframe. This is useful for loading a dataset from a local file and saving it to a remote storage.
+The minimal required data is a documents dataset, and the minimal required columns are `id` and `values`. The `id` column is a unique identifier for the document, and the `values` column is a list of floats representing the document vector.
 
-### Authenication to your own bucket
+```python
+import pandas as pd
 
-For now, Pinecone Datastes supports only GCS and S3 buckets, and with default authentication as provided by the fsspec implementation, respectively: `gcsfs` and `s3fs`.
+df = pd.read_parquet("my-dataset.parquet")
 
-### Using aws key/secret authentication methods
+dataset = Dataset.from_pandas(df)
+```
 
-first, to set a new endpoint, set the environment variable `PINECONE_DATASETS_ENDPOINT` to your bucket.
+Please check the documentation for more information on the expected dataframe schema. There's also a column mapping variable that can be used to map the dataframe columns to the expected schema.
 
-```bash
-export PINECONE_DATASETS_ENDPOINT="s3://my-bucket"
-```
 
-then, you can use the `key` and `secret` parameters to pass your credentials to the `list_datasets` and `load_dataset` functions.
+## Usage - Accessing data
 
-```python
-st = list_datasets(
-        key=os.environ.get("S3_ACCESS_KEY"),
-        secret=os.environ.get("S3_SECRET"),
-    )
+Pinecone Datasets is build on top of pandas. This means that you can use all the pandas API to access the data. In addition, we provide some helper functions to access the data in a more convenient way. 
 
-ds = load_dataset(
-        "test_dataset",
-        key=os.environ.get("S3_ACCESS_KEY"),
-        secret=os.environ.get("S3_SECRET"),
-)
-```
+### Accessing documents and queries dataframes
 
-## For developers
+accessing the documents and queries dataframes is done using the `documents` and `queries` properties. These properties are lazy and will only load the data when accessed. 
 
-This project is using poetry for dependency managemet. supported python version are 3.8+. To start developing, on project root directory run:
+```python
+document_df: pd.DataFrame = dataset.documents
 
-```bash
-poetry install --with dev
+query_df: pd.DataFrame = dataset.queries
 ```
 
-To run test locally run 
 
-```bash
-poetry run pytest --cov pinecone_datasets
-```
+## Usage - Iterating
+
+One of the main use cases for Pinecone Datasets is iterating over a dataset. This is useful for upserting a dataset to an index, or for benchmarking. It is also useful for iterating over large datasets - as of today, datasets are not yet lazy, however we are working on it.
 
-To create a pinecone-public dataset you may need to generate a dataset metadata. For example:
 
 ```python
-from pinecone_datasets.catalog import DatasetMetadata
 
-meta = DatasetMetadata(
-    name="test_dataset",
-    created_at="2023-02-17 14:17:01.481785",
-    documents=2,
-    queries=2,
-    source="manual",
-    bucket="LOCAL",
-    task="unittests",
-    dense_model={"name": "bert", "dimension": 3},
-    sparse_model={"name": "bm25"},
-)
-```
+# List Iterator, where every list of size N Dicts with ("id", "values", "sparse_values", "metadata")
+dataset.iter_documents(batch_size=n) 
 
-to see the complete schema you can run:
+# Dict Iterator, where every dict has ("vector", "sparse_vector", "filter", "top_k")
+dataset.iter_queries()
 
-```python
-meta.schema()
 ```
 
-in order to list a dataset you can save dataset metadata (NOTE: write permission to loacaion is needed)
+### upserting to Index
 
-```python
-dataset = Dataset("non-listed-dataset")
-dataset._save_metadata(meta)
+```bash
+pip install pinecone-client
 ```
 
-### Uploading and listing a dataset. 
+```python
+import pinecone
+pinecone.init(api_key="API_KEY", environment="us-west1-gcp")
 
-pinecone datasets can load dataset from every storage where it has access (using the default access: s3, gcs or local permissions)
+pinecone.create_index(name="my-index", dimension=384, pod_type='s1')
 
- we expect data to be uploaded to the following directory structure:
+index = pinecone.Index("my-index")
 
-    ├── base_path                     # path to where all datasets
-    │   ├── dataset_id                # name of dataset
-    │   │   ├── metadata.json         # dataset metadata (optional, only for listed)
-    │   │   ├── documents             # datasets documents
-    │   │   │   ├── file1.parquet      
-    │   │   │   └── file2.parquet      
-    │   │   ├── queries               # dataset queries
-    │   │   │   ├── file1.parquet  
-    │   │   │   └── file2.parquet   
-    └── ...
+# you can iterate over documents in batches
+for batch in dataset.iter_documents(batch_size=100):
+    index.upsert(vectors=batch)
 
-a listed dataset is a dataset that is loaded and listed using `load_dataset` and `list_dataset`
-pinecone datasets will scan storage and will list every dataset with metadata file, for example: `s3://my-bucket/my-dataset/metadata.json`
+# or upsert the dataset as dataframe
+index.upsert_from_dataframe(dataset.drop(columns=["blob"]))
+```
 
-### Accessing a non-listed dataset
 
-to access a non listed dataset you can directly load it via:
+## For developers
 
-```python
-from pinecone_datasets import Dataset
+This project is using poetry for dependency managemet. supported python version are 3.8+. To start developing, on project root directory run:
 
-dataset = Dataset("non-listed-dataset")
+```bash
+poetry install --with dev
 ```
 
+To run test locally run 
 
+```bash
+poetry run pytest --cov pinecone_datasets
+```
```

### Comparing `pinecone_datasets-0.4.0a0/pinecone_datasets/catalog.py` & `pinecone_datasets-0.5.0rc1/pinecone_datasets/catalog.py`

 * *Files identical despite different names*

### Comparing `pinecone_datasets-0.4.0a0/pinecone_datasets/dataset.py` & `pinecone_datasets-0.5.0rc1/pinecone_datasets/dataset.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 import sys
 import glob
 import os
 import json
 from functools import cached_property
-from typing import Any, Generator, Iterator, List, Union, Dict
+from typing import Any, Generator, Iterator, List, Union, Dict, Optional, Tuple
 import warnings
 from urllib.parse import urlparse
 
 import gcsfs
 from pydantic import ValidationError
 import s3fs
-import polars as pl
+
+# import polars as pl
 import pandas as pd
 import pyarrow.parquet as pq
 
 from pinecone_datasets import cfg
 from pinecone_datasets.catalog import DatasetMetadata
-from pinecone_datasets.fs import get_cloud_fs
+from pinecone_datasets.fs import get_cloud_fs, LocalFileSystem
 
 
 def iter_pandas_dataframe_slices(
     df: pd.DataFrame, batch_size=1
 ) -> Generator[List[Dict[str, Any]], None, None]:
     for i in range(0, len(df), batch_size):
         yield df.iloc[i : i + batch_size].to_dict(orient="records")
@@ -55,32 +56,92 @@
         Load a dataset from Pinecone's Datasets catalog, or from your own endpoint.
 
         Args:
             dataset_id (str): the id of the dataset to load within a catalog
             catalog_base_path (str): the catalog's base path. Defaults to DATASETS_CATALOG_BASEPATH environment variable.
                                      If neither are set, will use Pinecone's public catalog.
 
-        Keyword Args:
-            engine (str): the engine to use for loading the dataset. Options are ['polars', 'pandas']. Defaults to 'pandas'.
-
         Returns:
             Dataset: a Dataset object
         """
         catalog_base_path = (
             catalog_base_path
             if catalog_base_path
             else os.environ.get("DATASETS_CATALOG_BASEPATH", cfg.Storage.endpoint)
         )
         dataset_path = os.path.join(catalog_base_path, f"{dataset_id}")
         return cls(dataset_path=dataset_path, **kwargs)
 
+    @classmethod
+    def from_pandas(
+        cls,
+        documents: pd.DataFrame,
+        metadata: DatasetMetadata,
+        documents_column_mapping: Optional[Dict] = None,
+        queries: Optional[pd.DataFrame] = None,
+        queries_column_mapping: Optional[Dict] = None,
+        **kwargs,
+    ) -> "Dataset":
+        """
+        Create a Dataset object from a pandas DataFrame
+
+        Args:
+            documents (pd.DataFrame): a pandas DataFrame containing the documents
+            documents_column_mapping (Dict): a dictionary mapping the columns of the documents DataFrame to the Pinecone Datasets Schema
+            queries (pd.DataFrame): a pandas DataFrame containing the queries
+            queries_column_mapping (Dict): a dictionary mapping the columns of the queries DataFrame to the Pinecone Datasets Schema
+
+        Keyword Args:
+            kwargs (Dict): additional arguments to pass to the fsspec constructor
+
+        Returns:
+            Dataset: a Dataset object
+        """
+        clazz = Dataset(dataset_path=os.getcwd(), **kwargs)
+        clazz.documents = cls._read_pandas_dataframe(
+            documents, documents_column_mapping, cfg.Schema.Names.documents
+        )
+        clazz.queries = cls._read_pandas_dataframe(
+            queries, queries_column_mapping, cfg.Schema.Names.queries
+        )
+        clazz.metadata = metadata
+        return clazz
+
+    @staticmethod
+    def _read_pandas_dataframe(
+        df: pd.DataFrame, column_mapping: Dict[str, str], schema: List[Tuple[str, bool]]
+    ) -> pd.DataFrame:
+        """
+        Reads a pandas DataFrame and validates it against a schema.
+
+        Args:
+            df (pd.DataFrame): the pandas DataFrame to read
+            column_mapping (Dict[str, str]): a dictionary mapping the columns of the DataFrame to the Pinecone Datasets Schema (col_name, pinecone_name)
+            schema (List[Tuple[str, bool]]): the schema to validate against (column_name, is_nullable)
+
+        Returns:
+            pd.DataFrame: the validated, renamed DataFrame
+        """
+        if df is None or df.empty:
+            return pd.DataFrame(columns=[column_name for column_name, _ in schema])
+        else:
+            if column_mapping is not None:
+                df.rename(columns=column_mapping, inplace=True)
+            for column_name, is_nullable in schema:
+                if column_name not in df.columns and not is_nullable:
+                    raise ValueError(
+                        f"error, file is not matching Pinecone Datasets Schmea: {column_name} not found"
+                    )
+                elif column_name not in df.columns and is_nullable:
+                    df[column_name] = None
+            return df[[column_name for column_name, _ in schema]]
+
     def __init__(
         self,
         dataset_path: str,
-        engine: str = "pandas",
         **kwargs,
     ) -> None:
         """
         Dataset class to load and query datasets from the Pinecone Datasets catalog.
         See `from_path` and `from_dataset_id` for examples on how to load a dataset.
 
         Examples:
@@ -98,90 +159,93 @@
             # or
             dataset.documents # returns a pandas/polars DataFrame
             dataset.queries # returns a pandas/polars DataFrame
             ```
 
         """
         self._config = cfg
-        self._engine = engine
         endpoint = urlparse(dataset_path)._replace(path="").geturl()
         self._fs = get_cloud_fs(endpoint, **kwargs)
         self._dataset_path = dataset_path
 
         if not self._fs.exists(self._dataset_path):
             raise FileNotFoundError(
                 "Dataset does not exist. Please check the path or dataset_id"
             )
 
     def _is_datatype_exists(self, data_type: str) -> bool:
         return self._fs.exists(os.path.join(self._dataset_path, data_type))
 
-    def _safe_read_from_path(
-        self, data_type: str, enforced_schema: Dict[str, Any]
-    ) -> Union[pl.DataFrame, pd.DataFrame]:
+    def _safe_read_from_path(self, data_type: str) -> pd.DataFrame:
         read_path_str = os.path.join(self._dataset_path, data_type, "*.parquet")
         read_path = self._fs.glob(read_path_str)
         if self._is_datatype_exists(data_type):
             dataset = pq.ParquetDataset(read_path, filesystem=self._fs)
-            try:
-                if self._engine == "pandas":
-                    df = dataset.read_pandas().to_pandas()
-                elif self._engine == "polars":
-                    df = pl.from_arrow(dataset.read(), schema_overrides=enforced_schema)
+            dataset_schema_names = dataset.schema.names
+            columns_to_null = []
+            columns_not_null = []
+            for column_name, is_nullable in getattr(
+                self._config.Schema.Names, data_type
+            ):
+                if column_name not in dataset_schema_names and not is_nullable:
+                    raise ValueError(
+                        f"error, file is not matching Pinecone Datasets Schmea: {column_name} not found"
+                    )
+                elif column_name not in dataset_schema_names and is_nullable:
+                    columns_to_null.append(column_name)
                 else:
-                    raise ValueError("engine must be one of ['pandas', 'polars']")
+                    columns_not_null.append(column_name)
+            try:
+                # TODO: use of the columns_not_null and columns_to_null is only a workaround for proper schema validation and versioning
+                df = dataset.read_pandas(columns=columns_not_null).to_pandas()
+                for column_name in columns_to_null:
+                    df[column_name] = None
                 return df
-            except pl.PanicException as pe:
-                msg = f"error, file is not matching Pinecone Datasets Schmea: {pe}"
-                raise RuntimeError(msg)
+            # TODO: add more specific error handling, explain what is wrong
             except Exception as e:
                 print("error, no exception: {}".format(e), file=sys.stderr)
                 raise (e)
         else:
             warnings.warn(
                 "WARNING: No data found at: {}. Returning empty DF".format(
                     read_path_str
                 ),
                 UserWarning,
                 stacklevel=0,
             )
-            if self._engine == "pandas":
-                return pd.DataFrame()
-            elif self._engine == "polars":
-                return pl.DataFrame()
-            else:
-                raise ValueError("engine must be one of ['pandas', 'polars']")
+            return pd.DataFrame(columns=getattr(self._config.Schema.Names, data_type))
 
     def _load_metadata(self) -> DatasetMetadata:
         with self._fs.open(
             os.path.join(self._dataset_path, "metadata.json"), "rb"
         ) as f:
             metadata = json.load(f)
         try:
             out = DatasetMetadata(**metadata)
             return out
+        # TODO: add more specific error handling, explain what is wrong
         except ValidationError as e:
             raise e
 
     def _save_metadata(self, metadata: DatasetMetadata) -> None:  # pragma: no cover
         with self._fs.open(os.path.join(self._dataset_path, "metadata.json"), "w") as f:
             json.dump(metadata.dict(), f)
 
-    def __getitem__(self, key: str) -> pl.DataFrame:
+    def __getitem__(self, key: str):
         if key in ["documents", "queries"]:
             return getattr(self, key)
         else:
             raise KeyError("Dataset does not have key: {}".format(key))
 
     def __len__(self) -> int:
         return self.documents.shape[0]
 
     @cached_property
-    def documents(self) -> Union[pl.DataFrame, pd.DataFrame]:
-        return self._safe_read_from_path("documents", self._config.Schema.documents)
+    def documents(self) -> pd.DataFrame:
+        return self._safe_read_from_path("documents")
 
     def iter_documents(self, batch_size: int = 1) -> Iterator[List[Dict[str, Any]]]:
         """
         Iterates over the documents in the dataset.
 
         Args:
             batch_size (int, optional): The batch size to use for the iterator. Defaults to 1.
@@ -190,52 +254,87 @@
             Iterator[List[Dict[str, Any]]]: An iterator over the documents in the dataset.
 
         Examples:
             for batch in dataset.iter_documents(batch_size=100):
                 index.upsert(batch)
         """
         if isinstance(batch_size, int) and batch_size > 0:
-            if self._engine == "pandas":
-                return iter_pandas_dataframe_slices(
-                    self.documents[self._config.Schema.documents_select_columns],
-                    batch_size,
-                )
-            return map(
-                lambda x: x.to_dicts(),
-                self.documents.select(
-                    self._config.Schema.documents_select_columns
-                ).iter_slices(n_rows=batch_size),
+            return iter_pandas_dataframe_slices(
+                self.documents[self._config.Schema.documents_select_columns],
+                batch_size,
             )
         else:
             raise ValueError("batch_size must be greater than 0")
 
     @cached_property
-    def queries(self) -> Union[pl.DataFrame, pd.DataFrame]:
-        return self._safe_read_from_path("queries", self._config.Schema.documents)
+    def queries(self) -> pd.DataFrame:
+        return self._safe_read_from_path("queries")
 
     def iter_queries(self) -> Iterator[Dict[str, Any]]:
         """
         Iterates over the queries in the dataset.
 
         Returns:
             Iterator[Dict[str, Any]]: An iterator over the queries in the dataset.
 
         Examples:
             for query in dataset.iter_queries():
                 results = index.query(**query)
                 # do something with the results
         """
-        if self._engine == "pandas":
-            return iter_pandas_dataframe_single(
-                self.queries[self._config.Schema.queries_select_columns]
-            )
-        else:
-            return self.queries.select(
-                self.queries[self._config.Schema.queries_select_columns]
-            ).iter_rows(named=True)
+        return iter_pandas_dataframe_single(
+            self.queries[self._config.Schema.queries_select_columns]
+        )
 
     @cached_property
-    def metadata(self) -> Union[pl.DataFrame, pd.DataFrame]:
+    def metadata(self) -> pd.DataFrame:
         return self._load_metadata()
 
-    def head(self, n: int = 5) -> Union[pl.DataFrame, pd.DataFrame]:
+    def head(self, n: int = 5) -> pd.DataFrame:
         return self.documents.head(n)
+
+    def save_to_path(self, dataset_path: str, **kwargs):
+        """
+        Saves the dataset to a local or cloud storage path.
+        """
+        fs = get_cloud_fs(dataset_path, **kwargs)
+
+        # save documents
+        documents_path = os.path.join(dataset_path, "documents")
+        fs.makedirs(documents_path, exist_ok=True)
+        self.documents.to_parquet(
+            os.path.join(documents_path, "part-0.parquet"),
+            engine="pyarrow",
+            index=False,
+            filesystem=fs,
+        )
+        # save queries
+        if not self.queries.empty:
+            queries_path = os.path.join(dataset_path, "queries")
+            fs.makedirs(queries_path, exist_ok=True)
+            self.queries.to_parquet(
+                os.path.join(queries_path, "part-0.parquet"),
+                engine="pyarrow",
+                index=False,
+                filesystem=fs,
+            )
+        else:
+            warnings.warn("Queries are empty, not saving queries")
+
+        # save metadata
+        with fs.open(os.path.join(dataset_path, "metadata.json"), "w") as f:
+            json.dump(self.metadata.dict(), f)
+
+    def save_to_catalog(self, dataset_id: str, catalog_base_path: str = "", **kwargs):
+        """
+        Saves the dataset to the public catalog.
+        """
+
+        # TODO: duplicated code
+
+        catalog_base_path = (
+            catalog_base_path
+            if catalog_base_path
+            else os.environ.get("DATASETS_CATALOG_BASEPATH", cfg.Storage.endpoint)
+        )
+        dataset_path = os.path.join(catalog_base_path, f"{dataset_id}")
+        self.save_to_path(dataset_path, **kwargs)
```

### Comparing `pinecone_datasets-0.4.0a0/pinecone_datasets/fs.py` & `pinecone_datasets-0.5.0rc1/pinecone_datasets/fs.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 import gcsfs
 import s3fs
 from fsspec.implementations.local import LocalFileSystem
 
 from pinecone_datasets import cfg
 
 
-def get_cloud_fs(path, **kwargs) -> Union[gcsfs.GCSFileSystem, s3fs.S3FileSystem]:
+def get_cloud_fs(
+    path, **kwargs
+) -> Union[gcsfs.GCSFileSystem, s3fs.S3FileSystem, LocalFileSystem]:
     """
     returns a filesystem object for the given path, if it is a cloud storage path (gs:// or s3://)
 
     Args:
         path (str): the path to the file or directory
         **kwargs: additional arguments to pass to the filesystem constructor
```

### Comparing `pinecone_datasets-0.4.0a0/pinecone_datasets/public.py` & `pinecone_datasets-0.5.0rc1/pinecone_datasets/public.py`

 * *Files identical despite different names*

### Comparing `pinecone_datasets-0.4.0a0/pyproject.toml` & `pinecone_datasets-0.5.0rc1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pinecone-datasets"
-version = "0.4.0-alpha"
+version = "0.5.0-rc.1"
 description = "Pinecone Datasets lets you easily load datasets into your Pinecone index."
 authors = ["Pinecone"]
 maintainers = [
     "Roy Miara <miararoy@gmail.com>",
 ]
 readme = "README.md"
 
@@ -15,26 +15,28 @@
 pyarrow = "^12.0.0"
 fsspec = "^2023.1.0"
 gcsfs = "^2023.1.0"
 s3fs = "^2023.1.0"
 pydantic = "^1.10.5"
 protobuf = ">=3.19.3,<3.20.0"
 pandas = "^2.0.0"
+#pinecone-client = "3.0.0rc2"
 
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 ipykernel = "^6.21.1"
 pinecone-client = {version="^2.2", extras=["grpc"]}
 black = "^23.1.0"
 pytest-cov = "^4.0.0"
 mypy = "^1.0.1"
 pytest = "^7.2.2"
 pytest-html = "^3.2.0"
 pdoc = "^13.0.0"
+toml = "^0.10.2"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

