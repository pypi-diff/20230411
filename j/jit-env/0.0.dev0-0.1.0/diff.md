# Comparing `tmp/jit_env-0.0.dev0.tar.gz` & `tmp/jit_env-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jit_env-0.0.dev0.tar", last modified: Fri Apr  7 12:23:25 2023, max compression
+gzip compressed data, was "dist/jit_env-0.1.0.tar", last modified: Tue Apr 11 07:42:30 2023, max compression
```

## Comparing `jit_env-0.0.dev0.tar` & `jit_env-0.1.0.tar`

### file list

```diff
@@ -1,23 +1,26 @@
-drwxrwxrwx   0 joery     (1000) joery     (1000)        0 2023-04-07 12:23:25.237675 jit_env-0.0.dev0/
--rwxrwxrwx   0 joery     (1000) joery     (1000)     1062 2023-04-07 11:59:34.000000 jit_env-0.0.dev0/LICENSE
--rwxrwxrwx   0 joery     (1000) joery     (1000)     4210 2023-04-07 12:23:25.232395 jit_env-0.0.dev0/PKG-INFO
--rwxrwxrwx   0 joery     (1000) joery     (1000)     3303 2023-04-07 12:23:04.000000 jit_env-0.0.dev0/README.md
-drwxrwxrwx   0 joery     (1000) joery     (1000)        0 2023-04-07 12:23:24.974057 jit_env-0.0.dev0/jit_env/
--rwxrwxrwx   0 joery     (1000) joery     (1000)     1057 2023-04-07 09:34:23.000000 jit_env-0.0.dev0/jit_env/__init__.py
--rwxrwxrwx   0 joery     (1000) joery     (1000)    12005 2023-04-07 11:20:13.000000 jit_env-0.0.dev0/jit_env/_core.py
--rwxrwxrwx   0 joery     (1000) joery     (1000)        0 2023-04-07 12:08:12.000000 jit_env-0.0.dev0/jit_env/_test_compat.py
--rwxrwxrwx   0 joery     (1000) joery     (1000)        0 2023-04-07 12:08:04.000000 jit_env-0.0.dev0/jit_env/_test_core.py
--rwxrwxrwx   0 joery     (1000) joery     (1000)        0 2023-04-07 12:08:21.000000 jit_env-0.0.dev0/jit_env/_test_specs.py
--rwxrwxrwx   0 joery     (1000) joery     (1000)        0 2023-04-07 12:08:29.000000 jit_env-0.0.dev0/jit_env/_test_wrappers.py
--rwxrwxrwx   0 joery     (1000) joery     (1000)     3034 2023-04-07 11:05:25.000000 jit_env-0.0.dev0/jit_env/compat.py
--rwxrwxrwx   0 joery     (1000) joery     (1000)    19547 2023-04-07 11:54:04.000000 jit_env-0.0.dev0/jit_env/specs.py
--rwxrwxrwx   0 joery     (1000) joery     (1000)      306 2023-04-07 12:13:38.000000 jit_env-0.0.dev0/jit_env/version.py
--rwxrwxrwx   0 joery     (1000) joery     (1000)    12441 2023-04-07 10:04:53.000000 jit_env-0.0.dev0/jit_env/wrappers.py
-drwxrwxrwx   0 joery     (1000) joery     (1000)        0 2023-04-07 12:23:25.176192 jit_env-0.0.dev0/jit_env.egg-info/
--rwxrwxrwx   0 joery     (1000) joery     (1000)     4210 2023-04-07 12:23:23.000000 jit_env-0.0.dev0/jit_env.egg-info/PKG-INFO
--rwxrwxrwx   0 joery     (1000) joery     (1000)      386 2023-04-07 12:23:23.000000 jit_env-0.0.dev0/jit_env.egg-info/SOURCES.txt
--rwxrwxrwx   0 joery     (1000) joery     (1000)        1 2023-04-07 12:23:23.000000 jit_env-0.0.dev0/jit_env.egg-info/dependency_links.txt
--rwxrwxrwx   0 joery     (1000) joery     (1000)      101 2023-04-07 12:23:23.000000 jit_env-0.0.dev0/jit_env.egg-info/requires.txt
--rwxrwxrwx   0 joery     (1000) joery     (1000)        8 2023-04-07 12:23:23.000000 jit_env-0.0.dev0/jit_env.egg-info/top_level.txt
--rwxrwxrwx   0 joery     (1000) joery     (1000)       38 2023-04-07 12:23:25.239744 jit_env-0.0.dev0/setup.cfg
--rwxrwxrwx   0 joery     (1000) joery     (1000)     1902 2023-04-07 12:09:57.000000 jit_env-0.0.dev0/setup.py
+drwxrwxrwx   0 joery     (1000) joery     (1000)        0 2023-04-11 07:42:28.458306 jit_env-0.1.0/
+-rwxrwxrwx   0 joery     (1000) joery     (1000)     1062 2023-04-07 11:59:34.000000 jit_env-0.1.0/LICENSE
+-rwxrwxrwx   0 joery     (1000) joery     (1000)       29 2023-04-10 08:18:00.000000 jit_env-0.1.0/MANIFEST.in
+-rwxrwxrwx   0 joery     (1000) joery     (1000)     5573 2023-04-11 07:42:28.458306 jit_env-0.1.0/PKG-INFO
+-rwxrwxrwx   0 joery     (1000) joery     (1000)     4739 2023-04-11 07:42:07.000000 jit_env-0.1.0/README.md
+drwxrwxrwx   0 joery     (1000) joery     (1000)        0 2023-04-11 07:42:28.373406 jit_env-0.1.0/jit_env/
+-rwxrwxrwx   0 joery     (1000) joery     (1000)     1057 2023-04-07 09:34:23.000000 jit_env-0.1.0/jit_env/__init__.py
+-rwxrwxrwx   0 joery     (1000) joery     (1000)     4215 2023-04-11 07:18:45.000000 jit_env-0.1.0/jit_env/_compat_test.py
+-rwxrwxrwx   0 joery     (1000) joery     (1000)    13334 2023-04-11 06:27:58.000000 jit_env-0.1.0/jit_env/_core.py
+-rwxrwxrwx   0 joery     (1000) joery     (1000)     9289 2023-04-11 07:13:02.000000 jit_env-0.1.0/jit_env/_core_test.py
+-rwxrwxrwx   0 joery     (1000) joery     (1000)    16484 2023-04-10 12:51:38.000000 jit_env-0.1.0/jit_env/_specs_test.py
+-rwxrwxrwx   0 joery     (1000) joery     (1000)    11689 2023-04-11 06:25:55.000000 jit_env-0.1.0/jit_env/_wrappers_test.py
+-rwxrwxrwx   0 joery     (1000) joery     (1000)     4532 2023-04-11 07:17:00.000000 jit_env-0.1.0/jit_env/compat.py
+-rwxrwxrwx   0 joery     (1000) joery     (1000)    23230 2023-04-10 13:11:26.000000 jit_env-0.1.0/jit_env/specs.py
+-rwxrwxrwx   0 joery     (1000) joery     (1000)      304 2023-04-11 07:41:44.000000 jit_env-0.1.0/jit_env/version.py
+-rwxrwxrwx   0 joery     (1000) joery     (1000)    13538 2023-04-10 14:43:14.000000 jit_env-0.1.0/jit_env/wrappers.py
+drwxrwxrwx   0 joery     (1000) joery     (1000)        0 2023-04-11 07:42:28.443133 jit_env-0.1.0/jit_env.egg-info/
+-rwxrwxrwx   0 joery     (1000) joery     (1000)     5573 2023-04-11 07:42:27.000000 jit_env-0.1.0/jit_env.egg-info/PKG-INFO
+-rwxrwxrwx   0 joery     (1000) joery     (1000)      436 2023-04-11 07:42:27.000000 jit_env-0.1.0/jit_env.egg-info/SOURCES.txt
+-rwxrwxrwx   0 joery     (1000) joery     (1000)        1 2023-04-11 07:42:27.000000 jit_env-0.1.0/jit_env.egg-info/dependency_links.txt
+-rwxrwxrwx   0 joery     (1000) joery     (1000)      157 2023-04-11 07:42:27.000000 jit_env-0.1.0/jit_env.egg-info/requires.txt
+-rwxrwxrwx   0 joery     (1000) joery     (1000)        8 2023-04-11 07:42:27.000000 jit_env-0.1.0/jit_env.egg-info/top_level.txt
+-rwxrwxrwx   0 joery     (1000) joery     (1000)       44 2023-04-08 05:46:44.000000 jit_env-0.1.0/requirements.txt
+-rwxrwxrwx   0 joery     (1000) joery     (1000)      115 2023-04-10 08:18:00.000000 jit_env-0.1.0/requirements_dev.txt
+-rwxrwxrwx   0 joery     (1000) joery     (1000)       38 2023-04-11 07:42:28.458306 jit_env-0.1.0/setup.cfg
+-rwxrwxrwx   0 joery     (1000) joery     (1000)     1840 2023-04-10 08:18:00.000000 jit_env-0.1.0/setup.py
```

### Comparing `jit_env-0.0.dev0/LICENSE` & `jit_env-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jit_env-0.0.dev0/PKG-INFO` & `jit_env-0.1.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,96 +1,106 @@
 Metadata-Version: 2.1
 Name: jit_env
