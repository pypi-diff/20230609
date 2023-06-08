# Comparing `tmp/ostatslib-0.4.0.tar.gz` & `tmp/ostatslib-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ostatslib-0.4.0.tar", max compression
+gzip compressed data, was "ostatslib-0.5.0.tar", max compression
```

## Comparing `ostatslib-0.4.0.tar` & `ostatslib-0.5.0.tar`

### file list

```diff
@@ -1,56 +1,64 @@
--rw-r--r--   0        0        0     1109 2023-05-03 20:29:52.561631 ostatslib-0.4.0/LICENSE
--rw-r--r--   0        0        0      606 2023-05-03 20:29:52.561631 ostatslib-0.4.0/README.md
--rw-r--r--   0        0        0        0 2023-05-03 20:29:52.561631 ostatslib-0.4.0/ostatslib/__init__.py
--rw-r--r--   0        0        0      724 2023-05-03 20:29:52.561631 ostatslib-0.4.0/ostatslib/actions/__init__.py
--rw-r--r--   0        0        0      911 2023-05-03 20:29:52.561631 ostatslib-0.4.0/ostatslib/actions/action.py
--rw-r--r--   0        0        0     6398 2023-05-03 20:29:52.561631 ostatslib-0.4.0/ostatslib/actions/actions_space.py
--rw-r--r--   0        0        0      203 2023-05-03 20:29:52.561631 ostatslib-0.4.0/ostatslib/actions/classifiers/__init__.py
--rw-r--r--   0        0        0     2417 2023-05-03 20:29:52.561631 ostatslib-0.4.0/ostatslib/actions/classifiers/decision_tree.py
--rw-r--r--   0        0        0     2263 2023-05-03 20:29:52.561631 ostatslib-0.4.0/ostatslib/actions/classifiers/logistic_regression.py
--rw-r--r--   0        0        0     2359 2023-05-03 20:29:52.561631 ostatslib-0.4.0/ostatslib/actions/classifiers/support_vector_classification.py
--rw-r--r--   0        0        0       91 2023-05-03 20:29:52.561631 ostatslib-0.4.0/ostatslib/actions/clustering/__init__.py
--rw-r--r--   0        0        0     1616 2023-05-03 20:29:52.561631 ostatslib-0.4.0/ostatslib/actions/clustering/dbscan.py
--rw-r--r--   0        0        0     1702 2023-05-03 20:29:52.561631 ostatslib-0.4.0/ostatslib/actions/clustering/k_means.py
--rw-r--r--   0        0        0      527 2023-05-03 20:29:52.561631 ostatslib-0.4.0/ostatslib/actions/exploratory_actions/__init__.py
--rw-r--r--   0        0        0      455 2023-05-03 20:29:52.561631 ostatslib-0.4.0/ostatslib/actions/exploratory_actions/_get_exploratory_reward.py
--rw-r--r--   0        0        0     1563 2023-05-03 20:29:52.561631 ostatslib-0.4.0/ostatslib/actions/exploratory_actions/get_log_rows_count.py
--rw-r--r--   0        0        0     1764 2023-05-03 20:29:52.561631 ostatslib-0.4.0/ostatslib/actions/exploratory_actions/infer_response_dtype.py
--rw-r--r--   0        0        0     2283 2023-05-03 20:29:52.561631 ostatslib-0.4.0/ostatslib/actions/exploratory_actions/is_response_dichotomous_check.py
--rw-r--r--   0        0        0     1722 2023-05-03 20:29:52.561631 ostatslib-0.4.0/ostatslib/actions/exploratory_actions/is_response_discrete_check.py
--rw-r--r--   0        0        0     1763 2023-05-03 20:29:52.561631 ostatslib-0.4.0/ostatslib/actions/exploratory_actions/is_response_positive_values_only_check.py
--rw-r--r--   0        0        0     1478 2023-05-03 20:29:52.561631 ostatslib-0.4.0/ostatslib/actions/exploratory_actions/is_response_quantitative_check.py
--rw-r--r--   0        0        0     2872 2023-05-03 20:29:52.561631 ostatslib-0.4.0/ostatslib/actions/exploratory_actions/time_convertible_variable_search.py
--rw-r--r--   0        0        0      322 2023-05-03 20:29:52.561631 ostatslib-0.4.0/ostatslib/actions/regression_models/__init__.py
--rw-r--r--   0        0        0     2256 2023-05-03 20:29:52.561631 ostatslib-0.4.0/ostatslib/actions/regression_models/decision_tree_regression.py
--rw-r--r--   0        0        0     5741 2023-05-03 20:29:52.561631 ostatslib-0.4.0/ostatslib/actions/regression_models/linear_regression.py
--rw-r--r--   0        0        0     3222 2023-05-03 20:29:52.561631 ostatslib-0.4.0/ostatslib/actions/regression_models/poisson_regression.py
--rw-r--r--   0        0        0     2396 2023-05-03 20:29:52.561631 ostatslib-0.4.0/ostatslib/actions/regression_models/support_vector_regression.py
--rw-r--r--   0        0        0     4669 2023-05-03 20:29:52.561631 ostatslib-0.4.0/ostatslib/actions/regression_models/time_series_auto_arima.py
--rw-r--r--   0        0        0      453 2023-05-03 20:29:52.561631 ostatslib-0.4.0/ostatslib/actions/utils/__init__.py
--rw-r--r--   0        0        0      452 2023-05-03 20:29:52.561631 ostatslib-0.4.0/ostatslib/actions/utils/as_binary_array.py
--rw-r--r--   0        0        0      424 2023-05-03 20:29:52.561631 ostatslib-0.4.0/ostatslib/actions/utils/calculate_score_reward.py
--rw-r--r--   0        0        0     1837 2023-05-03 20:29:52.561631 ostatslib-0.4.0/ostatslib/actions/utils/explainability_rewards.py
--rw-r--r--   0        0        0      815 2023-05-03 20:29:52.561631 ostatslib-0.4.0/ostatslib/actions/utils/reward_cap.py
--rw-r--r--   0        0        0      841 2023-05-03 20:29:52.561631 ostatslib-0.4.0/ostatslib/actions/utils/split_response_from_explanatory_variables.py
--rw-r--r--   0        0        0      530 2023-05-03 20:29:52.561631 ostatslib-0.4.0/ostatslib/actions/utils/update_state_score.py
--rw-r--r--   0        0        0      124 2023-05-03 20:29:52.561631 ostatslib-0.4.0/ostatslib/agents/__init__.py
--rw-r--r--   0        0        0     2175 2023-05-03 20:29:52.561631 ostatslib-0.4.0/ostatslib/agents/agent.py
--rw-r--r--   0        0        0     1664 2023-05-03 20:29:52.561631 ostatslib-0.4.0/ostatslib/agents/analysis_result.py
--rw-r--r--   0        0        0     1913 2023-05-03 20:29:52.561631 ostatslib-0.4.0/ostatslib/agents/ppo_agent.py
--rw-r--r--   0        0        0       73 2023-05-03 20:29:52.561631 ostatslib-0.4.0/ostatslib/environments/__init__.py
--rw-r--r--   0        0        0     2630 2023-05-03 20:29:52.561631 ostatslib-0.4.0/ostatslib/environments/gym_environment.py
--rw-r--r--   0        0        0      101 2023-05-03 20:29:52.561631 ostatslib-0.4.0/ostatslib/environments/utils/__init__.py
--rw-r--r--   0        0        0     1106 2023-05-03 20:29:52.561631 ostatslib-0.4.0/ostatslib/environments/utils/_generate_from_datacooker.py
--rw-r--r--   0        0        0     3297 2023-05-03 20:29:52.561631 ostatslib-0.4.0/ostatslib/environments/utils/_generate_from_sklearn.py
--rw-r--r--   0        0        0      500 2023-05-03 20:29:52.561631 ostatslib-0.4.0/ostatslib/environments/utils/generate_training_dataset.py
--rw-r--r--   0        0        0       48 2023-05-03 20:29:52.561631 ostatslib-0.4.0/ostatslib/states/__init__.py
--rw-r--r--   0        0        0     1477 2023-05-03 20:29:52.561631 ostatslib-0.4.0/ostatslib/states/analysis_features_set.py
--rw-r--r--   0        0        0     2096 2023-05-03 20:29:52.561631 ostatslib-0.4.0/ostatslib/states/data_features_set.py
--rw-r--r--   0        0        0     1890 2023-05-03 20:29:52.565631 ostatslib-0.4.0/ostatslib/states/features_set.py
--rw-r--r--   0        0        0     1289 2023-05-03 20:29:52.565631 ostatslib-0.4.0/ostatslib/states/models_features_set.py
--rw-r--r--   0        0        0     5033 2023-05-03 20:29:52.565631 ostatslib-0.4.0/ostatslib/states/state.py
--rw-r--r--   0        0        0      604 2023-05-03 20:29:52.565631 ostatslib-0.4.0/ostatslib/states/state_iterator.py
--rw-r--r--   0        0        0       82 2023-05-03 20:29:52.565631 ostatslib-0.4.0/ostatslib/states/utils/__init__.py
--rw-r--r--   0        0        0      937 2023-05-03 20:29:52.565631 ostatslib-0.4.0/ostatslib/states/utils/init_features_set.py
--rw-r--r--   0        0        0     1002 2023-05-03 20:29:52.565631 ostatslib-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     1566 1970-01-01 00:00:00.000000 ostatslib-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1109 2023-06-08 22:51:08.653916 ostatslib-0.5.0/LICENSE
+-rw-r--r--   0        0        0      606 2023-06-08 22:51:08.653916 ostatslib-0.5.0/README.md
+-rw-r--r--   0        0        0        0 2023-06-08 22:51:08.653916 ostatslib-0.5.0/ostatslib/__init__.py
+-rw-r--r--   0        0        0      124 2023-06-08 22:51:08.653916 ostatslib-0.5.0/ostatslib/actions/__init__.py
+-rw-r--r--   0        0        0      910 2023-06-08 22:51:08.653916 ostatslib-0.5.0/ostatslib/actions/action.py
+-rw-r--r--   0        0        0     8118 2023-06-08 22:51:08.653916 ostatslib-0.5.0/ostatslib/actions/actions_space.py
+-rw-r--r--   0        0        0      331 2023-06-08 22:51:08.653916 ostatslib-0.5.0/ostatslib/actions/classifiers/__init__.py
+-rw-r--r--   0        0        0     2524 2023-06-08 22:51:08.653916 ostatslib-0.5.0/ostatslib/actions/classifiers/decision_tree.py
+-rw-r--r--   0        0        0     2750 2023-06-08 22:51:08.653916 ostatslib-0.5.0/ostatslib/actions/classifiers/linear_support_vector_classification.py
+-rw-r--r--   0        0        0     2371 2023-06-08 22:51:08.653916 ostatslib-0.5.0/ostatslib/actions/classifiers/logistic_regression.py
+-rw-r--r--   0        0        0     2696 2023-06-08 22:51:08.653916 ostatslib-0.5.0/ostatslib/actions/classifiers/random_forest.py
+-rw-r--r--   0        0        0     2623 2023-06-08 22:51:08.653916 ostatslib-0.5.0/ostatslib/actions/classifiers/support_vector_classification.py
+-rw-r--r--   0        0        0       91 2023-06-08 22:51:08.653916 ostatslib-0.5.0/ostatslib/actions/clustering/__init__.py
+-rw-r--r--   0        0        0     2364 2023-06-08 22:51:08.653916 ostatslib-0.5.0/ostatslib/actions/clustering/dbscan.py
+-rw-r--r--   0        0        0     1440 2023-06-08 22:51:08.653916 ostatslib-0.5.0/ostatslib/actions/clustering/k_means.py
+-rw-r--r--   0        0        0      606 2023-06-08 22:51:08.653916 ostatslib-0.5.0/ostatslib/actions/exploratory_actions/__init__.py
+-rw-r--r--   0        0        0      546 2023-06-08 22:51:08.653916 ostatslib-0.5.0/ostatslib/actions/exploratory_actions/_get_exploratory_reward.py
+-rw-r--r--   0        0        0     1688 2023-06-08 22:51:08.653916 ostatslib-0.5.0/ostatslib/actions/exploratory_actions/get_log_rows_count.py
+-rw-r--r--   0        0        0     2087 2023-06-08 22:51:08.653916 ostatslib-0.5.0/ostatslib/actions/exploratory_actions/get_response_unique_values_ratio.py
+-rw-r--r--   0        0        0     1721 2023-06-08 22:51:08.653916 ostatslib-0.5.0/ostatslib/actions/exploratory_actions/infer_response_dtype.py
+-rw-r--r--   0        0        0     2461 2023-06-08 22:51:08.653916 ostatslib-0.5.0/ostatslib/actions/exploratory_actions/is_response_dichotomous_check.py
+-rw-r--r--   0        0        0     1900 2023-06-08 22:51:08.653916 ostatslib-0.5.0/ostatslib/actions/exploratory_actions/is_response_discrete_check.py
+-rw-r--r--   0        0        0     1942 2023-06-08 22:51:08.653916 ostatslib-0.5.0/ostatslib/actions/exploratory_actions/is_response_positive_values_only_check.py
+-rw-r--r--   0        0        0     1657 2023-06-08 22:51:08.653916 ostatslib-0.5.0/ostatslib/actions/exploratory_actions/is_response_quantitative_check.py
+-rw-r--r--   0        0        0     3070 2023-06-08 22:51:08.653916 ostatslib-0.5.0/ostatslib/actions/exploratory_actions/time_convertible_variable_search.py
+-rw-r--r--   0        0        0      464 2023-06-08 22:51:08.657916 ostatslib-0.5.0/ostatslib/actions/regression_models/__init__.py
+-rw-r--r--   0        0        0     2735 2023-06-08 22:51:08.657916 ostatslib-0.5.0/ostatslib/actions/regression_models/decision_tree_regression.py
+-rw-r--r--   0        0        0     5919 2023-06-08 22:51:08.657916 ostatslib-0.5.0/ostatslib/actions/regression_models/linear_regression.py
+-rw-r--r--   0        0        0     2729 2023-06-08 22:51:08.657916 ostatslib-0.5.0/ostatslib/actions/regression_models/linear_support_vector_regression.py
+-rw-r--r--   0        0        0     3097 2023-06-08 22:51:08.657916 ostatslib-0.5.0/ostatslib/actions/regression_models/poisson_regression.py
+-rw-r--r--   0        0        0     2823 2023-06-08 22:51:08.657916 ostatslib-0.5.0/ostatslib/actions/regression_models/random_forest_regression.py
+-rw-r--r--   0        0        0     2562 2023-06-08 22:51:08.657916 ostatslib-0.5.0/ostatslib/actions/regression_models/support_vector_regression.py
+-rw-r--r--   0        0        0     5072 2023-06-08 22:51:08.657916 ostatslib-0.5.0/ostatslib/actions/regression_models/time_series_auto_arima.py
+-rw-r--r--   0        0        0      456 2023-06-08 22:51:08.657916 ostatslib-0.5.0/ostatslib/actions/utils/__init__.py
+-rw-r--r--   0        0        0      458 2023-06-08 22:51:08.657916 ostatslib-0.5.0/ostatslib/actions/utils/calculate_score_reward.py
+-rw-r--r--   0        0        0     1783 2023-06-08 22:51:08.657916 ostatslib-0.5.0/ostatslib/actions/utils/explainability_rewards.py
+-rw-r--r--   0        0        0     1224 2023-06-08 22:51:08.657916 ostatslib-0.5.0/ostatslib/actions/utils/model_selection.py
+-rw-r--r--   0        0        0      727 2023-06-08 22:51:08.657916 ostatslib-0.5.0/ostatslib/actions/utils/reward_cap.py
+-rw-r--r--   0        0        0      841 2023-06-08 22:51:08.657916 ostatslib-0.5.0/ostatslib/actions/utils/split_response_from_explanatory_variables.py
+-rw-r--r--   0        0        0      473 2023-06-08 22:51:08.657916 ostatslib-0.5.0/ostatslib/actions/utils/update_state_score.py
+-rw-r--r--   0        0        0     1972 2023-06-08 22:51:08.657916 ostatslib-0.5.0/ostatslib/actions/utils/validate_state.py
+-rw-r--r--   0        0        0      124 2023-06-08 22:51:08.657916 ostatslib-0.5.0/ostatslib/agents/__init__.py
+-rw-r--r--   0        0        0     2177 2023-06-08 22:51:08.657916 ostatslib-0.5.0/ostatslib/agents/agent.py
+-rw-r--r--   0        0        0     2195 2023-06-08 22:51:08.657916 ostatslib-0.5.0/ostatslib/agents/analysis_result.py
+-rw-r--r--   0        0        0     1927 2023-06-08 22:51:08.657916 ostatslib-0.5.0/ostatslib/agents/ppo_agent.py
+-rw-r--r--   0        0        0      385 2023-06-08 22:51:08.657916 ostatslib-0.5.0/ostatslib/config.py
+-rw-r--r--   0        0        0       73 2023-06-08 22:51:08.657916 ostatslib-0.5.0/ostatslib/environments/__init__.py
+-rw-r--r--   0        0        0     2708 2023-06-08 22:51:08.657916 ostatslib-0.5.0/ostatslib/environments/gym_environment.py
+-rw-r--r--   0        0        0      101 2023-06-08 22:51:08.657916 ostatslib-0.5.0/ostatslib/environments/utils/__init__.py
+-rw-r--r--   0        0        0     1106 2023-06-08 22:51:08.657916 ostatslib-0.5.0/ostatslib/environments/utils/_generate_from_datacooker.py
+-rw-r--r--   0        0        0     1475 2023-06-08 22:51:08.657916 ostatslib-0.5.0/ostatslib/environments/utils/_generate_from_pmlb.py
+-rw-r--r--   0        0        0     3639 2023-06-08 22:51:08.657916 ostatslib-0.5.0/ostatslib/environments/utils/_generate_from_sklearn.py
+-rw-r--r--   0        0        0      602 2023-06-08 22:51:08.657916 ostatslib-0.5.0/ostatslib/environments/utils/generate_training_dataset.py
+-rw-r--r--   0        0        0       48 2023-06-08 22:51:08.657916 ostatslib-0.5.0/ostatslib/states/__init__.py
+-rw-r--r--   0        0        0     1477 2023-06-08 22:51:08.657916 ostatslib-0.5.0/ostatslib/states/analysis_features_set.py
+-rw-r--r--   0        0        0     2264 2023-06-08 22:51:08.657916 ostatslib-0.5.0/ostatslib/states/data_features_set.py
+-rw-r--r--   0        0        0     1876 2023-06-08 22:51:08.657916 ostatslib-0.5.0/ostatslib/states/features_set.py
+-rw-r--r--   0        0        0     3401 2023-06-08 22:51:08.657916 ostatslib-0.5.0/ostatslib/states/models_features_set.py
+-rw-r--r--   0        0        0     5033 2023-06-08 22:51:08.657916 ostatslib-0.5.0/ostatslib/states/state.py
+-rw-r--r--   0        0        0      604 2023-06-08 22:51:08.657916 ostatslib-0.5.0/ostatslib/states/state_iterator.py
+-rw-r--r--   0        0        0       82 2023-06-08 22:51:08.657916 ostatslib-0.5.0/ostatslib/states/utils/__init__.py
+-rw-r--r--   0        0        0      937 2023-06-08 22:51:08.657916 ostatslib-0.5.0/ostatslib/states/utils/init_features_set.py
+-rw-r--r--   0        0        0     1061 2023-06-08 22:51:08.657916 ostatslib-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1655 1970-01-01 00:00:00.000000 ostatslib-0.5.0/PKG-INFO
```

### Comparing `ostatslib-0.4.0/LICENSE` & `ostatslib-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ostatslib-0.4.0/README.md` & `ostatslib-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `ostatslib-0.4.0/ostatslib/actions/action.py` & `ostatslib-0.5.0/ostatslib/actions/action.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,20 +6,20 @@
 
 from pandas import DataFrame
 from sklearn.base import BaseEstimator
 from statsmodels.base.model import LikelihoodModelResults, Results
 from statsmodels.tsa.base.tsa_model import TimeSeriesModelResults
 from ostatslib.states import State
 
-TModel = TypeVar('TModel',
+TModel = TypeVar('TModel', # pylint: disable=invalid-name
                  None,
                  BaseEstimator,
                  LikelihoodModelResults,
                  Results,
-                 TimeSeriesModelResults)  # pylint: disable=invalid-name
+                 TimeSeriesModelResults)
 
 
 class ActionInfo(TypedDict, Generic[TModel], total=False):
     """
     Action results information
     """
     action_name: str
```

