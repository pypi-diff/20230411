# Comparing `tmp/cognite_gql_pygen-0.1.1.tar.gz` & `tmp/cognite_gql_pygen-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_gql_pygen-0.1.1.tar", max compression
+gzip compressed data, was "cognite_gql_pygen-0.1.2.tar", max compression
```

## Comparing `cognite_gql_pygen-0.1.1.tar` & `cognite_gql_pygen-0.1.2.tar`

### file list

```diff
@@ -1,28 +1,32 @@
--rw-r--r--   0        0        0    11349 2023-03-31 13:27:26.924420 cognite_gql_pygen-0.1.1/LICENSE
--rw-r--r--   0        0        0     1758 2023-03-31 13:27:26.924420 cognite_gql_pygen-0.1.1/README.md
--rw-r--r--   0        0        0     8174 2023-03-31 13:27:26.924420 cognite_gql_pygen-0.1.1/cognite/fdm/README.md
--rw-r--r--   0        0        0        0 2023-03-31 13:27:26.924420 cognite_gql_pygen-0.1.1/cognite/fdm/__init__.py
--rw-r--r--   0        0        0      230 2023-03-31 13:27:26.924420 cognite_gql_pygen-0.1.1/cognite/fdm/bin/_functions.sh
--rwxr-xr-x   0        0        0      569 2023-03-31 13:27:26.924420 cognite_gql_pygen-0.1.1/cognite/fdm/bin/cdf_signin.sh
--rwxr-xr-x   0        0        0      377 2023-03-31 13:27:26.924420 cognite_gql_pygen-0.1.1/cognite/fdm/bin/schema_publish.sh
--rwxr-xr-x   0        0        0      443 2023-03-31 13:27:26.924420 cognite_gql_pygen-0.1.1/cognite/fdm/bin/schema_render.sh
--rw-r--r--   0        0        0      170 2023-03-31 13:27:26.924420 cognite_gql_pygen-0.1.1/cognite/fdm/cdf/__init__.py
--rw-r--r--   0        0        0    19044 2023-03-31 13:27:26.928420 cognite_gql_pygen-0.1.1/cognite/fdm/cdf/client_fdm_v3.py
--rw-r--r--   0        0        0     3911 2023-03-31 13:27:26.928420 cognite_gql_pygen-0.1.1/cognite/fdm/cdf/data_classes_fdm_v3.py
--rw-r--r--   0        0        0     2621 2023-03-31 13:27:26.928420 cognite_gql_pygen-0.1.1/cognite/fdm/cdf/get_client.py
--rw-r--r--   0        0        0      218 2023-03-31 13:27:26.928420 cognite_gql_pygen-0.1.1/cognite/fdm/config.example.yaml
--rw-r--r--   0        0        0      691 2023-03-31 13:27:26.928420 cognite_gql_pygen-0.1.1/cognite/fdm/config.py
--rw-r--r--   0        0        0      196 2023-03-31 13:27:26.928420 cognite_gql_pygen-0.1.1/cognite/fdm/general_domain/__init__.py
--rw-r--r--   0        0        0     6191 2023-03-31 13:27:26.928420 cognite_gql_pygen-0.1.1/cognite/fdm/general_domain/domain_client.py
--rw-r--r--   0        0        0     3043 2023-03-31 13:27:26.928420 cognite_gql_pygen-0.1.1/cognite/fdm/general_domain/domain_model.py
--rw-r--r--   0        0        0    15849 2023-03-31 13:27:26.928420 cognite_gql_pygen-0.1.1/cognite/fdm/general_domain/domain_model_api.py
--rw-r--r--   0        0        0     3597 2023-03-31 13:27:26.928420 cognite_gql_pygen-0.1.1/cognite/fdm/general_domain/relationship_api.py
--rw-r--r--   0        0        0     3929 2023-03-31 13:27:26.928420 cognite_gql_pygen-0.1.1/cognite/fdm/general_domain/schema.py
--rw-r--r--   0        0        0      869 2023-03-31 13:27:26.928420 cognite_gql_pygen-0.1.1/cognite/fdm/main.py
--rw-r--r--   0        0        0     1423 2023-03-31 13:27:26.928420 cognite_gql_pygen-0.1.1/cognite/fdm/misc.py
--rw-r--r--   0        0        0        0 2023-03-31 13:27:26.928420 cognite_gql_pygen-0.1.1/cognite/fdm/py.typed
--rw-r--r--   0        0        0       76 2023-03-31 13:27:26.928420 cognite_gql_pygen-0.1.1/cognite/gqlpygen/__init__.py
--rw-r--r--   0        0        0      300 2023-03-31 13:27:26.928420 cognite_gql_pygen-0.1.1/cognite/gqlpygen/main.py
--rw-r--r--   0        0        0       22 2023-03-31 13:27:26.928420 cognite_gql_pygen-0.1.1/cognite/gqlpygen/version.py
--rw-r--r--   0        0        0     1225 2023-03-31 13:27:26.928420 cognite_gql_pygen-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2662 1970-01-01 00:00:00.000000 cognite_gql_pygen-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11349 2023-04-11 11:54:24.795409 cognite_gql_pygen-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1758 2023-04-11 11:54:24.795409 cognite_gql_pygen-0.1.2/README.md
+-rw-r--r--   0        0        0     8174 2023-04-11 11:54:24.795409 cognite_gql_pygen-0.1.2/cognite/fdm/README.md
+-rw-r--r--   0        0        0        0 2023-04-11 11:54:24.795409 cognite_gql_pygen-0.1.2/cognite/fdm/__init__.py
+-rw-r--r--   0        0        0      230 2023-04-11 11:54:24.795409 cognite_gql_pygen-0.1.2/cognite/fdm/bin/_functions.sh
+-rwxr-xr-x   0        0        0      572 2023-04-11 11:54:24.795409 cognite_gql_pygen-0.1.2/cognite/fdm/bin/cdf_signin.sh
+-rwxr-xr-x   0        0        0      379 2023-04-11 11:54:24.795409 cognite_gql_pygen-0.1.2/cognite/fdm/bin/schema_publish.sh
+-rwxr-xr-x   0        0        0      321 2023-04-11 11:54:24.795409 cognite_gql_pygen-0.1.2/cognite/fdm/bin/schema_render.sh
+-rw-r--r--   0        0        0      170 2023-04-11 11:54:24.795409 cognite_gql_pygen-0.1.2/cognite/fdm/cdf/__init__.py
+-rw-r--r--   0        0        0    19044 2023-04-11 11:54:24.799409 cognite_gql_pygen-0.1.2/cognite/fdm/cdf/client_fdm_v3.py
+-rw-r--r--   0        0        0     3911 2023-04-11 11:54:24.799409 cognite_gql_pygen-0.1.2/cognite/fdm/cdf/data_classes_fdm_v3.py
+-rw-r--r--   0        0        0     2621 2023-04-11 11:54:24.799409 cognite_gql_pygen-0.1.2/cognite/fdm/cdf/get_client.py
+-rw-r--r--   0        0        0      218 2023-04-11 11:54:24.799409 cognite_gql_pygen-0.1.2/cognite/fdm/config.example.yaml
+-rw-r--r--   0        0        0      695 2023-04-11 11:54:24.799409 cognite_gql_pygen-0.1.2/cognite/fdm/config.py
+-rw-r--r--   0        0        0      192 2023-04-11 11:54:24.799409 cognite_gql_pygen-0.1.2/cognite/fdm/custom_types/__init__.py
+-rw-r--r--   0        0        0      236 2023-04-11 11:54:24.799409 cognite_gql_pygen-0.1.2/cognite/fdm/custom_types/_scalars.py
+-rw-r--r--   0        0        0      978 2023-04-11 11:54:24.799409 cognite_gql_pygen-0.1.2/cognite/fdm/custom_types/jsonobject.py
+-rw-r--r--   0        0        0     4948 2023-04-11 11:54:24.799409 cognite_gql_pygen-0.1.2/cognite/fdm/custom_types/timestamp.py
+-rw-r--r--   0        0        0      196 2023-04-11 11:54:24.799409 cognite_gql_pygen-0.1.2/cognite/fdm/general_domain/__init__.py
+-rw-r--r--   0        0        0     6191 2023-04-11 11:54:24.799409 cognite_gql_pygen-0.1.2/cognite/fdm/general_domain/domain_client.py
+-rw-r--r--   0        0        0     3043 2023-04-11 11:54:24.799409 cognite_gql_pygen-0.1.2/cognite/fdm/general_domain/domain_model.py
+-rw-r--r--   0        0        0    15849 2023-04-11 11:54:24.799409 cognite_gql_pygen-0.1.2/cognite/fdm/general_domain/domain_model_api.py
+-rw-r--r--   0        0        0     3597 2023-04-11 11:54:24.799409 cognite_gql_pygen-0.1.2/cognite/fdm/general_domain/relationship_api.py
+-rw-r--r--   0        0        0     6848 2023-04-11 11:54:24.799409 cognite_gql_pygen-0.1.2/cognite/fdm/general_domain/schema.py
+-rw-r--r--   0        0        0      869 2023-04-11 11:54:24.799409 cognite_gql_pygen-0.1.2/cognite/fdm/main.py
+-rw-r--r--   0        0        0     1423 2023-04-11 11:54:24.799409 cognite_gql_pygen-0.1.2/cognite/fdm/misc.py
+-rw-r--r--   0        0        0        0 2023-04-11 11:54:24.799409 cognite_gql_pygen-0.1.2/cognite/fdm/py.typed
+-rw-r--r--   0        0        0       76 2023-04-11 11:54:24.799409 cognite_gql_pygen-0.1.2/cognite/gqlpygen/__init__.py
+-rw-r--r--   0        0        0      300 2023-04-11 11:54:24.799409 cognite_gql_pygen-0.1.2/cognite/gqlpygen/main.py
+-rw-r--r--   0        0        0       22 2023-04-11 11:54:24.799409 cognite_gql_pygen-0.1.2/cognite/gqlpygen/version.py
+-rw-r--r--   0        0        0     1282 2023-04-11 11:54:24.799409 cognite_gql_pygen-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2662 1970-01-01 00:00:00.000000 cognite_gql_pygen-0.1.2/PKG-INFO
```

### Comparing `cognite_gql_pygen-0.1.1/LICENSE` & `cognite_gql_pygen-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.1.1/README.md` & `cognite_gql_pygen-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.1.1/cognite/fdm/README.md` & `cognite_gql_pygen-0.1.2/cognite/fdm/README.md`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.1.1/cognite/fdm/bin/cdf_signin.sh` & `cognite_gql_pygen-0.1.2/cognite/fdm/bin/cdf_signin.sh`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 #!/bin/bash
 set -e
 
