# Comparing `tmp/data_check-0.8.0.tar.gz` & `tmp/data_check-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_check-0.8.0.tar", max compression
+gzip compressed data, was "data_check-0.9.0.tar", max compression
```

## Comparing `data_check-0.8.0.tar` & `data_check-0.9.0.tar`

### file list

```diff
@@ -1,34 +1,36 @@
--rwxr-xr-x   0        0        0     3769 2021-10-29 02:35:58.563682 data_check-0.8.0/CHANGELOG.md
--rwxr-xr-x   0        0        0     1064 2020-12-25 19:26:34.739712 data_check-0.8.0/LICENSE
--rwxr-xr-x   0        0        0     4225 2021-10-07 06:38:18.179005 data_check-0.8.0/README.md
--rwxr-xr-x   0        0        0      155 2021-08-17 10:43:31.441187 data_check-0.8.0/data_check/__init__.py
--rwxr-xr-x   0        0        0     5428 2021-10-29 02:35:58.584495 data_check-0.8.0/data_check/__main__.py
--rwxr-xr-x   0        0        0      316 2021-10-29 02:35:58.585496 data_check-0.8.0/data_check/checks/__init__.py
--rwxr-xr-x   0        0        0      587 2021-10-29 02:35:58.585609 data_check-0.8.0/data_check/checks/base_check.py
--rwxr-xr-x   0        0        0     4615 2021-10-29 02:35:58.586682 data_check-0.8.0/data_check/checks/csv_check.py
--rwxr-xr-x   0        0        0     1149 2021-10-29 02:35:58.586682 data_check-0.8.0/data_check/checks/empty_set_check.py
--rwxr-xr-x   0        0        0     1391 2021-10-29 02:35:58.587837 data_check-0.8.0/data_check/checks/excel_check.py
--rwxr-xr-x   0        0        0     1313 2021-10-29 02:35:58.588833 data_check-0.8.0/data_check/checks/generator.py
--rwxr-xr-x   0        0        0      558 2021-10-29 02:35:58.588833 data_check-0.8.0/data_check/checks/path_not_exists.py
--rwxr-xr-x   0        0        0       55 2021-10-29 02:35:58.590419 data_check-0.8.0/data_check/checks/pipeline_check/__init__.py
--rwxr-xr-x   0        0        0     1113 2021-10-29 02:35:58.590419 data_check-0.8.0/data_check/checks/pipeline_check/cmd_step.py
--rwxr-xr-x   0        0        0     7056 2021-10-29 02:35:58.591724 data_check-0.8.0/data_check/checks/pipeline_check/pipeline_check.py
--rwxr-xr-x   0        0        0     2185 2021-10-29 02:35:58.591724 data_check-0.8.0/data_check/checks/pipeline_check/serial_pipeline_steps.py
--rwxr-xr-x   0        0        0     3227 2021-10-29 02:35:58.592736 data_check-0.8.0/data_check/config.py
--rwxr-xr-x   0        0        0     4162 2021-10-29 02:35:58.593737 data_check-0.8.0/data_check/data_check.py
--rwxr-xr-x   0        0        0     1205 2021-10-29 02:35:58.594676 data_check-0.8.0/data_check/date.py
--rwxr-xr-x   0        0        0      136 2021-07-09 12:35:26.237153 data_check-0.8.0/data_check/exceptions.py
--rwxr-xr-x   0        0        0     3550 2021-10-29 02:35:58.595677 data_check-0.8.0/data_check/io.py
--rwxr-xr-x   0        0        0       49 2021-10-29 02:35:58.596677 data_check-0.8.0/data_check/output/__init__.py
--rwxr-xr-x   0        0        0     1301 2021-10-29 02:35:58.597676 data_check-0.8.0/data_check/output/handler.py
--rwxr-xr-x   0        0        0     6657 2021-10-29 02:35:58.598385 data_check-0.8.0/data_check/output/output.py
--rwxr-xr-x   0        0        0     1068 2021-10-29 02:35:58.599913 data_check-0.8.0/data_check/result.py
--rwxr-xr-x   0        0        0     3048 2021-10-29 02:35:58.600938 data_check-0.8.0/data_check/runner.py
--rwxr-xr-x   0        0        0       88 2021-10-29 02:35:58.600938 data_check-0.8.0/data_check/sql/__init__.py
--rwxr-xr-x   0        0        0      498 2021-10-29 02:35:58.601939 data_check-0.8.0/data_check/sql/load_mode.py
--rwxr-xr-x   0        0        0     1617 2021-10-29 02:35:58.602640 data_check-0.8.0/data_check/sql/query_result.py
--rwxr-xr-x   0        0        0     4086 2021-10-29 02:35:58.604642 data_check-0.8.0/data_check/sql/sql.py
--rwxr-xr-x   0        0        0     7696 2021-10-29 02:35:58.605288 data_check-0.8.0/data_check/sql/table_loader.py
--rwxr-xr-x   0        0        0     1611 2021-10-29 02:35:58.625900 data_check-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     5556 2021-10-29 02:36:06.204774 data_check-0.8.0/setup.py
--rw-r--r--   0        0        0     5897 2021-10-29 02:36:06.205530 data_check-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     4339 2021-12-17 16:57:40.860301 data_check-0.9.0/CHANGELOG.md
+-rwxr-xr-x   0        0        0     1064 2021-11-01 16:01:59.176192 data_check-0.9.0/LICENSE
+-rw-r--r--   0        0        0     4378 2021-12-17 16:57:40.860301 data_check-0.9.0/README.md
+-rw-r--r--   0        0        0      155 2021-11-09 05:23:03.530045 data_check-0.9.0/data_check/__init__.py
+-rw-r--r--   0        0        0     5803 2021-12-17 16:57:40.860301 data_check-0.9.0/data_check/__main__.py
+-rw-r--r--   0        0        0      316 2021-12-17 14:28:03.460301 data_check-0.9.0/data_check/checks/__init__.py
+-rw-r--r--   0        0        0      725 2021-12-17 16:57:40.860301 data_check-0.9.0/data_check/checks/base_check.py
+-rw-r--r--   0        0        0     4977 2021-12-17 16:57:40.860301 data_check-0.9.0/data_check/checks/csv_check.py
+-rw-r--r--   0        0        0     1214 2021-12-17 16:57:40.860301 data_check-0.9.0/data_check/checks/empty_set_check.py
+-rw-r--r--   0        0        0     1504 2021-12-17 16:57:40.860301 data_check-0.9.0/data_check/checks/excel_check.py
+-rw-r--r--   0        0        0     1367 2021-12-17 16:57:40.860301 data_check-0.9.0/data_check/checks/generator.py
+-rw-r--r--   0        0        0      558 2021-11-09 05:23:03.540045 data_check-0.9.0/data_check/checks/path_not_exists.py
+-rw-r--r--   0        0        0       55 2021-11-09 05:23:03.540045 data_check-0.9.0/data_check/checks/pipeline_check/__init__.py
+-rw-r--r--   0        0        0     1295 2021-12-17 16:57:40.860301 data_check-0.9.0/data_check/checks/pipeline_check/cmd_step.py
+-rw-r--r--   0        0        0     7773 2021-12-17 16:57:40.860301 data_check-0.9.0/data_check/checks/pipeline_check/pipeline_check.py
+-rw-r--r--   0        0        0     2820 2021-12-17 16:57:40.860301 data_check-0.9.0/data_check/checks/pipeline_check/serial_pipeline_steps.py
+-rw-r--r--   0        0        0     3516 2021-12-17 16:57:40.860301 data_check-0.9.0/data_check/config.py
+-rw-r--r--   0        0        0     4594 2021-12-17 16:57:40.860301 data_check-0.9.0/data_check/data_check.py
+-rw-r--r--   0        0        0     1253 2021-12-17 16:57:40.860301 data_check-0.9.0/data_check/date.py
+-rw-r--r--   0        0        0      136 2021-11-09 05:23:03.560045 data_check-0.9.0/data_check/exceptions.py
+-rw-r--r--   0        0        0     3789 2021-12-17 16:57:40.860301 data_check-0.9.0/data_check/io.py
+-rw-r--r--   0        0        0       49 2021-11-09 05:23:03.560045 data_check-0.9.0/data_check/output/__init__.py
+-rw-r--r--   0        0        0     1666 2021-12-17 16:57:40.860301 data_check-0.9.0/data_check/output/handler.py
+-rw-r--r--   0        0        0     8390 2021-12-17 16:57:40.860301 data_check-0.9.0/data_check/output/output.py
+-rw-r--r--   0        0        0     1106 2021-12-17 16:57:40.860301 data_check-0.9.0/data_check/result.py
+-rw-r--r--   0        0        0     3023 2021-12-17 16:57:40.860301 data_check-0.9.0/data_check/runner.py
+-rw-r--r--   0        0        0       88 2021-11-09 05:23:03.560045 data_check-0.9.0/data_check/sql/__init__.py
+-rw-r--r--   0        0        0      498 2021-11-09 05:23:03.560045 data_check-0.9.0/data_check/sql/load_mode.py
+-rw-r--r--   0        0        0     1671 2021-12-17 16:57:40.860301 data_check-0.9.0/data_check/sql/query_result.py
+-rw-r--r--   0        0        0     4584 2021-12-17 16:57:40.860301 data_check-0.9.0/data_check/sql/sql.py
+-rw-r--r--   0        0        0     7696 2021-12-14 05:12:35.780997 data_check-0.9.0/data_check/sql/table_loader.py
+-rw-r--r--   0        0        0        0 2021-12-17 16:57:40.860301 data_check-0.9.0/data_check/utils/__init__.py
+-rw-r--r--   0        0        0     1438 2021-12-17 16:57:40.860301 data_check-0.9.0/data_check/utils/lookup_loader.py
+-rw-r--r--   0        0        0     1622 2021-12-17 16:57:40.860301 data_check-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     5727 2021-12-17 16:58:22.750687 data_check-0.9.0/setup.py
+-rw-r--r--   0        0        0     6044 2021-12-17 16:58:22.751212 data_check-0.9.0/PKG-INFO
```

### Comparing `data_check-0.8.0/CHANGELOG.md` & `data_check-0.9.0/CHANGELOG.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,34 @@
 # Changelog
 
 ## [Unreleased]
 
