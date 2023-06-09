# Comparing `tmp/grai_source_dbt_cloud-0.0.3a3.tar.gz` & `tmp/grai_source_dbt_cloud-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grai_source_dbt_cloud-0.0.3a3.tar", max compression
+gzip compressed data, was "grai_source_dbt_cloud-0.0.4.tar", max compression
```

## Comparing `grai_source_dbt_cloud-0.0.3a3.tar` & `grai_source_dbt_cloud-0.0.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      142 2023-05-17 10:43:12.453217 grai_source_dbt_cloud-0.0.3a3/README.md
--rw-r--r--   0        0        0      933 2023-05-18 14:29:08.425794 grai_source_dbt_cloud-0.0.3a3/pyproject.toml
--rw-r--r--   0        0        0       47 2023-05-17 10:43:12.458689 grai_source_dbt_cloud-0.0.3a3/src/grai_source_dbt_cloud/__init__.py
--rw-r--r--   0        0        0      929 2023-05-18 13:39:45.657214 grai_source_dbt_cloud-0.0.3a3/src/grai_source_dbt_cloud/base.py
--rw-r--r--   0        0        0     3729 2023-05-18 14:07:17.461144 grai_source_dbt_cloud-0.0.3a3/src/grai_source_dbt_cloud/loader.py
--rw-r--r--   0        0        0        0 2023-05-17 10:43:12.459210 grai_source_dbt_cloud-0.0.3a3/src/grai_source_dbt_cloud/py.typed
--rw-r--r--   0        0        0     1066 1970-01-01 00:00:00.000000 grai_source_dbt_cloud-0.0.3a3/PKG-INFO
+-rw-r--r--   0        0        0      142 2023-05-19 11:07:12.923589 grai_source_dbt_cloud-0.0.4/README.md
+-rw-r--r--   0        0        0      998 2023-06-09 19:59:37.557112 grai_source_dbt_cloud-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0       70 2023-06-09 19:59:37.562933 grai_source_dbt_cloud-0.0.4/src/grai_source_dbt_cloud/__init__.py
+-rw-r--r--   0        0        0     1386 2023-06-01 16:01:43.258274 grai_source_dbt_cloud-0.0.4/src/grai_source_dbt_cloud/base.py
+-rw-r--r--   0        0        0     4549 2023-06-01 16:01:43.258418 grai_source_dbt_cloud-0.0.4/src/grai_source_dbt_cloud/loader.py
+-rw-r--r--   0        0        0        0 2023-05-19 11:07:12.925377 grai_source_dbt_cloud-0.0.4/src/grai_source_dbt_cloud/py.typed
+-rw-r--r--   0        0        0     1064 1970-01-01 00:00:00.000000 grai_source_dbt_cloud-0.0.4/PKG-INFO
```

### Comparing `grai_source_dbt_cloud-0.0.3a3/src/grai_source_dbt_cloud/base.py` & `grai_source_dbt_cloud-0.0.4/src/grai_source_dbt_cloud/base.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,26 +5,60 @@
 from grai_schemas.base import Edge, Node
 from grai_source_dbt_cloud.loader import DbtCloudConnector
 
 from grai_source_dbt.adapters import adapt_to_client
 
 
 def get_events(connector: DbtCloudConnector, last_event_date: Optional[str]):
+    """
+
+    Args:
+        connector (DbtCloudConnector):
+        last_event_date (Optional[str]):
+
+    Returns:
+
+    Raises:
+
+    """
     events = connector.get_events(last_event_date=last_event_date)
 
     return events
 
 
 def get_nodes_and_edges(connector: DbtCloudConnector, version: str = "v1") -> Tuple[List[Node], List[Edge]]:
+    """
+
+    Args:
+        connector (DbtCloudConnector):
+        version (str, optional):  (Default value = "v1")
+
+    Returns:
+
+    Raises:
+
+    """
     nodes, edges = connector.get_nodes_and_edges()
 
     return nodes, edges
 
 
 def update_server(client: BaseClient, api_key: str, namespace: str = "default") -> None:
+    """
+
+    Args:
+        client (BaseClient):
+        api_key (str):
+        namespace (str, optional):  (Default value = "default")
+
+    Returns:
+
+    Raises:
+
+    """
     conn = DbtCloudConnector(
         namespace=namespace,
         api_key=api_key,
     )
     nodes, edges = get_nodes_and_edges(conn, client.id)
 
     update(client, nodes)
```

### Comparing `grai_source_dbt_cloud-0.0.3a3/PKG-INFO` & `grai_source_dbt_cloud-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grai-source-dbt-cloud
-Version: 0.0.3a3
+Version: 0.0.4
 Summary: 
 Home-page: https://www.grai.io/
 License: Elastic-2.0
 Author: Edward Louth
 Author-email: edward@grai.io
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
```

