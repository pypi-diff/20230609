# Comparing `tmp/coola-0.0.7.tar.gz` & `tmp/coola-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coola-0.0.7.tar", max compression
+gzip compressed data, was "coola-0.0.8.tar", max compression
```

## Comparing `coola-0.0.7.tar` & `coola-0.0.8.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0     1501 2023-05-16 02:38:26.151940 coola-0.0.7/LICENSE
--rw-r--r--   0        0        0     5049 2023-05-16 02:38:26.151940 coola-0.0.7/README.md
--rw-r--r--   0        0        0     4111 2023-05-16 02:38:26.151940 coola-0.0.7/pyproject.toml
--rw-r--r--   0        0        0      682 2023-05-16 02:38:26.151940 coola-0.0.7/src/coola/__init__.py
--rw-r--r--   0        0        0    18466 2023-05-16 02:38:26.151940 coola-0.0.7/src/coola/allclose.py
--rw-r--r--   0        0        0    13177 2023-05-16 02:38:26.151940 coola-0.0.7/src/coola/equality.py
--rw-r--r--   0        0        0     4261 2023-05-16 02:38:26.151940 coola-0.0.7/src/coola/ndarray.py
--rw-r--r--   0        0        0     7522 2023-05-16 02:38:26.151940 coola-0.0.7/src/coola/pytorch.py
--rw-r--r--   0        0        0      297 2023-05-16 02:38:26.151940 coola-0.0.7/src/coola/testing.py
--rw-r--r--   0        0        0        0 2023-05-16 02:38:26.151940 coola-0.0.7/src/coola/utils/__init__.py
--rw-r--r--   0        0        0     2456 2023-05-16 02:38:26.151940 coola-0.0.7/src/coola/utils/format.py
--rw-r--r--   0        0        0     1195 2023-05-16 02:38:26.155939 coola-0.0.7/src/coola/utils/imports.py
--rw-r--r--   0        0        0     6349 1970-01-01 00:00:00.000000 coola-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1501 2023-06-09 05:31:29.801109 coola-0.0.8/LICENSE
+-rw-r--r--   0        0        0     5043 2023-06-09 05:31:29.801109 coola-0.0.8/README.md
+-rw-r--r--   0        0        0     4147 2023-06-09 05:31:29.805109 coola-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0      939 2023-06-09 05:31:29.805109 coola-0.0.8/src/coola/__init__.py
+-rw-r--r--   0        0        0     4251 2023-06-09 05:31:29.805109 coola-0.0.8/src/coola/_numpy.py
+-rw-r--r--   0        0        0     7410 2023-06-09 05:31:29.805109 coola-0.0.8/src/coola/_torch.py
+-rw-r--r--   0        0        0     2632 2023-06-09 05:31:29.805109 coola-0.0.8/src/coola/_xarray.py
+-rw-r--r--   0        0        0    18491 2023-06-09 05:31:29.805109 coola-0.0.8/src/coola/allclose.py
+-rw-r--r--   0        0        0    13211 2023-06-09 05:31:29.805109 coola-0.0.8/src/coola/equality.py
+-rw-r--r--   0        0        0      489 2023-06-09 05:31:29.805109 coola-0.0.8/src/coola/testing.py
+-rw-r--r--   0        0        0        0 2023-06-09 05:31:29.805109 coola-0.0.8/src/coola/utils/__init__.py
+-rw-r--r--   0        0        0     2490 2023-06-09 05:31:29.805109 coola-0.0.8/src/coola/utils/format.py
+-rw-r--r--   0        0        0     1842 2023-06-09 05:31:29.805109 coola-0.0.8/src/coola/utils/imports.py
+-rw-r--r--   0        0        0     6243 1970-01-01 00:00:00.000000 coola-0.0.8/PKG-INFO
```

### Comparing `coola-0.0.7/LICENSE` & `coola-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `coola-0.0.7/README.md` & `coola-0.0.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         <img  alt="Monthly downloads" src="https://static.pepy.tech/badge/coola/month">
     </a>
     <br/>
 </p>
 
 ## Overview
 
-`coola` is a light Python library that provides simple functions to check in a single line if two
+`coola` is a Python library that provides simple functions to check in a single line if two
 complex/nested objects are equal or not.
 `coola` was initially designed to work
 with [PyTorch `Tensor`s](https://pytorch.org/docs/stable/tensors.html)
 and [NumPy `ndarray`](https://numpy.org/doc/stable/reference/generated/numpy.ndarray.html), but it
 is possible to extend it
 to [support other data structures](https://durandtibo.github.io/coola/customization).
 
@@ -71,16 +71,16 @@
 
 ```python
 import numpy
 import torch
 
 from coola import objects_are_equal
 
