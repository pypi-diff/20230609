# Comparing `tmp/ms_salesforce_api-0.0.42.tar.gz` & `tmp/ms_salesforce_api-0.0.43.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ms_salesforce_api-0.0.42.tar", max compression
+gzip compressed data, was "ms_salesforce_api-0.0.43.tar", max compression
```

## Comparing `ms_salesforce_api-0.0.42.tar` & `ms_salesforce_api-0.0.43.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0    35149 2023-06-06 09:12:49.418744 ms_salesforce_api-0.0.42/LICENSE
--rw-r--r--   0        0        0     5635 2023-06-06 09:12:49.418744 ms_salesforce_api-0.0.42/README.md
--rw-r--r--   0        0        0        0 2023-06-06 09:12:49.418744 ms_salesforce_api-0.0.42/ms_salesforce_api/__init__.py
--rw-r--r--   0        0        0     1491 2023-06-06 09:12:49.418744 ms_salesforce_api-0.0.42/ms_salesforce_api/salesforce/Auth.py
--rw-r--r--   0        0        0      982 2023-06-06 09:12:49.418744 ms_salesforce_api-0.0.42/ms_salesforce_api/salesforce/JWTGenerator.py
--rw-r--r--   0        0        0     2714 2023-06-06 09:12:49.418744 ms_salesforce_api-0.0.42/ms_salesforce_api/salesforce/SalesforceQueryExecutor.py
--rw-r--r--   0        0        0        0 2023-06-06 09:12:49.418744 ms_salesforce_api-0.0.42/ms_salesforce_api/salesforce/__init__.py
--rw-r--r--   0        0        0        0 2023-06-06 09:12:49.418744 ms_salesforce_api-0.0.42/ms_salesforce_api/salesforce/__tests__/__init__.py
--rw-r--r--   0        0        0     2749 2023-06-06 09:12:49.418744 ms_salesforce_api-0.0.42/ms_salesforce_api/salesforce/__tests__/test_Auth.py
--rw-r--r--   0        0        0     2395 2023-06-06 09:12:49.418744 ms_salesforce_api-0.0.42/ms_salesforce_api/salesforce/__tests__/test_JWTGenerator.py
--rw-r--r--   0        0        0     5168 2023-06-06 09:12:49.418744 ms_salesforce_api-0.0.42/ms_salesforce_api/salesforce/__tests__/test_SalesforceRequester.py
--rw-r--r--   0        0        0     3318 2023-06-06 09:12:49.422744 ms_salesforce_api-0.0.42/ms_salesforce_api/salesforce/project/__init__.py
--rw-r--r--   0        0        0        0 2023-06-06 09:12:49.422744 ms_salesforce_api-0.0.42/ms_salesforce_api/salesforce/project/__tests__/__init__.py
--rw-r--r--   0        0        0    15428 2023-06-06 09:12:49.422744 ms_salesforce_api-0.0.42/ms_salesforce_api/salesforce/project/__tests__/test_Project.py
--rw-r--r--   0        0        0     2082 2023-06-06 09:12:49.422744 ms_salesforce_api-0.0.42/ms_salesforce_api/salesforce/project/constants.py
--rw-r--r--   0        0        0     3804 2023-06-06 09:12:49.422744 ms_salesforce_api-0.0.42/ms_salesforce_api/salesforce/project/dto/BillingLineDTO.py
--rw-r--r--   0        0        0     8063 2023-06-06 09:12:49.422744 ms_salesforce_api-0.0.42/ms_salesforce_api/salesforce/project/dto/OpportunityDTO.py
--rw-r--r--   0        0        0     2166 2023-06-06 09:12:49.422744 ms_salesforce_api-0.0.42/ms_salesforce_api/salesforce/project/dto/ProjectLineItemDTO.py
--rw-r--r--   0        0        0        0 2023-06-06 09:12:49.422744 ms_salesforce_api-0.0.42/ms_salesforce_api/salesforce/project/dto/__init__.py
--rw-r--r--   0        0        0    12544 2023-06-06 09:12:49.422744 ms_salesforce_api-0.0.42/ms_salesforce_api/salesforce/project/export_data/Bigquery.py
--rw-r--r--   0        0        0     5148 2023-06-06 09:12:49.422744 ms_salesforce_api-0.0.42/ms_salesforce_api/salesforce/project/export_data/CloudSQL.py
--rw-r--r--   0        0        0        0 2023-06-06 09:12:49.422744 ms_salesforce_api-0.0.42/ms_salesforce_api/salesforce/project/export_data/__init__.py
--rw-r--r--   0        0        0        0 2023-06-06 09:12:49.422744 ms_salesforce_api-0.0.42/ms_salesforce_api/salesforce/project/export_data/__tests__/__init__.py
--rw-r--r--   0        0        0    14583 2023-06-06 09:12:49.422744 ms_salesforce_api-0.0.42/ms_salesforce_api/salesforce/project/export_data/__tests__/test_Bigquery.py
--rw-r--r--   0        0        0    13715 2023-06-06 09:12:49.422744 ms_salesforce_api-0.0.42/ms_salesforce_api/salesforce/project/export_data/__tests__/test_CloudSQL.py
--rw-r--r--   0        0        0     1056 2023-06-06 09:12:49.422744 ms_salesforce_api-0.0.42/pyproject.toml
--rw-r--r--   0        0        0     6412 1970-01-01 00:00:00.000000 ms_salesforce_api-0.0.42/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-09 10:48:31.524528 ms_salesforce_api-0.0.43/LICENSE
+-rw-r--r--   0        0        0     5635 2023-06-09 10:48:31.524528 ms_salesforce_api-0.0.43/README.md
+-rw-r--r--   0        0        0        0 2023-06-09 10:48:31.524528 ms_salesforce_api-0.0.43/ms_salesforce_api/__init__.py
+-rw-r--r--   0        0        0     1491 2023-06-09 10:48:31.524528 ms_salesforce_api-0.0.43/ms_salesforce_api/salesforce/Auth.py
+-rw-r--r--   0        0        0      982 2023-06-09 10:48:31.524528 ms_salesforce_api-0.0.43/ms_salesforce_api/salesforce/JWTGenerator.py
+-rw-r--r--   0        0        0     2712 2023-06-09 10:48:31.524528 ms_salesforce_api-0.0.43/ms_salesforce_api/salesforce/SalesforceQueryExecutor.py
+-rw-r--r--   0        0        0        0 2023-06-09 10:48:31.524528 ms_salesforce_api-0.0.43/ms_salesforce_api/salesforce/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-09 10:48:31.524528 ms_salesforce_api-0.0.43/ms_salesforce_api/salesforce/__tests__/__init__.py
+-rw-r--r--   0        0        0     2749 2023-06-09 10:48:31.524528 ms_salesforce_api-0.0.43/ms_salesforce_api/salesforce/__tests__/test_Auth.py
+-rw-r--r--   0        0        0     2395 2023-06-09 10:48:31.524528 ms_salesforce_api-0.0.43/ms_salesforce_api/salesforce/__tests__/test_JWTGenerator.py
+-rw-r--r--   0        0        0     5168 2023-06-09 10:48:31.524528 ms_salesforce_api-0.0.43/ms_salesforce_api/salesforce/__tests__/test_SalesforceRequester.py
+-rw-r--r--   0        0        0     3347 2023-06-09 10:48:31.524528 ms_salesforce_api-0.0.43/ms_salesforce_api/salesforce/project/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-09 10:48:31.524528 ms_salesforce_api-0.0.43/ms_salesforce_api/salesforce/project/__tests__/__init__.py
+-rw-r--r--   0        0        0    15436 2023-06-09 10:48:31.524528 ms_salesforce_api-0.0.43/ms_salesforce_api/salesforce/project/__tests__/test_Project.py
+-rw-r--r--   0        0        0     3055 2023-06-09 10:48:31.524528 ms_salesforce_api-0.0.43/ms_salesforce_api/salesforce/project/constants.py
+-rw-r--r--   0        0        0     3804 2023-06-09 10:48:31.524528 ms_salesforce_api-0.0.43/ms_salesforce_api/salesforce/project/dto/BillingLineDTO.py
+-rw-r--r--   0        0        0    19325 2023-06-09 10:48:31.524528 ms_salesforce_api-0.0.43/ms_salesforce_api/salesforce/project/dto/OpportunityDTO.py
+-rw-r--r--   0        0        0     2166 2023-06-09 10:48:31.524528 ms_salesforce_api-0.0.43/ms_salesforce_api/salesforce/project/dto/ProjectLineItemDTO.py
+-rw-r--r--   0        0        0        0 2023-06-09 10:48:31.524528 ms_salesforce_api-0.0.43/ms_salesforce_api/salesforce/project/dto/__init__.py
+-rw-r--r--   0        0        0    20751 2023-06-09 10:48:31.524528 ms_salesforce_api-0.0.43/ms_salesforce_api/salesforce/project/export_data/Bigquery.py
+-rw-r--r--   0        0        0     6021 2023-06-09 10:48:31.524528 ms_salesforce_api-0.0.43/ms_salesforce_api/salesforce/project/export_data/CloudSQL.py
+-rw-r--r--   0        0        0        0 2023-06-09 10:48:31.524528 ms_salesforce_api-0.0.43/ms_salesforce_api/salesforce/project/export_data/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-09 10:48:31.524528 ms_salesforce_api-0.0.43/ms_salesforce_api/salesforce/project/export_data/__tests__/__init__.py
+-rw-r--r--   0        0        0    17775 2023-06-09 10:48:31.524528 ms_salesforce_api-0.0.43/ms_salesforce_api/salesforce/project/export_data/__tests__/test_Bigquery.py
+-rw-r--r--   0        0        0    13715 2023-06-09 10:48:31.524528 ms_salesforce_api-0.0.43/ms_salesforce_api/salesforce/project/export_data/__tests__/test_CloudSQL.py
+-rw-r--r--   0        0        0     1056 2023-06-09 10:48:31.524528 ms_salesforce_api-0.0.43/pyproject.toml
+-rw-r--r--   0        0        0     6412 1970-01-01 00:00:00.000000 ms_salesforce_api-0.0.43/PKG-INFO
```

### Comparing `ms_salesforce_api-0.0.42/LICENSE` & `ms_salesforce_api-0.0.43/LICENSE`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-0.0.42/README.md` & `ms_salesforce_api-0.0.43/README.md`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-0.0.42/ms_salesforce_api/salesforce/Auth.py` & `ms_salesforce_api-0.0.43/ms_salesforce_api/salesforce/Auth.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-0.0.42/ms_salesforce_api/salesforce/JWTGenerator.py` & `ms_salesforce_api-0.0.43/ms_salesforce_api/salesforce/JWTGenerator.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-0.0.42/ms_salesforce_api/salesforce/SalesforceQueryExecutor.py` & `ms_salesforce_api-0.0.43/ms_salesforce_api/salesforce/SalesforceQueryExecutor.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,18 +41,16 @@
             logging.error("Authentication failed, cannot fetch data")
             return None
 
         headers = {"Authorization": f"Bearer {self.access_token}"}
 
         all_records = []
         next_url = f"{self.endpoint}?q={query}"
