# Comparing `tmp/astro-sdk-python-1.7.0a2.tar.gz` & `tmp/astro_sdk_python-1.7.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astro-sdk-python-1.7.0a2.tar", last modified: Fri May  5 23:38:53 2023, max compression
+gzip compressed data, was "astro_sdk_python-1.7.0a3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `astro-sdk-python-1.7.0a2.tar` & `astro_sdk_python-1.7.0a3.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-lrwxr-xr-x   0        0        0        0 2023-05-05 23:38:37.411658 astro-sdk-python-1.7.0a2/LICENSE -> ../LICENSE
--rw-r--r--   0        0        0     8344 2023-05-05 23:38:37.411658 astro-sdk-python-1.7.0a2/README.md
--rw-r--r--   0        0        0     5401 2023-05-05 23:38:37.423658 astro-sdk-python-1.7.0a2/pyproject.toml
--rw-r--r--   0        0        0      687 2023-05-05 23:38:37.423658 astro-sdk-python-1.7.0a2/src/astro/__init__.py
--rw-r--r--   0        0        0        0 2023-05-05 23:38:37.423658 astro-sdk-python-1.7.0a2/src/astro/airflow/__init__.py
--rw-r--r--   0        0        0     1605 2023-05-05 23:38:37.423658 astro-sdk-python-1.7.0a2/src/astro/airflow/datasets.py
--rw-r--r--   0        0        0     2256 2023-05-05 23:38:37.423658 astro-sdk-python-1.7.0a2/src/astro/constants.py
--rw-r--r--   0        0        0        0 2023-05-05 23:38:37.423658 astro-sdk-python-1.7.0a2/src/astro/custom_backend/__init__.py
--rw-r--r--   0        0        0     2187 2023-05-05 23:38:37.423658 astro-sdk-python-1.7.0a2/src/astro/custom_backend/astro_custom_backend.py
--rw-r--r--   0        0        0     3915 2023-05-05 23:38:37.423658 astro-sdk-python-1.7.0a2/src/astro/custom_backend/serializer.py
--rw-r--r--   0        0        0     1876 2023-05-05 23:38:37.423658 astro-sdk-python-1.7.0a2/src/astro/databases/__init__.py
--rw-r--r--   0        0        0        0 2023-05-05 23:38:37.423658 astro-sdk-python-1.7.0a2/src/astro/databases/aws/__init__.py
--rw-r--r--   0        0        0    18189 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/databases/aws/redshift.py
--rw-r--r--   0        0        0    37548 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/databases/base.py
--rw-r--r--   0        0        0        0 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/databases/databricks/__init__.py
--rw-r--r--   0        0        0     7247 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/databases/databricks/api_utils.py
--rw-r--r--   0        0        0    18134 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/databases/databricks/delta.py
--rw-r--r--   0        0        0        0 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/databases/databricks/load_file/__init__.py
--rw-r--r--   0        0        0      720 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/databases/databricks/load_file/jinja_templates/autoloader.py.jinja2
--rw-r--r--   0        0        0      647 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/databases/databricks/load_file/jinja_templates/copy_into.py.jinja2
--rw-r--r--   0        0        0      913 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/databases/databricks/load_file/jinja_templates/load_file_to_delta.py.jinja2
--rw-r--r--   0        0        0      512 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/databases/databricks/load_file/jinja_templates/load_secrets.py.jinja2
--rw-r--r--   0        0        0     6368 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/databases/databricks/load_file/load_file_job.py
--rw-r--r--   0        0        0      880 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/databases/databricks/load_file/load_file_python_code_generator.py
--rw-r--r--   0        0        0     2687 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/databases/databricks/load_options.py
--rw-r--r--   0        0        0     6181 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/databases/duckdb.py
--rw-r--r--   0        0        0        0 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/databases/google/__init__.py
--rw-r--r--   0        0        0    26823 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/databases/google/bigquery.py
--rw-r--r--   0        0        0    17049 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/databases/mssql.py
--rw-r--r--   0        0        0     9267 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/databases/mysql.py
--rw-r--r--   0        0        0    10682 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/databases/postgres.py
--rw-r--r--   0        0        0    42201 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/databases/snowflake.py
--rw-r--r--   0        0        0     6508 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/databases/sqlite.py
--rw-r--r--   0        0        0        0 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/dataframes/__init__.py
--rw-r--r--   0        0        0     4116 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/dataframes/load_options.py
--rw-r--r--   0        0        0     2356 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/dataframes/pandas.py
--rw-r--r--   0        0        0     1267 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/exceptions.py
--rw-r--r--   0        0        0     1096 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/files/__init__.py
--rw-r--r--   0        0        0    10151 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/files/base.py
--rw-r--r--   0        0        0     1535 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/files/locations/__init__.py
--rw-r--r--   0        0        0        0 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/files/locations/amazon/__init__.py
--rw-r--r--   0        0        0     3605 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/files/locations/amazon/s3.py
--rw-r--r--   0        0        0        0 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/files/locations/azure/__init__.py
--rw-r--r--   0        0        0     5867 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/files/locations/azure/wasb.py
--rw-r--r--   0        0        0     6601 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/files/locations/base.py
--rw-r--r--   0        0        0     2374 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/files/locations/ftp.py
--rw-r--r--   0        0        0        0 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/files/locations/google/__init__.py
--rw-r--r--   0        0        0     4420 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/files/locations/google/gcs.py
--rw-r--r--   0        0        0     5006 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/files/locations/google/gdrive.py
--rw-r--r--   0        0        0     1303 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/files/locations/http.py
--rw-r--r--   0        0        0     1531 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/files/locations/local.py
--rw-r--r--   0        0        0     3267 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/files/locations/sftp.py
--rw-r--r--   0        0        0        0 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/files/operators/__init__.py
--rw-r--r--   0        0        0     1595 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/files/operators/files.py
--rw-r--r--   0        0        0     2576 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/files/types/__init__.py
--rw-r--r--   0        0        0     1504 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/files/types/base.py
--rw-r--r--   0        0        0     1900 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/files/types/csv.py
--rw-r--r--   0        0        0     2197 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/files/types/json.py
--rw-r--r--   0        0        0     3652 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/files/types/ndjson.py
--rw-r--r--   0        0        0     2848 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/files/types/parquet.py
--rw-r--r--   0        0        0      700 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/lineage/__init__.py
--rw-r--r--   0        0        0     4264 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/lineage/facets.py
--rw-r--r--   0        0        0     3910 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/options.py
--rw-r--r--   0        0        0     1117 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/query_modifier.py
--rw-r--r--   0        0        0     4152 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/settings.py
--rw-r--r--   0        0        0     3194 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/sql/__init__.py
--rw-r--r--   0        0        0        0 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/sql/operators/__init__.py
--rw-r--r--   0        0        0     7857 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/sql/operators/append.py
--rw-r--r--   0        0        0    18419 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/sql/operators/base_decorator.py
--rw-r--r--   0        0        0      334 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/sql/operators/base_operator.py
--rw-r--r--   0        0        0    12688 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/sql/operators/cleanup.py
--rw-r--r--   0        0        0     7870 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/sql/operators/data_validations/check_column.py
--rw-r--r--   0        0        0     3696 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/sql/operators/data_validations/check_table.py
--rw-r--r--   0        0        0    15362 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/sql/operators/dataframe.py
--rw-r--r--   0        0        0     1435 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/sql/operators/drop.py
--rw-r--r--   0        0        0     2693 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/sql/operators/export_file.py
--rw-r--r--   0        0        0     2715 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/sql/operators/export_table_to_file.py
--rw-r--r--   0        0        0     7035 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/sql/operators/export_to_file.py
--rw-r--r--   0        0        0    17526 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/sql/operators/load_file.py
--rw-r--r--   0        0        0     8824 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/sql/operators/merge.py
--rw-r--r--   0        0        0     9898 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/sql/operators/raw_sql.py
--rw-r--r--   0        0        0     8055 2023-05-05 23:38:37.431658 astro-sdk-python-1.7.0a2/src/astro/sql/operators/transform.py
--rw-r--r--   0        0        0      880 2023-05-05 23:38:37.431658 astro-sdk-python-1.7.0a2/src/astro/sql/operators/upstream_task_mixin.py
--rw-r--r--   0        0        0      160 2023-05-05 23:38:37.431658 astro-sdk-python-1.7.0a2/src/astro/sql/table.py
--rw-r--r--   0        0        0     8747 2023-05-05 23:38:37.431658 astro-sdk-python-1.7.0a2/src/astro/table.py
--rw-r--r--   0        0        0        0 2023-05-05 23:38:37.431658 astro-sdk-python-1.7.0a2/src/astro/utils/__init__.py
--rw-r--r--   0        0        0        0 2023-05-05 23:38:37.431658 astro-sdk-python-1.7.0a2/src/astro/utils/compat/__init__.py
--rw-r--r--   0        0        0      359 2023-05-05 23:38:37.431658 astro-sdk-python-1.7.0a2/src/astro/utils/compat/functools.py
--rw-r--r--   0        0        0      843 2023-05-05 23:38:37.431658 astro-sdk-python-1.7.0a2/src/astro/utils/compat/typing.py
--rw-r--r--   0        0        0     2022 2023-05-05 23:38:37.431658 astro-sdk-python-1.7.0a2/src/astro/utils/dataframe.py
--rw-r--r--   0        0        0     1581 2023-05-05 23:38:37.431658 astro-sdk-python-1.7.0a2/src/astro/utils/load.py
--rw-r--r--   0        0        0     2790 2023-05-05 23:38:37.431658 astro-sdk-python-1.7.0a2/src/astro/utils/path.py
--rw-r--r--   0        0        0     4025 2023-05-05 23:38:37.431658 astro-sdk-python-1.7.0a2/src/astro/utils/table.py
--rw-r--r--   0        0        0    13466 1970-01-01 00:00:00.000000 astro-sdk-python-1.7.0a2/PKG-INFO
+lrwxr-xr-x   0        0        0        0 2023-05-30 06:40:32.905520 astro_sdk_python-1.7.0a3/LICENSE -> ../LICENSE
+-rw-r--r--   0        0        0     8344 2023-05-30 06:40:32.906281 astro_sdk_python-1.7.0a3/README.md
+-rw-r--r--   0        0        0     5411 2023-05-30 06:40:32.931249 astro_sdk_python-1.7.0a3/pyproject.toml
+-rw-r--r--   0        0        0      687 2023-06-09 16:56:08.339879 astro_sdk_python-1.7.0a3/src/astro/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-30 06:40:32.931594 astro_sdk_python-1.7.0a3/src/astro/airflow/__init__.py
+-rw-r--r--   0        0        0     1605 2023-05-30 06:40:32.931688 astro_sdk_python-1.7.0a3/src/astro/airflow/datasets.py
+-rw-r--r--   0        0        0     2256 2023-05-30 06:40:32.932006 astro_sdk_python-1.7.0a3/src/astro/constants.py
+-rw-r--r--   0        0        0        0 2023-05-30 06:40:32.932047 astro_sdk_python-1.7.0a3/src/astro/custom_backend/__init__.py
+-rw-r--r--   0        0        0     2187 2023-05-30 06:40:32.932139 astro_sdk_python-1.7.0a3/src/astro/custom_backend/astro_custom_backend.py
+-rw-r--r--   0        0        0     4019 2023-05-30 06:40:32.932649 astro_sdk_python-1.7.0a3/src/astro/custom_backend/serializer.py
+-rw-r--r--   0        0        0     1876 2023-05-30 06:40:32.932746 astro_sdk_python-1.7.0a3/src/astro/databases/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-30 06:40:32.932786 astro_sdk_python-1.7.0a3/src/astro/databases/aws/__init__.py
+-rw-r--r--   0        0        0    18189 2023-05-30 06:40:32.933166 astro_sdk_python-1.7.0a3/src/astro/databases/aws/redshift.py
+-rw-r--r--   0        0        0    38326 2023-06-09 13:33:48.664375 astro_sdk_python-1.7.0a3/src/astro/databases/base.py
+-rw-r--r--   0        0        0        0 2023-05-30 06:40:32.934050 astro_sdk_python-1.7.0a3/src/astro/databases/databricks/__init__.py
+-rw-r--r--   0        0        0     7247 2023-05-30 06:40:32.934195 astro_sdk_python-1.7.0a3/src/astro/databases/databricks/api_utils.py
+-rw-r--r--   0        0        0    18134 2023-05-30 06:40:32.934860 astro_sdk_python-1.7.0a3/src/astro/databases/databricks/delta.py
+-rw-r--r--   0        0        0        0 2023-05-30 06:40:32.934934 astro_sdk_python-1.7.0a3/src/astro/databases/databricks/load_file/__init__.py
+-rw-r--r--   0        0        0      720 2023-05-30 06:40:32.935093 astro_sdk_python-1.7.0a3/src/astro/databases/databricks/load_file/jinja_templates/autoloader.py.jinja2
+-rw-r--r--   0        0        0      647 2023-05-30 06:40:32.935174 astro_sdk_python-1.7.0a3/src/astro/databases/databricks/load_file/jinja_templates/copy_into.py.jinja2
+-rw-r--r--   0        0        0      913 2023-05-30 06:40:32.935251 astro_sdk_python-1.7.0a3/src/astro/databases/databricks/load_file/jinja_templates/load_file_to_delta.py.jinja2
+-rw-r--r--   0        0        0      512 2023-05-30 06:40:32.935332 astro_sdk_python-1.7.0a3/src/astro/databases/databricks/load_file/jinja_templates/load_secrets.py.jinja2
+-rw-r--r--   0        0        0     6368 2023-05-30 06:40:32.935427 astro_sdk_python-1.7.0a3/src/astro/databases/databricks/load_file/load_file_job.py
+-rw-r--r--   0        0        0      880 2023-05-30 06:40:32.935497 astro_sdk_python-1.7.0a3/src/astro/databases/databricks/load_file/load_file_python_code_generator.py
+-rw-r--r--   0        0        0     2687 2023-05-30 06:40:32.935592 astro_sdk_python-1.7.0a3/src/astro/databases/databricks/load_options.py
+-rw-r--r--   0        0        0     6181 2023-05-30 06:40:32.935946 astro_sdk_python-1.7.0a3/src/astro/databases/duckdb.py
+-rw-r--r--   0        0        0        0 2023-05-30 06:40:32.936001 astro_sdk_python-1.7.0a3/src/astro/databases/google/__init__.py
+-rw-r--r--   0        0        0    26823 2023-05-30 06:40:32.936094 astro_sdk_python-1.7.0a3/src/astro/databases/google/bigquery.py
+-rw-r--r--   0        0        0    17049 2023-05-30 06:40:32.936343 astro_sdk_python-1.7.0a3/src/astro/databases/mssql.py
+-rw-r--r--   0        0        0     9267 2023-05-30 06:40:32.936596 astro_sdk_python-1.7.0a3/src/astro/databases/mysql.py
+-rw-r--r--   0        0        0    10682 2023-05-30 06:40:32.937481 astro_sdk_python-1.7.0a3/src/astro/databases/postgres.py
+-rw-r--r--   0        0        0    42201 2023-05-30 06:40:32.937595 astro_sdk_python-1.7.0a3/src/astro/databases/snowflake.py
+-rw-r--r--   0        0        0     6508 2023-05-30 06:40:32.937898 astro_sdk_python-1.7.0a3/src/astro/databases/sqlite.py
+-rw-r--r--   0        0        0        0 2023-05-30 06:40:32.937947 astro_sdk_python-1.7.0a3/src/astro/dataframes/__init__.py
+-rw-r--r--   0        0        0     4116 2023-05-30 06:40:32.938336 astro_sdk_python-1.7.0a3/src/astro/dataframes/load_options.py
+-rw-r--r--   0        0        0     2356 2023-05-30 06:40:32.938438 astro_sdk_python-1.7.0a3/src/astro/dataframes/pandas.py
+-rw-r--r--   0        0        0     1267 2023-05-30 06:40:32.938556 astro_sdk_python-1.7.0a3/src/astro/exceptions.py
+-rw-r--r--   0        0        0     1096 2023-05-30 06:40:32.938647 astro_sdk_python-1.7.0a3/src/astro/files/__init__.py
+-rw-r--r--   0        0        0    10151 2023-05-30 06:40:32.938972 astro_sdk_python-1.7.0a3/src/astro/files/base.py
+-rw-r--r--   0        0        0     1535 2023-05-30 06:40:32.939205 astro_sdk_python-1.7.0a3/src/astro/files/locations/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-30 06:40:32.939247 astro_sdk_python-1.7.0a3/src/astro/files/locations/amazon/__init__.py
+-rw-r--r--   0        0        0     3605 2023-05-30 06:40:32.939509 astro_sdk_python-1.7.0a3/src/astro/files/locations/amazon/s3.py
+-rw-r--r--   0        0        0        0 2023-05-30 06:40:32.939562 astro_sdk_python-1.7.0a3/src/astro/files/locations/azure/__init__.py
+-rw-r--r--   0        0        0     5867 2023-05-30 06:40:32.939668 astro_sdk_python-1.7.0a3/src/astro/files/locations/azure/wasb.py
+-rw-r--r--   0        0        0     6601 2023-05-30 06:40:32.939759 astro_sdk_python-1.7.0a3/src/astro/files/locations/base.py
+-rw-r--r--   0        0        0     2374 2023-05-30 06:40:32.939870 astro_sdk_python-1.7.0a3/src/astro/files/locations/ftp.py
+-rw-r--r--   0        0        0        0 2023-05-30 06:40:32.939919 astro_sdk_python-1.7.0a3/src/astro/files/locations/google/__init__.py
+-rw-r--r--   0        0        0     4420 2023-05-30 06:40:32.940070 astro_sdk_python-1.7.0a3/src/astro/files/locations/google/gcs.py
+-rw-r--r--   0        0        0     5006 2023-05-30 06:40:32.940171 astro_sdk_python-1.7.0a3/src/astro/files/locations/google/gdrive.py
+-rw-r--r--   0        0        0     1303 2023-05-30 06:40:32.940245 astro_sdk_python-1.7.0a3/src/astro/files/locations/http.py
+-rw-r--r--   0        0        0     1531 2023-05-30 06:40:32.940315 astro_sdk_python-1.7.0a3/src/astro/files/locations/local.py
+-rw-r--r--   0        0        0     3267 2023-05-30 06:40:32.940371 astro_sdk_python-1.7.0a3/src/astro/files/locations/sftp.py
+-rw-r--r--   0        0        0        0 2023-05-30 06:40:32.940409 astro_sdk_python-1.7.0a3/src/astro/files/operators/__init__.py
+-rw-r--r--   0        0        0     1595 2023-05-30 06:40:32.940496 astro_sdk_python-1.7.0a3/src/astro/files/operators/files.py
+-rw-r--r--   0        0        0     2576 2023-05-30 06:40:32.940578 astro_sdk_python-1.7.0a3/src/astro/files/types/__init__.py
+-rw-r--r--   0        0        0     1504 2023-05-30 06:40:32.940656 astro_sdk_python-1.7.0a3/src/astro/files/types/base.py
+-rw-r--r--   0        0        0     1900 2023-05-30 06:40:32.941199 astro_sdk_python-1.7.0a3/src/astro/files/types/csv.py
+-rw-r--r--   0        0        0     2197 2023-05-30 06:40:32.941426 astro_sdk_python-1.7.0a3/src/astro/files/types/json.py
+-rw-r--r--   0        0        0     3652 2023-05-30 06:40:32.941597 astro_sdk_python-1.7.0a3/src/astro/files/types/ndjson.py
+-rw-r--r--   0        0        0     2848 2023-05-30 06:40:32.942005 astro_sdk_python-1.7.0a3/src/astro/files/types/parquet.py
+-rw-r--r--   0        0        0      700 2023-05-30 06:40:32.942094 astro_sdk_python-1.7.0a3/src/astro/lineage/__init__.py
+-rw-r--r--   0        0        0     4264 2023-05-30 06:40:32.942177 astro_sdk_python-1.7.0a3/src/astro/lineage/facets.py
+-rw-r--r--   0        0        0     3910 2023-05-30 06:40:32.942322 astro_sdk_python-1.7.0a3/src/astro/options.py
+-rw-r--r--   0        0        0     1117 2023-05-30 06:40:32.942391 astro_sdk_python-1.7.0a3/src/astro/query_modifier.py
+-rw-r--r--   0        0        0     4152 2023-05-30 06:40:32.942615 astro_sdk_python-1.7.0a3/src/astro/settings.py
+-rw-r--r--   0        0        0     3194 2023-05-30 06:40:32.942746 astro_sdk_python-1.7.0a3/src/astro/sql/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-30 06:40:32.942788 astro_sdk_python-1.7.0a3/src/astro/sql/operators/__init__.py
+-rw-r--r--   0        0        0     7857 2023-05-30 06:40:32.942906 astro_sdk_python-1.7.0a3/src/astro/sql/operators/append.py
+-rw-r--r--   0        0        0    18419 2023-05-30 06:40:32.943035 astro_sdk_python-1.7.0a3/src/astro/sql/operators/base_decorator.py
+-rw-r--r--   0        0        0      334 2023-05-30 06:40:32.943118 astro_sdk_python-1.7.0a3/src/astro/sql/operators/base_operator.py
+-rw-r--r--   0        0        0    12688 2023-05-30 06:40:32.944049 astro_sdk_python-1.7.0a3/src/astro/sql/operators/cleanup.py
+-rw-r--r--   0        0        0     7870 2023-05-30 06:40:32.944217 astro_sdk_python-1.7.0a3/src/astro/sql/operators/data_validations/check_column.py
+-rw-r--r--   0        0        0     3696 2023-05-30 06:40:32.944301 astro_sdk_python-1.7.0a3/src/astro/sql/operators/data_validations/check_table.py
+-rw-r--r--   0        0        0    15362 2023-05-30 06:40:32.944436 astro_sdk_python-1.7.0a3/src/astro/sql/operators/dataframe.py
+-rw-r--r--   0        0        0     1435 2023-05-30 06:40:32.944528 astro_sdk_python-1.7.0a3/src/astro/sql/operators/drop.py
+-rw-r--r--   0        0        0     2693 2023-05-30 06:40:32.944754 astro_sdk_python-1.7.0a3/src/astro/sql/operators/export_file.py
+-rw-r--r--   0        0        0     2715 2023-05-30 06:40:32.944834 astro_sdk_python-1.7.0a3/src/astro/sql/operators/export_table_to_file.py
+-rw-r--r--   0        0        0     7035 2023-05-30 06:40:32.944917 astro_sdk_python-1.7.0a3/src/astro/sql/operators/export_to_file.py
+-rw-r--r--   0        0        0    17526 2023-05-30 06:40:32.945308 astro_sdk_python-1.7.0a3/src/astro/sql/operators/load_file.py
+-rw-r--r--   0        0        0     8824 2023-05-30 06:40:32.945467 astro_sdk_python-1.7.0a3/src/astro/sql/operators/merge.py
+-rw-r--r--   0        0        0     9898 2023-05-30 06:40:32.945582 astro_sdk_python-1.7.0a3/src/astro/sql/operators/raw_sql.py
+-rw-r--r--   0        0        0     8055 2023-05-30 06:40:32.945979 astro_sdk_python-1.7.0a3/src/astro/sql/operators/transform.py
+-rw-r--r--   0        0        0      880 2023-05-30 06:40:32.946078 astro_sdk_python-1.7.0a3/src/astro/sql/operators/upstream_task_mixin.py
+-rw-r--r--   0        0        0      160 2023-05-30 06:40:32.946155 astro_sdk_python-1.7.0a3/src/astro/sql/table.py
+-rw-r--r--   0        0        0     8747 2023-05-30 06:40:32.946428 astro_sdk_python-1.7.0a3/src/astro/table.py
+-rw-r--r--   0        0        0        0 2023-05-30 06:40:32.946485 astro_sdk_python-1.7.0a3/src/astro/utils/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-30 06:40:32.946548 astro_sdk_python-1.7.0a3/src/astro/utils/compat/__init__.py
+-rw-r--r--   0        0        0      359 2023-05-30 06:40:32.946630 astro_sdk_python-1.7.0a3/src/astro/utils/compat/functools.py
+-rw-r--r--   0        0        0      843 2023-05-30 06:40:32.946707 astro_sdk_python-1.7.0a3/src/astro/utils/compat/typing.py
+-rw-r--r--   0        0        0     2022 2023-05-30 06:40:32.946796 astro_sdk_python-1.7.0a3/src/astro/utils/dataframe.py
+-rw-r--r--   0        0        0     1581 2023-05-30 06:40:32.946898 astro_sdk_python-1.7.0a3/src/astro/utils/load.py
+-rw-r--r--   0        0        0     2790 2023-05-30 06:40:32.946979 astro_sdk_python-1.7.0a3/src/astro/utils/path.py
+-rw-r--r--   0        0        0     4025 2023-05-30 06:40:32.947057 astro_sdk_python-1.7.0a3/src/astro/utils/table.py
+-rw-r--r--   0        0        0    13476 1970-01-01 00:00:00.000000 astro_sdk_python-1.7.0a3/PKG-INFO
```

### Comparing `astro-sdk-python-1.7.0a2/README.md` & `astro_sdk_python-1.7.0a3/README.md`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a2/pyproject.toml` & `astro_sdk_python-1.7.0a3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -136,15 +136,15 @@
     "sphinx>=4.4.0",
     "sphinx-autoapi==2.0.0", # Multiple FileType class (same name) import is broken in sphinx-autoapi 2.0.1
     "sphinx-rtd-theme"
 ]
 
 [project.urls]
 Home = "https://astronomer.io/"
-Source = "https://github.com/astronomer/astro-sdk/python-sdk"
+Source = "https://github.com/astronomer/astro-sdk/tree/main/python-sdk"
 Documentation = "https://astro-sdk-python.rtfd.io/"
 
 [project.entry-points.apache_airflow_provider]
 provider_info = "astro.__init__:get_provider_info"
 
 [tool.pytest.ini_options]
 minversion = "6.0"
```