### Comparing `ostatslib-0.4.0/ostatslib/actions/actions_space.py` & `ostatslib-0.5.0/ostatslib/actions/actions_space.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,106 +4,141 @@
 
 from functools import cached_property
 from gymnasium.spaces import MultiBinary
 
 import numpy as np
 import numpy.typing as npt
 from pandas import DataFrame
+from ostatslib import config
 
-from ostatslib.actions.exploratory_actions import (
+from ostatslib.states import State
+
+from .exploratory_actions import (
     get_log_rows_count,
     infer_response_dtype,
     is_response_dichotomous_check,
     is_response_discrete_check,
     is_response_positive_values_only_check,
     is_response_quantitative_check,
-    time_convertible_variable_search
+    time_convertible_variable_search,
+    get_response_unique_values_ratio
 )
-from ostatslib.actions.regression_models import (
+from .regression_models import (
     linear_regression,
     poisson_regression,
     support_vector_regression,
     decision_tree_regression,
-    time_series_auto_arima
+    time_series_auto_arima,
+    linear_support_vector_regression,
+    random_forest_regression
 )
-from ostatslib.actions.classifiers import (
+from .classifiers import (
     logistic_regression,
     support_vector_classification,
-    decision_tree
+    decision_tree,
+    linear_support_vector_classification,
+    random_forest
 )
-from ostatslib.actions.clustering import (
+from .clustering import (
     k_means,
     dbscan
 )
-from ostatslib.actions.utils import as_binary_array
-from ostatslib.states import State
+
 from .action import Action, ActionInfo, ActionResult
 
 
+def _as_binary_array(number: int, array_length: int) -> np.ndarray:
+    """
+    Converts an integer to a np.array of binary digits
+
+    Args:
+        number (int): integer number to be converted
+
+    Returns:
+        array: numpy array of converted digits
+    """
+    binary_str = bin(number)[2:].zfill(array_length)
+
+    return np.array([int(digit) for digit in binary_str])
+
+
 MaskNDArray = npt.NDArray[np.int8]
 ENCODING_LENGTH = 5
 
 # Encoding: 0 to 7
 EXPLORATORY_ACTIONS = {
     'get_log_rows_count': (get_log_rows_count,
-                           as_binary_array(0, ENCODING_LENGTH)),
+                           _as_binary_array(0, ENCODING_LENGTH)),
     'is_response_dichotomous_check': (is_response_dichotomous_check,
-                                      as_binary_array(1, ENCODING_LENGTH)),
+                                      _as_binary_array(1, ENCODING_LENGTH)),
     'is_response_discrete_check': (is_response_discrete_check,
-                                   as_binary_array(2, ENCODING_LENGTH)),
+                                   _as_binary_array(2, ENCODING_LENGTH)),
     'is_response_positive_values_only_check': (is_response_positive_values_only_check,
-                                               as_binary_array(3, ENCODING_LENGTH)),
+                                               _as_binary_array(3, ENCODING_LENGTH)),
     'is_response_quantitative_check': (is_response_quantitative_check,
-                                       as_binary_array(4, ENCODING_LENGTH)),
+                                       _as_binary_array(4, ENCODING_LENGTH)),
     'time_convertible_variable_search': (time_convertible_variable_search,
-                                         as_binary_array(5, ENCODING_LENGTH)),
+                                         _as_binary_array(5, ENCODING_LENGTH)),
     'infer_response_dtype': (infer_response_dtype,
-                             as_binary_array(6, ENCODING_LENGTH))
+                             _as_binary_array(6, ENCODING_LENGTH)),
+    'get_response_unique_values_ratio': (get_response_unique_values_ratio,
+                                         _as_binary_array(7, ENCODING_LENGTH))
 }
 
 # Encoding: 8 to 15
 CLASSIFIERS = {
     'logistic_regression': (logistic_regression,
-                            as_binary_array(8, ENCODING_LENGTH)),
+                            _as_binary_array(8, ENCODING_LENGTH)),
     'support_vector_classification': (support_vector_classification,
-                                      as_binary_array(9, ENCODING_LENGTH)),
+                                      _as_binary_array(9, ENCODING_LENGTH)),
+    'linear_support_vector_classification': (linear_support_vector_classification,
+                                             _as_binary_array(10, ENCODING_LENGTH)),
     'decision_tree': (decision_tree,
-                      as_binary_array(10, ENCODING_LENGTH))
+                      _as_binary_array(11, ENCODING_LENGTH)),
+    'random_forest': (random_forest,
+                      _as_binary_array(12, ENCODING_LENGTH)),
 }
 
 # Encoding: 16 to 23
 REGRESSION_MODELS = {
     'linear_regression': (linear_regression,
-                          as_binary_array(16, ENCODING_LENGTH)),
+                          _as_binary_array(16, ENCODING_LENGTH)),
     'poisson_regression': (poisson_regression,
-                           as_binary_array(17, ENCODING_LENGTH)),
+                           _as_binary_array(17, ENCODING_LENGTH)),
     'support_vector_regression': (support_vector_regression,
-                                  as_binary_array(18, ENCODING_LENGTH)),
+                                  _as_binary_array(18, ENCODING_LENGTH)),
+    'linear_support_vector_regression': (linear_support_vector_regression,
+                                         _as_binary_array(19, ENCODING_LENGTH)),
     'decision_tree_regression': (decision_tree_regression,
-                                 as_binary_array(19, ENCODING_LENGTH)),
+                                 _as_binary_array(20, ENCODING_LENGTH)),
+    'random_forest_regression': (random_forest_regression,
+                                 _as_binary_array(21, ENCODING_LENGTH)),
     'time_series_auto_arima': (time_series_auto_arima,
-                               as_binary_array(20, ENCODING_LENGTH))
+                               _as_binary_array(22, ENCODING_LENGTH))
 }
 
 # Encoding: 24 to 31
 CLUSTERING = {
     'k_means': (k_means,
-                as_binary_array(24, ENCODING_LENGTH)),
+                _as_binary_array(24, ENCODING_LENGTH)),
     'dbscan': (dbscan,
-               as_binary_array(25, ENCODING_LENGTH))
+               _as_binary_array(25, ENCODING_LENGTH))
 }
 
 
 def _invalid_action_step(state: State, data: DataFrame) -> ActionResult[None]:
-    reward = float(-1)
-    info = ActionInfo(action_name='Invalid Action',
-                      action_fn=_invalid_action_step,
-                      model=None,
-                      raised_exception=False)
-    return state, reward, info
+    if state and data is not None:
+        reward = config.MIN_REWARD
+        info = ActionInfo(action_name='Invalid Action',
+                          action_fn=_invalid_action_step,
+                          model=None,
+                          raised_exception=False)
+        return state, reward, info
+
+    raise ValueError("State and Data must be valid.")
 
 
 class ActionsSpace(MultiBinary):
     """
     Actions space
     """
 
@@ -165,14 +200,29 @@
             action_name (str): action name
 
         Returns:
             ActionFunction[T]: action function
         """
         return self.__actions[action_name][0]
 
+    def get_action_name_by_code(self, action_code: np.ndarray | list) -> str | None:
+        """Gets action name by code
+
+        Args:
+            action_code (np.ndarray): action code
+
+        Returns:
+            str: action name
+        """
+        for action_name, (_, code) in self.__actions.items():
+            if np.array_equal(code, action_code):
+                return action_name
+
+        return None
+
     def is_valid_action_by_encoding(self, action_code: np.ndarray) -> bool:
         """Check if action code is valid
 
         Args:
             action_code (np.array): action code
 
         Returns:
```

### Comparing `ostatslib-0.4.0/ostatslib/actions/classifiers/decision_tree.py` & `ostatslib-0.5.0/ostatslib/actions/classifiers/decision_tree.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,68 +1,66 @@
 """
 Decision Tree module
 """
 
-from numpy import ndarray
+import operator
 from pandas import DataFrame
-from sklearn.model_selection import cross_val_score
 from sklearn.tree import DecisionTreeClassifier
-from ostatslib.actions import Action, ActionInfo, ActionResult
-from ostatslib.actions.utils import (calculate_score_reward,
-                                     reward_cap,
-                                     comprehensible_model,
-                                     split_response_from_explanatory_variables,
-                                     update_state_score)
+from ostatslib import config
 from ostatslib.states import State
 
+from ..action import Action, ActionInfo, ActionResult
+from ..utils import (calculate_score_reward,
+                     reward_cap,
+                     comprehensible_model,
+                     split_response_from_explanatory_variables,
+                     update_state_score,
+                     validate_state,
+                     model_selection)
+
 _ACTION_NAME = "Decision Tree"
+_VALIDATIONS = [('response_variable_label', operator.truth, None),
+                ('is_response_discrete', operator.gt, 0),
+                ('decision_tree_score_reward', operator.eq, 0)]
 
 
+@validate_state(action_name=_ACTION_NAME, validator_fns=_VALIDATIONS)
 @reward_cap
 @comprehensible_model
 def _decision_tree(state: State, data: DataFrame) -> ActionResult[DecisionTreeClassifier]:
     """
     Fits data to a decision tree classifier
 
     Args:
         state (State): current environment state
         data (DataFrame): data under analysis
 
     Returns:
         ActionResult[DecisionTreeClassifier]: action result
     """
-    if not __is_valid_state(state):
-        return state, -1, ActionInfo(action_name=_ACTION_NAME,
-                                     action_fn=_decision_tree,
-                                     model=None,
-                                     raised_exception=False)
-
     y_values, x_values = split_response_from_explanatory_variables(state, data)
-    classifier = DecisionTreeClassifier()
+    classifier: DecisionTreeClassifier = DecisionTreeClassifier()
+    param_grid = {'criterion': ['gini', 'entropy', 'log_loss'],
+                  'max_features': ['sqrt', 'log2', None]}
 
     try:
-        scores: ndarray = cross_val_score(classifier, x_values, y_values, cv=5)
+        classifier, score = model_selection(classifier,
+                                            param_grid,
+                                            x_values,
+                                            y_values)
     except ValueError:
-        return state, -1, ActionInfo(action_name=_ACTION_NAME,
-                                     action_fn=_decision_tree,
-                                     model=None,
-                                     raised_exception=True)
+        state.set('decision_tree_score_reward', config.MIN_REWARD)
+        return state, config.MIN_REWARD, ActionInfo(action_name=_ACTION_NAME,
+                                                    action_fn=_decision_tree,
+                                                    model=None,
+                                                    raised_exception=True)
 
-    score: float = scores.mean() - scores.std()
-    reward: float = calculate_score_reward(score)
     update_state_score(state, score)
-    model = classifier.fit(X=x_values, y=y_values)
+    reward = calculate_score_reward(score)
+    state.set('decision_tree_score_reward', reward)
     return state, reward, ActionInfo(action_name=_ACTION_NAME,
                                      action_fn=_decision_tree,
-                                     model=model,
+                                     model=classifier,
                                      raised_exception=False)
 
 
-def __is_valid_state(state: State) -> bool:
-    if state.get("is_response_quantitative") > 0 or\
-            not bool(state.get("response_variable_label")):
-        return False
-
-    return True
-
-
 decision_tree: Action[DecisionTreeClassifier] = _decision_tree
```

### Comparing `ostatslib-0.4.0/ostatslib/actions/classifiers/logistic_regression.py` & `ostatslib-0.5.0/ostatslib/actions/classifiers/logistic_regression.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,63 +1,62 @@
 """
 Logistic regression module
 """
 
+import operator
 from pandas import DataFrame
 from sklearn.linear_model import LogisticRegressionCV
-from ostatslib.actions import Action, ActionInfo, ActionResult
-from ostatslib.actions.utils import (calculate_score_reward,
-                                     reward_cap,
-                                     interpretable_model,
-                                     split_response_from_explanatory_variables,
-                                     update_state_score)
+from ostatslib import config
 from ostatslib.states import State
 
