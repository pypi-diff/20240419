# Comparing `tmp/bayte-0.1.1-py3-none-any.whl.zip` & `tmp/bayte-0.2.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,12 @@
-Zip file size: 11934 bytes, number of entries: 9
--rw-r--r--  2.0 unx      324 b- defN 22-Nov-24 20:48 bayte/__init__.py
--rw-r--r--  2.0 unx       47 b- defN 22-Nov-24 20:48 bayte/_meta.py
--rw-r--r--  2.0 unx    13622 b- defN 22-Nov-24 20:48 bayte/encoder.py
--rw-r--r--  2.0 unx    14846 b- defN 22-Nov-24 20:48 bayte/ensemble.py
--rw-r--r--  2.0 unx     1802 b- defN 22-Nov-24 20:48 bayte/plots.py
--rw-r--r--  2.0 unx     6611 b- defN 22-Nov-24 20:49 bayte-0.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Nov-24 20:49 bayte-0.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        6 b- defN 22-Nov-24 20:49 bayte-0.1.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      651 b- defN 22-Nov-24 20:49 bayte-0.1.1.dist-info/RECORD
-9 files, 38001 bytes uncompressed, 10832 bytes compressed:  71.5%
+Zip file size: 13733 bytes, number of entries: 10
+-rw-r--r--  2.0 unx      338 b- defN 24-Apr-19 18:15 bayte/__init__.py
+-rw-r--r--  2.0 unx       47 b- defN 24-Apr-19 18:15 bayte/_meta.py
+-rw-r--r--  2.0 unx    13949 b- defN 24-Apr-19 18:15 bayte/encoder.py
+-rw-r--r--  2.0 unx    15603 b- defN 24-Apr-19 18:15 bayte/ensemble.py
+-rw-r--r--  2.0 unx     2024 b- defN 24-Apr-19 18:15 bayte/plots.py
+-rw-r--r--  2.0 unx     1069 b- defN 24-Apr-19 18:16 bayte-0.2.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     7423 b- defN 24-Apr-19 18:16 bayte-0.2.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-19 18:16 bayte-0.2.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        6 b- defN 24-Apr-19 18:16 bayte-0.2.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      737 b- defN 24-Apr-19 18:16 bayte-0.2.1.dist-info/RECORD
+10 files, 41288 bytes uncompressed, 12497 bytes compressed:  69.7%
```

## zipnote {}

```diff
@@ -9,20 +9,23 @@
 
 Filename: bayte/ensemble.py
 Comment: 
 
 Filename: bayte/plots.py
 Comment: 
 
-Filename: bayte-0.1.1.dist-info/METADATA
+Filename: bayte-0.2.1.dist-info/LICENSE
 Comment: 
 
-Filename: bayte-0.1.1.dist-info/WHEEL
+Filename: bayte-0.2.1.dist-info/METADATA
 Comment: 
 
-Filename: bayte-0.1.1.dist-info/top_level.txt
+Filename: bayte-0.2.1.dist-info/WHEEL
 Comment: 
 
-Filename: bayte-0.1.1.dist-info/RECORD
+Filename: bayte-0.2.1.dist-info/top_level.txt
+Comment: 
+
+Filename: bayte-0.2.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## bayte/__init__.py

```diff
@@ -1,14 +1,13 @@
 """Import path."""
 
-from ._meta import __version__  # noqa: F401
-
 from typing import List
 
-from .encoder import BayesianTargetEncoder
-from .ensemble import BayesianTargetClassifier, BayesianTargetRegressor
+from bayte._meta import __version__  # noqa: F401
+from bayte.encoder import BayesianTargetEncoder
+from bayte.ensemble import BayesianTargetClassifier, BayesianTargetRegressor
 
 __all__: List[str] = [
-    "BayesianTargetEncoder",
     "BayesianTargetClassifier",
+    "BayesianTargetEncoder",
     "BayesianTargetRegressor",
 ]
```

## bayte/_meta.py

```diff
@@ -1,3 +1,3 @@
 """Package metadata."""
 
-__version__ = "0.1.1"
+__version__ = "0.2.1"
```

## bayte/encoder.py