### Comparing `astro-sdk-python-1.7.0a2/src/astro/__init__.py` & `astro_sdk_python-1.7.0a3/src/astro/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """A decorator that allows users to run SQL queries natively in Airflow."""
 
-__version__ = "1.7.0a2"
+__version__ = "1.7.0a3"
 
 
 # This is needed to allow Airflow to pick up specific metadata fields it needs
 # for certain features. We recognize it's a bit unclean to define these in
 # multiple places, but at this point it's the only workaround if you'd like
 # your custom conn type to show up in the Airflow UI.
 def get_provider_info() -> dict:
```

### Comparing `astro-sdk-python-1.7.0a2/src/astro/airflow/datasets.py` & `astro_sdk_python-1.7.0a3/src/astro/airflow/datasets.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a2/src/astro/constants.py` & `astro_sdk_python-1.7.0a3/src/astro/constants.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a2/src/astro/custom_backend/astro_custom_backend.py` & `astro_sdk_python-1.7.0a3/src/astro/custom_backend/astro_custom_backend.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a2/src/astro/custom_backend/serializer.py` & `astro_sdk_python-1.7.0a3/src/astro/custom_backend/serializer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,35 @@
 from __future__ import annotations
 
 import json
 import logging
 from json import JSONDecodeError
 from typing import Any
 