-Version: 0.0.dev0
+Version: 0.1.0
 Summary: A Jax interface for Reinforcement Learning environments.
 Home-page: https://github.com/joeryjoery/jit_env
 Author: Joery A. de Vries
 Author-email: J.A.deVries@tudelft.nl
 License: MIT
 Keywords: reinforcement-learning python machine learning jax
-Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Testing :: Mocking
 Classifier: Topic :: Software Development :: Testing :: Unit
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
+![Run Tox Tests](https://github.com/joeryjoery/jit_env/actions/workflows/tests.yml/badge.svg)
+![Python Version](https://img.shields.io/badge/Python-3.9%20%7C%203.10%20%7C%203.11-blue)
+![Package Version](https://img.shields.io/badge/jit__env-0.1.0-blue)
 # `jit_env`: A Jax Compatible RL Environment API
 `jit_env` is a library that aims to adhere closely to the `dm_env` interface
-while allowing for `Jax` transformations inside Environment implementations
+while allowing for `jax` transformations inside Environment implementations
 and defining clear type annotations.
 
 Like `dm_env` our API consists of the main components:
 
 - `jit_env.Environment`: An abstract base class for RL environments.
 - `jit_env.TimeStep`: A container class representing the outputs of the environment on each time step (transition).
 - `jit_env.specs`: A module containing primitives that are used to describe the format of the actions consumed by an environment, as well as the observations, rewards, and discounts it returns.
-- TODO: Testing is not yet implemented.
 
 This is extended with the components:
 - `jit_env.Wrapper`: An interface built on top of Environment that allows modular transformations of the base Environment.
 - `jit_env.Action, jit_env.Observation, jit_env.State`: Explicit types that concern Agent-Environment IO.
 - `jit_env.compat`: A Module containing API hooks to other Agent-Environment interfaces like `dm_env` or `gymnasium`.
 - `jit_env.wrappers`: A Module containing a few generally useful implementations for `Wrapper` (that simultaneously serves as a reference).
 
 Note that this module is only an interface and does not implement any
-Environments itself.
+Environments itself. The implementations in `examples` serve to illustrate the syntax.
+For a more thorough review of the semantics, please refer to the [dm-env](https://github.com/deepmind/dm_env/blob/master/dm_env/specs.py) 
+wiki and compare our implementation of `jit_env.Environment` with `dm_env.Environment` and the conversion as given in [`compat.py`](https://github.com/joeryjoery/jit_env/blob/main/jit_env/compat.py).
 
-## The Big Difference
+## Installation
+`jit_env` can be installed with:
+
+`python -m pip install jit-env`
+
+You can also install it directly from our GitHub repository using pip:
+
+`python -m pip install git+git://github.com/joeryjoery/jit_env.git`
+
+or alternatively by checking out a local copy of our repository and running:
+
+`python -m pip install /path/to/local/jit_env/`
+
+## The Big Difference with `dm_env`
 The main difference between this API and the standard `dm_env` API is
 that our definition of `jit_env.Environment` is functionally pure.
 This allows the the logic to e.g., be batched over or accelerated 
 using `jax.vmap` or `jax.jit`. 
 
 On top of that, we extend the `specs` logic of what `dm_env` provides.
 The `specs` module defines primitive for how the Agent interacts with 
 the Environment. We explicitly implement additional specs that are 
 compatible with `jax` based `PyTree` objects.
 This allows for tree-based operations on the `spec` objects themselves, 
 which in turn gives some added flexibility in designing desired 
 state-action spaces.
 
-## Installation
-`jit_env` can be installed with:
+Some other modified behaviours include: 
+ - `restart` providing a reference value for reward and discount in place of `None`
+ - `StepType` is no longer an `enum` type as `jax.jit` would type convert `enum` types to jax primitives anyway. It remains a namespace for defining episode boundaries.
+ - `TimeStep` is now a frozen `chex.dataclass` to allow usage of `replace` within the public API (which is private for `NamedTuple`).
+ - `TimeStep` carries an additional `extras` field to carry optional data (metrics) not shown to the agent.
+ - all helper `restart`, `transition`, etc., now take a `shape` value to generate the reference `reward` or `discount` fields.
 
-`python -m pip install jit-env`
-
-You can also install it directly from our GitHub repository using pip:
-
-`python -m pip install git+git://github.com/joeryjoery/jit_env.git`
-
-or alternatively by checking out a local copy of our repository and running:
+### Why `jit_env`
+I developed this module to have a reliable Environment backend that is less subject
+to refactoring changes as other libraries while providing free compatibility to both `jax` 
+transforms as well as any other popular type of Agent-Environment interface. 
 
-`python -m pip install /path/to/local/jit_env/`
+The hope is that this library will not require much maintenance/ alterations 
+(aside from some type-hint updates) after an official 1.0.0 release. 
 
 ## Cite us
 If you are a particularly nice person and this work was useful to you, you can
 cite this repository as:
-```
+```bibtex
 @misc{jit_env_2023,
   author={Joery A. de Vries},
   title={jit\_env: A Jax interface for reinforcement learning environments},
   year={2023},
   url={http://github.com/joeryjoery/jit_env}
 }
 ```
 
 ## References
 This library was heavily inspired by the following libraries:
 - dm-env: [https://github.com/deepmind/dm_env](https://github.com/deepmind/dm_env)
 - jumanji: [https://github.com/instadeepai/jumanji](https://github.com/instadeepai/jumanji)
 - gymnax: [https://github.com/RobertTLange/gymnax](https://github.com/RobertTLange/gymnax)
-
-I developed this module to have a reliable Environment backend that is less subject
-to refactoring changes as these other libraries. The hope is that this library
-will not require much maintenance/ alterations at all (aside from some type-hint updates) 
-after an official 1.0.0 release.
-
-
```

### Comparing `jit_env-0.0.dev0/jit_env/__init__.py` & `jit_env-0.1.0/jit_env/__init__.py`

 * *Files identical despite different names*

### Comparing `jit_env-0.0.dev0/jit_env/_core.py` & `jit_env-0.1.0/jit_env/_core.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,21 +6,23 @@
     - An interface for composing Environment Logic
     - Helper functions to initialize Types communicated to the Agent.
 """
 from __future__ import annotations
 import abc
 
 from typing import Any, TYPE_CHECKING, TypeVar, Generic, Sequence, Protocol
+from dataclasses import field
 
-if TYPE_CHECKING:  # https://github.com/python/mypy/issues/6239
+if TYPE_CHECKING:  # pragma: no cover
+    # See: https://github.com/python/mypy/issues/6239
     from dataclasses import dataclass
 else:
     from chex import dataclass
 
-from jaxtyping import Bool, Array, PyTree, Num, Int8
+from jaxtyping import Array, ArrayLike, PyTree, Num, Int8, Bool
 
 import jax
 import jax.numpy as jnp
 
 from jit_env import specs
 
 
@@ -35,29 +37,35 @@
     `step` function, as this could be changed arbitrarily by the caller.
     In turn, this leads to un-reproducible behaviour.
     """
     key: jax.random.KeyArray
 
 
 # The following should all be valid Jax types
+Action = TypeVar("Action")
 Observation = TypeVar("Observation")
 State = TypeVar("State", bound="StateProtocol")
-Action = TypeVar("Action")
 
 
 class StepType:
     """Defines the status of a `TimeStep` within a sequence."""
     FIRST: Int8[Array, ''] = jnp.array(0, jnp.int8)
     MID: Int8[Array, ''] = jnp.array(1, jnp.int8)
     LAST: Int8[Array, ''] = jnp.array(2, jnp.int8)
 
 
-@dataclass
+@dataclass(init=True, repr=True, eq=True, frozen=True)
 class TimeStep(Generic[Observation]):
-    """Defines the datastructure that is communicated to the Agent
+    """Defines the datastructure that is communicated to the Agent.
+
+    While dm_env utilizes a NamedTuple, we opted for a mappable dataclass
+    to allow for modular transformations using `dataclasses.replace`, which
+    is a private method for `NamedTuple` types. To avoid mutability confusion
+    this dataclass is made `frozen`, fields can only be "modified" by creating
+    new objects of this Type.
 
     Like in dm_env, `env.reset` will generate a `TimeStep` with step_type set
     to `StepType.FIRST`. If `env.step` terminates the episode, step_type is
     set to `StepType.LAST`. Otherwise, step_type is set to `StepType.MID`.
 
     Attributes:
         step_type:
@@ -70,20 +78,21 @@
             Generic Jax-Compatible data-structure that the agent observes to
             compute new actions.
         extras:
             Optional data that is typically not communicated to the Agent
             but allows the user to track certain loss-metrics, accuracies,
             or other information. This can be stored in a Replay Buffer for
             training or for generally monitorring Agent behaviour.
+            This field is excluded from object comparisons.
     """
     step_type: Int8[Array, '']
-    reward: PyTree[Num[Array, '...']]
-    discount: PyTree[Num[Array, '...']]
+    reward: PyTree[ArrayLike]
+    discount: PyTree[ArrayLike]
     observation: Observation
-    extras: dict[str, Any] | None = None
+    extras: dict[str, Any] | None = field(default=None, compare=False)
 
     def first(self) -> Bool[Array, '']:
         """Proxy function to check if step was generated by `reset`."""
         return self.step_type == StepType.FIRST
 
     def mid(self) -> Bool[Array, '']:
         """Proxy function to check if step was generated during an episode."""
@@ -101,15 +110,15 @@
 
     def __str__(self) -> str:
         """Returns a minimal representation of the Environment Structure."""
         return self.__class__.__name__
 
     def __repr__(self) -> str:
         """Returns a complete informative representation of self."""
-        return super().__repr__()
+        return self.__str__()
 
     @property
     def unwrapped(self) -> Environment:
         """Helper function to support unpacking Composite Environments."""
         return self
 
     @abc.abstractmethod
@@ -211,16 +220,30 @@
         or via a context manager::
 
             with Env(...) as env:
               # Use env.
         """
 
     def render(self, state: State) -> Any:
-        """Generate a pixel-observation based on the given state. """
-        raise NotImplementedError("Render Function not Implemented")
+        """Generate a pixel-observation based on the given state.
+
+        This method is not annotated as abstract as implementing a render
+        is not neccesary to perform experiments. However it will raise
+        an Error if called without an implementation.
+
+        Args:
+            state: A state object to generate a visualization of.
+
+        Raises:
+            NotImplementedError:
+                If subclass does not implement this method.
+         """
+        raise NotImplementedError(  # pragma: no cover
+            "Render Function not Implemented"
+        )
 
     def __enter__(self) -> Environment:
         """Allows the environment to be used in a with-statement context."""
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         """Allows the environment to be used in a with-statement context."""
@@ -234,28 +257,31 @@
     metaclass=abc.ABCMeta
 ):
     """Interface for Composing Environment logic for RL-Agents. """
 
     def __init__(self, env: Environment):
         """Initializes the Composite Environment with a base Environment.
 
+        The `env` attribute can be accessed for reading out attributes, but it
+        should not be modified.
+
         Args:
             env: The base environment to extend with functionality.
         """
         super().__init__()
-        self.env = env
+        self._env = env
 
     def __str__(self) -> str:
         """Returns a recursive composition structure of all Wrappers."""
         return f"{self.__class__.__name__}({str(self.env)})"
 
-    def __getattr__(self, item: str) -> Any:
-        if item == "__setstate__":
-            raise AttributeError(item)
-        return getattr(self.env, item)
+    @property
+    def env(self):
+        """Helper function to unpack Composite Environments by one level."""
+        return self._env
 
     @property
     def unwrapped(self) -> Environment:
         """Helper function to unpack Composite Environments to the base."""
         return self.env.unwrapped
 
     def reset(self, key: jax.random.KeyArray) -> tuple[State, TimeStep]:
@@ -277,73 +303,77 @@
         return self.env.action_spec()
 
     def render(self, state: State) -> Any:
         return self.env.render(state)
 
 
 # Define helpers to instantiate TimeStep objects at Environment boundaries
+# Note that these helpers are not expected to conform to any Spec.
 
 def restart(
-    observation: Observation,
-    extras: dict | None = None,
-    shape: int | Sequence[int] = ()
+        observation: Observation,
+        extras: dict | None = None,
+        shape: int | Sequence[int] = (),
+        dtype: Any = float
 ) -> TimeStep:
-    """Returns a `TimeStep` with `step_type` set to `StepType.FIRST`. """
+    """Returns a `TimeStep` with `step_type` set to `StepType.FIRST`.
+
+    Unlike dm_env the reward and discount are not `None` to prevent array
+    shape inconsistensies when scanning over environments.
+    """
     return TimeStep(
         step_type=StepType.FIRST,
-        reward=jnp.zeros(shape, dtype=float),
+        reward=jnp.zeros(shape, dtype=dtype),
         discount=jnp.ones(shape, dtype=float),
         observation=observation,
         extras=extras,
     )
 
 
 def transition(
-    reward: PyTree[Num[Array, '...']],
-    observation: Observation,
-    discount: PyTree[Num[Array, '...']] | None = None,
-    extras: dict | None = None,
-    shape: int | Sequence[int] = ()
+        reward: PyTree[Num[Array, '...']],
+        observation: Observation,
+        discount: PyTree[Num[Array, '...']] | None = None,
+        extras: dict | None = None,
+        shape: int | Sequence[int] = ()
 ) -> TimeStep:
     """Returns a `TimeStep` with `step_type` set to `StepType.MID`. """
-    discount = jnp.ones(shape, jnp.float32) if discount is None else discount
     return TimeStep(
         step_type=StepType.MID,
         reward=reward,
-        discount=discount,
+        discount=(jnp.ones(shape, float) if discount is None else discount),
         observation=observation,
         extras=extras,
     )
 
 
 def termination(
-    reward: PyTree[Num[Array, '...']],
-    observation: Observation,
-    extras: dict | None = None,
-    shape: int | Sequence[int] = ()
+        reward: PyTree[Num[Array, '...']],
+        observation: Observation,
+        extras: dict | None = None,
+        shape: int | Sequence[int] = ()
 ) -> TimeStep:
     """Returns a `TimeStep` with `step_type` set to `StepType.LAST`. """
     return TimeStep(
         step_type=StepType.LAST,
         reward=reward,
         discount=jnp.zeros(shape, dtype=float),
         observation=observation,
         extras=extras,
     )
 
 
 def truncation(
-    reward: PyTree[Num[Array, '...']],
-    observation: Observation,
-    discount: PyTree[Num[Array, '...']] | None = None,
-    extras: dict | None = None,
-    shape: int | Sequence[int] = ()
+        reward: PyTree[Num[Array, '...']],
+        observation: Observation,
+        discount: PyTree[Num[Array, '...']] | None = None,
+        extras: dict | None = None,
+        shape: int | Sequence[int] = ()
 ) -> TimeStep:
     """Alternative to `termination` that does not set `discount` to zero. """
-    discount = jnp.ones(shape, jnp.float32) if discount is None else discount
     return TimeStep(
         step_type=StepType.LAST,
         reward=reward,
-        discount=discount,
+        discount=(jnp.ones(shape, float) if discount is None else discount),
         observation=observation,
         extras=extras,
     )
```

### Comparing `jit_env-0.0.dev0/jit_env/specs.py` & `jit_env-0.1.0/jit_env/specs.py`

 * *Files 13% similar despite different names*

```diff
@@ -17,80 +17,158 @@
 
     from jit_env.specs import Array
     a = Array(...)  # Can cause namespace clashes
 
 The basic Spec types defined in this Module were adapted from:
  - Jumanji: https://github.com/instadeepai/jumanji
 
+Our implementation of `validate` and `generate_value` are compatible with
+typical `jax` transformations like `jax.vmap` or `jax.jit`.
 """
 from __future__ import annotations as _annotations
 import abc as _abc
 import functools as _functools
 import inspect as _inspect
 import typing as _typing
 import typing_extensions as _type_ext
 
 import jaxtyping as _jxtype
 
 import jax as _jax
 from jax import numpy as _jnp
 from jax import tree_util as _tree_util
 
+import jit_env
 
 _T = _typing.TypeVar("_T")
 
 
-class Spec(_abc.ABC, _typing.Generic[_T]):
+class Spec(_typing.Generic[_T], metaclass=_abc.ABCMeta):
     """Interface for defining datastructure Specifications.
 
     This type is meant to 'Specify' a datastructure's shapes, types, and
     general structure without needing to instantiate said structure.
+
+    We copy the `__slots__` implementation from `dm_env` with read-only
+    properties to enforce that `specs` cannot be modified at runtime.
+
+    Notes
+        Specs are not composable with jax transformations.
     """
+    __slots__ = ('_name',)
 
     def __init__(self, name: str = ""):
         """Initialize a Spec by requiring an explicit naming.
 
         Args:
             name: Explicit string name for the datastructure specification.
         """
-        self.name = name
+        self._name = name
+
+    @property
+    def name(self) -> str:
+        return self._name
+
+    def __repr__(self) -> str:
+        """Return a string representation of the full Specification.
+
+        All __slot__ attributes are collected within the Spec's inheritance
+        chain and string concatenated top-to-bottom : left-to-right.
+
+        In other words, this method gives: 'Name(slots_top, slots_lower, ...)'
+        """
+        # iterator over ((slot_self_a, ...), (slot_super_a, ...), ...)
+        slots = (getattr(cls, '__slots__', ()) for cls in type(self).__mro__)
 
-    def __str__(self) -> str:
-        """Return a string representation of the full Specification."""
-        return f"{self.__class__.__name__}(name={self.name})"
+        reverse_ordered, seen = list(), set()
+        for s in slots:
+            if s and (s not in seen):
+                seen.add(s)
+                reverse_ordered += list(s)[::-1]
+
+        slot_values = ','.join(
+            [f'{attr}={getattr(self, attr)}'.lstrip('_')
+             for attr in reverse_ordered[::-1]]
+        )
+
+        return f"{self.__class__.__name__}({slot_values})"
 
     def _fail_validation(self, message: str):
-        """Helper function to distinguish validation between specs."""
-        raise ValueError(message + f' for spec "{self.name}"')
+        """Helper function for creating jax transform-compatible errors."""
+
+        def _raiser(*_):
+            raise ValueError(message + f' for spec "{self.name}"')
+
+        # ValueError is directly raised outside jax.jit/ jax.vmap/ etc.
+        # Otherwise, it is raised through the XLA dispather.
+        _jax.debug.callback(_raiser)
 
     @_abc.abstractmethod
     def validate(self, value: _T) -> _T:
         """Checks if a value conforms to spec. """
 
     @_abc.abstractmethod
     def generate_value(self) -> _T:
         """Generate a value which conforms to this spec."""
 
     @_abc.abstractmethod
     def replace(self, **kwargs: _typing.Any) -> Spec:
         """Returns a new copy of `self` with specified attributes replaced """
 
 
-class CompositeSpec(Spec[_T], _typing.Generic[_T], _abc.ABC):
+class PrimitiveSpec(Spec[_T], _typing.Generic[_T], metaclass=_abc.ABCMeta):
+    """Distinguishes `leaf` Spec Types from structured/ composite Specs.
+
+    In other words, these Specs do not build Specs from other Specs.
+    """
+    __slots__ = ('_shape', '_dtype')
+
+    def __init__(
+            self,
+            shape: _typing.Sequence[int],
+            dtype: _typing.Any,  # TODO: jax.typing.DTypeLike
+            name: str = ""
+    ):
+        """Initializes a new `PrimitiveSpec` spec.
+
+        Args:
+            shape: A Sequence of integers specifying the array shape.
+            dtype: A jax compatible dtype specification for the array.
+            name: Explicit string name for the array specification.
+        """
+        super().__init__(name)
+        self._shape = tuple(shape)
+        self._dtype = _jnp.zeros((), dtype).dtype  # get uniform `dtype` type
+
+    @property
+    def shape(self) -> int | _typing.Sequence[int]:
+        return self._shape
+
+    @property
+    def dtype(self) -> _typing.Any:
+        return self._dtype
+
+
+class CompositeSpec(Spec[_T], _typing.Generic[_T], metaclass=_abc.ABCMeta):
     """Prevent Spec Types that compose other Spec Types from using replace.
 
     Since multiple Specs may be composed with similar namespaces it becomes
     ambiguous and difficult to specify which objects should be replaced.
     Furthermore, in deeply nested composite Specs it will not alway be clear
     whether an object needs to be shallow or deep-copied in order to not
     mutate the original Spec.
 
     Instead, it is safer and more clear to modify any particular leaf Specs
     and rebuild the composite Spec using the constructor.
     """
+    __slots__ = ()
+
+    @_abc.abstractmethod
+    def as_spec_struct(self) -> _jxtype.PyTree[PrimitiveSpec]:
+        """Return the tree of primitive Spec types as is."""
 
     def replace(self, **kwargs: _typing.Any) -> Spec:
         """Composite Specs cannot be unambiguously replaced.
 
         Create new CompositeSpec types by calling the class constructor.
 
         Raises:
@@ -98,67 +176,44 @@
         """
         raise RuntimeError(
             "Composite Specs cannot be unambiguously mutated, "
             "create a new Spec through the Constructor instead."
         )
 
 
-class Array(Spec):
+class Array(PrimitiveSpec):
     """Describes a Jax Array Specification."""
-
-    def __init__(
-            self,
-            shape: _typing.Sequence[int],
-            dtype: _typing.Any,  # TODO: jax.typing.DTypeLike
-            name: str = ""
-    ):
-        """Initializes a new `Array` spec.
-
-        Args:
-            shape: A Sequence of integers specifying the array shape.
-            dtype: A jax compatible dtype specification for the array.
-            name: Explicit string name for the array specification.
-        """
-        super().__init__(name)
-        self._shape = tuple(shape)
-        self._dtype = dtype
-
-    def __str__(self) -> str:
-        return f"{self.__class__.__name__}(shape={str(self.shape)}, " \
-               f"dtype={str(self.dtype)}, name={str(self.name)})"
-
-    @property
-    def shape(self) -> tuple:
-        """Returns a `tuple` specifying the array shape."""
-        return self._shape
-
-    @property
-    def dtype(self) -> _typing.Any:  # TODO: jax.typing.DTypeLike
-        """Returns a jax numpy dtype specifying the array dtype."""
-        return self._dtype
+    __slots__ = ()
 
     def validate(
-            self, 
-            value: _jxtype.Num[_jxtype.Array, '...']
-    ) -> _jxtype.Num[_jxtype.Array, '...']:
+            self,
+            value: _jxtype.ArrayLike
+    ) -> _jxtype.ArrayLike:
         value = _jnp.asarray(value)
+
         if value.shape != self.shape:
             self._fail_validation(
                 f"Expected shape {self.shape} but found {value.shape}"
             )
         if value.dtype != self.dtype:
             self._fail_validation(
                 f"Expected dtype {self.dtype} but found {value.dtype}"
             )
         return value
 
     def generate_value(self) -> _jxtype.Num[_jxtype.Array, '...']:
         """Generate a value which conforms to this spec."""
         return _jnp.zeros(self.shape, self.dtype)
 
+    def __reduce__(
+            self
+    ) -> tuple[_typing.Type[Array], tuple[_typing.Any, ...]]:
+        """Specify how to de-serialize (unpickle) this class Type."""
+        return Array, (self._shape, self._dtype, self._name)
+
     def _get_constructor_kwargs(self) -> _typing.Any:
         """Returns constructor kwargs for instantiating a copy of self."""
         params = _inspect.signature(
             _functools.partial(self.__class__.__init__, self)
         ).parameters
         kinds = {value.kind for value in params.values()}
         if _inspect.Parameter.VAR_POSITIONAL in kinds:
@@ -176,23 +231,27 @@
     def replace(self, **kwargs: _typing.Any) -> _type_ext.Self:
         all_kwargs = self._get_constructor_kwargs()
         all_kwargs.update(kwargs)
         return self.__class__(**all_kwargs)
 
 
 class BoundedArray(Array):
-    """A variant of Array that imposes explicit minimum and maximum bounds."""
+    """A variant of Array that imposes explicit minimum and maximum bounds.
+
+    These bounds annotate (not enforced) a l1 Box constraint.
+    """
+    __slots__ = ('_minimum', '_maximum')
 
     def __init__(
-        self,
-        shape: _typing.Sequence[int],
-        dtype: _typing.Any,  # TODO: jax.typing.DTypeLike
-        minimum: int | float | _jxtype.Num[_jxtype.Array, '...'],
-        maximum: int | float | _jxtype.Num[_jxtype.Array, '...'],
-        name: str = ""
+            self,
+            shape: _typing.Sequence[int],
+            dtype: _typing.Any,  # TODO: jax.typing.DTypeLike
+            minimum: int | float | _jxtype.Num[_jxtype.Array, '...'],
+            maximum: int | float | _jxtype.Num[_jxtype.Array, '...'],
+            name: str = ""
     ):
         """Initializes a new `BoundedArray` spec.
 
         Args:
             shape: A Sequence of integers specifying the array shape.
             dtype: A jax compatible dtype specification for the array.
             minimum: A numerical value/ array of values for the lower bound
@@ -227,172 +286,122 @@
                 f"value in `maximum`, got: \n\t"
                 f"minimum={str(minimum)}\n\tmaximum={str(maximum)}"
             )
 
         self._minimum = minimum
         self._maximum = maximum
 
-    def __str__(self) -> str:
-        return (
-            f"BoundedArray(shape={str(self.shape)}, "
-            f"dtype={str(self.dtype)}, "
-            f"name={str(self.name)}, "
-            f"minimum={str(self.minimum)}, "
-            f"maximum={str(self.maximum)})"
-        )
-
     @property
     def minimum(self) -> _jxtype.Num[_jxtype.Array, '...']:
-        """Returns a Jax array specifying the minimum bounds (inclusive)."""
         return self._minimum
 
     @property
     def maximum(self) -> _jxtype.Num[_jxtype.Array, '...']:
-        """Returns a Jax array specifying the maximum bounds (inclusive)."""
         return self._maximum
 
     def validate(
-            self, 
-            value: _jxtype.Num[_jxtype.Array, '...']
-    ) -> _jxtype.Num[_jxtype.Array, '...']:
+            self,
+            value: _jxtype.ArrayLike
+    ) -> _jxtype.ArrayLike:
+        """Check if value falls inbetween the specified bounds."""
         value = super().validate(value)
-        if (value < self.minimum).any() or (value > self.maximum).any():
-            self._fail_validation(
-                "Values were not all within bounds "
-                f"{self.minimum} <= {value} <= {self.maximum}"
-            )
+
+        _ = _jax.lax.cond(
+            (value < self.minimum).any(),
+            lambda: self._fail_validation(
+                f'Value exceeded minimum: {self.minimum} > {value}'
+            ),
+            lambda: None
+        )
+
+        _ = _jax.lax.cond(
+            (value > self.maximum).any(),
+            lambda: self._fail_validation(
+                f'Value exceeded maximum: {value} > {self.maximum}'
+            ),
+            lambda: None,
+        )
+
         return value
 
     def generate_value(self) -> _jxtype.Num[_jxtype.Array, '...']:
         """Generate a jax array of the minima which conforms to this shape."""
-        return _jnp.ones(shape=self.shape, dtype=self.dtype) * self.minimum
+        return _jnp.full(
+            shape=self.shape, fill_value=self.minimum, dtype=self.dtype
+        )
+
+    def __reduce__(
+            self
+    ) -> tuple[_typing.Type[BoundedArray], tuple[_typing.Any, ...]]:
+        """Specify how to de-serialize (unpickle) this class Type."""
+        return BoundedArray, (self._shape, self._dtype,
+                              self._minimum, self._maximum, self._name)
 
 
 class DiscreteArray(BoundedArray):
-    """A variant of BoundedArray with integer values and a maximum."""
+    """A variant of BoundedArray with strict integer values and minimum=0."""
+    __slots__ = ()
 
     def __init__(
-            self, 
-            num_values: int,
+            self,
+            num_values: int | _typing.Sequence[int] | _jxtype.Integer[
+                _jxtype.Array, '...'
+            ],
             dtype: _typing.Any = _jnp.int32,  # TODO: jax.typing.DTypeLike
             name: str = ""
     ):
-        """Initializes a new `BoundedArray` spec.
+        """Initializes a new `DiscreteArray` spec.
 
         Args:
             num_values: The number of integers this spec should support.
             dtype: An int-like jax dtype for the array.
             name: Explicit string name for the array specification.
 
         Raises:
             ValueError:
                 if `num_values` is not positive or the given `dtype` is not a
                 jax-supported integer type.
         """
-        if (not num_values > 0) or (not _jnp.issubdtype(
-                type(num_values), _jnp.integer)):
-            raise ValueError(
-                f"`num_values` must be a positive integer, got {num_values}."
-            )
-
         if not _jnp.issubdtype(dtype, _jnp.integer):
             raise ValueError(f"`dtype` must be integer, got {dtype}.")
 
-        num_values = int(num_values)
-        maximum = num_values - 1
-
-        super().__init__((), dtype, minimum=0, maximum=maximum, name=name)
-        self._num_values = num_values
-
-    def __str__(self) -> str:
-        return (
-            f"DiscreteArray(shape={str(self.shape)}, "
-            f"dtype={str(self.dtype)}, "
-            f"name={str(self.name)}, minimum={str(self.minimum)},"
-            f" maximum={str(self.maximum)}, "
-            f"num_values={str(self.num_values)})"
-        )
-
-    @property
-    def num_values(self) -> int:
-        """Returns the number of items."""
-        return self._num_values
-
-
-class MultiDiscreteArray(BoundedArray):
-    """Generalizes DiscreteArray to higher dimensions."""
-
-    def __init__(
-        self,
-        num_values: _typing.Sequence[int] | _jxtype.Integer[
-            _jxtype.Array, '...'],
-        dtype: _typing.Any = _jnp.int32,
-        name: str = ""
-    ):
-        """Initializes a new `BoundedArray` spec.
-
-        Args:
-            num_values:
-                The number of integers this spec should support across
-                distinct action dimensions.
-            dtype:
-                An int-like jax dtype for the array.
-            name:
-                Explicit string name for the array specification.
-
-        Raises:
-            ValueError:
-                if `num_values` are not all positive or the given `dtype`
-                is not a jax-supported integer type.
-        """
         num_values = _jnp.asarray(num_values, dtype)
-        if (not (num_values > 0).all()) or (not _jnp.issubdtype(
-                num_values.dtype, _jnp.integer)):
+        if not (num_values > 0).all():
             raise ValueError(
-                f"`num_values` must be an array of positive integers, got {num_values}."
+                f"`num_values` may only contain positive integers, "
+                f"got {num_values}."
             )
 
-        if not _jnp.issubdtype(dtype, _jnp.integer):
-            raise ValueError(f"`dtype` must be integer, got {dtype}.")
-
-        num_values = num_values
-        maximum = num_values - 1
         super().__init__(
-            shape=num_values.shape,
+            shape=_jnp.shape(num_values),
             dtype=dtype,
-            minimum=_jnp.zeros_like(num_values),
-            maximum=maximum,
-            name=name,
+            minimum=0,
+            maximum=num_values - 1,
+            name=name
         )
-        self._num_values = num_values
 
     @property
     def num_values(self) -> _jxtype.Integer[_jxtype.Array, '...']:
-        """Returns the number of possible values across all dimensions."""
-        return self._num_values
+        return self.maximum + 1
 
-    def __repr__(self) -> str:
-        return (
-            f"MultiDiscreteArray("
-            f"shape={repr(self.shape)}, "
-            f"dtype={repr(self.dtype)}, "
-            f"name={repr(self.name)}, "
-            f"minimum={repr(self.minimum)}, "
-            f"maximum={repr(self.maximum)}, "
-            f"num_values={repr(self.num_values)})"
-        )
+    def __reduce__(
+            self
+    ) -> tuple[_typing.Type[DiscreteArray], tuple[_typing.Any, ...]]:
+        """Specify how to de-serialize (unpickle) this class Type."""
+        return DiscreteArray, (self._maximum+1, self._dtype, self._name)
 
 
 @_tree_util.register_pytree_node_class
 class Tree(CompositeSpec):
     """A Compositional Data Spec that behaves like a Jax PyTree.
 
     This Spec is created from other specs by providing the leaf specs and
     a desired PyTree structure.
     """
+    __slots__ = ('_leave_specs', '_treedef')
 
     def __init__(
             self,
             leaves: _typing.Sequence[Spec],
             structure: _tree_util.PyTreeDef,
             name: str = ""
     ):
@@ -404,16 +413,30 @@
                 of the given `structure`.
             structure:
                 The Jax PyTree defintion to unflatten `leaves`.
             name:
                 Explicit string name for the Tree specification.
         """
         super().__init__(name=name)
-        self.leave_specs = leaves
-        self.treedef = structure
+        self._leave_specs = leaves
+        self._treedef = structure
+
+    def __repr__(self) -> str:
+        """Override base `repr` by mapping `repr` over all leave-specs."""
+        leave_strs = _jax.tree_map(repr, self.leave_specs)
+        tree_str = str(_tree_util.tree_unflatten(self.treedef, leave_strs))
+        return f'{self.__class__.__name__}(name={self.name},tree={tree_str})'
+
+    @property
+    def leave_specs(self) -> _typing.Sequence[Spec]:
+        return self._leave_specs
+
+    @property
+    def treedef(self) -> _tree_util.PyTreeDef:
+        return self._treedef
 
     def tree_flatten(
             self
     ) -> tuple[_typing.Sequence[Spec], tuple[_tree_util.PyTreeDef, str]]:
         """Return the leaves and all data needed to reinitialize this class"""
         return self.leave_specs, (self.treedef, self.name)
 
@@ -422,63 +445,63 @@
             cls: _typing.Type[Tree],
             aux: tuple[_tree_util.PyTreeDef, str],
             children: _typing.Sequence[Spec]
     ) -> Tree:
         """Reinitialize the class from the leaves and the requisite data"""
         return cls(children, *aux)
 
-    @property
-    def spec_struct(self) -> _jxtype.PyTree[Spec]:
+    def as_spec_struct(self) -> _jxtype.PyTree[Spec]:
         """Return the unflattend Spec PyTree as is."""
         return _tree_util.tree_unflatten(self.treedef, self.leave_specs)
 
     def validate(
             self,
-            value: _jxtype.PyTree[_jxtype.Num[_jxtype.Array, '...'] | None]
-    ) -> _jxtype.PyTree[_jxtype.Num[_jxtype.Array, '...'] | None]:
-        as_leaves = _tree_util.tree_leaves(value)
-        leaves = _jax.tree_map(
-            lambda v, s: s.validate(v),
-            as_leaves, self.leave_specs
+            value: _jxtype.PyTree[_jxtype.ArrayLike | None]
+    ) -> _jxtype.PyTree[_jxtype.ArrayLike | None]:
+        return _jax.tree_map(
+            lambda s, v: s.validate(v),
+            self.as_spec_struct(), value
         )
-        return _tree_util.tree_unflatten(self.treedef, leaves)
 
     def generate_value(
             self
     ) -> _jxtype.PyTree[_jxtype.Num[_jxtype.Array, '...'] | None]:
         values = [s.generate_value() for s in self.leave_specs]
         return _tree_util.tree_unflatten(self.treedef, values)
 
-    def __str__(self) -> str:
-        leave_strs = _jax.tree_map(str, self.leave_specs)
-        tree_str = str(_tree_util.tree_unflatten(self.treedef, leave_strs))
-        return f'{self.__class__.__name__}(name={self.name}, {tree_str})'
-
 
 class Tuple(Tree):
     """Overrides Tree as a Tuple PyTree Structure."""
+    __slots__ = ()
 
     def __init__(self, *var_specs: Spec, name: str = ""):
         """Initializes a new `Tuple` spec.
 
         Args:
             var_specs:
                 A sequence of `Spec` objects to treat as a Spec tuple.
             name:
                 Explicit string name for the Tree specification.
+
+        Raises:
+            ValueError: If no specs are provided.
         """
+        if not var_specs:
+            raise ValueError("Cannot initialize an empty Spec")
+
         super().__init__(
             list(var_specs),
             _tree_util.tree_structure(var_specs),
             name
         )
 
 
 class Dict(Tree):
     """Overrides Tree as a Dictionary PyTree Structure."""
+    __slots__ = ()
 
     def __init__(
             self,
             dict_spec: dict[str, Spec] | None = None,
             name: str = "",
             **kwarg_specs: Spec
     ):
@@ -497,15 +520,14 @@
 
         Raises:
             ValueError: If the union of all provided specs are empty.
         """
         if dict_spec is None:
             dict_spec = {}
 
-        self._defaults = {'name': name, 'dict_spec': dict_spec} | kwarg_specs
         full_spec = dict_spec | kwarg_specs
 
         if not full_spec:
             raise ValueError("Cannot initialize an empty Spec")
 
         super().__init__(
             list(full_spec.values()),
@@ -516,14 +538,15 @@
 
 class Batched(CompositeSpec, _typing.Generic[_T]):
     """A generic CompositeSpec that prepends a fixed Batch dimension.
 
     This Spec type essentially wraps the base spec with a call to jax.vmap
     inside `validate` and `generate_value`
     """
+    __slots__ = ('_num', '_spec')
 
     def __init__(self, spec: Spec, num: int, name: str = ""):
         """Initializes a new `Batched` spec.
 
         Args:
             spec: The Specification to batch over.
             num: The batch-size to prepend `spec` with.
@@ -532,28 +555,145 @@
         Raises:
             ValueError: If `num` is not positive.
         """
         super().__init__(name)
         if not num > 0:
             raise ValueError("Cannot Batch over empty dimensions! num > 0!")
 
-        self.spec = spec
-        self.num = num
+        self._spec = spec
+        self._num = num
+
+    @property
+    def spec(self) -> Spec:
+        return self._spec
+
+    @property
+    def num(self) -> int:
+        return self._num
+
+    def as_spec_struct(self) -> _jxtype.PyTree[PrimitiveSpec]:
+        """Unpack and prepend batch-size to all leaf-specs.
+
+        Warning, to prevent unnecesarily unpacking nested structures, this
+        method only unpacks CompositeSpec types by one level, and "re-batches"
+        any CompositeSpecs 1 level down.
+
+        To do this recursively, see `unpack_spec`.
+        """
+        base_spec = self.spec
+        if isinstance(base_spec, CompositeSpec):
+            base_spec = base_spec.as_spec_struct()
+
+        def reshape(s: Spec):
+            if isinstance(s, PrimitiveSpec):
+                return reshape_spec(s, prepend=(self.num,))
+            return Batched(s, self.num)
 
-    def __str__(self) -> str:
-        return f'{self.__class__.__name__}(name={self.name}, ' \
-               f'spec={str(self.spec)}, num={self.num})'
+        return _jax.tree_map(reshape, base_spec)
 
     def validate(self, value: _T) -> _T:
-        return _jax.vmap(self.spec.validate)(value)
+        # jax.vmap fails as error-raising is non-homogenous.
+        return _jax.lax.map(self.spec.validate, value)
 
     def generate_value(self) -> _T:
         base_value = self.spec.generate_value()
         return _jax.vmap(lambda x: base_value)(_jnp.arange(self.num))
 
 
+# Utility functions for handling Spec types
+
+@_typing.overload
+def reshape_spec(
+        spec: DiscreteArray,
+        prepend: _typing.Sequence[int] = (),
+        append: _typing.Sequence[int] = ()
+) -> DiscreteArray:
+    ...  # pragma: no cover
+
+
+@_typing.overload
+def reshape_spec(
+        spec: BoundedArray,
+        prepend: _typing.Sequence[int] = (),
+        append: _typing.Sequence[int] = ()
+) -> BoundedArray:
+    ...  # pragma: no cover
+
+
+@_typing.overload
+def reshape_spec(
+        spec: Array,
+        prepend: _typing.Sequence[int] = (),
+        append: _typing.Sequence[int] = ()
+) -> Array:
+    ...  # pragma: no cover
+
+
+@_typing.overload
+def reshape_spec(
+        spec: Spec,
+        prepend: _typing.Sequence[int] = (),
+        append: _typing.Sequence[int] = ()
+) -> Spec:
+    ...  # pragma: no cover
+
+
+def reshape_spec(
+        spec: Spec,
+        prepend: _typing.Sequence[int] = (),
+        append: _typing.Sequence[int] = ()
+) -> Spec:
+    """Utility function to modularly reshape a Spec type.
+
+    This is useful for wrapping Environments with `jax.vmap` like transforms.
+
+    Args:
+        spec: The base spec to reshape
+        prepend: A sequence of integers to add before spec.shape
+        append: A sequence of integers to add after spec.shape
+
+    Returns:
+        The reshaped spec.
+
+    Raises:
+        NotImplementedError:
+            if spec is not of type Array.
+    """
+    if isinstance(spec, DiscreteArray):
+        batched_num = _jnp.broadcast_to(
+            spec.num_values, (*prepend, *spec.num_values.shape, *append)
+        )
+        return spec.replace(num_values=batched_num)
+    elif isinstance(spec, Array):
+        return spec.replace(
+            shape=(*prepend, *spec.shape, *append)  # type: ignore
+        )
+    else:
+        raise NotImplementedError(
+            f"Spec of type: {type(spec)} has no implemented reshape rule."
+        )
+
+
+def unpack_spec(
+        spec: Spec
+) -> Spec:
+    """Recursively unpack composite specs to a tree of Primitive Specs."""
+    if isinstance(spec, CompositeSpec):
+        return _jax.tree_map(unpack_spec, spec.as_spec_struct())
+    return spec
+
+
+def make_environment_spec(env: jit_env.Environment):
+    return EnvironmentSpec(
+        observations=env.observation_spec(),
+        actions=env.action_spec(),
+        rewards=env.reward_spec(),
+        discounts=env.discount_spec()
+    )
+
+
 class EnvironmentSpec(_typing.NamedTuple):
     """Type to collect all specs of an Environment in one place."""
     observations: Spec
     actions: Spec
     rewards: Spec
     discounts: Spec
```

### Comparing `jit_env-0.0.dev0/jit_env/wrappers.py` & `jit_env-0.1.0/jit_env/wrappers.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,18 +4,18 @@
  - Staging of the environment step and reset functions with jax.jit.
  - Batching of the environment step and reset functions with jax.vmap.
  - Automatically Resetting Environments upon `StepType.LAST`.
  - Optimized Wrappers for combining Batching and AutoResetting.
 """
 from __future__ import annotations as _annotations
 import typing as _typing
-import dataclasses as _dataclasses
 
 import jax as _jax
 
+import jit_env
 from jit_env import _core
 from jit_env import specs as _specs
 
 
 class Jit(_core.Wrapper):
     """Wrapper to jax.jit compile the environment step and reset functions."""
 
@@ -58,26 +58,48 @@
     """Wrapper to batch over the environment with unspecified size.
 
     Since `vmap` is ambiguous in the batch-size, we do not modify the
     environment `specs`. These should thus be interpreted as a `slice` of
     the batch dimensions.
     """
 
+    def __init__(self, env: jit_env.Environment, **step_vmap_kwargs):
+        """Initializes the transforming `env.step` and `env.reset` with vmap.
+
+        The step function may receive additional keyword arguments to modify
+        behaviour. Unlike Jit, these kwargs are not used for transforming
+        the reset function. This may be useful for holding either a state or
+        an action constant using `in_axes`, which is not symmetrically
+        compatible with `reset`.
+
+        Args:
+            env:
+                The environment to batch using jax.vmap.
+            **step_vmap_kwargs:
+                keyword arguments passed to jax.vmap only for `env.step`.
+                Defer to the jax documentation for up-to-date documentation
+                on the keyword arguments.
+        """
+        super().__init__(env)
+
+        self._step_fun = _jax.vmap(env.step, **step_vmap_kwargs)
+        self._reset_fun = _jax.vmap(env.reset)
+
     def reset(
             self,
             key: _jax.random.KeyArray  # (Batch, dim_key)
     ) -> tuple[_core.State, _core.TimeStep]:
-        return _jax.vmap(self.env.reset)(key)
+        return self._reset_fun(key)
 
     def step(
             self,
             state: _core.State,  # Tree[(Batch, dim_leaf), ...]
             action: _core.Action  # Tree[(Batch, dim_leaf), ...]
     ) -> tuple[_core.State, _core.TimeStep]:
-        return _jax.vmap(self.env.step)(state, action)
+        return self._step_fun(state, action)
 
     def render(self, state: _core.State) -> _typing.Any:
         """Generate a pixel-observation based on the 0'th state slice. """
         state_0 = _jax.tree_map(lambda x: x.at[0].get(), state)
         return super().render(state_0)
 
 
@@ -127,28 +149,28 @@
         """Either reshape or compose env.reward_spec() to a batch.
 
         If the env.reward_spec() is a Array type, which allows for reshaping,
         the spec is reshaped. Otherwise it is composed with Batched.
         """
         spec = self.env.reward_spec()
         if isinstance(spec, _specs.Array):
-            return spec.replace(shape=(self.num, *spec.shape))
+            return _specs.reshape_spec(spec, prepend=(self.num,))
 
         return _specs.Batched(self.env.reward_spec(), num=self.num)
 
     def discount_spec(self) -> _specs.Batched | _specs.BoundedArray:
         """Either reshape or compose env.discount_spec() to a batch.
 
         If the env.discount_spec() is a Array type, which allows for reshaping,
         the spec is reshaped. Otherwise it is composed with Batched.
         """
         spec = self.env.discount_spec()
         if isinstance(spec, _specs.BoundedArray):
             # TODO: Not compatibile with Array (should not be valid anyway).
-            return spec.replace(shape=(self.num, *spec.shape))
+            return _specs.reshape_spec(spec, prepend=(self.num,))
 
         return _specs.Batched(self.env.discount_spec(), num=self.num)
 
 
 class Tile(BatchSpecMixin, Vmap):
     """Wrapper to batch over the environment with fixed size.
 
@@ -158,15 +180,15 @@
     specified, which is done by the `BatchSpecMixin`.
 
     The constructor is called first through `BatchSpecMixin` which
     simultaneously requires the user to define the batch-size as `num`.
     """
 
     def reset(
-            self, 
+            self,
             key: _jax.random.KeyArray
     ) -> tuple[_core.State, _core.TimeStep]:
         return super().reset(_jax.random.split(key, num=self.num))
 
 
 class ResetMixin:
     """Mixin to provide helper functions for resetting Environments"""
@@ -202,26 +224,26 @@
                and observation generated by env.reset. The discount, reward,
                and extras fields are copied from the `step` argument.
         """
 
         key, _ = _jax.random.split(state.key)
         state, reset_timestep = self.env.reset(key)
 
-        # Replace observation with reset observation.
-        # Do not modify the rewards, discount, or extras.
-        timestep = _dataclasses.replace(
-            step,
-            observation=reset_timestep.observation,
-            step_type=reset_timestep.step_type,
+        timestep = _core.TimeStep(
+            step_type=reset_timestep.step_type,  # Overwrite step
+            reward=step.reward,
+            discount=step.discount,
+            observation=reset_timestep.observation,  # Overwrite step
+            extras=step.extras
         )
 
         return state, timestep
 
     @staticmethod
-    def _identity(x: _typing.Any) -> _typing.Any:
+    def _identity(*x: _typing.Any) -> _typing.Any:
         """Helper method defined to prevent recompilations of `lambda`s.
 
         Args:
             x: Some value
 
         Returns:
             The same value `x`.
@@ -296,32 +318,31 @@
     """
 
     def step(
             self,
             state: _core.State,
             action: _core.Action
     ) -> tuple[_core.State, _core.TimeStep]:
-
-        # Batched computation using `Vmap`.
+        # Batched homogenous computation using `Vmap`.
         state, timestep = super().step(state, action)
 
         # Map heterogeneous computation (non-parallelizable).
-        state, timestep = _jax.lax.map(
-            lambda args: self._maybe_reset(*args), (state, timestep)
-        )
+        state, timestep = _jax.lax.map(self._maybe_reset, (state, timestep))
+
         return state, timestep
 
     def _maybe_reset(
-        self, state: _core.State, step: _core.TimeStep
+            self, args: tuple[_core.State, _core.TimeStep]
     ) -> tuple[_core.State, _core.TimeStep]:
         """Helper method defined to prevent recompilations of `lambda`s."""
+        state, step = args
         return _jax.lax.cond(
             step.last(),
             self._auto_reset,
-            lambda *x: x,
+            self._identity,
             state,
             step,
         )
 
 
 class TileAutoReset(Tile, VmapAutoReset):
     """Variant of VmapAutoReset with a fixed batch size.
@@ -330,8 +351,12 @@
 
     Note that this mixed in class inherits from `Vmap` multiple times, the
     class method resolution order still gives precedence to Tile over Vmap
     when calling the `reset` and `spec` functions (which is all we need).
 
     The shortened MRO is given by:
     [TileAutoReset, Tile, BatchSpecMixin, VmapAutoReset, ResetMixin, Vmap, ...]
+
+    The mixed in functions by evalation order are:
+    [(), (reset), (*_spec), (step, _maybe_reset), (_identity, _auto_reset),
+    (reset, step, render)]
     """
```

### Comparing `jit_env-0.0.dev0/jit_env.egg-info/PKG-INFO` & `jit_env-0.1.0/jit_env.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,96 +1,106 @@
 Metadata-Version: 2.1
 Name: jit-env
-Version: 0.0.dev0
+Version: 0.1.0
 Summary: A Jax interface for Reinforcement Learning environments.
 Home-page: https://github.com/joeryjoery/jit_env
 Author: Joery A. de Vries
 Author-email: J.A.deVries@tudelft.nl
 License: MIT
 Keywords: reinforcement-learning python machine learning jax
-Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Testing :: Mocking
 Classifier: Topic :: Software Development :: Testing :: Unit
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
+![Run Tox Tests](https://github.com/joeryjoery/jit_env/actions/workflows/tests.yml/badge.svg)
+![Python Version](https://img.shields.io/badge/Python-3.9%20%7C%203.10%20%7C%203.11-blue)
+![Package Version](https://img.shields.io/badge/jit__env-0.1.0-blue)
 # `jit_env`: A Jax Compatible RL Environment API
 `jit_env` is a library that aims to adhere closely to the `dm_env` interface
-while allowing for `Jax` transformations inside Environment implementations
+while allowing for `jax` transformations inside Environment implementations
 and defining clear type annotations.
 
 Like `dm_env` our API consists of the main components:
 
 - `jit_env.Environment`: An abstract base class for RL environments.
 - `jit_env.TimeStep`: A container class representing the outputs of the environment on each time step (transition).
 - `jit_env.specs`: A module containing primitives that are used to describe the format of the actions consumed by an environment, as well as the observations, rewards, and discounts it returns.
-- TODO: Testing is not yet implemented.
 
 This is extended with the components:
 - `jit_env.Wrapper`: An interface built on top of Environment that allows modular transformations of the base Environment.
 - `jit_env.Action, jit_env.Observation, jit_env.State`: Explicit types that concern Agent-Environment IO.
 - `jit_env.compat`: A Module containing API hooks to other Agent-Environment interfaces like `dm_env` or `gymnasium`.
 - `jit_env.wrappers`: A Module containing a few generally useful implementations for `Wrapper` (that simultaneously serves as a reference).
 
 Note that this module is only an interface and does not implement any
-Environments itself.
+Environments itself. The implementations in `examples` serve to illustrate the syntax.
+For a more thorough review of the semantics, please refer to the [dm-env](https://github.com/deepmind/dm_env/blob/master/dm_env/specs.py) 
+wiki and compare our implementation of `jit_env.Environment` with `dm_env.Environment` and the conversion as given in [`compat.py`](https://github.com/joeryjoery/jit_env/blob/main/jit_env/compat.py).
 
-## The Big Difference
+## Installation
+`jit_env` can be installed with:
+
+`python -m pip install jit-env`
+
+You can also install it directly from our GitHub repository using pip:
+
+`python -m pip install git+git://github.com/joeryjoery/jit_env.git`
+
+or alternatively by checking out a local copy of our repository and running:
+
+`python -m pip install /path/to/local/jit_env/`
+
+## The Big Difference with `dm_env`
 The main difference between this API and the standard `dm_env` API is
 that our definition of `jit_env.Environment` is functionally pure.
 This allows the the logic to e.g., be batched over or accelerated 
 using `jax.vmap` or `jax.jit`. 
 
 On top of that, we extend the `specs` logic of what `dm_env` provides.
 The `specs` module defines primitive for how the Agent interacts with 
 the Environment. We explicitly implement additional specs that are 
 compatible with `jax` based `PyTree` objects.
 This allows for tree-based operations on the `spec` objects themselves, 
 which in turn gives some added flexibility in designing desired 
 state-action spaces.
 
-## Installation
-`jit_env` can be installed with:
+Some other modified behaviours include: 
+ - `restart` providing a reference value for reward and discount in place of `None`
+ - `StepType` is no longer an `enum` type as `jax.jit` would type convert `enum` types to jax primitives anyway. It remains a namespace for defining episode boundaries.
+ - `TimeStep` is now a frozen `chex.dataclass` to allow usage of `replace` within the public API (which is private for `NamedTuple`).
+ - `TimeStep` carries an additional `extras` field to carry optional data (metrics) not shown to the agent.
+ - all helper `restart`, `transition`, etc., now take a `shape` value to generate the reference `reward` or `discount` fields.
 
-`python -m pip install jit-env`
-
-You can also install it directly from our GitHub repository using pip:
-
-`python -m pip install git+git://github.com/joeryjoery/jit_env.git`
-
-or alternatively by checking out a local copy of our repository and running:
+### Why `jit_env`
+I developed this module to have a reliable Environment backend that is less subject
+to refactoring changes as other libraries while providing free compatibility to both `jax` 
+transforms as well as any other popular type of Agent-Environment interface. 
 
-`python -m pip install /path/to/local/jit_env/`
+The hope is that this library will not require much maintenance/ alterations 
+(aside from some type-hint updates) after an official 1.0.0 release. 
 
 ## Cite us
 If you are a particularly nice person and this work was useful to you, you can
 cite this repository as:
-```
+```bibtex
 @misc{jit_env_2023,
   author={Joery A. de Vries},
   title={jit\_env: A Jax interface for reinforcement learning environments},
   year={2023},
   url={http://github.com/joeryjoery/jit_env}
 }
 ```
 
 ## References
 This library was heavily inspired by the following libraries:
 - dm-env: [https://github.com/deepmind/dm_env](https://github.com/deepmind/dm_env)
 - jumanji: [https://github.com/instadeepai/jumanji](https://github.com/instadeepai/jumanji)
 - gymnax: [https://github.com/RobertTLange/gymnax](https://github.com/RobertTLange/gymnax)
-
-I developed this module to have a reliable Environment backend that is less subject
-to refactoring changes as these other libraries. The hope is that this library
-will not require much maintenance/ alterations at all (aside from some type-hint updates) 
-after an official 1.0.0 release.
-
-
```

### Comparing `jit_env-0.0.dev0/setup.py` & `jit_env-0.1.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,14 +9,16 @@
                if not (line.isspace() or line.startswith("#"))]
     return lst
 
 
 _pwd = os.path.dirname(os.path.abspath(__file__))
 _req = _parse_requirements(os.path.join(
     _pwd, './', 'requirements.txt'))
+_req_dev = _parse_requirements(os.path.join(
+    _pwd, './', 'requirements_dev.txt'))
 
 _d = {}
 with open('jit_env/version.py') as f:
     exec(f.read(), _d)
 
 try:
     __version__ = _d['__version__']
@@ -37,24 +39,18 @@
     author_email="J.A.deVries@tudelft.nl",
     keywords='reinforcement-learning python machine learning jax',
     packages=find_packages(),
     url='https://github.com/joeryjoery/jit_env',
     license='MIT',
     python_requires='>=3.7',
     install_requires=_req,
-    extras_require={'dev': [
-        'pytest>=7.1.2',
-        'twine>=4.0.2',
-        'wheel>=0.37.1',
-        'dm_env>=1.5'
-    ]},
+    extras_require={'dev': _req_dev},
     classifiers=[
         'Operating System :: OS Independent',
         'License :: OSI Approved :: MIT License',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Topic :: Software Development :: Testing :: Mocking',
         'Topic :: Software Development :: Testing :: Unit'
     ]
```

