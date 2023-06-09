# Comparing `tmp/bayesianbandits-0.4.0.tar.gz` & `tmp/bayesianbandits-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bayesianbandits-0.4.0.tar", max compression
+gzip compressed data, was "bayesianbandits-0.4.1.tar", max compression
```

## Comparing `bayesianbandits-0.4.0.tar` & `bayesianbandits-0.4.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1074 2023-06-07 16:57:03.981962 bayesianbandits-0.4.0/LICENSE
--rw-r--r--   0        0        0     1093 2023-06-07 16:57:03.981962 bayesianbandits-0.4.0/README.md
--rw-r--r--   0        0        0     2740 2023-06-07 16:57:03.981962 bayesianbandits-0.4.0/bayesianbandits/__init__.py
--rw-r--r--   0        0        0     3660 2023-06-07 16:57:03.981962 bayesianbandits-0.4.0/bayesianbandits/_arm.py
--rw-r--r--   0        0        0    19549 2023-06-07 16:57:03.981962 bayesianbandits-0.4.0/bayesianbandits/_basebandit.py
--rw-r--r--   0        0        0    29470 2023-06-07 16:57:03.981962 bayesianbandits-0.4.0/bayesianbandits/_estimators.py
--rw-r--r--   0        0        0     1304 2023-06-07 16:57:03.981962 bayesianbandits-0.4.0/bayesianbandits/_np_utils.py
--rw-r--r--   0        0        0     5122 2023-06-07 16:57:03.981962 bayesianbandits-0.4.0/bayesianbandits/_policy_decorators.py
--rw-r--r--   0        0        0     2656 2023-06-07 16:57:03.981962 bayesianbandits-0.4.0/bayesianbandits/_typing.py
--rw-r--r--   0        0        0      705 2023-06-07 16:57:03.989962 bayesianbandits-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     1627 1970-01-01 00:00:00.000000 bayesianbandits-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-06-09 17:22:40.840365 bayesianbandits-0.4.1/LICENSE
+-rw-r--r--   0        0        0     1093 2023-06-09 17:22:40.840365 bayesianbandits-0.4.1/README.md
+-rw-r--r--   0        0        0     2740 2023-06-09 17:22:40.844365 bayesianbandits-0.4.1/bayesianbandits/__init__.py
+-rw-r--r--   0        0        0     3538 2023-06-09 17:22:40.844365 bayesianbandits-0.4.1/bayesianbandits/_arm.py
+-rw-r--r--   0        0        0    20408 2023-06-09 17:22:40.844365 bayesianbandits-0.4.1/bayesianbandits/_basebandit.py
+-rw-r--r--   0        0        0    29470 2023-06-09 17:22:40.844365 bayesianbandits-0.4.1/bayesianbandits/_estimators.py
+-rw-r--r--   0        0        0     1304 2023-06-09 17:22:40.844365 bayesianbandits-0.4.1/bayesianbandits/_np_utils.py
+-rw-r--r--   0        0        0     5036 2023-06-09 17:22:40.844365 bayesianbandits-0.4.1/bayesianbandits/_policy_decorators.py
+-rw-r--r--   0        0        0     2634 2023-06-09 17:22:40.844365 bayesianbandits-0.4.1/bayesianbandits/_typing.py
+-rw-r--r--   0        0        0      705 2023-06-09 17:22:40.852366 bayesianbandits-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     1627 1970-01-01 00:00:00.000000 bayesianbandits-0.4.1/PKG-INFO
```

### Comparing `bayesianbandits-0.4.0/LICENSE` & `bayesianbandits-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bayesianbandits-0.4.0/README.md` & `bayesianbandits-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `bayesianbandits-0.4.0/bayesianbandits/__init__.py` & `bayesianbandits-0.4.1/bayesianbandits/__init__.py`

 * *Files identical despite different names*

### Comparing `bayesianbandits-0.4.0/bayesianbandits/_arm.py` & `bayesianbandits-0.4.1/bayesianbandits/_arm.py`

 * *Files 6% similar despite different names*

