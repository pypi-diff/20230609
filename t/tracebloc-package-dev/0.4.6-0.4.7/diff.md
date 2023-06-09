# Comparing `tmp/tracebloc_package-dev-0.4.6.tar.gz` & `tmp/tracebloc_package-dev-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tracebloc_package-dev-0.4.6.tar", last modified: Thu Jun  8 23:20:48 2023, max compression
+gzip compressed data, was "tracebloc_package-dev-0.4.7.tar", last modified: Fri Jun  9 08:05:31 2023, max compression
```

## Comparing `tracebloc_package-dev-0.4.6.tar` & `tracebloc_package-dev-0.4.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 divyasingh   (501) staff       (20)        0 2023-06-08 23:20:48.540060 tracebloc_package-dev-0.4.6/
--rw-r--r--   0 divyasingh   (501) staff       (20)     1048 2022-05-03 09:10:47.000000 tracebloc_package-dev-0.4.6/LICENSE.txt
--rw-r--r--   0 divyasingh   (501) staff       (20)      558 2023-06-08 23:20:48.540147 tracebloc_package-dev-0.4.6/PKG-INFO
--rw-r--r--   0 divyasingh   (501) staff       (20)      188 2022-05-03 09:10:47.000000 tracebloc_package-dev-0.4.6/README.md
--rw-r--r--   0 divyasingh   (501) staff       (20)       78 2023-06-08 23:20:48.540451 tracebloc_package-dev-0.4.6/setup.cfg
--rw-r--r--   0 divyasingh   (501) staff       (20)      949 2023-06-08 23:20:39.000000 tracebloc_package-dev-0.4.6/setup.py
-drwxr-xr-x   0 divyasingh   (501) staff       (20)        0 2023-06-08 23:20:48.538646 tracebloc_package-dev-0.4.6/tracebloc_package/
--rw-r--r--   0 divyasingh   (501) staff       (20)       67 2023-06-05 16:08:49.000000 tracebloc_package-dev-0.4.6/tracebloc_package/__init__.py
--rw-r--r--   0 divyasingh   (501) staff       (20)     5669 2023-06-05 16:08:49.000000 tracebloc_package-dev-0.4.6/tracebloc_package/check_parameters.py
--rw-r--r--   0 divyasingh   (501) staff       (20)    21242 2023-06-08 19:36:44.000000 tracebloc_package-dev-0.4.6/tracebloc_package/functional_test.py
--rw-r--r--   0 divyasingh   (501) staff       (20)    60423 2023-06-08 19:36:44.000000 tracebloc_package-dev-0.4.6/tracebloc_package/linkModelDataSet.py
--rw-r--r--   0 divyasingh   (501) staff       (20)     7100 2022-07-01 07:02:58.000000 tracebloc_package-dev-0.4.6/tracebloc_package/messages.py
--rw-r--r--   0 divyasingh   (501) staff       (20)    10184 2023-06-08 19:36:44.000000 tracebloc_package-dev-0.4.6/tracebloc_package/upload.py
--rw-r--r--   0 divyasingh   (501) staff       (20)    10428 2023-06-08 19:36:44.000000 tracebloc_package-dev-0.4.6/tracebloc_package/user.py
--rw-r--r--   0 divyasingh   (501) staff       (20)     5840 2023-06-05 16:08:49.000000 tracebloc_package-dev-0.4.6/tracebloc_package/utils.py
--rw-r--r--   0 divyasingh   (501) staff       (20)     3203 2022-06-09 14:39:28.000000 tracebloc_package-dev-0.4.6/tracebloc_package/weights.py
-drwxr-xr-x   0 divyasingh   (501) staff       (20)        0 2023-06-08 23:20:48.539900 tracebloc_package-dev-0.4.6/tracebloc_package_dev.egg-info/
--rw-r--r--   0 divyasingh   (501) staff       (20)      558 2023-06-08 23:20:48.000000 tracebloc_package-dev-0.4.6/tracebloc_package_dev.egg-info/PKG-INFO
--rw-r--r--   0 divyasingh   (501) staff       (20)      591 2023-06-08 23:20:48.000000 tracebloc_package-dev-0.4.6/tracebloc_package_dev.egg-info/SOURCES.txt
--rw-r--r--   0 divyasingh   (501) staff       (20)        1 2023-06-08 23:20:48.000000 tracebloc_package-dev-0.4.6/tracebloc_package_dev.egg-info/dependency_links.txt
--rw-r--r--   0 divyasingh   (501) staff       (20)        1 2023-06-08 23:20:48.000000 tracebloc_package-dev-0.4.6/tracebloc_package_dev.egg-info/not-zip-safe
--rw-r--r--   0 divyasingh   (501) staff       (20)      119 2023-06-08 23:20:48.000000 tracebloc_package-dev-0.4.6/tracebloc_package_dev.egg-info/requires.txt
--rw-r--r--   0 divyasingh   (501) staff       (20)       18 2023-06-08 23:20:48.000000 tracebloc_package-dev-0.4.6/tracebloc_package_dev.egg-info/top_level.txt
+drwxr-xr-x   0 divyasingh   (501) staff       (20)        0 2023-06-09 08:05:31.438547 tracebloc_package-dev-0.4.7/
+-rw-r--r--   0 divyasingh   (501) staff       (20)     1048 2022-05-03 09:10:47.000000 tracebloc_package-dev-0.4.7/LICENSE.txt
+-rw-r--r--   0 divyasingh   (501) staff       (20)      558 2023-06-09 08:05:31.438608 tracebloc_package-dev-0.4.7/PKG-INFO
+-rw-r--r--   0 divyasingh   (501) staff       (20)      188 2022-05-03 09:10:47.000000 tracebloc_package-dev-0.4.7/README.md
+-rw-r--r--   0 divyasingh   (501) staff       (20)       78 2023-06-09 08:05:31.438810 tracebloc_package-dev-0.4.7/setup.cfg
+-rw-r--r--   0 divyasingh   (501) staff       (20)      949 2023-06-09 08:03:28.000000 tracebloc_package-dev-0.4.7/setup.py
+drwxr-xr-x   0 divyasingh   (501) staff       (20)        0 2023-06-09 08:05:31.437719 tracebloc_package-dev-0.4.7/tracebloc_package/
+-rw-r--r--   0 divyasingh   (501) staff       (20)       67 2023-06-05 16:08:49.000000 tracebloc_package-dev-0.4.7/tracebloc_package/__init__.py
+-rw-r--r--   0 divyasingh   (501) staff       (20)     5669 2023-06-05 16:08:49.000000 tracebloc_package-dev-0.4.7/tracebloc_package/check_parameters.py
+-rw-r--r--   0 divyasingh   (501) staff       (20)    21521 2023-06-09 08:04:05.000000 tracebloc_package-dev-0.4.7/tracebloc_package/functional_test.py
+-rw-r--r--   0 divyasingh   (501) staff       (20)    61149 2023-06-09 08:05:15.000000 tracebloc_package-dev-0.4.7/tracebloc_package/linkModelDataSet.py
+-rw-r--r--   0 divyasingh   (501) staff       (20)     7100 2022-07-01 07:02:58.000000 tracebloc_package-dev-0.4.7/tracebloc_package/messages.py
+-rw-r--r--   0 divyasingh   (501) staff       (20)    10184 2023-06-08 19:36:44.000000 tracebloc_package-dev-0.4.7/tracebloc_package/upload.py
+-rw-r--r--   0 divyasingh   (501) staff       (20)    10427 2023-06-09 08:04:05.000000 tracebloc_package-dev-0.4.7/tracebloc_package/user.py
+-rw-r--r--   0 divyasingh   (501) staff       (20)     5840 2023-06-05 16:08:49.000000 tracebloc_package-dev-0.4.7/tracebloc_package/utils.py
+-rw-r--r--   0 divyasingh   (501) staff       (20)     3200 2023-06-09 08:04:05.000000 tracebloc_package-dev-0.4.7/tracebloc_package/weights.py
+drwxr-xr-x   0 divyasingh   (501) staff       (20)        0 2023-06-09 08:05:31.438447 tracebloc_package-dev-0.4.7/tracebloc_package_dev.egg-info/
+-rw-r--r--   0 divyasingh   (501) staff       (20)      558 2023-06-09 08:05:31.000000 tracebloc_package-dev-0.4.7/tracebloc_package_dev.egg-info/PKG-INFO
+-rw-r--r--   0 divyasingh   (501) staff       (20)      591 2023-06-09 08:05:31.000000 tracebloc_package-dev-0.4.7/tracebloc_package_dev.egg-info/SOURCES.txt
+-rw-r--r--   0 divyasingh   (501) staff       (20)        1 2023-06-09 08:05:31.000000 tracebloc_package-dev-0.4.7/tracebloc_package_dev.egg-info/dependency_links.txt
+-rw-r--r--   0 divyasingh   (501) staff       (20)        1 2023-06-09 08:05:31.000000 tracebloc_package-dev-0.4.7/tracebloc_package_dev.egg-info/not-zip-safe
+-rw-r--r--   0 divyasingh   (501) staff       (20)      119 2023-06-09 08:05:31.000000 tracebloc_package-dev-0.4.7/tracebloc_package_dev.egg-info/requires.txt
+-rw-r--r--   0 divyasingh   (501) staff       (20)       18 2023-06-09 08:05:31.000000 tracebloc_package-dev-0.4.7/tracebloc_package_dev.egg-info/top_level.txt
```

### Comparing `tracebloc_package-dev-0.4.6/LICENSE.txt` & `tracebloc_package-dev-0.4.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.4.6/PKG-INFO` & `tracebloc_package-dev-0.4.7/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tracebloc_package-dev
-Version: 0.4.6
+Version: 0.4.7
 Summary: Package required to run Tracebloc jupyter notebook to create experiment
 Home-page: https://gitlab.com/tracebloc/tracebloc-py-package/-/tree/dev
 Author: Tracebloc
 Author-email: info@tracebloc.io
 License: MIT
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

