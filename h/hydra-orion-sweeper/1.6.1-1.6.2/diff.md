# Comparing `tmp/hydra-orion-sweeper-1.6.1.tar.gz` & `tmp/hydra-orion-sweeper-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hydra-orion-sweeper-1.6.1.tar", last modified: Mon Apr  3 14:42:39 2023, max compression
+gzip compressed data, was "hydra-orion-sweeper-1.6.2.tar", last modified: Tue Apr 11 15:23:53 2023, max compression
```

## Comparing `hydra-orion-sweeper-1.6.1.tar` & `hydra-orion-sweeper-1.6.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 14:42:39.915406 hydra-orion-sweeper-1.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-03 14:41:32.000000 hydra-orion-sweeper-1.6.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5224 2023-04-03 14:42:39.915406 hydra-orion-sweeper-1.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-04-03 14:41:32.000000 hydra-orion-sweeper-1.6.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 14:42:39.911406 hydra-orion-sweeper-1.6.1/hydra_orion_sweeper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5224 2023-04-03 14:42:39.000000 hydra-orion-sweeper-1.6.1/hydra_orion_sweeper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-03 14:42:39.000000 hydra-orion-sweeper-1.6.1/hydra_orion_sweeper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 14:42:39.000000 hydra-orion-sweeper-1.6.1/hydra_orion_sweeper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-03 14:42:39.000000 hydra-orion-sweeper-1.6.1/hydra_orion_sweeper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-03 14:42:39.000000 hydra-orion-sweeper-1.6.1/hydra_orion_sweeper.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 14:42:39.911406 hydra-orion-sweeper-1.6.1/hydra_plugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 14:42:39.915406 hydra-orion-sweeper-1.6.1/hydra_plugins/hydra_orion_sweeper/
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-03 14:41:32.000000 hydra-orion-sweeper-1.6.1/hydra_plugins/hydra_orion_sweeper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-04-03 14:41:32.000000 hydra-orion-sweeper-1.6.1/hydra_plugins/hydra_orion_sweeper/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    19601 2023-04-03 14:41:32.000000 hydra-orion-sweeper-1.6.1/hydra_plugins/hydra_orion_sweeper/implementation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-04-03 14:41:32.000000 hydra-orion-sweeper-1.6.1/hydra_plugins/hydra_orion_sweeper/orion_sweeper.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-03 14:42:39.915406 hydra-orion-sweeper-1.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-03 14:41:32.000000 hydra-orion-sweeper-1.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:23:53.533922 hydra-orion-sweeper-1.6.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-11 15:23:01.000000 hydra-orion-sweeper-1.6.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-04-11 15:23:53.533922 hydra-orion-sweeper-1.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-04-11 15:23:01.000000 hydra-orion-sweeper-1.6.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:23:53.533922 hydra-orion-sweeper-1.6.2/hydra_orion_sweeper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-04-11 15:23:53.000000 hydra-orion-sweeper-1.6.2/hydra_orion_sweeper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-11 15:23:53.000000 hydra-orion-sweeper-1.6.2/hydra_orion_sweeper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 15:23:53.000000 hydra-orion-sweeper-1.6.2/hydra_orion_sweeper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-11 15:23:53.000000 hydra-orion-sweeper-1.6.2/hydra_orion_sweeper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-11 15:23:53.000000 hydra-orion-sweeper-1.6.2/hydra_orion_sweeper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:23:53.533922 hydra-orion-sweeper-1.6.2/hydra_plugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:23:53.533922 hydra-orion-sweeper-1.6.2/hydra_plugins/hydra_orion_sweeper/
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-11 15:23:01.000000 hydra-orion-sweeper-1.6.2/hydra_plugins/hydra_orion_sweeper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-04-11 15:23:01.000000 hydra-orion-sweeper-1.6.2/hydra_plugins/hydra_orion_sweeper/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20253 2023-04-11 15:23:01.000000 hydra-orion-sweeper-1.6.2/hydra_plugins/hydra_orion_sweeper/implementation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-04-11 15:23:01.000000 hydra-orion-sweeper-1.6.2/hydra_plugins/hydra_orion_sweeper/orion_sweeper.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 15:23:53.533922 hydra-orion-sweeper-1.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-11 15:23:01.000000 hydra-orion-sweeper-1.6.2/setup.py
```

### Comparing `hydra-orion-sweeper-1.6.1/PKG-INFO` & `hydra-orion-sweeper-1.6.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hydra-orion-sweeper
-Version: 1.6.1
+Version: 1.6.2
 Summary: Hydra Orion Sweeper plugin
 Home-page: https://orion.readthedocs.io/
 Author: Pierre Delaunay
 Author-email: pierre.delaunay@mila.quebec
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -93,15 +93,15 @@
 
    hydra:
        sweeper:
           params:
              a: "uniform(0, 1)"
              b: "uniform(0, 1)"
 