-. fdm/bin/_functions.sh "$1"
+. "${0%/*}/_functions.sh" "$1"
+
 
 CDF_CLUSTER=$(cat "$CONFIG" | extract 'cdf_cluster')
 PROJECT=$(cat "$CONFIG" | extract 'project')
 TENANT_ID=$(cat "$CONFIG" | extract 'tenant_id')
 CLIENT_ID=$(cat "$CONFIG" | extract 'client_id')
 CLIENT_SECRET=$(cat "$CONFIG" | extract 'client_secret')
```

### Comparing `cognite_gql_pygen-0.1.1/cognite/fdm/cdf/client_fdm_v3.py` & `cognite_gql_pygen-0.1.2/cognite/fdm/cdf/client_fdm_v3.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.1.1/cognite/fdm/cdf/data_classes_fdm_v3.py` & `cognite_gql_pygen-0.1.2/cognite/fdm/cdf/data_classes_fdm_v3.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.1.1/cognite/fdm/cdf/get_client.py` & `cognite_gql_pygen-0.1.2/cognite/fdm/cdf/get_client.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.1.1/cognite/fdm/config.py` & `cognite_gql_pygen-0.1.2/cognite/fdm/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,8 +28,8 @@
     with open(CONFIG_FILE) as f:
         CONFIG = yaml.safe_load(f)
 except FileNotFoundError:
     if "pytest" in sys.modules:
         CONFIG = test_config
     else:
         logger.error("config.yaml not found. Please see README.md to setup information.")
