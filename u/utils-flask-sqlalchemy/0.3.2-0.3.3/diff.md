# Comparing `tmp/utils-flask-sqlalchemy-0.3.2.tar.gz` & `tmp/utils-flask-sqlalchemy-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utils-flask-sqlalchemy-0.3.2.tar", last modified: Fri Mar  3 17:25:39 2023, max compression
+gzip compressed data, was "utils-flask-sqlalchemy-0.3.3.tar", last modified: Tue Apr 11 09:02:48 2023, max compression
```

## Comparing `utils-flask-sqlalchemy-0.3.2.tar` & `utils-flask-sqlalchemy-0.3.3.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 17:25:39.043055 utils-flask-sqlalchemy-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-03-03 17:25:29.000000 utils-flask-sqlalchemy-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-03-03 17:25:29.000000 utils-flask-sqlalchemy-0.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-03-03 17:25:39.043055 utils-flask-sqlalchemy-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-03-03 17:25:29.000000 utils-flask-sqlalchemy-0.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-03 17:25:29.000000 utils-flask-sqlalchemy-0.3.2/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-03-03 17:25:29.000000 utils-flask-sqlalchemy-0.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-03-03 17:25:29.000000 utils-flask-sqlalchemy-0.3.2/requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-03 17:25:39.043055 utils-flask-sqlalchemy-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-03-03 17:25:29.000000 utils-flask-sqlalchemy-0.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 17:25:39.039055 utils-flask-sqlalchemy-0.3.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 17:25:39.043055 utils-flask-sqlalchemy-0.3.2/src/utils_flask_sqla/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-03 17:25:29.000000 utils-flask-sqlalchemy-0.3.2/src/utils_flask_sqla/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9018 2023-03-03 17:25:29.000000 utils-flask-sqlalchemy-0.3.2/src/utils_flask_sqla/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-03-03 17:25:29.000000 utils-flask-sqlalchemy-0.3.2/src/utils_flask_sqla/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    11004 2023-03-03 17:25:29.000000 utils-flask-sqlalchemy-0.3.2/src/utils_flask_sqla/generic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 17:25:39.043055 utils-flask-sqlalchemy-0.3.2/src/utils_flask_sqla/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-03 17:25:29.000000 utils-flask-sqlalchemy-0.3.2/src/utils_flask_sqla/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-03-03 17:25:29.000000 utils-flask-sqlalchemy-0.3.2/src/utils_flask_sqla/migrations/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 17:25:39.043055 utils-flask-sqlalchemy-0.3.2/src/utils_flask_sqla/migrations/versions/
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-03-03 17:25:29.000000 utils-flask-sqlalchemy-0.3.2/src/utils_flask_sqla/migrations/versions/3842a6d800a0_sql_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-03 17:25:29.000000 utils-flask-sqlalchemy-0.3.2/src/utils_flask_sqla/migrations/versions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-03-03 17:25:29.000000 utils-flask-sqlalchemy-0.3.2/src/utils_flask_sqla/migrations/versions/ba207b468e31_create_fr_numeric_collation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-03-03 17:25:29.000000 utils-flask-sqlalchemy-0.3.2/src/utils_flask_sqla/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-03-03 17:25:29.000000 utils-flask-sqlalchemy-0.3.2/src/utils_flask_sqla/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    19523 2023-03-03 17:25:29.000000 utils-flask-sqlalchemy-0.3.2/src/utils_flask_sqla/serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 17:25:39.043055 utils-flask-sqlalchemy-0.3.2/src/utils_flask_sqla/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-03 17:25:29.000000 utils-flask-sqlalchemy-0.3.2/src/utils_flask_sqla/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-03-03 17:25:29.000000 utils-flask-sqlalchemy-0.3.2/src/utils_flask_sqla/tests/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-03-03 17:25:29.000000 utils-flask-sqlalchemy-0.3.2/src/utils_flask_sqla/tests/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    10979 2023-03-03 17:25:29.000000 utils-flask-sqlalchemy-0.3.2/src/utils_flask_sqla/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    24910 2023-03-03 17:25:29.000000 utils-flask-sqlalchemy-0.3.2/src/utils_flask_sqla/tests/test_serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-03-03 17:25:29.000000 utils-flask-sqlalchemy-0.3.2/src/utils_flask_sqla/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-03-03 17:25:29.000000 utils-flask-sqlalchemy-0.3.2/src/utils_flask_sqla/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 17:25:39.043055 utils-flask-sqlalchemy-0.3.2/src/utils_flask_sqlalchemy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-03-03 17:25:39.000000 utils-flask-sqlalchemy-0.3.2/src/utils_flask_sqlalchemy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-03-03 17:25:39.000000 utils-flask-sqlalchemy-0.3.2/src/utils_flask_sqlalchemy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-03 17:25:39.000000 utils-flask-sqlalchemy-0.3.2/src/utils_flask_sqlalchemy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-03-03 17:25:39.000000 utils-flask-sqlalchemy-0.3.2/src/utils_flask_sqlalchemy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-03-03 17:25:39.000000 utils-flask-sqlalchemy-0.3.2/src/utils_flask_sqlalchemy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-03 17:25:39.000000 utils-flask-sqlalchemy-0.3.2/src/utils_flask_sqlalchemy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-03-03 17:25:29.000000 utils-flask-sqlalchemy-0.3.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:02:48.387374 utils-flask-sqlalchemy-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-11 09:02:37.000000 utils-flask-sqlalchemy-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-11 09:02:37.000000 utils-flask-sqlalchemy-0.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-04-11 09:02:48.387374 utils-flask-sqlalchemy-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-04-11 09:02:37.000000 utils-flask-sqlalchemy-0.3.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-11 09:02:37.000000 utils-flask-sqlalchemy-0.3.3/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-11 09:02:37.000000 utils-flask-sqlalchemy-0.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-11 09:02:37.000000 utils-flask-sqlalchemy-0.3.3/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 09:02:48.387374 utils-flask-sqlalchemy-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-04-11 09:02:37.000000 utils-flask-sqlalchemy-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:02:48.383373 utils-flask-sqlalchemy-0.3.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:02:48.383373 utils-flask-sqlalchemy-0.3.3/src/utils_flask_sqla/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 09:02:37.000000 utils-flask-sqlalchemy-0.3.3/src/utils_flask_sqla/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9018 2023-04-11 09:02:37.000000 utils-flask-sqlalchemy-0.3.3/src/utils_flask_sqla/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-04-11 09:02:37.000000 utils-flask-sqlalchemy-0.3.3/src/utils_flask_sqla/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11004 2023-04-11 09:02:37.000000 utils-flask-sqlalchemy-0.3.3/src/utils_flask_sqla/generic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:02:48.383373 utils-flask-sqlalchemy-0.3.3/src/utils_flask_sqla/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 09:02:37.000000 utils-flask-sqlalchemy-0.3.3/src/utils_flask_sqla/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-04-11 09:02:37.000000 utils-flask-sqlalchemy-0.3.3/src/utils_flask_sqla/migrations/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:02:48.383373 utils-flask-sqlalchemy-0.3.3/src/utils_flask_sqla/migrations/versions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-04-11 09:02:37.000000 utils-flask-sqlalchemy-0.3.3/src/utils_flask_sqla/migrations/versions/3842a6d800a0_sql_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 09:02:37.000000 utils-flask-sqlalchemy-0.3.3/src/utils_flask_sqla/migrations/versions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-04-11 09:02:37.000000 utils-flask-sqlalchemy-0.3.3/src/utils_flask_sqla/migrations/versions/ba207b468e31_create_fr_numeric_collation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-04-11 09:02:37.000000 utils-flask-sqlalchemy-0.3.3/src/utils_flask_sqla/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-04-11 09:02:37.000000 utils-flask-sqlalchemy-0.3.3/src/utils_flask_sqla/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19519 2023-04-11 09:02:37.000000 utils-flask-sqlalchemy-0.3.3/src/utils_flask_sqla/serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:02:48.387374 utils-flask-sqlalchemy-0.3.3/src/utils_flask_sqla/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 09:02:37.000000 utils-flask-sqlalchemy-0.3.3/src/utils_flask_sqla/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-04-11 09:02:37.000000 utils-flask-sqlalchemy-0.3.3/src/utils_flask_sqla/tests/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-11 09:02:37.000000 utils-flask-sqlalchemy-0.3.3/src/utils_flask_sqla/tests/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11683 2023-04-11 09:02:37.000000 utils-flask-sqlalchemy-0.3.3/src/utils_flask_sqla/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24910 2023-04-11 09:02:37.000000 utils-flask-sqlalchemy-0.3.3/src/utils_flask_sqla/tests/test_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-04-11 09:02:37.000000 utils-flask-sqlalchemy-0.3.3/src/utils_flask_sqla/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-04-11 09:02:37.000000 utils-flask-sqlalchemy-0.3.3/src/utils_flask_sqla/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:02:48.387374 utils-flask-sqlalchemy-0.3.3/src/utils_flask_sqlalchemy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-04-11 09:02:48.000000 utils-flask-sqlalchemy-0.3.3/src/utils_flask_sqlalchemy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-04-11 09:02:48.000000 utils-flask-sqlalchemy-0.3.3/src/utils_flask_sqlalchemy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 09:02:48.000000 utils-flask-sqlalchemy-0.3.3/src/utils_flask_sqlalchemy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-11 09:02:48.000000 utils-flask-sqlalchemy-0.3.3/src/utils_flask_sqlalchemy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-11 09:02:48.000000 utils-flask-sqlalchemy-0.3.3/src/utils_flask_sqlalchemy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-11 09:02:48.000000 utils-flask-sqlalchemy-0.3.3/src/utils_flask_sqlalchemy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-11 09:02:37.000000 utils-flask-sqlalchemy-0.3.3/tox.ini
```

### Comparing `utils-flask-sqlalchemy-0.3.2/LICENSE` & `utils-flask-sqlalchemy-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `utils-flask-sqlalchemy-0.3.2/PKG-INFO` & `utils-flask-sqlalchemy-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utils-flask-sqlalchemy
-Version: 0.3.2
+Version: 0.3.3
 Summary: Python lib of tools for Flask and SQLAlchemy
 Home-page: https://github.com/PnX-SI/Utils-Flask-SQLAlchemy
 Maintainer: Parcs nationaux des Écrins et des Cévennes
 Maintainer-email: geonature@ecrins-parcnational.fr
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `utils-flask-sqlalchemy-0.3.2/README.md` & `utils-flask-sqlalchemy-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `utils-flask-sqlalchemy-0.3.2/setup.py` & `utils-flask-sqlalchemy-0.3.3/setup.py`

 * *Files identical despite different names*

