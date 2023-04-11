# Comparing `tmp/kpops-1.0.1.tar.gz` & `tmp/kpops-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kpops-1.0.1.tar", max compression
+gzip compressed data, was "kpops-1.1.0.tar", max compression
```

## Comparing `kpops-1.0.1.tar` & `kpops-1.1.0.tar`

### file list

```diff
@@ -1,61 +1,62 @@
--rw-r--r--   0        0        0     1064 2023-03-23 11:01:07.358459 kpops-1.0.1/LICENSE
--rw-r--r--   0        0        0     2192 2023-03-23 11:01:07.358459 kpops-1.0.1/README.md
--rw-r--r--   0        0        0        0 2023-03-23 11:01:07.362459 kpops-1.0.1/kpops/__init__.py
--rw-r--r--   0        0        0        0 2023-03-23 11:01:07.362459 kpops-1.0.1/kpops/cli/__init__.py
--rw-r--r--   0        0        0      761 2023-03-23 11:01:07.362459 kpops-1.0.1/kpops/cli/custom_formatter.py
--rw-r--r--   0        0        0      122 2023-03-23 11:01:07.362459 kpops-1.0.1/kpops/cli/exception.py
--rw-r--r--   0        0        0    10337 2023-03-23 11:01:07.362459 kpops-1.0.1/kpops/cli/main.py
--rw-r--r--   0        0        0     4228 2023-03-23 11:01:07.362459 kpops-1.0.1/kpops/cli/pipeline_config.py
--rw-r--r--   0        0        0     1711 2023-03-23 11:01:07.362459 kpops-1.0.1/kpops/cli/registry.py
--rw-r--r--   0        0        0      688 2023-03-23 11:01:07.362459 kpops-1.0.1/kpops/component_handlers/__init__.py
--rw-r--r--   0        0        0        0 2023-03-23 11:01:07.362459 kpops-1.0.1/kpops/component_handlers/helm_wrapper/__init__.py
--rw-r--r--   0        0        0       52 2023-03-23 11:01:07.362459 kpops-1.0.1/kpops/component_handlers/helm_wrapper/exception.py
--rw-r--r--   0        0        0     9371 2023-03-23 11:01:07.362459 kpops-1.0.1/kpops/component_handlers/helm_wrapper/helm.py
--rw-r--r--   0        0        0     2161 2023-03-23 11:01:07.362459 kpops-1.0.1/kpops/component_handlers/helm_wrapper/helm_diff.py
--rw-r--r--   0        0        0     2913 2023-03-23 11:01:07.362459 kpops-1.0.1/kpops/component_handlers/helm_wrapper/model.py
--rw-r--r--   0        0        0      667 2023-03-23 11:01:07.362459 kpops-1.0.1/kpops/component_handlers/helm_wrapper/utils.py
--rw-r--r--   0        0        0        0 2023-03-23 11:01:07.362459 kpops-1.0.1/kpops/component_handlers/kafka_connect/__init__.py
--rw-r--r--   0        0        0     8202 2023-03-23 11:01:07.362459 kpops-1.0.1/kpops/component_handlers/kafka_connect/connect_wrapper.py
--rw-r--r--   0        0        0      182 2023-03-23 11:01:07.362459 kpops-1.0.1/kpops/component_handlers/kafka_connect/exception.py
--rw-r--r--   0        0        0     5890 2023-03-23 11:01:07.362459 kpops-1.0.1/kpops/component_handlers/kafka_connect/kafka_connect_handler.py
--rw-r--r--   0        0        0     1470 2023-03-23 11:01:07.362459 kpops-1.0.1/kpops/component_handlers/kafka_connect/model.py
--rw-r--r--   0        0        0      788 2023-03-23 11:01:07.362459 kpops-1.0.1/kpops/component_handlers/kafka_connect/timeout.py
--rw-r--r--   0        0        0        0 2023-03-23 11:01:07.362459 kpops-1.0.1/kpops/component_handlers/schema_handler/__init__.py
--rw-r--r--   0        0        0     6035 2023-03-23 11:01:07.362459 kpops-1.0.1/kpops/component_handlers/schema_handler/schema_handler.py
--rw-r--r--   0        0        0      361 2023-03-23 11:01:07.362459 kpops-1.0.1/kpops/component_handlers/schema_handler/schema_provider.py
--rw-r--r--   0        0        0        0 2023-03-23 11:01:07.362459 kpops-1.0.1/kpops/component_handlers/topic/__init__.py
--rw-r--r--   0        0        0      180 2023-03-23 11:01:07.362459 kpops-1.0.1/kpops/component_handlers/topic/exception.py
--rw-r--r--   0        0        0     9588 2023-03-23 11:01:07.362459 kpops-1.0.1/kpops/component_handlers/topic/handler.py
--rw-r--r--   0        0        0     2503 2023-03-23 11:01:07.362459 kpops-1.0.1/kpops/component_handlers/topic/model.py
--rw-r--r--   0        0        0     6937 2023-03-23 11:01:07.362459 kpops-1.0.1/kpops/component_handlers/topic/proxy_wrapper.py
--rw-r--r--   0        0        0     2385 2023-03-23 11:01:07.362459 kpops-1.0.1/kpops/component_handlers/topic/utils.py
--rw-r--r--   0        0        0        0 2023-03-23 11:01:07.362459 kpops-1.0.1/kpops/component_handlers/utils/__init__.py
--rw-r--r--   0        0        0      630 2023-03-23 11:01:07.362459 kpops-1.0.1/kpops/component_handlers/utils/exception.py
--rw-r--r--   0        0        0      346 2023-03-23 11:01:07.362459 kpops-1.0.1/kpops/components/__init__.py
--rw-r--r--   0        0        0      466 2023-03-23 11:01:07.362459 kpops-1.0.1/kpops/components/base_components/__init__.py
--rw-r--r--   0        0        0     5528 2023-03-23 11:01:07.362459 kpops-1.0.1/kpops/components/base_components/base_defaults_component.py
--rw-r--r--   0        0        0     4552 2023-03-23 11:01:07.362459 kpops-1.0.1/kpops/components/base_components/kafka_app.py
--rw-r--r--   0        0        0    11549 2023-03-23 11:01:07.362459 kpops-1.0.1/kpops/components/base_components/kafka_connector.py
--rw-r--r--   0        0        0     4546 2023-03-23 11:01:07.362459 kpops-1.0.1/kpops/components/base_components/kubernetes_app.py
--rw-r--r--   0        0        0        0 2023-03-23 11:01:07.362459 kpops-1.0.1/kpops/components/base_components/models/__init__.py
--rw-r--r--   0        0        0     1169 2023-03-23 11:01:07.362459 kpops-1.0.1/kpops/components/base_components/models/from_section.py
--rw-r--r--   0        0        0     1754 2023-03-23 11:01:07.362459 kpops-1.0.1/kpops/components/base_components/models/to_section.py
--rw-r--r--   0        0        0     7097 2023-03-23 11:01:07.362459 kpops-1.0.1/kpops/components/base_components/pipeline_component.py
--rw-r--r--   0        0        0      211 2023-03-23 11:01:07.362459 kpops-1.0.1/kpops/components/streams_bootstrap/__init__.py
--rw-r--r--   0        0        0      217 2023-03-23 11:01:07.362459 kpops-1.0.1/kpops/components/streams_bootstrap/app_type.py
--rw-r--r--   0        0        0        0 2023-03-23 11:01:07.362459 kpops-1.0.1/kpops/components/streams_bootstrap/producer/__init__.py
--rw-r--r--   0        0        0      402 2023-03-23 11:01:07.362459 kpops-1.0.1/kpops/components/streams_bootstrap/producer/model.py
--rw-r--r--   0        0        0     2244 2023-03-23 11:01:07.362459 kpops-1.0.1/kpops/components/streams_bootstrap/producer/producer_app.py
--rw-r--r--   0        0        0        0 2023-03-23 11:01:07.362459 kpops-1.0.1/kpops/components/streams_bootstrap/streams/__init__.py
--rw-r--r--   0        0        0     4575 2023-03-23 11:01:07.362459 kpops-1.0.1/kpops/components/streams_bootstrap/streams/model.py
--rw-r--r--   0        0        0     3072 2023-03-23 11:01:07.362459 kpops-1.0.1/kpops/components/streams_bootstrap/streams/streams_app.py
--rw-r--r--   0        0        0        0 2023-03-23 11:01:07.362459 kpops-1.0.1/kpops/pipeline_generator/__init__.py
--rw-r--r--   0        0        0     9545 2023-03-23 11:01:07.362459 kpops-1.0.1/kpops/pipeline_generator/pipeline.py
--rw-r--r--   0        0        0        0 2023-03-23 11:01:07.362459 kpops-1.0.1/kpops/utils/__init__.py
--rw-r--r--   0        0        0      289 2023-03-23 11:01:07.362459 kpops-1.0.1/kpops/utils/colorify.py
--rw-r--r--   0        0        0     3043 2023-03-23 11:01:07.362459 kpops-1.0.1/kpops/utils/dict_differ.py
--rw-r--r--   0        0        0      291 2023-03-23 11:01:07.362459 kpops-1.0.1/kpops/utils/pydantic.py
--rw-r--r--   0        0        0     1107 2023-03-23 11:01:07.362459 kpops-1.0.1/kpops/utils/yaml_loading.py
--rw-r--r--   0        0        0     1840 2023-03-23 11:01:24.114837 kpops-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     3768 1970-01-01 00:00:00.000000 kpops-1.0.1/setup.py
--rw-r--r--   0        0        0     3787 1970-01-01 00:00:00.000000 kpops-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-04-11 16:18:00.214327 kpops-1.1.0/LICENSE
+-rw-r--r--   0        0        0     2370 2023-04-11 16:18:00.214327 kpops-1.1.0/README.md
+-rw-r--r--   0        0        0        0 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/cli/__init__.py
+-rw-r--r--   0        0        0      761 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/cli/custom_formatter.py
+-rw-r--r--   0        0        0      122 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/cli/exception.py
+-rw-r--r--   0        0        0    11186 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/cli/main.py
+-rw-r--r--   0        0        0     4226 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/cli/pipeline_config.py
+-rw-r--r--   0        0        0     1711 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/cli/registry.py
+-rw-r--r--   0        0        0      688 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/component_handlers/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/component_handlers/helm_wrapper/__init__.py
+-rw-r--r--   0        0        0       52 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/component_handlers/helm_wrapper/exception.py
+-rw-r--r--   0        0        0     9371 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/component_handlers/helm_wrapper/helm.py
+-rw-r--r--   0        0        0     2161 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/component_handlers/helm_wrapper/helm_diff.py
+-rw-r--r--   0        0        0     2913 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/component_handlers/helm_wrapper/model.py
+-rw-r--r--   0        0        0      667 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/component_handlers/helm_wrapper/utils.py
+-rw-r--r--   0        0        0        0 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/component_handlers/kafka_connect/__init__.py
+-rw-r--r--   0        0        0     8202 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/component_handlers/kafka_connect/connect_wrapper.py
+-rw-r--r--   0        0        0      182 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/component_handlers/kafka_connect/exception.py
+-rw-r--r--   0        0        0     5890 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/component_handlers/kafka_connect/kafka_connect_handler.py
+-rw-r--r--   0        0        0     1470 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/component_handlers/kafka_connect/model.py
+-rw-r--r--   0        0        0      788 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/component_handlers/kafka_connect/timeout.py
+-rw-r--r--   0        0        0        0 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/component_handlers/schema_handler/__init__.py
+-rw-r--r--   0        0        0     6035 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/component_handlers/schema_handler/schema_handler.py
+-rw-r--r--   0        0        0      361 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/component_handlers/schema_handler/schema_provider.py
+-rw-r--r--   0        0        0        0 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/component_handlers/topic/__init__.py
+-rw-r--r--   0        0        0      180 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/component_handlers/topic/exception.py
+-rw-r--r--   0        0        0     9588 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/component_handlers/topic/handler.py
+-rw-r--r--   0        0        0     2503 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/component_handlers/topic/model.py
+-rw-r--r--   0        0        0     6937 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/component_handlers/topic/proxy_wrapper.py
+-rw-r--r--   0        0        0     2385 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/component_handlers/topic/utils.py
+-rw-r--r--   0        0        0        0 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/component_handlers/utils/__init__.py
+-rw-r--r--   0        0        0      630 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/component_handlers/utils/exception.py
+-rw-r--r--   0        0        0      444 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/components/__init__.py
+-rw-r--r--   0        0        0      466 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/components/base_components/__init__.py
+-rw-r--r--   0        0        0     5528 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/components/base_components/base_defaults_component.py
+-rw-r--r--   0        0        0     4552 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/components/base_components/kafka_app.py
+-rw-r--r--   0        0        0    11549 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/components/base_components/kafka_connector.py
+-rw-r--r--   0        0        0     4546 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/components/base_components/kubernetes_app.py
+-rw-r--r--   0        0        0        0 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/components/base_components/models/__init__.py
+-rw-r--r--   0        0        0     1553 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/components/base_components/models/from_section.py
+-rw-r--r--   0        0        0     1754 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/components/base_components/models/to_section.py
+-rw-r--r--   0        0        0     7196 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/components/base_components/pipeline_component.py
+-rw-r--r--   0        0        0      211 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/components/streams_bootstrap/__init__.py
+-rw-r--r--   0        0        0      217 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/components/streams_bootstrap/app_type.py
+-rw-r--r--   0        0        0        0 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/components/streams_bootstrap/producer/__init__.py
+-rw-r--r--   0        0        0      402 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/components/streams_bootstrap/producer/model.py
+-rw-r--r--   0        0        0     2244 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/components/streams_bootstrap/producer/producer_app.py
+-rw-r--r--   0        0        0        0 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/components/streams_bootstrap/streams/__init__.py
+-rw-r--r--   0        0        0     4575 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/components/streams_bootstrap/streams/model.py
+-rw-r--r--   0        0        0     3072 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/components/streams_bootstrap/streams/streams_app.py
+-rw-r--r--   0        0        0        0 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/pipeline_generator/__init__.py
+-rw-r--r--   0        0        0    10755 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/pipeline_generator/pipeline.py
+-rw-r--r--   0        0        0        0 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/utils/__init__.py
+-rw-r--r--   0        0        0      289 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/utils/colorify.py
+-rw-r--r--   0        0        0     3043 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/utils/dict_differ.py
+-rw-r--r--   0        0        0     4407 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/utils/gen_schema.py
+-rw-r--r--   0        0        0      291 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/utils/pydantic.py
+-rw-r--r--   0        0        0     1107 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/utils/yaml_loading.py
+-rw-r--r--   0        0        0     1840 2023-04-11 16:18:16.890552 kpops-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3948 1970-01-01 00:00:00.000000 kpops-1.1.0/setup.py
+-rw-r--r--   0        0        0     3965 1970-01-01 00:00:00.000000 kpops-1.1.0/PKG-INFO
```

### Comparing `kpops-1.0.1/LICENSE` & `kpops-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kpops-1.0.1/README.md` & `kpops-1.1.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # KPOps
 
