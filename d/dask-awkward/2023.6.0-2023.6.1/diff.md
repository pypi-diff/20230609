# Comparing `tmp/dask_awkward-2023.6.0.tar.gz` & `tmp/dask_awkward-2023.6.1.tar.gz`

## Comparing `dask_awkward-2023.6.0.tar` & `dask_awkward-2023.6.1.tar`

### file list

```diff
@@ -1,29 +1,31 @@
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 dask_awkward-2023.6.0/src/dask_awkward/__init__.py
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 dask_awkward-2023.6.0/src/dask_awkward/awkward.yaml
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 dask_awkward-2023.6.0/src/dask_awkward/config.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dask_awkward-2023.6.0/src/dask_awkward/py.typed
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 dask_awkward-2023.6.0/src/dask_awkward/sizeof.py
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 dask_awkward-2023.6.0/src/dask_awkward/typing.py
--rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 dask_awkward-2023.6.0/src/dask_awkward/utils.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 dask_awkward-2023.6.0/src/dask_awkward/version.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 dask_awkward-2023.6.0/src/dask_awkward/version.pyi
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 dask_awkward-2023.6.0/src/dask_awkward/layers/__init__.py
--rw-r--r--   0        0        0     6818 2020-02-02 00:00:00.000000 dask_awkward-2023.6.0/src/dask_awkward/layers/layers.py
--rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 dask_awkward-2023.6.0/src/dask_awkward/lib/__init__.py
--rw-r--r--   0        0        0    61474 2020-02-02 00:00:00.000000 dask_awkward-2023.6.0/src/dask_awkward/lib/core.py
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 dask_awkward-2023.6.0/src/dask_awkward/lib/describe.py
--rw-r--r--   0        0        0     2319 2020-02-02 00:00:00.000000 dask_awkward-2023.6.0/src/dask_awkward/lib/inspect.py
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 dask_awkward-2023.6.0/src/dask_awkward/lib/operations.py
--rw-r--r--   0        0        0    15303 2020-02-02 00:00:00.000000 dask_awkward-2023.6.0/src/dask_awkward/lib/optimize.py
--rw-r--r--   0        0        0    11155 2020-02-02 00:00:00.000000 dask_awkward-2023.6.0/src/dask_awkward/lib/reducers.py
--rw-r--r--   0        0        0    27429 2020-02-02 00:00:00.000000 dask_awkward-2023.6.0/src/dask_awkward/lib/structure.py
--rw-r--r--   0        0        0     6327 2020-02-02 00:00:00.000000 dask_awkward-2023.6.0/src/dask_awkward/lib/testutils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dask_awkward-2023.6.0/src/dask_awkward/lib/io/__init__.py
--rw-r--r--   0        0        0    16762 2020-02-02 00:00:00.000000 dask_awkward-2023.6.0/src/dask_awkward/lib/io/io.py
--rw-r--r--   0        0        0    15217 2020-02-02 00:00:00.000000 dask_awkward-2023.6.0/src/dask_awkward/lib/io/json.py
--rw-r--r--   0        0        0    14163 2020-02-02 00:00:00.000000 dask_awkward-2023.6.0/src/dask_awkward/lib/io/parquet.py
--rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 dask_awkward-2023.6.0/.gitignore
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 dask_awkward-2023.6.0/LICENSE
--rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 dask_awkward-2023.6.0/README.md
--rw-r--r--   0        0        0     3480 2020-02-02 00:00:00.000000 dask_awkward-2023.6.0/pyproject.toml
--rw-r--r--   0        0        0     3281 2020-02-02 00:00:00.000000 dask_awkward-2023.6.0/PKG-INFO
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 dask_awkward-2023.6.1/src/dask_awkward/__init__.py
+-rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 dask_awkward-2023.6.1/src/dask_awkward/awkward.yaml
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 dask_awkward-2023.6.1/src/dask_awkward/config.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dask_awkward-2023.6.1/src/dask_awkward/py.typed
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 dask_awkward-2023.6.1/src/dask_awkward/sizeof.py
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 dask_awkward-2023.6.1/src/dask_awkward/typing.py
+-rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 dask_awkward-2023.6.1/src/dask_awkward/utils.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 dask_awkward-2023.6.1/src/dask_awkward/version.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 dask_awkward-2023.6.1/src/dask_awkward/version.pyi
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 dask_awkward-2023.6.1/src/dask_awkward/layers/__init__.py
+-rw-r--r--   0        0        0     8078 2020-02-02 00:00:00.000000 dask_awkward-2023.6.1/src/dask_awkward/layers/layers.py
+-rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 dask_awkward-2023.6.1/src/dask_awkward/lib/__init__.py
+-rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 dask_awkward-2023.6.1/src/dask_awkward/lib/_utils.py
+-rw-r--r--   0        0        0    63654 2020-02-02 00:00:00.000000 dask_awkward-2023.6.1/src/dask_awkward/lib/core.py
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 dask_awkward-2023.6.1/src/dask_awkward/lib/describe.py
+-rw-r--r--   0        0        0     3607 2020-02-02 00:00:00.000000 dask_awkward-2023.6.1/src/dask_awkward/lib/inspect.py
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 dask_awkward-2023.6.1/src/dask_awkward/lib/operations.py
+-rw-r--r--   0        0        0    15367 2020-02-02 00:00:00.000000 dask_awkward-2023.6.1/src/dask_awkward/lib/optimize.py
+-rw-r--r--   0        0        0    11155 2020-02-02 00:00:00.000000 dask_awkward-2023.6.1/src/dask_awkward/lib/reducers.py
+-rw-r--r--   0        0        0    27429 2020-02-02 00:00:00.000000 dask_awkward-2023.6.1/src/dask_awkward/lib/structure.py
+-rw-r--r--   0        0        0     6327 2020-02-02 00:00:00.000000 dask_awkward-2023.6.1/src/dask_awkward/lib/testutils.py
+-rw-r--r--   0        0        0    12797 2020-02-02 00:00:00.000000 dask_awkward-2023.6.1/src/dask_awkward/lib/unproject_layout.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dask_awkward-2023.6.1/src/dask_awkward/lib/io/__init__.py
+-rw-r--r--   0        0        0    16791 2020-02-02 00:00:00.000000 dask_awkward-2023.6.1/src/dask_awkward/lib/io/io.py
+-rw-r--r--   0        0        0    15217 2020-02-02 00:00:00.000000 dask_awkward-2023.6.1/src/dask_awkward/lib/io/json.py
+-rw-r--r--   0        0        0    14994 2020-02-02 00:00:00.000000 dask_awkward-2023.6.1/src/dask_awkward/lib/io/parquet.py
+-rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 dask_awkward-2023.6.1/.gitignore
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 dask_awkward-2023.6.1/LICENSE
+-rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 dask_awkward-2023.6.1/README.md
+-rw-r--r--   0        0        0     3480 2020-02-02 00:00:00.000000 dask_awkward-2023.6.1/pyproject.toml
+-rw-r--r--   0        0        0     3281 2020-02-02 00:00:00.000000 dask_awkward-2023.6.1/PKG-INFO
```

