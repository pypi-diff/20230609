# Comparing `tmp/sas-airflow-provider-0.0.3.tar.gz` & `tmp/sas-airflow-provider-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/sas-airflow-provider/sas-airflow-provider/dist/.tmp-kibsn5oh/sas-airflow-provider-0.0.3.tar", last modified: Fri May 26 20:22:25 2023, max compression
+gzip compressed data, was "/home/runner/work/sas-airflow-provider/sas-airflow-provider/dist/.tmp-d73ucuww/sas-airflow-provider-0.0.4.tar", last modified: Fri Jun  9 18:46:37 2023, max compression
```

## Comparing `sas-airflow-provider-0.0.3.tar` & `sas-airflow-provider-0.0.4.tar`

### file list

```diff
@@ -1,27 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:22:25.000000 sas-airflow-provider-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-26 20:22:12.000000 sas-airflow-provider-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-05-26 20:22:25.000000 sas-airflow-provider-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3622 2023-05-26 20:22:12.000000 sas-airflow-provider-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-26 20:22:12.000000 sas-airflow-provider-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-26 20:22:25.000000 sas-airflow-provider-0.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:22:25.000000 sas-airflow-provider-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:22:25.000000 sas-airflow-provider-0.0.3/src/sas_airflow_provider/
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-26 20:22:12.000000 sas-airflow-provider-0.0.3/src/sas_airflow_provider/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:22:25.000000 sas-airflow-provider-0.0.3/src/sas_airflow_provider/example_dags/
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-26 20:22:12.000000 sas-airflow-provider-0.0.3/src/sas_airflow_provider/example_dags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-05-26 20:22:12.000000 sas-airflow-provider-0.0.3/src/sas_airflow_provider/example_dags/example_sas_jobexecution.py
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-05-26 20:22:12.000000 sas-airflow-provider-0.0.3/src/sas_airflow_provider/example_dags/example_sas_studioflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     5076 2023-05-26 20:22:12.000000 sas-airflow-provider-0.0.3/src/sas_airflow_provider/example_dags/example_templating.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:22:25.000000 sas-airflow-provider-0.0.3/src/sas_airflow_provider/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-26 20:22:12.000000 sas-airflow-provider-0.0.3/src/sas_airflow_provider/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-05-26 20:22:12.000000 sas-airflow-provider-0.0.3/src/sas_airflow_provider/hooks/sas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:22:25.000000 sas-airflow-provider-0.0.3/src/sas_airflow_provider/operators/
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-26 20:22:12.000000 sas-airflow-provider-0.0.3/src/sas_airflow_provider/operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-05-26 20:22:12.000000 sas-airflow-provider-0.0.3/src/sas_airflow_provider/operators/sas_jobexecution.py
--rw-r--r--   0 runner    (1001) docker     (123)    11079 2023-05-26 20:22:12.000000 sas-airflow-provider-0.0.3/src/sas_airflow_provider/operators/sas_studioflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:22:25.000000 sas-airflow-provider-0.0.3/src/sas_airflow_provider.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-05-26 20:22:25.000000 sas-airflow-provider-0.0.3/src/sas_airflow_provider.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-26 20:22:25.000000 sas-airflow-provider-0.0.3/src/sas_airflow_provider.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 20:22:25.000000 sas-airflow-provider-0.0.3/src/sas_airflow_provider.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-26 20:22:25.000000 sas-airflow-provider-0.0.3/src/sas_airflow_provider.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-26 20:22:25.000000 sas-airflow-provider-0.0.3/src/sas_airflow_provider.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:46:37.000000 sas-airflow-provider-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-09 18:46:22.000000 sas-airflow-provider-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-06-09 18:46:37.000000 sas-airflow-provider-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3622 2023-06-09 18:46:22.000000 sas-airflow-provider-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-09 18:46:22.000000 sas-airflow-provider-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-09 18:46:37.000000 sas-airflow-provider-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:46:37.000000 sas-airflow-provider-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:46:37.000000 sas-airflow-provider-0.0.4/src/sas_airflow_provider/
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-09 18:46:22.000000 sas-airflow-provider-0.0.4/src/sas_airflow_provider/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:46:37.000000 sas-airflow-provider-0.0.4/src/sas_airflow_provider/example_dags/
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-09 18:46:22.000000 sas-airflow-provider-0.0.4/src/sas_airflow_provider/example_dags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-06-09 18:46:22.000000 sas-airflow-provider-0.0.4/src/sas_airflow_provider/example_dags/example_sas_jobexecution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-06-09 18:46:22.000000 sas-airflow-provider-0.0.4/src/sas_airflow_provider/example_dags/example_sas_studioflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5076 2023-06-09 18:46:22.000000 sas-airflow-provider-0.0.4/src/sas_airflow_provider/example_dags/example_templating.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:46:37.000000 sas-airflow-provider-0.0.4/src/sas_airflow_provider/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-09 18:46:22.000000 sas-airflow-provider-0.0.4/src/sas_airflow_provider/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-06-09 18:46:22.000000 sas-airflow-provider-0.0.4/src/sas_airflow_provider/hooks/sas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:46:37.000000 sas-airflow-provider-0.0.4/src/sas_airflow_provider/operators/
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-06-09 18:46:22.000000 sas-airflow-provider-0.0.4/src/sas_airflow_provider/operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-06-09 18:46:22.000000 sas-airflow-provider-0.0.4/src/sas_airflow_provider/operators/sas_jobexecution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10273 2023-06-09 18:46:22.000000 sas-airflow-provider-0.0.4/src/sas_airflow_provider/operators/sas_studioflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:46:37.000000 sas-airflow-provider-0.0.4/src/sas_airflow_provider/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-06-09 18:46:22.000000 sas-airflow-provider-0.0.4/src/sas_airflow_provider/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-06-09 18:46:22.000000 sas-airflow-provider-0.0.4/src/sas_airflow_provider/util/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:46:37.000000 sas-airflow-provider-0.0.4/src/sas_airflow_provider.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-06-09 18:46:37.000000 sas-airflow-provider-0.0.4/src/sas_airflow_provider.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-09 18:46:37.000000 sas-airflow-provider-0.0.4/src/sas_airflow_provider.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 18:46:37.000000 sas-airflow-provider-0.0.4/src/sas_airflow_provider.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-09 18:46:37.000000 sas-airflow-provider-0.0.4/src/sas_airflow_provider.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-09 18:46:37.000000 sas-airflow-provider-0.0.4/src/sas_airflow_provider.egg-info/top_level.txt
```

### Comparing `sas-airflow-provider-0.0.3/LICENSE` & `sas-airflow-provider-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sas-airflow-provider-0.0.3/PKG-INFO` & `sas-airflow-provider-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sas-airflow-provider
-Version: 0.0.3
+Version: 0.0.4
 Summary: Enables execution of Studio Flows and Jobs from Airflow
 Home-page: https://github.com/sassoftware/sas-airflow-provider
 Author: SAS
 Author-email: andrew.shakinovsky@sas.com
 Project-URL: Bug Tracker, https://github.com/sassoftware
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `sas-airflow-provider-0.0.3/README.md` & `sas-airflow-provider-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `sas-airflow-provider-0.0.3/setup.cfg` & `sas-airflow-provider-0.0.4/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sas-airflow-provider
-version = 0.0.3
+version = 0.0.4
 author = SAS
 author_email = andrew.shakinovsky@sas.com
 description = Enables execution of Studio Flows and Jobs from Airflow
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/sassoftware/sas-airflow-provider
 project_urls =
