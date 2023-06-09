# Comparing `tmp/cerebrium-1.0.5.tar.gz` & `tmp/cerebrium-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cerebrium-1.0.5.tar", max compression
+gzip compressed data, was "cerebrium-1.0.6.tar", max compression
```

## Comparing `cerebrium-1.0.5.tar` & `cerebrium-1.0.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0    34594 2023-06-08 12:44:17.440744 cerebrium-1.0.5/LICENSE
--rw-r--r--   0        0        0     3193 2023-06-08 12:44:17.440744 cerebrium-1.0.5/README.md
--rw-r--r--   0        0        0      285 2023-06-08 12:49:17.438397 cerebrium-1.0.5/cerebrium/__init__.py
--rwxr-xr-x   0        0        0     8478 2023-06-08 12:44:17.440744 cerebrium-1.0.5/cerebrium/cli.py
--rw-r--r--   0        0        0    31396 2023-06-08 12:44:17.440744 cerebrium-1.0.5/cerebrium/conduit.py
--rw-r--r--   0        0        0     4483 2023-06-08 12:44:17.440744 cerebrium-1.0.5/cerebrium/core.py
--rw-r--r--   0        0        0     2520 2023-06-08 12:44:17.440744 cerebrium-1.0.5/cerebrium/errors.py
--rw-r--r--   0        0        0    11229 2023-06-08 12:44:17.440744 cerebrium-1.0.5/cerebrium/flow.py
--rw-r--r--   0        0        0     2807 2023-06-08 12:44:17.440744 cerebrium-1.0.5/cerebrium/logging/arize.py
--rw-r--r--   0        0        0      705 2023-06-08 12:44:17.440744 cerebrium-1.0.5/cerebrium/logging/base.py
--rw-r--r--   0        0        0     3855 2023-06-08 12:44:17.440744 cerebrium-1.0.5/cerebrium/logging/censius.py
--rw-r--r--   0        0        0      911 2023-06-08 12:44:17.440744 cerebrium-1.0.5/cerebrium/models/base.py
--rw-r--r--   0        0        0      446 2023-06-08 12:44:17.440744 cerebrium-1.0.5/cerebrium/models/hf_pipeline.py
--rw-r--r--   0        0        0      418 2023-06-08 12:44:17.440744 cerebrium-1.0.5/cerebrium/models/onnx.py
--rw-r--r--   0        0        0     1116 2023-06-08 12:44:17.444744 cerebrium-1.0.5/cerebrium/models/sklearn.py
--rw-r--r--   0        0        0      244 2023-06-08 12:44:17.444744 cerebrium-1.0.5/cerebrium/models/spacy.py
--rw-r--r--   0        0        0      342 2023-06-08 12:44:17.444744 cerebrium-1.0.5/cerebrium/models/torch.py
--rw-r--r--   0        0        0     7124 2023-06-08 12:44:17.444744 cerebrium-1.0.5/cerebrium/requests.py
--rw-r--r--   0        0        0      465 2023-06-08 12:44:17.444744 cerebrium-1.0.5/cerebrium/utils.py
--rw-r--r--   0        0        0     2340 2023-06-08 12:49:17.434397 cerebrium-1.0.5/pyproject.toml
--rw-r--r--   0        0        0     5282 1970-01-01 00:00:00.000000 cerebrium-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0    34594 2023-06-09 10:01:40.665978 cerebrium-1.0.6/LICENSE
+-rw-r--r--   0        0        0     3193 2023-06-09 10:01:40.665978 cerebrium-1.0.6/README.md
+-rw-r--r--   0        0        0      285 2023-06-09 10:06:16.296230 cerebrium-1.0.6/cerebrium/__init__.py
+-rwxr-xr-x   0        0        0     8528 2023-06-09 10:01:40.665978 cerebrium-1.0.6/cerebrium/cli.py
+-rw-r--r--   0        0        0    31667 2023-06-09 10:01:40.665978 cerebrium-1.0.6/cerebrium/conduit.py
+-rw-r--r--   0        0        0     4483 2023-06-09 10:01:40.665978 cerebrium-1.0.6/cerebrium/core.py
+-rw-r--r--   0        0        0     2476 2023-06-09 10:01:40.665978 cerebrium-1.0.6/cerebrium/errors.py
+-rw-r--r--   0        0        0    11299 2023-06-09 10:01:40.665978 cerebrium-1.0.6/cerebrium/flow.py
+-rw-r--r--   0        0        0     2807 2023-06-09 10:01:40.665978 cerebrium-1.0.6/cerebrium/logging/arize.py
+-rw-r--r--   0        0        0      705 2023-06-09 10:01:40.665978 cerebrium-1.0.6/cerebrium/logging/base.py
+-rw-r--r--   0        0        0     3855 2023-06-09 10:01:40.665978 cerebrium-1.0.6/cerebrium/logging/censius.py
+-rw-r--r--   0        0        0      911 2023-06-09 10:01:40.665978 cerebrium-1.0.6/cerebrium/models/base.py
+-rw-r--r--   0        0        0      446 2023-06-09 10:01:40.665978 cerebrium-1.0.6/cerebrium/models/hf_pipeline.py
+-rw-r--r--   0        0        0      418 2023-06-09 10:01:40.665978 cerebrium-1.0.6/cerebrium/models/onnx.py
+-rw-r--r--   0        0        0     1116 2023-06-09 10:01:40.665978 cerebrium-1.0.6/cerebrium/models/sklearn.py
+-rw-r--r--   0        0        0      244 2023-06-09 10:01:40.665978 cerebrium-1.0.6/cerebrium/models/spacy.py
+-rw-r--r--   0        0        0      342 2023-06-09 10:01:40.665978 cerebrium-1.0.6/cerebrium/models/torch.py
+-rw-r--r--   0        0        0     7177 2023-06-09 10:01:40.665978 cerebrium-1.0.6/cerebrium/requests.py
+-rw-r--r--   0        0        0      465 2023-06-09 10:01:40.665978 cerebrium-1.0.6/cerebrium/utils.py
+-rw-r--r--   0        0        0     2340 2023-06-09 10:06:16.296230 cerebrium-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0     5282 1970-01-01 00:00:00.000000 cerebrium-1.0.6/PKG-INFO
```

### Comparing `cerebrium-1.0.5/LICENSE` & `cerebrium-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cerebrium-1.0.5/README.md` & `cerebrium-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `cerebrium-1.0.5/cerebrium/cli.py` & `cerebrium-1.0.6/cerebrium/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     ),
     pre_init_debug: bool = typer.Option(
         False,
         help="Stops the container before initialization.",
     ),
     log_level: str = typer.Option(
         "INFO",
-        help="Log level for the builder deployment. Can be one of 'DEBUG' or 'INFO'"
+        help="Log level for the builder deployment. Can be one of 'DEBUG' or 'INFO'",
     ),
 ):
     """
     Deploy a builder deployment to Cerebrium
     """
     print(f"Deploying {name} with {hardware} hardware to Cerebrium...")
 
@@ -137,20 +137,20 @@
             }
             with tqdm(
                 total=os.path.getsize(zip_path),
                 unit="B",
                 unit_scale=True,
                 unit_divisor=1024,
                 colour="#EB3A6F",
-            ) as pbar: # type: ignore
+            ) as pbar:  # type: ignore
                 wrapped_f = CallbackIOWrapper(pbar.update, f, "read")
                 upload_response = requests.put(
                     upload_url,
                     headers=headers,
-                    data=wrapped_f, # type: ignore
+                    data=wrapped_f,  # type: ignore
                     timeout=60,
                     stream=True,
                 )
             if upload_response.status_code != 200:
                 print(
                     "API request failed with status code:", upload_response.status_code
                 )
@@ -190,38 +190,43 @@
                     if message:
                         match = re.match(
                             r"^(\d{4}-\d{2}-\d{2}T\d{2}:\d{2}:\d{2}\.\d{9})Z ", message
                         )
                         if (
                             match is not None
                         ):  # If the regex matches the beginning of the string
-                            created = match.group(1)  # The first group is the creation time
-                            message = message[
-                                len(created) + 2 :
-                            ]
+                            created = match.group(
+                                1
+                            )  # The first group is the creation time
+                            message = message[len(created) + 2 :]
                         spinner.write(f"{message}")
                     else:
                         spinner.write("\n")
                 seen_index = len(logs)
-                spinner.text = f"🔨 Building... Status: {build_status}"    
+                spinner.text = f"🔨 Building... Status: {build_status}"
                 time.sleep(1)
             if time.time() - t1 > 600:
                 spinner.fail("⏲️ Build timed out.")
                 sys.exit(1)
             elif build_status == "build_failure" or build_status == "init_failure":
                 spinner.fail("❌ Build failed.")
                 sys.exit(1)
         spinner.text = f"Status: {build_status}"
         spinner.ok("🚀 Build complete!")
         print("\n🌍 Endpoint:", endpoint)
         print("💡 You can call the endpoint with the following curl command:")
-        print(colored(f"curl -X POST {endpoint} \\\n"
-                      "     -H 'Content-Type: application/json' \\\n"
-                      "     -H 'Authorization: <public_api_key>' \\\n"
-                      "     --data '{}'", "green"))
+        print(
+            colored(
+                f"curl -X POST {endpoint} \\\n"
+                "     -H 'Content-Type: application/json' \\\n"
+                "     -H 'Authorization: <public_api_key>' \\\n"
+                "     --data '{}'",
+                "green",
+            )
+        )
         print("----------------------------------------")
         print(
             f"🔗 View builds: https://dashboard.cerebrium.ai/projects/{project_id}/models/{project_id}-{name}?tab=builds"
         )
         print(
             f"🔗 View runs: https://dashboard.cerebrium.ai/projects/{project_id}/models/{project_id}-{name}?tab=runs"
         )
```

