# Comparing `tmp/monarch_py-0.6.0.tar.gz` & `tmp/monarch_py-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monarch_py-0.6.0.tar", max compression
+gzip compressed data, was "monarch_py-0.6.1.tar", max compression
```

## Comparing `monarch_py-0.6.0.tar` & `monarch_py-0.6.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0      955 2023-04-10 15:50:37.713391 monarch_py-0.6.0/pyproject.toml
--rw-r--r--   0        0        0       77 2023-04-10 15:50:37.713391 monarch_py-0.6.0/src/monarch_py/__init__.py
--rw-r--r--   0        0        0     5764 2023-04-10 15:50:37.713391 monarch_py-0.6.0/src/monarch_py/cli.py
--rw-r--r--   0        0        0        0 2023-04-10 15:50:37.713391 monarch_py-0.6.0/src/monarch_py/datamodels/__init__.py
--rw-r--r--   0        0        0     6595 2023-04-10 15:50:37.713391 monarch_py-0.6.0/src/monarch_py/datamodels/model.py
--rw-r--r--   0        0        0     6272 2023-04-10 15:50:37.713391 monarch_py-0.6.0/src/monarch_py/datamodels/model.yaml
--rw-r--r--   0        0        0     3300 2023-04-10 15:50:37.713391 monarch_py-0.6.0/src/monarch_py/datamodels/solr.py
--rw-r--r--   0        0        0        0 2023-04-10 15:50:37.713391 monarch_py-0.6.0/src/monarch_py/implementations/__init__.py
--rw-r--r--   0        0        0        0 2023-04-10 15:50:37.713391 monarch_py-0.6.0/src/monarch_py/implementations/solr/__init__.py
--rw-r--r--   0        0        0    16877 2023-04-10 15:50:37.713391 monarch_py-0.6.0/src/monarch_py/implementations/solr/solr_implementation.py
--rw-r--r--   0        0        0        0 2023-04-10 15:50:37.713391 monarch_py-0.6.0/src/monarch_py/implementations/sql/__init__.py
--rw-r--r--   0        0        0     8913 2023-04-10 15:50:37.713391 monarch_py-0.6.0/src/monarch_py/implementations/sql/sql_implementation.py
--rw-r--r--   0        0        0        0 2023-04-10 15:50:37.713391 monarch_py-0.6.0/src/monarch_py/interfaces/__init__.py
--rw-r--r--   0        0        0     2345 2023-04-10 15:50:37.713391 monarch_py-0.6.0/src/monarch_py/interfaces/association_interface.py
--rw-r--r--   0        0        0      985 2023-04-10 15:50:37.713391 monarch_py-0.6.0/src/monarch_py/interfaces/entity_interface.py
--rw-r--r--   0        0        0      890 2023-04-10 15:50:37.713391 monarch_py-0.6.0/src/monarch_py/interfaces/query_interface.py
--rw-r--r--   0        0        0     3732 2023-04-10 15:50:37.713391 monarch_py-0.6.0/src/monarch_py/interfaces/search_interface.py
--rw-r--r--   0        0        0        0 2023-04-10 15:50:37.713391 monarch_py-0.6.0/src/monarch_py/service/__init__.py
--rw-r--r--   0        0        0     2051 2023-04-10 15:50:37.713391 monarch_py-0.6.0/src/monarch_py/service/solr_service.py
--rw-r--r--   0        0        0     8096 2023-04-10 15:50:37.713391 monarch_py-0.6.0/src/monarch_py/solr_cli.py
--rw-r--r--   0        0        0     3794 2023-04-10 15:50:37.713391 monarch_py-0.6.0/src/monarch_py/sql_cli.py
--rw-r--r--   0        0        0        0 2023-04-10 15:50:37.713391 monarch_py-0.6.0/src/monarch_py/utils/__init__.py
--rw-r--r--   0        0        0     3657 2023-04-10 15:50:37.713391 monarch_py-0.6.0/src/monarch_py/utils/solr_cli_utils.py
--rw-r--r--   0        0        0     4262 2023-04-10 15:50:37.713391 monarch_py-0.6.0/src/monarch_py/utils/utils.py
--rw-r--r--   0        0        0      711 1970-01-01 00:00:00.000000 monarch_py-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0      955 2023-04-11 00:16:06.217694 monarch_py-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0       77 2023-04-11 00:16:06.217694 monarch_py-0.6.1/src/monarch_py/__init__.py
+-rw-r--r--   0        0        0     5897 2023-04-11 00:16:06.217694 monarch_py-0.6.1/src/monarch_py/cli.py
+-rw-r--r--   0        0        0        0 2023-04-11 00:16:06.217694 monarch_py-0.6.1/src/monarch_py/datamodels/__init__.py
+-rw-r--r--   0        0        0     6595 2023-04-11 00:16:06.217694 monarch_py-0.6.1/src/monarch_py/datamodels/model.py
+-rw-r--r--   0        0        0     6272 2023-04-11 00:16:06.217694 monarch_py-0.6.1/src/monarch_py/datamodels/model.yaml
+-rw-r--r--   0        0        0     3300 2023-04-11 00:16:06.217694 monarch_py-0.6.1/src/monarch_py/datamodels/solr.py
+-rw-r--r--   0        0        0        0 2023-04-11 00:16:06.217694 monarch_py-0.6.1/src/monarch_py/implementations/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-11 00:16:06.217694 monarch_py-0.6.1/src/monarch_py/implementations/solr/__init__.py
+-rw-r--r--   0        0        0    15888 2023-04-11 00:16:06.217694 monarch_py-0.6.1/src/monarch_py/implementations/solr/solr_implementation.py
+-rw-r--r--   0        0        0        0 2023-04-11 00:16:06.217694 monarch_py-0.6.1/src/monarch_py/implementations/sql/__init__.py
+-rw-r--r--   0        0        0     8913 2023-04-11 00:16:06.217694 monarch_py-0.6.1/src/monarch_py/implementations/sql/sql_implementation.py
+-rw-r--r--   0        0        0        0 2023-04-11 00:16:06.217694 monarch_py-0.6.1/src/monarch_py/interfaces/__init__.py
+-rw-r--r--   0        0        0     2345 2023-04-11 00:16:06.217694 monarch_py-0.6.1/src/monarch_py/interfaces/association_interface.py
+-rw-r--r--   0        0        0      985 2023-04-11 00:16:06.217694 monarch_py-0.6.1/src/monarch_py/interfaces/entity_interface.py
+-rw-r--r--   0        0        0      890 2023-04-11 00:16:06.217694 monarch_py-0.6.1/src/monarch_py/interfaces/query_interface.py
+-rw-r--r--   0        0        0     3732 2023-04-11 00:16:06.217694 monarch_py-0.6.1/src/monarch_py/interfaces/search_interface.py
+-rw-r--r--   0        0        0        0 2023-04-11 00:16:06.217694 monarch_py-0.6.1/src/monarch_py/service/__init__.py
+-rw-r--r--   0        0        0     2051 2023-04-11 00:16:06.217694 monarch_py-0.6.1/src/monarch_py/service/solr_service.py
+-rw-r--r--   0        0        0     8269 2023-04-11 00:16:06.217694 monarch_py-0.6.1/src/monarch_py/solr_cli.py
+-rw-r--r--   0        0        0     3794 2023-04-11 00:16:06.217694 monarch_py-0.6.1/src/monarch_py/sql_cli.py
+-rw-r--r--   0        0        0        0 2023-04-11 00:16:06.217694 monarch_py-0.6.1/src/monarch_py/utils/__init__.py
+-rw-r--r--   0        0        0     3657 2023-04-11 00:16:06.217694 monarch_py-0.6.1/src/monarch_py/utils/solr_cli_utils.py
+-rw-r--r--   0        0        0     4262 2023-04-11 00:16:06.217694 monarch_py-0.6.1/src/monarch_py/utils/utils.py
+-rw-r--r--   0        0        0      711 1970-01-01 00:00:00.000000 monarch_py-0.6.1/PKG-INFO
```

### Comparing `monarch_py-0.6.0/pyproject.toml` & `monarch_py-0.6.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "monarch-py"
-version = "0.6.0"
+version = "0.6.1"
 description = "Monarch Initiative data access library"
 authors = [
     "Kevin Schaper <kevin@tislab.org>",
     "Glass Elsarboukh <glass@tislab.org>",
     "The Monarch Initiative <info@monarchinitiative.org>"
 ]
 packages = [
```

### Comparing `monarch_py-0.6.0/src/monarch_py/cli.py` & `monarch_py-0.6.1/src/monarch_py/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,14 +67,15 @@
 def associations(
     category: str = typer.Option(None, "--category", "-c"),
     subject: str = typer.Option(None, "--subject", "-s"),
     predicate: str = typer.Option(None, "--predicate", "-p"),
     object: str = typer.Option(None, "--object", "-o"),
     entity: str = typer.Option(None, "--entity", "-e"),
     between: str = typer.Option(None, "--between"),
+    direct: bool = typer.Option(False, "--direct"),
     association_label: str = typer.Option(None, "--label"),
     limit: int = typer.Option(20, "--limit", "-l"),
     offset: int = typer.Option(0, "--offset"),
     update: bool = typer.Option(
         False, "--update", "-u", help="Whether to re-download the Monarch KG"
     ),
     fmt: str = typer.Option(
@@ -92,14 +93,15 @@
         predicate: The predicate of the association
         subject: The subject of the association
         object: The object of the association
         entity: The subject or object of the association
         between: The subject and object of the association
         association_label: The label of the association
         limit: The number of associations to return
+        direct: Whether to exclude associations with subject/object as ancestors
         offset: The offset of the first association to be retrieved
         fmt: The format of the output (TSV, YAML, JSON)
         output: The path to the output file (stdout if not specified)
     """
     solr_cli.associations(**locals())
```

### Comparing `monarch_py-0.6.0/src/monarch_py/datamodels/model.py` & `monarch_py-0.6.1/src/monarch_py/datamodels/model.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.6.0/src/monarch_py/datamodels/model.yaml` & `monarch_py-0.6.1/src/monarch_py/datamodels/model.yaml`

 * *Files identical despite different names*

### Comparing `monarch_py-0.6.0/src/monarch_py/datamodels/solr.py` & `monarch_py-0.6.1/src/monarch_py/datamodels/solr.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.6.0/src/monarch_py/implementations/solr/solr_implementation.py` & `monarch_py-0.6.1/src/monarch_py/implementations/solr/solr_implementation.py`

 * *Files 6% similar despite different names*

```diff
@@ -74,31 +74,32 @@
     ####################################
 
     def get_associations(
         self,
         category: str = None,
         predicate: str = None,
         subject: str = None,
-        subject_closure: str = None,
         object: str = None,
+        subject_closure: str = None,
         object_closure: str = None,
         entity: str = None,
         between: str = None,
+        direct: bool = None,
         association_label: AssociationLabel = None,
         offset: int = 0,
         limit: int = 20,
     ) -> AssociationResults:
         """Retrieve paginated association records, with filter options
 
         Args:
             category (str, optional): Filter to only associations matching the specified category. Defaults to None.
             predicate (str, optional): Filter to only associations matching the specified predicate. Defaults to None.
             subject (str, optional): Filter to only associations matching the specified subject. Defaults to None.
-            subject_closure (str, optional): Filter to only associations with the specified term ID as an ancestor of the subject. Defaults to None
             object (str, optional): Filter to only associations matching the specified object. Defaults to None.
+            subject_closure (str, optional): Filter to only associations with the specified term ID as an ancestor of the subject. Defaults to None
             object_closure (str, optional): Filter to only associations with the specified term ID as an ancestor of the object. Defaults to None
             entity (str, optional): Filter to only associations where the specified entity is the subject or the object. Defaults to None.
             between (Tuple[str, str], optional): Filter to bi-directional associations between two entities.
             offset (int, optional): Result offset, for pagination. Defaults to 0.
             limit (int, optional): Limit results to specified number. Defaults to 20.
 
         Returns:
@@ -107,19 +108,20 @@
 
         solr = SolrService(base_url=self.base_url, core=core.ASSOCIATION)
 
         query = self._populate_association_query(
             category=category,
             predicate=predicate,
             subject=subject,
-            subject_closure=subject_closure,
             object=object,
+            subject_closure=subject_closure,
             object_closure=object_closure,
             entity=entity,
             between=between,
+            direct=direct,
             association_label=association_label,
             offset=offset,
             limit=limit,
         )
 
         query_result = solr.query(query)
         total = query_result.response.num_found
@@ -140,65 +142,55 @@
         return results
 
     def _populate_association_query(
         self,
         category: str = None,
         predicate: str = None,
         subject: str = None,
-        subject_closure: str = None,
         object: str = None,
+        subject_closure: str = None,
         object_closure: str = None,
         entity: str = None,
         between: str = None,
+        direct: bool = None,
         association_label: AssociationLabel = None,
         offset: int = 0,
         limit: int = 20,
     ) -> SolrQuery:
-        """
-        Populate a SolrQuery object with association filters
-        Args:
-            category (str, optional): Filter to only associations matching the specified category. Defaults to None.
-            predicate (str, optional): Filter to only associations matching the specified predicate. Defaults to None.
-            subject (str, optional): Filter to only associations matching the specified subject. Defaults to None.
-            subject_closure (str, optional): Filter to only associations with the specified term ID as an ancestor of the subject. Defaults to None
-            object (str, optional): Filter to only associations matching the specified object. Defaults to None.
-            object_closure (str, optional): Filter to only associations with the specified term ID as an ancestor of the object. Defaults to None
-            entity (str, optional): Filter to only associations where the specified entity is the subject or the object. Defaults to None.
-            between (Tuple[str, str], optional): Filter to bi-directional associations between two entities.
-            offset (int, optional): Result offset, for pagination. Defaults to 0.
-            limit (int, optional): Limit results to specified number. Defaults to 20.
+        """Populate a SolrQuery object with association filters"""
 
-        Returns:
-            SolrQuery: A populated SolrQuery object
-        """
         query = SolrQuery(start=offset, rows=limit)
 
+        subject_field = "subject" if direct else "subject_closure"
+        object_field = "object" if direct else "object_closure"
+            
+
         if category:
             query.add_field_filter_query("category", category)
         if predicate:
             query.add_field_filter_query("predicate", predicate)
         if subject:
-            query.add_field_filter_query("subject", subject)
+            query.add_field_filter_query(subject_field, subject)
         if subject_closure:
             query.add_field_filter_query("subject_closure", subject_closure)
         if object:
-            query.add_field_filter_query("object", object)
+            query.add_field_filter_query(object_field, object)
         if object_closure:
             query.add_field_filter_query("object_closure", object_closure)
         if between:
             # todo: handle error reporting / parsing, think about another way to pass this?
             b = between.split(",")
             e1 = escape(b[0])
             e2 = escape(b[1])
             query.add_filter_query(
-                f'(subject:"{e1}" AND object:"{e2}") OR (subject:"{e2}" AND object:"{e1}")'
+                f'({subject_field}:"{e1}" AND {object_field}:"{e2}") OR ({subject_field}:"{e2}" AND {object_field}:"{e1}")'
             )
         if entity:
             query.add_filter_query(
-                f'subject:"{escape(entity)}" OR object:"{escape(entity)}"'
+                f'{subject_field}:"{escape(entity)}" OR {object_field}:"{escape(entity)}"'
             )
         if association_label:
             query.add_filter_query(AssociationLabelQuery[association_label].value)
 
         return query
 
     ###############################
```

### Comparing `monarch_py-0.6.0/src/monarch_py/implementations/sql/sql_implementation.py` & `monarch_py-0.6.1/src/monarch_py/implementations/sql/sql_implementation.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -89,32 +89,32 @@
     ####################################
 
     def get_associations(
         self,
         category: str = None,
         predicate: str = None,
         subject: str = None,
-        subject_closure: str = None,
         object: str = None,
+        subject_closure: str = None,
         object_closure: str = None,
         entity: str = None,
         between: str = None,
         association_label: str = None,
         offset: int = 0,
         limit: int = 20,
         update: bool = False,
     ) -> AssociationResults:
         """Retrieve paginated association records, with filter options
 
         Args:
             category (str, optional): Filter to only associations matching the specified category. Defaults to None.
             predicate (str, optional): Filter to only associations matching the specified predicate. Defaults to None.
             subject (str, optional): Filter to only associations matching the specified subject. Defaults to None.
-            subject_closure (str, optional): Filter to only associations with the specified term ID as an ancestor of the subject. Defaults to None.
             object (str, optional): Filter to only associations matching the specified object. Defaults to None.
+            subject_closure (str, optional): Filter to only associations with the specified term ID as an ancestor of the subject. Defaults to None.
             object_closure (str, optional): Filter to only associations the specified term ID as an ancestor of the object. Defaults to None.
             entity (str, optional): Filter to only associations where the specified entity is the subject or the object. Defaults to None.
             between (Tuple[str, str], optional): Filter to bi-directional associations between two entities.
             association_label (str, optional): Filter to only associations matching the specified association label. Defaults to None.
             offset (int, optional): Result offset, for pagination. Defaults to 0.
             limit (int, optional): Limit results to specified number. Defaults to 20.
 
@@ -125,18 +125,18 @@
         clauses = []
         if category:
             clauses.append(f"category = '{category}'")
         if predicate:
             clauses.append(f"predicate = '{predicate}'")
         if subject:
             clauses.append(f"subject = '{subject}'")
-        if subject_closure:
-            clauses.append(f"subject_closure like '%{subject_closure}%'")
         if object:
             clauses.append(f"object = '{object}'")
+        if subject_closure:
+            clauses.append(f"subject_closure like '%{subject_closure}%'")
         if object_closure:
             clauses.append(f"object_closure like '%{object_closure}%'")
         if entity:
             clauses.append(f"subject = '{entity}' OR object = '{entity}'")
         if between:
             # todo: handle error reporting / parsing, think about another way to pass this?
             b = between.split(",")
```

### Comparing `monarch_py-0.6.0/src/monarch_py/interfaces/association_interface.py` & `monarch_py-0.6.1/src/monarch_py/interfaces/association_interface.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.6.0/src/monarch_py/interfaces/entity_interface.py` & `monarch_py-0.6.1/src/monarch_py/interfaces/entity_interface.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.6.0/src/monarch_py/interfaces/query_interface.py` & `monarch_py-0.6.1/src/monarch_py/interfaces/query_interface.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.6.0/src/monarch_py/interfaces/search_interface.py` & `monarch_py-0.6.1/src/monarch_py/interfaces/search_interface.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.6.0/src/monarch_py/service/solr_service.py` & `monarch_py-0.6.1/src/monarch_py/service/solr_service.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.6.0/src/monarch_py/solr_cli.py` & `monarch_py-0.6.1/src/monarch_py/solr_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,14 +86,15 @@
 def associations(
     category: str = typer.Option(None, "--category"),
     subject: str = typer.Option(None, "--subject"),
     predicate: str = typer.Option(None, "--predicate"),
     object: str = typer.Option(None, "--object"),
     entity: str = typer.Option(None, "--entity"),
     between: str = typer.Option(None, "--between"),
+    direct: bool = typer.Option(False, "--direct"),
     association_label: str = typer.Option(None, "--label"),
     limit: int = typer.Option(20, "--limit"),
     offset: int = typer.Option(0, "--offset"),
     update: bool = typer.Option(
         False, "--update", "-u", help="Whether to re-download the Monarch KG"
     ),
     fmt: str = typer.Option(
@@ -109,14 +110,15 @@
     Args:
         category (str, optional): The category of the association.
         subject (str, optional): The subject of the association.
         predicate (str, optional): The predicate of the association.
         object (str, optional): The object of the association.
         entity (str, optional): The subject or object of the association.
         between (str, optional): Two comma-separated entities to get bi-directional associations.
+        direct (bool, optional): Exclude associations with the specified subject and objects as ancestors. Default False
         association_label (str, optional): The association label of the association
         limit (int, optional): The number of associations to return. Default 20
         offset (int, optional): The offset of the first association to be retrieved. Default 0
         update (bool, optional): Whether to re-download the Monarch KG. Default False
         fmt (str): The format of the output (TSV, YAML, JSON). Default JSON
         output (str): The path to the output file. Default stdout
     """
```

### Comparing `monarch_py-0.6.0/src/monarch_py/sql_cli.py` & `monarch_py-0.6.1/src/monarch_py/sql_cli.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.6.0/src/monarch_py/utils/solr_cli_utils.py` & `monarch_py-0.6.1/src/monarch_py/utils/solr_cli_utils.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.6.0/src/monarch_py/utils/utils.py` & `monarch_py-0.6.1/src/monarch_py/utils/utils.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.6.0/PKG-INFO` & `monarch_py-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monarch-py
-Version: 0.6.0
+Version: 0.6.1
 Summary: Monarch Initiative data access library
 Author: Kevin Schaper
 Author-email: kevin@tislab.org
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