-          orion:
+          experiment:
              name: 'experiment'
              version: '1'
 
           algorithm:
              type: random
              config:
                 seed: 1
```

### Comparing `hydra-orion-sweeper-1.6.1/README.rst` & `hydra-orion-sweeper-1.6.2/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -77,15 +77,15 @@
 
    hydra:
        sweeper:
           params:
              a: "uniform(0, 1)"
              b: "uniform(0, 1)"
 
-          orion:
+          experiment:
              name: 'experiment'
              version: '1'
 
           algorithm:
              type: random
              config:
                 seed: 1
```

### Comparing `hydra-orion-sweeper-1.6.1/hydra_orion_sweeper.egg-info/PKG-INFO` & `hydra-orion-sweeper-1.6.2/hydra_orion_sweeper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hydra-orion-sweeper
-Version: 1.6.1
+Version: 1.6.2
 Summary: Hydra Orion Sweeper plugin
 Home-page: https://orion.readthedocs.io/
 Author: Pierre Delaunay
 Author-email: pierre.delaunay@mila.quebec
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -93,15 +93,15 @@
 
    hydra:
        sweeper:
           params:
              a: "uniform(0, 1)"
              b: "uniform(0, 1)"
 
-          orion:
+          experiment:
              name: 'experiment'
              version: '1'
 
           algorithm:
              type: random
              config:
                 seed: 1
```

### Comparing `hydra-orion-sweeper-1.6.1/hydra_plugins/hydra_orion_sweeper/config.py` & `hydra-orion-sweeper-1.6.2/hydra_plugins/hydra_orion_sweeper/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     branching: Optional[str] = None
     debug: Optional[bool] = False
     workspace: Optional[str] = None
 
     # Set by the plugin
     id: Optional[str] = None
     trial: Optional[str] = None
