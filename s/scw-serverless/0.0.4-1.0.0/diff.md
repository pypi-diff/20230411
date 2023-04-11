# Comparing `tmp/scw_serverless-0.0.4.tar.gz` & `tmp/scw_serverless-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scw_serverless-0.0.4.tar", max compression
+gzip compressed data, was "scw_serverless-1.0.0.tar", max compression
```

## Comparing `scw_serverless-0.0.4.tar` & `scw_serverless-1.0.0.tar`

### file list

```diff
@@ -1,41 +1,38 @@
--rw-r--r--   0        0        0      411 2023-02-27 15:47:03.268949 scw_serverless-0.0.4/CHANGELOG.md
--rw-r--r--   0        0        0     1065 2023-02-02 17:20:42.069490 scw_serverless-0.0.4/LICENSE
--rw-r--r--   0        0        0     2495 2023-02-02 17:20:42.069490 scw_serverless-0.0.4/README.md
--rw-r--r--   0        0        0     2593 2023-02-27 15:47:03.272949 scw_serverless-0.0.4/pyproject.toml
--rw-r--r--   0        0        0       54 2023-02-02 17:20:42.073490 scw_serverless-0.0.4/scw_serverless/__init__.py
--rw-r--r--   0        0        0     4851 2023-02-20 10:14:05.179073 scw_serverless-0.0.4/scw_serverless/app.py
--rw-r--r--   0        0        0     6429 2023-02-27 15:17:33.009496 scw_serverless-0.0.4/scw_serverless/cli.py
--rw-r--r--   0        0        0       31 2023-02-02 17:20:42.073490 scw_serverless-0.0.4/scw_serverless/config/__init__.py
--rw-r--r--   0        0        0     5070 2023-02-20 10:14:05.179073 scw_serverless-0.0.4/scw_serverless/config/function.py
--rw-r--r--   0        0        0      138 2023-02-02 17:20:42.073490 scw_serverless-0.0.4/scw_serverless/config/generators/__init__.py
--rw-r--r--   0        0        0      219 2023-02-02 17:20:42.073490 scw_serverless-0.0.4/scw_serverless/config/generators/generator.py
--rw-r--r--   0        0        0     4169 2023-02-02 17:20:42.073490 scw_serverless-0.0.4/scw_serverless/config/generators/serverless_framework.py
--rw-r--r--   0        0        0     7045 2023-02-02 17:20:42.073490 scw_serverless-0.0.4/scw_serverless/config/generators/terraform.py
--rw-r--r--   0        0        0      454 2023-02-02 17:20:42.073490 scw_serverless-0.0.4/scw_serverless/config/route.py
--rw-r--r--   0        0        0       14 2023-02-02 17:20:42.073490 scw_serverless-0.0.4/scw_serverless/config/templates/.gitignore
--rw-r--r--   0        0        0      414 2023-02-02 17:20:42.073490 scw_serverless-0.0.4/scw_serverless/config/templates/serverless.yml
--rw-r--r--   0        0        0      426 2023-02-02 17:20:42.073490 scw_serverless-0.0.4/scw_serverless/config/templates/terraform.tf.json
--rw-r--r--   0        0        0      327 2023-02-02 17:20:42.073490 scw_serverless-0.0.4/scw_serverless/config/utils.py
--rw-r--r--   0        0        0     3416 2023-02-02 17:20:42.073490 scw_serverless-0.0.4/scw_serverless/dependencies_manager.py
--rw-r--r--   0        0        0        0 2023-02-02 17:20:42.073490 scw_serverless-0.0.4/scw_serverless/deploy/__init__.py
--rw-r--r--   0        0        0      172 2023-02-02 17:20:42.073490 scw_serverless-0.0.4/scw_serverless/deploy/backends/__init__.py
--rw-r--r--   0        0        0    11072 2023-02-02 17:20:42.073490 scw_serverless-0.0.4/scw_serverless/deploy/backends/scaleway_api_backend.py
--rw-r--r--   0        0        0      524 2023-02-02 17:20:42.073490 scw_serverless-0.0.4/scw_serverless/deploy/backends/serverless_backend.py
--rw-r--r--   0        0        0     1700 2023-02-02 17:20:42.073490 scw_serverless-0.0.4/scw_serverless/deploy/backends/serverless_framework_backend.py
--rw-r--r--   0        0        0       70 2023-02-02 17:20:42.073490 scw_serverless-0.0.4/scw_serverless/deploy/gateway/__init__.py
--rw-r--r--   0        0        0     1548 2023-02-02 17:20:42.073490 scw_serverless-0.0.4/scw_serverless/deploy/gateway/client.py
--rw-r--r--   0        0        0     4130 2023-02-09 12:28:15.314178 scw_serverless-0.0.4/scw_serverless/deploy/gateway/manager.py
--rw-r--r--   0        0        0      937 2023-02-02 17:20:42.073490 scw_serverless-0.0.4/scw_serverless/deploy/gateway/models.py
--rw-r--r--   0        0        0     2262 2023-02-02 17:20:42.073490 scw_serverless-0.0.4/scw_serverless/logger.py
--rw-r--r--   0        0        0      137 2023-02-02 17:20:42.073490 scw_serverless-0.0.4/scw_serverless/triggers/__init__.py
--rw-r--r--   0        0        0     1405 2023-02-02 17:20:42.073490 scw_serverless-0.0.4/scw_serverless/triggers/cron.py
--rw-r--r--   0        0        0        0 2023-02-02 17:20:42.073490 scw_serverless-0.0.4/scw_serverless/utils/__init__.py
--rw-r--r--   0        0        0      239 2023-02-02 17:20:42.073490 scw_serverless-0.0.4/scw_serverless/utils/commands.py
--rw-r--r--   0        0        0      967 2023-02-02 17:20:42.073490 scw_serverless-0.0.4/scw_serverless/utils/config.py
--rw-r--r--   0        0        0     1713 2023-02-02 17:20:42.073490 scw_serverless-0.0.4/scw_serverless/utils/credentials.py
--rw-r--r--   0        0        0      590 2023-02-02 17:20:42.073490 scw_serverless-0.0.4/scw_serverless/utils/files.py
--rw-r--r--   0        0        0     1476 2023-02-27 15:17:33.009496 scw_serverless-0.0.4/scw_serverless/utils/loader.py
--rw-r--r--   0        0        0      761 2023-02-02 17:20:42.073490 scw_serverless-0.0.4/scw_serverless/utils/string.py
--rw-r--r--   0        0        0       18 2023-02-02 17:20:42.073490 scw_serverless-0.0.4/scw_serverless/version.py
--rw-r--r--   0        0        0     3896 1970-01-01 00:00:00.000000 scw_serverless-0.0.4/setup.py
--rw-r--r--   0        0        0     4009 1970-01-01 00:00:00.000000 scw_serverless-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      499 2023-04-11 10:45:16.790571 scw_serverless-1.0.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1065 2023-02-02 17:20:42.069490 scw_serverless-1.0.0/LICENSE
+-rw-r--r--   0        0        0     2495 2023-02-02 17:20:42.069490 scw_serverless-1.0.0/README.md
+-rw-r--r--   0        0        0     2975 2023-04-11 10:45:16.790571 scw_serverless-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0       54 2023-02-02 17:20:42.073490 scw_serverless-1.0.0/scw_serverless/__init__.py
+-rw-r--r--   0        0        0     4716 2023-04-04 08:42:26.463081 scw_serverless-1.0.0/scw_serverless/app.py
+-rw-r--r--   0        0        0     6100 2023-04-04 08:42:26.463081 scw_serverless-1.0.0/scw_serverless/cli.py
+-rw-r--r--   0        0        0       31 2023-02-02 17:20:42.073490 scw_serverless-1.0.0/scw_serverless/config/__init__.py
+-rw-r--r--   0        0        0     5104 2023-04-04 13:54:31.192478 scw_serverless-1.0.0/scw_serverless/config/function.py
+-rw-r--r--   0        0        0      138 2023-02-02 17:20:42.073490 scw_serverless-1.0.0/scw_serverless/config/generators/__init__.py
+-rw-r--r--   0        0        0      219 2023-02-02 17:20:42.073490 scw_serverless-1.0.0/scw_serverless/config/generators/generator.py
+-rw-r--r--   0        0        0     4169 2023-02-02 17:20:42.073490 scw_serverless-1.0.0/scw_serverless/config/generators/serverless_framework.py
+-rw-r--r--   0        0        0     7045 2023-02-02 17:20:42.073490 scw_serverless-1.0.0/scw_serverless/config/generators/terraform.py
+-rw-r--r--   0        0        0     1247 2023-04-04 08:42:26.463081 scw_serverless-1.0.0/scw_serverless/config/route.py
+-rw-r--r--   0        0        0       14 2023-02-02 17:20:42.073490 scw_serverless-1.0.0/scw_serverless/config/templates/.gitignore
+-rw-r--r--   0        0        0      414 2023-02-02 17:20:42.073490 scw_serverless-1.0.0/scw_serverless/config/templates/serverless.yml
+-rw-r--r--   0        0        0      426 2023-02-02 17:20:42.073490 scw_serverless-1.0.0/scw_serverless/config/templates/terraform.tf.json
+-rw-r--r--   0        0        0      327 2023-02-02 17:20:42.073490 scw_serverless-1.0.0/scw_serverless/config/utils.py
+-rw-r--r--   0        0        0     3532 2023-04-04 08:42:26.463081 scw_serverless-1.0.0/scw_serverless/dependencies_manager.py
+-rw-r--r--   0        0        0        0 2023-02-02 17:20:42.073490 scw_serverless-1.0.0/scw_serverless/deploy/__init__.py
+-rw-r--r--   0        0        0      172 2023-02-02 17:20:42.073490 scw_serverless-1.0.0/scw_serverless/deploy/backends/__init__.py
+-rw-r--r--   0        0        0    11072 2023-03-13 13:34:16.012571 scw_serverless-1.0.0/scw_serverless/deploy/backends/scaleway_api_backend.py
+-rw-r--r--   0        0        0      524 2023-02-02 17:20:42.073490 scw_serverless-1.0.0/scw_serverless/deploy/backends/serverless_backend.py
+-rw-r--r--   0        0        0     1700 2023-02-02 17:20:42.073490 scw_serverless-1.0.0/scw_serverless/deploy/backends/serverless_framework_backend.py
+-rw-r--r--   0        0        0        0 2023-04-04 08:42:26.463081 scw_serverless-1.0.0/scw_serverless/gateway/__init__.py
+-rw-r--r--   0        0        0     1359 2023-04-04 08:42:26.463081 scw_serverless-1.0.0/scw_serverless/gateway/gateway_api_client.py
+-rw-r--r--   0        0        0     2792 2023-04-04 15:50:23.232104 scw_serverless-1.0.0/scw_serverless/gateway/gateway_manager.py
+-rw-r--r--   0        0        0     2262 2023-02-02 17:20:42.073490 scw_serverless-1.0.0/scw_serverless/logger.py
+-rw-r--r--   0        0        0      137 2023-02-02 17:20:42.073490 scw_serverless-1.0.0/scw_serverless/triggers/__init__.py
+-rw-r--r--   0        0        0     1405 2023-02-02 17:20:42.073490 scw_serverless-1.0.0/scw_serverless/triggers/cron.py
+-rw-r--r--   0        0        0        0 2023-02-02 17:20:42.073490 scw_serverless-1.0.0/scw_serverless/utils/__init__.py
+-rw-r--r--   0        0        0      239 2023-02-02 17:20:42.073490 scw_serverless-1.0.0/scw_serverless/utils/commands.py
+-rw-r--r--   0        0        0     1864 2023-03-14 08:51:57.235841 scw_serverless-1.0.0/scw_serverless/utils/credentials.py
+-rw-r--r--   0        0        0      590 2023-02-02 17:20:42.073490 scw_serverless-1.0.0/scw_serverless/utils/files.py
+-rw-r--r--   0        0        0     1476 2023-02-27 15:17:33.009496 scw_serverless-1.0.0/scw_serverless/utils/loader.py
+-rw-r--r--   0        0        0      761 2023-02-02 17:20:42.073490 scw_serverless-1.0.0/scw_serverless/utils/string.py
+-rw-r--r--   0        0        0     3890 1970-01-01 00:00:00.000000 scw_serverless-1.0.0/setup.py
+-rw-r--r--   0        0        0     4010 1970-01-01 00:00:00.000000 scw_serverless-1.0.0/PKG-INFO
```

### Comparing `scw_serverless-0.0.4/LICENSE` & `scw_serverless-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scw_serverless-0.0.4/README.md` & `scw_serverless-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `scw_serverless-0.0.4/pyproject.toml` & `scw_serverless-1.0.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "scw-serverless"
-version = "0.0.4"
+version = "1.0.0"
 description = "Framework for writing serverless APIs in Python, using Scaleway functions and containers."
 authors = ["Scaleway Serverless Team <opensource@scaleway.com>"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/scaleway/serverless-api-project"
 documentation = "https://serverless-api-project.readthedocs.io/en/latest/"
 keywords = ["serverless", "scaleway", "functions", "cloud", "faas"]
@@ -35,42 +35,49 @@
 
 [tool.poetry.scripts]
 scw-serverless = "scw_serverless.cli:main"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 click = "^8.1.3"
-scaleway = ">=0.7,<0.9"
+scaleway = ">=0.7,<0.11"
 requests = "^2.28.2"
 typing-extensions = { version = "^4.4.0", python = "<3.11" }
 pyyaml = "^6.0"
 
 [tool.poetry.group.dev.dependencies]
-pre-commit = "^2.21.0"
+pre-commit = ">=2.21,<4.0"
 pytest = "^7.2.0"
 pytest-xdist = "^3.1.0"
 pylint = "^2.15.10"
 pylint-per-file-ignores = "^1.1.0"
-responses = "^0.22"
+responses = ">=0.22,<0.24"
+boto3 = "^1.26.97"
 
 [tool.poetry.group.doc]
 optional = true
 
 [tool.poetry.group.doc.dependencies]
-myst_parser = "^0.18.1"
+myst_parser = ">=0.18.1,<1.1.0"
 sphinx = "^5.3.0"
 sphinx_rtd_theme = "^1.1.1"
 
+[tool.pytest.ini_options]
+filterwarnings = [
+    "ignore:.*pkg_resources\\.declare_namespace.*:DeprecationWarning",
+    "ignore:::pkg_resources",
+]
+
 [tool.pylint]
 load-plugins = ["pylint_per_file_ignores"]
 disable = "missing-module-docstring"
 # Commented Black formatted code.
 max-line-length = 89
 # Short and common names. e is commonly used for exceptions.
-good-names = "i,fp,e"
+good-names = "e,fp,i,s,s3"
 # Classes with a single responsibility are fine.
 min-public-methods = 1
 
 [tool.pylint-per-file-ignores]
 "/tests/" = "missing-function-docstring,protected-access"
 # Sphinx specific
 "/docs/" = "invalid-name,redefined-builtin"
@@ -83,10 +90,15 @@
 exclude = ["**/node_modules", "**/__pycache__", "**/package/**"]
 
 [tool.pydocstyle]
 # Compatible with Sphinx
 convention = "google"
 add_ignore = ["D100", "D107"]
 
+[tool.bandit]
+# B603:subprocess_without_shell_equals_true is skipped because of the nature of the wrapper
+# B404:blacklist is skipped to import subprocess
+skips = ["B101", "B603", "B404"]
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `scw_serverless-0.0.4/scw_serverless/app.py` & `scw_serverless-1.0.0/scw_serverless/app.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,27 +15,24 @@
     """Manage your Serverless Functions.
 
     Maps to a function namespace. Parameters will be scoped to the namespace.
 
     :param service_name: name of the namespace
     :param env: namespace level environment variables
     :param secret: namespace level secrets
-    :param gateway_domains: domains to be supported by the gateway
     """
 
     def __init__(
         self,
         service_name: str,
         env: Optional[dict[str, Any]] = None,
         secret: Optional[dict[str, Any]] = None,
-        gateway_domains: Optional[list[str]] = None,
     ):
         self.functions: list[Function] = []
         self.service_name: str = service_name