### Comparing `tracebloc_package-dev-0.4.6/setup.py` & `tracebloc_package-dev-0.4.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="tracebloc_package-dev",
-    version="0.4.6",
+    version="0.4.7",
     description="Package required to run Tracebloc jupyter notebook to create experiment",
     url="https://gitlab.com/tracebloc/tracebloc-py-package/-/tree/dev",
     license="MIT",
     python_requires=">=3",
     packages=["tracebloc_package"],
     author="Tracebloc",
     author_email="info@tracebloc.io",
```

### Comparing `tracebloc_package-dev-0.4.6/tracebloc_package/check_parameters.py` & `tracebloc_package-dev-0.4.7/tracebloc_package/check_parameters.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.4.6/tracebloc_package/functional_test.py` & `tracebloc_package-dev-0.4.7/tracebloc_package/functional_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,32 +89,40 @@
                 remove_lines.append(linenum)
                 if not main_file:
                     self.file_name = os.path.split(temp_file)[1]
                     main_file = True
             if self.framework == TENSORFLOW_FRAMEWORK:
                 for pattern, attribute in tensorflow_pattern_dict.items():
                     if pattern.match(fileline):
-                        setattr(self, attribute, re.sub(
-                            f"({attribute}\s{{0,}}[=]\s{{0,}})",
-                            "",
-                            fileline.replace("'", "").replace('"', ""),
-                        ))
+                        setattr(
+                            self,
+                            attribute,
+                            re.sub(
+                                f"({attribute}\s{{0,}}[=]\s{{0,}})",
+                                "",
+                                fileline.replace("'", "").replace('"', ""),
+                            ),
+                        )
                         remove_lines.append(linenum)
                         if not main_file:
                             self.file_name = os.path.split(temp_file)[1]
                             main_file = True
                         break
             elif self.framework == PYTORCH_FRAMEWORK:
                 for pattern, attribute in pytorch_pattern_dict.items():
                     if pattern.match(fileline):