+from ..action import Action, ActionInfo, ActionResult
+from ..utils import (calculate_score_reward,
+                     reward_cap,
+                     interpretable_model,
+                     split_response_from_explanatory_variables,
+                     update_state_score,
+                     validate_state)
+
 _ACTION_NAME = "Logistic Regression"
+_VALIDATIONS = [('response_variable_label', operator.truth, None),
+                ('is_response_dichotomous', operator.gt, 0),
+                ('response_variable_label', operator.truth, None),
+                ('logistic_regression_score_reward', operator.eq, 0)]
 
 
+@validate_state(action_name=_ACTION_NAME, validator_fns=_VALIDATIONS)
 @reward_cap
 @interpretable_model
 def _logistic_regression(state: State, data: DataFrame) -> ActionResult[LogisticRegressionCV]:
     """
     Fits data to a logistic regression model.
 
     Args:
         state (State): current environment state
         data (DataFrame): data under analysis
 
     Returns:
         ActionResult[LogisticRegressionCV]: action result
     """
-    if not __is_valid_state(state):
-        return state, -1, ActionInfo(action_name=_ACTION_NAME,
-                                     action_fn=_logistic_regression,
-                                     model=None,
-                                     raised_exception=False)
-
     y_values, x_values = split_response_from_explanatory_variables(state, data)
     regression = LogisticRegressionCV(cv=5)
 
     try:
         regression = regression.fit(x_values, y_values)
     except ValueError:
-        return state, -1, ActionInfo(action_name=_ACTION_NAME,
-                                     action_fn=_logistic_regression,
-                                     model=None,
-                                     raised_exception=True)
+        state.set('logistic_regression_score_reward', config.MIN_REWARD)
+        return state, config.MIN_REWARD, ActionInfo(action_name=_ACTION_NAME,
+                                                    action_fn=_logistic_regression,
+                                                    model=None,
+                                                    raised_exception=True)
 
     score: float = regression.score(x_values, y_values)
-    reward: float = calculate_score_reward(score)
     update_state_score(state, score)
+    reward: float = calculate_score_reward(score)
+    state.set('logistic_regression_score_reward', reward)
     return state, reward, ActionInfo(action_name=_ACTION_NAME,
                                      action_fn=_logistic_regression,
                                      model=regression,
                                      raised_exception=False)
 
-def __is_valid_state(state: State) -> bool:
-    if state.get("is_response_dichotomous") <= 0:
-        return False
-
-    return True
-
 
 logistic_regression: Action[LogisticRegressionCV] = _logistic_regression
```

### Comparing `ostatslib-0.4.0/ostatslib/actions/classifiers/support_vector_classification.py` & `ostatslib-0.5.0/ostatslib/actions/classifiers/linear_support_vector_classification.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,66 +1,69 @@
 """
-Support Vector Classification module
+Linear Support Vector Classification module
 """
 
-from numpy import ndarray
+import operator
 from pandas import DataFrame
-from sklearn.model_selection import cross_val_score
-from sklearn.svm import SVC
-from ostatslib.actions import Action, ActionInfo, ActionResult
-from ostatslib.actions.utils import (calculate_score_reward,
-                                     reward_cap,
-                                     opaque_model,
-                                     split_response_from_explanatory_variables,
-                                     update_state_score)
+from sklearn.svm import LinearSVC
+from ostatslib import config
 from ostatslib.states import State
 
-_ACTION_NAME = "Support Vector Classification"
+from ..action import Action, ActionInfo, ActionResult
+from ..utils import (calculate_score_reward,
+                     reward_cap,
+                     opaque_model,
+                     split_response_from_explanatory_variables,
+                     update_state_score,
+                     validate_state,
+                     model_selection)
+
+_ACTION_NAME = "Linear Support Vector Classification"
+_VALIDATIONS = [('response_variable_label', operator.truth, None),
+                ('is_response_discrete', operator.gt, 0),
+                ('log_rows_count', operator.gt, 0),
+                ('log_rows_count', operator.lt, 0.81),
+                ('linear_support_vector_classification_score_reward', operator.eq, 0)]
 
 
+@validate_state(action_name=_ACTION_NAME, validator_fns=_VALIDATIONS)
 @reward_cap
 @opaque_model
-def _support_vector_classification(state: State, data: DataFrame) -> ActionResult[SVC]:
+def _linear_support_vector_classification(state: State, data: DataFrame) -> ActionResult[LinearSVC]:
     """
-    Fits data to a SVC model
+    Fits data to a LinearSVC model
 
     Args:
         state (State): current environment state
         data (DataFrame): data under analysis
 
     Returns:
-        ActionResult[SVC]: action result
+        ActionResult[LinearSVC]: action result
     """
-    if not __is_valid_state(state):
-        return state, -1, ActionInfo(action_name=_ACTION_NAME,
-                                     action_fn=_support_vector_classification,
-                                     model=None,
-                                     raised_exception=False)
-
     y_values, x_values = split_response_from_explanatory_variables(state, data)
-    classifier = SVC()
+    classifier: LinearSVC = LinearSVC()
+    param_grid = {'penalty': ['l1', 'l2'],
+                  'loss': ['squared_hinge', 'hinge']}
 
     try:
-        scores: ndarray = cross_val_score(classifier, x_values, y_values, cv=5)
+        classifier, score = model_selection(classifier,
+                                            param_grid,
+                                            x_values,
+                                            y_values)
     except ValueError:
-        return state, -1, ActionInfo(action_name=_ACTION_NAME,
-                                     action_fn=_support_vector_classification,
-                                     model=None,
-                                     raised_exception=True)
+        state.set('linear_support_vector_classification_score_reward',
+                  config.MIN_REWARD)
+        return state, config.MIN_REWARD, ActionInfo(action_name=_ACTION_NAME,
+                                                    action_fn=_linear_support_vector_classification,
+                                                    model=None,
+                                                    raised_exception=True)
 
-    score: float = scores.mean() - scores.std()
-    reward: float = calculate_score_reward(score)
     update_state_score(state, score)
+    reward = calculate_score_reward(score)
+    state.set('linear_support_vector_classification_score_reward', reward)
     return state, reward, ActionInfo(action_name=_ACTION_NAME,
-                                     action_fn=_support_vector_classification,
+                                     action_fn=_linear_support_vector_classification,
                                      model=classifier,
                                      raised_exception=False)
 
 
-def __is_valid_state(state: State) -> bool:
-    if state.get("is_response_quantitative") > 0 or not bool(state.get("response_variable_label")):
-        return False
-
-    return True
-
-
-support_vector_classification: Action[SVC] = _support_vector_classification
+linear_support_vector_classification: Action[LinearSVC] = _linear_support_vector_classification
```

### Comparing `ostatslib-0.4.0/ostatslib/actions/clustering/k_means.py` & `ostatslib-0.5.0/ostatslib/actions/clustering/k_means.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,56 +1,49 @@
 """
 K-Means module
 """
 
+import operator
 from pandas import DataFrame
 from sklearn.cluster import KMeans
 from sklearn.metrics import silhouette_score
-from ostatslib.actions import Action, ActionInfo, ActionResult
-from ostatslib.actions.utils import (calculate_score_reward,
-                                     reward_cap,
-                                     update_state_score)
+
 from ostatslib.states import State
+from ..action import Action, ActionInfo, ActionResult
+from ..utils import (calculate_score_reward,
+                     reward_cap,
+                     update_state_score,
+                     validate_state)
 
 _ACTION_NAME = "K-Means"
+_VALIDATIONS = [('response_variable_label', operator.eq, ''),
+                ('clusters_count', operator.gt, 0)]
 
 
+@validate_state(action_name=_ACTION_NAME, validator_fns=_VALIDATIONS)
 @reward_cap
 def _k_means(state: State, data: DataFrame) -> ActionResult[KMeans]:
     """
     Fits data to a KMeans cluster
 
     Args:
         state (State): current environment state
         data (DataFrame): data under analysis
 
     Returns:
         ActionResult[KMeans]: action result
     """
-    if not __is_valid_state(state):
-        return state, -1, ActionInfo(action_name=_ACTION_NAME,
-                                     action_fn=_k_means,
-                                     model=None,
-                                     raised_exception=False)
-
     clusters_count: int = state.get("clusters_count")
     kmeans = KMeans(n_clusters=clusters_count)
     kmeans.fit(data)
 
     score: float = silhouette_score(data, kmeans.labels_)
 
     reward: float = calculate_score_reward(score)
     update_state_score(state, score)
     return state, reward, ActionInfo(action_name=_ACTION_NAME,
                                      action_fn=_k_means,
                                      model=kmeans,
                                      raised_exception=False)
 
 
-def __is_valid_state(state: State) -> bool:
-    if not bool(state.get("clusters_count")) or bool(state.get("response_variable_label")):
-        return False
-
-    return True
-
-
 k_means: Action[KMeans] = _k_means
```

### Comparing `ostatslib-0.4.0/ostatslib/actions/exploratory_actions/__init__.py` & `ostatslib-0.5.0/ostatslib/actions/exploratory_actions/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,7 +5,8 @@
 from .get_log_rows_count import get_log_rows_count
 from .infer_response_dtype import infer_response_dtype
 from .is_response_dichotomous_check import is_response_dichotomous_check
 from .is_response_discrete_check import is_response_discrete_check
 from .is_response_positive_values_only_check import is_response_positive_values_only_check
 from .is_response_quantitative_check import is_response_quantitative_check
 from .time_convertible_variable_search import time_convertible_variable_search
+from .get_response_unique_values_ratio import get_response_unique_values_ratio
```

### Comparing `ostatslib-0.4.0/ostatslib/actions/exploratory_actions/get_log_rows_count.py` & `ostatslib-0.5.0/ostatslib/actions/exploratory_actions/get_log_rows_count.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 """
 get_log_rows_count module
 """
 
 import numpy as np
 from pandas import DataFrame
-from ostatslib.actions import Action, ActionInfo, ActionResult
+from ostatslib import config
 from ostatslib.states import State
 
+from ..action import Action, ActionInfo, ActionResult
+
 _ACTION_NAME = "Get Log Rows Count"
 
 
 ROW_COUNT_UPPER_LIMIT = 150000