-import airflow
 import numpy as np
 import pandas
+import sqlalchemy
+from packaging import version
 
-if airflow.__version__ >= "2.3":
+try:
     from sqlalchemy.engine.row import LegacyRow as SQLAlcRow
-else:
+except ImportError:
     from sqlalchemy.engine.result import RowProxy as SQLAlcRow
 
+
 from astro.files import File
 from astro.table import Table, TempTable
 
 log = logging.getLogger("astro.utils.serializer")
 
 
+def is_newer_sqlalchemy():
+    return version(sqlalchemy.__version__) >= version.parse("1.4.0")
+
+
 def serialize(obj: Table | File | Any) -> dict | Any:  # noqa
     """
     Serialize astro SDK objects (tables, files and dataframes) into json safe dictionary
 
     :param obj: object to serialize
     :return:
     """
@@ -48,15 +54,15 @@
         return obj.tolist()
     elif isinstance(obj, SQLAlcRow):
         serialized_obj = {
             "class": "SQLAlcRow",
             "key_map": obj._keymap,  # skipcq PYL-W021
             "key_style": obj._key_style,  # skipcq PYL-W021
         }
-        if airflow.__version__ >= "2.3":
+        if is_newer_sqlalchemy():
             serialized_obj["data"] = obj._data  # skipcq PYL-W021
         return serialized_obj
 
     elif isinstance(obj, str):
         return {"class": "string", "value": obj}
     else:
         return _attempt_to_serialize_unknown_object(obj)