-[![Latest release](https://img.shields.io/github/v/release/bakdata/kpops)](https://github.com/bakdata/kpops/releases/latest)
 [![Build status](https://github.com/bakdata/kpops/actions/workflows/ci.yaml/badge.svg)](https://github.com/bakdata/kpops/actions/workflows/ci.yaml)
+[![pypi](https://img.shields.io/pypi/v/kpops.svg)](https://pypi.org/project/kpops)
+[![versions](https://img.shields.io/pypi/pyversions/kpops.svg)](https://github.com/bakdata/kpops)
+[![license](https://img.shields.io/github/license/bakdata/kpops.svg)](https://github.com/bakdata/kpops/blob/main/LICENSE)
 
 ## Key features
 
 - **Deploy Kafka apps to Kubernetes**: KPOps allows to deploy consecutive Kafka Streams applications and producers using an easy-to-read and -write pipeline definition.
 - **Manage Kafka Connectors**: KPOps connects with your Kafka Connect cluster and deploys, validates, and deletes your connectors.
 - **Configure multiple pipelines and steps**: KPOps has various abstractions that simplify configuring multiple pipelines and steps within pipelines by sharing common configuration between different components, such as producers or streaming applications.
 - **Handle your topics and schemas**: KPOps not only creates and deletes your topics but also registers and deletes your schemas.
```

### Comparing `kpops-1.0.1/kpops/cli/custom_formatter.py` & `kpops-1.1.0/kpops/cli/custom_formatter.py`

 * *Files identical despite different names*

### Comparing `kpops-1.0.1/kpops/cli/main.py` & `kpops-1.1.0/kpops/cli/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,19 +13,19 @@
 from kpops.component_handlers.kafka_connect.kafka_connect_handler import (
     KafkaConnectHandler,
 )
 from kpops.component_handlers.schema_handler.schema_handler import SchemaHandler
 from kpops.component_handlers.topic.handler import TopicHandler
 from kpops.component_handlers.topic.proxy_wrapper import ProxyWrapper
 from kpops.pipeline_generator.pipeline import Pipeline
+from kpops.utils.gen_schema import SchemaScope, gen_config_schema, gen_pipeline_schema
 
 if TYPE_CHECKING:
     from kpops.components.base_components import PipelineComponent
 
-
 LOG_DIVIDER = "#" * 100
 
 app = typer.Typer(
     pretty_exceptions_show_locals=False,
 )
 
 BASE_DIR_PATH_OPTION: Path = typer.Option(
@@ -184,14 +184,41 @@
     else:
         pipeline_config = PipelineConfig()
         pipeline_config.defaults_path = config.parent / pipeline_config.defaults_path
     return pipeline_config
 
 
 @app.command(
+    help="""
+    Generate json schema.
+
+    The schemas can be used to enable support for kpops files in a text editor.
+    """
+)
+def schema(
+    scope: SchemaScope = typer.Argument(
+        ...,
+        show_default=False,
+        help="""
+        Scope of the generated schema
+        \n\n\n
+        pipeline: Schema of PipelineComponents. Always includes the built-in kpops components. To include custom components, provide [COMPONENTS_MODULES].
+        \n\n\n
+        config: Schema of PipelineConfig.""",
+    ),
+    components_module: Optional[str] = COMPONENTS_MODULES,
+) -> None:
+    match scope:
+        case SchemaScope.PIPELINE:
+            gen_pipeline_schema(components_module)
+        case SchemaScope.CONFIG:
+            gen_config_schema()
+
+
+@app.command(
     help="Enriches pipelines steps with defaults. The output is used as input for the deploy/destroy/... commands."
 )
 def generate(
     pipeline_base_dir: Path = BASE_DIR_PATH_OPTION,
     pipeline_path: Path = PIPELINE_PATH_ARG,
     components_module: Optional[str] = COMPONENTS_MODULES,
     defaults: Optional[Path] = DEFAULT_PATH_OPTION,
@@ -216,16 +243,16 @@
     pipeline.print_yaml()
 
     if template:
         steps_to_apply = get_steps_to_apply(pipeline, steps)
         for component in steps_to_apply:
             component.template(api_version, ca_file, cert_file)
     elif cert_file or ca_file or api_version or steps:
-        raise TypeError(
-            "The following flags can only be used in conjuction with `--template`: \n \
+        log.warning(
+            "The following flags are considered only when `--template` is set: \n \
                 '--cert-file'\n \
                 '--ca-file'\n \
                 '--api-version'\n \
                 '--steps'"
         )
 
     return pipeline
```

### Comparing `kpops-1.0.1/kpops/cli/pipeline_config.py` & `kpops-1.1.0/kpops/cli/pipeline_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     """
     Pipeline configuration unrelated to the components.
     """
 
     defaults_path: Path = Field(
         default=Path("."),
         example="defaults",
-        description="The path to the folder containing the defaults.yaml file and the environment defaults files. \n"
+        description="The path to the folder containing the defaults.yaml file and the environment defaults files. "
         "Paths can either be absolute or relative to `config.yaml`",
     )
     environment: str = Field(
         default=...,
         env=f"{ENV_PREFIX}ENVIRONMENT",
         example="development",
         description="The environment you want to generate and deploy the pipeline to. "
```

### Comparing `kpops-1.0.1/kpops/cli/registry.py` & `kpops-1.1.0/kpops/cli/registry.py`

 * *Files identical despite different names*

### Comparing `kpops-1.0.1/kpops/component_handlers/__init__.py` & `kpops-1.1.0/kpops/component_handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `kpops-1.0.1/kpops/component_handlers/helm_wrapper/helm.py` & `kpops-1.1.0/kpops/component_handlers/helm_wrapper/helm.py`

 * *Files identical despite different names*

### Comparing `kpops-1.0.1/kpops/component_handlers/helm_wrapper/helm_diff.py` & `kpops-1.1.0/kpops/component_handlers/helm_wrapper/helm_diff.py`

 * *Files identical despite different names*

### Comparing `kpops-1.0.1/kpops/component_handlers/helm_wrapper/model.py` & `kpops-1.1.0/kpops/component_handlers/helm_wrapper/model.py`

 * *Files identical despite different names*

### Comparing `kpops-1.0.1/kpops/component_handlers/helm_wrapper/utils.py` & `kpops-1.1.0/kpops/component_handlers/helm_wrapper/utils.py`

 * *Files identical despite different names*

### Comparing `kpops-1.0.1/kpops/component_handlers/kafka_connect/connect_wrapper.py` & `kpops-1.1.0/kpops/component_handlers/kafka_connect/connect_wrapper.py`

 * *Files identical despite different names*

### Comparing `kpops-1.0.1/kpops/component_handlers/kafka_connect/kafka_connect_handler.py` & `kpops-1.1.0/kpops/component_handlers/kafka_connect/kafka_connect_handler.py`

 * *Files identical despite different names*

### Comparing `kpops-1.0.1/kpops/component_handlers/kafka_connect/model.py` & `kpops-1.1.0/kpops/component_handlers/kafka_connect/model.py`

 * *Files identical despite different names*

### Comparing `kpops-1.0.1/kpops/component_handlers/kafka_connect/timeout.py` & `kpops-1.1.0/kpops/component_handlers/kafka_connect/timeout.py`

 * *Files identical despite different names*

### Comparing `kpops-1.0.1/kpops/component_handlers/schema_handler/schema_handler.py` & `kpops-1.1.0/kpops/component_handlers/schema_handler/schema_handler.py`

 * *Files identical despite different names*

### Comparing `kpops-1.0.1/kpops/component_handlers/topic/handler.py` & `kpops-1.1.0/kpops/component_handlers/topic/handler.py`

 * *Files identical despite different names*

### Comparing `kpops-1.0.1/kpops/component_handlers/topic/model.py` & `kpops-1.1.0/kpops/component_handlers/topic/model.py`

 * *Files identical despite different names*

### Comparing `kpops-1.0.1/kpops/component_handlers/topic/proxy_wrapper.py` & `kpops-1.1.0/kpops/component_handlers/topic/proxy_wrapper.py`

 * *Files identical despite different names*

### Comparing `kpops-1.0.1/kpops/component_handlers/topic/utils.py` & `kpops-1.1.0/kpops/component_handlers/topic/utils.py`

 * *Files identical despite different names*

### Comparing `kpops-1.0.1/kpops/component_handlers/utils/exception.py` & `kpops-1.1.0/kpops/component_handlers/utils/exception.py`

 * *Files identical despite different names*

### Comparing `kpops-1.0.1/kpops/components/base_components/base_defaults_component.py` & `kpops-1.1.0/kpops/components/base_components/base_defaults_component.py`

 * *Files identical despite different names*

### Comparing `kpops-1.0.1/kpops/components/base_components/kafka_app.py` & `kpops-1.1.0/kpops/components/base_components/kafka_app.py`

 * *Files identical despite different names*

### Comparing `kpops-1.0.1/kpops/components/base_components/kafka_connector.py` & `kpops-1.1.0/kpops/components/base_components/kafka_connector.py`

 * *Files identical despite different names*

### Comparing `kpops-1.0.1/kpops/components/base_components/kubernetes_app.py` & `kpops-1.1.0/kpops/components/base_components/kubernetes_app.py`

 * *Files identical despite different names*

### Comparing `kpops-1.0.1/kpops/components/base_components/models/from_section.py` & `kpops-1.1.0/kpops/components/base_components/models/from_section.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from enum import Enum
+from typing import NewType
 
 from pydantic import BaseConfig, BaseModel, Extra, Field, root_validator
 
 
 class InputTopicTypes(str, Enum):
     INPUT = "input"
     EXTRA = "extra"
@@ -15,28 +16,39 @@
     role: str | None = None
 
     class Config(BaseConfig):
         extra = Extra.forbid
         use_enum_values = True
 
     @root_validator
-    def extra_topic_role(cls, values):
+    def extra_topic_role(cls, values: dict) -> dict:
         is_extra_topic = values["type"] in (
             InputTopicTypes.EXTRA,
             InputTopicTypes.EXTRA_PATTERN,
         )
         if is_extra_topic and not values.get("role"):
             raise ValueError(
-                "If you define an extra input topic or extra input pattern, you have to define a role."
+                "If you define an extra input component, extra input topic, or extra input pattern, you have to define a role."
             )
         if not is_extra_topic and values.get("role"):
             raise ValueError(
-                "If you do not define an input topic or input pattern, the role is unnecessary."
+                "If you do not define an input component, input topic, or input pattern, the role is unnecessary."
             )
         return values
 
 
+TopicName = NewType("TopicName", str)
+ComponentName = NewType("ComponentName", str)
+
+
 class FromSection(BaseModel):
-    topics: dict[str, FromTopic]
+    topics: dict[TopicName, FromTopic] = Field(
+        default={},
+        description="Topics to read from.",
+    )
+    components: dict[ComponentName, FromTopic] = Field(
+        default={},
+        description="Components to read from.",
+    )
 
     class Config(BaseConfig):
         extra = Extra.forbid
```

### Comparing `kpops-1.0.1/kpops/components/base_components/models/to_section.py` & `kpops-1.1.0/kpops/components/base_components/models/to_section.py`

 * *Files identical despite different names*

### Comparing `kpops-1.0.1/kpops/components/base_components/pipeline_component.py` & `kpops-1.1.0/kpops/components/base_components/pipeline_component.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,15 +110,15 @@
         Supports extra_input_topics (topics by role) or input_topics.
         """
         if self.from_:
             for name, topic in self.from_.topics.items():
                 self.apply_from_inputs(name, topic)
 
     def apply_from_inputs(self, name: str, topic: FromTopic) -> None:
-        match (topic.type):
+        match topic.type:
             case InputTopicTypes.INPUT:
                 self.add_input_topics([name])
             case InputTopicTypes.EXTRA if topic.role:
                 self.add_extra_input_topic(topic.role, [name])
             case InputTopicTypes.INPUT_PATTERN:
                 self.set_input_pattern(name)
             case InputTopicTypes.EXTRA_PATTERN if topic.role:
@@ -126,38 +126,42 @@
 
     def set_output_topics(self) -> None:
         if self.to:
             for name, topic in self.to.topics.items():
                 self.apply_to_outputs(name, topic)
 
     def apply_to_outputs(self, name: str, topic: TopicConfig) -> None:
-        match (topic.type):
+        match topic.type:
             case OutputTopicTypes.OUTPUT:
                 self.set_output_topic(name)
             case OutputTopicTypes.ERROR:
                 self.set_error_topic(name)
             case OutputTopicTypes.EXTRA if topic.role:
                 self.add_extra_output_topic(name, topic.role)
 
-    def weave_from_topics(self, prev_component_to: ToSection) -> None:
+    def weave_from_topics(
+        self,
+        to: ToSection | None,
+        from_topic: FromTopic = FromTopic(type=InputTopicTypes.INPUT),
+    ) -> None:
         """
         Weave output topics of upstream component or from component into config
         Override this method if you want to apply custom logic
         """
-        if self.from_:
+        if not to:
             return
         input_topics = [
             topic_name
-            for topic_name, topic_config in prev_component_to.topics.items()
+            for topic_name, topic_config in to.topics.items()
             if topic_config.type == OutputTopicTypes.OUTPUT
         ]
-        if input_topics:
-            self.add_input_topics(input_topics)
+        for input_topic in input_topics:
+            self.apply_from_inputs(input_topic, from_topic)
 
-    def substitute_name(self):
+    def substitute_name(self) -> None:
         if self.name:
             self.name = self.substitute_component_names(self.name, self.type)
         else:
             raise ValueError("Every component must have a name in the end.")
 
     def inflate(self) -> list[PipelineComponent]:
         """Inflate a component. This is helpful if one component should result in multiple components.
```

### Comparing `kpops-1.0.1/kpops/components/streams_bootstrap/producer/producer_app.py` & `kpops-1.1.0/kpops/components/streams_bootstrap/producer/producer_app.py`

 * *Files identical despite different names*

### Comparing `kpops-1.0.1/kpops/components/streams_bootstrap/streams/model.py` & `kpops-1.1.0/kpops/components/streams_bootstrap/streams/model.py`

 * *Files identical despite different names*

### Comparing `kpops-1.0.1/kpops/components/streams_bootstrap/streams/streams_app.py` & `kpops-1.1.0/kpops/components/streams_bootstrap/streams/streams_app.py`

 * *Files identical despite different names*

### Comparing `kpops-1.0.1/kpops/pipeline_generator/pipeline.py` & `kpops-1.1.0/kpops/pipeline_generator/pipeline.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,15 +23,44 @@
 
 
 class ParsingException(Exception):
     pass
 
 
 class PipelineComponents(BaseModel):
-    components: list[PipelineComponent]
+    components: list[PipelineComponent] = []
+
+    @property
+    def last(self) -> PipelineComponent:
+        return self.components[-1]
+
+    def find(self, component_name: str) -> PipelineComponent:
+        for component in self.components:
+            if component_name == component.name.removeprefix(component.prefix):
+                return component
+        raise ValueError(f"Component {component_name} not found")
+
+    def add(self, component: PipelineComponent) -> None:
+        self._populate_component_name(component)
+        self.components.append(component)
+
+    def __bool__(self) -> bool:
+        return bool(self.components)
+
+    def __iter__(self) -> Iterator[PipelineComponent]:  # type: ignore[override]
+        return iter(self.components)
+
+    @staticmethod
+    def _populate_component_name(component: PipelineComponent) -> None:
+        component.name = component.prefix + component.name
+        with suppress(
+            AttributeError  # Some components like Kafka Connect do not have a name_override attribute
+        ):
+            if component.app and getattr(component.app, "name_override") is None:
+                setattr(component.app, "name_override", component.name)
 
 
 def create_env_components_index(
     environment_components: list[dict],
 ) -> dict[str, dict]:
     """
     Create an index for all registered components in the project
@@ -57,53 +86,22 @@
     def __init__(
         self,
         component_list: list[dict],
         environment_components: list[dict],
         registry: Registry,
         config: PipelineConfig,
         handlers: ComponentHandlers,
-    ):
-        self.components: list[PipelineComponent] = []
+    ) -> None:
+        self.components: PipelineComponents = PipelineComponents()
         self.handlers = handlers
         self.config = config
         self.registry = registry
         self.env_components_index = create_env_components_index(environment_components)
         self.parse_components(component_list)
 
-    @staticmethod
-    def pipeline_filename_environment(path: Path, config: PipelineConfig) -> Path:
-        """
-        Adds the environment name from the PipelineConfig to the pipeline.yaml path
-        :param path: Path to pipeline.yaml file
-        :param config: The PipelineConfig
-        :return: Absolute path to the pipeline_<environment>.yaml
-        """
-        return path.with_stem(f"{path.stem}_{config.environment}")
-
-    @staticmethod
-    def set_pipeline_name_env_vars(base_dir: Path, path: Path) -> None:
-        """
-        Sets the environment variable pipeline_name relative to the given base_dir.
-        Moreover, for each sub-path an environment variable is set.
-        For example, for a given path ./data/v1/dev/pipeline.yaml the pipeline_name would be
-        set to data-v1-dev. Then the sub environment variables are set:
-        pipeline_name_0 = data
-        pipeline_name_1 = v1
-        pipeline_name_2 = dev
-        :param base_dir: Base directory to the pipeline files
-        :param path: Path to pipeline.yaml file
-        """
-        path_without_file = path.resolve().relative_to(base_dir.resolve()).parts[:-1]
-        if not path_without_file:
-            raise ValueError("The pipeline-base-dir should not equal the pipeline-path")
-        pipeline_name = "-".join(path_without_file)
-        os.environ["pipeline_name"] = pipeline_name
-        for level, parent in enumerate(path_without_file):
-            os.environ[f"pipeline_name_{level}"] = parent
-
     @classmethod
     def load_from_yaml(
         cls,
         base_dir: Path,
         path: Path,
         registry: Registry,
         config: PipelineConfig,
@@ -125,78 +123,76 @@
                     f"The pipeline definition {env_file} should contain a list of components"
                 )
 
         pipeline = cls(main_content, env_content, registry, config, handlers)
         return pipeline
 
     def parse_components(self, component_list: list[dict]) -> None:
-        previous_component: PipelineComponent | None = None
         for component_data in component_list:
             try:
                 try:
                     component_type: str = component_data["type"]
                 except KeyError:
                     raise ValueError(
                         "Every component must have a type defined, this component does not have one."
                     )
                 component_class = self.registry[component_type]
-                inflated_components = self.apply_component(
-                    component_data,
-                    component_class,
-                    previous_component,
-                )
-                self.populate_pipeline_component_names(inflated_components)
-                self.components.extend(inflated_components)
-                previous_component = inflated_components.pop()
+                self.apply_component(component_class, component_data)
             except Exception as ex:
                 if "name" in component_data:
                     raise ParsingException(
                         f"Error enriching {component_data['type']} component {component_data['name']}"
                     ) from ex
                 else:
                     raise ParsingException() from ex
 
-    def populate_pipeline_component_names(
-        self, inflated_components: list[PipelineComponent]
+    def apply_component(
+        self, component_class: type[PipelineComponent], component_data: dict
     ) -> None:
-        for component in inflated_components:
-            component.name = component.prefix + component.name
-            with suppress(
-                AttributeError  # Some components like Kafka Connect do not have a name_override attribute
-            ):
-                if component.app and getattr(component.app, "name_override") is None:
-                    setattr(component.app, "name_override", component.name)
+        """Instantiates, enriches and inflates pipeline component.
+        Applies input topics according to FromSection.
 
-    def apply_component(
-        self,
-        component_data: dict,
-        component_class: type[PipelineComponent],
-        previous_component: PipelineComponent | None,
-    ) -> list[PipelineComponent]:
+        :param component_class: Type of pipeline component
+        :param component_data: Arguments for instantiation of pipeline component
+        """
         component = component_class(
             config=self.config,
             handlers=self.handlers,
             **component_data,
         )
         component = self.enrich_component(component)
-        # weave from topics
-        if previous_component and previous_component.to:
-            component.weave_from_topics(previous_component.to)
 
         # inflate & enrich components
-        enriched_components: list[PipelineComponent] = []
-        for inflated_component in component.inflate():  # TODO: recursively:
+        for inflated_component in component.inflate():  # TODO: recursively
             enriched_component = self.enrich_component(inflated_component)
-            if enriched_components:
-                prev = enriched_components[-1]
-                if prev.to:
-                    enriched_component.weave_from_topics(prev.to)
-            enriched_components.append(enriched_component)
-
-        return enriched_components
+            if enriched_component.from_:
+                # read from specified components
+                for (
+                    original_from_component_name,
+                    from_topic,
+                ) in enriched_component.from_.components.items():
+                    original_from_component = self.components.find(
+                        original_from_component_name
+                    )
+                    inflated_from_component = original_from_component.inflate()[-1]
+                    if inflated_from_component is not original_from_component:
+                        resolved_from_component_name = inflated_from_component.name
+                    else:
+                        resolved_from_component_name = original_from_component_name
+                    resolved_from_component = self.components.find(
+                        resolved_from_component_name
+                    )
+                    enriched_component.weave_from_topics(
+                        resolved_from_component.to, from_topic
+                    )
+            elif self.components:
+                # read from previous component
+                prev_component = self.components.last
+                enriched_component.weave_from_topics(prev_component.to)
+            self.components.add(enriched_component)
 
     def enrich_component(
         self,
         component: PipelineComponent,
     ) -> PipelineComponent:
         env_component_definition = self.env_components_index.get(component.name, {})
         pair = update_nested_pair(
@@ -211,43 +207,72 @@
         return component_class(
             enrich=False,
             config=self.config,
             handlers=self.handlers,
             **component_data,
         )
 
+    def print_yaml(self, substitution: dict | None = None) -> None:
+        syntax = Syntax(
+            substitute(str(self), substitution), "yaml", background_color="default"
+        )
+        Console(
+            width=1000  # HACK: overwrite console width to avoid truncating output
+        ).print(syntax)
+
+    def __iter__(self) -> Iterator[PipelineComponent]:
+        return iter(self.components)
+
+    def __str__(self) -> str:
+        return yaml.dump(
+            json.loads(  # HACK: serialize types on Pydantic model export, which are not serialized by .dict(); e.g. pathlib.Path
+                self.components.json(exclude_none=True, by_alias=True)
+            )
+        )
+
     @staticmethod
     def substitute_component_specific_variables(
         component: PipelineComponent, pair: dict  # TODO: better parameter name for pair
     ) -> dict:
-        # Override component config with component config in pipeline environment definition
+        """Overrides component config with component config in pipeline environment definition."""
         # HACK: why do we need an intermediate JSON object?
         component_data: dict = json.loads(
             substitute(
                 json.dumps(pair),
                 {
                     "component_type": component.type,
                     "component_name": component.name,
                 },
             )
         )
         return component_data
 
-    def __str__(self) -> str:
-        return yaml.dump(
-            json.loads(  # HACK: serialize types on Pydantic model export, which are not serialized by .dict(); e.g. pathlib.Path
-                PipelineComponents(components=self.components).json(
-                    exclude_none=True, by_alias=True
-                )
-            )
-        )
-
-    def print_yaml(self, substitution: dict | None = None) -> None:
-        syntax = Syntax(
-            substitute(str(self), substitution), "yaml", background_color="default"
-        )
-        Console(
-            width=1000  # HACK: overwrite console width to avoid truncating output
-        ).print(syntax)
+    @staticmethod
+    def pipeline_filename_environment(path: Path, config: PipelineConfig) -> Path:
+        """
+        Adds the environment name from the PipelineConfig to the pipeline.yaml path
+        :param path: Path to pipeline.yaml file
+        :param config: The PipelineConfig
+        :return: Absolute path to the pipeline_<environment>.yaml
+        """
+        return path.with_stem(f"{path.stem}_{config.environment}")
 
-    def __iter__(self) -> Iterator[PipelineComponent]:
-        return iter(self.components)
+    @staticmethod
+    def set_pipeline_name_env_vars(base_dir: Path, path: Path) -> None:
+        """
+        Sets the environment variable pipeline_name relative to the given base_dir.
+        Moreover, for each sub-path an environment variable is set.
+        For example, for a given path ./data/v1/dev/pipeline.yaml the pipeline_name would be
+        set to data-v1-dev. Then the sub environment variables are set:
+        pipeline_name_0 = data
+        pipeline_name_1 = v1
+        pipeline_name_2 = dev
+        :param base_dir: Base directory to the pipeline files
+        :param path: Path to pipeline.yaml file
+        """
+        path_without_file = path.resolve().relative_to(base_dir.resolve()).parts[:-1]
+        if not path_without_file:
+            raise ValueError("The pipeline-base-dir should not equal the pipeline-path")
+        pipeline_name = "-".join(path_without_file)
+        os.environ["pipeline_name"] = pipeline_name
+        for level, parent in enumerate(path_without_file):
+            os.environ[f"pipeline_name_{level}"] = parent
```

### Comparing `kpops-1.0.1/kpops/utils/dict_differ.py` & `kpops-1.1.0/kpops/utils/dict_differ.py`

 * *Files identical despite different names*

### Comparing `kpops-1.0.1/kpops/utils/yaml_loading.py` & `kpops-1.1.0/kpops/utils/yaml_loading.py`

 * *Files identical despite different names*

### Comparing `kpops-1.0.1/pyproject.toml` & `kpops-1.1.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kpops"
-version = "1.0.1"
+version = "1.1.0"
 description = "KPOps is a tool to deploy Kafka pipelines to Kubernetes"
 authors = ["bakdata <opensource@bakdata.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/bakdata/kpops"
 documentation = "https://bakdata.github.io/kpops/latest"
 keywords = ["kafka", "kubernetes", "stream-processing", "pipelines"]
```

### Comparing `kpops-1.0.1/setup.py` & `kpops-1.1.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -34,17 +34,17 @@
  'typer[all]>=0.6.1,<0.7.0']
 
 entry_points = \
 {'console_scripts': ['kpops = kpops.cli.main:app']}
 
 setup_kwargs = {
     'name': 'kpops',
-    'version': '1.0.1',
+    'version': '1.1.0',
     'description': 'KPOps is a tool to deploy Kafka pipelines to Kubernetes',
-    'long_description': '# KPOps\n\n[![Latest release](https://img.shields.io/github/v/release/bakdata/kpops)](https://github.com/bakdata/kpops/releases/latest)\n[![Build status](https://github.com/bakdata/kpops/actions/workflows/ci.yaml/badge.svg)](https://github.com/bakdata/kpops/actions/workflows/ci.yaml)\n\n## Key features\n\n- **Deploy Kafka apps to Kubernetes**: KPOps allows to deploy consecutive Kafka Streams applications and producers using an easy-to-read and -write pipeline definition.\n- **Manage Kafka Connectors**: KPOps connects with your Kafka Connect cluster and deploys, validates, and deletes your connectors.\n- **Configure multiple pipelines and steps**: KPOps has various abstractions that simplify configuring multiple pipelines and steps within pipelines by sharing common configuration between different components, such as producers or streaming applications.\n- **Handle your topics and schemas**: KPOps not only creates and deletes your topics but also registers and deletes your schemas.\n- **Clean termination of Kafka components**: KPOps removes your pipeline components (i.e., Kafka Streams applications) from the Kubernetes cluster _and_ cleans up the component-related states (i.e., removing/resetting offset of Kafka consumer groups).\n- **Preview your pipeline changes**: With the KPOps dry-run, you can ensure your pipeline definition is set up correctly. This helps to minimize downtime and prevent potential errors or issues that could impact your production environment.\n\n## Documentation\n\nFor detailed usage and installation instructions, check out\nthe [documentation](https://bakdata.github.io/kpops/latest/user/what-is-kpops/).\n\n## Install KPOps\n\nKPOps comes as a [PyPI package](https://pypi.org/project/kpops/). \nYou can install it with [pip](https://github.com/pypa/pip):\n\n```shell\npip install kpops\n```\n\n## Contributing\n\nWe are happy if you want to contribute to this project.\nIf you find any bugs or have suggestions for improvements, please open an issue.\nWe are also happy to accept your PRs.\nJust open an issue beforehand and let us know what you want to do and why.\n\n## License\n\nKPOps is licensed under the [MIT License](https://github.com/bakdata/kpops/blob/main/LICENSE).\n',
+    'long_description': '# KPOps\n\n[![Build status](https://github.com/bakdata/kpops/actions/workflows/ci.yaml/badge.svg)](https://github.com/bakdata/kpops/actions/workflows/ci.yaml)\n[![pypi](https://img.shields.io/pypi/v/kpops.svg)](https://pypi.org/project/kpops)\n[![versions](https://img.shields.io/pypi/pyversions/kpops.svg)](https://github.com/bakdata/kpops)\n[![license](https://img.shields.io/github/license/bakdata/kpops.svg)](https://github.com/bakdata/kpops/blob/main/LICENSE)\n\n## Key features\n\n- **Deploy Kafka apps to Kubernetes**: KPOps allows to deploy consecutive Kafka Streams applications and producers using an easy-to-read and -write pipeline definition.\n- **Manage Kafka Connectors**: KPOps connects with your Kafka Connect cluster and deploys, validates, and deletes your connectors.\n- **Configure multiple pipelines and steps**: KPOps has various abstractions that simplify configuring multiple pipelines and steps within pipelines by sharing common configuration between different components, such as producers or streaming applications.\n- **Handle your topics and schemas**: KPOps not only creates and deletes your topics but also registers and deletes your schemas.\n- **Clean termination of Kafka components**: KPOps removes your pipeline components (i.e., Kafka Streams applications) from the Kubernetes cluster _and_ cleans up the component-related states (i.e., removing/resetting offset of Kafka consumer groups).\n- **Preview your pipeline changes**: With the KPOps dry-run, you can ensure your pipeline definition is set up correctly. This helps to minimize downtime and prevent potential errors or issues that could impact your production environment.\n\n## Documentation\n\nFor detailed usage and installation instructions, check out\nthe [documentation](https://bakdata.github.io/kpops/latest/user/what-is-kpops/).\n\n## Install KPOps\n\nKPOps comes as a [PyPI package](https://pypi.org/project/kpops/). \nYou can install it with [pip](https://github.com/pypa/pip):\n\n```shell\npip install kpops\n```\n\n## Contributing\n\nWe are happy if you want to contribute to this project.\nIf you find any bugs or have suggestions for improvements, please open an issue.\nWe are also happy to accept your PRs.\nJust open an issue beforehand and let us know what you want to do and why.\n\n## License\n\nKPOps is licensed under the [MIT License](https://github.com/bakdata/kpops/blob/main/LICENSE).\n',
     'author': 'bakdata',
     'author_email': 'opensource@bakdata.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/bakdata/kpops',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `kpops-1.0.1/PKG-INFO` & `kpops-1.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kpops
-Version: 1.0.1
+Version: 1.1.0
 Summary: KPOps is a tool to deploy Kafka pipelines to Kubernetes
 Home-page: https://github.com/bakdata/kpops
 License: MIT
 Keywords: kafka,kubernetes,stream-processing,pipelines
 Author: bakdata
 Author-email: opensource@bakdata.com
 Requires-Python: >=3.10,<4.0
@@ -34,16 +34,18 @@
 Requires-Dist: typer[all] (>=0.6.1,<0.7.0)
 Project-URL: Documentation, https://bakdata.github.io/kpops/latest
 Project-URL: Repository, https://github.com/bakdata/kpops
 Description-Content-Type: text/markdown
 
 # KPOps
 
-[![Latest release](https://img.shields.io/github/v/release/bakdata/kpops)](https://github.com/bakdata/kpops/releases/latest)
 [![Build status](https://github.com/bakdata/kpops/actions/workflows/ci.yaml/badge.svg)](https://github.com/bakdata/kpops/actions/workflows/ci.yaml)
+[![pypi](https://img.shields.io/pypi/v/kpops.svg)](https://pypi.org/project/kpops)
+[![versions](https://img.shields.io/pypi/pyversions/kpops.svg)](https://github.com/bakdata/kpops)
+[![license](https://img.shields.io/github/license/bakdata/kpops.svg)](https://github.com/bakdata/kpops/blob/main/LICENSE)
 
 ## Key features
 
 - **Deploy Kafka apps to Kubernetes**: KPOps allows to deploy consecutive Kafka Streams applications and producers using an easy-to-read and -write pipeline definition.
 - **Manage Kafka Connectors**: KPOps connects with your Kafka Connect cluster and deploys, validates, and deletes your connectors.
 - **Configure multiple pipelines and steps**: KPOps has various abstractions that simplify configuring multiple pipelines and steps within pipelines by sharing common configuration between different components, such as producers or streaming applications.
 - **Handle your topics and schemas**: KPOps not only creates and deletes your topics but also registers and deletes your schemas.
```

