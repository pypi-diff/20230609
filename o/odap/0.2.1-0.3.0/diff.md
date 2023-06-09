# Comparing `tmp/odap-0.2.1-py3-none-any.whl.zip` & `tmp/odap-0.3.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,47 +1,48 @@
-Zip file size: 50710 bytes, number of entries: 62
+Zip file size: 51825 bytes, number of entries: 63
 -rw-r--r--  2.0 unx     1669 b- defN 80-Jan-01 00:00 odap/common/config.py
--rw-r--r--  2.0 unx     1781 b- defN 80-Jan-01 00:00 odap/common/databricks.py
+-rw-r--r--  2.0 unx     1779 b- defN 80-Jan-01 00:00 odap/common/databricks.py
 -rw-r--r--  2.0 unx     2653 b- defN 80-Jan-01 00:00 odap/common/dataframes.py
 -rw-r--r--  2.0 unx      497 b- defN 80-Jan-01 00:00 odap/common/exceptions.py
 -rw-r--r--  2.0 unx      902 b- defN 80-Jan-01 00:00 odap/common/functions.py
 -rw-r--r--  2.0 unx      282 b- defN 80-Jan-01 00:00 odap/common/logger.py
 -rw-r--r--  2.0 unx     2920 b- defN 80-Jan-01 00:00 odap/common/notebook.py
 -rw-r--r--  2.0 unx     1963 b- defN 80-Jan-01 00:00 odap/common/tables.py
 -rw-r--r--  2.0 unx     2645 b- defN 80-Jan-01 00:00 odap/common/test/PySparkTestCase.py
 -rw-r--r--  2.0 unx     2903 b- defN 80-Jan-01 00:00 odap/common/test/notebook/NotebookParsingTest.py
 -rw-r--r--  2.0 unx     1970 b- defN 80-Jan-01 00:00 odap/common/test/notebook/python_notebook.txt
 -rw-r--r--  2.0 unx     1485 b- defN 80-Jan-01 00:00 odap/common/test/notebook/sql_notebook.txt
--rw-r--r--  2.0 unx     3494 b- defN 80-Jan-01 00:00 odap/common/utils.py
+-rw-r--r--  2.0 unx      454 b- defN 80-Jan-01 00:00 odap/common/test/runner.py
+-rw-r--r--  2.0 unx     3590 b- defN 80-Jan-01 00:00 odap/common/utils.py
 -rw-r--r--  2.0 unx      177 b- defN 80-Jan-01 00:00 odap/common/widgets.py
--rw-r--r--  2.0 unx     5588 b- defN 80-Jan-01 00:00 odap/feature_factory/config.py
+-rw-r--r--  2.0 unx     6189 b- defN 80-Jan-01 00:00 odap/feature_factory/config.py
 -rw-r--r--  2.0 unx     1399 b- defN 80-Jan-01 00:00 odap/feature_factory/const.py
 -rw-r--r--  2.0 unx      940 b- defN 80-Jan-01 00:00 odap/feature_factory/dataframes/dataframe_checker.py
 -rw-r--r--  2.0 unx     3723 b- defN 80-Jan-01 00:00 odap/feature_factory/dataframes/dataframe_creator.py
--rw-r--r--  2.0 unx     3197 b- defN 80-Jan-01 00:00 odap/feature_factory/dataframes/dataframe_writer.py
+-rw-r--r--  2.0 unx     3933 b- defN 80-Jan-01 00:00 odap/feature_factory/dataframes/dataframe_writer.py
 -rw-r--r--  2.0 unx     1910 b- defN 80-Jan-01 00:00 odap/feature_factory/dq_checks.py
--rw-r--r--  2.0 unx     1624 b- defN 80-Jan-01 00:00 odap/feature_factory/dry_run.py
--rw-r--r--  2.0 unx      265 b- defN 80-Jan-01 00:00 odap/feature_factory/exceptions.py
--rw-r--r--  2.0 unx     3600 b- defN 80-Jan-01 00:00 odap/feature_factory/feature_notebook.py
--rw-r--r--  2.0 unx     1097 b- defN 80-Jan-01 00:00 odap/feature_factory/feature_notebooks_selection.py
+-rw-r--r--  2.0 unx     1694 b- defN 80-Jan-01 00:00 odap/feature_factory/dry_run.py
+-rw-r--r--  2.0 unx      310 b- defN 80-Jan-01 00:00 odap/feature_factory/exceptions.py
+-rw-r--r--  2.0 unx     3619 b- defN 80-Jan-01 00:00 odap/feature_factory/feature_notebook.py
+-rw-r--r--  2.0 unx     2620 b- defN 80-Jan-01 00:00 odap/feature_factory/feature_notebooks_selection.py
 -rw-r--r--  2.0 unx     4116 b- defN 80-Jan-01 00:00 odap/feature_factory/feature_store.py
 -rw-r--r--  2.0 unx      624 b- defN 80-Jan-01 00:00 odap/feature_factory/ids.py
 -rw-r--r--  2.0 unx     5583 b- defN 80-Jan-01 00:00 odap/feature_factory/metadata.py
 -rw-r--r--  2.0 unx     3494 b- defN 80-Jan-01 00:00 odap/feature_factory/metadata_schema.py
 -rw-r--r--  2.0 unx     2120 b- defN 80-Jan-01 00:00 odap/feature_factory/no_target_optimizer.py