@@ -86,15 +92,15 @@
         if obj["class"] == "Table":
             log.debug("Found table dictionary %s, will attempt to deserialize", obj)
             return Table.from_json(obj)
         elif obj["class"] == "File":
             log.debug("Found file dictionary %s, will attempt to deserialize", obj)
             return _deserialize_file(obj)
         elif obj["class"] == "SQLAlcRow":
-            if airflow.__version__ >= "2.3":
+            if is_newer_sqlalchemy():
                 return SQLAlcRow(None, None, obj["key_map"], obj["key_style"], obj["data"])
             else:
                 return SQLAlcRow(None, None, obj["key_map"], obj["key_style"])
         else:
             return obj["value"]
     elif isinstance(obj, dict):
         return {k: deserialize(v) for k, v in obj.items()}
```

### Comparing `astro-sdk-python-1.7.0a2/src/astro/databases/__init__.py` & `astro_sdk_python-1.7.0a3/src/astro/databases/__init__.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a2/src/astro/databases/aws/redshift.py` & `astro_sdk_python-1.7.0a3/src/astro/databases/aws/redshift.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a2/src/astro/databases/base.py` & `astro_sdk_python-1.7.0a3/src/astro/databases/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,14 +99,38 @@
         return self.sqlalchemy_engine.connect()
 
     @cached_property
     def sqlalchemy_engine(self) -> sqlalchemy.engine.base.Engine:
         """Return Sqlalchemy engine."""
         return self.hook.get_sqlalchemy_engine()  # type: ignore[no-any-return]
 