```diff
@@ -1,15 +1,15 @@
 """Bayesian target encoder."""
 
 import logging
-from typing import Callable, List, Optional, Tuple, Union
+from typing import Callable, ClassVar, List, Optional, Tuple, Union
 
-from joblib import Parallel, effective_n_jobs
 import numpy as np
 import scipy.stats
+from joblib import Parallel, effective_n_jobs
 from sklearn.preprocessing._encoders import _BaseEncoder
 from sklearn.utils.fixes import delayed
 from sklearn.utils.validation import check_is_fitted
 
 LOG = logging.getLogger(__name__)
 
 
@@ -238,15 +238,15 @@
         The estimated hyperparameters for the prior distribution.
     posterior_params_ : list
         A list of lists. Each entry in the list corresponds to the categorical
         feature in ``categories_``. Each index in the nested list contains
         the parameters for the posterior distribution for the given level.
     """
 
-    _required_parameters = ["dist"]
+    _required_parameters: ClassVar[List[str]] = ["dist"]
 
     def __init__(
         self,
         dist: str,
         sample: bool = False,
         categories: Union[str, List] = "auto",
         initializer: Optional[Callable] = None,
@@ -279,16 +279,23 @@
             Target values. Will be cast to X's dtype if necessary.
 
         Returns
         -------
         self : object
             Fitted encoder.
         """
-        X, y = self._validate_data(X, y, dtype=None)
-        self._fit(X, handle_unknown=self.handle_unknown, force_all_finite=True)
+        tags = self._get_tags()
+        X, y = self._validate_data(
+            X, y, dtype=None, force_all_finite=not tags.get("allow_nan", True)
+        )
+        self._fit(
+            X,
+            handle_unknown=self.handle_unknown,
+            force_all_finite=not tags.get("allow_nan", True),
+        )
         # Initialize the prior distribution parameters
         initializer_ = self.initializer or _init_prior
         self.prior_params_ = initializer_(self.dist, y)
 
         if effective_n_jobs(self.n_jobs) == 1:
             parallel, fn = list, _update_posterior
         else:
@@ -318,18 +325,19 @@
         Returns
         -------
         ndarray
             Transformed input.
         """
         check_is_fitted(self)
 
+        tags = self._get_tags()
         X_int, X_mask = self._transform(
             X,
             handle_unknown=self.handle_unknown,
-            force_all_finite=True,
+            force_all_finite=not tags.get("allow_nan", True),
         )
 
         if effective_n_jobs(self.n_jobs) == 1:
             parallel, fn = list, _encode_level
         else:
             parallel = Parallel(n_jobs=self.n_jobs)
             fn = delayed(_encode_level)
@@ -372,18 +380,21 @@
             while len(varencoded) > 2:
                 if self.chunksize is None:
                     n_chunks = 1
                 else:
                     n_chunks = np.ceil(len(varencoded) / self.chunksize)
                 chunks = np.array_split(np.arange(len(varencoded)), n_chunks)
 
-                varencoded = list(
+                varencoded = [
                     np.ma.stack(varencoded[chunk[0] : chunk[-1] + 1], axis=2).sum(
                         axis=2
                     )
                     for chunk in chunks
-                )
+                ]
 
             combined = np.ma.stack(varencoded, axis=2).sum(axis=2)
             encoded.append(combined.data)
 
         return np.hstack(encoded)
+
+    def _more_tags(self):
+        return {"allow_nan": False}
```

## bayte/ensemble.py