```

### Comparing `sas-airflow-provider-0.0.3/src/sas_airflow_provider/example_dags/__init__.py` & `sas-airflow-provider-0.0.4/src/sas_airflow_provider/example_dags/__init__.py`

 * *Files identical despite different names*

### Comparing `sas-airflow-provider-0.0.3/src/sas_airflow_provider/example_dags/example_sas_jobexecution.py` & `sas-airflow-provider-0.0.4/src/sas_airflow_provider/example_dags/example_sas_jobexecution.py`

 * *Files identical despite different names*

### Comparing `sas-airflow-provider-0.0.3/src/sas_airflow_provider/example_dags/example_sas_studioflow.py` & `sas-airflow-provider-0.0.4/src/sas_airflow_provider/example_dags/example_sas_studioflow.py`

 * *Files identical despite different names*

### Comparing `sas-airflow-provider-0.0.3/src/sas_airflow_provider/example_dags/example_templating.py` & `sas-airflow-provider-0.0.4/src/sas_airflow_provider/example_dags/example_templating.py`

 * *Files identical despite different names*

### Comparing `sas-airflow-provider-0.0.3/src/sas_airflow_provider/hooks/__init__.py` & `sas-airflow-provider-0.0.4/src/sas_airflow_provider/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `sas-airflow-provider-0.0.3/src/sas_airflow_provider/hooks/sas.py` & `sas-airflow-provider-0.0.4/src/sas_airflow_provider/hooks/sas.py`

 * *Files identical despite different names*