### Comparing `cerebrium-1.0.5/cerebrium/conduit.py` & `cerebrium-1.0.6/cerebrium/conduit.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from cloudpickle import load as pickle_load
-from torch.jit import load as torchscript_load # type: ignore
+from torch.jit import load as torchscript_load  # type: ignore
 from tqdm import tqdm
 from tqdm.utils import CallbackIOWrapper
 import os
 import re
 import tempfile
 import zipfile
 import requests
 import json
 import enum
 from copy import deepcopy
-from typing import Any, Dict, Literal
+from typing import Any, Dict, Literal, Union
 from types import FunctionType
 
 from torch.nn import Module as TorchModule
 from torch.cuda import is_available
 from numpy import atleast_2d, ndarray
 from inspect import getsource, signature
 
@@ -52,15 +52,15 @@
     """
 
     def __init__(
         self,
         name: str = "",
         api_key: str = "",
         flow: CerebriumFlow = [],
-        hardware: Hardware | None = None,
+        hardware: Union[Hardware, None] = None,
         from_json: str = "",
     ):
         if not from_json:
             if api_key != "":
                 self.api_key = api_key
             else:
                 self.api_key = os.environ.get("CEREBRIUM_API_KEY", "")
@@ -82,15 +82,15 @@
                 config = json.load(f)
                 self.name = config["name"]
                 self.api_key = config["api_key"]
                 self.flow: CerebriumFlow = config["flow"]
                 self.logger_configs = config["logger_configs"]
                 self._processors = config["processors"]
                 # Set correct ModelTypes in flow
-                for i, (model_type, model_initialization, processors) in enumerate( # type: ignore
+                for i, (model_type, model_initialization, processors) in enumerate(  # type: ignore
                     self.flow
                 ):
                     self.flow[i] = (
                         ModelType(model_type),
                         model_initialization,
                         processors,
                     )
@@ -109,15 +109,15 @@
 
     def _determine_hardware(self):
         # Set the default hardware to GPU if the flow contains a Torch, ONNX or HuggingFace model
         if any(
             [
                 model_type
                 in [ModelType.TORCH, ModelType.ONNX, ModelType.HUGGINGFACE_PIPELINE]
-                for model_type, _, _ in self.flow # type: ignore
+                for model_type, _, _ in self.flow  # type: ignore
             ]
         ):
             return Hardware.GPU
         else:
             return Hardware.CPU
 
     def load(self, directory: str = "/cache/", direct_from_flow: bool = False):
@@ -128,34 +128,36 @@
             directory (str): The directory to load the Conduit components from.
         """
         from sklearn.base import ClassifierMixin, RegressorMixin, BaseEstimator
 
         if self.flow == []:
             raise ValueError("Conduit is empty. Please add models to the Conduit flow.")
         else:
-            for model_type, model_initialization, _ in self.flow: # type: ignore
+            for model_type, model_initialization, _ in self.flow:  # type: ignore
                 # Use correct path
                 if direct_from_flow:
                     model_initialization: str = os.path.abspath(model_initialization)
                 elif (
                     model_type != ModelType.PREBUILT
                     and model_type != ModelType.HUGGINGFACE_PIPELINE
-                ):  
+                ):
                     model_initialization: str = (
                         directory + model_initialization.split("/")[-1]
                     )
                 else:
                     pass
 
                 # Torch
                 if model_type == ModelType.TORCH:
                     from cerebrium.models.torch import TorchModel
 
                     if model_initialization.endswith(".pt"):
-                        torch_model: TorchModule = torchscript_load(model_initialization)
+                        torch_model: TorchModule = torchscript_load(
+                            model_initialization
+                        )
                     else:
                         with open(model_initialization, "rb") as f:
                             torch_model: TorchModule = pickle_load(f)
                     torch_model.to(self.device)
                     self.graph.append(TorchModel(torch_model))
 
                 # ONNX
@@ -230,23 +232,25 @@
                     self.graph.append(SKPreprocessorModel(sk_preprocessor))
 
                 # HuggingFace Pipeline
                 elif model_type == ModelType.HUGGINGFACE_PIPELINE:
                     from cerebrium.models.hf_pipeline import HFPipeline
                     from transformers.pipelines import pipeline
 
