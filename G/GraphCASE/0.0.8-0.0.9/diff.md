# Comparing `tmp/GraphCASE-0.0.8.tar.gz` & `tmp/GraphCASE-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GraphCASE-0.0.8.tar", last modified: Tue Jun  6 18:11:47 2023, max compression
+gzip compressed data, was "GraphCASE-0.0.9.tar", last modified: Fri Jun  9 07:13:36 2023, max compression
```

## Comparing `GraphCASE-0.0.8.tar` & `GraphCASE-0.0.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 tonpoppe   (501) staff       (20)        0 2023-06-06 18:11:47.617424 GraphCASE-0.0.8/
-drwxr-xr-x   0 tonpoppe   (501) staff       (20)        0 2023-06-06 18:11:47.614632 GraphCASE-0.0.8/GAE/
--rw-r--r--   0 tonpoppe   (501) staff       (20)        0 2020-07-29 20:02:56.000000 GraphCASE-0.0.8/GAE/__init__.py
--rw-rw-rw-   0 tonpoppe   (501) staff       (20)     6564 2020-07-21 05:00:15.000000 GraphCASE-0.0.8/GAE/dataFeeder.py
--rwxr-xr-x   0 tonpoppe   (501) staff       (20)    11515 2023-06-02 10:58:22.000000 GraphCASE-0.0.8/GAE/data_feeder_graphframes.py
--rwxr-xr-x   0 tonpoppe   (501) staff       (20)    13402 2023-05-26 07:12:59.000000 GraphCASE-0.0.8/GAE/data_feeder_nx.py
--rw-r--r--   0 tonpoppe   (501) staff       (20)    16805 2023-06-06 18:04:13.000000 GraphCASE-0.0.8/GAE/graph_case_controller.py
--rw-r--r--   0 tonpoppe   (501) staff       (20)     3867 2023-06-02 13:25:09.000000 GraphCASE-0.0.8/GAE/graph_case_tools.py
--rw-r--r--   0 tonpoppe   (501) staff       (20)     8247 2023-06-05 08:32:48.000000 GraphCASE-0.0.8/GAE/graph_reconstructor.py
--rw-r--r--   0 tonpoppe   (501) staff       (20)    13464 2023-06-05 17:58:06.000000 GraphCASE-0.0.8/GAE/input_layer_constructor.py
--rw-r--r--   0 tonpoppe   (501) staff       (20)     8746 2023-05-26 07:12:59.000000 GraphCASE-0.0.8/GAE/model.py
--rw-r--r--   0 tonpoppe   (501) staff       (20)    13478 2023-06-05 18:29:55.000000 GraphCASE-0.0.8/GAE/position_manager.py
--rw-r--r--   0 tonpoppe   (501) staff       (20)     6979 2023-05-26 07:12:59.000000 GraphCASE-0.0.8/GAE/transformation_layer.py
-drwxr-xr-x   0 tonpoppe   (501) staff       (20)        0 2023-06-06 18:11:47.616646 GraphCASE-0.0.8/GraphCASE.egg-info/
--rw-r--r--   0 tonpoppe   (501) staff       (20)      296 2023-06-06 18:11:46.000000 GraphCASE-0.0.8/GraphCASE.egg-info/PKG-INFO
--rw-r--r--   0 tonpoppe   (501) staff       (20)      425 2023-06-06 18:11:47.000000 GraphCASE-0.0.8/GraphCASE.egg-info/SOURCES.txt
--rw-r--r--   0 tonpoppe   (501) staff       (20)        1 2023-06-06 18:11:47.000000 GraphCASE-0.0.8/GraphCASE.egg-info/dependency_links.txt
--rw-r--r--   0 tonpoppe   (501) staff       (20)        4 2023-06-06 18:11:47.000000 GraphCASE-0.0.8/GraphCASE.egg-info/top_level.txt
--rw-r--r--   0 tonpoppe   (501) staff       (20)    35149 2020-07-19 21:06:49.000000 GraphCASE-0.0.8/LICENSE.txt
--rw-r--r--   0 tonpoppe   (501) staff       (20)      296 2023-06-06 18:11:47.617104 GraphCASE-0.0.8/PKG-INFO
--rw-r--r--   0 tonpoppe   (501) staff       (20)     7404 2022-09-19 17:31:14.000000 GraphCASE-0.0.8/README.md
--rw-r--r--   0 tonpoppe   (501) staff       (20)       38 2023-06-06 18:11:47.617532 GraphCASE-0.0.8/setup.cfg
--rw-r--r--   0 tonpoppe   (501) staff       (20)      322 2023-06-06 18:11:05.000000 GraphCASE-0.0.8/setup.py
+drwxr-xr-x   0 tonpoppe   (501) staff       (20)        0 2023-06-09 07:13:36.330572 GraphCASE-0.0.9/
+drwxr-xr-x   0 tonpoppe   (501) staff       (20)        0 2023-06-09 07:13:36.328148 GraphCASE-0.0.9/GAE/
+-rw-r--r--   0 tonpoppe   (501) staff       (20)        0 2020-07-29 20:02:56.000000 GraphCASE-0.0.9/GAE/__init__.py
+-rw-rw-rw-   0 tonpoppe   (501) staff       (20)     6564 2020-07-21 05:00:15.000000 GraphCASE-0.0.9/GAE/dataFeeder.py
+-rwxr-xr-x   0 tonpoppe   (501) staff       (20)    11515 2023-06-02 10:58:22.000000 GraphCASE-0.0.9/GAE/data_feeder_graphframes.py
+-rwxr-xr-x   0 tonpoppe   (501) staff       (20)    13402 2023-05-26 07:12:59.000000 GraphCASE-0.0.9/GAE/data_feeder_nx.py
+-rw-r--r--   0 tonpoppe   (501) staff       (20)    16783 2023-06-09 07:11:56.000000 GraphCASE-0.0.9/GAE/graph_case_controller.py
+-rw-r--r--   0 tonpoppe   (501) staff       (20)     3867 2023-06-02 13:25:09.000000 GraphCASE-0.0.9/GAE/graph_case_tools.py
+-rw-r--r--   0 tonpoppe   (501) staff       (20)     8247 2023-06-05 08:32:48.000000 GraphCASE-0.0.9/GAE/graph_reconstructor.py
+-rw-r--r--   0 tonpoppe   (501) staff       (20)    13464 2023-06-05 17:58:06.000000 GraphCASE-0.0.9/GAE/input_layer_constructor.py
+-rw-r--r--   0 tonpoppe   (501) staff       (20)     8746 2023-05-26 07:12:59.000000 GraphCASE-0.0.9/GAE/model.py
+-rw-r--r--   0 tonpoppe   (501) staff       (20)    13478 2023-06-05 18:29:55.000000 GraphCASE-0.0.9/GAE/position_manager.py
+-rw-r--r--   0 tonpoppe   (501) staff       (20)     6979 2023-05-26 07:12:59.000000 GraphCASE-0.0.9/GAE/transformation_layer.py
+drwxr-xr-x   0 tonpoppe   (501) staff       (20)        0 2023-06-09 07:13:36.329713 GraphCASE-0.0.9/GraphCASE.egg-info/
+-rw-r--r--   0 tonpoppe   (501) staff       (20)      296 2023-06-09 07:13:35.000000 GraphCASE-0.0.9/GraphCASE.egg-info/PKG-INFO
+-rw-r--r--   0 tonpoppe   (501) staff       (20)      425 2023-06-09 07:13:36.000000 GraphCASE-0.0.9/GraphCASE.egg-info/SOURCES.txt
+-rw-r--r--   0 tonpoppe   (501) staff       (20)        1 2023-06-09 07:13:35.000000 GraphCASE-0.0.9/GraphCASE.egg-info/dependency_links.txt
+-rw-r--r--   0 tonpoppe   (501) staff       (20)        4 2023-06-09 07:13:36.000000 GraphCASE-0.0.9/GraphCASE.egg-info/top_level.txt
+-rw-r--r--   0 tonpoppe   (501) staff       (20)    35149 2020-07-19 21:06:49.000000 GraphCASE-0.0.9/LICENSE.txt
+-rw-r--r--   0 tonpoppe   (501) staff       (20)      296 2023-06-09 07:13:36.330243 GraphCASE-0.0.9/PKG-INFO
+-rw-r--r--   0 tonpoppe   (501) staff       (20)     7404 2022-09-19 17:31:14.000000 GraphCASE-0.0.9/README.md
+-rw-r--r--   0 tonpoppe   (501) staff       (20)       38 2023-06-09 07:13:36.330683 GraphCASE-0.0.9/setup.cfg
+-rw-r--r--   0 tonpoppe   (501) staff       (20)      322 2023-06-09 07:13:31.000000 GraphCASE-0.0.9/setup.py
```

### Comparing `GraphCASE-0.0.8/GAE/dataFeeder.py` & `GraphCASE-0.0.9/GAE/dataFeeder.py`

 * *Files identical despite different names*

### Comparing `GraphCASE-0.0.8/GAE/data_feeder_graphframes.py` & `GraphCASE-0.0.9/GAE/data_feeder_graphframes.py`

 * *Files identical despite different names*

### Comparing `GraphCASE-0.0.8/GAE/data_feeder_nx.py` & `GraphCASE-0.0.9/GAE/data_feeder_nx.py`

 * *Files identical despite different names*

### Comparing `GraphCASE-0.0.8/GAE/graph_case_controller.py` & `GraphCASE-0.0.9/GAE/graph_case_controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -254,39 +254,40 @@
             if graph is not None:
                 self.sampler = self.__init_sampler(graph, self.val_fraction)
 
             layers = [None]
             if layer_wise:
                 layers = [i for i in range(len(self.dims))] + layers
 
