# Comparing `tmp/probabilistic_reconciliation-0.0.3.tar.gz` & `tmp/probabilistic_reconciliation-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "probabilistic_reconciliation-0.0.3.tar", max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `probabilistic_reconciliation-0.0.3.tar` & `probabilistic_reconciliation-0.0.4.tar`

### file list

```diff
@@ -1,10 +1,14 @@
--rw-r--r--   0        0        0    11345 2022-11-21 12:00:18.894616 probabilistic_reconciliation-0.0.3/LICENSE
--rw-r--r--   0        0        0     2169 2022-11-21 12:00:18.894616 probabilistic_reconciliation-0.0.3/README.md
--rw-r--r--   0        0        0     1661 2022-11-21 12:00:18.894616 probabilistic_reconciliation-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      304 2022-11-21 12:00:18.894616 probabilistic_reconciliation-0.0.3/reconcile/__init__.py
--rw-r--r--   0        0        0     2110 2022-11-21 12:00:18.894616 probabilistic_reconciliation-0.0.3/reconcile/data.py
--rw-r--r--   0        0        0     3793 2022-11-21 12:00:18.894616 probabilistic_reconciliation-0.0.3/reconcile/forecast.py
--rw-r--r--   0        0        0     8224 2022-11-21 12:00:18.894616 probabilistic_reconciliation-0.0.3/reconcile/grouping.py
--rw-r--r--   0        0        0     9160 2022-11-21 12:00:18.894616 probabilistic_reconciliation-0.0.3/reconcile/probabilistic_reconciliation.py
--rw-r--r--   0        0        0     3085 1970-01-01 00:00:00.000000 probabilistic_reconciliation-0.0.3/setup.py
--rw-r--r--   0        0        0     3304 1970-01-01 00:00:00.000000 probabilistic_reconciliation-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 probabilistic_reconciliation-0.0.4/Makefile
+-rw-r--r--   0        0        0     5875 2020-02-02 00:00:00.000000 probabilistic_reconciliation-0.0.4/examples/reconciliation.py
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 probabilistic_reconciliation-0.0.4/reconcile/__init__.py
+-rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 probabilistic_reconciliation-0.0.4/reconcile/conftest.py
+-rw-r--r--   0        0        0     3779 2020-02-02 00:00:00.000000 probabilistic_reconciliation-0.0.4/reconcile/forecast.py
+-rw-r--r--   0        0        0     8370 2020-02-02 00:00:00.000000 probabilistic_reconciliation-0.0.4/reconcile/grouping.py
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 probabilistic_reconciliation-0.0.4/reconcile/grouping_test.py
+-rw-r--r--   0        0        0     9172 2020-02-02 00:00:00.000000 probabilistic_reconciliation-0.0.4/reconcile/probabilistic_reconciliation.py
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 probabilistic_reconciliation-0.0.4/reconcile/reconciliation_test.py
+-rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 probabilistic_reconciliation-0.0.4/.gitignore
+-rw-r--r--   0        0        0    11345 2020-02-02 00:00:00.000000 probabilistic_reconciliation-0.0.4/LICENSE
+-rw-r--r--   0        0        0     2528 2020-02-02 00:00:00.000000 probabilistic_reconciliation-0.0.4/README.md
+-rw-r--r--   0        0        0     2255 2020-02-02 00:00:00.000000 probabilistic_reconciliation-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3469 2020-02-02 00:00:00.000000 probabilistic_reconciliation-0.0.4/PKG-INFO
```

### Comparing `probabilistic_reconciliation-0.0.3/LICENSE` & `probabilistic_reconciliation-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `probabilistic_reconciliation-0.0.3/README.md` & `probabilistic_reconciliation-0.0.4/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -17,20 +17,24 @@
 
 The package implements
 
 - methods to compute summing/aggregation matrices for grouped and hierarchical time series,
 - an abstract base forecasting class,
 - reconciliation methods for forecasts based on sampling and optimization
 