-                    hf_pipeline = HFPipeline(pipeline(**model_initialization)) # type: ignore
+                    hf_pipeline = HFPipeline(pipeline(**model_initialization))  # type: ignore
                     self.graph.append(hf_pipeline)
 
             # If there are processors, create a processors.py file with the respective processors
             # Save the processors.py file in the /usr/local/lib/python3.10/dist-packages/conduit_processors directory
             if self._processors:
                 app_name = os.getenv("APP_NAME", "")
                 assert app_name != "", "APP_NAME environment variable not set"
-                processor_path = f"/miniconda/envs/{app_name}/lib/python3.10/conduit_processors"
+                processor_path = (
+                    f"/miniconda/envs/{app_name}/lib/python3.10/conduit_processors"
+                )
                 os.makedirs(processor_path, exist_ok=True)
                 # Create the processors.py file
                 with open(
                     f"{processor_path}/processors.py",
                     "w",
                 ) as f:
                     f.write(
@@ -279,15 +283,15 @@
             data (list): The input data to run the Conduit on.
         """
         from torch import Tensor
 
         if self._processors:
             # List files in working directory
             files = os.listdir()
-            import conduit_processors # type: ignore
+            import conduit_processors  # type: ignore
 
         if not self.ready:
             return "Conduit not ready. Conduit components have not been loaded."
         else:
             # If there is no initial pre-processor, convert the data accordingly
             if not self.flow[0][2].get("pre", False):
                 if self.flow[0][0] == ModelType.TORCH:
@@ -307,20 +311,20 @@
                     data = atleast_2d(data)
 
             # Set input data
             input_data = data
 
             for (model_type, _, processors), (model) in zip(self.flow, self.graph):
                 # Run the preprocessor
-                preprocessor: FunctionType | str = processors.get("pre", "")
-                postprocessor: FunctionType | str = processors.get("post", "")
+                preprocessor: Union[FunctionType, str] = processors.get("pre", "")
+                postprocessor: Union[FunctionType, str] = processors.get("post", "")
                 if preprocessor:
                     if self._processors:
                         assert isinstance(preprocessor, str)
-                        preprocessor_function: FunctionType = getattr(conduit_processors, preprocessor) # type: ignore
+                        preprocessor_function: FunctionType = getattr(conduit_processors, preprocessor)  # type: ignore
                     else:
                         assert isinstance(preprocessor, FunctionType)
                         preprocessor_function: FunctionType = preprocessor
                     sig = signature(preprocessor_function)
                     if len(sig.parameters) == 1:
                         data = preprocessor_function(data)
                     elif len(sig.parameters) == 2:
@@ -335,15 +339,15 @@
                 # Run the model
                 data = model.predict(data)
 
                 # Run the postprocessor
                 if postprocessor:
                     if self._processors:
                         assert isinstance(postprocessor, str)
-                        postprocessor_function = getattr(conduit_processors, postprocessor) # type: ignore
+                        postprocessor_function = getattr(conduit_processors, postprocessor)  # type: ignore
                     else:
                         assert isinstance(postprocessor, FunctionType)
                         postprocessor_function: FunctionType = postprocessor
                     sig = signature(postprocessor_function)
                     if len(sig.parameters) == 1:
                         data = postprocessor_function(data)
                     elif len(sig.parameters) == 2:
@@ -356,15 +360,22 @@
                 data = data.detach().to("cpu").numpy().tolist()
             elif isinstance(data, ndarray):
                 data = data.tolist()
             elif not isinstance(data, list) and not isinstance(data, dict):
                 data = [data]
             return data
 
-    def add_model(self, model_type: ModelType, model_initialization: str | dict, postprocessor: Dict[Literal["pre"] | Literal["post"], FunctionType] | None = None):
+    def add_model(
+        self,
+        model_type: ModelType,
+        model_initialization: Union[str, dict],
+        postprocessor: Union[
+            Dict[Union[Literal["pre"], Literal["post"]], FunctionType], None
+        ] = None,
+    ):
         """
         Add a model to the Conduit's computational flow.
         """
         temp_flow = self.flow
         temp_flow.append((model_type, model_initialization, postprocessor))
         self.flow = _check_flow_type(temp_flow)
         self._determine_hardware()
@@ -532,29 +543,31 @@
         """
         Return the Conduit's configuration as a JSON string.
 
         Returns:
             str: The Conduit's configuration as a JSON string.
         """
 
-        def get_function_names(processors: Dict[Literal["pre"] | Literal["post"], FunctionType]):
+        def get_function_names(
+            processors: Dict[Union[Literal["pre"], Literal["post"]], FunctionType]
+        ):
             names = {}
             if "pre" in processors:
                 names["pre"] = processors["pre"].__name__
             else:
                 names["pre"] = None
             if "post" in processors:
                 names["post"] = processors["post"].__name__
             else:
                 names["post"] = None
             return names
 
         json_flow = [
-            (model_type.value, model_initialization, get_function_names(processors)) # type: ignore
-            for model_type, model_initialization, processors in self.flow 
+            (model_type.value, model_initialization, get_function_names(processors))  # type: ignore
+            for model_type, model_initialization, processors in self.flow
         ]
         with open(filename, "w") as f:
             json.dump(
                 {
                     "name": self.name,
                     "flow": json_flow,
                     "api_key": self.api_key,
@@ -641,15 +654,15 @@
                         unit_divisor=1024,
                         colour="#EB3A6F",
                     ) as pbar:
                         wrapped_f = CallbackIOWrapper(pbar.update, f, "read")
                         response = requests.put(
                             url,
                             headers=headers,
-                            data=wrapped_f, # type: ignore
+                            data=wrapped_f,  # type: ignore
                             timeout=60,
                             stream=True,
                         )
                     data = {} if not response.text else json.loads(response.text)
                     return {"status_code": response.status_code, "data": data}
 
     def deploy(self, dry_run=False) -> str:
@@ -708,14 +721,16 @@
                 print("🌍 Endpoint:", endpoint)
                 return endpoint
             else:
                 # Upload the conduit artefacts to Cerebrium
                 print("⬆️  Uploading conduit resources...")
                 self._upload(upload_url)
                 print("✅ Conduit resources uploaded successfully.")
-                _poll_deployment_status(self.api_key, build_id, self.name, project_id, endpoint)
+                _poll_deployment_status(
+                    self.api_key, build_id, self.name, project_id, endpoint
+                )
                 return endpoint
         else:
             if self.flow[0][0] == ModelType.PREBUILT:
                 raise NotImplementedError("Dry run not supported for prebuilt models")
             self.load(direct_from_flow=True)
             return self
```

### Comparing `cerebrium-1.0.5/cerebrium/core.py` & `cerebrium-1.0.6/cerebrium/core.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.0.5/cerebrium/errors.py` & `cerebrium-1.0.6/cerebrium/errors.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,18 +10,16 @@
     def __init__(self, status_code, endpoint, data={}):
         self.status_code = status_code
         self.endpoint = endpoint
         self.data = data
         super().__init__(self.status_code)
 
     def __str__(self):
-        msg = (
-                f"{self.status_code}\n`{self.endpoint}` API Call Failed.\n{self.data}."
-            )
-        
+        msg = f"{self.status_code}\n`{self.endpoint}` API Call Failed.\n{self.data}."
+
         if self.status_code == 401:
             msg = f"{self.status_code}\n`{self.endpoint} API key does not exist or is incorrect. If your key is correct, please contact the Cerebrium team."
         elif self.status_code == 403:
             plan_limits = self.data.get("planLimits")
             if plan_limits:
                 can_deploy_model = plan_limits.get("canDeployModel")
                 number_of_plan_models = plan_limits.get("numberOfPlanModels")
@@ -37,15 +35,15 @@
                 else " " + self.data.get("message", "") + "."
             )
             msg = f"{self.status_code}\n`{self.endpoint}` API Call Failed.{specific_message}"
         elif self.status_code == 500:
             msg = f"{self.status_code}\n`{self.endpoint}` API Call Failed. Internal Server Error: {self.data}."
         elif self.status_code == 502:
             msg = f"{self.status_code}\n`{self.endpoint}` API Call Failed. Bad Gateway."
-    
+
         return msg
 
 
 class CerebriumDeploymentError(Exception):
     """
     Class to handle the error code messages from the Cerebrium API.
```

### Comparing `cerebrium-1.0.5/cerebrium/flow.py` & `cerebrium-1.0.6/cerebrium/flow.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,21 @@
-from typing import Tuple, List, Dict, Literal
+from typing import Tuple, List, Dict, Literal, Union
 from types import FunctionType
 from inspect import getsource
 from pathlib import Path
 from cerebrium.models.base import ModelType
 
-CerebriumModel = Tuple[ModelType, str | dict, Dict[Literal["pre"] | Literal["post"], FunctionType] | None]
+CerebriumModel = Tuple[
+    ModelType,
+    Union[str, dict],
+    Union[Dict[Union[Literal["pre"], Literal["post"]], FunctionType], None],
+]
 CerebriumFlow = List[CerebriumModel]
 
+
 def _flow_string(flow: CerebriumFlow):
     """
     Convert a flow to a string.
 
     Args:
         flow (CerebriumFlow): The flow to convert.
 
@@ -38,36 +43,38 @@
     """
     argument_bracket_1 = def_string.find("(")
     argument_bracket_2 = def_string.find(")")
     argument_str = def_string[argument_bracket_1 + 1 : argument_bracket_2]
     return argument_str.split(",")
 
 
-def _check_input_tuple(model_flow: CerebriumFlow | CerebriumModel) -> CerebriumFlow:
+def _check_input_tuple(
+    model_flow: Union[CerebriumFlow, CerebriumModel]
+) -> CerebriumFlow:
     # if a CerebriumModel is passed, wrap it in a list
-    wrapped_flow = model_flow # type: ignore
+    wrapped_flow = model_flow  # type: ignore
     if len(model_flow) == 2:
         if (
             not isinstance(model_flow[0], list)
             and not isinstance(model_flow[0], tuple)
             and not isinstance(model_flow[1], list)
             and not isinstance(model_flow[1], tuple)
         ):
-            wrapped_flow: CerebriumFlow = [model_flow] # type: ignore
+            wrapped_flow: CerebriumFlow = [model_flow]  # type: ignore
     elif len(model_flow) == 3:
         if (
             not isinstance(model_flow[0], list)
             and not isinstance(model_flow[0], tuple)
             and not isinstance(model_flow[1], list)
             and not isinstance(model_flow[1], tuple)
             and not isinstance(model_flow[2], list)
             and not isinstance(model_flow[2], tuple)
         ):
-            wrapped_flow: CerebriumFlow = [model_flow] # type: ignore
-        
+            wrapped_flow: CerebriumFlow = [model_flow]  # type: ignore
+
     return wrapped_flow
 
 
 def _check_special_model(model_flow: CerebriumFlow) -> None:
     """
     Check if the model flow is a special model type. (These are handled differently, and so require a different check.)
 
@@ -81,15 +88,17 @@
         if len(model_flow) != 1:
             raise TypeError(
                 f"Prebuilt models must be a tuple or list of length 1, but is {len(model_flow)}"
             )
 
 
 def _check_valid_model(
-    model_type: ModelType, model_initialization: str | dict, pipeline_position: int
+    model_type: ModelType,
+    model_initialization: Union[str, dict],
+    pipeline_position: int,
 ):
     """
     Check that the model is valid, raising an error if not.
 
     Args:
         model_type: The type of the model.
         model_initialization: The initialization values needed for the Cerebrium model. For most models, this is a string filepath to the model.
@@ -207,15 +216,15 @@
             contains_return = [s.strip()[:6] == "return" for s in processor_str]
             if not any(contains_return):
                 raise NotImplementedError(
                     f"Model {processor}: The {stage}-processing function must return a value, but does not."
                 )
 
 
-def _check_flow_type(model_flow: CerebriumFlow | CerebriumModel) -> CerebriumFlow:
+def _check_flow_type(model_flow: Union[CerebriumFlow, CerebriumModel]) -> CerebriumFlow:
     """
     Check if the given model_flow is a valid CerebriumFlow.
 
     Args:
         model_flow: The model_flow to check.
 
     Returns:
@@ -250,15 +259,15 @@
                     model_type,
                     model_initialization,
                     {"post": flow_component[2]},
                 )
             else:
                 # Check if the processing functions are valid
                 keys = set(flow_component[2].keys())
-                remaining_keys = keys - {"post", "pre"} # type: ignore
+                remaining_keys = keys - {"post", "pre"}  # type: ignore
                 if remaining_keys != set():
                     raise TypeError(
                         f"Model {i}: The processing functions contains invalid keys {str(remaining_keys)}. Please use only 'post' and 'pre'."
                     )
                 if "post" in flow_component[2]:
                     post = flow_component[2]["post"]
                     _check_processor(post, i, "post")
```

### Comparing `cerebrium-1.0.5/cerebrium/logging/arize.py` & `cerebrium-1.0.6/cerebrium/logging/arize.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.0.5/cerebrium/logging/base.py` & `cerebrium-1.0.6/cerebrium/logging/base.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.0.5/cerebrium/logging/censius.py` & `cerebrium-1.0.6/cerebrium/logging/censius.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.0.5/cerebrium/models/base.py` & `cerebrium-1.0.6/cerebrium/models/base.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.0.5/cerebrium/models/sklearn.py` & `cerebrium-1.0.6/cerebrium/models/sklearn.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.0.5/cerebrium/requests.py` & `cerebrium-1.0.6/cerebrium/requests.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import requests
 import json
 import os
 import time
 import re
 from termcolor import colored
-from typing import Tuple
+from typing import Tuple, Union
 from tenacity import retry, stop_after_delay, wait_fixed
 from yaspin import yaspin
 from yaspin.spinners import Spinners
 from cerebrium.errors import CerebriumRequestError, CerebriumDeploymentError
 
 
 ENV = os.getenv("DEVELOPMENT_ENV", "prod")
@@ -46,15 +46,15 @@
             raise ValueError(f"Payload for '{method}' must contain 'name' key")
 
 
 def _cerebrium_request(
     method: str,
     http_method: str,
     api_key: str,
-    payload: dict | None = None,
+    payload: Union[dict, None] = None,
     enable_spinner: Tuple[bool, Tuple[str, str]] = (False, ("", "")),
 ) -> dict:
     """
     Make a request to the Cerebrium API.
 
     Args:
         method (str): The server method to use.
@@ -93,15 +93,17 @@
             )
     else:
         response = _request()
     return response
 
 
 @retry(stop=stop_after_delay(60), wait=wait_fixed(2))