+    paramhash: Optional[str] = None
     uuid: Optional[str] = None
 
 
 @dataclass
 class WorkerConf:
     """Orion Worker configuration
 
@@ -80,14 +81,17 @@
 class OrionSweeperConf:
     """Orion Sweeper configuration"""
 
     _target_: str = "hydra_plugins.hydra_orion_sweeper.orion_sweeper.OrionSweeper"
 
     experiment: OrionClientConf = field(default_factory=OrionClientConf)
 
+    # dreprecated
+    orion: Optional[OrionClientConf] = None
+
     worker: WorkerConf = field(default_factory=WorkerConf)
 
     algorithm: AlgorithmConf = field(default_factory=AlgorithmConf)
 
     storage: StorageConf = field(default_factory=StorageConf)
 
     # deprecated, use params instead
```

### Comparing `hydra-orion-sweeper-1.6.1/hydra_plugins/hydra_orion_sweeper/implementation.py` & `hydra-orion-sweeper-1.6.2/hydra_plugins/hydra_orion_sweeper/implementation.py`

 * *Files 5% similar despite different names*

```diff
@@ -156,25 +156,37 @@
     parser.functions.register(name="normal", func=normal)
     parser.functions.register(name="choices", func=choices)
     parser.functions.register(name="fidelity", func=fidelity)
     parser.functions.register(name="dict", func=override_dict)
     return parser
 
 
-def as_overrides(trial, additional, uuid):
+def as_overrides(trial, additional, uuid, compat=False):
     """Returns the trial arguments as hydra overrides"""
     kwargs = deepcopy(additional)
     kwargs.update(flatten(trial.params))
 
     args = [f"{k}={v}" for k, v in kwargs.items()]
     args += [
         f"hydra.sweeper.experiment.id={trial.experiment}",
         f"hydra.sweeper.experiment.trial={trial.id}",
+        # Note
+        #   Does not include fidelity
+        # https://orion.readthedocs.io/en/latest/code/core/worker/trial.html#orion.core.worker.trial.Trial.hash_params
+        f"hydra.sweeper.experiment.paramhash={trial.hash_params}",
         f"hydra.sweeper.experiment.uuid={uuid}",
     ]
+
+    if compat:
+        args += [
+            f"hydra.sweeper.orion.id={trial.experiment}",
+            f"hydra.sweeper.orion.trial={trial.id}",
+            f"hydra.sweeper.orion.paramhash={trial.hash_params}",
+            f"hydra.sweeper.orion.uuid={uuid}",
+        ]
     return tuple(args)
 
 
 def to_objective(value):
     """Convert a return value into an Orion objective"""
 
     if isinstance(value, (float, int)):
@@ -340,14 +352,15 @@
     def __init__(
         self,
         experiment: OrionClientConf,
         worker: WorkerConf,
         algorithm: AlgorithmConf,
         storage: StorageConf,
         params: Optional[DictConfig],
+        compat: bool = False,
     ):
         self.space = None
         self.arguments = dict()
         self.pending_trials = set()
         self.client = None
         self.storage = None
         self.uuid = uuid.uuid1().hex
@@ -360,14 +373,15 @@
         self.launcher: Optional[Launcher] = None
         self.hydra_context: Optional[HydraContext] = None
         self.job_results = None
         self.job_idx: Optional[int] = None
 
         self.space_parser = SpaceParser()
         self.space_parser.add_from_parametrization(params)
+        self.compat = compat
 
     def setup(
         self,
         *,
         hydra_context: HydraContext,
         task_function: TaskFunction,
         config: DictConfig,
@@ -532,15 +546,18 @@
         logger.debug("Suggest %d new trials", len(trials))
         self.pending_trials.update(set(trials))
         return trials
 
     def execute_trials(self, trials: List[Trial]) -> Sequence[JobReturn]:
         """Execture the given batch of trials"""
 
-        overrides = list(as_overrides(t, self.arguments, self.uuid) for t in trials)
+        overrides = list(
+            as_overrides(t, self.arguments, self.uuid, compat=self.compat)
+            for t in trials
+        )
         self.validate_batch_is_legal(overrides)
 
         returns = self.launcher.launch(overrides, initial_job_idx=self.job_idx)
         self.job_idx += len(returns)
         return returns
 
     def observe_one(
```

### Comparing `hydra-orion-sweeper-1.6.1/hydra_plugins/hydra_orion_sweeper/orion_sweeper.py` & `hydra-orion-sweeper-1.6.2/hydra_plugins/hydra_orion_sweeper/orion_sweeper.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,14 +20,15 @@
         self,
         experiment: Optional[OrionClientConf],
         worker: WorkerConf,
         algorithm: AlgorithmConf,
         storage: StorageConf,
         parametrization: Optional[DictConfig],
         params: Optional[DictConfig],
+        orion: Optional[OrionClientConf] = None,
     ):
         from .implementation import OrionSweeperImpl
 
         # >>> Remove with Issue #8
         if parametrization is not None and params is None:
             warn(
                 "`hydra.sweeper.parametrization` is deprecated;"
@@ -43,15 +44,29 @@
                 DeprecationWarning,
             )
         # <<<
 
         if params is None:
             params = dict()
 
-        self.sweeper = OrionSweeperImpl(experiment, worker, algorithm, storage, params)
+        compat = False
+        if orion is not None:
+            compat = True
+            warn(
+                "`hydra.sweeper.orion` as dreprecated in favour of `hydra.sweeper.experiment`."
+                "Please update to avoid misconfiguration",
+                DeprecationWarning,
+            )
+
+        if experiment is None:
+            experiment = orion
+
+        self.sweeper = OrionSweeperImpl(
+            experiment, worker, algorithm, storage, params, compat
+        )
 
     def setup(
         self,
         *,
         hydra_context: HydraContext,
         task_function: TaskFunction,
         config: DictConfig,
```

### Comparing `hydra-orion-sweeper-1.6.1/setup.py` & `hydra-orion-sweeper-1.6.2/setup.py`

 * *Files identical despite different names*