-                        setattr(self, attribute, re.sub(
-                            f"({attribute}\s{{0,}}[=]\s{{0,}})",
-                            "",
-                            fileline.replace("'", "").replace('"', ""),
-                        ))
+                        setattr(
+                            self,
+                            attribute,
+                            re.sub(
+                                f"({attribute}\s{{0,}}[=]\s{{0,}})",
+                                "",
+                                fileline.replace("'", "").replace('"', ""),
+                            ),
+                        )
                         remove_lines.append(linenum)
                         if not main_file:
                             self.file_name = os.path.split(temp_file)[1]
                             main_file = True
                         break
         if main_file and self.framework == "":
             print("Framework parameter missing from file")
@@ -347,15 +355,17 @@
             eligible = False
         if not eligible:
             return eligible, self.message, None, self.progress_bar  # pragma: no cover
         return True, self.message, self.model_name, self.progress_bar
 
 
 class TensorflowChecks:
-    def __init__(self, model, model_name, message, progress_bar, image_size, batch_size):
+    def __init__(
+        self, model, model_name, message, progress_bar, image_size, batch_size
+    ):
         self.message = message
         self.model = model
         self.model_name = model_name
         self.progress_bar = progress_bar
         self.image_size = image_size
         self.batch_size = batch_size
 