-        exit(1)
+        sys.exit(1)
```

### Comparing `cognite_gql_pygen-0.1.1/cognite/fdm/general_domain/domain_client.py` & `cognite_gql_pygen-0.1.2/cognite/fdm/general_domain/domain_client.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.1.1/cognite/fdm/general_domain/domain_model.py` & `cognite_gql_pygen-0.1.2/cognite/fdm/general_domain/domain_model.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.1.1/cognite/fdm/general_domain/domain_model_api.py` & `cognite_gql_pygen-0.1.2/cognite/fdm/general_domain/domain_model_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -239,15 +239,15 @@
 
     def retrieve(self, external_ids: Iterable[str]) -> List[DomainModelT]:
         cached_items, uncached_external_ids = self._get_from_cache(external_ids)
         retrieved_nodes = self.nodes_api.retrieve(self.view, uncached_external_ids)
         retrieved_instances = self._retrieve_full(retrieved_nodes)
         return [*cached_items, *retrieved_instances]  # TODO maintain order according to external_ids
 
-    # TODO maybe implement delete_by_ext_ids? Note delete_realted_items.
+    # TODO maybe implement delete_by_ext_ids? Note delete_related_items.
 
     def delete(self, items: Iterable[DomainModelT], delete_related_items: bool = False) -> None:
         if not items:
             return
         # Delete all edges that start on items.
         # Note: edges that _end_ on this node will remain unaffected!
         edges = self.relationships.list(from_ext_ids=[item.externalId for item in items if item.externalId])
```

### Comparing `cognite_gql_pygen-0.1.1/cognite/fdm/general_domain/relationship_api.py` & `cognite_gql_pygen-0.1.2/cognite/fdm/general_domain/relationship_api.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.1.1/cognite/fdm/main.py` & `cognite_gql_pygen-0.1.2/cognite/fdm/main.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.1.1/cognite/fdm/misc.py` & `cognite_gql_pygen-0.1.2/cognite/fdm/misc.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.1.1/pyproject.toml` & `cognite_gql_pygen-0.1.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cognite-gql-pygen"
-version = "0.1.1"
+version = "0.1.2"
 description = "Cognite graphQL Python generation SDK"
 readme = "README.md"
 authors = ["Cognite <support@cognite.com>"]
 
 packages = [{ include="cognite", from="." }]
 
 [tool.black]
@@ -44,10 +44,13 @@
 pre-commit = "*"
 toml = "*"
 python-dotenv = "*"
 pytest = "*"
 pytest-cov = "*"
 pytest-mock = "*"
 
+[tool.pytest.ini_options]
+addopts = "--doctest-modules"
+
 [build-system]
 requires = ["poetry>=1.0"]
 build-backend = "poetry.masonry.api"
```

### Comparing `cognite_gql_pygen-0.1.1/PKG-INFO` & `cognite_gql_pygen-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognite-gql-pygen
-Version: 0.1.1
+Version: 0.1.2
 Summary: Cognite graphQL Python generation SDK
 Author: Cognite
 Author-email: support@cognite.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