-        self.gateway_domains: list[str] = gateway_domains if gateway_domains else []
         self.env = env
         self.secret = secret
 
     def func(
         self,
         **kwargs: Unpack[FunctionKwargs],
     ) -> Callable:
@@ -104,57 +101,57 @@
 
         :param url: relative url to trigger the function
 
         .. note::
 
             Requires an API gateway
         """
-        kwargs |= {"url": url, "methods": [HTTPMethod.GET]}
+        kwargs |= {"relative_url": url, "http_methods": [HTTPMethod.GET]}
         return self.func(**kwargs)
 
     def post(self, url: str, **kwargs: Unpack[FunctionKwargs]) -> Callable:
         """Define a routed handler which will respond to POST requests.
 
         :param url: relative url to trigger the function
 
         .. note::
 
             Requires an API gateway
         """
-        kwargs |= {"url": url, "methods": [HTTPMethod.POST]}
+        kwargs |= {"relative_url": url, "http_methods": [HTTPMethod.POST]}
         return self.func(**kwargs)
 
     def put(self, url: str, **kwargs: Unpack[FunctionKwargs]) -> Callable:
         """Define a routed handler which will respond to PUT requests.
 
         :param url: relative url to trigger the function
 
         .. note::
 
             Requires an API gateway
         """
-        kwargs |= {"url": url, "methods": [HTTPMethod.PUT]}
+        kwargs |= {"relative_url": url, "http_methods": [HTTPMethod.PUT]}
         return self.func(**kwargs)
 
     def delete(self, url: str, **kwargs: Unpack[FunctionKwargs]) -> Callable:
         """Define a routed handler which will respond to DELETE requests.
 
         :param url: relative url to trigger the function
 
         .. note::
 
             Requires an API gateway
         """
-        kwargs |= {"url": url, "methods": [HTTPMethod.DELETE]}
+        kwargs |= {"relative_url": url, "http_methods": [HTTPMethod.DELETE]}
         return self.func(**kwargs)
 
     def patch(self, url: str, **kwargs: Unpack[FunctionKwargs]) -> Callable:
         """Define a routed handler which will respond to PATCH requests.
 
         :param url: relative url to trigger the function
 
         .. note::
 
             Requires an API gateway
         """
-        kwargs |= {"url": url, "methods": [HTTPMethod.PATCH]}
+        kwargs |= {"relative_url": url, "http_methods": [HTTPMethod.PATCH]}
         return self.func(**kwargs)
```

### Comparing `scw_serverless-0.0.4/scw_serverless/cli.py` & `scw_serverless-1.0.0/scw_serverless/cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 import os
 from pathlib import Path
 from typing import Literal, Optional
 
 import click
 
-from scw_serverless.config.generators.serverless_framework import (
-    ServerlessFrameworkGenerator,
-)
-from scw_serverless.config.generators.terraform import TerraformGenerator
+from scw_serverless.config import generators
 from scw_serverless.dependencies_manager import DependenciesManager
-from scw_serverless.deploy import backends, gateway
+from scw_serverless.deploy import backends
+from scw_serverless.gateway.gateway_manager import GatewayManager
 from scw_serverless.logger import DEFAULT, get_logger
-from scw_serverless.utils.config import Config
 from scw_serverless.utils.credentials import DEFAULT_REGION, get_scw_client
 from scw_serverless.utils.loader import get_app_instance
 
 CLICK_ARG_FILE = click.argument(
     "file",
     required=True,
     type=click.Path(
@@ -38,14 +35,42 @@
 
 
 # TODO?: clean up the locals by introducing a class
 # pylint: disable=too-many-arguments,too-many-locals
 @cli.command()
 @CLICK_ARG_FILE
 @click.option(
+    "--backend",
+    "-b",
+    "backend",
+    default="api",
+    type=click.Choice(["api", "serverless"], case_sensitive=False),
+    show_default=True,
+    help="Select the backend used to deploy",
+)
+@click.option(
+    "--no-single-source",
+    "single_source",
+    is_flag=True,
+    default=True,
+    help="Do not remove functions not present in the code being deployed",
+)
+@click.option(
+    "--gateway-url",
+    "gateway_url",
+    default=None,
+    help="URL of a deployed API Gateway.",
+)
+@click.option(
+    "--gateway-api-key",
+    "gateway_api_key",
+    default=None,
+    help="API key used to manage the routes of the API Gateway.",
+)
+@click.option(
     "--profile",
     "-p",
     "profile_name",
     default=None,
     help="Scaleway profile to use when loading credentials.",
 )
 @click.option(
@@ -64,52 +89,24 @@
 )
 @click.option(
     "--region",
     "region",
     default=None,
     help=f"Region to deploy to. Default: {DEFAULT_REGION}",
 )
-@click.option(
-    "--no-single-source",
-    "single_source",
-    is_flag=True,
-    default=True,
-    help="Do not remove functions not present in the code being deployed",
-)
-@click.option(
-    "--backend",
-    "-b",
-    "backend",
-    default="api",
-    type=click.Choice(["api", "serverless"], case_sensitive=False),
-    show_default=True,
-    help="Select the backend used to deploy",
-)
-@click.option(
-    "--gw-id",
-    "-g",
-    "gateway_id",
-    envvar="SCW_APIGW_ID",
-    help="API Gateway uuid to use with function endpoints",
-)
-@click.option(
-    "--api-gw-host",
-    envvar="SCW_API_GW_HOST",
-    help="Host of the API to manage gateways",
-)
 def deploy(
     file: Path,
     backend: Literal["api", "serverless"],
     single_source: bool,
+    gateway_url: Optional[str] = None,
+    gateway_api_key: Optional[str] = None,
     profile_name: Optional[str] = None,
     secret_key: Optional[str] = None,
     project_id: Optional[str] = None,
     region: Optional[str] = None,
-    gateway_id: Optional[str] = None,
-    api_gw_host: Optional[str] = None,
 ) -> None:
     """Deploy your functions to Scaleway.
 
     FILE is the file containing your functions handlers
 
     If the credentials are not provided, the credentials will
     be pulled from your Scaleway configuration.
