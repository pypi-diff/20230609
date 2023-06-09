# Comparing `tmp/monotonic-nn-0.3.1rc2.tar.gz` & `tmp/monotonic-nn-0.3.2rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monotonic-nn-0.3.1rc2.tar", last modified: Wed Jun  7 07:22:22 2023, max compression
+gzip compressed data, was "monotonic-nn-0.3.2rc0.tar", last modified: Fri Jun  9 05:16:50 2023, max compression
```

## Comparing `monotonic-nn-0.3.1rc2.tar` & `monotonic-nn-0.3.2rc0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-06-07 07:22:22.625995 monotonic-nn-0.3.1rc2/
--rw-rw-r--   0 davor     (1000) davor     (1000)    20848 2023-06-05 13:19:26.000000 monotonic-nn-0.3.1rc2/LICENSE
--rw-rw-r--   0 davor     (1000) davor     (1000)      111 2023-06-05 13:19:26.000000 monotonic-nn-0.3.1rc2/MANIFEST.in
--rw-rw-r--   0 davor     (1000) davor     (1000)    12019 2023-06-07 07:22:22.625995 monotonic-nn-0.3.1rc2/PKG-INFO
--rw-rw-r--   0 davor     (1000) davor     (1000)    10875 2023-06-07 07:21:40.000000 monotonic-nn-0.3.1rc2/README.md
-drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-06-07 07:22:22.621995 monotonic-nn-0.3.1rc2/airt/
--rw-rw-r--   0 davor     (1000) davor     (1000)      367 2023-06-07 07:21:55.000000 monotonic-nn-0.3.1rc2/airt/__init__.py
-drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-06-07 07:22:22.621995 monotonic-nn-0.3.1rc2/airt/_components/
--rw-rw-r--   0 davor     (1000) davor     (1000)        0 2023-06-07 07:21:55.000000 monotonic-nn-0.3.1rc2/airt/_components/__init__.py
--rw-rw-r--   0 davor     (1000) davor     (1000)      320 2023-06-07 07:21:55.000000 monotonic-nn-0.3.1rc2/airt/_components/helpers.py
--rw-rw-r--   0 davor     (1000) davor     (1000)    31436 2023-06-07 07:21:55.000000 monotonic-nn-0.3.1rc2/airt/_components/mono_dense_layer.py
--rw-rw-r--   0 davor     (1000) davor     (1000)     9935 2023-06-07 07:21:55.000000 monotonic-nn-0.3.1rc2/airt/_modidx.py
-drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-06-07 07:22:22.621995 monotonic-nn-0.3.1rc2/airt/keras/
--rw-rw-r--   0 davor     (1000) davor     (1000)        0 2023-06-07 07:21:55.000000 monotonic-nn-0.3.1rc2/airt/keras/__init__.py
--rw-rw-r--   0 davor     (1000) davor     (1000)    14089 2023-06-07 07:21:55.000000 monotonic-nn-0.3.1rc2/airt/keras/experiments.py
-drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-06-07 07:22:22.621995 monotonic-nn-0.3.1rc2/airt/keras/layers/
--rw-rw-r--   0 davor     (1000) davor     (1000)      344 2023-06-07 07:21:55.000000 monotonic-nn-0.3.1rc2/airt/keras/layers/__init__.py
-drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-06-07 07:22:22.625995 monotonic-nn-0.3.1rc2/monotonic_nn.egg-info/
--rw-rw-r--   0 davor     (1000) davor     (1000)    12019 2023-06-07 07:22:22.000000 monotonic-nn-0.3.1rc2/monotonic_nn.egg-info/PKG-INFO
--rw-rw-r--   0 davor     (1000) davor     (1000)      510 2023-06-07 07:22:22.000000 monotonic-nn-0.3.1rc2/monotonic_nn.egg-info/SOURCES.txt
--rw-rw-r--   0 davor     (1000) davor     (1000)        1 2023-06-07 07:22:22.000000 monotonic-nn-0.3.1rc2/monotonic_nn.egg-info/dependency_links.txt
--rw-rw-r--   0 davor     (1000) davor     (1000)       30 2023-06-07 07:22:22.000000 monotonic-nn-0.3.1rc2/monotonic_nn.egg-info/entry_points.txt
--rw-rw-r--   0 davor     (1000) davor     (1000)        1 2023-06-05 18:05:47.000000 monotonic-nn-0.3.1rc2/monotonic_nn.egg-info/not-zip-safe
--rw-rw-r--   0 davor     (1000) davor     (1000)      268 2023-06-07 07:22:22.000000 monotonic-nn-0.3.1rc2/monotonic_nn.egg-info/requires.txt
--rw-rw-r--   0 davor     (1000) davor     (1000)        5 2023-06-07 07:22:22.000000 monotonic-nn-0.3.1rc2/monotonic_nn.egg-info/top_level.txt
--rw-rw-r--   0 davor     (1000) davor     (1000)      919 2023-06-07 07:21:45.000000 monotonic-nn-0.3.1rc2/settings.ini
--rw-rw-r--   0 davor     (1000) davor     (1000)       38 2023-06-07 07:22:22.625995 monotonic-nn-0.3.1rc2/setup.cfg
--rw-rw-r--   0 davor     (1000) davor     (1000)     3157 2023-06-05 13:19:26.000000 monotonic-nn-0.3.1rc2/setup.py
+drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-06-09 05:16:50.713738 monotonic-nn-0.3.2rc0/
+-rw-rw-r--   0 davor     (1000) davor     (1000)    20848 2023-06-05 13:19:26.000000 monotonic-nn-0.3.2rc0/LICENSE
+-rw-rw-r--   0 davor     (1000) davor     (1000)      111 2023-06-05 13:19:26.000000 monotonic-nn-0.3.2rc0/MANIFEST.in
+-rw-rw-r--   0 davor     (1000) davor     (1000)    12019 2023-06-09 05:16:50.713738 monotonic-nn-0.3.2rc0/PKG-INFO
+-rw-rw-r--   0 davor     (1000) davor     (1000)    10875 2023-06-07 07:21:40.000000 monotonic-nn-0.3.2rc0/README.md
+drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-06-09 05:16:50.713738 monotonic-nn-0.3.2rc0/airt/
+-rw-rw-r--   0 davor     (1000) davor     (1000)      405 2023-06-09 05:15:47.000000 monotonic-nn-0.3.2rc0/airt/__init__.py
+drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-06-09 05:16:50.713738 monotonic-nn-0.3.2rc0/airt/_components/
+-rw-rw-r--   0 davor     (1000) davor     (1000)        0 2023-06-09 05:15:47.000000 monotonic-nn-0.3.2rc0/airt/_components/__init__.py
+-rw-rw-r--   0 davor     (1000) davor     (1000)      320 2023-06-09 05:15:47.000000 monotonic-nn-0.3.2rc0/airt/_components/helpers.py
+-rw-rw-r--   0 davor     (1000) davor     (1000)    31904 2023-06-09 05:15:47.000000 monotonic-nn-0.3.2rc0/airt/_components/mono_dense_layer.py
+-rw-rw-r--   0 davor     (1000) davor     (1000)    10242 2023-06-09 05:15:47.000000 monotonic-nn-0.3.2rc0/airt/_modidx.py
+drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-06-09 05:16:50.713738 monotonic-nn-0.3.2rc0/airt/keras/
+-rw-rw-r--   0 davor     (1000) davor     (1000)        0 2023-06-09 05:15:47.000000 monotonic-nn-0.3.2rc0/airt/keras/__init__.py
+-rw-rw-r--   0 davor     (1000) davor     (1000)    14180 2023-06-09 05:15:47.000000 monotonic-nn-0.3.2rc0/airt/keras/experiments.py
+drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-06-09 05:16:50.713738 monotonic-nn-0.3.2rc0/airt/keras/layers/
+-rw-rw-r--   0 davor     (1000) davor     (1000)      344 2023-06-09 05:15:47.000000 monotonic-nn-0.3.2rc0/airt/keras/layers/__init__.py
+drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-06-09 05:16:50.713738 monotonic-nn-0.3.2rc0/monotonic_nn.egg-info/
+-rw-rw-r--   0 davor     (1000) davor     (1000)    12019 2023-06-09 05:16:50.000000 monotonic-nn-0.3.2rc0/monotonic_nn.egg-info/PKG-INFO
+-rw-rw-r--   0 davor     (1000) davor     (1000)      510 2023-06-09 05:16:50.000000 monotonic-nn-0.3.2rc0/monotonic_nn.egg-info/SOURCES.txt
+-rw-rw-r--   0 davor     (1000) davor     (1000)        1 2023-06-09 05:16:50.000000 monotonic-nn-0.3.2rc0/monotonic_nn.egg-info/dependency_links.txt
+-rw-rw-r--   0 davor     (1000) davor     (1000)       30 2023-06-09 05:16:50.000000 monotonic-nn-0.3.2rc0/monotonic_nn.egg-info/entry_points.txt
+-rw-rw-r--   0 davor     (1000) davor     (1000)        1 2023-06-05 18:05:47.000000 monotonic-nn-0.3.2rc0/monotonic_nn.egg-info/not-zip-safe
+-rw-rw-r--   0 davor     (1000) davor     (1000)      268 2023-06-09 05:16:50.000000 monotonic-nn-0.3.2rc0/monotonic_nn.egg-info/requires.txt
+-rw-rw-r--   0 davor     (1000) davor     (1000)        5 2023-06-09 05:16:50.000000 monotonic-nn-0.3.2rc0/monotonic_nn.egg-info/top_level.txt
+-rw-rw-r--   0 davor     (1000) davor     (1000)      918 2023-06-09 05:07:03.000000 monotonic-nn-0.3.2rc0/settings.ini
+-rw-rw-r--   0 davor     (1000) davor     (1000)       38 2023-06-09 05:16:50.713738 monotonic-nn-0.3.2rc0/setup.cfg
+-rw-rw-r--   0 davor     (1000) davor     (1000)     3157 2023-06-09 04:49:50.000000 monotonic-nn-0.3.2rc0/setup.py
```

### Comparing `monotonic-nn-0.3.1rc2/LICENSE` & `monotonic-nn-0.3.2rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `monotonic-nn-0.3.1rc2/PKG-INFO` & `monotonic-nn-0.3.2rc0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monotonic-nn
-Version: 0.3.1rc2
+Version: 0.3.2rc0
 Summary: Monotonic Neural Networks
 Home-page: https://github.com/airtai/monotonic-nn
 Author: AIRT Technologies d.o.o.
 Author-email: info@airt.ai
 License: Creative Commons License
 Project-URL: Bug Tracker, https://github.com/airtai/monotonic-nn/issues
 Project-URL: CI, https://github.com/airtai/monotonic-nn/actions
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: monotonic-nn Version: 0.3.1rc2 Summary: Monotonic
+Metadata-Version: 2.1 Name: monotonic-nn Version: 0.3.2rc0 Summary: Monotonic
 Neural Networks Home-page: https://github.com/airtai/monotonic-nn Author: AIRT
 Technologies d.o.o. Author-email: info@airt.ai License: Creative Commons
 License Project-URL: Bug Tracker, https://github.com/airtai/monotonic-nn/issues
 Project-URL: CI, https://github.com/airtai/monotonic-nn/actions Project-URL:
 Documentation, https://monotonic.airt.ai/ Project-URL: Tutorial, https://
 colab.research.google.com/github/airtai/monotonic-nn/blob/main/nbs/index.ipynb
 Keywords: tensorflow keras monotone "monotonic neural networks" "dense layer"
```

