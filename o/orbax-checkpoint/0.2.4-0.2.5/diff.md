# Comparing `tmp/orbax_checkpoint-0.2.4.tar.gz` & `tmp/orbax_checkpoint-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orbax_checkpoint-0.2.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "orbax_checkpoint-0.2.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `orbax_checkpoint-0.2.4.tar` & `orbax_checkpoint-0.2.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0    11357 2023-06-01 15:35:33.579835 orbax_checkpoint-0.2.4/LICENSE
--rw-r--r--   0        0        0      834 2023-06-01 15:35:33.587835 orbax_checkpoint-0.2.4/README.md
--rw-r--r--   0        0        0     2666 2023-06-01 15:35:33.587835 orbax_checkpoint-0.2.4/orbax/checkpoint/__init__.py
--rw-r--r--   0        0        0     2599 2023-06-01 15:35:33.587835 orbax_checkpoint-0.2.4/orbax/checkpoint/abstract_checkpointer.py
--rw-r--r--   0        0        0     2629 2023-06-01 15:35:33.587835 orbax_checkpoint-0.2.4/orbax/checkpoint/aggregate_handlers.py
--rw-r--r--   0        0        0     5348 2023-06-01 15:35:33.587835 orbax_checkpoint-0.2.4/orbax/checkpoint/array_checkpoint_handler.py
--rw-r--r--   0        0        0     1440 2023-06-01 15:35:33.587835 orbax_checkpoint-0.2.4/orbax/checkpoint/async_checkpoint_handler.py
--rw-r--r--   0        0        0     4744 2023-06-01 15:35:33.587835 orbax_checkpoint-0.2.4/orbax/checkpoint/async_checkpointer.py
--rw-r--r--   0        0        0     2119 2023-06-01 15:35:33.587835 orbax_checkpoint-0.2.4/orbax/checkpoint/checkpoint_handler.py
--rw-r--r--   0        0        0    35205 2023-06-01 15:35:33.587835 orbax_checkpoint-0.2.4/orbax/checkpoint/checkpoint_manager.py
--rw-r--r--   0        0        0     9920 2023-06-01 15:35:33.587835 orbax_checkpoint-0.2.4/orbax/checkpoint/checkpoint_utils.py
--rw-r--r--   0        0        0     7190 2023-06-01 15:35:33.587835 orbax_checkpoint-0.2.4/orbax/checkpoint/checkpoint_utils_test.py
--rw-r--r--   0        0        0     4022 2023-06-01 15:35:33.587835 orbax_checkpoint-0.2.4/orbax/checkpoint/checkpointer.py
--rw-r--r--   0        0        0      740 2023-06-01 15:35:33.587835 orbax_checkpoint-0.2.4/orbax/checkpoint/conftest.py
--rw-r--r--   0        0        0     1465 2023-06-01 15:35:33.587835 orbax_checkpoint-0.2.4/orbax/checkpoint/future.py
--rw-r--r--   0        0        0     2103 2023-06-01 15:35:33.587835 orbax_checkpoint-0.2.4/orbax/checkpoint/json_checkpoint_handler.py
--rw-r--r--   0        0        0     1821 2023-06-01 15:35:33.587835 orbax_checkpoint-0.2.4/orbax/checkpoint/json_checkpoint_handler_test.py
--rw-r--r--   0        0        0     2002 2023-06-01 15:35:33.587835 orbax_checkpoint-0.2.4/orbax/checkpoint/lazy_utils.py
--rw-r--r--   0        0        0     7672 2023-06-01 15:35:33.587835 orbax_checkpoint-0.2.4/orbax/checkpoint/msgpack_utils.py
--rw-r--r--   0        0        0     1129 2023-06-01 15:35:33.587835 orbax_checkpoint-0.2.4/orbax/checkpoint/msgpack_utils_test.py
--rw-r--r--   0        0        0    45137 2023-06-01 15:35:33.587835 orbax_checkpoint-0.2.4/orbax/checkpoint/orbax_checkpoint.ipynb
--rw-r--r--   0        0        0    22735 2023-06-01 15:35:33.587835 orbax_checkpoint-0.2.4/orbax/checkpoint/pytree_checkpoint_handler.py
--rw-r--r--   0        0        0     5333 2023-06-01 15:35:33.587835 orbax_checkpoint-0.2.4/orbax/checkpoint/test_utils.py
--rw-r--r--   0        0        0    10077 2023-06-01 15:35:33.587835 orbax_checkpoint-0.2.4/orbax/checkpoint/transform_utils.py
--rw-r--r--   0        0        0    15155 2023-06-01 15:35:33.587835 orbax_checkpoint-0.2.4/orbax/checkpoint/transform_utils_test.py
--rw-r--r--   0        0        0    23039 2023-06-01 15:35:33.587835 orbax_checkpoint-0.2.4/orbax/checkpoint/type_handlers.py
--rw-r--r--   0        0        0    21981 2023-06-01 15:35:33.587835 orbax_checkpoint-0.2.4/orbax/checkpoint/utils.py
--rw-r--r--   0        0        0     7465 2023-06-01 15:35:33.587835 orbax_checkpoint-0.2.4/orbax/checkpoint/utils_test.py
--rw-r--r--   0        0        0     1172 2023-06-01 15:35:33.587835 orbax_checkpoint-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     1976 1970-01-01 00:00:00.000000 orbax_checkpoint-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-09 17:35:07.026293 orbax_checkpoint-0.2.5/LICENSE
+-rw-r--r--   0        0        0      834 2023-06-09 17:35:07.026293 orbax_checkpoint-0.2.5/README.md
+-rw-r--r--   0        0        0     2666 2023-06-09 17:35:07.026293 orbax_checkpoint-0.2.5/orbax/checkpoint/__init__.py
+-rw-r--r--   0        0        0     2599 2023-06-09 17:35:07.026293 orbax_checkpoint-0.2.5/orbax/checkpoint/abstract_checkpointer.py
+-rw-r--r--   0        0        0     2629 2023-06-09 17:35:07.026293 orbax_checkpoint-0.2.5/orbax/checkpoint/aggregate_handlers.py
+-rw-r--r--   0        0        0     5348 2023-06-09 17:35:07.026293 orbax_checkpoint-0.2.5/orbax/checkpoint/array_checkpoint_handler.py
+-rw-r--r--   0        0        0     1440 2023-06-09 17:35:07.026293 orbax_checkpoint-0.2.5/orbax/checkpoint/async_checkpoint_handler.py
+-rw-r--r--   0        0        0     4744 2023-06-09 17:35:07.026293 orbax_checkpoint-0.2.5/orbax/checkpoint/async_checkpointer.py
+-rw-r--r--   0        0        0     2119 2023-06-09 17:35:07.026293 orbax_checkpoint-0.2.5/orbax/checkpoint/checkpoint_handler.py
+-rw-r--r--   0        0        0    35838 2023-06-09 17:35:07.026293 orbax_checkpoint-0.2.5/orbax/checkpoint/checkpoint_manager.py
+-rw-r--r--   0        0        0     9920 2023-06-09 17:35:07.026293 orbax_checkpoint-0.2.5/orbax/checkpoint/checkpoint_utils.py
+-rw-r--r--   0        0        0     7190 2023-06-09 17:35:07.026293 orbax_checkpoint-0.2.5/orbax/checkpoint/checkpoint_utils_test.py
+-rw-r--r--   0        0        0     4022 2023-06-09 17:35:07.026293 orbax_checkpoint-0.2.5/orbax/checkpoint/checkpointer.py
+-rw-r--r--   0        0        0      740 2023-06-09 17:35:07.026293 orbax_checkpoint-0.2.5/orbax/checkpoint/conftest.py
+-rw-r--r--   0        0        0     1465 2023-06-09 17:35:07.026293 orbax_checkpoint-0.2.5/orbax/checkpoint/future.py
+-rw-r--r--   0        0        0     2103 2023-06-09 17:35:07.026293 orbax_checkpoint-0.2.5/orbax/checkpoint/json_checkpoint_handler.py
+-rw-r--r--   0        0        0     1821 2023-06-09 17:35:07.026293 orbax_checkpoint-0.2.5/orbax/checkpoint/json_checkpoint_handler_test.py
+-rw-r--r--   0        0        0     2002 2023-06-09 17:35:07.026293 orbax_checkpoint-0.2.5/orbax/checkpoint/lazy_utils.py
+-rw-r--r--   0        0        0     7672 2023-06-09 17:35:07.026293 orbax_checkpoint-0.2.5/orbax/checkpoint/msgpack_utils.py
+-rw-r--r--   0        0        0     1129 2023-06-09 17:35:07.026293 orbax_checkpoint-0.2.5/orbax/checkpoint/msgpack_utils_test.py
+-rw-r--r--   0        0        0    45137 2023-06-09 17:35:07.026293 orbax_checkpoint-0.2.5/orbax/checkpoint/orbax_checkpoint.ipynb
+-rw-r--r--   0        0        0    23131 2023-06-09 17:35:07.026293 orbax_checkpoint-0.2.5/orbax/checkpoint/pytree_checkpoint_handler.py
+-rw-r--r--   0        0        0     5333 2023-06-09 17:35:07.026293 orbax_checkpoint-0.2.5/orbax/checkpoint/test_utils.py
+-rw-r--r--   0        0        0    10077 2023-06-09 17:35:07.030293 orbax_checkpoint-0.2.5/orbax/checkpoint/transform_utils.py
+-rw-r--r--   0        0        0    15155 2023-06-09 17:35:07.030293 orbax_checkpoint-0.2.5/orbax/checkpoint/transform_utils_test.py
+-rw-r--r--   0        0        0    23039 2023-06-09 17:35:07.030293 orbax_checkpoint-0.2.5/orbax/checkpoint/type_handlers.py
+-rw-r--r--   0        0        0    22307 2023-06-09 17:35:07.030293 orbax_checkpoint-0.2.5/orbax/checkpoint/utils.py
+-rw-r--r--   0        0        0     7465 2023-06-09 17:35:07.030293 orbax_checkpoint-0.2.5/orbax/checkpoint/utils_test.py
+-rw-r--r--   0        0        0     1172 2023-06-09 17:35:07.030293 orbax_checkpoint-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     1976 1970-01-01 00:00:00.000000 orbax_checkpoint-0.2.5/PKG-INFO
```

### Comparing `orbax_checkpoint-0.2.4/LICENSE` & `orbax_checkpoint-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.2.4/README.md` & `orbax_checkpoint-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.2.4/orbax/checkpoint/__init__.py` & `orbax_checkpoint-0.2.5/orbax/checkpoint/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,8 +54,8 @@
 # Convenient shorthand where instead of the following:
 #   `checkpointer = Checkpointer(PyTreeCheckpointer())`
 # we can just use:
 #   `checkpointer = PyTreeCheckpointer()`
 PyTreeCheckpointer = functools.partial(Checkpointer, PyTreeCheckpointHandler())
 
 # A new PyPI release will be pushed everytime `__version__` is increased.