--rw-r--r--  2.0 unx     1224 b- defN 80-Jan-01 00:00 odap/feature_factory/orchestrate.py
+-rw-r--r--  2.0 unx     1386 b- defN 80-Jan-01 00:00 odap/feature_factory/orchestrate.py
 -rw-r--r--  2.0 unx     1038 b- defN 80-Jan-01 00:00 odap/feature_factory/tables_validator.py
 -rw-r--r--  2.0 unx     4106 b- defN 80-Jan-01 00:00 odap/feature_factory/templates.py
 -rw-r--r--  2.0 unx     1511 b- defN 80-Jan-01 00:00 odap/feature_factory/tests/LatestDataFrameTest.py
 -rw-r--r--  2.0 unx     2463 b- defN 80-Jan-01 00:00 odap/feature_factory/tests/NoTargetOptimizationTest.py
 -rw-r--r--  2.0 unx     4573 b- defN 80-Jan-01 00:00 odap/feature_factory/tests/TimeWindowsTest.py
 -rw-r--r--  2.0 unx     4310 b- defN 80-Jan-01 00:00 odap/feature_factory/tests/metadata_test.py
 -rw-r--r--  2.0 unx    10895 b- defN 80-Jan-01 00:00 odap/feature_factory/time_windows.py
 -rw-r--r--  2.0 unx     1543 b- defN 80-Jan-01 00:00 odap/feature_factory/type_checker.py
--rw-r--r--  2.0 unx      792 b- defN 80-Jan-01 00:00 odap/feature_factory/widgets.py
+-rw-r--r--  2.0 unx     1048 b- defN 80-Jan-01 00:00 odap/feature_factory/widgets.py
 -rw-r--r--  2.0 unx     3708 b- defN 80-Jan-01 00:00 odap/segment_factory/Export.py
 -rw-r--r--  2.0 unx     3490 b- defN 80-Jan-01 00:00 odap/segment_factory/config.py
 -rw-r--r--  2.0 unx     1207 b- defN 80-Jan-01 00:00 odap/segment_factory/config_checker.py
 -rw-r--r--  2.0 unx       52 b- defN 80-Jan-01 00:00 odap/segment_factory/exceptions.py
 -rw-r--r--  2.0 unx     1220 b- defN 80-Jan-01 00:00 odap/segment_factory/exporters.py
 -rw-r--r--  2.0 unx     2129 b- defN 80-Jan-01 00:00 odap/segment_factory/logs.py
 -rw-r--r--  2.0 unx      415 b- defN 80-Jan-01 00:00 odap/segment_factory/orchestrate.py
@@ -52,13 +53,13 @@
 -rw-r--r--  2.0 unx     1586 b- defN 80-Jan-01 00:00 odap/use_case/config.py
 -rw-r--r--  2.0 unx     1107 b- defN 80-Jan-01 00:00 odap/use_case/functions.py
 -rw-r--r--  2.0 unx      529 b- defN 80-Jan-01 00:00 odap/use_case/notebooks.py
 -rw-r--r--  2.0 unx      939 b- defN 80-Jan-01 00:00 odap/use_case/schemas.py
 -rw-r--r--  2.0 unx      423 b- defN 80-Jan-01 00:00 odap/use_case/status.py
 -rw-r--r--  2.0 unx      536 b- defN 80-Jan-01 00:00 odap/use_case/table.py
 -rw-r--r--  2.0 unx     1360 b- defN 80-Jan-01 00:00 odap/use_case/usecases.py
-?rw-r--r--  2.0 unx       99 b- defN 16-Jan-01 00:00 odap-0.2.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx     2473 b- defN 80-Jan-01 00:00 odap-0.2.1.dist-info/LICENSE
-?rw-r--r--  2.0 unx       83 b- defN 16-Jan-01 00:00 odap-0.2.1.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1710 b- defN 16-Jan-01 00:00 odap-0.2.1.dist-info/METADATA
-?rw-r--r--  2.0 unx     5513 b- defN 16-Jan-01 00:00 odap-0.2.1.dist-info/RECORD
-62 files, 131941 bytes uncompressed, 41874 bytes compressed:  68.3%
+?rw-r--r--  2.0 unx       99 b- defN 16-Jan-01 00:00 odap-0.3.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx     2473 b- defN 80-Jan-01 00:00 odap-0.3.0.dist-info/LICENSE
+?rw-r--r--  2.0 unx       83 b- defN 16-Jan-01 00:00 odap-0.3.0.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1659 b- defN 16-Jan-01 00:00 odap-0.3.0.dist-info/METADATA
+?rw-r--r--  2.0 unx     5596 b- defN 16-Jan-01 00:00 odap-0.3.0.dist-info/RECORD
+63 files, 135933 bytes uncompressed, 42861 bytes compressed:  68.5%
```

## zipnote {}

```diff
@@ -30,14 +30,17 @@
 
 Filename: odap/common/test/notebook/python_notebook.txt
 Comment: 
 
 Filename: odap/common/test/notebook/sql_notebook.txt
 Comment: 
 
