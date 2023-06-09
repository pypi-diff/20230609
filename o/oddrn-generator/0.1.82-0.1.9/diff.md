# Comparing `tmp/oddrn_generator-0.1.82.tar.gz` & `tmp/oddrn-generator-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oddrn_generator-0.1.82.tar", max compression
+gzip compressed data, was "oddrn-generator-0.1.9.tar", max compression
```

## Comparing `oddrn_generator-0.1.82.tar` & `oddrn-generator-0.1.9.tar`

### file list

```diff
@@ -1,12 +1,10 @@
--rw-r--r--   0        0        0    11356 2023-06-09 10:10:15.000000 oddrn_generator-0.1.82/LICENSE
--rw-r--r--   0        0        0     6337 2023-06-09 10:10:15.000000 oddrn_generator-0.1.82/README.md
--rw-r--r--   0        0        0     2496 2023-06-09 10:10:15.000000 oddrn_generator-0.1.82/oddrn_generator/__init__.py
--rw-r--r--   0        0        0      158 2023-06-09 10:10:15.000000 oddrn_generator-0.1.82/oddrn_generator/exceptions.py
--rw-r--r--   0        0        0    11982 2023-06-09 10:10:15.000000 oddrn_generator-0.1.82/oddrn_generator/generators.py
--rw-r--r--   0        0        0    23423 2023-06-09 10:10:15.000000 oddrn_generator-0.1.82/oddrn_generator/path_models.py
--rw-r--r--   0        0        0     3115 2023-06-09 10:10:15.000000 oddrn_generator-0.1.82/oddrn_generator/server_models.py
--rw-r--r--   0        0        0      287 2023-06-09 10:10:15.000000 oddrn_generator-0.1.82/oddrn_generator/utils/__init__.py
--rw-r--r--   0        0        0     7327 2023-06-09 10:10:15.000000 oddrn_generator-0.1.82/oddrn_generator/utils/external_generators.py
--rw-r--r--   0        0        0      734 2023-06-09 10:10:40.000000 oddrn_generator-0.1.82/pyproject.toml
--rw-r--r--   0        0        0     7363 1970-01-01 00:00:00.000000 oddrn_generator-0.1.82/setup.py
--rw-r--r--   0        0        0     7089 1970-01-01 00:00:00.000000 oddrn_generator-0.1.82/PKG-INFO
+-rw-r--r--   0        0        0    11356 2021-10-08 14:14:06.775943 oddrn-generator-0.1.9/LICENSE
+-rw-r--r--   0        0        0     4970 2021-10-18 10:25:57.387497 oddrn-generator-0.1.9/README.md
+-rw-r--r--   0        0        0      842 2021-10-18 12:18:05.407813 oddrn-generator-0.1.9/oddrn_generator/__init__.py
+-rw-r--r--   0        0        0      157 2021-10-08 14:14:06.777038 oddrn-generator-0.1.9/oddrn_generator/exceptions.py
+-rw-r--r--   0        0        0     5346 2021-10-18 10:28:14.410979 oddrn-generator-0.1.9/oddrn_generator/generators.py
+-rw-r--r--   0        0        0    10224 2021-10-18 12:18:05.411939 oddrn-generator-0.1.9/oddrn_generator/path_models.py
+-rw-r--r--   0        0        0      529 2021-10-08 14:14:06.777467 oddrn-generator-0.1.9/oddrn_generator/server_models.py
+-rw-r--r--   0        0        0      627 2021-10-18 12:18:05.403660 oddrn-generator-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     5904 2021-10-18 12:18:39.384833 oddrn-generator-0.1.9/setup.py
+-rw-r--r--   0        0        0     5719 2021-10-18 12:18:39.385238 oddrn-generator-0.1.9/PKG-INFO
```

### Comparing `oddrn_generator-0.1.82/LICENSE` & `oddrn-generator-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `oddrn_generator-0.1.82/README.md` & `oddrn-generator-0.1.9/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,102 +1,64 @@
-[![PyPI version](https://badge.fury.io/py/oddrn-generator.svg)](https://badge.fury.io/py/oddrn-generator)
-
 # Open Data Discovery Resource Name Generator
-
-Helps generate oddrn for data sources.
-
-* [Requirements](#requirements)
-* [Installation](#installation)
-* [Available generators](#available-generators)
-* [Generator properties](#generator-properties)
-* [Generator methods](#generator-methods)
-* [Generator properties](#generator-properties)
-* [Example usage](#example-usage)
-* [Exceptions](#example-usage)
-* [Development](#development)
-
 ## Requirements
-
-* __Python >= 3.7__
-
+Python >= 3.7
 ## Installation
-
-```bash
-poetry add oddrn-generator
-# or
-pip install oddrn-generator
 ```
-
+poetry install
+```
 ## Usage and configuration