-__version__ = '0.2.4'
+__version__ = '0.2.5'
```

### Comparing `orbax_checkpoint-0.2.4/orbax/checkpoint/abstract_checkpointer.py` & `orbax_checkpoint-0.2.5/orbax/checkpoint/abstract_checkpointer.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.2.4/orbax/checkpoint/aggregate_handlers.py` & `orbax_checkpoint-0.2.5/orbax/checkpoint/aggregate_handlers.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.2.4/orbax/checkpoint/array_checkpoint_handler.py` & `orbax_checkpoint-0.2.5/orbax/checkpoint/array_checkpoint_handler.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.2.4/orbax/checkpoint/async_checkpoint_handler.py` & `orbax_checkpoint-0.2.5/orbax/checkpoint/async_checkpoint_handler.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.2.4/orbax/checkpoint/async_checkpointer.py` & `orbax_checkpoint-0.2.5/orbax/checkpoint/async_checkpointer.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.2.4/orbax/checkpoint/checkpoint_handler.py` & `orbax_checkpoint-0.2.5/orbax/checkpoint/checkpoint_handler.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.2.4/orbax/checkpoint/checkpoint_manager.py` & `orbax_checkpoint-0.2.5/orbax/checkpoint/checkpoint_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""CheckpointManager, a sync implementation of AbstractCheckpointManager."""
+"""A class providing functionalities for managing multiple checkpoints."""
 
 import asyncio
 import dataclasses
 import datetime
 import threading
 from typing import Any, Callable, Container, List, Mapping, Optional, Sequence, Tuple, Union
 import uuid
@@ -85,15 +85,19 @@
 class CheckpointManagerOptions:
   """Optional arguments for CheckpointManager.
 
   save_interval_steps: the interval at which checkpoints should be saved.
   Ensures checkpoints will only be saved every n steps. Defaults to 1.
   max_to_keep: if provided, specifies the maximum number of checkpoints to
     keep. Older checkpoints are removed. By default, does not remove any old