-
         while next_url:
             response = self._make_request(next_url, headers, 0)
-
             if response:
                 data = response.json()
                 all_records.extend(data.get("records", []))
                 nextRecordsUrl = data.get("nextRecordsUrl", None)
                 if nextRecordsUrl:
                     next_url = f"{self.domain}{nextRecordsUrl}"
                 else:
```

### Comparing `ms_salesforce_api-0.0.42/ms_salesforce_api/salesforce/__tests__/test_Auth.py` & `ms_salesforce_api-0.0.43/ms_salesforce_api/salesforce/__tests__/test_Auth.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-0.0.42/ms_salesforce_api/salesforce/__tests__/test_JWTGenerator.py` & `ms_salesforce_api-0.0.43/ms_salesforce_api/salesforce/__tests__/test_JWTGenerator.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-0.0.42/ms_salesforce_api/salesforce/__tests__/test_SalesforceRequester.py` & `ms_salesforce_api-0.0.43/ms_salesforce_api/salesforce/__tests__/test_SalesforceRequester.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-0.0.42/ms_salesforce_api/salesforce/project/__init__.py` & `ms_salesforce_api-0.0.43/ms_salesforce_api/salesforce/project/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,15 +63,16 @@
 
             with ThreadPoolExecutor(max_workers=10) as executor:
                 for project_id_batch in self.get_batches(
                     project_ids, MAX_PROJECT_IDS_PER_QUERY
                 ):
                     batch_results = list(
                         executor.map(
-                            self.fetch_billing_lines, [project_id_batch]
+                            self.fetch_billing_lines,
+                            [project_id_batch],
                         )
                     )
                     for billing_line_data in batch_results:
                         for record in billing_line_data:
                             billing_line_dto = (
                                 BillingLineDTO.from_salesforce_record(record)
                             )