-
 ### Available generators
-| DataSource   | Generator class name  |
-|--------------|-----------------------|
-| cassandra    | CassandraGenerator    |
-| postgresql   | PostgresqlGenerator   |
-| mysql        | MysqlGenerator        |
-| glue         | GlueGenerator         |
-| s3           | S3Generator           |
-| kafka        | KafkaGenerator        |
-| kafkaconnect | KafkaConnectGenerator |
-| snowflake    | SnowflakeGenerator    |
-| airflow      | AirflowGenerator      |
-| hive         | HiveGenerator         |
-| dynamodb     | DynamodbGenerator     |
-| odbc         | OdbcGenerator         |
-| mssql        | MssqlGenerator        |
-| oracle       | OracleGenerator       |
-| redshift     | RedshiftGenerator     |
-| clickhouse   | ClickHouseGenerator   |
-| athena       | AthenaGenerator       |
-| quicksight   | QuicksightGenerator   |
-| dbt          | DbtGenerator          |
-| prefect      | PrefectGenerator      |
-| tableau      | TableauGenerator      |
-| neo4j        | Neo4jGenerator        |
-| mongodb      | MongoGenerator        |
-| vertica      | VerticaGenerator      |
-| CubeJs       | CubeJsGenerator       |
-| superset     | SupersetGenerator     |
-| Presto       | PrestoGenerator       |
-| Trino        | TrinoGenerator        |
-| dms          | DmsGenerator          |
-| powerbi      | PowerBiGenerator      |
+* postgresql - PostgresqlGenerator
+* mysql - MysqlGenerator
+* glue - GlueGenerator
+* kafka - KafkaGenerator
+* kafkaconnect - KafkaConnectGenerator
+* snowflake - SnowflakeGenerator
+* airflow - AirflowGenerator
+* hive - HiveGenerator
+* dynamodb - DynamodbGenerator
+* odbc - OdbcGenerator
+* mssql - MssqlGenerator
+* oracle - OracleGenerator
+* redshift - RedshiftGenerator
+* clickhouse - ClickHouseGenerator
+* athena - AthenaGenerator
+* quicksight - QuicksightGenerator
+* dbt - DbtGenerator
+* tableau - TableauGenerator
+### Work in progress generators
+* kubeflow - KubeflowGenerator
+* dvc - DVCGenerator
+* great_expectations - GreatExpectationsGenerator
 
 ### Generator properties
-
 * base_oddrn - Get base oddrn (without path)
-* available_paths - Get all available path of generator
+* available_paths - Get all available path of generator 
 
 ### Generator methods
-
-* get_oddrn_by_path(path_name, new_value=None) - Get oddrn string by path. You also can set value for this path using '
-  new_value' param
+* get_oddrn_by_path(path_name, new_value=None) - Get oddrn string by path. You also can set value for this path using 'new_value' param
 * set_oddrn_paths(**kwargs) - Set or update values of oddrn path
-* get_data_source_oddrn() - Get data source oddrn
+* get_data_source_oddrn() - Get datasouce oddrn 
 
 ### Generator parameters:
-
 * host_settings: str - optional. Hostname configuration
-* cloud_settings: dict - optional. Cloud configuration
+* cloud_settings: dict - optional.  Cloud configuration
 * **kwargs - path's name and values
 
 ### Example usage