-    checkpoints.
+    checkpoints. Must be None or non-negative. When set, checkpoints
+    may be considered for deletion when there are more than `max_to_keep`
+    checkpoints present. Checkpoints are kept if they meet any of the conditions
+    below, such as `keep_time_interval`, `keep_period`, etc. Any remaining
+    checkpoints that do not meet these conditions are garbage-collected.
   keep_time_interval: When more than max_to_keep checkpoints are present,
     an older checkpoint that would ordinarily be deleted will be preserved if it
     has been at least `keep_time_interval` since the previous preserved
     checkpoint. The default setting of `None` does not preserve any checkpoints
     in this way. For example, this may be used to ensure checkpoints are
     retained at a frequency of approximately than one per hour.
   keep_period: If set, will not delete any checkpoint where checkpoint_step %
@@ -134,14 +138,16 @@
 
   def __post_init__(self):
     if self.best_mode not in ('min', 'max'):
       msg = ("`CheckpointManagerOptions.best_mode` must be one of None, 'min' "
              "or 'max'. Got {self.dtype}.")
       raise ValueError(msg)
     self.save_on_steps = frozenset(self.save_on_steps or ())
+    if self.max_to_keep is not None and self.max_to_keep < 0:
+      raise ValueError('Setting of `max_to_keep` must be None or non-negative.')
 
 
 @dataclasses.dataclass
 class CheckpointInfo:
   """Metadata about a checkpoint."""
   step: int
   time: datetime.datetime
