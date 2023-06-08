# Comparing `tmp/tracebloc_package-dev-0.4.5.tar.gz` & `tmp/tracebloc_package-dev-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tracebloc_package-dev-0.4.5.tar", last modified: Wed Jun  7 07:45:33 2023, max compression
+gzip compressed data, was "tracebloc_package-dev-0.4.6.tar", last modified: Thu Jun  8 23:20:48 2023, max compression
```

## Comparing `tracebloc_package-dev-0.4.5.tar` & `tracebloc_package-dev-0.4.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 hasan      (501) staff       (20)        0 2023-06-07 07:45:33.619424 tracebloc_package-dev-0.4.5/
--rw-r--r--   0 hasan      (501) staff       (20)     1048 2022-05-16 08:30:43.000000 tracebloc_package-dev-0.4.5/LICENSE.txt
--rw-r--r--   0 hasan      (501) staff       (20)      577 2023-06-07 07:45:33.619510 tracebloc_package-dev-0.4.5/PKG-INFO
--rw-r--r--   0 hasan      (501) staff       (20)      188 2022-05-16 08:30:43.000000 tracebloc_package-dev-0.4.5/README.md
--rw-r--r--   0 hasan      (501) staff       (20)       78 2023-06-07 07:45:33.619821 tracebloc_package-dev-0.4.5/setup.cfg
--rw-r--r--   0 hasan      (501) staff       (20)      949 2023-06-07 07:43:59.000000 tracebloc_package-dev-0.4.5/setup.py
-drwxr-xr-x   0 hasan      (501) staff       (20)        0 2023-06-07 07:45:33.618034 tracebloc_package-dev-0.4.5/tracebloc_package/
--rw-r--r--   0 hasan      (501) staff       (20)       67 2023-03-15 10:59:39.000000 tracebloc_package-dev-0.4.5/tracebloc_package/__init__.py
--rw-r--r--   0 hasan      (501) staff       (20)     5669 2023-05-18 09:32:19.000000 tracebloc_package-dev-0.4.5/tracebloc_package/check_parameters.py
--rw-r--r--   0 hasan      (501) staff       (20)    20998 2023-06-07 07:44:09.000000 tracebloc_package-dev-0.4.5/tracebloc_package/functional_test.py
--rw-r--r--   0 hasan      (501) staff       (20)    60286 2023-06-07 07:44:09.000000 tracebloc_package-dev-0.4.5/tracebloc_package/linkModelDataSet.py
--rw-r--r--   0 hasan      (501) staff       (20)     7100 2023-03-23 11:28:43.000000 tracebloc_package-dev-0.4.5/tracebloc_package/messages.py
--rw-r--r--   0 hasan      (501) staff       (20)     9821 2023-06-07 07:44:08.000000 tracebloc_package-dev-0.4.5/tracebloc_package/upload.py
--rw-r--r--   0 hasan      (501) staff       (20)    10203 2023-06-07 07:44:08.000000 tracebloc_package-dev-0.4.5/tracebloc_package/user.py
--rw-r--r--   0 hasan      (501) staff       (20)     5840 2023-06-01 09:06:49.000000 tracebloc_package-dev-0.4.5/tracebloc_package/utils.py
--rw-r--r--   0 hasan      (501) staff       (20)     3203 2022-06-09 05:22:24.000000 tracebloc_package-dev-0.4.5/tracebloc_package/weights.py
-drwxr-xr-x   0 hasan      (501) staff       (20)        0 2023-06-07 07:45:33.619221 tracebloc_package-dev-0.4.5/tracebloc_package_dev.egg-info/
--rw-r--r--   0 hasan      (501) staff       (20)      577 2023-06-07 07:45:33.000000 tracebloc_package-dev-0.4.5/tracebloc_package_dev.egg-info/PKG-INFO
--rw-r--r--   0 hasan      (501) staff       (20)      591 2023-06-07 07:45:33.000000 tracebloc_package-dev-0.4.5/tracebloc_package_dev.egg-info/SOURCES.txt
--rw-r--r--   0 hasan      (501) staff       (20)        1 2023-06-07 07:45:33.000000 tracebloc_package-dev-0.4.5/tracebloc_package_dev.egg-info/dependency_links.txt
--rw-r--r--   0 hasan      (501) staff       (20)        1 2023-06-07 07:45:33.000000 tracebloc_package-dev-0.4.5/tracebloc_package_dev.egg-info/not-zip-safe
--rw-r--r--   0 hasan      (501) staff       (20)      119 2023-06-07 07:45:33.000000 tracebloc_package-dev-0.4.5/tracebloc_package_dev.egg-info/requires.txt
--rw-r--r--   0 hasan      (501) staff       (20)       18 2023-06-07 07:45:33.000000 tracebloc_package-dev-0.4.5/tracebloc_package_dev.egg-info/top_level.txt
+drwxr-xr-x   0 divyasingh   (501) staff       (20)        0 2023-06-08 23:20:48.540060 tracebloc_package-dev-0.4.6/
+-rw-r--r--   0 divyasingh   (501) staff       (20)     1048 2022-05-03 09:10:47.000000 tracebloc_package-dev-0.4.6/LICENSE.txt
+-rw-r--r--   0 divyasingh   (501) staff       (20)      558 2023-06-08 23:20:48.540147 tracebloc_package-dev-0.4.6/PKG-INFO
+-rw-r--r--   0 divyasingh   (501) staff       (20)      188 2022-05-03 09:10:47.000000 tracebloc_package-dev-0.4.6/README.md
+-rw-r--r--   0 divyasingh   (501) staff       (20)       78 2023-06-08 23:20:48.540451 tracebloc_package-dev-0.4.6/setup.cfg
+-rw-r--r--   0 divyasingh   (501) staff       (20)      949 2023-06-08 23:20:39.000000 tracebloc_package-dev-0.4.6/setup.py
+drwxr-xr-x   0 divyasingh   (501) staff       (20)        0 2023-06-08 23:20:48.538646 tracebloc_package-dev-0.4.6/tracebloc_package/
+-rw-r--r--   0 divyasingh   (501) staff       (20)       67 2023-06-05 16:08:49.000000 tracebloc_package-dev-0.4.6/tracebloc_package/__init__.py
+-rw-r--r--   0 divyasingh   (501) staff       (20)     5669 2023-06-05 16:08:49.000000 tracebloc_package-dev-0.4.6/tracebloc_package/check_parameters.py
+-rw-r--r--   0 divyasingh   (501) staff       (20)    21242 2023-06-08 19:36:44.000000 tracebloc_package-dev-0.4.6/tracebloc_package/functional_test.py
+-rw-r--r--   0 divyasingh   (501) staff       (20)    60423 2023-06-08 19:36:44.000000 tracebloc_package-dev-0.4.6/tracebloc_package/linkModelDataSet.py
+-rw-r--r--   0 divyasingh   (501) staff       (20)     7100 2022-07-01 07:02:58.000000 tracebloc_package-dev-0.4.6/tracebloc_package/messages.py
+-rw-r--r--   0 divyasingh   (501) staff       (20)    10184 2023-06-08 19:36:44.000000 tracebloc_package-dev-0.4.6/tracebloc_package/upload.py
+-rw-r--r--   0 divyasingh   (501) staff       (20)    10428 2023-06-08 19:36:44.000000 tracebloc_package-dev-0.4.6/tracebloc_package/user.py
+-rw-r--r--   0 divyasingh   (501) staff       (20)     5840 2023-06-05 16:08:49.000000 tracebloc_package-dev-0.4.6/tracebloc_package/utils.py
+-rw-r--r--   0 divyasingh   (501) staff       (20)     3203 2022-06-09 14:39:28.000000 tracebloc_package-dev-0.4.6/tracebloc_package/weights.py
+drwxr-xr-x   0 divyasingh   (501) staff       (20)        0 2023-06-08 23:20:48.539900 tracebloc_package-dev-0.4.6/tracebloc_package_dev.egg-info/
+-rw-r--r--   0 divyasingh   (501) staff       (20)      558 2023-06-08 23:20:48.000000 tracebloc_package-dev-0.4.6/tracebloc_package_dev.egg-info/PKG-INFO
+-rw-r--r--   0 divyasingh   (501) staff       (20)      591 2023-06-08 23:20:48.000000 tracebloc_package-dev-0.4.6/tracebloc_package_dev.egg-info/SOURCES.txt
+-rw-r--r--   0 divyasingh   (501) staff       (20)        1 2023-06-08 23:20:48.000000 tracebloc_package-dev-0.4.6/tracebloc_package_dev.egg-info/dependency_links.txt
+-rw-r--r--   0 divyasingh   (501) staff       (20)        1 2023-06-08 23:20:48.000000 tracebloc_package-dev-0.4.6/tracebloc_package_dev.egg-info/not-zip-safe
+-rw-r--r--   0 divyasingh   (501) staff       (20)      119 2023-06-08 23:20:48.000000 tracebloc_package-dev-0.4.6/tracebloc_package_dev.egg-info/requires.txt
+-rw-r--r--   0 divyasingh   (501) staff       (20)       18 2023-06-08 23:20:48.000000 tracebloc_package-dev-0.4.6/tracebloc_package_dev.egg-info/top_level.txt
```

### Comparing `tracebloc_package-dev-0.4.5/LICENSE.txt` & `tracebloc_package-dev-0.4.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.4.5/PKG-INFO` & `tracebloc_package-dev-0.4.6/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 Metadata-Version: 2.1
 Name: tracebloc_package-dev
