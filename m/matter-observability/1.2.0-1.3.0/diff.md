# Comparing `tmp/matter_observability-1.2.0-py3-none-any.whl.zip` & `tmp/matter_observability-1.3.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,23 @@
-Zip file size: 10739 bytes, number of entries: 20
+Zip file size: 11245 bytes, number of entries: 21
 -rw-r--r--  2.0 unx      134 b- defN 20-Feb-02 00:00 matter_observability/__about__.py
 -rw-r--r--  2.0 unx      112 b- defN 20-Feb-02 00:00 matter_observability/__init__.py
--rw-r--r--  2.0 unx      293 b- defN 20-Feb-02 00:00 matter_observability/config.py
--rw-r--r--  2.0 unx       48 b- defN 20-Feb-02 00:00 matter_observability/fastapi/__init__.py
+-rw-r--r--  2.0 unx      287 b- defN 20-Feb-02 00:00 matter_observability/config.py
+-rw-r--r--  2.0 unx      132 b- defN 20-Feb-02 00:00 matter_observability/exceptions.py
+-rw-r--r--  2.0 unx      133 b- defN 20-Feb-02 00:00 matter_observability/fastapi/__init__.py
 -rw-r--r--  2.0 unx      641 b- defN 20-Feb-02 00:00 matter_observability/fastapi/request_id.py
--rw-r--r--  2.0 unx      513 b- defN 20-Feb-02 00:00 matter_observability/fastapi/utils.py
--rw-r--r--  2.0 unx       57 b- defN 20-Feb-02 00:00 matter_observability/logging/__init__.py
--rw-r--r--  2.0 unx     1630 b- defN 20-Feb-02 00:00 matter_observability/logging/logging_config.py
+-rw-r--r--  2.0 unx      817 b- defN 20-Feb-02 00:00 matter_observability/fastapi/utils.py
+-rw-r--r--  2.0 unx       73 b- defN 20-Feb-02 00:00 matter_observability/logging/__init__.py
+-rw-r--r--  2.0 unx     1671 b- defN 20-Feb-02 00:00 matter_observability/logging/logging_config.py
 -rw-r--r--  2.0 unx      316 b- defN 20-Feb-02 00:00 matter_observability/metrics/__init__.py
 -rw-r--r--  2.0 unx      761 b- defN 20-Feb-02 00:00 matter_observability/metrics/custom_metrics.py
 -rw-r--r--  2.0 unx     2428 b- defN 20-Feb-02 00:00 matter_observability/metrics/decorators.py
 -rw-r--r--  2.0 unx      473 b- defN 20-Feb-02 00:00 matter_observability/metrics/labeled_counter.py
 -rw-r--r--  2.0 unx      489 b- defN 20-Feb-02 00:00 matter_observability/metrics/labeled_gauge.py
 -rw-r--r--  2.0 unx      708 b- defN 20-Feb-02 00:00 matter_observability/metrics/labeled_gauge_duration.py
 -rw-r--r--  2.0 unx      421 b- defN 20-Feb-02 00:00 matter_observability/metrics/labeled_metric.py
--rw-r--r--  2.0 unx      676 b- defN 20-Feb-02 00:00 matter_observability/metrics/utils.py
-?rw-r--r--  2.0 unx     5812 b- defN 20-Feb-02 00:00 matter_observability-1.2.0.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 matter_observability-1.2.0.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1068 b- defN 20-Feb-02 00:00 matter_observability-1.2.0.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx     1908 b- defN 20-Feb-02 00:00 matter_observability-1.2.0.dist-info/RECORD
-20 files, 18575 bytes uncompressed, 7517 bytes compressed:  59.5%
+-rw-r--r--  2.0 unx      903 b- defN 20-Feb-02 00:00 matter_observability/metrics/utils.py
+?rw-r--r--  2.0 unx     5852 b- defN 20-Feb-02 00:00 matter_observability-1.3.0.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 matter_observability-1.3.0.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1068 b- defN 20-Feb-02 00:00 matter_observability-1.3.0.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx     1999 b- defN 20-Feb-02 00:00 matter_observability-1.3.0.dist-info/RECORD
+21 files, 19505 bytes uncompressed, 7879 bytes compressed:  59.6%
```

## zipnote {}

```diff
@@ -3,14 +3,17 @@
 
 Filename: matter_observability/__init__.py
 Comment: 
 
 Filename: matter_observability/config.py
 Comment: 
 