-LOG_COMPRESSION_CONSTANT = 12
+LOG_COMPRESSION_CONSTANT = 5.176
+"""compression rate to keep log10(150K lines) close to 1"""
 
 
 def _get_log_rows_count(state: State,
                         data: DataFrame) -> ActionResult[None]:
     """
     Gets log rows count: log(#rows)/c, where c is a compression constant
 
@@ -42,17 +45,17 @@
         return 1
 
     return np.log10(rows_count)/LOG_COMPRESSION_CONSTANT
 
 
 def __calculate_reward(state: State, log_rows_count: float) -> float:
     if state.get("log_rows_count") == log_rows_count:
-        return -1
+        return config.MIN_REWARD
 
-    return 0.5
+    return config.MAX_EXPLORATORY_REWARD
 
 
 def __update_state(state: State, log_rows_count: float) -> State:
     state.set("log_rows_count", log_rows_count)
     return state
```

### Comparing `ostatslib-0.4.0/ostatslib/actions/exploratory_actions/infer_response_dtype.py` & `ostatslib-0.5.0/ostatslib/actions/exploratory_actions/infer_response_dtype.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,48 +1,47 @@
 """
 infer_response_dtype module
 """
 
+import operator
 from pandas import DataFrame, Series
 from pandas.api.types import infer_dtype
+from ostatslib import config
 
-from ostatslib.actions import Action, ActionInfo, ActionResult
 from ostatslib.states import State
 from ._get_exploratory_reward import get_exploratory_reward
+from ..action import Action, ActionInfo, ActionResult
+from ..utils import validate_state
 
 _ACTION_NAME = "Infer Response DType"
+_VALIDATIONS = [('response_variable_label', operator.truth, None)]
 
 
+@validate_state(action_name=_ACTION_NAME, validator_fns=_VALIDATIONS)
 def _infer_response_dtype(state: State, data: DataFrame) -> ActionResult[None]:
     """
     Infer response dtype
 
     Args:
         state (State): state
         data (DataFrame): data
 
     Returns:
         ActionResult[None]: action result
     """
     state_copy: State = state.copy()
     response_var_label: str = state.get("response_variable_label")
 
-    if not bool(response_var_label) or response_var_label is None:
-        return state, -1, ActionInfo(action_name=_ACTION_NAME,
-                                     action_fn=_infer_response_dtype,
-                                     model=None,
-                                     raised_exception=False)
-
     try:
         response: Series = data[response_var_label]
     except KeyError:
-        return state, -1, ActionInfo(action_name=_ACTION_NAME,
-                                     action_fn=_infer_response_dtype,
-                                     model=None,
-                                     raised_exception=True)
+        return state, config.MIN_REWARD, ActionInfo(action_name=_ACTION_NAME,
+                                                    action_fn=_infer_response_dtype,
+                                                    model=None,
+                                                    raised_exception=True)
 
     inferred_dtype = infer_dtype(response)
     state.set('response_inferred_dtype', inferred_dtype)
     reward = get_exploratory_reward(state, state_copy)
 
     return state, reward, ActionInfo(action_name=_ACTION_NAME,
                                      action_fn=_infer_response_dtype,
```

### Comparing `ostatslib-0.4.0/ostatslib/actions/exploratory_actions/is_response_dichotomous_check.py` & `ostatslib-0.5.0/ostatslib/actions/exploratory_actions/is_response_dichotomous_check.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 """
 is_response_dichotomous_check module
 """
 
+import operator
 from pandas import DataFrame, Series
 from pandas.api.types import infer_dtype
 import numpy as np
 
-from ostatslib.actions import Action, ActionInfo, ActionResult
 from ostatslib.states import State
 from ._get_exploratory_reward import get_exploratory_reward
+from ..action import Action, ActionInfo, ActionResult
+from ..utils import validate_state
 
 _ACTION_NAME = "Is Response Dichotomous Check"
+_VALIDATIONS = [('response_variable_label', operator.truth, None)]
 
-
+@validate_state(action_name=_ACTION_NAME, validator_fns=_VALIDATIONS)
 def _is_response_dichotomous_check(state: State, data: DataFrame) -> ActionResult[None]:
     """
     Check if response variable is dichotomous
 
     Args:
         state (State): state
         data (DataFrame): data
```

### Comparing `ostatslib-0.4.0/ostatslib/actions/exploratory_actions/is_response_discrete_check.py` & `ostatslib-0.5.0/ostatslib/actions/exploratory_actions/is_response_discrete_check.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 """
 is_response_discrete_check module
 """
 
+import operator
 from pandas import DataFrame, Series
 import numpy as np
 
-from ostatslib.actions import Action, ActionInfo, ActionResult
 from ostatslib.states import State
 from ._get_exploratory_reward import get_exploratory_reward
+from ..action import Action, ActionInfo, ActionResult
+from ..utils import validate_state
 
 _ACTION_NAME = "Is Response Discrete Check"
+_VALIDATIONS = [('response_variable_label', operator.truth, None)]
 
-
+@validate_state(action_name=_ACTION_NAME, validator_fns=_VALIDATIONS)
 def _is_response_discrete_check(state: State, data: DataFrame) -> ActionResult[None]:
     """
     Check if response variable is discrete
 
     Args:
         state (State): state
         data (DataFrame): data
```

### Comparing `ostatslib-0.4.0/ostatslib/actions/exploratory_actions/is_response_positive_values_only_check.py` & `ostatslib-0.5.0/ostatslib/actions/exploratory_actions/is_response_positive_values_only_check.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 # pylint: disable=broad-except
 """
 is_response_positive_values_only_check module
 """
 
+import operator
 from pandas import DataFrame, Series
 import numpy as np
-from ostatslib.actions import Action, ActionInfo, ActionResult
+
 from ostatslib.states import State
 from ._get_exploratory_reward import get_exploratory_reward
+from ..action import Action, ActionInfo, ActionResult
+from ..utils import validate_state
 
 _ACTION_NAME = "Is Response Positive Values Only Check"
+_VALIDATIONS = [('response_variable_label', operator.truth, None)]
 
-
+@validate_state(action_name=_ACTION_NAME, validator_fns=_VALIDATIONS)
 def _is_response_positive_values_only_check(state: State, data: DataFrame) -> ActionResult[None]:
     """
     Check if response variable values are positive only
 
     Args:
         state (State): state
         data (DataFrame): data
```

### Comparing `ostatslib-0.4.0/ostatslib/actions/exploratory_actions/time_convertible_variable_search.py` & `ostatslib-0.5.0/ostatslib/actions/exploratory_actions/time_convertible_variable_search.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 """
 time_convertible_variable_search module
 """
 
 from pandas import DataFrame
 from pandas.api.types import infer_dtype
-from ostatslib.actions import Action, ActionInfo, ActionResult
+
+from ostatslib import config
 from ostatslib.actions.utils import split_response_from_explanatory_variables
 from ostatslib.states import State