-Version: 0.4.5
+Version: 0.4.6
 Summary: Package required to run Tracebloc jupyter notebook to create experiment
 Home-page: https://gitlab.com/tracebloc/tracebloc-py-package/-/tree/dev
 Author: Tracebloc
 Author-email: info@tracebloc.io
 License: MIT
-Platform: UNKNOWN
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Tracebloc package
 This packeg is pre-requiste to run tracebloc jupyter notebook.
 
 
 This package helps to create and start the experiment for training ML models in 
 tracebloc environment.
-
```

### Comparing `tracebloc_package-dev-0.4.5/setup.py` & `tracebloc_package-dev-0.4.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="tracebloc_package-dev",
-    version="0.4.5",
+    version="0.4.6",
     description="Package required to run Tracebloc jupyter notebook to create experiment",
     url="https://gitlab.com/tracebloc/tracebloc-py-package/-/tree/dev",
     license="MIT",
     python_requires=">=3",
     packages=["tracebloc_package"],
     author="Tracebloc",
     author_email="info@tracebloc.io",
```

### Comparing `tracebloc_package-dev-0.4.5/tracebloc_package/check_parameters.py` & `tracebloc_package-dev-0.4.6/tracebloc_package/check_parameters.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.4.5/tracebloc_package/functional_test.py` & `tracebloc_package-dev-0.4.6/tracebloc_package/functional_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,39 +18,43 @@
 class CheckModel:
     MAX_MODEL_NAME_LENGTH = 64
     message = ""
     model = None
     tmp_file_path = ""
     file_name = "model.py"
     tmp_file = ""