+## [0.9.0] - 2021-12-17
+
+### Added
+
+- lookups
+- always_run steps in pipelines
+- print parameter in cmd pipeline step
+- logging in config file and --log argument
+- tests that --sql and sql in a pipeline use templates
+- test for non-ASCII characters in column names
+- '\' as escape character in CSVs
+- --print/--print-json with --verbose prints the output even if it's matching
+
+
+### Removed
+
+- --gen argument (use -g or --generate instead)
+
+### Fixed
+
+- handling pd.NaT
+- --generate escapes '#' in CSV
+- --ping works with --verbose and --traceback
 
 ## [0.8.0] - 2021-10-29
 
 ### Added
 
 - Excel support (for checks and loading tables)
 - --quiet suppresses all output
```

### Comparing `data_check-0.8.0/LICENSE` & `data_check-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `data_check-0.8.0/README.md` & `data_check-0.9.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 # data_check
 
-data_check is a simple data validation tool. In its most basic form it will execute SQL queries and compare the results against CSV files. But there are more advanced features:
+data_check is a simple data validation tool. In its most basic form it will execute SQL queries and compare the results against CSV or Excel files. But there are more advanced features:
 
 ## Features
 
 * [CSV checks](#csv-checks): compare SQL queries against CSV files
+* Excel support: Use Excel (xlsx) instead of CSV
 * multiple environments (databases) in the configuration file
 * populate tables from CSV files
 * execute any SQL files on a database
 * more complex [pipelines](#pipelines)
 * run any script/command (via pipelines)
+* simplified checks for empty datasets
+* lookups to reuse the same data in multiple queries
 
 ## Database support
 
 data_check should work with any database that works with [SQLAlchemy](https://docs.sqlalchemy.org/en/14/dialects/). Currently data_check is tested against PostgreSQL, MySQL, SQLite, Oracle and Microsoft SQL Server.
 
 ## Quickstart
```

### Comparing `data_check-0.8.0/data_check/__main__.py` & `data_check-0.9.0/data_check/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import click
 from pathlib import Path
 import sys
 from colorama import init
 from importlib_metadata import version
-from typing import Union, List, Optional
+from typing import Union, List, Optional, cast
 
 from data_check.data_check import DataCheck
 from data_check.config import DataCheckConfig
 
 
 @click.command()
 @click.option("--connection", "-c", type=str, help="connection to use")
@@ -34,15 +34,14 @@
 )
 @click.option(
     "--print-json",
     is_flag=True,
     help="shortcut for --print --print-format json",
 )
 @click.option(
-    "--gen",
     "--generate",
     "-g",
     "generate_expectations",
     is_flag=True,
     help="generate expectation files if they don't exist",
 )
 @click.option(
@@ -55,26 +54,26 @@
     type=str,
     default=DataCheckConfig.config_path,
     help=f"config file to use (default: {DataCheckConfig.config_path})",
 )
 @click.option(
     "--load",
     type=click.Path(),
-    help=f"load table data from a csv",
+    help="load table data from a csv",
 )
 @click.option(
     "--table",
     type=str,
-    help=f"table name to load data into",
+    help="table name to load data into",
 )
 @click.option(
     "--load-mode",
     type=str,
     default="truncate",
-    help=f"how to load the table: truncate (default), append or replace",
+    help="how to load the table: truncate (default), append or replace",
 )
 @click.option(
     "--load-tables", is_flag=True, help="load tables from a list of csv files"
 )
 @click.option(
     "--sql-file",
     "--sql-files",
@@ -88,15 +87,16 @@
     help="run any SQL statement; print result as CSV if it is a query",
 )
 @click.option("--output", "-o", type=click.Path(), help="output path for --sql")
 @click.option("--ping", is_flag=True, help="tries to connect to the database")
 @click.option("--verbose", is_flag=True, help="print verbose output")
 @click.option("--traceback", is_flag=True, help="print traceback output for debugging")
 @click.option("--quiet", is_flag=True, help="do not print any output")
-@click.version_option(version=version("data-check"))
+@click.option("--log", type=click.Path(), help="write output to a log file")
+@click.version_option(version=cast(str, version("data-check")))
 @click.argument("files", nargs=-1, type=click.Path())
 def main(
     connection: str = "",
     workers: int = DataCheckConfig.parallel_workers,
     print_failed: bool = False,
     print_format: str = DataCheckConfig.default_print_format,
     print_json: bool = False,
@@ -110,14 +110,15 @@
     sql_files: bool = False,
     sql: str = "",
     output: Union[str, Path] = "",
     ping: bool = False,
     verbose: bool = False,
     traceback: bool = False,
     quiet: bool = False,
+    log: Optional[Union[str, Path]] = None,
     files: List[Union[str, Path]] = [],
 ):
     """ FILES: list of checks files or folders"""
 
     if print_json:
         print_failed = True
         print_format = "json"
@@ -125,28 +126,32 @@
     init()  # init colorama
     config = Path(config)
     dc_config = (
         DataCheckConfig(config_path=config).load_config().set_connection(connection)
     )
     dc_config.generate_mode = generate_expectations
     dc_config.force = force
+    if log:
+        dc_config.log_path = Path(log)
 
     if not dc_config.connection:
         click.echo(f"unknown connection: {connection}")
         sys.exit(1)
 
     dc_config.parallel_workers = workers
 
     dc = DataCheck(config=dc_config)
     dc.output.configure_output(
         verbose=verbose,
         traceback=traceback,
         print_failed=print_failed,
         print_format=print_format,
         quiet=quiet,
+        # set log_path from config, so we can also use it from the config file
+        log_path=dc_config.log_path,
     )
 
     if load:
         if not table:
             click.echo("--table must be specified")
             sys.exit(1)
         else:
@@ -160,19 +165,21 @@
         path_list = [Path(f) for f in files]
         dc.sql.table_loader.load_tables_from_files(path_list, load_mode=load_mode)
         sys.exit(0)
 
     dc.load_template()
 
     if sql_files:
+        dc.load_lookups()
         path_list = [Path(f) for f in files]
         dc.run_sql_files(path_list)
         sys.exit(0)
 
     if sql:
+        dc.load_lookups()
         if dc.run_sql_query(sql, output=output):
             sys.exit(0)
         else:
             sys.exit(1)
 
     if not files:
         files = [dc_config.checks_path]  # use default checks path if nothing is given
@@ -181,14 +188,15 @@
     if ping:
         test = dc.sql.test_connection()
         if test:
             sys.exit(0)
         else:
             sys.exit(1)
     else:
+        dc.load_lookups()
         result = dc.run(path_list)
         if not result:
             sys.exit(1)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `data_check-0.8.0/data_check/checks/base_check.py` & `data_check-0.9.0/data_check/checks/path_not_exists.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 from pathlib import Path
 
-from ..result import DataCheckResult
+from .base_check import BaseCheck
+from ..result import DataCheckResult, ResultType
 
 
-class BaseCheck:
-    def __init__(self, data_check, check_path: Path) -> None:
-        self.data_check = data_check
-        self.check_path = check_path  # path to the check (some file or folder)
+class PathNotExists(BaseCheck):
+    """Special "check" that is used when a path/file that should contain a check doesn't exists.
+    Always returns a failing result.
+    """
 
     def run_test(self) -> DataCheckResult:
-        pass
+        return self.data_check.output.prepare_result(
+            ResultType.FAILED_PATH_NOT_EXISTS, source=self.check_path
+        )
 
     @staticmethod
     def is_check_path(path: Path) -> bool:
-        return False
-
-    def __lt__(self, other) -> bool:
-        return self.check_path < other.check_path
-
-    def __repr__(self) -> str:
-        return f"<{self.__class__.__name__} ({self.check_path})>"
+        return not path.exists()
```

### Comparing `data_check-0.8.0/data_check/checks/csv_check.py` & `data_check-0.9.0/data_check/checks/csv_check.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,42 +30,48 @@
             df_merged = sql_result.merge(expect_result, indicator=True, how="outer")
         return df_merged
 
     @staticmethod
     def is_check_path(path: Path):
         return path.suffix.lower() == ".sql"
 
-    @staticmethod
     def get_result(
-        sql_result: pd.DataFrame, expect_result: pd.DataFrame, return_all: bool
+        self, sql_result: pd.DataFrame, expect_result: pd.DataFrame, return_all: bool
     ) -> Tuple[ResultType, pd.DataFrame]:
         # replace missing values and None with pd.NA
         sql_result.fillna(value=pd.NA, inplace=True)
         # using "" instead of r'^$' doesn't work somehow, so we need to use regex
         sql_result.replace(r"^$", pd.NA, regex=True, inplace=True)
+        # replace empty datetime values with empty string
+        sql_result.replace({pd.NaT: pd.NA}, inplace=True)
 
         expect_result.fillna(value=pd.NA, inplace=True)
+        expect_result.replace(r"^$", pd.NA, regex=True, inplace=True)
+        expect_result.replace({pd.NaT: pd.NA}, inplace=True)
 
         df_merged = CSVCheck.merge_results(sql_result, expect_result)
         df_diff = df_merged[df_merged._merge != "both"]
         assert isinstance(df_diff, pd.DataFrame)  # assert a DataFrame, not a Series
+        return_all = return_all or self.data_check.output.verbose
         df_result = df_merged if return_all else df_diff
 
         # empty diff means there are no differences and the test has passed
         passed = len(df_diff) == 0
         if passed and len(sql_result) != len(expect_result):
             return (ResultType.FAILED_DIFFERENT_LENGTH, df_result)
         return (DataCheckResult.passed_to_result_type(passed), df_result)
 
     def read_sql_file(self, sql_file: Path) -> Union[DataCheckResult, QueryResult]:
         try:
             query = read_sql_file(
                 sql_file=sql_file, template_data=self.data_check.template_data
             )