+from ..action import Action, ActionInfo, ActionResult
 
 _ACTION_NAME = "Time Convertible Variable Search"
 
 
 ORDERED_LIST_OF_POSSIBLE_TIME_DTYPES = [
     "datetime64", "datetime", "date",
     "period",
@@ -26,16 +28,20 @@
     Args:
         state (State): state
         data (DataFrame): data
 
     Returns:
         ActionResult[None]: action result
     """
-    variables_dataframe: DataFrame = split_response_from_explanatory_variables(state,
-                                                                               data)[1]
+    if bool(state.get("response_variable_label")):
+        variables_dataframe: DataFrame = split_response_from_explanatory_variables(state,
+                                                                                   data)[1]
+    else:
+        variables_dataframe = data
+
     date_convertible_variable = __date_variable_search(variables_dataframe)
 
     reward: float = __calculate_reward(state, date_convertible_variable)
     __update_state(state, date_convertible_variable)
     return state, reward, ActionInfo(action_name=_ACTION_NAME,
                                      action_fn=_time_convertible_variable_search,
                                      model=None,
@@ -66,20 +72,20 @@
                 return var_name
 
     return time_related_variables[0]
 
 
 def __calculate_reward(state: State, date_convertible_variable: str | None) -> float:
     if state.get("time_convertible_variable") == date_convertible_variable:
-        return -1
+        return config.MIN_REWARD
 
     if date_convertible_variable == "":
-        return 0.25
+        return config.MAX_EXPLORATORY_REWARD * 0.5
 
-    return 0.5
+    return config.MAX_EXPLORATORY_REWARD
 
 
 def __update_state(state: State, date_convertible_variable: str | None) -> State:
     state.set("time_convertible_variable", date_convertible_variable)
     return state
```

### Comparing `ostatslib-0.4.0/ostatslib/actions/regression_models/decision_tree_regression.py` & `ostatslib-0.5.0/ostatslib/actions/clustering/dbscan.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,62 +1,81 @@
 """
-Decision Tree Regression module
+DBSCAN module
 """
 
-from numpy import ndarray
+import operator
+import numpy as np
+from kneed import KneeLocator
 from pandas import DataFrame
-from sklearn.model_selection import cross_val_score
-from sklearn.tree import DecisionTreeRegressor
-from ostatslib.actions import Action, ActionInfo, ActionResult
-from ostatslib.actions.utils import (calculate_score_reward,
-                                     reward_cap,
-                                     comprehensible_model,
-                                     split_response_from_explanatory_variables,
-                                     update_state_score)
-from ostatslib.states import State
+from sklearn.cluster import DBSCAN
+from sklearn.metrics import silhouette_score
+from sklearn.neighbors import NearestNeighbors
 
-_ACTION_NAME = "Decision Tree Regression"
+from ostatslib.states import State
+from ..action import Action, ActionInfo, ActionResult
+from ..utils import (calculate_score_reward,
+                     reward_cap,
+                     update_state_score,
+                     validate_state)
+
+_ACTION_NAME = "DBSCAN"
+_VALIDATIONS = [('response_variable_label', operator.eq, ''),
+                ('clusters_count', operator.eq, 0)]
 
 
+@validate_state(action_name=_ACTION_NAME, validator_fns=_VALIDATIONS)
 @reward_cap
-@comprehensible_model
-def _decision_tree_regression(state: State,
-                              data: DataFrame) -> ActionResult[DecisionTreeRegressor]:
+def _dbscan(state: State, data: DataFrame) -> ActionResult[DBSCAN]:
     """
-    Fits data to a decision tree regressor
+    Fits data to a DBSCAN cluster
 
     Args:
         state (State): current environment state
         data (DataFrame): data under analysis
 
     Returns:
-        ActionResult[DecisionTreeRegressor]: action result
+        ActionResult[DBSCAN]: action result
     """
-    if not __is_valid_state(state):
-        return state, -1, ActionInfo(action_name=_ACTION_NAME,
-                                     action_fn=_decision_tree_regression,
-                                     model=None,
-                                     raised_exception=False)
-
-    y_values, x_values = split_response_from_explanatory_variables(state, data)
-    classifier = DecisionTreeRegressor()
-    scores: ndarray = cross_val_score(classifier, x_values, y_values, cv=5)
-    score: float = scores.mean() - scores.std()
+    max_curvature_point = __get_max_curvature_point(data)
+    db_scan = DBSCAN(eps=max_curvature_point)
+    db_scan.fit(data)
+
+    if np.all(db_scan.labels_ == -1) or np.all(db_scan.labels_ == 0):
+        score = 0
+    else:
+        score = silhouette_score(data, db_scan.labels_)
 
     reward: float = calculate_score_reward(score)
     update_state_score(state, score)
     return state, reward, ActionInfo(action_name=_ACTION_NAME,
-                                     action_fn=_decision_tree_regression,
-                                     model=classifier,
+                                     action_fn=_dbscan,
+                                     model=db_scan,
                                      raised_exception=False)
 
 
-def __is_valid_state(state: State) -> bool:
-    if state.get("is_response_quantitative") <= 0 or \
-        state.get("is_response_dichotomous") > 0 or \
-            not bool(state.get("response_variable_label")):
-        return False
+def __get_max_curvature_point(data: DataFrame) -> float:
+    n_rows, n_columns = data.shape
+    if n_rows < 2 * n_columns:
+        min_points = 5
+    elif n_rows < 10 * n_columns:
+        min_points = n_columns
+    else:
+        min_points = 2* n_columns
+
+    neighbors_fit = NearestNeighbors(
+        n_neighbors=min_points, metric='euclidean').fit(data)
+    distances, _ = neighbors_fit.kneighbors(data)
+    distances = np.sort(distances.sum(axis=1), axis=0)
+    elbow_locator = KneeLocator(
+        range(0, len(distances)),
+        distances,
+        curve="convex",
+        direction="increasing",
+        interp_method='polynomial')
+
+    if elbow_locator.elbow_y is None:
+        return 0.5
 
-    return True
+    return elbow_locator.elbow_y
 
 
-decision_tree_regression: Action[DecisionTreeRegressor] = _decision_tree_regression
+dbscan: Action[DBSCAN] = _dbscan
```

### Comparing `ostatslib-0.4.0/ostatslib/actions/regression_models/linear_regression.py` & `ostatslib-0.5.0/ostatslib/actions/regression_models/linear_regression.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,98 +2,96 @@
 Linear regression module
 
 ref:
 https://www.kirenz.com/post/2021-11-14-linear-regression-diagnostics-in-python/linear-regression-diagnostics-in-python/
 """
 
 from math import nan
+import operator
 import numpy as np
 from pandas import DataFrame
 from statsmodels.api import OLS
 from statsmodels.stats.stattools import durbin_watson, jarque_bera
 from statsmodels.stats.diagnostic import het_breuschpagan, linear_harvey_collier
 from statsmodels.regression.linear_model import RegressionResults
-from ostatslib.actions import Action, ActionInfo, ActionResult
-from ostatslib.actions.utils import (calculate_score_reward,
-                                     reward_cap,
-                                     interpretable_model,
-                                     split_response_from_explanatory_variables,
-                                     update_state_score)
+from statsmodels.tools.tools import add_constant
+from ostatslib import config
+
 from ostatslib.states import State
+from ..action import Action, ActionInfo, ActionResult
+from ..utils import (calculate_score_reward,
+                     reward_cap,
+                     interpretable_model,
+                     split_response_from_explanatory_variables,
+                     update_state_score,
+                     validate_state)
 
 _ACTION_NAME = "Linear Regression"
+_VALIDATIONS = [('response_variable_label', operator.truth, None),
+                ('is_response_quantitative', operator.gt, 0),
+                ('linear_regression_score_reward', operator.eq, 0)]
 
 
+@validate_state(action_name=_ACTION_NAME, validator_fns=_VALIDATIONS)
 @reward_cap
 @interpretable_model
 def _linear_regression(state: State, data: DataFrame) -> ActionResult[RegressionResults]:
     """
     Fits data to a linear regression model.
 
     Args:
         state (State): current environment state
         data (DataFrame): data under analysis
 
     Returns:
         ActionResult[RegressionResults]: action result
     """
-    if not __is_valid_state(state):
-        return state, -1, ActionInfo(action_name=_ACTION_NAME,
-                                     action_fn=_linear_regression,
-                                     model=None,
-                                     raised_exception=False)
-
     response_var, explanatory_vars = split_response_from_explanatory_variables(
         state, data)
     try:
-        regression: RegressionResults = OLS(response_var, explanatory_vars).fit()
+        regression: RegressionResults = OLS(
+            response_var, add_constant(explanatory_vars)).fit()
     except ValueError:
-        return state, -1, ActionInfo(action_name=_ACTION_NAME,
-                                     action_fn=_linear_regression,
-                                     model=None,
-                                     raised_exception=True)
+        return state, config.MIN_REWARD, ActionInfo(action_name=_ACTION_NAME,
+                                                    action_fn=_linear_regression,
+                                                    model=None,
+                                                    raised_exception=True)
 
     reward = __calculate_reward(state, regression)
     update_state_score(state, regression.rsquared)
     return state, reward, ActionInfo(action_name=_ACTION_NAME,
                                      action_fn=_linear_regression,
                                      model=regression,
                                      raised_exception=False)
 
 
-def __is_valid_state(state: State) -> bool:
-    if state.get("is_response_quantitative") <= 0:
-        return False
-
-    return True
-
-
 def __calculate_reward(state: State, regression: RegressionResults) -> float:
     explanatory_vars: np.ndarray = regression.model.exog
     residuals: np.ndarray = regression.resid.values
-    reward: float = 0
+
+    reward = calculate_score_reward(regression.rsquared)
+    state.set('linear_regression_score_reward', reward)
 
     reward += __reward_for_normally_distributed_errors(state, regression)
     reward += __penalty_for_correlation_of_error_terms(state, residuals)
     reward += __reward_for_homoscedasticity(state, residuals, explanatory_vars)
     reward += __reward_for_recursive_residuals_mean(state, regression)
-    reward += calculate_score_reward(regression.rsquared)
 
     return reward
 
 
 def __reward_for_normally_distributed_errors(state: State,
                                              regression: RegressionResults) -> float:
     jarque_bera_pvalue = jarque_bera(regression.wresid.values)[1]
 
-    if jarque_bera_pvalue < .01:
+    if jarque_bera_pvalue < config.FULL_PENALIZED_PVALUE:
         state.set("are_linear_model_regression_residuals_normally_distributed", -1)
         return -.5
 
-    if jarque_bera_pvalue < .05:
+    if jarque_bera_pvalue < config.PARTIAL_PENALIZED_PVALUE:
         state.set(
             "are_linear_model_regression_residuals_normally_distributed", -0.5)
         return -.1
 
     if jarque_bera_pvalue < .1:
         state.set("are_linear_model_regression_residuals_normally_distributed", 0.5)
         return -.05
@@ -114,19 +112,19 @@
 
 
 def __reward_for_homoscedasticity(state: State,
                                   residuals: np.ndarray,
                                   explanatory_vars: np.ndarray) -> float:
     f_stat_pvalue = het_breuschpagan(residuals, explanatory_vars)[3]
 
-    if f_stat_pvalue < .01:
+    if f_stat_pvalue < config.FULL_PENALIZED_PVALUE:
         state.set("are_linear_model_regression_residuals_heteroscedastic", 1)
         return -.5
 
-    if f_stat_pvalue < .05:
+    if f_stat_pvalue < config.PARTIAL_PENALIZED_PVALUE:
         state.set("are_linear_model_regression_residuals_heteroscedastic", 0.5)
         return -.1
 
     if f_stat_pvalue < .1:
         state.set("are_linear_model_regression_residuals_heteroscedastic", -0.5)
         return 0.05
 
@@ -138,19 +136,19 @@
                                           regression: RegressionResults) -> float:
     try:
         pvalue = linear_harvey_collier(regression)[1]
     except ValueError:
         state.set("is_linear_model_regression_recursive_residuals_mean_zero", -1)
         return -.5
 
-    if pvalue < .01 or pvalue is nan:
+    if pvalue < config.FULL_PENALIZED_PVALUE or pvalue is nan:
         state.set("is_linear_model_regression_recursive_residuals_mean_zero", -1)
         return -.5
 
-    if pvalue < .05:
+    if pvalue < config.PARTIAL_PENALIZED_PVALUE:
         state.set("is_linear_model_regression_recursive_residuals_mean_zero", -0.5)
         return -.1
 
     if pvalue < .1:
         state.set("is_linear_model_regression_recursive_residuals_mean_zero", 0.5)
         return 0.05
```

### Comparing `ostatslib-0.4.0/ostatslib/actions/regression_models/poisson_regression.py` & `ostatslib-0.5.0/ostatslib/actions/regression_models/poisson_regression.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,84 +1,76 @@
 """
 Poisson regression module
 """
 
+import operator
 from pandas import DataFrame
 from statsmodels.api import GLM, families
 from statsmodels.genmod.generalized_linear_model import GLMResults
 from statsmodels.tools.sm_exceptions import PerfectSeparationError
-from ostatslib.actions import Action, ActionInfo, ActionResult
-from ostatslib.actions.utils import (calculate_score_reward,
-                                     reward_cap,
-                                     interpretable_model,
-                                     split_response_from_explanatory_variables,
-                                     update_state_score)
+from ostatslib import config
+
 from ostatslib.states import State
+from ..action import Action, ActionInfo, ActionResult
+from ..utils import (calculate_score_reward,
+                     reward_cap,
+                     interpretable_model,
+                     split_response_from_explanatory_variables,
+                     update_state_score,
+                     validate_state)
 
 _ACTION_NAME = "Poisson Regression"
+_VALIDATIONS = [('response_variable_label', operator.truth, None),
+                ('is_response_positive_values_only', operator.gt, 0),
+                ('is_response_discrete', operator.gt, 0),
+                ('log_rows_count', operator.lt, 0.81),
+                ('poisson_regression_score_reward', operator.eq, 0)]
 
 
+@validate_state(action_name=_ACTION_NAME, validator_fns=_VALIDATIONS)
 @reward_cap
 @interpretable_model
 def _poisson_regression(state: State, data: DataFrame) -> ActionResult[GLMResults]:
     """
     Fits data to a poisson regression model.
 
     Args:
         state (State): current environment state
         data (DataFrame): data under analysis
 
     Returns:
         ActionResult[GLMResults]: action result
     """
-    if not __is_valid_state(state):
-        return state, -1, ActionInfo(action_name=_ACTION_NAME,
-                                     action_fn=_poisson_regression,
-                                     model=None,
-                                     raised_exception=False)
-
     response_var, explanatory_vars = split_response_from_explanatory_variables(state,
                                                                                data)
     try:
         poisson_family = families.Poisson()
         regression: GLMResults = GLM(response_var,
                                      explanatory_vars,
                                      poisson_family).fit()
     except ValueError:
-        return state, -1, ActionInfo(action_name=_ACTION_NAME,
-                                     action_fn=_poisson_regression,
-                                     model=None,
-                                     raised_exception=True)
+        state.set('poisson_regression_score_reward', config.MIN_REWARD)
+        return __raised_exception_action_result(state)
     except PerfectSeparationError:
         state.set('does_poisson_regression_raises_perfect_separation_error', 1)
-        state.set('score', -1)
-        return state, -1, ActionInfo(action_name=_ACTION_NAME,
-                                     action_fn=_poisson_regression,
-                                     model=None,
-                                     raised_exception=True)
+        state.set('poisson_regression_score_reward', config.MIN_REWARD)
+        return __raised_exception_action_result(state)
 
     state.set('does_poisson_regression_raises_perfect_separation_error', -1)