```diff
@@ -73,24 +73,19 @@
     def pull(self) -> ActionToken:
         """Pull the arm."""
         return self.action_token
 
     @requires_learner
     def sample(
         self,
-        X: Optional[ArrayLike] = None,
+        X: NDArray[np.float_],
         size: int = 1,
     ) -> NDArray[np.float_]:
         """Sample from learner and compute the reward."""
-        if X is None:
-            X_new = np.array([[1]])
-        else:
-            X_new = np.atleast_2d(X)
-
-        return self.reward_function(self.learner.sample(X_new, size))  # type: ignore
+        return self.reward_function(self.learner.sample(X, size))  # type: ignore
 
     @requires_learner
     def update(self, X: NDArray[np.float_], y: NDArray[np.float_]) -> None:
         """Update the learner.
 
         If y is None, the data in X is used as the target and X is set to
         a `len(X)` rows of ones.
```

### Comparing `bayesianbandits-0.4.0/bayesianbandits/_basebandit.py` & `bayesianbandits-0.4.1/bayesianbandits/_basebandit.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,25 +5,26 @@
     Any,
     Callable,
     ClassVar,
     Collection,
     Dict,
     MutableMapping,
     Optional,
+    Tuple,
     Type,
     TypeVar,
     Union,
     cast,
     overload,
 )
 
 import numpy as np
 from numpy.typing import ArrayLike, NDArray
 from sklearn.base import clone
-from typing_extensions import dataclass_transform
+from typing_extensions import Literal, dataclass_transform
 
 from ._np_utils import groupby_array
 from ._typing import ArmProtocol, BanditProtocol, Learner
 
 
 _B = TypeVar("_B", bound="Bandit")
 
@@ -226,20 +227,17 @@
         Options
         -------
         unique_id : Any
             Unique identifier for the pull. Required when the `@delayed_reward`
             decorator is used.
         """
 
-        if X is None and self._contextual:
-            raise ValueError("X must be an array-like for a contextual bandit.")
-        elif X is not None and not self._contextual:
-            raise ValueError("X must be None for a non-contextual bandit.")
+        X_pull, _ = _validate_arrays(X, None, self._contextual, check_y=False)
 
-        arm = self.policy(X)
+        arm = self.policy(X_pull)
         self.last_arm_pulled = arm
         unique_id = None
 
         if self.__class__._delayed_reward is True:
             unique_id = kwargs.get("unique_id")
             if unique_id is None:
                 raise ValueError(
@@ -297,28 +295,15 @@
 
         Options
         -------
         unique_id : Any
             Unique identifier for the pull. Required when the `@delayed_reward`
             decorator is used.
         """