+Filename: odap/common/test/runner.py
+Comment: 
+
 Filename: odap/common/utils.py
 Comment: 
 
 Filename: odap/common/widgets.py
 Comment: 
 
 Filename: odap/feature_factory/config.py
@@ -165,23 +168,23 @@
 
 Filename: odap/use_case/table.py
 Comment: 
 
 Filename: odap/use_case/usecases.py
 Comment: 
 
-Filename: odap-0.2.1.dist-info/entry_points.txt
+Filename: odap-0.3.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: odap-0.2.1.dist-info/LICENSE
+Filename: odap-0.3.0.dist-info/LICENSE
 Comment: 
 
-Filename: odap-0.2.1.dist-info/WHEEL
+Filename: odap-0.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: odap-0.2.1.dist-info/METADATA
+Filename: odap-0.3.0.dist-info/METADATA
 Comment: 
 
-Filename: odap-0.2.1.dist-info/RECORD
+Filename: odap-0.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## odap/common/databricks.py

```diff
@@ -4,14 +4,17 @@
 from databricks_cli.workspace.api import WorkspaceApi
 from databricks_cli.repos.api import ReposApi
 from databricks_cli.sdk.api_client import ApiClient
 from odap.common.utils import get_repository_info
 from odap.common.exceptions import UnableToResolveBranchException
 
 
+spark = SparkSession.getActiveSession()
+
+
 def resolve_dbutils() -> DBUtils:
     return resolve_databricks_service("dbutils")
 
 
 def resolve_display():
     return resolve_databricks_service("display")
 
@@ -40,15 +43,14 @@
     dbutils = resolve_dbutils()
 
     api_client = ApiClient(host=get_host(), token=get_token(dbutils))
     return ReposApi(api_client)
 
 
 def get_host() -> str:
-    spark = SparkSession.getActiveSession()
     return f"https://{spark.conf.get('spark.databricks.workspaceUrl')}"
 
 
 def get_token(dbutils: DBUtils) -> str:
     return dbutils.notebook.entry_point.getDbutils().notebook().getContext().apiToken().get()
```

## odap/common/utils.py

```diff
@@ -17,22 +17,30 @@
     return min((path for path in sys.path if path.startswith("/Workspace/Repos")), key=len)
 
 
 def get_repository_root_api_path() -> str:
     return get_api_path(get_repository_root_fs_path())
 
 
+def offset_base_dir(root_path: Path) -> str:
+    odap_base_dir = os.environ.get("ODAP_BASE_DIR")
+
+    if not odap_base_dir:
+        return str(root_path)
+
+    return str(root_path / odap_base_dir)
+
+
 def get_project_root_fs_path() -> str:
-    dirs_to_search = [Path.cwd()] + list(Path.cwd().parents)
+    path = Path.cwd()
 
-    for path in dirs_to_search:
-        if path.joinpath("features").is_dir() and path.joinpath("config.yaml").is_file():
-            return str(path)
+    if path.parts[3] == ".internal":
+        return offset_base_dir(Path(*path.parts[0:6]))
 
-    raise Exception("Cannot resolve project root path")
+    return offset_base_dir(Path(*path.parts[0:5]))
 
 
 def get_project_root_api_path() -> str:
     return re.sub("^/Workspace", "", get_project_root_fs_path())
 
 
 def get_relative_path(path: str):
```

## odap/feature_factory/config.py

```diff
@@ -185,7 +185,29 @@
     entity_name = get_entity(config)
 
     return ids_table.format(entity=entity_name)
 
 
 def use_no_target_optimization(config: Config) -> bool:
     return config.get("no_target_optimization") is not None
+
+
+def get_feature_dir(config: Config) -> str:
+    return config.get("feature_dir", "features")
+
+
+def get_checkpoint_dir(config: Config):
+    checkpoint_dir = config.get("checkpoint_dir")
+
+    if not checkpoint_dir:
+        raise ConfigAttributeMissingException("checkpoint_dir not defined in config.yaml")
+
+    return checkpoint_dir
+
+
+def get_checkpoint_interval(config: Config):
+    checkpoint_interval = config.get("checkpoint_interval")
+
+    if not checkpoint_interval:
+        raise ConfigAttributeMissingException("checkpoint_interval not defined in config.yaml")
+
+    return checkpoint_interval
```

## odap/feature_factory/dataframes/dataframe_writer.py