@@ -442,15 +452,17 @@
         eligible, message = self.is_model_eligible()
         if not eligible:
             return eligible, message, None, self.progress_bar  # pragma: no cover
         return True, self.message, self.model_name, self.progress_bar
 
 
 class TorchChecks:
-    def __init__(self, model, model_name, message, progress_bar, image_size, batch_size):
+    def __init__(
+        self, model, model_name, message, progress_bar, image_size, batch_size
+    ):
         self.message = message
         self.model = model
         self.model_name = model_name
         self.progress_bar = progress_bar
         self.image_size = image_size
         self.batch_size = batch_size
 
@@ -475,21 +487,22 @@
             train_dataset = datasets.FakeData(
                 size=num_images,
                 image_size=(num_channels, self.image_size, self.image_size),
                 num_classes=num_classes,
                 transform=transforms.ToTensor(),
             )
 
-            train_loader = DataLoader(train_dataset, batch_size=self.batch_size, shuffle=True)
+            train_loader = DataLoader(
+                train_dataset, batch_size=self.batch_size, shuffle=True
+            )
 
             # train_loader, classes = mock_torch_data(self.tmp_path)
             criterion = nn.CrossEntropyLoss()
             optimizer = optim.SGD(self.model.parameters(), lr=0.001, momentum=0.9)
             for epoch in range(1):  # loop over the dataset multiple times
-
                 running_loss = 0.0
                 for i, data in enumerate(train_loader, 0):
                     # get the inputs; data is a list of [inputs, labels]
                     inputs, labels = data
                     labels = torch.tensor(labels, dtype=torch.long)
                     # zero the parameter gradients
                     optimizer.zero_grad()
@@ -500,17 +513,15 @@
                     loss.backward()
                     optimizer.step()
 
                     # print statistics
                     running_loss += loss.item()
             self.progress_bar.update(1)
         except Exception as e:  # pragma: no cover
-            self.message = (
-                f"\nModel not support training on image classification dataset as there is error {e} "
-            )
+            self.message = f"\nModel not support training on image classification dataset as there is error {e} "
             raise
 
     def model_func_checks(self):
         # check if model is eligible
         try:
             self.is_model_supported()
             self.progress_bar.update(2)
```

### Comparing `tracebloc_package-dev-0.4.6/tracebloc_package/linkModelDataSet.py` & `tracebloc_package-dev-0.4.7/tracebloc_package/linkModelDataSet.py`

 * *Files 0% similar despite different names*

```diff
@@ -216,15 +216,19 @@
             header = {"Authorization": f"Token {self.__token}"}
             data = {
                 "edges_involved": json.dumps(list(self.__total_images.keys())),
                 "images_per_class": json.dumps(training_dataset),
                 "type": "recalculate_image_count_per_edge",
                 "datasetId": self.__datasetId,
             }
