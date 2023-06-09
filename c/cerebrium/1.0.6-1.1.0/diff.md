# Comparing `tmp/cerebrium-1.0.6.tar.gz` & `tmp/cerebrium-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cerebrium-1.0.6.tar", max compression
+gzip compressed data, was "cerebrium-1.1.0.tar", max compression
```

## Comparing `cerebrium-1.0.6.tar` & `cerebrium-1.1.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0    34594 2023-06-09 10:01:40.665978 cerebrium-1.0.6/LICENSE
--rw-r--r--   0        0        0     3193 2023-06-09 10:01:40.665978 cerebrium-1.0.6/README.md
--rw-r--r--   0        0        0      285 2023-06-09 10:06:16.296230 cerebrium-1.0.6/cerebrium/__init__.py
--rwxr-xr-x   0        0        0     8528 2023-06-09 10:01:40.665978 cerebrium-1.0.6/cerebrium/cli.py
--rw-r--r--   0        0        0    31667 2023-06-09 10:01:40.665978 cerebrium-1.0.6/cerebrium/conduit.py
--rw-r--r--   0        0        0     4483 2023-06-09 10:01:40.665978 cerebrium-1.0.6/cerebrium/core.py
--rw-r--r--   0        0        0     2476 2023-06-09 10:01:40.665978 cerebrium-1.0.6/cerebrium/errors.py
--rw-r--r--   0        0        0    11299 2023-06-09 10:01:40.665978 cerebrium-1.0.6/cerebrium/flow.py
--rw-r--r--   0        0        0     2807 2023-06-09 10:01:40.665978 cerebrium-1.0.6/cerebrium/logging/arize.py
--rw-r--r--   0        0        0      705 2023-06-09 10:01:40.665978 cerebrium-1.0.6/cerebrium/logging/base.py
--rw-r--r--   0        0        0     3855 2023-06-09 10:01:40.665978 cerebrium-1.0.6/cerebrium/logging/censius.py
--rw-r--r--   0        0        0      911 2023-06-09 10:01:40.665978 cerebrium-1.0.6/cerebrium/models/base.py
--rw-r--r--   0        0        0      446 2023-06-09 10:01:40.665978 cerebrium-1.0.6/cerebrium/models/hf_pipeline.py
--rw-r--r--   0        0        0      418 2023-06-09 10:01:40.665978 cerebrium-1.0.6/cerebrium/models/onnx.py
--rw-r--r--   0        0        0     1116 2023-06-09 10:01:40.665978 cerebrium-1.0.6/cerebrium/models/sklearn.py
--rw-r--r--   0        0        0      244 2023-06-09 10:01:40.665978 cerebrium-1.0.6/cerebrium/models/spacy.py
--rw-r--r--   0        0        0      342 2023-06-09 10:01:40.665978 cerebrium-1.0.6/cerebrium/models/torch.py
--rw-r--r--   0        0        0     7177 2023-06-09 10:01:40.665978 cerebrium-1.0.6/cerebrium/requests.py
--rw-r--r--   0        0        0      465 2023-06-09 10:01:40.665978 cerebrium-1.0.6/cerebrium/utils.py
--rw-r--r--   0        0        0     2340 2023-06-09 10:06:16.296230 cerebrium-1.0.6/pyproject.toml
--rw-r--r--   0        0        0     5282 1970-01-01 00:00:00.000000 cerebrium-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0    34594 2023-06-09 13:01:37.533263 cerebrium-1.1.0/LICENSE
+-rw-r--r--   0        0        0     3193 2023-06-09 13:01:37.533263 cerebrium-1.1.0/README.md
+-rw-r--r--   0        0        0      330 2023-06-09 13:05:25.573181 cerebrium-1.1.0/cerebrium/__init__.py
+-rwxr-xr-x   0        0        0     8671 2023-06-09 13:01:37.533263 cerebrium-1.1.0/cerebrium/cli.py
+-rw-r--r--   0        0        0    31667 2023-06-09 13:01:37.533263 cerebrium-1.1.0/cerebrium/conduit.py
+-rw-r--r--   0        0        0     5049 2023-06-09 13:01:37.533263 cerebrium-1.1.0/cerebrium/core.py
+-rw-r--r--   0        0        0     2476 2023-06-09 13:01:37.533263 cerebrium-1.1.0/cerebrium/errors.py
+-rw-r--r--   0        0        0    11299 2023-06-09 13:01:37.533263 cerebrium-1.1.0/cerebrium/flow.py
+-rw-r--r--   0        0        0     2807 2023-06-09 13:01:37.533263 cerebrium-1.1.0/cerebrium/logging/arize.py
+-rw-r--r--   0        0        0      705 2023-06-09 13:01:37.533263 cerebrium-1.1.0/cerebrium/logging/base.py
+-rw-r--r--   0        0        0     3855 2023-06-09 13:01:37.533263 cerebrium-1.1.0/cerebrium/logging/censius.py
+-rw-r--r--   0        0        0      911 2023-06-09 13:01:37.533263 cerebrium-1.1.0/cerebrium/models/base.py
+-rw-r--r--   0        0        0      446 2023-06-09 13:01:37.533263 cerebrium-1.1.0/cerebrium/models/hf_pipeline.py
+-rw-r--r--   0        0        0      418 2023-06-09 13:01:37.533263 cerebrium-1.1.0/cerebrium/models/onnx.py
+-rw-r--r--   0        0        0     1116 2023-06-09 13:01:37.533263 cerebrium-1.1.0/cerebrium/models/sklearn.py
+-rw-r--r--   0        0        0      244 2023-06-09 13:01:37.533263 cerebrium-1.1.0/cerebrium/models/spacy.py
+-rw-r--r--   0        0        0      342 2023-06-09 13:01:37.533263 cerebrium-1.1.0/cerebrium/models/torch.py
+-rw-r--r--   0        0        0     8540 2023-06-09 13:01:37.533263 cerebrium-1.1.0/cerebrium/requests.py
+-rw-r--r--   0        0        0      465 2023-06-09 13:01:37.533263 cerebrium-1.1.0/cerebrium/utils.py
+-rw-r--r--   0        0        0     2546 2023-06-09 13:05:25.569181 cerebrium-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     5337 1970-01-01 00:00:00.000000 cerebrium-1.1.0/PKG-INFO
```

### Comparing `cerebrium-1.0.6/LICENSE` & `cerebrium-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cerebrium-1.0.6/README.md` & `cerebrium-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `cerebrium-1.0.6/cerebrium/cli.py` & `cerebrium-1.1.0/cerebrium/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -124,15 +124,19 @@
         zip_path = os.path.join(temp_dir, zip_file_name)
         dir_name = os.path.dirname(zip_path)
         os.makedirs(dir_name, exist_ok=True)
         with zipfile.ZipFile(zip_path, "w") as zip_file:
             # write every file in the current directory and subdirectories to the zip file
             for root, dirs, files in os.walk("."):
                 for file in files:
-                    if file != zip_file_name:
+                    if file != zip_file_name and file.lower() not in (
+                        "secrets.json",
+                        "secrets.yaml",
+                        "secrets.yml",
+                    ):
                         zip_file.write(os.path.join(root, file))
         print("⬆️  Uploading to Cerebrium...")
         with open(zip_path, "rb") as f:
             headers = {
                 "Content-Type": "application/zip",
             }
             with tqdm(
@@ -208,29 +212,29 @@
                 spinner.fail("⏲️ Build timed out.")
                 sys.exit(1)
             elif build_status == "build_failure" or build_status == "init_failure":
                 spinner.fail("❌ Build failed.")
                 sys.exit(1)
         spinner.text = f"Status: {build_status}"
         spinner.ok("🚀 Build complete!")
-        print("\n🌍 Endpoint:", endpoint)
+        print("\n🌍 Endpoint:", endpoint, "\n")
         print("💡 You can call the endpoint with the following curl command:")
         print(
             colored(
                 f"curl -X POST {endpoint} \\\n"
                 "     -H 'Content-Type: application/json' \\\n"
                 "     -H 'Authorization: <public_api_key>' \\\n"
                 "     --data '{}'",
                 "green",
             )
         )
         print("----------------------------------------")
         print(
-            f"🔗 View builds: https://dashboard.cerebrium.ai/projects/{project_id}/models/{project_id}-{name}?tab=builds"
+            f"🔗 View builds: {dashboard_url}/projects/{project_id}/models/{project_id}-{name}?tab=builds"
         )
         print(
-            f"🔗 View runs: https://dashboard.cerebrium.ai/projects/{project_id}/models/{project_id}-{name}?tab=runs"
+            f"🔗 View runs: {dashboard_url}/projects/{project_id}/models/{project_id}-{name}?tab=runs"
         )
 
 
 if __name__ == "__main__":
     app()
```