+Filename: matter_observability/exceptions.py
+Comment: 
+
 Filename: matter_observability/fastapi/__init__.py
 Comment: 
 
 Filename: matter_observability/fastapi/request_id.py
 Comment: 
 
 Filename: matter_observability/fastapi/utils.py
@@ -42,20 +45,20 @@
 
 Filename: matter_observability/metrics/labeled_metric.py
 Comment: 
 
 Filename: matter_observability/metrics/utils.py
 Comment: 
 
-Filename: matter_observability-1.2.0.dist-info/METADATA
+Filename: matter_observability-1.3.0.dist-info/METADATA
 Comment: 
 
-Filename: matter_observability-1.2.0.dist-info/WHEEL
+Filename: matter_observability-1.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: matter_observability-1.2.0.dist-info/licenses/LICENSE
+Filename: matter_observability-1.3.0.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: matter_observability-1.2.0.dist-info/RECORD
+Filename: matter_observability-1.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## matter_observability/__about__.py

```diff
@@ -1,4 +1,4 @@
 # SPDX-FileCopyrightText: 2023-present Rômulo Jales <romulo@thisismatter.com>
 #
 # SPDX-License-Identifier: MIT
-__version__ = "1.2.0"
+__version__ = "1.3.0"
```

## matter_observability/config.py

```diff
@@ -1,8 +1,8 @@
 import os
 
 
 class Config:
     ENABLE_METRICS = os.getenv("ENABLE_METRICS", "true").lower() == "true"
-    SERVER_LOG_LEVEL = os.environ.get("SERVER_LOG_LEVEL", "info")
-    PROMETHEUS_PUSH_GATEWAY_HOST = os.environ["PROMETHEUS_PUSH_GATEWAY_HOST"]
+    SERVER_LOG_LEVEL = os.getenv("SERVER_LOG_LEVEL", "info")
+    PROMETHEUS_PUSH_GATEWAY_HOST = os.getenv("PROMETHEUS_PUSH_GATEWAY_HOST")
     INSTANCE_NAME = os.environ["INSTANCE_NAME"]
```

## matter_observability/fastapi/__init__.py

```diff
@@ -1,3 +1,5 @@
-__all__ = []
+__all__ = ["configure_middleware", "add_middleware"]
 
-from .utils import add_middleware
+from .utils import configure_middleware
+
+add_middleware = configure_middleware
```

## matter_observability/fastapi/utils.py

```diff
@@ -1,16 +1,23 @@
 from starlette_exporter import PrometheusMiddleware, handle_metrics
 
 from matter_observability.config import Config
+from matter_observability.exceptions import MisConfigurationError
+from .request_id import process_request_id
 
 
-def add_middleware(app, skip_paths=None):
+def configure_middleware(app, skip_paths=None):
     metrics_path = "/internal/metrics"
 
+    app.middleware("http")(process_request_id)
+
     if Config.ENABLE_METRICS:
+        if bool(Config.INSTANCE_NAME) is False:
+            raise MisConfigurationError("Environment variable: INSTANCE_NAME is not valid")
+
         app.add_middleware(
             PrometheusMiddleware,
             app_name=Config.INSTANCE_NAME,
             group_paths=True,
             skip_paths=[metrics_path] + skip_paths if skip_paths else [metrics_path],
         )
         app.add_route(metrics_path, handle_metrics)
```

## matter_observability/logging/__init__.py