-            re = requests.post(f"{self.__url}check-model/", headers=header, data=data,)
+            re = requests.post(
+                f"{self.__url}check-model/",
+                headers=header,
+                data=data,
+            )
             body_unicode = re.content.decode("utf-8")
             content = json.loads(body_unicode)
             if re.status_code == 200:
                 self.__total_images = content["total_images_per_edge"]
                 self.__validation_split = self.__default_validation_split()
                 self.__images_per_class = json.dumps(
                     training_dataset
@@ -261,41 +265,50 @@
     def imageShape(self, image_shape: int):
         """
         Set image shape
         parameters: integer. value must be between 48 and 224
         example: trainingObject.imageShape(224)
         default: 224
         maximum value : 224
+        warning : for pytorch please only imageshape for which layers are designed and is specified in model file is allowed
         """
-        if type(image_shape) is int and (48 <= image_shape <= 224):
-            self.__image_shape = image_shape
-            self.__update_image_model()
-            self.__remove_error_method()
+        if self.__framework == TENSORFLOW_FRAMEWORK:
+            if type(image_shape) is int and (48 <= image_shape <= 224):
+                self.__image_shape = image_shape
+                self.__update_image_model()
+                self.__remove_error_method()
+            else:
+                error_msg = "Invalid input type or value '0' given for image shape"
+                self.__print_error(error_msg)
         else:
-            error_msg = "Invalid input type or value '0' given for image shape"
-            self.__print_error(error_msg)
+            error_msg = "for pytorch shape is fixed for each model"
+            self.__not_supported_parameters(error_msg)
 
     def imageType(self, image_type: str):
         """
         Set image type to be used for training
         parameters: string type values.
         supported type: ['rgb', 'gray']
         example: trainingObject.imageType('rgb')
         default: rgb
         """
-        allowed_types = ["rgb", "grayscale"]
-        try:
-            if type(image_type) is str:
-                allowed_types.index(image_type.lower())
-                self.__image_type = image_type.lower()
-                self.__update_image_model()
-                self.__remove_error_method()
-        except:
-            error_msg = "Enter values from supported values only "
-            self.__print_error(error_msg)
+        if self.__framework == TENSORFLOW_FRAMEWORK:
+            allowed_types = ["rgb", "grayscale"]
+            try:
+                if type(image_type) is str:
+                    allowed_types.index(image_type.lower())
+                    self.__image_type = image_type.lower()
+                    self.__update_image_model()
+                    self.__remove_error_method()
+            except:
+                error_msg = "Enter values from supported values only "
+                self.__print_error(error_msg)
+        else:
+            error_msg = "for pytorch only rgb is supported"
+            self.__not_supported_parameters(error_msg)
 
     def seed(self, seed: bool):
         """
         Boolean.
         Sets the global random seed when selected
         default: False
         example:trainingObject.seed(True)
@@ -439,15 +452,16 @@
             error_msg = f"Invalid input type or set value not less than {minimum} for validation_split\n"
             self.__print_error(error_msg)
 
     def optimizer(self, optimizer: str):
         """
         String (name of optimizer)
         example: trainingObject.optimizer('rmsprop')
-        supported optimizers: ['adam','rmsprop','sgd','adadelta', 'adagrad', 'adamax','nadam', 'ftrl']
+        supported optimizers: ['adam','rmsprop','sgd','adadelta', 'adagrad', 'adamax','nadam', 'ftrl'] for tensorflow
+        supported optimizers: ["adam", "rmsprop", "sgd", "adadelta", "adagrad", "adamax", "ftrl"] for pytorch
         default: 'sgd'
         """
         if self.__framework == TENSORFLOW_FRAMEWORK:
             o = [
                 "adam",
                 "rmsprop",
                 "sgd",
@@ -480,15 +494,14 @@
             o = [
                 "adam",
                 "rmsprop",
                 "sgd",
                 "adadelta",
                 "adagrad",
                 "adamax",
-                "nadam",
                 "ftrl",
             ]
             try:
                 o.index(optimizer)
                 self.__optimizer = optimizer
                 self.__remove_error_method()
             except:
@@ -912,15 +925,14 @@
         example: trainingObject.brightness_range((0.1,0.4))
         default: None
         """
         if self.__framework == TENSORFLOW_FRAMEWORK:
             if (type(brightness_range) == tuple and len(brightness_range) == 2) or (
                 type(brightness_range) == list and len(brightness_range)
             ) == 2:
-
                 if (
                     type(brightness_range[0]) == float
                     and type(brightness_range[1]) == float
                 ):
                     brightness_range = str(brightness_range)
                     self.__brightness_range = brightness_range
                     self.__remove_error_method()
```

### Comparing `tracebloc_package-dev-0.4.6/tracebloc_package/messages.py` & `tracebloc_package-dev-0.4.7/tracebloc_package/messages.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.4.6/tracebloc_package/upload.py` & `tracebloc_package-dev-0.4.7/tracebloc_package/upload.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.4.6/tracebloc_package/user.py` & `tracebloc_package-dev-0.4.7/tracebloc_package/user.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,14 @@
                 print("You have been logged out.")
             else:
                 print("Logout Failed. Retry!")
         except Exception as e:
             print("Logout Failed. Retry!")
 
     def uploadModel(self, modelname: str, weights=False):
-
         """
         Make sure model file and weights are in current directory
         Parameters: modelname
 
         modelname: model file name eg: vggnet, if file name is vggnet.py
         weights: upload pre trained weights if set True. Default: False
 
@@ -122,15 +121,15 @@
             (
                 self.__modelId,
                 self.__modelName,
                 self.__ext,
                 path,
                 self.__framework,
                 self.__image_size,
-                self.__batch_size
+                self.__batch_size,
             ) = modelobj.getNewModelId()
             self.__model = modelobj.model
             if self.__modelId == "" or self.__modelId is None:
                 text = colored(f"'{self.__modelName}' upload Failed.", "red")
                 print(text, "\n")
                 self.__weights = False
                 return
@@ -138,15 +137,14 @@
                 text = colored(f"\n'{self.__modelName}' upload successful.", "green")
                 print(text, "\n")
 
         except:
             return
 
     def linkModelDataset(self, datasetId: str):
-
         """
         Role: Link and checks model & datasetId compatibility
               create training plan object
 
         parameters: modelId, datasetId
         return: training plan object
         """
```

### Comparing `tracebloc_package-dev-0.4.6/tracebloc_package/utils.py` & `tracebloc_package-dev-0.4.7/tracebloc_package/utils.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.4.6/tracebloc_package/weights.py` & `tracebloc_package-dev-0.4.7/tracebloc_package/weights.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,19 +13,17 @@
     ***
     Please provide a valid username and password
     Call getToken method on Login to get new token for provided
     username and password
     """
 
     def __init__(self):
-
         self.__modelname = input("Enter Model Name : ")
 
     def generateweights(self):
-
         """
         Make sure model file is in current directory
         Parameters: modelname
 
         modelname: model file name eg: vggnet, if file name is vggnet.py
         *******
         return: weights file
@@ -59,15 +57,14 @@
                 print(f"Dumped new weights for {self.__modelname} model")
             except Exception as e:
                 print(f"Weights dump failed.\n")
         except Exception as e:
             print(f"{self.__modelname} Model load failed.\n")
 
     def checkweights(self):
-
         """
         Role: Check if weight are correct
         return: weights Summary
         """
         # Load weights to check if it works
         try:
             if os.path.exists(self.__modelname + ".py"):
```

### Comparing `tracebloc_package-dev-0.4.6/tracebloc_package_dev.egg-info/PKG-INFO` & `tracebloc_package-dev-0.4.7/tracebloc_package_dev.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tracebloc-package-dev
-Version: 0.4.6
+Version: 0.4.7
 Summary: Package required to run Tracebloc jupyter notebook to create experiment
 Home-page: https://gitlab.com/tracebloc/tracebloc-py-package/-/tree/dev
 Author: Tracebloc
 Author-email: info@tracebloc.io
 License: MIT
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

### Comparing `tracebloc_package-dev-0.4.6/tracebloc_package_dev.egg-info/SOURCES.txt` & `tracebloc_package-dev-0.4.7/tracebloc_package_dev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