-    method_name = ""
-    class_name = ""
+    main_method = ""
+    main_class = ""
     input_shape = ""
     output_classes = ""
+    image_size = 224
+    batch_size = 16
     framework = ""
     notallowed = ["__MACOSX", "__pycache__"]
     input_shape_patt = re.compile("(^input_shape\s{0,}[=]\s{0,}[a-zA-Z_\-0-9'\"])")
     out_classes_patt = re.compile("(^output_classes\s{0,}[=]\s{0,}[a-zA-Z_\-0-9'\"])")
     main_method_patt = re.compile("(^main_method\s{0,}[=]\s{0,}[a-zA-Z_\-0-9'\"])")
     main_class_patt = re.compile("(^main_class\s{0,}[=]\s{0,}[a-zA-Z_\-0-9'\"])")
     framework_patt = re.compile("(^framework\s{0,}[=]\s{0,}[a-zA-Z_\-0-9'\"])")
+    image_size_patt = re.compile("(^image_size\s{0,}[=]\s{0,}[a-zA-Z_\-0-9'\"])")
+    batch_size_patt = re.compile("(^batch_size\s{0,}[=]\s{0,}[a-zA-Z_\-0-9'\"])")
 
     def __init__(
         self, progress_bar, model_name=None, model_path=None
     ):  # pragma: no cover
         self.model_name = model_name
         self.model_path = model_path
         self.progress_bar = progress_bar
 
     def prepare_file(self, temp_file):
         try:
             main_file, remove_lines, filelines = self.get_variables(temp_file)
             if main_file and self.framework == TENSORFLOW_FRAMEWORK:
                 self.tmp_file = os.path.join(self.tmp_file_path, self.file_name)