### Comparing `cerebrium-1.0.6/cerebrium/conduit.py` & `cerebrium-1.1.0/cerebrium/conduit.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.0.6/cerebrium/core.py` & `cerebrium-1.1.0/cerebrium/core.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,21 +4,42 @@
 
 import requests
 import json
 from typing import Union, List
 import boto3
 import os
 from uuid import uuid4
-
+import yaml
 from numpy import ndarray
 from torch import Tensor
 from cerebrium.requests import _cerebrium_request, ENV
 
 IS_SERVER = os.getenv("IS_SERVER", "false")
 _objects = {}
+if os.path.exists("secrets.json"):
+    with open("secrets.json") as f:
+        SECRETS = json.load(f)
+elif os.path.exists("secrets.yaml"):
+    with open("secrets.yaml") as f:
+        SECRETS = yaml.load(f, Loader=yaml.FullLoader)
+else:
+    SECRETS = {}
+
+
+def get_secret(key):
+    if SECRETS:
+        secret = SECRETS.get(key, "")
+    else:
+        secret = os.getenv(key, "")
+    if secret == "":
+        raise Exception(
+            f"Secret not found for key: {key}, please check set your environment variable"
+        )
+    else:
+        return secret
 
 
 def upload(file_name):
     # Upload a file to Cerebrium S3 and return a URL to the file
     from cerebrium.conduit import API_KEY
 
     if API_KEY and IS_SERVER == "true":