```diff
@@ -1,32 +1,32 @@
-from typing import Dict
+from typing import Dict, Iterable
 
-from pyspark.sql import SparkSession
-from databricks.feature_store import FeatureStoreClient
+from pyspark.sql import SparkSession, functions as f
 from delta import DeltaTable
 
 from odap.common.config import TIMESTAMP_COLUMN, Config
+from odap.common.databricks import spark
 from odap.common.tables import create_table_if_not_exists
 from odap.feature_factory.config import (
     get_entity_primary_key,
     get_features_table,
     get_features_table_path,
     get_latest_features_table,
     get_latest_features_table_path,
     get_metadata_table,
     get_metadata_table_path,
-    get_entity,
+    get_checkpoint_dir,
+    get_checkpoint_interval,
 )
 from odap.feature_factory.dataframes.dataframe_creator import (
     create_metadata_df,
     create_features_df,
     fill_nulls,
 )
-from odap.feature_factory.feature_store import write_df_to_feature_store, write_latest_table, generate_feature_lookups
-from odap.feature_factory.ids import get_latest_ids
+from odap.feature_factory.feature_store import write_df_to_feature_store, write_latest_table
 from odap.feature_factory.metadata_schema import get_metadata_pk_columns, get_metadata_columns, get_metadata_schema
 from odap.feature_factory.feature_notebook import FeatureNotebookList
 
 
 def write_metadata_df(feature_notebooks: FeatureNotebookList, config: Config):
     create_table_if_not_exists(get_metadata_table(config), get_metadata_table_path(config), get_metadata_schema())
     metadata_df = create_metadata_df(feature_notebooks)
@@ -58,24 +58,38 @@
             table_name=get_features_table(table_name, config),
             table_path=get_features_table_path(table_name, config),
             primary_keys=[entity_primary_key],
             timestamp_keys=[TIMESTAMP_COLUMN],
         )
 
 
-def write_latest_features(feature_notebooks: FeatureNotebookList, config: Config):
-    fs = FeatureStoreClient()
-    entity_name = get_entity(config)
+def get_latest_dataframe(feature_tables: Iterable[str], config: Config):
+    spark.sparkContext.setCheckpointDir(get_checkpoint_dir(config))
 
-    ids_df = get_latest_ids(config)
+    features_dfs = [spark.table(get_features_table(table, config)) for table in feature_tables]
 
-    latest_df = (
-        fs.create_training_set(ids_df, generate_feature_lookups(entity_name), label=None)
-        .load_df()
-        .drop(TIMESTAMP_COLUMN)
-    )
+    features_dfs_max_date = [(df, df.select(f.max(TIMESTAMP_COLUMN)).collect()[0][0]) for df in features_dfs]
+
+    features_dfs_max_date_filtered = [
+        df.filter(f.col(TIMESTAMP_COLUMN) == max_ts).drop(TIMESTAMP_COLUMN) for df, max_ts in features_dfs_max_date
+    ]
+
+    latest_df = features_dfs_max_date_filtered[0]
+
+    for i, df in enumerate(features_dfs_max_date_filtered[1:]):
+        latest_df = latest_df.join(df, on=get_entity_primary_key(config), how="full")
+        if not i % get_checkpoint_interval(config):
+            latest_df.checkpoint()
+    return latest_df
+
+
+def write_latest_features(feature_notebooks: FeatureNotebookList, config: Config):
+    metadata_df = spark.table(get_metadata_table(config))
+    feature_tables = [row.table for row in metadata_df.select("table").distinct().collect()]
+
+    latest_df = get_latest_dataframe(feature_tables, config)
     latest_features_filled = fill_nulls(latest_df, feature_notebooks)
 
     latest_table_path = get_latest_features_table_path(config)
     latest_table_name = get_latest_features_table(config)
 
     write_latest_table(latest_features_filled, latest_table_name, latest_table_path)
```

## odap/feature_factory/dry_run.py

```diff
@@ -1,22 +1,23 @@
 from pyspark.sql import DataFrame
 
 from odap.common.config import ConfigNamespace, get_config_namespace
 from odap.common.logger import logger
 from odap.common.widgets import get_widget_value
 from odap.feature_factory import const
-from odap.feature_factory.config import get_entity_primary_key
+from odap.feature_factory.config import get_entity_primary_key, get_feature_dir
 from odap.feature_factory.dataframes.dataframe_creator import create_features_df, create_metadata_df
 from odap.feature_factory.feature_notebook import load_feature_notebooks
 from odap.feature_factory.feature_notebooks_selection import get_list_of_selected_feature_notebooks
 
 
 def dry_run():
     config = get_config_namespace(ConfigNamespace.FEATURE_FACTORY)
-    feature_notebooks = load_feature_notebooks(config, get_list_of_selected_feature_notebooks())
+    feature_dir = get_feature_dir(config)
+    feature_notebooks = load_feature_notebooks(config, get_list_of_selected_feature_notebooks(feature_dir))
 
     entity_primary_key = get_entity_primary_key(config)
 
     features_df = create_features_df(feature_notebooks, entity_primary_key)
     metadata_df = create_metadata_df(feature_notebooks)
 
     logger.info("Success. No errors found!")
```

## odap/feature_factory/exceptions.py