### Comparing `dask_awkward-2023.6.0/src/dask_awkward/awkward.yaml` & `dask_awkward-2023.6.1/src/dask_awkward/awkward.yaml`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.6.0/src/dask_awkward/typing.py` & `dask_awkward-2023.6.1/src/dask_awkward/typing.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.6.0/src/dask_awkward/utils.py` & `dask_awkward-2023.6.1/src/dask_awkward/utils.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.6.0/src/dask_awkward/layers/layers.py` & `dask_awkward-2023.6.1/src/dask_awkward/layers/layers.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import copy
 import pickle
 from collections.abc import Callable, Mapping
 from typing import TYPE_CHECKING, Any
 
 from dask.blockwise import Blockwise, BlockwiseDepDict, blockwise_token
+from dask.highlevelgraph import MaterializedLayer
 
 from dask_awkward.utils import LazyInputsDict
 
 if TYPE_CHECKING:
     from awkward.typetracer import TypeTracerReport
 
 
@@ -129,15 +130,15 @@
         TypeTracerReport
             The mutable report object that is updated upon computation
             of a graph starting with the new AwkwardInputLayer.
 
         """
         import awkward as ak
 
-        from dask_awkward.lib.core import set_form_keys
+        from dask_awkward.lib._utils import set_form_keys
 
         starting_form = copy.deepcopy(self._meta.layout.form)
         starting_layout = starting_form.length_zero_array(highlevel=False)
         new_meta = ak.Array(
             starting_layout.to_typetracer(forget_length=True),
             behavior=self._behavior,
         )
@@ -164,27 +165,66 @@
     def project_columns(self, columns: list[str]) -> AwkwardInputLayer:
         if hasattr(self.io_func, "project_columns"):
             # TODO: make project_columns call sites never pass in an
             # empty list.
             if len(columns) == 0:
                 columns = self._meta.fields[:1]
 
-            # requested columns to original order; adds on extra columns, which are probably
-            # wildcard ones
-            form_columns = self._meta.layout.form.columns()
-            original = [c for c in form_columns if c in columns]
-            new = [c for c in columns if c not in form_columns]
+            # original form
+            original_form = self._meta.layout.form
+
+            # original columns before column projection
+            original_form_columns = original_form.columns()
+
+            # make sure that the requested columns match the order of
+            # the original columns; tack on "new" columns that are
+            # likely the wildcard columns.
+            original = [c for c in original_form_columns if c in columns]
+            new = [c for c in columns if c not in original_form_columns]
             columns = original + new
-            io_func = self.io_func.project_columns(columns)
+
+            try:
+                io_func = self.io_func.project_columns(
+                    columns,
+                    original_form=original_form,
+                )
+            except TypeError:
+                io_func = self.io_func.project_columns(columns)
             return AwkwardInputLayer(
                 name=self.name,
                 columns=columns,
                 inputs=self.inputs,
                 io_func=io_func,
                 label=self.label,
                 produces_tasks=self.produces_tasks,
                 creation_info=self.creation_info,
                 annotations=self.annotations,
                 meta=self._meta,
                 behavior=self._behavior,
             )
         return self
+
+
+class AwkwardMaterializedLayer(MaterializedLayer):
+    def __init__(self, mapping, previous_layer_name, **kwargs):
+        self.prev_name = previous_layer_name
+        super().__init__(mapping, **kwargs)
+
+    def mock(self):
+        mapping = self.mapping.copy()
+        if not mapping:
+            # no partitions at all
+            return self
+        name = next(iter(mapping))[0]
+
+        if (name, 0) in mapping:
+            task = mapping[(name, 0)]
+            task = tuple(
+                (self.prev_name, 0)
+                if isinstance(v, tuple) and len(v) == 2 and v[0] == self.prev_name
+                else v
+                for v in task
+            )
+            return MaterializedLayer({(name, 0): task})
+
+        # failed to cull during column opt
+        return self
```

### Comparing `dask_awkward-2023.6.0/src/dask_awkward/lib/__init__.py` & `dask_awkward-2023.6.1/src/dask_awkward/lib/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from dask_awkward.lib.core import Array, Record, Scalar
 from dask_awkward.lib.core import _type as type
 from dask_awkward.lib.core import map_partitions, typetracer_from_form
 from dask_awkward.lib.describe import fields
-from dask_awkward.lib.inspect import necessary_columns
+from dask_awkward.lib.inspect import necessary_columns, sample
 from dask_awkward.lib.io.io import (
     ImplementsFormTransformation,
     from_awkward,
     from_dask_array,
     from_delayed,
     from_lists,
     from_map,
```

### Comparing `dask_awkward-2023.6.0/src/dask_awkward/lib/core.py` & `dask_awkward-2023.6.1/src/dask_awkward/lib/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 from dask.delayed import Delayed
 from dask.highlevelgraph import HighLevelGraph
 from dask.threaded import get as threaded_get
 from dask.utils import IndexCallable, funcname, key_split
 from numpy.lib.mixins import NDArrayOperatorsMixin
 from tlz import first
 
-from dask_awkward.layers import AwkwardBlockwiseLayer
+from dask_awkward.layers import AwkwardBlockwiseLayer, AwkwardMaterializedLayer
 from dask_awkward.lib.optimize import all_optimizations
 from dask_awkward.typing import AwkwardDaskCollection
 from dask_awkward.utils import (
     DaskAwkwardNotImplemented,
     IncompatiblePartitions,
     hyphenize,
     is_empty_slice,
@@ -702,15 +702,15 @@
         raw = normalize_index(index, (self.npartitions,))
         index = tuple(slice(k, k + 1) if isinstance(k, Number) else k for k in raw)  # type: ignore
         name = f"partitions-{token}"
         new_keys = self.keys_array[index].tolist()
         dsk = {(name, i): tuple(key) for i, key in enumerate(new_keys)}
         graph = HighLevelGraph.from_collections(
             name,
-            dsk,
+            AwkwardMaterializedLayer(dsk, previous_layer_name=self.name),
             dependencies=[self],
         )
 
         # if a single partition was requested we trivially know the new divisions.
         if len(raw) == 1 and isinstance(raw[0], int) and self.known_divisions:
             new_divisions = (
                 0,
@@ -861,35 +861,103 @@
                 _outer_int_getitem_fn,
                 partition.__dask_keys__()[0],
                 where,
             )
         }
         hlg = HighLevelGraph.from_collections(
             name,
-            dsk,
+            AwkwardMaterializedLayer(dsk, previous_layer_name=self.name),
             dependencies=[partition],
         )
         if isinstance(new_meta, ak.Record):
             return new_record_object(hlg, name, meta=new_meta)
         else:
             return new_scalar_object(hlg, name, meta=new_meta)
 
+    def _getitem_slice_on_zero(self, where: tuple[slice, ...]):
+        # normalise
+        sl: slice = where[0]
+        rest = tuple(where[1:])
+        step = sl.step or 1
+        start = sl.start or 0
+
+        if not self.known_divisions:
+            self.eager_compute_divisions()
+        stop = sl.stop or self.divisions[-1]
+        start = start if start >= 0 else self.divisions[-1] + start
+        stop = stop if stop >= 0 else self.divisions[-1] + stop
+        if step < 0:
+            raise DaskAwkwardNotImplemented("negative step slice on zeroth dimension")
+
+        # setup
+        token = tokenize(self, where)
+        name = f"getitem-{token}"
+        remainder = 0
+        outpart = 0
+        divisions = [0]
+        dask = {}
+        # make low-level graph
+        for i in range(self.npartitions):
+            if start > self.divisions[i + 1]:
+                # first partition not found
+                continue
+            if stop < self.divisions[i] and dask:
+                # no more partitions with valid rows
+                # does **NOT** exit if there are no partitions yet, to make sure there is always
+                # at least one, needed to get metadata of empty output right
+                break
+            slice_start = max(start - self.divisions[i] + remainder, 0)
+            slice_end = min(stop - self.divisions[i], self.divisions[i + 1])
+            if (
+                slice_end == slice_start
+                and (self.divisions[i + 1] - self.divisions[i])
+                and dask
+            ):
+                # in case of zero-row last partition (if not only partition)
+                break
+            dask[(name, outpart)] = (
+                _zero_getitem,
+                (self.name, i),
+                slice(slice_start, slice_end, step),
+                rest,
+            )
+            outpart += 1
+            remainder += (self.divisions[i + 1] - self.divisions[i]) % step
+            divisions.append(
+                (self.divisions[i + 1] - self.divisions[i]) // step + divisions[-1]
+            )
+            remainder = remainder % step
+        hlg = HighLevelGraph.from_collections(
+            name,
+            AwkwardMaterializedLayer(dask, previous_layer_name=self.name),
+            dependencies=[self],
+        )
+        return new_array_object(
+            hlg,
+            name,
+            meta=self._meta,
+            behavior=self.behavior,
+            divisions=tuple(divisions),
+        )
+
     def _getitem_tuple(self, where: tuple[Any, ...]) -> Array:
         if isinstance(where[0], int):
             return self._getitem_outer_int(where)
 
         elif isinstance(where[0], str):
             return self._getitem_outer_str_or_list(where)
 
         elif isinstance(where[0], list):
             return self._getitem_outer_str_or_list(where)
 
         elif isinstance(where[0], slice) and is_empty_slice(where[0]):
             return self._getitem_trivial_map_partitions(where)
 
+        elif isinstance(where[0], slice):
+            return self._getitem_slice_on_zero(where)
         # boolean array
         elif isinstance(where[0], Array):
             try:
                 dtype = where[0].layout.dtype.type
             except AttributeError:
                 dtype = where[0].layout.content.dtype.type
             if issubclass(dtype, (np.bool_, bool, np.int64, np.int32, int)):
@@ -910,33 +978,37 @@
         )
 
     def _getitem_single(self, where: Any) -> Array:
         # a single string
         if isinstance(where, str):
             return self._getitem_outer_str_or_list(where, label=where)
 
+        # an empty slice
+
+        elif is_empty_slice(where):
+            return self
+
         elif isinstance(where, list):
             return self._getitem_outer_str_or_list(where)
 
+        elif isinstance(where, slice):
+            return self._getitem_slice_on_zero((where,))
+
         # a single integer
         elif isinstance(where, int):
             return self._getitem_outer_int(where)
 
         elif isinstance(where, Array):
             layout = where.layout
             while not hasattr(layout, "dtype"):
                 layout = layout.content
             dtype = layout.dtype.type
             if issubclass(dtype, (np.bool_, bool, np.int64, np.int32, int)):
                 return self._getitem_outer_bool_or_int_lazy_array(where)
 
-        # an empty slice
-        elif is_empty_slice(where):
-            return self
-
         # a single ellipsis
         elif where is Ellipsis:
             return self
 
         elif self.npartitions == 1:
             return self.map_partitions(operator.getitem, where)
 
@@ -1194,14 +1266,36 @@
         return to_parquet(self, path, storage_options=storage_options, **kwargs)
 
     def to_dask_bag(self) -> DaskBag:
         from dask_awkward.lib.io.io import to_dask_bag
 
         return to_dask_bag(self)
 
+    def head(self, nrow=10, compute=True):
+        """First few rows of the array
+
+        These rows are taken only from the first partition for simplicity. If that partition
+        has fewer rows than ``nrow``, no attempt is made to fetch more from subsequent
+        partitions.
+
+        By default this is then processed eagerly and returned.
+        """
+        out: Array = self.partitions[0].map_partitions(
+            lambda x: x[:nrow], meta=self._meta
+        )
+        if compute:
+            return out.compute()
+        if self.known_divisions:
+            out._divisions = (0, min(nrow, self.divisions[1]))
+        return out
+
+
+def _zero_getitem(arr: ak.Array, zeroth: slice, rest: tuple[slice, ...]) -> ak.Array:
+    return arr.__getitem__((zeroth,) + rest)
+
 
 def compute_typetracer(dsk: HighLevelGraph, name: str) -> ak.Array:
     key = (name, 0)
     return typetracer_array(
         Delayed(
             key,
             dsk.cull({key}),
@@ -1948,54 +2042,7 @@
     -------
     awkward.Array
         Resulting highlevel typetracer Array
 
     """
     layout = form.length_zero_array(highlevel=False)
     return ak.Array(layout.to_typetracer(forget_length=True))