```diff
@@ -1,35 +1,55 @@
 """BayesianTargetEstimator.
 
 Ensemble estimator that creates multiple models through sampling.
 """
 
-from copy import deepcopy
 import logging
-from typing import List, Optional, Union
+from copy import deepcopy
+from typing import ClassVar, List, Literal, Optional, Union
 
-from joblib import Parallel, effective_n_jobs
 import numpy as np
+from joblib import Parallel, effective_n_jobs
 from pandas.api.types import is_categorical_dtype
 from sklearn.base import (
     ClassifierMixin,
     RegressorMixin,
     clone,
     is_classifier,
 )
 from sklearn.ensemble._base import BaseEnsemble
 from sklearn.utils import check_random_state
+from sklearn.utils._available_if import available_if
 from sklearn.utils.fixes import delayed
-from sklearn.utils.metaestimators import if_delegate_has_method
 from sklearn.utils.multiclass import check_classification_targets
 from sklearn.utils.validation import check_array, check_is_fitted
 
 LOG = logging.getLogger(__name__)
 
 
+def _available_if_estimator_has(attr: str):
+    """Return a function to check if the estimator has ``attr``.
+
+    Parameters
+    ----------
+    attr : str
+        The attribute to look for.
+
+    Returns
+    -------
+    Any
+        The output of ``available_if``
+    """
+
+    def _check(self):
+        return hasattr(self.estimator, attr)
+
+    return available_if(_check)
+
+
 def _sample_and_fit(
     estimator, encoder, X, y, categorical_feature, random_state, **fit_params
 ):
     """Sample and fit the estimator.
 
     Parameters
     ----------
@@ -68,60 +88,64 @@
     This estimator will use the bayesian target encoder to encode multiple
     training datasets. The supplied estimator will be trained multiple times,
     producing ``n_estimators`` submodels. The prediction from the model will
     be an average of each submodel's output.
 
     Parameters
     ----------
-    base_estimator : object
+    estimator : object
         The base estimator from which the ensemble is built.
     encoder : BayesianTargetEncoder
         A bayesian target encoder object.
     n_estimators : int, optional (default 10)
         The number of estimators to train.
     n_jobs : int, optional (default None)
         The number of cores to run in parallel when fitting the encoder.
         ``None`` means 1 unless in a ``joblib.parallel_backend`` context.
         ``-1`` means using all processors.
     random_state : int, optional (default None)
         Random seed used for generating random seeds for sampling.
+    base_estimator : {"deprecated"}
+        Use ``estimator`` instead.
 
     Attributes
     ----------
     categorical_ : np.ndarray
         A boolean mask indicating which columns are categorical and which are continuous.
-    base_estimator_ : estimator object
+    estimator_ : estimator object
         The base estimator from which the ensemble is grown.
     estimators_ : list
         The collection of fitted base estimators.
     """
 
-    _required_parameters = ["base_estimator", "encoder"]
+    _required_parameters: ClassVar[List[str]] = ["estimator", "encoder"]
 
     def __init__(
         self,
-        base_estimator,
+        estimator,
         encoder,
         n_estimators: int = 10,
         n_jobs: Optional[int] = None,
         random_state: Optional[int] = None,
+        base_estimator: Literal["deprecated"] = "deprecated",
     ):
         """Init method."""
-        self.base_estimator = base_estimator
+        self.estimator = estimator
         self.n_estimators = n_estimators
         self.encoder = encoder
         self.n_jobs = n_jobs
         self.random_state = random_state
+        self.base_estimator = base_estimator
 
     def fit(
         self,
         X,
         y,
         categorical_feature: Union[List[str], List[int], str] = "auto",
-        **fit_params
+        **fit_params,
     ):
         """Fit the estimator.
 
         Fitting the estimator involves
 
         1. Fitting the encoder,
         2. Sampling the encoder ``n_estimators`` times,
@@ -148,23 +172,23 @@
         self
             The trained estimator.
         """
         rng = check_random_state(self.random_state)
         self.rstates_ = rng.randint(self.n_estimators * 10, size=self.n_estimators)
         # Get the categorical columns
         if hasattr(X, "columns"):
-            self.categorical_ = np.zeros(X.shape[1], dtype=bool)
+            self.categorical_: np.ndarray = np.zeros(X.shape[1], dtype=bool)
             for idx, col in enumerate(X.columns):
                 if categorical_feature == "auto":
                     if is_categorical_dtype(X[col]):
                         self.categorical_[idx] = True
                 elif col in categorical_feature:
                     self.categorical_[idx] = True
 
-        if is_classifier(self.base_estimator):
+        if is_classifier(self.estimator):
             check_classification_targets(y)
             self.classes_ = np.unique(y)
 
         X, y = self._validate_data(X, y, dtype=None)
 
         if not hasattr(self, "categorical_"):
             if categorical_feature == "auto":
@@ -196,21 +220,21 @@
         else:
             parallel = Parallel(n_jobs=self.n_jobs)
             fn = delayed(_sample_and_fit)
 
         LOG.info("Training the estimator(s).")
         self.estimators_ = parallel(
             fn(
-                clone(self.base_estimator),
+                clone(self.estimator),
                 deepcopy(self.encoder_),
                 X,
                 y,
                 self.categorical_,
                 self.rstates_[idx],
-                **fit_params
+                **fit_params,
             )
             for idx in range(self.n_estimators)
         )
 
         return self
 
 
@@ -220,36 +244,38 @@
     This estimator will use the bayesian target encoder to encode multiple
     training datasets. The supplied estimator will be trained multiple times,
     producing ``n_estimators`` submodels. The prediction from the model will
     be an average of each submodel's output.
 
     Parameters
     ----------
-    base_estimator : object
+    estimator : object
         The base estimator from which the ensemble is built.
     encoder : BayesianTargetEncoder
         A bayesian target encoder object.
     n_estimators : int, optional (default 10)
         The number of estimators to train.
     n_jobs : int, optional (default None)
         The number of cores to run in parallel when fitting the encoder.
         ``None`` means 1 unless in a ``joblib.parallel_backend`` context.
         ``-1`` means using all processors.
+    base_estimator : {"deprecated"}
+        Use ``estimator`` instead.
 
     Attributes
     ----------
     categorical_ : np.ndarray
         A boolean mask indicating which columns are categorical and which are continuous.
-    base_estimator_ : estimator object
+    estimator_ : estimator object
         The base estimator from which the ensemble is grown.
     estimators_ : list
         The collection of fitted base estimators.
     """
 
-    @if_delegate_has_method(delegate="base_estimator")
+    @_available_if_estimator_has("predict")
     def predict(self, X):
         """Call predict on the estimators.
 
         The output of this function is the average prediction from all submodels.
         The function will encode the categorical variables using the mean of the posterior
         distribution.
 
@@ -288,15 +314,15 @@
     based on majority rule voting (``voting="hard"``) or using the argmax of
     the sums of predicted probabilities (``voting="soft"``).
 
     Voting implementation from `scikit-learn <https://github.com/scikit-learn/scikit-learn/blob/e707e61d85127dae1f58e9ad2689ca2708add0a4/sklearn/ensemble/_voting.py#L148>`_  # noqa: E501
 
     Parameters
     ----------