-            return self.data_check.sql.run_query_with_result(query)
+            return self.data_check.sql.run_query_with_result(
+                query, params=self.data_check.sql_params
+            )
         except Exception as exc:
             return self.data_check.output.prepare_result(
                 ResultType.FAILED_WITH_EXCEPTION, source=sql_file, exception=exc
             )
 
     def read_expect_file(
         self, expect_file: Path, string_columns
@@ -106,13 +112,13 @@
         if isinstance(sql_result, DataCheckResult):
             return sql_result
 
         expect_result = self.read_expect_file(expect_file, sql_result.string_columns)
         if isinstance(expect_result, DataCheckResult):
             return expect_result
 
-        result_type, df_result = CSVCheck.get_result(
+        result_type, df_result = self.get_result(
             sql_result.df, expect_result, return_all
         )
         return self.data_check.output.prepare_result(
             result_type, source=sql_file, result=df_result
         )
```

### Comparing `data_check-0.8.0/data_check/checks/empty_set_check.py` & `data_check-0.9.0/data_check/checks/empty_set_check.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,17 @@
         return path.suffix.lower() == ".sql" and path.with_suffix(".empty").exists()
 
     def run_test(self) -> DataCheckResult:
         try:
             query = read_sql_file(
                 sql_file=self.check_path, template_data=self.data_check.template_data
             )
-            sql_result = self.data_check.sql.run_query_with_result(query)
+            sql_result = self.data_check.sql.run_query_with_result(
+                query, params=self.data_check.sql_params
+            )
             if len(sql_result) == 0:
                 return self.data_check.output.prepare_result(
                     ResultType.PASSED, source=self.check_path, result=sql_result.df
                 )
             else:
                 return self.data_check.output.prepare_result(
                     ResultType.FAILED_DIFFERENT_LENGTH, source=self.check_path
```

### Comparing `data_check-0.8.0/data_check/checks/excel_check.py` & `data_check-0.9.0/data_check/checks/excel_check.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from pathlib import Path
 import pandas as pd
-from typing import Union
+from typing import Union, List, cast
 
 from .csv_check import CSVCheck
 from ..result import DataCheckResult, ResultType
 
 
 class ExcelCheck(CSVCheck):
     @staticmethod
@@ -24,18 +24,22 @@
                     _col = column.apply(self.clean_string_column)
                     df[column_name] = _col
             except Exception:
                 pass
         return df
 
     def read_expect_file(
-        self, expect_file: Path, string_columns
+        self, expect_file: Path, string_columns: List[str]
     ) -> Union[DataCheckResult, pd.DataFrame]:
         try:
-            expect_result = pd.read_excel(
-                expect_file, sheet_name=0, header=0, engine="openpyxl", dtype="object"
+            expect_result: pd.DataFrame = pd.read_excel(
+                cast(str, expect_file),
+                sheet_name=0,
+                header=0,
+                engine="openpyxl",
+                dtype="object",
             )
             return self.clean_excel_df(expect_result)
         except Exception as exc_csv:
             return self.data_check.output.prepare_result(
                 ResultType.FAILED_WITH_EXCEPTION, source=expect_file, exception=exc_csv
             )
```

### Comparing `data_check-0.8.0/data_check/checks/generator.py` & `data_check-0.9.0/data_check/checks/generator.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from pathlib import Path
 from typing import Dict, Any
 
 from .base_check import BaseCheck
 
-from ..io import get_expect_file, read_sql_file, rel_path
+from ..io import get_expect_file, read_sql_file, rel_path, write_csv
 from ..result import DataCheckResult
 
 
 class DataCheckGenerator(BaseCheck):
     """Special type of a "check" to generate the expectation files."""
 
     def gen_expectation(
@@ -17,17 +17,18 @@
         Executes the query for a data_check test
         and stores the result in the csv file.
         """
         expect_result = get_expect_file(sql_file)
         _rel_path = rel_path(expect_result)
         if not expect_result.exists() or force:
             result = self.data_check.sql.run_query(
-                read_sql_file(sql_file=sql_file, template_data=template_data)
+                read_sql_file(sql_file=sql_file, template_data=template_data),
+                params=self.data_check.sql_params,
             )
-            result.to_csv(expect_result, index=False)
+            write_csv(result, expect_result)
             output = f"expectation written to {_rel_path}"
         else:
             output = f"expectation skipped for {_rel_path}"
         return DataCheckResult(True, output, output)
 
     def run_test(self) -> DataCheckResult:
         return self.gen_expectation(
```

### Comparing `data_check-0.8.0/data_check/checks/pipeline_check/cmd_step.py` & `data_check-0.9.0/data_check/checks/pipeline_check/cmd_step.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,35 @@
 from pathlib import Path
-from typing import List, Union
+from typing import List, Union, TYPE_CHECKING
 import subprocess
 
+if TYPE_CHECKING:
+    from data_check.output import DataCheckOutput
+
 
 class CmdStep:
-    def __init__(self, cmd: Union[str, List[str]], output) -> None:
+    def __init__(
+        self, cmd: Union[str, List[str]], output: "DataCheckOutput", print: bool = True
+    ) -> None:
         self.cmd = cmd
         self.output = output
+        self.print = print
 
     def _run_cmd(self, cmd: str, base_path: Path = Path(".")):
         self.output.print(f"# {cmd}")
         process = subprocess.Popen(
             cmd,
             stdout=subprocess.PIPE,
             stderr=subprocess.STDOUT,
             cwd=base_path,
             shell=True,
         )
         assert process.stdout is not None
         with process.stdout:
-            self.output.handle_subprocess_output(process.stdout)
+            self.output.handle_subprocess_output(process.stdout, print=self.print)
         exitcode = process.wait()
         return exitcode == 0
 
     def run(self, base_path: Path = Path(".")):
         if isinstance(self.cmd, List):
             for c in self.cmd:
                 if not self._run_cmd(c, base_path=base_path):
```

### Comparing `data_check-0.8.0/data_check/checks/pipeline_check/pipeline_check.py` & `data_check-0.9.0/data_check/checks/pipeline_check/pipeline_check.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 from pathlib import Path
-from typing import Callable, List, Dict, Any, Union, Optional
+from typing import Callable, List, Dict, Any, Union, Optional, TYPE_CHECKING, cast
 from copy import deepcopy
 import inspect
 from functools import partial
 
 from ..base_check import BaseCheck
 from ...result import DataCheckResult
 from ...io import read_yaml
 from .serial_pipeline_steps import SerialPipelineSteps
 from .cmd_step import CmdStep
 
+if TYPE_CHECKING:
+    from data_check import DataCheck
+
 DATA_CHECK_PIPELINE_FILE = "data_check_pipeline.yml"
 
 
 class PipelineCheck(BaseCheck):
-    def __init__(self, data_check, check_path: Path) -> None:
+    def __init__(self, data_check: "DataCheck", check_path: Path) -> None:
         super().__init__(data_check, check_path)
-        self.pipeline_steps = {}
+        self.pipeline_steps: Dict[str, Dict[str, Any]] = {}
         self.register_pipelines()
 
     def register_pipelines(self):
         self.register_pipeline_step(
             "load_tables",
             self.data_check.sql.table_loader.load_tables_from_files,
             convert_to_path_list=["files"],
@@ -40,14 +43,15 @@
         self.register_pipeline_step(
             "sql_file", self.data_check.run_sql_files, convert_to_path_list=["files"]
         )
         pipeline_run_sql_query = partial(
             self.data_check.run_sql_query, print_query=True
         )
         self.register_pipeline_step("sql", pipeline_run_sql_query)
+        self.register_pipeline_step("always_run", self.always_run)
 
     @staticmethod
     def is_check_path(path: Path) -> bool:
         return path.is_dir() and (path / DATA_CHECK_PIPELINE_FILE).exists()
 
     def register_pipeline_step(
         self,
@@ -58,15 +62,15 @@
     ):
         self.pipeline_steps[step_name] = {
             "method": method,
             "convert_to_path_list": convert_to_path_list,
             "convert_to_path": convert_to_path,
         }
 
-    def get_pipeline_method(self, step_name):
+    def get_pipeline_method(self, step_name: str) -> Optional[Callable[..., Any]]:
         return self.pipeline_steps.get(step_name, {}).get("method", None)
 
     def _parse_pipeline_file(self, pipeline_file: Path) -> Dict[str, Any]:
         if pipeline_file.exists():
             yaml = read_yaml(
                 pipeline_file,
                 template_data=dict(
@@ -92,22 +96,37 @@
             self,
             steps,
             self.check_path,
             pipeline_name=str(self.check_path),
         )
         return serial_steps.run()
 
-    def run_cmd(self, commands: List[str], base_path: Path = Path(".")):
-        c = CmdStep(commands, self.data_check.output)
+    def run_cmd(
+        self, commands: List[str], print: bool = True, base_path: Path = Path(".")
+    ):
+        c = CmdStep(commands, self.data_check.output, print=print)
         return c.run(base_path=base_path)
 
+    def always_run(self, steps: List[Any]) -> DataCheckResult:
+        serial_steps = SerialPipelineSteps(
+            self.data_check,
+            self,
+            steps,
+            self.check_path,
+            pipeline_name=str(self.check_path),
+        )
+        # Also return the result of the run,
+        # so that if all steps pass,
+        # the overall result will be also passed.
+        return serial_steps.run()
+
     def template_parameters(self, pipeline_path: Path) -> Dict[str, str]:
         return {
-            "CONNECTION": self.data_check.config.connection_name,
-            "CONNECTION_STRING": self.data_check.config.connection,
+            "CONNECTION": cast(str, self.data_check.config.connection_name),
+            "CONNECTION_STRING": cast(str, self.data_check.config.connection),
             "PIPELINE_PATH": str(pipeline_path.absolute()),
             "PIPELINE_NAME": str(pipeline_path.name),
             "PROJECT_PATH": str(self.data_check.config.project_path),
         }
 
     def get_prepared_parameters(
         self, method: str, params: Union[str, List[str], Dict[str, Any]]
```

### Comparing `data_check-0.8.0/data_check/checks/pipeline_check/serial_pipeline_steps.py` & `data_check-0.9.0/data_check/checks/pipeline_check/serial_pipeline_steps.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,59 +1,73 @@
 from pathlib import Path
-from typing import List, Dict, Any
+from typing import List, Dict, Any, TYPE_CHECKING
 import inspect
 
 from ...result import DataCheckResult, ResultType
 
+if TYPE_CHECKING:
+    from data_check import DataCheck
+    from data_check.checks import PipelineCheck
+
 
 class SerialPipelineSteps:
     def __init__(
         self,
-        data_check,
-        pipeline_check,
+        data_check: "DataCheck",
+        pipeline_check: "PipelineCheck",
         steps: List[Any],
         path: Path,
         pipeline_name: str,
     ) -> None:
         self.data_check = data_check
         self.pipeline_check = pipeline_check
         self.path = path
         self.steps = steps
         self.pipeline_name = pipeline_name
+        self.processed_step_indices: List[int] = []
 
     def run(self) -> DataCheckResult:
-        for step in self.steps:
+        for idx, step in enumerate(self.steps):
             try:
-                result = self.run_pipeline_step(self.path, step)
+                result = self.run_pipeline_step(self.path, step, idx)
                 if not result:
+                    self.process_always_run()
                     result_msg = (
                         f"pipeline {self.pipeline_name}: "
                         f"{self.data_check.output.failed_message}"
                     )
                     return DataCheckResult(
                         passed=False,
                         result=result,
                         message=result_msg,
                     )
             except Exception as e:
+                self.process_always_run()
                 return self.data_check.output.prepare_result(
                     result_type=ResultType.FAILED_WITH_EXCEPTION,
                     source=self.path,
                     exception=e,
                 )
 
         return DataCheckResult(
             passed=True,
             result=(
                 f"pipeline {self.pipeline_name}: "
                 f"{self.data_check.output.passed_message}"
             ),
         )
 
-    def run_pipeline_step(self, path: Path, step: Dict[str, Any]):
+    def process_always_run(self):
+        for idx, step in enumerate(self.steps):
+            if idx not in self.processed_step_indices:
+                # just run the step but ignore any result or output
+                self.run_pipeline_step(self.path, step, idx)
+
+    def run_pipeline_step(self, path: Path, step: Dict[str, Any], idx: int):
+        self.processed_step_indices.append(idx)
         step_type = next(iter(step.keys()))
         params = next(iter(step.values()))
         call_method = self.pipeline_check.get_pipeline_method(step_type)
         if call_method:
             prepared_params = self.pipeline_check.get_prepared_parameters(
                 step_type, params
             )
```

### Comparing `data_check-0.8.0/data_check/config.py` & `data_check-0.9.0/data_check/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from pathlib import Path
 from .io import read_yaml
 from typing import Optional, Dict, Any, Tuple
 
 
 TEMPLATE_FILE = "template.yml"
 CHECKS_PATH = "checks"
+LOOKUPS_PATH = "lookups"
 
 
 class DataCheckConfig:
     config_path = Path("data_check.yml")
 
     parallel_workers = 4
 
@@ -23,14 +24,15 @@
             self.config_path = config_path
 
         self.project_path = Path(".").absolute()
         self.base_path = Path(".").absolute()
 
         self.generate_mode = False
         self.force = False
+        self.log_path: Optional[Path] = None
 
     @property
     def print_overall_result(self):
         """When to print the overall result on console."""
         return not self.generate_mode
 
     @property
@@ -47,38 +49,44 @@
         else:
             return self.base_path
 
     @property
     def template_path(self) -> Path:
         return self.project_path / CHECKS_PATH / TEMPLATE_FILE
 
+    @property
+    def lookups_path(self) -> Path:
+        return self.project_path / LOOKUPS_PATH
+
     def find_config(self, base_path: Path) -> Path:
         abs_base_path = base_path.absolute()
         config_path = abs_base_path / self.config_path
         if not config_path.exists():
             if abs_base_path.parent == abs_base_path:
                 raise Exception(f"could not find {self.config_path} in {abs_base_path}")
             return self.find_config(abs_base_path.parent)
         return abs_base_path / self.config_path
 
-    def load_config(self, base_path=Path(".")):
+    def load_config(self, base_path: Path = Path(".")):
         try:
             config_path = self.find_config(base_path)
         except Exception:
             # raise basically the same exception as in find_config
             # but with base_path for better debugging
             raise Exception(
                 f"could not find {self.config_path} in {base_path.absolute()}"
             )
 
         # project_path is always the directory where the config file is stored
         self.project_path = config_path.parent
         self.base_path = base_path.absolute()
         self.config_path = config_path
         self.config = read_yaml(config_path)
+        _log_path = self.config.get("log", None)
+        self.log_path = Path(_log_path) if _log_path else None
         return self
 
     def set_connection(self, connection: str):
         self.connection, self.connection_name = self.select_connection(connection)
         return self
 
     def select_connection(self, connection: str) -> Tuple[str, str]:
```

### Comparing `data_check-0.8.0/data_check/data_check.py` & `data_check-0.9.0/data_check/data_check.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,31 +13,39 @@
     DataCheckGenerator,
     CSVCheck,
     PipelineCheck,
     EmptySetCheck,
     ExcelCheck,
     PathNotExists,
 )
+from .utils.lookup_loader import load_lookups_from_path
 
 
 class DataCheck:
     """
     Main class for data_check.
     """
 
     def __init__(self, config: Optional[DataCheckConfig] = None):
         if config is None:
             config = DataCheckConfig()
         self.config = config
         self.output = DataCheckOutput()
         self.runner = DataCheckRunner(config.parallel_workers, output=self.output)
+        if not isinstance(config.connection, str):
+            raise Exception("connection is not initialized")
         self.sql = DataCheckSql(
             connection=config.connection, runner=self.runner, output=self.output
         )
         self.template_data: Dict[str, Any] = {}
+        self.lookup_data: Dict[str, Any] = {}
+
+    @property
+    def sql_params(self) -> Dict[str, Any]:
+        return self.lookup_data
 
     def load_template(self):
         if self.config.template_path.exists():
             self.template_data = read_yaml(self.config.template_path)
 
     def delegate_test(self, check: BaseCheck) -> DataCheckResult:
         return check.run_test()
@@ -59,15 +67,15 @@
         else:
             return None
 
     def collect_checks(
         self, files: List[Path], base_path: Path = Path(".")
     ) -> List[BaseCheck]:
         base_path = base_path.absolute()
-        checks = []
+        checks: List[BaseCheck] = []
         for f in sorted(files):
             abs_file = f if f.is_absolute() else base_path / f
             check = self.get_check(abs_file)
             if check is not None:
                 checks.append(check)
             elif abs_file.is_dir():
                 dir_files = [d for d in abs_file.iterdir()]
@@ -100,13 +108,16 @@
         )
 
     def run_sql_query(
         self,
         query: str,
         output: Union[str, Path] = "",
         base_path: Path = Path("."),
-        print_query=False,
+        print_query: bool = False,
     ):
         sql_query = parse_template(query, template_data=self.template_data)
         if print_query:
             self.output.print(f"-- {sql_query}")
         return self.sql.run_sql(sql_query, output, base_path)
+
+    def load_lookups(self):
+        self.lookup_data.update(load_lookups_from_path(self))
```

### Comparing `data_check-0.8.0/data_check/date.py` & `data_check-0.9.0/data_check/date.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-from typing import List, Tuple
+from typing import List, Tuple, Union
 import pandas as pd
 from dateutil.parser import isoparse as _isoparse
 import math
 
 
 def parse_date_columns(df: pd.DataFrame) -> Tuple[List[str], pd.DataFrame]:
     """Tries to parse each column as a date.
     Returns a tuple with the list of the column names that were parsed as dates
     and the DataFrame with these columns replaced as datetime.
     """
-    _date_columns = []
+    _date_columns: List[str] = []
     for column_name, column in df.items():
         # only try to convert, if some values exist in the column
         if not column.isna().all():
             try:
                 _col = column.apply(isoparse, convert_dtype=False)
                 df[column_name] = _col
                 _date_columns.append(str(column_name))
             except Exception:
                 pass
     return _date_columns, df
 
 
-def isoparse(column):
+def isoparse(column: Union[int, float, str, None]):
     if isinstance(column, float) and math.isnan(column):
         column = ""
     if column is None or len(str(column)) == 0:
         return ""
     if len(str(column)) < 10 or not isinstance(column, str):
         # must be at least of format YYYY-MM-DD to be a date
         raise ValueError(("VE", column, type(column)))
```

### Comparing `data_check-0.8.0/data_check/io.py` & `data_check-0.9.0/data_check/io.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Dict, Any, Union, Optional
+from typing import List, Dict, Any, Union, Optional, cast
 from pathlib import Path
 from jinja2 import Template
 import pandas as pd
 from pandas.core.frame import DataFrame
 import yaml
 
 from .date import isoparse, parse_date_columns
@@ -77,14 +77,15 @@
         parse_dates = False
     dtypes = {s: "object" for s in string_columns}
     df = pd.read_csv(
         csv_file,
         na_values=[""],  # use empty string as nan
         keep_default_na=False,
         comment="#",
+        escapechar="\\",
         quotechar='"',
         quoting=0,
         engine="c",
         parse_dates=parse_dates,
         date_parser=isoparse,
         dtype=dtypes,
     )
@@ -97,15 +98,19 @@
     print_method(df.to_csv(index=False))
 
 
 def write_csv(
     df: DataFrame, output: Union[str, Path] = "", base_path: Path = Path(".")
 ):
     if output:
-        df.to_csv(base_path / output, index=False)
+        result = df.to_csv(index=False)
+        result = cast(str, result)
+        # escape # in strings that would otherwise be treated as the start of a comment
+        result = result.replace("#", "\\#")
+        Path(base_path / output).write_text(result)
 
 
 def read_yaml(
     yaml_file: Path,
     encoding: str = "UTF-8",
     template_data: Optional[Dict[str, Any]] = None,
 ):
```

### Comparing `data_check-0.8.0/data_check/output/handler.py` & `data_check-0.9.0/data_check/output/handler.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,44 +1,50 @@
 import multiprocessing
-from typing import Any
+from typing import IO, Any, Optional
 import os
 import locale
+from pathlib import Path
+import datetime
 
 
 class OutputHandler:
     """
     Handles the output for data_check.
     """
 
     def __init__(self, quiet: bool):
         self.quiet = quiet
         self.encoding = locale.getpreferredencoding(False)
+        self.log_path: Optional[Path] = None
 
     @property
     def is_main(self):
         return multiprocessing.current_process().name == "MainProcess"
 
     def write_log(self, msg: str):
-        pass
+        if self.log_path:
+            with self.log_path.open("a") as log:
+                s_log = f"{datetime.datetime.now()}: {msg}{os.linesep}"
+                log.write(s_log)
 
-    def print(self, msg: Any, prefix: str = ""):
+    def print(self, msg: Any, prefix: str = "", _print: bool = True):
         if prefix:
             msg = f"{prefix}: {str(msg)}"
         else:
             msg = str(msg)
-        if not self.quiet:
+        if not self.quiet and _print:
             print(msg)
         self.write_log(msg)
 
-    def log(self, msg: Any, prefix: str = "", level="INFO"):
+    def log(self, msg: Any, prefix: str = "", level: str = "INFO"):
         if not self.is_main:
             prefix = f"{prefix}@{multiprocessing.current_process().name}"
         self.print(f"{level}: {str(msg)}", prefix=prefix)
 
-    def handle_subprocess_output(self, pipe):
+    def handle_subprocess_output(self, pipe: IO[bytes], print: bool = True):
         for line in iter(pipe.readline, b""):
             try:
                 # try printing the line with the system encoding
-                self.print(line.decode(self.encoding).rstrip(os.linesep))
+                self.print(line.decode(self.encoding).rstrip(os.linesep), _print=print)
             except Exception:
                 # if this doesn't help, print the raw bytes without the b''
-                self.print(str(line)[2:-1].rstrip(os.linesep))
+                self.print(str(line)[2:-1].rstrip(os.linesep), _print=print)
```

### Comparing `data_check-0.8.0/data_check/output/output.py` & `data_check-0.9.0/data_check/output/output.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from pathlib import Path
 import pandas as pd
 from colorama import Fore, Style
 import traceback
 from os import linesep
-from typing import Optional, Any
+from typing import IO, Optional, Any, Tuple, Union, List, cast
 
 from ..exceptions import DataCheckException
 from ..result import DataCheckResult, ResultType
 from ..io import rel_path
 from .handler import OutputHandler
 
 
@@ -15,39 +15,55 @@
     def __init__(self):
         self.verbose = False
         self.traceback = False
         self.print_failed = False
         self.print_format = "pandas"
         self.quiet = False
         self.handler = OutputHandler(self.quiet)
+        self.log_path = None
 
     def configure_output(
         self,
         verbose: bool,
         traceback: bool,
         print_failed: bool,
         print_format: str,
         quiet: bool = False,
+        log_path: Optional[Path] = None,
     ):
         self.verbose = verbose
         self.traceback = traceback
         self.print_failed = print_failed
         self.print_format = print_format
         self.quiet = quiet
+        self.log_path = log_path
 
         self.handler.quiet = quiet
+        self.handler.log_path = log_path
+
+    def print_exception(self, exc: Exception):
+        if self.traceback:
+            self.print(
+                "".join(
+                    traceback.format_exception(
+                        value=exc, tb=exc.__traceback__, etype=Exception
+                    )
+                )
+            )
+        elif self.verbose:
+            self.print(str(exc))
 
     def print(self, msg: Any, prefix: str = ""):
         self.handler.print(msg, prefix)
 
-    def log(self, msg: Any, prefix: str = "", level="INFO"):
+    def log(self, msg: Any, prefix: str = "", level: str = "INFO"):
         self.handler.log(msg, prefix, level)
 
-    def handle_subprocess_output(self, pipe):
-        self.handler.handle_subprocess_output(pipe)
+    def handle_subprocess_output(self, pipe: IO[bytes], print: bool = True):
+        self.handler.handle_subprocess_output(pipe, print=print)
 
     def pprint_overall_result(self, passed: bool) -> None:
         overall_result_msg = self.passed_message if passed else self.failed_message
         # print newline to separate other results from the overall result message
         self.print("")
         self.print(f"overall result: {overall_result_msg}")
 
@@ -96,50 +112,74 @@
     def failed_message(self) -> str:
         return self.str_fail("FAILED")
 
     def prepare_result(
         self,
         result_type: ResultType,
         source: Path,
-        result: Optional[pd.DataFrame] = None,
+        result: Union[pd.DataFrame, List[Tuple[str, pd.DataFrame]], None] = None,
         exception: Optional[Exception] = None,
     ) -> DataCheckResult:
         passed = DataCheckResult.result_type_passed(result_type)
         # always print path relative to where data_check is started
         rel_source = rel_path(source)
         if result_type == ResultType.PASSED:
-            assert isinstance(result, pd.DataFrame)
-            return self._passed_result(passed, rel_source, result)
+            return self._passed_result(passed, rel_source, cast(pd.DataFrame, result))
         elif result_type == ResultType.FAILED:
-            assert isinstance(result, pd.DataFrame)
-            return self._failed_result(passed, rel_source, result)
+            return self._failed_result(passed, rel_source, cast(pd.DataFrame, result))
+        elif result_type == ResultType.FAILED_WITH_MULTIPLE_FAILURES:
+            return self._failed_result_multiple_failures(
+                passed, rel_source, cast(List[Tuple[str, pd.DataFrame]], result)
+            )
         elif result_type == ResultType.NO_EXPECTED_RESULTS_FILE:
             return self._no_expected_file_result(passed, rel_source)
         elif result_type == ResultType.FAILED_WITH_EXCEPTION:
-            assert isinstance(exception, Exception)
-            return self._failed_with_exception_result(passed, rel_source, exception)
+            return self._failed_with_exception_result(
+                passed, rel_source, cast(Exception, exception)
+            )
         elif result_type == ResultType.FAILED_DIFFERENT_LENGTH:
             return self._failed_result_different_length(passed, rel_source)
         elif result_type == ResultType.FAILED_PATH_NOT_EXISTS:
             return self._failed_path_not_exists(passed, rel_source)
+        else:
+            raise Exception(f"unknown ResultType: {result_type}")
 
     def _passed_result(
         self, passed: bool, source: Path, result: pd.DataFrame
     ) -> DataCheckResult:
         message = f"{source}: {self.passed_message}"
+        if self.print_failed and self.verbose:
+            message += linesep + self.pprint_failed(result.copy())
         return DataCheckResult(passed=passed, result=result, message=message)
 
     def _failed_result(
         self, passed: bool, source: Path, result: pd.DataFrame
     ) -> DataCheckResult:
         message = f"{source}: {self.failed_message}"
         if self.print_failed:
             message += linesep + self.pprint_failed(result.copy())
         return DataCheckResult(passed=passed, result=result, message=message)
 
+    def _failed_result_multiple_failures(
+        self, passed: bool, source: Path, result: List[Tuple[str, pd.DataFrame]]
+    ) -> DataCheckResult:
+        message = f"{source}: {self.failed_message}"
+        failure_message = ""
+        for failure in result:
+            failure_message += (
+                linesep
+                + failure[0]
+                + ":"
+                + linesep
+                + self.pprint_failed(failure[1].copy())
+            )
+        if self.print_failed:
+            message += failure_message
+        return DataCheckResult(passed=passed, result=failure_message, message=message)
+
     def _failed_result_different_length(
         self, passed: bool, source: Path
     ) -> DataCheckResult:
         message = f"{source}: {self.failed_message}"
         result = "same data but the length differs"
         if self.print_failed:
             message += linesep + result
@@ -158,15 +198,19 @@
         self, passed: bool, source: Path, exception: Exception
     ):
         fail = self.str_fail(f"FAILED (with exception in {source})")
         message = f"{source}: {fail}"
         if self.verbose:
             message += linesep + str(exception)
         if self.traceback:
-            message += linesep + traceback.format_exc()
+            message += linesep + "".join(
+                traceback.format_exception(
+                    value=exception, tb=exception.__traceback__, etype=Exception
+                )
+            )
         return DataCheckResult(
             passed=passed,
             result=f"{source} generated an exception: {exception}",
             message=message,
         )
 
     def _failed_path_not_exists(self, passed: bool, source: Path) -> DataCheckResult:
```

### Comparing `data_check-0.8.0/data_check/result.py` & `data_check-0.9.0/data_check/result.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 class ResultType(Enum):
     PASSED = 1
     FAILED = 2
     FAILED_WITH_EXCEPTION = 3
     NO_EXPECTED_RESULTS_FILE = 4
     FAILED_DIFFERENT_LENGTH = 5
     FAILED_PATH_NOT_EXISTS = 6
+    FAILED_WITH_MULTIPLE_FAILURES = 7
 
 
 class DataCheckResult:
     """
     Wrapper class holding the result of a test run.
     """
```

### Comparing `data_check-0.8.0/data_check/runner.py` & `data_check-0.9.0/data_check/runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import concurrent.futures
 from typing import Callable, List, Any, Dict, Optional
-from pathlib import Path
 
 from .checks.base_check import BaseCheck
 from .result import DataCheckResult
 from .output import DataCheckOutput
 
 
 class DataCheckRunner:
```

### Comparing `data_check-0.8.0/data_check/sql/query_result.py` & `data_check-0.9.0/data_check/sql/query_result.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,47 +1,46 @@
 import pandas as pd
-from typing import List, Optional
+from typing import List, Optional, cast
 from pandas.api.types import is_string_dtype
+from sqlalchemy.engine.cursor import CursorResult
+from sqlalchemy.engine.row import Row
 
 from ..date import parse_date_columns
 
 
 class QueryResult:
-    def __init__(self, query: str, result):
+    def __init__(self, query: str, result: CursorResult):
         self.query = query
         self.result = result
-        self._data = None
+        self._data: Optional[List[Row]] = None
         self._df: Optional[pd.DataFrame] = None
         self._date_columns: List[str] = []
 
     @property
-    def data(self):
+    def data(self) -> List[Row]:
         if self._data is None:
-            self._data = self.result.fetchall()
+            self._data = cast(List[Row], self.result.fetchall())
         return self._data
 
     @property
     def columns(self) -> List[str]:
-        return self.result.keys()
+        return cast(List[str], self.result.keys())
 
     @property
     def date_columns(self) -> List[str]:
         if self._df is None:
             self._load_df()
         return self._date_columns
 
     @property
     def string_columns(self) -> List[str]:
-        if self._df is None:
-            self._load_df()
-        assert isinstance(self._df, pd.DataFrame)
         return [
             k
-            for k in self._df.keys()
-            if is_string_dtype(self._df[k]) and k not in self.date_columns
+            for k in cast(List[str], self.df.keys())
+            if is_string_dtype(self.df[k]) and k not in self.date_columns
         ]
 
     def _load_df(self):
         # use coerce_float=True as it is used in pandas by default
         frame = pd.DataFrame.from_records(
             self.data, columns=self.columns, coerce_float=True
         )
@@ -49,12 +48,11 @@
         self._date_columns = date_cols
         self._df = df
 
     @property
     def df(self) -> pd.DataFrame:
         if self._df is None:
             self._load_df()
-        assert isinstance(self._df, pd.DataFrame)
-        return self._df
+        return cast(pd.DataFrame, self._df)
 
     def __len__(self):
         return len(self.df)
```

### Comparing `data_check-0.8.0/data_check/sql/sql.py` & `data_check-0.9.0/data_check/sql/sql.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,15 @@
-from typing import Dict, Any, Optional, Union
+from typing import Dict, Any, Optional, Union, List
 from os import path
 from sqlalchemy import create_engine
 from sqlalchemy.engine import Engine, Connection
+from sqlalchemy.engine.row import Row
+from sqlalchemy.engine.cursor import CursorResult
 from sqlalchemy.sql import text
+from sqlalchemy.sql.expression import bindparam
 import pandas as pd
 from pathlib import Path
 
 
 from ..exceptions import DataCheckException
 from ..output import DataCheckOutput
 from ..io import print_csv, write_csv
@@ -80,48 +83,56 @@
                 return _connection
         return self.__connection
 
     @property
     def dialect(self) -> str:
         return self.get_connection().dialect.name
 
-    def run_query(self, query: str) -> pd.DataFrame:
+    def run_query(self, query: str, params: Dict[str, Any] = {}) -> pd.DataFrame:
         """
         Run a query on the database and return a Pandas DataFrame with the result.
         """
-        return self.run_query_with_result(query).df
+        return self.run_query_with_result(query, params=params).df
 
-    def run_query_with_result(self, query: str) -> QueryResult:
+    def run_query_with_result(
+        self, query: str, params: Dict[str, Any] = {}
+    ) -> QueryResult:
         if not self.connection:
             raise DataCheckException(f"undefined connection: {self.connection}")
-        result = QueryResult(query, self.get_connection().execute(text(query)))
+        sql = text(query)
+        for bp in sql._bindparams.keys():
+            sql = sql.bindparams(bindparam(bp, expanding=True))
+
+        result = QueryResult(query, self.get_connection().execute(sql, **params))
         return result
 
     def test_connection(self) -> bool:
         """
         Returns True if we can connect to the database.
         Mainly for integration tests.
         """
         engine = self.get_engine(extra_params={"pool_pre_ping": True})
         try:
             engine.connect()
             self.output.print("connecting succeeded")
             return True
-        except:  # noqa E722
+        except Exception as e:  # noqa E722
+            self.output.print_exception(e)
             self.output.print("connecting failed")
             return False
 
     def run_sql(
         self, query: str, output: Union[str, Path] = "", base_path: Path = Path(".")
     ):
         sq_text = text(query)
-        result = self.get_connection().execute(
+        result: CursorResult = self.get_connection().execute(
             sq_text.execution_options(autocommit=True)
         )
         try:
-            res = result.fetchall()
-            df = pd.DataFrame(data=res, columns=result.keys())
+            res: List[Row] = result.fetchall()
+            columns: List[str] = result.keys()
+            df = pd.DataFrame(data=res, columns=columns)
             print_csv(df, self.output.print)
             write_csv(df, output=output, base_path=base_path)
             return res
-        except:
+        except Exception:
             return bool(result)
```

### Comparing `data_check-0.8.0/data_check/sql/table_loader.py` & `data_check-0.9.0/data_check/sql/table_loader.py`

 * *Files identical despite different names*

### Comparing `data_check-0.8.0/pyproject.toml` & `data_check-0.9.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "data_check"
-version = "0.8.0"
+version = "0.9.0"
 description = "simple data validation"
 authors = ["Andreas Rjasanow <andrjas@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://andrjas.github.io/data_check/"
 repository = "https://github.com/andrjas/data_check"
 keywords = ["data", "validation", "testing", "quality"]
@@ -19,17 +19,17 @@
         "Topic :: Software Development :: Testing",
     ]
 include = ["CHANGELOG.md", "LICENSE"]
 
 [tool.poetry.dependencies]
 python = "^3.6.2"
 SQLAlchemy = "^1.4"
-pandas = "^1.1.5"
+pandas = "^1.1.5,<1.2"
 pyyaml = "^5.3.1"
-numpy = "^1.19.5"
+numpy = "^1.19.5,<1.20"
 click = "^7.1.2"
 colorama = "^0.4.4"
 importlib-metadata = "^3.4.0"
 Jinja2 = "^2.11.3"
 
 psycopg2-binary = { version = "^2.8.6", optional = true }
 cx_Oracle = { version = "^8.1.0", optional = true}
```

### Comparing `data_check-0.8.0/setup.py` & `data_check-0.9.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,45 +2,46 @@
 from setuptools import setup
 
 packages = \
 ['data_check',
  'data_check.checks',
  'data_check.checks.pipeline_check',
  'data_check.output',
- 'data_check.sql']
+ 'data_check.sql',
+ 'data_check.utils']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['Jinja2>=2.11.3,<3.0.0',
  'SQLAlchemy>=1.4,<2.0',
  'click>=7.1.2,<8.0.0',
  'colorama>=0.4.4,<0.5.0',
  'importlib-metadata>=3.4.0,<4.0.0',
- 'numpy>=1.19.5,<2.0.0',
+ 'numpy>=1.19.5,<1.20',
  'openpyxl>=3.0.9,<4.0.0',
- 'pandas>=1.1.5,<2.0.0',
+ 'pandas>=1.1.5,<1.2',
  'python-dateutil>=2.8.2,<3.0.0',
  'pyyaml>=5.3.1,<6.0.0']
 
 extras_require = \
 {'mssql': ['pyodbc>=4.0.30,<5.0.0'],
  'mysql': ['pymysql[rsa]'],
  'oracle': ['cx_Oracle>=8.1.0,<9.0.0'],
  'postgres': ['psycopg2-binary>=2.8.6,<3.0.0']}
 
 entry_points = \
 {'console_scripts': ['data_check = data_check.__main__:main']}
 
 setup_kwargs = {
     'name': 'data-check',
-    'version': '0.8.0',
+    'version': '0.9.0',
     'description': 'simple data validation',
-    'long_description': '# data_check\n\ndata_check is a simple data validation tool. In its most basic form it will execute SQL queries and compare the results against CSV files. But there are more advanced features:\n\n## Features\n\n* [CSV checks](#csv-checks): compare SQL queries against CSV files\n* multiple environments (databases) in the configuration file\n* populate tables from CSV files\n* execute any SQL files on a database\n* more complex [pipelines](#pipelines)\n* run any script/command (via pipelines)\n\n## Database support\n\ndata_check should work with any database that works with [SQLAlchemy](https://docs.sqlalchemy.org/en/14/dialects/). Currently data_check is tested against PostgreSQL, MySQL, SQLite, Oracle and Microsoft SQL Server.\n\n## Quickstart\n\nYou need Python 3.6.2 or above to run data_check. The easiest way to install data_check is via [pipx](https://github.com/pipxproject/pipx):\n\n`pipx install data-check`\n\nThe data_check Git repository is also a sample data_check project. Clone the repository, switch to the folder and run data_check:\n\n```\ngit clone git@github.com:andrjas/data_check.git\ncd data_check\ndata_check\n```\n\nThis will run the tests in the _checks_ folder using the default connection as set in data_check.yml.\n\nSee the [documentation](https://andrjas.github.io/data_check) how to install data_check in different environments with additional database drivers and other usages of data_check.\n\n## Project layout\n\ndata_check has a simple layout for projects: a single configuration file and a folder with the test files. You can also organize the test files in subfolders.\n\n    data_check.yml    # The configuration file\n    checks/           # Default folder for data tests\n        some_test.sql # SQL file with the query to run against the database\n        some_test.csv # CSV file with the expected result\n        subfolder/    # Tests can be nested in subfolders\n\n## CSV checks\n\nThis is the default mode when running data_check. data_check expects a SQL file and a CSV file. The SQL file will be executed against the database and the result is compared with the CSV file. If they match, the test is passed, otherwise it fails.\n\n## Pipelines\n\nIf data_check finds a file named _data\\_check\\_pipeline.yml_ in a folder, it will treat this folder as a pipeline check. Instead of running [CSV checks](#csv-checks) it will execute the steps in the YAML file.\n\nExample project with a pipeline:\n\n    data_check.yml\n    checks/\n        some_test.sql                # this test will run in parallel to the pipeline test\n        some_test.csv\n        sample_pipeline/\n            data_check_pipeline.yml  # configuration for the pipeline\n            data/\n                my_schema.some_table.csv       # data for a table\n            data2/\n                some_data.csv        # other data\n            some_checks/             # folder with CSV checks\n                check1.sql\n                check1.csl\n                ...\n            run_this.sql             # a SQL file that will be executed\n            cleanup.sql\n        other_pipeline/              # you can have multiple pipelines that will run in parallel\n            data_check_pipeline.yml\n            ...\n\nThe file _sample\\_pipeline/data\\_check\\_pipeline.yml_ can look like this:\n\n```yaml\nsteps:\n    # this will truncate the table my_schema.some_table and load it with the data from data/my_schema.some_table.csv\n    - load_tables: data\n    # this will execute the SQL statement in run_this.sql\n    - sql_file: run_this.sql\n    # this will append the data from data2/some_data.csv to my_schema.other_table\n    - load:\n        file: data2/some_data.csv\n        table: my_schema.other_table\n        load_mode: append\n    # this will run a python script and pass the connection name\n    - cmd: "python3 /path/to/my_pipeline.py --connection {{CONNECTION}}"\n    # this will run the CSV checks in the some_checks folder\n    - check: some_checks\n```\n\nPipeline checks and simple CSV checks can coexist in a project.\n\n## Documentation\n\nSee the [documentation](https://andrjas.github.io/data_check) how to setup data_check, how to create a new project and more options.\n',
+    'long_description': '# data_check\n\ndata_check is a simple data validation tool. In its most basic form it will execute SQL queries and compare the results against CSV or Excel files. But there are more advanced features:\n\n## Features\n\n* [CSV checks](#csv-checks): compare SQL queries against CSV files\n* Excel support: Use Excel (xlsx) instead of CSV\n* multiple environments (databases) in the configuration file\n* populate tables from CSV files\n* execute any SQL files on a database\n* more complex [pipelines](#pipelines)\n* run any script/command (via pipelines)\n* simplified checks for empty datasets\n* lookups to reuse the same data in multiple queries\n\n## Database support\n\ndata_check should work with any database that works with [SQLAlchemy](https://docs.sqlalchemy.org/en/14/dialects/). Currently data_check is tested against PostgreSQL, MySQL, SQLite, Oracle and Microsoft SQL Server.\n\n## Quickstart\n\nYou need Python 3.6.2 or above to run data_check. The easiest way to install data_check is via [pipx](https://github.com/pipxproject/pipx):\n\n`pipx install data-check`\n\nThe data_check Git repository is also a sample data_check project. Clone the repository, switch to the folder and run data_check:\n\n```\ngit clone git@github.com:andrjas/data_check.git\ncd data_check\ndata_check\n```\n\nThis will run the tests in the _checks_ folder using the default connection as set in data_check.yml.\n\nSee the [documentation](https://andrjas.github.io/data_check) how to install data_check in different environments with additional database drivers and other usages of data_check.\n\n## Project layout\n\ndata_check has a simple layout for projects: a single configuration file and a folder with the test files. You can also organize the test files in subfolders.\n\n    data_check.yml    # The configuration file\n    checks/           # Default folder for data tests\n        some_test.sql # SQL file with the query to run against the database\n        some_test.csv # CSV file with the expected result\n        subfolder/    # Tests can be nested in subfolders\n\n## CSV checks\n\nThis is the default mode when running data_check. data_check expects a SQL file and a CSV file. The SQL file will be executed against the database and the result is compared with the CSV file. If they match, the test is passed, otherwise it fails.\n\n## Pipelines\n\nIf data_check finds a file named _data\\_check\\_pipeline.yml_ in a folder, it will treat this folder as a pipeline check. Instead of running [CSV checks](#csv-checks) it will execute the steps in the YAML file.\n\nExample project with a pipeline:\n\n    data_check.yml\n    checks/\n        some_test.sql                # this test will run in parallel to the pipeline test\n        some_test.csv\n        sample_pipeline/\n            data_check_pipeline.yml  # configuration for the pipeline\n            data/\n                my_schema.some_table.csv       # data for a table\n            data2/\n                some_data.csv        # other data\n            some_checks/             # folder with CSV checks\n                check1.sql\n                check1.csl\n                ...\n            run_this.sql             # a SQL file that will be executed\n            cleanup.sql\n        other_pipeline/              # you can have multiple pipelines that will run in parallel\n            data_check_pipeline.yml\n            ...\n\nThe file _sample\\_pipeline/data\\_check\\_pipeline.yml_ can look like this:\n\n```yaml\nsteps:\n    # this will truncate the table my_schema.some_table and load it with the data from data/my_schema.some_table.csv\n    - load_tables: data\n    # this will execute the SQL statement in run_this.sql\n    - sql_file: run_this.sql\n    # this will append the data from data2/some_data.csv to my_schema.other_table\n    - load:\n        file: data2/some_data.csv\n        table: my_schema.other_table\n        load_mode: append\n    # this will run a python script and pass the connection name\n    - cmd: "python3 /path/to/my_pipeline.py --connection {{CONNECTION}}"\n    # this will run the CSV checks in the some_checks folder\n    - check: some_checks\n```\n\nPipeline checks and simple CSV checks can coexist in a project.\n\n## Documentation\n\nSee the [documentation](https://andrjas.github.io/data_check) how to setup data_check, how to create a new project and more options.\n',
     'author': 'Andreas Rjasanow',
     'author_email': 'andrjas@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://andrjas.github.io/data_check/',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `data_check-0.8.0/PKG-INFO` & `data_check-0.9.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-check
-Version: 0.8.0
+Version: 0.9.0
 Summary: simple data validation
 Home-page: https://andrjas.github.io/data_check/
 License: MIT
 Keywords: data,validation,testing,quality
 Author: Andreas Rjasanow
 Author-email: andrjas@gmail.com
 Requires-Python: >=3.6.2,<4.0.0
@@ -28,37 +28,40 @@
 Provides-Extra: postgres
 Requires-Dist: Jinja2 (>=2.11.3,<3.0.0)
 Requires-Dist: SQLAlchemy (>=1.4,<2.0)
 Requires-Dist: click (>=7.1.2,<8.0.0)
 Requires-Dist: colorama (>=0.4.4,<0.5.0)
 Requires-Dist: cx_Oracle (>=8.1.0,<9.0.0); extra == "oracle"
 Requires-Dist: importlib-metadata (>=3.4.0,<4.0.0)
-Requires-Dist: numpy (>=1.19.5,<2.0.0)
+Requires-Dist: numpy (>=1.19.5,<1.20)
 Requires-Dist: openpyxl (>=3.0.9,<4.0.0)
-Requires-Dist: pandas (>=1.1.5,<2.0.0)
+Requires-Dist: pandas (>=1.1.5,<1.2)
 Requires-Dist: psycopg2-binary (>=2.8.6,<3.0.0); extra == "postgres"
 Requires-Dist: pymysql[rsa]; extra == "mysql"
 Requires-Dist: pyodbc (>=4.0.30,<5.0.0); extra == "mssql"
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Requires-Dist: pyyaml (>=5.3.1,<6.0.0)
 Project-URL: Repository, https://github.com/andrjas/data_check
 Description-Content-Type: text/markdown
 
 # data_check
 
-data_check is a simple data validation tool. In its most basic form it will execute SQL queries and compare the results against CSV files. But there are more advanced features:
+data_check is a simple data validation tool. In its most basic form it will execute SQL queries and compare the results against CSV or Excel files. But there are more advanced features:
 
 ## Features
 
 * [CSV checks](#csv-checks): compare SQL queries against CSV files
+* Excel support: Use Excel (xlsx) instead of CSV
 * multiple environments (databases) in the configuration file
 * populate tables from CSV files
 * execute any SQL files on a database
 * more complex [pipelines](#pipelines)
 * run any script/command (via pipelines)
+* simplified checks for empty datasets
+* lookups to reuse the same data in multiple queries
 
 ## Database support
 
 data_check should work with any database that works with [SQLAlchemy](https://docs.sqlalchemy.org/en/14/dialects/). Currently data_check is tested against PostgreSQL, MySQL, SQLite, Oracle and Microsoft SQL Server.
 
 ## Quickstart
```