### Comparing `utils-flask-sqlalchemy-0.3.2/src/utils_flask_sqla/commands.py` & `utils-flask-sqlalchemy-0.3.3/src/utils_flask_sqla/commands.py`

 * *Files identical despite different names*

### Comparing `utils-flask-sqlalchemy-0.3.2/src/utils_flask_sqla/errors.py` & `utils-flask-sqlalchemy-0.3.3/src/utils_flask_sqla/errors.py`

 * *Files identical despite different names*

### Comparing `utils-flask-sqlalchemy-0.3.2/src/utils_flask_sqla/generic.py` & `utils-flask-sqlalchemy-0.3.3/src/utils_flask_sqla/generic.py`

 * *Files identical despite different names*

### Comparing `utils-flask-sqlalchemy-0.3.2/src/utils_flask_sqla/migrations/utils.py` & `utils-flask-sqlalchemy-0.3.3/src/utils_flask_sqla/migrations/utils.py`

 * *Files identical despite different names*

### Comparing `utils-flask-sqlalchemy-0.3.2/src/utils_flask_sqla/migrations/versions/3842a6d800a0_sql_utils.py` & `utils-flask-sqlalchemy-0.3.3/src/utils_flask_sqla/migrations/versions/3842a6d800a0_sql_utils.py`

 * *Files identical despite different names*