-    reward = __calculate_reward(regression)
-    state = update_state_score(state, regression.pseudo_rsquared())
+    score = regression.pseudo_rsquared()
+    reward = calculate_score_reward(score)
+    state = update_state_score(state, score)
+    state.set('poisson_regression_score_reward', reward)
     return state, reward, ActionInfo(action_name=_ACTION_NAME,
                                      action_fn=_poisson_regression,
                                      model=regression,
                                      raised_exception=False)
 
 
-def __is_valid_state(state: State) -> bool:
-    if state.get("is_response_positive_values_only") <= 0:
-        return False
-
-    if state.get("is_response_discrete") <= 0:
-        return False
-
-    return True
-
-
-def __calculate_reward(regression: GLMResults) -> float:
-    reward: float = 0
-    reward += calculate_score_reward(regression.pseudo_rsquared())
-    return reward
+def __raised_exception_action_result(state):
+    return state, config.MIN_REWARD, ActionInfo(action_name=_ACTION_NAME,
+                                                action_fn=_poisson_regression,
+                                                model=None,
+                                                raised_exception=True)
 
 
 poisson_regression: Action[GLMResults] = _poisson_regression
```

### Comparing `ostatslib-0.4.0/ostatslib/actions/regression_models/time_series_auto_arima.py` & `ostatslib-0.5.0/ostatslib/actions/regression_models/time_series_auto_arima.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,37 @@
 """
 Time series using Auto Arima module
 
 ref: https://www.machinelearningplus.com/time-series/arima-model-time-series-forecasting-python/
 """
 
+import operator
 from pandas import DataFrame, Series, to_datetime
 from pmdarima import auto_arima, ARIMA as AUTOARIMA
 from statsmodels.tsa.statespace.sarimax import SARIMAXResults
 import numpy as np
-from ostatslib.actions import Action, ActionInfo, ActionResult
-from ostatslib.actions.utils import (calculate_score_reward,
-                                     reward_cap,
-                                     interpretable_model,
-                                     split_response_from_explanatory_variables)
+from ostatslib import config
+
 from ostatslib.states import State
+from ..action import Action, ActionInfo, ActionResult
+from ..utils import (calculate_score_reward,
+                     reward_cap,
+                     interpretable_model,
+                     split_response_from_explanatory_variables,
+                     validate_state)
 
 TRAINING_FRACTION: float = 0.9
 
 _ACTION_NAME = "Time Series - SARIMAX"
+_VALIDATIONS = [('response_variable_label', operator.truth, None),
+                ('is_response_quantitative', operator.gt, 0),
+                ('time_series_auto_arima_score_reward', operator.eq, 0)]
 
 
+@validate_state(action_name=_ACTION_NAME, validator_fns=_VALIDATIONS)
 @reward_cap
 @interpretable_model
 def _time_series_auto_arima(state: State,
                             data: DataFrame) -> ActionResult[SARIMAXResults]:
     """
     Fits data to an ARIMA model
 
@@ -31,18 +39,18 @@
         state (State): current environment state
         data (DataFrame): data under analysis
 
     Returns:
         ActionResult[SARIMAXResults]: action result
     """
     if not __is_valid_state(state):
-        return state, -1, ActionInfo(action_name=_ACTION_NAME,
-                                     action_fn=_time_series_auto_arima,
-                                     model=None,
-                                     raised_exception=False)
+        return state, config.MIN_REWARD, ActionInfo(action_name=_ACTION_NAME,
+                                                    action_fn=_time_series_auto_arima,
+                                                    model=None,
+                                                    raised_exception=False)
 
     y_data, x_data = __build_time_index_dataframes_for_y_and_x(state, data)
     data_length = len(y_data)
     training_split_index = int(data_length * TRAINING_FRACTION)
     y_training, y_testing = (y_data.iloc[:training_split_index],
                              y_data.iloc[training_split_index:])
     if x_data is None:
@@ -55,15 +63,15 @@
     model: SARIMAXResults = auto_arima_model.arima_res_
 
     forecast: Series = model.forecast(data_length - training_split_index,
                                       exog=x_testing)
     score: float = 1 - \
         __calculate_mean_abs_percentage_error(forecast, y_testing)
 
-    reward: float = __calculate_reward(model, score)
+    reward: float = __calculate_reward(state, model, score)
     return state, reward, ActionInfo(action_name=_ACTION_NAME,
                                      action_fn=_time_series_auto_arima,
                                      model=model,
                                      raised_exception=False)
 
 
 def __is_valid_state(state: State) -> bool:
@@ -77,20 +85,22 @@
 
 def __calculate_mean_abs_percentage_error(forecast: Series, y_testing: DataFrame) -> float:
     forecast_values = forecast.values.flatten()
     y_testing_values = y_testing.values.flatten()
     return np.mean(np.abs(forecast_values - y_testing_values)/np.abs(y_testing_values))
 
 
-def __calculate_reward(model: SARIMAXResults, correlation_coef: float) -> float:
-    reward: float = 0
+def __calculate_reward(state: State, model: SARIMAXResults, correlation_coef: float) -> float:
+    reward = calculate_score_reward(correlation_coef)
+    state.set('time_series_auto_arima_score_reward', reward)
+
     reward += __penalty_for_correlated_residuals(model)
     reward += __penalty_for_heteroskedasticity_residuals(model)
     reward += __penalty_for_non_normal_residuals(model)
-    reward += calculate_score_reward(correlation_coef)
+
     return reward
 
 
 def __penalty_for_correlated_residuals(model: SARIMAXResults) -> float:
     lag_correlations = model.test_serial_correlation(method='ljungbox')[:, 1]
     max_corr = np.max(lag_correlations)
```

### Comparing `ostatslib-0.4.0/ostatslib/actions/utils/explainability_rewards.py` & `ostatslib-0.5.0/ostatslib/actions/utils/explainability_rewards.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 """
 explainability rewards decorators module
 """
 
 from functools import wraps
-from typing import TypeVar
 
 from pandas import DataFrame
 
 from ostatslib.states import State
-from ostatslib.actions import Action, TModel
-
-T = TypeVar("T")
+from ..action import Action, TModel
 
 OPAQUE_PENALTY = -.1
 INTERPRETABLE_REWARD = .1
 COMPREHENSIBLE_REWARD = .075
 
 
 def opaque_model(
```

### Comparing `ostatslib-0.4.0/ostatslib/actions/utils/reward_cap.py` & `ostatslib-0.5.0/ostatslib/actions/utils/reward_cap.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,17 @@
 """
 reward_cap function module
 """
 
 from functools import wraps
-from typing import TypeVar
 from pandas import DataFrame
-from ostatslib.actions import Action, TModel
+from ostatslib import config
 from ostatslib.states import State
+from ..action import Action, TModel
 
-REWARD_UPPER_LIMIT = float(1)
-REWARD_LOWER_LIMIT = float(-1)
-
-T = TypeVar('T')
 
 def reward_cap(action_function: Action[TModel]) -> Action[TModel]:
     """
     Limits rewards from an action within lower and upper limits
 
     Args:
         action_function (Action[TModel]): action
@@ -23,11 +19,11 @@
     Returns:
         Action[TModel]: action
     """
     wraps(action_function)
 
     def function_wrapper(state: State, data: DataFrame):
         state, reward, info = action_function(state, data)
-        reward = min(max(REWARD_LOWER_LIMIT, reward), REWARD_UPPER_LIMIT)
+        reward = min(max(config.MIN_REWARD, reward), config.MAX_REWARD)
         return state, reward, info
 
     return function_wrapper
```

### Comparing `ostatslib-0.4.0/ostatslib/actions/utils/split_response_from_explanatory_variables.py` & `ostatslib-0.5.0/ostatslib/actions/utils/split_response_from_explanatory_variables.py`

 * *Files identical despite different names*

### Comparing `ostatslib-0.4.0/ostatslib/agents/agent.py` & `ostatslib-0.5.0/ostatslib/agents/agent.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Open Stats Agent abstract module
 """
 
 from abc import ABC, abstractmethod
-from typing import Tuple
 from numpy import ndarray
 from pandas import DataFrame
+from ostatslib import config
 
 from ostatslib.agents.analysis_result import AnalysisResult
 from ostatslib.environments import GymEnvironment
 from ostatslib.states.state import State
 
 
 class Agent(ABC):
@@ -46,22 +46,22 @@
         Returns:
             ndarray: action
         """
 
     def analyze(self,
                 data: DataFrame,
                 initial_state: State = State(),
-                max_steps: int = 20) -> AnalysisResult:
+                max_steps: int = config.MAX_STEPS) -> AnalysisResult:
         """
         Analyzes a dataset
 
         Args:
             data (DataFrame): dataset
             initial_state (State, optional): initial state. Defaults to State().
-            max_steps (int, optional): maximum number of steps. Defaults to 20.
+            max_steps (int, optional): maximum number of steps.
 
         Returns:
             AnalysisResult: analysis result
         """
         environment = GymEnvironment()
         environment.reset()
         environment.set_data(data)
```

### Comparing `ostatslib-0.4.0/ostatslib/agents/analysis_result.py` & `ostatslib-0.5.0/ostatslib/agents/analysis_result.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,17 +17,27 @@
     """
     Analysis class
     """
     initial_state: State
     steps: list[tuple[float, ActionInfo]]
     done: bool
     timestamp: datetime = field(init=False)
+    steps_count: int = field(init=False)
+    total_reward: float = field(init=False)
+    actions_names_list: list[str] = field(init=False)
 
     def __post_init__(self):
         object.__setattr__(self, 'timestamp', datetime.now())
+        object.__setattr__(self, 'steps_count', len(self.steps))
+        object.__setattr__(self,
+                           'total_reward',
+                           sum(reward for reward, _ in self.steps))
+        object.__setattr__(self,
+                           'actions_names_list',
+                           [info['action_name'] for _, info in self.steps])
 
     def summary(self) -> str:
         """
         Returns analysis summary
 
         Returns:
             str: analysis summary
@@ -48,11 +58,12 @@
         table_rows: StepsRows = []
 
         for i, (reward, info) in enumerate(self.steps):
             table_rows.append((
                 i+1,
                 str(info['action_name']),
                 reward,
-                tabulate(info['state_delta'].list_known_features(), tablefmt="plain")
+                tabulate(info['state_delta'].list_known_features(),
+                         tablefmt="plain")
             ))
 
         return tabulate(table_rows, steps_headers)
```

### Comparing `ostatslib-0.4.0/ostatslib/agents/ppo_agent.py` & `ostatslib-0.5.0/ostatslib/agents/ppo_agent.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,10 +44,10 @@
     def _predict(self, observation: dict) -> ndarray:
         action, _ = self.__model.predict(observation, deterministic=True)
         return action[0]
 
     def __init__model(self, path: str | None, training_envs_count: int) -> PPO:
         if path is None:
             environments = make_vec_env(GymEnvironment, training_envs_count)
-            return PPO(POLICY, environments, verbose=1, policy_kwargs=POLICY_KWARGS)
+            return PPO(POLICY, environments, verbose=1, n_steps=6144, policy_kwargs=POLICY_KWARGS)
 
         return PPO.load(path)
```

### Comparing `ostatslib-0.4.0/ostatslib/environments/gym_environment.py` & `ostatslib-0.5.0/ostatslib/environments/gym_environment.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,37 +3,37 @@
 """
 
 from typing import Any
 from numpy import ndarray
 from pandas import DataFrame
 from gymnasium import Env
 from gymnasium.spaces import Dict