-        if self._contextual:
-            if y is None:
-                raise ValueError(
-                    "X and y must both be array-likes for a contextual bandit."
-                )
-            y_fit, X_fit = np.atleast_1d(y), np.atleast_2d(X)
-        else:
-            if y is not None:
-                raise ValueError(
-                    "The second argument must be None for a non-contextual bandit."
-                    " The first argument to `update` must be the outcome."
-                )
-            y_fit = np.atleast_1d(X)
-            X_fit = np.ones_like(y_fit, dtype=np.float64)[:, np.newaxis]
+        X_fit, y_fit = _validate_arrays(X, y, self._contextual, check_y=True)
 
         if self.__class__._delayed_reward is True:
             unique_id: Union[Collection[Any], str, None] = kwargs.get("unique_id", None)
             if unique_id is None:
                 raise ValueError(
                     "The `unique_id` keyword argument is required when the "
                     "`delayed_reward = True`."
@@ -375,22 +360,19 @@
         X : Optional[ArrayLike]
             Context for the bandit. Only provided when the @contextual
             decorator is used.
         size : int, default=1
             Number of samples to draw.
 
         """
-        if X is None and self._contextual:
-            raise ValueError("X must be an array-like for a contextual bandit.")
-        elif X is not None and not self._contextual:
-            raise ValueError("X must be None for a non-contextual bandit.")
+        X_sample, _ = _validate_arrays(X, None, self._contextual, check_y=False)
         # choose an arm, draw a sample, and repeat `size` times
         # TODO: this is not the most efficient way to do this
         # but I can't imagine a situation where this would be a bottleneck.
-        return np.array([self.policy(X).sample(X) for _ in range(size)])
+        return np.array([self.policy(X_sample).sample(X_sample) for _ in range(size)])
 
     @overload
     def decay(
         self, /, *, decay_rate: Optional[float] = None, decay_last_arm: bool = True
     ) -> None:
         ...
 
@@ -421,24 +403,17 @@
         ----------
         X : Optional[ArrayLike]
             Context for the bandit. Only provided when the @contextual
             decorator is used.
         decay_last_arm : bool, default=True
             Whether to decay the last arm pulled.
         """
-        if X is None and self._contextual:
-            raise ValueError("X must be an array-like for a contextual bandit.")
-        elif X is not None and not self._contextual:
-            raise ValueError("X must be None for a non-contextual bandit.")
-
-        if not self._contextual:
-            X_decay = np.array([[1]], dtype=float)
-        else:
-            assert X is not None  # for the type checker
-            X_decay = np.atleast_2d(X)
+        X_decay, _ = _validate_arrays(
+            X, None, contextual=self._contextual, check_y=False
+        )
 
         for arm in self.arms.values():
             if decay_last_arm or arm is not self.last_arm_pulled:
                 arm.decay(X_decay, decay_rate=decay_rate)
 
     def __post_init__(self) -> None:
         """Moves all class attributes that are instances of `Arm` to instance
@@ -506,14 +481,87 @@
         return {
             name: attr
             for name, attr in self.__dict__.items()
             if isinstance(attr, ArmProtocol)
         }
 
 
+@overload
+def _validate_arrays(
+    X: ArrayLike,
+    y: Optional[ArrayLike],
+    /,
+    contextual: bool,
+    check_y: Literal[True] = True,
+) -> Tuple[NDArray[np.float_], NDArray[np.float_]]:
+    ...
+
+
+@overload
+def _validate_arrays(
+    X: Optional[ArrayLike],
+    y: Literal[None],
+    /,
+    contextual: bool,
+    check_y: Literal[False] = False,
+) -> Tuple[NDArray[np.float_], None]:
+    ...
+
+
+def _validate_arrays(
+    X: Optional[ArrayLike],
+    y: Optional[ArrayLike],
+    /,
+    contextual: bool,
+    check_y: bool = True,
+) -> Tuple[NDArray[np.float_], Optional[NDArray[np.float_]]]:
+    """Validate the `X` and `y` arrays.
+
+    Parameters
+    ----------
+    X : ArrayLike
+        Context for the bandit. Only provided when the @contextual
+        decorator is used. Otherwise, this position is used for `y`.
+    y : Optional[ArrayLike]
+        Reward for the bandit. Only provided when the @contextual
+        decorator is used. Otherwise, this position should be None.
+    contextual : bool
+        Whether the bandit is contextual.
+    check_y : bool, default=True
+        Whether to check the `y` array.
+
+    Returns
+    -------
+    Tuple[NDArray, NDArray]
+        Validated `X` and `y` arrays.
+    """
+    if check_y:
+        should_not_be_none_if_contextual = y
+    else:
+        should_not_be_none_if_contextual = X
+
+    if contextual and should_not_be_none_if_contextual is None:
+        raise ValueError("Context must be provided for a contextual bandit.")
+    if not contextual and should_not_be_none_if_contextual is not None:
+        raise ValueError("Context must be None for a non-contextual bandit.")
+
+    if contextual:
+        X = np.atleast_2d(cast(ArrayLike, X))  # type: ignore
+        y = np.atleast_1d(cast(ArrayLike, y)) if check_y else None
+    else:
+        y = np.atleast_1d(cast(ArrayLike, X)) if check_y else None
+        X = (  # type: ignore
+            np.ones_like(y, dtype=float)[:, np.newaxis]
+            if check_y
+            else np.array([[1]], dtype=float)
+        )
+
+    return X, y
+
+
 def contextual(
     cls: Type[_B],
 ) -> Type[_B]:
     """Decorator for making a bandit contextual.
 
     This decorator adds methods to a Bandit subclass that allow it to be used
     in a contextual setting. The `pull` and `sample` methods will take `X`
```

### Comparing `bayesianbandits-0.4.0/bayesianbandits/_estimators.py` & `bayesianbandits-0.4.1/bayesianbandits/_estimators.py`

 * *Files identical despite different names*

### Comparing `bayesianbandits-0.4.0/bayesianbandits/_np_utils.py` & `bayesianbandits-0.4.1/bayesianbandits/_np_utils.py`

 * *Files identical despite different names*

### Comparing `bayesianbandits-0.4.0/bayesianbandits/_policy_decorators.py` & `bayesianbandits-0.4.1/bayesianbandits/_policy_decorators.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 from __future__ import annotations
 from functools import partial
-from typing import Callable, Optional, cast
+from typing import Callable, cast
 
 import numpy as np
-from numpy.typing import ArrayLike, NDArray
+from numpy.typing import NDArray
 
 from ._typing import ArmProtocol, BanditProtocol
 
 
 def epsilon_greedy(
     epsilon: float = 0.1,
     *,
     samples: int = 1000,
-) -> Callable[[BanditProtocol, Optional[ArrayLike]], ArmProtocol]:
+) -> Callable[[BanditProtocol, NDArray[np.float_]], ArmProtocol]:
     """Creates an epsilon-greedy choice algorithm. To be used with the
     `Bandit` class.
 
     Parameters
     ----------
     epsilon : float, default=0.1
         Probability of choosing a random arm.
     samples : int, default=1000
         Number of samples to use to compute the mean of the posterior.
 
     Returns
     -------
-    Callable[[BanditProtocol, Optional[ArrayLike]], ArmProtocol]
+    Callable[[BanditProtocol, NDArray[np.float_]], ArmProtocol]
         Closure that chooses an arm using epsilon-greedy.
     """
 
     def _choose_arm(
         self: BanditProtocol,
-        X: Optional[ArrayLike] = None,
+        X: NDArray[np.float_],
     ) -> ArmProtocol:
         """Choose an arm using epsilon-greedy."""
 
         if self.rng.random() < epsilon:  # type: ignore
             return self.rng.choice(list(self.arms.values()))  # type: ignore
         else:
             key_func = partial(_compute_arm_mean, X=X, samples=samples)