### Comparing `utils-flask-sqlalchemy-0.3.2/src/utils_flask_sqla/migrations/versions/ba207b468e31_create_fr_numeric_collation.py` & `utils-flask-sqlalchemy-0.3.3/src/utils_flask_sqla/migrations/versions/ba207b468e31_create_fr_numeric_collation.py`

 * *Files identical despite different names*

### Comparing `utils-flask-sqlalchemy-0.3.2/src/utils_flask_sqla/response.py` & `utils-flask-sqlalchemy-0.3.3/src/utils_flask_sqla/response.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,14 @@
         filename, data, columns, separator = res
         return to_csv_resp(filename, data, columns, separator)
 
     return _csv_resp
 
 
 def to_csv_resp(filename, data, columns, separator=";"):
-
     headers = Headers()
     headers.add("Content-Type", "text/plain")
     headers.add("Content-Disposition", "attachment", filename="export_%s.csv" % filename)
     out = generate_csv_content(columns, data, separator)
     return Response(out, headers=headers)
```

### Comparing `utils-flask-sqlalchemy-0.3.2/src/utils_flask_sqla/schema.py` & `utils-flask-sqlalchemy-0.3.3/src/utils_flask_sqla/schema.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,14 +19,20 @@
             # excluded fields at meta level are not even generated by auto-schema
             if field is None:
                 continue
             if isinstance(field, Nested):
                 nested_fields.add(name)
             elif field.metadata.get("exclude", False):
                 excluded_fields.add(name)
+            elif (
+                hasattr(self.opts, "model")
+                and hasattr(self.opts.model.__mapper__.column_attrs, name)
+                and getattr(self.opts.model.__mapper__.column_attrs, name).deferred
+            ):
+                excluded_fields.add(name)
             else:
                 included_fields.add(name)
 
         only = kwargs.pop("only", None)
         only = set(only) if only is not None else set()
         additional_fields = {field[1:] for field in only if field.startswith("+")}
         only = {field[1:] if field.startswith("+") else field for field in only}