-
-
-def set_form_keys(form: Form, *, key: str) -> Form:
-    """Recursive function to apply key labels to `form`.
-
-    Parameters
-    ----------
-    form : awkward.forms.form.Form
-        Awkward Array form object to mutate.
-    key : str
-        Label to apply. If recursion is triggered by passing in a
-        Record Form, the key is used as a prefix for a specific
-        field.
-
-    Returns
-    -------
-    awkward.forms.form.Form
-        Mutated Form object.
-
-    """
-
-    # If the form is a record we need to loop over all fields in the
-    # record and set form that include the field name; this will keep
-    # recursing as well.
-    if form.is_record:
-        for field in form.fields:
-            full_key = f"{key}.{field}"
-            set_form_keys(form.content(field), key=full_key)
-
-    # If the form is a list (e.g. ListOffsetArray) we append a
-    # __list__ suffix to notify the optimization pass that we only
-    # touched the offsets and not the data buffer for this kind of
-    # identified form; keep recursing
-    elif form.is_list:
-        form.form_key = f"{key}.__list__"
-        set_form_keys(form.content, key=key)
-
-    # NumPy like array is easy
-    elif form.is_numpy:
-        form.form_key = key
-
-    # Anything else grab the content and keep recursing
-    else:
-        set_form_keys(form.content, key=key)
-
-    # Return the now mutated Form object.
-    return form
```

### Comparing `dask_awkward-2023.6.0/src/dask_awkward/lib/describe.py` & `dask_awkward-2023.6.1/src/dask_awkward/lib/describe.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.6.0/src/dask_awkward/lib/operations.py` & `dask_awkward-2023.6.1/src/dask_awkward/lib/operations.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.6.0/src/dask_awkward/lib/optimize.py` & `dask_awkward-2023.6.1/src/dask_awkward/lib/optimize.py`

 * *Files 1% similar despite different names*

```diff
@@ -470,9 +470,11 @@
         for field in imeta.fields:
             wholecol = f"{col[:-2]}.{field}"
             if wholecol in good_columns:
                 break
         else:
             if imeta.fields:
                 good_columns.append(f"{col[:-2]}.{imeta.fields[0]}")