-                if self.method_name == "":
+                if self.main_method == "":
                     self.load_model(temp_file)
                     self.add_method(temp_file, remove_lines)
                 else:
                     self.edit_file(temp_file, filelines, remove_lines)
             elif self.framework == PYTORCH_FRAMEWORK:
                 self.tmp_file = os.path.join(self.tmp_file_path, self.file_name)
                 self.edit_file(temp_file, filelines, remove_lines)
@@ -61,65 +65,62 @@
 
     def get_variables(self, temp_file):
         main_file = False
         remove_lines = []
         with open(temp_file, "r") as tmp_fp:
             filedata = tmp_fp.read()
         filelines = filedata.split("\n")
+        tensorflow_pattern_dict = {
+            self.input_shape_patt: "input_shape",
+            self.out_classes_patt: "output_classes",
+            self.main_method_patt: "main_method",
+        }
+        pytorch_pattern_dict = {
+            self.main_class_patt: "main_class",
+            self.image_size_patt: "image_size",
+            self.batch_size_patt: "batch_size",
+        }
         for linenum, fileline in enumerate(filelines):
             if self.framework_patt.match(fileline):
                 self.framework = re.sub(
                     "(framework\s{0,}[=]\s{0,})",
                     "",
                     fileline.replace("'", "").replace('"', ""),
                 )
                 remove_lines.append(linenum)
                 if not main_file:
                     self.file_name = os.path.split(temp_file)[1]
                     main_file = True
             if self.framework == TENSORFLOW_FRAMEWORK:
-                if (
-                    self.input_shape_patt.match(fileline)
-                    or self.out_classes_patt.match(fileline)
-                    or self.main_method_patt.match(fileline)
-                ):
-                    if self.input_shape_patt.match(fileline):
-                        self.input_shape = re.sub(
-                            "(input_shape\s{0,}[=]\s{0,})",
+                for pattern, attribute in tensorflow_pattern_dict.items():
+                    if pattern.match(fileline):
+                        setattr(self, attribute, re.sub(
+                            f"({attribute}\s{{0,}}[=]\s{{0,}})",
                             "",
                             fileline.replace("'", "").replace('"', ""),
-                        )
-                    elif self.out_classes_patt.match(fileline):
-                        self.output_classes = re.sub(
-                            "(output_classes\s{0,}[=]\s{0,})",
-                            "",
-                            fileline.replace("'", "").replace('"', ""),
-                        )
-                    elif self.main_method_patt.match(fileline):
-                        self.method_name = re.sub(
-                            "(main_method\s{0,}[=]\s{0,})",
+                        ))
+                        remove_lines.append(linenum)
+                        if not main_file:
+                            self.file_name = os.path.split(temp_file)[1]
+                            main_file = True
+                        break
+            elif self.framework == PYTORCH_FRAMEWORK:
+                for pattern, attribute in pytorch_pattern_dict.items():
+                    if pattern.match(fileline):
+                        setattr(self, attribute, re.sub(
+                            f"({attribute}\s{{0,}}[=]\s{{0,}})",
                             "",
                             fileline.replace("'", "").replace('"', ""),
-                        )
-                    remove_lines.append(linenum)
-                    if not main_file:
-                        self.file_name = os.path.split(temp_file)[1]
-                        main_file = True
-            elif self.framework == PYTORCH_FRAMEWORK:
-                if self.main_class_patt.match(fileline):
-                    self.class_name = re.sub(
-                        "(main_class\s{0,}[=]\s{0,})",
-                        "",
-                        fileline.replace("'", "").replace('"', ""),
-                    )
-                    remove_lines.append(linenum)
-                    if not main_file:
-                        self.file_name = os.path.split(temp_file)[1]
-                        main_file = True
-        if self.framework == "":
+                        ))
+                        remove_lines.append(linenum)
+                        if not main_file:
+                            self.file_name = os.path.split(temp_file)[1]
+                            main_file = True
+                        break
+        if main_file and self.framework == "":
             print("Framework parameter missing from file")
             return False, [], []
         tmp_fp.close()
         return main_file, remove_lines, filelines
 
     def replace_vars(self, code):
         if re.search(
@@ -150,22 +151,22 @@
         edited_data = []
         with open(temp_file, "w") as tmp_fp:
             for linenum, fileline in enumerate(filelines):
                 if linenum in remove_lines:
                     continue
                 else:
                     if self.framework == TENSORFLOW_FRAMEWORK:
-                        if re.search(f"def {self.method_name}\(.*\)", fileline):
+                        if re.search(f"def {self.main_method}\(.*\)", fileline):
                             fileline = fileline.replace(
-                                str(self.method_name), "MyModel"
+                                str(self.main_method), "MyModel"
                             )
                         fileline = self.replace_vars(fileline)
                     elif self.framework == PYTORCH_FRAMEWORK:
-                        if re.search(f"class {self.class_name}\(.*\)", fileline):
-                            fileline = fileline.replace(str(self.class_name), "MyModel")
+                        if re.search(f"class {self.main_class}\(.*\)", fileline):
+                            fileline = fileline.replace(str(self.main_class), "MyModel")
                     edited_data.append(fileline)
             tmp_fp.writelines("\n".join(edited_data))
         tmp_fp.close()
 
     def get_imports(self, codelines):
         instructions = dis.get_instructions(codelines)
         instructions = [__ for __ in instructions]
@@ -346,19 +347,21 @@
             eligible = False
         if not eligible:
             return eligible, self.message, None, self.progress_bar  # pragma: no cover
         return True, self.message, self.model_name, self.progress_bar
 
 
 class TensorflowChecks:
-    def __init__(self, model, model_name, message, progress_bar):
+    def __init__(self, model, model_name, message, progress_bar, image_size, batch_size):
         self.message = message
         self.model = model
         self.model_name = model_name
         self.progress_bar = progress_bar
+        self.image_size = image_size
+        self.batch_size = batch_size
 
     def progress_bar_update(self):
         if self.progress_bar is not None:
             self.progress_bar.update(1)
 
     def is_model_supported(self):
         """
@@ -439,19 +442,21 @@
         eligible, message = self.is_model_eligible()
         if not eligible:
             return eligible, message, None, self.progress_bar  # pragma: no cover
         return True, self.message, self.model_name, self.progress_bar
 
 
 class TorchChecks:
-    def __init__(self, model, model_name, message, progress_bar):
+    def __init__(self, model, model_name, message, progress_bar, image_size, batch_size):
         self.message = message
         self.model = model
         self.model_name = model_name
         self.progress_bar = progress_bar
+        self.image_size = image_size
+        self.batch_size = batch_size
 
     def is_model_supported(self):
         """
         Check if model contains:
             - forward function
         """
         model = self.model
@@ -460,26 +465,25 @@
             raise Exception("forward func missing")
         self.progress_bar.update(1)
 
     def small_training_loop(self, custom_loss=None):
         try:
             # Define the number of fake images and other properties
             num_images = 100
-            image_size = 32
             num_channels = 3
-            num_classes = 10
+            num_classes = 1
             # Create fake image data
             train_dataset = datasets.FakeData(
                 size=num_images,
-                image_size=(num_channels, image_size, image_size),
+                image_size=(num_channels, self.image_size, self.image_size),
                 num_classes=num_classes,
                 transform=transforms.ToTensor(),
             )
 
-            train_loader = DataLoader(train_dataset, batch_size=16, shuffle=True)
+            train_loader = DataLoader(train_dataset, batch_size=self.batch_size, shuffle=True)
 
             # train_loader, classes = mock_torch_data(self.tmp_path)
             criterion = nn.CrossEntropyLoss()
             optimizer = optim.SGD(self.model.parameters(), lr=0.001, momentum=0.9)
             for epoch in range(1):  # loop over the dataset multiple times
 
                 running_loss = 0.0
@@ -497,15 +501,15 @@
                     optimizer.step()
 
                     # print statistics
                     running_loss += loss.item()
             self.progress_bar.update(1)
         except Exception as e:  # pragma: no cover
             self.message = (
-                "\nModel not support training on image classification dataset."
+                f"\nModel not support training on image classification dataset as there is error {e} "
             )
             raise
 
     def model_func_checks(self):
         # check if model is eligible
         try:
             self.is_model_supported()
```

### Comparing `tracebloc_package-dev-0.4.5/tracebloc_package/linkModelDataSet.py` & `tracebloc_package-dev-0.4.6/tracebloc_package/linkModelDataSet.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,20 +24,22 @@
         datasetId,
         token,
         weights,
         totalDatasetSize,
         total_images,
         num_classes,
         class_names,
+        image_size,
+        batchsize,
         url="",
         environment="production",
         framework=TENSORFLOW_FRAMEWORK,
     ):
+        self.__framework = framework
         self.__url = url
-        # self.__url = 'http://127.0.0.1:8000/'
         self.__token = token
         self.__earlystopCallback = {}
         self.__reducelrCallback = {}
         self.__modelCheckpointCallback = {}
         self.__terminateOnNaNCallback = {}
         self.__learningRateSet = False
         self.__optimizerSet = False
@@ -45,28 +47,28 @@
         self.__message = "training"
         self.__datasetId = datasetId
         self.__epochs = 10
         self.__cycles = 1
         self.__modelId = modelId
         self.__modelName = modelname
         self.__model = model
-        self.__image_shape = 224
+        self.__image_shape = image_size
         self.__image_type = "rgb"
         self.__optimizer = "sgd"
         self.__totalDatasetSize = totalDatasetSize
         self.__trainingDatasetSize = totalDatasetSize
         self.__trainingClasses = class_names
         self.__subdataset = {}
         self.__lossFunction = {TYPE: STANDARD, VALUE: "mse"}
         self.__learningRate = {TYPE: CONSTANT, VALUE: 0.001}
         self.__seed = False
         self.__total_images = total_images
         self.__num_classes = num_classes
         self.__class_names = class_names
-        self.__batchSize = self.__default_batchSize()
+        self.__batchSize = self.__default_batchSize(batchsize)
         self.__featurewise_center = False
         self.__samplewise_center = False
         self.__featurewise_std_normalization = False
         self.__samplewise_std_normalization = False
         self.__zca_whitening = False
         self.__rotation_range = 0
         self.__width_shift_range = 0.0
@@ -91,16 +93,15 @@
         self.__upperboundTime = 0
         self.__weights = weights
         self.__images_per_class = json.dumps(self.__class_names)
         self.__eligibility_passed = True
         self.__error_method = []
         self.__reform_model = False
         self._environment = environment
-        self.__framework = framework
-        self.__experiment_url = "https://ai.tracebloc.io/experiments/"
+        self.__experimenturl = "https://ai.tracebloc.io/experiments/"
         if environment == "development" or environment == "ds":
             self.__experimenturl = "https://dev.tracebloc.io/experiments/"
         elif environment == "staging":
             self.__experimenturl = "https://stg.tracebloc.io/experiments/"
 
     def resetTrainingPlan(self):
         self.__earlystopCallback = {}
@@ -215,19 +216,15 @@
             header = {"Authorization": f"Token {self.__token}"}
             data = {
                 "edges_involved": json.dumps(list(self.__total_images.keys())),
                 "images_per_class": json.dumps(training_dataset),
                 "type": "recalculate_image_count_per_edge",
                 "datasetId": self.__datasetId,
             }
-            re = requests.post(
-                f"{self.__url}check-model/",
-                headers=header,
-                data=data,
-            )
+            re = requests.post(f"{self.__url}check-model/", headers=header, data=data,)
             body_unicode = re.content.decode("utf-8")
             content = json.loads(body_unicode)
             if re.status_code == 200:
                 self.__total_images = content["total_images_per_edge"]
                 self.__validation_split = self.__default_validation_split()
                 self.__images_per_class = json.dumps(
                     training_dataset
@@ -361,41 +358,44 @@
             self.__cycles = cycles
             self.__remove_error_method()
         else:
             self.__eligibility_passed = False
             error_msg = "Invalid input type or value '0' given for cycles\n"
             self.__print_error(error_msg)
 
-    def __default_batchSize(self):
+    def __default_batchSize(self, batchsize=None):
         """
         set default batch size when training object is created
         """
         # get edge with the lowest images
-        edge_min = min(self.__total_images, key=self.__total_images.get)
-        # get images count for selected edge
-        images = int(self.__total_images[edge_min])
-        batch = images // 3
-        if 8 < batch < 16:
-            return 8
-        elif 16 < batch < 32:
-            return 16
-        elif 32 < batch < 64:
-            return 32
-        elif batch > 64:
-            return 64
+        if self.__framework == TENSORFLOW_FRAMEWORK or batchsize is None:
+            edge_min = min(self.__total_images, key=self.__total_images.get)
+            # get images count for selected edge
+            images = int(self.__total_images[edge_min])
+            batch = images // 3
+            if 8 < batch < 16:
+                return 8
+            elif 16 < batch < 32:
+                return 16
+            elif 32 < batch < 64:
+                return 32
+            elif batch > 64:
+                return 64
+            else:
+                return batch
         else:
-            return batch
+            return batchsize
 
     def batchSize(self, batchSize: int):
         """
         Integer or None. Number of samples per gradient update. If unspecified, batch_size will default to 32.
         example: trainingObject.batchSize(16)
         default: 32
         """
-        # get edge with lowest images
+        # get edge with the lowest images
         edge_min = min(self.__total_images, key=self.__total_images.get)
         # get images count for selected edge
         images = int(self.__total_images[edge_min])
         # check for no of batches
         if type(batchSize) == int:
             if images // batchSize < 3 and self.__framework == TENSORFLOW_FRAMEWORK:
                 error_msg = "Please choose smaller batch size as dataset selected have less images\n"
```

### Comparing `tracebloc_package-dev-0.4.5/tracebloc_package/messages.py` & `tracebloc_package-dev-0.4.6/tracebloc_package/messages.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.4.5/tracebloc_package/upload.py` & `tracebloc_package-dev-0.4.6/tracebloc_package/upload.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,14 +26,16 @@
     """
 
     def __init__(self, modelname, token, weights=False, url=""):
         self.__modelname = ""
         self.__model_path = ""
         self.__weights_path = ""
         self.__framework = TENSORFLOW_FRAMEWORK
+        self.__image_size = 224
+        self.__batch_size = 16
         self.__ext = ".py"
         self.model = None
         self.__get_paths(modelname)
         self.__token = token
         self.weights = weights
         self.__url = url + "upload/"
         self.__check_model_url = url + "check-model/"
@@ -79,14 +81,16 @@
         if self.__recievedModelname is not None:
             return (
                 self.__recievedModelname,
                 self.__modelname,
                 self.__ext,
                 self.__model_path,
                 self.__framework,
+                self.__image_size,
+                self.__batch_size,
             )
 
     def upload(self):
         # load model from current directory
         status = False
         message = None
         # create progress bar with total number of nested functions
@@ -111,24 +115,28 @@
                     "red",
                 )
                 print(text, "\n")
                 self.progress_bar.close()
                 return None
             loaded_model = model_checks_generic.model
             self.__framework = model_checks_generic.framework