```

### Comparing `utils-flask-sqlalchemy-0.3.2/src/utils_flask_sqla/serializers.py` & `utils-flask-sqlalchemy-0.3.3/src/utils_flask_sqla/serializers.py`

 * *Files 1% similar despite different names*

```diff
@@ -365,16 +365,15 @@
             # si non recursif, on ne traite pas les relationship
             if not recursif:
                 return self
 
             # gestion des relationships
             frel = get_cls_db_relationships()
 
-            for (rel, uselist, Model) in frel:
-
+            for rel, uselist, Model in frel:
                 if rel not in dict_in:
                     continue
 
                 values = dict_in.get(rel)
                 if not values:
                     # check if None or {}
                     setattr(self, rel, [] if uselist else None)
@@ -405,15 +404,14 @@
                     getattr(Model, id_field_name).in_(ids)
                 ).all()
 
                 # resul
                 v_obj = []
 
                 for data in values:
-
                     id_value = data.get(id_field_name)
 
                     # si id_value est null
                     # creation -> on supprime id_value
                     if not id_value:
                         data.pop(id_field_name)
```

### Comparing `utils-flask-sqlalchemy-0.3.2/src/utils_flask_sqla/tests/fixtures.py` & `utils-flask-sqlalchemy-0.3.3/src/utils_flask_sqla/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `utils-flask-sqlalchemy-0.3.2/src/utils_flask_sqla/tests/test_schema.py` & `utils-flask-sqlalchemy-0.3.3/src/utils_flask_sqla/tests/test_schema.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from unittest import TestCase
 
 import marshmallow as ma
 from marshmallow.fields import Nested
 from marshmallow_sqlalchemy import SQLAlchemyAutoSchema, auto_field
 from sqlalchemy import Column, Integer, String, ForeignKey
-from sqlalchemy.orm import relationship
+from sqlalchemy.orm import relationship, deferred
 from sqlalchemy.ext.hybrid import hybrid_property
 from flask_sqlalchemy import SQLAlchemy
 
 from utils_flask_sqla.schema import SmartRelationshipsMixin
 
 
 db = SQLAlchemy()
@@ -384,7 +384,25 @@
             {
                 "child": {
                     "a": "A",
                     "b": "B",
                 },
             },
         )
+
+    def test_deferred_field(self):
+        class DeferredModel(db.Model):
+            pk = db.Column(db.Integer, primary_key=True)
+            a = db.Column(db.String)
+            b = deferred(db.Column(db.String))
+
+        class DeferredSchema(SmartRelationshipsMixin, SQLAlchemyAutoSchema):
+            class Meta:
+                model = DeferredModel
+
+        d = DeferredModel(pk=1, a="A", b="B")
+
+        TestCase().assertDictEqual(DeferredSchema().dump(d), {"pk": 1, "a": "A"})
+        TestCase().assertDictEqual(
+            DeferredSchema(only=["+b"]).dump(d), {"pk": 1, "a": "A", "b": "B"}
+        )
+        TestCase().assertDictEqual(DeferredSchema(only=["b"]).dump(d), {"b": "B"})
```

### Comparing `utils-flask-sqlalchemy-0.3.2/src/utils_flask_sqla/tests/test_serializers.py` & `utils-flask-sqlalchemy-0.3.3/src/utils_flask_sqla/tests/test_serializers.py`

 * *Files identical despite different names*

### Comparing `utils-flask-sqlalchemy-0.3.2/src/utils_flask_sqla/tests/utils.py` & `utils-flask-sqlalchemy-0.3.3/src/utils_flask_sqla/tests/utils.py`

 * *Files identical despite different names*

### Comparing `utils-flask-sqlalchemy-0.3.2/src/utils_flask_sqla/utils.py` & `utils-flask-sqlalchemy-0.3.3/src/utils_flask_sqla/utils.py`

 * *Files identical despite different names*

### Comparing `utils-flask-sqlalchemy-0.3.2/src/utils_flask_sqlalchemy.egg-info/PKG-INFO` & `utils-flask-sqlalchemy-0.3.3/src/utils_flask_sqlalchemy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utils-flask-sqlalchemy
-Version: 0.3.2
+Version: 0.3.3
 Summary: Python lib of tools for Flask and SQLAlchemy
 Home-page: https://github.com/PnX-SI/Utils-Flask-SQLAlchemy
 Maintainer: Parcs nationaux des Écrins et des Cévennes
 Maintainer-email: geonature@ecrins-parcnational.fr
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `utils-flask-sqlalchemy-0.3.2/src/utils_flask_sqlalchemy.egg-info/SOURCES.txt` & `utils-flask-sqlalchemy-0.3.3/src/utils_flask_sqlalchemy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