@@ -44,15 +44,15 @@
     return _choose_arm
 
 
 def upper_confidence_bound(
     alpha: float = 0.68,
     *,
     samples: int = 1000,
-) -> Callable[[BanditProtocol, Optional[ArrayLike]], ArmProtocol]:
+) -> Callable[[BanditProtocol, NDArray[np.float_]], ArmProtocol]:
     """Creates a UCB choice algorithm. To be used with the
     `Bandit` class.
 
     Actually uses the upper bound of the one-sided credible interval,
     which will deviate from the upper bound of the one-sided confidence
     interval depending on the strength of the prior.
 
@@ -63,15 +63,15 @@
     samples : int, default=1000
         Number of samples to use to compute the upper bound of the
         credible interval. The larger `alpha` is, the larger `samples`
         should be.
 
     Returns
     -------
-    Callable[[BanditProtocol, Optional[ArrayLike]], ArmProtocol]
+    Callable[[BanditProtocol, NDArray[np.float_]], ArmProtocol]
         Closure that chooses an arm using UCB.
 
     Notes
     -----
     A deeper analysis of this Bayesian UCB algorithm can be found in
     [1].
 
@@ -84,31 +84,31 @@
     """
 
     if not 0 < alpha < 1:
         raise ValueError("alpha must be in (0, 1).")
 
     def _choose_arm(
         self: BanditProtocol,
-        X: Optional[ArrayLike] = None,
+        X: NDArray[np.float_],
     ) -> ArmProtocol:
         """Choose an arm using UCB1."""
 
         key_func = partial(_compute_arm_upper_bound, X=X, alpha=alpha, samples=samples)
         return max(self.arms.values(), key=key_func)  # type: ignore
 
     return _choose_arm
 
 