```diff
@@ -1,3 +1,3 @@
-__all__ = []
+__all__ = ["LOGGING_CONFIG"]
 
 from .logging_config import LOGGING_CONFIG
```

## matter_observability/logging/logging_config.py

```diff
@@ -1,10 +1,11 @@
-from matter_observability.config import Config
+from matter_observability.config import Config  # pragma: no cover
 
-LOGGING_CONFIG = {
+
+LOGGING_CONFIG = {  # pragma: no cover
     "version": 1,
     "filters": {"request_id": {"()": "matter_observability.fastapi.request_id.RequestIdLogFilter"}},
     "formatters": {
         "standard": {
             "format": "[%(asctime)s] [%(levelname)s] [%(name)s] [%(request_id)s] [%(filename)s:%(funcName)s:%(lineno)s] - %(message)s"
         },
         "no_request_id": {
```

## matter_observability/metrics/utils.py

```diff
@@ -1,21 +1,24 @@
 import logging
 from urllib.error import HTTPError
 
 from prometheus_client import push_to_gateway, CollectorRegistry
 
 from matter_observability.config import Config
-
+from matter_observability.exceptions import MisConfigurationError
 
 registry = CollectorRegistry()
 job_name = f"batch_{Config.INSTANCE_NAME}"
 
 
 def publish_metrics():
     if Config.ENABLE_METRICS:
+        if Config.PROMETHEUS_PUSH_GATEWAY_HOST is None:
+            raise MisConfigurationError("Environment variable: PROMETHEUS_PUSH_GATEWAY_HOST is not set")
+
         try:
             push_to_gateway(
                 f"{Config.PROMETHEUS_PUSH_GATEWAY_HOST}:9091",
                 job=job_name,
                 registry=registry,
                 timeout=1,  # The connection timeout
             )
```

## Comparing `matter_observability-1.2.0.dist-info/METADATA` & `matter_observability-1.3.0.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: matter-observability
-Version: 1.2.0
+Version: 1.3.0
 Summary: A template for Matter's observability library
 Project-URL: Documentation, https://github.com/Matter-Tech/matter-observability#readme
 Project-URL: Issues, https://github.com/Matter-Tech/matter-observability/issues
 Project-URL: Source, https://github.com/Matter-Tech/matter-observability
 Author-email: Tomer Sasson <tomer@thisismatter.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10
+Requires-Dist: matter-exceptions==1.0.*
 Requires-Dist: starlette-exporter==0.15.1
 Description-Content-Type: text/markdown
 
 # matter-observability
 
 **Table of Contents**
```

## Comparing `matter_observability-1.2.0.dist-info/licenses/LICENSE` & `matter_observability-1.3.0.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

## Comparing `matter_observability-1.2.0.dist-info/RECORD` & `matter_observability-1.3.0.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-matter_observability/__about__.py,sha256=bJZ4QuVO53FpCQDaei3XZ3hp7NNjLm1SJ-DBD3aFyc8,134
+matter_observability/__about__.py,sha256=sHZUTLmLexxwRvrDNZ89yyP2935yJ2Bgf90rThihHFA,134
 matter_observability/__init__.py,sha256=3w1lcMfVq_KzRTAJVSrwL5vGSnu2BzERE4WFHCGvzFY,112
-matter_observability/config.py,sha256=w9fA25xabB3dOrwr8UYQznylnM_TF4IjEzAbITttyso,293
-matter_observability/fastapi/__init__.py,sha256=2WOHIy0WkTRaHV9G7Uqs6ht8fDJzHCen4wQJ9MXqMs8,48
+matter_observability/config.py,sha256=fv7xrBqG99_Ptkw9ObF9ZSEC8zYJWhgbp2ScBR2BcCA,287
+matter_observability/exceptions.py,sha256=vc3AZT1ZsrkTgnkeoiOFsAgsSIlCkywHryUnm-APVQo,132
+matter_observability/fastapi/__init__.py,sha256=TBGRRAMg7Q2Ov_a6sUZuWIoH9ITxWF036CYLVn-K25g,133
 matter_observability/fastapi/request_id.py,sha256=frjbfIr6U3J6ElbA5ZDnNFiz7eKerCGStevHHZu78P0,641