-    base_estimator : object
+    estimator : object
         The base estimator from which the ensemble is built.
     encoder : BayesianTargetEncoder
         A bayesian target encoder object.
     n_estimators : int, optional (default 10)
         The number of estimators to train.
     voting : {"hard", "soft"}, optional (default "hard")
         If "hard", uses predicted class labels for majority rule voting.
@@ -305,45 +331,49 @@
         well-calibrated classifiers.
     n_jobs : int, optional (default None)
         The number of cores to run in parallel when fitting the encoder.
         ``None`` means 1 unless in a ``joblib.parallel_backend`` context.
         ``-1`` means using all processors.
     random_state : int, optional (default None)
         Random seed used for generating random seeds for sampling.
+    base_estimator : {"deprecated"}
+        Use ``estimator`` instead.
 
     Attributes
     ----------
     categorical_ : np.ndarray
         A boolean mask indicating which columns are categorical and which are continuous.
-    base_estimator_ : estimator object
+    estimator_ : estimator object
         The base estimator from which the ensemble is grown.
     estimators_ : list
         The collection of fitted base estimators.
     """
 
-    _required_parameters = ["base_estimator", "encoder"]
+    _required_parameters: ClassVar[List[str]] = ["estimator", "encoder"]
 
     def __init__(
         self,
-        base_estimator,
+        estimator,
         encoder,
         n_estimators: int = 10,
         voting: str = "hard",
         n_jobs: Optional[int] = None,
         random_state: Optional[int] = None,
+        base_estimator: Literal["deprecated"] = "deprecated",
     ):
         """Init method."""
-        self.base_estimator = base_estimator
+        self.estimator = estimator
         self.n_estimators = n_estimators
         self.voting = voting
         self.encoder = encoder
         self.n_jobs = n_jobs
         self.random_state = random_state
+        self.base_estimator = base_estimator
 
-    @if_delegate_has_method(delegate="base_estimator")
+    @_available_if_estimator_has("predict")
     def predict(self, X):
         """Predict class labels for X.
 
         Parameters
         ----------
         X : indexable, length (n_samples,)
             Must fulfill the assumptions of ``fit``.
@@ -378,15 +408,15 @@
             out = np.asarray(out)
             vote = np.apply_along_axis(
                 lambda x: np.argmax(np.bincount(x)), axis=0, arr=out
             )
 
         return vote
 