```

### Comparing `cerebrium-1.0.6/cerebrium/errors.py` & `cerebrium-1.1.0/cerebrium/errors.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.0.6/cerebrium/flow.py` & `cerebrium-1.1.0/cerebrium/flow.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.0.6/cerebrium/logging/arize.py` & `cerebrium-1.1.0/cerebrium/logging/arize.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.0.6/cerebrium/logging/base.py` & `cerebrium-1.1.0/cerebrium/logging/base.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.0.6/cerebrium/logging/censius.py` & `cerebrium-1.1.0/cerebrium/logging/censius.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.0.6/cerebrium/models/base.py` & `cerebrium-1.1.0/cerebrium/models/base.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.0.6/cerebrium/models/sklearn.py` & `cerebrium-1.1.0/cerebrium/models/sklearn.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.0.6/cerebrium/requests.py` & `cerebrium-1.1.0/cerebrium/requests.py`

 * *Files 10% similar despite different names*

```diff
@@ -182,7 +182,42 @@
         print("----------------------------------------")
         print(
             f"🔗 View builds: https://dashboard.cerebrium.ai/projects/{project_id}/models/{project_id}-{name}?tab=builds"
         )
         print(
             f"🔗 View runs: https://dashboard.cerebrium.ai/projects/{project_id}/models/{project_id}-{name}?tab=runs"
         )
+
+
+@retry(stop=stop_after_delay(60), wait=wait_fixed(2))
+def _poll_training_deploy_status(training_name: str, api_key: str) -> str:
+    """
+    Poll the deployment status of a training job.
+
+    Args:
+        training_name (str): The name of the training to check the status of.
+        api_key (str): The API key for the Cerebrium account.
+
+    Returns:
+        str: The endpoint of the deployed model.
+    """
+    # Check the status of the deployment by polling the Cerebrium API for deployment status
+    with yaspin(
+        spinner=Spinners.arc, text="Checking deployment status...", color="magenta"
+    ) as spinner:
+        response = _cerebrium_request(
+            "checkDeploymentStatus",
+            api_key,
+            payload={"arguments": {"name": training_name}},
+        )
+    if response["data"]["status"] == "deployed":
+        endpoint = response["data"]["endpoint"]
+        print("✅ FineTuning deployed!")
+        return endpoint
+    elif response["data"]["status"] == "failed":
+        print("❌ FineTuning deployment failed.")
+        raise CerebriumDeploymentError(response["data"]["failureMessage"])
+    else:
+        print("⏳ FineTuning deployment in progress...")
+        raise CerebriumDeploymentError(
+            "Deployment Not Complete. Your conduit might be large and take longer to deploy. Please try again later."
+        )
```

### Comparing `cerebrium-1.0.6/pyproject.toml` & `cerebrium-1.1.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 [tool.poetry]
 name = "cerebrium"