### Comparing `sas-airflow-provider-0.0.3/src/sas_airflow_provider/operators/__init__.py` & `sas-airflow-provider-0.0.4/src/sas_airflow_provider/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `sas-airflow-provider-0.0.3/src/sas_airflow_provider/operators/sas_studioflow.py` & `sas-airflow-provider-0.0.4/src/sas_airflow_provider/operators/sas_studioflow.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 
 import requests
 
 from airflow.exceptions import AirflowFailException
 from airflow.exceptions import AirflowException
 from airflow.models import BaseOperator
 from sas_airflow_provider.hooks.sas import SasHook
+from sas_airflow_provider.util.util import dump_logs
 
 class SASStudioFlowOperator(BaseOperator):
     """
     Executes a SAS Studio flow
 
     .. seealso::
         For more information on how to use this operator, take a look at the guide:
@@ -122,15 +123,15 @@
         except Exception as e:
             raise AirflowException(f"SASStudioFlowOperator error: {str(e)}")
 
         # display logs if needed
         if self.flow_exec_log is True:
             # Safeguard if we are unable to retreive the log. We will NOT throw any exceptions
             try:
-                _dump_logs(session, job)
+                dump_logs(session, job)
             except Exception as e:
                 self.log.info("Unable to retrieve log. Maybe the log is too large.")
 
         # raise exception in Airflow if SAS Studio Flow ended execution with "failed" "canceled" or "timed out" state
         # support retry for 'failed' (typically there is an ERROR in the log) and 'timed out'
         # do NOT support retry for 'canceled' (typically the SAS Job called ABORT ABEND)
         if job_state == "failed":
@@ -236,27 +237,16 @@
 
     if response.status_code != 201:
         raise RuntimeError(f"Failed to create session: {response.text}")
 
     return response.json()
 
 
-def _get_file_contents(session, file_uri) -> str:
-    r = session.get(f"{file_uri}/content")
-    if r.status_code != 200:
-        raise RuntimeError(f"Failed to get file contents for {file_uri}: {r.text}")
-    return r.text
 
 
-def _get_uri(links, rel):
-    link = next((x for x in links if x["rel"] == rel), None)
-    if link is None:
-        return None
-    return link["uri"]
-
 
 JES_URI = "/jobExecution"
 JOB_URI = f"{JES_URI}/jobs"
 
 
 def _run_job_and_wait(session, job_request: dict, poll_interval: int) -> dict:
     uri = JOB_URI
@@ -277,18 +267,7 @@
             raise RuntimeError(f"Failed to get job: {response.text}")
         job = response.json()
         state = job["state"]
     print("Job request has completed execution with the status: " + str(state))
     return job
 
 
-def _dump_logs(session, job):
-    # Get the log from the job
-    log_uri = _get_uri(job["links"], "log")
-    if not log_uri:
-        print("Warning: failed to retrieve log uri from links. Log will not be displayed")
-    else:
-        log_contents = _get_file_contents(session, log_uri)
-        # Parse the json log format and print each line
-        jcontents = json.loads(log_contents)
-        for line in jcontents["items"]:
-            print(f'{line["type"]}: {line["line"]}\n')
```

### Comparing `sas-airflow-provider-0.0.3/src/sas_airflow_provider.egg-info/PKG-INFO` & `sas-airflow-provider-0.0.4/src/sas_airflow_provider.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sas-airflow-provider
-Version: 0.0.3
+Version: 0.0.4
 Summary: Enables execution of Studio Flows and Jobs from Airflow
 Home-page: https://github.com/sassoftware/sas-airflow-provider
 Author: SAS
 Author-email: andrew.shakinovsky@sas.com
 Project-URL: Bug Tracker, https://github.com/sassoftware
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `sas-airflow-provider-0.0.3/src/sas_airflow_provider.egg-info/SOURCES.txt` & `sas-airflow-provider-0.0.4/src/sas_airflow_provider.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -12,8 +12,10 @@
 src/sas_airflow_provider/example_dags/example_sas_jobexecution.py
 src/sas_airflow_provider/example_dags/example_sas_studioflow.py
 src/sas_airflow_provider/example_dags/example_templating.py
 src/sas_airflow_provider/hooks/__init__.py
 src/sas_airflow_provider/hooks/sas.py
 src/sas_airflow_provider/operators/__init__.py
 src/sas_airflow_provider/operators/sas_jobexecution.py
-src/sas_airflow_provider/operators/sas_studioflow.py
+src/sas_airflow_provider/operators/sas_studioflow.py
+src/sas_airflow_provider/util/__init__.py
+src/sas_airflow_provider/util/util.py
```