-An example application can be found in `examples/reconciliation.py`
+An example application can be found in `examples/reconciliation.py` and
+a **case study on probabilistic forecast reconciliation of stock index data**
+can be found [here](https://dirmeier.github.io/etudes/probabilistic_reconciliation.html).
 
 ## Installation
 
+Make sure to have a working `JAX` installation. Depending whether you want to use CPU/GPU/TPU,
+please follow [these instructions](https://github.com/google/jax#installation).
 
-To install from PyPI, call:
+To install the package from PyPI, call:
 
 ```bash
 pip install probabilistic-reconciliation
 ```
 
 To install the latest GitHub <RELEASE>, just call the following on the
 command line:
```

#### html2text {}

```diff
@@ -19,11 +19,16 @@
 preprint arXiv:2210.02286 (2022). 2) Panagiotelis, Anastasios, et al.
 ["Probabilistic forecast reconciliation: Properties, evaluation and score
 optimisation."](https://doi.org/10.1016/j.ejor.2022.07.040) European Journal of
 Operational Research (2022). The package implements - methods to compute
 summing/aggregation matrices for grouped and hierarchical time series, - an
 abstract base forecasting class, - reconciliation methods for forecasts based
 on sampling and optimization An example application can be found in `examples/
-reconciliation.py` ## Installation To install from PyPI, call: ```bash pip
-install probabilistic-reconciliation ``` To install the latest GitHub , just
-call the following on the command line: ```bash pip install git+https://
-github.com/dirmeier/reconcile@ ``` ## Author Simon Dirmeier sfyrbnd_@_pm_me
+reconciliation.py` and a **case study on probabilistic forecast reconciliation
+of stock index data** can be found [here](https://dirmeier.github.io/etudes/
+probabilistic_reconciliation.html). ## Installation Make sure to have a working
+`JAX` installation. Depending whether you want to use CPU/GPU/TPU, please
+follow [these instructions](https://github.com/google/jax#installation). To
+install the package from PyPI, call: ```bash pip install probabilistic-
+reconciliation ``` To install the latest GitHub , just call the following on
+the command line: ```bash pip install git+https://github.com/dirmeier/
+reconcile@ ``` ## Author Simon Dirmeier sfyrbnd_@_pm_me
```

### Comparing `probabilistic_reconciliation-0.0.3/reconcile/forecast.py` & `probabilistic_reconciliation-0.0.4/reconcile/forecast.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,28 +8,30 @@
 class Forecaster(metaclass=abc.ABCMeta):
     """
     Forecast base class
 
     Needs to be inherited for using a custom forecaster
     """
 
+    def __init__(self):
+        pass
+
     @property
     @abc.abstractmethod
     def data(self) -> Tuple[Array, Array]:
         """
         Returns the data set used for training
 
         Returns
         -------
         Tuple
             returns a tuple consisting of two chex.Arrays where the first
             element are the time series (Y), and the second element are the
             features (X)
         """
-        pass
 
     @abc.abstractmethod
     def fit(self, rng_key: PRNGKey, ys: Array, xs: Array) -> None:
         """
         Fit the forecaster to data
 
         Fit a forecaster for each base and upper time series. Can be implemented
@@ -45,15 +47,14 @@
             and the last axis (N) are measurements at different time points
         xs: chex.Array
             a (1 x P x N)-dimensional array of time points where
             the second axis (P) corresponds to the different time series
             and the last axis (N) are the time points for which measurements
             are taken
         """
-        pass
 
     @abc.abstractmethod
     def posterior_predictive(
         self, rng_key: PRNGKey, xs_test: Array
     ) -> distrax.Distribution:
         """
         Computes the posterior predictive distribution at some input points
@@ -72,15 +73,14 @@
         Returns
         -------
         distrax.Distribution
             returns a distrax Distribution with batch shape (,P) and event
             shape (,M), such that a single sample has shape (P, M) and
             multiple samples have shape (S, P, M)
         """
-        pass
 
     @abc.abstractmethod
     def predictive_posterior_probability(
         self, rng_key: PRNGKey, ys_test: Array, xs_test: Array
     ) -> Array:
         """
         Evaluates the probability of an observation
@@ -104,8 +104,7 @@
 
         Returns
         -------
         chex.Array
             returns a chex Array of size P with the log predictive probability
             of the data given a fit
         """
-        pass
```

### Comparing `probabilistic_reconciliation-0.0.3/reconcile/grouping.py` & `probabilistic_reconciliation-0.0.4/reconcile/grouping.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,18 +3,20 @@
 
 import numpy as np
 import pandas as pd
 from jax import numpy as jnp
 from scipy import sparse
 
 
+# pylint: disable=missing-function-docstring
 def as_list(maybe_list):
     return maybe_list if isinstance(maybe_list, list) else [maybe_list]
 
 
+# pylint: disable=missing-function-docstring,too-many-locals,unnecessary-comprehension  # noqa: E501
 class Grouping:
     """
     Class that represents a grouping/hierarchy of a grouped or hierarchical
     time series
     """
 
     def __init__(self, groups: pd.DataFrame):
```

### Comparing `probabilistic_reconciliation-0.0.3/reconcile/probabilistic_reconciliation.py` & `probabilistic_reconciliation-0.0.4/reconcile/probabilistic_reconciliation.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 from reconcile.forecast import Forecaster
 from reconcile.grouping import Grouping
 
 logger = logging.getLogger(__name__)
 
 
+# pylint: disable=too-many-arguments,too-many-locals,arguments-differ
 class ProbabilisticReconciliation:
     """
     Probabilistic reconcilation of hierarchical time series class
     """
 
     def __init__(self, grouping: Grouping, forecaster: Forecaster):
         self._forecaster = forecaster
@@ -78,34 +79,34 @@
             y = jnp.concatenate([u, b], axis=1)
             x = jnp.tile(xs_test, [y.shape[0], 1, 1])
             lp = self._forecaster.predictive_posterior_probability(
                 rng_key, y, x
             )
             return jnp.sum(lp)
 
+        def lp(x):
+            return _logprob_fn(**x)
+
         curr_key, rng_key = random.split(rng_key, 2)
         initial_positions = self._forecaster.posterior_predictive(
             curr_key,
             xs_test,
         ).sample(seed=rng_key, sample_shape=(n_chains,))
         initial_positions = {
             "b": self._grouping.extract_bottom_timeseries(initial_positions)
         }
 
-        curr_keys, rng_key = random.split(rng_key)
-        warmup = blackjax.window_adaptation(
-            blackjax.nuts,
-            lambda x: _logprob_fn(**x),
-            n_warmup,
-        )
-        initial_states = jax.vmap(
+        init_keys = random.split(rng_key, n_chains)
+        warmup = blackjax.window_adaptation(blackjax.nuts, lp)
+        initial_states, kernel_params = jax.vmap(
             lambda seed, param: warmup.run(seed, param)[0]
-        )(random.split(curr_keys, n_chains), initial_positions)
-        warmup_init = {"b": initial_positions["b"][0]}
-        _, kernel, _ = warmup.run(rng_key, warmup_init)
+        )(init_keys, initial_positions)
+
+        kernel_params = {k: v[0] for k, v in kernel_params.items()}
+        _, kernel = blackjax.nuts(lp, **kernel_params)
 
         def _inference_loop(rng_key, kernel, initial_state, num_samples):
             @jax.jit
             def _step(states, rng_key):
                 keys = jax.random.split(rng_key, n_chains)
                 states, infos = jax.vmap(kernel)(keys, states)
                 return states, (states, infos)
@@ -192,15 +193,15 @@
             rhs = 0.5 * jnp.linalg.norm(
                 y_reconciled_0 - y_reconciled_1, axis=2, keepdims=True
             )
             loss = jnp.mean(lhs - rhs, axis=0, keepdims=True)
             loss = jnp.sum(loss, axis=-1)
             return loss
 
-        def _step(state, epoch_key, y_batched, y_predictive_batched):
+        def _step(state, y_batched, y_predictive_batched):
             def loss_fn(params):
                 b_reconciled_pred = state.apply_fn(params, y_predictive_batched)
                 y_reconciled_pred = self._grouping.all_timeseries(
                     b_reconciled_pred
                 )
                 loss = _loss(
                     y_batched,
@@ -223,26 +224,26 @@
         tx = optax.adam(0.001)
         state = TrainState.create(apply_fn=model.apply, params=params, tx=tx)
 
         batch_size = 64
         early_stop = EarlyStopping(min_delta=0.1, patience=5)
         itr = 0
         while True:
-            sample_key, epoch_key, rng_key = random.split(rng_key, 3)
+            sample_key, rng_key = random.split(rng_key)
             y_predictive_batch = predictive.sample(
                 seed=sample_key,
                 sample_shape=(batch_size, 2),
             )
-            state, loss = _step(state, epoch_key, ys, y_predictive_batch)
+            state, loss = _step(state, ys, y_predictive_batch)
             logger.info("Loss after batch update %d", loss)
             _, early_stop = early_stop.update(loss)
             if early_stop.should_stop and n_iter is None:
                 logger.info("Met early stopping criteria, breaking...")
                 break
-            elif n_iter is not None and itr == n_iter:
+            if n_iter is not None and itr == n_iter:
                 break
             itr += 1
 
         predictive = self._forecaster.posterior_predictive(rng_key, xs_test)
         y_predictive = predictive.sample(
             seed=rng_key, sample_shape=(n_samples,)
         )
```

### Comparing `probabilistic_reconciliation-0.0.3/setup.py` & `probabilistic_reconciliation-0.0.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,72 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: probabilistic-reconciliation
+Version: 0.0.4
+Summary: Probabilistic reconciliation of time series forecasts
+Project-URL: homepage, https://github.com/dirmeier/reconcile
+Author-email: Simon Dirmeier <sfyrbnd@pm.me>
+License-Expression: Apache-2.0
+License-File: LICENSE
+Keywords: forecasting,hierarchical time series,probabilistic reconciliation,timeseries
+Classifier: Development Status :: 1 - Planning
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Requires-Python: >=3.9
+Requires-Dist: blackjax-nightly>=0.9.6.post127
+Requires-Dist: chex>=0.1.5
+Requires-Dist: distrax>=0.1.2
+Requires-Dist: flax>=0.6.1
+Requires-Dist: optax>=0.1.3
+Requires-Dist: pandas>=1.5.1
+Description-Content-Type: text/markdown
+
+# reconcile
+
+[![status](http://www.repostatus.org/badges/latest/concept.svg)](http://www.repostatus.org/#concept)
+[![ci](https://github.com/dirmeier/reconcile/actions/workflows/ci.yaml/badge.svg)](https://github.com/dirmeier/reconcile/actions/workflows/ci.yaml)
+[![codacy badge](https://app.codacy.com/project/badge/Grade/f0a254348e894c7c85b4e979bc81f1d9)](https://www.codacy.com/gh/dirmeier/reconcile/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=dirmeier/reconcile&amp;utm_campaign=Badge_Grade)
+[![codacy badge](https://app.codacy.com/project/badge/Coverage/f0a254348e894c7c85b4e979bc81f1d9)](https://www.codacy.com/gh/dirmeier/reconcile/dashboard?utm_source=github.com&utm_medium=referral&utm_content=dirmeier/reconcile&utm_campaign=Badge_Coverage)
+[![version](https://img.shields.io/pypi/v/probabilistic-reconciliation.svg?colorB=black&style=flat)](https://pypi.org/project/probabilistic-reconciliation/)
+
+> Probabilistic reconciliation of time series forecasts
+
+## About
+
+Reconcile implements probabilistic time series forecast reconciliation methods introduced in
+
+1) Zambon, Lorenzo, Dario Azzimonti, and Giorgio Corani. ["Probabilistic reconciliation of forecasts via importance sampling."](https://doi.org/10.48550/arXiv.2210.02286) arXiv preprint arXiv:2210.02286 (2022).
+2) Panagiotelis, Anastasios, et al. ["Probabilistic forecast reconciliation: Properties, evaluation and score optimisation."](https://doi.org/10.1016/j.ejor.2022.07.040) European Journal of Operational Research (2022).
+
+The package implements
+
+- methods to compute summing/aggregation matrices for grouped and hierarchical time series,
+- an abstract base forecasting class,
+- reconciliation methods for forecasts based on sampling and optimization
+
+An example application can be found in `examples/reconciliation.py` and
+a **case study on probabilistic forecast reconciliation of stock index data**
+can be found [here](https://dirmeier.github.io/etudes/probabilistic_reconciliation.html).
+
+## Installation
+
+Make sure to have a working `JAX` installation. Depending whether you want to use CPU/GPU/TPU,
+please follow [these instructions](https://github.com/google/jax#installation).
+
+To install the package from PyPI, call:
+
+```bash
+pip install probabilistic-reconciliation
+```
+
+To install the latest GitHub <RELEASE>, just call the following on the
+command line:
+
+```bash
+pip install git+https://github.com/dirmeier/reconcile@<RELEASE>
+```
 
-packages = \
-['reconcile']
+## Author
 
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['blackjax>=0.9.6,<0.10.0',
- 'chex>=0.1.5,<0.2.0',
- 'flax>=0.6.1,<0.7.0',
- 'numpy>=1.23.4,<2.0.0',
- 'optax>=0.1.3,<0.2.0',
- 'pandas>=1.5.1,<2.0.0',
- 'scipy>=1.9.3,<2.0.0',
- 'statsmodels>=0.13.2,<0.14.0']
-
-setup_kwargs = {
-    'name': 'probabilistic-reconciliation',
-    'version': '0.0.3',
-    'description': 'Probabilistic reconciliation of time series forecasts',
-    'long_description': '# reconcile\n\n[![status](http://www.repostatus.org/badges/latest/concept.svg)](http://www.repostatus.org/#concept)\n[![ci](https://github.com/dirmeier/reconcile/actions/workflows/ci.yaml/badge.svg)](https://github.com/dirmeier/reconcile/actions/workflows/ci.yaml)\n[![codacy badge](https://app.codacy.com/project/badge/Grade/f0a254348e894c7c85b4e979bc81f1d9)](https://www.codacy.com/gh/dirmeier/reconcile/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=dirmeier/reconcile&amp;utm_campaign=Badge_Grade)\n[![codacy badge](https://app.codacy.com/project/badge/Coverage/f0a254348e894c7c85b4e979bc81f1d9)](https://www.codacy.com/gh/dirmeier/reconcile/dashboard?utm_source=github.com&utm_medium=referral&utm_content=dirmeier/reconcile&utm_campaign=Badge_Coverage)\n[![version](https://img.shields.io/pypi/v/probabilistic-reconciliation.svg?colorB=black&style=flat)](https://pypi.org/project/probabilistic-reconciliation/)\n\n> Probabilistic reconciliation of time series forecasts\n\n## About\n\nReconcile implements probabilistic time series forecast reconciliation methods introduced in\n\n1) Zambon, Lorenzo, Dario Azzimonti, and Giorgio Corani. ["Probabilistic reconciliation of forecasts via importance sampling."](https://doi.org/10.48550/arXiv.2210.02286) arXiv preprint arXiv:2210.02286 (2022).\n2) Panagiotelis, Anastasios, et al. ["Probabilistic forecast reconciliation: Properties, evaluation and score optimisation."](https://doi.org/10.1016/j.ejor.2022.07.040) European Journal of Operational Research (2022).\n\nThe package implements\n\n- methods to compute summing/aggregation matrices for grouped and hierarchical time series,\n- an abstract base forecasting class,\n- reconciliation methods for forecasts based on sampling and optimization\n\nAn example application can be found in `examples/reconciliation.py`\n\n## Installation\n\n\nTo install from PyPI, call:\n\n```bash\npip install probabilistic-reconciliation\n```\n\nTo install the latest GitHub <RELEASE>, just call the following on the\ncommand line:\n\n```bash\npip install git+https://github.com/dirmeier/reconcile@<RELEASE>\n```\n\n## Author\n\nSimon Dirmeier <a href="mailto:sfyrbnd @ pm me">sfyrbnd @ pm me</a>\n',
-    'author': 'Simon Dirmeier',
-    'author_email': 'sfyrbnd@pm.me',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/dirmeier/reconcile',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.9,<3.10',
-}
-
-
-setup(**setup_kwargs)
+Simon Dirmeier <a href="mailto:sfyrbnd @ pm me">sfyrbnd @ pm me</a>
```

#### html2text {}

```diff
@@ -1,42 +1,46 @@
-# -*- coding: utf-8 -*- from setuptools import setup packages = \ ['reconcile']
-package_data = \ {'': ['*']} install_requires = \ ['blackjax>=0.9.6,<0.10.0',
-'chex>=0.1.5,<0.2.0', 'flax>=0.6.1,<0.7.0', 'numpy>=1.23.4,<2.0.0',
-'optax>=0.1.3,<0.2.0', 'pandas>=1.5.1,<2.0.0', 'scipy>=1.9.3,<2.0.0',
-'statsmodels>=0.13.2,<0.14.0'] setup_kwargs = { 'name': 'probabilistic-
-reconciliation', 'version': '0.0.3', 'description': 'Probabilistic
-reconciliation of time series forecasts', 'long_description': '# reconcile\n\n
-[![status](http://www.repostatus.org/badges/latest/concept.svg)](http://
-www.repostatus.org/#concept)\n[![ci](https://github.com/dirmeier/reconcile/
-actions/workflows/ci.yaml/badge.svg)](https://github.com/dirmeier/reconcile/
-actions/workflows/ci.yaml)\n[![codacy badge](https://app.codacy.com/project/
-badge/Grade/f0a254348e894c7c85b4e979bc81f1d9)](https://www.codacy.com/gh/
-dirmeier/reconcile/
+Metadata-Version: 2.1 Name: probabilistic-reconciliation Version: 0.0.4
+Summary: Probabilistic reconciliation of time series forecasts Project-URL:
+homepage, https://github.com/dirmeier/reconcile Author-email: Simon Dirmeier
+pm.me> License-Expression: Apache-2.0 License-File: LICENSE Keywords:
+forecasting,hierarchical time series,probabilistic reconciliation,timeseries
+Classifier: Development Status :: 1 - Planning Classifier: Intended Audience ::
+Science/Research Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Requires-Python: >=3.9 Requires-Dist: blackjax-nightly>=0.9.6.post127 Requires-
+Dist: chex>=0.1.5 Requires-Dist: distrax>=0.1.2 Requires-Dist: flax>=0.6.1
+Requires-Dist: optax>=0.1.3 Requires-Dist: pandas>=1.5.1 Description-Content-
+Type: text/markdown # reconcile [![status](http://www.repostatus.org/badges/
+latest/concept.svg)](http://www.repostatus.org/#concept) [![ci](https://
+github.com/dirmeier/reconcile/actions/workflows/ci.yaml/badge.svg)](https://
+github.com/dirmeier/reconcile/actions/workflows/ci.yaml) [![codacy badge]
+(https://app.codacy.com/project/badge/Grade/f0a254348e894c7c85b4e979bc81f1d9)]
+(https://www.codacy.com/gh/dirmeier/reconcile/
 dashboard?utm_source=github.com&utm_medium=referral&utm_content=dirmeier/
-reconcile&utm_campaign=Badge_Grade)\n[![codacy badge](https://app.codacy.com/
+reconcile&utm_campaign=Badge_Grade) [![codacy badge](https://app.codacy.com/
 project/badge/Coverage/f0a254348e894c7c85b4e979bc81f1d9)](https://
 www.codacy.com/gh/dirmeier/reconcile/
 dashboard?utm_source=github.com&utm_medium=referral&utm_content=dirmeier/
-reconcile&utm_campaign=Badge_Coverage)\n[![version](https://img.shields.io/
-pypi/v/probabilistic-reconciliation.svg?colorB=black&style=flat)](https://
-pypi.org/project/probabilistic-reconciliation/)\n\n> Probabilistic
-reconciliation of time series forecasts\n\n## About\n\nReconcile implements
-probabilistic time series forecast reconciliation methods introduced in\n\n1)
-Zambon, Lorenzo, Dario Azzimonti, and Giorgio Corani. ["Probabilistic
-reconciliation of forecasts via importance sampling."](https://doi.org/
-10.48550/arXiv.2210.02286) arXiv preprint arXiv:2210.02286 (2022).\n2)
-Panagiotelis, Anastasios, et al. ["Probabilistic forecast reconciliation:
-Properties, evaluation and score optimisation."](https://doi.org/10.1016/
-j.ejor.2022.07.040) European Journal of Operational Research (2022).\n\nThe
-package implements\n\n- methods to compute summing/aggregation matrices for
-grouped and hierarchical time series,\n- an abstract base forecasting class,\n-
-reconciliation methods for forecasts based on sampling and optimization\n\nAn
-example application can be found in `examples/reconciliation.py`\n\n##
-Installation\n\n\nTo install from PyPI, call:\n\n```bash\npip install
-probabilistic-reconciliation\n```\n\nTo install the latest GitHub , just call
-the following on the\ncommand line:\n\n```bash\npip install git+https://
-github.com/dirmeier/reconcile@\n```\n\n## Author\n\nSimon Dirmeier sfyrbnd_@_pm
-me\n', 'author': 'Simon Dirmeier', 'author_email': 'sfyrbnd@pm.me',
-'maintainer': 'None', 'maintainer_email': 'None', 'url': 'https://github.com/
-dirmeier/reconcile', 'packages': packages, 'package_data': package_data,
-'install_requires': install_requires, 'python_requires': '>=3.9,<3.10', } setup
-(**setup_kwargs)
+reconcile&utm_campaign=Badge_Coverage) [![version](https://img.shields.io/pypi/
+v/probabilistic-reconciliation.svg?colorB=black&style=flat)](https://pypi.org/
+project/probabilistic-reconciliation/) > Probabilistic reconciliation of time
+series forecasts ## About Reconcile implements probabilistic time series
+forecast reconciliation methods introduced in 1) Zambon, Lorenzo, Dario
+Azzimonti, and Giorgio Corani. ["Probabilistic reconciliation of forecasts via
+importance sampling."](https://doi.org/10.48550/arXiv.2210.02286) arXiv
+preprint arXiv:2210.02286 (2022). 2) Panagiotelis, Anastasios, et al.
+["Probabilistic forecast reconciliation: Properties, evaluation and score
+optimisation."](https://doi.org/10.1016/j.ejor.2022.07.040) European Journal of
+Operational Research (2022). The package implements - methods to compute
+summing/aggregation matrices for grouped and hierarchical time series, - an
+abstract base forecasting class, - reconciliation methods for forecasts based
+on sampling and optimization An example application can be found in `examples/
+reconciliation.py` and a **case study on probabilistic forecast reconciliation
+of stock index data** can be found [here](https://dirmeier.github.io/etudes/
+probabilistic_reconciliation.html). ## Installation Make sure to have a working
+`JAX` installation. Depending whether you want to use CPU/GPU/TPU, please
+follow [these instructions](https://github.com/google/jax#installation). To
+install the package from PyPI, call: ```bash pip install probabilistic-
+reconciliation ``` To install the latest GitHub , just call the following on
+the command line: ```bash pip install git+https://github.com/dirmeier/
+reconcile@ ``` ## Author Simon Dirmeier sfyrbnd_@_pm_me
```