+            else:
+                good_columns.append(col[:-2])
 
     return good_columns
```

### Comparing `dask_awkward-2023.6.0/src/dask_awkward/lib/reducers.py` & `dask_awkward-2023.6.1/src/dask_awkward/lib/reducers.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.6.0/src/dask_awkward/lib/structure.py` & `dask_awkward-2023.6.1/src/dask_awkward/lib/structure.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.6.0/src/dask_awkward/lib/testutils.py` & `dask_awkward-2023.6.1/src/dask_awkward/lib/testutils.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.6.0/src/dask_awkward/lib/io/io.py` & `dask_awkward-2023.6.1/src/dask_awkward/lib/io/io.py`

 * *Files 1% similar despite different names*

```diff
@@ -403,15 +403,17 @@
     intermediate = map_partitions(
         ak.to_dataframe,
         array,
         meta=empty_typetracer(),
         label="to-dataframe",
         **kwargs,
     )
-    meta = ak.to_dataframe(array._meta.layout.form.length_zero_array(), **kwargs)
+    meta = ak.to_dataframe(
+        array._meta.layout.form.length_zero_array(highlevel=False), **kwargs
+    )
     return new_dd_object(
         intermediate.dask,
         intermediate.name,
         meta,
         intermediate.divisions,
     )