-            for _, l in enumerate(layers):
+        for _, l in enumerate(layers):
+            with tf.device(self.cpu):
                 self.model.sub_model_layer = l
                 self.sampler.init_train_batch()
                 train_data = self.sampler.get_train_samples()
                 validation_data = self.sampler.get_val_samples()
 
                 train_epoch_size, val_epoch_size = self.sampler.get_epoch_sizes()
                 steps_per_epoch = int(train_epoch_size / self.batch_size)
                 assert steps_per_epoch>0, "batch_size greater then 1 train epoch"
                 validation_steps = int(val_epoch_size / self.batch_size)
                 assert validation_steps>0, "batch_size greater then 1 validation epoch"
-                # early_stop = tf.keras.callbacks.EarlyStopping(
-                #     monitor='val_loss', min_delta=0, patience=3, verbose=0
-                # )
-                with tf.device(self.mpu):
-                    history = self.model.fit(
-                        train_data,
-                        validation_data=validation_data,
-                        epochs=epochs,
-                        verbose=model_verbose,
-                        steps_per_epoch=steps_per_epoch,
-                        validation_steps=validation_steps,
-                        # callbacks=[early_stop]
-                    )
-                hist[l] = history
+            # early_stop = tf.keras.callbacks.EarlyStopping(
+            #     monitor='val_loss', min_delta=0, patience=3, verbose=0
+            # )
+            with tf.device(self.mpu):
+                history = self.model.fit(
+                    train_data,
+                    validation_data=validation_data,
+                    epochs=epochs,
+                    verbose=model_verbose,
+                    steps_per_epoch=steps_per_epoch,
+                    validation_steps=validation_steps,
+                    # callbacks=[early_stop]
+                )
+            hist[l] = history
         return hist
 
     def fit_supervised(
         self, label_name, model, compiler_dict, train_dict, graph=None, verbose=None):
         """
         expends the GAE with a supervised model and trains the model and the given graph or if
         none is provide the current graph.
```

### Comparing `GraphCASE-0.0.8/GAE/graph_case_tools.py` & `GraphCASE-0.0.9/GAE/graph_case_tools.py`

 * *Files identical despite different names*

### Comparing `GraphCASE-0.0.8/GAE/graph_reconstructor.py` & `GraphCASE-0.0.9/GAE/graph_reconstructor.py`

 * *Files identical despite different names*

### Comparing `GraphCASE-0.0.8/GAE/input_layer_constructor.py` & `GraphCASE-0.0.9/GAE/input_layer_constructor.py`

 * *Files identical despite different names*

### Comparing `GraphCASE-0.0.8/GAE/model.py` & `GraphCASE-0.0.9/GAE/model.py`

 * *Files identical despite different names*

### Comparing `GraphCASE-0.0.8/GAE/position_manager.py` & `GraphCASE-0.0.9/GAE/position_manager.py`

 * *Files identical despite different names*

### Comparing `GraphCASE-0.0.8/GAE/transformation_layer.py` & `GraphCASE-0.0.9/GAE/transformation_layer.py`

 * *Files identical despite different names*

### Comparing `GraphCASE-0.0.8/LICENSE.txt` & `GraphCASE-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `GraphCASE-0.0.8/README.md` & `GraphCASE-0.0.9/README.md`

 * *Files identical despite different names*

