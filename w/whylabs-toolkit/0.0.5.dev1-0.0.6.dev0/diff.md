# Comparing `tmp/whylabs_toolkit-0.0.5.dev1.tar.gz` & `tmp/whylabs_toolkit-0.0.6.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whylabs_toolkit-0.0.5.dev1.tar", max compression
+gzip compressed data, was "whylabs_toolkit-0.0.6.dev0.tar", max compression
```

## Comparing `whylabs_toolkit-0.0.5.dev1.tar` & `whylabs_toolkit-0.0.6.dev0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0    11357 2023-03-28 19:59:13.175980 whylabs_toolkit-0.0.5.dev1/LICENSE
--rw-r--r--   0        0        0     1409 2023-03-28 19:59:13.175980 whylabs_toolkit-0.0.5.dev1/README.md
--rw-r--r--   0        0        0      855 2023-03-28 19:59:13.175980 whylabs_toolkit-0.0.5.dev1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-28 19:59:13.175980 whylabs_toolkit-0.0.5.dev1/whylabs_toolkit/__init__.py
--rw-r--r--   0        0        0        0 2023-03-28 19:59:13.175980 whylabs_toolkit-0.0.5.dev1/whylabs_toolkit/cli/__init__.py
--rw-r--r--   0        0        0      559 2023-03-28 19:59:13.175980 whylabs_toolkit-0.0.5.dev1/whylabs_toolkit/container/config_types.py
--rw-r--r--   0        0        0        0 2023-03-28 19:59:13.179980 whylabs_toolkit-0.0.5.dev1/whylabs_toolkit/helpers/__init__.py
--rw-r--r--   0        0        0      362 2023-03-28 19:59:13.179980 whylabs_toolkit-0.0.5.dev1/whylabs_toolkit/helpers/client.py
--rw-r--r--   0        0        0     1600 2023-03-28 19:59:13.179980 whylabs_toolkit-0.0.5.dev1/whylabs_toolkit/helpers/config.py
--rw-r--r--   0        0        0      960 2023-03-28 19:59:13.179980 whylabs_toolkit-0.0.5.dev1/whylabs_toolkit/helpers/dataset_profiles.py
--rw-r--r--   0        0        0     1458 2023-03-28 19:59:13.179980 whylabs_toolkit-0.0.5.dev1/whylabs_toolkit/helpers/models.py
--rw-r--r--   0        0        0     3398 2023-03-28 19:59:13.179980 whylabs_toolkit-0.0.5.dev1/whylabs_toolkit/helpers/monitor_helpers.py
--rw-r--r--   0        0        0     6066 2023-03-28 19:59:13.179980 whylabs_toolkit-0.0.5.dev1/whylabs_toolkit/helpers/schema.py
--rw-r--r--   0        0        0      922 2023-03-28 19:59:13.179980 whylabs_toolkit-0.0.5.dev1/whylabs_toolkit/helpers/utils.py
--rw-r--r--   0        0        0      121 2023-03-28 19:59:13.179980 whylabs_toolkit-0.0.5.dev1/whylabs_toolkit/monitor/__init__.py
--rw-r--r--   0        0        0      178 2023-03-28 19:59:13.179980 whylabs_toolkit-0.0.5.dev1/whylabs_toolkit/monitor/manager/__init__.py
--rw-r--r--   0        0        0      557 2023-03-28 19:59:13.179980 whylabs_toolkit-0.0.5.dev1/whylabs_toolkit/monitor/manager/credentials.py
--rw-r--r--   0        0        0     4862 2023-03-28 19:59:13.179980 whylabs_toolkit-0.0.5.dev1/whylabs_toolkit/monitor/manager/manager.py
--rw-r--r--   0        0        0     8760 2023-03-28 19:59:13.179980 whylabs_toolkit-0.0.5.dev1/whylabs_toolkit/monitor/manager/monitor_setup.py
--rw-r--r--   0        0        0     1500 2023-03-28 19:59:13.179980 whylabs_toolkit-0.0.5.dev1/whylabs_toolkit/monitor/models/__init__.py
--rw-r--r--   0        0        0      841 2023-03-28 19:59:13.179980 whylabs_toolkit-0.0.5.dev1/whylabs_toolkit/monitor/models/analyzer/__init__.py
--rw-r--r--   0        0        0    12589 2023-03-28 19:59:13.179980 whylabs_toolkit-0.0.5.dev1/whylabs_toolkit/monitor/models/analyzer/algorithms.py
--rw-r--r--   0        0        0     4597 2023-03-28 19:59:13.179980 whylabs_toolkit-0.0.5.dev1/whylabs_toolkit/monitor/models/analyzer/analyzer.py
--rw-r--r--   0        0        0     3242 2023-03-28 19:59:13.179980 whylabs_toolkit-0.0.5.dev1/whylabs_toolkit/monitor/models/analyzer/baseline.py
--rw-r--r--   0        0        0     2071 2023-03-28 19:59:13.179980 whylabs_toolkit-0.0.5.dev1/whylabs_toolkit/monitor/models/analyzer/targets.py
--rw-r--r--   0        0        0     4115 2023-03-28 19:59:13.179980 whylabs_toolkit-0.0.5.dev1/whylabs_toolkit/monitor/models/column_schema.py
--rw-r--r--   0        0        0     3363 2023-03-28 19:59:13.179980 whylabs_toolkit-0.0.5.dev1/whylabs_toolkit/monitor/models/commons.py
--rw-r--r--   0        0        0     2497 2023-03-28 19:59:13.179980 whylabs_toolkit-0.0.5.dev1/whylabs_toolkit/monitor/models/document.py
--rw-r--r--   0        0        0     9201 2023-03-28 19:59:13.179980 whylabs_toolkit-0.0.5.dev1/whylabs_toolkit/monitor/models/monitor.py
--rw-r--r--   0        0        0      574 2023-03-28 19:59:13.179980 whylabs_toolkit-0.0.5.dev1/whylabs_toolkit/monitor/models/segments.py
--rw-r--r--   0        0        0      961 2023-03-28 19:59:13.179980 whylabs_toolkit-0.0.5.dev1/whylabs_toolkit/monitor/models/utils.py
--rw-r--r--   0        0        0    66146 2023-03-28 19:59:13.179980 whylabs_toolkit-0.0.5.dev1/whylabs_toolkit/monitor/schema/schema.json
--rw-r--r--   0        0        0     2512 1970-01-01 00:00:00.000000 whylabs_toolkit-0.0.5.dev1/setup.py
--rw-r--r--   0        0        0     2244 1970-01-01 00:00:00.000000 whylabs_toolkit-0.0.5.dev1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-10 22:21:38.271279 whylabs_toolkit-0.0.6.dev0/LICENSE
+-rw-r--r--   0        0        0     1409 2023-04-10 22:21:38.271279 whylabs_toolkit-0.0.6.dev0/README.md
+-rw-r--r--   0        0        0      855 2023-04-10 22:21:38.275279 whylabs_toolkit-0.0.6.dev0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-10 22:21:38.275279 whylabs_toolkit-0.0.6.dev0/whylabs_toolkit/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-10 22:21:38.275279 whylabs_toolkit-0.0.6.dev0/whylabs_toolkit/cli/__init__.py
+-rw-r--r--   0        0        0      559 2023-04-10 22:21:38.275279 whylabs_toolkit-0.0.6.dev0/whylabs_toolkit/container/config_types.py
+-rw-r--r--   0        0        0        0 2023-04-10 22:21:38.275279 whylabs_toolkit-0.0.6.dev0/whylabs_toolkit/helpers/__init__.py
+-rw-r--r--   0        0        0      362 2023-04-10 22:21:38.275279 whylabs_toolkit-0.0.6.dev0/whylabs_toolkit/helpers/client.py
+-rw-r--r--   0        0        0     1600 2023-04-10 22:21:38.275279 whylabs_toolkit-0.0.6.dev0/whylabs_toolkit/helpers/config.py
+-rw-r--r--   0        0        0      960 2023-04-10 22:21:38.275279 whylabs_toolkit-0.0.6.dev0/whylabs_toolkit/helpers/dataset_profiles.py
+-rw-r--r--   0        0        0     1458 2023-04-10 22:21:38.275279 whylabs_toolkit-0.0.6.dev0/whylabs_toolkit/helpers/models.py
+-rw-r--r--   0        0        0     3398 2023-04-10 22:21:38.275279 whylabs_toolkit-0.0.6.dev0/whylabs_toolkit/helpers/monitor_helpers.py
+-rw-r--r--   0        0        0     6066 2023-04-10 22:21:38.275279 whylabs_toolkit-0.0.6.dev0/whylabs_toolkit/helpers/schema.py
+-rw-r--r--   0        0        0      922 2023-04-10 22:21:38.275279 whylabs_toolkit-0.0.6.dev0/whylabs_toolkit/helpers/utils.py
+-rw-r--r--   0        0        0      121 2023-04-10 22:21:38.275279 whylabs_toolkit-0.0.6.dev0/whylabs_toolkit/monitor/__init__.py
+-rw-r--r--   0        0        0      178 2023-04-10 22:21:38.275279 whylabs_toolkit-0.0.6.dev0/whylabs_toolkit/monitor/manager/__init__.py
+-rw-r--r--   0        0        0      557 2023-04-10 22:21:38.275279 whylabs_toolkit-0.0.6.dev0/whylabs_toolkit/monitor/manager/credentials.py
+-rw-r--r--   0        0        0     5777 2023-04-10 22:21:38.275279 whylabs_toolkit-0.0.6.dev0/whylabs_toolkit/monitor/manager/manager.py
+-rw-r--r--   0        0        0     9551 2023-04-10 22:21:38.275279 whylabs_toolkit-0.0.6.dev0/whylabs_toolkit/monitor/manager/monitor_setup.py
+-rw-r--r--   0        0        0     1500 2023-04-10 22:21:38.275279 whylabs_toolkit-0.0.6.dev0/whylabs_toolkit/monitor/models/__init__.py
+-rw-r--r--   0        0        0      841 2023-04-10 22:21:38.279279 whylabs_toolkit-0.0.6.dev0/whylabs_toolkit/monitor/models/analyzer/__init__.py
+-rw-r--r--   0        0        0    12589 2023-04-10 22:21:38.279279 whylabs_toolkit-0.0.6.dev0/whylabs_toolkit/monitor/models/analyzer/algorithms.py
+-rw-r--r--   0        0        0     4597 2023-04-10 22:21:38.279279 whylabs_toolkit-0.0.6.dev0/whylabs_toolkit/monitor/models/analyzer/analyzer.py
+-rw-r--r--   0        0        0     3242 2023-04-10 22:21:38.279279 whylabs_toolkit-0.0.6.dev0/whylabs_toolkit/monitor/models/analyzer/baseline.py
+-rw-r--r--   0        0        0     2071 2023-04-10 22:21:38.279279 whylabs_toolkit-0.0.6.dev0/whylabs_toolkit/monitor/models/analyzer/targets.py
+-rw-r--r--   0        0        0     4115 2023-04-10 22:21:38.279279 whylabs_toolkit-0.0.6.dev0/whylabs_toolkit/monitor/models/column_schema.py
+-rw-r--r--   0        0        0     3363 2023-04-10 22:21:38.279279 whylabs_toolkit-0.0.6.dev0/whylabs_toolkit/monitor/models/commons.py
+-rw-r--r--   0        0        0     2497 2023-04-10 22:21:38.279279 whylabs_toolkit-0.0.6.dev0/whylabs_toolkit/monitor/models/document.py
+-rw-r--r--   0        0        0     9201 2023-04-10 22:21:38.279279 whylabs_toolkit-0.0.6.dev0/whylabs_toolkit/monitor/models/monitor.py
+-rw-r--r--   0        0        0      574 2023-04-10 22:21:38.279279 whylabs_toolkit-0.0.6.dev0/whylabs_toolkit/monitor/models/segments.py
+-rw-r--r--   0        0        0      961 2023-04-10 22:21:38.279279 whylabs_toolkit-0.0.6.dev0/whylabs_toolkit/monitor/models/utils.py
+-rw-r--r--   0        0        0    75902 2023-04-10 22:21:38.279279 whylabs_toolkit-0.0.6.dev0/whylabs_toolkit/monitor/schema/schema.json
+-rw-r--r--   0        0        0     2512 1970-01-01 00:00:00.000000 whylabs_toolkit-0.0.6.dev0/setup.py
+-rw-r--r--   0        0        0     2244 1970-01-01 00:00:00.000000 whylabs_toolkit-0.0.6.dev0/PKG-INFO
```

### Comparing `whylabs_toolkit-0.0.5.dev1/LICENSE` & `whylabs_toolkit-0.0.6.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `whylabs_toolkit-0.0.5.dev1/README.md` & `whylabs_toolkit-0.0.6.dev0/README.md`

 * *Files identical despite different names*