```

### Comparing `dask_awkward-2023.6.0/src/dask_awkward/lib/io/json.py` & `dask_awkward-2023.6.1/src/dask_awkward/lib/io/json.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.6.0/src/dask_awkward/lib/io/parquet.py` & `dask_awkward-2023.6.1/src/dask_awkward/lib/io/parquet.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import logging
 import math
 import operator
 from typing import Any, Sequence
 
 import awkward as ak
 import fsspec
+from awkward.forms.form import Form
 from awkward.operations import ak_from_parquet, to_arrow_table
 from awkward.operations.ak_from_parquet import _load
 from dask.base import tokenize
 from dask.blockwise import BlockIndex
 from dask.highlevelgraph import HighLevelGraph
 from fsspec import AbstractFileSystem
 from fsspec.core import get_fs_token_paths
@@ -21,50 +22,57 @@
     Array,
     Scalar,
     map_partitions,
     new_scalar_object,
     typetracer_array,
 )
 from dask_awkward.lib.io.io import from_map
+from dask_awkward.lib.unproject_layout import unproject_layout
 
 log = logging.getLogger(__name__)
 
 
 class _FromParquetFn:
     def __init__(
         self,
         *,
         fs: AbstractFileSystem,
         schema: Any,
         listsep: str = "list.item",
         unnamed_root: bool = False,
+        original_form: Form | None = None,
     ) -> None:
         self.fs = fs
         self.schema = schema
         self.listsep = listsep
         self.unnamed_root = unnamed_root
         self.columns = self.schema.columns(self.listsep)
         if self.unnamed_root:
             self.columns = [f".{c}" for c in self.columns]
