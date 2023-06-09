# Comparing `tmp/wnb-0.1.13.tar.gz` & `tmp/wnb-0.1.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wnb-0.1.13.tar", last modified: Sun Jun  4 17:17:51 2023, max compression
+gzip compressed data, was "wnb-0.1.14.tar", last modified: Fri Jun  9 18:20:06 2023, max compression
```

## Comparing `wnb-0.1.13.tar` & `wnb-0.1.14.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 17:17:50.996507 wnb-0.1.13/
--rw-r--r--   0 runner    (1001) docker     (123)     4402 2023-06-04 17:17:50.996507 wnb-0.1.13/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3459 2023-06-04 17:17:39.000000 wnb-0.1.13/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 17:17:50.996507 wnb-0.1.13/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-06-04 17:17:39.000000 wnb-0.1.13/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 17:17:50.992507 wnb-0.1.13/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5301 2023-06-04 17:17:39.000000 wnb-0.1.13/tests/test_gnb.py
--rw-r--r--   0 runner    (1001) docker     (123)     5568 2023-06-04 17:17:39.000000 wnb-0.1.13/tests/test_gwnb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 17:17:50.992507 wnb-0.1.13/wnb/
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-04 17:17:39.000000 wnb-0.1.13/wnb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-06-04 17:17:39.000000 wnb-0.1.13/wnb/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-04 17:17:39.000000 wnb-0.1.13/wnb/_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     5966 2023-06-04 17:17:39.000000 wnb-0.1.13/wnb/dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     9969 2023-06-04 17:17:39.000000 wnb-0.1.13/wnb/gnb.py
--rw-r--r--   0 runner    (1001) docker     (123)    14969 2023-06-04 17:17:39.000000 wnb-0.1.13/wnb/gwnb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 17:17:50.996507 wnb-0.1.13/wnb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4402 2023-06-04 17:17:50.000000 wnb-0.1.13/wnb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-04 17:17:50.000000 wnb-0.1.13/wnb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 17:17:50.000000 wnb-0.1.13/wnb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-04 17:17:50.000000 wnb-0.1.13/wnb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-04 17:17:50.000000 wnb-0.1.13/wnb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:20:06.043672 wnb-0.1.14/
+-rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-06-09 18:20:06.043672 wnb-0.1.14/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-06-09 18:19:55.000000 wnb-0.1.14/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 18:20:06.043672 wnb-0.1.14/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-06-09 18:19:55.000000 wnb-0.1.14/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:20:06.035672 wnb-0.1.14/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7762 2023-06-09 18:19:55.000000 wnb-0.1.14/tests/test_gnb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5568 2023-06-09 18:19:55.000000 wnb-0.1.14/tests/test_gwnb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:20:06.039672 wnb-0.1.14/wnb/
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-09 18:19:55.000000 wnb-0.1.14/wnb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-06-09 18:19:55.000000 wnb-0.1.14/wnb/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-06-09 18:19:55.000000 wnb-0.1.14/wnb/_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-06-09 18:19:55.000000 wnb-0.1.14/wnb/dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10559 2023-06-09 18:19:55.000000 wnb-0.1.14/wnb/gnb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14969 2023-06-09 18:19:55.000000 wnb-0.1.14/wnb/gwnb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:20:06.039672 wnb-0.1.14/wnb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-06-09 18:20:06.000000 wnb-0.1.14/wnb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-09 18:20:06.000000 wnb-0.1.14/wnb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 18:20:06.000000 wnb-0.1.14/wnb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-09 18:20:06.000000 wnb-0.1.14/wnb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-09 18:20:06.000000 wnb-0.1.14/wnb.egg-info/top_level.txt
```

### Comparing `wnb-0.1.13/PKG-INFO` & `wnb-0.1.14/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wnb
-Version: 0.1.13
+Version: 0.1.14
 Summary: Python library for the implementations of general and weighted naive Bayes (WNB) classifiers.
 Home-page: https://github.com/msamsami/weighted-naive-bayes
 Author: Mehdi Samsami
 Author-email: mehdisamsami@live.com
 Keywords: python,bayes,naivebayes,classifier,probabilistic
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
@@ -17,18 +17,20 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # WNB: General and weighted naive Bayes classifiers
 