-data1 = {'torch': torch.ones(2, 3), 'numpy': numpy.zeros((2, 3))}
-data2 = {'torch': torch.zeros(2, 3), 'numpy': numpy.ones((2, 3))}
+data1 = {"torch": torch.ones(2, 3), "numpy": numpy.zeros((2, 3))}
+data2 = {"torch": torch.zeros(2, 3), "numpy": numpy.ones((2, 3))}
 
 objects_are_equal(data1, data2)
 ```
 
 `coola` also provides a function `objects_are_allclose` that can indicate if two complex/nested
 objects are equal within a tolerance or not.
```

#### html2text {}

```diff
@@ -1,32 +1,32 @@
 # coola
           [CI] [CI] [Codecov] [https://api.codeclimate.com/v1/badges/
  83ebb50e6c6f67b0570d/maintainability] [https://api.codeclimate.com/v1/badges/
                      83ebb50e6c6f67b0570d/test_coverage]
 [PYPI_version] [Python] [BSD-3-Clause] [Code_style:_black] [Doc_style:_google]
                        [Downloads] [Monthly_downloads]
-## Overview `coola` is a light Python library that provides simple functions to
-check in a single line if two complex/nested objects are equal or not. `coola`
-was initially designed to work with [PyTorch `Tensor`s](https://pytorch.org/
-docs/stable/tensors.html) and [NumPy `ndarray`](https://numpy.org/doc/stable/
+## Overview `coola` is a Python library that provides simple functions to check
+in a single line if two complex/nested objects are equal or not. `coola` was
+initially designed to work with [PyTorch `Tensor`s](https://pytorch.org/docs/
+stable/tensors.html) and [NumPy `ndarray`](https://numpy.org/doc/stable/
 reference/generated/numpy.ndarray.html), but it is possible to extend it to
 [support other data structures](https://durandtibo.github.io/coola/
 customization). - [Motivation](#motivation) - [Documentation](https://
 durandtibo.github.io/coola/) - [Installation](#installation) - [Contributing]
 (#contributing) - [API stability](#api-stability) - [License](#license) ##
 Motivation Let's imagine you have the following dictionaries that contain both
 a PyTorch `Tensor` and a NumPy `ndarray`. You want to check if the two
 dictionaries are equal or not. By default, Python does not provide an easy way
 to check if the two dictionaries are equal or not. It is not possible to use
 the default equality operator `==` because it will raise an error. The `coola`
 library was developed to fill this gap. `coola` provides a function
 `objects_are_equal` that can indicate if two complex/nested objects are equal
 or not. ```python import numpy import torch from coola import objects_are_equal
-data1 = {'torch': torch.ones(2, 3), 'numpy': numpy.zeros((2, 3))} data2 =
-{'torch': torch.zeros(2, 3), 'numpy': numpy.ones((2, 3))} objects_are_equal
+data1 = {"torch": torch.ones(2, 3), "numpy": numpy.zeros((2, 3))} data2 =
+{"torch": torch.zeros(2, 3), "numpy": numpy.ones((2, 3))} objects_are_equal
 (data1, data2) ``` `coola` also provides a function `objects_are_allclose` that
 can indicate if two complex/nested objects are equal within a tolerance or not.
 ```python from coola import objects_are_allclose objects_are_allclose(data1,
 data2, atol=1e-6) ``` Please check the [quickstart page](https://
 durandtibo.github.io/coola/quickstart) to learn more on how to use `coola`. ##
 Installation We highly recommend installing a [virtual environment](https://
 packaging.python.org/guides/installing-using-pip-and-virtual-environments/).
```