@@ -765,16 +771,16 @@
   def _delete_directory(self, step: int):
     if jax.process_index() == 0:
       # TODO(cpgaffney) Optimize tree removal if possible.
       self._get_save_directory(step, self.directory).rmtree()
 
   def _remove_old_checkpoints(self):
     """Keeps the `max_to_keep` most recent checkpoint steps."""
-    # Must have set max_to_keep or keep_time_interval.
-    if not self._options.max_to_keep and not self._options.keep_time_interval:
+    # Must have set max_to_keep in order to remove any checkpoints.
+    if self._options.max_to_keep is None:
       return
     # Not enough checkpoints accumulated to consider deletion.
     if len(self._checkpoints) <= self._options.max_to_keep:
       return
     if self._track_best:
       # Best steps (to keep) are at the end, after sorting.
       (
@@ -784,21 +790,26 @@
     else:
       # checkpoints already sorted by ascending step
       checkpoints_without_metrics = []
       sorted_checkpoints = self._checkpoints
 
     keep = int(self._options.max_to_keep)
     if self._options.keep_checkpoints_without_metrics:
-      maybe_delete = sorted_checkpoints[:-keep]
-      active_checkpoints = checkpoints_without_metrics + sorted_checkpoints[
-          -keep:]
+      maybe_delete = (
+          sorted_checkpoints[:-keep] if keep > 0 else sorted_checkpoints
+      )
+      active_checkpoints = (
+          checkpoints_without_metrics + sorted_checkpoints[-keep:]
+          if keep > 0
+          else []
+      )
     else:
       all_checkpoints = checkpoints_without_metrics + sorted_checkpoints
-      maybe_delete = all_checkpoints[:-keep]
-      active_checkpoints = all_checkpoints[-keep:]
+      maybe_delete = all_checkpoints[:-keep] if keep > 0 else sorted_checkpoints
+      active_checkpoints = all_checkpoints[-keep:] if keep > 0 else []
 
     kept_checkpoints = []
     for info in maybe_delete:
       if (
           self._options.keep_time_interval is not None
           and self._interval_preserved_checkpoints
       ):
```

### Comparing `orbax_checkpoint-0.2.4/orbax/checkpoint/checkpoint_utils.py` & `orbax_checkpoint-0.2.5/orbax/checkpoint/checkpoint_utils.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.2.4/orbax/checkpoint/checkpoint_utils_test.py` & `orbax_checkpoint-0.2.5/orbax/checkpoint/checkpoint_utils_test.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.2.4/orbax/checkpoint/checkpointer.py` & `orbax_checkpoint-0.2.5/orbax/checkpoint/checkpointer.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.2.4/orbax/checkpoint/conftest.py` & `orbax_checkpoint-0.2.5/orbax/checkpoint/conftest.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.2.4/orbax/checkpoint/future.py` & `orbax_checkpoint-0.2.5/orbax/checkpoint/future.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.2.4/orbax/checkpoint/json_checkpoint_handler.py` & `orbax_checkpoint-0.2.5/orbax/checkpoint/json_checkpoint_handler.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.2.4/orbax/checkpoint/json_checkpoint_handler_test.py` & `orbax_checkpoint-0.2.5/orbax/checkpoint/json_checkpoint_handler_test.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.2.4/orbax/checkpoint/lazy_utils.py` & `orbax_checkpoint-0.2.5/orbax/checkpoint/lazy_utils.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.2.4/orbax/checkpoint/msgpack_utils.py` & `orbax_checkpoint-0.2.5/orbax/checkpoint/msgpack_utils.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.2.4/orbax/checkpoint/msgpack_utils_test.py` & `orbax_checkpoint-0.2.5/orbax/checkpoint/msgpack_utils_test.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.2.4/orbax/checkpoint/orbax_checkpoint.ipynb` & `orbax_checkpoint-0.2.5/orbax/checkpoint/orbax_checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.2.4/orbax/checkpoint/pytree_checkpoint_handler.py` & `orbax_checkpoint-0.2.5/orbax/checkpoint/pytree_checkpoint_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,20 @@
 
 async def _create_param_save_dir(param_info: ParamInfo, args: SaveArgs):
   # Directory will be unused.
   path = param_info.path
   if path is None or args.aggregate:
     return
   if jax.process_index() == 0:
-    await utils.async_makedirs(path)
+    # TODO(b/273803615): Note that keys with slashes ('/', generated by Haiku,
+    # for example) will result in the creation of nested sub-directories, rather
+    # than flat parameter directories like for a standard neste PyTree. This
+    # discrepancy, while potentially problematic, will not be addressed since we
+    # anticipate moving fully to OCDBT within a quarter or two.
+    await utils.async_makedirs(path, parents=True)
 
 
 def _maybe_set_default_save_args(value, args):
   # If already set, return.
   if isinstance(args, SaveArgs):
     return args
   aggregate = not type_handlers.has_type_handler(type(value))
```

### Comparing `orbax_checkpoint-0.2.4/orbax/checkpoint/test_utils.py` & `orbax_checkpoint-0.2.5/orbax/checkpoint/test_utils.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.2.4/orbax/checkpoint/transform_utils.py` & `orbax_checkpoint-0.2.5/orbax/checkpoint/transform_utils.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.2.4/orbax/checkpoint/transform_utils_test.py` & `orbax_checkpoint-0.2.5/orbax/checkpoint/transform_utils_test.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.2.4/orbax/checkpoint/type_handlers.py` & `orbax_checkpoint-0.2.5/orbax/checkpoint/type_handlers.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.2.4/orbax/checkpoint/utils.py` & `orbax_checkpoint-0.2.5/orbax/checkpoint/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -456,27 +456,37 @@
                          primary_host: Optional[int] = 0) -> epath.Path:
   """Creates a temporary directory for saving at the given path."""
   # Share a timestamp across devices.
   final_dir = epath.Path(final_dir)
   # Renames are not atomic in GCS. Save directly to final_dir and rely on commit
   # completion file to indicate success.
   if is_gcs_path(final_dir):