-    @if_delegate_has_method(delegate="base_estimator")
+    @_available_if_estimator_has("predict_proba")
     def predict_proba(self, X):
         """Call predict_proba on the estimators.
 
         The output of this function is the average prediction from all submodels.
         The function will encode the categorical variables using the mean of the posterior
         distribution.
```

## bayte/plots.py

```diff
@@ -1,54 +1,62 @@
 """Helpful visualizations for target encoding."""
 
-from typing import Dict, List
+from typing import Dict, List, Optional
 
-from matplotlib.figure import Figure
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import scipy.stats
 import seaborn as sns
-
+from matplotlib.figure import Figure
 
 DIST_MAPPING: Dict = {
     "exponential": "expon",
     "gamma": "gamma",
     "invgamma": "invgamma",
     "normal": "norm",
 }
 
+DEFAULT_CANDIDATES: List[str] = ["exponential", "gamma", "invgamma", "normal"]
+
 
 def visualize_target_dist(
     y: np.ndarray,
-    candidates: List[str] = ["exponential", "gamma", "invgamma", "normal"],
+    candidates: Optional[List[str]] = None,
 ) -> Figure:
     """Produce a histogram for the target variable with traces.
 
     This function will create a histogram of the target and
     layer traces for any compatible distribution that is also
     available for Bayesian Target Encoding.
 
     Parameters
     ----------
     y : array-like of shape (n_samples,)
         Target values.