### Comparing `whylabs_toolkit-0.0.5.dev1/pyproject.toml` & `whylabs_toolkit-0.0.6.dev0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "whylabs-toolkit"
-version = "0.0.5-dev1"
+version = "0.0.6-dev0"
 description = "Whylabs CLI and Helpers package."
 authors = ["Anthony Naddeo <anthony.naddeo@gmail.com>", "Murilo Mendonca <murilommen@gmail.com>"]
 license = "Apache-2.0 license"
 readme = "README.md"
 packages = [{include = "whylabs_toolkit/**/*.py"}]
 include = ["whylabs_toolkit/monitor/schema/schema.json"]
```

### Comparing `whylabs_toolkit-0.0.5.dev1/whylabs_toolkit/container/config_types.py` & `whylabs_toolkit-0.0.6.dev0/whylabs_toolkit/container/config_types.py`

 * *Files identical despite different names*

### Comparing `whylabs_toolkit-0.0.5.dev1/whylabs_toolkit/helpers/config.py` & `whylabs_toolkit-0.0.6.dev0/whylabs_toolkit/helpers/config.py`

 * *Files identical despite different names*

### Comparing `whylabs_toolkit-0.0.5.dev1/whylabs_toolkit/helpers/dataset_profiles.py` & `whylabs_toolkit-0.0.6.dev0/whylabs_toolkit/helpers/dataset_profiles.py`

 * *Files identical despite different names*

### Comparing `whylabs_toolkit-0.0.5.dev1/whylabs_toolkit/helpers/models.py` & `whylabs_toolkit-0.0.6.dev0/whylabs_toolkit/helpers/models.py`

 * *Files identical despite different names*

### Comparing `whylabs_toolkit-0.0.5.dev1/whylabs_toolkit/helpers/monitor_helpers.py` & `whylabs_toolkit-0.0.6.dev0/whylabs_toolkit/helpers/monitor_helpers.py`

 * *Files identical despite different names*

### Comparing `whylabs_toolkit-0.0.5.dev1/whylabs_toolkit/helpers/schema.py` & `whylabs_toolkit-0.0.6.dev0/whylabs_toolkit/helpers/schema.py`

 * *Files identical despite different names*

### Comparing `whylabs_toolkit-0.0.5.dev1/whylabs_toolkit/helpers/utils.py` & `whylabs_toolkit-0.0.6.dev0/whylabs_toolkit/helpers/utils.py`

 * *Files identical despite different names*

### Comparing `whylabs_toolkit-0.0.5.dev1/whylabs_toolkit/monitor/manager/credentials.py` & `whylabs_toolkit-0.0.6.dev0/whylabs_toolkit/monitor/manager/credentials.py`

 * *Files identical despite different names*

### Comparing `whylabs_toolkit-0.0.5.dev1/whylabs_toolkit/monitor/manager/manager.py` & `whylabs_toolkit-0.0.6.dev0/whylabs_toolkit/monitor/manager/manager.py`

 * *Files 16% similar despite different names*

```diff
@@ -18,21 +18,23 @@
 logger = logging.getLogger(__name__)
 
 
 class MonitorManager:
     def __init__(
         self,
         setup: MonitorSetup,
+        eager: Optional[bool] = None,
         notifications_api: Optional[NotificationSettingsApi] = None,
         monitor_api: Optional[ModelsApi] = None,
         config: Config = Config(),
     ) -> None:
         self._setup = setup
         self.__notifications_api = notifications_api or get_notification_api(config=config)
         self.__monitor_api = monitor_api or get_monitor_api(config=config)