-matter_observability/fastapi/utils.py,sha256=vBvWu7OHkhRkQrpzyPpRmKHMQvA8ftzBZEhUkFIh5X4,513
-matter_observability/logging/__init__.py,sha256=IWHkh6Oh3fA2SGVgF8hGdUchHrj7RhkrydA7SfiIDeQ,57
-matter_observability/logging/logging_config.py,sha256=RzNOnjK8r8yTsj4SARuWKUrpCOV2-xIYN--u8t_zTY4,1630
+matter_observability/fastapi/utils.py,sha256=7_42_uQDpMliYsSz-K5txWLJMUySmPKThdmS559moKw,817
+matter_observability/logging/__init__.py,sha256=Xz1akGf5QHmMHjF9PpQ6Ljx8V5VI28N1tjom11jEKnQ,73
+matter_observability/logging/logging_config.py,sha256=TMRD_8nqEzO9TGu7r8p8ID0C10xUJNWPLygBIEP5q-E,1671
 matter_observability/metrics/__init__.py,sha256=CRAS0OI8AddFdIZFa66JvVam2tTjbfw-CLLEFRiwxnU,316
 matter_observability/metrics/custom_metrics.py,sha256=4WufeO-g14BzVfj0PEOWhaSug52K9vMNM5ZIVxlzESk,761
 matter_observability/metrics/decorators.py,sha256=DU-3lQZLYjSv_pTf36W_kdAvSZsOBrS61aPN7o8ryeM,2428
 matter_observability/metrics/labeled_counter.py,sha256=9ziI7Xlu1ApKo-eQcEVCSyAId_xvqo8jm6y3yLGT9ak,473
 matter_observability/metrics/labeled_gauge.py,sha256=MYJRPuqsvrjdBmDIiBaxzA66CUjJVI1KOGvzRRhDas0,489
 matter_observability/metrics/labeled_gauge_duration.py,sha256=-Xaxskzx2NytzBnLtbm6tJWjfHiBuqlNZ1WcG7HW7wA,708
 matter_observability/metrics/labeled_metric.py,sha256=Qn4psWuJJTyALay8-wU0vK2Y0epp25JWPSoZ8BQK8hM,421
-matter_observability/metrics/utils.py,sha256=J_Q7wsWp0AghYid2xyRZiZ0uoDqgnlbi3Mo2kUoX5_Y,676
-matter_observability-1.2.0.dist-info/METADATA,sha256=lu_geZ8_CVugEpxH8jlOm-3O8UnBLzvbC8lo9AgrklY,5812
-matter_observability-1.2.0.dist-info/WHEEL,sha256=EI2JsGydwUL5GP9t6kzZv7G3HDPi7FuZDDf9In6amRM,87
-matter_observability-1.2.0.dist-info/licenses/LICENSE,sha256=bqRY4B_u4xSKzKFb3ML8l0nCWvMXyzEGwY2B2hteV8g,1068
-matter_observability-1.2.0.dist-info/RECORD,,
+matter_observability/metrics/utils.py,sha256=TTe2pIfrr8R9F9_YNex9Klr_akQ_Ej-FUHEsNWjDwg0,903
+matter_observability-1.3.0.dist-info/METADATA,sha256=LlpHxkXdfQdvC4JEBX6aHlQbPEAOZ74Ul5QeQ8VlsXU,5852
+matter_observability-1.3.0.dist-info/WHEEL,sha256=EI2JsGydwUL5GP9t6kzZv7G3HDPi7FuZDDf9In6amRM,87
+matter_observability-1.3.0.dist-info/licenses/LICENSE,sha256=bqRY4B_u4xSKzKFb3ML8l0nCWvMXyzEGwY2B2hteV8g,1068
+matter_observability-1.3.0.dist-info/RECORD,,
```