```diff
@@ -1,4 +1,8 @@
 class WrongFillnaValueTypeError(Exception):
     def __init__(self, value: str, name_template: str, dtype: str):
         message = f"Value for fillna_with: {value} is not compatible with feature {name_template} of the type {dtype}"
         super().__init__(message)
+
+
+class WidgetException(Exception):
+    pass
```

## odap/feature_factory/feature_notebook.py

```diff
@@ -54,16 +54,16 @@
 
         logger.info(f"Feature {self.info.path} successfully loaded.")
 
 
 FeatureNotebookList = List[FeatureNotebook]
 
 
-def get_feature_notebooks_info(workspace_api: WorkspaceApi) -> List[WorkspaceFileInfo]:
-    features_path = get_absolute_api_path("features")
+def get_feature_notebooks_info(workspace_api: WorkspaceApi, feature_dir: str) -> List[WorkspaceFileInfo]:
+    features_path = get_absolute_api_path(feature_dir)
 
     return list_notebooks_info(features_path, workspace_api, recurse=True)
 
 
 def get_feature_notebook_cells(info: WorkspaceFileInfo, workspace_api: WorkspaceApi, config: Config) -> List[str]:
     notebook_cells = get_notebook_cells(info, workspace_api)
     if use_no_target_optimization(config):
```

## odap/feature_factory/feature_notebooks_selection.py

```diff
@@ -2,29 +2,65 @@
 
 from databricks_cli.workspace.api import WorkspaceFileInfo
 
 from odap.common.databricks import get_workspace_api
 from odap.common.widgets import get_widget_value
 from odap.feature_factory import const
 from odap.feature_factory.feature_notebook import get_feature_notebooks_info
+from odap.feature_factory.exceptions import WidgetException
 
 
-def get_list_of_selected_feature_notebooks() -> List[WorkspaceFileInfo]:
+def get_list_of_selected_feature_notebooks(feature_dir: str) -> List[WorkspaceFileInfo]:
     feature_notebooks_str = get_widget_value(const.FEATURE_WIDGET)
-    feature_notebooks = get_feature_notebooks_info(get_workspace_api())
+    feature_notebooks = get_feature_notebooks_info(get_workspace_api(), feature_dir)
 
     if feature_notebooks_str == const.ALL_FEATURES:
         return feature_notebooks
 
     feature_notebooks_list = feature_notebooks_str.split(",")
 
+    feature_notebooks = [
+        feature_notebook
+        for feature_notebook in feature_notebooks
+        if feature_notebook.basename in feature_notebooks_list
+    ]
+
+    verify_feature_notebooks(feature_notebooks_list, feature_notebooks)
+
+    return feature_notebooks
+
+
+def verify_feature_notebooks(feature_notebooks_list: List[str], feature_notebooks: List[WorkspaceFileInfo]):
+    check_all_features_is_not_present(feature_notebooks_list)
+
+    check_for_missing_feature_notebooks(feature_notebooks_list, feature_notebooks)
+
+    check_for_duplicate_notebook_names(feature_notebooks_list)
+
+
+def check_all_features_is_not_present(feature_notebooks_list):
     if const.ALL_FEATURES in feature_notebooks_list:
-        raise Exception(
+        raise WidgetException(
             f"`{const.ALL_FEATURES}` together with selected notebooks is not a valid option. Please select "
             f"either `{const.ALL_FEATURES}` only or a subset of notebooks"
         )
 
-    return [
-        feature_notebook
-        for feature_notebook in feature_notebooks
-        if feature_notebook.basename in feature_notebooks_list
-    ]
+
+def check_for_missing_feature_notebooks(feature_notebooks_list: List[str], feature_notebooks: List[WorkspaceFileInfo]):
+    if len(feature_notebooks_list) == 1 and feature_notebooks_list[0] == "":
+        raise WidgetException("No feature notebooks were selected")
+
+    missing_feature_notebooks = set(feature_notebooks_list) - set(notebook.basename for notebook in feature_notebooks)
+
+    if missing_feature_notebooks:
+        raise WidgetException(f"Following feature notebooks were not found: {missing_feature_notebooks}")
+
+
+def check_for_duplicate_notebook_names(feature_notebooks_list: List[str]):
+    duplicate_notebook_names = set(
+        notebook for notebook in feature_notebooks_list if feature_notebooks_list.count(notebook) > 1
+    )
+
+    if duplicate_notebook_names:
+        raise WidgetException(
+            f"Following feature notebook names are present more than once: {duplicate_notebook_names}"
+        )
```

## odap/feature_factory/orchestrate.py

