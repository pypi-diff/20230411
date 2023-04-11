# Comparing `tmp/cognite_gql_pygen-0.1.2.tar.gz` & `tmp/cognite_gql_pygen-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_gql_pygen-0.1.2.tar", max compression
+gzip compressed data, was "cognite_gql_pygen-0.1.3.tar", max compression
```

## Comparing `cognite_gql_pygen-0.1.2.tar` & `cognite_gql_pygen-0.1.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0    11349 2023-04-11 11:54:24.795409 cognite_gql_pygen-0.1.2/LICENSE
--rw-r--r--   0        0        0     1758 2023-04-11 11:54:24.795409 cognite_gql_pygen-0.1.2/README.md
--rw-r--r--   0        0        0     8174 2023-04-11 11:54:24.795409 cognite_gql_pygen-0.1.2/cognite/fdm/README.md
--rw-r--r--   0        0        0        0 2023-04-11 11:54:24.795409 cognite_gql_pygen-0.1.2/cognite/fdm/__init__.py
--rw-r--r--   0        0        0      230 2023-04-11 11:54:24.795409 cognite_gql_pygen-0.1.2/cognite/fdm/bin/_functions.sh
--rwxr-xr-x   0        0        0      572 2023-04-11 11:54:24.795409 cognite_gql_pygen-0.1.2/cognite/fdm/bin/cdf_signin.sh
--rwxr-xr-x   0        0        0      379 2023-04-11 11:54:24.795409 cognite_gql_pygen-0.1.2/cognite/fdm/bin/schema_publish.sh
--rwxr-xr-x   0        0        0      321 2023-04-11 11:54:24.795409 cognite_gql_pygen-0.1.2/cognite/fdm/bin/schema_render.sh
--rw-r--r--   0        0        0      170 2023-04-11 11:54:24.795409 cognite_gql_pygen-0.1.2/cognite/fdm/cdf/__init__.py
--rw-r--r--   0        0        0    19044 2023-04-11 11:54:24.799409 cognite_gql_pygen-0.1.2/cognite/fdm/cdf/client_fdm_v3.py
--rw-r--r--   0        0        0     3911 2023-04-11 11:54:24.799409 cognite_gql_pygen-0.1.2/cognite/fdm/cdf/data_classes_fdm_v3.py
--rw-r--r--   0        0        0     2621 2023-04-11 11:54:24.799409 cognite_gql_pygen-0.1.2/cognite/fdm/cdf/get_client.py
--rw-r--r--   0        0        0      218 2023-04-11 11:54:24.799409 cognite_gql_pygen-0.1.2/cognite/fdm/config.example.yaml
--rw-r--r--   0        0        0      695 2023-04-11 11:54:24.799409 cognite_gql_pygen-0.1.2/cognite/fdm/config.py
--rw-r--r--   0        0        0      192 2023-04-11 11:54:24.799409 cognite_gql_pygen-0.1.2/cognite/fdm/custom_types/__init__.py
--rw-r--r--   0        0        0      236 2023-04-11 11:54:24.799409 cognite_gql_pygen-0.1.2/cognite/fdm/custom_types/_scalars.py
--rw-r--r--   0        0        0      978 2023-04-11 11:54:24.799409 cognite_gql_pygen-0.1.2/cognite/fdm/custom_types/jsonobject.py
--rw-r--r--   0        0        0     4948 2023-04-11 11:54:24.799409 cognite_gql_pygen-0.1.2/cognite/fdm/custom_types/timestamp.py
--rw-r--r--   0        0        0      196 2023-04-11 11:54:24.799409 cognite_gql_pygen-0.1.2/cognite/fdm/general_domain/__init__.py
--rw-r--r--   0        0        0     6191 2023-04-11 11:54:24.799409 cognite_gql_pygen-0.1.2/cognite/fdm/general_domain/domain_client.py
--rw-r--r--   0        0        0     3043 2023-04-11 11:54:24.799409 cognite_gql_pygen-0.1.2/cognite/fdm/general_domain/domain_model.py
--rw-r--r--   0        0        0    15849 2023-04-11 11:54:24.799409 cognite_gql_pygen-0.1.2/cognite/fdm/general_domain/domain_model_api.py
--rw-r--r--   0        0        0     3597 2023-04-11 11:54:24.799409 cognite_gql_pygen-0.1.2/cognite/fdm/general_domain/relationship_api.py
--rw-r--r--   0        0        0     6848 2023-04-11 11:54:24.799409 cognite_gql_pygen-0.1.2/cognite/fdm/general_domain/schema.py
--rw-r--r--   0        0        0      869 2023-04-11 11:54:24.799409 cognite_gql_pygen-0.1.2/cognite/fdm/main.py
--rw-r--r--   0        0        0     1423 2023-04-11 11:54:24.799409 cognite_gql_pygen-0.1.2/cognite/fdm/misc.py
--rw-r--r--   0        0        0        0 2023-04-11 11:54:24.799409 cognite_gql_pygen-0.1.2/cognite/fdm/py.typed
--rw-r--r--   0        0        0       76 2023-04-11 11:54:24.799409 cognite_gql_pygen-0.1.2/cognite/gqlpygen/__init__.py
--rw-r--r--   0        0        0      300 2023-04-11 11:54:24.799409 cognite_gql_pygen-0.1.2/cognite/gqlpygen/main.py
--rw-r--r--   0        0        0       22 2023-04-11 11:54:24.799409 cognite_gql_pygen-0.1.2/cognite/gqlpygen/version.py
--rw-r--r--   0        0        0     1282 2023-04-11 11:54:24.799409 cognite_gql_pygen-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2662 1970-01-01 00:00:00.000000 cognite_gql_pygen-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    11349 2023-04-11 12:46:44.297154 cognite_gql_pygen-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1782 2023-04-11 12:46:44.297154 cognite_gql_pygen-0.1.3/README.md
+-rw-r--r--   0        0        0     8252 2023-04-11 12:46:44.297154 cognite_gql_pygen-0.1.3/cognite/dm_clients/README.md
+-rw-r--r--   0        0        0        0 2023-04-11 12:46:44.297154 cognite_gql_pygen-0.1.3/cognite/dm_clients/__init__.py
+-rw-r--r--   0        0        0      237 2023-04-11 12:46:44.297154 cognite_gql_pygen-0.1.3/cognite/dm_clients/bin/_functions.sh
+-rwxr-xr-x   0        0        0      572 2023-04-11 12:46:44.297154 cognite_gql_pygen-0.1.3/cognite/dm_clients/bin/cdf_signin.sh
+-rwxr-xr-x   0        0        0      379 2023-04-11 12:46:44.297154 cognite_gql_pygen-0.1.3/cognite/dm_clients/bin/schema_publish.sh
+-rwxr-xr-x   0        0        0      369 2023-04-11 12:46:44.297154 cognite_gql_pygen-0.1.3/cognite/dm_clients/bin/schema_render.sh
+-rw-r--r--   0        0        0      167 2023-04-11 12:46:44.297154 cognite_gql_pygen-0.1.3/cognite/dm_clients/cdf/__init__.py
+-rw-r--r--   0        0        0    19067 2023-04-11 12:46:44.297154 cognite_gql_pygen-0.1.3/cognite/dm_clients/cdf/client_dm_v3.py
+-rw-r--r--   0        0        0     3910 2023-04-11 12:46:44.297154 cognite_gql_pygen-0.1.3/cognite/dm_clients/cdf/data_classes_dm_v3.py
+-rw-r--r--   0        0        0     2628 2023-04-11 12:46:44.297154 cognite_gql_pygen-0.1.3/cognite/dm_clients/cdf/get_client.py
+-rw-r--r--   0        0        0      225 2023-04-11 12:46:44.297154 cognite_gql_pygen-0.1.3/cognite/dm_clients/config.example.yaml
+-rw-r--r--   0        0        0      709 2023-04-11 12:46:44.297154 cognite_gql_pygen-0.1.3/cognite/dm_clients/config.py
+-rw-r--r--   0        0        0      192 2023-04-11 12:46:44.297154 cognite_gql_pygen-0.1.3/cognite/dm_clients/custom_types/__init__.py
+-rw-r--r--   0        0        0      236 2023-04-11 12:46:44.297154 cognite_gql_pygen-0.1.3/cognite/dm_clients/custom_types/_scalars.py
+-rw-r--r--   0        0        0      760 2023-04-11 12:46:44.297154 cognite_gql_pygen-0.1.3/cognite/dm_clients/custom_types/jsonobject.py
+-rw-r--r--   0        0        0     4724 2023-04-11 12:46:44.297154 cognite_gql_pygen-0.1.3/cognite/dm_clients/custom_types/timestamp.py
+-rw-r--r--   0        0        0      196 2023-04-11 12:46:44.297154 cognite_gql_pygen-0.1.3/cognite/dm_clients/domain_modeling/__init__.py
+-rw-r--r--   0        0        0     6273 2023-04-11 12:46:44.297154 cognite_gql_pygen-0.1.3/cognite/dm_clients/domain_modeling/domain_client.py
+-rw-r--r--   0        0        0     3046 2023-04-11 12:46:44.297154 cognite_gql_pygen-0.1.3/cognite/dm_clients/domain_modeling/domain_model.py
+-rw-r--r--   0        0        0    15859 2023-04-11 12:46:44.297154 cognite_gql_pygen-0.1.3/cognite/dm_clients/domain_modeling/domain_model_api.py
+-rw-r--r--   0        0        0     3609 2023-04-11 12:46:44.297154 cognite_gql_pygen-0.1.3/cognite/dm_clients/domain_modeling/relationship_api.py
+-rw-r--r--   0        0        0     6828 2023-04-11 12:46:44.297154 cognite_gql_pygen-0.1.3/cognite/dm_clients/domain_modeling/schema.py
+-rw-r--r--   0        0        0      868 2023-04-11 12:46:44.297154 cognite_gql_pygen-0.1.3/cognite/dm_clients/main.py
+-rw-r--r--   0        0        0     1423 2023-04-11 12:46:44.297154 cognite_gql_pygen-0.1.3/cognite/dm_clients/misc.py
+-rw-r--r--   0        0        0        0 2023-04-11 12:46:44.297154 cognite_gql_pygen-0.1.3/cognite/dm_clients/py.typed
+-rw-r--r--   0        0        0       76 2023-04-11 12:46:44.297154 cognite_gql_pygen-0.1.3/cognite/gqlpygen/__init__.py
+-rw-r--r--   0        0        0      300 2023-04-11 12:46:44.301154 cognite_gql_pygen-0.1.3/cognite/gqlpygen/main.py
+-rw-r--r--   0        0        0       22 2023-04-11 12:46:44.301154 cognite_gql_pygen-0.1.3/cognite/gqlpygen/version.py
+-rw-r--r--   0        0        0     1696 2023-04-11 12:46:44.301154 cognite_gql_pygen-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2686 1970-01-01 00:00:00.000000 cognite_gql_pygen-0.1.3/PKG-INFO
```

### Comparing `cognite_gql_pygen-0.1.2/LICENSE` & `cognite_gql_pygen-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.1.2/README.md` & `cognite_gql_pygen-0.1.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Cognite GraphQL Python Generator
 ==========================
 [![build](https://github.com/cognitedata/cognite-gql-pygen/actions/workflows/release.yaml/badge.svg)](https://github.com/cognitedata/cognite-gql-pygen/actions/workflows/release.yaml)
 [![GitHub](https://img.shields.io/github/license/cognitedata/cognite-gql-pygen)](https://github.com/cognitedata/cognite-gql-pygen/blob/master/LICENSE)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
 
 This is the Cognite GraphQL Python Generator, `gqlpygen`, which is a CLI for automatically generating Python SDK code
-from `.graphql` to interact with Cognite Data Fusion's (CDF) Flexible Data Models (FDM). It also supports other cases,
+from `.graphql` to interact with Cognite Data Fusion's (CDF) Flexible Data Models (DM). It also supports other cases,
 such as generating `.graphql` from `pydantic` classes.
 
 **[DISCLAIMER!]** This project is in a highly experimental no guarantees are made for consistency between versions. The
 project may also become deprecated if the experimentation turns out to be a dead end.
 
 
-### FDM Non-GraphQl API
+### DM Non-GraphQl API
 
-This package also contains `cognite.fdm` which is a simplified wrapper for non-GraphQL endpoints in FDM API v3.
+This package also contains `cognite.dm_clients` which is a simplified wrapper for non-GraphQL endpoints in DM API v3.
 
-See [fdm/README.md](./fdm/README.md) for more details.
+See [dm_clients/README.md](cognite/dm_clients/README.md) for more details.
 
 ## Installation
 
 To install this package:
 ```bash
 $ pip install cognite-gql-pygen
 ```
```

### Comparing `cognite_gql_pygen-0.1.2/cognite/fdm/README.md` & `cognite_gql_pygen-0.1.3/cognite/dm_clients/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,77 +1,77 @@
-# Non-GraphQL FDM API
+# Non-GraphQL DM API
 
-This is an experimental module which wraps non-GraphQL API for FDM.
+This is an experimental module which wraps non-GraphQL API for DM.
 
-It provides a simplified set of features for interacting with FDM in an intuitive way and without needing to work with
+It provides a simplified set of features for interacting with DM in an intuitive way and without needing to work with
 the underlying data structures.
 
 **[DISCLAIMER!]** This project is in a highly experimental no guarantees are made for consistency between versions. The
 project may also become deprecated if the experimentation turns out to be a dead end.
 
 
 ## Motivation
 
-Uploading some data into a FDM data model was cumbersome when interacting directly with the FDM API.
+Uploading some data into a DM data model was cumbersome when interacting directly with the DM API.
 
 
 ## Concepts
 
-`fdm` package takes Python code as the "source of truth". So a normal workflow is like this:
+`dm_clients` package takes Python code as the "source of truth". So a normal workflow is like this:
 
 1. Define use case models in Python (in a "schema" module).
 2. Use CLI from this package to generate GraphQL schema.
-3. Use CLI from this package to upload this schema to FDM.
-4. Populate and manipulate data items / instances in FDM using a `DomainClient` provided in this package.
+3. Use CLI from this package to upload this schema to DM.
+4. Populate and manipulate data items / instances in DM using a `DomainClient` provided in this package.
 
 
 > Note: This might change in the future: as `gqlpygen` module evolves we should be able to dynamically create Python
-> data types from existing GraphQL schemas in FDM.
+> data types from existing GraphQL schemas in DM.
 
 
 ## Future
 
 Uncertain. No guarantees are made about maintenance of this project. Contributions, however, are very welcome!
 
-With the (future) arrival of GraphQL mutations in FDM, this package might become obsolete.
+With the (future) arrival of GraphQL mutations in DM, this package might become obsolete.
 
 
 ## Glossary
 
- * FDM - Flexible Data Model, data service by Cognite. For our purposes, it is "the API".
- * `fdm` - this package
- * Space - FDM object, a high-level container for all things in FDM. Like a namespace. Subordinate only to CDF project.
+ * DM - CDF Data Modeling, data service by Cognite. For our purposes, it is "the API".
+ * `dm_clients` - this package
+ * Space - DM object, a high-level container for all things in DM. Like a namespace. Subordinate only to CDF project.
  * Data Model - Often used interchangeably with "Schema", a set of Domain Models (a.k.a. schema types) that together
    help model a use case.
  * Domain - knowledge domain, similar to use case (though we can have multiple use cases that use a single Domain,
    like several clients in a very similar business)
- * Domain Model - an `fdm` term - often used interchangeably with "schema type" - a single class of objects with all
-   its fields, e.g. "pump" or "generator".
- * Item - an `fdm` term - an instance of a Domain Model, e.g. generator "G42".
- * Instance - an FDM term - a data entity, either a Node or an Edge (see below).
- * Node - an FDM term - a data entity, can contain multiple fields.
- * Edge - an FDM term - a data entity that connects two nodes (directionally).
- * DomainAPI - an `fdm` term - a top-level Python class for a Domain. It provides easy access to various DomainModelAPIs
-   (see below).
- * DomainModelAPI - an `fdm` term - a Python class (or class instance) which provides management over a single Domain
-   Model, e.g. create new pumps, delete a pump, list all pumps...
- * DomainClient - an `fdm` term - a Python class (or class instance) which serves as a namespace for easy acces to all
-   DomainModelAPIs in a use case.
+ * Domain Model - a `dm_clients` term - often used interchangeably with "schema type" - a single class of objects with
+   all its fields, e.g. "pump" or "generator".
+ * Item - a `dm_clients` term - an instance of a Domain Model, e.g. generator "G42".
+ * Instance - a DM term - a data entity, either a Node or an Edge (see below).
+ * Node - a DM term - a data entity, can contain multiple fields.
+ * Edge - a DM term - a data entity that connects two nodes (directionally).
+ * DomainAPI - a `dm_clients` term - a top-level Python class for a Domain. It provides easy access to various
+   DomainModelAPIs (see below).
+ * DomainModelAPI - a `dm_clients` term - a Python class (or class instance) which provides management over a single
+   DomainModel, e.g. create new pumps, delete a pump, list all pumps...
+ * DomainClient - a `dm_clients` term - a Python class (or class instance) which serves as a namespace for easy access
+   to all DomainModelAPIs in a use case.
 
 
 ## Installation
 
 1. `pip install cognite-gql-pygen`
 2. Create a `config.yaml` file (exact name not important), see [config.example.yaml](./config.example.yaml).
    - > TODO: Then need for `config.yaml` should be removed...
-3. Define `FDM_CONFIG` env variable to contain the full path to `config.yaml` file.
+3. Define `DM_CLIENTS_CONFIG` env variable to contain the full path to `config.yaml` file.
 4. Test if it works:
    ```
    $ python
-   >>> from cognite.fdm.general_domain.domain_client import get_empty_domain_client
+   >>> from cognite.dm_clients.domain_modeling.domain_client import get_empty_domain_client
    >>> c = get_empty_domain_client()
    >>> c._client.spaces.list()
    [Space(space="...
    ```
 5. Install CDF CLI client
    - [setup instructions](https://docs.cognite.com/cdf/cli/)
    - But basically:
@@ -107,24 +107,24 @@
 > Before proceeding, make sure that `config.yaml` is populated with credentials and configuration.
 
 
 ##### Step 1: Render Schema
 
 GraphQL schema file is committed to this repo, so this step is not required, but it is here for completeness.
 
-Execute `fdm schema render`. This will update the schema file (defined in `config.yaml`) according to Python code in
+Execute `dm_clients schema render`. This will update the schema file (defined in `config.yaml`) according to Python code in
 the schema module.
 
 
 ##### Step 2: Upload Schema
 
-Authenticate against CDF by running `fdm signin`. The authentication data is cached on the filesystem
+Authenticate against CDF by running `dm_clients signin`. The authentication data is cached on the filesystem
 locally, so this is needed rarely (every few? days).
 
-Execute `fdm schema publish`. This will upload the schema to CDF / FDM.
+Execute `dm_clients schema publish`. This will upload the schema to CDF / DM.
 
 > Note: Depending on the changes made to the schema, you might be required to update the schema version in config.yaml.
 > This happens when the changes are not backwards-compatible, e.g. deleting a field.
 
 
 ### Manipulate Items
 
@@ -154,21 +154,21 @@
 Note that `_client` is a subclass of `CogniteClient` and can be used to access "classic" data types (Assets,
 Timeseries, etc.)
 
 ## Pros and Cons
 
 Pros:
 
- * Simplifies interaction with FDM API
+ * Simplifies interaction with DM API
  * Uses Pydantic to validate the items before sending then to the API.
 
 Drawbacks and Limitations:
 
- * Not all features of FDM are supported.
-   * `fdm` is only tested to work within a single space.
+ * Not all features of DM are supported.
+   * `dm_clients` is only tested to work within a single space.
      * Across-space relationships are in principle possible, but some work would be needed to implement it.
    * Nodes (and consequently items) work with properties from only one view.
      * No hard barriers to implementing this in the future.
  * Not terribly efficient.
    * Developed mostly as a tool for getting things done, rather than an optimal implementation.
  * Unpolished, possibly with some bugs.
    * External IDs are constructed, not safely considering the char limit.
@@ -199,14 +199,14 @@
 Contributions welcome!
 
 See [TODO](#todo) above.
 
 ### Project Structure
 
 Important modules:
- * `cognite/fdm/cdf`
-    * general-purpose FDM client (nothing specific to PowerOps in here)
+ * `cognite/dm_clients/cdf`
+    * general-purpose DM client (nothing specific to PowerOps in here)
     * inspired by https://github.com/cognitedata/tech-demo-powerops/ :]
- * `cognite/fdm/general_domain`
+ * `cognite/dm_clients/domain_modeling`
     * base classes for use cases, "boilerplate"
  * `examples/cinematography_domain`
     * a toy example use case with minimal code
```

### Comparing `cognite_gql_pygen-0.1.2/cognite/fdm/bin/cdf_signin.sh` & `cognite_gql_pygen-0.1.3/cognite/dm_clients/bin/cdf_signin.sh`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.1.2/cognite/fdm/cdf/client_fdm_v3.py` & `cognite_gql_pygen-0.1.3/cognite/dm_clients/cdf/client_dm_v3.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,24 +9,24 @@
 from cognite.client import ClientConfig, CogniteClient
 from cognite.client._api_client import APIClient
 from cognite.client.exceptions import CogniteAPIError
 from pydantic import parse_obj_as
 from requests import Response
 from retry import retry
 
-from cognite.fdm.cdf.data_classes_fdm_v3 import Container, DataModel, Edge, Node, Space, View
-from cognite.fdm.cdf.get_client import get_client_config
-from cognite.fdm.config import CONFIG
+from cognite.dm_clients.cdf.data_classes_dm_v3 import Container, DataModel, Edge, Node, Space, View
+from cognite.dm_clients.cdf.get_client import get_client_config
+from cognite.dm_clients.config import CONFIG
 
 logger = logging.getLogger(__name__)
 
 
 HttpVerbT = Literal["GET", "PUT", "DELETE", "POST"]
 
-_MAX_TRIES = int(CONFIG["fdm"].get("max_tries", 15))
+_MAX_TRIES = int(CONFIG["dm_clients"].get("max_tries", 15))
 
 
 class DataModelStorageAPI(APIClient):
     """Base for other API classes"""
 
     @property
     def url(self) -> str:
@@ -467,15 +467,15 @@
         _ext_ids = list(external_ids)
         if not _ext_ids:
             return
         payload = {"items": [self._payload_item(space, ext_id) for ext_id in _ext_ids]}
         self._post_to_endpoint(payload, "/delete")
 
 
-class CogniteClientFdmV3(CogniteClient):
+class CogniteClientDmV3(CogniteClient):
     def __init__(self, config: ClientConfig):
         # config.headers["cdf-version"] = "alpha"
         super().__init__(config)
         self.spaces = SpacesAPI(self._config, api_version=self._API_VERSION, cognite_client=self)
         self.datamodels = DataModelAPI(self._config, api_version=self._API_VERSION, cognite_client=self)
         self.views = ViewsAPI(self._config, api_version=self._API_VERSION, cognite_client=self)
         self.containers = ContainersAPI(self._config, api_version=self._API_VERSION, cognite_client=self)
@@ -489,10 +489,10 @@
         return self.post(
             f"/api/v1/projects/{self.config.project}/userapis"
             f"/spaces/{space}/datamodels/{datamodel}/versions/{version}/graphql",
             json={"query": query},
         ).json()
 
 
-def get_cognite_client_fdm_v3() -> CogniteClientFdmV3:
+def get_cognite_client_dm_v3() -> CogniteClientDmV3:
     client_config = get_client_config()
-    return CogniteClientFdmV3(client_config)
+    return CogniteClientDmV3(client_config)
```

### Comparing `cognite_gql_pygen-0.1.2/cognite/fdm/cdf/data_classes_fdm_v3.py` & `cognite_gql_pygen-0.1.3/cognite/dm_clients/cdf/data_classes_dm_v3.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,15 +107,15 @@
     startNode: RelationReference
     endNode: RelationReference
     version: Optional[str] = None
     createdTime: Optional[int] = None
     lastUpdatedTime: Optional[int] = None
     deletedTime: Optional[int] = None
     properties: Optional[dict] = None  # TODO much structure here, nested spaces, view-or-container, then properties
-    # TODO Edge.properties not fully supported yet by FDM and not implemented in this library!
+    # TODO Edge.properties not fully supported yet by DM and not implemented in this library!
 
 
 class ExternalIdStr(ConstrainedStr):
     min_length = 1
     max_length = 255
```

### Comparing `cognite_gql_pygen-0.1.2/cognite/fdm/cdf/get_client.py` & `cognite_gql_pygen-0.1.3/cognite/dm_clients/cdf/get_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 from typing import List, Optional, Union
 
 from cognite.client import ClientConfig, CogniteClient
 from cognite.client.credentials import OAuthClientCredentials, OAuthInteractive
 from pydantic import BaseSettings, validator
 
-from cognite.fdm.config import CONFIG
+from cognite.dm_clients.config import CONFIG
 
 
 class CogniteConfig(BaseSettings):
     project: str
     cdf_cluster: str
     tenant_id: str
     client_id: Optional[str]
```

### Comparing `cognite_gql_pygen-0.1.2/cognite/fdm/config.py` & `cognite_gql_pygen-0.1.3/cognite/dm_clients/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 
 import yaml
 
 logger = logging.getLogger(__name__)
 
 PWD = Path().absolute()
 
-CONFIG_FILE = os.environ.get("FDM_CONFIG", PWD / "config.yaml")
+CONFIG_FILE = os.environ.get("DM_CLIENTS_CONFIG", PWD / "config.yaml")
 
 __all__ = [
     "CONFIG",
     "PWD",
 ]
 
 test_config = {
-    "fdm": {
+    "dm_clients": {
         "max_tries": 1,
     }
 }
 
 
 # TODO since this is in an installable package now, we should refactor to remove the need for a config file.
 try:
```

### Comparing `cognite_gql_pygen-0.1.2/cognite/fdm/custom_types/jsonobject.py` & `cognite_gql_pygen-0.1.3/cognite/dm_clients/custom_types/jsonobject.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,45 +1,35 @@
 from __future__ import annotations
 
 import json
 import logging
-from typing import TYPE_CHECKING, Annotated, Any, Dict
+from typing import Any, Dict
 
 logger = logging.getLogger(__name__)
 
 
 __all__ = [
     "JSONObject",
 ]
 
 
-class _JSONObject(dict):
+class JSONObject(dict):
     """
     Python dict that can be serialized into JSON format.
-    Note: FDM supports lists as well, but this implementation does not!
+    Note: DM supports lists as well, but this implementation does not!
     """
 
     @classmethod
     def __get_validators__(cls):
         yield cls.validate
 
     @classmethod
     def __modify_schema__(cls, field_schema):
         field_schema["description"] = "JSON-serializable Python dict."
 
     @classmethod
-    def validate(cls, value: Dict[str, Any]) -> _JSONObject:
+    def validate(cls, value: Dict[str, Any]) -> JSONObject:
         json.dumps(value)
         return cls(value)
 
     def __repr__(self) -> str:
         return f"JSONObject({super().__repr__()})"
-
-
-# Keeping mypy and strawberry and pydantic happy:
-
-_JSONObject.__name__ = "JSONObject"
-
-if TYPE_CHECKING:
-    JSONObject = Annotated[dict, _JSONObject]
-else:
-    JSONObject = _JSONObject
```

### Comparing `cognite_gql_pygen-0.1.2/cognite/fdm/custom_types/timestamp.py` & `cognite_gql_pygen-0.1.3/cognite/dm_clients/custom_types/timestamp.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from __future__ import annotations
 
 import logging
 import re
 from contextlib import suppress
 from datetime import datetime
 from math import floor
-from typing import TYPE_CHECKING, Annotated, TypeVar
+from typing import TypeVar
 
 logger = logging.getLogger(__name__)
 
 
 __all__ = [
     "Timestamp",
 ]
 
 
 TimestampParsable = TypeVar("TimestampParsable", str, datetime)
 
 
-class _Timestamp(str):
+class Timestamp(str):
     """
     String in the format 'YYYY-MM-DDTHH:MM:SS[.millis][Z|time zone]' with optional milliseconds having precision
     of 1-3 decimal digits and optional timezone with format ±HH:MM, ±HHMM, ±HH or Z, where Z represents UTC, Year
     must be between 0001 and 9999.
 
     Value must conform to this format to be accepted.
     One exception to this is that additional decimal digits of the second will be accepted but the value will be cut
@@ -102,15 +102,15 @@
 
         for fmt in formats:
             with suppress(ValueError):
                 return datetime.strptime(value, fmt)
         raise ValueError(f"Cannot parse Timestamp: {value}")
 
     @classmethod
-    def validate(cls, value: TimestampParsable) -> _Timestamp:
+    def validate(cls, value: TimestampParsable) -> Timestamp:
         str_value: str
         datetime_value: datetime
 
         if isinstance(value, str):
             datetime_value = cls._parse_str(value)
             str_value = value
 
@@ -130,17 +130,7 @@
         return cls(str_value)
 
     def __repr__(self) -> str:
         return f"Timestamp({super().__repr__()})"
 
     def datetime(self) -> datetime:
         return Timestamp._parse_str(self)
-
-
-# Keeping mypy and strawberry and pydantic happy:
-
-_Timestamp.__name__ = "Timestamp"
-
-if TYPE_CHECKING:
-    Timestamp = Annotated[TimestampParsable, _Timestamp]
-else:
-    Timestamp = _Timestamp
```

### Comparing `cognite_gql_pygen-0.1.2/cognite/fdm/general_domain/domain_client.py` & `cognite_gql_pygen-0.1.3/cognite/dm_clients/domain_modeling/domain_client.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Dict, Generic, Iterable, List, Optional, Type, TypeVar
 
 from cachelib import BaseCache
 from cognite.client import ClientConfig
 
-from cognite.fdm.cdf.client_fdm_v3 import CogniteClientFdmV3, EdgesAPI, NodesAPI
-from cognite.fdm.config import CONFIG
+from cognite.dm_clients.cdf.client_dm_v3 import CogniteClientDmV3, EdgesAPI, NodesAPI
+from cognite.dm_clients.config import CONFIG
 
-from ..cdf.client_fdm_v3 import ViewsAPI
+from ..cdf.client_dm_v3 import ViewsAPI
 from .domain_model import DomainModel
 
 if TYPE_CHECKING:
     from .domain_model_api import DomainModelAPI
     from .schema import Schema
 
 
@@ -42,21 +42,21 @@
         schema_version: Optional[int] = None,
         # TODO ^ some of these args are redundant.
     ):
         # TODO make all these attributes "_private" to distinguish from domain model APIs
         self.schema = schema
         self._domain_model_api_class = domain_model_api_class
         self.cache: BaseCache = cache
-        self._client = CogniteClientFdmV3(config)
+        self._client = CogniteClientDmV3(config)
         self._client._config.headers["cdf-version"] = "alpha"
         if space_id is None:
-            space_id = CONFIG["fdm"]["space"]
+            space_id = CONFIG["dm_clients"]["space"]
         self.space_id = space_id
-        self._data_model = data_model or CONFIG["fdm"].get("datamodel")
-        self.schema_version = schema_version or CONFIG["fdm"].get("schema_version")
+        self._data_model = data_model or CONFIG["dm_clients"].get("datamodel")
+        self.schema_version = schema_version or CONFIG["dm_clients"].get("schema_version")
         if self.schema_version is None:
             raise NotImplementedError("Please specify the schema version")
             # TODO find latest version of the data model
         self._api_map: Dict[Type[DomainModelT], str] = {}
 
         nodes_api = NodesAPI(
             self._client.config,
@@ -133,21 +133,21 @@
     def graph(self, query: str):
         return self._client.graph(self.space_id, self._data_model, str(self.schema_version), query)
 
 
 def get_empty_domain_client():
     from cachelib import SimpleCache
 
-    from cognite.fdm.cdf.get_client import get_client_config
-    from cognite.fdm.config import CONFIG
-    from cognite.fdm.general_domain.domain_model_api import DomainModelAPI
-    from cognite.fdm.general_domain.schema import Schema
+    from cognite.dm_clients.cdf.get_client import get_client_config
+    from cognite.dm_clients.config import CONFIG
+    from cognite.dm_clients.domain_modeling.domain_model_api import DomainModelAPI
+    from cognite.dm_clients.domain_modeling.schema import Schema
 
     return DomainClient(
         schema=Schema(),
         domain_model_api_class=DomainModelAPI,
         cache=SimpleCache(),
         config=get_client_config(),
-        space_id=CONFIG["fdm"]["space"],
-        data_model=CONFIG["fdm"]["datamodel"],
-        schema_version=CONFIG["fdm"]["schema_version"],
+        space_id=CONFIG["dm_clients"]["space"],
+        data_model=CONFIG["dm_clients"]["datamodel"],
+        schema_version=CONFIG["dm_clients"]["schema_version"],
     )
```

### Comparing `cognite_gql_pygen-0.1.2/cognite/fdm/general_domain/domain_model.py` & `cognite_gql_pygen-0.1.3/cognite/dm_clients/domain_modeling/domain_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,32 +2,32 @@
 
 import logging
 from typing import Dict, Optional, Type, get_args
 
 import strawberry
 from pydantic import Extra
 
-from cognite.fdm.cdf.data_classes_fdm_v3 import DataModelBase
+from cognite.dm_clients.cdf.data_classes_dm_v3 import DataModelBase
 
 __all__ = [
     "DomainModel",
 ]
 
 
 logger = logging.getLogger(__name__)
 
 
 class DomainModel(DataModelBase):
     """
     Base class for all models in schema_types.py
 
     A bit of nomenclature: instances of DomainModel we call "items".
-    This is pretty much because all other words I can think of have been taken by FDM >:]
+    This is pretty much because all other words I can think of have been taken by DM >:]
 
-    Even this is confusing... A data model in FDM is a collection of domain models.
+    Even this is confusing... A data model in DM is a collection of domain models.
     """
 
     externalId: strawberry.Private[Optional[str]] = None
     # Private ^ means the field will not be exposed in GraphQL schema
     # Used here because actual objects (returned from the API) have these fields. These are "implicit" field.
 
     class Config:
@@ -35,15 +35,15 @@
         #  ^ raises exception if extra fields are passed to the constructor. Very useful for development.
         arbitrary_types_allowed = True
 
     @classmethod
     def get_one_to_many_attrs(cls) -> Dict[str, Type[DomainModel]]:
         """
         Get attributes which describe one-to-many relationships.
-        These attributes usually require additional considerations with FDM.
+        These attributes usually require additional considerations with DM.
         """
         attrs = {}
         props: Dict[str, dict] = cls.schema()["properties"]
         for field_name, field_info in props.items():
             if field_info.get("type") != "array":
                 continue  # one-to-many has to be an array
             if field_info.get("items", {}).get("$ref", "").startswith("#/definitions/"):
```

### Comparing `cognite_gql_pygen-0.1.2/cognite/fdm/general_domain/domain_model_api.py` & `cognite_gql_pygen-0.1.3/cognite/dm_clients/domain_modeling/domain_model_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 import logging
 from collections import defaultdict
 from concurrent.futures import ThreadPoolExecutor
 from typing import Any, Dict, Generic, Iterable, List, Optional, Tuple, Type, TypeVar, get_args
 from uuid import uuid4
 
-from cognite.fdm.cdf.client_fdm_v3 import EdgesAPI, NodesAPI
-from cognite.fdm.cdf.data_classes_fdm_v3 import Node, View
+from cognite.dm_clients.cdf.client_dm_v3 import EdgesAPI, NodesAPI
+from cognite.dm_clients.cdf.data_classes_dm_v3 import Node, View
 
 from .domain_client import DomainClient
 from .domain_model import DomainModel
 from .relationship_api import RelationshipAPI
 
 __all__ = [
     "DomainModelAPI",
@@ -24,15 +24,15 @@
 
 
 DomainModelT = TypeVar("DomainModelT", bound=DomainModel)
 
 
 class DomainModelAPI(Generic[DomainModelT]):
     """
-    Node is an instance of a type in FDM, i.e. an instance of a subclass of DomainModel,
+    Node is an instance of a type in DM, i.e. an instance of a subclass of DomainModel,
     e.g: a single plant, a single pump...
     Caution: Naming is not terribly consistent inside cdf package!
     """
 
     def __init__(
         self,
         domain_model: Type[DomainModelT],
@@ -69,15 +69,15 @@
         o2m_attrs = self.domain_model.get_one_to_many_attrs()
 
         for item in items:
             # invent externalId if missing:
             if not item.externalId:
                 item.externalId = f"{type(item).__name__}_{uuid4().hex[:16]}"  # TODO configurable rnd hash length
 
-            # FDM doesn't like empty lists, making sure they are replaced with None:
+            # DM doesn't like empty lists, making sure they are replaced with None:
             # TODO this ^ was true for v2, check again for v3
             for attr in o2m_attrs:
                 val = getattr(item, attr)
                 if isinstance(val, list) and not val:
                     setattr(item, attr, None)
 
         return list(items)
```

### Comparing `cognite_gql_pygen-0.1.2/cognite/fdm/general_domain/relationship_api.py` & `cognite_gql_pygen-0.1.3/cognite/dm_clients/domain_modeling/relationship_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 import logging
 from concurrent.futures import ThreadPoolExecutor
 from typing import Iterable, List, Sequence, Type
 
-from cognite.fdm.cdf.client_fdm_v3 import EdgesAPI
-from cognite.fdm.cdf.data_classes_fdm_v3 import Edge, RelationReference, View
+from cognite.dm_clients.cdf.client_dm_v3 import EdgesAPI
+from cognite.dm_clients.cdf.data_classes_dm_v3 import Edge, RelationReference, View
 
 from .domain_model import DomainModel
 
 logger = logging.getLogger(__name__)
 
 
 class RelationshipAPI:
```

### Comparing `cognite_gql_pygen-0.1.2/cognite/fdm/general_domain/schema.py` & `cognite_gql_pygen-0.1.3/cognite/dm_clients/domain_modeling/schema.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 import logging
 from typing import Dict, Generic, List, Optional, Type, TypeVar, Union, cast, get_args
 
 import strawberry
 from strawberry.experimental.pydantic import UnregisteredTypeException
 from strawberry.schema.config import StrawberryConfig
 
-from cognite.fdm.general_domain.domain_model import DomainModel
-from cognite.fdm.misc import to_snake
+from cognite.dm_clients.domain_modeling.domain_model import DomainModel
+from cognite.dm_clients.misc import to_snake
 
 from ..custom_types import SCALARS
 from ..custom_types._scalars import *  # noqa
 
 DomainModelT = TypeVar("DomainModelT", bound=DomainModel)
 
 
@@ -29,34 +29,34 @@
     def _strawberry_schema(self) -> strawberry.Schema:
         if self._root_type is None:
             raise ValueError("define one of the schema types with @schema.register_type(root_type=True)")
         return strawberry.Schema(query=self._root_type, config=StrawberryConfig(auto_camel_case=False))
 
     def as_str(self) -> str:
         """
-        Removing things that FDM does not need:
+        Removing things that DM does not need:
          * `schema { query: ... }`
          * `scalar ...`
         """
         raw_schema = self._strawberry_schema().as_str()
         raw_lines = raw_schema.splitlines()
         # Loop over all the lines *backwards* and remove what we don't need.
-        fdm_lines: List[str] = []
+        dm_lines: List[str] = []
         for line in raw_lines[::-1]:
             if line.startswith("scalar "):
-                if fdm_lines:
-                    fdm_lines.pop()
+                if dm_lines:
+                    dm_lines.pop()
                 continue
             if line.startswith("schema {"):
-                fdm_lines.pop()
-                fdm_lines.pop()
-                fdm_lines.pop()
+                dm_lines.pop()
+                dm_lines.pop()
+                dm_lines.pop()
                 continue
-            fdm_lines.append(line)
-        return "\n".join(fdm_lines[::-1])
+            dm_lines.append(line)
+        return "\n".join(dm_lines[::-1])
 
     def register_type(
         self, lowercase_type_name: Optional[Union[str, Type[DomainModelT]]] = None, root_type: bool = False
     ):
         """
         Class decorator for schema types.
 
@@ -87,15 +87,15 @@
                     raise ValueError(f"Multiple types registered with root_type=True: {self._root_type_cls}, {cls}")
                 self._root_type_cls = cls
 
             return cls
 
         if isinstance(lowercase_type_name, type):
             # decorator was used without attributes, so lowercase_name is actually a DomainModel class
-            cls_ = cast(Type[DomainModelT], lowercase_type_name)
+            cls_ = lowercase_type_name
             lowercase_type_name = to_snake(cls_.__name__)
             return _register_type(cls_)
 
         return _register_type
 
     def _do_register(self, name: str, cls: Type[DomainModelT]) -> None:
         """Actually register a DomainModel with Strawberry."""
```

### Comparing `cognite_gql_pygen-0.1.2/cognite/fdm/main.py` & `cognite_gql_pygen-0.1.3/cognite/dm_clients/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     """
     _run(Path(__file__).parent / "bin/schema_render.sh")
 
 
 @schema_app.command()
 def publish():
     """
-    Uploads the GraphQL schema file to FDM.
+    Uploads the GraphQL schema file to DM.
     Takes configuration from config.yaml.
     """
     _run(Path(__file__).parent / "bin/schema_publish.sh")
 
 
 app.add_typer(schema_app, name="schema")
```

### Comparing `cognite_gql_pygen-0.1.2/cognite/fdm/misc.py` & `cognite_gql_pygen-0.1.3/cognite/dm_clients/misc.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.1.2/PKG-INFO` & `cognite_gql_pygen-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognite-gql-pygen
-Version: 0.1.2
+Version: 0.1.3
 Summary: Cognite graphQL Python generation SDK
 Author: Cognite
 Author-email: support@cognite.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -26,26 +26,26 @@
 Cognite GraphQL Python Generator
 ==========================
 [![build](https://github.com/cognitedata/cognite-gql-pygen/actions/workflows/release.yaml/badge.svg)](https://github.com/cognitedata/cognite-gql-pygen/actions/workflows/release.yaml)
 [![GitHub](https://img.shields.io/github/license/cognitedata/cognite-gql-pygen)](https://github.com/cognitedata/cognite-gql-pygen/blob/master/LICENSE)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
 
 This is the Cognite GraphQL Python Generator, `gqlpygen`, which is a CLI for automatically generating Python SDK code
-from `.graphql` to interact with Cognite Data Fusion's (CDF) Flexible Data Models (FDM). It also supports other cases,
+from `.graphql` to interact with Cognite Data Fusion's (CDF) Flexible Data Models (DM). It also supports other cases,
 such as generating `.graphql` from `pydantic` classes.
 
 **[DISCLAIMER!]** This project is in a highly experimental no guarantees are made for consistency between versions. The
 project may also become deprecated if the experimentation turns out to be a dead end.
 
 
-### FDM Non-GraphQl API
+### DM Non-GraphQl API
 
-This package also contains `cognite.fdm` which is a simplified wrapper for non-GraphQL endpoints in FDM API v3.
+This package also contains `cognite.dm_clients` which is a simplified wrapper for non-GraphQL endpoints in DM API v3.
 
-See [fdm/README.md](./fdm/README.md) for more details.
+See [dm_clients/README.md](cognite/dm_clients/README.md) for more details.
 
 ## Installation
 
 To install this package:
 ```bash
 $ pip install cognite-gql-pygen
 ```
```