+        self.__eager = eager
 
     def _get_existing_notification_actions(self) -> List[str]:
         actions_dict_list = self.__notifications_api.list_notification_actions(org_id=self._setup.credentials.org_id)
         action_ids = []
         for action in actions_dict_list:
             action_ids.append(action.get("id"))
         return action_ids
@@ -71,25 +73,32 @@
 
         if self._setup.monitor:
             self._setup.monitor.actions = [
                 action if isinstance(action, GlobalAction) else GlobalAction(target=action.id)
                 for action in self._setup.monitor.actions
             ]
 
+    def _get_current_monitor_config(self) -> Optional[Any]:
+        monitor_config = self.__monitor_api.get_monitor_config_v3(
+            org_id=self._setup.credentials.org_id, dataset_id=self._setup.credentials.dataset_id
+        )
+        return monitor_config
+
     def dump(self) -> Any:
         self._update_notification_actions()
 
         doc = Document(
             orgId=self._setup.credentials.org_id,
             datasetId=self._setup.credentials.dataset_id,
             granularity=get_model_granularity(
                 org_id=self._setup.credentials.org_id, dataset_id=self._setup.credentials.dataset_id  # type: ignore
             ),
             analyzers=[self._setup.analyzer],
             monitors=[self._setup.monitor],
+            allowPartialTargetBatches=self.__eager,
         )
         return doc.json(indent=2, exclude_none=True)
 
     def validate(self) -> bool:
         try:
             Monitor.validate(self._setup.monitor)
             Analyzer.validate(self._setup.analyzer)
@@ -100,20 +109,29 @@
             validate(instance=json.loads(document), schema=schema)
             return True
         except ValidationError as e:
             raise e
 
     def save(self) -> None:
         if self.validate() is True:
-
             self.__monitor_api.put_analyzer(
                 org_id=self._setup.credentials.org_id,
                 dataset_id=self._setup.credentials.dataset_id,
                 analyzer_id=self._setup.credentials.analyzer_id,
                 body=self._setup.analyzer.dict(exclude_none=True),  # type: ignore
             )
             self.__monitor_api.put_monitor(
                 org_id=self._setup.credentials.org_id,
                 dataset_id=self._setup.credentials.dataset_id,
                 monitor_id=self._setup.credentials.monitor_id,
                 body=self._setup.monitor.dict(exclude_none=True),  # type: ignore
             )
+        if self.__eager is not None:
+            current_config = self._get_current_monitor_config()
+
+            if self.__eager != current_config.get("allowPartialTargetBatches"):  # type: ignore
+                current_config["allowPartialTargetBatches"] = self.__eager  # type: ignore
+                self.__monitor_api.put_monitor_config_v3(
+                    org_id=self._setup.credentials.org_id,
+                    dataset_id=self._setup.credentials.dataset_id,
+                    body=current_config,
+                )
```

### Comparing `whylabs_toolkit-0.0.5.dev1/whylabs_toolkit/monitor/manager/monitor_setup.py` & `whylabs_toolkit-0.0.6.dev0/whylabs_toolkit/monitor/manager/monitor_setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -133,17 +133,23 @@
     def mode(self, mode: Union[EveryAnomalyMode, DigestMode]) -> None:
         self._monitor_mode = mode
 
     def _validate_columns_input(self, columns: List[str]) -> bool:
         if type(columns) != list or not all(isinstance(column, str) for column in columns):
             raise ValueError("columns argument must be a List of strings")
 