-    # Sync needed to prevent an error since caller may think the directory
-    # exists from a previous save, rather than just having been created.
-    sync_global_devices('create_tmp_directory:pre')
     tmp_dir = final_dir
   else:
     tmp_dir = get_tmp_directory(final_dir)
 
+  if tmp_dir.exists():
+    if is_gcs_path(tmp_dir):
+      raise FileExistsError(
+          f'Attempted to create temporary directory {tmp_dir} which already'
+          ' exists.'
+      )
+    else:
+      raise AssertionError(
+          f'Attempted to create temporary directory {tmp_dir} which already'
+          ' exists. This condition should never arise on non-GCS'
+          ' filesystems.'
+      )
+  # Sync after existence check to ensure that the directory has not just been
+  # created by another host.
+  sync_global_devices('create_tmp_directory:pre')
+
   if primary_host is None or jax.process_index() == primary_host:
-    assert not tmp_dir.exists()
     tmp_dir.mkdir(parents=True)
-
   sync_global_devices('create_tmp_directory')
-
   return tmp_dir
 
 
 def ensure_atomic_save(temp_ckpt_dir: epath.Path, final_ckpt_dir: epath.Path):
   """Finalizes atomic save by renaming tmp_dir or writing a success file."""
   if temp_ckpt_dir == final_ckpt_dir:
     (final_ckpt_dir / _COMMIT_SUCCESS_FILE
```

### Comparing `orbax_checkpoint-0.2.4/orbax/checkpoint/utils_test.py` & `orbax_checkpoint-0.2.5/orbax/checkpoint/utils_test.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.2.4/pyproject.toml` & `orbax_checkpoint-0.2.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.2.4/PKG-INFO` & `orbax_checkpoint-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orbax-checkpoint
-Version: 0.2.4
+Version: 0.2.5
 Summary: Orbax Checkpoint
 Keywords: JAX machine learning,checkpoint,training
 Author-email: Orbax Authors <orbax-dev@google.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