-def _poll_deployment_status(api_key: str, build_id: str, name: str, project_id: str, endpoint: str):
+def _poll_deployment_status(
+    api_key: str, build_id: str, name: str, project_id: str, endpoint: str
+):
     """
     Poll the deployment status of a conduit.
 
     Args:
         conduit_name (str): The name of the conduit to check the status of.
         api_key (str): The API key for the Cerebrium account.
 
@@ -140,23 +142,23 @@
                     if message:
                         match = re.match(
                             r"^(\d{4}-\d{2}-\d{2}T\d{2}:\d{2}:\d{2}\.\d{9})Z ", message
                         )
                         if (
                             match is not None
                         ):  # If the regex matches the beginning of the string
-                            created = match.group(1)  # The first group is the creation time
-                            message = message[
-                                len(created) + 2 :
-                            ]
+                            created = match.group(
+                                1
+                            )  # The first group is the creation time
+                            message = message[len(created) + 2 :]
                         spinner.write(f"{message}")
                     else:
                         spinner.write("\n")
                 seen_index = len(logs)
-                spinner.text = f"🔨 Building... Status: {build_status}"    
+                spinner.text = f"🔨 Building... Status: {build_status}"
                 time.sleep(1)
             if time.time() - t1 > 600:
                 spinner.fail("Build timed out.")
                 raise CerebriumDeploymentError(
                     "Deployment Timed Out. Your conduit might be large and take longer to deploy. Please try again later."
                 )
             elif build_status == "failed":
@@ -164,19 +166,23 @@
                 raise CerebriumDeploymentError(
                     "Deployment Failed. Please check your conduit and try again."
                 )
         spinner.text = f"Status: {build_status}"
         spinner.ok("🚀 Build complete!")
         print("\n🌍 Endpoint:", endpoint)
         print("💡 You can call the endpoint with the following curl command:")
-        print(colored(f"curl -X POST {endpoint} \\\n"
-                      "     -H 'Content-Type: application/json' \\\n"
-                      "     -H 'Authorization: <public_api_key>' \\\n"
-                      "     --data '{}'", "green"))
+        print(
+            colored(
+                f"curl -X POST {endpoint} \\\n"
+                "     -H 'Content-Type: application/json' \\\n"
+                "     -H 'Authorization: <public_api_key>' \\\n"
+                "     --data '{}'",
+                "green",
+            )
+        )
         print("----------------------------------------")
         print(
             f"🔗 View builds: https://dashboard.cerebrium.ai/projects/{project_id}/models/{project_id}-{name}?tab=builds"
         )
         print(
             f"🔗 View runs: https://dashboard.cerebrium.ai/projects/{project_id}/models/{project_id}-{name}?tab=runs"
         )
-
```

### Comparing `cerebrium-1.0.5/pyproject.toml` & `cerebrium-1.0.6/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cerebrium"
-version = "1.0.5"
+version = "1.0.6"
 description = ""
 authors = ["Elijah Roussos <elijah@cerebrium.ai>"]
 license = "AGPL-3.0-only"
 readme = "README.md"
 exclude = ["tests/*", "dist/*", "worker/*", "builder/*", "prebuilt/*", "common/*", "examples/*"]
 
 [tool.poetry.urls]
```

### Comparing `cerebrium-1.0.5/PKG-INFO` & `cerebrium-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cerebrium
-Version: 1.0.5
+Version: 1.0.6
 Summary: 
 License: AGPL-3.0-only
 Author: Elijah Roussos
 Author-email: elijah@cerebrium.ai
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
```