```

### Comparing `ms_salesforce_api-0.0.42/ms_salesforce_api/salesforce/project/__tests__/test_Project.py` & `ms_salesforce_api-0.0.43/ms_salesforce_api/salesforce/project/__tests__/test_Project.py`

 * *Files 1% similar despite different names*

```diff
@@ -289,15 +289,15 @@
             opportunity["created_at"], "2020-07-14T12:55:56.000+0000"
         )
         self.assertEqual(
             opportunity["last_updated_at"], "2023-05-16T13:18:04.000+0000"
         )
         self.assertEqual(opportunity["opportunity_name"], "ESMOPP")
         self.assertEqual(opportunity["stage"], "Qualification")
-        self.assertEqual(opportunity["billing_country"], "ES")
+        self.assertEqual(opportunity["account_billing_country"], "ES")
         self.assertEqual(opportunity["lead_source"], "Other")
         self.assertEqual(opportunity["project_code"], "ESMSEX00430")
         self.assertEqual(opportunity["project_id"], "a003X000015kaPxQAI")
         self.assertEqual(opportunity["project_name"], "ESMProject")
         self.assertEqual(opportunity["project_start_date"], "2023-05-13")
         self.assertEqual(
             opportunity["controller_email"], "jhon.doe@ext.makingscience.com"
```

### Comparing `ms_salesforce_api-0.0.42/ms_salesforce_api/salesforce/project/dto/BillingLineDTO.py` & `ms_salesforce_api-0.0.43/ms_salesforce_api/salesforce/project/dto/BillingLineDTO.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-0.0.42/ms_salesforce_api/salesforce/project/dto/ProjectLineItemDTO.py` & `ms_salesforce_api-0.0.43/ms_salesforce_api/salesforce/project/dto/ProjectLineItemDTO.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-0.0.42/ms_salesforce_api/salesforce/project/export_data/Bigquery.py` & `ms_salesforce_api-0.0.43/ms_salesforce_api/salesforce/project/export_data/__tests__/test_CloudSQL.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,315 +1,356 @@
-from urllib.parse import quote
+import unittest
+from unittest.mock import MagicMock, patch
 
-from gc_google_services_api.bigquery import BigQueryManager
+from psycopg2 import sql
 
+from ..CloudSQL import CloudSQL
 
-class BigQueryExporter:
-    def __init__(self, project_id, dataset_id):
-        self.project_id = project_id
-        self.dataset_id = dataset_id
-        self.client = BigQueryManager(
-            project_id=project_id, dataset_id=dataset_id
-        )
-        self.batch_size = 200
-        self.schemas = {
-            "last_executed_at": {
-                "last_executed_at": "TIMESTAMP",
-            },
-            "opportunities": {
-                "client_fiscal_name": "STRING",
-                "client_account_name": "STRING",
-                "currency": "STRING",
-                "amount": "FLOAT",
-                "invoicing_country_code": "STRING",
-                "operation_coordinator_email": "STRING",
-                "operation_coordinator_sub_email": "STRING",
-                "created_at": "TIMESTAMP",
-                "last_updated_at": "TIMESTAMP",
-                "opportunity_name": "STRING",
-                "stage": "STRING",
-                "billing_country": "STRING",
-                "lead_source": "STRING",
-                "project_code": "STRING",
-                "project_id": "STRING",
-                "project_name": "STRING",
-                "project_start_date": "DATE",
-                "controller_email": "STRING",
-                "controller_sub_email": "STRING",
-                "profit_center": "STRING",
-                "cost_center": "STRING",
-                "project_tier": "STRING",
-                "jira_task_url": "STRING",
-                "opportunity_percentage": "STRING",
-            },
-            "billing_lines": {
-                "id": "STRING",
-                "project_id": "STRING",
-                "name": "STRING",
-                "currency": "STRING",
-                "created_date": "TIMESTAMP",
-                "last_modified_date": "TIMESTAMP",
-                "billing_amount": "FLOAT",
-                "billing_date": "DATE",
-                "billing_period_ending_date": "DATE",
-                "billing_period_starting_date": "DATE",
-                "hourly_price": "FLOAT",
-                "revenue_dedication": "FLOAT",
-                "billing_plan_amount": "STRING",
-                "billing_plan_billing_date": "DATE",
-                "billing_plan_item": "STRING",
-                "billing_plan_service_end_date": "DATE",
-                "billing_plan_service_start_date": "DATE",
-            },
-            "project_line_items": {
-                "country": "STRING",
-                "project_id": "STRING",
-                "created_date": "TIMESTAMP",
-                "effort": "STRING",
-                "ending_date": "DATE",
-                "id": "STRING",
-                "last_modified_date": "TIMESTAMP",
-                "ms_pli_name": "STRING",
-                "product_name": "STRING",
-                "quantity": "FLOAT",
-                "starting_date": "DATE",
-                "total_price": "STRING",
-                "unit_price": "STRING",
-            },
-        }
-
-        for table_name, table_schema in self.schemas.items():
-            self.client.create_table_if_not_exists(table_name, table_schema)
-
-    def _export_opportunities(self, opportunities):
-        opportunities_values = []
-        for opp in opportunities:
-            project_start_date = (
-                f'DATE "{opp["project_start_date"]}"'
-                if opp["project_start_date"]
-                else "NULL"
-            )
-            profit_center = (
-                f'"{opp["profit_center"]}"' if opp["profit_center"] else "NULL"
-            )
-            cost_center = (
-                f'"{opp["cost_center"]}"' if opp["cost_center"] else "NULL"
-            )
-
-            opportunities_values.append(
-                f"""
-                (
-                    "{opp['client_fiscal_name']}",
-                    "{opp['client_account_name']}",
-                    "{opp['currency']}",
-                    {opp['amount']},
-                    "{opp['invoicing_country_code']}",
-                    "{opp['operation_coordinator_email']}",
-                    "{opp['operation_coordinator_sub_email']}",
-                    TIMESTAMP "{opp['created_at']}",
-                    TIMESTAMP "{opp['last_updated_at']}",
-                    "{opp['opportunity_name']}",
-                    "{opp['stage']}",
-                    "{opp['billing_country']}",
-                    "{opp['lead_source']}",
-                    "{opp['project_code']}",
-                    "{opp['project_id']}",
-                    "{opp['project_name']}",
-                    {project_start_date},
-                    "{opp['controller_email']}",
-                    "{opp['controller_sub_email']}",
-                    {profit_center},
-                    {cost_center},
-                    "{opp['project_tier']}",
-                    "{quote(opp['jira_task_url'], safe='s')}",
-                   "{opp['opportunity_percentage']}"
-                )
+
+def compare_queries(query_strings, expected_queries):
+    for query_string, expected_query in zip(query_strings, expected_queries):
+        if not compare_query(query_string, expected_query):
+            return False
+    return True
+
+
+def compare_query(query_string, expected_query):
+    expected_elements = get_elements(expected_query)
+    for element in expected_elements:
+        if element not in query_string:
+            return False
+    return True
+
+
+def get_elements(query):
+    elements = []
+    if isinstance(query, str):
+        elements.append(query)
+    elif isinstance(query, tuple):
+        for item in query:
+            elements.extend(get_elements(item))
+    elif isinstance(query, list):
+        for sublist in query:
+            elements.extend(get_elements(sublist))
+    return elements
+
+
+class TestCloudSQL(unittest.TestCase):
+    def setUp(self):
+        mock_cursor = MagicMock()
+        mock_cursor.__enter__.return_value = mock_cursor
+
+        mock_connection = MagicMock()
+        mock_connection.cursor.return_value = mock_cursor
+
+        mock_connect = MagicMock(return_value=mock_connection)
+
+        with patch("psycopg2.connect", mock_connect):
+            self.cloudsql = CloudSQL("host", "user", "password", "dbname")
+
+    @patch("psycopg2.connect")
+    def test_export_data(self, mock_connect):
+        mock_connection = mock_connect.return_value
+        mock_cursor = mock_connection.cursor.return_value
+
+        opportunities = [
+            {
+                "client_fiscal_name": "ESMProjectAcc",
+                "client_account_name": "ESMProjectAccount",
+                "currency": "EUR",
+                "amount": 0,
+                "invoicing_country_code": "ES",
+                "operation_coordinator_email": "test@test.com",
+                "operation_coordinator_sub_email": "test@test.com",
+                "created_at": "2020-07-14T12:55:56.000+0000",
+                "last_updated_at": "2023-05-16T13:18:04.000+0000",
+                "opportunity_name": "ESMOPP",
+                "stage": "Qualification",
+                "billing_country": "ES",
+                "lead_source": "Other",
+                "project_code": "ESMSEX00430",
+                "project_id": "a003X000015kaPxQAI",
+                "project_name": "ESMProject",
+                "project_start_date": "2023-05-13",
+                "controller_email": "test@test.com",
+                "controller_sub_email": "test@test.com",
+                "profit_center": None,
+                "cost_center": None,
+                "project_tier": "Unknown",
+                "jira_task_url": "ESMSBD0001-11848",
+                "opportunity_percentage": 10.0,
+                "billing_lines": [
+                    {
+                        "id": "a0sAa0000004Lx7IAE",
+                        "project_id": "a003X000015kaPxQAI",
+                        "name": "BL-000320965",
+                        "currency": "EUR",
+                        "created_date": "2023-05-13T09:04:20.000+0000",
+                        "last_modified_date": "2023-05-16T13:18:01.000+0000",
+                        "billing_amount": 90.0,
+                        "billing_date": "2023-05-13",
+                        "billing_period_ending_date": "2023-05-27",
+                        "billing_period_starting_date": "2023-05-13",
+                        "hourly_price": None,
+                        "revenue_dedication": None,
+                        "billing_plan_amount": "90",
+                        "billing_plan_billing_date": "2023-05-13",
+                        "billing_plan_item": "12345",
+                        "billing_plan_service_end_date": "2023-05-27",
+                        "billing_plan_service_start_date": "2023-05-13",
+                    }
+                ],
+                "project_line_items": [
+                    {
+                        "country": "Spain",
+                        "created_date": "2023-05-13T09:03:14.000+0000",
+                        "effort": "12",
+                        "ending_date": "2023-05-27",
+                        "id": "a0VAa000000fWbdMAE",
+                        "last_modified_date": "2023-05-16T13:18:01.000+0000",
+                        "ms_pli_name": "_MSEX00430",
+                        "product_name": "ESM PRODUCT",
+                        "quantity": 12.0,
+                        "starting_date": "2023-05-13",
+                        "total_price": 1080.0,
+                        "unit_price": 90.0,
+                    }
+                ],
+            }
+        ]
+
+        opportunity_fixed = [
+            {
+                "opportunity_name": "ESMOPP",
+                "client_fiscal_name": "ESMProjectAcc",
+                "client_account_name": "ESMProjectAccount",
+                "currency": "EUR",
+                "amount": 0,
+                "invoicing_country_code": "ES",
+                "operation_coordinator_email": "test@test.com",
+                "operation_coordinator_sub_email": "test@test.com",
+                "created_at": "2020-07-14T12:55:56.000+0000",
+                "last_updated_at": "2023-05-16T13:18:04.000+0000",
+                "stage": "Qualification",
+                "billing_country": "ES",
+                "lead_source": "Other",
+                "project_code": "ESMSEX00430",
+                "project_id": "a003X000015kaPxQAI",
+                "project_name": "ESMProject",
+                "project_start_date": "2023-05-13",
+                "controller_email": "test@test.com",
+                "controller_sub_email": "test@test.com",
+                "profit_center": None,
+                "cost_center": None,
+                "project_tier": "Unknown",
+                "jira_task_url": "ESMSBD0001-11848",
+                "opportunity_percentage": 10.0,
+            }
+        ]
+        billing_fixed = [
+            {
+                "id": "BL-000320965",
+                "project_id": "a003X000015kaPxQAI",
+                "name": "Billing Line 1",
+                "currency": "EUR",
+                "created_date": "2023-05-13T09:04:20.000+0000",
+                "last_modified_date": "2023-05-16T13:18:01.000+0000",
+                "billing_amount": 90.0,
+                "billing_date": "2023-05-13",
+                "billing_period_ending_date": "2023-05-27",
+                "billing_period_starting_date": "2023-05-13",
+                "hourly_price": None,
+                "revenue_dedication": None,
+                "billing_plan_amount": "90",
+                "billing_plan_billing_date": "2023-05-13",
+                "billing_plan_item": "12345",
+                "billing_plan_service_end_date": "2023-05-27",
+                "billing_plan_service_start_date": "2023-05-13",
+            }
+        ]
+
+        project_fixed = [
+            {
+                "country": "Spain",
+                "created_date": "2023-05-13T09:03:14.000+0000",
+                "effort": "12",
+                "ending_date": "2023-05-27",
+                "id": "a0VAa000000fWbdMAE",
+                "last_modified_date": "2023-05-16T13:18:01.000+0000",
+                "ms_pli_name": "_MSEX00430",
+                "product_name": "ESM PRODUCT",
+                "quantity": 12.0,
+                "starting_date": "2023-05-13",
+                "total_price": 1080.0,
+                "unit_price": 90.0,
+                "project_id": "a003X000015kaPxQAI",
+            }
+        ]
+
+        mock_cursor = MagicMock()
+        mock_cursor.__enter__.return_value = mock_cursor
+
+        mock_connection = MagicMock()
+        mock_connection.cursor.return_value = mock_cursor
+
+        mock_connect = MagicMock(return_value=mock_connection)
+
+        with patch("psycopg2.connect", mock_connect):
+            cloudsql = CloudSQL("host", "user", "password", "dbname")
+            cloudsql.export_data(opportunities)
+
+        mock_cursor.executemany.assert_called()
+        self.assertEqual(
+            mock_cursor.executemany.call_count, 3
+        )  # 3 tables: Opportunities, BillingLines, ProjectLine
+
+        queries = [
+            sql.SQL(str(call[0][0]))
+            for call in mock_cursor.executemany.call_args_list
+        ]
+        query_strings = [
+            query.as_string(mock_cursor.executemany.call_args[0][1])
+            for query in queries
+        ]
+
+        expected_queries = [
+            sql.SQL(
                 """
-            )
-        if opportunities_values:
-            insert_opportunities_query = f"""
-                INSERT INTO `{self.project_id}.{self.dataset_id}.opportunities` (
-                    client_fiscal_name,
-                    client_account_name,
-                    currency,
-                    amount,
-                    invoicing_country_code,
-                    operation_coordinator_email,
-                    operation_coordinator_sub_email,
-                    created_at,
-                    last_updated_at,
-                    opportunity_name,
-                    stage,
-                    billing_country,
-                    lead_source,
-                    project_code,
-                    project_id,
-                    project_name,
-                    project_start_date,
-                    controller_email,
-                    controller_sub_email,
-                    profit_center,
-                    cost_center,
-                    project_tier,
-                    jira_task_url,
-                    opportunity_percentage
-                ) VALUES {', '.join(opportunities_values)};
-            """
-            self.client.execute_query(insert_opportunities_query, None)
-
-    def _export_billing_lines(self, opportunities):
-        billing_lines_values = []
-        for opp in opportunities:
-            for bl in opp["billing_lines"]:
-                billing_date = (
-                    f'DATE "{bl["billing_date"]}"'
-                    if bl["billing_date"]
-                    else "NULL"
-                )
-                billing_period_ending_date = (
-                    f'DATE "{bl["billing_period_ending_date"]}"'
-                    if bl["billing_period_ending_date"]
-                    else "NULL"
-                )
-                billing_period_starting_date = (
-                    f'DATE "{bl["billing_period_starting_date"]}"'
-                    if bl["billing_period_starting_date"]
-                    else "NULL"
-                )
-                billing_plan_billing_date = (
-                    f'DATE "{bl["billing_plan_billing_date"]}"'
-                    if bl["billing_plan_billing_date"]
-                    else "NULL"
-                )
-                billing_plan_service_end_date = (
-                    f'DATE "{bl["billing_plan_service_end_date"]}"'
-                    if bl["billing_plan_service_end_date"]
-                    else "NULL"
-                )
-                billing_plan_service_start_date = (
-                    f'DATE "{bl["billing_plan_service_start_date"]}"'
-                    if bl["billing_plan_service_start_date"]
-                    else "NULL"
-                )
-
-                billing_lines_values.append(
-                    f"""
-                    (
-                        "{bl['id']}",
-                        "{bl['project_id']}",
-                        "{bl['name']}",
-                        "{bl['currency']}",
-                        TIMESTAMP "{bl['created_date']}",
-                        TIMESTAMP "{bl['last_modified_date']}",
-                        {bl['billing_amount']},
-                        {billing_date},
-                        {billing_period_ending_date},
-                        {billing_period_starting_date},
-                        {bl['hourly_price'] if bl['hourly_price'] else 'NULL'},
-                        {bl['revenue_dedication'] if bl['revenue_dedication'] else 'NULL'},
-                        "{bl['billing_plan_amount']}",
-                        {billing_plan_billing_date},
-                        "{bl['billing_plan_item']}",
-                        {billing_plan_service_end_date},
-                        {billing_plan_service_start_date}
-                    )
-                    """
-                )
-        if billing_lines_values:
-            insert_billing_lines_query = f"""
-                INSERT INTO `{self.project_id}.{self.dataset_id}.billing_lines` (
-                    id,
-                    project_id,
-                    name,
-                    currency,
-                    created_date,
-                    last_modified_date,
-                    billing_amount,
-                    billing_date,
-                    billing_period_ending_date,
-                    billing_period_starting_date,
-                    hourly_price,
-                    revenue_dedication,
-                    billing_plan_amount,
-                    billing_plan_billing_date,
-                    billing_plan_item,
-                    billing_plan_service_end_date,
-                    billing_plan_service_start_date
-                ) VALUES {', '.join(billing_lines_values)};
-            """
-
-            self.client.execute_query(insert_billing_lines_query, None)
-
-    def _export_PLIs(self, opportunities):
-        project_line_items_values = []
-        for opp in opportunities:
-            project_id = opp["project_id"]
-            for pli in opp["project_line_items"]:
-                effort = f"{pli['effort']}" if pli["effort"] else "NULL"
-                total_price = (
-                    f"{pli['total_price']}" if pli["total_price"] else "NULL"
-                )
-                unit_price = (
-                    f"{pli['unit_price']}" if pli["unit_price"] else "NULL"
-                )
-                ending_date = (
-                    f'DATE "{pli["ending_date"]}"'
-                    if pli["ending_date"]
-                    else "NULL"
-                )
-                starting_date = (
-                    f'DATE "{pli["starting_date"]}"'
-                    if pli["starting_date"]
-                    else "NULL"
-                )
-
-                project_line_items_values.append(
-                    f"""
-                    (
-                        "{pli['country']}",
-                        TIMESTAMP "{pli['created_date']}",
-                        "{effort}",
-                        {ending_date},
-                        "{pli['id']}",
-                        TIMESTAMP "{pli['last_modified_date']}",
-                        "{pli['ms_pli_name']}",
-                        "{pli['product_name']}",
-                        {pli['quantity'] if pli['quantity'] else 0.0},
-                        {starting_date},
-                        "{total_price}",
-                        "{unit_price}",
-                        "{project_id}"
+                INSERT INTO Opportunities ({})
+                VALUES ({})
+                """
+            ).format(
+                sql.SQL(", ").join(
+                    map(sql.Identifier, opportunity_fixed[0].keys())
+                ),
+                sql.SQL(", ").join(
+                    map(
+                        lambda x: sql.Placeholder(),
+                        opportunity_fixed[0].keys(),
                     )
-                    """
-                )
+                ),
+            ),
+            sql.SQL(
+                """
+                INSERT INTO BillingLines ({})
+                VALUES ({})
+                """
+            ).format(
+                sql.SQL(", ").join(
+                    map(sql.Identifier, billing_fixed[0].keys())
+                ),
+                sql.SQL(", ").join(
+                    map(lambda x: sql.Placeholder(), billing_fixed[0].keys())
+                ),
+            ),
+            sql.SQL(
+                """
+                INSERT INTO ProjectLine ({})
+                VALUES ({})
+                """
+            ).format(
+                sql.SQL(", ").join(
+                    map(sql.Identifier, project_fixed[0].keys())
+                ),
+                sql.SQL(", ").join(
+                    map(lambda x: sql.Placeholder(), project_fixed[0].keys())
+                ),
+            ),
+        ]
 
-        if project_line_items_values:
-            insert_project_line_items_query = f"""
-                INSERT INTO `{self.project_id}.{self.dataset_id}.project_line_items` (
-                    country,
-                    created_date,
-                    effort,
-                    ending_date,
-                    id,
-                    last_modified_date,
-                    ms_pli_name,
-                    product_name,
-                    quantity,
-                    starting_date,
-                    total_price,
-                    unit_price,
-                    project_id
-                ) VALUES {', '.join(project_line_items_values)};
-            """
-            self.client.execute_query(insert_project_line_items_query, None)
-
-    def export_data(self, opportunities):
-        opportunities_batches = [
-            opportunities[i : i + self.batch_size]  # noqa: E203
-            for i in range(0, len(opportunities), self.batch_size)
+        result = compare_queries(query_strings, expected_queries)
+
+        self.assertEqual(result, True)
+
+    def test_create_batches(self):
+        data = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
+        batch_size = 3
+        expected_batches = [[1, 2, 3], [4, 5, 6], [7, 8, 9], [10]]
+
+        batches = self.cloudsql._create_batches(data, batch_size)
+        self.assertEqual(batches, expected_batches)
+
+    def test_create_billing_lines(self):
+        billing_lines = [
+            {
+                "id": "a0sAa0000004Lx7IAE",
+                "name": "BL-000320965",
+                "currency": "EUR",
+                "created_date": "2023-05-13T09:04:20.000+0000",
+                "last_modified_date": "2023-05-16T13:18:01.000+0000",
+                "billing_amount": 90.0,
+                "billing_date": "2023-05-13",
+                "billing_period_ending_date": "2023-05-27",
+                "billing_period_starting_date": "2023-05-13",
+                "hourly_price": None,
+                "revenue_dedication": None,
+                "billing_plan_amount": "90",
+                "billing_plan_billing_date": "2023-05-13",
+                "billing_plan_item": "12345",
+                "billing_plan_service_end_date": "2023-05-27",
+                "billing_plan_service_start_date": "2023-05-13",
+            }
+        ]
+        project_id = "a003X000015kaPxQAI"
+        expected_billing_lines = [
+            {
+                "id": "a0sAa0000004Lx7IAE",
+                "project_id": "a003X000015kaPxQAI",
+                "name": "BL-000320965",
+                "currency": "EUR",
+                "created_date": "2023-05-13T09:04:20.000+0000",
+                "last_modified_date": "2023-05-16T13:18:01.000+0000",
+                "billing_amount": 90.0,
+                "billing_date": "2023-05-13",
+                "billing_period_ending_date": "2023-05-27",
+                "billing_period_starting_date": "2023-05-13",
+                "hourly_price": None,
+                "revenue_dedication": None,
+                "billing_plan_amount": "90",
+                "billing_plan_billing_date": "2023-05-13",
+                "billing_plan_item": "12345",
+                "billing_plan_service_end_date": "2023-05-27",
+                "billing_plan_service_start_date": "2023-05-13",
+            }
         ]
-        for batch in opportunities_batches:
-            self._export_opportunities(batch)
 
-            self._export_billing_lines(batch)
+        result = self.cloudsql._create_billing_lines(billing_lines, project_id)
+        self.assertEqual(result, expected_billing_lines)
+
+    def test_create_project_lines(self):
+        project_lines = [
+            {
+                "country": "Spain",
+                "created_date": "2023-05-13T09:03:14.000+0000",
+                "effort": "12",
+                "ending_date": "2023-05-27",
+                "id": "a0VAa000000fWbdMAE",
+                "last_modified_date": "2023-05-16T13:18:01.000+0000",
+                "ms_pli_name": "_MSEX00430",
+                "product_name": "ESM PRODUCT",
+                "quantity": 12.0,
+                "starting_date": "2023-05-13",
+                "total_price": 1080.0,
+                "unit_price": 90.0,
+            }
+        ]
+        project_id = "a003X000015kaPxQAI"
+        expected_project_lines = [
+            {
+                "country": "Spain",
+                "created_date": "2023-05-13T09:03:14.000+0000",
+                "effort": "12",
+                "ending_date": "2023-05-27",
+                "id": "a0VAa000000fWbdMAE",
+                "last_modified_date": "2023-05-16T13:18:01.000+0000",
+                "ms_pli_name": "_MSEX00430",
+                "product_name": "ESM PRODUCT",
+                "quantity": 12.0,
+                "starting_date": "2023-05-13",
+                "total_price": 1080.0,
+                "unit_price": 90.0,
+                "project_id": "a003X000015kaPxQAI",
+            }
+        ]
 
-            self._export_PLIs(batch)
+        result = self.cloudsql._create_project_lines(project_lines, project_id)
+        self.assertEqual(result, expected_project_lines)
```

### Comparing `ms_salesforce_api-0.0.42/ms_salesforce_api/salesforce/project/export_data/CloudSQL.py` & `ms_salesforce_api-0.0.43/ms_salesforce_api/salesforce/project/export_data/CloudSQL.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,21 +9,52 @@
 
 
 class CloudSQL:
     BATCH_SIZE = 200
 
     def __init__(self, host, user, password, dbname, debug_mode=False):
         self.debug_mode = debug_mode
+
+        self.check_and_create_database(host, user, password, dbname)
+
         self.connection = psycopg2.connect(
             host=host,
             user=user,
             password=password,
             dbname=dbname,
         )
 
+    def check_and_create_database(self, host, user, password, database):
+        conn = psycopg2.connect(
+            host=host,
+            user=user,
+            password=password,
+            dbname="postgres",
+        )
+
+        cursor = conn.cursor()
+
+        check_db_query = f"SELECT 1 FROM pg_catalog.pg_database WHERE datname = '{database}'"  # noqa: E501
+
+        cursor.execute(check_db_query)
+
+        result = cursor.fetchone()
+
+        if result is None:
+            logging.info(f"Creating database '{database}'...")
+            create_db_query = f"CREATE DATABASE {database}"
+            cursor.execute("COMMIT")
+            cursor.execute(create_db_query)
+            logging.info(f"Database '{database}' created.")
+
+        conn.commit()
+
+        cursor.close()
+        conn.close()
+
     def export_data(self, opportunities):
         with self.connection.cursor() as cursor:
             opportunity_batches = self._create_batches(
                 opportunities, self.BATCH_SIZE
             )
             for opportunity_batch in opportunity_batches:
                 self._insert_opportunities_batch(cursor, opportunity_batch)
```

### Comparing `ms_salesforce_api-0.0.42/ms_salesforce_api/salesforce/project/export_data/__tests__/test_Bigquery.py` & `ms_salesforce_api-0.0.43/ms_salesforce_api/salesforce/project/export_data/__tests__/test_Bigquery.py`

 * *Files 21% similar despite different names*

```diff
@@ -17,15 +17,14 @@
                 "invoicing_country_code": "ES",
                 "operation_coordinator_email": "test@test.com",
                 "operation_coordinator_sub_email": "test@test.com",
                 "created_at": "2020-07-14T12:55:56.000+0000",
                 "last_updated_at": "2023-05-16T13:18:04.000+0000",
                 "opportunity_name": "ESMOPP",
                 "stage": "Qualification",
-                "billing_country": "ES",
                 "lead_source": "Other",
                 "project_code": "ESMSEX00430",
                 "project_id": "a003X000015kaPxQAI",
                 "project_name": "ESMProject",
                 "project_start_date": "2023-05-13",
                 "controller_email": "test@test.com",
                 "controller_sub_email": "test@test.com",
@@ -67,14 +66,39 @@
                         "product_name": "ESM PRODUCT",
                         "quantity": 12.0,
                         "starting_date": "2023-05-13",
                         "total_price": 1080.0,
                         "unit_price": 90.0,
                     }
                 ],
+                "account_billing_country": "ES",
+                "account_assigment_group": None,
+                "account_tax_category": None,
+                "account_tax_classification": "0",
+                "account_txt_sapid": "10004171",
+                "account_business_function": "BP03",
+                "account_tax_id_type": "CA2",
+                "account_currency_code": "",
+                "account_created_date": "2023-02-15T09:27:46.000+0000",
+                "account_tier": "T1",
+                "account_pec_email": None,
+                "account_phone": None,
+                "account_fax": None,
+                "account_website": None,
+                "account_cif": "700812894RC0001",
+                "account_billing_address": "12 Strickland Avenue, Toronto, Ontario, M6K 2H8, Canada",  # noqa: E501
+                "account_billing_city": "Toronto",
+                "account_billing_postal_code": "M6K 2H8",
+                "account_billing_street": "12 Strickland Avenue",
+                "account_company_invoicing": "2411",
+                "account_office": "1313X000000Y5DEQA0",
+                "account_payment_terms": "T060",
+                "account_billing_state_code": "ON",
+                "account_mail_invoicing": None,
+                "account_invoicing_email": "test@5822.group",
             },
         ]
 
         self.mock_bigquery_manager = mock.patch(
             "gc_google_services_api.bigquery.BigQueryManager"
         ).start()
         from ..Bigquery import BigQueryExporter
@@ -85,51 +109,45 @@
         self.mock_bigquery_manager.reset_mock()
 
     def test_export_opportunities(self):
         self.exporter._export_opportunities(self.opportunities)
 
         expected_query = """
             INSERT INTO `your-project-id.your-dataset-id.opportunities` (
-                    client_fiscal_name,
-                    client_account_name,
                     currency,
                     amount,
                     invoicing_country_code,
                     operation_coordinator_email,
                     operation_coordinator_sub_email,
                     created_at,
                     last_updated_at,
                     opportunity_name,
                     stage,
-                    billing_country,
                     lead_source,
                     project_code,
                     project_id,
                     project_name,
                     project_start_date,
                     controller_email,
                     controller_sub_email,
                     profit_center,
                     cost_center,
                     project_tier,
                     jira_task_url,
                     opportunity_percentage
                 ) VALUES (
-                    "ESMProjectAcc",
-                    "ESMProjectAccount",
                     "EUR",
                     0,
                     "ES",
                     "test@test.com",
                     "test@test.com",
                     TIMESTAMP "2020-07-14T12:55:56.000+0000",
                     TIMESTAMP "2023-05-16T13:18:04.000+0000",
                     "ESMOPP",
                     "Qualification",
-                    "ES",
                     "Other",
                     "ESMSEX00430",
                     "a003X000015kaPxQAI",
                     "ESMProject",
                     DATE "2023-05-13",
                     "test@test.com",
                     "test@test.com",
@@ -253,51 +271,45 @@
         mock_client = mock.Mock()
         mock_bq_manager.return_value = mock_client
 
         self.exporter.export_data(self.opportunities)
 
         expected_opportunities_query = """
             INSERT INTO `your-project-id.your-dataset-id.opportunities` (
-                client_fiscal_name,
-                client_account_name,
                 currency,
                 amount,
                 invoicing_country_code,
                 operation_coordinator_email,
                 operation_coordinator_sub_email,
                 created_at,
                 last_updated_at,
                 opportunity_name,
                 stage,
-                billing_country,
                 lead_source,
                 project_code,
                 project_id,
                 project_name,
                 project_start_date,
                 controller_email,
                 controller_sub_email,
                 profit_center,
                 cost_center,
                 project_tier,
                 jira_task_url,
                 opportunity_percentage
             ) VALUES (
-                "ESMProjectAcc",
-                "ESMProjectAccount",
                 "EUR",
                 0,
                 "ES",
                 "test@test.com",
                 "test@test.com",
                 TIMESTAMP "2020-07-14T12:55:56.000+0000",
                 TIMESTAMP "2023-05-16T13:18:04.000+0000",
                 "ESMOPP",
                 "Qualification",
-                "ES",
                 "Other",
                 "ESMSEX00430",
                 "a003X000015kaPxQAI",
                 "ESMProject",
                 DATE "2023-05-13",
                 "test@test.com",
                 "test@test.com",
@@ -376,39 +388,120 @@
                 12.0,
                 DATE "2023-05-13",
                 "1080.0",
                 "90.0",
                 "a003X000015kaPxQAI"
             );
         """
+        expected_accounts_query = """
+            INSERT INTO `your-project-id.your-dataset-id.accounts` (
+                project_id,
+                name,
+                account_assigment_group,
+                tax_category,
+                tax_classification,
+                sap_id,
+                business_function,
+                tax_id_type,
+                currency_code,
+                created_date,
+                tier,
+                pec_email,
+                phone,
+                fax,
+                website,
+                cif,
+                billing_country_code,
+                business_name,
+                billing_address,
+                billing_city,
+                billing_postal_code,
+                billing_street,
+                company_invoicing,
+                office,
+                payment_terms,
+                billing_state_sode,
+                mail_invoicing,
+                invoicing_email
+            ) VALUES
+                (
+                    "a003X000015kaPxQAI",
+                    "ESMProjectAccount",
+                    NULL,
+                    NULL,
+                    "0",
+                    "10004171",
+                    "BP03",
+                    "CA2",
+                    NULL,
+                    "2023-02-15T09:27:46.000+0000",
+                    "T1",
+                    NULL,
+                    NULL,
+                    NULL,
+                    NULL,
+                    "700812894RC0001",
+                    "ES",
+                    "ESMProjectAcc",
+                    "12 Strickland Avenue, Toronto, Ontario, M6K 2H8, Canada",
+                    "Toronto",
+                    "M6K 2H8",
+                    "12 Strickland Avenue",
+                    "2411",
+                    "1313X000000Y5DEQA0",
+                    "T060",
+                    "ON",
+                    NULL,
+                    "test@5822.group"
+                )
+                ;
+        """
         execute_query_calls = self.exporter.client.execute_query.call_args_list
 
         expected_opportunities_query_stripped = re.sub(
             r"\s+", "", expected_opportunities_query
         )
+
         execute_opportunities_query_stripped = re.sub(
             r"\s+", "", str(execute_query_calls[1][0][0])
         )
 
         expected_billinglines_query_stripped = re.sub(
             r"\s+", "", expected_billing_lines_query
         )
+
         execute_billinglines_query_stripped = re.sub(
             r"\s+", "", str(execute_query_calls[0][0][0])
         )
 
         expected_pli_query_stripped = re.sub(r"\s+", "", expected_PLIs_query)
         execute_pli_query_stripped = re.sub(
             r"\s+", "", str(execute_query_calls[3][0][0])
         )
 
+        expected_accounts_query_stripped = re.sub(
+            r"\s+", "", expected_accounts_query
+        )
+
+        execute_accounts_query_stripped = re.sub(
+            r"\s+", "", str(execute_query_calls[4][0][0])
+        )
+
         self.assertEqual(
             execute_opportunities_query_stripped,
             expected_opportunities_query_stripped,
         )
+
         self.assertEqual(
             execute_billinglines_query_stripped,
             expected_billinglines_query_stripped,
         )
+
+        self.assertEqual(
+            execute_pli_query_stripped,
+            expected_pli_query_stripped,
+        )
+
         self.assertEqual(
-            execute_pli_query_stripped, expected_pli_query_stripped
+            execute_accounts_query_stripped,
+            expected_accounts_query_stripped,
         )
```

### Comparing `ms_salesforce_api-0.0.42/pyproject.toml` & `ms_salesforce_api-0.0.43/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ms-salesforce-api"
-version = "0.0.42"
+version = "0.0.43"
 description = "Python library used to extract data from Salesforce API and migrate it to Bigquery and Postgres."
 authors = ["Making Science"]
 readme = "README.md"
 packages = [{include = "ms_salesforce_api"}]
 include = ["pre-commit-config.yaml"]
 
 [tool.poetry.dependencies]
```

### Comparing `ms_salesforce_api-0.0.42/PKG-INFO` & `ms_salesforce_api-0.0.43/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ms-salesforce-api
-Version: 0.0.42
+Version: 0.0.43
 Summary: Python library used to extract data from Salesforce API and migrate it to Bigquery and Postgres.
 Author: Making Science
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ms-salesforce-api Version: 0.0.42 Summary: Python
+Metadata-Version: 2.1 Name: ms-salesforce-api Version: 0.0.43 Summary: Python
 library used to extract data from Salesforce API and migrate it to Bigquery and
 Postgres. Author: Making Science Requires-Python: >=3.8.1,<4.0.0 Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Requires-Dist: flake8 (>=6.0.0,<7.0.0)
 Requires-Dist: gc-google-services-api (>=1.2.7,<2.0.0) Requires-Dist: isort
 (>=5.12.0,<6.0.0) Requires-Dist: pre-commit (>=3.1.1,<4.0.0) Requires-Dist:
```