-
 ```python
 # postgresql
 from oddrn_generator import PostgresqlGenerator
-
 oddrn_gen = PostgresqlGenerator(
-    host_settings='my.host.com:5432',
-    schemas='schema_name', databases='database_name', tables='table_name'
+  host_settings='my.host.com:5432', 
+  schemas='schema_name', databases='database_name', tables='table_name'
 )
 
 oddrn_gen.base_oddrn
-# //postgresql/host/my.host.com:5432
+# //postgresql/host/my.host.com:5432/
 oddrn_gen.available_paths
 # ('schemas', 'databases', 'tables', 'columns')
 
 oddrn_gen.get_data_source_oddrn()
 # //postgresql/host/my.host.com:5432/schemas/schema_name/databases/database_name
 
 oddrn_gen.get_oddrn_by_path("schemas")
@@ -116,19 +78,18 @@
 # you can get path wih new values:
 oddrn_gen.get_oddrn_by_path("columns", new_value="another_new_column_name")
 # //postgresql/host/my.host.com:5432/schemas/schema_name/databases/database_name/tables/another_table_name/columns/another_new_column_name
 
 
 # glue
 from oddrn_generator import GlueGenerator
-
 oddrn_gen = GlueGenerator(
-    cloud_settings={'account': 'acc_id', 'region': 'reg_id'},
-    databases='database_name', tables='table_name', columns='column_name',
-    jobs='job_name', runs='run_name', owners='owner_name'
+  cloud_settings={'account': 'acc_id', 'region':'reg_id'}, 
+  databases='database_name', tables='table_name', columns='column_name', 
+  jobs='job_name', runs='run_name', owners='owner_name'
 )
 
 oddrn_gen.available_paths
 # ('databases', 'tables', 'columns', 'owners', 'jobs', 'runs')
 
 oddrn_gen.get_oddrn_by_path("databases")
 # //glue/cloud/aws/account/acc_id/region/reg_id/databases/database_name
@@ -147,59 +108,37 @@
 
 oddrn_gen.get_oddrn_by_path("owners")
 # //glue/cloud/aws/account/acc_id/region/reg_id/owners/owner_name
 
 ```
 
 ### Exceptions
-
 * WrongPathOrderException - raises when trying set path that depends on another path
-
 ```python
 from oddrn_generator import PostgresqlGenerator
-
 oddrn_gen = PostgresqlGenerator(
-    host_settings='my.host.com:5432',
+    host_settings='my.host.com:5432', 
     schemas='schema_name', databases='database_name',
     columns='column_without_table'
 )
 # WrongPathOrderException: 'columns' can not be without 'tables' attribute
 ```
-
 * EmptyPathValueException - raises when trying to get a path that is not set up
-
 ```python
 from oddrn_generator import PostgresqlGenerator
-
 oddrn_gen = PostgresqlGenerator(
     host_settings='my.host.com:5432', schemas='schema_name', databases='database_name',
 )
 oddrn_gen.get_oddrn_by_path("tables")
 
 # EmptyPathValueException: Path 'tables' is not set up
 ```
-
 * PathDoestExistException - raises when trying to get not existing oddrn path
-
 ```python
 from oddrn_generator import PostgresqlGenerator
-
 oddrn_gen = PostgresqlGenerator(
     host_settings='my.host.com:5432', schemas='schema_name', databases='database_name',
 )
 oddrn_gen.get_oddrn_by_path("jobs")
 
 # PathDoestExistException: Path 'jobs' doesn't exist in generator
-```
-
-## Development
-
-```bash
-#Install dependencies
-poetry install
-
-#Activate shell
-poetry shell
-
-# Run tests
-python run pytest
-```
+```
```

### Comparing `oddrn_generator-0.1.82/pyproject.toml` & `oddrn-generator-0.1.9/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,23 @@
 [tool.poetry]
 name = "oddrn-generator"