-    candidates : list, optional (default ["exponential", "gamma", "invgamma", "normal"])
-        The candidate likelihoods to consider.
+    candidates : list, optional (default None)
+        The candidate likelihoods to consider. By default, the following distributions
+        will be visualized:
+
+        * ``exponential``,
+        * ``gamma``,
+        * ``invgamma``, and
+        * ``normal``.
 
     Returns
     -------
     Figure
         The figure object to persist or display
     """
     dflist = []
     # Clip target values above the 99th percentile of the data
     extremes = np.quantile(y, q=[0.01, 0.99])
     target = y[(y > extremes[0]) & (y < extremes[1])]
-    for label in candidates:
+    cand_ = candidates or DEFAULT_CANDIDATES
+    for label in cand_:
         params = getattr(scipy.stats, DIST_MAPPING[label]).fit(target)
         rv = getattr(scipy.stats, DIST_MAPPING[label])(*params)
         x = np.linspace(rv.ppf(0.01), rv.ppf(0.99))
         dflist.append(pd.DataFrame({"x": x, "y": rv.pdf(x), "dist": label}))
 
     tracedf = pd.concat(dflist, ignore_index=True)
```

## Comparing `bayte-0.1.1.dist-info/METADATA` & `bayte-0.2.1.dist-info/METADATA`

 * *Files 26% similar despite different names*

```diff
@@ -1,71 +1,81 @@
 Metadata-Version: 2.1
 Name: bayte
-Version: 0.1.1
+Version: 0.2.1
 Summary: Bayesian target encoding with scikit-learn and scipy
-Home-page: https://github.com/ak-gupta/bayte
-Author: Akshay Gupta
-Author-email: akgcodes@gmail.com
-License: MIT license
-Classifier: Development Status :: 3 - Alpha
+Author-email: Akshay Gupta <akgcodes@gmail.com>
+License: MIT License
+        
+        Copyright (c) 2024 Akshay Gupta
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: documentation, https://bayte.readthedocs.io/
+Project-URL: repository, https://github.com/ak-gupta/bayte
+Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
-Requires-Dist: pandas (<=1.5.2,>=1.0.0)
-Requires-Dist: scikit-learn (<=1.1.3,>=1.0.0)
+License-File: LICENSE
+Requires-Dist: pandas <=2.2.2,>=1.0.0
+Requires-Dist: scikit-learn <=1.4.2,>=1.0.0
 Provides-Extra: build
 Requires-Dist: build ; extra == 'build'
 Requires-Dist: bumpver ; extra == 'build'
 Requires-Dist: twine ; extra == 'build'
 Requires-Dist: wheel ; extra == 'build'
 Provides-Extra: dev
-Requires-Dist: build ; extra == 'dev'
-Requires-Dist: bumpver ; extra == 'dev'
-Requires-Dist: twine ; extra == 'dev'
-Requires-Dist: wheel ; extra == 'dev'
-Requires-Dist: seaborn (<=0.12.1,>=0.11.0) ; extra == 'dev'
-Requires-Dist: furo ; extra == 'dev'
-Requires-Dist: myst-nb ; extra == 'dev'
-Requires-Dist: sphinx ; extra == 'dev'
-Requires-Dist: sphinxcontrib-bibtex ; extra == 'dev'
-Requires-Dist: sphinx-tabs ; extra == 'dev'
-Requires-Dist: black ; extra == 'dev'
-Requires-Dist: flake8 ; extra == 'dev'
-Requires-Dist: mypy ; extra == 'dev'
-Requires-Dist: pip-tools ; extra == 'dev'
-Requires-Dist: pydocstyle ; extra == 'dev'
-Requires-Dist: pytest ; extra == 'dev'
-Requires-Dist: pytest-cov ; extra == 'dev'
+Requires-Dist: bayte[build] ; extra == 'dev'
+Requires-Dist: bayte[docs] ; extra == 'dev'
+Requires-Dist: bayte[experiments] ; extra == 'dev'
+Requires-Dist: bayte[plots] ; extra == 'dev'
+Requires-Dist: bayte[qa] ; extra == 'dev'
+Requires-Dist: bayte[tests] ; extra == 'dev'
 Provides-Extra: docs
 Requires-Dist: furo ; extra == 'docs'
 Requires-Dist: myst-nb ; extra == 'docs'
 Requires-Dist: sphinx ; extra == 'docs'
 Requires-Dist: sphinxcontrib-bibtex ; extra == 'docs'
 Requires-Dist: sphinx-tabs ; extra == 'docs'
 Provides-Extra: experiments
-Requires-Dist: category-encoders (==2.3.0) ; extra == 'experiments'
-Requires-Dist: lazyscribe (==0.3.0) ; extra == 'experiments'
-Requires-Dist: lightgbm (==3.3.1) ; extra == 'experiments'
-Requires-Dist: seaborn (<=0.12.1,>=0.11.0) ; extra == 'experiments'
-Requires-Dist: prefect (==0.15.10) ; extra == 'experiments'
-Requires-Dist: xgboost (==1.5.1) ; extra == 'experiments'
+Requires-Dist: category-encoders ==2.3.0 ; extra == 'experiments'
+Requires-Dist: lazyscribe ==0.3.0 ; extra == 'experiments'
+Requires-Dist: lightgbm ==3.3.1 ; extra == 'experiments'
+Requires-Dist: seaborn <=0.13.2,>=0.11.0 ; extra == 'experiments'
+Requires-Dist: prefect ==0.15.10 ; extra == 'experiments'
+Requires-Dist: xgboost ==1.5.1 ; extra == 'experiments'
 Provides-Extra: plots
-Requires-Dist: seaborn (<=0.12.1,>=0.11.0) ; extra == 'plots'
+Requires-Dist: seaborn <=0.13.2,>=0.11.0 ; extra == 'plots'
 Provides-Extra: qa
-Requires-Dist: black ; extra == 'qa'
-Requires-Dist: flake8 ; extra == 'qa'
+Requires-Dist: ruff ==0.3.7 ; extra == 'qa'
 Requires-Dist: mypy ; extra == 'qa'
 Requires-Dist: pip-tools ; extra == 'qa'
-Requires-Dist: pydocstyle ; extra == 'qa'
 Provides-Extra: tests
 Requires-Dist: pytest ; extra == 'tests'
 Requires-Dist: pytest-cov ; extra == 'tests'
 
 
 [![codecov](https://codecov.io/github/ak-gupta/bayte/branch/main/graph/badge.svg?token=S8BUVKF37O)](https://codecov.io/github/ak-gupta/bayte) [![Maintainability](https://api.codeclimate.com/v1/badges/5c0b77d0e9b8f899ee95/maintainability)](https://codeclimate.com/github/ak-gupta/bayte/maintainability) ![PyPI](https://img.shields.io/pypi/v/bayte) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/bayte) [![Documentation Status](https://readthedocs.org/projects/bayte/badge/?version=latest)](https://bayte.readthedocs.io/en/latest/?badge=latest)
```