-def thompson_sampling() -> Callable[[BanditProtocol, Optional[ArrayLike]], ArmProtocol]:
+def thompson_sampling() -> Callable[[BanditProtocol, NDArray[np.float_]], ArmProtocol]:
     """Creates a Thompson sampling choice algorithm. To be used with the
     `Bandit` class.
 
     Returns
     -------
-    Callable[[BanditProtocol, Optional[ArrayLike]], ArmProtocol]
+    Callable[[BanditProtocol, NDArray[np.float_]], ArmProtocol]
         Closure that chooses an arm using Thompson sampling.
 
     Notes
     -----
     This is a very simple implementation of Thompson sampling, identical
     to the one used in [1]. This generally works well in practice and
     has no hyperparameters to tune.
@@ -118,50 +118,47 @@
     [1] D. Russo, B. Van Row, A. Kazerouni, I. Osband, and Z. Wen, “A
         Tutorial on Thompson Sampling,” Foundations and Trends® in Machine
         Learning, vol. 11, no. 1, pp. 1-96, 2018.
     """
 
     def _choose_arm(
         self: BanditProtocol,
-        X: Optional[ArrayLike] = None,
+        X: NDArray[np.float_],
     ) -> ArmProtocol:
         """Choose an arm using Thompson sampling."""
 
         key_func = partial(_draw_one_sample, X=X)
         return max(self.arms.values(), key=key_func)  # type: ignore
 
     return _choose_arm
 
 
-def _draw_one_sample(
-    arm: ArmProtocol,
-    X: Optional[ArrayLike] = None,
-) -> np.float_:
+def _draw_one_sample(arm: ArmProtocol, X: NDArray[np.float_]) -> np.float_:
     """Draw one sample from the posterior distribution for the arm."""
     return arm.sample(X, size=1).item()  # type: ignore
 
 
 def _compute_arm_upper_bound(
     arm: ArmProtocol,
-    X: Optional[ArrayLike] = None,
+    X: NDArray[np.float_],
     *,
     alpha: float = 0.68,
     samples: int = 1000,
 ) -> np.float_:
     """Compute the upper bound of a one-sided credible interval with size
     `alpha` from the posterior distribution for the arm."""
     posterior_samples = arm.sample(X, size=samples)
     posterior_samples = cast(NDArray[np.float64], posterior_samples)
 
     return np.quantile(posterior_samples, q=alpha)  # type: ignore
 
 
 def _compute_arm_mean(
     arm: ArmProtocol,
-    X: Optional[ArrayLike] = None,
+    X: NDArray[np.float_],
     *,
     samples: int = 1000,
 ) -> np.float_:
     """Compute the mean of the posterior distribution for the arm."""
     posterior_samples = arm.sample(X, size=samples)
     posterior_samples = cast(NDArray[np.float64], posterior_samples)
```

### Comparing `bayesianbandits-0.4.0/bayesianbandits/_typing.py` & `bayesianbandits-0.4.1/bayesianbandits/_typing.py`

 * *Files 10% similar despite different names*

```diff
@@ -62,17 +62,15 @@
     """
 
     learner: Optional[Learner]
 
     def pull(self) -> ActionToken:
         ...
 
-    def sample(
-        self, X: Optional[ArrayLike] = None, size: int = 1
-    ) -> NDArray[np.float_]:
+    def sample(self, X: NDArray[np.float_], size: int = 1) -> NDArray[np.float_]:
         ...
 
     def update(self, X: NDArray[np.float_], y: NDArray[np.float_]) -> None:
         ...
 
     def decay(
         self,
```

### Comparing `bayesianbandits-0.4.0/pyproject.toml` & `bayesianbandits-0.4.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bayesianbandits"
-version = "0.4.0"
+version = "0.4.1"
 description = ""
 authors = ["Rishi Kulkarni <rishi@kulkarni.science>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9, <3.12"
 scipy = "^1.10.0"
```

### Comparing `bayesianbandits-0.4.0/PKG-INFO` & `bayesianbandits-0.4.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bayesianbandits
-Version: 0.4.0
+Version: 0.4.1
 Summary: 
 Author: Rishi Kulkarni
 Author-email: rishi@kulkarni.science
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