+            self.__image_size = int(model_checks_generic.image_size)
+            self.__batch_size = int(model_checks_generic.batch_size)
             model_check_class = TensorflowChecks
             if self.__framework == PYTORCH_FRAMEWORK:
                 model_check_class = TorchChecks
             elif self.__framework == TENSORFLOW_FRAMEWORK:
                 model_check_class = TensorflowChecks
             model_checks = model_check_class(
                 model=loaded_model,
                 model_name=model_name,
                 message=message,
                 progress_bar=self.progress_bar,
+                image_size=self.__image_size,
+                batch_size=self.__batch_size,
             )
             (
                 status,
                 message,
                 model_name,
                 progress_bar,
             ) = model_checks.model_func_checks()
```

### Comparing `tracebloc_package-dev-0.4.5/tracebloc_package/user.py` & `tracebloc_package-dev-0.4.6/tracebloc_package/user.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,14 +30,16 @@
             )
             print(text, "\n")
             return
         self.__username = input("Enter your email address : ")
         self.__password = getpass.getpass("Enter your password : ")
         self.__token = self.login()
         self.__ext = ".py"
+        self.__image_size = 224
+        self.__batch_size = 16
         if self.__token is None or self.__token == "":
             # text = colored(
             #     "You are not logged in. Please go back to ‘1. Connect to Tracebloc’ and proceed with logging in.",
             #     "red",
             # )
             # print(text, "\n")
             return