### Comparing `monotonic-nn-0.3.1rc2/README.md` & `monotonic-nn-0.3.2rc0/README.md`

 * *Files identical despite different names*

### Comparing `monotonic-nn-0.3.1rc2/airt/_components/mono_dense_layer.py` & `monotonic-nn-0.3.2rc0/airt/_components/mono_dense_layer.py`

 * *Files 0% similar despite different names*

```diff
@@ -175,14 +175,15 @@
     try:
         yield
     finally:
         layer.kernel = old_kernel
 
 # %% ../../nbs/MonoDenseLayer.ipynb 29
 @export
+@tf.keras.saving.register_keras_serializable("airt.keras.layers")
 class MonoDense(Dense):
     """Monotonic counterpart of the regular Dense Layer of tf.keras
 
     This is an implementation of our Monotonic Dense Unit or Constrained Monotone Fully Connected Layer. The below is the figure from the paper for reference.
 
     - the parameter `monotonicity_indicator` corresponds to **t** in the figure below, and
 
@@ -247,25 +248,36 @@
                 f"Values of activation_weights must be non-negative, but we have this instead: {activation_weights}."
             )
 
         super(MonoDense, self).__init__(units=units, activation=None, **kwargs)
 
         self.units = units
         self.org_activation = activation
-        self.activation_weights = activation_weights
         self.monotonicity_indicator = monotonicity_indicator
         self.is_convex = is_convex
         self.is_concave = is_concave
+        self.activation_weights = activation_weights
 
         (
             self.convex_activation,
             self.concave_activation,
             self.saturated_activation,
         ) = get_activation_functions(self.org_activation)
 
+    def get_config(self) -> Dict[str, Any]:
+        """Get config is used for saving the model"""
+        return dict(
+            units=self.units,
+            activation=self.org_activation,
+            monotonicity_indicator=self.monotonicity_indicator,
+            is_convex=self.is_convex,
+            is_concave=self.is_concave,
+            activation_weights=self.activation_weights,
+        )
+
     def build(self, input_shape: Tuple, *args: List[Any], **kwargs: Any) -> None:
         """Build
 
         Args:
             input_shape: input tensor
             args: positional arguments passed to Dense.build()
             kwargs: keyword arguments passed to Dense.build()
@@ -435,15 +447,15 @@
             final_activation=final_activation,
             monotonicity_indicator=monotonicity_indicator,
             is_convex=is_convex,
             is_concave=is_concave,
             dropout=dropout,
         )
 
-# %% ../../nbs/MonoDenseLayer.ipynb 33
+# %% ../../nbs/MonoDenseLayer.ipynb 34
 def _create_mono_block(
     *,
     units: List[int],
     activation: Union[str, Callable[[TensorLike], TensorLike]],
     monotonicity_indicator: TensorLike = 1,
     is_convex: bool = False,
     is_concave: bool = False,
@@ -477,15 +489,15 @@
             if (i < len(units) - 1) and dropout:
                 y = Dropout(dropout)(y)
 
         return y
 
     return create_mono_block_inner
 
-# %% ../../nbs/MonoDenseLayer.ipynb 35
+# %% ../../nbs/MonoDenseLayer.ipynb 36
 T = TypeVar("T")
 
 
 def _prepare_mono_input_n_param(
     inputs: Union[TensorLike, Dict[str, TensorLike], List[TensorLike]],
     param: Union[T, Dict[str, T], List[T]],
 ) -> Tuple[List[TensorLike], List[T], List[str]]:
@@ -519,15 +531,15 @@
             raise ValueError(f"Uncompatible types: {type(inputs)=}, {type(param)=}")
         inputs = [inputs]
         param = [param]  # type: ignore
         sorted_feature_names = ["inputs"]
 
     return inputs, param, sorted_feature_names
 
-# %% ../../nbs/MonoDenseLayer.ipynb 43
+# %% ../../nbs/MonoDenseLayer.ipynb 44
 def _check_convexity_params(
     monotonicity_indicator: List[int],
     is_convex: List[bool],
     is_concave: List[bool],
     names: List[str],
 ) -> Tuple[bool, bool]:
     ix = [
@@ -542,15 +554,15 @@
     has_convex = any(is_convex)
     has_concave = any(is_concave)
     if has_convex and has_concave:
         print("WARNING: we have both convex and concave parameters")
 
     return has_convex, has_concave
 
-# %% ../../nbs/MonoDenseLayer.ipynb 46
+# %% ../../nbs/MonoDenseLayer.ipynb 47
 @export
 def _create_type_1(
     inputs: Union[TensorLike, Dict[str, TensorLike], List[TensorLike]],
     *,
     units: int,
     final_units: int,
     activation: Union[str, Callable[[TensorLike], TensorLike]],
@@ -616,15 +628,15 @@
     )(y)
 
     if final_activation is not None:
         y = tf.keras.activations.get(final_activation)(y)
 
     return y
 
-# %% ../../nbs/MonoDenseLayer.ipynb 51
+# %% ../../nbs/MonoDenseLayer.ipynb 52
 @export
 def _create_type_2(
     inputs: Union[TensorLike, Dict[str, TensorLike], List[TensorLike]],
     *,
     input_units: Optional[int] = None,
     units: int,
     final_units: int,
```