### Comparing `coola-0.0.7/pyproject.toml` & `coola-0.0.8/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "coola"
-version = "0.0.7"
+version = "0.0.8"
 description = "A light library to check if two complex/nested objects are equal or not"
 readme = "README.md"
 authors = ["Thibaut Durand <durand.tibo+gh@gmail.com>"]
 homepage = "https://github.com/durandtibo/coola"
 repository = "https://github.com/durandtibo/coola"
 keywords = ["equality", "complex/nested objects"]
 license = "BSD-3-Clause"
@@ -26,33 +26,34 @@
 packages = [
     { include = "coola", from = "src" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 numpy = { version = "^1.20", optional = true }
-torch = { version = ">= 1.10, < 3.0", optional = true}
+torch = { version = ">=1.10,<3.0", optional = true}
+xarray = { version = ">=2022.3.0", optional = true}
 
 [tool.poetry.extras]
-all = ["numpy", "torch"]
+all = ["numpy", "torch", "xarray"]
 
 [tool.poetry.group.docs.dependencies]
 mkdocs-material = "^9.1"
-mkdocstrings = "^0.21"
+mkdocstrings = "^0.22"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3"
-coverage = { extras = ["toml"], version = "^6.5" }
-docformatter = "^1.6"
-pre-commit = "^2.20"
+coverage = { extras = ["toml"], version = "^7.2" }
+docformatter = { extras = ["tomli"], version = "^1.7" }
+pre-commit = "^3.3"
 pylint = "^2.17"
 pytest = "^7.3"
-pytest-cov = "^4.0"
+pytest-cov = "^4.1"
 pytest-timeout = "^2.1"
-ruff = "^0.0.261"
+ruff = "^0.0,>=0.0.272"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.coverage.paths]
 source = ["src", "*/site-packages"]
@@ -61,16 +62,14 @@
 branch = true
 source = ["coola"]
 
 [tool.coverage.report]
 show_missing = true
 exclude_lines = [
     "pragma: no cover",
-    "if is_torch_available()",
-    "if is_numpy_available()",
 ]
 
 [tool.pytest.ini_options]
 testpaths = "tests/"
 log_format = "%(asctime)s - %(levelname)s - %(name)s - %(message)s"
 log_level = "DEBUG"
 addopts = "--color yes --durations 10 -rf"
```

### Comparing `coola-0.0.7/src/coola/allclose.py` & `coola-0.0.8/src/coola/allclose.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 __all__ = [
     "AllCloseTester",
     "BaseAllCloseOperator",
     "BaseAllCloseTester",
     "DefaultAllCloseOperator",
     "MappingAllCloseOperator",
     "ScalarAllCloseOperator",
@@ -9,15 +11,15 @@
     "objects_are_allclose",
 ]
 
 import logging
 import math
 from abc import ABC, abstractmethod
 from collections.abc import Mapping, Sequence
-from typing import Any, Generic, Optional, TypeVar, Union
+from typing import Any, Generic, TypeVar, Union
 
 from coola.utils.format import str_dict, str_indent
 
 logger = logging.getLogger(__name__)
 
 T = TypeVar("T")
 
@@ -53,15 +55,15 @@
 
         Returns:
             bool: ``True`` if the two objects are equal within a
                 tolerance, otherwise ``False``
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from coola import AllCloseTester, BaseAllCloseTester
             >>> tester: BaseAllCloseTester = AllCloseTester()
             >>> tester.allclose(
             ...     [torch.ones(2, 3), torch.zeros(2)],
             ...     [torch.ones(2, 3), torch.zeros(2)],
@@ -85,15 +87,15 @@
 def objects_are_allclose(
     object1: Any,
     object2: Any,
     rtol: float = 1e-5,
     atol: float = 1e-8,
     equal_nan: bool = False,
     show_difference: bool = False,
-    tester: Optional[BaseAllCloseTester] = None,
+    tester: BaseAllCloseTester | None = None,
 ) -> bool:
     r"""Indicates if two objects are equal within a tolerance.
 
     Args:
         object1: Specifies the first object to compare.
         object2: Specifies the second object to compare.
         rtol (float, optional): Specifies the relative tolerance
@@ -112,22 +114,22 @@
 
     Returns:
         bool: ``True`` if the two objects are (element-wise) equal
             within a tolerance, otherwise ``False``
 
     Example usage:
 
-    .. code-block:: python
+    .. code-block:: pycon
 
         >>> import torch
         >>> from coola import objects_are_allclose
         >>> objects_are_allclose(
         ...     [torch.ones(2, 3), torch.zeros(2)],
         ...     [torch.ones(2, 3), torch.zeros(2)],
-        ...     )
+        ... )
         True
         >>> objects_are_allclose(
         ...     [torch.ones(2, 3), torch.ones(2)],
         ...     [torch.ones(2, 3), torch.zeros(2)],
         ... )
         False
         >>> objects_are_allclose(
@@ -258,15 +260,15 @@
 
 class ScalarAllCloseOperator(BaseAllCloseOperator[Union[bool, int, float]]):
     r"""Implements an allclose operator for scalar values."""
 
     def allclose(
         self,
         tester: BaseAllCloseTester,
-        object1: Union[bool, int, float],
+        object1: bool | int | float,
         object2: Any,
         rtol: float = 1e-5,
         atol: float = 1e-8,
         equal_nan: bool = False,
         show_difference: bool = False,
     ) -> bool:
         if type(object1) is not type(object2):
@@ -370,33 +372,34 @@
 
         Raises:
             ValueError if an operator is already registered for the
                 data type and ``exist_ok=False``.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> from coola import (
             ...     AllCloseTester,
             ...     BaseAllCloseTester,
             ...     BaseAllCloseOperator,
             ... )
             >>> class MyStringAllCloseOperator(BaseAllCloseOperator[str]):
-            ...    def allclose(
+            ...     def allclose(
             ...         self,
             ...         tester: BaseAllCloseTester,
             ...         object1: str,
             ...         object2: Any,
             ...         rtol: float = 1e-5,
             ...         atol: float = 1e-8,
             ...         equal_nan: bool = False,
             ...         show_difference: bool = False,
             ...     ) -> bool:
             ...         ...  # Custom implementation to test strings
+            ...
             >>> AllCloseTester.add_allclose_operator(str, MyStringAllCloseOperator())
             # To overwrite an existing operato
             >>> AllCloseTester.add_allclose_operator(str, MyStringAllCloseOperator(), exist_ok=True)
         """
         if data_type in cls.registry and not exist_ok:
             raise RuntimeError(
                 f"An operator ({cls.registry[data_type]}) is already registered for the data "
@@ -432,15 +435,15 @@
 
         Returns:
             bool: ``True`` if the two objects are equal within a
                 tolerance, otherwise ``False``
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from coola import AllCloseTester
             >>> tester = AllCloseTester()
             >>> tester.allclose(
             ...     [torch.ones(2, 3), torch.zeros(2)],
             ...     [torch.ones(2, 3), torch.zeros(2)],
@@ -461,27 +464,27 @@
         """
         return self.find_allclose_operator(type(object1)).allclose(
             self, object1, object2, rtol, atol, equal_nan, show_difference
         )
 
     @classmethod
     def has_allclose_operator(cls, data_type: type[object]) -> bool:
-        r"""Indicates if an allclose operator is registered for the given data
-        type.
+        r"""Indicates if an allclose operator is registered for the given
+        data type.
 
         Args:
             data_type: Specifies the data type to check.
 
         Returns:
             bool: ``True`` if an allclose operator is registered,
                 otherwise ``False``.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> from coola import AllCloseTester
             >>> AllCloseTester.has_allclose_operator(list)
             True
             >>> AllCloseTester.has_allclose_operator(str)
             False
         """
@@ -496,15 +499,15 @@
 
         Returns:
             ``BaseAllCloseOperator``: The allclose operator associated
                 to the data type.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> from coola import AllCloseTester
             >>> AllCloseTester.find_allclose_operator(list)
             SequenceAllCloseOperator()
             >>> AllCloseTester.has_allclose_operator(str)
             DefaultAllCloseOperator()
         """
```

### Comparing `coola-0.0.7/src/coola/equality.py` & `coola-0.0.8/src/coola/equality.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
+from __future__ import annotations
+
 __all__ = [
     "BaseEqualityOperator",
     "BaseEqualityTester",
     "DefaultEqualityOperator",
     "EqualityTester",
     "MappingEqualityOperator",
     "SequenceEqualityOperator",
     "objects_are_equal",
 ]
 
 import logging
 from abc import ABC, abstractmethod
 from collections.abc import Mapping, Sequence
-from typing import Any, Generic, Optional, TypeVar
+from typing import Any, Generic, TypeVar
 
 from coola.utils.format import str_dict, str_indent
 
 logger = logging.getLogger(__name__)
 
 T = TypeVar("T")
 
@@ -37,15 +39,15 @@
 
         Returns:
             bool: ``True`` if the two objects are equal, otherwise
                 ``False``.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from coola import BaseEqualityTester, EqualityTester
             >>> tester: BaseEqualityTester = EqualityTester()
             >>> tester.equal(
             ...     [torch.ones(2, 3), torch.zeros(2)],
             ...     [torch.ones(2, 3), torch.zeros(2)],
@@ -56,15 +58,15 @@
         """
 
 
 def objects_are_equal(
     object1: Any,
     object2: Any,
     show_difference: bool = False,
-    tester: Optional[BaseEqualityTester] = None,
+    tester: BaseEqualityTester | None = None,
 ) -> bool:
     r"""Indicates if two objects are equal or not.
 
     Args:
         object1: Specifies the first object to compare.
         object2: Specifies the second object to compare.
         show_difference (bool, optional): If ``True``, it shows a
@@ -77,15 +79,15 @@
 
     Returns:
         bool: ``True`` if the two nested data are equal, otherwise
             ``False``.
 
     Example usage:
 
-    .. code-block:: python
+    .. code-block:: pycon
 
         >>> import torch
         >>> from coola import objects_are_equal
         >>> objects_are_equal(
         ...     [torch.ones(2, 3), torch.zeros(2)],
         ...     [torch.ones(2, 3), torch.zeros(2)],
         ... )
@@ -258,26 +260,27 @@
 
         Raises:
             ValueError if an operator is already registered for the
                 data type and ``exist_ok=False``.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> from coola import EqualityTester, BaseEqualityTester, BaseEqualityOperator
             >>> class MyStringEqualityOperator(BaseEqualityOperator[str]):
-            ...    def equal(
+            ...     def equal(
             ...         self,
             ...         tester: BaseEqualityTester,
             ...         object1: str,
             ...         object2: Any,
             ...         show_difference: bool = False,
             ...     ) -> bool:
             ...         ...  # Custom implementation to test strings
+            ...
             >>> EqualityTester.add_equality_operator(str, MyStringEqualityOperator())
             # To overwrite an existing operato
             >>> EqualityTester.add_equality_operator(str, MyStringEqualityOperator(), exist_ok=True)
         """
         if data_type in cls.registry and not exist_ok:
             raise RuntimeError(
                 f"An operator ({cls.registry[data_type]}) is already registered for the data "
@@ -299,15 +302,15 @@
 
         Returns:
             bool: ``True`` if the two objects are equal, otherwise
                 ``False``.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from coola import EqualityTester
             >>> tester = EqualityTester()
             >>> tester.equal(
             ...     [torch.ones(2, 3), torch.zeros(2)],
             ...     [torch.ones(2, 3), torch.zeros(2)],
@@ -318,27 +321,27 @@
         """
         return self.find_equality_operator(type(object1)).equal(
             self, object1, object2, show_difference
         )
 
     @classmethod
     def has_equality_operator(cls, data_type: type[object]) -> bool:
-        r"""Indicates if an equality operator is registered for the given data
-        type.
+        r"""Indicates if an equality operator is registered for the given
+        data type.
 
         Args:
             data_type: Specifies the data type to check.
 
         Returns:
             bool: ``True`` if an equality operator is registered,
                 otherwise ``False``.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> from coola import EqualityTester
             >>> EqualityTester.has_equality_operator(list)
             True
             >>> EqualityTester.has_equality_operator(str)
             False
         """
@@ -353,15 +356,15 @@
 
         Returns:
             ``BaseEqualityOperator``: The equality operator associated
                 to the data type.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> from coola import EqualityTester
             >>> EqualityTester.find_equality_operator(list)
             SequenceEqualityOperator()
             >>> EqualityTester.find_equality_operator(str)
             DefaultEqualityOperator()
         """
```

### Comparing `coola-0.0.7/src/coola/ndarray.py` & `coola-0.0.8/src/coola/_numpy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__all__ = ["NDArrayAllCloseOperator", "NDArrayEqualityOperator"]
+from __future__ import annotations
 
 import logging
 from typing import Any
 
 from coola.allclose import AllCloseTester, BaseAllCloseOperator, BaseAllCloseTester
 from coola.equality import BaseEqualityOperator, BaseEqualityTester, EqualityTester
 from coola.utils.imports import check_numpy, is_numpy_available
@@ -104,12 +104,12 @@
             return False
         object_equal = array_equal(object1, object2)
         if show_difference and not object_equal:
             logger.info(f"numpy.ndarrays are different\nobject1=\n{object1}\nobject2=\n{object2}")
         return object_equal
 
 
-if is_numpy_available():
+if is_numpy_available():  # pragma: no cover
     if not AllCloseTester.has_allclose_operator(ndarray):
         AllCloseTester.add_allclose_operator(ndarray, NDArrayAllCloseOperator())
     if not EqualityTester.has_equality_operator(ndarray):
         EqualityTester.add_equality_operator(ndarray, NDArrayEqualityOperator())
```

### Comparing `coola-0.0.7/src/coola/pytorch.py` & `coola-0.0.8/src/coola/_torch.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,21 @@
-__all__ = [
-    "PackedSequenceAllCloseOperator",
-    "PackedSequenceEqualityOperator",
-    "TensorAllCloseOperator",
-    "TensorEqualityOperator",
-]
+from __future__ import annotations
 
 import logging
 from typing import Any
 
 from coola.allclose import AllCloseTester, BaseAllCloseOperator, BaseAllCloseTester
 from coola.equality import BaseEqualityOperator, BaseEqualityTester, EqualityTester
 from coola.utils.imports import check_torch, is_torch_available
 
 if is_torch_available():
     from torch import Tensor, is_tensor
     from torch.nn.utils.rnn import PackedSequence
 else:
-    PackedSequence, Tensor, is_tensor = None, None, None  # pragma: no cover
+    PackedSequence, Tensor = None, None  # pragma: no cover
 
 logger = logging.getLogger(__name__)
 
 
 class PackedSequenceAllCloseOperator(BaseAllCloseOperator[PackedSequence]):
     r"""Implements an allclose operator for
     ``torch.nn.utils.rnn.PackedSequence``."""
@@ -195,15 +190,15 @@
             return False
         object_equal = object1.equal(object2)
         if show_difference and not object_equal:
             logger.info(f"torch.Tensors are different\nobject1=\n{object1}\nobject2=\n{object2}")
         return object_equal
 
 
-if is_torch_available():
+if is_torch_available():  # pragma: no cover
     if not AllCloseTester.has_allclose_operator(PackedSequence):
         AllCloseTester.add_allclose_operator(PackedSequence, PackedSequenceAllCloseOperator())
     if not AllCloseTester.has_allclose_operator(Tensor):
         AllCloseTester.add_allclose_operator(Tensor, TensorAllCloseOperator())
     if not EqualityTester.has_equality_operator(PackedSequence):
         EqualityTester.add_equality_operator(PackedSequence, PackedSequenceEqualityOperator())
     if not EqualityTester.has_equality_operator(Tensor):
```

### Comparing `coola-0.0.7/src/coola/utils/format.py` & `coola-0.0.8/src/coola/utils/format.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 __all__ = ["str_dict", "str_indent"]
 
 from typing import Any
 
 
 def str_dict(data: dict[str, Any], sorted_keys: bool = False, indent: int = 0) -> str:
     r"""Converts a dict to a pretty string representation.
@@ -19,15 +21,15 @@
             should be greater or equal to 0. Default: ``0``
 
     Returns:
         str: The string representation.
 
         Example usage:
 
-    .. code-block:: python
+    .. code-block:: pycon
 
         >>> from coola.utils.format import str_dict
         >>> str_dict({"my_key": "my_value"})
         'my_key : my_value'
         >>> str_dict({"key1": "value1", "key2": "value2"})
         'key1 : value1\nkey2 : value2'
     """
@@ -54,15 +56,15 @@
             used for the indentation. Default: ``2``.
 
     Returns:
         str: The indented string.
 
     Example usage:
 
-    .. code-block:: python
+    .. code-block:: pycon
 
         >>> from coola.utils.format import str_indent
         >>> print(f"\t{str_indent('string1\nstring2', 4)}")
             string1
             string2
     """
     formatted_str = str(original).split("\n")
```

### Comparing `coola-0.0.7/src/coola/utils/imports.py` & `coola-0.0.8/src/coola/utils/imports.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,17 @@
-__all__ = ["check_numpy", "check_torch", "is_numpy_available", "is_torch_available"]
+from __future__ import annotations
+
+__all__ = [
+    "check_numpy",
+    "check_torch",
+    "check_xarray",
+    "is_numpy_available",
+    "is_torch_available",
+    "is_xarray_available",
+]
 
 from importlib.util import find_spec
 
 
 def is_numpy_available() -> bool:
     r"""Indicates if the NumPy package is installed or not."""
     return find_spec("numpy") is not None
@@ -35,7 +44,26 @@
     """
     if not is_torch_available():
         raise RuntimeError(
             "`torch` package is required but not installed. "
             "You can install `torch` package with the command:\n\n"
             "pip install torch\n"
         )
+
+
+def is_xarray_available() -> bool:
+    r"""Indicates if the NumPy package is installed or not."""
+    return find_spec("xarray") is not None
+
+
+def check_xarray() -> None:
+    r"""Checks if the xarray package is installed.
+
+    Raises:
+        RuntimeError if the xarray package is not installed.
+    """
+    if not is_xarray_available():
+        raise RuntimeError(
+            "`xarray` package is required but not installed. "
+            "You can install `xarray` package with the command:\n\n"
+            "pip install xarray\n"
+        )
```

### Comparing `coola-0.0.7/PKG-INFO` & `coola-0.0.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coola
-Version: 0.0.7
+Version: 0.0.8
 Summary: A light library to check if two complex/nested objects are equal or not
 Home-page: https://github.com/durandtibo/coola
 License: BSD-3-Clause
 Keywords: equality,complex/nested objects
 Author: Thibaut Durand
 Author-email: durand.tibo+gh@gmail.com
 Requires-Python: >=3.9,<4.0
@@ -14,22 +14,20 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Libraries
 Provides-Extra: all
 Requires-Dist: numpy (>=1.20,<2.0) ; extra == "all"
 Requires-Dist: torch (>=1.10,<3.0) ; extra == "all"
+Requires-Dist: xarray (>=2022.3.0) ; extra == "all"
 Project-URL: Repository, https://github.com/durandtibo/coola
 Description-Content-Type: text/markdown
 
 # coola
 
 <p align="center">
     <a href="https://github.com/durandtibo/coola/actions">
@@ -71,15 +69,15 @@
         <img  alt="Monthly downloads" src="https://static.pepy.tech/badge/coola/month">
     </a>
     <br/>
 </p>
 
 ## Overview
 
-`coola` is a light Python library that provides simple functions to check in a single line if two
+`coola` is a Python library that provides simple functions to check in a single line if two
 complex/nested objects are equal or not.
 `coola` was initially designed to work
 with [PyTorch `Tensor`s](https://pytorch.org/docs/stable/tensors.html)
 and [NumPy `ndarray`](https://numpy.org/doc/stable/reference/generated/numpy.ndarray.html), but it
 is possible to extend it
 to [support other data structures](https://durandtibo.github.io/coola/customization).
 
@@ -102,16 +100,16 @@
 
 ```python
 import numpy
 import torch
 
 from coola import objects_are_equal
 
-data1 = {'torch': torch.ones(2, 3), 'numpy': numpy.zeros((2, 3))}
-data2 = {'torch': torch.zeros(2, 3), 'numpy': numpy.ones((2, 3))}
+data1 = {"torch": torch.ones(2, 3), "numpy": numpy.zeros((2, 3))}
+data2 = {"torch": torch.zeros(2, 3), "numpy": numpy.ones((2, 3))}
 
 objects_are_equal(data1, data2)
 ```
 
 `coola` also provides a function `objects_are_allclose` that can indicate if two complex/nested
 objects are equal within a tolerance or not.
```

#### html2text {}

```diff
@@ -1,49 +1,47 @@
-Metadata-Version: 2.1 Name: coola Version: 0.0.7 Summary: A light library to
+Metadata-Version: 2.1 Name: coola Version: 0.0.8 Summary: A light library to
 check if two complex/nested objects are equal or not Home-page: https://
 github.com/durandtibo/coola License: BSD-3-Clause Keywords: equality,complex/
 nested objects Author: Thibaut Durand Author-email: durand.tibo+gh@gmail.com
 Requires-Python: >=3.9,<4.0 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Information Technology Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License Classifier: Operating System
 :: POSIX :: Linux Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.11 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Topic :: Scientific/Engineering Classifier: Topic :: Software Development ::
 Libraries Provides-Extra: all Requires-Dist: numpy (>=1.20,<2.0) ; extra ==
-"all" Requires-Dist: torch (>=1.10,<3.0) ; extra == "all" Project-URL:
-Repository, https://github.com/durandtibo/coola Description-Content-Type: text/
-markdown # coola
+"all" Requires-Dist: torch (>=1.10,<3.0) ; extra == "all" Requires-Dist: xarray
+(>=2022.3.0) ; extra == "all" Project-URL: Repository, https://github.com/
+durandtibo/coola Description-Content-Type: text/markdown # coola
           [CI] [CI] [Codecov] [https://api.codeclimate.com/v1/badges/
  83ebb50e6c6f67b0570d/maintainability] [https://api.codeclimate.com/v1/badges/
                      83ebb50e6c6f67b0570d/test_coverage]
 [PYPI_version] [Python] [BSD-3-Clause] [Code_style:_black] [Doc_style:_google]
                        [Downloads] [Monthly_downloads]
-## Overview `coola` is a light Python library that provides simple functions to
-check in a single line if two complex/nested objects are equal or not. `coola`
-was initially designed to work with [PyTorch `Tensor`s](https://pytorch.org/
-docs/stable/tensors.html) and [NumPy `ndarray`](https://numpy.org/doc/stable/
+## Overview `coola` is a Python library that provides simple functions to check
+in a single line if two complex/nested objects are equal or not. `coola` was
+initially designed to work with [PyTorch `Tensor`s](https://pytorch.org/docs/
+stable/tensors.html) and [NumPy `ndarray`](https://numpy.org/doc/stable/
 reference/generated/numpy.ndarray.html), but it is possible to extend it to
 [support other data structures](https://durandtibo.github.io/coola/
 customization). - [Motivation](#motivation) - [Documentation](https://
 durandtibo.github.io/coola/) - [Installation](#installation) - [Contributing]
 (#contributing) - [API stability](#api-stability) - [License](#license) ##
 Motivation Let's imagine you have the following dictionaries that contain both
 a PyTorch `Tensor` and a NumPy `ndarray`. You want to check if the two
 dictionaries are equal or not. By default, Python does not provide an easy way
 to check if the two dictionaries are equal or not. It is not possible to use
 the default equality operator `==` because it will raise an error. The `coola`
 library was developed to fill this gap. `coola` provides a function
 `objects_are_equal` that can indicate if two complex/nested objects are equal
 or not. ```python import numpy import torch from coola import objects_are_equal
-data1 = {'torch': torch.ones(2, 3), 'numpy': numpy.zeros((2, 3))} data2 =
-{'torch': torch.zeros(2, 3), 'numpy': numpy.ones((2, 3))} objects_are_equal
+data1 = {"torch": torch.ones(2, 3), "numpy": numpy.zeros((2, 3))} data2 =
+{"torch": torch.zeros(2, 3), "numpy": numpy.ones((2, 3))} objects_are_equal
 (data1, data2) ``` `coola` also provides a function `objects_are_allclose` that
 can indicate if two complex/nested objects are equal within a tolerance or not.
 ```python from coola import objects_are_allclose objects_are_allclose(data1,
 data2, atol=1e-6) ``` Please check the [quickstart page](https://
 durandtibo.github.io/coola/quickstart) to learn more on how to use `coola`. ##
 Installation We highly recommend installing a [virtual environment](https://
 packaging.python.org/guides/installing-using-pip-and-virtual-environments/).
```