@@ -119,14 +121,16 @@
             modelobj = Model(self.__modelName, self.__token, self.__weights, self.__url)
             (
                 self.__modelId,
                 self.__modelName,
                 self.__ext,
                 path,
                 self.__framework,
+                self.__image_size,
+                self.__batch_size
             ) = modelobj.getNewModelId()
             self.__model = modelobj.model
             if self.__modelId == "" or self.__modelId is None:
                 text = colored(f"'{self.__modelName}' upload Failed.", "red")
                 print(text, "\n")
                 self.__weights = False
                 return
@@ -168,21 +172,23 @@
                     datasetId,
                     self.__token,
                     self.__weights,
                     self.__totalDatasetSize,
                     self.__total_images,
                     self.__num_classes,
                     self.__class_names,
+                    self.__image_size,
+                    self.__batch_size,
                     self.__url,
                     self.__environment,
                     self.__framework,
                 )
             else:
                 return None
-        except:
+        except Exception as e:
             text = colored("Model Link Failed!", "red")
             print(text, "\n")
 
     def __checkmodel(self, datasetId):
         try:
             header = {"Authorization": f"Token {self.__token}"}
             re = requests.post(
```

### Comparing `tracebloc_package-dev-0.4.5/tracebloc_package/utils.py` & `tracebloc_package-dev-0.4.6/tracebloc_package/utils.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.4.5/tracebloc_package/weights.py` & `tracebloc_package-dev-0.4.6/tracebloc_package/weights.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.4.5/tracebloc_package_dev.egg-info/PKG-INFO` & `tracebloc_package-dev-0.4.6/tracebloc_package_dev.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 Metadata-Version: 2.1
 Name: tracebloc-package-dev
-Version: 0.4.5
+Version: 0.4.6
 Summary: Package required to run Tracebloc jupyter notebook to create experiment
 Home-page: https://gitlab.com/tracebloc/tracebloc-py-package/-/tree/dev
 Author: Tracebloc
 Author-email: info@tracebloc.io
 License: MIT
-Platform: UNKNOWN
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Tracebloc package
 This packeg is pre-requiste to run tracebloc jupyter notebook.
 
 
 This package helps to create and start the experiment for training ML models in 
 tracebloc environment.
-
```

### Comparing `tracebloc_package-dev-0.4.5/tracebloc_package_dev.egg-info/SOURCES.txt` & `tracebloc_package-dev-0.4.6/tracebloc_package_dev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