+        self.original_form = original_form
 
     @abc.abstractmethod
     def __call__(self, source: Any) -> ak.Array:
         ...
 
     @abc.abstractmethod
-    def project_columns(self, columns: Sequence[str] | None) -> _FromParquetFn:
+    def project_columns(
+        self,
+        columns: Sequence[str] | None,
+        orignal_form: Form | None = None,
+    ) -> _FromParquetFn:
         ...
 
     def __repr__(self) -> str:
         s = (
             "\nFromParquetFn(\n"
             f"  schema={repr(self.schema)}\n"
             f"  listsep={self.listsep}\n"
             f"  unnamed_root={self.unnamed_root}\n"
-            f"  self.columns={self.columns}\n)"
+            f"  columns={self.columns}\n"
         )
         return s
 
     def __str__(self) -> str:
         return self.__repr__()
 
 
@@ -72,37 +80,48 @@
     def __init__(
         self,
         *,
         fs: AbstractFileSystem,
         schema: Any,
         listsep: str = "list.item",
         unnamed_root: bool = False,
+        original_form: Form | None = None,
     ) -> None:
         super().__init__(
-            fs=fs, schema=schema, listsep=listsep, unnamed_root=unnamed_root
+            fs=fs,
+            schema=schema,
+            listsep=listsep,
+            unnamed_root=unnamed_root,
+            original_form=original_form,
         )
 
     def __call__(self, source: Any) -> Any:
-        return _file_to_partition(
+        array = _file_to_partition(
             source,
             self.fs,
             self.columns,
             self.schema,
         )
+        return ak.Array(unproject_layout(self.original_form, array.layout))
 
-    def project_columns(self, columns: Sequence[str] | None) -> _FromParquetFileWiseFn:
+    def project_columns(
+        self,
+        columns: Sequence[str] | None,
+        original_form: Form | None = None,
+    ) -> _FromParquetFileWiseFn:
         if columns is None:
             return self
 
         new_schema = self.schema.select_columns(columns)
         new = _FromParquetFileWiseFn(
             fs=self.fs,
             schema=new_schema,
             listsep=self.listsep,
             unnamed_root=self.unnamed_root,
+            original_form=original_form,
         )
 
         log.debug(f"project_columns received: {columns}")
         log.debug(f"new schema is {repr(new_schema)}")
         log.debug(f"new schema columns are: {new_schema.columns(self.listsep)}")
         log.debug(new)
 
@@ -113,41 +132,49 @@
     def __init__(
         self,
         *,
         fs: AbstractFileSystem,
         schema: Any,
         listsep: str = "list.item",
         unnamed_root: bool = False,
+        original_form: Form | None = None,
     ) -> None:
         super().__init__(
-            fs=fs, schema=schema, listsep=listsep, unnamed_root=unnamed_root
+            fs=fs,
+            schema=schema,
+            listsep=listsep,
+            unnamed_root=unnamed_root,
+            original_form=original_form,
         )
 
     def __call__(self, pair: Any) -> ak.Array:
         subrg, source = pair
         if isinstance(subrg, int):
             subrg = [[subrg]]
-        return _file_to_partition(
+        array = _file_to_partition(
             source,
             self.fs,
             self.columns,
             self.schema,
             subrg=subrg,
         )
+        return ak.Array(unproject_layout(self.original_form, array.layout))
 
     def project_columns(
         self,
         columns: Sequence[str] | None,
+        original_form: Form | None = None,
     ) -> _FromParquetFragmentWiseFn:
         if columns is None:
             return self
         return _FromParquetFragmentWiseFn(
             fs=self.fs,
             schema=self.schema.select_columns(columns),
             unnamed_root=self.unnamed_root,
+            original_form=original_form,
         )
 
 
 def from_parquet(
     path: Any,
     storage_options: dict | None = None,
     ignore_metadata: bool = True,
```

### Comparing `dask_awkward-2023.6.0/.gitignore` & `dask_awkward-2023.6.1/.gitignore`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.6.0/LICENSE` & `dask_awkward-2023.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.6.0/README.md` & `dask_awkward-2023.6.1/README.md`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.6.0/pyproject.toml` & `dask_awkward-2023.6.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
   "Programming Language :: Python :: 3 :: Only",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Topic :: Scientific/Engineering",
 ]
 dependencies = [
-  "awkward >=2.2.1",
+  "awkward >=2.2.2",
   "dask >=2023.04.0",
 ]
 dynamic = ["version"]
 
 [project.urls]
 Homepage = "https://github.com/dask-contrib/dask-awkward"
 "Bug Tracker" = "https://github.com/dask-contrib/dask-awkward/issues"
```

### Comparing `dask_awkward-2023.6.0/PKG-INFO` & `dask_awkward-2023.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dask-awkward
-Version: 2023.6.0
+Version: 2023.6.1
 Summary: Awkward Array meets Dask
 Project-URL: Homepage, https://github.com/dask-contrib/dask-awkward
 Project-URL: Bug Tracker, https://github.com/dask-contrib/dask-awkward/issues
 Author-email: Doug Davis <ddavis@ddavis.io>, Martin Durant <mdurant@anaconda.com>
 Maintainer-email: Doug Davis <ddavis@ddavis.io>, Martin Durant <mdurant@anaconda.com>
 License: BSD-3-Clause
 License-File: LICENSE
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.8
-Requires-Dist: awkward>=2.2.1
+Requires-Dist: awkward>=2.2.2
 Requires-Dist: dask>=2023.04.0
 Provides-Extra: complete
 Requires-Dist: aiohttp; extra == 'complete'
 Requires-Dist: pyarrow; extra == 'complete'
 Requires-Dist: pytest-cov>=3.0.0; extra == 'complete'
 Requires-Dist: pytest>=6.0; extra == 'complete'
 Requires-Dist: requests>=2.27.1; extra == 'complete'
```