-        if "group:" in columns[0]:
+        group_columns = ColumnGroups.__members__.values()
+        allowed_groups = any(col in group_columns for col in columns)
+
+        if allowed_groups:
             return True
 
+        if "group:" in columns and not allowed_groups:
+            raise ValueError(f"group:[group_type] should be one of {group_columns}")
+
         schema = self._models_api.get_entity_schema(
             org_id=self.credentials.org_id, dataset_id=self.credentials.dataset_id
         )
         columns_dict = schema["columns"]
 
         for col in columns:
             if col not in columns_dict.keys():
@@ -175,14 +181,18 @@
             end_date = end_date.replace(tzinfo=pytz.UTC)
         # TODO make baseline nullable and default baseline to be TrailingWindowBaseline(size=14)
         self._analyzer_config.baseline = TimeRangeBaseline(  # type: ignore
             range=TimeRange(start=start_date, end=end_date)
         )
 
     def __set_analyzer(self) -> None:
+        self.__configure_target_matrix()
+
+        self.__set_dataset_matrix_for_dataset_metric()
+
         self.analyzer = Analyzer(
             id=self.credentials.analyzer_id,
             displayName=self.credentials.analyzer_id,
             targetMatrix=self._target_matrix,
             tags=[],
             schedule=self._analyzer_schedule,
             config=self._analyzer_config,
@@ -202,24 +212,35 @@
             actions=monitor_actions,
         )
 
     def __configure_target_matrix(self) -> None:
         self._target_matrix = self._target_matrix or ColumnMatrix(
             include=self._target_columns or ["*"], exclude=self._exclude_columns, segments=[]
         )
-        if self.analyzer:
-            if isinstance(self.analyzer.config.metric, DatasetMetric):
-                self._target_matrix = DatasetMatrix()
+
+    def __set_dataset_matrix_for_dataset_metric(self) -> None:
+        if self._analyzer_config:
+            if isinstance(self._analyzer_config.metric, DatasetMetric) and isinstance(
+                self._target_matrix, ColumnMatrix
+            ):
+                self._target_matrix = DatasetMatrix(segments=[])
+                return None
+
+            elif isinstance(self._target_matrix, DatasetMatrix) and not isinstance(
+                self._analyzer_config.metric, DatasetMetric
+            ):
+                self._target_matrix = None
+                self.__configure_target_matrix()
+                return None
 
     def apply(self) -> None:
         monitor_mode = self._monitor_mode or DigestMode()
         actions = self._monitor_actions or []
         self._analyzer_schedule = self._analyzer_schedule or FixedCadenceSchedule(
             cadence=get_model_granularity(
                 org_id=self.credentials.org_id, dataset_id=self.credentials.dataset_id  # type: ignore
             )
         )
 
         self.__set_monitor(monitor_mode=monitor_mode, monitor_actions=actions)
 
-        self.__configure_target_matrix()
         self.__set_analyzer()