@@ -137,32 +134,32 @@
         logger.warning(f"Unknown backend selected: {backend}")
 
     deploy_backend.deploy()
 
     needs_gateway = any(function.gateway_route for function in app_instance.functions)
     if not needs_gateway:
         return
-    config = Config(api_gw_host, gateway_id).update_from_config_file()
-    # If gateway_id is not configured, gateway_domains needs to be set
-    is_gateway_configured = config.gateway_id or app_instance.gateway_domains
-    if not is_gateway_configured:
+
+    if not gateway_url:
         raise RuntimeError(
-            "Deploying a routed functions requires a"
-            + "gateway_id or a gateway_domain to be configured"
+            "Your application requires an API Gateway but no gateway URL was provided"
         )
-    if not config.api_gw_host:
-        raise RuntimeError("No api gateway host was configured")
-    # Update the gateway
-    manager = gateway.GatewayManager(
-        app_instance,
-        client,
-        config.gateway_id,
-        gateway.GatewayClient(config.api_gw_host),
+    if not gateway_api_key:
+        raise RuntimeError(
+            "Your application requires an API Gateway but "
+            + "no gateway API key was provided to manage routes"
+        )
+
+    manager = GatewayManager(
+        app_instance=app_instance,
+        gateway_url=gateway_url,
+        gateway_api_key=gateway_api_key,
+        sdk_client=client,
     )
-    manager.update_gateway_routes()
+    manager.update_routes()
 
 
 @cli.command()
 @CLICK_ARG_FILE
 @click.option(
     "--target",
     "-t",
@@ -190,25 +187,26 @@
     app_instance = get_app_instance(file)  # Get the serverless App instance
 
     get_logger().default(f"Generating configuration for target: {target}")
 
     if not os.path.exists(save):
         os.mkdir(save)
 
+    generator = None
     if target == "serverless":
-        serverless_framework_generator = ServerlessFrameworkGenerator(app_instance)
-        serverless_framework_generator.write(save)
+        generator = generators.ServerlessFrameworkGenerator(app_instance)
     elif target == "terraform":
-        terraform_generator = TerraformGenerator(
+        generator = generators.TerraformGenerator(
             app_instance,
             deps_manager=DependenciesManager(
                 file.parent.resolve(), file.parent.resolve()
             ),
         )
-        terraform_generator.write(save)
+    if generator:
+        generator.write(save)
 
     get_logger().success(f"Done! Generated configuration file saved in {save}")
 
 
 def main() -> int:
     """Entrypoint for click"""
     # Set logging level to DEFAULT. (ignore debug)
```

### Comparing `scw_serverless-0.0.4/scw_serverless/config/function.py` & `scw_serverless-1.0.0/scw_serverless/config/function.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,14 +39,15 @@
     :param max_scale: Maximum replicas for your function.
     :param memory_limit: Memory (in MB) allocated to your function.
     :param timeout: Max duration to respond to a request.
     :param description: Description. Defaults to the function docstring if defined.
     :param http_option: Either "enabled" or "redirected".
                         If "redirected" (default), allow http traffic to your function.
                         Blocked otherwise.
+
     .. seealso::
 
         Scaleway Developers Documentation
         https://developers.scaleway.com/en/products/functions/api/#create-a-function
     """
 
     env: dict[str, str]
@@ -56,16 +57,16 @@
     memory_limit: MemoryLimit
     timeout: str
     custom_domains: list[str]
     privacy: Privacy
     description: str
     http_option: HTTPOption
     # Parameters for the Gateway
-    url: str
-    methods: list[HTTPMethod]
+    relative_url: str
+    http_methods: list[HTTPMethod]
     # Triggers
     triggers: list[Trigger]
 
 
 # pylint: disable=too-many-instance-attributes
 @dataclass
 class Function:
@@ -102,16 +103,16 @@
         privacy = None
         if args_privacy := args.get("privacy"):
             privacy = sdk.FunctionPrivacy(args_privacy)
         http_option = None
         if args_http_option := args.get("http_option"):
             http_option = sdk.FunctionHttpOption(args_http_option)
         gateway_route = None
-        if url := args.get("url"):
-            gateway_route = GatewayRoute(url, methods=args.get("methods"))
+        if url := args.get("relative_url"):
+            gateway_route = GatewayRoute(url, http_methods=args.get("http_methods"))
 
         return Function(
             name=to_valid_fn_name(handler.__name__),
             handler=module_to_path(handler.__module__) + "." + handler.__name__,
             environment_variables=args.get("env"),
             min_scale=args.get("min_scale"),
             max_scale=args.get("max_scale"),
```

### Comparing `scw_serverless-0.0.4/scw_serverless/config/generators/serverless_framework.py` & `scw_serverless-1.0.0/scw_serverless/config/generators/serverless_framework.py`

 * *Files identical despite different names*

### Comparing `scw_serverless-0.0.4/scw_serverless/config/generators/terraform.py` & `scw_serverless-1.0.0/scw_serverless/config/generators/terraform.py`

 * *Files identical despite different names*

### Comparing `scw_serverless-0.0.4/scw_serverless/dependencies_manager.py` & `scw_serverless-1.0.0/scw_serverless/dependencies_manager.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 import pathlib
 import subprocess
 import sys
+from importlib.metadata import version
 from typing import Optional
 
 from scw_serverless.logger import get_logger
 
 REQUIREMENTS_NAME = "requirements.txt"
 
 
@@ -67,27 +68,29 @@
 
     def _check_for_scw_serverless(self):
         """Checks for scw_serverless after vendoring the dependencies."""
         if (
             not self.pkg_path.exists()
             or not self.pkg_path.joinpath(__package__).exists()
         ):
-            self._run_pip_install("scw_serverless")
+            # Installs the current version with pip
+            self._run_pip_install(f"{__package__}=={version(__package__)}")
 
     def _run_pip_install(self, *args: str):
         python_path = sys.executable
         command = [
             python_path,
             "-m",
             "pip",
             "install",
             *args,
             "--target",
             str(self.pkg_path.resolve()),
         ]
+
         try:
             subprocess.run(
                 command,
                 check=True,
                 stdout=subprocess.PIPE,
                 stderr=subprocess.PIPE,
                 cwd=str(self.out_path.resolve()),
```

### Comparing `scw_serverless-0.0.4/scw_serverless/deploy/backends/scaleway_api_backend.py` & `scw_serverless-1.0.0/scw_serverless/deploy/backends/scaleway_api_backend.py`

 * *Files identical despite different names*

### Comparing `scw_serverless-0.0.4/scw_serverless/deploy/backends/serverless_backend.py` & `scw_serverless-1.0.0/scw_serverless/deploy/backends/serverless_backend.py`

 * *Files identical despite different names*

### Comparing `scw_serverless-0.0.4/scw_serverless/deploy/backends/serverless_framework_backend.py` & `scw_serverless-1.0.0/scw_serverless/deploy/backends/serverless_framework_backend.py`

 * *Files identical despite different names*

### Comparing `scw_serverless-0.0.4/scw_serverless/logger.py` & `scw_serverless-1.0.0/scw_serverless/logger.py`

 * *Files identical despite different names*

### Comparing `scw_serverless-0.0.4/scw_serverless/triggers/cron.py` & `scw_serverless-1.0.0/scw_serverless/triggers/cron.py`

 * *Files identical despite different names*

### Comparing `scw_serverless-0.0.4/scw_serverless/utils/credentials.py` & `scw_serverless-1.0.0/scw_serverless/utils/credentials.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     secret_key: Optional[str],
     project_id: Optional[str],
     region: Optional[str],
 ) -> Client:
     """Attempts to load the profile. Will raise on invalid profiles."""
     client = Client.from_config_file_and_env(profile_name)
     _update_client_from_cli(client, secret_key, project_id, region)
+
     return _validate_client(client)
 
 
 def _validate_client(client: Client) -> Client:
     """Validate a SDK profile to be used with scw_serverless.
     Note: because we do not specify the project_id in API calls,
     it needs to be defined in the client.
@@ -43,7 +44,11 @@
     client.user_agent = f'scw-serverless/{version("scw_serverless")}'
     client.secret_key = secret_key or client.secret_key
     client.default_project_id = project_id or client.default_project_id
     client.default_region = region or client.default_region
     if not client.default_region:
         get_logger().info(f"No region was configured, using {DEFAULT_REGION}")
         client.default_region = DEFAULT_REGION
+
+    # Not used by the API framework
+    # Can lead to issues if project_id does not belong to organization
+    client.default_organization_id = None
```

### Comparing `scw_serverless-0.0.4/scw_serverless/utils/files.py` & `scw_serverless-1.0.0/scw_serverless/utils/files.py`

 * *Files identical despite different names*

### Comparing `scw_serverless-0.0.4/scw_serverless/utils/loader.py` & `scw_serverless-1.0.0/scw_serverless/utils/loader.py`

 * *Files identical despite different names*

### Comparing `scw_serverless-0.0.4/scw_serverless/utils/string.py` & `scw_serverless-1.0.0/scw_serverless/utils/string.py`

 * *Files identical despite different names*

### Comparing `scw_serverless-0.0.4/setup.py` & `scw_serverless-1.0.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,36 +3,36 @@
 
 packages = \
 ['scw_serverless',
  'scw_serverless.config',
  'scw_serverless.config.generators',
  'scw_serverless.deploy',
  'scw_serverless.deploy.backends',
- 'scw_serverless.deploy.gateway',
+ 'scw_serverless.gateway',
  'scw_serverless.triggers',
  'scw_serverless.utils']
 
 package_data = \
 {'': ['*'], 'scw_serverless.config': ['templates/*']}
 
 install_requires = \
 ['click>=8.1.3,<9.0.0',
  'pyyaml>=6.0,<7.0',
  'requests>=2.28.2,<3.0.0',
- 'scaleway>=0.7,<0.9']
+ 'scaleway>=0.7,<0.11']
 
 extras_require = \
 {':python_version < "3.11"': ['typing-extensions>=4.4.0,<5.0.0']}
 
 entry_points = \
 {'console_scripts': ['scw-serverless = scw_serverless.cli:main']}
 
 setup_kwargs = {
     'name': 'scw-serverless',
-    'version': '0.0.4',
+    'version': '1.0.0',
     'description': 'Framework for writing serverless APIs in Python, using Scaleway functions and containers.',
     'long_description': '# Serverless API Framework\n\n[![PyPI version](https://badge.fury.io/py/scw-serverless.svg)](https://badge.fury.io/py/scw-serverless)\n[![Documentation Status](https://readthedocs.org/projects/serverless-api-project/badge/?version=latest)](https://serverless-api-project.readthedocs.io/en/latest/?badge=latest)\n[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/scaleway/serverless-api-project/main.svg)](https://results.pre-commit.ci/latest/github/scaleway/serverless-api-project/main)\n\nServerless API Framework is a tool that lets you write and deploy serverless functions in python.\nIt bridges your code with the deployment configuration to make it a breeze to work with serverless functions.\n\nStarts by defining a simple Python function:\n\n```python\nfrom scw_serverless import Serverless\n\napp = Serverless("hello-namespace")\n\n@app.func(memory_limit=256)\ndef hello_world(event, context):\n    return "Hello World!"\n```\n\nDeploy it with `scw-serverless`:\n\n```console\nscw-serverless deploy app.py\n```\n\n## Quickstart\n\n### Install\n\n```console\npip install scw-serverless\n```\n\nThis will install the `scw-serverless` CLI:\n\n```console\nscw-serverless --help\n```\n\n### Writing and configuring functions\n\nYou can transform your python functions into serverless functions by using decorators:\n\n```python\nimport os\nimport requests\nfrom scw_serverless import Serverless\n\napp = Serverless("hello-namespace")\nAPI_URL = os.environ["API_URL"]\n\n@app.func(memory_limit=256, env={"API_URL": API_URL})\ndef hello_world(event, context):\n    return requests.get(API_URL)\n```\n\nThe configuration is done by passing arguments to the decorator.\nTo view which arguments are supported, head over to this [documentation](https://serverless-api-project.readthedocs.io/) page.\n\nWhen you are ready, you can deploy your function with the `scw-serverless` CLI tool:\n\n```console\nscw-serverless deploy app.py\n```\n\nThe tool will use your Scaleway credentials from your environment and config file.\n\n## What’s Next?\n\nTo learn more about the framework, have a look at the [documentation](https://serverless-api-project.readthedocs.io/).\nIf you want to see it in action, we provide some [examples](https://github.com/scaleway/serverless-api-project/tree/main/examples) to get you started.\n\n## Contributing\n\nWe welcome all contributions.\n\nThis project uses [pre-commit](https://pre-commit.com/) hooks to run code quality checks locally. We recommended installing them before contributing.\n\n```console\npre-commit install\n```\n',
     'author': 'Scaleway Serverless Team',
     'author_email': 'opensource@scaleway.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/scaleway/serverless-api-project',
```

### Comparing `scw_serverless-0.0.4/PKG-INFO` & `scw_serverless-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scw-serverless
-Version: 0.0.4
+Version: 1.0.0
 Summary: Framework for writing serverless APIs in Python, using Scaleway functions and containers.
 Home-page: https://github.com/scaleway/serverless-api-project
 License: MIT
 Keywords: serverless,scaleway,functions,cloud,faas
 Author: Scaleway Serverless Team
 Author-email: opensource@scaleway.com
 Requires-Python: >=3.9,<4.0
@@ -21,15 +21,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
-Requires-Dist: scaleway (>=0.7,<0.9)
+Requires-Dist: scaleway (>=0.7,<0.11)
 Requires-Dist: typing-extensions (>=4.4.0,<5.0.0) ; python_version < "3.11"
 Project-URL: Documentation, https://serverless-api-project.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/scaleway/serverless-api-project
 Description-Content-Type: text/markdown
 
 # Serverless API Framework
```