### Comparing `monotonic-nn-0.3.1rc2/airt/_modidx.py` & `monotonic-nn-0.3.2rc0/airt/_modidx.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,16 @@
                                                                                                           'airt/_components/mono_dense_layer.py'),
                                                    'airt._components.mono_dense_layer.MonoDense.call': ( 'monodenselayer.html#monodense.call',
                                                                                                          'airt/_components/mono_dense_layer.py'),
                                                    'airt._components.mono_dense_layer.MonoDense.create_type_1': ( 'monodenselayer.html#monodense.create_type_1',
                                                                                                                   'airt/_components/mono_dense_layer.py'),
                                                    'airt._components.mono_dense_layer.MonoDense.create_type_2': ( 'monodenselayer.html#monodense.create_type_2',
                                                                                                                   'airt/_components/mono_dense_layer.py'),
+                                                   'airt._components.mono_dense_layer.MonoDense.get_config': ( 'monodenselayer.html#monodense.get_config',
+                                                                                                               'airt/_components/mono_dense_layer.py'),
                                                    'airt._components.mono_dense_layer._check_convexity_params': ( 'monodenselayer.html#_check_convexity_params',
                                                                                                                   'airt/_components/mono_dense_layer.py'),
                                                    'airt._components.mono_dense_layer._create_mono_block': ( 'monodenselayer.html#_create_mono_block',
                                                                                                              'airt/_components/mono_dense_layer.py'),
                                                    'airt._components.mono_dense_layer._create_type_1': ( 'monodenselayer.html#_create_type_1',
                                                                                                          'airt/_components/mono_dense_layer.py'),
                                                    'airt._components.mono_dense_layer._create_type_2': ( 'monodenselayer.html#_create_type_2',
```

### Comparing `monotonic-nn-0.3.1rc2/airt/keras/experiments.py` & `monotonic-nn-0.3.2rc0/airt/keras/experiments.py`

 * *Files 2% similar despite different names*

```diff
@@ -254,14 +254,15 @@
     executions_per_trial: int = 3,
     max_consecutive_failed_trials: int = 5,
     patience: int = 10,
 ) -> Tuner:
     """Search for optimal hyperparameters
 
     Args:
+        dataset_name: name of the dataset, one of "auto", "heart", compas", "blog", "loan"
         monotonicity_indicator: monotonicity indicator as used in `MonoDense.__init__`
         final_activation:  final activation of the neural network
         loss: Tensorflow loss function
         metrics: Tensorflow metrics function
         hp_params_f: a function constructing sampling hyperparameters using Keras Tuner
         max_trials: maximum number of trials
         max_epochs: maximum number of epochs in each trial
```

### Comparing `monotonic-nn-0.3.1rc2/monotonic_nn.egg-info/PKG-INFO` & `monotonic-nn-0.3.2rc0/monotonic_nn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monotonic-nn
-Version: 0.3.1rc2
+Version: 0.3.2rc0
 Summary: Monotonic Neural Networks
 Home-page: https://github.com/airtai/monotonic-nn
 Author: AIRT Technologies d.o.o.
 Author-email: info@airt.ai
 License: Creative Commons License
 Project-URL: Bug Tracker, https://github.com/airtai/monotonic-nn/issues
 Project-URL: CI, https://github.com/airtai/monotonic-nn/actions
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: monotonic-nn Version: 0.3.1rc2 Summary: Monotonic
+Metadata-Version: 2.1 Name: monotonic-nn Version: 0.3.2rc0 Summary: Monotonic
 Neural Networks Home-page: https://github.com/airtai/monotonic-nn Author: AIRT
 Technologies d.o.o. Author-email: info@airt.ai License: Creative Commons
 License Project-URL: Bug Tracker, https://github.com/airtai/monotonic-nn/issues
 Project-URL: CI, https://github.com/airtai/monotonic-nn/actions Project-URL:
 Documentation, https://monotonic.airt.ai/ Project-URL: Tutorial, https://
 colab.research.google.com/github/airtai/monotonic-nn/blob/main/nbs/index.ipynb
 Keywords: tensorflow keras monotone "monotonic neural networks" "dense layer"
```

### Comparing `monotonic-nn-0.3.1rc2/settings.ini` & `monotonic-nn-0.3.2rc0/settings.ini`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = monotonic-nn
 lib_name = %(repo)s
-version = 0.3.1rc2
+version = 0.3.2rc
 min_python = 3.8
 license = cc
 
 ### nbdev ###
 doc_path = _docs
 lib_path = airt
 nbs_path = nbs
 recursive = True
 tst_flags = notest skip
 put_version_in_init = True
 black_formatting = True
-docs_versioning = patch
+docs_versioning = minor
 
 ### Docs ###
 branch = main
 custom_sidebar = True
 doc_host = https://%(user)s.github.io
 doc_baseurl = /%(repo)s
 git_url = https://github.com/%(user)s/%(repo)s
```

### Comparing `monotonic-nn-0.3.1rc2/setup.py` & `monotonic-nn-0.3.2rc0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 statuses = [ '1 - Planning', '2 - Pre-Alpha', '3 - Alpha',
     '4 - Beta', '5 - Production/Stable', '6 - Mature', '7 - Inactive' ]
 py_versions = '3.6 3.7 3.8 3.9 3.10 3.11'.split()
 
 min_python = cfg['min_python']
 lic = licenses.get(cfg['license'].lower(), (cfg['license'], None))
 
-requirements = ["tensorflow>=2.10.0"]
+requirements = ["tensorflow>=2.12.0"]
 
 experiments_requirements = [
     "keras-tuner[bayesian]==1.3.5"
 ]
 
 dev_requirements = [
     "nbdev_mkdocs==0.5.1",
```