```

### Comparing `whylabs_toolkit-0.0.5.dev1/whylabs_toolkit/monitor/models/__init__.py` & `whylabs_toolkit-0.0.6.dev0/whylabs_toolkit/monitor/models/__init__.py`

 * *Files identical despite different names*

### Comparing `whylabs_toolkit-0.0.5.dev1/whylabs_toolkit/monitor/models/analyzer/__init__.py` & `whylabs_toolkit-0.0.6.dev0/whylabs_toolkit/monitor/models/analyzer/__init__.py`

 * *Files identical despite different names*

### Comparing `whylabs_toolkit-0.0.5.dev1/whylabs_toolkit/monitor/models/analyzer/algorithms.py` & `whylabs_toolkit-0.0.6.dev0/whylabs_toolkit/monitor/models/analyzer/algorithms.py`

 * *Files identical despite different names*

### Comparing `whylabs_toolkit-0.0.5.dev1/whylabs_toolkit/monitor/models/analyzer/analyzer.py` & `whylabs_toolkit-0.0.6.dev0/whylabs_toolkit/monitor/models/analyzer/analyzer.py`

 * *Files identical despite different names*

### Comparing `whylabs_toolkit-0.0.5.dev1/whylabs_toolkit/monitor/models/analyzer/baseline.py` & `whylabs_toolkit-0.0.6.dev0/whylabs_toolkit/monitor/models/analyzer/baseline.py`

 * *Files identical despite different names*

### Comparing `whylabs_toolkit-0.0.5.dev1/whylabs_toolkit/monitor/models/analyzer/targets.py` & `whylabs_toolkit-0.0.6.dev0/whylabs_toolkit/monitor/models/analyzer/targets.py`

 * *Files identical despite different names*

### Comparing `whylabs_toolkit-0.0.5.dev1/whylabs_toolkit/monitor/models/column_schema.py` & `whylabs_toolkit-0.0.6.dev0/whylabs_toolkit/monitor/models/column_schema.py`

 * *Files identical despite different names*

### Comparing `whylabs_toolkit-0.0.5.dev1/whylabs_toolkit/monitor/models/commons.py` & `whylabs_toolkit-0.0.6.dev0/whylabs_toolkit/monitor/models/commons.py`

 * *Files identical despite different names*

### Comparing `whylabs_toolkit-0.0.5.dev1/whylabs_toolkit/monitor/models/document.py` & `whylabs_toolkit-0.0.6.dev0/whylabs_toolkit/monitor/models/document.py`

 * *Files identical despite different names*

### Comparing `whylabs_toolkit-0.0.5.dev1/whylabs_toolkit/monitor/models/monitor.py` & `whylabs_toolkit-0.0.6.dev0/whylabs_toolkit/monitor/models/monitor.py`

 * *Files identical despite different names*

### Comparing `whylabs_toolkit-0.0.5.dev1/whylabs_toolkit/monitor/models/segments.py` & `whylabs_toolkit-0.0.6.dev0/whylabs_toolkit/monitor/models/segments.py`

 * *Files identical despite different names*

### Comparing `whylabs_toolkit-0.0.5.dev1/whylabs_toolkit/monitor/models/utils.py` & `whylabs_toolkit-0.0.6.dev0/whylabs_toolkit/monitor/models/utils.py`

 * *Files identical despite different names*

### Comparing `whylabs_toolkit-0.0.5.dev1/whylabs_toolkit/monitor/schema/schema.json` & `whylabs_toolkit-0.0.6.dev0/whylabs_toolkit/monitor/schema/schema.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8839441311883385%*

 * *Differences: {"'$id'": "'https://gitlab.com/whylabs/core/montor-schema/-/blob/main/schema/schema.json'",*

 * * "'definitions'": "{'ColumnMatrix': {'properties': {'excludeSegments': OrderedDict([('title', "*

 * *                  "'Excludesegments'), ('description', 'List of segments to be excluded'), "*

 * *                  "('maxItems', 1000), ('type', 'array'), ('items', OrderedDict([('$ref', "*

 * *                  "'#/definitions/Segment')]))])}}, 'DatasetMatrix': {'properties': "*

 * *                  "{'excludeSegments': OrderedDict([( […]*

```diff
@@ -1,17 +1,20 @@
 {
+    "$id": "https://gitlab.com/whylabs/core/montor-schema/-/blob/main/schema/schema.json",
     "$version": "1.0",
     "additionalProperties": false,
     "definitions": {
         "AlgorithmType": {
             "description": "Specify the algorithm type.",
             "enum": [
                 "expected",
                 "column_list",
                 "comparison",
+                "list_comparison",
+                "frequent_string_comparison",
                 "diff",
                 "drift",
                 "stddev",
                 "seasonal",
                 "fixed",
                 "experimental"
             ],
@@ -42,27 +45,35 @@
                         "mapping": {
                             "column_list": "#/definitions/ColumnListChangeConfig",
                             "comparison": "#/definitions/ComparisonConfig",
                             "diff": "#/definitions/DiffConfig",
                             "drift": "#/definitions/DriftConfig",
                             "experimental": "#/definitions/ExperimentalConfig",
                             "fixed": "#/definitions/FixedThresholdsConfig",
+                            "frequent_string_comparison": "#/definitions/FrequentStringComparisonConfig",
+                            "list_comparison": "#/definitions/ListComparisonConfig",
                             "seasonal": "#/definitions/SeasonalConfig",
                             "stddev": "#/definitions/StddevConfig"
                         },
                         "propertyName": "type"
                     },
                     "oneOf": [
                         {
                             "$ref": "#/definitions/DiffConfig"
                         },
                         {
                             "$ref": "#/definitions/ComparisonConfig"
                         },
                         {
+                            "$ref": "#/definitions/ListComparisonConfig"
+                        },
+                        {
+                            "$ref": "#/definitions/FrequentStringComparisonConfig"
+                        },
+                        {
                             "$ref": "#/definitions/ColumnListChangeConfig"
                         },
                         {
                             "$ref": "#/definitions/FixedThresholdsConfig"
                         },
                         {
                             "$ref": "#/definitions/StddevConfig"
@@ -290,14 +301,24 @@
             "type": "string"
         },
         "ColumnListChangeConfig": {
             "additionalProperties": false,
             "description": "Compare whether the target is equal to a value or not.\n\nThis is useful to detect data type change, for instance.",
             "properties": {
                 "baseline": {
+                    "description": "A baseline for running the analyzer.",
+                    "discriminator": {
+                        "mapping": {
+                            "CurrentBatch": "#/definitions/SingleBatchBaseline",
+                            "Reference": "#/definitions/ReferenceProfileId",
+                            "TimeRange": "#/definitions/TimeRangeBaseline",
+                            "TrailingWindow": "#/definitions/TrailingWindowBaseline"
+                        },
+                        "propertyName": "type"
+                    },
                     "oneOf": [
                         {
                             "$ref": "#/definitions/TrailingWindowBaseline"
                         },
                         {
                             "$ref": "#/definitions/ReferenceProfileId"
                         },
@@ -343,15 +364,15 @@
                         "type": "string"
                     },
                     "description": "Extra parameters for the algorithm",
                     "title": "Params",
                     "type": "object"
                 },
                 "schemaVersion": {
-                    "description": "The schema version of an algorithm. Typically this valueis not required.",
+                    "description": "The schema version of an algorithm. Typically this value is not required.",
                     "title": "SchemaVersion",
                     "type": "integer"
                 },
                 "type": {
                     "enum": [
                         "column_list"
                     ],
@@ -384,14 +405,23 @@
                             }
                         ]
                     },
                     "maxItems": 1000,
                     "title": "Exclude",
                     "type": "array"
                 },
+                "excludeSegments": {
+                    "description": "List of segments to be excluded",
+                    "items": {
+                        "$ref": "#/definitions/Segment"
+                    },
+                    "maxItems": 1000,
+                    "title": "Excludesegments",
+                    "type": "array"
+                },
                 "include": {
                     "description": "List of allowed fields/features/columns. Could be a grouping as well.",
                     "items": {
                         "anyOf": [
                             {
                                 "$ref": "#/definitions/ColumnGroups"
                             },
@@ -461,17 +491,27 @@
                 "dataType"
             ],
             "title": "ColumnSchema",
             "type": "object"
         },
         "ComparisonConfig": {
             "additionalProperties": false,
-            "description": "Compare whether the target against a value or against a baseline's metric.\n\nThis is useful to detect data type change, for instance.",
+            "description": "Compare whether the target against either an expect value or against the  baseline.\n\nThis is useful to detect data type change, for instance.",
             "properties": {
                 "baseline": {
+                    "description": "A baseline for running the analyzer.",
+                    "discriminator": {
+                        "mapping": {
+                            "CurrentBatch": "#/definitions/SingleBatchBaseline",
+                            "Reference": "#/definitions/ReferenceProfileId",
+                            "TimeRange": "#/definitions/TimeRangeBaseline",
+                            "TrailingWindow": "#/definitions/TrailingWindowBaseline"
+                        },
+                        "propertyName": "type"
+                    },
                     "oneOf": [
                         {
                             "$ref": "#/definitions/TrailingWindowBaseline"
                         },
                         {
                             "$ref": "#/definitions/ReferenceProfileId"
                         },
@@ -523,15 +563,15 @@
                         "type": "string"
                     },
                     "description": "Extra parameters for the algorithm",
                     "title": "Params",
                     "type": "object"
                 },
                 "schemaVersion": {
-                    "description": "The schema version of an algorithm. Typically this valueis not required.",
+                    "description": "The schema version of an algorithm. Typically this value is not required.",
                     "title": "SchemaVersion",
                     "type": "integer"
                 },
                 "type": {
                     "enum": [
                         "comparison"
                     ],
@@ -592,14 +632,23 @@
             "title": "CronSchedule",
             "type": "object"
         },
         "DatasetMatrix": {
             "additionalProperties": false,
             "description": "Define the matrix of fields and segments to fan out for monitoring.\n\n.",
             "properties": {
+                "excludeSegments": {
+                    "description": "List of segments to be excluded",
+                    "items": {
+                        "$ref": "#/definitions/Segment"
+                    },
+                    "maxItems": 1000,
+                    "title": "Excludesegments",
+                    "type": "array"
+                },
                 "segments": {
                     "description": "List of targeted segments. If not set, default to the overall segment",
                     "items": {
                         "$ref": "#/definitions/Segment"
                     },
                     "maxItems": 1000,
                     "title": "Segments",
@@ -642,14 +691,24 @@
             "type": "string"
         },
         "DiffConfig": {
             "additionalProperties": false,
             "description": "Detecting the differences between two numerical metrics.",
             "properties": {
                 "baseline": {
+                    "description": "A baseline for running the analyzer.",
+                    "discriminator": {
+                        "mapping": {
+                            "CurrentBatch": "#/definitions/SingleBatchBaseline",
+                            "Reference": "#/definitions/ReferenceProfileId",
+                            "TimeRange": "#/definitions/TimeRangeBaseline",
+                            "TrailingWindow": "#/definitions/TrailingWindowBaseline"
+                        },
+                        "propertyName": "type"
+                    },
                     "oneOf": [
                         {
                             "$ref": "#/definitions/TrailingWindowBaseline"
                         },
                         {
                             "$ref": "#/definitions/ReferenceProfileId"
                         },
@@ -687,15 +746,15 @@
                         "type": "string"
                     },
                     "description": "Extra parameters for the algorithm",
                     "title": "Params",
                     "type": "object"
                 },
                 "schemaVersion": {
-                    "description": "The schema version of an algorithm. Typically this valueis not required.",
+                    "description": "The schema version of an algorithm. Typically this value is not required.",
                     "title": "SchemaVersion",
                     "type": "integer"
                 },
                 "threshold": {
                     "description": "The minimum threshold that will trigger an anomaly. The monitor detect the difference betweenthe target's metric and the baseline metric. Both of these metrics MUST be in rolled up form",
                     "title": "Threshold",
                     "type": "number"
@@ -802,14 +861,24 @@
                         "kl_divergence",
                         "variation_distance"
                     ],
                     "title": "Algorithm",
                     "type": "string"
                 },
                 "baseline": {
+                    "description": "A baseline for running the analyzer.",
+                    "discriminator": {
+                        "mapping": {
+                            "CurrentBatch": "#/definitions/SingleBatchBaseline",
+                            "Reference": "#/definitions/ReferenceProfileId",
+                            "TimeRange": "#/definitions/TimeRangeBaseline",
+                            "TrailingWindow": "#/definitions/TrailingWindowBaseline"
+                        },
+                        "propertyName": "type"
+                    },
                     "oneOf": [
                         {
                             "$ref": "#/definitions/TrailingWindowBaseline"
                         },
                         {
                             "$ref": "#/definitions/ReferenceProfileId"
                         },
@@ -843,15 +912,15 @@
                         "type": "string"
                     },
                     "description": "Extra parameters for the algorithm",
                     "title": "Params",
                     "type": "object"
                 },
                 "schemaVersion": {
-                    "description": "The schema version of an algorithm. Typically this valueis not required.",
+                    "description": "The schema version of an algorithm. Typically this value is not required.",
                     "title": "SchemaVersion",
                     "type": "integer"
                 },
                 "threshold": {
                     "default": 0.7,
                     "description": "The threshold for the distance algorithm. Depending on the algorithm, this thresholdis used for greater than or less than comparison.",
                     "title": "Threshold",
@@ -985,14 +1054,24 @@
             "type": "object"
         },
         "ExperimentalConfig": {
             "additionalProperties": false,
             "description": "Experimental algorithm that is not standardized by the above ones yet.",
             "properties": {
                 "baseline": {
+                    "description": "A baseline for running the analyzer.",
+                    "discriminator": {
+                        "mapping": {
+                            "CurrentBatch": "#/definitions/SingleBatchBaseline",
+                            "Reference": "#/definitions/ReferenceProfileId",
+                            "TimeRange": "#/definitions/TimeRangeBaseline",
+                            "TrailingWindow": "#/definitions/TrailingWindowBaseline"
+                        },
+                        "propertyName": "type"
+                    },
                     "oneOf": [
                         {
                             "$ref": "#/definitions/TrailingWindowBaseline"
                         },
                         {
                             "$ref": "#/definitions/ReferenceProfileId"
                         },
@@ -1033,15 +1112,15 @@
                         "type": "string"
                     },
                     "description": "Extra parameters for the algorithm",
                     "title": "Params",
                     "type": "object"
                 },
                 "schemaVersion": {
-                    "description": "The schema version of an algorithm. Typically this valueis not required.",
+                    "description": "The schema version of an algorithm. Typically this value is not required.",
                     "title": "SchemaVersion",
                     "type": "integer"
                 },
                 "stub": {
                     "allOf": [
                         {
                             "$ref": "#/definitions/AlgorithmType"
@@ -1135,15 +1214,15 @@
                         "type": "string"
                     },
                     "description": "Extra parameters for the algorithm",
                     "title": "Params",
                     "type": "object"
                 },
                 "schemaVersion": {
-                    "description": "The schema version of an algorithm. Typically this valueis not required.",
+                    "description": "The schema version of an algorithm. Typically this value is not required.",
                     "title": "SchemaVersion",
                     "type": "integer"
                 },
                 "type": {
                     "enum": [
                         "fixed"
                     ],
@@ -1159,14 +1238,101 @@
             "required": [
                 "metric",
                 "type"
             ],
             "title": "FixedThresholdsConfig",
             "type": "object"
         },
+        "FrequentStringComparisonConfig": {
+            "additionalProperties": false,
+            "description": "Compare whether target against a list of values.",
+            "properties": {
+                "baseline": {
+                    "description": "A baseline for running the analyzer.",
+                    "discriminator": {
+                        "mapping": {
+                            "CurrentBatch": "#/definitions/SingleBatchBaseline",
+                            "Reference": "#/definitions/ReferenceProfileId",
+                            "TimeRange": "#/definitions/TimeRangeBaseline",
+                            "TrailingWindow": "#/definitions/TrailingWindowBaseline"
+                        },
+                        "propertyName": "type"
+                    },
+                    "oneOf": [
+                        {
+                            "$ref": "#/definitions/TrailingWindowBaseline"
+                        },
+                        {
+                            "$ref": "#/definitions/ReferenceProfileId"
+                        },
+                        {
+                            "$ref": "#/definitions/TimeRangeBaseline"
+                        },
+                        {
+                            "$ref": "#/definitions/SingleBatchBaseline"
+                        }
+                    ],
+                    "title": "Baseline"
+                },
+                "metric": {
+                    "enum": [
+                        "frequent_items"
+                    ],
+                    "title": "Metric",
+                    "type": "string"
+                },
+                "operator": {
+                    "allOf": [
+                        {
+                            "$ref": "#/definitions/FrequentStringComparisonOperator"
+                        }
+                    ],
+                    "description": "The operator for the comparison."
+                },
+                "params": {
+                    "additionalProperties": {
+                        "maxLength": 1000,
+                        "type": "string"
+                    },
+                    "description": "Extra parameters for the algorithm",
+                    "title": "Params",
+                    "type": "object"
+                },
+                "schemaVersion": {
+                    "description": "The schema version of an algorithm. Typically this value is not required.",
+                    "title": "SchemaVersion",
+                    "type": "integer"
+                },
+                "type": {
+                    "enum": [
+                        "frequent_string_comparison"
+                    ],
+                    "title": "Type",
+                    "type": "string"
+                }
+            },
+            "required": [
+                "metric",
+                "type",
+                "operator",
+                "baseline"
+            ],
+            "title": "FrequentStringComparisonConfig",
+            "type": "object"
+        },
+        "FrequentStringComparisonOperator": {
+            "description": "Operators for performing a comparison.",
+            "enum": [
+                "eq",
+                "target_includes_all_baseline",
+                "baseline_includes_all_target"
+            ],
+            "title": "FrequentStringComparisonOperator",
+            "type": "string"
+        },
         "GlobalAction": {
             "additionalProperties": false,
             "description": "Actions that are configured at the team/organization level.",
             "properties": {
                 "target": {
                     "description": "The unique action ID in the platform",
                     "maxLength": 100,
@@ -1214,14 +1380,116 @@
             },
             "required": [
                 "type"
             ],
             "title": "ImmediateSchedule",
             "type": "object"
         },
+        "ListComparisonConfig": {
+            "additionalProperties": false,
+            "description": "Compare a target list of values against a baseline list of values.",
+            "properties": {
+                "baseline": {
+                    "description": "A baseline for running the analyzer.",
+                    "discriminator": {
+                        "mapping": {
+                            "CurrentBatch": "#/definitions/SingleBatchBaseline",
+                            "Reference": "#/definitions/ReferenceProfileId",
+                            "TimeRange": "#/definitions/TimeRangeBaseline",
+                            "TrailingWindow": "#/definitions/TrailingWindowBaseline"
+                        },
+                        "propertyName": "type"
+                    },
+                    "oneOf": [
+                        {
+                            "$ref": "#/definitions/TrailingWindowBaseline"
+                        },
+                        {
+                            "$ref": "#/definitions/ReferenceProfileId"
+                        },
+                        {
+                            "$ref": "#/definitions/TimeRangeBaseline"
+                        },
+                        {
+                            "$ref": "#/definitions/SingleBatchBaseline"
+                        }
+                    ],
+                    "title": "Baseline"
+                },
+                "expected": {
+                    "description": "The expected values of the equality. If the value is not set we will extract the corresponding metric from the baseline and perform the comparison",
+                    "items": {
+                        "$ref": "#/definitions/ExpectedValue"
+                    },
+                    "title": "Expected",
+                    "type": "array"
+                },
+                "metric": {
+                    "anyOf": [
+                        {
+                            "$ref": "#/definitions/DatasetMetric"
+                        },
+                        {
+                            "$ref": "#/definitions/SimpleColumnMetric"
+                        },
+                        {
+                            "maxLength": 100,
+                            "type": "string"
+                        }
+                    ],
+                    "description": "The target metric. This field cannot be change once the analyzer is created.",
+                    "title": "Metric"
+                },
+                "operator": {
+                    "allOf": [
+                        {
+                            "$ref": "#/definitions/ListComparisonOperator"
+                        }
+                    ],
+                    "description": "The operator for the comparison. The right hand side is the target batch's metric. The left handside is the expected value or a baseline's metric."
+                },
+                "params": {
+                    "additionalProperties": {
+                        "maxLength": 1000,
+                        "type": "string"
+                    },
+                    "description": "Extra parameters for the algorithm",
+                    "title": "Params",
+                    "type": "object"
+                },
+                "schemaVersion": {
+                    "description": "The schema version of an algorithm. Typically this value is not required.",
+                    "title": "SchemaVersion",
+                    "type": "integer"
+                },
+                "type": {
+                    "enum": [
+                        "list_comparison"
+                    ],
+                    "title": "Type",
+                    "type": "string"
+                }
+            },
+            "required": [
+                "metric",
+                "type",
+                "operator"
+            ],
+            "title": "ListComparisonConfig",
+            "type": "object"
+        },
+        "ListComparisonOperator": {
+            "description": "Operators for performing a comparison.",
+            "enum": [
+                "in",
+                "not_in"
+            ],
+            "title": "ListComparisonOperator",
+            "type": "string"
+        },
         "Metadata": {
             "additionalProperties": false,
             "description": "Metadata for a top-level objects such as monitors, analyzers, and schema.\n\nThis object is managed by WhyLabs. Any user-provided values will be ignored on WhyLabs side.",
             "properties": {
                 "author": {
                     "description": "The author of the change. It can be an API Key ID, a user ID, or a WhyLabs system ID.",
                     "maxLength": 100,
@@ -1346,14 +1614,22 @@
                             "$ref": "#/definitions/DigestMode"
                         }
                     ],
                     "title": "Mode"
                 },
                 "schedule": {
                     "description": "Schedule of the monitor. We only support hourly monitor at the finest granularity",
+                    "discriminator": {
+                        "mapping": {
+                            "cron": "#/definitions/CronSchedule",
+                            "fixed": "#/definitions/FixedCadenceSchedule",
+                            "immediate": "#/definitions/ImmediateSchedule"
+                        },
+                        "propertyName": "type"
+                    },
                     "oneOf": [
                         {
                             "$ref": "#/definitions/FixedCadenceSchedule"
                         },
                         {
                             "$ref": "#/definitions/CronSchedule"
                         },
@@ -1511,15 +1787,15 @@
                         "type": "string"
                     },
                     "description": "Extra parameters for the algorithm",
                     "title": "Params",
                     "type": "object"
                 },
                 "schemaVersion": {
-                    "description": "The schema version of an algorithm. Typically this valueis not required.",
+                    "description": "The schema version of an algorithm. Typically this value is not required.",
                     "title": "SchemaVersion",
                     "type": "integer"
                 },
                 "stddevFactor": {
                     "default": 1.0,
                     "description": "The multiplier factor for calculating upper bounds and lower bounds from the prediction.",
                     "title": "Stddevfactor",
@@ -1751,14 +2027,23 @@
             "type": "object"
         },
         "StddevConfig": {
             "additionalProperties": false,
             "description": "Calculates upper bounds and lower bounds based on stddev from a series of numbers.\n\nAn analyzer using stddev for a window of time range.\n\nThis calculation will fall back to Poisson distribution if there is only 1 value in the baseline.\nFor 2 values, we use the formula sqrt((x_i - avg(x))^2 / n - 1)",
             "properties": {
                 "baseline": {
+                    "description": "A baseline for running the analyzer.",
+                    "discriminator": {
+                        "mapping": {
+                            "Reference": "#/definitions/ReferenceProfileId",
+                            "TimeRange": "#/definitions/TimeRangeBaseline",
+                            "TrailingWindow": "#/definitions/TrailingWindowBaseline"
+                        },
+                        "propertyName": "type"
+                    },
                     "oneOf": [
                         {
                             "$ref": "#/definitions/TrailingWindowBaseline"
                         },
                         {
                             "$ref": "#/definitions/TimeRangeBaseline"
                         },
@@ -1813,15 +2098,15 @@
                         "type": "string"
                     },
                     "description": "Extra parameters for the algorithm",
                     "title": "Params",
                     "type": "object"
                 },
                 "schemaVersion": {
-                    "description": "The schema version of an algorithm. Typically this valueis not required.",
+                    "description": "The schema version of an algorithm. Typically this value is not required.",
                     "title": "SchemaVersion",
                     "type": "integer"
                 },
                 "type": {
                     "enum": [
                         "stddev"
                     ],
@@ -1834,15 +2119,15 @@
                 "type",
                 "baseline"
             ],
             "title": "StddevConfig",
             "type": "object"
         },
         "ThresholdType": {
-            "description": "By default an anomaly will be generated when the target is above or below the baseline\n    by the specified threshold.\n\n    If its only desirable to alert when the target is above the\n    baseline and not the other way around, specify upper for your ThresholdType.",
+            "description": "Threshold Type declaring the upper and lower bound.\n\n    By default an anomaly will be generated when the target is above or below the baseline\n    by the specified threshold.\n\n    If its only desirable to alert when the target is above the\n    baseline and not the other way around, specify upper for your ThresholdType.\n    ",
             "enum": [
                 "lower",
                 "upper"
             ],
             "title": "ThresholdType",
             "type": "string"
         },
@@ -1981,15 +2266,15 @@
             "title": "WeightConfig",
             "type": "object"
         }
     },
     "description": "The main document that dictates how the monitor should be run. This document is managed by WhyLabs internally.",
     "properties": {
         "allowPartialTargetBatches": {
-            "description": "The standard \n        flow waits for a target batch as defined by the dataset granularity \n        setting to conclude before running analysis. For example, on monthly datasets datapoints in the \n        current month would be analyzed at midnight on the last day of the month anticipating additional \n        data may be profiled. With allowPartialTargetBatches enabled a target batch may be analyzed as \n        soon as the data is present and dataReadinessDuration/batchCooldownPeriod (if configured) \n        conditions have been met. This can be ideal for data pipelines that upload a single profile per \n        dataset granularity to reduce the waiting time for analysis.",
+            "description": "The standard\n        flow waits for a target batch as defined by the dataset granularity\n        setting to conclude before running analysis. For example, on monthly datasets datapoints in the\n        current month would be analyzed at midnight on the last day of the month anticipating additional\n        data may be profiled. With allowPartialTargetBatches enabled a target batch may be analyzed as\n        soon as the data is present and dataReadinessDuration/batchCooldownPeriod (if configured)\n        conditions have been met. This can be ideal for data pipelines that upload a single profile per\n        dataset granularity to reduce the waiting time for analysis.",
             "title": "AllowPartialTargetBatches",
             "type": "boolean"
         },
         "analyzers": {
             "description": "List of analyzers",
             "items": {
                 "$ref": "#/definitions/Analyzer"
```

### Comparing `whylabs_toolkit-0.0.5.dev1/setup.py` & `whylabs_toolkit-0.0.6.dev0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
  'pytz>=2022.7.1,<2023.0.0',
  'types-pytz>=2022.7.1.0,<2023.0.0.0',
  'whylabs-client>=0.4.4,<0.5.0',
  'whylogs>=1.1.26,<2.0.0']
 
 setup_kwargs = {
     'name': 'whylabs-toolkit',
-    'version': '0.0.5.dev1',
+    'version': '0.0.6.dev0',
     'description': 'Whylabs CLI and Helpers package.',
     'long_description': "# WhyLabs Toolkit\n\nThe WhyLabs Toolkit package contains helper methods to help users interact with our internal APIs. Users will benefit from using it if they want to abstract some of WhyLabs' internal logic and also automate recurring API calls.\n\n\n## Basic usage\nTo start using the `whylabs_toolkit` package, install it from PyPI with:\n```bash\npip install whylabs_toolkit\n``` \n\n## Packages\n\nThe available packages that we have enable different use-cases for the `whylabs_toolkit`. To get started, navigate to one of the following sections and find useful tutorials there.\n\n| Package             | Usage                |\n|---------------------|----------------------|\n| [Monitor Manager](/whylabs_toolkit/monitor/manager/README.md) | Author and modify existing WhyLabs monitor with Python |\n| [WhyLabs Helpers](/whylabs_toolkit/helpers/README.md) | Interact with and modify your Datasets and ML Models specs in WhyLabs. |\n\n## Development\n\nTo start contributing, you will manage dependencies with [Poetry](https://python-poetry.org/) and also a handful of `Makefile` commands. To install all necessary dependencies and activate the virtual environment, run:\n\n```bash\nmake setup && poetry shell\n```\n\n## Get in touch\nIf you want to learn more how you can benefit from this package or if there is anything missing, please [contact our support](https://whylabs.ai/contact-us), we'll be more than happy to help you!",
     'author': 'Anthony Naddeo',
     'author_email': 'anthony.naddeo@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `whylabs_toolkit-0.0.5.dev1/PKG-INFO` & `whylabs_toolkit-0.0.6.dev0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whylabs-toolkit
-Version: 0.0.5.dev1
+Version: 0.0.6.dev0
 Summary: Whylabs CLI and Helpers package.
 License: Apache-2.0 license
 Author: Anthony Naddeo
 Author-email: anthony.naddeo@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