```diff
@@ -1,28 +1,31 @@
 from odap.common.config import get_config_namespace, ConfigNamespace
+from odap.feature_factory.config import get_feature_dir
 from odap.feature_factory.dataframes.dataframe_writer import (
     write_features_df,
     write_latest_features,
     write_metadata_df,
 )
 from odap.feature_factory.feature_notebook import create_notebook_table_mapping, load_feature_notebooks
 from odap.feature_factory.feature_notebooks_selection import get_list_of_selected_feature_notebooks
 from odap.feature_factory.tables_validator import validate_feature_store_tables
 
 
 def orchestrate():
     config = get_config_namespace(ConfigNamespace.FEATURE_FACTORY)
+    feature_dir = get_feature_dir(config)
 
-    feature_notebooks = load_feature_notebooks(config, get_list_of_selected_feature_notebooks())
+    feature_notebooks = load_feature_notebooks(config, get_list_of_selected_feature_notebooks(feature_dir))
     notebook_table_mapping = create_notebook_table_mapping(feature_notebooks)
     feature_tables = list(notebook_table_mapping.keys())
     validate_feature_store_tables(feature_tables, config)
 
     write_metadata_df(feature_notebooks, config)
     write_features_df(notebook_table_mapping, config)
 
 
 def calculate_latest_table():
     config = get_config_namespace(ConfigNamespace.FEATURE_FACTORY)
+    feature_dir = get_feature_dir(config)
 
-    feature_notebooks = load_feature_notebooks(config, get_list_of_selected_feature_notebooks())
+    feature_notebooks = load_feature_notebooks(config, get_list_of_selected_feature_notebooks(feature_dir))
     write_latest_features(feature_notebooks, config)
```

## odap/feature_factory/widgets.py

```diff
@@ -1,18 +1,24 @@
+from odap.common.config import get_config_namespace, ConfigNamespace
 from odap.common.databricks import resolve_dbutils, get_workspace_api
 from odap.common.utils import get_notebook_name
 from odap.feature_factory import const
+from odap.feature_factory.config import get_feature_dir
 from odap.feature_factory.feature_notebook import get_feature_notebooks_info
 
 
 def create_notebooks_widget():
     dbutils = resolve_dbutils()
 
+    config = get_config_namespace(ConfigNamespace.FEATURE_FACTORY)
+    feature_dir = get_feature_dir(config)
+
     features = [
-        get_notebook_name(notebook_info.path) for notebook_info in get_feature_notebooks_info(get_workspace_api())
+        get_notebook_name(notebook_info.path)
+        for notebook_info in get_feature_notebooks_info(get_workspace_api(), feature_dir)
     ]
 
     dbutils.widgets.multiselect(const.FEATURE_WIDGET, const.ALL_FEATURES, [const.ALL_FEATURES] + features)
 
 
 def create_dry_run_widgets():
     dbutils = resolve_dbutils()
```

## Comparing `odap-0.2.1.dist-info/LICENSE` & `odap-0.3.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `odap-0.2.1.dist-info/METADATA` & `odap-0.3.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: odap
-Version: 0.2.1
+Version: 0.3.0
 Summary: ODAP framework
 License: Proprietary
 Author: Jiri Koutny
 Author-email: jiri.koutny@datasentics.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 
 # ODAP Use Case Builder Framework
 
 ## Overview
```

## Comparing `odap-0.2.1.dist-info/RECORD` & `odap-0.3.0.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -1,46 +1,47 @@
 odap/common/config.py,sha256=YBRQzyi3UxtGGbOUiUzCwwnJAqdFAmyQxFX4m-hmR_4,1669
-odap/common/databricks.py,sha256=o4fjvHuXF924SdKtbPhfdAHPpnOXPfqVjA3hvIczFT8,1781
+odap/common/databricks.py,sha256=4Gz7uhu7ahNZZEnttV9VjzX6ecJ_X1OpXbqLAuq0V-s,1779
 odap/common/dataframes.py,sha256=QZNcPKQ0PAUKeqQMWgb-EYAMvzOP6ifkxG8OG2roh9o,2653
 odap/common/exceptions.py,sha256=zoNAWEmrr-FRVbF4910c4oMMLJKy2sSyhtJMWmmXu1Y,497
 odap/common/functions.py,sha256=tVFkWo1i01ySeW6u4a1HzpNfGKFP5LOdIe-Q2zCtQmM,902
 odap/common/logger.py,sha256=gKyoz2rIfUvG5xpa9w7A6Dom1L_gOFg9hqD0bVo8IQ8,282
 odap/common/notebook.py,sha256=rUZW6j4HtvSK3SY9NLmAK84gi6XuWfXaH8baLUW1Kls,2920
 odap/common/tables.py,sha256=zmRApOHgwcHjds5D7dggUK4KbwdxDBsoqT_LBH3EXTk,1963
 odap/common/test/PySparkTestCase.py,sha256=2dHcT5zw3acxGzT8YT-E1wVCACnb5kaZaFFjDS5fOew,2645
 odap/common/test/notebook/NotebookParsingTest.py,sha256=6eeFhyQkM8R3xNe15N5DcGw2w_xbEiYdkXV7u6Rt5HU,2903
 odap/common/test/notebook/python_notebook.txt,sha256=ds4aCaRi7ko7BPoivDRJunbz8yCw3SI54TXSmIXaQc0,1970
 odap/common/test/notebook/sql_notebook.txt,sha256=S4HPnA2Wxley-mx3Nnpl4guKg6xLPjGWwcjBwEdShIU,1485