+from ostatslib import config
 from ostatslib.actions import ActionsSpace
 from ostatslib.actions.action import ActionInfo
 from ostatslib.actions.actions_space import _invalid_action_step
 from ostatslib.states import State
 from .utils import generate_training_dataset
 
 ObsType = Dict
-REWARD_RANGE = (-1, 1)
 
 
 class GymEnvironment(Env):
     """
     Statistical environment implemented as Gymnasium environment
     """
 
     __state: State
     __data: DataFrame
 
     def __init__(self) -> None:
         self.__init_state_and_data()
         self.observation_space = State().as_gymnasium_space
         self.action_space: ActionsSpace = ActionsSpace()
-        self.reward_range = REWARD_RANGE
+        self.reward_range = config.REWARD_RANGE
         self.__steps_taken = 0
 
     def render(self) -> None:
         print("Render has no effect yet")
 
     def reset(self,
               *,
@@ -74,11 +74,12 @@
 
         Args:
             state (State): State
         """
         self.__state = state
 
     def __is_done(self, state: State, reward: float) -> bool:
-        return (state.get("score") > 0.6 and reward > 0.5) or self.__steps_taken >= 10
+        return (state.get("score") > config.MIN_ACCEPTED_SCORE and reward > config.MAX_REWARD/2)\
+            or self.__steps_taken >= config.MAX_STEPS
 
     def __init_state_and_data(self):
         self.__data, self.__state = generate_training_dataset()
```

### Comparing `ostatslib-0.4.0/ostatslib/environments/utils/_generate_from_datacooker.py` & `ostatslib-0.5.0/ostatslib/environments/utils/_generate_from_datacooker.py`

 * *Files identical despite different names*

### Comparing `ostatslib-0.4.0/ostatslib/environments/utils/_generate_from_sklearn.py` & `ostatslib-0.5.0/ostatslib/environments/utils/_generate_from_sklearn.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 # "make_sparse_coded_signal",
 # "make_sparse_spd_matrix",
 # "make_sparse_uncorrelated",
 # "make_spd_matrix",
 # "make_swiss_roll",
 """
 
-from random import choice
+from random import choice, getrandbits
 from pandas import DataFrame
 import sklearn.datasets as sklearn_dts
 import numpy as np
 
 from ostatslib.states import State
 
 
@@ -37,15 +37,15 @@
     """
     Generates a dataset from sklearn's toy datasets or generated
     https://scikit-learn.org/stable/datasets.html
 
     Returns:
         tuple[DataFrame, State]: dataset and initial state
     """
-    sklearn_gen_fn = choice([_from_toy, __from_generated])
+    sklearn_gen_fn = choice([_from_toy, __from_generated, __from_cluster])
     return sklearn_gen_fn()
 
 
 _TOY_FUNCTIONS = (
     sklearn_dts.load_iris,
     sklearn_dts.load_diabetes,
     sklearn_dts.load_digits,
@@ -61,23 +61,37 @@
     state = State()
     state.set('response_variable_label', y_series.name)
     return data, state
 
 
 def __from_generated() -> tuple[DataFrame, State]:
     sample_gen_fn = choice([
-        __make_blobs,
         __make_classification,
         __make_regression
     ])
     x_values, y_values = sample_gen_fn()
+
     data = DataFrame(x_values)
-    data['result'] = y_values
+    data['target'] = y_values
+
     state = State()
-    state.set('response_variable_label', 'result')
+    state.set('response_variable_label', 'target')
+
+    return data, state
+
+
+def __from_cluster() -> tuple[DataFrame, State]:
+    n_centers, xy_tuple = __make_blobs()
+    data = DataFrame(xy_tuple[0])
+    state = State()
+    state.set('response_variable_label', '')
+
+    if bool(getrandbits(1)):
+        state.set('clusters_count', n_centers)
+
     return data, state
 
 
 def __get_n_samples_and_features() -> tuple[int, int]:
     n_samples = np.random.randint(20, 1000)
     n_features = np.random.randint(5, 50)
     return n_samples, n_features
@@ -109,13 +123,14 @@
         n_repeated=n_repeated,
         n_classes=n_classes
     )
 
 
 def __make_blobs():
     n_samples, n_features = __get_n_samples_and_features()
-    centers = np.random.randint(2, 20)
-    return sklearn_dts.make_blobs(
+    n_centers = np.random.randint(2, 20)
+    return n_centers, sklearn_dts.make_blobs(
         n_samples=n_samples,
         n_features=n_features,
-        centers=centers
+        centers=n_centers,
+        cluster_std=0.5
     )
```

### Comparing `ostatslib-0.4.0/ostatslib/states/analysis_features_set.py` & `ostatslib-0.5.0/ostatslib/states/analysis_features_set.py`

 * *Files identical despite different names*

### Comparing `ostatslib-0.4.0/ostatslib/states/data_features_set.py` & `ostatslib-0.5.0/ostatslib/states/data_features_set.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,14 +52,21 @@
     log_rows_count: float = field(
         default=0,
         metadata={
             'gym_space': Box(0, 1),
             'get_value_fn': None
         })
 
+    response_unique_values_ratio: float = field(
+        default=0,
+        metadata={
+            'gym_space': Box(0, 1),
+            'get_value_fn': None
+        })
+
     response_inferred_dtype: str = field(
         default="unknown-array",
         metadata={
             'gym_space': MultiBinary(MAX_INFERRED_DTYPE_INDEX),
             'get_value_fn': _map_inferred_dtype_to_binary_array
         })
```

### Comparing `ostatslib-0.4.0/ostatslib/states/features_set.py` & `ostatslib-0.5.0/ostatslib/states/features_set.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,24 +33,24 @@
     def as_gymnasium_space(self) -> dict:
         """
         Features as Gymnasium space
 
         Returns:
             dict: dictionary of features and their Gymnasium spaces
         """
-        return dict((field.name, field.metadata['gym_space']) for field in fields(self))
+        return {field.name: field.metadata['gym_space'] for field in fields(self)}
 
     def as_features_dict(self) -> dict:
         """
         Features values as dictionary
 
         Returns:
             dict: dictionary with features values
         """
-        return dict([(field.name, self.__get_feature_value(field)) for field in fields(self)])
+        return {field.name: self.__get_feature_value(field) for field in fields(self)}
 
     def __array__(self):
         return np.concatenate([self.__get_feature_value(field) for field in fields(self)])
 
     def __get_feature_value(self, _field: Field) -> NDArray[np.float64]:
         get_value_fn = _field.metadata['get_value_fn']
         field_value = getattr(self, _field.name)
```

### Comparing `ostatslib-0.4.0/ostatslib/states/state.py` & `ostatslib-0.5.0/ostatslib/states/state.py`

 * *Files identical despite different names*

### Comparing `ostatslib-0.4.0/ostatslib/states/state_iterator.py` & `ostatslib-0.5.0/ostatslib/states/state_iterator.py`

 * *Files identical despite different names*

### Comparing `ostatslib-0.4.0/ostatslib/states/utils/init_features_set.py` & `ostatslib-0.5.0/ostatslib/states/utils/init_features_set.py`

 * *Files identical despite different names*

### Comparing `ostatslib-0.4.0/pyproject.toml` & `ostatslib-0.5.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,42 +1,44 @@
 [tool.poetry]
 name = "ostatslib"
-version = "0.4.0"
+version = "0.5.0"
 description = "Open Statistical Analysis Agent Library"
 authors = ["Guilherme <g.lisboa.oliveira@outlook.com>"]
 repository = "https://github.com/OStatsAA/ostatslib"
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.12"
 numpy = "^1.23.4"
-pandas = "^1.5.0"
-statsmodels = "^0.13.2"
+pandas = "^2.0.1"
+statsmodels = ">=0.13.2,<0.15.0"
 scipy = "^1.9.3"
 scikit-learn = "^1.1.2"
 pmdarima = "^2.0.2"
 tabulate = "^0.9.0"
-datacooker = "0.4.0"
+datacooker = "^0.4.1"
 tensorboard = "^2.12.0"
-stable-baselines3 = "2.0.0a5"
+stable-baselines3 = "2.0.0a10"
+pmlb = "^1.0.1.post3"
+kneed = "^0.8.3"
 
 [tool.poetry.group.dev.dependencies]
 pylint = "^2.15.4"
 autopep8 = ">=1.7,<3.0"
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.1.3"
 pytest-cov = "^4.0.0"
 scipy = "^1.9.2"
 
 
 [tool.poetry.group.docs.dependencies]
 jupyter-book = "^0.15.0"
-sphinxcontrib-mermaid = "^0.8.1"
+sphinxcontrib-mermaid = ">=0.8.1,<0.10.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.coverage.run]
 relative_files = true
```

### Comparing `ostatslib-0.4.0/PKG-INFO` & `ostatslib-0.5.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 Metadata-Version: 2.1
 Name: ostatslib
-Version: 0.4.0
+Version: 0.5.0
 Summary: Open Statistical Analysis Agent Library
 Home-page: https://github.com/OStatsAA/ostatslib
 License: MIT
 Author: Guilherme
 Author-email: g.lisboa.oliveira@outlook.com
 Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: datacooker (==0.4.0)
+Requires-Dist: datacooker (>=0.4.1,<0.5.0)
+Requires-Dist: kneed (>=0.8.3,<0.9.0)
 Requires-Dist: numpy (>=1.23.4,<2.0.0)
-Requires-Dist: pandas (>=1.5.0,<2.0.0)
+Requires-Dist: pandas (>=2.0.1,<3.0.0)
 Requires-Dist: pmdarima (>=2.0.2,<3.0.0)
+Requires-Dist: pmlb (>=1.0.1.post3,<2.0.0)
 Requires-Dist: scikit-learn (>=1.1.2,<2.0.0)
 Requires-Dist: scipy (>=1.9.3,<2.0.0)
-Requires-Dist: stable-baselines3 (==2.0.0a5)
-Requires-Dist: statsmodels (>=0.13.2,<0.14.0)
+Requires-Dist: stable-baselines3 (==2.0.0a10)
+Requires-Dist: statsmodels (>=0.13.2,<0.15.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Requires-Dist: tensorboard (>=2.12.0,<3.0.0)
 Project-URL: Repository, https://github.com/OStatsAA/ostatslib
 Description-Content-Type: text/markdown
 
 # ostatslib
 Open Statistics Library
```