-![](https://img.shields.io/badge/version-v0.1.13-green)
+![](https://img.shields.io/badge/version-v0.1.14-green)
 ![](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9-blue)
 ![](https://github.com/msamsami/weighted-naive-bayes/actions/workflows/python-publish.yml/badge.svg)
 [![](https://img.shields.io/pypi/v/wnb)](https://pypi.org/project/wnb/)
+![](https://img.shields.io/pypi/dm/wnb)
+
 
 <p>
 <img src="https://raw.githubusercontent.com/msamsami/weighted-naive-bayes/main/logo.png" alt="wnb logo" width="275" />
 <br>
 </p>
 
 ## Introduction
@@ -105,7 +107,18 @@
 wnb.fit(X, y)
 ```
 
 4. Predict on test data
 ```python
 wnb.predict(x_test)
 ```
+
+## Tests
+To run the tests, install development requirements:
+```
+pip install -r requirements_dev.txt
+```
+
+Then, run pytest:
+```
+pytest
+```
```

### Comparing `wnb-0.1.13/README.md` & `wnb-0.1.14/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # WNB: General and weighted naive Bayes classifiers
 
-![](https://img.shields.io/badge/version-v0.1.13-green)
+![](https://img.shields.io/badge/version-v0.1.14-green)
 ![](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9-blue)
 ![](https://github.com/msamsami/weighted-naive-bayes/actions/workflows/python-publish.yml/badge.svg)
 [![](https://img.shields.io/pypi/v/wnb)](https://pypi.org/project/wnb/)
+![](https://img.shields.io/pypi/dm/wnb)
+
 
 <p>
 <img src="https://raw.githubusercontent.com/msamsami/weighted-naive-bayes/main/logo.png" alt="wnb logo" width="275" />
 <br>
 </p>
 
 ## Introduction
@@ -84,7 +86,18 @@
 wnb.fit(X, y)
 ```
 
 4. Predict on test data
 ```python
 wnb.predict(x_test)
 ```
+
+## Tests
+To run the tests, install development requirements:
+```
+pip install -r requirements_dev.txt
+```
+
+Then, run pytest:
+```
+pytest
+```
```

### Comparing `wnb-0.1.13/setup.py` & `wnb-0.1.14/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import codecs
 from os import path
 from setuptools import setup
 
 
 setup(
     name='wnb',
-    version='0.1.13',
+    version='0.1.14',
     description='Python library for the implementations of general and weighted naive Bayes (WNB) classifiers.',
     keywords=['python', 'bayes', 'naivebayes', 'classifier', 'probabilistic'],
     author='Mehdi Samsami',
     author_email='mehdisamsami@live.com',
     url='https://github.com/msamsami/weighted-naive-bayes',
     long_description=codecs.open(path.join(path.abspath(path.dirname(__file__)), 'README.md'), encoding='utf-8').read(),
     long_description_content_type='text/markdown',
```

### Comparing `wnb-0.1.13/tests/test_gnb.py` & `wnb-0.1.14/tests/test_gwnb.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import numpy as np
 
 import pytest
 from sklearn.utils.estimator_checks import check_estimator
 from sklearn.base import is_classifier
 from sklearn.utils._testing import assert_array_equal, assert_array_almost_equal
-from sklearn.naive_bayes import GaussianNB
 
-from wnb import GeneralNB, Distribution as D
+from wnb import GaussianWNB
 
 # Data is just 6 separable points in the plane
 X = np.array([[-2, -1], [-1, -1], [-1, -2], [1, 1], [1, 2], [2, 1]])
 y = np.array([1, 1, 1, 2, 2, 2])
 
 
 @pytest.fixture
@@ -22,101 +21,108 @@
     # A bit more random tests
     rng = np.random.RandomState(global_random_seed)
     X1 = rng.normal(size=(10, 3))
     y1 = (rng.normal(size=10) > 0).astype(int)
     return X1, y1
 
 
-def test_gnb():
-    """General Naive Bayes classification
+def test_gwnb():
+    """Binary Gaussian MLD-WNB classification
 
-    Checks that GeneralNB implements fit and predict and returns correct values for a simple toy dataset.
+    Checks that GaussianWNB implements fit and predict and returns correct values for a simple toy dataset.
     """
-    clf = GeneralNB()
+    clf = GaussianWNB()
     y_pred = clf.fit(X, y).predict(X)
     assert_array_equal(y_pred, y)
 
     y_pred_proba = clf.predict_proba(X)
     y_pred_log_proba = clf.predict_log_proba(X)
     assert_array_almost_equal(np.log(y_pred_proba), y_pred_log_proba, 8)
 
 
-def test_gnb_vs_sklearn():
-    """General Naive Bayes classification vs sklearn Gaussian Naive Bayes classification.
-
-    Test GeneralNB with gaussian likelihoods returns the same outputs as the sklearn GaussianNB.
+def test_gwnb_estimator():
     """
-    clf1 = GeneralNB()
-    clf1.fit(X, y)
-
-    clf2 = GaussianNB()
-    clf2.fit(X, y)
-
-    y_pred1 = clf1.predict(X)
-    y_pred2 = clf2.predict(X)
-    assert_array_equal(y_pred1, y_pred2)
-
-    y_pred_proba1 = clf1.predict_proba(X)
-    y_pred_proba2 = clf2.predict_proba(X)
-    assert_array_almost_equal(y_pred_proba1, y_pred_proba2, 6)
-
-    y_pred_log_proba1 = clf1.predict_log_proba(X)
-    y_pred_log_proba2 = clf2.predict_log_proba(X)
-    assert_array_almost_equal(y_pred_log_proba1, y_pred_log_proba2, 5)
-
-
-def test_gnb_estimator():
+    Test whether GaussianWNB estimator adheres to scikit-learn conventions.
     """
-    Test whether GeneralNB estimator adheres to scikit-learn conventions.
-    """
-    # check_estimator(GeneralNB())
-    assert is_classifier(GeneralNB)
+    check_estimator(GaussianWNB())
+    assert is_classifier(GaussianWNB)
 
 
-def test_gnb_prior(global_random_seed):
+def test_gwnb_prior(global_random_seed):
     """
     Test whether class priors are properly set.
     """
-    clf = GeneralNB().fit(X, y)
+    clf = GaussianWNB().fit(X, y)
     assert_array_almost_equal(np.array([3, 3]) / 6.0, clf.class_prior_, 8)
 
     X1, y1 = get_random_normal_x_binary_y(global_random_seed)
-    clf = GeneralNB().fit(X1, y1)
+    clf = GaussianWNB().fit(X1, y1)
 
     # Check that the class priors sum to 1
     assert_array_almost_equal(clf.class_prior_.sum(), 1)
 
 
-def test_gnb_neg_priors():
+def test_gwnb_neg_priors():
     """
     Test whether an error is raised in case of negative priors.
     """
-    clf = GeneralNB(priors=np.array([-1.0, 2.0]))
+    clf = GaussianWNB(priors=np.array([-1.0, 2.0]))
 
     msg = "Priors must be non-negative"
     with pytest.raises(ValueError, match=msg):
         clf.fit(X, y)
 
 
-def test_gnb_priors():
+def test_gwnb_priors():
     """
     Test whether the class priors override is properly used.
     """
-    clf = GeneralNB(priors=np.array([0.3, 0.7])).fit(X, y)
+    clf = GaussianWNB(priors=np.array([0.3, 0.7])).fit(X, y)
     assert_array_almost_equal(
         clf.predict_proba([[-0.1, -0.1]]),
-        np.array([[0.825303662161683, 0.174696337838317]]),
-        6,
+        np.array([[0.823571, 0.176429]]),
+        8,
     )
     assert_array_almost_equal(clf.class_prior_, np.array([0.3, 0.7]))
 
 
-def test_gnb_priors_sum_isclose():
+def test_gwnb_wrong_nb_priors():
+    """
+    Test whether an error is raised if the number of priors is different from the number of classes.
+    """
+    clf = GaussianWNB(priors=np.array([0.25, 0.25, 0.25, 0.25]))
+
+    msg = "Number of priors must match the number of classes"
+    with pytest.raises(ValueError, match=msg):
+        clf.fit(X, y)
+
+
+def test_gwnb_prior_greater_one():
+    """
+    Test if an error is raised if the sum of priors greater than one.
+    """
+    clf = GaussianWNB(priors=np.array([2.0, 1.0]))
+
+    msg = "The sum of the priors should be 1"
+    with pytest.raises(ValueError, match=msg):
+        clf.fit(X, y)
+
+
+def test_gwnb_prior_large_bias():
     """
-    Test whether the class priors sum is properly tested.
+    Test if good prediction when class priors favor largely one class.
+    """
+    clf = GaussianWNB(priors=np.array([0.01, 0.99]))
+    clf.fit(X, y)
+    assert clf.predict(np.array([[-0.1, -0.1]])) == np.array([2])
+
+
+def test_gwnb_non_binary():
+    """
+    Test if an error is raised when given non-binary targets.
     """
     X_ = np.array(
         [
             [-1, -1],
             [-2, -1],
             [-3, -2],
             [-4, -5],
@@ -124,64 +130,71 @@
             [1, 1],
             [2, 1],
             [3, 2],
             [4, 4],
             [5, 5],
         ]
     )
-    priors = np.array([0.08, 0.14, 0.03, 0.16, 0.11, 0.16, 0.07, 0.14, 0.11, 0.0])
-    y_ = np.array([1, 2, 3, 4, 5, 6, 7, 8, 9, 10])
-    clf = GeneralNB(priors=priors)
-    clf.fit(X_, y_)
+    y_ = np.array([1, 2, 3, 4, 4, 3, 2, 1, 1, 2])
+    clf = GaussianWNB()
+
+    msg = "Unknown label type: non-binary"
+    with pytest.raises(ValueError, match=msg):
+        clf.fit(X_, y_)
 
 
-def test_gnb_wrong_nb_priors():
+def test_gwnb_wrong_error_weights():
     """
-    Test whether an error is raised if the number of priors is different from the number of classes.
+    Test whether an error is raised in case error weight is not a square array of size (n_classes, n_classes).
     """
-    clf = GeneralNB(priors=np.array([0.25, 0.25, 0.25, 0.25]))
+    clf = GaussianWNB(error_weights=np.array([[1, 2, 0], [0, -2, -3]]))
 
-    msg = "Number of priors must match the number of classes"
+    msg = "The shape of error weights matrix does not match the number of classes"
+    with pytest.raises(ValueError, match=msg):
+        clf.fit(X, y)
+
+    clf = GaussianWNB(error_weights=np.array([[1, 2, 0], [0, -2, -3], [-2, 1, 1.5]]))
+    msg = "The shape of error weights matrix does not match the number of classes"
     with pytest.raises(ValueError, match=msg):
         clf.fit(X, y)
 
 
-def test_gnb_prior_greater_one():
+def test_gwnb_wrong_penalty():
     """
-    Test if an error is raised if the sum of priors greater than one.
+    Test whether an error is raised in case regularization penalty is not supported.
     """
-    clf = GeneralNB(priors=np.array([2.0, 1.0]))
+    clf = GaussianWNB(penalty="dropout")
 
-    msg = "The sum of the priors should be 1"
+    msg = "Regularization type must be either 'l1' or 'l2'"
     with pytest.raises(ValueError, match=msg):
         clf.fit(X, y)
 
 
-def test_gnb_prior_large_bias():
+def test_gwnb_neg_C():
     """
-    Test if good prediction when class priors favor largely one class.
+    Test whether an error is raised in case of negative regularization parameter, C.
     """
-    clf = GeneralNB(priors=np.array([0.01, 0.99]))
-    clf.fit(X, y)
-    assert clf.predict(np.array([[-0.1, -0.1]])) == np.array([2])
+    clf = GaussianWNB(C=-0.6)
+
+    msg = "Regularization parameter must be positive"
+    with pytest.raises(ValueError, match=msg):
+        clf.fit(X, y)
 
 
-def test_gnb_wrong_nb_dist():
+def test_gwnb_neg_max_iter():
     """
-    Test whether an error is raised if the number of distributions is different from the number of features.
+    Test whether an error is raised in case number of iteration is negative.
     """
-    clf = GeneralNB(distributions=[D.NORMAL, D.GAMMA, D.PARETO])
+    clf = GaussianWNB(max_iter=-10)
 
-    msg = "Number of specified distributions must match the number of features"
+    msg = "Maximum number of iteration must be a positive integer"
     with pytest.raises(ValueError, match=msg):
         clf.fit(X, y)
 
 
-def test_gnb_invalid_dist():
+def test_gwnb_no_cost_hist():
     """
-    Test whether an error is raised if an invalid distribution is provided.
+    Test whether cost_hist_ is None if learning_hist is not enabled.
     """
-    clf = GeneralNB(distributions=["Normal", "Borel"])
-
-    msg = "Distribution 'Borel' is not supported"
-    with pytest.raises(ValueError, match=msg):
-        clf.fit(X, y)
+    clf = GaussianWNB(max_iter=10)
+    clf.fit(X, y)
+    assert clf.cost_hist_ is None
```

### Comparing `wnb-0.1.13/wnb/_base.py` & `wnb-0.1.14/wnb/_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -89,16 +89,15 @@
             out[key] = value
         return out
 
     @property
     def support(self) -> Union[List[float], Tuple[float, float]]:
         """Returns the support of the probability distribution.
 
-        If support is a list, the support is a limited number of discrete values. If it is a tuple, it indicates a
-        limited set/range of continuous values.
+        If support is a list, it represents a limited number of discrete values. If it is a tuple, it indicates a limited or unlimited range of continuous values.
 
         """
         return self._support
 
     def _check_support(self, x):
         if (isinstance(self.support, list) and x not in self.support) or \
            (isinstance(self.support, tuple) and (x < self.support[0] or x > self.support[1])):
```

### Comparing `wnb-0.1.13/wnb/dist.py` & `wnb-0.1.14/wnb/dist.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     'LognormalDist',
     'ExponentialDist',
     'UniformDist',
     'ParetoDist',
     'GammaDist',
     'BernoulliDist',
     'CategoricalDist',
-    'MultinomialDist',
+    # 'MultinomialDist',
     'GeometricDist',
     'PoissonDist'
 ]
 
 
 class NormalDist(ContinuousDistMixin):
     name = D.NORMAL
@@ -136,57 +136,57 @@
 
     def __init__(self, p: float):
         self.p = p
         super().__init__()
 
     @classmethod
     def from_data(cls, data):
-        return cls(p=(np.array(data) == 1).sum() / len(data))
+        return cls(p=((np.array(data) == 1).sum() + 1e-10) / len(data))  # TODO: use alpha instead of 1e-10
 
     def pmf(self, x: int) -> float:
-        return 0.0 if x not in [0, 1] else self.p if x == 1 else 1 - self.p
+        return 0.0 if x not in self._support else self.p if x == 1 else 1 - self.p
 
 
 class CategoricalDist(DiscreteDistMixin):
     name = D.CATEGORICAL
 
     def __init__(self, prob: Mapping[Any, float]):
         self.prob = prob
         self._support = list(self.prob.keys())
         super().__init__()
 
     @classmethod
     def from_data(cls, data):
         values, counts = np.unique(data, return_counts=True)
-        return cls(prob={v: c/len(data) for v, c in zip(values, counts)})
+        return cls(prob={v: (c + 1e-10)/len(data) for v, c in zip(values, counts)})  # TODO: use alpha instead of 1e-10
 
     def pmf(self, x: Any) -> float:
-        return self.prob.get(x)
+        return self.prob.get(x, 0.0)
 
 
-class MultinomialDist(DiscreteDistMixin):
-    name = D.MULTINOMIAL
-
-    def __init__(self, n: int, prob: Mapping[Any, float]):
-        self.n = n
-        self.prob = prob
-        self._support = [i for i in range(self.n+1)]
-        super().__init__()
-
-    @classmethod
-    def from_data(cls, data: Sequence[int]):
-        values, counts = np.unique(data, return_counts=True)
-        return cls(n=int(np.sum(values)), prob={v: c / len(data) for v, c in zip(values, counts)})
-
-    def pmf(self, x: Sequence[int]) -> float:
-        if sum(x) != self.n:
-            return 0.0
-        else:
-            return np.math.factorial(self.n) * np.product([p**v for v, p in self.prob.items()]) / \
-                np.product([np.math.factorial(v) for v in self.prob.keys()])
+# class MultinomialDist(DiscreteDistMixin):
+#     name = D.MULTINOMIAL
+#
+#     def __init__(self, n: int, prob: Mapping[int, float]):
+#         self.n = n
+#         self.prob = prob
+#         self._support = [i for i in range(self.n+1)]
+#         super().__init__()
+#
+#     @classmethod
+#     def from_data(cls, data: Sequence[int]):
+#         values, counts = np.unique(data, return_counts=True)
+#         return cls(n=int(np.sum(values)), prob={v: c / len(data) for v, c in zip(values, counts)})
+#
+#     def pmf(self, x: Sequence[int]) -> float:
+#         if sum(x) != self.n:
+#             return 0.0
+#         else:
+#             return np.math.factorial(self.n) * np.product([self.prob.get(v, 0.0)**v for v in x]) / \
+#                 np.product([np.math.factorial(v) for v in x])
 
 
 class GeometricDist(DiscreteDistMixin):
     name = D.GEOMETRIC
     _support = (1, np.inf)
 
     def __init__(self, p: float):
@@ -217,7 +217,10 @@
         return (np.exp(-self.rate) * self.rate**x) / np.math.factorial(x)
 
 
 AllDistributions = {
     eval(cls).name: eval(cls)
     for cls in __all__
 }
+
+
+NonNumericDistributions = [D.CATEGORICAL, ]
```

### Comparing `wnb-0.1.13/wnb/gnb.py` & `wnb-0.1.14/wnb/gnb.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from sklearn.base import BaseEstimator, ClassifierMixin
 from sklearn.exceptions import DataConversionWarning
 from sklearn.utils import check_array, as_float_array
 from sklearn.utils.validation import check_is_fitted
 
 from ._base import ContinuousDistMixin, DiscreteDistMixin
 from ._enums import Distribution
-from .dist import AllDistributions
+from .dist import AllDistributions, NonNumericDistributions
 
 
 class GeneralNB(ClassifierMixin, BaseEstimator, metaclass=ABCMeta):
     """
     A general Naive Bayes classifier that allows you to specify the likelihood distribution for each feature.
     """
 
@@ -40,24 +40,31 @@
 
     def _more_tags(self):
         return {
             'multilabel': True,
             'requires_y': True
         }
 
+    def _get_distributions(self):
+        try:
+            if self.distributions_ is not None:
+                return self.distributions_
+        except:
+            return self.distributions if self.distributions is not None else []
+
     def _check_inputs(self, X, y):
         # Check if only one class is present in label vector
         if self.n_classes_ == 1:
             raise ValueError("Classifier can't train when only one class is present")
 
         X = check_array(
             array=X,
             accept_sparse=False,
             accept_large_sparse=False,
-            dtype='numeric',
+            dtype=None if any(d in self._get_distributions() for d in NonNumericDistributions) else 'numeric',
             force_all_finite=True,
             ensure_2d=True,
             ensure_min_samples=1,
             ensure_min_features=1,
             estimator=self
         )
 
@@ -72,15 +79,15 @@
             )
 
     def _prepare_X_y(self, X=None, y=None):
         if X is not None:
             # Convert to NumPy array if X is Pandas DataFrame
             if isinstance(X, pd.DataFrame):
                 X = X.values
-            X = as_float_array(X)
+            X = X if any(d in self._get_distributions() for d in NonNumericDistributions) else as_float_array(X)
 
         if y is not None:
             # Convert to a NumPy array
             if isinstance(y, pd.DataFrame) or isinstance(y, pd.Series):
                 y = y.values
             else:
                 y = np.array(y)
@@ -206,15 +213,21 @@
                         The log-probability of the samples for each class in the model.
                         The columns correspond to the classes in sorted order, as they appear in the attribute `classes_`.
         """
         # Check is fit had been called
         check_is_fitted(self)
 
         # Input validation
-        X = check_array(array=X, accept_large_sparse=False, force_all_finite=True, estimator=self)
+        X = check_array(
+            array=X,
+            accept_large_sparse=False,
+            force_all_finite=True,
+            dtype=None if any(d in self._get_distributions() for d in NonNumericDistributions) else 'numeric',
+            estimator=self
+        )
 
         # Check if the number of input features matches the data seen during fit
         if not X.shape[1] == self.n_features_in_:
             raise ValueError(
                 "Expected input with %d features, got %d instead." % (self.n_features_in_, X.shape[1])
             )
```

### Comparing `wnb-0.1.13/wnb/gwnb.py` & `wnb-0.1.14/wnb/gwnb.py`

 * *Files identical despite different names*

### Comparing `wnb-0.1.13/wnb.egg-info/PKG-INFO` & `wnb-0.1.14/wnb.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wnb
-Version: 0.1.13
+Version: 0.1.14
 Summary: Python library for the implementations of general and weighted naive Bayes (WNB) classifiers.
 Home-page: https://github.com/msamsami/weighted-naive-bayes
 Author: Mehdi Samsami
 Author-email: mehdisamsami@live.com
 Keywords: python,bayes,naivebayes,classifier,probabilistic
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
@@ -17,18 +17,20 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # WNB: General and weighted naive Bayes classifiers
 
-![](https://img.shields.io/badge/version-v0.1.13-green)
+![](https://img.shields.io/badge/version-v0.1.14-green)
 ![](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9-blue)
 ![](https://github.com/msamsami/weighted-naive-bayes/actions/workflows/python-publish.yml/badge.svg)
 [![](https://img.shields.io/pypi/v/wnb)](https://pypi.org/project/wnb/)
+![](https://img.shields.io/pypi/dm/wnb)
+
 
 <p>
 <img src="https://raw.githubusercontent.com/msamsami/weighted-naive-bayes/main/logo.png" alt="wnb logo" width="275" />
 <br>
 </p>
 
 ## Introduction
@@ -105,7 +107,18 @@
 wnb.fit(X, y)
 ```
 
 4. Predict on test data
 ```python
 wnb.predict(x_test)
 ```
+
+## Tests
+To run the tests, install development requirements:
+```
+pip install -r requirements_dev.txt
+```
+
+Then, run pytest:
+```
+pytest
+```
```