-odap/common/utils.py,sha256=MPddvcAtsyvldBbXfe0UMN7MNYCLo9muPCUnWpBb4h4,3494
+odap/common/test/runner.py,sha256=m_-l4SNGXDyz8VtZWza_Ly4eVRldKS5ZhRy01TXSal8,454
+odap/common/utils.py,sha256=otAWTAZd9_Drsa5odquh2Vn4KqXL6SLzBT1iWLeHMZk,3590
 odap/common/widgets.py,sha256=AEy-EeG5cP3iRV9ehgdnW-Va3hWpQ7DdAsrQypDCszk,177
-odap/feature_factory/config.py,sha256=of_-ktzkNMGBEx1EQovQIvol9jC_jRtP4JsokG728Lo,5588
+odap/feature_factory/config.py,sha256=OLtSNKbMrT7nN_bM5bCiE03qZI-ZEE5hljpmxgMtenA,6189
 odap/feature_factory/const.py,sha256=iF8DzX6I-koPXNcFeYSObZ2fmgULTWe_c20oP4rjX7E,1399
 odap/feature_factory/dataframes/dataframe_checker.py,sha256=l0NsnPzGV2W0EM3bonuBx1oKmzQWOEaKzJLNBgUhPqw,940
 odap/feature_factory/dataframes/dataframe_creator.py,sha256=31uaA50FbHan1vh9VSZfvNgSbLJpDlr7spXud-60vcA,3723
-odap/feature_factory/dataframes/dataframe_writer.py,sha256=dnl3Y-nDLz4LOYII5yMBPg6mj24Rnf4rhmmFZyvw1ZI,3197
+odap/feature_factory/dataframes/dataframe_writer.py,sha256=JilZkFNxiojI9v7CJjsgmYoymYZbCuCghI17f13Uye8,3933
 odap/feature_factory/dq_checks.py,sha256=A8wukD9EUsSVdn3zSM1YuDaGVtw2gtKGiy8lBjkV_v8,1910
-odap/feature_factory/dry_run.py,sha256=1cxrBVOumMQZEvfeqHi0a1iszOpPKYA8v66qOTd90AA,1624
-odap/feature_factory/exceptions.py,sha256=mXsW9MX17NPEOoteHOqVbKdwocJF69OVzUbwcmrfcW4,265
-odap/feature_factory/feature_notebook.py,sha256=Of-p5vV9lMF2P7wzDrylMUrEDowAgGOOFNpcOauGxv4,3600
-odap/feature_factory/feature_notebooks_selection.py,sha256=linKOKdcZTrNOr-HpptdFWQQQiTc4a7jt2PuJ-9Z42c,1097
+odap/feature_factory/dry_run.py,sha256=6NdrVx_wmGX9oU31VnqqPk9te4GCH5wHYDTy_NgaEsI,1694
+odap/feature_factory/exceptions.py,sha256=EV32PH5_8EbuiD3_2tkKSXNyLG5kpZ-PSHNc9K-CoAw,310
+odap/feature_factory/feature_notebook.py,sha256=hWDJ44qoyo91ZRLmbLxKmtuAcoLZPiAehBzrRxvcLVI,3619
+odap/feature_factory/feature_notebooks_selection.py,sha256=LUxSwnX0NATKVf7usrU0QO_PleKUt1ev30StKio2g9U,2620
 odap/feature_factory/feature_store.py,sha256=FaurZ4_L97rF8NApL-bC3RCUYsQDzM8YpVpidjRhz8o,4116
 odap/feature_factory/ids.py,sha256=TPm8mnLejz5bdlQMCa8hIiKcWXZfYJuEPSA8LJ7Yvs8,624
 odap/feature_factory/metadata.py,sha256=U2b6vzSCHYL6KaVJgHiz3gOR3TGxvWseroVmOOH5HaM,5583
 odap/feature_factory/metadata_schema.py,sha256=nLT2HlRAQ9ZE8MCHDLuTqfWrJVIAch_NPf-hSdxiaH4,3494
 odap/feature_factory/no_target_optimizer.py,sha256=4IOjPmU5LwQMYHYHhrbigOfORqzLajU4AZMmG59sunc,2120