-version = "1.0.6"
+version = "1.1.0"
 description = ""
 authors = ["Elijah Roussos <elijah@cerebrium.ai>"]
 license = "AGPL-3.0-only"
 readme = "README.md"
 exclude = ["tests/*", "dist/*", "worker/*", "builder/*", "prebuilt/*", "common/*", "examples/*"]
 
 [tool.poetry.urls]
 "Homepage" = "https://www.cerebrium.ai"
 "Documentation" = "https://docs.cerebrium.ai/"
 
+[[tool.poetry.source]]
+name = "cerebrium"
+url = "https://cerebrium-288552132534.d.codeartifact.eu-west-1.amazonaws.com/pypi/cerebrium-pypi/"
+
 [tool.poetry.scripts]
 cerebrium = "cerebrium.cli:app"
 
 [tool.poetry-dynamic-versioning]
 enable = false
 
 [tool.poetry.dependencies]
@@ -44,14 +48,15 @@
 datasets = { version = ">=2.10.0,<2.11.0", optional= true }
 celery = { version = ">=5.2.0,<5.3.0", optional= true }
 accelerate = { version = ">=0.18.0,<0.19.0", optional= true }
 bitsandbytes = { version = ">=0.38.0,<0.39.0", optional= true }
 tensorflow = { version = ">=2.12.0", optional= true }
 typer = { version = "0.7.0", extras = ["all"] }
 keras = { version = ">=2.12.0", optional= true }
+xformers = { version = ">=0.0.16", optional= true }
 
 [tool.poetry.group.dev.dependencies]
 black = ">=23.1,<23.2"
 ipython = ">=8.9,<8.10"
 ipykernel = ">=6.21,<6.22"
 poetry-dotenv = "0.3.0"
 poetry-dynamic-versioning = {extras = ["plugin"], version = ">=0.21,<0.22"}
@@ -61,13 +66,13 @@
 pytest-cov = ">=4.0,<4.1"
 notebook = ">=6.5,<6.6"
 torchinfo = ">=1.7,<1.8"
 
 [tool.poetry.extras]
 onnxruntime = ["onnxruntime"]
 onnxruntime-gpu = ["onnxruntime-gpu"]
-worker = ["loguru", "ddtrace", "datadog", "Pillow", "chitra", "datasets", "celery", "accelerate", "bitsandbytes"]
+worker = ["loguru", "ddtrace", "datadog", "Pillow", "chitra", "datasets", "celery", "accelerate", "bitsandbytes", "xformers"]
 tensorflow = ["tensorflow", "keras"]
 
 [build-system]
 requires = ["poetry-core", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
```

### Comparing `cerebrium-1.0.6/PKG-INFO` & `cerebrium-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cerebrium
-Version: 1.0.6
+Version: 1.1.0
 Summary: 
 License: AGPL-3.0-only
 Author: Elijah Roussos
 Author-email: elijah@cerebrium.ai
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
@@ -38,14 +38,15 @@
 Requires-Dist: spacy (>=3.5.0,<4.0.0)
 Requires-Dist: tenacity (>=8.2,<8.3)
 Requires-Dist: tensorflow (>=2.12.0) ; extra == "tensorflow"
 Requires-Dist: torch (>=1.13,<3.0)
 Requires-Dist: tqdm (>=4.64,<4.65)
 Requires-Dist: transformers (>=4.26,<5.0)
 Requires-Dist: typer[all] (==0.7.0)
+Requires-Dist: xformers (>=0.0.16) ; extra == "worker"
 Requires-Dist: xgboost (>=1.7,<2.0)
 Requires-Dist: yaspin (>=2.3,<2.4)
 Project-URL: Documentation, https://docs.cerebrium.ai/
 Project-URL: Homepage, https://www.cerebrium.ai
 Description-Content-Type: text/markdown
 
 # Cerebrium
```