-version = "0.1.82"
+version = "0.1.9"
 description = "Open Data Discovery Resource Name Generator"
 authors = ["Open Data Discovery <pypi@opendatadiscovery.org>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/opendatadiscovery/oddrn-generator"
 repository = "https://github.com/opendatadiscovery/oddrn-generator"
 keywords = ["oddrn", "opendatadiscovery"]
 include = ["LICENSE"]
 
 
 [tool.poetry.dependencies]
-python = "^3.9"
-pydantic = "^1.9.1"
+python = "^3.7"
+pydantic = "^1.8.2"
 
 [tool.poetry.dev-dependencies]
 pytest = "^5.2"
-black = "^22.8.0"
-
-[tool.poetry.group.dev.dependencies]
-isort = "^5.12.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
-
-[tool.isort]
-profile = "black"
```

### Comparing `oddrn_generator-0.1.82/PKG-INFO` & `oddrn-generator-0.1.9/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,121 +1,83 @@
 Metadata-Version: 2.1
 Name: oddrn-generator
-Version: 0.1.82
+Version: 0.1.9
 Summary: Open Data Discovery Resource Name Generator
 Home-page: https://github.com/opendatadiscovery/oddrn-generator
 License: Apache-2.0
 Keywords: oddrn,opendatadiscovery
 Author: Open Data Discovery
 Author-email: pypi@opendatadiscovery.org
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: pydantic (>=1.9.1,<2.0.0)
+Requires-Dist: pydantic (>=1.8.2,<2.0.0)
 Project-URL: Repository, https://github.com/opendatadiscovery/oddrn-generator
 Description-Content-Type: text/markdown
 
-[![PyPI version](https://badge.fury.io/py/oddrn-generator.svg)](https://badge.fury.io/py/oddrn-generator)
-
 # Open Data Discovery Resource Name Generator
-
-Helps generate oddrn for data sources.
-
-* [Requirements](#requirements)
-* [Installation](#installation)
-* [Available generators](#available-generators)
-* [Generator properties](#generator-properties)
-* [Generator methods](#generator-methods)
-* [Generator properties](#generator-properties)
-* [Example usage](#example-usage)
-* [Exceptions](#example-usage)
-* [Development](#development)
-
 ## Requirements
-
-* __Python >= 3.7__
-
+Python >= 3.7
 ## Installation
-
-```bash
-poetry add oddrn-generator
-# or
-pip install oddrn-generator
 ```
-
+poetry install
+```
 ## Usage and configuration
-
 ### Available generators
-| DataSource   | Generator class name  |
-|--------------|-----------------------|
-| cassandra    | CassandraGenerator    |
-| postgresql   | PostgresqlGenerator   |
-| mysql        | MysqlGenerator        |
-| glue         | GlueGenerator         |
-| s3           | S3Generator           |
-| kafka        | KafkaGenerator        |
-| kafkaconnect | KafkaConnectGenerator |
-| snowflake    | SnowflakeGenerator    |
-| airflow      | AirflowGenerator      |
-| hive         | HiveGenerator         |
-| dynamodb     | DynamodbGenerator     |
-| odbc         | OdbcGenerator         |
-| mssql        | MssqlGenerator        |
-| oracle       | OracleGenerator       |
-| redshift     | RedshiftGenerator     |
-| clickhouse   | ClickHouseGenerator   |
-| athena       | AthenaGenerator       |
-| quicksight   | QuicksightGenerator   |
-| dbt          | DbtGenerator          |
-| prefect      | PrefectGenerator      |
-| tableau      | TableauGenerator      |
-| neo4j        | Neo4jGenerator        |
-| mongodb      | MongoGenerator        |
-| vertica      | VerticaGenerator      |
-| CubeJs       | CubeJsGenerator       |
-| superset     | SupersetGenerator     |
-| Presto       | PrestoGenerator       |
-| Trino        | TrinoGenerator        |
-| dms          | DmsGenerator          |
-| powerbi      | PowerBiGenerator      |
+* postgresql - PostgresqlGenerator
+* mysql - MysqlGenerator
+* glue - GlueGenerator
+* kafka - KafkaGenerator
+* kafkaconnect - KafkaConnectGenerator
+* snowflake - SnowflakeGenerator
+* airflow - AirflowGenerator
+* hive - HiveGenerator
+* dynamodb - DynamodbGenerator
+* odbc - OdbcGenerator
+* mssql - MssqlGenerator
+* oracle - OracleGenerator
+* redshift - RedshiftGenerator
+* clickhouse - ClickHouseGenerator
+* athena - AthenaGenerator
+* quicksight - QuicksightGenerator
+* dbt - DbtGenerator
+* tableau - TableauGenerator
+### Work in progress generators
+* kubeflow - KubeflowGenerator
+* dvc - DVCGenerator
+* great_expectations - GreatExpectationsGenerator
 
 ### Generator properties
-
 * base_oddrn - Get base oddrn (without path)
-* available_paths - Get all available path of generator
+* available_paths - Get all available path of generator 
 
 ### Generator methods
-
-* get_oddrn_by_path(path_name, new_value=None) - Get oddrn string by path. You also can set value for this path using '
-  new_value' param
+* get_oddrn_by_path(path_name, new_value=None) - Get oddrn string by path. You also can set value for this path using 'new_value' param
 * set_oddrn_paths(**kwargs) - Set or update values of oddrn path
-* get_data_source_oddrn() - Get data source oddrn
+* get_data_source_oddrn() - Get datasouce oddrn 
 
 ### Generator parameters:
-
 * host_settings: str - optional. Hostname configuration
-* cloud_settings: dict - optional. Cloud configuration
+* cloud_settings: dict - optional.  Cloud configuration
 * **kwargs - path's name and values
 
 ### Example usage
-
 ```python
 # postgresql
 from oddrn_generator import PostgresqlGenerator
-
 oddrn_gen = PostgresqlGenerator(
-    host_settings='my.host.com:5432',
-    schemas='schema_name', databases='database_name', tables='table_name'
+  host_settings='my.host.com:5432', 
+  schemas='schema_name', databases='database_name', tables='table_name'
 )
 
 oddrn_gen.base_oddrn
-# //postgresql/host/my.host.com:5432
+# //postgresql/host/my.host.com:5432/
 oddrn_gen.available_paths
 # ('schemas', 'databases', 'tables', 'columns')
 
 oddrn_gen.get_data_source_oddrn()
 # //postgresql/host/my.host.com:5432/schemas/schema_name/databases/database_name
 
 oddrn_gen.get_oddrn_by_path("schemas")
@@ -135,19 +97,18 @@
 # you can get path wih new values:
 oddrn_gen.get_oddrn_by_path("columns", new_value="another_new_column_name")
 # //postgresql/host/my.host.com:5432/schemas/schema_name/databases/database_name/tables/another_table_name/columns/another_new_column_name
 
 
 # glue
 from oddrn_generator import GlueGenerator
-
 oddrn_gen = GlueGenerator(
-    cloud_settings={'account': 'acc_id', 'region': 'reg_id'},
-    databases='database_name', tables='table_name', columns='column_name',
-    jobs='job_name', runs='run_name', owners='owner_name'
+  cloud_settings={'account': 'acc_id', 'region':'reg_id'}, 
+  databases='database_name', tables='table_name', columns='column_name', 
+  jobs='job_name', runs='run_name', owners='owner_name'
 )
 
 oddrn_gen.available_paths
 # ('databases', 'tables', 'columns', 'owners', 'jobs', 'runs')
 
 oddrn_gen.get_oddrn_by_path("databases")
 # //glue/cloud/aws/account/acc_id/region/reg_id/databases/database_name
@@ -166,60 +127,37 @@
 
 oddrn_gen.get_oddrn_by_path("owners")
 # //glue/cloud/aws/account/acc_id/region/reg_id/owners/owner_name
 
 ```
 
 ### Exceptions
-
 * WrongPathOrderException - raises when trying set path that depends on another path
-
 ```python
 from oddrn_generator import PostgresqlGenerator
-
 oddrn_gen = PostgresqlGenerator(
-    host_settings='my.host.com:5432',
+    host_settings='my.host.com:5432', 
     schemas='schema_name', databases='database_name',
     columns='column_without_table'
 )
 # WrongPathOrderException: 'columns' can not be without 'tables' attribute
 ```
-
 * EmptyPathValueException - raises when trying to get a path that is not set up
-
 ```python
 from oddrn_generator import PostgresqlGenerator
-
 oddrn_gen = PostgresqlGenerator(
     host_settings='my.host.com:5432', schemas='schema_name', databases='database_name',
 )
 oddrn_gen.get_oddrn_by_path("tables")
 
 # EmptyPathValueException: Path 'tables' is not set up
 ```
-
 * PathDoestExistException - raises when trying to get not existing oddrn path
-
 ```python
 from oddrn_generator import PostgresqlGenerator
-
 oddrn_gen = PostgresqlGenerator(
     host_settings='my.host.com:5432', schemas='schema_name', databases='database_name',
 )
 oddrn_gen.get_oddrn_by_path("jobs")
 
 # PathDoestExistException: Path 'jobs' doesn't exist in generator
 ```
-
-## Development
-
-```bash
-#Install dependencies
-poetry install
-
-#Activate shell
-poetry shell
-
-# Run tests
-python run pytest
-```
-
```