-odap/feature_factory/orchestrate.py,sha256=5R6lGOfL6v4yRL_9-Z_5f5ZzgFd27b67uu0BtW1hJ9s,1224
+odap/feature_factory/orchestrate.py,sha256=JG8SKsmcS2-qq60W87nH3NRqHHGPNohjRQjgh74sGa8,1386
 odap/feature_factory/tables_validator.py,sha256=GZoN_uyIKH_isUhmCS5eAHUoPuOjGiASFUjdJJXm3kc,1038
 odap/feature_factory/templates.py,sha256=XfCHJzv8tAuUMrvfaM2munpuQP02ibNwQJRbPlRtOG4,4106
 odap/feature_factory/tests/LatestDataFrameTest.py,sha256=xPrf4AhcFGOD41OBGd6ojs17rfewAEQ7bc-_5F0_Iv0,1511
 odap/feature_factory/tests/NoTargetOptimizationTest.py,sha256=VCtKUqY1mir5r3AlaS_EYCsCE3-XoLws5ISzwmUnlyg,2463
 odap/feature_factory/tests/TimeWindowsTest.py,sha256=HFe9PerIFyKt6E4Qt06czPYGxX4syFvTEFEOWqhC1IY,4573
 odap/feature_factory/tests/metadata_test.py,sha256=uHd7Mg0uDe5eHYBaXFk3FCANTruVOfyrMyU2RhgDQjw,4310
 odap/feature_factory/time_windows.py,sha256=2IZenm2wjvqO05FTqzIhPX_-nI2ce_ZeOqkb3Tqk9j8,10895
 odap/feature_factory/type_checker.py,sha256=pgmSwfowOnEtvHm1y_NT9JSI2NI4l-qi9nvTqBOiQNU,1543
-odap/feature_factory/widgets.py,sha256=U3L-VrIWMYslerw10E41v4uGkLMm8NZb8p4eM6k5n5g,792
+odap/feature_factory/widgets.py,sha256=GK5l6iOUSUmfyWqEn-UgVW74HTEYWTsX2r8QQNDSAOE,1048
 odap/segment_factory/Export.py,sha256=1dEl2IOI2LwCdybRg7IXy4KchSewqY_uOSrLM7HHbZ4,3708
 odap/segment_factory/config.py,sha256=BZBEmRowNdRkVVvLbouKLj_6NnvRdBngPN2_JtMW21g,3490
 odap/segment_factory/config_checker.py,sha256=R4SAJByGQJT3K3Tlgfye9TaQehNWwzE3tTxRi9MRygI,1207
 odap/segment_factory/exceptions.py,sha256=eQ04AdbrNYB20kGzK9v1bU7VZkcVTeVQYp-qSnJWqow,52
 odap/segment_factory/exporters.py,sha256=QAZlcEG3a2S6MWUYQI-LYMiJBzWtItvSRPNPA5qM2mo,1220
 odap/segment_factory/logs.py,sha256=SGlQTg9HzC_8X5axOTmnXWra6UbpnrmVIzbA2MHwG-g,2129
 odap/segment_factory/orchestrate.py,sha256=0qm4_CSSpxy-J3to1nFKiUH8FX1TO2dSRxHZFd3PKc8,415
@@ -51,12 +52,12 @@
 odap/use_case/config.py,sha256=YBr4paZCQfP6ANkjrD69waXc1eqxqVVZOJ6GGh7Og0E,1586
 odap/use_case/functions.py,sha256=6iJ6bv6_NLqSuP68PUtGAsKkdKLd_rn9Xn7FuNLeQHw,1107
 odap/use_case/notebooks.py,sha256=c53sSuis02P4P65yQmVQBp0IkyO5TZ_U1gEO9Z-jlaU,529
 odap/use_case/schemas.py,sha256=AfREgaOZv_kxjIMieSNzXppaJKjp4zCOrV1BuU93K2E,939
 odap/use_case/status.py,sha256=WDCFZI-9f4yWM7K6StbTMrefqj5CJW0f6ah5T2CiqR4,423
 odap/use_case/table.py,sha256=3wy1EWwQvqiGa-qTa7ltSmXll0Fw47VpBZw5TvYVKJg,536
 odap/use_case/usecases.py,sha256=CsL3o8cOEf_3bd0fa--EgemK0hk-3glswpRcT6lYj7E,1360
-odap-0.2.1.dist-info/entry_points.txt,sha256=QXVQtlr9JG_kOXiPd_ttPEdqWHJJaM4WohBThAfeb4Y,99
-odap-0.2.1.dist-info/LICENSE,sha256=ITxuTlsYJVT6xChvCiIdtQ9WfPAccufieGU46cPpQ08,2473
-odap-0.2.1.dist-info/WHEEL,sha256=DA86_h4QwwzGeRoz62o1svYt5kGEXpoUTuTtwzoTb30,83
-odap-0.2.1.dist-info/METADATA,sha256=cHMytdzCzynm-RBD80t9uDZp3gytsKpqBxl1pSws8JI,1710
-odap-0.2.1.dist-info/RECORD,,
+odap-0.3.0.dist-info/entry_points.txt,sha256=QXVQtlr9JG_kOXiPd_ttPEdqWHJJaM4WohBThAfeb4Y,99
+odap-0.3.0.dist-info/LICENSE,sha256=ITxuTlsYJVT6xChvCiIdtQ9WfPAccufieGU46cPpQ08,2473
+odap-0.3.0.dist-info/WHEEL,sha256=N0LZrBtofpkS5mJXgVHTCEy52Sam4D6PHQWC8HnMeTs,83
+odap-0.3.0.dist-info/METADATA,sha256=RoSEymVVuY2M7CYdCofncVw3_pivMDashBm2RWXYJak,1659
+odap-0.3.0.dist-info/RECORD,,
```