+    def run_single_sql_query(
+        self,
+        sql: str | ClauseElement = "",
+        parameters: dict | None = None,
+    ) -> Any:
+        """
+        Return the results to running a SQL statement.
+
+        Whenever possible, this method should be implemented using Airflow Hooks,
+        since this will simplify the integration with Async operators.
+
+        :param sql: Contains SQL query to be run against database
+        :param parameters: Optional parameters to be used to render the query
+        """
+        # We need to autocommit=True to make sure the query runs. This is done exclusively for SnowflakeDatabase's
+        # truncate method to reflect changes.
+        if isinstance(sql, str):
+            result = self.connection.execute(
+                sqlalchemy.text(sql).execution_options(autocommit=True), parameters
+            )
+        else:
+            result = self.connection.execute(sql, parameters)
+        return result
+
     def run_sql(
         self,
         sql: str | ClauseElement = "",
         parameters: dict | None = None,
         handler: Callable | None = None,
         query_modifier: QueryModifier = QueryModifier(),
         **kwargs,
@@ -130,23 +154,23 @@
             warnings.warn(
                 "`sql_statement` is deprecated and will be removed in future release"
                 "Please use  `sql` param instead.",
                 DeprecationWarning,
                 stacklevel=2,
             )
             sql = kwargs.get("sql_statement")  # type: ignore
-        sql = query_modifier.merge_pre_and_post_queries(sql)
-        # We need to autocommit=True to make sure the query runs. This is done exclusively for SnowflakeDatabase's
-        # truncate method to reflect changes.
-        if isinstance(sql, str):
-            result = self.connection.execute(
-                sqlalchemy.text(sql).execution_options(autocommit=True), parameters
-            )
-        else:
-            result = self.connection.execute(sql, parameters)
+
+        for sql_query in query_modifier.pre_queries:
+            _ = self.run_single_sql_query(sql_query, parameters)
+
+        result = self.run_single_sql_query(sql, parameters)
+
+        for sql_query in query_modifier.post_queries:
+            _ = self.run_single_sql_query(sql_query, parameters)
+
         if handler:
             return handler(result)
         return None
 
     def columns_exist(self, table: BaseTable, columns: list[str]) -> bool:
         """
         Check that a list of columns exist in the given table.
```

### Comparing `astro-sdk-python-1.7.0a2/src/astro/databases/databricks/api_utils.py` & `astro_sdk_python-1.7.0a3/src/astro/databases/databricks/api_utils.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a2/src/astro/databases/databricks/delta.py` & `astro_sdk_python-1.7.0a3/src/astro/databases/databricks/delta.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a2/src/astro/databases/databricks/load_file/jinja_templates/autoloader.py.jinja2` & `astro_sdk_python-1.7.0a3/src/astro/databases/databricks/load_file/jinja_templates/autoloader.py.jinja2`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a2/src/astro/databases/databricks/load_file/jinja_templates/copy_into.py.jinja2` & `astro_sdk_python-1.7.0a3/src/astro/databases/databricks/load_file/jinja_templates/copy_into.py.jinja2`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a2/src/astro/databases/databricks/load_file/jinja_templates/load_file_to_delta.py.jinja2` & `astro_sdk_python-1.7.0a3/src/astro/databases/databricks/load_file/jinja_templates/load_file_to_delta.py.jinja2`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a2/src/astro/databases/databricks/load_file/jinja_templates/load_secrets.py.jinja2` & `astro_sdk_python-1.7.0a3/src/astro/databases/databricks/load_file/jinja_templates/load_secrets.py.jinja2`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a2/src/astro/databases/databricks/load_file/load_file_job.py` & `astro_sdk_python-1.7.0a3/src/astro/databases/databricks/load_file/load_file_job.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a2/src/astro/databases/databricks/load_file/load_file_python_code_generator.py` & `astro_sdk_python-1.7.0a3/src/astro/databases/databricks/load_file/load_file_python_code_generator.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a2/src/astro/databases/databricks/load_options.py` & `astro_sdk_python-1.7.0a3/src/astro/databases/databricks/load_options.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a2/src/astro/databases/duckdb.py` & `astro_sdk_python-1.7.0a3/src/astro/databases/duckdb.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a2/src/astro/databases/google/bigquery.py` & `astro_sdk_python-1.7.0a3/src/astro/databases/google/bigquery.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a2/src/astro/databases/mssql.py` & `astro_sdk_python-1.7.0a3/src/astro/databases/mssql.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a2/src/astro/databases/mysql.py` & `astro_sdk_python-1.7.0a3/src/astro/databases/mysql.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a2/src/astro/databases/postgres.py` & `astro_sdk_python-1.7.0a3/src/astro/databases/postgres.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a2/src/astro/databases/snowflake.py` & `astro_sdk_python-1.7.0a3/src/astro/databases/snowflake.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a2/src/astro/databases/sqlite.py` & `astro_sdk_python-1.7.0a3/src/astro/databases/sqlite.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a2/src/astro/dataframes/load_options.py` & `astro_sdk_python-1.7.0a3/src/astro/dataframes/load_options.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a2/src/astro/dataframes/pandas.py` & `astro_sdk_python-1.7.0a3/src/astro/dataframes/pandas.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a2/src/astro/exceptions.py` & `astro_sdk_python-1.7.0a3/src/astro/exceptions.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a2/src/astro/files/__init__.py` & `astro_sdk_python-1.7.0a3/src/astro/files/__init__.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a2/src/astro/files/base.py` & `astro_sdk_python-1.7.0a3/src/astro/files/base.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a2/src/astro/files/locations/__init__.py` & `astro_sdk_python-1.7.0a3/src/astro/files/locations/__init__.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a2/src/astro/files/locations/amazon/s3.py` & `astro_sdk_python-1.7.0a3/src/astro/files/locations/amazon/s3.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a2/src/astro/files/locations/azure/wasb.py` & `astro_sdk_python-1.7.0a3/src/astro/files/locations/azure/wasb.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a2/src/astro/files/locations/base.py` & `astro_sdk_python-1.7.0a3/src/astro/files/locations/base.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a2/src/astro/files/locations/ftp.py` & `astro_sdk_python-1.7.0a3/src/astro/files/locations/ftp.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a2/src/astro/files/locations/google/gcs.py` & `astro_sdk_python-1.7.0a3/src/astro/files/locations/google/gcs.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a2/src/astro/files/locations/google/gdrive.py` & `astro_sdk_python-1.7.0a3/src/astro/files/locations/google/gdrive.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a2/src/astro/files/locations/http.py` & `astro_sdk_python-1.7.0a3/src/astro/files/locations/http.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a2/src/astro/files/locations/local.py` & `astro_sdk_python-1.7.0a3/src/astro/files/locations/local.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a2/src/astro/files/locations/sftp.py` & `astro_sdk_python-1.7.0a3/src/astro/files/locations/sftp.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a2/src/astro/files/operators/files.py` & `astro_sdk_python-1.7.0a3/src/astro/files/operators/files.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a2/src/astro/files/types/__init__.py` & `astro_sdk_python-1.7.0a3/src/astro/files/types/__init__.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a2/src/astro/files/types/base.py` & `astro_sdk_python-1.7.0a3/src/astro/files/types/base.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a2/src/astro/files/types/csv.py` & `astro_sdk_python-1.7.0a3/src/astro/files/types/csv.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a2/src/astro/files/types/json.py` & `astro_sdk_python-1.7.0a3/src/astro/files/types/json.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a2/src/astro/files/types/ndjson.py` & `astro_sdk_python-1.7.0a3/src/astro/files/types/ndjson.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a2/src/astro/files/types/parquet.py` & `astro_sdk_python-1.7.0a3/src/astro/files/types/parquet.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a2/src/astro/lineage/__init__.py` & `astro_sdk_python-1.7.0a3/src/astro/lineage/__init__.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a2/src/astro/lineage/facets.py` & `astro_sdk_python-1.7.0a3/src/astro/lineage/facets.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a2/src/astro/options.py` & `astro_sdk_python-1.7.0a3/src/astro/options.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a2/src/astro/query_modifier.py` & `astro_sdk_python-1.7.0a3/src/astro/query_modifier.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a2/src/astro/settings.py` & `astro_sdk_python-1.7.0a3/src/astro/settings.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a2/src/astro/sql/__init__.py` & `astro_sdk_python-1.7.0a3/src/astro/sql/__init__.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a2/src/astro/sql/operators/append.py` & `astro_sdk_python-1.7.0a3/src/astro/sql/operators/append.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a2/src/astro/sql/operators/base_decorator.py` & `astro_sdk_python-1.7.0a3/src/astro/sql/operators/base_decorator.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a2/src/astro/sql/operators/cleanup.py` & `astro_sdk_python-1.7.0a3/src/astro/sql/operators/cleanup.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a2/src/astro/sql/operators/data_validations/check_column.py` & `astro_sdk_python-1.7.0a3/src/astro/sql/operators/data_validations/check_column.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a2/src/astro/sql/operators/data_validations/check_table.py` & `astro_sdk_python-1.7.0a3/src/astro/sql/operators/data_validations/check_table.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a2/src/astro/sql/operators/dataframe.py` & `astro_sdk_python-1.7.0a3/src/astro/sql/operators/dataframe.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a2/src/astro/sql/operators/drop.py` & `astro_sdk_python-1.7.0a3/src/astro/sql/operators/drop.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a2/src/astro/sql/operators/export_file.py` & `astro_sdk_python-1.7.0a3/src/astro/sql/operators/export_file.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a2/src/astro/sql/operators/export_table_to_file.py` & `astro_sdk_python-1.7.0a3/src/astro/sql/operators/export_table_to_file.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a2/src/astro/sql/operators/export_to_file.py` & `astro_sdk_python-1.7.0a3/src/astro/sql/operators/export_to_file.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a2/src/astro/sql/operators/load_file.py` & `astro_sdk_python-1.7.0a3/src/astro/sql/operators/load_file.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a2/src/astro/sql/operators/merge.py` & `astro_sdk_python-1.7.0a3/src/astro/sql/operators/merge.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a2/src/astro/sql/operators/raw_sql.py` & `astro_sdk_python-1.7.0a3/src/astro/sql/operators/raw_sql.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a2/src/astro/sql/operators/transform.py` & `astro_sdk_python-1.7.0a3/src/astro/sql/operators/transform.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a2/src/astro/sql/operators/upstream_task_mixin.py` & `astro_sdk_python-1.7.0a3/src/astro/sql/operators/upstream_task_mixin.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a2/src/astro/table.py` & `astro_sdk_python-1.7.0a3/src/astro/table.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a2/src/astro/utils/compat/typing.py` & `astro_sdk_python-1.7.0a3/src/astro/utils/compat/typing.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a2/src/astro/utils/dataframe.py` & `astro_sdk_python-1.7.0a3/src/astro/utils/dataframe.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a2/src/astro/utils/load.py` & `astro_sdk_python-1.7.0a3/src/astro/utils/load.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a2/src/astro/utils/path.py` & `astro_sdk_python-1.7.0a3/src/astro/utils/path.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a2/src/astro/utils/table.py` & `astro_sdk_python-1.7.0a3/src/astro/utils/table.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a2/PKG-INFO` & `astro_sdk_python-1.7.0a3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astro-sdk-python
-Version: 1.7.0a2
+Version: 1.7.0a3
 Summary: Astro SDK allows rapid and clean development of {Extract, Load, Transform} workflows using Python and SQL, powered by Apache Airflow.
 Keywords: airflow,provider,astronomer,sql,decorator,task flow,elt,etl,dag
 Author-email: Astronomer <humans@astronomer.io>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
@@ -80,15 +80,15 @@
 Requires-Dist: pytest-cov ; extra == "tests"
 Requires-Dist: pytest-describe ; extra == "tests"
 Requires-Dist: types-requests ; extra == "tests"
 Requires-Dist: mypy ; extra == "tests"
 Requires-Dist: sqlalchemy-stubs ; extra == "tests"
 Project-URL: Documentation, https://astro-sdk-python.rtfd.io/
 Project-URL: Home, https://astronomer.io/
-Project-URL: Source, https://github.com/astronomer/astro-sdk/python-sdk
+Project-URL: Source, https://github.com/astronomer/astro-sdk/tree/main/python-sdk
 Provides-Extra: all
 Provides-Extra: amazon
 Provides-Extra: azure
 Provides-Extra: databricks
 Provides-Extra: doc
 Provides-Extra: duckdb
 Provides-Extra: ftp
```

